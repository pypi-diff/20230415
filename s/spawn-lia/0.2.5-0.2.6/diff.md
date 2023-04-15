# Comparing `tmp/spawn-lia-0.2.5.tar.gz` & `tmp/spawn-lia-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spawn-lia-0.2.5.tar", last modified: Thu Apr 13 18:24:52 2023, max compression
+gzip compressed data, was "spawn-lia-0.2.6.tar", last modified: Sat Apr 15 20:40:27 2023, max compression
```

## Comparing `spawn-lia-0.2.5.tar` & `spawn-lia-0.2.6.tar`

### file list

```diff
@@ -1,43 +1,45 @@
-drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-13 18:24:52.216154 spawn-lia-0.2.5/
--rw-r--r--   0 developer  (1001) developer  (1001)    34693 2023-04-13 18:24:44.000000 spawn-lia-0.2.5/LICENSE.txt
--rw-r--r--   0 developer  (1001) developer  (1001)     4301 2023-04-13 18:24:52.216154 spawn-lia-0.2.5/PKG-INFO
--rw-r--r--   0 developer  (1001) developer  (1001)     3835 2023-04-07 19:35:39.000000 spawn-lia-0.2.5/README.md
-drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-13 18:24:52.212821 spawn-lia-0.2.5/lia/
--rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-03 18:48:44.000000 spawn-lia-0.2.5/lia/__init__.py
-drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-13 18:24:52.212821 spawn-lia-0.2.5/lia/bounty/
--rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-13 17:54:43.000000 spawn-lia-0.2.5/lia/bounty/__init__.py
--rw-r--r--   0 developer  (1001) developer  (1001)     4815 2023-04-13 18:24:44.000000 spawn-lia-0.2.5/lia/bounty/heal.py
--rw-r--r--   0 developer  (1001) developer  (1001)      553 2023-04-12 17:13:31.000000 spawn-lia-0.2.5/lia/bounty/testing.py
-drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-13 18:24:52.212821 spawn-lia-0.2.5/lia/check_git/
--rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-03 18:48:44.000000 spawn-lia-0.2.5/lia/check_git/__init__.py
--rw-r--r--   0 developer  (1001) developer  (1001)     1486 2023-04-13 18:24:44.000000 spawn-lia-0.2.5/lia/check_git/verify_branch.py
-drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-13 18:24:52.212821 spawn-lia-0.2.5/lia/conversation/
--rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-04 20:03:31.000000 spawn-lia-0.2.5/lia/conversation/__init__.py
--rw-r--r--   0 developer  (1001) developer  (1001)     1003 2023-04-13 18:24:44.000000 spawn-lia-0.2.5/lia/conversation/ask_to_proceed.py
--rw-r--r--   0 developer  (1001) developer  (1001)      104 2023-04-08 09:57:30.000000 spawn-lia-0.2.5/lia/conversation/decision.py
--rw-r--r--   0 developer  (1001) developer  (1001)      873 2023-04-08 10:05:19.000000 spawn-lia-0.2.5/lia/conversation/emojis.py
--rw-r--r--   0 developer  (1001) developer  (1001)      396 2023-04-13 18:24:33.000000 spawn-lia-0.2.5/lia/conversation/end_message.py
--rw-r--r--   0 developer  (1001) developer  (1001)     1026 2023-04-08 10:18:13.000000 spawn-lia-0.2.5/lia/conversation/start_message.py
--rw-r--r--   0 developer  (1001) developer  (1001)     2236 2023-04-12 17:13:06.000000 spawn-lia-0.2.5/lia/conversation/virtualenv.py
--rw-r--r--   0 developer  (1001) developer  (1001)      542 2023-04-12 17:07:04.000000 spawn-lia-0.2.5/lia/main.py
-drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-13 18:24:52.212821 spawn-lia-0.2.5/lia/simplify/
--rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-04 19:56:24.000000 spawn-lia-0.2.5/lia/simplify/__init__.py
--rw-r--r--   0 developer  (1001) developer  (1001)     1774 2023-04-13 18:24:44.000000 spawn-lia-0.2.5/lia/simplify/create_venv.py
--rw-r--r--   0 developer  (1001) developer  (1001)      246 2023-04-03 18:48:44.000000 spawn-lia-0.2.5/lia/simplify/verify_package.py
-drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-13 18:24:52.212821 spawn-lia-0.2.5/lia/support/
--rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-13 17:55:51.000000 spawn-lia-0.2.5/lia/support/__init__.py
--rw-r--r--   0 developer  (1001) developer  (1001)     1256 2023-04-12 17:02:43.000000 spawn-lia-0.2.5/lia/support/deploy.py
--rw-r--r--   0 developer  (1001) developer  (1001)       38 2023-04-13 18:24:52.216154 spawn-lia-0.2.5/setup.cfg
--rw-r--r--   0 developer  (1001) developer  (1001)     1156 2023-04-13 18:24:41.000000 spawn-lia-0.2.5/setup.py
-drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-13 18:24:52.216154 spawn-lia-0.2.5/spawn_lia.egg-info/
--rw-r--r--   0 developer  (1001) developer  (1001)     4301 2023-04-13 18:24:52.000000 spawn-lia-0.2.5/spawn_lia.egg-info/PKG-INFO
--rw-r--r--   0 developer  (1001) developer  (1001)      809 2023-04-13 18:24:52.000000 spawn-lia-0.2.5/spawn_lia.egg-info/SOURCES.txt
--rw-r--r--   0 developer  (1001) developer  (1001)        1 2023-04-13 18:24:52.000000 spawn-lia-0.2.5/spawn_lia.egg-info/dependency_links.txt
--rw-r--r--   0 developer  (1001) developer  (1001)       40 2023-04-13 18:24:52.000000 spawn-lia-0.2.5/spawn_lia.egg-info/entry_points.txt
--rw-r--r--   0 developer  (1001) developer  (1001)       96 2023-04-13 18:24:52.000000 spawn-lia-0.2.5/spawn_lia.egg-info/requires.txt
--rw-r--r--   0 developer  (1001) developer  (1001)        4 2023-04-13 18:24:52.000000 spawn-lia-0.2.5/spawn_lia.egg-info/top_level.txt
-drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-13 18:24:52.216154 spawn-lia-0.2.5/tests/
--rw-r--r--   0 developer  (1001) developer  (1001)      626 2023-04-07 19:00:56.000000 spawn-lia-0.2.5/tests/test_deploy.py
--rw-r--r--   0 developer  (1001) developer  (1001)     3841 2023-04-07 19:00:56.000000 spawn-lia-0.2.5/tests/test_git_check.py
--rw-r--r--   0 developer  (1001) developer  (1001)     1140 2023-04-12 17:06:07.000000 spawn-lia-0.2.5/tests/test_heal.py
--rw-r--r--   0 developer  (1001) developer  (1001)      772 2023-04-08 10:13:59.000000 spawn-lia-0.2.5/tests/test_venv.py
+drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-15 20:40:27.645855 spawn-lia-0.2.6/
+-rw-r--r--   0 developer  (1001) developer  (1001)    34693 2023-04-15 20:40:16.000000 spawn-lia-0.2.6/LICENSE.txt
+-rw-r--r--   0 developer  (1001) developer  (1001)     4301 2023-04-15 20:40:27.642521 spawn-lia-0.2.6/PKG-INFO
+-rw-r--r--   0 developer  (1001) developer  (1001)     3835 2023-04-07 19:35:39.000000 spawn-lia-0.2.6/README.md
+drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-15 20:40:27.642521 spawn-lia-0.2.6/lia/
+-rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-14 19:08:10.000000 spawn-lia-0.2.6/lia/__init__.py
+drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-15 20:40:27.642521 spawn-lia-0.2.6/lia/bounty/
+-rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-14 19:08:10.000000 spawn-lia-0.2.6/lia/bounty/__init__.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     4814 2023-04-15 20:40:16.000000 spawn-lia-0.2.6/lia/bounty/heal.py
+-rw-r--r--   0 developer  (1001) developer  (1001)      554 2023-04-15 20:40:15.000000 spawn-lia-0.2.6/lia/bounty/testing.py
+drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-15 20:40:27.642521 spawn-lia-0.2.6/lia/conversation/
+-rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-14 19:08:10.000000 spawn-lia-0.2.6/lia/conversation/__init__.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     1028 2023-04-15 20:40:16.000000 spawn-lia-0.2.6/lia/conversation/ask_to_proceed.py
+-rw-r--r--   0 developer  (1001) developer  (1001)      103 2023-04-14 19:08:10.000000 spawn-lia-0.2.6/lia/conversation/decision.py
+-rw-r--r--   0 developer  (1001) developer  (1001)      960 2023-04-15 20:40:15.000000 spawn-lia-0.2.6/lia/conversation/emojis.py
+-rw-r--r--   0 developer  (1001) developer  (1001)      395 2023-04-14 19:08:10.000000 spawn-lia-0.2.6/lia/conversation/end_message.py
+-rw-r--r--   0 developer  (1001) developer  (1001)      506 2023-04-15 20:40:15.000000 spawn-lia-0.2.6/lia/conversation/get_input.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     1015 2023-04-14 19:08:10.000000 spawn-lia-0.2.6/lia/conversation/start_message.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     2218 2023-04-14 19:08:10.000000 spawn-lia-0.2.6/lia/conversation/virtualenv.py
+drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-15 20:40:27.642521 spawn-lia-0.2.6/lia/git_operations/
+-rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-14 19:08:10.000000 spawn-lia-0.2.6/lia/git_operations/__init__.py
+-rw-r--r--   0 developer  (1001) developer  (1001)      974 2023-04-15 20:40:16.000000 spawn-lia-0.2.6/lia/git_operations/push.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     1486 2023-04-15 20:40:16.000000 spawn-lia-0.2.6/lia/git_operations/verify_branch.py
+-rw-r--r--   0 developer  (1001) developer  (1001)      608 2023-04-15 20:40:15.000000 spawn-lia-0.2.6/lia/main.py
+drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-15 20:40:27.642521 spawn-lia-0.2.6/lia/simplify/
+-rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-14 19:08:10.000000 spawn-lia-0.2.6/lia/simplify/__init__.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     1768 2023-04-15 20:40:16.000000 spawn-lia-0.2.6/lia/simplify/create_venv.py
+-rw-r--r--   0 developer  (1001) developer  (1001)      246 2023-04-14 19:08:10.000000 spawn-lia-0.2.6/lia/simplify/verify_package.py
+drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-15 20:40:27.642521 spawn-lia-0.2.6/lia/support/
+-rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-14 19:08:10.000000 spawn-lia-0.2.6/lia/support/__init__.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     1260 2023-04-15 19:23:40.000000 spawn-lia-0.2.6/lia/support/deploy.py
+-rw-r--r--   0 developer  (1001) developer  (1001)       38 2023-04-15 20:40:27.645855 spawn-lia-0.2.6/setup.cfg
+-rw-r--r--   0 developer  (1001) developer  (1001)     1156 2023-04-15 20:40:08.000000 spawn-lia-0.2.6/setup.py
+drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-15 20:40:27.642521 spawn-lia-0.2.6/spawn_lia.egg-info/
+-rw-r--r--   0 developer  (1001) developer  (1001)     4301 2023-04-15 20:40:27.000000 spawn-lia-0.2.6/spawn_lia.egg-info/PKG-INFO
+-rw-r--r--   0 developer  (1001) developer  (1001)      894 2023-04-15 20:40:27.000000 spawn-lia-0.2.6/spawn_lia.egg-info/SOURCES.txt
+-rw-r--r--   0 developer  (1001) developer  (1001)        1 2023-04-15 20:40:27.000000 spawn-lia-0.2.6/spawn_lia.egg-info/dependency_links.txt
+-rw-r--r--   0 developer  (1001) developer  (1001)       40 2023-04-15 20:40:27.000000 spawn-lia-0.2.6/spawn_lia.egg-info/entry_points.txt
+-rw-r--r--   0 developer  (1001) developer  (1001)       96 2023-04-15 20:40:27.000000 spawn-lia-0.2.6/spawn_lia.egg-info/requires.txt
+-rw-r--r--   0 developer  (1001) developer  (1001)        4 2023-04-15 20:40:27.000000 spawn-lia-0.2.6/spawn_lia.egg-info/top_level.txt
+drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-15 20:40:27.642521 spawn-lia-0.2.6/tests/
+-rw-r--r--   0 developer  (1001) developer  (1001)      626 2023-04-07 19:00:56.000000 spawn-lia-0.2.6/tests/test_deploy.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     5008 2023-04-15 20:39:34.000000 spawn-lia-0.2.6/tests/test_git_operations.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     1140 2023-04-12 17:06:07.000000 spawn-lia-0.2.6/tests/test_heal.py
+-rw-r--r--   0 developer  (1001) developer  (1001)      885 2023-04-15 20:39:34.000000 spawn-lia-0.2.6/tests/test_venv.py
```

### Comparing `spawn-lia-0.2.5/LICENSE.txt` & `spawn-lia-0.2.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `spawn-lia-0.2.5/PKG-INFO` & `spawn-lia-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spawn-lia
-Version: 0.2.5
+Version: 0.2.6
 Summary: The most wanted support
 Home-page: https://codeberg.org/cap_jmk/lia
 Author: Julian M. Kleber
 Author-email: julian.kleber@sail.black
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `spawn-lia-0.2.5/README.md` & `spawn-lia-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `spawn-lia-0.2.5/lia/bounty/heal.py` & `spawn-lia-0.2.6/lia/bounty/heal.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
-"""
-Module for python file bug revealing functionality 
+"""Module for python file bug revealing functionality.
 
 :author: Julian M. Kleber
 """
 import os
 import subprocess
 import click
 
 from lia.conversation.end_message import say_end_message
 from lia.conversation.start_message import say_start_message
 
-from lia.check_git.verify_branch import verify_branch
+from lia.git_operations.verify_branch import verify_branch
 
 from lia.bounty.testing import test_package
 
 
 @click.command()
 @click.argument("packagename")
 @click.option("-t", default="y", help="If test should be run")
@@ -57,20 +56,19 @@
 
     say_end_message()
 
 
 @click.command(name="heal-file")
 @click.argument("file_name")
 def heal_file(file_name: str) -> None:
-    """
-    The heal_file function is a wrapper for the bounty_routine function.
-    It is designed to be called from the command line, and it takes one argument:
-    the name of a file in your repository that you want to heal. It will then run
-    the bounty_routine on that file, which will check out all commits where that
-    file was changed and attempt to fix any errors found by flake8.
+    """The heal_file function is a wrapper for the bounty_routine function. It
+    is designed to be called from the command line, and it takes one argument:
+    the name of a file in your repository that you want to heal. It will then
+    run the bounty_routine on that file, which will check out all commits where
+    that file was changed and attempt to fix any errors found by flake8.
 
     :param file_name:str: Used to specify the name of the file that is being healed.
     :return: Nothing.
 
     :doc-author: Julian M. Kleber
     """
```

