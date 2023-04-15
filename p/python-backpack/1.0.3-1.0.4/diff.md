# Comparing `tmp/python-backpack-1.0.3.tar.gz` & `tmp/python-backpack-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-backpack-1.0.3.tar", last modified: Sun Jul 24 18:33:46 2022, max compression
+gzip compressed data, was "python-backpack-1.0.4.tar", last modified: Sat Apr 15 02:51:05 2023, max compression
```

## Comparing `python-backpack-1.0.3.tar` & `python-backpack-1.0.4.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2022-07-24 18:33:46.492972 python-backpack-1.0.3/
--rw-rw-rw-   0        0        0    35823 2022-07-19 16:09:57.000000 python-backpack-1.0.3/LICENSE
--rw-rw-rw-   0        0        0       19 2021-03-12 21:28:06.000000 python-backpack-1.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     2244 2022-07-24 18:33:46.492972 python-backpack-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1577 2022-07-24 17:23:38.000000 python-backpack-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2022-07-24 18:33:46.473971 python-backpack-1.0.3/backpack/
--rw-rw-rw-   0        0        0        0 2022-07-03 20:54:02.000000 python-backpack-1.0.3/backpack/__init__.py
--rw-rw-rw-   0        0        0     1275 2022-07-19 17:22:54.000000 python-backpack-1.0.3/backpack/custom_errors.py
--rw-rw-rw-   0        0        0     2483 2022-07-23 02:55:46.000000 python-backpack-1.0.3/backpack/file_utils.py
--rw-rw-rw-   0        0        0     2957 2022-07-20 01:30:36.000000 python-backpack-1.0.3/backpack/folder_utils.py
--rw-rw-rw-   0        0        0     5108 2022-07-24 17:39:20.000000 python-backpack-1.0.3/backpack/json_metadata.py
--rw-rw-rw-   0        0        0     2484 2022-07-24 18:15:38.000000 python-backpack-1.0.3/backpack/json_user_settings.py
--rw-rw-rw-   0        0        0     1227 2022-07-24 18:24:48.000000 python-backpack-1.0.3/backpack/json_utils.py
--rw-rw-rw-   0        0        0      464 2022-07-19 23:08:20.000000 python-backpack-1.0.3/backpack/logger.py
--rw-rw-rw-   0        0        0      848 2022-07-23 17:23:26.000000 python-backpack-1.0.3/backpack/patterns.py
--rw-rw-rw-   0        0        0     2235 2022-07-19 21:17:47.000000 python-backpack-1.0.3/backpack/strings.py
--rw-rw-rw-   0        0        0     1135 2022-07-20 15:08:27.000000 python-backpack-1.0.3/backpack/test_utils.py
--rw-rw-rw-   0        0        0      466 2022-07-24 18:33:25.000000 python-backpack-1.0.3/backpack/version.py
-drwxrwxrwx   0        0        0        0 2022-07-24 18:33:46.485971 python-backpack-1.0.3/python_backpack.egg-info/
--rw-rw-rw-   0        0        0     2244 2022-07-24 18:33:46.000000 python-backpack-1.0.3/python_backpack.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      708 2022-07-24 18:33:46.000000 python-backpack-1.0.3/python_backpack.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-24 18:33:46.000000 python-backpack-1.0.3/python_backpack.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2022-07-24 18:33:46.000000 python-backpack-1.0.3/python_backpack.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-07-24 18:33:46.492972 python-backpack-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1254 2022-07-19 16:43:51.000000 python-backpack-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2022-07-24 18:33:46.491971 python-backpack-1.0.3/tests/
--rw-rw-rw-   0        0        0        0 2021-01-19 15:17:59.000000 python-backpack-1.0.3/tests/__init__.py
--rw-rw-rw-   0        0        0     1580 2022-07-23 02:07:10.000000 python-backpack-1.0.3/tests/test_errors.py
--rw-rw-rw-   0        0        0     1836 2022-07-23 17:36:37.000000 python-backpack-1.0.3/tests/test_file_utils.py
--rw-rw-rw-   0        0        0     3123 2022-07-23 02:34:06.000000 python-backpack-1.0.3/tests/test_folder_utils.py
--rw-rw-rw-   0        0        0     2032 2022-07-24 18:19:09.000000 python-backpack-1.0.3/tests/test_json_user_settings.py
--rw-rw-rw-   0        0        0     1616 2022-07-24 18:25:31.000000 python-backpack-1.0.3/tests/test_json_utils.py
--rw-rw-rw-   0        0        0     2546 2022-07-24 18:14:15.000000 python-backpack-1.0.3/tests/test_jsonmd.py
--rw-rw-rw-   0        0        0     1675 2022-07-23 17:21:54.000000 python-backpack-1.0.3/tests/test_misc.py
--rw-rw-rw-   0        0        0     2526 2022-07-19 21:16:08.000000 python-backpack-1.0.3/tests/test_strings.py
--rw-rw-rw-   0        0        0     1191 2022-07-20 15:08:43.000000 python-backpack-1.0.3/tests/test_test_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-15 02:51:05.762869 python-backpack-1.0.4/
+-rw-rw-rw-   0        0        0    35823 2022-07-19 16:09:57.000000 python-backpack-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0       19 2021-03-12 21:28:06.000000 python-backpack-1.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     2335 2023-04-15 02:51:05.761868 python-backpack-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1616 2023-04-14 23:58:08.000000 python-backpack-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-15 02:51:05.737869 python-backpack-1.0.4/backpack/
+-rw-rw-rw-   0        0        0        0 2022-07-03 20:54:02.000000 python-backpack-1.0.4/backpack/__init__.py
+-rw-rw-rw-   0        0        0     1275 2022-07-19 17:22:54.000000 python-backpack-1.0.4/backpack/custom_errors.py
+-rw-rw-rw-   0        0        0     2483 2022-07-23 02:55:46.000000 python-backpack-1.0.4/backpack/file_utils.py
+-rw-rw-rw-   0        0        0     2957 2022-07-20 01:30:36.000000 python-backpack-1.0.4/backpack/folder_utils.py
+-rw-rw-rw-   0        0        0     5108 2022-07-24 17:39:20.000000 python-backpack-1.0.4/backpack/json_metadata.py
+-rw-rw-rw-   0        0        0     2484 2023-04-15 02:37:12.000000 python-backpack-1.0.4/backpack/json_user_settings.py
+-rw-rw-rw-   0        0        0     1227 2022-07-24 18:24:48.000000 python-backpack-1.0.4/backpack/json_utils.py
+-rw-rw-rw-   0        0        0      464 2022-07-19 23:08:20.000000 python-backpack-1.0.4/backpack/logger.py
+-rw-rw-rw-   0        0        0      848 2022-07-23 17:23:26.000000 python-backpack-1.0.4/backpack/patterns.py
+-rw-rw-rw-   0        0        0     3289 2023-04-15 02:16:46.000000 python-backpack-1.0.4/backpack/strings.py
+-rw-rw-rw-   0        0        0     1135 2022-07-20 15:08:27.000000 python-backpack-1.0.4/backpack/test_utils.py
+-rw-rw-rw-   0        0        0      523 2023-04-14 23:50:49.000000 python-backpack-1.0.4/backpack/version.py
+drwxrwxrwx   0        0        0        0 2023-04-15 02:51:05.751869 python-backpack-1.0.4/python_backpack.egg-info/
+-rw-rw-rw-   0        0        0     2335 2023-04-15 02:51:05.000000 python-backpack-1.0.4/python_backpack.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      708 2023-04-15 02:51:05.000000 python-backpack-1.0.4/python_backpack.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 02:51:05.000000 python-backpack-1.0.4/python_backpack.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-04-15 02:51:05.000000 python-backpack-1.0.4/python_backpack.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-15 02:51:05.762869 python-backpack-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1305 2023-04-15 02:50:08.000000 python-backpack-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 02:51:05.760869 python-backpack-1.0.4/tests/
+-rw-rw-rw-   0        0        0        0 2021-01-19 15:17:59.000000 python-backpack-1.0.4/tests/__init__.py
+-rw-rw-rw-   0        0        0     1580 2022-07-23 02:07:10.000000 python-backpack-1.0.4/tests/test_errors.py
+-rw-rw-rw-   0        0        0     1836 2022-07-23 17:36:37.000000 python-backpack-1.0.4/tests/test_file_utils.py
+-rw-rw-rw-   0        0        0     3123 2022-07-23 02:34:06.000000 python-backpack-1.0.4/tests/test_folder_utils.py
+-rw-rw-rw-   0        0        0     2224 2023-04-15 02:45:26.000000 python-backpack-1.0.4/tests/test_json_user_settings.py
+-rw-rw-rw-   0        0        0     1616 2022-07-24 18:25:31.000000 python-backpack-1.0.4/tests/test_json_utils.py
+-rw-rw-rw-   0        0        0     2546 2022-07-24 18:14:15.000000 python-backpack-1.0.4/tests/test_jsonmd.py
+-rw-rw-rw-   0        0        0     1675 2022-07-23 17:21:54.000000 python-backpack-1.0.4/tests/test_misc.py
+-rw-rw-rw-   0        0        0     3704 2023-04-15 02:13:42.000000 python-backpack-1.0.4/tests/test_strings.py
+-rw-rw-rw-   0        0        0     1191 2022-07-20 15:08:43.000000 python-backpack-1.0.4/tests/test_test_utils.py
```

### Comparing `python-backpack-1.0.3/LICENSE` & `python-backpack-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `python-backpack-1.0.3/PKG-INFO` & `python-backpack-1.0.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: python-backpack
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python Utilities for json/files/strings/errors
 Home-page: https://github.com/MaxRocamora/python-backpack
 Author: Maximiliano Rocamora
 Author-email: maxirocamora@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: Freely Distributable
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -45,24 +46,25 @@
 + file_is_writeable()
 
 ## String Validation
 + reformat_input_string()
 + begin_or_end_with_numbers()
 + begin_with_number()
 + has_numbers()
++ camelcase_to_snakecase()
 
 ## Custom Errors
 + EnvironmentVariableNotFound()
 + ApplicationNotFound()
 
 ## Test Utils
 + time_function_decorator()
 + random_string()
 
-## Others
+## Others / Patterns
 + Singleton()
 
 ---
 
 ### pip install
 pip install python-backpack
```

