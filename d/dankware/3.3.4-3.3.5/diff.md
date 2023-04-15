# Comparing `tmp/dankware-3.3.4.tar.gz` & `tmp/dankware-3.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dankware-3.3.4.tar", last modified: Sun Apr  9 09:25:53 2023, max compression
+gzip compressed data, was "dankware-3.3.5.tar", last modified: Sat Apr 15 10:09:28 2023, max compression
```

## Comparing `dankware-3.3.4.tar` & `dankware-3.3.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 09:25:53.121963 dankware-3.3.4/
--rw-rw-rw-   0        0        0     1085 2023-02-11 12:53:16.000000 dankware-3.3.4/LICENSE
--rw-rw-rw-   0        0        0    14134 2023-04-09 09:25:53.119362 dankware-3.3.4/PKG-INFO
--rw-rw-rw-   0        0        0    13217 2023-03-29 08:26:24.000000 dankware-3.3.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-09 09:25:53.114362 dankware-3.3.4/dankware/
--rw-rw-rw-   0        0        0    46597 2023-04-09 09:00:17.000000 dankware-3.3.4/dankware/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-09 09:25:53.119362 dankware-3.3.4/dankware.egg-info/
--rw-rw-rw-   0        0        0    14134 2023-04-09 09:25:53.000000 dankware-3.3.4/dankware.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      229 2023-04-09 09:25:53.000000 dankware-3.3.4/dankware.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 09:25:53.000000 dankware-3.3.4/dankware.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-04-09 09:25:53.000000 dankware-3.3.4/dankware.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-09 09:25:53.000000 dankware-3.3.4/dankware.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-09 09:25:53.121963 dankware-3.3.4/setup.cfg
--rw-rw-rw-   0        0        0     1478 2023-04-09 09:10:13.000000 dankware-3.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:09:28.407583 dankware-3.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-15 10:09:15.000000 dankware-3.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13768 2023-04-15 10:09:28.407583 dankware-3.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12829 2023-04-15 10:09:15.000000 dankware-3.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:09:28.407583 dankware-3.3.5/dankware/
+-rw-r--r--   0 runner    (1001) docker     (123)    45628 2023-04-15 10:09:15.000000 dankware-3.3.5/dankware/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:09:28.407583 dankware-3.3.5/dankware.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13768 2023-04-15 10:09:28.000000 dankware-3.3.5/dankware.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-15 10:09:28.000000 dankware-3.3.5/dankware.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 10:09:28.000000 dankware-3.3.5/dankware.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-15 10:09:28.000000 dankware-3.3.5/dankware.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-15 10:09:28.000000 dankware-3.3.5/dankware.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 10:09:28.407583 dankware-3.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-15 10:09:15.000000 dankware-3.3.5/setup.py
```

### Comparing `dankware-3.3.4/LICENSE` & `dankware-3.3.5/LICENSE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 SirDank
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 SirDank
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `dankware-3.3.4/PKG-INFO` & `dankware-3.3.5/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,409 +1,388 @@
-Metadata-Version: 2.1
-Name: dankware
-Version: 3.3.4
-Summary: Python package with various features!
-Home-page: https://github.com/SirDank/dankware
-Author: SirDank
-Author-email: SirDankenstein@protonmail.com
-License: MIT
-Project-URL: GitHub, https://github.com/SirDank/dankware
-Project-URL: Bug Tracker, https://github.com/SirDank/dankware/issues
-Keywords: dank,dankware,multithread,gradient,fade,registry key,error traceback,random ip generator,github scraper,splash screen,hide window,file selector
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
-Classifier: Topic :: Software Development
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-<p align="center">
-  <b>~ Visits ~</b><br><br>
-  <img src="https://profile-counter.glitch.me/dankware/count.svg" />
-</p>
-
-<p align="center">
-  <b>~ Stats ~</b><br><br>
-  <img src="https://static.pepy.tech/personalized-badge/dankware?period=total&units=international_system&left_color=black&right_color=brightgreen&left_text=downloads" />
-  <img src="https://static.pepy.tech/personalized-badge/dankware?period=month&units=international_system&left_color=black&right_color=brightgreen&left_text=downloads%20/%20month" />
-  <img src="https://static.pepy.tech/personalized-badge/dankware?period=week&units=international_system&left_color=black&right_color=brightgreen&left_text=downloads%20/%20week" />
-</p>
-
-# 🚨 dankware 🚨
- Python module with various features! Install with the below command!
-```
-pip install dankware
-```
-
-Update to the latest version with the below command!
-```
-pip install --upgrade dankware
-```
- 
-# 🚨 Multithreading 🚨
-```py
-from dankware import multithread
-import time
-
-a = 0
-def example():
-    global a
-    a += 1
-    print(a)
-    time.sleep(5)
-        
-multithread(example, 10) # func: example | threads: 10 | single: 50 seconds | multi: 5 seconds
-```
-> <img width="500" alt="image" src="https://user-images.githubusercontent.com/52797753/224534374-4693f9fb-2c0c-426b-970d-face9926b9cd.png">
-
-```py
-from dankware import multithread
-import time
-
-new_list = [1, 2, 3, 4, 5]; sum = 0
-
-def example(num):
-    global sum
-    sum += num
-    time.sleep(5)
-
-multithread(example, 10, new_list) # input_one: list
-print(sum)
-```
-> <img width="500" alt="image" src="https://user-images.githubusercontent.com/52797753/224534424-f03f5884-e9c8-445f-8c0a-5bb227c35aed.png">
-
-```py
-from dankware import multithread
-import time
-
-list1 = [1, 2, 3, 4, 5]
-list2 = [5, 4, 3, 2, 1]
-
-def example(num1, num2):
-    print(num1 + num2)
-    time.sleep(5)
-
-multithread(example, 10, list1, list2) # input_one: list1 | input_two: list2
-```
-> <img width="500" alt="image" src="https://user-images.githubusercontent.com/52797753/224534446-c956dfb0-81a2-4717-bd80-e04484e76507.png">
-
-```py
-from dankware import multithread
-import time
-
-new_list = [1, 2, 3, 4, 5]
-
-def example(num1, num2):
-    print(num1 * num2)
-    time.sleep(5)
-
-multithread(example, 10, new_list, 5, progress_bar=False) # input_two: 5 | disabled progress bar
-```
-> <img width="60" alt="image" src="https://user-images.githubusercontent.com/52797753/153749433-95512c4d-afcd-4ad7-9797-caded6e44239.png">
-
-<p>&nbsp;</p>    
-
----  
-
-# 🚨 Export Registry Keys 🚨
-
-```py
-import os
-from dankware import export_registry_keys, is_admin
-
-# [NOTE]: this function requires admin privileges!
-
-export_path = "D:\\export.reg"
-registry_root = r'HKEY_CURRENT_USER'
-registry_path = r'Software\Google\Chrome\PreferenceMACs'
-#export_path = os.path.join(os.environ['USERPROFILE'], 'Desktop', 'export.reg')
-
-export_registry_keys(registry_root, registry_path, recursive=True, export_path=export_path)
-```
-> <img width="500" alt="image" src="https://user-images.githubusercontent.com/52797753/221345714-f1cdea4a-0c08-4c47-8c95-c64d95d12dec.png">
-
-> <img width="500" alt="image" src="https://user-images.githubusercontent.com/52797753/221345782-3a5a6ef0-d3b4-48a7-b8f8-c40f210b067d.png">
-
-<p>&nbsp;</p>    
-
----  
-
-# 🚨 Splash Screen 🚨
-
-```py
-from dankware import splash_screen
-# Supports: GIFs / PNGs / JPGs / BMPs / ICOs
-splash_screen("D:\\splash.gif", duration=5)
-# runs on main thread
-```
-
-```py
-from dankware import splash_screen
-from concurrent.futures import ThreadPoolExecutor
-ThreadPoolExecutor(1).submit(splash_screen, "splash.png", 5)
-# runs on separate thread
-```
-
-> <img width="250" alt="image" src="https://user-images.githubusercontent.com/52797753/228445332-004f8f69-d8be-4d36-95e5-9065891e4d09.gif">
-
-# 🚨 Error Traceback 🚨
-
-```py
-import sys
-from dankware import err, clr
-try: value = 1/0
-except: print(clr(err(sys.exc_info()),2))
-```
-> <img width="700" alt="image" src="https://user-images.githubusercontent.com/52797753/221346044-db739b15-b365-47b3-b6f1-20d199c58ab2.png">
-
-<p>&nbsp;</p>    
-
----  
-
-# 🚨 Scraping 🚨
-
-```py
-from dankware import github_downloads
-# full url > https://api.github.com/repos/EssentialsX/Essentials/releases/latest
-for url in github_downloads("EssentialsX/Essentials"): print(url)
-```
-> <img width="700" alt="image" src="https://user-images.githubusercontent.com/52797753/216242124-ed911013-bae4-4622-8c0a-0d11638da750.png">
-
-```py
-from dankware import github_file_selector
-# full url > https://api.github.com/repos/EssentialsX/Essentials/releases/latest
-for url in github_file_selector("EssentialsX/Essentials", "remove", ['AntiBuild', 'Discord', 'GeoIP', 'Protect', 'XMPP']): print(url)
-```
-> <img width="700" alt="image" src="https://user-images.githubusercontent.com/52797753/216241961-5359d662-a117-4eb4-b74e-e82b41a895bc.png">
-
-<p>&nbsp;</p>    
-
----  
-
-# 🚨 Generate Random IPs 🚨
-
-```py
-from dankware import random_ip
-print(random_ip())
-```
-
-> <img width="200" alt="image" src="https://user-images.githubusercontent.com/52797753/194127781-8f622448-4595-4c2a-a3e7-3e4356076840.png">
-
-<p>&nbsp;</p>    
-
----  
-
-# 🚨 Colour Special Characters 🚨
-
-```py
-from dankware import clr
-# default mode = 1
-# default colour_one = white
-# default colour_two = magenta
-print(clr("\n  > Hey! Long time no see :)"))
-#print(clr("\n  > Hey! Long time no see :)", colour_one = white, colour_two = magenta))
-```
-> <img width="350" alt="image" src="https://user-images.githubusercontent.com/52797753/153749617-bb0483fe-0385-490b-8695-72f448300c39.png">
-
-```py
-from dankware import clr, white, magenta
-# default mode = 1
-# default colour_one = white
-# default colour_two = magenta
-print(clr("\n  > Hey! Long time no see :)", colour_one = magenta, colour_two = white))
-```
-> <img width="350" alt="image" src="https://user-images.githubusercontent.com/52797753/220981909-d6361e6a-d109-447a-8401-85e2813e7859.png">
-
-```py
-from dankware import clr
-print(clr("\n  This is a string: True | This is an integer: False"))
-```
-> <img width="350" alt="image" src="https://user-images.githubusercontent.com/52797753/153749921-3332f3e6-eaa8-4bf1-ab4d-3fe35d245492.png">
-
-```py
-from dankware import clr, green, magenta
-# dankware now supports adding custom colours on both the text and the function itself!
-# colour_two = green
-print(clr(f"\n  > {magenta}Purple{white} thinks he's better than everyone else :(", colour_two=green))
-```
-> <img width="350" alt="image" src="https://user-images.githubusercontent.com/52797753/190898116-750e256e-a1d9-4c8a-a3b2-d0ac209fa0f7.png">
-
-```py
-from dankware import clr
-# mode = 2
-print(clr("\n  > Error in sector [7] redirecting... | INTEGRITY_CHECK_SUCCESS: TRUE",2))
-```
-> <img width="500" alt="image" src="https://user-images.githubusercontent.com/52797753/153749821-ae3e4dfd-26dc-4e08-a06e-677ac26457a1.png">
-
-```py
-from dankware import clr
-# mode = 3
-print(clr("\n  > Is this a randomly coloured string: TRUE | As you can see it does not colour True/False",3))
-```
-> <img width="650" alt="image" src="https://user-images.githubusercontent.com/52797753/155293415-7b065b5a-44dd-4fe7-995d-a25582f904cb.png">
-
-<p>&nbsp;</p>    
-
----  
-
-# 🚨 Banners 🚨
-
-```py
-banner = '''
-
-     888                   888                                             
-     888                   888           s i r . d a n k ' s               
-     888                   888                                             
- .d88888  8888b.  88888b.  888  888 888  888  888  8888b.  888d888 .d88b.  
-d88" 888     "88b 888 "88b 888 .88P 888  888  888     "88b 888P"  d8P  Y8b 
-888  888 .d888888 888  888 888888K  888  888  888 .d888888 888    88888888 
-Y88b 888 888  888 888  888 888 "88b Y88b 888 d88P 888  888 888    Y8b.     
- "Y88888 "Y888888 888  888 888  888  "Y8888888P"  "Y888888 888     "Y8888  
-
-'''
-```
-
-## ♦️ Colourize Banner (random) ♦️
-```py
-from dankware import clr
-# mode = 4
-print(clr(banner,4))
-```
-> <img width="550" alt="image" src="https://user-images.githubusercontent.com/52797753/153722086-2f372bfa-4872-46a0-81f8-cdf7c2344fd6.png">
-
-## ♦️ Align Banner (console center) ♦️
-```py
-from dankware import align
-print(align(banner)) # also works with single text line (even coloured)
-```
-> <img width="800" alt="image" src="https://user-images.githubusercontent.com/52797753/153722230-1f3b6103-6d8a-4537-9828-1718a6bd3367.png">
-
-## ♦️ Align Coloured Banner ♦️
-```py
-from dankware import align, clr
-print(align(clr(banner,4)))
-```
-> <img width="800" alt="image" src="https://user-images.githubusercontent.com/52797753/153722373-9925dd25-83bb-4d1c-83eb-bfaae1802088.png">
-
-<p>&nbsp;</p>    
-
----  
-
-# 🚨 Gradient Reworked [ Originally By @venaxyt ] 🚨
-
-```py
-from dankware import fade
-banner = '''
-
-                              888 d8b                   888    
-       v e n a x y t ' s      888 Y8P                   888    
-                              888                       888    
- .d88b.  888d888 8888b.   .d88888 888  .d88b.  88888b.  888888 
-d88P"88b 888P"      "88b d88" 888 888 d8P  Y8b 888 "88b 888    
-888  888 888    .d888888 888  888 888 88888888 888  888 888    
-Y88b 888 888    888  888 Y88b 888 888 Y8b.     888  888 Y88b.  
- "Y88888 888    "Y888888  "Y88888 888  "Y8888  888  888  "Y888 
-     888                                                       
-Y8b d88P                                                       
- "Y88P"                                                        
-
-
-'''
-```
-
-## ♦️ Black ♦️
-```py
-print(fade(banner, "black"))
-```
-> <img width="475" alt="image" src="https://user-images.githubusercontent.com/52797753/153722811-b257611e-9111-4a0e-92fb-7dbe503ce6db.png">
-```py
-print(fade(banner, "black-v"))
-```
-> <img width="475" alt="image" src="https://user-images.githubusercontent.com/52797753/153723205-a91eb1c6-07bc-4bc6-9fa6-52231e50a25c.png">
-
-## ♦️ Red ♦️
-```py
-print(fade(banner, "red"))
-```
-> <img width="475" alt="image" src="https://user-images.githubusercontent.com/52797753/153722946-3221bfd8-ff9d-4c9d-8b70-0c2736ec4e30.png">
-```py
-print(fade(banner, "red-v"))
-```
-> <img width="475" alt="image" src="https://user-images.githubusercontent.com/52797753/153723473-bdb75ea7-2df2-4f70-adb5-cf5caa57200a.png">
-
-## ♦️ Green ♦️
-```py
-print(fade(banner, "green"))
-```
-> <img width="475" alt="image" src="https://user-images.githubusercontent.com/52797753/153723050-c30bd3f1-989a-4141-b40a-2869a2dadef6.png">
-```py
-print(fade(banner, "green-v"))
-```
-> <img width="475" alt="image" src="https://user-images.githubusercontent.com/52797753/153723481-2e5c21b2-0f12-4d99-ab8d-a3e5c40e4c16.png">
-
-## ♦️ Cyan ♦️
-```py
-print(fade(banner, "cyan"))
-```
-> <img width="475" alt="image" src="https://user-images.githubusercontent.com/52797753/153723059-b4808365-6006-4726-b427-b6848e0fc0e5.png">
-```py
-print(fade(banner, "cyan-v"))
-```
-> <img width="475" alt="image" src="https://user-images.githubusercontent.com/52797753/153723496-8d03c5d3-601e-499d-80cd-51c3648957bf.png">
-
-## ♦️ Blue ♦️
-```py
-print(fade(banner, "blue"))
-```
-> <img width="475" alt="image" src="https://user-images.githubusercontent.com/52797753/153723092-0a32d8e6-680e-4df3-bdf1-089663f25f45.png">
-```py
-print(fade(banner, "blue-v"))
-```
-> <img width="475" alt="image" src="https://user-images.githubusercontent.com/52797753/153723509-41732010-b7d5-4867-95f9-690d47322536.png">
-
-## ♦️ Purple ♦️
-```py
-print(fade(banner, "purple"))
-```
-> <img width="475" alt="image" src="https://user-images.githubusercontent.com/52797753/153723148-2c94c459-1441-4752-a11f-a547754da7bc.png">
-```py
-print(fade(banner, "purple-v"))
-```
-> <img width="475" alt="image" src="https://user-images.githubusercontent.com/52797753/153723519-00aa980e-4a04-4d8d-a319-5691c1f8e517.png">
-
-## ♦️ Pink ♦️
-```py
-print(fade(banner, "pink-v"))
-```
-> <img width="475" alt="image" src="https://user-images.githubusercontent.com/52797753/153723540-b324dfe1-5ae2-4b66-ad3a-546a589558c8.png">
-
-## ♦️ Random ♦️
-```py
-print(fade(banner, "random"))
-```
-> <img width="475" alt="image" src="https://user-images.githubusercontent.com/52797753/153723545-0ea34ea7-1844-4ace-8948-3e71e28c0a30.png">
-
-<p>&nbsp;</p>    
-
----  
-
-# 🚨 Also check out 🚨
-<p align="center">
-  <a href="https://github.com/SirDank/dank.tool">
-  <img width="700" alt="image" src="https://user-images.githubusercontent.com/52797753/192086704-35f5a0db-3c5d-4782-95a9-6e2756cc8528.png">
-  </a>
-</p>
-
-<p>&nbsp;</p>    
-
----  
-
-# 🚨 Stats 🚨
-
-<br><p align="center"><img width="800" alt="image" src="https://repobeats.axiom.co/api/embed/ed44a86c2d46a8719705f5f57efde209b8cb5492.svg"></p><br>
-
-# 🚨 Star History 🚨
-
-<br><p align="center">[![Star History Chart](https://api.star-history.com/svg?repos=SirDank/dankware&type=Date)](https://star-history.com/#SirDank/dankware&Date)</p><br>
+<p align="center">
+  <b>~ Visits ~</b><br><br>
+  <img src="https://profile-counter.glitch.me/dankware/count.svg" />
+</p>
+
+<p align="center">
+  <b>~ Stats ~</b><br><br>
+  <img src="https://static.pepy.tech/personalized-badge/dankware?period=total&units=international_system&left_color=black&right_color=brightgreen&left_text=downloads" />
+  <img src="https://static.pepy.tech/personalized-badge/dankware?period=month&units=international_system&left_color=black&right_color=brightgreen&left_text=downloads%20/%20month" />
+  <img src="https://static.pepy.tech/personalized-badge/dankware?period=week&units=international_system&left_color=black&right_color=brightgreen&left_text=downloads%20/%20week" />
+</p>
+
+# 🚨 dankware 🚨
+ Python module with various features! Install with the below command!
+```
+pip install dankware
+```
+
+Update to the latest version with the below command!
+```
+pip install --upgrade dankware
+```
+ 
+# 🚨 Multithreading 🚨
+```py
+from dankware import multithread
+import time
+
+a = 0
+def example():
+    global a
+    a += 1
+    print(a)
+    time.sleep(5)
+        
+multithread(example, 10) # func: example | threads: 10 | single: 50 seconds | multi: 5 seconds
+```
+> <img width="500" alt="image" src="https://user-images.githubusercontent.com/52797753/224534374-4693f9fb-2c0c-426b-970d-face9926b9cd.png">
+
+```py
+from dankware import multithread
+import time
+
+new_list = [1, 2, 3, 4, 5]; sum = 0
+
+def example(num):
+    global sum
+    sum += num
+    time.sleep(5)
+
+multithread(example, 10, new_list) # input_one: list
+print(sum)
+```
+> <img width="500" alt="image" src="https://user-images.githubusercontent.com/52797753/224534424-f03f5884-e9c8-445f-8c0a-5bb227c35aed.png">
+
+```py
+from dankware import multithread
+import time
+
+list1 = [1, 2, 3, 4, 5]
+list2 = [5, 4, 3, 2, 1]
+
+def example(num1, num2):
+    print(num1 + num2)
+    time.sleep(5)
+
+multithread(example, 10, list1, list2) # input_one: list1 | input_two: list2
+```
+> <img width="500" alt="image" src="https://user-images.githubusercontent.com/52797753/224534446-c956dfb0-81a2-4717-bd80-e04484e76507.png">
+
+```py
+from dankware import multithread
+import time
+
+new_list = [1, 2, 3, 4, 5]
+
+def example(num1, num2):
+    print(num1 * num2)
+    time.sleep(5)
+
+multithread(example, 10, new_list, 5, progress_bar=False) # input_two: 5 | disabled progress bar
+```
+> <img width="60" alt="image" src="https://user-images.githubusercontent.com/52797753/153749433-95512c4d-afcd-4ad7-9797-caded6e44239.png">
+
+<p>&nbsp;</p>    
+
+---  
+
+# 🚨 Export Registry Keys 🚨
+
+```py
+import os
+from dankware import export_registry_keys, is_admin
+
+# [NOTE]: this function requires admin privileges!
+
+export_path = "D:\\export.reg"
+registry_root = r'HKEY_CURRENT_USER'
+registry_path = r'Software\Google\Chrome\PreferenceMACs'
+#export_path = os.path.join(os.environ['USERPROFILE'], 'Desktop', 'export.reg')
+
+export_registry_keys(registry_root, registry_path, recursive=True, export_path=export_path)
+```
+> <img width="500" alt="image" src="https://user-images.githubusercontent.com/52797753/221345714-f1cdea4a-0c08-4c47-8c95-c64d95d12dec.png">
+
+> <img width="500" alt="image" src="https://user-images.githubusercontent.com/52797753/221345782-3a5a6ef0-d3b4-48a7-b8f8-c40f210b067d.png">
+
+<p>&nbsp;</p>    
+
+---  
+
+# 🚨 Splash Screen 🚨
+
+```py
+from dankware import splash_screen
+# Supports: GIFs / PNGs / JPGs / BMPs / ICOs
+splash_screen("D:\\splash.gif", duration=5)
+# runs on main thread
+```
+
+```py
+from dankware import splash_screen
+from concurrent.futures import ThreadPoolExecutor
+ThreadPoolExecutor(1).submit(splash_screen, "splash.png", 5)
+# runs on separate thread
+```
+
+> <img width="250" alt="image" src="https://user-images.githubusercontent.com/52797753/228445332-004f8f69-d8be-4d36-95e5-9065891e4d09.gif">
+
+# 🚨 Error Traceback 🚨
+
+```py
+import sys
+from dankware import err, clr
+try: value = 1/0
+except: print(clr(err(sys.exc_info()),2))
+```
+> <img width="700" alt="image" src="https://user-images.githubusercontent.com/52797753/221346044-db739b15-b365-47b3-b6f1-20d199c58ab2.png">
+
+<p>&nbsp;</p>    
+
+---  
+
+# 🚨 Scraping 🚨
+
+```py
+from dankware import github_downloads
+# full url > https://api.github.com/repos/EssentialsX/Essentials/releases/latest
+for url in github_downloads("EssentialsX/Essentials"): print(url)
+```
+> <img width="700" alt="image" src="https://user-images.githubusercontent.com/52797753/216242124-ed911013-bae4-4622-8c0a-0d11638da750.png">
+
+```py
+from dankware import github_file_selector
+# full url > https://api.github.com/repos/EssentialsX/Essentials/releases/latest
+for url in github_file_selector("EssentialsX/Essentials", "remove", ['AntiBuild', 'Discord', 'GeoIP', 'Protect', 'XMPP']): print(url)
+```
+> <img width="700" alt="image" src="https://user-images.githubusercontent.com/52797753/216241961-5359d662-a117-4eb4-b74e-e82b41a895bc.png">
+
+<p>&nbsp;</p>    
+
+---  
+
+# 🚨 Generate Random IPs 🚨
+
+```py
+from dankware import random_ip
+print(random_ip())
+```
+
+> <img width="200" alt="image" src="https://user-images.githubusercontent.com/52797753/194127781-8f622448-4595-4c2a-a3e7-3e4356076840.png">
+
+<p>&nbsp;</p>    
+
+---  
+
+# 🚨 Colour Special Characters 🚨
+
+```py
+from dankware import clr
+# default mode = 1
+# default colour_one = white
+# default colour_two = magenta
+print(clr("\n  > Hey! Long time no see :)"))
+#print(clr("\n  > Hey! Long time no see :)", colour_one = white, colour_two = magenta))
+```
+> <img width="350" alt="image" src="https://user-images.githubusercontent.com/52797753/153749617-bb0483fe-0385-490b-8695-72f448300c39.png">
+
+```py
+from dankware import clr, white, magenta
+# default mode = 1
+# default colour_one = white
+# default colour_two = magenta
+print(clr("\n  > Hey! Long time no see :)", colour_one = magenta, colour_two = white))
+```
+> <img width="350" alt="image" src="https://user-images.githubusercontent.com/52797753/220981909-d6361e6a-d109-447a-8401-85e2813e7859.png">
+
+```py
+from dankware import clr
+print(clr("\n  This is a string: True | This is an integer: False"))
+```
+> <img width="350" alt="image" src="https://user-images.githubusercontent.com/52797753/153749921-3332f3e6-eaa8-4bf1-ab4d-3fe35d245492.png">
+
+```py
+from dankware import clr, green, magenta
+# dankware now supports adding custom colours on both the text and the function itself!
+# colour_two = green
+print(clr(f"\n  > {magenta}Purple{white} thinks he's better than everyone else :(", colour_two=green))
+```
+> <img width="350" alt="image" src="https://user-images.githubusercontent.com/52797753/190898116-750e256e-a1d9-4c8a-a3b2-d0ac209fa0f7.png">
+
+```py
+from dankware import clr
+# mode = 2
+print(clr("\n  > Error in sector [7] redirecting... | INTEGRITY_CHECK_SUCCESS: TRUE",2))
+```
+> <img width="500" alt="image" src="https://user-images.githubusercontent.com/52797753/153749821-ae3e4dfd-26dc-4e08-a06e-677ac26457a1.png">
+
+```py
+from dankware import clr
+# mode = 3
+print(clr("\n  > Is this a randomly coloured string: TRUE | As you can see it does not colour True/False",3))
+```
+> <img width="650" alt="image" src="https://user-images.githubusercontent.com/52797753/155293415-7b065b5a-44dd-4fe7-995d-a25582f904cb.png">
+
+<p>&nbsp;</p>    
+
+---  
+
+# 🚨 Banners 🚨
+
+```py
+banner = '''
+
+     888                   888                                             
+     888                   888           s i r . d a n k ' s               
+     888                   888                                             
+ .d88888  8888b.  88888b.  888  888 888  888  888  8888b.  888d888 .d88b.  
+d88" 888     "88b 888 "88b 888 .88P 888  888  888     "88b 888P"  d8P  Y8b 
+888  888 .d888888 888  888 888888K  888  888  888 .d888888 888    88888888 
+Y88b 888 888  888 888  888 888 "88b Y88b 888 d88P 888  888 888    Y8b.     
+ "Y88888 "Y888888 888  888 888  888  "Y8888888P"  "Y888888 888     "Y8888  
+
+'''
+```
+
+## ♦️ Colourize Banner (random) ♦️
+```py
+from dankware import clr
+# mode = 4
+print(clr(banner,4))
+```
+> <img width="550" alt="image" src="https://user-images.githubusercontent.com/52797753/153722086-2f372bfa-4872-46a0-81f8-cdf7c2344fd6.png">
+
+## ♦️ Align Banner (console center) ♦️
+```py
+from dankware import align
+print(align(banner)) # also works with single text line (even coloured)
+```
+> <img width="800" alt="image" src="https://user-images.githubusercontent.com/52797753/153722230-1f3b6103-6d8a-4537-9828-1718a6bd3367.png">
+
+## ♦️ Align Coloured Banner ♦️
+```py
+from dankware import align, clr
+print(align(clr(banner,4)))
+```
+> <img width="800" alt="image" src="https://user-images.githubusercontent.com/52797753/153722373-9925dd25-83bb-4d1c-83eb-bfaae1802088.png">
+
+<p>&nbsp;</p>    
+
+---  
+
+# 🚨 Gradient Reworked [ Originally By @venaxyt ] 🚨
+
+```py
+from dankware import fade
+banner = '''
+
+                              888 d8b                   888    
+       v e n a x y t ' s      888 Y8P                   888    
+                              888                       888    
+ .d88b.  888d888 8888b.   .d88888 888  .d88b.  88888b.  888888 
+d88P"88b 888P"      "88b d88" 888 888 d8P  Y8b 888 "88b 888    
+888  888 888    .d888888 888  888 888 88888888 888  888 888    
+Y88b 888 888    888  888 Y88b 888 888 Y8b.     888  888 Y88b.  
+ "Y88888 888    "Y888888  "Y88888 888  "Y8888  888  888  "Y888 
+     888                                                       
+Y8b d88P                                                       
+ "Y88P"                                                        
+
+
+'''
+```
+
+## ♦️ Black ♦️
+```py
+print(fade(banner, "black"))
+```
+> <img width="475" alt="image" src="https://user-images.githubusercontent.com/52797753/153722811-b257611e-9111-4a0e-92fb-7dbe503ce6db.png">
+```py
+print(fade(banner, "black-v"))
+```
+> <img width="475" alt="image" src="https://user-images.githubusercontent.com/52797753/153723205-a91eb1c6-07bc-4bc6-9fa6-52231e50a25c.png">
+
+## ♦️ Red ♦️
+```py
+print(fade(banner, "red"))
+```
+> <img width="475" alt="image" src="https://user-images.githubusercontent.com/52797753/153722946-3221bfd8-ff9d-4c9d-8b70-0c2736ec4e30.png">
+```py
+print(fade(banner, "red-v"))
+```
+> <img width="475" alt="image" src="https://user-images.githubusercontent.com/52797753/153723473-bdb75ea7-2df2-4f70-adb5-cf5caa57200a.png">
+
+## ♦️ Green ♦️
+```py
+print(fade(banner, "green"))
+```
+> <img width="475" alt="image" src="https://user-images.githubusercontent.com/52797753/153723050-c30bd3f1-989a-4141-b40a-2869a2dadef6.png">
+```py
+print(fade(banner, "green-v"))
+```
+> <img width="475" alt="image" src="https://user-images.githubusercontent.com/52797753/153723481-2e5c21b2-0f12-4d99-ab8d-a3e5c40e4c16.png">
+
+## ♦️ Cyan ♦️
+```py
+print(fade(banner, "cyan"))
+```
+> <img width="475" alt="image" src="https://user-images.githubusercontent.com/52797753/153723059-b4808365-6006-4726-b427-b6848e0fc0e5.png">
+```py
+print(fade(banner, "cyan-v"))
+```
+> <img width="475" alt="image" src="https://user-images.githubusercontent.com/52797753/153723496-8d03c5d3-601e-499d-80cd-51c3648957bf.png">
+
+## ♦️ Blue ♦️
+```py
+print(fade(banner, "blue"))
+```
+> <img width="475" alt="image" src="https://user-images.githubusercontent.com/52797753/153723092-0a32d8e6-680e-4df3-bdf1-089663f25f45.png">
+```py
+print(fade(banner, "blue-v"))
+```
+> <img width="475" alt="image" src="https://user-images.githubusercontent.com/52797753/153723509-41732010-b7d5-4867-95f9-690d47322536.png">
+
+## ♦️ Purple ♦️
+```py
+print(fade(banner, "purple"))
+```
+> <img width="475" alt="image" src="https://user-images.githubusercontent.com/52797753/153723148-2c94c459-1441-4752-a11f-a547754da7bc.png">
+```py
+print(fade(banner, "purple-v"))
+```
+> <img width="475" alt="image" src="https://user-images.githubusercontent.com/52797753/153723519-00aa980e-4a04-4d8d-a319-5691c1f8e517.png">
+
+## ♦️ Pink ♦️
+```py
+print(fade(banner, "pink-v"))
+```
+> <img width="475" alt="image" src="https://user-images.githubusercontent.com/52797753/153723540-b324dfe1-5ae2-4b66-ad3a-546a589558c8.png">
+
+## ♦️ Random ♦️
+```py
+print(fade(banner, "random"))
+```
+> <img width="475" alt="image" src="https://user-images.githubusercontent.com/52797753/153723545-0ea34ea7-1844-4ace-8948-3e71e28c0a30.png">
+
+<p>&nbsp;</p>    
+
+---  
+
+# 🚨 Also check out 🚨
+<p align="center">
+  <a href="https://github.com/SirDank/dank.tool">
+  <img width="700" alt="image" src="https://user-images.githubusercontent.com/52797753/192086704-35f5a0db-3c5d-4782-95a9-6e2756cc8528.png">
+  </a>
+</p>
+
+<p>&nbsp;</p>    
+
+---  
+
+# 🚨 Stats 🚨
+
+<br><p align="center"><img width="800" alt="image" src="https://repobeats.axiom.co/api/embed/ed44a86c2d46a8719705f5f57efde209b8cb5492.svg"></p><br>
+
+# 🚨 Star History 🚨
+
+<br><p align="center">[![Star History Chart](https://api.star-history.com/svg?repos=SirDank/dankware&type=Date)](https://star-history.com/#SirDank/dankware&Date)</p><br>
```

