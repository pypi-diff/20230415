# Comparing `tmp/orion_nais-0.1.1.tar.gz` & `tmp/orion_nais-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orion_nais-0.1.1.tar", max compression
+gzip compressed data, was "orion_nais-0.1.2.tar", max compression
```

## Comparing `orion_nais-0.1.1.tar` & `orion_nais-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1072 2023-02-10 13:07:27.340638 orion_nais-0.1.1/LICENSE
--rw-r--r--   0        0        0     6081 2023-04-14 11:14:29.054669 orion_nais-0.1.1/README.md
--rw-r--r--   0        0        0       39 2023-01-26 14:12:33.833384 orion_nais-0.1.1/orion/__init__.py
--rw-r--r--   0        0        0    16061 2023-04-14 10:54:20.572049 orion_nais-0.1.1/orion/client.py
--rw-r--r--   0        0        0    17303 2023-02-10 12:06:31.153714 orion_nais-0.1.1/orion/mmsi.py
--rw-r--r--   0        0        0        0 2023-02-03 22:04:07.481203 orion_nais-0.1.1/orion/types/__init__.py
--rw-r--r--   0        0        0      296 2023-02-03 09:47:58.249080 orion_nais-0.1.1/orion/types/ais.py
--rw-r--r--   0        0        0      136 2023-01-27 13:52:51.653087 orion_nais-0.1.1/orion/urls.py
--rw-r--r--   0        0        0        0 2023-02-04 00:21:05.300372 orion_nais-0.1.1/orion/utils/__init__.py
--rw-r--r--   0        0        0     1100 2023-02-10 10:06:30.752969 orion_nais-0.1.1/orion/utils/get_data.py
--rw-r--r--   0        0        0    16329 2023-02-10 12:07:42.453458 orion_nais-0.1.1/orion/vessel_codes.py
--rw-r--r--   0        0        0     1378 2023-04-14 11:15:41.046256 orion_nais-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     7146 1970-01-01 00:00:00.000000 orion_nais-0.1.1/setup.py
--rw-r--r--   0        0        0     6752 1970-01-01 00:00:00.000000 orion_nais-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-02-10 13:07:27.340638 orion_nais-0.1.2/LICENSE
+-rw-r--r--   0        0        0     6590 2023-04-15 09:26:36.509871 orion_nais-0.1.2/README.md
+-rw-r--r--   0        0        0       39 2023-01-26 14:12:33.833384 orion_nais-0.1.2/orion/__init__.py
+-rw-r--r--   0        0        0    16061 2023-04-15 13:15:33.647801 orion_nais-0.1.2/orion/client.py
+-rw-r--r--   0        0        0    17635 2023-04-15 13:20:41.818455 orion_nais-0.1.2/orion/mmsi.py
+-rw-r--r--   0        0        0        0 2023-02-03 22:04:07.481203 orion_nais-0.1.2/orion/types/__init__.py
+-rw-r--r--   0        0        0      296 2023-02-03 09:47:58.249080 orion_nais-0.1.2/orion/types/ais.py
+-rw-r--r--   0        0        0      136 2023-01-27 13:52:51.653087 orion_nais-0.1.2/orion/urls.py
+-rw-r--r--   0        0        0        0 2023-02-04 00:21:05.300372 orion_nais-0.1.2/orion/utils/__init__.py
+-rw-r--r--   0        0        0     1100 2023-02-10 10:06:30.752969 orion_nais-0.1.2/orion/utils/get_data.py
+-rw-r--r--   0        0        0    16652 2023-04-15 13:25:46.276172 orion_nais-0.1.2/orion/vessel_codes.py
+-rw-r--r--   0        0        0     1654 2023-04-15 13:53:48.863111 orion_nais-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     7713 1970-01-01 00:00:00.000000 orion_nais-0.1.2/setup.py
+-rw-r--r--   0        0        0     7451 1970-01-01 00:00:00.000000 orion_nais-0.1.2/PKG-INFO
```

### Comparing `orion_nais-0.1.1/LICENSE` & `orion_nais-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `orion_nais-0.1.1/README.md` & `orion_nais-0.1.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -4,26 +4,28 @@
 <!-- TABLE OF CONTENTS -->
 <details open="open">
   <summary><h2 style="display: inline-block">Table of Contents</h2></summary>
   <ol>
     <li>
       <a href="#about-the-project">About The Project</a>
       <ul>
-        <li><a href="#requirements">Requirements</a></li>
-        <li><a href="#structure">Structure</a></li>
+        <li><a href="#requirements">Why the nanme Orion?</a></li>
       </ul>
     </li>
     <li>
-      <a href="#getting-started">Getting Started</a>
+      <a href="#installation">Installation</a>
+    </li>
+    <li><a href="#usage">Usage</a></li>
+    <li><a href="#local-development">Local development</a>
       <ul>
-        <li><a href="#prerequisites">Prerequisites</a></li>
-        <li><a href="#installation">Installation</a></li>
+        <li><a href="#requirements">Requirements</a></li>
+        <li><a href="#makefile-commands">Makefile commands</a></li>
+        <li><a href="#structure">Structure</a></li>
       </ul>
     </li>
-    <li><a href="#usage">Usage</a></li>
     <li><a href="#contributing">Contributing</a></li>
     <li><a href="#contact">Contact</a></li>
   </ol>
 </details>
 
 <!-- ABOUT THE PROJECT -->
 
@@ -59,21 +61,46 @@
 
 ```bash
 poetry add orion-nais
 ```
 
 ## Usage
 
-There are a heap of functions for you to use. Enjoy.
+To install the package in your project run
+
+```bash
+
+poetry add orion-nais
+```
+
+then add an .env file to your project with the following variables:
+
+```bash
+CLIENT_ID=
+CLIENT_SECRET=
+```
+
+If you don't have a client id and secret you can get one from your [BarentsWatch account](https://www.barentswatch.no/minside/).
+
+Then you can use the client like this:
+
+```python
+from orion import Orion
+
+orion = Orion()
+# Get the last 24 hours of AIS data for a ship with MMSI XXXXXXXXXX
+ais = orion.get_ais_last_24H(SHIP_MMSI)
+# Convert the AIS data to a line
+line = orion.ais_to_line(ais)
+
+```
 
 ## Local development
 
 ### Requirements
----
-
 - pyenv - manage python versions
 - poetry - manage python dependencies
 
 To install on mac you can use homebrew:
 
 ```bash
 brew upgrade
@@ -162,23 +189,14 @@
     - `get_data.py`
       - A function for getting data from other sources. Not used by the Orion client. Contains code for getting data from the Norwegian Petroleum Directorate.
   - `vessel_codes.py`
     - A dataclass for looking up vessel codes.
 - `tests`
   - Tests for the package.
 
-## Usage
-
-To install the package in your project run
-
-```bash
-
-poetry add orion-nais
-```
-
 ## Contributing
 
 Do you have write permissions to the repo? Then you can clone this project to a folder on your computer.
 
 ```bash
 git clone https://github.com/BergensTidende/orion-nais.git
 ```
@@ -186,15 +204,15 @@
 If not do the following:
 
 - Create a personal fork of the project on Github.
 - Clone the fork on your local machine. Your remote repo on Github is called `origin`.
 - Add the original repository as a remote called `upstream`.
 - If you created your fork a while ago be sure to pull upstream changes into your local repository.
 
-This will clone the repo into `pakkenellik`. 
+This will clone the repo into `orion-nais`. 
 
 Create a branch for your changes
 
 ```bash
 git checkout -b name-of-branch
 ```
 
@@ -202,16 +220,15 @@
 
 If you're working on a clone push the branch to github and make PR.
 
 If your're working a fork:
 
 - Squash your commits into a single commit with git's [interactive rebase](https://help.github.com/articles/interactive-rebase). Create a new branch if necessary.
 - Push your branch to your fork on Github, the remote `origin`.
