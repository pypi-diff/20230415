# Comparing `tmp/jcmutils-1.1.9.tar.gz` & `tmp/jcmutils-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jcmutils-1.1.9.tar", last modified: Thu Mar 23 08:31:41 2023, max compression
+gzip compressed data, was "jcmutils-1.2.0.tar", last modified: Sat Apr 15 13:23:04 2023, max compression
```

## Comparing `jcmutils-1.1.9.tar` & `jcmutils-1.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 junquan   (1000) junquan   (1000)        0 2023-03-23 08:31:41.312073 jcmutils-1.1.9/
--rw-r--r--   0 junquan   (1000) junquan   (1000)     1073 2023-03-21 08:05:20.000000 jcmutils-1.1.9/LICENSE
--rw-r--r--   0 junquan   (1000) junquan   (1000)      332 2023-03-23 08:31:41.312073 jcmutils-1.1.9/PKG-INFO
--rw-r--r--   0 junquan   (1000) junquan   (1000)     3044 2023-03-23 02:43:21.000000 jcmutils-1.1.9/README.md
-drwxr-xr-x   0 junquan   (1000) junquan   (1000)        0 2023-03-23 08:31:41.312073 jcmutils-1.1.9/jcmutils/
--rw-r--r--   0 junquan   (1000) junquan   (1000)      130 2023-03-22 11:53:40.000000 jcmutils-1.1.9/jcmutils/__init__.py
--rw-r--r--   0 junquan   (1000) junquan   (1000)     2151 2023-03-23 01:22:06.000000 jcmutils-1.1.9/jcmutils/gen_sources.py
--rw-r--r--   0 junquan   (1000) junquan   (1000)     1496 2023-03-22 11:53:40.000000 jcmutils-1.1.9/jcmutils/logger.py
--rw-r--r--   0 junquan   (1000) junquan   (1000)     8148 2023-03-23 08:30:52.000000 jcmutils-1.1.9/jcmutils/solver.py
-drwxr-xr-x   0 junquan   (1000) junquan   (1000)        0 2023-03-23 08:31:41.312073 jcmutils-1.1.9/jcmutils.egg-info/
--rw-r--r--   0 junquan   (1000) junquan   (1000)      332 2023-03-23 08:31:41.000000 jcmutils-1.1.9/jcmutils.egg-info/PKG-INFO
--rw-r--r--   0 junquan   (1000) junquan   (1000)      268 2023-03-23 08:31:41.000000 jcmutils-1.1.9/jcmutils.egg-info/SOURCES.txt
--rw-r--r--   0 junquan   (1000) junquan   (1000)        1 2023-03-23 08:31:41.000000 jcmutils-1.1.9/jcmutils.egg-info/dependency_links.txt
--rw-r--r--   0 junquan   (1000) junquan   (1000)       17 2023-03-23 08:31:41.000000 jcmutils-1.1.9/jcmutils.egg-info/requires.txt
--rw-r--r--   0 junquan   (1000) junquan   (1000)        9 2023-03-23 08:31:41.000000 jcmutils-1.1.9/jcmutils.egg-info/top_level.txt
--rw-r--r--   0 junquan   (1000) junquan   (1000)       38 2023-03-23 08:31:41.312073 jcmutils-1.1.9/setup.cfg
--rw-r--r--   0 junquan   (1000) junquan   (1000)      514 2023-03-23 08:31:21.000000 jcmutils-1.1.9/setup.py
+drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-04-15 13:23:04.124179 jcmutils-1.2.0/
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     1073 2023-04-15 12:55:54.000000 jcmutils-1.2.0/LICENSE
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      332 2023-04-15 13:23:04.124179 jcmutils-1.2.0/PKG-INFO
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     3044 2023-04-15 12:55:54.000000 jcmutils-1.2.0/README.md
+drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-04-15 13:23:04.124179 jcmutils-1.2.0/jcmutils/
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      130 2023-04-15 12:55:54.000000 jcmutils-1.2.0/jcmutils/__init__.py
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     2151 2023-04-15 12:55:54.000000 jcmutils-1.2.0/jcmutils/gen_sources.py
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     1496 2023-04-15 12:55:54.000000 jcmutils-1.2.0/jcmutils/logger.py
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     9093 2023-04-15 13:13:52.000000 jcmutils-1.2.0/jcmutils/solver.py
+drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-04-15 13:23:04.124179 jcmutils-1.2.0/jcmutils.egg-info/
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      332 2023-04-15 13:23:04.000000 jcmutils-1.2.0/jcmutils.egg-info/PKG-INFO
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      268 2023-04-15 13:23:04.000000 jcmutils-1.2.0/jcmutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)        1 2023-04-15 13:23:04.000000 jcmutils-1.2.0/jcmutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)       17 2023-04-15 13:23:04.000000 jcmutils-1.2.0/jcmutils.egg-info/requires.txt
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)        9 2023-04-15 13:23:04.000000 jcmutils-1.2.0/jcmutils.egg-info/top_level.txt
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)       38 2023-04-15 13:23:04.124179 jcmutils-1.2.0/setup.cfg
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      514 2023-04-15 13:15:27.000000 jcmutils-1.2.0/setup.py
```

### Comparing `jcmutils-1.1.9/LICENSE` & `jcmutils-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jcmutils-1.1.9/README.md` & `jcmutils-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `jcmutils-1.1.9/jcmutils/gen_sources.py` & `jcmutils-1.2.0/jcmutils/gen_sources.py`

 * *Files identical despite different names*

