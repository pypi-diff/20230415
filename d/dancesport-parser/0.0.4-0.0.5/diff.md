# Comparing `tmp/dancesport_parser-0.0.4.tar.gz` & `tmp/dancesport_parser-0.0.5.tar.gz`

## Comparing `dancesport_parser-0.0.4.tar` & `dancesport_parser-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rwxr-xr-x   0        0        0      857 2020-02-02 00:00:00.000000 dancesport_parser-0.0.4/Makefile
--rwxr-xr-x   0        0        0       12 2020-02-02 00:00:00.000000 dancesport_parser-0.0.4/requirements-dev.txt
--rwxr-xr-x   0        0        0       13 2020-02-02 00:00:00.000000 dancesport_parser-0.0.4/requirements.txt
--rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 dancesport_parser-0.0.4/.pytest_cache/.gitignore
--rwxr-xr-x   0        0        0      191 2020-02-02 00:00:00.000000 dancesport_parser-0.0.4/.pytest_cache/CACHEDIR.TAG
--rwxr-xr-x   0        0        0      302 2020-02-02 00:00:00.000000 dancesport_parser-0.0.4/.pytest_cache/README.md
--rwxr-xr-x   0        0        0        2 2020-02-02 00:00:00.000000 dancesport_parser-0.0.4/.pytest_cache/v/cache/stepwise
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 dancesport_parser-0.0.4/src/dancesport_parser/__init__.py
--rwxr-xr-x   0        0        0      205 2020-02-02 00:00:00.000000 dancesport_parser-0.0.4/src/dancesport_parser/util.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 dancesport_parser-0.0.4/src/dancesport_parser/o2cm/__init__.py
--rwxr-xr-x   0        0        0      132 2020-02-02 00:00:00.000000 dancesport_parser-0.0.4/src/dancesport_parser/o2cm/model.py
--rwxr-xr-x   0        0        0     1775 2020-02-02 00:00:00.000000 dancesport_parser-0.0.4/src/dancesport_parser/o2cm/parser.py
--rwxr-xr-x   0        0        0     3911 2020-02-02 00:00:00.000000 dancesport_parser-0.0.4/test/test_o2cm_parser.py
--rwxr-xr-x   0        0        0       45 2020-02-02 00:00:00.000000 dancesport_parser-0.0.4/.gitignore
--rwxr-xr-x   0        0        0    35149 2020-02-02 00:00:00.000000 dancesport_parser-0.0.4/LICENSE
--rwxr-xr-x   0        0        0       63 2020-02-02 00:00:00.000000 dancesport_parser-0.0.4/README.md
--rwxr-xr-x   0        0        0      818 2020-02-02 00:00:00.000000 dancesport_parser-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 dancesport_parser-0.0.4/PKG-INFO
+-rwxr-xr-x   0        0        0      857 2020-02-02 00:00:00.000000 dancesport_parser-0.0.5/Makefile
+-rwxr-xr-x   0        0        0       12 2020-02-02 00:00:00.000000 dancesport_parser-0.0.5/requirements-dev.txt
+-rwxr-xr-x   0        0        0       13 2020-02-02 00:00:00.000000 dancesport_parser-0.0.5/requirements.txt
+-rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 dancesport_parser-0.0.5/.pytest_cache/.gitignore
+-rwxr-xr-x   0        0        0      191 2020-02-02 00:00:00.000000 dancesport_parser-0.0.5/.pytest_cache/CACHEDIR.TAG
+-rwxr-xr-x   0        0        0      302 2020-02-02 00:00:00.000000 dancesport_parser-0.0.5/.pytest_cache/README.md
+-rwxr-xr-x   0        0        0      106 2020-02-02 00:00:00.000000 dancesport_parser-0.0.5/.pytest_cache/v/cache/nodeids
+-rwxr-xr-x   0        0        0        2 2020-02-02 00:00:00.000000 dancesport_parser-0.0.5/.pytest_cache/v/cache/stepwise
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 dancesport_parser-0.0.5/src/dancesport_parser/__init__.py
+-rwxr-xr-x   0        0        0      205 2020-02-02 00:00:00.000000 dancesport_parser-0.0.5/src/dancesport_parser/util.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 dancesport_parser-0.0.5/src/dancesport_parser/o2cm/__init__.py
+-rwxr-xr-x   0        0        0      145 2020-02-02 00:00:00.000000 dancesport_parser-0.0.5/src/dancesport_parser/o2cm/model.py
+-rwxr-xr-x   0        0        0     1889 2020-02-02 00:00:00.000000 dancesport_parser-0.0.5/src/dancesport_parser/o2cm/parser.py
+-rwxr-xr-x   0        0        0     4121 2020-02-02 00:00:00.000000 dancesport_parser-0.0.5/test/test_o2cm_parser.py
+-rwxr-xr-x   0        0        0       45 2020-02-02 00:00:00.000000 dancesport_parser-0.0.5/.gitignore
+-rwxr-xr-x   0        0        0    35149 2020-02-02 00:00:00.000000 dancesport_parser-0.0.5/LICENSE
+-rwxr-xr-x   0        0        0       63 2020-02-02 00:00:00.000000 dancesport_parser-0.0.5/README.md
+-rwxr-xr-x   0        0        0      818 2020-02-02 00:00:00.000000 dancesport_parser-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 dancesport_parser-0.0.5/PKG-INFO
```

### Comparing `dancesport_parser-0.0.4/Makefile` & `dancesport_parser-0.0.5/Makefile`

 * *Files identical despite different names*

### Comparing `dancesport_parser-0.0.4/src/dancesport_parser/o2cm/parser.py` & `dancesport_parser-0.0.5/src/dancesport_parser/o2cm/parser.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 import datetime
 import re
