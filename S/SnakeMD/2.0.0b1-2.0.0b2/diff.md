# Comparing `tmp/SnakeMD-2.0.0b1.tar.gz` & `tmp/SnakeMD-2.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SnakeMD-2.0.0b1.tar", last modified: Fri Apr  7 00:02:40 2023, max compression
+gzip compressed data, was "SnakeMD-2.0.0b2.tar", last modified: Mon Apr 10 17:10:39 2023, max compression
```

## Comparing `SnakeMD-2.0.0b1.tar` & `SnakeMD-2.0.0b2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 00:02:40.675195 SnakeMD-2.0.0b1/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-07 00:02:29.000000 SnakeMD-2.0.0b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7728 2023-04-07 00:02:40.675195 SnakeMD-2.0.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7060 2023-04-07 00:02:29.000000 SnakeMD-2.0.0b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 00:02:40.671194 SnakeMD-2.0.0b1/SnakeMD.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7728 2023-04-07 00:02:40.000000 SnakeMD-2.0.0b1/SnakeMD.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-07 00:02:40.000000 SnakeMD-2.0.0b1/SnakeMD.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 00:02:40.000000 SnakeMD-2.0.0b1/SnakeMD.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-07 00:02:40.000000 SnakeMD-2.0.0b1/SnakeMD.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 00:02:40.675195 SnakeMD-2.0.0b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-04-07 00:02:29.000000 SnakeMD-2.0.0b1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 00:02:40.675195 SnakeMD-2.0.0b1/snakemd/
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-07 00:02:29.000000 SnakeMD-2.0.0b1/snakemd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10826 2023-04-07 00:02:29.000000 SnakeMD-2.0.0b1/snakemd/document.py
--rw-r--r--   0 runner    (1001) docker     (123)    34244 2023-04-07 00:02:29.000000 SnakeMD-2.0.0b1/snakemd/elements.py
--rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-04-07 00:02:29.000000 SnakeMD-2.0.0b1/snakemd/templates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 00:02:40.675195 SnakeMD-2.0.0b1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-07 00:02:29.000000 SnakeMD-2.0.0b1/tests/test_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-04-07 00:02:29.000000 SnakeMD-2.0.0b1/tests/test_document.py
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-04-07 00:02:29.000000 SnakeMD-2.0.0b1/tests/test_heading.py
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-07 00:02:29.000000 SnakeMD-2.0.0b1/tests/test_horizontal_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     9141 2023-04-07 00:02:29.000000 SnakeMD-2.0.0b1/tests/test_inline.py
--rw-r--r--   0 runner    (1001) docker     (123)     5683 2023-04-07 00:02:29.000000 SnakeMD-2.0.0b1/tests/test_md_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-07 00:02:29.000000 SnakeMD-2.0.0b1/tests/test_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-04-07 00:02:29.000000 SnakeMD-2.0.0b1/tests/test_paragraph.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-07 00:02:29.000000 SnakeMD-2.0.0b1/tests/test_quote.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-07 00:02:29.000000 SnakeMD-2.0.0b1/tests/test_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-04-07 00:02:29.000000 SnakeMD-2.0.0b1/tests/test_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-04-07 00:02:29.000000 SnakeMD-2.0.0b1/tests/test_table_of_contents.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:10:39.686669 SnakeMD-2.0.0b2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-10 17:10:27.000000 SnakeMD-2.0.0b2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7728 2023-04-10 17:10:39.682669 SnakeMD-2.0.0b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7060 2023-04-10 17:10:27.000000 SnakeMD-2.0.0b2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:10:39.682669 SnakeMD-2.0.0b2/SnakeMD.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7728 2023-04-10 17:10:39.000000 SnakeMD-2.0.0b2/SnakeMD.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-10 17:10:39.000000 SnakeMD-2.0.0b2/SnakeMD.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 17:10:39.000000 SnakeMD-2.0.0b2/SnakeMD.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-10 17:10:39.000000 SnakeMD-2.0.0b2/SnakeMD.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 17:10:39.686669 SnakeMD-2.0.0b2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-04-10 17:10:27.000000 SnakeMD-2.0.0b2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:10:39.682669 SnakeMD-2.0.0b2/snakemd/
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-10 17:10:27.000000 SnakeMD-2.0.0b2/snakemd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13530 2023-04-10 17:10:27.000000 SnakeMD-2.0.0b2/snakemd/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39935 2023-04-10 17:10:27.000000 SnakeMD-2.0.0b2/snakemd/elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-04-10 17:10:27.000000 SnakeMD-2.0.0b2/snakemd/templates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:10:39.682669 SnakeMD-2.0.0b2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-10 17:10:27.000000 SnakeMD-2.0.0b2/tests/test_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-04-10 17:10:27.000000 SnakeMD-2.0.0b2/tests/test_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-04-10 17:10:27.000000 SnakeMD-2.0.0b2/tests/test_heading.py
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-10 17:10:27.000000 SnakeMD-2.0.0b2/tests/test_horizontal_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9141 2023-04-10 17:10:27.000000 SnakeMD-2.0.0b2/tests/test_inline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6694 2023-04-10 17:10:27.000000 SnakeMD-2.0.0b2/tests/test_md_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-10 17:10:27.000000 SnakeMD-2.0.0b2/tests/test_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-04-10 17:10:27.000000 SnakeMD-2.0.0b2/tests/test_paragraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-10 17:10:27.000000 SnakeMD-2.0.0b2/tests/test_quote.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-10 17:10:27.000000 SnakeMD-2.0.0b2/tests/test_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-04-10 17:10:27.000000 SnakeMD-2.0.0b2/tests/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-04-10 17:10:27.000000 SnakeMD-2.0.0b2/tests/test_table_of_contents.py
```

### Comparing `SnakeMD-2.0.0b1/LICENSE` & `SnakeMD-2.0.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `SnakeMD-2.0.0b1/PKG-INFO` & `SnakeMD-2.0.0b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SnakeMD
-Version: 2.0.0b1
+Version: 2.0.0b2
 Summary: A markdown generation library for Python.
 Home-page: https://github.com/TheRenegadeCoder/SnakeMD
 Author: The Renegade Coder
 Author-email: jeremy.grifski@therenegadecoder.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `SnakeMD-2.0.0b1/README.md` & `SnakeMD-2.0.0b2/README.md`

 * *Files identical despite different names*

### Comparing `SnakeMD-2.0.0b1/SnakeMD.egg-info/PKG-INFO` & `SnakeMD-2.0.0b2/SnakeMD.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SnakeMD
-Version: 2.0.0b1
+Version: 2.0.0b2
 Summary: A markdown generation library for Python.
 Home-page: https://github.com/TheRenegadeCoder/SnakeMD
 Author: The Renegade Coder
 Author-email: jeremy.grifski@therenegadecoder.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `SnakeMD-2.0.0b1/setup.py` & `SnakeMD-2.0.0b2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,18 +10,19 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 MAJOR = 2
 MINOR = 0
 PATCH = 0
+PRE = "b2"
 
 name = "SnakeMD"
 version = f"{MAJOR}.{MINOR}"
-release = f"{MAJOR}.{MINOR}.{PATCH}b1"
+release = f"{MAJOR}.{MINOR}.{PATCH}{PRE}"
 setuptools.setup(
     name=name,
     version=release,
     author="The Renegade Coder",
     author_email="jeremy.grifski@therenegadecoder.com",
     description="A markdown generation library for Python.",
     long_description=long_description,
```

