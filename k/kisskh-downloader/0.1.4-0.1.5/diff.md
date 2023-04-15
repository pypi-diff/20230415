# Comparing `tmp/kisskh-downloader-0.1.4.tar.gz` & `tmp/kisskh-downloader-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kisskh-downloader-0.1.4.tar", max compression
+gzip compressed data, was "kisskh-downloader-0.1.5.tar", max compression
```

## Comparing `kisskh-downloader-0.1.4.tar` & `kisskh-downloader-0.1.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     2080 2023-03-02 08:03:58.368296 kisskh-downloader-0.1.4/README.md
--rw-r--r--   0        0        0      901 2023-03-02 08:04:06.480209 kisskh-downloader-0.1.4/pyproject.toml
--rw-r--r--   0        0        0       22 2023-03-02 08:03:58.368296 kisskh-downloader-0.1.4/src/kisskh_downloader/__init__.py
--rw-r--r--   0        0        0     3480 2023-03-02 08:03:58.368296 kisskh-downloader-0.1.4/src/kisskh_downloader/cli.py
--rw-r--r--   0        0        0     1688 2023-03-02 08:03:58.368296 kisskh-downloader-0.1.4/src/kisskh_downloader/downloader.py
--rw-r--r--   0        0        0        0 2023-03-02 08:03:58.368296 kisskh-downloader-0.1.4/src/kisskh_downloader/enums/__init__.py
--rw-r--r--   0        0        0      134 2023-03-02 08:03:58.368296 kisskh-downloader-0.1.4/src/kisskh_downloader/enums/quality.py
--rw-r--r--   0        0        0     5246 2023-03-02 08:03:58.368296 kisskh-downloader-0.1.4/src/kisskh_downloader/kisskh_api.py
--rw-r--r--   0        0        0        0 2023-03-02 08:03:58.368296 kisskh-downloader-0.1.4/src/kisskh_downloader/models/__init__.py
--rw-r--r--   0        0        0     1289 2023-03-02 08:03:58.368296 kisskh-downloader-0.1.4/src/kisskh_downloader/models/drama.py
--rw-r--r--   0        0        0      555 2023-03-02 08:03:58.368296 kisskh-downloader-0.1.4/src/kisskh_downloader/models/search.py
--rw-r--r--   0        0        0      426 2023-03-02 08:03:58.368296 kisskh-downloader-0.1.4/src/kisskh_downloader/models/sub.py
--rw-r--r--   0        0        0     3150 2023-03-02 08:04:07.888818 kisskh-downloader-0.1.4/setup.py
--rw-r--r--   0        0        0     2733 2023-03-02 08:04:07.889211 kisskh-downloader-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     3422 2023-04-15 07:16:37.704767 kisskh-downloader-0.1.5/README.md
+-rw-r--r--   0        0        0      932 2023-04-15 07:16:47.992754 kisskh-downloader-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-04-15 07:16:37.704767 kisskh-downloader-0.1.5/src/kisskh_downloader/__init__.py
+-rw-r--r--   0        0        0     3554 2023-04-15 07:16:37.704767 kisskh-downloader-0.1.5/src/kisskh_downloader/cli.py
+-rw-r--r--   0        0        0     1688 2023-04-15 07:16:37.704767 kisskh-downloader-0.1.5/src/kisskh_downloader/downloader.py
+-rw-r--r--   0        0        0        0 2023-04-15 07:16:37.704767 kisskh-downloader-0.1.5/src/kisskh_downloader/enums/__init__.py
+-rw-r--r--   0        0        0      134 2023-04-15 07:16:37.704767 kisskh-downloader-0.1.5/src/kisskh_downloader/enums/quality.py
+-rw-r--r--   0        0        0     5246 2023-04-15 07:16:37.704767 kisskh-downloader-0.1.5/src/kisskh_downloader/kisskh_api.py
+-rw-r--r--   0        0        0        0 2023-04-15 07:16:37.704767 kisskh-downloader-0.1.5/src/kisskh_downloader/models/__init__.py
+-rw-r--r--   0        0        0     1289 2023-04-15 07:16:37.704767 kisskh-downloader-0.1.5/src/kisskh_downloader/models/drama.py
+-rw-r--r--   0        0        0      555 2023-04-15 07:16:37.704767 kisskh-downloader-0.1.5/src/kisskh_downloader/models/search.py
+-rw-r--r--   0        0        0      426 2023-04-15 07:16:37.704767 kisskh-downloader-0.1.5/src/kisskh_downloader/models/sub.py
+-rw-r--r--   0        0        0     4528 2023-04-15 07:16:49.484022 kisskh-downloader-0.1.5/setup.py
+-rw-r--r--   0        0        0     4075 2023-04-15 07:16:49.484481 kisskh-downloader-0.1.5/PKG-INFO
```

### Comparing `kisskh-downloader-0.1.4/pyproject.toml` & `kisskh-downloader-0.1.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "kisskh-downloader"
-version = "v0.1.4"
-description = "Simple downloaded for https://kisskh.me/"
+version = "v0.1.5"
+description = "Simple downloaded for https://kisskh.co/"
 readme = "README.md"
 authors = ["Debakar Roy <allinonedibakar@gmail.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 click = "^8.1.3"
 requests = "^2.28.2"
@@ -21,14 +21,15 @@
 flake8-bandit = "^4.1.1"
 flake8-comprehensions = "^3.10.1"
 flake8-isort = "^6.0.0"
 pep8-naming = "^0.13.3"
 pytest-cov = "^4.0.0"
 mypy = "^1.0.1"
 black = "^23.1.0"
+types-requests = "^2.28.11.15"
 
 [tool.black]
 line-length = 120
 
 [tool.poetry.scripts]
 kisskh = "kisskh_downloader.cli:kisskh"
```

### Comparing `kisskh-downloader-0.1.4/src/kisskh_downloader/cli.py` & `kisskh-downloader-0.1.5/src/kisskh_downloader/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 import re
 import sys
 from pathlib import Path
-from typing import List, Union
+from typing import Dict, List, Union
 from urllib.parse import parse_qs, urlparse
 
 import click
 import validators
 
 from kisskh_downloader.downloader import Downloader
 from kisskh_downloader.enums.quality import Quality
@@ -53,44 +53,44 @@
     last: int,
     quality: str,
     sub_langs: List[str],
     output_dir: Union[Path, str],
 ) -> None:
     logger = logging.getLogger(__name__)
     kisskh_api = KissKHApi()
