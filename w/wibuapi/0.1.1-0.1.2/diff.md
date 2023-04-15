# Comparing `tmp/wibuapi-0.1.1.tar.gz` & `tmp/wibuapi-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wibuapi-0.1.1.tar", last modified: Sun Mar 26 14:21:16 2023, max compression
+gzip compressed data, was "wibuapi-0.1.2.tar", last modified: Sat Apr 15 20:18:31 2023, max compression
```

## Comparing `wibuapi-0.1.1.tar` & `wibuapi-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 14:21:16.482707 wibuapi-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35145 2023-03-26 14:21:03.000000 wibuapi-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7942 2023-03-26 14:21:16.482707 wibuapi-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7276 2023-03-26 14:21:03.000000 wibuapi-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 14:21:16.482707 wibuapi-0.1.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-26 14:21:03.000000 wibuapi-0.1.1/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-03-26 14:21:03.000000 wibuapi-0.1.1/examples/google_search.py
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-03-26 14:21:03.000000 wibuapi-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-26 14:21:16.482707 wibuapi-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-03-26 14:21:03.000000 wibuapi-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 14:21:16.482707 wibuapi-0.1.1/wibuapi/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-03-26 14:21:03.000000 wibuapi-0.1.1/wibuapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15025 2023-03-26 14:21:03.000000 wibuapi-0.1.1/wibuapi/wibuapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-03-26 14:21:03.000000 wibuapi-0.1.1/wibuapi/zyxdevs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 14:21:16.482707 wibuapi-0.1.1/wibuapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7942 2023-03-26 14:21:16.000000 wibuapi-0.1.1/wibuapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-03-26 14:21:16.000000 wibuapi-0.1.1/wibuapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-26 14:21:16.000000 wibuapi-0.1.1/wibuapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-26 14:21:16.000000 wibuapi-0.1.1/wibuapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-26 14:21:16.000000 wibuapi-0.1.1/wibuapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 20:18:31.534878 wibuapi-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35145 2023-04-15 20:18:18.000000 wibuapi-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9476 2023-04-15 20:18:31.534878 wibuapi-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8810 2023-04-15 20:18:18.000000 wibuapi-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-15 20:18:18.000000 wibuapi-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 20:18:31.534878 wibuapi-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-15 20:18:18.000000 wibuapi-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 20:18:31.530878 wibuapi-0.1.2/wibuapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-15 20:18:18.000000 wibuapi-0.1.2/wibuapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16424 2023-04-15 20:18:18.000000 wibuapi-0.1.2/wibuapi/wibuapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-04-15 20:18:18.000000 wibuapi-0.1.2/wibuapi/zyxdevs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 20:18:31.534878 wibuapi-0.1.2/wibuapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9476 2023-04-15 20:18:31.000000 wibuapi-0.1.2/wibuapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-15 20:18:31.000000 wibuapi-0.1.2/wibuapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 20:18:31.000000 wibuapi-0.1.2/wibuapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-15 20:18:31.000000 wibuapi-0.1.2/wibuapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-15 20:18:31.000000 wibuapi-0.1.2/wibuapi.egg-info/top_level.txt
```

### Comparing `wibuapi-0.1.1/LICENSE` & `wibuapi-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wibuapi-0.1.1/PKG-INFO` & `wibuapi-0.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wibuapi
-Version: 0.1.1
+Version: 0.1.2
 Summary: Official Python Wrapper for Wibu API.
 Home-page: https://github.com/zYxDevs/wibu-api-py
 Author: Yoga Pranata
 Author-email: yoga@zyxdevs.eu.org
 License: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -34,46 +34,66 @@
 
 #### Get latest update
 ```
 pip3 install -U wibuapi
 ```
 
 #### Install from repo
