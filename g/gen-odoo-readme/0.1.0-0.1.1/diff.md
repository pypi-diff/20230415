# Comparing `tmp/gen-odoo-readme-0.1.0.tar.gz` & `tmp/gen-odoo-readme-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gen-odoo-readme-0.1.0.tar", last modified: Sat Jan 28 20:12:41 2023, max compression
+gzip compressed data, was "gen-odoo-readme-0.1.1.tar", last modified: Sat Apr 15 16:30:17 2023, max compression
```

## Comparing `gen-odoo-readme-0.1.0.tar` & `gen-odoo-readme-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-28 20:12:41.436686 gen-odoo-readme-0.1.0/
--rw-rw-r--   0 root         (0) root         (0)    34523 2023-01-28 13:41:54.000000 gen-odoo-readme-0.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2905 2023-01-28 20:12:41.436686 gen-odoo-readme-0.1.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     2266 2023-01-28 20:11:39.000000 gen-odoo-readme-0.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-28 20:12:41.436686 gen-odoo-readme-0.1.0/gen_odoo_readme.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2905 2023-01-28 20:12:41.000000 gen-odoo-readme-0.1.0/gen_odoo_readme.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      322 2023-01-28 20:12:41.000000 gen-odoo-readme-0.1.0/gen_odoo_readme.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-28 20:12:41.000000 gen-odoo-readme-0.1.0/gen_odoo_readme.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       59 2023-01-28 20:12:41.000000 gen-odoo-readme-0.1.0/gen_odoo_readme.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-01-28 20:12:41.000000 gen-odoo-readme-0.1.0/gen_odoo_readme.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)       80 2023-01-28 20:12:41.436686 gen-odoo-readme-0.1.0/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1129 2023-01-28 19:40:47.000000 gen-odoo-readme-0.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-28 20:12:41.436686 gen-odoo-readme-0.1.0/tools/
--rw-rw-r--   0 root         (0) root         (0)       43 2023-01-28 17:44:43.000000 gen-odoo-readme-0.1.0/tools/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3030 2023-01-28 15:40:07.000000 gen-odoo-readme-0.1.0/tools/gen_addon_readme.template
--rw-rw-r--   0 root         (0) root         (0)     9279 2023-01-28 17:37:44.000000 gen-odoo-readme-0.1.0/tools/gen_readme.py
--rw-rw-r--   0 root         (0) root         (0)     1199 2023-01-28 15:13:03.000000 gen-odoo-readme-0.1.0/tools/manifest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 16:30:17.855699 gen-odoo-readme-0.1.1/
+-rw-rw-r--   0 root         (0) root         (0)    34523 2023-01-28 13:41:54.000000 gen-odoo-readme-0.1.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2912 2023-04-15 16:30:17.855699 gen-odoo-readme-0.1.1/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     2273 2023-04-15 14:41:28.000000 gen-odoo-readme-0.1.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 16:30:17.855699 gen-odoo-readme-0.1.1/gen_odoo_readme.egg-info/
+-rw-rw-r--   0 root         (0) root         (0)     2912 2023-04-15 16:30:17.000000 gen-odoo-readme-0.1.1/gen_odoo_readme.egg-info/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      360 2023-04-15 16:30:17.000000 gen-odoo-readme-0.1.1/gen_odoo_readme.egg-info/SOURCES.txt
+-rw-rw-r--   0 root         (0) root         (0)        1 2023-04-15 16:30:17.000000 gen-odoo-readme-0.1.1/gen_odoo_readme.egg-info/dependency_links.txt
+-rw-rw-r--   0 root         (0) root         (0)       59 2023-04-15 16:30:17.000000 gen-odoo-readme-0.1.1/gen_odoo_readme.egg-info/entry_points.txt
+-rw-rw-r--   0 root         (0) root         (0)       42 2023-04-15 16:30:17.000000 gen-odoo-readme-0.1.1/gen_odoo_readme.egg-info/requires.txt
+-rw-rw-r--   0 root         (0) root         (0)        6 2023-04-15 16:30:17.000000 gen-odoo-readme-0.1.1/gen_odoo_readme.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)       80 2023-04-15 16:30:17.859699 gen-odoo-readme-0.1.1/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1182 2023-04-15 15:24:49.000000 gen-odoo-readme-0.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 16:30:17.855699 gen-odoo-readme-0.1.1/tools/
+-rw-rw-r--   0 root         (0) root         (0)       22 2023-04-15 16:22:39.000000 gen-odoo-readme-0.1.1/tools/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3030 2023-01-28 15:40:07.000000 gen-odoo-readme-0.1.1/tools/gen_addon_readme.template
+-rw-rw-r--   0 root         (0) root         (0)     9361 2023-04-15 15:34:36.000000 gen-odoo-readme-0.1.1/tools/gen_readme.py
+-rw-rw-r--   0 root         (0) root         (0)     1199 2023-01-28 15:13:03.000000 gen-odoo-readme-0.1.1/tools/manifest.py
```

### Comparing `gen-odoo-readme-0.1.0/LICENSE` & `gen-odoo-readme-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gen-odoo-readme-0.1.0/PKG-INFO` & `gen-odoo-readme-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen-odoo-readme
-Version: 0.1.0
+Version: 0.1.1
 Summary: Tool to create README.rst files for Odoo
 Home-page: https://github.com/jobiols/gen-readme
 Author: Jorge E. Obiols
 Author-email: jorge.obiols@gmail.com
 Keywords: odoo documentation readme rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -49,15 +49,15 @@
 
 The result is a fully pypi compilant README.rst in the root of each module of the repo
 
 
 Installation
 ------------
 
