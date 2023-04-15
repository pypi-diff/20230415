# Comparing `tmp/update-linux-2.0.0.tar.gz` & `tmp/update-linux-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "update-linux-2.0.0.tar", last modified: Mon Apr  3 10:39:37 2023, max compression
+gzip compressed data, was "update-linux-2.1.0.tar", last modified: Sat Apr 15 15:34:22 2023, max compression
```

## Comparing `update-linux-2.0.0.tar` & `update-linux-2.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 barry     (1000) barry     (1000)        0 2023-04-03 10:39:37.652385 update-linux-2.0.0/
--rw-r--r--   0 barry     (1000) barry     (1000)     5345 2023-04-03 10:39:37.652385 update-linux-2.0.0/PKG-INFO
--rw-r--r--   0 barry     (1000) barry     (1000)     4791 2023-04-03 10:39:37.000000 update-linux-2.0.0/README.md
--rw-r--r--   0 barry     (1000) barry     (1000)       38 2023-04-03 10:39:37.652385 update-linux-2.0.0/setup.cfg
--rw-r--r--   0 barry     (1000) barry     (1000)     2127 2023-04-02 12:26:46.000000 update-linux-2.0.0/setup_update_linux.py
-drwxr-xr-x   0 barry     (1000) barry     (1000)        0 2023-04-03 10:39:37.652385 update-linux-2.0.0/update_linux/
--rwxr-xr-x   0 barry     (1000) barry     (1000)    17036 2023-04-03 10:39:17.000000 update-linux-2.0.0/update_linux/__init__.py
--rw-r--r--   0 barry     (1000) barry     (1000)      105 2023-04-02 12:32:25.000000 update-linux-2.0.0/update_linux/__main__.py
-drwxr-xr-x   0 barry     (1000) barry     (1000)        0 2023-04-03 10:39:37.652385 update-linux-2.0.0/update_linux.egg-info/
--rw-r--r--   0 barry     (1000) barry     (1000)     5345 2023-04-03 10:39:37.000000 update-linux-2.0.0/update_linux.egg-info/PKG-INFO
--rw-r--r--   0 barry     (1000) barry     (1000)      299 2023-04-03 10:39:37.000000 update-linux-2.0.0/update_linux.egg-info/SOURCES.txt
--rw-r--r--   0 barry     (1000) barry     (1000)        1 2023-04-03 10:39:37.000000 update-linux-2.0.0/update_linux.egg-info/dependency_links.txt
--rw-r--r--   0 barry     (1000) barry     (1000)       60 2023-04-03 10:39:37.000000 update-linux-2.0.0/update_linux.egg-info/entry_points.txt
--rw-r--r--   0 barry     (1000) barry     (1000)       21 2023-04-03 10:39:37.000000 update-linux-2.0.0/update_linux.egg-info/requires.txt
--rw-r--r--   0 barry     (1000) barry     (1000)       13 2023-04-03 10:39:37.000000 update-linux-2.0.0/update_linux.egg-info/top_level.txt
+drwxr-xr-x   0 barry     (1000) barry     (1000)        0 2023-04-15 15:34:22.347320 update-linux-2.1.0/
+-rw-r--r--   0 barry     (1000) barry     (1000)     5408 2023-04-15 15:34:22.347320 update-linux-2.1.0/PKG-INFO
+-rw-r--r--   0 barry     (1000) barry     (1000)     4854 2023-04-15 15:34:21.000000 update-linux-2.1.0/README.md
+-rw-r--r--   0 barry     (1000) barry     (1000)       38 2023-04-15 15:34:22.347320 update-linux-2.1.0/setup.cfg
+-rw-r--r--   0 barry     (1000) barry     (1000)     2127 2023-04-02 12:26:46.000000 update-linux-2.1.0/setup_update_linux.py
+drwxr-xr-x   0 barry     (1000) barry     (1000)        0 2023-04-15 15:34:22.347320 update-linux-2.1.0/update_linux/
+-rwxr-xr-x   0 barry     (1000) barry     (1000)    17956 2023-04-15 09:47:12.000000 update-linux-2.1.0/update_linux/__init__.py
+-rw-r--r--   0 barry     (1000) barry     (1000)      144 2023-04-15 08:24:45.000000 update-linux-2.1.0/update_linux/__main__.py
+drwxr-xr-x   0 barry     (1000) barry     (1000)        0 2023-04-15 15:34:22.347320 update-linux-2.1.0/update_linux.egg-info/
+-rw-r--r--   0 barry     (1000) barry     (1000)     5408 2023-04-15 15:34:22.000000 update-linux-2.1.0/update_linux.egg-info/PKG-INFO
+-rw-r--r--   0 barry     (1000) barry     (1000)      299 2023-04-15 15:34:22.000000 update-linux-2.1.0/update_linux.egg-info/SOURCES.txt
+-rw-r--r--   0 barry     (1000) barry     (1000)        1 2023-04-15 15:34:22.000000 update-linux-2.1.0/update_linux.egg-info/dependency_links.txt
+-rw-r--r--   0 barry     (1000) barry     (1000)       60 2023-04-15 15:34:22.000000 update-linux-2.1.0/update_linux.egg-info/entry_points.txt
+-rw-r--r--   0 barry     (1000) barry     (1000)       21 2023-04-15 15:34:22.000000 update-linux-2.1.0/update_linux.egg-info/requires.txt
+-rw-r--r--   0 barry     (1000) barry     (1000)       13 2023-04-15 15:34:22.000000 update-linux-2.1.0/update_linux.egg-info/top_level.txt
```

### Comparing `update-linux-2.0.0/PKG-INFO` & `update-linux-2.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: update-linux
-Version: 2.0.0
+Version: 2.1.0
 Summary: Update Linux
 Home-page: https://github.com/barry-scott/CLI-tools
 Author: Barry Scott
 Author-email: barry@barrys-emacs.org
 License: Apache 2.0
 Keywords: development
 Classifier: Development Status :: 5 - Production/Stable
