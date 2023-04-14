# Comparing `tmp/useq_schema-0.2.0.tar.gz` & `tmp/useq_schema-0.2.1.tar.gz`

## Comparing `useq_schema-0.2.0.tar` & `useq_schema-0.2.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 useq_schema-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2197 2020-02-02 00:00:00.000000 useq_schema-0.2.0/mkdocs.yml
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 useq_schema-0.2.0/setup.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 useq_schema-0.2.0/.github/dependabot.yml
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 useq_schema-0.2.0/.github/workflows/docs.yml
--rw-r--r--   0        0        0     2742 2020-02-02 00:00:00.000000 useq_schema-0.2.0/.github/workflows/test_and_deploy.yml
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 useq_schema-0.2.0/docs/api.md
--rw-r--r--   0        0        0     7341 2020-02-02 00:00:00.000000 useq_schema-0.2.0/docs/index.md
--rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 useq_schema-0.2.0/docs/images/favicon.ico
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 useq_schema-0.2.0/docs/schema/axes.md
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 useq_schema-0.2.0/docs/schema/event.md
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 useq_schema-0.2.0/docs/schema/sequence.md
--rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 useq_schema-0.2.0/docs/stylesheets/extra.css
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 useq_schema-0.2.0/src/useq/__init__.py
--rw-r--r--   0        0        0     5684 2020-02-02 00:00:00.000000 useq_schema-0.2.0/src/useq/_base_model.py
--rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 useq_schema-0.2.0/src/useq/_channel.py
--rw-r--r--   0        0        0     7730 2020-02-02 00:00:00.000000 useq_schema-0.2.0/src/useq/_grid.py
--rw-r--r--   0        0        0     5911 2020-02-02 00:00:00.000000 useq_schema-0.2.0/src/useq/_mda_event.py
--rw-r--r--   0        0        0    19468 2020-02-02 00:00:00.000000 useq_schema-0.2.0/src/useq/_mda_sequence.py
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 useq_schema-0.2.0/src/useq/_position.py
--rw-r--r--   0        0        0     3882 2020-02-02 00:00:00.000000 useq_schema-0.2.0/src/useq/_time.py
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 useq_schema-0.2.0/src/useq/_utils.py
--rw-r--r--   0        0        0     3867 2020-02-02 00:00:00.000000 useq_schema-0.2.0/src/useq/_z.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 useq_schema-0.2.0/src/useq/py.typed
--rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 useq_schema-0.2.0/tests/conftest.py
--rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 useq_schema-0.2.0/tests/test_grid.py
--rw-r--r--   0        0        0    23284 2020-02-02 00:00:00.000000 useq_schema-0.2.0/tests/test_position_sequence.py
--rw-r--r--   0        0        0    10315 2020-02-02 00:00:00.000000 useq_schema-0.2.0/tests/test_sequence.py
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 useq_schema-0.2.0/tests/test_serialization.py
--rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 useq_schema-0.2.0/tests/fixtures/mda.json
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 useq_schema-0.2.0/tests/fixtures/mda.yaml
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 useq_schema-0.2.0/.gitignore
--rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 useq_schema-0.2.0/LICENSE
--rw-r--r--   0        0        0     7746 2020-02-02 00:00:00.000000 useq_schema-0.2.0/README.md
--rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 useq_schema-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     9574 2020-02-02 00:00:00.000000 useq_schema-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 useq_schema-0.2.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2197 2020-02-02 00:00:00.000000 useq_schema-0.2.1/mkdocs.yml
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 useq_schema-0.2.1/setup.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 useq_schema-0.2.1/.github/dependabot.yml
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 useq_schema-0.2.1/.github/workflows/docs.yml
+-rw-r--r--   0        0        0     2742 2020-02-02 00:00:00.000000 useq_schema-0.2.1/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 useq_schema-0.2.1/docs/api.md
+-rw-r--r--   0        0        0     7341 2020-02-02 00:00:00.000000 useq_schema-0.2.1/docs/index.md
+-rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 useq_schema-0.2.1/docs/images/favicon.ico
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 useq_schema-0.2.1/docs/schema/axes.md
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 useq_schema-0.2.1/docs/schema/event.md
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 useq_schema-0.2.1/docs/schema/sequence.md
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 useq_schema-0.2.1/docs/stylesheets/extra.css
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 useq_schema-0.2.1/src/useq/__init__.py
+-rw-r--r--   0        0        0     5728 2020-02-02 00:00:00.000000 useq_schema-0.2.1/src/useq/_base_model.py
+-rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 useq_schema-0.2.1/src/useq/_channel.py
+-rw-r--r--   0        0        0     7730 2020-02-02 00:00:00.000000 useq_schema-0.2.1/src/useq/_grid.py
+-rw-r--r--   0        0        0     5911 2020-02-02 00:00:00.000000 useq_schema-0.2.1/src/useq/_mda_event.py
+-rw-r--r--   0        0        0    19634 2020-02-02 00:00:00.000000 useq_schema-0.2.1/src/useq/_mda_sequence.py
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 useq_schema-0.2.1/src/useq/_position.py
+-rw-r--r--   0        0        0     3882 2020-02-02 00:00:00.000000 useq_schema-0.2.1/src/useq/_time.py
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 useq_schema-0.2.1/src/useq/_utils.py
+-rw-r--r--   0        0        0     3867 2020-02-02 00:00:00.000000 useq_schema-0.2.1/src/useq/_z.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 useq_schema-0.2.1/src/useq/py.typed
+-rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 useq_schema-0.2.1/tests/conftest.py
+-rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 useq_schema-0.2.1/tests/test_grid.py
+-rw-r--r--   0        0        0    23284 2020-02-02 00:00:00.000000 useq_schema-0.2.1/tests/test_position_sequence.py
+-rw-r--r--   0        0        0    10315 2020-02-02 00:00:00.000000 useq_schema-0.2.1/tests/test_sequence.py
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 useq_schema-0.2.1/tests/test_serialization.py
+-rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 useq_schema-0.2.1/tests/fixtures/mda.json
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 useq_schema-0.2.1/tests/fixtures/mda.yaml
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 useq_schema-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 useq_schema-0.2.1/LICENSE
+-rw-r--r--   0        0        0     7746 2020-02-02 00:00:00.000000 useq_schema-0.2.1/README.md
+-rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 useq_schema-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     9578 2020-02-02 00:00:00.000000 useq_schema-0.2.1/PKG-INFO
```

### Comparing `useq_schema-0.2.0/.pre-commit-config.yaml` & `useq_schema-0.2.1/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -18,30 +18,30 @@
       - id: check-docstring-first
       - id: end-of-file-fixer
       - id: trailing-whitespace
       - id: pretty-format-json
         args: ["--autofix"]
 
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.254
+    rev: v0.0.261
     hooks:
       - id: ruff
         args: [--fix]
 
   - repo: https://github.com/psf/black
