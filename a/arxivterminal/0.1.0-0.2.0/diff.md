# Comparing `tmp/arxivterminal-0.1.0.tar.gz` & `tmp/arxivterminal-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arxivterminal-0.1.0.tar", max compression
+gzip compressed data, was "arxivterminal-0.2.0.tar", max compression
```

## Comparing `arxivterminal-0.1.0.tar` & `arxivterminal-0.2.0.tar`

### file list

```diff
@@ -1,11 +1,13 @@
--rw-r--r--   0        0        0    35149 2023-04-15 01:36:31.930555 arxivterminal-0.1.0/LICENSE
--rw-r--r--   0        0        0     1648 2023-04-15 04:01:25.324051 arxivterminal-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-04-10 04:49:57.408686 arxivterminal-0.1.0/arxivterminal/__init__.py
--rw-r--r--   0        0        0     2929 2023-04-15 03:47:50.900488 arxivterminal-0.1.0/arxivterminal/cli.py
--rw-r--r--   0        0        0     8910 2023-04-15 01:16:02.093725 arxivterminal-0.1.0/arxivterminal/db.py
--rw-r--r--   0        0        0     2171 2023-04-15 01:16:02.874162 arxivterminal-0.1.0/arxivterminal/fetch.py
--rw-r--r--   0        0        0      322 2023-04-15 01:16:03.622287 arxivterminal-0.1.0/arxivterminal/models.py
--rw-r--r--   0        0        0     2564 2023-04-15 01:17:16.487366 arxivterminal-0.1.0/arxivterminal/output.py
--rw-r--r--   0        0        0      735 2023-04-15 03:50:40.329059 arxivterminal-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2695 1970-01-01 00:00:00.000000 arxivterminal-0.1.0/setup.py
--rw-r--r--   0        0        0     2538 1970-01-01 00:00:00.000000 arxivterminal-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-15 01:36:31.930555 arxivterminal-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3229 2023-04-15 07:14:41.405271 arxivterminal-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-15 06:44:50.310227 arxivterminal-0.2.0/arxivterminal/__init__.py
+-rw-r--r--   0        0        0     3864 2023-04-15 07:14:41.405840 arxivterminal-0.2.0/arxivterminal/cli.py
+-rw-r--r--   0        0        0      349 2023-04-15 07:14:41.406231 arxivterminal-0.2.0/arxivterminal/constants.py
+-rw-r--r--   0        0        0     9486 2023-04-15 07:14:41.406551 arxivterminal-0.2.0/arxivterminal/db.py
+-rw-r--r--   0        0        0     2171 2023-04-15 06:44:47.860863 arxivterminal-0.2.0/arxivterminal/fetch.py
+-rw-r--r--   0        0        0     5222 2023-04-15 07:14:41.406823 arxivterminal-0.2.0/arxivterminal/ml.py
+-rw-r--r--   0        0        0      322 2023-04-15 01:16:03.622287 arxivterminal-0.2.0/arxivterminal/models.py
+-rw-r--r--   0        0        0     3269 2023-04-15 07:14:41.407077 arxivterminal-0.2.0/arxivterminal/output.py
+-rw-r--r--   0        0        0      772 2023-04-15 07:14:41.408183 arxivterminal-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4346 1970-01-01 00:00:00.000000 arxivterminal-0.2.0/setup.py
+-rw-r--r--   0        0        0     4213 1970-01-01 00:00:00.000000 arxivterminal-0.2.0/PKG-INFO
```

### Comparing `arxivterminal-0.1.0/LICENSE` & `arxivterminal-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `arxivterminal-0.1.0/arxivterminal/db.py` & `arxivterminal-0.2.0/arxivterminal/db.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 import sqlite3
 from datetime import datetime
-from typing import List, Tuple
+from typing import List, Optional, Tuple
 
 from arxivterminal.models import ArxivPaper, ArxivStats
 
 
 class ArxivDatabase:
     def __init__(self, database_path: str):
         """
@@ -139,42 +139,55 @@
             # Commit the changes to the database and close the connection
             conn.commit()
 
         # Log the number of papers inserted and updated
         logging.info(f"Inserted {num_inserted} papers")
         logging.info(f"Updated {num_updated} papers")
 
-    def get_papers(self, published_after: datetime) -> List[ArxivPaper]:
+    def get_papers(
+        self, published_after: Optional[datetime] = None
+    ) -> List[ArxivPaper]:
         """
         Retrieve papers from the database that were published after a specified date.
 
         Parameters
         ----------
-        published_after : datetime
+        published_after : datetime, optional
             A datetime object representing the lower bound of the publication date for retrieved papers.
+            If None, then no filters are applied and all papers are returned.
 
         Returns
         -------
         List[ArxivPaper]
             A list of ArxivPaper objects that match the specified criteria.
         """
         # Connect to the database
         with sqlite3.connect(self.database_path) as conn:
             cursor = conn.cursor()
 
-            # Query the database for papers published after the specified date
-            cursor.execute(
+            if published_after is not None:
+                # Query the database for papers published after the specified date
+                cursor.execute(
+                    """
+                    SELECT entry_id, updated, published, title, summary, authors, categories
+                    FROM papers
+                    WHERE published >= ?
+                    ORDER BY published ASC
+                """,
+                    (published_after.isoformat(),),
+                )
+            else:
+                # Query the database for papers published after the specified date
+                cursor.execute(
+                    """
+                    SELECT entry_id, updated, published, title, summary, authors, categories
+                    FROM papers
+                    ORDER BY published ASC
                 """
-                SELECT entry_id, updated, published, title, summary, authors, categories
-                FROM papers
-                WHERE published >= ?
-                ORDER BY published ASC
-            """,
-                (published_after.isoformat(),),
-            )
+                )
 
             # Parse the results into ArxivPaper objects
             papers = []
             for row in cursor.fetchall():
                 paper = self.convert_to_paper(row)
                 papers.append(paper)
```

