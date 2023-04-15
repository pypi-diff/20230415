# Comparing `tmp/EdgeGPT-0.1.8.tar.gz` & `tmp/EdgeGPT-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EdgeGPT-0.1.8.tar", last modified: Fri Mar 24 10:23:53 2023, max compression
+gzip compressed data, was "EdgeGPT-0.1.9.tar", last modified: Sat Mar 25 02:59:03 2023, max compression
```

## Comparing `EdgeGPT-0.1.8.tar` & `EdgeGPT-0.1.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 10:23:53.600009 EdgeGPT-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-03-24 10:23:42.000000 EdgeGPT-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6350 2023-03-24 10:23:53.600009 EdgeGPT-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-03-24 10:23:42.000000 EdgeGPT-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-24 10:23:53.600009 EdgeGPT-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-03-24 10:23:42.000000 EdgeGPT-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 10:23:53.600009 EdgeGPT-0.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 10:23:53.600009 EdgeGPT-0.1.8/src/EdgeGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6350 2023-03-24 10:23:53.000000 EdgeGPT-0.1.8/src/EdgeGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-03-24 10:23:53.000000 EdgeGPT-0.1.8/src/EdgeGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 10:23:53.000000 EdgeGPT-0.1.8/src/EdgeGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-03-24 10:23:53.000000 EdgeGPT-0.1.8/src/EdgeGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-24 10:23:53.000000 EdgeGPT-0.1.8/src/EdgeGPT.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    15265 2023-03-24 10:23:42.000000 EdgeGPT-0.1.8/src/EdgeGPT.py
--rw-r--r--   0 runner    (1001) docker     (123)     4637 2023-03-24 10:23:42.000000 EdgeGPT-0.1.8/src/ImageGen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 02:59:03.517855 EdgeGPT-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-03-25 02:58:41.000000 EdgeGPT-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6351 2023-03-25 02:59:03.517855 EdgeGPT-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5586 2023-03-25 02:58:41.000000 EdgeGPT-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-25 02:59:03.521855 EdgeGPT-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-03-25 02:58:41.000000 EdgeGPT-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 02:59:03.517855 EdgeGPT-0.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 02:59:03.517855 EdgeGPT-0.1.9/src/EdgeGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6351 2023-03-25 02:59:03.000000 EdgeGPT-0.1.9/src/EdgeGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-03-25 02:59:03.000000 EdgeGPT-0.1.9/src/EdgeGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-25 02:59:03.000000 EdgeGPT-0.1.9/src/EdgeGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-03-25 02:59:03.000000 EdgeGPT-0.1.9/src/EdgeGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-25 02:59:03.000000 EdgeGPT-0.1.9/src/EdgeGPT.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    15462 2023-03-25 02:58:41.000000 EdgeGPT-0.1.9/src/EdgeGPT.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4637 2023-03-25 02:58:41.000000 EdgeGPT-0.1.9/src/ImageGen.py
```

### Comparing `EdgeGPT-0.1.8/LICENSE` & `EdgeGPT-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `EdgeGPT-0.1.8/PKG-INFO` & `EdgeGPT-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: EdgeGPT
-Version: 0.1.8
+Version: 0.1.9
 Summary: Reverse engineered Edge Chat API
 Home-page: https://github.com/acheong08/EdgeGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/issues/new
-Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
+Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
@@ -52,15 +52,15 @@
   <summary>
 
 ### Checking access (Required)
 
   </summary>
 
 - Install the latest version of Microsoft Edge
-- Alternatively, you can use any browser and set the user-agent to look like you're using Edge (e.g., `Mozilla/5.0 (Windows NT 10.0) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/109.0.0.0 Safari/537.36 Edg/109.0.1474.0`). You can do this easily with an extension like "User-Agent Switcher and Manager" for [Chrome](https://chrome.google.com/webstore/detail/user-agent-switcher-and-m/bhchdcejhohfmigjafbampogmaanbfkg) and [Firefox](https://addons.mozilla.org/en-US/firefox/addon/user-agent-string-switcher/).
+- Alternatively, you can use any browser and set the user-agent to look like you're using Edge (e.g., `Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 Safari/537.36 Edg/111.0.1661.51`). You can do this easily with an extension like "User-Agent Switcher and Manager" for [Chrome](https://chrome.google.com/webstore/detail/user-agent-switcher-and-m/bhchdcejhohfmigjafbampogmaanbfkg) and [Firefox](https://addons.mozilla.org/en-US/firefox/addon/user-agent-string-switcher/).
 - Open [bing.com/chat](https://bing.com/chat)
 - If you see a chat feature, you are good to go
 
 </details>
 
 <details>
   <summary>
```