-    downloader = Downloader(referer="https://kisskh.me")
-    episode_ids = []
+    downloader = Downloader(referer="https://kisskh.co")
+    episode_ids: Dict[int, int] = {}
     if validators.url(drama_url_or_name):
         parsed_url = urlparse(drama_url_or_name)
         ids = parse_qs(parsed_url.query).get("id")
         if ids is None:
             raise FileNotFoundError("Not a valid url for a drama!")
         drama_id = int(ids[0])
         episode_id = parse_qs(parsed_url.query).get("ep")
         episode_number = None
         if episode_string := re.search(r"Episode-(\d+)", parsed_url.path):
-            episode_number = int(episode_string.group(1))
+            episode_number = episode_string.group(1)
         if episode_id and episode_number:
-            episode_ids = {episode_number: episode_id[0]}
-        drama_name = parsed_url.path.split("/")[-1].replace("-", "_")
+            episode_ids = {int(episode_number): int(episode_id[0])}
+        drama_name = parsed_url.path.split("/")[2].replace("-", "_")
     else:
         drama = kisskh_api.get_drama_by_query(drama_url_or_name)
         if drama is None:
             logger.warning("No drama found with the query provided...")
             return None
         drama_id = drama.id
         drama_name = drama.title
 
     if not episode_ids:
         episode_ids = kisskh_api.get_episode_ids(drama_id=drama_id, start=first, stop=last)
 
-    for episode_number, episode_id in episode_ids.items():
+    for episode_number, episode_id in episode_ids.items():  # type: ignore
         logger.info(f"Getting details for Episode {episode_number}...")
-        video_stream_url = kisskh_api.get_stream_url(episode_id)
-        subtitles = kisskh_api.get_subtitles(episode_id, *sub_langs)
+        video_stream_url = kisskh_api.get_stream_url(episode_id)  # type: ignore
+        subtitles = kisskh_api.get_subtitles(episode_id, *sub_langs)  # type: ignore
         if "tickcounter" in video_stream_url:
             logger.warning(f"Episode {episode_number} still not released!")
             continue
 
         filepath = f"{output_dir}/{drama_name}/{drama_name}_E{episode_number:02d}"
         logger.debug(f"Using video url: {video_stream_url}")
         downloader.download_video_from_stream_url(video_stream_url, filepath, quality)
```

### Comparing `kisskh-downloader-0.1.4/src/kisskh_downloader/downloader.py` & `kisskh-downloader-0.1.5/src/kisskh_downloader/downloader.py`

 * *Files identical despite different names*

### Comparing `kisskh-downloader-0.1.4/src/kisskh_downloader/kisskh_api.py` & `kisskh-downloader-0.1.5/src/kisskh_downloader/kisskh_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from kisskh_downloader.models.sub import Sub, SubItem
 
 logger = logging.getLogger(__name__)
 
 
 class KissKHApi:
     def __init__(self):