### Comparing `SnakeMD-2.0.0b1/snakemd/document.py` & `SnakeMD-2.0.0b2/snakemd/document.py`

 * *Files 21% similar despite different names*

```diff
@@ -19,22 +19,22 @@
     between to generate the markdown document. Document methods
     are intended to provided convenience when generating a
     markdown file. However, the functionality is not exhaustive.
     To get the full range of markdown functionality, you can
     take advantage of the :func:`add_block` function to provide
     custom markdown blocks.
 
-    All methods described in the Document class include sample
-    code. Sample code assumes a generic :code:`doc` object exists,
-    which can be created as follows:
-
-    .. code-block:: Python
-
+    .. testsetup:: document
+    
         import snakemd
-        doc = snakemd.new_doc()
+        
+    .. testcleanup:: document
+    
+        import os
+        os.remove("README.md")
     """
 
     def __init__(self) -> None:
         self._contents: list[Block] = list()
         logger.debug("New document initialized")
 
     def __str__(self):
@@ -47,49 +47,65 @@
         return "\n\n".join(str(block) for block in self._contents)
 
     def add_block(self, block: Block) -> Block:
         """
         A generic function for appending blocks to the document.
         Use this function when you want a little more control over
         what the output looks like.
-
-        .. code-block:: Python
-
-            doc.add_block(Heading("Python is Cool!", 2))
+        
+        .. doctest:: document
+        
+            >>> doc = snakemd.new_doc()
+            >>> doc.add_block(snakemd.Heading("Python is Cool!", 2)) 
+            <snakemd.elements.Heading object at ...>
+            >>> str(doc)
+            '## Python is Cool!'
 
         :param Block block: 
             a markdown block (e.g., Table, Heading, etc.)
         :return: 
             the :class:`Block` added to this Document
         """
         self._contents.append(block)
         logger.debug(f"Added custom block to document\n{block}")
         return block
 
     def add_raw(self, text: str) -> Raw:
         """
         A convenience method which adds text as-is to the document:
-
-        .. code-block:: Python
-
-            doc.add_raw("X: 5\\nY: 4\\nZ: 3")
+        
+        .. doctest:: document
+        
+            >>> doc = snakemd.new_doc()
+            >>> doc.add_raw("X: 5\\nY: 4\\nZ: 3")
+            <snakemd.elements.Raw object at ...>
+            >>> str(doc)
+            'X: 5\\nY: 4\\nZ: 3'
 
         :param str text: 
             some text 
         :return: 
             the :class:`Raw` block added to this Document
         """
         raw = Raw(text)
         self._contents.append(raw)
         logger.debug(f"Added raw block to document\n{text}")
         return raw
 
     def add_heading(self, text: str, level: int = 1) -> Heading:
         """
         A convenience method which adds a heading to the document:
+        
+        .. doctest:: document
+        
+            >>> doc = snakemd.new_doc()
+            >>> doc.add_heading("Welcome to SnakeMD!")
+            <snakemd.elements.Heading object at ...>
+            >>> str(doc)
+            '# Welcome to SnakeMD!'
 
         .. code-block:: Python
 
             doc.add_heading("Welcome to SnakeMD!")
 
         :param str text: 
             the text for the heading
@@ -102,104 +118,119 @@
         self._contents.append(heading)
         logger.debug(f"Added heading to document\n{heading}")
         return heading
 
     def add_paragraph(self, text: str) -> Paragraph:
         """
         A convenience method which adds a paragraph of text to the document:
-
-        .. code-block:: Python
-
-            doc.add_paragraph("Mitochondria is the powerhouse of the cell.")
+        
+        .. doctest:: document
+        
+            >>> doc = snakemd.new_doc()
+            >>> doc.add_paragraph("Mitochondria is the powerhouse of the cell.")
+            <snakemd.elements.Paragraph object at ...>
+            >>> str(doc)
+            'Mitochondria is the powerhouse of the cell.'
 
         :param str text: 
             any arbitrary text
         :return: 
             the :class:`Paragraph` added to this Document
         """
         paragraph = Paragraph([Inline(text)])
         self._contents.append(paragraph)
         logger.debug(f"Added paragraph to document\n{paragraph}")
         return paragraph
 
     def add_ordered_list(self, items: Iterable[str]) -> MDList:
         """
         A convenience method which adds an ordered list to the document:
-
-        .. code-block:: Python
-
-            doc.add_ordered_list(["Goku", "Piccolo", "Vegeta"])
+        
+        .. doctest:: document
+        
+            >>> doc = snakemd.new_doc()
+            >>> doc.add_ordered_list(["Goku", "Piccolo", "Vegeta"])
+            <snakemd.elements.MDList object at ...>
+            >>> str(doc)
+            '1. Goku\\n2. Piccolo\\n3. Vegeta'
 
         :param Iterable[str] items: 
             a "list" of strings
         :return: 
             the :class:`MDList` added to this Document
         """
-        md_list = MDList([Inline(item) for item in items], ordered=True)
+        md_list = MDList(items, ordered=True)
         self._contents.append(md_list)
         logger.debug(f"Added ordered list to document\n{md_list}")
         return md_list
 
     def add_unordered_list(self, items: Iterable[str]) -> MDList:
         """
         A convenience method which adds an unordered list to the document.
-
-        .. code-block:: Python
-
-            doc.add_unordered_list(["Deku", "Bakugo", "Kirishima"])
+        
+        .. doctest:: document
+        
+            >>> doc = snakemd.new_doc()
+            >>> doc.add_unordered_list(["Deku", "Bakugo", "Kirishima"])
+            <snakemd.elements.MDList object at ...>
+            >>> str(doc)
+            '- Deku\\n- Bakugo\\n- Kirishima'
 
         :param Iterable[str] items: 
             a "list" of strings
         :return: 
             the :class:`MDList` added to this Document
         """
-        md_list = MDList([Inline(item) for item in items])
+        md_list = MDList(items)
         self._contents.append(md_list)
         logger.debug(f"Added unordered list to document\n{md_list}")
         return md_list
 
     def add_checklist(self, items: Iterable[str]) -> MDList:
         """
         A convenience method which adds a checklist to the document.
-
-        .. code-block:: Python
-
-            doc.add_checklist(["Okabe", "Mayuri", "Kurisu"])
+        
+        .. doctest:: document
+        
+            >>> doc = snakemd.new_doc()
+            >>> doc.add_checklist(["Okabe", "Mayuri", "Kurisu"])
+            <snakemd.elements.MDList object at ...>
+            >>> str(doc)
+            '- [ ] Okabe\\n- [ ] Mayuri\\n- [ ] Kurisu'
 
         :param Iterable[str] items: 
             a "list" of strings
         :return: 
             the :class:`MDList` added to this Document
         """
-        md_checklist = MDList([Inline(item) for item in items], checked=False)
+        md_checklist = MDList(items, checked=False)
         self._contents.append(md_checklist)
         logger.debug(f"Added checklist to document\n{md_checklist}")
         return md_checklist
 
     def add_table(
         self,
         header: Iterable[str],
         data: Iterable[Iterable[str]],
         align: Iterable[Table.Align] = None,
         indent: int = 0
     ) -> Table:
         """
         A convenience method which adds a table to the document:
-
-        .. code-block:: Python
-
-            doc.add_table(
-                ["Place", "Name"],
-                [
-                    ["1st", "Robert"],
-                    ["2nd", "Rae"]
-                ],
-                [snakemd.Table.Align.CENTER, snakemd.Table.Align.RIGHT],
-                0
-            )
+        
+        .. doctest:: document
+        
+            >>> doc = snakemd.new_doc()
+            >>> header = ["Place", "Name"]
+            >>> rows = [["1st", "Robert"], ["2nd", "Rae"]]
+            >>> align = [snakemd.Table.Align.CENTER, snakemd.Table.Align.RIGHT]
+            >>> doc.add_table(header, rows, align=align)
+            <snakemd.elements.Table object at ...>
+            >>> str(doc)
+            '| Place | Name   |\\n| :---: | -----: |\\n| 1st   | Robert |\\n| 2nd   | Rae    |'
 
         :param Iterable[str] header: 
             a "list" of strings
         :param Iterable[Iterable[str]] data: 
             a "list" of "lists" of strings
         :param Iterable[Table.Align] align: 
             a "list" of column alignment values;
@@ -215,18 +246,22 @@
         self._contents.append(table)
         logger.debug(f"Added table to document\n{table}")
         return table
 
     def add_code(self, code: str, lang: str = "generic") -> Code:
         """
         A convenience method which adds a code block to the document:
-
-        .. code-block:: Python
-
-            doc.add_code("x = 5")
+        
+        .. doctest:: document
+        
+            >>> doc = snakemd.new_doc()
+            >>> doc.add_code("x = 5")
+            <snakemd.elements.Code object at ...>
+            >>> str(doc)
+            '```generic\\nx = 5\\n```'
 
         :param str code: 
             a preformatted code string
         :param str lang: 
             the language for syntax highlighting
         :return: 
             the :class:`Code` block added to this Document
@@ -235,36 +270,44 @@
         self._contents.append(code_block)
         logger.debug(f"Added code block to document\n{code_block}")
         return code_block
 
     def add_quote(self, text: str) -> Quote:
         """
         A convenience method which adds a blockquote to the document:
-
-        .. code-block:: Python
-
-            doc.add_quote("Welcome to the Internet!")
+        
+        .. doctest:: document
+        
+            >>> doc = snakemd.new_doc()
+            >>> doc.add_quote("Welcome to the Internet!")
+            <snakemd.elements.Quote object at ...>
+            >>> str(doc)
+            '> Welcome to the Internet!'
 
         :param str text: 
             the text to be quoted
         :return: 
             the :class:`Quote` added to this Document
         """
         quote = Quote(text)
         self._contents.append(quote)
         logger.debug(f"Added quote to document\n{quote}")
         return quote
 
     def add_horizontal_rule(self) -> HorizontalRule:
         """
         A convenience method which adds a horizontal rule to the document:
-
-        .. code-block:: Python
-
-            doc.add_horizontal_rule()
+        
+        .. doctest:: document
+        
+            >>> doc = snakemd.new_doc()
+            >>> doc.add_horizontal_rule()
+            <snakemd.elements.HorizontalRule object at ...>
+            >>> str(doc)
+            '***'
 
         :return: 
             the :class:`HorizontalRule` added to this Document
         """
         hr = HorizontalRule()
         self._contents.append(hr)
         logger.debug(f"Added horizontal rule to document\n{hr}")
@@ -273,18 +316,26 @@
     def add_table_of_contents(self, levels: range = range(2, 3)) -> TableOfContents:
         """
         A convenience method which creates a table of contents. This function
         can be called where you want to add a table of contents to your
         document. The table itself is lazy loaded, so it always captures
         all of the heading blocks regardless of where the table of contents
         is added to the document.
-
-        .. code-block:: Python
-
-            doc.add_table_of_contents()
+        
+        .. doctest:: document
+        
+            >>> doc = snakemd.new_doc()
+            >>> doc.add_table_of_contents()
+            <snakemd.templates.TableOfContents object at ...>
+            >>> doc.add_heading("First Item", 2)
+            <snakemd.elements.Heading object at ...>
+            >>> doc.add_heading("Second Item", 2) 
+            <snakemd.elements.Heading object at ...>
+            >>> str(doc)
+            '1. [First Item](#first-item)\\n2. [Second Item](#second-item)\\n\\n## First Item\\n\\n## Second Item'
 
         :param range levels: 
             a range of heading levels to be included in the table of contents
         :return: 
             the :class:`TableOfContents` added to this Document
         """
         toc = TableOfContents(self, levels=levels)
@@ -294,33 +345,41 @@
         )
         return toc
 
     def scramble(self) -> None:
         """
         A silly method which mixes all of the blocks in this document in
         a random order.
-
-        .. code-block:: Python
-
-            doc.scramble()
+        
+        .. doctest:: document
+        
+            >>> doc = snakemd.new_doc()
+            >>> doc.add_horizontal_rule()
+            <snakemd.elements.HorizontalRule object at ...>
+            >>> doc.scramble()
+            >>> str(doc)
+            '***'
         """
         random.shuffle(self._contents)
         logger.debug(f"Scrambled document")
 
     def dump(self, name: str, dir: str | os.PathLike = "", ext: str = "md", encoding: str = "utf-8") -> None:
         """
         Outputs the markdown document to a file. This method assumes the output directory
         is the current working directory. Any alternative directory provided will be
         made if it does not already exist. This method also assumes a file extension of md
         and a file encoding of utf-8, all of which are configurable through the method
         parameters.
-
-        .. code-block:: Python
-
-            doc.dump("README")
+        
+        .. doctest:: document
+        
+            >>> doc = snakemd.new_doc()
+            >>> doc.add_horizontal_rule()
+            <snakemd.elements.HorizontalRule object at ...>
+            >>> doc.dump("README")
 
         :param str name: 
             the name of the markdown file to output without the file extension
         :param str | os.PathLike dir: 
             the output directory for the markdown file; defaults to ""
         :param str ext: 
             the output file extension; defaults to "md"
```

