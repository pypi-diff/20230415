# Comparing `tmp/osintbuddy-0.0.2rc13.post1.tar.gz` & `tmp/osintbuddy-0.0.2rc14.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osintbuddy-0.0.2rc13.post1.tar", last modified: Sat Apr 15 16:54:25 2023, max compression
+gzip compressed data, was "osintbuddy-0.0.2rc14.post1.tar", last modified: Sat Apr 15 16:57:01 2023, max compression
```

## Comparing `osintbuddy-0.0.2rc13.post1.tar` & `osintbuddy-0.0.2rc14.post1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      274 2023-04-15 16:54:21.785703 osintbuddy-0.0.2rc13.post1/.github/dependabot.yml
--rw-r--r--   0        0        0      447 2023-04-15 16:54:21.785703 osintbuddy-0.0.2rc13.post1/.github/workflows/CI.yml
--rw-r--r--   0        0        0      263 2023-04-15 16:54:21.785703 osintbuddy-0.0.2rc13.post1/.github/workflows/publish.yml
--rw-r--r--   0        0        0      314 2023-04-15 16:54:21.785703 osintbuddy-0.0.2rc13.post1/.github/workflows/semantic-pr-check.yml
--rw-r--r--   0        0        0     1807 2023-04-15 16:54:21.785703 osintbuddy-0.0.2rc13.post1/.gitignore
--rw-r--r--   0        0        0     1540 2023-04-15 16:54:21.785703 osintbuddy-0.0.2rc13.post1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      158 2023-04-15 16:54:21.785703 osintbuddy-0.0.2rc13.post1/.pypirc
--rw-r--r--   0        0        0      444 2023-04-15 16:54:21.785703 osintbuddy-0.0.2rc13.post1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      316 2023-04-15 16:54:21.785703 osintbuddy-0.0.2rc13.post1/Dockerfile
--rw-r--r--   0        0        0       11 2023-04-15 16:54:21.785703 osintbuddy-0.0.2rc13.post1/LICENSE
--rw-r--r--   0        0        0     7534 2023-04-15 16:54:21.785703 osintbuddy-0.0.2rc13.post1/README.md
--rw-r--r--   0        0        0       47 2023-04-15 16:54:21.789703 osintbuddy-0.0.2rc13.post1/docs/developer.md
--rw-r--r--   0        0        0      471 2023-04-15 16:54:21.789703 osintbuddy-0.0.2rc13.post1/docs/pre-commit-config.md
--rw-r--r--   0        0        0    16088 2023-04-15 16:54:21.789703 osintbuddy-0.0.2rc13.post1/docs/pylint.md
--rw-r--r--   0        0        0      497 2023-04-15 16:54:21.789703 osintbuddy-0.0.2rc13.post1/docs/pyproject.md
--rw-r--r--   0        0        0      208 2023-04-15 16:54:21.789703 osintbuddy-0.0.2rc13.post1/docs/workflows.md
--rw-r--r--   0        0        0     6635 2023-04-15 16:54:21.789703 osintbuddy-0.0.2rc13.post1/pyproject.toml
--rw-r--r--   0        0        0      251 2023-04-15 16:54:21.789703 osintbuddy-0.0.2rc13.post1/src/README.md
--rw-r--r--   0        0        0      374 2023-04-15 16:54:24.681748 osintbuddy-0.0.2rc13.post1/src/osintbuddy/__init__.py
--rw-r--r--   0        0        0      454 2023-04-15 16:54:21.789703 osintbuddy-0.0.2rc13.post1/src/osintbuddy/plugins.py
--rw-r--r--   0        0        0      989 2023-04-15 16:54:21.789703 osintbuddy-0.0.2rc13.post1/tests/conftest.py
--rw-r--r--   0        0        0      715 2023-04-15 16:54:21.789703 osintbuddy-0.0.2rc13.post1/tests/test_methods.py
--rw-r--r--   0        0        0     9374 1970-01-01 00:00:00.000000 osintbuddy-0.0.2rc13.post1/PKG-INFO
+-rw-r--r--   0        0        0      274 2023-04-15 16:56:56.890528 osintbuddy-0.0.2rc14.post1/.github/dependabot.yml
+-rw-r--r--   0        0        0      447 2023-04-15 16:56:56.890528 osintbuddy-0.0.2rc14.post1/.github/workflows/CI.yml
+-rw-r--r--   0        0        0      263 2023-04-15 16:56:56.890528 osintbuddy-0.0.2rc14.post1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      314 2023-04-15 16:56:56.890528 osintbuddy-0.0.2rc14.post1/.github/workflows/semantic-pr-check.yml
+-rw-r--r--   0        0        0     1807 2023-04-15 16:56:56.890528 osintbuddy-0.0.2rc14.post1/.gitignore
+-rw-r--r--   0        0        0     1540 2023-04-15 16:56:56.890528 osintbuddy-0.0.2rc14.post1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      158 2023-04-15 16:56:56.890528 osintbuddy-0.0.2rc14.post1/.pypirc
+-rw-r--r--   0        0        0      444 2023-04-15 16:56:56.890528 osintbuddy-0.0.2rc14.post1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      316 2023-04-15 16:56:56.890528 osintbuddy-0.0.2rc14.post1/Dockerfile
+-rw-r--r--   0        0        0       11 2023-04-15 16:56:56.890528 osintbuddy-0.0.2rc14.post1/LICENSE
+-rw-r--r--   0        0        0     5859 2023-04-15 16:56:56.890528 osintbuddy-0.0.2rc14.post1/README.md
+-rw-r--r--   0        0        0       47 2023-04-15 16:56:56.890528 osintbuddy-0.0.2rc14.post1/docs/developer.md
+-rw-r--r--   0        0        0      471 2023-04-15 16:56:56.890528 osintbuddy-0.0.2rc14.post1/docs/pre-commit-config.md
+-rw-r--r--   0        0        0    16088 2023-04-15 16:56:56.890528 osintbuddy-0.0.2rc14.post1/docs/pylint.md
+-rw-r--r--   0        0        0      497 2023-04-15 16:56:56.890528 osintbuddy-0.0.2rc14.post1/docs/pyproject.md
+-rw-r--r--   0        0        0      208 2023-04-15 16:56:56.890528 osintbuddy-0.0.2rc14.post1/docs/workflows.md
+-rw-r--r--   0        0        0     6635 2023-04-15 16:56:56.890528 osintbuddy-0.0.2rc14.post1/pyproject.toml
+-rw-r--r--   0        0        0      251 2023-04-15 16:56:56.890528 osintbuddy-0.0.2rc14.post1/src/README.md
+-rw-r--r--   0        0        0      374 2023-04-15 16:57:00.694547 osintbuddy-0.0.2rc14.post1/src/osintbuddy/__init__.py
+-rw-r--r--   0        0        0      454 2023-04-15 16:56:56.890528 osintbuddy-0.0.2rc14.post1/src/osintbuddy/plugins.py
+-rw-r--r--   0        0        0      989 2023-04-15 16:56:56.890528 osintbuddy-0.0.2rc14.post1/tests/conftest.py
+-rw-r--r--   0        0        0      715 2023-04-15 16:56:56.890528 osintbuddy-0.0.2rc14.post1/tests/test_methods.py
+-rw-r--r--   0        0        0     7699 1970-01-01 00:00:00.000000 osintbuddy-0.0.2rc14.post1/PKG-INFO
```

### Comparing `osintbuddy-0.0.2rc13.post1/.gitignore` & `osintbuddy-0.0.2rc14.post1/.gitignore`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.2rc13.post1/.pre-commit-config.yaml` & `osintbuddy-0.0.2rc14.post1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.2rc13.post1/README.md` & `osintbuddy-0.0.2rc14.post1/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,29 +1,30 @@
-# OSINTBuddy
+# OSINTBuddy plugins and extensions
+
+The plugins library for [jerlendds/osintbuddy](https://github.com/jerlendds/osintbuddy), coming soon...
+
 
 This project follows the Python Standards declared in PEP 621. It uses a pyproject.yaml file to configure the project and Flit to simplify the build process and publish to PyPI. Flit simplifies the build and packaging process for Python projects by eliminating the need for separate setup.py and setup.cfg files. With Flit, you can manage all relevant configurations within the pyproject.toml file, streamlining development and promoting maintainability by centralizing project metadata, dependencies, and build specifications in one place.
 
+## Extending OSINTBuddy with extension/plugins
+
+@todo
+
+## Creating a plugin with dependent plugins...
+
+@todo
+
+
 ## Project Organization
 
 - `.github/workflows`: Contains GitHub Actions used for building, testing, and publishing.
-- `.devcontainer/Dockerfile`: Contains Dockerfile to build a development container for VSCode with all the necessary extensions for Python development installed.
-- `.devcontainer/devcontainer.json`: Contains the configuration for the development container for VSCode, including the Docker image to use, any additional VSCode extensions to install, and whether or not to mount the project directory into the container.
-- `.vscode/settings.json`: Contains VSCode settings specific to the project, such as the Python interpreter to use and the maximum line length for auto-formatting.
 - `src`: Place new source code here.
 - `tests`: Contains Python-based test cases to validate source code.
 - `pyproject.toml`: Contains metadata about the project and configurations for additional tools used to format, lint, type-check, and analyze Python code.
 
-### `pyproject.toml`
-
-The pyproject.toml file is a centralized configuration file for modern Python projects. It streamlines the development process by managing project metadata, dependencies, and development tool configurations in a single, structured file. This approach ensures consistency and maintainability, simplifying project setup and enabling developers to focus on writing quality code. Key components include project metadata, required and optional dependencies, development tool configurations (e.g., linters, formatters, and test runners), and build system specifications.
-
-In this particular pyproject.toml file, the [build-system] section specifies that the Flit package should be used to build the project. The [project] section provides metadata about the project, such as the name, description, authors, and classifiers. The [project.optional-dependencies] section lists optional dependencies, like pyspark, while the [project.urls] section supplies URLs for project documentation, source code, and issue tracking.
-
-The file also contains various configuration sections for different tools, including bandit, black, coverage, flake8, pyright, pytest, tox, and pylint. These sections specify settings for each tool, such as the maximum line length for flake8 and the minimum code coverage percentage for coverage.
-
 #### Tool Sections
 
 ##### black
 
 Black is a Python code formatter that automatically reformats Python code to conform to the PEP 8 style guide. It is used to maintain a consistent code style throughout the project.
 
 The pyproject.toml file specifies the maximum line length and whether or not to use a "fast" mode for formatting. Black also allows for a pyproject.toml configuration file to be included in the project directory to customize its behavior.
```

