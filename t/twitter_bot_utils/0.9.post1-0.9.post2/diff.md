# Comparing `tmp/twitter_bot_utils-0.9.post1.tar.gz` & `tmp/twitter_bot_utils-0.9.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/twitter_bot_utils-0.9.post1.tar", last modified: Tue Jul 28 02:35:47 2015, max compression
+gzip compressed data, was "dist/twitter_bot_utils-0.9.post2.tar", last modified: Tue Jul 28 02:55:05 2015, max compression
```

## Comparing `twitter_bot_utils-0.9.post1.tar` & `twitter_bot_utils-0.9.post2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 neil       (501) _www        (70)        0 2015-07-28 02:35:47.000000 twitter_bot_utils-0.9.post1/
--rw-r--r--   0 neil       (501) _www        (70)    10660 2015-07-28 02:35:47.000000 twitter_bot_utils-0.9.post1/PKG-INFO
--rw-r--r--   0 neil       (501) _www        (70)       88 2015-07-28 02:35:47.000000 twitter_bot_utils-0.9.post1/setup.cfg
--rw-r--r--   0 neil       (501) _www        (70)      817 2015-07-28 02:35:37.000000 twitter_bot_utils-0.9.post1/setup.py
-drwxr-xr-x   0 neil       (501) _www        (70)        0 2015-07-28 02:35:47.000000 twitter_bot_utils-0.9.post1/twitter_bot_utils/
--rw-r--r--   0 neil       (501) _www        (70)      910 2015-07-28 02:35:29.000000 twitter_bot_utils-0.9.post1/twitter_bot_utils/__init__.py
--rw-r--r--   0 neil       (501) _www        (70)     3284 2015-07-27 19:41:03.000000 twitter_bot_utils-0.9.post1/twitter_bot_utils/api.py
--rw-r--r--   0 neil       (501) _www        (70)     1390 2014-12-18 20:19:06.000000 twitter_bot_utils-0.9.post1/twitter_bot_utils/archive.py
--rw-r--r--   0 neil       (501) _www        (70)     3194 2015-07-27 19:07:07.000000 twitter_bot_utils-0.9.post1/twitter_bot_utils/args.py
--rw-r--r--   0 neil       (501) _www        (70)     1896 2015-03-23 16:57:39.000000 twitter_bot_utils-0.9.post1/twitter_bot_utils/cli.py
--rw-r--r--   0 neil       (501) _www        (70)     4146 2015-07-27 19:41:04.000000 twitter_bot_utils-0.9.post1/twitter_bot_utils/confighelper.py
--rw-r--r--   0 neil       (501) _www        (70)     3771 2015-07-28 01:28:15.000000 twitter_bot_utils-0.9.post1/twitter_bot_utils/helpers.py
--rw-r--r--   0 neil       (501) _www        (70)     3183 2015-03-23 16:57:39.000000 twitter_bot_utils-0.9.post1/twitter_bot_utils/tools.py
-drwxr-xr-x   0 neil       (501) _www        (70)        0 2015-07-28 02:35:47.000000 twitter_bot_utils-0.9.post1/twitter_bot_utils.egg-info/
--rw-r--r--   0 neil       (501) _www        (70)        1 2015-07-28 02:35:46.000000 twitter_bot_utils-0.9.post1/twitter_bot_utils.egg-info/dependency_links.txt
--rw-r--r--   0 neil       (501) _www        (70)      135 2015-07-28 02:35:46.000000 twitter_bot_utils-0.9.post1/twitter_bot_utils.egg-info/entry_points.txt
--rw-r--r--   0 neil       (501) _www        (70)    10660 2015-07-28 02:35:46.000000 twitter_bot_utils-0.9.post1/twitter_bot_utils.egg-info/PKG-INFO
--rw-r--r--   0 neil       (501) _www        (70)       48 2015-07-28 02:35:46.000000 twitter_bot_utils-0.9.post1/twitter_bot_utils.egg-info/requires.txt
--rw-r--r--   0 neil       (501) _www        (70)      491 2015-07-28 02:35:46.000000 twitter_bot_utils-0.9.post1/twitter_bot_utils.egg-info/SOURCES.txt
--rw-r--r--   0 neil       (501) _www        (70)       18 2015-07-28 02:35:46.000000 twitter_bot_utils-0.9.post1/twitter_bot_utils.egg-info/top_level.txt
+drwxr-xr-x   0 neil       (501) _www        (70)        0 2015-07-28 02:55:05.000000 twitter_bot_utils-0.9.post2/
+-rw-r--r--   0 neil       (501) _www        (70)    10660 2015-07-28 02:55:05.000000 twitter_bot_utils-0.9.post2/PKG-INFO
+-rw-r--r--   0 neil       (501) _www        (70)       88 2015-07-28 02:55:05.000000 twitter_bot_utils-0.9.post2/setup.cfg
+-rw-r--r--   0 neil       (501) _www        (70)      907 2015-07-28 02:54:30.000000 twitter_bot_utils-0.9.post2/setup.py
+drwxr-xr-x   0 neil       (501) _www        (70)        0 2015-07-28 02:55:05.000000 twitter_bot_utils-0.9.post2/twitter_bot_utils/
+-rw-r--r--   0 neil       (501) _www        (70)      910 2015-07-28 02:54:46.000000 twitter_bot_utils-0.9.post2/twitter_bot_utils/__init__.py
+-rw-r--r--   0 neil       (501) _www        (70)     3284 2015-07-27 19:41:03.000000 twitter_bot_utils-0.9.post2/twitter_bot_utils/api.py
+-rw-r--r--   0 neil       (501) _www        (70)     1390 2014-12-18 20:19:06.000000 twitter_bot_utils-0.9.post2/twitter_bot_utils/archive.py
+-rw-r--r--   0 neil       (501) _www        (70)     3194 2015-07-27 19:07:07.000000 twitter_bot_utils-0.9.post2/twitter_bot_utils/args.py
+-rw-r--r--   0 neil       (501) _www        (70)     1896 2015-03-23 16:57:39.000000 twitter_bot_utils-0.9.post2/twitter_bot_utils/cli.py
+-rw-r--r--   0 neil       (501) _www        (70)     4146 2015-07-27 19:41:04.000000 twitter_bot_utils-0.9.post2/twitter_bot_utils/confighelper.py
+-rw-r--r--   0 neil       (501) _www        (70)     3771 2015-07-28 01:28:15.000000 twitter_bot_utils-0.9.post2/twitter_bot_utils/helpers.py
+-rw-r--r--   0 neil       (501) _www        (70)     3183 2015-03-23 16:57:39.000000 twitter_bot_utils-0.9.post2/twitter_bot_utils/tools.py
+drwxr-xr-x   0 neil       (501) _www        (70)        0 2015-07-28 02:55:05.000000 twitter_bot_utils-0.9.post2/twitter_bot_utils.egg-info/
+-rw-r--r--   0 neil       (501) _www        (70)        1 2015-07-28 02:55:04.000000 twitter_bot_utils-0.9.post2/twitter_bot_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 neil       (501) _www        (70)      135 2015-07-28 02:55:04.000000 twitter_bot_utils-0.9.post2/twitter_bot_utils.egg-info/entry_points.txt
+-rw-r--r--   0 neil       (501) _www        (70)    10660 2015-07-28 02:55:04.000000 twitter_bot_utils-0.9.post2/twitter_bot_utils.egg-info/PKG-INFO
+-rw-r--r--   0 neil       (501) _www        (70)       48 2015-07-28 02:55:04.000000 twitter_bot_utils-0.9.post2/twitter_bot_utils.egg-info/requires.txt
+-rw-r--r--   0 neil       (501) _www        (70)      491 2015-07-28 02:55:05.000000 twitter_bot_utils-0.9.post2/twitter_bot_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 neil       (501) _www        (70)       18 2015-07-28 02:55:04.000000 twitter_bot_utils-0.9.post2/twitter_bot_utils.egg-info/top_level.txt
```

### Comparing `twitter_bot_utils-0.9.post1/PKG-INFO` & `twitter_bot_utils-0.9.post2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: twitter_bot_utils
-Version: 0.9.post1
+Version: 0.9.post2
 Summary: Python utilities for twitter bots
 Home-page: http://github.com/fitnr/twitter_bot_utils
 Author: Neil Freeman
 Author-email: contact@fakeisthenewreal.org
 License: GPLv3
 Description: twitter bot utils
         =================