### Comparing `spawn-lia-0.2.5/lia/bounty/testing.py` & `spawn-lia-0.2.6/lia/bounty/testing.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,20 @@
-"""
-Module to execute automatized tests
+"""Module to execute automatized tests.
 
 :author: Julian M. Kleber
-
 """
 import subprocess
 
 
 def test_package() -> None:
-    """
-    The test_package function is used to test the package.
-    It is called by the main function if the user chooses to run tests.
-    The function uses subprocess and pytest to run all of our tests in a single command.
+    """The test_package function is used to test the package. It is called by
+    the main function if the user chooses to run tests. The function uses
+    subprocess and pytest to run all of our tests in a single command.
 
-    :return: Nothing.
+    :return: Julian M. Kleber
 
     :doc-author: Julian M. Kleber
     """
-
     try:
         subprocess.run(["python -m pytest tests/"], shell=True, check=True)
     except Exception as exc:
         print(str(exc))
```

### Comparing `spawn-lia-0.2.5/lia/check_git/verify_branch.py` & `spawn-lia-0.2.6/lia/git_operations/verify_branch.py`

 * *Files identical despite different names*

### Comparing `spawn-lia-0.2.5/lia/conversation/ask_to_proceed.py` & `spawn-lia-0.2.6/lia/conversation/ask_to_proceed.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,29 +8,29 @@
 from lia.conversation.emojis import (
     fearful_face,
     pensive_face,
     magic_wand,
     kissing_cat,
     face_with_rolling_eyes,
 )
