# Comparing `tmp/packagelister-1.2.0.tar.gz` & `tmp/packagelister-1.3.0.tar.gz`

## Comparing `packagelister-1.2.0.tar` & `packagelister-1.3.0.tar`

### file list

```diff
@@ -1,14 +1,16 @@
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 packagelister-1.2.0/CHANGELOG.md
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 packagelister-1.2.0/docs/index.html
--rw-r--r--   0        0        0    34190 2020-02-02 00:00:00.000000 packagelister-1.2.0/docs/packagelister.html
--rw-r--r--   0        0        0    21653 2020-02-02 00:00:00.000000 packagelister-1.2.0/docs/search.js
--rw-r--r--   0        0        0    69384 2020-02-02 00:00:00.000000 packagelister-1.2.0/docs/packagelister/packagelister.html
--rw-r--r--   0        0        0    74342 2020-02-02 00:00:00.000000 packagelister-1.2.0/docs/packagelister/packagelister_cli.html
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 packagelister-1.2.0/src/packagelister/__init__.py
--rw-r--r--   0        0        0     2973 2020-02-02 00:00:00.000000 packagelister-1.2.0/src/packagelister/packagelister.py
--rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 packagelister-1.2.0/src/packagelister/packagelister_cli.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 packagelister-1.2.0/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 packagelister-1.2.0/LICENSE.txt
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 packagelister-1.2.0/README.md
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 packagelister-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 packagelister-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 packagelister-1.3.0/CHANGELOG.md
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 packagelister-1.3.0/docs/index.html
+-rw-r--r--   0        0        0    34264 2020-02-02 00:00:00.000000 packagelister-1.3.0/docs/packagelister.html
+-rw-r--r--   0        0        0    23684 2020-02-02 00:00:00.000000 packagelister-1.3.0/docs/search.js
+-rw-r--r--   0        0        0    69384 2020-02-02 00:00:00.000000 packagelister-1.3.0/docs/packagelister/packagelister.html
+-rw-r--r--   0        0        0    74342 2020-02-02 00:00:00.000000 packagelister-1.3.0/docs/packagelister/packagelister_cli.html
+-rw-r--r--   0        0        0    56419 2020-02-02 00:00:00.000000 packagelister-1.3.0/docs/packagelister/whouses.html
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 packagelister-1.3.0/src/packagelister/__init__.py
+-rw-r--r--   0        0        0     2973 2020-02-02 00:00:00.000000 packagelister-1.3.0/src/packagelister/packagelister.py
+-rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 packagelister-1.3.0/src/packagelister/packagelister_cli.py
+-rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 packagelister-1.3.0/src/packagelister/whouses.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 packagelister-1.3.0/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 packagelister-1.3.0/LICENSE.txt
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 packagelister-1.3.0/README.md
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 packagelister-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 packagelister-1.3.0/PKG-INFO
```

### Comparing `packagelister-1.2.0/docs/packagelister.html` & `packagelister-1.3.0/docs/packagelister.html`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
                    pattern=".+" required>
 
 
         <h2>Submodules</h2>
         <ul>
                 <li><a href="packagelister/packagelister.html">packagelister</a></li>
                 <li><a href="packagelister/packagelister_cli.html">packagelister_cli</a></li>
+                <li><a href="packagelister/whouses.html">whouses</a></li>
         </ul>
 
 
 
         <a class="attribution" title="pdoc: Python API documentation generator" href="https://pdoc.dev" target="_blank">
             built with <span class="visually-hidden">pdoc</span><img
                 alt="pdoc logo"
```

#### html2text {}

```diff
@@ -1,13 +1,14 @@
 
 
   ⁰
 [Unknown INPUT type]
 ***** Submodules *****
     * packagelister
     * packagelister_cli
+    * whouses
 built_with_pdoc[pdoc_logo]
 
 ****** packagelister ******
 ⁰ View Source
 1from .packagelister import scan
```

### Comparing `packagelister-1.2.0/docs/search.js` & `packagelister-1.3.0/docs/search.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -709,14 +709,43 @@
         "fullname": "packagelister.packagelister_cli.main",
         "modulename": "packagelister.packagelister_cli",
         "qualname": "main",
         "kind": "function",
         "doc": "<p></p>\n",
         "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"return-annotation\">):</span></span>",
         "funcdef": "def"
