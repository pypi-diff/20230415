# Comparing `tmp/plantao_noticias_b3-0.1.0.tar.gz` & `tmp/plantao_noticias_b3-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plantao_noticias_b3-0.1.0.tar", max compression
+gzip compressed data, was "plantao_noticias_b3-0.1.1.tar", max compression
```

## Comparing `plantao_noticias_b3-0.1.0.tar` & `plantao_noticias_b3-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1099 2023-04-15 02:12:06.277086 plantao_noticias_b3-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0       58 2023-04-15 02:09:32.757024 plantao_noticias_b3-0.1.0/plantao_noticias_b3/__init__.py
--rw-r--r--   0        0        0     1837 2023-04-15 02:10:56.999243 plantao_noticias_b3-0.1.0/plantao_noticias_b3/news_functions.py
--rw-r--r--   0        0        0      669 2023-04-15 02:22:21.834057 plantao_noticias_b3-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-14 20:41:18.690392 plantao_noticias_b3-0.1.0/README.md
--rw-r--r--   0        0        0      684 1970-01-01 00:00:00.000000 plantao_noticias_b3-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1099 2023-04-15 02:12:06.277086 plantao_noticias_b3-0.1.1/LICENSE.txt
+-rw-r--r--   0        0        0       58 2023-04-15 02:09:32.757024 plantao_noticias_b3-0.1.1/plantao_noticias_b3/__init__.py
+-rw-r--r--   0        0        0     1841 2023-04-15 03:48:42.558353 plantao_noticias_b3-0.1.1/plantao_noticias_b3/news_functions.py
+-rw-r--r--   0        0        0      669 2023-04-15 03:49:08.939337 plantao_noticias_b3-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-14 20:41:18.690392 plantao_noticias_b3-0.1.1/README.md
+-rw-r--r--   0        0        0      684 1970-01-01 00:00:00.000000 plantao_noticias_b3-0.1.1/PKG-INFO
```

### Comparing `plantao_noticias_b3-0.1.0/LICENSE.txt` & `plantao_noticias_b3-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plantao_noticias_b3-0.1.0/plantao_noticias_b3/news_functions.py` & `plantao_noticias_b3-0.1.1/plantao_noticias_b3/news_functions.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
         except:
             raise ValueError(
                 f"Date format '{date}' not valid. Please enter a valid format."
             )
     return datetime.date.today().strftime("%Y-%m-%d")
 
 
-def request_get_with_timeout(url: str, timeout_time: float):
+def request_get_with_timeout(url: str, timeout_time: float = 5):
     try:
         r = requests.get(url, timeout=timeout_time)
         if r.status_code == 200:
             return r
         r.raise_for_status()
     except requests.exceptions.Timeout:
         raise requests.exceptions.Timeout(
```

### Comparing `plantao_noticias_b3-0.1.0/pyproject.toml` & `plantao_noticias_b3-0.1.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "plantao-noticias-b3"
-version = "0.1.0"
+version = "0.1.1"
 description = "Wrapper básico e prático para ler notícias do plantão de notícias da B3"
 authors = ["renanmoretto <himynameisrenan@outlook.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "plantao_noticias_b3"}]
 repository = "https://github.com/renanmoretto/plantao_noticias_b3"
 keywords = ["b3", "plantao", "noticias", "bolsa", "plantao de noticias"]
```

### Comparing `plantao_noticias_b3-0.1.0/PKG-INFO` & `plantao_noticias_b3-0.1.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plantao-noticias-b3
-Version: 0.1.0
+Version: 0.1.1
 Summary: Wrapper básico e prático para ler notícias do plantão de notícias da B3
 Home-page: https://github.com/renanmoretto/plantao_noticias_b3
 License: MIT
 Keywords: b3,plantao,noticias,bolsa,plantao de noticias
 Author: renanmoretto
 Author-email: himynameisrenan@outlook.com
 Requires-Python: >=3.11,<4.0
```