-    sudo pip install gen_odoo_readme
+    sudo pip install gen-odoo-readme
 
 see proyect in https://pypi.org/project/gen-odoo-readme/
 
 Use el comando gen-readme --help para obtener esta ayuda
 
     Usage: gen-readme [OPTIONS]
 
@@ -80,10 +80,10 @@
     #################################
     # Generate the odoo README.rst documentacion for each module in
     # the current repository.
     # you must install this: pip install gen-odoo-readme
 
     gen-readme \
         --org-name quilsoft-org \
-        --repo-name tony_star \
+        --repo-name star_enterprises \
         --branch 16.0 \
         --addons-dir "$PWD"
```

### Comparing `gen-odoo-readme-0.1.0/README.md` & `gen-odoo-readme-0.1.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 The result is a fully pypi compilant README.rst in the root of each module of the repo
 
 
 Installation
 ------------
 
-    sudo pip install gen_odoo_readme
+    sudo pip install gen-odoo-readme
 
 see proyect in https://pypi.org/project/gen-odoo-readme/
 
 Use el comando gen-readme --help para obtener esta ayuda
 
     Usage: gen-readme [OPTIONS]
 
@@ -62,10 +62,10 @@
     #################################
     # Generate the odoo README.rst documentacion for each module in
     # the current repository.
     # you must install this: pip install gen-odoo-readme
 
     gen-readme \
         --org-name quilsoft-org \
-        --repo-name tony_star \
+        --repo-name star_enterprises \
         --branch 16.0 \
         --addons-dir "$PWD"
```

### Comparing `gen-odoo-readme-0.1.0/gen_odoo_readme.egg-info/PKG-INFO` & `gen-odoo-readme-0.1.1/gen_odoo_readme.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen-odoo-readme
-Version: 0.1.0
+Version: 0.1.1
 Summary: Tool to create README.rst files for Odoo
 Home-page: https://github.com/jobiols/gen-readme
 Author: Jorge E. Obiols
 Author-email: jorge.obiols@gmail.com
 Keywords: odoo documentation readme rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -49,15 +49,15 @@
 
 The result is a fully pypi compilant README.rst in the root of each module of the repo
 
 
 Installation
 ------------
 
-    sudo pip install gen_odoo_readme
+    sudo pip install gen-odoo-readme
 
 see proyect in https://pypi.org/project/gen-odoo-readme/
 
 Use el comando gen-readme --help para obtener esta ayuda
 
     Usage: gen-readme [OPTIONS]
 
