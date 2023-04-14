# Comparing `tmp/teamtalk_py-1.1.0.tar.gz` & `tmp/teamtalk_py-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "teamtalk_py-1.1.0.tar", max compression
+gzip compressed data, was "teamtalk_py-1.1.1.tar", max compression
```

## Comparing `teamtalk_py-1.1.0.tar` & `teamtalk_py-1.1.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1058 2023-03-24 14:57:54.064768 teamtalk_py-1.1.0/LICENSE
--rw-r--r--   0        0        0     2395 2023-03-24 14:57:54.064768 teamtalk_py-1.1.0/README.md
--rw-r--r--   0        0        0     1856 2023-03-24 14:57:54.064768 teamtalk_py-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     1298 2023-03-24 14:57:54.064768 teamtalk_py-1.1.0/teamtalk/__init__.py
--rw-r--r--   0        0        0     4467 2023-03-24 14:57:54.064768 teamtalk_py-1.1.0/teamtalk/_utils.py
--rw-r--r--   0        0        0     8810 2023-03-24 14:57:54.064768 teamtalk_py-1.1.0/teamtalk/bot.py
--rw-r--r--   0        0        0     7438 2023-03-24 14:57:54.064768 teamtalk_py-1.1.0/teamtalk/channel.py
--rw-r--r--   0        0        0      254 2023-03-24 14:57:54.064768 teamtalk_py-1.1.0/teamtalk/download_sdk.py
--rw-r--r--   0        0        0     4203 2023-03-24 14:57:54.064768 teamtalk_py-1.1.0/teamtalk/enums.py
--rw-r--r--   0        0        0      571 2023-03-24 14:57:54.064768 teamtalk_py-1.1.0/teamtalk/exceptions.py
--rw-r--r--   0        0        0        0 2023-03-24 14:57:54.064768 teamtalk_py-1.1.0/teamtalk/implementation/__init__.py
--rw-r--r--   0        0        0    36085 2023-03-24 14:57:54.064768 teamtalk_py-1.1.0/teamtalk/instance.py
--rw-r--r--   0        0        0     5327 2023-03-24 14:57:54.064768 teamtalk_py-1.1.0/teamtalk/message.py
--rw-r--r--   0        0        0      426 2023-03-24 14:57:54.064768 teamtalk_py-1.1.0/teamtalk/permission.py
--rw-r--r--   0        0        0     9019 2023-03-24 14:57:54.064768 teamtalk_py-1.1.0/teamtalk/server.py
--rw-r--r--   0        0        0     8147 2023-03-24 14:57:54.064768 teamtalk_py-1.1.0/teamtalk/streamer.py
--rw-r--r--   0        0        0        0 2023-03-24 14:57:54.068768 teamtalk_py-1.1.0/teamtalk/tools/__init__.py
--rw-r--r--   0        0        0      457 2023-03-24 14:57:54.068768 teamtalk_py-1.1.0/teamtalk/tools/downloader.py
--rw-r--r--   0        0        0     3733 2023-03-24 14:57:54.068768 teamtalk_py-1.1.0/teamtalk/tools/ttsdk_downloader.py
--rw-r--r--   0        0        0     1518 2023-03-24 14:57:54.068768 teamtalk_py-1.1.0/teamtalk/tt_file.py
--rw-r--r--   0        0        0     4128 2023-03-24 14:57:54.068768 teamtalk_py-1.1.0/teamtalk/user.py
--rw-r--r--   0        0        0     1814 2023-03-24 14:57:54.068768 teamtalk_py-1.1.0/teamtalk/user_account.py
--rw-r--r--   0        0        0     3915 1970-01-01 00:00:00.000000 teamtalk_py-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-02-26 15:33:54.712304 teamtalk_py-1.1.1/LICENSE
+-rw-r--r--   0        0        0     1922 2023-04-14 23:30:40.410225 teamtalk_py-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2462 2023-04-02 02:04:57.366268 teamtalk_py-1.1.1/README.md
+-rw-r--r--   0        0        0     1331 2023-03-22 21:01:45.385889 teamtalk_py-1.1.1/teamtalk/__init__.py
+-rw-r--r--   0        0        0     4613 2023-03-22 21:01:45.386888 teamtalk_py-1.1.1/teamtalk/_utils.py
+-rw-r--r--   0        0        0     9075 2023-03-16 19:08:45.915985 teamtalk_py-1.1.1/teamtalk/bot.py
+-rw-r--r--   0        0        0     7636 2023-04-14 23:30:32.243621 teamtalk_py-1.1.1/teamtalk/channel.py
+-rw-r--r--   0        0        0      262 2023-02-26 01:27:20.843944 teamtalk_py-1.1.1/teamtalk/download_sdk.py
+-rw-r--r--   0        0        0     4332 2023-03-24 14:26:13.544726 teamtalk_py-1.1.1/teamtalk/enums.py
+-rw-r--r--   0        0        0      591 2023-02-26 01:34:42.379984 teamtalk_py-1.1.1/teamtalk/exceptions.py
+-rw-r--r--   0        0        0        0 2023-03-22 19:04:26.034320 teamtalk_py-1.1.1/teamtalk/implementation/__init__.py
+-rw-r--r--   0        0        0    36939 2023-04-14 23:30:32.244626 teamtalk_py-1.1.1/teamtalk/instance.py
+-rw-r--r--   0        0        0     5468 2023-04-14 23:30:32.245627 teamtalk_py-1.1.1/teamtalk/message.py
+-rw-r--r--   0        0        0      439 2023-02-25 17:41:42.714809 teamtalk_py-1.1.1/teamtalk/permission.py
+-rw-r--r--   0        0        0     9282 2023-03-22 21:01:45.388890 teamtalk_py-1.1.1/teamtalk/server.py
+-rw-r--r--   0        0        0     8345 2023-03-04 03:34:40.991502 teamtalk_py-1.1.1/teamtalk/streamer.py
+-rw-r--r--   0        0        0        0 2023-02-25 22:54:54.673036 teamtalk_py-1.1.1/teamtalk/tools/__init__.py
+-rw-r--r--   0        0        0      472 2023-03-22 14:14:29.605453 teamtalk_py-1.1.1/teamtalk/tools/downloader.py
+-rw-r--r--   0        0        0     3848 2023-03-22 14:14:29.606453 teamtalk_py-1.1.1/teamtalk/tools/ttsdk_downloader.py
+-rw-r--r--   0        0        0     1562 2023-02-26 00:38:18.408470 teamtalk_py-1.1.1/teamtalk/tt_file.py
+-rw-r--r--   0        0        0     4240 2023-04-14 23:30:32.246627 teamtalk_py-1.1.1/teamtalk/user.py
+-rw-r--r--   0        0        0     1861 2023-03-22 21:01:45.388890 teamtalk_py-1.1.1/teamtalk/user_account.py
+-rw-r--r--   0        0        0     3913 1970-01-01 00:00:00.000000 teamtalk_py-1.1.1/PKG-INFO
```

### Comparing `teamtalk_py-1.1.0/LICENSE` & `teamtalk_py-1.1.1/LICENSE`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,4 +1,4 @@
-Copyright 2023 JessicaTegner
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+Copyright 2023 JessicaTegner
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `teamtalk_py-1.1.0/README.md` & `teamtalk_py-1.1.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,71 +1,69 @@
-# Teamtalk.py
-
-[![Documentation](https://img.shields.io/readthedocs/teamtalkpy?style=flat-square)](http://teamtalkpy.readthedocs.io/en/latest)
-[![Build Status](https://github.com/JessicaTegner/teamtalk.py/actions/workflows/ci.yaml/badge.svg)](https://github.com/JessicaTegner/teamtalk.py/actions/workflows/ci.yaml)
-[![GitHub Releases](https://img.shields.io/github/tag/JessicaTegner/teamtalk.py.svg?style=flat-square)](https://github.com/JessicaTegner/teamtalk.py/releases)
-[![PyPI Version](https://img.shields.io/pypi/v/teamtalk.py?style=flat-square)](https://pypi.org/project/teamtalk.py/)
-[![Python versions](https://img.shields.io/pypi/pyversions/teamtalk.py.svg?style=flat-square)](https://pypi.python.org/pypi/teamtalk.py/)
-![License](https://img.shields.io/pypi/l/pypandoc.svg?style=flat-square)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](http://makeapullrequest.com)
-
-teamtalk.py is a simple but powerful pythonic library for making bots for the [TeamTalk5 Conferencing System](https://bearware.dk/)
-
-
-### Installing
-
-Python 3.8 or higher is required
-
-#### From PyPI
-
-```bash
-pip install teamtalk.py
-```
-
-#### From source
-
-```bash
-git clone https://github.com/JessicaTegner/teamtalk.py
-cd teamtalk.py
-poetry install
-```
-
-
-### Usage
-
-```python
-import teamtalk
-
-bot = teamtalk.TeamTalkBot()
-
-@bot.event
-async def on_ready():
-    test_server = teamtalk.TeamTalkServerInfo("localhost", 10335, 10335, "user", "pass")
-    await bot.add_server(test_server)
-
-@bot.event
-async def on_message(message):
-    if message.content.lower() == "ping":
-        message.reply("pong")
-
-bot.run()
-```
-
-
-## Documentation
-
-You can find the full documentation [here](http://teamtalkpy.readthedocs.io/en/latest)
-
-
-## Contributing
-
-So you want to contribute to teamtalk.py? Great! There are many ways to contribute to this project, and all contributions are welcome.
-
-If you have found a bug, have a feature request or want to help improve documentation please [open an issue](https://https://github.com/jessicaTegner/issues/new)_
-
-You can also donate to the projects maintainer (JessicaTegner) to help support the development of teamtalk.py:
-
-
-## License
-
-This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details
+# Teamtalk.py
+
+[![Documentation](https://img.shields.io/readthedocs/teamtalkpy?style=flat-square)](http://teamtalkpy.readthedocs.io/en/latest)
+[![Build Status](https://github.com/JessicaTegner/teamtalk.py/actions/workflows/ci.yaml/badge.svg)](https://github.com/JessicaTegner/teamtalk.py/actions/workflows/ci.yaml)
+[![GitHub Releases](https://img.shields.io/github/tag/JessicaTegner/teamtalk.py.svg?style=flat-square)](https://github.com/JessicaTegner/teamtalk.py/releases)
+[![PyPI Version](https://img.shields.io/pypi/v/teamtalk.py?style=flat-square)](https://pypi.org/project/teamtalk.py/)
+[![Python versions](https://img.shields.io/pypi/pyversions/teamtalk.py.svg?style=flat-square)](https://pypi.python.org/pypi/teamtalk.py/)
+![License](https://img.shields.io/pypi/l/pypandoc.svg?style=flat-square)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](http://makeapullrequest.com)
+
+teamtalk.py is a simple but powerful pythonic library for making bots for the [TeamTalk5 Conferencing System](https://bearware.dk/)
+
+
+### Installing
+
+Python 3.8 or higher is required
+
+#### From PyPI
+
+```bash
+pip install teamtalk.py
+```
+
+#### From source
+
+```bash
+git clone https://github.com/JessicaTegner/teamtalk.py
+cd teamtalk.py
+poetry install
+```
+
+
+### Usage
+
+```python
+import teamtalk
+
+bot = teamtalk.TeamTalkBot()
+
+@bot.event
+async def on_ready():
+    test_server = teamtalk.TeamTalkServerInfo("localhost", 10335, 10335, "user", "pass")
+    await bot.add_server(test_server)
+
+@bot.event
+async def on_message(message):
+    if message.content.lower() == "ping":
+        message.reply("pong")
+
+bot.run()
+```
+
+
+## Documentation
+
+You can find the full documentation [here](http://teamtalkpy.readthedocs.io/en/latest)
+
+
+## Contributing
+
+So you want to contribute to teamtalk.py? Great! There are many ways to contribute to this project, and all contributions are welcome.
+If you have found a bug, have a feature request or want to help improve documentation please [open an issue](https://https://github.com/jessicaTegner/issues/new)_
+You can also donate to the projects maintainer (JessicaTegner) to help support the development of teamtalk.py:
+
+
+## License
+
+This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details
```

### Comparing `teamtalk_py-1.1.0/pyproject.toml` & `teamtalk_py-1.1.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,66 +1,66 @@
-[tool.poetry]
-name = "teamtalk-py"
-version = "1.1.0"
-description = "a simple but powerful pythonic library for making bots for the TeamTalk5 Conferencing System"
-authors = ["JessicaTegner <jessica.tegner@outlook.com>"]
-license = "MIT"
-readme = "README.md"
-homepage = "https://github.com/JessicaTegner/teamtalk.py/"
-repository = "https://github.com/JessicaTegner/teamtalk.py/"
-documentation = "https://teamtalkpy.readthedocs.io/en/latest/"
-keywords = ["teamtalk", "teamtalk5", "teamtalk sdk", "conferencing"]
-
-classifiers = [
-    "Development Status :: 4 - Beta",
-    "Framework :: AsyncIO",
-    "Natural Language :: English",
-    "Operating System :: OS Independent",
-    "Topic :: Internet",
-    "Topic :: Software Development :: Libraries",
-    "Topic :: Software Development :: Libraries :: Python Modules",
-    "Topic :: Utilities",
-    "Typing :: Typed",
-]
-
-packages = [{include = "teamtalk"}]
-
-[tool.poetry.dependencies]
-python = "^3.8"
-typing-extensions = "^4.5"
-requests = "^2.28"
-beautifulsoup4 = "^4.11"
-patool = "^1.12"
-pywave = "^0.5"
-
-
-[tool.poetry.group.dev.dependencies]
-pre-commit = "^3.1"
-
-[tool.poetry.group.docs]
-optional = true
-
-[tool.poetry.group.docs.dependencies]
-sphinx = "^6.1"
-sphinxcontrib-trio = "^1.1"
-sphinxcontrib-napoleon = "^0.7"
-sphinx-sitemap = "^2.5.0"
-
-[tool.black]
-line-length = 125
-skip-string-normalization = true
-
-[tool.flake8]
-ignore = ["E203", "E731", "W503", "D401", "DAR402", "DAR103"]
-exclude = ['docs/*', 'tests/*', 'teamtalk/tools/*', '__pycache__', 'teamtalk/implementation/*', 'teamtalk/__init__.py', 'teamtalk/implementation/__init__.py', 'example.py']
-max-line-length = 125
-count = true
-statistics = true
-max-complexity = 20
-
-[tool.poetry.urls]
-"Issue Tracker" = "https://github.com/JessicaTegner/teamtalk.py/issues/"
-
-
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+[tool.poetry]
+name = "teamtalk-py"
+version = "1.1.1"
+description = "a simple but powerful pythonic library for making bots for the TeamTalk5 Conferencing System"
+authors = ["JessicaTegner <jessica.tegner@outlook.com>"]
+license = "MIT"
+readme = "README.md"
+homepage = "https://github.com/JessicaTegner/teamtalk.py/"
+repository = "https://github.com/JessicaTegner/teamtalk.py/"
+documentation = "https://teamtalkpy.readthedocs.io/en/latest/"
+keywords = ["teamtalk", "teamtalk5", "teamtalk sdk", "conferencing"]
+
+classifiers = [
+    "Development Status :: 4 - Beta",
+    "Framework :: AsyncIO",
+    "Natural Language :: English",
+    "Operating System :: OS Independent",
+    "Topic :: Internet",
+    "Topic :: Software Development :: Libraries",
+    "Topic :: Software Development :: Libraries :: Python Modules",
+    "Topic :: Utilities",
+    "Typing :: Typed",
+]
+
+packages = [{include = "teamtalk"}]
+
+[tool.poetry.dependencies]
+python = "^3.8"
+typing-extensions = "^4.5"
+requests = "^2.28"
+beautifulsoup4 = "^4.11"
+patool = "^1.12"
+pywave = "^0.5"
+
+
+[tool.poetry.group.dev.dependencies]
+pre-commit = "^3.1"
+
+[tool.poetry.group.docs]
+optional = true
+
+[tool.poetry.group.docs.dependencies]
+sphinx = "^6.1"
+sphinxcontrib-trio = "^1.1"
+sphinxcontrib-napoleon = "^0.7"
+sphinx-sitemap = "^2.5.0"
+
+[tool.black]
+line-length = 125
+skip-string-normalization = true
+
+[tool.flake8]
+ignore = ["E203", "E731", "W503", "D401", "DAR402", "DAR103"]
+exclude = ['docs/*', 'tests/*', 'teamtalk/tools/*', '__pycache__', 'teamtalk/implementation/*', 'teamtalk/__init__.py', 'teamtalk/implementation/__init__.py', 'example.py']
+max-line-length = 125
+count = true
+statistics = true
+max-complexity = 20
+
+[tool.poetry.urls]
+"Issue Tracker" = "https://github.com/JessicaTegner/teamtalk.py/issues/"
+
+
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `teamtalk_py-1.1.0/teamtalk/__init__.py` & `teamtalk_py-1.1.1/teamtalk/__init__.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-# if the implementation can't be found. Try to download it
-# from the internet and install it.
-
-# first add our to be implmentation/TeamTalk_DLL to the path
-import os
-import sys
-
-from ctypes import *
-
-# if we are on linux we do a little hack for the LD_LIBRARY_PATH
-try:
-    if sys.platform.startswith("linux"):
-        # get the full path to the implementation/TeamTalk_DLL folder
-        libpath = os.path.join(os.path.dirname(__file__), "implementation", "TeamTalk_DLL", "libTeamTalk5.so")
-        dll = cdll.LoadLibrary(libpath)
-    from .implementation.TeamTalkPy import TeamTalk5 as sdk
-except:
-    from .download_sdk import download_sdk
-
-    download_sdk()
-    if sys.platform.startswith("linux"):
-        # get the full path to the implementation/TeamTalk_DLL folder
-        libpath = os.path.join(os.path.dirname(__file__), "implementation", "TeamTalk_DLL", "libTeamTalk5.so")
-        dll = cdll.LoadLibrary(libpath)
-    from .implementation.TeamTalkPy import TeamTalk5 as sdk
-
-from .bot import TeamTalkBot
-from .channel import Channel
-from .enums import TeamTalkServerInfo, UserStatusMode, UserType
-from .instance import TeamTalkInstance
-from .message import BroadcastMessage, ChannelMessage, CustomMessage, DirectMessage
-from .permission import Permission
-from .streamer import Streamer
+# if the implementation can't be found. Try to download it
+# from the internet and install it.
+
+# first add our to be implmentation/TeamTalk_DLL to the path
+import os
+import sys
+
+from ctypes import *
+
+# if we are on linux we do a little hack for the LD_LIBRARY_PATH
+try:
+    if sys.platform.startswith("linux"):
+        # get the full path to the implementation/TeamTalk_DLL folder
+        libpath = os.path.join(os.path.dirname(__file__), "implementation", "TeamTalk_DLL", "libTeamTalk5.so")
+        dll = cdll.LoadLibrary(libpath)
+    from .implementation.TeamTalkPy import TeamTalk5 as sdk
+except:
+    from .download_sdk import download_sdk
+
+    download_sdk()
+    if sys.platform.startswith("linux"):
+        # get the full path to the implementation/TeamTalk_DLL folder
+        libpath = os.path.join(os.path.dirname(__file__), "implementation", "TeamTalk_DLL", "libTeamTalk5.so")
+        dll = cdll.LoadLibrary(libpath)
+    from .implementation.TeamTalkPy import TeamTalk5 as sdk
+
+from .bot import TeamTalkBot
+from .channel import Channel
+from .enums import TeamTalkServerInfo, UserStatusMode, UserType
+from .instance import TeamTalkInstance
+from .message import BroadcastMessage, ChannelMessage, CustomMessage, DirectMessage
+from .permission import Permission
+from .streamer import Streamer
```

### Comparing `teamtalk_py-1.1.0/teamtalk/_utils.py` & `teamtalk_py-1.1.1/teamtalk/_utils.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,146 +1,146 @@
-import time
-import threading
-
-from .implementation.TeamTalkPy import TeamTalk5 as sdk
-
-timestamp = lambda: int(round(time.time() * 1000))
-DEF_WAIT = 1500
-
-
-def _waitForEvent(ttclient, event, timeout=DEF_WAIT):
-    msg = ttclient.getMessage(timeout)
-    end = timestamp() + timeout
-    while msg.nClientEvent != event:
-        if timestamp() >= end:
-            return False, sdk.TTMessage()
-        msg = ttclient.getMessage(timeout)
-
-    return True, msg
-
-
-def _waitForCmdSuccess(ttclient, cmdid, timeout):
-    result = True
-    while result:
-        result, msg = _waitForEvent(ttclient, sdk.ClientEvent.CLIENTEVENT_CMD_SUCCESS, timeout)
-        if result and msg.nSource == cmdid:
-            return result, msg
-
-    return False, sdk.TTMessage()
-
-
-def _waitForCmd(ttclient, cmdid, timeout):
-    end = timestamp() + timeout
-    while True:
-        msg = ttclient.getMessage()
-        if msg.nClientEvent == sdk.ClientEvent.CLIENTEVENT_CMD_ERROR:
-            if msg.nSource == cmdid:
-                return False, msg.clienterrormsg
-        elif msg.nClientEvent == sdk.ClientEvent.CLIENTEVENT_CMD_SUCCESS:
-            if msg.nSource == cmdid:
-                return True, msg
-        if timestamp() >= end:
-            return False, sdk.TTMessage()
-
-
-def _getAbsTimeDiff(t1, t2):
-    t1 = int(round(t1 * 1000))
-    t2 = int(round(t2 * 1000))
-    return abs(t1 - t2)
-
-
-def _get_tt_obj_attribute(obj, attr):
-    name = ""
-    for name_part in attr.split("_"):
-        # if the name_part is "id" or "ID" then we want to keep it as "ID"
-        if name_part.lower() == "id":
-            name += "ID"
-        else:
-            # otherwise we want to capitalize the first letter
-            name += name_part.capitalize()
-    # first try to prefix with "n" and then get obj.name
-    try:
-        return getattr(obj, f"n{name}")
-    except AttributeError:
-        pass
-    # if that fails, try to prefix name with "sz" and then get obj.name
-    try:
-        return getattr(obj, f"sz{name}")
-    except AttributeError:
-        pass
-    # if that fails, try to prefix name with "b" and then get obj.name
-    try:
-        return getattr(obj, f"b{name}")
-    except AttributeError:
-        pass
-    # if that fails, try to prefix name with "u" and then get obj.name
-    try:
-        return getattr(obj, f"u{name}")
-    except AttributeError:
-        pass
-    # if that fails, try to lowercase the first letter name and then get obj.name
-    try:
-        return getattr(obj, f"{name[0].lower()}{name[1:]}")
-    except AttributeError:
-        pass
-    # if we are still here we failed to get the attribute
-    raise AttributeError(f"Could not find attribute {name} in {obj}")
-
-
-def _set_tt_obj_attribute(obj, attr, value):
-    name = ""
-    for name_part in attr.split("_"):
-        # if the name_part is "id" or "ID" then we want to keep it as "ID"
-        if name_part.lower() == "id":
-            name += "ID"
-        else:
-            # otherwise we want to capitalize the first letter
-            name += name_part.capitalize()
-    # first try to prefix with "n" and then set obj.name to value
-    try:
-        setattr(obj, f"n{name}", value)
-        return
-    except AttributeError:
-        pass
-    # if that fails, try to prefix name with "sz" and then set obj.name to value
-    try:
-        setattr(obj, f"sz{name}", value)
-        return
-    except AttributeError:
-        pass
-    # if that fails, try to prefix name with "b" and then set obj.name to value
-    try:
-        setattr(obj, f"b{name}", value)
-        return
-    except AttributeError:
-        pass
-    # if that fails, try to prefix name with "u" and then set obj.name to value
-    try:
-        setattr(obj, f"u{name}", value)
-        return
-    except AttributeError:
-        pass
-    # if that fails, try to lowercase the first letter name and then set obj.name to value
-    try:
-        setattr(obj, f"{name[0].lower()}{name[1:]}", value)
-        return
-    except AttributeError:
-        pass
-    # if we are still here we failed to get the attribute
-    raise AttributeError(f"Could not set attribute {name} in {obj}")
-
-
-def _do_after(delay, func):
-    def _do_after_thread(delay, func):
-        initial_time = time.time()
-        while _getAbsTimeDiff(initial_time, time.time()) < (delay * 1000):
-            time.sleep(0.001)
-        func()
-
-    threading.Thread(
-        daemon=True,
-        target=_do_after_thread,
-        args=(
-            delay,
-            func,
-        ),
-    ).start()
+import time
+import threading
+
+from .implementation.TeamTalkPy import TeamTalk5 as sdk
+
+timestamp = lambda: int(round(time.time() * 1000))
+DEF_WAIT = 1500
+
+
+def _waitForEvent(ttclient, event, timeout=DEF_WAIT):
+    msg = ttclient.getMessage(timeout)
+    end = timestamp() + timeout
+    while msg.nClientEvent != event:
+        if timestamp() >= end:
+            return False, sdk.TTMessage()
+        msg = ttclient.getMessage(timeout)
+
+    return True, msg
+
+
+def _waitForCmdSuccess(ttclient, cmdid, timeout):
+    result = True
+    while result:
+        result, msg = _waitForEvent(ttclient, sdk.ClientEvent.CLIENTEVENT_CMD_SUCCESS, timeout)
+        if result and msg.nSource == cmdid:
+            return result, msg
+
+    return False, sdk.TTMessage()
+
+
+def _waitForCmd(ttclient, cmdid, timeout):
+    end = timestamp() + timeout
+    while True:
+        msg = ttclient.getMessage()
+        if msg.nClientEvent == sdk.ClientEvent.CLIENTEVENT_CMD_ERROR:
+            if msg.nSource == cmdid:
+                return False, msg.clienterrormsg
+        elif msg.nClientEvent == sdk.ClientEvent.CLIENTEVENT_CMD_SUCCESS:
+            if msg.nSource == cmdid:
+                return True, msg
+        if timestamp() >= end:
+            return False, sdk.TTMessage()
+
+
+def _getAbsTimeDiff(t1, t2):
+    t1 = int(round(t1 * 1000))
+    t2 = int(round(t2 * 1000))
+    return abs(t1 - t2)
+
+
+def _get_tt_obj_attribute(obj, attr):
+    name = ""
+    for name_part in attr.split("_"):
+        # if the name_part is "id" or "ID" then we want to keep it as "ID"
+        if name_part.lower() == "id":
+            name += "ID"
+        else:
+            # otherwise we want to capitalize the first letter
+            name += name_part.capitalize()
+    # first try to prefix with "n" and then get obj.name
+    try:
+        return getattr(obj, f"n{name}")
+    except AttributeError:
+        pass
+    # if that fails, try to prefix name with "sz" and then get obj.name
+    try:
+        return getattr(obj, f"sz{name}")
+    except AttributeError:
+        pass
+    # if that fails, try to prefix name with "b" and then get obj.name
+    try:
+        return getattr(obj, f"b{name}")
+    except AttributeError:
+        pass
+    # if that fails, try to prefix name with "u" and then get obj.name
+    try:
+        return getattr(obj, f"u{name}")
+    except AttributeError:
+        pass
+    # if that fails, try to lowercase the first letter name and then get obj.name
+    try:
+        return getattr(obj, f"{name[0].lower()}{name[1:]}")
+    except AttributeError:
+        pass
+    # if we are still here we failed to get the attribute
+    raise AttributeError(f"Could not find attribute {name} in {obj}")
+
+
+def _set_tt_obj_attribute(obj, attr, value):
+    name = ""
+    for name_part in attr.split("_"):
+        # if the name_part is "id" or "ID" then we want to keep it as "ID"
+        if name_part.lower() == "id":
+            name += "ID"
+        else:
+            # otherwise we want to capitalize the first letter
+            name += name_part.capitalize()
+    # first try to prefix with "n" and then set obj.name to value
+    try:
+        setattr(obj, f"n{name}", value)
+        return
+    except AttributeError:
+        pass
+    # if that fails, try to prefix name with "sz" and then set obj.name to value
+    try:
+        setattr(obj, f"sz{name}", value)
+        return
+    except AttributeError:
+        pass
+    # if that fails, try to prefix name with "b" and then set obj.name to value
+    try:
+        setattr(obj, f"b{name}", value)
+        return
+    except AttributeError:
+        pass
+    # if that fails, try to prefix name with "u" and then set obj.name to value
+    try:
+        setattr(obj, f"u{name}", value)
+        return
+    except AttributeError:
+        pass
+    # if that fails, try to lowercase the first letter name and then set obj.name to value
+    try:
+        setattr(obj, f"{name[0].lower()}{name[1:]}", value)
+        return
+    except AttributeError:
+        pass
+    # if we are still here we failed to get the attribute
+    raise AttributeError(f"Could not set attribute {name} in {obj}")
+
+
+def _do_after(delay, func):
+    def _do_after_thread(delay, func):
+        initial_time = time.time()
+        while _getAbsTimeDiff(initial_time, time.time()) < (delay * 1000):
+            time.sleep(0.001)
+        func()
+
+    threading.Thread(
+        daemon=True,
+        target=_do_after_thread,
+        args=(
+            delay,
+            func,
+        ),
+    ).start()
```

### Comparing `teamtalk_py-1.1.0/teamtalk/bot.py` & `teamtalk_py-1.1.1/teamtalk/bot.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,265 +1,265 @@
-"""A module that contains the TeamTalkBot class.
-
-The TeamTalkBot class is the main class of the library.
-It's used to create a bot,connect to any amount of TeamTalk servers and dispatch events.
-"""
-
-import asyncio
-import logging
-from typing import Any, Callable, Coroutine, Dict, List, Optional, Tuple, Type, TypeVar, Union
-
-from typing_extensions import Self
-
-from .enums import TeamTalkServerInfo
-from .instance import TeamTalkInstance
-
-T = TypeVar("T")
-Coro = Coroutine[Any, Any, T]
-CoroT = TypeVar("CoroT", bound=Callable[..., Coro[Any]])
-
-
-class _LoopSentinel:
-    __slots__ = ()
-
-    def __getattr__(self, attr: str) -> None:
-        msg = "loop attribute cannot be accessed in non-async contexts. "
-        raise AttributeError(msg)
-
-
-_loop: Any = _LoopSentinel()
-_log = logging.getLogger(__name__)
-
-
-class TeamTalkBot:
-    """A class that represents a TeamTalk bot."""
-
-    def __init__(self, client_name: Optional[str] = "Teamtalk.py") -> None:
-        """Initialize a TeamTalkBot object.
-
-        Args:
-            client_name (Optional[str]): The name of the client. Defaults to "Teamtalk.py".
-        """
-        self.client_name = client_name
-        self.loop: asyncio.AbstractEventLoop = _loop
-        # hold a list of TeamTalk instances
-        self.teamtalks: List[TeamTalkInstance] = []
-        self._listeners: Dict[str, List[Tuple[asyncio.Future, Callable[..., bool]]]] = {}
-
-    async def add_server(self, server: Union[TeamTalkServerInfo, dict]) -> None:
-        """Add a server to the bot.
-
-        Args:
-            server: A Union[TeamTalkServerInfo, dict] object representing the server to add.
-                If a dictionary is provided, it will be converted to a TeamTalkServerInfo object.
-        """
-        if isinstance(server, dict):
-            server = TeamTalkServerInfo.from_dict(server)
-        _log.debug(f"Adding server: {self, server}")
-        tt = TeamTalkInstance(self, server)
-        # connect
-        tt.connect()
-        # login
-        tt.login()
-        self.teamtalks.append(tt)
-
-    def run(self):
-        """A blocking call that connects to all added servers and handles all events."""
-
-        async def runner():
-            async with self:
-                await self._start()
-
-        # setup logging to log debug messages
-        # and log everyhting to console
-        logging.basicConfig(level=logging.DEBUG)
-
-        try:
-            # set our loop the asyncio event loop
-            asyncio.run(runner())
-        except KeyboardInterrupt:
-            # nothing to do here
-            # `asyncio.run` handles the loop cleanup
-            # and `self.start` closes all sockets and the HTTPClient instance.
-            return
-
-    async def _async_setup_hook(self) -> None:
-        # Called whenever the client needs to initialise asyncio objects with a running loop
-        loop = asyncio.get_running_loop()
-        self.loop = loop
-
-    async def __aenter__(self) -> Self:
-        """A context manager that is used to get the correct event loop.
-
-        Returns:
-            Self: The TeamTalkBot object.
-        """
-        await self._async_setup_hook()
-        return self
-
-    async def __aexit__(
-        self,
-        exc_type: Optional[Type[BaseException]],
-        exc_value: Optional[BaseException],
-        traceback,
-    ) -> None:
-        """When we exit the program, try to disconnect from all servers.
-
-        Args:
-            exc_type (Optional[Type[BaseException]]): The exception type.
-            exc_value (Optional[BaseException]): The exception value.
-            traceback: The traceback.
-        """
-        for teamtalk in self.teamtalks:
-            teamtalk.disconnect()
-            teamtalk.closeTeamTalk()
-
-    def event(self, coro: CoroT, /) -> CoroT:
-        """A decorator that registers an event to listen to.
-
-        The events must be a :ref:`coroutine <coroutine>`, if not, :exc:`TypeError` is raised.
-
-        Example
-        ---------
-
-        .. code-block:: python3
-
-            @client.event
-            async def on_ready():
-                print('Ready!')
-
-
-        See the :doc:`event Reference </events>` for more information and a list of all events.
-
-
-        Args:
-            coro (CoroT): The coroutine to register.
-
-        Returns:
-            CoroT: The coroutine that was registered.
-
-        Raises:
-            TypeError: The coroutine is not a coroutine function.
-        """
-        _log.debug("Registering event %s", coro.__name__)
-
-        if not asyncio.iscoroutinefunction(coro):
-            raise TypeError("event registered must be a coroutine function")
-
-        setattr(self, coro.__name__, coro)
-        _log.debug("Registered event %s", coro.__name__)
-        return coro
-
-    async def _run_event(
-        self,
-        coro: Callable[..., Coroutine[Any, Any, Any]],
-        event_name: str,
-        *args: Any,
-        **kwargs: Any,
-    ) -> None:
-        try:
-            _log.debug("Running event %s", event_name)
-            await coro(*args, **kwargs)
-        except asyncio.CancelledError:
-            _log.debug("Event %s was cancelled", event_name)
-        except Exception:
-            try:
-                await self.on_error(event_name, *args, **kwargs)
-            except asyncio.CancelledError:
-                pass
-
-    def _schedule_event(
-        self,
-        coro: Callable[..., Coroutine[Any, Any, Any]],
-        event_name: str,
-        *args: Any,
-        **kwargs: Any,
-    ) -> asyncio.Task:
-        # print all the events to log
-        wrapped = self._run_event(coro, event_name, *args, **kwargs)
-        # Schedules the task
-        return self.loop.create_task(wrapped, name=f"teamtalk.py: {event_name}")
-
-    async def on_error(self, event_method: str, /, *args: Any, **kwargs: Any) -> None:
-        """|coro| .
-
-        The default error handler provided by the client.
-
-        By default this logs to the library logger however it could be
-        overridden to have a different implementation.
-        The traceback from this exception is logged to the logging module.
-
-        Args:
-            event_method (str): The event method that errored.
-            *args (Any): The arguments to the event.
-            **kwargs (Any): The keyword arguments to the event.
-        """
-        _log.exception("Ignoring exception in %s", event_method)
-
-    def dispatch(self, event: str, /, *args: Any, **kwargs: Any) -> None:
-        """Dispatch an event to all listeners. This is called internally.
-
-        Args:
-            event (str): The name of the event to dispatch.
-            *args (Any): The arguments to the event.
-            **kwargs (Any): The keyword arguments to the event.
-        """
-        _log.debug("Dispatching event %s", event)
-        method = "on_" + event
-
-        listeners = self._listeners.get(event)
-        if listeners:
-            removed = []
-            for i, (future, condition) in enumerate(listeners):
-                if future.cancelled():
-                    removed.append(i)
-                    continue
-
-                try:
-                    result = condition(*args)
-                except Exception as exc:
-                    future.set_exception(exc)
-                    removed.append(i)
-                else:
-                    if result:
-                        if len(args) == 0:
-                            future.set_result(None)
-                        elif len(args) == 1:
-                            future.set_result(args[0])
-                        else:
-                            future.set_result(args)
-                        removed.append(i)
-
-            if len(removed) == len(listeners):
-                self._listeners.pop(event)
-            else:
-                for idx in reversed(removed):
-                    del listeners[idx]
-
-        try:
-            coro = getattr(self, method)
-        except AttributeError:
-            pass
-        else:
-            self._schedule_event(coro, method, *args, **kwargs)
-
-    async def _start(self):
-        self.dispatch("ready")
-        # make a while loop and allow it to run forever
-        try:
-            while True:
-                # loop through the teamtalks and check  for events
-                for teamtalk in self.teamtalks:
-                    await teamtalk._process_events()
-                await asyncio.sleep(0.001)
-        except KeyboardInterrupt:
-            # try to disconnect everything cleanly
-            for teamtalk in self.teamtalks:
-                # disconnect from the server
-                teamtalk.doLogout()
-                self.dispatch("my_logout", teamtalk.server)
-                teamtalk.disconnect()
-                self.dispatch("my_disconnect", teamtalk.server)
-
-    async def _do_after_delay(self, delay, func, *args, **kwargs):
-        await asyncio.sleep(delay)
-        print("WORKS")
+"""A module that contains the TeamTalkBot class.
+
+The TeamTalkBot class is the main class of the library.
+It's used to create a bot,connect to any amount of TeamTalk servers and dispatch events.
+"""
+
+import asyncio
+import logging
+from typing import Any, Callable, Coroutine, Dict, List, Optional, Tuple, Type, TypeVar, Union
+
+from typing_extensions import Self
+
+from .enums import TeamTalkServerInfo
+from .instance import TeamTalkInstance
+
+T = TypeVar("T")
+Coro = Coroutine[Any, Any, T]
+CoroT = TypeVar("CoroT", bound=Callable[..., Coro[Any]])
+
+
+class _LoopSentinel:
+    __slots__ = ()
+
+    def __getattr__(self, attr: str) -> None:
+        msg = "loop attribute cannot be accessed in non-async contexts. "
+        raise AttributeError(msg)
+
+
+_loop: Any = _LoopSentinel()
+_log = logging.getLogger(__name__)
+
+
+class TeamTalkBot:
+    """A class that represents a TeamTalk bot."""
+
+    def __init__(self, client_name: Optional[str] = "Teamtalk.py") -> None:
+        """Initialize a TeamTalkBot object.
+
+        Args:
+            client_name (Optional[str]): The name of the client. Defaults to "Teamtalk.py".
+        """
+        self.client_name = client_name
+        self.loop: asyncio.AbstractEventLoop = _loop
+        # hold a list of TeamTalk instances
+        self.teamtalks: List[TeamTalkInstance] = []
+        self._listeners: Dict[str, List[Tuple[asyncio.Future, Callable[..., bool]]]] = {}
+
+    async def add_server(self, server: Union[TeamTalkServerInfo, dict]) -> None:
+        """Add a server to the bot.
+
+        Args:
+            server: A Union[TeamTalkServerInfo, dict] object representing the server to add.
+                If a dictionary is provided, it will be converted to a TeamTalkServerInfo object.
+        """
+        if isinstance(server, dict):
+            server = TeamTalkServerInfo.from_dict(server)
+        _log.debug(f"Adding server: {self, server}")
+        tt = TeamTalkInstance(self, server)
+        # connect
+        tt.connect()
+        # login
+        tt.login()
+        self.teamtalks.append(tt)
+
+    def run(self):
+        """A blocking call that connects to all added servers and handles all events."""
+
+        async def runner():
+            async with self:
+                await self._start()
+
+        # setup logging to log debug messages
+        # and log everyhting to console
+        logging.basicConfig(level=logging.DEBUG)
+
+        try:
+            # set our loop the asyncio event loop
+            asyncio.run(runner())
+        except KeyboardInterrupt:
+            # nothing to do here
+            # `asyncio.run` handles the loop cleanup
+            # and `self.start` closes all sockets and the HTTPClient instance.
+            return
+
+    async def _async_setup_hook(self) -> None:
+        # Called whenever the client needs to initialise asyncio objects with a running loop
+        loop = asyncio.get_running_loop()
+        self.loop = loop
+
+    async def __aenter__(self) -> Self:
+        """A context manager that is used to get the correct event loop.
+
+        Returns:
+            Self: The TeamTalkBot object.
+        """
+        await self._async_setup_hook()
+        return self
+
+    async def __aexit__(
+        self,
+        exc_type: Optional[Type[BaseException]],
+        exc_value: Optional[BaseException],
+        traceback,
+    ) -> None:
+        """When we exit the program, try to disconnect from all servers.
+
+        Args:
+            exc_type (Optional[Type[BaseException]]): The exception type.
+            exc_value (Optional[BaseException]): The exception value.
+            traceback: The traceback.
+        """
+        for teamtalk in self.teamtalks:
+            teamtalk.disconnect()
+            teamtalk.closeTeamTalk()
+
+    def event(self, coro: CoroT, /) -> CoroT:
+        """A decorator that registers an event to listen to.
+
+        The events must be a :ref:`coroutine <coroutine>`, if not, :exc:`TypeError` is raised.
+
+        Example
+        ---------
+
+        .. code-block:: python3
+
+            @client.event
+            async def on_ready():
+                print('Ready!')
+
+
+        See the :doc:`event Reference </events>` for more information and a list of all events.
+
+
+        Args:
+            coro (CoroT): The coroutine to register.
+
+        Returns:
+            CoroT: The coroutine that was registered.
+
+        Raises:
+            TypeError: The coroutine is not a coroutine function.
+        """
+        _log.debug("Registering event %s", coro.__name__)
+
+        if not asyncio.iscoroutinefunction(coro):
+            raise TypeError("event registered must be a coroutine function")
+
+        setattr(self, coro.__name__, coro)
+        _log.debug("Registered event %s", coro.__name__)
+        return coro
+
+    async def _run_event(
+        self,
+        coro: Callable[..., Coroutine[Any, Any, Any]],
+        event_name: str,
+        *args: Any,
+        **kwargs: Any,
+    ) -> None:
+        try:
+            _log.debug("Running event %s", event_name)
+            await coro(*args, **kwargs)
+        except asyncio.CancelledError:
+            _log.debug("Event %s was cancelled", event_name)
+        except Exception:
+            try:
+                await self.on_error(event_name, *args, **kwargs)
+            except asyncio.CancelledError:
+                pass
+
+    def _schedule_event(
+        self,
+        coro: Callable[..., Coroutine[Any, Any, Any]],
+        event_name: str,
+        *args: Any,
+        **kwargs: Any,
+    ) -> asyncio.Task:
+        # print all the events to log
+        wrapped = self._run_event(coro, event_name, *args, **kwargs)
+        # Schedules the task
+        return self.loop.create_task(wrapped, name=f"teamtalk.py: {event_name}")
+
+    async def on_error(self, event_method: str, /, *args: Any, **kwargs: Any) -> None:
+        """|coro| .
+
+        The default error handler provided by the client.
+
+        By default this logs to the library logger however it could be
+        overridden to have a different implementation.
+        The traceback from this exception is logged to the logging module.
+
+        Args:
+            event_method (str): The event method that errored.
+            *args (Any): The arguments to the event.
+            **kwargs (Any): The keyword arguments to the event.
+        """
+        _log.exception("Ignoring exception in %s", event_method)
+
+    def dispatch(self, event: str, /, *args: Any, **kwargs: Any) -> None:
+        """Dispatch an event to all listeners. This is called internally.
+
+        Args:
+            event (str): The name of the event to dispatch.
+            *args (Any): The arguments to the event.
+            **kwargs (Any): The keyword arguments to the event.
+        """
+        _log.debug("Dispatching event %s", event)
+        method = "on_" + event
+
+        listeners = self._listeners.get(event)
+        if listeners:
+            removed = []
+            for i, (future, condition) in enumerate(listeners):
+                if future.cancelled():
+                    removed.append(i)
+                    continue
+
+                try:
+                    result = condition(*args)
+                except Exception as exc:
+                    future.set_exception(exc)
+                    removed.append(i)
+                else:
+                    if result:
+                        if len(args) == 0:
+                            future.set_result(None)
+                        elif len(args) == 1:
+                            future.set_result(args[0])
+                        else:
+                            future.set_result(args)
+                        removed.append(i)
+
+            if len(removed) == len(listeners):
+                self._listeners.pop(event)
+            else:
+                for idx in reversed(removed):
+                    del listeners[idx]
+
+        try:
+            coro = getattr(self, method)
+        except AttributeError:
+            pass
+        else:
+            self._schedule_event(coro, method, *args, **kwargs)
+
+    async def _start(self):
+        self.dispatch("ready")
+        # make a while loop and allow it to run forever
+        try:
+            while True:
+                # loop through the teamtalks and check  for events
+                for teamtalk in self.teamtalks:
+                    await teamtalk._process_events()
+                await asyncio.sleep(0.001)
+        except KeyboardInterrupt:
+            # try to disconnect everything cleanly
+            for teamtalk in self.teamtalks:
+                # disconnect from the server
+                teamtalk.doLogout()
+                self.dispatch("my_logout", teamtalk.server)
+                teamtalk.disconnect()
+                self.dispatch("my_disconnect", teamtalk.server)
+
+    async def _do_after_delay(self, delay, func, *args, **kwargs):
+        await asyncio.sleep(delay)
+        print("WORKS")
```

### Comparing `teamtalk_py-1.1.0/teamtalk/enums.py` & `teamtalk_py-1.1.1/teamtalk/enums.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,129 +1,129 @@
-"""TeamTalk enums and constants."""
-
-from typing_extensions import Self
-
-
-class TeamTalkServerInfo:
-    """Holds the required information to connect and login to a TeamTalk server."""
-
-    def __init__(
-        self,
-        host: str,
-        tcp_port: int,
-        udp_port: int,
-        username: str,
-        password: str = "",
-        encrypted: bool = False,
-        nickname: str = "",
-        join_channel_id: int = -1,
-        join_channel_password: str = "",
-    ) -> None:
-        """Initialize a TeamTalkServerInfo object.
-
-        Args:
-            host (str): The host of the TeamTalk server.
-            tcp_port (int): The TCP port of the TeamTalk server.
-            udp_port (int): The UDP port of the TeamTalk server.
-            username (str): The username to login with.
-            password (str): The password to login with. Defaults to "" (no password).
-            encrypted (bool): Whether or not to use encryption. Defaults to False.
-            nickname (str): The nickname to use. Defaults to "teamtalk.py Bot".
-            join_channel_id (int): The channel ID to join. Defaults to -1 (don't join a channel on login). Set to 0 to join the root channel, or a positive integer to join a specific channel. # noqa: E501
-            join_channel_password (str): The password to join the channel with. Defaults to "" (no password).
-        """
-        self.host = host
-        self.tcp_port = tcp_port
-        self.udp_port = udp_port
-        self.username = username
-        self.password = password
-        self.encrypted = encrypted
-        self.nickname = nickname if nickname else username
-        self.join_channel_id = join_channel_id
-        self.join_channel_password = join_channel_password
-
-    @classmethod
-    def from_dict(cls, data: dict) -> Self:
-        """Construct a TeamTalkServerInfo object from a dictionary.
-
-        Args:
-            data (dict): The dictionary to construct the object from.
-
-        Returns:
-            Self: The constructed object.
-        """
-        return cls(**data)
-
-    # convert this object to a dictionary
-    def to_dict(self) -> dict:
-        """Convert this object to a dictionary.
-
-        Returns:
-            dict: The dictionary representation of this object.
-        """
-        return {
-            "host": self.host,
-            "tcp_port": self.tcp_port,
-            "udp_port": self.udp_port,
-            "username": self.username,
-            "password": self.password,
-            "encrypted": self.encrypted,
-            "nickname": self.nickname if self.nickname else "",
-            "join_channel_id": self.join_channel_id,
-            "join_channel_password": self.join_channel_password,
-        }
-
-    # compare this object to another object
-    def __eq__(self, other: object) -> bool:
-        """Compare this object to another object.
-
-        Args:
-            other: The object to compare to.
-
-        Returns:
-            bool: Whether or not the objects are equal.
-        """
-        if not isinstance(other, TeamTalkServerInfo):
-            return False
-        return (
-            self.host == other.host
-            and self.tcp_port == other.tcp_port
-            and self.udp_port == other.udp_port
-            and self.username == other.username
-            and self.password == other.password
-            and self.encrypted == other.encrypted
-        )
-
-    # compare this object to another object
-    def __ne__(self, other: object) -> bool:
-        """Compare this object to another object.
-
-        Args:
-            other: The object to compare to.
-
-        Returns:
-            bool: Whether or not the objects are not equal.
-        """
-        return not self.__eq__(other)
-
-
-class UserStatusMode:
-    """The status mode of a user. This is used in the teamtalk.TeamTalkInstance.change_status call."""
-
-    ONLINE = 0
-    """The user is online."""
-
-    AWAY = 1
-    """The user is away."""
-
-    QUESTION = 2
-    """The user has a question"""
-
-
-class UserType:
-    """The type of a user account."""
-
-    DEFAULT = 0x1
-    """The default user type. This only has the permissions set, and no other permissions."""
-
-    ADMIN = 0x02
-    """The admin user type. This has all permissions."""
+"""TeamTalk enums and constants."""
+
+from typing_extensions import Self
+
+
+class TeamTalkServerInfo:
+    """Holds the required information to connect and login to a TeamTalk server."""
+
+    def __init__(
+        self,
+        host: str,
+        tcp_port: int,
+        udp_port: int,
+        username: str,
+        password: str = "",
+        encrypted: bool = False,
+        nickname: str = "",
+        join_channel_id: int = -1,
+        join_channel_password: str = "",
+    ) -> None:
+        """Initialize a TeamTalkServerInfo object.
+
+        Args:
+            host (str): The host of the TeamTalk server.
+            tcp_port (int): The TCP port of the TeamTalk server.
+            udp_port (int): The UDP port of the TeamTalk server.
+            username (str): The username to login with.
+            password (str): The password to login with. Defaults to "" (no password).
+            encrypted (bool): Whether or not to use encryption. Defaults to False.
+            nickname (str): The nickname to use. Defaults to "teamtalk.py Bot".
+            join_channel_id (int): The channel ID to join. Defaults to -1 (don't join a channel on login). Set to 0 to join the root channel, or a positive integer to join a specific channel. # noqa: E501
+            join_channel_password (str): The password to join the channel with. Defaults to "" (no password).
+        """
+        self.host = host
+        self.tcp_port = tcp_port
+        self.udp_port = udp_port
+        self.username = username
+        self.password = password
+        self.encrypted = encrypted
+        self.nickname = nickname if nickname else username
+        self.join_channel_id = join_channel_id
+        self.join_channel_password = join_channel_password
+
+    @classmethod
+    def from_dict(cls, data: dict) -> Self:
+        """Construct a TeamTalkServerInfo object from a dictionary.
+
+        Args:
+            data (dict): The dictionary to construct the object from.
+
+        Returns:
+            Self: The constructed object.
+        """
+        return cls(**data)
+
+    # convert this object to a dictionary
+    def to_dict(self) -> dict:
+        """Convert this object to a dictionary.
+
+        Returns:
+            dict: The dictionary representation of this object.
+        """
+        return {
+            "host": self.host,
+            "tcp_port": self.tcp_port,
+            "udp_port": self.udp_port,
+            "username": self.username,
+            "password": self.password,
+            "encrypted": self.encrypted,
+            "nickname": self.nickname if self.nickname else "",
+            "join_channel_id": self.join_channel_id,
+            "join_channel_password": self.join_channel_password,
+        }
+
+    # compare this object to another object
+    def __eq__(self, other: object) -> bool:
+        """Compare this object to another object.
+
+        Args:
+            other: The object to compare to.
+
+        Returns:
+            bool: Whether or not the objects are equal.
+        """
+        if not isinstance(other, TeamTalkServerInfo):
+            return False
+        return (
+            self.host == other.host
+            and self.tcp_port == other.tcp_port
+            and self.udp_port == other.udp_port
+            and self.username == other.username
+            and self.password == other.password
+            and self.encrypted == other.encrypted
+        )
+
+    # compare this object to another object
+    def __ne__(self, other: object) -> bool:
+        """Compare this object to another object.
+
+        Args:
+            other: The object to compare to.
+
+        Returns:
+            bool: Whether or not the objects are not equal.
+        """
+        return not self.__eq__(other)
+
+
+class UserStatusMode:
+    """The status mode of a user. This is used in the teamtalk.TeamTalkInstance.change_status call."""
+
+    ONLINE = 0
+    """The user is online."""
+
+    AWAY = 1
+    """The user is away."""
+
+    QUESTION = 2
+    """The user has a question"""
+
+
+class UserType:
+    """The type of a user account."""
+
+    DEFAULT = 0x1
+    """The default user type. This only has the permissions set, and no other permissions."""
+
+    ADMIN = 0x02
+    """The admin user type. This has all permissions."""
```

### Comparing `teamtalk_py-1.1.0/teamtalk/exceptions.py` & `teamtalk_py-1.1.1/teamtalk/exceptions.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-"""teamtalk.py exceptions."""
-
-
-class TeamTalkException(Exception):
-    """Base exception class for teamtalk.py.
-
-    All other exceptions inherit from this class, which inherits from :exc:`Exception`.
-    """
-
-    def __init__(self, message: str) -> None:
-        """Initialise the exception.
-
-        Args:
-            message (str): The message to be displayed when the exception is raised.
-        """
-        super().__init__(message)
-
-
-class PermissionError(TeamTalkException):
-    """Exception raised when the bot does not have permission to perform an action."""
+"""teamtalk.py exceptions."""
+
+
+class TeamTalkException(Exception):
+    """Base exception class for teamtalk.py.
+
+    All other exceptions inherit from this class, which inherits from :exc:`Exception`.
+    """
+
+    def __init__(self, message: str) -> None:
+        """Initialise the exception.
+
+        Args:
+            message (str): The message to be displayed when the exception is raised.
+        """
+        super().__init__(message)
+
+
+class PermissionError(TeamTalkException):
+    """Exception raised when the bot does not have permission to perform an action."""
```

### Comparing `teamtalk_py-1.1.0/teamtalk/instance.py` & `teamtalk_py-1.1.1/teamtalk/instance.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,854 +1,854 @@
-"""This module contains the TeamTalkInstance class.
-
-The TeamTalkInstance class contains one instance of a connection to a TeamTalkServer.
-It is used to send and receive messages, join and leave channels, and perform other actions.
-In addition, it's also here that events are dispatched.
-"""
-
-import asyncio
-import os
-import logging
-import time
-import ctypes
-from typing import List, Union
-
-from ._utils import _getAbsTimeDiff, _waitForEvent, _waitForCmd, _do_after
-from .channel import Channel as TeamTalkChannel
-from .channel import ChannelType
-from .enums import TeamTalkServerInfo, UserStatusMode, UserType
-from .exceptions import PermissionError
-from .implementation.TeamTalkPy import TeamTalk5 as sdk
-from .message import BroadcastMessage, ChannelMessage, CustomMessage, DirectMessage
-from .permission import Permission
-from .server import Server as TeamTalkServer
-from .tt_file import RemoteFile
-from .user import User as TeamTalkUser
-from .user_account import UserAccount as TeamTalkUserAccount
-from .user_account import BannedUserAccount as TeamTalkBannedUserAccount
-
-
-_log = logging.getLogger(__name__)
-
-
-class TeamTalkInstance(sdk.TeamTalk):
-    """Represents a TeamTalk5 instance."""
-
-    def __init__(self, bot, server_info: TeamTalkServerInfo) -> None:
-        """Initializes a teamtalk.TeamTalkInstance instance.
-
-        Args:
-            bot: The teamtalk.Bot instance.
-            server_info: The server info for the server we wish to connect to.
-        """
-        # put the super class in a variable so we can call it later
-        self.super = super()
-        # call the super class's __init__ method
-        self.super.__init__()
-        # set the bot
-        self.bot = bot
-        # set the server info
-        self.server_info = server_info
-        self.server = TeamTalkServer(self, server_info)
-        self.channel = lambda: self.get_channel(self.super.getMyChannelID())
-        self.connected = False
-        self.logged_in = False
-        self.init_time = time.time()
-        self.user_accounts = []
-        self.banned_users = []
-
-    def connect(self) -> bool:
-        """Connects to the server. This doesn't return until the connection is successful or fails.
-
-        Returns:
-            bool: True if the connection was successful, False otherwise.
-        """
-        if not self.super.connect(
-            sdk.ttstr(self.server_info.host),
-            self.server_info.tcp_port,
-            self.server_info.udp_port,
-            self.server_info.encrypted,
-        ):
-            return False
-        result, msg = _waitForEvent(self.super, sdk.ClientEvent.CLIENTEVENT_CON_SUCCESS)
-        if not result:
-            return False
-        self.bot.dispatch("my_connect", self.server)
-        self.connected = True
-        self.init_time = time.time()
-        return True
-
-    def login(self, join_channel_on_login: bool = True) -> bool:
-        """Logs in to the server. This doesn't return until the login is successful or fails.
-
-        Args:
-            join_channel_on_login: Whether to join the channel on login or not.
-
-        Returns:
-            bool: True if the login was successful, False otherwise.
-        """
-        self.super.doLogin(
-            sdk.ttstr(self.server_info.nickname),
-            sdk.ttstr(self.server_info.username),
-            sdk.ttstr(self.server_info.password),
-            sdk.ttstr(self.bot.client_name),
-        )
-        result, msg = _waitForEvent(self.super, sdk.ClientEvent.CLIENTEVENT_CMD_MYSELF_LOGGEDIN)
-        if not result:
-            return False
-        self.bot.dispatch("my_login", self.server)
-        self.logged_in = True
-        if join_channel_on_login:
-            channel_id = self.server_info.join_channel_id
-            if channel_id < 1:
-                channel_id = self.super.getRootChannelID()
-            self.join_channel_by_id(channel_id)
-        self.init_time = time.time()
-        return True
-
-    def logout(self):
-        """Logs out of the server."""
-        self.super.doLogout()
-        self.logged_in = False
-
-    def disconnect(self):
-        """Disconnects from the server."""
-        self.super.disconnect()
-        self.connected = False
-
-    def change_nickname(self, nickname: str):
-        """Changes the nickname of the bot.
-
-        Args:
-            nickname: The new nickname.
-        """
-        self.super.doChangeNickname(nickname)
-
-    def change_status(self, status_mode: UserStatusMode, status_message: str):
-        """Changes the status of the bot.
-
-        Args:
-            status_mode: The status mode.
-            status_message: The status message.
-        """
-        self.super.doChangeStatus(status_mode, status_message)
-
-    # permission stuff
-    def has_permission(self, permission: Permission) -> bool:
-        """Checks if the bot has a permission.
-
-        If the user is an admin, they have all permissions.
-
-        Args:
-            permission: The permission to check for.
-
-        Returns:
-            bool: True if the bot has the permission, False otherwise.
-        """
-        user = self.super.getMyUserAccount()
-        # first check if they are an admin
-        if user.uUserType == sdk.UserType.USERTYPE_ADMIN:
-            return True
-        user_rights = user.uUserRights
-        return (user_rights & permission) == permission
-
-    def is_admin(self) -> bool:
-        """Checks if the bot is an admin.
-
-        Returns:
-            bool: True if the bot is an admin, False otherwise.
-        """
-        return self.is_user_admin(self.super.getMyUserID())
-
-    def is_user_admin(self, user: Union[TeamTalkUser, int]) -> bool:
-        """Checks if a user is an admin.
-
-        Args:
-            user: The user to check.
-
-        Returns:
-            bool: True if the user is an admin, False otherwise.
-
-        Raises:
-            TypeError: If the user is not of type teamtalk.User or int.
-        """
-        if isinstance(user, int):
-            user = self.super.getUser(user)
-            return user.uUserType == sdk.UserType.USERTYPE_ADMIN
-        if isinstance(user, TeamTalkUser):
-            return user.user_type == sdk.UserType.USERTYPE_ADMIN
-        raise TypeError("User must be of type teamtalk.User or int")
-
-    def join_root_channel(self):
-        """Joins the root channel."""
-        self.join_channel_by_id(self.super.getRootChannelID())
-
-    def join_channel_by_id(self, id: int, password: str = ""):
-        """Joins a channel by its ID.
-
-        Args:
-            id: The ID of the channel to join.
-            password: The password of the channel to join.
-        """
-        self.super.doJoinChannelByID(id, sdk.ttstr(password))
-
-    def join_channel(self, channel: TeamTalkChannel):
-        """Joins a channel.
-
-        Args:
-            channel: The channel to join.
-        """
-        self.super.doJoinChannelByID(channel.id, sdk.ttstr(channel.password))
-
-    def leave_channel(self):
-        """Leaves the current channel."""
-        self.super.doLeaveChannel()
-
-    def get_channel(self, channel_id: int) -> TeamTalkChannel:
-        """Gets a channel by its ID.
-
-        Args:
-            channel_id: The ID of the channel to get.
-
-        Returns:
-            TeamTalkChannel: The channel.
-        """
-        return TeamTalkChannel(self, channel_id)
-
-    def get_path_from_channel(self, channel: Union[TeamTalkChannel, int]) -> str:
-        """Gets the path of a channel.
-
-        Args:
-            channel: The channel to get the path of.
-
-        Returns:
-            str: The path of the channel.
-
-        Raises:
-            TypeError: If the channel is not of type teamtalk.Channel or int.
-            ValueError: If the channel is not found.
-        """
-        if isinstance(channel, TeamTalkChannel):
-            channel = channel.id
-        # variable to hold the path
-        path = sdk.TTCHAR()
-        result = sdk._GetChannelPath(self.super, channel, path)
-        if not result:
-            raise ValueError("Channel not found")
-        return path.value
-
-    def get_channel_from_path(self, path: str) -> TeamTalkChannel:
-        """Gets a channel by its path.
-
-        Args:
-            path: The path of the channel to get.
-
-        Returns:
-            TeamTalkChannel: The channel.
-
-        Raises:
-            ValueError: If the channel is not found.
-        """
-        result = sdk._GetChannelIDFromPath(self.super, sdk.ttstr(path))
-        if result == 0:
-            raise ValueError("Channel not found")
-        return TeamTalkChannel(self, result)
-
-    # create a channel. Take in a name, parent channel. Optionally take in a topic, password and channel type
-    def create_channel(
-        self,
-        name: str,
-        parent_channel: Union[TeamTalkChannel, int],
-        topic: str = "",
-        password: str = "",
-        channel_type: ChannelType = ChannelType.CHANNEL_DEFAULT,
-    ) -> bool:
-        """Creates a channel.
-
-        Args:
-            name: The name of the channel to create.
-            parent_channel: The parent channel of the channel.
-            topic: The topic of the channel.
-            password: The password of the channel. Leave empty for no password.
-            channel_type: The type of the channel. Defaults to CHANNEL_DEFAULT.
-
-        Raises:
-            PermissionError: If the bot does not have permission to create channels.
-            ValueError: If the channel could not be created.
-
-        Returns:
-            bool: True if the channel was created, False otherwise.
-        """
-        if not self.has_permission(Permission.MODIFY_CHANNELS):
-            raise PermissionError("The bot does not have permission to create channels")
-        if isinstance(parent_channel, TeamTalkChannel):
-            parent_channel = parent_channel.id
-        new_channel = sdk.Channel()
-        new_channel.nParentID = parent_channel
-        new_channel.szName = sdk.ttstr(name)
-        new_channel.szTopic = sdk.ttstr(topic)
-        new_channel.szPassword = sdk.ttstr(password)
-        new_channel.bPassword = password != ""
-        new_channel.uChannelType = channel_type
-        result = sdk._DoMakeChannel(self._tt, new_channel)
-        if result == -1:
-            raise ValueError("Channel could not be created")
-        cmd_result, cmd_err = _waitForCmd(self.super, result, 2000)
-        if not cmd_result:
-            err_nr = cmd_err.nErrorNo
-            if err_nr == sdk.ClientError.CMDERR_NOT_LOGGEDIN:
-                raise PermissionError("The bot is not logged in")
-            if err_nr == sdk.ClientError.CMDERR_NOT_AUTHORIZED:
-                raise PermissionError("The bot does not have permission to create channels")
-            if err_nr == sdk.ClientError.CMDERR_CHANNEL_ALREADY_EXISTS:
-                raise ValueError("Channel already exists")
-            if err_nr == sdk.ClientError.CMDERR_CHANNEL_NOT_FOUND:
-                raise ValueError("Combined channel path is too long. Try using a shorter channel name")
-            if err_nr == sdk.ClientError.CMDERR_INCORRECT_CHANNEL_PASSWORD:
-                raise ValueError("Channel password too long")
-        return True
-
-    def delete_channel(self, channel: Union[TeamTalkChannel, int]):
-        """Deletes a channel.
-
-        Args:
-            channel: The channel to delete.
-
-        Raises:
-            TypeError: If the channel is not of type teamtalk.Channel or int.
-            PermissionError: If the bot doesn't have the permission to delete the channel.
-            ValueError: If the channel is not found.
-
-        Returns:
-            bool: True if the channel was deleted.
-        """
-        if not self.has_permission(Permission.MODIFY_CHANNELS):
-            raise PermissionError("The bot does not have permission to delete channels")
-        if isinstance(channel, TeamTalkChannel):
-            channel = channel.id
-        result = sdk._DoRemoveChannel(self._tt, channel)
-        if result == -1:
-            raise ValueError("Channel could not be deleted")
-        cmd_result, cmd_err = _waitForCmd(self.super, result, 2000)
-        if not cmd_result:
-            err_nr = cmd_err.nErrorNo
-            if err_nr == sdk.ClientError.CMDERR_NOT_LOGGEDIN:
-                raise PermissionError("The bot is not logged in")
-            if err_nr == sdk.ClientError.CMDERR_NOT_AUTHORIZED:
-                raise PermissionError("The bot does not have permission to delete channels")
-            if err_nr == sdk.ClientError.CMDERR_CHANNEL_NOT_FOUND:
-                raise ValueError("Channel not found.")
-        return True
-
-    def make_channel_operator(
-        self, user: Union[TeamTalkUser, int], channel: Union[TeamTalkUser, int], operator_password: str = ""
-    ) -> bool:
-        """Makes a user the channel operator.
-
-        Args:
-            user: The user to make the channel operator.
-            channel: The channel to make the user the channel operator in.
-            operator_password: The operator password of the channel.
-
-        Raises:
-            TypeError: If the user or channel is not of type teamtalk.User or int.
-            PermissionError: If the bot doesn't have the permission to make a user the channel operator.
-            ValueError: If the user or channel is not found.
-
-        Returns:
-            bool: True if the user was made the channel operator, False otherwise.
-        """
-        if isinstance(user, int):
-            user = self.get_user(user)
-        if isinstance(channel, int):
-            channel = self.get_channel(channel)
-        result = sdk.DoChannelOpEx(self.super, user.id, channel.id, sdk.ttstr(operator_password), True)
-        if result == -1:
-            raise PermissionError("The bot does not have the permission to make a user the channel operator")
-            return False
-        cmd_result, cmd_err = _waitForCmd(self.super, result, 2000)
-        if not cmd_result:
-            err_nr = cmd_err.nErrorNo
-            if err_nr == sdk.ClientError.CMDERR_NOT_LOGGEDIN:
-                raise PermissionError("The bot is not logged in")
-            if err_nr == sdk.ClientError.CMDERR_NOT_AUTHORIZED:
-                raise PermissionError("The bot does not have permission to make a user the channel operator")
-            if err_nr == sdk.ClientError.CMDERR_CHANNEL_NOT_FOUND:
-                raise ValueError("The channel does not exist")
-            if err_nr == sdk.ClientError.CMDERR_USER_NOT_FOUND:
-                raise ValueError("The user does not exist")
-            if err_nr == sdk.ClientError.CMDERR_INCORRECT_OP_PASSWORD:
-                raise ValueError("The operator password is incorrect")
-            return False
-        return True
-
-    def remove_channel_operator(
-        self, user: Union[TeamTalkUser, int], channel: Union[TeamTalkUser, int], operator_password: str = ""
-    ) -> bool:
-        """Removes a user as the channel operator.
-
-        Args:
-            user: The user to make the channel operator.
-            channel: The channel to make the user the channel operator in.
-            operator_password: The operator password of the channel.
-
-        Raises:
-            TypeError: If the user or channel is not of type teamtalk.User or int.
-            PermissionError: If the bot doesn't have the permission to make a user the channel operator.
-            ValueError: If the channel or user does not exist.
-
-        Returns:
-            bool: True if the user was removed as the channel operator, False otherwise.
-        """
-        if isinstance(user, int):
-            user = self.get_user(user)
-        if isinstance(channel, int):
-            channel = self.get_channel(channel)
-        result = sdk.DoChannelOpEx(self.super, user.id, channel.id, sdk.ttstr(operator_password), False)
-        if result == -1:
-            raise PermissionError("The bot does not have the permission to make a user the channel operator")
-            return False
-        cmd_result, cmd_err = _waitForCmd(self.super, result, 2000)
-        if not cmd_result:
-            err_nr = cmd_err.nErrorNo
-            if err_nr == sdk.ClientError.CMDERR_NOT_LOGGEDIN:
-                raise PermissionError("The bot is not logged in")
-            if err_nr == sdk.ClientError.CMDERR_NOT_AUTHORIZED:
-                raise PermissionError("The bot does not have permission to make a user the channel operator")
-            if err_nr == sdk.ClientError.CMDERR_CHANNEL_NOT_FOUND:
-                raise ValueError("The channel does not exist")
-            if err_nr == sdk.ClientError.CMDERR_USER_NOT_FOUND:
-                raise ValueError("The user does not exist")
-            if err_nr == sdk.ClientError.CMDERR_INCORRECT_OP_PASSWORD:
-                raise ValueError("The operator password is incorrect")
-            return False
-        return True
-
-    def get_user(self, user_id: int) -> TeamTalkUser:
-        """Gets a user by its ID.
-
-        Args:
-            user_id: The ID of the user to get.
-
-        Returns:
-            TeamTalkUser: The user.
-        """
-        return TeamTalkUser(self, user_id)
-
-    # user account stuff
-    def create_user_account(self, username: str, password: str, usertype: UserType) -> TeamTalkUserAccount:  # noqa
-        """Creates a user account on the server.
-
-        Args:
-            username: The username of the user account.
-            password: The password of the user account.
-            usertype: The type of the user account.
-
-        Returns:
-            TeamTalkUserAccount: The user account.
-
-        Raises:
-            ValueError: If the username or password is invalid.
-            PermissionError: If the bot does not have permission to create a user account or if the bot is not logged in.
-        """
-        account = sdk.UserAccount()
-        account.szUsername = username
-        account.szPassword = password
-        account.uUserType = usertype
-        result = sdk._DoNewUserAccount(self._tt, account)
-        if result == -1:
-            raise ValueError("Username or password is invalid")
-        cmd_result, cmd_err = _waitForCmd(self.super, result, 2000)
-        if not cmd_result:
-            err_nr = cmd_err.nErrorNo
-            if err_nr == sdk.ClientError.CMDERR_INVALID_USERNAME:
-                raise ValueError("Username is invalid")
-            if err_nr == sdk.ClientError.CMDERR_NOT_AUTHORIZED:
-                raise PermissionError("The bot does not have permission to create a user account")
-            if err_nr == sdk.ClientError.CMDERR_NOT_LOGGEDIN:
-                raise PermissionError("The bot is not logged in")
-        return True
-
-    def delete_user_account(self, username: str) -> bool:
-        """Deletes a user account.
-
-        Args:
-            username: The username of the user account to delete.
-
-        Returns:
-            bool: True if the user account was deleted, False otherwise.
-
-        Raises:
-            ValueError: If the username is empty or the user account does not exist.
-            PermissionError: If the user does not have permission to delete a user account.
-        """
-        if not username:
-            raise ValueError("Username is empty")
-        username = sdk.ttstr(username)
-        result = sdk._DoDeleteUserAccount(self._tt, username)
-        if result == -1:
-            raise ValueError("User account does not exist")
-        cmd_result, cmd_err = _waitForCmd(self.super, result, 2000)
-        if not cmd_result:
-            err_nr = cmd_err.nErrorNo
-            if err_nr == sdk.ClientError.CMDERR_NOT_AUTHORIZED:
-                raise PermissionError("The bot does not have permission to delete a user account")
-            if err_nr == sdk.ClientError.CMDERR_NOT_LOGGEDIN:
-                raise PermissionError("The bot is not logged in")
-            if err_nr == sdk.ClientError.CMDERR_ACCOUNT_NOT_FOUND:
-                raise ValueError("User account does not exist")
-        return True
-
-    async def list_user_accounts(self) -> List[TeamTalkUserAccount]:
-        """Lists all user accounts on the server.
-
-        Returns:
-            A list of all user accounts.
-
-        Raises:
-            PermissionError: If the bot is not an admin.
-            ValueError: If an unknown error occurred.
-        """
-        if not self.is_admin():
-            raise PermissionError("The bot is not an admin")
-        self.user_accounts = []
-        result = sdk._DoListUserAccounts(self._tt, 0, 1000000)
-        if result == -1:
-            raise ValueError("Unknown error")
-        await asyncio.sleep(1)
-        return self.user_accounts
-
-    # file stuff
-    def upload_file(self, channel_id: int, filepath: str) -> None:
-        """Uploads a local file to a channel.
-
-        Args:
-            channel_id: The ID of the channel to upload the file to.
-            filepath: The path to the local file to upload.
-
-        Raises:
-            PermissionError: If the bot does not have permission to upload files.
-            ValueError: If the channel ID is less than 0.
-            FileNotFoundError: If the local file does not exist.
-        """
-        if not self.has_permission(Permission.UPLOAD_FILES):
-            raise PermissionError("You do not have permission to upload files")
-        if channel_id < 0:
-            raise ValueError("Channel ID must be greater than 0")
-        if not os.path.exists(filepath):
-            raise FileNotFoundError(f"File {filepath} does not exist")
-        self.super.doSendFile(channel_id, sdk.ttstr(filepath))
-
-    def download_file(self, channel_id: int, remote_file_name: str, local_file_path: str) -> None:
-        """Downloads a remote file from a channel.
-
-        Args:
-            channel_id: The ID of the channel to download the file from.
-            remote_file_name: The name of the remote file to download.
-            local_file_path: The path to save the file to.
-
-        Raises:
-            PermissionError: If the bot does not have permission to download files.
-            ValueError: If the channel ID is less than 0.
-        """
-        if not self.has_permission(Permission.DOWNLOAD_FILES):
-            raise PermissionError("You do not have permission to download files")
-        if channel_id < 0:
-            raise ValueError("Channel ID must be greater than 0")
-        remote_files = self.get_channel_files(channel_id)
-        # loop through files and print the name
-        for file in remote_files:
-            if file.file_name == remote_file_name:
-                self.download_file_by_id(channel_id, file.file_id, local_file_path)
-
-    def download_file_by_id(self, channel_id: int, file_id: int, filepath: str):
-        """Downloads a remote file from a channel by its ID.
-
-        Args:
-            channel_id: The ID of the channel to download the file from.
-            file_id: The ID of the file to download.
-            filepath: The path to save the file to.
-
-        Raises:
-            PermissionError: If the bot does not have permission to download files.
-        """
-        if not self.has_permission(Permission.DOWNLOAD_FILES):
-            raise PermissionError("You do not have permission to download files")
-        self.super.doRecvFile(channel_id, file_id, sdk.ttstr(filepath))
-
-    def delete_file_by_id(self, channel_id: int, file_id: int):
-        """Deletes a remote file from a channel by its ID.
-
-        Args:
-            channel_id: The ID of the channel to delete the file from.
-            file_id: The ID of the file to delete.
-
-        Raises:
-            PermissionError: If the bot does not have permission to delete files.
-        """
-        if not self.is_admin(self.super.getMyUserID()):
-            raise PermissionError("You do not have permission to delete files")
-        self.super.doDeleteFile(channel_id, file_id)
-
-    def get_channel_files(self, channel_id: int) -> List[RemoteFile]:
-        """Gets a list of remote files in a channel.
-
-        Args:
-            channel_id: The ID of the channel to get the files from.
-
-        Returns:
-            List[RemoteFile]: A list of remote files in the channel.
-        """
-        files = self.super.getChannelFiles(channel_id)
-        return [RemoteFile(self, file) for file in files]
-
-    def move_user(self, user: Union[TeamTalkUser, int], channel: Union[TeamTalkChannel, int]) -> None:
-        """Moves a user to a channel.
-
-        Args:
-            user: The user to move.
-            channel: The channel to move the user to.
-
-        Raises:
-            PermissionError: If the bot does not have permission to move users.
-            TypeError: If the user or channel is not a subclass of User or Channel.
-        """
-        if not self.has_permission(Permission.MOVE_USERS):
-            raise PermissionError("You do not have permission to move users")
-        _log.debug(f"Moving user {user} to channel {channel}")
-        self._do_cmd(user, channel, "_DoMoveUser")
-
-    def kick_user(self, user: Union[TeamTalkUser, int], channel: Union[TeamTalkChannel, int]) -> None:
-        """Kicks a user from a channel or the server.
-
-        Args:
-            user: The user to kick.
-            channel: The channel to kick the user from. If 0, the user will be kicked from the server. # noqa
-
-        Raises:
-            PermissionError: If the bot does not have permission to kick users.
-            TypeError: If the user or channel is not a subclass of User or Channel.
-            ValueError: If the user or channel is not found.
-        """
-        # first check if we are kicking from channel or server
-        if channel == 0:  # server
-            if not self.has_permission(Permission.KICK_USERS):
-                raise PermissionError("You do not have permission to kick users")
-            _log.debug(f"Kicking user {user} from channel {channel}")
-            self._do_cmd(user, channel, "_DoKickUser")
-        else:  # channel
-            if not self.has_permission(Permission.KICK_USERS_FROM_CHANNEL) or not sdk._IsChannelOperator(
-                self._tt, self.super.getMyUserID(), channel
-            ):
-                raise PermissionError("You do not have permission to kick users from channels")
-            result = self._do_cmd(user, channel, "_DoKickUser")
-        if result == -1:
-            raise ValueError("Uknown error")
-            cmd_result, cmd_err = _waitForCmd(self.super, result, 2000)
-            if not cmd_result:
-                err_nr = cmd_err.nErrorNo
-                if err_nr == sdk.ClientError.CMDERR_USER_NOT_FOUND:
-                    raise ValueError("User not found")
-                if err_nr == sdk.ClientError.CMDERR_CHANNEL_NOT_FOUND:
-                    raise ValueError("Channel not found")
-            return cmd_result
-
-    def ban_user(self, user: Union[TeamTalkUser, int], channel: Union[TeamTalkChannel, int]) -> None:
-        """Bans a user from a channel or the server.
-
-        Args:
-            user: The user to ban.
-            channel: The channel to ban the user from. If 0, the user will be banned from the server. # noqa
-
-        Raises:
-            PermissionError: If the bot does not have permission to ban users.
-            TypeError: If the user or channel is not a subclass of User or Channel.
-            ValueError: If the user is not found.
-        """
-        if not self.has_permission(Permission.BAN_USERS):
-            raise PermissionError("You do not have permission to ban users")
-        _log.debug(f"Banning user {user} from channel {channel}")
-        result = self._do_cmd(user, channel, "_DoBanUser")
-        if result == -1:
-            raise ValueError("Uknown error")
-            cmd_result, cmd_err = _waitForCmd(self.super, result, 2000)
-            if not cmd_result:
-                err_nr = cmd_err.nErrorNo
-                if err_nr == sdk.ClientError.CMDERR_USER_NOT_FOUND:
-                    raise ValueError("User not found")
-            return cmd_result
-
-    def unban_user(self, ip: str, channel: Union[TeamTalkChannel, int]) -> None:
-        """Unbans a user from the server.
-
-        Args:
-            ip: The IP address of the user to unban.
-            channel: The channel to unban the user from. If 0, the user will be unbanned from the server. # noqa
-
-        Raises:
-            PermissionError: If the bot does not have permission to unban users.
-        """
-        if not self.has_permission(Permission.UNBAN_USERS):
-            raise PermissionError("You do not have permission to unban users")
-        if not isinstance(ip, str):
-            raise TypeError("IP must be a string")
-        if not isinstance(channel, (TeamTalkChannel, int)):
-            raise TypeError("Channel must be a subclass of Channel or a channel ID")
-        channel_id = channel
-        if isinstance(channel, TeamTalkChannel):
-            channel_id = channel.id
-        _log.debug(f"Unbanning user {ip}")
-        sdk._DoUnBanUser(self._tt, sdk.ttstr(ip), channel_id)
-
-    async def list_banned_users(self) -> List[TeamTalkBannedUserAccount]:
-        """Lists all banned users.
-
-        Returns:
-            List[BannedUserAccount]: A list of banned users.
-
-        Raises:
-            PermissionError: If the bot is not an admin.
-            ValueError: If an unknown error occurs.
-        """
-        if not self.is_admin():
-            raise PermissionError("The bot is not an admin")
-        self.banned_users = []
-        result = sdk._DoListBans(self._tt, 0, 0, 1000000)
-        if result == -1:
-            raise ValueError("Unknown error")
-        await asyncio.sleep(1)
-        return self.banned_users
-
-    def _send_message(self, message: sdk.TextMessage, **kwargs):
-        """Sends a message.
-
-        Args:
-            message: The message to send.
-            delay: The delay in seconds before sending the message. Defaults to 0 which means no delay. # noqa
-            **kwargs: Keyword arguments. Reserved for future use.
-
-
-        Raises:
-            TypeError: If the message is not a subclass of Message.
-        """
-        if not isinstance(message, sdk.TextMessage):
-            raise TypeError("Message must be a subclass of sdk.TextMessage")
-        if not issubclass(type(message), sdk.TextMessage):
-            raise TypeError("Message must be a subclass of sdk.TextMessage")
-        delay = kwargs.get("delay", 0)
-        _do_after(delay, lambda: self.super.doTextMessage(ctypes.POINTER(sdk.TextMessage)(message)))
-
-    async def _process_events(self) -> None:  # noqa: C901
-        """Processes events from the server. This is automatically called by teamtalk.Bot."""
-        msg = self.super.getMessage()
-        event = msg.nClientEvent
-        if event != sdk.ClientEvent.CLIENTEVENT_NONE and _getAbsTimeDiff(self.init_time, time.time()) < 1500:
-            # done so we don't get random events when logging in
-            return
-        if event == sdk.ClientEvent.CLIENTEVENT_NONE:
-            return
-        if event == sdk.ClientEvent.CLIENTEVENT_USER_AUDIOBLOCK:
-            self.bot.dispatch("user_audio", self, msg)
-            return
-        if event == sdk.ClientEvent.CLIENTEVENT_CMD_USER_TEXTMSG:
-            message = None
-            if msg.textmessage.nMsgType == sdk.TextMsgType.MSGTYPE_USER:
-                message = DirectMessage(self, msg.textmessage)
-            elif msg.textmessage.nMsgType == sdk.TextMsgType.MSGTYPE_CHANNEL:
-                message = ChannelMessage(self, msg.textmessage)
-            elif msg.textmessage.nMsgType == sdk.TextMsgType.MSGTYPE_BROADCAST:
-                message = BroadcastMessage(self, msg.textmessage)
-            elif msg.textmessage.nMsgType == sdk.TextMsgType.MSGTYPE_CUSTOM:
-                message = CustomMessage(self, msg.textmessage)
-            if message:
-                self.bot.dispatch("message", message)
-                return
-            # user events
-        if event == sdk.ClientEvent.CLIENTEVENT_CMD_USER_LOGGEDIN:
-            self.bot.dispatch("user_login", TeamTalkUser(self, msg.user))
-            return
-        if event == sdk.ClientEvent.CLIENTEVENT_CMD_USER_LOGGEDOUT:
-            self.bot.dispatch("user_logout", TeamTalkUser(self, msg.user))
-            return
-        if event == sdk.ClientEvent.CLIENTEVENT_CMD_USER_UPDATE:
-            self.bot.dispatch("user_update", TeamTalkUser(self, msg.user))
-            return
-        if event == sdk.ClientEvent.CLIENTEVENT_CMD_USER_JOINED:
-            user = TeamTalkUser(self, msg.user)
-            self.bot.dispatch("user_join", user, user.channel)
-            return
-        if event == sdk.ClientEvent.CLIENTEVENT_CMD_USER_LEFT:
-            user = TeamTalkUser(self, msg.user)
-            self.bot.dispatch("user_left", user, TeamTalkChannel(self, msg.nSource))
-            return
-        # channel events
-        if event == sdk.ClientEvent.CLIENTEVENT_CMD_CHANNEL_NEW:
-            self.bot.dispatch("channel_new", TeamTalkChannel(self, msg.channel))
-            return
-        if event == sdk.ClientEvent.CLIENTEVENT_CMD_CHANNEL_UPDATE:
-            self.bot.dispatch("channel_update", TeamTalkChannel(self, msg.channel))
-            return
-        if event == sdk.ClientEvent.CLIENTEVENT_CMD_CHANNEL_REMOVE:
-            self.bot.dispatch("channel_delete", TeamTalkChannel(self, msg.channel))
-            return
-        # server events
-        if event == sdk.ClientEvent.CLIENTEVENT_CMD_SERVER_UPDATE:
-            self.bot.dispatch("server_update", self.server)
-            return
-        if event == sdk.ClientEvent.CLIENTEVENT_CMD_SERVERSTATISTICS:
-            self.bot.dispatch("server_statistics", self.server)
-            return
-        # FILE EVENTS
-        if event == sdk.ClientEvent.CLIENTEVENT_CMD_FILE_NEW:
-            self.bot.dispatch("file_new", RemoteFile(self, msg.remotefile))
-            return
-        if event == sdk.ClientEvent.CLIENTEVENT_CMD_FILE_REMOVE:
-            self.bot.dispatch("file_delete", RemoteFile(self, msg.remotefile))
-            return
-        # other "my" events
-        if event == sdk.ClientEvent.CLIENTEVENT_CMD_MYSELF_KICKED:
-            self.bot.dispatch("my_kicked_from_channel", TeamTalkChannel(self, msg.nSource))
-            return
-        if event == sdk.ClientEvent.CLIENTEVENT_CMD_USERACCOUNT:
-            account = TeamTalkUserAccount(self, msg.useraccount)
-            self.user_accounts.append(account)
-            return
-        if event == sdk.ClientEvent.CLIENTEVENT_CMD_BANNEDUSER:
-            # cast our msg.useraccount to a banned user
-            banned_user_struct = sdk.BannedUser()
-            ctypes.memmove(ctypes.byref(banned_user_struct), ctypes.byref(msg.useraccount), ctypes.sizeof(sdk.BannedUser))
-            banned_user = TeamTalkBannedUserAccount(self, banned_user_struct)
-            self.banned_users.append(banned_user)
-            return
-        else:
-            # if we haven't handled the event, log it
-            # except if it's CLIENTEVENT_CMD_PROCESSING or CLIENTEVENT_CMD_ERROR or CLIENTEVENT_CMD_SUCCESS
-            if event not in (
-                sdk.ClientEvent.CLIENTEVENT_CMD_PROCESSING,
-                sdk.ClientEvent.CLIENTEVENT_CMD_ERROR,
-                sdk.ClientEvent.CLIENTEVENT_CMD_SUCCESS,
-            ):
-                _log.warning(f"Unhandled event: {event}")
-
-    def _get_channel_info(self, channel_id: int):
-        _channel = self.getChannel(channel_id)
-        _channel_path = self.getChannelPath(channel_id)
-        return _channel, _channel_path
-
-    def _get_my_permissions(self):
-        return self.super._GetMyUserRights()
-
-    def _do_cmd(self, user: Union[TeamTalkUser, int], channel: Union[TeamTalkChannel, int], func) -> None:
-        if not self.has_permission(Permission.KICK_USERS):
-            raise PermissionError("You do not have permission to kick users")
-        if not isinstance(user, (TeamTalkUser, int)):
-            raise TypeError("User must be a teamtalk.User or a user id")
-        if not isinstance(channel, (TeamTalkChannel, int)):
-            raise TypeError("Channel must be a teamtalk.Channel or a channel id")
-        user_id = user
-        if isinstance(user, TeamTalkUser):
-            user_id = user.user_id
-        channel_id = channel
-        if isinstance(channel, TeamTalkChannel):
-            channel_id = channel.id
-        sdk_func = getattr(sdk, func)
-        return sdk_func(self._tt, user_id, channel_id)
+"""This module contains the TeamTalkInstance class.
+
+The TeamTalkInstance class contains one instance of a connection to a TeamTalkServer.
+It is used to send and receive messages, join and leave channels, and perform other actions.
+In addition, it's also here that events are dispatched.
+"""
+
+import asyncio
+import os
+import logging
+import time
+import ctypes
+from typing import List, Union
+
+from ._utils import _getAbsTimeDiff, _waitForEvent, _waitForCmd, _do_after
+from .channel import Channel as TeamTalkChannel
+from .channel import ChannelType
+from .enums import TeamTalkServerInfo, UserStatusMode, UserType
+from .exceptions import PermissionError
+from .implementation.TeamTalkPy import TeamTalk5 as sdk
+from .message import BroadcastMessage, ChannelMessage, CustomMessage, DirectMessage
+from .permission import Permission
+from .server import Server as TeamTalkServer
+from .tt_file import RemoteFile
+from .user import User as TeamTalkUser
+from .user_account import UserAccount as TeamTalkUserAccount
+from .user_account import BannedUserAccount as TeamTalkBannedUserAccount
+
+
+_log = logging.getLogger(__name__)
+
+
+class TeamTalkInstance(sdk.TeamTalk):
+    """Represents a TeamTalk5 instance."""
+
+    def __init__(self, bot, server_info: TeamTalkServerInfo) -> None:
+        """Initializes a teamtalk.TeamTalkInstance instance.
+
+        Args:
+            bot: The teamtalk.Bot instance.
+            server_info: The server info for the server we wish to connect to.
+        """
+        # put the super class in a variable so we can call it later
+        self.super = super()
+        # call the super class's __init__ method
+        self.super.__init__()
+        # set the bot
+        self.bot = bot
+        # set the server info
+        self.server_info = server_info
+        self.server = TeamTalkServer(self, server_info)
+        self.channel = lambda: self.get_channel(self.super.getMyChannelID())
+        self.connected = False
+        self.logged_in = False
+        self.init_time = time.time()
+        self.user_accounts = []
+        self.banned_users = []
+
+    def connect(self) -> bool:
+        """Connects to the server. This doesn't return until the connection is successful or fails.
+
+        Returns:
+            bool: True if the connection was successful, False otherwise.
+        """
+        if not self.super.connect(
+            sdk.ttstr(self.server_info.host),
+            self.server_info.tcp_port,
+            self.server_info.udp_port,
+            self.server_info.encrypted,
+        ):
+            return False
+        result, msg = _waitForEvent(self.super, sdk.ClientEvent.CLIENTEVENT_CON_SUCCESS)
+        if not result:
+            return False
+        self.bot.dispatch("my_connect", self.server)
+        self.connected = True
+        self.init_time = time.time()
+        return True
+
+    def login(self, join_channel_on_login: bool = True) -> bool:
+        """Logs in to the server. This doesn't return until the login is successful or fails.
+
+        Args:
+            join_channel_on_login: Whether to join the channel on login or not.
+
+        Returns:
+            bool: True if the login was successful, False otherwise.
+        """
+        self.super.doLogin(
+            sdk.ttstr(self.server_info.nickname),
+            sdk.ttstr(self.server_info.username),
+            sdk.ttstr(self.server_info.password),
+            sdk.ttstr(self.bot.client_name),
+        )
+        result, msg = _waitForEvent(self.super, sdk.ClientEvent.CLIENTEVENT_CMD_MYSELF_LOGGEDIN)
+        if not result:
+            return False
+        self.bot.dispatch("my_login", self.server)
+        self.logged_in = True
+        if join_channel_on_login:
+            channel_id = self.server_info.join_channel_id
+            if channel_id < 1:
+                channel_id = self.super.getRootChannelID()
+            self.join_channel_by_id(channel_id)
+        self.init_time = time.time()
+        return True
+
+    def logout(self):
+        """Logs out of the server."""
+        self.super.doLogout()
+        self.logged_in = False
+
+    def disconnect(self):
+        """Disconnects from the server."""
+        self.super.disconnect()
+        self.connected = False
+
+    def change_nickname(self, nickname: str):
+        """Changes the nickname of the bot.
+
+        Args:
+            nickname: The new nickname.
+        """
+        self.super.doChangeNickname(nickname)
+
+    def change_status(self, status_mode: UserStatusMode, status_message: str):
+        """Changes the status of the bot.
+
+        Args:
+            status_mode: The status mode.
+            status_message: The status message.
+        """
+        self.super.doChangeStatus(status_mode, status_message)
+
+    # permission stuff
+    def has_permission(self, permission: Permission) -> bool:
+        """Checks if the bot has a permission.
+
+        If the user is an admin, they have all permissions.
+
+        Args:
+            permission: The permission to check for.
+
+        Returns:
+            bool: True if the bot has the permission, False otherwise.
+        """
+        user = self.super.getMyUserAccount()
+        # first check if they are an admin
+        if user.uUserType == sdk.UserType.USERTYPE_ADMIN:
+            return True
+        user_rights = user.uUserRights
+        return (user_rights & permission) == permission
+
+    def is_admin(self) -> bool:
+        """Checks if the bot is an admin.
+
+        Returns:
+            bool: True if the bot is an admin, False otherwise.
+        """
+        return self.is_user_admin(self.super.getMyUserID())
+
+    def is_user_admin(self, user: Union[TeamTalkUser, int]) -> bool:
+        """Checks if a user is an admin.
+
+        Args:
+            user: The user to check.
+
+        Returns:
+            bool: True if the user is an admin, False otherwise.
+
+        Raises:
+            TypeError: If the user is not of type teamtalk.User or int.
+        """
+        if isinstance(user, int):
+            user = self.super.getUser(user)
+            return user.uUserType == sdk.UserType.USERTYPE_ADMIN
+        if isinstance(user, TeamTalkUser):
+            return user.user_type == sdk.UserType.USERTYPE_ADMIN
+        raise TypeError("User must be of type teamtalk.User or int")
+
+    def join_root_channel(self):
+        """Joins the root channel."""
+        self.join_channel_by_id(self.super.getRootChannelID())
+
+    def join_channel_by_id(self, id: int, password: str = ""):
+        """Joins a channel by its ID.
+
+        Args:
+            id: The ID of the channel to join.
+            password: The password of the channel to join.
+        """
+        self.super.doJoinChannelByID(id, sdk.ttstr(password))
+
+    def join_channel(self, channel: TeamTalkChannel):
+        """Joins a channel.
+
+        Args:
+            channel: The channel to join.
+        """
+        self.super.doJoinChannelByID(channel.id, sdk.ttstr(channel.password))
+
+    def leave_channel(self):
+        """Leaves the current channel."""
+        self.super.doLeaveChannel()
+
+    def get_channel(self, channel_id: int) -> TeamTalkChannel:
+        """Gets a channel by its ID.
+
+        Args:
+            channel_id: The ID of the channel to get.
+
+        Returns:
+            TeamTalkChannel: The channel.
+        """
+        return TeamTalkChannel(self, channel_id)
+
+    def get_path_from_channel(self, channel: Union[TeamTalkChannel, int]) -> str:
+        """Gets the path of a channel.
+
+        Args:
+            channel: The channel to get the path of.
+
+        Returns:
+            str: The path of the channel.
+
+        Raises:
+            TypeError: If the channel is not of type teamtalk.Channel or int.
+            ValueError: If the channel is not found.
+        """
+        if isinstance(channel, TeamTalkChannel):
+            channel = channel.id
+        # variable to hold the path
+        path = sdk.TTCHAR()
+        result = sdk._GetChannelPath(self.super, channel, path)
+        if not result:
+            raise ValueError("Channel not found")
+        return path.value
+
+    def get_channel_from_path(self, path: str) -> TeamTalkChannel:
+        """Gets a channel by its path.
+
+        Args:
+            path: The path of the channel to get.
+
+        Returns:
+            TeamTalkChannel: The channel.
+
+        Raises:
+            ValueError: If the channel is not found.
+        """
+        result = sdk._GetChannelIDFromPath(self.super, sdk.ttstr(path))
+        if result == 0:
+            raise ValueError("Channel not found")
+        return TeamTalkChannel(self, result)
+
+    # create a channel. Take in a name, parent channel. Optionally take in a topic, password and channel type
+    def create_channel(
+        self,
+        name: str,
+        parent_channel: Union[TeamTalkChannel, int],
+        topic: str = "",
+        password: str = "",
+        channel_type: ChannelType = ChannelType.CHANNEL_DEFAULT,
+    ) -> bool:
+        """Creates a channel.
+
+        Args:
+            name: The name of the channel to create.
+            parent_channel: The parent channel of the channel.
+            topic: The topic of the channel.
+            password: The password of the channel. Leave empty for no password.
+            channel_type: The type of the channel. Defaults to CHANNEL_DEFAULT.
+
+        Raises:
+            PermissionError: If the bot does not have permission to create channels.
+            ValueError: If the channel could not be created.
+
+        Returns:
+            bool: True if the channel was created, False otherwise.
+        """
+        if not self.has_permission(Permission.MODIFY_CHANNELS):
+            raise PermissionError("The bot does not have permission to create channels")
+        if isinstance(parent_channel, TeamTalkChannel):
+            parent_channel = parent_channel.id
+        new_channel = sdk.Channel()
+        new_channel.nParentID = parent_channel
+        new_channel.szName = sdk.ttstr(name)
+        new_channel.szTopic = sdk.ttstr(topic)
+        new_channel.szPassword = sdk.ttstr(password)
+        new_channel.bPassword = password != ""
+        new_channel.uChannelType = channel_type
+        result = sdk._DoMakeChannel(self._tt, new_channel)
+        if result == -1:
+            raise ValueError("Channel could not be created")
+        cmd_result, cmd_err = _waitForCmd(self.super, result, 2000)
+        if not cmd_result:
+            err_nr = cmd_err.nErrorNo
+            if err_nr == sdk.ClientError.CMDERR_NOT_LOGGEDIN:
+                raise PermissionError("The bot is not logged in")
+            if err_nr == sdk.ClientError.CMDERR_NOT_AUTHORIZED:
+                raise PermissionError("The bot does not have permission to create channels")
+            if err_nr == sdk.ClientError.CMDERR_CHANNEL_ALREADY_EXISTS:
+                raise ValueError("Channel already exists")
+            if err_nr == sdk.ClientError.CMDERR_CHANNEL_NOT_FOUND:
+                raise ValueError("Combined channel path is too long. Try using a shorter channel name")
+            if err_nr == sdk.ClientError.CMDERR_INCORRECT_CHANNEL_PASSWORD:
+                raise ValueError("Channel password too long")
+        return True
+
+    def delete_channel(self, channel: Union[TeamTalkChannel, int]):
+        """Deletes a channel.
+
+        Args:
+            channel: The channel to delete.
+
+        Raises:
+            TypeError: If the channel is not of type teamtalk.Channel or int.
+            PermissionError: If the bot doesn't have the permission to delete the channel.
+            ValueError: If the channel is not found.
+
+        Returns:
+            bool: True if the channel was deleted.
+        """
+        if not self.has_permission(Permission.MODIFY_CHANNELS):
+            raise PermissionError("The bot does not have permission to delete channels")
+        if isinstance(channel, TeamTalkChannel):
+            channel = channel.id
+        result = sdk._DoRemoveChannel(self._tt, channel)
+        if result == -1:
+            raise ValueError("Channel could not be deleted")
+        cmd_result, cmd_err = _waitForCmd(self.super, result, 2000)
+        if not cmd_result:
+            err_nr = cmd_err.nErrorNo
+            if err_nr == sdk.ClientError.CMDERR_NOT_LOGGEDIN:
+                raise PermissionError("The bot is not logged in")
+            if err_nr == sdk.ClientError.CMDERR_NOT_AUTHORIZED:
+                raise PermissionError("The bot does not have permission to delete channels")
+            if err_nr == sdk.ClientError.CMDERR_CHANNEL_NOT_FOUND:
+                raise ValueError("Channel not found.")
+        return True
+
+    def make_channel_operator(
+        self, user: Union[TeamTalkUser, int], channel: Union[TeamTalkUser, int], operator_password: str = ""
+    ) -> bool:
+        """Makes a user the channel operator.
+
+        Args:
+            user: The user to make the channel operator.
+            channel: The channel to make the user the channel operator in.
+            operator_password: The operator password of the channel.
+
+        Raises:
+            TypeError: If the user or channel is not of type teamtalk.User or int.
+            PermissionError: If the bot doesn't have the permission to make a user the channel operator.
+            ValueError: If the user or channel is not found.
+
+        Returns:
+            bool: True if the user was made the channel operator, False otherwise.
+        """
+        if isinstance(user, int):
+            user = self.get_user(user)
+        if isinstance(channel, int):
+            channel = self.get_channel(channel)
+        result = sdk.DoChannelOpEx(self.super, user.id, channel.id, sdk.ttstr(operator_password), True)
+        if result == -1:
+            raise PermissionError("The bot does not have the permission to make a user the channel operator")
+            return False
+        cmd_result, cmd_err = _waitForCmd(self.super, result, 2000)
+        if not cmd_result:
+            err_nr = cmd_err.nErrorNo
+            if err_nr == sdk.ClientError.CMDERR_NOT_LOGGEDIN:
+                raise PermissionError("The bot is not logged in")
+            if err_nr == sdk.ClientError.CMDERR_NOT_AUTHORIZED:
+                raise PermissionError("The bot does not have permission to make a user the channel operator")
+            if err_nr == sdk.ClientError.CMDERR_CHANNEL_NOT_FOUND:
+                raise ValueError("The channel does not exist")
+            if err_nr == sdk.ClientError.CMDERR_USER_NOT_FOUND:
+                raise ValueError("The user does not exist")
+            if err_nr == sdk.ClientError.CMDERR_INCORRECT_OP_PASSWORD:
+                raise ValueError("The operator password is incorrect")
+            return False
+        return True
+
+    def remove_channel_operator(
+        self, user: Union[TeamTalkUser, int], channel: Union[TeamTalkUser, int], operator_password: str = ""
+    ) -> bool:
+        """Removes a user as the channel operator.
+
+        Args:
+            user: The user to make the channel operator.
+            channel: The channel to make the user the channel operator in.
+            operator_password: The operator password of the channel.
+
+        Raises:
+            TypeError: If the user or channel is not of type teamtalk.User or int.
+            PermissionError: If the bot doesn't have the permission to make a user the channel operator.
+            ValueError: If the channel or user does not exist.
+
+        Returns:
+            bool: True if the user was removed as the channel operator, False otherwise.
+        """
+        if isinstance(user, int):
+            user = self.get_user(user)
+        if isinstance(channel, int):
+            channel = self.get_channel(channel)
+        result = sdk.DoChannelOpEx(self.super, user.id, channel.id, sdk.ttstr(operator_password), False)
+        if result == -1:
+            raise PermissionError("The bot does not have the permission to make a user the channel operator")
+            return False
+        cmd_result, cmd_err = _waitForCmd(self.super, result, 2000)
+        if not cmd_result:
+            err_nr = cmd_err.nErrorNo
+            if err_nr == sdk.ClientError.CMDERR_NOT_LOGGEDIN:
+                raise PermissionError("The bot is not logged in")
+            if err_nr == sdk.ClientError.CMDERR_NOT_AUTHORIZED:
+                raise PermissionError("The bot does not have permission to make a user the channel operator")
+            if err_nr == sdk.ClientError.CMDERR_CHANNEL_NOT_FOUND:
+                raise ValueError("The channel does not exist")
+            if err_nr == sdk.ClientError.CMDERR_USER_NOT_FOUND:
+                raise ValueError("The user does not exist")
+            if err_nr == sdk.ClientError.CMDERR_INCORRECT_OP_PASSWORD:
+                raise ValueError("The operator password is incorrect")
+            return False
+        return True
+
+    def get_user(self, user_id: int) -> TeamTalkUser:
+        """Gets a user by its ID.
+
+        Args:
+            user_id: The ID of the user to get.
+
+        Returns:
+            TeamTalkUser: The user.
+        """
+        return TeamTalkUser(self, user_id)
+
+    # user account stuff
+    def create_user_account(self, username: str, password: str, usertype: UserType) -> TeamTalkUserAccount:  # noqa
+        """Creates a user account on the server.
+
+        Args:
+            username: The username of the user account.
+            password: The password of the user account.
+            usertype: The type of the user account.
+
+        Returns:
+            TeamTalkUserAccount: The user account.
+
+        Raises:
+            ValueError: If the username or password is invalid.
+            PermissionError: If the bot does not have permission to create a user account or if the bot is not logged in.
+        """
+        account = sdk.UserAccount()
+        account.szUsername = username
+        account.szPassword = password
+        account.uUserType = usertype
+        result = sdk._DoNewUserAccount(self._tt, account)
+        if result == -1:
+            raise ValueError("Username or password is invalid")
+        cmd_result, cmd_err = _waitForCmd(self.super, result, 2000)
+        if not cmd_result:
+            err_nr = cmd_err.nErrorNo
+            if err_nr == sdk.ClientError.CMDERR_INVALID_USERNAME:
+                raise ValueError("Username is invalid")
+            if err_nr == sdk.ClientError.CMDERR_NOT_AUTHORIZED:
+                raise PermissionError("The bot does not have permission to create a user account")
+            if err_nr == sdk.ClientError.CMDERR_NOT_LOGGEDIN:
+                raise PermissionError("The bot is not logged in")
+        return True
+
+    def delete_user_account(self, username: str) -> bool:
+        """Deletes a user account.
+
+        Args:
+            username: The username of the user account to delete.
+
+        Returns:
+            bool: True if the user account was deleted, False otherwise.
+
+        Raises:
+            ValueError: If the username is empty or the user account does not exist.
+            PermissionError: If the user does not have permission to delete a user account.
+        """
+        if not username:
+            raise ValueError("Username is empty")
+        username = sdk.ttstr(username)
+        result = sdk._DoDeleteUserAccount(self._tt, username)
+        if result == -1:
+            raise ValueError("User account does not exist")
+        cmd_result, cmd_err = _waitForCmd(self.super, result, 2000)
+        if not cmd_result:
+            err_nr = cmd_err.nErrorNo
+            if err_nr == sdk.ClientError.CMDERR_NOT_AUTHORIZED:
+                raise PermissionError("The bot does not have permission to delete a user account")
+            if err_nr == sdk.ClientError.CMDERR_NOT_LOGGEDIN:
+                raise PermissionError("The bot is not logged in")
+            if err_nr == sdk.ClientError.CMDERR_ACCOUNT_NOT_FOUND:
+                raise ValueError("User account does not exist")
+        return True
+
+    async def list_user_accounts(self) -> List[TeamTalkUserAccount]:
+        """Lists all user accounts on the server.
+
+        Returns:
+            A list of all user accounts.
+
+        Raises:
+            PermissionError: If the bot is not an admin.
+            ValueError: If an unknown error occurred.
+        """
+        if not self.is_admin():
+            raise PermissionError("The bot is not an admin")
+        self.user_accounts = []
+        result = sdk._DoListUserAccounts(self._tt, 0, 1000000)
+        if result == -1:
+            raise ValueError("Unknown error")
+        await asyncio.sleep(1)
+        return self.user_accounts
+
+    # file stuff
+    def upload_file(self, channel_id: int, filepath: str) -> None:
+        """Uploads a local file to a channel.
+
+        Args:
+            channel_id: The ID of the channel to upload the file to.
+            filepath: The path to the local file to upload.
+
+        Raises:
+            PermissionError: If the bot does not have permission to upload files.
+            ValueError: If the channel ID is less than 0.
+            FileNotFoundError: If the local file does not exist.
+        """
+        if not self.has_permission(Permission.UPLOAD_FILES):
+            raise PermissionError("You do not have permission to upload files")
+        if channel_id < 0:
+            raise ValueError("Channel ID must be greater than 0")
+        if not os.path.exists(filepath):
+            raise FileNotFoundError(f"File {filepath} does not exist")
+        self.super.doSendFile(channel_id, sdk.ttstr(filepath))
+
+    def download_file(self, channel_id: int, remote_file_name: str, local_file_path: str) -> None:
+        """Downloads a remote file from a channel.
+
+        Args:
+            channel_id: The ID of the channel to download the file from.
+            remote_file_name: The name of the remote file to download.
+            local_file_path: The path to save the file to.
+
+        Raises:
+            PermissionError: If the bot does not have permission to download files.
+            ValueError: If the channel ID is less than 0.
+        """
+        if not self.has_permission(Permission.DOWNLOAD_FILES):
+            raise PermissionError("You do not have permission to download files")
+        if channel_id < 0:
+            raise ValueError("Channel ID must be greater than 0")
+        remote_files = self.get_channel_files(channel_id)
+        # loop through files and print the name
+        for file in remote_files:
+            if file.file_name == remote_file_name:
+                self.download_file_by_id(channel_id, file.file_id, local_file_path)
+
+    def download_file_by_id(self, channel_id: int, file_id: int, filepath: str):
+        """Downloads a remote file from a channel by its ID.
+
+        Args:
+            channel_id: The ID of the channel to download the file from.
+            file_id: The ID of the file to download.
+            filepath: The path to save the file to.
+
+        Raises:
+            PermissionError: If the bot does not have permission to download files.
+        """
+        if not self.has_permission(Permission.DOWNLOAD_FILES):
+            raise PermissionError("You do not have permission to download files")
+        self.super.doRecvFile(channel_id, file_id, sdk.ttstr(filepath))
+
+    def delete_file_by_id(self, channel_id: int, file_id: int):
+        """Deletes a remote file from a channel by its ID.
+
+        Args:
+            channel_id: The ID of the channel to delete the file from.
+            file_id: The ID of the file to delete.
+
+        Raises:
+            PermissionError: If the bot does not have permission to delete files.
+        """
+        if not self.is_admin(self.super.getMyUserID()):
+            raise PermissionError("You do not have permission to delete files")
+        self.super.doDeleteFile(channel_id, file_id)
+
+    def get_channel_files(self, channel_id: int) -> List[RemoteFile]:
+        """Gets a list of remote files in a channel.
+
+        Args:
+            channel_id: The ID of the channel to get the files from.
+
+        Returns:
+            List[RemoteFile]: A list of remote files in the channel.
+        """
+        files = self.super.getChannelFiles(channel_id)
+        return [RemoteFile(self, file) for file in files]
+
+    def move_user(self, user: Union[TeamTalkUser, int], channel: Union[TeamTalkChannel, int]) -> None:
+        """Moves a user to a channel.
+
+        Args:
+            user: The user to move.
+            channel: The channel to move the user to.
+
+        Raises:
+            PermissionError: If the bot does not have permission to move users.
+            TypeError: If the user or channel is not a subclass of User or Channel.
+        """
+        if not self.has_permission(Permission.MOVE_USERS):
+            raise PermissionError("You do not have permission to move users")
+        _log.debug(f"Moving user {user} to channel {channel}")
+        self._do_cmd(user, channel, "_DoMoveUser")
+
+    def kick_user(self, user: Union[TeamTalkUser, int], channel: Union[TeamTalkChannel, int]) -> None:
+        """Kicks a user from a channel or the server.
+
+        Args:
+            user: The user to kick.
+            channel: The channel to kick the user from. If 0, the user will be kicked from the server. # noqa
+
+        Raises:
+            PermissionError: If the bot does not have permission to kick users.
+            TypeError: If the user or channel is not a subclass of User or Channel.
+            ValueError: If the user or channel is not found.
+        """
+        # first check if we are kicking from channel or server
+        if channel == 0:  # server
+            if not self.has_permission(Permission.KICK_USERS):
+                raise PermissionError("You do not have permission to kick users")
+            _log.debug(f"Kicking user {user} from channel {channel}")
+            self._do_cmd(user, channel, "_DoKickUser")
+        else:  # channel
+            if not self.has_permission(Permission.KICK_USERS_FROM_CHANNEL) or not sdk._IsChannelOperator(
+                self._tt, self.super.getMyUserID(), channel
+            ):
+                raise PermissionError("You do not have permission to kick users from channels")
+            result = self._do_cmd(user, channel, "_DoKickUser")
+        if result == -1:
+            raise ValueError("Uknown error")
+            cmd_result, cmd_err = _waitForCmd(self.super, result, 2000)
+            if not cmd_result:
+                err_nr = cmd_err.nErrorNo
+                if err_nr == sdk.ClientError.CMDERR_USER_NOT_FOUND:
+                    raise ValueError("User not found")
+                if err_nr == sdk.ClientError.CMDERR_CHANNEL_NOT_FOUND:
+                    raise ValueError("Channel not found")
+            return cmd_result
+
+    def ban_user(self, user: Union[TeamTalkUser, int], channel: Union[TeamTalkChannel, int]) -> None:
+        """Bans a user from a channel or the server.
+
+        Args:
+            user: The user to ban.
+            channel: The channel to ban the user from. If 0, the user will be banned from the server. # noqa
+
+        Raises:
+            PermissionError: If the bot does not have permission to ban users.
+            TypeError: If the user or channel is not a subclass of User or Channel.
+            ValueError: If the user is not found.
+        """
+        if not self.has_permission(Permission.BAN_USERS):
+            raise PermissionError("You do not have permission to ban users")
+        _log.debug(f"Banning user {user} from channel {channel}")
+        result = self._do_cmd(user, channel, "_DoBanUser")
+        if result == -1:
+            raise ValueError("Uknown error")
+            cmd_result, cmd_err = _waitForCmd(self.super, result, 2000)
+            if not cmd_result:
+                err_nr = cmd_err.nErrorNo
+                if err_nr == sdk.ClientError.CMDERR_USER_NOT_FOUND:
+                    raise ValueError("User not found")
+            return cmd_result
+
+    def unban_user(self, ip: str, channel: Union[TeamTalkChannel, int]) -> None:
+        """Unbans a user from the server.
+
+        Args:
+            ip: The IP address of the user to unban.
+            channel: The channel to unban the user from. If 0, the user will be unbanned from the server. # noqa
+
+        Raises:
+            PermissionError: If the bot does not have permission to unban users.
+        """
+        if not self.has_permission(Permission.UNBAN_USERS):
+            raise PermissionError("You do not have permission to unban users")
+        if not isinstance(ip, str):
+            raise TypeError("IP must be a string")
+        if not isinstance(channel, (TeamTalkChannel, int)):
+            raise TypeError("Channel must be a subclass of Channel or a channel ID")
+        channel_id = channel
+        if isinstance(channel, TeamTalkChannel):
+            channel_id = channel.id
+        _log.debug(f"Unbanning user {ip}")
+        sdk._DoUnBanUser(self._tt, sdk.ttstr(ip), channel_id)
+
+    async def list_banned_users(self) -> List[TeamTalkBannedUserAccount]:
+        """Lists all banned users.
+
+        Returns:
+            List[BannedUserAccount]: A list of banned users.
+
+        Raises:
+            PermissionError: If the bot is not an admin.
+            ValueError: If an unknown error occurs.
+        """
+        if not self.is_admin():
+            raise PermissionError("The bot is not an admin")
+        self.banned_users = []
+        result = sdk._DoListBans(self._tt, 0, 0, 1000000)
+        if result == -1:
+            raise ValueError("Unknown error")
+        await asyncio.sleep(1)
+        return self.banned_users
+
+    def _send_message(self, message: sdk.TextMessage, **kwargs):
+        """Sends a message.
+
+        Args:
+            message: The message to send.
+            delay: The delay in seconds before sending the message. Defaults to 0 which means no delay. # noqa
+            **kwargs: Keyword arguments. Reserved for future use.
+
+
+        Raises:
+            TypeError: If the message is not a subclass of Message.
+        """
+        if not isinstance(message, sdk.TextMessage):
+            raise TypeError("Message must be a subclass of sdk.TextMessage")
+        if not issubclass(type(message), sdk.TextMessage):
+            raise TypeError("Message must be a subclass of sdk.TextMessage")
+        delay = kwargs.get("delay", 0)
+        _do_after(delay, lambda: self.super.doTextMessage(ctypes.POINTER(sdk.TextMessage)(message)))
+
+    async def _process_events(self) -> None:  # noqa: C901
+        """Processes events from the server. This is automatically called by teamtalk.Bot."""
+        msg = self.super.getMessage()
+        event = msg.nClientEvent
+        if event != sdk.ClientEvent.CLIENTEVENT_NONE and _getAbsTimeDiff(self.init_time, time.time()) < 1500:
+            # done so we don't get random events when logging in
+            return
+        if event == sdk.ClientEvent.CLIENTEVENT_NONE:
+            return
+        if event == sdk.ClientEvent.CLIENTEVENT_USER_AUDIOBLOCK:
+            self.bot.dispatch("user_audio", self, msg)
+            return
+        if event == sdk.ClientEvent.CLIENTEVENT_CMD_USER_TEXTMSG:
+            message = None
+            if msg.textmessage.nMsgType == sdk.TextMsgType.MSGTYPE_USER:
+                message = DirectMessage(self, msg.textmessage)
+            elif msg.textmessage.nMsgType == sdk.TextMsgType.MSGTYPE_CHANNEL:
+                message = ChannelMessage(self, msg.textmessage)
+            elif msg.textmessage.nMsgType == sdk.TextMsgType.MSGTYPE_BROADCAST:
+                message = BroadcastMessage(self, msg.textmessage)
+            elif msg.textmessage.nMsgType == sdk.TextMsgType.MSGTYPE_CUSTOM:
+                message = CustomMessage(self, msg.textmessage)
+            if message:
+                self.bot.dispatch("message", message)
+                return
+            # user events
+        if event == sdk.ClientEvent.CLIENTEVENT_CMD_USER_LOGGEDIN:
+            self.bot.dispatch("user_login", TeamTalkUser(self, msg.user))
+            return
+        if event == sdk.ClientEvent.CLIENTEVENT_CMD_USER_LOGGEDOUT:
+            self.bot.dispatch("user_logout", TeamTalkUser(self, msg.user))
+            return
+        if event == sdk.ClientEvent.CLIENTEVENT_CMD_USER_UPDATE:
+            self.bot.dispatch("user_update", TeamTalkUser(self, msg.user))
+            return
+        if event == sdk.ClientEvent.CLIENTEVENT_CMD_USER_JOINED:
+            user = TeamTalkUser(self, msg.user)
+            self.bot.dispatch("user_join", user, user.channel)
+            return
+        if event == sdk.ClientEvent.CLIENTEVENT_CMD_USER_LEFT:
+            user = TeamTalkUser(self, msg.user)
+            self.bot.dispatch("user_left", user, TeamTalkChannel(self, msg.nSource))
+            return
+        # channel events
+        if event == sdk.ClientEvent.CLIENTEVENT_CMD_CHANNEL_NEW:
+            self.bot.dispatch("channel_new", TeamTalkChannel(self, msg.channel))
+            return
+        if event == sdk.ClientEvent.CLIENTEVENT_CMD_CHANNEL_UPDATE:
+            self.bot.dispatch("channel_update", TeamTalkChannel(self, msg.channel))
+            return
+        if event == sdk.ClientEvent.CLIENTEVENT_CMD_CHANNEL_REMOVE:
+            self.bot.dispatch("channel_delete", TeamTalkChannel(self, msg.channel))
+            return
+        # server events
+        if event == sdk.ClientEvent.CLIENTEVENT_CMD_SERVER_UPDATE:
+            self.bot.dispatch("server_update", self.server)
+            return
+        if event == sdk.ClientEvent.CLIENTEVENT_CMD_SERVERSTATISTICS:
+            self.bot.dispatch("server_statistics", self.server)
+            return
+        # FILE EVENTS
+        if event == sdk.ClientEvent.CLIENTEVENT_CMD_FILE_NEW:
+            self.bot.dispatch("file_new", RemoteFile(self, msg.remotefile))
+            return
+        if event == sdk.ClientEvent.CLIENTEVENT_CMD_FILE_REMOVE:
+            self.bot.dispatch("file_delete", RemoteFile(self, msg.remotefile))
+            return
+        # other "my" events
+        if event == sdk.ClientEvent.CLIENTEVENT_CMD_MYSELF_KICKED:
+            self.bot.dispatch("my_kicked_from_channel", TeamTalkChannel(self, msg.nSource))
+            return
+        if event == sdk.ClientEvent.CLIENTEVENT_CMD_USERACCOUNT:
+            account = TeamTalkUserAccount(self, msg.useraccount)
+            self.user_accounts.append(account)
+            return
+        if event == sdk.ClientEvent.CLIENTEVENT_CMD_BANNEDUSER:
+            # cast our msg.useraccount to a banned user
+            banned_user_struct = sdk.BannedUser()
+            ctypes.memmove(ctypes.byref(banned_user_struct), ctypes.byref(msg.useraccount), ctypes.sizeof(sdk.BannedUser))
+            banned_user = TeamTalkBannedUserAccount(self, banned_user_struct)
+            self.banned_users.append(banned_user)
+            return
+        else:
+            # if we haven't handled the event, log it
+            # except if it's CLIENTEVENT_CMD_PROCESSING or CLIENTEVENT_CMD_ERROR or CLIENTEVENT_CMD_SUCCESS
+            if event not in (
+                sdk.ClientEvent.CLIENTEVENT_CMD_PROCESSING,
+                sdk.ClientEvent.CLIENTEVENT_CMD_ERROR,
+                sdk.ClientEvent.CLIENTEVENT_CMD_SUCCESS,
+            ):
+                _log.warning(f"Unhandled event: {event}")
+
+    def _get_channel_info(self, channel_id: int):
+        _channel = self.getChannel(channel_id)
+        _channel_path = self.getChannelPath(channel_id)
+        return _channel, _channel_path
+
+    def _get_my_permissions(self):
+        return self.super._GetMyUserRights()
+
+    def _do_cmd(self, user: Union[TeamTalkUser, int], channel: Union[TeamTalkChannel, int], func) -> None:
+        if not self.has_permission(Permission.KICK_USERS):
+            raise PermissionError("You do not have permission to kick users")
+        if not isinstance(user, (TeamTalkUser, int)):
+            raise TypeError("User must be a teamtalk.User or a user id")
+        if not isinstance(channel, (TeamTalkChannel, int)):
+            raise TypeError("Channel must be a teamtalk.Channel or a channel id")
+        user_id = user
+        if isinstance(user, TeamTalkUser):
+            user_id = user.user_id
+        channel_id = channel
+        if isinstance(channel, TeamTalkChannel):
+            channel_id = channel.id
+        sdk_func = getattr(sdk, func)
+        return sdk_func(self._tt, user_id, channel_id)
```

### Comparing `teamtalk_py-1.1.0/teamtalk/message.py` & `teamtalk_py-1.1.1/teamtalk/message.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,141 +1,141 @@
-"""This module contains the Message class and its subclasses."""
-
-
-from .implementation.TeamTalkPy import TeamTalk5 as sdk
-
-
-class Message:
-    """Represents a TeamTalk5 message. This class should not be instantiated directly."""
-
-    def __init__(self, teamtalk_instance, msg):
-        """Initializes a Message instance.
-
-        Args:
-            teamtalk_instance: An instance of teamtalk.TeamTalkInstance.
-            msg: The message.
-        """
-        self.teamtalk_instance = teamtalk_instance
-        self.type = msg.nMsgType
-        self.from_id = msg.nFromUserID
-        self.to_id = msg.nToUserID
-        self.content = msg.szMessage
-        # if content is a byte array, decode it
-        if isinstance(self.content, bytes):
-            self.content = self.content.decode("utf-8")
-        self.user = self.teamtalk_instance.get_user(self.from_id)
-
-    def reply(self, content, **kwargs):
-        """Replies to the message.
-
-        The reply will be sent to the place where the message was sent from.
-        Meaning that if the message was sent to a channel, the reply will be sent to the channel.
-        If the message was sent to a user, the reply will be sent to the user.
-        And if the message was a broadcast message, the reply will be sent to the server as a broadcast.
-
-        Args:
-            content: The content of the message.
-            **kwargs: Keyword arguments. See teamtalk.TeamTalkInstance.send_message for more information.
-
-        Returns:
-            The message ID of the reply.
-
-        Raises:
-            PermissionError: If the sender doesn't have permission to send the message.
-        """
-        msg = sdk.TextMessage()
-        msg.nMsgType = self.type
-        msg.nFromUserID = self.teamtalk_instance.super.getMyUserID()
-        msg.szFromUsername = self.teamtalk_instance.super.getMyUserAccount().szUsername
-        # if self is channel message, then reply to channel
-        if isinstance(self, ChannelMessage):
-            if self.teamtalk_instance.super.getMyChannelID() != self.to_id:
-                if not self.teamtalk_instance.is_admin():
-                    raise PermissionError("You don't have permission to send messages across channels.")
-            msg.nChannelID = self.to_id
-        if isinstance(self, BroadcastMessage):
-            # if we aren ot admin we cant do this
-            if not self.teamtalk_instance.is_admin():
-                raise PermissionError("You don't have permission to send broadcast messages.")
-            msg.nToUserID = 0
-            msg.nChannelID = 0
-        else:
-            msg.nToUserID = self.from_id
-        msg.szMessage = sdk.ttstr(content)
-        msg.bMore = False
-        return self.teamtalk_instance._send_message(msg, **kwargs)
-
-    def is_me(self) -> bool:
-        """Checks if the message was sent by the bot.
-
-        Returns:
-            True if the message was sent by the bot, False otherwise.
-        """
-        return self.from_id == self.teamtalk_instance.super.getMyUserID()
-
-    def __str__(self) -> str:
-        """Returns a string representation of the message.
-
-        Returns:
-            A string representation of the message.
-        """
-        return f"teamtalk.{type(self).__name__}(from_id={self.from_id}, to_id={self.to_id}, content={self.content})"
-
-
-# make a channel message subclass
-class ChannelMessage(Message):
-    """Represents a message sent to a channel. This class should not be instantiated directly."""
-
-    def __init__(self, teamtalk_instance, msg):
-        """Initializes a ChannelMessage instance.
-
-        Args:
-            teamtalk_instance: An instance of teamtalk.TeamTalkInstance.
-            msg: The message payload.
-        """
-        super().__init__(teamtalk_instance, msg)
-        self.to_id = msg.nChannelID
-        self.channel_id = msg.nChannelID
-        _, self.channel = self.teamtalk_instance.get_channel(self.channel_id)
-
-
-class DirectMessage(Message):
-    """Represents a message sent to a user. This class should not be instantiated directly."""
-
-    def __init__(self, teamtalk_instance, msg):
-        """Initializes a DirectMessage instance.
-
-        Args:
-            teamtalk_instance: An instance of teamtalk.TeamTalkInstance.
-            msg: The message payload.
-        """
-        super().__init__(teamtalk_instance, msg)
-        self.to_id = msg.nToUserID
-        # if the id is still 0, then it's a private message to the bot
-        if self.to_id == 0:
-            self.to_id = teamtalk_instance.getMyUserID()
-
-
-class BroadcastMessage(Message):
-    """Represents a message sent to a server. This class should not be instantiated directly."""
-
-    def __init__(self, teamtalk_instance, msg):
-        """Initializes a BroadcastMessage instance.
-
-        Args:
-            teamtalk_instance: An instance of teamtalk.TeamTalkInstance.
-            msg: The message payload.
-        """
-        super().__init__(teamtalk_instance, msg)
-
-
-class CustomMessage(Message):
-    """Represents a custom message. This class should not be instantiated directly."""
-
-    def __init__(self, teamtalk_instance, msg):
-        """Initializes a CustomMessage instance.
-
-        Args:
-            teamtalk_instance: An instance of teamtalk.TeamTalkInstance.
-            msg: The message payload.
-        """
-        super().__init__(teamtalk_instance, msg)
+"""This module contains the Message class and its subclasses."""
+
+
+from .implementation.TeamTalkPy import TeamTalk5 as sdk
+
+
+class Message:
+    """Represents a TeamTalk5 message. This class should not be instantiated directly."""
+
+    def __init__(self, teamtalk_instance, msg):
+        """Initializes a Message instance.
+
+        Args:
+            teamtalk_instance: An instance of teamtalk.TeamTalkInstance.
+            msg: The message.
+        """
+        self.teamtalk_instance = teamtalk_instance
+        self.type = msg.nMsgType
+        self.from_id = msg.nFromUserID
+        self.to_id = msg.nToUserID
+        self.content = msg.szMessage
+        # if content is a byte array, decode it
+        if isinstance(self.content, bytes):
+            self.content = self.content.decode("utf-8")
+        self.user = self.teamtalk_instance.get_user(self.from_id)
+
+    def reply(self, content, **kwargs):
+        """Replies to the message.
+
+        The reply will be sent to the place where the message was sent from.
+        Meaning that if the message was sent to a channel, the reply will be sent to the channel.
+        If the message was sent to a user, the reply will be sent to the user.
+        And if the message was a broadcast message, the reply will be sent to the server as a broadcast.
+
+        Args:
+            content: The content of the message.
+            **kwargs: Keyword arguments. See teamtalk.TeamTalkInstance.send_message for more information.
+
+        Returns:
+            The message ID of the reply.
+
+        Raises:
+            PermissionError: If the sender doesn't have permission to send the message.
+        """
+        msg = sdk.TextMessage()
+        msg.nMsgType = self.type
+        msg.nFromUserID = self.teamtalk_instance.super.getMyUserID()
+        msg.szFromUsername = self.teamtalk_instance.super.getMyUserAccount().szUsername
+        # if self is channel message, then reply to channel
+        if isinstance(self, ChannelMessage):
+            if self.teamtalk_instance.super.getMyChannelID() != self.to_id:
+                if not self.teamtalk_instance.is_admin():
+                    raise PermissionError("You don't have permission to send messages across channels.")
+            msg.nChannelID = self.to_id
+        if isinstance(self, BroadcastMessage):
+            # if we aren ot admin we cant do this
+            if not self.teamtalk_instance.is_admin():
+                raise PermissionError("You don't have permission to send broadcast messages.")
+            msg.nToUserID = 0
+            msg.nChannelID = 0
+        else:
+            msg.nToUserID = self.from_id
+        msg.szMessage = sdk.ttstr(content)
+        msg.bMore = False
+        return self.teamtalk_instance._send_message(msg, **kwargs)
+
+    def is_me(self) -> bool:
+        """Checks if the message was sent by the bot.
+
+        Returns:
+            True if the message was sent by the bot, False otherwise.
+        """
+        return self.from_id == self.teamtalk_instance.super.getMyUserID()
+
+    def __str__(self) -> str:
+        """Returns a string representation of the message.
+
+        Returns:
+            A string representation of the message.
+        """
+        return f"teamtalk.{type(self).__name__}(from_id={self.from_id}, to_id={self.to_id}, content={self.content})"
+
+
+# make a channel message subclass
+class ChannelMessage(Message):
+    """Represents a message sent to a channel. This class should not be instantiated directly."""
+
+    def __init__(self, teamtalk_instance, msg):
+        """Initializes a ChannelMessage instance.
+
+        Args:
+            teamtalk_instance: An instance of teamtalk.TeamTalkInstance.
+            msg: The message payload.
+        """
+        super().__init__(teamtalk_instance, msg)
+        self.to_id = msg.nChannelID
+        self.channel_id = msg.nChannelID
+        _, self.channel = self.teamtalk_instance.get_channel(self.channel_id)
+
+
+class DirectMessage(Message):
+    """Represents a message sent to a user. This class should not be instantiated directly."""
+
+    def __init__(self, teamtalk_instance, msg):
+        """Initializes a DirectMessage instance.
+
+        Args:
+            teamtalk_instance: An instance of teamtalk.TeamTalkInstance.
+            msg: The message payload.
+        """
+        super().__init__(teamtalk_instance, msg)
+        self.to_id = msg.nToUserID
+        # if the id is still 0, then it's a private message to the bot
+        if self.to_id == 0:
+            self.to_id = teamtalk_instance.getMyUserID()
+
+
+class BroadcastMessage(Message):
+    """Represents a message sent to a server. This class should not be instantiated directly."""
+
+    def __init__(self, teamtalk_instance, msg):
+        """Initializes a BroadcastMessage instance.
+
+        Args:
+            teamtalk_instance: An instance of teamtalk.TeamTalkInstance.
+            msg: The message payload.
+        """
+        super().__init__(teamtalk_instance, msg)
+
+
+class CustomMessage(Message):
+    """Represents a custom message. This class should not be instantiated directly."""
+
+    def __init__(self, teamtalk_instance, msg):
+        """Initializes a CustomMessage instance.
+
+        Args:
+            teamtalk_instance: An instance of teamtalk.TeamTalkInstance.
+            msg: The message payload.
+        """
+        super().__init__(teamtalk_instance, msg)
```

### Comparing `teamtalk_py-1.1.0/teamtalk/server.py` & `teamtalk_py-1.1.1/teamtalk/server.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,263 +1,263 @@
-"""Provides the Server class for interacting with a TeamTalk5 server."""
-
-import ctypes
-from typing import Union
-
-from ._utils import _get_tt_obj_attribute, _set_tt_obj_attribute
-from .permission import Permission
-from .channel import Channel as TeamTalkChannel
-from .exceptions import PermissionError
-from .implementation.TeamTalkPy import TeamTalk5 as sdk
-from .user import User as TeamTalkUser
-
-
-class Server:
-    """Represents a TeamTalk5 server.
-
-    Attributes:
-        teamtalk_instance: An instance of teamtalk.TeamTalkInstance.
-        info: The server information.
-    """
-
-    def __init__(self, teamtalk_instance, server_info):
-        """Initializes a Server instance.
-
-        Args:
-            teamtalk_instance: An instance of teamtalk.TeamTalkInstance.
-            server_info: The server information.
-        """
-        self.teamtalk_instance = teamtalk_instance
-        self.info = server_info
-
-    def send_message(self, content: str, **kwargs):
-        """Sends a message to all users on the server, using a broadcast message.
-
-        Args:
-            content: The content of the message.
-            **kwargs: Keyword arguments. See teamtalk.TeamTalkInstance.send_message for more information.
-
-        Returns:
-            The result of the doTextMessage call.
-
-        Raises:
-            PermissionError: If the user is not an admin.
-        """
-        if not self.teamtalk_instance.is_admin():
-            raise PermissionError("You must be an admin to send messages to the server")
-        msg = sdk.TextMessage()
-        msg.nMsgType = sdk.TextMsgType.MSGTYPE_BROADCAST
-        msg.nFromUserID = self.teamtalk_instance.getMyUserID()
-        msg.szFromUsername = self.teamtalk_instance.getMyUserAccount().szUsername
-        msg.nToUserID = 0
-        msg.szMessage = content
-        msg.bMore = False
-        # get a pointer to our message
-        return self.teamtalk_instance._send_message(msg, **kwargs)
-
-    def ping(self) -> bool:
-        """Pings the server.
-
-        Returns:
-            True if the ping is successful, False otherwise.
-        """
-        return self.teamtalk_instance.super._DoPing(self.info.nServerPort)
-
-    def get_users(self) -> list:
-        """Gets a list of users on the server.
-
-        Returns:
-            A list of teamtalk.User instances representing the users on the server.
-        """
-        users = self.teamtalk_instance.super.getServerUsers()
-        return [TeamTalkUser(self.teamtalk_instance, user) for user in users]
-
-    def get_channels(self) -> list:
-        """Gets a list of channels on the server.
-
-        Returns:
-            A list of teamtalk.Channel instances representing the channels on the server.
-        """
-        channels = self.teamtalk_instance.super.getServerChannels()
-        return [TeamTalkChannel(self.teamtalk_instance, channel) for channel in channels]
-
-    def get_channel(self, channel_id):
-        """Gets the channel with the specified ID.
-
-        Args:
-            channel_id: The ID of the channel.
-
-        Returns:
-            The teamtalk.Channel instance representing the channel with the specified ID.
-        """
-        channel = self.teamtalk_instance.super.getChannel(channel_id)
-        return TeamTalkChannel(self.teamtalk_instance, channel)
-
-    def get_user(self, user_id):
-        """Gets the user with the specified ID.
-
-        Args:
-            user_id: The ID of the user.
-
-        Returns:
-            The teamtalk.User instance representing the user with the specified ID.
-        """
-        user = self.teamtalk_instance.super.getUser(user_id)
-        return TeamTalkUser(self.teamtalk_instance, user)
-
-    def move_user(self, user: Union[TeamTalkUser, int], channel: Union[TeamTalkChannel, int]):
-        """Moves the specified user to the specified channel.
-
-        Args:
-            user: The user to move.
-            channel: The channel to move the user to.
-
-        Raises:
-            PermissionError: If the user is not an admin.
-        """
-        if not self.teamtalk_instance.is_admin():
-            raise PermissionError("You must be an admin to move users")
-        if isinstance(user, TeamTalkUser):
-            user = user.id
-        if isinstance(channel, TeamTalkChannel):
-            channel = channel.id
-        self.teamtalk_instance.move_user(user, channel)
-
-    def kick(self, user: Union[TeamTalkUser, int]):
-        """Kicks the specified user from the specified channel.
-
-        Args:
-            user: The user to kick.
-
-        Raises:
-            PermissionError: If the user is not an admin.
-        """
-        self.teamtalk_instance.kick_user(user, 0)
-
-    def ban(self, user: Union[TeamTalkUser, int]):
-        """Bans the specified user from the specified channel.
-
-        Args:
-            user: The user to ban.
-
-        Raises:
-            PermissionError: If the user is not an admin.
-        """
-        self.teamtalk_instance.ban_user(user, 0)
-
-    def unban(self, user: Union[TeamTalkUser, int]):
-        """Unbans the specified user from the specified channel.
-
-        Args:
-            user: The user to unban.
-
-        Raises:
-            PermissionError: If the user is not an admin.
-        """
-        self.teamtalk_instance.unban_user(user, 0)
-
-    def get_properties(self) -> "ServerProperties":
-        """Gets the properties of the server.
-
-        Returns:
-            A teamtalk.ServerProperties instance representing the properties of the server.
-        """
-        props = self.teamtalk_instance.super.getServerProperties()
-        return ServerProperties(self.teamtalk_instance, props)
-
-    def update_properties(self, properties: "ServerProperties"):
-        """Updates the properties of the server.
-
-        Args:
-            properties: The updated properties. See teamtalk.ServerProperties for more information.
-
-        Raises:
-            PermissionError: If the bot does not have the permission to update the properties.
-        """
-        if not self.teamtalk_instance.has_permission(Permission.UPDATE_SERVERPROPERTIES):
-            raise PermissionError("The bot does not have permission to update the server properties")
-        # get the underlying properties object
-        properties = properties.properties
-        sdk._DoUpdateServer(self.teamtalk_instance._tt, ctypes.byref(properties))
-
-    def __getattr__(self, name: str):
-        """Try to get the specified attribute on server.
-
-        Args:
-            name: The name of the attribute.
-
-        Returns:
-            The value of the specified attribute.
-
-        Raises:
-            AttributeError: If the specified attribute is not found. This is the default behavior. # noqa
-        """
-        if name in dir(self):
-            return self.__dict__[name]
-        else:
-            return _get_tt_obj_attribute(self._user, name)
-
-
-class ServerProperties(object):
-    """Represents the properties of a server.
-
-    This class should not be instantiated directly. Instead, use the teamtalk.Server.get_properties() method. # noqa
-
-    Example:
-        >>> server = teamtalk server
-        >>> properties = server.get_properties()
-        >>> properties.max_users
-        1000
-        >>> properties.max_users = 500
-        >>> server.update_properties(properties)
-        >>> properties = server.get_properties()
-        >>> properties.max_users
-        500
-    """
-
-    def __init__(self, teamtalk_instance, properties):
-        """Initializes a new instance of the ServerProperties class.
-
-        Args:
-            teamtalk_instance: The teamtalk.TeamTalk instance.
-            properties: The underlying properties object.
-        """
-        self.teamtalk_instance = teamtalk_instance
-        self.properties = properties
-
-    def __getattr__(self, name: str):
-        """Try to get the specified attribute on server.
-
-        Args:
-            name: The name of the attribute.
-
-        Returns:
-            The value of the specified attribute.
-
-        Raises:
-            AttributeError: If the specified attribute is not found. This is the default behavior. # noqa
-        """
-        if name in dir(self):
-            return self.__dict__[name]
-        else:
-            return _get_tt_obj_attribute(self.properties, name)
-
-    def __setattr__(self, name: str, value):
-        """Try to set the specified attribute on properties.
-
-        Args:
-            name: The name of the attribute.
-            value: The value to set the attribute to.
-
-            Raises:
-                AttributeError: If the specified attribute is not found.
-        """
-        if name in dir(self):
-            self.__dict__[name] = value
-        else:
-            # if name is either teamtalk_instance or properties, just set it on self
-            if name in ["teamtalk_instance", "properties"]:
-                self.__dict__[name] = value
-            else:
-                _get_tt_obj_attribute(self.properties, name)
-                # if we have gotten here, we can set the attribute
-                _set_tt_obj_attribute(self.properties, name, value)
+"""Provides the Server class for interacting with a TeamTalk5 server."""
+
+import ctypes
+from typing import Union
+
+from ._utils import _get_tt_obj_attribute, _set_tt_obj_attribute
+from .permission import Permission
+from .channel import Channel as TeamTalkChannel
+from .exceptions import PermissionError
+from .implementation.TeamTalkPy import TeamTalk5 as sdk
+from .user import User as TeamTalkUser
+
+
+class Server:
+    """Represents a TeamTalk5 server.
+
+    Attributes:
+        teamtalk_instance: An instance of teamtalk.TeamTalkInstance.
+        info: The server information.
+    """
+
+    def __init__(self, teamtalk_instance, server_info):
+        """Initializes a Server instance.
+
+        Args:
+            teamtalk_instance: An instance of teamtalk.TeamTalkInstance.
+            server_info: The server information.
+        """
+        self.teamtalk_instance = teamtalk_instance
+        self.info = server_info
+
+    def send_message(self, content: str, **kwargs):
+        """Sends a message to all users on the server, using a broadcast message.
+
+        Args:
+            content: The content of the message.
+            **kwargs: Keyword arguments. See teamtalk.TeamTalkInstance.send_message for more information.
+
+        Returns:
+            The result of the doTextMessage call.
+
+        Raises:
+            PermissionError: If the user is not an admin.
+        """
+        if not self.teamtalk_instance.is_admin():
+            raise PermissionError("You must be an admin to send messages to the server")
+        msg = sdk.TextMessage()
+        msg.nMsgType = sdk.TextMsgType.MSGTYPE_BROADCAST
+        msg.nFromUserID = self.teamtalk_instance.getMyUserID()
+        msg.szFromUsername = self.teamtalk_instance.getMyUserAccount().szUsername
+        msg.nToUserID = 0
+        msg.szMessage = content
+        msg.bMore = False
+        # get a pointer to our message
+        return self.teamtalk_instance._send_message(msg, **kwargs)
+
+    def ping(self) -> bool:
+        """Pings the server.
+
+        Returns:
+            True if the ping is successful, False otherwise.
+        """
+        return self.teamtalk_instance.super._DoPing(self.info.nServerPort)
+
+    def get_users(self) -> list:
+        """Gets a list of users on the server.
+
+        Returns:
+            A list of teamtalk.User instances representing the users on the server.
+        """
+        users = self.teamtalk_instance.super.getServerUsers()
+        return [TeamTalkUser(self.teamtalk_instance, user) for user in users]
+
+    def get_channels(self) -> list:
+        """Gets a list of channels on the server.
+
+        Returns:
+            A list of teamtalk.Channel instances representing the channels on the server.
+        """
+        channels = self.teamtalk_instance.super.getServerChannels()
+        return [TeamTalkChannel(self.teamtalk_instance, channel) for channel in channels]
+
+    def get_channel(self, channel_id):
+        """Gets the channel with the specified ID.
+
+        Args:
+            channel_id: The ID of the channel.
+
+        Returns:
+            The teamtalk.Channel instance representing the channel with the specified ID.
+        """
+        channel = self.teamtalk_instance.super.getChannel(channel_id)
+        return TeamTalkChannel(self.teamtalk_instance, channel)
+
+    def get_user(self, user_id):
+        """Gets the user with the specified ID.
+
+        Args:
+            user_id: The ID of the user.
+
+        Returns:
+            The teamtalk.User instance representing the user with the specified ID.
+        """
+        user = self.teamtalk_instance.super.getUser(user_id)
+        return TeamTalkUser(self.teamtalk_instance, user)
+
+    def move_user(self, user: Union[TeamTalkUser, int], channel: Union[TeamTalkChannel, int]):
+        """Moves the specified user to the specified channel.
+
+        Args:
+            user: The user to move.
+            channel: The channel to move the user to.
+
+        Raises:
+            PermissionError: If the user is not an admin.
+        """
+        if not self.teamtalk_instance.is_admin():
+            raise PermissionError("You must be an admin to move users")
+        if isinstance(user, TeamTalkUser):
+            user = user.id
+        if isinstance(channel, TeamTalkChannel):
+            channel = channel.id
+        self.teamtalk_instance.move_user(user, channel)
+
+    def kick(self, user: Union[TeamTalkUser, int]):
+        """Kicks the specified user from the specified channel.
+
+        Args:
+            user: The user to kick.
+
+        Raises:
+            PermissionError: If the user is not an admin.
+        """
+        self.teamtalk_instance.kick_user(user, 0)
+
+    def ban(self, user: Union[TeamTalkUser, int]):
+        """Bans the specified user from the specified channel.
+
+        Args:
+            user: The user to ban.
+
+        Raises:
+            PermissionError: If the user is not an admin.
+        """
+        self.teamtalk_instance.ban_user(user, 0)
+
+    def unban(self, user: Union[TeamTalkUser, int]):
+        """Unbans the specified user from the specified channel.
+
+        Args:
+            user: The user to unban.
+
+        Raises:
+            PermissionError: If the user is not an admin.
+        """
+        self.teamtalk_instance.unban_user(user, 0)
+
+    def get_properties(self) -> "ServerProperties":
+        """Gets the properties of the server.
+
+        Returns:
+            A teamtalk.ServerProperties instance representing the properties of the server.
+        """
+        props = self.teamtalk_instance.super.getServerProperties()
+        return ServerProperties(self.teamtalk_instance, props)
+
+    def update_properties(self, properties: "ServerProperties"):
+        """Updates the properties of the server.
+
+        Args:
+            properties: The updated properties. See teamtalk.ServerProperties for more information.
+
+        Raises:
+            PermissionError: If the bot does not have the permission to update the properties.
+        """
+        if not self.teamtalk_instance.has_permission(Permission.UPDATE_SERVERPROPERTIES):
+            raise PermissionError("The bot does not have permission to update the server properties")
+        # get the underlying properties object
+        properties = properties.properties
+        sdk._DoUpdateServer(self.teamtalk_instance._tt, ctypes.byref(properties))
+
+    def __getattr__(self, name: str):
+        """Try to get the specified attribute on server.
+
+        Args:
+            name: The name of the attribute.
+
+        Returns:
+            The value of the specified attribute.
+
+        Raises:
+            AttributeError: If the specified attribute is not found. This is the default behavior. # noqa
+        """
+        if name in dir(self):
+            return self.__dict__[name]
+        else:
+            return _get_tt_obj_attribute(self._user, name)
+
+
+class ServerProperties(object):
+    """Represents the properties of a server.
+
+    This class should not be instantiated directly. Instead, use the teamtalk.Server.get_properties() method. # noqa
+
+    Example:
+        >>> server = teamtalk server
+        >>> properties = server.get_properties()
+        >>> properties.max_users
+        1000
+        >>> properties.max_users = 500
+        >>> server.update_properties(properties)
+        >>> properties = server.get_properties()
+        >>> properties.max_users
+        500
+    """
+
+    def __init__(self, teamtalk_instance, properties):
+        """Initializes a new instance of the ServerProperties class.
+
+        Args:
+            teamtalk_instance: The teamtalk.TeamTalk instance.
+            properties: The underlying properties object.
+        """
+        self.teamtalk_instance = teamtalk_instance
+        self.properties = properties
+
+    def __getattr__(self, name: str):
+        """Try to get the specified attribute on server.
+
+        Args:
+            name: The name of the attribute.
+
+        Returns:
+            The value of the specified attribute.
+
+        Raises:
+            AttributeError: If the specified attribute is not found. This is the default behavior. # noqa
+        """
+        if name in dir(self):
+            return self.__dict__[name]
+        else:
+            return _get_tt_obj_attribute(self.properties, name)
+
+    def __setattr__(self, name: str, value):
+        """Try to set the specified attribute on properties.
+
+        Args:
+            name: The name of the attribute.
+            value: The value to set the attribute to.
+
+            Raises:
+                AttributeError: If the specified attribute is not found.
+        """
+        if name in dir(self):
+            self.__dict__[name] = value
+        else:
+            # if name is either teamtalk_instance or properties, just set it on self
+            if name in ["teamtalk_instance", "properties"]:
+                self.__dict__[name] = value
+            else:
+                _get_tt_obj_attribute(self.properties, name)
+                # if we have gotten here, we can set the attribute
+                _set_tt_obj_attribute(self.properties, name, value)
```

### Comparing `teamtalk_py-1.1.0/teamtalk/streamer.py` & `teamtalk_py-1.1.1/teamtalk/streamer.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,198 +1,198 @@
-"""A module containing the Streamer class.
-
-This module contains the Streamer class, which is used to stream audio data to a TeamTalk channel.
-
-.. warning::
-   To use other files than .wav files, you need to have ffmpeg installed on your system.
-
-Example:
-    >>> import teamtalk
-    >>> # asuming we have a bot in the variable bot
-    >>> @bot.event
-    >>> async def on_message(message):
-    >>>     if message.content.lower() == "play":
-    >>>         stream = teamtalk.Streamer(message.channel)
-    >>>         stream.stream_file("test.wav")
-
-
-It's also possible to stream audio from an arbitrary data stream, such as a microphone or a url stream.
-To do this, you need to set the correct sample rate and number of channels on initialization,
-and then feed the data to the streamer as it becomes available.
-The data needs to be in 16 bit PCM format (pcm_s16le).
-
-Example:
-    >>> import teamtalk
-    >>> # asuming we have a bot in the variable bot
-    >>> @bot.event
-    >>> async def on_message(message):
-    >>>     if message.content.lower() == "play":
-    >>>         stream = teamtalk.Stream(message.channel, sample_rate=48000, channels=2)
-    >>>         # we could get the data from any source, so let's assume it's coming from a live microphone and/or url stream
-    >>>         data_stream = # connect to microphone and/or url stream
-    >>>         while True:
-    >>>             # get the data from the stream
-    >>>             data = data_stream.read(streamer.block_size*16) # we are reading 16 chunks at a time to combat buffering
-    >>>             if data == 0:
-    >>>                 break
-    >>>             # add the data to the streamer
-    >>>             stream.feed(data)
-    >>>         # close the connection to our microphone and/or url stream
-"""
-
-import os
-import ctypes
-import threading
-import random
-import subprocess
-import tempfile
-
-import PyWave
-
-from .implementation.TeamTalkPy import TeamTalk5 as sdk
-
-from .channel import Channel as TeamTalkChannel
-
-
-class Streamer:
-    """A class representing a streamer for audio data to a TeamTalk channel."""
-
-    def __init__(self, channel: TeamTalkChannel, sample_rate: int = 48000, channels: int = 2, block_size: int = 4 * 1024):
-        """Initializes a new instance of the TeamTalkStreamer class.
-
-        Args:
-            channel (TeamTalkChannel): The TeamTalk channel to which the streamer streams the audio data.
-            sample_rate (int, optional): The sample rate of the audio data. Defaults to 48000.
-            channels (int, optional): The number of channels in the audio data. Defaults to 2.
-            block_size (int, optional): The block size of the audio data. Defaults to 4 * 1024 (4kb)
-        """
-        self.channel = channel
-        self.sample_rate = sample_rate
-        self.channels = channels
-        self.block_size = block_size
-        # the list of blocks that will be streamed
-        self.blocks = []
-        self.current_data = b""
-        # streamer id
-        self.stream_id = random.randint(6000, 6999)
-        # start the stream function on another thread
-        self.running = True
-        threading.Thread(target=self._do_stream).start()
-
-    def __del__(self):
-        """Shuts down the streamer by adding a null-block to the blocks list and waiting for the blocks list to be empty."""
-        # add a block with 0 length to the blocks list to stop the streamer
-        self.blocks.append(b"")
-        # wait for the blocks list to be empty
-        while len(self.blocks) > 0:
-            pass
-        # stop the streamer
-        self.running = False
-
-    def stream_file(self, filepath: str, _tried: int = 0) -> int:
-        """Streams a file to the channel.
-
-        Args:
-            filepath (str): The path to the file to stream.
-
-        Returns:
-            int: The stream id of the stream.
-
-        Raises:
-            FileNotFoundError: If the file could not be found.
-            RuntimeError: If the file could not be opened as a wav file or if the file could not be converted to a wav file.
-        """
-        if not os.path.isfile(filepath):
-            raise FileNotFoundError(f"Could not find file {filepath}")
-        try:
-            wf = PyWave.open(filepath, "r")
-        except PyWave.PyWaveError:
-            if _tried < 3:
-                new_filepath = self._convert_to_wav(filepath)
-                return self.stream_file(new_filepath, _tried=_tried + 1)
-            else:
-                raise RuntimeError(f"Could not open file {filepath}.")
-            # not normally done, but since we have a file, we don't need to asume
-        self.sample_rate = wf.frequency
-        self.channels = wf.channels
-        while True:
-            block = wf.read(self.block_size * 16)
-            if len(block) == 0:
-                break
-            self.feed(block)
-        wf.close()
-        return self.stream_id
-
-    def feed(self, data: bytes) -> int:
-        """Feeds data to the streamer.
-
-        Args:
-            data (bytes): The data to feed to the streamer.
-
-        Returns:
-            int: The stream id of the stream.
-        """
-        # first add the data to the current data
-        self.current_data += data
-        if len(self.current_data) >= self.block_size:
-            # if it is, then split it into 4*1024 byte chunks
-            chunks = [self.current_data[i : i + self.block_size] for i in range(0, len(self.current_data), self.block_size)]
-            # then add all but the last chunk to the blocks list
-            self.blocks.extend(chunks[:-1])
-            # then set the current data to the last chunk
-            self.current_data = chunks[-1]
-        else:
-            # if it is not, then just add the block to the blocks list
-            self.blocks.append(data)
-        return self.stream_id
-
-    def _do_stream(self):
-        while self.running:
-            # if there are blocks to stream
-            if len(self.blocks) > 0:
-                # get the first block
-                block = self.blocks[0]
-                # create a new audio block
-                audio_block = sdk.AudioBlock()
-                audio_block.nStreamID = self.stream_id
-                audio_block.nSampleRate = self.sample_rate
-                audio_block.nChannels = self.channels
-                audio_block.nSamples = len(block) // 4
-                audio_block.lpRawAudio = ctypes.cast((ctypes.c_char * len(block)).from_buffer_copy(block), ctypes.c_void_p)
-                audio_block.uStreamTypes = sdk.StreamType.STREAMTYPE_VOICE
-                # send the audio block
-                result = 0
-                while result == 0:
-                    result = sdk._InsertAudioBlock(self.channel.teamtalk._tt, audio_block)
-                # remove the block from the blocks list
-                self.blocks = self.blocks[1:]
-
-    def _convert_to_wav(self, filepath):
-        if not self._has_ffmpeg():
-            raise RuntimeError("Could not convert file to wav. ffmpeg is not installed.")
-        # get a path to a temp dir we can write to
-        temp_dir = tempfile.gettempdir()
-        # make sure it exists
-        if not os.path.isdir(temp_dir):
-            os.makedirs(temp_dir)
-        # get a path to a randomly named temp file
-        temp_file = os.path.join(temp_dir, next(tempfile._get_candidate_names()))
-        # add a wav extension to the temp file
-        temp_file = f"{temp_file}.wav"
-        cmd = ["ffmpeg", "-i", filepath, "-acodec", "pcm_s16le", temp_file]
-        # call our command, prinitng stdout and stderr if we fail
-        result = subprocess.run(cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
-        if result.returncode != 0:
-            print(result.stdout)
-            print(result.stderr)
-            raise RuntimeError(f"Could not convert file {filepath} to wav.")
-        return temp_file
-
-    def _has_ffmpeg(self):
-        # check if ffmpeg is installed
-        try:
-            result = subprocess.run(["ffmpeg", "-version"], stdout=subprocess.PIPE, stderr=subprocess.PIPE)
-            if result.returncode != 0:
-                return False
-        except FileNotFoundError:
-            return False
-        return True
+"""A module containing the Streamer class.
+
+This module contains the Streamer class, which is used to stream audio data to a TeamTalk channel.
+
+.. warning::
+   To use other files than .wav files, you need to have ffmpeg installed on your system.
+
+Example:
+    >>> import teamtalk
+    >>> # asuming we have a bot in the variable bot
+    >>> @bot.event
+    >>> async def on_message(message):
+    >>>     if message.content.lower() == "play":
+    >>>         stream = teamtalk.Streamer(message.channel)
+    >>>         stream.stream_file("test.wav")
+
+
+It's also possible to stream audio from an arbitrary data stream, such as a microphone or a url stream.
+To do this, you need to set the correct sample rate and number of channels on initialization,
+and then feed the data to the streamer as it becomes available.
+The data needs to be in 16 bit PCM format (pcm_s16le).
+
+Example:
+    >>> import teamtalk
+    >>> # asuming we have a bot in the variable bot
+    >>> @bot.event
+    >>> async def on_message(message):
+    >>>     if message.content.lower() == "play":
+    >>>         stream = teamtalk.Stream(message.channel, sample_rate=48000, channels=2)
+    >>>         # we could get the data from any source, so let's assume it's coming from a live microphone and/or url stream
+    >>>         data_stream = # connect to microphone and/or url stream
+    >>>         while True:
+    >>>             # get the data from the stream
+    >>>             data = data_stream.read(streamer.block_size*16) # we are reading 16 chunks at a time to combat buffering
+    >>>             if data == 0:
+    >>>                 break
+    >>>             # add the data to the streamer
+    >>>             stream.feed(data)
+    >>>         # close the connection to our microphone and/or url stream
+"""
+
+import os
+import ctypes
+import threading
+import random
+import subprocess
+import tempfile
+
+import PyWave
+
+from .implementation.TeamTalkPy import TeamTalk5 as sdk
+
+from .channel import Channel as TeamTalkChannel
+
+
+class Streamer:
+    """A class representing a streamer for audio data to a TeamTalk channel."""
+
+    def __init__(self, channel: TeamTalkChannel, sample_rate: int = 48000, channels: int = 2, block_size: int = 4 * 1024):
+        """Initializes a new instance of the TeamTalkStreamer class.
+
+        Args:
+            channel (TeamTalkChannel): The TeamTalk channel to which the streamer streams the audio data.
+            sample_rate (int, optional): The sample rate of the audio data. Defaults to 48000.
+            channels (int, optional): The number of channels in the audio data. Defaults to 2.
+            block_size (int, optional): The block size of the audio data. Defaults to 4 * 1024 (4kb)
+        """
+        self.channel = channel
+        self.sample_rate = sample_rate
+        self.channels = channels
+        self.block_size = block_size
+        # the list of blocks that will be streamed
+        self.blocks = []
+        self.current_data = b""
+        # streamer id
+        self.stream_id = random.randint(6000, 6999)
+        # start the stream function on another thread
+        self.running = True
+        threading.Thread(target=self._do_stream).start()
+
+    def __del__(self):
+        """Shuts down the streamer by adding a null-block to the blocks list and waiting for the blocks list to be empty."""
+        # add a block with 0 length to the blocks list to stop the streamer
+        self.blocks.append(b"")
+        # wait for the blocks list to be empty
+        while len(self.blocks) > 0:
+            pass
+        # stop the streamer
+        self.running = False
+
+    def stream_file(self, filepath: str, _tried: int = 0) -> int:
+        """Streams a file to the channel.
+
+        Args:
+            filepath (str): The path to the file to stream.
+
+        Returns:
+            int: The stream id of the stream.
+
+        Raises:
+            FileNotFoundError: If the file could not be found.
+            RuntimeError: If the file could not be opened as a wav file or if the file could not be converted to a wav file.
+        """
+        if not os.path.isfile(filepath):
+            raise FileNotFoundError(f"Could not find file {filepath}")
+        try:
+            wf = PyWave.open(filepath, "r")
+        except PyWave.PyWaveError:
+            if _tried < 3:
+                new_filepath = self._convert_to_wav(filepath)
+                return self.stream_file(new_filepath, _tried=_tried + 1)
+            else:
+                raise RuntimeError(f"Could not open file {filepath}.")
+            # not normally done, but since we have a file, we don't need to asume
+        self.sample_rate = wf.frequency
+        self.channels = wf.channels
+        while True:
+            block = wf.read(self.block_size * 16)
+            if len(block) == 0:
+                break
+            self.feed(block)
+        wf.close()
+        return self.stream_id
+
+    def feed(self, data: bytes) -> int:
+        """Feeds data to the streamer.
+
+        Args:
+            data (bytes): The data to feed to the streamer.
+
+        Returns:
+            int: The stream id of the stream.
+        """
+        # first add the data to the current data
+        self.current_data += data
+        if len(self.current_data) >= self.block_size:
+            # if it is, then split it into 4*1024 byte chunks
+            chunks = [self.current_data[i : i + self.block_size] for i in range(0, len(self.current_data), self.block_size)]
+            # then add all but the last chunk to the blocks list
+            self.blocks.extend(chunks[:-1])
+            # then set the current data to the last chunk
+            self.current_data = chunks[-1]
+        else:
+            # if it is not, then just add the block to the blocks list
+            self.blocks.append(data)
+        return self.stream_id
+
+    def _do_stream(self):
+        while self.running:
+            # if there are blocks to stream
+            if len(self.blocks) > 0:
+                # get the first block
+                block = self.blocks[0]
+                # create a new audio block
+                audio_block = sdk.AudioBlock()
+                audio_block.nStreamID = self.stream_id
+                audio_block.nSampleRate = self.sample_rate
+                audio_block.nChannels = self.channels
+                audio_block.nSamples = len(block) // 4
+                audio_block.lpRawAudio = ctypes.cast((ctypes.c_char * len(block)).from_buffer_copy(block), ctypes.c_void_p)
+                audio_block.uStreamTypes = sdk.StreamType.STREAMTYPE_VOICE
+                # send the audio block
+                result = 0
+                while result == 0:
+                    result = sdk._InsertAudioBlock(self.channel.teamtalk._tt, audio_block)
+                # remove the block from the blocks list
+                self.blocks = self.blocks[1:]
+
+    def _convert_to_wav(self, filepath):
+        if not self._has_ffmpeg():
+            raise RuntimeError("Could not convert file to wav. ffmpeg is not installed.")
+        # get a path to a temp dir we can write to
+        temp_dir = tempfile.gettempdir()
+        # make sure it exists
+        if not os.path.isdir(temp_dir):
+            os.makedirs(temp_dir)
+        # get a path to a randomly named temp file
+        temp_file = os.path.join(temp_dir, next(tempfile._get_candidate_names()))
+        # add a wav extension to the temp file
+        temp_file = f"{temp_file}.wav"
+        cmd = ["ffmpeg", "-i", filepath, "-acodec", "pcm_s16le", temp_file]
+        # call our command, prinitng stdout and stderr if we fail
+        result = subprocess.run(cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+        if result.returncode != 0:
+            print(result.stdout)
+            print(result.stderr)
+            raise RuntimeError(f"Could not convert file {filepath} to wav.")
+        return temp_file
+
+    def _has_ffmpeg(self):
+        # check if ffmpeg is installed
+        try:
+            result = subprocess.run(["ffmpeg", "-version"], stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+            if result.returncode != 0:
+                return False
+        except FileNotFoundError:
+            return False
+        return True
```

### Comparing `teamtalk_py-1.1.0/teamtalk/tt_file.py` & `teamtalk_py-1.1.1/teamtalk/tt_file.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-"""Teamtalk file object."""
-
-from ._utils import _get_tt_obj_attribute
-
-
-class RemoteFile:
-    """Represents a file on a TeamTalk server. Should not be instantiated directly."""
-
-    def __init__(self, teamtalk_instance, payload):
-        """Initializes the RemoteFile instance.
-
-        Args:
-            teamtalk_instance: The teamtalk.TeamTalkInstance instance.
-            payload: An instance of sdk.RemoteFile.
-        """
-        self.teamtalk = teamtalk_instance
-        self.channel = lambda self: self.teamtalk.get_channel(payload.nChannelID)
-        self.server = lambda self: self.teamtalk.server
-        self.payload = payload
-
-    def __str__(self) -> str:
-        """Returns a string representation of the RemoteFile instance.
-
-        Returns:
-            A string representation of the RemoteFile instance.
-        """
-        return f"Teamtalk.RemoteFile(file_name={self.file_name}, file_id={self.file_id}, file_size={self.file_size}, username={self.username}, upload_time={self.upload_time})"  # noqa: E501
-
-    def __getattr__(self, name: str):
-        """Returns the value of the specified attribute of the remote file.
-
-        Args:
-            name: The name of the attribute.
-
-        Returns:
-            The value of the specified attribute.
-
-        Raises:
-            AttributeError: If the specified attribute is not found. # noqa
-        """
-        if name in dir(self):
-            return self.__dict__[name]
-        else:
-            return _get_tt_obj_attribute(self.payload, name)
+"""Teamtalk file object."""
+
+from ._utils import _get_tt_obj_attribute
+
+
+class RemoteFile:
+    """Represents a file on a TeamTalk server. Should not be instantiated directly."""
+
+    def __init__(self, teamtalk_instance, payload):
+        """Initializes the RemoteFile instance.
+
+        Args:
+            teamtalk_instance: The teamtalk.TeamTalkInstance instance.
+            payload: An instance of sdk.RemoteFile.
+        """
+        self.teamtalk = teamtalk_instance
+        self.channel = lambda self: self.teamtalk.get_channel(payload.nChannelID)
+        self.server = lambda self: self.teamtalk.server
+        self.payload = payload
+
+    def __str__(self) -> str:
+        """Returns a string representation of the RemoteFile instance.
+
+        Returns:
+            A string representation of the RemoteFile instance.
+        """
+        return f"Teamtalk.RemoteFile(file_name={self.file_name}, file_id={self.file_id}, file_size={self.file_size}, username={self.username}, upload_time={self.upload_time})"  # noqa: E501
+
+    def __getattr__(self, name: str):
+        """Returns the value of the specified attribute of the remote file.
+
+        Args:
+            name: The name of the attribute.
+
+        Returns:
+            The value of the specified attribute.
+
+        Raises:
+            AttributeError: If the specified attribute is not found. # noqa
+        """
+        if name in dir(self):
+            return self.__dict__[name]
+        else:
+            return _get_tt_obj_attribute(self.payload, name)
```

### Comparing `teamtalk_py-1.1.0/teamtalk/user.py` & `teamtalk_py-1.1.1/teamtalk/user.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,112 +1,112 @@
-"""This module defines a User class that represents a user on a TeamTalk server."""
-
-# Union type
-from typing import Union
-
-from ._utils import _get_tt_obj_attribute
-from .implementation.TeamTalkPy import TeamTalk5 as sdk
-
-
-class User:
-    """Represents a user on a TeamTalk server.
-
-    Attributes:
-        teamtalk_instance: An instance of TeamTalk.TeamTalkInstance.
-        user: Either a string (username) or an int (user_id) or an instance of sdk.User.
-    """
-
-    def __init__(self, teamtalk_instance, user: Union[str, int, sdk.User]):
-        """Initializes the User instance.
-
-        Args:
-            teamtalk_instance: An instance of TeamTalk5.
-            user: Either a string (username) or an int (user_id) or an instance of sdk.User.
-
-        Raises:
-            TypeError: If the user argument is not of the expected type.
-        """
-        self.teamtalk_instance = teamtalk_instance
-        # if user is str, assume it's a username
-        if isinstance(user, str):
-            self._user = self.teamtalk_instance.super.getUserByUsername(user)
-        # if user is int, assume it's a user_id
-        elif isinstance(user, int):
-            self._user = self.teamtalk_instance.super.getUser(user)
-        # if the user argument is already of type sdk.User, just set it to self._user
-        elif isinstance(user, sdk.User):
-            self._user = user
-        else:
-            raise TypeError(f"user must be either a string or an int. Argument has type: {str(type(user))}.")
-        self.id = self.user_id
-        _, self.channel = self.teamtalk_instance.get_channel(self._user.nChannelID)
-        self.server = self.channel.server
-
-    def send_message(self, content: str, **kwargs) -> int:
-        """Sends a text message to this user.
-
-        Args:
-            content: The content of the message.
-            **kwargs: Keyword arguments. See teamtalk.TeamTalkInstance.send_message for more information.
-
-        Returns:
-            The ID of the message if successful, or a negative value if unsuccessful.
-        """
-        msg = sdk.TextMessage()
-        msg.nMsgType = sdk.TextMsgType.MSGTYPE_USER
-        msg.nFromUserID = self.teamtalk_instance.getMyUserID()
-        msg.szFromUsername = self.teamtalk_instance.getMyUserAccount().szUsername
-        msg.nToUserID = self.user_id
-        msg.szMessage = content
-        msg.bMore = False
-        # get a pointer to our message
-        return self.teamtalk_instance._send_message(msg, **kwargs)
-
-    def move(self, channel) -> bool:
-        """Moves this user to the specified channel.
-
-        Args:
-            channel: The channel to move this user to.
-
-        Returns:
-            True if the user was moved successfully, False otherwise.
-        """
-        return self.server.move_user(self, channel)
-
-    def kick(self, from_server: bool) -> None:
-        """Kicks this user from the server.
-
-        Args:
-            from_server: If True, the user will be kicked from the server. If False, the user will be kicked from the channel. # noqa
-        """
-        channel_id = 0
-        if not from_server:
-            channel_id = self.channel.id
-        self.teamtalk_instance.kick_user(self, channel_id)
-
-    def ban(self, from_server: bool) -> None:
-        """Bans this user from the server.
-
-        Args:
-            from_server: If True, the user will be banned from the server. If False, the user will be banned from the channel. # noqa
-        """
-        channel_id = 0
-        if not from_server:
-            channel_id = self.channel.id
-        self.teamtalk_instance.ban_user(self, channel_id)
-
-    def __getattr__(self, name: str):
-        """Try to get the specified attribute from self._user if it is not found in self.
-
-        Args:
-            name: The name of the attribute.
-
-        Returns:
-            The value of the specified attribute.
-
-        Raises:
-            AttributeError: If the specified attribute is not found. This is the default behavior. # noqa
-        """
-        if name in dir(self):
-            return self.__dict__[name]
-        else:
-            return _get_tt_obj_attribute(self._user, name)
+"""This module defines a User class that represents a user on a TeamTalk server."""
+
+# Union type
+from typing import Union
+
+from ._utils import _get_tt_obj_attribute
+from .implementation.TeamTalkPy import TeamTalk5 as sdk
+
+
+class User:
+    """Represents a user on a TeamTalk server.
+
+    Attributes:
+        teamtalk_instance: An instance of TeamTalk.TeamTalkInstance.
+        user: Either a string (username) or an int (user_id) or an instance of sdk.User.
+    """
+
+    def __init__(self, teamtalk_instance, user: Union[str, int, sdk.User]):
+        """Initializes the User instance.
+
+        Args:
+            teamtalk_instance: An instance of TeamTalk5.
+            user: Either a string (username) or an int (user_id) or an instance of sdk.User.
+
+        Raises:
+            TypeError: If the user argument is not of the expected type.
+        """
+        self.teamtalk_instance = teamtalk_instance
+        # if user is str, assume it's a username
+        if isinstance(user, str):
+            self._user = self.teamtalk_instance.super.getUserByUsername(user)
+        # if user is int, assume it's a user_id
+        elif isinstance(user, int):
+            self._user = self.teamtalk_instance.super.getUser(user)
+        # if the user argument is already of type sdk.User, just set it to self._user
+        elif isinstance(user, sdk.User):
+            self._user = user
+        else:
+            raise TypeError(f"user must be either a string or an int. Argument has type: {str(type(user))}.")
+        self.id = self.user_id
+        _, self.channel = self.teamtalk_instance.get_channel(self._user.nChannelID)
+        self.server = self.channel.server
+
+    def send_message(self, content: str, **kwargs) -> int:
+        """Sends a text message to this user.
+
+        Args:
+            content: The content of the message.
+            **kwargs: Keyword arguments. See teamtalk.TeamTalkInstance.send_message for more information.
+
+        Returns:
+            The ID of the message if successful, or a negative value if unsuccessful.
+        """
+        msg = sdk.TextMessage()
+        msg.nMsgType = sdk.TextMsgType.MSGTYPE_USER
+        msg.nFromUserID = self.teamtalk_instance.getMyUserID()
+        msg.szFromUsername = self.teamtalk_instance.getMyUserAccount().szUsername
+        msg.nToUserID = self.user_id
+        msg.szMessage = content
+        msg.bMore = False
+        # get a pointer to our message
+        return self.teamtalk_instance._send_message(msg, **kwargs)
+
+    def move(self, channel) -> bool:
+        """Moves this user to the specified channel.
+
+        Args:
+            channel: The channel to move this user to.
+
+        Returns:
+            True if the user was moved successfully, False otherwise.
+        """
+        return self.server.move_user(self, channel)
+
+    def kick(self, from_server: bool) -> None:
+        """Kicks this user from the server.
+
+        Args:
+            from_server: If True, the user will be kicked from the server. If False, the user will be kicked from the channel. # noqa
+        """
+        channel_id = 0
+        if not from_server:
+            channel_id = self.channel.id
+        self.teamtalk_instance.kick_user(self, channel_id)
+
+    def ban(self, from_server: bool) -> None:
+        """Bans this user from the server.
+
+        Args:
+            from_server: If True, the user will be banned from the server. If False, the user will be banned from the channel. # noqa
+        """
+        channel_id = 0
+        if not from_server:
+            channel_id = self.channel.id
+        self.teamtalk_instance.ban_user(self, channel_id)
+
+    def __getattr__(self, name: str):
+        """Try to get the specified attribute from self._user if it is not found in self.
+
+        Args:
+            name: The name of the attribute.
+
+        Returns:
+            The value of the specified attribute.
+
+        Raises:
+            AttributeError: If the specified attribute is not found. This is the default behavior. # noqa
+        """
+        if name in dir(self):
+            return self.__dict__[name]
+        else:
+            return _get_tt_obj_attribute(self._user, name)
```

### Comparing `teamtalk_py-1.1.0/teamtalk/user_account.py` & `teamtalk_py-1.1.1/teamtalk/user_account.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-"""This module defines a class for a User Account on a TeamTalk server.
-
-The difference between this class and the User class is that this class represents a user account,
-while the User class represents a user that is currently connected to the server.
-"""
-
-from ._utils import _get_tt_obj_attribute
-from .implementation.TeamTalkPy import TeamTalk5 as sdk
-
-
-class UserAccount:
-    """A class for a user account on a TeamTalk server. This class is not meant to be instantiated directly. Instead, use the TeamTalkBot.list_user_accounts() method to get a list of UserAccount objects. # noqa"""
-
-    def __init__(self, teamtalk_instance, account: sdk.UserAccount) -> None:
-        """Initialize a UserAccount object.
-
-        Args:
-            teamtalk_instance: The TeamTalk instance.
-            account: The user account.
-        """
-        self.teamtalk_instance = teamtalk_instance
-        self._account = account
-
-    def __getattr__(self, name: str):
-        """Try to get the specified attribute from self._user if it is not found in self.
-
-        Args:
-            name: The name of the attribute.
-
-        Returns:
-            The value of the specified attribute.
-
-        Raises:
-            AttributeError: If the specified attribute is not found. This is the default behavior. # noqa
-        """
-        if name in dir(self):
-            return self.__dict__[name]
-        else:
-            return _get_tt_obj_attribute(self._account, name)
-
-
-# make a subclass of UserAccount for a banned user
-class BannedUserAccount(UserAccount):
-    """Represents a banned user account on a TeamTalk server. This class is not meant to be instantiated directly. Instead, use the TeamTalkBot.list_banned_users() method to get a list of BannedUserAccount objects. # noqa"""
-
-    # shouldn't do anything extra
-    pass
+"""This module defines a class for a User Account on a TeamTalk server.
+
+The difference between this class and the User class is that this class represents a user account,
+while the User class represents a user that is currently connected to the server.
+"""
+
+from ._utils import _get_tt_obj_attribute
+from .implementation.TeamTalkPy import TeamTalk5 as sdk
+
+
+class UserAccount:
+    """A class for a user account on a TeamTalk server. This class is not meant to be instantiated directly. Instead, use the TeamTalkBot.list_user_accounts() method to get a list of UserAccount objects. # noqa"""
+
+    def __init__(self, teamtalk_instance, account: sdk.UserAccount) -> None:
+        """Initialize a UserAccount object.
+
+        Args:
+            teamtalk_instance: The TeamTalk instance.
+            account: The user account.
+        """
+        self.teamtalk_instance = teamtalk_instance
+        self._account = account
+
+    def __getattr__(self, name: str):
+        """Try to get the specified attribute from self._user if it is not found in self.
+
+        Args:
+            name: The name of the attribute.
+
+        Returns:
+            The value of the specified attribute.
+
+        Raises:
+            AttributeError: If the specified attribute is not found. This is the default behavior. # noqa
+        """
+        if name in dir(self):
+            return self.__dict__[name]
+        else:
+            return _get_tt_obj_attribute(self._account, name)
+
+
+# make a subclass of UserAccount for a banned user
+class BannedUserAccount(UserAccount):
+    """Represents a banned user account on a TeamTalk server. This class is not meant to be instantiated directly. Instead, use the TeamTalkBot.list_banned_users() method to get a list of BannedUserAccount objects. # noqa"""
+
+    # shouldn't do anything extra
+    pass
```

### Comparing `teamtalk_py-1.1.0/PKG-INFO` & `teamtalk_py-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teamtalk-py
-Version: 1.1.0
+Version: 1.1.1
 Summary: a simple but powerful pythonic library for making bots for the TeamTalk5 Conferencing System
 Home-page: https://github.com/JessicaTegner/teamtalk.py/
 License: MIT
 Keywords: teamtalk,teamtalk5,teamtalk sdk,conferencing
 Author: JessicaTegner
 Author-email: jessica.tegner@outlook.com
 Requires-Python: >=3.8,<4.0
@@ -91,17 +91,15 @@
 
 You can find the full documentation [here](http://teamtalkpy.readthedocs.io/en/latest)
 
 
 ## Contributing
 
 So you want to contribute to teamtalk.py? Great! There are many ways to contribute to this project, and all contributions are welcome.
-
 If you have found a bug, have a feature request or want to help improve documentation please [open an issue](https://https://github.com/jessicaTegner/issues/new)_
-
 You can also donate to the projects maintainer (JessicaTegner) to help support the development of teamtalk.py:
 
 
 ## License
 
 This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details
```