### Comparing `SnakeMD-2.0.0b1/snakemd/elements.py` & `SnakeMD-2.0.0b2/snakemd/elements.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,41 +32,51 @@
     applied last. Due to this design, some forms of inline text are not
     possible. For example, inline elements can be used to show inline 
     markdown as an inline code element (e.g., :code:`![here](https://example.com)`).
     However, inline elements cannot be used to style inline code (e.g., :code:`**`code`**`).
     If styled code is necessary, it's possible to render the inline element
     as a string and pass the result to another inline element. 
 
-    All methods described in the Inline class include sample
-    code. Sample code assumes a generic :code:`inline` object exists,
-    which can be created as follows:
-
-    .. code-block:: Python
-
+    .. testsetup:: inline
+    
         from snakemd import Inline
-        inline = Inline("Sample Text")
 
     :param str text: 
         the inline text to render
     :param None | str image: 
         the source (either url or path) associated with an image
+        
+        - defaults to :code:`None`
+        - set to a string representing a URL or path to render an image (i.e., :code:`![text](image)`)
     :param None | str link: 
         the link (either url or path) associated with the inline element
+        
+        - defaults to :code:`None`
+        - set to a string representing a URL or path to render a link (i.e., :code:`[text](link)`)
     :param bool bold: 
-        the bold state of the inline text;
-        set to True to render bold inline text (i.e., True -> **bold**)
+        the bold state of the inline text
+        
+        - defaults to :code:`False`
+        - set to :code:`True` to render bold text (i.e., :code:`**text**`)
     :param bool italics: 