### Comparing `arxivterminal-0.1.0/arxivterminal/fetch.py` & `arxivterminal-0.2.0/arxivterminal/fetch.py`

 * *Files identical despite different names*

### Comparing `arxivterminal-0.1.0/arxivterminal/output.py` & `arxivterminal-0.2.0/arxivterminal/output.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,31 +1,40 @@
 from typing import List
 
 from termcolor import colored
 
-from arxivterminal.db import ArxivStats
+from arxivterminal.constants import DATABASE_PATH, MODEL_PATH
+from arxivterminal.db import ArxivDatabase, ArxivStats
 from arxivterminal.fetch import ArxivPaper
+from arxivterminal.ml import LsaDocumentSearch
 
 
-def print_papers(papers: List[ArxivPaper]):
+class ExitAppException(Exception):
+    pass
+
+
+def print_papers(papers: List[ArxivPaper], show_dates: bool = True):
     """
     Print a list of Arxiv papers and their publication date in a formatted manner.
 
     Parameters
     ----------
     papers : List[ArxivPaper]
         A list of ArxivPaper objects to be printed.
+    show_dates: bool
+        If true, then the publish date of the paper is shown. Otherwise, date headers are
+        omitted.
     """
     current_date = None
     total_papers = len(papers)
 
     while True:
         for i, paper in enumerate(papers):
             paper_date = paper.published.date()
-            if paper_date != current_date:
+            if (paper_date != current_date) and show_dates:
                 print(colored(f"\n{paper_date}", "cyan"))
                 print(colored("".join(["-"] * 10), "cyan"))
                 current_date = paper_date
             inverted_line_number = total_papers - i
             print(f"{colored(inverted_line_number, 'yellow')}. {paper.title}")
 
         # Get the line number from the user
@@ -43,19 +52,25 @@
                     print(
                         f"\n{colored('Abstract:', 'cyan')} {selected_paper.summary}\n"
                     )
                 else:
                     print("Invalid line number. Please try again.")
             except ValueError:
                 if user_input.lower() == "q":
-                    return
+                    raise ExitAppException
+                elif user_input.lower() == "s":
+                    db = ArxivDatabase(str(DATABASE_PATH))
+                    lsa = LsaDocumentSearch(str(MODEL_PATH))
+                    search_results = lsa.search(db, selected_paper.summary)
+                    print_papers(search_results, show_dates=False)
+
                 print("Invalid input. Please try again.")
 
             user_input = input(
-                "Enter the line number to show the full abstract, 'b' to go back, or 'q' to quit: "
+                "Enter the line number to show the full abstract, 'b' to go back, 's' to search similar, or 'q' to quit: "  # noqa: E501
             )
 
 
 def print_stats(stats: List[ArxivStats]):
     """
     Print the count of Arxiv papers by their publication date in a formatted manner.
```

### Comparing `arxivterminal-0.1.0/pyproject.toml` & `arxivterminal-0.2.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 [tool.poetry]
 name = "arxivterminal"
-version = "0.1.0"
+version = "0.2.0"
 description = "An application for summarizing Arxiv results within the terminal"
 authors = ["John Bencina <jbencina@users.noreply.github.com>"]
-license = "MIT"
+license = "GPL-3.0-or-later"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 requests = "^2.28.2"
 bs4 = "^0.0.1"
 openai = "^0.27.4"
 lxml = "^4.9.2"
 pydantic = "^1.10.7"
 arxiv = "^1.4.3"
 click = "^8.1.3"
 termcolor = "^2.2.0"
 appdirs = "^1.4.4"
+scikit-learn = "^1.2.2"
 
 
 [tool.poetry.group.dev.dependencies]
 flake8 = "^6.0.0"
 black = "^23.3.0"
 mypy = "^1.2.0"
 pytest = "^7.3.1"
```