### Comparing `osintbuddy-0.0.2rc13.post1/docs/pylint.md` & `osintbuddy-0.0.2rc14.post1/docs/pylint.md`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.2rc13.post1/pyproject.toml` & `osintbuddy-0.0.2rc14.post1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.2rc13.post1/tests/conftest.py` & `osintbuddy-0.0.2rc14.post1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.2rc13.post1/tests/test_methods.py` & `osintbuddy-0.0.2rc14.post1/tests/test_methods.py`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.2rc13.post1/PKG-INFO` & `osintbuddy-0.0.2rc14.post1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osintbuddy
-Version: 0.0.2rc13.post1
+Version: 0.0.2rc14.post1
 Summary: OSINTBuddy - mine, merge, and map data for novel insights
 Author-email: jerlendds <jerlendsdev@proton.me>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -33,36 +33,37 @@
 Requires-Dist: shellcheck-py==0.9.0.2 ; extra == "test"
 Project-URL: Documentation, https://docs-osintbuddy-com.vercel.app/
 Project-URL: Source, https://github.com/jerlendds/osintbuddy
 Project-URL: Tracker, https://github.com/jerlendds/osintbuddy/issues
 Provides-Extra: spark
 Provides-Extra: test
 
-# OSINTBuddy
+# OSINTBuddy plugins and extensions
+
+The plugins library for [jerlendds/osintbuddy](https://github.com/jerlendds/osintbuddy), coming soon...
+
 
 This project follows the Python Standards declared in PEP 621. It uses a pyproject.yaml file to configure the project and Flit to simplify the build process and publish to PyPI. Flit simplifies the build and packaging process for Python projects by eliminating the need for separate setup.py and setup.cfg files. With Flit, you can manage all relevant configurations within the pyproject.toml file, streamlining development and promoting maintainability by centralizing project metadata, dependencies, and build specifications in one place.
 
+## Extending OSINTBuddy with extension/plugins
+
+@todo
+
+## Creating a plugin with dependent plugins...
+
+@todo
+
+
 ## Project Organization
 
 - `.github/workflows`: Contains GitHub Actions used for building, testing, and publishing.
-- `.devcontainer/Dockerfile`: Contains Dockerfile to build a development container for VSCode with all the necessary extensions for Python development installed.
-- `.devcontainer/devcontainer.json`: Contains the configuration for the development container for VSCode, including the Docker image to use, any additional VSCode extensions to install, and whether or not to mount the project directory into the container.
-- `.vscode/settings.json`: Contains VSCode settings specific to the project, such as the Python interpreter to use and the maximum line length for auto-formatting.
 - `src`: Place new source code here.
 - `tests`: Contains Python-based test cases to validate source code.
 - `pyproject.toml`: Contains metadata about the project and configurations for additional tools used to format, lint, type-check, and analyze Python code.
 
-### `pyproject.toml`
-
-The pyproject.toml file is a centralized configuration file for modern Python projects. It streamlines the development process by managing project metadata, dependencies, and development tool configurations in a single, structured file. This approach ensures consistency and maintainability, simplifying project setup and enabling developers to focus on writing quality code. Key components include project metadata, required and optional dependencies, development tool configurations (e.g., linters, formatters, and test runners), and build system specifications.
-
-In this particular pyproject.toml file, the [build-system] section specifies that the Flit package should be used to build the project. The [project] section provides metadata about the project, such as the name, description, authors, and classifiers. The [project.optional-dependencies] section lists optional dependencies, like pyspark, while the [project.urls] section supplies URLs for project documentation, source code, and issue tracking.
-
-The file also contains various configuration sections for different tools, including bandit, black, coverage, flake8, pyright, pytest, tox, and pylint. These sections specify settings for each tool, such as the maximum line length for flake8 and the minimum code coverage percentage for coverage.
-
 #### Tool Sections
 
 ##### black
 
 Black is a Python code formatter that automatically reformats Python code to conform to the PEP 8 style guide. It is used to maintain a consistent code style throughout the project.
 
 The pyproject.toml file specifies the maximum line length and whether or not to use a "fast" mode for formatting. Black also allows for a pyproject.toml configuration file to be included in the project directory to customize its behavior.
```