#### html2text {}

```diff
@@ -1,36 +1,35 @@
-Metadata-Version: 2.1 Name: EdgeGPT Version: 0.1.8 Summary: Reverse engineered
+Metadata-Version: 2.1 Name: EdgeGPT Version: 0.1.9 Summary: Reverse engineered
 Edge Chat API Home-page: https://github.com/acheong08/EdgeGPT Author: Antonio
 Cheong Author-email: acheong@student.dalat.org License: GNU General Public
 License v2.0 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/
-issues/new Classifier: License :: OSI Approved :: GNU General Public License v2
-(GPLv2) Classifier: Intended Audience :: Developers Classifier: Topic ::
-Software Development :: Libraries :: Python Modules Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Description-Content-Type: text/markdown License-
-File: LICENSE
+issues/new Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
+Classifier: Intended Audience :: Developers Classifier: Topic :: Software
+Development :: Libraries :: Python Modules Classifier: Programming Language ::
+Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Description-Content-Type: text/markdown License-File: LICENSE
    [EdgeGPT] # Edge GPT _The reverse engineering the chat feature of the new
                                version of Bing_
                         [PyPI_version] [Python version]
 --- ## Setup ### Install package ```bash python3 -m pip install EdgeGPT --
 upgrade ``` ### Requirements - python 3.8+ - A Microsoft Account with early
 access to
 bing.com/chat> (Required)   ### Checking access (Required)  - Install the
 latest version of Microsoft Edge - Alternatively, you can use any browser and
 set the user-agent to look like you're using Edge (e.g., `Mozilla/5.0 (Windows
-NT 10.0) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/109.0.0.0 Safari/537.36
-Edg/109.0.1474.0`). You can do this easily with an extension like "User-Agent
-Switcher and Manager" for [Chrome](https://chrome.google.com/webstore/detail/
-user-agent-switcher-and-m/bhchdcejhohfmigjafbampogmaanbfkg) and [Firefox]
-(https://addons.mozilla.org/en-US/firefox/addon/user-agent-string-switcher/). -
-Open [bing.com/chat](https://bing.com/chat) - If you see a chat feature, you
-are good to go    ### Getting authentication (Required)  - Install the cookie
-editor extension for [Chrome](https://chrome.google.com/webstore/detail/cookie-
-editor/hlkenndednhfkekhgcdicdfddnkalmdm) or [Firefox](https://
+NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0
+Safari/537.36 Edg/111.0.1661.51`). You can do this easily with an extension
+like "User-Agent Switcher and Manager" for [Chrome](https://chrome.google.com/
+webstore/detail/user-agent-switcher-and-m/bhchdcejhohfmigjafbampogmaanbfkg) and
+[Firefox](https://addons.mozilla.org/en-US/firefox/addon/user-agent-string-
+switcher/). - Open [bing.com/chat](https://bing.com/chat) - If you see a chat
+feature, you are good to go    ### Getting authentication (Required)  - Install
+the cookie editor extension for [Chrome](https://chrome.google.com/webstore/
+detail/cookie-editor/hlkenndednhfkekhgcdicdfddnkalmdm) or [Firefox](https://
 addons.mozilla.org/en-US/firefox/addon/cookie-editor/) - Go to `bing.com` -
 Open the extension - Click "Export" on the bottom right (This saves your
 cookies to clipboard) - Paste your cookies into a file `cookies.json`    ##
 Chatbot  ## Usage ### Quick start ``` $ python3 -m EdgeGPT -h EdgeGPT - A demo
 of reverse engineering the Bing GPT chatbot Repo: github.com/acheong08/EdgeGPT
 By: Antonio Cheong !help for help Type !exit to exit Enter twice to send
 message or set --enter-once to send one line message usage: EdgeGPT.py [-h] [--
```

### Comparing `EdgeGPT-0.1.8/README.md` & `EdgeGPT-0.1.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
   <summary>
 
 ### Checking access (Required)
 
   </summary>
 
 - Install the latest version of Microsoft Edge
-- Alternatively, you can use any browser and set the user-agent to look like you're using Edge (e.g., `Mozilla/5.0 (Windows NT 10.0) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/109.0.0.0 Safari/537.36 Edg/109.0.1474.0`). You can do this easily with an extension like "User-Agent Switcher and Manager" for [Chrome](https://chrome.google.com/webstore/detail/user-agent-switcher-and-m/bhchdcejhohfmigjafbampogmaanbfkg) and [Firefox](https://addons.mozilla.org/en-US/firefox/addon/user-agent-string-switcher/).
+- Alternatively, you can use any browser and set the user-agent to look like you're using Edge (e.g., `Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 Safari/537.36 Edg/111.0.1661.51`). You can do this easily with an extension like "User-Agent Switcher and Manager" for [Chrome](https://chrome.google.com/webstore/detail/user-agent-switcher-and-m/bhchdcejhohfmigjafbampogmaanbfkg) and [Firefox](https://addons.mozilla.org/en-US/firefox/addon/user-agent-string-switcher/).
 - Open [bing.com/chat](https://bing.com/chat)
 - If you see a chat feature, you are good to go
 
 </details>
 
 <details>
   <summary>
```

### Comparing `EdgeGPT-0.1.8/setup.py` & `EdgeGPT-0.1.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_packages
 from setuptools import setup
 
 setup(
     name="EdgeGPT",
-    version="0.1.8",
+    version="0.1.9",
     license="GNU General Public License v2.0",
     author="Antonio Cheong",
     author_email="acheong@student.dalat.org",
     description="Reverse engineered Edge Chat API",
     packages=find_packages("src"),
     package_dir={"": "src"},
     url="https://github.com/acheong08/EdgeGPT",
@@ -21,15 +21,15 @@
         "regex",
         "requests",
     ],
     long_description=open("README.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     py_modules=["EdgeGPT", "ImageGen"],
     classifiers=[
-        "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
+        "License :: OSI Approved :: The Unlicense (Unlicense)",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
     ],
```

### Comparing `EdgeGPT-0.1.8/src/EdgeGPT.egg-info/PKG-INFO` & `EdgeGPT-0.1.9/src/EdgeGPT.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: EdgeGPT
-Version: 0.1.8
+Version: 0.1.9
 Summary: Reverse engineered Edge Chat API
 Home-page: https://github.com/acheong08/EdgeGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/issues/new
-Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
+Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
@@ -52,15 +52,15 @@
   <summary>
 
 ### Checking access (Required)
 
   </summary>
 
 - Install the latest version of Microsoft Edge
-- Alternatively, you can use any browser and set the user-agent to look like you're using Edge (e.g., `Mozilla/5.0 (Windows NT 10.0) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/109.0.0.0 Safari/537.36 Edg/109.0.1474.0`). You can do this easily with an extension like "User-Agent Switcher and Manager" for [Chrome](https://chrome.google.com/webstore/detail/user-agent-switcher-and-m/bhchdcejhohfmigjafbampogmaanbfkg) and [Firefox](https://addons.mozilla.org/en-US/firefox/addon/user-agent-string-switcher/).
+- Alternatively, you can use any browser and set the user-agent to look like you're using Edge (e.g., `Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 Safari/537.36 Edg/111.0.1661.51`). You can do this easily with an extension like "User-Agent Switcher and Manager" for [Chrome](https://chrome.google.com/webstore/detail/user-agent-switcher-and-m/bhchdcejhohfmigjafbampogmaanbfkg) and [Firefox](https://addons.mozilla.org/en-US/firefox/addon/user-agent-string-switcher/).
 - Open [bing.com/chat](https://bing.com/chat)
 - If you see a chat feature, you are good to go
 
 </details>
 
 <details>
   <summary>
```

#### html2text {}

```diff
@@ -1,36 +1,35 @@
-Metadata-Version: 2.1 Name: EdgeGPT Version: 0.1.8 Summary: Reverse engineered
+Metadata-Version: 2.1 Name: EdgeGPT Version: 0.1.9 Summary: Reverse engineered
 Edge Chat API Home-page: https://github.com/acheong08/EdgeGPT Author: Antonio
 Cheong Author-email: acheong@student.dalat.org License: GNU General Public
 License v2.0 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/
-issues/new Classifier: License :: OSI Approved :: GNU General Public License v2
-(GPLv2) Classifier: Intended Audience :: Developers Classifier: Topic ::
-Software Development :: Libraries :: Python Modules Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Description-Content-Type: text/markdown License-
-File: LICENSE
+issues/new Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
+Classifier: Intended Audience :: Developers Classifier: Topic :: Software
+Development :: Libraries :: Python Modules Classifier: Programming Language ::
+Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Description-Content-Type: text/markdown License-File: LICENSE
    [EdgeGPT] # Edge GPT _The reverse engineering the chat feature of the new
                                version of Bing_
                         [PyPI_version] [Python version]
 --- ## Setup ### Install package ```bash python3 -m pip install EdgeGPT --
 upgrade ``` ### Requirements - python 3.8+ - A Microsoft Account with early
 access to
 bing.com/chat> (Required)   ### Checking access (Required)  - Install the
 latest version of Microsoft Edge - Alternatively, you can use any browser and
 set the user-agent to look like you're using Edge (e.g., `Mozilla/5.0 (Windows
-NT 10.0) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/109.0.0.0 Safari/537.36
-Edg/109.0.1474.0`). You can do this easily with an extension like "User-Agent
-Switcher and Manager" for [Chrome](https://chrome.google.com/webstore/detail/
-user-agent-switcher-and-m/bhchdcejhohfmigjafbampogmaanbfkg) and [Firefox]
-(https://addons.mozilla.org/en-US/firefox/addon/user-agent-string-switcher/). -
-Open [bing.com/chat](https://bing.com/chat) - If you see a chat feature, you
-are good to go    ### Getting authentication (Required)  - Install the cookie
-editor extension for [Chrome](https://chrome.google.com/webstore/detail/cookie-
-editor/hlkenndednhfkekhgcdicdfddnkalmdm) or [Firefox](https://
+NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0
+Safari/537.36 Edg/111.0.1661.51`). You can do this easily with an extension
+like "User-Agent Switcher and Manager" for [Chrome](https://chrome.google.com/
+webstore/detail/user-agent-switcher-and-m/bhchdcejhohfmigjafbampogmaanbfkg) and
+[Firefox](https://addons.mozilla.org/en-US/firefox/addon/user-agent-string-
+switcher/). - Open [bing.com/chat](https://bing.com/chat) - If you see a chat
+feature, you are good to go    ### Getting authentication (Required)  - Install
+the cookie editor extension for [Chrome](https://chrome.google.com/webstore/
+detail/cookie-editor/hlkenndednhfkekhgcdicdfddnkalmdm) or [Firefox](https://
 addons.mozilla.org/en-US/firefox/addon/cookie-editor/) - Go to `bing.com` -
 Open the extension - Click "Export" on the bottom right (This saves your
 cookies to clipboard) - Paste your cookies into a file `cookies.json`    ##
 Chatbot  ## Usage ### Quick start ``` $ python3 -m EdgeGPT -h EdgeGPT - A demo
 of reverse engineering the Bing GPT chatbot Repo: github.com/acheong08/EdgeGPT
 By: Antonio Cheong !help for help Type !exit to exit Enter twice to send
 message or set --enter-once to send one line message usage: EdgeGPT.py [-h] [--
```

### Comparing `EdgeGPT-0.1.8/src/EdgeGPT.py` & `EdgeGPT-0.1.9/src/EdgeGPT.py`

 * *Files 2% similar despite different names*

```diff
@@ -215,18 +215,22 @@
 
         # Send GET request
         response = self.session.get(
             url=os.environ.get("BING_PROXY_URL")
             or "https://edgeservices.bing.com/edgesvc/turing/conversation/create"
         )
         if response.status_code != 200:
-            print(f"Status code: {response.status_code}")
-            print(response.text)
-            print(response.url)
-            raise Exception("Authentication failed")
+            response = self.session.get(
+                "https://edge.churchless.tech/edgesvc/turing/conversation/create"
+            )
+            if response.status_code != 200:
+                print(f"Status code: {response.status_code}")
+                print(response.text)
+                print(response.url)
+                raise Exception("Authentication failed")
         try:
             self.struct = response.json()
             if self.struct["result"]["value"] == "UnauthorizedRequest":
                 raise NotAllowedToAccess(self.struct["result"]["message"])
         except (json.decoder.JSONDecodeError, NotAllowedToAccess) as exc:
             raise Exception(
                 "Authentication failed. You have not been accepted into the beta.",
```

### Comparing `EdgeGPT-0.1.8/src/ImageGen.py` & `EdgeGPT-0.1.9/src/ImageGen.py`

 * *Files identical despite different names*