@@ -23,14 +23,16 @@
 
 It assumes that it can `ssh root@<host>` without a password prompt.
 
 If running update-linux on a macOS system it is necessary to flush DNS so that freshly booted hosts can be accessed by host-name.
 
 This is done with the command `sudo killall -HUP mDNSResponder`.
 
+update-linux will refuse to update the host it is running on.
+
 ## update-linux update process
 
 ```
 $ update-linux host
 ```
 
 For an update the following steps are performed:
```

### Comparing `update-linux-2.0.0/README.md` & `update-linux-2.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 
 It assumes that it can `ssh root@<host>` without a password prompt.
 
 If running update-linux on a macOS system it is necessary to flush DNS so that freshly booted hosts can be accessed by host-name.
 
 This is done with the command `sudo killall -HUP mDNSResponder`.
 
+update-linux will refuse to update the host it is running on.
+
 ## update-linux update process
 
 ```
 $ update-linux host
 ```
 
 For an update the following steps are performed:
```

### Comparing `update-linux-2.0.0/setup_update_linux.py` & `update-linux-2.1.0/setup_update_linux.py`

 * *Files identical despite different names*

### Comparing `update-linux-2.0.0/update_linux/__init__.py` & `update-linux-2.1.0/update_linux/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import time
 import socket
 import platform
 import tempfile
 import json
 from config_path import ConfigPath
 
-VERSION = '2.0.0'
+VERSION = '2.1.0'
 
 default_json_config_template = u'''{
     "group":
         {"all": []},
     "logdir":   "%(logdir)s"
 }
 '''
@@ -190,61 +190,85 @@
             for group in self.all_groups:
                 print( fmt % (group, ', '.join( self.all_groups[ group ]) ) )
 
             print()
             print( 'Log directory: %s' % (self.logdir,) )
             return 0
 
