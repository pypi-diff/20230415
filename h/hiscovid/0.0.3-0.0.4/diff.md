# Comparing `tmp/hiscovid-0.0.3.tar.gz` & `tmp/hiscovid-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hiscovid-0.0.3.tar", last modified: Tue Mar 14 04:40:32 2023, max compression
+gzip compressed data, was "hiscovid-0.0.4.tar", last modified: Sat Apr 15 08:31:23 2023, max compression
```

## Comparing `hiscovid-0.0.3.tar` & `hiscovid-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-03-14 04:40:32.426534 hiscovid-0.0.3/
--rw-r--r--   0 yt        (1000) yt        (1000)     2040 2023-03-14 04:40:32.426534 hiscovid-0.0.3/PKG-INFO
--rw-r--r--   0 yt        (1000) yt        (1000)     1488 2022-05-05 10:27:54.000000 hiscovid-0.0.3/README.md
--rw-r--r--   0 yt        (1000) yt        (1000)       38 2023-03-14 04:40:32.426534 hiscovid-0.0.3/setup.cfg
--rw-r--r--   0 yt        (1000) yt        (1000)      972 2023-03-14 04:39:26.000000 hiscovid-0.0.3/setup.py
-drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-03-14 04:40:32.410651 hiscovid-0.0.3/src/
-drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-03-14 04:40:32.426534 hiscovid-0.0.3/src/hiscovid.egg-info/
--rw-r--r--   0 yt        (1000) yt        (1000)     2040 2023-03-14 04:40:31.000000 hiscovid-0.0.3/src/hiscovid.egg-info/PKG-INFO
--rw-r--r--   0 yt        (1000) yt        (1000)      217 2023-03-14 04:40:31.000000 hiscovid-0.0.3/src/hiscovid.egg-info/SOURCES.txt
--rw-r--r--   0 yt        (1000) yt        (1000)        1 2023-03-14 04:40:31.000000 hiscovid-0.0.3/src/hiscovid.egg-info/dependency_links.txt
--rw-r--r--   0 yt        (1000) yt        (1000)       44 2023-03-14 04:40:31.000000 hiscovid-0.0.3/src/hiscovid.egg-info/entry_points.txt
--rw-r--r--   0 yt        (1000) yt        (1000)        9 2023-03-14 04:40:31.000000 hiscovid-0.0.3/src/hiscovid.egg-info/top_level.txt
--rw-r--r--   0 yt        (1000) yt        (1000)     1945 2023-03-14 04:38:24.000000 hiscovid-0.0.3/src/hiscovid.py
+drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-04-15 08:31:23.347775 hiscovid-0.0.4/
+-rw-r--r--   0 yt        (1000) yt        (1000)     2040 2023-04-15 08:31:23.346536 hiscovid-0.0.4/PKG-INFO
+-rw-r--r--   0 yt        (1000) yt        (1000)     1488 2022-05-05 10:27:54.000000 hiscovid-0.0.4/README.md
+-rw-r--r--   0 yt        (1000) yt        (1000)       38 2023-04-15 08:31:23.347775 hiscovid-0.0.4/setup.cfg
+-rw-r--r--   0 yt        (1000) yt        (1000)      972 2023-04-15 08:30:16.000000 hiscovid-0.0.4/setup.py
+drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-04-15 08:31:23.339421 hiscovid-0.0.4/src/
+drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-04-15 08:31:23.346536 hiscovid-0.0.4/src/hiscovid.egg-info/
+-rw-r--r--   0 yt        (1000) yt        (1000)     2040 2023-04-15 08:31:22.000000 hiscovid-0.0.4/src/hiscovid.egg-info/PKG-INFO
+-rw-r--r--   0 yt        (1000) yt        (1000)      217 2023-04-15 08:31:22.000000 hiscovid-0.0.4/src/hiscovid.egg-info/SOURCES.txt
+-rw-r--r--   0 yt        (1000) yt        (1000)        1 2023-04-15 08:31:22.000000 hiscovid-0.0.4/src/hiscovid.egg-info/dependency_links.txt
+-rw-r--r--   0 yt        (1000) yt        (1000)       44 2023-04-15 08:31:22.000000 hiscovid-0.0.4/src/hiscovid.egg-info/entry_points.txt
+-rw-r--r--   0 yt        (1000) yt        (1000)        9 2023-04-15 08:31:22.000000 hiscovid-0.0.4/src/hiscovid.egg-info/top_level.txt
+-rw-r--r--   0 yt        (1000) yt        (1000)     1941 2023-04-15 08:29:35.000000 hiscovid-0.0.4/src/hiscovid.py
```

### Comparing `hiscovid-0.0.3/PKG-INFO` & `hiscovid-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hiscovid
-Version: 0.0.3
+Version: 0.0.4
 Summary: A package for calculating time transition policy scores against COVID-19
 Home-page: https://github.com/ytakefuji/hiscovid
 Author: yoshiyasu takefuji
 Author-email: takefuji@keio.jp
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ytakefuji/hiscovid
 Platform: UNKNOWN
```

### Comparing `hiscovid-0.0.3/README.md` & `hiscovid-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `hiscovid-0.0.3/setup.py` & `hiscovid-0.0.4/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="hiscovid",
-    version="0.0.3",
+    version="0.0.4",
     author="yoshiyasu takefuji",
     author_email="takefuji@keio.jp",
     description="A package for calculating time transition policy scores against COVID-19",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ytakefuji/hiscovid",
     project_urls={
```

### Comparing `hiscovid-0.0.3/src/hiscovid.egg-info/PKG-INFO` & `hiscovid-0.0.4/src/hiscovid.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hiscovid
-Version: 0.0.3
+Version: 0.0.4
 Summary: A package for calculating time transition policy scores against COVID-19
 Home-page: https://github.com/ytakefuji/hiscovid
 Author: yoshiyasu takefuji
 Author-email: takefuji@keio.jp
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ytakefuji/hiscovid
 Platform: UNKNOWN
```

### Comparing `hiscovid-0.0.3/src/hiscovid.py` & `hiscovid-0.0.4/src/hiscovid.py`

 * *Files 5% similar despite different names*

```diff
@@ -66,12 +66,12 @@
   i=pd.read_csv(countries[i]+'.csv') 
   plt.ylabel('score')
   plt.plot(i.date[0:-5],i.score[0:-5])
   plt.xticks(np.arange(0,days,30*days/770),rotation=90)
   fig=plt.figure(1)
   fig.set_size_inches(10,3)
  plt.legend(countries)
- plt.savefig('result.png',dpi=fig.dpi,bbox_inches='tight')
+ plt.savefig('result.png',dpi=300,bbox_inches='tight')
  plt.show()
 
 if __name__ == "__main__":
  main()
```