-        the italics state of the inline element;
-        set to True to render inline text in italics (i.e., True -> *italics*)
+        the italics state of the inline element
+        
+        - defaults to :code:`False`
+        - set to :code:`True` to render text in italics (i.e., :code:`_text_`)
     :param bool strikethrough: 
-        the strikethrough state of the inline text;
-        set to True to render inline text with a strikethrough (i.e., True -> ~~strikethrough~~)
+        the strikethrough state of the inline text
+        
+        - defaults to :code:`False`
+        - set to :code:`True` to render text with a strikethrough 
+          (i.e., :code:`~~text~~`)
     :param bool code: 
-        the italics state of the inline text;
-        set to True to render inline text as code (i.e., True -> `code`)
+        the code state of the inline text
+        
+        - defaults to :code:`False`
+        - set to :code:`True` to render text as code (i.e., ```text```)
     """
 
     def __init__(
         self,
         text: str,
         image: None | str = None,
         link: None | str = None,
@@ -82,16 +92,22 @@
         self._italics = italics
         self._strikethrough = strikethrough
         self._code = code
 
     def __str__(self) -> str:
         """
         Renders self as a string. In this case,
-        inline text can represent many different types of data from
-        stylized text to inline code to links and images.
+        inline can represent many different types of data from
+        stylized text to code, links, and images.
+        
+        .. doctest:: inline
+
+            >>> inline = Inline("This is formatted text", bold=True, italics=True)
+            >>> str(inline)
+            '_**This is formatted text**_'
 
         :return: 
             the Inline object as a string
         """
         text = self._text
         if self._image:
             text = f"![{text}]({self._image})"
@@ -109,186 +125,212 @@
         return text
 
     def is_text(self) -> bool:
         """
         Checks if this Inline element is a text-only element. If not, it must
         be an image, a link, or a code snippet.
 
-        .. code-block:: Python
+        .. doctest:: inline
 
-            is_inline_text: bool = inline.is_text()
+            >>> inline = Inline("This is text")
+            >>> inline.is_text()
+            True
 
         :return: 
             True if this is a text-only element; False otherwise
         """
         return not (self._code or self._image or self._link)
 
     def is_link(self) -> bool:
         """
         Checks if the Inline object represents a link.
 
-        .. code-block:: Python
+        .. doctest:: inline
 
-            is_inline_link: bool = inline.is_link()
+            >>> inline = Inline("This is not a link")
+            >>> inline.is_link()
+            False
 
         :return: 
             True if the object has a link; False otherwise
         """
         return bool(self._link)
 
     def bold(self) -> Inline:
         """
         Adds bold styling to self.
 
-        .. code-block:: Python
+        .. doctest:: inline
 
