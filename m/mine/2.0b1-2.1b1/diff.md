# Comparing `tmp/mine-2.0b1.tar.gz` & `tmp/mine-2.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mine-2.0b1.tar", max compression
+gzip compressed data, was "mine-2.1b1.tar", max compression
```

## Comparing `mine-2.0b1.tar` & `mine-2.1b1.tar`

### file list

```diff
@@ -1,33 +1,32 @@
--rw-r--r--   0        0        0     1088 2019-05-21 02:49:19.000000 mine-2.0b1/LICENSE.md
--rw-r--r--   0        0        0     2819 2022-08-15 16:48:34.392641 mine-2.0b1/README.md
--rw-r--r--   0        0        0      217 2019-05-21 02:49:19.000000 mine-2.0b1/mine/__init__.py
--rw-r--r--   0        0        0     6625 2022-08-15 16:49:56.206192 mine-2.0b1/mine/cli.py
--rw-r--r--   0        0        0     2866 2019-05-21 02:49:19.000000 mine-2.0b1/mine/common.py
--rw-r--r--   0        0        0     6585 2022-08-15 16:50:17.193486 mine-2.0b1/mine/manager.py
--rw-r--r--   0        0        0      232 2019-05-21 02:49:19.000000 mine-2.0b1/mine/models/__init__.py
--rw-r--r--   0        0        0      424 2021-06-02 19:31:21.821486 mine-2.0b1/mine/models/_bases.py
--rw-r--r--   0        0        0     1803 2019-05-21 02:49:19.000000 mine-2.0b1/mine/models/application.py
--rw-r--r--   0        0        0     2955 2019-05-21 02:49:19.000000 mine-2.0b1/mine/models/computer.py
--rw-r--r--   0        0        0      501 2019-05-21 02:49:19.000000 mine-2.0b1/mine/models/config.py
--rw-r--r--   0        0        0     5145 2020-05-16 16:13:05.000000 mine-2.0b1/mine/models/data.py
--rw-r--r--   0        0        0     6544 2019-05-21 02:49:19.000000 mine-2.0b1/mine/models/status.py
--rw-r--r--   0        0        0     1052 2019-05-21 02:49:19.000000 mine-2.0b1/mine/models/timestamp.py
--rwxr-xr-x   0        0        0     2668 2019-05-21 02:49:19.000000 mine-2.0b1/mine/services.py
--rw-r--r--   0        0        0      574 2019-05-21 02:49:19.000000 mine-2.0b1/mine/settings.py
--rw-r--r--   0        0        0       34 2016-09-23 05:48:42.000000 mine-2.0b1/mine/tests/__init__.py
--rw-r--r--   0        0        0     1039 2020-02-01 14:42:25.000000 mine-2.0b1/mine/tests/conftest.py
--rw-r--r--   0        0        0        9 2016-09-23 02:41:14.000000 mine-2.0b1/mine/tests/files/.gitignore
--rw-r--r--   0        0        0      513 2016-09-23 02:41:14.000000 mine-2.0b1/mine/tests/files/mine-in.yml
--rw-r--r--   0        0        0      587 2016-09-23 02:41:14.000000 mine-2.0b1/mine/tests/files/mine-out.yml
--rw-r--r--   0        0        0     4038 2019-05-21 02:49:19.000000 mine-2.0b1/mine/tests/test_cli.py
--rw-r--r--   0        0        0     3567 2019-05-21 02:49:19.000000 mine-2.0b1/mine/tests/test_manager.py
--rw-r--r--   0        0        0     1550 2016-11-01 16:54:59.000000 mine-2.0b1/mine/tests/test_models_application.py
--rw-r--r--   0        0        0     3976 2019-05-21 02:49:19.000000 mine-2.0b1/mine/tests/test_models_computer.py
--rw-r--r--   0        0        0      377 2016-11-01 16:54:59.000000 mine-2.0b1/mine/tests/test_models_config.py
--rw-r--r--   0        0        0      712 2020-05-16 16:13:00.000000 mine-2.0b1/mine/tests/test_models_data.py
--rw-r--r--   0        0        0     5003 2019-05-21 02:49:19.000000 mine-2.0b1/mine/tests/test_models_status.py
--rw-r--r--   0        0        0     1811 2016-11-01 16:54:59.000000 mine-2.0b1/mine/tests/test_models_timestamp.py
--rw-r--r--   0        0        0     3241 2019-05-21 02:49:19.000000 mine-2.0b1/mine/tests/test_services.py
--rw-r--r--   0        0        0     1846 2022-08-15 16:53:16.971054 mine-2.0b1/pyproject.toml
--rw-r--r--   0        0        0     3837 2022-08-15 17:33:42.697054 mine-2.0b1/setup.py
--rw-r--r--   0        0        0     4085 2022-08-15 17:33:42.697496 mine-2.0b1/PKG-INFO
+-rw-r--r--   0        0        0     1088 2020-10-23 17:27:35.488744 mine-2.1b1/LICENSE.md
+-rw-r--r--   0        0        0     2840 2023-04-15 20:49:09.265706 mine-2.1b1/README.md
+-rw-r--r--   0        0        0      216 2023-04-15 20:01:06.833951 mine-2.1b1/mine/__init__.py
+-rw-r--r--   0        0        0     6624 2023-04-15 20:01:06.838916 mine-2.1b1/mine/cli.py
+-rw-r--r--   0        0        0     2865 2023-04-15 20:01:06.841171 mine-2.1b1/mine/common.py
+-rw-r--r--   0        0        0     6669 2023-04-15 20:03:50.591247 mine-2.1b1/mine/manager.py
+-rw-r--r--   0        0        0      232 2020-10-23 17:27:35.490798 mine-2.1b1/mine/models/__init__.py
+-rw-r--r--   0        0        0      424 2021-05-25 20:38:13.436751 mine-2.1b1/mine/models/_bases.py
+-rw-r--r--   0        0        0     1803 2020-10-23 17:27:35.491009 mine-2.1b1/mine/models/application.py
+-rw-r--r--   0        0        0     2955 2022-09-12 19:07:44.626407 mine-2.1b1/mine/models/computer.py
+-rw-r--r--   0        0        0      501 2020-10-23 17:27:35.491219 mine-2.1b1/mine/models/config.py
+-rw-r--r--   0        0        0     5145 2020-10-23 17:27:35.491342 mine-2.1b1/mine/models/data.py
+-rw-r--r--   0        0        0     6544 2022-09-12 19:07:44.627359 mine-2.1b1/mine/models/status.py
+-rw-r--r--   0        0        0     1052 2020-10-23 17:27:35.491579 mine-2.1b1/mine/models/timestamp.py
+-rwxr-xr-x   0        0        0     2667 2023-04-15 20:01:06.831410 mine-2.1b1/mine/services.py
+-rw-r--r--   0        0        0      573 2023-04-15 20:01:06.843477 mine-2.1b1/mine/settings.py
+-rw-r--r--   0        0        0       34 2020-10-23 17:27:35.491927 mine-2.1b1/mine/tests/__init__.py
+-rw-r--r--   0        0        0     1038 2023-04-15 20:01:06.853224 mine-2.1b1/mine/tests/conftest.py
+-rw-r--r--   0        0        0        9 2020-10-23 17:27:35.492167 mine-2.1b1/mine/tests/files/.gitignore
+-rw-r--r--   0        0        0      513 2020-10-23 17:27:35.492276 mine-2.1b1/mine/tests/files/mine-in.yml
+-rw-r--r--   0        0        0      587 2020-10-23 17:27:35.492361 mine-2.1b1/mine/tests/files/mine-out.yml
+-rw-r--r--   0        0        0     3996 2023-04-15 20:06:10.353515 mine-2.1b1/mine/tests/test_cli.py
+-rw-r--r--   0        0        0     3506 2023-04-15 20:07:27.661985 mine-2.1b1/mine/tests/test_manager.py
+-rw-r--r--   0        0        0     1489 2023-04-15 20:06:45.463018 mine-2.1b1/mine/tests/test_models_application.py
+-rw-r--r--   0        0        0     3915 2023-04-15 20:06:45.540928 mine-2.1b1/mine/tests/test_models_computer.py
+-rw-r--r--   0        0        0      316 2023-04-15 20:06:45.425665 mine-2.1b1/mine/tests/test_models_config.py
+-rw-r--r--   0        0        0      682 2023-04-15 20:05:20.538342 mine-2.1b1/mine/tests/test_models_data.py
+-rw-r--r--   0        0        0     4961 2023-04-15 20:06:10.399880 mine-2.1b1/mine/tests/test_models_status.py
+-rw-r--r--   0        0        0     1750 2023-04-15 20:06:45.481558 mine-2.1b1/mine/tests/test_models_timestamp.py
+-rw-r--r--   0        0        0     3217 2023-04-15 20:10:31.204378 mine-2.1b1/mine/tests/test_services.py
+-rw-r--r--   0        0        0     2326 2023-04-15 20:39:21.861328 mine-2.1b1/pyproject.toml
+-rw-r--r--   0        0        0     4353 1970-01-01 00:00:00.000000 mine-2.1b1/PKG-INFO
```

### Comparing `mine-2.0b1/LICENSE.md` & `mine-2.1b1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mine-2.0b1/README.md` & `mine-2.1b1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -16,26 +16,26 @@
 
 and some just don't make sense to keep running on all your computers:
 
 - Slack
 - HipChat
 - etc.
 