### Comparing `jcmutils-1.1.9/jcmutils/logger.py` & `jcmutils-1.2.0/jcmutils/logger.py`

 * *Files identical despite different names*

### Comparing `jcmutils-1.1.9/jcmutils/solver.py` & `jcmutils-1.2.0/jcmutils/solver.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,18 +11,20 @@
         # 初始化成员变量
         self.jcmp_path = jcmp_path
         self.keys = keys
         if os.path.isabs(database_path):
             abs_resultbag_dir = database_path
         else:
             abs_resultbag_dir = os.path.join(os.getcwd(), database_path)
+        if not os.path.exists(os.path.dirname(database_path)):
+            os.makedirs(os.path.dirname(database_path))
         self.resultbag = jcmwave.Resultbag(abs_resultbag_dir)
         self.has_inited = True
         logger.info("solver inited")
-        logger.debug(f"solver parameters:jcmp_path-{jcmp_path};database_path-{jcmp_path}")
+        logger.debug(f"solver parameters:jcmp_path-{jcmp_path};database_path-{abs_resultbag_dir}")
 
     def solve(self):
         # 检查是否被以被初始化，若还未被初始化则报错
         try:
             if self.has_inited:
                 logger.debug("solver class have been inited")
         except NameError:
@@ -73,60 +75,68 @@
 
             # 如果出现了oom错误，替换队列，再次计算
             if not no_error:
                 waiting_keys = backup_keys
 
         logger.info("analyse complete ! No error report ! solve mission done!!")
 
-    def show_image(self, key, num_of_result, is_light_intense=False):
+    def show_image(self, key, num_of_result, is_light_intense=False,vmax=None):
         if not self.resultbag.check_result(key):
             logger.error("get result failed! target key not find")
             logger.error(f"the key is : {key}")
             return -1
 
         # 开始提取
         result = self.resultbag.get_result(key)
         field = (result[num_of_result]['field'][0].conj() *
                  result[num_of_result]['field'][0]).sum(axis=2).real
         if is_light_intense:
             field = np.power(field, 2)
         plt.cla()
         plt.axis('square')
         plt.axis('off')