-            inline.bold()
+            >>> inline = Inline("This is bold text").bold()
+            >>> str(inline)
+            '**This is bold text**'
 
         :return: 
             self
         """
         self._bold = True
         return self
 
     def unbold(self) -> Inline:
         """
         Removes bold styling from self.
 
-        .. code-block:: Python
+        .. doctest:: inline
 
-            inline.unbold()
+            >>> inline = Inline("This is normal text", bold=True).unbold()
+            >>> str(inline)
+            'This is normal text'
 
         :return: 
             self
         """
         self._bold = False
         return self
 
     def italicize(self) -> Inline:
         """
         Adds italics styling to self.
 
-        .. code-block:: Python
+        .. doctest:: inline
 
-            inline.italicize()
+            >>> inline = Inline("This is italicized text").italicize()
+            >>> str(inline)
+            '_This is italicized text_'
 
         :return: 
             self
         """
         self._italics = True
         return self
 
     def unitalicize(self) -> Inline:
         """
         Removes italics styling from self.
 
-        .. code-block:: Python
+        .. doctest:: inline
 
-            inline.unitalicize()
+            >>> inline = Inline("This is normal text", italics=True).unitalicize()
+            >>> str(inline)
+            'This is normal text'
 
         :return: 
             self
         """
         self._italics = False
         return self
 
     def strikethrough(self) -> Inline:
         """
         Adds strikethrough styling to self.
 
-        .. code-block:: Python
+        .. doctest:: inline
 
-            inline.strikethrough()
+            >>> inline = Inline("This is striked text").strikethrough()
+            >>> str(inline)
+            '~~This is striked text~~'
 
         :return: 
             self
         """
         self._strikethrough = True
         return self
 
     def unstrikethrough(self) -> Inline:
         """
         Remove strikethrough styling from self.
 
-        .. code-block:: Python
+        .. doctest:: inline
 
-            inline.unstrikethrough()
+            >>> inline = Inline("This is normal text", strikethrough=True).unstrikethrough()
+            >>> str(inline)
+            'This is normal text'
 
         :return: 
             self
         """
         self._strikethrough = False
         return self
 
     def code(self) -> Inline:
         """
         Adds code style to self.
 
-        .. code-block:: Python
+        .. doctest:: inline
 
-            inline.code()
+            >>> inline = Inline("x = 5").code()
+            >>> str(inline)
+            '`x = 5`'
 
         :return: 
             self
         """
         self._code = True
         return self
 
     def uncode(self) -> Inline:
         """
         Removes code styling from self.
 
-        .. code-block:: Python
+        .. doctest:: inline
 
-            inline.uncode()
+            >>> inline = Inline("This is normal text", code=True).uncode()
+            >>> str(inline)
+            'This is normal text'
 
         :return: 
             self
         """
         self._code = False
         return self
 
     def link(self, link: str) -> Inline:
         """
         Adds link to self.
 
-        .. code-block:: Python
+        .. doctest:: inline
 
-            inline.link("https://snakemd.io")
+            >>> inline = Inline("here").link("https://snakemd.io")
+            >>> str(inline)
+            '[here](https://snakemd.io)'
 
         :param str link: 
             the URL or path to apply to this Inline element
         :return: 
             self
         """
         self._link = link
         return self
 
     def unlink(self) -> Inline:
         """
         Removes link from self.
 
-        .. code-block:: Python
+        .. doctest:: inline
 
-            inline.unlink()
+            >>> inline = Inline("This is normal text", link="https://snakemd.io").unlink()
+            >>> str(inline)
+            'This is normal text'
 
         :return: 
             self
         """
         self._link = None
         return self
 
     def reset(self) -> Inline:
         """
         Removes all settings from self (e.g., bold, code, italics, url, etc.).
         All that will remain is the text itself.
 
-        .. code-block:: Python
+        .. doctest:: inline
 
-            inline.reset()
+            >>> inline = Inline("This is normal text", link="https://snakemd.io", bold=True).reset()
+            >>> str(inline)
+            'This is normal text'
 
         :return: 
             self
         """
         self._image = None
         self._link = None
         self._code = False
@@ -309,14 +351,22 @@
 
 
 class Code(Block):
     """
     A code block is a standalone block of syntax-highlighted code.
     Code blocks can have generic highlighting or highlighting based
     on their language. 
+    
+    :param str | Code code:
+        the sourcecode to format as a Markdown code block
+        
+        - set to a string to render a preformatted code block (i.e., whitespace is respected)
+        - set to a Code object to render a nested code block
+    :param str lang:
+        the programming language for the code block; defaults to 'generic'
     """
 
     def __init__(self, code: str | Code, lang: str = "generic"):
         super().__init__()
         self._code = code
         self._lang = lang
         self._backticks = self._process_backticks(code)
@@ -359,28 +409,28 @@
     
     
 class Heading(Block):
     """
     A heading is a text block which serves as the title for a new
     section of a document. Headings come in six main sizes which
     correspond to the six headings sizes in HTML (e.g., :code:`<h1>`).
-
-    All methods described in the Heading class include sample
-    code. Sample code assumes a generic :code:`heading` object exists,
-    which can be created as follows:
-
-    .. code-block:: python
-
+    
+    .. testsetup:: heading
+    
         from snakemd import Heading
-        heading = Heading("Sample Heading", 1)
 
     :raises ValueError: 
         when level < 1 or level > 6
     :param str | Inline | Iterable[Inline | str] text: 
         the heading text
+        
+        - set to a string to render raw heading text
+        - set to an Inline object to render a styled heading (e.g., bold, link, code, etc.)
+        - set to a "list" of the prior options to render a header with more granular 
+          control over the individual inline elements
     :param int level: 
         the heading level between 1 and 6
     """
 
     def __init__(self, text: str | Inline | Iterable[Inline | str], level: int) -> None:
         if level < 1 or level > 6:
             raise ValueError(
@@ -425,45 +475,61 @@
             return [text]
         else:
             return [
                 item if isinstance(item, Inline) else Inline(item)
                 for item in text
             ]
 
-    def promote(self) -> None:
+    def promote(self) -> Heading:
         """
         Promotes a heading up a level. Fails silently
         if the heading is already at the highest level (i.e., :code:`<h1>`).
+        
+        .. doctest:: heading
 
