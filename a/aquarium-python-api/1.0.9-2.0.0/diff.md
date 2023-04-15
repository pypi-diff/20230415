# Comparing `tmp/aquarium-python-api-1.0.9.tar.gz` & `tmp/aquarium-python-api-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aquarium-python-api-1.0.9.tar", last modified: Wed Sep 28 14:38:53 2022, max compression
+gzip compressed data, was "dist/aquarium-python-api-2.0.0.tar", last modified: Sat Apr 15 09:32:25 2023, max compression
```

## Comparing `aquarium-python-api-1.0.9.tar` & `aquarium-python-api-2.0.0.tar`

### file list

```diff
@@ -1,30 +1,33 @@
-drwxr-xr-x   0 yann       (501) staff       (20)        0 2022-09-28 14:38:53.149000 aquarium-python-api-1.0.9/
--rw-r--r--   0 yann       (501) staff       (20)    34915 2021-02-18 17:12:41.000000 aquarium-python-api-1.0.9/LICENSE.md
--rw-r--r--   0 yann       (501) staff       (20)     3241 2022-09-28 14:38:53.149422 aquarium-python-api-1.0.9/PKG-INFO
--rw-r--r--   0 yann       (501) staff       (20)     1816 2021-09-14 14:40:57.000000 aquarium-python-api-1.0.9/README.md
-drwxr-xr-x   0 yann       (501) staff       (20)        0 2022-09-28 14:38:53.118789 aquarium-python-api-1.0.9/aquarium/
--rw-r--r--   0 yann       (501) staff       (20)      917 2021-02-01 10:01:21.000000 aquarium-python-api-1.0.9/aquarium/__init__.py
--rw-r--r--   0 yann       (501) staff       (20)     7810 2021-11-09 10:01:24.000000 aquarium-python-api-1.0.9/aquarium/aquarium.py
--rw-r--r--   0 yann       (501) staff       (20)     3399 2021-02-19 08:43:44.000000 aquarium-python-api-1.0.9/aquarium/edge.py
--rw-r--r--   0 yann       (501) staff       (20)     1542 2021-02-18 17:12:41.000000 aquarium-python-api-1.0.9/aquarium/element.py
--rw-r--r--   0 yann       (501) staff       (20)     2899 2022-04-29 12:15:47.000000 aquarium-python-api-1.0.9/aquarium/entity.py
--rw-r--r--   0 yann       (501) staff       (20)      511 2021-02-18 17:12:41.000000 aquarium-python-api-1.0.9/aquarium/exceptions.py
--rw-r--r--   0 yann       (501) staff       (20)    18240 2021-11-10 11:43:44.000000 aquarium-python-api-1.0.9/aquarium/item.py
-drwxr-xr-x   0 yann       (501) staff       (20)        0 2022-09-28 14:38:53.140927 aquarium-python-api-1.0.9/aquarium/items/
--rw-r--r--   0 yann       (501) staff       (20)       24 2021-02-01 10:01:25.000000 aquarium-python-api-1.0.9/aquarium/items/__init__.py
--rw-r--r--   0 yann       (501) staff       (20)     4821 2022-09-28 14:19:48.000000 aquarium-python-api-1.0.9/aquarium/items/asset.py
--rw-r--r--   0 yann       (501) staff       (20)     1746 2021-02-19 09:44:35.000000 aquarium-python-api-1.0.9/aquarium/items/project.py
--rw-r--r--   0 yann       (501) staff       (20)      271 2021-02-18 12:06:41.000000 aquarium-python-api-1.0.9/aquarium/items/shot.py
--rw-r--r--   0 yann       (501) staff       (20)     5675 2022-06-23 08:57:47.000000 aquarium-python-api-1.0.9/aquarium/items/task.py
--rw-r--r--   0 yann       (501) staff       (20)      660 2021-02-19 09:35:47.000000 aquarium-python-api-1.0.9/aquarium/items/template.py
--rw-r--r--   0 yann       (501) staff       (20)     3331 2021-02-19 09:15:18.000000 aquarium-python-api-1.0.9/aquarium/items/user.py
--rw-r--r--   0 yann       (501) staff       (20)     1653 2021-02-19 09:03:04.000000 aquarium-python-api-1.0.9/aquarium/items/usergroup.py
--rw-r--r--   0 yann       (501) staff       (20)     1784 2021-02-18 18:39:22.000000 aquarium-python-api-1.0.9/aquarium/utils.py
-drwxr-xr-x   0 yann       (501) staff       (20)        0 2022-09-28 14:38:53.148258 aquarium-python-api-1.0.9/aquarium_python_api.egg-info/
--rw-r--r--   0 yann       (501) staff       (20)     3241 2022-09-28 14:38:52.000000 aquarium-python-api-1.0.9/aquarium_python_api.egg-info/PKG-INFO
--rw-r--r--   0 yann       (501) staff       (20)      610 2022-09-28 14:38:52.000000 aquarium-python-api-1.0.9/aquarium_python_api.egg-info/SOURCES.txt
--rw-r--r--   0 yann       (501) staff       (20)        1 2022-09-28 14:38:52.000000 aquarium-python-api-1.0.9/aquarium_python_api.egg-info/dependency_links.txt
--rw-r--r--   0 yann       (501) staff       (20)      110 2022-09-28 14:38:52.000000 aquarium-python-api-1.0.9/aquarium_python_api.egg-info/requires.txt
--rw-r--r--   0 yann       (501) staff       (20)        9 2022-09-28 14:38:52.000000 aquarium-python-api-1.0.9/aquarium_python_api.egg-info/top_level.txt
--rw-r--r--   0 yann       (501) staff       (20)     1266 2022-09-28 14:38:53.152411 aquarium-python-api-1.0.9/setup.cfg
--rw-r--r--   0 yann       (501) staff       (20)       37 2021-01-12 10:42:28.000000 aquarium-python-api-1.0.9/setup.py
+drwxr-xr-x   0 yann       (501) staff       (20)        0 2023-04-15 09:32:25.028462 aquarium-python-api-2.0.0/
+-rw-r--r--   0 yann       (501) staff       (20)    34915 2021-02-18 17:12:41.000000 aquarium-python-api-2.0.0/LICENSE.md
+-rw-r--r--   0 yann       (501) staff       (20)     3238 2023-04-15 09:32:25.028681 aquarium-python-api-2.0.0/PKG-INFO
+-rw-r--r--   0 yann       (501) staff       (20)     1813 2022-11-05 09:19:19.000000 aquarium-python-api-2.0.0/README.md
+drwxr-xr-x   0 yann       (501) staff       (20)        0 2023-04-15 09:32:25.001463 aquarium-python-api-2.0.0/aquarium/
+-rw-r--r--   0 yann       (501) staff       (20)      917 2021-02-01 10:01:21.000000 aquarium-python-api-2.0.0/aquarium/__init__.py
+-rw-r--r--   0 yann       (501) staff       (20)    12537 2023-04-15 09:11:35.000000 aquarium-python-api-2.0.0/aquarium/aquarium.py
+-rw-r--r--   0 yann       (501) staff       (20)     3399 2022-11-09 16:10:59.000000 aquarium-python-api-2.0.0/aquarium/edge.py
+-rw-r--r--   0 yann       (501) staff       (20)     1542 2022-11-09 16:11:01.000000 aquarium-python-api-2.0.0/aquarium/element.py
+-rw-r--r--   0 yann       (501) staff       (20)     2899 2022-11-09 16:11:03.000000 aquarium-python-api-2.0.0/aquarium/entity.py
+-rw-r--r--   0 yann       (501) staff       (20)      941 2023-04-15 08:48:21.000000 aquarium-python-api-2.0.0/aquarium/exceptions.py
+-rw-r--r--   0 yann       (501) staff       (20)    26536 2023-04-15 08:46:19.000000 aquarium-python-api-2.0.0/aquarium/item.py
+drwxr-xr-x   0 yann       (501) staff       (20)        0 2023-04-15 09:32:25.023566 aquarium-python-api-2.0.0/aquarium/items/
+-rw-r--r--   0 yann       (501) staff       (20)       24 2021-02-01 10:01:25.000000 aquarium-python-api-2.0.0/aquarium/items/__init__.py
+-rw-r--r--   0 yann       (501) staff       (20)     6444 2022-10-24 12:24:48.000000 aquarium-python-api-2.0.0/aquarium/items/asset.py
+-rw-r--r--   0 yann       (501) staff       (20)     5092 2023-04-15 09:03:56.000000 aquarium-python-api-2.0.0/aquarium/items/organisation.py
+-rw-r--r--   0 yann       (501) staff       (20)     5070 2022-11-10 09:26:31.000000 aquarium-python-api-2.0.0/aquarium/items/playlist.py
+-rw-r--r--   0 yann       (501) staff       (20)     2278 2022-10-07 09:30:26.000000 aquarium-python-api-2.0.0/aquarium/items/project.py
+-rw-r--r--   0 yann       (501) staff       (20)      271 2021-02-18 12:06:41.000000 aquarium-python-api-2.0.0/aquarium/items/shot.py
+-rw-r--r--   0 yann       (501) staff       (20)     6578 2023-01-12 08:03:01.000000 aquarium-python-api-2.0.0/aquarium/items/task.py
+-rw-r--r--   0 yann       (501) staff       (20)     1055 2023-04-15 08:53:33.000000 aquarium-python-api-2.0.0/aquarium/items/template.py
+-rw-r--r--   0 yann       (501) staff       (20)     4087 2022-11-05 08:59:00.000000 aquarium-python-api-2.0.0/aquarium/items/user.py
+-rw-r--r--   0 yann       (501) staff       (20)     1653 2021-02-19 09:03:04.000000 aquarium-python-api-2.0.0/aquarium/items/usergroup.py
+-rw-r--r--   0 yann       (501) staff       (20)     1870 2023-04-15 07:32:38.000000 aquarium-python-api-2.0.0/aquarium/tools.py
+-rw-r--r--   0 yann       (501) staff       (20)     3823 2023-02-07 11:39:40.000000 aquarium-python-api-2.0.0/aquarium/utils.py
+drwxr-xr-x   0 yann       (501) staff       (20)        0 2023-04-15 09:32:25.028041 aquarium-python-api-2.0.0/aquarium_python_api.egg-info/
+-rw-r--r--   0 yann       (501) staff       (20)     3238 2023-04-15 09:32:24.000000 aquarium-python-api-2.0.0/aquarium_python_api.egg-info/PKG-INFO
+-rw-r--r--   0 yann       (501) staff       (20)      686 2023-04-15 09:32:24.000000 aquarium-python-api-2.0.0/aquarium_python_api.egg-info/SOURCES.txt
+-rw-r--r--   0 yann       (501) staff       (20)        1 2023-04-15 09:32:24.000000 aquarium-python-api-2.0.0/aquarium_python_api.egg-info/dependency_links.txt
+-rw-r--r--   0 yann       (501) staff       (20)      123 2023-04-15 09:32:24.000000 aquarium-python-api-2.0.0/aquarium_python_api.egg-info/requires.txt
+-rw-r--r--   0 yann       (501) staff       (20)        9 2023-04-15 09:32:24.000000 aquarium-python-api-2.0.0/aquarium_python_api.egg-info/top_level.txt
+-rw-r--r--   0 yann       (501) staff       (20)     1280 2023-04-15 09:32:25.030188 aquarium-python-api-2.0.0/setup.cfg
+-rw-r--r--   0 yann       (501) staff       (20)       37 2021-01-12 10:42:28.000000 aquarium-python-api-2.0.0/setup.py
```

### Comparing `aquarium-python-api-1.0.9/LICENSE.md` & `aquarium-python-api-2.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-1.0.9/PKG-INFO` & `aquarium-python-api-2.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aquarium-python-api
-Version: 1.0.9
+Version: 2.0.0
 Summary: Aquarium python package
 Home-page: https://docs.fatfish.app/dev/python/index.html
 Author: Fatfish Lab
 Author-email: lab@fatfi.sh
 License: gpl-3.0
 Project-URL: Documentation, https://docs.fatfish.app/dev/python/index.html
 Project-URL: Source, https://github.com/fatfish-lab/aquarium-python-api
