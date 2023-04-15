# Comparing `tmp/cmdgpt-0.2.4.1.tar.gz` & `tmp/cmdgpt-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmdgpt-0.2.4.1.tar", last modified: Thu Mar 30 09:23:08 2023, max compression
+gzip compressed data, was "cmdgpt-0.2.5.tar", last modified: Sat Apr 15 02:49:19 2023, max compression
```

## Comparing `cmdgpt-0.2.4.1.tar` & `cmdgpt-0.2.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:23:08.881657 cmdgpt-0.2.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-03-30 09:22:48.000000 cmdgpt-0.2.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-03-30 09:23:08.881657 cmdgpt-0.2.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-03-30 09:22:48.000000 cmdgpt-0.2.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:23:08.877657 cmdgpt-0.2.4.1/cmdgpt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 09:22:48.000000 cmdgpt-0.2.4.1/cmdgpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-03-30 09:22:48.000000 cmdgpt-0.2.4.1/cmdgpt/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-03-30 09:22:48.000000 cmdgpt-0.2.4.1/cmdgpt/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-03-30 09:22:48.000000 cmdgpt-0.2.4.1/cmdgpt/openai_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-03-30 09:22:48.000000 cmdgpt-0.2.4.1/cmdgpt/presets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-03-30 09:22:48.000000 cmdgpt-0.2.4.1/cmdgpt/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:23:08.877657 cmdgpt-0.2.4.1/cmdgpt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-03-30 09:23:08.000000 cmdgpt-0.2.4.1/cmdgpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-03-30 09:23:08.000000 cmdgpt-0.2.4.1/cmdgpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 09:23:08.000000 cmdgpt-0.2.4.1/cmdgpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-30 09:23:08.000000 cmdgpt-0.2.4.1/cmdgpt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-30 09:23:08.000000 cmdgpt-0.2.4.1/cmdgpt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-30 09:23:08.000000 cmdgpt-0.2.4.1/cmdgpt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-30 09:23:08.881657 cmdgpt-0.2.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-03-30 09:22:48.000000 cmdgpt-0.2.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:49:19.409025 cmdgpt-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-15 02:49:08.000000 cmdgpt-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-04-15 02:49:19.409025 cmdgpt-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-04-15 02:49:08.000000 cmdgpt-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:49:19.409025 cmdgpt-0.2.5/cmdgpt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 02:49:08.000000 cmdgpt-0.2.5/cmdgpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-04-15 02:49:08.000000 cmdgpt-0.2.5/cmdgpt/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-04-15 02:49:08.000000 cmdgpt-0.2.5/cmdgpt/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-04-15 02:49:08.000000 cmdgpt-0.2.5/cmdgpt/openai_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-04-15 02:49:08.000000 cmdgpt-0.2.5/cmdgpt/presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-04-15 02:49:08.000000 cmdgpt-0.2.5/cmdgpt/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:49:19.409025 cmdgpt-0.2.5/cmdgpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-04-15 02:49:19.000000 cmdgpt-0.2.5/cmdgpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-15 02:49:19.000000 cmdgpt-0.2.5/cmdgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 02:49:19.000000 cmdgpt-0.2.5/cmdgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-15 02:49:19.000000 cmdgpt-0.2.5/cmdgpt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-15 02:49:19.000000 cmdgpt-0.2.5/cmdgpt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-15 02:49:19.000000 cmdgpt-0.2.5/cmdgpt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 02:49:19.409025 cmdgpt-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-04-15 02:49:08.000000 cmdgpt-0.2.5/setup.py
```

### Comparing `cmdgpt-0.2.4.1/LICENSE` & `cmdgpt-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cmdgpt-0.2.4.1/PKG-INFO` & `cmdgpt-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmdgpt
-Version: 0.2.4.1
+Version: 0.2.5
 Summary: Interact with the command line using natural language | 用自然语言操控命令行
 Home-page: https://github.com/MZhao-ouo/CMDGPT
 Author: MZhao
 Author-email: mzhao.ouo@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `cmdgpt-0.2.4.1/README.md` & `cmdgpt-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `cmdgpt-0.2.4.1/cmdgpt/functions.py` & `cmdgpt-0.2.5/cmdgpt/functions.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,37 +12,40 @@
         ]
     response = get_chat_response(messages, temperature=0,apiurl=COMPLETIONS_URL)
     response_contents = decode_chat_response(response)
     try_exec(response_contents)
 
 def try_exec(response_contents):
     cmd = ""
