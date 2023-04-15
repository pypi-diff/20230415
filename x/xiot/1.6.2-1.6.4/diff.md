# Comparing `tmp/xiot-1.6.2.tar.gz` & `tmp/xiot-1.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/xiot-1.6.2.tar", last modified: Tue Mar 21 15:32:45 2023, max compression
+gzip compressed data, was "dist/xiot-1.6.4.tar", last modified: Sat Apr 15 07:33:11 2023, max compression
```

## Comparing `xiot-1.6.2.tar` & `xiot-1.6.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 Robin      (501) staff       (20)        0 2023-03-21 15:32:45.000000 xiot-1.6.2/
--rw-r--r--   0 Robin      (501) staff       (20)      242 2023-03-21 15:32:45.000000 xiot-1.6.2/PKG-INFO
-drwxr-xr-x   0 Robin      (501) staff       (20)        0 2023-03-21 15:32:45.000000 xiot-1.6.2/xiot.egg-info/
--rw-r--r--   0 Robin      (501) staff       (20)      242 2023-03-21 15:32:45.000000 xiot-1.6.2/xiot.egg-info/PKG-INFO
--rw-r--r--   0 Robin      (501) staff       (20)      168 2023-03-21 15:32:45.000000 xiot-1.6.2/xiot.egg-info/SOURCES.txt
--rw-r--r--   0 Robin      (501) staff       (20)       23 2023-03-21 15:32:45.000000 xiot-1.6.2/xiot.egg-info/requires.txt
--rw-r--r--   0 Robin      (501) staff       (20)       15 2023-03-21 15:32:45.000000 xiot-1.6.2/xiot.egg-info/top_level.txt
--rw-r--r--   0 Robin      (501) staff       (20)        1 2023-03-21 15:32:45.000000 xiot-1.6.2/xiot.egg-info/dependency_links.txt
--rw-r--r--   0 Robin      (501) staff       (20)     9112 2022-09-08 03:04:36.000000 xiot-1.6.2/xiot.py
--rw-r--r--   0 Robin      (501) staff       (20)      395 2020-02-10 15:11:28.000000 xiot-1.6.2/setup.py
--rw-r--r--   0 Robin      (501) staff       (20)       38 2023-03-21 15:32:45.000000 xiot-1.6.2/setup.cfg
--rw-r--r--   0 Robin      (501) staff       (20)    17090 2022-12-09 07:16:01.000000 xiot-1.6.2/xiotshell.py
+drwxr-xr-x   0 Robin      (501) staff       (20)        0 2023-04-15 07:33:11.000000 xiot-1.6.4/
+-rw-r--r--   0 Robin      (501) staff       (20)      242 2023-04-15 07:33:11.000000 xiot-1.6.4/PKG-INFO
+-rw-r--r--   0 Robin      (501) staff       (20)       38 2023-04-15 07:33:11.000000 xiot-1.6.4/setup.cfg
+-rw-r--r--   0 Robin      (501) staff       (20)      395 2020-02-10 15:11:28.000000 xiot-1.6.4/setup.py
+drwxr-xr-x   0 Robin      (501) staff       (20)        0 2023-04-15 07:33:11.000000 xiot-1.6.4/xiot.egg-info/
+-rw-r--r--   0 Robin      (501) staff       (20)      242 2023-04-15 07:33:11.000000 xiot-1.6.4/xiot.egg-info/PKG-INFO
+-rw-r--r--   0 Robin      (501) staff       (20)      168 2023-04-15 07:33:11.000000 xiot-1.6.4/xiot.egg-info/SOURCES.txt
+-rw-r--r--   0 Robin      (501) staff       (20)        1 2023-04-15 07:33:11.000000 xiot-1.6.4/xiot.egg-info/dependency_links.txt
+-rw-r--r--   0 Robin      (501) staff       (20)       23 2023-04-15 07:33:11.000000 xiot-1.6.4/xiot.egg-info/requires.txt
+-rw-r--r--   0 Robin      (501) staff       (20)       15 2023-04-15 07:33:11.000000 xiot-1.6.4/xiot.egg-info/top_level.txt
+-rw-r--r--   0 Robin      (501) staff       (20)     9453 2023-04-15 04:41:31.000000 xiot-1.6.4/xiot.py
+-rw-r--r--   0 Robin      (501) staff       (20)    17265 2023-04-15 06:15:40.000000 xiot-1.6.4/xiotshell.py
```

### Comparing `xiot-1.6.2/xiot.py` & `xiot-1.6.4/xiot.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 '''
 Created on 2018年11月23日
 
 @author: Robin
 '''
 from __future__ import print_function
 
-__version__ = '1.6.2'
+__version__ = '1.6.4'
 
 
 def md5(s):
     import hashlib
     m2 = hashlib.md5()
     m2.update(s.encode("utf8"))
     return m2.hexdigest()