-    rev: 23.1.0
+    rev: 23.3.0
     hooks:
       - id: black
 
   - repo: https://github.com/abravalheri/validate-pyproject
-    rev: v0.12.1
+    rev: v0.12.2
     hooks:
       - id: validate-pyproject
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.0.1
+    rev: v1.1.1
     hooks:
       - id: mypy
         additional_dependencies:
           - types-PyYAML
           - pydantic
         files: "^src/"
```

### Comparing `useq_schema-0.2.0/mkdocs.yml` & `useq_schema-0.2.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `useq_schema-0.2.0/setup.py` & `useq_schema-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.2.0/.github/workflows/test_and_deploy.yml` & `useq_schema-0.2.1/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `useq_schema-0.2.0/docs/api.md` & `useq_schema-0.2.1/docs/api.md`

 * *Files identical despite different names*

### Comparing `useq_schema-0.2.0/docs/index.md` & `useq_schema-0.2.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `useq_schema-0.2.0/docs/images/favicon.ico` & `useq_schema-0.2.1/docs/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `useq_schema-0.2.0/docs/schema/axes.md` & `useq_schema-0.2.1/docs/schema/axes.md`

 * *Files identical despite different names*

### Comparing `useq_schema-0.2.0/docs/stylesheets/extra.css` & `useq_schema-0.2.1/docs/stylesheets/extra.css`

 * *Files identical despite different names*

### Comparing `useq_schema-0.2.0/src/useq/__init__.py` & `useq_schema-0.2.1/src/useq/__init__.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.2.0/src/useq/_base_model.py` & `useq_schema-0.2.1/src/useq/_base_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,17 @@
 
     @root_validator(pre=False, skip_on_failure=True)
     def _validate_kwargs(cls, values: Dict[str, Any]) -> Dict[str, Any]:
         """Validate kwargs for MDASequence."""
         extra_kwargs = set(values) - set(cls.__fields__)
         if extra_kwargs:
             name = getattr(cls, "__name__", "")
