# Comparing `tmp/branthebuilder-1.0.8.tar.gz` & `tmp/branthebuilder-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "branthebuilder-1.0.8.tar", last modified: Wed Nov 23 23:43:40 2022, max compression
+gzip compressed data, was "branthebuilder-1.0.9.tar", last modified: Fri Dec 23 18:28:01 2022, max compression
```

## Comparing `branthebuilder-1.0.8.tar` & `branthebuilder-1.0.9.tar`

### file list

```diff
@@ -1,35 +1,37 @@
--rw-r--r--   0        0        0      859 2022-11-23 23:43:32.636621 branthebuilder-1.0.8/.github/workflows/test.yml
--rw-r--r--   0        0        0      565 2022-11-23 23:43:32.636621 branthebuilder-1.0.8/.github/workflows/twine_release.yml
--rw-r--r--   0        0        0     1770 2022-11-23 23:43:32.636621 branthebuilder-1.0.8/.gitignore
--rw-r--r--   0        0        0      287 2022-11-23 23:43:32.636621 branthebuilder-1.0.8/.readthedocs.yml
--rw-r--r--   0        0        0     1056 2022-11-23 23:43:32.636621 branthebuilder-1.0.8/LICENSE
--rw-r--r--   0        0        0      719 2022-11-23 23:43:32.636621 branthebuilder-1.0.8/README.md
--rw-r--r--   0        0        0       85 2022-11-23 23:43:32.636621 branthebuilder-1.0.8/branthebuilder/__init__.py
--rw-r--r--   0        0        0     5241 2022-11-23 23:43:32.636621 branthebuilder-1.0.8/branthebuilder/main.py
--rw-r--r--   0        0        0      587 2022-11-23 23:43:32.636621 branthebuilder-1.0.8/branthebuilder/nb_scripts.py
--rw-r--r--   0        0        0     1221 2022-11-23 23:43:32.636621 branthebuilder-1.0.8/branthebuilder/tests/test_integration.py
--rw-r--r--   0        0        0     1075 2022-11-23 23:43:32.636621 branthebuilder-1.0.8/branthebuilder/vars.py
--rw-r--r--   0        0        0       43 2022-11-23 23:43:32.636621 branthebuilder-1.0.8/docs/autosumm.rst
--rw-r--r--   0        0        0     2401 2022-11-23 23:43:32.636621 branthebuilder-1.0.8/docs/conf.py
--rw-r--r--   0        0        0      263 2022-11-23 23:43:32.636621 branthebuilder-1.0.8/docs/index.rst
--rw-r--r--   0        0        0       79 2022-11-23 23:43:32.636621 branthebuilder-1.0.8/docs/notebooks/doc-000-intro.rst
--rw-r--r--   0        0        0      102 2022-11-23 23:43:32.636621 branthebuilder-1.0.8/docs/release_notes/main.rst
--rw-r--r--   0        0        0       37 2022-11-23 23:43:32.636621 branthebuilder-1.0.8/docs/release_notes/v0.0.0.rst
--rw-r--r--   0        0        0       38 2022-11-23 23:43:32.636621 branthebuilder-1.0.8/docs/release_notes/v0.0.1.rst
--rw-r--r--   0        0        0       33 2022-11-23 23:43:32.636621 branthebuilder-1.0.8/docs/release_notes/v0.0.2.rst
--rw-r--r--   0        0        0       38 2022-11-23 23:43:32.636621 branthebuilder-1.0.8/docs/release_notes/v0.0.3.rst
--rw-r--r--   0        0        0       37 2022-11-23 23:43:32.636621 branthebuilder-1.0.8/docs/release_notes/v0.0.4.rst
--rw-r--r--   0        0        0       48 2022-11-23 23:43:32.636621 branthebuilder-1.0.8/docs/release_notes/v0.1.0.rst
--rw-r--r--   0        0        0       80 2022-11-23 23:43:32.636621 branthebuilder-1.0.8/docs/release_notes/v0.1.1.rst
--rw-r--r--   0        0        0       49 2022-11-23 23:43:32.636621 branthebuilder-1.0.8/docs/release_notes/v1.0.0.rst
--rw-r--r--   0        0        0       31 2022-11-23 23:43:32.636621 branthebuilder-1.0.8/docs/release_notes/v1.0.1.rst
--rw-r--r--   0        0        0       15 2022-11-23 23:43:32.636621 branthebuilder-1.0.8/docs/release_notes/v1.0.2.rst
--rw-r--r--   0        0        0       31 2022-11-23 23:43:32.636621 branthebuilder-1.0.8/docs/release_notes/v1.0.3.rst
--rw-r--r--   0        0        0       43 2022-11-23 23:43:32.636621 branthebuilder-1.0.8/docs/release_notes/v1.0.4.rst
--rw-r--r--   0        0        0       40 2022-11-23 23:43:32.636621 branthebuilder-1.0.8/docs/release_notes/v1.0.5.rst
--rw-r--r--   0        0        0       34 2022-11-23 23:43:32.636621 branthebuilder-1.0.8/docs/release_notes/v1.0.6.rst
--rw-r--r--   0        0        0       34 2022-11-23 23:43:32.636621 branthebuilder-1.0.8/docs/release_notes/v1.0.7.rst
--rw-r--r--   0        0        0       46 2022-11-23 23:43:32.636621 branthebuilder-1.0.8/docs/release_notes/v1.0.8.rst
--rw-r--r--   0        0        0      615 2022-11-23 23:43:32.636621 branthebuilder-1.0.8/notebooks/doc-000-intro.ipynb
--rw-r--r--   0        0        0      822 2022-11-23 23:43:32.636621 branthebuilder-1.0.8/pyproject.toml
--rw-r--r--   0        0        0     1593 1970-01-01 00:00:00.000000 branthebuilder-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0      859 2022-12-23 18:27:57.890702 branthebuilder-1.0.9/.github/workflows/test.yml
+-rw-r--r--   0        0        0      565 2022-12-23 18:27:57.890702 branthebuilder-1.0.9/.github/workflows/twine_release.yml
+-rw-r--r--   0        0        0     1770 2022-12-23 18:27:57.890702 branthebuilder-1.0.9/.gitignore
+-rw-r--r--   0        0        0      287 2022-12-23 18:27:57.890702 branthebuilder-1.0.9/.readthedocs.yml
+-rw-r--r--   0        0        0      310 2022-12-23 18:27:57.890702 branthebuilder-1.0.9/CITATION.cff
+-rw-r--r--   0        0        0     1056 2022-12-23 18:27:57.890702 branthebuilder-1.0.9/LICENSE
+-rw-r--r--   0        0        0      719 2022-12-23 18:27:57.890702 branthebuilder-1.0.9/README.md
+-rw-r--r--   0        0        0       85 2022-12-23 18:27:57.890702 branthebuilder-1.0.9/branthebuilder/__init__.py
+-rw-r--r--   0        0        0     6492 2022-12-23 18:27:57.890702 branthebuilder-1.0.9/branthebuilder/main.py
+-rw-r--r--   0        0        0      587 2022-12-23 18:27:57.890702 branthebuilder-1.0.9/branthebuilder/nb_scripts.py
+-rw-r--r--   0        0        0     1239 2022-12-23 18:27:57.890702 branthebuilder-1.0.9/branthebuilder/tests/test_integration.py
+-rw-r--r--   0        0        0     1136 2022-12-23 18:27:57.890702 branthebuilder-1.0.9/branthebuilder/vars.py
+-rw-r--r--   0        0        0       43 2022-12-23 18:27:57.890702 branthebuilder-1.0.9/docs/autosumm.rst
+-rw-r--r--   0        0        0     2401 2022-12-23 18:27:57.890702 branthebuilder-1.0.9/docs/conf.py
+-rw-r--r--   0        0        0      263 2022-12-23 18:27:57.890702 branthebuilder-1.0.9/docs/index.rst
+-rw-r--r--   0        0        0       79 2022-12-23 18:27:57.890702 branthebuilder-1.0.9/docs/notebooks/doc-000-intro.rst
+-rw-r--r--   0        0        0      102 2022-12-23 18:27:57.890702 branthebuilder-1.0.9/docs/release_notes/main.rst
+-rw-r--r--   0        0        0       37 2022-12-23 18:27:57.894702 branthebuilder-1.0.9/docs/release_notes/v0.0.0.rst
+-rw-r--r--   0        0        0       38 2022-12-23 18:27:57.894702 branthebuilder-1.0.9/docs/release_notes/v0.0.1.rst
+-rw-r--r--   0        0        0       33 2022-12-23 18:27:57.894702 branthebuilder-1.0.9/docs/release_notes/v0.0.2.rst
+-rw-r--r--   0        0        0       38 2022-12-23 18:27:57.894702 branthebuilder-1.0.9/docs/release_notes/v0.0.3.rst
+-rw-r--r--   0        0        0       37 2022-12-23 18:27:57.894702 branthebuilder-1.0.9/docs/release_notes/v0.0.4.rst
+-rw-r--r--   0        0        0       48 2022-12-23 18:27:57.894702 branthebuilder-1.0.9/docs/release_notes/v0.1.0.rst
+-rw-r--r--   0        0        0       80 2022-12-23 18:27:57.894702 branthebuilder-1.0.9/docs/release_notes/v0.1.1.rst
+-rw-r--r--   0        0        0       49 2022-12-23 18:27:57.894702 branthebuilder-1.0.9/docs/release_notes/v1.0.0.rst
+-rw-r--r--   0        0        0       31 2022-12-23 18:27:57.894702 branthebuilder-1.0.9/docs/release_notes/v1.0.1.rst
+-rw-r--r--   0        0        0       15 2022-12-23 18:27:57.894702 branthebuilder-1.0.9/docs/release_notes/v1.0.2.rst
+-rw-r--r--   0        0        0       31 2022-12-23 18:27:57.894702 branthebuilder-1.0.9/docs/release_notes/v1.0.3.rst
+-rw-r--r--   0        0        0       43 2022-12-23 18:27:57.894702 branthebuilder-1.0.9/docs/release_notes/v1.0.4.rst
+-rw-r--r--   0        0        0       40 2022-12-23 18:27:57.894702 branthebuilder-1.0.9/docs/release_notes/v1.0.5.rst
+-rw-r--r--   0        0        0       34 2022-12-23 18:27:57.894702 branthebuilder-1.0.9/docs/release_notes/v1.0.6.rst
+-rw-r--r--   0        0        0       34 2022-12-23 18:27:57.894702 branthebuilder-1.0.9/docs/release_notes/v1.0.7.rst
+-rw-r--r--   0        0        0       46 2022-12-23 18:27:57.894702 branthebuilder-1.0.9/docs/release_notes/v1.0.8.rst
+-rw-r--r--   0        0        0       33 2022-12-23 18:27:57.894702 branthebuilder-1.0.9/docs/release_notes/v1.0.9.rst
+-rw-r--r--   0        0        0      615 2022-12-23 18:27:57.894702 branthebuilder-1.0.9/notebooks/doc-000-intro.ipynb
+-rw-r--r--   0        0        0      835 2022-12-23 18:27:57.894702 branthebuilder-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1615 1970-01-01 00:00:00.000000 branthebuilder-1.0.9/PKG-INFO
```

### Comparing `branthebuilder-1.0.8/.github/workflows/test.yml` & `branthebuilder-1.0.9/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `branthebuilder-1.0.8/.github/workflows/twine_release.yml` & `branthebuilder-1.0.9/.github/workflows/twine_release.yml`

 * *Files identical despite different names*