@@ -184,20 +184,29 @@
                     return
                 if not data or type(data) != dict:
                     return
                 typename = data.get('type')
                 datafrom = data.get('_from')
                 topicls = topic.split('/')
                 # print(topic, data)
+                r = None
                 if len(topicls) == 3:
                     appid, dtu_id, dev_id = topicls
                     if typename == 'action' and data.get('data', {}).get('action'):
-                        dtu.on_action(dev_id, action=data['data']['action'], value=data['data'].get('value'))
+                        r = dtu.on_action(dev_id, action=data['data']['action'], value=data['data'].get('value'))
                     elif typename == 'notify' and data.get('data'):
-                        dtu.on_notify(dev_id, data=data['data'])
+                        r = dtu.on_notify(dev_id, data=data['data'])
+                if data.get('_return'):
+                    # 动作回执
+                    ret = data['_return']
+                    # print('r', data, r)
+                    self.publish(ret['topic'], {
+                        'key': ret['key'],
+                        'data': r
+                    })
 
         client = Client(host=self.mqtt_host, port=self.mqtt_port, username=mqtt_username, password=mqtt_password)
         client.connect()
         topic = '%s/%s/#' % (self.app.appid, self.dtu_id)
         client.subscribe(topic)
         self.client = client
```

### Comparing `xiot-1.6.2/xiotshell.py` & `xiot-1.6.4/xiotshell.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,18 +62,18 @@
         MQTTDTU.__init__(self, app=self.shell.app, dtu_id=self.shell.gw_id,
                          mqtt_host=self.shell.mqtt_host,
                          mqtt_port=self.shell.mqtt_port,
                          mqtt_username=self.shell.mqtt_username,
                          mqtt_password=self.shell.mqtt_password)
 
     def on_action(self, dev_id, action, value=None):
-        self.shell.on_action(dev_id, action, value)
+        return self.shell.on_action(dev_id, action, value)
 
     def on_notify(self, dev_id, data):
-        self.shell.on_notify(dev_id, data)
+        return self.shell.on_notify(dev_id, data)
 
 
 class Runner(object):
     running = True
 
     def __init__(self, name=None):
         if not name:
@@ -162,28 +162,34 @@
     def new_dtu(self):
         if self.mqtt_host:
             dtu = ShellMQTTDTU(self)
         else:
             dtu = ShellDTU(self)
         return dtu
 
+    def on_ticks(self):
+        pass
+
+    def get_default_attributes(self):
+        return [
+            {'attr_id': 'version', 'name': '版本', 'value': __version__},
+            {'attr_id': 'type', 'name': '类型', 'value': 'shell'},
+            {'attr_id': 'code', 'name': '代码', 'value': self.dev_id},
+        ]
+
     def __shell_run__(self):
         while True:
             dtu = None
             while self.running:
                 try:
                     dtu = self.new_dtu()
                     self.dtu = dtu
                     define = self.runner.get_define()
                     attrs = define.get('attributes') or []
-                    attrs += [
-                        {'attr_id': 'version', 'name': '版本', 'value': __version__},
-                        {'attr_id': 'type', 'name': '类型', 'value': 'shell'},
-                        {'attr_id': 'code', 'name': '代码', 'value': self.dev_id},
-                    ]
+                    attrs += self.get_default_attributes() or []
                     if self.name:
                         define['name'] = self.name
                     define['attributes'] = attrs
                     print('registering %s ...' % define['name'])
                     self.app.doApi('register', {'dtu_id': self.dtu.dtu_id, 'dev_id': self.dev_id, 'define': define})
                     time.sleep(1)
                     print('running...')
@@ -202,21 +208,23 @@
                         if nd:
                             # print('update', nd)
                             dtu.updateValues(self.dev_id, nd)
                         lastdata.update(nd)
 
                     while self.running:
                         update()
+                        self.on_ticks()
                         ct = self.interval
                         while ct > 0 and self.running:
                             time.sleep(1)
                             ct -= 1
                 except:
                     import traceback
                     traceback.print_exc()
+                    time.sleep(3)
             if dtu:
                 dtu.sendEvent(self.dev_id, 'normal', u'主动断开连接')
                 dtu.updateValues(self.dev_id, {'status': 'disconnected'})
                 time.sleep(3)
                 dtu.stop()
                 self.dtu = None
         self.running = False
@@ -240,15 +248,15 @@
     def on_notify(self, dev_id, data):
         '''通知'''
         # print('shell on_notify', dev_id, data)
         pass
 
     def on_action(self, dev_id, action, value):
         if dev_id == self.dev_id:
-            self.runner.on_action(self.dtu, dev_id, action, value)
+            return self.runner.on_action(self.dtu, dev_id, action, value)
 
 
 class CommandRunner(Runner):
     def __init__(self, name=None, commands=[]):
         Runner.__init__(self, name)
         cmdmap = {}
         cmds = []
```