### Comparing `python-backpack-1.0.3/README.md` & `python-backpack-1.0.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -26,24 +26,25 @@
 + file_is_writeable()
 
 ## String Validation
 + reformat_input_string()
 + begin_or_end_with_numbers()
 + begin_with_number()
 + has_numbers()
++ camelcase_to_snakecase()
 
 ## Custom Errors
 + EnvironmentVariableNotFound()
 + ApplicationNotFound()
 
 ## Test Utils
 + time_function_decorator()
 + random_string()
 
-## Others
+## Others / Patterns
 + Singleton()
 
 ---
 
 ### pip install
 pip install python-backpack
```

### Comparing `python-backpack-1.0.3/backpack/custom_errors.py` & `python-backpack-1.0.4/backpack/custom_errors.py`

 * *Files identical despite different names*

### Comparing `python-backpack-1.0.3/backpack/file_utils.py` & `python-backpack-1.0.4/backpack/file_utils.py`

 * *Files identical despite different names*

### Comparing `python-backpack-1.0.3/backpack/folder_utils.py` & `python-backpack-1.0.4/backpack/folder_utils.py`

 * *Files identical despite different names*

### Comparing `python-backpack-1.0.3/backpack/json_metadata.py` & `python-backpack-1.0.4/backpack/json_metadata.py`

 * *Files identical despite different names*

### Comparing `python-backpack-1.0.3/backpack/json_user_settings.py` & `python-backpack-1.0.4/backpack/json_user_settings.py`

 * *Files identical despite different names*

### Comparing `python-backpack-1.0.3/backpack/json_utils.py` & `python-backpack-1.0.4/backpack/json_utils.py`

 * *Files identical despite different names*

### Comparing `python-backpack-1.0.3/backpack/patterns.py` & `python-backpack-1.0.4/backpack/patterns.py`

 * *Files identical despite different names*

### Comparing `python-backpack-1.0.3/backpack/test_utils.py` & `python-backpack-1.0.4/backpack/test_utils.py`

 * *Files identical despite different names*

### Comparing `python-backpack-1.0.3/python_backpack.egg-info/PKG-INFO` & `python-backpack-1.0.4/python_backpack.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: python-backpack
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python Utilities for json/files/strings/errors
 Home-page: https://github.com/MaxRocamora/python-backpack
 Author: Maximiliano Rocamora
 Author-email: maxirocamora@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: Freely Distributable
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -45,24 +46,25 @@
 + file_is_writeable()
 
 ## String Validation
 + reformat_input_string()
 + begin_or_end_with_numbers()
 + begin_with_number()
 + has_numbers()
