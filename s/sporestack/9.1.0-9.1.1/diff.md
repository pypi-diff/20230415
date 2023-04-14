# Comparing `tmp/sporestack-9.1.0.tar.gz` & `tmp/sporestack-9.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sporestack-9.1.0.tar", last modified: Wed Mar 29 01:51:06 2023, max compression
+gzip compressed data, was "sporestack-9.1.1.tar", last modified: Wed Apr 12 00:36:08 2023, max compression
```

## Comparing `sporestack-9.1.0.tar` & `sporestack-9.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      167 2023-03-29 01:51:06.000000 sporestack-9.1.0/.editorconfig
--rw-r--r--   0        0        0       81 2023-03-29 01:51:06.000000 sporestack-9.1.0/.gitignore
--rw-r--r--   0        0        0     1338 2023-03-29 01:51:06.000000 sporestack-9.1.0/.woodpecker.yml
--rw-r--r--   0        0        0     4252 2023-03-29 01:51:06.000000 sporestack-9.1.0/CHANGELOG.md
--rw-r--r--   0        0        0     1211 2023-03-29 01:51:06.000000 sporestack-9.1.0/LICENSE.txt
--rw-r--r--   0        0        0      579 2023-03-29 01:51:06.000000 sporestack-9.1.0/Makefile
--rw-r--r--   0        0        0      468 2023-03-29 01:51:06.000000 sporestack-9.1.0/Pipfile
--rw-r--r--   0        0        0    48157 2023-03-29 01:51:06.000000 sporestack-9.1.0/Pipfile.lock
--rw-r--r--   0        0        0     1615 2023-03-29 01:51:06.000000 sporestack-9.1.0/README.md
--rw-r--r--   0        0        0     1557 2023-03-29 01:51:06.000000 sporestack-9.1.0/pyproject.toml
--rw-r--r--   0        0        0      144 2023-03-29 01:51:06.000000 sporestack-9.1.0/src/sporestack/__init__.py
--rw-r--r--   0        0        0     3905 2023-03-29 01:51:06.000000 sporestack-9.1.0/src/sporestack/api.py
--rw-r--r--   0        0        0    10776 2023-03-29 01:51:06.000000 sporestack-9.1.0/src/sporestack/api_client.py
--rw-r--r--   0        0        0    24812 2023-03-29 01:51:06.000000 sporestack-9.1.0/src/sporestack/cli.py
--rw-r--r--   0        0        0     4453 2023-03-29 01:51:06.000000 sporestack-9.1.0/src/sporestack/client.py
--rw-r--r--   0        0        0      195 2023-03-29 01:51:06.000000 sporestack-9.1.0/src/sporestack/exceptions.py
--rw-r--r--   0        0        0      719 2023-03-29 01:51:06.000000 sporestack-9.1.0/src/sporestack/models.py
--rw-r--r--   0        0        0        0 2023-03-29 01:51:06.000000 sporestack-9.1.0/src/sporestack/py.typed
--rw-r--r--   0        0        0      711 2023-03-29 01:51:06.000000 sporestack-9.1.0/src/sporestack/utils.py
--rw-r--r--   0        0        0        0 2023-03-29 01:51:06.000000 sporestack-9.1.0/tests/__init__.py
--rw-r--r--   0        0        0      732 2023-03-29 01:51:06.000000 sporestack-9.1.0/tests/test_api_client.py
--rw-r--r--   0        0        0     2120 2023-03-29 01:51:06.000000 sporestack-9.1.0/tests/test_cli.py
--rw-r--r--   0        0        0      520 2023-03-29 01:51:06.000000 sporestack-9.1.0/tests/test_utils.py
--rw-r--r--   0        0        0     2218 1970-01-01 00:00:00.000000 sporestack-9.1.0/PKG-INFO
+-rw-r--r--   0        0        0      167 2023-04-12 00:36:08.000000 sporestack-9.1.1/.editorconfig
+-rw-r--r--   0        0        0       81 2023-04-12 00:36:08.000000 sporestack-9.1.1/.gitignore
+-rw-r--r--   0        0        0     1338 2023-04-12 00:36:08.000000 sporestack-9.1.1/.woodpecker.yml
+-rw-r--r--   0        0        0     4331 2023-04-12 00:36:08.000000 sporestack-9.1.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1211 2023-04-12 00:36:08.000000 sporestack-9.1.1/LICENSE.txt
+-rw-r--r--   0        0        0      579 2023-04-12 00:36:08.000000 sporestack-9.1.1/Makefile
+-rw-r--r--   0        0        0      484 2023-04-12 00:36:08.000000 sporestack-9.1.1/Pipfile
+-rw-r--r--   0        0        0    46235 2023-04-12 00:36:08.000000 sporestack-9.1.1/Pipfile.lock
+-rw-r--r--   0        0        0     1615 2023-04-12 00:36:08.000000 sporestack-9.1.1/README.md
+-rw-r--r--   0        0        0     1557 2023-04-12 00:36:08.000000 sporestack-9.1.1/pyproject.toml
+-rw-r--r--   0        0        0      144 2023-04-12 00:36:08.000000 sporestack-9.1.1/src/sporestack/__init__.py
+-rw-r--r--   0        0        0     3905 2023-04-12 00:36:08.000000 sporestack-9.1.1/src/sporestack/api.py
+-rw-r--r--   0        0        0    10776 2023-04-12 00:36:08.000000 sporestack-9.1.1/src/sporestack/api_client.py
+-rw-r--r--   0        0        0    24815 2023-04-12 00:36:08.000000 sporestack-9.1.1/src/sporestack/cli.py
+-rw-r--r--   0        0        0     4523 2023-04-12 00:36:08.000000 sporestack-9.1.1/src/sporestack/client.py
+-rw-r--r--   0        0        0      195 2023-04-12 00:36:08.000000 sporestack-9.1.1/src/sporestack/exceptions.py
+-rw-r--r--   0        0        0      719 2023-04-12 00:36:08.000000 sporestack-9.1.1/src/sporestack/models.py
+-rw-r--r--   0        0        0        0 2023-04-12 00:36:08.000000 sporestack-9.1.1/src/sporestack/py.typed
+-rw-r--r--   0        0        0      711 2023-04-12 00:36:08.000000 sporestack-9.1.1/src/sporestack/utils.py
+-rw-r--r--   0        0        0        0 2023-04-12 00:36:08.000000 sporestack-9.1.1/tests/__init__.py
+-rw-r--r--   0        0        0      732 2023-04-12 00:36:08.000000 sporestack-9.1.1/tests/test_api_client.py
+-rw-r--r--   0        0        0     2120 2023-04-12 00:36:08.000000 sporestack-9.1.1/tests/test_cli.py
+-rw-r--r--   0        0        0      520 2023-04-12 00:36:08.000000 sporestack-9.1.1/tests/test_utils.py
+-rw-r--r--   0        0        0     2218 1970-01-01 00:00:00.000000 sporestack-9.1.1/PKG-INFO
```

### Comparing `sporestack-9.1.0/.woodpecker.yml` & `sporestack-9.1.1/.woodpecker.yml`

 * *Files identical despite different names*

### Comparing `sporestack-9.1.0/CHANGELOG.md` & `sporestack-9.1.1/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,20 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [9.1.1 - 2023-04-12]
+
+### Changed
+
+- Bug fix with `default_factory` issue.
+
 ## [9.1.0 - 2023-03-28]
 
 ### Added
 
 - Token messages support.
 - `deleted_at` field in Server Info respones.