-        .. code-block:: Python
-
-            heading.promote()
+            >>> heading = Heading("This is an H2 heading", 3).promote()
+            >>> str(heading)
+            '## This is an H2 heading'
+            
+        :return:
+            self
         """
         if self._level > 1:
             self._level -= 1
+        return self
 
-    def demote(self) -> None:
+    def demote(self) -> Heading:
         """
         Demotes a heading down a level. Fails silently if
         the heading is already at the lowest level (i.e., :code:`<h6>`).
 
-        .. code-block:: Python
+        .. doctest:: heading
 
-            heading.demote()
+            >>> heading = Heading("This is an H2 heading", 1).demote()
+            >>> str(heading)
+            '## This is an H2 heading'
+            
+        :return:
+            self
         """
         if self._level < 6:
             self._level += 1
+        return self
 
     def get_text(self) -> str:
         """
-        Returns the heading text free of any styling.
-
-        .. code-block:: Python
-
-            text: str = heading.get_text()
+        Returns the heading text free of any styling. Useful
+        when the heading is composed of various Inline elements,
+        and the raw text is needed without styling or linking.
+
+        .. doctest:: heading
+
+            >>> heading = Heading("This is the heading text", 1)
+            >>> heading.get_text()
+            'This is the heading text'
 
         :return: 
             the heading as a string
         """
         text_elements = [item._text for item in self._text]
         return ''.join(text_elements)
 
@@ -491,35 +557,51 @@
         return "***"
     
     
 class MDList(Block):
     """
     A markdown list is a standalone list that comes in three varieties: ordered, unordered, and checked.
 
+    :raises ValueError: 
+        when the checked argument is an Iterable[bool] that does not 
+        match the number of top-level elements in the list
     :param Iterable[str | Inline | Block] items:
         a "list" of objects to be rendered as a list
     :param bool ordered: 
-        the ordered state of the list;
-        set to True to render an ordered list (i.e., True -> 1. item)
+        the ordered state of the list
+        
+        - defaults to :code:`False` which renders an unordered list (i.e., :code:`-`)
+        - set to :code:`True` to render an ordered list (i.e., :code:`1.`)
     :param None | bool | Iterable[bool] checked: 
-        the checked state of the list;
-        set to True, False, or an iterable of booleans to enable the checklist feature.
+        the checked state of the list
+        
+        - defaults to :code:`None` which excludes checkboxes from being rendered
+        - set to :code:`False` to render a series of unchecked boxes (i.e., :code:`- [ ]`)
+        - set to :code:`True` to render a series of checked boxes (i.e., :code:`- [x]`)
+        - set to :code:`Iterable[bool]` to render the checked 
+          status of the top-level list elements directly
     """
 
     def __init__(
         self,
         items: Iterable[str | Inline | Block],
         ordered: bool = False,
         checked: None | bool | Iterable[bool] = None
     ) -> None:
         super().__init__()
         self._items: list[Block] = self._process_items(items)
-        self._ordered = ordered
-        self._checked = checked
+        self._ordered: bool = ordered
+        self._checked: bool | list[bool] = checked \
+            if checked is None or isinstance(checked, bool) \
+            else [_ for _ in checked]
         self._space = ""
+        if isinstance(self._checked, list) and self._top_level_count() != len(self._checked):
+            raise ValueError(
+                f"Number of top-level elements in checklist does not match number of booleans supplied by checked parameter: {self._checked}"
+            )
 
     def __str__(self) -> str:
         """
         Renders the markdown list as a markdown string. Markdown lists
         come in a variety of flavors and are customized according to 
         the settings provided. For example, if the the ordered flag is 
         set, an ordered list will be rendered in markdown. Unordered
@@ -582,14 +664,31 @@
         processed = []
         for item in items:
             if isinstance(item, (str, Inline)):
                 processed.append(Paragraph([item]))
             else:
                 processed.append(item)
         return processed
+    
+    def _top_level_count(self) -> int:
+        """
+        Given that MDList can accept a variety of blocks,
+        we need to know how many items in the provided list
+        are top-level elements (i.e., not nested list elements).
+        We use this number to throw errors if this count does
+        not match up with the checklist count.
+
+        :return: 
+            a count of top-level elements
+        """
+        count = 0
+        for item in self._items:
+            if not isinstance(item, MDList):
+                count += 1
+        return count
 
     def _get_indent_size(self, item_index: int = -1) -> int:
         """
         Returns the number of spaces that any sublists should be indented.
 
         :param int item_index: 
             the index of the item to check (only used for ordered lists);
@@ -603,29 +702,30 @@
             # Ordered items vary in length, so we adjust the result based on the index
             return 2 + len(str(item_index))
 
 
 class Paragraph(Block):
     """
     A paragraph is a standalone block of text. 
-
-    All methods described in the Paragraph class include sample
-    code. Sample code assumes a generic :code:`paragraph` object exists,
-    which can be created as follows:
-
-    .. code-block:: python
-
+    
+    .. testsetup:: paragraph
+    
         from snakemd import Paragraph
-        paragraph = Paragraph("Hello, World!")
 
-    :param str | Iterable[Inline | str] content: 
-        a single string or a "list" of text objects to render as a paragraph        
+    :param str | Iterable[str | Inline] content: 
+        the text to be rendered as a paragraph where whitespace is not respected
+        (see :class:`snakemd.Raw` for whitespace sensitive applications)
+        
+        - set to a string to render a single line of unformatted text
+        - set to a "list" of text objects to render a paragraph with more 
+          granular control over the individual text objects (e.g., linking,
+          styling, etc.)     
     """
 
-    def __init__(self, content: str | Iterable[Inline | str]):
+    def __init__(self, content: str | Iterable[str | Inline]):
         super().__init__()
         self._content: list[Inline] = self._process_content(content)
 
     @staticmethod
     def _process_content(content) -> list[Inline]:
         """
         Processes the incoming content for the Paragraph.
@@ -659,28 +759,33 @@
 
         :return: 
             the paragraph as a markdown string
         """
         paragraph = ''.join(str(item) for item in self._content)
         return " ".join(paragraph.split())
 
-    def add(self, text: Inline | str) -> None:
+    def add(self, text: str | Inline) -> Paragraph:
         """
         Adds a text object to the paragraph.
+        
+        .. doctest:: paragraph
+        
+            >>> paragraph = Paragraph("Hello! ").add("I come in peace")
+            >>> str(paragraph)
+            'Hello! I come in peace'
 