```

### Comparing `twitter_bot_utils-0.9.post1/twitter_bot_utils/__init__.py` & `twitter_bot_utils-0.9.post2/twitter_bot_utils/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,13 +8,13 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-__version__ = '0.9.post1'
+__version__ = '0.9.post2'
 __author__ = 'Neil Freeman'
 __license__ = 'GPLv3'
 __all__ = ['api', 'args', 'archive', 'confighelper', 'helpers', 'tools']
 
 from . import api, args, archive, confighelper, helpers, tools
```

### Comparing `twitter_bot_utils-0.9.post1/twitter_bot_utils/api.py` & `twitter_bot_utils-0.9.post2/twitter_bot_utils/api.py`

 * *Files identical despite different names*

### Comparing `twitter_bot_utils-0.9.post1/twitter_bot_utils/archive.py` & `twitter_bot_utils-0.9.post2/twitter_bot_utils/archive.py`

 * *Files identical despite different names*

### Comparing `twitter_bot_utils-0.9.post1/twitter_bot_utils/args.py` & `twitter_bot_utils-0.9.post2/twitter_bot_utils/args.py`

 * *Files identical despite different names*

### Comparing `twitter_bot_utils-0.9.post1/twitter_bot_utils/cli.py` & `twitter_bot_utils-0.9.post2/twitter_bot_utils/cli.py`

 * *Files identical despite different names*

### Comparing `twitter_bot_utils-0.9.post1/twitter_bot_utils/confighelper.py` & `twitter_bot_utils-0.9.post2/twitter_bot_utils/confighelper.py`

 * *Files identical despite different names*

### Comparing `twitter_bot_utils-0.9.post1/twitter_bot_utils/helpers.py` & `twitter_bot_utils-0.9.post2/twitter_bot_utils/helpers.py`

 * *Files identical despite different names*

### Comparing `twitter_bot_utils-0.9.post1/twitter_bot_utils/tools.py` & `twitter_bot_utils-0.9.post2/twitter_bot_utils/tools.py`

 * *Files identical despite different names*

### Comparing `twitter_bot_utils-0.9.post1/twitter_bot_utils.egg-info/PKG-INFO` & `twitter_bot_utils-0.9.post2/twitter_bot_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: twitter-bot-utils
-Version: 0.9.post1
+Version: 0.9.post2
 Summary: Python utilities for twitter bots
 Home-page: http://github.com/fitnr/twitter_bot_utils
 Author: Neil Freeman
 Author-email: contact@fakeisthenewreal.org
 License: GPLv3
 Description: twitter bot utils
         =================
```