### Comparing `branthebuilder-1.0.8/.gitignore` & `branthebuilder-1.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `branthebuilder-1.0.8/LICENSE` & `branthebuilder-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `branthebuilder-1.0.8/README.md` & `branthebuilder-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `branthebuilder-1.0.8/branthebuilder/main.py` & `branthebuilder-1.0.9/branthebuilder/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,22 @@
+import datetime as dt
+import json
 import os
 import sys
 from pathlib import Path
 from shutil import rmtree
 from subprocess import check_call, check_output
 from warnings import warn
 
 import typer
+import yaml
 from cookiecutter.main import cookiecutter
 
 from .nb_scripts import get_nb_scripts, get_notebooks, nb_dir
-from .vars import cc_repo, conf, docdir
+from .vars import CFF_PATH, ORCID_DIC_ENV, cc_repo, conf, docdir
 
 app = typer.Typer()
 
 
 class SetupException(Exception):
     pass
 
@@ -141,20 +144,52 @@
         raise SetupException(f"{tag_version} version already tagged")
     if Path(docdir).exists():
         note_rst = f"{tag_version}\n---------------------\n\n" + msg
         Path(docdir, "release_notes", f"{tag_version}.rst").write_text(note_rst)
         build_docs()
         check_call(["git", "add", "docs"])
         check_call(["git", "commit", "-m", f"docs for {tag_version}"])