++ camelcase_to_snakecase()
 
 ## Custom Errors
 + EnvironmentVariableNotFound()
 + ApplicationNotFound()
 
 ## Test Utils
 + time_function_decorator()
 + random_string()
 
-## Others
+## Others / Patterns
 + Singleton()
 
 ---
 
 ### pip install
 pip install python-backpack
```

### Comparing `python-backpack-1.0.3/python_backpack.egg-info/SOURCES.txt` & `python-backpack-1.0.4/python_backpack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-backpack-1.0.3/setup.py` & `python-backpack-1.0.4/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -23,13 +23,14 @@
     url='https://github.com/MaxRocamora/python-backpack',
     license='GNU GENERAL PUBLIC LICENSE',
     packages=find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "License :: Freely Distributable",
         "Operating System :: OS Independent",
         "Intended Audience :: Developers",
     ],
     python_requires='>=3.7'
 )
```

### Comparing `python-backpack-1.0.3/tests/test_errors.py` & `python-backpack-1.0.4/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `python-backpack-1.0.3/tests/test_file_utils.py` & `python-backpack-1.0.4/tests/test_file_utils.py`

 * *Files identical despite different names*

### Comparing `python-backpack-1.0.3/tests/test_folder_utils.py` & `python-backpack-1.0.4/tests/test_folder_utils.py`

 * *Files identical despite different names*