+from lia.conversation.get_input import get_input
 
 
 def ask_to_proceed() -> None:
     """The ask_to_proceed function asks the user if they want to proceed with
     the script. If they answer 'y', then it will continue. If they answer 'n',
     then it will exit.
 
     :return: None.
 
     :doc-author: Julian M. Kleber
     """
 
-    answer = input(
+    answer = get_input(
         f"Are you sure that you want to proceed {fearful_face}? (y/n)\n")
-    answer = answer.lower()
 
     if answer == "n":
         echo(f"Okay, I guess you got this... {pensive_face}")
     elif answer == "y":
         echo(f"Good decision, darling {magic_wand} {kissing_cat}")
         sys.exit()
     else:
```

### Comparing `spawn-lia-0.2.5/lia/conversation/emojis.py` & `spawn-lia-0.2.6/lia/conversation/emojis.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,36 @@
 """This is an emoji map for usage in shell outputs.
 
 :author: Julian M. Kleber
 """
 from emoji import emojize
 
 
+# faces
+
 angered_face = emojize(":enraged_face:")
+face_with_hearts = emojize(":smiling_face_with_hearts:")
 face_blowing_kiss = emojize(":face_blowing_a_kiss:")
 fearful_face = emojize(":fearful_face:")
 face_screaming_in_fear = emojize(":face_screaming_in_fear:")
-magic_wand = emojize(":magic_wand:")
 pensive_face = emojize(":pensive_face:")
-kissing_cat = emojize(":kissing_cat:")
 face_with_rolling_eyes = emojize(":face_with_rolling_eyes:")
+
+# cat
+kissing_cat = emojize(":kissing_cat:")
+
+
+# utilities
+magic_wand = emojize(":magic_wand:")
 anatomical_heart = emojize(":anatomical_heart:")
 mechanical_arm = emojize(":mechanical_arm:")
-call_me_hand = emojize(":call_me_hand:")
 sailing_ship = emojize(":sailboat:")
 broken_heart = emojize(":broken_heart:")
 
 # gestures
 
 pointing_down = emojize(":backhand_index_pointing_down:")
 pointing_right = emojize(":backhand_index_pointing_right:")
+call_me_hand = emojize(":call_me_hand:")
 # fancy effects
 
 dizzy = emojize(":dizzy:")
```

### Comparing `spawn-lia-0.2.5/lia/conversation/start_message.py` & `spawn-lia-0.2.6/lia/conversation/start_message.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-"""
-Module for start messages 
+"""Module for start messages.
 
 :author: Julian M. Kleber
 """
 
 from click import echo
 
 from lia.conversation.emojis import (
@@ -11,31 +10,29 @@
     call_me_hand,
     sailing_ship,
     anatomical_heart,
 )
 
 
 def say_start_message() -> None:
-    """
-    The say_start_message function prints a message to the console that welcomes the user and
-    explains how to use this program.
+    """The say_start_message function prints a message to the console that
+    welcomes the user and explains how to use this program.
 
     :return: None
 
     :doc-author: Julian M. Kleber
     """
 
     message = standard_message()
     echo(message=message)
 
 
 def standard_message() -> str:
-    """
-    The standard_message function returns a string that is the standard message
-    that Lia prints to the console when it starts up.
+    """The standard_message function returns a string that is the standard
+    message that Lia prints to the console when it starts up.
 
     :return: A string.
 
     :doc-author: Julian M. Kleber
     """
 
     message = (
```

### Comparing `spawn-lia-0.2.5/lia/conversation/virtualenv.py` & `spawn-lia-0.2.6/lia/conversation/virtualenv.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-"""
-Conversation about the virtualenv method
+"""Conversation about the virtualenv method.
 
 :author: Julian M. Kleber
 """
 
 import sys
 import subprocess
 from click import echo
@@ -17,16 +16,15 @@
     broken_heart,
     dizzy,
     pensive_face,
 )
 
 
 def is_activated(venv_path: str) -> str:
-    """
-    The is_activated function checks if a virtualenv is already activated.
+    """The is_activated function checks if a virtualenv is already activated.
     If so, it returns a message with the path to the venv.
 
     :param venv_path:str: Used to pass the path of the venv to be deactivated.
     :return: The message for the CLI tool.
 
     :doc-author: Julian M. Kleber
     """
@@ -43,18 +41,17 @@
 
 def shall_i_deactivate(
     venv_path: str,
 ) -> (
     None
 ):  # TODO: Experimental feature -> handling the shells a bit difficult, deactivate must be run
     # in the same shell
-    """
-    The shall_i_deactivate function asks the user if they want to deactivate their virtualenv.
-        If the answer is 'y', then it will run a subprocess that runs "deactivate" in the shell.
-        If not, it will exit with an error message.
+    """The shall_i_deactivate function asks the user if they want to deactivate
+    their virtualenv. If the answer is 'y', then it will run a subprocess that
+    runs "deactivate" in the shell. If not, it will exit with an error message.
 
     :return: None.
 
     :doc-author: Julian M. Kleber
     """
 
     venv_path = append_slash(venv_path) + "bin/activate"
```

### Comparing `spawn-lia-0.2.5/lia/main.py` & `spawn-lia-0.2.6/lia/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import click
 
 
 # spells
 from lia.bounty.heal import heal, heal_file
 from lia.support.deploy import deploy
 from lia.simplify.create_venv import create_venv