-        plt.pcolormesh(field[num_of_result]['X'], field[num_of_result]['Y'],
+        if(vmax is None):
+            plt.pcolormesh(field[num_of_result]['X'], field[num_of_result]['Y'],
                        field, shading='gouraud', cmap='gray')
+        else:
+            plt.pcolormesh(field[num_of_result]['X'], field[num_of_result]['Y'],
+                       field, shading='gouraud', cmap='gray',vmax=vmax)
         plt.show()
 
     def get_result(self, key):
         return self.resultbag.get_result(key)
 
-    def save_image(self, target_directory, key, num_of_result, is_light_intense=False):
+    def save_image(self, target_directory, key, num_of_result, is_light_intense=False,vmax=None):
         if not self.resultbag.check_result(key):
             logger.error("get result failed! target key not find")
             logger.error(f"the key is : {key}")
             return -1
 
         # 开始提取
         result = self.resultbag.get_result(key)
         field = (result[num_of_result]['field'][0].conj() *
                  result[num_of_result]['field'][0]).sum(axis=2).real
         if is_light_intense:
             field = np.power(field, 2)
         if not os.path.exists(target_directory):
             logger.debug("target directory dosen't exist,creating...")
-            os.mkdir(target_directory)
+            os.makedirs(target_directory)
         plt.cla()
-        plt.pcolormesh(field[num_of_result]['X'], field[num_of_result]['Y'],
+        if(vmax is None):
+            plt.pcolormesh(field[num_of_result]['X'], field[num_of_result]['Y'],
                        field, shading='gouraud', cmap='gray')
+        else:
+            plt.pcolormesh(field[num_of_result]['X'], field[num_of_result]['Y'],
+                       field, shading='gouraud', cmap='gray',vmax=vmax)
         plt.axis('square')
         plt.axis('off')
         plt.savefig(target_directory.rstrip("/") + "output.jpg",
                     bbox_inches='tight', pad_inches=0)
 
-    def save_all_image(self, num_of_result, target_directory, is_light_intense=False, is_symmetry=False):
+    def save_all_image(self, num_of_result, target_directory, is_light_intense=False, is_symmetry=False,vmax=None):
         if not self.resultbag.check_result(self.keys[0]):
             logger.error("get result failed! target key not find")
             logger.error(f"the key is : {self.keys[0]}")
             return -1
 
         # 开始提取
         # 先确定total_result的形状
@@ -143,15 +153,15 @@
                      result[num_of_result]['field'][0]).sum(axis=2).real
             if is_light_intense:
                 field = np.power(field, 2)
             total_results += field
 
             if not os.path.exists(target_directory):
                 logger.debug("target directory dosen't exist,creating...")
-                os.mkdir(target_directory)
+                os.makedirs(target_directory)
             file_name = target_directory.rstrip(
                 '/') + '/' + self.__solve_dict(key) + ".jpg"
             plt.cla()
             plt.pcolormesh(result[num_of_result]['X'], result[num_of_result]['Y'],
                            field, shading='gouraud', cmap='gray')
             plt.axis('square')
             plt.axis('off')
@@ -159,16 +169,21 @@
             logger.debug(f"key {key} successfully saved")
             if is_symmetry and not (key['thetaphi'][0] == 0 and key['thetaphi'][1] == 0):
                 field = np.rot90(field, 2)
                 total_results += field
                 logger.debug("key was rotated for symmetry")
 
         plt.cla()
-        plt.pcolormesh(temp_result[num_of_result]['X'], temp_result[num_of_result]['Y'],
+        if(vmax is None):
+            plt.pcolormesh(temp_result[num_of_result]['X'], temp_result[num_of_result]['Y'],
                        total_results, shading='gouraud', cmap='gray')
+        else:
+            plt.pcolormesh(temp_result[num_of_result]['X'], temp_result[num_of_result]['Y'],
+                       total_results, shading='gouraud', cmap='gray',vmax=vmax)
+        logger.debug(f"printing max value of results:{max(total_results)}")
         plt.axis('square')
         plt.axis('off')
         file_name = target_directory.rstrip('/') + '/' + "total_result.jpg"
         plt.savefig(file_name, bbox_inches='tight', pad_inches=0)
         logger.info("all target image saved completed!")
 
     def __solve_dict(self, target_dict):
@@ -186,8 +201,10 @@
         res.rstrip('-')
         return res
 
     def move_total_results(self,root_dir,target_dir):
         filelist = os.listdir(root_dir)
         for file in filelist:
             if file == "total_result.jpg":
+                if not os.path.exists(target_dir):
+                    os.makedirs(target_dir)
                 shutil.copyfile(os.path.join(root_dir,file),os.path.join(target_dir,os.path.basename(root_dir) + ".jpg"))
```

### Comparing `jcmutils-1.1.9/setup.py` & `jcmutils-1.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup,find_packages
 
-VERSION = '1.1.9'
+VERSION = '1.2.0'
 DESCRIPTION = "A general utils for jcmsuite"
 
 setup(
     name="jcmutils",
     version=VERSION,
     author="crafter-z",
     author_email="crafterz@163.com",
```

