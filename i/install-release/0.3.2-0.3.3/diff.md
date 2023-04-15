# Comparing `tmp/install_release-0.3.2.tar.gz` & `tmp/install_release-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "install_release-0.3.2.tar", max compression
+gzip compressed data, was "install_release-0.3.3.tar", max compression
```

## Comparing `install_release-0.3.2.tar` & `install_release-0.3.3.tar`

### file list

```diff
@@ -1,14 +1,13 @@
--rw-r--r--   0        0        0      295 2023-02-20 15:16:57.686311 install_release-0.3.2/InstallRelease/Makefile
--rw-r--r--   0        0        0       22 2023-02-20 15:16:57.686311 install_release-0.3.2/InstallRelease/__init__.py
--rw-r--r--   0        0        0     4856 2023-02-20 15:16:57.686311 install_release-0.3.2/InstallRelease/cli.py
--rw-r--r--   0        0        0     8560 2023-02-20 15:16:57.686311 install_release-0.3.2/InstallRelease/cli_interact.py
--rw-r--r--   0        0        0     1288 2023-02-20 15:16:57.686311 install_release-0.3.2/InstallRelease/constants.py
--rw-r--r--   0        0        0     7226 2023-02-20 15:16:57.686311 install_release-0.3.2/InstallRelease/core.py
--rw-r--r--   0        0        0     2221 2023-02-20 15:16:57.686311 install_release-0.3.2/InstallRelease/data.py
--rw-r--r--   0        0        0     2285 2023-02-20 15:16:57.686311 install_release-0.3.2/InstallRelease/state.py
--rw-r--r--   0        0        0     7351 2023-02-20 15:16:57.686311 install_release-0.3.2/InstallRelease/utils.py
--rw-r--r--   0        0        0    35149 2023-02-20 15:16:57.686311 install_release-0.3.2/LICENSE
--rw-r--r--   0        0        0     8423 2023-02-20 15:16:57.690311 install_release-0.3.2/README.md
--rw-r--r--   0        0        0      927 2023-02-20 15:16:57.690311 install_release-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     9592 1970-01-01 00:00:00.000000 install_release-0.3.2/setup.py
--rw-r--r--   0        0        0     9288 1970-01-01 00:00:00.000000 install_release-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0      295 2023-04-15 11:36:21.006124 install_release-0.3.3/InstallRelease/Makefile
+-rw-r--r--   0        0        0       22 2023-04-15 11:36:21.006124 install_release-0.3.3/InstallRelease/__init__.py
+-rw-r--r--   0        0        0     5070 2023-04-15 11:36:21.006124 install_release-0.3.3/InstallRelease/cli.py
+-rw-r--r--   0        0        0     8560 2023-04-15 11:36:21.006124 install_release-0.3.3/InstallRelease/cli_interact.py
+-rw-r--r--   0        0        0     1288 2023-04-15 11:36:21.006124 install_release-0.3.3/InstallRelease/constants.py
+-rw-r--r--   0        0        0     7226 2023-04-15 11:36:21.006124 install_release-0.3.3/InstallRelease/core.py
+-rw-r--r--   0        0        0     2221 2023-04-15 11:36:21.006124 install_release-0.3.3/InstallRelease/data.py
+-rw-r--r--   0        0        0     2285 2023-04-15 11:36:21.006124 install_release-0.3.3/InstallRelease/state.py
+-rw-r--r--   0        0        0     7351 2023-04-15 11:36:21.006124 install_release-0.3.3/InstallRelease/utils.py
+-rw-r--r--   0        0        0    35149 2023-04-15 11:36:21.006124 install_release-0.3.3/LICENSE
+-rw-r--r--   0        0        0     8430 2023-04-15 11:36:21.006124 install_release-0.3.3/README.md
+-rw-r--r--   0        0        0      927 2023-04-15 11:36:21.006124 install_release-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     9295 1970-01-01 00:00:00.000000 install_release-0.3.3/PKG-INFO
```

### Comparing `install_release-0.3.2/InstallRelease/cli.py` & `install_release-0.3.3/InstallRelease/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import sys
 import logging
 import os
 
 # pipi
 import typer
 
 # locals