### Comparing `python-backpack-1.0.3/tests/test_json_user_settings.py` & `python-backpack-1.0.4/tests/test_json_user_settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,16 +13,15 @@
 
 mod_path = os.path.dirname(__file__)
 if mod_path not in sys.path:
     sys.path.append(mod_path)
 
 
 # test path & name
-FOLDER = 'tox_user_setting'
-NAME = 'test'
+FOLDER = 'tox_test_folder'
 TEST_FOLDER = os.path.join(os.path.expanduser('~'), FOLDER)
 
 
 class Test_windows(unittest.TestCase):
 
     @classmethod
     def setUp(cls):
@@ -34,39 +33,44 @@
     def tearDownClass(cls):
         # remove test files
         with contextlib.suppress(OSError):
             os.remove(TEST_FOLDER)
 
     def test_json_user_settings(self):
 
+        # make sure folder does not exist
+        with contextlib.suppress(PermissionError, OSError):
+            if os.path.exists(TEST_FOLDER):
+                os.removedirs(TEST_FOLDER)
+
         # class and properties
-        js = JsonUserSettings(NAME, FOLDER)
-        assert(js.filepath)
-        assert(os.path.exists(js.os_user_folder))
-        assert(isinstance(js.user_data, dict))
+        js = JsonUserSettings(FOLDER, 'user')
+        assert (js.filepath)
+        assert (os.path.exists(js.os_user_folder))
+        assert (isinstance(js.user_data, dict))
 
         # load from a missing file
         js.filename = 'random_file'
         self.assertFalse(js.load_settings())
 
     def test_json_settings_save(self):
         ''' test json settings: save '''
 
         # save a setting