+    if CFF_PATH.exists():
+        cff_dic = yaml.safe_load(CFF_PATH.read_text())
+        cff_dic["version"] = conf.version
+        cff_dic["date-released"] = dt.date.today()
+        _dump_cff(cff_dic)
+        check_call(["git", "add", CFF_PATH.as_posix()])
+        check_call(["git", "commit", "-m", f"update cff {tag_version}"])
 
     check_call(["git", "tag", "-a", tag_version, "-m", msg])
     check_call(["git", "push"])
     check_call(["git", "push", "origin", tag_version])
 
 
+@app.command()
+def init_cff():
+    proj = conf.pytom["project"]
+    url = proj["urls"]["Homepage"]
+    cff_dic = {
+        "cff-version": "1.2.0",
+        "message": "If you use this software, please cite it as below.",
+        "url": url,
+        "authors": [],
+        "title": "/".join(url.split("/")[-2:]),
+        # TODO: "doi": "10.5281/zenodo.1234",
+    }
+
+    orcid_dic = json.loads(os.environ.get(ORCID_DIC_ENV, "{}"))
+    for author in proj["authors"]:
+        names = author["name"].split()
+        adic = {"family-names": names[-1], "given-names": " ".join(names[:-1])}
+        orcid = orcid_dic.get(author["name"])
+        if orcid:
+            adic["orcid"] = orcid
+        cff_dic["authors"].append(adic)
+
+    _dump_cff(cff_dic)
+
+
 def _get_branch():
     comm = ["git", "rev-parse", "--abbrev-ref", "HEAD"]
     return check_output(comm).strip().decode("utf-8")
 
 
 def _cleanup(leave_docs, leave_actions, leave_notebooks, single_file):
     if not leave_docs:
@@ -172,7 +207,11 @@
 
 
 def _no_tb_call(args):
     try:
         check_call(args)
     except Exception:
         sys.exit(1)
+
+
+def _dump_cff(dic):
+    CFF_PATH.write_text(yaml.safe_dump(dic, allow_unicode=True, sort_keys=False))
```

### Comparing `branthebuilder-1.0.8/branthebuilder/nb_scripts.py` & `branthebuilder-1.0.9/branthebuilder/nb_scripts.py`

 * *Files identical despite different names*

### Comparing `branthebuilder-1.0.8/branthebuilder/tests/test_integration.py` & `branthebuilder-1.0.9/branthebuilder/tests/test_integration.py`

 * *Files 14% similar despite different names*

```diff
@@ -28,14 +28,15 @@
             f.write(DOCTESTED_FUN)
 
     check_call(["git", "remote", "add", "origin", "../remote"])
     check_call(["git", "push", "--set-upstream", "origin", "main"])
     sys.path.insert(0, Path(tmp_path, "testproject").as_posix())
     ns.lint()
     ns.test(True, True, True)
+    ns.init_cff()
     ns.tag("tag msg")
     check_call(["flit", "build"])
     ns.update_boilerplate(True)
 
 
 def test_errs(tmp_path):
     os.chdir(tmp_path)
```

### Comparing `branthebuilder-1.0.8/branthebuilder/vars.py` & `branthebuilder-1.0.9/branthebuilder/vars.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import importlib
 from pathlib import Path
 from warnings import warn
 
 import toml
 
+CFF_PATH = Path("CITATION.cff")
+ORCID_DIC_ENV = "ORCID_MAP"
+
 docdir = "docs"
 cc_repo = "https://github.com/endremborza/python-boilerplate-v2"
 
 _D = {"project": {"name": ".", "author": []}, "tool": {"branb": {"line-length": 88}}}
 
 
 class PackageConf:
```

### Comparing `branthebuilder-1.0.8/docs/conf.py` & `branthebuilder-1.0.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `branthebuilder-1.0.8/notebooks/doc-000-intro.ipynb` & `branthebuilder-1.0.9/notebooks/doc-000-intro.ipynb`

 * *Files identical despite different names*

### Comparing `branthebuilder-1.0.8/pyproject.toml` & `branthebuilder-1.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     "pytest",
     "pytest-cov",
     "codecov",
     "toml",
     "flake8",
     "isort",
     "cookiecutter",
+    "pyyaml"
 ]
 
 [project.optional-dependencies]
 test = []
 doc = [
     "sphinx",
     "graphviz",
```

### Comparing `branthebuilder-1.0.8/PKG-INFO` & `branthebuilder-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: branthebuilder
-Version: 1.0.8
+Version: 1.0.9
 Summary: Python package management
 Author-email: Endre Márk Borza <endremborza@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: typer
 Requires-Dist: flit
 Requires-Dist: jupyter
@@ -12,14 +12,15 @@
 Requires-Dist: pytest
 Requires-Dist: pytest-cov
 Requires-Dist: codecov
 Requires-Dist: toml
 Requires-Dist: flake8
 Requires-Dist: isort
 Requires-Dist: cookiecutter
+Requires-Dist: pyyaml
 Requires-Dist: sphinx ; extra == "doc"
 Requires-Dist: graphviz ; extra == "doc"
 Requires-Dist: pandoc ; extra == "doc"
 Requires-Dist: sphinx-automodapi ; extra == "doc"
 Requires-Dist: sphinx-rtd-theme ; extra == "doc"
 Requires-Dist: myst-parser ; extra == "doc"
 Requires-Dist: pygments ; extra == "doc"
```