```

### Comparing `sporestack-9.1.0/LICENSE.txt` & `sporestack-9.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sporestack-9.1.0/Makefile` & `sporestack-9.1.1/Makefile`

 * *Files identical despite different names*

### Comparing `sporestack-9.1.0/Pipfile.lock` & `sporestack-9.1.1/Pipfile.lock`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9174435028248588%*

 * *Differences: {"'_meta'": "{'hash': {'sha256': "*

 * *            "'ad9d790601f514743ccca149f2c41fce3db8493e9386372bb8416af64a06eebf'}}",*

 * * "'default'": "{'httpcore': {'hashes': "*

 * *              "['sha256:0fdfea45e94f0c9fd96eab9286077f9ff788dd186635ae61b312693e4d943599', "*

 * *              "'sha256:cc045a3241afbf60ce056202301b4d8b6af08845e3294055eb26b09913ef903c'], "*

 * *              "'version': '==0.17.0'}, 'httpx': {'hashes': "*

 * *              "['sha256:447556b50c1921c351ea54b4fe79d91b724ed2b027462ab9a329465d147d5a4e', "*

 * *             […]*

```diff
@@ -1,11 +1,11 @@
 {
     "_meta": {
         "hash": {
-            "sha256": "bd2a497c6cec1a778bb49921a6aeb2eb4d6300ec949621d570bc3841850aafab"
+            "sha256": "ad9d790601f514743ccca149f2c41fce3db8493e9386372bb8416af64a06eebf"
         },
         "pipfile-spec": 6,
         "requires": {},
         "sources": [
             {
                 "name": "pypi",
                 "url": "https://pypi.org/simple",
@@ -44,90 +44,80 @@
                 "sha256:e3fe4ac4b851c468cc8363d500db52c2ead036020723024a109d37346efaa761"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==0.14.0"
         },
         "httpcore": {
             "hashes": [
-                "sha256:c5d6f04e2fc530f39e0c077e6a30caa53f1451096120f1f38b954afd0b17c0cb",
-                "sha256:da1fb708784a938aa084bde4feb8317056c55037247c787bd7e19eb2c2949dc0"
+                "sha256:0fdfea45e94f0c9fd96eab9286077f9ff788dd186635ae61b312693e4d943599",
+                "sha256:cc045a3241afbf60ce056202301b4d8b6af08845e3294055eb26b09913ef903c"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==0.16.3"
+            "version": "==0.17.0"
         },
         "httpx": {
             "extras": [
                 "socks"
             ],
             "hashes": [
-                "sha256:9818458eb565bb54898ccb9b8b251a28785dd4a55afbc23d0eb410754fe7d0f9",
-                "sha256:a211fcce9b1254ea24f0cd6af9869b3d29aba40154e947d2a07bb499b3e310d6"
+                "sha256:447556b50c1921c351ea54b4fe79d91b724ed2b027462ab9a329465d147d5a4e",
+                "sha256:507d676fc3e26110d41df7d35ebd8b3b8585052450f4097401c9be59d928c63e"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==0.23.3"
+            "version": "==0.24.0"
         },
         "idna": {
             "hashes": [
                 "sha256:814f528e8dead7d329833b91c5faa87d60bf71824cd12a7530b5526063d02cb4",
                 "sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2"
             ],
             "markers": "python_version >= '3.5'",
             "version": "==3.4"
         },
         "pydantic": {
             "hashes": [
-                "sha256:05a81b006be15655b2a1bae5faa4280cf7c81d0e09fcb49b342ebf826abe5a72",
-                "sha256:0b53e1d41e97063d51a02821b80538053ee4608b9a181c1005441f1673c55423",
-                "sha256:2b3ce5f16deb45c472dde1a0ee05619298c864a20cded09c4edd820e1454129f",
-                "sha256:2e82a6d37a95e0b1b42b82ab340ada3963aea1317fd7f888bb6b9dfbf4fff57c",
-                "sha256:301d626a59edbe5dfb48fcae245896379a450d04baeed50ef40d8199f2733b06",
-                "sha256:39f4a73e5342b25c2959529f07f026ef58147249f9b7431e1ba8414a36761f53",
-                "sha256:4948f264678c703f3877d1c8877c4e3b2e12e549c57795107f08cf70c6ec7774",
-                "sha256:4b05697738e7d2040696b0a66d9f0a10bec0efa1883ca75ee9e55baf511909d6",
-                "sha256:51bdeb10d2db0f288e71d49c9cefa609bca271720ecd0c58009bd7504a0c464c",
-                "sha256:55b1625899acd33229c4352ce0ae54038529b412bd51c4915349b49ca575258f",
-                "sha256:572066051eeac73d23f95ba9a71349c42a3e05999d0ee1572b7860235b850cc6",
-                "sha256:6a05a9db1ef5be0fe63e988f9617ca2551013f55000289c671f71ec16f4985e3",
-                "sha256:6dc1cc241440ed7ca9ab59d9929075445da6b7c94ced281b3dd4cfe6c8cff817",
-                "sha256:6e7124d6855b2780611d9f5e1e145e86667eaa3bd9459192c8dc1a097f5e9903",
-                "sha256:75d52162fe6b2b55964fbb0af2ee58e99791a3138588c482572bb6087953113a",
-                "sha256:78cec42b95dbb500a1f7120bdf95c401f6abb616bbe8785ef09887306792e66e",
-                "sha256:7feb6a2d401f4d6863050f58325b8d99c1e56f4512d98b11ac64ad1751dc647d",
-                "sha256:8775d4ef5e7299a2f4699501077a0defdaac5b6c4321173bcb0f3c496fbadf85",
-                "sha256:887ca463c3bc47103c123bc06919c86720e80e1214aab79e9b779cda0ff92a00",
-                "sha256:9193d4f4ee8feca58bc56c8306bcb820f5c7905fd919e0750acdeeeef0615b28",
-                "sha256:983e720704431a6573d626b00662eb78a07148c9115129f9b4351091ec95ecc3",
-                "sha256:990406d226dea0e8f25f643b370224771878142155b879784ce89f633541a024",
-                "sha256:9cbdc268a62d9a98c56e2452d6c41c0263d64a2009aac69246486f01b4f594c4",
-                "sha256:a48f1953c4a1d9bd0b5167ac50da9a79f6072c63c4cef4cf2a3736994903583e",
-                "sha256:a9a6747cac06c2beb466064dda999a13176b23535e4c496c9d48e6406f92d42d",
-                "sha256:a9f2de23bec87ff306aef658384b02aa7c32389766af3c5dee9ce33e80222dfa",
-                "sha256:b5635de53e6686fe7a44b5cf25fcc419a0d5e5c1a1efe73d49d48fe7586db854",
-                "sha256:b6f9d649892a6f54a39ed56b8dfd5e08b5f3be5f893da430bed76975f3735d15",
-                "sha256:b9a3859f24eb4e097502a3be1fb4b2abb79b6103dd9e2e0edb70613a4459a648",
-                "sha256:cd8702c5142afda03dc2b1ee6bc358b62b3735b2cce53fc77b31ca9f728e4bc8",
-                "sha256:d7b5a3821225f5c43496c324b0d6875fde910a1c2933d726a743ce328fbb2a8c",
-                "sha256:d88c4c0e5c5dfd05092a4b271282ef0588e5f4aaf345778056fc5259ba098857",
-                "sha256:eb992a1ef739cc7b543576337bebfc62c0e6567434e522e97291b251a41dad7f",
-                "sha256:f2f7eb6273dd12472d7f218e1fef6f7c7c2f00ac2e1ecde4db8824c457300416",
-                "sha256:fdf88ab63c3ee282c76d652fc86518aacb737ff35796023fae56a65ced1a5978",
-                "sha256:fdf8d759ef326962b4678d89e275ffc55b7ce59d917d9f72233762061fd04a2d"
+                "sha256:01aea3a42c13f2602b7ecbbea484a98169fb568ebd9e247593ea05f01b884b2e",
+                "sha256:0cd181f1d0b1d00e2b705f1bf1ac7799a2d938cce3376b8007df62b29be3c2c6",
+                "sha256:10a86d8c8db68086f1e30a530f7d5f83eb0685e632e411dbbcf2d5c0150e8dcd",
+                "sha256:193924c563fae6ddcb71d3f06fa153866423ac1b793a47936656e806b64e24ca",
+                "sha256:464855a7ff7f2cc2cf537ecc421291b9132aa9c79aef44e917ad711b4a93163b",
+                "sha256:516f1ed9bc2406a0467dd777afc636c7091d71f214d5e413d64fef45174cfc7a",
+                "sha256:6434b49c0b03a51021ade5c4daa7d70c98f7a79e95b551201fff682fc1661245",
+                "sha256:64d34ab766fa056df49013bb6e79921a0265204c071984e75a09cbceacbbdd5d",
+                "sha256:670bb4683ad1e48b0ecb06f0cfe2178dcf74ff27921cdf1606e527d2617a81ee",
+                "sha256:68792151e174a4aa9e9fc1b4e653e65a354a2fa0fed169f7b3d09902ad2cb6f1",
+                "sha256:701daea9ffe9d26f97b52f1d157e0d4121644f0fcf80b443248434958fd03dc3",
+                "sha256:7d45fc99d64af9aaf7e308054a0067fdcd87ffe974f2442312372dfa66e1001d",
+                "sha256:80b1fab4deb08a8292d15e43a6edccdffa5377a36a4597bb545b93e79c5ff0a5",
+                "sha256:82dffb306dd20bd5268fd6379bc4bfe75242a9c2b79fec58e1041fbbdb1f7914",
+                "sha256:8c7f51861d73e8b9ddcb9916ae7ac39fb52761d9ea0df41128e81e2ba42886cd",
+                "sha256:950ce33857841f9a337ce07ddf46bc84e1c4946d2a3bba18f8280297157a3fd1",
+                "sha256:976cae77ba6a49d80f461fd8bba183ff7ba79f44aa5cfa82f1346b5626542f8e",
+                "sha256:9f6f0fd68d73257ad6685419478c5aece46432f4bdd8d32c7345f1986496171e",
+                "sha256:a7cd2251439988b413cb0a985c4ed82b6c6aac382dbaff53ae03c4b23a70e80a",
+                "sha256:abfb7d4a7cd5cc4e1d1887c43503a7c5dd608eadf8bc615413fc498d3e4645cd",
+                "sha256:ae150a63564929c675d7f2303008d88426a0add46efd76c3fc797cd71cb1b46f",
+                "sha256:b0f85904f73161817b80781cc150f8b906d521fa11e3cdabae19a581c3606209",
+                "sha256:b4a849d10f211389502059c33332e91327bc154acc1845f375a99eca3afa802d",
+                "sha256:c15582f9055fbc1bfe50266a19771bbbef33dd28c45e78afbe1996fd70966c2a",
+                "sha256:c230c0d8a322276d6e7b88c3f7ce885f9ed16e0910354510e0bae84d54991143",
+                "sha256:cc1dde4e50a5fc1336ee0581c1612215bc64ed6d28d2c7c6f25d2fe3e7c3e918",
+                "sha256:cf135c46099ff3f919d2150a948ce94b9ce545598ef2c6c7bf55dca98a304b52",
+                "sha256:cfc83c0678b6ba51b0532bea66860617c4cd4251ecf76e9846fa5a9f3454e97e",
+                "sha256:d2a5ebb48958754d386195fe9e9c5106f11275867051bf017a8059410e9abf1f",
+                "sha256:d71e69699498b020ea198468e2480a2f1e7433e32a3a99760058c6520e2bea7e",
+                "sha256:d75ae19d2a3dbb146b6f324031c24f8a3f52ff5d6a9f22f0683694b3afcb16fb",
+                "sha256:dfe2507b8ef209da71b6fb5f4e597b50c5a34b78d7e857c4f8f3115effaef5fe",
+                "sha256:e0cfe895a504c060e5d36b287ee696e2fdad02d89e0d895f83037245218a87fe",
+                "sha256:e79e999e539872e903767c417c897e729e015872040e56b96e67968c3b918b2d",
+                "sha256:ecbbc51391248116c0a055899e6c3e7ffbb11fb5e2a4cd6f2d0b93272118a209",
+                "sha256:f4a2b50e2b03d5776e7f21af73e2070e1b5c0d0df255a827e7c632962f8315af"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==1.10.4"
-        },
-        "rfc3986": {
-            "extras": [
-                "idna2008"
-            ],
-            "hashes": [
-                "sha256:270aaf10d87d0d4e095063c65bf3ddbc6ee3d0b226328ce21e036f946e421835",
-                "sha256:a86d6e1f5b1dc238b218b012df0aa79409667bb209e58da56d0b94704e712a97"
-            ],
-            "version": "==1.5.0"
+            "version": "==1.10.7"
         },
         "segno": {
             "hashes": [
                 "sha256:983424b296e62189d70fc73460cd946cf56dcbe82b9bda18c066fc1b24371cdc",
                 "sha256:b17ace8171aad3987e01bb4aeadf7e0450c40674024c4c57b4da54028e55f1e9"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
@@ -158,310 +148,273 @@
                 "sha256:ff797846578a9f2a201b53442aedeb543319466870fbe1c701eab66dd7681165"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==0.7.0"
         },
         "typing-extensions": {
             "hashes": [
-                "sha256:1511434bb92bf8dd198c12b1cc812e800d4181cfcb867674e0f8279cc93087aa",
-                "sha256:16fa4864408f655d35ec496218b85f79b3437c829e93320c7c9215ccfd92489e"
+                "sha256:5cb5f4a79139d699607b3ef622a1dedafa84e115ab0024e0d9c044a9479ca7cb",
+                "sha256:fb33085c39dd998ac16d1431ebc293a8b3eedd00fd4a32de0ff79002c19511b4"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==4.4.0"
+            "version": "==4.5.0"
         }
     },
     "develop": {
         "almost-make": {
             "hashes": [
                 "sha256:5d22b5668a0addbb90abae520be0127aec4d733fb6d7ca5953bd820b4a8ae54b",
                 "sha256:de75234582d934131f1f4b3641c30a577568d0a184353e22af195afd6ed99567"
             ],
             "index": "pypi",
             "version": "==0.5.2"
         },
-        "astunparse": {
-            "hashes": [
-                "sha256:5ad93a8456f0d084c3456d059fd9a92cce667963232cbf763eac3bc5b7940872",
-                "sha256:c2652417f2c8b5bb325c885ae329bdf3f86424075c4fd1a128674bc6fba4b8e8"
-            ],
-            "markers": "python_version < '3.9'",
-            "version": "==1.6.3"
-        },
-        "attrs": {
-            "hashes": [
-                "sha256:29e95c7f6778868dbd49170f98f8818f78f3dc5e0e37c0b1f474e3561b240836",
-                "sha256:c9227bfc2f01993c03f68db37d1d15c9690188323c067c641f1a35ca58185f99"
-            ],
-            "markers": "python_version >= '3.6'",
-            "version": "==22.2.0"
-        },
         "black": {
             "hashes": [
-                "sha256:0052dba51dec07ed029ed61b18183942043e00008ec65d5028814afaab9a22fd",
-                "sha256:0680d4380db3719ebcfb2613f34e86c8e6d15ffeabcf8ec59355c5e7b85bb555",
-                "sha256:121ca7f10b4a01fd99951234abdbd97728e1240be89fde18480ffac16503d481",
-                "sha256:162e37d49e93bd6eb6f1afc3e17a3d23a823042530c37c3c42eeeaf026f38468",
-                "sha256:2a951cc83ab535d248c89f300eccbd625e80ab880fbcfb5ac8afb5f01a258ac9",
-                "sha256:2bf649fda611c8550ca9d7592b69f0637218c2369b7744694c5e4902873b2f3a",
-                "sha256:382998821f58e5c8238d3166c492139573325287820963d2f7de4d518bd76958",
-                "sha256:49f7b39e30f326a34b5c9a4213213a6b221d7ae9d58ec70df1c4a307cf2a1580",
-                "sha256:57c18c5165c1dbe291d5306e53fb3988122890e57bd9b3dcb75f967f13411a26",
-                "sha256:7a0f701d314cfa0896b9001df70a530eb2472babb76086344e688829efd97d32",
-                "sha256:8178318cb74f98bc571eef19068f6ab5613b3e59d4f47771582f04e175570ed8",
-                "sha256:8b70eb40a78dfac24842458476135f9b99ab952dd3f2dab738c1881a9b38b753",
-                "sha256:9880d7d419bb7e709b37e28deb5e68a49227713b623c72b2b931028ea65f619b",
-                "sha256:9afd3f493666a0cd8f8df9a0200c6359ac53940cbde049dcb1a7eb6ee2dd7074",
-                "sha256:a29650759a6a0944e7cca036674655c2f0f63806ddecc45ed40b7b8aa314b651",
-                "sha256:a436e7881d33acaf2536c46a454bb964a50eff59b21b51c6ccf5a40601fbef24",
-                "sha256:a59db0a2094d2259c554676403fa2fac3473ccf1354c1c63eccf7ae65aac8ab6",
-                "sha256:a8471939da5e824b891b25751955be52ee7f8a30a916d570a5ba8e0f2eb2ecad",
-                "sha256:b0bd97bea8903f5a2ba7219257a44e3f1f9d00073d6cc1add68f0beec69692ac",
-                "sha256:b6a92a41ee34b883b359998f0c8e6eb8e99803aa8bf3123bf2b2e6fec505a221",
-                "sha256:bb460c8561c8c1bec7824ecbc3ce085eb50005883a6203dcfb0122e95797ee06",
-                "sha256:bfffba28dc52a58f04492181392ee380e95262af14ee01d4bc7bb1b1c6ca8d27",
-                "sha256:c1c476bc7b7d021321e7d93dc2cbd78ce103b84d5a4cf97ed535fbc0d6660648",
-                "sha256:c91dfc2c2a4e50df0026f88d2215e166616e0c80e86004d0003ece0488db2739",
-                "sha256:e6663f91b6feca5d06f2ccd49a10f254f9298cc1f7f49c46e498a0771b507104"
+                "sha256:064101748afa12ad2291c2b91c960be28b817c0c7eaa35bec09cc63aa56493c5",
+                "sha256:0945e13506be58bf7db93ee5853243eb368ace1c08a24c65ce108986eac65915",
+                "sha256:11c410f71b876f961d1de77b9699ad19f939094c3a677323f43d7a29855fe326",
+                "sha256:1c7b8d606e728a41ea1ccbd7264677e494e87cf630e399262ced92d4a8dac940",
+                "sha256:1d06691f1eb8de91cd1b322f21e3bfc9efe0c7ca1f0e1eb1db44ea367dff656b",
+                "sha256:3238f2aacf827d18d26db07524e44741233ae09a584273aa059066d644ca7b30",
+                "sha256:32daa9783106c28815d05b724238e30718f34155653d4d6e125dc7daec8e260c",
+                "sha256:35d1381d7a22cc5b2be2f72c7dfdae4072a3336060635718cc7e1ede24221d6c",
+                "sha256:3a150542a204124ed00683f0db1f5cf1c2aaaa9cc3495b7a3b5976fb136090ab",
+                "sha256:48f9d345675bb7fbc3dd85821b12487e1b9a75242028adad0333ce36ed2a6d27",
+                "sha256:50cb33cac881766a5cd9913e10ff75b1e8eb71babf4c7104f2e9c52da1fb7de2",
+                "sha256:562bd3a70495facf56814293149e51aa1be9931567474993c7942ff7d3533961",
+                "sha256:67de8d0c209eb5b330cce2469503de11bca4085880d62f1628bd9972cc3366b9",
+                "sha256:6b39abdfb402002b8a7d030ccc85cf5afff64ee90fa4c5aebc531e3ad0175ddb",
+                "sha256:6f3c333ea1dd6771b2d3777482429864f8e258899f6ff05826c3a4fcc5ce3f70",
+                "sha256:714290490c18fb0126baa0fca0a54ee795f7502b44177e1ce7624ba1c00f2331",
+                "sha256:7c3eb7cea23904399866c55826b31c1f55bbcd3890ce22ff70466b907b6775c2",
+                "sha256:92c543f6854c28a3c7f39f4d9b7694f9a6eb9d3c5e2ece488c327b6e7ea9b266",
+                "sha256:a6f6886c9869d4daae2d1715ce34a19bbc4b95006d20ed785ca00fa03cba312d",
+                "sha256:a8a968125d0a6a404842fa1bf0b349a568634f856aa08ffaff40ae0dfa52e7c6",
+                "sha256:c7ab5790333c448903c4b721b59c0d80b11fe5e9803d8703e84dcb8da56fec1b",
+                "sha256:e114420bf26b90d4b9daa597351337762b63039752bdf72bf361364c1aa05925",
+                "sha256:e198cf27888ad6f4ff331ca1c48ffc038848ea9f031a3b40ba36aced7e22f2c8",
+                "sha256:ec751418022185b0c1bb7d7736e6933d40bbb14c14a0abcf9123d1b159f98dd4",
+                "sha256:f0bd2f4a58d6666500542b26354978218a9babcdc972722f4bf90779524515f3"
             ],
             "index": "pypi",
-            "version": "==23.1.0"
+            "version": "==23.3.0"
         },
         "bleach": {
             "hashes": [
                 "sha256:1a1a85c1595e07d8db14c5f09f09e6433502c51c595970edc090551f0db99414",
                 "sha256:33c16e3353dbd13028ab4799a0f89a83f113405c766e9c122df8a06f5b85b3f4"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==6.0.0"
         },
         "build": {
             "hashes": [
-                "sha256:1aaadcd69338252ade4f7ec1265e1a19184bf916d84c9b7df095f423948cb89f",
-                "sha256:21b7ebbd1b22499c4dac536abc7606696ea4d909fd755e00f09f3c0f2c05e3c8"
+                "sha256:af266720050a66c893a6096a2f410989eeac74ff9a68ba194b3f6473e8e26171",
+                "sha256:d5b71264afdb5951d6704482aac78de887c80691c52b88a9ad195983ca2c9269"
             ],
             "index": "pypi",
-            "version": "==0.7.0"
+            "version": "==0.10.0"
         },
         "certifi": {
             "hashes": [
                 "sha256:35824b4c3a97115964b408844d64aa14db1cc518f6562e8d7261699d1350a9e3",
                 "sha256:4ad3232f5e926d6718ec31cfc1fcadfde020920e278684144551c91769c7bc18"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==2022.12.7"
         },
         "charset-normalizer": {
             "hashes": [
-                "sha256:00d3ffdaafe92a5dc603cb9bd5111aaa36dfa187c8285c543be562e61b755f6b",
-                "sha256:024e606be3ed92216e2b6952ed859d86b4cfa52cd5bc5f050e7dc28f9b43ec42",
-                "sha256:0298eafff88c99982a4cf66ba2efa1128e4ddaca0b05eec4c456bbc7db691d8d",
-                "sha256:02a51034802cbf38db3f89c66fb5d2ec57e6fe7ef2f4a44d070a593c3688667b",
-                "sha256:083c8d17153ecb403e5e1eb76a7ef4babfc2c48d58899c98fcaa04833e7a2f9a",
-                "sha256:0a11e971ed097d24c534c037d298ad32c6ce81a45736d31e0ff0ad37ab437d59",
-                "sha256:0bf2dae5291758b6f84cf923bfaa285632816007db0330002fa1de38bfcb7154",
-                "sha256:0c0a590235ccd933d9892c627dec5bc7511ce6ad6c1011fdf5b11363022746c1",
-                "sha256:0f438ae3532723fb6ead77e7c604be7c8374094ef4ee2c5e03a3a17f1fca256c",
-                "sha256:109487860ef6a328f3eec66f2bf78b0b72400280d8f8ea05f69c51644ba6521a",
-                "sha256:11b53acf2411c3b09e6af37e4b9005cba376c872503c8f28218c7243582df45d",
-                "sha256:12db3b2c533c23ab812c2b25934f60383361f8a376ae272665f8e48b88e8e1c6",
-                "sha256:14e76c0f23218b8f46c4d87018ca2e441535aed3632ca134b10239dfb6dadd6b",
-                "sha256:16a8663d6e281208d78806dbe14ee9903715361cf81f6d4309944e4d1e59ac5b",
-                "sha256:292d5e8ba896bbfd6334b096e34bffb56161c81408d6d036a7dfa6929cff8783",
-                "sha256:2c03cc56021a4bd59be889c2b9257dae13bf55041a3372d3295416f86b295fb5",
-                "sha256:2e396d70bc4ef5325b72b593a72c8979999aa52fb8bcf03f701c1b03e1166918",
-                "sha256:2edb64ee7bf1ed524a1da60cdcd2e1f6e2b4f66ef7c077680739f1641f62f555",
-                "sha256:31a9ddf4718d10ae04d9b18801bd776693487cbb57d74cc3458a7673f6f34639",
-                "sha256:356541bf4381fa35856dafa6a965916e54bed415ad8a24ee6de6e37deccf2786",
-                "sha256:358a7c4cb8ba9b46c453b1dd8d9e431452d5249072e4f56cfda3149f6ab1405e",
-                "sha256:37f8febc8ec50c14f3ec9637505f28e58d4f66752207ea177c1d67df25da5aed",
-                "sha256:39049da0ffb96c8cbb65cbf5c5f3ca3168990adf3551bd1dee10c48fce8ae820",
-                "sha256:39cf9ed17fe3b1bc81f33c9ceb6ce67683ee7526e65fde1447c772afc54a1bb8",
-                "sha256:3ae1de54a77dc0d6d5fcf623290af4266412a7c4be0b1ff7444394f03f5c54e3",
-                "sha256:3b590df687e3c5ee0deef9fc8c547d81986d9a1b56073d82de008744452d6541",
-                "sha256:3e45867f1f2ab0711d60c6c71746ac53537f1684baa699f4f668d4c6f6ce8e14",
-                "sha256:3fc1c4a2ffd64890aebdb3f97e1278b0cc72579a08ca4de8cd2c04799a3a22be",
-                "sha256:4457ea6774b5611f4bed5eaa5df55f70abde42364d498c5134b7ef4c6958e20e",
-                "sha256:44ba614de5361b3e5278e1241fda3dc1838deed864b50a10d7ce92983797fa76",
-                "sha256:4a8fcf28c05c1f6d7e177a9a46a1c52798bfe2ad80681d275b10dcf317deaf0b",
-                "sha256:4b0d02d7102dd0f997580b51edc4cebcf2ab6397a7edf89f1c73b586c614272c",
-                "sha256:502218f52498a36d6bf5ea77081844017bf7982cdbe521ad85e64cabee1b608b",
-                "sha256:503e65837c71b875ecdd733877d852adbc465bd82c768a067badd953bf1bc5a3",
-                "sha256:5995f0164fa7df59db4746112fec3f49c461dd6b31b841873443bdb077c13cfc",
-                "sha256:59e5686dd847347e55dffcc191a96622f016bc0ad89105e24c14e0d6305acbc6",
-                "sha256:601f36512f9e28f029d9481bdaf8e89e5148ac5d89cffd3b05cd533eeb423b59",
-                "sha256:608862a7bf6957f2333fc54ab4399e405baad0163dc9f8d99cb236816db169d4",
-                "sha256:62595ab75873d50d57323a91dd03e6966eb79c41fa834b7a1661ed043b2d404d",
-                "sha256:70990b9c51340e4044cfc394a81f614f3f90d41397104d226f21e66de668730d",
-                "sha256:71140351489970dfe5e60fc621ada3e0f41104a5eddaca47a7acb3c1b851d6d3",
-                "sha256:72966d1b297c741541ca8cf1223ff262a6febe52481af742036a0b296e35fa5a",
-                "sha256:74292fc76c905c0ef095fe11e188a32ebd03bc38f3f3e9bcb85e4e6db177b7ea",
-                "sha256:761e8904c07ad053d285670f36dd94e1b6ab7f16ce62b9805c475b7aa1cffde6",
-                "sha256:772b87914ff1152b92a197ef4ea40efe27a378606c39446ded52c8f80f79702e",
-                "sha256:79909e27e8e4fcc9db4addea88aa63f6423ebb171db091fb4373e3312cb6d603",
-                "sha256:7e189e2e1d3ed2f4aebabd2d5b0f931e883676e51c7624826e0a4e5fe8a0bf24",
-                "sha256:7eb33a30d75562222b64f569c642ff3dc6689e09adda43a082208397f016c39a",
-                "sha256:81d6741ab457d14fdedc215516665050f3822d3e56508921cc7239f8c8e66a58",
-                "sha256:8499ca8f4502af841f68135133d8258f7b32a53a1d594aa98cc52013fff55678",
-                "sha256:84c3990934bae40ea69a82034912ffe5a62c60bbf6ec5bc9691419641d7d5c9a",
-                "sha256:87701167f2a5c930b403e9756fab1d31d4d4da52856143b609e30a1ce7160f3c",
-                "sha256:88600c72ef7587fe1708fd242b385b6ed4b8904976d5da0893e31df8b3480cb6",
-                "sha256:8ac7b6a045b814cf0c47f3623d21ebd88b3e8cf216a14790b455ea7ff0135d18",
-                "sha256:8b8af03d2e37866d023ad0ddea594edefc31e827fee64f8de5611a1dbc373174",
-                "sha256:8c7fe7afa480e3e82eed58e0ca89f751cd14d767638e2550c77a92a9e749c317",
-                "sha256:8eade758719add78ec36dc13201483f8e9b5d940329285edcd5f70c0a9edbd7f",
-                "sha256:911d8a40b2bef5b8bbae2e36a0b103f142ac53557ab421dc16ac4aafee6f53dc",
-                "sha256:93ad6d87ac18e2a90b0fe89df7c65263b9a99a0eb98f0a3d2e079f12a0735837",
-                "sha256:95dea361dd73757c6f1c0a1480ac499952c16ac83f7f5f4f84f0658a01b8ef41",
-                "sha256:9ab77acb98eba3fd2a85cd160851816bfce6871d944d885febf012713f06659c",
-                "sha256:9cb3032517f1627cc012dbc80a8ec976ae76d93ea2b5feaa9d2a5b8882597579",
-                "sha256:9cf4e8ad252f7c38dd1f676b46514f92dc0ebeb0db5552f5f403509705e24753",
-                "sha256:9d9153257a3f70d5f69edf2325357251ed20f772b12e593f3b3377b5f78e7ef8",
-                "sha256:a152f5f33d64a6be73f1d30c9cc82dfc73cec6477ec268e7c6e4c7d23c2d2291",
-                "sha256:a16418ecf1329f71df119e8a65f3aa68004a3f9383821edcb20f0702934d8087",
-                "sha256:a60332922359f920193b1d4826953c507a877b523b2395ad7bc716ddd386d866",
-                "sha256:a8d0fc946c784ff7f7c3742310cc8a57c5c6dc31631269876a88b809dbeff3d3",
-                "sha256:ab5de034a886f616a5668aa5d098af2b5385ed70142090e2a31bcbd0af0fdb3d",
-                "sha256:c22d3fe05ce11d3671297dc8973267daa0f938b93ec716e12e0f6dee81591dc1",
-                "sha256:c2ac1b08635a8cd4e0cbeaf6f5e922085908d48eb05d44c5ae9eabab148512ca",
-                "sha256:c512accbd6ff0270939b9ac214b84fb5ada5f0409c44298361b2f5e13f9aed9e",
-                "sha256:c75ffc45f25324e68ab238cb4b5c0a38cd1c3d7f1fb1f72b5541de469e2247db",
-                "sha256:c95a03c79bbe30eec3ec2b7f076074f4281526724c8685a42872974ef4d36b72",
-                "sha256:cadaeaba78750d58d3cc6ac4d1fd867da6fc73c88156b7a3212a3cd4819d679d",
-                "sha256:cd6056167405314a4dc3c173943f11249fa0f1b204f8b51ed4bde1a9cd1834dc",
-                "sha256:db72b07027db150f468fbada4d85b3b2729a3db39178abf5c543b784c1254539",
-                "sha256:df2c707231459e8a4028eabcd3cfc827befd635b3ef72eada84ab13b52e1574d",
-                "sha256:e62164b50f84e20601c1ff8eb55620d2ad25fb81b59e3cd776a1902527a788af",
-                "sha256:e696f0dd336161fca9adbb846875d40752e6eba585843c768935ba5c9960722b",
-                "sha256:eaa379fcd227ca235d04152ca6704c7cb55564116f8bc52545ff357628e10602",
-                "sha256:ebea339af930f8ca5d7a699b921106c6e29c617fe9606fa7baa043c1cdae326f",
-                "sha256:f4c39b0e3eac288fedc2b43055cfc2ca7a60362d0e5e87a637beac5d801ef478",
-                "sha256:f5057856d21e7586765171eac8b9fc3f7d44ef39425f85dbcccb13b3ebea806c",
-                "sha256:f6f45710b4459401609ebebdbcfb34515da4fc2aa886f95107f556ac69a9147e",
-                "sha256:f97e83fa6c25693c7a35de154681fcc257c1c41b38beb0304b9c4d2d9e164479",
-                "sha256:f9d0c5c045a3ca9bedfc35dca8526798eb91a07aa7a2c0fee134c6c6f321cbd7",
-                "sha256:ff6f3db31555657f3163b15a6b7c6938d08df7adbfc9dd13d9d19edad678f1e8"
+                "sha256:04afa6387e2b282cf78ff3dbce20f0cc071c12dc8f685bd40960cc68644cfea6",
+                "sha256:04eefcee095f58eaabe6dc3cc2262f3bcd776d2c67005880894f447b3f2cb9c1",
+                "sha256:0be65ccf618c1e7ac9b849c315cc2e8a8751d9cfdaa43027d4f6624bd587ab7e",
+                "sha256:0c95f12b74681e9ae127728f7e5409cbbef9cd914d5896ef238cc779b8152373",
+                "sha256:0ca564606d2caafb0abe6d1b5311c2649e8071eb241b2d64e75a0d0065107e62",
+                "sha256:10c93628d7497c81686e8e5e557aafa78f230cd9e77dd0c40032ef90c18f2230",
+                "sha256:11d117e6c63e8f495412d37e7dc2e2fff09c34b2d09dbe2bee3c6229577818be",
+                "sha256:11d3bcb7be35e7b1bba2c23beedac81ee893ac9871d0ba79effc7fc01167db6c",
+                "sha256:12a2b561af122e3d94cdb97fe6fb2bb2b82cef0cdca131646fdb940a1eda04f0",
+                "sha256:12d1a39aa6b8c6f6248bb54550efcc1c38ce0d8096a146638fd4738e42284448",
+                "sha256:1435ae15108b1cb6fffbcea2af3d468683b7afed0169ad718451f8db5d1aff6f",
+                "sha256:1c60b9c202d00052183c9be85e5eaf18a4ada0a47d188a83c8f5c5b23252f649",
+                "sha256:1e8fcdd8f672a1c4fc8d0bd3a2b576b152d2a349782d1eb0f6b8e52e9954731d",
+                "sha256:20064ead0717cf9a73a6d1e779b23d149b53daf971169289ed2ed43a71e8d3b0",
+                "sha256:21fa558996782fc226b529fdd2ed7866c2c6ec91cee82735c98a197fae39f706",
+                "sha256:22908891a380d50738e1f978667536f6c6b526a2064156203d418f4856d6e86a",
+                "sha256:3160a0fd9754aab7d47f95a6b63ab355388d890163eb03b2d2b87ab0a30cfa59",
+                "sha256:322102cdf1ab682ecc7d9b1c5eed4ec59657a65e1c146a0da342b78f4112db23",
+                "sha256:34e0a2f9c370eb95597aae63bf85eb5e96826d81e3dcf88b8886012906f509b5",
+                "sha256:3573d376454d956553c356df45bb824262c397c6e26ce43e8203c4c540ee0acb",
+                "sha256:3747443b6a904001473370d7810aa19c3a180ccd52a7157aacc264a5ac79265e",
+                "sha256:38e812a197bf8e71a59fe55b757a84c1f946d0ac114acafaafaf21667a7e169e",
+                "sha256:3a06f32c9634a8705f4ca9946d667609f52cf130d5548881401f1eb2c39b1e2c",
+                "sha256:3a5fc78f9e3f501a1614a98f7c54d3969f3ad9bba8ba3d9b438c3bc5d047dd28",
+                "sha256:3d9098b479e78c85080c98e1e35ff40b4a31d8953102bb0fd7d1b6f8a2111a3d",
+                "sha256:3dc5b6a8ecfdc5748a7e429782598e4f17ef378e3e272eeb1340ea57c9109f41",
+                "sha256:4155b51ae05ed47199dc5b2a4e62abccb274cee6b01da5b895099b61b1982974",
+                "sha256:49919f8400b5e49e961f320c735388ee686a62327e773fa5b3ce6721f7e785ce",
+                "sha256:53d0a3fa5f8af98a1e261de6a3943ca631c526635eb5817a87a59d9a57ebf48f",
+                "sha256:5f008525e02908b20e04707a4f704cd286d94718f48bb33edddc7d7b584dddc1",
+                "sha256:628c985afb2c7d27a4800bfb609e03985aaecb42f955049957814e0491d4006d",
+                "sha256:65ed923f84a6844de5fd29726b888e58c62820e0769b76565480e1fdc3d062f8",
+                "sha256:6734e606355834f13445b6adc38b53c0fd45f1a56a9ba06c2058f86893ae8017",
+                "sha256:6baf0baf0d5d265fa7944feb9f7451cc316bfe30e8df1a61b1bb08577c554f31",
+                "sha256:6f4f4668e1831850ebcc2fd0b1cd11721947b6dc7c00bf1c6bd3c929ae14f2c7",
+                "sha256:6f5c2e7bc8a4bf7c426599765b1bd33217ec84023033672c1e9a8b35eaeaaaf8",
+                "sha256:6f6c7a8a57e9405cad7485f4c9d3172ae486cfef1344b5ddd8e5239582d7355e",
+                "sha256:7381c66e0561c5757ffe616af869b916c8b4e42b367ab29fedc98481d1e74e14",
+                "sha256:73dc03a6a7e30b7edc5b01b601e53e7fc924b04e1835e8e407c12c037e81adbd",
+                "sha256:74db0052d985cf37fa111828d0dd230776ac99c740e1a758ad99094be4f1803d",
+                "sha256:75f2568b4189dda1c567339b48cba4ac7384accb9c2a7ed655cd86b04055c795",
+                "sha256:78cacd03e79d009d95635e7d6ff12c21eb89b894c354bd2b2ed0b4763373693b",
+                "sha256:80d1543d58bd3d6c271b66abf454d437a438dff01c3e62fdbcd68f2a11310d4b",
+                "sha256:830d2948a5ec37c386d3170c483063798d7879037492540f10a475e3fd6f244b",
+                "sha256:891cf9b48776b5c61c700b55a598621fdb7b1e301a550365571e9624f270c203",
+                "sha256:8f25e17ab3039b05f762b0a55ae0b3632b2e073d9c8fc88e89aca31a6198e88f",
+                "sha256:9a3267620866c9d17b959a84dd0bd2d45719b817245e49371ead79ed4f710d19",
+                "sha256:a04f86f41a8916fe45ac5024ec477f41f886b3c435da2d4e3d2709b22ab02af1",
+                "sha256:aaf53a6cebad0eae578f062c7d462155eada9c172bd8c4d250b8c1d8eb7f916a",
+                "sha256:abc1185d79f47c0a7aaf7e2412a0eb2c03b724581139193d2d82b3ad8cbb00ac",
+                "sha256:ac0aa6cd53ab9a31d397f8303f92c42f534693528fafbdb997c82bae6e477ad9",
+                "sha256:ac3775e3311661d4adace3697a52ac0bab17edd166087d493b52d4f4f553f9f0",
+                "sha256:b06f0d3bf045158d2fb8837c5785fe9ff9b8c93358be64461a1089f5da983137",
+                "sha256:b116502087ce8a6b7a5f1814568ccbd0e9f6cfd99948aa59b0e241dc57cf739f",
+                "sha256:b82fab78e0b1329e183a65260581de4375f619167478dddab510c6c6fb04d9b6",
+                "sha256:bd7163182133c0c7701b25e604cf1611c0d87712e56e88e7ee5d72deab3e76b5",
+                "sha256:c36bcbc0d5174a80d6cccf43a0ecaca44e81d25be4b7f90f0ed7bcfbb5a00909",
+                "sha256:c3af8e0f07399d3176b179f2e2634c3ce9c1301379a6b8c9c9aeecd481da494f",
+                "sha256:c84132a54c750fda57729d1e2599bb598f5fa0344085dbde5003ba429a4798c0",
+                "sha256:cb7b2ab0188829593b9de646545175547a70d9a6e2b63bf2cd87a0a391599324",
+                "sha256:cca4def576f47a09a943666b8f829606bcb17e2bc2d5911a46c8f8da45f56755",
+                "sha256:cf6511efa4801b9b38dc5546d7547d5b5c6ef4b081c60b23e4d941d0eba9cbeb",
+                "sha256:d16fd5252f883eb074ca55cb622bc0bee49b979ae4e8639fff6ca3ff44f9f854",
+                "sha256:d2686f91611f9e17f4548dbf050e75b079bbc2a82be565832bc8ea9047b61c8c",
+                "sha256:d7fc3fca01da18fbabe4625d64bb612b533533ed10045a2ac3dd194bfa656b60",
+                "sha256:dd5653e67b149503c68c4018bf07e42eeed6b4e956b24c00ccdf93ac79cdff84",
+                "sha256:de5695a6f1d8340b12a5d6d4484290ee74d61e467c39ff03b39e30df62cf83a0",
+                "sha256:e0ac8959c929593fee38da1c2b64ee9778733cdf03c482c9ff1d508b6b593b2b",
+                "sha256:e1b25e3ad6c909f398df8921780d6a3d120d8c09466720226fc621605b6f92b1",
+                "sha256:e633940f28c1e913615fd624fcdd72fdba807bf53ea6925d6a588e84e1151531",
+                "sha256:e89df2958e5159b811af9ff0f92614dabf4ff617c03a4c1c6ff53bf1c399e0e1",
+                "sha256:ea9f9c6034ea2d93d9147818f17c2a0860d41b71c38b9ce4d55f21b6f9165a11",
+                "sha256:f645caaf0008bacf349875a974220f1f1da349c5dbe7c4ec93048cdc785a3326",
+                "sha256:f8303414c7b03f794347ad062c0516cee0e15f7a612abd0ce1e25caf6ceb47df",
+                "sha256:fca62a8301b605b954ad2e9c3666f9d97f63872aa4efcae5492baca2056b74ab"
             ],
-            "markers": "python_full_version >= '3.6.0'",
-            "version": "==3.0.1"
+            "markers": "python_full_version >= '3.7.0'",
+            "version": "==3.1.0"
         },
         "click": {
             "hashes": [
                 "sha256:7682dc8afb30297001674575ea00d1814d808d6a36af415a82bd481d37ba7b8e",
                 "sha256:bb4d8133cb15a609f44e8213d9b391b0809795062913b383c62be0ee95b1db48"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==8.1.3"
         },
-        "colorama": {
-            "hashes": [
-                "sha256:08695f5cb7ed6e0531a20572697297273c47b8cae5a63ffc6d6ed5c201be6e44",
-                "sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6"
-            ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6'",
-            "version": "==0.4.6"
-        },
         "coverage": {
             "extras": [
                 "toml"
             ],
             "hashes": [
-                "sha256:04481245ef966fbd24ae9b9e537ce899ae584d521dfbe78f89cad003c38ca2ab",
-                "sha256:0c45948f613d5d18c9ec5eaa203ce06a653334cf1bd47c783a12d0dd4fd9c851",
-                "sha256:10188fe543560ec4874f974b5305cd1a8bdcfa885ee00ea3a03733464c4ca265",
-                "sha256:218fe982371ac7387304153ecd51205f14e9d731b34fb0568181abaf7b443ba0",
-                "sha256:29571503c37f2ef2138a306d23e7270687c0efb9cab4bd8038d609b5c2393a3a",
-                "sha256:2a60d6513781e87047c3e630b33b4d1e89f39836dac6e069ffee28c4786715f5",
-                "sha256:2bf1d5f2084c3932b56b962a683074a3692bce7cabd3aa023c987a2a8e7612f6",
-                "sha256:3164d31078fa9efe406e198aecd2a02d32a62fecbdef74f76dad6a46c7e48311",
-                "sha256:32df215215f3af2c1617a55dbdfb403b772d463d54d219985ac7cd3bf124cada",
-                "sha256:33d1ae9d4079e05ac4cc1ef9e20c648f5afabf1a92adfaf2ccf509c50b85717f",
-                "sha256:33ff26d0f6cc3ca8de13d14fde1ff8efe1456b53e3f0273e63cc8b3c84a063d8",
-                "sha256:38da2db80cc505a611938d8624801158e409928b136c8916cd2e203970dde4dc",
-                "sha256:3b155caf3760408d1cb903b21e6a97ad4e2bdad43cbc265e3ce0afb8e0057e73",
-                "sha256:3b946bbcd5a8231383450b195cfb58cb01cbe7f8949f5758566b881df4b33baf",
-                "sha256:3baf5f126f30781b5e93dbefcc8271cb2491647f8283f20ac54d12161dff080e",
-                "sha256:4b14d5e09c656de5038a3f9bfe5228f53439282abcab87317c9f7f1acb280352",
-                "sha256:51b236e764840a6df0661b67e50697aaa0e7d4124ca95e5058fa3d7cbc240b7c",
-                "sha256:63ffd21aa133ff48c4dff7adcc46b7ec8b565491bfc371212122dd999812ea1c",
-                "sha256:6a43c7823cd7427b4ed763aa7fb63901ca8288591323b58c9cd6ec31ad910f3c",
-                "sha256:755e89e32376c850f826c425ece2c35a4fc266c081490eb0a841e7c1cb0d3bda",
-                "sha256:7a726d742816cb3a8973c8c9a97539c734b3a309345236cd533c4883dda05b8d",
-                "sha256:7c7c0d0827e853315c9bbd43c1162c006dd808dbbe297db7ae66cd17b07830f0",
-                "sha256:7ed681b0f8e8bcbbffa58ba26fcf5dbc8f79e7997595bf071ed5430d8c08d6f3",
-                "sha256:7ee5c9bb51695f80878faaa5598040dd6c9e172ddcf490382e8aedb8ec3fec8d",
-                "sha256:8361be1c2c073919500b6601220a6f2f98ea0b6d2fec5014c1d9cfa23dd07038",
-                "sha256:8ae125d1134bf236acba8b83e74c603d1b30e207266121e76484562bc816344c",
-                "sha256:9817733f0d3ea91bea80de0f79ef971ae94f81ca52f9b66500c6a2fea8e4b4f8",
-                "sha256:98b85dd86514d889a2e3dd22ab3c18c9d0019e696478391d86708b805f4ea0fa",
-                "sha256:9ccb092c9ede70b2517a57382a601619d20981f56f440eae7e4d7eaafd1d1d09",
-                "sha256:9d58885215094ab4a86a6aef044e42994a2bd76a446dc59b352622655ba6621b",
-                "sha256:b643cb30821e7570c0aaf54feaf0bfb630b79059f85741843e9dc23f33aaca2c",
-                "sha256:bc7c85a150501286f8b56bd8ed3aa4093f4b88fb68c0843d21ff9656f0009d6a",
-                "sha256:beeb129cacea34490ffd4d6153af70509aa3cda20fdda2ea1a2be870dfec8d52",
-                "sha256:c31b75ae466c053a98bf26843563b3b3517b8f37da4d47b1c582fdc703112bc3",
-                "sha256:c4e4881fa9e9667afcc742f0c244d9364d197490fbc91d12ac3b5de0bf2df146",
-                "sha256:c5b15ed7644ae4bee0ecf74fee95808dcc34ba6ace87e8dfbf5cb0dc20eab45a",
-                "sha256:d12d076582507ea460ea2a89a8c85cb558f83406c8a41dd641d7be9a32e1274f",
-                "sha256:d248cd4a92065a4d4543b8331660121b31c4148dd00a691bfb7a5cdc7483cfa4",
-                "sha256:d47dd659a4ee952e90dc56c97d78132573dc5c7b09d61b416a9deef4ebe01a0c",
-                "sha256:d4a5a5879a939cb84959d86869132b00176197ca561c664fc21478c1eee60d75",
-                "sha256:da9b41d4539eefd408c46725fb76ecba3a50a3367cafb7dea5f250d0653c1040",
-                "sha256:db61a79c07331e88b9a9974815c075fbd812bc9dbc4dc44b366b5368a2936063",
-                "sha256:ddb726cb861c3117a553f940372a495fe1078249ff5f8a5478c0576c7be12050",
-                "sha256:ded59300d6330be27bc6cf0b74b89ada58069ced87c48eaf9344e5e84b0072f7",
-                "sha256:e2617759031dae1bf183c16cef8fcfb3de7617f394c813fa5e8e46e9b82d4222",
-                "sha256:e5cdbb5cafcedea04924568d990e20ce7f1945a1dd54b560f879ee2d57226912",
-                "sha256:ec8e767f13be637d056f7e07e61d089e555f719b387a7070154ad80a0ff31801",
-                "sha256:ef382417db92ba23dfb5864a3fc9be27ea4894e86620d342a116b243ade5d35d",
-                "sha256:f2cba5c6db29ce991029b5e4ac51eb36774458f0a3b8d3137241b32d1bb91f06",
-                "sha256:f5b4198d85a3755d27e64c52f8c95d6333119e49fd001ae5798dac872c95e0f8",
-                "sha256:ffeeb38ee4a80a30a6877c5c4c359e5498eec095878f1581453202bfacc8fbc2"
+                "sha256:06ddd9c0249a0546997fdda5a30fbcb40f23926df0a874a60a8a185bc3a87d93",
+                "sha256:0743b0035d4b0e32bc1df5de70fba3059662ace5b9a2a86a9f894cfe66569013",
+                "sha256:0f3736a5d34e091b0a611964c6262fd68ca4363df56185902528f0b75dbb9c1f",
+                "sha256:1127b16220f7bfb3f1049ed4a62d26d81970a723544e8252db0efde853268e21",
+                "sha256:172db976ae6327ed4728e2507daf8a4de73c7cc89796483e0a9198fd2e47b462",
+                "sha256:182eb9ac3f2b4874a1f41b78b87db20b66da6b9cdc32737fbbf4fea0c35b23fc",
+                "sha256:1bb1e77a9a311346294621be905ea8a2c30d3ad371fc15bb72e98bfcfae532df",
+                "sha256:1fd78b911aea9cec3b7e1e2622c8018d51c0d2bbcf8faaf53c2497eb114911c1",
+                "sha256:20d1a2a76bb4eb00e4d36b9699f9b7aba93271c9c29220ad4c6a9581a0320235",
+                "sha256:21b154aba06df42e4b96fc915512ab39595105f6c483991287021ed95776d934",
+                "sha256:2c2e58e45fe53fab81f85474e5d4d226eeab0f27b45aa062856c89389da2f0d9",
+                "sha256:2c3b2803e730dc2797a017335827e9da6da0e84c745ce0f552e66400abdfb9a1",
+                "sha256:3146b8e16fa60427e03884301bf8209221f5761ac754ee6b267642a2fd354c48",
+                "sha256:344e714bd0fe921fc72d97404ebbdbf9127bac0ca1ff66d7b79efc143cf7c0c4",
+                "sha256:387065e420aed3c71b61af7e82c7b6bc1c592f7e3c7a66e9f78dd178699da4fe",
+                "sha256:3f04becd4fcda03c0160d0da9c8f0c246bc78f2f7af0feea1ec0930e7c93fa4a",
+                "sha256:4a42e1eff0ca9a7cb7dc9ecda41dfc7cbc17cb1d02117214be0561bd1134772b",
+                "sha256:4ea748802cc0de4de92ef8244dd84ffd793bd2e7be784cd8394d557a3c751e21",
+                "sha256:55416d7385774285b6e2a5feca0af9652f7f444a4fa3d29d8ab052fafef9d00d",
+                "sha256:5d0391fb4cfc171ce40437f67eb050a340fdbd0f9f49d6353a387f1b7f9dd4fa",
+                "sha256:63cdeaac4ae85a179a8d6bc09b77b564c096250d759eed343a89d91bce8b6367",
+                "sha256:72fcae5bcac3333a4cf3b8f34eec99cea1187acd55af723bcbd559adfdcb5535",
+                "sha256:7c4ed4e9f3b123aa403ab424430b426a1992e6f4c8fd3cb56ea520446e04d152",
+                "sha256:83957d349838a636e768251c7e9979e899a569794b44c3728eaebd11d848e58e",
+                "sha256:87ecc7c9a1a9f912e306997ffee020297ccb5ea388421fe62a2a02747e4d5539",
+                "sha256:8f69770f5ca1994cb32c38965e95f57504d3aea96b6c024624fdd5bb1aa494a1",
+                "sha256:8f6c930fd70d91ddee53194e93029e3ef2aabe26725aa3c2753df057e296b925",
+                "sha256:965ee3e782c7892befc25575fa171b521d33798132692df428a09efacaffe8d0",
+                "sha256:974bc90d6f6c1e59ceb1516ab00cf1cdfbb2e555795d49fa9571d611f449bcb2",
+                "sha256:981b4df72c93e3bc04478153df516d385317628bd9c10be699c93c26ddcca8ab",
+                "sha256:aa784405f0c640940595fa0f14064d8e84aff0b0f762fa18393e2760a2cf5841",
+                "sha256:ae7863a1d8db6a014b6f2ff9c1582ab1aad55a6d25bac19710a8df68921b6e30",
+                "sha256:aeae2aa38395b18106e552833f2a50c27ea0000122bde421c31d11ed7e6f9c91",
+                "sha256:b2317d5ed777bf5a033e83d4f1389fd4ef045763141d8f10eb09a7035cee774c",
+                "sha256:be19931a8dcbe6ab464f3339966856996b12a00f9fe53f346ab3be872d03e257",
+                "sha256:be9824c1c874b73b96288c6d3de793bf7f3a597770205068c6163ea1f326e8b9",
+                "sha256:c0045f8f23a5fb30b2eb3b8a83664d8dc4fb58faddf8155d7109166adb9f2040",
+                "sha256:c86bd45d1659b1ae3d0ba1909326b03598affbc9ed71520e0ff8c31a993ad911",
+                "sha256:ca0f34363e2634deffd390a0fef1aa99168ae9ed2af01af4a1f5865e362f8623",
+                "sha256:d298c2815fa4891edd9abe5ad6e6cb4207104c7dd9fd13aea3fdebf6f9b91259",
+                "sha256:d2a3a6146fe9319926e1d477842ca2a63fe99af5ae690b1f5c11e6af074a6b5c",
+                "sha256:dfd393094cd82ceb9b40df4c77976015a314b267d498268a076e940fe7be6b79",
+                "sha256:e58c0d41d336569d63d1b113bd573db8363bc4146f39444125b7f8060e4e04f5",
+                "sha256:ea3f5bc91d7d457da7d48c7a732beaf79d0c8131df3ab278e6bba6297e23c6c4",
+                "sha256:ea53151d87c52e98133eb8ac78f1206498c015849662ca8dc246255265d9c3c4",
+                "sha256:eb0edc3ce9760d2f21637766c3aa04822030e7451981ce569a1b3456b7053f22",
+                "sha256:f649dd53833b495c3ebd04d6eec58479454a1784987af8afb77540d6c1767abd",
+                "sha256:f760073fcf8f3d6933178d67754f4f2d4e924e321f4bb0dcef0424ca0215eba1",
+                "sha256:fa546d66639d69aa967bf08156eb8c9d0cd6f6de84be9e8c9819f52ad499c910",
+                "sha256:fd214917cabdd6f673a29d708574e9fbdb892cb77eb426d0eae3490d95ca7859",
+                "sha256:fff5aaa6becf2c6a1699ae6a39e2e6fb0672c2d42eca8eb0cafa91cf2e9bd312"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==7.1.0"
+            "version": "==7.2.3"
         },
         "docutils": {
             "hashes": [
                 "sha256:33995a6753c30b7f577febfc2c50411fec6aac7f7ffeb7c4cfe5991072dcf9e6",
                 "sha256:5e1de4d849fee02c63b040a4a3fd567f4ab104defd8a5511fbbc24a8a017efbc"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==0.19"
         },
-        "exceptiongroup": {
+        "flit": {
+            "hashes": [
+                "sha256:5ee0f88fd1cfa4160d1a8fa01237e96d06d677ae0403a0bbabbb277cb37c5e9c",
+                "sha256:d0f2a8f4bd45dc794befbf5839ecc0fd3830d65a57bd52b5997542fac5d5e937"
+            ],
+            "index": "pypi",
+            "version": "==3.8.0"
+        },
+        "flit-core": {
             "hashes": [
-                "sha256:327cbda3da756e2de031a3107b81ab7b3770a602c4d16ca618298c526f4bec1e",
-                "sha256:bcb67d800a4497e1b404c2dd44fca47d3b7a5e5433dbab67f96c1a685cdfdf23"
+                "sha256:64a29ec845164a6abe1136bf4bc5ae012bdfe758ed42fc7571a9059a7c80bd83",
+                "sha256:b305b30c99526df5e63d6022dd2310a0a941a187bd3884f4c8ef0418df6c39f3"
             ],
-            "markers": "python_version < '3.11'",
-            "version": "==1.1.0"
+            "markers": "python_version >= '3.6'",
+            "version": "==3.8.0"
         },
         "idna": {
             "hashes": [
                 "sha256:814f528e8dead7d329833b91c5faa87d60bf71824cd12a7530b5526063d02cb4",
                 "sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2"
             ],
             "markers": "python_version >= '3.5'",
             "version": "==3.4"
         },
         "importlib-metadata": {
             "hashes": [
-                "sha256:7efb448ec9a5e313a57655d35aa54cd3e01b7e1fbcf72dce1bf06119420f5bad",
-                "sha256:e354bedeb60efa6affdcc8ae121b73544a7aa74156d047311948f6d711cd378d"
+                "sha256:23c2bcae4762dfb0bbe072d358faec24957901d75b6c4ab11172c0c982532402",
+                "sha256:8f8bd2af397cf33bd344d35cfe7f489219b7d14fc79a3f854b75b8417e9226b0"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==6.0.0"
-        },
-        "importlib-resources": {
-            "hashes": [
-                "sha256:7d543798b0beca10b6a01ac7cafda9f822c54db9e8376a6bf57e0cbd74d486b6",
-                "sha256:e4a96c8cc0339647ff9a5e0550d9f276fc5a01ffa276012b58ec108cfd7b8484"
-            ],
-            "markers": "python_version < '3.9'",
-            "version": "==5.10.2"
+            "version": "==6.3.0"
         },
         "iniconfig": {
             "hashes": [
                 "sha256:2d91e135bf72d31a410b17c16da610a82cb55f6b0477d1a902134b24a455b8b3",
                 "sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374"
             ],
             "markers": "python_version >= '3.7'",
@@ -487,14 +440,22 @@
             "hashes": [
                 "sha256:771ed2a91909389ed6148631de678f82ddc73737d85a927f382a8a1b157898cd",
                 "sha256:ba2e15a9b35e21908d0aaf4e0a47acc52d6ae33444df0da2b49d41a46ef6d678"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==23.13.1"
         },
+        "markdown-it-py": {
+            "hashes": [
+                "sha256:5a35f8d1870171d9acc47b99612dc146129b631baf04970128b568f190d0cc30",
+                "sha256:7c9a5e412688bc771c67432cbfebcdd686c93ce6484913dccf06cb5a0bea35a1"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==2.2.0"
+        },
         "markupsafe": {
             "hashes": [
                 "sha256:0576fe974b40a400449768941d5d0858cc624e3249dfd1e0c33674e5c7ca7aed",
                 "sha256:085fd3201e7b12809f9e6e9bc1e5c96a368c8523fad5afb02afe3c051ae4afcc",
                 "sha256:090376d812fb6ac5f171e5938e82e7f2d7adc2b629101cec0db8b267815c85e2",
                 "sha256:0b462104ba25f1ac006fdab8b6a01ebbfbce9ed37fd37fd4acd70c67c973e460",
                 "sha256:137678c63c977754abe9086a3ec011e8fd985ab90631145dfb9294ad09c102a7",
@@ -543,53 +504,61 @@
                 "sha256:f1cd098434e83e656abf198f103a8207a8187c0fc110306691a2e94a78d0abb2",
                 "sha256:f2bfb563d0211ce16b63c7cb9395d2c682a23187f54c3d79bfec33e6705473c6",
                 "sha256:f8ffb705ffcf5ddd0e80b65ddf7bed7ee4f5a441ea7d3419e861a12eaf41af58"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.1.2"
         },
+        "mdurl": {
+            "hashes": [
+                "sha256:84008a41e51615a49fc9966191ff91509e3c40b939176e643fd50a5c2196b8f8",
+                "sha256:bb413d29f5eea38f31dd4754dd7377d4465116fb207585f97bf925588687c1ba"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==0.1.2"
+        },
         "more-itertools": {
             "hashes": [
-                "sha256:250e83d7e81d0c87ca6bd942e6aeab8cc9daa6096d12c5308f3f92fa5e5c1f41",
-                "sha256:5a6257e40878ef0520b1803990e3e22303a41b5714006c32a3fd8304b26ea1ab"
+                "sha256:cabaa341ad0389ea83c17a94566a53ae4c9d07349861ecb14dc6d0345cf9ac5d",
+                "sha256:d2bc7f02446e86a68911e58ded76d6561eea00cddfb2a91e7019bbb586c799f3"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==9.0.0"
+            "version": "==9.1.0"
         },
         "mypy": {
             "hashes": [
-                "sha256:01b1b9e1ed40544ef486fa8ac022232ccc57109f379611633ede8e71630d07d2",
-                "sha256:0ab090d9240d6b4e99e1fa998c2d0aa5b29fc0fb06bd30e7ad6183c95fa07593",
-                "sha256:14d776869a3e6c89c17eb943100f7868f677703c8a4e00b3803918f86aafbc52",
-                "sha256:1ace23f6bb4aec4604b86c4843276e8fa548d667dbbd0cb83a3ae14b18b2db6c",
-                "sha256:2efa963bdddb27cb4a0d42545cd137a8d2b883bd181bbc4525b568ef6eca258f",
-                "sha256:2f6ac8c87e046dc18c7d1d7f6653a66787a4555085b056fe2d599f1f1a2a2d21",
-                "sha256:3ae4c7a99e5153496243146a3baf33b9beff714464ca386b5f62daad601d87af",
-                "sha256:3cfad08f16a9c6611e6143485a93de0e1e13f48cfb90bcad7d5fde1c0cec3d36",
-                "sha256:4e5175026618c178dfba6188228b845b64131034ab3ba52acaffa8f6c361f805",
-                "sha256:50979d5efff8d4135d9db293c6cb2c42260e70fb010cbc697b1311a4d7a39ddb",
-                "sha256:5cd187d92b6939617f1168a4fe68f68add749902c010e66fe574c165c742ed88",
-                "sha256:5cfca124f0ac6707747544c127880893ad72a656e136adc935c8600740b21ff5",
-                "sha256:5e398652d005a198a7f3c132426b33c6b85d98aa7dc852137a2a3be8890c4072",
-                "sha256:67cced7f15654710386e5c10b96608f1ee3d5c94ca1da5a2aad5889793a824c1",
-                "sha256:7306edca1c6f1b5fa0bc9aa645e6ac8393014fa82d0fa180d0ebc990ebe15964",
-                "sha256:7cc2c01dfc5a3cbddfa6c13f530ef3b95292f926329929001d45e124342cd6b7",
-                "sha256:87edfaf344c9401942883fad030909116aa77b0fa7e6e8e1c5407e14549afe9a",
-                "sha256:8845125d0b7c57838a10fd8925b0f5f709d0e08568ce587cc862aacce453e3dd",
-                "sha256:92024447a339400ea00ac228369cd242e988dd775640755fa4ac0c126e49bb74",
-                "sha256:a86b794e8a56ada65c573183756eac8ac5b8d3d59daf9d5ebd72ecdbb7867a43",
-                "sha256:bb2782a036d9eb6b5a6efcdda0986774bf798beef86a62da86cb73e2a10b423d",
-                "sha256:be78077064d016bc1b639c2cbcc5be945b47b4261a4f4b7d8923f6c69c5c9457",
-                "sha256:c7cf862aef988b5fbaa17764ad1d21b4831436701c7d2b653156a9497d92c83c",
-                "sha256:e0626db16705ab9f7fa6c249c017c887baf20738ce7f9129da162bb3075fc1af",
-                "sha256:f34495079c8d9da05b183f9f7daec2878280c2ad7cc81da686ef0b484cea2ecf",
-                "sha256:fe523fcbd52c05040c7bee370d66fee8373c5972171e4fbc323153433198592d"
+                "sha256:023fe9e618182ca6317ae89833ba422c411469156b690fde6a315ad10695a521",
+                "sha256:031fc69c9a7e12bcc5660b74122ed84b3f1c505e762cc4296884096c6d8ee140",
+                "sha256:2de7babe398cb7a85ac7f1fd5c42f396c215ab3eff731b4d761d68d0f6a80f48",
+                "sha256:2e93a8a553e0394b26c4ca683923b85a69f7ccdc0139e6acd1354cc884fe0128",
+                "sha256:390bc685ec209ada4e9d35068ac6988c60160b2b703072d2850457b62499e336",
+                "sha256:3a2d219775a120581a0ae8ca392b31f238d452729adbcb6892fa89688cb8306a",
+                "sha256:3efde4af6f2d3ccf58ae825495dbb8d74abd6d176ee686ce2ab19bd025273f41",
+                "sha256:4a99fe1768925e4a139aace8f3fb66db3576ee1c30b9c0f70f744ead7e329c9f",
+                "sha256:4b41412df69ec06ab141808d12e0bf2823717b1c363bd77b4c0820feaa37249e",
+                "sha256:4c8d8c6b80aa4a1689f2a179d31d86ae1367ea4a12855cc13aa3ba24bb36b2d8",
+                "sha256:4d19f1a239d59f10fdc31263d48b7937c585810288376671eaf75380b074f238",
+                "sha256:4e4a682b3f2489d218751981639cffc4e281d548f9d517addfd5a2917ac78119",
+                "sha256:695c45cea7e8abb6f088a34a6034b1d273122e5530aeebb9c09626cea6dca4cb",
+                "sha256:701189408b460a2ff42b984e6bd45c3f41f0ac9f5f58b8873bbedc511900086d",
+                "sha256:70894c5345bea98321a2fe84df35f43ee7bb0feec117a71420c60459fc3e1eed",
+                "sha256:8293a216e902ac12779eb7a08f2bc39ec6c878d7c6025aa59464e0c4c16f7eb9",
+                "sha256:8d26b513225ffd3eacece727f4387bdce6469192ef029ca9dd469940158bc89e",
+                "sha256:a197ad3a774f8e74f21e428f0de7f60ad26a8d23437b69638aac2764d1e06a6a",
+                "sha256:bea55fc25b96c53affab852ad94bf111a3083bc1d8b0c76a61dd101d8a388cf5",
+                "sha256:c9a084bce1061e55cdc0493a2ad890375af359c766b8ac311ac8120d3a472950",
+                "sha256:d0e9464a0af6715852267bf29c9553e4555b61f5904a4fc538547a4d67617937",
+                "sha256:d8e9187bfcd5ffedbe87403195e1fc340189a68463903c39e2b63307c9fa0394",
+                "sha256:eaeaa0888b7f3ccb7bcd40b50497ca30923dba14f385bde4af78fac713d6d6f6",
+                "sha256:f46af8d162f3d470d8ffc997aaf7a269996d205f9d746124a179d3abe05ac602",
+                "sha256:f70a40410d774ae23fcb4afbbeca652905a04de7948eaf0b1789c8d1426b72d1",
+                "sha256:fe91be1c51c90e2afe6827601ca14353bbf3953f343c2129fa1e247d55fd95ba"
             ],
             "index": "pypi",
-            "version": "==1.0.0"
+            "version": "==1.2.0"
         },
         "mypy-extensions": {
             "hashes": [
                 "sha256:4392f6c0eb8a5668a69e23d168ffa70f0be9ccfd32b5cc2d26a34ae5b844552d",
                 "sha256:75dbf8955dc00442a438fc4d0666508a9a97b6bd41aa2f0ffe9d2f2725af0782"
             ],
             "markers": "python_version >= '3.5'",
@@ -601,75 +570,75 @@
                 "sha256:b6ad297f8907de0fa2fe1ccbd26fdaf387f5f47c7275fedf8cce89f99446cf97"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==23.0"
         },
         "pathspec": {
             "hashes": [
-                "sha256:3a66eb970cbac598f9e5ccb5b2cf58930cd8e3ed86d393d541eaf2d8b1705229",
-                "sha256:64d338d4e0914e91c1792321e6907b5a593f1ab1851de7fc269557a21b30ebbc"
+                "sha256:2798de800fa92780e33acca925945e9a19a133b715067cf165b8866c15a31687",
+                "sha256:d8af70af76652554bd134c22b3e8a1cc46ed7d91edcdd721ef1a0c51a84a5293"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==0.11.0"
+            "version": "==0.11.1"
         },
         "pdoc": {
             "hashes": [
-                "sha256:453236f225feddb8a9071428f1982a78d74b9b3da4bc4433aedb64dbd0cc87ab",
-                "sha256:c3f24f31286e634de9c76fa6e67bd5c0c5e74360b41dc91e6b82499831eb52d8"
+                "sha256:074ae532b3df71c90df043303a83dcbc92a54e6e63ebf12f30bdd0c7b6f6dbb4",
+                "sha256:f44cb93e2508b2f2411f33bf3abbe4fcc1ef766bc61b7433eddd0860f430cea6"
             ],
             "index": "pypi",
-            "version": "==12.3.1"
-        },
-        "pep517": {
-            "hashes": [
-                "sha256:4ba4446d80aed5b5eac6509ade100bff3e7943a8489de249654a5ae9b33ee35b",
-                "sha256:ae69927c5c172be1add9203726d4b84cf3ebad1edcd5f71fcdc746e66e829f59"
-            ],
-            "markers": "python_version >= '3.6'",
-            "version": "==0.13.0"
+            "version": "==13.1.0"
         },
         "pkginfo": {
             "hashes": [
                 "sha256:4b7a555a6d5a22169fcc9cf7bfd78d296b0361adad412a346c1226849af5e546",
                 "sha256:8fd5896e8718a4372f0ea9cc9d96f6417c9b986e23a4d116dda26b62cc29d046"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==1.9.6"
         },
         "platformdirs": {
             "hashes": [
-                "sha256:8a1228abb1ef82d788f74139988b137e78692984ec7b08eaa6c65f1723af28f9",
-                "sha256:b1d5eb14f221506f50d6604a561f4c5786d9e80355219694a1b244bcd96f4567"
+                "sha256:d5b638ca397f25f979350ff789db335903d7ea010ab28903f57b27e1b16c2b08",
+                "sha256:ebe11c0d7a805086e99506aa331612429a72ca7cd52a1f0d277dc4adc20cb10e"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.0.0"
+            "version": "==3.2.0"
         },
         "pluggy": {
             "hashes": [
                 "sha256:4224373bacce55f955a878bf9cfa763c1e360858e330072059e10bad68531159",
                 "sha256:74134bbf457f031a36d68416e1509f34bd5ccc019f0bcc952c7b909d06b37bd3"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==1.0.0"
         },
         "pygments": {
             "hashes": [
-                "sha256:b3ed06a9e8ac9a9aae5a6f5dbe78a8a58655d17b43b93c078f094ddc476ae297",
-                "sha256:fa7bd7bd2771287c0de303af8bfdfc731f51bd2c6a47ab69d117138893b82717"
+                "sha256:77a3299119af881904cd5ecd1ac6a66214b6e9bed1f2db16993b54adede64094",
+                "sha256:f7e36cffc4c517fbc252861b9a6e4644ca0e5abadf9a113c72d1358ad09b9500"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==2.14.0"
+            "markers": "python_version >= '3.7'",
+            "version": "==2.15.0"
+        },
+        "pyproject-hooks": {
+            "hashes": [
+                "sha256:283c11acd6b928d2f6a7c73fa0d01cb2bdc5f07c57a2eeb6e83d5e56b97976f8",
+                "sha256:f271b298b97f5955d53fb12b72c1fb1948c22c1a6b70b315c54cedaca0264ef5"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==1.0.0"
         },
         "pytest": {
             "hashes": [
-                "sha256:c7c6ca206e93355074ae32f7403e8ea12163b1163c976fee7d4d84027c162be5",
-                "sha256:d45e0952f3727241918b8fd0f376f5ff6b301cc0777c6f9a556935c92d8a7d42"
+                "sha256:58ecc27ebf0ea643ebfdf7fb1249335da761a00c9f955bcd922349bcb68ee57d",
+                "sha256:933051fa1bfbd38a21e73c3960cebdad4cf59483ddba7696c48509727e17f201"
             ],
             "index": "pypi",
-            "version": "==7.2.1"
+            "version": "==7.3.0"
         },
         "pytest-cov": {
             "hashes": [
                 "sha256:2feb1b751d66a8bd934e5edfa2e961d11309dc37b73b0eabe73b5945fee20f6b",
                 "sha256:996b79efde6433cdbd0088872dbc5fb3ed7fe1578b68cdbba634f14bb8dd0470"
             ],
             "index": "pypi",
@@ -681,30 +650,29 @@
                 "sha256:fbbdb085ef7c252a326fd8cdcac0aa3b1333d8811f131bdcc701002e1be7ed4f"
             ],
             "index": "pypi",
             "version": "==3.10.0"
         },
         "pytest-socket": {
             "hashes": [
-                "sha256:7c4b81dc6a51cbc0093f11791de00ff4a15ac698f5da96879a80f5d9ad4179b6",
-                "sha256:8726fd47b83b127451532b6d570c5b6c4cd204fca363936509b1f53195de6f4f"
+                "sha256:363c1d67228315d4fc7912f1aabfd570de29d0e3db6217d61db5728adacd7138",
+                "sha256:cca72f134ff01e0023c402e78d31b32e68da3efdf3493bf7788f8eba86a6824c"
             ],
             "index": "pypi",
-            "version": "==0.5.1"
+            "version": "==0.6.0"
         },
         "readme-renderer": {
             "hashes": [
                 "sha256:cd653186dfc73055656f090f227f5cb22a046d7f71a841dfa305f55c9a513273",
                 "sha256:f67a16caedfa71eef48a31b39708637a6f4664c4394801a7b0d6432d13907343"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==37.3"
         },
         "requests": {
-            "extras": [],
             "hashes": [
                 "sha256:64299f4909223da747622c030b781c0d7811e359c37124b4bd368fb8c6518baa",
                 "sha256:98b1b2782e3c6c4904938b84c0eb932721069dfdb9134313beff7c83c2df24bf"
             ],
             "markers": "python_version >= '3.7' and python_version < '4'",
             "version": "==2.28.2"
         },
@@ -713,126 +681,126 @@
                 "sha256:18565aa58116d9951ac39baa288d3adb5b3ff975c4f25eee78555d89e8f247f7",
                 "sha256:62e09f7ff5ccbda92772a29f394a49c3ad6cb181d568b1337626b2abb628a63d"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
             "version": "==0.10.1"
         },
         "rfc3986": {
-            "extras": [
-                "idna2008"
+            "extras": [],
+            "hashes": [
+                "sha256:50b1502b60e289cb37883f3dfd34532b8873c7de9f49bb546641ce9cbd256ebd",
+                "sha256:97aacf9dbd4bfd829baad6e6309fa6573aaf1be3f6fa735c8ab05e46cecb261c"
             ],
+            "markers": "python_version >= '3.7'",
+            "version": "==2.0.0"
+        },
+        "rich": {
             "hashes": [
-                "sha256:270aaf10d87d0d4e095063c65bf3ddbc6ee3d0b226328ce21e036f946e421835",
-                "sha256:a86d6e1f5b1dc238b218b012df0aa79409667bb209e58da56d0b94704e712a97"
+                "sha256:540c7d6d26a1178e8e8b37e9ba44573a3cd1464ff6348b99ee7061b95d1c6333",
+                "sha256:dc84400a9d842b3a9c5ff74addd8eb798d155f36c1c91303888e0a66850d2a15"
             ],
-            "version": "==1.5.0"
+            "markers": "python_full_version >= '3.7.0'",
+            "version": "==13.3.3"
         },
         "ruff": {
             "hashes": [
-                "sha256:0056b7e1975a3ad7ef7eb9df4ca9f905661caf924c6843ecbe4e10719cd6cd0b",
-                "sha256:1e523edf92c5e888d93a145ef20ad548fca4da7cbd7a8321b3539967a03b7caf",
-                "sha256:216592db3bd93c260cc329d3237548f17fea1f43f87673ab5cdeb04d548fbea9",
-                "sha256:25c3a84f8db9281385685041e98b67afd4a0bb5a872e897331af8229eb28b965",
-                "sha256:3b1caea095c22067abc685b8452be5a9079ca27b88bffd80730f9e4ca8f81e7c",
-                "sha256:71c05f627fb9efb0859af248fe00f61391266d14e9406c10236dec7db1b1bfe5",
-                "sha256:7afe3bc50339b916b75a587ed299859fae9c1056ed73d35531c0af610dbe67f6",
-                "sha256:801a209887f777811caf9fd4513eec9b505e139d1b0844e1eacd1b4683b0eba2",
-                "sha256:97293bae6da5bd82672473f6d43421de7dd27fe8a8b1b3c79ffeda37bcb492b4",
-                "sha256:a1bdd3b5ea60b160d3ceb2f8fef4d88af58b7932d4ed46c85c586ef2f277b71d",
-                "sha256:b38916c62eb2587743d2ec8e1f03a43eb5889cf4a56cb55f5eb3bffee5260e32",
-                "sha256:bbb1fe64d4641ce7e5855bbebd9e81f6a596501bcb67842600186b3aa9b950cf",
-                "sha256:d3e4bb03333b0c8012ad7d27246a7a95dba3d6ec8796c172af055a179a86b61c",
-                "sha256:daac673996ecbef77bccf8cd03189c60302568b7aec669e352aa2d8925b074b2",
-                "sha256:de9830cfcca81c5d25233bf4be6f2f95deb58a7eaf2295f91280de97a54240d7",
-                "sha256:e54233e7d97d5b705582f673dc3184c7b16c42f7eac3be707c0adf716e457293"
+                "sha256:0fbc689c23609edda36169c8708bb91bab111d8f44cb4a88330541757770ab30",
+                "sha256:2dba68a9e558ab33e6dd5d280af798a2d9d3c80c913ad9c8b8e97d7b287f1cc9",
+                "sha256:39abd02342cec0c131b2ddcaace08b2eae9700cab3ca7dba64ae5fd4f4881bd0",
+                "sha256:4bcec45abdf65c1328a269cf6cc193f7ff85b777fa2865c64cf2c96b80148a2c",
+                "sha256:581e64fa1518df495ca890a605ee65065101a86db56b6858f848bade69fc6489",
+                "sha256:6624a966c4a21110cee6780333e2216522a831364896f3d98f13120936eff40a",
+                "sha256:6c5f397ec0af42a434ad4b6f86565027406c5d0d0ebeea0d5b3f90c4bf55bc82",
+                "sha256:8dbd0cee5a81b0785dc0feeb2640c1e31abe93f0d77c5233507ac59731a626f1",
+                "sha256:8fa98e747e0fe185d65a40b0ea13f55c492f3b5f9a032a1097e82edaddb9e52e",
+                "sha256:aaa4f52a6e513f8daa450dac4859e80390d947052f592f0d8e796baab24df2fc",
+                "sha256:c1c715b0d1e18f9c509d7c411ca61da3543a4aa459325b1b1e52b8301d65c6d2",
+                "sha256:cc970f6ece0b4950e419f0252895ee42e9e8e5689c6494d18f5dc2c6ebb7f798",
+                "sha256:d1293acc64eba16a11109678dc4743df08c207ed2edbeaf38b3e10eb2597321b",
+                "sha256:d2eddc60ae75fc87f8bb8fd6e8d5339cf884cd6de81e82a50287424309c187ba",
+                "sha256:d95596e2f4cafead19a6d1ec0b86f8fda45ba66fe934de3956d71146a87959b3",
+                "sha256:daff64b4e86e42ce69e6367d63aab9562fc213cd4db0e146859df8abc283dba0",
+                "sha256:f268d52a71bf410aa45c232870c17049df322a7d20e871cfe622c9fc784aab7b"
             ],
             "index": "pypi",
-            "version": "==0.0.239"
+            "version": "==0.0.261"
         },
         "six": {
             "hashes": [
                 "sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926",
                 "sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
             "version": "==1.16.0"
         },
-        "tomli": {
+        "tomli-w": {
             "hashes": [
-                "sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc",
-                "sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f"
+                "sha256:9f2a07e8be30a0729e533ec968016807069991ae2fd921a78d42f429ae5f4463",
+                "sha256:f463434305e0336248cac9c2dc8076b707d8a12d019dd349f5c1e382dd1ae1b9"
             ],
-            "markers": "python_version < '3.11'",
-            "version": "==2.0.1"
-        },
-        "tqdm": {
-            "hashes": [
-                "sha256:5f4f682a004951c1b450bc753c710e9280c5746ce6ffedee253ddbcbf54cf1e4",
-                "sha256:6fee160d6ffcd1b1c68c65f14c829c22832bc401726335ce92c52d395944a6a1"
-            ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
-            "version": "==4.64.1"
+            "markers": "python_version >= '3.7'",
+            "version": "==1.0.0"
         },
         "twine": {
             "hashes": [
-                "sha256:8efa52658e0ae770686a13b675569328f1fba9837e5de1867bfe5f46a9aefe19",
-                "sha256:d0550fca9dc19f3d5e8eadfce0c227294df0a2a951251a4385797c8a6198b7c8"
+                "sha256:929bc3c280033347a00f847236564d1c52a3e61b1ac2516c97c48f3ceab756d8",
+                "sha256:9e102ef5fdd5a20661eb88fad46338806c3bd32cf1db729603fe3697b1bc83c8"
             ],
             "index": "pypi",
-            "version": "==3.8.0"
+            "version": "==4.0.2"
         },
         "types-requests": {
             "hashes": [
-                "sha256:dbc2933635860e553ffc59f5e264264981358baffe6342b925e3eb8261f866ee",
-                "sha256:fd530aab3fc4f05ee36406af168f0836e6f00f1ee51a0b96b7311f82cb675230"
+                "sha256:0d580652ce903f643f8c3b494dd01d29367ea57cea0c7ad7f65cf3169092edb0",
+                "sha256:cc1aba862575019306b2ed134eb1ea994cab1c887a22e18d3383e6dd42e9789b"
             ],
             "index": "pypi",
-            "version": "==2.28.11.12"
+            "version": "==2.28.11.17"
         },
         "types-urllib3": {
             "hashes": [
-                "sha256:5630e578246d170d91ebe3901788cd28d53c4e044dc2e2488e3b0d55fb6895d8",
-                "sha256:e8f25c8bb85cde658c72ee931e56e7abd28803c26032441eea9ff4a4df2b0c31"
+                "sha256:12c744609d588340a07e45d333bf870069fc8793bcf96bae7a96d4712a42591d",
+                "sha256:c44881cde9fc8256d05ad6b21f50c4681eb20092552351570ab0a8a0653286d6"
             ],
-            "version": "==1.26.25.5"
+            "version": "==1.26.25.10"
         },
         "typing-extensions": {
             "hashes": [
-                "sha256:1511434bb92bf8dd198c12b1cc812e800d4181cfcb867674e0f8279cc93087aa",
-                "sha256:16fa4864408f655d35ec496218b85f79b3437c829e93320c7c9215ccfd92489e"
+                "sha256:5cb5f4a79139d699607b3ef622a1dedafa84e115ab0024e0d9c044a9479ca7cb",
+                "sha256:fb33085c39dd998ac16d1431ebc293a8b3eedd00fd4a32de0ff79002c19511b4"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==4.4.0"
+            "version": "==4.5.0"
         },
         "urllib3": {
             "hashes": [
-                "sha256:076907bf8fd355cde77728471316625a4d2f7e713c125f51953bb5b3eecf4f72",
-                "sha256:75edcdc2f7d85b137124a6c3c9fc3933cdeaa12ecb9a6a959f22797a0feca7e1"
+                "sha256:8a388717b9476f934a21484e8c8e61875ab60644d29b9b39e11e4b9dc1c6b305",
+                "sha256:aa751d169e23c7479ce47a0cb0da579e3ede798f994f5816a74e4f4500dcea42"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'",
-            "version": "==1.26.14"
+            "version": "==1.26.15"
         },
         "webencodings": {
             "hashes": [
                 "sha256:a0af1213f3c2226497a97e2b3aa01a7e4bee4f403f95be16fc9acd2947514a78",
                 "sha256:b36a1c245f2d304965eb4e0a82848379241dc04b865afcc4aab16748587e1923"
             ],
             "version": "==0.5.1"
         },
         "wheel": {
             "hashes": [
-                "sha256:965f5259b566725405b05e7cf774052044b1ed30119b5d586b2703aafe8719ac",
-                "sha256:b60533f3f5d530e971d6737ca6d58681ee434818fab630c83a734bb10c083ce8"
+                "sha256:cd1196f3faee2b31968d626e1731c94f99cbdb67cf5a46e4f5656cbee7738873",
+                "sha256:d236b20e7cb522daf2390fa84c55eea81c5c30190f90f29ae2ca1ad8355bf247"
             ],
             "index": "pypi",
-            "version": "==0.38.4"
+            "version": "==0.40.0"
         },
         "zipp": {
             "hashes": [
-                "sha256:6c4fe274b8f85ec73c37a8e4e3fa00df9fb9335da96fb789e3b96b318e5097b3",
-                "sha256:a3cac813d40993596b39ea9e93a18e8a2076d5c378b8bc88ec32ab264e04ad02"
+                "sha256:112929ad649da941c23de50f356a2b5570c954b65150642bccdd66bf194d224b",
+                "sha256:48904fc76a60e542af151aded95726c1a5c34ed43ab4134b597665c86d7ad556"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.12.1"
+            "version": "==3.15.0"
         }
     }
 }
```

### Comparing `sporestack-9.1.0/README.md` & `sporestack-9.1.1/README.md`

 * *Files identical despite different names*

### Comparing `sporestack-9.1.0/pyproject.toml` & `sporestack-9.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sporestack-9.1.0/src/sporestack/api.py` & `sporestack-9.1.1/src/sporestack/api.py`

 * *Files identical despite different names*

### Comparing `sporestack-9.1.0/src/sporestack/api_client.py` & `sporestack-9.1.1/src/sporestack/api_client.py`

 * *Files identical despite different names*

### Comparing `sporestack-9.1.0/src/sporestack/cli.py` & `sporestack-9.1.1/src/sporestack/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 HOME = Path(_home)
 
 token_cli = typer.Typer(help="Commands to interact with SporeStack tokens")
 cli.add_typer(token_cli, name="token")
 server_cli = typer.Typer(help="Commands to interact with SporeStack servers")
 cli.add_typer(server_cli, name="server")
 
-_log_level = os.getenv("LOG_LEVEL", "info").upper()
+_log_level = os.getenv("LOG_LEVEL", "warning").upper()
 _numeric_log_level = getattr(logging, _log_level, None)
 if _numeric_log_level is None:
     raise ValueError(f"LOG_LEVEL: {_log_level} is invalid. Aborting!")
 assert isinstance(_numeric_log_level, int)
 logging.basicConfig(level=_numeric_log_level)
 
 DEFAULT_TOKEN = "primary"
```

### Comparing `sporestack-9.1.0/src/sporestack/client.py` & `sporestack-9.1.1/src/sporestack/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from typing import List, Union
 
 from . import api
 from .api_client import APIClient
 from .utils import random_machine_id, random_token
 
 
 @dataclass
 class Server:
     machine_id: str
-    api_client: APIClient = APIClient()
+    api_client: APIClient = field(default_factory=APIClient)
     token: Union[str, None] = None
 
     def info(self) -> api.ServerInfo.Response:
         return self.api_client.server_info(self.machine_id)
 
     def rebuild(self) -> None:
         self.api_client.server_rebuild(self.machine_id)
@@ -50,15 +50,15 @@
             machine_id=self.machine_id, days=days, token=self.token
         )
 
 
 @dataclass
 class Token:
     token: str = random_token()
-    api_client: APIClient = APIClient()
+    api_client: APIClient = field(default_factory=APIClient)
 
     def add(self, dollars: int, currency: str) -> None:
         """Add to token"""
         self.api_client.token_add(token=self.token, dollars=dollars, currency=currency)
 
     def balance(self) -> int:
         """Returns the token's balance in cents."""
@@ -111,15 +111,15 @@
         )
 
 
 @dataclass
 class Client:
     client_token: str = ""
     """Token to manage/pay for servers with."""
-    api_client: APIClient = APIClient()
+    api_client: APIClient = field(default_factory=APIClient)
     """Your own API Client, perhaps if you want to connect through Tor."""
 
     def flavors(self) -> api.Flavors.Response:
         """Returns available flavors (server sizes)."""
         return self.api_client.flavors()
 
     def operating_systems(self) -> api.OperatingSystems.Response:
```

### Comparing `sporestack-9.1.0/src/sporestack/models.py` & `sporestack-9.1.1/src/sporestack/models.py`

 * *Files identical despite different names*

### Comparing `sporestack-9.1.0/src/sporestack/utils.py` & `sporestack-9.1.1/src/sporestack/utils.py`

 * *Files identical despite different names*

### Comparing `sporestack-9.1.0/tests/test_api_client.py` & `sporestack-9.1.1/tests/test_api_client.py`

 * *Files identical despite different names*

### Comparing `sporestack-9.1.0/tests/test_cli.py` & `sporestack-9.1.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `sporestack-9.1.0/tests/test_utils.py` & `sporestack-9.1.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `sporestack-9.1.0/PKG-INFO` & `sporestack-9.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sporestack
-Version: 9.1.0
+Version: 9.1.1
 Summary: SporeStack API and CLI for launching servers with Monero or Bitcoin
 Keywords: bitcoin,monero,vps
 Author-email: SporeStack <support@sporestack.com>
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: pydantic
 Requires-Dist: httpx[socks]
```