+    }, {
+        "fullname": "packagelister.whouses",
+        "modulename": "packagelister.whouses",
+        "kind": "module",
+        "doc": "<p></p>\n"
+    }, {
+        "fullname": "packagelister.whouses.get_args",
+        "modulename": "packagelister.whouses",
+        "qualname": "get_args",
+        "kind": "function",
+        "doc": "<p></p>\n",
+        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"return-annotation\">) -> <span class=\"n\">argparse</span><span class=\"o\">.</span><span class=\"n\">Namespace</span>:</span></span>",
+        "funcdef": "def"
+    }, {
+        "fullname": "packagelister.whouses.find",
+        "modulename": "packagelister.whouses",
+        "qualname": "find",
+        "kind": "function",
+        "doc": "<p>Find what sub-folders of top_dir, excluding those in ignore, use 'package'.</p>\n",
+        "signature": "<span class=\"signature pdoc-code multiline\">(<span class=\"param\">\t<span class=\"n\">top_dir</span><span class=\"p\">:</span> <span class=\"n\">pathier</span><span class=\"o\">.</span><span class=\"n\">pathier</span><span class=\"o\">.</span><span class=\"n\">Pathier</span>,</span><span class=\"param\">\t<span class=\"n\">package</span><span class=\"p\">:</span> <span class=\"nb\">str</span>,</span><span class=\"param\">\t<span class=\"n\">ignore</span><span class=\"p\">:</span> <span class=\"nb\">list</span><span class=\"p\">[</span><span class=\"nb\">str</span><span class=\"p\">]</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">list</span><span class=\"p\">[</span><span class=\"nb\">str</span><span class=\"p\">]</span>:</span></span>",
+        "funcdef": "def"
+    }, {
+        "fullname": "packagelister.whouses.main",
+        "modulename": "packagelister.whouses",
+        "qualname": "main",
+        "kind": "function",
+        "doc": "<p></p>\n",
+        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">args</span><span class=\"p\">:</span> <span class=\"n\">argparse</span><span class=\"o\">.</span><span class=\"n\">Namespace</span> <span class=\"o\">=</span> <span class=\"kc\">None</span></span><span class=\"return-annotation\">):</span></span>",
+        "funcdef": "def"
     }];
 
     // mirrored in build-search-index.js (part 1)
     // Also split on html tags. this is a cheap heuristic, but good enough.
     elasticlunr.tokenizer.setSeperator(/[\s\-.;&_'"=,()]+|<[^>]*>/);
 
     let searchIndex;
```

### Comparing `packagelister-1.2.0/docs/packagelister/packagelister.html` & `packagelister-1.3.0/docs/packagelister/packagelister.html`

 * *Files identical despite different names*

### Comparing `packagelister-1.2.0/docs/packagelister/packagelister_cli.html` & `packagelister-1.3.0/docs/packagelister/packagelister_cli.html`

 * *Files identical despite different names*

### Comparing `packagelister-1.2.0/src/packagelister/packagelister.py` & `packagelister-1.3.0/src/packagelister/packagelister.py`

 * *Files identical despite different names*

### Comparing `packagelister-1.2.0/src/packagelister/packagelister_cli.py` & `packagelister-1.3.0/src/packagelister/packagelister_cli.py`

 * *Files identical despite different names*

### Comparing `packagelister-1.2.0/LICENSE.txt` & `packagelister-1.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `packagelister-1.2.0/README.md` & `packagelister-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `packagelister-1.2.0/pyproject.toml` & `packagelister-1.3.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -8,63 +8,66 @@
 00000070: 0d0a 6175 7468 6f72 7320 3d20 5b7b 6e61  ..authors = [{na
 00000080: 6d65 3d22 4d61 7474 204d 616e 6573 227d  me="Matt Manes"}
 00000090: 5d0d 0a64 6573 6372 6970 7469 6f6e 203d  ]..description =
 000000a0: 2022 4465 7465 726d 696e 6520 7768 6174   "Determine what
 000000b0: 2033 7264 2d70 6172 7479 2070 6163 6b61   3rd-party packa
 000000c0: 6765 7320 6120 7072 6f6a 6563 7420 696d  ges a project im
 000000d0: 706f 7274 732e 220d 0a76 6572 7369 6f6e  ports."..version
-000000e0: 203d 2022 312e 322e 3022 0d0a 7265 7175   = "1.2.0"..requ
+000000e0: 203d 2022 312e 332e 3022 0d0a 7265 7175   = "1.3.0"..requ
 000000f0: 6972 6573 2d70 7974 686f 6e20 3d20 223e  ires-python = ">
 00000100: 3d33 2e31 3022 0d0a 6465 7065 6e64 656e  =3.10"..dependen
 00000110: 6369 6573 203d 205b 2270 6174 6863 7261  cies = ["pathcra
 00000120: 776c 6572 222c 2022 7072 696e 7462 7564  wler", "printbud
-00000130: 6469 6573 222c 2022 7079 7465 7374 225d  dies", "pytest"]
-00000140: 0d0a 7265 6164 6d65 203d 2022 5245 4144  ..readme = "READ
-00000150: 4d45 2e6d 6422 0d0a 6b65 7977 6f72 6473  ME.md"..keywords
-00000160: 203d 205b 0d0a 0922 7061 636b 6167 6522   = [..."package"
-00000170: 2c0d 0a09 2269 6d70 6f72 7422 2c0d 0a09  ,..."import",...
-00000180: 226d 6f64 756c 6522 0d0a 2020 2020 5d0d  "module"..    ].
-00000190: 0a63 6c61 7373 6966 6965 7273 203d 205b  .classifiers = [
-000001a0: 0d0a 2020 2020 2250 726f 6772 616d 6d69  ..    "Programmi
-000001b0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-000001c0: 7974 686f 6e20 3a3a 2033 222c 0d0a 2020  ython :: 3",..  
-000001d0: 2020 224c 6963 656e 7365 203a 3a20 4f53    "License :: OS
-000001e0: 4920 4170 7072 6f76 6564 203a 3a20 4d49  I Approved :: MI
-000001f0: 5420 4c69 6365 6e73 6522 2c0d 0a20 2020  T License",..   
-00000200: 2022 4f70 6572 6174 696e 6720 5379 7374   "Operating Syst
-00000210: 656d 203a 3a20 4f53 2049 6e64 6570 656e  em :: OS Indepen
-00000220: 6465 6e74 222c 0d0a 2020 2020 5d0d 0a0d  dent",..    ]...
-00000230: 0a5b 7072 6f6a 6563 742e 7572 6c73 5d0d  .[project.urls].
-00000240: 0a22 486f 6d65 7061 6765 2220 3d20 2268  ."Homepage" = "h
-00000250: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000260: 6d2f 6d61 7474 2d6d 616e 6573 2f70 6163  m/matt-manes/pac
-00000270: 6b61 6765 6c69 7374 6572 220d 0a22 446f  kagelister".."Do
-00000280: 6375 6d65 6e74 6174 696f 6e22 203d 2022  cumentation" = "
-00000290: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000002a0: 6f6d 2f6d 6174 742d 6d61 6e65 732f 7061  om/matt-manes/pa
-000002b0: 636b 6167 656c 6973 7465 722f 7472 6565  ckagelister/tree
-000002c0: 2f6d 6169 6e2f 646f 6373 220d 0a22 536f  /main/docs".."So
-000002d0: 7572 6365 2063 6f64 6522 203d 2022 6874  urce code" = "ht
-000002e0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-000002f0: 2f6d 6174 742d 6d61 6e65 732f 7061 636b  /matt-manes/pack
-00000300: 6167 656c 6973 7465 722f 7472 6565 2f6d  agelister/tree/m
-00000310: 6169 6e2f 7372 632f 7061 636b 6167 656c  ain/src/packagel
-00000320: 6973 7465 7222 0d0a 0d0a 5b70 726f 6a65  ister"....[proje
-00000330: 6374 2e73 6372 6970 7473 5d0d 0a70 6163  ct.scripts]..pac
-00000340: 6b61 6765 6c69 7374 6572 203d 2022 7061  kagelister = "pa
-00000350: 636b 6167 656c 6973 7465 722e 7061 636b  ckagelister.pack
-00000360: 6167 656c 6973 7465 725f 636c 693a 6d61  agelister_cli:ma
-00000370: 696e 220d 0a0d 0a5b 746f 6f6c 2e70 7974  in"....[tool.pyt
-00000380: 6573 742e 696e 695f 6f70 7469 6f6e 735d  est.ini_options]
-00000390: 0d0a 6164 646f 7074 7320 3d20 5b0d 0a20  ..addopts = [.. 
-000003a0: 2020 2022 2d2d 696d 706f 7274 2d6d 6f64     "--import-mod
-000003b0: 653d 696d 706f 7274 6c69 6222 2c0d 0a20  e=importlib",.. 
-000003c0: 2020 205d 0d0a 7079 7468 6f6e 7061 7468     ]..pythonpath
-000003d0: 203d 2022 7372 6322 0d0a 0d0a 5b74 6f6f   = "src"....[too
-000003e0: 6c2e 6861 7463 682e 6275 696c 642e 7461  l.hatch.build.ta
-000003f0: 7267 6574 732e 7364 6973 745d 0d0a 6578  rgets.sdist]..ex
-00000400: 636c 7564 6520 3d20 5b0d 0a20 2020 2022  clude = [..    "
-00000410: 2e63 6f76 6572 6167 6522 2c0d 0a20 2020  .coverage",..   
-00000420: 2022 2e70 7974 6573 745f 6361 6368 6522   ".pytest_cache"
-00000430: 2c0d 0a20 2020 2022 2e76 7363 6f64 6522  ,..    ".vscode"
-00000440: 2c0d 0a20 2020 2022 7465 7374 7322 0d0a  ,..    "tests"..
-00000450: 2020 2020 5d                                 ]
+00000130: 6469 6573 222c 2022 7079 7465 7374 222c  dies", "pytest",
+00000140: 2022 7061 7468 6965 7222 5d0d 0a72 6561   "pathier"]..rea
+00000150: 646d 6520 3d20 2252 4541 444d 452e 6d64  dme = "README.md
+00000160: 220d 0a6b 6579 776f 7264 7320 3d20 5b0d  "..keywords = [.
+00000170: 0a09 2270 6163 6b61 6765 222c 0d0a 0922  .."package",..."
+00000180: 696d 706f 7274 222c 0d0a 0922 6d6f 6475  import",..."modu
+00000190: 6c65 220d 0a20 2020 205d 0d0a 636c 6173  le"..    ]..clas
+000001a0: 7369 6669 6572 7320 3d20 5b0d 0a20 2020  sifiers = [..   
+000001b0: 2022 5072 6f67 7261 6d6d 696e 6720 4c61   "Programming La
+000001c0: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+000001d0: 203a 3a20 3322 2c0d 0a20 2020 2022 4c69   :: 3",..    "Li
+000001e0: 6365 6e73 6520 3a3a 204f 5349 2041 7070  cense :: OSI App
+000001f0: 726f 7665 6420 3a3a 204d 4954 204c 6963  roved :: MIT Lic
+00000200: 656e 7365 222c 0d0a 2020 2020 224f 7065  ense",..    "Ope
+00000210: 7261 7469 6e67 2053 7973 7465 6d20 3a3a  rating System ::
+00000220: 204f 5320 496e 6465 7065 6e64 656e 7422   OS Independent"
+00000230: 2c0d 0a20 2020 205d 0d0a 0d0a 5b70 726f  ,..    ]....[pro
+00000240: 6a65 6374 2e75 726c 735d 0d0a 2248 6f6d  ject.urls].."Hom
+00000250: 6570 6167 6522 203d 2022 6874 7470 733a  epage" = "https:
+00000260: 2f2f 6769 7468 7562 2e63 6f6d 2f6d 6174  //github.com/mat
+00000270: 742d 6d61 6e65 732f 7061 636b 6167 656c  t-manes/packagel
+00000280: 6973 7465 7222 0d0a 2244 6f63 756d 656e  ister".."Documen
+00000290: 7461 7469 6f6e 2220 3d20 2268 7474 7073  tation" = "https
+000002a0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6d61  ://github.com/ma
+000002b0: 7474 2d6d 616e 6573 2f70 6163 6b61 6765  tt-manes/package
+000002c0: 6c69 7374 6572 2f74 7265 652f 6d61 696e  lister/tree/main
+000002d0: 2f64 6f63 7322 0d0a 2253 6f75 7263 6520  /docs".."Source 
+000002e0: 636f 6465 2220 3d20 2268 7474 7073 3a2f  code" = "https:/
+000002f0: 2f67 6974 6875 622e 636f 6d2f 6d61 7474  /github.com/matt
+00000300: 2d6d 616e 6573 2f70 6163 6b61 6765 6c69  -manes/packageli
+00000310: 7374 6572 2f74 7265 652f 6d61 696e 2f73  ster/tree/main/s
+00000320: 7263 2f70 6163 6b61 6765 6c69 7374 6572  rc/packagelister
+00000330: 220d 0a0d 0a5b 7072 6f6a 6563 742e 7363  "....[project.sc
+00000340: 7269 7074 735d 0d0a 7061 636b 6167 656c  ripts]..packagel
+00000350: 6973 7465 7220 3d20 2270 6163 6b61 6765  ister = "package
+00000360: 6c69 7374 6572 2e70 6163 6b61 6765 6c69  lister.packageli
+00000370: 7374 6572 5f63 6c69 3a6d 6169 6e22 0d0a  ster_cli:main"..
+00000380: 7768 6f75 7365 7320 3d20 2270 6163 6b61  whouses = "packa
+00000390: 6765 6c69 7374 6572 2e77 686f 7573 6573  gelister.whouses
+000003a0: 3a6d 6169 6e22 0d0a 0d0a 5b74 6f6f 6c2e  :main"....[tool.
+000003b0: 7079 7465 7374 2e69 6e69 5f6f 7074 696f  pytest.ini_optio
+000003c0: 6e73 5d0d 0a61 6464 6f70 7473 203d 205b  ns]..addopts = [
+000003d0: 0d0a 2020 2020 222d 2d69 6d70 6f72 742d  ..    "--import-
+000003e0: 6d6f 6465 3d69 6d70 6f72 746c 6962 222c  mode=importlib",
+000003f0: 0d0a 2020 2020 5d0d 0a70 7974 686f 6e70  ..    ]..pythonp
+00000400: 6174 6820 3d20 2273 7263 220d 0a0d 0a5b  ath = "src"....[
+00000410: 746f 6f6c 2e68 6174 6368 2e62 7569 6c64  tool.hatch.build
+00000420: 2e74 6172 6765 7473 2e73 6469 7374 5d0d  .targets.sdist].
+00000430: 0a65 7863 6c75 6465 203d 205b 0d0a 2020  .exclude = [..  
+00000440: 2020 222e 636f 7665 7261 6765 222c 0d0a    ".coverage",..
+00000450: 2020 2020 222e 7079 7465 7374 5f63 6163      ".pytest_cac
+00000460: 6865 222c 0d0a 2020 2020 222e 7673 636f  he",..    ".vsco
+00000470: 6465 222c 0d0a 2020 2020 2274 6573 7473  de",..    "tests
+00000480: 220d 0a20 2020 205d                      "..    ]
```

### Comparing `packagelister-1.2.0/PKG-INFO` & `packagelister-1.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: packagelister
-Version: 1.2.0
+Version: 1.3.0
 Summary: Determine what 3rd-party packages a project imports.
 Project-URL: Homepage, https://github.com/matt-manes/packagelister
 Project-URL: Documentation, https://github.com/matt-manes/packagelister/tree/main/docs
 Project-URL: Source code, https://github.com/matt-manes/packagelister/tree/main/src/packagelister
 Author: Matt Manes
 License-File: LICENSE.txt
 Keywords: import,module,package
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: pathcrawler
+Requires-Dist: pathier
 Requires-Dist: printbuddies
 Requires-Dist: pytest
 Description-Content-Type: text/markdown
 
 # packagelister
 Determine what packages and versions a project imports. <br>
 Install with:
```