+from lia.git_operations.push import push
 
 
 @click.group()
 def spells() -> None:
     """Collection for Lia's spells.
 
     For more info ask for help on each specific spell.
@@ -20,10 +21,11 @@
     pass  # pragma: no cover
 
 
 spells.add_command(heal)
 spells.add_command(heal_file)
 spells.add_command(deploy)
 spells.add_command(create_venv)
+spells.add_command(push)
 
 if __name__ == "__main__":
     spells()
```

### Comparing `spawn-lia-0.2.5/lia/simplify/create_venv.py` & `spawn-lia-0.2.6/lia/simplify/create_venv.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-"""
-Helping with venv operations to avoid confusions
+"""Helping with venv operations to avoid confusions.
 
 :author: Julian M. Kleber
 """
 
 import subprocess
 from amarium.utils import append_slash
 import click
@@ -11,20 +10,19 @@
 
 from lia.conversation.virtualenv import is_activated
 
 
 @click.command()
 @click.argument("directory")
 def create_venv(directory: str) -> None:
-    """
-    The create_venv function creates a virtual environment in the directory
+    """The create_venv function creates a virtual environment in the directory
     specified by the user. It first checks to see if there is an active virtual
-    environment, and if so, it asks the user whether they would like to deactivate
-    it before creating a new one. If not, it creates a new venv called "venv" in
-    the specified directory.
+    environment, and if so, it asks the user whether they would like to
+    deactivate it before creating a new one. If not, it creates a new venv
+    called "venv" in the specified directory.
 
     :param directory: Used to Create a virtual environment in the.
     :return: None.
 
     :doc-author: Julian M. Kleber
     """
 
@@ -39,17 +37,17 @@
     venv_name = append_slash(directory) + "venv"
     subprocess.run([f"python3 -m venv {venv_name}"], shell=True, check=True)
     subprocess.run([f"source {venv_name}/bin/activate"],
                    shell=True, check=True)
 
 
 def check_venv() -> bytes:
-    """
-    The check_venv function checks to see if the user is in a virtual environment.
-    If they are, it returns the path to that virtual environment. If not, it raises an error.
+    """The check_venv function checks to see if the user is in a virtual
+    environment. If they are, it returns the path to that virtual environment.
+    If not, it raises an error.
 
     :return: A byte string.
 
     :doc-author: Julian M. Kleber
     """
 
     out = subprocess.run(
```

### Comparing `spawn-lia-0.2.5/lia/support/deploy.py` & `spawn-lia-0.2.6/lia/support/deploy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-"""
-Module for deployment functionality 
+"""Module for deployment functionality.
 
 :author: Julian M. Kleber
 """
 import subprocess
 import os
 
 import click
 from click import echo
 
 from lia.conversation.end_message import say_end_message
 from lia.conversation.start_message import say_start_message
-from lia.check_git.verify_branch import verify_branch
+from lia.git_operations.verify_branch import verify_branch
 
 
 @click.command()
 @click.option("-t", default="y", help="If test should be run")
 def deploy(t: str) -> None:
     """Deployment routine.
```

### Comparing `spawn-lia-0.2.5/setup.py` & `spawn-lia-0.2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setup(
     name="spawn-lia",
-    version="0.2.5",
+    version="0.2.6",
     packages=find_packages(include=["lia*"]),
     include_package_data=True,
     install_requires=[
         "Click",
         "black",
         "autopep8",
         "mypy",
```

### Comparing `spawn-lia-0.2.5/spawn_lia.egg-info/PKG-INFO` & `spawn-lia-0.2.6/spawn_lia.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spawn-lia
-Version: 0.2.5
+Version: 0.2.6
 Summary: The most wanted support
 Home-page: https://codeberg.org/cap_jmk/lia
 Author: Julian M. Kleber
 Author-email: julian.kleber@sail.black
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `spawn-lia-0.2.5/spawn_lia.egg-info/SOURCES.txt` & `spawn-lia-0.2.6/spawn_lia.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 LICENSE.txt
 README.md
 setup.py
 lia/__init__.py
 lia/main.py
+lia/utils.py
 lia/bounty/__init__.py
 lia/bounty/heal.py
 lia/bounty/testing.py
-lia/check_git/__init__.py
-lia/check_git/verify_branch.py
 lia/conversation/__init__.py
 lia/conversation/ask_to_proceed.py
 lia/conversation/decision.py
 lia/conversation/emojis.py
 lia/conversation/end_message.py
+lia/conversation/get_input.py
 lia/conversation/start_message.py
 lia/conversation/virtualenv.py
+lia/git_operations/__init__.py
+lia/git_operations/push.py
+lia/git_operations/verify_branch.py
 lia/simplify/__init__.py
 lia/simplify/create_venv.py
 lia/simplify/verify_package.py
 lia/support/__init__.py
 lia/support/deploy.py
 spawn_lia.egg-info/PKG-INFO
 spawn_lia.egg-info/SOURCES.txt
 spawn_lia.egg-info/dependency_links.txt
 spawn_lia.egg-info/entry_points.txt
 spawn_lia.egg-info/requires.txt
 spawn_lia.egg-info/top_level.txt
 tests/test_deploy.py
-tests/test_git_check.py
+tests/test_git_operations.py
 tests/test_heal.py
 tests/test_venv.py
```

### Comparing `spawn-lia-0.2.5/tests/test_deploy.py` & `spawn-lia-0.2.6/tests/test_deploy.py`

 * *Files identical despite different names*

### Comparing `spawn-lia-0.2.5/tests/test_git_check.py` & `spawn-lia-0.2.6/tests/test_git_operations.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import subprocess
 from subprocess import Popen, PIPE
 from lia.conversation import ask_to_proceed
-from lia.check_git import verify_branch
+from lia.git_operations import verify_branch
 
 
 def test_verify_branch():
     # case 1
 
     out = subprocess.Popen(
         ["python", "./lia/conversation/ask_to_proceed.py"], stdin=PIPE, stdout=PIPE
@@ -54,17 +54,17 @@
     try:
         subprocess.run(["git checkout -b dev"], check=True, shell=True)
     except:
         print("branch already exists")
     finally:
         subprocess.run(["git checkout dev"], check=True, shell=True)
     out = subprocess.Popen(
-        ["python", "./lia/check_git/verify_branch.py"], stdin=PIPE, stdout=PIPE
+        ["python", "./lia/git_operations/verify_branch.py"], stdin=PIPE, stdout=PIPE
     )
-    # out.stdin.write(b"y\n")
+   
     outputlog, errorlog = out.communicate()
     out.stdin.close()
     assert (
         outputlog
         == b"It seems like you are on a good branch.\nThe way is free for you to go ahead \xf0\x9f\xaa\x84 \xf0\x9f\x98\xbd\n"
     )
     assert errorlog is None
@@ -73,15 +73,15 @@
     try:
         subprocess.run(["git checkout -b master"], check=True, shell=True)
     except:
         print("branch already exists")
     finally:
         subprocess.run(["git checkout master"], check=True, shell=True)
     out = subprocess.Popen(
-        ["python", "./lia/check_git/verify_branch.py"], stdin=PIPE, stdout=PIPE
+        ["python", "./lia/git_operations/verify_branch.py"], stdin=PIPE, stdout=PIPE
     )
     out.stdin.write(b"y\n")
     outputlog, errorlog = out.communicate()
     out.stdin.close()
 
     assert (
         outputlog
@@ -96,19 +96,48 @@
     """try:
         subprocess.run(["git checkout -b main"], check=True, shell=True)
     except: 
         print("branch already exists")
     finally: 
         subprocess.run(["git checkout main"], check=True, shell=True)
     out = subprocess.Popen(
-        ["python", "./lia/check_git/verify_branch.py"], stdin=PIPE, stdout=PIPE
+        ["python", "./lia/git_operations/verify_branch.py"], stdin=PIPE, stdout=PIPE
     )
     out.stdin.write(b"y\n")
     outputlog, errorlog = out.communicate()
     out.stdin.close()
 
     assert 1 == 2, str(outputlog)
     assert outputlog == b"We don't use master branches any longer \xf0\x9f\x98\xa1\nPlease rename the branch, darling \xf0\x9f\x98\x98\n"
     assert errorlog is None
 
     subprocess.run(["git checkout dev"], shell=True, check=True)
    """  # -> can only implement after merge
+
+def test_push(): 
+
+    #switch to temporary branch to avoid contaminations
+    out = subprocess.run(["git status"], check=True, shell=True, capture_output=True)
+    out2 = subprocess.run(["git branch"], check=True, shell=True, capture_output=True)
+    if b"On branch test_branch" not in out.stdout:
+        if "test_branch" not in out2.stdout.decode("utf-8"):
+            subprocess.run(["git checkout -b test_branch"], check=True, shell=True)
+        else: 
+            subprocess.run(["git checkout test_branch"], check=True, shell=True)
+
+    out = subprocess.Popen(
+        ["lia", "push"], stdin=PIPE, stdout=PIPE
+    )
+
+    out.stdin.write(b"push done by test\n")
+    outputlog, errorlog = out.communicate()
+
+    out.stdin.close()
+    assert 1 == 2, outputlog +" - " + errorlog
+    subprocess.run["git checkout dev"]
+    out = subprocess.Popen(
+        ["python", "./lia/git_operations/verify_branch.py"], stdin=PIPE, stdout=PIPE
+    )
+    
+    outputlog, errorlog = out.communicate()
+    out.stdin.close()
+    assert outputlog == b"You are on the master branch but we agreed to only use main... \xf0\x9f\x98\xa1\nPlease rename the branch, darling \xf0\x9f\x98\x98\n"
```

### Comparing `spawn-lia-0.2.5/tests/test_heal.py` & `spawn-lia-0.2.6/tests/test_heal.py`

 * *Files identical despite different names*

### Comparing `spawn-lia-0.2.5/tests/test_venv.py` & `spawn-lia-0.2.6/tests/test_venv.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import os
 import subprocess
 
 
 def test_creating_venv_func():
     # prepare
-
-    # no venv actiavated
+    if os.path.isdir("tests/test_venv"):
+        subprocess.run(["rm -r tests/test_venv"], shell=True, check=True)
+    # no venv activated
     out = subprocess.run(
         ["lia create-venv tests/test_venv"], shell=True, check=True, capture_output=True
     )
     assert "venv" in os.listdir("tests/test_venv")
     # venv activated
     out = subprocess.run(
         ["lia create-venv tests/test_venv"], shell=True, check=True, capture_output=True
```

