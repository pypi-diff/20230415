# Comparing `tmp/xiot-1.7.0.tar.gz` & `tmp/xiot-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/xiot-1.7.0.tar", last modified: Sat Apr 15 14:09:41 2023, max compression
+gzip compressed data, was "dist/xiot-1.7.2.tar", last modified: Sat Apr 15 14:10:55 2023, max compression
```

## Comparing `xiot-1.7.0.tar` & `xiot-1.7.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 Robin      (501) staff       (20)        0 2023-04-15 14:09:41.000000 xiot-1.7.0/
--rw-r--r--   0 Robin      (501) staff       (20)      242 2023-04-15 14:09:41.000000 xiot-1.7.0/PKG-INFO
-drwxr-xr-x   0 Robin      (501) staff       (20)        0 2023-04-15 14:09:41.000000 xiot-1.7.0/xiot.egg-info/
--rw-r--r--   0 Robin      (501) staff       (20)      242 2023-04-15 14:09:41.000000 xiot-1.7.0/xiot.egg-info/PKG-INFO
--rw-r--r--   0 Robin      (501) staff       (20)      168 2023-04-15 14:09:41.000000 xiot-1.7.0/xiot.egg-info/SOURCES.txt
--rw-r--r--   0 Robin      (501) staff       (20)       23 2023-04-15 14:09:41.000000 xiot-1.7.0/xiot.egg-info/requires.txt
--rw-r--r--   0 Robin      (501) staff       (20)       15 2023-04-15 14:09:41.000000 xiot-1.7.0/xiot.egg-info/top_level.txt
--rw-r--r--   0 Robin      (501) staff       (20)        1 2023-04-15 14:09:41.000000 xiot-1.7.0/xiot.egg-info/dependency_links.txt
--rw-r--r--   0 Robin      (501) staff       (20)     9459 2023-04-15 14:09:35.000000 xiot-1.7.0/xiot.py
--rw-r--r--   0 Robin      (501) staff       (20)      395 2020-02-10 15:11:28.000000 xiot-1.7.0/setup.py
--rw-r--r--   0 Robin      (501) staff       (20)       38 2023-04-15 14:09:41.000000 xiot-1.7.0/setup.cfg
--rw-r--r--   0 Robin      (501) staff       (20)    17265 2023-04-15 06:15:40.000000 xiot-1.7.0/xiotshell.py
+drwxr-xr-x   0 Robin      (501) staff       (20)        0 2023-04-15 14:10:55.000000 xiot-1.7.2/
+-rw-r--r--   0 Robin      (501) staff       (20)      242 2023-04-15 14:10:55.000000 xiot-1.7.2/PKG-INFO
+drwxr-xr-x   0 Robin      (501) staff       (20)        0 2023-04-15 14:10:55.000000 xiot-1.7.2/xiot.egg-info/
+-rw-r--r--   0 Robin      (501) staff       (20)      242 2023-04-15 14:10:55.000000 xiot-1.7.2/xiot.egg-info/PKG-INFO
+-rw-r--r--   0 Robin      (501) staff       (20)      168 2023-04-15 14:10:55.000000 xiot-1.7.2/xiot.egg-info/SOURCES.txt
+-rw-r--r--   0 Robin      (501) staff       (20)       23 2023-04-15 14:10:55.000000 xiot-1.7.2/xiot.egg-info/requires.txt
+-rw-r--r--   0 Robin      (501) staff       (20)       15 2023-04-15 14:10:55.000000 xiot-1.7.2/xiot.egg-info/top_level.txt
+-rw-r--r--   0 Robin      (501) staff       (20)        1 2023-04-15 14:10:55.000000 xiot-1.7.2/xiot.egg-info/dependency_links.txt
+-rw-r--r--   0 Robin      (501) staff       (20)     9471 2023-04-15 14:10:31.000000 xiot-1.7.2/xiot.py
+-rw-r--r--   0 Robin      (501) staff       (20)      395 2020-02-10 15:11:28.000000 xiot-1.7.2/setup.py
+-rw-r--r--   0 Robin      (501) staff       (20)       38 2023-04-15 14:10:55.000000 xiot-1.7.2/setup.cfg
+-rw-r--r--   0 Robin      (501) staff       (20)    17265 2023-04-15 06:15:40.000000 xiot-1.7.2/xiotshell.py
```

### Comparing `xiot-1.7.0/xiot.py` & `xiot-1.7.2/xiot.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 '''
 Created on 2018年11月23日
 
 @author: Robin
 '''
 from __future__ import print_function
 
-__version__ = '1.7.0'
+__version__ = '1.7.2'
 
 
 def md5(s):
     import hashlib
     m2 = hashlib.md5()
     m2.update(s.encode("utf8"))
     return m2.hexdigest()
@@ -191,15 +191,15 @@
                 r = None
                 if len(topicls) == 3:
                     appid, dtu_id, dev_id = topicls
                     if typename == 'action' and data.get('data', {}).get('action'):
                         r = dtu.on_action(dev_id, action=data['data']['action'], value=data['data'].get('value'))
                     elif typename == 'notify' and data.get('data'):
                         r = dtu.on_notify(dev_id, data=data['data'])
-                if r and data.get('_return'):
+                if r is not None and data.get('_return'):
                     # 动作回执
                     ret = data['_return']
                     # print('r', data, r)
                     self.publish(ret['topic'], {
                         'key': ret['key'],
                         'data': r
                     })
```

### Comparing `xiot-1.7.0/xiotshell.py` & `xiot-1.7.2/xiotshell.py`

 * *Files identical despite different names*