@@ -83,14 +84,16 @@
     quite: bool = __optionQuite,
     force: bool = __optionForce,
 ):
     """
     | Upgrade all installed release, cli tools
     """
     setLogger(quite, debug)
+    os.system(f"{sys.executable} -m pip install -U install-release")
+
     _upgrade(force=force)
 
 
 @app.command()
 def ls(
     hold: bool = typer.Option(
         False,
@@ -210,18 +213,22 @@
     version: bool = typer.Option(
         False, "--version", help="print version this tool, install-release."
     ),
 ):
     """
     | Update install-release tool.
     """
+    import InstallRelease
+
+    _v = InstallRelease.__version__
 
     if update:
-        os.system("python3 -m pip install -U install-release")
+        os.system(f"{sys.executable} -m pip install -U install-release")
     elif version:
-        import InstallRelease
-
-        print(InstallRelease.__version__)
+        rprint(_v)
+    else:
+        rprint(f"Version: {_v}")
+        rprint(f"Repo:    https://github.com/Rishang/install-release")
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `install_release-0.3.2/InstallRelease/cli_interact.py` & `install_release-0.3.3/InstallRelease/cli_interact.py`

 * *Files identical despite different names*

### Comparing `install_release-0.3.2/InstallRelease/constants.py` & `install_release-0.3.3/InstallRelease/constants.py`

 * *Files identical despite different names*

### Comparing `install_release-0.3.2/InstallRelease/core.py` & `install_release-0.3.3/InstallRelease/core.py`

 * *Files identical despite different names*

### Comparing `install_release-0.3.2/InstallRelease/data.py` & `install_release-0.3.3/InstallRelease/data.py`

 * *Files identical despite different names*

### Comparing `install_release-0.3.2/InstallRelease/state.py` & `install_release-0.3.3/InstallRelease/state.py`

 * *Files identical despite different names*

### Comparing `install_release-0.3.2/InstallRelease/utils.py` & `install_release-0.3.3/InstallRelease/utils.py`

 * *Files identical despite different names*

### Comparing `install_release-0.3.2/LICENSE` & `install_release-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `install_release-0.3.2/README.md` & `install_release-0.3.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 ```
 
 For updating:
 ```bash
 install-release me --upgrade
 ```
 
-### Example usage `install-release`
+### Example usage `install-release --help`
 
 
 ```
 # Help page
 
 ❯ install-release --help
 Usage: install-release [OPTIONS] COMMAND [ARGS]...
```

### Comparing `install_release-0.3.2/pyproject.toml` & `install_release-0.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [virtualenvs]
 in-project = true
 
 [tool.poetry]
 name = "install-release"
-version = "0.3.2"
+version = "0.3.3"
 readme = "README.md"
 description = "A cli tool to install tools based on your device info directly from github releases and keep them updated."
 authors = ["Rishang <rishangbhavsarcs@gmail.com>"]
 packages = [
   { include = "InstallRelease" }
 ]
 homepage = "https://github.com/Rishang/install-releases"
```

### Comparing `install_release-0.3.2/setup.py` & `install_release-0.3.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,269 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: install-release
+Version: 0.3.3
+Summary: A cli tool to install tools based on your device info directly from github releases and keep them updated.
+Home-page: https://github.com/Rishang/install-releases
+Author: Rishang
+Author-email: rishangbhavsarcs@gmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: python-magic (>=0.4.27,<0.5.0)
+Requires-Dist: requests
+Requires-Dist: rich
+Requires-Dist: typer (>=0.7.0,<0.8.0)
+Description-Content-Type: text/markdown
 
-packages = \
-['InstallRelease']
+# install-release 🚀
+[![Python Version](https://img.shields.io/badge/Python-3.8_to_3.10-xx.svg)](https://shields.io/) [![Downloads](https://static.pepy.tech/personalized-badge/install-release?&units=international_system&left_color=black&right_color=orange&left_text=Downloads)](https://pepy.tech/project/install-release)
 
-package_data = \
-{'': ['*']}
+`install-release` is a cli tool to install any tool for your device directly from their github releases and keep them updated. you can consider it as a small package manager for github releases.
 
-install_requires = \
-['python-magic>=0.4.27,<0.5.0', 'requests', 'rich', 'typer>=0.7.0,<0.8.0']
-
-entry_points = \
-{'console_scripts': ['install-release = InstallRelease.cli:app']}
-
-setup_kwargs = {
-    'name': 'install-release',
-    'version': '0.3.2',
-    'description': 'A cli tool to install tools based on your device info directly from github releases and keep them updated.',
-    'long_description': '# install-release 🚀\n[![Python Version](https://img.shields.io/badge/Python-3.8_to_3.10-xx.svg)](https://shields.io/) [![Downloads](https://static.pepy.tech/personalized-badge/install-release?&units=international_system&left_color=black&right_color=orange&left_text=Downloads)](https://pepy.tech/project/install-release)\n\n`install-release` is a cli tool to install any tool for your device directly from their github releases and keep them updated. you can consider it as a small package manager for github releases.\n\nThis can be any tool you want to install, which is pre-compiled for your device and present on github releases.\n\n> INFO: It\'s mainly for installing tools that are not directly available officially by package managers like `apt, yum, pacman` etc.\n\n```bash\n# Install install-release\npip install -U install-release\n```\n\n```\n# Example Installation a tool named `gron` directly from its github releases\n\n# install-release get [GITHUB-URL]\n\n❯ install-release get https://github.com/tomnomnom/gron \n```\n\n![demo](.github/images/demo.png)\n\n\nChecking for gron is installed using installed-release:\n\n```\n❯ which gron\n/home/noobi/bin/gron\n\n❯ gron --help\nTransform JSON (from a file, URL, or stdin) into discrete assignments to make it greppable\n... # more\n```\n\n## Prerequisites\n\n- python3.8 or higher\n\n- [libmagic](https://github.com/ahupp/python-magic#installation)\n- Default releases Installation Path is: `~/bin/`,\nThis is the path where installed tools will get stored.\n\n- In order to run installed tools, you need to add the following line your `~/.bashrc` or `~/.zshrc` file:\n\n```bash\nexport PATH=$HOME/bin:$PATH\n```\n\n\n## Install this package\n\n```bash\npip install -U install-release\n```\n\n## Update this package\n\nFor seeing verison:\n```bash\ninstall-release me --version\n```\n\nFor updating:\n```bash\ninstall-release me --upgrade\n```\n\n### Example usage `install-release`\n\n\n```\n# Help page\n\n❯ install-release --help\nUsage: install-release [OPTIONS] COMMAND [ARGS]...\n\n  Github Release Installer, based on your system\n\n  Commands:\n    get      | Install github release, cli tool\n    ls       | list all installed release, cli tools\n    rm       | remove any installed release, cli tools\n    upgrade  | Upgrade all installed release, cli tools\n    state    | show currnet stored state\n    config   | Set configs for tool\n    pull     | Install tools from remote state\n    hold     | Keep updates a tool on hold.\n    me       | Update install-release tool.\n```\n\nFor sub command help use: `install-release <sub-command> --help`\n\nExample: `install-release get --help`\n\n\nYou can shorten the command by setting alias to your `.bashrc` or `.zshrc`\n\n```bash\nalias ir="install-release"\n```\nafter this you can you alias directly for easiness\n\nExample: `ir get --help`\n\n#### Install completion for shell\n```bash\n# install-release --install-completion [SHELL: bash|zsh|fish|powershell]\n# Example for zsh:\ninstall-release --install-completion zsh\n```\n\n#### Install tool from github releases\n\n```bash\n❯ install-release get "https://github.com/ahmetb/kubectx"\n\n📑 Repo     : ahmetb/kubectx\n🌟 Stars    : 13295\n✨ Language : Go\n🔥 Title    : Faster way to switch between clusters and namespaces in kubectl\n\n                              🚀 Install: kubectx                               \n┏━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━┳━━━━━━━━━┳━━━━━━━━━━━┓\n┃ Name    ┃ Selected Item                      ┃ Version ┃ Size Mb ┃ Downloads ┃\n┡━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━╇━━━━━━━━━╇━━━━━━━━━━━┩\n│ kubectx │ kubectx_v0.9.4_linux_x86_64.tar.gz │ v0.9.4  │ 1.0     │ 43811     │\n└─────────┴────────────────────────────────────┴─────────┴─────────┴───────────┘\nInstall this tool (Y/n): y\n INFO     Downloaded: \'kubectx_v0.9.4_linux_x86_64.tar.gz\' at /tmp/dn_kubectx_ph6i7dmk                                                               utils.py:159\n INFO     install /tmp/dn_kubectx_ph6i7dmk/kubectx /home/noobi/bin/kubectx                                                                  core.py:132\n INFO     Installed: kubectx\n```\n```\n# checking if kubectx is installed\n❯ which kubectx\n/home/noobi/bin/kubectx\n\n❯ kubectx --version\n0.9.4\n```\n\n#### List installed tools\n\n```bash\n❯ install-release ls\n\n                       Installed tools                        \n┏━━━━━━━━━━━┳━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┓\n┃ Name      ┃ Version ┃ Url                                  ┃\n┡━━━━━━━━━━━╇━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┩\n│ terrascan │ v1.15.2 │ https://github.com/tenable/terrascan │\n│ gron      │ v0.7.1  │ https://github.com/tomnomnom/gron    │\n│ kubectx   │ v0.9.4  │ https://github.com/ahmetb/kubectx    │\n└───────────┴─────────┴──────────────────────────────────────┘    \n```\n\n#### Remove installed release\n\n```bash\n# Remove installed release\n\n❯ install-release rm gron\n    \nINFO     Removed: gron           \n```\n\n#### Update all previously installed tools to the latest version\n\n```bash\n❯ install-release upgrade\n\nFetching: https://github.com/tenable/terrascan#terrascan\nFetching: https://github.com/ahmetb/kubectx#kubectx\n\nFollowing tools will be upgraded:\n\nterrascan\n\nUpgrade these tools, (Y/n): y\n\nUpdating: terrascan, v1.15.0 => v1.15.2\n INFO     Downloaded: \'terrascan_1.15.2_Linux_x86_64.tar.gz\' at /tmp/dn_terrascan_0as71a6v\n INFO     install /tmp/dn_terrascan_0as71a6v/terrascan ~/bin/terrascan\n INFO     Installed: terrascan\n\nProgress... ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 100% 0:00:00 \n```\n\n#### Hold Update to specific installed tool.\n\nIn case you want to hold update to specific tool, you can use `hold {tool-name}` command by which it will pause update for that tool.\n\nExample: keep tool named [k9s](https://github.com/derailed/k9s) update on hold\n\n```bash\n❯ install-release hold k9s\n INFO     Update on hold for, k9s to True\n```\n\nYou can list tools on hold updates  by `ls --hold` command\n\n```bash\n❯ install-release ls --hold\n             Installed tools kept on hold             \n┏━━━━━━┳━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┓\n┃ Name ┃ Version ┃ Url                               ┃\n┡━━━━━━╇━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┩\n│ k9s  │ v0.26.7 │ https://github.com/derailed/k9s   │\n└──────┴─────────┴───────────────────────────────────┘\n```\n\nIn case you want to unhold update to specific tool, you can use `hold --unset {tool-name}` command by which it will pause update for that tool.\n\n```\n❯ install-release hold --unset k9s\n INFO     Update on hold for, k9s to False\n```\n\n#### Config tool installation path\n\n```bash\n❯ install-release config --path ~/.local/bin\n\nINFO   updated path to:  ~/.local/bin\nINFO   Done\n```\n\n#### Config updates for pre release versions\n\nThis is useful when you want to install pre-release versions of tools like beta or alpha releases. by default it is set to `False` in which case it will only check for latest release.\n\n```bash\n❯ install-release config --pre-release\n```\n\n#### Config github to token for higher rate limit\n\n\n\n```bash\n❯ install-release config --token [your github token]\n\nINFO: Update token\nINFO: Done.\n```\n',
-    'author': 'Rishang',
-    'author_email': 'rishangbhavsarcs@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/Rishang/install-releases',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<4.0',
-}
+This can be any tool you want to install, which is pre-compiled for your device and present on github releases.
 
+> INFO: It's mainly for installing tools that are not directly available officially by package managers like `apt, yum, pacman` etc.
+
+```bash
+# Install install-release
+pip install -U install-release
+```
+
+```
+# Example Installation a tool named `gron` directly from its github releases
+
+# install-release get [GITHUB-URL]
+
+❯ install-release get https://github.com/tomnomnom/gron 
+```
+
+![demo](.github/images/demo.png)
+
+
+Checking for gron is installed using installed-release:
+
+```
+❯ which gron
+/home/noobi/bin/gron
+
+❯ gron --help
+Transform JSON (from a file, URL, or stdin) into discrete assignments to make it greppable
+... # more
+```
+
+## Prerequisites
+
+- python3.8 or higher
+
+- [libmagic](https://github.com/ahupp/python-magic#installation)
+- Default releases Installation Path is: `~/bin/`,
+This is the path where installed tools will get stored.
+
+- In order to run installed tools, you need to add the following line your `~/.bashrc` or `~/.zshrc` file:
+
+```bash
+export PATH=$HOME/bin:$PATH
+```
+
+
+## Install this package
+
+```bash
+pip install -U install-release
+```
+
+## Update this package
+
+For seeing verison:
+```bash
+install-release me --version
+```
+
+For updating:
+```bash
+install-release me --upgrade
+```
+
+### Example usage `install-release --help`
+
+
+```
+# Help page
+
+❯ install-release --help
+Usage: install-release [OPTIONS] COMMAND [ARGS]...
+
+  Github Release Installer, based on your system
+
+  Commands:
+    get      | Install github release, cli tool
+    ls       | list all installed release, cli tools
+    rm       | remove any installed release, cli tools
+    upgrade  | Upgrade all installed release, cli tools
+    state    | show currnet stored state
+    config   | Set configs for tool
+    pull     | Install tools from remote state
+    hold     | Keep updates a tool on hold.
+    me       | Update install-release tool.
+```
+
+For sub command help use: `install-release <sub-command> --help`
+
+Example: `install-release get --help`
+
+
+You can shorten the command by setting alias to your `.bashrc` or `.zshrc`
+
+```bash
+alias ir="install-release"
+```
+after this you can you alias directly for easiness
+
+Example: `ir get --help`
+
+#### Install completion for shell
+```bash
+# install-release --install-completion [SHELL: bash|zsh|fish|powershell]
+# Example for zsh:
+install-release --install-completion zsh
+```
+
+#### Install tool from github releases
+
+```bash
+❯ install-release get "https://github.com/ahmetb/kubectx"
+
+📑 Repo     : ahmetb/kubectx
+🌟 Stars    : 13295
+✨ Language : Go
+🔥 Title    : Faster way to switch between clusters and namespaces in kubectl
+
+                              🚀 Install: kubectx                               
+┏━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━┳━━━━━━━━━┳━━━━━━━━━━━┓
+┃ Name    ┃ Selected Item                      ┃ Version ┃ Size Mb ┃ Downloads ┃
+┡━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━╇━━━━━━━━━╇━━━━━━━━━━━┩
+│ kubectx │ kubectx_v0.9.4_linux_x86_64.tar.gz │ v0.9.4  │ 1.0     │ 43811     │
+└─────────┴────────────────────────────────────┴─────────┴─────────┴───────────┘
+Install this tool (Y/n): y
+ INFO     Downloaded: 'kubectx_v0.9.4_linux_x86_64.tar.gz' at /tmp/dn_kubectx_ph6i7dmk                                                               utils.py:159
+ INFO     install /tmp/dn_kubectx_ph6i7dmk/kubectx /home/noobi/bin/kubectx                                                                  core.py:132
+ INFO     Installed: kubectx
+```
+```
+# checking if kubectx is installed
+❯ which kubectx
+/home/noobi/bin/kubectx
+
+❯ kubectx --version
+0.9.4
+```
+
+#### List installed tools
+
+```bash
+❯ install-release ls
+
+                       Installed tools                        
+┏━━━━━━━━━━━┳━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┓
+┃ Name      ┃ Version ┃ Url                                  ┃
+┡━━━━━━━━━━━╇━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┩
+│ terrascan │ v1.15.2 │ https://github.com/tenable/terrascan │
+│ gron      │ v0.7.1  │ https://github.com/tomnomnom/gron    │
+│ kubectx   │ v0.9.4  │ https://github.com/ahmetb/kubectx    │
+└───────────┴─────────┴──────────────────────────────────────┘    
+```
+
+#### Remove installed release
+
+```bash
+# Remove installed release
+
+❯ install-release rm gron
+    
+INFO     Removed: gron           
+```
+
+#### Update all previously installed tools to the latest version
+
+```bash
+❯ install-release upgrade
+
+Fetching: https://github.com/tenable/terrascan#terrascan
+Fetching: https://github.com/ahmetb/kubectx#kubectx
+
+Following tools will be upgraded:
+
+terrascan
+
+Upgrade these tools, (Y/n): y
+
+Updating: terrascan, v1.15.0 => v1.15.2
+ INFO     Downloaded: 'terrascan_1.15.2_Linux_x86_64.tar.gz' at /tmp/dn_terrascan_0as71a6v
+ INFO     install /tmp/dn_terrascan_0as71a6v/terrascan ~/bin/terrascan
+ INFO     Installed: terrascan
+
+Progress... ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 100% 0:00:00 
+```
+
+#### Hold Update to specific installed tool.
+
+In case you want to hold update to specific tool, you can use `hold {tool-name}` command by which it will pause update for that tool.
+
+Example: keep tool named [k9s](https://github.com/derailed/k9s) update on hold
+
+```bash
+❯ install-release hold k9s
+ INFO     Update on hold for, k9s to True
+```
+
+You can list tools on hold updates  by `ls --hold` command
+
+```bash
+❯ install-release ls --hold
+             Installed tools kept on hold             
+┏━━━━━━┳━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┓
+┃ Name ┃ Version ┃ Url                               ┃
+┡━━━━━━╇━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┩
+│ k9s  │ v0.26.7 │ https://github.com/derailed/k9s   │
+└──────┴─────────┴───────────────────────────────────┘
+```
+
+In case you want to unhold update to specific tool, you can use `hold --unset {tool-name}` command by which it will pause update for that tool.
+
+```
+❯ install-release hold --unset k9s
+ INFO     Update on hold for, k9s to False
+```
+
+#### Config tool installation path
+
+```bash
+❯ install-release config --path ~/.local/bin
+
+INFO   updated path to:  ~/.local/bin
+INFO   Done
+```
+
+#### Config updates for pre release versions
+
+This is useful when you want to install pre-release versions of tools like beta or alpha releases. by default it is set to `False` in which case it will only check for latest release.
+
+```bash
+❯ install-release config --pre-release
+```
+
+#### Config github to token for higher rate limit
+
+
+
+```bash
+❯ install-release config --token [your github token]
+
+INFO: Update token
+INFO: Done.
+```
 
-setup(**setup_kwargs)
```