-        js = JsonUserSettings(NAME, 'tox')
+        js = JsonUserSettings(FOLDER, 'tox')
         data = {'age': 99}
-        assert(js.save_settings(data))
+        assert (js.save_settings(data))
 
         # load it back
-        js = JsonUserSettings(NAME, 'tox')
+        js = JsonUserSettings(FOLDER, 'tox')
         data = js.load_settings()
-        assert(data['age'] == 99)
+        assert (data['age'] == 99)
         # save custom setting
         js.user_data = {'custom': 'value'}
-        assert(js.save_settings())
+        assert (js.save_settings())
         # load it back
         data = js.load_settings()
-        assert(data['custom'] == 'value')
+        assert (data['custom'] == 'value')
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `python-backpack-1.0.3/tests/test_json_utils.py` & `python-backpack-1.0.4/tests/test_json_utils.py`

 * *Files identical despite different names*

### Comparing `python-backpack-1.0.3/tests/test_jsonmd.py` & `python-backpack-1.0.4/tests/test_jsonmd.py`

 * *Files identical despite different names*

### Comparing `python-backpack-1.0.3/tests/test_misc.py` & `python-backpack-1.0.4/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `python-backpack-1.0.3/tests/test_strings.py` & `python-backpack-1.0.4/tests/test_strings.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # ----------------------------------------------------------------------------------------
 
 import os
 import sys
 import unittest
 
 from backpack.strings import has_numbers, begin_with_number, begin_or_end_with_numbers
-from backpack.strings import reformat_input_string
+from backpack.strings import reformat_input_string, camelcase_to_snakecase
 
 
 mod_path = os.path.dirname(__file__)
 if mod_path not in sys.path:
     sys.path.append(mod_path)
 
 # Tests Constants
@@ -63,10 +63,32 @@
         self.assertEqual(reformat_input_string(REFORMAT_BOTH), REFORMAT_BOTH_RESULT)
         # only regex
         self.assertEqual(
             reformat_input_string(
                 REFORMAT_BOTH, under_spaces=False, under_hyphen=False), REFORMAT_BOTH
         )
 
+    def test_camelcase_to_snakecase(self):
+
+        # Test case 1: Input with no uppercase characters
+        input_str, expected_output = "nocamelcase", "nocamelcase"
+        self.assertEqual(camelcase_to_snakecase(input_str), expected_output)
+
+        # Test case 2: Input with single uppercase character
+        input_str, expected_output = "OneCamelCaseChar", "one_camel_case_char"
+        self.assertEqual(camelcase_to_snakecase(input_str), expected_output)
+
+        # Test case 3: Input with multiple uppercase characters
+        input_str, expected_output = "MultiCamelCaseString", "multi_camel_case_string"
+        self.assertEqual(camelcase_to_snakecase(input_str), expected_output)
+
+        # Test case 4: Input with leading and trailing underscores
+        input_str, expected_output = "_CamelCase_", "_camel_case_"
+        self.assertEqual(camelcase_to_snakecase(input_str), expected_output)
+
+        # Test case 5: Input with leading and trailing underscores and lowercase
+        input_str, expected_output = "_camel_Case_", "_camel_case_"
+        self.assertEqual(camelcase_to_snakecase(input_str), expected_output)
+
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `python-backpack-1.0.3/tests/test_test_utils.py` & `python-backpack-1.0.4/tests/test_test_utils.py`

 * *Files identical despite different names*