-    print(f"{Fore.BLUE}CMDGPT:{Style.RESET_ALL} Do you want to execute the following command? (y/n):")
+    print(f"{Fore.BLUE}CMDGPT:{Style.RESET_ALL} ")
+    print("Run(R), Cancel(C)", end="", flush=True)
+    print("\x1b[1A\r\x1b[8C", end="")
     for chunk in response_contents:
         print(Fore.YELLOW + chunk + Style.RESET_ALL, end="", flush=True)
         cmd += chunk
-    print()
+    print("\x1b[1B\r\x1b[18C", end="")
     if "MZHAO" in cmd:
-        print(Fore.RED + "Please provide a valuable description." + Style.RESET_ALL)
+        print("\r" + Fore.RED + "Please provide a valuable description." + Style.RESET_ALL)
         return
     if os.name == "nt":
-        print("Please execute it manually in Windows.")
+        print("\r" + "Please execute it manually in Windows.")
         return
     if "\n" in cmd:
-        print("It is a multi-line command. Please execute it manually.")
+        print("\r" + "It is a multi-line command. Please execute it manually.")
         return
     while True:
         pressed_key = get_key()
         if pressed_key:
             pressed_key = pressed_key.lower()
-            if pressed_key == "y":
+            if pressed_key == "r":
+                print("\x1b[1A", end="")
                 os.system(cmd)
                 break
-            elif pressed_key == "n":
-                print("Canceled.")
+            elif pressed_key == "c":
+                print("\rCanceled." + " " * 20)
                 break
 
 # set openai api key
 def set_openai_key(api_key):
     cmdgpt_conf["openai_api_key"] = api_key
     with open(cmdgpt_conf_path, "w+") as f:
         json.dump(cmdgpt_conf, f)
```

### Comparing `cmdgpt-0.2.4.1/cmdgpt/main.py` & `cmdgpt-0.2.5/cmdgpt/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,16 +34,16 @@
     if args.key:
         set_openai_key(args.key)
     if args.api_host:
         set_apihost(args.api_host)
     if args.query:
         exec_query(args.query)
         exit()
-    if args.credit:
-        get_credit(credit_url=CREDIT_URL)
-        exit()
+    # if args.credit:
+    #     get_credit(credit_url=CREDIT_URL)
+    #     exit()
     if args.usage:
         get_usage(usage_url=USAGE_URL, start_date=args.start_date, end_date=args.end_date)
         exit()
 
 if __name__ == "__main__":
     main()
```

### Comparing `cmdgpt-0.2.4.1/cmdgpt/openai_func.py` & `cmdgpt-0.2.5/cmdgpt/openai_func.py`

 * *Files identical despite different names*

### Comparing `cmdgpt-0.2.4.1/cmdgpt/presets.py` & `cmdgpt-0.2.5/cmdgpt/presets.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import requests
 from colorama import Fore, Style
 from .utils import get_cmd_history, load_conf, init_conf
 
 parser = argparse.ArgumentParser(description="description")
 parser.add_argument("query", nargs="?", help="Describe the command you want.", default=None)
 parser.add_argument("--key", type=str, help="api_key", required=False, default=None)
-parser.add_argument("--credit", action="store_true", help="show OpenAI Credit")
+# parser.add_argument("--credit", action="store_true", help="show OpenAI Credit")
 parser.add_argument("--api_host", type=str, help="OpenAI API URL", required=False)
 parser.add_argument("--reset_conf", action="store_true", help="reset the default configuration")
 parser.add_argument("--chat", action="store_true", help="chat with gpt-3.5")
 parser.add_argument("--usage", action="store_true", help="show OpenAI Usage")
 parser.add_argument("--start_date", type=str, help="start date", required=False, default=None)
 parser.add_argument("--end_date", type=str, help="end date", required=False, default=None)
 parser.add_argument('--debug', action='store_true', help='enable debug mode')
```

### Comparing `cmdgpt-0.2.4.1/cmdgpt/utils.py` & `cmdgpt-0.2.5/cmdgpt/utils.py`

 * *Files identical despite different names*

### Comparing `cmdgpt-0.2.4.1/cmdgpt.egg-info/PKG-INFO` & `cmdgpt-0.2.5/cmdgpt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmdgpt
-Version: 0.2.4.1
+Version: 0.2.5
 Summary: Interact with the command line using natural language | 用自然语言操控命令行
 Home-page: https://github.com/MZhao-ouo/CMDGPT
 Author: MZhao
 Author-email: mzhao.ouo@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `cmdgpt-0.2.4.1/setup.py` & `cmdgpt-0.2.5/setup.py`

 * *Files identical despite different names*