-- From your fork open a pull request in the correct branch. Target the project's `develop` branch if there is one, else go for `master`!
-- …
+- From your fork open a pull request in the correct branch. Target the project's `develop` branch if there is one, else go for `master`.
 - If the maintainer requests further changes just push them to your branch. The PR will be updated automatically.
 - Once the pull request is approved and merged you can pull the changes from `upstream` to your local repo and delete
   your extra branch(es).
 
  <!-- CONTACT -->
 
 ## Contact
```

#### html2text {}

```diff
@@ -1,48 +1,56 @@
 # Orion-NAIS
 ***** Table of Contents *****
    1. About_The_Project
+          o Why_the_nanme_Orion?
+   2. Installation
+   3. Usage
+   4. Local_development
           o Requirements
+          o Makefile_commands
           o Structure
-   2. Getting_Started
-          o Prerequisites
-          o Installation
-   3. Usage
-   4. Contributing
-   5. Contact
+   5. Contributing
+   6. Contact
   ## About The Project Orion-NAIS is a client to work with the NAIS API. It
 helps with authentication and provides a simple interface to work with the API.
 When working with the API you need to have a valid token. The token is valid
 for a set period of time. The client will automatically refresh the token when
 it expires. ### Why the name Orion? The NAIS Api is provided through
 BarentsWatch. BarentsWatch is a Norwegian information portal that provides
 overview of activity and knowledge in coastal and sea areas. The Norwegian
 movie "Orion's Belt" from 1985 is an action movie set in the Barents region.
 About three men, a bulldozer, a Russian helicopter and a ship. Thus the name
 Orion. ## Installation Requires Python 3.10 or later. ```bash pip install
 orion-nais ``` or using pipenv: ```bash pipenv install orion-nais ``` or using
-poetry: ```bash poetry add orion-nais ``` ## Usage There are a heap of
-functions for you to use. Enjoy. ## Local development ### Requirements --- -
-pyenv - manage python versions - poetry - manage python dependencies To install
-on mac you can use homebrew: ```bash brew upgrade brew install pyenv ``` You
-can either install poetry with homebrew or the way described in the
-[documentation](https://python-poetry.org/docs/#installation) ### Makefile
-commands - `make lint` - lint the code in the src folder with black, isort and
-flake8. Mypy will check for correct typing. - `make format` - format the code
-in the src folder with black and isort. - `make test` - run the tests in the
-tests folder. - `make bump-patch` - bump the patch version of the package.
-Example: 0.1.0 -> 0.1.1 - `make bump-minor` - bump the minor version of the
-package. Example: 0.1.0 -> 0.2.0 - `make bump-major` - bump the major version
-of the package. Example: 0.1.0 -> 1.0.0 - `make release` - publish the package
-to pypi. You need to have an account and be logged in to pypi. ### Structure
-``` . âââ .bumpversion.cfg âââ .editorconfig âââ .flake8
-âââ .gitignore âââ Makefile âââ README.md âââ orion â
-âââ client.py â âââ mmsi.py â âââ types â â âââ
-ais.py â âââ urls.py â âââ utils â â âââ get_data.py
-â âââ vessel_codes.py âââ poetry.lock âââ pyproject.toml
+poetry: ```bash poetry add orion-nais ``` ## Usage To install the package in
+your project run ```bash poetry add orion-nais ``` then add an .env file to
+your project with the following variables: ```bash CLIENT_ID= CLIENT_SECRET=
+``` If you don't have a client id and secret you can get one from your
+[BarentsWatch account](https://www.barentswatch.no/minside/). Then you can use
+the client like this: ```python from orion import Orion orion = Orion() # Get
+the last 24 hours of AIS data for a ship with MMSI XXXXXXXXXX ais =
+orion.get_ais_last_24H(SHIP_MMSI) # Convert the AIS data to a line line =
+orion.ais_to_line(ais) ``` ## Local development ### Requirements - pyenv -
+manage python versions - poetry - manage python dependencies To install on mac
+you can use homebrew: ```bash brew upgrade brew install pyenv ``` You can
+either install poetry with homebrew or the way described in the [documentation]
+(https://python-poetry.org/docs/#installation) ### Makefile commands - `make
+lint` - lint the code in the src folder with black, isort and flake8. Mypy will
+check for correct typing. - `make format` - format the code in the src folder
+with black and isort. - `make test` - run the tests in the tests folder. -
+`make bump-patch` - bump the patch version of the package. Example: 0.1.0 -
+> 0.1.1 - `make bump-minor` - bump the minor version of the package. Example:
+0.1.0 -> 0.2.0 - `make bump-major` - bump the major version of the package.
+Example: 0.1.0 -> 1.0.0 - `make release` - publish the package to pypi. You
+need to have an account and be logged in to pypi. ### Structure ``` . âââ
+.bumpversion.cfg âââ .editorconfig âââ .flake8 âââ .gitignore
+âââ Makefile âââ README.md âââ orion â âââ client.py
+â âââ mmsi.py â âââ types â â âââ ais.py â
+âââ urls.py â âââ utils â â âââ get_data.py â
+âââ vessel_codes.py âââ poetry.lock âââ pyproject.toml
 âââ tests âââ make_mock_data.py âââ mocks âââ
 test_orion.py ``` - `.bumpversion.cfg` - Configuration file for bumpversion. -
 `.editorconfig` - Configuration file for editorconfig. - `.flake8` -
 Configuration file for flake8. - `.gitignore` - Configuration file for git. -
 `pyproject.toml` - Configuration file for poetry. Mypy and isort is configured
 here. - `poetry.lock` - Lock file for poetry. - `Makefile` - Makefile for the
 project. Here you can find commands for linting and formatting. - `README.md` -
@@ -50,29 +58,28 @@
 client class. - `mmsi.py` - A dataclass for handling MMSI numbers and MID-codes
 (jurisdiction). - `types` - A folder for types. - `ais.py` - A class for
 handling AIS messages. - `urls.py` - A file with urls for the API. - `utils` -
 A folder for utility functions. - `get_data.py` - A function for getting data
 from other sources. Not used by the Orion client. Contains code for getting
 data from the Norwegian Petroleum Directorate. - `vessel_codes.py` - A
 dataclass for looking up vessel codes. - `tests` - Tests for the package. ##
-Usage To install the package in your project run ```bash poetry add orion-nais
-``` ## Contributing Do you have write permissions to the repo? Then you can
-clone this project to a folder on your computer. ```bash git clone https://
-github.com/BergensTidende/orion-nais.git ``` If not do the following: - Create
-a personal fork of the project on Github. - Clone the fork on your local
-machine. Your remote repo on Github is called `origin`. - Add the original
-repository as a remote called `upstream`. - If you created your fork a while
-ago be sure to pull upstream changes into your local repository. This will
-clone the repo into `pakkenellik`. Create a branch for your changes ```bash git
-checkout -b name-of-branch ``` Make your changes, rememeber to commit. And
-always write your commit messages in the present tense. Your commit message
-should describe what the commit, when applied, does to the code â not what
-you did to the code. If you're working on a clone push the branch to github and
-make PR. If your're working a fork: - Squash your commits into a single commit
-with git's [interactive rebase](https://help.github.com/articles/interactive-
-rebase). Create a new branch if necessary. - Push your branch to your fork on
-Github, the remote `origin`. - From your fork open a pull request in the
-correct branch. Target the project's `develop` branch if there is one, else go
-for `master`! - â¦ - If the maintainer requests further changes just push them
-to your branch. The PR will be updated automatically. - Once the pull request
-is approved and merged you can pull the changes from `upstream` to your local
-repo and delete your extra branch(es).  ## Contact Bord4 - bord4@bt.no
+Contributing Do you have write permissions to the repo? Then you can clone this
+project to a folder on your computer. ```bash git clone https://github.com/
+BergensTidende/orion-nais.git ``` If not do the following: - Create a personal
+fork of the project on Github. - Clone the fork on your local machine. Your
+remote repo on Github is called `origin`. - Add the original repository as a
+remote called `upstream`. - If you created your fork a while ago be sure to
+pull upstream changes into your local repository. This will clone the repo into
+`orion-nais`. Create a branch for your changes ```bash git checkout -b name-of-
+branch ``` Make your changes, rememeber to commit. And always write your commit
+messages in the present tense. Your commit message should describe what the
+commit, when applied, does to the code â not what you did to the code. If
+you're working on a clone push the branch to github and make PR. If your're
+working a fork: - Squash your commits into a single commit with git's
+[interactive rebase](https://help.github.com/articles/interactive-rebase).
+Create a new branch if necessary. - Push your branch to your fork on Github,
+the remote `origin`. - From your fork open a pull request in the correct
+branch. Target the project's `develop` branch if there is one, else go for
+`master`. - If the maintainer requests further changes just push them to your
+branch. The PR will be updated automatically. - Once the pull request is
+approved and merged you can pull the changes from `upstream` to your local repo
+and delete your extra branch(es).  ## Contact Bord4 - bord4@bt.no
```

### Comparing `orion_nais-0.1.1/orion/client.py` & `orion_nais-0.1.2/orion/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,55 +46,56 @@
 
     """Interface to Barentswatch API
 
     The CLIENT_ID and CLIENT_SECRET should be exposed as environment variables called
     `CLIENT_ID` and `CLIENT_SECRET` or passed as parameters
     when creating an instance of the class.
 
-    >>>  orion = Orion(client_id="myclientid", client_secret="myclientsecret")
+    orion = Orion(client_id="myclientid", client_secret="myclientsecret")
+
+    Args:
+            client_id (Optional[str]): id for your user at Barentswatch.
+                Use if not set in .env file.
+            client_secret (Optional[str]): secret for your user at Barentswatch.
+                Use if not set in .env file.
+            skip_auth (Optional[bool]): skip authentication. Useful for testing.
     """
 
     def __init__(
         self,
         client_id: Optional[str] = None,
         client_secret: Optional[str] = None,
         skip_auth: Optional[bool] = False,
     ) -> None:
-        """
-        Args:
-            client_id (str): id for your user at Barentswatch.
-            client_secret (str): secret for your user at Barentswatch.
-            skip_auth (Optional[bool]): skip authentication. Useful for testing.
-        """
-        if not skip_auth:
-            self.client_id = client_id or CLIENT_ID
-            self.client_secret = client_secret or CLIENT_SECRET
-
-            if (not self.client_id) | (
-                not self.client_secret
-            ):  # pragma: no cover # noqa
-                raise ValueError(
-                    """
+
+        if skip_auth:
+            return
+        self.client_id = client_id or CLIENT_ID
+        self.client_secret = client_secret or CLIENT_SECRET
+
+        if (not self.client_id) | (not self.client_secret):  # pragma: no cover # noqa
+            raise ValueError(
+                """
                     Please either set CLIENT_ID and CLIENT_SECRET in .env file
                     or provide them when creating an instance of the class
                     """
-                )
+            )
 
-            if type(self.client_id) == str:  # pragma: no cover
-                self.client_id = urllib.parse.quote_plus(self.client_id)
-            if type(self.client_secret) == str:  # pragma: no cover
-                self.client_secret = urllib.parse.quote_plus(self.client_secret)
-
-            self.authenticate_session = requests.Session()  # Session for tokens
-            self.authenticate()
-            self.access = ""
-
-            self.session = requests.Session()
-            self.session.auth = self.auth  # type: ignore
-            self.session.hooks["response"].append(self.reauth)
+        if type(self.client_id) == str:  # pragma: no cover
+            self.client_id = urllib.parse.quote_plus(self.client_id)
+        if type(self.client_secret) == str:  # pragma: no cover
+            self.client_secret = urllib.parse.quote_plus(self.client_secret)
+
+        self.authenticate_session = requests.Session()  # Session for tokens
+        self.authenticate()
+        self.access = ""
+
+        self.session = requests.Session()
+        self.session.auth = self.auth  # type: ignore
+        self.session.hooks["response"].append(self.reauth)
 
     def reauth(  # type: ignore
         self, response: requests.models.Response, *args, **kwargs
     ) -> requests.models.Response:
         if response.status_code != requests.codes.unauthorized:
             return response
         logger.info("Fetching new token as the previous token expired")
```

### Comparing `orion_nais-0.1.1/orion/mmsi.py` & `orion_nais-0.1.2/orion/mmsi.py`

 * *Files 5% similar despite different names*

```diff
@@ -301,21 +301,30 @@
         Jurisdiction("UY", "770", "Uruguay"),
         Jurisdiction("VE", "775", "Venezuela"),
     ]
 
 
 @dataclass
 class Jurisdiction:
+    """
+    Represents a jurisdiction. A jurisdiction is a country or a group of countries
+    """
     name: str
     midcode: str
     full_name: str
 
 
 @dataclass
 class Mmsi:
+    """
+    Used for working with MMSI numbers. MMSI numbers are used to identify ships.
+    Has utility methods for checking if a MMSI is a ship and
+    getting the MID code for a ship. Also for filtering on country codes.
+
+    """
     jurisdictions: List[Jurisdiction] = field(default_factory=make_jurisdictions)
 
     def is_valid_ship_mmsi(self, mmsi: int) -> bool:
         """check if mmsi is a ship.
 
         Args:
             mmsi (int): mmsi number
```

### Comparing `orion_nais-0.1.1/orion/utils/get_data.py` & `orion_nais-0.1.2/orion/utils/get_data.py`

 * *Files identical despite different names*

### Comparing `orion_nais-0.1.1/orion/vessel_codes.py` & `orion_nais-0.1.2/orion/vessel_codes.py`

 * *Files 0% similar despite different names*

```diff
@@ -576,22 +576,32 @@
             "Towing Vessel",
         ),
     ]
 
 
 @dataclass
 class AisVesselCode:
+    """
+    Represents a vessel type code. A vessel code is a number that
+    represents a type of vessel. Either as a single number or a range of numbers.
+    Example: Vesel code 51 is a Search and Rescue vessel
+    """
+
     name: str
     fromCode: int
     toCode: int
     description: str
 
 
 @dataclass
 class AisVesselCodes:
+    """
+    Class to look up vessel codes and different utility functions for vessel codes.
+    """
+
     codes: List[AisVesselCode] = field(default_factory=make_vessel_codes)
 
     def get_vessel_type(self, code: int) -> Optional[AisVesselCode]:
         """Find a vessel type by code
 
         Args:
             code (int): the vessel code to search for
```

### Comparing `orion_nais-0.1.1/pyproject.toml` & `orion_nais-0.1.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 [tool.poetry]
 name = "orion-nais"
-version = "0.1.1"
+version = "0.1.2"
 description = "A client for the NAIS API from FThe Norwegian Coastal Administration"
 authors = ["Lasse Lambrechts <lasse.lambrechts@bt.no>"]
+license = "MIT"
+repository = "https://github.com/BergensTidende/orion-nais"
 readme = "README.md"
 packages = [{include = "orion"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 geopandas = "^0.12.2"
 pandas = "^1.5.2"
@@ -23,15 +25,25 @@
 types-requests = "^2.28.11.7"
 bump2version = "^1.0.1"
 pytest = "^7.2.1"
 pytest-cov = "^4.0.0"
 pyogrio = "^0.5.1"
 deepdiff = "^6.2.3"
 types-pytz = "^2022.7.1.0"
-sphinx = "^6.1.3"
+
+[tool.poetry.group.docs]
+optional = true
+
+[tool.poetry.group.docs.dependencies]
+Sphinx = "^5.3"
+sphinx-copybutton = "^0.5.2"
+sphinx-rtd-theme = "^1.1"
+m2r = "^0.3.1"
+attrs = "^22"
+sphinx-autodoc-typehints = "^1.23.0"
 
 [tool.isort]
 profile = "black"
 
 [tool.mypy]
 # 3rd party import
 ignore_missing_imports = true
```

### Comparing `orion_nais-0.1.1/setup.py` & `orion_nais-0.1.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,22 +13,22 @@
  'python-dotenv>=0.21.0,<0.22.0',
  'pytz>=2022.7.1,<2023.0.0',
  'requests>=2.28.0,<3.0.0',
  'shapely>=2.0.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'orion-nais',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': 'A client for the NAIS API from FThe Norwegian Coastal Administration',
-    'long_description': '# Orion-NAIS\n\n\n<!-- TABLE OF CONTENTS -->\n<details open="open">\n  <summary><h2 style="display: inline-block">Table of Contents</h2></summary>\n  <ol>\n    <li>\n      <a href="#about-the-project">About The Project</a>\n      <ul>\n        <li><a href="#requirements">Requirements</a></li>\n        <li><a href="#structure">Structure</a></li>\n      </ul>\n    </li>\n    <li>\n      <a href="#getting-started">Getting Started</a>\n      <ul>\n        <li><a href="#prerequisites">Prerequisites</a></li>\n        <li><a href="#installation">Installation</a></li>\n      </ul>\n    </li>\n    <li><a href="#usage">Usage</a></li>\n    <li><a href="#contributing">Contributing</a></li>\n    <li><a href="#contact">Contact</a></li>\n  </ol>\n</details>\n\n<!-- ABOUT THE PROJECT -->\n\n## About The Project\n\nOrion-NAIS is a client to work with the NAIS API. It helps with authentication and provides a simple interface to work with the API.\n\nWhen working with the API you need to have a valid token. The token is valid for a set period of time. The client will automatically refresh the token when it expires.\n\n### Why the name Orion?\n\nThe NAIS Api is provided through BarentsWatch. BarentsWatch is a Norwegian information portal that provides overview of activity and knowledge in coastal and sea areas. The Norwegian movie "Orion\'s Belt" from 1985 is an action movie set in the Barents region. About three men, a bulldozer, a Russian helicopter and a ship. Thus the name Orion.\n\n## Installation\n\nRequires Python 3.10 or later.\n\n```bash\n\npip install orion-nais\n\n```\n\nor using pipenv:\n\n```bash\n\npipenv install orion-nais\n\n```\n\nor using poetry:\n\n```bash\npoetry add orion-nais\n```\n\n## Usage\n\nThere are a heap of functions for you to use. Enjoy.\n\n## Local development\n\n### Requirements\n---\n\n- pyenv - manage python versions\n- poetry - manage python dependencies\n\nTo install on mac you can use homebrew:\n\n```bash\nbrew upgrade\nbrew install pyenv\n```\n\nYou can either install poetry with homebrew or the way described in the [documentation](https://python-poetry.org/docs/#installation)\n\n\n### Makefile commands\n\n- `make lint`\n  - lint the code in the src folder with black, isort and flake8. Mypy will check for correct typing.\n- `make format`\n  - format the code in the src folder with black and isort.\n- `make test`\n  - run the tests in the tests folder.\n- `make bump-patch`\n  - bump the patch version of the package. Example: 0.1.0 -> 0.1.1\n- `make bump-minor`\n  - bump the minor version of the package. Example: 0.1.0 -> 0.2.0\n- `make bump-major`\n  - bump the major version of the package. Example: 0.1.0 -> 1.0.0 \n- `make release`\n  - publish the package to pypi. You need to have an account and be logged in to pypi.\n\n\n### Structure\n\n```\n.\n├── .bumpversion.cfg\n├── .editorconfig\n├── .flake8\n├── .gitignore\n├── Makefile\n├── README.md\n├── orion\n│   ├── client.py\n│   ├── mmsi.py\n│   ├── types\n│   │   └── ais.py\n│   ├── urls.py\n│   ├── utils\n│   │   └── get_data.py\n│   └── vessel_codes.py\n├── poetry.lock\n├── pyproject.toml\n└── tests\n    ├── make_mock_data.py\n    ├── mocks\n    └── test_orion.py\n    \n```\n\n- `.bumpversion.cfg`\n  - Configuration file for bumpversion.\n- `.editorconfig`\n  - Configuration file for editorconfig.\n- `.flake8`\n  - Configuration file for flake8.\n- `.gitignore`\n  - Configuration file for git.\n- `pyproject.toml`\n  - Configuration file for poetry. Mypy and isort is configured here.\n- `poetry.lock`\n  - Lock file for poetry.\n- `Makefile`\n  - Makefile for the project. Here you can find commands for linting and formatting.\n- `README.md`\n  - This file.\n- `orion`\n  - The source code for the package.\n  - `client.py`\n    - The client class.\n  - `mmsi.py`\n    - A dataclass for handling MMSI numbers and MID-codes (jurisdiction).\n  - `types`\n    - A folder for types.\n    - `ais.py`\n      - A class for handling AIS messages.\n  - `urls.py`\n    - A file with urls for the API.\n  - `utils`\n    - A folder for utility functions.\n    - `get_data.py`\n      - A function for getting data from other sources. Not used by the Orion client. Contains code for getting data from the Norwegian Petroleum Directorate.\n  - `vessel_codes.py`\n    - A dataclass for looking up vessel codes.\n- `tests`\n  - Tests for the package.\n\n## Usage\n\nTo install the package in your project run\n\n```bash\n\npoetry add orion-nais\n```\n\n## Contributing\n\nDo you have write permissions to the repo? Then you can clone this project to a folder on your computer.\n\n```bash\ngit clone https://github.com/BergensTidende/orion-nais.git\n```\n\nIf not do the following:\n\n- Create a personal fork of the project on Github.\n- Clone the fork on your local machine. Your remote repo on Github is called `origin`.\n- Add the original repository as a remote called `upstream`.\n- If you created your fork a while ago be sure to pull upstream changes into your local repository.\n\nThis will clone the repo into `pakkenellik`. \n\nCreate a branch for your changes\n\n```bash\ngit checkout -b name-of-branch\n```\n\nMake your changes, rememeber to commit. And always write your commit messages in the present tense. Your commit message should describe what the commit, when applied, does to the code – not what you did to the code.\n\nIf you\'re working on a clone push the branch to github and make PR.\n\nIf your\'re working a fork:\n\n- Squash your commits into a single commit with git\'s [interactive rebase](https://help.github.com/articles/interactive-rebase). Create a new branch if necessary.\n- Push your branch to your fork on Github, the remote `origin`.\n- From your fork open a pull request in the correct branch. Target the project\'s `develop` branch if there is one, else go for `master`!\n- …\n- If the maintainer requests further changes just push them to your branch. The PR will be updated automatically.\n- Once the pull request is approved and merged you can pull the changes from `upstream` to your local repo and delete\n  your extra branch(es).\n\n <!-- CONTACT -->\n\n## Contact\n\nBord4 - bord4@bt.no\n',
+    'long_description': '# Orion-NAIS\n\n\n<!-- TABLE OF CONTENTS -->\n<details open="open">\n  <summary><h2 style="display: inline-block">Table of Contents</h2></summary>\n  <ol>\n    <li>\n      <a href="#about-the-project">About The Project</a>\n      <ul>\n        <li><a href="#requirements">Why the nanme Orion?</a></li>\n      </ul>\n    </li>\n    <li>\n      <a href="#installation">Installation</a>\n    </li>\n    <li><a href="#usage">Usage</a></li>\n    <li><a href="#local-development">Local development</a>\n      <ul>\n        <li><a href="#requirements">Requirements</a></li>\n        <li><a href="#makefile-commands">Makefile commands</a></li>\n        <li><a href="#structure">Structure</a></li>\n      </ul>\n    </li>\n    <li><a href="#contributing">Contributing</a></li>\n    <li><a href="#contact">Contact</a></li>\n  </ol>\n</details>\n\n<!-- ABOUT THE PROJECT -->\n\n## About The Project\n\nOrion-NAIS is a client to work with the NAIS API. It helps with authentication and provides a simple interface to work with the API.\n\nWhen working with the API you need to have a valid token. The token is valid for a set period of time. The client will automatically refresh the token when it expires.\n\n### Why the name Orion?\n\nThe NAIS Api is provided through BarentsWatch. BarentsWatch is a Norwegian information portal that provides overview of activity and knowledge in coastal and sea areas. The Norwegian movie "Orion\'s Belt" from 1985 is an action movie set in the Barents region. About three men, a bulldozer, a Russian helicopter and a ship. Thus the name Orion.\n\n## Installation\n\nRequires Python 3.10 or later.\n\n```bash\n\npip install orion-nais\n\n```\n\nor using pipenv:\n\n```bash\n\npipenv install orion-nais\n\n```\n\nor using poetry:\n\n```bash\npoetry add orion-nais\n```\n\n## Usage\n\nTo install the package in your project run\n\n```bash\n\npoetry add orion-nais\n```\n\nthen add an .env file to your project with the following variables:\n\n```bash\nCLIENT_ID=\nCLIENT_SECRET=\n```\n\nIf you don\'t have a client id and secret you can get one from your [BarentsWatch account](https://www.barentswatch.no/minside/).\n\nThen you can use the client like this:\n\n```python\nfrom orion import Orion\n\norion = Orion()\n# Get the last 24 hours of AIS data for a ship with MMSI XXXXXXXXXX\nais = orion.get_ais_last_24H(SHIP_MMSI)\n# Convert the AIS data to a line\nline = orion.ais_to_line(ais)\n\n```\n\n## Local development\n\n### Requirements\n- pyenv - manage python versions\n- poetry - manage python dependencies\n\nTo install on mac you can use homebrew:\n\n```bash\nbrew upgrade\nbrew install pyenv\n```\n\nYou can either install poetry with homebrew or the way described in the [documentation](https://python-poetry.org/docs/#installation)\n\n\n### Makefile commands\n\n- `make lint`\n  - lint the code in the src folder with black, isort and flake8. Mypy will check for correct typing.\n- `make format`\n  - format the code in the src folder with black and isort.\n- `make test`\n  - run the tests in the tests folder.\n- `make bump-patch`\n  - bump the patch version of the package. Example: 0.1.0 -> 0.1.1\n- `make bump-minor`\n  - bump the minor version of the package. Example: 0.1.0 -> 0.2.0\n- `make bump-major`\n  - bump the major version of the package. Example: 0.1.0 -> 1.0.0 \n- `make release`\n  - publish the package to pypi. You need to have an account and be logged in to pypi.\n\n\n### Structure\n\n```\n.\n├── .bumpversion.cfg\n├── .editorconfig\n├── .flake8\n├── .gitignore\n├── Makefile\n├── README.md\n├── orion\n│   ├── client.py\n│   ├── mmsi.py\n│   ├── types\n│   │   └── ais.py\n│   ├── urls.py\n│   ├── utils\n│   │   └── get_data.py\n│   └── vessel_codes.py\n├── poetry.lock\n├── pyproject.toml\n└── tests\n    ├── make_mock_data.py\n    ├── mocks\n    └── test_orion.py\n    \n```\n\n- `.bumpversion.cfg`\n  - Configuration file for bumpversion.\n- `.editorconfig`\n  - Configuration file for editorconfig.\n- `.flake8`\n  - Configuration file for flake8.\n- `.gitignore`\n  - Configuration file for git.\n- `pyproject.toml`\n  - Configuration file for poetry. Mypy and isort is configured here.\n- `poetry.lock`\n  - Lock file for poetry.\n- `Makefile`\n  - Makefile for the project. Here you can find commands for linting and formatting.\n- `README.md`\n  - This file.\n- `orion`\n  - The source code for the package.\n  - `client.py`\n    - The client class.\n  - `mmsi.py`\n    - A dataclass for handling MMSI numbers and MID-codes (jurisdiction).\n  - `types`\n    - A folder for types.\n    - `ais.py`\n      - A class for handling AIS messages.\n  - `urls.py`\n    - A file with urls for the API.\n  - `utils`\n    - A folder for utility functions.\n    - `get_data.py`\n      - A function for getting data from other sources. Not used by the Orion client. Contains code for getting data from the Norwegian Petroleum Directorate.\n  - `vessel_codes.py`\n    - A dataclass for looking up vessel codes.\n- `tests`\n  - Tests for the package.\n\n## Contributing\n\nDo you have write permissions to the repo? Then you can clone this project to a folder on your computer.\n\n```bash\ngit clone https://github.com/BergensTidende/orion-nais.git\n```\n\nIf not do the following:\n\n- Create a personal fork of the project on Github.\n- Clone the fork on your local machine. Your remote repo on Github is called `origin`.\n- Add the original repository as a remote called `upstream`.\n- If you created your fork a while ago be sure to pull upstream changes into your local repository.\n\nThis will clone the repo into `orion-nais`. \n\nCreate a branch for your changes\n\n```bash\ngit checkout -b name-of-branch\n```\n\nMake your changes, rememeber to commit. And always write your commit messages in the present tense. Your commit message should describe what the commit, when applied, does to the code – not what you did to the code.\n\nIf you\'re working on a clone push the branch to github and make PR.\n\nIf your\'re working a fork:\n\n- Squash your commits into a single commit with git\'s [interactive rebase](https://help.github.com/articles/interactive-rebase). Create a new branch if necessary.\n- Push your branch to your fork on Github, the remote `origin`.\n- From your fork open a pull request in the correct branch. Target the project\'s `develop` branch if there is one, else go for `master`.\n- If the maintainer requests further changes just push them to your branch. The PR will be updated automatically.\n- Once the pull request is approved and merged you can pull the changes from `upstream` to your local repo and delete\n  your extra branch(es).\n\n <!-- CONTACT -->\n\n## Contact\n\nBord4 - bord4@bt.no\n',
     'author': 'Lasse Lambrechts',
     'author_email': 'lasse.lambrechts@bt.no',
     'maintainer': 'None',
     'maintainer_email': 'None',
-    'url': 'None',
+    'url': 'https://github.com/BergensTidende/orion-nais',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'python_requires': '>=3.10,<4.0',
 }
```

#### html2text {}

```diff
@@ -1,67 +1,76 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['orion',
 'orion.types', 'orion.utils'] package_data = \ {'': ['*']} install_requires = \
 ['geopandas>=0.12.2,<0.13.0', 'pandas>=1.5.2,<2.0.0', 'python-
 dotenv>=0.21.0,<0.22.0', 'pytz>=2022.7.1,<2023.0.0', 'requests>=2.28.0,<3.0.0',
 'shapely>=2.0.0,<3.0.0'] setup_kwargs = { 'name': 'orion-nais', 'version':
-'0.1.1', 'description': 'A client for the NAIS API from FThe Norwegian Coastal
+'0.1.2', 'description': 'A client for the NAIS API from FThe Norwegian Coastal
 Administration', 'long_description': '# Orion-NAIS\n\n\n\n\n
 ***** Table of Contents *****
 \n
    1. \n
    2. \n About_The_Project\n
           o \n
-          o Requirements
-          o \n
-          o Structure
+          o Why_the_nanme_Orion?
           o \n
       \n
    3. \n
-   4. \n Getting_Started\n
+   4. \n Installation\n
+   5. \n
+   6. Usage
+   7. \n
+   8. Local_development\n
           o \n
-          o Prerequisites
+          o Requirements
+          o \n
+          o Makefile_commands
           o \n
-          o Installation
+          o Structure
           o \n
       \n
-   5. \n
-   6. Usage
-   7. \n
-   8. Contributing
    9. \n
-  10. Contact
+  10. Contributing
   11. \n
+  12. Contact
+  13. \n
 \n\n\n\n\n## About The Project\n\nOrion-NAIS is a client to work with the NAIS
 API. It helps with authentication and provides a simple interface to work with
 the API.\n\nWhen working with the API you need to have a valid token. The token
 is valid for a set period of time. The client will automatically refresh the
 token when it expires.\n\n### Why the name Orion?\n\nThe NAIS Api is provided
 through BarentsWatch. BarentsWatch is a Norwegian information portal that
 provides overview of activity and knowledge in coastal and sea areas. The
 Norwegian movie "Orion\'s Belt" from 1985 is an action movie set in the Barents
 region. About three men, a bulldozer, a Russian helicopter and a ship. Thus the
 name Orion.\n\n## Installation\n\nRequires Python 3.10 or
 later.\n\n```bash\n\npip install orion-nais\n\n```\n\nor using pipenv:
 \n\n```bash\n\npipenv install orion-nais\n\n```\n\nor using poetry:
-\n\n```bash\npoetry add orion-nais\n```\n\n## Usage\n\nThere are a heap of
-functions for you to use. Enjoy.\n\n## Local development\n\n### Requirements\n-
---\n\n- pyenv - manage python versions\n- poetry - manage python
-dependencies\n\nTo install on mac you can use homebrew:\n\n```bash\nbrew
-upgrade\nbrew install pyenv\n```\n\nYou can either install poetry with homebrew
-or the way described in the [documentation](https://python-poetry.org/docs/
-#installation)\n\n\n### Makefile commands\n\n- `make lint`\n - lint the code in
-the src folder with black, isort and flake8. Mypy will check for correct
-typing.\n- `make format`\n - format the code in the src folder with black and
-isort.\n- `make test`\n - run the tests in the tests folder.\n- `make bump-
-patch`\n - bump the patch version of the package. Example: 0.1.0 -> 0.1.1\n-
-`make bump-minor`\n - bump the minor version of the package. Example: 0.1.0 -
-> 0.2.0\n- `make bump-major`\n - bump the major version of the package.
-Example: 0.1.0 -> 1.0.0 \n- `make release`\n - publish the package to pypi. You
-need to have an account and be logged in to pypi.\n\n\n###
-Structure\n\n```\n.\nâââ .bumpversion.cfg\nâââ
+\n\n```bash\npoetry add orion-nais\n```\n\n## Usage\n\nTo install the package
+in your project run\n\n```bash\n\npoetry add orion-nais\n```\n\nthen add an
+.env file to your project with the following variables:
+\n\n```bash\nCLIENT_ID=\nCLIENT_SECRET=\n```\n\nIf you don\'t have a client id
+and secret you can get one from your [BarentsWatch account](https://
+www.barentswatch.no/minside/).\n\nThen you can use the client like this:
+\n\n```python\nfrom orion import Orion\n\norion = Orion()\n# Get the last 24
+hours of AIS data for a ship with MMSI XXXXXXXXXX\nais = orion.get_ais_last_24H
+(SHIP_MMSI)\n# Convert the AIS data to a line\nline = orion.ais_to_line
+(ais)\n\n```\n\n## Local development\n\n### Requirements\n- pyenv - manage
+python versions\n- poetry - manage python dependencies\n\nTo install on mac you
+can use homebrew:\n\n```bash\nbrew upgrade\nbrew install pyenv\n```\n\nYou can
+either install poetry with homebrew or the way described in the [documentation]
+(https://python-poetry.org/docs/#installation)\n\n\n### Makefile commands\n\n-
+`make lint`\n - lint the code in the src folder with black, isort and flake8.
+Mypy will check for correct typing.\n- `make format`\n - format the code in the
+src folder with black and isort.\n- `make test`\n - run the tests in the tests
+folder.\n- `make bump-patch`\n - bump the patch version of the package.
+Example: 0.1.0 -> 0.1.1\n- `make bump-minor`\n - bump the minor version of the
+package. Example: 0.1.0 -> 0.2.0\n- `make bump-major`\n - bump the major
+version of the package. Example: 0.1.0 -> 1.0.0 \n- `make release`\n - publish
+the package to pypi. You need to have an account and be logged in to
+pypi.\n\n\n### Structure\n\n```\n.\nâââ .bumpversion.cfg\nâââ
 .editorconfig\nâââ .flake8\nâââ .gitignore\nâââ
 Makefile\nâââ README.md\nâââ orion\nâ âââ client.py\nâ
 âââ mmsi.py\nâ âââ types\nâ â âââ ais.py\nâ âââ
 urls.py\nâ âââ utils\nâ â âââ get_data.py\nâ âââ
 vessel_codes.py\nâââ poetry.lock\nâââ pyproject.toml\nâââ
 tests\n âââ make_mock_data.py\n âââ mocks\n âââ
 test_orion.py\n \n```\n\n- `.bumpversion.cfg`\n - Configuration file for
@@ -75,35 +84,34 @@
 dataclass for handling MMSI numbers and MID-codes (jurisdiction).\n - `types`\n
 - A folder for types.\n - `ais.py`\n - A class for handling AIS messages.\n -
 `urls.py`\n - A file with urls for the API.\n - `utils`\n - A folder for
 utility functions.\n - `get_data.py`\n - A function for getting data from other
 sources. Not used by the Orion client. Contains code for getting data from the
 Norwegian Petroleum Directorate.\n - `vessel_codes.py`\n - A dataclass for
 looking up vessel codes.\n- `tests`\n - Tests for the package.\n\n##
-Usage\n\nTo install the package in your project run\n\n```bash\n\npoetry add
-orion-nais\n```\n\n## Contributing\n\nDo you have write permissions to the
-repo? Then you can clone this project to a folder on your
-computer.\n\n```bash\ngit clone https://github.com/BergensTidende/orion-
-nais.git\n```\n\nIf not do the following:\n\n- Create a personal fork of the
-project on Github.\n- Clone the fork on your local machine. Your remote repo on
-Github is called `origin`.\n- Add the original repository as a remote called
-`upstream`.\n- If you created your fork a while ago be sure to pull upstream
-changes into your local repository.\n\nThis will clone the repo into
-`pakkenellik`. \n\nCreate a branch for your changes\n\n```bash\ngit checkout -
-b name-of-branch\n```\n\nMake your changes, rememeber to commit. And always
-write your commit messages in the present tense. Your commit message should
-describe what the commit, when applied, does to the code â not what you did
-to the code.\n\nIf you\'re working on a clone push the branch to github and
-make PR.\n\nIf your\'re working a fork:\n\n- Squash your commits into a single
-commit with git\'s [interactive rebase](https://help.github.com/articles/
-interactive-rebase). Create a new branch if necessary.\n- Push your branch to
-your fork on Github, the remote `origin`.\n- From your fork open a pull request
-in the correct branch. Target the project\'s `develop` branch if there is one,
-else go for `master`!\n- â¦\n- If the maintainer requests further changes just
-push them to your branch. The PR will be updated automatically.\n- Once the
-pull request is approved and merged you can pull the changes from `upstream` to
-your local repo and delete\n your extra branch(es).\n\n \n\n## Contact\n\nBord4
-- bord4@bt.no\n', 'author': 'Lasse Lambrechts', 'author_email':
+Contributing\n\nDo you have write permissions to the repo? Then you can clone
+this project to a folder on your computer.\n\n```bash\ngit clone https://
+github.com/BergensTidende/orion-nais.git\n```\n\nIf not do the following:\n\n-
+Create a personal fork of the project on Github.\n- Clone the fork on your
+local machine. Your remote repo on Github is called `origin`.\n- Add the
+original repository as a remote called `upstream`.\n- If you created your fork
+a while ago be sure to pull upstream changes into your local
+repository.\n\nThis will clone the repo into `orion-nais`. \n\nCreate a branch
+for your changes\n\n```bash\ngit checkout -b name-of-branch\n```\n\nMake your
+changes, rememeber to commit. And always write your commit messages in the
+present tense. Your commit message should describe what the commit, when
+applied, does to the code â not what you did to the code.\n\nIf you\'re
+working on a clone push the branch to github and make PR.\n\nIf your\'re
+working a fork:\n\n- Squash your commits into a single commit with git\'s
+[interactive rebase](https://help.github.com/articles/interactive-rebase).
+Create a new branch if necessary.\n- Push your branch to your fork on Github,
+the remote `origin`.\n- From your fork open a pull request in the correct
+branch. Target the project\'s `develop` branch if there is one, else go for
+`master`.\n- If the maintainer requests further changes just push them to your
+branch. The PR will be updated automatically.\n- Once the pull request is
+approved and merged you can pull the changes from `upstream` to your local repo
+and delete\n your extra branch(es).\n\n \n\n## Contact\n\nBord4 -
+bord4@bt.no\n', 'author': 'Lasse Lambrechts', 'author_email':
 'lasse.lambrechts@bt.no', 'maintainer': 'None', 'maintainer_email': 'None',
-'url': 'None', 'packages': packages, 'package_data': package_data,
-'install_requires': install_requires, 'python_requires': '>=3.10,<4.0', } setup
-(**setup_kwargs)
+'url': 'https://github.com/BergensTidende/orion-nais', 'packages': packages,
+'package_data': package_data, 'install_requires': install_requires,
+'python_requires': '>=3.10,<4.0', } setup(**setup_kwargs)
```

### Comparing `orion_nais-0.1.1/PKG-INFO` & `orion_nais-0.1.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,47 +1,53 @@
 Metadata-Version: 2.1
 Name: orion-nais
-Version: 0.1.1
+Version: 0.1.2
 Summary: A client for the NAIS API from FThe Norwegian Coastal Administration
+Home-page: https://github.com/BergensTidende/orion-nais
+License: MIT
 Author: Lasse Lambrechts
 Author-email: lasse.lambrechts@bt.no
 Requires-Python: >=3.10,<4.0
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: geopandas (>=0.12.2,<0.13.0)
 Requires-Dist: pandas (>=1.5.2,<2.0.0)
 Requires-Dist: python-dotenv (>=0.21.0,<0.22.0)
 Requires-Dist: pytz (>=2022.7.1,<2023.0.0)
 Requires-Dist: requests (>=2.28.0,<3.0.0)
 Requires-Dist: shapely (>=2.0.0,<3.0.0)
+Project-URL: Repository, https://github.com/BergensTidende/orion-nais
 Description-Content-Type: text/markdown
 
 # Orion-NAIS
 
 
 <!-- TABLE OF CONTENTS -->
 <details open="open">
   <summary><h2 style="display: inline-block">Table of Contents</h2></summary>
   <ol>
     <li>
       <a href="#about-the-project">About The Project</a>
       <ul>
-        <li><a href="#requirements">Requirements</a></li>
-        <li><a href="#structure">Structure</a></li>
+        <li><a href="#requirements">Why the nanme Orion?</a></li>
       </ul>
     </li>
     <li>
-      <a href="#getting-started">Getting Started</a>
+      <a href="#installation">Installation</a>
+    </li>
+    <li><a href="#usage">Usage</a></li>
+    <li><a href="#local-development">Local development</a>
       <ul>
-        <li><a href="#prerequisites">Prerequisites</a></li>
-        <li><a href="#installation">Installation</a></li>
+        <li><a href="#requirements">Requirements</a></li>
+        <li><a href="#makefile-commands">Makefile commands</a></li>
+        <li><a href="#structure">Structure</a></li>
       </ul>
     </li>
-    <li><a href="#usage">Usage</a></li>
     <li><a href="#contributing">Contributing</a></li>
     <li><a href="#contact">Contact</a></li>
   </ol>
 </details>
 
 <!-- ABOUT THE PROJECT -->
 
@@ -77,21 +83,46 @@
 
 ```bash
 poetry add orion-nais
 ```
 
 ## Usage
 
-There are a heap of functions for you to use. Enjoy.
+To install the package in your project run
+
+```bash
+
+poetry add orion-nais
+```
+
+then add an .env file to your project with the following variables:
+
+```bash
+CLIENT_ID=
+CLIENT_SECRET=
+```
+
+If you don't have a client id and secret you can get one from your [BarentsWatch account](https://www.barentswatch.no/minside/).
+
+Then you can use the client like this:
+
+```python
+from orion import Orion
+
+orion = Orion()
+# Get the last 24 hours of AIS data for a ship with MMSI XXXXXXXXXX
+ais = orion.get_ais_last_24H(SHIP_MMSI)
+# Convert the AIS data to a line
+line = orion.ais_to_line(ais)
+
+```
 
 ## Local development
 
 ### Requirements
----
-
 - pyenv - manage python versions
 - poetry - manage python dependencies
 
 To install on mac you can use homebrew:
 
 ```bash
 brew upgrade
@@ -180,23 +211,14 @@
     - `get_data.py`
       - A function for getting data from other sources. Not used by the Orion client. Contains code for getting data from the Norwegian Petroleum Directorate.
   - `vessel_codes.py`
     - A dataclass for looking up vessel codes.
 - `tests`
   - Tests for the package.
 
-## Usage
-
-To install the package in your project run
-
-```bash
-
-poetry add orion-nais
-```
-
 ## Contributing
 
 Do you have write permissions to the repo? Then you can clone this project to a folder on your computer.
 
 ```bash
 git clone https://github.com/BergensTidende/orion-nais.git
 ```
@@ -204,15 +226,15 @@
 If not do the following:
 
 - Create a personal fork of the project on Github.
 - Clone the fork on your local machine. Your remote repo on Github is called `origin`.
 - Add the original repository as a remote called `upstream`.
 - If you created your fork a while ago be sure to pull upstream changes into your local repository.
 
-This will clone the repo into `pakkenellik`. 
+This will clone the repo into `orion-nais`. 
 
 Create a branch for your changes
 
 ```bash
 git checkout -b name-of-branch
 ```
 
@@ -220,16 +242,15 @@
 
 If you're working on a clone push the branch to github and make PR.
 
 If your're working a fork:
 
 - Squash your commits into a single commit with git's [interactive rebase](https://help.github.com/articles/interactive-rebase). Create a new branch if necessary.
 - Push your branch to your fork on Github, the remote `origin`.
-- From your fork open a pull request in the correct branch. Target the project's `develop` branch if there is one, else go for `master`!
-- …
+- From your fork open a pull request in the correct branch. Target the project's `develop` branch if there is one, else go for `master`.
 - If the maintainer requests further changes just push them to your branch. The PR will be updated automatically.
 - Once the pull request is approved and merged you can pull the changes from `upstream` to your local repo and delete
   your extra branch(es).
 
  <!-- CONTACT -->
 
 ## Contact
```

#### html2text {}

```diff
@@ -1,56 +1,67 @@
-Metadata-Version: 2.1 Name: orion-nais Version: 0.1.1 Summary: A client for the
-NAIS API from FThe Norwegian Coastal Administration Author: Lasse Lambrechts
+Metadata-Version: 2.1 Name: orion-nais Version: 0.1.2 Summary: A client for the
+NAIS API from FThe Norwegian Coastal Administration Home-page: https://
+github.com/BergensTidende/orion-nais License: MIT Author: Lasse Lambrechts
 Author-email: lasse.lambrechts@bt.no Requires-Python: >=3.10,<4.0 Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-Dist:
-geopandas (>=0.12.2,<0.13.0) Requires-Dist: pandas (>=1.5.2,<2.0.0) Requires-
-Dist: python-dotenv (>=0.21.0,<0.22.0) Requires-Dist: pytz
-(>=2022.7.1,<2023.0.0) Requires-Dist: requests (>=2.28.0,<3.0.0) Requires-Dist:
-shapely (>=2.0.0,<3.0.0) Description-Content-Type: text/markdown # Orion-NAIS
+License :: OSI Approved :: MIT License Classifier: Programming Language ::
+Python :: 3 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Requires-Dist: geopandas
+(>=0.12.2,<0.13.0) Requires-Dist: pandas (>=1.5.2,<2.0.0) Requires-Dist:
+python-dotenv (>=0.21.0,<0.22.0) Requires-Dist: pytz (>=2022.7.1,<2023.0.0)
+Requires-Dist: requests (>=2.28.0,<3.0.0) Requires-Dist: shapely
+(>=2.0.0,<3.0.0) Project-URL: Repository, https://github.com/BergensTidende/
+orion-nais Description-Content-Type: text/markdown # Orion-NAIS
 ***** Table of Contents *****
    1. About_The_Project
+          o Why_the_nanme_Orion?
+   2. Installation
+   3. Usage
+   4. Local_development
           o Requirements
+          o Makefile_commands
           o Structure
-   2. Getting_Started
-          o Prerequisites
-          o Installation
-   3. Usage
-   4. Contributing
-   5. Contact
+   5. Contributing
+   6. Contact
   ## About The Project Orion-NAIS is a client to work with the NAIS API. It
 helps with authentication and provides a simple interface to work with the API.
 When working with the API you need to have a valid token. The token is valid
 for a set period of time. The client will automatically refresh the token when
 it expires. ### Why the name Orion? The NAIS Api is provided through
 BarentsWatch. BarentsWatch is a Norwegian information portal that provides
 overview of activity and knowledge in coastal and sea areas. The Norwegian
 movie "Orion's Belt" from 1985 is an action movie set in the Barents region.
 About three men, a bulldozer, a Russian helicopter and a ship. Thus the name
 Orion. ## Installation Requires Python 3.10 or later. ```bash pip install
 orion-nais ``` or using pipenv: ```bash pipenv install orion-nais ``` or using
-poetry: ```bash poetry add orion-nais ``` ## Usage There are a heap of
-functions for you to use. Enjoy. ## Local development ### Requirements --- -
-pyenv - manage python versions - poetry - manage python dependencies To install
-on mac you can use homebrew: ```bash brew upgrade brew install pyenv ``` You
-can either install poetry with homebrew or the way described in the
-[documentation](https://python-poetry.org/docs/#installation) ### Makefile
-commands - `make lint` - lint the code in the src folder with black, isort and
-flake8. Mypy will check for correct typing. - `make format` - format the code
-in the src folder with black and isort. - `make test` - run the tests in the
-tests folder. - `make bump-patch` - bump the patch version of the package.
-Example: 0.1.0 -> 0.1.1 - `make bump-minor` - bump the minor version of the
-package. Example: 0.1.0 -> 0.2.0 - `make bump-major` - bump the major version
-of the package. Example: 0.1.0 -> 1.0.0 - `make release` - publish the package
-to pypi. You need to have an account and be logged in to pypi. ### Structure
-``` . âââ .bumpversion.cfg âââ .editorconfig âââ .flake8
-âââ .gitignore âââ Makefile âââ README.md âââ orion â
-âââ client.py â âââ mmsi.py â âââ types â â âââ
-ais.py â âââ urls.py â âââ utils â â âââ get_data.py
-â âââ vessel_codes.py âââ poetry.lock âââ pyproject.toml
+poetry: ```bash poetry add orion-nais ``` ## Usage To install the package in
+your project run ```bash poetry add orion-nais ``` then add an .env file to
+your project with the following variables: ```bash CLIENT_ID= CLIENT_SECRET=
+``` If you don't have a client id and secret you can get one from your
+[BarentsWatch account](https://www.barentswatch.no/minside/). Then you can use
+the client like this: ```python from orion import Orion orion = Orion() # Get
+the last 24 hours of AIS data for a ship with MMSI XXXXXXXXXX ais =
+orion.get_ais_last_24H(SHIP_MMSI) # Convert the AIS data to a line line =
+orion.ais_to_line(ais) ``` ## Local development ### Requirements - pyenv -
+manage python versions - poetry - manage python dependencies To install on mac
+you can use homebrew: ```bash brew upgrade brew install pyenv ``` You can
+either install poetry with homebrew or the way described in the [documentation]
+(https://python-poetry.org/docs/#installation) ### Makefile commands - `make
+lint` - lint the code in the src folder with black, isort and flake8. Mypy will
+check for correct typing. - `make format` - format the code in the src folder
+with black and isort. - `make test` - run the tests in the tests folder. -
+`make bump-patch` - bump the patch version of the package. Example: 0.1.0 -
+> 0.1.1 - `make bump-minor` - bump the minor version of the package. Example:
+0.1.0 -> 0.2.0 - `make bump-major` - bump the major version of the package.
+Example: 0.1.0 -> 1.0.0 - `make release` - publish the package to pypi. You
+need to have an account and be logged in to pypi. ### Structure ``` . âââ
+.bumpversion.cfg âââ .editorconfig âââ .flake8 âââ .gitignore
+âââ Makefile âââ README.md âââ orion â âââ client.py
+â âââ mmsi.py â âââ types â â âââ ais.py â
+âââ urls.py â âââ utils â â âââ get_data.py â
+âââ vessel_codes.py âââ poetry.lock âââ pyproject.toml
 âââ tests âââ make_mock_data.py âââ mocks âââ
 test_orion.py ``` - `.bumpversion.cfg` - Configuration file for bumpversion. -
 `.editorconfig` - Configuration file for editorconfig. - `.flake8` -
 Configuration file for flake8. - `.gitignore` - Configuration file for git. -
 `pyproject.toml` - Configuration file for poetry. Mypy and isort is configured
 here. - `poetry.lock` - Lock file for poetry. - `Makefile` - Makefile for the
 project. Here you can find commands for linting and formatting. - `README.md` -
@@ -58,29 +69,28 @@
 client class. - `mmsi.py` - A dataclass for handling MMSI numbers and MID-codes
 (jurisdiction). - `types` - A folder for types. - `ais.py` - A class for
 handling AIS messages. - `urls.py` - A file with urls for the API. - `utils` -
 A folder for utility functions. - `get_data.py` - A function for getting data
 from other sources. Not used by the Orion client. Contains code for getting
 data from the Norwegian Petroleum Directorate. - `vessel_codes.py` - A
 dataclass for looking up vessel codes. - `tests` - Tests for the package. ##
-Usage To install the package in your project run ```bash poetry add orion-nais
-``` ## Contributing Do you have write permissions to the repo? Then you can
-clone this project to a folder on your computer. ```bash git clone https://
-github.com/BergensTidende/orion-nais.git ``` If not do the following: - Create
-a personal fork of the project on Github. - Clone the fork on your local
-machine. Your remote repo on Github is called `origin`. - Add the original
-repository as a remote called `upstream`. - If you created your fork a while
-ago be sure to pull upstream changes into your local repository. This will
-clone the repo into `pakkenellik`. Create a branch for your changes ```bash git
-checkout -b name-of-branch ``` Make your changes, rememeber to commit. And
-always write your commit messages in the present tense. Your commit message
-should describe what the commit, when applied, does to the code â not what
-you did to the code. If you're working on a clone push the branch to github and
-make PR. If your're working a fork: - Squash your commits into a single commit
-with git's [interactive rebase](https://help.github.com/articles/interactive-
-rebase). Create a new branch if necessary. - Push your branch to your fork on
-Github, the remote `origin`. - From your fork open a pull request in the
-correct branch. Target the project's `develop` branch if there is one, else go
-for `master`! - â¦ - If the maintainer requests further changes just push them
-to your branch. The PR will be updated automatically. - Once the pull request
-is approved and merged you can pull the changes from `upstream` to your local
-repo and delete your extra branch(es).  ## Contact Bord4 - bord4@bt.no
+Contributing Do you have write permissions to the repo? Then you can clone this
+project to a folder on your computer. ```bash git clone https://github.com/
+BergensTidende/orion-nais.git ``` If not do the following: - Create a personal
+fork of the project on Github. - Clone the fork on your local machine. Your
+remote repo on Github is called `origin`. - Add the original repository as a
+remote called `upstream`. - If you created your fork a while ago be sure to
+pull upstream changes into your local repository. This will clone the repo into
+`orion-nais`. Create a branch for your changes ```bash git checkout -b name-of-
+branch ``` Make your changes, rememeber to commit. And always write your commit
+messages in the present tense. Your commit message should describe what the
+commit, when applied, does to the code â not what you did to the code. If
+you're working on a clone push the branch to github and make PR. If your're
+working a fork: - Squash your commits into a single commit with git's
+[interactive rebase](https://help.github.com/articles/interactive-rebase).
+Create a new branch if necessary. - Push your branch to your fork on Github,
+the remote `origin`. - From your fork open a pull request in the correct
+branch. Target the project's `develop` branch if there is one, else go for
+`master`. - If the maintainer requests further changes just push them to your
+branch. The PR will be updated automatically. - Once the pull request is
+approved and merged you can pull the changes from `upstream` to your local repo
+and delete your extra branch(es).  ## Contact Bord4 - bord4@bt.no
```

