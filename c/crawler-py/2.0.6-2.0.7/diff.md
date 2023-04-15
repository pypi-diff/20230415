# Comparing `tmp/crawler-py-2.0.6.tar.gz` & `tmp/crawler-py-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crawler-py-2.0.6.tar", last modified: Sat Oct 16 15:59:41 2021, max compression
+gzip compressed data, was "crawler-py-2.0.7.tar", last modified: Sat Apr 15 13:06:30 2023, max compression
```

## Comparing `crawler-py-2.0.6.tar` & `crawler-py-2.0.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 johann    (1000) johann    (1000)        0 2021-10-16 15:59:41.526882 crawler-py-2.0.6/
--rw-r--r--   0 johann    (1000) johann    (1000)    18047 2020-06-05 19:34:07.000000 crawler-py-2.0.6/LICENSE
--rw-r--r--   0 johann    (1000) johann    (1000)     1182 2021-10-16 15:59:41.526882 crawler-py-2.0.6/PKG-INFO
--rw-r--r--   0 johann    (1000) johann    (1000)      398 2020-06-05 19:34:07.000000 crawler-py-2.0.6/README.md
-drwxr-xr-x   0 johann    (1000) johann    (1000)        0 2021-10-16 15:59:41.526882 crawler-py-2.0.6/crawler_py.egg-info/
--rw-r--r--   0 johann    (1000) johann    (1000)     1182 2021-10-16 15:59:41.000000 crawler-py-2.0.6/crawler_py.egg-info/PKG-INFO
--rw-r--r--   0 johann    (1000) johann    (1000)      337 2021-10-16 15:59:41.000000 crawler-py-2.0.6/crawler_py.egg-info/SOURCES.txt
--rw-r--r--   0 johann    (1000) johann    (1000)        1 2021-10-16 15:59:41.000000 crawler-py-2.0.6/crawler_py.egg-info/dependency_links.txt
--rw-r--r--   0 johann    (1000) johann    (1000)        1 2021-10-16 15:59:41.000000 crawler-py-2.0.6/crawler_py.egg-info/not-zip-safe
--rw-r--r--   0 johann    (1000) johann    (1000)       39 2021-10-16 15:59:41.000000 crawler-py-2.0.6/crawler_py.egg-info/requires.txt
--rw-r--r--   0 johann    (1000) johann    (1000)       10 2021-10-16 15:59:41.000000 crawler-py-2.0.6/crawler_py.egg-info/top_level.txt
-drwxr-xr-x   0 johann    (1000) johann    (1000)        0 2021-10-16 15:59:41.526882 crawler-py-2.0.6/crawlerpy/
--rw-r--r--   0 johann    (1000) johann    (1000)      500 2020-06-05 19:34:07.000000 crawler-py-2.0.6/crawlerpy/__init__.py
--rw-r--r--   0 johann    (1000) johann    (1000)     3014 2021-10-15 23:02:43.000000 crawler-py-2.0.6/crawlerpy/dtc.py
--rw-r--r--   0 johann    (1000) johann    (1000)     1007 2020-06-05 19:34:07.000000 crawler-py-2.0.6/crawlerpy/sap.py
--rw-r--r--   0 johann    (1000) johann    (1000)     2269 2021-06-09 22:15:39.000000 crawler-py-2.0.6/crawlerpy/scmb.py
--rw-r--r--   0 johann    (1000) johann    (1000)      357 2020-06-05 19:34:07.000000 crawler-py-2.0.6/crawlerpy/util.py
--rw-r--r--   0 johann    (1000) johann    (1000)     3964 2021-10-16 15:58:21.000000 crawler-py-2.0.6/crawlerpy/vdm.py
--rw-r--r--   0 johann    (1000) johann    (1000)       38 2021-10-16 15:59:41.526882 crawler-py-2.0.6/setup.cfg
--rw-r--r--   0 johann    (1000) johann    (1000)      957 2021-10-16 13:58:52.000000 crawler-py-2.0.6/setup.py
+drwxr-xr-x   0 johann    (1000) johann    (1000)        0 2023-04-15 13:06:30.311706 crawler-py-2.0.7/
+-rw-r--r--   0 johann    (1000) johann    (1000)    18047 2020-06-05 19:34:07.000000 crawler-py-2.0.7/LICENSE
+-rw-r--r--   0 johann    (1000) johann    (1000)     1017 2023-04-15 13:06:30.311706 crawler-py-2.0.7/PKG-INFO
+-rw-r--r--   0 johann    (1000) johann    (1000)      398 2020-06-05 19:34:07.000000 crawler-py-2.0.7/README.md
+drwxr-xr-x   0 johann    (1000) johann    (1000)        0 2023-04-15 13:06:30.308373 crawler-py-2.0.7/crawler_py.egg-info/
+-rw-r--r--   0 johann    (1000) johann    (1000)     1017 2023-04-15 13:06:30.000000 crawler-py-2.0.7/crawler_py.egg-info/PKG-INFO
+-rw-r--r--   0 johann    (1000) johann    (1000)      337 2023-04-15 13:06:30.000000 crawler-py-2.0.7/crawler_py.egg-info/SOURCES.txt
+-rw-r--r--   0 johann    (1000) johann    (1000)        1 2023-04-15 13:06:30.000000 crawler-py-2.0.7/crawler_py.egg-info/dependency_links.txt
+-rw-r--r--   0 johann    (1000) johann    (1000)        1 2020-06-06 21:35:50.000000 crawler-py-2.0.7/crawler_py.egg-info/not-zip-safe
+-rw-r--r--   0 johann    (1000) johann    (1000)       39 2023-04-15 13:06:30.000000 crawler-py-2.0.7/crawler_py.egg-info/requires.txt
+-rw-r--r--   0 johann    (1000) johann    (1000)       10 2023-04-15 13:06:30.000000 crawler-py-2.0.7/crawler_py.egg-info/top_level.txt
+drwxr-xr-x   0 johann    (1000) johann    (1000)        0 2023-04-15 13:06:30.311706 crawler-py-2.0.7/crawlerpy/
+-rw-r--r--   0 johann    (1000) johann    (1000)      500 2020-06-05 19:34:07.000000 crawler-py-2.0.7/crawlerpy/__init__.py
+-rw-r--r--   0 johann    (1000) johann    (1000)     3189 2023-04-15 13:05:19.000000 crawler-py-2.0.7/crawlerpy/dtc.py
+-rw-r--r--   0 johann    (1000) johann    (1000)     1007 2020-06-05 19:34:07.000000 crawler-py-2.0.7/crawlerpy/sap.py
+-rw-r--r--   0 johann    (1000) johann    (1000)     2269 2020-06-05 19:34:07.000000 crawler-py-2.0.7/crawlerpy/scmb.py
+-rw-r--r--   0 johann    (1000) johann    (1000)      357 2020-06-05 19:34:07.000000 crawler-py-2.0.7/crawlerpy/util.py
+-rw-r--r--   0 johann    (1000) johann    (1000)     3893 2023-04-15 13:05:19.000000 crawler-py-2.0.7/crawlerpy/vdm.py
+-rw-r--r--   0 johann    (1000) johann    (1000)       38 2023-04-15 13:06:30.311706 crawler-py-2.0.7/setup.cfg
+-rw-r--r--   0 johann    (1000) johann    (1000)      957 2023-04-15 13:05:19.000000 crawler-py-2.0.7/setup.py
```

### Comparing `crawler-py-2.0.6/LICENSE` & `crawler-py-2.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `crawler-py-2.0.6/crawlerpy/dtc.py` & `crawler-py-2.0.7/crawlerpy/scmb.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,97 +1,68 @@
 # -*- coding: utf-8 -*-
-from html import unescape
-#from re import findall, I, U, DOTALL
 from bs4 import BeautifulSoup
-from bs4.element import NavigableString, Tag
+from html import unescape
 
 from crawlerpy import ArticleCrawler, ParseException
 from crawlerpy.sap import Article, Section, Data
 from crawlerpy.util import get
 
-LIEN_ACCUEIL = "http://danstonchat.com/latest.html"
-LIEN_ALEATOIRE = "http://danstonchat.com/random.html"
-LIEN_PAGE = "http://danstonchat.com/latest/{0}.html"
-LIEN_ARTICLE = "http://danstonchat.com/{0}.html"
-
-
-def parse_contenu(div):
-    t = div.find("h3")
-    titre=""
-    if t:
-        titre = "".join(t.find("a").find_all(text=True, recursive=False)).strip()
-    identifiant = "".join(div.get("class")).replace("item","").strip()
-    article = Article(identifiant)
-    section = Section("quote")
-    t=""
-    for e in div.find("div",attrs={"class":"item-content"}).find("a").children:
-        if e.name=="br":
-            section.add_content(Data("string",t))
-            t=""
-        elif e.name=="span":
-            for d in e.contents:
-                if type(d) == Tag:
-                    t = "<" + d.name + "> "
-                    break
-            else:
-                t = "".join(e.find_all(text=True, recursive=False)).strip()+" "
-        elif type(e)== NavigableString:
-            t+=e.string.strip()
-    section.add_content(Data("string",t))
-    article.add_section(section)
-    return article
+LIEN_ACCUEIL = "http://secouchermoinsbete.fr"
+LIEN_ALEATOIRE = "http://secouchermoinsbete.fr/random"
+LIEN_PAGE = "http://secouchermoinsbete.fr/?page={0}"
+LIEN_ARTICLE = "http://secouchermoinsbete.fr/{0}"
 
-def parse_page(text):
+
+def parse(text):
     try:
         reponse = []
         soup = BeautifulSoup(text, 'html.parser')
-        d = soup.find("div",attrs={"class":"items"})
-        for div in d.find_all("div", recursive=False):
-            reponse.append(parse_contenu(div))
+        articles = soup.find_all("article")
+        for article in articles:
+            if "anecdote" not in article.get("class"):
+                continue
+            header = article.find("header")
+            if header is None:  # if one article in the page
+                for cl in soup.find_all("section"):
+                    if cl.get("id") == "anecdote-item":
+                        container_lien = soup.find("section").find("h1")
+            else:  # many article in the page
+                container_lien = header.find("h1")
+            lien = container_lien.find("a").get("href").replace("/", "")
+            text = article.find("p").get_text().replace('En savoir plus', "").strip()
+            section = Section("anecdote")
+            section.add_content(Data("string", text))
+            article = Article(lien)
+            article.add_section(section)
+            reponse.append(article)
         return reponse
     except Exception as e:
         raise ParseException(e)
 
-def parse_article(text, id_):
-    try:
-        soup = BeautifulSoup(text, 'html.parser')
-        return parse_contenu(soup.find("div",attrs={"id":id_}))
-    except Exception as e:
-        raise ParseException(e)
 
-class DtcCrawler(ArticleCrawler):
-    """The implementation of DansTonChat crawler"""
+class ScmbCrawler(ArticleCrawler):
+    """The implementation of VieDeMerde crawler"""
     def __init__(self):
         ArticleCrawler.__init__(self)
 
-    def get_text(self, lien):
+    def __go(self, lien):
         code, text = get(lien)
         if code == 200:
             text = unescape(text)
-        return code, text
+            try:
+                return 200, parse(text)
+            except ParseException:
+                return 521, []
+            code = 200
+        return code, []
 
     def page(self, id_):
-        code, data = self.get_text(LIEN_PAGE.format(int(id_) + 1))
-        if code != 200:
-            return code, []
-        try:
-            return 200, parse_page(data)
-        except ParseException:
-            return 521, []
+        code, data = self.__go(LIEN_PAGE.format(int(id_) + 1))
+        return code, data
 
     def article(self, id_):
-        code, data = self.get_text(LIEN_ARTICLE.format(id_))
-        if code != 200:
-            return code, []
-        try:
-            return 200, parse_article(data, id_)
-        except ParseException:
-            return 521, []
+        code, data = self.__go(LIEN_ARTICLE.format(id_))
+        return code, data[0]
 
     def random(self):
-        code, data = self.get_text(LIEN_ALEATOIRE)
-        if code != 200:
-            return code, []
-        try:
-            return 200, parse_page(data)
-        except ParseException:
-            return 521, []
+        code, data = self.__go(LIEN_ALEATOIRE)
+        return code, data
```