-        self.base_url = "https://kisskh.me/api/"
+        self.base_url = "https://kisskh.co/api/"
         self.session = None
 
     def _drama_api_url(self, drama_id: int) -> str:
         """API endpoint for drama details
 
         :param drama_id: drama id
         :return: api url for a specific drama
```

### Comparing `kisskh-downloader-0.1.4/src/kisskh_downloader/models/drama.py` & `kisskh-downloader-0.1.5/src/kisskh_downloader/models/drama.py`

 * *Files identical despite different names*

### Comparing `kisskh-downloader-0.1.4/src/kisskh_downloader/models/search.py` & `kisskh-downloader-0.1.5/src/kisskh_downloader/models/search.py`

 * *Files identical despite different names*

### Comparing `kisskh-downloader-0.1.4/PKG-INFO` & `kisskh-downloader-0.1.5/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,171 +1,214 @@
-00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310a 4e61 6d65 3a20 6b69 7373  : 2.1.Name: kiss
-00000020: 6b68 2d64 6f77 6e6c 6f61 6465 720a 5665  kh-downloader.Ve
-00000030: 7273 696f 6e3a 2030 2e31 2e34 0a53 756d  rsion: 0.1.4.Sum
-00000040: 6d61 7279 3a20 5369 6d70 6c65 2064 6f77  mary: Simple dow
-00000050: 6e6c 6f61 6465 6420 666f 7220 6874 7470  nloaded for http
-00000060: 733a 2f2f 6b69 7373 6b68 2e6d 652f 0a41  s://kisskh.me/.A
-00000070: 7574 686f 723a 2044 6562 616b 6172 2052  uthor: Debakar R
-00000080: 6f79 0a41 7574 686f 722d 656d 6169 6c3a  oy.Author-email:
-00000090: 2061 6c6c 696e 6f6e 6564 6962 616b 6172   allinonedibakar
-000000a0: 4067 6d61 696c 2e63 6f6d 0a52 6571 7569  @gmail.com.Requi
-000000b0: 7265 732d 5079 7468 6f6e 3a20 3e3d 332e  res-Python: >=3.
-000000c0: 382c 3c34 2e30 0a43 6c61 7373 6966 6965  8,<4.0.Classifie
-000000d0: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
-000000e0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-000000f0: 6e20 3a3a 2033 0a43 6c61 7373 6966 6965  n :: 3.Classifie
-00000100: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
-00000110: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-00000120: 6e20 3a3a 2033 2e31 300a 436c 6173 7369  n :: 3.10.Classi
-00000130: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
-00000140: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-00000150: 7468 6f6e 203a 3a20 332e 380a 436c 6173  thon :: 3.8.Clas
-00000160: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
-00000170: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-00000180: 5079 7468 6f6e 203a 3a20 332e 390a 5265  Python :: 3.9.Re
-00000190: 7175 6972 6573 2d44 6973 743a 2063 6c69  quires-Dist: cli
-000001a0: 636b 2028 3e3d 382e 312e 332c 3c39 2e30  ck (>=8.1.3,<9.0
-000001b0: 2e30 290a 5265 7175 6972 6573 2d44 6973  .0).Requires-Dis
-000001c0: 743a 2070 7964 616e 7469 6320 283e 3d31  t: pydantic (>=1
-000001d0: 2e31 302e 352c 3c32 2e30 2e30 290a 5265  .10.5,<2.0.0).Re
-000001e0: 7175 6972 6573 2d44 6973 743a 2072 6571  quires-Dist: req
-000001f0: 7565 7374 7320 283e 3d32 2e32 382e 322c  uests (>=2.28.2,
-00000200: 3c33 2e30 2e30 290a 5265 7175 6972 6573  <3.0.0).Requires
-00000210: 2d44 6973 743a 2076 616c 6964 6174 6f72  -Dist: validator
-00000220: 7320 283e 3d30 2e32 302e 302c 3c30 2e32  s (>=0.20.0,<0.2
-00000230: 312e 3029 0a52 6571 7569 7265 732d 4469  1.0).Requires-Di
-00000240: 7374 3a20 7974 2d64 6c70 2028 3e3d 3230  st: yt-dlp (>=20
-00000250: 3233 2e32 2e31 372c 3c32 3032 342e 302e  23.2.17,<2024.0.
-00000260: 3029 0a44 6573 6372 6970 7469 6f6e 2d43  0).Description-C
-00000270: 6f6e 7465 6e74 2d54 7970 653a 2074 6578  ontent-Type: tex
-00000280: 742f 6d61 726b 646f 776e 0a0a 2320 3a74  t/markdown..# :t
-00000290: 763a 206b 6973 736b 682d 646c 0a0a 5369  v: kisskh-dl..Si
-000002a0: 6d70 6c65 2064 6f77 6e6c 6f61 6465 6420  mple downloaded 
-000002b0: 666f 7220 6874 7470 733a 2f2f 6b69 7373  for https://kiss
-000002c0: 6b68 2e6d 652f 0a0a 2d2d 2d0a 0a23 2320  kh.me/..---..## 
-000002d0: 3a69 6e62 6f78 5f74 7261 793a 2049 6e73  :inbox_tray: Ins
-000002e0: 7461 6c6c 6174 696f 6e0a 0a60 6060 636f  tallation..```co
-000002f0: 6e73 6f6c 650a 7069 7020 696e 7374 616c  nsole.pip instal
-00000300: 6c20 2d55 206b 6973 736b 682d 646f 776e  l -U kisskh-down
-00000310: 6c6f 6164 6572 0a60 6060 0a0a 2323 203a  loader.```..## :
-00000320: 626f 6f6b 733a 2055 7361 6765 0a0a 6060  books: Usage..``
-00000330: 6063 6f6e 736f 6c65 0a6b 6973 736b 6820  `console.kisskh 
-00000340: 646c 202d 2d68 656c 700a 5573 6167 653a  dl --help.Usage:
-00000350: 206b 6973 736b 6820 646c 205b 4f50 5449   kisskh dl [OPTI
-00000360: 4f4e 535d 2044 5241 4d41 5f55 524c 5f4f  ONS] DRAMA_URL_O
-00000370: 525f 4e41 4d45 0a0a 4f70 7469 6f6e 733a  R_NAME..Options:
-00000380: 0a20 202d 662c 202d 2d66 6972 7374 2049  .  -f, --first I
-00000390: 4e54 4547 4552 2020 2020 2020 2020 2020  NTEGER          
-000003a0: 2020 2053 7461 7274 696e 6720 6570 6973     Starting epis
-000003b0: 6f64 6520 6e75 6d62 6572 2e0a 2020 2d6c  ode number..  -l
-000003c0: 2c20 2d2d 6c61 7374 2049 4e54 4547 4552  , --last INTEGER
-000003d0: 2020 2020 2020 2020 2020 2020 2020 456e                En
-000003e0: 6469 6e67 2065 7069 736f 6465 206e 756d  ding episode num
-000003f0: 6265 722e 0a20 202d 712c 202d 2d71 7561  ber..  -q, --qua
-00000400: 6c69 7479 205b 3336 3070 7c34 3830 707c  lity [360p|480p|
-00000410: 3534 3070 7c37 3230 707c 3130 3830 705d  540p|720p|1080p]
-00000420: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000440: 2020 2051 7561 6c69 7479 206f 6620 7468     Quality of th
-00000450: 6520 7669 6465 6f20 746f 2062 6520 646f  e video to be do
-00000460: 776e 6c6f 6164 6564 2e0a 2020 2d73 2c20  wnloaded..  -s, 
-00000470: 2d2d 7375 622d 6c61 6e67 7320 5445 5854  --sub-langs TEXT
-00000480: 2020 2020 2020 2020 2020 2020 4c61 6e67              Lang
-00000490: 7561 6765 7320 6f66 2074 6865 2073 7562  uages of the sub
-000004a0: 7469 746c 6573 2074 6f20 646f 776e 6c6f  titles to downlo
-000004b0: 6164 2e0a 2020 2d6f 2c20 2d2d 6f75 7470  ad..  -o, --outp
-000004c0: 7574 2d64 6972 2054 4558 5420 2020 2020  ut-dir TEXT     
-000004d0: 2020 2020 2020 4f75 7470 7574 2064 6972        Output dir
-000004e0: 6563 746f 7279 2077 6865 7265 2064 6f77  ectory where dow
-000004f0: 6e6c 6f61 6465 6420 6669 6c65 7320 7769  nloaded files wi
-00000500: 6c6c 0a20 2020 2020 2020 2020 2020 2020  ll.             
-00000510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000520: 2020 2020 2062 6520 7374 6f72 652e 0a20       be store.. 
-00000530: 202d 2d68 656c 7020 2020 2020 2020 2020   --help         
-00000540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000550: 2053 686f 7720 7468 6973 206d 6573 7361   Show this messa
-00000560: 6765 2061 6e64 2065 7869 742e 0a60 6060  ge and exit..```
-00000570: 0a0a 2323 2320 3a68 6967 685f 6272 6967  ..### :high_brig
-00000580: 6874 6e65 7373 3a20 4469 7265 6374 2064  htness: Direct d
-00000590: 6f77 6e6c 6f61 6420 656e 7469 7265 2073  ownload entire s
-000005a0: 6572 6965 7320 696e 2068 6967 6865 7374  eries in highest
-000005b0: 2071 7561 6c69 7479 2061 7661 696c 6162   quality availab
-000005c0: 6c65 0a0a 6060 6063 6f6e 736f 6c65 0a6b  le..```console.k
-000005d0: 6973 736b 6820 646c 2022 6874 7470 733a  isskh dl "https:
-000005e0: 2f2f 6b69 7373 6b68 2e6d 652f 4472 616d  //kisskh.me/Dram
-000005f0: 612f 4d6f 6e65 792d 4865 6973 742d 2d4b  a/Money-Heist--K
-00000600: 6f72 6561 2d2d 2d4a 6f69 6e74 2d45 636f  orea---Joint-Eco
-00000610: 6e6f 6d69 632d 4172 6561 3f69 643d 3530  nomic-Area?id=50
-00000620: 3434 220a 6060 600a 0a23 2323 203a 6d61  44".```..### :ma
-00000630: 675f 7269 6768 743a 2053 6561 7263 6820  g_right: Search 
-00000640: 616e 6420 646f 776e 6c6f 6164 2065 6e74  and download ent
-00000650: 6972 6520 7365 7269 6573 2069 6e20 6869  ire series in hi
-00000660: 6768 6573 7420 7175 616c 6974 7920 6176  ghest quality av
-00000670: 6169 6c61 626c 650a 0a60 6060 636f 6e73  ailable..```cons
-00000680: 6f6c 650a 6b69 7373 6b68 2064 6c20 2253  ole.kisskh dl "S
-00000690: 7472 616e 6765 7220 5468 696e 6773 220a  tranger Things".
-000006a0: 312e 2053 7472 616e 6765 7220 5468 696e  1. Stranger Thin
-000006b0: 6773 202d 2053 6561 736f 6e20 340a 322e  gs - Season 4.2.
-000006c0: 2053 7472 616e 6765 7220 5468 696e 6773   Stranger Things
-000006d0: 202d 2053 6561 736f 6e20 310a 332e 2053   - Season 1.3. S
-000006e0: 7472 616e 6765 7220 5468 696e 6773 202d  tranger Things -
-000006f0: 2053 6561 736f 6e20 320a 342e 2053 7472   Season 2.4. Str
-00000700: 616e 6765 7220 5468 696e 6773 202d 2053  anger Things - S
-00000710: 6561 736f 6e20 330a 506c 6561 7365 2073  eason 3.Please s
-00000720: 656c 6563 7420 6f6e 6520 6672 6f6d 2061  elect one from a
-00000730: 626f 7665 3a20 310a 6060 600a 0a23 2323  bove: 1.```..###
-00000740: 203a 6172 726f 775f 666f 7277 6172 643a   :arrow_forward:
-00000750: 2044 6f77 6e6c 6f61 6420 7370 6563 6966   Download specif
-00000760: 6963 2065 7069 736f 6465 7320 7769 7468  ic episodes with
-00000770: 2073 7065 6369 6669 6320 7175 616c 6974   specific qualit
-00000780: 790a 0a3e 203a 6578 636c 616d 6174 696f  y..> :exclamatio
-00000790: 6e3a 204e 6f74 6520 7468 6174 2069 6620  n: Note that if 
-000007a0: 7468 6520 7365 6c65 6374 6564 2071 7561  the selected qua
-000007b0: 6c69 7479 2069 7320 6e6f 7420 6176 6169  lity is not avai
-000007c0: 6c61 626c 652c 2069 7420 7769 6c6c 2074  lable, it will t
-000007d0: 7279 2074 6f20 6765 7420 736f 6d65 7468  ry to get someth
-000007e0: 696e 6720 6c6f 7765 7220 7468 616e 2074  ing lower than t
-000007f0: 6861 7420 7175 616c 6974 792e 2049 6620  hat quality. If 
-00000800: 7468 6174 2061 6c73 6f20 6973 206e 6f74  that also is not
-00000810: 2061 7661 696c 6162 6c65 2c20 6974 2077   available, it w
-00000820: 696c 6c20 7472 7920 746f 2067 6574 2074  ill try to get t
-00000830: 6865 2062 6573 7420 7175 616c 6974 7920  he best quality 
-00000840: 6176 6169 6c61 626c 652e 0a0a 446f 776e  available...Down
-00000850: 6c6f 6164 7320 6570 6973 6f64 6520 3420  loads episode 4 
-00000860: 746f 2038 206f 6620 6041 6c63 6865 6d79  to 8 of `Alchemy
-00000870: 206f 6620 536f 756c 7360 2069 6e20 3732   of Souls` in 72
-00000880: 3070 3a0a 6060 6063 6f6e 736f 6c65 0a6b  0p:.```console.k
-00000890: 6973 736b 6820 646c 2022 6874 7470 733a  isskh dl "https:
-000008a0: 2f2f 6b69 7373 6b68 2e6d 652f 4472 616d  //kisskh.me/Dram
-000008b0: 612f 416c 6368 656d 792d 6f66 2d53 6f75  a/Alchemy-of-Sou
-000008c0: 6c73 3f69 643d 3530 3433 2220 2d66 2034  ls?id=5043" -f 4
-000008d0: 202d 6c20 3820 2d71 2037 3230 700a 6060   -l 8 -q 720p.``
-000008e0: 600a 0a44 6f77 6e6c 6f61 6473 2065 7069  `..Downloads epi
-000008f0: 736f 6465 2033 206f 6620 6041 2042 7573  sode 3 of `A Bus
-00000900: 696e 6573 7320 5072 6f70 6f73 616c 6020  iness Proposal` 
-00000910: 696e 2037 3230 703a 0a60 6060 636f 6e73  in 720p:.```cons
-00000920: 6f6c 650a 6b69 7373 6b68 2064 6c20 2268  ole.kisskh dl "h
-00000930: 7474 7073 3a2f 2f6b 6973 736b 682e 6d65  ttps://kisskh.me
-00000940: 2f44 7261 6d61 2f41 2d42 7573 696e 6573  /Drama/A-Busines
-00000950: 732d 5072 6f70 6f73 616c 3f69 643d 3436  s-Proposal?id=46
-00000960: 3038 2220 2d66 2033 202d 6c20 3320 2d71  08" -f 3 -l 3 -q
-00000970: 2037 3230 700a 6060 600a 0a2d 2d2d 0a0a   720p.```..---..
-00000980: 2320 3a62 6565 746c 653a 2044 4542 5547  # :beetle: DEBUG
-00000990: 0a0a 5573 6520 2d76 7620 666c 6167 2077  ..Use -vv flag w
-000009a0: 6869 6c65 2072 756e 6e69 6e67 2060 6b69  hile running `ki
-000009b0: 7373 6b68 2064 6c60 0a60 6060 636f 6e73  sskh dl`.```cons
-000009c0: 6f6c 650a 6b69 7373 6b68 202d 7676 2064  ole.kisskh -vv d
-000009d0: 6c20 2268 7474 7073 3a2f 2f6b 6973 736b  l "https://kissk
-000009e0: 682e 6d65 2f44 7261 6d61 2f41 2d42 7573  h.me/Drama/A-Bus
-000009f0: 696e 6573 732d 5072 6f70 6f73 616c 3f69  iness-Proposal?i
-00000a00: 643d 3436 3038 2220 2d66 2033 202d 6c20  d=4608" -f 3 -l 
-00000a10: 3320 2d71 2037 3230 700a 6060 600a 0a2d  3 -q 720p.```..-
-00000a20: 2d2d 0a0a 2320 3a63 6f6e 7374 7275 6374  --..# :construct
-00000a30: 696f 6e3a 2054 4f44 4f0a 2d20 5b20 5d20  ion: TODO.- [ ] 
-00000a40: 4164 6420 756e 6974 2074 6573 740a 2d20  Add unit test.- 
-00000a50: 5b20 5d20 4164 6420 6162 696c 6974 7920  [ ] Add ability 
-00000a60: 746f 2065 7870 6f72 7420 616c 6c20 646f  to export all do
-00000a70: 776e 6c6f 6164 206c 696e 6b0a 2d20 5b20  wnload link.- [ 
-00000a80: 5d20 4164 6420 6162 696c 6974 7920 746f  ] Add ability to
-00000a90: 206f 7065 6e20 7374 7265 616d 2069 6e20   open stream in 
-00000aa0: 736f 6d65 2070 6c61 7965 720a 0a         some player..
+00000000: 2320 3a74 763a 206b 6973 736b 682d 646c  # :tv: kisskh-dl
+00000010: 0a0a 3c64 6976 2061 6c69 676e 3d22 6365  ..<div align="ce
+00000020: 6e74 6572 223e 0a20 2020 3c69 6d67 2073  nter">.   <img s
+00000030: 7263 3d22 6874 7470 733a 2f2f 692e 696d  rc="https://i.im
+00000040: 6775 722e 636f 6d2f 6e68 5174 4f5a 612e  gur.com/nhQtOZa.
+00000050: 706e 6722 3e0a 2020 203c 6272 3e0a 2020  png">.   <br>.  
+00000060: 203c 7374 726f 6e67 3e3c 693e 5369 6d70   <strong><i>Simp
+00000070: 6c65 2064 6f77 6e6c 6f61 6465 6420 666f  le downloaded fo
+00000080: 7220 6874 7470 733a 2f2f 6b69 7373 6b68  r https://kisskh
+00000090: 2e63 6f2f 3c2f 693e 3c2f 7374 726f 6e67  .co/</i></strong
+000000a0: 3e0a 2020 203c 6272 3e0a 2020 203c 6120  >.   <br>.   <a 
+000000b0: 6872 6566 3d22 6874 7470 733a 2f2f 7079  href="https://py
+000000c0: 7069 2e6f 7267 2f70 726f 6a65 6374 2f6b  pi.org/project/k
+000000d0: 6973 736b 682d 646f 776e 6c6f 6164 6572  isskh-downloader
+000000e0: 2f22 3e0a 2020 203c 696d 6720 7372 633d  /">.   <img src=
+000000f0: 2268 7474 7073 3a2f 2f69 6d67 2e73 6869  "https://img.shi
+00000100: 656c 6473 2e69 6f2f 7079 7069 2f76 2f6b  elds.io/pypi/v/k
+00000110: 6973 736b 682d 646f 776e 6c6f 6164 6572  isskh-downloader
+00000120: 3f73 7479 6c65 3d66 6f72 2d74 6865 2d62  ?style=for-the-b
+00000130: 6164 6765 223e 0a20 2020 3c2f 613e 0a20  adge">.   </a>. 
+00000140: 2020 3c69 6d67 2073 7263 3d22 6874 7470    <img src="http
+00000150: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+00000160: 696f 2f67 6974 6875 622f 6163 7469 6f6e  io/github/action
+00000170: 732f 776f 726b 666c 6f77 2f73 7461 7475  s/workflow/statu
+00000180: 732f 4469 6261 6b61 7272 6f79 3139 3937  s/Dibakarroy1997
+00000190: 2f6b 6973 736b 682d 646c 2f70 756c 6c2d  /kisskh-dl/pull-
+000001a0: 7265 7175 6573 742e 796d 6c3f 7374 796c  request.yml?styl
+000001b0: 653d 666f 722d 7468 652d 6261 6467 6522  e=for-the-badge"
+000001c0: 3e0a 2020 203c 696d 6720 7372 633d 2268  >.   <img src="h
+000001d0: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+000001e0: 6473 2e69 6f2f 7079 7069 2f64 6d2f 6b69  ds.io/pypi/dm/ki
+000001f0: 7373 6b68 2d64 6f77 6e6c 6f61 6465 723f  sskh-downloader?
+00000200: 7374 796c 653d 666f 722d 7468 652d 6261  style=for-the-ba
+00000210: 6467 6522 3e0a 3c2f 6469 763e 0a0a 2d2d  dge">.</div>..--
+00000220: 2d0a 0af0 9f91 8b20 5765 6c63 6f6d 6520  -...... Welcome 
+00000230: 746f 2074 6865 206b 6973 736b 682d 646f  to the kisskh-do
+00000240: 776e 6c6f 6164 6572 2052 4541 444d 4521  wnloader README!
+00000250: 2054 6869 7320 7061 636b 6167 6520 6973   This package is
+00000260: 2061 2073 696d 706c 6520 636f 6d6d 616e   a simple comman
+00000270: 642d 6c69 6e65 2074 6f6f 6c20 666f 7220  d-line tool for 
+00000280: 646f 776e 6c6f 6164 696e 6720 7368 6f77  downloading show
+00000290: 7320 6672 6f6d 2068 7474 7073 3a2f 2f6b  s from https://k
+000002a0: 6973 736b 682e 636f 2f2e 2048 6572 6527  isskh.co/. Here'
+000002b0: 7320 6576 6572 7974 6869 6e67 2079 6f75  s everything you
+000002c0: 206e 6565 6420 746f 206b 6e6f 7720 746f   need to know to
+000002d0: 2067 6574 2073 7461 7274 6564 3a0a 0a23   get started:..#
+000002e0: 2320 f09f 92bb 2049 6e73 7461 6c6c 6174  # .... Installat
+000002f0: 696f 6e0a 0a54 6f20 696e 7374 616c 6c20  ion..To install 
+00000300: 6b69 7373 6b68 2d64 6f77 6e6c 6f61 6465  kisskh-downloade
+00000310: 722c 2073 696d 706c 7920 7275 6e20 7468  r, simply run th
+00000320: 6520 666f 6c6c 6f77 696e 6720 636f 6d6d  e following comm
+00000330: 616e 643a 0a0a 6060 6063 6f6e 736f 6c65  and:..```console
+00000340: 0a70 6970 2069 6e73 7461 6c6c 202d 5520  .pip install -U 
+00000350: 6b69 7373 6b68 2d64 6f77 6e6c 6f61 6465  kisskh-downloade
+00000360: 720a 6060 600a 0a23 2320 f09f 939a 2055  r.```..## .... U
+00000370: 7361 6765 0a0a 4166 7465 7220 696e 7374  sage..After inst
+00000380: 616c 6c69 6e67 2074 6865 2070 6163 6b61  alling the packa
+00000390: 6765 2c20 796f 7520 6361 6e20 7573 6520  ge, you can use 
+000003a0: 7468 6520 606b 6973 736b 6820 646c 6020  the `kisskh dl` 
+000003b0: 636f 6d6d 616e 6420 746f 2064 6f77 6e6c  command to downl
+000003c0: 6f61 6420 7368 6f77 7320 6672 6f6d 2074  oad shows from t
+000003d0: 6865 2063 6f6d 6d61 6e64 206c 696e 652e  he command line.
+000003e0: 0a0a 6060 6063 6f6e 736f 6c65 0a6b 6973  ..```console.kis
+000003f0: 736b 6820 646c 202d 2d68 656c 700a 5573  skh dl --help.Us
+00000400: 6167 653a 206b 6973 736b 6820 646c 205b  age: kisskh dl [
+00000410: 4f50 5449 4f4e 535d 2044 5241 4d41 5f55  OPTIONS] DRAMA_U
+00000420: 524c 5f4f 525f 4e41 4d45 0a0a 4f70 7469  RL_OR_NAME..Opti
+00000430: 6f6e 733a 0a20 202d 662c 202d 2d66 6972  ons:.  -f, --fir
+00000440: 7374 2049 4e54 4547 4552 2020 2020 2020  st INTEGER      
+00000450: 2020 2020 2020 2053 7461 7274 696e 6720         Starting 
+00000460: 6570 6973 6f64 6520 6e75 6d62 6572 2e0a  episode number..
+00000470: 2020 2d6c 2c20 2d2d 6c61 7374 2049 4e54    -l, --last INT
+00000480: 4547 4552 2020 2020 2020 2020 2020 2020  EGER            
+00000490: 2020 456e 6469 6e67 2065 7069 736f 6465    Ending episode
+000004a0: 206e 756d 6265 722e 0a20 202d 712c 202d   number..  -q, -
+000004b0: 2d71 7561 6c69 7479 205b 3336 3070 7c34  -quality [360p|4
+000004c0: 3830 707c 3534 3070 7c37 3230 707c 3130  80p|540p|720p|10
+000004d0: 3830 705d 0a20 2020 2020 2020 2020 2020  80p].           
+000004e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000004f0: 2020 2020 2020 2051 7561 6c69 7479 206f         Quality o
+00000500: 6620 7468 6520 7669 6465 6f20 746f 2062  f the video to b
+00000510: 6520 646f 776e 6c6f 6164 6564 2e0a 2020  e downloaded..  
+00000520: 2d73 2c20 2d2d 7375 622d 6c61 6e67 7320  -s, --sub-langs 
+00000530: 5445 5854 2020 2020 2020 2020 2020 2020  TEXT            
+00000540: 4c61 6e67 7561 6765 7320 6f66 2074 6865  Languages of the
+00000550: 2073 7562 7469 746c 6573 2074 6f20 646f   subtitles to do
+00000560: 776e 6c6f 6164 2e0a 2020 2d6f 2c20 2d2d  wnload..  -o, --
+00000570: 6f75 7470 7574 2d64 6972 2054 4558 5420  output-dir TEXT 
+00000580: 2020 2020 2020 2020 2020 4f75 7470 7574            Output
+00000590: 2064 6972 6563 746f 7279 2077 6865 7265   directory where
+000005a0: 2064 6f77 6e6c 6f61 6465 6420 6669 6c65   downloaded file
+000005b0: 7320 7769 6c6c 0a20 2020 2020 2020 2020  s will.         
+000005c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000005d0: 2020 2020 2020 2020 2062 6520 7374 6f72           be stor
+000005e0: 652e 0a20 202d 2d68 656c 7020 2020 2020  e..  --help     
+000005f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000600: 2020 2020 2053 686f 7720 7468 6973 206d       Show this m
+00000610: 6573 7361 6765 2061 6e64 2065 7869 742e  essage and exit.
+00000620: 0a60 6060 0a0a 4865 7265 2061 7265 2073  .```..Here are s
+00000630: 6f6d 6520 6578 616d 706c 6573 3a0a 0a23  ome examples:..#
+00000640: 2323 20f0 9f94 9720 4469 7265 6374 2064  ## .... Direct d
+00000650: 6f77 6e6c 6f61 6420 656e 7469 7265 2073  ownload entire s
+00000660: 6572 6965 7320 696e 2068 6967 6865 7374  eries in highest
+00000670: 2071 7561 6c69 7479 2061 7661 696c 6162   quality availab
+00000680: 6c65 2069 6e20 6375 7272 656e 7420 666f  le in current fo
+00000690: 6c64 6572 0a0a 6060 6063 6f6e 736f 6c65  lder..```console
+000006a0: 0a6b 6973 736b 6820 646c 2022 6874 7470  .kisskh dl "http
+000006b0: 733a 2f2f 6b69 7373 6b68 2e63 6f2f 4472  s://kisskh.co/Dr
+000006c0: 616d 612f 4973 6c61 6e64 2d53 6561 736f  ama/Island-Seaso
+000006d0: 6e2d 323f 6964 3d37 3030 3022 202d 6f20  n-2?id=7000" -o 
+000006e0: 2e0a 6060 600a 0a21 5b44 6f77 6e6c 6f61  ..```..![Downloa
+000006f0: 6420 616c 6c20 7573 696e 6720 5552 4c5d  d all using URL]
+00000700: 2868 7474 7073 3a2f 2f69 2e69 6d67 7572  (https://i.imgur
+00000710: 2e63 6f6d 2f63 764b 5971 4b33 2e67 6966  .com/cvKYqK3.gif
+00000720: 290a 0a0a 2323 2320 f09f 948d 2053 6561  )...### .... Sea
+00000730: 7263 6820 616e 6420 646f 776e 6c6f 6164  rch and download
+00000740: 2065 6e74 6972 6520 7365 7269 6573 2069   entire series i
+00000750: 6e20 6869 6768 6573 7420 7175 616c 6974  n highest qualit
+00000760: 7920 6176 6169 6c61 626c 6520 696e 2063  y available in c
+00000770: 7572 7265 6e74 2066 6f6c 6465 720a 0a60  urrent folder..`
+00000780: 6060 636f 6e73 6f6c 650a 6b69 7373 6b68  ``console.kisskh
+00000790: 2064 6c20 2253 7472 616e 6765 7220 5468   dl "Stranger Th
+000007a0: 696e 6773 2220 2d6f 202e 0a31 2e20 5374  ings" -o ..1. St
+000007b0: 7261 6e67 6572 2054 6869 6e67 7320 2d20  ranger Things - 
+000007c0: 5365 6173 6f6e 2034 0a32 2e20 5374 7261  Season 4.2. Stra
+000007d0: 6e67 6572 2054 6869 6e67 7320 2d20 5365  nger Things - Se
+000007e0: 6173 6f6e 2031 0a33 2e20 5374 7261 6e67  ason 1.3. Strang
+000007f0: 6572 2054 6869 6e67 7320 2d20 5365 6173  er Things - Seas
+00000800: 6f6e 2032 0a34 2e20 5374 7261 6e67 6572  on 2.4. Stranger
+00000810: 2054 6869 6e67 7320 2d20 5365 6173 6f6e   Things - Season
+00000820: 2033 0a50 6c65 6173 6520 7365 6c65 6374   3.Please select
+00000830: 206f 6e65 2066 726f 6d20 6162 6f76 653a   one from above:
+00000840: 2031 0a60 6060 0a0a 215b 446f 776e 6c6f   1.```..![Downlo
+00000850: 6164 2061 6c6c 2075 7369 6e67 2055 524c  ad all using URL
+00000860: 5d28 6874 7470 733a 2f2f 692e 696d 6775  ](https://i.imgu
+00000870: 722e 636f 6d2f 6d4c 5071 6a67 6a2e 6769  r.com/mLPqjgj.gi
+00000880: 6629 0a0a 2323 2320 e2ac 87ef b88f 2044  f)..### ...... D
+00000890: 6f77 6e6c 6f61 6420 7370 6563 6966 6963  ownload specific
+000008a0: 2065 7069 736f 6465 7320 7769 7468 2073   episodes with s
+000008b0: 7065 6369 6669 6320 7175 616c 6974 790a  pecific quality.
+000008c0: 0a3e 203a 6578 636c 616d 6174 696f 6e3a  .> :exclamation:
+000008d0: 204e 6f74 6520 7468 6174 2069 6620 7468   Note that if th
+000008e0: 6520 7365 6c65 6374 6564 2071 7561 6c69  e selected quali
+000008f0: 7479 2069 7320 6e6f 7420 6176 6169 6c61  ty is not availa
+00000900: 626c 652c 2069 7420 7769 6c6c 2074 7279  ble, it will try
+00000910: 2074 6f20 6765 7420 736f 6d65 7468 696e   to get somethin
+00000920: 6720 6c6f 7765 7220 7468 616e 2074 6861  g lower than tha
+00000930: 7420 7175 616c 6974 792e 2049 6620 7468  t quality. If th
+00000940: 6174 2061 6c73 6f20 6973 206e 6f74 2061  at also is not a
+00000950: 7661 696c 6162 6c65 2c20 6974 2077 696c  vailable, it wil
+00000960: 6c20 7472 7920 746f 2067 6574 2074 6865  l try to get the
+00000970: 2062 6573 7420 7175 616c 6974 7920 6176   best quality av
+00000980: 6169 6c61 626c 652e 0a0a 446f 776e 6c6f  ailable...Downlo
+00000990: 6164 7320 6570 6973 6f64 6520 3420 746f  ads episode 4 to
+000009a0: 2038 206f 6620 6041 6c63 6865 6d79 206f   8 of `Alchemy o
+000009b0: 6620 536f 756c 7360 2069 6e20 3732 3070  f Souls` in 720p
+000009c0: 3a0a 6060 6063 6f6e 736f 6c65 0a6b 6973  :.```console.kis
+000009d0: 736b 6820 646c 2022 6874 7470 733a 2f2f  skh dl "https://
+000009e0: 6b69 7373 6b68 2e63 6f2f 4472 616d 612f  kisskh.co/Drama/
+000009f0: 416c 6368 656d 792d 6f66 2d53 6f75 6c73  Alchemy-of-Souls
+00000a00: 3f69 643d 3530 3433 2220 2d66 2034 202d  ?id=5043" -f 4 -
+00000a10: 6c20 3820 2d71 2037 3230 7020 2d6f 202e  l 8 -q 720p -o .
+00000a20: 0a60 6060 0a0a 215b 446f 776e 6c6f 6164  .```..![Download
+00000a30: 2072 616e 6765 206f 6620 6570 6973 6f64   range of episod
+00000a40: 6573 5d28 6874 7470 733a 2f2f 692e 696d  es](https://i.im
+00000a50: 6775 722e 636f 6d2f 5136 3639 3770 612e  gur.com/Q6697pa.
+00000a60: 6769 6629 0a0a 446f 776e 6c6f 6164 7320  gif)..Downloads 
+00000a70: 6570 6973 6f64 6520 3320 6f66 2060 4120  episode 3 of `A 
+00000a80: 4275 7369 6e65 7373 2050 726f 706f 7361  Business Proposa
+00000a90: 6c60 2069 6e20 3732 3070 3a0a 6060 6063  l` in 720p:.```c
+00000aa0: 6f6e 736f 6c65 0a6b 6973 736b 6820 646c  onsole.kisskh dl
+00000ab0: 2022 6874 7470 733a 2f2f 6b69 7373 6b68   "https://kisskh
+00000ac0: 2e63 6f2f 4472 616d 612f 412d 4275 7369  .co/Drama/A-Busi
+00000ad0: 6e65 7373 2d50 726f 706f 7361 6c3f 6964  ness-Proposal?id
+00000ae0: 3d34 3630 3822 202d 6620 3320 2d6c 2033  =4608" -f 3 -l 3
+00000af0: 202d 7120 3732 3070 202d 6f20 2e0a 6060   -q 720p -o ..``
+00000b00: 600a 0a21 5b44 6f77 6e6c 6f61 6420 7369  `..![Download si
+00000b10: 6e67 6c65 2065 7069 736f 6465 5d28 6874  ngle episode](ht
+00000b20: 7470 733a 2f2f 692e 696d 6775 722e 636f  tps://i.imgur.co
+00000b30: 6d2f 634e 6c45 4438 6d2e 6769 6629 0a0a  m/cNlED8m.gif)..
+00000b40: 596f 7520 6361 6e20 616c 736f 2064 6f77  You can also dow
+00000b50: 6c6f 6164 2073 696e 676c 6520 6570 6973  load single epis
+00000b60: 6f64 6520 6279 2070 726f 7669 6469 6e67  ode by providing
+00000b70: 2074 6865 2065 7069 736f 6465 2055 524c   the episode URL
+00000b80: 0a0a 6060 6063 6f6e 736f 6c65 0a6b 6973  ..```console.kis
+00000b90: 736b 6820 646c 2022 6874 7470 733a 2f2f  skh dl "https://
+00000ba0: 6b69 7373 6b68 2e63 6f2f 4472 616d 612f  kisskh.co/Drama/
+00000bb0: 412d 4275 7369 6e65 7373 2d50 726f 706f  A-Business-Propo
+00000bc0: 7361 6c2f 4570 6973 6f64 652d 333f 6964  sal/Episode-3?id
+00000bd0: 3d34 3630 3826 6570 3d38 3634 3339 2670  =4608&ep=86439&p
+00000be0: 6167 653d 3026 7061 6765 5369 7a65 3d31  age=0&pageSize=1
+00000bf0: 3030 2220 2d6f 202e 0a60 6060 0a0a 466f  00" -o ..```..Fo
+00000c00: 7220 6d6f 7265 206f 7074 696f 6e73 2c20  r more options, 
+00000c10: 7573 6520 7468 6520 602d 2d68 656c 7060  use the `--help`
+00000c20: 2066 6c61 672e 0a0a 2d2d 2d0a 0a23 20f0   flag...---..# .
+00000c30: 9f90 9e20 4445 4255 470a 0a54 6f20 656e  ... DEBUG..To en
+00000c40: 6162 6c65 2064 6562 7567 6769 6e67 2c20  able debugging, 
+00000c50: 7573 6520 7468 6520 602d 7676 6020 666c  use the `-vv` fl
+00000c60: 6167 2077 6869 6c65 2072 756e 6e69 6e67  ag while running
+00000c70: 2060 6b69 7373 6b68 2064 6c60 2e0a 0a60   `kisskh dl`...`
+00000c80: 6060 636f 6e73 6f6c 650a 6b69 7373 6b68  ``console.kisskh
+00000c90: 202d 7676 2064 6c20 2268 7474 7073 3a2f   -vv dl "https:/
+00000ca0: 2f6b 6973 736b 682e 636f 2f44 7261 6d61  /kisskh.co/Drama
+00000cb0: 2f41 2d42 7573 696e 6573 732d 5072 6f70  /A-Business-Prop
+00000cc0: 6f73 616c 3f69 643d 3436 3038 2220 2d66  osal?id=4608" -f
+00000cd0: 2033 202d 6c20 3320 2d71 2037 3230 700a   3 -l 3 -q 720p.
+00000ce0: 6060 600a 0a2d 2d2d 0a0a 2320 3a63 6f6e  ```..---..# :con
+00000cf0: 7374 7275 6374 696f 6e3a 2054 4f44 4f0a  struction: TODO.
+00000d00: 2d20 5b20 5d20 4164 6420 6162 696c 6974  - [ ] Add abilit
+00000d10: 7920 746f 2065 7870 6f72 7420 616c 6c20  y to export all 
+00000d20: 646f 776e 6c6f 6164 206c 696e 6b0a 2d20  download link.- 
+00000d30: 5b20 5d20 4164 6420 6162 696c 6974 7920  [ ] Add ability 
+00000d40: 746f 206f 7065 6e20 7374 7265 616d 2069  to open stream i
+00000d50: 6e20 736f 6d65 2070 6c61 7965 720a       n some player.
```