+from os import path
 from typing import List
 
 from bs4 import BeautifulSoup
 
 from dancesport_parser.util import parseHtml
 from dancesport_parser.o2cm.model import Competition
 
+
+RESULTS_MAIN_DOMAIN = "https://results.o2cm.com/"
+
+
 def parseMain(htmlDOM: BeautifulSoup = None, rawHtml: str = None) -> List[Competition]:
     """Parse o2cm main results screen, i.e. results.o2cm.com.
     
     Keyword arguments:
     htmlDOM -- HTML contents to parse.
     rawHtml -- If `htmlDOM` is unspecified, raw string to directly parse.
     """
@@ -35,10 +40,10 @@
             date = str(rowData[0].get_text().strip())
             compName = rowData[1].get_text().strip()
             compUrl = row.find("a")["href"]
             matchCompUrl = re.match(r'event[23].asp\?event=([a-zA-Z]{0,4}\d{0,5}[a-zA-Z]?)&.*', compUrl)
             compId = matchCompUrl.group(1).lower()
             fullDate = date + " " + str(year)
             compDate = datetime.datetime.strptime(fullDate, "%b %d %Y").date()
-            competition = Competition(compId, compName, compDate)
+            competition = Competition(compId, compName, compDate, path.join(RESULTS_MAIN_DOMAIN, compUrl))
             results.append(competition)
     return results
```

### Comparing `dancesport_parser-0.0.4/test/test_o2cm_parser.py` & `dancesport_parser-0.0.5/test/test_o2cm_parser.py`

 * *Files 7% similar despite different names*

```diff
@@ -68,10 +68,12 @@
 def o2cm_parser_assertion_helper(results: List[Competition]) -> None:
     competitionSorter: Callable[[Competition, ], str] = lambda comp: comp.id
     results.sort(key=competitionSorter)
     assert len(results) == 6
     assert results[0].id == "bcb23"
     assert results[0].date == date(2023, 4, 8)
     assert results[0].name == "Berkeley Classic Ballroom Competition"
+    assert results[0].url == "https://results.o2cm.com/event3.asp?event=bcb23&bclr=#FFFFFF&tclr=#000000"
     assert results[1].id == "big22"
     assert results[1].date == date(2022, 12, 10)
     assert results[1].name == "Big Apple Dancesport Challenge"
+    assert results[1].url == "https://results.o2cm.com/event3.asp?event=big22&bclr=#FFFFFF&tclr=#000000"
```

#### html2text {}

```diff
@@ -24,9 +24,12 @@
 o2cm_parser_assertion_helper(results) def test_o2cm_parser_raw() -> None: #
 Execute results = parseMain(rawHtml=MAIN_RESULTS_PAGE1) # Verify
 o2cm_parser_assertion_helper(results) def o2cm_parser_assertion_helper(results:
 List[Competition]) -> None: competitionSorter: Callable[[Competition, ], str] =
 lambda comp: comp.id results.sort(key=competitionSorter) assert len(results) ==
 6 assert results[0].id == "bcb23" assert results[0].date == date(2023, 4, 8)
 assert results[0].name == "Berkeley Classic Ballroom Competition" assert
-results[1].id == "big22" assert results[1].date == date(2022, 12, 10) assert
-results[1].name == "Big Apple Dancesport Challenge"
+results[0].url == "https://results.o2cm.com/
+event3.asp?event=bcb23&bclr=#FFFFFF&tclr=#000000" assert results[1].id ==
+"big22" assert results[1].date == date(2022, 12, 10) assert results[1].name ==
+"Big Apple Dancesport Challenge" assert results[1].url == "https://
+results.o2cm.com/event3.asp?event=big22&bclr=#FFFFFF&tclr=#000000"
```

### Comparing `dancesport_parser-0.0.4/LICENSE` & `dancesport_parser-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dancesport_parser-0.0.4/pyproject.toml` & `dancesport_parser-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dancesport_parser"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Eric Lam", email="eric@ericblam.com" },
 ]
 description = "Parsing library for dancesport information"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `dancesport_parser-0.0.4/PKG-INFO` & `dancesport_parser-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dancesport_parser
-Version: 0.0.4
+Version: 0.0.5
 Summary: Parsing library for dancesport information
 Project-URL: Homepage, https://github.com/ballroombookkeeper/dancesport-parser
 Project-URL: Bug Tracker, https://github.com/ballroombookkeeper/dancesport-parser/issues
 Author-email: Eric Lam <eric@ericblam.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