-[![Build Status](https://img.shields.io/travis/jacebrowning/mine/main.svg)](https://travis-ci.org/jacebrowning/mine)
+[![Build Status](https://img.shields.io/travis/com/jacebrowning/mine/main.svg?label=build)](https://travis-ci.com/jacebrowning/mine)
 [![Coverage Status](https://img.shields.io/coveralls/jacebrowning/mine/main.svg)](https://coveralls.io/r/jacebrowning/mine)
 [![Scrutinizer Code Quality](https://img.shields.io/scrutinizer/g/jacebrowning/mine.svg)](https://scrutinizer-ci.com/g/jacebrowning/mine/?branch=main)
 [![PyPI Version](https://img.shields.io/pypi/v/mine.svg)](https://pypi.org/project/mine)
 
-# Setup
+## Setup
 
-## Requirements
+### Requirements
 
 - Python 3.7+
 
-## Installation
+### Installation
 
 Install `mine` with [pipx](https://pipxproject.github.io/pipx/installation/) (or pip):
 
 ```sh
 $ pipx install mine
 ```
 
@@ -43,15 +43,15 @@
 
 ```sh
 $ git clone https://github.com/jacebrowning/mine.git
 $ cd mine
 $ python setup.py install
 ```
 
-## Configuration
+### Configuration
 
 Create a `mine.yml` in your Dropbox:
 
 ```yaml
 config:
   computers:
     - name: My iMac
@@ -79,15 +79,15 @@
         linux: null
 ```
 
 Include the applications you would like `mine` to manage. Computers are added automatically when `mine` is run.
 
 The `versions` dictionary identifies the name of the executable on each platform. The `properties.auto_queue` setting indicates `mine` should attempt to launch the application automatically when switching computers. The `properties.single_instance` setting indicates the application must be closed on other computers before another instance can start.
 
-# Usage
+## Usage
 
 To synchronize the current computer's state:
 
 ```sh
 $ mine
 ```
```

### Comparing `mine-2.0b1/mine/cli.py` & `mine-2.1b1/mine/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,117 +11,116 @@
 import yorm
 from startfile import startfile
 
 from . import CLI, DESCRIPTION, VERSION, common, services
 from .manager import get_manager
 from .models import Application, Data
 
-
 daemon = Application(CLI, filename=CLI)
 
 
 def main(args=None):
     """Process command-line arguments and run the program."""
 
     # Shared options
     debug = argparse.ArgumentParser(add_help=False)
-    debug.add_argument('-V', '--version', action='version', version=VERSION)
+    debug.add_argument("-V", "--version", action="version", version=VERSION)
     group = debug.add_mutually_exclusive_group()
     group.add_argument(
-        '-v', '--verbose', action='count', default=0, help="enable verbose logging"
+        "-v", "--verbose", action="count", default=0, help="enable verbose logging"
     )
     group.add_argument(
-        '-q',
-        '--quiet',
-        action='store_const',
+        "-q",
+        "--quiet",
+        action="store_const",
         const=-1,
-        dest='verbose',
+        dest="verbose",
         help="only display errors and prompts",
     )
 
     # Build main parser
     parser = argparse.ArgumentParser(
         prog=CLI,
         description=DESCRIPTION,
         formatter_class=common.HelpFormatter,
         parents=[debug],
     )
     parser.add_argument(
-        '-d',
-        '--daemon',
-        metavar='DELAY',
-        nargs='?',
+        "-d",
+        "--daemon",
+        metavar="DELAY",
+        nargs="?",
         const=300,
         type=int,
         help="run continuously with delay [seconds]",
     )
-    parser.add_argument('-f', '--file', help="custom settings file path")
-    subs = parser.add_subparsers(help="", dest='command', metavar="<command>")
+    parser.add_argument("-f", "--file", help="custom settings file path")
+    subs = parser.add_subparsers(help="", dest="command", metavar="<command>")
 
     # Build switch parser
     info = "start applications on another computer"
     sub = subs.add_parser(
-        'switch',
-        description=info.capitalize() + '.',
+        "switch",
+        description=info.capitalize() + ".",
         help=info,
         formatter_class=common.HelpFormatter,
         parents=[debug],
     )
     sub.add_argument(
-        'name', nargs='?', help="computer to queue for launch (default: current)"
+        "name", nargs="?", help="computer to queue for launch (default: current)"
     )
 
     # Build close parser
     info = "close applications on this computer"
     sub = subs.add_parser(
-        'close',
-        description=info.capitalize() + '.',
+        "close",
+        description=info.capitalize() + ".",
         help=info,
         formatter_class=common.HelpFormatter,
         parents=[debug],
     )
 
     # Build edit parser
     info = "launch the settings file for editing"
     sub = subs.add_parser(
-        'edit',
-        description=info.capitalize() + '.',
+        "edit",
+        description=info.capitalize() + ".",
         help=info,
         formatter_class=common.HelpFormatter,
         parents=[debug],
     )
 
     # Build clean parser
     info = "display and delete conflicted files"
     sub = subs.add_parser(
-        'clean',
-        description=info.capitalize() + '.',
+        "clean",
+        description=info.capitalize() + ".",
         help=info,
         formatter_class=common.HelpFormatter,
         parents=[debug],
     )
     sub.add_argument(
-        '-f',
-        '--force',
-        action='store_true',
+        "-f",
+        "--force",
+        action="store_true",
         help="actually delete the conflicted files",
     )
 
     # Parse arguments
     args = parser.parse_args(args=args)
-    kwargs = {'delay': args.daemon}
-    if args.command == 'switch':
-        kwargs['switch'] = args.name if args.name else True
-    elif args.command == 'close':
-        kwargs['switch'] = False
-    elif args.command == 'edit':
-        kwargs['edit'] = True
-    elif args.command == 'clean':
-        kwargs['delete'] = True
-        kwargs['force'] = args.force
+    kwargs = {"delay": args.daemon}
+    if args.command == "switch":
+        kwargs["switch"] = args.name if args.name else True
+    elif args.command == "close":
+        kwargs["switch"] = False
+    elif args.command == "edit":
+        kwargs["edit"] = True
+    elif args.command == "clean":
+        kwargs["delete"] = True
+        kwargs["force"] = args.force
 
     # Configure logging
     common.configure_logging(args.verbose)
 
     # Run the program
     try:
         log.debug("Running main command...")
@@ -240,9 +239,9 @@
 
         log.error("Manually start daemon: %s", cmd)
         return False
 
     return True
 
 
-if __name__ == '__main__':  # pragma: no cover (manual test)
+if __name__ == "__main__":  # pragma: no cover (manual test)
     main()
```

### Comparing `mine-2.0b1/mine/common.py` & `mine-2.1b1/mine/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 """Common exceptions, classes, and functions."""
 
 import argparse
 import logging
 
 from . import settings
 
-
 MAX_VERBOSITY = 4
 
 verbosity = 0
 
 
 class HelpFormatter(argparse.HelpFormatter):
     """Command-line help text formatter with wider help text."""
 
     def __init__(self, *args, **kwargs):
-        kwargs['max_help_position'] = 40
+        kwargs["max_help_position"] = 40
         super().__init__(*args, **kwargs)
 
 
 class WarningFormatter(logging.Formatter):
     """Logging formatter that displays verbose formatting for WARNING+."""
 
     def __init__(self, default_format, verbose_format, *args, **kwargs):
@@ -69,15 +68,15 @@
     # Set a custom formatter
     logging.basicConfig(level=level)
     logging.captureWarnings(True)
     formatter = WarningFormatter(
         default_format, verbose_format, datefmt=settings.LOGGING_DATEFMT
     )
     logging.root.handlers[0].setFormatter(formatter)
-    logging.getLogger('yorm').setLevel(max(level, settings.YORM_LOGGING_LEVEL))
+    logging.getLogger("yorm").setLevel(max(level, settings.YORM_LOGGING_LEVEL))
 
     # Warn about excessive verbosity
     global verbosity
     if count > MAX_VERBOSITY:
         msg = "Maximum verbosity level is {}".format(MAX_VERBOSITY)
         logging.warning(msg)
         verbosity = MAX_VERBOSITY
```

### Comparing `mine-2.0b1/mine/manager.py` & `mine-2.1b1/mine/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 import platform
 import time
 from typing import List
 
 import log
 import psutil
 
-
 # TODO: delete this after implementing `BaseManager`
 # https://github.com/jacebrowning/mine/issues/8
 # https://github.com/jacebrowning/mine/issues/9
 
 
 # TODO: enable coverage when a Linux test is implemented
 def log_running(func):  # pragma: no cover (manual)
@@ -58,15 +57,15 @@
 
     return wrapped
 
 
 class BaseManager(metaclass=abc.ABCMeta):  # pragma: no cover (abstract)
     """Base application manager."""
 
-    NAME = FRIENDLY = ''
+    NAME = FRIENDLY = ""
 
     IGNORED_APPLICATION_NAMES: List[str] = []
 
     def __str__(self):
         return self.FRIENDLY
 
     @abc.abstractmethod
@@ -87,15 +86,15 @@
     @classmethod
     def _get_process(cls, name):
         """Get a process whose executable path contains an app name."""
         log.debug("Searching for exe path containing '%s'...", name)
 
         for process in psutil.process_iter():
             try:
-                command = ' '.join(process.cmdline()).lower()
+                command = " ".join(process.cmdline()).lower()
                 parts = []
                 for arg in process.cmdline():
                     parts.extend([p.lower() for p in arg.split(os.sep)])
             except psutil.AccessDenied:
                 continue  # the process is likely owned by root
 
             if name.lower() not in parts:
@@ -119,15 +118,15 @@
 
         return None
 
 
 class LinuxManager(BaseManager):  # pragma: no cover (manual)
     """Application manager for Linux."""
 
-    NAME = 'Linux'
+    NAME = "Linux"
     FRIENDLY = NAME
 
     def is_running(self, application):
         name = application.versions.linux
         if not name:
             return None
         process = self._get_process(name)
@@ -140,26 +139,28 @@
         name = application.versions.linux
         process = self._get_process(name)
         if process.is_running():
             process.terminate()
 
 
 class MacManager(BaseManager):  # pragma: no cover (manual)
-    """Application manager for OS X."""
+    """Application manager for macOS."""
 
-    NAME = 'Darwin'
-    FRIENDLY = 'Mac'
+    NAME = "Darwin"
+    FRIENDLY = "Mac"
 
     IGNORED_APPLICATION_NAMES = [
         "iTunesHelper.app",
         "slack helper.app",
         "garcon.appex",
         "musiccacheextension",
         "podcastswidget",
         "mailcachedelete",
+        "com.apple.mail.spotlightindexextension",
+        "mailshortcutsextension",
     ]
 
     @log_running
     def is_running(self, application):
         name = application.versions.mac
         if not name:
             return None
@@ -195,23 +196,23 @@
         if process and process.is_running():
             process.terminate()
 
     @staticmethod
     def _start_app(path):
         """Start an application from it's .app directory."""
         assert os.path.exists(path), path
-        process = psutil.Popen(['open', path])
+        process = psutil.Popen(["open", path])
         time.sleep(1)
         return process
 
 
 class WindowsManager(BaseManager):  # pragma: no cover (manual)
     """Application manager for Windows."""
 
-    NAME = 'Windows'
+    NAME = "Windows"
     FRIENDLY = NAME
 
     def is_running(self, application):
         pass
 
     def start(self, application):
         pass
```

### Comparing `mine-2.0b1/mine/models/application.py` & `mine-2.1b1/mine/models/application.py`

 * *Files identical despite different names*

### Comparing `mine-2.0b1/mine/models/computer.py` & `mine-2.1b1/mine/models/computer.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         self.hostname = hostname or self.get_hostname()
 
     @staticmethod
     def get_address(node=None):
         """Get this computer's MAC address."""
         if node is None:
             node = uuid.getnode()
-        return ':'.join(("%012X" % node)[i : i + 2] for i in range(0, 12, 2))
+        return ":".join(("%012X" % node)[i : i + 2] for i in range(0, 12, 2))
 
     @staticmethod
     def get_hostname():
         """Get this computer's hostname."""
         return socket.gethostname()
 
 
@@ -79,22 +79,22 @@
         for other in self:
             if this.hostname == other.hostname:
                 other.address = this.address
                 return other
 
         # Else, this is a new computer
         this.name = self.generate_name(this)
-        assert this.name != 'localhost'
+        assert this.name != "localhost"
         log.debug("New computer: %s", this)
         self.append(this)
         return this
 
     def generate_name(self, computer):
         """Generate a new label for a computer."""
-        name = computer.hostname.lower().split('.')[0]
+        name = computer.hostname.lower().split(".")[0]
         copy = 1
         while name in self.names:
             copy += 1
             name2 = "{}-{}".format(name, copy)
             if name2 not in self.names:
                 name = name2
         return name
```

### Comparing `mine-2.0b1/mine/models/data.py` & `mine-2.1b1/mine/models/data.py`

 * *Files identical despite different names*

### Comparing `mine-2.0b1/mine/models/status.py` & `mine-2.1b1/mine/models/status.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,15 +119,15 @@
             if status.application == application.name:
                 states = [s for s in status.computers if s.timestamp.active]
                 if states:
                     states.sort(key=lambda s: s.timestamp, reverse=True)
                     log.debug(
                         "%s marked as started on: %s",
                         application,
-                        ', '.join(str(s) for s in states),
+                        ", ".join(str(s) for s in states),
                     )
                     # TODO: consider returning the computer instance?
                     return states[0].computer
 
         log.debug("marked as started on: nothing")
         return None
```

### Comparing `mine-2.0b1/mine/models/timestamp.py` & `mine-2.1b1/mine/models/timestamp.py`

 * *Files identical despite different names*

### Comparing `mine-2.0b1/mine/services.py` & `mine-2.1b1/mine/services.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,72 +3,71 @@
 import os
 import re
 
 import log
 
 from .models.application import Application, Versions
 
-
 ROOTS = (r"C:\Users", r"/Users", r"/home")
-SERVICES = ('Dropbox', 'Dropbox (Personal)')
-CONFIG = 'mine.yml'
+SERVICES = ("Dropbox", "Dropbox (Personal)")
+CONFIG = "mine.yml"
 CONFLICT_BASE = r"{} \(.+'s conflicted copy \d+-\d+-\d+.*\).*"
 CONFLICT_ANY = CONFLICT_BASE.format(".+")
 CONFLICT_CONFIG = CONFLICT_BASE.format("mine")
 DEPTH = 3  # number of levels to search for the settings file
 APPLICATION = Application(
     "Dropbox",
     versions=Versions(mac="Dropbox.app", windows="Dropbox.exe", linux="dropbox"),
 )
 
 
 def find_root(top=None):
     """Get the root of the shared directory."""
-    top = top or os.path.expanduser('~')
+    top = top or os.path.expanduser("~")
 
     log.debug("Looking for sharing service in '%s'...", top)
     for directory in os.listdir(top):
         if directory in SERVICES:
             path = os.path.join(top, directory)
             log.debug("Found sharing service: %s", path)
             return path
 
     msg = "no sharing service found"
-    if os.getenv('CI'):
+    if os.getenv("CI"):
         log.warning(msg)
         return top
 
     raise EnvironmentError(msg)
 
 
 def find_config_path(top=None, root=None):
     """Get the path to the settings file."""
     log.info("Looking for settings file...")
-    top = top or os.path.expanduser('~')
+    top = top or os.path.expanduser("~")
     root = root or find_root(top=top)
 
     log.debug("Looking for '%s' in '%s'...", CONFIG, root)
     for dirpath, dirnames, _ in os.walk(root):
         depth = dirpath.count(os.path.sep) - root.count(os.path.sep)
         if depth >= DEPTH:
             del dirnames[:]
             continue
         path = os.path.join(dirpath, CONFIG)
-        if os.path.isfile(path) and not os.path.isfile(os.path.join(path, 'setup.py')):
+        if os.path.isfile(path) and not os.path.isfile(os.path.join(path, "setup.py")):
             log.info("Found settings file: %s", path)
             return path
 
     raise EnvironmentError("No '{}' file found".format(CONFIG))
 
 
 def delete_conflicts(root=None, config_only=False, force=False):
     """Delete all files with conflicted filenames."""
     root = root or find_root()
 
-    log.info("%s conflicted files...", 'Deleting' if force else 'Displaying')
+    log.info("%s conflicted files...", "Deleting" if force else "Displaying")
     pattern = CONFLICT_CONFIG if config_only else CONFLICT_ANY
     log.debug("Pattern: %r", pattern)
     regex = re.compile(pattern)
     count = 0
     for dirname, _, filenames in os.walk(root):
         for filename in filenames:
             if regex.match(filename):
```

### Comparing `mine-2.0b1/mine/settings.py` & `mine-2.1b1/mine/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Program defaults."""
 
 import logging
 
-
 # Logging settings
 DEFAULT_LOGGING_FORMAT = "%(message)s"
 LEVELED_LOGGING_FORMAT = "%(levelname)s: %(message)s"
 VERBOSE_LOGGING_FORMAT = "[%(asctime)s %(levelname)8s] %(message)s"
 VERBOSE2_LOGGING_FORMAT = (
     "[%(asctime)s %(levelname)8s] (%(name)-13s @%(lineno)4d) %(message)s"
 )
```

### Comparing `mine-2.0b1/mine/tests/conftest.py` & `mine-2.1b1/mine/tests/conftest.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,33 +2,32 @@
 
 import os
 import platform
 
 import log
 import pytest
 
-
-ENV = 'TEST_INTEGRATION'  # environment variable to enable integration tests
+ENV = "TEST_INTEGRATION"  # environment variable to enable integration tests
 REASON = "'{0}' variable not set".format(ENV)
 
 ROOT = os.path.dirname(__file__)
-FILES = os.path.join(ROOT, 'files')
+FILES = os.path.join(ROOT, "files")
 
 
 def pytest_configure(config):
     """Disable verbose output when running tests."""
     log.init(
         level=log.DEBUG, format="[%(levelname)-8s] (%(name)s @%(lineno)4d) %(message)s"
     )
-    log.silence('yorm', allow_warning=True)
+    log.silence("yorm", allow_warning=True)
 
-    terminal = config.pluginmanager.getplugin('terminal')
+    terminal = config.pluginmanager.getplugin("terminal")
     terminal.TerminalReporter.showfspath = False
 
 
 def pytest_runtest_setup(item):
-    if 'linux_only' in item.keywords and platform.system() != 'Linux':
+    if "linux_only" in item.keywords and platform.system() != "Linux":
         pytest.skip("test can only be run on Linux")
-    if 'mac_only' in item.keywords and platform.system() != 'Darwin':
+    if "mac_only" in item.keywords and platform.system() != "Darwin":
         pytest.skip("test can only be run on OS X")
-    if 'windows_only' in item.keywords and platform.system() != 'Windows':
+    if "windows_only" in item.keywords and platform.system() != "Windows":
         pytest.skip("test can only be run on Windows")
```

### Comparing `mine-2.0b1/mine/tests/files/mine-in.yml` & `mine-2.1b1/mine/tests/files/mine-in.yml`

 * *Files identical despite different names*

### Comparing `mine-2.0b1/mine/tests/files/mine-out.yml` & `mine-2.1b1/mine/tests/files/mine-out.yml`

 * *Files identical despite different names*

### Comparing `mine-2.0b1/mine/tests/test_cli.py` & `mine-2.1b1/mine/tests/test_cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,138 +1,138 @@
-# pylint: disable=misplaced-comparison-constant,no-self-use,redefined-outer-name
+# pylint: disable=redefined-outer-name
 
 import logging
 import os
 from unittest.mock import Mock, patch
 
 import pytest
 
 from mine import cli, common
 from mine.models import Application
 
 
 @pytest.fixture
 def tmp_path(tmpdir):
-    return tmpdir.join('custom.ext').strpath
+    return tmpdir.join("custom.ext").strpath
 
 
 class TestMain:
     """Unit tests for the `main` function."""
 
-    @patch('mine.cli.run', Mock(return_value=True))
+    @patch("mine.cli.run", Mock(return_value=True))
     def test_run(self):
         """Verify the CLI can be run."""
         cli.main([])
 
-    @patch('mine.cli.run', Mock(return_value=False))
+    @patch("mine.cli.run", Mock(return_value=False))
     def test_run_fail(self):
         """Verify the CLI can detect errors."""
         with pytest.raises(SystemExit):
             cli.main([])
 
     def test_help(self):
         """Verify the CLI help text can be displayed."""
         with pytest.raises(SystemExit):
-            cli.main(['--help'])
+            cli.main(["--help"])
 
-    @patch('mine.cli.run', Mock(side_effect=KeyboardInterrupt))
+    @patch("mine.cli.run", Mock(side_effect=KeyboardInterrupt))
     def test_interrupt(self):
         """Verify the CLI can be interrupted."""
         with pytest.raises(SystemExit):
             cli.main([])
 
-    @patch('mine.cli.log')
-    @patch('mine.cli.run', Mock(side_effect=KeyboardInterrupt))
+    @patch("mine.cli.log")
+    @patch("mine.cli.run", Mock(side_effect=KeyboardInterrupt))
     def test_interrupt_verbose(self, mock_log):
         """Verify the CLI can be interrupted (verbose output)."""
         with pytest.raises(SystemExit):
-            cli.main(['-vvvv'])
+            cli.main(["-vvvv"])
         assert mock_log.exception.call_count == 1
 
-    @patch('mine.cli.daemon', None)
+    @patch("mine.cli.daemon", None)
     def test_path(self, tmp_path):
         """Verify a custom setting file path can be used."""
-        cli.main(['--file', tmp_path])
+        cli.main(["--file", tmp_path])
 
         assert os.path.isfile(tmp_path)
 
-    @patch('mine.cli.run')
+    @patch("mine.cli.run")
     def test_daemon(self, mock_run):
-        cli.main(['--daemon'])
+        cli.main(["--daemon"])
         mock_run.assert_called_once_with(path=None, delay=300)
 
-    @patch('mine.cli.run')
+    @patch("mine.cli.run")
     def test_daemon_with_specific_delay(self, mock_run):
-        cli.main(['--daemon', '42'])
+        cli.main(["--daemon", "42"])
         mock_run.assert_called_once_with(path=None, delay=42)
 
-    @patch('mine.cli.daemon', Application(None))
+    @patch("mine.cli.daemon", Application(None))
     def test_warning_when_daemon_is_not_running(self, tmp_path):
         with pytest.raises(SystemExit):
-            cli.main(['--file', tmp_path])
+            cli.main(["--file", tmp_path])
 
 
 class TestSwitch:
     """Unit tests for the `switch` function."""
 
-    @patch('mine.cli.run')
+    @patch("mine.cli.run")
     def test_switch(self, mock_run):
         """Verify a the current computer can be queued."""
-        cli.main(['switch'])
+        cli.main(["switch"])
         mock_run.assert_called_once_with(path=None, delay=None, switch=True)
 
-    @patch('mine.cli.run')
+    @patch("mine.cli.run")
     def test_switch_specific(self, mock_run):
         """Verify a specific computer can be queued."""
-        cli.main(['switch', 'foobar'])
-        mock_run.assert_called_once_with(path=None, delay=None, switch='foobar')
+        cli.main(["switch", "foobar"])
+        mock_run.assert_called_once_with(path=None, delay=None, switch="foobar")
 
 
 class TestClean:
-    @patch('mine.cli.run')
+    @patch("mine.cli.run")
     def test_clean(self, mock_run):
-        cli.main(['clean'])
+        cli.main(["clean"])
         mock_run.assert_called_once_with(
             path=None, delay=None, delete=True, force=False
         )
 
-    @patch('mine.cli.run')
+    @patch("mine.cli.run")
     def test_clean_with_force(self, mock_run):
-        cli.main(['clean', '--force'])
+        cli.main(["clean", "--force"])
         mock_run.assert_called_once_with(path=None, delay=None, delete=True, force=True)
 
 
 class TestEdit:
-    @patch('mine.cli.run')
+    @patch("mine.cli.run")
     def test_edit(self, mock_run):
-        cli.main(['edit'])
+        cli.main(["edit"])
         mock_run.assert_called_once_with(path=None, delay=None, edit=True)
 
 
 def _mock_run(*args, **kwargs):
     """Placeholder logic for logging tests."""
     logging.debug(args)
     logging.debug(kwargs)
     logging.warning("warning")
     logging.error("error")
     return True
 
 
-@patch('mine.cli.run', _mock_run)
+@patch("mine.cli.run", _mock_run)
 class TestLogging:
     """Integration tests for the Doorstop CLI logging."""
 
     arg_verbosity = [
-        ('', 0),
-        ('-v', 1),
-        ('-vv', 2),
-        ('-vvv', 3),
-        ('-vvvv', 4),
-        ('-vvvvv', 4),
-        ('-q', -1),
+        ("", 0),
+        ("-v", 1),
+        ("-vv", 2),
+        ("-vvv", 3),
+        ("-vvvv", 4),
+        ("-vvvvv", 4),
+        ("-q", -1),
     ]
 
     @pytest.mark.parametrize("arg,verbosity", arg_verbosity)
     def test_verbose(self, arg, verbosity):
         """Verify verbose level can be set."""
         cli.main([arg] if arg else [])
         assert verbosity == common.verbosity
```

### Comparing `mine-2.0b1/mine/tests/test_manager.py` & `mine-2.1b1/mine/tests/test_manager.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,99 +1,97 @@
-# pylint: disable=misplaced-comparison-constant,no-self-use
-
 import pytest
 
 from mine.manager import LinuxManager, MacManager, WindowsManager, get_manager
 from mine.models import Application
 
 
 class TestLinuxManager:
     """Unit tests for the Linux manager class."""
 
-    manager = get_manager('Linux')
+    manager = get_manager("Linux")
 
     def test_init(self):
         """Verify the OS is detected correctly."""
         assert isinstance(self.manager, LinuxManager)
 
     def test_is_running_false(self):
         """Verify a process can be detected as not running."""
         pytest.skip("TODO: implement test")
-        application = Application('fake-program-for-mine')
-        application.versions.linux = 'fake_program_for_mine.sh'
+        application = Application("fake-program-for-mine")
+        application.versions.linux = "fake_program_for_mine.sh"
         assert False is self.manager.is_running(application)
 
     @pytest.mark.linux_only
     def test_is_running_true(self):
         """Verify a process can be detected as running."""
         pytest.skip("TODO: implement test")
 
     def test_is_running_none(self):
         """Verify a process can be detected as untracked."""
-        application = Application('fake-program-for-mine')
+        application = Application("fake-program-for-mine")
         assert None is self.manager.is_running(application)
 
 
 class TestMacManager:
     """Unit tests for the Mac manager class."""
 
-    manager = get_manager('Darwin')
+    manager = get_manager("Darwin")
 
     def test_init(self):
         """Verify the OS is detected correctly."""
         assert isinstance(self.manager, MacManager)
 
     def test_is_running_false(self):
         """Verify a process can be detected as not running."""
-        application = Application('fake-program-for-mine')
-        application.versions.mac = 'FakeProgramForMine.app'
+        application = Application("fake-program-for-mine")
+        application.versions.mac = "FakeProgramForMine.app"
         assert False is self.manager.is_running(application)
 
     @pytest.mark.mac_only
     def test_is_running_true(self):
         """Verify a process can be detected as running."""
-        application = Application('finder')
-        application.versions.mac = 'Finder.app'
+        application = Application("finder")
+        application.versions.mac = "Finder.app"
         assert True is self.manager.is_running(application)
 
     def test_is_running_none(self):
         """Verify a process can be detected as untracked."""
-        application = Application('fake-program-for-mine')
+        application = Application("fake-program-for-mine")
         assert None is self.manager.is_running(application)
 
     @pytest.mark.mac_only
     def test_stop(self):
         """Verify a process can be stopped."""
-        application = Application('mail')
-        application.versions.mac = 'Mail.app'
+        application = Application("mail")
+        application.versions.mac = "Mail.app"
         self.manager.stop(application)
         assert not self.manager.is_running(application)
 
 
 class TestWindowsManager:
     """Unit tests for the Windows manager class."""
 
-    manager = get_manager('Windows')
+    manager = get_manager("Windows")
 
     def test_init(self):
         """Verify the OS is detected correctly."""
         assert isinstance(self.manager, WindowsManager)
 
     def test_is_running_false(self):
         """Verify a process can be detected as not running."""
         pytest.skip("TODO: implement test")
-        application = Application('fake-program-for-mine')
-        application.versions.windows = 'FakeProgramForMine.exe'
+        application = Application("fake-program-for-mine")
+        application.versions.windows = "FakeProgramForMine.exe"
         assert False is self.manager.is_running(application)
 
     @pytest.mark.windows_only
     def test_is_running_true(self):
         """Verify a process can be detected as running."""
         pytest.skip("TODO: implement test")
-        application = Application('explorer')
-        application.versions.windows = 'explorer.exe'
+        application = Application("explorer")
+        application.versions.windows = "explorer.exe"
         assert True is self.manager.is_running(application)
 
     def test_is_running_none(self):
         """Verify a process can be detected as untracked."""
-        application = Application('fake-program-for-mine')
+        application = Application("fake-program-for-mine")
         assert None is self.manager.is_running(application)
```

### Comparing `mine-2.0b1/mine/tests/test_models_application.py` & `mine-2.1b1/mine/tests/test_models_application.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,21 @@
-# pylint: disable=misplaced-comparison-constant,no-self-use
-
 import pytest
 
 from mine.models import Application, Applications
 
 
 class TestApplication:
     """Unit tests for the application class."""
 
-    app1 = Application('iTunes')
-    app1.versions.mac = 'iTunes.app'
-    app2 = Application('HipChat')
-    app3 = Application('Sublime Text')
-    app3.versions.linux = 'sublime_text'
-    app4 = Application('hipchat')
+    app1 = Application("iTunes")
+    app1.versions.mac = "iTunes.app"
+    app2 = Application("HipChat")
+    app3 = Application("Sublime Text")
+    app3.versions.linux = "sublime_text"
+    app4 = Application("hipchat")
 
     str_application = [
         ("iTunes", app1),
         ("HipChat", app2),
         ("Sublime Text", app3),
         ("hipchat", app4),
     ]
@@ -41,14 +39,14 @@
 class TestApplications:
     """Unit tests for lists of applications."""
 
     apps = Applications([TestApplication.app1, TestApplication.app2])
 
     def test_get(self):
         """Verify an application can be found in a list."""
-        app = self.apps.get('itunes')
-        assert 'iTunes' == app.name
+        app = self.apps.get("itunes")
+        assert "iTunes" == app.name
 
     def test_get_missing(self):
         """Verify an invalid names raise an assertion."""
         with pytest.raises(AssertionError):
-            self.apps.get('fake')
+            self.apps.get("fake")
```

### Comparing `mine-2.0b1/mine/tests/test_models_computer.py` & `mine-2.1b1/mine/tests/test_models_computer.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,108 +1,106 @@
-# pylint: disable=misplaced-comparison-constant,no-self-use
-
 from unittest.mock import Mock, patch
 
 import pytest
 
 from mine.models import Computer, Computers
 
 
-@patch('uuid.getnode', Mock(return_value=0))
-@patch('socket.gethostname', Mock(return_value='Sample.local'))
+@patch("uuid.getnode", Mock(return_value=0))
+@patch("socket.gethostname", Mock(return_value="Sample.local"))
 class TestComputer:
     """Unit tests for the computer classes."""
 
     def test_init(self):
         """Verify the correct computer information is loaded."""
-        computer = Computer('my-sample')
-        assert 'my-sample' == computer.name
-        assert '00:00:00:00:00:00' == computer.address
-        assert 'Sample.local' == computer.hostname
+        computer = Computer("my-sample")
+        assert "my-sample" == computer.name
+        assert "00:00:00:00:00:00" == computer.address
+        assert "Sample.local" == computer.hostname
 
     def test_init_defaults(self):
         """Verify the correct computer information can be overridden."""
-        computer = Computer('name', 'hostname', 'address')
-        assert 'name' == computer.name
-        assert 'address' == computer.address
-        assert 'hostname' == computer.hostname
+        computer = Computer("name", "hostname", "address")
+        assert "name" == computer.name
+        assert "address" == computer.address
+        assert "hostname" == computer.hostname
 
     def test_eq(self):
         """Verify computers and strings can be equated."""
-        assert Computer('mac1') == Computer('mac1')
-        assert Computer('mac1') != Computer('mac2')
-        assert Computer('mac1') == 'mac1'
-        assert 'mac1' != Computer('mac2')
+        assert Computer("mac1") == Computer("mac1")
+        assert Computer("mac1") != Computer("mac2")
+        assert Computer("mac1") == "mac1"
+        assert "mac1" != Computer("mac2")
 
     def test_lt(self):
         """Verify computers can be sorted."""
-        assert Computer('mac1') < Computer('mac2')
-        assert Computer('def') > Computer('ABC')
+        assert Computer("mac1") < Computer("mac2")
+        assert Computer("def") > Computer("ABC")
 
     def test_get_match_none(self):
         """Verify a computer is added when missing."""
-        other = Computer('name', 'hostname', 'address')
+        other = Computer("name", "hostname", "address")
         computers = Computers([other])
         this = computers.get_current()
-        assert 'sample' == this.name
-        assert '00:00:00:00:00:00' == this.address
-        assert 'Sample.local' == this.hostname
+        assert "sample" == this.name
+        assert "00:00:00:00:00:00" == this.address
+        assert "Sample.local" == this.hostname
         assert 2 == len(computers)
 
     def test_get_match_all(self):
         """Verify a computer can be matched exactly."""
-        other = Computer('all', 'Sample.local', '00:00:00:00:00:00')
+        other = Computer("all", "Sample.local", "00:00:00:00:00:00")
         computers = Computers([other])
         this = computers.get_current()
-        assert 'all' == this.name
-        assert '00:00:00:00:00:00' == this.address
-        assert 'Sample.local' == this.hostname
+        assert "all" == this.name
+        assert "00:00:00:00:00:00" == this.address
+        assert "Sample.local" == this.hostname
         assert 1 == len(computers)
 
 
-@patch('uuid.getnode', Mock(return_value=0))
-@patch('socket.gethostname', Mock(return_value='Sample.local'))
+@patch("uuid.getnode", Mock(return_value=0))
+@patch("socket.gethostname", Mock(return_value="Sample.local"))
 class TestComputers:
     """Unit tests for lists of computers."""
 
     computers = Computers(
-        [Computer('abc', 'abc.local', 1), Computer('def', 'def.local', 2)]
+        [Computer("abc", "abc.local", 1), Computer("def", "def.local", 2)]
     )
 
     def test_get(self):
         """Verify a computer can be found in a list."""
-        computer = self.computers.get('ABC')
-        assert 'abc' == computer.name
+        computer = self.computers.get("ABC")
+        assert "abc" == computer.name
 
     def test_get_missing(self):
         """Verify an invalid names raise an assertion."""
         with pytest.raises(AssertionError):
-            self.computers.get('fake')
+            self.computers.get("fake")
 
     def test_match(self):
         """Verify a similar computer can be found."""
-        computer = self.computers.match('AB')
-        assert 'abc' == computer.name
+        computer = self.computers.match("AB")
+        assert "abc" == computer.name
 
     def test_generate_name(self):
         """Verify a computer name is generated correctly."""
         computers = Computers()
-        computer = Computer(None, hostname='Jaces-iMac.local')
+        computer = Computer(None, hostname="Jaces-iMac.local")
         name = computers.generate_name(computer)
-        assert 'jaces-imac' == name
+        assert "jaces-imac" == name
 
     def test_generate_name_duplicates(self):
         """Verify a computer name is generated correctly with duplicates."""
-        computers = Computers([Computer('jaces-imac')])
-        computer = Computer(None, hostname='Jaces-iMac.local')
+        computers = Computers([Computer("jaces-imac")])
+        computer = Computer(None, hostname="Jaces-iMac.local")
         name = computers.generate_name(computer)
-        assert 'jaces-imac-2' == name
+        assert "jaces-imac-2" == name
 
     def test_get_current_by_matching_address(self):
-        computers = Computers([Computer('abc', 'foobar', '00:00:00:00:00:00')])
+        computers = Computers([Computer("abc", "foobar", "00:00:00:00:00:00")])
         computer = computers.get_current()
-        assert 'abc' == computer.name
+        assert "abc" == computer.name
 
     def test_get_current_by_matching_hostname(self):
-        computers = Computers([Computer('abc', 'Sample.local', 'foobar')])
+        computers = Computers([Computer("abc", "Sample.local", "foobar")])
         computer = computers.get_current()
-        assert 'abc' == computer.name
+        assert "abc" == computer.name
```

### Comparing `mine-2.0b1/mine/tests/test_models_data.py` & `mine-2.1b1/mine/tests/test_models_data.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=misplaced-comparison-constant,unused-variable
+# pylint: disable=unused-variable
 
 import pytest
 
 from mine.models import Data
 
 
 def describe_data():
```

### Comparing `mine-2.0b1/mine/tests/test_models_status.py` & `mine-2.1b1/mine/tests/test_models_status.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-# pylint: disable=misplaced-comparison-constant,no-self-use,attribute-defined-outside-init
+# pylint: disable=attribute-defined-outside-init
 
 from unittest.mock import Mock
 
 import pytest
 
 from mine.models import Application, ProgramStatus, State, Status
 
 
 class TestState:
     """Unit tests for the computer state class."""
 
-    state1 = State('computer1')
-    state2 = State('computer2')
+    state1 = State("computer1")
+    state2 = State("computer2")
     state2.timestamp.started = 42
-    state3 = State('Computer2')
-    state4 = State('Computer2')
+    state3 = State("Computer2")
+    state4 = State("Computer2")
 
     str_state = [("computer1", state1), ("computer2", state2), ("Computer2", state3)]
 
     @pytest.mark.parametrize("string,state", str_state)
     def test_str(self, string, state):
         """Verify states can be converted to strings."""
         assert string == str(state)
@@ -34,18 +34,18 @@
         assert self.state1 < self.state2
         assert self.state3 > self.state1
 
 
 class TestStatus:
     """Unit tests for the application status class."""
 
-    status1 = Status('app1')
-    status2 = Status('app2')
-    status3 = Status('App2')
-    status4 = Status('App2')
+    status1 = Status("app1")
+    status2 = Status("app2")
+    status3 = Status("App2")
+    status4 = Status("App2")
 
     str_status = [("app1", status1), ("app2", status2), ("App2", status3)]
 
     @pytest.mark.parametrize("string,status", str_status)
     def test_str(self, string, status):
         """Verify statuss can be converted to strings."""
         assert string == str(status)
@@ -64,21 +64,21 @@
 
 class TestProgramStatus:
     """Unit tests for the program status class."""
 
     def setup_method(self, _):
         """Create an empty program status for all tests."""
         self.status = ProgramStatus()
-        self.application = Application('my-application')
+        self.application = Application("my-application")
         self.computer = Mock()
-        self.computer.name = 'local'
+        self.computer.name = "local"
         self.computer2 = Mock()
-        self.computer2.name = 'remote'
+        self.computer2.name = "remote"
         self.computer3 = Mock()
-        self.computer3.name = 'remote2'
+        self.computer3.name = "remote2"
 
     def test_get_latest(self):
         """Verify the latest computer can be determined."""
         self.status.start(self.application, self.computer)
         self.status.start(self.application, self.computer2)
         self.status.stop(self.application, self.computer3)
         assert self.computer2.name == self.status.get_latest(self.application)
```

### Comparing `mine-2.0b1/mine/tests/test_models_timestamp.py` & `mine-2.1b1/mine/tests/test_models_timestamp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# pylint: disable=misplaced-comparison-constant,no-self-use
-
 import pytest
 
 from mine.models import Timestamp
 
 
 class TestTimestamp:
     """Unit tests for the timestamp class."""
```

### Comparing `mine-2.0b1/mine/tests/test_services.py` & `mine-2.1b1/mine/tests/test_services.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=misplaced-comparison-constant,no-self-use,redefined-outer-name
+# pylint: disable=redefined-outer-name
 
 import os
 from unittest.mock import Mock, patch
 
 import pytest
 
 from mine import services
@@ -19,64 +19,64 @@
 
 def touch(*parts):
     """Create an empty file at the given path."""
     path = os.path.join(*parts)
     dirpath = os.path.dirname(path)
     if not os.path.isdir(dirpath):
         os.makedirs(dirpath)
-    open(path, 'w').close()
+    open(path, "w", encoding="utf-8").close()
 
 
 class TestFindRoot:
-    @patch('os.listdir', Mock(return_value=[]))
-    @patch('os.getenv', Mock(return_value=True))
+    @patch("os.listdir", Mock(return_value=[]))
+    @patch("os.getenv", Mock(return_value=True))
     def test_ci_workaround_enabled(self):
         root = services.find_root(top="mock/top")
         assert "mock/top" == root
 
-    @patch('os.listdir', Mock(return_value=[]))
-    @patch('os.getenv', Mock(return_value=False))
+    @patch("os.listdir", Mock(return_value=[]))
+    @patch("os.getenv", Mock(return_value=False))
     def test_ci_workaround_disabled(self):
         with pytest.raises(EnvironmentError):
             services.find_root(top="mock/top")
 
 
 class TestFindConfigPath:
     def test_find_dropbox(self, tmp_dir):
         """Verify a settings file can be found in Dropbox."""
-        touch('Dropbox', 'mine.yml')
+        touch("Dropbox", "mine.yml")
 
         path = services.find_config_path(tmp_dir)
 
         assert os.path.isfile(path)
 
     def test_find_dropbox_personal(self, tmp_dir):
         """Verify a settings file can be found in Dropbox (Personal)."""
-        touch('Dropbox (Personal)', 'mine.yml')
+        touch("Dropbox (Personal)", "mine.yml")
 
         path = services.find_config_path(tmp_dir)
 
         assert os.path.isfile(path)
 
-    @patch('mine.services.DEPTH', 2)
+    @patch("mine.services.DEPTH", 2)
     def test_find_depth(self, tmp_dir):
         """Verify a settings file is not found below the maximum depth."""
-        touch('Dropbox', 'a', 'b', 'mine.yml')
+        touch("Dropbox", "a", "b", "mine.yml")
 
         with pytest.raises(OSError):
             services.find_config_path(tmp_dir)
 
     def test_find_no_share(self):
         """Verify an error occurs when no service directory is found."""
         with pytest.raises(EnvironmentError):
-            with patch('os.getenv', Mock(return_value=False)):
+            with patch("os.getenv", Mock(return_value=False)):
                 services.find_config_path(FILES)
 
 
-@patch('os.remove')
+@patch("os.remove")
 class TestDeleteConflicts:
     @staticmethod
     def _create_conflicts(tmp_dir, count=2):
         for index in range(count):
             fmt = "{} (Jace's conflicted copy 2015-03-11).fake"
             filename = fmt.format(index)
             touch(tmp_dir, filename)
```

### Comparing `mine-2.0b1/pyproject.toml` & `mine-2.1b1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 
 name = "mine"
-version = "2.0b1"
+version = "2.1b1"
 description = "Share application state across computers using Dropbox."
 
 license = "MIT"
 
 authors = ["Jace Browning <jacebrowning@gmail.com>"]
 
 readme = "README.md"
@@ -21,72 +21,103 @@
     "Environment :: Console",
     "Intended Audience :: End Users/Desktop",
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Topic :: System",
     "Topic :: System :: Monitoring",
     "Topic :: Utilities",
 ]
 
 [tool.poetry.dependencies]
 
-python = "^3.7"
+python = "^3.8"
 
 YORM = "^1.4"
-psutil = "^2.1"
-crayons = "~0.1.2"
-minilog = "^0.3"
+psutil = "^2.2"
+crayons = "~0.1"
+minilog = "^2.0"
 universal-startfile = "*"
 
 [tool.poetry.dev-dependencies]
 
 # Formatters
-black = "=20.8b1"
-isort = "=5.6.4"
+black = "^22.1"
+tomli = "*" # missing 'black' dependency
+isort = "^5.10"
 
 # Linters
-mypy = "^0.812"
-pydocstyle = "*"
-pylint = "^2.0"
+mypy = "^1.0"
+pydocstyle = "^6.1"
+pylint = "~2.15"
+wrapt = "*" # missing 'pylint' dependency
+types-setuptools = "*"
 
 # Testing
-pytest = "^5.3.5"
-pytest-cov = "*"
-pytest-describe = "*"
-pytest-expecter = "*"
+pytest = "^7.1"
+pytest-describe = "^2.0"
+pytest-expecter = "^3.0"
 pytest-random = "*"
+pytest-cov = "^3.0"
 freezegun = "*"
 
 # Reports
-coveragespace = "^3.1"
+coveragespace = "^6.0"
 
 # Documentation
-mkdocs = "^1.3"
-pygments = "*"
+mkdocs = "^1.4"
+pygments = "^2.11"
 
 # Tooling
 pyinstaller = "*"
 sniffer = "*"
 MacFSEvents = { version = "*", platform = "darwin" }
 pync = { version = "*", platform = "darwin" }
-ipython = "^7.12.0"
+ipython = "^7.16.3"
 
 [tool.poetry.scripts]
 
 mine = "mine.cli:main"
 
 [tool.black]
 
-target-version = ["py36", "py37"]
-skip-string-normalization = true
+quiet = true
+
+[tool.isort]
+
+profile = "black"
+
+[tool.mypy]
+
+ignore_missing_imports = true
+no_implicit_optional = true
+check_untyped_defs = true
+
+cache_dir = ".cache/mypy/"
+
+[tool.pytest.ini_options]
+
+addopts = """
+--strict-markers
+
+-r sxX
+--show-capture=log
+
+--cov-report=html
+--cov-report=term-missing:skip-covered
+--no-cov-on-fail
+"""
+
+cache_dir = ".cache/pytest/"
+
+markers = ["linux_only", "mac_only", "windows_only"]
 
 [build-system]
 
-requires = ["poetry>=0.12"]
-build-backend = "poetry.masonry.api"
+requires = ["poetry-core>=1.0.0"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `mine-2.0b1/setup.py` & `mine-2.1b1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,38 +1,155 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: mine
+Version: 2.1b1
+Summary: Share application state across computers using Dropbox.
+Home-page: https://pypi.org/project/mine
+License: MIT
+Author: Jace Browning
+Author-email: jacebrowning@gmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: System
+Classifier: Topic :: System :: Monitoring
+Classifier: Topic :: Utilities
+Requires-Dist: YORM (>=1.4,<2.0)
+Requires-Dist: crayons (>=0.1,<0.2)
+Requires-Dist: minilog (>=2.0,<3.0)
+Requires-Dist: psutil (>=2.2,<3.0)
+Requires-Dist: universal-startfile
+Project-URL: Documentation, https://mine.readthedocs.io
+Project-URL: Repository, https://github.com/jacebrowning/mine
+Description-Content-Type: text/markdown
+
+# Overview
+
+This program lets you synchronize application data using Dropbox.
+
+It automatically starts and stops programs that would otherwise fight over data in a shared folder and ensures only one instance is running. Many applications work fine when their data is stored in Dropbox, but some programs overwrite databases:
+
+- iTunes
+- iPhoto
+- etc.
+
+while others periodically write snapshot data:
+
+- Eclipse
+- Xcode
+- etc.
+
+and some just don't make sense to keep running on all your computers:
+
+- Slack
+- HipChat
+- etc.
+
+[![Build Status](https://img.shields.io/travis/com/jacebrowning/mine/main.svg?label=build)](https://travis-ci.com/jacebrowning/mine)
+[![Coverage Status](https://img.shields.io/coveralls/jacebrowning/mine/main.svg)](https://coveralls.io/r/jacebrowning/mine)
+[![Scrutinizer Code Quality](https://img.shields.io/scrutinizer/g/jacebrowning/mine.svg)](https://scrutinizer-ci.com/g/jacebrowning/mine/?branch=main)
+[![PyPI Version](https://img.shields.io/pypi/v/mine.svg)](https://pypi.org/project/mine)
+
+## Setup
+
+### Requirements
+
+- Python 3.7+
+
+### Installation
+
+Install `mine` with [pipx](https://pipxproject.github.io/pipx/installation/) (or pip):
+
+```sh
+$ pipx install mine
+```
+
+or directly from the source code:
+
+```sh
+$ git clone https://github.com/jacebrowning/mine.git
+$ cd mine
+$ python setup.py install
+```
+
+### Configuration
+
+Create a `mine.yml` in your Dropbox:
+
+```yaml
+config:
+  computers:
+    - name: My iMac
+      hostname: My-iMac.local
+      address: 00:11:22:33:44:55
+    - name: My MacBook Air
+      hostname: My-MacBook-Air.local
+      address: AA:BB:CC:DD:EE:FF
+  applications:
+    - name: iTunes
+      properties:
+        auto_queue: false
+        single_instance: true
+      versions:
+        mac: iTunes.app
+        windows: iTunes.exe
+        linux: null
+    - name: Slack
+      properties:
+        auto_queue: true
+        single_instance: false
+      versions:
+        mac: Slack.app
+        windows: null
+        linux: null
+```
+
+Include the applications you would like `mine` to manage. Computers are added automatically when `mine` is run.
+
+The `versions` dictionary identifies the name of the executable on each platform. The `properties.auto_queue` setting indicates `mine` should attempt to launch the application automatically when switching computers. The `properties.single_instance` setting indicates the application must be closed on other computers before another instance can start.
+
+## Usage
+
+To synchronize the current computer's state:
+
+```sh
+$ mine
+```
+
+To close applications on remote computers and start them locally:
+
+```sh
+$ mine switch
+```
+
+To close applications running locally:
+
+```sh
+$ mine close
+```
+
+To close applications locally and start them on another computer:
+
+```sh
+$ mine switch <name>
+```
+
+To delete conflicted files in your Dropbox:
+
+```sh
+$ mine clean
+```
 
-packages = \
-['mine', 'mine.models', 'mine.tests']
-
-package_data = \
-{'': ['*'], 'mine.tests': ['files/*']}
-
-install_requires = \
-['YORM>=1.4,<2.0',
- 'crayons>=0.1.2,<0.2.0',
- 'minilog>=0.3,<0.4',
- 'psutil>=2.1,<3.0',
- 'universal-startfile']
-
-entry_points = \
-{'console_scripts': ['mine = mine.cli:main']}
-
-setup_kwargs = {
-    'name': 'mine',
-    'version': '2.0b1',
-    'description': 'Share application state across computers using Dropbox.',
-    'long_description': "# Overview\n\nThis program lets you synchronize application data using Dropbox.\n\nIt automatically starts and stops programs that would otherwise fight over data in a shared folder and ensures only one instance is running. Many applications work fine when their data is stored in Dropbox, but some programs overwrite databases:\n\n- iTunes\n- iPhoto\n- etc.\n\nwhile others periodically write snapshot data:\n\n- Eclipse\n- Xcode\n- etc.\n\nand some just don't make sense to keep running on all your computers:\n\n- Slack\n- HipChat\n- etc.\n\n[![Build Status](https://img.shields.io/travis/jacebrowning/mine/main.svg)](https://travis-ci.org/jacebrowning/mine)\n[![Coverage Status](https://img.shields.io/coveralls/jacebrowning/mine/main.svg)](https://coveralls.io/r/jacebrowning/mine)\n[![Scrutinizer Code Quality](https://img.shields.io/scrutinizer/g/jacebrowning/mine.svg)](https://scrutinizer-ci.com/g/jacebrowning/mine/?branch=main)\n[![PyPI Version](https://img.shields.io/pypi/v/mine.svg)](https://pypi.org/project/mine)\n\n# Setup\n\n## Requirements\n\n- Python 3.7+\n\n## Installation\n\nInstall `mine` with [pipx](https://pipxproject.github.io/pipx/installation/) (or pip):\n\n```sh\n$ pipx install mine\n```\n\nor directly from the source code:\n\n```sh\n$ git clone https://github.com/jacebrowning/mine.git\n$ cd mine\n$ python setup.py install\n```\n\n## Configuration\n\nCreate a `mine.yml` in your Dropbox:\n\n```yaml\nconfig:\n  computers:\n    - name: My iMac\n      hostname: My-iMac.local\n      address: 00:11:22:33:44:55\n    - name: My MacBook Air\n      hostname: My-MacBook-Air.local\n      address: AA:BB:CC:DD:EE:FF\n  applications:\n    - name: iTunes\n      properties:\n        auto_queue: false\n        single_instance: true\n      versions:\n        mac: iTunes.app\n        windows: iTunes.exe\n        linux: null\n    - name: Slack\n      properties:\n        auto_queue: true\n        single_instance: false\n      versions:\n        mac: Slack.app\n        windows: null\n        linux: null\n```\n\nInclude the applications you would like `mine` to manage. Computers are added automatically when `mine` is run.\n\nThe `versions` dictionary identifies the name of the executable on each platform. The `properties.auto_queue` setting indicates `mine` should attempt to launch the application automatically when switching computers. The `properties.single_instance` setting indicates the application must be closed on other computers before another instance can start.\n\n# Usage\n\nTo synchronize the current computer's state:\n\n```sh\n$ mine\n```\n\nTo close applications on remote computers and start them locally:\n\n```sh\n$ mine switch\n```\n\nTo close applications running locally:\n\n```sh\n$ mine close\n```\n\nTo close applications locally and start them on another computer:\n\n```sh\n$ mine switch <name>\n```\n\nTo delete conflicted files in your Dropbox:\n\n```sh\n$ mine clean\n```\n",
-    'author': 'Jace Browning',
-    'author_email': 'jacebrowning@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://pypi.org/project/mine',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