@@ -18,15 +18,15 @@
         
         Aquarium Studio is developed by [Fatfish Lab](https://fatfi.sh)
         
         ```python
         # -*- coding: utf-8 -*-
         from aquarium import Aquarium
         
-        aq = Aquarium('https://your-aquarium-server/v1')
+        aq = Aquarium('https://your-aquarium-server')
         aq.connect(AQ_USER, AQ_PASSWORD)
         
         me = aq.get_current_user()
         my_tasks = me.get_tasks()
         ```
         
         ## Installation
```

### Comparing `aquarium-python-api-1.0.9/README.md` & `aquarium-python-api-2.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 Aquarium Studio is developed by [Fatfish Lab](https://fatfi.sh)
 
 ```python
 # -*- coding: utf-8 -*-
 from aquarium import Aquarium
 
-aq = Aquarium('https://your-aquarium-server/v1')
+aq = Aquarium('https://your-aquarium-server')
 aq.connect(AQ_USER, AQ_PASSWORD)
 
 me = aq.get_current_user()
 my_tasks = me.get_tasks()
 ```
 
 ## Installation
```

### Comparing `aquarium-python-api-1.0.9/aquarium/__init__.py` & `aquarium-python-api-2.0.0/aquarium/__init__.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-1.0.9/aquarium/aquarium.py` & `aquarium-python-api-2.0.0/aquarium/aquarium.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,65 +1,100 @@
 # -*- coding: utf-8 -*-
 from . import JSON_CONTENT_TYPE
 from .item import Item
 from .edge import Edge
-from .utils import evaluate
+from .tools import evaluate
 from .items.user import User
 from .items.template import Template
 from .items.project import Project
 from .items.task import Task
 from .items.shot import Shot
 from .items.asset import Asset
 from .items.usergroup import Usergroup
+from .items.organisation import Organisation
+from .items.playlist import Playlist
 from .element import Element
+from .utils import Utils
 
 import requests
+
+import sys
+if sys.version_info[0] > 2:
+    from urllib.parse import urljoin, urlparse
+else:
+    from urlparse import urljoin, urlparse
+
 import json
 import logging
 logger=logging.getLogger(__name__)
 
 
 class Aquarium(object):
     """
     This class describes the main class of Aquarium
 
-    :param api_url: Specify the URL of the API. Don't forget to add the version you use ex: `/v1`
+    :param api_url: Specify the URL of the API.
     :type api_url: string
-    :param token: Specify the authentication token, to avoid :func:`~aquarium.aquarium.Aquarium.connect`
-    :type token: string
-
-    :ivar edge: Access to :class:`~aquarium.edge.Edge`
-    :ivar item: Access to :class:`~aquarium.item.Item`
-    :ivar asset: Access to subclass :class:`~aquarium.items.asset.Asset`
-    :ivar project: Access to subclass :class:`~aquarium.items.project.Project`
-    :ivar shot: Access to subclass :class:`~aquarium.items.shot.Shot`
-    :ivar task: Access to subclass :class:`~aquarium.items.task.Task`
-    :ivar template: Access to subclass :class:`~aquarium.items.template.Template`
-    :ivar user: Access to subclass :class:`~aquarium.items.user.User`
-    :ivar usergroup: Access to subclass :class:`~aquarium.items.usergroup.Usergroup`
+    :param token: Specify the authentication token, to avoid :func:`~aquarium.aquarium.Aquarium.signin`
+    :type token: string, optional
+    :param api_version: Specify the API version you want to use (default : `v1`).
+    :type api_version: string, optional
+    :param domain: Specify the domain used for unauthenticated requests. Mainly for Aquarium Fatfish Lab dev or local Aquarium server without DNS
+    :type domain: string, optional
+
+    :var token: Get the current token (populated after a first :func:`~aquarium.aquarium.Aquarium.signin`)
+    :var edge: Access to Edge class
+    :vartype edge: :class:`~aquarium.edge.Edge`
+    :var item: Access to Item class
+    :vartype item: :class:`~aquarium.item.Item`
+    :var asset: Access to Asset subclass
+    :vartype asset: :class:`~aquarium.items.asset.Asset`
+    :var playlist: Access to Playlist subclass
+    :vartype playlist: :class:`~aquarium.items.playlist.Playlist`
+    :var project: Access to Project subclass
+    :vartype project: :class:`~aquarium.items.project.Project`
+    :var shot: Access to Shot subclass
+    :vartype shot: :class:`~aquarium.items.shot.Shot`
+    :var task: Access to Task subclass
+    :vartype task: :class:`~aquarium.items.task.Task`
+    :var template: Access to Template subclass
+    :vartype template: :class:`~aquarium.items.template.Template`
+    :var user: Access to User subclass
+    :vartype user: :class:`~aquarium.items.user.User`
+    :var usergroup: Access to Usergroup subclass
+    :vartype usergroup: :class:`~aquarium.items.usergroup.Usergroup`
+    :var organisation: Access to Organisation subclass
+    :vartype organisation: :class:`~aquarium.items.organisation.Organisation`
+    :var utils: Access to Utils class
+    :vartype utils: :class:`~aquarium.utils.Utils`
     """
 
-    def __init__(self, api_url='', token=''):
+    def __init__(self, api_url='', token='', api_version='v1', domain=None):
         """
         Constructs a new instance.
         """
         # Session
         self.session=requests.Session()
 
         self.api_url=api_url
+        self.api_version=api_version
         self.token=token
+        self.domain=domain
         # Classes
         self.element=Element(parent=self)
         self.item=Item(parent=self)
         self.edge=Edge(parent=self)
+        self.utils=Utils()
+        # SubClasses
         self.user=User(parent=self)
         self.usergroup=Usergroup(parent=self)
+        self.organisation=Organisation(parent=self)
         self.template=Template(parent=self)
-        # SubClasses
         self.project=Project(parent=self)
+        self.playlist=Playlist(parent=self)
         self.task=Task(parent=self)
         self.shot=Shot(parent=self)
         self.asset=Asset(parent=self)
 
     def do_request(self, *args, **kwargs):
         """
         Execute a request to the API
@@ -82,19 +117,32 @@
             headers=kwargs.pop('headers')
             if headers is not None:
                 headers.update(dict(authorization=token))
         else:
             headers=dict(authorization=token)
             headers.update(JSON_CONTENT_TYPE)
 
+        if (self.domain):
+            headers['aquarium-domain'] = self.domain
+
         args=list(args)
         typ=args[0]
-        path=self.api_url
+        path = self.api_url
+
         if len(args) > 1:
-            path += '/'+args[1]
+            is_files = args[1].find('/files/') >= 0
+            if (is_files):
+                path = urljoin(path, args[1])
+            else:
+                path = urljoin(path, '{api_version}/{endpoint}'.format(
+                    api_version=self.api_version,
+                    endpoint=args[1]
+                ))
+        else:
+            path = urljoin(path, self.api_version)
 
         logger.debug('Send request : %s %s', typ, path)
         self.session.headers.update(headers)
         response=self.session.request(typ, path, **kwargs)
         evaluate(response)
         if decoding:
             response=response.json()
@@ -116,80 +164,163 @@
             id=data.get('_id')
             cls=None
             #As Item
             if id.split('/')[0]=='items':
                 type=data.get('type')
                 if type=='Project':
                     cls=self.project
+                elif type=='Playlist':
+                    cls=self.playlist
                 elif type=='User':
                     cls=self.user
                 elif type=='Template':
                     cls=self.template
                 elif type=='Usergroup':
                     cls=self.usergroup
                 elif type=='Asset':
                     cls=self.asset
                 elif type=='Shot':
                     cls=self.shot
                 elif type=='Task':
                     cls=self.task
+                elif type=='Organisation':
+                    cls=self.organisation
                 else:
                     cls=self.item
             #As Edge
             elif id.split('/')[0]=='connections':
                 cls=self.edge
             if cls is not None:
                 value=cls(data=data)
 
         return value
 
-    def connect(self, email='', password=''):
+    def signin(self, email='', password=''):
         """
         Sign in a user with its email and password
 
         :param      email:     The email of the user
         :type       email:     string
         :param      password:  The password of the user
         :type       password:  string
         """
-        return self.user.connect(email=email, password=password)
+        return self.user.signin(email=email, password=password)
 
-    def logout(self):
+    def connect(self, email='', password=''):
+        """
+        Alias of :func:`~aquarium.aquarium.Aquarium.signin`
+        """
+        return self.user.signin(email=email, password=password)
+
+    def signout(self):
         """
         Sign out current user by clearing the stored authentication token
 
         .. note::
-            After a :func:`~aquarium.aquarium.Aquarium.logout`, you need to use a :func:`~aquarium.aquarium.Aquarium.connect` before sending authenticated requests
+            After a :func:`~aquarium.aquarium.Aquarium.signout`, you need to use a :func:`~aquarium.aquarium.Aquarium.signin` before sending authenticated requests
 
         :returns: None
         """
         logger.info('Disconnect current user')
         logger.debug('Clear authentication token for logout')
-        self.token=''
+        self.user.signout()
+
+    def logout(self):
+        """
+        Alias of :func:`~aquarium.aquarium.Aquarium.signout`
+        """
+        self.signout()
+
+    def me(self):
+        """
+        Alias of :func:`~aquarium.aquarium.Aquarium.get_current_user`
+
+
+        :returns:   A :class:`~aquarium.items.user.User` instance of the connected user.
+        :rtype:     :class:`~aquarium.items.user.User` object
+        """
+        return self.get_current_user()
 
     def get_current_user(self):
         """
-        Gets the user profil of the connected user
+        Alias of :func:`~aquarium.items.user.User.get_current`
+
 
         :returns:   A :class:`~aquarium.items.user.User` instance of the connected user.
         :rtype:     :class:`~aquarium.items.user.User` object
         """
         result=self.user.get_current()
         return result
 
+    def mine(self):
+        """
+        Alias of :func:`~aquarium.items.user.User.get_profile`
+
+
+        :returns:   User, Usergroups and Organisations object
+        :rtype:     Dict {user: :class:`~aquarium.items.user.User`, usergroups: [:class:`~aquarium.items.usergroup.Usergroup`], organisations: [:class:`~aquarium.items.organisation.Organisation`]}
+        """
+        return self.user.get_profile()
+
     def get_server_status(self):
         """
         Gets the server status.
 
         :returns:   The server status
         :rtype:     dictionary
         """
         result=self.do_request('GET', 'status')
         return result
 
+    def ping (self):
+        """
+        Ping Aquarium server
+
+        :returns: Ping response: pong
+        :rtype:   string
+        """
+        ping = self.do_request('GET', 'ping', decoding=False)
+        return ping.text
+
+    def get_users (self):
+        """
+        Get all users
+
+        :returns: List of all users
+        :rtype:   List of :class:`~aquarium.items.user.User`
+        """
+
+        users = self.do_request('GET', 'users')
+
+        users = [self.cast(user) for user in users]
+        return users
+
+    def create_user (self, email, name=None):
+        """
+        Create a new user
+
+        :param      email:  The email of the new user
+        :type       email:  string
+        :param      name:   The name of the new user
+        :type       name:   string, optional
+
+        :returns:   User object
+        :rtype:     :class:`~aquarium.items.user.User`
+        """
+
+        payload = dict(email=email)
+        if name != None:
+            payload['name'] = name
+
+        user = self.do_request(
+            'POST', 'users', data=json.dumps(payload))
+
+        user = self.cast(user)
+        return user
+
     def upload_file(self, path=''):
         """
         Uploads a file on the server
 
         .. note::
             The file is just uploaded to Aquarium. The metadata are not saved on any item. Use :func:`~aquarium.item.Item.update_data` to save them on an item.
             You can also directly upload a file on an item with :func:`~aquarium.item.Item.upload_file`.
@@ -204,22 +335,39 @@
         files=dict(file=open(path, 'rb'))
         result = self.do_request('POST', 'upload', headers={'Content-Type': None}, files=files)
         files['file'].close()
         return result
 
     def query(self, meshql='', aliases={}):
         """
-        Query Entitys
+        Query entities
+
+        .. tip::
+            For better performances, we advice you to use the function :func:`~aquarium.item.Item.traverse`
 
         :param      meshql:        The meshql string
         :type       meshql:        string
         :param      aliases:       The aliases used in the meshql query
         :type       aliases:       dictionary
 
         :returns:   List of item, edge or VIEW used in the meshql query
         :rtype:     list
         """
         logger.debug('Send query : meshql : %s / aliases : %r',
                      meshql, aliases)
         data=dict(query=meshql, aliases=aliases)
         result=self.do_request('POST', 'query', data=json.dumps(data))
         return result
+
+    def get_file(self, file_path):
+        """
+        Get stored file on Aquarium server
+
+        :param      file_path:     The file path from item property (Exemple: `/files/file_id.jpg`)
+        :type       file_path:     string
+
+        :returns:   The file
+        :rtype:     list
+        """
+
+        response = self.do_request('GET', file_path, decoding=False)
+        return response.content
```

### Comparing `aquarium-python-api-1.0.9/aquarium/edge.py` & `aquarium-python-api-2.0.0/aquarium/edge.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 import json
-from .utils import to_string_url
+from .tools import to_string_url
 from .entity import Entity
 
 
 class Edge(Entity):
     """
     This class describes an Edge object child of Aquarium class.
     """
```

### Comparing `aquarium-python-api-1.0.9/aquarium/element.py` & `aquarium-python-api-2.0.0/aquarium/element.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-from .utils import pretty_print_format
+from .tools import pretty_print_format
 from inspect import ismethod
 
 class Element(object):
     def __init__(self, parent=None):
         self.parent=parent
 
     def __call__(self, data={}):
```

### Comparing `aquarium-python-api-1.0.9/aquarium/entity.py` & `aquarium-python-api-2.0.0/aquarium/entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 from . import JSON_CONTENT_TYPE
-from .utils import evaluate, pretty_print_format
+from .tools import evaluate, pretty_print_format
 from dotmap import DotMap
 import requests
 import logging
 logger=logging.getLogger(__name__)
 
 
 class Entity(object):
```

### Comparing `aquarium-python-api-1.0.9/aquarium/items/asset.py` & `aquarium-python-api-2.0.0/aquarium/items/asset.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,55 +1,85 @@
 # -*- coding: utf-8 -*-
+import os
 from ..item import Item
 
 
 class Asset(Item):
     """
     This class describes an Asset object child of Item class.
     """
 
-    def upload_on_task(self, task_name='', path='', data={}, message = None):
+    def upload_on_task(self, task_name='', path='', data={}, version_name=None, override_media = True, message = None):
         """
         Uploads new media version on asset task
 
-        :param      task_name:  The task name
-        :type       task_name:  string
-        :param      path:       The media path to upload
-        :type       path:       string
-        :param      data:  The data you want to upload with the file, optional
-        :type       data:  dict
-        :param      message:  The message associated with the upload, optional
-        :type       message:  string
+        :param      task_name:      The task name
+        :type       task_name:      string
+        :param      path:           The media path to upload
+        :type       path:           string
+        :param      data:           The data you want to upload with the file, optional
+        :type       data:           dict
+        :param      version_name:   The name of the version where you want to upload the file. Without version_name, the media is uploaded in the task, optional
+        :type       version_name:   string
+        :param      override_media: If the media already exist, a new history is created to override the existing one, optional
+        :type       override_media: boolean
+        :param      message:        The message associated with the upload, optional
+        :type       message:        string
 
         :returns:   Updated media object
         :rtype:     dictionary
         """
-        query="# -($Child, 2)> $Task AND item.data.name == '{0}' VIEW $view".format(task_name)
+        file_dir, file_name = os.path.split(path)
+        query = "# -($Child, 2)> 0,1 $Task AND item.data.name == '{0}' VIEW $view".format(
+            task_name)
 
         aliases={
             'view':{
-                "taskKey": "item._key",
+                "item": "item",
                 "mediaKey": "FIRST(# -($Child)> 0,1 $Media VIEW item._key)"
             }
         }
 
-        view=self.traverse(meshql=query, aliases=aliases)
-        if not view:
+        tasks=self.traverse(meshql=query, aliases=aliases)
+        if not tasks or len(tasks) == 0:
             raise RuntimeError('Could not find request')
-        view=view[0]
-        media_key=view.get('mediaKey')
 
-        if not media_key:
-            media=self.parent.task(view.get('taskKey')).append(type='Media')
-            media_key=media.item._key
+        media_key = tasks[0].get('mediaKey')
+        task = self.parent.cast(tasks[0]['item'])
 
-        if isinstance(media_key, list):
-            media_key=media_key[0]
+        if version_name == None:
+            if not media_key or override_media == False:
+                return task.append(type='Media', data=data, path=path)
+            else:
+                return self.parent.item(media_key).upload_file(path=path, data=data, message=message)
+        else:
+            versions = task.get_children(types='Version', names=version_name)
+
+            if len(versions) > 0:
+                version = versions[0].item
+            else:
+                version = task.append(
+                    type='Version', data=dict(name=version_name)).item
+
+            if override_media:
+                medias = version.get_children(types='Media')
+
+                if len(medias) > 0:
+                    existing_medias = [media for media in medias if media.item.data.originalname == file_name]
+                    if len(existing_medias) > 0:
+                        media = existing_medias[0].item
+                        return media.upload_file(
+                            path=path, data=data, message=message)
+                    else:
+                        return version.append(type='Media', data=data, path=path)
+                else:
+                    return version.append(type='Media', data=data, path=path)
+            else:
+                return version.append(type='Media', data=data, path=path)
 
-        return self.parent.item(media_key).upload_file(path=path, data=data, message=message)
 
     def get_tasks(self, task_name='', task_status=''):
         """
         Gets the tasks of the asset
 
         :param      task_name:    The name of the task
         :type       task_name:    string, optional
```

### Comparing `aquarium-python-api-1.0.9/aquarium/items/project.py` & `aquarium-python-api-2.0.0/aquarium/items/project.py`

 * *Files 20% similar despite different names*

```diff
@@ -28,26 +28,40 @@
         result = [self.parent.cast(data) for data in result]
         return result
 
     def get_shots(self):
         """
         Gets all the shots of the project
 
-        :returns:   List of Shot class and Edge class
-        :rtype:     List of dictionary {item: :class:`~aquarium.items.shot.Shot`, edge: :class:`~aquarium.edge.Edge`}
+        :returns:   List of Shot class, Edge class and Tasks
+        :rtype:     List of dictionary {item: :class:`~aquarium.items.shot.Shot`, edge: :class:`~aquarium.edge.Edge`, tasks: [:class:`~aquarium.items.task.Task`]}
         """
-        query = "# -($Child, 5)> 0, 0 $Shot"
-        result = self.traverse(meshql=query)
+        query = "# -($Child, 5)> 0, 0 $Shot VIEW $view"
+        aliases = {
+            "view": {
+                "item": 'item',
+                "edge": 'edge',
+                "tasks": '# -($Child)> $Task VIEW item'
+            }
+        }
+        result = self.traverse(meshql=query, aliases=aliases)
         result = [self.parent.element(data) for data in result]
         return result
 
     def get_assets(self):
         """
         Gets all the assets of the project
 
-        :returns:   List of Asset class and Edge class
-        :rtype:     List of dictionary {item: :class:`~aquarium.items.asset.Asset`, edge: :class:`~aquarium.edge.Edge`}
+        :returns:   List of Asset class, Edge class and Tasks
+        :rtype:     List of dictionary {item: :class:`~aquarium.items.asset.Asset`, edge: :class:`~aquarium.edge.Edge`, tasks: [:class:`~aquarium.items.task.Task`]}
         """
-        query = "# -($Child, 5)> 0, 0 $Asset"
-        result = self.traverse(meshql=query)
+        query = "# -($Child, 5)> 0, 0 $Asset VIEW $view"
+        aliases = {
+            "view": {
+                "item": 'item',
+                "edge": 'edge',
+                "tasks": '# -($Child)> $Task VIEW item'
+            }
+        }
+        result = self.traverse(meshql=query, aliases=aliases)
         result = [self.parent.element(data) for data in result]
         return result
```

### Comparing `aquarium-python-api-1.0.9/aquarium/items/task.py` & `aquarium-python-api-2.0.0/aquarium/items/task.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,38 +11,61 @@
     def assign_to(self, user_key=''):
         """
         Assign the task to user
 
         :param      user_key:  The user key
         :type       user_key:  string
 
-        :returns:   Edge object
+        :returns:   Created assigned edge object
         :rtype:     :class:`~aquarium.edge.Edge`
         """
         result = self.parent.edge.create(
-            type='Assigned', from_key=self._key, to_key=user_key)
+            type='Assigned', from_key=str(self._key), to_key=str(user_key))
         return result
 
-    def add_timelog(self, user_key='', comment='', date='', duration=''):
+    def unassign_from(self, user_key=''):
+        """
+        Unassign the task from user
+
+        :param      user_key:  The user key
+        :type       user_key:  string
+
+        :returns:   Deleted assigned edge object
+        :rtype:     :class:`~aquarium.edge.Edge`
+        """
+        result = self.traverse(
+            meshql='# -($Assigned)> 0,1 $User AND item._key == "{user_key}" VIEW edge'.format(user_key=user_key))
+
+        if len(result) > 0:
+            assigned_edge = self.parent.cast(result[0])
+            assigned_edge.delete()
+            return assigned_edge
+        else:
+            return None
+
+    def add_timelog(self, user_key, comment='', date='', duration=''):
         """
         Add a timelog to the task
 
         :param      user_key:  The user key
         :type       user_key:  string
         :param      comment:   The comment
         :type       comment:   string
-        :param      date:      The date
+        :param      date:      The date of the timelog. Use :func:`~aquarium.utils.Utils.date` to generate an ISO date string.
         :type       date:      string ISO 8601 (date)
-        :param      duration:  The duration
+        :param      duration:  The duration of the timelog. Use :func:`~aquarium.utils.Utils.duration` to generate an ISO duration string.
         :type       duration:  string ISO 8601 (duration)
 
         :returns:   Dictionary of Item object and Edge object
         :rtype:     dictionary {item: :class:`~aquarium.item.Item`, edge: :class:`~aquarium.edge.Edge`}
         """
 
+        if user_key == None:
+            user_key = self.parent.me()._key
+
         data = dict(
             duration=duration,
             comment=comment,
             performedAt=date,
             performedBy=user_key
         )
         result = self.append(type='Job', data=data)
```

### Comparing `aquarium-python-api-1.0.9/aquarium/items/user.py` & `aquarium-python-api-2.0.0/aquarium/items/user.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,47 +7,70 @@
 
 
 class User(Item):
     """
     This class describes an User object child of Item class.
     """
 
-    def connect(self, email='', password=''):
+    def signin(self, email='', password=''):
         """
         Sign in a user with it's email and password
 
         :param      email:     The email of the user
         :type       email:     string
         :param      password:  The password of the user
         :type       password:  string
 
-        :returns: Dictionary of token and User object
-        :rtype: dictionary
+        :returns: Dictionary User object
+        :rtype: Dict {user: :class:`~aquarium.items.user.User`}
         """
         logging.debug('Connect user %s', email)
         # Authenticate and retrieve the access token
         payload = dict(email=email, password=password)
         result = self.do_request(
             'POST', 'signin', headers=URL_CONTENT_TYPE, data=payload)
 
        # Store authentification information
         token = result.pop("token")
         self.parent.token = token
         result = self.parent.element(result)
 
         return result
 
+    def connect(self, email='', password=''):
+        """
+        Alias of :func:`~aquarium.items.user.User.signin`
+        """
+        return self.signin(email, password)
+
+    def signout(self):
+        """
+        Sign out the current user by clearing the stored authentication token
+
+        .. note::
+            After a :func:`~aquarium.items.user.User.signout`, you need to use a :func:`~aquarium.items.user.User.signin` before sending authenticated requests
+
+        :returns: None
+        """
+        self.do_request(
+            'POST', 'signout', decoding=False)
+
+       # Remove authentification information
+        self.parent.token = None
+
+        return None
+
     def get_profile(self):
         """
         Get the current profil.
 
-        :returns:   User and Usergroup object
-        :rtype:     Dict {user: :class:`~aquarium.items.user.User`, usergroups: [:class:`~aquarium.items.usergroup.Usergroup`]}
+        :returns:   User, Usergroups and Organisations object
+        :rtype:     Dict {user: :class:`~aquarium.items.user.User`, usergroups: [:class:`~aquarium.items.usergroup.Usergroup`], organisations: [:class:`~aquarium.items.organisation.Organisation`]}
         """
-        result = self.do_request('GET', 'users/me', headers=URL_CONTENT_TYPE)
+        result = self.do_request('GET', 'users/me')
         result = self.parent.element(result)
         return result
 
     def get_current(self):
         """
         Get the current user.
```

### Comparing `aquarium-python-api-1.0.9/aquarium/items/usergroup.py` & `aquarium-python-api-2.0.0/aquarium/items/usergroup.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-1.0.9/aquarium/utils.py` & `aquarium-python-api-2.0.0/aquarium/tools.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 import pprint
 import logging
 logger=logging.getLogger(__name__)
 from .exceptions import RequestError, AuthentificationError,\
                         AutorisationError, PathNotFoundError, \
-                        ConflictError, UploadExceedLimit, InternalError
+                        MethodNotAllowed, ConflictError, UploadExceedLimit, InternalError
 
 def pretty_print_format(data={}, indent=8, width=80, depth=10):
     dict_string=pprint.pformat(data, indent=indent, width=width, depth=depth)
     return dict_string
 
 def to_string_url(value=None):
     """
@@ -43,14 +43,16 @@
         raise RequestError(response)
     elif status_code==401:
         raise AuthentificationError(response)
     elif status_code==403:
         raise AutorisationError(response)
     elif status_code==404:
         raise PathNotFoundError(response)
+    elif status_code==405:
+        raise MethodNotAllowed(response)
     elif status_code==409:
         raise ConflictError(response)
     elif status_code==413:
         raise UploadExceedLimit(response)
     elif status_code==500:
         raise InternalError(response)
     else:
```

### Comparing `aquarium-python-api-1.0.9/aquarium_python_api.egg-info/PKG-INFO` & `aquarium-python-api-2.0.0/aquarium_python_api.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aquarium-python-api
-Version: 1.0.9
+Version: 2.0.0
 Summary: Aquarium python package
 Home-page: https://docs.fatfish.app/dev/python/index.html
 Author: Fatfish Lab
 Author-email: lab@fatfi.sh
 License: gpl-3.0
 Project-URL: Documentation, https://docs.fatfish.app/dev/python/index.html
 Project-URL: Source, https://github.com/fatfish-lab/aquarium-python-api
@@ -18,15 +18,15 @@
         
         Aquarium Studio is developed by [Fatfish Lab](https://fatfi.sh)
         
         ```python
         # -*- coding: utf-8 -*-
         from aquarium import Aquarium
         
-        aq = Aquarium('https://your-aquarium-server/v1')
+        aq = Aquarium('https://your-aquarium-server')
         aq.connect(AQ_USER, AQ_PASSWORD)
         
         me = aq.get_current_user()
         my_tasks = me.get_tasks()
         ```
         
         ## Installation
```

### Comparing `aquarium-python-api-1.0.9/aquarium_python_api.egg-info/SOURCES.txt` & `aquarium-python-api-2.0.0/aquarium_python_api.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -5,17 +5,20 @@
 aquarium/__init__.py
 aquarium/aquarium.py
 aquarium/edge.py
 aquarium/element.py
 aquarium/entity.py
 aquarium/exceptions.py
 aquarium/item.py
+aquarium/tools.py
 aquarium/utils.py
 aquarium/items/__init__.py
 aquarium/items/asset.py
+aquarium/items/organisation.py
+aquarium/items/playlist.py
 aquarium/items/project.py
 aquarium/items/shot.py
 aquarium/items/task.py
 aquarium/items/template.py
 aquarium/items/user.py
 aquarium/items/usergroup.py
 aquarium_python_api.egg-info/PKG-INFO
```

### Comparing `aquarium-python-api-1.0.9/setup.cfg` & `aquarium-python-api-2.0.0/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://docs.fatfish.app/dev/python/index.html
 project_urls = 
 	Documentation = https://docs.fatfish.app/dev/python/index.html
 	Source = https://github.com/fatfish-lab/aquarium-python-api
 	Aquarium = https://fatfi.sh/aquarium
-version = 1.0.9
+version = 2.0.0
 author = Fatfish Lab
 author_email = lab@fatfi.sh
 keywords = fatfish, lab, aquarium, studio, project, management, nodal, sdk, rest, cgi, vfx, api, python
 license = gpl-3.0
 license_file = LICENSE.md
 platform = any
 python_requires = '>=2.4'
@@ -28,14 +28,15 @@
 packages = find:
 setup_requires = 
 	setuptools>=30.3.0
 include_package_data = True
 install_requires = 
 	requests==2.25.1
 	dotmap==1.3.23
+	pytz>=2020.5
 
 [options.packages.find]
 exclude = 
 	tests
 	docs
 	examples
```