@@ -80,10 +80,10 @@
     #################################
     # Generate the odoo README.rst documentacion for each module in
     # the current repository.
     # you must install this: pip install gen-odoo-readme
 
     gen-readme \
         --org-name quilsoft-org \
-        --repo-name tony_star \
+        --repo-name star_enterprises \
         --branch 16.0 \
         --addons-dir "$PWD"
```

### Comparing `gen-odoo-readme-0.1.0/setup.py` & `gen-odoo-readme-0.1.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,32 @@
-# -*- coding: utf-8 -*-
-
 import setuptools
 
-with open("README.md", "r") as fh:
+with open("README.md") as fh:
     long_description = fh.read()
 
+from tools import __version__
+
 setuptools.setup(
-    name='gen-odoo-readme',
-    version='0.1.0',
-    author='Jorge E. Obiols',
-    description='Tool to create README.rst files for Odoo',
+    name="gen-odoo-readme",
+    version=__version__,
+    author="Jorge E. Obiols",
+    description="Tool to create README.rst files for Odoo",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url='https://github.com/jobiols/gen-readme',
-    author_email='jorge.obiols@gmail.com',
-    python_requires='>=3.8',
+    url="https://github.com/jobiols/gen-readme",
+    author_email="jorge.obiols@gmail.com",
+    python_requires=">=3.8",
     entry_points={
-        'console_scripts': [
-            'gen-readme=tools.gen_readme:gen_readme',
+        "console_scripts": [
+            "gen-readme=tools.gen_readme:gen_readme",
         ],
     },
     include_package_data=True,
-    data_files=[('mypackage', ['tools/gen_addon_readme.template'])],
-    install_requires=[],
-
+    data_files=[("mypackage", ["tools/gen_addon_readme.template"])],
+    install_requires=["click==8.1.3", "jinja2==3.1.2", "docutils==0.19"],
     packages=setuptools.find_packages(),
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.8",
         "Operating System :: OS Independent",
```

### Comparing `gen-odoo-readme-0.1.0/tools/gen_addon_readme.template` & `gen-odoo-readme-0.1.1/tools/gen_addon_readme.template`

 * *Files identical despite different names*

### Comparing `gen-odoo-readme-0.1.0/tools/gen_readme.py` & `gen-odoo-readme-0.1.1/tools/gen_readme.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,232 +2,235 @@
 import os
 import re
 from .manifest import find_addons
 from jinja2 import Template
 from docutils.core import publish_file
 import tempfile
 
-FRAGMENTS_DIR = 'readme'
+FRAGMENTS_DIR = "readme"
 
 FRAGMENTS = (
-    'DESCRIPTION',
-    'INSTALL',
-    'CONFIGURE',
-    'USAGE',
-    'ROADMAP',
-    'DEVELOP',
-    'CONTRIBUTORS',
-    'CREDITS',
-    'HISTORY',
+    "DESCRIPTION",
+    "INSTALL",
+    "CONFIGURE",
+    "USAGE",
+    "ROADMAP",
+    "DEVELOP",
+    "CONTRIBUTORS",
+    "CREDITS",
+    "HISTORY",
 )
 
 DEVELOPMENT_STATUS_BADGES = {
-    'mature': (
-        'https://img.shields.io/badge/maturity-Mature-brightgreen.png',
-        'https://odoo-community.org/page/development-status',
-        'Mature',
+    "mature": (
+        "https://img.shields.io/badge/maturity-Mature-brightgreen.png",
+        "https://odoo-community.org/page/development-status",
+        "Mature",
     ),
-    'production/stable': (
-        'https://img.shields.io/badge/maturity-Production%2FStable-green.png',
-        'https://odoo-community.org/page/development-status',
-        'Production/Stable',
+    "production/stable": (
+        "https://img.shields.io/badge/maturity-Production%2FStable-green.png",
+        "https://odoo-community.org/page/development-status",
+        "Production/Stable",
     ),
-    'beta': (
-        'https://img.shields.io/badge/maturity-Beta-yellow.png',
-        'https://odoo-community.org/page/development-status',
-        'Beta',
+    "beta": (
+        "https://img.shields.io/badge/maturity-Beta-yellow.png",
+        "https://odoo-community.org/page/development-status",
+        "Beta",
     ),
-    'alpha': (
-        'https://img.shields.io/badge/maturity-Alpha-red.png',
-        'https://odoo-community.org/page/development-status',
-        'Alpha',
+    "alpha": (
+        "https://img.shields.io/badge/maturity-Alpha-red.png",
+        "https://odoo-community.org/page/development-status",
+        "Alpha",
     ),
 }
 
 LICENSE_BADGES = {
-    'AGPL-3': (
-        'https://img.shields.io/badge/licence-AGPL--3-blue.png',
-        'http://www.gnu.org/licenses/agpl-3.0-standalone.html',
-        'License: AGPL-3',
+    "AGPL-3": (
+        "https://img.shields.io/badge/licence-AGPL--3-blue.png",
+        "http://www.gnu.org/licenses/agpl-3.0-standalone.html",
+        "License: AGPL-3",
     ),
-    'LGPL-3': (
-        'https://img.shields.io/badge/licence-LGPL--3-blue.png',
-        'http://www.gnu.org/licenses/lgpl-3.0-standalone.html',
-        'License: LGPL-3',
+    "LGPL-3": (
+        "https://img.shields.io/badge/licence-LGPL--3-blue.png",
+        "http://www.gnu.org/licenses/lgpl-3.0-standalone.html",
+        "License: LGPL-3",
     ),
-    'GPL-3': (
-        'https://img.shields.io/badge/licence-GPL--3-blue.png',
-        'http://www.gnu.org/licenses/gpl-3.0-standalone.html',
-        'License: GPL-3',
+    "GPL-3": (
+        "https://img.shields.io/badge/licence-GPL--3-blue.png",
+        "http://www.gnu.org/licenses/gpl-3.0-standalone.html",
+        "License: GPL-3",
     ),
 }
 
 # this comes from pypa/readme_renderer
 RST2HTML_SETTINGS = {
     # Prevent local files from being included into the rendered output.
     # This is a security concern because people can insert files
     # that are part of the system, such as /etc/passwd.
     "file_insertion_enabled": False,
-
     # Halt rendering and throw an exception if there was any errors or
     # warnings from docutils.
     "halt_level": 2,
-
     # Output math blocks as LaTeX that can be interpreted by MathJax for
     # a prettier display of Math formulas.
     "math_output": "MathJax",
-
     # Disable raw html as enabling it is a security risk, we do not want
     # people to be able to include any old HTML in the final output.
     "raw_enabled": False,
-
     # Use typographic quotes, and transform --, ---, and ... into their
     # typographic counterparts.
     "smart_quotes": True,
-
     # Use the short form of syntax highlighting so that the generated
     # Pygments CSS can be used to style the output.
     "syntax_highlight": "short",
 }
 
+
 def gen_one_addon_index(readme_filename):
     addon_dir = os.path.dirname(readme_filename)
-    index_dir = os.path.join(addon_dir, 'static', 'description')
-    index_filename = os.path.join(index_dir, 'index.html')
+    index_dir = os.path.join(addon_dir, "static", "description")
+    index_filename = os.path.join(index_dir, "index.html")
     if os.path.exists(index_filename):
         with open(index_filename) as f:
-            if 'oca-gen-addon-readme' not in f.read():
+            if "oca-gen-addon-readme" not in f.read():
                 # index was created manually
                 return
     if not os.path.isdir(index_dir):
         os.makedirs(index_dir)
     publish_file(
         source_path=readme_filename,
         destination_path=index_filename,
-        writer_name='html4css1',
+        writer_name="html4css1",
         settings_overrides=RST2HTML_SETTINGS,
     )
     with open(index_filename, "rb") as f:
         index = f.read()
     # remove the docutils version from generated html, to avoid
     # useless changes in the readme
     index = re.sub(
-        rb'(<meta.*generator.*Docutils)\s*[\d.]+', rb"\1", index, re.MULTILINE
+        rb"(<meta.*generator.*Docutils)\s*[\d.]+", rb"\1", index, re.MULTILINE
     )
     with open(index_filename, "wb") as f:
         f.write(index)
     return index_filename
 
+
 def check_rst(readme_filename):
     with tempfile.NamedTemporaryFile() as f:
         publish_file(
             source_path=readme_filename,
             destination=f,
-            writer_name='html4css1',
+            writer_name="html4css1",
             settings_overrides=RST2HTML_SETTINGS,
         )
 
+
 def make_repo_badge(org_name, repo_name, branch, addon_name):
-    badge_repo_name = repo_name.replace('-', '--')
+    badge_repo_name = repo_name.replace("-", "--")
     return (
-        'https://img.shields.io/badge/github-{org_name}%2F{badge_repo_name}'
-        '-lightgray.png?logo=github'.format(**locals()),
-        'https://github.com/{org_name}/{repo_name}/tree/'
-        '{branch}/{addon_name}'.format(**locals()),
-        '{org_name}/{repo_name}'.format(**locals()),
+        "https://img.shields.io/badge/github-{org_name}%2F{badge_repo_name}"
+        "-lightgray.png?logo=github".format(**locals()),
+        "https://github.com/{org_name}/{repo_name}/tree/"
+        "{branch}/{addon_name}".format(**locals()),
+        "{org_name}/{repo_name}".format(**locals()),
     )
 
+
 def generate_fragment(org_name, repo_name, branch, addon_name, file):
     fragment_lines = file.readlines()
     if not fragment_lines:
         return False
 
     # Replace relative path by absolute path for figures
-    image_path_re = re.compile(
-        r'.*\s*\.\..* (figure|image)::\s+(?P<path>.*?)\s*$')
-    module_url = "https://raw.githubusercontent.com/{org_name}/{repo_name}"\
+    image_path_re = re.compile(r".*\s*\.\..* (figure|image)::\s+(?P<path>.*?)\s*$")
+    module_url = (
+        "https://raw.githubusercontent.com/{org_name}/{repo_name}"
         "/{branch}/{addon_name}/".format(**locals())
+    )
     for index, fragment_line in enumerate(fragment_lines):
         mo = image_path_re.match(fragment_line)
         if not mo:
             continue
-        path = mo.group('path')
+        path = mo.group("path")
 
-        if path.startswith('http'):
+        if path.startswith("http"):
             # It is already an absolute path
             continue
         else:
             # remove '../' if exists that make the fragment working
             # on github interface, in the 'readme' subfolder
-            relative_path = path.replace('../', '')
+            relative_path = path.replace("../", "")
             fragment_lines[index] = fragment_line.replace(
-                path, urljoin(module_url, relative_path))
-    fragment = ''.join(fragment_lines)
+                path, urljoin(module_url, relative_path)
+            )
+    fragment = "".join(fragment_lines)
 
     # ensure that there is a new empty line at the end of the fragment
-    if fragment[-1] != '\n':
-        fragment += '\n'
+    if fragment[-1] != "\n":
+        fragment += "\n"
     return fragment
 
 
 def gen_one_addon_readme(org_name, repo_name, branch, addon_name, addon_dir, manifest):
     fragments = {}
     for fragment_name in FRAGMENTS:
         fragment_filename = os.path.join(
-            addon_dir, FRAGMENTS_DIR, fragment_name + '.rst',
+            addon_dir,
+            FRAGMENTS_DIR,
+            fragment_name + ".rst",
         )
         if os.path.exists(fragment_filename):
-            with open(fragment_filename, 'r', encoding='utf8') as f:
-                fragment = generate_fragment(
-                    org_name, repo_name, branch, addon_name, f)
+            with open(fragment_filename, encoding="utf8") as f:
+                fragment = generate_fragment(org_name, repo_name, branch, addon_name, f)
                 if fragment:
                     fragments[fragment_name] = fragment
     badges = []
-    development_status = manifest.get('development_status', 'Beta').lower()
+    development_status = manifest.get("development_status", "Beta").lower()
     if development_status in DEVELOPMENT_STATUS_BADGES:
         badges.append(DEVELOPMENT_STATUS_BADGES[development_status])
-    license = manifest.get('license')
+    license = manifest.get("license")
     if license in LICENSE_BADGES:
         badges.append(LICENSE_BADGES[license])
     badges.append(make_repo_badge(org_name, repo_name, branch, addon_name))
     authors = [
         a.strip()
-        for a in manifest.get('author', '').split(',')
-        if '(OCA)' not in a
+        for a in manifest.get("author", "").split(",")
+        if "(OCA)" not in a
         # remove OCA because it's in authors for the purpose
         # of finding OCA addons in apps.odoo.com, OCA is not
         # a real author, but is rather referenced in the
         # maintainers section
     ]
     # generate
-    template_filename = \
-        os.path.join(os.path.dirname(__file__), 'gen_addon_readme.template')
-    readme_filename = \
-        os.path.join(addon_dir, 'README.rst')
-    with open(template_filename, 'r', encoding='utf8') as tf:
+    template_filename = os.path.join(
+        os.path.dirname(__file__), "gen_addon_readme.template"
+    )
+    readme_filename = os.path.join(addon_dir, "README.rst")
+    with open(template_filename, encoding="utf8") as tf:
         template = Template(tf.read())
-    with open(readme_filename, 'w', encoding='utf8') as rf:
-        rf.write(template.render(
-            addon_name=addon_name,
-            authors=authors,
-            badges=badges,
-            branch=branch,
-            fragments=fragments,
-            manifest=manifest,
-            org_name=org_name,
-            repo_name=repo_name,
-            development_status=development_status,
-        ))
+    with open(readme_filename, "w", encoding="utf8") as rf:
+        rf.write(
+            template.render(
+                addon_name=addon_name,
+                authors=authors,
+                badges=badges,
+                branch=branch,
+                fragments=fragments,
+                manifest=manifest,
+                org_name=org_name,
+                repo_name=repo_name,
+                development_status=development_status,
+            )
+        )
         # Agregar una linea en blanco al final del RST para que no falle el test
-        # W7908(missing-newline-extrafiles)
-        rf.write('\n')
+        # W7908(missing-newline-extrafiles).
+        rf.write("\n")
     return readme_filename
 
 
-
 @click.command()
 @click.option(
     "--org-name",
     required=True,
     help="Organization name",
 )
 @click.option(
@@ -255,22 +258,25 @@
 def gen_readme(org_name, repo_name, branch, addons_dir, gen_html):
     addons = list()
     if addons_dir:
         addons.extend(find_addons(addons_dir))
     readme_filenames = []
     for addon_name, addon_dir, manifest in addons:
         if not os.path.exists(
-                os.path.join(addon_dir, FRAGMENTS_DIR, 'DESCRIPTION.rst')):
+            os.path.join(addon_dir, FRAGMENTS_DIR, "DESCRIPTION.rst")
+        ):
             continue
         readme_filename = gen_one_addon_readme(
-            org_name, repo_name, branch, addon_name, addon_dir, manifest)
+            org_name, repo_name, branch, addon_name, addon_dir, manifest
+        )
         check_rst(readme_filename)
         readme_filenames.append(readme_filename)
         if gen_html:
-            if not manifest.get('preloadable', True):
+            if not manifest.get("preloadable", True):
                 continue
             index_filename = gen_one_addon_index(readme_filename)
             if index_filename:
                 readme_filenames.append(index_filename)
 
+
 if __name__ == "__main__":
     gen_readme()
```

### Comparing `gen-odoo-readme-0.1.0/tools/manifest.py` & `gen-odoo-readme-0.1.1/tools/manifest.py`

 * *Files identical despite different names*