-            warnings.warn(f"{name} got unknown keyword arguments: {extra_kwargs}")
+            warnings.warn(
+                f"{name} got unknown keyword arguments: {extra_kwargs}", stacklevel=2
+            )
             for k in extra_kwargs:
                 values.pop(k)
         return values
 
 
 class UseqModel(FrozenModel):
     def __repr_args__(self) -> ReprArgs:
```

### Comparing `useq_schema-0.2.0/src/useq/_channel.py` & `useq_schema-0.2.1/src/useq/_channel.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.2.0/src/useq/_grid.py` & `useq_schema-0.2.1/src/useq/_grid.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.2.0/src/useq/_mda_event.py` & `useq_schema-0.2.1/src/useq/_mda_event.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.2.0/src/useq/_mda_sequence.py` & `useq_schema-0.2.1/src/useq/_mda_sequence.py`

 * *Files 1% similar despite different names*

```diff
@@ -232,29 +232,34 @@
             CHANNEL in order
             and TIME in order
             and any(c.acquire_every > 1 for c in channels)
             and order.index(CHANNEL) < order.index(TIME)
         ):
             warn(
                 f"Channels with skipped frames detected, but {CHANNEL!r} precedes "
-                "{TIME!r} in the acquisition order: may not yield intended results."
+                "{TIME!r} in the acquisition order: may not yield intended results.",
+                stacklevel=2,
             )
 
         if (
             GRID in order
             and POSITION in order
-            and grid_plan
+            and grid_plan is not None
+            and not isinstance(grid_plan, NoGrid)
             and not grid_plan.is_relative
             and len(stage_positions) > 1
         ):
             sub_position_grid_plans = [
                 p for p in stage_positions if p.sequence and p.sequence.grid_plan
             ]
             if len(stage_positions) - len(sub_position_grid_plans) > 1:
-                warn("Global grid plan will override sub-position grid plans.")
+                warn(
+                    "Global grid plan will override sub-position grid plans.",
+                    stacklevel=2,
+                )
 
         if (
             POSITION in order
             and stage_positions
             and any(p.sequence.stage_positions for p in stage_positions if p.sequence)
         ):
             raise ValueError(
```

### Comparing `useq_schema-0.2.0/src/useq/_position.py` & `useq_schema-0.2.1/src/useq/_position.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.2.0/src/useq/_time.py` & `useq_schema-0.2.1/src/useq/_time.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.2.0/src/useq/_utils.py` & `useq_schema-0.2.1/src/useq/_utils.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.2.0/src/useq/_z.py` & `useq_schema-0.2.1/src/useq/_z.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.2.0/tests/conftest.py` & `useq_schema-0.2.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.2.0/tests/test_grid.py` & `useq_schema-0.2.1/tests/test_grid.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.2.0/tests/test_position_sequence.py` & `useq_schema-0.2.1/tests/test_position_sequence.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.2.0/tests/test_sequence.py` & `useq_schema-0.2.1/tests/test_sequence.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.2.0/tests/fixtures/mda.json` & `useq_schema-0.2.1/tests/fixtures/mda.json`

 * *Files identical despite different names*

### Comparing `useq_schema-0.2.0/tests/fixtures/mda.yaml` & `useq_schema-0.2.1/tests/fixtures/mda.yaml`

 * *Files identical despite different names*

### Comparing `useq_schema-0.2.0/.gitignore` & `useq_schema-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `useq_schema-0.2.0/LICENSE` & `useq_schema-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `useq_schema-0.2.0/README.md` & `useq_schema-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `useq_schema-0.2.0/pyproject.toml` & `useq_schema-0.2.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     "Programming Language :: Python :: 3 :: Only",
     "Topic :: Scientific/Engineering",
     "Topic :: Scientific/Engineering :: Medical Science Apps.",
     "Topic :: Scientific/Engineering :: Image Processing",
     "Topic :: Software Development",
 ]
 dynamic = ["version"]
-dependencies = ["pydantic", "numpy"]
+dependencies = ["pydantic<2.0", "numpy"]
 
 # extras
 # https://peps.python.org/pep-0621/#dependencies-optional-dependencies
 [project.optional-dependencies]
 yaml = ["PyYAML"]
 test = ["pytest>=6.0", "pytest-cov", "PyYAML"]
 dev = [
@@ -41,19 +41,15 @@
     "pre-commit",
     "pytest-cov",
     "pytest",
     "rich",
     "ruff",
     "PyYaml",
 ]
-docs = [
-    "mkdocs >=1.4",
-    "mkdocs-material",
-    "mkdocstrings-python",
-]
+docs = ["mkdocs >=1.4", "mkdocs-material", "mkdocstrings-python"]
 
 [project.urls]
 Source = "https://github.com/pymmcore-plus/useq-schema"
 Tracker = "https://github.com/pymmcore-plus/useq-schema/issues"
 
 # https://hatch.pypa.io/latest/config/metadata/
 [tool.hatch.version]
@@ -70,22 +66,21 @@
 src = ["src", "tests"]
 select = [
     "E",    # style errors
     "F",    # flakes
     "D",    # pydocstyle
     "I",    # isort
     "UP",   # pyupgrade
-    # "N",  # pep8-naming
     "S",    # bandit
-    "C",    # comprehensions
+    "C4",   # comprehensions
     "B",    # bugbear
     "A001", # Variable shadowing a python builtin
     "RUF",  # ruff-specific rules
 ]
-extend-ignore = [
+ignore = [
     "D100", # Missing docstring in public module
     "D104", # Missing docstring in public package
     "D107", # Missing docstring in __init__
     "D203", # 1 blank line required before class docstring
     "D212", # Multi-line docstring summary should start at the first line
     "D213", # Multi-line docstring summary should start at the second line
     "D401", # Imperative mood
@@ -110,15 +105,15 @@
 [tool.mypy]
 files = "src/**/"
 strict = true
 disallow_any_generics = false
 disallow_subclassing_any = false
 show_error_codes = true
 pretty = true
-
+plugins = ["pydantic.mypy"]
 
 # https://coverage.readthedocs.io/en/6.4/config.html
 [tool.coverage.report]
 exclude_lines = [
     "pragma: no cover",
     "if TYPE_CHECKING:",
     "@overload",
@@ -130,9 +125,9 @@
 [tool.check-manifest]
 ignore = [
     ".github_changelog_generator",
     ".pre-commit-config.yaml",
     ".ruff_cache/**/*",
     "tests/**/*",
     "tox.ini",
-    "setup.py"
+    "setup.py",
 ]
```

### Comparing `useq_schema-0.2.0/PKG-INFO` & `useq_schema-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: useq-schema
-Version: 0.2.0
+Version: 0.2.1
 Summary: Schema for multi-dimensional microscopy experiments
 Project-URL: Source, https://github.com/pymmcore-plus/useq-schema
 Project-URL: Tracker, https://github.com/pymmcore-plus/useq-schema/issues
 Author-email: Talley Lambert <talley.lambert@gmail.com>
 License: BSD 3-Clause License
 License-File: LICENSE
 Keywords: microscopy,schema
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Classifier: Topic :: Software Development
 Requires-Python: >=3.7
 Requires-Dist: numpy
-Requires-Dist: pydantic
+Requires-Dist: pydantic<2.0
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: ipython; extra == 'dev'
 Requires-Dist: mypy; extra == 'dev'
 Requires-Dist: pdbpp; extra == 'dev'
 Requires-Dist: pre-commit; extra == 'dev'
 Requires-Dist: pytest; extra == 'dev'
```