-```bash
+```shell
 root@zyxdevs:~ git clone https://github.com/zYxDevs/wibu-api-py wibuapi
 root@zyxdevs:~ cd wibuapi
 root@zyxdevs:~ python3 setup.py install
 ```
 
 ## Telegram Bot:
-_I've created official telegram bot to interacted with WibuAPI_
+_There's many useful features in bot but it required big resource, so i make it for paid users only. If you interest to buy PM me on Telegram._
+
+**Paid Features:**
+
+- [x] LH Translation zipper
+- [x] Shinigami zipper
+- [x] Worldmanhwas zipper
+- [x] Maid Manga zipper
+- [x] Mangayaro zipper
+- [x] Cosmicscans zipper
+- [x] nHentai zipper
+- [x] Sheakomik, Sheamanga zipper
+- [x] Komikindo.info zipper
+- [x] Otomi Games
+  - [x] Search parser
+  - [x] Download link scrapper
+- [x] Javhd
+  - [x] Search parser
+  - [x] Download link scrapper
+- [x] Other incoming features
 
 [![WibuAPI Bot](https://img.shields.io/badge/WibuAPI-Bot-blue?&logo=telegram)](https://wibuapibot.t.me)
 [![Yoga Pranata](https://img.shields.io/badge/Yoga-Pranata-blue?&logo=telegram)](https://t.me/Yoga_CIC)
 [![Supoort Chat](https://img.shields.io/badge/Support-Chat-blue?&logo=telegram)](https://ybotssupport.t.me)
 [![Update Channel](https://img.shields.io/badge/Update-Channel-blue?&logo=telegram)](https://spreadnetworks.t.me)
 
 ## Examples:
 ### Importing modules
 ```python
 from wibuapi import WibuAPI
 api = WibuAPI()
 ```
 
 ### Anime, Hentai, Donghua
-_For nekopoi scrapper only works in [bot](https://t.me/wibuapibot)._
+_For nekopoi search only works in [bot](https://t.me/wibuapibot)._
 
 | Website | Params |
 | :-: | :-: |
 | [Lendrive](https://github.com/zYxDevs/wibu-api-py#lendrive)| link |
 | [Anichin](https://github.com/zYxDevs/wibu-api-py#anichin) | link |
 | [Donghua](https://github.com/zYxDevs/wibu-api-py#donghua) | link |
 | [Kusonime](https://github.com/zYxDevs/wibu-api-py#kusonime) | link |
 | [Doronime](https://github.com/zYxDevs/wibu-api-py#doronime) | link |
 | [Samehadaku](https://github.com/zYxDevs/wibu-api-py#samehadaku) | link |
+| [Nekopoi](https://github.com/zYxDevs/wibu-api-py#nekopoi) | link |
 
 #### [Lendrive](https://lendrive.web.id)
 ```python
 # works with batch, bd, and single eps link
 url = "https://lendrive.web.id/tondemo-skill-de-isekai-hourou-meshi-ep-04-dual-subs-x265-hevc-subtitle-indonesia-english/"
 res = api.lendrive(url)
 print(res)
@@ -99,41 +119,51 @@
 ```python
 # works with batch, bd, and single eps link
 url = "https://kusonime.com/isekai-ojisan-batch-subtitle-indonesia/"
 res = api.kusonime(url)
 print(res)
 ```
 
-#### [Doronime](https://doronime.id)
+#### [Doronime](https://doroni.me)
 ```python
 # works with batch, bd, and single eps link
-url = "https://doronime.id/anime/om-ke-isekai/batch"
+url = "https://doroni.me/anime/om-ke-isekai/batch"
 res = api.doronime(url)
 print(res)
 ```
 
 #### [Samehadaku](https://samehadaku.run)
 ```python
 # works with batch, bd, and single eps link
 url = "https://samehadaku.run/nierautomata-ver1-1a-episode-8/"
 res = api.samehadaku(url)
 print(res)
 ```
 
