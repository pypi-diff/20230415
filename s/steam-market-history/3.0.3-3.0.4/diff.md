# Comparing `tmp/steam-market-history-3.0.3.tar.gz` & `tmp/steam_market_history-3.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "steam-market-history-3.0.3.tar", max compression
+gzip compressed data, was "steam_market_history-3.0.4.tar", max compression
```

## Comparing `steam-market-history-3.0.3.tar` & `steam_market_history-3.0.4.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0     1070 2022-08-20 23:22:08.541037 steam-market-history-3.0.3/LICENSE
--rw-r--r--   0        0        0     6167 2022-08-20 23:22:08.541037 steam-market-history-3.0.3/README.md
--rw-r--r--   0        0        0      732 2022-08-20 23:22:08.552037 steam-market-history-3.0.3/pyproject.toml
--rw-r--r--   0        0        0      144 2022-08-20 23:22:08.552037 steam-market-history-3.0.3/steam_market_history/__init__.py
--rw-r--r--   0        0        0     2159 2022-08-20 23:22:08.552037 steam-market-history-3.0.3/steam_market_history/main.py
--rw-r--r--   0        0        0        0 2022-08-20 23:22:08.552037 steam-market-history-3.0.3/steam_market_history/modules/__init__.py
--rw-r--r--   0        0        0      603 2022-08-20 23:22:08.552037 steam-market-history-3.0.3/steam_market_history/modules/auth.py
--rw-r--r--   0        0        0     1341 2022-08-20 23:22:08.552037 steam-market-history-3.0.3/steam_market_history/modules/generator.py
--rw-r--r--   0        0        0     3175 2022-08-20 23:22:08.552037 steam-market-history-3.0.3/steam_market_history/modules/steam.py
--rw-r--r--   0        0        0     6167 2022-08-20 23:22:08.552037 steam-market-history-3.0.3/steam_market_history/templates/index.html
--rw-r--r--   0        0        0     7388 2022-08-20 23:22:35.931231 steam-market-history-3.0.3/setup.py
--rw-r--r--   0        0        0     7012 2022-08-20 23:22:35.931722 steam-market-history-3.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-04-15 00:07:27.850930 steam_market_history-3.0.4/LICENSE
+-rw-r--r--   0        0        0     6156 2023-04-15 00:07:27.850930 steam_market_history-3.0.4/README.md
+-rw-r--r--   0        0        0      732 2023-04-15 00:07:27.859930 steam_market_history-3.0.4/pyproject.toml
+-rw-r--r--   0        0        0      144 2023-04-15 00:07:27.859930 steam_market_history-3.0.4/steam_market_history/__init__.py
+-rw-r--r--   0        0        0     2159 2023-04-15 00:07:27.859930 steam_market_history-3.0.4/steam_market_history/main.py
+-rw-r--r--   0        0        0        0 2023-04-15 00:07:27.860930 steam_market_history-3.0.4/steam_market_history/modules/__init__.py
+-rw-r--r--   0        0        0      603 2023-04-15 00:07:27.860930 steam_market_history-3.0.4/steam_market_history/modules/auth.py
+-rw-r--r--   0        0        0     1341 2023-04-15 00:07:27.860930 steam_market_history-3.0.4/steam_market_history/modules/generator.py
+-rw-r--r--   0        0        0     3381 2023-04-15 00:07:27.860930 steam_market_history-3.0.4/steam_market_history/modules/steam.py
+-rw-r--r--   0        0        0     6167 2023-04-15 00:07:27.860930 steam_market_history-3.0.4/steam_market_history/templates/index.html
+-rw-r--r--   0        0        0     7052 1970-01-01 00:00:00.000000 steam_market_history-3.0.4/PKG-INFO
```

### Comparing `steam-market-history-3.0.3/LICENSE` & `steam_market_history-3.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `steam-market-history-3.0.3/README.md` & `steam_market_history-3.0.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 <div id="top"></div>
 
 <!-- PROJECT SHIELDS -->
 
 ![PyPI](https://img.shields.io/pypi/v/steam-market-history?style=for-the-badge)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/steam-market-history?style=for-the-badge)
-![Gitlab pipeline status](https://img.shields.io/gitlab/pipeline-status/fabieu-ci/steam-market-history?style=for-the-badge)
-![GitLab issues](https://img.shields.io/gitlab/issues/open/fabieu-ci/steam-market-history?style=for-the-badge)
-![GitLab merge requests](https://img.shields.io/gitlab/merge-requests/open-raw/fabieu-ci/steam-market-history?style=for-the-badge)
-![GitLab](https://img.shields.io/gitlab/license/fabieu-ci/steam-market-history?style=for-the-badge)
+![Gitlab pipeline status](https://img.shields.io/gitlab/pipeline-status/sustineo/steam-market-history?style=for-the-badge)
+![GitLab issues](https://img.shields.io/gitlab/issues/open/sustineo/steam-market-history?style=for-the-badge)
+![GitLab merge requests](https://img.shields.io/gitlab/merge-requests/open-raw/sustineo/steam-market-history?style=for-the-badge)
+![GitLab](https://img.shields.io/gitlab/license/sustineo/steam-market-history?style=for-the-badge)
 
 <!-- PROJECT LOGO -->
 <br />
 <div align="center">
-  <a href="https://gitlab.com/fabieu-ci/steam-market-history">
-    <img src="https://gitlab.com/fabieu-ci/steam-market-history/-/raw/main/docs/images/logo.svg" alt="Logo" width="120" height="120">
+  <a href="https://gitlab.com/sustineo/steam-market-history">
+    <img src="https://gitlab.com/sustineo/steam-market-history/-/raw/main/docs/images/logo.svg" alt="Logo" width="120" height="120">
   </a>
 
 <h3 align="center">steam-market-history</h3>
 
   <p align="center">
     An easy-to-use CLI to export your steam market history to various formats
     <br />
-    <a href="https://gitlab.com/fabieu-ci/steam-market-history/-/raw/main/docs/demo.gif">View Demo</a>
+    <a href="https://gitlab.com/sustineo/steam-market-history/-/raw/main/docs/demo.gif">View Demo</a>
     ·
-    <a href="https://gitlab.com/fabieu-ci/steam-market-history/-/issues">Report Bug</a>
+    <a href="https://gitlab.com/sustineo/steam-market-history/-/issues">Report Bug</a>
     ·
-    <a href="https://gitlab.com/fabieu-ci/steam-market-history/-/issues">Request Feature</a>
+    <a href="https://gitlab.com/sustineo/steam-market-history/-/issues">Request Feature</a>
   </p>
 </div>
 
 <!-- TABLE OF CONTENTS -->
 <details>
   <summary>Table of Contents</summary>
   <ol>
@@ -92,15 +92,15 @@
 pip install steam-market-history
 ```
 
 Manual:
 
 1. Clone the repo
    ```sh
-   git clone https://gitlab.com/fabieu-ci/steam-market-history.git
+   git clone https://gitlab.com/sustineo/steam-market-history.git
    ```
 2. Install poetry (if not already installled)
    ```sh
    pip install poetry
    ```
 3. Install dependencies and start virtual environment
    ```sh
@@ -153,15 +153,15 @@
 <!-- ROADMAP -->
 
 ## Roadmap
 
 - [ ] Add options of verbosity
 - [ ] Export to JSON
 
-See the [open issues](https://gitlab.com/fabieu-ci/steam-market-history/-/issues) for a full list of proposed features (and known issues).
+See the [open issues](https://gitlab.com/sustineo/steam-market-history/-/issues) for a full list of proposed features (and known issues).
 
 <p align="right">(<a href="#top">back to top</a>)</p>
 
 <!-- CONTRIBUTING -->
 
 ## Contributing
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
  ![PyPI](https://img.shields.io/pypi/v/steam-market-history?style=for-the-
 badge) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/steam-
 market-history?style=for-the-badge) ![Gitlab pipeline status](https://
-img.shields.io/gitlab/pipeline-status/fabieu-ci/steam-market-history?style=for-
-the-badge) ![GitLab issues](https://img.shields.io/gitlab/issues/open/fabieu-
-ci/steam-market-history?style=for-the-badge) ![GitLab merge requests](https://
-img.shields.io/gitlab/merge-requests/open-raw/fabieu-ci/steam-market-
+img.shields.io/gitlab/pipeline-status/sustineo/steam-market-history?style=for-
+the-badge) ![GitLab issues](https://img.shields.io/gitlab/issues/open/sustineo/
+steam-market-history?style=for-the-badge) ![GitLab merge requests](https://
+img.shields.io/gitlab/merge-requests/open-raw/sustineo/steam-market-
 history?style=for-the-badge) ![GitLab](https://img.shields.io/gitlab/license/
-fabieu-ci/steam-market-history?style=for-the-badge)
+sustineo/steam-market-history?style=for-the-badge)
                                     [Logo]
                         **** steam-market-history ****
   An easy-to-use CLI to export your steam market history to various formats
                   View_Demo Â· Report_Bug Â· Request_Feature
   Table of Contents
    1. About_The_Project
           o Built_With
@@ -30,15 +30,15 @@
 - Overview of _all_ transactions on a user-friendly webpage with searchable and
 filterable results ### Built With - [Python](https://www.python.org/) - [Typer]
 (https://typer.tiangolo.com/)
                                                                   (back_to_top)
  ## Getting Started To get a local copy up and running follow these simple
 example steps. ### Prerequisites - Python >= 3.8 ### Installation Pip
 (recommended): ```python pip install steam-market-history ``` Manual: 1. Clone
-the repo ```sh git clone https://gitlab.com/fabieu-ci/steam-market-history.git
+the repo ```sh git clone https://gitlab.com/sustineo/steam-market-history.git
 ``` 2. Install poetry (if not already installled) ```sh pip install poetry ```
 3. Install dependencies and start virtual environment ```sh poetry install &&
 poetry shell ``` 4. Start virtual environment ```sh poetry shell ```
                                                                   (back_to_top)
  ## Usage Currently the following commands are supported: ### `export` Export
 your steam market history to a CSV or HTML file > When running the tool you
 will be prompted to insert your steam credentials. All processing is done