### Comparing `dankware-3.3.4/README.md` & `dankware-3.3.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,388 +1,410 @@
-<p align="center">
-  <b>~ Visits ~</b><br><br>
-  <img src="https://profile-counter.glitch.me/dankware/count.svg" />
-</p>
-
-<p align="center">
-  <b>~ Stats ~</b><br><br>
-  <img src="https://static.pepy.tech/personalized-badge/dankware?period=total&units=international_system&left_color=black&right_color=brightgreen&left_text=downloads" />
-  <img src="https://static.pepy.tech/personalized-badge/dankware?period=month&units=international_system&left_color=black&right_color=brightgreen&left_text=downloads%20/%20month" />
-  <img src="https://static.pepy.tech/personalized-badge/dankware?period=week&units=international_system&left_color=black&right_color=brightgreen&left_text=downloads%20/%20week" />
-</p>
-
-# 🚨 dankware 🚨
- Python module with various features! Install with the below command!
-```
-pip install dankware
-```
-
-Update to the latest version with the below command!
-```
-pip install --upgrade dankware
-```
- 
-# 🚨 Multithreading 🚨
-```py
-from dankware import multithread
-import time
-
-a = 0
-def example():
-    global a
-    a += 1
-    print(a)
-    time.sleep(5)
-        
-multithread(example, 10) # func: example | threads: 10 | single: 50 seconds | multi: 5 seconds
-```
-> <img width="500" alt="image" src="https://user-images.githubusercontent.com/52797753/224534374-4693f9fb-2c0c-426b-970d-face9926b9cd.png">
-
-```py
-from dankware import multithread
-import time
-
-new_list = [1, 2, 3, 4, 5]; sum = 0
-
-def example(num):
-    global sum
-    sum += num
-    time.sleep(5)
-
-multithread(example, 10, new_list) # input_one: list
-print(sum)
-```
-> <img width="500" alt="image" src="https://user-images.githubusercontent.com/52797753/224534424-f03f5884-e9c8-445f-8c0a-5bb227c35aed.png">
-
-```py
-from dankware import multithread
-import time
-
-list1 = [1, 2, 3, 4, 5]
-list2 = [5, 4, 3, 2, 1]
-
-def example(num1, num2):
-    print(num1 + num2)
-    time.sleep(5)
-
-multithread(example, 10, list1, list2) # input_one: list1 | input_two: list2
-```
-> <img width="500" alt="image" src="https://user-images.githubusercontent.com/52797753/224534446-c956dfb0-81a2-4717-bd80-e04484e76507.png">
-
-```py
-from dankware import multithread
-import time
-
-new_list = [1, 2, 3, 4, 5]
-
-def example(num1, num2):
-    print(num1 * num2)
-    time.sleep(5)
-
-multithread(example, 10, new_list, 5, progress_bar=False) # input_two: 5 | disabled progress bar
-```
-> <img width="60" alt="image" src="https://user-images.githubusercontent.com/52797753/153749433-95512c4d-afcd-4ad7-9797-caded6e44239.png">
-
-<p>&nbsp;</p>    
-
----  
-
-# 🚨 Export Registry Keys 🚨
-
-```py
-import os
-from dankware import export_registry_keys, is_admin
-
-# [NOTE]: this function requires admin privileges!
-
-export_path = "D:\\export.reg"
-registry_root = r'HKEY_CURRENT_USER'
-registry_path = r'Software\Google\Chrome\PreferenceMACs'
-#export_path = os.path.join(os.environ['USERPROFILE'], 'Desktop', 'export.reg')
-
-export_registry_keys(registry_root, registry_path, recursive=True, export_path=export_path)
-```
-> <img width="500" alt="image" src="https://user-images.githubusercontent.com/52797753/221345714-f1cdea4a-0c08-4c47-8c95-c64d95d12dec.png">
-
-> <img width="500" alt="image" src="https://user-images.githubusercontent.com/52797753/221345782-3a5a6ef0-d3b4-48a7-b8f8-c40f210b067d.png">
-
-<p>&nbsp;</p>    
-
----  
-
-# 🚨 Splash Screen 🚨
-
-```py
-from dankware import splash_screen
-# Supports: GIFs / PNGs / JPGs / BMPs / ICOs
-splash_screen("D:\\splash.gif", duration=5)
-# runs on main thread
-```
-
-```py
-from dankware import splash_screen
-from concurrent.futures import ThreadPoolExecutor
-ThreadPoolExecutor(1).submit(splash_screen, "splash.png", 5)
-# runs on separate thread
-```
-
-> <img width="250" alt="image" src="https://user-images.githubusercontent.com/52797753/228445332-004f8f69-d8be-4d36-95e5-9065891e4d09.gif">
-
-# 🚨 Error Traceback 🚨
-
-```py
-import sys
-from dankware import err, clr
-try: value = 1/0
-except: print(clr(err(sys.exc_info()),2))
-```
-> <img width="700" alt="image" src="https://user-images.githubusercontent.com/52797753/221346044-db739b15-b365-47b3-b6f1-20d199c58ab2.png">
-
-<p>&nbsp;</p>    
-
----  
-
-# 🚨 Scraping 🚨
-
-```py
-from dankware import github_downloads
-# full url > https://api.github.com/repos/EssentialsX/Essentials/releases/latest
-for url in github_downloads("EssentialsX/Essentials"): print(url)
-```
-> <img width="700" alt="image" src="https://user-images.githubusercontent.com/52797753/216242124-ed911013-bae4-4622-8c0a-0d11638da750.png">
-
-```py
-from dankware import github_file_selector
-# full url > https://api.github.com/repos/EssentialsX/Essentials/releases/latest
-for url in github_file_selector("EssentialsX/Essentials", "remove", ['AntiBuild', 'Discord', 'GeoIP', 'Protect', 'XMPP']): print(url)
-```
-> <img width="700" alt="image" src="https://user-images.githubusercontent.com/52797753/216241961-5359d662-a117-4eb4-b74e-e82b41a895bc.png">
-
-<p>&nbsp;</p>    
-
----  
-
-# 🚨 Generate Random IPs 🚨
-
-```py
-from dankware import random_ip
-print(random_ip())
-```
-
-> <img width="200" alt="image" src="https://user-images.githubusercontent.com/52797753/194127781-8f622448-4595-4c2a-a3e7-3e4356076840.png">
-
-<p>&nbsp;</p>    
-
----  
-
-# 🚨 Colour Special Characters 🚨
-
-```py
-from dankware import clr
-# default mode = 1
-# default colour_one = white
-# default colour_two = magenta
-print(clr("\n  > Hey! Long time no see :)"))
-#print(clr("\n  > Hey! Long time no see :)", colour_one = white, colour_two = magenta))
-```
-> <img width="350" alt="image" src="https://user-images.githubusercontent.com/52797753/153749617-bb0483fe-0385-490b-8695-72f448300c39.png">
-
-```py
-from dankware import clr, white, magenta
-# default mode = 1
-# default colour_one = white
-# default colour_two = magenta
-print(clr("\n  > Hey! Long time no see :)", colour_one = magenta, colour_two = white))
-```
-> <img width="350" alt="image" src="https://user-images.githubusercontent.com/52797753/220981909-d6361e6a-d109-447a-8401-85e2813e7859.png">
-
-```py
-from dankware import clr
-print(clr("\n  This is a string: True | This is an integer: False"))
-```
-> <img width="350" alt="image" src="https://user-images.githubusercontent.com/52797753/153749921-3332f3e6-eaa8-4bf1-ab4d-3fe35d245492.png">
-
-```py
-from dankware import clr, green, magenta
-# dankware now supports adding custom colours on both the text and the function itself!
-# colour_two = green
-print(clr(f"\n  > {magenta}Purple{white} thinks he's better than everyone else :(", colour_two=green))
-```
-> <img width="350" alt="image" src="https://user-images.githubusercontent.com/52797753/190898116-750e256e-a1d9-4c8a-a3b2-d0ac209fa0f7.png">
-
-```py
-from dankware import clr
-# mode = 2
-print(clr("\n  > Error in sector [7] redirecting... | INTEGRITY_CHECK_SUCCESS: TRUE",2))
-```
-> <img width="500" alt="image" src="https://user-images.githubusercontent.com/52797753/153749821-ae3e4dfd-26dc-4e08-a06e-677ac26457a1.png">
-
-```py
-from dankware import clr
-# mode = 3
-print(clr("\n  > Is this a randomly coloured string: TRUE | As you can see it does not colour True/False",3))
-```
-> <img width="650" alt="image" src="https://user-images.githubusercontent.com/52797753/155293415-7b065b5a-44dd-4fe7-995d-a25582f904cb.png">
-
-<p>&nbsp;</p>    
-
----  
-
-# 🚨 Banners 🚨
-
-```py
-banner = '''
-
-     888                   888                                             
-     888                   888           s i r . d a n k ' s               
-     888                   888                                             
- .d88888  8888b.  88888b.  888  888 888  888  888  8888b.  888d888 .d88b.  
-d88" 888     "88b 888 "88b 888 .88P 888  888  888     "88b 888P"  d8P  Y8b 
-888  888 .d888888 888  888 888888K  888  888  888 .d888888 888    88888888 
-Y88b 888 888  888 888  888 888 "88b Y88b 888 d88P 888  888 888    Y8b.     
- "Y88888 "Y888888 888  888 888  888  "Y8888888P"  "Y888888 888     "Y8888  
-
-'''
-```
-
-## ♦️ Colourize Banner (random) ♦️
-```py
-from dankware import clr
-# mode = 4
-print(clr(banner,4))
-```
-> <img width="550" alt="image" src="https://user-images.githubusercontent.com/52797753/153722086-2f372bfa-4872-46a0-81f8-cdf7c2344fd6.png">
-
-## ♦️ Align Banner (console center) ♦️
-```py
-from dankware import align
-print(align(banner)) # also works with single text line (even coloured)
-```
-> <img width="800" alt="image" src="https://user-images.githubusercontent.com/52797753/153722230-1f3b6103-6d8a-4537-9828-1718a6bd3367.png">
-
-## ♦️ Align Coloured Banner ♦️
-```py
-from dankware import align, clr
-print(align(clr(banner,4)))
-```
-> <img width="800" alt="image" src="https://user-images.githubusercontent.com/52797753/153722373-9925dd25-83bb-4d1c-83eb-bfaae1802088.png">
-
-<p>&nbsp;</p>    
-
----  
-
-# 🚨 Gradient Reworked [ Originally By @venaxyt ] 🚨
-
-```py
-from dankware import fade
-banner = '''
-
-                              888 d8b                   888    
-       v e n a x y t ' s      888 Y8P                   888    
-                              888                       888    
- .d88b.  888d888 8888b.   .d88888 888  .d88b.  88888b.  888888 
-d88P"88b 888P"      "88b d88" 888 888 d8P  Y8b 888 "88b 888    
-888  888 888    .d888888 888  888 888 88888888 888  888 888    
-Y88b 888 888    888  888 Y88b 888 888 Y8b.     888  888 Y88b.  
- "Y88888 888    "Y888888  "Y88888 888  "Y8888  888  888  "Y888 
-     888                                                       
-Y8b d88P                                                       
- "Y88P"                                                        
-
-
-'''
-```
-
-## ♦️ Black ♦️
-```py
-print(fade(banner, "black"))
-```
-> <img width="475" alt="image" src="https://user-images.githubusercontent.com/52797753/153722811-b257611e-9111-4a0e-92fb-7dbe503ce6db.png">
-```py
-print(fade(banner, "black-v"))
-```
-> <img width="475" alt="image" src="https://user-images.githubusercontent.com/52797753/153723205-a91eb1c6-07bc-4bc6-9fa6-52231e50a25c.png">
-
-## ♦️ Red ♦️
-```py
-print(fade(banner, "red"))
-```
-> <img width="475" alt="image" src="https://user-images.githubusercontent.com/52797753/153722946-3221bfd8-ff9d-4c9d-8b70-0c2736ec4e30.png">
-```py
-print(fade(banner, "red-v"))
-```
-> <img width="475" alt="image" src="https://user-images.githubusercontent.com/52797753/153723473-bdb75ea7-2df2-4f70-adb5-cf5caa57200a.png">
-
-## ♦️ Green ♦️
-```py
-print(fade(banner, "green"))
-```
-> <img width="475" alt="image" src="https://user-images.githubusercontent.com/52797753/153723050-c30bd3f1-989a-4141-b40a-2869a2dadef6.png">
-```py
-print(fade(banner, "green-v"))
-```
-> <img width="475" alt="image" src="https://user-images.githubusercontent.com/52797753/153723481-2e5c21b2-0f12-4d99-ab8d-a3e5c40e4c16.png">
-
-## ♦️ Cyan ♦️
-```py
-print(fade(banner, "cyan"))
-```
-> <img width="475" alt="image" src="https://user-images.githubusercontent.com/52797753/153723059-b4808365-6006-4726-b427-b6848e0fc0e5.png">
-```py
-print(fade(banner, "cyan-v"))
-```
-> <img width="475" alt="image" src="https://user-images.githubusercontent.com/52797753/153723496-8d03c5d3-601e-499d-80cd-51c3648957bf.png">
-
-## ♦️ Blue ♦️
-```py
-print(fade(banner, "blue"))
-```
-> <img width="475" alt="image" src="https://user-images.githubusercontent.com/52797753/153723092-0a32d8e6-680e-4df3-bdf1-089663f25f45.png">
-```py
-print(fade(banner, "blue-v"))
-```
-> <img width="475" alt="image" src="https://user-images.githubusercontent.com/52797753/153723509-41732010-b7d5-4867-95f9-690d47322536.png">
-
-## ♦️ Purple ♦️
-```py
-print(fade(banner, "purple"))
-```
-> <img width="475" alt="image" src="https://user-images.githubusercontent.com/52797753/153723148-2c94c459-1441-4752-a11f-a547754da7bc.png">
-```py
-print(fade(banner, "purple-v"))
-```
-> <img width="475" alt="image" src="https://user-images.githubusercontent.com/52797753/153723519-00aa980e-4a04-4d8d-a319-5691c1f8e517.png">
-
-## ♦️ Pink ♦️
-```py
-print(fade(banner, "pink-v"))
-```
-> <img width="475" alt="image" src="https://user-images.githubusercontent.com/52797753/153723540-b324dfe1-5ae2-4b66-ad3a-546a589558c8.png">
-
-## ♦️ Random ♦️
-```py
-print(fade(banner, "random"))
-```
-> <img width="475" alt="image" src="https://user-images.githubusercontent.com/52797753/153723545-0ea34ea7-1844-4ace-8948-3e71e28c0a30.png">
-
-<p>&nbsp;</p>    
-
----  
-
-# 🚨 Also check out 🚨
-<p align="center">
-  <a href="https://github.com/SirDank/dank.tool">
-  <img width="700" alt="image" src="https://user-images.githubusercontent.com/52797753/192086704-35f5a0db-3c5d-4782-95a9-6e2756cc8528.png">
-  </a>
-</p>
-
-<p>&nbsp;</p>    
-
----  
-
-# 🚨 Stats 🚨
-
-<br><p align="center"><img width="800" alt="image" src="https://repobeats.axiom.co/api/embed/ed44a86c2d46a8719705f5f57efde209b8cb5492.svg"></p><br>
-
-# 🚨 Star History 🚨
-
-<br><p align="center">[![Star History Chart](https://api.star-history.com/svg?repos=SirDank/dankware&type=Date)](https://star-history.com/#SirDank/dankware&Date)</p><br>
+Metadata-Version: 2.1
+Name: dankware
+Version: 3.3.5
+Summary: Python package with various features!
+Home-page: https://github.com/SirDank/dankware
+Author: SirDank
+Author-email: SirDankenstein@protonmail.com
+License: MIT
+Project-URL: GitHub, https://github.com/SirDank/dankware
+Project-URL: Bug Tracker, https://github.com/SirDank/dankware/issues
+Keywords: dank,dankware,multithread,gradient,fade,registry key,error traceback,random ip generator,github scraper,splash screen,hide window,file selector
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Natural Language :: English
+Classifier: Topic :: Software Development
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<p align="center">
+  <b>~ Visits ~</b><br><br>
+  <img src="https://profile-counter.glitch.me/dankware/count.svg" />
+</p>
+
+<p align="center">
+  <b>~ Stats ~</b><br><br>
+  <img src="https://static.pepy.tech/personalized-badge/dankware?period=total&units=international_system&left_color=black&right_color=brightgreen&left_text=downloads" />
+  <img src="https://static.pepy.tech/personalized-badge/dankware?period=month&units=international_system&left_color=black&right_color=brightgreen&left_text=downloads%20/%20month" />
+  <img src="https://static.pepy.tech/personalized-badge/dankware?period=week&units=international_system&left_color=black&right_color=brightgreen&left_text=downloads%20/%20week" />
+</p>
+
+# 🚨 dankware 🚨
+ Python module with various features! Install with the below command!
+```
+pip install dankware
+```
+
+Update to the latest version with the below command!
+```
+pip install --upgrade dankware
+```
+ 
+# 🚨 Multithreading 🚨
+```py
+from dankware import multithread
+import time
+
+a = 0
+def example():
+    global a
+    a += 1
+    print(a)
+    time.sleep(5)
+        
+multithread(example, 10) # func: example | threads: 10 | single: 50 seconds | multi: 5 seconds
+```
+> <img width="500" alt="image" src="https://user-images.githubusercontent.com/52797753/224534374-4693f9fb-2c0c-426b-970d-face9926b9cd.png">
+
+```py
+from dankware import multithread
+import time
+
+new_list = [1, 2, 3, 4, 5]; sum = 0
+
+def example(num):
+    global sum
+    sum += num
+    time.sleep(5)
+
+multithread(example, 10, new_list) # input_one: list
+print(sum)
+```
+> <img width="500" alt="image" src="https://user-images.githubusercontent.com/52797753/224534424-f03f5884-e9c8-445f-8c0a-5bb227c35aed.png">
+
+```py
+from dankware import multithread
+import time
+
+list1 = [1, 2, 3, 4, 5]
+list2 = [5, 4, 3, 2, 1]
+
+def example(num1, num2):
+    print(num1 + num2)
+    time.sleep(5)
+
+multithread(example, 10, list1, list2) # input_one: list1 | input_two: list2
+```
+> <img width="500" alt="image" src="https://user-images.githubusercontent.com/52797753/224534446-c956dfb0-81a2-4717-bd80-e04484e76507.png">
+
+```py
+from dankware import multithread
+import time
+
+new_list = [1, 2, 3, 4, 5]
+
+def example(num1, num2):
+    print(num1 * num2)
+    time.sleep(5)
+
+multithread(example, 10, new_list, 5, progress_bar=False) # input_two: 5 | disabled progress bar
+```
+> <img width="60" alt="image" src="https://user-images.githubusercontent.com/52797753/153749433-95512c4d-afcd-4ad7-9797-caded6e44239.png">
+
+<p>&nbsp;</p>    
+
+---  
+
+# 🚨 Export Registry Keys 🚨
+
+```py
+import os
+from dankware import export_registry_keys, is_admin
+
+# [NOTE]: this function requires admin privileges!
+
+export_path = "D:\\export.reg"
+registry_root = r'HKEY_CURRENT_USER'
+registry_path = r'Software\Google\Chrome\PreferenceMACs'
+#export_path = os.path.join(os.environ['USERPROFILE'], 'Desktop', 'export.reg')
+
+export_registry_keys(registry_root, registry_path, recursive=True, export_path=export_path)
+```
+> <img width="500" alt="image" src="https://user-images.githubusercontent.com/52797753/221345714-f1cdea4a-0c08-4c47-8c95-c64d95d12dec.png">
+
+> <img width="500" alt="image" src="https://user-images.githubusercontent.com/52797753/221345782-3a5a6ef0-d3b4-48a7-b8f8-c40f210b067d.png">
+
+<p>&nbsp;</p>    
+
+---  
+
+# 🚨 Splash Screen 🚨
+
+```py
+from dankware import splash_screen
+# Supports: GIFs / PNGs / JPGs / BMPs / ICOs
+splash_screen("D:\\splash.gif", duration=5)
+# runs on main thread
+```
+
+```py
+from dankware import splash_screen
+from concurrent.futures import ThreadPoolExecutor
+ThreadPoolExecutor(1).submit(splash_screen, "splash.png", 5)
+# runs on separate thread
+```
+
+> <img width="250" alt="image" src="https://user-images.githubusercontent.com/52797753/228445332-004f8f69-d8be-4d36-95e5-9065891e4d09.gif">
+
+# 🚨 Error Traceback 🚨
+
+```py
+import sys
+from dankware import err, clr
+try: value = 1/0
+except: print(clr(err(sys.exc_info()),2))
+```
+> <img width="700" alt="image" src="https://user-images.githubusercontent.com/52797753/221346044-db739b15-b365-47b3-b6f1-20d199c58ab2.png">
+
+<p>&nbsp;</p>    
+
+---  
+
+# 🚨 Scraping 🚨
+
+```py
+from dankware import github_downloads
+# full url > https://api.github.com/repos/EssentialsX/Essentials/releases/latest
+for url in github_downloads("EssentialsX/Essentials"): print(url)
+```
+> <img width="700" alt="image" src="https://user-images.githubusercontent.com/52797753/216242124-ed911013-bae4-4622-8c0a-0d11638da750.png">
+
+```py
+from dankware import github_file_selector
+# full url > https://api.github.com/repos/EssentialsX/Essentials/releases/latest
+for url in github_file_selector("EssentialsX/Essentials", "remove", ['AntiBuild', 'Discord', 'GeoIP', 'Protect', 'XMPP']): print(url)
+```
+> <img width="700" alt="image" src="https://user-images.githubusercontent.com/52797753/216241961-5359d662-a117-4eb4-b74e-e82b41a895bc.png">
+
+<p>&nbsp;</p>    
+
+---  
+
+# 🚨 Generate Random IPs 🚨
+
+```py
+from dankware import random_ip
+print(random_ip())
+```
+
+> <img width="200" alt="image" src="https://user-images.githubusercontent.com/52797753/194127781-8f622448-4595-4c2a-a3e7-3e4356076840.png">
+
+<p>&nbsp;</p>    
+
+---  
+
+# 🚨 Colour Special Characters 🚨
+
+```py
+from dankware import clr
+# default mode = 1
+# default colour_one = white
+# default colour_two = magenta
+print(clr("\n  > Hey! Long time no see :)"))
+#print(clr("\n  > Hey! Long time no see :)", colour_one = white, colour_two = magenta))
+```
+> <img width="350" alt="image" src="https://user-images.githubusercontent.com/52797753/153749617-bb0483fe-0385-490b-8695-72f448300c39.png">
+
+```py
+from dankware import clr, white, magenta
+# default mode = 1
+# default colour_one = white
+# default colour_two = magenta
+print(clr("\n  > Hey! Long time no see :)", colour_one = magenta, colour_two = white))
+```
+> <img width="350" alt="image" src="https://user-images.githubusercontent.com/52797753/220981909-d6361e6a-d109-447a-8401-85e2813e7859.png">
+
+```py
+from dankware import clr
+print(clr("\n  This is a string: True | This is an integer: False"))
+```
+> <img width="350" alt="image" src="https://user-images.githubusercontent.com/52797753/153749921-3332f3e6-eaa8-4bf1-ab4d-3fe35d245492.png">
+
+```py
+from dankware import clr, green, magenta
+# dankware now supports adding custom colours on both the text and the function itself!
+# colour_two = green
+print(clr(f"\n  > {magenta}Purple{white} thinks he's better than everyone else :(", colour_two=green))
+```
+> <img width="350" alt="image" src="https://user-images.githubusercontent.com/52797753/190898116-750e256e-a1d9-4c8a-a3b2-d0ac209fa0f7.png">
+
+```py
+from dankware import clr
+# mode = 2
+print(clr("\n  > Error in sector [7] redirecting... | INTEGRITY_CHECK_SUCCESS: TRUE",2))
+```
+> <img width="500" alt="image" src="https://user-images.githubusercontent.com/52797753/153749821-ae3e4dfd-26dc-4e08-a06e-677ac26457a1.png">
+
+```py
+from dankware import clr
+# mode = 3
+print(clr("\n  > Is this a randomly coloured string: TRUE | As you can see it does not colour True/False",3))
+```
+> <img width="650" alt="image" src="https://user-images.githubusercontent.com/52797753/155293415-7b065b5a-44dd-4fe7-995d-a25582f904cb.png">
+
+<p>&nbsp;</p>    
+
+---  
+
+# 🚨 Banners 🚨
+
+```py
+banner = '''
+
+     888                   888                                             
+     888                   888           s i r . d a n k ' s               
+     888                   888                                             
+ .d88888  8888b.  88888b.  888  888 888  888  888  8888b.  888d888 .d88b.  
+d88" 888     "88b 888 "88b 888 .88P 888  888  888     "88b 888P"  d8P  Y8b 
+888  888 .d888888 888  888 888888K  888  888  888 .d888888 888    88888888 
+Y88b 888 888  888 888  888 888 "88b Y88b 888 d88P 888  888 888    Y8b.     
+ "Y88888 "Y888888 888  888 888  888  "Y8888888P"  "Y888888 888     "Y8888  
+
+'''
+```
+
+## ♦️ Colourize Banner (random) ♦️
+```py
+from dankware import clr
+# mode = 4
+print(clr(banner,4))
+```
+> <img width="550" alt="image" src="https://user-images.githubusercontent.com/52797753/153722086-2f372bfa-4872-46a0-81f8-cdf7c2344fd6.png">
+
+## ♦️ Align Banner (console center) ♦️
+```py
+from dankware import align
+print(align(banner)) # also works with single text line (even coloured)
+```
+> <img width="800" alt="image" src="https://user-images.githubusercontent.com/52797753/153722230-1f3b6103-6d8a-4537-9828-1718a6bd3367.png">
+
+## ♦️ Align Coloured Banner ♦️
+```py
+from dankware import align, clr
+print(align(clr(banner,4)))
+```
+> <img width="800" alt="image" src="https://user-images.githubusercontent.com/52797753/153722373-9925dd25-83bb-4d1c-83eb-bfaae1802088.png">
+
+<p>&nbsp;</p>    
+
+---  
+
+# 🚨 Gradient Reworked [ Originally By @venaxyt ] 🚨
+
+```py
+from dankware import fade
+banner = '''
+
+                              888 d8b                   888    
+       v e n a x y t ' s      888 Y8P                   888    
+                              888                       888    
+ .d88b.  888d888 8888b.   .d88888 888  .d88b.  88888b.  888888 
+d88P"88b 888P"      "88b d88" 888 888 d8P  Y8b 888 "88b 888    
+888  888 888    .d888888 888  888 888 88888888 888  888 888    
+Y88b 888 888    888  888 Y88b 888 888 Y8b.     888  888 Y88b.  
+ "Y88888 888    "Y888888  "Y88888 888  "Y8888  888  888  "Y888 
+     888                                                       
+Y8b d88P                                                       
+ "Y88P"                                                        
+
+
+'''
+```
+
+## ♦️ Black ♦️
+```py
+print(fade(banner, "black"))
+```
+> <img width="475" alt="image" src="https://user-images.githubusercontent.com/52797753/153722811-b257611e-9111-4a0e-92fb-7dbe503ce6db.png">
+```py
+print(fade(banner, "black-v"))
+```
+> <img width="475" alt="image" src="https://user-images.githubusercontent.com/52797753/153723205-a91eb1c6-07bc-4bc6-9fa6-52231e50a25c.png">
+
+## ♦️ Red ♦️
+```py
+print(fade(banner, "red"))
+```
+> <img width="475" alt="image" src="https://user-images.githubusercontent.com/52797753/153722946-3221bfd8-ff9d-4c9d-8b70-0c2736ec4e30.png">
+```py
+print(fade(banner, "red-v"))
+```
+> <img width="475" alt="image" src="https://user-images.githubusercontent.com/52797753/153723473-bdb75ea7-2df2-4f70-adb5-cf5caa57200a.png">
+
+## ♦️ Green ♦️
+```py
+print(fade(banner, "green"))
+```
+> <img width="475" alt="image" src="https://user-images.githubusercontent.com/52797753/153723050-c30bd3f1-989a-4141-b40a-2869a2dadef6.png">
+```py
+print(fade(banner, "green-v"))
+```
+> <img width="475" alt="image" src="https://user-images.githubusercontent.com/52797753/153723481-2e5c21b2-0f12-4d99-ab8d-a3e5c40e4c16.png">
+
+## ♦️ Cyan ♦️
+```py
+print(fade(banner, "cyan"))
+```
+> <img width="475" alt="image" src="https://user-images.githubusercontent.com/52797753/153723059-b4808365-6006-4726-b427-b6848e0fc0e5.png">
+```py
+print(fade(banner, "cyan-v"))
+```
+> <img width="475" alt="image" src="https://user-images.githubusercontent.com/52797753/153723496-8d03c5d3-601e-499d-80cd-51c3648957bf.png">
+
+## ♦️ Blue ♦️
+```py
+print(fade(banner, "blue"))
+```
+> <img width="475" alt="image" src="https://user-images.githubusercontent.com/52797753/153723092-0a32d8e6-680e-4df3-bdf1-089663f25f45.png">
+```py
+print(fade(banner, "blue-v"))
+```
+> <img width="475" alt="image" src="https://user-images.githubusercontent.com/52797753/153723509-41732010-b7d5-4867-95f9-690d47322536.png">
+
+## ♦️ Purple ♦️
+```py
+print(fade(banner, "purple"))
+```
+> <img width="475" alt="image" src="https://user-images.githubusercontent.com/52797753/153723148-2c94c459-1441-4752-a11f-a547754da7bc.png">
+```py
+print(fade(banner, "purple-v"))
+```
+> <img width="475" alt="image" src="https://user-images.githubusercontent.com/52797753/153723519-00aa980e-4a04-4d8d-a319-5691c1f8e517.png">
+
+## ♦️ Pink ♦️
+```py
+print(fade(banner, "pink-v"))
+```
+> <img width="475" alt="image" src="https://user-images.githubusercontent.com/52797753/153723540-b324dfe1-5ae2-4b66-ad3a-546a589558c8.png">
+
+## ♦️ Random ♦️
+```py
+print(fade(banner, "random"))
+```
+> <img width="475" alt="image" src="https://user-images.githubusercontent.com/52797753/153723545-0ea34ea7-1844-4ace-8948-3e71e28c0a30.png">
+
+<p>&nbsp;</p>    
+
+---  
+
+# 🚨 Also check out 🚨
+<p align="center">
+  <a href="https://github.com/SirDank/dank.tool">
+  <img width="700" alt="image" src="https://user-images.githubusercontent.com/52797753/192086704-35f5a0db-3c5d-4782-95a9-6e2756cc8528.png">
+  </a>
+</p>
+
+<p>&nbsp;</p>    
+
+---  
+
+# 🚨 Stats 🚨
+
+<br><p align="center"><img width="800" alt="image" src="https://repobeats.axiom.co/api/embed/ed44a86c2d46a8719705f5f57efde209b8cb5492.svg"></p><br>
+
+# 🚨 Star History 🚨
+
+<br><p align="center">[![Star History Chart](https://api.star-history.com/svg?repos=SirDank/dankware&type=Date)](https://star-history.com/#SirDank/dankware&Date)</p><br>
```

### Comparing `dankware-3.3.4/dankware/__init__.py` & `dankware-3.3.5/dankware/__init__.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,969 +1,969 @@
-###################################################################################
-
-#                            https://github.com/SirDank                            
-
-###################################################################################
-
-# > Please read the documentation on github before using this module!
-
-import os
-import sys
-import time
-import random
-from datetime import datetime
-from colorama import Fore, Style
-
-# colorama colours
-
-black = Fore.BLACK + Style.BRIGHT
-blue = Fore.BLUE + Style.BRIGHT
-cyan = Fore.CYAN + Style.BRIGHT
-green = Fore.GREEN + Style.BRIGHT
-magenta = Fore.MAGENTA + Style.BRIGHT
-red = Fore.RED + Style.BRIGHT
-reset = Style.RESET_ALL
-white = Fore.WHITE + Style.BRIGHT
-yellow = Fore.YELLOW + Style.BRIGHT
-
-# dankware variables
-
-chars = ['>','<','.',',','=','-','_','?','!','|','(',')','{','}','/','\\',':','"',"'","%"]
-words_green = ['true', 'True', 'TRUE', 'online', 'Online', 'ONLINE', 'successfully', 'Successfully', 'SUCCESSFULLY', 'successful', 'Successful', 'SUCCESSFUL', 'success', 'Success', 'SUCCESS']
-words_red = ['falsely', 'Falsely', 'FALSELY', 'false', 'False', 'FALSE', 'offline', 'Offline', 'OFFLINE', 'failures', 'Failures', 'FAILURES', 'failure', 'Failure', 'FAILURE', 'failed', 'Failed', 'FAILED', 'fail', 'Fail', 'FAIL']
-colours_to_replace = [Fore.BLACK, Fore.BLUE, Fore.CYAN, Fore.GREEN, Fore.MAGENTA, Fore.RED, Fore.WHITE, Fore.YELLOW, Style.BRIGHT, Style.RESET_ALL]
-colours_alt = ["BBLACKK", "BBLUEE", "CCYANN", "GGREENN", "MMAGENTAA", "RREDD", "WWHITEE", "YYELLOWW", "BBRIGHTT", "RRESETT"]
-bad_colours = ['BLACK', 'WHITE', 'LIGHTBLACK_EX', 'LIGHTWHITE_EX', 'RESET']
-codes = vars(Fore); colours = [codes[colour] for colour in codes if colour not in bad_colours]
-styles = [Style.BRIGHT, Style.DIM, Style.NORMAL]
-available_colours = ['black','red','green','cyan','blue','purple','random','black-v','red-v','green-v','cyan-v','blue-v','purple-v','pink-v']
-
-excluded_prefixes_one = {'6.': '', '7.': '', '10.': '', '11.': '', '21.': '', '22.': '', '26.': '', '28.': '', '29.': '', '30.': '', '33.': '', '55.': '', '127.': '', '136.': '', '205.': '', '214.': '', '215.': ''}
-excluded_prefixes_two = {'23.27.': '', '31.25.': '', '50.117.': '', '74.115.': '', '75.127.': '', '81.87.': '', '100.64.': '', '128.16.': '', '128.40.': '', '128.41.': '', '128.86.': '', '128.232.': '', '128.240.': '', '128.243.': '', '129.11.': '', '129.12.': '', '129.31.': '', '129.67.': '', '129.123.': '', '129.169.': '', '129.215.': '', '129.234.': '', '130.88.': '', '130.159.': '', '130.209.': '', '130.246.': '', '131.111.': '', '131.227.': '', '131.231.': '', '131.251.': '', '134.36.': '', '134.83.': '', '134.151.': '', '134.219.': '', '134.220.': '', '134.225.': '', '136.148.': '', '136.156.': '', '137.44.': '', '137.50.': '', '137.73.': '', '137.108.': '', '137.195.': '', '137.222.': '', '137.253.': '', '138.38.': '', '138.40.': '', '138.250.': '', '138.253.': '', '139.133.': '', '139.153.': '', '139.166.': '', '139.184.': '', '139.222.': '', '140.97.': '', '141.163.': '', '141.241.': '', '142.111.': '', '142.252.': '', '143.52.': '', '143.117.': '', '143.167.': '', '143.210.': '', '143.234.': '', '144.32.': '', '144.39.': '', '144.82.': '', '144.124.': '', '144.173.': '', '146.87.': '', '146.97.': '', '146.169.': '', '146.176.': '', '146.179.': '', '146.191.': '', '146.227.': '', '147.143.': '', '147.188.': '', '147.197.': '', '148.79.': '', '148.88.': '', '148.197.': '', '149.155.': '', '149.170.': '', '150.204.': '', '152.71.': '', '152.78.': '', '152.105.': '', '153.11.': '', '155.198.': '', '155.245.': '', '157.140.': '', '157.228.': '', '158.94.': '', '158.125.': '', '158.143.': '', '158.223.': '', '159.92.': '', '160.5.': '', '160.9.': '', '161.73.': '', '161.74.': '', '161.76.': '', '161.112.': '', '163.1.': '', '163.119.': '', '163.160.': '', '163.167.': '', '164.11.': '', '165.160.': '', '166.88.': '', '169.254.': '', '172.252.': '', '192.168.': '', '192.177.': '', '192.186.': '', '193.60.': '', '194.66.': '', '194.80.': '', '195.194.': '', '198.18.': '', '205.164.': '', '212.121.': '', '212.219.': ''}
-excluded_prefixes_three = {'4.53.201.': '', '5.152.179.': '', '8.12.162.': '', '8.12.163.': '', '8.12.164.': '', '8.14.84.': '', '8.14.145.': '', '8.14.146.': '', '8.14.147.': '', '8.17.250.': '', '8.17.251.': '', '8.17.252.': '', '23.231.128.': '', '31.25.2.': '', '31.25.4.': '', '37.72.112.': '', '37.72.172.': '', '38.72.200.': '', '46.254.200.': '', '50.93.192.': '', '50.93.193.': '', '50.93.194.': '', '50.93.195.': '', '50.93.196.': '', '50.93.197.': '', '50.115.128.': '', '50.118.128.': '', '63.141.222.': '', '64.62.253.': '', '64.92.96.': '', '64.145.79.': '', '64.145.82.': '', '64.158.146.': '', '65.49.24.': '', '65.49.93.': '', '65.162.192.': '', '66.79.160.': '', '66.160.191.': '', '68.68.96.': '', '69.46.64.': '', '69.176.80.': '', '72.13.80.': '', '72.52.76.': '', '74.82.43.': '', '74.82.160.': '', '74.114.88.': '', '74.115.2.': '', '74.115.4.': '', '74.122.100.': '', '85.12.64.': '', '89.207.208.': '', '92.245.224.': '', '103.251.91.': '', '108.171.32.': '', '108.171.42.': '', '108.171.52.': '', '108.171.62.': '', '118.193.78.': '', '130.93.16.': '', '132.206.9.': '', '132.206.123.': '', '132.206.125.': '', '141.170.64.': '', '141.170.96.': '', '141.170.100.': '', '146.82.55.93': '', '149.54.136.': '', '149.54.152.': '', '159.86.128.': '', '173.245.64.': '', '173.245.194.': '', '173.245.220.': '', '173.252.192.': '', '178.18.16.': '', '178.18.26.': '', '178.18.27.': '', '178.18.28.': '', '178.18.29.': '', '183.182.22.': '', '185.83.168.': '', '192.12.72.': '', '192.18.195.': '', '192.35.172.': '', '192.41.104.': '', '192.41.112.': '', '192.41.128.': '', '192.68.153.': '', '192.76.6.': '', '192.76.8.': '', '192.76.16.': '', '192.76.32.': '', '192.82.153.': '', '192.84.5.': '', '192.84.75.': '', '192.84.76.': '', '192.84.80.': '', '192.84.212.': '', '192.88.9.': '', '192.88.10.': '', '192.88.99.': '', '192.92.114.': '', '192.94.235.': '', '192.100.78.': '', '192.100.154.': '', '192.107.168.': '', '192.108.120.': '', '192.124.46.': '', '192.133.244.': '', '192.149.111.': '', '192.150.180.': '', '192.150.184.': '', '192.153.213.': '', '192.155.160.': '', '192.156.162.': '', '192.160.194.': '', '192.171.128.': '', '192.171.192.': '', '192.173.1.': '', '192.173.2.': '', '192.173.4.': '', '192.173.128.': '', '192.188.157.': '', '192.188.158.': '', '192.190.201.': '', '192.190.202.': '', '192.195.42.': '', '192.195.105.': '', '192.195.116.': '', '192.195.118.': '', '192.249.64.': '', '192.250.240.': '', '193.32.22.': '', '193.37.225.': '', '193.37.240.': '', '193.38.143.': '', '193.39.80.': '', '193.39.172.': '', '193.39.212.': '', '193.107.116.': '', '193.130.15.': '', '193.133.28.': '', '193.138.86.': '', '194.32.32.': '', '194.35.93.': '', '194.35.186.': '', '194.35.192.': '', '194.35.241.': '', '194.36.1.': '', '194.36.2.': '', '194.36.121.': '', '194.36.152.': '', '194.60.218.': '', '194.110.214.': '', '194.187.32.': '', '198.12.120.': '', '198.12.121.': '', '198.12.122.': '', '198.51.100.': '', '198.144.240.': '', '199.33.120.': '', '199.33.124.': '', '199.48.147.': '', '199.68.196.': '', '199.127.240.': '', '199.187.168.': '', '199.188.238.': '', '199.255.208.': '', '203.12.6.': '', '204.13.64.': '', '204.16.192.': '', '204.19.238.': '', '204.74.208.': '', '204.113.91.': '', '205.159.189.': '', '205.209.128.': '', '206.108.52.': '', '206.165.4.': '', '208.77.40.': '', '208.80.4.': '', '208.123.223.': '', '209.51.185.': '', '209.54.48.': '', '209.107.192.': '', '209.107.210.': '', '209.107.212.': '', '211.156.110.': '', '212.121.192.': '', '216.151.183.': '', '216.151.190.': '', '216.172.128.': '', '216.185.36.': '', '216.218.233.': '', '216.224.112.': ''}
-
-def multithread(function: callable, threads: int = 1, *args, progress_bar: bool = True) -> None:
-    
-    """
-    > Please read the documentation on github before using this function!
-    
-    ________________________________________________________________________________
-
-    Run the given function in multiple threads with the specified inputs.
-
-    - function: The function to run in multiple threads.
-    - threads: The number of threads to use.
-    - *args: Input(s) for the function. Can be a list, a single value.
-    - progress_bar: Whether to display a progress bar.
-    """
-    
-    from rich.live import Live
-    from rich.panel import Panel
-    from rich.table import Table
-    from shutil import get_terminal_size
-    from concurrent.futures import ThreadPoolExecutor, as_completed
-    from rich.progress import Progress, SpinnerColumn, BarColumn, TextColumn, TimeRemainingColumn, TimeElapsedColumn
-
-    try:
-        
-        def submit_task(executor, *args):
-            return executor.submit(function, *args)
-        
-        if threads < 1:
-            raise ValueError("The number of threads must be a positive integer.")
-
-        futures = []
-        executor = ThreadPoolExecutor(max_workers=threads)
-
-        if not args:
-            for _ in range(threads): futures.append(executor.submit(function))
-        else:
-            input_lists = []
-            for arg in args:
-                if isinstance(arg, list):
-                    input_lists.append(arg)
-                else:
-                    input_lists.append([arg] * threads)
-
-            for task_args in zip(*input_lists):
-                futures.append(submit_task(executor, *task_args))
-
-        if progress_bar:
-            width = get_terminal_size().columns
-            job_progress = Progress("{task.description}", SpinnerColumn(), BarColumn(bar_width=width), TextColumn("[deep_pink1][progress.percentage][bright_cyan]{task.percentage:>3.0f}%"), "[bright_cyan]ETA", TimeRemainingColumn(), TimeElapsedColumn())
-            overall_task = job_progress.add_task("[bright_green]Progress", total=int(len(futures)))
-            progress_table = Table.grid()
-            progress_table.add_row(Panel.fit(job_progress, title="[bright_red]Jobs", border_style="magenta1", padding=(1, 2)))
-
-            with Live(progress_table, refresh_per_second=10):
-                while not job_progress.finished:
-                    time.sleep(0.1)
-                    for future in as_completed(futures):
-                        if future.done():
-                            try: future.result()
-                            except: pass
-                            job_progress.advance(overall_task)
-
-        else:
-            for future in as_completed(futures):
-                if future.done():
-                    try: future.result()
-                    except: pass
-                
-    except: 
-        try: executor.shutdown()
-        except: pass
-        sys.exit(clr(err(sys.exc_info()),2))
-
-# --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
-
-def github_downloads(user_repo: str) -> list:
-
-    """
-    Extracts direct download urls from the latest release on github and returns it as a list
-
-    - Example Input: USER_NAME/REPO_NAME ( from https://api.github.com/repos/USER_NAME/REPO_NAME/releases/latest )
-    - Example Output: ['https://github.com/USER_NAME/REPO_NAME/releases/download/VERSION/EXAMPLE.TXT']
-    
-    _____________________________________________________________________________________________________________________________________
-    
-    [ EXAMPLE ]
-    ```python
-    from dankware import github_downloads
-    for _ in github_downloads("SirDank/dank.tool"): print(_)
-    ```
-    """
-    
-    import requests
-    
-    urls = []
-
-    #if "https://api.github.com/repos/" not in url or "/releases/latest" not in url:
-    #    raise ValueError(clr('  > Invalid url! Must follow: "https://api.github.com/repos/NAME/NAME/releases/latest"',2)) 
-    while True:
-        try: response = requests.get(f"https://api.github.com/repos/{user_repo}/releases/latest").json(); break
-        except: input(clr("  > Make sure you are connected to the Internet! Press [ENTER] to try again... ",2))
-    
-    for data in response["assets"]:
-        urls.append(data["browser_download_url"])
-
-    return urls
-
-# --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
-
-def github_file_selector(user_repo: str, filter_mode: str, name_list: list) -> list:
-    
-    """
-    
-    This function is used to filter the output from github_downloads()
-    
-    - user_repo = 'USER_NAME/REPO_NAME' ( from https://api.github.com/repos/USER_NAME/REPO_NAME/releases/latest )
-    - filter_mode = 'add' or 'remove'
-    - name_list = list of names to be added or removed
-    
-    _______________________________________________________________________________________________________________________________________________________________________
-    
-    [ EXAMPLE ]
-    ```python
-    from dankware import github_file_selector
-    for file_url in github_file_selector("EssentialsX/Essentials", "remove", ['AntiBuild', 'Discord', 'GeoIP', 'Protect', 'XMPP']):
-        print(file_url)
-    ```
-    
-    _______________________________________________________________________________________________________________________________________________________________________
-    
-    Example output from github_downloads("EX_USER/EX_REPO"): [
-        'https://github.com/EX_USER/EX_REPO/releases/download/VERSION/EXAMPLE.TXT'
-        'https://github.com/EX_USER/EX_REPO/releases/download/VERSION/EXAMPLE_2.TXT'
-        'https://github.com/EX_USER/EX_REPO/releases/download/VERSION/EXAMPLE_3.TXT'
-        'https://github.com/EX_USER/EX_REPO/releases/download/VERSION/TEST.TXT'
-        'https://github.com/EX_USER/EX_REPO/releases/download/VERSION/TEST_2.TXT'
-        'https://github.com/EX_USER/EX_REPO/releases/download/VERSION/TEST_3.TXT'
-    ]
-    
-    _______________________________________________________________________________________________________________________________________________________________________
-    
-    Example Input: "EX_USER/EX_REPO", "add", ["EXAMPLE"]
-        
-    Example Output: [
-        'https://github.com/EX_USER/EX_REPO/releases/download/VERSION/EXAMPLE.TXT'
-        'https://github.com/EX_USER/EX_REPO/releases/download/VERSION/EXAMPLE_2.TXT'
-        'https://github.com/EX_USER/EX_REPO/releases/download/VERSION/EXAMPLE_3.TXT'
-    ]
-        
-    - Note: Only urls with filenames containing "EXAMPLE" were returned.
-
-    _______________________________________________________________________________________________________________________________________________________________________
-
-    Example Input: "EX_USER/EX_REPO", "remove", ["EXAMPLE"]
-    
-    Example Output: [
-        'https://github.com/EX_USER/EX_REPO/releases/download/VERSION/TEST.TXT'
-        'https://github.com/EX_USER/EX_REPO/releases/download/VERSION/TEST_2.TXT'
-        'https://github.com/EX_USER/EX_REPO/releases/download/VERSION/TEST_3.TXT'
-    ]
-    
-    - Note: Only urls with filenames not containing "EXAMPLE" were returned.
-    
-    """
-
-    urls = []
-    for file_url in github_downloads(user_repo):
-        if filter_mode == "add": valid = False
-        elif filter_mode == "remove": valid = True
-        for name in name_list:
-            if name in file_url.split('/')[-1]:
-                if filter_mode == "add": valid = True
-                elif filter_mode == "remove": valid = False
-        if valid: urls.append(file_url)
-    return urls
-
-# --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
-
-def random_ip() -> str:
-    
-    """
-    Generates a random valid computer ip
-    - Follows: https://github.com/robertdavidgraham/masscan/blob/master/data/exclude.conf
-    """
-    
-    while True:
-        
-        first_octet = random.randint(1, 223)
-        second_octet = random.randint(0, 255)
-        third_octet = random.randint(0, 255)
-        fourth_octet = random.randint(0, 255)
-
-        if f"{first_octet}." in excluded_prefixes_one.keys(): continue
-        elif f"{first_octet}.{second_octet}." in excluded_prefixes_two.keys(): continue
-        elif f"{first_octet}.{second_octet}.{third_octet}" in excluded_prefixes_three.keys(): continue
-        
-        if first_octet == 172 and second_octet >= 16 and second_octet <= 31: continue
-        elif first_octet == 192:
-            if fourth_octet == 170 or fourth_octet == 171 or third_octet == 2: continue
-        elif first_octet == 203 and third_octet == 113: continue
-        elif first_octet == 216 and second_octet == 83 and third_octet >= 33 and third_octet <= 63: continue
-        elif second_octet == 255 and third_octet == 255 and third_octet == 255: continue
-
-        break
-    
-    ip = f"{first_octet}.{second_octet}.{third_octet}.{fourth_octet}"
-        
-    return ip
-
-# --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
-
-def is_admin() -> bool:
-    
-    import ctypes
-    
-    """
-    Checks if the current user has admin privileges and returns True if found else False
-    """
-    
-    try: return ctypes.windll.shell32.IsUserAnAdmin()
-    except: return False
-    
-'''
-def run_as_admin() -> None:
-    
-    """
-    Executes the script with admin privileges
-    """
-    
-    ctypes.windll.shell32.ShellExecuteW(None, "runas", sys.executable, __file__, None, 1)
-    #sys.exit(clr("\n  > Exiting original un-elevated script...",2))
-'''
-
-# --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
-
-def export_registry_keys(registry_root: str, registry_path: str, recursive: bool = True, export_path: str = "export.reg") -> None:
-
-    """
-    Function to export registry keys with or without its subkeys and saves them to export_path
-    - Examples for registry_root: 'HKEY_CLASSES_ROOT', 'HKEY_CURRENT_USER', 'HKEY_LOCAL_MACHINE', 'HKEY_USERS', 'HKEY_CURRENT_CONFIG'
-    - Example for registry_path: r'Software\Google\Chrome\PreferenceMACs'
-    - recursive: True (subkeys saved)
-    - recursive: False (subkeys not saved)
-    - export_path: "exported.reg" (default)
-    
-    _______________________________________________________________________________________________________________________________________________________________________
-    
-    [ EXAMPLE ]
-    
-    ```python
-    from dankware import export_registry_keys
-    export_registry_keys('HKEY_CURRENT_USER', r'Software\Google\Chrome\PreferenceMACs')
-    ```
-    """
-
-    import winreg
-    
-    try:
-    
-        key_data = []
-        key_map = {
-            'HKEY_CLASSES_ROOT': winreg.HKEY_CLASSES_ROOT,
-            'HKEY_CURRENT_USER': winreg.HKEY_CURRENT_USER,
-            'HKEY_LOCAL_MACHINE': winreg.HKEY_LOCAL_MACHINE,
-            'HKEY_USERS': winreg.HKEY_USERS,
-            'HKEY_CURRENT_CONFIG': winreg.HKEY_CURRENT_CONFIG,
-        }
-        
-        if not export_path.endswith('.reg'):
-            raise ValueError("Invalid Export Path! export_path must end with '.reg'")
-        if registry_root not in key_map.keys():
-            raise ValueError(f"Invalid Registry Root! Use one of the following: {', '.join(key_map.keys())}")
-        if not is_admin():
-            raise RuntimeError("Current user is not an administrator! Exporting registry keys requires admin privileges!")
-            # If the current user is not an admin, relaunch the script with admin privileges
-            #run_as_admin()
-            
-        def exporter(key, registry_root, subkey_path, key_data, recursive) -> None:
-
-            subkey = winreg.OpenKey(key, subkey_path, 0, winreg.KEY_READ | winreg.KEY_WOW64_64KEY)
-            subkey_count = winreg.QueryInfoKey(subkey)[0]
-            key_data.append(f'[{registry_root}\\{subkey_path}]')
-    
-            for i in range(winreg.QueryInfoKey(subkey)[1]):
-                value_name, value_data, value_type = winreg.EnumValue(subkey, i)
-                key_data.append(f'"{value_name}"="{value_data}"')
-
-            key_data.append('')
-            for i in range(subkey_count):
-                subkey_name = winreg.EnumKey(subkey, i)
-                subkey_full_path = subkey_path + '\\' + subkey_name if subkey_path else subkey_name
-                if recursive: exporter(key, registry_root, subkey_full_path, key_data, recursive)
-
-            winreg.CloseKey(subkey)
-
-        key = key_map[registry_root]
-        exporter(key, registry_root, registry_path, key_data, recursive)
-        open(export_path, 'w', encoding='utf-16').write('Windows Registry Editor Version 5.00\n\n' + '\n'.join(key_data))
-        print(clr(f"\n  > Successfully exported registry keys to \"{os.path.join(os.getcwd(), 'export.reg') if export_path == 'export.reg' else export_path}\""))
-    
-    except: sys.exit(clr(err(sys.exc_info()),2))
-
-# --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
-
-def clr(text: str, mode: int = 1, colour_one: str = white, colour_two: str = magenta) -> str:
-    
-    """
-    
-    this function colours special characters inside the 'chars' list
-    
-    ___________________________________________
-    
-    - mode: 1 | to display general text (default)
-    - text = white (default) / specified colour
-    - spl = magenta (default) / specified colour
-
-    ___________________________________________
-
-    - mode: 2 | to display error messages
-    - text = red (fixed colour)
-    - spl = white (fixed colour)
-
-    ___________________________________________
-
-    - mode: 3
-    - text = random (fixed colour)
-    - spl = white (fixed colour)
-
-    ___________________________________________
-
-    - mode: 4 | to display banners
-    - text & spl = random (fixed colour)
-    
-    """
-    
-    try:
-        if mode != 3:
-            for _ in range(len(colours_to_replace)):
-                text = text.replace(colours_to_replace[_], colours_alt[_])
-        else:
-            for _ in range(len(colours_to_replace)):
-                text = text.replace(colours_to_replace[_], '')
-
-        # default
-
-        if mode == 1:
-            text = text.replace("[",f"{colour_two}[{colour_one}").replace("]",f"{colour_two}]{colour_one}")
-            for char in chars: text = text.replace(char, f"{colour_two}{char}{colour_one}")
-            for word in words_green:
-                replacement = green.join(list(word))
-                text = text.replace(word, f"{green}{replacement}{colour_one}")
-            for word in words_red:
-                replacement = red.join(list(word))
-                text = text.replace(word, f"{red}{replacement}{colour_one}")
-        
-        # for error messages
-        
-        elif mode == 2:
-            text = text.replace("[",f"{white}[{red}").replace("]",f"{white}]{red}")
-            for char in chars: text = text.replace(char, f"{white}{char}{red}")
-            #for word in words_green: text = text.replace(word, f"{green}{word}{red}")
-        
-        # random | TRUE, FALSE will not be coloured!
-        
-        elif mode == 3 or mode == 4:
-            text = [char for char in text]
-            if mode == 3: colour_spl = True
-            else: colour_spl = False
-            for _ in range(len(text)):
-                char = text[_]
-                if char != ' ' and char != '\n':
-                    if colour_spl:
-                        if char in ( ['[',']'] + chars ): text[_] = white + char
-                        else: text[_] = random.choice(colours) + Style.BRIGHT + char
-                    else:
-                        text[_] = random.choice(colours) + Style.BRIGHT + char
-            text = ''.join(text)
-
-        else: raise ValueError(f"\n  {white}> {red}Invalid Mode {white}[{red}{mode}{white}] | Valid Modes{white}: {red}1{white},{red}2{white},{red}3{white},{red}4" + reset)
-
-        if mode != 3:
-            for _ in range(len(colours_to_replace)):
-                text = str(text).replace(colours_alt[_], colours_to_replace[_])
-
-        if mode == 1: return white + text + reset
-        elif mode == 2: return red + text + reset
-        elif mode == 3 or mode == 4: return text + reset
-    
-    except: sys.exit(clr(err(sys.exc_info()),2))
-
-# --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
-
-def align(text: str) -> str: 
-    
-    """
-    center align banner / line ( supports both coloured and non-coloured )
-    - [NOTE] align supports: clr, does not support: fade
-    """
-    
-    from shutil import get_terminal_size
-
-    width = get_terminal_size().columns; aligned = text
-    for colour in vars(Fore).values(): aligned = aligned.replace(colour,'')
-    for style in vars(Style).values(): aligned = aligned.replace(style,'')
-    text = text.split('\n'); aligned = aligned.split('\n')
-    for _ in range(len(aligned)): aligned[_] = aligned[_].center(width).replace(aligned[_],text[_])
-    return str('\n'.join(aligned) + reset)
-
-# --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
-
-def fade(text: str, colour: str = "purple") -> str:
-    
-    """
-    credits to https://github.com/venaxyt/gratient & https://github.com/venaxyt/fade <3
-    - available_colours = black, red, green, cyan, blue, purple, random, black-v, red-v, green-v, cyan-v, blue-v, purple-v, pink-v
-    """
-
-    try:
-        colour = colour.lower()
-        if not colour in available_colours: raise ValueError(clr(f"\n  > Invalid Colour: {colour} | Available Colours: {', '.join(available_colours)}",2))
-            
-        faded = ""
-        if len(text.splitlines()) > 1: multi_line = True
-        else: multi_line = False
-
-        if colour == "black":
-            for line in text.splitlines():
-                R = 0; G = 0; B = 0
-                for char in line:
-                    R += 3; G += 3; B += 3
-                    if R > 255 and G > 255 and B > 255: R = 255; G = 255; B = 255
-                    faded += f"\033[38;2;{R};{G};{B}m{char}\033[0m"
-                if multi_line: faded += "\n"
-                
-        elif colour == "red":
-            for line in text.splitlines():
-                G = 250
-                for char in line:
-                    G -= 5
-                    if G < 0: G = 0
-                    faded += f"\033[38;2;255;{G};0m{char}\033[0m"
-                if multi_line: faded += "\n"
-                
-        elif colour == "green":
-            for line in text.splitlines():
-                R = 0
-                for char in line:
-                    if not R > 200: R += 3
-                    faded += f"\033[38;2;{R};255;0m{char}\033[0m"
-                if multi_line: faded += "\n"
-                
-        elif colour == "cyan":
-            for line in text.splitlines():
-                B = 100
-                for char in line:
-                    B += 2
-                    if B > 255: B = 255
-                    faded += f"\033[38;2;0;255;{B}m{char}\033[0m"
-                if multi_line: faded += "\n"
-
-        elif colour == "blue":
-            for line in text.splitlines():
-                G = 0
-                for char in line:
-                    G += 3
-                    if G > 255: G = 255
-                    faded += f"\033[38;2;0;{G};255m{char}\033[0m"
-                if multi_line: faded += "\n"
-            
-        elif colour == "purple":
-            for line in text.splitlines():
-                R = 35
-                for char in line:
-                    R += 3
-                    if R > 255: R = 255
-                    faded += f"\033[38;2;{R};0;220m{char}\033[0m"
-                if multi_line: faded += "\n"
-
-        elif colour == "black-v":
-            R = 0; G = 0; B = 0
-            for line in text.splitlines():
-                faded += (f"\033[38;2;{R};{G};{B}m{line}\033[0m")
-                if not R == 255 and not G == 255 and not B == 255:
-                    R += 20; G += 20; B += 20
-                    if R > 255 and G > 255 and B > 255: R = 255; G = 255; B = 255
-                if multi_line: faded += "\n"
-                        
-        elif colour == "red-v":
-            G = 250
-            for line in text.splitlines():
-                faded += f"\033[38;2;255;{G};0m{line}\033[0m"
-                if not G == 0:
-                    G -= 25
-                    if G < 0: G = 0
-                if multi_line:faded += "\n"
-
-        elif colour == "green-v":
-            R = 0
-            for line in text.splitlines():
-                faded += f"\033[38;2;{R};255;0m{line}\033[0m"
-                if not R > 200: R += 30
-                if multi_line: faded += "\n"
-            
-        elif colour == "cyan-v":
-            B = 100
-            for line in text.splitlines():
-                faded += f"\033[38;2;0;255;{B}m{line}\033[0m"
-                if not B == 255:
-                    B += 15
-                    if B > 255: B = 255
-                if multi_line: faded += "\n"
-            
-        elif colour == "blue-v":
-            G = 10
-            for line in text.splitlines():
-                faded += f"\033[38;2;0;{G};255m{line}\033[0m"
-                if not G == 255:
-                    G += 15
-                    if G > 255: G = 255
-                if multi_line: faded += "\n"
-            
-        elif colour == "purple-v":
-            R = 40
-            for line in text.splitlines():
-                faded += f"\033[38;2;{R};0;220m{line}\033[0m"
-                if not R == 255:
-                    R += 15
-                    if R > 255: R = 255
-                if multi_line: faded += "\n"
-            
-        elif colour == "pink-v":
-            B = 255
-            for line in text.splitlines():
-                faded += f"\033[38;2;255;0;{B}m{line}\033[0m"
-                if not B == 0:
-                    B -= 20
-                    if B < 0: B = 0
-                if multi_line: faded += "\n"
-
-        elif colour == "random":
-            for line in text.splitlines():
-                for char in line:
-                    R, G, B = random.randint(0,255), random.randint(0,255), random.randint(0,255)
-                    faded += f"\033[38;2;{R};{G};{B}m{char}\033[0m"
-                if multi_line: faded += "\n"
-        
-        else: raise ValueError(clr(f"\n  > FADE ERROR! - [{colour}] is not supported yet!",2))
-        
-        if multi_line: faded = faded[:-1]
-        return faded
-    except: sys.exit(clr(err(sys.exc_info()),2))
-
-# --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
-
-def get_duration(then: datetime, now: datetime = None, interval = "default"):
-
-    """
-    Returns a duration as specified by the 'interval' variable
-    
-    __________________________________________________________
-    
-    valid intervals:
-    - years -> int
-    - days -> int
-    - hours -> int
-    - minutes -> int
-    - seconds -> int
-    - dynamic -> str
-    - default -> str
-    """
-    
-    if now is None: now = datetime.now()
-
-    duration = now - then
-
-    if interval in ("year", "years"): return int(duration.days / 365)
-    elif interval in ("day", "days"): return duration.days
-    elif interval in ("hour", "hours"): return int(duration.total_seconds() / 3600)
-    elif interval in ("minute", "minutes"): return int(duration.total_seconds() / 60)
-    elif interval in ("second", "seconds"): return int(duration.total_seconds())
-    elif interval == "dynamic":
-
-        seconds = duration.total_seconds()
-
-        if seconds < 60:
-            return f"{int(seconds)} second{'s' if seconds > 1 else ''}"
-        
-        elif seconds < 3600:
-            minutes = int(seconds / 60)
-            return f"{minutes} minute{'s' if minutes > 1 else ''}"
-        
-        elif seconds < 86400:
-            hours = int(seconds / 3600)
-            return f"{hours} hour{'s' if hours > 1 else ''}"
-       
-        elif seconds < 31536000:
-            days = int(seconds / 86400)
-            return f"{days} day{'s' if days > 1 else ''}"
-        
-        else:
-            years = int(seconds / 31536000)
-            return f"{years} year{'s' if years > 1 else ''}"
-    
-    else:
-        seconds = duration.total_seconds()
-
-        years = int(seconds / 31536000)
-        days = int((seconds % 31536000) / 86400)
-        hours = int((seconds % 86400) / 3600)
-        minutes = int((seconds % 3600) / 60)
-        seconds = int(seconds % 60)
-
-        parts = []
-        if years: parts.append(f"{years} year{'s' if years > 1 else ''}")
-        if days: parts.append(f"{days} day{'s' if days > 1 else ''}")
-        if hours: parts.append(f"{hours} hour{'s' if hours > 1 else ''}")
-        if minutes: parts.append(f"{minutes} minute{'s' if minutes > 1 else ''}")
-        if seconds: parts.append(f"{seconds} second{'s' if seconds > 1 else ''}")
-
-        return ", ".join(parts)
-
-# --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
-
-def err(exc_info) -> str:
-    
-    """
-    Returns a short traceback
-    
-    __________________________________________
-
-    [ EXAMPLE ]
-
-    ```python
-    import sys
-    from dankware import err, clr
-    try: value = 1/0
-    except: print(clr(err(sys.exc_info()),2))
-    ```
-    """
-    
-    from traceback import extract_tb
-
-    ex_type, ex_value, ex_traceback = exc_info
-    trace_back = extract_tb(ex_traceback)
-    stack_trace = []
-
-    for trace in trace_back:
-        filename = trace[0]
-        if filename == "<string>": filename = str(__name__)
-        #elif filename.endswith(".pyc"): filename = filename[:-1]
-        #elif filename.endswith("$py.class"): filename = filename[:-9] + ".py"
-        stack_trace.append("    - File: {} | Line: {} | Function: {}{}".format(filename, trace[1], trace[2] if trace[2] != '<module>' else 'top-level', ' | ' + trace[3] if trace[3] else ''))
-
-    report = "  > Error Type: {}".format(ex_type.__name__)
-    if ex_value: report += "\n  > Error Message: \n    - {}".format(ex_value)
-    report += "\n  > Error Stack Trace: \n{}".format('\n'.join(stack_trace))
-
-    return report
-
-# --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
-
-def splash_screen(img_path: str, duration: int = 3) -> None:
-    
-    """
-    Displays a splash screen for the given duration
-    - Supports: GIFs / PNGs / JPGs / BMPs / ICOs
-    
-    __________________________________________
-    
-    [ EXAMPLE ]
-    
-    ```python
-    from concurrent.futures import ThreadPoolExecutor
-    ThreadPoolExecutor().submit(splash_screen, "splash.gif", duration=3)
-    ```
-    """
-    
-    import tkinter as tk
-    from PIL import Image, ImageTk
-    
-    class SplashScreen(tk.Toplevel):
-
-        def __init__(self, img_path):
-            super().__init__()
-            self.img_path = img_path
-            self.setup_window()
-            self.load_image()
-            self.animate_image()
-
-        def setup_window(self):
-            self.overrideredirect(True)
-            self.wm_attributes("-topmost", True)
-            #self.wm_attributes("-transparentcolor", "white")
-
-            self.image = Image.open(self.img_path)
-            screen_width = self.winfo_screenwidth()
-            screen_height = self.winfo_screenheight()
-
-            width = self.image.width
-            height = self.image.height
-            x = (screen_width - width) // 2
-            y = (screen_height - height) // 2
-
-            self.geometry(f"{width}x{height}+{x}+{y}")
-
-            self.canvas = tk.Canvas(self, bg="white", highlightthickness=0)
-            self.canvas.pack()
-
-        def load_image(self):
-            if self.img_path.lower().endswith('.gif'):
-                self.frames = []
-                for i in range(self.image.n_frames):
-                    self.image.seek(i)
-                    frame = ImageTk.PhotoImage(self.image)
-                    self.frames.append(frame)
-            else:
-                self.frames = [ImageTk.PhotoImage(self.image)]
-
-        def animate_image(self, current_frame=0):
-            self.canvas.delete(tk.ALL)
-            self.canvas.config(width=self.frames[current_frame].width(), height=self.frames[current_frame].height())
-            self.canvas.create_image(self.frames[current_frame].width() // 2, self.frames[current_frame].height() // 2, image=self.frames[current_frame])
-            current_frame = (current_frame + 1) % len(self.frames)
-            if len(self.frames) > 1:
-                self.after(int(1000 / self.image.info['duration']), self.animate_image, current_frame)
-    
-    root = tk.Tk()
-    root.withdraw()
-    SplashScreen(img_path)  
-    root.after(int(duration * 1000), root.quit)
-    root.mainloop()
-
-# --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
-
-def hide_window() -> None:
-
-    """
-    Hides console window
-    """
-    
-    from ctypes import windll
-
-    hWnd = windll.kernel32.GetConsoleWindow()
-    windll.user32.ShowWindow(hWnd, 0)
-
-def show_window() -> None:
-
-    """
-    Shows console window
-    """
-    
-    from ctypes import windll
-
-    hWnd = windll.kernel32.GetConsoleWindow()
-    windll.user32.ShowWindow(hWnd, 1)
-    
-def hide_window_for(duration: int = 3) -> None:
-    
-    """
-    Hides console window for the given duration
-    """
-
-    from concurrent.futures import ThreadPoolExecutor
-    
-    def tmp():
-        hide_window()
-        time.sleep(duration)
-        show_window()
-    
-    ThreadPoolExecutor(10).submit(tmp)
-
-# --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
-
-def file_selector(title: str = "Open", icon_path: str = "") -> str:
-    
-    """
-    Opens file selector and returns selected file path
-    - Allows custom title and icon
-    """
-    
-    from tkinter import Tk
-    from tkinter.filedialog import askopenfilename
-
-    root = Tk()
-    root.withdraw()
-    if icon_path: root.iconbitmap(icon_path)
-    file_path = askopenfilename(title=title)
-    return file_path.replace("/", "\\")
-
-# --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
-
-def cls() -> None: 
-    
-    """
-    Clear screen for multi-os
-    """
-    
-    print(reset)
-    if os.name == 'nt': _ = os.system('cls')
-    else: _ = os.system('clear')
-
-# --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
-
-def title(title: str) -> None:
-    
-    """
-    Changes console window title
-    """
-
-    if os.name == 'nt': os.system(f"title {title}")
-
-# --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
-
-def rm_line() -> None:
-    
-    """
-    Deletes previous line
-    """
-    
-    from shutil import get_terminal_size
-
-    print("\033[A" + " " * (get_terminal_size().columns - 6) + "\033[A")
-
-# --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
-
-def chdir(mode: str) -> str:
-    
-    """
-    - running "os.chdir(os.path.dirname(__file__))" inside example.py will change its directory to the example.py file's location
-    - running "os.chdir(os.path.dirname(sys.argv[0]))" inside example.exe will change its directory to the example.exe file's location (nuitka)
-    - for changing directory to exe's path as exe: exec(chdir("exe"))
-    - for changing directory to script's path as script: exec(chdir("script"))
-    - [NOTE] When I build executables, the [ exec_mode = "script" ] is automatically replaced with [ exec_mode = "exe" ] inside the script
-    - [NOTE] If you run "os.chdir(os.path.dirname(__file__))" as an executable, it will change its directory to its temp folder [ C:\\Users\\user\\AppData\\Local\\Temp\\dankware_PPID ]
-    """
-
-    if mode == "script": return "os.chdir(os.path.dirname(__file__))" # as .py
-    elif mode == "exe": return "os.chdir(os.path.dirname(sys.argv[0]))" # as .exe
-
-# --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
-
-def sys_open(item: str) -> None:
-    
-    """
-    Can do the following:
-    - Open the url on the default browser on windows / linux
-    - Open directory
-    - Start file
-    """
-    
-    if os.name == 'nt': os.system(f'start {item}')
-    else: os.system(f'xdg-open {item}')
-
-# --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
-
-def dankware_banner() -> None:
-    
-    """
-    Dankware banner printer with github url
-    """
-    
-    from shutil import get_terminal_size
-    
-    num_lines = get_terminal_size().lines
-    banner="\n 8 888888888o.     \n 8 8888    `^888.  \n 8 8888        `88.\n 8 8888         `88\n 8 8888          88\n 8 8888          88\n 8 8888         ,88\n 8 8888        ,88'\n 8 8888    ,o88P'  \n 8 888888888P'     \n\n\n          .8.         \n         .888.        \n        :88888.       \n       . `88888.      \n      .8. `88888.     \n     .8`8. `88888.    \n    .8' `8. `88888.   \n   .8'   `8. `88888.  \n  .888888888. `88888. \n .8'       `8. `88888.\n\n\n b.             8\n 888o.          8\n Y88888o.       8\n .`Y888888o.    8\n 8o. `Y888888o. 8\n 8`Y8o. `Y88888o8\n 8   `Y8o. `Y8888\n 8      `Y8o. `Y8\n 8         `Y8o.`\n 8            `Yo\n\n\n 8 8888     ,88'\n 8 8888    ,88' \n 8 8888   ,88'  \n 8 8888  ,88'   \n 8 8888 ,88'    \n 8 8888 88'     \n 8 888888<      \n 8 8888 `Y8.    \n 8 8888   `Y8.  \n 8 8888     `Y8.\n\n\n `8.`888b                 ,8'\n  `8.`888b               ,8' \n   `8.`888b             ,8'  \n    `8.`888b     .b    ,8'   \n     `8.`888b    88b  ,8'    \n      `8.`888b .`888b,8'     \n       `8.`888b8.`8888'      \n        `8.`888`8.`88'       \n         `8.`8' `8,`'        \n          `8.`   `8'         \n\n\n          .8.         \n         .888.        \n        :88888.       \n       . `88888.      \n      .8. `88888.     \n     .8`8. `88888.    \n    .8' `8. `88888.   \n   .8'   `8. `88888.  \n  .888888888. `88888. \n .8'       `8. `88888.\n\n\n 8 888888888o.  \n 8 8888    `88. \n 8 8888     `88 \n 8 8888     ,88 \n 8 8888.   ,88' \n 8 888888888P'  \n 8 8888`8b      \n 8 8888 `8b.    \n 8 8888   `8b.  \n 8 8888     `88.\n\n\n 8 8888888888   \n 8 8888         \n 8 8888         \n 8 8888         \n 8 888888888888 \n 8 8888         \n 8 8888         \n 8 8888         \n 8 8888         \n 8 888888888888 \n "
-    
-    tmp = ""
-    to_print = []
-    sleep_time = []
-    sleep_time_1 = 0.05
-    sleep_time_2 = 0.01
-    sleep_time_3 = 0.333
-    sleep_time_variation = 0.01
-    
-    # sleep_time_1
-        
-    for line in align(clr(banner,4)).splitlines():
-        to_print.append(line)
-        sleep_time.append(sleep_time_1)
-        
-    for _ in range(num_lines):
-        tmp += "     \n"
-        to_print.append("     ")
-        sleep_time.append(sleep_time_1)
-        
-    # sleep_time_2
-    
-    tmp += (align(clr("github.com / SirDank")) + '\n')
-    to_print.append(align(clr("github.com / SirDank")))
-    sleep_time.append(sleep_time_2)
-    
-    for _ in range(int(num_lines/2)):
-        tmp += "     \n"
-        to_print.append("     ")
-        sleep_time.append(sleep_time_2)
-        sleep_time_2 = float(f'{(sleep_time_2 + sleep_time_variation):.3f}')
-        
-    # sleep_time_3
-
-    for _ in range(3):
-        to_print.append(tmp.replace(align(clr("github.com / SirDank")), align(clr("< github.com / SirDank >"))))
-        sleep_time.append(sleep_time_3)
-        to_print.append(tmp.replace(align(clr("github.com / SirDank")), align(clr("<   github.com / SirDank   >"))))
-        sleep_time.append(sleep_time_3)
-        to_print.append(tmp.replace(align(clr("github.com / SirDank")), align(clr("<     github.com / SirDank     >"))))
-        sleep_time.append(sleep_time_3)
-    to_print.append(tmp)
-    sleep_time.append(sleep_time_3)
-    
-    sleep_time[-1] = 4
-    
-    for _ in range(int(num_lines/2)):
-        to_print.append("     ")
-        sleep_time.append(0.01)
-        #sleep_time.append(sleep_time_2)
-        #sleep_time_2 = float(f'{(sleep_time_2 - sleep_time_variation):.3f}')
-        
-    # start
-        
-    cls(); print('\n' * 60)
-    for _, amt in zip(to_print, sleep_time):
-        print(_); time.sleep(amt)
-    
-    # finish
-        
-    cls()
+###################################################################################
+
+#                            https://github.com/SirDank                            
+
+###################################################################################
+
+# > Please read the documentation on github before using this module!
+
+import os
+import sys
+import time
+import random
+from datetime import datetime
+from colorama import Fore, Style
+
+# colorama colours
+
+black = Fore.BLACK + Style.BRIGHT
+blue = Fore.BLUE + Style.BRIGHT
+cyan = Fore.CYAN + Style.BRIGHT
+green = Fore.GREEN + Style.BRIGHT
+magenta = Fore.MAGENTA + Style.BRIGHT
+red = Fore.RED + Style.BRIGHT
+reset = Style.RESET_ALL
+white = Fore.WHITE + Style.BRIGHT
+yellow = Fore.YELLOW + Style.BRIGHT
+
+# dankware variables
+
+chars = ['>','<','.',',','=','-','_','?','!','|','(',')','{','}','/','\\',':','"',"'","%"]
+words_green = ['true', 'True', 'TRUE', 'online', 'Online', 'ONLINE', 'successfully', 'Successfully', 'SUCCESSFULLY', 'successful', 'Successful', 'SUCCESSFUL', 'success', 'Success', 'SUCCESS']
+words_red = ['falsely', 'Falsely', 'FALSELY', 'false', 'False', 'FALSE', 'offline', 'Offline', 'OFFLINE', 'failures', 'Failures', 'FAILURES', 'failure', 'Failure', 'FAILURE', 'failed', 'Failed', 'FAILED', 'fail', 'Fail', 'FAIL']
+colours_to_replace = [Fore.BLACK, Fore.BLUE, Fore.CYAN, Fore.GREEN, Fore.MAGENTA, Fore.RED, Fore.WHITE, Fore.YELLOW, Style.BRIGHT, Style.RESET_ALL]
+colours_alt = ["BBLACKK", "BBLUEE", "CCYANN", "GGREENN", "MMAGENTAA", "RREDD", "WWHITEE", "YYELLOWW", "BBRIGHTT", "RRESETT"]
+bad_colours = ['BLACK', 'WHITE', 'LIGHTBLACK_EX', 'LIGHTWHITE_EX', 'RESET']
+codes = vars(Fore); colours = [codes[colour] for colour in codes if colour not in bad_colours]
+styles = [Style.BRIGHT, Style.DIM, Style.NORMAL]
+available_colours = ['black','red','green','cyan','blue','purple','random','black-v','red-v','green-v','cyan-v','blue-v','purple-v','pink-v']
+
+excluded_prefixes_one = {'6.': '', '7.': '', '10.': '', '11.': '', '21.': '', '22.': '', '26.': '', '28.': '', '29.': '', '30.': '', '33.': '', '55.': '', '127.': '', '136.': '', '205.': '', '214.': '', '215.': ''}
+excluded_prefixes_two = {'23.27.': '', '31.25.': '', '50.117.': '', '74.115.': '', '75.127.': '', '81.87.': '', '100.64.': '', '128.16.': '', '128.40.': '', '128.41.': '', '128.86.': '', '128.232.': '', '128.240.': '', '128.243.': '', '129.11.': '', '129.12.': '', '129.31.': '', '129.67.': '', '129.123.': '', '129.169.': '', '129.215.': '', '129.234.': '', '130.88.': '', '130.159.': '', '130.209.': '', '130.246.': '', '131.111.': '', '131.227.': '', '131.231.': '', '131.251.': '', '134.36.': '', '134.83.': '', '134.151.': '', '134.219.': '', '134.220.': '', '134.225.': '', '136.148.': '', '136.156.': '', '137.44.': '', '137.50.': '', '137.73.': '', '137.108.': '', '137.195.': '', '137.222.': '', '137.253.': '', '138.38.': '', '138.40.': '', '138.250.': '', '138.253.': '', '139.133.': '', '139.153.': '', '139.166.': '', '139.184.': '', '139.222.': '', '140.97.': '', '141.163.': '', '141.241.': '', '142.111.': '', '142.252.': '', '143.52.': '', '143.117.': '', '143.167.': '', '143.210.': '', '143.234.': '', '144.32.': '', '144.39.': '', '144.82.': '', '144.124.': '', '144.173.': '', '146.87.': '', '146.97.': '', '146.169.': '', '146.176.': '', '146.179.': '', '146.191.': '', '146.227.': '', '147.143.': '', '147.188.': '', '147.197.': '', '148.79.': '', '148.88.': '', '148.197.': '', '149.155.': '', '149.170.': '', '150.204.': '', '152.71.': '', '152.78.': '', '152.105.': '', '153.11.': '', '155.198.': '', '155.245.': '', '157.140.': '', '157.228.': '', '158.94.': '', '158.125.': '', '158.143.': '', '158.223.': '', '159.92.': '', '160.5.': '', '160.9.': '', '161.73.': '', '161.74.': '', '161.76.': '', '161.112.': '', '163.1.': '', '163.119.': '', '163.160.': '', '163.167.': '', '164.11.': '', '165.160.': '', '166.88.': '', '169.254.': '', '172.252.': '', '192.168.': '', '192.177.': '', '192.186.': '', '193.60.': '', '194.66.': '', '194.80.': '', '195.194.': '', '198.18.': '', '205.164.': '', '212.121.': '', '212.219.': ''}
+excluded_prefixes_three = {'4.53.201.': '', '5.152.179.': '', '8.12.162.': '', '8.12.163.': '', '8.12.164.': '', '8.14.84.': '', '8.14.145.': '', '8.14.146.': '', '8.14.147.': '', '8.17.250.': '', '8.17.251.': '', '8.17.252.': '', '23.231.128.': '', '31.25.2.': '', '31.25.4.': '', '37.72.112.': '', '37.72.172.': '', '38.72.200.': '', '46.254.200.': '', '50.93.192.': '', '50.93.193.': '', '50.93.194.': '', '50.93.195.': '', '50.93.196.': '', '50.93.197.': '', '50.115.128.': '', '50.118.128.': '', '63.141.222.': '', '64.62.253.': '', '64.92.96.': '', '64.145.79.': '', '64.145.82.': '', '64.158.146.': '', '65.49.24.': '', '65.49.93.': '', '65.162.192.': '', '66.79.160.': '', '66.160.191.': '', '68.68.96.': '', '69.46.64.': '', '69.176.80.': '', '72.13.80.': '', '72.52.76.': '', '74.82.43.': '', '74.82.160.': '', '74.114.88.': '', '74.115.2.': '', '74.115.4.': '', '74.122.100.': '', '85.12.64.': '', '89.207.208.': '', '92.245.224.': '', '103.251.91.': '', '108.171.32.': '', '108.171.42.': '', '108.171.52.': '', '108.171.62.': '', '118.193.78.': '', '130.93.16.': '', '132.206.9.': '', '132.206.123.': '', '132.206.125.': '', '141.170.64.': '', '141.170.96.': '', '141.170.100.': '', '146.82.55.93': '', '149.54.136.': '', '149.54.152.': '', '159.86.128.': '', '173.245.64.': '', '173.245.194.': '', '173.245.220.': '', '173.252.192.': '', '178.18.16.': '', '178.18.26.': '', '178.18.27.': '', '178.18.28.': '', '178.18.29.': '', '183.182.22.': '', '185.83.168.': '', '192.12.72.': '', '192.18.195.': '', '192.35.172.': '', '192.41.104.': '', '192.41.112.': '', '192.41.128.': '', '192.68.153.': '', '192.76.6.': '', '192.76.8.': '', '192.76.16.': '', '192.76.32.': '', '192.82.153.': '', '192.84.5.': '', '192.84.75.': '', '192.84.76.': '', '192.84.80.': '', '192.84.212.': '', '192.88.9.': '', '192.88.10.': '', '192.88.99.': '', '192.92.114.': '', '192.94.235.': '', '192.100.78.': '', '192.100.154.': '', '192.107.168.': '', '192.108.120.': '', '192.124.46.': '', '192.133.244.': '', '192.149.111.': '', '192.150.180.': '', '192.150.184.': '', '192.153.213.': '', '192.155.160.': '', '192.156.162.': '', '192.160.194.': '', '192.171.128.': '', '192.171.192.': '', '192.173.1.': '', '192.173.2.': '', '192.173.4.': '', '192.173.128.': '', '192.188.157.': '', '192.188.158.': '', '192.190.201.': '', '192.190.202.': '', '192.195.42.': '', '192.195.105.': '', '192.195.116.': '', '192.195.118.': '', '192.249.64.': '', '192.250.240.': '', '193.32.22.': '', '193.37.225.': '', '193.37.240.': '', '193.38.143.': '', '193.39.80.': '', '193.39.172.': '', '193.39.212.': '', '193.107.116.': '', '193.130.15.': '', '193.133.28.': '', '193.138.86.': '', '194.32.32.': '', '194.35.93.': '', '194.35.186.': '', '194.35.192.': '', '194.35.241.': '', '194.36.1.': '', '194.36.2.': '', '194.36.121.': '', '194.36.152.': '', '194.60.218.': '', '194.110.214.': '', '194.187.32.': '', '198.12.120.': '', '198.12.121.': '', '198.12.122.': '', '198.51.100.': '', '198.144.240.': '', '199.33.120.': '', '199.33.124.': '', '199.48.147.': '', '199.68.196.': '', '199.127.240.': '', '199.187.168.': '', '199.188.238.': '', '199.255.208.': '', '203.12.6.': '', '204.13.64.': '', '204.16.192.': '', '204.19.238.': '', '204.74.208.': '', '204.113.91.': '', '205.159.189.': '', '205.209.128.': '', '206.108.52.': '', '206.165.4.': '', '208.77.40.': '', '208.80.4.': '', '208.123.223.': '', '209.51.185.': '', '209.54.48.': '', '209.107.192.': '', '209.107.210.': '', '209.107.212.': '', '211.156.110.': '', '212.121.192.': '', '216.151.183.': '', '216.151.190.': '', '216.172.128.': '', '216.185.36.': '', '216.218.233.': '', '216.224.112.': ''}
+
+def multithread(function: callable, threads: int = 1, *args, progress_bar: bool = True) -> None:
+    
+    """
+    > Please read the documentation on github before using this function!
+    
+    ________________________________________________________________________________
+
+    Run the given function in multiple threads with the specified inputs.
+
+    - function: The function to run in multiple threads.
+    - threads: The number of threads to use.
+    - *args: Input(s) for the function. Can be a list, a single value.
+    - progress_bar: Whether to display a progress bar.
+    """
+    
+    from rich.live import Live
+    from rich.panel import Panel
+    from rich.table import Table
+    from shutil import get_terminal_size
+    from concurrent.futures import ThreadPoolExecutor, as_completed
+    from rich.progress import Progress, SpinnerColumn, BarColumn, TextColumn, TimeRemainingColumn, TimeElapsedColumn
+
+    try:
+        
+        def submit_task(executor, *args):
+            return executor.submit(function, *args)
+        
+        if threads < 1:
+            raise ValueError("The number of threads must be a positive integer.")
+
+        futures = []
+        executor = ThreadPoolExecutor(max_workers=threads)
+
+        if not args:
+            for _ in range(threads): futures.append(executor.submit(function))
+        else:
+            input_lists = []
+            for arg in args:
+                if isinstance(arg, list):
+                    input_lists.append(arg)
+                else:
+                    input_lists.append([arg] * threads)
+
+            for task_args in zip(*input_lists):
+                futures.append(submit_task(executor, *task_args))
+
+        if progress_bar:
+            width = get_terminal_size().columns
+            job_progress = Progress("{task.description}", SpinnerColumn(), BarColumn(bar_width=width), TextColumn("[deep_pink1][progress.percentage][bright_cyan]{task.percentage:>3.0f}%"), "[bright_cyan]ETA", TimeRemainingColumn(), TimeElapsedColumn())
+            overall_task = job_progress.add_task("[bright_green]Progress", total=int(len(futures)))
+            progress_table = Table.grid()
+            progress_table.add_row(Panel.fit(job_progress, title="[bright_red]Jobs", border_style="magenta1", padding=(1, 2)))
+
+            with Live(progress_table, refresh_per_second=10):
+                while not job_progress.finished:
+                    time.sleep(0.1)
+                    for future in as_completed(futures):
+                        if future.done():
+                            try: future.result()
+                            except: pass
+                            job_progress.advance(overall_task)
+
+        else:
+            for future in as_completed(futures):
+                if future.done():
+                    try: future.result()
+                    except: pass
+                
+    except: 
+        try: executor.shutdown()
+        except: pass
+        sys.exit(clr(err(sys.exc_info()),2))
+
+# --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
+
+def github_downloads(user_repo: str) -> list:
+
+    """
+    Extracts direct download urls from the latest release on github and returns it as a list
+
+    - Example Input: USER_NAME/REPO_NAME ( from https://api.github.com/repos/USER_NAME/REPO_NAME/releases/latest )
+    - Example Output: ['https://github.com/USER_NAME/REPO_NAME/releases/download/VERSION/EXAMPLE.TXT']
+    
+    _____________________________________________________________________________________________________________________________________
+    
+    [ EXAMPLE ]
+    ```python
+    from dankware import github_downloads
+    for _ in github_downloads("SirDank/dank.tool"): print(_)
+    ```
+    """
+    
+    import requests
+    
+    urls = []
+
+    #if "https://api.github.com/repos/" not in url or "/releases/latest" not in url:
+    #    raise ValueError(clr('  > Invalid url! Must follow: "https://api.github.com/repos/NAME/NAME/releases/latest"',2)) 
+    while True:
+        try: response = requests.get(f"https://api.github.com/repos/{user_repo}/releases/latest").json(); break
+        except: input(clr("  > Make sure you are connected to the Internet! Press [ENTER] to try again... ",2))
+    
+    for data in response["assets"]:
+        urls.append(data["browser_download_url"])
+
+    return urls
+
+# --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
+
+def github_file_selector(user_repo: str, filter_mode: str, name_list: list) -> list:
+    
+    """
+    
+    This function is used to filter the output from github_downloads()
+    
+    - user_repo = 'USER_NAME/REPO_NAME' ( from https://api.github.com/repos/USER_NAME/REPO_NAME/releases/latest )
+    - filter_mode = 'add' or 'remove'
+    - name_list = list of names to be added or removed
+    
+    _______________________________________________________________________________________________________________________________________________________________________
+    
+    [ EXAMPLE ]
+    ```python
+    from dankware import github_file_selector
+    for file_url in github_file_selector("EssentialsX/Essentials", "remove", ['AntiBuild', 'Discord', 'GeoIP', 'Protect', 'XMPP']):
+        print(file_url)
+    ```
+    
+    _______________________________________________________________________________________________________________________________________________________________________
+    
+    Example output from github_downloads("EX_USER/EX_REPO"): [
+        'https://github.com/EX_USER/EX_REPO/releases/download/VERSION/EXAMPLE.TXT'
+        'https://github.com/EX_USER/EX_REPO/releases/download/VERSION/EXAMPLE_2.TXT'
+        'https://github.com/EX_USER/EX_REPO/releases/download/VERSION/EXAMPLE_3.TXT'
+        'https://github.com/EX_USER/EX_REPO/releases/download/VERSION/TEST.TXT'
+        'https://github.com/EX_USER/EX_REPO/releases/download/VERSION/TEST_2.TXT'
+        'https://github.com/EX_USER/EX_REPO/releases/download/VERSION/TEST_3.TXT'
+    ]
+    
+    _______________________________________________________________________________________________________________________________________________________________________
+    
+    Example Input: "EX_USER/EX_REPO", "add", ["EXAMPLE"]
+        
+    Example Output: [
+        'https://github.com/EX_USER/EX_REPO/releases/download/VERSION/EXAMPLE.TXT'
+        'https://github.com/EX_USER/EX_REPO/releases/download/VERSION/EXAMPLE_2.TXT'
+        'https://github.com/EX_USER/EX_REPO/releases/download/VERSION/EXAMPLE_3.TXT'
+    ]
+        
+    - Note: Only urls with filenames containing "EXAMPLE" were returned.
+
+    _______________________________________________________________________________________________________________________________________________________________________
+
+    Example Input: "EX_USER/EX_REPO", "remove", ["EXAMPLE"]
+    
+    Example Output: [
+        'https://github.com/EX_USER/EX_REPO/releases/download/VERSION/TEST.TXT'
+        'https://github.com/EX_USER/EX_REPO/releases/download/VERSION/TEST_2.TXT'
+        'https://github.com/EX_USER/EX_REPO/releases/download/VERSION/TEST_3.TXT'
+    ]
+    
+    - Note: Only urls with filenames not containing "EXAMPLE" were returned.
+    
+    """
+
+    urls = []
+    for file_url in github_downloads(user_repo):
+        if filter_mode == "add": valid = False
+        elif filter_mode == "remove": valid = True
+        for name in name_list:
+            if name in file_url.split('/')[-1]:
+                if filter_mode == "add": valid = True
+                elif filter_mode == "remove": valid = False
+        if valid: urls.append(file_url)
+    return urls
+
+# --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
+
+def random_ip() -> str:
+    
+    """
+    Generates a random valid computer ip
+    - Follows: https://github.com/robertdavidgraham/masscan/blob/master/data/exclude.conf
+    """
+    
+    while True:
+        
+        first_octet = random.randint(1, 223)
+        second_octet = random.randint(0, 255)
+        third_octet = random.randint(0, 255)
+        fourth_octet = random.randint(0, 255)
+
+        if f"{first_octet}." in excluded_prefixes_one.keys(): continue
+        elif f"{first_octet}.{second_octet}." in excluded_prefixes_two.keys(): continue
+        elif f"{first_octet}.{second_octet}.{third_octet}" in excluded_prefixes_three.keys(): continue
+        
+        if first_octet == 172 and second_octet >= 16 and second_octet <= 31: continue
+        elif first_octet == 192:
+            if fourth_octet == 170 or fourth_octet == 171 or third_octet == 2: continue
+        elif first_octet == 203 and third_octet == 113: continue
+        elif first_octet == 216 and second_octet == 83 and third_octet >= 33 and third_octet <= 63: continue
+        elif second_octet == 255 and third_octet == 255 and third_octet == 255: continue
+
+        break
+    
+    ip = f"{first_octet}.{second_octet}.{third_octet}.{fourth_octet}"
+        
+    return ip
+
+# --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
+
+def is_admin() -> bool:
+    
+    import ctypes
+    
+    """
+    Checks if the current user has admin privileges and returns True if found else False
+    """
+    
+    try: return ctypes.windll.shell32.IsUserAnAdmin()
+    except: return False
+    
+'''
+def run_as_admin() -> None:
+    
+    """
+    Executes the script with admin privileges
+    """
+    
+    ctypes.windll.shell32.ShellExecuteW(None, "runas", sys.executable, __file__, None, 1)
+    #sys.exit(clr("\n  > Exiting original un-elevated script...",2))
+'''
+
+# --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
+
+def export_registry_keys(registry_root: str, registry_path: str, recursive: bool = True, export_path: str = "export.reg") -> None:
+
+    """
+    Function to export registry keys with or without its subkeys and saves them to export_path
+    - Examples for registry_root: 'HKEY_CLASSES_ROOT', 'HKEY_CURRENT_USER', 'HKEY_LOCAL_MACHINE', 'HKEY_USERS', 'HKEY_CURRENT_CONFIG'
+    - Example for registry_path: r'Software\Google\Chrome\PreferenceMACs'
+    - recursive: True (subkeys saved)
+    - recursive: False (subkeys not saved)
+    - export_path: "exported.reg" (default)
+    
+    _______________________________________________________________________________________________________________________________________________________________________
+    
+    [ EXAMPLE ]
+    
+    ```python
+    from dankware import export_registry_keys
+    export_registry_keys('HKEY_CURRENT_USER', r'Software\Google\Chrome\PreferenceMACs')
+    ```
+    """
+
+    import winreg
+    
+    try:
+    
+        key_data = []
+        key_map = {
+            'HKEY_CLASSES_ROOT': winreg.HKEY_CLASSES_ROOT,
+            'HKEY_CURRENT_USER': winreg.HKEY_CURRENT_USER,
+            'HKEY_LOCAL_MACHINE': winreg.HKEY_LOCAL_MACHINE,
+            'HKEY_USERS': winreg.HKEY_USERS,
+            'HKEY_CURRENT_CONFIG': winreg.HKEY_CURRENT_CONFIG,
+        }
+        
+        if not export_path.endswith('.reg'):
+            raise ValueError("Invalid Export Path! export_path must end with '.reg'")
+        if registry_root not in key_map.keys():
+            raise ValueError(f"Invalid Registry Root! Use one of the following: {', '.join(key_map.keys())}")
+        if not is_admin():
+            raise RuntimeError("Current user is not an administrator! Exporting registry keys requires admin privileges!")
+            # If the current user is not an admin, relaunch the script with admin privileges
+            #run_as_admin()
+            
+        def exporter(key, registry_root, subkey_path, key_data, recursive) -> None:
+
+            subkey = winreg.OpenKey(key, subkey_path, 0, winreg.KEY_READ | winreg.KEY_WOW64_64KEY)
+            subkey_count = winreg.QueryInfoKey(subkey)[0]
+            key_data.append(f'[{registry_root}\\{subkey_path}]')
+    
+            for i in range(winreg.QueryInfoKey(subkey)[1]):
+                value_name, value_data, value_type = winreg.EnumValue(subkey, i)
+                key_data.append(f'"{value_name}"="{value_data}"')
+
+            key_data.append('')
+            for i in range(subkey_count):
+                subkey_name = winreg.EnumKey(subkey, i)
+                subkey_full_path = subkey_path + '\\' + subkey_name if subkey_path else subkey_name
+                if recursive: exporter(key, registry_root, subkey_full_path, key_data, recursive)
+
+            winreg.CloseKey(subkey)
+
+        key = key_map[registry_root]
+        exporter(key, registry_root, registry_path, key_data, recursive)
+        open(export_path, 'w', encoding='utf-16').write('Windows Registry Editor Version 5.00\n\n' + '\n'.join(key_data))
+        print(clr(f"\n  > Successfully exported registry keys to \"{os.path.join(os.getcwd(), 'export.reg') if export_path == 'export.reg' else export_path}\""))
+    
+    except: sys.exit(clr(err(sys.exc_info()),2))
+
+# --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
+
+def clr(text: str, mode: int = 1, colour_one: str = white, colour_two: str = magenta) -> str:
+    
+    """
+    
+    this function colours special characters inside the 'chars' list
+    
+    ___________________________________________
+    
+    - mode: 1 | to display general text (default)
+    - text = white (default) / specified colour
+    - spl = magenta (default) / specified colour
+
+    ___________________________________________
+
+    - mode: 2 | to display error messages
+    - text = red (fixed colour)
+    - spl = white (fixed colour)
+
+    ___________________________________________
+
+    - mode: 3
+    - text = random (fixed colour)
+    - spl = white (fixed colour)
+
+    ___________________________________________
+
+    - mode: 4 | to display banners
+    - text & spl = random (fixed colour)
+    
+    """
+    
+    try:
+        if mode != 3:
+            for _ in range(len(colours_to_replace)):
+                text = text.replace(colours_to_replace[_], colours_alt[_])
+        else:
+            for _ in range(len(colours_to_replace)):
+                text = text.replace(colours_to_replace[_], '')
+
+        # default
+
+        if mode == 1:
+            text = text.replace("[",f"{colour_two}[{colour_one}").replace("]",f"{colour_two}]{colour_one}")
+            for char in chars: text = text.replace(char, f"{colour_two}{char}{colour_one}")
+            for word in words_green:
+                replacement = green.join(list(word))
+                text = text.replace(word, f"{green}{replacement}{colour_one}")
+            for word in words_red:
+                replacement = red.join(list(word))
+                text = text.replace(word, f"{red}{replacement}{colour_one}")
+        
+        # for error messages
+        
+        elif mode == 2:
+            text = text.replace("[",f"{white}[{red}").replace("]",f"{white}]{red}")
+            for char in chars: text = text.replace(char, f"{white}{char}{red}")
+            #for word in words_green: text = text.replace(word, f"{green}{word}{red}")
+        
+        # random | TRUE, FALSE will not be coloured!
+        
+        elif mode == 3 or mode == 4:
+            text = [char for char in text]
+            if mode == 3: colour_spl = True
+            else: colour_spl = False
+            for _ in range(len(text)):
+                char = text[_]
+                if char != ' ' and char != '\n':
+                    if colour_spl:
+                        if char in ( ['[',']'] + chars ): text[_] = white + char
+                        else: text[_] = random.choice(colours) + Style.BRIGHT + char
+                    else:
+                        text[_] = random.choice(colours) + Style.BRIGHT + char
+            text = ''.join(text)
+
+        else: raise ValueError(f"\n  {white}> {red}Invalid Mode {white}[{red}{mode}{white}] | Valid Modes{white}: {red}1{white},{red}2{white},{red}3{white},{red}4" + reset)
+
+        if mode != 3:
+            for _ in range(len(colours_to_replace)):
+                text = str(text).replace(colours_alt[_], colours_to_replace[_])
+
+        if mode == 1: return white + text + reset
+        elif mode == 2: return red + text + reset
+        elif mode == 3 or mode == 4: return text + reset
+    
+    except: sys.exit(clr(err(sys.exc_info()),2))
+
+# --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
+
+def align(text: str) -> str: 
+    
+    """
+    center align banner / line ( supports both coloured and non-coloured )
+    - [NOTE] align supports: clr, does not support: fade
+    """
+    
+    from shutil import get_terminal_size
+
+    width = get_terminal_size().columns; aligned = text
+    for colour in vars(Fore).values(): aligned = aligned.replace(colour,'')
+    for style in vars(Style).values(): aligned = aligned.replace(style,'')
+    text = text.split('\n'); aligned = aligned.split('\n')
+    for _ in range(len(aligned)): aligned[_] = aligned[_].center(width).replace(aligned[_],text[_])
+    return str('\n'.join(aligned) + reset)
+
+# --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
+
+def fade(text: str, colour: str = "purple") -> str:
+    
+    """
+    credits to https://github.com/venaxyt/gratient & https://github.com/venaxyt/fade <3
+    - available_colours = black, red, green, cyan, blue, purple, random, black-v, red-v, green-v, cyan-v, blue-v, purple-v, pink-v
+    """
+
+    try:
+        colour = colour.lower()
+        if not colour in available_colours: raise ValueError(clr(f"\n  > Invalid Colour: {colour} | Available Colours: {', '.join(available_colours)}",2))
+            
+        faded = ""
+        if len(text.splitlines()) > 1: multi_line = True
+        else: multi_line = False
+
+        if colour == "black":
+            for line in text.splitlines():
+                R = 0; G = 0; B = 0
+                for char in line:
+                    R += 3; G += 3; B += 3
+                    if R > 255 and G > 255 and B > 255: R = 255; G = 255; B = 255
+                    faded += f"\033[38;2;{R};{G};{B}m{char}\033[0m"
+                if multi_line: faded += "\n"
+                
+        elif colour == "red":
+            for line in text.splitlines():
+                G = 250
+                for char in line:
+                    G -= 5
+                    if G < 0: G = 0
+                    faded += f"\033[38;2;255;{G};0m{char}\033[0m"
+                if multi_line: faded += "\n"
+                
+        elif colour == "green":
+            for line in text.splitlines():
+                R = 0
+                for char in line:
+                    if not R > 200: R += 3
+                    faded += f"\033[38;2;{R};255;0m{char}\033[0m"
+                if multi_line: faded += "\n"
+                
+        elif colour == "cyan":
+            for line in text.splitlines():
+                B = 100
+                for char in line:
+                    B += 2
+                    if B > 255: B = 255
+                    faded += f"\033[38;2;0;255;{B}m{char}\033[0m"
+                if multi_line: faded += "\n"
+
+        elif colour == "blue":
+            for line in text.splitlines():
+                G = 0
+                for char in line:
+                    G += 3
+                    if G > 255: G = 255
+                    faded += f"\033[38;2;0;{G};255m{char}\033[0m"
+                if multi_line: faded += "\n"
+            
+        elif colour == "purple":
+            for line in text.splitlines():
+                R = 35
+                for char in line:
+                    R += 3
+                    if R > 255: R = 255
+                    faded += f"\033[38;2;{R};0;220m{char}\033[0m"
+                if multi_line: faded += "\n"
+
+        elif colour == "black-v":
+            R = 0; G = 0; B = 0
+            for line in text.splitlines():
+                faded += (f"\033[38;2;{R};{G};{B}m{line}\033[0m")
+                if not R == 255 and not G == 255 and not B == 255:
+                    R += 20; G += 20; B += 20
+                    if R > 255 and G > 255 and B > 255: R = 255; G = 255; B = 255
+                if multi_line: faded += "\n"
+                        
+        elif colour == "red-v":
+            G = 250
+            for line in text.splitlines():
+                faded += f"\033[38;2;255;{G};0m{line}\033[0m"
+                if not G == 0:
+                    G -= 25
+                    if G < 0: G = 0
+                if multi_line:faded += "\n"
+
+        elif colour == "green-v":
+            R = 0
+            for line in text.splitlines():
+                faded += f"\033[38;2;{R};255;0m{line}\033[0m"
+                if not R > 200: R += 30
+                if multi_line: faded += "\n"
+            
+        elif colour == "cyan-v":
+            B = 100
+            for line in text.splitlines():
+                faded += f"\033[38;2;0;255;{B}m{line}\033[0m"
+                if not B == 255:
+                    B += 15
+                    if B > 255: B = 255
+                if multi_line: faded += "\n"
+            
+        elif colour == "blue-v":
+            G = 10
+            for line in text.splitlines():
+                faded += f"\033[38;2;0;{G};255m{line}\033[0m"
+                if not G == 255:
+                    G += 15
+                    if G > 255: G = 255
+                if multi_line: faded += "\n"
+            
+        elif colour == "purple-v":
+            R = 40
+            for line in text.splitlines():
+                faded += f"\033[38;2;{R};0;220m{line}\033[0m"
+                if not R == 255:
+                    R += 15
+                    if R > 255: R = 255
+                if multi_line: faded += "\n"
+            
+        elif colour == "pink-v":
+            B = 255
+            for line in text.splitlines():
+                faded += f"\033[38;2;255;0;{B}m{line}\033[0m"
+                if not B == 0:
+                    B -= 20
+                    if B < 0: B = 0
+                if multi_line: faded += "\n"
+
+        elif colour == "random":
+            for line in text.splitlines():
+                for char in line:
+                    R, G, B = random.randint(0,255), random.randint(0,255), random.randint(0,255)
+                    faded += f"\033[38;2;{R};{G};{B}m{char}\033[0m"
+                if multi_line: faded += "\n"
+        
+        else: raise ValueError(clr(f"\n  > FADE ERROR! - [{colour}] is not supported yet!",2))
+        
+        if multi_line: faded = faded[:-1]
+        return faded
+    except: sys.exit(clr(err(sys.exc_info()),2))
+
+# --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
+
+def get_duration(then: datetime, now: datetime = None, interval = "default"):
+
+    """
+    Returns a duration as specified by the 'interval' variable
+    
+    __________________________________________________________
+    
+    valid intervals:
+    - years -> int
+    - days -> int
+    - hours -> int
+    - minutes -> int
+    - seconds -> int
+    - dynamic -> str
+    - default -> str
+    """
+    
+    if now is None: now = datetime.now()
+
+    duration = now - then
+
+    if interval in ("year", "years"): return int(duration.days / 365)
+    elif interval in ("day", "days"): return duration.days
+    elif interval in ("hour", "hours"): return int(duration.total_seconds() / 3600)
+    elif interval in ("minute", "minutes"): return int(duration.total_seconds() / 60)
+    elif interval in ("second", "seconds"): return int(duration.total_seconds())
+    elif interval == "dynamic":
+
+        seconds = duration.total_seconds()
+
+        if seconds < 60:
+            return f"{int(seconds)} second{'s' if seconds > 1 else ''}"
+        
+        elif seconds < 3600:
+            minutes = int(seconds / 60)
+            return f"{minutes} minute{'s' if minutes > 1 else ''}"
+        
+        elif seconds < 86400:
+            hours = int(seconds / 3600)
+            return f"{hours} hour{'s' if hours > 1 else ''}"
+       
+        elif seconds < 31536000:
+            days = int(seconds / 86400)
+            return f"{days} day{'s' if days > 1 else ''}"
+        
+        else:
+            years = int(seconds / 31536000)
+            return f"{years} year{'s' if years > 1 else ''}"
+    
+    else:
+        seconds = duration.total_seconds()
+
+        years = int(seconds / 31536000)
+        days = int((seconds % 31536000) / 86400)
+        hours = int((seconds % 86400) / 3600)
+        minutes = int((seconds % 3600) / 60)
+        seconds = int(seconds % 60)
+
+        parts = []
+        if years: parts.append(f"{years} year{'s' if years > 1 else ''}")
+        if days: parts.append(f"{days} day{'s' if days > 1 else ''}")
+        if hours: parts.append(f"{hours} hour{'s' if hours > 1 else ''}")
+        if minutes: parts.append(f"{minutes} minute{'s' if minutes > 1 else ''}")
+        if seconds: parts.append(f"{seconds} second{'s' if seconds > 1 else ''}")
+
+        return ", ".join(parts)
+
+# --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
+
+def err(exc_info) -> str:
+    
+    """
+    Returns a short traceback
+    
+    __________________________________________
+
+    [ EXAMPLE ]
+
+    ```python
+    import sys
+    from dankware import err, clr
+    try: value = 1/0
+    except: print(clr(err(sys.exc_info()),2))
+    ```
+    """
+    
+    from traceback import extract_tb
+
+    ex_type, ex_value, ex_traceback = exc_info
+    trace_back = extract_tb(ex_traceback)
+    stack_trace = []
+
+    for trace in trace_back:
+        filename = trace[0]
+        if filename == "<string>": filename = str(__name__)
+        #elif filename.endswith(".pyc"): filename = filename[:-1]
+        #elif filename.endswith("$py.class"): filename = filename[:-9] + ".py"
+        stack_trace.append("    - File: {} | Line: {} | Function: {}{}".format(filename, trace[1], trace[2] if trace[2] != '<module>' else 'top-level', ' | ' + trace[3] if trace[3] else ''))
+
+    report = "  > Error Type: {}".format(ex_type.__name__)
+    if ex_value: report += "\n  > Error Message: \n    - {}".format(ex_value)
+    report += "\n  > Error Stack Trace: \n{}".format('\n'.join(stack_trace))
+
+    return report
+
+# --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
+
+def splash_screen(img_path: str, duration: int = 3) -> None:
+    
+    """
+    Displays a splash screen for the given duration
+    - Supports: GIFs / PNGs / JPGs / BMPs / ICOs
+    
+    __________________________________________
+    
+    [ EXAMPLE ]
+    
+    ```python
+    from concurrent.futures import ThreadPoolExecutor
+    ThreadPoolExecutor().submit(splash_screen, "splash.gif", duration=3)
+    ```
+    """
+    
+    import tkinter as tk
+    from PIL import Image, ImageTk
+    
+    class SplashScreen(tk.Toplevel):
+
+        def __init__(self, img_path):
+            super().__init__()
+            self.img_path = img_path
+            self.setup_window()
+            self.load_image()
+            self.animate_image()
+
+        def setup_window(self):
+            self.overrideredirect(True)
+            self.wm_attributes("-topmost", True)
+            #self.wm_attributes("-transparentcolor", "white")
+
+            self.image = Image.open(self.img_path)
+            screen_width = self.winfo_screenwidth()
+            screen_height = self.winfo_screenheight()
+
+            width = self.image.width
+            height = self.image.height
+            x = (screen_width - width) // 2
+            y = (screen_height - height) // 2
+
+            self.geometry(f"{width}x{height}+{x}+{y}")
+
+            self.canvas = tk.Canvas(self, bg="white", highlightthickness=0)
+            self.canvas.pack()
+
+        def load_image(self):
+            if self.img_path.lower().endswith('.gif'):
+                self.frames = []
+                for i in range(self.image.n_frames):
+                    self.image.seek(i)
+                    frame = ImageTk.PhotoImage(self.image)
+                    self.frames.append(frame)
+            else:
+                self.frames = [ImageTk.PhotoImage(self.image)]
+
+        def animate_image(self, current_frame=0):
+            self.canvas.delete(tk.ALL)
+            self.canvas.config(width=self.frames[current_frame].width(), height=self.frames[current_frame].height())
+            self.canvas.create_image(self.frames[current_frame].width() // 2, self.frames[current_frame].height() // 2, image=self.frames[current_frame])
+            current_frame = (current_frame + 1) % len(self.frames)
+            if len(self.frames) > 1:
+                self.after(int(1000 / self.image.info['duration']), self.animate_image, current_frame)
+    
+    root = tk.Tk()
+    root.withdraw()
+    SplashScreen(img_path)  
+    root.after(int(duration * 1000), root.quit)
+    root.mainloop()
+
+# --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
+
+def hide_window() -> None:
+
+    """
+    Hides console window
+    """
+    
+    from ctypes import windll
+
+    hWnd = windll.kernel32.GetConsoleWindow()
+    windll.user32.ShowWindow(hWnd, 0)
+
+def show_window() -> None:
+
+    """
+    Shows console window
+    """
+    
+    from ctypes import windll
+
+    hWnd = windll.kernel32.GetConsoleWindow()
+    windll.user32.ShowWindow(hWnd, 1)
+    
+def hide_window_for(duration: int = 3) -> None:
+    
+    """
+    Hides console window for the given duration
+    """
+
+    from concurrent.futures import ThreadPoolExecutor
+    
+    def tmp():
+        hide_window()
+        time.sleep(duration)
+        show_window()
+    
+    ThreadPoolExecutor(10).submit(tmp)
+
+# --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
+
+def file_selector(title: str = "Open", icon_path: str = "") -> str:
+    
+    """
+    Opens file selector and returns selected file path
+    - Allows custom title and icon
+    """
+    
+    from tkinter import Tk
+    from tkinter.filedialog import askopenfilename
+
+    root = Tk()
+    root.withdraw()
+    if icon_path: root.iconbitmap(icon_path)
+    file_path = askopenfilename(title=title)
+    return file_path.replace("/", "\\")
+
+# --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
+
+def cls() -> None: 
+    
+    """
+    Clear screen for multi-os
+    """
+    
+    print(reset)
+    if os.name == 'nt': _ = os.system('cls')
+    else: _ = os.system('clear')
+
+# --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
+
+def title(title: str) -> None:
+    
+    """
+    Changes console window title
+    """
+
+    if os.name == 'nt': os.system(f"title {title}")
+
+# --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
+
+def rm_line() -> None:
+    
+    """
+    Deletes previous line
+    """
+    
+    from shutil import get_terminal_size
+
+    print("\033[A" + " " * (get_terminal_size().columns - 6) + "\033[A")
+
+# --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
+
+def chdir(mode: str) -> str:
+    
+    """
+    - running "os.chdir(os.path.dirname(__file__))" inside example.py will change its directory to the example.py file's location
+    - running "os.chdir(os.path.dirname(sys.argv[0]))" inside example.exe will change its directory to the example.exe file's location (nuitka)
+    - for changing directory to exe's path as exe: exec(chdir("exe"))
+    - for changing directory to script's path as script: exec(chdir("script"))
+    - [NOTE] When I build executables, the [ exec_mode = "script" ] is automatically replaced with [ exec_mode = "exe" ] inside the script
+    - [NOTE] If you run "os.chdir(os.path.dirname(__file__))" as an executable, it will change its directory to its temp folder [ C:\\Users\\user\\AppData\\Local\\Temp\\dankware_PPID ]
+    """
+
+    if mode == "script": return "os.chdir(os.path.dirname(__file__))" # as .py
+    elif mode == "exe": return "os.chdir(os.path.dirname(sys.argv[0]))" # as .exe
+
+# --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
+
+def sys_open(item: str) -> None:
+    
+    """
+    Can do the following:
+    - Open the url on the default browser on windows / linux
+    - Open directory
+    - Start file
+    """
+    
+    if os.name == 'nt': os.system(f'start {item}')
+    else: os.system(f'xdg-open {item}')
+
+# --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
+
+def dankware_banner() -> None:
+    
+    """
+    Dankware banner printer with github url
+    """
+    
+    from shutil import get_terminal_size
+    
+    num_lines = get_terminal_size().lines
+    banner="\n 8 888888888o.     \n 8 8888    `^888.  \n 8 8888        `88.\n 8 8888         `88\n 8 8888          88\n 8 8888          88\n 8 8888         ,88\n 8 8888        ,88'\n 8 8888    ,o88P'  \n 8 888888888P'     \n\n\n          .8.         \n         .888.        \n        :88888.       \n       . `88888.      \n      .8. `88888.     \n     .8`8. `88888.    \n    .8' `8. `88888.   \n   .8'   `8. `88888.  \n  .888888888. `88888. \n .8'       `8. `88888.\n\n\n b.             8\n 888o.          8\n Y88888o.       8\n .`Y888888o.    8\n 8o. `Y888888o. 8\n 8`Y8o. `Y88888o8\n 8   `Y8o. `Y8888\n 8      `Y8o. `Y8\n 8         `Y8o.`\n 8            `Yo\n\n\n 8 8888     ,88'\n 8 8888    ,88' \n 8 8888   ,88'  \n 8 8888  ,88'   \n 8 8888 ,88'    \n 8 8888 88'     \n 8 888888<      \n 8 8888 `Y8.    \n 8 8888   `Y8.  \n 8 8888     `Y8.\n\n\n `8.`888b                 ,8'\n  `8.`888b               ,8' \n   `8.`888b             ,8'  \n    `8.`888b     .b    ,8'   \n     `8.`888b    88b  ,8'    \n      `8.`888b .`888b,8'     \n       `8.`888b8.`8888'      \n        `8.`888`8.`88'       \n         `8.`8' `8,`'        \n          `8.`   `8'         \n\n\n          .8.         \n         .888.        \n        :88888.       \n       . `88888.      \n      .8. `88888.     \n     .8`8. `88888.    \n    .8' `8. `88888.   \n   .8'   `8. `88888.  \n  .888888888. `88888. \n .8'       `8. `88888.\n\n\n 8 888888888o.  \n 8 8888    `88. \n 8 8888     `88 \n 8 8888     ,88 \n 8 8888.   ,88' \n 8 888888888P'  \n 8 8888`8b      \n 8 8888 `8b.    \n 8 8888   `8b.  \n 8 8888     `88.\n\n\n 8 8888888888   \n 8 8888         \n 8 8888         \n 8 8888         \n 8 888888888888 \n 8 8888         \n 8 8888         \n 8 8888         \n 8 8888         \n 8 888888888888 \n "
+    
+    tmp = ""
+    to_print = []
+    sleep_time = []
+    sleep_time_1 = 0.05
+    sleep_time_2 = 0.01
+    sleep_time_3 = 0.333
+    sleep_time_variation = 0.01
+    
+    # sleep_time_1
+        
+    for line in align(clr(banner,4)).splitlines():
+        to_print.append(line)
+        sleep_time.append(sleep_time_1)
+        
+    for _ in range(num_lines):
+        tmp += "     \n"
+        to_print.append("     ")
+        sleep_time.append(sleep_time_1)
+        
+    # sleep_time_2
+    
+    tmp += (align(clr("github.com / SirDank")) + '\n')
+    to_print.append(align(clr("github.com / SirDank")))
+    sleep_time.append(sleep_time_2)
+    
+    for _ in range(int(num_lines/2)):
+        tmp += "     \n"
+        to_print.append("     ")
+        sleep_time.append(sleep_time_2)
+        sleep_time_2 = float(f'{(sleep_time_2 + sleep_time_variation):.3f}')
+        
+    # sleep_time_3
+
+    for _ in range(3):
+        to_print.append(tmp.replace(align(clr("github.com / SirDank")), align(clr("< github.com / SirDank >"))))
+        sleep_time.append(sleep_time_3)
+        to_print.append(tmp.replace(align(clr("github.com / SirDank")), align(clr("<   github.com / SirDank   >"))))
+        sleep_time.append(sleep_time_3)
+        to_print.append(tmp.replace(align(clr("github.com / SirDank")), align(clr("<     github.com / SirDank     >"))))
+        sleep_time.append(sleep_time_3)
+    to_print.append(tmp)
+    sleep_time.append(sleep_time_3)
+    
+    sleep_time[-1] = 4
+    
+    for _ in range(int(num_lines/2)):
+        to_print.append("     ")
+        sleep_time.append(0.01)
+        #sleep_time.append(sleep_time_2)
+        #sleep_time_2 = float(f'{(sleep_time_2 - sleep_time_variation):.3f}')
+        
+    # start
+        
+    cls(); print('\n' * 60)
+    for _, amt in zip(to_print, sleep_time):
+        print(_); time.sleep(amt)
+    
+    # finish
+        
+    cls()
```

### Comparing `dankware-3.3.4/dankware.egg-info/PKG-INFO` & `dankware-3.3.5/dankware.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,409 +1,410 @@
-Metadata-Version: 2.1
-Name: dankware
-Version: 3.3.4
-Summary: Python package with various features!
-Home-page: https://github.com/SirDank/dankware
-Author: SirDank
-Author-email: SirDankenstein@protonmail.com
-License: MIT
-Project-URL: GitHub, https://github.com/SirDank/dankware
-Project-URL: Bug Tracker, https://github.com/SirDank/dankware/issues
-Keywords: dank,dankware,multithread,gradient,fade,registry key,error traceback,random ip generator,github scraper,splash screen,hide window,file selector
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
-Classifier: Topic :: Software Development
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-<p align="center">
-  <b>~ Visits ~</b><br><br>
-  <img src="https://profile-counter.glitch.me/dankware/count.svg" />
-</p>
-
-<p align="center">
-  <b>~ Stats ~</b><br><br>
-  <img src="https://static.pepy.tech/personalized-badge/dankware?period=total&units=international_system&left_color=black&right_color=brightgreen&left_text=downloads" />
-  <img src="https://static.pepy.tech/personalized-badge/dankware?period=month&units=international_system&left_color=black&right_color=brightgreen&left_text=downloads%20/%20month" />
-  <img src="https://static.pepy.tech/personalized-badge/dankware?period=week&units=international_system&left_color=black&right_color=brightgreen&left_text=downloads%20/%20week" />
-</p>
-
-# 🚨 dankware 🚨
- Python module with various features! Install with the below command!
-```
-pip install dankware
-```
-
-Update to the latest version with the below command!
-```
-pip install --upgrade dankware
-```
- 
-# 🚨 Multithreading 🚨
-```py
-from dankware import multithread
-import time
-
-a = 0
-def example():
-    global a
-    a += 1
-    print(a)
-    time.sleep(5)
-        
-multithread(example, 10) # func: example | threads: 10 | single: 50 seconds | multi: 5 seconds
-```
-> <img width="500" alt="image" src="https://user-images.githubusercontent.com/52797753/224534374-4693f9fb-2c0c-426b-970d-face9926b9cd.png">
-
-```py
-from dankware import multithread
-import time
-
-new_list = [1, 2, 3, 4, 5]; sum = 0
-
-def example(num):
-    global sum
-    sum += num
-    time.sleep(5)
-
-multithread(example, 10, new_list) # input_one: list
-print(sum)
-```
-> <img width="500" alt="image" src="https://user-images.githubusercontent.com/52797753/224534424-f03f5884-e9c8-445f-8c0a-5bb227c35aed.png">
-
-```py
-from dankware import multithread
-import time
-
-list1 = [1, 2, 3, 4, 5]
-list2 = [5, 4, 3, 2, 1]
-
-def example(num1, num2):
-    print(num1 + num2)
-    time.sleep(5)
-
-multithread(example, 10, list1, list2) # input_one: list1 | input_two: list2
-```
-> <img width="500" alt="image" src="https://user-images.githubusercontent.com/52797753/224534446-c956dfb0-81a2-4717-bd80-e04484e76507.png">
-
-```py
-from dankware import multithread
-import time
-
-new_list = [1, 2, 3, 4, 5]
-
-def example(num1, num2):
-    print(num1 * num2)
-    time.sleep(5)
-
-multithread(example, 10, new_list, 5, progress_bar=False) # input_two: 5 | disabled progress bar
-```
-> <img width="60" alt="image" src="https://user-images.githubusercontent.com/52797753/153749433-95512c4d-afcd-4ad7-9797-caded6e44239.png">
-
-<p>&nbsp;</p>    
-
----  
-
-# 🚨 Export Registry Keys 🚨
-
-```py
-import os
-from dankware import export_registry_keys, is_admin
-
-# [NOTE]: this function requires admin privileges!
-
-export_path = "D:\\export.reg"
-registry_root = r'HKEY_CURRENT_USER'
-registry_path = r'Software\Google\Chrome\PreferenceMACs'
-#export_path = os.path.join(os.environ['USERPROFILE'], 'Desktop', 'export.reg')
-
-export_registry_keys(registry_root, registry_path, recursive=True, export_path=export_path)
-```
-> <img width="500" alt="image" src="https://user-images.githubusercontent.com/52797753/221345714-f1cdea4a-0c08-4c47-8c95-c64d95d12dec.png">
-
-> <img width="500" alt="image" src="https://user-images.githubusercontent.com/52797753/221345782-3a5a6ef0-d3b4-48a7-b8f8-c40f210b067d.png">
-
-<p>&nbsp;</p>    
-
----  
-
-# 🚨 Splash Screen 🚨
-
-```py
-from dankware import splash_screen
-# Supports: GIFs / PNGs / JPGs / BMPs / ICOs
-splash_screen("D:\\splash.gif", duration=5)
-# runs on main thread
-```
-
-```py
-from dankware import splash_screen
-from concurrent.futures import ThreadPoolExecutor
-ThreadPoolExecutor(1).submit(splash_screen, "splash.png", 5)
-# runs on separate thread
-```
-
-> <img width="250" alt="image" src="https://user-images.githubusercontent.com/52797753/228445332-004f8f69-d8be-4d36-95e5-9065891e4d09.gif">
-
-# 🚨 Error Traceback 🚨
-
-```py
-import sys
-from dankware import err, clr
-try: value = 1/0
-except: print(clr(err(sys.exc_info()),2))
-```
-> <img width="700" alt="image" src="https://user-images.githubusercontent.com/52797753/221346044-db739b15-b365-47b3-b6f1-20d199c58ab2.png">
-
-<p>&nbsp;</p>    
-
----  
-
-# 🚨 Scraping 🚨
-
-```py
-from dankware import github_downloads
-# full url > https://api.github.com/repos/EssentialsX/Essentials/releases/latest
-for url in github_downloads("EssentialsX/Essentials"): print(url)
-```
-> <img width="700" alt="image" src="https://user-images.githubusercontent.com/52797753/216242124-ed911013-bae4-4622-8c0a-0d11638da750.png">
-
-```py
-from dankware import github_file_selector
-# full url > https://api.github.com/repos/EssentialsX/Essentials/releases/latest
-for url in github_file_selector("EssentialsX/Essentials", "remove", ['AntiBuild', 'Discord', 'GeoIP', 'Protect', 'XMPP']): print(url)
-```
-> <img width="700" alt="image" src="https://user-images.githubusercontent.com/52797753/216241961-5359d662-a117-4eb4-b74e-e82b41a895bc.png">
-
-<p>&nbsp;</p>    
-
----  
-
-# 🚨 Generate Random IPs 🚨
-
-```py
-from dankware import random_ip
-print(random_ip())
-```
-
-> <img width="200" alt="image" src="https://user-images.githubusercontent.com/52797753/194127781-8f622448-4595-4c2a-a3e7-3e4356076840.png">
-
-<p>&nbsp;</p>    
-
----  
-
-# 🚨 Colour Special Characters 🚨
-
-```py
-from dankware import clr
-# default mode = 1
-# default colour_one = white
-# default colour_two = magenta
-print(clr("\n  > Hey! Long time no see :)"))
-#print(clr("\n  > Hey! Long time no see :)", colour_one = white, colour_two = magenta))
-```
-> <img width="350" alt="image" src="https://user-images.githubusercontent.com/52797753/153749617-bb0483fe-0385-490b-8695-72f448300c39.png">
-
-```py
-from dankware import clr, white, magenta
-# default mode = 1
-# default colour_one = white
-# default colour_two = magenta
-print(clr("\n  > Hey! Long time no see :)", colour_one = magenta, colour_two = white))
-```
-> <img width="350" alt="image" src="https://user-images.githubusercontent.com/52797753/220981909-d6361e6a-d109-447a-8401-85e2813e7859.png">
-
-```py
-from dankware import clr
-print(clr("\n  This is a string: True | This is an integer: False"))
-```
-> <img width="350" alt="image" src="https://user-images.githubusercontent.com/52797753/153749921-3332f3e6-eaa8-4bf1-ab4d-3fe35d245492.png">
-
-```py
-from dankware import clr, green, magenta
-# dankware now supports adding custom colours on both the text and the function itself!
-# colour_two = green
-print(clr(f"\n  > {magenta}Purple{white} thinks he's better than everyone else :(", colour_two=green))
-```
-> <img width="350" alt="image" src="https://user-images.githubusercontent.com/52797753/190898116-750e256e-a1d9-4c8a-a3b2-d0ac209fa0f7.png">
-
-```py
-from dankware import clr
-# mode = 2
-print(clr("\n  > Error in sector [7] redirecting... | INTEGRITY_CHECK_SUCCESS: TRUE",2))
-```
-> <img width="500" alt="image" src="https://user-images.githubusercontent.com/52797753/153749821-ae3e4dfd-26dc-4e08-a06e-677ac26457a1.png">
-
-```py
-from dankware import clr
-# mode = 3
-print(clr("\n  > Is this a randomly coloured string: TRUE | As you can see it does not colour True/False",3))
-```
-> <img width="650" alt="image" src="https://user-images.githubusercontent.com/52797753/155293415-7b065b5a-44dd-4fe7-995d-a25582f904cb.png">
-
-<p>&nbsp;</p>    
-
----  
-
-# 🚨 Banners 🚨
-
-```py
-banner = '''
-
-     888                   888                                             
-     888                   888           s i r . d a n k ' s               
-     888                   888                                             
- .d88888  8888b.  88888b.  888  888 888  888  888  8888b.  888d888 .d88b.  
-d88" 888     "88b 888 "88b 888 .88P 888  888  888     "88b 888P"  d8P  Y8b 
-888  888 .d888888 888  888 888888K  888  888  888 .d888888 888    88888888 
-Y88b 888 888  888 888  888 888 "88b Y88b 888 d88P 888  888 888    Y8b.     
- "Y88888 "Y888888 888  888 888  888  "Y8888888P"  "Y888888 888     "Y8888  
-
-'''
-```
-
-## ♦️ Colourize Banner (random) ♦️
-```py
-from dankware import clr
-# mode = 4
-print(clr(banner,4))
-```
-> <img width="550" alt="image" src="https://user-images.githubusercontent.com/52797753/153722086-2f372bfa-4872-46a0-81f8-cdf7c2344fd6.png">
-
-## ♦️ Align Banner (console center) ♦️
-```py
-from dankware import align
-print(align(banner)) # also works with single text line (even coloured)
-```
-> <img width="800" alt="image" src="https://user-images.githubusercontent.com/52797753/153722230-1f3b6103-6d8a-4537-9828-1718a6bd3367.png">
-
-## ♦️ Align Coloured Banner ♦️
-```py
-from dankware import align, clr
-print(align(clr(banner,4)))
-```
-> <img width="800" alt="image" src="https://user-images.githubusercontent.com/52797753/153722373-9925dd25-83bb-4d1c-83eb-bfaae1802088.png">
-
-<p>&nbsp;</p>    
-
----  
-
-# 🚨 Gradient Reworked [ Originally By @venaxyt ] 🚨
-
-```py
-from dankware import fade
-banner = '''
-
-                              888 d8b                   888    
-       v e n a x y t ' s      888 Y8P                   888    
-                              888                       888    
- .d88b.  888d888 8888b.   .d88888 888  .d88b.  88888b.  888888 
-d88P"88b 888P"      "88b d88" 888 888 d8P  Y8b 888 "88b 888    
-888  888 888    .d888888 888  888 888 88888888 888  888 888    
-Y88b 888 888    888  888 Y88b 888 888 Y8b.     888  888 Y88b.  
- "Y88888 888    "Y888888  "Y88888 888  "Y8888  888  888  "Y888 
-     888                                                       
-Y8b d88P                                                       
- "Y88P"                                                        
-
-
-'''
-```
-
-## ♦️ Black ♦️
-```py
-print(fade(banner, "black"))
-```
-> <img width="475" alt="image" src="https://user-images.githubusercontent.com/52797753/153722811-b257611e-9111-4a0e-92fb-7dbe503ce6db.png">
-```py
-print(fade(banner, "black-v"))
-```
-> <img width="475" alt="image" src="https://user-images.githubusercontent.com/52797753/153723205-a91eb1c6-07bc-4bc6-9fa6-52231e50a25c.png">
-
-## ♦️ Red ♦️
-```py
-print(fade(banner, "red"))
-```
-> <img width="475" alt="image" src="https://user-images.githubusercontent.com/52797753/153722946-3221bfd8-ff9d-4c9d-8b70-0c2736ec4e30.png">
-```py
-print(fade(banner, "red-v"))
-```
-> <img width="475" alt="image" src="https://user-images.githubusercontent.com/52797753/153723473-bdb75ea7-2df2-4f70-adb5-cf5caa57200a.png">
-
-## ♦️ Green ♦️
-```py
-print(fade(banner, "green"))
-```
-> <img width="475" alt="image" src="https://user-images.githubusercontent.com/52797753/153723050-c30bd3f1-989a-4141-b40a-2869a2dadef6.png">
-```py
-print(fade(banner, "green-v"))
-```
-> <img width="475" alt="image" src="https://user-images.githubusercontent.com/52797753/153723481-2e5c21b2-0f12-4d99-ab8d-a3e5c40e4c16.png">
-
-## ♦️ Cyan ♦️
-```py
-print(fade(banner, "cyan"))
-```
-> <img width="475" alt="image" src="https://user-images.githubusercontent.com/52797753/153723059-b4808365-6006-4726-b427-b6848e0fc0e5.png">
-```py
-print(fade(banner, "cyan-v"))
-```
-> <img width="475" alt="image" src="https://user-images.githubusercontent.com/52797753/153723496-8d03c5d3-601e-499d-80cd-51c3648957bf.png">
-
-## ♦️ Blue ♦️
-```py
-print(fade(banner, "blue"))
-```
-> <img width="475" alt="image" src="https://user-images.githubusercontent.com/52797753/153723092-0a32d8e6-680e-4df3-bdf1-089663f25f45.png">
-```py
-print(fade(banner, "blue-v"))
-```
-> <img width="475" alt="image" src="https://user-images.githubusercontent.com/52797753/153723509-41732010-b7d5-4867-95f9-690d47322536.png">
-
-## ♦️ Purple ♦️
-```py
-print(fade(banner, "purple"))
-```
-> <img width="475" alt="image" src="https://user-images.githubusercontent.com/52797753/153723148-2c94c459-1441-4752-a11f-a547754da7bc.png">
-```py
-print(fade(banner, "purple-v"))
-```
-> <img width="475" alt="image" src="https://user-images.githubusercontent.com/52797753/153723519-00aa980e-4a04-4d8d-a319-5691c1f8e517.png">
-
-## ♦️ Pink ♦️
-```py
-print(fade(banner, "pink-v"))
-```
-> <img width="475" alt="image" src="https://user-images.githubusercontent.com/52797753/153723540-b324dfe1-5ae2-4b66-ad3a-546a589558c8.png">
-
-## ♦️ Random ♦️
-```py
-print(fade(banner, "random"))
-```
-> <img width="475" alt="image" src="https://user-images.githubusercontent.com/52797753/153723545-0ea34ea7-1844-4ace-8948-3e71e28c0a30.png">
-
-<p>&nbsp;</p>    
-
----  
-
-# 🚨 Also check out 🚨
-<p align="center">
-  <a href="https://github.com/SirDank/dank.tool">
-  <img width="700" alt="image" src="https://user-images.githubusercontent.com/52797753/192086704-35f5a0db-3c5d-4782-95a9-6e2756cc8528.png">
-  </a>
-</p>
-
-<p>&nbsp;</p>    
-
----  
-
-# 🚨 Stats 🚨
-
-<br><p align="center"><img width="800" alt="image" src="https://repobeats.axiom.co/api/embed/ed44a86c2d46a8719705f5f57efde209b8cb5492.svg"></p><br>
-
-# 🚨 Star History 🚨
-
-<br><p align="center">[![Star History Chart](https://api.star-history.com/svg?repos=SirDank/dankware&type=Date)](https://star-history.com/#SirDank/dankware&Date)</p><br>
+Metadata-Version: 2.1
+Name: dankware
+Version: 3.3.5
+Summary: Python package with various features!
+Home-page: https://github.com/SirDank/dankware
+Author: SirDank
+Author-email: SirDankenstein@protonmail.com
+License: MIT
+Project-URL: GitHub, https://github.com/SirDank/dankware
+Project-URL: Bug Tracker, https://github.com/SirDank/dankware/issues
+Keywords: dank,dankware,multithread,gradient,fade,registry key,error traceback,random ip generator,github scraper,splash screen,hide window,file selector
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Natural Language :: English
+Classifier: Topic :: Software Development
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<p align="center">
+  <b>~ Visits ~</b><br><br>
+  <img src="https://profile-counter.glitch.me/dankware/count.svg" />
+</p>
+
+<p align="center">
+  <b>~ Stats ~</b><br><br>
+  <img src="https://static.pepy.tech/personalized-badge/dankware?period=total&units=international_system&left_color=black&right_color=brightgreen&left_text=downloads" />
+  <img src="https://static.pepy.tech/personalized-badge/dankware?period=month&units=international_system&left_color=black&right_color=brightgreen&left_text=downloads%20/%20month" />
+  <img src="https://static.pepy.tech/personalized-badge/dankware?period=week&units=international_system&left_color=black&right_color=brightgreen&left_text=downloads%20/%20week" />
+</p>
+
+# 🚨 dankware 🚨
+ Python module with various features! Install with the below command!
+```
+pip install dankware
+```
+
+Update to the latest version with the below command!
+```
+pip install --upgrade dankware
+```
+ 
+# 🚨 Multithreading 🚨
+```py
+from dankware import multithread
+import time
+
+a = 0
+def example():
+    global a
+    a += 1
+    print(a)
+    time.sleep(5)
+        
+multithread(example, 10) # func: example | threads: 10 | single: 50 seconds | multi: 5 seconds
+```
+> <img width="500" alt="image" src="https://user-images.githubusercontent.com/52797753/224534374-4693f9fb-2c0c-426b-970d-face9926b9cd.png">
+
+```py
+from dankware import multithread
+import time
+
+new_list = [1, 2, 3, 4, 5]; sum = 0
+
+def example(num):
+    global sum
+    sum += num
+    time.sleep(5)
+
+multithread(example, 10, new_list) # input_one: list
+print(sum)
+```
+> <img width="500" alt="image" src="https://user-images.githubusercontent.com/52797753/224534424-f03f5884-e9c8-445f-8c0a-5bb227c35aed.png">
+
+```py
+from dankware import multithread
+import time
+
+list1 = [1, 2, 3, 4, 5]
+list2 = [5, 4, 3, 2, 1]
+
+def example(num1, num2):
+    print(num1 + num2)
+    time.sleep(5)
+
+multithread(example, 10, list1, list2) # input_one: list1 | input_two: list2
+```
+> <img width="500" alt="image" src="https://user-images.githubusercontent.com/52797753/224534446-c956dfb0-81a2-4717-bd80-e04484e76507.png">
+
+```py
+from dankware import multithread
+import time
+
+new_list = [1, 2, 3, 4, 5]
+
+def example(num1, num2):
+    print(num1 * num2)
+    time.sleep(5)
+
+multithread(example, 10, new_list, 5, progress_bar=False) # input_two: 5 | disabled progress bar
+```
+> <img width="60" alt="image" src="https://user-images.githubusercontent.com/52797753/153749433-95512c4d-afcd-4ad7-9797-caded6e44239.png">
+
+<p>&nbsp;</p>    
+
+---  
+
+# 🚨 Export Registry Keys 🚨
+
+```py
+import os
+from dankware import export_registry_keys, is_admin
+
+# [NOTE]: this function requires admin privileges!
+
+export_path = "D:\\export.reg"
+registry_root = r'HKEY_CURRENT_USER'
+registry_path = r'Software\Google\Chrome\PreferenceMACs'
+#export_path = os.path.join(os.environ['USERPROFILE'], 'Desktop', 'export.reg')
+
+export_registry_keys(registry_root, registry_path, recursive=True, export_path=export_path)
+```
+> <img width="500" alt="image" src="https://user-images.githubusercontent.com/52797753/221345714-f1cdea4a-0c08-4c47-8c95-c64d95d12dec.png">
+
+> <img width="500" alt="image" src="https://user-images.githubusercontent.com/52797753/221345782-3a5a6ef0-d3b4-48a7-b8f8-c40f210b067d.png">
+
+<p>&nbsp;</p>    
+
+---  
+
+# 🚨 Splash Screen 🚨
+
+```py
+from dankware import splash_screen
+# Supports: GIFs / PNGs / JPGs / BMPs / ICOs
+splash_screen("D:\\splash.gif", duration=5)
+# runs on main thread
+```
+
+```py
+from dankware import splash_screen
+from concurrent.futures import ThreadPoolExecutor
+ThreadPoolExecutor(1).submit(splash_screen, "splash.png", 5)
+# runs on separate thread
+```
+
+> <img width="250" alt="image" src="https://user-images.githubusercontent.com/52797753/228445332-004f8f69-d8be-4d36-95e5-9065891e4d09.gif">
+
+# 🚨 Error Traceback 🚨
+
+```py
+import sys
+from dankware import err, clr
+try: value = 1/0
+except: print(clr(err(sys.exc_info()),2))
+```
+> <img width="700" alt="image" src="https://user-images.githubusercontent.com/52797753/221346044-db739b15-b365-47b3-b6f1-20d199c58ab2.png">
+
+<p>&nbsp;</p>    
+
+---  
+
+# 🚨 Scraping 🚨
+
+```py
+from dankware import github_downloads
+# full url > https://api.github.com/repos/EssentialsX/Essentials/releases/latest
+for url in github_downloads("EssentialsX/Essentials"): print(url)
+```
+> <img width="700" alt="image" src="https://user-images.githubusercontent.com/52797753/216242124-ed911013-bae4-4622-8c0a-0d11638da750.png">
+
+```py
+from dankware import github_file_selector
+# full url > https://api.github.com/repos/EssentialsX/Essentials/releases/latest
+for url in github_file_selector("EssentialsX/Essentials", "remove", ['AntiBuild', 'Discord', 'GeoIP', 'Protect', 'XMPP']): print(url)
+```
+> <img width="700" alt="image" src="https://user-images.githubusercontent.com/52797753/216241961-5359d662-a117-4eb4-b74e-e82b41a895bc.png">
+
+<p>&nbsp;</p>    
+
+---  
+
+# 🚨 Generate Random IPs 🚨
+
+```py
+from dankware import random_ip
+print(random_ip())
+```
+
+> <img width="200" alt="image" src="https://user-images.githubusercontent.com/52797753/194127781-8f622448-4595-4c2a-a3e7-3e4356076840.png">
+
+<p>&nbsp;</p>    
+
+---  
+
+# 🚨 Colour Special Characters 🚨
+
+```py
+from dankware import clr
+# default mode = 1
+# default colour_one = white
+# default colour_two = magenta
+print(clr("\n  > Hey! Long time no see :)"))
+#print(clr("\n  > Hey! Long time no see :)", colour_one = white, colour_two = magenta))
+```
+> <img width="350" alt="image" src="https://user-images.githubusercontent.com/52797753/153749617-bb0483fe-0385-490b-8695-72f448300c39.png">
+
+```py
+from dankware import clr, white, magenta
+# default mode = 1
+# default colour_one = white
+# default colour_two = magenta
+print(clr("\n  > Hey! Long time no see :)", colour_one = magenta, colour_two = white))
+```
+> <img width="350" alt="image" src="https://user-images.githubusercontent.com/52797753/220981909-d6361e6a-d109-447a-8401-85e2813e7859.png">
+
+```py
+from dankware import clr
+print(clr("\n  This is a string: True | This is an integer: False"))
+```
+> <img width="350" alt="image" src="https://user-images.githubusercontent.com/52797753/153749921-3332f3e6-eaa8-4bf1-ab4d-3fe35d245492.png">
+
+```py
+from dankware import clr, green, magenta
+# dankware now supports adding custom colours on both the text and the function itself!
+# colour_two = green
+print(clr(f"\n  > {magenta}Purple{white} thinks he's better than everyone else :(", colour_two=green))
+```
+> <img width="350" alt="image" src="https://user-images.githubusercontent.com/52797753/190898116-750e256e-a1d9-4c8a-a3b2-d0ac209fa0f7.png">
+
+```py
+from dankware import clr
+# mode = 2
+print(clr("\n  > Error in sector [7] redirecting... | INTEGRITY_CHECK_SUCCESS: TRUE",2))
+```
+> <img width="500" alt="image" src="https://user-images.githubusercontent.com/52797753/153749821-ae3e4dfd-26dc-4e08-a06e-677ac26457a1.png">
+
+```py
+from dankware import clr
+# mode = 3
+print(clr("\n  > Is this a randomly coloured string: TRUE | As you can see it does not colour True/False",3))
+```
+> <img width="650" alt="image" src="https://user-images.githubusercontent.com/52797753/155293415-7b065b5a-44dd-4fe7-995d-a25582f904cb.png">
+
+<p>&nbsp;</p>    
+
+---  
+
+# 🚨 Banners 🚨
+
+```py
+banner = '''
+
+     888                   888                                             
+     888                   888           s i r . d a n k ' s               
+     888                   888                                             
+ .d88888  8888b.  88888b.  888  888 888  888  888  8888b.  888d888 .d88b.  
+d88" 888     "88b 888 "88b 888 .88P 888  888  888     "88b 888P"  d8P  Y8b 
+888  888 .d888888 888  888 888888K  888  888  888 .d888888 888    88888888 
+Y88b 888 888  888 888  888 888 "88b Y88b 888 d88P 888  888 888    Y8b.     
+ "Y88888 "Y888888 888  888 888  888  "Y8888888P"  "Y888888 888     "Y8888  
+
+'''
+```
+
+## ♦️ Colourize Banner (random) ♦️
+```py
+from dankware import clr
+# mode = 4
+print(clr(banner,4))
+```
+> <img width="550" alt="image" src="https://user-images.githubusercontent.com/52797753/153722086-2f372bfa-4872-46a0-81f8-cdf7c2344fd6.png">
+
+## ♦️ Align Banner (console center) ♦️
+```py
+from dankware import align
+print(align(banner)) # also works with single text line (even coloured)
+```
+> <img width="800" alt="image" src="https://user-images.githubusercontent.com/52797753/153722230-1f3b6103-6d8a-4537-9828-1718a6bd3367.png">
+
+## ♦️ Align Coloured Banner ♦️
+```py
+from dankware import align, clr
+print(align(clr(banner,4)))
+```
+> <img width="800" alt="image" src="https://user-images.githubusercontent.com/52797753/153722373-9925dd25-83bb-4d1c-83eb-bfaae1802088.png">
+
+<p>&nbsp;</p>    
+
+---  
+
+# 🚨 Gradient Reworked [ Originally By @venaxyt ] 🚨
+
+```py
+from dankware import fade
+banner = '''
+
+                              888 d8b                   888    
+       v e n a x y t ' s      888 Y8P                   888    
+                              888                       888    
+ .d88b.  888d888 8888b.   .d88888 888  .d88b.  88888b.  888888 
+d88P"88b 888P"      "88b d88" 888 888 d8P  Y8b 888 "88b 888    
+888  888 888    .d888888 888  888 888 88888888 888  888 888    
+Y88b 888 888    888  888 Y88b 888 888 Y8b.     888  888 Y88b.  
+ "Y88888 888    "Y888888  "Y88888 888  "Y8888  888  888  "Y888 
+     888                                                       
+Y8b d88P                                                       
+ "Y88P"                                                        
+
+
+'''
+```
+
+## ♦️ Black ♦️
+```py
+print(fade(banner, "black"))
+```
+> <img width="475" alt="image" src="https://user-images.githubusercontent.com/52797753/153722811-b257611e-9111-4a0e-92fb-7dbe503ce6db.png">
+```py
+print(fade(banner, "black-v"))
+```
+> <img width="475" alt="image" src="https://user-images.githubusercontent.com/52797753/153723205-a91eb1c6-07bc-4bc6-9fa6-52231e50a25c.png">
+
+## ♦️ Red ♦️
+```py
+print(fade(banner, "red"))
+```
+> <img width="475" alt="image" src="https://user-images.githubusercontent.com/52797753/153722946-3221bfd8-ff9d-4c9d-8b70-0c2736ec4e30.png">
+```py
+print(fade(banner, "red-v"))
+```
+> <img width="475" alt="image" src="https://user-images.githubusercontent.com/52797753/153723473-bdb75ea7-2df2-4f70-adb5-cf5caa57200a.png">
+
+## ♦️ Green ♦️
+```py
+print(fade(banner, "green"))
+```
+> <img width="475" alt="image" src="https://user-images.githubusercontent.com/52797753/153723050-c30bd3f1-989a-4141-b40a-2869a2dadef6.png">
+```py
+print(fade(banner, "green-v"))
+```
+> <img width="475" alt="image" src="https://user-images.githubusercontent.com/52797753/153723481-2e5c21b2-0f12-4d99-ab8d-a3e5c40e4c16.png">
+
+## ♦️ Cyan ♦️
+```py
+print(fade(banner, "cyan"))
+```
+> <img width="475" alt="image" src="https://user-images.githubusercontent.com/52797753/153723059-b4808365-6006-4726-b427-b6848e0fc0e5.png">
+```py
+print(fade(banner, "cyan-v"))
+```
+> <img width="475" alt="image" src="https://user-images.githubusercontent.com/52797753/153723496-8d03c5d3-601e-499d-80cd-51c3648957bf.png">
+
+## ♦️ Blue ♦️
+```py
+print(fade(banner, "blue"))
+```
+> <img width="475" alt="image" src="https://user-images.githubusercontent.com/52797753/153723092-0a32d8e6-680e-4df3-bdf1-089663f25f45.png">
+```py
+print(fade(banner, "blue-v"))
+```
+> <img width="475" alt="image" src="https://user-images.githubusercontent.com/52797753/153723509-41732010-b7d5-4867-95f9-690d47322536.png">
+
+## ♦️ Purple ♦️
+```py
+print(fade(banner, "purple"))
+```
+> <img width="475" alt="image" src="https://user-images.githubusercontent.com/52797753/153723148-2c94c459-1441-4752-a11f-a547754da7bc.png">
+```py
+print(fade(banner, "purple-v"))
+```
+> <img width="475" alt="image" src="https://user-images.githubusercontent.com/52797753/153723519-00aa980e-4a04-4d8d-a319-5691c1f8e517.png">
+
+## ♦️ Pink ♦️
+```py
+print(fade(banner, "pink-v"))
+```
+> <img width="475" alt="image" src="https://user-images.githubusercontent.com/52797753/153723540-b324dfe1-5ae2-4b66-ad3a-546a589558c8.png">
+
+## ♦️ Random ♦️
+```py
+print(fade(banner, "random"))
+```
+> <img width="475" alt="image" src="https://user-images.githubusercontent.com/52797753/153723545-0ea34ea7-1844-4ace-8948-3e71e28c0a30.png">
+
+<p>&nbsp;</p>    
+
+---  
+
+# 🚨 Also check out 🚨
+<p align="center">
+  <a href="https://github.com/SirDank/dank.tool">
+  <img width="700" alt="image" src="https://user-images.githubusercontent.com/52797753/192086704-35f5a0db-3c5d-4782-95a9-6e2756cc8528.png">
+  </a>
+</p>
+
+<p>&nbsp;</p>    
+
+---  
+
+# 🚨 Stats 🚨
+
+<br><p align="center"><img width="800" alt="image" src="https://repobeats.axiom.co/api/embed/ed44a86c2d46a8719705f5f57efde209b8cb5492.svg"></p><br>
+
+# 🚨 Star History 🚨
+
+<br><p align="center">[![Star History Chart](https://api.star-history.com/svg?repos=SirDank/dankware&type=Date)](https://star-history.com/#SirDank/dankware&Date)</p><br>
```