+#### [Nekopoi](https://nekopoi.care)
+```python
+# works with single eps link (hentai, jav)
+url = "https://nekopoi.care/koumi-jima-shuu-7-de-umeru-mesu-tachi-episode-1-subtitle-indonesia/"
+res = api.nekopoi(url)
+print(res)
+```
+
 ### Manga, Doujin, Manhua, Manhwa
 
 | Website | Params |
 | :-: | :-: |
 | [Rawkuma](https://github.com/zYxDevs/wibu-api-py#rawkuma) | link |
 | [Westmanga](https://github.com/zYxDevs/wibu-api-py#westmanga) | link |
 | [Komikindo](https://github.com/zYxDevs/wibu-api-py#komikindo) | link |
 | [Mangatale](https://github.com/zYxDevs/wibu-api-py#mangatale) | link |
 | [Kiryuu](https://github.com/zYxDevs/wibu-api-py#kiryuu) | link |
 | [Masterkomik](https://github.com/zYxDevs/wibu-api-py#masterkomik) | link |
+| [Mangakita](https://github.com/zYxDevs/wibu-api-py#mangakita) | link |
 | [Doujindesu](https://github.com/zYxDevs/wibu-api-py#doujindesu) | link |
+| [Crotpedia](https://github.com/zYxDevs/wibu-api-py#crotpedia) | link |
 
 #### [Rawkuma](https://rawkuma.com)
 ```python
 # works with list and single chapter
 # list: https://rawkuma.com/manga/guilty-circle/
 # single: https://rawkuma.com/guilty-circle-chapter-83/
 url = "https://rawkuma.com/manga/guilty-circle/"
@@ -187,32 +217,51 @@
 # list: https://masterkomik.com/manga/max-level-player/
 # single: https://masterkomik.com/max-level-player-chapter-07/
 url = "https://masterkomik.com/manga/max-level-player/"
 res = api.masterkomik(url)
 print(res)
 ```
 
+#### [Mangakita](https://mangakita.net)
+```python
+# works with list and single chapter
+# list: https://mangakita.net/manga/please-go-home-akutsu-san/
+# single: https://mangakita.net/please-go-home-akutsu-san-chapter-137/
+url = "https://mangakita.net/manga/please-go-home-akutsu-san/"
+res = api.mangakita(url)
+print(res)
+```
+
 #### [Doujindesu](https://212.32.226.234)
 ```python
 # works with list and single chapter
 # list: https://212.32.226.234/manga/i-cant-stand-it-ajumma/
 # single: https://212.32.226.234/i-cant-stand-it-ajumma-chapter-20/
 url = "https://212.32.226.234/manga/i-cant-stand-it-ajumma/"
 res = api.doujindesu(url)
 print(res)
 ```
 
+#### [Crotpedia](https://38.242.194.12)
+```python
+# works with list chapter
+# list: https://38.242.194.12/baca/series/young-housemaid/
+url = "https://38.242.194.12/baca/series/young-housemaid/"
+res = api.crotpedia(url)
+print(res)
+```
+
 **Note:**
 ```
 You can see more endpoints on https://wibu-api.eu.org/docs or wibuapi.py file.
-```
-```
+
 Sometimes their will change domains, that will make some endpoints wont works.
 Please let me know when their sites change domains, I will asap fix dead endpoints.
 
+If you find any bugs or requests a new sites,
 You can ping me on telegram or make new issue.
 ```
 
 ## Copyright:
 ```
 © 2022-2023 Yoga Pranata
 ```
```

### Comparing `wibuapi-0.1.1/README.md` & `wibuapi-0.1.2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -16,46 +16,66 @@
 
 #### Get latest update
 ```
 pip3 install -U wibuapi
 ```
 
 #### Install from repo
-```bash
+```shell
 root@zyxdevs:~ git clone https://github.com/zYxDevs/wibu-api-py wibuapi
 root@zyxdevs:~ cd wibuapi
 root@zyxdevs:~ python3 setup.py install
 ```
 
 ## Telegram Bot:
-_I've created official telegram bot to interacted with WibuAPI_
+_There's many useful features in bot but it required big resource, so i make it for paid users only. If you interest to buy PM me on Telegram._
+
+**Paid Features:**
+
+- [x] LH Translation zipper
+- [x] Shinigami zipper
+- [x] Worldmanhwas zipper
+- [x] Maid Manga zipper
+- [x] Mangayaro zipper
+- [x] Cosmicscans zipper
+- [x] nHentai zipper
+- [x] Sheakomik, Sheamanga zipper
+- [x] Komikindo.info zipper
+- [x] Otomi Games
+  - [x] Search parser
+  - [x] Download link scrapper
+- [x] Javhd
+  - [x] Search parser
+  - [x] Download link scrapper
+- [x] Other incoming features
 
 [![WibuAPI Bot](https://img.shields.io/badge/WibuAPI-Bot-blue?&logo=telegram)](https://wibuapibot.t.me)
 [![Yoga Pranata](https://img.shields.io/badge/Yoga-Pranata-blue?&logo=telegram)](https://t.me/Yoga_CIC)
 [![Supoort Chat](https://img.shields.io/badge/Support-Chat-blue?&logo=telegram)](https://ybotssupport.t.me)
 [![Update Channel](https://img.shields.io/badge/Update-Channel-blue?&logo=telegram)](https://spreadnetworks.t.me)
 
 ## Examples:
 ### Importing modules
 ```python
 from wibuapi import WibuAPI
 api = WibuAPI()
 ```
 
 ### Anime, Hentai, Donghua
-_For nekopoi scrapper only works in [bot](https://t.me/wibuapibot)._
+_For nekopoi search only works in [bot](https://t.me/wibuapibot)._
 
 | Website | Params |
 | :-: | :-: |
 | [Lendrive](https://github.com/zYxDevs/wibu-api-py#lendrive)| link |
 | [Anichin](https://github.com/zYxDevs/wibu-api-py#anichin) | link |
 | [Donghua](https://github.com/zYxDevs/wibu-api-py#donghua) | link |
 | [Kusonime](https://github.com/zYxDevs/wibu-api-py#kusonime) | link |
 | [Doronime](https://github.com/zYxDevs/wibu-api-py#doronime) | link |
 | [Samehadaku](https://github.com/zYxDevs/wibu-api-py#samehadaku) | link |
+| [Nekopoi](https://github.com/zYxDevs/wibu-api-py#nekopoi) | link |
 
 #### [Lendrive](https://lendrive.web.id)
 ```python
 # works with batch, bd, and single eps link
 url = "https://lendrive.web.id/tondemo-skill-de-isekai-hourou-meshi-ep-04-dual-subs-x265-hevc-subtitle-indonesia-english/"
 res = api.lendrive(url)
 print(res)
@@ -81,41 +101,51 @@
 ```python
 # works with batch, bd, and single eps link
 url = "https://kusonime.com/isekai-ojisan-batch-subtitle-indonesia/"
 res = api.kusonime(url)
 print(res)
 ```
 
-#### [Doronime](https://doronime.id)
+#### [Doronime](https://doroni.me)
 ```python
 # works with batch, bd, and single eps link
-url = "https://doronime.id/anime/om-ke-isekai/batch"
+url = "https://doroni.me/anime/om-ke-isekai/batch"
 res = api.doronime(url)
 print(res)
 ```
 
 #### [Samehadaku](https://samehadaku.run)
 ```python
 # works with batch, bd, and single eps link
 url = "https://samehadaku.run/nierautomata-ver1-1a-episode-8/"
 res = api.samehadaku(url)
 print(res)
 ```
 
+#### [Nekopoi](https://nekopoi.care)
+```python
+# works with single eps link (hentai, jav)
+url = "https://nekopoi.care/koumi-jima-shuu-7-de-umeru-mesu-tachi-episode-1-subtitle-indonesia/"
+res = api.nekopoi(url)
+print(res)
+```
+
 ### Manga, Doujin, Manhua, Manhwa
 
 | Website | Params |
 | :-: | :-: |
 | [Rawkuma](https://github.com/zYxDevs/wibu-api-py#rawkuma) | link |
 | [Westmanga](https://github.com/zYxDevs/wibu-api-py#westmanga) | link |
 | [Komikindo](https://github.com/zYxDevs/wibu-api-py#komikindo) | link |
 | [Mangatale](https://github.com/zYxDevs/wibu-api-py#mangatale) | link |
 | [Kiryuu](https://github.com/zYxDevs/wibu-api-py#kiryuu) | link |
 | [Masterkomik](https://github.com/zYxDevs/wibu-api-py#masterkomik) | link |
+| [Mangakita](https://github.com/zYxDevs/wibu-api-py#mangakita) | link |
 | [Doujindesu](https://github.com/zYxDevs/wibu-api-py#doujindesu) | link |
+| [Crotpedia](https://github.com/zYxDevs/wibu-api-py#crotpedia) | link |
 
 #### [Rawkuma](https://rawkuma.com)
 ```python
 # works with list and single chapter
 # list: https://rawkuma.com/manga/guilty-circle/
 # single: https://rawkuma.com/guilty-circle-chapter-83/
 url = "https://rawkuma.com/manga/guilty-circle/"
@@ -169,32 +199,51 @@
 # list: https://masterkomik.com/manga/max-level-player/
 # single: https://masterkomik.com/max-level-player-chapter-07/
 url = "https://masterkomik.com/manga/max-level-player/"
 res = api.masterkomik(url)
 print(res)
 ```
 
+#### [Mangakita](https://mangakita.net)
+```python
+# works with list and single chapter
+# list: https://mangakita.net/manga/please-go-home-akutsu-san/
+# single: https://mangakita.net/please-go-home-akutsu-san-chapter-137/
+url = "https://mangakita.net/manga/please-go-home-akutsu-san/"
+res = api.mangakita(url)
+print(res)
+```
+
 #### [Doujindesu](https://212.32.226.234)
 ```python
 # works with list and single chapter
 # list: https://212.32.226.234/manga/i-cant-stand-it-ajumma/
 # single: https://212.32.226.234/i-cant-stand-it-ajumma-chapter-20/
 url = "https://212.32.226.234/manga/i-cant-stand-it-ajumma/"
 res = api.doujindesu(url)
 print(res)
 ```
 
+#### [Crotpedia](https://38.242.194.12)
+```python
+# works with list chapter
+# list: https://38.242.194.12/baca/series/young-housemaid/
+url = "https://38.242.194.12/baca/series/young-housemaid/"
+res = api.crotpedia(url)
+print(res)
+```
+
 **Note:**
 ```
 You can see more endpoints on https://wibu-api.eu.org/docs or wibuapi.py file.
-```
-```
+
 Sometimes their will change domains, that will make some endpoints wont works.
 Please let me know when their sites change domains, I will asap fix dead endpoints.
 
+If you find any bugs or requests a new sites,
 You can ping me on telegram or make new issue.
 ```
 
 ## Copyright:
 ```
 © 2022-2023 Yoga Pranata
 ```
```

### Comparing `wibuapi-0.1.1/setup.py` & `wibuapi-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r") as txt:
     long_description = txt.read()
 
 setuptools.setup(
     name="wibuapi",
-    version="0.1.1",
+    version="0.1.2",
     description="Official Python Wrapper for Wibu API.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
     author="Yoga Pranata",
     author_email="yoga@zyxdevs.eu.org",
     url="https://github.com/zYxDevs/wibu-api-py",
```

### Comparing `wibuapi-0.1.1/wibuapi/wibuapi.py` & `wibuapi-0.1.2/wibuapi/wibuapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,30 +37,41 @@
         https://anichin.vip/soul-land-season-2-episode-226-252-subtitle-indonesia/
         """
         try:
             url = f"{self.base_url}/anime/anichin?link={link}"
             response = get(url, timeout=15).json()
             return dumps(response, indent=2)
         except Exception as e:
-            return "An error occured report on @YBotsSupport\n\n{}".format(e)
+            return f"An error occured report on @YBotsSupport\n\n{e}"
+
+    def nekopoi(self, link: str):
+        """works with single eps link
+        https://nekopoi.care/koumi-jima-shuu-7-de-umeru-mesu-tachi-episode-1-subtitle-indonesia/
+        """
+        try:
+            url = f"{self.base_url}/anime/nekopoi?link={link}"
+            response = get(url, timeout=15).json()
+            return dumps(response, indent=2)
+        except Exception as e:
+            return f"An error occured report on @YBotsSupport\n\n{e}"
 
     def kusonime(self, link: str):
         """works with batch, bd, and single eps link
         https://kusonime.com/isekai-ojisan-batch-subtitle-indonesia/
         """
         try:
             url = f"{self.base_url}/anime/kusonime?link={link}"
             response = get(url, timeout=15).json()
             return dumps(response, indent=2)
         except Exception as e:
             return f"An error occured report on @YBotsSupport\n\n{e}"
 
     def doronime(self, link: str):
         """works with batch, bd, and single eps link
-        https://doronime.id/anime/om-ke-isekai/batch
+        https://doroni.me/anime/om-ke-isekai/batch
         """
         try:
             url = f"{self.base_url}/anime/doronime?link={link}"
             response = get(url, timeout=15).json()
             return dumps(response, indent=2)
         except Exception as e:
             return f"An error occured report on @YBotsSupport\n\n{e}"
@@ -144,26 +155,49 @@
         try:
             url = f"{self.base_url}/manga/masterkomik?link={link}"
             response = get(url, timeout=15).json()
             return dumps(response, indent=2)
         except Exception as e:
             return f"An error occured report on @YBotsSupport\n\n{e}"
 
+    def mangakita(self, link: str):
+        """work with list and single chapter
+        list: https://mangakita.net/manga/please-go-home-akutsu-san/
+        single: https://mangakita.net/please-go-home-akutsu-san-chapter-137/
+        """
+        try:
+            url = f"{self.base_url}/manga/mangakita?link={link}"
+            response = get(url, timeout=15).json()
+            return dumps(response, indent=2)
+        except Exception as e:
+            return f"An error occured report on @YBotsSupport\n\n{e}"
+
     def doujindesu(self, link: str):
         """works with list and single chapter
         list: https://212.32.226.234/manga/i-cant-stand-it-ajumma/
         single: https://212.32.226.234/i-cant-stand-it-ajumma-chapter-20/
         """
         try:
             url = f"{self.base_url}/manga/doudesu?link={link}"
             response = get(url, timeout=15).json()
             return dumps(response, indent=2)
         except Exception as e:
             return f"An error occured report on @YBotsSupport\n\n{e}"
 
+    def crotpedia(self, link: str):
+        """works with list chapter
+        list: https://38.242.194.12/baca/series/young-housemaid/
+        """
+        try:
+            url = f"{self.base_url}/manga/crotpedia?link={link}"
+            response = get(url, timeout=15).json()
+            return dumps(response, indent=2)
+        except Exception as e:
+            return f"An error occured report on @YBotsSupport\n\n{e}"
+
     def wibusubs(self, link: str):
         """work with single post link (may bug sometimes)
         https://www.wibusubs.moe/2023/03/brother-trap-2023-09-tamat-subtitle.html
         """
         try:
             url = f"{self.base_url}/drama/wibusubs?link={link}"
             response = get(url, timeout=5).json()
@@ -175,14 +209,22 @@
         try:
             url = f"{self.base_url}/music/sukidesuost?link={link}"
             response = get(url, timeout=15).json()
             return dumps(response, indent=2)
         except Exception as e:
             return f"An error occured report on @YBotsSupport\n\n{e}"
 
+    def hikarinoakari(self, link: str):
+        try:
+            url = f"{self.base_url}/music/hikarinoakari?link={link}"
+            response = get(url, timeout=15).json()
+            return dumps(response, indent=2)
+        except Exception as e:
+            return f"An error occured report on @YBotsSupport\n\n{e}"
+
     def google(self, query: str):
         try:
             url = f"{self.base_url}/google/search?query={query}"
             response = get(url, timeout=15).json()
             return dumps(response, indent=2)
         except Exception as e:
             return f"An error occured report on @YBotsSupport\n\n{e}"
@@ -319,22 +361,14 @@
         try:
             url = f"{self.base_url}/etc/ud?query={query}"
             response = get(url, timeout=15).json()
             return dumps(response, indent=2)
         except Exception as e:
             return f"An error occured report on @YBotsSupport\n\n{e}"
 
-    def wall(self, query: str):
-        try:
-            url = f"{self.base_url}/etc/wallhd?query={query}"
-            response = get(url, timeout=15).json()
-            return dumps(response, indent=2)
-        except Exception as e:
-            return f"An error occured report on @YBotsSupport\n\n{e}"
-
     def youtube(self, url: str):
         """tested on youtube video link, other not tested yet
         https://www.youtube.com/watch?v=a1V0UbBNliM
         """
         try:
             url = f"{self.base_url}/etc/youtube?url={url}"
             response = get(url, timeout=15).json()
```

### Comparing `wibuapi-0.1.1/wibuapi/zyxdevs.py` & `wibuapi-0.1.2/wibuapi/zyxdevs.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,13 +23,12 @@
     def xCode(self, url: str):
         """
         Personal site parser(lazy to make new repo) so i add this to here.
         https://xcodebasisdrive.blogspot.com
         """
         try:
             response = get(url)
-            parse = re.findall(
+            return re.findall(
                 "window.location[ ]{0,}=[ ]{0,}[(|\)](.*?)[(|\)]", response.text
             )[0].replace('"', "")
-            return parse
         except Exception as e:
             return f"An error occured report on @YBotsSupport\n\n{e}"
```

### Comparing `wibuapi-0.1.1/wibuapi.egg-info/PKG-INFO` & `wibuapi-0.1.2/wibuapi.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wibuapi
-Version: 0.1.1
+Version: 0.1.2
 Summary: Official Python Wrapper for Wibu API.
 Home-page: https://github.com/zYxDevs/wibu-api-py
 Author: Yoga Pranata
 Author-email: yoga@zyxdevs.eu.org
 License: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -34,46 +34,66 @@
 
 #### Get latest update
 ```
 pip3 install -U wibuapi
 ```
 
 #### Install from repo
-```bash
+```shell
 root@zyxdevs:~ git clone https://github.com/zYxDevs/wibu-api-py wibuapi
 root@zyxdevs:~ cd wibuapi
 root@zyxdevs:~ python3 setup.py install
 ```
 
 ## Telegram Bot:
-_I've created official telegram bot to interacted with WibuAPI_
+_There's many useful features in bot but it required big resource, so i make it for paid users only. If you interest to buy PM me on Telegram._
+
+**Paid Features:**
+
+- [x] LH Translation zipper
+- [x] Shinigami zipper
+- [x] Worldmanhwas zipper
+- [x] Maid Manga zipper
+- [x] Mangayaro zipper
+- [x] Cosmicscans zipper
+- [x] nHentai zipper
+- [x] Sheakomik, Sheamanga zipper
+- [x] Komikindo.info zipper
+- [x] Otomi Games
+  - [x] Search parser
+  - [x] Download link scrapper
+- [x] Javhd
+  - [x] Search parser
+  - [x] Download link scrapper
+- [x] Other incoming features
 
 [![WibuAPI Bot](https://img.shields.io/badge/WibuAPI-Bot-blue?&logo=telegram)](https://wibuapibot.t.me)
 [![Yoga Pranata](https://img.shields.io/badge/Yoga-Pranata-blue?&logo=telegram)](https://t.me/Yoga_CIC)
 [![Supoort Chat](https://img.shields.io/badge/Support-Chat-blue?&logo=telegram)](https://ybotssupport.t.me)
 [![Update Channel](https://img.shields.io/badge/Update-Channel-blue?&logo=telegram)](https://spreadnetworks.t.me)
 
 ## Examples:
 ### Importing modules
 ```python
 from wibuapi import WibuAPI
 api = WibuAPI()
 ```
 
 ### Anime, Hentai, Donghua
-_For nekopoi scrapper only works in [bot](https://t.me/wibuapibot)._
+_For nekopoi search only works in [bot](https://t.me/wibuapibot)._
 
 | Website | Params |
 | :-: | :-: |
 | [Lendrive](https://github.com/zYxDevs/wibu-api-py#lendrive)| link |
 | [Anichin](https://github.com/zYxDevs/wibu-api-py#anichin) | link |
 | [Donghua](https://github.com/zYxDevs/wibu-api-py#donghua) | link |
 | [Kusonime](https://github.com/zYxDevs/wibu-api-py#kusonime) | link |
 | [Doronime](https://github.com/zYxDevs/wibu-api-py#doronime) | link |
 | [Samehadaku](https://github.com/zYxDevs/wibu-api-py#samehadaku) | link |
+| [Nekopoi](https://github.com/zYxDevs/wibu-api-py#nekopoi) | link |
 
 #### [Lendrive](https://lendrive.web.id)
 ```python
 # works with batch, bd, and single eps link
 url = "https://lendrive.web.id/tondemo-skill-de-isekai-hourou-meshi-ep-04-dual-subs-x265-hevc-subtitle-indonesia-english/"
 res = api.lendrive(url)
 print(res)
@@ -99,41 +119,51 @@
 ```python
 # works with batch, bd, and single eps link
 url = "https://kusonime.com/isekai-ojisan-batch-subtitle-indonesia/"
 res = api.kusonime(url)
 print(res)
 ```
 
-#### [Doronime](https://doronime.id)
+#### [Doronime](https://doroni.me)
 ```python
 # works with batch, bd, and single eps link
-url = "https://doronime.id/anime/om-ke-isekai/batch"
+url = "https://doroni.me/anime/om-ke-isekai/batch"
 res = api.doronime(url)
 print(res)
 ```
 
 #### [Samehadaku](https://samehadaku.run)
 ```python
 # works with batch, bd, and single eps link
 url = "https://samehadaku.run/nierautomata-ver1-1a-episode-8/"
 res = api.samehadaku(url)
 print(res)
 ```
 
+#### [Nekopoi](https://nekopoi.care)
+```python
+# works with single eps link (hentai, jav)
+url = "https://nekopoi.care/koumi-jima-shuu-7-de-umeru-mesu-tachi-episode-1-subtitle-indonesia/"
+res = api.nekopoi(url)
+print(res)
+```
+
 ### Manga, Doujin, Manhua, Manhwa
 
 | Website | Params |
 | :-: | :-: |
 | [Rawkuma](https://github.com/zYxDevs/wibu-api-py#rawkuma) | link |
 | [Westmanga](https://github.com/zYxDevs/wibu-api-py#westmanga) | link |
 | [Komikindo](https://github.com/zYxDevs/wibu-api-py#komikindo) | link |
 | [Mangatale](https://github.com/zYxDevs/wibu-api-py#mangatale) | link |
 | [Kiryuu](https://github.com/zYxDevs/wibu-api-py#kiryuu) | link |
 | [Masterkomik](https://github.com/zYxDevs/wibu-api-py#masterkomik) | link |
+| [Mangakita](https://github.com/zYxDevs/wibu-api-py#mangakita) | link |
 | [Doujindesu](https://github.com/zYxDevs/wibu-api-py#doujindesu) | link |
+| [Crotpedia](https://github.com/zYxDevs/wibu-api-py#crotpedia) | link |
 
 #### [Rawkuma](https://rawkuma.com)
 ```python
 # works with list and single chapter
 # list: https://rawkuma.com/manga/guilty-circle/
 # single: https://rawkuma.com/guilty-circle-chapter-83/
 url = "https://rawkuma.com/manga/guilty-circle/"
@@ -187,32 +217,51 @@
 # list: https://masterkomik.com/manga/max-level-player/
 # single: https://masterkomik.com/max-level-player-chapter-07/
 url = "https://masterkomik.com/manga/max-level-player/"
 res = api.masterkomik(url)
 print(res)
 ```
 
+#### [Mangakita](https://mangakita.net)
+```python
+# works with list and single chapter
+# list: https://mangakita.net/manga/please-go-home-akutsu-san/
+# single: https://mangakita.net/please-go-home-akutsu-san-chapter-137/
+url = "https://mangakita.net/manga/please-go-home-akutsu-san/"
+res = api.mangakita(url)
+print(res)
+```
+
 #### [Doujindesu](https://212.32.226.234)
 ```python
 # works with list and single chapter
 # list: https://212.32.226.234/manga/i-cant-stand-it-ajumma/
 # single: https://212.32.226.234/i-cant-stand-it-ajumma-chapter-20/
 url = "https://212.32.226.234/manga/i-cant-stand-it-ajumma/"
 res = api.doujindesu(url)
 print(res)
 ```
 
+#### [Crotpedia](https://38.242.194.12)
+```python
+# works with list chapter
+# list: https://38.242.194.12/baca/series/young-housemaid/
+url = "https://38.242.194.12/baca/series/young-housemaid/"
+res = api.crotpedia(url)
+print(res)
+```
+
 **Note:**
 ```
 You can see more endpoints on https://wibu-api.eu.org/docs or wibuapi.py file.
-```
-```
+
 Sometimes their will change domains, that will make some endpoints wont works.
 Please let me know when their sites change domains, I will asap fix dead endpoints.
 
+If you find any bugs or requests a new sites,
 You can ping me on telegram or make new issue.
 ```
 
 ## Copyright:
 ```
 © 2022-2023 Yoga Pranata
 ```
```

