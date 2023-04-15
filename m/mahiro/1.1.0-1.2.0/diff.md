# Comparing `tmp/mahiro-1.1.0.tar.gz` & `tmp/mahiro-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mahiro-1.1.0.tar", last modified: Sat Apr 15 16:08:39 2023, max compression
+gzip compressed data, was "mahiro-1.2.0.tar", last modified: Sat Apr 15 20:09:03 2023, max compression
```

## Comparing `mahiro-1.1.0.tar` & `mahiro-1.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 ryu        (501) staff       (20)        0 2023-04-15 16:08:39.059854 mahiro-1.1.0/
--rw-r--r--   0 ryu        (501) staff       (20)     1064 2023-04-15 13:55:07.000000 mahiro-1.1.0/LICENSE
--rw-r--r--   0 ryu        (501) staff       (20)      399 2023-04-15 16:08:39.059198 mahiro-1.1.0/PKG-INFO
--rw-r--r--   0 ryu        (501) staff       (20)      105 2023-04-15 14:22:50.000000 mahiro-1.1.0/README.md
-drwxr-xr-x   0 ryu        (501) staff       (20)        0 2023-04-15 16:08:39.050600 mahiro-1.1.0/mahiro/
--rw-r--r--   0 ryu        (501) staff       (20)       79 2023-04-15 14:58:09.000000 mahiro-1.1.0/mahiro/__init__.py
--rw-r--r--   0 ryu        (501) staff       (20)      955 2023-04-15 15:41:29.000000 mahiro-1.1.0/mahiro/main.py
--rw-r--r--   0 ryu        (501) staff       (20)     4092 2023-04-15 16:06:38.000000 mahiro-1.1.0/mahiro/models.py
--rw-r--r--   0 ryu        (501) staff       (20)     1871 2023-04-15 15:40:57.000000 mahiro-1.1.0/mahiro/send.py
-drwxr-xr-x   0 ryu        (501) staff       (20)        0 2023-04-15 16:08:39.058236 mahiro-1.1.0/mahiro.egg-info/
--rw-r--r--   0 ryu        (501) staff       (20)      399 2023-04-15 16:08:38.000000 mahiro-1.1.0/mahiro.egg-info/PKG-INFO
--rw-r--r--   0 ryu        (501) staff       (20)      241 2023-04-15 16:08:38.000000 mahiro-1.1.0/mahiro.egg-info/SOURCES.txt
--rw-r--r--   0 ryu        (501) staff       (20)        1 2023-04-15 16:08:38.000000 mahiro-1.1.0/mahiro.egg-info/dependency_links.txt
--rw-r--r--   0 ryu        (501) staff       (20)       78 2023-04-15 16:08:38.000000 mahiro-1.1.0/mahiro.egg-info/requires.txt
--rw-r--r--   0 ryu        (501) staff       (20)        7 2023-04-15 16:08:38.000000 mahiro-1.1.0/mahiro.egg-info/top_level.txt
--rw-r--r--   0 ryu        (501) staff       (20)       38 2023-04-15 16:08:39.060103 mahiro-1.1.0/setup.cfg
--rw-r--r--   0 ryu        (501) staff       (20)      690 2023-04-15 16:08:30.000000 mahiro-1.1.0/setup.py
+drwxr-xr-x   0 ryu        (501) staff       (20)        0 2023-04-15 20:09:03.618352 mahiro-1.2.0/
+-rw-r--r--   0 ryu        (501) staff       (20)     1064 2023-04-15 13:55:07.000000 mahiro-1.2.0/LICENSE
+-rw-r--r--   0 ryu        (501) staff       (20)      399 2023-04-15 20:09:03.617374 mahiro-1.2.0/PKG-INFO
+-rw-r--r--   0 ryu        (501) staff       (20)      105 2023-04-15 14:22:50.000000 mahiro-1.2.0/README.md
+drwxr-xr-x   0 ryu        (501) staff       (20)        0 2023-04-15 20:09:03.612288 mahiro-1.2.0/mahiro/
+-rw-r--r--   0 ryu        (501) staff       (20)       79 2023-04-15 14:58:09.000000 mahiro-1.2.0/mahiro/__init__.py
+-rw-r--r--   0 ryu        (501) staff       (20)      955 2023-04-15 15:41:29.000000 mahiro-1.2.0/mahiro/main.py
+-rw-r--r--   0 ryu        (501) staff       (20)     4088 2023-04-15 20:07:58.000000 mahiro-1.2.0/mahiro/models.py
+-rw-r--r--   0 ryu        (501) staff       (20)     1871 2023-04-15 15:40:57.000000 mahiro-1.2.0/mahiro/send.py
+drwxr-xr-x   0 ryu        (501) staff       (20)        0 2023-04-15 20:09:03.616459 mahiro-1.2.0/mahiro.egg-info/
+-rw-r--r--   0 ryu        (501) staff       (20)      399 2023-04-15 20:09:03.000000 mahiro-1.2.0/mahiro.egg-info/PKG-INFO
+-rw-r--r--   0 ryu        (501) staff       (20)      241 2023-04-15 20:09:03.000000 mahiro-1.2.0/mahiro.egg-info/SOURCES.txt
+-rw-r--r--   0 ryu        (501) staff       (20)        1 2023-04-15 20:09:03.000000 mahiro-1.2.0/mahiro.egg-info/dependency_links.txt
+-rw-r--r--   0 ryu        (501) staff       (20)       78 2023-04-15 20:09:03.000000 mahiro-1.2.0/mahiro.egg-info/requires.txt
+-rw-r--r--   0 ryu        (501) staff       (20)        7 2023-04-15 20:09:03.000000 mahiro-1.2.0/mahiro.egg-info/top_level.txt
+-rw-r--r--   0 ryu        (501) staff       (20)       38 2023-04-15 20:09:03.618522 mahiro-1.2.0/setup.cfg
+-rw-r--r--   0 ryu        (501) staff       (20)      690 2023-04-15 20:08:25.000000 mahiro-1.2.0/setup.py
```

### Comparing `mahiro-1.1.0/LICENSE` & `mahiro-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mahiro-1.1.0/mahiro/main.py` & `mahiro-1.2.0/mahiro/main.py`

 * *Files identical despite different names*

### Comparing `mahiro-1.1.0/mahiro/models.py` & `mahiro-1.2.0/mahiro/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         sender = Sender(id=id, qq=ctx.qq)
         return GroupMessageMahiro(ctx=ctx, sender=sender, extra=extra)
 
 
 # friend msg
 class FriendMessage(BaseModel):
     userId: int
-    userNickname: str = ""
+    userName: str = ""
     msg: Msg
     qq: int
 
 
 class FriendMessageMahiro:
     ctx: FriendMessage
     sender: Sender
```

### Comparing `mahiro-1.1.0/mahiro/send.py` & `mahiro-1.2.0/mahiro/send.py`

 * *Files identical despite different names*

### Comparing `mahiro-1.1.0/setup.py` & `mahiro-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     return "\n".join(data)
 
 setup(
     name="mahiro",
     description="Python bridge for Mahiro",
     long_description=read_files(["README.md"]),
     long_description_content_type="text/markdown",
-    version="1.1.0",
+    version="1.2.0",
     author="fz6m",
     author_email="i@fz6m.com",
     url="https://github.com/opq-osc/mahiro",
     license="MIT",
     keywords=["OPQ", "OPQBot", "mahiro"],
     packages=find_packages(),
     install_requires=read_files(["requirements.txt"]),
```