@@ -50,15 +50,15 @@
 a file cache for all market transactions (default: `--no-cache`) - `--
 interactive` / `--non-interactive` - Interactive or non-interactive steam
 authentication [default: `--interactive`] Example: ``` steam-market-history
 export --csv --path /tmp/out ``` ### `version` Display detailed information
 about this package ``` steam-market-history version ```
                                                                   (back_to_top)
  ## Roadmap - [ ] Add options of verbosity - [ ] Export to JSON See the [open
-issues](https://gitlab.com/fabieu-ci/steam-market-history/-/issues) for a full
+issues](https://gitlab.com/sustineo/steam-market-history/-/issues) for a full
 list of proposed features (and known issues).
                                                                   (back_to_top)
  ## Contributing Contributions are what make the open source community such an
 amazing place to learn, inspire, and create. Any contributions you make are
 **greatly appreciated**. If you have a suggestion that would make this better,
 please fork the repo and create a pull request. You can also simply open an
 issue with the tag "enhancement". Don't forget to give the project a star!
```

### Comparing `steam-market-history-3.0.3/pyproject.toml` & `steam_market_history-3.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "steam-market-history"
-version = "3.0.3"
+version = "3.0.4"
 description = "An easy-to-use CLI to export your steam market history to various formats"
 authors = ["Fabian Eulitz <dev@sustineo.de>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/fabieu/steam-market-history"
 keywords = ["steam", "CLI"]
```

### Comparing `steam-market-history-3.0.3/steam_market_history/main.py` & `steam_market_history-3.0.4/steam_market_history/main.py`

 * *Files identical despite different names*

### Comparing `steam-market-history-3.0.3/steam_market_history/modules/auth.py` & `steam_market_history-3.0.4/steam_market_history/modules/auth.py`

 * *Files identical despite different names*

### Comparing `steam-market-history-3.0.3/steam_market_history/modules/generator.py` & `steam_market_history-3.0.4/steam_market_history/modules/generator.py`

 * *Files identical despite different names*

### Comparing `steam-market-history-3.0.3/steam_market_history/templates/index.html` & `steam_market_history-3.0.4/steam_market_history/templates/index.html`

 * *Files identical despite different names*

### Comparing `steam-market-history-3.0.3/setup.py` & `steam_market_history-3.0.4/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,234 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: steam-market-history
+Version: 3.0.4
+Summary: An easy-to-use CLI to export your steam market history to various formats
+Home-page: https://github.com/fabieu/steam-market-history
+License: MIT
+Keywords: steam,CLI
+Author: Fabian Eulitz
+Author-email: dev@sustineo.de
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
+Requires-Dist: beautifulsoup4 (>=4.11.1,<5.0.0)
+Requires-Dist: steam (>=1.2.1,<2.0.0)
+Requires-Dist: typer (>=0.4.1,<0.5.0)
+Project-URL: Repository, https://github.com/fabieu/steam-market-history
+Description-Content-Type: text/markdown
 
-packages = \
-['steam_market_history', 'steam_market_history.modules']
+<div id="top"></div>
 
-package_data = \
-{'': ['*'], 'steam_market_history': ['templates/*']}
+<!-- PROJECT SHIELDS -->
 
-install_requires = \
-['Jinja2>=3.1.2,<4.0.0',
- 'beautifulsoup4>=4.11.1,<5.0.0',
- 'steam>=1.2.1,<2.0.0',
- 'typer>=0.4.1,<0.5.0']
-
-entry_points = \
-{'console_scripts': ['steam-market-history = steam_market_history.main:app']}
-
-setup_kwargs = {
-    'name': 'steam-market-history',
-    'version': '3.0.3',
-    'description': 'An easy-to-use CLI to export your steam market history to various formats',
-    'long_description': '<div id="top"></div>\n\n<!-- PROJECT SHIELDS -->\n\n![PyPI](https://img.shields.io/pypi/v/steam-market-history?style=for-the-badge)\n![PyPI - Python Version](https://img.shields.io/pypi/pyversions/steam-market-history?style=for-the-badge)\n![Gitlab pipeline status](https://img.shields.io/gitlab/pipeline-status/fabieu-ci/steam-market-history?style=for-the-badge)\n![GitLab issues](https://img.shields.io/gitlab/issues/open/fabieu-ci/steam-market-history?style=for-the-badge)\n![GitLab merge requests](https://img.shields.io/gitlab/merge-requests/open-raw/fabieu-ci/steam-market-history?style=for-the-badge)\n![GitLab](https://img.shields.io/gitlab/license/fabieu-ci/steam-market-history?style=for-the-badge)\n\n<!-- PROJECT LOGO -->\n<br />\n<div align="center">\n  <a href="https://gitlab.com/fabieu-ci/steam-market-history">\n    <img src="https://gitlab.com/fabieu-ci/steam-market-history/-/raw/main/docs/images/logo.svg" alt="Logo" width="120" height="120">\n  </a>\n\n<h3 align="center">steam-market-history</h3>\n\n  <p align="center">\n    An easy-to-use CLI to export your steam market history to various formats\n    <br />\n    <a href="https://gitlab.com/fabieu-ci/steam-market-history/-/raw/main/docs/demo.gif">View Demo</a>\n    ·\n    <a href="https://gitlab.com/fabieu-ci/steam-market-history/-/issues">Report Bug</a>\n    ·\n    <a href="https://gitlab.com/fabieu-ci/steam-market-history/-/issues">Request Feature</a>\n  </p>\n</div>\n\n<!-- TABLE OF CONTENTS -->\n<details>\n  <summary>Table of Contents</summary>\n  <ol>\n    <li>\n      <a href="#about-the-project">About The Project</a>\n      <ul>\n        <li><a href="#built-with">Built With</a></li>\n      </ul>\n    </li>\n    <li>\n      <a href="#getting-started">Getting Started</a>\n      <ul>\n        <li><a href="#prerequisites">Prerequisites</a></li>\n        <li><a href="#installation">Installation</a></li>\n      </ul>\n    </li>\n    <li><a href="#usage">Usage</a></li>\n    <li><a href="#roadmap">Roadmap</a></li>\n    <li><a href="#contributing">Contributing</a></li>\n    <li><a href="#license">License</a></li>\n    <li><a href="#contact">Contact</a></li>\n    <li><a href="#acknowledgments">Acknowledgments</a></li>\n  </ol>\n</details>\n\n<!-- ABOUT THE PROJECT -->\n\n## About The Project\n\nsteam-market-history is a command line tool written in Python which allows you to extract your entire Steam Market History with all transaction (sales/purchases) in a CSV or HTML file.\n\n### Key features\n\n- Extract your **entire** Steam Market History\n- Create a CSV-File with all transactions\n- Overview of _all_ transactions on a user-friendly webpage with searchable and filterable results\n\n### Built With\n\n- [Python](https://www.python.org/)\n- [Typer](https://typer.tiangolo.com/)\n\n<p align="right">(<a href="#top">back to top</a>)</p>\n\n<!-- GETTING STARTED -->\n\n## Getting Started\n\nTo get a local copy up and running follow these simple example steps.\n\n### Prerequisites\n\n- Python >= 3.8\n\n### Installation\n\nPip (recommended):\n\n```python\npip install steam-market-history\n```\n\nManual:\n\n1. Clone the repo\n   ```sh\n   git clone https://gitlab.com/fabieu-ci/steam-market-history.git\n   ```\n2. Install poetry (if not already installled)\n   ```sh\n   pip install poetry\n   ```\n3. Install dependencies and start virtual environment\n   ```sh\n   poetry install && poetry shell\n   ```\n4. Start virtual environment\n   ```sh\n   poetry shell\n   ```\n\n<p align="right">(<a href="#top">back to top</a>)</p>\n\n<!-- USAGE EXAMPLES -->\n\n## Usage\n\nCurrently the following commands are supported:\n\n### `export`\n\nExport your steam market history to a CSV or HTML file\n\n> When running the tool you will be prompted to insert your steam credentials. All processing is done locally on your own computer. This package does not save your credentials in any way.\n\nOptions:\n\n- `--csv` - Export to csv file\n- `--html` - Export to html file\n- `--path` - Output directory for all file based operations (default: current working directory)\n- `--launch` / `--no-launch` - Automatically open file(s) after export (default: `--launch`)\n- `--cache` / `--no-cache` - Create a file cache for all market transactions (default: `--no-cache`)\n- `--interactive` / `--non-interactive` - Interactive or non-interactive steam authentication [default: `--interactive`]\n\nExample:\n\n```\nsteam-market-history export --csv --path /tmp/out\n```\n\n### `version`\n\nDisplay detailed information about this package\n\n```\nsteam-market-history version\n```\n\n<p align="right">(<a href="#top">back to top</a>)</p>\n\n<!-- ROADMAP -->\n\n## Roadmap\n\n- [ ] Add options of verbosity\n- [ ] Export to JSON\n\nSee the [open issues](https://gitlab.com/fabieu-ci/steam-market-history/-/issues) for a full list of proposed features (and known issues).\n\n<p align="right">(<a href="#top">back to top</a>)</p>\n\n<!-- CONTRIBUTING -->\n\n## Contributing\n\nContributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.\n\nIf you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".\nDon\'t forget to give the project a star! Thanks again!\n\n1. Fork the Project\n2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)\n3. Commit your Changes (`git commit -m \'Add some AmazingFeature\'`)\n4. Push to the Branch (`git push origin feature/AmazingFeature`)\n5. Open a Pull Request\n\n<p align="right">(<a href="#top">back to top</a>)</p>\n\n<!-- LICENSE -->\n\n## License\n\nDistributed under the MIT License. See `LICENSE` for more information.\n\n<p align="right">(<a href="#top">back to top</a>)</p>\n\n<!-- CONTACT -->\n\n## Contact\n\nsustineo\\_ - [@sustineo\\_](https://twitter.com/sustineo_) - dev@sustineo.de\n\n<p align="right">(<a href="#top">back to top</a>)</p>\n\n<!-- ACKNOWLEDGMENTS -->\n\n## Acknowledgments\n\n- [Typer](https://typer.tiangolo.com/)\n- [Choose a license](https://choosealicense.com/)\n\n<p align="right">(<a href="#top">back to top</a>)</p>\n\n## Disclaimer:\n\nThe Steam Market History Exported is a community project and is not affiliated with Valve or Steam.\n\n<p align="right">(<a href="#top">back to top</a>)</p>\n',
-    'author': 'Fabian Eulitz',
-    'author_email': 'dev@sustineo.de',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/fabieu/steam-market-history',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<4.0',
-}
+![PyPI](https://img.shields.io/pypi/v/steam-market-history?style=for-the-badge)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/steam-market-history?style=for-the-badge)
+![Gitlab pipeline status](https://img.shields.io/gitlab/pipeline-status/sustineo/steam-market-history?style=for-the-badge)
+![GitLab issues](https://img.shields.io/gitlab/issues/open/sustineo/steam-market-history?style=for-the-badge)
+![GitLab merge requests](https://img.shields.io/gitlab/merge-requests/open-raw/sustineo/steam-market-history?style=for-the-badge)
+![GitLab](https://img.shields.io/gitlab/license/sustineo/steam-market-history?style=for-the-badge)
 
+<!-- PROJECT LOGO -->
+<br />
+<div align="center">
+  <a href="https://gitlab.com/sustineo/steam-market-history">
+    <img src="https://gitlab.com/sustineo/steam-market-history/-/raw/main/docs/images/logo.svg" alt="Logo" width="120" height="120">
+  </a>
+
+<h3 align="center">steam-market-history</h3>
+
+  <p align="center">
+    An easy-to-use CLI to export your steam market history to various formats
+    <br />
+    <a href="https://gitlab.com/sustineo/steam-market-history/-/raw/main/docs/demo.gif">View Demo</a>
+    ·
+    <a href="https://gitlab.com/sustineo/steam-market-history/-/issues">Report Bug</a>
+    ·
+    <a href="https://gitlab.com/sustineo/steam-market-history/-/issues">Request Feature</a>
+  </p>
+</div>
+
+<!-- TABLE OF CONTENTS -->
+<details>
+  <summary>Table of Contents</summary>
+  <ol>
+    <li>
+      <a href="#about-the-project">About The Project</a>
+      <ul>
+        <li><a href="#built-with">Built With</a></li>
+      </ul>
+    </li>
+    <li>
+      <a href="#getting-started">Getting Started</a>
+      <ul>
+        <li><a href="#prerequisites">Prerequisites</a></li>
+        <li><a href="#installation">Installation</a></li>
+      </ul>
+    </li>
+    <li><a href="#usage">Usage</a></li>
+    <li><a href="#roadmap">Roadmap</a></li>
+    <li><a href="#contributing">Contributing</a></li>
+    <li><a href="#license">License</a></li>
+    <li><a href="#contact">Contact</a></li>
+    <li><a href="#acknowledgments">Acknowledgments</a></li>
+  </ol>
+</details>
+
+<!-- ABOUT THE PROJECT -->
+
+## About The Project
+
+steam-market-history is a command line tool written in Python which allows you to extract your entire Steam Market History with all transaction (sales/purchases) in a CSV or HTML file.
+
+### Key features
+
+- Extract your **entire** Steam Market History
+- Create a CSV-File with all transactions
+- Overview of _all_ transactions on a user-friendly webpage with searchable and filterable results
+
+### Built With
+
+- [Python](https://www.python.org/)
+- [Typer](https://typer.tiangolo.com/)
+
+<p align="right">(<a href="#top">back to top</a>)</p>
+
+<!-- GETTING STARTED -->
+
+## Getting Started
+
+To get a local copy up and running follow these simple example steps.
+
+### Prerequisites
+
+- Python >= 3.8
+
+### Installation
+
+Pip (recommended):
+
+```python
+pip install steam-market-history
+```
+
+Manual:
+
+1. Clone the repo
+   ```sh
+   git clone https://gitlab.com/sustineo/steam-market-history.git
+   ```
+2. Install poetry (if not already installled)
+   ```sh
+   pip install poetry
+   ```
+3. Install dependencies and start virtual environment
+   ```sh
+   poetry install && poetry shell
+   ```
+4. Start virtual environment
+   ```sh
+   poetry shell
+   ```
+
+<p align="right">(<a href="#top">back to top</a>)</p>
+
+<!-- USAGE EXAMPLES -->
+
+## Usage
+
+Currently the following commands are supported:
+
+### `export`
+
+Export your steam market history to a CSV or HTML file
+
+> When running the tool you will be prompted to insert your steam credentials. All processing is done locally on your own computer. This package does not save your credentials in any way.
+
+Options:
+
+- `--csv` - Export to csv file
+- `--html` - Export to html file
+- `--path` - Output directory for all file based operations (default: current working directory)
+- `--launch` / `--no-launch` - Automatically open file(s) after export (default: `--launch`)
+- `--cache` / `--no-cache` - Create a file cache for all market transactions (default: `--no-cache`)
+- `--interactive` / `--non-interactive` - Interactive or non-interactive steam authentication [default: `--interactive`]
+
+Example:
+
+```
+steam-market-history export --csv --path /tmp/out
+```
+
+### `version`
+
+Display detailed information about this package
+
+```
+steam-market-history version
+```
+
+<p align="right">(<a href="#top">back to top</a>)</p>
+
+<!-- ROADMAP -->
+
+## Roadmap
+
+- [ ] Add options of verbosity
+- [ ] Export to JSON
+
+See the [open issues](https://gitlab.com/sustineo/steam-market-history/-/issues) for a full list of proposed features (and known issues).
+
+<p align="right">(<a href="#top">back to top</a>)</p>
+
+<!-- CONTRIBUTING -->
+
+## Contributing
+
+Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.
+
+If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
+Don't forget to give the project a star! Thanks again!
+
+1. Fork the Project
+2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
+3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
+4. Push to the Branch (`git push origin feature/AmazingFeature`)
+5. Open a Pull Request
+
+<p align="right">(<a href="#top">back to top</a>)</p>
+
+<!-- LICENSE -->
+
+## License
+
+Distributed under the MIT License. See `LICENSE` for more information.
+
+<p align="right">(<a href="#top">back to top</a>)</p>
+
+<!-- CONTACT -->
+
+## Contact
+
+sustineo\_ - [@sustineo\_](https://twitter.com/sustineo_) - dev@sustineo.de
+
+<p align="right">(<a href="#top">back to top</a>)</p>
+
+<!-- ACKNOWLEDGMENTS -->
+
+## Acknowledgments
+
+- [Typer](https://typer.tiangolo.com/)
+- [Choose a license](https://choosealicense.com/)
+
+<p align="right">(<a href="#top">back to top</a>)</p>
+
+## Disclaimer:
+
+The Steam Market History Exported is a community project and is not affiliated with Valve or Steam.
+
+<p align="right">(<a href="#top">back to top</a>)</p>
 
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,116 +1,93 @@
-# -*- coding: utf-8 -*- from setuptools import setup packages = \
-['steam_market_history', 'steam_market_history.modules'] package_data = \ {'':
-['*'], 'steam_market_history': ['templates/*']} install_requires = \
-['Jinja2>=3.1.2,<4.0.0', 'beautifulsoup4>=4.11.1,<5.0.0',
-'steam>=1.2.1,<2.0.0', 'typer>=0.4.1,<0.5.0'] entry_points = \
-{'console_scripts': ['steam-market-history = steam_market_history.main:app']}
-setup_kwargs = { 'name': 'steam-market-history', 'version': '3.0.3',
-'description': 'An easy-to-use CLI to export your steam market history to
-various formats', 'long_description': '
-\n\n\n\n![PyPI](https://img.shields.io/pypi/v/steam-market-history?style=for-
-the-badge)\n![PyPI - Python Version](https://img.shields.io/pypi/pyversions/
-steam-market-history?style=for-the-badge)\n![Gitlab pipeline status](https://
-img.shields.io/gitlab/pipeline-status/fabieu-ci/steam-market-history?style=for-
-the-badge)\n![GitLab issues](https://img.shields.io/gitlab/issues/open/fabieu-
-ci/steam-market-history?style=for-the-badge)\n![GitLab merge requests](https://
-img.shields.io/gitlab/merge-requests/open-raw/fabieu-ci/steam-market-
-history?style=for-the-badge)\n![GitLab](https://img.shields.io/gitlab/license/
-fabieu-ci/steam-market-history?style=for-the-badge)\n\n\n
-\n
-                              \n \n_[Logo]\n\n\n
+Metadata-Version: 2.1 Name: steam-market-history Version: 3.0.4 Summary: An
+easy-to-use CLI to export your steam market history to various formats Home-
+page: https://github.com/fabieu/steam-market-history License: MIT Keywords:
+steam,CLI Author: Fabian Eulitz Author-email: dev@sustineo.de Requires-Python:
+>=3.8,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Requires-Dist: Jinja2 (>=3.1.2,<4.0.0) Requires-Dist:
+beautifulsoup4 (>=4.11.1,<5.0.0) Requires-Dist: steam (>=1.2.1,<2.0.0)
+Requires-Dist: typer (>=0.4.1,<0.5.0) Project-URL: Repository, https://
+github.com/fabieu/steam-market-history Description-Content-Type: text/markdown
+ ![PyPI](https://img.shields.io/pypi/v/steam-market-history?style=for-the-
+badge) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/steam-
+market-history?style=for-the-badge) ![Gitlab pipeline status](https://
+img.shields.io/gitlab/pipeline-status/sustineo/steam-market-history?style=for-
+the-badge) ![GitLab issues](https://img.shields.io/gitlab/issues/open/sustineo/
+steam-market-history?style=for-the-badge) ![GitLab merge requests](https://
+img.shields.io/gitlab/merge-requests/open-raw/sustineo/steam-market-
+history?style=for-the-badge) ![GitLab](https://img.shields.io/gitlab/license/
+sustineo/steam-market-history?style=for-the-badge)
+                                    [Logo]
                         **** steam-market-history ****
-                                     \n\n
-\n An easy-to-use CLI to export your steam market history to various formats\n
-            \n View_Demo\n Â·\n Report_Bug\n Â·\n Request_Feature\n
-                                      \n
-\n\n\n\n Table of Contents\n
-   1. \n
-   2. \n About_The_Project\n
-          o \n
+  An easy-to-use CLI to export your steam market history to various formats
+                  View_Demo Â· Report_Bug Â· Request_Feature
+  Table of Contents
+   1. About_The_Project
           o Built_With
-          o \n
-      \n
-   3. \n
-   4. \n Getting_Started\n
-          o \n
+   2. Getting_Started
           o Prerequisites
-          o \n
           o Installation
-          o \n
-      \n
-   5. \n
-   6. Usage
-   7. \n
-   8. Roadmap
-   9. \n
-  10. Contributing
-  11. \n
-  12. License
-  13. \n
-  14. Contact
-  15. \n
-  16. Acknowledgments
-  17. \n
-\n\n\n\n\n## About The Project\n\nsteam-market-history is a command line tool
-written in Python which allows you to extract your entire Steam Market History
-with all transaction (sales/purchases) in a CSV or HTML file.\n\n### Key
-features\n\n- Extract your **entire** Steam Market History\n- Create a CSV-File
-with all transactions\n- Overview of _all_ transactions on a user-friendly
-webpage with searchable and filterable results\n\n### Built With\n\n- [Python]
-(https://www.python.org/)\n- [Typer](https://typer.tiangolo.com/)\n\n
-                                                                  (back_to_top)
-\n\n\n\n## Getting Started\n\nTo get a local copy up and running follow these
-simple example steps.\n\n### Prerequisites\n\n- Python >= 3.8\n\n###
-Installation\n\nPip (recommended):\n\n```python\npip install steam-market-
-history\n```\n\nManual:\n\n1. Clone the repo\n ```sh\n git clone https://
-gitlab.com/fabieu-ci/steam-market-history.git\n ```\n2. Install poetry (if not
-already installled)\n ```sh\n pip install poetry\n ```\n3. Install dependencies
-and start virtual environment\n ```sh\n poetry install && poetry shell\n
-```\n4. Start virtual environment\n ```sh\n poetry shell\n ```\n\n
-                                                                  (back_to_top)
-\n\n\n\n## Usage\n\nCurrently the following commands are supported:\n\n###
-`export`\n\nExport your steam market history to a CSV or HTML file\n\n> When
-running the tool you will be prompted to insert your steam credentials. All
-processing is done locally on your own computer. This package does not save
-your credentials in any way.\n\nOptions:\n\n- `--csv` - Export to csv file\n-
-`--html` - Export to html file\n- `--path` - Output directory for all file
-based operations (default: current working directory)\n- `--launch` / `--no-
-launch` - Automatically open file(s) after export (default: `--launch`)\n- `--
-cache` / `--no-cache` - Create a file cache for all market transactions
-(default: `--no-cache`)\n- `--interactive` / `--non-interactive` - Interactive
-or non-interactive steam authentication [default: `--interactive`]\n\nExample:
-\n\n```\nsteam-market-history export --csv --path /tmp/out\n```\n\n###
-`version`\n\nDisplay detailed information about this package\n\n```\nsteam-
-market-history version\n```\n\n
-                                                                  (back_to_top)
-\n\n\n\n## Roadmap\n\n- [ ] Add options of verbosity\n- [ ] Export to
-JSON\n\nSee the [open issues](https://gitlab.com/fabieu-ci/steam-market-
-history/-/issues) for a full list of proposed features (and known issues).\n\n
-                                                                  (back_to_top)
-\n\n\n\n## Contributing\n\nContributions are what make the open source
-community such an amazing place to learn, inspire, and create. Any
-contributions you make are **greatly appreciated**.\n\nIf you have a suggestion
-that would make this better, please fork the repo and create a pull request.
-You can also simply open an issue with the tag "enhancement".\nDon\'t forget to
-give the project a star! Thanks again!\n\n1. Fork the Project\n2. Create your
-Feature Branch (`git checkout -b feature/AmazingFeature`)\n3. Commit your
-Changes (`git commit -m \'Add some AmazingFeature\'`)\n4. Push to the Branch
-(`git push origin feature/AmazingFeature`)\n5. Open a Pull Request\n\n
-                                                                  (back_to_top)
-\n\n\n\n## License\n\nDistributed under the MIT License. See `LICENSE` for more
-information.\n\n
-                                                                  (back_to_top)
-\n\n\n\n## Contact\n\nsustineo\\_ - [@sustineo\\_](https://twitter.com/
-sustineo_) - dev@sustineo.de\n\n
-                                                                  (back_to_top)
-\n\n\n\n## Acknowledgments\n\n- [Typer](https://typer.tiangolo.com/)\n- [Choose
-a license](https://choosealicense.com/)\n\n
-                                                                  (back_to_top)
-\n\n## Disclaimer:\n\nThe Steam Market History Exported is a community project
-and is not affiliated with Valve or Steam.\n\n
-                                                                  (back_to_top)
-\n', 'author': 'Fabian Eulitz', 'author_email': 'dev@sustineo.de',
-'maintainer': None, 'maintainer_email': None, 'url': 'https://github.com/
-fabieu/steam-market-history', 'packages': packages, 'package_data':
-package_data, 'install_requires': install_requires, 'entry_points':
-entry_points, 'python_requires': '>=3.8,<4.0', } setup(**setup_kwargs)
+   3. Usage
+   4. Roadmap
+   5. Contributing
+   6. License
+   7. Contact
+   8. Acknowledgments
+  ## About The Project steam-market-history is a command line tool written in
+Python which allows you to extract your entire Steam Market History with all
+transaction (sales/purchases) in a CSV or HTML file. ### Key features - Extract
+your **entire** Steam Market History - Create a CSV-File with all transactions
+- Overview of _all_ transactions on a user-friendly webpage with searchable and
+filterable results ### Built With - [Python](https://www.python.org/) - [Typer]
+(https://typer.tiangolo.com/)
+                                                                  (back_to_top)
+ ## Getting Started To get a local copy up and running follow these simple
+example steps. ### Prerequisites - Python >= 3.8 ### Installation Pip
+(recommended): ```python pip install steam-market-history ``` Manual: 1. Clone
+the repo ```sh git clone https://gitlab.com/sustineo/steam-market-history.git
+``` 2. Install poetry (if not already installled) ```sh pip install poetry ```
+3. Install dependencies and start virtual environment ```sh poetry install &&
+poetry shell ``` 4. Start virtual environment ```sh poetry shell ```
+                                                                  (back_to_top)
+ ## Usage Currently the following commands are supported: ### `export` Export
+your steam market history to a CSV or HTML file > When running the tool you
+will be prompted to insert your steam credentials. All processing is done
+locally on your own computer. This package does not save your credentials in
+any way. Options: - `--csv` - Export to csv file - `--html` - Export to html
+file - `--path` - Output directory for all file based operations (default:
+current working directory) - `--launch` / `--no-launch` - Automatically open
+file(s) after export (default: `--launch`) - `--cache` / `--no-cache` - Create
+a file cache for all market transactions (default: `--no-cache`) - `--
+interactive` / `--non-interactive` - Interactive or non-interactive steam
+authentication [default: `--interactive`] Example: ``` steam-market-history
+export --csv --path /tmp/out ``` ### `version` Display detailed information
+about this package ``` steam-market-history version ```
+                                                                  (back_to_top)
+ ## Roadmap - [ ] Add options of verbosity - [ ] Export to JSON See the [open
+issues](https://gitlab.com/sustineo/steam-market-history/-/issues) for a full
+list of proposed features (and known issues).
+                                                                  (back_to_top)
+ ## Contributing Contributions are what make the open source community such an
+amazing place to learn, inspire, and create. Any contributions you make are
+**greatly appreciated**. If you have a suggestion that would make this better,
+please fork the repo and create a pull request. You can also simply open an
+issue with the tag "enhancement". Don't forget to give the project a star!
+Thanks again! 1. Fork the Project 2. Create your Feature Branch (`git checkout
+-b feature/AmazingFeature`) 3. Commit your Changes (`git commit -m 'Add some
+AmazingFeature'`) 4. Push to the Branch (`git push origin feature/
+AmazingFeature`) 5. Open a Pull Request
+                                                                  (back_to_top)
+ ## License Distributed under the MIT License. See `LICENSE` for more
+information.
+                                                                  (back_to_top)
+ ## Contact sustineo\_ - [@sustineo\_](https://twitter.com/sustineo_) -
+dev@sustineo.de
+                                                                  (back_to_top)
+ ## Acknowledgments - [Typer](https://typer.tiangolo.com/) - [Choose a license]
+(https://choosealicense.com/)
+                                                                  (back_to_top)
+## Disclaimer: The Steam Market History Exported is a community project and is
+not affiliated with Valve or Steam.
+                                                                  (back_to_top)
```

