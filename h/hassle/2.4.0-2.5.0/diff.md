# Comparing `tmp/hassle-2.4.0.tar.gz` & `tmp/hassle-2.5.0.tar.gz`

## Comparing `hassle-2.4.0.tar` & `hassle-2.5.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 hassle-2.4.0/CHANGELOG.md
--rw-r--r--   0        0        0    33936 2020-02-02 00:00:00.000000 hassle-2.4.0/docs/hassle.html
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 hassle-2.4.0/docs/index.html
--rw-r--r--   0        0        0    40634 2020-02-02 00:00:00.000000 hassle-2.4.0/docs/search.js
--rw-r--r--   0        0        0    93051 2020-02-02 00:00:00.000000 hassle-2.4.0/docs/hassle/generate_tests.html
--rw-r--r--   0        0        0   123141 2020-02-02 00:00:00.000000 hassle-2.4.0/docs/hassle/hassle.html
--rw-r--r--   0        0        0   108137 2020-02-02 00:00:00.000000 hassle-2.4.0/docs/hassle/hassle_config.html
--rw-r--r--   0        0        0   105696 2020-02-02 00:00:00.000000 hassle-2.4.0/docs/hassle/hassle_utilities.html
--rw-r--r--   0        0        0   165865 2020-02-02 00:00:00.000000 hassle-2.4.0/docs/hassle/new_project.html
--rw-r--r--   0        0        0    51897 2020-02-02 00:00:00.000000 hassle-2.4.0/docs/hassle/run_tests.html
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 hassle-2.4.0/src/hassle/.gitignore_template
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 hassle-2.4.0/src/hassle/.vscode_template
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 hassle-2.4.0/src/hassle/README_template.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hassle-2.4.0/src/hassle/__init__.py
--rw-r--r--   0        0        0     4082 2020-02-02 00:00:00.000000 hassle-2.4.0/src/hassle/generate_tests.py
--rw-r--r--   0        0        0     6851 2020-02-02 00:00:00.000000 hassle-2.4.0/src/hassle/hassle.py
--rw-r--r--   0        0        0     5505 2020-02-02 00:00:00.000000 hassle-2.4.0/src/hassle/hassle_config.py
--rw-r--r--   0        0        0     4761 2020-02-02 00:00:00.000000 hassle-2.4.0/src/hassle/hassle_utilities.py
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 hassle-2.4.0/src/hassle/license_template.txt
--rw-r--r--   0        0        0     9213 2020-02-02 00:00:00.000000 hassle-2.4.0/src/hassle/new_project.py
--rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 hassle-2.4.0/src/hassle/pyproject_template.toml
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 hassle-2.4.0/src/hassle/run_tests.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 hassle-2.4.0/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 hassle-2.4.0/LICENSE.txt
--rw-r--r--   0        0        0    22059 2020-02-02 00:00:00.000000 hassle-2.4.0/README.md
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 hassle-2.4.0/pyproject.toml
--rw-r--r--   0        0        0    22561 2020-02-02 00:00:00.000000 hassle-2.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 hassle-2.5.0/CHANGELOG.md
+-rw-r--r--   0        0        0    33936 2020-02-02 00:00:00.000000 hassle-2.5.0/docs/hassle.html
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 hassle-2.5.0/docs/index.html
+-rw-r--r--   0        0        0    41427 2020-02-02 00:00:00.000000 hassle-2.5.0/docs/search.js
+-rw-r--r--   0        0        0    93051 2020-02-02 00:00:00.000000 hassle-2.5.0/docs/hassle/generate_tests.html
+-rw-r--r--   0        0        0   121512 2020-02-02 00:00:00.000000 hassle-2.5.0/docs/hassle/hassle.html
+-rw-r--r--   0        0        0   107599 2020-02-02 00:00:00.000000 hassle-2.5.0/docs/hassle/hassle_config.html
+-rw-r--r--   0        0        0   103640 2020-02-02 00:00:00.000000 hassle-2.5.0/docs/hassle/hassle_utilities.html
+-rw-r--r--   0        0        0   165766 2020-02-02 00:00:00.000000 hassle-2.5.0/docs/hassle/new_project.html
+-rw-r--r--   0        0        0    52052 2020-02-02 00:00:00.000000 hassle-2.5.0/docs/hassle/run_tests.html
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 hassle-2.5.0/src/hassle/.gitignore_template
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 hassle-2.5.0/src/hassle/.vscode_template
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 hassle-2.5.0/src/hassle/README_template.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hassle-2.5.0/src/hassle/__init__.py
+-rw-r--r--   0        0        0     4082 2020-02-02 00:00:00.000000 hassle-2.5.0/src/hassle/generate_tests.py
+-rw-r--r--   0        0        0     6737 2020-02-02 00:00:00.000000 hassle-2.5.0/src/hassle/hassle.py
+-rw-r--r--   0        0        0     5456 2020-02-02 00:00:00.000000 hassle-2.5.0/src/hassle/hassle_config.py
+-rw-r--r--   0        0        0     4579 2020-02-02 00:00:00.000000 hassle-2.5.0/src/hassle/hassle_utilities.py
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 hassle-2.5.0/src/hassle/license_template.txt
+-rw-r--r--   0        0        0     9173 2020-02-02 00:00:00.000000 hassle-2.5.0/src/hassle/new_project.py
+-rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 hassle-2.5.0/src/hassle/pyproject_template.toml
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 hassle-2.5.0/src/hassle/run_tests.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 hassle-2.5.0/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 hassle-2.5.0/LICENSE.txt
+-rw-r--r--   0        0        0    22059 2020-02-02 00:00:00.000000 hassle-2.5.0/README.md
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 hassle-2.5.0/pyproject.toml
+-rw-r--r--   0        0        0    22508 2020-02-02 00:00:00.000000 hassle-2.5.0/PKG-INFO
```

### Comparing `hassle-2.4.0/CHANGELOG.md` & `hassle-2.5.0/CHANGELOG.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,33 @@
 # Changelog
 
-## 2.3.2 (2023-04-02)
+## 2.4.0 (2023-04-07)
+
+#### New Features
+
+* implement manual override for 'tests' location
+* generate_tests cli accepts individual files instead of only directories
+#### Fixes
+
+* add tests_dir.mkdir() to write_placeholders to keep pytest from throwing a fit
+* fix not passing args.tests_dir param to test file generators
+#### Refactorings
+
+* generated test functions will have the form 'test_{function_name}'
+
+
+## v2.3.2 (2023-04-02)
 
 #### Refactorings
 
 * install command will always isntall local copy b/c pypi doesn't update fast enough
+#### Others
+
+* build v2.3.2
+* update changelog
 
 
 ## v2.3.1 (2023-03-31)
 
 #### Fixes
 
 * fix commit_all not adding untracked files in /dist
```

### Comparing `hassle-2.4.0/docs/hassle.html` & `hassle-2.5.0/docs/hassle.html`

 * *Files identical despite different names*

### Comparing `hassle-2.4.0/docs/search.js` & `hassle-2.5.0/docs/search.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -821,55 +821,55 @@
         "doc": "<p></p>\n"
     }, {
         "fullname": "hassle.hassle_utilities.increment_version",
         "modulename": "hassle.hassle_utilities",
         "qualname": "increment_version",
         "kind": "function",
         "doc": "<p>Increment the project.version field in pyproject.toml.</p>\n\n<h6 id=\"parameters\">Parameters</h6>\n\n<ul>\n<li><p><strong>package_path</strong>:  Path to the package/project directory.</p></li>\n<li><p><strong>increment_type</strong>:  One from 'major', 'minor', or 'patch'.</p></li>\n</ul>\n",
-        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">pyproject_path</span><span class=\"p\">:</span> <span class=\"n\">pathlib</span><span class=\"o\">.</span><span class=\"n\">Path</span>, </span><span class=\"param\"><span class=\"n\">increment_type</span><span class=\"p\">:</span> <span class=\"nb\">str</span></span><span class=\"return-annotation\">):</span></span>",
+        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">pyproject_path</span><span class=\"p\">:</span> <span class=\"n\">pathier</span><span class=\"o\">.</span><span class=\"n\">pathier</span><span class=\"o\">.</span><span class=\"n\">Pathier</span>, </span><span class=\"param\"><span class=\"n\">increment_type</span><span class=\"p\">:</span> <span class=\"nb\">str</span></span><span class=\"return-annotation\">):</span></span>",
         "funcdef": "def"
     }, {
         "fullname": "hassle.hassle_utilities.update_minimum_python_version",
         "modulename": "hassle.hassle_utilities",
         "qualname": "update_minimum_python_version",
         "kind": "function",
         "doc": "<p>Use vermin to determine the minimum compatible\nPython version and update the corresponding field\nin pyproject.toml.</p>\n",
-        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">pyproject_path</span><span class=\"p\">:</span> <span class=\"n\">pathlib</span><span class=\"o\">.</span><span class=\"n\">Path</span></span><span class=\"return-annotation\">):</span></span>",
+        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">pyproject_path</span><span class=\"p\">:</span> <span class=\"n\">pathier</span><span class=\"o\">.</span><span class=\"n\">pathier</span><span class=\"o\">.</span><span class=\"n\">Pathier</span></span><span class=\"return-annotation\">):</span></span>",
         "funcdef": "def"
     }, {
         "fullname": "hassle.hassle_utilities.generate_docs",
         "modulename": "hassle.hassle_utilities",
         "qualname": "generate_docs",
         "kind": "function",
         "doc": "<p>Generate project documentation using pdoc.</p>\n",
-        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">package_path</span><span class=\"p\">:</span> <span class=\"n\">pathlib</span><span class=\"o\">.</span><span class=\"n\">Path</span></span><span class=\"return-annotation\">):</span></span>",
+        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">package_path</span><span class=\"p\">:</span> <span class=\"n\">pathier</span><span class=\"o\">.</span><span class=\"n\">pathier</span><span class=\"o\">.</span><span class=\"n\">Pathier</span></span><span class=\"return-annotation\">):</span></span>",
         "funcdef": "def"
     }, {
         "fullname": "hassle.hassle_utilities.update_dependencies",
         "modulename": "hassle.hassle_utilities",
         "qualname": "update_dependencies",
         "kind": "function",
         "doc": "<p>Update dependencies list in pyproject.toml.</p>\n\n<h6 id=\"parameters\">Parameters</h6>\n\n<ul>\n<li><strong>overwrite</strong>:  If True, replace the dependencies in pyproject.toml\nwith the results of packagelister.scan() .\nIf False, packages returned by packagelister are appended to\nthe current dependencies in pyproject.toml if they don't already\nexist in the field.</li>\n</ul>\n",
-        "signature": "<span class=\"signature pdoc-code multiline\">(<span class=\"param\">\t<span class=\"n\">pyproject_path</span><span class=\"p\">:</span> <span class=\"n\">pathlib</span><span class=\"o\">.</span><span class=\"n\">Path</span>,</span><span class=\"param\">\t<span class=\"n\">overwrite</span><span class=\"p\">:</span> <span class=\"nb\">bool</span>,</span><span class=\"param\">\t<span class=\"n\">include_versions</span><span class=\"p\">:</span> <span class=\"nb\">bool</span> <span class=\"o\">=</span> <span class=\"kc\">False</span></span><span class=\"return-annotation\">):</span></span>",
+        "signature": "<span class=\"signature pdoc-code multiline\">(<span class=\"param\">\t<span class=\"n\">pyproject_path</span><span class=\"p\">:</span> <span class=\"n\">pathier</span><span class=\"o\">.</span><span class=\"n\">pathier</span><span class=\"o\">.</span><span class=\"n\">Pathier</span>,</span><span class=\"param\">\t<span class=\"n\">overwrite</span><span class=\"p\">:</span> <span class=\"nb\">bool</span>,</span><span class=\"param\">\t<span class=\"n\">include_versions</span><span class=\"p\">:</span> <span class=\"nb\">bool</span> <span class=\"o\">=</span> <span class=\"kc\">False</span></span><span class=\"return-annotation\">):</span></span>",
         "funcdef": "def"
     }, {
         "fullname": "hassle.hassle_utilities.update_changelog",
         "modulename": "hassle.hassle_utilities",
         "qualname": "update_changelog",
         "kind": "function",
         "doc": "<p>Update project changelog.</p>\n",
-        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">pyproject_path</span><span class=\"p\">:</span> <span class=\"n\">pathlib</span><span class=\"o\">.</span><span class=\"n\">Path</span></span><span class=\"return-annotation\">):</span></span>",
+        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">pyproject_path</span><span class=\"p\">:</span> <span class=\"n\">pathier</span><span class=\"o\">.</span><span class=\"n\">pathier</span><span class=\"o\">.</span><span class=\"n\">Pathier</span></span><span class=\"return-annotation\">):</span></span>",
         "funcdef": "def"
     }, {
         "fullname": "hassle.hassle_utilities.tag_version",
         "modulename": "hassle.hassle_utilities",
         "qualname": "tag_version",
         "kind": "function",
         "doc": "<p>Add a git tag corresponding\nto the version number in pyproject.toml.</p>\n",
-        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">package_path</span><span class=\"p\">:</span> <span class=\"n\">pathlib</span><span class=\"o\">.</span><span class=\"n\">Path</span></span><span class=\"return-annotation\">):</span></span>",
+        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">package_path</span><span class=\"p\">:</span> <span class=\"n\">pathier</span><span class=\"o\">.</span><span class=\"n\">pathier</span><span class=\"o\">.</span><span class=\"n\">Pathier</span></span><span class=\"return-annotation\">):</span></span>",
         "funcdef": "def"
     }, {
         "fullname": "hassle.new_project",
         "modulename": "hassle.new_project",
         "kind": "module",
         "doc": "<p></p>\n"
     }, {
@@ -906,55 +906,55 @@
         "funcdef": "def"
     }, {
         "fullname": "hassle.new_project.create_pyproject_file",
         "modulename": "hassle.new_project",
         "qualname": "create_pyproject_file",
         "kind": "function",
         "doc": "<p>Create pyproject.toml in ./{project_name} from args,\npyproject_template, and hassle_config.</p>\n",
-        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">targetdir</span><span class=\"p\">:</span> <span class=\"n\">pathlib</span><span class=\"o\">.</span><span class=\"n\">Path</span>, </span><span class=\"param\"><span class=\"n\">args</span><span class=\"p\">:</span> <span class=\"n\">argparse</span><span class=\"o\">.</span><span class=\"n\">Namespace</span></span><span class=\"return-annotation\">):</span></span>",
+        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">targetdir</span><span class=\"p\">:</span> <span class=\"n\">pathier</span><span class=\"o\">.</span><span class=\"n\">pathier</span><span class=\"o\">.</span><span class=\"n\">Pathier</span>, </span><span class=\"param\"><span class=\"n\">args</span><span class=\"p\">:</span> <span class=\"n\">argparse</span><span class=\"o\">.</span><span class=\"n\">Namespace</span></span><span class=\"return-annotation\">):</span></span>",
         "funcdef": "def"
     }, {
         "fullname": "hassle.new_project.create_source_files",
         "modulename": "hassle.new_project",
         "qualname": "create_source_files",
         "kind": "function",
         "doc": "<p>Generate empty source files in ./{package_name}/src/{package_name}/</p>\n",
-        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">srcdir</span><span class=\"p\">:</span> <span class=\"n\">pathlib</span><span class=\"o\">.</span><span class=\"n\">Path</span>, </span><span class=\"param\"><span class=\"n\">filelist</span><span class=\"p\">:</span> <span class=\"nb\">list</span><span class=\"p\">[</span><span class=\"nb\">str</span><span class=\"p\">]</span></span><span class=\"return-annotation\">):</span></span>",
+        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">srcdir</span><span class=\"p\">:</span> <span class=\"n\">pathier</span><span class=\"o\">.</span><span class=\"n\">pathier</span><span class=\"o\">.</span><span class=\"n\">Pathier</span>, </span><span class=\"param\"><span class=\"n\">filelist</span><span class=\"p\">:</span> <span class=\"nb\">list</span><span class=\"p\">[</span><span class=\"nb\">str</span><span class=\"p\">]</span></span><span class=\"return-annotation\">):</span></span>",
         "funcdef": "def"
     }, {
         "fullname": "hassle.new_project.create_readme",
         "modulename": "hassle.new_project",
         "qualname": "create_readme",
         "kind": "function",
         "doc": "<p>Create README.md in ./{package_name}\nfrom readme_template and args.</p>\n",
-        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">targetdir</span><span class=\"p\">:</span> <span class=\"n\">pathlib</span><span class=\"o\">.</span><span class=\"n\">Path</span>, </span><span class=\"param\"><span class=\"n\">args</span><span class=\"p\">:</span> <span class=\"n\">argparse</span><span class=\"o\">.</span><span class=\"n\">Namespace</span></span><span class=\"return-annotation\">):</span></span>",
+        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">targetdir</span><span class=\"p\">:</span> <span class=\"n\">pathier</span><span class=\"o\">.</span><span class=\"n\">pathier</span><span class=\"o\">.</span><span class=\"n\">Pathier</span>, </span><span class=\"param\"><span class=\"n\">args</span><span class=\"p\">:</span> <span class=\"n\">argparse</span><span class=\"o\">.</span><span class=\"n\">Namespace</span></span><span class=\"return-annotation\">):</span></span>",
         "funcdef": "def"
     }, {
         "fullname": "hassle.new_project.create_license",
         "modulename": "hassle.new_project",
         "qualname": "create_license",
         "kind": "function",
         "doc": "<p>Add MIT license file to ./{package_name} .</p>\n",
-        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">targetdir</span><span class=\"p\">:</span> <span class=\"n\">pathlib</span><span class=\"o\">.</span><span class=\"n\">Path</span></span><span class=\"return-annotation\">):</span></span>",
+        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">targetdir</span><span class=\"p\">:</span> <span class=\"n\">pathier</span><span class=\"o\">.</span><span class=\"n\">pathier</span><span class=\"o\">.</span><span class=\"n\">Pathier</span></span><span class=\"return-annotation\">):</span></span>",
         "funcdef": "def"
     }, {
         "fullname": "hassle.new_project.create_gitignore",
         "modulename": "hassle.new_project",
         "qualname": "create_gitignore",
         "kind": "function",
         "doc": "<p>Add .gitignore to ./{package_name}</p>\n",
-        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">targetdir</span><span class=\"p\">:</span> <span class=\"n\">pathlib</span><span class=\"o\">.</span><span class=\"n\">Path</span></span><span class=\"return-annotation\">):</span></span>",
+        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">targetdir</span><span class=\"p\">:</span> <span class=\"n\">pathier</span><span class=\"o\">.</span><span class=\"n\">pathier</span><span class=\"o\">.</span><span class=\"n\">Pathier</span></span><span class=\"return-annotation\">):</span></span>",
         "funcdef": "def"
     }, {
         "fullname": "hassle.new_project.create_vscode_settings",
         "modulename": "hassle.new_project",
         "qualname": "create_vscode_settings",
         "kind": "function",
         "doc": "<p>Add settings.json to ./.vscode</p>\n",
-        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">targetdir</span><span class=\"p\">:</span> <span class=\"n\">pathlib</span><span class=\"o\">.</span><span class=\"n\">Path</span></span><span class=\"return-annotation\">):</span></span>",
+        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">targetdir</span><span class=\"p\">:</span> <span class=\"n\">pathier</span><span class=\"o\">.</span><span class=\"n\">pathier</span><span class=\"o\">.</span><span class=\"n\">Pathier</span></span><span class=\"return-annotation\">):</span></span>",
         "funcdef": "def"
     }, {
         "fullname": "hassle.new_project.main",
         "modulename": "hassle.new_project",
         "qualname": "main",
         "kind": "function",
         "doc": "<p></p>\n",
@@ -975,15 +975,15 @@
         "funcdef": "def"
     }, {
         "fullname": "hassle.run_tests.run_tests",
         "modulename": "hassle.run_tests",
         "qualname": "run_tests",
         "kind": "function",
         "doc": "<p>Run tests with coverage and pytest.</p>\n",
-        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">package_path</span><span class=\"p\">:</span> <span class=\"n\">pathlib</span><span class=\"o\">.</span><span class=\"n\">Path</span></span><span class=\"return-annotation\">):</span></span>",
+        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">package_path</span><span class=\"p\">:</span> <span class=\"n\">pathier</span><span class=\"o\">.</span><span class=\"n\">pathier</span><span class=\"o\">.</span><span class=\"n\">Pathier</span></span><span class=\"return-annotation\">):</span></span>",
         "funcdef": "def"
     }, {
         "fullname": "hassle.run_tests.main",
         "modulename": "hassle.run_tests",
         "qualname": "main",
         "kind": "function",
         "doc": "<p></p>\n",
```

### Comparing `hassle-2.4.0/docs/hassle/generate_tests.html` & `hassle-2.5.0/docs/hassle/generate_tests.html`

 * *Files identical despite different names*

### Comparing `hassle-2.4.0/docs/hassle/hassle.html` & `hassle-2.5.0/docs/hassle/hassle.html`

 * *Files 0% similar despite different names*

```diff
@@ -55,241 +55,236 @@
                 
                         <input id="mod-hassle-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 
                         <label class="view-source-button" for="mod-hassle-view-source"><span>View Source</span></label>
 
                         <div class="pdoc-code codehilite"><pre><span></span><span id="L-1"><a href="#L-1"><span class="linenos">  1</span></a><span class="kn">import</span> <span class="nn">argparse</span>
 </span><span id="L-2"><a href="#L-2"><span class="linenos">  2</span></a><span class="kn">import</span> <span class="nn">os</span>
-</span><span id="L-3"><a href="#L-3"><span class="linenos">  3</span></a><span class="kn">import</span> <span class="nn">shutil</span>
-</span><span id="L-4"><a href="#L-4"><span class="linenos">  4</span></a><span class="kn">from</span> <span class="nn">pathlib</span> <span class="kn">import</span> <span class="n">Path</span>
+</span><span id="L-3"><a href="#L-3"><span class="linenos">  3</span></a>
+</span><span id="L-4"><a href="#L-4"><span class="linenos">  4</span></a><span class="kn">from</span> <span class="nn">pathier</span> <span class="kn">import</span> <span class="n">Pathier</span>
 </span><span id="L-5"><a href="#L-5"><span class="linenos">  5</span></a>
-</span><span id="L-6"><a href="#L-6"><span class="linenos">  6</span></a><span class="kn">import</span> <span class="nn">tomlkit</span>
-</span><span id="L-7"><a href="#L-7"><span class="linenos">  7</span></a>
-</span><span id="L-8"><a href="#L-8"><span class="linenos">  8</span></a><span class="kn">from</span> <span class="nn">hassle</span> <span class="kn">import</span> <span class="n">hassle_utilities</span>
-</span><span id="L-9"><a href="#L-9"><span class="linenos">  9</span></a><span class="kn">from</span> <span class="nn">hassle.generate_tests</span> <span class="kn">import</span> <span class="n">generate_test_files</span>
-</span><span id="L-10"><a href="#L-10"><span class="linenos"> 10</span></a><span class="kn">from</span> <span class="nn">hassle.run_tests</span> <span class="kn">import</span> <span class="n">run_tests</span>
+</span><span id="L-6"><a href="#L-6"><span class="linenos">  6</span></a><span class="kn">from</span> <span class="nn">hassle</span> <span class="kn">import</span> <span class="n">hassle_utilities</span>
+</span><span id="L-7"><a href="#L-7"><span class="linenos">  7</span></a><span class="kn">from</span> <span class="nn">hassle.generate_tests</span> <span class="kn">import</span> <span class="n">generate_test_files</span>
+</span><span id="L-8"><a href="#L-8"><span class="linenos">  8</span></a><span class="kn">from</span> <span class="nn">hassle.run_tests</span> <span class="kn">import</span> <span class="n">run_tests</span>
+</span><span id="L-9"><a href="#L-9"><span class="linenos">  9</span></a>
+</span><span id="L-10"><a href="#L-10"><span class="linenos"> 10</span></a><span class="n">root</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="vm">__file__</span><span class="p">)</span><span class="o">.</span><span class="n">parent</span>
 </span><span id="L-11"><a href="#L-11"><span class="linenos"> 11</span></a>
-</span><span id="L-12"><a href="#L-12"><span class="linenos"> 12</span></a><span class="n">root</span> <span class="o">=</span> <span class="n">Path</span><span class="p">(</span><span class="vm">__file__</span><span class="p">)</span><span class="o">.</span><span class="n">parent</span>
-</span><span id="L-13"><a href="#L-13"><span class="linenos"> 13</span></a>
-</span><span id="L-14"><a href="#L-14"><span class="linenos"> 14</span></a>
-</span><span id="L-15"><a href="#L-15"><span class="linenos"> 15</span></a><span class="k">def</span> <span class="nf">get_args</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">:</span>
-</span><span id="L-16"><a href="#L-16"><span class="linenos"> 16</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">argparse</span><span class="o">.</span><span class="n">ArgumentParser</span><span class="p">()</span>
-</span><span id="L-17"><a href="#L-17"><span class="linenos"> 17</span></a>
-</span><span id="L-18"><a href="#L-18"><span class="linenos"> 18</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-19"><a href="#L-19"><span class="linenos"> 19</span></a>        <span class="s2">&quot;package&quot;</span><span class="p">,</span>
-</span><span id="L-20"><a href="#L-20"><span class="linenos"> 20</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
-</span><span id="L-21"><a href="#L-21"><span class="linenos"> 21</span></a>        <span class="n">default</span><span class="o">=</span><span class="s2">&quot;.&quot;</span><span class="p">,</span>
-</span><span id="L-22"><a href="#L-22"><span class="linenos"> 22</span></a>        <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;?&quot;</span><span class="p">,</span>
-</span><span id="L-23"><a href="#L-23"><span class="linenos"> 23</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; The name of the package or project to use,</span>
-</span><span id="L-24"><a href="#L-24"><span class="linenos"> 24</span></a><span class="s2">        assuming it&#39;s a subfolder of your current working directory.</span>
-</span><span id="L-25"><a href="#L-25"><span class="linenos"> 25</span></a><span class="s2">        Can also be a full path to the package. If nothing is given,</span>
-</span><span id="L-26"><a href="#L-26"><span class="linenos"> 26</span></a><span class="s2">        the current working directory will be used.&quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-27"><a href="#L-27"><span class="linenos"> 27</span></a>    <span class="p">)</span>
-</span><span id="L-28"><a href="#L-28"><span class="linenos"> 28</span></a>
-</span><span id="L-29"><a href="#L-29"><span class="linenos"> 29</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-30"><a href="#L-30"><span class="linenos"> 30</span></a>        <span class="s2">&quot;-b&quot;</span><span class="p">,</span> <span class="s2">&quot;--build&quot;</span><span class="p">,</span> <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span> <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Build the package. &quot;&quot;&quot;</span>
-</span><span id="L-31"><a href="#L-31"><span class="linenos"> 31</span></a>    <span class="p">)</span>
-</span><span id="L-32"><a href="#L-32"><span class="linenos"> 32</span></a>
-</span><span id="L-33"><a href="#L-33"><span class="linenos"> 33</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-34"><a href="#L-34"><span class="linenos"> 34</span></a>        <span class="s2">&quot;-t&quot;</span><span class="p">,</span>
-</span><span id="L-35"><a href="#L-35"><span class="linenos"> 35</span></a>        <span class="s2">&quot;--tag_version&quot;</span><span class="p">,</span>
-</span><span id="L-36"><a href="#L-36"><span class="linenos"> 36</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
-</span><span id="L-37"><a href="#L-37"><span class="linenos"> 37</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Add a git tag corresponding to the version in pyproject.toml. &quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-38"><a href="#L-38"><span class="linenos"> 38</span></a>    <span class="p">)</span>
-</span><span id="L-39"><a href="#L-39"><span class="linenos"> 39</span></a>
-</span><span id="L-40"><a href="#L-40"><span class="linenos"> 40</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-41"><a href="#L-41"><span class="linenos"> 41</span></a>        <span class="s2">&quot;-i&quot;</span><span class="p">,</span>
-</span><span id="L-42"><a href="#L-42"><span class="linenos"> 42</span></a>        <span class="s2">&quot;--install&quot;</span><span class="p">,</span>
-</span><span id="L-43"><a href="#L-43"><span class="linenos"> 43</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
-</span><span id="L-44"><a href="#L-44"><span class="linenos"> 44</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Install the package from source. &quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-45"><a href="#L-45"><span class="linenos"> 45</span></a>    <span class="p">)</span>
-</span><span id="L-46"><a href="#L-46"><span class="linenos"> 46</span></a>
-</span><span id="L-47"><a href="#L-47"><span class="linenos"> 47</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-48"><a href="#L-48"><span class="linenos"> 48</span></a>        <span class="s2">&quot;-iv&quot;</span><span class="p">,</span>
-</span><span id="L-49"><a href="#L-49"><span class="linenos"> 49</span></a>        <span class="s2">&quot;--increment_version&quot;</span><span class="p">,</span>
-</span><span id="L-50"><a href="#L-50"><span class="linenos"> 50</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
-</span><span id="L-51"><a href="#L-51"><span class="linenos"> 51</span></a>        <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
-</span><span id="L-52"><a href="#L-52"><span class="linenos"> 52</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Increment version in pyproject.toml.</span>
-</span><span id="L-53"><a href="#L-53"><span class="linenos"> 53</span></a><span class="s2">        Can be one of &quot;major&quot;, &quot;minor&quot;, or &quot;patch&quot;. &quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-54"><a href="#L-54"><span class="linenos"> 54</span></a>    <span class="p">)</span>
-</span><span id="L-55"><a href="#L-55"><span class="linenos"> 55</span></a>
-</span><span id="L-56"><a href="#L-56"><span class="linenos"> 56</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-57"><a href="#L-57"><span class="linenos"> 57</span></a>        <span class="s2">&quot;-p&quot;</span><span class="p">,</span>
-</span><span id="L-58"><a href="#L-58"><span class="linenos"> 58</span></a>        <span class="s2">&quot;--publish&quot;</span><span class="p">,</span>
-</span><span id="L-59"><a href="#L-59"><span class="linenos"> 59</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
-</span><span id="L-60"><a href="#L-60"><span class="linenos"> 60</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Publish package to PyPi.</span>
-</span><span id="L-61"><a href="#L-61"><span class="linenos"> 61</span></a><span class="s2">        Note: You must have configured twine </span>
-</span><span id="L-62"><a href="#L-62"><span class="linenos"> 62</span></a><span class="s2">        and registered a PyPi account/generated an API</span>
-</span><span id="L-63"><a href="#L-63"><span class="linenos"> 63</span></a><span class="s2">        key to use this option.&quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-64"><a href="#L-64"><span class="linenos"> 64</span></a>    <span class="p">)</span>
-</span><span id="L-65"><a href="#L-65"><span class="linenos"> 65</span></a>
-</span><span id="L-66"><a href="#L-66"><span class="linenos"> 66</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-67"><a href="#L-67"><span class="linenos"> 67</span></a>        <span class="s2">&quot;-rt&quot;</span><span class="p">,</span>
-</span><span id="L-68"><a href="#L-68"><span class="linenos"> 68</span></a>        <span class="s2">&quot;--run_tests&quot;</span><span class="p">,</span>
-</span><span id="L-69"><a href="#L-69"><span class="linenos"> 69</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
-</span><span id="L-70"><a href="#L-70"><span class="linenos"> 70</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Run tests for the package. &quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-71"><a href="#L-71"><span class="linenos"> 71</span></a>    <span class="p">)</span>
-</span><span id="L-72"><a href="#L-72"><span class="linenos"> 72</span></a>
-</span><span id="L-73"><a href="#L-73"><span class="linenos"> 73</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-74"><a href="#L-74"><span class="linenos"> 74</span></a>        <span class="s2">&quot;-gt&quot;</span><span class="p">,</span>
-</span><span id="L-75"><a href="#L-75"><span class="linenos"> 75</span></a>        <span class="s2">&quot;--generate_tests&quot;</span><span class="p">,</span>
-</span><span id="L-76"><a href="#L-76"><span class="linenos"> 76</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
-</span><span id="L-77"><a href="#L-77"><span class="linenos"> 77</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Generate tests for the package. &quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-78"><a href="#L-78"><span class="linenos"> 78</span></a>    <span class="p">)</span>
-</span><span id="L-79"><a href="#L-79"><span class="linenos"> 79</span></a>
-</span><span id="L-80"><a href="#L-80"><span class="linenos"> 80</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-81"><a href="#L-81"><span class="linenos"> 81</span></a>        <span class="s2">&quot;-uc&quot;</span><span class="p">,</span>
-</span><span id="L-82"><a href="#L-82"><span class="linenos"> 82</span></a>        <span class="s2">&quot;--update_changelog&quot;</span><span class="p">,</span>
-</span><span id="L-83"><a href="#L-83"><span class="linenos"> 83</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
-</span><span id="L-84"><a href="#L-84"><span class="linenos"> 84</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Update changelog file. &quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-85"><a href="#L-85"><span class="linenos"> 85</span></a>    <span class="p">)</span>
-</span><span id="L-86"><a href="#L-86"><span class="linenos"> 86</span></a>
-</span><span id="L-87"><a href="#L-87"><span class="linenos"> 87</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-88"><a href="#L-88"><span class="linenos"> 88</span></a>        <span class="s2">&quot;-od&quot;</span><span class="p">,</span>
-</span><span id="L-89"><a href="#L-89"><span class="linenos"> 89</span></a>        <span class="s2">&quot;--overwrite_dependencies&quot;</span><span class="p">,</span>
-</span><span id="L-90"><a href="#L-90"><span class="linenos"> 90</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
-</span><span id="L-91"><a href="#L-91"><span class="linenos"> 91</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; When building a package, packagelister will be used</span>
-</span><span id="L-92"><a href="#L-92"><span class="linenos"> 92</span></a><span class="s2">        to update the dependencies list in pyproject.toml.</span>
-</span><span id="L-93"><a href="#L-93"><span class="linenos"> 93</span></a><span class="s2">        The default behavior is to append any new dependencies to</span>
-</span><span id="L-94"><a href="#L-94"><span class="linenos"> 94</span></a><span class="s2">        the current list so as not to erase any manually added dependencies</span>
-</span><span id="L-95"><a href="#L-95"><span class="linenos"> 95</span></a><span class="s2">        that packagelister may not detect. If you don&#39;t have any manually </span>
-</span><span id="L-96"><a href="#L-96"><span class="linenos"> 96</span></a><span class="s2">        added dependencies and want to remove any dependencies that your</span>
-</span><span id="L-97"><a href="#L-97"><span class="linenos"> 97</span></a><span class="s2">        project no longer uses, pass this flag.&quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-98"><a href="#L-98"><span class="linenos"> 98</span></a>    <span class="p">)</span>
-</span><span id="L-99"><a href="#L-99"><span class="linenos"> 99</span></a>
-</span><span id="L-100"><a href="#L-100"><span class="linenos">100</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-101"><a href="#L-101"><span class="linenos">101</span></a>        <span class="s2">&quot;-ca&quot;</span><span class="p">,</span>
-</span><span id="L-102"><a href="#L-102"><span class="linenos">102</span></a>        <span class="s2">&quot;--commit_all&quot;</span><span class="p">,</span>
-</span><span id="L-103"><a href="#L-103"><span class="linenos">103</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
-</span><span id="L-104"><a href="#L-104"><span class="linenos">104</span></a>        <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
-</span><span id="L-105"><a href="#L-105"><span class="linenos">105</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Git stage and commit all tracked files</span>
-</span><span id="L-106"><a href="#L-106"><span class="linenos">106</span></a><span class="s2">        with this supplied commit message.</span>
-</span><span id="L-107"><a href="#L-107"><span class="linenos">107</span></a><span class="s2">        If &#39;build&#39; is passed, all commits will have</span>
-</span><span id="L-108"><a href="#L-108"><span class="linenos">108</span></a><span class="s2">        message: &#39;chore: build v</span><span class="si">{current_version}</span><span class="s2">&quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-109"><a href="#L-109"><span class="linenos">109</span></a>    <span class="p">)</span>
-</span><span id="L-110"><a href="#L-110"><span class="linenos">110</span></a>
-</span><span id="L-111"><a href="#L-111"><span class="linenos">111</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-112"><a href="#L-112"><span class="linenos">112</span></a>        <span class="s2">&quot;-s&quot;</span><span class="p">,</span>
-</span><span id="L-113"><a href="#L-113"><span class="linenos">113</span></a>        <span class="s2">&quot;--sync&quot;</span><span class="p">,</span>
-</span><span id="L-114"><a href="#L-114"><span class="linenos">114</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
-</span><span id="L-115"><a href="#L-115"><span class="linenos">115</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Pull from github, then push current commit to repo. &quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-116"><a href="#L-116"><span class="linenos">116</span></a>    <span class="p">)</span>
-</span><span id="L-117"><a href="#L-117"><span class="linenos">117</span></a>
-</span><span id="L-118"><a href="#L-118"><span class="linenos">118</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-119"><a href="#L-119"><span class="linenos">119</span></a>        <span class="s2">&quot;-dv&quot;</span><span class="p">,</span>
-</span><span id="L-120"><a href="#L-120"><span class="linenos">120</span></a>        <span class="s2">&quot;--dependency_versions&quot;</span><span class="p">,</span>
-</span><span id="L-121"><a href="#L-121"><span class="linenos">121</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
-</span><span id="L-122"><a href="#L-122"><span class="linenos">122</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Include version specifiers for dependencies in</span>
-</span><span id="L-123"><a href="#L-123"><span class="linenos">123</span></a><span class="s2">        pyproject.toml.&quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-124"><a href="#L-124"><span class="linenos">124</span></a>    <span class="p">)</span>
-</span><span id="L-125"><a href="#L-125"><span class="linenos">125</span></a>
-</span><span id="L-126"><a href="#L-126"><span class="linenos">126</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-127"><a href="#L-127"><span class="linenos">127</span></a>        <span class="s2">&quot;-up&quot;</span><span class="p">,</span>
-</span><span id="L-128"><a href="#L-128"><span class="linenos">128</span></a>        <span class="s2">&quot;--update&quot;</span><span class="p">,</span>
-</span><span id="L-129"><a href="#L-129"><span class="linenos">129</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
-</span><span id="L-130"><a href="#L-130"><span class="linenos">130</span></a>        <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
-</span><span id="L-131"><a href="#L-131"><span class="linenos">131</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Excpects one argument: &quot;major&quot;, &quot;minor&quot;, or &quot;patch&quot;.</span>
-</span><span id="L-132"><a href="#L-132"><span class="linenos">132</span></a><span class="s2">        Passing &quot;-up minor&quot; is equivalent to passing the cli string: &quot;-b -t -i -iv minor -uc -ca build -s&quot;.</span>
-</span><span id="L-133"><a href="#L-133"><span class="linenos">133</span></a><span class="s2">        To publish the updated package, the -p/--publish switch needs to be added to the cli input.&quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-134"><a href="#L-134"><span class="linenos">134</span></a>    <span class="p">)</span>
+</span><span id="L-12"><a href="#L-12"><span class="linenos"> 12</span></a>
+</span><span id="L-13"><a href="#L-13"><span class="linenos"> 13</span></a><span class="k">def</span> <span class="nf">get_args</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">:</span>
+</span><span id="L-14"><a href="#L-14"><span class="linenos"> 14</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">argparse</span><span class="o">.</span><span class="n">ArgumentParser</span><span class="p">()</span>
+</span><span id="L-15"><a href="#L-15"><span class="linenos"> 15</span></a>
+</span><span id="L-16"><a href="#L-16"><span class="linenos"> 16</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-17"><a href="#L-17"><span class="linenos"> 17</span></a>        <span class="s2">&quot;package&quot;</span><span class="p">,</span>
+</span><span id="L-18"><a href="#L-18"><span class="linenos"> 18</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
+</span><span id="L-19"><a href="#L-19"><span class="linenos"> 19</span></a>        <span class="n">default</span><span class="o">=</span><span class="s2">&quot;.&quot;</span><span class="p">,</span>
+</span><span id="L-20"><a href="#L-20"><span class="linenos"> 20</span></a>        <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;?&quot;</span><span class="p">,</span>
+</span><span id="L-21"><a href="#L-21"><span class="linenos"> 21</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; The name of the package or project to use,</span>
+</span><span id="L-22"><a href="#L-22"><span class="linenos"> 22</span></a><span class="s2">        assuming it&#39;s a subfolder of your current working directory.</span>
+</span><span id="L-23"><a href="#L-23"><span class="linenos"> 23</span></a><span class="s2">        Can also be a full path to the package. If nothing is given,</span>
+</span><span id="L-24"><a href="#L-24"><span class="linenos"> 24</span></a><span class="s2">        the current working directory will be used.&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-25"><a href="#L-25"><span class="linenos"> 25</span></a>    <span class="p">)</span>
+</span><span id="L-26"><a href="#L-26"><span class="linenos"> 26</span></a>
+</span><span id="L-27"><a href="#L-27"><span class="linenos"> 27</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-28"><a href="#L-28"><span class="linenos"> 28</span></a>        <span class="s2">&quot;-b&quot;</span><span class="p">,</span> <span class="s2">&quot;--build&quot;</span><span class="p">,</span> <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span> <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Build the package. &quot;&quot;&quot;</span>
+</span><span id="L-29"><a href="#L-29"><span class="linenos"> 29</span></a>    <span class="p">)</span>
+</span><span id="L-30"><a href="#L-30"><span class="linenos"> 30</span></a>
+</span><span id="L-31"><a href="#L-31"><span class="linenos"> 31</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-32"><a href="#L-32"><span class="linenos"> 32</span></a>        <span class="s2">&quot;-t&quot;</span><span class="p">,</span>
+</span><span id="L-33"><a href="#L-33"><span class="linenos"> 33</span></a>        <span class="s2">&quot;--tag_version&quot;</span><span class="p">,</span>
+</span><span id="L-34"><a href="#L-34"><span class="linenos"> 34</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="L-35"><a href="#L-35"><span class="linenos"> 35</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Add a git tag corresponding to the version in pyproject.toml. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-36"><a href="#L-36"><span class="linenos"> 36</span></a>    <span class="p">)</span>
+</span><span id="L-37"><a href="#L-37"><span class="linenos"> 37</span></a>
+</span><span id="L-38"><a href="#L-38"><span class="linenos"> 38</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-39"><a href="#L-39"><span class="linenos"> 39</span></a>        <span class="s2">&quot;-i&quot;</span><span class="p">,</span>
+</span><span id="L-40"><a href="#L-40"><span class="linenos"> 40</span></a>        <span class="s2">&quot;--install&quot;</span><span class="p">,</span>
+</span><span id="L-41"><a href="#L-41"><span class="linenos"> 41</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="L-42"><a href="#L-42"><span class="linenos"> 42</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Install the package from source. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-43"><a href="#L-43"><span class="linenos"> 43</span></a>    <span class="p">)</span>
+</span><span id="L-44"><a href="#L-44"><span class="linenos"> 44</span></a>
+</span><span id="L-45"><a href="#L-45"><span class="linenos"> 45</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-46"><a href="#L-46"><span class="linenos"> 46</span></a>        <span class="s2">&quot;-iv&quot;</span><span class="p">,</span>
+</span><span id="L-47"><a href="#L-47"><span class="linenos"> 47</span></a>        <span class="s2">&quot;--increment_version&quot;</span><span class="p">,</span>
+</span><span id="L-48"><a href="#L-48"><span class="linenos"> 48</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
+</span><span id="L-49"><a href="#L-49"><span class="linenos"> 49</span></a>        <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
+</span><span id="L-50"><a href="#L-50"><span class="linenos"> 50</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Increment version in pyproject.toml.</span>
+</span><span id="L-51"><a href="#L-51"><span class="linenos"> 51</span></a><span class="s2">        Can be one of &quot;major&quot;, &quot;minor&quot;, or &quot;patch&quot;. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-52"><a href="#L-52"><span class="linenos"> 52</span></a>    <span class="p">)</span>
+</span><span id="L-53"><a href="#L-53"><span class="linenos"> 53</span></a>
+</span><span id="L-54"><a href="#L-54"><span class="linenos"> 54</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-55"><a href="#L-55"><span class="linenos"> 55</span></a>        <span class="s2">&quot;-p&quot;</span><span class="p">,</span>
+</span><span id="L-56"><a href="#L-56"><span class="linenos"> 56</span></a>        <span class="s2">&quot;--publish&quot;</span><span class="p">,</span>
+</span><span id="L-57"><a href="#L-57"><span class="linenos"> 57</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="L-58"><a href="#L-58"><span class="linenos"> 58</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Publish package to PyPi.</span>
+</span><span id="L-59"><a href="#L-59"><span class="linenos"> 59</span></a><span class="s2">        Note: You must have configured twine </span>
+</span><span id="L-60"><a href="#L-60"><span class="linenos"> 60</span></a><span class="s2">        and registered a PyPi account/generated an API</span>
+</span><span id="L-61"><a href="#L-61"><span class="linenos"> 61</span></a><span class="s2">        key to use this option.&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-62"><a href="#L-62"><span class="linenos"> 62</span></a>    <span class="p">)</span>
+</span><span id="L-63"><a href="#L-63"><span class="linenos"> 63</span></a>
+</span><span id="L-64"><a href="#L-64"><span class="linenos"> 64</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-65"><a href="#L-65"><span class="linenos"> 65</span></a>        <span class="s2">&quot;-rt&quot;</span><span class="p">,</span>
+</span><span id="L-66"><a href="#L-66"><span class="linenos"> 66</span></a>        <span class="s2">&quot;--run_tests&quot;</span><span class="p">,</span>
+</span><span id="L-67"><a href="#L-67"><span class="linenos"> 67</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="L-68"><a href="#L-68"><span class="linenos"> 68</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Run tests for the package. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-69"><a href="#L-69"><span class="linenos"> 69</span></a>    <span class="p">)</span>
+</span><span id="L-70"><a href="#L-70"><span class="linenos"> 70</span></a>
+</span><span id="L-71"><a href="#L-71"><span class="linenos"> 71</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-72"><a href="#L-72"><span class="linenos"> 72</span></a>        <span class="s2">&quot;-gt&quot;</span><span class="p">,</span>
+</span><span id="L-73"><a href="#L-73"><span class="linenos"> 73</span></a>        <span class="s2">&quot;--generate_tests&quot;</span><span class="p">,</span>
+</span><span id="L-74"><a href="#L-74"><span class="linenos"> 74</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="L-75"><a href="#L-75"><span class="linenos"> 75</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Generate tests for the package. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-76"><a href="#L-76"><span class="linenos"> 76</span></a>    <span class="p">)</span>
+</span><span id="L-77"><a href="#L-77"><span class="linenos"> 77</span></a>
+</span><span id="L-78"><a href="#L-78"><span class="linenos"> 78</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-79"><a href="#L-79"><span class="linenos"> 79</span></a>        <span class="s2">&quot;-uc&quot;</span><span class="p">,</span>
+</span><span id="L-80"><a href="#L-80"><span class="linenos"> 80</span></a>        <span class="s2">&quot;--update_changelog&quot;</span><span class="p">,</span>
+</span><span id="L-81"><a href="#L-81"><span class="linenos"> 81</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="L-82"><a href="#L-82"><span class="linenos"> 82</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Update changelog file. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-83"><a href="#L-83"><span class="linenos"> 83</span></a>    <span class="p">)</span>
+</span><span id="L-84"><a href="#L-84"><span class="linenos"> 84</span></a>
+</span><span id="L-85"><a href="#L-85"><span class="linenos"> 85</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-86"><a href="#L-86"><span class="linenos"> 86</span></a>        <span class="s2">&quot;-od&quot;</span><span class="p">,</span>
+</span><span id="L-87"><a href="#L-87"><span class="linenos"> 87</span></a>        <span class="s2">&quot;--overwrite_dependencies&quot;</span><span class="p">,</span>
+</span><span id="L-88"><a href="#L-88"><span class="linenos"> 88</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="L-89"><a href="#L-89"><span class="linenos"> 89</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; When building a package, packagelister will be used</span>
+</span><span id="L-90"><a href="#L-90"><span class="linenos"> 90</span></a><span class="s2">        to update the dependencies list in pyproject.toml.</span>
+</span><span id="L-91"><a href="#L-91"><span class="linenos"> 91</span></a><span class="s2">        The default behavior is to append any new dependencies to</span>
+</span><span id="L-92"><a href="#L-92"><span class="linenos"> 92</span></a><span class="s2">        the current list so as not to erase any manually added dependencies</span>
+</span><span id="L-93"><a href="#L-93"><span class="linenos"> 93</span></a><span class="s2">        that packagelister may not detect. If you don&#39;t have any manually </span>
+</span><span id="L-94"><a href="#L-94"><span class="linenos"> 94</span></a><span class="s2">        added dependencies and want to remove any dependencies that your</span>
+</span><span id="L-95"><a href="#L-95"><span class="linenos"> 95</span></a><span class="s2">        project no longer uses, pass this flag.&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-96"><a href="#L-96"><span class="linenos"> 96</span></a>    <span class="p">)</span>
+</span><span id="L-97"><a href="#L-97"><span class="linenos"> 97</span></a>
+</span><span id="L-98"><a href="#L-98"><span class="linenos"> 98</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-99"><a href="#L-99"><span class="linenos"> 99</span></a>        <span class="s2">&quot;-ca&quot;</span><span class="p">,</span>
+</span><span id="L-100"><a href="#L-100"><span class="linenos">100</span></a>        <span class="s2">&quot;--commit_all&quot;</span><span class="p">,</span>
+</span><span id="L-101"><a href="#L-101"><span class="linenos">101</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
+</span><span id="L-102"><a href="#L-102"><span class="linenos">102</span></a>        <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
+</span><span id="L-103"><a href="#L-103"><span class="linenos">103</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Git stage and commit all tracked files</span>
+</span><span id="L-104"><a href="#L-104"><span class="linenos">104</span></a><span class="s2">        with this supplied commit message.</span>
+</span><span id="L-105"><a href="#L-105"><span class="linenos">105</span></a><span class="s2">        If &#39;build&#39; is passed, all commits will have</span>
+</span><span id="L-106"><a href="#L-106"><span class="linenos">106</span></a><span class="s2">        message: &#39;chore: build v</span><span class="si">{current_version}</span><span class="s2">&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-107"><a href="#L-107"><span class="linenos">107</span></a>    <span class="p">)</span>
+</span><span id="L-108"><a href="#L-108"><span class="linenos">108</span></a>
+</span><span id="L-109"><a href="#L-109"><span class="linenos">109</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-110"><a href="#L-110"><span class="linenos">110</span></a>        <span class="s2">&quot;-s&quot;</span><span class="p">,</span>
+</span><span id="L-111"><a href="#L-111"><span class="linenos">111</span></a>        <span class="s2">&quot;--sync&quot;</span><span class="p">,</span>
+</span><span id="L-112"><a href="#L-112"><span class="linenos">112</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="L-113"><a href="#L-113"><span class="linenos">113</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Pull from github, then push current commit to repo. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-114"><a href="#L-114"><span class="linenos">114</span></a>    <span class="p">)</span>
+</span><span id="L-115"><a href="#L-115"><span class="linenos">115</span></a>
+</span><span id="L-116"><a href="#L-116"><span class="linenos">116</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-117"><a href="#L-117"><span class="linenos">117</span></a>        <span class="s2">&quot;-dv&quot;</span><span class="p">,</span>
+</span><span id="L-118"><a href="#L-118"><span class="linenos">118</span></a>        <span class="s2">&quot;--dependency_versions&quot;</span><span class="p">,</span>
+</span><span id="L-119"><a href="#L-119"><span class="linenos">119</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="L-120"><a href="#L-120"><span class="linenos">120</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Include version specifiers for dependencies in</span>
+</span><span id="L-121"><a href="#L-121"><span class="linenos">121</span></a><span class="s2">        pyproject.toml.&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-122"><a href="#L-122"><span class="linenos">122</span></a>    <span class="p">)</span>
+</span><span id="L-123"><a href="#L-123"><span class="linenos">123</span></a>
+</span><span id="L-124"><a href="#L-124"><span class="linenos">124</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-125"><a href="#L-125"><span class="linenos">125</span></a>        <span class="s2">&quot;-up&quot;</span><span class="p">,</span>
+</span><span id="L-126"><a href="#L-126"><span class="linenos">126</span></a>        <span class="s2">&quot;--update&quot;</span><span class="p">,</span>
+</span><span id="L-127"><a href="#L-127"><span class="linenos">127</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
+</span><span id="L-128"><a href="#L-128"><span class="linenos">128</span></a>        <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
+</span><span id="L-129"><a href="#L-129"><span class="linenos">129</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Excpects one argument: &quot;major&quot;, &quot;minor&quot;, or &quot;patch&quot;.</span>
+</span><span id="L-130"><a href="#L-130"><span class="linenos">130</span></a><span class="s2">        Passing &quot;-up minor&quot; is equivalent to passing the cli string: &quot;-b -t -i -iv minor -uc -ca build -s&quot;.</span>
+</span><span id="L-131"><a href="#L-131"><span class="linenos">131</span></a><span class="s2">        To publish the updated package, the -p/--publish switch needs to be added to the cli input.&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-132"><a href="#L-132"><span class="linenos">132</span></a>    <span class="p">)</span>
+</span><span id="L-133"><a href="#L-133"><span class="linenos">133</span></a>
+</span><span id="L-134"><a href="#L-134"><span class="linenos">134</span></a>    <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="o">.</span><span class="n">parse_args</span><span class="p">()</span>
 </span><span id="L-135"><a href="#L-135"><span class="linenos">135</span></a>
-</span><span id="L-136"><a href="#L-136"><span class="linenos">136</span></a>    <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="o">.</span><span class="n">parse_args</span><span class="p">()</span>
+</span><span id="L-136"><a href="#L-136"><span class="linenos">136</span></a>    <span class="n">args</span><span class="o">.</span><span class="n">package</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span><span class="o">.</span><span class="n">resolve</span><span class="p">()</span>
 </span><span id="L-137"><a href="#L-137"><span class="linenos">137</span></a>
-</span><span id="L-138"><a href="#L-138"><span class="linenos">138</span></a>    <span class="n">args</span><span class="o">.</span><span class="n">package</span> <span class="o">=</span> <span class="n">Path</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span><span class="o">.</span><span class="n">resolve</span><span class="p">()</span>
-</span><span id="L-139"><a href="#L-139"><span class="linenos">139</span></a>
-</span><span id="L-140"><a href="#L-140"><span class="linenos">140</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">update</span><span class="p">:</span>
-</span><span id="L-141"><a href="#L-141"><span class="linenos">141</span></a>        <span class="n">args</span><span class="o">.</span><span class="n">build</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="L-142"><a href="#L-142"><span class="linenos">142</span></a>        <span class="n">args</span><span class="o">.</span><span class="n">tag_version</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="L-143"><a href="#L-143"><span class="linenos">143</span></a>        <span class="n">args</span><span class="o">.</span><span class="n">install</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="L-144"><a href="#L-144"><span class="linenos">144</span></a>        <span class="n">args</span><span class="o">.</span><span class="n">increment_version</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">update</span>
-</span><span id="L-145"><a href="#L-145"><span class="linenos">145</span></a>        <span class="n">args</span><span class="o">.</span><span class="n">update_changelog</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="L-146"><a href="#L-146"><span class="linenos">146</span></a>        <span class="n">args</span><span class="o">.</span><span class="n">commit_all</span> <span class="o">=</span> <span class="s2">&quot;build&quot;</span>
-</span><span id="L-147"><a href="#L-147"><span class="linenos">147</span></a>        <span class="n">args</span><span class="o">.</span><span class="n">sync</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="L-148"><a href="#L-148"><span class="linenos">148</span></a>
-</span><span id="L-149"><a href="#L-149"><span class="linenos">149</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">increment_version</span> <span class="ow">and</span> <span class="n">args</span><span class="o">.</span><span class="n">increment_version</span> <span class="ow">not</span> <span class="ow">in</span> <span class="p">[</span>
-</span><span id="L-150"><a href="#L-150"><span class="linenos">150</span></a>        <span class="s2">&quot;major&quot;</span><span class="p">,</span>
-</span><span id="L-151"><a href="#L-151"><span class="linenos">151</span></a>        <span class="s2">&quot;minor&quot;</span><span class="p">,</span>
-</span><span id="L-152"><a href="#L-152"><span class="linenos">152</span></a>        <span class="s2">&quot;patch&quot;</span><span class="p">,</span>
-</span><span id="L-153"><a href="#L-153"><span class="linenos">153</span></a>    <span class="p">]:</span>
-</span><span id="L-154"><a href="#L-154"><span class="linenos">154</span></a>        <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span>
-</span><span id="L-155"><a href="#L-155"><span class="linenos">155</span></a>            <span class="sa">f</span><span class="s2">&quot;Invalid option for -iv/--increment_version: </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">increment_version</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="L-156"><a href="#L-156"><span class="linenos">156</span></a>        <span class="p">)</span>
-</span><span id="L-157"><a href="#L-157"><span class="linenos">157</span></a>
-</span><span id="L-158"><a href="#L-158"><span class="linenos">158</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">commit_all</span> <span class="o">==</span> <span class="s2">&quot;&quot;</span><span class="p">:</span>
-</span><span id="L-159"><a href="#L-159"><span class="linenos">159</span></a>        <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="s2">&quot;Commit message for args.commit_all cannot be empty.&quot;</span><span class="p">)</span>
+</span><span id="L-138"><a href="#L-138"><span class="linenos">138</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">update</span><span class="p">:</span>
+</span><span id="L-139"><a href="#L-139"><span class="linenos">139</span></a>        <span class="n">args</span><span class="o">.</span><span class="n">build</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="L-140"><a href="#L-140"><span class="linenos">140</span></a>        <span class="n">args</span><span class="o">.</span><span class="n">tag_version</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="L-141"><a href="#L-141"><span class="linenos">141</span></a>        <span class="n">args</span><span class="o">.</span><span class="n">install</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="L-142"><a href="#L-142"><span class="linenos">142</span></a>        <span class="n">args</span><span class="o">.</span><span class="n">increment_version</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">update</span>
+</span><span id="L-143"><a href="#L-143"><span class="linenos">143</span></a>        <span class="n">args</span><span class="o">.</span><span class="n">update_changelog</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="L-144"><a href="#L-144"><span class="linenos">144</span></a>        <span class="n">args</span><span class="o">.</span><span class="n">commit_all</span> <span class="o">=</span> <span class="s2">&quot;build&quot;</span>
+</span><span id="L-145"><a href="#L-145"><span class="linenos">145</span></a>        <span class="n">args</span><span class="o">.</span><span class="n">sync</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="L-146"><a href="#L-146"><span class="linenos">146</span></a>
+</span><span id="L-147"><a href="#L-147"><span class="linenos">147</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">increment_version</span> <span class="ow">and</span> <span class="n">args</span><span class="o">.</span><span class="n">increment_version</span> <span class="ow">not</span> <span class="ow">in</span> <span class="p">[</span>
+</span><span id="L-148"><a href="#L-148"><span class="linenos">148</span></a>        <span class="s2">&quot;major&quot;</span><span class="p">,</span>
+</span><span id="L-149"><a href="#L-149"><span class="linenos">149</span></a>        <span class="s2">&quot;minor&quot;</span><span class="p">,</span>
+</span><span id="L-150"><a href="#L-150"><span class="linenos">150</span></a>        <span class="s2">&quot;patch&quot;</span><span class="p">,</span>
+</span><span id="L-151"><a href="#L-151"><span class="linenos">151</span></a>    <span class="p">]:</span>
+</span><span id="L-152"><a href="#L-152"><span class="linenos">152</span></a>        <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span>
+</span><span id="L-153"><a href="#L-153"><span class="linenos">153</span></a>            <span class="sa">f</span><span class="s2">&quot;Invalid option for -iv/--increment_version: </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">increment_version</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="L-154"><a href="#L-154"><span class="linenos">154</span></a>        <span class="p">)</span>
+</span><span id="L-155"><a href="#L-155"><span class="linenos">155</span></a>
+</span><span id="L-156"><a href="#L-156"><span class="linenos">156</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">commit_all</span> <span class="o">==</span> <span class="s2">&quot;&quot;</span><span class="p">:</span>
+</span><span id="L-157"><a href="#L-157"><span class="linenos">157</span></a>        <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="s2">&quot;Commit message for args.commit_all cannot be empty.&quot;</span><span class="p">)</span>
+</span><span id="L-158"><a href="#L-158"><span class="linenos">158</span></a>
+</span><span id="L-159"><a href="#L-159"><span class="linenos">159</span></a>    <span class="k">return</span> <span class="n">args</span>
 </span><span id="L-160"><a href="#L-160"><span class="linenos">160</span></a>
-</span><span id="L-161"><a href="#L-161"><span class="linenos">161</span></a>    <span class="k">return</span> <span class="n">args</span>
-</span><span id="L-162"><a href="#L-162"><span class="linenos">162</span></a>
-</span><span id="L-163"><a href="#L-163"><span class="linenos">163</span></a>
-</span><span id="L-164"><a href="#L-164"><span class="linenos">164</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
-</span><span id="L-165"><a href="#L-165"><span class="linenos">165</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="p">:</span>
-</span><span id="L-166"><a href="#L-166"><span class="linenos">166</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
+</span><span id="L-161"><a href="#L-161"><span class="linenos">161</span></a>
+</span><span id="L-162"><a href="#L-162"><span class="linenos">162</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
+</span><span id="L-163"><a href="#L-163"><span class="linenos">163</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="p">:</span>
+</span><span id="L-164"><a href="#L-164"><span class="linenos">164</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
+</span><span id="L-165"><a href="#L-165"><span class="linenos">165</span></a>
+</span><span id="L-166"><a href="#L-166"><span class="linenos">166</span></a>    <span class="n">pyproject_path</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">package</span> <span class="o">/</span> <span class="s2">&quot;pyproject.toml&quot;</span>
 </span><span id="L-167"><a href="#L-167"><span class="linenos">167</span></a>
-</span><span id="L-168"><a href="#L-168"><span class="linenos">168</span></a>    <span class="n">pyproject_path</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">package</span> <span class="o">/</span> <span class="s2">&quot;pyproject.toml&quot;</span>
-</span><span id="L-169"><a href="#L-169"><span class="linenos">169</span></a>
-</span><span id="L-170"><a href="#L-170"><span class="linenos">170</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">pyproject_path</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
-</span><span id="L-171"><a href="#L-171"><span class="linenos">171</span></a>        <span class="k">raise</span> <span class="ne">FileNotFoundError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Could not locate pyproject.toml for </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-172"><a href="#L-172"><span class="linenos">172</span></a>
-</span><span id="L-173"><a href="#L-173"><span class="linenos">173</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">generate_tests</span><span class="p">:</span>
-</span><span id="L-174"><a href="#L-174"><span class="linenos">174</span></a>        <span class="n">generate_test_files</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span>
-</span><span id="L-175"><a href="#L-175"><span class="linenos">175</span></a>
-</span><span id="L-176"><a href="#L-176"><span class="linenos">176</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">run_tests</span><span class="p">:</span>
-</span><span id="L-177"><a href="#L-177"><span class="linenos">177</span></a>        <span class="n">run_tests</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span>
-</span><span id="L-178"><a href="#L-178"><span class="linenos">178</span></a>
-</span><span id="L-179"><a href="#L-179"><span class="linenos">179</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">increment_version</span><span class="p">:</span>
-</span><span id="L-180"><a href="#L-180"><span class="linenos">180</span></a>        <span class="n">hassle_utilities</span><span class="o">.</span><span class="n">increment_version</span><span class="p">(</span><span class="n">pyproject_path</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">increment_version</span><span class="p">)</span>
-</span><span id="L-181"><a href="#L-181"><span class="linenos">181</span></a>
-</span><span id="L-182"><a href="#L-182"><span class="linenos">182</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">build</span><span class="p">:</span>
-</span><span id="L-183"><a href="#L-183"><span class="linenos">183</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="L-184"><a href="#L-184"><span class="linenos">184</span></a>            <span class="n">shutil</span><span class="o">.</span><span class="n">rmtree</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="si">}</span><span class="s2">/dist&quot;</span><span class="p">)</span>
-</span><span id="L-185"><a href="#L-185"><span class="linenos">185</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="L-186"><a href="#L-186"><span class="linenos">186</span></a>            <span class="k">pass</span>
-</span><span id="L-187"><a href="#L-187"><span class="linenos">187</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;black </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-188"><a href="#L-188"><span class="linenos">188</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;isort </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-189"><a href="#L-189"><span class="linenos">189</span></a>        <span class="n">hassle_utilities</span><span class="o">.</span><span class="n">update_dependencies</span><span class="p">(</span>
-</span><span id="L-190"><a href="#L-190"><span class="linenos">190</span></a>            <span class="n">pyproject_path</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">overwrite_dependencies</span>
-</span><span id="L-191"><a href="#L-191"><span class="linenos">191</span></a>        <span class="p">)</span>
-</span><span id="L-192"><a href="#L-192"><span class="linenos">192</span></a>        <span class="n">hassle_utilities</span><span class="o">.</span><span class="n">update_minimum_python_version</span><span class="p">(</span><span class="n">pyproject_path</span><span class="p">)</span>
-</span><span id="L-193"><a href="#L-193"><span class="linenos">193</span></a>        <span class="n">hassle_utilities</span><span class="o">.</span><span class="n">generate_docs</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span>
-</span><span id="L-194"><a href="#L-194"><span class="linenos">194</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;py -m build </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-195"><a href="#L-195"><span class="linenos">195</span></a>
-</span><span id="L-196"><a href="#L-196"><span class="linenos">196</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">update_changelog</span><span class="p">:</span>
-</span><span id="L-197"><a href="#L-197"><span class="linenos">197</span></a>        <span class="n">hassle_utilities</span><span class="o">.</span><span class="n">update_changelog</span><span class="p">(</span><span class="n">pyproject_path</span><span class="p">)</span>
-</span><span id="L-198"><a href="#L-198"><span class="linenos">198</span></a>        <span class="c1"># If we&#39;re going to add tag for current version</span>
-</span><span id="L-199"><a href="#L-199"><span class="linenos">199</span></a>        <span class="c1"># commit changelog first</span>
-</span><span id="L-200"><a href="#L-200"><span class="linenos">200</span></a>        <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">tag_version</span><span class="p">:</span>
-</span><span id="L-201"><a href="#L-201"><span class="linenos">201</span></a>            <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span>
-</span><span id="L-202"><a href="#L-202"><span class="linenos">202</span></a>            <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="s2">&quot;git add CHANGELOG.md&quot;</span><span class="p">)</span>
-</span><span id="L-203"><a href="#L-203"><span class="linenos">203</span></a>            <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="s1">&#39;git commit CHANGELOG.md -m &quot;chore: update changelog&quot;&#39;</span><span class="p">)</span>
-</span><span id="L-204"><a href="#L-204"><span class="linenos">204</span></a>
-</span><span id="L-205"><a href="#L-205"><span class="linenos">205</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">commit_all</span><span class="p">:</span>
-</span><span id="L-206"><a href="#L-206"><span class="linenos">206</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span>
-</span><span id="L-207"><a href="#L-207"><span class="linenos">207</span></a>        <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">commit_all</span> <span class="o">==</span> <span class="s2">&quot;build&quot;</span><span class="p">:</span>
-</span><span id="L-208"><a href="#L-208"><span class="linenos">208</span></a>            <span class="n">version</span> <span class="o">=</span> <span class="n">tomlkit</span><span class="o">.</span><span class="n">loads</span><span class="p">(</span><span class="n">pyproject_path</span><span class="o">.</span><span class="n">read_text</span><span class="p">())[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;version&quot;</span><span class="p">]</span>
-</span><span id="L-209"><a href="#L-209"><span class="linenos">209</span></a>            <span class="n">args</span><span class="o">.</span><span class="n">commit_all</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;chore: build v</span><span class="si">{</span><span class="n">version</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="L-210"><a href="#L-210"><span class="linenos">210</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="s2">&quot;git add .&quot;</span><span class="p">)</span>
-</span><span id="L-211"><a href="#L-211"><span class="linenos">211</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;git commit -m &quot;</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">commit_all</span><span class="si">}</span><span class="s1">&quot;&#39;</span><span class="p">)</span>
-</span><span id="L-212"><a href="#L-212"><span class="linenos">212</span></a>
-</span><span id="L-213"><a href="#L-213"><span class="linenos">213</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">tag_version</span><span class="p">:</span>
-</span><span id="L-214"><a href="#L-214"><span class="linenos">214</span></a>        <span class="n">hassle_utilities</span><span class="o">.</span><span class="n">tag_version</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span>
-</span><span id="L-215"><a href="#L-215"><span class="linenos">215</span></a>
-</span><span id="L-216"><a href="#L-216"><span class="linenos">216</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">publish</span><span class="p">:</span>
-</span><span id="L-217"><a href="#L-217"><span class="linenos">217</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;twine upload </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">package</span> <span class="o">/</span> <span class="s1">&#39;dist&#39;</span> <span class="o">/</span> <span class="s1">&#39;*&#39;</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-218"><a href="#L-218"><span class="linenos">218</span></a>
-</span><span id="L-219"><a href="#L-219"><span class="linenos">219</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">install</span><span class="p">:</span>
-</span><span id="L-220"><a href="#L-220"><span class="linenos">220</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;pip install </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="si">}</span><span class="s2"> --no-deps --upgrade --no-cache-dir&quot;</span><span class="p">)</span>
+</span><span id="L-168"><a href="#L-168"><span class="linenos">168</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">pyproject_path</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
+</span><span id="L-169"><a href="#L-169"><span class="linenos">169</span></a>        <span class="k">raise</span> <span class="ne">FileNotFoundError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Could not locate pyproject.toml for </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-170"><a href="#L-170"><span class="linenos">170</span></a>
+</span><span id="L-171"><a href="#L-171"><span class="linenos">171</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">generate_tests</span><span class="p">:</span>
+</span><span id="L-172"><a href="#L-172"><span class="linenos">172</span></a>        <span class="n">generate_test_files</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span>
+</span><span id="L-173"><a href="#L-173"><span class="linenos">173</span></a>
+</span><span id="L-174"><a href="#L-174"><span class="linenos">174</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">run_tests</span><span class="p">:</span>
+</span><span id="L-175"><a href="#L-175"><span class="linenos">175</span></a>        <span class="n">run_tests</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span>
+</span><span id="L-176"><a href="#L-176"><span class="linenos">176</span></a>
+</span><span id="L-177"><a href="#L-177"><span class="linenos">177</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">increment_version</span><span class="p">:</span>
+</span><span id="L-178"><a href="#L-178"><span class="linenos">178</span></a>        <span class="n">hassle_utilities</span><span class="o">.</span><span class="n">increment_version</span><span class="p">(</span><span class="n">pyproject_path</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">increment_version</span><span class="p">)</span>
+</span><span id="L-179"><a href="#L-179"><span class="linenos">179</span></a>
+</span><span id="L-180"><a href="#L-180"><span class="linenos">180</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">build</span><span class="p">:</span>
+</span><span id="L-181"><a href="#L-181"><span class="linenos">181</span></a>        <span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span> <span class="o">/</span> <span class="s2">&quot;dist&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">delete</span><span class="p">()</span>
+</span><span id="L-182"><a href="#L-182"><span class="linenos">182</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;black </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-183"><a href="#L-183"><span class="linenos">183</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;isort </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-184"><a href="#L-184"><span class="linenos">184</span></a>        <span class="n">hassle_utilities</span><span class="o">.</span><span class="n">update_dependencies</span><span class="p">(</span>
+</span><span id="L-185"><a href="#L-185"><span class="linenos">185</span></a>            <span class="n">pyproject_path</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">overwrite_dependencies</span>
+</span><span id="L-186"><a href="#L-186"><span class="linenos">186</span></a>        <span class="p">)</span>
+</span><span id="L-187"><a href="#L-187"><span class="linenos">187</span></a>        <span class="n">hassle_utilities</span><span class="o">.</span><span class="n">update_minimum_python_version</span><span class="p">(</span><span class="n">pyproject_path</span><span class="p">)</span>
+</span><span id="L-188"><a href="#L-188"><span class="linenos">188</span></a>        <span class="n">hassle_utilities</span><span class="o">.</span><span class="n">generate_docs</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span>
+</span><span id="L-189"><a href="#L-189"><span class="linenos">189</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;py -m build </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-190"><a href="#L-190"><span class="linenos">190</span></a>
+</span><span id="L-191"><a href="#L-191"><span class="linenos">191</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">update_changelog</span><span class="p">:</span>
+</span><span id="L-192"><a href="#L-192"><span class="linenos">192</span></a>        <span class="n">hassle_utilities</span><span class="o">.</span><span class="n">update_changelog</span><span class="p">(</span><span class="n">pyproject_path</span><span class="p">)</span>
+</span><span id="L-193"><a href="#L-193"><span class="linenos">193</span></a>        <span class="c1"># If we&#39;re going to add tag for current version</span>
+</span><span id="L-194"><a href="#L-194"><span class="linenos">194</span></a>        <span class="c1"># commit changelog first</span>
+</span><span id="L-195"><a href="#L-195"><span class="linenos">195</span></a>        <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">tag_version</span><span class="p">:</span>
+</span><span id="L-196"><a href="#L-196"><span class="linenos">196</span></a>            <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span>
+</span><span id="L-197"><a href="#L-197"><span class="linenos">197</span></a>            <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="s2">&quot;git add CHANGELOG.md&quot;</span><span class="p">)</span>
+</span><span id="L-198"><a href="#L-198"><span class="linenos">198</span></a>            <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="s1">&#39;git commit CHANGELOG.md -m &quot;chore: update changelog&quot;&#39;</span><span class="p">)</span>
+</span><span id="L-199"><a href="#L-199"><span class="linenos">199</span></a>
+</span><span id="L-200"><a href="#L-200"><span class="linenos">200</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">commit_all</span><span class="p">:</span>
+</span><span id="L-201"><a href="#L-201"><span class="linenos">201</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span>
+</span><span id="L-202"><a href="#L-202"><span class="linenos">202</span></a>        <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">commit_all</span> <span class="o">==</span> <span class="s2">&quot;build&quot;</span><span class="p">:</span>
+</span><span id="L-203"><a href="#L-203"><span class="linenos">203</span></a>            <span class="n">version</span> <span class="o">=</span> <span class="n">pyproject_path</span><span class="o">.</span><span class="n">loads</span><span class="p">()[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;version&quot;</span><span class="p">]</span>
+</span><span id="L-204"><a href="#L-204"><span class="linenos">204</span></a>            <span class="n">args</span><span class="o">.</span><span class="n">commit_all</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;chore: build v</span><span class="si">{</span><span class="n">version</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="L-205"><a href="#L-205"><span class="linenos">205</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="s2">&quot;git add .&quot;</span><span class="p">)</span>
+</span><span id="L-206"><a href="#L-206"><span class="linenos">206</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;git commit -m &quot;</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">commit_all</span><span class="si">}</span><span class="s1">&quot;&#39;</span><span class="p">)</span>
+</span><span id="L-207"><a href="#L-207"><span class="linenos">207</span></a>
+</span><span id="L-208"><a href="#L-208"><span class="linenos">208</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">tag_version</span><span class="p">:</span>
+</span><span id="L-209"><a href="#L-209"><span class="linenos">209</span></a>        <span class="n">hassle_utilities</span><span class="o">.</span><span class="n">tag_version</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span>
+</span><span id="L-210"><a href="#L-210"><span class="linenos">210</span></a>
+</span><span id="L-211"><a href="#L-211"><span class="linenos">211</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">publish</span><span class="p">:</span>
+</span><span id="L-212"><a href="#L-212"><span class="linenos">212</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;twine upload </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">package</span> <span class="o">/</span> <span class="s1">&#39;dist&#39;</span> <span class="o">/</span> <span class="s1">&#39;*&#39;</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-213"><a href="#L-213"><span class="linenos">213</span></a>
+</span><span id="L-214"><a href="#L-214"><span class="linenos">214</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">install</span><span class="p">:</span>
+</span><span id="L-215"><a href="#L-215"><span class="linenos">215</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;pip install </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="si">}</span><span class="s2"> --no-deps --upgrade --no-cache-dir&quot;</span><span class="p">)</span>
+</span><span id="L-216"><a href="#L-216"><span class="linenos">216</span></a>
+</span><span id="L-217"><a href="#L-217"><span class="linenos">217</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">sync</span><span class="p">:</span>
+</span><span id="L-218"><a href="#L-218"><span class="linenos">218</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span>
+</span><span id="L-219"><a href="#L-219"><span class="linenos">219</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;git pull --tags origin main&quot;</span><span class="p">)</span>
+</span><span id="L-220"><a href="#L-220"><span class="linenos">220</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;git push origin main:main --tags&quot;</span><span class="p">)</span>
 </span><span id="L-221"><a href="#L-221"><span class="linenos">221</span></a>
-</span><span id="L-222"><a href="#L-222"><span class="linenos">222</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">sync</span><span class="p">:</span>
-</span><span id="L-223"><a href="#L-223"><span class="linenos">223</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span>
-</span><span id="L-224"><a href="#L-224"><span class="linenos">224</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;git pull --tags origin main&quot;</span><span class="p">)</span>
-</span><span id="L-225"><a href="#L-225"><span class="linenos">225</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;git push origin main:main --tags&quot;</span><span class="p">)</span>
-</span><span id="L-226"><a href="#L-226"><span class="linenos">226</span></a>
-</span><span id="L-227"><a href="#L-227"><span class="linenos">227</span></a>
-</span><span id="L-228"><a href="#L-228"><span class="linenos">228</span></a><span class="k">if</span> <span class="vm">__name__</span> <span class="o">==</span> <span class="s2">&quot;__main__&quot;</span><span class="p">:</span>
-</span><span id="L-229"><a href="#L-229"><span class="linenos">229</span></a>    <span class="n">main</span><span class="p">(</span><span class="n">get_args</span><span class="p">())</span>
+</span><span id="L-222"><a href="#L-222"><span class="linenos">222</span></a>
+</span><span id="L-223"><a href="#L-223"><span class="linenos">223</span></a><span class="k">if</span> <span class="vm">__name__</span> <span class="o">==</span> <span class="s2">&quot;__main__&quot;</span><span class="p">:</span>
+</span><span id="L-224"><a href="#L-224"><span class="linenos">224</span></a>    <span class="n">main</span><span class="p">(</span><span class="n">get_args</span><span class="p">())</span>
 </span></pre></div>
 
 
             </section>
                 <section id="get_args">
                             <input id="get_args-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
@@ -297,161 +292,161 @@
         <span class="def">def</span>
         <span class="name">get_args</span><span class="signature pdoc-code condensed">(<span class="return-annotation">) -> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span>:</span></span>
 
                 <label class="view-source-button" for="get_args-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#get_args"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="get_args-16"><a href="#get_args-16"><span class="linenos"> 16</span></a><span class="k">def</span> <span class="nf">get_args</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">:</span>
-</span><span id="get_args-17"><a href="#get_args-17"><span class="linenos"> 17</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">argparse</span><span class="o">.</span><span class="n">ArgumentParser</span><span class="p">()</span>
-</span><span id="get_args-18"><a href="#get_args-18"><span class="linenos"> 18</span></a>
-</span><span id="get_args-19"><a href="#get_args-19"><span class="linenos"> 19</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="get_args-20"><a href="#get_args-20"><span class="linenos"> 20</span></a>        <span class="s2">&quot;package&quot;</span><span class="p">,</span>
-</span><span id="get_args-21"><a href="#get_args-21"><span class="linenos"> 21</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
-</span><span id="get_args-22"><a href="#get_args-22"><span class="linenos"> 22</span></a>        <span class="n">default</span><span class="o">=</span><span class="s2">&quot;.&quot;</span><span class="p">,</span>
-</span><span id="get_args-23"><a href="#get_args-23"><span class="linenos"> 23</span></a>        <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;?&quot;</span><span class="p">,</span>
-</span><span id="get_args-24"><a href="#get_args-24"><span class="linenos"> 24</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; The name of the package or project to use,</span>
-</span><span id="get_args-25"><a href="#get_args-25"><span class="linenos"> 25</span></a><span class="s2">        assuming it&#39;s a subfolder of your current working directory.</span>
-</span><span id="get_args-26"><a href="#get_args-26"><span class="linenos"> 26</span></a><span class="s2">        Can also be a full path to the package. If nothing is given,</span>
-</span><span id="get_args-27"><a href="#get_args-27"><span class="linenos"> 27</span></a><span class="s2">        the current working directory will be used.&quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="get_args-28"><a href="#get_args-28"><span class="linenos"> 28</span></a>    <span class="p">)</span>
-</span><span id="get_args-29"><a href="#get_args-29"><span class="linenos"> 29</span></a>
-</span><span id="get_args-30"><a href="#get_args-30"><span class="linenos"> 30</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="get_args-31"><a href="#get_args-31"><span class="linenos"> 31</span></a>        <span class="s2">&quot;-b&quot;</span><span class="p">,</span> <span class="s2">&quot;--build&quot;</span><span class="p">,</span> <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span> <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Build the package. &quot;&quot;&quot;</span>
-</span><span id="get_args-32"><a href="#get_args-32"><span class="linenos"> 32</span></a>    <span class="p">)</span>
-</span><span id="get_args-33"><a href="#get_args-33"><span class="linenos"> 33</span></a>
-</span><span id="get_args-34"><a href="#get_args-34"><span class="linenos"> 34</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="get_args-35"><a href="#get_args-35"><span class="linenos"> 35</span></a>        <span class="s2">&quot;-t&quot;</span><span class="p">,</span>
-</span><span id="get_args-36"><a href="#get_args-36"><span class="linenos"> 36</span></a>        <span class="s2">&quot;--tag_version&quot;</span><span class="p">,</span>
-</span><span id="get_args-37"><a href="#get_args-37"><span class="linenos"> 37</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
-</span><span id="get_args-38"><a href="#get_args-38"><span class="linenos"> 38</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Add a git tag corresponding to the version in pyproject.toml. &quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="get_args-39"><a href="#get_args-39"><span class="linenos"> 39</span></a>    <span class="p">)</span>
-</span><span id="get_args-40"><a href="#get_args-40"><span class="linenos"> 40</span></a>
-</span><span id="get_args-41"><a href="#get_args-41"><span class="linenos"> 41</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="get_args-42"><a href="#get_args-42"><span class="linenos"> 42</span></a>        <span class="s2">&quot;-i&quot;</span><span class="p">,</span>
-</span><span id="get_args-43"><a href="#get_args-43"><span class="linenos"> 43</span></a>        <span class="s2">&quot;--install&quot;</span><span class="p">,</span>
-</span><span id="get_args-44"><a href="#get_args-44"><span class="linenos"> 44</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
-</span><span id="get_args-45"><a href="#get_args-45"><span class="linenos"> 45</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Install the package from source. &quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="get_args-46"><a href="#get_args-46"><span class="linenos"> 46</span></a>    <span class="p">)</span>
-</span><span id="get_args-47"><a href="#get_args-47"><span class="linenos"> 47</span></a>
-</span><span id="get_args-48"><a href="#get_args-48"><span class="linenos"> 48</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="get_args-49"><a href="#get_args-49"><span class="linenos"> 49</span></a>        <span class="s2">&quot;-iv&quot;</span><span class="p">,</span>
-</span><span id="get_args-50"><a href="#get_args-50"><span class="linenos"> 50</span></a>        <span class="s2">&quot;--increment_version&quot;</span><span class="p">,</span>
-</span><span id="get_args-51"><a href="#get_args-51"><span class="linenos"> 51</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
-</span><span id="get_args-52"><a href="#get_args-52"><span class="linenos"> 52</span></a>        <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
-</span><span id="get_args-53"><a href="#get_args-53"><span class="linenos"> 53</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Increment version in pyproject.toml.</span>
-</span><span id="get_args-54"><a href="#get_args-54"><span class="linenos"> 54</span></a><span class="s2">        Can be one of &quot;major&quot;, &quot;minor&quot;, or &quot;patch&quot;. &quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="get_args-55"><a href="#get_args-55"><span class="linenos"> 55</span></a>    <span class="p">)</span>
-</span><span id="get_args-56"><a href="#get_args-56"><span class="linenos"> 56</span></a>
-</span><span id="get_args-57"><a href="#get_args-57"><span class="linenos"> 57</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="get_args-58"><a href="#get_args-58"><span class="linenos"> 58</span></a>        <span class="s2">&quot;-p&quot;</span><span class="p">,</span>
-</span><span id="get_args-59"><a href="#get_args-59"><span class="linenos"> 59</span></a>        <span class="s2">&quot;--publish&quot;</span><span class="p">,</span>
-</span><span id="get_args-60"><a href="#get_args-60"><span class="linenos"> 60</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
-</span><span id="get_args-61"><a href="#get_args-61"><span class="linenos"> 61</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Publish package to PyPi.</span>
-</span><span id="get_args-62"><a href="#get_args-62"><span class="linenos"> 62</span></a><span class="s2">        Note: You must have configured twine </span>
-</span><span id="get_args-63"><a href="#get_args-63"><span class="linenos"> 63</span></a><span class="s2">        and registered a PyPi account/generated an API</span>
-</span><span id="get_args-64"><a href="#get_args-64"><span class="linenos"> 64</span></a><span class="s2">        key to use this option.&quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="get_args-65"><a href="#get_args-65"><span class="linenos"> 65</span></a>    <span class="p">)</span>
-</span><span id="get_args-66"><a href="#get_args-66"><span class="linenos"> 66</span></a>
-</span><span id="get_args-67"><a href="#get_args-67"><span class="linenos"> 67</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="get_args-68"><a href="#get_args-68"><span class="linenos"> 68</span></a>        <span class="s2">&quot;-rt&quot;</span><span class="p">,</span>
-</span><span id="get_args-69"><a href="#get_args-69"><span class="linenos"> 69</span></a>        <span class="s2">&quot;--run_tests&quot;</span><span class="p">,</span>
-</span><span id="get_args-70"><a href="#get_args-70"><span class="linenos"> 70</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
-</span><span id="get_args-71"><a href="#get_args-71"><span class="linenos"> 71</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Run tests for the package. &quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="get_args-72"><a href="#get_args-72"><span class="linenos"> 72</span></a>    <span class="p">)</span>
-</span><span id="get_args-73"><a href="#get_args-73"><span class="linenos"> 73</span></a>
-</span><span id="get_args-74"><a href="#get_args-74"><span class="linenos"> 74</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="get_args-75"><a href="#get_args-75"><span class="linenos"> 75</span></a>        <span class="s2">&quot;-gt&quot;</span><span class="p">,</span>
-</span><span id="get_args-76"><a href="#get_args-76"><span class="linenos"> 76</span></a>        <span class="s2">&quot;--generate_tests&quot;</span><span class="p">,</span>
-</span><span id="get_args-77"><a href="#get_args-77"><span class="linenos"> 77</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
-</span><span id="get_args-78"><a href="#get_args-78"><span class="linenos"> 78</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Generate tests for the package. &quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="get_args-79"><a href="#get_args-79"><span class="linenos"> 79</span></a>    <span class="p">)</span>
-</span><span id="get_args-80"><a href="#get_args-80"><span class="linenos"> 80</span></a>
-</span><span id="get_args-81"><a href="#get_args-81"><span class="linenos"> 81</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="get_args-82"><a href="#get_args-82"><span class="linenos"> 82</span></a>        <span class="s2">&quot;-uc&quot;</span><span class="p">,</span>
-</span><span id="get_args-83"><a href="#get_args-83"><span class="linenos"> 83</span></a>        <span class="s2">&quot;--update_changelog&quot;</span><span class="p">,</span>
-</span><span id="get_args-84"><a href="#get_args-84"><span class="linenos"> 84</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
-</span><span id="get_args-85"><a href="#get_args-85"><span class="linenos"> 85</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Update changelog file. &quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="get_args-86"><a href="#get_args-86"><span class="linenos"> 86</span></a>    <span class="p">)</span>
-</span><span id="get_args-87"><a href="#get_args-87"><span class="linenos"> 87</span></a>
-</span><span id="get_args-88"><a href="#get_args-88"><span class="linenos"> 88</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="get_args-89"><a href="#get_args-89"><span class="linenos"> 89</span></a>        <span class="s2">&quot;-od&quot;</span><span class="p">,</span>
-</span><span id="get_args-90"><a href="#get_args-90"><span class="linenos"> 90</span></a>        <span class="s2">&quot;--overwrite_dependencies&quot;</span><span class="p">,</span>
-</span><span id="get_args-91"><a href="#get_args-91"><span class="linenos"> 91</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
-</span><span id="get_args-92"><a href="#get_args-92"><span class="linenos"> 92</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; When building a package, packagelister will be used</span>
-</span><span id="get_args-93"><a href="#get_args-93"><span class="linenos"> 93</span></a><span class="s2">        to update the dependencies list in pyproject.toml.</span>
-</span><span id="get_args-94"><a href="#get_args-94"><span class="linenos"> 94</span></a><span class="s2">        The default behavior is to append any new dependencies to</span>
-</span><span id="get_args-95"><a href="#get_args-95"><span class="linenos"> 95</span></a><span class="s2">        the current list so as not to erase any manually added dependencies</span>
-</span><span id="get_args-96"><a href="#get_args-96"><span class="linenos"> 96</span></a><span class="s2">        that packagelister may not detect. If you don&#39;t have any manually </span>
-</span><span id="get_args-97"><a href="#get_args-97"><span class="linenos"> 97</span></a><span class="s2">        added dependencies and want to remove any dependencies that your</span>
-</span><span id="get_args-98"><a href="#get_args-98"><span class="linenos"> 98</span></a><span class="s2">        project no longer uses, pass this flag.&quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="get_args-99"><a href="#get_args-99"><span class="linenos"> 99</span></a>    <span class="p">)</span>
-</span><span id="get_args-100"><a href="#get_args-100"><span class="linenos">100</span></a>
-</span><span id="get_args-101"><a href="#get_args-101"><span class="linenos">101</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="get_args-102"><a href="#get_args-102"><span class="linenos">102</span></a>        <span class="s2">&quot;-ca&quot;</span><span class="p">,</span>
-</span><span id="get_args-103"><a href="#get_args-103"><span class="linenos">103</span></a>        <span class="s2">&quot;--commit_all&quot;</span><span class="p">,</span>
-</span><span id="get_args-104"><a href="#get_args-104"><span class="linenos">104</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
-</span><span id="get_args-105"><a href="#get_args-105"><span class="linenos">105</span></a>        <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
-</span><span id="get_args-106"><a href="#get_args-106"><span class="linenos">106</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Git stage and commit all tracked files</span>
-</span><span id="get_args-107"><a href="#get_args-107"><span class="linenos">107</span></a><span class="s2">        with this supplied commit message.</span>
-</span><span id="get_args-108"><a href="#get_args-108"><span class="linenos">108</span></a><span class="s2">        If &#39;build&#39; is passed, all commits will have</span>
-</span><span id="get_args-109"><a href="#get_args-109"><span class="linenos">109</span></a><span class="s2">        message: &#39;chore: build v</span><span class="si">{current_version}</span><span class="s2">&quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="get_args-110"><a href="#get_args-110"><span class="linenos">110</span></a>    <span class="p">)</span>
-</span><span id="get_args-111"><a href="#get_args-111"><span class="linenos">111</span></a>
-</span><span id="get_args-112"><a href="#get_args-112"><span class="linenos">112</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="get_args-113"><a href="#get_args-113"><span class="linenos">113</span></a>        <span class="s2">&quot;-s&quot;</span><span class="p">,</span>
-</span><span id="get_args-114"><a href="#get_args-114"><span class="linenos">114</span></a>        <span class="s2">&quot;--sync&quot;</span><span class="p">,</span>
-</span><span id="get_args-115"><a href="#get_args-115"><span class="linenos">115</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
-</span><span id="get_args-116"><a href="#get_args-116"><span class="linenos">116</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Pull from github, then push current commit to repo. &quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="get_args-117"><a href="#get_args-117"><span class="linenos">117</span></a>    <span class="p">)</span>
-</span><span id="get_args-118"><a href="#get_args-118"><span class="linenos">118</span></a>
-</span><span id="get_args-119"><a href="#get_args-119"><span class="linenos">119</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="get_args-120"><a href="#get_args-120"><span class="linenos">120</span></a>        <span class="s2">&quot;-dv&quot;</span><span class="p">,</span>
-</span><span id="get_args-121"><a href="#get_args-121"><span class="linenos">121</span></a>        <span class="s2">&quot;--dependency_versions&quot;</span><span class="p">,</span>
-</span><span id="get_args-122"><a href="#get_args-122"><span class="linenos">122</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
-</span><span id="get_args-123"><a href="#get_args-123"><span class="linenos">123</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Include version specifiers for dependencies in</span>
-</span><span id="get_args-124"><a href="#get_args-124"><span class="linenos">124</span></a><span class="s2">        pyproject.toml.&quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="get_args-125"><a href="#get_args-125"><span class="linenos">125</span></a>    <span class="p">)</span>
-</span><span id="get_args-126"><a href="#get_args-126"><span class="linenos">126</span></a>
-</span><span id="get_args-127"><a href="#get_args-127"><span class="linenos">127</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="get_args-128"><a href="#get_args-128"><span class="linenos">128</span></a>        <span class="s2">&quot;-up&quot;</span><span class="p">,</span>
-</span><span id="get_args-129"><a href="#get_args-129"><span class="linenos">129</span></a>        <span class="s2">&quot;--update&quot;</span><span class="p">,</span>
-</span><span id="get_args-130"><a href="#get_args-130"><span class="linenos">130</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
-</span><span id="get_args-131"><a href="#get_args-131"><span class="linenos">131</span></a>        <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
-</span><span id="get_args-132"><a href="#get_args-132"><span class="linenos">132</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Excpects one argument: &quot;major&quot;, &quot;minor&quot;, or &quot;patch&quot;.</span>
-</span><span id="get_args-133"><a href="#get_args-133"><span class="linenos">133</span></a><span class="s2">        Passing &quot;-up minor&quot; is equivalent to passing the cli string: &quot;-b -t -i -iv minor -uc -ca build -s&quot;.</span>
-</span><span id="get_args-134"><a href="#get_args-134"><span class="linenos">134</span></a><span class="s2">        To publish the updated package, the -p/--publish switch needs to be added to the cli input.&quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="get_args-135"><a href="#get_args-135"><span class="linenos">135</span></a>    <span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="get_args-14"><a href="#get_args-14"><span class="linenos"> 14</span></a><span class="k">def</span> <span class="nf">get_args</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">:</span>
+</span><span id="get_args-15"><a href="#get_args-15"><span class="linenos"> 15</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">argparse</span><span class="o">.</span><span class="n">ArgumentParser</span><span class="p">()</span>
+</span><span id="get_args-16"><a href="#get_args-16"><span class="linenos"> 16</span></a>
+</span><span id="get_args-17"><a href="#get_args-17"><span class="linenos"> 17</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="get_args-18"><a href="#get_args-18"><span class="linenos"> 18</span></a>        <span class="s2">&quot;package&quot;</span><span class="p">,</span>
+</span><span id="get_args-19"><a href="#get_args-19"><span class="linenos"> 19</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
+</span><span id="get_args-20"><a href="#get_args-20"><span class="linenos"> 20</span></a>        <span class="n">default</span><span class="o">=</span><span class="s2">&quot;.&quot;</span><span class="p">,</span>
+</span><span id="get_args-21"><a href="#get_args-21"><span class="linenos"> 21</span></a>        <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;?&quot;</span><span class="p">,</span>
+</span><span id="get_args-22"><a href="#get_args-22"><span class="linenos"> 22</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; The name of the package or project to use,</span>
+</span><span id="get_args-23"><a href="#get_args-23"><span class="linenos"> 23</span></a><span class="s2">        assuming it&#39;s a subfolder of your current working directory.</span>
+</span><span id="get_args-24"><a href="#get_args-24"><span class="linenos"> 24</span></a><span class="s2">        Can also be a full path to the package. If nothing is given,</span>
+</span><span id="get_args-25"><a href="#get_args-25"><span class="linenos"> 25</span></a><span class="s2">        the current working directory will be used.&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="get_args-26"><a href="#get_args-26"><span class="linenos"> 26</span></a>    <span class="p">)</span>
+</span><span id="get_args-27"><a href="#get_args-27"><span class="linenos"> 27</span></a>
+</span><span id="get_args-28"><a href="#get_args-28"><span class="linenos"> 28</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="get_args-29"><a href="#get_args-29"><span class="linenos"> 29</span></a>        <span class="s2">&quot;-b&quot;</span><span class="p">,</span> <span class="s2">&quot;--build&quot;</span><span class="p">,</span> <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span> <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Build the package. &quot;&quot;&quot;</span>
+</span><span id="get_args-30"><a href="#get_args-30"><span class="linenos"> 30</span></a>    <span class="p">)</span>
+</span><span id="get_args-31"><a href="#get_args-31"><span class="linenos"> 31</span></a>
+</span><span id="get_args-32"><a href="#get_args-32"><span class="linenos"> 32</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="get_args-33"><a href="#get_args-33"><span class="linenos"> 33</span></a>        <span class="s2">&quot;-t&quot;</span><span class="p">,</span>
+</span><span id="get_args-34"><a href="#get_args-34"><span class="linenos"> 34</span></a>        <span class="s2">&quot;--tag_version&quot;</span><span class="p">,</span>
+</span><span id="get_args-35"><a href="#get_args-35"><span class="linenos"> 35</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="get_args-36"><a href="#get_args-36"><span class="linenos"> 36</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Add a git tag corresponding to the version in pyproject.toml. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="get_args-37"><a href="#get_args-37"><span class="linenos"> 37</span></a>    <span class="p">)</span>
+</span><span id="get_args-38"><a href="#get_args-38"><span class="linenos"> 38</span></a>
+</span><span id="get_args-39"><a href="#get_args-39"><span class="linenos"> 39</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="get_args-40"><a href="#get_args-40"><span class="linenos"> 40</span></a>        <span class="s2">&quot;-i&quot;</span><span class="p">,</span>
+</span><span id="get_args-41"><a href="#get_args-41"><span class="linenos"> 41</span></a>        <span class="s2">&quot;--install&quot;</span><span class="p">,</span>
+</span><span id="get_args-42"><a href="#get_args-42"><span class="linenos"> 42</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="get_args-43"><a href="#get_args-43"><span class="linenos"> 43</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Install the package from source. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="get_args-44"><a href="#get_args-44"><span class="linenos"> 44</span></a>    <span class="p">)</span>
+</span><span id="get_args-45"><a href="#get_args-45"><span class="linenos"> 45</span></a>
+</span><span id="get_args-46"><a href="#get_args-46"><span class="linenos"> 46</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="get_args-47"><a href="#get_args-47"><span class="linenos"> 47</span></a>        <span class="s2">&quot;-iv&quot;</span><span class="p">,</span>
+</span><span id="get_args-48"><a href="#get_args-48"><span class="linenos"> 48</span></a>        <span class="s2">&quot;--increment_version&quot;</span><span class="p">,</span>
+</span><span id="get_args-49"><a href="#get_args-49"><span class="linenos"> 49</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
+</span><span id="get_args-50"><a href="#get_args-50"><span class="linenos"> 50</span></a>        <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
+</span><span id="get_args-51"><a href="#get_args-51"><span class="linenos"> 51</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Increment version in pyproject.toml.</span>
+</span><span id="get_args-52"><a href="#get_args-52"><span class="linenos"> 52</span></a><span class="s2">        Can be one of &quot;major&quot;, &quot;minor&quot;, or &quot;patch&quot;. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="get_args-53"><a href="#get_args-53"><span class="linenos"> 53</span></a>    <span class="p">)</span>
+</span><span id="get_args-54"><a href="#get_args-54"><span class="linenos"> 54</span></a>
+</span><span id="get_args-55"><a href="#get_args-55"><span class="linenos"> 55</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="get_args-56"><a href="#get_args-56"><span class="linenos"> 56</span></a>        <span class="s2">&quot;-p&quot;</span><span class="p">,</span>
+</span><span id="get_args-57"><a href="#get_args-57"><span class="linenos"> 57</span></a>        <span class="s2">&quot;--publish&quot;</span><span class="p">,</span>
+</span><span id="get_args-58"><a href="#get_args-58"><span class="linenos"> 58</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="get_args-59"><a href="#get_args-59"><span class="linenos"> 59</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Publish package to PyPi.</span>
+</span><span id="get_args-60"><a href="#get_args-60"><span class="linenos"> 60</span></a><span class="s2">        Note: You must have configured twine </span>
+</span><span id="get_args-61"><a href="#get_args-61"><span class="linenos"> 61</span></a><span class="s2">        and registered a PyPi account/generated an API</span>
+</span><span id="get_args-62"><a href="#get_args-62"><span class="linenos"> 62</span></a><span class="s2">        key to use this option.&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="get_args-63"><a href="#get_args-63"><span class="linenos"> 63</span></a>    <span class="p">)</span>
+</span><span id="get_args-64"><a href="#get_args-64"><span class="linenos"> 64</span></a>
+</span><span id="get_args-65"><a href="#get_args-65"><span class="linenos"> 65</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="get_args-66"><a href="#get_args-66"><span class="linenos"> 66</span></a>        <span class="s2">&quot;-rt&quot;</span><span class="p">,</span>
+</span><span id="get_args-67"><a href="#get_args-67"><span class="linenos"> 67</span></a>        <span class="s2">&quot;--run_tests&quot;</span><span class="p">,</span>
+</span><span id="get_args-68"><a href="#get_args-68"><span class="linenos"> 68</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="get_args-69"><a href="#get_args-69"><span class="linenos"> 69</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Run tests for the package. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="get_args-70"><a href="#get_args-70"><span class="linenos"> 70</span></a>    <span class="p">)</span>
+</span><span id="get_args-71"><a href="#get_args-71"><span class="linenos"> 71</span></a>
+</span><span id="get_args-72"><a href="#get_args-72"><span class="linenos"> 72</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="get_args-73"><a href="#get_args-73"><span class="linenos"> 73</span></a>        <span class="s2">&quot;-gt&quot;</span><span class="p">,</span>
+</span><span id="get_args-74"><a href="#get_args-74"><span class="linenos"> 74</span></a>        <span class="s2">&quot;--generate_tests&quot;</span><span class="p">,</span>
+</span><span id="get_args-75"><a href="#get_args-75"><span class="linenos"> 75</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="get_args-76"><a href="#get_args-76"><span class="linenos"> 76</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Generate tests for the package. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="get_args-77"><a href="#get_args-77"><span class="linenos"> 77</span></a>    <span class="p">)</span>
+</span><span id="get_args-78"><a href="#get_args-78"><span class="linenos"> 78</span></a>
+</span><span id="get_args-79"><a href="#get_args-79"><span class="linenos"> 79</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="get_args-80"><a href="#get_args-80"><span class="linenos"> 80</span></a>        <span class="s2">&quot;-uc&quot;</span><span class="p">,</span>
+</span><span id="get_args-81"><a href="#get_args-81"><span class="linenos"> 81</span></a>        <span class="s2">&quot;--update_changelog&quot;</span><span class="p">,</span>
+</span><span id="get_args-82"><a href="#get_args-82"><span class="linenos"> 82</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="get_args-83"><a href="#get_args-83"><span class="linenos"> 83</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Update changelog file. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="get_args-84"><a href="#get_args-84"><span class="linenos"> 84</span></a>    <span class="p">)</span>
+</span><span id="get_args-85"><a href="#get_args-85"><span class="linenos"> 85</span></a>
+</span><span id="get_args-86"><a href="#get_args-86"><span class="linenos"> 86</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="get_args-87"><a href="#get_args-87"><span class="linenos"> 87</span></a>        <span class="s2">&quot;-od&quot;</span><span class="p">,</span>
+</span><span id="get_args-88"><a href="#get_args-88"><span class="linenos"> 88</span></a>        <span class="s2">&quot;--overwrite_dependencies&quot;</span><span class="p">,</span>
+</span><span id="get_args-89"><a href="#get_args-89"><span class="linenos"> 89</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="get_args-90"><a href="#get_args-90"><span class="linenos"> 90</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; When building a package, packagelister will be used</span>
+</span><span id="get_args-91"><a href="#get_args-91"><span class="linenos"> 91</span></a><span class="s2">        to update the dependencies list in pyproject.toml.</span>
+</span><span id="get_args-92"><a href="#get_args-92"><span class="linenos"> 92</span></a><span class="s2">        The default behavior is to append any new dependencies to</span>
+</span><span id="get_args-93"><a href="#get_args-93"><span class="linenos"> 93</span></a><span class="s2">        the current list so as not to erase any manually added dependencies</span>
+</span><span id="get_args-94"><a href="#get_args-94"><span class="linenos"> 94</span></a><span class="s2">        that packagelister may not detect. If you don&#39;t have any manually </span>
+</span><span id="get_args-95"><a href="#get_args-95"><span class="linenos"> 95</span></a><span class="s2">        added dependencies and want to remove any dependencies that your</span>
+</span><span id="get_args-96"><a href="#get_args-96"><span class="linenos"> 96</span></a><span class="s2">        project no longer uses, pass this flag.&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="get_args-97"><a href="#get_args-97"><span class="linenos"> 97</span></a>    <span class="p">)</span>
+</span><span id="get_args-98"><a href="#get_args-98"><span class="linenos"> 98</span></a>
+</span><span id="get_args-99"><a href="#get_args-99"><span class="linenos"> 99</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="get_args-100"><a href="#get_args-100"><span class="linenos">100</span></a>        <span class="s2">&quot;-ca&quot;</span><span class="p">,</span>
+</span><span id="get_args-101"><a href="#get_args-101"><span class="linenos">101</span></a>        <span class="s2">&quot;--commit_all&quot;</span><span class="p">,</span>
+</span><span id="get_args-102"><a href="#get_args-102"><span class="linenos">102</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
+</span><span id="get_args-103"><a href="#get_args-103"><span class="linenos">103</span></a>        <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
+</span><span id="get_args-104"><a href="#get_args-104"><span class="linenos">104</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Git stage and commit all tracked files</span>
+</span><span id="get_args-105"><a href="#get_args-105"><span class="linenos">105</span></a><span class="s2">        with this supplied commit message.</span>
+</span><span id="get_args-106"><a href="#get_args-106"><span class="linenos">106</span></a><span class="s2">        If &#39;build&#39; is passed, all commits will have</span>
+</span><span id="get_args-107"><a href="#get_args-107"><span class="linenos">107</span></a><span class="s2">        message: &#39;chore: build v</span><span class="si">{current_version}</span><span class="s2">&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="get_args-108"><a href="#get_args-108"><span class="linenos">108</span></a>    <span class="p">)</span>
+</span><span id="get_args-109"><a href="#get_args-109"><span class="linenos">109</span></a>
+</span><span id="get_args-110"><a href="#get_args-110"><span class="linenos">110</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="get_args-111"><a href="#get_args-111"><span class="linenos">111</span></a>        <span class="s2">&quot;-s&quot;</span><span class="p">,</span>
+</span><span id="get_args-112"><a href="#get_args-112"><span class="linenos">112</span></a>        <span class="s2">&quot;--sync&quot;</span><span class="p">,</span>
+</span><span id="get_args-113"><a href="#get_args-113"><span class="linenos">113</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="get_args-114"><a href="#get_args-114"><span class="linenos">114</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Pull from github, then push current commit to repo. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="get_args-115"><a href="#get_args-115"><span class="linenos">115</span></a>    <span class="p">)</span>
+</span><span id="get_args-116"><a href="#get_args-116"><span class="linenos">116</span></a>
+</span><span id="get_args-117"><a href="#get_args-117"><span class="linenos">117</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="get_args-118"><a href="#get_args-118"><span class="linenos">118</span></a>        <span class="s2">&quot;-dv&quot;</span><span class="p">,</span>
+</span><span id="get_args-119"><a href="#get_args-119"><span class="linenos">119</span></a>        <span class="s2">&quot;--dependency_versions&quot;</span><span class="p">,</span>
+</span><span id="get_args-120"><a href="#get_args-120"><span class="linenos">120</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="get_args-121"><a href="#get_args-121"><span class="linenos">121</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Include version specifiers for dependencies in</span>
+</span><span id="get_args-122"><a href="#get_args-122"><span class="linenos">122</span></a><span class="s2">        pyproject.toml.&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="get_args-123"><a href="#get_args-123"><span class="linenos">123</span></a>    <span class="p">)</span>
+</span><span id="get_args-124"><a href="#get_args-124"><span class="linenos">124</span></a>
+</span><span id="get_args-125"><a href="#get_args-125"><span class="linenos">125</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="get_args-126"><a href="#get_args-126"><span class="linenos">126</span></a>        <span class="s2">&quot;-up&quot;</span><span class="p">,</span>
+</span><span id="get_args-127"><a href="#get_args-127"><span class="linenos">127</span></a>        <span class="s2">&quot;--update&quot;</span><span class="p">,</span>
+</span><span id="get_args-128"><a href="#get_args-128"><span class="linenos">128</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
+</span><span id="get_args-129"><a href="#get_args-129"><span class="linenos">129</span></a>        <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
+</span><span id="get_args-130"><a href="#get_args-130"><span class="linenos">130</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Excpects one argument: &quot;major&quot;, &quot;minor&quot;, or &quot;patch&quot;.</span>
+</span><span id="get_args-131"><a href="#get_args-131"><span class="linenos">131</span></a><span class="s2">        Passing &quot;-up minor&quot; is equivalent to passing the cli string: &quot;-b -t -i -iv minor -uc -ca build -s&quot;.</span>
+</span><span id="get_args-132"><a href="#get_args-132"><span class="linenos">132</span></a><span class="s2">        To publish the updated package, the -p/--publish switch needs to be added to the cli input.&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="get_args-133"><a href="#get_args-133"><span class="linenos">133</span></a>    <span class="p">)</span>
+</span><span id="get_args-134"><a href="#get_args-134"><span class="linenos">134</span></a>
+</span><span id="get_args-135"><a href="#get_args-135"><span class="linenos">135</span></a>    <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="o">.</span><span class="n">parse_args</span><span class="p">()</span>
 </span><span id="get_args-136"><a href="#get_args-136"><span class="linenos">136</span></a>
-</span><span id="get_args-137"><a href="#get_args-137"><span class="linenos">137</span></a>    <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="o">.</span><span class="n">parse_args</span><span class="p">()</span>
+</span><span id="get_args-137"><a href="#get_args-137"><span class="linenos">137</span></a>    <span class="n">args</span><span class="o">.</span><span class="n">package</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span><span class="o">.</span><span class="n">resolve</span><span class="p">()</span>
 </span><span id="get_args-138"><a href="#get_args-138"><span class="linenos">138</span></a>
-</span><span id="get_args-139"><a href="#get_args-139"><span class="linenos">139</span></a>    <span class="n">args</span><span class="o">.</span><span class="n">package</span> <span class="o">=</span> <span class="n">Path</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span><span class="o">.</span><span class="n">resolve</span><span class="p">()</span>
-</span><span id="get_args-140"><a href="#get_args-140"><span class="linenos">140</span></a>
-</span><span id="get_args-141"><a href="#get_args-141"><span class="linenos">141</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">update</span><span class="p">:</span>
-</span><span id="get_args-142"><a href="#get_args-142"><span class="linenos">142</span></a>        <span class="n">args</span><span class="o">.</span><span class="n">build</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="get_args-143"><a href="#get_args-143"><span class="linenos">143</span></a>        <span class="n">args</span><span class="o">.</span><span class="n">tag_version</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="get_args-144"><a href="#get_args-144"><span class="linenos">144</span></a>        <span class="n">args</span><span class="o">.</span><span class="n">install</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="get_args-145"><a href="#get_args-145"><span class="linenos">145</span></a>        <span class="n">args</span><span class="o">.</span><span class="n">increment_version</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">update</span>
-</span><span id="get_args-146"><a href="#get_args-146"><span class="linenos">146</span></a>        <span class="n">args</span><span class="o">.</span><span class="n">update_changelog</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="get_args-147"><a href="#get_args-147"><span class="linenos">147</span></a>        <span class="n">args</span><span class="o">.</span><span class="n">commit_all</span> <span class="o">=</span> <span class="s2">&quot;build&quot;</span>
-</span><span id="get_args-148"><a href="#get_args-148"><span class="linenos">148</span></a>        <span class="n">args</span><span class="o">.</span><span class="n">sync</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="get_args-149"><a href="#get_args-149"><span class="linenos">149</span></a>
-</span><span id="get_args-150"><a href="#get_args-150"><span class="linenos">150</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">increment_version</span> <span class="ow">and</span> <span class="n">args</span><span class="o">.</span><span class="n">increment_version</span> <span class="ow">not</span> <span class="ow">in</span> <span class="p">[</span>
-</span><span id="get_args-151"><a href="#get_args-151"><span class="linenos">151</span></a>        <span class="s2">&quot;major&quot;</span><span class="p">,</span>
-</span><span id="get_args-152"><a href="#get_args-152"><span class="linenos">152</span></a>        <span class="s2">&quot;minor&quot;</span><span class="p">,</span>
-</span><span id="get_args-153"><a href="#get_args-153"><span class="linenos">153</span></a>        <span class="s2">&quot;patch&quot;</span><span class="p">,</span>
-</span><span id="get_args-154"><a href="#get_args-154"><span class="linenos">154</span></a>    <span class="p">]:</span>
-</span><span id="get_args-155"><a href="#get_args-155"><span class="linenos">155</span></a>        <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span>
-</span><span id="get_args-156"><a href="#get_args-156"><span class="linenos">156</span></a>            <span class="sa">f</span><span class="s2">&quot;Invalid option for -iv/--increment_version: </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">increment_version</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="get_args-157"><a href="#get_args-157"><span class="linenos">157</span></a>        <span class="p">)</span>
-</span><span id="get_args-158"><a href="#get_args-158"><span class="linenos">158</span></a>
-</span><span id="get_args-159"><a href="#get_args-159"><span class="linenos">159</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">commit_all</span> <span class="o">==</span> <span class="s2">&quot;&quot;</span><span class="p">:</span>
-</span><span id="get_args-160"><a href="#get_args-160"><span class="linenos">160</span></a>        <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="s2">&quot;Commit message for args.commit_all cannot be empty.&quot;</span><span class="p">)</span>
-</span><span id="get_args-161"><a href="#get_args-161"><span class="linenos">161</span></a>
-</span><span id="get_args-162"><a href="#get_args-162"><span class="linenos">162</span></a>    <span class="k">return</span> <span class="n">args</span>
+</span><span id="get_args-139"><a href="#get_args-139"><span class="linenos">139</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">update</span><span class="p">:</span>
+</span><span id="get_args-140"><a href="#get_args-140"><span class="linenos">140</span></a>        <span class="n">args</span><span class="o">.</span><span class="n">build</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="get_args-141"><a href="#get_args-141"><span class="linenos">141</span></a>        <span class="n">args</span><span class="o">.</span><span class="n">tag_version</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="get_args-142"><a href="#get_args-142"><span class="linenos">142</span></a>        <span class="n">args</span><span class="o">.</span><span class="n">install</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="get_args-143"><a href="#get_args-143"><span class="linenos">143</span></a>        <span class="n">args</span><span class="o">.</span><span class="n">increment_version</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">update</span>
+</span><span id="get_args-144"><a href="#get_args-144"><span class="linenos">144</span></a>        <span class="n">args</span><span class="o">.</span><span class="n">update_changelog</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="get_args-145"><a href="#get_args-145"><span class="linenos">145</span></a>        <span class="n">args</span><span class="o">.</span><span class="n">commit_all</span> <span class="o">=</span> <span class="s2">&quot;build&quot;</span>
+</span><span id="get_args-146"><a href="#get_args-146"><span class="linenos">146</span></a>        <span class="n">args</span><span class="o">.</span><span class="n">sync</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="get_args-147"><a href="#get_args-147"><span class="linenos">147</span></a>
+</span><span id="get_args-148"><a href="#get_args-148"><span class="linenos">148</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">increment_version</span> <span class="ow">and</span> <span class="n">args</span><span class="o">.</span><span class="n">increment_version</span> <span class="ow">not</span> <span class="ow">in</span> <span class="p">[</span>
+</span><span id="get_args-149"><a href="#get_args-149"><span class="linenos">149</span></a>        <span class="s2">&quot;major&quot;</span><span class="p">,</span>
+</span><span id="get_args-150"><a href="#get_args-150"><span class="linenos">150</span></a>        <span class="s2">&quot;minor&quot;</span><span class="p">,</span>
+</span><span id="get_args-151"><a href="#get_args-151"><span class="linenos">151</span></a>        <span class="s2">&quot;patch&quot;</span><span class="p">,</span>
+</span><span id="get_args-152"><a href="#get_args-152"><span class="linenos">152</span></a>    <span class="p">]:</span>
+</span><span id="get_args-153"><a href="#get_args-153"><span class="linenos">153</span></a>        <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span>
+</span><span id="get_args-154"><a href="#get_args-154"><span class="linenos">154</span></a>            <span class="sa">f</span><span class="s2">&quot;Invalid option for -iv/--increment_version: </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">increment_version</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="get_args-155"><a href="#get_args-155"><span class="linenos">155</span></a>        <span class="p">)</span>
+</span><span id="get_args-156"><a href="#get_args-156"><span class="linenos">156</span></a>
+</span><span id="get_args-157"><a href="#get_args-157"><span class="linenos">157</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">commit_all</span> <span class="o">==</span> <span class="s2">&quot;&quot;</span><span class="p">:</span>
+</span><span id="get_args-158"><a href="#get_args-158"><span class="linenos">158</span></a>        <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="s2">&quot;Commit message for args.commit_all cannot be empty.&quot;</span><span class="p">)</span>
+</span><span id="get_args-159"><a href="#get_args-159"><span class="linenos">159</span></a>
+</span><span id="get_args-160"><a href="#get_args-160"><span class="linenos">160</span></a>    <span class="k">return</span> <span class="n">args</span>
 </span></pre></div>
 
 
     
 
                 </section>
                 <section id="main">
@@ -461,76 +456,73 @@
         <span class="def">def</span>
         <span class="name">main</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">=</span> <span class="kc">None</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="main-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#main"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="main-165"><a href="#main-165"><span class="linenos">165</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
-</span><span id="main-166"><a href="#main-166"><span class="linenos">166</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="p">:</span>
-</span><span id="main-167"><a href="#main-167"><span class="linenos">167</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="main-163"><a href="#main-163"><span class="linenos">163</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
+</span><span id="main-164"><a href="#main-164"><span class="linenos">164</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="p">:</span>
+</span><span id="main-165"><a href="#main-165"><span class="linenos">165</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
+</span><span id="main-166"><a href="#main-166"><span class="linenos">166</span></a>
+</span><span id="main-167"><a href="#main-167"><span class="linenos">167</span></a>    <span class="n">pyproject_path</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">package</span> <span class="o">/</span> <span class="s2">&quot;pyproject.toml&quot;</span>
 </span><span id="main-168"><a href="#main-168"><span class="linenos">168</span></a>
-</span><span id="main-169"><a href="#main-169"><span class="linenos">169</span></a>    <span class="n">pyproject_path</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">package</span> <span class="o">/</span> <span class="s2">&quot;pyproject.toml&quot;</span>
-</span><span id="main-170"><a href="#main-170"><span class="linenos">170</span></a>
-</span><span id="main-171"><a href="#main-171"><span class="linenos">171</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">pyproject_path</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
-</span><span id="main-172"><a href="#main-172"><span class="linenos">172</span></a>        <span class="k">raise</span> <span class="ne">FileNotFoundError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Could not locate pyproject.toml for </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="main-173"><a href="#main-173"><span class="linenos">173</span></a>
-</span><span id="main-174"><a href="#main-174"><span class="linenos">174</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">generate_tests</span><span class="p">:</span>
-</span><span id="main-175"><a href="#main-175"><span class="linenos">175</span></a>        <span class="n">generate_test_files</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span>
-</span><span id="main-176"><a href="#main-176"><span class="linenos">176</span></a>
-</span><span id="main-177"><a href="#main-177"><span class="linenos">177</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">run_tests</span><span class="p">:</span>
-</span><span id="main-178"><a href="#main-178"><span class="linenos">178</span></a>        <span class="n">run_tests</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span>
-</span><span id="main-179"><a href="#main-179"><span class="linenos">179</span></a>
-</span><span id="main-180"><a href="#main-180"><span class="linenos">180</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">increment_version</span><span class="p">:</span>
-</span><span id="main-181"><a href="#main-181"><span class="linenos">181</span></a>        <span class="n">hassle_utilities</span><span class="o">.</span><span class="n">increment_version</span><span class="p">(</span><span class="n">pyproject_path</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">increment_version</span><span class="p">)</span>
-</span><span id="main-182"><a href="#main-182"><span class="linenos">182</span></a>
-</span><span id="main-183"><a href="#main-183"><span class="linenos">183</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">build</span><span class="p">:</span>
-</span><span id="main-184"><a href="#main-184"><span class="linenos">184</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="main-185"><a href="#main-185"><span class="linenos">185</span></a>            <span class="n">shutil</span><span class="o">.</span><span class="n">rmtree</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="si">}</span><span class="s2">/dist&quot;</span><span class="p">)</span>
-</span><span id="main-186"><a href="#main-186"><span class="linenos">186</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="main-187"><a href="#main-187"><span class="linenos">187</span></a>            <span class="k">pass</span>
-</span><span id="main-188"><a href="#main-188"><span class="linenos">188</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;black </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="main-189"><a href="#main-189"><span class="linenos">189</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;isort </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="main-190"><a href="#main-190"><span class="linenos">190</span></a>        <span class="n">hassle_utilities</span><span class="o">.</span><span class="n">update_dependencies</span><span class="p">(</span>
-</span><span id="main-191"><a href="#main-191"><span class="linenos">191</span></a>            <span class="n">pyproject_path</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">overwrite_dependencies</span>
-</span><span id="main-192"><a href="#main-192"><span class="linenos">192</span></a>        <span class="p">)</span>
-</span><span id="main-193"><a href="#main-193"><span class="linenos">193</span></a>        <span class="n">hassle_utilities</span><span class="o">.</span><span class="n">update_minimum_python_version</span><span class="p">(</span><span class="n">pyproject_path</span><span class="p">)</span>
-</span><span id="main-194"><a href="#main-194"><span class="linenos">194</span></a>        <span class="n">hassle_utilities</span><span class="o">.</span><span class="n">generate_docs</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span>
-</span><span id="main-195"><a href="#main-195"><span class="linenos">195</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;py -m build </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="main-196"><a href="#main-196"><span class="linenos">196</span></a>
-</span><span id="main-197"><a href="#main-197"><span class="linenos">197</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">update_changelog</span><span class="p">:</span>
-</span><span id="main-198"><a href="#main-198"><span class="linenos">198</span></a>        <span class="n">hassle_utilities</span><span class="o">.</span><span class="n">update_changelog</span><span class="p">(</span><span class="n">pyproject_path</span><span class="p">)</span>
-</span><span id="main-199"><a href="#main-199"><span class="linenos">199</span></a>        <span class="c1"># If we&#39;re going to add tag for current version</span>
-</span><span id="main-200"><a href="#main-200"><span class="linenos">200</span></a>        <span class="c1"># commit changelog first</span>
-</span><span id="main-201"><a href="#main-201"><span class="linenos">201</span></a>        <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">tag_version</span><span class="p">:</span>
-</span><span id="main-202"><a href="#main-202"><span class="linenos">202</span></a>            <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span>
-</span><span id="main-203"><a href="#main-203"><span class="linenos">203</span></a>            <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="s2">&quot;git add CHANGELOG.md&quot;</span><span class="p">)</span>
-</span><span id="main-204"><a href="#main-204"><span class="linenos">204</span></a>            <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="s1">&#39;git commit CHANGELOG.md -m &quot;chore: update changelog&quot;&#39;</span><span class="p">)</span>
-</span><span id="main-205"><a href="#main-205"><span class="linenos">205</span></a>
-</span><span id="main-206"><a href="#main-206"><span class="linenos">206</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">commit_all</span><span class="p">:</span>
-</span><span id="main-207"><a href="#main-207"><span class="linenos">207</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span>
-</span><span id="main-208"><a href="#main-208"><span class="linenos">208</span></a>        <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">commit_all</span> <span class="o">==</span> <span class="s2">&quot;build&quot;</span><span class="p">:</span>
-</span><span id="main-209"><a href="#main-209"><span class="linenos">209</span></a>            <span class="n">version</span> <span class="o">=</span> <span class="n">tomlkit</span><span class="o">.</span><span class="n">loads</span><span class="p">(</span><span class="n">pyproject_path</span><span class="o">.</span><span class="n">read_text</span><span class="p">())[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;version&quot;</span><span class="p">]</span>
-</span><span id="main-210"><a href="#main-210"><span class="linenos">210</span></a>            <span class="n">args</span><span class="o">.</span><span class="n">commit_all</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;chore: build v</span><span class="si">{</span><span class="n">version</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="main-211"><a href="#main-211"><span class="linenos">211</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="s2">&quot;git add .&quot;</span><span class="p">)</span>
-</span><span id="main-212"><a href="#main-212"><span class="linenos">212</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;git commit -m &quot;</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">commit_all</span><span class="si">}</span><span class="s1">&quot;&#39;</span><span class="p">)</span>
-</span><span id="main-213"><a href="#main-213"><span class="linenos">213</span></a>
-</span><span id="main-214"><a href="#main-214"><span class="linenos">214</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">tag_version</span><span class="p">:</span>
-</span><span id="main-215"><a href="#main-215"><span class="linenos">215</span></a>        <span class="n">hassle_utilities</span><span class="o">.</span><span class="n">tag_version</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span>
-</span><span id="main-216"><a href="#main-216"><span class="linenos">216</span></a>
-</span><span id="main-217"><a href="#main-217"><span class="linenos">217</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">publish</span><span class="p">:</span>
-</span><span id="main-218"><a href="#main-218"><span class="linenos">218</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;twine upload </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">package</span> <span class="o">/</span> <span class="s1">&#39;dist&#39;</span> <span class="o">/</span> <span class="s1">&#39;*&#39;</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="main-219"><a href="#main-219"><span class="linenos">219</span></a>
-</span><span id="main-220"><a href="#main-220"><span class="linenos">220</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">install</span><span class="p">:</span>
-</span><span id="main-221"><a href="#main-221"><span class="linenos">221</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;pip install </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="si">}</span><span class="s2"> --no-deps --upgrade --no-cache-dir&quot;</span><span class="p">)</span>
-</span><span id="main-222"><a href="#main-222"><span class="linenos">222</span></a>
-</span><span id="main-223"><a href="#main-223"><span class="linenos">223</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">sync</span><span class="p">:</span>
-</span><span id="main-224"><a href="#main-224"><span class="linenos">224</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span>
-</span><span id="main-225"><a href="#main-225"><span class="linenos">225</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;git pull --tags origin main&quot;</span><span class="p">)</span>
-</span><span id="main-226"><a href="#main-226"><span class="linenos">226</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;git push origin main:main --tags&quot;</span><span class="p">)</span>
+</span><span id="main-169"><a href="#main-169"><span class="linenos">169</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">pyproject_path</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
+</span><span id="main-170"><a href="#main-170"><span class="linenos">170</span></a>        <span class="k">raise</span> <span class="ne">FileNotFoundError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Could not locate pyproject.toml for </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="main-171"><a href="#main-171"><span class="linenos">171</span></a>
+</span><span id="main-172"><a href="#main-172"><span class="linenos">172</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">generate_tests</span><span class="p">:</span>
+</span><span id="main-173"><a href="#main-173"><span class="linenos">173</span></a>        <span class="n">generate_test_files</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span>
+</span><span id="main-174"><a href="#main-174"><span class="linenos">174</span></a>
+</span><span id="main-175"><a href="#main-175"><span class="linenos">175</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">run_tests</span><span class="p">:</span>
+</span><span id="main-176"><a href="#main-176"><span class="linenos">176</span></a>        <span class="n">run_tests</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span>
+</span><span id="main-177"><a href="#main-177"><span class="linenos">177</span></a>
+</span><span id="main-178"><a href="#main-178"><span class="linenos">178</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">increment_version</span><span class="p">:</span>
+</span><span id="main-179"><a href="#main-179"><span class="linenos">179</span></a>        <span class="n">hassle_utilities</span><span class="o">.</span><span class="n">increment_version</span><span class="p">(</span><span class="n">pyproject_path</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">increment_version</span><span class="p">)</span>
+</span><span id="main-180"><a href="#main-180"><span class="linenos">180</span></a>
+</span><span id="main-181"><a href="#main-181"><span class="linenos">181</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">build</span><span class="p">:</span>
+</span><span id="main-182"><a href="#main-182"><span class="linenos">182</span></a>        <span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span> <span class="o">/</span> <span class="s2">&quot;dist&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">delete</span><span class="p">()</span>
+</span><span id="main-183"><a href="#main-183"><span class="linenos">183</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;black </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="main-184"><a href="#main-184"><span class="linenos">184</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;isort </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="main-185"><a href="#main-185"><span class="linenos">185</span></a>        <span class="n">hassle_utilities</span><span class="o">.</span><span class="n">update_dependencies</span><span class="p">(</span>
+</span><span id="main-186"><a href="#main-186"><span class="linenos">186</span></a>            <span class="n">pyproject_path</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">overwrite_dependencies</span>
+</span><span id="main-187"><a href="#main-187"><span class="linenos">187</span></a>        <span class="p">)</span>
+</span><span id="main-188"><a href="#main-188"><span class="linenos">188</span></a>        <span class="n">hassle_utilities</span><span class="o">.</span><span class="n">update_minimum_python_version</span><span class="p">(</span><span class="n">pyproject_path</span><span class="p">)</span>
+</span><span id="main-189"><a href="#main-189"><span class="linenos">189</span></a>        <span class="n">hassle_utilities</span><span class="o">.</span><span class="n">generate_docs</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span>
+</span><span id="main-190"><a href="#main-190"><span class="linenos">190</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;py -m build </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="main-191"><a href="#main-191"><span class="linenos">191</span></a>
+</span><span id="main-192"><a href="#main-192"><span class="linenos">192</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">update_changelog</span><span class="p">:</span>
+</span><span id="main-193"><a href="#main-193"><span class="linenos">193</span></a>        <span class="n">hassle_utilities</span><span class="o">.</span><span class="n">update_changelog</span><span class="p">(</span><span class="n">pyproject_path</span><span class="p">)</span>
+</span><span id="main-194"><a href="#main-194"><span class="linenos">194</span></a>        <span class="c1"># If we&#39;re going to add tag for current version</span>
+</span><span id="main-195"><a href="#main-195"><span class="linenos">195</span></a>        <span class="c1"># commit changelog first</span>
+</span><span id="main-196"><a href="#main-196"><span class="linenos">196</span></a>        <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">tag_version</span><span class="p">:</span>
+</span><span id="main-197"><a href="#main-197"><span class="linenos">197</span></a>            <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span>
+</span><span id="main-198"><a href="#main-198"><span class="linenos">198</span></a>            <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="s2">&quot;git add CHANGELOG.md&quot;</span><span class="p">)</span>
+</span><span id="main-199"><a href="#main-199"><span class="linenos">199</span></a>            <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="s1">&#39;git commit CHANGELOG.md -m &quot;chore: update changelog&quot;&#39;</span><span class="p">)</span>
+</span><span id="main-200"><a href="#main-200"><span class="linenos">200</span></a>
+</span><span id="main-201"><a href="#main-201"><span class="linenos">201</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">commit_all</span><span class="p">:</span>
+</span><span id="main-202"><a href="#main-202"><span class="linenos">202</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span>
+</span><span id="main-203"><a href="#main-203"><span class="linenos">203</span></a>        <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">commit_all</span> <span class="o">==</span> <span class="s2">&quot;build&quot;</span><span class="p">:</span>
+</span><span id="main-204"><a href="#main-204"><span class="linenos">204</span></a>            <span class="n">version</span> <span class="o">=</span> <span class="n">pyproject_path</span><span class="o">.</span><span class="n">loads</span><span class="p">()[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;version&quot;</span><span class="p">]</span>
+</span><span id="main-205"><a href="#main-205"><span class="linenos">205</span></a>            <span class="n">args</span><span class="o">.</span><span class="n">commit_all</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;chore: build v</span><span class="si">{</span><span class="n">version</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="main-206"><a href="#main-206"><span class="linenos">206</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="s2">&quot;git add .&quot;</span><span class="p">)</span>
+</span><span id="main-207"><a href="#main-207"><span class="linenos">207</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;git commit -m &quot;</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">commit_all</span><span class="si">}</span><span class="s1">&quot;&#39;</span><span class="p">)</span>
+</span><span id="main-208"><a href="#main-208"><span class="linenos">208</span></a>
+</span><span id="main-209"><a href="#main-209"><span class="linenos">209</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">tag_version</span><span class="p">:</span>
+</span><span id="main-210"><a href="#main-210"><span class="linenos">210</span></a>        <span class="n">hassle_utilities</span><span class="o">.</span><span class="n">tag_version</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span>
+</span><span id="main-211"><a href="#main-211"><span class="linenos">211</span></a>
+</span><span id="main-212"><a href="#main-212"><span class="linenos">212</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">publish</span><span class="p">:</span>
+</span><span id="main-213"><a href="#main-213"><span class="linenos">213</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;twine upload </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">package</span> <span class="o">/</span> <span class="s1">&#39;dist&#39;</span> <span class="o">/</span> <span class="s1">&#39;*&#39;</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="main-214"><a href="#main-214"><span class="linenos">214</span></a>
+</span><span id="main-215"><a href="#main-215"><span class="linenos">215</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">install</span><span class="p">:</span>
+</span><span id="main-216"><a href="#main-216"><span class="linenos">216</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;pip install </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="si">}</span><span class="s2"> --no-deps --upgrade --no-cache-dir&quot;</span><span class="p">)</span>
+</span><span id="main-217"><a href="#main-217"><span class="linenos">217</span></a>
+</span><span id="main-218"><a href="#main-218"><span class="linenos">218</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">sync</span><span class="p">:</span>
+</span><span id="main-219"><a href="#main-219"><span class="linenos">219</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span>
+</span><span id="main-220"><a href="#main-220"><span class="linenos">220</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;git pull --tags origin main&quot;</span><span class="p">)</span>
+</span><span id="main-221"><a href="#main-221"><span class="linenos">221</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;git push origin main:main --tags&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
     
 
                 </section>
     </main>
```

#### html2text {}

```diff
@@ -7,470 +7,460 @@
     * main
 built_with_pdoc[pdoc_logo]
 
 ****** hassle.hassle ******
 ⁰ View Source
 __1import argparse
 __2import os
-__3import shutil
-__4from pathlib import Path
+__3
+__4from pathier import Pathier
 __5
-__6import tomlkit
-__7
-__8from hassle import hassle_utilities
-__9from hassle.generate_tests import generate_test_files
-_10from hassle.run_tests import run_tests
+__6from hassle import hassle_utilities
+__7from hassle.generate_tests import generate_test_files
+__8from hassle.run_tests import run_tests
+__9
+_10root = Pathier(__file__).parent
 _11
-_12root = Path(__file__).parent
-_13
-_14
-_15def get_args() -> argparse.Namespace:
-_16    parser = argparse.ArgumentParser()
-_17
-_18    parser.add_argument(
-_19        "package",
-_20        type=str,
-_21        default=".",
-_22        nargs="?",
-_23        help=""" The name of the package or project to use,
-_24        assuming it's a subfolder of your current working directory.
-_25        Can also be a full path to the package. If nothing is given,
-_26        the current working directory will be used.""",
-_27    )
-_28
-_29    parser.add_argument(
-_30        "-b", "--build", action="store_true", help=""" Build the package.
+_12
+_13def get_args() -> argparse.Namespace:
+_14    parser = argparse.ArgumentParser()
+_15
+_16    parser.add_argument(
+_17        "package",
+_18        type=str,
+_19        default=".",
+_20        nargs="?",
+_21        help=""" The name of the package or project to use,
+_22        assuming it's a subfolder of your current working directory.
+_23        Can also be a full path to the package. If nothing is given,
+_24        the current working directory will be used.""",
+_25    )
+_26
+_27    parser.add_argument(
+_28        "-b", "--build", action="store_true", help=""" Build the package.
 """
-_31    )
-_32
-_33    parser.add_argument(
-_34        "-t",
-_35        "--tag_version",
-_36        action="store_true",
-_37        help=""" Add a git tag corresponding to the version in
+_29    )
+_30
+_31    parser.add_argument(
+_32        "-t",
+_33        "--tag_version",
+_34        action="store_true",
+_35        help=""" Add a git tag corresponding to the version in
 pyproject.toml. """,
-_38    )
-_39
-_40    parser.add_argument(
-_41        "-i",
-_42        "--install",
-_43        action="store_true",
-_44        help=""" Install the package from source. """,
-_45    )
-_46
-_47    parser.add_argument(
-_48        "-iv",
-_49        "--increment_version",
-_50        type=str,
-_51        default=None,
-_52        help=""" Increment version in pyproject.toml.
-_53        Can be one of "major", "minor", or "patch". """,
-_54    )
-_55
-_56    parser.add_argument(
-_57        "-p",
-_58        "--publish",
-_59        action="store_true",
-_60        help=""" Publish package to PyPi.
-_61        Note: You must have configured twine
-_62        and registered a PyPi account/generated an API
-_63        key to use this option.""",
-_64    )
-_65
-_66    parser.add_argument(
-_67        "-rt",
-_68        "--run_tests",
-_69        action="store_true",
-_70        help=""" Run tests for the package. """,
-_71    )
-_72
-_73    parser.add_argument(
-_74        "-gt",
-_75        "--generate_tests",
-_76        action="store_true",
-_77        help=""" Generate tests for the package. """,
-_78    )
-_79
-_80    parser.add_argument(
-_81        "-uc",
-_82        "--update_changelog",
-_83        action="store_true",
-_84        help=""" Update changelog file. """,
-_85    )
-_86
-_87    parser.add_argument(
-_88        "-od",
-_89        "--overwrite_dependencies",
-_90        action="store_true",
-_91        help=""" When building a package, packagelister will be used
-_92        to update the dependencies list in pyproject.toml.
-_93        The default behavior is to append any new dependencies to
-_94        the current list so as not to erase any manually added dependencies
-_95        that packagelister may not detect. If you don't have any manually
-_96        added dependencies and want to remove any dependencies that your
-_97        project no longer uses, pass this flag.""",
-_98    )
-_99
-100    parser.add_argument(
-101        "-ca",
-102        "--commit_all",
-103        type=str,
-104        default=None,
-105        help=""" Git stage and commit all tracked files
-106        with this supplied commit message.
-107        If 'build' is passed, all commits will have
-108        message: 'chore: build v{current_version}""",
-109    )
-110
-111    parser.add_argument(
-112        "-s",
-113        "--sync",
-114        action="store_true",
-115        help=""" Pull from github, then push current commit to repo. """,
-116    )
-117
-118    parser.add_argument(
-119        "-dv",
-120        "--dependency_versions",
-121        action="store_true",
-122        help=""" Include version specifiers for dependencies in
-123        pyproject.toml.""",
-124    )
-125
-126    parser.add_argument(
-127        "-up",
-128        "--update",
-129        type=str,
-130        default=None,
-131        help=""" Excpects one argument: "major", "minor", or "patch".
-132        Passing "-up minor" is equivalent to passing the cli string: "-b -
+_36    )
+_37
+_38    parser.add_argument(
+_39        "-i",
+_40        "--install",
+_41        action="store_true",
+_42        help=""" Install the package from source. """,
+_43    )
+_44
+_45    parser.add_argument(
+_46        "-iv",
+_47        "--increment_version",
+_48        type=str,
+_49        default=None,
+_50        help=""" Increment version in pyproject.toml.
+_51        Can be one of "major", "minor", or "patch". """,
+_52    )
+_53
+_54    parser.add_argument(
+_55        "-p",
+_56        "--publish",
+_57        action="store_true",
+_58        help=""" Publish package to PyPi.
+_59        Note: You must have configured twine
+_60        and registered a PyPi account/generated an API
+_61        key to use this option.""",
+_62    )
+_63
+_64    parser.add_argument(
+_65        "-rt",
+_66        "--run_tests",
+_67        action="store_true",
+_68        help=""" Run tests for the package. """,
+_69    )
+_70
+_71    parser.add_argument(
+_72        "-gt",
+_73        "--generate_tests",
+_74        action="store_true",
+_75        help=""" Generate tests for the package. """,
+_76    )
+_77
+_78    parser.add_argument(
+_79        "-uc",
+_80        "--update_changelog",
+_81        action="store_true",
+_82        help=""" Update changelog file. """,
+_83    )
+_84
+_85    parser.add_argument(
+_86        "-od",
+_87        "--overwrite_dependencies",
+_88        action="store_true",
+_89        help=""" When building a package, packagelister will be used
+_90        to update the dependencies list in pyproject.toml.
+_91        The default behavior is to append any new dependencies to
+_92        the current list so as not to erase any manually added dependencies
+_93        that packagelister may not detect. If you don't have any manually
+_94        added dependencies and want to remove any dependencies that your
+_95        project no longer uses, pass this flag.""",
+_96    )
+_97
+_98    parser.add_argument(
+_99        "-ca",
+100        "--commit_all",
+101        type=str,
+102        default=None,
+103        help=""" Git stage and commit all tracked files
+104        with this supplied commit message.
+105        If 'build' is passed, all commits will have
+106        message: 'chore: build v{current_version}""",
+107    )
+108
+109    parser.add_argument(
+110        "-s",
+111        "--sync",
+112        action="store_true",
+113        help=""" Pull from github, then push current commit to repo. """,
+114    )
+115
+116    parser.add_argument(
+117        "-dv",
+118        "--dependency_versions",
+119        action="store_true",
+120        help=""" Include version specifiers for dependencies in
+121        pyproject.toml.""",
+122    )
+123
+124    parser.add_argument(
+125        "-up",
+126        "--update",
+127        type=str,
+128        default=None,
+129        help=""" Excpects one argument: "major", "minor", or "patch".
+130        Passing "-up minor" is equivalent to passing the cli string: "-b -
 t -i -iv minor -uc -ca build -s".
-133        To publish the updated package, the -p/--publish switch needs to be
+131        To publish the updated package, the -p/--publish switch needs to be
 added to the cli input.""",
-134    )
+132    )
+133
+134    args = parser.parse_args()
 135
-136    args = parser.parse_args()
+136    args.package = Pathier(args.package).resolve()
 137
-138    args.package = Path(args.package).resolve()
-139
-140    if args.update:
-141        args.build = True
-142        args.tag_version = True
-143        args.install = True
-144        args.increment_version = args.update
-145        args.update_changelog = True
-146        args.commit_all = "build"
-147        args.sync = True
-148
-149    if args.increment_version and args.increment_version not in [
-150        "major",
-151        "minor",
-152        "patch",
-153    ]:
-154        raise ValueError(
-155            f"Invalid option for -iv/--increment_version:
+138    if args.update:
+139        args.build = True
+140        args.tag_version = True
+141        args.install = True
+142        args.increment_version = args.update
+143        args.update_changelog = True
+144        args.commit_all = "build"
+145        args.sync = True
+146
+147    if args.increment_version and args.increment_version not in [
+148        "major",
+149        "minor",
+150        "patch",
+151    ]:
+152        raise ValueError(
+153            f"Invalid option for -iv/--increment_version:
 {args.increment_version}"
-156        )
-157
-158    if args.commit_all == "":
-159        raise ValueError("Commit message for args.commit_all cannot be
+154        )
+155
+156    if args.commit_all == "":
+157        raise ValueError("Commit message for args.commit_all cannot be
 empty.")
+158
+159    return args
 160
-161    return args
-162
-163
-164def main(args: argparse.Namespace = None):
-165    if not args:
-166        args = get_args()
+161
+162def main(args: argparse.Namespace = None):
+163    if not args:
+164        args = get_args()
+165
+166    pyproject_path = args.package / "pyproject.toml"
 167
-168    pyproject_path = args.package / "pyproject.toml"
-169
-170    if not pyproject_path.exists():
-171        raise FileNotFoundError(f"Could not locate pyproject.toml for
+168    if not pyproject_path.exists():
+169        raise FileNotFoundError(f"Could not locate pyproject.toml for
 {args.package}")
-172
-173    if args.generate_tests:
-174        generate_test_files(args.package)
-175
-176    if args.run_tests:
-177        run_tests(args.package)
-178
-179    if args.increment_version:
-180        hassle_utilities.increment_version(pyproject_path,
+170
+171    if args.generate_tests:
+172        generate_test_files(args.package)
+173
+174    if args.run_tests:
+175        run_tests(args.package)
+176
+177    if args.increment_version:
+178        hassle_utilities.increment_version(pyproject_path,
 args.increment_version)
-181
-182    if args.build:
-183        try:
-184            shutil.rmtree(f"{args.package}/dist")
-185        except Exception as e:
-186            pass
-187        os.system(f"black {args.package}")
-188        os.system(f"isort {args.package}")
-189        hassle_utilities.update_dependencies(
-190            pyproject_path, args.overwrite_dependencies
-191        )
-192        hassle_utilities.update_minimum_python_version(pyproject_path)
-193        hassle_utilities.generate_docs(args.package)
-194        os.system(f"py -m build {args.package}")
-195
-196    if args.update_changelog:
-197        hassle_utilities.update_changelog(pyproject_path)
-198        # If we're going to add tag for current version
-199        # commit changelog first
-200        if args.tag_version:
-201            os.chdir(args.package)
-202            os.system("git add CHANGELOG.md")
-203            os.system('git commit CHANGELOG.md -m "chore: update
+179
+180    if args.build:
+181        (args.package / "dist").delete()
+182        os.system(f"black {args.package}")
+183        os.system(f"isort {args.package}")
+184        hassle_utilities.update_dependencies(
+185            pyproject_path, args.overwrite_dependencies
+186        )
+187        hassle_utilities.update_minimum_python_version(pyproject_path)
+188        hassle_utilities.generate_docs(args.package)
+189        os.system(f"py -m build {args.package}")
+190
+191    if args.update_changelog:
+192        hassle_utilities.update_changelog(pyproject_path)
+193        # If we're going to add tag for current version
+194        # commit changelog first
+195        if args.tag_version:
+196            os.chdir(args.package)
+197            os.system("git add CHANGELOG.md")
+198            os.system('git commit CHANGELOG.md -m "chore: update
 changelog"')
-204
-205    if args.commit_all:
-206        os.chdir(args.package)
-207        if args.commit_all == "build":
-208            version = tomlkit.loads(pyproject_path.read_text())["project"]
-["version"]
-209            args.commit_all = f"chore: build v{version}"
-210        os.system("git add .")
-211        os.system(f'git commit -m "{args.commit_all}"')
-212
-213    if args.tag_version:
-214        hassle_utilities.tag_version(args.package)
-215
-216    if args.publish:
-217        os.system(f"twine upload {args.package / 'dist' / '*'}")
-218
-219    if args.install:
-220        os.system(f"pip install {args.package} --no-deps --upgrade --no-
+199
+200    if args.commit_all:
+201        os.chdir(args.package)
+202        if args.commit_all == "build":
+203            version = pyproject_path.loads()["project"]["version"]
+204            args.commit_all = f"chore: build v{version}"
+205        os.system("git add .")
+206        os.system(f'git commit -m "{args.commit_all}"')
+207
+208    if args.tag_version:
+209        hassle_utilities.tag_version(args.package)
+210
+211    if args.publish:
+212        os.system(f"twine upload {args.package / 'dist' / '*'}")
+213
+214    if args.install:
+215        os.system(f"pip install {args.package} --no-deps --upgrade --no-
 cache-dir")
+216
+217    if args.sync:
+218        os.chdir(args.package)
+219        os.system(f"git pull --tags origin main")
+220        os.system(f"git push origin main:main --tags")
 221
-222    if args.sync:
-223        os.chdir(args.package)
-224        os.system(f"git pull --tags origin main")
-225        os.system(f"git push origin main:main --tags")
-226
-227
-228if __name__ == "__main__":
-229    main(get_args())
+222
+223if __name__ == "__main__":
+224    main(get_args())
   ⁰
 def get_args() -> argparse.Namespace: View Source
-_16def get_args() -> argparse.Namespace:
-_17    parser = argparse.ArgumentParser()
-_18
-_19    parser.add_argument(
-_20        "package",
-_21        type=str,
-_22        default=".",
-_23        nargs="?",
-_24        help=""" The name of the package or project to use,
-_25        assuming it's a subfolder of your current working directory.
-_26        Can also be a full path to the package. If nothing is given,
-_27        the current working directory will be used.""",
-_28    )
-_29
-_30    parser.add_argument(
-_31        "-b", "--build", action="store_true", help=""" Build the package.
+_14def get_args() -> argparse.Namespace:
+_15    parser = argparse.ArgumentParser()
+_16
+_17    parser.add_argument(
+_18        "package",
+_19        type=str,
+_20        default=".",
+_21        nargs="?",
+_22        help=""" The name of the package or project to use,
+_23        assuming it's a subfolder of your current working directory.
+_24        Can also be a full path to the package. If nothing is given,
+_25        the current working directory will be used.""",
+_26    )
+_27
+_28    parser.add_argument(
+_29        "-b", "--build", action="store_true", help=""" Build the package.
 """
-_32    )
-_33
-_34    parser.add_argument(
-_35        "-t",
-_36        "--tag_version",
-_37        action="store_true",
-_38        help=""" Add a git tag corresponding to the version in
+_30    )
+_31
+_32    parser.add_argument(
+_33        "-t",
+_34        "--tag_version",
+_35        action="store_true",
+_36        help=""" Add a git tag corresponding to the version in
 pyproject.toml. """,
-_39    )
-_40
-_41    parser.add_argument(
-_42        "-i",
-_43        "--install",
-_44        action="store_true",
-_45        help=""" Install the package from source. """,
-_46    )
-_47
-_48    parser.add_argument(
-_49        "-iv",
-_50        "--increment_version",
-_51        type=str,
-_52        default=None,
-_53        help=""" Increment version in pyproject.toml.
-_54        Can be one of "major", "minor", or "patch". """,
-_55    )
-_56
-_57    parser.add_argument(
-_58        "-p",
-_59        "--publish",
-_60        action="store_true",
-_61        help=""" Publish package to PyPi.
-_62        Note: You must have configured twine
-_63        and registered a PyPi account/generated an API
-_64        key to use this option.""",
-_65    )
-_66
-_67    parser.add_argument(
-_68        "-rt",
-_69        "--run_tests",
-_70        action="store_true",
-_71        help=""" Run tests for the package. """,
-_72    )
-_73
-_74    parser.add_argument(
-_75        "-gt",
-_76        "--generate_tests",
-_77        action="store_true",
-_78        help=""" Generate tests for the package. """,
-_79    )
-_80
-_81    parser.add_argument(
-_82        "-uc",
-_83        "--update_changelog",
-_84        action="store_true",
-_85        help=""" Update changelog file. """,
-_86    )
-_87
-_88    parser.add_argument(
-_89        "-od",
-_90        "--overwrite_dependencies",
-_91        action="store_true",
-_92        help=""" When building a package, packagelister will be used
-_93        to update the dependencies list in pyproject.toml.
-_94        The default behavior is to append any new dependencies to
-_95        the current list so as not to erase any manually added dependencies
-_96        that packagelister may not detect. If you don't have any manually
-_97        added dependencies and want to remove any dependencies that your
-_98        project no longer uses, pass this flag.""",
-_99    )
-100
-101    parser.add_argument(
-102        "-ca",
-103        "--commit_all",
-104        type=str,
-105        default=None,
-106        help=""" Git stage and commit all tracked files
-107        with this supplied commit message.
-108        If 'build' is passed, all commits will have
-109        message: 'chore: build v{current_version}""",
-110    )
-111
-112    parser.add_argument(
-113        "-s",
-114        "--sync",
-115        action="store_true",
-116        help=""" Pull from github, then push current commit to repo. """,
-117    )
-118
-119    parser.add_argument(
-120        "-dv",
-121        "--dependency_versions",
-122        action="store_true",
-123        help=""" Include version specifiers for dependencies in
-124        pyproject.toml.""",
-125    )
-126
-127    parser.add_argument(
-128        "-up",
-129        "--update",
-130        type=str,
-131        default=None,
-132        help=""" Excpects one argument: "major", "minor", or "patch".
-133        Passing "-up minor" is equivalent to passing the cli string: "-b -
+_37    )
+_38
+_39    parser.add_argument(
+_40        "-i",
+_41        "--install",
+_42        action="store_true",
+_43        help=""" Install the package from source. """,
+_44    )
+_45
+_46    parser.add_argument(
+_47        "-iv",
+_48        "--increment_version",
+_49        type=str,
+_50        default=None,
+_51        help=""" Increment version in pyproject.toml.
+_52        Can be one of "major", "minor", or "patch". """,
+_53    )
+_54
+_55    parser.add_argument(
+_56        "-p",
+_57        "--publish",
+_58        action="store_true",
+_59        help=""" Publish package to PyPi.
+_60        Note: You must have configured twine
+_61        and registered a PyPi account/generated an API
+_62        key to use this option.""",
+_63    )
+_64
+_65    parser.add_argument(
+_66        "-rt",
+_67        "--run_tests",
+_68        action="store_true",
+_69        help=""" Run tests for the package. """,
+_70    )
+_71
+_72    parser.add_argument(
+_73        "-gt",
+_74        "--generate_tests",
+_75        action="store_true",
+_76        help=""" Generate tests for the package. """,
+_77    )
+_78
+_79    parser.add_argument(
+_80        "-uc",
+_81        "--update_changelog",
+_82        action="store_true",
+_83        help=""" Update changelog file. """,
+_84    )
+_85
+_86    parser.add_argument(
+_87        "-od",
+_88        "--overwrite_dependencies",
+_89        action="store_true",
+_90        help=""" When building a package, packagelister will be used
+_91        to update the dependencies list in pyproject.toml.
+_92        The default behavior is to append any new dependencies to
+_93        the current list so as not to erase any manually added dependencies
+_94        that packagelister may not detect. If you don't have any manually
+_95        added dependencies and want to remove any dependencies that your
+_96        project no longer uses, pass this flag.""",
+_97    )
+_98
+_99    parser.add_argument(
+100        "-ca",
+101        "--commit_all",
+102        type=str,
+103        default=None,
+104        help=""" Git stage and commit all tracked files
+105        with this supplied commit message.
+106        If 'build' is passed, all commits will have
+107        message: 'chore: build v{current_version}""",
+108    )
+109
+110    parser.add_argument(
+111        "-s",
+112        "--sync",
+113        action="store_true",
+114        help=""" Pull from github, then push current commit to repo. """,
+115    )
+116
+117    parser.add_argument(
+118        "-dv",
+119        "--dependency_versions",
+120        action="store_true",
+121        help=""" Include version specifiers for dependencies in
+122        pyproject.toml.""",
+123    )
+124
+125    parser.add_argument(
+126        "-up",
+127        "--update",
+128        type=str,
+129        default=None,
+130        help=""" Excpects one argument: "major", "minor", or "patch".
+131        Passing "-up minor" is equivalent to passing the cli string: "-b -
 t -i -iv minor -uc -ca build -s".
-134        To publish the updated package, the -p/--publish switch needs to be
+132        To publish the updated package, the -p/--publish switch needs to be
 added to the cli input.""",
-135    )
+133    )
+134
+135    args = parser.parse_args()
 136
-137    args = parser.parse_args()
+137    args.package = Pathier(args.package).resolve()
 138
-139    args.package = Path(args.package).resolve()
-140
-141    if args.update:
-142        args.build = True
-143        args.tag_version = True
-144        args.install = True
-145        args.increment_version = args.update
-146        args.update_changelog = True
-147        args.commit_all = "build"
-148        args.sync = True
-149
-150    if args.increment_version and args.increment_version not in [
-151        "major",
-152        "minor",
-153        "patch",
-154    ]:
-155        raise ValueError(
-156            f"Invalid option for -iv/--increment_version:
+139    if args.update:
+140        args.build = True
+141        args.tag_version = True
+142        args.install = True
+143        args.increment_version = args.update
+144        args.update_changelog = True
+145        args.commit_all = "build"
+146        args.sync = True
+147
+148    if args.increment_version and args.increment_version not in [
+149        "major",
+150        "minor",
+151        "patch",
+152    ]:
+153        raise ValueError(
+154            f"Invalid option for -iv/--increment_version:
 {args.increment_version}"
-157        )
-158
-159    if args.commit_all == "":
-160        raise ValueError("Commit message for args.commit_all cannot be
+155        )
+156
+157    if args.commit_all == "":
+158        raise ValueError("Commit message for args.commit_all cannot be
 empty.")
-161
-162    return args
+159
+160    return args
   ⁰
 def main(args: argparse.Namespace = None): View Source
-165def main(args: argparse.Namespace = None):
-166    if not args:
-167        args = get_args()
+163def main(args: argparse.Namespace = None):
+164    if not args:
+165        args = get_args()
+166
+167    pyproject_path = args.package / "pyproject.toml"
 168
-169    pyproject_path = args.package / "pyproject.toml"
-170
-171    if not pyproject_path.exists():
-172        raise FileNotFoundError(f"Could not locate pyproject.toml for
+169    if not pyproject_path.exists():
+170        raise FileNotFoundError(f"Could not locate pyproject.toml for
 {args.package}")
-173
-174    if args.generate_tests:
-175        generate_test_files(args.package)
-176
-177    if args.run_tests:
-178        run_tests(args.package)
-179
-180    if args.increment_version:
-181        hassle_utilities.increment_version(pyproject_path,
+171
+172    if args.generate_tests:
+173        generate_test_files(args.package)
+174
+175    if args.run_tests:
+176        run_tests(args.package)
+177
+178    if args.increment_version:
+179        hassle_utilities.increment_version(pyproject_path,
 args.increment_version)
-182
-183    if args.build:
-184        try:
-185            shutil.rmtree(f"{args.package}/dist")
-186        except Exception as e:
-187            pass
-188        os.system(f"black {args.package}")
-189        os.system(f"isort {args.package}")
-190        hassle_utilities.update_dependencies(
-191            pyproject_path, args.overwrite_dependencies
-192        )
-193        hassle_utilities.update_minimum_python_version(pyproject_path)
-194        hassle_utilities.generate_docs(args.package)
-195        os.system(f"py -m build {args.package}")
-196
-197    if args.update_changelog:
-198        hassle_utilities.update_changelog(pyproject_path)
-199        # If we're going to add tag for current version
-200        # commit changelog first
-201        if args.tag_version:
-202            os.chdir(args.package)
-203            os.system("git add CHANGELOG.md")
-204            os.system('git commit CHANGELOG.md -m "chore: update
+180
+181    if args.build:
+182        (args.package / "dist").delete()
+183        os.system(f"black {args.package}")
+184        os.system(f"isort {args.package}")
+185        hassle_utilities.update_dependencies(
+186            pyproject_path, args.overwrite_dependencies
+187        )
+188        hassle_utilities.update_minimum_python_version(pyproject_path)
+189        hassle_utilities.generate_docs(args.package)
+190        os.system(f"py -m build {args.package}")
+191
+192    if args.update_changelog:
+193        hassle_utilities.update_changelog(pyproject_path)
+194        # If we're going to add tag for current version
+195        # commit changelog first
+196        if args.tag_version:
+197            os.chdir(args.package)
+198            os.system("git add CHANGELOG.md")
+199            os.system('git commit CHANGELOG.md -m "chore: update
 changelog"')
-205
-206    if args.commit_all:
-207        os.chdir(args.package)
-208        if args.commit_all == "build":
-209            version = tomlkit.loads(pyproject_path.read_text())["project"]
-["version"]
-210            args.commit_all = f"chore: build v{version}"
-211        os.system("git add .")
-212        os.system(f'git commit -m "{args.commit_all}"')
-213
-214    if args.tag_version:
-215        hassle_utilities.tag_version(args.package)
-216
-217    if args.publish:
-218        os.system(f"twine upload {args.package / 'dist' / '*'}")
-219
-220    if args.install:
-221        os.system(f"pip install {args.package} --no-deps --upgrade --no-
+200
+201    if args.commit_all:
+202        os.chdir(args.package)
+203        if args.commit_all == "build":
+204            version = pyproject_path.loads()["project"]["version"]
+205            args.commit_all = f"chore: build v{version}"
+206        os.system("git add .")
+207        os.system(f'git commit -m "{args.commit_all}"')
+208
+209    if args.tag_version:
+210        hassle_utilities.tag_version(args.package)
+211
+212    if args.publish:
+213        os.system(f"twine upload {args.package / 'dist' / '*'}")
+214
+215    if args.install:
+216        os.system(f"pip install {args.package} --no-deps --upgrade --no-
 cache-dir")
-222
-223    if args.sync:
-224        os.chdir(args.package)
-225        os.system(f"git pull --tags origin main")
-226        os.system(f"git push origin main:main --tags")
+217
+218    if args.sync:
+219        os.chdir(args.package)
+220        os.system(f"git pull --tags origin main")
+221        os.system(f"git push origin main:main --tags")
```

### Comparing `hassle-2.4.0/docs/hassle/hassle_config.html` & `hassle-2.5.0/docs/hassle/hassle_config.html`

 * *Files 0% similar despite different names*

```diff
@@ -69,180 +69,179 @@
 
                 
                         <input id="mod-hassle_config-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 
                         <label class="view-source-button" for="mod-hassle_config-view-source"><span>View Source</span></label>
 
                         <div class="pdoc-code codehilite"><pre><span></span><span id="L-1"><a href="#L-1"><span class="linenos">  1</span></a><span class="kn">import</span> <span class="nn">argparse</span>
-</span><span id="L-2"><a href="#L-2"><span class="linenos">  2</span></a><span class="kn">from</span> <span class="nn">pathlib</span> <span class="kn">import</span> <span class="n">Path</span>
-</span><span id="L-3"><a href="#L-3"><span class="linenos">  3</span></a>
-</span><span id="L-4"><a href="#L-4"><span class="linenos">  4</span></a><span class="kn">import</span> <span class="nn">tomlkit</span>
-</span><span id="L-5"><a href="#L-5"><span class="linenos">  5</span></a>
-</span><span id="L-6"><a href="#L-6"><span class="linenos">  6</span></a><span class="n">root</span> <span class="o">=</span> <span class="n">Path</span><span class="p">(</span><span class="vm">__file__</span><span class="p">)</span><span class="o">.</span><span class="n">parent</span>
+</span><span id="L-2"><a href="#L-2"><span class="linenos">  2</span></a>
+</span><span id="L-3"><a href="#L-3"><span class="linenos">  3</span></a><span class="kn">from</span> <span class="nn">pathier</span> <span class="kn">import</span> <span class="n">Pathier</span>
+</span><span id="L-4"><a href="#L-4"><span class="linenos">  4</span></a>
+</span><span id="L-5"><a href="#L-5"><span class="linenos">  5</span></a><span class="n">root</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="vm">__file__</span><span class="p">)</span><span class="o">.</span><span class="n">parent</span>
+</span><span id="L-6"><a href="#L-6"><span class="linenos">  6</span></a>
 </span><span id="L-7"><a href="#L-7"><span class="linenos">  7</span></a>
-</span><span id="L-8"><a href="#L-8"><span class="linenos">  8</span></a>
-</span><span id="L-9"><a href="#L-9"><span class="linenos">  9</span></a><span class="k">def</span> <span class="nf">get_args</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">:</span>
-</span><span id="L-10"><a href="#L-10"><span class="linenos"> 10</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">argparse</span><span class="o">.</span><span class="n">ArgumentParser</span><span class="p">()</span>
-</span><span id="L-11"><a href="#L-11"><span class="linenos"> 11</span></a>
-</span><span id="L-12"><a href="#L-12"><span class="linenos"> 12</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-13"><a href="#L-13"><span class="linenos"> 13</span></a>        <span class="s2">&quot;-n&quot;</span><span class="p">,</span>
-</span><span id="L-14"><a href="#L-14"><span class="linenos"> 14</span></a>        <span class="s2">&quot;--name&quot;</span><span class="p">,</span>
-</span><span id="L-15"><a href="#L-15"><span class="linenos"> 15</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
-</span><span id="L-16"><a href="#L-16"><span class="linenos"> 16</span></a>        <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
-</span><span id="L-17"><a href="#L-17"><span class="linenos"> 17</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Your name. This will be used to populate the &#39;authors&#39; field of a packages &#39;pyproject.toml&#39;. &quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-18"><a href="#L-18"><span class="linenos"> 18</span></a>    <span class="p">)</span>
-</span><span id="L-19"><a href="#L-19"><span class="linenos"> 19</span></a>
-</span><span id="L-20"><a href="#L-20"><span class="linenos"> 20</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-21"><a href="#L-21"><span class="linenos"> 21</span></a>        <span class="s2">&quot;-e&quot;</span><span class="p">,</span>
-</span><span id="L-22"><a href="#L-22"><span class="linenos"> 22</span></a>        <span class="s2">&quot;--email&quot;</span><span class="p">,</span>
-</span><span id="L-23"><a href="#L-23"><span class="linenos"> 23</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
-</span><span id="L-24"><a href="#L-24"><span class="linenos"> 24</span></a>        <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
-</span><span id="L-25"><a href="#L-25"><span class="linenos"> 25</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Your email. This will be used to populate the &#39;authors&#39; field of a packages &#39;pyproject.toml&#39;. &quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-26"><a href="#L-26"><span class="linenos"> 26</span></a>    <span class="p">)</span>
-</span><span id="L-27"><a href="#L-27"><span class="linenos"> 27</span></a>
-</span><span id="L-28"><a href="#L-28"><span class="linenos"> 28</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-29"><a href="#L-29"><span class="linenos"> 29</span></a>        <span class="s2">&quot;-g&quot;</span><span class="p">,</span>
-</span><span id="L-30"><a href="#L-30"><span class="linenos"> 30</span></a>        <span class="s2">&quot;--github_username&quot;</span><span class="p">,</span>
-</span><span id="L-31"><a href="#L-31"><span class="linenos"> 31</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
-</span><span id="L-32"><a href="#L-32"><span class="linenos"> 32</span></a>        <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
-</span><span id="L-33"><a href="#L-33"><span class="linenos"> 33</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Your github account name. When creating a new package,</span>
-</span><span id="L-34"><a href="#L-34"><span class="linenos"> 34</span></a><span class="s2">        say with the name &#39;mypackage&#39;, the pyproject.toml &#39;Homepage&#39; field</span>
-</span><span id="L-35"><a href="#L-35"><span class="linenos"> 35</span></a><span class="s2">        will be set to &#39;https://github.com/</span><span class="si">{github_username}</span><span class="s2">/mypackage&#39;</span>
-</span><span id="L-36"><a href="#L-36"><span class="linenos"> 36</span></a><span class="s2">        and the &#39;Source code&#39; field will be set to</span>
-</span><span id="L-37"><a href="#L-37"><span class="linenos"> 37</span></a><span class="s2">        &#39;https://github.com/</span><span class="si">{github_username}</span><span class="s2">/mypackage/tree/main/src/mypackage&#39;.&quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-38"><a href="#L-38"><span class="linenos"> 38</span></a>    <span class="p">)</span>
-</span><span id="L-39"><a href="#L-39"><span class="linenos"> 39</span></a>
-</span><span id="L-40"><a href="#L-40"><span class="linenos"> 40</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-41"><a href="#L-41"><span class="linenos"> 41</span></a>        <span class="s2">&quot;-d&quot;</span><span class="p">,</span>
-</span><span id="L-42"><a href="#L-42"><span class="linenos"> 42</span></a>        <span class="s2">&quot;--docs_url&quot;</span><span class="p">,</span>
-</span><span id="L-43"><a href="#L-43"><span class="linenos"> 43</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
-</span><span id="L-44"><a href="#L-44"><span class="linenos"> 44</span></a>        <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
-</span><span id="L-45"><a href="#L-45"><span class="linenos"> 45</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; The template url to be used in your pyproject.toml file</span>
-</span><span id="L-46"><a href="#L-46"><span class="linenos"> 46</span></a><span class="s2">        indicating where your project docs will be hosted.</span>
-</span><span id="L-47"><a href="#L-47"><span class="linenos"> 47</span></a><span class="s2">        Pass the url such that the spot the actual package name will go is</span>
-</span><span id="L-48"><a href="#L-48"><span class="linenos"> 48</span></a><span class="s2">        held by &#39;$name&#39;, e.g. &#39;https://somedocswebsite/user/projects/$name&#39;.</span>
-</span><span id="L-49"><a href="#L-49"><span class="linenos"> 49</span></a><span class="s2">        If &#39;hassle_config.toml&#39; didn&#39;t exist prior to running this tool and nothing</span>
-</span><span id="L-50"><a href="#L-50"><span class="linenos"> 50</span></a><span class="s2">        is given for this arg, it will default to using the package&#39;s github</span>
-</span><span id="L-51"><a href="#L-51"><span class="linenos"> 51</span></a><span class="s2">        url. e.g. for package &#39;mypackage&#39; the url will be </span>
-</span><span id="L-52"><a href="#L-52"><span class="linenos"> 52</span></a><span class="s2">        &#39;https://github.com/</span><span class="si">{your_github_name}</span><span class="s2">/mypackage/tree/main/docs&#39; &quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-53"><a href="#L-53"><span class="linenos"> 53</span></a>    <span class="p">)</span>
-</span><span id="L-54"><a href="#L-54"><span class="linenos"> 54</span></a>
-</span><span id="L-55"><a href="#L-55"><span class="linenos"> 55</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-56"><a href="#L-56"><span class="linenos"> 56</span></a>        <span class="s2">&quot;-t&quot;</span><span class="p">,</span>
-</span><span id="L-57"><a href="#L-57"><span class="linenos"> 57</span></a>        <span class="s2">&quot;--tag_prefix&quot;</span><span class="p">,</span>
-</span><span id="L-58"><a href="#L-58"><span class="linenos"> 58</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
-</span><span id="L-59"><a href="#L-59"><span class="linenos"> 59</span></a>        <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
-</span><span id="L-60"><a href="#L-60"><span class="linenos"> 60</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; The tag prefix to use with git when tagging source code versions.</span>
-</span><span id="L-61"><a href="#L-61"><span class="linenos"> 61</span></a><span class="s2">        e.g. hassle will use the current version in your pyproject.toml file to when </span>
-</span><span id="L-62"><a href="#L-62"><span class="linenos"> 62</span></a><span class="s2">        adding a git tag. If you&#39;ve passed &#39;v&#39; to this arg and the version of your</span>
-</span><span id="L-63"><a href="#L-63"><span class="linenos"> 63</span></a><span class="s2">        hypothetical package is &#39;1.0.1&#39;, it will be tagged as &#39;v1.0.1&#39;.</span>
-</span><span id="L-64"><a href="#L-64"><span class="linenos"> 64</span></a><span class="s2">        If &#39;hassle_config.toml&#39; didn&#39;t exist prior to running this tool and you</span>
-</span><span id="L-65"><a href="#L-65"><span class="linenos"> 65</span></a><span class="s2">        don&#39;t pass anything for this arg, it will default to &#39;&#39;.&quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-66"><a href="#L-66"><span class="linenos"> 66</span></a>    <span class="p">)</span>
-</span><span id="L-67"><a href="#L-67"><span class="linenos"> 67</span></a>
-</span><span id="L-68"><a href="#L-68"><span class="linenos"> 68</span></a>    <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="o">.</span><span class="n">parse_args</span><span class="p">()</span>
-</span><span id="L-69"><a href="#L-69"><span class="linenos"> 69</span></a>
-</span><span id="L-70"><a href="#L-70"><span class="linenos"> 70</span></a>    <span class="k">return</span> <span class="n">args</span>
+</span><span id="L-8"><a href="#L-8"><span class="linenos">  8</span></a><span class="k">def</span> <span class="nf">get_args</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">:</span>
+</span><span id="L-9"><a href="#L-9"><span class="linenos">  9</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">argparse</span><span class="o">.</span><span class="n">ArgumentParser</span><span class="p">()</span>
+</span><span id="L-10"><a href="#L-10"><span class="linenos"> 10</span></a>
+</span><span id="L-11"><a href="#L-11"><span class="linenos"> 11</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-12"><a href="#L-12"><span class="linenos"> 12</span></a>        <span class="s2">&quot;-n&quot;</span><span class="p">,</span>
+</span><span id="L-13"><a href="#L-13"><span class="linenos"> 13</span></a>        <span class="s2">&quot;--name&quot;</span><span class="p">,</span>
+</span><span id="L-14"><a href="#L-14"><span class="linenos"> 14</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
+</span><span id="L-15"><a href="#L-15"><span class="linenos"> 15</span></a>        <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
+</span><span id="L-16"><a href="#L-16"><span class="linenos"> 16</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Your name. This will be used to populate the &#39;authors&#39; field of a packages &#39;pyproject.toml&#39;. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-17"><a href="#L-17"><span class="linenos"> 17</span></a>    <span class="p">)</span>
+</span><span id="L-18"><a href="#L-18"><span class="linenos"> 18</span></a>
+</span><span id="L-19"><a href="#L-19"><span class="linenos"> 19</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-20"><a href="#L-20"><span class="linenos"> 20</span></a>        <span class="s2">&quot;-e&quot;</span><span class="p">,</span>
+</span><span id="L-21"><a href="#L-21"><span class="linenos"> 21</span></a>        <span class="s2">&quot;--email&quot;</span><span class="p">,</span>
+</span><span id="L-22"><a href="#L-22"><span class="linenos"> 22</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
+</span><span id="L-23"><a href="#L-23"><span class="linenos"> 23</span></a>        <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
+</span><span id="L-24"><a href="#L-24"><span class="linenos"> 24</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Your email. This will be used to populate the &#39;authors&#39; field of a packages &#39;pyproject.toml&#39;. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-25"><a href="#L-25"><span class="linenos"> 25</span></a>    <span class="p">)</span>
+</span><span id="L-26"><a href="#L-26"><span class="linenos"> 26</span></a>
+</span><span id="L-27"><a href="#L-27"><span class="linenos"> 27</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-28"><a href="#L-28"><span class="linenos"> 28</span></a>        <span class="s2">&quot;-g&quot;</span><span class="p">,</span>
+</span><span id="L-29"><a href="#L-29"><span class="linenos"> 29</span></a>        <span class="s2">&quot;--github_username&quot;</span><span class="p">,</span>
+</span><span id="L-30"><a href="#L-30"><span class="linenos"> 30</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
+</span><span id="L-31"><a href="#L-31"><span class="linenos"> 31</span></a>        <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
+</span><span id="L-32"><a href="#L-32"><span class="linenos"> 32</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Your github account name. When creating a new package,</span>
+</span><span id="L-33"><a href="#L-33"><span class="linenos"> 33</span></a><span class="s2">        say with the name &#39;mypackage&#39;, the pyproject.toml &#39;Homepage&#39; field</span>
+</span><span id="L-34"><a href="#L-34"><span class="linenos"> 34</span></a><span class="s2">        will be set to &#39;https://github.com/</span><span class="si">{github_username}</span><span class="s2">/mypackage&#39;</span>
+</span><span id="L-35"><a href="#L-35"><span class="linenos"> 35</span></a><span class="s2">        and the &#39;Source code&#39; field will be set to</span>
+</span><span id="L-36"><a href="#L-36"><span class="linenos"> 36</span></a><span class="s2">        &#39;https://github.com/</span><span class="si">{github_username}</span><span class="s2">/mypackage/tree/main/src/mypackage&#39;.&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-37"><a href="#L-37"><span class="linenos"> 37</span></a>    <span class="p">)</span>
+</span><span id="L-38"><a href="#L-38"><span class="linenos"> 38</span></a>
+</span><span id="L-39"><a href="#L-39"><span class="linenos"> 39</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-40"><a href="#L-40"><span class="linenos"> 40</span></a>        <span class="s2">&quot;-d&quot;</span><span class="p">,</span>
+</span><span id="L-41"><a href="#L-41"><span class="linenos"> 41</span></a>        <span class="s2">&quot;--docs_url&quot;</span><span class="p">,</span>
+</span><span id="L-42"><a href="#L-42"><span class="linenos"> 42</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
+</span><span id="L-43"><a href="#L-43"><span class="linenos"> 43</span></a>        <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
+</span><span id="L-44"><a href="#L-44"><span class="linenos"> 44</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; The template url to be used in your pyproject.toml file</span>
+</span><span id="L-45"><a href="#L-45"><span class="linenos"> 45</span></a><span class="s2">        indicating where your project docs will be hosted.</span>
+</span><span id="L-46"><a href="#L-46"><span class="linenos"> 46</span></a><span class="s2">        Pass the url such that the spot the actual package name will go is</span>
+</span><span id="L-47"><a href="#L-47"><span class="linenos"> 47</span></a><span class="s2">        held by &#39;$name&#39;, e.g. &#39;https://somedocswebsite/user/projects/$name&#39;.</span>
+</span><span id="L-48"><a href="#L-48"><span class="linenos"> 48</span></a><span class="s2">        If &#39;hassle_config.toml&#39; didn&#39;t exist prior to running this tool and nothing</span>
+</span><span id="L-49"><a href="#L-49"><span class="linenos"> 49</span></a><span class="s2">        is given for this arg, it will default to using the package&#39;s github</span>
+</span><span id="L-50"><a href="#L-50"><span class="linenos"> 50</span></a><span class="s2">        url. e.g. for package &#39;mypackage&#39; the url will be </span>
+</span><span id="L-51"><a href="#L-51"><span class="linenos"> 51</span></a><span class="s2">        &#39;https://github.com/</span><span class="si">{your_github_name}</span><span class="s2">/mypackage/tree/main/docs&#39; &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-52"><a href="#L-52"><span class="linenos"> 52</span></a>    <span class="p">)</span>
+</span><span id="L-53"><a href="#L-53"><span class="linenos"> 53</span></a>
+</span><span id="L-54"><a href="#L-54"><span class="linenos"> 54</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-55"><a href="#L-55"><span class="linenos"> 55</span></a>        <span class="s2">&quot;-t&quot;</span><span class="p">,</span>
+</span><span id="L-56"><a href="#L-56"><span class="linenos"> 56</span></a>        <span class="s2">&quot;--tag_prefix&quot;</span><span class="p">,</span>
+</span><span id="L-57"><a href="#L-57"><span class="linenos"> 57</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
+</span><span id="L-58"><a href="#L-58"><span class="linenos"> 58</span></a>        <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
+</span><span id="L-59"><a href="#L-59"><span class="linenos"> 59</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; The tag prefix to use with git when tagging source code versions.</span>
+</span><span id="L-60"><a href="#L-60"><span class="linenos"> 60</span></a><span class="s2">        e.g. hassle will use the current version in your pyproject.toml file to when </span>
+</span><span id="L-61"><a href="#L-61"><span class="linenos"> 61</span></a><span class="s2">        adding a git tag. If you&#39;ve passed &#39;v&#39; to this arg and the version of your</span>
+</span><span id="L-62"><a href="#L-62"><span class="linenos"> 62</span></a><span class="s2">        hypothetical package is &#39;1.0.1&#39;, it will be tagged as &#39;v1.0.1&#39;.</span>
+</span><span id="L-63"><a href="#L-63"><span class="linenos"> 63</span></a><span class="s2">        If &#39;hassle_config.toml&#39; didn&#39;t exist prior to running this tool and you</span>
+</span><span id="L-64"><a href="#L-64"><span class="linenos"> 64</span></a><span class="s2">        don&#39;t pass anything for this arg, it will default to &#39;&#39;.&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-65"><a href="#L-65"><span class="linenos"> 65</span></a>    <span class="p">)</span>
+</span><span id="L-66"><a href="#L-66"><span class="linenos"> 66</span></a>
+</span><span id="L-67"><a href="#L-67"><span class="linenos"> 67</span></a>    <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="o">.</span><span class="n">parse_args</span><span class="p">()</span>
+</span><span id="L-68"><a href="#L-68"><span class="linenos"> 68</span></a>
+</span><span id="L-69"><a href="#L-69"><span class="linenos"> 69</span></a>    <span class="k">return</span> <span class="n">args</span>
+</span><span id="L-70"><a href="#L-70"><span class="linenos"> 70</span></a>
 </span><span id="L-71"><a href="#L-71"><span class="linenos"> 71</span></a>
-</span><span id="L-72"><a href="#L-72"><span class="linenos"> 72</span></a>
-</span><span id="L-73"><a href="#L-73"><span class="linenos"> 73</span></a><span class="k">def</span> <span class="nf">config_exists</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
-</span><span id="L-74"><a href="#L-74"><span class="linenos"> 74</span></a>    <span class="sd">&quot;&quot;&quot;Check if hassle_config.toml exists.&quot;&quot;&quot;</span>
-</span><span id="L-75"><a href="#L-75"><span class="linenos"> 75</span></a>    <span class="k">return</span> <span class="p">(</span><span class="n">root</span> <span class="o">/</span> <span class="s2">&quot;hassle_config.toml&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">exists</span><span class="p">()</span>
+</span><span id="L-72"><a href="#L-72"><span class="linenos"> 72</span></a><span class="k">def</span> <span class="nf">config_exists</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
+</span><span id="L-73"><a href="#L-73"><span class="linenos"> 73</span></a>    <span class="sd">&quot;&quot;&quot;Check if hassle_config.toml exists.&quot;&quot;&quot;</span>
+</span><span id="L-74"><a href="#L-74"><span class="linenos"> 74</span></a>    <span class="k">return</span> <span class="p">(</span><span class="n">root</span> <span class="o">/</span> <span class="s2">&quot;hassle_config.toml&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">exists</span><span class="p">()</span>
+</span><span id="L-75"><a href="#L-75"><span class="linenos"> 75</span></a>
 </span><span id="L-76"><a href="#L-76"><span class="linenos"> 76</span></a>
-</span><span id="L-77"><a href="#L-77"><span class="linenos"> 77</span></a>
-</span><span id="L-78"><a href="#L-78"><span class="linenos"> 78</span></a><span class="k">def</span> <span class="nf">load_config</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="nb">dict</span><span class="p">:</span>
-</span><span id="L-79"><a href="#L-79"><span class="linenos"> 79</span></a>    <span class="s2">&quot;Load and return hassle_config contents if it exists.&quot;</span>
-</span><span id="L-80"><a href="#L-80"><span class="linenos"> 80</span></a>    <span class="k">if</span> <span class="n">config_exists</span><span class="p">():</span>
-</span><span id="L-81"><a href="#L-81"><span class="linenos"> 81</span></a>        <span class="k">return</span> <span class="n">tomlkit</span><span class="o">.</span><span class="n">loads</span><span class="p">((</span><span class="n">root</span> <span class="o">/</span> <span class="s2">&quot;hassle_config.toml&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">read_text</span><span class="p">())</span>
-</span><span id="L-82"><a href="#L-82"><span class="linenos"> 82</span></a>    <span class="k">else</span><span class="p">:</span>
-</span><span id="L-83"><a href="#L-83"><span class="linenos"> 83</span></a>        <span class="k">raise</span> <span class="ne">FileNotFoundError</span><span class="p">(</span>
-</span><span id="L-84"><a href="#L-84"><span class="linenos"> 84</span></a>            <span class="sa">f</span><span class="s2">&quot;load_config() could not find </span><span class="si">{</span><span class="n">root</span><span class="o">/</span><span class="s1">&#39;hassle_config.toml&#39;</span><span class="si">}</span><span class="s2">.</span><span class="se">\n</span><span class="s2">Run hassle_config to set it.&quot;</span>
-</span><span id="L-85"><a href="#L-85"><span class="linenos"> 85</span></a>        <span class="p">)</span>
+</span><span id="L-77"><a href="#L-77"><span class="linenos"> 77</span></a><span class="k">def</span> <span class="nf">load_config</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="nb">dict</span><span class="p">:</span>
+</span><span id="L-78"><a href="#L-78"><span class="linenos"> 78</span></a>    <span class="s2">&quot;Load and return hassle_config contents if it exists.&quot;</span>
+</span><span id="L-79"><a href="#L-79"><span class="linenos"> 79</span></a>    <span class="k">if</span> <span class="n">config_exists</span><span class="p">():</span>
+</span><span id="L-80"><a href="#L-80"><span class="linenos"> 80</span></a>        <span class="k">return</span> <span class="p">(</span><span class="n">root</span> <span class="o">/</span> <span class="s2">&quot;hassle_config.toml&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">loads</span><span class="p">()</span>
+</span><span id="L-81"><a href="#L-81"><span class="linenos"> 81</span></a>    <span class="k">else</span><span class="p">:</span>
+</span><span id="L-82"><a href="#L-82"><span class="linenos"> 82</span></a>        <span class="k">raise</span> <span class="ne">FileNotFoundError</span><span class="p">(</span>
+</span><span id="L-83"><a href="#L-83"><span class="linenos"> 83</span></a>            <span class="sa">f</span><span class="s2">&quot;load_config() could not find </span><span class="si">{</span><span class="n">root</span><span class="o">/</span><span class="s1">&#39;hassle_config.toml&#39;</span><span class="si">}</span><span class="s2">.</span><span class="se">\n</span><span class="s2">Run hassle_config to set it.&quot;</span>
+</span><span id="L-84"><a href="#L-84"><span class="linenos"> 84</span></a>        <span class="p">)</span>
+</span><span id="L-85"><a href="#L-85"><span class="linenos"> 85</span></a>
 </span><span id="L-86"><a href="#L-86"><span class="linenos"> 86</span></a>
-</span><span id="L-87"><a href="#L-87"><span class="linenos"> 87</span></a>
-</span><span id="L-88"><a href="#L-88"><span class="linenos"> 88</span></a><span class="k">def</span> <span class="nf">write_config</span><span class="p">(</span><span class="n">config</span><span class="p">:</span> <span class="nb">dict</span><span class="p">):</span>
-</span><span id="L-89"><a href="#L-89"><span class="linenos"> 89</span></a>    <span class="sd">&quot;&quot;&quot;Dump config to &quot;hassle_config.toml.&quot;&quot;&quot;</span>
-</span><span id="L-90"><a href="#L-90"><span class="linenos"> 90</span></a>    <span class="p">(</span><span class="n">root</span> <span class="o">/</span> <span class="s2">&quot;hassle_config.toml&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="n">tomlkit</span><span class="o">.</span><span class="n">dumps</span><span class="p">(</span><span class="n">config</span><span class="p">))</span>
+</span><span id="L-87"><a href="#L-87"><span class="linenos"> 87</span></a><span class="k">def</span> <span class="nf">write_config</span><span class="p">(</span><span class="n">config</span><span class="p">:</span> <span class="nb">dict</span><span class="p">):</span>
+</span><span id="L-88"><a href="#L-88"><span class="linenos"> 88</span></a>    <span class="sd">&quot;&quot;&quot;Dump config to &quot;hassle_config.toml.&quot;&quot;&quot;</span>
+</span><span id="L-89"><a href="#L-89"><span class="linenos"> 89</span></a>    <span class="p">(</span><span class="n">root</span> <span class="o">/</span> <span class="s2">&quot;hassle_config.toml&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">dumps</span><span class="p">(</span><span class="n">config</span><span class="p">)</span>
+</span><span id="L-90"><a href="#L-90"><span class="linenos"> 90</span></a>
 </span><span id="L-91"><a href="#L-91"><span class="linenos"> 91</span></a>
-</span><span id="L-92"><a href="#L-92"><span class="linenos"> 92</span></a>
-</span><span id="L-93"><a href="#L-93"><span class="linenos"> 93</span></a><span class="k">def</span> <span class="nf">warn</span><span class="p">():</span>
-</span><span id="L-94"><a href="#L-94"><span class="linenos"> 94</span></a>    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;hassle_config.toml has not been set.&quot;</span><span class="p">)</span>
-</span><span id="L-95"><a href="#L-95"><span class="linenos"> 95</span></a>    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Run hassle_config to set it.&quot;</span><span class="p">)</span>
-</span><span id="L-96"><a href="#L-96"><span class="linenos"> 96</span></a>    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Run &#39;hassle_config -h&#39; for help.&quot;</span><span class="p">)</span>
+</span><span id="L-92"><a href="#L-92"><span class="linenos"> 92</span></a><span class="k">def</span> <span class="nf">warn</span><span class="p">():</span>
+</span><span id="L-93"><a href="#L-93"><span class="linenos"> 93</span></a>    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;hassle_config.toml has not been set.&quot;</span><span class="p">)</span>
+</span><span id="L-94"><a href="#L-94"><span class="linenos"> 94</span></a>    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Run hassle_config to set it.&quot;</span><span class="p">)</span>
+</span><span id="L-95"><a href="#L-95"><span class="linenos"> 95</span></a>    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Run &#39;hassle_config -h&#39; for help.&quot;</span><span class="p">)</span>
+</span><span id="L-96"><a href="#L-96"><span class="linenos"> 96</span></a>
 </span><span id="L-97"><a href="#L-97"><span class="linenos"> 97</span></a>
-</span><span id="L-98"><a href="#L-98"><span class="linenos"> 98</span></a>
-</span><span id="L-99"><a href="#L-99"><span class="linenos"> 99</span></a><span class="k">def</span> <span class="nf">create_config</span><span class="p">(</span>
-</span><span id="L-100"><a href="#L-100"><span class="linenos">100</span></a>    <span class="n">name</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="L-101"><a href="#L-101"><span class="linenos">101</span></a>    <span class="n">email</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="L-102"><a href="#L-102"><span class="linenos">102</span></a>    <span class="n">github_username</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="L-103"><a href="#L-103"><span class="linenos">103</span></a>    <span class="n">docs_url</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="L-104"><a href="#L-104"><span class="linenos">104</span></a>    <span class="n">tag_prefix</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="L-105"><a href="#L-105"><span class="linenos">105</span></a><span class="p">):</span>
-</span><span id="L-106"><a href="#L-106"><span class="linenos">106</span></a>    <span class="sd">&quot;&quot;&quot;Create hassle_config.toml from given args.&quot;&quot;&quot;</span>
-</span><span id="L-107"><a href="#L-107"><span class="linenos">107</span></a>    <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Manual edits can be made at </span><span class="si">{</span><span class="n">root</span><span class="o">/</span><span class="s1">&#39;hassle_config.toml&#39;</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-108"><a href="#L-108"><span class="linenos">108</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">config_exists</span><span class="p">():</span>
-</span><span id="L-109"><a href="#L-109"><span class="linenos">109</span></a>        <span class="n">config</span> <span class="o">=</span> <span class="p">{}</span>
-</span><span id="L-110"><a href="#L-110"><span class="linenos">110</span></a>        <span class="k">if</span> <span class="n">name</span> <span class="ow">and</span> <span class="n">email</span><span class="p">:</span>
-</span><span id="L-111"><a href="#L-111"><span class="linenos">111</span></a>            <span class="n">config</span><span class="p">[</span><span class="s2">&quot;authors&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="p">[{</span><span class="s2">&quot;name&quot;</span><span class="p">:</span> <span class="n">name</span><span class="p">,</span> <span class="s2">&quot;email&quot;</span><span class="p">:</span> <span class="n">email</span><span class="p">}]</span>
-</span><span id="L-112"><a href="#L-112"><span class="linenos">112</span></a>        <span class="k">elif</span> <span class="n">name</span><span class="p">:</span>
-</span><span id="L-113"><a href="#L-113"><span class="linenos">113</span></a>            <span class="n">config</span><span class="p">[</span><span class="s2">&quot;authors&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="p">[{</span><span class="s2">&quot;name&quot;</span><span class="p">:</span> <span class="n">name</span><span class="p">}]</span>
-</span><span id="L-114"><a href="#L-114"><span class="linenos">114</span></a>        <span class="k">elif</span> <span class="n">email</span><span class="p">:</span>
-</span><span id="L-115"><a href="#L-115"><span class="linenos">115</span></a>            <span class="n">config</span><span class="p">[</span><span class="s2">&quot;authors&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="p">[{</span><span class="s2">&quot;email&quot;</span><span class="p">:</span> <span class="n">email</span><span class="p">}]</span>
-</span><span id="L-116"><a href="#L-116"><span class="linenos">116</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="L-117"><a href="#L-117"><span class="linenos">117</span></a>            <span class="c1"># In case anything upstream would fail if nothing is present for &#39;authors&#39;</span>
-</span><span id="L-118"><a href="#L-118"><span class="linenos">118</span></a>            <span class="n">config</span><span class="p">[</span><span class="s2">&quot;authors&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="p">[{</span><span class="s2">&quot;name&quot;</span><span class="p">:</span> <span class="s2">&quot;&quot;</span><span class="p">,</span> <span class="s2">&quot;email&quot;</span><span class="p">:</span> <span class="s2">&quot;&quot;</span><span class="p">}]</span>
-</span><span id="L-119"><a href="#L-119"><span class="linenos">119</span></a>        <span class="n">config</span><span class="p">[</span><span class="s2">&quot;project_urls&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="p">{</span>
-</span><span id="L-120"><a href="#L-120"><span class="linenos">120</span></a>            <span class="s2">&quot;Homepage&quot;</span><span class="p">:</span> <span class="s2">&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-121"><a href="#L-121"><span class="linenos">121</span></a>            <span class="s2">&quot;Documentation&quot;</span><span class="p">:</span> <span class="s2">&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-122"><a href="#L-122"><span class="linenos">122</span></a>            <span class="s2">&quot;Source code&quot;</span><span class="p">:</span> <span class="s2">&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-123"><a href="#L-123"><span class="linenos">123</span></a>        <span class="p">}</span>
-</span><span id="L-124"><a href="#L-124"><span class="linenos">124</span></a>        <span class="n">config</span><span class="p">[</span><span class="s2">&quot;git&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="p">{}</span>
-</span><span id="L-125"><a href="#L-125"><span class="linenos">125</span></a>    <span class="k">else</span><span class="p">:</span>
-</span><span id="L-126"><a href="#L-126"><span class="linenos">126</span></a>        <span class="n">config</span> <span class="o">=</span> <span class="n">load_config</span><span class="p">()</span>
-</span><span id="L-127"><a href="#L-127"><span class="linenos">127</span></a>        <span class="k">if</span> <span class="n">name</span> <span class="ow">and</span> <span class="n">email</span><span class="p">:</span>
-</span><span id="L-128"><a href="#L-128"><span class="linenos">128</span></a>            <span class="n">config</span><span class="p">[</span><span class="s2">&quot;authors&quot;</span><span class="p">]</span><span class="o">.</span><span class="n">append</span><span class="p">({</span><span class="s2">&quot;name&quot;</span><span class="p">:</span> <span class="n">name</span><span class="p">,</span> <span class="s2">&quot;email&quot;</span><span class="p">:</span> <span class="n">email</span><span class="p">})</span>
-</span><span id="L-129"><a href="#L-129"><span class="linenos">129</span></a>        <span class="k">elif</span> <span class="n">name</span><span class="p">:</span>
-</span><span id="L-130"><a href="#L-130"><span class="linenos">130</span></a>            <span class="n">config</span><span class="p">[</span><span class="s2">&quot;authors&quot;</span><span class="p">]</span><span class="o">.</span><span class="n">append</span><span class="p">({</span><span class="s2">&quot;name&quot;</span><span class="p">:</span> <span class="n">name</span><span class="p">})</span>
-</span><span id="L-131"><a href="#L-131"><span class="linenos">131</span></a>        <span class="k">elif</span> <span class="n">email</span><span class="p">:</span>
-</span><span id="L-132"><a href="#L-132"><span class="linenos">132</span></a>            <span class="n">config</span><span class="p">[</span><span class="s2">&quot;authors&quot;</span><span class="p">]</span><span class="o">.</span><span class="n">append</span><span class="p">({</span><span class="s2">&quot;email&quot;</span><span class="p">:</span> <span class="n">email</span><span class="p">})</span>
-</span><span id="L-133"><a href="#L-133"><span class="linenos">133</span></a>
-</span><span id="L-134"><a href="#L-134"><span class="linenos">134</span></a>    <span class="k">if</span> <span class="n">github_username</span><span class="p">:</span>
-</span><span id="L-135"><a href="#L-135"><span class="linenos">135</span></a>        <span class="n">config</span><span class="p">[</span><span class="s2">&quot;project_urls&quot;</span><span class="p">][</span>
-</span><span id="L-136"><a href="#L-136"><span class="linenos">136</span></a>            <span class="s2">&quot;Homepage&quot;</span>
-</span><span id="L-137"><a href="#L-137"><span class="linenos">137</span></a>        <span class="p">]</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;https://github.com/</span><span class="si">{</span><span class="n">github_username</span><span class="si">}</span><span class="s2">/$name&quot;</span>
-</span><span id="L-138"><a href="#L-138"><span class="linenos">138</span></a>        <span class="n">config</span><span class="p">[</span><span class="s2">&quot;project_urls&quot;</span><span class="p">][</span>
-</span><span id="L-139"><a href="#L-139"><span class="linenos">139</span></a>            <span class="s2">&quot;Source code&quot;</span>
-</span><span id="L-140"><a href="#L-140"><span class="linenos">140</span></a>        <span class="p">]</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">config</span><span class="p">[</span><span class="s1">&#39;project_urls&#39;</span><span class="p">][</span><span class="s1">&#39;Homepage&#39;</span><span class="p">]</span><span class="si">}</span><span class="s2">/tree/main/src/$name&quot;</span>
-</span><span id="L-141"><a href="#L-141"><span class="linenos">141</span></a>
-</span><span id="L-142"><a href="#L-142"><span class="linenos">142</span></a>    <span class="k">if</span> <span class="n">docs_url</span><span class="p">:</span>
-</span><span id="L-143"><a href="#L-143"><span class="linenos">143</span></a>        <span class="n">config</span><span class="p">[</span><span class="s2">&quot;project_urls&quot;</span><span class="p">][</span><span class="s2">&quot;Documentation&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">docs_url</span>
-</span><span id="L-144"><a href="#L-144"><span class="linenos">144</span></a>    <span class="k">elif</span> <span class="n">github_username</span> <span class="ow">and</span> <span class="n">config</span><span class="p">[</span><span class="s2">&quot;project_urls&quot;</span><span class="p">][</span><span class="s2">&quot;Documentation&quot;</span><span class="p">]</span> <span class="o">==</span> <span class="s2">&quot;&quot;</span><span class="p">:</span>
-</span><span id="L-145"><a href="#L-145"><span class="linenos">145</span></a>        <span class="n">config</span><span class="p">[</span><span class="s2">&quot;project_urls&quot;</span><span class="p">][</span>
-</span><span id="L-146"><a href="#L-146"><span class="linenos">146</span></a>            <span class="s2">&quot;Documentation&quot;</span>
-</span><span id="L-147"><a href="#L-147"><span class="linenos">147</span></a>        <span class="p">]</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;https://github.com/</span><span class="si">{</span><span class="n">github_username</span><span class="si">}</span><span class="s2">/$name/tree/main/docs&quot;</span>
-</span><span id="L-148"><a href="#L-148"><span class="linenos">148</span></a>
-</span><span id="L-149"><a href="#L-149"><span class="linenos">149</span></a>    <span class="k">if</span> <span class="n">tag_prefix</span><span class="p">:</span>
-</span><span id="L-150"><a href="#L-150"><span class="linenos">150</span></a>        <span class="n">config</span><span class="p">[</span><span class="s2">&quot;git&quot;</span><span class="p">][</span><span class="s2">&quot;tag_prefix&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">tag_prefix</span>
-</span><span id="L-151"><a href="#L-151"><span class="linenos">151</span></a>    <span class="k">elif</span> <span class="ow">not</span> <span class="n">config_exists</span><span class="p">()</span> <span class="ow">and</span> <span class="ow">not</span> <span class="n">tag_prefix</span><span class="p">:</span>
-</span><span id="L-152"><a href="#L-152"><span class="linenos">152</span></a>        <span class="n">config</span><span class="p">[</span><span class="s2">&quot;git&quot;</span><span class="p">][</span><span class="s2">&quot;tag_prefix&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
-</span><span id="L-153"><a href="#L-153"><span class="linenos">153</span></a>
-</span><span id="L-154"><a href="#L-154"><span class="linenos">154</span></a>    <span class="k">if</span> <span class="n">config</span><span class="p">:</span>
-</span><span id="L-155"><a href="#L-155"><span class="linenos">155</span></a>        <span class="n">write_config</span><span class="p">(</span><span class="n">config</span><span class="p">)</span>
+</span><span id="L-98"><a href="#L-98"><span class="linenos"> 98</span></a><span class="k">def</span> <span class="nf">create_config</span><span class="p">(</span>
+</span><span id="L-99"><a href="#L-99"><span class="linenos"> 99</span></a>    <span class="n">name</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="L-100"><a href="#L-100"><span class="linenos">100</span></a>    <span class="n">email</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="L-101"><a href="#L-101"><span class="linenos">101</span></a>    <span class="n">github_username</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="L-102"><a href="#L-102"><span class="linenos">102</span></a>    <span class="n">docs_url</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="L-103"><a href="#L-103"><span class="linenos">103</span></a>    <span class="n">tag_prefix</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="L-104"><a href="#L-104"><span class="linenos">104</span></a><span class="p">):</span>
+</span><span id="L-105"><a href="#L-105"><span class="linenos">105</span></a>    <span class="sd">&quot;&quot;&quot;Create hassle_config.toml from given args.&quot;&quot;&quot;</span>
+</span><span id="L-106"><a href="#L-106"><span class="linenos">106</span></a>    <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Manual edits can be made at </span><span class="si">{</span><span class="n">root</span><span class="o">/</span><span class="s1">&#39;hassle_config.toml&#39;</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-107"><a href="#L-107"><span class="linenos">107</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">config_exists</span><span class="p">():</span>
+</span><span id="L-108"><a href="#L-108"><span class="linenos">108</span></a>        <span class="n">config</span> <span class="o">=</span> <span class="p">{}</span>
+</span><span id="L-109"><a href="#L-109"><span class="linenos">109</span></a>        <span class="k">if</span> <span class="n">name</span> <span class="ow">and</span> <span class="n">email</span><span class="p">:</span>
+</span><span id="L-110"><a href="#L-110"><span class="linenos">110</span></a>            <span class="n">config</span><span class="p">[</span><span class="s2">&quot;authors&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="p">[{</span><span class="s2">&quot;name&quot;</span><span class="p">:</span> <span class="n">name</span><span class="p">,</span> <span class="s2">&quot;email&quot;</span><span class="p">:</span> <span class="n">email</span><span class="p">}]</span>
+</span><span id="L-111"><a href="#L-111"><span class="linenos">111</span></a>        <span class="k">elif</span> <span class="n">name</span><span class="p">:</span>
+</span><span id="L-112"><a href="#L-112"><span class="linenos">112</span></a>            <span class="n">config</span><span class="p">[</span><span class="s2">&quot;authors&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="p">[{</span><span class="s2">&quot;name&quot;</span><span class="p">:</span> <span class="n">name</span><span class="p">}]</span>
+</span><span id="L-113"><a href="#L-113"><span class="linenos">113</span></a>        <span class="k">elif</span> <span class="n">email</span><span class="p">:</span>
+</span><span id="L-114"><a href="#L-114"><span class="linenos">114</span></a>            <span class="n">config</span><span class="p">[</span><span class="s2">&quot;authors&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="p">[{</span><span class="s2">&quot;email&quot;</span><span class="p">:</span> <span class="n">email</span><span class="p">}]</span>
+</span><span id="L-115"><a href="#L-115"><span class="linenos">115</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="L-116"><a href="#L-116"><span class="linenos">116</span></a>            <span class="c1"># In case anything upstream would fail if nothing is present for &#39;authors&#39;</span>
+</span><span id="L-117"><a href="#L-117"><span class="linenos">117</span></a>            <span class="n">config</span><span class="p">[</span><span class="s2">&quot;authors&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="p">[{</span><span class="s2">&quot;name&quot;</span><span class="p">:</span> <span class="s2">&quot;&quot;</span><span class="p">,</span> <span class="s2">&quot;email&quot;</span><span class="p">:</span> <span class="s2">&quot;&quot;</span><span class="p">}]</span>
+</span><span id="L-118"><a href="#L-118"><span class="linenos">118</span></a>        <span class="n">config</span><span class="p">[</span><span class="s2">&quot;project_urls&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="p">{</span>
+</span><span id="L-119"><a href="#L-119"><span class="linenos">119</span></a>            <span class="s2">&quot;Homepage&quot;</span><span class="p">:</span> <span class="s2">&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-120"><a href="#L-120"><span class="linenos">120</span></a>            <span class="s2">&quot;Documentation&quot;</span><span class="p">:</span> <span class="s2">&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-121"><a href="#L-121"><span class="linenos">121</span></a>            <span class="s2">&quot;Source code&quot;</span><span class="p">:</span> <span class="s2">&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-122"><a href="#L-122"><span class="linenos">122</span></a>        <span class="p">}</span>
+</span><span id="L-123"><a href="#L-123"><span class="linenos">123</span></a>        <span class="n">config</span><span class="p">[</span><span class="s2">&quot;git&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="p">{}</span>
+</span><span id="L-124"><a href="#L-124"><span class="linenos">124</span></a>    <span class="k">else</span><span class="p">:</span>
+</span><span id="L-125"><a href="#L-125"><span class="linenos">125</span></a>        <span class="n">config</span> <span class="o">=</span> <span class="n">load_config</span><span class="p">()</span>
+</span><span id="L-126"><a href="#L-126"><span class="linenos">126</span></a>        <span class="k">if</span> <span class="n">name</span> <span class="ow">and</span> <span class="n">email</span><span class="p">:</span>
+</span><span id="L-127"><a href="#L-127"><span class="linenos">127</span></a>            <span class="n">config</span><span class="p">[</span><span class="s2">&quot;authors&quot;</span><span class="p">]</span><span class="o">.</span><span class="n">append</span><span class="p">({</span><span class="s2">&quot;name&quot;</span><span class="p">:</span> <span class="n">name</span><span class="p">,</span> <span class="s2">&quot;email&quot;</span><span class="p">:</span> <span class="n">email</span><span class="p">})</span>
+</span><span id="L-128"><a href="#L-128"><span class="linenos">128</span></a>        <span class="k">elif</span> <span class="n">name</span><span class="p">:</span>
+</span><span id="L-129"><a href="#L-129"><span class="linenos">129</span></a>            <span class="n">config</span><span class="p">[</span><span class="s2">&quot;authors&quot;</span><span class="p">]</span><span class="o">.</span><span class="n">append</span><span class="p">({</span><span class="s2">&quot;name&quot;</span><span class="p">:</span> <span class="n">name</span><span class="p">})</span>
+</span><span id="L-130"><a href="#L-130"><span class="linenos">130</span></a>        <span class="k">elif</span> <span class="n">email</span><span class="p">:</span>
+</span><span id="L-131"><a href="#L-131"><span class="linenos">131</span></a>            <span class="n">config</span><span class="p">[</span><span class="s2">&quot;authors&quot;</span><span class="p">]</span><span class="o">.</span><span class="n">append</span><span class="p">({</span><span class="s2">&quot;email&quot;</span><span class="p">:</span> <span class="n">email</span><span class="p">})</span>
+</span><span id="L-132"><a href="#L-132"><span class="linenos">132</span></a>
+</span><span id="L-133"><a href="#L-133"><span class="linenos">133</span></a>    <span class="k">if</span> <span class="n">github_username</span><span class="p">:</span>
+</span><span id="L-134"><a href="#L-134"><span class="linenos">134</span></a>        <span class="n">config</span><span class="p">[</span><span class="s2">&quot;project_urls&quot;</span><span class="p">][</span>
+</span><span id="L-135"><a href="#L-135"><span class="linenos">135</span></a>            <span class="s2">&quot;Homepage&quot;</span>
+</span><span id="L-136"><a href="#L-136"><span class="linenos">136</span></a>        <span class="p">]</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;https://github.com/</span><span class="si">{</span><span class="n">github_username</span><span class="si">}</span><span class="s2">/$name&quot;</span>
+</span><span id="L-137"><a href="#L-137"><span class="linenos">137</span></a>        <span class="n">config</span><span class="p">[</span><span class="s2">&quot;project_urls&quot;</span><span class="p">][</span>
+</span><span id="L-138"><a href="#L-138"><span class="linenos">138</span></a>            <span class="s2">&quot;Source code&quot;</span>
+</span><span id="L-139"><a href="#L-139"><span class="linenos">139</span></a>        <span class="p">]</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">config</span><span class="p">[</span><span class="s1">&#39;project_urls&#39;</span><span class="p">][</span><span class="s1">&#39;Homepage&#39;</span><span class="p">]</span><span class="si">}</span><span class="s2">/tree/main/src/$name&quot;</span>
+</span><span id="L-140"><a href="#L-140"><span class="linenos">140</span></a>
+</span><span id="L-141"><a href="#L-141"><span class="linenos">141</span></a>    <span class="k">if</span> <span class="n">docs_url</span><span class="p">:</span>
+</span><span id="L-142"><a href="#L-142"><span class="linenos">142</span></a>        <span class="n">config</span><span class="p">[</span><span class="s2">&quot;project_urls&quot;</span><span class="p">][</span><span class="s2">&quot;Documentation&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">docs_url</span>
+</span><span id="L-143"><a href="#L-143"><span class="linenos">143</span></a>    <span class="k">elif</span> <span class="n">github_username</span> <span class="ow">and</span> <span class="n">config</span><span class="p">[</span><span class="s2">&quot;project_urls&quot;</span><span class="p">][</span><span class="s2">&quot;Documentation&quot;</span><span class="p">]</span> <span class="o">==</span> <span class="s2">&quot;&quot;</span><span class="p">:</span>
+</span><span id="L-144"><a href="#L-144"><span class="linenos">144</span></a>        <span class="n">config</span><span class="p">[</span><span class="s2">&quot;project_urls&quot;</span><span class="p">][</span>
+</span><span id="L-145"><a href="#L-145"><span class="linenos">145</span></a>            <span class="s2">&quot;Documentation&quot;</span>
+</span><span id="L-146"><a href="#L-146"><span class="linenos">146</span></a>        <span class="p">]</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;https://github.com/</span><span class="si">{</span><span class="n">github_username</span><span class="si">}</span><span class="s2">/$name/tree/main/docs&quot;</span>
+</span><span id="L-147"><a href="#L-147"><span class="linenos">147</span></a>
+</span><span id="L-148"><a href="#L-148"><span class="linenos">148</span></a>    <span class="k">if</span> <span class="n">tag_prefix</span><span class="p">:</span>
+</span><span id="L-149"><a href="#L-149"><span class="linenos">149</span></a>        <span class="n">config</span><span class="p">[</span><span class="s2">&quot;git&quot;</span><span class="p">][</span><span class="s2">&quot;tag_prefix&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">tag_prefix</span>
+</span><span id="L-150"><a href="#L-150"><span class="linenos">150</span></a>    <span class="k">elif</span> <span class="ow">not</span> <span class="n">config_exists</span><span class="p">()</span> <span class="ow">and</span> <span class="ow">not</span> <span class="n">tag_prefix</span><span class="p">:</span>
+</span><span id="L-151"><a href="#L-151"><span class="linenos">151</span></a>        <span class="n">config</span><span class="p">[</span><span class="s2">&quot;git&quot;</span><span class="p">][</span><span class="s2">&quot;tag_prefix&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
+</span><span id="L-152"><a href="#L-152"><span class="linenos">152</span></a>
+</span><span id="L-153"><a href="#L-153"><span class="linenos">153</span></a>    <span class="k">if</span> <span class="n">config</span><span class="p">:</span>
+</span><span id="L-154"><a href="#L-154"><span class="linenos">154</span></a>        <span class="n">write_config</span><span class="p">(</span><span class="n">config</span><span class="p">)</span>
+</span><span id="L-155"><a href="#L-155"><span class="linenos">155</span></a>
 </span><span id="L-156"><a href="#L-156"><span class="linenos">156</span></a>
-</span><span id="L-157"><a href="#L-157"><span class="linenos">157</span></a>
-</span><span id="L-158"><a href="#L-158"><span class="linenos">158</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
-</span><span id="L-159"><a href="#L-159"><span class="linenos">159</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="p">:</span>
-</span><span id="L-160"><a href="#L-160"><span class="linenos">160</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
-</span><span id="L-161"><a href="#L-161"><span class="linenos">161</span></a>    <span class="n">create_config</span><span class="p">(</span>
-</span><span id="L-162"><a href="#L-162"><span class="linenos">162</span></a>        <span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">email</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">github_username</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">docs_url</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">tag_prefix</span>
-</span><span id="L-163"><a href="#L-163"><span class="linenos">163</span></a>    <span class="p">)</span>
+</span><span id="L-157"><a href="#L-157"><span class="linenos">157</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
+</span><span id="L-158"><a href="#L-158"><span class="linenos">158</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="p">:</span>
+</span><span id="L-159"><a href="#L-159"><span class="linenos">159</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
+</span><span id="L-160"><a href="#L-160"><span class="linenos">160</span></a>    <span class="n">create_config</span><span class="p">(</span>
+</span><span id="L-161"><a href="#L-161"><span class="linenos">161</span></a>        <span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">email</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">github_username</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">docs_url</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">tag_prefix</span>
+</span><span id="L-162"><a href="#L-162"><span class="linenos">162</span></a>    <span class="p">)</span>
+</span><span id="L-163"><a href="#L-163"><span class="linenos">163</span></a>
 </span><span id="L-164"><a href="#L-164"><span class="linenos">164</span></a>
-</span><span id="L-165"><a href="#L-165"><span class="linenos">165</span></a>
-</span><span id="L-166"><a href="#L-166"><span class="linenos">166</span></a><span class="k">if</span> <span class="vm">__name__</span> <span class="o">==</span> <span class="s2">&quot;__main__&quot;</span><span class="p">:</span>
-</span><span id="L-167"><a href="#L-167"><span class="linenos">167</span></a>    <span class="n">main</span><span class="p">(</span><span class="n">get_args</span><span class="p">())</span>
+</span><span id="L-165"><a href="#L-165"><span class="linenos">165</span></a><span class="k">if</span> <span class="vm">__name__</span> <span class="o">==</span> <span class="s2">&quot;__main__&quot;</span><span class="p">:</span>
+</span><span id="L-166"><a href="#L-166"><span class="linenos">166</span></a>    <span class="n">main</span><span class="p">(</span><span class="n">get_args</span><span class="p">())</span>
 </span></pre></div>
 
 
             </section>
                 <section id="get_args">
                             <input id="get_args-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
@@ -250,76 +249,76 @@
         <span class="def">def</span>
         <span class="name">get_args</span><span class="signature pdoc-code condensed">(<span class="return-annotation">) -> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span>:</span></span>
 
                 <label class="view-source-button" for="get_args-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#get_args"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="get_args-10"><a href="#get_args-10"><span class="linenos">10</span></a><span class="k">def</span> <span class="nf">get_args</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">:</span>
-</span><span id="get_args-11"><a href="#get_args-11"><span class="linenos">11</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">argparse</span><span class="o">.</span><span class="n">ArgumentParser</span><span class="p">()</span>
-</span><span id="get_args-12"><a href="#get_args-12"><span class="linenos">12</span></a>
-</span><span id="get_args-13"><a href="#get_args-13"><span class="linenos">13</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="get_args-14"><a href="#get_args-14"><span class="linenos">14</span></a>        <span class="s2">&quot;-n&quot;</span><span class="p">,</span>
-</span><span id="get_args-15"><a href="#get_args-15"><span class="linenos">15</span></a>        <span class="s2">&quot;--name&quot;</span><span class="p">,</span>
-</span><span id="get_args-16"><a href="#get_args-16"><span class="linenos">16</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
-</span><span id="get_args-17"><a href="#get_args-17"><span class="linenos">17</span></a>        <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
-</span><span id="get_args-18"><a href="#get_args-18"><span class="linenos">18</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Your name. This will be used to populate the &#39;authors&#39; field of a packages &#39;pyproject.toml&#39;. &quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="get_args-19"><a href="#get_args-19"><span class="linenos">19</span></a>    <span class="p">)</span>
-</span><span id="get_args-20"><a href="#get_args-20"><span class="linenos">20</span></a>
-</span><span id="get_args-21"><a href="#get_args-21"><span class="linenos">21</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="get_args-22"><a href="#get_args-22"><span class="linenos">22</span></a>        <span class="s2">&quot;-e&quot;</span><span class="p">,</span>
-</span><span id="get_args-23"><a href="#get_args-23"><span class="linenos">23</span></a>        <span class="s2">&quot;--email&quot;</span><span class="p">,</span>
-</span><span id="get_args-24"><a href="#get_args-24"><span class="linenos">24</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
-</span><span id="get_args-25"><a href="#get_args-25"><span class="linenos">25</span></a>        <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
-</span><span id="get_args-26"><a href="#get_args-26"><span class="linenos">26</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Your email. This will be used to populate the &#39;authors&#39; field of a packages &#39;pyproject.toml&#39;. &quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="get_args-27"><a href="#get_args-27"><span class="linenos">27</span></a>    <span class="p">)</span>
-</span><span id="get_args-28"><a href="#get_args-28"><span class="linenos">28</span></a>
-</span><span id="get_args-29"><a href="#get_args-29"><span class="linenos">29</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="get_args-30"><a href="#get_args-30"><span class="linenos">30</span></a>        <span class="s2">&quot;-g&quot;</span><span class="p">,</span>
-</span><span id="get_args-31"><a href="#get_args-31"><span class="linenos">31</span></a>        <span class="s2">&quot;--github_username&quot;</span><span class="p">,</span>
-</span><span id="get_args-32"><a href="#get_args-32"><span class="linenos">32</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
-</span><span id="get_args-33"><a href="#get_args-33"><span class="linenos">33</span></a>        <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
-</span><span id="get_args-34"><a href="#get_args-34"><span class="linenos">34</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Your github account name. When creating a new package,</span>
-</span><span id="get_args-35"><a href="#get_args-35"><span class="linenos">35</span></a><span class="s2">        say with the name &#39;mypackage&#39;, the pyproject.toml &#39;Homepage&#39; field</span>
-</span><span id="get_args-36"><a href="#get_args-36"><span class="linenos">36</span></a><span class="s2">        will be set to &#39;https://github.com/</span><span class="si">{github_username}</span><span class="s2">/mypackage&#39;</span>
-</span><span id="get_args-37"><a href="#get_args-37"><span class="linenos">37</span></a><span class="s2">        and the &#39;Source code&#39; field will be set to</span>
-</span><span id="get_args-38"><a href="#get_args-38"><span class="linenos">38</span></a><span class="s2">        &#39;https://github.com/</span><span class="si">{github_username}</span><span class="s2">/mypackage/tree/main/src/mypackage&#39;.&quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="get_args-39"><a href="#get_args-39"><span class="linenos">39</span></a>    <span class="p">)</span>
-</span><span id="get_args-40"><a href="#get_args-40"><span class="linenos">40</span></a>
-</span><span id="get_args-41"><a href="#get_args-41"><span class="linenos">41</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="get_args-42"><a href="#get_args-42"><span class="linenos">42</span></a>        <span class="s2">&quot;-d&quot;</span><span class="p">,</span>
-</span><span id="get_args-43"><a href="#get_args-43"><span class="linenos">43</span></a>        <span class="s2">&quot;--docs_url&quot;</span><span class="p">,</span>
-</span><span id="get_args-44"><a href="#get_args-44"><span class="linenos">44</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
-</span><span id="get_args-45"><a href="#get_args-45"><span class="linenos">45</span></a>        <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
-</span><span id="get_args-46"><a href="#get_args-46"><span class="linenos">46</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; The template url to be used in your pyproject.toml file</span>
-</span><span id="get_args-47"><a href="#get_args-47"><span class="linenos">47</span></a><span class="s2">        indicating where your project docs will be hosted.</span>
-</span><span id="get_args-48"><a href="#get_args-48"><span class="linenos">48</span></a><span class="s2">        Pass the url such that the spot the actual package name will go is</span>
-</span><span id="get_args-49"><a href="#get_args-49"><span class="linenos">49</span></a><span class="s2">        held by &#39;$name&#39;, e.g. &#39;https://somedocswebsite/user/projects/$name&#39;.</span>
-</span><span id="get_args-50"><a href="#get_args-50"><span class="linenos">50</span></a><span class="s2">        If &#39;hassle_config.toml&#39; didn&#39;t exist prior to running this tool and nothing</span>
-</span><span id="get_args-51"><a href="#get_args-51"><span class="linenos">51</span></a><span class="s2">        is given for this arg, it will default to using the package&#39;s github</span>
-</span><span id="get_args-52"><a href="#get_args-52"><span class="linenos">52</span></a><span class="s2">        url. e.g. for package &#39;mypackage&#39; the url will be </span>
-</span><span id="get_args-53"><a href="#get_args-53"><span class="linenos">53</span></a><span class="s2">        &#39;https://github.com/</span><span class="si">{your_github_name}</span><span class="s2">/mypackage/tree/main/docs&#39; &quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="get_args-54"><a href="#get_args-54"><span class="linenos">54</span></a>    <span class="p">)</span>
-</span><span id="get_args-55"><a href="#get_args-55"><span class="linenos">55</span></a>
-</span><span id="get_args-56"><a href="#get_args-56"><span class="linenos">56</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="get_args-57"><a href="#get_args-57"><span class="linenos">57</span></a>        <span class="s2">&quot;-t&quot;</span><span class="p">,</span>
-</span><span id="get_args-58"><a href="#get_args-58"><span class="linenos">58</span></a>        <span class="s2">&quot;--tag_prefix&quot;</span><span class="p">,</span>
-</span><span id="get_args-59"><a href="#get_args-59"><span class="linenos">59</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
-</span><span id="get_args-60"><a href="#get_args-60"><span class="linenos">60</span></a>        <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
-</span><span id="get_args-61"><a href="#get_args-61"><span class="linenos">61</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; The tag prefix to use with git when tagging source code versions.</span>
-</span><span id="get_args-62"><a href="#get_args-62"><span class="linenos">62</span></a><span class="s2">        e.g. hassle will use the current version in your pyproject.toml file to when </span>
-</span><span id="get_args-63"><a href="#get_args-63"><span class="linenos">63</span></a><span class="s2">        adding a git tag. If you&#39;ve passed &#39;v&#39; to this arg and the version of your</span>
-</span><span id="get_args-64"><a href="#get_args-64"><span class="linenos">64</span></a><span class="s2">        hypothetical package is &#39;1.0.1&#39;, it will be tagged as &#39;v1.0.1&#39;.</span>
-</span><span id="get_args-65"><a href="#get_args-65"><span class="linenos">65</span></a><span class="s2">        If &#39;hassle_config.toml&#39; didn&#39;t exist prior to running this tool and you</span>
-</span><span id="get_args-66"><a href="#get_args-66"><span class="linenos">66</span></a><span class="s2">        don&#39;t pass anything for this arg, it will default to &#39;&#39;.&quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="get_args-67"><a href="#get_args-67"><span class="linenos">67</span></a>    <span class="p">)</span>
-</span><span id="get_args-68"><a href="#get_args-68"><span class="linenos">68</span></a>
-</span><span id="get_args-69"><a href="#get_args-69"><span class="linenos">69</span></a>    <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="o">.</span><span class="n">parse_args</span><span class="p">()</span>
-</span><span id="get_args-70"><a href="#get_args-70"><span class="linenos">70</span></a>
-</span><span id="get_args-71"><a href="#get_args-71"><span class="linenos">71</span></a>    <span class="k">return</span> <span class="n">args</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="get_args-9"><a href="#get_args-9"><span class="linenos"> 9</span></a><span class="k">def</span> <span class="nf">get_args</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">:</span>
+</span><span id="get_args-10"><a href="#get_args-10"><span class="linenos">10</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">argparse</span><span class="o">.</span><span class="n">ArgumentParser</span><span class="p">()</span>
+</span><span id="get_args-11"><a href="#get_args-11"><span class="linenos">11</span></a>
+</span><span id="get_args-12"><a href="#get_args-12"><span class="linenos">12</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="get_args-13"><a href="#get_args-13"><span class="linenos">13</span></a>        <span class="s2">&quot;-n&quot;</span><span class="p">,</span>
+</span><span id="get_args-14"><a href="#get_args-14"><span class="linenos">14</span></a>        <span class="s2">&quot;--name&quot;</span><span class="p">,</span>
+</span><span id="get_args-15"><a href="#get_args-15"><span class="linenos">15</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
+</span><span id="get_args-16"><a href="#get_args-16"><span class="linenos">16</span></a>        <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
+</span><span id="get_args-17"><a href="#get_args-17"><span class="linenos">17</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Your name. This will be used to populate the &#39;authors&#39; field of a packages &#39;pyproject.toml&#39;. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="get_args-18"><a href="#get_args-18"><span class="linenos">18</span></a>    <span class="p">)</span>
+</span><span id="get_args-19"><a href="#get_args-19"><span class="linenos">19</span></a>
+</span><span id="get_args-20"><a href="#get_args-20"><span class="linenos">20</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="get_args-21"><a href="#get_args-21"><span class="linenos">21</span></a>        <span class="s2">&quot;-e&quot;</span><span class="p">,</span>
+</span><span id="get_args-22"><a href="#get_args-22"><span class="linenos">22</span></a>        <span class="s2">&quot;--email&quot;</span><span class="p">,</span>
+</span><span id="get_args-23"><a href="#get_args-23"><span class="linenos">23</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
+</span><span id="get_args-24"><a href="#get_args-24"><span class="linenos">24</span></a>        <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
+</span><span id="get_args-25"><a href="#get_args-25"><span class="linenos">25</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Your email. This will be used to populate the &#39;authors&#39; field of a packages &#39;pyproject.toml&#39;. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="get_args-26"><a href="#get_args-26"><span class="linenos">26</span></a>    <span class="p">)</span>
+</span><span id="get_args-27"><a href="#get_args-27"><span class="linenos">27</span></a>
+</span><span id="get_args-28"><a href="#get_args-28"><span class="linenos">28</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="get_args-29"><a href="#get_args-29"><span class="linenos">29</span></a>        <span class="s2">&quot;-g&quot;</span><span class="p">,</span>
+</span><span id="get_args-30"><a href="#get_args-30"><span class="linenos">30</span></a>        <span class="s2">&quot;--github_username&quot;</span><span class="p">,</span>
+</span><span id="get_args-31"><a href="#get_args-31"><span class="linenos">31</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
+</span><span id="get_args-32"><a href="#get_args-32"><span class="linenos">32</span></a>        <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
+</span><span id="get_args-33"><a href="#get_args-33"><span class="linenos">33</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Your github account name. When creating a new package,</span>
+</span><span id="get_args-34"><a href="#get_args-34"><span class="linenos">34</span></a><span class="s2">        say with the name &#39;mypackage&#39;, the pyproject.toml &#39;Homepage&#39; field</span>
+</span><span id="get_args-35"><a href="#get_args-35"><span class="linenos">35</span></a><span class="s2">        will be set to &#39;https://github.com/</span><span class="si">{github_username}</span><span class="s2">/mypackage&#39;</span>
+</span><span id="get_args-36"><a href="#get_args-36"><span class="linenos">36</span></a><span class="s2">        and the &#39;Source code&#39; field will be set to</span>
+</span><span id="get_args-37"><a href="#get_args-37"><span class="linenos">37</span></a><span class="s2">        &#39;https://github.com/</span><span class="si">{github_username}</span><span class="s2">/mypackage/tree/main/src/mypackage&#39;.&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="get_args-38"><a href="#get_args-38"><span class="linenos">38</span></a>    <span class="p">)</span>
+</span><span id="get_args-39"><a href="#get_args-39"><span class="linenos">39</span></a>
+</span><span id="get_args-40"><a href="#get_args-40"><span class="linenos">40</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="get_args-41"><a href="#get_args-41"><span class="linenos">41</span></a>        <span class="s2">&quot;-d&quot;</span><span class="p">,</span>
+</span><span id="get_args-42"><a href="#get_args-42"><span class="linenos">42</span></a>        <span class="s2">&quot;--docs_url&quot;</span><span class="p">,</span>
+</span><span id="get_args-43"><a href="#get_args-43"><span class="linenos">43</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
+</span><span id="get_args-44"><a href="#get_args-44"><span class="linenos">44</span></a>        <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
+</span><span id="get_args-45"><a href="#get_args-45"><span class="linenos">45</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; The template url to be used in your pyproject.toml file</span>
+</span><span id="get_args-46"><a href="#get_args-46"><span class="linenos">46</span></a><span class="s2">        indicating where your project docs will be hosted.</span>
+</span><span id="get_args-47"><a href="#get_args-47"><span class="linenos">47</span></a><span class="s2">        Pass the url such that the spot the actual package name will go is</span>
+</span><span id="get_args-48"><a href="#get_args-48"><span class="linenos">48</span></a><span class="s2">        held by &#39;$name&#39;, e.g. &#39;https://somedocswebsite/user/projects/$name&#39;.</span>
+</span><span id="get_args-49"><a href="#get_args-49"><span class="linenos">49</span></a><span class="s2">        If &#39;hassle_config.toml&#39; didn&#39;t exist prior to running this tool and nothing</span>
+</span><span id="get_args-50"><a href="#get_args-50"><span class="linenos">50</span></a><span class="s2">        is given for this arg, it will default to using the package&#39;s github</span>
+</span><span id="get_args-51"><a href="#get_args-51"><span class="linenos">51</span></a><span class="s2">        url. e.g. for package &#39;mypackage&#39; the url will be </span>
+</span><span id="get_args-52"><a href="#get_args-52"><span class="linenos">52</span></a><span class="s2">        &#39;https://github.com/</span><span class="si">{your_github_name}</span><span class="s2">/mypackage/tree/main/docs&#39; &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="get_args-53"><a href="#get_args-53"><span class="linenos">53</span></a>    <span class="p">)</span>
+</span><span id="get_args-54"><a href="#get_args-54"><span class="linenos">54</span></a>
+</span><span id="get_args-55"><a href="#get_args-55"><span class="linenos">55</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="get_args-56"><a href="#get_args-56"><span class="linenos">56</span></a>        <span class="s2">&quot;-t&quot;</span><span class="p">,</span>
+</span><span id="get_args-57"><a href="#get_args-57"><span class="linenos">57</span></a>        <span class="s2">&quot;--tag_prefix&quot;</span><span class="p">,</span>
+</span><span id="get_args-58"><a href="#get_args-58"><span class="linenos">58</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
+</span><span id="get_args-59"><a href="#get_args-59"><span class="linenos">59</span></a>        <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
+</span><span id="get_args-60"><a href="#get_args-60"><span class="linenos">60</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; The tag prefix to use with git when tagging source code versions.</span>
+</span><span id="get_args-61"><a href="#get_args-61"><span class="linenos">61</span></a><span class="s2">        e.g. hassle will use the current version in your pyproject.toml file to when </span>
+</span><span id="get_args-62"><a href="#get_args-62"><span class="linenos">62</span></a><span class="s2">        adding a git tag. If you&#39;ve passed &#39;v&#39; to this arg and the version of your</span>
+</span><span id="get_args-63"><a href="#get_args-63"><span class="linenos">63</span></a><span class="s2">        hypothetical package is &#39;1.0.1&#39;, it will be tagged as &#39;v1.0.1&#39;.</span>
+</span><span id="get_args-64"><a href="#get_args-64"><span class="linenos">64</span></a><span class="s2">        If &#39;hassle_config.toml&#39; didn&#39;t exist prior to running this tool and you</span>
+</span><span id="get_args-65"><a href="#get_args-65"><span class="linenos">65</span></a><span class="s2">        don&#39;t pass anything for this arg, it will default to &#39;&#39;.&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="get_args-66"><a href="#get_args-66"><span class="linenos">66</span></a>    <span class="p">)</span>
+</span><span id="get_args-67"><a href="#get_args-67"><span class="linenos">67</span></a>
+</span><span id="get_args-68"><a href="#get_args-68"><span class="linenos">68</span></a>    <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="o">.</span><span class="n">parse_args</span><span class="p">()</span>
+</span><span id="get_args-69"><a href="#get_args-69"><span class="linenos">69</span></a>
+</span><span id="get_args-70"><a href="#get_args-70"><span class="linenos">70</span></a>    <span class="k">return</span> <span class="n">args</span>
 </span></pre></div>
 
 
     
 
                 </section>
                 <section id="config_exists">
@@ -329,17 +328,17 @@
         <span class="def">def</span>
         <span class="name">config_exists</span><span class="signature pdoc-code condensed">(<span class="return-annotation">) -> <span class="nb">bool</span>:</span></span>
 
                 <label class="view-source-button" for="config_exists-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#config_exists"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="config_exists-74"><a href="#config_exists-74"><span class="linenos">74</span></a><span class="k">def</span> <span class="nf">config_exists</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
-</span><span id="config_exists-75"><a href="#config_exists-75"><span class="linenos">75</span></a>    <span class="sd">&quot;&quot;&quot;Check if hassle_config.toml exists.&quot;&quot;&quot;</span>
-</span><span id="config_exists-76"><a href="#config_exists-76"><span class="linenos">76</span></a>    <span class="k">return</span> <span class="p">(</span><span class="n">root</span> <span class="o">/</span> <span class="s2">&quot;hassle_config.toml&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">exists</span><span class="p">()</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="config_exists-73"><a href="#config_exists-73"><span class="linenos">73</span></a><span class="k">def</span> <span class="nf">config_exists</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
+</span><span id="config_exists-74"><a href="#config_exists-74"><span class="linenos">74</span></a>    <span class="sd">&quot;&quot;&quot;Check if hassle_config.toml exists.&quot;&quot;&quot;</span>
+</span><span id="config_exists-75"><a href="#config_exists-75"><span class="linenos">75</span></a>    <span class="k">return</span> <span class="p">(</span><span class="n">root</span> <span class="o">/</span> <span class="s2">&quot;hassle_config.toml&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">exists</span><span class="p">()</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Check if hassle_config.toml exists.</p>
 </div>
 
 
@@ -351,22 +350,22 @@
         <span class="def">def</span>
         <span class="name">load_config</span><span class="signature pdoc-code condensed">(<span class="return-annotation">) -> <span class="nb">dict</span>:</span></span>
 
                 <label class="view-source-button" for="load_config-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#load_config"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="load_config-79"><a href="#load_config-79"><span class="linenos">79</span></a><span class="k">def</span> <span class="nf">load_config</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="nb">dict</span><span class="p">:</span>
-</span><span id="load_config-80"><a href="#load_config-80"><span class="linenos">80</span></a>    <span class="s2">&quot;Load and return hassle_config contents if it exists.&quot;</span>
-</span><span id="load_config-81"><a href="#load_config-81"><span class="linenos">81</span></a>    <span class="k">if</span> <span class="n">config_exists</span><span class="p">():</span>
-</span><span id="load_config-82"><a href="#load_config-82"><span class="linenos">82</span></a>        <span class="k">return</span> <span class="n">tomlkit</span><span class="o">.</span><span class="n">loads</span><span class="p">((</span><span class="n">root</span> <span class="o">/</span> <span class="s2">&quot;hassle_config.toml&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">read_text</span><span class="p">())</span>
-</span><span id="load_config-83"><a href="#load_config-83"><span class="linenos">83</span></a>    <span class="k">else</span><span class="p">:</span>
-</span><span id="load_config-84"><a href="#load_config-84"><span class="linenos">84</span></a>        <span class="k">raise</span> <span class="ne">FileNotFoundError</span><span class="p">(</span>
-</span><span id="load_config-85"><a href="#load_config-85"><span class="linenos">85</span></a>            <span class="sa">f</span><span class="s2">&quot;load_config() could not find </span><span class="si">{</span><span class="n">root</span><span class="o">/</span><span class="s1">&#39;hassle_config.toml&#39;</span><span class="si">}</span><span class="s2">.</span><span class="se">\n</span><span class="s2">Run hassle_config to set it.&quot;</span>
-</span><span id="load_config-86"><a href="#load_config-86"><span class="linenos">86</span></a>        <span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="load_config-78"><a href="#load_config-78"><span class="linenos">78</span></a><span class="k">def</span> <span class="nf">load_config</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="nb">dict</span><span class="p">:</span>
+</span><span id="load_config-79"><a href="#load_config-79"><span class="linenos">79</span></a>    <span class="s2">&quot;Load and return hassle_config contents if it exists.&quot;</span>
+</span><span id="load_config-80"><a href="#load_config-80"><span class="linenos">80</span></a>    <span class="k">if</span> <span class="n">config_exists</span><span class="p">():</span>
+</span><span id="load_config-81"><a href="#load_config-81"><span class="linenos">81</span></a>        <span class="k">return</span> <span class="p">(</span><span class="n">root</span> <span class="o">/</span> <span class="s2">&quot;hassle_config.toml&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">loads</span><span class="p">()</span>
+</span><span id="load_config-82"><a href="#load_config-82"><span class="linenos">82</span></a>    <span class="k">else</span><span class="p">:</span>
+</span><span id="load_config-83"><a href="#load_config-83"><span class="linenos">83</span></a>        <span class="k">raise</span> <span class="ne">FileNotFoundError</span><span class="p">(</span>
+</span><span id="load_config-84"><a href="#load_config-84"><span class="linenos">84</span></a>            <span class="sa">f</span><span class="s2">&quot;load_config() could not find </span><span class="si">{</span><span class="n">root</span><span class="o">/</span><span class="s1">&#39;hassle_config.toml&#39;</span><span class="si">}</span><span class="s2">.</span><span class="se">\n</span><span class="s2">Run hassle_config to set it.&quot;</span>
+</span><span id="load_config-85"><a href="#load_config-85"><span class="linenos">85</span></a>        <span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Load and return hassle_config contents if it exists.</p>
 </div>
 
 
@@ -378,17 +377,17 @@
         <span class="def">def</span>
         <span class="name">write_config</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">config</span><span class="p">:</span> <span class="nb">dict</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="write_config-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#write_config"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="write_config-89"><a href="#write_config-89"><span class="linenos">89</span></a><span class="k">def</span> <span class="nf">write_config</span><span class="p">(</span><span class="n">config</span><span class="p">:</span> <span class="nb">dict</span><span class="p">):</span>
-</span><span id="write_config-90"><a href="#write_config-90"><span class="linenos">90</span></a>    <span class="sd">&quot;&quot;&quot;Dump config to &quot;hassle_config.toml.&quot;&quot;&quot;</span>
-</span><span id="write_config-91"><a href="#write_config-91"><span class="linenos">91</span></a>    <span class="p">(</span><span class="n">root</span> <span class="o">/</span> <span class="s2">&quot;hassle_config.toml&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="n">tomlkit</span><span class="o">.</span><span class="n">dumps</span><span class="p">(</span><span class="n">config</span><span class="p">))</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="write_config-88"><a href="#write_config-88"><span class="linenos">88</span></a><span class="k">def</span> <span class="nf">write_config</span><span class="p">(</span><span class="n">config</span><span class="p">:</span> <span class="nb">dict</span><span class="p">):</span>
+</span><span id="write_config-89"><a href="#write_config-89"><span class="linenos">89</span></a>    <span class="sd">&quot;&quot;&quot;Dump config to &quot;hassle_config.toml.&quot;&quot;&quot;</span>
+</span><span id="write_config-90"><a href="#write_config-90"><span class="linenos">90</span></a>    <span class="p">(</span><span class="n">root</span> <span class="o">/</span> <span class="s2">&quot;hassle_config.toml&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">dumps</span><span class="p">(</span><span class="n">config</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Dump config to "hassle_config.toml.</p>
 </div>
 
 
@@ -400,18 +399,18 @@
         <span class="def">def</span>
         <span class="name">warn</span><span class="signature pdoc-code condensed">(<span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="warn-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#warn"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="warn-94"><a href="#warn-94"><span class="linenos">94</span></a><span class="k">def</span> <span class="nf">warn</span><span class="p">():</span>
-</span><span id="warn-95"><a href="#warn-95"><span class="linenos">95</span></a>    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;hassle_config.toml has not been set.&quot;</span><span class="p">)</span>
-</span><span id="warn-96"><a href="#warn-96"><span class="linenos">96</span></a>    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Run hassle_config to set it.&quot;</span><span class="p">)</span>
-</span><span id="warn-97"><a href="#warn-97"><span class="linenos">97</span></a>    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Run &#39;hassle_config -h&#39; for help.&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="warn-93"><a href="#warn-93"><span class="linenos">93</span></a><span class="k">def</span> <span class="nf">warn</span><span class="p">():</span>
+</span><span id="warn-94"><a href="#warn-94"><span class="linenos">94</span></a>    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;hassle_config.toml has not been set.&quot;</span><span class="p">)</span>
+</span><span id="warn-95"><a href="#warn-95"><span class="linenos">95</span></a>    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Run hassle_config to set it.&quot;</span><span class="p">)</span>
+</span><span id="warn-96"><a href="#warn-96"><span class="linenos">96</span></a>    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Run &#39;hassle_config -h&#39; for help.&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
     
 
                 </section>
                 <section id="create_config">
@@ -421,71 +420,71 @@
         <span class="def">def</span>
         <span class="name">create_config</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="n">name</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">email</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">github_username</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">docs_url</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">tag_prefix</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="create_config-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#create_config"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="create_config-100"><a href="#create_config-100"><span class="linenos">100</span></a><span class="k">def</span> <span class="nf">create_config</span><span class="p">(</span>
-</span><span id="create_config-101"><a href="#create_config-101"><span class="linenos">101</span></a>    <span class="n">name</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="create_config-102"><a href="#create_config-102"><span class="linenos">102</span></a>    <span class="n">email</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="create_config-103"><a href="#create_config-103"><span class="linenos">103</span></a>    <span class="n">github_username</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="create_config-104"><a href="#create_config-104"><span class="linenos">104</span></a>    <span class="n">docs_url</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="create_config-105"><a href="#create_config-105"><span class="linenos">105</span></a>    <span class="n">tag_prefix</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="create_config-106"><a href="#create_config-106"><span class="linenos">106</span></a><span class="p">):</span>
-</span><span id="create_config-107"><a href="#create_config-107"><span class="linenos">107</span></a>    <span class="sd">&quot;&quot;&quot;Create hassle_config.toml from given args.&quot;&quot;&quot;</span>
-</span><span id="create_config-108"><a href="#create_config-108"><span class="linenos">108</span></a>    <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Manual edits can be made at </span><span class="si">{</span><span class="n">root</span><span class="o">/</span><span class="s1">&#39;hassle_config.toml&#39;</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="create_config-109"><a href="#create_config-109"><span class="linenos">109</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">config_exists</span><span class="p">():</span>
-</span><span id="create_config-110"><a href="#create_config-110"><span class="linenos">110</span></a>        <span class="n">config</span> <span class="o">=</span> <span class="p">{}</span>
-</span><span id="create_config-111"><a href="#create_config-111"><span class="linenos">111</span></a>        <span class="k">if</span> <span class="n">name</span> <span class="ow">and</span> <span class="n">email</span><span class="p">:</span>
-</span><span id="create_config-112"><a href="#create_config-112"><span class="linenos">112</span></a>            <span class="n">config</span><span class="p">[</span><span class="s2">&quot;authors&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="p">[{</span><span class="s2">&quot;name&quot;</span><span class="p">:</span> <span class="n">name</span><span class="p">,</span> <span class="s2">&quot;email&quot;</span><span class="p">:</span> <span class="n">email</span><span class="p">}]</span>
-</span><span id="create_config-113"><a href="#create_config-113"><span class="linenos">113</span></a>        <span class="k">elif</span> <span class="n">name</span><span class="p">:</span>
-</span><span id="create_config-114"><a href="#create_config-114"><span class="linenos">114</span></a>            <span class="n">config</span><span class="p">[</span><span class="s2">&quot;authors&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="p">[{</span><span class="s2">&quot;name&quot;</span><span class="p">:</span> <span class="n">name</span><span class="p">}]</span>
-</span><span id="create_config-115"><a href="#create_config-115"><span class="linenos">115</span></a>        <span class="k">elif</span> <span class="n">email</span><span class="p">:</span>
-</span><span id="create_config-116"><a href="#create_config-116"><span class="linenos">116</span></a>            <span class="n">config</span><span class="p">[</span><span class="s2">&quot;authors&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="p">[{</span><span class="s2">&quot;email&quot;</span><span class="p">:</span> <span class="n">email</span><span class="p">}]</span>
-</span><span id="create_config-117"><a href="#create_config-117"><span class="linenos">117</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="create_config-118"><a href="#create_config-118"><span class="linenos">118</span></a>            <span class="c1"># In case anything upstream would fail if nothing is present for &#39;authors&#39;</span>
-</span><span id="create_config-119"><a href="#create_config-119"><span class="linenos">119</span></a>            <span class="n">config</span><span class="p">[</span><span class="s2">&quot;authors&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="p">[{</span><span class="s2">&quot;name&quot;</span><span class="p">:</span> <span class="s2">&quot;&quot;</span><span class="p">,</span> <span class="s2">&quot;email&quot;</span><span class="p">:</span> <span class="s2">&quot;&quot;</span><span class="p">}]</span>
-</span><span id="create_config-120"><a href="#create_config-120"><span class="linenos">120</span></a>        <span class="n">config</span><span class="p">[</span><span class="s2">&quot;project_urls&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="p">{</span>
-</span><span id="create_config-121"><a href="#create_config-121"><span class="linenos">121</span></a>            <span class="s2">&quot;Homepage&quot;</span><span class="p">:</span> <span class="s2">&quot;&quot;</span><span class="p">,</span>
-</span><span id="create_config-122"><a href="#create_config-122"><span class="linenos">122</span></a>            <span class="s2">&quot;Documentation&quot;</span><span class="p">:</span> <span class="s2">&quot;&quot;</span><span class="p">,</span>
-</span><span id="create_config-123"><a href="#create_config-123"><span class="linenos">123</span></a>            <span class="s2">&quot;Source code&quot;</span><span class="p">:</span> <span class="s2">&quot;&quot;</span><span class="p">,</span>
-</span><span id="create_config-124"><a href="#create_config-124"><span class="linenos">124</span></a>        <span class="p">}</span>
-</span><span id="create_config-125"><a href="#create_config-125"><span class="linenos">125</span></a>        <span class="n">config</span><span class="p">[</span><span class="s2">&quot;git&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="p">{}</span>
-</span><span id="create_config-126"><a href="#create_config-126"><span class="linenos">126</span></a>    <span class="k">else</span><span class="p">:</span>
-</span><span id="create_config-127"><a href="#create_config-127"><span class="linenos">127</span></a>        <span class="n">config</span> <span class="o">=</span> <span class="n">load_config</span><span class="p">()</span>
-</span><span id="create_config-128"><a href="#create_config-128"><span class="linenos">128</span></a>        <span class="k">if</span> <span class="n">name</span> <span class="ow">and</span> <span class="n">email</span><span class="p">:</span>
-</span><span id="create_config-129"><a href="#create_config-129"><span class="linenos">129</span></a>            <span class="n">config</span><span class="p">[</span><span class="s2">&quot;authors&quot;</span><span class="p">]</span><span class="o">.</span><span class="n">append</span><span class="p">({</span><span class="s2">&quot;name&quot;</span><span class="p">:</span> <span class="n">name</span><span class="p">,</span> <span class="s2">&quot;email&quot;</span><span class="p">:</span> <span class="n">email</span><span class="p">})</span>
-</span><span id="create_config-130"><a href="#create_config-130"><span class="linenos">130</span></a>        <span class="k">elif</span> <span class="n">name</span><span class="p">:</span>
-</span><span id="create_config-131"><a href="#create_config-131"><span class="linenos">131</span></a>            <span class="n">config</span><span class="p">[</span><span class="s2">&quot;authors&quot;</span><span class="p">]</span><span class="o">.</span><span class="n">append</span><span class="p">({</span><span class="s2">&quot;name&quot;</span><span class="p">:</span> <span class="n">name</span><span class="p">})</span>
-</span><span id="create_config-132"><a href="#create_config-132"><span class="linenos">132</span></a>        <span class="k">elif</span> <span class="n">email</span><span class="p">:</span>
-</span><span id="create_config-133"><a href="#create_config-133"><span class="linenos">133</span></a>            <span class="n">config</span><span class="p">[</span><span class="s2">&quot;authors&quot;</span><span class="p">]</span><span class="o">.</span><span class="n">append</span><span class="p">({</span><span class="s2">&quot;email&quot;</span><span class="p">:</span> <span class="n">email</span><span class="p">})</span>
-</span><span id="create_config-134"><a href="#create_config-134"><span class="linenos">134</span></a>
-</span><span id="create_config-135"><a href="#create_config-135"><span class="linenos">135</span></a>    <span class="k">if</span> <span class="n">github_username</span><span class="p">:</span>
-</span><span id="create_config-136"><a href="#create_config-136"><span class="linenos">136</span></a>        <span class="n">config</span><span class="p">[</span><span class="s2">&quot;project_urls&quot;</span><span class="p">][</span>
-</span><span id="create_config-137"><a href="#create_config-137"><span class="linenos">137</span></a>            <span class="s2">&quot;Homepage&quot;</span>
-</span><span id="create_config-138"><a href="#create_config-138"><span class="linenos">138</span></a>        <span class="p">]</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;https://github.com/</span><span class="si">{</span><span class="n">github_username</span><span class="si">}</span><span class="s2">/$name&quot;</span>
-</span><span id="create_config-139"><a href="#create_config-139"><span class="linenos">139</span></a>        <span class="n">config</span><span class="p">[</span><span class="s2">&quot;project_urls&quot;</span><span class="p">][</span>
-</span><span id="create_config-140"><a href="#create_config-140"><span class="linenos">140</span></a>            <span class="s2">&quot;Source code&quot;</span>
-</span><span id="create_config-141"><a href="#create_config-141"><span class="linenos">141</span></a>        <span class="p">]</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">config</span><span class="p">[</span><span class="s1">&#39;project_urls&#39;</span><span class="p">][</span><span class="s1">&#39;Homepage&#39;</span><span class="p">]</span><span class="si">}</span><span class="s2">/tree/main/src/$name&quot;</span>
-</span><span id="create_config-142"><a href="#create_config-142"><span class="linenos">142</span></a>
-</span><span id="create_config-143"><a href="#create_config-143"><span class="linenos">143</span></a>    <span class="k">if</span> <span class="n">docs_url</span><span class="p">:</span>
-</span><span id="create_config-144"><a href="#create_config-144"><span class="linenos">144</span></a>        <span class="n">config</span><span class="p">[</span><span class="s2">&quot;project_urls&quot;</span><span class="p">][</span><span class="s2">&quot;Documentation&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">docs_url</span>
-</span><span id="create_config-145"><a href="#create_config-145"><span class="linenos">145</span></a>    <span class="k">elif</span> <span class="n">github_username</span> <span class="ow">and</span> <span class="n">config</span><span class="p">[</span><span class="s2">&quot;project_urls&quot;</span><span class="p">][</span><span class="s2">&quot;Documentation&quot;</span><span class="p">]</span> <span class="o">==</span> <span class="s2">&quot;&quot;</span><span class="p">:</span>
-</span><span id="create_config-146"><a href="#create_config-146"><span class="linenos">146</span></a>        <span class="n">config</span><span class="p">[</span><span class="s2">&quot;project_urls&quot;</span><span class="p">][</span>
-</span><span id="create_config-147"><a href="#create_config-147"><span class="linenos">147</span></a>            <span class="s2">&quot;Documentation&quot;</span>
-</span><span id="create_config-148"><a href="#create_config-148"><span class="linenos">148</span></a>        <span class="p">]</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;https://github.com/</span><span class="si">{</span><span class="n">github_username</span><span class="si">}</span><span class="s2">/$name/tree/main/docs&quot;</span>
-</span><span id="create_config-149"><a href="#create_config-149"><span class="linenos">149</span></a>
-</span><span id="create_config-150"><a href="#create_config-150"><span class="linenos">150</span></a>    <span class="k">if</span> <span class="n">tag_prefix</span><span class="p">:</span>
-</span><span id="create_config-151"><a href="#create_config-151"><span class="linenos">151</span></a>        <span class="n">config</span><span class="p">[</span><span class="s2">&quot;git&quot;</span><span class="p">][</span><span class="s2">&quot;tag_prefix&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">tag_prefix</span>
-</span><span id="create_config-152"><a href="#create_config-152"><span class="linenos">152</span></a>    <span class="k">elif</span> <span class="ow">not</span> <span class="n">config_exists</span><span class="p">()</span> <span class="ow">and</span> <span class="ow">not</span> <span class="n">tag_prefix</span><span class="p">:</span>
-</span><span id="create_config-153"><a href="#create_config-153"><span class="linenos">153</span></a>        <span class="n">config</span><span class="p">[</span><span class="s2">&quot;git&quot;</span><span class="p">][</span><span class="s2">&quot;tag_prefix&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
-</span><span id="create_config-154"><a href="#create_config-154"><span class="linenos">154</span></a>
-</span><span id="create_config-155"><a href="#create_config-155"><span class="linenos">155</span></a>    <span class="k">if</span> <span class="n">config</span><span class="p">:</span>
-</span><span id="create_config-156"><a href="#create_config-156"><span class="linenos">156</span></a>        <span class="n">write_config</span><span class="p">(</span><span class="n">config</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="create_config-99"><a href="#create_config-99"><span class="linenos"> 99</span></a><span class="k">def</span> <span class="nf">create_config</span><span class="p">(</span>
+</span><span id="create_config-100"><a href="#create_config-100"><span class="linenos">100</span></a>    <span class="n">name</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="create_config-101"><a href="#create_config-101"><span class="linenos">101</span></a>    <span class="n">email</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="create_config-102"><a href="#create_config-102"><span class="linenos">102</span></a>    <span class="n">github_username</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="create_config-103"><a href="#create_config-103"><span class="linenos">103</span></a>    <span class="n">docs_url</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="create_config-104"><a href="#create_config-104"><span class="linenos">104</span></a>    <span class="n">tag_prefix</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="create_config-105"><a href="#create_config-105"><span class="linenos">105</span></a><span class="p">):</span>
+</span><span id="create_config-106"><a href="#create_config-106"><span class="linenos">106</span></a>    <span class="sd">&quot;&quot;&quot;Create hassle_config.toml from given args.&quot;&quot;&quot;</span>
+</span><span id="create_config-107"><a href="#create_config-107"><span class="linenos">107</span></a>    <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Manual edits can be made at </span><span class="si">{</span><span class="n">root</span><span class="o">/</span><span class="s1">&#39;hassle_config.toml&#39;</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="create_config-108"><a href="#create_config-108"><span class="linenos">108</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">config_exists</span><span class="p">():</span>
+</span><span id="create_config-109"><a href="#create_config-109"><span class="linenos">109</span></a>        <span class="n">config</span> <span class="o">=</span> <span class="p">{}</span>
+</span><span id="create_config-110"><a href="#create_config-110"><span class="linenos">110</span></a>        <span class="k">if</span> <span class="n">name</span> <span class="ow">and</span> <span class="n">email</span><span class="p">:</span>
+</span><span id="create_config-111"><a href="#create_config-111"><span class="linenos">111</span></a>            <span class="n">config</span><span class="p">[</span><span class="s2">&quot;authors&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="p">[{</span><span class="s2">&quot;name&quot;</span><span class="p">:</span> <span class="n">name</span><span class="p">,</span> <span class="s2">&quot;email&quot;</span><span class="p">:</span> <span class="n">email</span><span class="p">}]</span>
+</span><span id="create_config-112"><a href="#create_config-112"><span class="linenos">112</span></a>        <span class="k">elif</span> <span class="n">name</span><span class="p">:</span>
+</span><span id="create_config-113"><a href="#create_config-113"><span class="linenos">113</span></a>            <span class="n">config</span><span class="p">[</span><span class="s2">&quot;authors&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="p">[{</span><span class="s2">&quot;name&quot;</span><span class="p">:</span> <span class="n">name</span><span class="p">}]</span>
+</span><span id="create_config-114"><a href="#create_config-114"><span class="linenos">114</span></a>        <span class="k">elif</span> <span class="n">email</span><span class="p">:</span>
+</span><span id="create_config-115"><a href="#create_config-115"><span class="linenos">115</span></a>            <span class="n">config</span><span class="p">[</span><span class="s2">&quot;authors&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="p">[{</span><span class="s2">&quot;email&quot;</span><span class="p">:</span> <span class="n">email</span><span class="p">}]</span>
+</span><span id="create_config-116"><a href="#create_config-116"><span class="linenos">116</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="create_config-117"><a href="#create_config-117"><span class="linenos">117</span></a>            <span class="c1"># In case anything upstream would fail if nothing is present for &#39;authors&#39;</span>
+</span><span id="create_config-118"><a href="#create_config-118"><span class="linenos">118</span></a>            <span class="n">config</span><span class="p">[</span><span class="s2">&quot;authors&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="p">[{</span><span class="s2">&quot;name&quot;</span><span class="p">:</span> <span class="s2">&quot;&quot;</span><span class="p">,</span> <span class="s2">&quot;email&quot;</span><span class="p">:</span> <span class="s2">&quot;&quot;</span><span class="p">}]</span>
+</span><span id="create_config-119"><a href="#create_config-119"><span class="linenos">119</span></a>        <span class="n">config</span><span class="p">[</span><span class="s2">&quot;project_urls&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="p">{</span>
+</span><span id="create_config-120"><a href="#create_config-120"><span class="linenos">120</span></a>            <span class="s2">&quot;Homepage&quot;</span><span class="p">:</span> <span class="s2">&quot;&quot;</span><span class="p">,</span>
+</span><span id="create_config-121"><a href="#create_config-121"><span class="linenos">121</span></a>            <span class="s2">&quot;Documentation&quot;</span><span class="p">:</span> <span class="s2">&quot;&quot;</span><span class="p">,</span>
+</span><span id="create_config-122"><a href="#create_config-122"><span class="linenos">122</span></a>            <span class="s2">&quot;Source code&quot;</span><span class="p">:</span> <span class="s2">&quot;&quot;</span><span class="p">,</span>
+</span><span id="create_config-123"><a href="#create_config-123"><span class="linenos">123</span></a>        <span class="p">}</span>
+</span><span id="create_config-124"><a href="#create_config-124"><span class="linenos">124</span></a>        <span class="n">config</span><span class="p">[</span><span class="s2">&quot;git&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="p">{}</span>
+</span><span id="create_config-125"><a href="#create_config-125"><span class="linenos">125</span></a>    <span class="k">else</span><span class="p">:</span>
+</span><span id="create_config-126"><a href="#create_config-126"><span class="linenos">126</span></a>        <span class="n">config</span> <span class="o">=</span> <span class="n">load_config</span><span class="p">()</span>
+</span><span id="create_config-127"><a href="#create_config-127"><span class="linenos">127</span></a>        <span class="k">if</span> <span class="n">name</span> <span class="ow">and</span> <span class="n">email</span><span class="p">:</span>
+</span><span id="create_config-128"><a href="#create_config-128"><span class="linenos">128</span></a>            <span class="n">config</span><span class="p">[</span><span class="s2">&quot;authors&quot;</span><span class="p">]</span><span class="o">.</span><span class="n">append</span><span class="p">({</span><span class="s2">&quot;name&quot;</span><span class="p">:</span> <span class="n">name</span><span class="p">,</span> <span class="s2">&quot;email&quot;</span><span class="p">:</span> <span class="n">email</span><span class="p">})</span>
+</span><span id="create_config-129"><a href="#create_config-129"><span class="linenos">129</span></a>        <span class="k">elif</span> <span class="n">name</span><span class="p">:</span>
+</span><span id="create_config-130"><a href="#create_config-130"><span class="linenos">130</span></a>            <span class="n">config</span><span class="p">[</span><span class="s2">&quot;authors&quot;</span><span class="p">]</span><span class="o">.</span><span class="n">append</span><span class="p">({</span><span class="s2">&quot;name&quot;</span><span class="p">:</span> <span class="n">name</span><span class="p">})</span>
+</span><span id="create_config-131"><a href="#create_config-131"><span class="linenos">131</span></a>        <span class="k">elif</span> <span class="n">email</span><span class="p">:</span>
+</span><span id="create_config-132"><a href="#create_config-132"><span class="linenos">132</span></a>            <span class="n">config</span><span class="p">[</span><span class="s2">&quot;authors&quot;</span><span class="p">]</span><span class="o">.</span><span class="n">append</span><span class="p">({</span><span class="s2">&quot;email&quot;</span><span class="p">:</span> <span class="n">email</span><span class="p">})</span>
+</span><span id="create_config-133"><a href="#create_config-133"><span class="linenos">133</span></a>
+</span><span id="create_config-134"><a href="#create_config-134"><span class="linenos">134</span></a>    <span class="k">if</span> <span class="n">github_username</span><span class="p">:</span>
+</span><span id="create_config-135"><a href="#create_config-135"><span class="linenos">135</span></a>        <span class="n">config</span><span class="p">[</span><span class="s2">&quot;project_urls&quot;</span><span class="p">][</span>
+</span><span id="create_config-136"><a href="#create_config-136"><span class="linenos">136</span></a>            <span class="s2">&quot;Homepage&quot;</span>
+</span><span id="create_config-137"><a href="#create_config-137"><span class="linenos">137</span></a>        <span class="p">]</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;https://github.com/</span><span class="si">{</span><span class="n">github_username</span><span class="si">}</span><span class="s2">/$name&quot;</span>
+</span><span id="create_config-138"><a href="#create_config-138"><span class="linenos">138</span></a>        <span class="n">config</span><span class="p">[</span><span class="s2">&quot;project_urls&quot;</span><span class="p">][</span>
+</span><span id="create_config-139"><a href="#create_config-139"><span class="linenos">139</span></a>            <span class="s2">&quot;Source code&quot;</span>
+</span><span id="create_config-140"><a href="#create_config-140"><span class="linenos">140</span></a>        <span class="p">]</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">config</span><span class="p">[</span><span class="s1">&#39;project_urls&#39;</span><span class="p">][</span><span class="s1">&#39;Homepage&#39;</span><span class="p">]</span><span class="si">}</span><span class="s2">/tree/main/src/$name&quot;</span>
+</span><span id="create_config-141"><a href="#create_config-141"><span class="linenos">141</span></a>
+</span><span id="create_config-142"><a href="#create_config-142"><span class="linenos">142</span></a>    <span class="k">if</span> <span class="n">docs_url</span><span class="p">:</span>
+</span><span id="create_config-143"><a href="#create_config-143"><span class="linenos">143</span></a>        <span class="n">config</span><span class="p">[</span><span class="s2">&quot;project_urls&quot;</span><span class="p">][</span><span class="s2">&quot;Documentation&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">docs_url</span>
+</span><span id="create_config-144"><a href="#create_config-144"><span class="linenos">144</span></a>    <span class="k">elif</span> <span class="n">github_username</span> <span class="ow">and</span> <span class="n">config</span><span class="p">[</span><span class="s2">&quot;project_urls&quot;</span><span class="p">][</span><span class="s2">&quot;Documentation&quot;</span><span class="p">]</span> <span class="o">==</span> <span class="s2">&quot;&quot;</span><span class="p">:</span>
+</span><span id="create_config-145"><a href="#create_config-145"><span class="linenos">145</span></a>        <span class="n">config</span><span class="p">[</span><span class="s2">&quot;project_urls&quot;</span><span class="p">][</span>
+</span><span id="create_config-146"><a href="#create_config-146"><span class="linenos">146</span></a>            <span class="s2">&quot;Documentation&quot;</span>
+</span><span id="create_config-147"><a href="#create_config-147"><span class="linenos">147</span></a>        <span class="p">]</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;https://github.com/</span><span class="si">{</span><span class="n">github_username</span><span class="si">}</span><span class="s2">/$name/tree/main/docs&quot;</span>
+</span><span id="create_config-148"><a href="#create_config-148"><span class="linenos">148</span></a>
+</span><span id="create_config-149"><a href="#create_config-149"><span class="linenos">149</span></a>    <span class="k">if</span> <span class="n">tag_prefix</span><span class="p">:</span>
+</span><span id="create_config-150"><a href="#create_config-150"><span class="linenos">150</span></a>        <span class="n">config</span><span class="p">[</span><span class="s2">&quot;git&quot;</span><span class="p">][</span><span class="s2">&quot;tag_prefix&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">tag_prefix</span>
+</span><span id="create_config-151"><a href="#create_config-151"><span class="linenos">151</span></a>    <span class="k">elif</span> <span class="ow">not</span> <span class="n">config_exists</span><span class="p">()</span> <span class="ow">and</span> <span class="ow">not</span> <span class="n">tag_prefix</span><span class="p">:</span>
+</span><span id="create_config-152"><a href="#create_config-152"><span class="linenos">152</span></a>        <span class="n">config</span><span class="p">[</span><span class="s2">&quot;git&quot;</span><span class="p">][</span><span class="s2">&quot;tag_prefix&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
+</span><span id="create_config-153"><a href="#create_config-153"><span class="linenos">153</span></a>
+</span><span id="create_config-154"><a href="#create_config-154"><span class="linenos">154</span></a>    <span class="k">if</span> <span class="n">config</span><span class="p">:</span>
+</span><span id="create_config-155"><a href="#create_config-155"><span class="linenos">155</span></a>        <span class="n">write_config</span><span class="p">(</span><span class="n">config</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Create hassle_config.toml from given args.</p>
 </div>
 
 
@@ -497,20 +496,20 @@
         <span class="def">def</span>
         <span class="name">main</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">=</span> <span class="kc">None</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="main-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#main"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="main-159"><a href="#main-159"><span class="linenos">159</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
-</span><span id="main-160"><a href="#main-160"><span class="linenos">160</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="p">:</span>
-</span><span id="main-161"><a href="#main-161"><span class="linenos">161</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
-</span><span id="main-162"><a href="#main-162"><span class="linenos">162</span></a>    <span class="n">create_config</span><span class="p">(</span>
-</span><span id="main-163"><a href="#main-163"><span class="linenos">163</span></a>        <span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">email</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">github_username</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">docs_url</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">tag_prefix</span>
-</span><span id="main-164"><a href="#main-164"><span class="linenos">164</span></a>    <span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="main-158"><a href="#main-158"><span class="linenos">158</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
+</span><span id="main-159"><a href="#main-159"><span class="linenos">159</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="p">:</span>
+</span><span id="main-160"><a href="#main-160"><span class="linenos">160</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
+</span><span id="main-161"><a href="#main-161"><span class="linenos">161</span></a>    <span class="n">create_config</span><span class="p">(</span>
+</span><span id="main-162"><a href="#main-162"><span class="linenos">162</span></a>        <span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">email</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">github_username</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">docs_url</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">tag_prefix</span>
+</span><span id="main-163"><a href="#main-163"><span class="linenos">163</span></a>    <span class="p">)</span>
 </span></pre></div>
 
 
     
 
                 </section>
     </main>
```

#### html2text {}

```diff
@@ -11,121 +11,300 @@
     * create_config
     * main
 built_with_pdoc[pdoc_logo]
 
 ****** hassle.hassle_config ******
 ⁰ View Source
 __1import argparse
-__2from pathlib import Path
-__3
-__4import tomlkit
-__5
-__6root = Path(__file__).parent
+__2
+__3from pathier import Pathier
+__4
+__5root = Pathier(__file__).parent
+__6
 __7
-__8
-__9def get_args() -> argparse.Namespace:
-_10    parser = argparse.ArgumentParser()
-_11
-_12    parser.add_argument(
-_13        "-n",
-_14        "--name",
-_15        type=str,
-_16        default=None,
-_17        help=""" Your name. This will be used to populate the 'authors'
+__8def get_args() -> argparse.Namespace:
+__9    parser = argparse.ArgumentParser()
+_10
+_11    parser.add_argument(
+_12        "-n",
+_13        "--name",
+_14        type=str,
+_15        default=None,
+_16        help=""" Your name. This will be used to populate the 'authors'
 field of a packages 'pyproject.toml'. """,
-_18    )
-_19
-_20    parser.add_argument(
-_21        "-e",
-_22        "--email",
-_23        type=str,
-_24        default=None,
-_25        help=""" Your email. This will be used to populate the 'authors'
+_17    )
+_18
+_19    parser.add_argument(
+_20        "-e",
+_21        "--email",
+_22        type=str,
+_23        default=None,
+_24        help=""" Your email. This will be used to populate the 'authors'
 field of a packages 'pyproject.toml'. """,
-_26    )
-_27
-_28    parser.add_argument(
-_29        "-g",
-_30        "--github_username",
-_31        type=str,
-_32        default=None,
-_33        help=""" Your github account name. When creating a new package,
-_34        say with the name 'mypackage', the pyproject.toml 'Homepage' field
-_35        will be set to 'https://github.com/{github_username}/mypackage'
-_36        and the 'Source code' field will be set to
-_37        'https://github.com/{github_username}/mypackage/tree/main/src/
+_25    )
+_26
+_27    parser.add_argument(
+_28        "-g",
+_29        "--github_username",
+_30        type=str,
+_31        default=None,
+_32        help=""" Your github account name. When creating a new package,
+_33        say with the name 'mypackage', the pyproject.toml 'Homepage' field
+_34        will be set to 'https://github.com/{github_username}/mypackage'
+_35        and the 'Source code' field will be set to
+_36        'https://github.com/{github_username}/mypackage/tree/main/src/
 mypackage'.""",
-_38    )
-_39
-_40    parser.add_argument(
-_41        "-d",
-_42        "--docs_url",
-_43        type=str,
-_44        default=None,
-_45        help=""" The template url to be used in your pyproject.toml file
-_46        indicating where your project docs will be hosted.
-_47        Pass the url such that the spot the actual package name will go is
-_48        held by '$name', e.g. 'https://somedocswebsite/user/projects/$name'.
-_49        If 'hassle_config.toml' didn't exist prior to running this tool and
+_37    )
+_38
+_39    parser.add_argument(
+_40        "-d",
+_41        "--docs_url",
+_42        type=str,
+_43        default=None,
+_44        help=""" The template url to be used in your pyproject.toml file
+_45        indicating where your project docs will be hosted.
+_46        Pass the url such that the spot the actual package name will go is
+_47        held by '$name', e.g. 'https://somedocswebsite/user/projects/$name'.
+_48        If 'hassle_config.toml' didn't exist prior to running this tool and
 nothing
-_50        is given for this arg, it will default to using the package's github
-_51        url. e.g. for package 'mypackage' the url will be
-_52        'https://github.com/{your_github_name}/mypackage/tree/main/docs'
+_49        is given for this arg, it will default to using the package's github
+_50        url. e.g. for package 'mypackage' the url will be
+_51        'https://github.com/{your_github_name}/mypackage/tree/main/docs'
 """,
-_53    )
-_54
-_55    parser.add_argument(
-_56        "-t",
-_57        "--tag_prefix",
-_58        type=str,
-_59        default=None,
-_60        help=""" The tag prefix to use with git when tagging source code
+_52    )
+_53
+_54    parser.add_argument(
+_55        "-t",
+_56        "--tag_prefix",
+_57        type=str,
+_58        default=None,
+_59        help=""" The tag prefix to use with git when tagging source code
 versions.
-_61        e.g. hassle will use the current version in your pyproject.toml file
+_60        e.g. hassle will use the current version in your pyproject.toml file
 to when
-_62        adding a git tag. If you've passed 'v' to this arg and the version
+_61        adding a git tag. If you've passed 'v' to this arg and the version
 of your
-_63        hypothetical package is '1.0.1', it will be tagged as 'v1.0.1'.
-_64        If 'hassle_config.toml' didn't exist prior to running this tool and
+_62        hypothetical package is '1.0.1', it will be tagged as 'v1.0.1'.
+_63        If 'hassle_config.toml' didn't exist prior to running this tool and
 you
-_65        don't pass anything for this arg, it will default to ''.""",
-_66    )
-_67
-_68    args = parser.parse_args()
-_69
-_70    return args
+_64        don't pass anything for this arg, it will default to ''.""",
+_65    )
+_66
+_67    args = parser.parse_args()
+_68
+_69    return args
+_70
 _71
-_72
-_73def config_exists() -> bool:
-_74    """Check if hassle_config.toml exists."""
-_75    return (root / "hassle_config.toml").exists()
+_72def config_exists() -> bool:
+_73    """Check if hassle_config.toml exists."""
+_74    return (root / "hassle_config.toml").exists()
+_75
 _76
-_77
-_78def load_config() -> dict:
-_79    "Load and return hassle_config contents if it exists."
-_80    if config_exists():
-_81        return tomlkit.loads((root / "hassle_config.toml").read_text())
-_82    else:
-_83        raise FileNotFoundError(
-_84            f"load_config() could not find {root/'hassle_config.toml'}.\nRun
+_77def load_config() -> dict:
+_78    "Load and return hassle_config contents if it exists."
+_79    if config_exists():
+_80        return (root / "hassle_config.toml").loads()
+_81    else:
+_82        raise FileNotFoundError(
+_83            f"load_config() could not find {root/'hassle_config.toml'}.\nRun
 hassle_config to set it."
-_85        )
+_84        )
+_85
 _86
-_87
-_88def write_config(config: dict):
-_89    """Dump config to "hassle_config.toml."""
-_90    (root / "hassle_config.toml").write_text(tomlkit.dumps(config))
+_87def write_config(config: dict):
+_88    """Dump config to "hassle_config.toml."""
+_89    (root / "hassle_config.toml").dumps(config)
+_90
 _91
-_92
-_93def warn():
-_94    print("hassle_config.toml has not been set.")
-_95    print("Run hassle_config to set it.")
-_96    print("Run 'hassle_config -h' for help.")
+_92def warn():
+_93    print("hassle_config.toml has not been set.")
+_94    print("Run hassle_config to set it.")
+_95    print("Run 'hassle_config -h' for help.")
+_96
 _97
-_98
+_98def create_config(
+_99    name: str = None,
+100    email: str = None,
+101    github_username: str = None,
+102    docs_url: str = None,
+103    tag_prefix: str = None,
+104):
+105    """Create hassle_config.toml from given args."""
+106    print(f"Manual edits can be made at {root/'hassle_config.toml'}")
+107    if not config_exists():
+108        config = {}
+109        if name and email:
+110            config["authors"] = [{"name": name, "email": email}]
+111        elif name:
+112            config["authors"] = [{"name": name}]
+113        elif email:
+114            config["authors"] = [{"email": email}]
+115        else:
+116            # In case anything upstream would fail if nothing is present for
+'authors'
+117            config["authors"] = [{"name": "", "email": ""}]
+118        config["project_urls"] = {
+119            "Homepage": "",
+120            "Documentation": "",
+121            "Source code": "",
+122        }
+123        config["git"] = {}
+124    else:
+125        config = load_config()
+126        if name and email:
+127            config["authors"].append({"name": name, "email": email})
+128        elif name:
+129            config["authors"].append({"name": name})
+130        elif email:
+131            config["authors"].append({"email": email})
+132
+133    if github_username:
+134        config["project_urls"][
+135            "Homepage"
+136        ] = f"https://github.com/{github_username}/$name"
+137        config["project_urls"][
+138            "Source code"
+139        ] = f"{config['project_urls']['Homepage']}/tree/main/src/$name"
+140
+141    if docs_url:
+142        config["project_urls"]["Documentation"] = docs_url
+143    elif github_username and config["project_urls"]["Documentation"] == "":
+144        config["project_urls"][
+145            "Documentation"
+146        ] = f"https://github.com/{github_username}/$name/tree/main/docs"
+147
+148    if tag_prefix:
+149        config["git"]["tag_prefix"] = tag_prefix
+150    elif not config_exists() and not tag_prefix:
+151        config["git"]["tag_prefix"] = ""
+152
+153    if config:
+154        write_config(config)
+155
+156
+157def main(args: argparse.Namespace = None):
+158    if not args:
+159        args = get_args()
+160    create_config(
+161        args.name, args.email, args.github_username, args.docs_url,
+args.tag_prefix
+162    )
+163
+164
+165if __name__ == "__main__":
+166    main(get_args())
+  ⁰
+def get_args() -> argparse.Namespace: View Source
+_9def get_args() -> argparse.Namespace:
+10    parser = argparse.ArgumentParser()
+11
+12    parser.add_argument(
+13        "-n",
+14        "--name",
+15        type=str,
+16        default=None,
+17        help=""" Your name. This will be used to populate the 'authors' field
+of a packages 'pyproject.toml'. """,
+18    )
+19
+20    parser.add_argument(
+21        "-e",
+22        "--email",
+23        type=str,
+24        default=None,
+25        help=""" Your email. This will be used to populate the 'authors'
+field of a packages 'pyproject.toml'. """,
+26    )
+27
+28    parser.add_argument(
+29        "-g",
+30        "--github_username",
+31        type=str,
+32        default=None,
+33        help=""" Your github account name. When creating a new package,
+34        say with the name 'mypackage', the pyproject.toml 'Homepage' field
+35        will be set to 'https://github.com/{github_username}/mypackage'
+36        and the 'Source code' field will be set to
+37        'https://github.com/{github_username}/mypackage/tree/main/src/
+mypackage'.""",
+38    )
+39
+40    parser.add_argument(
+41        "-d",
+42        "--docs_url",
+43        type=str,
+44        default=None,
+45        help=""" The template url to be used in your pyproject.toml file
+46        indicating where your project docs will be hosted.
+47        Pass the url such that the spot the actual package name will go is
+48        held by '$name', e.g. 'https://somedocswebsite/user/projects/$name'.
+49        If 'hassle_config.toml' didn't exist prior to running this tool and
+nothing
+50        is given for this arg, it will default to using the package's github
+51        url. e.g. for package 'mypackage' the url will be
+52        'https://github.com/{your_github_name}/mypackage/tree/main/docs' """,
+53    )
+54
+55    parser.add_argument(
+56        "-t",
+57        "--tag_prefix",
+58        type=str,
+59        default=None,
+60        help=""" The tag prefix to use with git when tagging source code
+versions.
+61        e.g. hassle will use the current version in your pyproject.toml file
+to when
+62        adding a git tag. If you've passed 'v' to this arg and the version of
+your
+63        hypothetical package is '1.0.1', it will be tagged as 'v1.0.1'.
+64        If 'hassle_config.toml' didn't exist prior to running this tool and
+you
+65        don't pass anything for this arg, it will default to ''.""",
+66    )
+67
+68    args = parser.parse_args()
+69
+70    return args
+  ⁰
+def config_exists() -> bool: View Source
+73def config_exists() -> bool:
+74    """Check if hassle_config.toml exists."""
+75    return (root / "hassle_config.toml").exists()
+Check if hassle_config.toml exists.
+  ⁰
+def load_config() -> dict: View Source
+78def load_config() -> dict:
+79    "Load and return hassle_config contents if it exists."
+80    if config_exists():
+81        return (root / "hassle_config.toml").loads()
+82    else:
+83        raise FileNotFoundError(
+84            f"load_config() could not find {root/'hassle_config.toml'}.\nRun
+hassle_config to set it."
+85        )
+Load and return hassle_config contents if it exists.
+  ⁰
+def write_config(config: dict): View Source
+88def write_config(config: dict):
+89    """Dump config to "hassle_config.toml."""
+90    (root / "hassle_config.toml").dumps(config)
+Dump config to "hassle_config.toml.
+  ⁰
+def warn(): View Source
+93def warn():
+94    print("hassle_config.toml has not been set.")
+95    print("Run hassle_config to set it.")
+96    print("Run 'hassle_config -h' for help.")
+  ⁰
+def create_config(
+name: str = None,
+email: str = None,
+github_username: str = None,
+docs_url: str = None,
+tag_prefix: str = None): View Source
 _99def create_config(
 100    name: str = None,
 101    email: str = None,
 102    github_username: str = None,
 103    docs_url: str = None,
 104    tag_prefix: str = None,
 105):
@@ -176,198 +355,18 @@
 149    if tag_prefix:
 150        config["git"]["tag_prefix"] = tag_prefix
 151    elif not config_exists() and not tag_prefix:
 152        config["git"]["tag_prefix"] = ""
 153
 154    if config:
 155        write_config(config)
-156
-157
+Create hassle_config.toml from given args.
+  ⁰
+def main(args: argparse.Namespace = None): View Source
 158def main(args: argparse.Namespace = None):
 159    if not args:
 160        args = get_args()
 161    create_config(
 162        args.name, args.email, args.github_username, args.docs_url,
 args.tag_prefix
 163    )
-164
-165
-166if __name__ == "__main__":
-167    main(get_args())
-  ⁰
-def get_args() -> argparse.Namespace: View Source
-10def get_args() -> argparse.Namespace:
-11    parser = argparse.ArgumentParser()
-12
-13    parser.add_argument(
-14        "-n",
-15        "--name",
-16        type=str,
-17        default=None,
-18        help=""" Your name. This will be used to populate the 'authors' field
-of a packages 'pyproject.toml'. """,
-19    )
-20
-21    parser.add_argument(
-22        "-e",
-23        "--email",
-24        type=str,
-25        default=None,
-26        help=""" Your email. This will be used to populate the 'authors'
-field of a packages 'pyproject.toml'. """,
-27    )
-28
-29    parser.add_argument(
-30        "-g",
-31        "--github_username",
-32        type=str,
-33        default=None,
-34        help=""" Your github account name. When creating a new package,
-35        say with the name 'mypackage', the pyproject.toml 'Homepage' field
-36        will be set to 'https://github.com/{github_username}/mypackage'
-37        and the 'Source code' field will be set to
-38        'https://github.com/{github_username}/mypackage/tree/main/src/
-mypackage'.""",
-39    )
-40
-41    parser.add_argument(
-42        "-d",
-43        "--docs_url",
-44        type=str,
-45        default=None,
-46        help=""" The template url to be used in your pyproject.toml file
-47        indicating where your project docs will be hosted.
-48        Pass the url such that the spot the actual package name will go is
-49        held by '$name', e.g. 'https://somedocswebsite/user/projects/$name'.
-50        If 'hassle_config.toml' didn't exist prior to running this tool and
-nothing
-51        is given for this arg, it will default to using the package's github
-52        url. e.g. for package 'mypackage' the url will be
-53        'https://github.com/{your_github_name}/mypackage/tree/main/docs' """,
-54    )
-55
-56    parser.add_argument(
-57        "-t",
-58        "--tag_prefix",
-59        type=str,
-60        default=None,
-61        help=""" The tag prefix to use with git when tagging source code
-versions.
-62        e.g. hassle will use the current version in your pyproject.toml file
-to when
-63        adding a git tag. If you've passed 'v' to this arg and the version of
-your
-64        hypothetical package is '1.0.1', it will be tagged as 'v1.0.1'.
-65        If 'hassle_config.toml' didn't exist prior to running this tool and
-you
-66        don't pass anything for this arg, it will default to ''.""",
-67    )
-68
-69    args = parser.parse_args()
-70
-71    return args
-  ⁰
-def config_exists() -> bool: View Source
-74def config_exists() -> bool:
-75    """Check if hassle_config.toml exists."""
-76    return (root / "hassle_config.toml").exists()
-Check if hassle_config.toml exists.
-  ⁰
-def load_config() -> dict: View Source
-79def load_config() -> dict:
-80    "Load and return hassle_config contents if it exists."
-81    if config_exists():
-82        return tomlkit.loads((root / "hassle_config.toml").read_text())
-83    else:
-84        raise FileNotFoundError(
-85            f"load_config() could not find {root/'hassle_config.toml'}.\nRun
-hassle_config to set it."
-86        )
-Load and return hassle_config contents if it exists.
-  ⁰
-def write_config(config: dict): View Source
-89def write_config(config: dict):
-90    """Dump config to "hassle_config.toml."""
-91    (root / "hassle_config.toml").write_text(tomlkit.dumps(config))
-Dump config to "hassle_config.toml.
-  ⁰
-def warn(): View Source
-94def warn():
-95    print("hassle_config.toml has not been set.")
-96    print("Run hassle_config to set it.")
-97    print("Run 'hassle_config -h' for help.")
-  ⁰
-def create_config(
-name: str = None,
-email: str = None,
-github_username: str = None,
-docs_url: str = None,
-tag_prefix: str = None): View Source
-100def create_config(
-101    name: str = None,
-102    email: str = None,
-103    github_username: str = None,
-104    docs_url: str = None,
-105    tag_prefix: str = None,
-106):
-107    """Create hassle_config.toml from given args."""
-108    print(f"Manual edits can be made at {root/'hassle_config.toml'}")
-109    if not config_exists():
-110        config = {}
-111        if name and email:
-112            config["authors"] = [{"name": name, "email": email}]
-113        elif name:
-114            config["authors"] = [{"name": name}]
-115        elif email:
-116            config["authors"] = [{"email": email}]
-117        else:
-118            # In case anything upstream would fail if nothing is present for
-'authors'
-119            config["authors"] = [{"name": "", "email": ""}]
-120        config["project_urls"] = {
-121            "Homepage": "",
-122            "Documentation": "",
-123            "Source code": "",
-124        }
-125        config["git"] = {}
-126    else:
-127        config = load_config()
-128        if name and email:
-129            config["authors"].append({"name": name, "email": email})
-130        elif name:
-131            config["authors"].append({"name": name})
-132        elif email:
-133            config["authors"].append({"email": email})
-134
-135    if github_username:
-136        config["project_urls"][
-137            "Homepage"
-138        ] = f"https://github.com/{github_username}/$name"
-139        config["project_urls"][
-140            "Source code"
-141        ] = f"{config['project_urls']['Homepage']}/tree/main/src/$name"
-142
-143    if docs_url:
-144        config["project_urls"]["Documentation"] = docs_url
-145    elif github_username and config["project_urls"]["Documentation"] == "":
-146        config["project_urls"][
-147            "Documentation"
-148        ] = f"https://github.com/{github_username}/$name/tree/main/docs"
-149
-150    if tag_prefix:
-151        config["git"]["tag_prefix"] = tag_prefix
-152    elif not config_exists() and not tag_prefix:
-153        config["git"]["tag_prefix"] = ""
-154
-155    if config:
-156        write_config(config)
-Create hassle_config.toml from given args.
-  ⁰
-def main(args: argparse.Namespace = None): View Source
-159def main(args: argparse.Namespace = None):
-160    if not args:
-161        args = get_args()
-162    create_config(
-163        args.name, args.email, args.github_username, args.docs_url,
-args.tag_prefix
-164    )
```

### Comparing `hassle-2.4.0/docs/hassle/hassle_utilities.html` & `hassle-2.5.0/docs/hassle/hassle_utilities.html`

 * *Files 1% similar despite different names*

```diff
@@ -66,180 +66,176 @@
 
                 
                         <input id="mod-hassle_utilities-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 
                         <label class="view-source-button" for="mod-hassle_utilities-view-source"><span>View Source</span></label>
 
                         <div class="pdoc-code codehilite"><pre><span></span><span id="L-1"><a href="#L-1"><span class="linenos">  1</span></a><span class="kn">import</span> <span class="nn">os</span>
-</span><span id="L-2"><a href="#L-2"><span class="linenos">  2</span></a><span class="kn">import</span> <span class="nn">shutil</span>
-</span><span id="L-3"><a href="#L-3"><span class="linenos">  3</span></a><span class="kn">from</span> <span class="nn">pathlib</span> <span class="kn">import</span> <span class="n">Path</span>
-</span><span id="L-4"><a href="#L-4"><span class="linenos">  4</span></a>
-</span><span id="L-5"><a href="#L-5"><span class="linenos">  5</span></a><span class="kn">import</span> <span class="nn">packagelister</span>
-</span><span id="L-6"><a href="#L-6"><span class="linenos">  6</span></a><span class="kn">import</span> <span class="nn">tomlkit</span>
-</span><span id="L-7"><a href="#L-7"><span class="linenos">  7</span></a><span class="kn">import</span> <span class="nn">vermin</span>
+</span><span id="L-2"><a href="#L-2"><span class="linenos">  2</span></a>
+</span><span id="L-3"><a href="#L-3"><span class="linenos">  3</span></a><span class="kn">import</span> <span class="nn">packagelister</span>
+</span><span id="L-4"><a href="#L-4"><span class="linenos">  4</span></a><span class="kn">import</span> <span class="nn">vermin</span>
+</span><span id="L-5"><a href="#L-5"><span class="linenos">  5</span></a><span class="kn">from</span> <span class="nn">pathier</span> <span class="kn">import</span> <span class="n">Pathier</span>
+</span><span id="L-6"><a href="#L-6"><span class="linenos">  6</span></a>
+</span><span id="L-7"><a href="#L-7"><span class="linenos">  7</span></a><span class="kn">from</span> <span class="nn">hassle</span> <span class="kn">import</span> <span class="n">hassle_config</span>
 </span><span id="L-8"><a href="#L-8"><span class="linenos">  8</span></a>
-</span><span id="L-9"><a href="#L-9"><span class="linenos">  9</span></a><span class="kn">from</span> <span class="nn">hassle</span> <span class="kn">import</span> <span class="n">hassle_config</span>
+</span><span id="L-9"><a href="#L-9"><span class="linenos">  9</span></a><span class="n">root</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="vm">__file__</span><span class="p">)</span><span class="o">.</span><span class="n">parent</span>
 </span><span id="L-10"><a href="#L-10"><span class="linenos"> 10</span></a>
-</span><span id="L-11"><a href="#L-11"><span class="linenos"> 11</span></a><span class="n">root</span> <span class="o">=</span> <span class="n">Path</span><span class="p">(</span><span class="vm">__file__</span><span class="p">)</span><span class="o">.</span><span class="n">parent</span>
-</span><span id="L-12"><a href="#L-12"><span class="linenos"> 12</span></a>
-</span><span id="L-13"><a href="#L-13"><span class="linenos"> 13</span></a>
-</span><span id="L-14"><a href="#L-14"><span class="linenos"> 14</span></a><span class="k">def</span> <span class="nf">increment_version</span><span class="p">(</span><span class="n">pyproject_path</span><span class="p">:</span> <span class="n">Path</span><span class="p">,</span> <span class="n">increment_type</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-15"><a href="#L-15"><span class="linenos"> 15</span></a>    <span class="sd">&quot;&quot;&quot;Increment the project.version field in pyproject.toml.</span>
+</span><span id="L-11"><a href="#L-11"><span class="linenos"> 11</span></a>
+</span><span id="L-12"><a href="#L-12"><span class="linenos"> 12</span></a><span class="k">def</span> <span class="nf">increment_version</span><span class="p">(</span><span class="n">pyproject_path</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">,</span> <span class="n">increment_type</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-13"><a href="#L-13"><span class="linenos"> 13</span></a>    <span class="sd">&quot;&quot;&quot;Increment the project.version field in pyproject.toml.</span>
+</span><span id="L-14"><a href="#L-14"><span class="linenos"> 14</span></a>
+</span><span id="L-15"><a href="#L-15"><span class="linenos"> 15</span></a><span class="sd">    :param package_path: Path to the package/project directory.</span>
 </span><span id="L-16"><a href="#L-16"><span class="linenos"> 16</span></a>
-</span><span id="L-17"><a href="#L-17"><span class="linenos"> 17</span></a><span class="sd">    :param package_path: Path to the package/project directory.</span>
-</span><span id="L-18"><a href="#L-18"><span class="linenos"> 18</span></a>
-</span><span id="L-19"><a href="#L-19"><span class="linenos"> 19</span></a><span class="sd">    :param increment_type: One from &#39;major&#39;, &#39;minor&#39;, or &#39;patch&#39;.&quot;&quot;&quot;</span>
-</span><span id="L-20"><a href="#L-20"><span class="linenos"> 20</span></a>    <span class="n">meta</span> <span class="o">=</span> <span class="n">tomlkit</span><span class="o">.</span><span class="n">loads</span><span class="p">(</span><span class="n">pyproject_path</span><span class="o">.</span><span class="n">read_text</span><span class="p">())</span>
-</span><span id="L-21"><a href="#L-21"><span class="linenos"> 21</span></a>    <span class="n">major</span><span class="p">,</span> <span class="n">minor</span><span class="p">,</span> <span class="n">patch</span> <span class="o">=</span> <span class="p">[</span><span class="nb">int</span><span class="p">(</span><span class="n">num</span><span class="p">)</span> <span class="k">for</span> <span class="n">num</span> <span class="ow">in</span> <span class="n">meta</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;version&quot;</span><span class="p">]</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;.&quot;</span><span class="p">)]</span>
-</span><span id="L-22"><a href="#L-22"><span class="linenos"> 22</span></a>    <span class="k">if</span> <span class="n">increment_type</span> <span class="o">==</span> <span class="s2">&quot;major&quot;</span><span class="p">:</span>
-</span><span id="L-23"><a href="#L-23"><span class="linenos"> 23</span></a>        <span class="n">major</span> <span class="o">+=</span> <span class="mi">1</span>
-</span><span id="L-24"><a href="#L-24"><span class="linenos"> 24</span></a>        <span class="n">minor</span> <span class="o">=</span> <span class="mi">0</span>
-</span><span id="L-25"><a href="#L-25"><span class="linenos"> 25</span></a>        <span class="n">patch</span> <span class="o">=</span> <span class="mi">0</span>
-</span><span id="L-26"><a href="#L-26"><span class="linenos"> 26</span></a>    <span class="k">elif</span> <span class="n">increment_type</span> <span class="o">==</span> <span class="s2">&quot;minor&quot;</span><span class="p">:</span>
-</span><span id="L-27"><a href="#L-27"><span class="linenos"> 27</span></a>        <span class="n">minor</span> <span class="o">+=</span> <span class="mi">1</span>
-</span><span id="L-28"><a href="#L-28"><span class="linenos"> 28</span></a>        <span class="n">patch</span> <span class="o">=</span> <span class="mi">0</span>
-</span><span id="L-29"><a href="#L-29"><span class="linenos"> 29</span></a>    <span class="k">elif</span> <span class="n">increment_type</span> <span class="o">==</span> <span class="s2">&quot;patch&quot;</span><span class="p">:</span>
-</span><span id="L-30"><a href="#L-30"><span class="linenos"> 30</span></a>        <span class="n">patch</span> <span class="o">+=</span> <span class="mi">1</span>
-</span><span id="L-31"><a href="#L-31"><span class="linenos"> 31</span></a>    <span class="n">incremented_version</span> <span class="o">=</span> <span class="s2">&quot;.&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="n">num</span><span class="p">)</span> <span class="k">for</span> <span class="n">num</span> <span class="ow">in</span> <span class="p">[</span><span class="n">major</span><span class="p">,</span> <span class="n">minor</span><span class="p">,</span> <span class="n">patch</span><span class="p">])</span>
-</span><span id="L-32"><a href="#L-32"><span class="linenos"> 32</span></a>    <span class="n">meta</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;version&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">incremented_version</span>
-</span><span id="L-33"><a href="#L-33"><span class="linenos"> 33</span></a>    <span class="n">pyproject_path</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="n">tomlkit</span><span class="o">.</span><span class="n">dumps</span><span class="p">(</span><span class="n">meta</span><span class="p">))</span>
-</span><span id="L-34"><a href="#L-34"><span class="linenos"> 34</span></a>
-</span><span id="L-35"><a href="#L-35"><span class="linenos"> 35</span></a>
-</span><span id="L-36"><a href="#L-36"><span class="linenos"> 36</span></a><span class="k">def</span> <span class="nf">update_minimum_python_version</span><span class="p">(</span><span class="n">pyproject_path</span><span class="p">:</span> <span class="n">Path</span><span class="p">):</span>
-</span><span id="L-37"><a href="#L-37"><span class="linenos"> 37</span></a>    <span class="sd">&quot;&quot;&quot;Use vermin to determine the minimum compatible</span>
-</span><span id="L-38"><a href="#L-38"><span class="linenos"> 38</span></a><span class="sd">    Python version and update the corresponding field</span>
-</span><span id="L-39"><a href="#L-39"><span class="linenos"> 39</span></a><span class="sd">    in pyproject.toml.&quot;&quot;&quot;</span>
-</span><span id="L-40"><a href="#L-40"><span class="linenos"> 40</span></a>    <span class="n">project_code</span> <span class="o">=</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span>
-</span><span id="L-41"><a href="#L-41"><span class="linenos"> 41</span></a>        <span class="n">file</span><span class="o">.</span><span class="n">read_text</span><span class="p">()</span> <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="p">(</span><span class="n">pyproject_path</span><span class="o">.</span><span class="n">parent</span> <span class="o">/</span> <span class="s2">&quot;src&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="s2">&quot;*.py&quot;</span><span class="p">)</span>
-</span><span id="L-42"><a href="#L-42"><span class="linenos"> 42</span></a>    <span class="p">)</span>
-</span><span id="L-43"><a href="#L-43"><span class="linenos"> 43</span></a>    <span class="n">meta</span> <span class="o">=</span> <span class="n">tomlkit</span><span class="o">.</span><span class="n">loads</span><span class="p">(</span><span class="n">pyproject_path</span><span class="o">.</span><span class="n">read_text</span><span class="p">())</span>
-</span><span id="L-44"><a href="#L-44"><span class="linenos"> 44</span></a>    <span class="n">minimum_version</span> <span class="o">=</span> <span class="n">vermin</span><span class="o">.</span><span class="n">visit</span><span class="p">(</span><span class="n">project_code</span><span class="p">,</span> <span class="n">vermin</span><span class="o">.</span><span class="n">Config</span><span class="p">())</span><span class="o">.</span><span class="n">minimum_versions</span><span class="p">()[</span><span class="mi">1</span><span class="p">]</span>
-</span><span id="L-45"><a href="#L-45"><span class="linenos"> 45</span></a>    <span class="n">minimum_version</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;&gt;=</span><span class="si">{</span><span class="n">minimum_version</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="si">}</span><span class="s2">.</span><span class="si">{</span><span class="n">minimum_version</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="L-46"><a href="#L-46"><span class="linenos"> 46</span></a>    <span class="n">meta</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;requires-python&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">minimum_version</span>
-</span><span id="L-47"><a href="#L-47"><span class="linenos"> 47</span></a>    <span class="n">pyproject_path</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="n">tomlkit</span><span class="o">.</span><span class="n">dumps</span><span class="p">(</span><span class="n">meta</span><span class="p">))</span>
-</span><span id="L-48"><a href="#L-48"><span class="linenos"> 48</span></a>
-</span><span id="L-49"><a href="#L-49"><span class="linenos"> 49</span></a>
-</span><span id="L-50"><a href="#L-50"><span class="linenos"> 50</span></a><span class="k">def</span> <span class="nf">generate_docs</span><span class="p">(</span><span class="n">package_path</span><span class="p">:</span> <span class="n">Path</span><span class="p">):</span>
-</span><span id="L-51"><a href="#L-51"><span class="linenos"> 51</span></a>    <span class="sd">&quot;&quot;&quot;Generate project documentation using pdoc.&quot;&quot;&quot;</span>
-</span><span id="L-52"><a href="#L-52"><span class="linenos"> 52</span></a>    <span class="k">try</span><span class="p">:</span>
-</span><span id="L-53"><a href="#L-53"><span class="linenos"> 53</span></a>        <span class="n">shutil</span><span class="o">.</span><span class="n">rmtree</span><span class="p">(</span><span class="n">package_path</span> <span class="o">/</span> <span class="s2">&quot;docs&quot;</span><span class="p">)</span>
-</span><span id="L-54"><a href="#L-54"><span class="linenos"> 54</span></a>    <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="L-55"><a href="#L-55"><span class="linenos"> 55</span></a>        <span class="k">pass</span>
-</span><span id="L-56"><a href="#L-56"><span class="linenos"> 56</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span>
-</span><span id="L-57"><a href="#L-57"><span class="linenos"> 57</span></a>        <span class="sa">f</span><span class="s2">&quot;pdoc -o </span><span class="si">{</span><span class="n">package_path</span> <span class="o">/</span> <span class="s1">&#39;docs&#39;</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">package_path</span> <span class="o">/</span> <span class="s1">&#39;src&#39;</span> <span class="o">/</span> <span class="n">package_path</span><span class="o">.</span><span class="n">stem</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="L-58"><a href="#L-58"><span class="linenos"> 58</span></a>    <span class="p">)</span>
-</span><span id="L-59"><a href="#L-59"><span class="linenos"> 59</span></a>
-</span><span id="L-60"><a href="#L-60"><span class="linenos"> 60</span></a>
-</span><span id="L-61"><a href="#L-61"><span class="linenos"> 61</span></a><span class="k">def</span> <span class="nf">update_dependencies</span><span class="p">(</span>
-</span><span id="L-62"><a href="#L-62"><span class="linenos"> 62</span></a>    <span class="n">pyproject_path</span><span class="p">:</span> <span class="n">Path</span><span class="p">,</span> <span class="n">overwrite</span><span class="p">:</span> <span class="nb">bool</span><span class="p">,</span> <span class="n">include_versions</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>
-</span><span id="L-63"><a href="#L-63"><span class="linenos"> 63</span></a><span class="p">):</span>
-</span><span id="L-64"><a href="#L-64"><span class="linenos"> 64</span></a>    <span class="sd">&quot;&quot;&quot;Update dependencies list in pyproject.toml.</span>
-</span><span id="L-65"><a href="#L-65"><span class="linenos"> 65</span></a>
-</span><span id="L-66"><a href="#L-66"><span class="linenos"> 66</span></a><span class="sd">    :param overwrite: If True, replace the dependencies in pyproject.toml</span>
-</span><span id="L-67"><a href="#L-67"><span class="linenos"> 67</span></a><span class="sd">    with the results of packagelister.scan() .</span>
-</span><span id="L-68"><a href="#L-68"><span class="linenos"> 68</span></a><span class="sd">    If False, packages returned by packagelister are appended to</span>
-</span><span id="L-69"><a href="#L-69"><span class="linenos"> 69</span></a><span class="sd">    the current dependencies in pyproject.toml if they don&#39;t already</span>
-</span><span id="L-70"><a href="#L-70"><span class="linenos"> 70</span></a><span class="sd">    exist in the field.&quot;&quot;&quot;</span>
-</span><span id="L-71"><a href="#L-71"><span class="linenos"> 71</span></a>    <span class="n">packages</span> <span class="o">=</span> <span class="n">packagelister</span><span class="o">.</span><span class="n">scan</span><span class="p">(</span><span class="n">pyproject_path</span><span class="o">.</span><span class="n">parent</span><span class="p">)</span>
-</span><span id="L-72"><a href="#L-72"><span class="linenos"> 72</span></a>
-</span><span id="L-73"><a href="#L-73"><span class="linenos"> 73</span></a>    <span class="n">packages</span> <span class="o">=</span> <span class="p">[</span>
-</span><span id="L-74"><a href="#L-74"><span class="linenos"> 74</span></a>        <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">package</span><span class="si">}</span><span class="s2">~=</span><span class="si">{</span><span class="n">packages</span><span class="p">[</span><span class="n">package</span><span class="p">][</span><span class="s1">&#39;version&#39;</span><span class="p">]</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="L-75"><a href="#L-75"><span class="linenos"> 75</span></a>        <span class="k">if</span> <span class="n">packages</span><span class="p">[</span><span class="n">package</span><span class="p">][</span><span class="s2">&quot;version&quot;</span><span class="p">]</span> <span class="ow">and</span> <span class="n">include_versions</span>
-</span><span id="L-76"><a href="#L-76"><span class="linenos"> 76</span></a>        <span class="k">else</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">package</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="L-77"><a href="#L-77"><span class="linenos"> 77</span></a>        <span class="k">for</span> <span class="n">package</span> <span class="ow">in</span> <span class="n">packages</span>
-</span><span id="L-78"><a href="#L-78"><span class="linenos"> 78</span></a>        <span class="k">if</span> <span class="n">package</span> <span class="o">!=</span> <span class="n">pyproject_path</span><span class="o">.</span><span class="n">parent</span><span class="o">.</span><span class="n">stem</span>
-</span><span id="L-79"><a href="#L-79"><span class="linenos"> 79</span></a>    <span class="p">]</span>
-</span><span id="L-80"><a href="#L-80"><span class="linenos"> 80</span></a>    <span class="n">packages</span> <span class="o">=</span> <span class="p">[</span>
-</span><span id="L-81"><a href="#L-81"><span class="linenos"> 81</span></a>        <span class="n">package</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;speech_recognition&quot;</span><span class="p">,</span> <span class="s2">&quot;speechRecognition&quot;</span><span class="p">)</span>
-</span><span id="L-82"><a href="#L-82"><span class="linenos"> 82</span></a>        <span class="k">for</span> <span class="n">package</span> <span class="ow">in</span> <span class="n">packages</span>
-</span><span id="L-83"><a href="#L-83"><span class="linenos"> 83</span></a>    <span class="p">]</span>
-</span><span id="L-84"><a href="#L-84"><span class="linenos"> 84</span></a>    <span class="n">meta</span> <span class="o">=</span> <span class="n">tomlkit</span><span class="o">.</span><span class="n">loads</span><span class="p">(</span><span class="n">pyproject_path</span><span class="o">.</span><span class="n">read_text</span><span class="p">())</span>
-</span><span id="L-85"><a href="#L-85"><span class="linenos"> 85</span></a>    <span class="k">if</span> <span class="n">overwrite</span><span class="p">:</span>
-</span><span id="L-86"><a href="#L-86"><span class="linenos"> 86</span></a>        <span class="n">meta</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;dependencies&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">packages</span>
-</span><span id="L-87"><a href="#L-87"><span class="linenos"> 87</span></a>    <span class="k">else</span><span class="p">:</span>
-</span><span id="L-88"><a href="#L-88"><span class="linenos"> 88</span></a>        <span class="k">for</span> <span class="n">package</span> <span class="ow">in</span> <span class="n">packages</span><span class="p">:</span>
-</span><span id="L-89"><a href="#L-89"><span class="linenos"> 89</span></a>            <span class="k">if</span> <span class="s2">&quot;~&quot;</span> <span class="ow">in</span> <span class="n">package</span><span class="p">:</span>
-</span><span id="L-90"><a href="#L-90"><span class="linenos"> 90</span></a>                <span class="n">name</span> <span class="o">=</span> <span class="n">package</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;~&quot;</span><span class="p">)[</span><span class="mi">0</span><span class="p">]</span>
-</span><span id="L-91"><a href="#L-91"><span class="linenos"> 91</span></a>            <span class="k">elif</span> <span class="s2">&quot;=&quot;</span> <span class="ow">in</span> <span class="n">package</span><span class="p">:</span>
-</span><span id="L-92"><a href="#L-92"><span class="linenos"> 92</span></a>                <span class="n">name</span> <span class="o">=</span> <span class="n">package</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;=&quot;</span><span class="p">)[</span><span class="mi">0</span><span class="p">]</span>
-</span><span id="L-93"><a href="#L-93"><span class="linenos"> 93</span></a>            <span class="k">else</span><span class="p">:</span>
-</span><span id="L-94"><a href="#L-94"><span class="linenos"> 94</span></a>                <span class="n">name</span> <span class="o">=</span> <span class="n">package</span>
-</span><span id="L-95"><a href="#L-95"><span class="linenos"> 95</span></a>            <span class="k">if</span> <span class="nb">all</span><span class="p">(</span>
-</span><span id="L-96"><a href="#L-96"><span class="linenos"> 96</span></a>                <span class="n">name</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">dependency</span> <span class="k">for</span> <span class="n">dependency</span> <span class="ow">in</span> <span class="n">meta</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;dependencies&quot;</span><span class="p">]</span>
-</span><span id="L-97"><a href="#L-97"><span class="linenos"> 97</span></a>            <span class="p">):</span>
-</span><span id="L-98"><a href="#L-98"><span class="linenos"> 98</span></a>                <span class="n">meta</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;dependencies&quot;</span><span class="p">]</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">package</span><span class="p">)</span>
-</span><span id="L-99"><a href="#L-99"><span class="linenos"> 99</span></a>    <span class="n">pyproject_path</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="n">tomlkit</span><span class="o">.</span><span class="n">dumps</span><span class="p">(</span><span class="n">meta</span><span class="p">))</span>
-</span><span id="L-100"><a href="#L-100"><span class="linenos">100</span></a>
-</span><span id="L-101"><a href="#L-101"><span class="linenos">101</span></a>
-</span><span id="L-102"><a href="#L-102"><span class="linenos">102</span></a><span class="k">def</span> <span class="nf">update_changelog</span><span class="p">(</span><span class="n">pyproject_path</span><span class="p">:</span> <span class="n">Path</span><span class="p">):</span>
-</span><span id="L-103"><a href="#L-103"><span class="linenos">103</span></a>    <span class="sd">&quot;&quot;&quot;Update project changelog.&quot;&quot;&quot;</span>
-</span><span id="L-104"><a href="#L-104"><span class="linenos">104</span></a>    <span class="n">meta</span> <span class="o">=</span> <span class="n">tomlkit</span><span class="o">.</span><span class="n">loads</span><span class="p">(</span><span class="n">pyproject_path</span><span class="o">.</span><span class="n">read_text</span><span class="p">())</span>
-</span><span id="L-105"><a href="#L-105"><span class="linenos">105</span></a>    <span class="k">if</span> <span class="n">hassle_config</span><span class="o">.</span><span class="n">config_exists</span><span class="p">():</span>
-</span><span id="L-106"><a href="#L-106"><span class="linenos">106</span></a>        <span class="n">config</span> <span class="o">=</span> <span class="n">hassle_config</span><span class="o">.</span><span class="n">load_config</span><span class="p">()</span>
-</span><span id="L-107"><a href="#L-107"><span class="linenos">107</span></a>    <span class="k">else</span><span class="p">:</span>
-</span><span id="L-108"><a href="#L-108"><span class="linenos">108</span></a>        <span class="n">hassle_config</span><span class="o">.</span><span class="n">warn</span><span class="p">()</span>
-</span><span id="L-109"><a href="#L-109"><span class="linenos">109</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Creating blank hassle_config.toml...&quot;</span><span class="p">)</span>
-</span><span id="L-110"><a href="#L-110"><span class="linenos">110</span></a>        <span class="n">config</span> <span class="o">=</span> <span class="n">hassle_config</span><span class="o">.</span><span class="n">load_config</span><span class="p">()</span>
-</span><span id="L-111"><a href="#L-111"><span class="linenos">111</span></a>    <span class="n">changelog_path</span> <span class="o">=</span> <span class="n">pyproject_path</span><span class="o">.</span><span class="n">parent</span> <span class="o">/</span> <span class="s2">&quot;CHANGELOG.md&quot;</span>
-</span><span id="L-112"><a href="#L-112"><span class="linenos">112</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span>
-</span><span id="L-113"><a href="#L-113"><span class="linenos">113</span></a>        <span class="sa">f</span><span class="s2">&quot;auto-changelog -p </span><span class="si">{</span><span class="n">pyproject_path</span><span class="o">.</span><span class="n">parent</span><span class="si">}</span><span class="s2"> --tag-prefix </span><span class="si">{</span><span class="n">config</span><span class="p">[</span><span class="s1">&#39;git&#39;</span><span class="p">][</span><span class="s1">&#39;tag_prefix&#39;</span><span class="p">]</span><span class="si">}</span><span class="s2"> --unreleased -v </span><span class="si">{</span><span class="n">meta</span><span class="p">[</span><span class="s1">&#39;project&#39;</span><span class="p">][</span><span class="s1">&#39;version&#39;</span><span class="p">]</span><span class="si">}</span><span class="s2"> -o </span><span class="si">{</span><span class="n">changelog_path</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="L-114"><a href="#L-114"><span class="linenos">114</span></a>    <span class="p">)</span>
-</span><span id="L-115"><a href="#L-115"><span class="linenos">115</span></a>    <span class="n">changelog</span> <span class="o">=</span> <span class="n">changelog_path</span><span class="o">.</span><span class="n">read_text</span><span class="p">()</span><span class="o">.</span><span class="n">splitlines</span><span class="p">()</span>
-</span><span id="L-116"><a href="#L-116"><span class="linenos">116</span></a>    <span class="n">changelog</span> <span class="o">=</span> <span class="p">[</span><span class="n">line</span> <span class="k">for</span> <span class="n">line</span> <span class="ow">in</span> <span class="n">changelog</span> <span class="k">if</span> <span class="s2">&quot;Full set of changes:&quot;</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">line</span><span class="p">]</span>
-</span><span id="L-117"><a href="#L-117"><span class="linenos">117</span></a>    <span class="n">changelog_path</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">changelog</span><span class="p">))</span>
-</span><span id="L-118"><a href="#L-118"><span class="linenos">118</span></a>
-</span><span id="L-119"><a href="#L-119"><span class="linenos">119</span></a>
-</span><span id="L-120"><a href="#L-120"><span class="linenos">120</span></a><span class="k">def</span> <span class="nf">tag_version</span><span class="p">(</span><span class="n">package_path</span><span class="p">:</span> <span class="n">Path</span><span class="p">):</span>
-</span><span id="L-121"><a href="#L-121"><span class="linenos">121</span></a>    <span class="sd">&quot;&quot;&quot;Add a git tag corresponding</span>
-</span><span id="L-122"><a href="#L-122"><span class="linenos">122</span></a><span class="sd">    to the version number in pyproject.toml.&quot;&quot;&quot;</span>
-</span><span id="L-123"><a href="#L-123"><span class="linenos">123</span></a>    <span class="k">if</span> <span class="n">hassle_config</span><span class="o">.</span><span class="n">config_exists</span><span class="p">():</span>
-</span><span id="L-124"><a href="#L-124"><span class="linenos">124</span></a>        <span class="n">tag_prefix</span> <span class="o">=</span> <span class="n">hassle_config</span><span class="o">.</span><span class="n">load_config</span><span class="p">()[</span><span class="s2">&quot;git&quot;</span><span class="p">][</span><span class="s2">&quot;tag_prefix&quot;</span><span class="p">]</span>
-</span><span id="L-125"><a href="#L-125"><span class="linenos">125</span></a>    <span class="k">else</span><span class="p">:</span>
-</span><span id="L-126"><a href="#L-126"><span class="linenos">126</span></a>        <span class="n">hassle_config</span><span class="o">.</span><span class="n">warn</span><span class="p">()</span>
-</span><span id="L-127"><a href="#L-127"><span class="linenos">127</span></a>        <span class="n">tag_prefix</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
-</span><span id="L-128"><a href="#L-128"><span class="linenos">128</span></a>    <span class="n">version</span> <span class="o">=</span> <span class="n">tomlkit</span><span class="o">.</span><span class="n">loads</span><span class="p">((</span><span class="n">package_path</span> <span class="o">/</span> <span class="s2">&quot;pyproject.toml&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">read_text</span><span class="p">())[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span>
-</span><span id="L-129"><a href="#L-129"><span class="linenos">129</span></a>        <span class="s2">&quot;version&quot;</span>
-</span><span id="L-130"><a href="#L-130"><span class="linenos">130</span></a>    <span class="p">]</span>
-</span><span id="L-131"><a href="#L-131"><span class="linenos">131</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">package_path</span><span class="p">)</span>
-</span><span id="L-132"><a href="#L-132"><span class="linenos">132</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;git tag </span><span class="si">{</span><span class="n">tag_prefix</span><span class="si">}{</span><span class="n">version</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-17"><a href="#L-17"><span class="linenos"> 17</span></a><span class="sd">    :param increment_type: One from &#39;major&#39;, &#39;minor&#39;, or &#39;patch&#39;.&quot;&quot;&quot;</span>
+</span><span id="L-18"><a href="#L-18"><span class="linenos"> 18</span></a>    <span class="n">meta</span> <span class="o">=</span> <span class="n">pyproject_path</span><span class="o">.</span><span class="n">loads</span><span class="p">()</span>
+</span><span id="L-19"><a href="#L-19"><span class="linenos"> 19</span></a>    <span class="n">major</span><span class="p">,</span> <span class="n">minor</span><span class="p">,</span> <span class="n">patch</span> <span class="o">=</span> <span class="p">[</span><span class="nb">int</span><span class="p">(</span><span class="n">num</span><span class="p">)</span> <span class="k">for</span> <span class="n">num</span> <span class="ow">in</span> <span class="n">meta</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;version&quot;</span><span class="p">]</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;.&quot;</span><span class="p">)]</span>
+</span><span id="L-20"><a href="#L-20"><span class="linenos"> 20</span></a>    <span class="k">if</span> <span class="n">increment_type</span> <span class="o">==</span> <span class="s2">&quot;major&quot;</span><span class="p">:</span>
+</span><span id="L-21"><a href="#L-21"><span class="linenos"> 21</span></a>        <span class="n">major</span> <span class="o">+=</span> <span class="mi">1</span>
+</span><span id="L-22"><a href="#L-22"><span class="linenos"> 22</span></a>        <span class="n">minor</span> <span class="o">=</span> <span class="mi">0</span>
+</span><span id="L-23"><a href="#L-23"><span class="linenos"> 23</span></a>        <span class="n">patch</span> <span class="o">=</span> <span class="mi">0</span>
+</span><span id="L-24"><a href="#L-24"><span class="linenos"> 24</span></a>    <span class="k">elif</span> <span class="n">increment_type</span> <span class="o">==</span> <span class="s2">&quot;minor&quot;</span><span class="p">:</span>
+</span><span id="L-25"><a href="#L-25"><span class="linenos"> 25</span></a>        <span class="n">minor</span> <span class="o">+=</span> <span class="mi">1</span>
+</span><span id="L-26"><a href="#L-26"><span class="linenos"> 26</span></a>        <span class="n">patch</span> <span class="o">=</span> <span class="mi">0</span>
+</span><span id="L-27"><a href="#L-27"><span class="linenos"> 27</span></a>    <span class="k">elif</span> <span class="n">increment_type</span> <span class="o">==</span> <span class="s2">&quot;patch&quot;</span><span class="p">:</span>
+</span><span id="L-28"><a href="#L-28"><span class="linenos"> 28</span></a>        <span class="n">patch</span> <span class="o">+=</span> <span class="mi">1</span>
+</span><span id="L-29"><a href="#L-29"><span class="linenos"> 29</span></a>    <span class="n">incremented_version</span> <span class="o">=</span> <span class="s2">&quot;.&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="n">num</span><span class="p">)</span> <span class="k">for</span> <span class="n">num</span> <span class="ow">in</span> <span class="p">[</span><span class="n">major</span><span class="p">,</span> <span class="n">minor</span><span class="p">,</span> <span class="n">patch</span><span class="p">])</span>
+</span><span id="L-30"><a href="#L-30"><span class="linenos"> 30</span></a>    <span class="n">meta</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;version&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">incremented_version</span>
+</span><span id="L-31"><a href="#L-31"><span class="linenos"> 31</span></a>    <span class="n">pyproject_path</span><span class="o">.</span><span class="n">dumps</span><span class="p">(</span><span class="n">meta</span><span class="p">)</span>
+</span><span id="L-32"><a href="#L-32"><span class="linenos"> 32</span></a>
+</span><span id="L-33"><a href="#L-33"><span class="linenos"> 33</span></a>
+</span><span id="L-34"><a href="#L-34"><span class="linenos"> 34</span></a><span class="k">def</span> <span class="nf">update_minimum_python_version</span><span class="p">(</span><span class="n">pyproject_path</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">):</span>
+</span><span id="L-35"><a href="#L-35"><span class="linenos"> 35</span></a>    <span class="sd">&quot;&quot;&quot;Use vermin to determine the minimum compatible</span>
+</span><span id="L-36"><a href="#L-36"><span class="linenos"> 36</span></a><span class="sd">    Python version and update the corresponding field</span>
+</span><span id="L-37"><a href="#L-37"><span class="linenos"> 37</span></a><span class="sd">    in pyproject.toml.&quot;&quot;&quot;</span>
+</span><span id="L-38"><a href="#L-38"><span class="linenos"> 38</span></a>    <span class="n">project_code</span> <span class="o">=</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span>
+</span><span id="L-39"><a href="#L-39"><span class="linenos"> 39</span></a>        <span class="n">file</span><span class="o">.</span><span class="n">read_text</span><span class="p">()</span> <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="p">(</span><span class="n">pyproject_path</span><span class="o">.</span><span class="n">parent</span> <span class="o">/</span> <span class="s2">&quot;src&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="s2">&quot;*.py&quot;</span><span class="p">)</span>
+</span><span id="L-40"><a href="#L-40"><span class="linenos"> 40</span></a>    <span class="p">)</span>
+</span><span id="L-41"><a href="#L-41"><span class="linenos"> 41</span></a>    <span class="n">meta</span> <span class="o">=</span> <span class="n">pyproject_path</span><span class="o">.</span><span class="n">loads</span><span class="p">()</span>
+</span><span id="L-42"><a href="#L-42"><span class="linenos"> 42</span></a>    <span class="n">minimum_version</span> <span class="o">=</span> <span class="n">vermin</span><span class="o">.</span><span class="n">visit</span><span class="p">(</span><span class="n">project_code</span><span class="p">,</span> <span class="n">vermin</span><span class="o">.</span><span class="n">Config</span><span class="p">())</span><span class="o">.</span><span class="n">minimum_versions</span><span class="p">()[</span><span class="mi">1</span><span class="p">]</span>
+</span><span id="L-43"><a href="#L-43"><span class="linenos"> 43</span></a>    <span class="n">minimum_version</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;&gt;=</span><span class="si">{</span><span class="n">minimum_version</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="si">}</span><span class="s2">.</span><span class="si">{</span><span class="n">minimum_version</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="L-44"><a href="#L-44"><span class="linenos"> 44</span></a>    <span class="n">meta</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;requires-python&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">minimum_version</span>
+</span><span id="L-45"><a href="#L-45"><span class="linenos"> 45</span></a>    <span class="n">pyproject_path</span><span class="o">.</span><span class="n">dumps</span><span class="p">(</span><span class="n">meta</span><span class="p">)</span>
+</span><span id="L-46"><a href="#L-46"><span class="linenos"> 46</span></a>
+</span><span id="L-47"><a href="#L-47"><span class="linenos"> 47</span></a>
+</span><span id="L-48"><a href="#L-48"><span class="linenos"> 48</span></a><span class="k">def</span> <span class="nf">generate_docs</span><span class="p">(</span><span class="n">package_path</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">):</span>
+</span><span id="L-49"><a href="#L-49"><span class="linenos"> 49</span></a>    <span class="sd">&quot;&quot;&quot;Generate project documentation using pdoc.&quot;&quot;&quot;</span>
+</span><span id="L-50"><a href="#L-50"><span class="linenos"> 50</span></a>    <span class="k">try</span><span class="p">:</span>
+</span><span id="L-51"><a href="#L-51"><span class="linenos"> 51</span></a>        <span class="p">(</span><span class="n">package_path</span> <span class="o">/</span> <span class="s2">&quot;docs&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">delete</span><span class="p">()</span>
+</span><span id="L-52"><a href="#L-52"><span class="linenos"> 52</span></a>    <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="L-53"><a href="#L-53"><span class="linenos"> 53</span></a>        <span class="k">pass</span>
+</span><span id="L-54"><a href="#L-54"><span class="linenos"> 54</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span>
+</span><span id="L-55"><a href="#L-55"><span class="linenos"> 55</span></a>        <span class="sa">f</span><span class="s2">&quot;pdoc -o </span><span class="si">{</span><span class="n">package_path</span> <span class="o">/</span> <span class="s1">&#39;docs&#39;</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">package_path</span> <span class="o">/</span> <span class="s1">&#39;src&#39;</span> <span class="o">/</span> <span class="n">package_path</span><span class="o">.</span><span class="n">stem</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="L-56"><a href="#L-56"><span class="linenos"> 56</span></a>    <span class="p">)</span>
+</span><span id="L-57"><a href="#L-57"><span class="linenos"> 57</span></a>
+</span><span id="L-58"><a href="#L-58"><span class="linenos"> 58</span></a>
+</span><span id="L-59"><a href="#L-59"><span class="linenos"> 59</span></a><span class="k">def</span> <span class="nf">update_dependencies</span><span class="p">(</span>
+</span><span id="L-60"><a href="#L-60"><span class="linenos"> 60</span></a>    <span class="n">pyproject_path</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">,</span> <span class="n">overwrite</span><span class="p">:</span> <span class="nb">bool</span><span class="p">,</span> <span class="n">include_versions</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>
+</span><span id="L-61"><a href="#L-61"><span class="linenos"> 61</span></a><span class="p">):</span>
+</span><span id="L-62"><a href="#L-62"><span class="linenos"> 62</span></a>    <span class="sd">&quot;&quot;&quot;Update dependencies list in pyproject.toml.</span>
+</span><span id="L-63"><a href="#L-63"><span class="linenos"> 63</span></a>
+</span><span id="L-64"><a href="#L-64"><span class="linenos"> 64</span></a><span class="sd">    :param overwrite: If True, replace the dependencies in pyproject.toml</span>
+</span><span id="L-65"><a href="#L-65"><span class="linenos"> 65</span></a><span class="sd">    with the results of packagelister.scan() .</span>
+</span><span id="L-66"><a href="#L-66"><span class="linenos"> 66</span></a><span class="sd">    If False, packages returned by packagelister are appended to</span>
+</span><span id="L-67"><a href="#L-67"><span class="linenos"> 67</span></a><span class="sd">    the current dependencies in pyproject.toml if they don&#39;t already</span>
+</span><span id="L-68"><a href="#L-68"><span class="linenos"> 68</span></a><span class="sd">    exist in the field.&quot;&quot;&quot;</span>
+</span><span id="L-69"><a href="#L-69"><span class="linenos"> 69</span></a>    <span class="n">packages</span> <span class="o">=</span> <span class="n">packagelister</span><span class="o">.</span><span class="n">scan</span><span class="p">(</span><span class="n">pyproject_path</span><span class="o">.</span><span class="n">parent</span><span class="p">)</span>
+</span><span id="L-70"><a href="#L-70"><span class="linenos"> 70</span></a>
+</span><span id="L-71"><a href="#L-71"><span class="linenos"> 71</span></a>    <span class="n">packages</span> <span class="o">=</span> <span class="p">[</span>
+</span><span id="L-72"><a href="#L-72"><span class="linenos"> 72</span></a>        <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">package</span><span class="si">}</span><span class="s2">~=</span><span class="si">{</span><span class="n">packages</span><span class="p">[</span><span class="n">package</span><span class="p">][</span><span class="s1">&#39;version&#39;</span><span class="p">]</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="L-73"><a href="#L-73"><span class="linenos"> 73</span></a>        <span class="k">if</span> <span class="n">packages</span><span class="p">[</span><span class="n">package</span><span class="p">][</span><span class="s2">&quot;version&quot;</span><span class="p">]</span> <span class="ow">and</span> <span class="n">include_versions</span>
+</span><span id="L-74"><a href="#L-74"><span class="linenos"> 74</span></a>        <span class="k">else</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">package</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="L-75"><a href="#L-75"><span class="linenos"> 75</span></a>        <span class="k">for</span> <span class="n">package</span> <span class="ow">in</span> <span class="n">packages</span>
+</span><span id="L-76"><a href="#L-76"><span class="linenos"> 76</span></a>        <span class="k">if</span> <span class="n">package</span> <span class="o">!=</span> <span class="n">pyproject_path</span><span class="o">.</span><span class="n">parent</span><span class="o">.</span><span class="n">stem</span>
+</span><span id="L-77"><a href="#L-77"><span class="linenos"> 77</span></a>    <span class="p">]</span>
+</span><span id="L-78"><a href="#L-78"><span class="linenos"> 78</span></a>    <span class="n">packages</span> <span class="o">=</span> <span class="p">[</span>
+</span><span id="L-79"><a href="#L-79"><span class="linenos"> 79</span></a>        <span class="n">package</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;speech_recognition&quot;</span><span class="p">,</span> <span class="s2">&quot;speechRecognition&quot;</span><span class="p">)</span>
+</span><span id="L-80"><a href="#L-80"><span class="linenos"> 80</span></a>        <span class="k">for</span> <span class="n">package</span> <span class="ow">in</span> <span class="n">packages</span>
+</span><span id="L-81"><a href="#L-81"><span class="linenos"> 81</span></a>    <span class="p">]</span>
+</span><span id="L-82"><a href="#L-82"><span class="linenos"> 82</span></a>    <span class="n">meta</span> <span class="o">=</span> <span class="n">pyproject_path</span><span class="o">.</span><span class="n">loads</span><span class="p">()</span>
+</span><span id="L-83"><a href="#L-83"><span class="linenos"> 83</span></a>    <span class="k">if</span> <span class="n">overwrite</span><span class="p">:</span>
+</span><span id="L-84"><a href="#L-84"><span class="linenos"> 84</span></a>        <span class="n">meta</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;dependencies&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">packages</span>
+</span><span id="L-85"><a href="#L-85"><span class="linenos"> 85</span></a>    <span class="k">else</span><span class="p">:</span>
+</span><span id="L-86"><a href="#L-86"><span class="linenos"> 86</span></a>        <span class="k">for</span> <span class="n">package</span> <span class="ow">in</span> <span class="n">packages</span><span class="p">:</span>
+</span><span id="L-87"><a href="#L-87"><span class="linenos"> 87</span></a>            <span class="k">if</span> <span class="s2">&quot;~&quot;</span> <span class="ow">in</span> <span class="n">package</span><span class="p">:</span>
+</span><span id="L-88"><a href="#L-88"><span class="linenos"> 88</span></a>                <span class="n">name</span> <span class="o">=</span> <span class="n">package</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;~&quot;</span><span class="p">)[</span><span class="mi">0</span><span class="p">]</span>
+</span><span id="L-89"><a href="#L-89"><span class="linenos"> 89</span></a>            <span class="k">elif</span> <span class="s2">&quot;=&quot;</span> <span class="ow">in</span> <span class="n">package</span><span class="p">:</span>
+</span><span id="L-90"><a href="#L-90"><span class="linenos"> 90</span></a>                <span class="n">name</span> <span class="o">=</span> <span class="n">package</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;=&quot;</span><span class="p">)[</span><span class="mi">0</span><span class="p">]</span>
+</span><span id="L-91"><a href="#L-91"><span class="linenos"> 91</span></a>            <span class="k">else</span><span class="p">:</span>
+</span><span id="L-92"><a href="#L-92"><span class="linenos"> 92</span></a>                <span class="n">name</span> <span class="o">=</span> <span class="n">package</span>
+</span><span id="L-93"><a href="#L-93"><span class="linenos"> 93</span></a>            <span class="k">if</span> <span class="nb">all</span><span class="p">(</span>
+</span><span id="L-94"><a href="#L-94"><span class="linenos"> 94</span></a>                <span class="n">name</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">dependency</span> <span class="k">for</span> <span class="n">dependency</span> <span class="ow">in</span> <span class="n">meta</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;dependencies&quot;</span><span class="p">]</span>
+</span><span id="L-95"><a href="#L-95"><span class="linenos"> 95</span></a>            <span class="p">):</span>
+</span><span id="L-96"><a href="#L-96"><span class="linenos"> 96</span></a>                <span class="n">meta</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;dependencies&quot;</span><span class="p">]</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">package</span><span class="p">)</span>
+</span><span id="L-97"><a href="#L-97"><span class="linenos"> 97</span></a>    <span class="n">pyproject_path</span><span class="o">.</span><span class="n">dumps</span><span class="p">(</span><span class="n">meta</span><span class="p">)</span>
+</span><span id="L-98"><a href="#L-98"><span class="linenos"> 98</span></a>
+</span><span id="L-99"><a href="#L-99"><span class="linenos"> 99</span></a>
+</span><span id="L-100"><a href="#L-100"><span class="linenos">100</span></a><span class="k">def</span> <span class="nf">update_changelog</span><span class="p">(</span><span class="n">pyproject_path</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">):</span>
+</span><span id="L-101"><a href="#L-101"><span class="linenos">101</span></a>    <span class="sd">&quot;&quot;&quot;Update project changelog.&quot;&quot;&quot;</span>
+</span><span id="L-102"><a href="#L-102"><span class="linenos">102</span></a>    <span class="n">meta</span> <span class="o">=</span> <span class="n">pyproject_path</span><span class="o">.</span><span class="n">loads</span><span class="p">()</span>
+</span><span id="L-103"><a href="#L-103"><span class="linenos">103</span></a>    <span class="k">if</span> <span class="n">hassle_config</span><span class="o">.</span><span class="n">config_exists</span><span class="p">():</span>
+</span><span id="L-104"><a href="#L-104"><span class="linenos">104</span></a>        <span class="n">config</span> <span class="o">=</span> <span class="n">hassle_config</span><span class="o">.</span><span class="n">load_config</span><span class="p">()</span>
+</span><span id="L-105"><a href="#L-105"><span class="linenos">105</span></a>    <span class="k">else</span><span class="p">:</span>
+</span><span id="L-106"><a href="#L-106"><span class="linenos">106</span></a>        <span class="n">hassle_config</span><span class="o">.</span><span class="n">warn</span><span class="p">()</span>
+</span><span id="L-107"><a href="#L-107"><span class="linenos">107</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Creating blank hassle_config.toml...&quot;</span><span class="p">)</span>
+</span><span id="L-108"><a href="#L-108"><span class="linenos">108</span></a>        <span class="n">config</span> <span class="o">=</span> <span class="n">hassle_config</span><span class="o">.</span><span class="n">load_config</span><span class="p">()</span>
+</span><span id="L-109"><a href="#L-109"><span class="linenos">109</span></a>    <span class="n">changelog_path</span> <span class="o">=</span> <span class="n">pyproject_path</span><span class="o">.</span><span class="n">parent</span> <span class="o">/</span> <span class="s2">&quot;CHANGELOG.md&quot;</span>
+</span><span id="L-110"><a href="#L-110"><span class="linenos">110</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span>
+</span><span id="L-111"><a href="#L-111"><span class="linenos">111</span></a>        <span class="sa">f</span><span class="s2">&quot;auto-changelog -p </span><span class="si">{</span><span class="n">pyproject_path</span><span class="o">.</span><span class="n">parent</span><span class="si">}</span><span class="s2"> --tag-prefix </span><span class="si">{</span><span class="n">config</span><span class="p">[</span><span class="s1">&#39;git&#39;</span><span class="p">][</span><span class="s1">&#39;tag_prefix&#39;</span><span class="p">]</span><span class="si">}</span><span class="s2"> --unreleased -v </span><span class="si">{</span><span class="n">meta</span><span class="p">[</span><span class="s1">&#39;project&#39;</span><span class="p">][</span><span class="s1">&#39;version&#39;</span><span class="p">]</span><span class="si">}</span><span class="s2"> -o </span><span class="si">{</span><span class="n">changelog_path</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="L-112"><a href="#L-112"><span class="linenos">112</span></a>    <span class="p">)</span>
+</span><span id="L-113"><a href="#L-113"><span class="linenos">113</span></a>    <span class="n">changelog</span> <span class="o">=</span> <span class="n">changelog_path</span><span class="o">.</span><span class="n">read_text</span><span class="p">()</span><span class="o">.</span><span class="n">splitlines</span><span class="p">()</span>
+</span><span id="L-114"><a href="#L-114"><span class="linenos">114</span></a>    <span class="n">changelog</span> <span class="o">=</span> <span class="p">[</span><span class="n">line</span> <span class="k">for</span> <span class="n">line</span> <span class="ow">in</span> <span class="n">changelog</span> <span class="k">if</span> <span class="s2">&quot;Full set of changes:&quot;</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">line</span><span class="p">]</span>
+</span><span id="L-115"><a href="#L-115"><span class="linenos">115</span></a>    <span class="n">changelog_path</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">changelog</span><span class="p">))</span>
+</span><span id="L-116"><a href="#L-116"><span class="linenos">116</span></a>
+</span><span id="L-117"><a href="#L-117"><span class="linenos">117</span></a>
+</span><span id="L-118"><a href="#L-118"><span class="linenos">118</span></a><span class="k">def</span> <span class="nf">tag_version</span><span class="p">(</span><span class="n">package_path</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">):</span>
+</span><span id="L-119"><a href="#L-119"><span class="linenos">119</span></a>    <span class="sd">&quot;&quot;&quot;Add a git tag corresponding</span>
+</span><span id="L-120"><a href="#L-120"><span class="linenos">120</span></a><span class="sd">    to the version number in pyproject.toml.&quot;&quot;&quot;</span>
+</span><span id="L-121"><a href="#L-121"><span class="linenos">121</span></a>    <span class="k">if</span> <span class="n">hassle_config</span><span class="o">.</span><span class="n">config_exists</span><span class="p">():</span>
+</span><span id="L-122"><a href="#L-122"><span class="linenos">122</span></a>        <span class="n">tag_prefix</span> <span class="o">=</span> <span class="n">hassle_config</span><span class="o">.</span><span class="n">load_config</span><span class="p">()[</span><span class="s2">&quot;git&quot;</span><span class="p">][</span><span class="s2">&quot;tag_prefix&quot;</span><span class="p">]</span>
+</span><span id="L-123"><a href="#L-123"><span class="linenos">123</span></a>    <span class="k">else</span><span class="p">:</span>
+</span><span id="L-124"><a href="#L-124"><span class="linenos">124</span></a>        <span class="n">hassle_config</span><span class="o">.</span><span class="n">warn</span><span class="p">()</span>
+</span><span id="L-125"><a href="#L-125"><span class="linenos">125</span></a>        <span class="n">tag_prefix</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
+</span><span id="L-126"><a href="#L-126"><span class="linenos">126</span></a>    <span class="n">version</span> <span class="o">=</span> <span class="p">(</span><span class="n">package_path</span> <span class="o">/</span> <span class="s2">&quot;pyproject.toml&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">loads</span><span class="p">()[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;version&quot;</span><span class="p">]</span>
+</span><span id="L-127"><a href="#L-127"><span class="linenos">127</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">package_path</span><span class="p">)</span>
+</span><span id="L-128"><a href="#L-128"><span class="linenos">128</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;git tag </span><span class="si">{</span><span class="n">tag_prefix</span><span class="si">}{</span><span class="n">version</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             </section>
                 <section id="increment_version">
                             <input id="increment_version-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="def">def</span>
-        <span class="name">increment_version</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">pyproject_path</span><span class="p">:</span> <span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span>, </span><span class="param"><span class="n">increment_type</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
+        <span class="name">increment_version</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">pyproject_path</span><span class="p">:</span> <span class="n">pathier</span><span class="o">.</span><span class="n">pathier</span><span class="o">.</span><span class="n">Pathier</span>, </span><span class="param"><span class="n">increment_type</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="increment_version-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#increment_version"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="increment_version-15"><a href="#increment_version-15"><span class="linenos">15</span></a><span class="k">def</span> <span class="nf">increment_version</span><span class="p">(</span><span class="n">pyproject_path</span><span class="p">:</span> <span class="n">Path</span><span class="p">,</span> <span class="n">increment_type</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="increment_version-16"><a href="#increment_version-16"><span class="linenos">16</span></a>    <span class="sd">&quot;&quot;&quot;Increment the project.version field in pyproject.toml.</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="increment_version-13"><a href="#increment_version-13"><span class="linenos">13</span></a><span class="k">def</span> <span class="nf">increment_version</span><span class="p">(</span><span class="n">pyproject_path</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">,</span> <span class="n">increment_type</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="increment_version-14"><a href="#increment_version-14"><span class="linenos">14</span></a>    <span class="sd">&quot;&quot;&quot;Increment the project.version field in pyproject.toml.</span>
+</span><span id="increment_version-15"><a href="#increment_version-15"><span class="linenos">15</span></a>
+</span><span id="increment_version-16"><a href="#increment_version-16"><span class="linenos">16</span></a><span class="sd">    :param package_path: Path to the package/project directory.</span>
 </span><span id="increment_version-17"><a href="#increment_version-17"><span class="linenos">17</span></a>
-</span><span id="increment_version-18"><a href="#increment_version-18"><span class="linenos">18</span></a><span class="sd">    :param package_path: Path to the package/project directory.</span>
-</span><span id="increment_version-19"><a href="#increment_version-19"><span class="linenos">19</span></a>
-</span><span id="increment_version-20"><a href="#increment_version-20"><span class="linenos">20</span></a><span class="sd">    :param increment_type: One from &#39;major&#39;, &#39;minor&#39;, or &#39;patch&#39;.&quot;&quot;&quot;</span>
-</span><span id="increment_version-21"><a href="#increment_version-21"><span class="linenos">21</span></a>    <span class="n">meta</span> <span class="o">=</span> <span class="n">tomlkit</span><span class="o">.</span><span class="n">loads</span><span class="p">(</span><span class="n">pyproject_path</span><span class="o">.</span><span class="n">read_text</span><span class="p">())</span>
-</span><span id="increment_version-22"><a href="#increment_version-22"><span class="linenos">22</span></a>    <span class="n">major</span><span class="p">,</span> <span class="n">minor</span><span class="p">,</span> <span class="n">patch</span> <span class="o">=</span> <span class="p">[</span><span class="nb">int</span><span class="p">(</span><span class="n">num</span><span class="p">)</span> <span class="k">for</span> <span class="n">num</span> <span class="ow">in</span> <span class="n">meta</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;version&quot;</span><span class="p">]</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;.&quot;</span><span class="p">)]</span>
-</span><span id="increment_version-23"><a href="#increment_version-23"><span class="linenos">23</span></a>    <span class="k">if</span> <span class="n">increment_type</span> <span class="o">==</span> <span class="s2">&quot;major&quot;</span><span class="p">:</span>
-</span><span id="increment_version-24"><a href="#increment_version-24"><span class="linenos">24</span></a>        <span class="n">major</span> <span class="o">+=</span> <span class="mi">1</span>
-</span><span id="increment_version-25"><a href="#increment_version-25"><span class="linenos">25</span></a>        <span class="n">minor</span> <span class="o">=</span> <span class="mi">0</span>
-</span><span id="increment_version-26"><a href="#increment_version-26"><span class="linenos">26</span></a>        <span class="n">patch</span> <span class="o">=</span> <span class="mi">0</span>
-</span><span id="increment_version-27"><a href="#increment_version-27"><span class="linenos">27</span></a>    <span class="k">elif</span> <span class="n">increment_type</span> <span class="o">==</span> <span class="s2">&quot;minor&quot;</span><span class="p">:</span>
-</span><span id="increment_version-28"><a href="#increment_version-28"><span class="linenos">28</span></a>        <span class="n">minor</span> <span class="o">+=</span> <span class="mi">1</span>
-</span><span id="increment_version-29"><a href="#increment_version-29"><span class="linenos">29</span></a>        <span class="n">patch</span> <span class="o">=</span> <span class="mi">0</span>
-</span><span id="increment_version-30"><a href="#increment_version-30"><span class="linenos">30</span></a>    <span class="k">elif</span> <span class="n">increment_type</span> <span class="o">==</span> <span class="s2">&quot;patch&quot;</span><span class="p">:</span>
-</span><span id="increment_version-31"><a href="#increment_version-31"><span class="linenos">31</span></a>        <span class="n">patch</span> <span class="o">+=</span> <span class="mi">1</span>
-</span><span id="increment_version-32"><a href="#increment_version-32"><span class="linenos">32</span></a>    <span class="n">incremented_version</span> <span class="o">=</span> <span class="s2">&quot;.&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="n">num</span><span class="p">)</span> <span class="k">for</span> <span class="n">num</span> <span class="ow">in</span> <span class="p">[</span><span class="n">major</span><span class="p">,</span> <span class="n">minor</span><span class="p">,</span> <span class="n">patch</span><span class="p">])</span>
-</span><span id="increment_version-33"><a href="#increment_version-33"><span class="linenos">33</span></a>    <span class="n">meta</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;version&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">incremented_version</span>
-</span><span id="increment_version-34"><a href="#increment_version-34"><span class="linenos">34</span></a>    <span class="n">pyproject_path</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="n">tomlkit</span><span class="o">.</span><span class="n">dumps</span><span class="p">(</span><span class="n">meta</span><span class="p">))</span>
+</span><span id="increment_version-18"><a href="#increment_version-18"><span class="linenos">18</span></a><span class="sd">    :param increment_type: One from &#39;major&#39;, &#39;minor&#39;, or &#39;patch&#39;.&quot;&quot;&quot;</span>
+</span><span id="increment_version-19"><a href="#increment_version-19"><span class="linenos">19</span></a>    <span class="n">meta</span> <span class="o">=</span> <span class="n">pyproject_path</span><span class="o">.</span><span class="n">loads</span><span class="p">()</span>
+</span><span id="increment_version-20"><a href="#increment_version-20"><span class="linenos">20</span></a>    <span class="n">major</span><span class="p">,</span> <span class="n">minor</span><span class="p">,</span> <span class="n">patch</span> <span class="o">=</span> <span class="p">[</span><span class="nb">int</span><span class="p">(</span><span class="n">num</span><span class="p">)</span> <span class="k">for</span> <span class="n">num</span> <span class="ow">in</span> <span class="n">meta</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;version&quot;</span><span class="p">]</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;.&quot;</span><span class="p">)]</span>
+</span><span id="increment_version-21"><a href="#increment_version-21"><span class="linenos">21</span></a>    <span class="k">if</span> <span class="n">increment_type</span> <span class="o">==</span> <span class="s2">&quot;major&quot;</span><span class="p">:</span>
+</span><span id="increment_version-22"><a href="#increment_version-22"><span class="linenos">22</span></a>        <span class="n">major</span> <span class="o">+=</span> <span class="mi">1</span>
+</span><span id="increment_version-23"><a href="#increment_version-23"><span class="linenos">23</span></a>        <span class="n">minor</span> <span class="o">=</span> <span class="mi">0</span>
+</span><span id="increment_version-24"><a href="#increment_version-24"><span class="linenos">24</span></a>        <span class="n">patch</span> <span class="o">=</span> <span class="mi">0</span>
+</span><span id="increment_version-25"><a href="#increment_version-25"><span class="linenos">25</span></a>    <span class="k">elif</span> <span class="n">increment_type</span> <span class="o">==</span> <span class="s2">&quot;minor&quot;</span><span class="p">:</span>
+</span><span id="increment_version-26"><a href="#increment_version-26"><span class="linenos">26</span></a>        <span class="n">minor</span> <span class="o">+=</span> <span class="mi">1</span>
+</span><span id="increment_version-27"><a href="#increment_version-27"><span class="linenos">27</span></a>        <span class="n">patch</span> <span class="o">=</span> <span class="mi">0</span>
+</span><span id="increment_version-28"><a href="#increment_version-28"><span class="linenos">28</span></a>    <span class="k">elif</span> <span class="n">increment_type</span> <span class="o">==</span> <span class="s2">&quot;patch&quot;</span><span class="p">:</span>
+</span><span id="increment_version-29"><a href="#increment_version-29"><span class="linenos">29</span></a>        <span class="n">patch</span> <span class="o">+=</span> <span class="mi">1</span>
+</span><span id="increment_version-30"><a href="#increment_version-30"><span class="linenos">30</span></a>    <span class="n">incremented_version</span> <span class="o">=</span> <span class="s2">&quot;.&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="n">num</span><span class="p">)</span> <span class="k">for</span> <span class="n">num</span> <span class="ow">in</span> <span class="p">[</span><span class="n">major</span><span class="p">,</span> <span class="n">minor</span><span class="p">,</span> <span class="n">patch</span><span class="p">])</span>
+</span><span id="increment_version-31"><a href="#increment_version-31"><span class="linenos">31</span></a>    <span class="n">meta</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;version&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">incremented_version</span>
+</span><span id="increment_version-32"><a href="#increment_version-32"><span class="linenos">32</span></a>    <span class="n">pyproject_path</span><span class="o">.</span><span class="n">dumps</span><span class="p">(</span><span class="n">meta</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Increment the project.version field in pyproject.toml.</p>
 
 <h6 id="parameters">Parameters</h6>
 
@@ -252,32 +248,32 @@
 
                 </section>
                 <section id="update_minimum_python_version">
                             <input id="update_minimum_python_version-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="def">def</span>
-        <span class="name">update_minimum_python_version</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">pyproject_path</span><span class="p">:</span> <span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span></span><span class="return-annotation">):</span></span>
+        <span class="name">update_minimum_python_version</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">pyproject_path</span><span class="p">:</span> <span class="n">pathier</span><span class="o">.</span><span class="n">pathier</span><span class="o">.</span><span class="n">Pathier</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="update_minimum_python_version-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#update_minimum_python_version"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="update_minimum_python_version-37"><a href="#update_minimum_python_version-37"><span class="linenos">37</span></a><span class="k">def</span> <span class="nf">update_minimum_python_version</span><span class="p">(</span><span class="n">pyproject_path</span><span class="p">:</span> <span class="n">Path</span><span class="p">):</span>
-</span><span id="update_minimum_python_version-38"><a href="#update_minimum_python_version-38"><span class="linenos">38</span></a>    <span class="sd">&quot;&quot;&quot;Use vermin to determine the minimum compatible</span>
-</span><span id="update_minimum_python_version-39"><a href="#update_minimum_python_version-39"><span class="linenos">39</span></a><span class="sd">    Python version and update the corresponding field</span>
-</span><span id="update_minimum_python_version-40"><a href="#update_minimum_python_version-40"><span class="linenos">40</span></a><span class="sd">    in pyproject.toml.&quot;&quot;&quot;</span>
-</span><span id="update_minimum_python_version-41"><a href="#update_minimum_python_version-41"><span class="linenos">41</span></a>    <span class="n">project_code</span> <span class="o">=</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span>
-</span><span id="update_minimum_python_version-42"><a href="#update_minimum_python_version-42"><span class="linenos">42</span></a>        <span class="n">file</span><span class="o">.</span><span class="n">read_text</span><span class="p">()</span> <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="p">(</span><span class="n">pyproject_path</span><span class="o">.</span><span class="n">parent</span> <span class="o">/</span> <span class="s2">&quot;src&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="s2">&quot;*.py&quot;</span><span class="p">)</span>
-</span><span id="update_minimum_python_version-43"><a href="#update_minimum_python_version-43"><span class="linenos">43</span></a>    <span class="p">)</span>
-</span><span id="update_minimum_python_version-44"><a href="#update_minimum_python_version-44"><span class="linenos">44</span></a>    <span class="n">meta</span> <span class="o">=</span> <span class="n">tomlkit</span><span class="o">.</span><span class="n">loads</span><span class="p">(</span><span class="n">pyproject_path</span><span class="o">.</span><span class="n">read_text</span><span class="p">())</span>
-</span><span id="update_minimum_python_version-45"><a href="#update_minimum_python_version-45"><span class="linenos">45</span></a>    <span class="n">minimum_version</span> <span class="o">=</span> <span class="n">vermin</span><span class="o">.</span><span class="n">visit</span><span class="p">(</span><span class="n">project_code</span><span class="p">,</span> <span class="n">vermin</span><span class="o">.</span><span class="n">Config</span><span class="p">())</span><span class="o">.</span><span class="n">minimum_versions</span><span class="p">()[</span><span class="mi">1</span><span class="p">]</span>
-</span><span id="update_minimum_python_version-46"><a href="#update_minimum_python_version-46"><span class="linenos">46</span></a>    <span class="n">minimum_version</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;&gt;=</span><span class="si">{</span><span class="n">minimum_version</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="si">}</span><span class="s2">.</span><span class="si">{</span><span class="n">minimum_version</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="update_minimum_python_version-47"><a href="#update_minimum_python_version-47"><span class="linenos">47</span></a>    <span class="n">meta</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;requires-python&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">minimum_version</span>
-</span><span id="update_minimum_python_version-48"><a href="#update_minimum_python_version-48"><span class="linenos">48</span></a>    <span class="n">pyproject_path</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="n">tomlkit</span><span class="o">.</span><span class="n">dumps</span><span class="p">(</span><span class="n">meta</span><span class="p">))</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="update_minimum_python_version-35"><a href="#update_minimum_python_version-35"><span class="linenos">35</span></a><span class="k">def</span> <span class="nf">update_minimum_python_version</span><span class="p">(</span><span class="n">pyproject_path</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">):</span>
+</span><span id="update_minimum_python_version-36"><a href="#update_minimum_python_version-36"><span class="linenos">36</span></a>    <span class="sd">&quot;&quot;&quot;Use vermin to determine the minimum compatible</span>
+</span><span id="update_minimum_python_version-37"><a href="#update_minimum_python_version-37"><span class="linenos">37</span></a><span class="sd">    Python version and update the corresponding field</span>
+</span><span id="update_minimum_python_version-38"><a href="#update_minimum_python_version-38"><span class="linenos">38</span></a><span class="sd">    in pyproject.toml.&quot;&quot;&quot;</span>
+</span><span id="update_minimum_python_version-39"><a href="#update_minimum_python_version-39"><span class="linenos">39</span></a>    <span class="n">project_code</span> <span class="o">=</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span>
+</span><span id="update_minimum_python_version-40"><a href="#update_minimum_python_version-40"><span class="linenos">40</span></a>        <span class="n">file</span><span class="o">.</span><span class="n">read_text</span><span class="p">()</span> <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="p">(</span><span class="n">pyproject_path</span><span class="o">.</span><span class="n">parent</span> <span class="o">/</span> <span class="s2">&quot;src&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="s2">&quot;*.py&quot;</span><span class="p">)</span>
+</span><span id="update_minimum_python_version-41"><a href="#update_minimum_python_version-41"><span class="linenos">41</span></a>    <span class="p">)</span>
+</span><span id="update_minimum_python_version-42"><a href="#update_minimum_python_version-42"><span class="linenos">42</span></a>    <span class="n">meta</span> <span class="o">=</span> <span class="n">pyproject_path</span><span class="o">.</span><span class="n">loads</span><span class="p">()</span>
+</span><span id="update_minimum_python_version-43"><a href="#update_minimum_python_version-43"><span class="linenos">43</span></a>    <span class="n">minimum_version</span> <span class="o">=</span> <span class="n">vermin</span><span class="o">.</span><span class="n">visit</span><span class="p">(</span><span class="n">project_code</span><span class="p">,</span> <span class="n">vermin</span><span class="o">.</span><span class="n">Config</span><span class="p">())</span><span class="o">.</span><span class="n">minimum_versions</span><span class="p">()[</span><span class="mi">1</span><span class="p">]</span>
+</span><span id="update_minimum_python_version-44"><a href="#update_minimum_python_version-44"><span class="linenos">44</span></a>    <span class="n">minimum_version</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;&gt;=</span><span class="si">{</span><span class="n">minimum_version</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="si">}</span><span class="s2">.</span><span class="si">{</span><span class="n">minimum_version</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="update_minimum_python_version-45"><a href="#update_minimum_python_version-45"><span class="linenos">45</span></a>    <span class="n">meta</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;requires-python&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">minimum_version</span>
+</span><span id="update_minimum_python_version-46"><a href="#update_minimum_python_version-46"><span class="linenos">46</span></a>    <span class="n">pyproject_path</span><span class="o">.</span><span class="n">dumps</span><span class="p">(</span><span class="n">meta</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Use vermin to determine the minimum compatible
 Python version and update the corresponding field
 in pyproject.toml.</p>
 </div>
@@ -285,87 +281,87 @@
 
                 </section>
                 <section id="generate_docs">
                             <input id="generate_docs-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="def">def</span>
-        <span class="name">generate_docs</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">package_path</span><span class="p">:</span> <span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span></span><span class="return-annotation">):</span></span>
+        <span class="name">generate_docs</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">package_path</span><span class="p">:</span> <span class="n">pathier</span><span class="o">.</span><span class="n">pathier</span><span class="o">.</span><span class="n">Pathier</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="generate_docs-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#generate_docs"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="generate_docs-51"><a href="#generate_docs-51"><span class="linenos">51</span></a><span class="k">def</span> <span class="nf">generate_docs</span><span class="p">(</span><span class="n">package_path</span><span class="p">:</span> <span class="n">Path</span><span class="p">):</span>
-</span><span id="generate_docs-52"><a href="#generate_docs-52"><span class="linenos">52</span></a>    <span class="sd">&quot;&quot;&quot;Generate project documentation using pdoc.&quot;&quot;&quot;</span>
-</span><span id="generate_docs-53"><a href="#generate_docs-53"><span class="linenos">53</span></a>    <span class="k">try</span><span class="p">:</span>
-</span><span id="generate_docs-54"><a href="#generate_docs-54"><span class="linenos">54</span></a>        <span class="n">shutil</span><span class="o">.</span><span class="n">rmtree</span><span class="p">(</span><span class="n">package_path</span> <span class="o">/</span> <span class="s2">&quot;docs&quot;</span><span class="p">)</span>
-</span><span id="generate_docs-55"><a href="#generate_docs-55"><span class="linenos">55</span></a>    <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="generate_docs-56"><a href="#generate_docs-56"><span class="linenos">56</span></a>        <span class="k">pass</span>
-</span><span id="generate_docs-57"><a href="#generate_docs-57"><span class="linenos">57</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span>
-</span><span id="generate_docs-58"><a href="#generate_docs-58"><span class="linenos">58</span></a>        <span class="sa">f</span><span class="s2">&quot;pdoc -o </span><span class="si">{</span><span class="n">package_path</span> <span class="o">/</span> <span class="s1">&#39;docs&#39;</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">package_path</span> <span class="o">/</span> <span class="s1">&#39;src&#39;</span> <span class="o">/</span> <span class="n">package_path</span><span class="o">.</span><span class="n">stem</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="generate_docs-59"><a href="#generate_docs-59"><span class="linenos">59</span></a>    <span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="generate_docs-49"><a href="#generate_docs-49"><span class="linenos">49</span></a><span class="k">def</span> <span class="nf">generate_docs</span><span class="p">(</span><span class="n">package_path</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">):</span>
+</span><span id="generate_docs-50"><a href="#generate_docs-50"><span class="linenos">50</span></a>    <span class="sd">&quot;&quot;&quot;Generate project documentation using pdoc.&quot;&quot;&quot;</span>
+</span><span id="generate_docs-51"><a href="#generate_docs-51"><span class="linenos">51</span></a>    <span class="k">try</span><span class="p">:</span>
+</span><span id="generate_docs-52"><a href="#generate_docs-52"><span class="linenos">52</span></a>        <span class="p">(</span><span class="n">package_path</span> <span class="o">/</span> <span class="s2">&quot;docs&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">delete</span><span class="p">()</span>
+</span><span id="generate_docs-53"><a href="#generate_docs-53"><span class="linenos">53</span></a>    <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="generate_docs-54"><a href="#generate_docs-54"><span class="linenos">54</span></a>        <span class="k">pass</span>
+</span><span id="generate_docs-55"><a href="#generate_docs-55"><span class="linenos">55</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span>
+</span><span id="generate_docs-56"><a href="#generate_docs-56"><span class="linenos">56</span></a>        <span class="sa">f</span><span class="s2">&quot;pdoc -o </span><span class="si">{</span><span class="n">package_path</span> <span class="o">/</span> <span class="s1">&#39;docs&#39;</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">package_path</span> <span class="o">/</span> <span class="s1">&#39;src&#39;</span> <span class="o">/</span> <span class="n">package_path</span><span class="o">.</span><span class="n">stem</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="generate_docs-57"><a href="#generate_docs-57"><span class="linenos">57</span></a>    <span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Generate project documentation using pdoc.</p>
 </div>
 
 
                 </section>
                 <section id="update_dependencies">
                             <input id="update_dependencies-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="def">def</span>
-        <span class="name">update_dependencies</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="n">pyproject_path</span><span class="p">:</span> <span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span>,</span><span class="param">	<span class="n">overwrite</span><span class="p">:</span> <span class="nb">bool</span>,</span><span class="param">	<span class="n">include_versions</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span></span><span class="return-annotation">):</span></span>
+        <span class="name">update_dependencies</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="n">pyproject_path</span><span class="p">:</span> <span class="n">pathier</span><span class="o">.</span><span class="n">pathier</span><span class="o">.</span><span class="n">Pathier</span>,</span><span class="param">	<span class="n">overwrite</span><span class="p">:</span> <span class="nb">bool</span>,</span><span class="param">	<span class="n">include_versions</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="update_dependencies-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#update_dependencies"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="update_dependencies-62"><a href="#update_dependencies-62"><span class="linenos"> 62</span></a><span class="k">def</span> <span class="nf">update_dependencies</span><span class="p">(</span>
-</span><span id="update_dependencies-63"><a href="#update_dependencies-63"><span class="linenos"> 63</span></a>    <span class="n">pyproject_path</span><span class="p">:</span> <span class="n">Path</span><span class="p">,</span> <span class="n">overwrite</span><span class="p">:</span> <span class="nb">bool</span><span class="p">,</span> <span class="n">include_versions</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>
-</span><span id="update_dependencies-64"><a href="#update_dependencies-64"><span class="linenos"> 64</span></a><span class="p">):</span>
-</span><span id="update_dependencies-65"><a href="#update_dependencies-65"><span class="linenos"> 65</span></a>    <span class="sd">&quot;&quot;&quot;Update dependencies list in pyproject.toml.</span>
-</span><span id="update_dependencies-66"><a href="#update_dependencies-66"><span class="linenos"> 66</span></a>
-</span><span id="update_dependencies-67"><a href="#update_dependencies-67"><span class="linenos"> 67</span></a><span class="sd">    :param overwrite: If True, replace the dependencies in pyproject.toml</span>
-</span><span id="update_dependencies-68"><a href="#update_dependencies-68"><span class="linenos"> 68</span></a><span class="sd">    with the results of packagelister.scan() .</span>
-</span><span id="update_dependencies-69"><a href="#update_dependencies-69"><span class="linenos"> 69</span></a><span class="sd">    If False, packages returned by packagelister are appended to</span>
-</span><span id="update_dependencies-70"><a href="#update_dependencies-70"><span class="linenos"> 70</span></a><span class="sd">    the current dependencies in pyproject.toml if they don&#39;t already</span>
-</span><span id="update_dependencies-71"><a href="#update_dependencies-71"><span class="linenos"> 71</span></a><span class="sd">    exist in the field.&quot;&quot;&quot;</span>
-</span><span id="update_dependencies-72"><a href="#update_dependencies-72"><span class="linenos"> 72</span></a>    <span class="n">packages</span> <span class="o">=</span> <span class="n">packagelister</span><span class="o">.</span><span class="n">scan</span><span class="p">(</span><span class="n">pyproject_path</span><span class="o">.</span><span class="n">parent</span><span class="p">)</span>
-</span><span id="update_dependencies-73"><a href="#update_dependencies-73"><span class="linenos"> 73</span></a>
-</span><span id="update_dependencies-74"><a href="#update_dependencies-74"><span class="linenos"> 74</span></a>    <span class="n">packages</span> <span class="o">=</span> <span class="p">[</span>
-</span><span id="update_dependencies-75"><a href="#update_dependencies-75"><span class="linenos"> 75</span></a>        <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">package</span><span class="si">}</span><span class="s2">~=</span><span class="si">{</span><span class="n">packages</span><span class="p">[</span><span class="n">package</span><span class="p">][</span><span class="s1">&#39;version&#39;</span><span class="p">]</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="update_dependencies-76"><a href="#update_dependencies-76"><span class="linenos"> 76</span></a>        <span class="k">if</span> <span class="n">packages</span><span class="p">[</span><span class="n">package</span><span class="p">][</span><span class="s2">&quot;version&quot;</span><span class="p">]</span> <span class="ow">and</span> <span class="n">include_versions</span>
-</span><span id="update_dependencies-77"><a href="#update_dependencies-77"><span class="linenos"> 77</span></a>        <span class="k">else</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">package</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="update_dependencies-78"><a href="#update_dependencies-78"><span class="linenos"> 78</span></a>        <span class="k">for</span> <span class="n">package</span> <span class="ow">in</span> <span class="n">packages</span>
-</span><span id="update_dependencies-79"><a href="#update_dependencies-79"><span class="linenos"> 79</span></a>        <span class="k">if</span> <span class="n">package</span> <span class="o">!=</span> <span class="n">pyproject_path</span><span class="o">.</span><span class="n">parent</span><span class="o">.</span><span class="n">stem</span>
-</span><span id="update_dependencies-80"><a href="#update_dependencies-80"><span class="linenos"> 80</span></a>    <span class="p">]</span>
-</span><span id="update_dependencies-81"><a href="#update_dependencies-81"><span class="linenos"> 81</span></a>    <span class="n">packages</span> <span class="o">=</span> <span class="p">[</span>
-</span><span id="update_dependencies-82"><a href="#update_dependencies-82"><span class="linenos"> 82</span></a>        <span class="n">package</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;speech_recognition&quot;</span><span class="p">,</span> <span class="s2">&quot;speechRecognition&quot;</span><span class="p">)</span>
-</span><span id="update_dependencies-83"><a href="#update_dependencies-83"><span class="linenos"> 83</span></a>        <span class="k">for</span> <span class="n">package</span> <span class="ow">in</span> <span class="n">packages</span>
-</span><span id="update_dependencies-84"><a href="#update_dependencies-84"><span class="linenos"> 84</span></a>    <span class="p">]</span>
-</span><span id="update_dependencies-85"><a href="#update_dependencies-85"><span class="linenos"> 85</span></a>    <span class="n">meta</span> <span class="o">=</span> <span class="n">tomlkit</span><span class="o">.</span><span class="n">loads</span><span class="p">(</span><span class="n">pyproject_path</span><span class="o">.</span><span class="n">read_text</span><span class="p">())</span>
-</span><span id="update_dependencies-86"><a href="#update_dependencies-86"><span class="linenos"> 86</span></a>    <span class="k">if</span> <span class="n">overwrite</span><span class="p">:</span>
-</span><span id="update_dependencies-87"><a href="#update_dependencies-87"><span class="linenos"> 87</span></a>        <span class="n">meta</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;dependencies&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">packages</span>
-</span><span id="update_dependencies-88"><a href="#update_dependencies-88"><span class="linenos"> 88</span></a>    <span class="k">else</span><span class="p">:</span>
-</span><span id="update_dependencies-89"><a href="#update_dependencies-89"><span class="linenos"> 89</span></a>        <span class="k">for</span> <span class="n">package</span> <span class="ow">in</span> <span class="n">packages</span><span class="p">:</span>
-</span><span id="update_dependencies-90"><a href="#update_dependencies-90"><span class="linenos"> 90</span></a>            <span class="k">if</span> <span class="s2">&quot;~&quot;</span> <span class="ow">in</span> <span class="n">package</span><span class="p">:</span>
-</span><span id="update_dependencies-91"><a href="#update_dependencies-91"><span class="linenos"> 91</span></a>                <span class="n">name</span> <span class="o">=</span> <span class="n">package</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;~&quot;</span><span class="p">)[</span><span class="mi">0</span><span class="p">]</span>
-</span><span id="update_dependencies-92"><a href="#update_dependencies-92"><span class="linenos"> 92</span></a>            <span class="k">elif</span> <span class="s2">&quot;=&quot;</span> <span class="ow">in</span> <span class="n">package</span><span class="p">:</span>
-</span><span id="update_dependencies-93"><a href="#update_dependencies-93"><span class="linenos"> 93</span></a>                <span class="n">name</span> <span class="o">=</span> <span class="n">package</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;=&quot;</span><span class="p">)[</span><span class="mi">0</span><span class="p">]</span>
-</span><span id="update_dependencies-94"><a href="#update_dependencies-94"><span class="linenos"> 94</span></a>            <span class="k">else</span><span class="p">:</span>
-</span><span id="update_dependencies-95"><a href="#update_dependencies-95"><span class="linenos"> 95</span></a>                <span class="n">name</span> <span class="o">=</span> <span class="n">package</span>
-</span><span id="update_dependencies-96"><a href="#update_dependencies-96"><span class="linenos"> 96</span></a>            <span class="k">if</span> <span class="nb">all</span><span class="p">(</span>
-</span><span id="update_dependencies-97"><a href="#update_dependencies-97"><span class="linenos"> 97</span></a>                <span class="n">name</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">dependency</span> <span class="k">for</span> <span class="n">dependency</span> <span class="ow">in</span> <span class="n">meta</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;dependencies&quot;</span><span class="p">]</span>
-</span><span id="update_dependencies-98"><a href="#update_dependencies-98"><span class="linenos"> 98</span></a>            <span class="p">):</span>
-</span><span id="update_dependencies-99"><a href="#update_dependencies-99"><span class="linenos"> 99</span></a>                <span class="n">meta</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;dependencies&quot;</span><span class="p">]</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">package</span><span class="p">)</span>
-</span><span id="update_dependencies-100"><a href="#update_dependencies-100"><span class="linenos">100</span></a>    <span class="n">pyproject_path</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="n">tomlkit</span><span class="o">.</span><span class="n">dumps</span><span class="p">(</span><span class="n">meta</span><span class="p">))</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="update_dependencies-60"><a href="#update_dependencies-60"><span class="linenos">60</span></a><span class="k">def</span> <span class="nf">update_dependencies</span><span class="p">(</span>
+</span><span id="update_dependencies-61"><a href="#update_dependencies-61"><span class="linenos">61</span></a>    <span class="n">pyproject_path</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">,</span> <span class="n">overwrite</span><span class="p">:</span> <span class="nb">bool</span><span class="p">,</span> <span class="n">include_versions</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>
+</span><span id="update_dependencies-62"><a href="#update_dependencies-62"><span class="linenos">62</span></a><span class="p">):</span>
+</span><span id="update_dependencies-63"><a href="#update_dependencies-63"><span class="linenos">63</span></a>    <span class="sd">&quot;&quot;&quot;Update dependencies list in pyproject.toml.</span>
+</span><span id="update_dependencies-64"><a href="#update_dependencies-64"><span class="linenos">64</span></a>
+</span><span id="update_dependencies-65"><a href="#update_dependencies-65"><span class="linenos">65</span></a><span class="sd">    :param overwrite: If True, replace the dependencies in pyproject.toml</span>
+</span><span id="update_dependencies-66"><a href="#update_dependencies-66"><span class="linenos">66</span></a><span class="sd">    with the results of packagelister.scan() .</span>
+</span><span id="update_dependencies-67"><a href="#update_dependencies-67"><span class="linenos">67</span></a><span class="sd">    If False, packages returned by packagelister are appended to</span>
+</span><span id="update_dependencies-68"><a href="#update_dependencies-68"><span class="linenos">68</span></a><span class="sd">    the current dependencies in pyproject.toml if they don&#39;t already</span>
+</span><span id="update_dependencies-69"><a href="#update_dependencies-69"><span class="linenos">69</span></a><span class="sd">    exist in the field.&quot;&quot;&quot;</span>
+</span><span id="update_dependencies-70"><a href="#update_dependencies-70"><span class="linenos">70</span></a>    <span class="n">packages</span> <span class="o">=</span> <span class="n">packagelister</span><span class="o">.</span><span class="n">scan</span><span class="p">(</span><span class="n">pyproject_path</span><span class="o">.</span><span class="n">parent</span><span class="p">)</span>
+</span><span id="update_dependencies-71"><a href="#update_dependencies-71"><span class="linenos">71</span></a>
+</span><span id="update_dependencies-72"><a href="#update_dependencies-72"><span class="linenos">72</span></a>    <span class="n">packages</span> <span class="o">=</span> <span class="p">[</span>
+</span><span id="update_dependencies-73"><a href="#update_dependencies-73"><span class="linenos">73</span></a>        <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">package</span><span class="si">}</span><span class="s2">~=</span><span class="si">{</span><span class="n">packages</span><span class="p">[</span><span class="n">package</span><span class="p">][</span><span class="s1">&#39;version&#39;</span><span class="p">]</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="update_dependencies-74"><a href="#update_dependencies-74"><span class="linenos">74</span></a>        <span class="k">if</span> <span class="n">packages</span><span class="p">[</span><span class="n">package</span><span class="p">][</span><span class="s2">&quot;version&quot;</span><span class="p">]</span> <span class="ow">and</span> <span class="n">include_versions</span>
+</span><span id="update_dependencies-75"><a href="#update_dependencies-75"><span class="linenos">75</span></a>        <span class="k">else</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">package</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="update_dependencies-76"><a href="#update_dependencies-76"><span class="linenos">76</span></a>        <span class="k">for</span> <span class="n">package</span> <span class="ow">in</span> <span class="n">packages</span>
+</span><span id="update_dependencies-77"><a href="#update_dependencies-77"><span class="linenos">77</span></a>        <span class="k">if</span> <span class="n">package</span> <span class="o">!=</span> <span class="n">pyproject_path</span><span class="o">.</span><span class="n">parent</span><span class="o">.</span><span class="n">stem</span>
+</span><span id="update_dependencies-78"><a href="#update_dependencies-78"><span class="linenos">78</span></a>    <span class="p">]</span>
+</span><span id="update_dependencies-79"><a href="#update_dependencies-79"><span class="linenos">79</span></a>    <span class="n">packages</span> <span class="o">=</span> <span class="p">[</span>
+</span><span id="update_dependencies-80"><a href="#update_dependencies-80"><span class="linenos">80</span></a>        <span class="n">package</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;speech_recognition&quot;</span><span class="p">,</span> <span class="s2">&quot;speechRecognition&quot;</span><span class="p">)</span>
+</span><span id="update_dependencies-81"><a href="#update_dependencies-81"><span class="linenos">81</span></a>        <span class="k">for</span> <span class="n">package</span> <span class="ow">in</span> <span class="n">packages</span>
+</span><span id="update_dependencies-82"><a href="#update_dependencies-82"><span class="linenos">82</span></a>    <span class="p">]</span>
+</span><span id="update_dependencies-83"><a href="#update_dependencies-83"><span class="linenos">83</span></a>    <span class="n">meta</span> <span class="o">=</span> <span class="n">pyproject_path</span><span class="o">.</span><span class="n">loads</span><span class="p">()</span>
+</span><span id="update_dependencies-84"><a href="#update_dependencies-84"><span class="linenos">84</span></a>    <span class="k">if</span> <span class="n">overwrite</span><span class="p">:</span>
+</span><span id="update_dependencies-85"><a href="#update_dependencies-85"><span class="linenos">85</span></a>        <span class="n">meta</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;dependencies&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">packages</span>
+</span><span id="update_dependencies-86"><a href="#update_dependencies-86"><span class="linenos">86</span></a>    <span class="k">else</span><span class="p">:</span>
+</span><span id="update_dependencies-87"><a href="#update_dependencies-87"><span class="linenos">87</span></a>        <span class="k">for</span> <span class="n">package</span> <span class="ow">in</span> <span class="n">packages</span><span class="p">:</span>
+</span><span id="update_dependencies-88"><a href="#update_dependencies-88"><span class="linenos">88</span></a>            <span class="k">if</span> <span class="s2">&quot;~&quot;</span> <span class="ow">in</span> <span class="n">package</span><span class="p">:</span>
+</span><span id="update_dependencies-89"><a href="#update_dependencies-89"><span class="linenos">89</span></a>                <span class="n">name</span> <span class="o">=</span> <span class="n">package</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;~&quot;</span><span class="p">)[</span><span class="mi">0</span><span class="p">]</span>
+</span><span id="update_dependencies-90"><a href="#update_dependencies-90"><span class="linenos">90</span></a>            <span class="k">elif</span> <span class="s2">&quot;=&quot;</span> <span class="ow">in</span> <span class="n">package</span><span class="p">:</span>
+</span><span id="update_dependencies-91"><a href="#update_dependencies-91"><span class="linenos">91</span></a>                <span class="n">name</span> <span class="o">=</span> <span class="n">package</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;=&quot;</span><span class="p">)[</span><span class="mi">0</span><span class="p">]</span>
+</span><span id="update_dependencies-92"><a href="#update_dependencies-92"><span class="linenos">92</span></a>            <span class="k">else</span><span class="p">:</span>
+</span><span id="update_dependencies-93"><a href="#update_dependencies-93"><span class="linenos">93</span></a>                <span class="n">name</span> <span class="o">=</span> <span class="n">package</span>
+</span><span id="update_dependencies-94"><a href="#update_dependencies-94"><span class="linenos">94</span></a>            <span class="k">if</span> <span class="nb">all</span><span class="p">(</span>
+</span><span id="update_dependencies-95"><a href="#update_dependencies-95"><span class="linenos">95</span></a>                <span class="n">name</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">dependency</span> <span class="k">for</span> <span class="n">dependency</span> <span class="ow">in</span> <span class="n">meta</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;dependencies&quot;</span><span class="p">]</span>
+</span><span id="update_dependencies-96"><a href="#update_dependencies-96"><span class="linenos">96</span></a>            <span class="p">):</span>
+</span><span id="update_dependencies-97"><a href="#update_dependencies-97"><span class="linenos">97</span></a>                <span class="n">meta</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;dependencies&quot;</span><span class="p">]</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">package</span><span class="p">)</span>
+</span><span id="update_dependencies-98"><a href="#update_dependencies-98"><span class="linenos">98</span></a>    <span class="n">pyproject_path</span><span class="o">.</span><span class="n">dumps</span><span class="p">(</span><span class="n">meta</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Update dependencies list in pyproject.toml.</p>
 
 <h6 id="parameters">Parameters</h6>
 
@@ -381,68 +377,66 @@
 
                 </section>
                 <section id="update_changelog">
                             <input id="update_changelog-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="def">def</span>
-        <span class="name">update_changelog</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">pyproject_path</span><span class="p">:</span> <span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span></span><span class="return-annotation">):</span></span>
+        <span class="name">update_changelog</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">pyproject_path</span><span class="p">:</span> <span class="n">pathier</span><span class="o">.</span><span class="n">pathier</span><span class="o">.</span><span class="n">Pathier</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="update_changelog-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#update_changelog"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="update_changelog-103"><a href="#update_changelog-103"><span class="linenos">103</span></a><span class="k">def</span> <span class="nf">update_changelog</span><span class="p">(</span><span class="n">pyproject_path</span><span class="p">:</span> <span class="n">Path</span><span class="p">):</span>
-</span><span id="update_changelog-104"><a href="#update_changelog-104"><span class="linenos">104</span></a>    <span class="sd">&quot;&quot;&quot;Update project changelog.&quot;&quot;&quot;</span>
-</span><span id="update_changelog-105"><a href="#update_changelog-105"><span class="linenos">105</span></a>    <span class="n">meta</span> <span class="o">=</span> <span class="n">tomlkit</span><span class="o">.</span><span class="n">loads</span><span class="p">(</span><span class="n">pyproject_path</span><span class="o">.</span><span class="n">read_text</span><span class="p">())</span>
-</span><span id="update_changelog-106"><a href="#update_changelog-106"><span class="linenos">106</span></a>    <span class="k">if</span> <span class="n">hassle_config</span><span class="o">.</span><span class="n">config_exists</span><span class="p">():</span>
-</span><span id="update_changelog-107"><a href="#update_changelog-107"><span class="linenos">107</span></a>        <span class="n">config</span> <span class="o">=</span> <span class="n">hassle_config</span><span class="o">.</span><span class="n">load_config</span><span class="p">()</span>
-</span><span id="update_changelog-108"><a href="#update_changelog-108"><span class="linenos">108</span></a>    <span class="k">else</span><span class="p">:</span>
-</span><span id="update_changelog-109"><a href="#update_changelog-109"><span class="linenos">109</span></a>        <span class="n">hassle_config</span><span class="o">.</span><span class="n">warn</span><span class="p">()</span>
-</span><span id="update_changelog-110"><a href="#update_changelog-110"><span class="linenos">110</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Creating blank hassle_config.toml...&quot;</span><span class="p">)</span>
-</span><span id="update_changelog-111"><a href="#update_changelog-111"><span class="linenos">111</span></a>        <span class="n">config</span> <span class="o">=</span> <span class="n">hassle_config</span><span class="o">.</span><span class="n">load_config</span><span class="p">()</span>
-</span><span id="update_changelog-112"><a href="#update_changelog-112"><span class="linenos">112</span></a>    <span class="n">changelog_path</span> <span class="o">=</span> <span class="n">pyproject_path</span><span class="o">.</span><span class="n">parent</span> <span class="o">/</span> <span class="s2">&quot;CHANGELOG.md&quot;</span>
-</span><span id="update_changelog-113"><a href="#update_changelog-113"><span class="linenos">113</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span>
-</span><span id="update_changelog-114"><a href="#update_changelog-114"><span class="linenos">114</span></a>        <span class="sa">f</span><span class="s2">&quot;auto-changelog -p </span><span class="si">{</span><span class="n">pyproject_path</span><span class="o">.</span><span class="n">parent</span><span class="si">}</span><span class="s2"> --tag-prefix </span><span class="si">{</span><span class="n">config</span><span class="p">[</span><span class="s1">&#39;git&#39;</span><span class="p">][</span><span class="s1">&#39;tag_prefix&#39;</span><span class="p">]</span><span class="si">}</span><span class="s2"> --unreleased -v </span><span class="si">{</span><span class="n">meta</span><span class="p">[</span><span class="s1">&#39;project&#39;</span><span class="p">][</span><span class="s1">&#39;version&#39;</span><span class="p">]</span><span class="si">}</span><span class="s2"> -o </span><span class="si">{</span><span class="n">changelog_path</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="update_changelog-115"><a href="#update_changelog-115"><span class="linenos">115</span></a>    <span class="p">)</span>
-</span><span id="update_changelog-116"><a href="#update_changelog-116"><span class="linenos">116</span></a>    <span class="n">changelog</span> <span class="o">=</span> <span class="n">changelog_path</span><span class="o">.</span><span class="n">read_text</span><span class="p">()</span><span class="o">.</span><span class="n">splitlines</span><span class="p">()</span>
-</span><span id="update_changelog-117"><a href="#update_changelog-117"><span class="linenos">117</span></a>    <span class="n">changelog</span> <span class="o">=</span> <span class="p">[</span><span class="n">line</span> <span class="k">for</span> <span class="n">line</span> <span class="ow">in</span> <span class="n">changelog</span> <span class="k">if</span> <span class="s2">&quot;Full set of changes:&quot;</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">line</span><span class="p">]</span>
-</span><span id="update_changelog-118"><a href="#update_changelog-118"><span class="linenos">118</span></a>    <span class="n">changelog_path</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">changelog</span><span class="p">))</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="update_changelog-101"><a href="#update_changelog-101"><span class="linenos">101</span></a><span class="k">def</span> <span class="nf">update_changelog</span><span class="p">(</span><span class="n">pyproject_path</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">):</span>
+</span><span id="update_changelog-102"><a href="#update_changelog-102"><span class="linenos">102</span></a>    <span class="sd">&quot;&quot;&quot;Update project changelog.&quot;&quot;&quot;</span>
+</span><span id="update_changelog-103"><a href="#update_changelog-103"><span class="linenos">103</span></a>    <span class="n">meta</span> <span class="o">=</span> <span class="n">pyproject_path</span><span class="o">.</span><span class="n">loads</span><span class="p">()</span>
+</span><span id="update_changelog-104"><a href="#update_changelog-104"><span class="linenos">104</span></a>    <span class="k">if</span> <span class="n">hassle_config</span><span class="o">.</span><span class="n">config_exists</span><span class="p">():</span>
+</span><span id="update_changelog-105"><a href="#update_changelog-105"><span class="linenos">105</span></a>        <span class="n">config</span> <span class="o">=</span> <span class="n">hassle_config</span><span class="o">.</span><span class="n">load_config</span><span class="p">()</span>
+</span><span id="update_changelog-106"><a href="#update_changelog-106"><span class="linenos">106</span></a>    <span class="k">else</span><span class="p">:</span>
+</span><span id="update_changelog-107"><a href="#update_changelog-107"><span class="linenos">107</span></a>        <span class="n">hassle_config</span><span class="o">.</span><span class="n">warn</span><span class="p">()</span>
+</span><span id="update_changelog-108"><a href="#update_changelog-108"><span class="linenos">108</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Creating blank hassle_config.toml...&quot;</span><span class="p">)</span>
+</span><span id="update_changelog-109"><a href="#update_changelog-109"><span class="linenos">109</span></a>        <span class="n">config</span> <span class="o">=</span> <span class="n">hassle_config</span><span class="o">.</span><span class="n">load_config</span><span class="p">()</span>
+</span><span id="update_changelog-110"><a href="#update_changelog-110"><span class="linenos">110</span></a>    <span class="n">changelog_path</span> <span class="o">=</span> <span class="n">pyproject_path</span><span class="o">.</span><span class="n">parent</span> <span class="o">/</span> <span class="s2">&quot;CHANGELOG.md&quot;</span>
+</span><span id="update_changelog-111"><a href="#update_changelog-111"><span class="linenos">111</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span>
+</span><span id="update_changelog-112"><a href="#update_changelog-112"><span class="linenos">112</span></a>        <span class="sa">f</span><span class="s2">&quot;auto-changelog -p </span><span class="si">{</span><span class="n">pyproject_path</span><span class="o">.</span><span class="n">parent</span><span class="si">}</span><span class="s2"> --tag-prefix </span><span class="si">{</span><span class="n">config</span><span class="p">[</span><span class="s1">&#39;git&#39;</span><span class="p">][</span><span class="s1">&#39;tag_prefix&#39;</span><span class="p">]</span><span class="si">}</span><span class="s2"> --unreleased -v </span><span class="si">{</span><span class="n">meta</span><span class="p">[</span><span class="s1">&#39;project&#39;</span><span class="p">][</span><span class="s1">&#39;version&#39;</span><span class="p">]</span><span class="si">}</span><span class="s2"> -o </span><span class="si">{</span><span class="n">changelog_path</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="update_changelog-113"><a href="#update_changelog-113"><span class="linenos">113</span></a>    <span class="p">)</span>
+</span><span id="update_changelog-114"><a href="#update_changelog-114"><span class="linenos">114</span></a>    <span class="n">changelog</span> <span class="o">=</span> <span class="n">changelog_path</span><span class="o">.</span><span class="n">read_text</span><span class="p">()</span><span class="o">.</span><span class="n">splitlines</span><span class="p">()</span>
+</span><span id="update_changelog-115"><a href="#update_changelog-115"><span class="linenos">115</span></a>    <span class="n">changelog</span> <span class="o">=</span> <span class="p">[</span><span class="n">line</span> <span class="k">for</span> <span class="n">line</span> <span class="ow">in</span> <span class="n">changelog</span> <span class="k">if</span> <span class="s2">&quot;Full set of changes:&quot;</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">line</span><span class="p">]</span>
+</span><span id="update_changelog-116"><a href="#update_changelog-116"><span class="linenos">116</span></a>    <span class="n">changelog_path</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">changelog</span><span class="p">))</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Update project changelog.</p>
 </div>
 
 
                 </section>
                 <section id="tag_version">
                             <input id="tag_version-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="def">def</span>
-        <span class="name">tag_version</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">package_path</span><span class="p">:</span> <span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span></span><span class="return-annotation">):</span></span>
+        <span class="name">tag_version</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">package_path</span><span class="p">:</span> <span class="n">pathier</span><span class="o">.</span><span class="n">pathier</span><span class="o">.</span><span class="n">Pathier</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="tag_version-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#tag_version"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="tag_version-121"><a href="#tag_version-121"><span class="linenos">121</span></a><span class="k">def</span> <span class="nf">tag_version</span><span class="p">(</span><span class="n">package_path</span><span class="p">:</span> <span class="n">Path</span><span class="p">):</span>
-</span><span id="tag_version-122"><a href="#tag_version-122"><span class="linenos">122</span></a>    <span class="sd">&quot;&quot;&quot;Add a git tag corresponding</span>
-</span><span id="tag_version-123"><a href="#tag_version-123"><span class="linenos">123</span></a><span class="sd">    to the version number in pyproject.toml.&quot;&quot;&quot;</span>
-</span><span id="tag_version-124"><a href="#tag_version-124"><span class="linenos">124</span></a>    <span class="k">if</span> <span class="n">hassle_config</span><span class="o">.</span><span class="n">config_exists</span><span class="p">():</span>
-</span><span id="tag_version-125"><a href="#tag_version-125"><span class="linenos">125</span></a>        <span class="n">tag_prefix</span> <span class="o">=</span> <span class="n">hassle_config</span><span class="o">.</span><span class="n">load_config</span><span class="p">()[</span><span class="s2">&quot;git&quot;</span><span class="p">][</span><span class="s2">&quot;tag_prefix&quot;</span><span class="p">]</span>
-</span><span id="tag_version-126"><a href="#tag_version-126"><span class="linenos">126</span></a>    <span class="k">else</span><span class="p">:</span>
-</span><span id="tag_version-127"><a href="#tag_version-127"><span class="linenos">127</span></a>        <span class="n">hassle_config</span><span class="o">.</span><span class="n">warn</span><span class="p">()</span>
-</span><span id="tag_version-128"><a href="#tag_version-128"><span class="linenos">128</span></a>        <span class="n">tag_prefix</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
-</span><span id="tag_version-129"><a href="#tag_version-129"><span class="linenos">129</span></a>    <span class="n">version</span> <span class="o">=</span> <span class="n">tomlkit</span><span class="o">.</span><span class="n">loads</span><span class="p">((</span><span class="n">package_path</span> <span class="o">/</span> <span class="s2">&quot;pyproject.toml&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">read_text</span><span class="p">())[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span>
-</span><span id="tag_version-130"><a href="#tag_version-130"><span class="linenos">130</span></a>        <span class="s2">&quot;version&quot;</span>
-</span><span id="tag_version-131"><a href="#tag_version-131"><span class="linenos">131</span></a>    <span class="p">]</span>
-</span><span id="tag_version-132"><a href="#tag_version-132"><span class="linenos">132</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">package_path</span><span class="p">)</span>
-</span><span id="tag_version-133"><a href="#tag_version-133"><span class="linenos">133</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;git tag </span><span class="si">{</span><span class="n">tag_prefix</span><span class="si">}{</span><span class="n">version</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="tag_version-119"><a href="#tag_version-119"><span class="linenos">119</span></a><span class="k">def</span> <span class="nf">tag_version</span><span class="p">(</span><span class="n">package_path</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">):</span>
+</span><span id="tag_version-120"><a href="#tag_version-120"><span class="linenos">120</span></a>    <span class="sd">&quot;&quot;&quot;Add a git tag corresponding</span>
+</span><span id="tag_version-121"><a href="#tag_version-121"><span class="linenos">121</span></a><span class="sd">    to the version number in pyproject.toml.&quot;&quot;&quot;</span>
+</span><span id="tag_version-122"><a href="#tag_version-122"><span class="linenos">122</span></a>    <span class="k">if</span> <span class="n">hassle_config</span><span class="o">.</span><span class="n">config_exists</span><span class="p">():</span>
+</span><span id="tag_version-123"><a href="#tag_version-123"><span class="linenos">123</span></a>        <span class="n">tag_prefix</span> <span class="o">=</span> <span class="n">hassle_config</span><span class="o">.</span><span class="n">load_config</span><span class="p">()[</span><span class="s2">&quot;git&quot;</span><span class="p">][</span><span class="s2">&quot;tag_prefix&quot;</span><span class="p">]</span>
+</span><span id="tag_version-124"><a href="#tag_version-124"><span class="linenos">124</span></a>    <span class="k">else</span><span class="p">:</span>
+</span><span id="tag_version-125"><a href="#tag_version-125"><span class="linenos">125</span></a>        <span class="n">hassle_config</span><span class="o">.</span><span class="n">warn</span><span class="p">()</span>
+</span><span id="tag_version-126"><a href="#tag_version-126"><span class="linenos">126</span></a>        <span class="n">tag_prefix</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
+</span><span id="tag_version-127"><a href="#tag_version-127"><span class="linenos">127</span></a>    <span class="n">version</span> <span class="o">=</span> <span class="p">(</span><span class="n">package_path</span> <span class="o">/</span> <span class="s2">&quot;pyproject.toml&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">loads</span><span class="p">()[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;version&quot;</span><span class="p">]</span>
+</span><span id="tag_version-128"><a href="#tag_version-128"><span class="linenos">128</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">package_path</span><span class="p">)</span>
+</span><span id="tag_version-129"><a href="#tag_version-129"><span class="linenos">129</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;git tag </span><span class="si">{</span><span class="n">tag_prefix</span><span class="si">}{</span><span class="n">version</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Add a git tag corresponding
 to the version number in pyproject.toml.</p>
 </div>
```

#### html2text {}

```diff
@@ -10,298 +10,293 @@
     * update_changelog
     * tag_version
 built_with_pdoc[pdoc_logo]
 
 ****** hassle.hassle_utilities ******
 ⁰ View Source
 __1import os
-__2import shutil
-__3from pathlib import Path
-__4
-__5import packagelister
-__6import tomlkit
-__7import vermin
+__2
+__3import packagelister
+__4import vermin
+__5from pathier import Pathier
+__6
+__7from hassle import hassle_config
 __8
-__9from hassle import hassle_config
+__9root = Pathier(__file__).parent
 _10
-_11root = Path(__file__).parent
-_12
-_13
-_14def increment_version(pyproject_path: Path, increment_type: str):
-_15    """Increment the project.version field in pyproject.toml.
+_11
+_12def increment_version(pyproject_path: Pathier, increment_type: str):
+_13    """Increment the project.version field in pyproject.toml.
+_14
+_15    :param package_path: Path to the package/project directory.
 _16
-_17    :param package_path: Path to the package/project directory.
-_18
-_19    :param increment_type: One from 'major', 'minor', or 'patch'."""
-_20    meta = tomlkit.loads(pyproject_path.read_text())
-_21    major, minor, patch = [int(num) for num in meta["project"]
+_17    :param increment_type: One from 'major', 'minor', or 'patch'."""
+_18    meta = pyproject_path.loads()
+_19    major, minor, patch = [int(num) for num in meta["project"]
 ["version"].split(".")]
-_22    if increment_type == "major":
-_23        major += 1
-_24        minor = 0
-_25        patch = 0
-_26    elif increment_type == "minor":
-_27        minor += 1
-_28        patch = 0
-_29    elif increment_type == "patch":
-_30        patch += 1
-_31    incremented_version = ".".join(str(num) for num in [major, minor,
+_20    if increment_type == "major":
+_21        major += 1
+_22        minor = 0
+_23        patch = 0
+_24    elif increment_type == "minor":
+_25        minor += 1
+_26        patch = 0
+_27    elif increment_type == "patch":
+_28        patch += 1
+_29    incremented_version = ".".join(str(num) for num in [major, minor,
 patch])
-_32    meta["project"]["version"] = incremented_version
-_33    pyproject_path.write_text(tomlkit.dumps(meta))
-_34
-_35
-_36def update_minimum_python_version(pyproject_path: Path):
-_37    """Use vermin to determine the minimum compatible
-_38    Python version and update the corresponding field
-_39    in pyproject.toml."""
-_40    project_code = "\n".join(
-_41        file.read_text() for file in (pyproject_path.parent / "src").rglob
+_30    meta["project"]["version"] = incremented_version
+_31    pyproject_path.dumps(meta)
+_32
+_33
+_34def update_minimum_python_version(pyproject_path: Pathier):
+_35    """Use vermin to determine the minimum compatible
+_36    Python version and update the corresponding field
+_37    in pyproject.toml."""
+_38    project_code = "\n".join(
+_39        file.read_text() for file in (pyproject_path.parent / "src").rglob
 ("*.py")
-_42    )
-_43    meta = tomlkit.loads(pyproject_path.read_text())
-_44    minimum_version = vermin.visit(project_code, vermin.Config
+_40    )
+_41    meta = pyproject_path.loads()
+_42    minimum_version = vermin.visit(project_code, vermin.Config
 ()).minimum_versions()[1]
-_45    minimum_version = f">={minimum_version[0]}.{minimum_version[1]}"
-_46    meta["project"]["requires-python"] = minimum_version
-_47    pyproject_path.write_text(tomlkit.dumps(meta))
-_48
-_49
-_50def generate_docs(package_path: Path):
-_51    """Generate project documentation using pdoc."""
-_52    try:
-_53        shutil.rmtree(package_path / "docs")
-_54    except Exception as e:
-_55        pass
-_56    os.system(
-_57        f"pdoc -o {package_path / 'docs'} {package_path / 'src' /
+_43    minimum_version = f">={minimum_version[0]}.{minimum_version[1]}"
+_44    meta["project"]["requires-python"] = minimum_version
+_45    pyproject_path.dumps(meta)
+_46
+_47
+_48def generate_docs(package_path: Pathier):
+_49    """Generate project documentation using pdoc."""
+_50    try:
+_51        (package_path / "docs").delete()
+_52    except Exception as e:
+_53        pass
+_54    os.system(
+_55        f"pdoc -o {package_path / 'docs'} {package_path / 'src' /
 package_path.stem}"
-_58    )
-_59
-_60
-_61def update_dependencies(
-_62    pyproject_path: Path, overwrite: bool, include_versions: bool = False
-_63):
-_64    """Update dependencies list in pyproject.toml.
-_65
-_66    :param overwrite: If True, replace the dependencies in pyproject.toml
-_67    with the results of packagelister.scan() .
-_68    If False, packages returned by packagelister are appended to
-_69    the current dependencies in pyproject.toml if they don't already
-_70    exist in the field."""
-_71    packages = packagelister.scan(pyproject_path.parent)
-_72
-_73    packages = [
-_74        f"{package}~={packages[package]['version']}"
-_75        if packages[package]["version"] and include_versions
-_76        else f"{package}"
-_77        for package in packages
-_78        if package != pyproject_path.parent.stem
-_79    ]
-_80    packages = [
-_81        package.replace("speech_recognition", "speechRecognition")
-_82        for package in packages
-_83    ]
-_84    meta = tomlkit.loads(pyproject_path.read_text())
-_85    if overwrite:
-_86        meta["project"]["dependencies"] = packages
-_87    else:
-_88        for package in packages:
-_89            if "~" in package:
-_90                name = package.split("~")[0]
-_91            elif "=" in package:
-_92                name = package.split("=")[0]
-_93            else:
-_94                name = package
-_95            if all(
-_96                name not in dependency for dependency in meta["project"]
+_56    )
+_57
+_58
+_59def update_dependencies(
+_60    pyproject_path: Pathier, overwrite: bool, include_versions: bool = False
+_61):
+_62    """Update dependencies list in pyproject.toml.
+_63
+_64    :param overwrite: If True, replace the dependencies in pyproject.toml
+_65    with the results of packagelister.scan() .
+_66    If False, packages returned by packagelister are appended to
+_67    the current dependencies in pyproject.toml if they don't already
+_68    exist in the field."""
+_69    packages = packagelister.scan(pyproject_path.parent)
+_70
+_71    packages = [
+_72        f"{package}~={packages[package]['version']}"
+_73        if packages[package]["version"] and include_versions
+_74        else f"{package}"
+_75        for package in packages
+_76        if package != pyproject_path.parent.stem
+_77    ]
+_78    packages = [
+_79        package.replace("speech_recognition", "speechRecognition")
+_80        for package in packages
+_81    ]
+_82    meta = pyproject_path.loads()
+_83    if overwrite:
+_84        meta["project"]["dependencies"] = packages
+_85    else:
+_86        for package in packages:
+_87            if "~" in package:
+_88                name = package.split("~")[0]
+_89            elif "=" in package:
+_90                name = package.split("=")[0]
+_91            else:
+_92                name = package
+_93            if all(
+_94                name not in dependency for dependency in meta["project"]
 ["dependencies"]
-_97            ):
-_98                meta["project"]["dependencies"].append(package)
-_99    pyproject_path.write_text(tomlkit.dumps(meta))
-100
-101
-102def update_changelog(pyproject_path: Path):
-103    """Update project changelog."""
-104    meta = tomlkit.loads(pyproject_path.read_text())
-105    if hassle_config.config_exists():
-106        config = hassle_config.load_config()
-107    else:
-108        hassle_config.warn()
-109        print("Creating blank hassle_config.toml...")
-110        config = hassle_config.load_config()
-111    changelog_path = pyproject_path.parent / "CHANGELOG.md"
-112    os.system(
-113        f"auto-changelog -p {pyproject_path.parent} --tag-prefix {config
+_95            ):
+_96                meta["project"]["dependencies"].append(package)
+_97    pyproject_path.dumps(meta)
+_98
+_99
+100def update_changelog(pyproject_path: Pathier):
+101    """Update project changelog."""
+102    meta = pyproject_path.loads()
+103    if hassle_config.config_exists():
+104        config = hassle_config.load_config()
+105    else:
+106        hassle_config.warn()
+107        print("Creating blank hassle_config.toml...")
+108        config = hassle_config.load_config()
+109    changelog_path = pyproject_path.parent / "CHANGELOG.md"
+110    os.system(
+111        f"auto-changelog -p {pyproject_path.parent} --tag-prefix {config
 ['git']['tag_prefix']} --unreleased -v {meta['project']['version']} -o
 {changelog_path}"
-114    )
-115    changelog = changelog_path.read_text().splitlines()
-116    changelog = [line for line in changelog if "Full set of changes:" not in
+112    )
+113    changelog = changelog_path.read_text().splitlines()
+114    changelog = [line for line in changelog if "Full set of changes:" not in
 line]
-117    changelog_path.write_text("\n".join(changelog))
-118
-119
-120def tag_version(package_path: Path):
-121    """Add a git tag corresponding
-122    to the version number in pyproject.toml."""
-123    if hassle_config.config_exists():
-124        tag_prefix = hassle_config.load_config()["git"]["tag_prefix"]
-125    else:
-126        hassle_config.warn()
-127        tag_prefix = ""
-128    version = tomlkit.loads((package_path / "pyproject.toml").read_text())
-["project"][
-129        "version"
-130    ]
-131    os.chdir(package_path)
-132    os.system(f"git tag {tag_prefix}{version}")
+115    changelog_path.write_text("\n".join(changelog))
+116
+117
+118def tag_version(package_path: Pathier):
+119    """Add a git tag corresponding
+120    to the version number in pyproject.toml."""
+121    if hassle_config.config_exists():
+122        tag_prefix = hassle_config.load_config()["git"]["tag_prefix"]
+123    else:
+124        hassle_config.warn()
+125        tag_prefix = ""
+126    version = (package_path / "pyproject.toml").loads()["project"]
+["version"]
+127    os.chdir(package_path)
+128    os.system(f"git tag {tag_prefix}{version}")
   ⁰
-def increment_version(pyproject_path: pathlib.Path, increment_type: str): View
-Source
-15def increment_version(pyproject_path: Path, increment_type: str):
-16    """Increment the project.version field in pyproject.toml.
+def increment_version(pyproject_path: pathier.pathier.Pathier, increment_type:
+str): View Source
+13def increment_version(pyproject_path: Pathier, increment_type: str):
+14    """Increment the project.version field in pyproject.toml.
+15
+16    :param package_path: Path to the package/project directory.
 17
-18    :param package_path: Path to the package/project directory.
-19
-20    :param increment_type: One from 'major', 'minor', or 'patch'."""
-21    meta = tomlkit.loads(pyproject_path.read_text())
-22    major, minor, patch = [int(num) for num in meta["project"]
+18    :param increment_type: One from 'major', 'minor', or 'patch'."""
+19    meta = pyproject_path.loads()
+20    major, minor, patch = [int(num) for num in meta["project"]
 ["version"].split(".")]
-23    if increment_type == "major":
-24        major += 1
-25        minor = 0
-26        patch = 0
-27    elif increment_type == "minor":
-28        minor += 1
-29        patch = 0
-30    elif increment_type == "patch":
-31        patch += 1
-32    incremented_version = ".".join(str(num) for num in [major, minor, patch])
-33    meta["project"]["version"] = incremented_version
-34    pyproject_path.write_text(tomlkit.dumps(meta))
+21    if increment_type == "major":
+22        major += 1
+23        minor = 0
+24        patch = 0
+25    elif increment_type == "minor":
+26        minor += 1
+27        patch = 0
+28    elif increment_type == "patch":
+29        patch += 1
+30    incremented_version = ".".join(str(num) for num in [major, minor, patch])
+31    meta["project"]["version"] = incremented_version
+32    pyproject_path.dumps(meta)
 Increment the project.version field in pyproject.toml.
 * Parameters *
     * package_path: Path to the package/project directory.
     * increment_type: One from 'major', 'minor', or 'patch'.
   ⁰
-def update_minimum_python_version(pyproject_path: pathlib.Path): View Source
-37def update_minimum_python_version(pyproject_path: Path):
-38    """Use vermin to determine the minimum compatible
-39    Python version and update the corresponding field
-40    in pyproject.toml."""
-41    project_code = "\n".join(
-42        file.read_text() for file in (pyproject_path.parent / "src").rglob
+def update_minimum_python_version(pyproject_path: pathier.pathier.Pathier):
+View Source
+35def update_minimum_python_version(pyproject_path: Pathier):
+36    """Use vermin to determine the minimum compatible
+37    Python version and update the corresponding field
+38    in pyproject.toml."""
+39    project_code = "\n".join(
+40        file.read_text() for file in (pyproject_path.parent / "src").rglob
 ("*.py")
-43    )
-44    meta = tomlkit.loads(pyproject_path.read_text())
-45    minimum_version = vermin.visit(project_code, vermin.Config
+41    )
+42    meta = pyproject_path.loads()
+43    minimum_version = vermin.visit(project_code, vermin.Config
 ()).minimum_versions()[1]
-46    minimum_version = f">={minimum_version[0]}.{minimum_version[1]}"
-47    meta["project"]["requires-python"] = minimum_version
-48    pyproject_path.write_text(tomlkit.dumps(meta))
+44    minimum_version = f">={minimum_version[0]}.{minimum_version[1]}"
+45    meta["project"]["requires-python"] = minimum_version
+46    pyproject_path.dumps(meta)
 Use vermin to determine the minimum compatible Python version and update the
 corresponding field in pyproject.toml.
   ⁰
-def generate_docs(package_path: pathlib.Path): View Source
-51def generate_docs(package_path: Path):
-52    """Generate project documentation using pdoc."""
-53    try:
-54        shutil.rmtree(package_path / "docs")
-55    except Exception as e:
-56        pass
-57    os.system(
-58        f"pdoc -o {package_path / 'docs'} {package_path / 'src' /
+def generate_docs(package_path: pathier.pathier.Pathier): View Source
+49def generate_docs(package_path: Pathier):
+50    """Generate project documentation using pdoc."""
+51    try:
+52        (package_path / "docs").delete()
+53    except Exception as e:
+54        pass
+55    os.system(
+56        f"pdoc -o {package_path / 'docs'} {package_path / 'src' /
 package_path.stem}"
-59    )
+57    )
 Generate project documentation using pdoc.
   ⁰
 def update_dependencies(
-pyproject_path: pathlib.Path,
+pyproject_path: pathier.pathier.Pathier,
 overwrite: bool,
 include_versions: bool = False): View Source
-_62def update_dependencies(
-_63    pyproject_path: Path, overwrite: bool, include_versions: bool = False
-_64):
-_65    """Update dependencies list in pyproject.toml.
-_66
-_67    :param overwrite: If True, replace the dependencies in pyproject.toml
-_68    with the results of packagelister.scan() .
-_69    If False, packages returned by packagelister are appended to
-_70    the current dependencies in pyproject.toml if they don't already
-_71    exist in the field."""
-_72    packages = packagelister.scan(pyproject_path.parent)
-_73
-_74    packages = [
-_75        f"{package}~={packages[package]['version']}"
-_76        if packages[package]["version"] and include_versions
-_77        else f"{package}"
-_78        for package in packages
-_79        if package != pyproject_path.parent.stem
-_80    ]
-_81    packages = [
-_82        package.replace("speech_recognition", "speechRecognition")
-_83        for package in packages
-_84    ]
-_85    meta = tomlkit.loads(pyproject_path.read_text())
-_86    if overwrite:
-_87        meta["project"]["dependencies"] = packages
-_88    else:
-_89        for package in packages:
-_90            if "~" in package:
-_91                name = package.split("~")[0]
-_92            elif "=" in package:
-_93                name = package.split("=")[0]
-_94            else:
-_95                name = package
-_96            if all(
-_97                name not in dependency for dependency in meta["project"]
+60def update_dependencies(
+61    pyproject_path: Pathier, overwrite: bool, include_versions: bool = False
+62):
+63    """Update dependencies list in pyproject.toml.
+64
+65    :param overwrite: If True, replace the dependencies in pyproject.toml
+66    with the results of packagelister.scan() .
+67    If False, packages returned by packagelister are appended to
+68    the current dependencies in pyproject.toml if they don't already
+69    exist in the field."""
+70    packages = packagelister.scan(pyproject_path.parent)
+71
+72    packages = [
+73        f"{package}~={packages[package]['version']}"
+74        if packages[package]["version"] and include_versions
+75        else f"{package}"
+76        for package in packages
+77        if package != pyproject_path.parent.stem
+78    ]
+79    packages = [
+80        package.replace("speech_recognition", "speechRecognition")
+81        for package in packages
+82    ]
+83    meta = pyproject_path.loads()
+84    if overwrite:
+85        meta["project"]["dependencies"] = packages
+86    else:
+87        for package in packages:
+88            if "~" in package:
+89                name = package.split("~")[0]
+90            elif "=" in package:
+91                name = package.split("=")[0]
+92            else:
+93                name = package
+94            if all(
+95                name not in dependency for dependency in meta["project"]
 ["dependencies"]
-_98            ):
-_99                meta["project"]["dependencies"].append(package)
-100    pyproject_path.write_text(tomlkit.dumps(meta))
+96            ):
+97                meta["project"]["dependencies"].append(package)
+98    pyproject_path.dumps(meta)
 Update dependencies list in pyproject.toml.
 * Parameters *
     * overwrite: If True, replace the dependencies in pyproject.toml with the
       results of packagelister.scan() . If False, packages returned by
       packagelister are appended to the current dependencies in pyproject.toml
       if they don't already exist in the field.
   ⁰
-def update_changelog(pyproject_path: pathlib.Path): View Source
-103def update_changelog(pyproject_path: Path):
-104    """Update project changelog."""
-105    meta = tomlkit.loads(pyproject_path.read_text())
-106    if hassle_config.config_exists():
-107        config = hassle_config.load_config()
-108    else:
-109        hassle_config.warn()
-110        print("Creating blank hassle_config.toml...")
-111        config = hassle_config.load_config()
-112    changelog_path = pyproject_path.parent / "CHANGELOG.md"
-113    os.system(
-114        f"auto-changelog -p {pyproject_path.parent} --tag-prefix {config
+def update_changelog(pyproject_path: pathier.pathier.Pathier): View Source
+101def update_changelog(pyproject_path: Pathier):
+102    """Update project changelog."""
+103    meta = pyproject_path.loads()
+104    if hassle_config.config_exists():
+105        config = hassle_config.load_config()
+106    else:
+107        hassle_config.warn()
+108        print("Creating blank hassle_config.toml...")
+109        config = hassle_config.load_config()
+110    changelog_path = pyproject_path.parent / "CHANGELOG.md"
+111    os.system(
+112        f"auto-changelog -p {pyproject_path.parent} --tag-prefix {config
 ['git']['tag_prefix']} --unreleased -v {meta['project']['version']} -o
 {changelog_path}"
-115    )
-116    changelog = changelog_path.read_text().splitlines()
-117    changelog = [line for line in changelog if "Full set of changes:" not in
+113    )
+114    changelog = changelog_path.read_text().splitlines()
+115    changelog = [line for line in changelog if "Full set of changes:" not in
 line]
-118    changelog_path.write_text("\n".join(changelog))
+116    changelog_path.write_text("\n".join(changelog))
 Update project changelog.
   ⁰
-def tag_version(package_path: pathlib.Path): View Source
-121def tag_version(package_path: Path):
-122    """Add a git tag corresponding
-123    to the version number in pyproject.toml."""
-124    if hassle_config.config_exists():
-125        tag_prefix = hassle_config.load_config()["git"]["tag_prefix"]
-126    else:
-127        hassle_config.warn()
-128        tag_prefix = ""
-129    version = tomlkit.loads((package_path / "pyproject.toml").read_text())
-["project"][
-130        "version"
-131    ]
-132    os.chdir(package_path)
-133    os.system(f"git tag {tag_prefix}{version}")
+def tag_version(package_path: pathier.pathier.Pathier): View Source
+119def tag_version(package_path: Pathier):
+120    """Add a git tag corresponding
+121    to the version number in pyproject.toml."""
+122    if hassle_config.config_exists():
+123        tag_prefix = hassle_config.load_config()["git"]["tag_prefix"]
+124    else:
+125        hassle_config.warn()
+126        tag_prefix = ""
+127    version = (package_path / "pyproject.toml").loads()["project"]
+["version"]
+128    os.chdir(package_path)
+129    os.system(f"git tag {tag_prefix}{version}")
 Add a git tag corresponding to the version number in pyproject.toml.
```

### Comparing `hassle-2.4.0/docs/hassle/new_project.html` & `hassle-2.5.0/docs/hassle/new_project.html`

 * *Files 2% similar despite different names*

```diff
@@ -82,286 +82,284 @@
                 
                         <input id="mod-new_project-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 
                         <label class="view-source-button" for="mod-new_project-view-source"><span>View Source</span></label>
 
                         <div class="pdoc-code codehilite"><pre><span></span><span id="L-1"><a href="#L-1"><span class="linenos">  1</span></a><span class="kn">import</span> <span class="nn">argparse</span>
 </span><span id="L-2"><a href="#L-2"><span class="linenos">  2</span></a><span class="kn">import</span> <span class="nn">os</span>
-</span><span id="L-3"><a href="#L-3"><span class="linenos">  3</span></a><span class="kn">import</span> <span class="nn">shutil</span>
-</span><span id="L-4"><a href="#L-4"><span class="linenos">  4</span></a><span class="kn">import</span> <span class="nn">sys</span>
-</span><span id="L-5"><a href="#L-5"><span class="linenos">  5</span></a><span class="kn">from</span> <span class="nn">datetime</span> <span class="kn">import</span> <span class="n">datetime</span>
-</span><span id="L-6"><a href="#L-6"><span class="linenos">  6</span></a><span class="kn">from</span> <span class="nn">pathlib</span> <span class="kn">import</span> <span class="n">Path</span>
-</span><span id="L-7"><a href="#L-7"><span class="linenos">  7</span></a>
-</span><span id="L-8"><a href="#L-8"><span class="linenos">  8</span></a><span class="kn">import</span> <span class="nn">requests</span>
-</span><span id="L-9"><a href="#L-9"><span class="linenos">  9</span></a><span class="kn">import</span> <span class="nn">tomlkit</span>
-</span><span id="L-10"><a href="#L-10"><span class="linenos"> 10</span></a><span class="kn">from</span> <span class="nn">bs4</span> <span class="kn">import</span> <span class="n">BeautifulSoup</span>
-</span><span id="L-11"><a href="#L-11"><span class="linenos"> 11</span></a>
-</span><span id="L-12"><a href="#L-12"><span class="linenos"> 12</span></a><span class="kn">import</span> <span class="nn">hassle.hassle_config</span> <span class="k">as</span> <span class="nn">hassle_config</span>
-</span><span id="L-13"><a href="#L-13"><span class="linenos"> 13</span></a><span class="kn">from</span> <span class="nn">hassle.generate_tests</span> <span class="kn">import</span> <span class="n">generate_test_files</span>
+</span><span id="L-3"><a href="#L-3"><span class="linenos">  3</span></a><span class="kn">import</span> <span class="nn">sys</span>
+</span><span id="L-4"><a href="#L-4"><span class="linenos">  4</span></a><span class="kn">from</span> <span class="nn">datetime</span> <span class="kn">import</span> <span class="n">datetime</span>
+</span><span id="L-5"><a href="#L-5"><span class="linenos">  5</span></a>
+</span><span id="L-6"><a href="#L-6"><span class="linenos">  6</span></a><span class="kn">import</span> <span class="nn">requests</span>
+</span><span id="L-7"><a href="#L-7"><span class="linenos">  7</span></a><span class="kn">from</span> <span class="nn">bs4</span> <span class="kn">import</span> <span class="n">BeautifulSoup</span>
+</span><span id="L-8"><a href="#L-8"><span class="linenos">  8</span></a><span class="kn">from</span> <span class="nn">pathier</span> <span class="kn">import</span> <span class="n">Pathier</span>
+</span><span id="L-9"><a href="#L-9"><span class="linenos">  9</span></a>
+</span><span id="L-10"><a href="#L-10"><span class="linenos"> 10</span></a><span class="kn">import</span> <span class="nn">hassle.hassle_config</span> <span class="k">as</span> <span class="nn">hassle_config</span>
+</span><span id="L-11"><a href="#L-11"><span class="linenos"> 11</span></a><span class="kn">from</span> <span class="nn">hassle.generate_tests</span> <span class="kn">import</span> <span class="n">generate_test_files</span>
+</span><span id="L-12"><a href="#L-12"><span class="linenos"> 12</span></a>
+</span><span id="L-13"><a href="#L-13"><span class="linenos"> 13</span></a><span class="n">root</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="vm">__file__</span><span class="p">)</span><span class="o">.</span><span class="n">parent</span>
 </span><span id="L-14"><a href="#L-14"><span class="linenos"> 14</span></a>
-</span><span id="L-15"><a href="#L-15"><span class="linenos"> 15</span></a><span class="n">root</span> <span class="o">=</span> <span class="n">Path</span><span class="p">(</span><span class="vm">__file__</span><span class="p">)</span><span class="o">.</span><span class="n">parent</span>
-</span><span id="L-16"><a href="#L-16"><span class="linenos"> 16</span></a>
-</span><span id="L-17"><a href="#L-17"><span class="linenos"> 17</span></a>
-</span><span id="L-18"><a href="#L-18"><span class="linenos"> 18</span></a><span class="k">def</span> <span class="nf">get_args</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">:</span>
-</span><span id="L-19"><a href="#L-19"><span class="linenos"> 19</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">argparse</span><span class="o">.</span><span class="n">ArgumentParser</span><span class="p">()</span>
-</span><span id="L-20"><a href="#L-20"><span class="linenos"> 20</span></a>
-</span><span id="L-21"><a href="#L-21"><span class="linenos"> 21</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-22"><a href="#L-22"><span class="linenos"> 22</span></a>        <span class="s2">&quot;name&quot;</span><span class="p">,</span>
-</span><span id="L-23"><a href="#L-23"><span class="linenos"> 23</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
-</span><span id="L-24"><a href="#L-24"><span class="linenos"> 24</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Name of the package to create in the current working directory. &quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-25"><a href="#L-25"><span class="linenos"> 25</span></a>    <span class="p">)</span>
-</span><span id="L-26"><a href="#L-26"><span class="linenos"> 26</span></a>
-</span><span id="L-27"><a href="#L-27"><span class="linenos"> 27</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-28"><a href="#L-28"><span class="linenos"> 28</span></a>        <span class="s2">&quot;-s&quot;</span><span class="p">,</span>
-</span><span id="L-29"><a href="#L-29"><span class="linenos"> 29</span></a>        <span class="s2">&quot;--source_files&quot;</span><span class="p">,</span>
-</span><span id="L-30"><a href="#L-30"><span class="linenos"> 30</span></a>        <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;*&quot;</span><span class="p">,</span>
-</span><span id="L-31"><a href="#L-31"><span class="linenos"> 31</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
-</span><span id="L-32"><a href="#L-32"><span class="linenos"> 32</span></a>        <span class="n">default</span><span class="o">=</span><span class="p">[],</span>
-</span><span id="L-33"><a href="#L-33"><span class="linenos"> 33</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; List of additional source files to create in addition to the default</span>
-</span><span id="L-34"><a href="#L-34"><span class="linenos"> 34</span></a><span class="s2">        __init__.py and </span><span class="si">{name}</span><span class="s2">.py files.&quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-35"><a href="#L-35"><span class="linenos"> 35</span></a>    <span class="p">)</span>
-</span><span id="L-36"><a href="#L-36"><span class="linenos"> 36</span></a>
-</span><span id="L-37"><a href="#L-37"><span class="linenos"> 37</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-38"><a href="#L-38"><span class="linenos"> 38</span></a>        <span class="s2">&quot;-d&quot;</span><span class="p">,</span>
-</span><span id="L-39"><a href="#L-39"><span class="linenos"> 39</span></a>        <span class="s2">&quot;--description&quot;</span><span class="p">,</span>
-</span><span id="L-40"><a href="#L-40"><span class="linenos"> 40</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
-</span><span id="L-41"><a href="#L-41"><span class="linenos"> 41</span></a>        <span class="n">default</span><span class="o">=</span><span class="s2">&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-42"><a href="#L-42"><span class="linenos"> 42</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; The package description to be added to the pyproject.toml file. &quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-43"><a href="#L-43"><span class="linenos"> 43</span></a>    <span class="p">)</span>
-</span><span id="L-44"><a href="#L-44"><span class="linenos"> 44</span></a>
-</span><span id="L-45"><a href="#L-45"><span class="linenos"> 45</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-46"><a href="#L-46"><span class="linenos"> 46</span></a>        <span class="s2">&quot;-dp&quot;</span><span class="p">,</span>
-</span><span id="L-47"><a href="#L-47"><span class="linenos"> 47</span></a>        <span class="s2">&quot;--dependencies&quot;</span><span class="p">,</span>
-</span><span id="L-48"><a href="#L-48"><span class="linenos"> 48</span></a>        <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;*&quot;</span><span class="p">,</span>
-</span><span id="L-49"><a href="#L-49"><span class="linenos"> 49</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
-</span><span id="L-50"><a href="#L-50"><span class="linenos"> 50</span></a>        <span class="n">default</span><span class="o">=</span><span class="p">[],</span>
-</span><span id="L-51"><a href="#L-51"><span class="linenos"> 51</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; List of dependencies to add to pyproject.toml.</span>
-</span><span id="L-52"><a href="#L-52"><span class="linenos"> 52</span></a><span class="s2">        Note: hassle.py will automatically scan your project for 3rd party</span>
-</span><span id="L-53"><a href="#L-53"><span class="linenos"> 53</span></a><span class="s2">        imports and update pyproject.toml. This switch is largely useful</span>
-</span><span id="L-54"><a href="#L-54"><span class="linenos"> 54</span></a><span class="s2">        for adding dependencies your project might need, but doesn&#39;t</span>
-</span><span id="L-55"><a href="#L-55"><span class="linenos"> 55</span></a><span class="s2">        directly import in any source files,</span>
-</span><span id="L-56"><a href="#L-56"><span class="linenos"> 56</span></a><span class="s2">        like an os.system() call that invokes a 3rd party cli.&quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-57"><a href="#L-57"><span class="linenos"> 57</span></a>    <span class="p">)</span>
-</span><span id="L-58"><a href="#L-58"><span class="linenos"> 58</span></a>
-</span><span id="L-59"><a href="#L-59"><span class="linenos"> 59</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-60"><a href="#L-60"><span class="linenos"> 60</span></a>        <span class="s2">&quot;-k&quot;</span><span class="p">,</span>
-</span><span id="L-61"><a href="#L-61"><span class="linenos"> 61</span></a>        <span class="s2">&quot;--keywords&quot;</span><span class="p">,</span>
-</span><span id="L-62"><a href="#L-62"><span class="linenos"> 62</span></a>        <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;*&quot;</span><span class="p">,</span>
-</span><span id="L-63"><a href="#L-63"><span class="linenos"> 63</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
-</span><span id="L-64"><a href="#L-64"><span class="linenos"> 64</span></a>        <span class="n">default</span><span class="o">=</span><span class="p">[],</span>
-</span><span id="L-65"><a href="#L-65"><span class="linenos"> 65</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; List of keywords to be added to the keywords field in pyproject.toml. &quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-66"><a href="#L-66"><span class="linenos"> 66</span></a>    <span class="p">)</span>
-</span><span id="L-67"><a href="#L-67"><span class="linenos"> 67</span></a>
-</span><span id="L-68"><a href="#L-68"><span class="linenos"> 68</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-69"><a href="#L-69"><span class="linenos"> 69</span></a>        <span class="s2">&quot;-as&quot;</span><span class="p">,</span>
-</span><span id="L-70"><a href="#L-70"><span class="linenos"> 70</span></a>        <span class="s2">&quot;--add_script&quot;</span><span class="p">,</span>
-</span><span id="L-71"><a href="#L-71"><span class="linenos"> 71</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
-</span><span id="L-72"><a href="#L-72"><span class="linenos"> 72</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Add section to pyproject.toml declaring the package </span>
-</span><span id="L-73"><a href="#L-73"><span class="linenos"> 73</span></a><span class="s2">        should be installed with command line scripts added. </span>
-</span><span id="L-74"><a href="#L-74"><span class="linenos"> 74</span></a><span class="s2">        The default is &#39;</span><span class="si">{name}</span><span class="s2"> = &quot;</span><span class="si">{name}</span><span class="s2">.</span><span class="si">{name}</span><span class="s2">:main&quot;.</span>
-</span><span id="L-75"><a href="#L-75"><span class="linenos"> 75</span></a><span class="s2">        You will need to manually change this field.&quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-76"><a href="#L-76"><span class="linenos"> 76</span></a>    <span class="p">)</span>
-</span><span id="L-77"><a href="#L-77"><span class="linenos"> 77</span></a>
-</span><span id="L-78"><a href="#L-78"><span class="linenos"> 78</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-79"><a href="#L-79"><span class="linenos"> 79</span></a>        <span class="s2">&quot;-nl&quot;</span><span class="p">,</span>
-</span><span id="L-80"><a href="#L-80"><span class="linenos"> 80</span></a>        <span class="s2">&quot;--no_license&quot;</span><span class="p">,</span>
-</span><span id="L-81"><a href="#L-81"><span class="linenos"> 81</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
-</span><span id="L-82"><a href="#L-82"><span class="linenos"> 82</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; By default, projects are created with an MIT license.</span>
-</span><span id="L-83"><a href="#L-83"><span class="linenos"> 83</span></a><span class="s2">        Set this flag to avoid adding a license if you want to configure licensing</span>
-</span><span id="L-84"><a href="#L-84"><span class="linenos"> 84</span></a><span class="s2">        at another time.&quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-85"><a href="#L-85"><span class="linenos"> 85</span></a>    <span class="p">)</span>
-</span><span id="L-86"><a href="#L-86"><span class="linenos"> 86</span></a>
-</span><span id="L-87"><a href="#L-87"><span class="linenos"> 87</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-88"><a href="#L-88"><span class="linenos"> 88</span></a>        <span class="s2">&quot;-os&quot;</span><span class="p">,</span>
-</span><span id="L-89"><a href="#L-89"><span class="linenos"> 89</span></a>        <span class="s2">&quot;--operating_system&quot;</span><span class="p">,</span>
-</span><span id="L-90"><a href="#L-90"><span class="linenos"> 90</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
-</span><span id="L-91"><a href="#L-91"><span class="linenos"> 91</span></a>        <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
-</span><span id="L-92"><a href="#L-92"><span class="linenos"> 92</span></a>        <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;*&quot;</span><span class="p">,</span>
-</span><span id="L-93"><a href="#L-93"><span class="linenos"> 93</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; List of operating systems this package will be compatible with.</span>
-</span><span id="L-94"><a href="#L-94"><span class="linenos"> 94</span></a><span class="s2">        The default is OS Independent.</span>
-</span><span id="L-95"><a href="#L-95"><span class="linenos"> 95</span></a><span class="s2">        This only affects the &#39;classifiers&#39; field of pyproject.toml .&quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-96"><a href="#L-96"><span class="linenos"> 96</span></a>    <span class="p">)</span>
-</span><span id="L-97"><a href="#L-97"><span class="linenos"> 97</span></a>
-</span><span id="L-98"><a href="#L-98"><span class="linenos"> 98</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-99"><a href="#L-99"><span class="linenos"> 99</span></a>        <span class="s2">&quot;-np&quot;</span><span class="p">,</span>
-</span><span id="L-100"><a href="#L-100"><span class="linenos">100</span></a>        <span class="s2">&quot;--not_package&quot;</span><span class="p">,</span>
-</span><span id="L-101"><a href="#L-101"><span class="linenos">101</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
-</span><span id="L-102"><a href="#L-102"><span class="linenos">102</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Put source files in top level directory and delete tests folder. &quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-103"><a href="#L-103"><span class="linenos">103</span></a>    <span class="p">)</span>
-</span><span id="L-104"><a href="#L-104"><span class="linenos">104</span></a>
-</span><span id="L-105"><a href="#L-105"><span class="linenos">105</span></a>    <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="o">.</span><span class="n">parse_args</span><span class="p">()</span>
-</span><span id="L-106"><a href="#L-106"><span class="linenos">106</span></a>    <span class="n">args</span><span class="o">.</span><span class="n">source_files</span><span class="o">.</span><span class="n">extend</span><span class="p">([</span><span class="s2">&quot;__init__.py&quot;</span><span class="p">,</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2">.py&quot;</span><span class="p">])</span>
+</span><span id="L-15"><a href="#L-15"><span class="linenos"> 15</span></a>
+</span><span id="L-16"><a href="#L-16"><span class="linenos"> 16</span></a><span class="k">def</span> <span class="nf">get_args</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">:</span>
+</span><span id="L-17"><a href="#L-17"><span class="linenos"> 17</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">argparse</span><span class="o">.</span><span class="n">ArgumentParser</span><span class="p">()</span>
+</span><span id="L-18"><a href="#L-18"><span class="linenos"> 18</span></a>
+</span><span id="L-19"><a href="#L-19"><span class="linenos"> 19</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-20"><a href="#L-20"><span class="linenos"> 20</span></a>        <span class="s2">&quot;name&quot;</span><span class="p">,</span>
+</span><span id="L-21"><a href="#L-21"><span class="linenos"> 21</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
+</span><span id="L-22"><a href="#L-22"><span class="linenos"> 22</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Name of the package to create in the current working directory. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-23"><a href="#L-23"><span class="linenos"> 23</span></a>    <span class="p">)</span>
+</span><span id="L-24"><a href="#L-24"><span class="linenos"> 24</span></a>
+</span><span id="L-25"><a href="#L-25"><span class="linenos"> 25</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-26"><a href="#L-26"><span class="linenos"> 26</span></a>        <span class="s2">&quot;-s&quot;</span><span class="p">,</span>
+</span><span id="L-27"><a href="#L-27"><span class="linenos"> 27</span></a>        <span class="s2">&quot;--source_files&quot;</span><span class="p">,</span>
+</span><span id="L-28"><a href="#L-28"><span class="linenos"> 28</span></a>        <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;*&quot;</span><span class="p">,</span>
+</span><span id="L-29"><a href="#L-29"><span class="linenos"> 29</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
+</span><span id="L-30"><a href="#L-30"><span class="linenos"> 30</span></a>        <span class="n">default</span><span class="o">=</span><span class="p">[],</span>
+</span><span id="L-31"><a href="#L-31"><span class="linenos"> 31</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; List of additional source files to create in addition to the default</span>
+</span><span id="L-32"><a href="#L-32"><span class="linenos"> 32</span></a><span class="s2">        __init__.py and </span><span class="si">{name}</span><span class="s2">.py files.&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-33"><a href="#L-33"><span class="linenos"> 33</span></a>    <span class="p">)</span>
+</span><span id="L-34"><a href="#L-34"><span class="linenos"> 34</span></a>
+</span><span id="L-35"><a href="#L-35"><span class="linenos"> 35</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-36"><a href="#L-36"><span class="linenos"> 36</span></a>        <span class="s2">&quot;-d&quot;</span><span class="p">,</span>
+</span><span id="L-37"><a href="#L-37"><span class="linenos"> 37</span></a>        <span class="s2">&quot;--description&quot;</span><span class="p">,</span>
+</span><span id="L-38"><a href="#L-38"><span class="linenos"> 38</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
+</span><span id="L-39"><a href="#L-39"><span class="linenos"> 39</span></a>        <span class="n">default</span><span class="o">=</span><span class="s2">&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-40"><a href="#L-40"><span class="linenos"> 40</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; The package description to be added to the pyproject.toml file. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-41"><a href="#L-41"><span class="linenos"> 41</span></a>    <span class="p">)</span>
+</span><span id="L-42"><a href="#L-42"><span class="linenos"> 42</span></a>
+</span><span id="L-43"><a href="#L-43"><span class="linenos"> 43</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-44"><a href="#L-44"><span class="linenos"> 44</span></a>        <span class="s2">&quot;-dp&quot;</span><span class="p">,</span>
+</span><span id="L-45"><a href="#L-45"><span class="linenos"> 45</span></a>        <span class="s2">&quot;--dependencies&quot;</span><span class="p">,</span>
+</span><span id="L-46"><a href="#L-46"><span class="linenos"> 46</span></a>        <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;*&quot;</span><span class="p">,</span>
+</span><span id="L-47"><a href="#L-47"><span class="linenos"> 47</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
+</span><span id="L-48"><a href="#L-48"><span class="linenos"> 48</span></a>        <span class="n">default</span><span class="o">=</span><span class="p">[],</span>
+</span><span id="L-49"><a href="#L-49"><span class="linenos"> 49</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; List of dependencies to add to pyproject.toml.</span>
+</span><span id="L-50"><a href="#L-50"><span class="linenos"> 50</span></a><span class="s2">        Note: hassle.py will automatically scan your project for 3rd party</span>
+</span><span id="L-51"><a href="#L-51"><span class="linenos"> 51</span></a><span class="s2">        imports and update pyproject.toml. This switch is largely useful</span>
+</span><span id="L-52"><a href="#L-52"><span class="linenos"> 52</span></a><span class="s2">        for adding dependencies your project might need, but doesn&#39;t</span>
+</span><span id="L-53"><a href="#L-53"><span class="linenos"> 53</span></a><span class="s2">        directly import in any source files,</span>
+</span><span id="L-54"><a href="#L-54"><span class="linenos"> 54</span></a><span class="s2">        like an os.system() call that invokes a 3rd party cli.&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-55"><a href="#L-55"><span class="linenos"> 55</span></a>    <span class="p">)</span>
+</span><span id="L-56"><a href="#L-56"><span class="linenos"> 56</span></a>
+</span><span id="L-57"><a href="#L-57"><span class="linenos"> 57</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-58"><a href="#L-58"><span class="linenos"> 58</span></a>        <span class="s2">&quot;-k&quot;</span><span class="p">,</span>
+</span><span id="L-59"><a href="#L-59"><span class="linenos"> 59</span></a>        <span class="s2">&quot;--keywords&quot;</span><span class="p">,</span>
+</span><span id="L-60"><a href="#L-60"><span class="linenos"> 60</span></a>        <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;*&quot;</span><span class="p">,</span>
+</span><span id="L-61"><a href="#L-61"><span class="linenos"> 61</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
+</span><span id="L-62"><a href="#L-62"><span class="linenos"> 62</span></a>        <span class="n">default</span><span class="o">=</span><span class="p">[],</span>
+</span><span id="L-63"><a href="#L-63"><span class="linenos"> 63</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; List of keywords to be added to the keywords field in pyproject.toml. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-64"><a href="#L-64"><span class="linenos"> 64</span></a>    <span class="p">)</span>
+</span><span id="L-65"><a href="#L-65"><span class="linenos"> 65</span></a>
+</span><span id="L-66"><a href="#L-66"><span class="linenos"> 66</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-67"><a href="#L-67"><span class="linenos"> 67</span></a>        <span class="s2">&quot;-as&quot;</span><span class="p">,</span>
+</span><span id="L-68"><a href="#L-68"><span class="linenos"> 68</span></a>        <span class="s2">&quot;--add_script&quot;</span><span class="p">,</span>
+</span><span id="L-69"><a href="#L-69"><span class="linenos"> 69</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="L-70"><a href="#L-70"><span class="linenos"> 70</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Add section to pyproject.toml declaring the package </span>
+</span><span id="L-71"><a href="#L-71"><span class="linenos"> 71</span></a><span class="s2">        should be installed with command line scripts added. </span>
+</span><span id="L-72"><a href="#L-72"><span class="linenos"> 72</span></a><span class="s2">        The default is &#39;</span><span class="si">{name}</span><span class="s2"> = &quot;</span><span class="si">{name}</span><span class="s2">.</span><span class="si">{name}</span><span class="s2">:main&quot;.</span>
+</span><span id="L-73"><a href="#L-73"><span class="linenos"> 73</span></a><span class="s2">        You will need to manually change this field.&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-74"><a href="#L-74"><span class="linenos"> 74</span></a>    <span class="p">)</span>
+</span><span id="L-75"><a href="#L-75"><span class="linenos"> 75</span></a>
+</span><span id="L-76"><a href="#L-76"><span class="linenos"> 76</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-77"><a href="#L-77"><span class="linenos"> 77</span></a>        <span class="s2">&quot;-nl&quot;</span><span class="p">,</span>
+</span><span id="L-78"><a href="#L-78"><span class="linenos"> 78</span></a>        <span class="s2">&quot;--no_license&quot;</span><span class="p">,</span>
+</span><span id="L-79"><a href="#L-79"><span class="linenos"> 79</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="L-80"><a href="#L-80"><span class="linenos"> 80</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; By default, projects are created with an MIT license.</span>
+</span><span id="L-81"><a href="#L-81"><span class="linenos"> 81</span></a><span class="s2">        Set this flag to avoid adding a license if you want to configure licensing</span>
+</span><span id="L-82"><a href="#L-82"><span class="linenos"> 82</span></a><span class="s2">        at another time.&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-83"><a href="#L-83"><span class="linenos"> 83</span></a>    <span class="p">)</span>
+</span><span id="L-84"><a href="#L-84"><span class="linenos"> 84</span></a>
+</span><span id="L-85"><a href="#L-85"><span class="linenos"> 85</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-86"><a href="#L-86"><span class="linenos"> 86</span></a>        <span class="s2">&quot;-os&quot;</span><span class="p">,</span>
+</span><span id="L-87"><a href="#L-87"><span class="linenos"> 87</span></a>        <span class="s2">&quot;--operating_system&quot;</span><span class="p">,</span>
+</span><span id="L-88"><a href="#L-88"><span class="linenos"> 88</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
+</span><span id="L-89"><a href="#L-89"><span class="linenos"> 89</span></a>        <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
+</span><span id="L-90"><a href="#L-90"><span class="linenos"> 90</span></a>        <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;*&quot;</span><span class="p">,</span>
+</span><span id="L-91"><a href="#L-91"><span class="linenos"> 91</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; List of operating systems this package will be compatible with.</span>
+</span><span id="L-92"><a href="#L-92"><span class="linenos"> 92</span></a><span class="s2">        The default is OS Independent.</span>
+</span><span id="L-93"><a href="#L-93"><span class="linenos"> 93</span></a><span class="s2">        This only affects the &#39;classifiers&#39; field of pyproject.toml .&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-94"><a href="#L-94"><span class="linenos"> 94</span></a>    <span class="p">)</span>
+</span><span id="L-95"><a href="#L-95"><span class="linenos"> 95</span></a>
+</span><span id="L-96"><a href="#L-96"><span class="linenos"> 96</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-97"><a href="#L-97"><span class="linenos"> 97</span></a>        <span class="s2">&quot;-np&quot;</span><span class="p">,</span>
+</span><span id="L-98"><a href="#L-98"><span class="linenos"> 98</span></a>        <span class="s2">&quot;--not_package&quot;</span><span class="p">,</span>
+</span><span id="L-99"><a href="#L-99"><span class="linenos"> 99</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="L-100"><a href="#L-100"><span class="linenos">100</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Put source files in top level directory and delete tests folder. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-101"><a href="#L-101"><span class="linenos">101</span></a>    <span class="p">)</span>
+</span><span id="L-102"><a href="#L-102"><span class="linenos">102</span></a>
+</span><span id="L-103"><a href="#L-103"><span class="linenos">103</span></a>    <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="o">.</span><span class="n">parse_args</span><span class="p">()</span>
+</span><span id="L-104"><a href="#L-104"><span class="linenos">104</span></a>    <span class="n">args</span><span class="o">.</span><span class="n">source_files</span><span class="o">.</span><span class="n">extend</span><span class="p">([</span><span class="s2">&quot;__init__.py&quot;</span><span class="p">,</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2">.py&quot;</span><span class="p">])</span>
+</span><span id="L-105"><a href="#L-105"><span class="linenos">105</span></a>
+</span><span id="L-106"><a href="#L-106"><span class="linenos">106</span></a>    <span class="k">return</span> <span class="n">args</span>
 </span><span id="L-107"><a href="#L-107"><span class="linenos">107</span></a>
-</span><span id="L-108"><a href="#L-108"><span class="linenos">108</span></a>    <span class="k">return</span> <span class="n">args</span>
-</span><span id="L-109"><a href="#L-109"><span class="linenos">109</span></a>
-</span><span id="L-110"><a href="#L-110"><span class="linenos">110</span></a>
-</span><span id="L-111"><a href="#L-111"><span class="linenos">111</span></a><span class="k">def</span> <span class="nf">get_answer</span><span class="p">(</span><span class="n">question</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
-</span><span id="L-112"><a href="#L-112"><span class="linenos">112</span></a>    <span class="sd">&quot;&quot;&quot;Repeatedly ask the user a yes/no question</span>
-</span><span id="L-113"><a href="#L-113"><span class="linenos">113</span></a><span class="sd">    until a &#39;y&#39; or a &#39;n&#39; is received.&quot;&quot;&quot;</span>
-</span><span id="L-114"><a href="#L-114"><span class="linenos">114</span></a>    <span class="n">ans</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
-</span><span id="L-115"><a href="#L-115"><span class="linenos">115</span></a>    <span class="n">question</span> <span class="o">=</span> <span class="n">question</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span>
-</span><span id="L-116"><a href="#L-116"><span class="linenos">116</span></a>    <span class="k">if</span> <span class="s2">&quot;?&quot;</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">question</span><span class="p">:</span>
-</span><span id="L-117"><a href="#L-117"><span class="linenos">117</span></a>        <span class="n">question</span> <span class="o">+=</span> <span class="s2">&quot;?&quot;</span>
-</span><span id="L-118"><a href="#L-118"><span class="linenos">118</span></a>    <span class="n">question</span> <span class="o">+=</span> <span class="s2">&quot; (y/n): &quot;</span>
-</span><span id="L-119"><a href="#L-119"><span class="linenos">119</span></a>    <span class="k">while</span> <span class="n">ans</span> <span class="ow">not</span> <span class="ow">in</span> <span class="p">[</span><span class="s2">&quot;y&quot;</span><span class="p">,</span> <span class="s2">&quot;yes&quot;</span><span class="p">,</span> <span class="s2">&quot;no&quot;</span><span class="p">,</span> <span class="s2">&quot;n&quot;</span><span class="p">]:</span>
-</span><span id="L-120"><a href="#L-120"><span class="linenos">120</span></a>        <span class="n">ans</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span><span class="n">question</span><span class="p">)</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span>
-</span><span id="L-121"><a href="#L-121"><span class="linenos">121</span></a>        <span class="k">if</span> <span class="n">ans</span> <span class="ow">in</span> <span class="p">[</span><span class="s2">&quot;y&quot;</span><span class="p">,</span> <span class="s2">&quot;yes&quot;</span><span class="p">]:</span>
-</span><span id="L-122"><a href="#L-122"><span class="linenos">122</span></a>            <span class="k">return</span> <span class="kc">True</span>
-</span><span id="L-123"><a href="#L-123"><span class="linenos">123</span></a>        <span class="k">elif</span> <span class="n">ans</span> <span class="ow">in</span> <span class="p">[</span><span class="s2">&quot;n&quot;</span><span class="p">,</span> <span class="s2">&quot;no&quot;</span><span class="p">]:</span>
-</span><span id="L-124"><a href="#L-124"><span class="linenos">124</span></a>            <span class="k">return</span> <span class="kc">False</span>
-</span><span id="L-125"><a href="#L-125"><span class="linenos">125</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="L-126"><a href="#L-126"><span class="linenos">126</span></a>            <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Invalid answer.&quot;</span><span class="p">)</span>
-</span><span id="L-127"><a href="#L-127"><span class="linenos">127</span></a>
-</span><span id="L-128"><a href="#L-128"><span class="linenos">128</span></a>
-</span><span id="L-129"><a href="#L-129"><span class="linenos">129</span></a><span class="k">def</span> <span class="nf">check_pypi_for_name</span><span class="p">(</span><span class="n">package_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
-</span><span id="L-130"><a href="#L-130"><span class="linenos">130</span></a>    <span class="sd">&quot;&quot;&quot;Check if a package with package_name</span>
-</span><span id="L-131"><a href="#L-131"><span class="linenos">131</span></a><span class="sd">    already exists on pypi.org .</span>
-</span><span id="L-132"><a href="#L-132"><span class="linenos">132</span></a><span class="sd">    Returns True if package name exists.</span>
-</span><span id="L-133"><a href="#L-133"><span class="linenos">133</span></a><span class="sd">    Only checks the first page of results.&quot;&quot;&quot;</span>
-</span><span id="L-134"><a href="#L-134"><span class="linenos">134</span></a>    <span class="n">url</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;https://pypi.org/search/?q=</span><span class="si">{</span><span class="n">package_name</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="L-135"><a href="#L-135"><span class="linenos">135</span></a>    <span class="n">response</span> <span class="o">=</span> <span class="n">requests</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="n">url</span><span class="p">)</span>
-</span><span id="L-136"><a href="#L-136"><span class="linenos">136</span></a>    <span class="k">if</span> <span class="n">response</span><span class="o">.</span><span class="n">status_code</span> <span class="o">!=</span> <span class="mi">200</span><span class="p">:</span>
-</span><span id="L-137"><a href="#L-137"><span class="linenos">137</span></a>        <span class="k">raise</span> <span class="ne">RuntimeError</span><span class="p">(</span>
-</span><span id="L-138"><a href="#L-138"><span class="linenos">138</span></a>            <span class="sa">f</span><span class="s2">&quot;Error: pypi.org returned status code: </span><span class="si">{</span><span class="n">response</span><span class="o">.</span><span class="n">status_code</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="L-139"><a href="#L-139"><span class="linenos">139</span></a>        <span class="p">)</span>
-</span><span id="L-140"><a href="#L-140"><span class="linenos">140</span></a>    <span class="n">soup</span> <span class="o">=</span> <span class="n">BeautifulSoup</span><span class="p">(</span><span class="n">response</span><span class="o">.</span><span class="n">text</span><span class="p">,</span> <span class="s2">&quot;html.parser&quot;</span><span class="p">)</span>
-</span><span id="L-141"><a href="#L-141"><span class="linenos">141</span></a>    <span class="n">pypi_packages</span> <span class="o">=</span> <span class="p">[</span>
-</span><span id="L-142"><a href="#L-142"><span class="linenos">142</span></a>        <span class="n">span</span><span class="o">.</span><span class="n">text</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span>
-</span><span id="L-143"><a href="#L-143"><span class="linenos">143</span></a>        <span class="k">for</span> <span class="n">span</span> <span class="ow">in</span> <span class="n">soup</span><span class="o">.</span><span class="n">find_all</span><span class="p">(</span><span class="s2">&quot;span&quot;</span><span class="p">,</span> <span class="n">class_</span><span class="o">=</span><span class="s2">&quot;package-snippet__name&quot;</span><span class="p">)</span>
-</span><span id="L-144"><a href="#L-144"><span class="linenos">144</span></a>    <span class="p">]</span>
-</span><span id="L-145"><a href="#L-145"><span class="linenos">145</span></a>    <span class="k">return</span> <span class="n">package_name</span> <span class="ow">in</span> <span class="n">pypi_packages</span>
-</span><span id="L-146"><a href="#L-146"><span class="linenos">146</span></a>
-</span><span id="L-147"><a href="#L-147"><span class="linenos">147</span></a>
-</span><span id="L-148"><a href="#L-148"><span class="linenos">148</span></a><span class="k">def</span> <span class="nf">check_pypi_for_name_cli</span><span class="p">():</span>
-</span><span id="L-149"><a href="#L-149"><span class="linenos">149</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">argparse</span><span class="o">.</span><span class="n">ArgumentParser</span><span class="p">()</span>
-</span><span id="L-150"><a href="#L-150"><span class="linenos">150</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span><span class="s2">&quot;name&quot;</span><span class="p">,</span> <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">)</span>
-</span><span id="L-151"><a href="#L-151"><span class="linenos">151</span></a>    <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="o">.</span><span class="n">parse_args</span><span class="p">()</span>
-</span><span id="L-152"><a href="#L-152"><span class="linenos">152</span></a>    <span class="k">if</span> <span class="n">check_pypi_for_name</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="p">):</span>
-</span><span id="L-153"><a href="#L-153"><span class="linenos">153</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2"> is already taken.&quot;</span><span class="p">)</span>
-</span><span id="L-154"><a href="#L-154"><span class="linenos">154</span></a>    <span class="k">else</span><span class="p">:</span>
-</span><span id="L-155"><a href="#L-155"><span class="linenos">155</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2"> is available.&quot;</span><span class="p">)</span>
-</span><span id="L-156"><a href="#L-156"><span class="linenos">156</span></a>
-</span><span id="L-157"><a href="#L-157"><span class="linenos">157</span></a>
-</span><span id="L-158"><a href="#L-158"><span class="linenos">158</span></a><span class="k">def</span> <span class="nf">create_pyproject_file</span><span class="p">(</span><span class="n">targetdir</span><span class="p">:</span> <span class="n">Path</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
-</span><span id="L-159"><a href="#L-159"><span class="linenos">159</span></a>    <span class="sd">&quot;&quot;&quot;Create pyproject.toml in ./{project_name} from args,</span>
-</span><span id="L-160"><a href="#L-160"><span class="linenos">160</span></a><span class="sd">    pyproject_template, and hassle_config.&quot;&quot;&quot;</span>
-</span><span id="L-161"><a href="#L-161"><span class="linenos">161</span></a>    <span class="n">pyproject</span> <span class="o">=</span> <span class="n">tomlkit</span><span class="o">.</span><span class="n">loads</span><span class="p">((</span><span class="n">root</span> <span class="o">/</span> <span class="s2">&quot;pyproject_template.toml&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">read_text</span><span class="p">())</span>
-</span><span id="L-162"><a href="#L-162"><span class="linenos">162</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">hassle_config</span><span class="o">.</span><span class="n">config_exists</span><span class="p">():</span>
-</span><span id="L-163"><a href="#L-163"><span class="linenos">163</span></a>        <span class="n">hassle_config</span><span class="o">.</span><span class="n">warn</span><span class="p">()</span>
-</span><span id="L-164"><a href="#L-164"><span class="linenos">164</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">get_answer</span><span class="p">(</span><span class="s2">&quot;Continue creating new package with blank config?&quot;</span><span class="p">):</span>
-</span><span id="L-165"><a href="#L-165"><span class="linenos">165</span></a>            <span class="k">raise</span> <span class="ne">Exception</span><span class="p">(</span><span class="s2">&quot;Aborting new package creation&quot;</span><span class="p">)</span>
-</span><span id="L-166"><a href="#L-166"><span class="linenos">166</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="L-167"><a href="#L-167"><span class="linenos">167</span></a>            <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Creating blank hassle_config.toml...&quot;</span><span class="p">)</span>
-</span><span id="L-168"><a href="#L-168"><span class="linenos">168</span></a>            <span class="n">hassle_config</span><span class="o">.</span><span class="n">create_config</span><span class="p">()</span>
-</span><span id="L-169"><a href="#L-169"><span class="linenos">169</span></a>    <span class="n">config</span> <span class="o">=</span> <span class="n">hassle_config</span><span class="o">.</span><span class="n">load_config</span><span class="p">()</span>
-</span><span id="L-170"><a href="#L-170"><span class="linenos">170</span></a>    <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;name&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">name</span>
-</span><span id="L-171"><a href="#L-171"><span class="linenos">171</span></a>    <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;authors&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">config</span><span class="p">[</span><span class="s2">&quot;authors&quot;</span><span class="p">]</span>
-</span><span id="L-172"><a href="#L-172"><span class="linenos">172</span></a>    <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;description&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">description</span>
-</span><span id="L-173"><a href="#L-173"><span class="linenos">173</span></a>    <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;dependencies&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">dependencies</span>
-</span><span id="L-174"><a href="#L-174"><span class="linenos">174</span></a>    <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;keywords&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">keywords</span>
-</span><span id="L-175"><a href="#L-175"><span class="linenos">175</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">operating_system</span><span class="p">:</span>
-</span><span id="L-176"><a href="#L-176"><span class="linenos">176</span></a>        <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;classifiers&quot;</span><span class="p">][</span><span class="mi">2</span><span class="p">]</span> <span class="o">=</span> <span class="s2">&quot;Operating System :: &quot;</span> <span class="o">+</span> <span class="s2">&quot; &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span>
-</span><span id="L-177"><a href="#L-177"><span class="linenos">177</span></a>            <span class="n">args</span><span class="o">.</span><span class="n">operating_system</span>
-</span><span id="L-178"><a href="#L-178"><span class="linenos">178</span></a>        <span class="p">)</span>
-</span><span id="L-179"><a href="#L-179"><span class="linenos">179</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">no_license</span><span class="p">:</span>
-</span><span id="L-180"><a href="#L-180"><span class="linenos">180</span></a>        <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;classifiers&quot;</span><span class="p">]</span><span class="o">.</span><span class="n">pop</span><span class="p">(</span><span class="mi">1</span><span class="p">)</span>
-</span><span id="L-181"><a href="#L-181"><span class="linenos">181</span></a>    <span class="k">for</span> <span class="n">field</span> <span class="ow">in</span> <span class="n">config</span><span class="p">[</span><span class="s2">&quot;project_urls&quot;</span><span class="p">]:</span>
-</span><span id="L-182"><a href="#L-182"><span class="linenos">182</span></a>        <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;urls&quot;</span><span class="p">][</span><span class="n">field</span><span class="p">]</span> <span class="o">=</span> <span class="n">config</span><span class="p">[</span><span class="s2">&quot;project_urls&quot;</span><span class="p">][</span><span class="n">field</span><span class="p">]</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span>
-</span><span id="L-183"><a href="#L-183"><span class="linenos">183</span></a>            <span class="s2">&quot;$name&quot;</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">name</span>
-</span><span id="L-184"><a href="#L-184"><span class="linenos">184</span></a>        <span class="p">)</span>
-</span><span id="L-185"><a href="#L-185"><span class="linenos">185</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">add_script</span><span class="p">:</span>
-</span><span id="L-186"><a href="#L-186"><span class="linenos">186</span></a>        <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;scripts&quot;</span><span class="p">][</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="p">]</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2">.</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2">:main&quot;</span>
-</span><span id="L-187"><a href="#L-187"><span class="linenos">187</span></a>    <span class="p">(</span><span class="n">targetdir</span> <span class="o">/</span> <span class="s2">&quot;pyproject.toml&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="n">tomlkit</span><span class="o">.</span><span class="n">dumps</span><span class="p">(</span><span class="n">pyproject</span><span class="p">))</span>
-</span><span id="L-188"><a href="#L-188"><span class="linenos">188</span></a>
-</span><span id="L-189"><a href="#L-189"><span class="linenos">189</span></a>
-</span><span id="L-190"><a href="#L-190"><span class="linenos">190</span></a><span class="k">def</span> <span class="nf">create_source_files</span><span class="p">(</span><span class="n">srcdir</span><span class="p">:</span> <span class="n">Path</span><span class="p">,</span> <span class="n">filelist</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]):</span>
-</span><span id="L-191"><a href="#L-191"><span class="linenos">191</span></a>    <span class="sd">&quot;&quot;&quot;Generate empty source files in ./{package_name}/src/{package_name}/&quot;&quot;&quot;</span>
-</span><span id="L-192"><a href="#L-192"><span class="linenos">192</span></a>    <span class="n">srcdir</span><span class="o">.</span><span class="n">mkdir</span><span class="p">(</span><span class="n">parents</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">exist_ok</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
-</span><span id="L-193"><a href="#L-193"><span class="linenos">193</span></a>    <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">filelist</span><span class="p">:</span>
-</span><span id="L-194"><a href="#L-194"><span class="linenos">194</span></a>        <span class="p">(</span><span class="n">srcdir</span> <span class="o">/</span> <span class="n">file</span><span class="p">)</span><span class="o">.</span><span class="n">touch</span><span class="p">()</span>
-</span><span id="L-195"><a href="#L-195"><span class="linenos">195</span></a>
-</span><span id="L-196"><a href="#L-196"><span class="linenos">196</span></a>
-</span><span id="L-197"><a href="#L-197"><span class="linenos">197</span></a><span class="k">def</span> <span class="nf">create_readme</span><span class="p">(</span><span class="n">targetdir</span><span class="p">:</span> <span class="n">Path</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
-</span><span id="L-198"><a href="#L-198"><span class="linenos">198</span></a>    <span class="sd">&quot;&quot;&quot;Create README.md in ./{package_name}</span>
-</span><span id="L-199"><a href="#L-199"><span class="linenos">199</span></a><span class="sd">    from readme_template and args.&quot;&quot;&quot;</span>
-</span><span id="L-200"><a href="#L-200"><span class="linenos">200</span></a>    <span class="n">readme</span> <span class="o">=</span> <span class="p">(</span><span class="n">root</span> <span class="o">/</span> <span class="s2">&quot;README_template.md&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">read_text</span><span class="p">()</span>
-</span><span id="L-201"><a href="#L-201"><span class="linenos">201</span></a>    <span class="n">readme</span> <span class="o">=</span> <span class="n">readme</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;$name&quot;</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="p">)</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span>
-</span><span id="L-202"><a href="#L-202"><span class="linenos">202</span></a>        <span class="s2">&quot;$description&quot;</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">description</span>
-</span><span id="L-203"><a href="#L-203"><span class="linenos">203</span></a>    <span class="p">)</span>
-</span><span id="L-204"><a href="#L-204"><span class="linenos">204</span></a>    <span class="p">(</span><span class="n">targetdir</span> <span class="o">/</span> <span class="s2">&quot;README.md&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="n">readme</span><span class="p">)</span>
-</span><span id="L-205"><a href="#L-205"><span class="linenos">205</span></a>
-</span><span id="L-206"><a href="#L-206"><span class="linenos">206</span></a>
-</span><span id="L-207"><a href="#L-207"><span class="linenos">207</span></a><span class="k">def</span> <span class="nf">create_license</span><span class="p">(</span><span class="n">targetdir</span><span class="p">:</span> <span class="n">Path</span><span class="p">):</span>
-</span><span id="L-208"><a href="#L-208"><span class="linenos">208</span></a>    <span class="sd">&quot;&quot;&quot;Add MIT license file to ./{package_name} .&quot;&quot;&quot;</span>
-</span><span id="L-209"><a href="#L-209"><span class="linenos">209</span></a>    <span class="n">license_template</span> <span class="o">=</span> <span class="p">(</span><span class="n">root</span> <span class="o">/</span> <span class="s2">&quot;license_template.txt&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">read_text</span><span class="p">()</span>
-</span><span id="L-210"><a href="#L-210"><span class="linenos">210</span></a>    <span class="n">license_template</span> <span class="o">=</span> <span class="n">license_template</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;$year&quot;</span><span class="p">,</span> <span class="nb">str</span><span class="p">(</span><span class="n">datetime</span><span class="o">.</span><span class="n">now</span><span class="p">()</span><span class="o">.</span><span class="n">year</span><span class="p">))</span>
-</span><span id="L-211"><a href="#L-211"><span class="linenos">211</span></a>    <span class="p">(</span><span class="n">targetdir</span> <span class="o">/</span> <span class="s2">&quot;LICENSE.txt&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="n">license_template</span><span class="p">)</span>
-</span><span id="L-212"><a href="#L-212"><span class="linenos">212</span></a>
-</span><span id="L-213"><a href="#L-213"><span class="linenos">213</span></a>
-</span><span id="L-214"><a href="#L-214"><span class="linenos">214</span></a><span class="k">def</span> <span class="nf">create_gitignore</span><span class="p">(</span><span class="n">targetdir</span><span class="p">:</span> <span class="n">Path</span><span class="p">):</span>
-</span><span id="L-215"><a href="#L-215"><span class="linenos">215</span></a>    <span class="sd">&quot;&quot;&quot;Add .gitignore to ./{package_name}&quot;&quot;&quot;</span>
-</span><span id="L-216"><a href="#L-216"><span class="linenos">216</span></a>    <span class="n">shutil</span><span class="o">.</span><span class="n">copy</span><span class="p">(</span><span class="n">root</span> <span class="o">/</span> <span class="s2">&quot;.gitignore_template&quot;</span><span class="p">,</span> <span class="n">targetdir</span> <span class="o">/</span> <span class="s2">&quot;.gitignore&quot;</span><span class="p">)</span>
-</span><span id="L-217"><a href="#L-217"><span class="linenos">217</span></a>
-</span><span id="L-218"><a href="#L-218"><span class="linenos">218</span></a>
-</span><span id="L-219"><a href="#L-219"><span class="linenos">219</span></a><span class="k">def</span> <span class="nf">create_vscode_settings</span><span class="p">(</span><span class="n">targetdir</span><span class="p">:</span> <span class="n">Path</span><span class="p">):</span>
-</span><span id="L-220"><a href="#L-220"><span class="linenos">220</span></a>    <span class="sd">&quot;&quot;&quot;Add settings.json to ./.vscode&quot;&quot;&quot;</span>
-</span><span id="L-221"><a href="#L-221"><span class="linenos">221</span></a>    <span class="n">vsdir</span> <span class="o">=</span> <span class="n">targetdir</span> <span class="o">/</span> <span class="s2">&quot;.vscode&quot;</span>
-</span><span id="L-222"><a href="#L-222"><span class="linenos">222</span></a>    <span class="n">vsdir</span><span class="o">.</span><span class="n">mkdir</span><span class="p">(</span><span class="n">parents</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">exist_ok</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
-</span><span id="L-223"><a href="#L-223"><span class="linenos">223</span></a>    <span class="n">shutil</span><span class="o">.</span><span class="n">copy</span><span class="p">(</span><span class="n">root</span> <span class="o">/</span> <span class="s2">&quot;.vscode_template&quot;</span><span class="p">,</span> <span class="n">vsdir</span> <span class="o">/</span> <span class="s2">&quot;settings.json&quot;</span><span class="p">)</span>
-</span><span id="L-224"><a href="#L-224"><span class="linenos">224</span></a>
-</span><span id="L-225"><a href="#L-225"><span class="linenos">225</span></a>
-</span><span id="L-226"><a href="#L-226"><span class="linenos">226</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
-</span><span id="L-227"><a href="#L-227"><span class="linenos">227</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="p">:</span>
-</span><span id="L-228"><a href="#L-228"><span class="linenos">228</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
-</span><span id="L-229"><a href="#L-229"><span class="linenos">229</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">not_package</span><span class="p">:</span>
-</span><span id="L-230"><a href="#L-230"><span class="linenos">230</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="L-231"><a href="#L-231"><span class="linenos">231</span></a>            <span class="k">if</span> <span class="n">check_pypi_for_name</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="p">):</span>
-</span><span id="L-232"><a href="#L-232"><span class="linenos">232</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2"> already exists on pypi.org&quot;</span><span class="p">)</span>
-</span><span id="L-233"><a href="#L-233"><span class="linenos">233</span></a>                <span class="k">if</span> <span class="ow">not</span> <span class="n">get_answer</span><span class="p">(</span><span class="s2">&quot;Continue anyway?&quot;</span><span class="p">):</span>
-</span><span id="L-234"><a href="#L-234"><span class="linenos">234</span></a>                    <span class="n">sys</span><span class="o">.</span><span class="n">exit</span><span class="p">(</span><span class="mi">0</span><span class="p">)</span>
-</span><span id="L-235"><a href="#L-235"><span class="linenos">235</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="L-236"><a href="#L-236"><span class="linenos">236</span></a>            <span class="nb">print</span><span class="p">(</span><span class="n">e</span><span class="p">)</span>
-</span><span id="L-237"><a href="#L-237"><span class="linenos">237</span></a>            <span class="nb">print</span><span class="p">(</span>
-</span><span id="L-238"><a href="#L-238"><span class="linenos">238</span></a>                <span class="sa">f</span><span class="s2">&quot;Couldn&#39;t verify that </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2"> doesn&#39;t already exist on pypi.org .&quot;</span>
-</span><span id="L-239"><a href="#L-239"><span class="linenos">239</span></a>            <span class="p">)</span>
-</span><span id="L-240"><a href="#L-240"><span class="linenos">240</span></a>            <span class="k">if</span> <span class="ow">not</span> <span class="n">get_answer</span><span class="p">(</span><span class="s2">&quot;Continue anyway?&quot;</span><span class="p">):</span>
-</span><span id="L-241"><a href="#L-241"><span class="linenos">241</span></a>                <span class="n">sys</span><span class="o">.</span><span class="n">exit</span><span class="p">(</span><span class="mi">0</span><span class="p">)</span>
-</span><span id="L-242"><a href="#L-242"><span class="linenos">242</span></a>    <span class="k">try</span><span class="p">:</span>
-</span><span id="L-243"><a href="#L-243"><span class="linenos">243</span></a>        <span class="n">targetdir</span> <span class="o">=</span> <span class="n">Path</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span> <span class="o">/</span> <span class="n">args</span><span class="o">.</span><span class="n">name</span>
-</span><span id="L-244"><a href="#L-244"><span class="linenos">244</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="L-245"><a href="#L-245"><span class="linenos">245</span></a>            <span class="n">targetdir</span><span class="o">.</span><span class="n">mkdir</span><span class="p">(</span><span class="n">parents</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">exist_ok</span><span class="o">=</span><span class="kc">False</span><span class="p">)</span>
-</span><span id="L-246"><a href="#L-246"><span class="linenos">246</span></a>        <span class="k">except</span><span class="p">:</span>
-</span><span id="L-247"><a href="#L-247"><span class="linenos">247</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">targetdir</span><span class="si">}</span><span class="s2"> already exists.&quot;</span><span class="p">)</span>
-</span><span id="L-248"><a href="#L-248"><span class="linenos">248</span></a>            <span class="k">if</span> <span class="ow">not</span> <span class="n">get_answer</span><span class="p">(</span><span class="s2">&quot;Overwrite?&quot;</span><span class="p">):</span>
-</span><span id="L-249"><a href="#L-249"><span class="linenos">249</span></a>                <span class="n">sys</span><span class="o">.</span><span class="n">exit</span><span class="p">(</span><span class="mi">0</span><span class="p">)</span>
-</span><span id="L-250"><a href="#L-250"><span class="linenos">250</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">not_package</span><span class="p">:</span>
-</span><span id="L-251"><a href="#L-251"><span class="linenos">251</span></a>            <span class="n">create_pyproject_file</span><span class="p">(</span><span class="n">targetdir</span><span class="p">,</span> <span class="n">args</span><span class="p">)</span>
-</span><span id="L-252"><a href="#L-252"><span class="linenos">252</span></a>        <span class="n">create_source_files</span><span class="p">(</span>
-</span><span id="L-253"><a href="#L-253"><span class="linenos">253</span></a>            <span class="n">targetdir</span> <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">not_package</span> <span class="k">else</span> <span class="p">(</span><span class="n">targetdir</span> <span class="o">/</span> <span class="s2">&quot;src&quot;</span> <span class="o">/</span> <span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="p">),</span>
-</span><span id="L-254"><a href="#L-254"><span class="linenos">254</span></a>            <span class="n">args</span><span class="o">.</span><span class="n">source_files</span><span class="p">[</span><span class="mi">1</span><span class="p">:]</span> <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">not_package</span> <span class="k">else</span> <span class="n">args</span><span class="o">.</span><span class="n">source_files</span><span class="p">,</span>
-</span><span id="L-255"><a href="#L-255"><span class="linenos">255</span></a>        <span class="p">)</span>
-</span><span id="L-256"><a href="#L-256"><span class="linenos">256</span></a>        <span class="n">create_readme</span><span class="p">(</span><span class="n">targetdir</span><span class="p">,</span> <span class="n">args</span><span class="p">)</span>
-</span><span id="L-257"><a href="#L-257"><span class="linenos">257</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">not_package</span><span class="p">:</span>
-</span><span id="L-258"><a href="#L-258"><span class="linenos">258</span></a>            <span class="n">generate_test_files</span><span class="p">(</span><span class="n">targetdir</span><span class="p">)</span>
-</span><span id="L-259"><a href="#L-259"><span class="linenos">259</span></a>            <span class="n">create_vscode_settings</span><span class="p">(</span><span class="n">targetdir</span><span class="p">)</span>
-</span><span id="L-260"><a href="#L-260"><span class="linenos">260</span></a>        <span class="n">create_gitignore</span><span class="p">(</span><span class="n">targetdir</span><span class="p">)</span>
-</span><span id="L-261"><a href="#L-261"><span class="linenos">261</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">no_license</span><span class="p">:</span>
-</span><span id="L-262"><a href="#L-262"><span class="linenos">262</span></a>            <span class="n">create_license</span><span class="p">(</span><span class="n">targetdir</span><span class="p">)</span>
-</span><span id="L-263"><a href="#L-263"><span class="linenos">263</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">targetdir</span><span class="p">)</span>
-</span><span id="L-264"><a href="#L-264"><span class="linenos">264</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="s2">&quot;git init -b main&quot;</span><span class="p">)</span>
-</span><span id="L-265"><a href="#L-265"><span class="linenos">265</span></a>
-</span><span id="L-266"><a href="#L-266"><span class="linenos">266</span></a>    <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="L-267"><a href="#L-267"><span class="linenos">267</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="s2">&quot;Aborting new package creation&quot;</span> <span class="ow">in</span> <span class="nb">str</span><span class="p">(</span><span class="n">e</span><span class="p">):</span>
-</span><span id="L-268"><a href="#L-268"><span class="linenos">268</span></a>            <span class="nb">print</span><span class="p">(</span><span class="n">e</span><span class="p">)</span>
-</span><span id="L-269"><a href="#L-269"><span class="linenos">269</span></a>        <span class="k">if</span> <span class="n">get_answer</span><span class="p">(</span><span class="s2">&quot;Delete created files?&quot;</span><span class="p">):</span>
-</span><span id="L-270"><a href="#L-270"><span class="linenos">270</span></a>            <span class="n">shutil</span><span class="o">.</span><span class="n">rmtree</span><span class="p">(</span><span class="n">targetdir</span><span class="p">)</span>
-</span><span id="L-271"><a href="#L-271"><span class="linenos">271</span></a>
-</span><span id="L-272"><a href="#L-272"><span class="linenos">272</span></a>
-</span><span id="L-273"><a href="#L-273"><span class="linenos">273</span></a><span class="k">if</span> <span class="vm">__name__</span> <span class="o">==</span> <span class="s2">&quot;__main__&quot;</span><span class="p">:</span>
-</span><span id="L-274"><a href="#L-274"><span class="linenos">274</span></a>    <span class="n">main</span><span class="p">(</span><span class="n">get_args</span><span class="p">())</span>
+</span><span id="L-108"><a href="#L-108"><span class="linenos">108</span></a>
+</span><span id="L-109"><a href="#L-109"><span class="linenos">109</span></a><span class="k">def</span> <span class="nf">get_answer</span><span class="p">(</span><span class="n">question</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
+</span><span id="L-110"><a href="#L-110"><span class="linenos">110</span></a>    <span class="sd">&quot;&quot;&quot;Repeatedly ask the user a yes/no question</span>
+</span><span id="L-111"><a href="#L-111"><span class="linenos">111</span></a><span class="sd">    until a &#39;y&#39; or a &#39;n&#39; is received.&quot;&quot;&quot;</span>
+</span><span id="L-112"><a href="#L-112"><span class="linenos">112</span></a>    <span class="n">ans</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
+</span><span id="L-113"><a href="#L-113"><span class="linenos">113</span></a>    <span class="n">question</span> <span class="o">=</span> <span class="n">question</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span>
+</span><span id="L-114"><a href="#L-114"><span class="linenos">114</span></a>    <span class="k">if</span> <span class="s2">&quot;?&quot;</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">question</span><span class="p">:</span>
+</span><span id="L-115"><a href="#L-115"><span class="linenos">115</span></a>        <span class="n">question</span> <span class="o">+=</span> <span class="s2">&quot;?&quot;</span>
+</span><span id="L-116"><a href="#L-116"><span class="linenos">116</span></a>    <span class="n">question</span> <span class="o">+=</span> <span class="s2">&quot; (y/n): &quot;</span>
+</span><span id="L-117"><a href="#L-117"><span class="linenos">117</span></a>    <span class="k">while</span> <span class="n">ans</span> <span class="ow">not</span> <span class="ow">in</span> <span class="p">[</span><span class="s2">&quot;y&quot;</span><span class="p">,</span> <span class="s2">&quot;yes&quot;</span><span class="p">,</span> <span class="s2">&quot;no&quot;</span><span class="p">,</span> <span class="s2">&quot;n&quot;</span><span class="p">]:</span>
+</span><span id="L-118"><a href="#L-118"><span class="linenos">118</span></a>        <span class="n">ans</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span><span class="n">question</span><span class="p">)</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span>
+</span><span id="L-119"><a href="#L-119"><span class="linenos">119</span></a>        <span class="k">if</span> <span class="n">ans</span> <span class="ow">in</span> <span class="p">[</span><span class="s2">&quot;y&quot;</span><span class="p">,</span> <span class="s2">&quot;yes&quot;</span><span class="p">]:</span>
+</span><span id="L-120"><a href="#L-120"><span class="linenos">120</span></a>            <span class="k">return</span> <span class="kc">True</span>
+</span><span id="L-121"><a href="#L-121"><span class="linenos">121</span></a>        <span class="k">elif</span> <span class="n">ans</span> <span class="ow">in</span> <span class="p">[</span><span class="s2">&quot;n&quot;</span><span class="p">,</span> <span class="s2">&quot;no&quot;</span><span class="p">]:</span>
+</span><span id="L-122"><a href="#L-122"><span class="linenos">122</span></a>            <span class="k">return</span> <span class="kc">False</span>
+</span><span id="L-123"><a href="#L-123"><span class="linenos">123</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="L-124"><a href="#L-124"><span class="linenos">124</span></a>            <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Invalid answer.&quot;</span><span class="p">)</span>
+</span><span id="L-125"><a href="#L-125"><span class="linenos">125</span></a>
+</span><span id="L-126"><a href="#L-126"><span class="linenos">126</span></a>
+</span><span id="L-127"><a href="#L-127"><span class="linenos">127</span></a><span class="k">def</span> <span class="nf">check_pypi_for_name</span><span class="p">(</span><span class="n">package_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
+</span><span id="L-128"><a href="#L-128"><span class="linenos">128</span></a>    <span class="sd">&quot;&quot;&quot;Check if a package with package_name</span>
+</span><span id="L-129"><a href="#L-129"><span class="linenos">129</span></a><span class="sd">    already exists on pypi.org .</span>
+</span><span id="L-130"><a href="#L-130"><span class="linenos">130</span></a><span class="sd">    Returns True if package name exists.</span>
+</span><span id="L-131"><a href="#L-131"><span class="linenos">131</span></a><span class="sd">    Only checks the first page of results.&quot;&quot;&quot;</span>
+</span><span id="L-132"><a href="#L-132"><span class="linenos">132</span></a>    <span class="n">url</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;https://pypi.org/search/?q=</span><span class="si">{</span><span class="n">package_name</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="L-133"><a href="#L-133"><span class="linenos">133</span></a>    <span class="n">response</span> <span class="o">=</span> <span class="n">requests</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="n">url</span><span class="p">)</span>
+</span><span id="L-134"><a href="#L-134"><span class="linenos">134</span></a>    <span class="k">if</span> <span class="n">response</span><span class="o">.</span><span class="n">status_code</span> <span class="o">!=</span> <span class="mi">200</span><span class="p">:</span>
+</span><span id="L-135"><a href="#L-135"><span class="linenos">135</span></a>        <span class="k">raise</span> <span class="ne">RuntimeError</span><span class="p">(</span>
+</span><span id="L-136"><a href="#L-136"><span class="linenos">136</span></a>            <span class="sa">f</span><span class="s2">&quot;Error: pypi.org returned status code: </span><span class="si">{</span><span class="n">response</span><span class="o">.</span><span class="n">status_code</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="L-137"><a href="#L-137"><span class="linenos">137</span></a>        <span class="p">)</span>
+</span><span id="L-138"><a href="#L-138"><span class="linenos">138</span></a>    <span class="n">soup</span> <span class="o">=</span> <span class="n">BeautifulSoup</span><span class="p">(</span><span class="n">response</span><span class="o">.</span><span class="n">text</span><span class="p">,</span> <span class="s2">&quot;html.parser&quot;</span><span class="p">)</span>
+</span><span id="L-139"><a href="#L-139"><span class="linenos">139</span></a>    <span class="n">pypi_packages</span> <span class="o">=</span> <span class="p">[</span>
+</span><span id="L-140"><a href="#L-140"><span class="linenos">140</span></a>        <span class="n">span</span><span class="o">.</span><span class="n">text</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span>
+</span><span id="L-141"><a href="#L-141"><span class="linenos">141</span></a>        <span class="k">for</span> <span class="n">span</span> <span class="ow">in</span> <span class="n">soup</span><span class="o">.</span><span class="n">find_all</span><span class="p">(</span><span class="s2">&quot;span&quot;</span><span class="p">,</span> <span class="n">class_</span><span class="o">=</span><span class="s2">&quot;package-snippet__name&quot;</span><span class="p">)</span>
+</span><span id="L-142"><a href="#L-142"><span class="linenos">142</span></a>    <span class="p">]</span>
+</span><span id="L-143"><a href="#L-143"><span class="linenos">143</span></a>    <span class="k">return</span> <span class="n">package_name</span> <span class="ow">in</span> <span class="n">pypi_packages</span>
+</span><span id="L-144"><a href="#L-144"><span class="linenos">144</span></a>
+</span><span id="L-145"><a href="#L-145"><span class="linenos">145</span></a>
+</span><span id="L-146"><a href="#L-146"><span class="linenos">146</span></a><span class="k">def</span> <span class="nf">check_pypi_for_name_cli</span><span class="p">():</span>
+</span><span id="L-147"><a href="#L-147"><span class="linenos">147</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">argparse</span><span class="o">.</span><span class="n">ArgumentParser</span><span class="p">()</span>
+</span><span id="L-148"><a href="#L-148"><span class="linenos">148</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span><span class="s2">&quot;name&quot;</span><span class="p">,</span> <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">)</span>
+</span><span id="L-149"><a href="#L-149"><span class="linenos">149</span></a>    <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="o">.</span><span class="n">parse_args</span><span class="p">()</span>
+</span><span id="L-150"><a href="#L-150"><span class="linenos">150</span></a>    <span class="k">if</span> <span class="n">check_pypi_for_name</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="p">):</span>
+</span><span id="L-151"><a href="#L-151"><span class="linenos">151</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2"> is already taken.&quot;</span><span class="p">)</span>
+</span><span id="L-152"><a href="#L-152"><span class="linenos">152</span></a>    <span class="k">else</span><span class="p">:</span>
+</span><span id="L-153"><a href="#L-153"><span class="linenos">153</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2"> is available.&quot;</span><span class="p">)</span>
+</span><span id="L-154"><a href="#L-154"><span class="linenos">154</span></a>
+</span><span id="L-155"><a href="#L-155"><span class="linenos">155</span></a>
+</span><span id="L-156"><a href="#L-156"><span class="linenos">156</span></a><span class="k">def</span> <span class="nf">create_pyproject_file</span><span class="p">(</span><span class="n">targetdir</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
+</span><span id="L-157"><a href="#L-157"><span class="linenos">157</span></a>    <span class="sd">&quot;&quot;&quot;Create pyproject.toml in ./{project_name} from args,</span>
+</span><span id="L-158"><a href="#L-158"><span class="linenos">158</span></a><span class="sd">    pyproject_template, and hassle_config.&quot;&quot;&quot;</span>
+</span><span id="L-159"><a href="#L-159"><span class="linenos">159</span></a>    <span class="n">pyproject</span> <span class="o">=</span> <span class="p">(</span><span class="n">root</span> <span class="o">/</span> <span class="s2">&quot;pyproject_template.toml&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">loads</span><span class="p">()</span>
+</span><span id="L-160"><a href="#L-160"><span class="linenos">160</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">hassle_config</span><span class="o">.</span><span class="n">config_exists</span><span class="p">():</span>
+</span><span id="L-161"><a href="#L-161"><span class="linenos">161</span></a>        <span class="n">hassle_config</span><span class="o">.</span><span class="n">warn</span><span class="p">()</span>
+</span><span id="L-162"><a href="#L-162"><span class="linenos">162</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">get_answer</span><span class="p">(</span><span class="s2">&quot;Continue creating new package with blank config?&quot;</span><span class="p">):</span>
+</span><span id="L-163"><a href="#L-163"><span class="linenos">163</span></a>            <span class="k">raise</span> <span class="ne">Exception</span><span class="p">(</span><span class="s2">&quot;Aborting new package creation&quot;</span><span class="p">)</span>
+</span><span id="L-164"><a href="#L-164"><span class="linenos">164</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="L-165"><a href="#L-165"><span class="linenos">165</span></a>            <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Creating blank hassle_config.toml...&quot;</span><span class="p">)</span>
+</span><span id="L-166"><a href="#L-166"><span class="linenos">166</span></a>            <span class="n">hassle_config</span><span class="o">.</span><span class="n">create_config</span><span class="p">()</span>
+</span><span id="L-167"><a href="#L-167"><span class="linenos">167</span></a>    <span class="n">config</span> <span class="o">=</span> <span class="n">hassle_config</span><span class="o">.</span><span class="n">load_config</span><span class="p">()</span>
+</span><span id="L-168"><a href="#L-168"><span class="linenos">168</span></a>    <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;name&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">name</span>
+</span><span id="L-169"><a href="#L-169"><span class="linenos">169</span></a>    <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;authors&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">config</span><span class="p">[</span><span class="s2">&quot;authors&quot;</span><span class="p">]</span>
+</span><span id="L-170"><a href="#L-170"><span class="linenos">170</span></a>    <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;description&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">description</span>
+</span><span id="L-171"><a href="#L-171"><span class="linenos">171</span></a>    <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;dependencies&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">dependencies</span>
+</span><span id="L-172"><a href="#L-172"><span class="linenos">172</span></a>    <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;keywords&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">keywords</span>
+</span><span id="L-173"><a href="#L-173"><span class="linenos">173</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">operating_system</span><span class="p">:</span>
+</span><span id="L-174"><a href="#L-174"><span class="linenos">174</span></a>        <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;classifiers&quot;</span><span class="p">][</span><span class="mi">2</span><span class="p">]</span> <span class="o">=</span> <span class="s2">&quot;Operating System :: &quot;</span> <span class="o">+</span> <span class="s2">&quot; &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span>
+</span><span id="L-175"><a href="#L-175"><span class="linenos">175</span></a>            <span class="n">args</span><span class="o">.</span><span class="n">operating_system</span>
+</span><span id="L-176"><a href="#L-176"><span class="linenos">176</span></a>        <span class="p">)</span>
+</span><span id="L-177"><a href="#L-177"><span class="linenos">177</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">no_license</span><span class="p">:</span>
+</span><span id="L-178"><a href="#L-178"><span class="linenos">178</span></a>        <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;classifiers&quot;</span><span class="p">]</span><span class="o">.</span><span class="n">pop</span><span class="p">(</span><span class="mi">1</span><span class="p">)</span>
+</span><span id="L-179"><a href="#L-179"><span class="linenos">179</span></a>    <span class="k">for</span> <span class="n">field</span> <span class="ow">in</span> <span class="n">config</span><span class="p">[</span><span class="s2">&quot;project_urls&quot;</span><span class="p">]:</span>
+</span><span id="L-180"><a href="#L-180"><span class="linenos">180</span></a>        <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;urls&quot;</span><span class="p">][</span><span class="n">field</span><span class="p">]</span> <span class="o">=</span> <span class="n">config</span><span class="p">[</span><span class="s2">&quot;project_urls&quot;</span><span class="p">][</span><span class="n">field</span><span class="p">]</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span>
+</span><span id="L-181"><a href="#L-181"><span class="linenos">181</span></a>            <span class="s2">&quot;$name&quot;</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">name</span>
+</span><span id="L-182"><a href="#L-182"><span class="linenos">182</span></a>        <span class="p">)</span>
+</span><span id="L-183"><a href="#L-183"><span class="linenos">183</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">add_script</span><span class="p">:</span>
+</span><span id="L-184"><a href="#L-184"><span class="linenos">184</span></a>        <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;scripts&quot;</span><span class="p">][</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="p">]</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2">.</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2">:main&quot;</span>
+</span><span id="L-185"><a href="#L-185"><span class="linenos">185</span></a>    <span class="p">(</span><span class="n">targetdir</span> <span class="o">/</span> <span class="s2">&quot;pyproject.toml&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">dumps</span><span class="p">(</span><span class="n">pyproject</span><span class="p">)</span>
+</span><span id="L-186"><a href="#L-186"><span class="linenos">186</span></a>
+</span><span id="L-187"><a href="#L-187"><span class="linenos">187</span></a>
+</span><span id="L-188"><a href="#L-188"><span class="linenos">188</span></a><span class="k">def</span> <span class="nf">create_source_files</span><span class="p">(</span><span class="n">srcdir</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">,</span> <span class="n">filelist</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]):</span>
+</span><span id="L-189"><a href="#L-189"><span class="linenos">189</span></a>    <span class="sd">&quot;&quot;&quot;Generate empty source files in ./{package_name}/src/{package_name}/&quot;&quot;&quot;</span>
+</span><span id="L-190"><a href="#L-190"><span class="linenos">190</span></a>    <span class="n">srcdir</span><span class="o">.</span><span class="n">mkdir</span><span class="p">(</span><span class="n">parents</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">exist_ok</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
+</span><span id="L-191"><a href="#L-191"><span class="linenos">191</span></a>    <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">filelist</span><span class="p">:</span>
+</span><span id="L-192"><a href="#L-192"><span class="linenos">192</span></a>        <span class="p">(</span><span class="n">srcdir</span> <span class="o">/</span> <span class="n">file</span><span class="p">)</span><span class="o">.</span><span class="n">touch</span><span class="p">()</span>
+</span><span id="L-193"><a href="#L-193"><span class="linenos">193</span></a>
+</span><span id="L-194"><a href="#L-194"><span class="linenos">194</span></a>
+</span><span id="L-195"><a href="#L-195"><span class="linenos">195</span></a><span class="k">def</span> <span class="nf">create_readme</span><span class="p">(</span><span class="n">targetdir</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
+</span><span id="L-196"><a href="#L-196"><span class="linenos">196</span></a>    <span class="sd">&quot;&quot;&quot;Create README.md in ./{package_name}</span>
+</span><span id="L-197"><a href="#L-197"><span class="linenos">197</span></a><span class="sd">    from readme_template and args.&quot;&quot;&quot;</span>
+</span><span id="L-198"><a href="#L-198"><span class="linenos">198</span></a>    <span class="n">readme</span> <span class="o">=</span> <span class="p">(</span><span class="n">root</span> <span class="o">/</span> <span class="s2">&quot;README_template.md&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">read_text</span><span class="p">()</span>
+</span><span id="L-199"><a href="#L-199"><span class="linenos">199</span></a>    <span class="n">readme</span> <span class="o">=</span> <span class="n">readme</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;$name&quot;</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="p">)</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span>
+</span><span id="L-200"><a href="#L-200"><span class="linenos">200</span></a>        <span class="s2">&quot;$description&quot;</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">description</span>
+</span><span id="L-201"><a href="#L-201"><span class="linenos">201</span></a>    <span class="p">)</span>
+</span><span id="L-202"><a href="#L-202"><span class="linenos">202</span></a>    <span class="p">(</span><span class="n">targetdir</span> <span class="o">/</span> <span class="s2">&quot;README.md&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="n">readme</span><span class="p">)</span>
+</span><span id="L-203"><a href="#L-203"><span class="linenos">203</span></a>
+</span><span id="L-204"><a href="#L-204"><span class="linenos">204</span></a>
+</span><span id="L-205"><a href="#L-205"><span class="linenos">205</span></a><span class="k">def</span> <span class="nf">create_license</span><span class="p">(</span><span class="n">targetdir</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">):</span>
+</span><span id="L-206"><a href="#L-206"><span class="linenos">206</span></a>    <span class="sd">&quot;&quot;&quot;Add MIT license file to ./{package_name} .&quot;&quot;&quot;</span>
+</span><span id="L-207"><a href="#L-207"><span class="linenos">207</span></a>    <span class="n">license_template</span> <span class="o">=</span> <span class="p">(</span><span class="n">root</span> <span class="o">/</span> <span class="s2">&quot;license_template.txt&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">read_text</span><span class="p">()</span>
+</span><span id="L-208"><a href="#L-208"><span class="linenos">208</span></a>    <span class="n">license_template</span> <span class="o">=</span> <span class="n">license_template</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;$year&quot;</span><span class="p">,</span> <span class="nb">str</span><span class="p">(</span><span class="n">datetime</span><span class="o">.</span><span class="n">now</span><span class="p">()</span><span class="o">.</span><span class="n">year</span><span class="p">))</span>
+</span><span id="L-209"><a href="#L-209"><span class="linenos">209</span></a>    <span class="p">(</span><span class="n">targetdir</span> <span class="o">/</span> <span class="s2">&quot;LICENSE.txt&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="n">license_template</span><span class="p">)</span>
+</span><span id="L-210"><a href="#L-210"><span class="linenos">210</span></a>
+</span><span id="L-211"><a href="#L-211"><span class="linenos">211</span></a>
+</span><span id="L-212"><a href="#L-212"><span class="linenos">212</span></a><span class="k">def</span> <span class="nf">create_gitignore</span><span class="p">(</span><span class="n">targetdir</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">):</span>
+</span><span id="L-213"><a href="#L-213"><span class="linenos">213</span></a>    <span class="sd">&quot;&quot;&quot;Add .gitignore to ./{package_name}&quot;&quot;&quot;</span>
+</span><span id="L-214"><a href="#L-214"><span class="linenos">214</span></a>    <span class="p">(</span><span class="n">root</span> <span class="o">/</span> <span class="s2">&quot;.gitignore_template&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">copy</span><span class="p">(</span><span class="n">targetdir</span> <span class="o">/</span> <span class="s2">&quot;.gitignore&quot;</span><span class="p">,</span> <span class="kc">True</span><span class="p">)</span>
+</span><span id="L-215"><a href="#L-215"><span class="linenos">215</span></a>
+</span><span id="L-216"><a href="#L-216"><span class="linenos">216</span></a>
+</span><span id="L-217"><a href="#L-217"><span class="linenos">217</span></a><span class="k">def</span> <span class="nf">create_vscode_settings</span><span class="p">(</span><span class="n">targetdir</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">):</span>
+</span><span id="L-218"><a href="#L-218"><span class="linenos">218</span></a>    <span class="sd">&quot;&quot;&quot;Add settings.json to ./.vscode&quot;&quot;&quot;</span>
+</span><span id="L-219"><a href="#L-219"><span class="linenos">219</span></a>    <span class="n">vsdir</span> <span class="o">=</span> <span class="n">targetdir</span> <span class="o">/</span> <span class="s2">&quot;.vscode&quot;</span>
+</span><span id="L-220"><a href="#L-220"><span class="linenos">220</span></a>    <span class="n">vsdir</span><span class="o">.</span><span class="n">mkdir</span><span class="p">(</span><span class="n">parents</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">exist_ok</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
+</span><span id="L-221"><a href="#L-221"><span class="linenos">221</span></a>    <span class="p">(</span><span class="n">root</span> <span class="o">/</span> <span class="s2">&quot;.vscode_template&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">copy</span><span class="p">(</span><span class="n">vsdir</span> <span class="o">/</span> <span class="s2">&quot;settings.json&quot;</span><span class="p">,</span> <span class="kc">True</span><span class="p">)</span>
+</span><span id="L-222"><a href="#L-222"><span class="linenos">222</span></a>
+</span><span id="L-223"><a href="#L-223"><span class="linenos">223</span></a>
+</span><span id="L-224"><a href="#L-224"><span class="linenos">224</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
+</span><span id="L-225"><a href="#L-225"><span class="linenos">225</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="p">:</span>
+</span><span id="L-226"><a href="#L-226"><span class="linenos">226</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
+</span><span id="L-227"><a href="#L-227"><span class="linenos">227</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">not_package</span><span class="p">:</span>
+</span><span id="L-228"><a href="#L-228"><span class="linenos">228</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="L-229"><a href="#L-229"><span class="linenos">229</span></a>            <span class="k">if</span> <span class="n">check_pypi_for_name</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="p">):</span>
+</span><span id="L-230"><a href="#L-230"><span class="linenos">230</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2"> already exists on pypi.org&quot;</span><span class="p">)</span>
+</span><span id="L-231"><a href="#L-231"><span class="linenos">231</span></a>                <span class="k">if</span> <span class="ow">not</span> <span class="n">get_answer</span><span class="p">(</span><span class="s2">&quot;Continue anyway?&quot;</span><span class="p">):</span>
+</span><span id="L-232"><a href="#L-232"><span class="linenos">232</span></a>                    <span class="n">sys</span><span class="o">.</span><span class="n">exit</span><span class="p">(</span><span class="mi">0</span><span class="p">)</span>
+</span><span id="L-233"><a href="#L-233"><span class="linenos">233</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="L-234"><a href="#L-234"><span class="linenos">234</span></a>            <span class="nb">print</span><span class="p">(</span><span class="n">e</span><span class="p">)</span>
+</span><span id="L-235"><a href="#L-235"><span class="linenos">235</span></a>            <span class="nb">print</span><span class="p">(</span>
+</span><span id="L-236"><a href="#L-236"><span class="linenos">236</span></a>                <span class="sa">f</span><span class="s2">&quot;Couldn&#39;t verify that </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2"> doesn&#39;t already exist on pypi.org .&quot;</span>
+</span><span id="L-237"><a href="#L-237"><span class="linenos">237</span></a>            <span class="p">)</span>
+</span><span id="L-238"><a href="#L-238"><span class="linenos">238</span></a>            <span class="k">if</span> <span class="ow">not</span> <span class="n">get_answer</span><span class="p">(</span><span class="s2">&quot;Continue anyway?&quot;</span><span class="p">):</span>
+</span><span id="L-239"><a href="#L-239"><span class="linenos">239</span></a>                <span class="n">sys</span><span class="o">.</span><span class="n">exit</span><span class="p">(</span><span class="mi">0</span><span class="p">)</span>
+</span><span id="L-240"><a href="#L-240"><span class="linenos">240</span></a>    <span class="k">try</span><span class="p">:</span>
+</span><span id="L-241"><a href="#L-241"><span class="linenos">241</span></a>        <span class="n">targetdir</span><span class="p">:</span> <span class="n">Pathier</span> <span class="o">=</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span> <span class="o">/</span> <span class="n">args</span><span class="o">.</span><span class="n">name</span>
+</span><span id="L-242"><a href="#L-242"><span class="linenos">242</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="L-243"><a href="#L-243"><span class="linenos">243</span></a>            <span class="n">targetdir</span><span class="o">.</span><span class="n">mkdir</span><span class="p">(</span><span class="n">parents</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">exist_ok</span><span class="o">=</span><span class="kc">False</span><span class="p">)</span>
+</span><span id="L-244"><a href="#L-244"><span class="linenos">244</span></a>        <span class="k">except</span><span class="p">:</span>
+</span><span id="L-245"><a href="#L-245"><span class="linenos">245</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">targetdir</span><span class="si">}</span><span class="s2"> already exists.&quot;</span><span class="p">)</span>
+</span><span id="L-246"><a href="#L-246"><span class="linenos">246</span></a>            <span class="k">if</span> <span class="ow">not</span> <span class="n">get_answer</span><span class="p">(</span><span class="s2">&quot;Overwrite?&quot;</span><span class="p">):</span>
+</span><span id="L-247"><a href="#L-247"><span class="linenos">247</span></a>                <span class="n">sys</span><span class="o">.</span><span class="n">exit</span><span class="p">(</span><span class="mi">0</span><span class="p">)</span>
+</span><span id="L-248"><a href="#L-248"><span class="linenos">248</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">not_package</span><span class="p">:</span>
+</span><span id="L-249"><a href="#L-249"><span class="linenos">249</span></a>            <span class="n">create_pyproject_file</span><span class="p">(</span><span class="n">targetdir</span><span class="p">,</span> <span class="n">args</span><span class="p">)</span>
+</span><span id="L-250"><a href="#L-250"><span class="linenos">250</span></a>        <span class="n">create_source_files</span><span class="p">(</span>
+</span><span id="L-251"><a href="#L-251"><span class="linenos">251</span></a>            <span class="n">targetdir</span> <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">not_package</span> <span class="k">else</span> <span class="p">(</span><span class="n">targetdir</span> <span class="o">/</span> <span class="s2">&quot;src&quot;</span> <span class="o">/</span> <span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="p">),</span>
+</span><span id="L-252"><a href="#L-252"><span class="linenos">252</span></a>            <span class="n">args</span><span class="o">.</span><span class="n">source_files</span><span class="p">[</span><span class="mi">1</span><span class="p">:]</span> <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">not_package</span> <span class="k">else</span> <span class="n">args</span><span class="o">.</span><span class="n">source_files</span><span class="p">,</span>
+</span><span id="L-253"><a href="#L-253"><span class="linenos">253</span></a>        <span class="p">)</span>
+</span><span id="L-254"><a href="#L-254"><span class="linenos">254</span></a>        <span class="n">create_readme</span><span class="p">(</span><span class="n">targetdir</span><span class="p">,</span> <span class="n">args</span><span class="p">)</span>
+</span><span id="L-255"><a href="#L-255"><span class="linenos">255</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">not_package</span><span class="p">:</span>
+</span><span id="L-256"><a href="#L-256"><span class="linenos">256</span></a>            <span class="n">generate_test_files</span><span class="p">(</span><span class="n">targetdir</span><span class="p">)</span>
+</span><span id="L-257"><a href="#L-257"><span class="linenos">257</span></a>            <span class="n">create_vscode_settings</span><span class="p">(</span><span class="n">targetdir</span><span class="p">)</span>
+</span><span id="L-258"><a href="#L-258"><span class="linenos">258</span></a>        <span class="n">create_gitignore</span><span class="p">(</span><span class="n">targetdir</span><span class="p">)</span>
+</span><span id="L-259"><a href="#L-259"><span class="linenos">259</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">no_license</span><span class="p">:</span>
+</span><span id="L-260"><a href="#L-260"><span class="linenos">260</span></a>            <span class="n">create_license</span><span class="p">(</span><span class="n">targetdir</span><span class="p">)</span>
+</span><span id="L-261"><a href="#L-261"><span class="linenos">261</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">targetdir</span><span class="p">)</span>
+</span><span id="L-262"><a href="#L-262"><span class="linenos">262</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="s2">&quot;git init -b main&quot;</span><span class="p">)</span>
+</span><span id="L-263"><a href="#L-263"><span class="linenos">263</span></a>
+</span><span id="L-264"><a href="#L-264"><span class="linenos">264</span></a>    <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="L-265"><a href="#L-265"><span class="linenos">265</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="s2">&quot;Aborting new package creation&quot;</span> <span class="ow">in</span> <span class="nb">str</span><span class="p">(</span><span class="n">e</span><span class="p">):</span>
+</span><span id="L-266"><a href="#L-266"><span class="linenos">266</span></a>            <span class="nb">print</span><span class="p">(</span><span class="n">e</span><span class="p">)</span>
+</span><span id="L-267"><a href="#L-267"><span class="linenos">267</span></a>        <span class="k">if</span> <span class="n">get_answer</span><span class="p">(</span><span class="s2">&quot;Delete created files?&quot;</span><span class="p">):</span>
+</span><span id="L-268"><a href="#L-268"><span class="linenos">268</span></a>            <span class="n">targetdir</span><span class="o">.</span><span class="n">delete</span><span class="p">()</span>
+</span><span id="L-269"><a href="#L-269"><span class="linenos">269</span></a>
+</span><span id="L-270"><a href="#L-270"><span class="linenos">270</span></a>
+</span><span id="L-271"><a href="#L-271"><span class="linenos">271</span></a><span class="k">if</span> <span class="vm">__name__</span> <span class="o">==</span> <span class="s2">&quot;__main__&quot;</span><span class="p">:</span>
+</span><span id="L-272"><a href="#L-272"><span class="linenos">272</span></a>    <span class="n">main</span><span class="p">(</span><span class="n">get_args</span><span class="p">())</span>
 </span></pre></div>
 
 
             </section>
                 <section id="get_args">
                             <input id="get_args-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
@@ -369,105 +367,105 @@
         <span class="def">def</span>
         <span class="name">get_args</span><span class="signature pdoc-code condensed">(<span class="return-annotation">) -> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span>:</span></span>
 
                 <label class="view-source-button" for="get_args-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#get_args"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="get_args-19"><a href="#get_args-19"><span class="linenos"> 19</span></a><span class="k">def</span> <span class="nf">get_args</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">:</span>
-</span><span id="get_args-20"><a href="#get_args-20"><span class="linenos"> 20</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">argparse</span><span class="o">.</span><span class="n">ArgumentParser</span><span class="p">()</span>
-</span><span id="get_args-21"><a href="#get_args-21"><span class="linenos"> 21</span></a>
-</span><span id="get_args-22"><a href="#get_args-22"><span class="linenos"> 22</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="get_args-23"><a href="#get_args-23"><span class="linenos"> 23</span></a>        <span class="s2">&quot;name&quot;</span><span class="p">,</span>
-</span><span id="get_args-24"><a href="#get_args-24"><span class="linenos"> 24</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
-</span><span id="get_args-25"><a href="#get_args-25"><span class="linenos"> 25</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Name of the package to create in the current working directory. &quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="get_args-26"><a href="#get_args-26"><span class="linenos"> 26</span></a>    <span class="p">)</span>
-</span><span id="get_args-27"><a href="#get_args-27"><span class="linenos"> 27</span></a>
-</span><span id="get_args-28"><a href="#get_args-28"><span class="linenos"> 28</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="get_args-29"><a href="#get_args-29"><span class="linenos"> 29</span></a>        <span class="s2">&quot;-s&quot;</span><span class="p">,</span>
-</span><span id="get_args-30"><a href="#get_args-30"><span class="linenos"> 30</span></a>        <span class="s2">&quot;--source_files&quot;</span><span class="p">,</span>
-</span><span id="get_args-31"><a href="#get_args-31"><span class="linenos"> 31</span></a>        <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;*&quot;</span><span class="p">,</span>
-</span><span id="get_args-32"><a href="#get_args-32"><span class="linenos"> 32</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
-</span><span id="get_args-33"><a href="#get_args-33"><span class="linenos"> 33</span></a>        <span class="n">default</span><span class="o">=</span><span class="p">[],</span>
-</span><span id="get_args-34"><a href="#get_args-34"><span class="linenos"> 34</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; List of additional source files to create in addition to the default</span>
-</span><span id="get_args-35"><a href="#get_args-35"><span class="linenos"> 35</span></a><span class="s2">        __init__.py and </span><span class="si">{name}</span><span class="s2">.py files.&quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="get_args-36"><a href="#get_args-36"><span class="linenos"> 36</span></a>    <span class="p">)</span>
-</span><span id="get_args-37"><a href="#get_args-37"><span class="linenos"> 37</span></a>
-</span><span id="get_args-38"><a href="#get_args-38"><span class="linenos"> 38</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="get_args-39"><a href="#get_args-39"><span class="linenos"> 39</span></a>        <span class="s2">&quot;-d&quot;</span><span class="p">,</span>
-</span><span id="get_args-40"><a href="#get_args-40"><span class="linenos"> 40</span></a>        <span class="s2">&quot;--description&quot;</span><span class="p">,</span>
-</span><span id="get_args-41"><a href="#get_args-41"><span class="linenos"> 41</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
-</span><span id="get_args-42"><a href="#get_args-42"><span class="linenos"> 42</span></a>        <span class="n">default</span><span class="o">=</span><span class="s2">&quot;&quot;</span><span class="p">,</span>
-</span><span id="get_args-43"><a href="#get_args-43"><span class="linenos"> 43</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; The package description to be added to the pyproject.toml file. &quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="get_args-44"><a href="#get_args-44"><span class="linenos"> 44</span></a>    <span class="p">)</span>
-</span><span id="get_args-45"><a href="#get_args-45"><span class="linenos"> 45</span></a>
-</span><span id="get_args-46"><a href="#get_args-46"><span class="linenos"> 46</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="get_args-47"><a href="#get_args-47"><span class="linenos"> 47</span></a>        <span class="s2">&quot;-dp&quot;</span><span class="p">,</span>
-</span><span id="get_args-48"><a href="#get_args-48"><span class="linenos"> 48</span></a>        <span class="s2">&quot;--dependencies&quot;</span><span class="p">,</span>
-</span><span id="get_args-49"><a href="#get_args-49"><span class="linenos"> 49</span></a>        <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;*&quot;</span><span class="p">,</span>
-</span><span id="get_args-50"><a href="#get_args-50"><span class="linenos"> 50</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
-</span><span id="get_args-51"><a href="#get_args-51"><span class="linenos"> 51</span></a>        <span class="n">default</span><span class="o">=</span><span class="p">[],</span>
-</span><span id="get_args-52"><a href="#get_args-52"><span class="linenos"> 52</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; List of dependencies to add to pyproject.toml.</span>
-</span><span id="get_args-53"><a href="#get_args-53"><span class="linenos"> 53</span></a><span class="s2">        Note: hassle.py will automatically scan your project for 3rd party</span>
-</span><span id="get_args-54"><a href="#get_args-54"><span class="linenos"> 54</span></a><span class="s2">        imports and update pyproject.toml. This switch is largely useful</span>
-</span><span id="get_args-55"><a href="#get_args-55"><span class="linenos"> 55</span></a><span class="s2">        for adding dependencies your project might need, but doesn&#39;t</span>
-</span><span id="get_args-56"><a href="#get_args-56"><span class="linenos"> 56</span></a><span class="s2">        directly import in any source files,</span>
-</span><span id="get_args-57"><a href="#get_args-57"><span class="linenos"> 57</span></a><span class="s2">        like an os.system() call that invokes a 3rd party cli.&quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="get_args-58"><a href="#get_args-58"><span class="linenos"> 58</span></a>    <span class="p">)</span>
-</span><span id="get_args-59"><a href="#get_args-59"><span class="linenos"> 59</span></a>
-</span><span id="get_args-60"><a href="#get_args-60"><span class="linenos"> 60</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="get_args-61"><a href="#get_args-61"><span class="linenos"> 61</span></a>        <span class="s2">&quot;-k&quot;</span><span class="p">,</span>
-</span><span id="get_args-62"><a href="#get_args-62"><span class="linenos"> 62</span></a>        <span class="s2">&quot;--keywords&quot;</span><span class="p">,</span>
-</span><span id="get_args-63"><a href="#get_args-63"><span class="linenos"> 63</span></a>        <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;*&quot;</span><span class="p">,</span>
-</span><span id="get_args-64"><a href="#get_args-64"><span class="linenos"> 64</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
-</span><span id="get_args-65"><a href="#get_args-65"><span class="linenos"> 65</span></a>        <span class="n">default</span><span class="o">=</span><span class="p">[],</span>
-</span><span id="get_args-66"><a href="#get_args-66"><span class="linenos"> 66</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; List of keywords to be added to the keywords field in pyproject.toml. &quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="get_args-67"><a href="#get_args-67"><span class="linenos"> 67</span></a>    <span class="p">)</span>
-</span><span id="get_args-68"><a href="#get_args-68"><span class="linenos"> 68</span></a>
-</span><span id="get_args-69"><a href="#get_args-69"><span class="linenos"> 69</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="get_args-70"><a href="#get_args-70"><span class="linenos"> 70</span></a>        <span class="s2">&quot;-as&quot;</span><span class="p">,</span>
-</span><span id="get_args-71"><a href="#get_args-71"><span class="linenos"> 71</span></a>        <span class="s2">&quot;--add_script&quot;</span><span class="p">,</span>
-</span><span id="get_args-72"><a href="#get_args-72"><span class="linenos"> 72</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
-</span><span id="get_args-73"><a href="#get_args-73"><span class="linenos"> 73</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Add section to pyproject.toml declaring the package </span>
-</span><span id="get_args-74"><a href="#get_args-74"><span class="linenos"> 74</span></a><span class="s2">        should be installed with command line scripts added. </span>
-</span><span id="get_args-75"><a href="#get_args-75"><span class="linenos"> 75</span></a><span class="s2">        The default is &#39;</span><span class="si">{name}</span><span class="s2"> = &quot;</span><span class="si">{name}</span><span class="s2">.</span><span class="si">{name}</span><span class="s2">:main&quot;.</span>
-</span><span id="get_args-76"><a href="#get_args-76"><span class="linenos"> 76</span></a><span class="s2">        You will need to manually change this field.&quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="get_args-77"><a href="#get_args-77"><span class="linenos"> 77</span></a>    <span class="p">)</span>
-</span><span id="get_args-78"><a href="#get_args-78"><span class="linenos"> 78</span></a>
-</span><span id="get_args-79"><a href="#get_args-79"><span class="linenos"> 79</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="get_args-80"><a href="#get_args-80"><span class="linenos"> 80</span></a>        <span class="s2">&quot;-nl&quot;</span><span class="p">,</span>
-</span><span id="get_args-81"><a href="#get_args-81"><span class="linenos"> 81</span></a>        <span class="s2">&quot;--no_license&quot;</span><span class="p">,</span>
-</span><span id="get_args-82"><a href="#get_args-82"><span class="linenos"> 82</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
-</span><span id="get_args-83"><a href="#get_args-83"><span class="linenos"> 83</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; By default, projects are created with an MIT license.</span>
-</span><span id="get_args-84"><a href="#get_args-84"><span class="linenos"> 84</span></a><span class="s2">        Set this flag to avoid adding a license if you want to configure licensing</span>
-</span><span id="get_args-85"><a href="#get_args-85"><span class="linenos"> 85</span></a><span class="s2">        at another time.&quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="get_args-86"><a href="#get_args-86"><span class="linenos"> 86</span></a>    <span class="p">)</span>
-</span><span id="get_args-87"><a href="#get_args-87"><span class="linenos"> 87</span></a>
-</span><span id="get_args-88"><a href="#get_args-88"><span class="linenos"> 88</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="get_args-89"><a href="#get_args-89"><span class="linenos"> 89</span></a>        <span class="s2">&quot;-os&quot;</span><span class="p">,</span>
-</span><span id="get_args-90"><a href="#get_args-90"><span class="linenos"> 90</span></a>        <span class="s2">&quot;--operating_system&quot;</span><span class="p">,</span>
-</span><span id="get_args-91"><a href="#get_args-91"><span class="linenos"> 91</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
-</span><span id="get_args-92"><a href="#get_args-92"><span class="linenos"> 92</span></a>        <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
-</span><span id="get_args-93"><a href="#get_args-93"><span class="linenos"> 93</span></a>        <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;*&quot;</span><span class="p">,</span>
-</span><span id="get_args-94"><a href="#get_args-94"><span class="linenos"> 94</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; List of operating systems this package will be compatible with.</span>
-</span><span id="get_args-95"><a href="#get_args-95"><span class="linenos"> 95</span></a><span class="s2">        The default is OS Independent.</span>
-</span><span id="get_args-96"><a href="#get_args-96"><span class="linenos"> 96</span></a><span class="s2">        This only affects the &#39;classifiers&#39; field of pyproject.toml .&quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="get_args-97"><a href="#get_args-97"><span class="linenos"> 97</span></a>    <span class="p">)</span>
-</span><span id="get_args-98"><a href="#get_args-98"><span class="linenos"> 98</span></a>
-</span><span id="get_args-99"><a href="#get_args-99"><span class="linenos"> 99</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="get_args-100"><a href="#get_args-100"><span class="linenos">100</span></a>        <span class="s2">&quot;-np&quot;</span><span class="p">,</span>
-</span><span id="get_args-101"><a href="#get_args-101"><span class="linenos">101</span></a>        <span class="s2">&quot;--not_package&quot;</span><span class="p">,</span>
-</span><span id="get_args-102"><a href="#get_args-102"><span class="linenos">102</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
-</span><span id="get_args-103"><a href="#get_args-103"><span class="linenos">103</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Put source files in top level directory and delete tests folder. &quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="get_args-104"><a href="#get_args-104"><span class="linenos">104</span></a>    <span class="p">)</span>
-</span><span id="get_args-105"><a href="#get_args-105"><span class="linenos">105</span></a>
-</span><span id="get_args-106"><a href="#get_args-106"><span class="linenos">106</span></a>    <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="o">.</span><span class="n">parse_args</span><span class="p">()</span>
-</span><span id="get_args-107"><a href="#get_args-107"><span class="linenos">107</span></a>    <span class="n">args</span><span class="o">.</span><span class="n">source_files</span><span class="o">.</span><span class="n">extend</span><span class="p">([</span><span class="s2">&quot;__init__.py&quot;</span><span class="p">,</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2">.py&quot;</span><span class="p">])</span>
-</span><span id="get_args-108"><a href="#get_args-108"><span class="linenos">108</span></a>
-</span><span id="get_args-109"><a href="#get_args-109"><span class="linenos">109</span></a>    <span class="k">return</span> <span class="n">args</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="get_args-17"><a href="#get_args-17"><span class="linenos"> 17</span></a><span class="k">def</span> <span class="nf">get_args</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">:</span>
+</span><span id="get_args-18"><a href="#get_args-18"><span class="linenos"> 18</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">argparse</span><span class="o">.</span><span class="n">ArgumentParser</span><span class="p">()</span>
+</span><span id="get_args-19"><a href="#get_args-19"><span class="linenos"> 19</span></a>
+</span><span id="get_args-20"><a href="#get_args-20"><span class="linenos"> 20</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="get_args-21"><a href="#get_args-21"><span class="linenos"> 21</span></a>        <span class="s2">&quot;name&quot;</span><span class="p">,</span>
+</span><span id="get_args-22"><a href="#get_args-22"><span class="linenos"> 22</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
+</span><span id="get_args-23"><a href="#get_args-23"><span class="linenos"> 23</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Name of the package to create in the current working directory. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="get_args-24"><a href="#get_args-24"><span class="linenos"> 24</span></a>    <span class="p">)</span>
+</span><span id="get_args-25"><a href="#get_args-25"><span class="linenos"> 25</span></a>
+</span><span id="get_args-26"><a href="#get_args-26"><span class="linenos"> 26</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="get_args-27"><a href="#get_args-27"><span class="linenos"> 27</span></a>        <span class="s2">&quot;-s&quot;</span><span class="p">,</span>
+</span><span id="get_args-28"><a href="#get_args-28"><span class="linenos"> 28</span></a>        <span class="s2">&quot;--source_files&quot;</span><span class="p">,</span>
+</span><span id="get_args-29"><a href="#get_args-29"><span class="linenos"> 29</span></a>        <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;*&quot;</span><span class="p">,</span>
+</span><span id="get_args-30"><a href="#get_args-30"><span class="linenos"> 30</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
+</span><span id="get_args-31"><a href="#get_args-31"><span class="linenos"> 31</span></a>        <span class="n">default</span><span class="o">=</span><span class="p">[],</span>
+</span><span id="get_args-32"><a href="#get_args-32"><span class="linenos"> 32</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; List of additional source files to create in addition to the default</span>
+</span><span id="get_args-33"><a href="#get_args-33"><span class="linenos"> 33</span></a><span class="s2">        __init__.py and </span><span class="si">{name}</span><span class="s2">.py files.&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="get_args-34"><a href="#get_args-34"><span class="linenos"> 34</span></a>    <span class="p">)</span>
+</span><span id="get_args-35"><a href="#get_args-35"><span class="linenos"> 35</span></a>
+</span><span id="get_args-36"><a href="#get_args-36"><span class="linenos"> 36</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="get_args-37"><a href="#get_args-37"><span class="linenos"> 37</span></a>        <span class="s2">&quot;-d&quot;</span><span class="p">,</span>
+</span><span id="get_args-38"><a href="#get_args-38"><span class="linenos"> 38</span></a>        <span class="s2">&quot;--description&quot;</span><span class="p">,</span>
+</span><span id="get_args-39"><a href="#get_args-39"><span class="linenos"> 39</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
+</span><span id="get_args-40"><a href="#get_args-40"><span class="linenos"> 40</span></a>        <span class="n">default</span><span class="o">=</span><span class="s2">&quot;&quot;</span><span class="p">,</span>
+</span><span id="get_args-41"><a href="#get_args-41"><span class="linenos"> 41</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; The package description to be added to the pyproject.toml file. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="get_args-42"><a href="#get_args-42"><span class="linenos"> 42</span></a>    <span class="p">)</span>
+</span><span id="get_args-43"><a href="#get_args-43"><span class="linenos"> 43</span></a>
+</span><span id="get_args-44"><a href="#get_args-44"><span class="linenos"> 44</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="get_args-45"><a href="#get_args-45"><span class="linenos"> 45</span></a>        <span class="s2">&quot;-dp&quot;</span><span class="p">,</span>
+</span><span id="get_args-46"><a href="#get_args-46"><span class="linenos"> 46</span></a>        <span class="s2">&quot;--dependencies&quot;</span><span class="p">,</span>
+</span><span id="get_args-47"><a href="#get_args-47"><span class="linenos"> 47</span></a>        <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;*&quot;</span><span class="p">,</span>
+</span><span id="get_args-48"><a href="#get_args-48"><span class="linenos"> 48</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
+</span><span id="get_args-49"><a href="#get_args-49"><span class="linenos"> 49</span></a>        <span class="n">default</span><span class="o">=</span><span class="p">[],</span>
+</span><span id="get_args-50"><a href="#get_args-50"><span class="linenos"> 50</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; List of dependencies to add to pyproject.toml.</span>
+</span><span id="get_args-51"><a href="#get_args-51"><span class="linenos"> 51</span></a><span class="s2">        Note: hassle.py will automatically scan your project for 3rd party</span>
+</span><span id="get_args-52"><a href="#get_args-52"><span class="linenos"> 52</span></a><span class="s2">        imports and update pyproject.toml. This switch is largely useful</span>
+</span><span id="get_args-53"><a href="#get_args-53"><span class="linenos"> 53</span></a><span class="s2">        for adding dependencies your project might need, but doesn&#39;t</span>
+</span><span id="get_args-54"><a href="#get_args-54"><span class="linenos"> 54</span></a><span class="s2">        directly import in any source files,</span>
+</span><span id="get_args-55"><a href="#get_args-55"><span class="linenos"> 55</span></a><span class="s2">        like an os.system() call that invokes a 3rd party cli.&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="get_args-56"><a href="#get_args-56"><span class="linenos"> 56</span></a>    <span class="p">)</span>
+</span><span id="get_args-57"><a href="#get_args-57"><span class="linenos"> 57</span></a>
+</span><span id="get_args-58"><a href="#get_args-58"><span class="linenos"> 58</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="get_args-59"><a href="#get_args-59"><span class="linenos"> 59</span></a>        <span class="s2">&quot;-k&quot;</span><span class="p">,</span>
+</span><span id="get_args-60"><a href="#get_args-60"><span class="linenos"> 60</span></a>        <span class="s2">&quot;--keywords&quot;</span><span class="p">,</span>
+</span><span id="get_args-61"><a href="#get_args-61"><span class="linenos"> 61</span></a>        <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;*&quot;</span><span class="p">,</span>
+</span><span id="get_args-62"><a href="#get_args-62"><span class="linenos"> 62</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
+</span><span id="get_args-63"><a href="#get_args-63"><span class="linenos"> 63</span></a>        <span class="n">default</span><span class="o">=</span><span class="p">[],</span>
+</span><span id="get_args-64"><a href="#get_args-64"><span class="linenos"> 64</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; List of keywords to be added to the keywords field in pyproject.toml. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="get_args-65"><a href="#get_args-65"><span class="linenos"> 65</span></a>    <span class="p">)</span>
+</span><span id="get_args-66"><a href="#get_args-66"><span class="linenos"> 66</span></a>
+</span><span id="get_args-67"><a href="#get_args-67"><span class="linenos"> 67</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="get_args-68"><a href="#get_args-68"><span class="linenos"> 68</span></a>        <span class="s2">&quot;-as&quot;</span><span class="p">,</span>
+</span><span id="get_args-69"><a href="#get_args-69"><span class="linenos"> 69</span></a>        <span class="s2">&quot;--add_script&quot;</span><span class="p">,</span>
+</span><span id="get_args-70"><a href="#get_args-70"><span class="linenos"> 70</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="get_args-71"><a href="#get_args-71"><span class="linenos"> 71</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Add section to pyproject.toml declaring the package </span>
+</span><span id="get_args-72"><a href="#get_args-72"><span class="linenos"> 72</span></a><span class="s2">        should be installed with command line scripts added. </span>
+</span><span id="get_args-73"><a href="#get_args-73"><span class="linenos"> 73</span></a><span class="s2">        The default is &#39;</span><span class="si">{name}</span><span class="s2"> = &quot;</span><span class="si">{name}</span><span class="s2">.</span><span class="si">{name}</span><span class="s2">:main&quot;.</span>
+</span><span id="get_args-74"><a href="#get_args-74"><span class="linenos"> 74</span></a><span class="s2">        You will need to manually change this field.&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="get_args-75"><a href="#get_args-75"><span class="linenos"> 75</span></a>    <span class="p">)</span>
+</span><span id="get_args-76"><a href="#get_args-76"><span class="linenos"> 76</span></a>
+</span><span id="get_args-77"><a href="#get_args-77"><span class="linenos"> 77</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="get_args-78"><a href="#get_args-78"><span class="linenos"> 78</span></a>        <span class="s2">&quot;-nl&quot;</span><span class="p">,</span>
+</span><span id="get_args-79"><a href="#get_args-79"><span class="linenos"> 79</span></a>        <span class="s2">&quot;--no_license&quot;</span><span class="p">,</span>
+</span><span id="get_args-80"><a href="#get_args-80"><span class="linenos"> 80</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="get_args-81"><a href="#get_args-81"><span class="linenos"> 81</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; By default, projects are created with an MIT license.</span>
+</span><span id="get_args-82"><a href="#get_args-82"><span class="linenos"> 82</span></a><span class="s2">        Set this flag to avoid adding a license if you want to configure licensing</span>
+</span><span id="get_args-83"><a href="#get_args-83"><span class="linenos"> 83</span></a><span class="s2">        at another time.&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="get_args-84"><a href="#get_args-84"><span class="linenos"> 84</span></a>    <span class="p">)</span>
+</span><span id="get_args-85"><a href="#get_args-85"><span class="linenos"> 85</span></a>
+</span><span id="get_args-86"><a href="#get_args-86"><span class="linenos"> 86</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="get_args-87"><a href="#get_args-87"><span class="linenos"> 87</span></a>        <span class="s2">&quot;-os&quot;</span><span class="p">,</span>
+</span><span id="get_args-88"><a href="#get_args-88"><span class="linenos"> 88</span></a>        <span class="s2">&quot;--operating_system&quot;</span><span class="p">,</span>
+</span><span id="get_args-89"><a href="#get_args-89"><span class="linenos"> 89</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
+</span><span id="get_args-90"><a href="#get_args-90"><span class="linenos"> 90</span></a>        <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
+</span><span id="get_args-91"><a href="#get_args-91"><span class="linenos"> 91</span></a>        <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;*&quot;</span><span class="p">,</span>
+</span><span id="get_args-92"><a href="#get_args-92"><span class="linenos"> 92</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; List of operating systems this package will be compatible with.</span>
+</span><span id="get_args-93"><a href="#get_args-93"><span class="linenos"> 93</span></a><span class="s2">        The default is OS Independent.</span>
+</span><span id="get_args-94"><a href="#get_args-94"><span class="linenos"> 94</span></a><span class="s2">        This only affects the &#39;classifiers&#39; field of pyproject.toml .&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="get_args-95"><a href="#get_args-95"><span class="linenos"> 95</span></a>    <span class="p">)</span>
+</span><span id="get_args-96"><a href="#get_args-96"><span class="linenos"> 96</span></a>
+</span><span id="get_args-97"><a href="#get_args-97"><span class="linenos"> 97</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="get_args-98"><a href="#get_args-98"><span class="linenos"> 98</span></a>        <span class="s2">&quot;-np&quot;</span><span class="p">,</span>
+</span><span id="get_args-99"><a href="#get_args-99"><span class="linenos"> 99</span></a>        <span class="s2">&quot;--not_package&quot;</span><span class="p">,</span>
+</span><span id="get_args-100"><a href="#get_args-100"><span class="linenos">100</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="get_args-101"><a href="#get_args-101"><span class="linenos">101</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Put source files in top level directory and delete tests folder. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="get_args-102"><a href="#get_args-102"><span class="linenos">102</span></a>    <span class="p">)</span>
+</span><span id="get_args-103"><a href="#get_args-103"><span class="linenos">103</span></a>
+</span><span id="get_args-104"><a href="#get_args-104"><span class="linenos">104</span></a>    <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="o">.</span><span class="n">parse_args</span><span class="p">()</span>
+</span><span id="get_args-105"><a href="#get_args-105"><span class="linenos">105</span></a>    <span class="n">args</span><span class="o">.</span><span class="n">source_files</span><span class="o">.</span><span class="n">extend</span><span class="p">([</span><span class="s2">&quot;__init__.py&quot;</span><span class="p">,</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2">.py&quot;</span><span class="p">])</span>
+</span><span id="get_args-106"><a href="#get_args-106"><span class="linenos">106</span></a>
+</span><span id="get_args-107"><a href="#get_args-107"><span class="linenos">107</span></a>    <span class="k">return</span> <span class="n">args</span>
 </span></pre></div>
 
 
     
 
                 </section>
                 <section id="get_answer">
@@ -477,30 +475,30 @@
         <span class="def">def</span>
         <span class="name">get_answer</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">question</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">) -> <span class="nb">bool</span>:</span></span>
 
                 <label class="view-source-button" for="get_answer-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#get_answer"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="get_answer-112"><a href="#get_answer-112"><span class="linenos">112</span></a><span class="k">def</span> <span class="nf">get_answer</span><span class="p">(</span><span class="n">question</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
-</span><span id="get_answer-113"><a href="#get_answer-113"><span class="linenos">113</span></a>    <span class="sd">&quot;&quot;&quot;Repeatedly ask the user a yes/no question</span>
-</span><span id="get_answer-114"><a href="#get_answer-114"><span class="linenos">114</span></a><span class="sd">    until a &#39;y&#39; or a &#39;n&#39; is received.&quot;&quot;&quot;</span>
-</span><span id="get_answer-115"><a href="#get_answer-115"><span class="linenos">115</span></a>    <span class="n">ans</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
-</span><span id="get_answer-116"><a href="#get_answer-116"><span class="linenos">116</span></a>    <span class="n">question</span> <span class="o">=</span> <span class="n">question</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span>
-</span><span id="get_answer-117"><a href="#get_answer-117"><span class="linenos">117</span></a>    <span class="k">if</span> <span class="s2">&quot;?&quot;</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">question</span><span class="p">:</span>
-</span><span id="get_answer-118"><a href="#get_answer-118"><span class="linenos">118</span></a>        <span class="n">question</span> <span class="o">+=</span> <span class="s2">&quot;?&quot;</span>
-</span><span id="get_answer-119"><a href="#get_answer-119"><span class="linenos">119</span></a>    <span class="n">question</span> <span class="o">+=</span> <span class="s2">&quot; (y/n): &quot;</span>
-</span><span id="get_answer-120"><a href="#get_answer-120"><span class="linenos">120</span></a>    <span class="k">while</span> <span class="n">ans</span> <span class="ow">not</span> <span class="ow">in</span> <span class="p">[</span><span class="s2">&quot;y&quot;</span><span class="p">,</span> <span class="s2">&quot;yes&quot;</span><span class="p">,</span> <span class="s2">&quot;no&quot;</span><span class="p">,</span> <span class="s2">&quot;n&quot;</span><span class="p">]:</span>
-</span><span id="get_answer-121"><a href="#get_answer-121"><span class="linenos">121</span></a>        <span class="n">ans</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span><span class="n">question</span><span class="p">)</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span>
-</span><span id="get_answer-122"><a href="#get_answer-122"><span class="linenos">122</span></a>        <span class="k">if</span> <span class="n">ans</span> <span class="ow">in</span> <span class="p">[</span><span class="s2">&quot;y&quot;</span><span class="p">,</span> <span class="s2">&quot;yes&quot;</span><span class="p">]:</span>
-</span><span id="get_answer-123"><a href="#get_answer-123"><span class="linenos">123</span></a>            <span class="k">return</span> <span class="kc">True</span>
-</span><span id="get_answer-124"><a href="#get_answer-124"><span class="linenos">124</span></a>        <span class="k">elif</span> <span class="n">ans</span> <span class="ow">in</span> <span class="p">[</span><span class="s2">&quot;n&quot;</span><span class="p">,</span> <span class="s2">&quot;no&quot;</span><span class="p">]:</span>
-</span><span id="get_answer-125"><a href="#get_answer-125"><span class="linenos">125</span></a>            <span class="k">return</span> <span class="kc">False</span>
-</span><span id="get_answer-126"><a href="#get_answer-126"><span class="linenos">126</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="get_answer-127"><a href="#get_answer-127"><span class="linenos">127</span></a>            <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Invalid answer.&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="get_answer-110"><a href="#get_answer-110"><span class="linenos">110</span></a><span class="k">def</span> <span class="nf">get_answer</span><span class="p">(</span><span class="n">question</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
+</span><span id="get_answer-111"><a href="#get_answer-111"><span class="linenos">111</span></a>    <span class="sd">&quot;&quot;&quot;Repeatedly ask the user a yes/no question</span>
+</span><span id="get_answer-112"><a href="#get_answer-112"><span class="linenos">112</span></a><span class="sd">    until a &#39;y&#39; or a &#39;n&#39; is received.&quot;&quot;&quot;</span>
+</span><span id="get_answer-113"><a href="#get_answer-113"><span class="linenos">113</span></a>    <span class="n">ans</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
+</span><span id="get_answer-114"><a href="#get_answer-114"><span class="linenos">114</span></a>    <span class="n">question</span> <span class="o">=</span> <span class="n">question</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span>
+</span><span id="get_answer-115"><a href="#get_answer-115"><span class="linenos">115</span></a>    <span class="k">if</span> <span class="s2">&quot;?&quot;</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">question</span><span class="p">:</span>
+</span><span id="get_answer-116"><a href="#get_answer-116"><span class="linenos">116</span></a>        <span class="n">question</span> <span class="o">+=</span> <span class="s2">&quot;?&quot;</span>
+</span><span id="get_answer-117"><a href="#get_answer-117"><span class="linenos">117</span></a>    <span class="n">question</span> <span class="o">+=</span> <span class="s2">&quot; (y/n): &quot;</span>
+</span><span id="get_answer-118"><a href="#get_answer-118"><span class="linenos">118</span></a>    <span class="k">while</span> <span class="n">ans</span> <span class="ow">not</span> <span class="ow">in</span> <span class="p">[</span><span class="s2">&quot;y&quot;</span><span class="p">,</span> <span class="s2">&quot;yes&quot;</span><span class="p">,</span> <span class="s2">&quot;no&quot;</span><span class="p">,</span> <span class="s2">&quot;n&quot;</span><span class="p">]:</span>
+</span><span id="get_answer-119"><a href="#get_answer-119"><span class="linenos">119</span></a>        <span class="n">ans</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span><span class="n">question</span><span class="p">)</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span>
+</span><span id="get_answer-120"><a href="#get_answer-120"><span class="linenos">120</span></a>        <span class="k">if</span> <span class="n">ans</span> <span class="ow">in</span> <span class="p">[</span><span class="s2">&quot;y&quot;</span><span class="p">,</span> <span class="s2">&quot;yes&quot;</span><span class="p">]:</span>
+</span><span id="get_answer-121"><a href="#get_answer-121"><span class="linenos">121</span></a>            <span class="k">return</span> <span class="kc">True</span>
+</span><span id="get_answer-122"><a href="#get_answer-122"><span class="linenos">122</span></a>        <span class="k">elif</span> <span class="n">ans</span> <span class="ow">in</span> <span class="p">[</span><span class="s2">&quot;n&quot;</span><span class="p">,</span> <span class="s2">&quot;no&quot;</span><span class="p">]:</span>
+</span><span id="get_answer-123"><a href="#get_answer-123"><span class="linenos">123</span></a>            <span class="k">return</span> <span class="kc">False</span>
+</span><span id="get_answer-124"><a href="#get_answer-124"><span class="linenos">124</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="get_answer-125"><a href="#get_answer-125"><span class="linenos">125</span></a>            <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Invalid answer.&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Repeatedly ask the user a yes/no question
 until a 'y' or a 'n' is received.</p>
 </div>
 
@@ -513,31 +511,31 @@
         <span class="def">def</span>
         <span class="name">check_pypi_for_name</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">package_name</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">) -> <span class="nb">bool</span>:</span></span>
 
                 <label class="view-source-button" for="check_pypi_for_name-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#check_pypi_for_name"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="check_pypi_for_name-130"><a href="#check_pypi_for_name-130"><span class="linenos">130</span></a><span class="k">def</span> <span class="nf">check_pypi_for_name</span><span class="p">(</span><span class="n">package_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
-</span><span id="check_pypi_for_name-131"><a href="#check_pypi_for_name-131"><span class="linenos">131</span></a>    <span class="sd">&quot;&quot;&quot;Check if a package with package_name</span>
-</span><span id="check_pypi_for_name-132"><a href="#check_pypi_for_name-132"><span class="linenos">132</span></a><span class="sd">    already exists on pypi.org .</span>
-</span><span id="check_pypi_for_name-133"><a href="#check_pypi_for_name-133"><span class="linenos">133</span></a><span class="sd">    Returns True if package name exists.</span>
-</span><span id="check_pypi_for_name-134"><a href="#check_pypi_for_name-134"><span class="linenos">134</span></a><span class="sd">    Only checks the first page of results.&quot;&quot;&quot;</span>
-</span><span id="check_pypi_for_name-135"><a href="#check_pypi_for_name-135"><span class="linenos">135</span></a>    <span class="n">url</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;https://pypi.org/search/?q=</span><span class="si">{</span><span class="n">package_name</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="check_pypi_for_name-136"><a href="#check_pypi_for_name-136"><span class="linenos">136</span></a>    <span class="n">response</span> <span class="o">=</span> <span class="n">requests</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="n">url</span><span class="p">)</span>
-</span><span id="check_pypi_for_name-137"><a href="#check_pypi_for_name-137"><span class="linenos">137</span></a>    <span class="k">if</span> <span class="n">response</span><span class="o">.</span><span class="n">status_code</span> <span class="o">!=</span> <span class="mi">200</span><span class="p">:</span>
-</span><span id="check_pypi_for_name-138"><a href="#check_pypi_for_name-138"><span class="linenos">138</span></a>        <span class="k">raise</span> <span class="ne">RuntimeError</span><span class="p">(</span>
-</span><span id="check_pypi_for_name-139"><a href="#check_pypi_for_name-139"><span class="linenos">139</span></a>            <span class="sa">f</span><span class="s2">&quot;Error: pypi.org returned status code: </span><span class="si">{</span><span class="n">response</span><span class="o">.</span><span class="n">status_code</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="check_pypi_for_name-140"><a href="#check_pypi_for_name-140"><span class="linenos">140</span></a>        <span class="p">)</span>
-</span><span id="check_pypi_for_name-141"><a href="#check_pypi_for_name-141"><span class="linenos">141</span></a>    <span class="n">soup</span> <span class="o">=</span> <span class="n">BeautifulSoup</span><span class="p">(</span><span class="n">response</span><span class="o">.</span><span class="n">text</span><span class="p">,</span> <span class="s2">&quot;html.parser&quot;</span><span class="p">)</span>
-</span><span id="check_pypi_for_name-142"><a href="#check_pypi_for_name-142"><span class="linenos">142</span></a>    <span class="n">pypi_packages</span> <span class="o">=</span> <span class="p">[</span>
-</span><span id="check_pypi_for_name-143"><a href="#check_pypi_for_name-143"><span class="linenos">143</span></a>        <span class="n">span</span><span class="o">.</span><span class="n">text</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span>
-</span><span id="check_pypi_for_name-144"><a href="#check_pypi_for_name-144"><span class="linenos">144</span></a>        <span class="k">for</span> <span class="n">span</span> <span class="ow">in</span> <span class="n">soup</span><span class="o">.</span><span class="n">find_all</span><span class="p">(</span><span class="s2">&quot;span&quot;</span><span class="p">,</span> <span class="n">class_</span><span class="o">=</span><span class="s2">&quot;package-snippet__name&quot;</span><span class="p">)</span>
-</span><span id="check_pypi_for_name-145"><a href="#check_pypi_for_name-145"><span class="linenos">145</span></a>    <span class="p">]</span>
-</span><span id="check_pypi_for_name-146"><a href="#check_pypi_for_name-146"><span class="linenos">146</span></a>    <span class="k">return</span> <span class="n">package_name</span> <span class="ow">in</span> <span class="n">pypi_packages</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="check_pypi_for_name-128"><a href="#check_pypi_for_name-128"><span class="linenos">128</span></a><span class="k">def</span> <span class="nf">check_pypi_for_name</span><span class="p">(</span><span class="n">package_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
+</span><span id="check_pypi_for_name-129"><a href="#check_pypi_for_name-129"><span class="linenos">129</span></a>    <span class="sd">&quot;&quot;&quot;Check if a package with package_name</span>
+</span><span id="check_pypi_for_name-130"><a href="#check_pypi_for_name-130"><span class="linenos">130</span></a><span class="sd">    already exists on pypi.org .</span>
+</span><span id="check_pypi_for_name-131"><a href="#check_pypi_for_name-131"><span class="linenos">131</span></a><span class="sd">    Returns True if package name exists.</span>
+</span><span id="check_pypi_for_name-132"><a href="#check_pypi_for_name-132"><span class="linenos">132</span></a><span class="sd">    Only checks the first page of results.&quot;&quot;&quot;</span>
+</span><span id="check_pypi_for_name-133"><a href="#check_pypi_for_name-133"><span class="linenos">133</span></a>    <span class="n">url</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;https://pypi.org/search/?q=</span><span class="si">{</span><span class="n">package_name</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="check_pypi_for_name-134"><a href="#check_pypi_for_name-134"><span class="linenos">134</span></a>    <span class="n">response</span> <span class="o">=</span> <span class="n">requests</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="n">url</span><span class="p">)</span>
+</span><span id="check_pypi_for_name-135"><a href="#check_pypi_for_name-135"><span class="linenos">135</span></a>    <span class="k">if</span> <span class="n">response</span><span class="o">.</span><span class="n">status_code</span> <span class="o">!=</span> <span class="mi">200</span><span class="p">:</span>
+</span><span id="check_pypi_for_name-136"><a href="#check_pypi_for_name-136"><span class="linenos">136</span></a>        <span class="k">raise</span> <span class="ne">RuntimeError</span><span class="p">(</span>
+</span><span id="check_pypi_for_name-137"><a href="#check_pypi_for_name-137"><span class="linenos">137</span></a>            <span class="sa">f</span><span class="s2">&quot;Error: pypi.org returned status code: </span><span class="si">{</span><span class="n">response</span><span class="o">.</span><span class="n">status_code</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="check_pypi_for_name-138"><a href="#check_pypi_for_name-138"><span class="linenos">138</span></a>        <span class="p">)</span>
+</span><span id="check_pypi_for_name-139"><a href="#check_pypi_for_name-139"><span class="linenos">139</span></a>    <span class="n">soup</span> <span class="o">=</span> <span class="n">BeautifulSoup</span><span class="p">(</span><span class="n">response</span><span class="o">.</span><span class="n">text</span><span class="p">,</span> <span class="s2">&quot;html.parser&quot;</span><span class="p">)</span>
+</span><span id="check_pypi_for_name-140"><a href="#check_pypi_for_name-140"><span class="linenos">140</span></a>    <span class="n">pypi_packages</span> <span class="o">=</span> <span class="p">[</span>
+</span><span id="check_pypi_for_name-141"><a href="#check_pypi_for_name-141"><span class="linenos">141</span></a>        <span class="n">span</span><span class="o">.</span><span class="n">text</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span>
+</span><span id="check_pypi_for_name-142"><a href="#check_pypi_for_name-142"><span class="linenos">142</span></a>        <span class="k">for</span> <span class="n">span</span> <span class="ow">in</span> <span class="n">soup</span><span class="o">.</span><span class="n">find_all</span><span class="p">(</span><span class="s2">&quot;span&quot;</span><span class="p">,</span> <span class="n">class_</span><span class="o">=</span><span class="s2">&quot;package-snippet__name&quot;</span><span class="p">)</span>
+</span><span id="check_pypi_for_name-143"><a href="#check_pypi_for_name-143"><span class="linenos">143</span></a>    <span class="p">]</span>
+</span><span id="check_pypi_for_name-144"><a href="#check_pypi_for_name-144"><span class="linenos">144</span></a>    <span class="k">return</span> <span class="n">package_name</span> <span class="ow">in</span> <span class="n">pypi_packages</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Check if a package with package_name
 already exists on pypi.org .
 Returns True if package name exists.
 Only checks the first page of results.</p>
@@ -552,192 +550,192 @@
         <span class="def">def</span>
         <span class="name">check_pypi_for_name_cli</span><span class="signature pdoc-code condensed">(<span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="check_pypi_for_name_cli-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#check_pypi_for_name_cli"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="check_pypi_for_name_cli-149"><a href="#check_pypi_for_name_cli-149"><span class="linenos">149</span></a><span class="k">def</span> <span class="nf">check_pypi_for_name_cli</span><span class="p">():</span>
-</span><span id="check_pypi_for_name_cli-150"><a href="#check_pypi_for_name_cli-150"><span class="linenos">150</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">argparse</span><span class="o">.</span><span class="n">ArgumentParser</span><span class="p">()</span>
-</span><span id="check_pypi_for_name_cli-151"><a href="#check_pypi_for_name_cli-151"><span class="linenos">151</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span><span class="s2">&quot;name&quot;</span><span class="p">,</span> <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">)</span>
-</span><span id="check_pypi_for_name_cli-152"><a href="#check_pypi_for_name_cli-152"><span class="linenos">152</span></a>    <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="o">.</span><span class="n">parse_args</span><span class="p">()</span>
-</span><span id="check_pypi_for_name_cli-153"><a href="#check_pypi_for_name_cli-153"><span class="linenos">153</span></a>    <span class="k">if</span> <span class="n">check_pypi_for_name</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="p">):</span>
-</span><span id="check_pypi_for_name_cli-154"><a href="#check_pypi_for_name_cli-154"><span class="linenos">154</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2"> is already taken.&quot;</span><span class="p">)</span>
-</span><span id="check_pypi_for_name_cli-155"><a href="#check_pypi_for_name_cli-155"><span class="linenos">155</span></a>    <span class="k">else</span><span class="p">:</span>
-</span><span id="check_pypi_for_name_cli-156"><a href="#check_pypi_for_name_cli-156"><span class="linenos">156</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2"> is available.&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="check_pypi_for_name_cli-147"><a href="#check_pypi_for_name_cli-147"><span class="linenos">147</span></a><span class="k">def</span> <span class="nf">check_pypi_for_name_cli</span><span class="p">():</span>
+</span><span id="check_pypi_for_name_cli-148"><a href="#check_pypi_for_name_cli-148"><span class="linenos">148</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">argparse</span><span class="o">.</span><span class="n">ArgumentParser</span><span class="p">()</span>
+</span><span id="check_pypi_for_name_cli-149"><a href="#check_pypi_for_name_cli-149"><span class="linenos">149</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span><span class="s2">&quot;name&quot;</span><span class="p">,</span> <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">)</span>
+</span><span id="check_pypi_for_name_cli-150"><a href="#check_pypi_for_name_cli-150"><span class="linenos">150</span></a>    <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="o">.</span><span class="n">parse_args</span><span class="p">()</span>
+</span><span id="check_pypi_for_name_cli-151"><a href="#check_pypi_for_name_cli-151"><span class="linenos">151</span></a>    <span class="k">if</span> <span class="n">check_pypi_for_name</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="p">):</span>
+</span><span id="check_pypi_for_name_cli-152"><a href="#check_pypi_for_name_cli-152"><span class="linenos">152</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2"> is already taken.&quot;</span><span class="p">)</span>
+</span><span id="check_pypi_for_name_cli-153"><a href="#check_pypi_for_name_cli-153"><span class="linenos">153</span></a>    <span class="k">else</span><span class="p">:</span>
+</span><span id="check_pypi_for_name_cli-154"><a href="#check_pypi_for_name_cli-154"><span class="linenos">154</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2"> is available.&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
     
 
                 </section>
                 <section id="create_pyproject_file">
                             <input id="create_pyproject_file-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="def">def</span>
-        <span class="name">create_pyproject_file</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">targetdir</span><span class="p">:</span> <span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span>, </span><span class="param"><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span></span><span class="return-annotation">):</span></span>
+        <span class="name">create_pyproject_file</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">targetdir</span><span class="p">:</span> <span class="n">pathier</span><span class="o">.</span><span class="n">pathier</span><span class="o">.</span><span class="n">Pathier</span>, </span><span class="param"><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="create_pyproject_file-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#create_pyproject_file"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="create_pyproject_file-159"><a href="#create_pyproject_file-159"><span class="linenos">159</span></a><span class="k">def</span> <span class="nf">create_pyproject_file</span><span class="p">(</span><span class="n">targetdir</span><span class="p">:</span> <span class="n">Path</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
-</span><span id="create_pyproject_file-160"><a href="#create_pyproject_file-160"><span class="linenos">160</span></a>    <span class="sd">&quot;&quot;&quot;Create pyproject.toml in ./{project_name} from args,</span>
-</span><span id="create_pyproject_file-161"><a href="#create_pyproject_file-161"><span class="linenos">161</span></a><span class="sd">    pyproject_template, and hassle_config.&quot;&quot;&quot;</span>
-</span><span id="create_pyproject_file-162"><a href="#create_pyproject_file-162"><span class="linenos">162</span></a>    <span class="n">pyproject</span> <span class="o">=</span> <span class="n">tomlkit</span><span class="o">.</span><span class="n">loads</span><span class="p">((</span><span class="n">root</span> <span class="o">/</span> <span class="s2">&quot;pyproject_template.toml&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">read_text</span><span class="p">())</span>
-</span><span id="create_pyproject_file-163"><a href="#create_pyproject_file-163"><span class="linenos">163</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">hassle_config</span><span class="o">.</span><span class="n">config_exists</span><span class="p">():</span>
-</span><span id="create_pyproject_file-164"><a href="#create_pyproject_file-164"><span class="linenos">164</span></a>        <span class="n">hassle_config</span><span class="o">.</span><span class="n">warn</span><span class="p">()</span>
-</span><span id="create_pyproject_file-165"><a href="#create_pyproject_file-165"><span class="linenos">165</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">get_answer</span><span class="p">(</span><span class="s2">&quot;Continue creating new package with blank config?&quot;</span><span class="p">):</span>
-</span><span id="create_pyproject_file-166"><a href="#create_pyproject_file-166"><span class="linenos">166</span></a>            <span class="k">raise</span> <span class="ne">Exception</span><span class="p">(</span><span class="s2">&quot;Aborting new package creation&quot;</span><span class="p">)</span>
-</span><span id="create_pyproject_file-167"><a href="#create_pyproject_file-167"><span class="linenos">167</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="create_pyproject_file-168"><a href="#create_pyproject_file-168"><span class="linenos">168</span></a>            <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Creating blank hassle_config.toml...&quot;</span><span class="p">)</span>
-</span><span id="create_pyproject_file-169"><a href="#create_pyproject_file-169"><span class="linenos">169</span></a>            <span class="n">hassle_config</span><span class="o">.</span><span class="n">create_config</span><span class="p">()</span>
-</span><span id="create_pyproject_file-170"><a href="#create_pyproject_file-170"><span class="linenos">170</span></a>    <span class="n">config</span> <span class="o">=</span> <span class="n">hassle_config</span><span class="o">.</span><span class="n">load_config</span><span class="p">()</span>
-</span><span id="create_pyproject_file-171"><a href="#create_pyproject_file-171"><span class="linenos">171</span></a>    <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;name&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">name</span>
-</span><span id="create_pyproject_file-172"><a href="#create_pyproject_file-172"><span class="linenos">172</span></a>    <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;authors&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">config</span><span class="p">[</span><span class="s2">&quot;authors&quot;</span><span class="p">]</span>
-</span><span id="create_pyproject_file-173"><a href="#create_pyproject_file-173"><span class="linenos">173</span></a>    <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;description&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">description</span>
-</span><span id="create_pyproject_file-174"><a href="#create_pyproject_file-174"><span class="linenos">174</span></a>    <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;dependencies&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">dependencies</span>
-</span><span id="create_pyproject_file-175"><a href="#create_pyproject_file-175"><span class="linenos">175</span></a>    <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;keywords&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">keywords</span>
-</span><span id="create_pyproject_file-176"><a href="#create_pyproject_file-176"><span class="linenos">176</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">operating_system</span><span class="p">:</span>
-</span><span id="create_pyproject_file-177"><a href="#create_pyproject_file-177"><span class="linenos">177</span></a>        <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;classifiers&quot;</span><span class="p">][</span><span class="mi">2</span><span class="p">]</span> <span class="o">=</span> <span class="s2">&quot;Operating System :: &quot;</span> <span class="o">+</span> <span class="s2">&quot; &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span>
-</span><span id="create_pyproject_file-178"><a href="#create_pyproject_file-178"><span class="linenos">178</span></a>            <span class="n">args</span><span class="o">.</span><span class="n">operating_system</span>
-</span><span id="create_pyproject_file-179"><a href="#create_pyproject_file-179"><span class="linenos">179</span></a>        <span class="p">)</span>
-</span><span id="create_pyproject_file-180"><a href="#create_pyproject_file-180"><span class="linenos">180</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">no_license</span><span class="p">:</span>
-</span><span id="create_pyproject_file-181"><a href="#create_pyproject_file-181"><span class="linenos">181</span></a>        <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;classifiers&quot;</span><span class="p">]</span><span class="o">.</span><span class="n">pop</span><span class="p">(</span><span class="mi">1</span><span class="p">)</span>
-</span><span id="create_pyproject_file-182"><a href="#create_pyproject_file-182"><span class="linenos">182</span></a>    <span class="k">for</span> <span class="n">field</span> <span class="ow">in</span> <span class="n">config</span><span class="p">[</span><span class="s2">&quot;project_urls&quot;</span><span class="p">]:</span>
-</span><span id="create_pyproject_file-183"><a href="#create_pyproject_file-183"><span class="linenos">183</span></a>        <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;urls&quot;</span><span class="p">][</span><span class="n">field</span><span class="p">]</span> <span class="o">=</span> <span class="n">config</span><span class="p">[</span><span class="s2">&quot;project_urls&quot;</span><span class="p">][</span><span class="n">field</span><span class="p">]</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span>
-</span><span id="create_pyproject_file-184"><a href="#create_pyproject_file-184"><span class="linenos">184</span></a>            <span class="s2">&quot;$name&quot;</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">name</span>
-</span><span id="create_pyproject_file-185"><a href="#create_pyproject_file-185"><span class="linenos">185</span></a>        <span class="p">)</span>
-</span><span id="create_pyproject_file-186"><a href="#create_pyproject_file-186"><span class="linenos">186</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">add_script</span><span class="p">:</span>
-</span><span id="create_pyproject_file-187"><a href="#create_pyproject_file-187"><span class="linenos">187</span></a>        <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;scripts&quot;</span><span class="p">][</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="p">]</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2">.</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2">:main&quot;</span>
-</span><span id="create_pyproject_file-188"><a href="#create_pyproject_file-188"><span class="linenos">188</span></a>    <span class="p">(</span><span class="n">targetdir</span> <span class="o">/</span> <span class="s2">&quot;pyproject.toml&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="n">tomlkit</span><span class="o">.</span><span class="n">dumps</span><span class="p">(</span><span class="n">pyproject</span><span class="p">))</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="create_pyproject_file-157"><a href="#create_pyproject_file-157"><span class="linenos">157</span></a><span class="k">def</span> <span class="nf">create_pyproject_file</span><span class="p">(</span><span class="n">targetdir</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
+</span><span id="create_pyproject_file-158"><a href="#create_pyproject_file-158"><span class="linenos">158</span></a>    <span class="sd">&quot;&quot;&quot;Create pyproject.toml in ./{project_name} from args,</span>
+</span><span id="create_pyproject_file-159"><a href="#create_pyproject_file-159"><span class="linenos">159</span></a><span class="sd">    pyproject_template, and hassle_config.&quot;&quot;&quot;</span>
+</span><span id="create_pyproject_file-160"><a href="#create_pyproject_file-160"><span class="linenos">160</span></a>    <span class="n">pyproject</span> <span class="o">=</span> <span class="p">(</span><span class="n">root</span> <span class="o">/</span> <span class="s2">&quot;pyproject_template.toml&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">loads</span><span class="p">()</span>
+</span><span id="create_pyproject_file-161"><a href="#create_pyproject_file-161"><span class="linenos">161</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">hassle_config</span><span class="o">.</span><span class="n">config_exists</span><span class="p">():</span>
+</span><span id="create_pyproject_file-162"><a href="#create_pyproject_file-162"><span class="linenos">162</span></a>        <span class="n">hassle_config</span><span class="o">.</span><span class="n">warn</span><span class="p">()</span>
+</span><span id="create_pyproject_file-163"><a href="#create_pyproject_file-163"><span class="linenos">163</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">get_answer</span><span class="p">(</span><span class="s2">&quot;Continue creating new package with blank config?&quot;</span><span class="p">):</span>
+</span><span id="create_pyproject_file-164"><a href="#create_pyproject_file-164"><span class="linenos">164</span></a>            <span class="k">raise</span> <span class="ne">Exception</span><span class="p">(</span><span class="s2">&quot;Aborting new package creation&quot;</span><span class="p">)</span>
+</span><span id="create_pyproject_file-165"><a href="#create_pyproject_file-165"><span class="linenos">165</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="create_pyproject_file-166"><a href="#create_pyproject_file-166"><span class="linenos">166</span></a>            <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Creating blank hassle_config.toml...&quot;</span><span class="p">)</span>
+</span><span id="create_pyproject_file-167"><a href="#create_pyproject_file-167"><span class="linenos">167</span></a>            <span class="n">hassle_config</span><span class="o">.</span><span class="n">create_config</span><span class="p">()</span>
+</span><span id="create_pyproject_file-168"><a href="#create_pyproject_file-168"><span class="linenos">168</span></a>    <span class="n">config</span> <span class="o">=</span> <span class="n">hassle_config</span><span class="o">.</span><span class="n">load_config</span><span class="p">()</span>
+</span><span id="create_pyproject_file-169"><a href="#create_pyproject_file-169"><span class="linenos">169</span></a>    <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;name&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">name</span>
+</span><span id="create_pyproject_file-170"><a href="#create_pyproject_file-170"><span class="linenos">170</span></a>    <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;authors&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">config</span><span class="p">[</span><span class="s2">&quot;authors&quot;</span><span class="p">]</span>
+</span><span id="create_pyproject_file-171"><a href="#create_pyproject_file-171"><span class="linenos">171</span></a>    <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;description&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">description</span>
+</span><span id="create_pyproject_file-172"><a href="#create_pyproject_file-172"><span class="linenos">172</span></a>    <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;dependencies&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">dependencies</span>
+</span><span id="create_pyproject_file-173"><a href="#create_pyproject_file-173"><span class="linenos">173</span></a>    <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;keywords&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">keywords</span>
+</span><span id="create_pyproject_file-174"><a href="#create_pyproject_file-174"><span class="linenos">174</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">operating_system</span><span class="p">:</span>
+</span><span id="create_pyproject_file-175"><a href="#create_pyproject_file-175"><span class="linenos">175</span></a>        <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;classifiers&quot;</span><span class="p">][</span><span class="mi">2</span><span class="p">]</span> <span class="o">=</span> <span class="s2">&quot;Operating System :: &quot;</span> <span class="o">+</span> <span class="s2">&quot; &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span>
+</span><span id="create_pyproject_file-176"><a href="#create_pyproject_file-176"><span class="linenos">176</span></a>            <span class="n">args</span><span class="o">.</span><span class="n">operating_system</span>
+</span><span id="create_pyproject_file-177"><a href="#create_pyproject_file-177"><span class="linenos">177</span></a>        <span class="p">)</span>
+</span><span id="create_pyproject_file-178"><a href="#create_pyproject_file-178"><span class="linenos">178</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">no_license</span><span class="p">:</span>
+</span><span id="create_pyproject_file-179"><a href="#create_pyproject_file-179"><span class="linenos">179</span></a>        <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;classifiers&quot;</span><span class="p">]</span><span class="o">.</span><span class="n">pop</span><span class="p">(</span><span class="mi">1</span><span class="p">)</span>
+</span><span id="create_pyproject_file-180"><a href="#create_pyproject_file-180"><span class="linenos">180</span></a>    <span class="k">for</span> <span class="n">field</span> <span class="ow">in</span> <span class="n">config</span><span class="p">[</span><span class="s2">&quot;project_urls&quot;</span><span class="p">]:</span>
+</span><span id="create_pyproject_file-181"><a href="#create_pyproject_file-181"><span class="linenos">181</span></a>        <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;urls&quot;</span><span class="p">][</span><span class="n">field</span><span class="p">]</span> <span class="o">=</span> <span class="n">config</span><span class="p">[</span><span class="s2">&quot;project_urls&quot;</span><span class="p">][</span><span class="n">field</span><span class="p">]</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span>
+</span><span id="create_pyproject_file-182"><a href="#create_pyproject_file-182"><span class="linenos">182</span></a>            <span class="s2">&quot;$name&quot;</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">name</span>
+</span><span id="create_pyproject_file-183"><a href="#create_pyproject_file-183"><span class="linenos">183</span></a>        <span class="p">)</span>
+</span><span id="create_pyproject_file-184"><a href="#create_pyproject_file-184"><span class="linenos">184</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">add_script</span><span class="p">:</span>
+</span><span id="create_pyproject_file-185"><a href="#create_pyproject_file-185"><span class="linenos">185</span></a>        <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;scripts&quot;</span><span class="p">][</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="p">]</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2">.</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2">:main&quot;</span>
+</span><span id="create_pyproject_file-186"><a href="#create_pyproject_file-186"><span class="linenos">186</span></a>    <span class="p">(</span><span class="n">targetdir</span> <span class="o">/</span> <span class="s2">&quot;pyproject.toml&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">dumps</span><span class="p">(</span><span class="n">pyproject</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Create pyproject.toml in ./{project_name} from args,
 pyproject_template, and hassle_config.</p>
 </div>
 
 
                 </section>
                 <section id="create_source_files">
                             <input id="create_source_files-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="def">def</span>
-        <span class="name">create_source_files</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">srcdir</span><span class="p">:</span> <span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span>, </span><span class="param"><span class="n">filelist</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span></span><span class="return-annotation">):</span></span>
+        <span class="name">create_source_files</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">srcdir</span><span class="p">:</span> <span class="n">pathier</span><span class="o">.</span><span class="n">pathier</span><span class="o">.</span><span class="n">Pathier</span>, </span><span class="param"><span class="n">filelist</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="create_source_files-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#create_source_files"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="create_source_files-191"><a href="#create_source_files-191"><span class="linenos">191</span></a><span class="k">def</span> <span class="nf">create_source_files</span><span class="p">(</span><span class="n">srcdir</span><span class="p">:</span> <span class="n">Path</span><span class="p">,</span> <span class="n">filelist</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]):</span>
-</span><span id="create_source_files-192"><a href="#create_source_files-192"><span class="linenos">192</span></a>    <span class="sd">&quot;&quot;&quot;Generate empty source files in ./{package_name}/src/{package_name}/&quot;&quot;&quot;</span>
-</span><span id="create_source_files-193"><a href="#create_source_files-193"><span class="linenos">193</span></a>    <span class="n">srcdir</span><span class="o">.</span><span class="n">mkdir</span><span class="p">(</span><span class="n">parents</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">exist_ok</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
-</span><span id="create_source_files-194"><a href="#create_source_files-194"><span class="linenos">194</span></a>    <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">filelist</span><span class="p">:</span>
-</span><span id="create_source_files-195"><a href="#create_source_files-195"><span class="linenos">195</span></a>        <span class="p">(</span><span class="n">srcdir</span> <span class="o">/</span> <span class="n">file</span><span class="p">)</span><span class="o">.</span><span class="n">touch</span><span class="p">()</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="create_source_files-189"><a href="#create_source_files-189"><span class="linenos">189</span></a><span class="k">def</span> <span class="nf">create_source_files</span><span class="p">(</span><span class="n">srcdir</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">,</span> <span class="n">filelist</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]):</span>
+</span><span id="create_source_files-190"><a href="#create_source_files-190"><span class="linenos">190</span></a>    <span class="sd">&quot;&quot;&quot;Generate empty source files in ./{package_name}/src/{package_name}/&quot;&quot;&quot;</span>
+</span><span id="create_source_files-191"><a href="#create_source_files-191"><span class="linenos">191</span></a>    <span class="n">srcdir</span><span class="o">.</span><span class="n">mkdir</span><span class="p">(</span><span class="n">parents</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">exist_ok</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
+</span><span id="create_source_files-192"><a href="#create_source_files-192"><span class="linenos">192</span></a>    <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">filelist</span><span class="p">:</span>
+</span><span id="create_source_files-193"><a href="#create_source_files-193"><span class="linenos">193</span></a>        <span class="p">(</span><span class="n">srcdir</span> <span class="o">/</span> <span class="n">file</span><span class="p">)</span><span class="o">.</span><span class="n">touch</span><span class="p">()</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Generate empty source files in ./{package_name}/src/{package_name}/</p>
 </div>
 
 
                 </section>
                 <section id="create_readme">
                             <input id="create_readme-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="def">def</span>
-        <span class="name">create_readme</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">targetdir</span><span class="p">:</span> <span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span>, </span><span class="param"><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span></span><span class="return-annotation">):</span></span>
+        <span class="name">create_readme</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">targetdir</span><span class="p">:</span> <span class="n">pathier</span><span class="o">.</span><span class="n">pathier</span><span class="o">.</span><span class="n">Pathier</span>, </span><span class="param"><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="create_readme-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#create_readme"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="create_readme-198"><a href="#create_readme-198"><span class="linenos">198</span></a><span class="k">def</span> <span class="nf">create_readme</span><span class="p">(</span><span class="n">targetdir</span><span class="p">:</span> <span class="n">Path</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
-</span><span id="create_readme-199"><a href="#create_readme-199"><span class="linenos">199</span></a>    <span class="sd">&quot;&quot;&quot;Create README.md in ./{package_name}</span>
-</span><span id="create_readme-200"><a href="#create_readme-200"><span class="linenos">200</span></a><span class="sd">    from readme_template and args.&quot;&quot;&quot;</span>
-</span><span id="create_readme-201"><a href="#create_readme-201"><span class="linenos">201</span></a>    <span class="n">readme</span> <span class="o">=</span> <span class="p">(</span><span class="n">root</span> <span class="o">/</span> <span class="s2">&quot;README_template.md&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">read_text</span><span class="p">()</span>
-</span><span id="create_readme-202"><a href="#create_readme-202"><span class="linenos">202</span></a>    <span class="n">readme</span> <span class="o">=</span> <span class="n">readme</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;$name&quot;</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="p">)</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span>
-</span><span id="create_readme-203"><a href="#create_readme-203"><span class="linenos">203</span></a>        <span class="s2">&quot;$description&quot;</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">description</span>
-</span><span id="create_readme-204"><a href="#create_readme-204"><span class="linenos">204</span></a>    <span class="p">)</span>
-</span><span id="create_readme-205"><a href="#create_readme-205"><span class="linenos">205</span></a>    <span class="p">(</span><span class="n">targetdir</span> <span class="o">/</span> <span class="s2">&quot;README.md&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="n">readme</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="create_readme-196"><a href="#create_readme-196"><span class="linenos">196</span></a><span class="k">def</span> <span class="nf">create_readme</span><span class="p">(</span><span class="n">targetdir</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
+</span><span id="create_readme-197"><a href="#create_readme-197"><span class="linenos">197</span></a>    <span class="sd">&quot;&quot;&quot;Create README.md in ./{package_name}</span>
+</span><span id="create_readme-198"><a href="#create_readme-198"><span class="linenos">198</span></a><span class="sd">    from readme_template and args.&quot;&quot;&quot;</span>
+</span><span id="create_readme-199"><a href="#create_readme-199"><span class="linenos">199</span></a>    <span class="n">readme</span> <span class="o">=</span> <span class="p">(</span><span class="n">root</span> <span class="o">/</span> <span class="s2">&quot;README_template.md&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">read_text</span><span class="p">()</span>
+</span><span id="create_readme-200"><a href="#create_readme-200"><span class="linenos">200</span></a>    <span class="n">readme</span> <span class="o">=</span> <span class="n">readme</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;$name&quot;</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="p">)</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span>
+</span><span id="create_readme-201"><a href="#create_readme-201"><span class="linenos">201</span></a>        <span class="s2">&quot;$description&quot;</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">description</span>
+</span><span id="create_readme-202"><a href="#create_readme-202"><span class="linenos">202</span></a>    <span class="p">)</span>
+</span><span id="create_readme-203"><a href="#create_readme-203"><span class="linenos">203</span></a>    <span class="p">(</span><span class="n">targetdir</span> <span class="o">/</span> <span class="s2">&quot;README.md&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="n">readme</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Create README.md in ./{package_name}
 from readme_template and args.</p>
 </div>
 
 
                 </section>
                 <section id="create_license">
                             <input id="create_license-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="def">def</span>
-        <span class="name">create_license</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">targetdir</span><span class="p">:</span> <span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span></span><span class="return-annotation">):</span></span>
+        <span class="name">create_license</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">targetdir</span><span class="p">:</span> <span class="n">pathier</span><span class="o">.</span><span class="n">pathier</span><span class="o">.</span><span class="n">Pathier</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="create_license-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#create_license"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="create_license-208"><a href="#create_license-208"><span class="linenos">208</span></a><span class="k">def</span> <span class="nf">create_license</span><span class="p">(</span><span class="n">targetdir</span><span class="p">:</span> <span class="n">Path</span><span class="p">):</span>
-</span><span id="create_license-209"><a href="#create_license-209"><span class="linenos">209</span></a>    <span class="sd">&quot;&quot;&quot;Add MIT license file to ./{package_name} .&quot;&quot;&quot;</span>
-</span><span id="create_license-210"><a href="#create_license-210"><span class="linenos">210</span></a>    <span class="n">license_template</span> <span class="o">=</span> <span class="p">(</span><span class="n">root</span> <span class="o">/</span> <span class="s2">&quot;license_template.txt&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">read_text</span><span class="p">()</span>
-</span><span id="create_license-211"><a href="#create_license-211"><span class="linenos">211</span></a>    <span class="n">license_template</span> <span class="o">=</span> <span class="n">license_template</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;$year&quot;</span><span class="p">,</span> <span class="nb">str</span><span class="p">(</span><span class="n">datetime</span><span class="o">.</span><span class="n">now</span><span class="p">()</span><span class="o">.</span><span class="n">year</span><span class="p">))</span>
-</span><span id="create_license-212"><a href="#create_license-212"><span class="linenos">212</span></a>    <span class="p">(</span><span class="n">targetdir</span> <span class="o">/</span> <span class="s2">&quot;LICENSE.txt&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="n">license_template</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="create_license-206"><a href="#create_license-206"><span class="linenos">206</span></a><span class="k">def</span> <span class="nf">create_license</span><span class="p">(</span><span class="n">targetdir</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">):</span>
+</span><span id="create_license-207"><a href="#create_license-207"><span class="linenos">207</span></a>    <span class="sd">&quot;&quot;&quot;Add MIT license file to ./{package_name} .&quot;&quot;&quot;</span>
+</span><span id="create_license-208"><a href="#create_license-208"><span class="linenos">208</span></a>    <span class="n">license_template</span> <span class="o">=</span> <span class="p">(</span><span class="n">root</span> <span class="o">/</span> <span class="s2">&quot;license_template.txt&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">read_text</span><span class="p">()</span>
+</span><span id="create_license-209"><a href="#create_license-209"><span class="linenos">209</span></a>    <span class="n">license_template</span> <span class="o">=</span> <span class="n">license_template</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;$year&quot;</span><span class="p">,</span> <span class="nb">str</span><span class="p">(</span><span class="n">datetime</span><span class="o">.</span><span class="n">now</span><span class="p">()</span><span class="o">.</span><span class="n">year</span><span class="p">))</span>
+</span><span id="create_license-210"><a href="#create_license-210"><span class="linenos">210</span></a>    <span class="p">(</span><span class="n">targetdir</span> <span class="o">/</span> <span class="s2">&quot;LICENSE.txt&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="n">license_template</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Add MIT license file to ./{package_name} .</p>
 </div>
 
 
                 </section>
                 <section id="create_gitignore">
                             <input id="create_gitignore-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="def">def</span>
-        <span class="name">create_gitignore</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">targetdir</span><span class="p">:</span> <span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span></span><span class="return-annotation">):</span></span>
+        <span class="name">create_gitignore</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">targetdir</span><span class="p">:</span> <span class="n">pathier</span><span class="o">.</span><span class="n">pathier</span><span class="o">.</span><span class="n">Pathier</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="create_gitignore-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#create_gitignore"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="create_gitignore-215"><a href="#create_gitignore-215"><span class="linenos">215</span></a><span class="k">def</span> <span class="nf">create_gitignore</span><span class="p">(</span><span class="n">targetdir</span><span class="p">:</span> <span class="n">Path</span><span class="p">):</span>
-</span><span id="create_gitignore-216"><a href="#create_gitignore-216"><span class="linenos">216</span></a>    <span class="sd">&quot;&quot;&quot;Add .gitignore to ./{package_name}&quot;&quot;&quot;</span>
-</span><span id="create_gitignore-217"><a href="#create_gitignore-217"><span class="linenos">217</span></a>    <span class="n">shutil</span><span class="o">.</span><span class="n">copy</span><span class="p">(</span><span class="n">root</span> <span class="o">/</span> <span class="s2">&quot;.gitignore_template&quot;</span><span class="p">,</span> <span class="n">targetdir</span> <span class="o">/</span> <span class="s2">&quot;.gitignore&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="create_gitignore-213"><a href="#create_gitignore-213"><span class="linenos">213</span></a><span class="k">def</span> <span class="nf">create_gitignore</span><span class="p">(</span><span class="n">targetdir</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">):</span>
+</span><span id="create_gitignore-214"><a href="#create_gitignore-214"><span class="linenos">214</span></a>    <span class="sd">&quot;&quot;&quot;Add .gitignore to ./{package_name}&quot;&quot;&quot;</span>
+</span><span id="create_gitignore-215"><a href="#create_gitignore-215"><span class="linenos">215</span></a>    <span class="p">(</span><span class="n">root</span> <span class="o">/</span> <span class="s2">&quot;.gitignore_template&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">copy</span><span class="p">(</span><span class="n">targetdir</span> <span class="o">/</span> <span class="s2">&quot;.gitignore&quot;</span><span class="p">,</span> <span class="kc">True</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Add .gitignore to ./{package_name}</p>
 </div>
 
 
                 </section>
                 <section id="create_vscode_settings">
                             <input id="create_vscode_settings-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="def">def</span>
-        <span class="name">create_vscode_settings</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">targetdir</span><span class="p">:</span> <span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span></span><span class="return-annotation">):</span></span>
+        <span class="name">create_vscode_settings</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">targetdir</span><span class="p">:</span> <span class="n">pathier</span><span class="o">.</span><span class="n">pathier</span><span class="o">.</span><span class="n">Pathier</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="create_vscode_settings-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#create_vscode_settings"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="create_vscode_settings-220"><a href="#create_vscode_settings-220"><span class="linenos">220</span></a><span class="k">def</span> <span class="nf">create_vscode_settings</span><span class="p">(</span><span class="n">targetdir</span><span class="p">:</span> <span class="n">Path</span><span class="p">):</span>
-</span><span id="create_vscode_settings-221"><a href="#create_vscode_settings-221"><span class="linenos">221</span></a>    <span class="sd">&quot;&quot;&quot;Add settings.json to ./.vscode&quot;&quot;&quot;</span>
-</span><span id="create_vscode_settings-222"><a href="#create_vscode_settings-222"><span class="linenos">222</span></a>    <span class="n">vsdir</span> <span class="o">=</span> <span class="n">targetdir</span> <span class="o">/</span> <span class="s2">&quot;.vscode&quot;</span>
-</span><span id="create_vscode_settings-223"><a href="#create_vscode_settings-223"><span class="linenos">223</span></a>    <span class="n">vsdir</span><span class="o">.</span><span class="n">mkdir</span><span class="p">(</span><span class="n">parents</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">exist_ok</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
-</span><span id="create_vscode_settings-224"><a href="#create_vscode_settings-224"><span class="linenos">224</span></a>    <span class="n">shutil</span><span class="o">.</span><span class="n">copy</span><span class="p">(</span><span class="n">root</span> <span class="o">/</span> <span class="s2">&quot;.vscode_template&quot;</span><span class="p">,</span> <span class="n">vsdir</span> <span class="o">/</span> <span class="s2">&quot;settings.json&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="create_vscode_settings-218"><a href="#create_vscode_settings-218"><span class="linenos">218</span></a><span class="k">def</span> <span class="nf">create_vscode_settings</span><span class="p">(</span><span class="n">targetdir</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">):</span>
+</span><span id="create_vscode_settings-219"><a href="#create_vscode_settings-219"><span class="linenos">219</span></a>    <span class="sd">&quot;&quot;&quot;Add settings.json to ./.vscode&quot;&quot;&quot;</span>
+</span><span id="create_vscode_settings-220"><a href="#create_vscode_settings-220"><span class="linenos">220</span></a>    <span class="n">vsdir</span> <span class="o">=</span> <span class="n">targetdir</span> <span class="o">/</span> <span class="s2">&quot;.vscode&quot;</span>
+</span><span id="create_vscode_settings-221"><a href="#create_vscode_settings-221"><span class="linenos">221</span></a>    <span class="n">vsdir</span><span class="o">.</span><span class="n">mkdir</span><span class="p">(</span><span class="n">parents</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">exist_ok</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
+</span><span id="create_vscode_settings-222"><a href="#create_vscode_settings-222"><span class="linenos">222</span></a>    <span class="p">(</span><span class="n">root</span> <span class="o">/</span> <span class="s2">&quot;.vscode_template&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">copy</span><span class="p">(</span><span class="n">vsdir</span> <span class="o">/</span> <span class="s2">&quot;settings.json&quot;</span><span class="p">,</span> <span class="kc">True</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Add settings.json to ./.vscode</p>
 </div>
 
 
@@ -749,59 +747,59 @@
         <span class="def">def</span>
         <span class="name">main</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">=</span> <span class="kc">None</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="main-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#main"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="main-227"><a href="#main-227"><span class="linenos">227</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
-</span><span id="main-228"><a href="#main-228"><span class="linenos">228</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="p">:</span>
-</span><span id="main-229"><a href="#main-229"><span class="linenos">229</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
-</span><span id="main-230"><a href="#main-230"><span class="linenos">230</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">not_package</span><span class="p">:</span>
-</span><span id="main-231"><a href="#main-231"><span class="linenos">231</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="main-232"><a href="#main-232"><span class="linenos">232</span></a>            <span class="k">if</span> <span class="n">check_pypi_for_name</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="p">):</span>
-</span><span id="main-233"><a href="#main-233"><span class="linenos">233</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2"> already exists on pypi.org&quot;</span><span class="p">)</span>
-</span><span id="main-234"><a href="#main-234"><span class="linenos">234</span></a>                <span class="k">if</span> <span class="ow">not</span> <span class="n">get_answer</span><span class="p">(</span><span class="s2">&quot;Continue anyway?&quot;</span><span class="p">):</span>
-</span><span id="main-235"><a href="#main-235"><span class="linenos">235</span></a>                    <span class="n">sys</span><span class="o">.</span><span class="n">exit</span><span class="p">(</span><span class="mi">0</span><span class="p">)</span>
-</span><span id="main-236"><a href="#main-236"><span class="linenos">236</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="main-237"><a href="#main-237"><span class="linenos">237</span></a>            <span class="nb">print</span><span class="p">(</span><span class="n">e</span><span class="p">)</span>
-</span><span id="main-238"><a href="#main-238"><span class="linenos">238</span></a>            <span class="nb">print</span><span class="p">(</span>
-</span><span id="main-239"><a href="#main-239"><span class="linenos">239</span></a>                <span class="sa">f</span><span class="s2">&quot;Couldn&#39;t verify that </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2"> doesn&#39;t already exist on pypi.org .&quot;</span>
-</span><span id="main-240"><a href="#main-240"><span class="linenos">240</span></a>            <span class="p">)</span>
-</span><span id="main-241"><a href="#main-241"><span class="linenos">241</span></a>            <span class="k">if</span> <span class="ow">not</span> <span class="n">get_answer</span><span class="p">(</span><span class="s2">&quot;Continue anyway?&quot;</span><span class="p">):</span>
-</span><span id="main-242"><a href="#main-242"><span class="linenos">242</span></a>                <span class="n">sys</span><span class="o">.</span><span class="n">exit</span><span class="p">(</span><span class="mi">0</span><span class="p">)</span>
-</span><span id="main-243"><a href="#main-243"><span class="linenos">243</span></a>    <span class="k">try</span><span class="p">:</span>
-</span><span id="main-244"><a href="#main-244"><span class="linenos">244</span></a>        <span class="n">targetdir</span> <span class="o">=</span> <span class="n">Path</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span> <span class="o">/</span> <span class="n">args</span><span class="o">.</span><span class="n">name</span>
-</span><span id="main-245"><a href="#main-245"><span class="linenos">245</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="main-246"><a href="#main-246"><span class="linenos">246</span></a>            <span class="n">targetdir</span><span class="o">.</span><span class="n">mkdir</span><span class="p">(</span><span class="n">parents</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">exist_ok</span><span class="o">=</span><span class="kc">False</span><span class="p">)</span>
-</span><span id="main-247"><a href="#main-247"><span class="linenos">247</span></a>        <span class="k">except</span><span class="p">:</span>
-</span><span id="main-248"><a href="#main-248"><span class="linenos">248</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">targetdir</span><span class="si">}</span><span class="s2"> already exists.&quot;</span><span class="p">)</span>
-</span><span id="main-249"><a href="#main-249"><span class="linenos">249</span></a>            <span class="k">if</span> <span class="ow">not</span> <span class="n">get_answer</span><span class="p">(</span><span class="s2">&quot;Overwrite?&quot;</span><span class="p">):</span>
-</span><span id="main-250"><a href="#main-250"><span class="linenos">250</span></a>                <span class="n">sys</span><span class="o">.</span><span class="n">exit</span><span class="p">(</span><span class="mi">0</span><span class="p">)</span>
-</span><span id="main-251"><a href="#main-251"><span class="linenos">251</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">not_package</span><span class="p">:</span>
-</span><span id="main-252"><a href="#main-252"><span class="linenos">252</span></a>            <span class="n">create_pyproject_file</span><span class="p">(</span><span class="n">targetdir</span><span class="p">,</span> <span class="n">args</span><span class="p">)</span>
-</span><span id="main-253"><a href="#main-253"><span class="linenos">253</span></a>        <span class="n">create_source_files</span><span class="p">(</span>
-</span><span id="main-254"><a href="#main-254"><span class="linenos">254</span></a>            <span class="n">targetdir</span> <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">not_package</span> <span class="k">else</span> <span class="p">(</span><span class="n">targetdir</span> <span class="o">/</span> <span class="s2">&quot;src&quot;</span> <span class="o">/</span> <span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="p">),</span>
-</span><span id="main-255"><a href="#main-255"><span class="linenos">255</span></a>            <span class="n">args</span><span class="o">.</span><span class="n">source_files</span><span class="p">[</span><span class="mi">1</span><span class="p">:]</span> <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">not_package</span> <span class="k">else</span> <span class="n">args</span><span class="o">.</span><span class="n">source_files</span><span class="p">,</span>
-</span><span id="main-256"><a href="#main-256"><span class="linenos">256</span></a>        <span class="p">)</span>
-</span><span id="main-257"><a href="#main-257"><span class="linenos">257</span></a>        <span class="n">create_readme</span><span class="p">(</span><span class="n">targetdir</span><span class="p">,</span> <span class="n">args</span><span class="p">)</span>
-</span><span id="main-258"><a href="#main-258"><span class="linenos">258</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">not_package</span><span class="p">:</span>
-</span><span id="main-259"><a href="#main-259"><span class="linenos">259</span></a>            <span class="n">generate_test_files</span><span class="p">(</span><span class="n">targetdir</span><span class="p">)</span>
-</span><span id="main-260"><a href="#main-260"><span class="linenos">260</span></a>            <span class="n">create_vscode_settings</span><span class="p">(</span><span class="n">targetdir</span><span class="p">)</span>
-</span><span id="main-261"><a href="#main-261"><span class="linenos">261</span></a>        <span class="n">create_gitignore</span><span class="p">(</span><span class="n">targetdir</span><span class="p">)</span>
-</span><span id="main-262"><a href="#main-262"><span class="linenos">262</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">no_license</span><span class="p">:</span>
-</span><span id="main-263"><a href="#main-263"><span class="linenos">263</span></a>            <span class="n">create_license</span><span class="p">(</span><span class="n">targetdir</span><span class="p">)</span>
-</span><span id="main-264"><a href="#main-264"><span class="linenos">264</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">targetdir</span><span class="p">)</span>
-</span><span id="main-265"><a href="#main-265"><span class="linenos">265</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="s2">&quot;git init -b main&quot;</span><span class="p">)</span>
-</span><span id="main-266"><a href="#main-266"><span class="linenos">266</span></a>
-</span><span id="main-267"><a href="#main-267"><span class="linenos">267</span></a>    <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="main-268"><a href="#main-268"><span class="linenos">268</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="s2">&quot;Aborting new package creation&quot;</span> <span class="ow">in</span> <span class="nb">str</span><span class="p">(</span><span class="n">e</span><span class="p">):</span>
-</span><span id="main-269"><a href="#main-269"><span class="linenos">269</span></a>            <span class="nb">print</span><span class="p">(</span><span class="n">e</span><span class="p">)</span>
-</span><span id="main-270"><a href="#main-270"><span class="linenos">270</span></a>        <span class="k">if</span> <span class="n">get_answer</span><span class="p">(</span><span class="s2">&quot;Delete created files?&quot;</span><span class="p">):</span>
-</span><span id="main-271"><a href="#main-271"><span class="linenos">271</span></a>            <span class="n">shutil</span><span class="o">.</span><span class="n">rmtree</span><span class="p">(</span><span class="n">targetdir</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="main-225"><a href="#main-225"><span class="linenos">225</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
+</span><span id="main-226"><a href="#main-226"><span class="linenos">226</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="p">:</span>
+</span><span id="main-227"><a href="#main-227"><span class="linenos">227</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
+</span><span id="main-228"><a href="#main-228"><span class="linenos">228</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">not_package</span><span class="p">:</span>
+</span><span id="main-229"><a href="#main-229"><span class="linenos">229</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="main-230"><a href="#main-230"><span class="linenos">230</span></a>            <span class="k">if</span> <span class="n">check_pypi_for_name</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="p">):</span>
+</span><span id="main-231"><a href="#main-231"><span class="linenos">231</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2"> already exists on pypi.org&quot;</span><span class="p">)</span>
+</span><span id="main-232"><a href="#main-232"><span class="linenos">232</span></a>                <span class="k">if</span> <span class="ow">not</span> <span class="n">get_answer</span><span class="p">(</span><span class="s2">&quot;Continue anyway?&quot;</span><span class="p">):</span>
+</span><span id="main-233"><a href="#main-233"><span class="linenos">233</span></a>                    <span class="n">sys</span><span class="o">.</span><span class="n">exit</span><span class="p">(</span><span class="mi">0</span><span class="p">)</span>
+</span><span id="main-234"><a href="#main-234"><span class="linenos">234</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="main-235"><a href="#main-235"><span class="linenos">235</span></a>            <span class="nb">print</span><span class="p">(</span><span class="n">e</span><span class="p">)</span>
+</span><span id="main-236"><a href="#main-236"><span class="linenos">236</span></a>            <span class="nb">print</span><span class="p">(</span>
+</span><span id="main-237"><a href="#main-237"><span class="linenos">237</span></a>                <span class="sa">f</span><span class="s2">&quot;Couldn&#39;t verify that </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2"> doesn&#39;t already exist on pypi.org .&quot;</span>
+</span><span id="main-238"><a href="#main-238"><span class="linenos">238</span></a>            <span class="p">)</span>
+</span><span id="main-239"><a href="#main-239"><span class="linenos">239</span></a>            <span class="k">if</span> <span class="ow">not</span> <span class="n">get_answer</span><span class="p">(</span><span class="s2">&quot;Continue anyway?&quot;</span><span class="p">):</span>
+</span><span id="main-240"><a href="#main-240"><span class="linenos">240</span></a>                <span class="n">sys</span><span class="o">.</span><span class="n">exit</span><span class="p">(</span><span class="mi">0</span><span class="p">)</span>
+</span><span id="main-241"><a href="#main-241"><span class="linenos">241</span></a>    <span class="k">try</span><span class="p">:</span>
+</span><span id="main-242"><a href="#main-242"><span class="linenos">242</span></a>        <span class="n">targetdir</span><span class="p">:</span> <span class="n">Pathier</span> <span class="o">=</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span> <span class="o">/</span> <span class="n">args</span><span class="o">.</span><span class="n">name</span>
+</span><span id="main-243"><a href="#main-243"><span class="linenos">243</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="main-244"><a href="#main-244"><span class="linenos">244</span></a>            <span class="n">targetdir</span><span class="o">.</span><span class="n">mkdir</span><span class="p">(</span><span class="n">parents</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">exist_ok</span><span class="o">=</span><span class="kc">False</span><span class="p">)</span>
+</span><span id="main-245"><a href="#main-245"><span class="linenos">245</span></a>        <span class="k">except</span><span class="p">:</span>
+</span><span id="main-246"><a href="#main-246"><span class="linenos">246</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">targetdir</span><span class="si">}</span><span class="s2"> already exists.&quot;</span><span class="p">)</span>
+</span><span id="main-247"><a href="#main-247"><span class="linenos">247</span></a>            <span class="k">if</span> <span class="ow">not</span> <span class="n">get_answer</span><span class="p">(</span><span class="s2">&quot;Overwrite?&quot;</span><span class="p">):</span>
+</span><span id="main-248"><a href="#main-248"><span class="linenos">248</span></a>                <span class="n">sys</span><span class="o">.</span><span class="n">exit</span><span class="p">(</span><span class="mi">0</span><span class="p">)</span>
+</span><span id="main-249"><a href="#main-249"><span class="linenos">249</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">not_package</span><span class="p">:</span>
+</span><span id="main-250"><a href="#main-250"><span class="linenos">250</span></a>            <span class="n">create_pyproject_file</span><span class="p">(</span><span class="n">targetdir</span><span class="p">,</span> <span class="n">args</span><span class="p">)</span>
+</span><span id="main-251"><a href="#main-251"><span class="linenos">251</span></a>        <span class="n">create_source_files</span><span class="p">(</span>
+</span><span id="main-252"><a href="#main-252"><span class="linenos">252</span></a>            <span class="n">targetdir</span> <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">not_package</span> <span class="k">else</span> <span class="p">(</span><span class="n">targetdir</span> <span class="o">/</span> <span class="s2">&quot;src&quot;</span> <span class="o">/</span> <span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="p">),</span>
+</span><span id="main-253"><a href="#main-253"><span class="linenos">253</span></a>            <span class="n">args</span><span class="o">.</span><span class="n">source_files</span><span class="p">[</span><span class="mi">1</span><span class="p">:]</span> <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">not_package</span> <span class="k">else</span> <span class="n">args</span><span class="o">.</span><span class="n">source_files</span><span class="p">,</span>
+</span><span id="main-254"><a href="#main-254"><span class="linenos">254</span></a>        <span class="p">)</span>
+</span><span id="main-255"><a href="#main-255"><span class="linenos">255</span></a>        <span class="n">create_readme</span><span class="p">(</span><span class="n">targetdir</span><span class="p">,</span> <span class="n">args</span><span class="p">)</span>
+</span><span id="main-256"><a href="#main-256"><span class="linenos">256</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">not_package</span><span class="p">:</span>
+</span><span id="main-257"><a href="#main-257"><span class="linenos">257</span></a>            <span class="n">generate_test_files</span><span class="p">(</span><span class="n">targetdir</span><span class="p">)</span>
+</span><span id="main-258"><a href="#main-258"><span class="linenos">258</span></a>            <span class="n">create_vscode_settings</span><span class="p">(</span><span class="n">targetdir</span><span class="p">)</span>
+</span><span id="main-259"><a href="#main-259"><span class="linenos">259</span></a>        <span class="n">create_gitignore</span><span class="p">(</span><span class="n">targetdir</span><span class="p">)</span>
+</span><span id="main-260"><a href="#main-260"><span class="linenos">260</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">no_license</span><span class="p">:</span>
+</span><span id="main-261"><a href="#main-261"><span class="linenos">261</span></a>            <span class="n">create_license</span><span class="p">(</span><span class="n">targetdir</span><span class="p">)</span>
+</span><span id="main-262"><a href="#main-262"><span class="linenos">262</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">targetdir</span><span class="p">)</span>
+</span><span id="main-263"><a href="#main-263"><span class="linenos">263</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="s2">&quot;git init -b main&quot;</span><span class="p">)</span>
+</span><span id="main-264"><a href="#main-264"><span class="linenos">264</span></a>
+</span><span id="main-265"><a href="#main-265"><span class="linenos">265</span></a>    <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="main-266"><a href="#main-266"><span class="linenos">266</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="s2">&quot;Aborting new package creation&quot;</span> <span class="ow">in</span> <span class="nb">str</span><span class="p">(</span><span class="n">e</span><span class="p">):</span>
+</span><span id="main-267"><a href="#main-267"><span class="linenos">267</span></a>            <span class="nb">print</span><span class="p">(</span><span class="n">e</span><span class="p">)</span>
+</span><span id="main-268"><a href="#main-268"><span class="linenos">268</span></a>        <span class="k">if</span> <span class="n">get_answer</span><span class="p">(</span><span class="s2">&quot;Delete created files?&quot;</span><span class="p">):</span>
+</span><span id="main-269"><a href="#main-269"><span class="linenos">269</span></a>            <span class="n">targetdir</span><span class="o">.</span><span class="n">delete</span><span class="p">()</span>
 </span></pre></div>
 
 
     
 
                 </section>
     </main>
```

#### html2text {}

```diff
@@ -16,581 +16,578 @@
     * main
 built_with_pdoc[pdoc_logo]
 
 ****** hassle.new_project ******
 ⁰ View Source
 __1import argparse
 __2import os
-__3import shutil
-__4import sys
-__5from datetime import datetime
-__6from pathlib import Path
-__7
-__8import requests
-__9import tomlkit
-_10from bs4 import BeautifulSoup
-_11
-_12import hassle.hassle_config as hassle_config
-_13from hassle.generate_tests import generate_test_files
+__3import sys
+__4from datetime import datetime
+__5
+__6import requests
+__7from bs4 import BeautifulSoup
+__8from pathier import Pathier
+__9
+_10import hassle.hassle_config as hassle_config
+_11from hassle.generate_tests import generate_test_files
+_12
+_13root = Pathier(__file__).parent
 _14
-_15root = Path(__file__).parent
-_16
-_17
-_18def get_args() -> argparse.Namespace:
-_19    parser = argparse.ArgumentParser()
-_20
-_21    parser.add_argument(
-_22        "name",
-_23        type=str,
-_24        help=""" Name of the package to create in the current working
+_15
+_16def get_args() -> argparse.Namespace:
+_17    parser = argparse.ArgumentParser()
+_18
+_19    parser.add_argument(
+_20        "name",
+_21        type=str,
+_22        help=""" Name of the package to create in the current working
 directory. """,
-_25    )
-_26
-_27    parser.add_argument(
-_28        "-s",
-_29        "--source_files",
-_30        nargs="*",
-_31        type=str,
-_32        default=[],
-_33        help=""" List of additional source files to create in addition to
+_23    )
+_24
+_25    parser.add_argument(
+_26        "-s",
+_27        "--source_files",
+_28        nargs="*",
+_29        type=str,
+_30        default=[],
+_31        help=""" List of additional source files to create in addition to
 the default
-_34        __init__.py and {name}.py files.""",
-_35    )
-_36
-_37    parser.add_argument(
-_38        "-d",
-_39        "--description",
-_40        type=str,
-_41        default="",
-_42        help=""" The package description to be added to the pyproject.toml
+_32        __init__.py and {name}.py files.""",
+_33    )
+_34
+_35    parser.add_argument(
+_36        "-d",
+_37        "--description",
+_38        type=str,
+_39        default="",
+_40        help=""" The package description to be added to the pyproject.toml
 file. """,
-_43    )
-_44
-_45    parser.add_argument(
-_46        "-dp",
-_47        "--dependencies",
-_48        nargs="*",
-_49        type=str,
-_50        default=[],
-_51        help=""" List of dependencies to add to pyproject.toml.
-_52        Note: hassle.py will automatically scan your project for 3rd party
-_53        imports and update pyproject.toml. This switch is largely useful
-_54        for adding dependencies your project might need, but doesn't
-_55        directly import in any source files,
-_56        like an os.system() call that invokes a 3rd party cli.""",
-_57    )
-_58
-_59    parser.add_argument(
-_60        "-k",
-_61        "--keywords",
-_62        nargs="*",
-_63        type=str,
-_64        default=[],
-_65        help=""" List of keywords to be added to the keywords field in
+_41    )
+_42
+_43    parser.add_argument(
+_44        "-dp",
+_45        "--dependencies",
+_46        nargs="*",
+_47        type=str,
+_48        default=[],
+_49        help=""" List of dependencies to add to pyproject.toml.
+_50        Note: hassle.py will automatically scan your project for 3rd party
+_51        imports and update pyproject.toml. This switch is largely useful
+_52        for adding dependencies your project might need, but doesn't
+_53        directly import in any source files,
+_54        like an os.system() call that invokes a 3rd party cli.""",
+_55    )
+_56
+_57    parser.add_argument(
+_58        "-k",
+_59        "--keywords",
+_60        nargs="*",
+_61        type=str,
+_62        default=[],
+_63        help=""" List of keywords to be added to the keywords field in
 pyproject.toml. """,
-_66    )
-_67
-_68    parser.add_argument(
-_69        "-as",
-_70        "--add_script",
-_71        action="store_true",
-_72        help=""" Add section to pyproject.toml declaring the package
-_73        should be installed with command line scripts added.
-_74        The default is '{name} = "{name}.{name}:main".
-_75        You will need to manually change this field.""",
-_76    )
-_77
-_78    parser.add_argument(
-_79        "-nl",
-_80        "--no_license",
-_81        action="store_true",
-_82        help=""" By default, projects are created with an MIT license.
-_83        Set this flag to avoid adding a license if you want to configure
+_64    )
+_65
+_66    parser.add_argument(
+_67        "-as",
+_68        "--add_script",
+_69        action="store_true",
+_70        help=""" Add section to pyproject.toml declaring the package
+_71        should be installed with command line scripts added.
+_72        The default is '{name} = "{name}.{name}:main".
+_73        You will need to manually change this field.""",
+_74    )
+_75
+_76    parser.add_argument(
+_77        "-nl",
+_78        "--no_license",
+_79        action="store_true",
+_80        help=""" By default, projects are created with an MIT license.
+_81        Set this flag to avoid adding a license if you want to configure
 licensing
-_84        at another time.""",
-_85    )
-_86
-_87    parser.add_argument(
-_88        "-os",
-_89        "--operating_system",
-_90        type=str,
-_91        default=None,
-_92        nargs="*",
-_93        help=""" List of operating systems this package will be compatible
+_82        at another time.""",
+_83    )
+_84
+_85    parser.add_argument(
+_86        "-os",
+_87        "--operating_system",
+_88        type=str,
+_89        default=None,
+_90        nargs="*",
+_91        help=""" List of operating systems this package will be compatible
 with.
-_94        The default is OS Independent.
-_95        This only affects the 'classifiers' field of pyproject.toml .""",
-_96    )
-_97
-_98    parser.add_argument(
-_99        "-np",
-100        "--not_package",
-101        action="store_true",
-102        help=""" Put source files in top level directory and delete tests
+_92        The default is OS Independent.
+_93        This only affects the 'classifiers' field of pyproject.toml .""",
+_94    )
+_95
+_96    parser.add_argument(
+_97        "-np",
+_98        "--not_package",
+_99        action="store_true",
+100        help=""" Put source files in top level directory and delete tests
 folder. """,
-103    )
-104
-105    args = parser.parse_args()
-106    args.source_files.extend(["__init__.py", f"{args.name}.py"])
+101    )
+102
+103    args = parser.parse_args()
+104    args.source_files.extend(["__init__.py", f"{args.name}.py"])
+105
+106    return args
 107
-108    return args
-109
-110
-111def get_answer(question: str) -> bool:
-112    """Repeatedly ask the user a yes/no question
-113    until a 'y' or a 'n' is received."""
-114    ans = ""
-115    question = question.strip()
-116    if "?" not in question:
-117        question += "?"
-118    question += " (y/n): "
-119    while ans not in ["y", "yes", "no", "n"]:
-120        ans = input(question).strip().lower()
-121        if ans in ["y", "yes"]:
-122            return True
-123        elif ans in ["n", "no"]:
-124            return False
-125        else:
-126            print("Invalid answer.")
-127
-128
-129def check_pypi_for_name(package_name: str) -> bool:
-130    """Check if a package with package_name
-131    already exists on pypi.org .
-132    Returns True if package name exists.
-133    Only checks the first page of results."""
-134    url = f"https://pypi.org/search/?q={package_name.lower()}"
-135    response = requests.get(url)
-136    if response.status_code != 200:
-137        raise RuntimeError(
-138            f"Error: pypi.org returned status code: {response.status_code}"
-139        )
-140    soup = BeautifulSoup(response.text, "html.parser")
-141    pypi_packages = [
-142        span.text.lower()
-143        for span in soup.find_all("span", class_="package-snippet__name")
-144    ]
-145    return package_name in pypi_packages
-146
-147
-148def check_pypi_for_name_cli():
-149    parser = argparse.ArgumentParser()
-150    parser.add_argument("name", type=str)
-151    args = parser.parse_args()
-152    if check_pypi_for_name(args.name):
-153        print(f"{args.name} is already taken.")
-154    else:
-155        print(f"{args.name} is available.")
-156
-157
-158def create_pyproject_file(targetdir: Path, args: argparse.Namespace):
-159    """Create pyproject.toml in ./{project_name} from args,
-160    pyproject_template, and hassle_config."""
-161    pyproject = tomlkit.loads((root / "pyproject_template.toml").read_text
-())
-162    if not hassle_config.config_exists():
-163        hassle_config.warn()
-164        if not get_answer("Continue creating new package with blank
+108
+109def get_answer(question: str) -> bool:
+110    """Repeatedly ask the user a yes/no question
+111    until a 'y' or a 'n' is received."""
+112    ans = ""
+113    question = question.strip()
+114    if "?" not in question:
+115        question += "?"
+116    question += " (y/n): "
+117    while ans not in ["y", "yes", "no", "n"]:
+118        ans = input(question).strip().lower()
+119        if ans in ["y", "yes"]:
+120            return True
+121        elif ans in ["n", "no"]:
+122            return False
+123        else:
+124            print("Invalid answer.")
+125
+126
+127def check_pypi_for_name(package_name: str) -> bool:
+128    """Check if a package with package_name
+129    already exists on pypi.org .
+130    Returns True if package name exists.
+131    Only checks the first page of results."""
+132    url = f"https://pypi.org/search/?q={package_name.lower()}"
+133    response = requests.get(url)
+134    if response.status_code != 200:
+135        raise RuntimeError(
+136            f"Error: pypi.org returned status code: {response.status_code}"
+137        )
+138    soup = BeautifulSoup(response.text, "html.parser")
+139    pypi_packages = [
+140        span.text.lower()
+141        for span in soup.find_all("span", class_="package-snippet__name")
+142    ]
+143    return package_name in pypi_packages
+144
+145
+146def check_pypi_for_name_cli():
+147    parser = argparse.ArgumentParser()
+148    parser.add_argument("name", type=str)
+149    args = parser.parse_args()
+150    if check_pypi_for_name(args.name):
+151        print(f"{args.name} is already taken.")
+152    else:
+153        print(f"{args.name} is available.")
+154
+155
+156def create_pyproject_file(targetdir: Pathier, args: argparse.Namespace):
+157    """Create pyproject.toml in ./{project_name} from args,
+158    pyproject_template, and hassle_config."""
+159    pyproject = (root / "pyproject_template.toml").loads()
+160    if not hassle_config.config_exists():
+161        hassle_config.warn()
+162        if not get_answer("Continue creating new package with blank
 config?"):
-165            raise Exception("Aborting new package creation")
-166        else:
-167            print("Creating blank hassle_config.toml...")
-168            hassle_config.create_config()
-169    config = hassle_config.load_config()
-170    pyproject["project"]["name"] = args.name
-171    pyproject["project"]["authors"] = config["authors"]
-172    pyproject["project"]["description"] = args.description
-173    pyproject["project"]["dependencies"] = args.dependencies
-174    pyproject["project"]["keywords"] = args.keywords
-175    if args.operating_system:
-176        pyproject["project"]["classifiers"][2] = "Operating System :: " + "
+163            raise Exception("Aborting new package creation")
+164        else:
+165            print("Creating blank hassle_config.toml...")
+166            hassle_config.create_config()
+167    config = hassle_config.load_config()
+168    pyproject["project"]["name"] = args.name
+169    pyproject["project"]["authors"] = config["authors"]
+170    pyproject["project"]["description"] = args.description
+171    pyproject["project"]["dependencies"] = args.dependencies
+172    pyproject["project"]["keywords"] = args.keywords
+173    if args.operating_system:
+174        pyproject["project"]["classifiers"][2] = "Operating System :: " + "
 ".join(
-177            args.operating_system
-178        )
-179    if args.no_license:
-180        pyproject["project"]["classifiers"].pop(1)
-181    for field in config["project_urls"]:
-182        pyproject["project"]["urls"][field] = config["project_urls"]
+175            args.operating_system
+176        )
+177    if args.no_license:
+178        pyproject["project"]["classifiers"].pop(1)
+179    for field in config["project_urls"]:
+180        pyproject["project"]["urls"][field] = config["project_urls"]
 [field].replace(
-183            "$name", args.name
-184        )
-185    if args.add_script:
-186        pyproject["project"]["scripts"][args.name] = f"{args.name}.
+181            "$name", args.name
+182        )
+183    if args.add_script:
+184        pyproject["project"]["scripts"][args.name] = f"{args.name}.
 {args.name}:main"
-187    (targetdir / "pyproject.toml").write_text(tomlkit.dumps(pyproject))
-188
-189
-190def create_source_files(srcdir: Path, filelist: list[str]):
-191    """Generate empty source files in ./{package_name}/src/{package_name}/
+185    (targetdir / "pyproject.toml").dumps(pyproject)
+186
+187
+188def create_source_files(srcdir: Pathier, filelist: list[str]):
+189    """Generate empty source files in ./{package_name}/src/{package_name}/
 """
-192    srcdir.mkdir(parents=True, exist_ok=True)
-193    for file in filelist:
-194        (srcdir / file).touch()
-195
-196
-197def create_readme(targetdir: Path, args: argparse.Namespace):
-198    """Create README.md in ./{package_name}
-199    from readme_template and args."""
-200    readme = (root / "README_template.md").read_text()
-201    readme = readme.replace("$name", args.name).replace(
-202        "$description", args.description
-203    )
-204    (targetdir / "README.md").write_text(readme)
-205
-206
-207def create_license(targetdir: Path):
-208    """Add MIT license file to ./{package_name} ."""
-209    license_template = (root / "license_template.txt").read_text()
-210    license_template = license_template.replace("$year", str(datetime.now
+190    srcdir.mkdir(parents=True, exist_ok=True)
+191    for file in filelist:
+192        (srcdir / file).touch()
+193
+194
+195def create_readme(targetdir: Pathier, args: argparse.Namespace):
+196    """Create README.md in ./{package_name}
+197    from readme_template and args."""
+198    readme = (root / "README_template.md").read_text()
+199    readme = readme.replace("$name", args.name).replace(
+200        "$description", args.description
+201    )
+202    (targetdir / "README.md").write_text(readme)
+203
+204
+205def create_license(targetdir: Pathier):
+206    """Add MIT license file to ./{package_name} ."""
+207    license_template = (root / "license_template.txt").read_text()
+208    license_template = license_template.replace("$year", str(datetime.now
 ().year))
-211    (targetdir / "LICENSE.txt").write_text(license_template)
-212
-213
-214def create_gitignore(targetdir: Path):
-215    """Add .gitignore to ./{package_name}"""
-216    shutil.copy(root / ".gitignore_template", targetdir / ".gitignore")
-217
-218
-219def create_vscode_settings(targetdir: Path):
-220    """Add settings.json to ./.vscode"""
-221    vsdir = targetdir / ".vscode"
-222    vsdir.mkdir(parents=True, exist_ok=True)
-223    shutil.copy(root / ".vscode_template", vsdir / "settings.json")
-224
-225
-226def main(args: argparse.Namespace = None):
-227    if not args:
-228        args = get_args()
-229    if not args.not_package:
-230        try:
-231            if check_pypi_for_name(args.name):
-232                print(f"{args.name} already exists on pypi.org")
-233                if not get_answer("Continue anyway?"):
-234                    sys.exit(0)
-235        except Exception as e:
-236            print(e)
-237            print(
-238                f"Couldn't verify that {args.name} doesn't already exist on
+209    (targetdir / "LICENSE.txt").write_text(license_template)
+210
+211
+212def create_gitignore(targetdir: Pathier):
+213    """Add .gitignore to ./{package_name}"""
+214    (root / ".gitignore_template").copy(targetdir / ".gitignore", True)
+215
+216
+217def create_vscode_settings(targetdir: Pathier):
+218    """Add settings.json to ./.vscode"""
+219    vsdir = targetdir / ".vscode"
+220    vsdir.mkdir(parents=True, exist_ok=True)
+221    (root / ".vscode_template").copy(vsdir / "settings.json", True)
+222
+223
+224def main(args: argparse.Namespace = None):
+225    if not args:
+226        args = get_args()
+227    if not args.not_package:
+228        try:
+229            if check_pypi_for_name(args.name):
+230                print(f"{args.name} already exists on pypi.org")
+231                if not get_answer("Continue anyway?"):
+232                    sys.exit(0)
+233        except Exception as e:
+234            print(e)
+235            print(
+236                f"Couldn't verify that {args.name} doesn't already exist on
 pypi.org ."
-239            )
-240            if not get_answer("Continue anyway?"):
-241                sys.exit(0)
-242    try:
-243        targetdir = Path.cwd() / args.name
-244        try:
-245            targetdir.mkdir(parents=True, exist_ok=False)
-246        except:
-247            print(f"{targetdir} already exists.")
-248            if not get_answer("Overwrite?"):
-249                sys.exit(0)
-250        if not args.not_package:
-251            create_pyproject_file(targetdir, args)
-252        create_source_files(
-253            targetdir if args.not_package else (targetdir / "src" /
+237            )
+238            if not get_answer("Continue anyway?"):
+239                sys.exit(0)
+240    try:
+241        targetdir: Pathier = Pathier.cwd() / args.name
+242        try:
+243            targetdir.mkdir(parents=True, exist_ok=False)
+244        except:
+245            print(f"{targetdir} already exists.")
+246            if not get_answer("Overwrite?"):
+247                sys.exit(0)
+248        if not args.not_package:
+249            create_pyproject_file(targetdir, args)
+250        create_source_files(
+251            targetdir if args.not_package else (targetdir / "src" /
 args.name),
-254            args.source_files[1:] if args.not_package else
+252            args.source_files[1:] if args.not_package else
 args.source_files,
-255        )
-256        create_readme(targetdir, args)
-257        if not args.not_package:
-258            generate_test_files(targetdir)
-259            create_vscode_settings(targetdir)
-260        create_gitignore(targetdir)
-261        if not args.no_license:
-262            create_license(targetdir)
-263        os.chdir(targetdir)
-264        os.system("git init -b main")
-265
-266    except Exception as e:
-267        if not "Aborting new package creation" in str(e):
-268            print(e)
-269        if get_answer("Delete created files?"):
-270            shutil.rmtree(targetdir)
-271
-272
-273if __name__ == "__main__":
-274    main(get_args())
+253        )
+254        create_readme(targetdir, args)
+255        if not args.not_package:
+256            generate_test_files(targetdir)
+257            create_vscode_settings(targetdir)
+258        create_gitignore(targetdir)
+259        if not args.no_license:
+260            create_license(targetdir)
+261        os.chdir(targetdir)
+262        os.system("git init -b main")
+263
+264    except Exception as e:
+265        if not "Aborting new package creation" in str(e):
+266            print(e)
+267        if get_answer("Delete created files?"):
+268            targetdir.delete()
+269
+270
+271if __name__ == "__main__":
+272    main(get_args())
   ⁰
 def get_args() -> argparse.Namespace: View Source
-_19def get_args() -> argparse.Namespace:
-_20    parser = argparse.ArgumentParser()
-_21
-_22    parser.add_argument(
-_23        "name",
-_24        type=str,
-_25        help=""" Name of the package to create in the current working
+_17def get_args() -> argparse.Namespace:
+_18    parser = argparse.ArgumentParser()
+_19
+_20    parser.add_argument(
+_21        "name",
+_22        type=str,
+_23        help=""" Name of the package to create in the current working
 directory. """,
-_26    )
-_27
-_28    parser.add_argument(
-_29        "-s",
-_30        "--source_files",
-_31        nargs="*",
-_32        type=str,
-_33        default=[],
-_34        help=""" List of additional source files to create in addition to
+_24    )
+_25
+_26    parser.add_argument(
+_27        "-s",
+_28        "--source_files",
+_29        nargs="*",
+_30        type=str,
+_31        default=[],
+_32        help=""" List of additional source files to create in addition to
 the default
-_35        __init__.py and {name}.py files.""",
-_36    )
-_37
-_38    parser.add_argument(
-_39        "-d",
-_40        "--description",
-_41        type=str,
-_42        default="",
-_43        help=""" The package description to be added to the pyproject.toml
+_33        __init__.py and {name}.py files.""",
+_34    )
+_35
+_36    parser.add_argument(
+_37        "-d",
+_38        "--description",
+_39        type=str,
+_40        default="",
+_41        help=""" The package description to be added to the pyproject.toml
 file. """,
-_44    )
-_45
-_46    parser.add_argument(
-_47        "-dp",
-_48        "--dependencies",
-_49        nargs="*",
-_50        type=str,
-_51        default=[],
-_52        help=""" List of dependencies to add to pyproject.toml.
-_53        Note: hassle.py will automatically scan your project for 3rd party
-_54        imports and update pyproject.toml. This switch is largely useful
-_55        for adding dependencies your project might need, but doesn't
-_56        directly import in any source files,
-_57        like an os.system() call that invokes a 3rd party cli.""",
-_58    )
-_59
-_60    parser.add_argument(
-_61        "-k",
-_62        "--keywords",
-_63        nargs="*",
-_64        type=str,
-_65        default=[],
-_66        help=""" List of keywords to be added to the keywords field in
+_42    )
+_43
+_44    parser.add_argument(
+_45        "-dp",
+_46        "--dependencies",
+_47        nargs="*",
+_48        type=str,
+_49        default=[],
+_50        help=""" List of dependencies to add to pyproject.toml.
+_51        Note: hassle.py will automatically scan your project for 3rd party
+_52        imports and update pyproject.toml. This switch is largely useful
+_53        for adding dependencies your project might need, but doesn't
+_54        directly import in any source files,
+_55        like an os.system() call that invokes a 3rd party cli.""",
+_56    )
+_57
+_58    parser.add_argument(
+_59        "-k",
+_60        "--keywords",
+_61        nargs="*",
+_62        type=str,
+_63        default=[],
+_64        help=""" List of keywords to be added to the keywords field in
 pyproject.toml. """,
-_67    )
-_68
-_69    parser.add_argument(
-_70        "-as",
-_71        "--add_script",
-_72        action="store_true",
-_73        help=""" Add section to pyproject.toml declaring the package
-_74        should be installed with command line scripts added.
-_75        The default is '{name} = "{name}.{name}:main".
-_76        You will need to manually change this field.""",
-_77    )
-_78
-_79    parser.add_argument(
-_80        "-nl",
-_81        "--no_license",
-_82        action="store_true",
-_83        help=""" By default, projects are created with an MIT license.
-_84        Set this flag to avoid adding a license if you want to configure
+_65    )
+_66
+_67    parser.add_argument(
+_68        "-as",
+_69        "--add_script",
+_70        action="store_true",
+_71        help=""" Add section to pyproject.toml declaring the package
+_72        should be installed with command line scripts added.
+_73        The default is '{name} = "{name}.{name}:main".
+_74        You will need to manually change this field.""",
+_75    )
+_76
+_77    parser.add_argument(
+_78        "-nl",
+_79        "--no_license",
+_80        action="store_true",
+_81        help=""" By default, projects are created with an MIT license.
+_82        Set this flag to avoid adding a license if you want to configure
 licensing
-_85        at another time.""",
-_86    )
-_87
-_88    parser.add_argument(
-_89        "-os",
-_90        "--operating_system",
-_91        type=str,
-_92        default=None,
-_93        nargs="*",
-_94        help=""" List of operating systems this package will be compatible
+_83        at another time.""",
+_84    )
+_85
+_86    parser.add_argument(
+_87        "-os",
+_88        "--operating_system",
+_89        type=str,
+_90        default=None,
+_91        nargs="*",
+_92        help=""" List of operating systems this package will be compatible
 with.
-_95        The default is OS Independent.
-_96        This only affects the 'classifiers' field of pyproject.toml .""",
-_97    )
-_98
-_99    parser.add_argument(
-100        "-np",
-101        "--not_package",
-102        action="store_true",
-103        help=""" Put source files in top level directory and delete tests
+_93        The default is OS Independent.
+_94        This only affects the 'classifiers' field of pyproject.toml .""",
+_95    )
+_96
+_97    parser.add_argument(
+_98        "-np",
+_99        "--not_package",
+100        action="store_true",
+101        help=""" Put source files in top level directory and delete tests
 folder. """,
-104    )
-105
-106    args = parser.parse_args()
-107    args.source_files.extend(["__init__.py", f"{args.name}.py"])
-108
-109    return args
+102    )
+103
+104    args = parser.parse_args()
+105    args.source_files.extend(["__init__.py", f"{args.name}.py"])
+106
+107    return args
   ⁰
 def get_answer(question: str) -> bool: View Source
-112def get_answer(question: str) -> bool:
-113    """Repeatedly ask the user a yes/no question
-114    until a 'y' or a 'n' is received."""
-115    ans = ""
-116    question = question.strip()
-117    if "?" not in question:
-118        question += "?"
-119    question += " (y/n): "
-120    while ans not in ["y", "yes", "no", "n"]:
-121        ans = input(question).strip().lower()
-122        if ans in ["y", "yes"]:
-123            return True
-124        elif ans in ["n", "no"]:
-125            return False
-126        else:
-127            print("Invalid answer.")
+110def get_answer(question: str) -> bool:
+111    """Repeatedly ask the user a yes/no question
+112    until a 'y' or a 'n' is received."""
+113    ans = ""
+114    question = question.strip()
+115    if "?" not in question:
+116        question += "?"
+117    question += " (y/n): "
+118    while ans not in ["y", "yes", "no", "n"]:
+119        ans = input(question).strip().lower()
+120        if ans in ["y", "yes"]:
+121            return True
+122        elif ans in ["n", "no"]:
+123            return False
+124        else:
+125            print("Invalid answer.")
 Repeatedly ask the user a yes/no question until a 'y' or a 'n' is received.
   ⁰
 def check_pypi_for_name(package_name: str) -> bool: View Source
-130def check_pypi_for_name(package_name: str) -> bool:
-131    """Check if a package with package_name
-132    already exists on pypi.org .
-133    Returns True if package name exists.
-134    Only checks the first page of results."""
-135    url = f"https://pypi.org/search/?q={package_name.lower()}"
-136    response = requests.get(url)
-137    if response.status_code != 200:
-138        raise RuntimeError(
-139            f"Error: pypi.org returned status code: {response.status_code}"
-140        )
-141    soup = BeautifulSoup(response.text, "html.parser")
-142    pypi_packages = [
-143        span.text.lower()
-144        for span in soup.find_all("span", class_="package-snippet__name")
-145    ]
-146    return package_name in pypi_packages
+128def check_pypi_for_name(package_name: str) -> bool:
+129    """Check if a package with package_name
+130    already exists on pypi.org .
+131    Returns True if package name exists.
+132    Only checks the first page of results."""
+133    url = f"https://pypi.org/search/?q={package_name.lower()}"
+134    response = requests.get(url)
+135    if response.status_code != 200:
+136        raise RuntimeError(
+137            f"Error: pypi.org returned status code: {response.status_code}"
+138        )
+139    soup = BeautifulSoup(response.text, "html.parser")
+140    pypi_packages = [
+141        span.text.lower()
+142        for span in soup.find_all("span", class_="package-snippet__name")
+143    ]
+144    return package_name in pypi_packages
 Check if a package with package_name already exists on pypi.org . Returns True
 if package name exists. Only checks the first page of results.
   ⁰
 def check_pypi_for_name_cli(): View Source
-149def check_pypi_for_name_cli():
-150    parser = argparse.ArgumentParser()
-151    parser.add_argument("name", type=str)
-152    args = parser.parse_args()
-153    if check_pypi_for_name(args.name):
-154        print(f"{args.name} is already taken.")
-155    else:
-156        print(f"{args.name} is available.")
-  ⁰
-def create_pyproject_file(targetdir: pathlib.Path, args: argparse.Namespace):
-View Source
-159def create_pyproject_file(targetdir: Path, args: argparse.Namespace):
-160    """Create pyproject.toml in ./{project_name} from args,
-161    pyproject_template, and hassle_config."""
-162    pyproject = tomlkit.loads((root / "pyproject_template.toml").read_text
-())
-163    if not hassle_config.config_exists():
-164        hassle_config.warn()
-165        if not get_answer("Continue creating new package with blank
+147def check_pypi_for_name_cli():
+148    parser = argparse.ArgumentParser()
+149    parser.add_argument("name", type=str)
+150    args = parser.parse_args()
+151    if check_pypi_for_name(args.name):
+152        print(f"{args.name} is already taken.")
+153    else:
+154        print(f"{args.name} is available.")
+  ⁰
+def create_pyproject_file(targetdir: pathier.pathier.Pathier, args:
+argparse.Namespace): View Source
+157def create_pyproject_file(targetdir: Pathier, args: argparse.Namespace):
+158    """Create pyproject.toml in ./{project_name} from args,
+159    pyproject_template, and hassle_config."""
+160    pyproject = (root / "pyproject_template.toml").loads()
+161    if not hassle_config.config_exists():
+162        hassle_config.warn()
+163        if not get_answer("Continue creating new package with blank
 config?"):
-166            raise Exception("Aborting new package creation")
-167        else:
-168            print("Creating blank hassle_config.toml...")
-169            hassle_config.create_config()
-170    config = hassle_config.load_config()
-171    pyproject["project"]["name"] = args.name
-172    pyproject["project"]["authors"] = config["authors"]
-173    pyproject["project"]["description"] = args.description
-174    pyproject["project"]["dependencies"] = args.dependencies
-175    pyproject["project"]["keywords"] = args.keywords
-176    if args.operating_system:
-177        pyproject["project"]["classifiers"][2] = "Operating System :: " + "
+164            raise Exception("Aborting new package creation")
+165        else:
+166            print("Creating blank hassle_config.toml...")
+167            hassle_config.create_config()
+168    config = hassle_config.load_config()
+169    pyproject["project"]["name"] = args.name
+170    pyproject["project"]["authors"] = config["authors"]
+171    pyproject["project"]["description"] = args.description
+172    pyproject["project"]["dependencies"] = args.dependencies
+173    pyproject["project"]["keywords"] = args.keywords
+174    if args.operating_system:
+175        pyproject["project"]["classifiers"][2] = "Operating System :: " + "
 ".join(
-178            args.operating_system
-179        )
-180    if args.no_license:
-181        pyproject["project"]["classifiers"].pop(1)
-182    for field in config["project_urls"]:
-183        pyproject["project"]["urls"][field] = config["project_urls"]
+176            args.operating_system
+177        )
+178    if args.no_license:
+179        pyproject["project"]["classifiers"].pop(1)
+180    for field in config["project_urls"]:
+181        pyproject["project"]["urls"][field] = config["project_urls"]
 [field].replace(
-184            "$name", args.name
-185        )
-186    if args.add_script:
-187        pyproject["project"]["scripts"][args.name] = f"{args.name}.
+182            "$name", args.name
+183        )
+184    if args.add_script:
+185        pyproject["project"]["scripts"][args.name] = f"{args.name}.
 {args.name}:main"
-188    (targetdir / "pyproject.toml").write_text(tomlkit.dumps(pyproject))
+186    (targetdir / "pyproject.toml").dumps(pyproject)
 Create pyproject.toml in ./{project_name} from args, pyproject_template, and
 hassle_config.
   ⁰
-def create_source_files(srcdir: pathlib.Path, filelist: list[str]): View Source
-191def create_source_files(srcdir: Path, filelist: list[str]):
-192    """Generate empty source files in ./{package_name}/src/{package_name}/
+def create_source_files(srcdir: pathier.pathier.Pathier, filelist: list[str]):
+View Source
+189def create_source_files(srcdir: Pathier, filelist: list[str]):
+190    """Generate empty source files in ./{package_name}/src/{package_name}/
 """
-193    srcdir.mkdir(parents=True, exist_ok=True)
-194    for file in filelist:
-195        (srcdir / file).touch()
+191    srcdir.mkdir(parents=True, exist_ok=True)
+192    for file in filelist:
+193        (srcdir / file).touch()
 Generate empty source files in ./{package_name}/src/{package_name}/
   ⁰
-def create_readme(targetdir: pathlib.Path, args: argparse.Namespace): View
-Source
-198def create_readme(targetdir: Path, args: argparse.Namespace):
-199    """Create README.md in ./{package_name}
-200    from readme_template and args."""
-201    readme = (root / "README_template.md").read_text()
-202    readme = readme.replace("$name", args.name).replace(
-203        "$description", args.description
-204    )
-205    (targetdir / "README.md").write_text(readme)
+def create_readme(targetdir: pathier.pathier.Pathier, args:
+argparse.Namespace): View Source
+196def create_readme(targetdir: Pathier, args: argparse.Namespace):
+197    """Create README.md in ./{package_name}
+198    from readme_template and args."""
+199    readme = (root / "README_template.md").read_text()
+200    readme = readme.replace("$name", args.name).replace(
+201        "$description", args.description
+202    )
+203    (targetdir / "README.md").write_text(readme)
 Create README.md in ./{package_name} from readme_template and args.
   ⁰
-def create_license(targetdir: pathlib.Path): View Source
-208def create_license(targetdir: Path):
-209    """Add MIT license file to ./{package_name} ."""
-210    license_template = (root / "license_template.txt").read_text()
-211    license_template = license_template.replace("$year", str(datetime.now
+def create_license(targetdir: pathier.pathier.Pathier): View Source
+206def create_license(targetdir: Pathier):
+207    """Add MIT license file to ./{package_name} ."""
+208    license_template = (root / "license_template.txt").read_text()
+209    license_template = license_template.replace("$year", str(datetime.now
 ().year))
-212    (targetdir / "LICENSE.txt").write_text(license_template)
+210    (targetdir / "LICENSE.txt").write_text(license_template)
 Add MIT license file to ./{package_name} .
   ⁰
-def create_gitignore(targetdir: pathlib.Path): View Source
-215def create_gitignore(targetdir: Path):
-216    """Add .gitignore to ./{package_name}"""
-217    shutil.copy(root / ".gitignore_template", targetdir / ".gitignore")
+def create_gitignore(targetdir: pathier.pathier.Pathier): View Source
+213def create_gitignore(targetdir: Pathier):
+214    """Add .gitignore to ./{package_name}"""
+215    (root / ".gitignore_template").copy(targetdir / ".gitignore", True)
 Add .gitignore to ./{package_name}
   ⁰
-def create_vscode_settings(targetdir: pathlib.Path): View Source
-220def create_vscode_settings(targetdir: Path):
-221    """Add settings.json to ./.vscode"""
-222    vsdir = targetdir / ".vscode"
-223    vsdir.mkdir(parents=True, exist_ok=True)
-224    shutil.copy(root / ".vscode_template", vsdir / "settings.json")
+def create_vscode_settings(targetdir: pathier.pathier.Pathier): View Source
+218def create_vscode_settings(targetdir: Pathier):
+219    """Add settings.json to ./.vscode"""
+220    vsdir = targetdir / ".vscode"
+221    vsdir.mkdir(parents=True, exist_ok=True)
+222    (root / ".vscode_template").copy(vsdir / "settings.json", True)
 Add settings.json to ./.vscode
   ⁰
 def main(args: argparse.Namespace = None): View Source
-227def main(args: argparse.Namespace = None):
-228    if not args:
-229        args = get_args()
-230    if not args.not_package:
-231        try:
-232            if check_pypi_for_name(args.name):
-233                print(f"{args.name} already exists on pypi.org")
-234                if not get_answer("Continue anyway?"):
-235                    sys.exit(0)
-236        except Exception as e:
-237            print(e)
-238            print(
-239                f"Couldn't verify that {args.name} doesn't already exist on
+225def main(args: argparse.Namespace = None):
+226    if not args:
+227        args = get_args()
+228    if not args.not_package:
+229        try:
+230            if check_pypi_for_name(args.name):
+231                print(f"{args.name} already exists on pypi.org")
+232                if not get_answer("Continue anyway?"):
+233                    sys.exit(0)
+234        except Exception as e:
+235            print(e)
+236            print(
+237                f"Couldn't verify that {args.name} doesn't already exist on
 pypi.org ."
-240            )
-241            if not get_answer("Continue anyway?"):
-242                sys.exit(0)
-243    try:
-244        targetdir = Path.cwd() / args.name
-245        try:
-246            targetdir.mkdir(parents=True, exist_ok=False)
-247        except:
-248            print(f"{targetdir} already exists.")
-249            if not get_answer("Overwrite?"):
-250                sys.exit(0)
-251        if not args.not_package:
-252            create_pyproject_file(targetdir, args)
-253        create_source_files(
-254            targetdir if args.not_package else (targetdir / "src" /
+238            )
+239            if not get_answer("Continue anyway?"):
+240                sys.exit(0)
+241    try:
+242        targetdir: Pathier = Pathier.cwd() / args.name
+243        try:
+244            targetdir.mkdir(parents=True, exist_ok=False)
+245        except:
+246            print(f"{targetdir} already exists.")
+247            if not get_answer("Overwrite?"):
+248                sys.exit(0)
+249        if not args.not_package:
+250            create_pyproject_file(targetdir, args)
+251        create_source_files(
+252            targetdir if args.not_package else (targetdir / "src" /
 args.name),
-255            args.source_files[1:] if args.not_package else
+253            args.source_files[1:] if args.not_package else
 args.source_files,
-256        )
-257        create_readme(targetdir, args)
-258        if not args.not_package:
-259            generate_test_files(targetdir)
-260            create_vscode_settings(targetdir)
-261        create_gitignore(targetdir)
-262        if not args.no_license:
-263            create_license(targetdir)
-264        os.chdir(targetdir)
-265        os.system("git init -b main")
-266
-267    except Exception as e:
-268        if not "Aborting new package creation" in str(e):
-269            print(e)
-270        if get_answer("Delete created files?"):
-271            shutil.rmtree(targetdir)
+254        )
+255        create_readme(targetdir, args)
+256        if not args.not_package:
+257            generate_test_files(targetdir)
+258            create_vscode_settings(targetdir)
+259        create_gitignore(targetdir)
+260        if not args.no_license:
+261            create_license(targetdir)
+262        os.chdir(targetdir)
+263        os.system("git init -b main")
+264
+265    except Exception as e:
+266        if not "Aborting new package creation" in str(e):
+267            print(e)
+268        if get_answer("Delete created files?"):
+269            targetdir.delete()
```

### Comparing `hassle-2.4.0/docs/hassle/run_tests.html` & `hassle-2.5.0/docs/hassle/run_tests.html`

 * *Files 0% similar despite different names*

```diff
@@ -58,55 +58,56 @@
                 
                         <input id="mod-run_tests-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 
                         <label class="view-source-button" for="mod-run_tests-view-source"><span>View Source</span></label>
 
                         <div class="pdoc-code codehilite"><pre><span></span><span id="L-1"><a href="#L-1"><span class="linenos"> 1</span></a><span class="kn">import</span> <span class="nn">argparse</span>
 </span><span id="L-2"><a href="#L-2"><span class="linenos"> 2</span></a><span class="kn">import</span> <span class="nn">os</span>
-</span><span id="L-3"><a href="#L-3"><span class="linenos"> 3</span></a><span class="kn">from</span> <span class="nn">pathlib</span> <span class="kn">import</span> <span class="n">Path</span>
-</span><span id="L-4"><a href="#L-4"><span class="linenos"> 4</span></a>
+</span><span id="L-3"><a href="#L-3"><span class="linenos"> 3</span></a>
+</span><span id="L-4"><a href="#L-4"><span class="linenos"> 4</span></a><span class="kn">from</span> <span class="nn">pathier</span> <span class="kn">import</span> <span class="n">Pathier</span>
 </span><span id="L-5"><a href="#L-5"><span class="linenos"> 5</span></a>
-</span><span id="L-6"><a href="#L-6"><span class="linenos"> 6</span></a><span class="k">def</span> <span class="nf">get_args</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">:</span>
-</span><span id="L-7"><a href="#L-7"><span class="linenos"> 7</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">argparse</span><span class="o">.</span><span class="n">ArgumentParser</span><span class="p">()</span>
-</span><span id="L-8"><a href="#L-8"><span class="linenos"> 8</span></a>
-</span><span id="L-9"><a href="#L-9"><span class="linenos"> 9</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-10"><a href="#L-10"><span class="linenos">10</span></a>        <span class="s2">&quot;package_name&quot;</span><span class="p">,</span>
-</span><span id="L-11"><a href="#L-11"><span class="linenos">11</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
-</span><span id="L-12"><a href="#L-12"><span class="linenos">12</span></a>        <span class="n">default</span><span class="o">=</span><span class="s2">&quot;.&quot;</span><span class="p">,</span>
-</span><span id="L-13"><a href="#L-13"><span class="linenos">13</span></a>        <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;?&quot;</span><span class="p">,</span>
-</span><span id="L-14"><a href="#L-14"><span class="linenos">14</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; The name of the package or project to run tests for,</span>
-</span><span id="L-15"><a href="#L-15"><span class="linenos">15</span></a><span class="s2">        assuming it&#39;s a subfolder of your current working directory.</span>
-</span><span id="L-16"><a href="#L-16"><span class="linenos">16</span></a><span class="s2">        Can also be a full path to the package. If nothing is given,</span>
-</span><span id="L-17"><a href="#L-17"><span class="linenos">17</span></a><span class="s2">        the current working directory will be used.&quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-18"><a href="#L-18"><span class="linenos">18</span></a>    <span class="p">)</span>
-</span><span id="L-19"><a href="#L-19"><span class="linenos">19</span></a>
-</span><span id="L-20"><a href="#L-20"><span class="linenos">20</span></a>    <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="o">.</span><span class="n">parse_args</span><span class="p">()</span>
-</span><span id="L-21"><a href="#L-21"><span class="linenos">21</span></a>
-</span><span id="L-22"><a href="#L-22"><span class="linenos">22</span></a>    <span class="k">return</span> <span class="n">args</span>
-</span><span id="L-23"><a href="#L-23"><span class="linenos">23</span></a>
+</span><span id="L-6"><a href="#L-6"><span class="linenos"> 6</span></a>
+</span><span id="L-7"><a href="#L-7"><span class="linenos"> 7</span></a><span class="k">def</span> <span class="nf">get_args</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">:</span>
+</span><span id="L-8"><a href="#L-8"><span class="linenos"> 8</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">argparse</span><span class="o">.</span><span class="n">ArgumentParser</span><span class="p">()</span>
+</span><span id="L-9"><a href="#L-9"><span class="linenos"> 9</span></a>
+</span><span id="L-10"><a href="#L-10"><span class="linenos">10</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-11"><a href="#L-11"><span class="linenos">11</span></a>        <span class="s2">&quot;package_name&quot;</span><span class="p">,</span>
+</span><span id="L-12"><a href="#L-12"><span class="linenos">12</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
+</span><span id="L-13"><a href="#L-13"><span class="linenos">13</span></a>        <span class="n">default</span><span class="o">=</span><span class="s2">&quot;.&quot;</span><span class="p">,</span>
+</span><span id="L-14"><a href="#L-14"><span class="linenos">14</span></a>        <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;?&quot;</span><span class="p">,</span>
+</span><span id="L-15"><a href="#L-15"><span class="linenos">15</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; The name of the package or project to run tests for,</span>
+</span><span id="L-16"><a href="#L-16"><span class="linenos">16</span></a><span class="s2">        assuming it&#39;s a subfolder of your current working directory.</span>
+</span><span id="L-17"><a href="#L-17"><span class="linenos">17</span></a><span class="s2">        Can also be a full path to the package. If nothing is given,</span>
+</span><span id="L-18"><a href="#L-18"><span class="linenos">18</span></a><span class="s2">        the current working directory will be used.&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-19"><a href="#L-19"><span class="linenos">19</span></a>    <span class="p">)</span>
+</span><span id="L-20"><a href="#L-20"><span class="linenos">20</span></a>
+</span><span id="L-21"><a href="#L-21"><span class="linenos">21</span></a>    <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="o">.</span><span class="n">parse_args</span><span class="p">()</span>
+</span><span id="L-22"><a href="#L-22"><span class="linenos">22</span></a>
+</span><span id="L-23"><a href="#L-23"><span class="linenos">23</span></a>    <span class="k">return</span> <span class="n">args</span>
 </span><span id="L-24"><a href="#L-24"><span class="linenos">24</span></a>
-</span><span id="L-25"><a href="#L-25"><span class="linenos">25</span></a><span class="k">def</span> <span class="nf">run_tests</span><span class="p">(</span><span class="n">package_path</span><span class="p">:</span> <span class="n">Path</span><span class="p">):</span>
-</span><span id="L-26"><a href="#L-26"><span class="linenos">26</span></a>    <span class="sd">&quot;&quot;&quot;Run tests with coverage and pytest.&quot;&quot;&quot;</span>
-</span><span id="L-27"><a href="#L-27"><span class="linenos">27</span></a>    <span class="n">startdir</span> <span class="o">=</span> <span class="n">Path</span><span class="p">()</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span>
-</span><span id="L-28"><a href="#L-28"><span class="linenos">28</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">package_path</span><span class="p">)</span>
-</span><span id="L-29"><a href="#L-29"><span class="linenos">29</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;pip install -e .&quot;</span><span class="p">)</span>
-</span><span id="L-30"><a href="#L-30"><span class="linenos">30</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;coverage run -m pytest -s&quot;</span><span class="p">)</span>
-</span><span id="L-31"><a href="#L-31"><span class="linenos">31</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;coverage report -m&quot;</span><span class="p">)</span>
-</span><span id="L-32"><a href="#L-32"><span class="linenos">32</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">startdir</span><span class="p">)</span>
-</span><span id="L-33"><a href="#L-33"><span class="linenos">33</span></a>
+</span><span id="L-25"><a href="#L-25"><span class="linenos">25</span></a>
+</span><span id="L-26"><a href="#L-26"><span class="linenos">26</span></a><span class="k">def</span> <span class="nf">run_tests</span><span class="p">(</span><span class="n">package_path</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">):</span>
+</span><span id="L-27"><a href="#L-27"><span class="linenos">27</span></a>    <span class="sd">&quot;&quot;&quot;Run tests with coverage and pytest.&quot;&quot;&quot;</span>
+</span><span id="L-28"><a href="#L-28"><span class="linenos">28</span></a>    <span class="n">startdir</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">()</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span>
+</span><span id="L-29"><a href="#L-29"><span class="linenos">29</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">package_path</span><span class="p">)</span>
+</span><span id="L-30"><a href="#L-30"><span class="linenos">30</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;pip install -e .&quot;</span><span class="p">)</span>
+</span><span id="L-31"><a href="#L-31"><span class="linenos">31</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;coverage run -m pytest -s&quot;</span><span class="p">)</span>
+</span><span id="L-32"><a href="#L-32"><span class="linenos">32</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;coverage report -m&quot;</span><span class="p">)</span>
+</span><span id="L-33"><a href="#L-33"><span class="linenos">33</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">startdir</span><span class="p">)</span>
 </span><span id="L-34"><a href="#L-34"><span class="linenos">34</span></a>
-</span><span id="L-35"><a href="#L-35"><span class="linenos">35</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
-</span><span id="L-36"><a href="#L-36"><span class="linenos">36</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="p">:</span>
-</span><span id="L-37"><a href="#L-37"><span class="linenos">37</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
-</span><span id="L-38"><a href="#L-38"><span class="linenos">38</span></a>    <span class="n">package_path</span> <span class="o">=</span> <span class="n">Path</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package_name</span><span class="p">)</span><span class="o">.</span><span class="n">resolve</span><span class="p">()</span>
-</span><span id="L-39"><a href="#L-39"><span class="linenos">39</span></a>    <span class="n">run_tests</span><span class="p">(</span><span class="n">package_path</span><span class="p">)</span>
-</span><span id="L-40"><a href="#L-40"><span class="linenos">40</span></a>
+</span><span id="L-35"><a href="#L-35"><span class="linenos">35</span></a>
+</span><span id="L-36"><a href="#L-36"><span class="linenos">36</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
+</span><span id="L-37"><a href="#L-37"><span class="linenos">37</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="p">:</span>
+</span><span id="L-38"><a href="#L-38"><span class="linenos">38</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
+</span><span id="L-39"><a href="#L-39"><span class="linenos">39</span></a>    <span class="n">package_path</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package_name</span><span class="p">)</span><span class="o">.</span><span class="n">resolve</span><span class="p">()</span>
+</span><span id="L-40"><a href="#L-40"><span class="linenos">40</span></a>    <span class="n">run_tests</span><span class="p">(</span><span class="n">package_path</span><span class="p">)</span>
 </span><span id="L-41"><a href="#L-41"><span class="linenos">41</span></a>
-</span><span id="L-42"><a href="#L-42"><span class="linenos">42</span></a><span class="k">if</span> <span class="vm">__name__</span> <span class="o">==</span> <span class="s2">&quot;__main__&quot;</span><span class="p">:</span>
-</span><span id="L-43"><a href="#L-43"><span class="linenos">43</span></a>    <span class="n">main</span><span class="p">(</span><span class="n">get_args</span><span class="p">())</span>
+</span><span id="L-42"><a href="#L-42"><span class="linenos">42</span></a>
+</span><span id="L-43"><a href="#L-43"><span class="linenos">43</span></a><span class="k">if</span> <span class="vm">__name__</span> <span class="o">==</span> <span class="s2">&quot;__main__&quot;</span><span class="p">:</span>
+</span><span id="L-44"><a href="#L-44"><span class="linenos">44</span></a>    <span class="n">main</span><span class="p">(</span><span class="n">get_args</span><span class="p">())</span>
 </span></pre></div>
 
 
             </section>
                 <section id="get_args">
                             <input id="get_args-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
@@ -114,56 +115,56 @@
         <span class="def">def</span>
         <span class="name">get_args</span><span class="signature pdoc-code condensed">(<span class="return-annotation">) -> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span>:</span></span>
 
                 <label class="view-source-button" for="get_args-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#get_args"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="get_args-7"><a href="#get_args-7"><span class="linenos"> 7</span></a><span class="k">def</span> <span class="nf">get_args</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">:</span>
-</span><span id="get_args-8"><a href="#get_args-8"><span class="linenos"> 8</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">argparse</span><span class="o">.</span><span class="n">ArgumentParser</span><span class="p">()</span>
-</span><span id="get_args-9"><a href="#get_args-9"><span class="linenos"> 9</span></a>
-</span><span id="get_args-10"><a href="#get_args-10"><span class="linenos">10</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="get_args-11"><a href="#get_args-11"><span class="linenos">11</span></a>        <span class="s2">&quot;package_name&quot;</span><span class="p">,</span>
-</span><span id="get_args-12"><a href="#get_args-12"><span class="linenos">12</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
-</span><span id="get_args-13"><a href="#get_args-13"><span class="linenos">13</span></a>        <span class="n">default</span><span class="o">=</span><span class="s2">&quot;.&quot;</span><span class="p">,</span>
-</span><span id="get_args-14"><a href="#get_args-14"><span class="linenos">14</span></a>        <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;?&quot;</span><span class="p">,</span>
-</span><span id="get_args-15"><a href="#get_args-15"><span class="linenos">15</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; The name of the package or project to run tests for,</span>
-</span><span id="get_args-16"><a href="#get_args-16"><span class="linenos">16</span></a><span class="s2">        assuming it&#39;s a subfolder of your current working directory.</span>
-</span><span id="get_args-17"><a href="#get_args-17"><span class="linenos">17</span></a><span class="s2">        Can also be a full path to the package. If nothing is given,</span>
-</span><span id="get_args-18"><a href="#get_args-18"><span class="linenos">18</span></a><span class="s2">        the current working directory will be used.&quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="get_args-19"><a href="#get_args-19"><span class="linenos">19</span></a>    <span class="p">)</span>
-</span><span id="get_args-20"><a href="#get_args-20"><span class="linenos">20</span></a>
-</span><span id="get_args-21"><a href="#get_args-21"><span class="linenos">21</span></a>    <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="o">.</span><span class="n">parse_args</span><span class="p">()</span>
-</span><span id="get_args-22"><a href="#get_args-22"><span class="linenos">22</span></a>
-</span><span id="get_args-23"><a href="#get_args-23"><span class="linenos">23</span></a>    <span class="k">return</span> <span class="n">args</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="get_args-8"><a href="#get_args-8"><span class="linenos"> 8</span></a><span class="k">def</span> <span class="nf">get_args</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">:</span>
+</span><span id="get_args-9"><a href="#get_args-9"><span class="linenos"> 9</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">argparse</span><span class="o">.</span><span class="n">ArgumentParser</span><span class="p">()</span>
+</span><span id="get_args-10"><a href="#get_args-10"><span class="linenos">10</span></a>
+</span><span id="get_args-11"><a href="#get_args-11"><span class="linenos">11</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="get_args-12"><a href="#get_args-12"><span class="linenos">12</span></a>        <span class="s2">&quot;package_name&quot;</span><span class="p">,</span>
+</span><span id="get_args-13"><a href="#get_args-13"><span class="linenos">13</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
+</span><span id="get_args-14"><a href="#get_args-14"><span class="linenos">14</span></a>        <span class="n">default</span><span class="o">=</span><span class="s2">&quot;.&quot;</span><span class="p">,</span>
+</span><span id="get_args-15"><a href="#get_args-15"><span class="linenos">15</span></a>        <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;?&quot;</span><span class="p">,</span>
+</span><span id="get_args-16"><a href="#get_args-16"><span class="linenos">16</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; The name of the package or project to run tests for,</span>
+</span><span id="get_args-17"><a href="#get_args-17"><span class="linenos">17</span></a><span class="s2">        assuming it&#39;s a subfolder of your current working directory.</span>
+</span><span id="get_args-18"><a href="#get_args-18"><span class="linenos">18</span></a><span class="s2">        Can also be a full path to the package. If nothing is given,</span>
+</span><span id="get_args-19"><a href="#get_args-19"><span class="linenos">19</span></a><span class="s2">        the current working directory will be used.&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="get_args-20"><a href="#get_args-20"><span class="linenos">20</span></a>    <span class="p">)</span>
+</span><span id="get_args-21"><a href="#get_args-21"><span class="linenos">21</span></a>
+</span><span id="get_args-22"><a href="#get_args-22"><span class="linenos">22</span></a>    <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="o">.</span><span class="n">parse_args</span><span class="p">()</span>
+</span><span id="get_args-23"><a href="#get_args-23"><span class="linenos">23</span></a>
+</span><span id="get_args-24"><a href="#get_args-24"><span class="linenos">24</span></a>    <span class="k">return</span> <span class="n">args</span>
 </span></pre></div>
 
 
     
 
                 </section>
                 <section id="run_tests">
                             <input id="run_tests-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="def">def</span>
-        <span class="name">run_tests</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">package_path</span><span class="p">:</span> <span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span></span><span class="return-annotation">):</span></span>
+        <span class="name">run_tests</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">package_path</span><span class="p">:</span> <span class="n">pathier</span><span class="o">.</span><span class="n">pathier</span><span class="o">.</span><span class="n">Pathier</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="run_tests-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#run_tests"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="run_tests-26"><a href="#run_tests-26"><span class="linenos">26</span></a><span class="k">def</span> <span class="nf">run_tests</span><span class="p">(</span><span class="n">package_path</span><span class="p">:</span> <span class="n">Path</span><span class="p">):</span>
-</span><span id="run_tests-27"><a href="#run_tests-27"><span class="linenos">27</span></a>    <span class="sd">&quot;&quot;&quot;Run tests with coverage and pytest.&quot;&quot;&quot;</span>
-</span><span id="run_tests-28"><a href="#run_tests-28"><span class="linenos">28</span></a>    <span class="n">startdir</span> <span class="o">=</span> <span class="n">Path</span><span class="p">()</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span>
-</span><span id="run_tests-29"><a href="#run_tests-29"><span class="linenos">29</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">package_path</span><span class="p">)</span>
-</span><span id="run_tests-30"><a href="#run_tests-30"><span class="linenos">30</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;pip install -e .&quot;</span><span class="p">)</span>
-</span><span id="run_tests-31"><a href="#run_tests-31"><span class="linenos">31</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;coverage run -m pytest -s&quot;</span><span class="p">)</span>
-</span><span id="run_tests-32"><a href="#run_tests-32"><span class="linenos">32</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;coverage report -m&quot;</span><span class="p">)</span>
-</span><span id="run_tests-33"><a href="#run_tests-33"><span class="linenos">33</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">startdir</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="run_tests-27"><a href="#run_tests-27"><span class="linenos">27</span></a><span class="k">def</span> <span class="nf">run_tests</span><span class="p">(</span><span class="n">package_path</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">):</span>
+</span><span id="run_tests-28"><a href="#run_tests-28"><span class="linenos">28</span></a>    <span class="sd">&quot;&quot;&quot;Run tests with coverage and pytest.&quot;&quot;&quot;</span>
+</span><span id="run_tests-29"><a href="#run_tests-29"><span class="linenos">29</span></a>    <span class="n">startdir</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">()</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span>
+</span><span id="run_tests-30"><a href="#run_tests-30"><span class="linenos">30</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">package_path</span><span class="p">)</span>
+</span><span id="run_tests-31"><a href="#run_tests-31"><span class="linenos">31</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;pip install -e .&quot;</span><span class="p">)</span>
+</span><span id="run_tests-32"><a href="#run_tests-32"><span class="linenos">32</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;coverage run -m pytest -s&quot;</span><span class="p">)</span>
+</span><span id="run_tests-33"><a href="#run_tests-33"><span class="linenos">33</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;coverage report -m&quot;</span><span class="p">)</span>
+</span><span id="run_tests-34"><a href="#run_tests-34"><span class="linenos">34</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">startdir</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Run tests with coverage and pytest.</p>
 </div>
 
 
@@ -175,19 +176,19 @@
         <span class="def">def</span>
         <span class="name">main</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">=</span> <span class="kc">None</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="main-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#main"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="main-36"><a href="#main-36"><span class="linenos">36</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
-</span><span id="main-37"><a href="#main-37"><span class="linenos">37</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="p">:</span>
-</span><span id="main-38"><a href="#main-38"><span class="linenos">38</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
-</span><span id="main-39"><a href="#main-39"><span class="linenos">39</span></a>    <span class="n">package_path</span> <span class="o">=</span> <span class="n">Path</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package_name</span><span class="p">)</span><span class="o">.</span><span class="n">resolve</span><span class="p">()</span>
-</span><span id="main-40"><a href="#main-40"><span class="linenos">40</span></a>    <span class="n">run_tests</span><span class="p">(</span><span class="n">package_path</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="main-37"><a href="#main-37"><span class="linenos">37</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
+</span><span id="main-38"><a href="#main-38"><span class="linenos">38</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="p">:</span>
+</span><span id="main-39"><a href="#main-39"><span class="linenos">39</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
+</span><span id="main-40"><a href="#main-40"><span class="linenos">40</span></a>    <span class="n">package_path</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package_name</span><span class="p">)</span><span class="o">.</span><span class="n">resolve</span><span class="p">()</span>
+</span><span id="main-41"><a href="#main-41"><span class="linenos">41</span></a>    <span class="n">run_tests</span><span class="p">(</span><span class="n">package_path</span><span class="p">)</span>
 </span></pre></div>
 
 
     
 
                 </section>
     </main>
```

#### html2text {}

```diff
@@ -8,57 +8,18 @@
     * main
 built_with_pdoc[pdoc_logo]
 
 ****** hassle.run_tests ******
 ⁰ View Source
 _1import argparse
 _2import os
-_3from pathlib import Path
-_4
+_3
+_4from pathier import Pathier
 _5
-_6def get_args() -> argparse.Namespace:
-_7    parser = argparse.ArgumentParser()
-_8
-_9    parser.add_argument(
-10        "package_name",
-11        type=str,
-12        default=".",
-13        nargs="?",
-14        help=""" The name of the package or project to run tests for,
-15        assuming it's a subfolder of your current working directory.
-16        Can also be a full path to the package. If nothing is given,
-17        the current working directory will be used.""",
-18    )
-19
-20    args = parser.parse_args()
-21
-22    return args
-23
-24
-25def run_tests(package_path: Path):
-26    """Run tests with coverage and pytest."""
-27    startdir = Path().cwd()
-28    os.chdir(package_path)
-29    os.system(f"pip install -e .")
-30    os.system(f"coverage run -m pytest -s")
-31    os.system(f"coverage report -m")
-32    os.chdir(startdir)
-33
-34
-35def main(args: argparse.Namespace = None):
-36    if not args:
-37        args = get_args()
-38    package_path = Path(args.package_name).resolve()
-39    run_tests(package_path)
-40
-41
-42if __name__ == "__main__":
-43    main(get_args())
-  ⁰
-def get_args() -> argparse.Namespace: View Source
+_6
 _7def get_args() -> argparse.Namespace:
 _8    parser = argparse.ArgumentParser()
 _9
 10    parser.add_argument(
 11        "package_name",
 12        type=str,
 13        default=".",
@@ -68,26 +29,66 @@
 17        Can also be a full path to the package. If nothing is given,
 18        the current working directory will be used.""",
 19    )
 20
 21    args = parser.parse_args()
 22
 23    return args
-  ⁰
-def run_tests(package_path: pathlib.Path): View Source
-26def run_tests(package_path: Path):
+24
+25
+26def run_tests(package_path: Pathier):
 27    """Run tests with coverage and pytest."""
-28    startdir = Path().cwd()
+28    startdir = Pathier().cwd()
 29    os.chdir(package_path)
 30    os.system(f"pip install -e .")
 31    os.system(f"coverage run -m pytest -s")
 32    os.system(f"coverage report -m")
 33    os.chdir(startdir)
-Run tests with coverage and pytest.
-  ⁰
-def main(args: argparse.Namespace = None): View Source
+34
+35
 36def main(args: argparse.Namespace = None):
 37    if not args:
 38        args = get_args()
-39    package_path = Path(args.package_name).resolve()
+39    package_path = Pathier(args.package_name).resolve()
 40    run_tests(package_path)
+41
+42
+43if __name__ == "__main__":
+44    main(get_args())
+  ⁰
+def get_args() -> argparse.Namespace: View Source
+_8def get_args() -> argparse.Namespace:
+_9    parser = argparse.ArgumentParser()
+10
+11    parser.add_argument(
+12        "package_name",
+13        type=str,
+14        default=".",
+15        nargs="?",
+16        help=""" The name of the package or project to run tests for,
+17        assuming it's a subfolder of your current working directory.
+18        Can also be a full path to the package. If nothing is given,
+19        the current working directory will be used.""",
+20    )
+21
+22    args = parser.parse_args()
+23
+24    return args
+  ⁰
+def run_tests(package_path: pathier.pathier.Pathier): View Source
+27def run_tests(package_path: Pathier):
+28    """Run tests with coverage and pytest."""
+29    startdir = Pathier().cwd()
+30    os.chdir(package_path)
+31    os.system(f"pip install -e .")
+32    os.system(f"coverage run -m pytest -s")
+33    os.system(f"coverage report -m")
+34    os.chdir(startdir)
+Run tests with coverage and pytest.
+  ⁰
+def main(args: argparse.Namespace = None): View Source
+37def main(args: argparse.Namespace = None):
+38    if not args:
+39        args = get_args()
+40    package_path = Pathier(args.package_name).resolve()
+41    run_tests(package_path)
```

### Comparing `hassle-2.4.0/src/hassle/generate_tests.py` & `hassle-2.5.0/src/hassle/generate_tests.py`

 * *Files identical despite different names*

### Comparing `hassle-2.4.0/src/hassle/hassle.py` & `hassle-2.5.0/src/hassle/hassle.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 import argparse
 import os
-import shutil
-from pathlib import Path
 
-import tomlkit
+from pathier import Pathier
 
 from hassle import hassle_utilities
 from hassle.generate_tests import generate_test_files
 from hassle.run_tests import run_tests
 
-root = Path(__file__).parent
+root = Pathier(__file__).parent
 
 
 def get_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser()
 
     parser.add_argument(
         "package",
@@ -131,15 +129,15 @@
         help=""" Excpects one argument: "major", "minor", or "patch".
         Passing "-up minor" is equivalent to passing the cli string: "-b -t -i -iv minor -uc -ca build -s".
         To publish the updated package, the -p/--publish switch needs to be added to the cli input.""",
     )
 
     args = parser.parse_args()
 
-    args.package = Path(args.package).resolve()
+    args.package = Pathier(args.package).resolve()
 
     if args.update:
         args.build = True
         args.tag_version = True
         args.install = True
         args.increment_version = args.update
         args.update_changelog = True
@@ -176,18 +174,15 @@
     if args.run_tests:
         run_tests(args.package)
 
     if args.increment_version:
         hassle_utilities.increment_version(pyproject_path, args.increment_version)
 
     if args.build:
-        try:
-            shutil.rmtree(f"{args.package}/dist")
-        except Exception as e:
-            pass
+        (args.package / "dist").delete()
         os.system(f"black {args.package}")
         os.system(f"isort {args.package}")
         hassle_utilities.update_dependencies(
             pyproject_path, args.overwrite_dependencies
         )
         hassle_utilities.update_minimum_python_version(pyproject_path)
         hassle_utilities.generate_docs(args.package)
@@ -201,15 +196,15 @@
             os.chdir(args.package)
             os.system("git add CHANGELOG.md")
             os.system('git commit CHANGELOG.md -m "chore: update changelog"')
 
     if args.commit_all:
         os.chdir(args.package)
         if args.commit_all == "build":
-            version = tomlkit.loads(pyproject_path.read_text())["project"]["version"]
+            version = pyproject_path.loads()["project"]["version"]
             args.commit_all = f"chore: build v{version}"
         os.system("git add .")
         os.system(f'git commit -m "{args.commit_all}"')
 
     if args.tag_version:
         hassle_utilities.tag_version(args.package)
```

### Comparing `hassle-2.4.0/src/hassle/hassle_config.py` & `hassle-2.5.0/src/hassle/hassle_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import argparse
-from pathlib import Path
 
-import tomlkit
+from pathier import Pathier
 
-root = Path(__file__).parent
+root = Pathier(__file__).parent
 
 
 def get_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser()
 
     parser.add_argument(
         "-n",
@@ -74,24 +73,24 @@
     """Check if hassle_config.toml exists."""
     return (root / "hassle_config.toml").exists()
 
 
 def load_config() -> dict:
     "Load and return hassle_config contents if it exists."
     if config_exists():
-        return tomlkit.loads((root / "hassle_config.toml").read_text())
+        return (root / "hassle_config.toml").loads()
     else:
         raise FileNotFoundError(
             f"load_config() could not find {root/'hassle_config.toml'}.\nRun hassle_config to set it."
         )
 
 
 def write_config(config: dict):
     """Dump config to "hassle_config.toml."""
-    (root / "hassle_config.toml").write_text(tomlkit.dumps(config))
+    (root / "hassle_config.toml").dumps(config)
 
 
 def warn():
     print("hassle_config.toml has not been set.")
     print("Run hassle_config to set it.")
     print("Run 'hassle_config -h' for help.")
```

### Comparing `hassle-2.4.0/src/hassle/hassle_utilities.py` & `hassle-2.5.0/src/hassle/hassle_utilities.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,69 +1,67 @@
 import os
-import shutil
-from pathlib import Path
 
 import packagelister
-import tomlkit
 import vermin
+from pathier import Pathier
 
 from hassle import hassle_config
 
-root = Path(__file__).parent
+root = Pathier(__file__).parent
 
 
-def increment_version(pyproject_path: Path, increment_type: str):
+def increment_version(pyproject_path: Pathier, increment_type: str):
     """Increment the project.version field in pyproject.toml.
 
     :param package_path: Path to the package/project directory.
 
     :param increment_type: One from 'major', 'minor', or 'patch'."""
-    meta = tomlkit.loads(pyproject_path.read_text())
+    meta = pyproject_path.loads()
     major, minor, patch = [int(num) for num in meta["project"]["version"].split(".")]
     if increment_type == "major":
         major += 1
         minor = 0
         patch = 0
     elif increment_type == "minor":
         minor += 1
         patch = 0
     elif increment_type == "patch":
         patch += 1
     incremented_version = ".".join(str(num) for num in [major, minor, patch])
     meta["project"]["version"] = incremented_version
-    pyproject_path.write_text(tomlkit.dumps(meta))
+    pyproject_path.dumps(meta)
 
 
-def update_minimum_python_version(pyproject_path: Path):
+def update_minimum_python_version(pyproject_path: Pathier):
     """Use vermin to determine the minimum compatible
     Python version and update the corresponding field
     in pyproject.toml."""
     project_code = "\n".join(
         file.read_text() for file in (pyproject_path.parent / "src").rglob("*.py")
     )
-    meta = tomlkit.loads(pyproject_path.read_text())
+    meta = pyproject_path.loads()
     minimum_version = vermin.visit(project_code, vermin.Config()).minimum_versions()[1]
     minimum_version = f">={minimum_version[0]}.{minimum_version[1]}"
     meta["project"]["requires-python"] = minimum_version
-    pyproject_path.write_text(tomlkit.dumps(meta))
+    pyproject_path.dumps(meta)
 
 
-def generate_docs(package_path: Path):
+def generate_docs(package_path: Pathier):
     """Generate project documentation using pdoc."""
     try:
-        shutil.rmtree(package_path / "docs")
+        (package_path / "docs").delete()
     except Exception as e:
         pass
     os.system(
         f"pdoc -o {package_path / 'docs'} {package_path / 'src' / package_path.stem}"
     )
 
 
 def update_dependencies(
-    pyproject_path: Path, overwrite: bool, include_versions: bool = False
+    pyproject_path: Pathier, overwrite: bool, include_versions: bool = False
 ):
     """Update dependencies list in pyproject.toml.
 
     :param overwrite: If True, replace the dependencies in pyproject.toml
     with the results of packagelister.scan() .
     If False, packages returned by packagelister are appended to
     the current dependencies in pyproject.toml if they don't already
@@ -77,35 +75,35 @@
         for package in packages
         if package != pyproject_path.parent.stem
     ]
     packages = [
         package.replace("speech_recognition", "speechRecognition")
         for package in packages
     ]
-    meta = tomlkit.loads(pyproject_path.read_text())
+    meta = pyproject_path.loads()
     if overwrite:
         meta["project"]["dependencies"] = packages
     else:
         for package in packages:
             if "~" in package:
                 name = package.split("~")[0]
             elif "=" in package:
                 name = package.split("=")[0]
             else:
                 name = package
             if all(
                 name not in dependency for dependency in meta["project"]["dependencies"]
             ):
                 meta["project"]["dependencies"].append(package)
-    pyproject_path.write_text(tomlkit.dumps(meta))
+    pyproject_path.dumps(meta)
 
 
-def update_changelog(pyproject_path: Path):
+def update_changelog(pyproject_path: Pathier):
     """Update project changelog."""
-    meta = tomlkit.loads(pyproject_path.read_text())
+    meta = pyproject_path.loads()
     if hassle_config.config_exists():
         config = hassle_config.load_config()
     else:
         hassle_config.warn()
         print("Creating blank hassle_config.toml...")
         config = hassle_config.load_config()
     changelog_path = pyproject_path.parent / "CHANGELOG.md"
@@ -113,20 +111,18 @@
         f"auto-changelog -p {pyproject_path.parent} --tag-prefix {config['git']['tag_prefix']} --unreleased -v {meta['project']['version']} -o {changelog_path}"
     )
     changelog = changelog_path.read_text().splitlines()
     changelog = [line for line in changelog if "Full set of changes:" not in line]
     changelog_path.write_text("\n".join(changelog))
 
 
-def tag_version(package_path: Path):
+def tag_version(package_path: Pathier):
     """Add a git tag corresponding
     to the version number in pyproject.toml."""
     if hassle_config.config_exists():
         tag_prefix = hassle_config.load_config()["git"]["tag_prefix"]
     else:
         hassle_config.warn()
         tag_prefix = ""
-    version = tomlkit.loads((package_path / "pyproject.toml").read_text())["project"][
-        "version"
-    ]
+    version = (package_path / "pyproject.toml").loads()["project"]["version"]
     os.chdir(package_path)
     os.system(f"git tag {tag_prefix}{version}")
```

### Comparing `hassle-2.4.0/src/hassle/license_template.txt` & `hassle-2.5.0/src/hassle/license_template.txt`

 * *Files identical despite different names*

### Comparing `hassle-2.4.0/src/hassle/new_project.py` & `hassle-2.5.0/src/hassle/new_project.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 import argparse
 import os
-import shutil
 import sys
 from datetime import datetime
-from pathlib import Path
 
 import requests
-import tomlkit
 from bs4 import BeautifulSoup
+from pathier import Pathier
 
 import hassle.hassle_config as hassle_config
 from hassle.generate_tests import generate_test_files
 
-root = Path(__file__).parent
+root = Pathier(__file__).parent
 
 
 def get_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser()
 
     parser.add_argument(
         "name",
@@ -151,18 +149,18 @@
     args = parser.parse_args()
     if check_pypi_for_name(args.name):
         print(f"{args.name} is already taken.")
     else:
         print(f"{args.name} is available.")
 
 
-def create_pyproject_file(targetdir: Path, args: argparse.Namespace):
+def create_pyproject_file(targetdir: Pathier, args: argparse.Namespace):
     """Create pyproject.toml in ./{project_name} from args,
     pyproject_template, and hassle_config."""
-    pyproject = tomlkit.loads((root / "pyproject_template.toml").read_text())
+    pyproject = (root / "pyproject_template.toml").loads()
     if not hassle_config.config_exists():
         hassle_config.warn()
         if not get_answer("Continue creating new package with blank config?"):
             raise Exception("Aborting new package creation")
         else:
             print("Creating blank hassle_config.toml...")
             hassle_config.create_config()
@@ -180,51 +178,51 @@
         pyproject["project"]["classifiers"].pop(1)
     for field in config["project_urls"]:
         pyproject["project"]["urls"][field] = config["project_urls"][field].replace(
             "$name", args.name
         )
     if args.add_script:
         pyproject["project"]["scripts"][args.name] = f"{args.name}.{args.name}:main"
-    (targetdir / "pyproject.toml").write_text(tomlkit.dumps(pyproject))
+    (targetdir / "pyproject.toml").dumps(pyproject)
 
 
-def create_source_files(srcdir: Path, filelist: list[str]):
+def create_source_files(srcdir: Pathier, filelist: list[str]):
     """Generate empty source files in ./{package_name}/src/{package_name}/"""
     srcdir.mkdir(parents=True, exist_ok=True)
     for file in filelist:
         (srcdir / file).touch()
 
 
-def create_readme(targetdir: Path, args: argparse.Namespace):
+def create_readme(targetdir: Pathier, args: argparse.Namespace):
     """Create README.md in ./{package_name}
     from readme_template and args."""
     readme = (root / "README_template.md").read_text()
     readme = readme.replace("$name", args.name).replace(
         "$description", args.description
     )
     (targetdir / "README.md").write_text(readme)
 
 
-def create_license(targetdir: Path):
+def create_license(targetdir: Pathier):
     """Add MIT license file to ./{package_name} ."""
     license_template = (root / "license_template.txt").read_text()
     license_template = license_template.replace("$year", str(datetime.now().year))
     (targetdir / "LICENSE.txt").write_text(license_template)
 
 
-def create_gitignore(targetdir: Path):
+def create_gitignore(targetdir: Pathier):
     """Add .gitignore to ./{package_name}"""
-    shutil.copy(root / ".gitignore_template", targetdir / ".gitignore")
+    (root / ".gitignore_template").copy(targetdir / ".gitignore", True)
 
 
-def create_vscode_settings(targetdir: Path):
+def create_vscode_settings(targetdir: Pathier):
     """Add settings.json to ./.vscode"""
     vsdir = targetdir / ".vscode"
     vsdir.mkdir(parents=True, exist_ok=True)
-    shutil.copy(root / ".vscode_template", vsdir / "settings.json")
+    (root / ".vscode_template").copy(vsdir / "settings.json", True)
 
 
 def main(args: argparse.Namespace = None):
     if not args:
         args = get_args()
     if not args.not_package:
         try:
@@ -236,15 +234,15 @@
             print(e)
             print(
                 f"Couldn't verify that {args.name} doesn't already exist on pypi.org ."
             )
             if not get_answer("Continue anyway?"):
                 sys.exit(0)
     try:
-        targetdir = Path.cwd() / args.name
+        targetdir: Pathier = Pathier.cwd() / args.name
         try:
             targetdir.mkdir(parents=True, exist_ok=False)
         except:
             print(f"{targetdir} already exists.")
             if not get_answer("Overwrite?"):
                 sys.exit(0)
         if not args.not_package:
@@ -263,12 +261,12 @@
         os.chdir(targetdir)
         os.system("git init -b main")
 
     except Exception as e:
         if not "Aborting new package creation" in str(e):
             print(e)
         if get_answer("Delete created files?"):
-            shutil.rmtree(targetdir)
+            targetdir.delete()
 
 
 if __name__ == "__main__":
     main(get_args())
```

### Comparing `hassle-2.4.0/src/hassle/pyproject_template.toml` & `hassle-2.5.0/src/hassle/pyproject_template.toml`

 * *Files identical despite different names*

### Comparing `hassle-2.4.0/src/hassle/run_tests.py` & `hassle-2.5.0/src/hassle/run_tests.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import argparse
 import os
-from pathlib import Path
+
+from pathier import Pathier
 
 
 def get_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser()
 
     parser.add_argument(
         "package_name",
@@ -18,26 +19,26 @@
     )
 
     args = parser.parse_args()
 
     return args
 
 
-def run_tests(package_path: Path):
+def run_tests(package_path: Pathier):
     """Run tests with coverage and pytest."""
-    startdir = Path().cwd()
+    startdir = Pathier().cwd()
     os.chdir(package_path)
     os.system(f"pip install -e .")
     os.system(f"coverage run -m pytest -s")
     os.system(f"coverage report -m")
     os.chdir(startdir)
 
 
 def main(args: argparse.Namespace = None):
     if not args:
         args = get_args()
-    package_path = Path(args.package_name).resolve()
+    package_path = Pathier(args.package_name).resolve()
     run_tests(package_path)
 
 
 if __name__ == "__main__":
     main(get_args())
```

### Comparing `hassle-2.4.0/LICENSE.txt` & `hassle-2.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hassle-2.4.0/README.md` & `hassle-2.5.0/README.md`

 * *Files identical despite different names*

### Comparing `hassle-2.4.0/pyproject.toml` & `hassle-2.5.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -10,93 +10,90 @@
 00000090: 226d 6174 746d 616e 6573 4070 6d2e 6d65  "mattmanes@pm.me
 000000a0: 227d 5d0d 0a64 6573 6372 6970 7469 6f6e  "}]..description
 000000b0: 203d 2022 4372 6561 7465 2c20 6275 696c   = "Create, buil
 000000c0: 642c 2074 6573 742c 2061 6e64 2070 7562  d, test, and pub
 000000d0: 6c69 7368 2050 7974 686f 6e20 7072 6f6a  lish Python proj
 000000e0: 6563 7473 2061 6e64 2070 6163 6b61 6765  ects and package
 000000f0: 732e 220d 0a76 6572 7369 6f6e 203d 2022  s."..version = "
-00000100: 322e 342e 3022 0d0a 7265 7175 6972 6573  2.4.0"..requires
+00000100: 322e 352e 3022 0d0a 7265 7175 6972 6573  2.5.0"..requires
 00000110: 2d70 7974 686f 6e20 3d20 223e 3d33 2e31  -python = ">=3.1
 00000120: 3022 0d0a 6465 7065 6e64 656e 6369 6573  0"..dependencies
-00000130: 203d 205b 0d0a 2020 2020 2274 6f6d 6c6b   = [..    "tomlk
-00000140: 6974 3d3d 302e 3131 2e36 222c 200d 0a20  it==0.11.6", .. 
-00000150: 2020 2022 626c 6163 6b22 2c20 0d0a 2020     "black", ..  
-00000160: 2020 2269 736f 7274 222c 200d 0a20 2020    "isort", ..   
-00000170: 2022 7079 7465 7374 7e3d 372e 322e 3122   "pytest~=7.2.1"
-00000180: 2c20 0d0a 2020 2020 2263 6f76 6572 6167  , ..    "coverag
-00000190: 6522 2c0d 0a20 2020 2022 7061 636b 6167  e",..    "packag
-000001a0: 656c 6973 7465 727e 3d31 2e31 2e32 222c  elister~=1.1.2",
-000001b0: 0d0a 2020 2020 2276 6572 6d69 6e3d 3d31  ..    "vermin==1
-000001c0: 2e35 2e31 222c 0d0a 2020 2020 2270 646f  .5.1",..    "pdo
-000001d0: 6322 2c0d 0a20 2020 2022 7477 696e 6522  c",..    "twine"
-000001e0: 2c0d 0a20 2020 2022 6175 746f 2d63 6861  ,..    "auto-cha
-000001f0: 6e67 656c 6f67 222c 0d0a 2020 2020 2262  ngelog",..    "b
-00000200: 7334 3d3d 302e 302e 3122 2c0d 0a20 2020  s4==0.0.1",..   
-00000210: 2022 7265 7175 6573 7473 7e3d 322e 3238   "requests~=2.28
-00000220: 2e31 222c 0d0a 2020 2020 2262 7569 6c64  .1",..    "build
-00000230: 222c 0d0a 2020 2020 2270 6174 6869 6572  ",..    "pathier
-00000240: 220d 0a20 2020 205d 0d0a 7265 6164 6d65  "..    ]..readme
-00000250: 203d 2022 5245 4144 4d45 2e6d 6422 0d0a   = "README.md"..
-00000260: 6b65 7977 6f72 6473 203d 205b 2264 6576  keywords = ["dev
-00000270: 6f70 7322 2c20 2270 6163 6b61 6769 6e67  ops", "packaging
-00000280: 222c 2022 6275 696c 6422 2c20 2274 6573  ", "build", "tes
-00000290: 7422 2c20 2261 7574 6f6d 6174 696f 6e22  t", "automation"
-000002a0: 5d0d 0a63 6c61 7373 6966 6965 7273 203d  ]..classifiers =
-000002b0: 205b 0d0a 2020 2020 2250 726f 6772 616d   [..    "Program
-000002c0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-000002d0: 2050 7974 686f 6e20 3a3a 2033 222c 0d0a   Python :: 3",..
-000002e0: 2020 2020 224c 6963 656e 7365 203a 3a20      "License :: 
-000002f0: 4f53 4920 4170 7072 6f76 6564 203a 3a20  OSI Approved :: 
-00000300: 4d49 5420 4c69 6365 6e73 6522 2c0d 0a20  MIT License",.. 
-00000310: 2020 2022 4f70 6572 6174 696e 6720 5379     "Operating Sy
-00000320: 7374 656d 203a 3a20 4f53 2049 6e64 6570  stem :: OS Indep
-00000330: 656e 6465 6e74 222c 0d0a 2020 2020 5d0d  endent",..    ].
-00000340: 0a0d 0a5b 7072 6f6a 6563 742e 7572 6c73  ...[project.urls
-00000350: 5d0d 0a22 486f 6d65 7061 6765 2220 3d20  ].."Homepage" = 
-00000360: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
-00000370: 636f 6d2f 6d61 7474 2d6d 616e 6573 2f68  com/matt-manes/h
-00000380: 6173 736c 6522 0d0a 2244 6f63 756d 656e  assle".."Documen
-00000390: 7461 7469 6f6e 2220 3d20 2268 7474 7073  tation" = "https
-000003a0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6d61  ://github.com/ma
-000003b0: 7474 2d6d 616e 6573 2f68 6173 736c 652f  tt-manes/hassle/
-000003c0: 7472 6565 2f6d 6169 6e2f 646f 6373 220d  tree/main/docs".
-000003d0: 0a22 536f 7572 6365 2063 6f64 6522 203d  ."Source code" =
-000003e0: 2022 6874 7470 733a 2f2f 6769 7468 7562   "https://github
-000003f0: 2e63 6f6d 2f6d 6174 742d 6d61 6e65 732f  .com/matt-manes/
-00000400: 6861 7373 6c65 2f74 7265 652f 6d61 696e  hassle/tree/main
-00000410: 2f73 7263 2f68 6173 736c 6522 0d0a 0d0a  /src/hassle"....
-00000420: 5b74 6f6f 6c2e 7079 7465 7374 2e69 6e69  [tool.pytest.ini
-00000430: 5f6f 7074 696f 6e73 5d0d 0a61 6464 6f70  _options]..addop
-00000440: 7473 203d 205b 0d0a 2020 2020 222d 2d69  ts = [..    "--i
-00000450: 6d70 6f72 742d 6d6f 6465 3d69 6d70 6f72  mport-mode=impor
-00000460: 746c 6962 222c 0d0a 2020 2020 5d0d 0a70  tlib",..    ]..p
-00000470: 7974 686f 6e70 6174 6820 3d20 2273 7263  ythonpath = "src
-00000480: 220d 0a0d 0a5b 746f 6f6c 2e68 6174 6368  "....[tool.hatch
-00000490: 2e62 7569 6c64 2e74 6172 6765 7473 2e73  .build.targets.s
-000004a0: 6469 7374 5d0d 0a65 7863 6c75 6465 203d  dist]..exclude =
-000004b0: 205b 0d0a 2020 2020 222e 636f 7665 7261   [..    ".covera
-000004c0: 6765 222c 0d0a 2020 2020 222e 7079 7465  ge",..    ".pyte
-000004d0: 7374 5f63 6163 6865 222c 0d0a 2020 2020  st_cache",..    
-000004e0: 222e 7673 636f 6465 222c 0d0a 2020 2020  ".vscode",..    
-000004f0: 2274 6573 7473 222c 0d0a 2020 2020 226e  "tests",..    "n
-00000500: 6f74 6573 2e74 7874 222c 0d0a 2020 2020  otes.txt",..    
-00000510: 222e 6769 7469 676e 6f72 6522 2c0d 0a20  ".gitignore",.. 
-00000520: 2020 2022 6861 7373 6c65 5f63 6f6e 6669     "hassle_confi
-00000530: 672e 746f 6d6c 220d 0a20 2020 205d 0d0a  g.toml"..    ]..
-00000540: 5b70 726f 6a65 6374 2e73 6372 6970 7473  [project.scripts
-00000550: 5d0d 0a68 6173 736c 6520 3d20 2268 6173  ]..hassle = "has
-00000560: 736c 652e 6861 7373 6c65 3a6d 6169 6e22  sle.hassle:main"
-00000570: 0d0a 6e65 775f 7072 6f6a 6563 7420 3d20  ..new_project = 
-00000580: 2268 6173 736c 652e 6e65 775f 7072 6f6a  "hassle.new_proj
-00000590: 6563 743a 6d61 696e 220d 0a67 656e 6572  ect:main"..gener
-000005a0: 6174 655f 7465 7374 7320 3d20 2268 6173  ate_tests = "has
-000005b0: 736c 652e 6765 6e65 7261 7465 5f74 6573  sle.generate_tes
-000005c0: 7473 3a6d 6169 6e22 0d0a 7275 6e5f 7465  ts:main"..run_te
-000005d0: 7374 7320 3d20 2268 6173 736c 652e 7275  sts = "hassle.ru
-000005e0: 6e5f 7465 7374 733a 6d61 696e 220d 0a68  n_tests:main"..h
-000005f0: 6173 736c 655f 636f 6e66 6967 203d 2022  assle_config = "
-00000600: 6861 7373 6c65 2e68 6173 736c 655f 636f  hassle.hassle_co
-00000610: 6e66 6967 3a6d 6169 6e22 0d0a 6368 6563  nfig:main"..chec
-00000620: 6b5f 7079 7069 203d 2022 6861 7373 6c65  k_pypi = "hassle
-00000630: 2e6e 6577 5f70 726f 6a65 6374 3a63 6865  .new_project:che
-00000640: 636b 5f70 7970 695f 666f 725f 6e61 6d65  ck_pypi_for_name
-00000650: 5f63 6c69 22                             _cli"
+00000130: 203d 205b 0d0a 2020 2020 2262 6c61 636b   = [..    "black
+00000140: 222c 200d 0a20 2020 2022 6973 6f72 7422  ", ..    "isort"
+00000150: 2c20 0d0a 2020 2020 2270 7974 6573 747e  , ..    "pytest~
+00000160: 3d37 2e32 2e31 222c 200d 0a20 2020 2022  =7.2.1", ..    "
+00000170: 636f 7665 7261 6765 222c 0d0a 2020 2020  coverage",..    
+00000180: 2270 6163 6b61 6765 6c69 7374 6572 222c  "packagelister",
+00000190: 0d0a 2020 2020 2276 6572 6d69 6e3d 3d31  ..    "vermin==1
+000001a0: 2e35 2e31 222c 0d0a 2020 2020 2270 646f  .5.1",..    "pdo
+000001b0: 6322 2c0d 0a20 2020 2022 7477 696e 6522  c",..    "twine"
+000001c0: 2c0d 0a20 2020 2022 6175 746f 2d63 6861  ,..    "auto-cha
+000001d0: 6e67 656c 6f67 222c 0d0a 2020 2020 2262  ngelog",..    "b
+000001e0: 7334 222c 0d0a 2020 2020 2272 6571 7565  s4",..    "reque
+000001f0: 7374 7322 2c0d 0a20 2020 2022 6275 696c  sts",..    "buil
+00000200: 6422 2c0d 0a20 2020 2022 7061 7468 6965  d",..    "pathie
+00000210: 7222 0d0a 2020 2020 5d0d 0a72 6561 646d  r"..    ]..readm
+00000220: 6520 3d20 2252 4541 444d 452e 6d64 220d  e = "README.md".
+00000230: 0a6b 6579 776f 7264 7320 3d20 5b22 6465  .keywords = ["de
+00000240: 766f 7073 222c 2022 7061 636b 6167 696e  vops", "packagin
+00000250: 6722 2c20 2262 7569 6c64 222c 2022 7465  g", "build", "te
+00000260: 7374 222c 2022 6175 746f 6d61 7469 6f6e  st", "automation
+00000270: 225d 0d0a 636c 6173 7369 6669 6572 7320  "]..classifiers 
+00000280: 3d20 5b0d 0a20 2020 2022 5072 6f67 7261  = [..    "Progra
+00000290: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+000002a0: 3a20 5079 7468 6f6e 203a 3a20 3322 2c0d  : Python :: 3",.
+000002b0: 0a20 2020 2022 4c69 6365 6e73 6520 3a3a  .    "License ::
+000002c0: 204f 5349 2041 7070 726f 7665 6420 3a3a   OSI Approved ::
+000002d0: 204d 4954 204c 6963 656e 7365 222c 0d0a   MIT License",..
+000002e0: 2020 2020 224f 7065 7261 7469 6e67 2053      "Operating S
+000002f0: 7973 7465 6d20 3a3a 204f 5320 496e 6465  ystem :: OS Inde
+00000300: 7065 6e64 656e 7422 2c0d 0a20 2020 205d  pendent",..    ]
+00000310: 0d0a 0d0a 5b70 726f 6a65 6374 2e75 726c  ....[project.url
+00000320: 735d 0d0a 2248 6f6d 6570 6167 6522 203d  s].."Homepage" =
+00000330: 2022 6874 7470 733a 2f2f 6769 7468 7562   "https://github
+00000340: 2e63 6f6d 2f6d 6174 742d 6d61 6e65 732f  .com/matt-manes/
+00000350: 6861 7373 6c65 220d 0a22 446f 6375 6d65  hassle".."Docume
+00000360: 6e74 6174 696f 6e22 203d 2022 6874 7470  ntation" = "http
+00000370: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6d  s://github.com/m
+00000380: 6174 742d 6d61 6e65 732f 6861 7373 6c65  att-manes/hassle
+00000390: 2f74 7265 652f 6d61 696e 2f64 6f63 7322  /tree/main/docs"
+000003a0: 0d0a 2253 6f75 7263 6520 636f 6465 2220  .."Source code" 
+000003b0: 3d20 2268 7474 7073 3a2f 2f67 6974 6875  = "https://githu
+000003c0: 622e 636f 6d2f 6d61 7474 2d6d 616e 6573  b.com/matt-manes
+000003d0: 2f68 6173 736c 652f 7472 6565 2f6d 6169  /hassle/tree/mai
+000003e0: 6e2f 7372 632f 6861 7373 6c65 220d 0a0d  n/src/hassle"...
+000003f0: 0a5b 746f 6f6c 2e70 7974 6573 742e 696e  .[tool.pytest.in
+00000400: 695f 6f70 7469 6f6e 735d 0d0a 6164 646f  i_options]..addo
+00000410: 7074 7320 3d20 5b0d 0a20 2020 2022 2d2d  pts = [..    "--
+00000420: 696d 706f 7274 2d6d 6f64 653d 696d 706f  import-mode=impo
+00000430: 7274 6c69 6222 2c0d 0a20 2020 205d 0d0a  rtlib",..    ]..
+00000440: 7079 7468 6f6e 7061 7468 203d 2022 7372  pythonpath = "sr
+00000450: 6322 0d0a 0d0a 5b74 6f6f 6c2e 6861 7463  c"....[tool.hatc
+00000460: 682e 6275 696c 642e 7461 7267 6574 732e  h.build.targets.
+00000470: 7364 6973 745d 0d0a 6578 636c 7564 6520  sdist]..exclude 
+00000480: 3d20 5b0d 0a20 2020 2022 2e63 6f76 6572  = [..    ".cover
+00000490: 6167 6522 2c0d 0a20 2020 2022 2e70 7974  age",..    ".pyt
+000004a0: 6573 745f 6361 6368 6522 2c0d 0a20 2020  est_cache",..   
+000004b0: 2022 2e76 7363 6f64 6522 2c0d 0a20 2020   ".vscode",..   
+000004c0: 2022 7465 7374 7322 2c0d 0a20 2020 2022   "tests",..    "
+000004d0: 6e6f 7465 732e 7478 7422 2c0d 0a20 2020  notes.txt",..   
+000004e0: 2022 2e67 6974 6967 6e6f 7265 222c 0d0a   ".gitignore",..
+000004f0: 2020 2020 2268 6173 736c 655f 636f 6e66      "hassle_conf
+00000500: 6967 2e74 6f6d 6c22 0d0a 2020 2020 5d0d  ig.toml"..    ].
+00000510: 0a5b 7072 6f6a 6563 742e 7363 7269 7074  .[project.script
+00000520: 735d 0d0a 6861 7373 6c65 203d 2022 6861  s]..hassle = "ha
+00000530: 7373 6c65 2e68 6173 736c 653a 6d61 696e  ssle.hassle:main
+00000540: 220d 0a6e 6577 5f70 726f 6a65 6374 203d  "..new_project =
+00000550: 2022 6861 7373 6c65 2e6e 6577 5f70 726f   "hassle.new_pro
+00000560: 6a65 6374 3a6d 6169 6e22 0d0a 6765 6e65  ject:main"..gene
+00000570: 7261 7465 5f74 6573 7473 203d 2022 6861  rate_tests = "ha
+00000580: 7373 6c65 2e67 656e 6572 6174 655f 7465  ssle.generate_te
+00000590: 7374 733a 6d61 696e 220d 0a72 756e 5f74  sts:main"..run_t
+000005a0: 6573 7473 203d 2022 6861 7373 6c65 2e72  ests = "hassle.r
+000005b0: 756e 5f74 6573 7473 3a6d 6169 6e22 0d0a  un_tests:main"..
+000005c0: 6861 7373 6c65 5f63 6f6e 6669 6720 3d20  hassle_config = 
+000005d0: 2268 6173 736c 652e 6861 7373 6c65 5f63  "hassle.hassle_c
+000005e0: 6f6e 6669 673a 6d61 696e 220d 0a63 6865  onfig:main"..che
+000005f0: 636b 5f70 7970 6920 3d20 2268 6173 736c  ck_pypi = "hassl
+00000600: 652e 6e65 775f 7072 6f6a 6563 743a 6368  e.new_project:ch
+00000610: 6563 6b5f 7079 7069 5f66 6f72 5f6e 616d  eck_pypi_for_nam
+00000620: 655f 636c 6922                           e_cli"
```

### Comparing `hassle-2.4.0/PKG-INFO` & `hassle-2.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 Metadata-Version: 2.1
 Name: hassle
-Version: 2.4.0
+Version: 2.5.0
 Summary: Create, build, test, and publish Python projects and packages.
 Project-URL: Homepage, https://github.com/matt-manes/hassle
 Project-URL: Documentation, https://github.com/matt-manes/hassle/tree/main/docs
 Project-URL: Source code, https://github.com/matt-manes/hassle/tree/main/src/hassle
 Author-email: Matt Manes <mattmanes@pm.me>
 License-File: LICENSE.txt
 Keywords: automation,build,devops,packaging,test
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: auto-changelog
 Requires-Dist: black
-Requires-Dist: bs4==0.0.1
+Requires-Dist: bs4
 Requires-Dist: build
 Requires-Dist: coverage
 Requires-Dist: isort
-Requires-Dist: packagelister~=1.1.2
+Requires-Dist: packagelister
 Requires-Dist: pathier
 Requires-Dist: pdoc
 Requires-Dist: pytest~=7.2.1
-Requires-Dist: requests~=2.28.1
-Requires-Dist: tomlkit==0.11.6
+Requires-Dist: requests
 Requires-Dist: twine
 Requires-Dist: vermin==1.5.1
 Description-Content-Type: text/markdown
 
 # Hassle
 
 Automate creating, building, testing, and publishing Python projects and packages from the command line. <br>
```