### Comparing `crawler-py-2.0.6/crawlerpy/sap.py` & `crawler-py-2.0.7/crawlerpy/sap.py`

 * *Files identical despite different names*

### Comparing `crawler-py-2.0.6/crawlerpy/vdm.py` & `crawler-py-2.0.7/crawlerpy/vdm.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # -*- coding: utf-8 -*-
+import re
 from bs4 import BeautifulSoup
 from html import unescape
 
 from crawlerpy import ArticleCrawler, ParseException
 from crawlerpy.sap import Article, Section, Data
 from crawlerpy.util import get
 
@@ -53,18 +54,15 @@
     except Exception as e:
         raise ParseException(e)
 
 def parse_random(text):
     try:
         reponse = []
         soup = BeautifulSoup(text, 'html.parser')
-        for principale_div in soup.find_all("div"):
-            cl = principale_div.get("class")
-            if not (cl and "w-full" in cl):
-                continue
+        for principale_div in soup.find_all("div", class_=re.compile("^w-full lg")):
             for div in principale_div.find_all("article"):
                 for a in div.find_all("a"):
                     cl = a.get("class")
                     if cl and "block" in cl:
                         id_= a.get("href").replace("/article/", "").replace(".html", "")
                         citation = "".join(a.find_all(text=True, recursive=False)).strip()
                         break
```

### Comparing `crawler-py-2.0.6/setup.py` & `crawler-py-2.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='crawler-py',
-    version='2.0.6',
+    version='2.0.7',
     url='http://johann-lecocq.fr/informatique-detail---bibliotheque--crawlerpy.html',
     license='GNU GPL 2',
     author='Johann Lecocq',
     author_email='git-jo@johann-lecocq.fr',
     description='A web Crawler for DTC(dans ton chat), VDM(vie de merde) and SCMB(se coucher moins bete)',
     long_description=open('README_en.md').read(),
     long_description_content_type='text/markdown',
```