-        .. code-block:: Python
-
-            paragraph.add("I come in peace")
-
-        :param Inline | str text: 
+        :param str | Inline text: 
             a custom Inline element
+        :return:
+            self
         """
         if isinstance(text, str):
             text = Inline(text)
         self._content.append(text)
+        return self
 
     def _replace_any(self, target: str, text: Inline, count: int = -1) -> Paragraph:
         """
         Given a target string, this helper method replaces it with the specified
         Inline object. This method was created because insert_link and
         replace were literally one line different. This method serves as the
         mediator. Note that using this method will introduce several new
@@ -719,66 +824,74 @@
 
     def replace(self, target: str, replacement: str, count: int = -1) -> Paragraph:
         """
         A convenience method which replaces a target string with a string of
         the users choice. Like :meth:`insert_link`, this method is modeled after
         :py:meth:`str.replace` of the standard library. As a result, a count
         can be provided to limit the number of strings replaced in the paragraph.
-
-        .. code-block:: Python
-
-            paragraph.replace("Here", "There")
+        
+        .. doctest:: paragraph
+        
+            >>> paragraph = Paragraph("I come in piece").replace("piece", "peace")
+            >>> str(paragraph)
+            'I come in peace'
 
         :param str target: 
             the target string to replace
         :param str replacement: 
             the Inline object to insert in place of the target
         :param int count: 
-            the number of links to insert; defaults to -1
+            the number of targets to replace; defaults to -1 (all)
         :return: 
             self
         """
         return self._replace_any(target, Inline(replacement), count)
 
-    def insert_link(self, target: str, url: str, count: int = -1) -> Paragraph:
+    def insert_link(self, target: str, link: str, count: int = -1) -> Paragraph:
         """
         A convenience method which inserts links in the paragraph
         for all matching instances of a target string. This method
         is modeled after :py:meth:`str.replace`, so a count can be
         provided to limit the number of insertions. This method
         will not replace links of text that have already been linked.
         See :meth:`snakemd.Paragraph.replace_link` for that behavior.
-
-        .. code-block:: Python
-
-            paragraph.insert_link("Here", "https://therenegadecoder.com")
+        
+        .. doctest:: paragraph
+        
+            >>> paragraph = Paragraph("Go here for docs").insert_link("here", "https://snakemd.io")
+            >>> str(paragraph)
+            'Go [here](https://snakemd.io) for docs'
 
         :param str target: 
             the string to link
-        :param str url: 
-            the url to link
+        :param str link: 
+            the url or path
         :param int count: 
             the number of links to insert; defaults to -1 (all)
         :return: 
             self
         """
-        return self._replace_any(target, Inline(target, link=url), count)
+        return self._replace_any(target, Inline(target, link=link), count)
 
     def replace_link(self, target_link: str, replacement_link: str, count: int = -1) -> Paragraph:
         """
         A convenience method which replaces matching URLs in the paragraph with
         a new url. Like :meth:`insert_link` and :meth:`replace`, this method is also
         modeled after :py:meth:`str.replace`, so a count can be provided to limit
         the number of links replaced in the paragraph. This method is useful
         if you want to replace existing URLs but don't necessarily care what
         the anchor text is.
-
-        .. code-block:: Python
-
-            paragraph.replace_link("https://stackoverflow.com", "https://therenegadecoder.com")
+        
+        .. doctest:: paragraph
+        
+            >>> old = "https://therenegadecoder.com"
+            >>> new = "https://snakemd.io"
+            >>> paragraph = Paragraph("Go here for docs").insert_link("here", old).replace_link(old, new) 
+            >>> str(paragraph)
+            'Go [here](https://snakemd.io) for docs'
 
         :param str target_link: 
             the link to replace
         :param str replacement_link: 
             the link to swap in
         :param int count: 
             the number of links to replace; defaults to -1 (all)
@@ -794,21 +907,25 @@
     
     
 class Quote(Block):
     """
     A quote is a standalone block of emphasized text. Quotes can be
     nested and can contain other blocks. 
 
-    :param str | Iterable[str | Inline | Block] lines: 
-        a single string or a "list" of text objects to be formatted as a quote
+    :param str | Iterable[str | Inline | Block] content:
+        the text to be formatted as a Markdown quote
+         
+        - set to a string to render a whitespace respected quote (similar to :class:`snakemd.Code`)
+        - set to a "list" of text objects to render a document-like quote
+          (i.e., all items will be separated by newlines)
     """
 
-    def __init__(self, lines: str | Iterable[str | Inline | Block]) -> None:
+    def __init__(self, content: str | Iterable[str | Inline | Block]) -> None:
         super().__init__()
-        self._lines: list[Block] = self._process_content(lines)
+        self._lines: list[Block] = self._process_content(content)
         self._depth = 1
 
     @staticmethod
     def _process_content(lines) -> list[Block]:
         """
         Converts the raw input lines to something that is
         a bit easier to work with. In this case, the lines
@@ -817,20 +934,20 @@
         :param lines: 
             a "list" of text objects or a string
         :return: 
             a list of Blocks
         """
         logger.debug(f"Processing quote lines: {lines}")
         if isinstance(lines, str):
-            processed_lines = [Paragraph(lines)]
+            processed_lines = [Raw(lines)]
         else:
             processed_lines = []
             for line in lines:
                 if isinstance(line, (str, Inline)):
-                    processed_lines.append(Paragraph(line))
+                    processed_lines.append(Raw(line))
                 else:
                     processed_lines.append(line)
         return processed_lines
 
     def __str__(self) -> str:
         """
         Renders the quote as a markdown string. Markdown quotes
