# Comparing `tmp/slg-dev-ops-1.8.0.tar.gz` & `tmp/slg-dev-ops-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slg-dev-ops-1.8.0.tar", last modified: Thu Dec  9 14:38:40 2021, max compression
+gzip compressed data, was "slg-dev-ops-1.9.0.tar", last modified: Fri Dec 10 00:49:39 2021, max compression
```

## Comparing `slg-dev-ops-1.8.0.tar` & `slg-dev-ops-1.9.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-09 14:38:40.949467 slg-dev-ops-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (121)      703 2021-12-09 14:38:40.949467 slg-dev-ops-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      494 2021-12-09 14:38:29.000000 slg-dev-ops-1.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-09 14:38:40.949467 slg-dev-ops-1.8.0/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (121)     2209 2021-12-09 14:38:29.000000 slg-dev-ops-1.8.0/scripts/slg-create-python-script
--rwxr-xr-x   0 runner    (1001) docker     (121)     4004 2021-12-09 14:38:29.000000 slg-dev-ops-1.8.0/scripts/slg-digital-ocean-droplet-setup
--rw-r--r--   0 runner    (1001) docker     (121)      990 2021-12-09 14:38:29.000000 slg-dev-ops-1.8.0/scripts/slg-git-clone-default-username
--rw-r--r--   0 runner    (1001) docker     (121)     2415 2021-12-09 14:38:29.000000 slg-dev-ops-1.8.0/scripts/slg-git-make-repo-subdir-into-submodule
--rwxr-xr-x   0 runner    (1001) docker     (121)     3788 2021-12-09 14:38:29.000000 slg-dev-ops-1.8.0/scripts/slg-git-release
--rw-r--r--   0 runner    (1001) docker     (121)     1993 2021-12-09 14:38:29.000000 slg-dev-ops-1.8.0/scripts/slg-git-remove-submodule
--rw-r--r--   0 runner    (1001) docker     (121)     1694 2021-12-09 14:38:29.000000 slg-dev-ops-1.8.0/scripts/slg-git-setup-gh
--rwxr-xr-x   0 runner    (1001) docker     (121)     3320 2021-12-09 14:38:29.000000 slg-dev-ops-1.8.0/scripts/slg-init-nginx-conf-gunicorn
--rwxr-xr-x   0 runner    (1001) docker     (121)     1715 2021-12-09 14:38:29.000000 slg-dev-ops-1.8.0/scripts/slg-init-remote-crontab
--rwxr-xr-x   0 runner    (1001) docker     (121)      516 2021-12-09 14:38:29.000000 slg-dev-ops-1.8.0/scripts/slg-install-ansible
--rwxr-xr-x   0 runner    (1001) docker     (121)     1181 2021-12-09 14:38:29.000000 slg-dev-ops-1.8.0/scripts/slg-install-firewall
--rw-r--r--   0 runner    (1001) docker     (121)     1727 2021-12-09 14:38:29.000000 slg-dev-ops-1.8.0/scripts/slg-install-nginx
--rw-r--r--   0 runner    (1001) docker     (121)      913 2021-12-09 14:38:29.000000 slg-dev-ops-1.8.0/scripts/slg-nginx-reverse-proxy-to-multiple-https-sites
--rwxr-xr-x   0 runner    (1001) docker     (121)     2465 2021-12-09 14:38:29.000000 slg-dev-ops-1.8.0/scripts/slg-setup-tls-ssl-nginx
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-12-09 14:38:40.949467 slg-dev-ops-1.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      940 2021-12-09 14:38:29.000000 slg-dev-ops-1.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-09 14:38:40.949467 slg-dev-ops-1.8.0/slg_dev_ops/
--rw-r--r--   0 runner    (1001) docker     (121)      187 2021-12-09 14:38:29.000000 slg-dev-ops-1.8.0/slg_dev_ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1573 2021-12-09 14:38:29.000000 slg-dev-ops-1.8.0/slg_dev_ops/install_nginx.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-09 14:38:40.949467 slg-dev-ops-1.8.0/slg_dev_ops.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      703 2021-12-09 14:38:40.000000 slg-dev-ops-1.8.0/slg_dev_ops.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      693 2021-12-09 14:38:40.000000 slg-dev-ops-1.8.0/slg_dev_ops.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-09 14:38:40.000000 slg-dev-ops-1.8.0/slg_dev_ops.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2021-12-09 14:38:40.000000 slg-dev-ops-1.8.0/slg_dev_ops.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-10 00:49:39.431786 slg-dev-ops-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)      703 2021-12-10 00:49:39.431786 slg-dev-ops-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      494 2021-12-10 00:49:26.000000 slg-dev-ops-1.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-10 00:49:39.431786 slg-dev-ops-1.9.0/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2209 2021-12-10 00:49:26.000000 slg-dev-ops-1.9.0/scripts/slg-create-python-script
+-rwxr-xr-x   0 runner    (1001) docker     (121)     4573 2021-12-10 00:49:26.000000 slg-dev-ops-1.9.0/scripts/slg-digital-ocean-droplet-setup
+-rw-r--r--   0 runner    (1001) docker     (121)      990 2021-12-10 00:49:26.000000 slg-dev-ops-1.9.0/scripts/slg-git-clone-default-username
+-rw-r--r--   0 runner    (1001) docker     (121)     2415 2021-12-10 00:49:26.000000 slg-dev-ops-1.9.0/scripts/slg-git-make-repo-subdir-into-submodule
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3788 2021-12-10 00:49:26.000000 slg-dev-ops-1.9.0/scripts/slg-git-release
+-rw-r--r--   0 runner    (1001) docker     (121)     1993 2021-12-10 00:49:26.000000 slg-dev-ops-1.9.0/scripts/slg-git-remove-submodule
+-rw-r--r--   0 runner    (1001) docker     (121)     1694 2021-12-10 00:49:26.000000 slg-dev-ops-1.9.0/scripts/slg-git-setup-gh
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3320 2021-12-10 00:49:26.000000 slg-dev-ops-1.9.0/scripts/slg-init-nginx-conf-gunicorn
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1715 2021-12-10 00:49:26.000000 slg-dev-ops-1.9.0/scripts/slg-init-remote-crontab
+-rwxr-xr-x   0 runner    (1001) docker     (121)      516 2021-12-10 00:49:26.000000 slg-dev-ops-1.9.0/scripts/slg-install-ansible
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1181 2021-12-10 00:49:26.000000 slg-dev-ops-1.9.0/scripts/slg-install-firewall
+-rw-r--r--   0 runner    (1001) docker     (121)     1727 2021-12-10 00:49:26.000000 slg-dev-ops-1.9.0/scripts/slg-install-nginx
+-rw-r--r--   0 runner    (1001) docker     (121)      913 2021-12-10 00:49:26.000000 slg-dev-ops-1.9.0/scripts/slg-nginx-reverse-proxy-to-multiple-https-sites
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2465 2021-12-10 00:49:26.000000 slg-dev-ops-1.9.0/scripts/slg-setup-tls-ssl-nginx
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-12-10 00:49:39.431786 slg-dev-ops-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      940 2021-12-10 00:49:26.000000 slg-dev-ops-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-10 00:49:39.431786 slg-dev-ops-1.9.0/slg_dev_ops/
+-rw-r--r--   0 runner    (1001) docker     (121)      187 2021-12-10 00:49:26.000000 slg-dev-ops-1.9.0/slg_dev_ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1573 2021-12-10 00:49:26.000000 slg-dev-ops-1.9.0/slg_dev_ops/install_nginx.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-10 00:49:39.431786 slg-dev-ops-1.9.0/slg_dev_ops.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      703 2021-12-10 00:49:39.000000 slg-dev-ops-1.9.0/slg_dev_ops.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      693 2021-12-10 00:49:39.000000 slg-dev-ops-1.9.0/slg_dev_ops.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-10 00:49:39.000000 slg-dev-ops-1.9.0/slg_dev_ops.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       12 2021-12-10 00:49:39.000000 slg-dev-ops-1.9.0/slg_dev_ops.egg-info/top_level.txt
```

### Comparing `slg-dev-ops-1.8.0/PKG-INFO` & `slg-dev-ops-1.9.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slg-dev-ops
-Version: 1.8.0
+Version: 1.9.0
 Summary: This is a description.
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.6.3
 Description-Content-Type: text/markdown