-        if len(positional_args) == 0:
+        all_to_exclude = []
+        if self.opt_exclude:
+            all_to_exclude = self.all_groups.get( self.opt_exclude(), self.opt_exclude() )
+
+        for group_or_host in positional_args:
+            if group_or_host in self.all_groups:
+                for host in self.all_groups[ group_or_host ]:
+                    if host not in all_to_exclude:
+                        self.all_hosts.append( host )
+            else:
+                if host not in all_to_exclude:
+                    self.all_hosts.append( group_or_host )
+
+        if len(self.all_hosts) == 0:
             self.error( '', 'No hosts to update' )
             print('''
 For help:
     %s --help
 ''' % (appname.name,))
             return 1
 
-        this_host = socket.gethostname().split('.')[0]
-
         self.summary_log_name = self.logdir / ('update-summary-%s.log' % (self.ts,))
 
         with open( self.summary_log_name, 'a' ) as self.summary_log:
             t = datetime.datetime.now()
             self.header( 'Update summary %s' % (t.strftime( '%Y-%m-%d %H:%M:%S' ),) )
 
-            for group_or_host in positional_args:
-                if group_or_host in self.all_groups:
-                    for host in self.all_groups[ group_or_host ]:
-                        self.all_hosts.append( host )
-                else:
-                    self.all_hosts.append( group_or_host )
-
             for host in self.all_hosts:
+                if host in all_to_exclude:
+                    continue
+
                 self.flushDns()
                 if self.opt_check:
                     self.check( host )
 
                 elif self.opt_install_package() is not None:
                     self.installPackage( host, self.opt_install_package )
 
-                elif self.opt_system_upgrade:
-                    self.systemUpgrade( host, self.opt_system_upgrade )
-
                 else:
-                    if host == this_host:
+                    if self.isThisHost( host ):
                         self.warn( host, 'Refusing to update this host' )
 
+                    elif self.opt_system_upgrade:
+                        self.systemUpgrade( host, self.opt_system_upgrade )
+
                     else:
                         self.update( host )
 
         print( '-' * 60 )
         for line in self.all_summary_lines:
             print( line )
 
         return 0
 
+    def isThisHost( self, other_host ):
+        this_host = socket.gethostname()
+        this_info = socket.getaddrinfo( this_host, 'ssh', proto=socket.IPPROTO_TCP )
+        this_addrs = set(info[4][0] for info in this_info) | set(['::1', '127.0.0.1'])
+
+        try:
+            other_info = socket.getaddrinfo( other_host, 'ssh', proto=socket.IPPROTO_TCP )
+        except socket.gaierror as e:
+            self.warn( other_host, str(e) )
+            # return true to prevent update
+            return True
+
+        other_addrs = set(info[4][0] for info in other_info)
+
+        # share any address in common?
+        return len(this_addrs & other_addrs) > 0
+
     def loadConfig( self ):
         self.config = ConfigPath( 'update-linux', 'barrys-emacs.org', '.json' )
         config_file = self.config.readFilePath()
         default_json_config = default_json_config_template % {
                         'logdir': tempfile.gettempdir()
                         }
         if config_file is None:
```

### Comparing `update-linux-2.0.0/update_linux.egg-info/PKG-INFO` & `update-linux-2.1.0/update_linux.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: update-linux
-Version: 2.0.0
+Version: 2.1.0
 Summary: Update Linux
 Home-page: https://github.com/barry-scott/CLI-tools
 Author: Barry Scott
 Author-email: barry@barrys-emacs.org
 License: Apache 2.0
 Keywords: development
 Classifier: Development Status :: 5 - Production/Stable
@@ -23,14 +23,16 @@
 
 It assumes that it can `ssh root@<host>` without a password prompt.
 
 If running update-linux on a macOS system it is necessary to flush DNS so that freshly booted hosts can be accessed by host-name.
 
 This is done with the command `sudo killall -HUP mDNSResponder`.
 
+update-linux will refuse to update the host it is running on.
+
 ## update-linux update process
 
 ```
 $ update-linux host
 ```
 
 For an update the following steps are performed:
```