@@ -904,27 +1021,23 @@
         return self._text
 
 
 class Table(Block):
     """
     A table is a standalone block of rows and columns. Data is rendered
     according to underlying Inline items.
-
-    All methods described in the Table class include sample
-    code. Sample code assumes a generic :code:`table` object exists,
-    which can be created as follows:
-
-    .. code-block:: Python
-
+    
+    .. testsetup:: table
+    
         from snakemd import Table
-        table = Table(["Place", "Name"], [["1st", "Crosby"], ["2nd", "McDavid"]])
 
     :raises ValueError: 
-        when rows of table are of varying lengths or 
-        when lengths of header and rows of table do not match
+    
+        - when rows of table are of varying lengths
+        - when lengths of header and rows of table do not match
     :param Iterable[str | Inline | Paragraph] header: 
         the header row of labels
     :param Iterable[Iterable[str | Inline | Paragraph]] body: 
         the collection of rows of data; defaults to an empty list
     :param None | Iterable[Align] align: 
         the column alignment; defaults to None
     :param int indent: 
@@ -1062,28 +1175,49 @@
         widths = [len(str(word)) for word in header]
         for row in body:
             for i, item in enumerate(row):
                 if (width := len(str(item))) > widths[i]:
                     widths[i] = width
         return widths
 
-    def add_row(self, row: Iterable[str | Inline | Paragraph]) -> None:
+    def add_row(self, row: Iterable[str | Inline | Paragraph]) -> Table:
         """
         A convenience method which adds a row to the end of table.
         Use this method to build a table row-by-row rather than constructing
         the table rows upfront.  
-
-        .. code-block:: Python
-
-            table.add_row(["3rd", "Matthews"])
+        
+        .. doctest:: table
+        
+            >>> table = Table(["Rank", "Player"], [["1st", "Crosby"], ["2nd", "McDavid"]])
+            >>> table.add_row(["3rd", "Matthews"])
+            <snakemd.elements.Table object at ...>
+            >>> str(table)
+            '| Rank | Player   |\\n| ---- | -------- |\\n| 1st  | Crosby   |\\n| 2nd  | McDavid  |\\n| 3rd  | Matthews |'
 
         :raises ValueError: 
             when row is not the same width as the table header
         :param Iterable[str | Inline | Paragraph] row: 
             a row of data
+        :return:
+            self
         """
+
+        # Consume row
+        row_list = [_ for _ in row]
+        logger.debug(f"Adding row to table: {row_list}")
+        
+        # Verify that it's safe to add
         if len(row) != len(self._header):
             raise ValueError(
-                f"Unable to add row with width {len(row)} to table with header of width {len(self._header)}"
+                f"Unable to add row with width {len(row_list)} to table with header of width {len(self._header)}"
             )
-        logger.debug(f"Adding row to table: {row}")
-        self._body.append(row)
+        
+        # Add it to table
+        self._body.append(row_list)
+        
+        # Update widths as needed
+        for i, item in enumerate(row_list):
+            item_width = len(str(item))
+            if item_width > self._widths[i]:
+                self._widths[i] = item_width
+
+        return self
```

### Comparing `SnakeMD-2.0.0b1/snakemd/templates.py` & `SnakeMD-2.0.0b2/snakemd/templates.py`

 * *Files identical despite different names*

### Comparing `SnakeMD-2.0.0b1/tests/test_code.py` & `SnakeMD-2.0.0b2/tests/test_code.py`

 * *Files identical despite different names*

### Comparing `SnakeMD-2.0.0b1/tests/test_document.py` & `SnakeMD-2.0.0b2/tests/test_document.py`

 * *Files identical despite different names*

### Comparing `SnakeMD-2.0.0b1/tests/test_heading.py` & `SnakeMD-2.0.0b2/tests/test_heading.py`

 * *Files identical despite different names*

### Comparing `SnakeMD-2.0.0b1/tests/test_inline.py` & `SnakeMD-2.0.0b2/tests/test_inline.py`

 * *Files identical despite different names*

### Comparing `SnakeMD-2.0.0b1/tests/test_md_list.py` & `SnakeMD-2.0.0b2/tests/test_md_list.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import markdown
+import pytest
 
 from snakemd import Code, Heading, HorizontalRule, Inline, MDList, Paragraph
 
 # Constructor tests (Unordered)
 
 
 def test_md_list_empty():
@@ -249,7 +250,51 @@
             "Characters", 
             inner_list, 
             "Powers"
         ], 
         checked=[False, True]
     )
     assert str(outer_list) == "- [ ] Characters\n  - [X] Deku\n  - [X] Bakugo\n  - [ ] Uraraka\n- [X] Powers"
+    
+    
+def test_md_list_checked_exception_list():
+    with pytest.raises(ValueError):
+        MDList(
+            [
+                "Deku", 
+                "Bakugo", 
+                "Uraraka"
+            ], 
+            checked=[True, True]
+        )
+        
+
+def test_md_list_checked_exception_iterable():
+    with pytest.raises(ValueError):
+        MDList(
+            [
+                "Deku", 
+                "Bakugo", 
+                "Uraraka"
+            ], 
+            checked=(x for x in [True, True])
+        )
+
+    
+def test_md_list_nested_checked_nested_exception_list():
+    with pytest.raises(ValueError):
+        inner_list = MDList(
+            [
+                "Deku", 
+                "Bakugo", 
+                "Uraraka"
+            ], 
+            checked=[True, True, False]
+        )
+        MDList(
+            [
+                "Characters", 
+                inner_list, 
+                "Powers"
+            ], 
+            checked=[False, True, False]
+        )
```

### Comparing `SnakeMD-2.0.0b1/tests/test_paragraph.py` & `SnakeMD-2.0.0b2/tests/test_paragraph.py`

 * *Files identical despite different names*

### Comparing `SnakeMD-2.0.0b1/tests/test_quote.py` & `SnakeMD-2.0.0b2/tests/test_quote.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 from snakemd import Quote, Heading, Code, HorizontalRule, MDList
 
 
 def test_quote_one_str():
     quote = Quote("Single Phrase")
     assert str(quote) == "> Single Phrase"
     
+    
+def test_quote_one_str_formatted():
+    quote = Quote("Single Phrase\n\tLet's go!")
+    assert str(quote) == "> Single Phrase\n> \tLet's go!"
+    
 
 def test_quote_multiple_lines():
     quote = Quote(["First", "Second", "Third"])
     assert str(quote) == "> First\n> Second\n> Third"
     
 
 def test_quote_nested():
```

### Comparing `SnakeMD-2.0.0b1/tests/test_table.py` & `SnakeMD-2.0.0b2/tests/test_table.py`

 * *Files identical despite different names*

### Comparing `SnakeMD-2.0.0b1/tests/test_table_of_contents.py` & `SnakeMD-2.0.0b2/tests/test_table_of_contents.py`

 * *Files identical despite different names*