```

### Comparing `slg-dev-ops-1.8.0/scripts/slg-create-python-script` & `slg-dev-ops-1.9.0/scripts/slg-create-python-script`

 * *Files identical despite different names*

### Comparing `slg-dev-ops-1.8.0/scripts/slg-digital-ocean-droplet-setup` & `slg-dev-ops-1.9.0/scripts/slg-digital-ocean-droplet-setup`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,16 @@
     parser.add_argument('-r', '--remote_ip',
                         help='Remote IP of the machine were connecting to.')
 
     bools.add_argument('-d', '--docker', action='store_true',
                        help='should we install docker?')
     bools.add_argument('-c', '--compose', action='store_true',
                        help='should we install docker-compose?')
+    bools.add_argument('-n', '--node', action='store_true',
+                       help='should we install node?')
 
     args = parser.parse_args()
 
     return args
 
 
 def verify_location(location):
@@ -89,14 +91,24 @@
             echo {password} | sudo -S curl -L "https://github.com/docker/compose/releases/download/1.29.1/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose &&
             echo {password} | sudo -S chmod +x /usr/local/bin/docker-compose
         '''
         subprocess.run(
             f'ssh {args.username}@{remote_ip} "{cmd}"', shell=True)
         print('Docker compose successfully installed')
 
+    if args.node:
+        cmd = f'''
+            echo {password} | sudo -S curl -sL https://deb.nodesource.com/setup_16.x -o /home/{args.username}/nodesource_setup.sh &&
+            echo {password} | sudo -S bash nodesource_setup.sh &&
+            echo {password} | sudo -S apt-get install -y nodejs
+        '''
+        subprocess.run(
+            f'ssh {args.username}@{remote_ip} "{cmd}"', shell=True)
+        print('Node/npm successfully installed')
+
     print(
         f"\n\nNow you can login as {args.username}: ssh {args.username}@{remote_ip}!")
 
     if args.docker:
         print("\n\nTo start docker run systemctl start docker && systemctl enable docker")
 
     # # copy github private ssh key from local machine to /Users/{args.username}/.ssh/ directory
```

### Comparing `slg-dev-ops-1.8.0/scripts/slg-git-clone-default-username` & `slg-dev-ops-1.9.0/scripts/slg-git-clone-default-username`

 * *Files identical despite different names*

### Comparing `slg-dev-ops-1.8.0/scripts/slg-git-make-repo-subdir-into-submodule` & `slg-dev-ops-1.9.0/scripts/slg-git-make-repo-subdir-into-submodule`

 * *Files identical despite different names*

### Comparing `slg-dev-ops-1.8.0/scripts/slg-git-release` & `slg-dev-ops-1.9.0/scripts/slg-git-release`

 * *Files identical despite different names*

### Comparing `slg-dev-ops-1.8.0/scripts/slg-git-remove-submodule` & `slg-dev-ops-1.9.0/scripts/slg-git-remove-submodule`

 * *Files identical despite different names*

### Comparing `slg-dev-ops-1.8.0/scripts/slg-git-setup-gh` & `slg-dev-ops-1.9.0/scripts/slg-git-setup-gh`

 * *Files identical despite different names*

### Comparing `slg-dev-ops-1.8.0/scripts/slg-init-nginx-conf-gunicorn` & `slg-dev-ops-1.9.0/scripts/slg-init-nginx-conf-gunicorn`

 * *Files identical despite different names*

### Comparing `slg-dev-ops-1.8.0/scripts/slg-init-remote-crontab` & `slg-dev-ops-1.9.0/scripts/slg-init-remote-crontab`

 * *Files identical despite different names*

### Comparing `slg-dev-ops-1.8.0/scripts/slg-install-ansible` & `slg-dev-ops-1.9.0/scripts/slg-install-ansible`

 * *Files identical despite different names*

### Comparing `slg-dev-ops-1.8.0/scripts/slg-install-firewall` & `slg-dev-ops-1.9.0/scripts/slg-install-firewall`

 * *Files identical despite different names*

### Comparing `slg-dev-ops-1.8.0/scripts/slg-install-nginx` & `slg-dev-ops-1.9.0/scripts/slg-install-nginx`

 * *Files identical despite different names*

### Comparing `slg-dev-ops-1.8.0/scripts/slg-nginx-reverse-proxy-to-multiple-https-sites` & `slg-dev-ops-1.9.0/scripts/slg-nginx-reverse-proxy-to-multiple-https-sites`

 * *Files identical despite different names*

### Comparing `slg-dev-ops-1.8.0/scripts/slg-setup-tls-ssl-nginx` & `slg-dev-ops-1.9.0/scripts/slg-setup-tls-ssl-nginx`

 * *Files identical despite different names*

### Comparing `slg-dev-ops-1.8.0/setup.py` & `slg-dev-ops-1.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `slg-dev-ops-1.8.0/slg_dev_ops/install_nginx.py` & `slg-dev-ops-1.9.0/slg_dev_ops/install_nginx.py`

 * *Files identical despite different names*

### Comparing `slg-dev-ops-1.8.0/slg_dev_ops.egg-info/PKG-INFO` & `slg-dev-ops-1.9.0/slg_dev_ops.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slg-dev-ops
-Version: 1.8.0
+Version: 1.9.0
 Summary: This is a description.
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.6.3
 Description-Content-Type: text/markdown
```

### Comparing `slg-dev-ops-1.8.0/slg_dev_ops.egg-info/SOURCES.txt` & `slg-dev-ops-1.9.0/slg_dev_ops.egg-info/SOURCES.txt`

 * *Files identical despite different names*

