# Comparing `tmp/pypub3-1.0.2.tar.gz` & `tmp/pypub3-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypub3-1.0.2.tar", last modified: Mon Nov 28 07:04:17 2022, max compression
+gzip compressed data, was "pypub3-2.0.0.tar", last modified: Fri Apr 14 23:32:56 2023, max compression
```

## Comparing `pypub3-1.0.2.tar` & `pypub3-2.0.0.tar`

### file list

```diff
@@ -1,39 +1,41 @@
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2022-11-28 07:04:16.995526 pypub3-1.0.2/
--rw-r--r--   0 andrew    (1000) andrew    (1000)     1075 2020-06-20 20:57:00.000000 pypub3-1.0.2/LICENSE
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     2840 2022-11-28 07:04:16.995526 pypub3-1.0.2/PKG-INFO
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     2384 2022-11-14 00:14:02.000000 pypub3-1.0.2/README.md
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2022-11-28 07:04:16.991526 pypub3-1.0.2/pypub/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      275 2020-06-21 22:02:44.000000 pypub3-1.0.2/pypub/__init__.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)    10452 2022-11-28 07:03:27.000000 pypub3-1.0.2/pypub/chapter.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     4824 2022-11-28 07:03:27.000000 pypub3-1.0.2/pypub/const.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     8636 2022-11-28 07:03:27.000000 pypub3-1.0.2/pypub/epub.py
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2022-11-28 07:04:16.991526 pypub3-1.0.2/pypub/static/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      232 2020-06-20 06:04:37.000000 pypub3-1.0.2/pypub/static/container.xml
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      627 2020-06-20 07:23:50.000000 pypub3-1.0.2/pypub/static/coverpage.xhtml
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2022-11-28 07:04:16.991526 pypub3-1.0.2/pypub/static/css/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)       85 2020-06-20 05:31:24.000000 pypub3-1.0.2/pypub/static/css/coverpage.css
--rw-rw-r--   0 andrew    (1000) andrew    (1000)        1 2020-06-21 09:05:48.000000 pypub3-1.0.2/pypub/static/css/styles.css
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2022-11-28 07:04:16.991526 pypub3-1.0.2/pypub/static/fonts/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)   592752 2022-11-14 00:13:49.000000 pypub3-1.0.2/pypub/static/fonts/free_mono.ttf
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2022-11-28 07:04:16.995526 pypub3-1.0.2/pypub/static/img/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)    88953 2022-11-14 00:13:49.000000 pypub3-1.0.2/pypub/static/img/cover.png
--rw-rw-r--   0 andrew    (1000) andrew    (1000)       20 2020-06-20 06:34:26.000000 pypub3-1.0.2/pypub/static/mimetype
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2022-11-28 07:04:16.995526 pypub3-1.0.2/pypub/templates/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      688 2020-06-20 07:07:49.000000 pypub3-1.0.2/pypub/templates/book.ncx.xml.j2
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     1908 2022-11-14 00:13:49.000000 pypub3-1.0.2/pypub/templates/book.opf.xml.j2
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      637 2022-11-14 00:13:49.000000 pypub3-1.0.2/pypub/templates/page.xhtml.xml.j2
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      598 2020-06-20 07:09:56.000000 pypub3-1.0.2/pypub/templates/toc.xhtml.xml.j2
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2022-11-28 07:04:16.995526 pypub3-1.0.2/pypub/tests/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)        0 2020-06-20 21:17:13.000000 pypub3-1.0.2/pypub/tests/__init__.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      137 2020-06-21 08:43:18.000000 pypub3-1.0.2/pypub/tests/__main__.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     3973 2022-11-28 07:03:27.000000 pypub3-1.0.2/pypub/tests/chapter_test.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     1266 2022-11-14 00:13:49.000000 pypub3-1.0.2/pypub/tests/epub_test.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     1148 2020-06-21 08:43:46.000000 pypub3-1.0.2/pypub/tests/profile_test.py
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2022-11-28 07:04:16.995526 pypub3-1.0.2/pypub3.egg-info/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     2840 2022-11-28 07:04:16.000000 pypub3-1.0.2/pypub3.egg-info/PKG-INFO
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      706 2022-11-28 07:04:16.000000 pypub3-1.0.2/pypub3.egg-info/SOURCES.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)        1 2022-11-28 07:04:16.000000 pypub3-1.0.2/pypub3.egg-info/dependency_links.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)       19 2022-11-28 07:04:16.000000 pypub3-1.0.2/pypub3.egg-info/requires.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)        6 2022-11-28 07:04:16.000000 pypub3-1.0.2/pypub3.egg-info/top_level.txt
--rw-r--r--   0 andrew    (1000) andrew    (1000)       79 2022-11-28 07:04:16.995526 pypub3-1.0.2/setup.cfg
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      935 2022-11-28 07:03:46.000000 pypub3-1.0.2/setup.py
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-04-14 23:32:56.120629 pypub3-2.0.0/
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     1075 2020-06-20 20:57:00.000000 pypub3-2.0.0/LICENSE
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     2043 2023-04-14 23:32:56.120629 pypub3-2.0.0/PKG-INFO
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     1587 2023-04-14 23:31:44.000000 pypub3-2.0.0/README.md
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-04-14 23:32:56.116629 pypub3-2.0.0/pypub/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      558 2023-04-14 23:31:44.000000 pypub3-2.0.0/pypub/__init__.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)    10259 2023-04-14 23:31:44.000000 pypub3-2.0.0/pypub/builder.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     6452 2023-04-14 23:31:44.000000 pypub3-2.0.0/pypub/chapter.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     2133 2023-04-14 23:31:44.000000 pypub3-2.0.0/pypub/epub.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     9221 2023-04-14 23:31:44.000000 pypub3-2.0.0/pypub/factory.py
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-04-14 23:32:56.116629 pypub3-2.0.0/pypub/static/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      232 2023-03-28 06:24:00.000000 pypub3-2.0.0/pypub/static/container.xml
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      627 2023-03-28 06:24:00.000000 pypub3-2.0.0/pypub/static/coverpage.xhtml
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-04-14 23:32:56.116629 pypub3-2.0.0/pypub/static/css/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)       85 2023-03-28 06:24:00.000000 pypub3-2.0.0/pypub/static/css/coverpage.css
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)        1 2023-03-28 06:24:00.000000 pypub3-2.0.0/pypub/static/css/styles.css
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-04-14 23:32:56.116629 pypub3-2.0.0/pypub/static/fonts/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)   592752 2023-03-28 06:24:00.000000 pypub3-2.0.0/pypub/static/fonts/free_mono.ttf
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-04-14 23:32:56.116629 pypub3-2.0.0/pypub/static/img/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)    88953 2023-03-28 06:24:00.000000 pypub3-2.0.0/pypub/static/img/cover.png
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)       20 2023-03-28 06:24:00.000000 pypub3-2.0.0/pypub/static/mimetype
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-04-14 23:32:56.116629 pypub3-2.0.0/pypub/templates/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      705 2023-04-14 23:31:44.000000 pypub3-2.0.0/pypub/templates/book.ncx.j2
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     1978 2023-04-14 23:31:44.000000 pypub3-2.0.0/pypub/templates/book.opf.j2
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      635 2023-04-14 23:31:44.000000 pypub3-2.0.0/pypub/templates/page.xhtml.j2
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      606 2023-04-14 23:31:44.000000 pypub3-2.0.0/pypub/templates/toc.xhtml.j2
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-04-14 23:32:56.116629 pypub3-2.0.0/pypub/tests/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      196 2023-04-14 23:31:44.000000 pypub3-2.0.0/pypub/tests/__init__.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      113 2023-04-14 23:31:44.000000 pypub3-2.0.0/pypub/tests/__main__.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     1272 2023-04-14 23:31:44.000000 pypub3-2.0.0/pypub/tests/chapter.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     1305 2023-04-14 23:31:44.000000 pypub3-2.0.0/pypub/tests/epub.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     3265 2023-04-14 23:31:44.000000 pypub3-2.0.0/pypub/tests/factory.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     1140 2023-04-14 23:31:44.000000 pypub3-2.0.0/pypub/tests/profile.py
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-04-14 23:32:56.120629 pypub3-2.0.0/pypub3.egg-info/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     2043 2023-04-14 23:32:56.000000 pypub3-2.0.0/pypub3.egg-info/PKG-INFO
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      707 2023-04-14 23:32:56.000000 pypub3-2.0.0/pypub3.egg-info/SOURCES.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)        1 2023-04-14 23:32:56.000000 pypub3-2.0.0/pypub3.egg-info/dependency_links.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)       33 2023-04-14 23:32:56.000000 pypub3-2.0.0/pypub3.egg-info/requires.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)        6 2023-04-14 23:32:56.000000 pypub3-2.0.0/pypub3.egg-info/top_level.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)       38 2023-04-14 23:32:56.120629 pypub3-2.0.0/setup.cfg
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      961 2023-04-14 23:32:03.000000 pypub3-2.0.0/setup.py
```

### Comparing `pypub3-1.0.2/LICENSE` & `pypub3-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pypub3-1.0.2/README.md` & `pypub3-2.0.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,44 +1,46 @@
-# Pypub 3 #
+pypub
+------
 
-Create epub's using Python. Pypub is a Python library to create epub files quickly, without having to worry about the intricacies of the epub specification.
+Create epub's using Python. 
+Pypub is a Python library to create epub files quickly, 
+without having to worry about the intricacies of the epub specification.
 
-This package was orignally forked and re-written based on [WCember's Python 2 version](https://github.com/wcember/pypub),
-but due to a lack of response has been re-released as a new package to support Python 3.
+This package was originally forked and re-written based on WCember's Python 2 
+version, but due to a lack of response has been re-released as a new package 
+to support Python 3.
 
-# Installation #
-The current release of pypub is available through pip:
+The codebase has since gone through a few substantial rewrites and operates 
+as its own library moving forward.
 
-    $ pip install pypub3
+### Installation
 
-Pypub3 is only compatible with Python <= 3.6.
+```
+pip install pypub3
+```
 
-# Quickstart #
+### Quickstart
 
-```python3
+```python
 import pypub
+
 my_first_epub = pypub.Epub('My First Epub')
 my_first_chapter = pypub.create_chapter_from_url('https://en.wikipedia.org/wiki/EPUB')
 my_first_epub.add_chapter(my_first_chapter)
-my_first_epub.create_epub('OUTPUT_DIRECTORY')
+my_first_epub.create('./my-first-epub.epub')
 ```
 
 # Features #
 * Pypub is **easy to install** and has minimal dependencies.
-* Pypub **abstracts the epub specification**. Create epubs without worrying about what an NCX is.
-* Pypub can **create epubs from websites, html files, strings**, or a combination of all three.
-* Pypub can **clean up poorly formatted and complicated html**, so it will show cleanly as a chapter in your book.
-* Pypub **creates epubs specifically so they can be converted into Amazon Kindle mobi or azw3 files**. Don't know which tags Amazon supports? Don't worry about it because pypub does. 
-* Pypub is **customizable**. Don't like the way pypub sanitizes html files for you ebook? Pypub can be configured with your own sanitation function.
+* Pypub **abstracts the epub specification**. 
+  Create epubs without worrying about what an NCX is.
+* Pypub can **create epubs from websites, html files, strings**, 
+  or a combination of all three.
+* Pypub can **clean up poorly formatted and complicated html**, 
+  so it will show cleanly as a chapter in your book.
+* Pypub **creates epubs specifically so they can be converted into 
+  Amazon Kindle mobi or azw3 files**. Don't know which tags Amazon 
+  supports? Don't worry about it because pypub does. 
+* Pypub is **customizable**. Don't like the way pypub sanitizes html 
+  files for you ebook? Pypub can be configured with your own sanitation 
+  function.
 * Pypub is **licensed under the MIT license**. Do what you want with it.
-
-# Documentation #
-
-Documentation is available at [http://pypub3.readthedocs.org/en/latest/developer_interface.html](http://pypub3.readthedocs.org/en/latest/developer_interface.html)
-
-# Copyright and License #
-
-Copyright (c) 2022 Andrew Scott
-
-[**Licensed**](https://github.com/imgurbot12/pypub/blob/master/LICENSE) under the MIT License
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `pypub3-1.0.2/pypub/chapter.py` & `pypub3-2.0.0/pypub/factory.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,176 +1,234 @@
 """
-contains chapter object and chapter generating utilities
+Chapter Rendering Factory Implementation
 """
 import os
-import html
 import uuid
-import imghdr
-import lxml.html
+import urllib.error
 import urllib.parse
 import urllib.request
+from logging import Logger
+from abc import abstractmethod
+from dataclasses import dataclass, field
+from typing import Protocol
+
+import imghdr
+import pyxml.html
+from pyxml.html import HtmlElement
 from jinja2 import Template
-from typing import Optional
 
-from .const import log, validate, xmlprettify, SUPPORTED_TAGS
+from .chapter import Chapter, urlrequest, htmltostring
 
 #** Variables **#
 __all__ = [
-    'Chapter',
+    'SUPPORTED_TAGS',
 
-    'create_chapter_from_url',
-    'create_chapter_from_file',
-    'create_chapter_from_string',
+    'urlrequest',
+    'render_images',
+    'xmlprettify',
+
+    'RenderCtx', 
+    'ChapterFactory', 
+    'SimpleChapterFactory'
 ]
 
-# install believable browser user-agent for default urllib.request.open
-ua     = 'Mozilla/5.0 (X11; Ubuntu; Linux x86_64; rv:77.0) Gecko/20100101 Firefox/77.0'
-opener = urllib.request.build_opener()
-opener.addheaders = [('User-agent', ua)]
-urllib.request.install_opener(opener)
+#: unicode characters to replace if found in content
+REPLACE = dict([(ord(x), ord(y)) for x,y in zip(u"‘’´“”–-", u"'''\"\"--")])
 
-#** Functions **#
+#: supported tags and attributes allowed in an epub
+SUPPORTED_TAGS = {
+    'a':          ('href', 'id'),
+    'b':          ('id', ),
+    'big':        (),
+    'blockquote': ('id', ),
+    'body':       (),
+    'br':         ('id', ),
+    'center':     (),
+    'cite':       (),
+    'dd':         ('id', 'title'),
+    'del':        (),
+    'dfn':        (),
+    'div':        ('align', 'id', 'bgcolor'),
+    'em':         ('id', 'title'),
+    'font':       ('color', 'face', 'id', 'size'),
+    'head':       (),
+    'h1':         (),
+    'h2':         (),
+    'h3':         (),
+    'h4':         (),
+    'h5':         (),
+    'h6':         (),
+    'html':       (),
+    'i':          ('class', 'id'),
+    'img':        ('align', 'border', 'height', 'id', 'src', 'width'),
+    'li':         ('class', 'id', 'title'),
+    'ol':         ('id', ),
+    'p':          ('align', 'id', 'title'),
+    's':          ('id', 'style', 'title'),
+    'small':      ('id', ),
+    'span':       ('bgcolor', 'title'),
+    'strike':     ('class', 'id'),
+    'strong':     ('class', 'id'),
+    'sub':        ('id', ),
+    'sup':        ('class', 'id'),
+    'u':          ('id', ),
+    'ul':         ('class', 'id'),
+    'var':        (),
+}
 
-def create_chapter_from_string(
-    html:          str,
-    title:         Optional[str] = None,
-    url:           Optional[str] = None,
-    title_xpath:   Optional[str] = None,
-    content_xpath: Optional[str] = None,
-    factory:       Optional['Chapter'] = None,
-) -> 'Chapter':
-    """
-    generate a chapter object from the given html string
+#** Functions **#
 
-    :param html:          html string making up chapter content
-    :param title:         title used for the given chpater
-    :param url:           url assigned to this particular chapter
-    :param title_xpath:   xpath used to find title in html
-    :param content_xpath: xpath used to find content in html
-    :param factory:       chapter factory override (for customization)
+def render_images(ctx: 'RenderCtx', chunk_size: int = 8192):
     """
-    html  = '<div>%s</div>' % html
-    etree = None
-    # attempt to parse title if not given
-    if not title:
-        etree  = etree if etree is not None else lxml.html.fromstring(html)
-        xpath  = (title_xpath or './/title').rsplit('text()', 1)[0] + '/text()'
-        elem   = etree.xpath(xpath)
-        # raise error if title-xpath failed
-        if not elem and title_xpath:
-            raise ValueError('no such title xpath: %r' % title_xpath)
-        # assign title to new collection
-        title  = elem[0] if elem else 'Epub Chapter'
-    # attempt to parse content if given xml-path
-    if content_xpath:
-        etree = etree if etree is not None else lxml.html.fromstring(html)
-        elem  = etree.xpath(content_xpath)
-        # if no elements are found, raise error
-        if len(elem) == 0:
-            raise ValueError('no content w/ xpath: %s' % content_xpath)
-        # if one element is found, set as root
-        if len(elem) == 1:
-            html = lxml.html.tostring(elem[0]).decode()
-        # if multiple elements were found, append all to new root
-        else:
-            etree = lxml.html.fromstring('<div></div>')
-            for child in elem:
-                etree.append(child)
-            html = lxml.html.tostring(etree).decode()
-    # generate chapter object
-    factory = factory or Chapter
-    return factory(title=title, content=html, url=url)
-
-def create_chapter_from_file(
-    fpath:         str,
-    title:         Optional[str] = None,
-    url:           Optional[str] = None,
-    title_xpath:   Optional[str] = None,
-    content_xpath: Optional[str] = None,
-    factory:       Optional['Chapter'] = None,
-) -> 'Chapter':
+    replace global image references w/ local downloaded ones
     """
-    generate a chapter object from the given file
+    downloads = {}
+    for image in ctx.etree.xpath('.//img[@src]'):
+        # cleanup link and resolve relative paths
+        url = image.attrib['src'].rsplit('?', 1)[0]
+        fmt = (ctx.chapter.title, url)
+        if '://' not in url:
+            if not ctx.chapter.url:
+                ctx.logger.warning(
+                    'chapter[%s] cannot render image %r w/o chapter-url' % fmt)
+                continue
+            url = urllib.parse.urljoin(ctx.chapter.url, url)
+            fmt = (ctx.chapter.title, url)
+        # skip if url has already been downloaded
+        if url in downloads:
+            image.attrib['src'] = downloads[url]
+            continue
+        # download url into local image folder for epub
+        ctx.logger.debug(f'chapter[%s] downloading image: %r' % fmt)
+        try:
+            res = urlrequest(url, timeout=ctx.timeout)
+            # ensure status of response is valid
+            if res.status and res.status != 200:
+                raise urllib.error.URLError(f'status: {res.status}')
+            # read first chunk to determine content-type
+            chunk = res.read(chunk_size)
+            mime  = imghdr.what(None, h=chunk)
+            if not mime:
+                ctx.logger.warning('chapter[%s] cannot identify %r mime' % fmt)
+                continue
+            fname = f'{uuid.uuid4()}.{mime}'
+            fpath = os.path.join(ctx.imagedir, fname)
+            # read rest of the content into associated file
+            with open(fpath, 'wb') as f:
+                while chunk:
+                    f.write(chunk)
+                    chunk = res.read(chunk_size)
+            # save epub-path in downloads cache and update image attribs
+            epub_path = os.path.join('images/', fname)
+            downloads[url] = epub_path
+            image.attrib['src'] = epub_path
+        except urllib.error.URLError:
+            ctx.logger.error('chapter[%s] failed to download %r' % fmt)
 
-    :param fpath:         html file location making up chapter content
-    :param title:         title used for the given chpater
-    :param url:           url assigned to this particular chapter
-    :param title_xpath:   xpath used to find title in html
-    :param content_xpath: xpath used to find content in html
-    :param factory:       chapter factory override (for customization)
+def xmlprettify(elem: HtmlElement, chars: str='  ', level: int=1):
     """
-    with open(fpath, 'r') as f:
-        url = url or f'file://{os.path.abspath(fpath)}'
-        return create_chapter_from_string(f.read(),
-            title, url, title_xpath, content_xpath, factory)
-
-def create_chapter_from_url(
-    url:           str,
-    title:         Optional[str] = None,
-    title_xpath:   Optional[str] = None,
-    content_xpath: Optional[str] = None,
-    factory:       Optional['Chapter'] = None,
-) -> 'Chapter':
+    prettify the given element-tree w/ new indentations
+    
+    :param elem:  element being prettified
+    :param chars: characters used for single indent
+    :param level: internal variable used to track indent level
     """
-    generate a chapter object from the given file
-
-    :param url:           url being downloaded for html content
-    :param title:         title used for the given chpater
-    :param title_xpath:   xpath used to find title in html
-    :param content_xpath: xpath used to find content in html
-    :param factory:       chapter factory override (for customization)
-    """
-    r = urllib.request.urlopen(url, timeout=10)
-    return create_chapter_from_string(r.read().decode(),
-        title, url, title_xpath, content_xpath, factory)
+    start    = '\n' + level * chars
+    end      = '\n' + (level - 1) * chars
+    children = elem.getchildren()
+    if children:
+        # make modifications
+        if elem.text:
+            elem.text = elem.text.rstrip() + start
+        if elem.tail:
+            elem.tail = elem.tail.rstrip() + end
+        # iterate children
+        for child in children:
+            xmlprettify(child, chars, level + 1)
+        # ensure last child has tail indentation of parent
+        if children:
+            child = children[-1]
+            child.tail = (child.tail or '').rstrip() + end
+    else:
+        elem.text = '' if not elem.text else elem.text
+        if elem.tail:
+            elem.tail = (elem.tail or '').rstrip() + end
 
 #** Classes **#
 
-class Chapter:
-    """chapter object to be attached to epub"""
+@dataclass
+class RenderCtx:
+    """variables and data associated w/ rendering a chapter"""
+    logger:        Logger
+    chapter:       Chapter
+    etree:         HtmlElement
+    imagedir:      str
+    template:      Template
+    render_kwargs: dict = field(default_factory=dict)
+    timeout:       int  = 10
+
+class ChapterFactory(Protocol):
+    
+    @abstractmethod
+    def cleanup_html(self, content: bytes) -> HtmlElement:
+        """
+        cleanup raw html content and render as an lxml element tree
+        """
+        raise NotImplementedError
+
+    @abstractmethod
+    def hydrate(self, ctx: RenderCtx):
+        """
+        modify contents of chapter and etree before final rendering
+        """
+        raise NotImplementedError
+
+    @abstractmethod
+    def finalize(self, ctx: RenderCtx) -> bytes:
+        """
+        complete final rendering of chapter object and render as html bytes
+        """
+        raise NotImplementedError
+   
+    @abstractmethod
+    def prettify(self, root: HtmlElement):
+        """
+        factory implementation to prettify etree at the end of finalization
+        """
+        raise NotImplementedError
+
+    def render(self, log: Logger, chapter: Chapter, *args, **kwargs) -> bytes:
+        """
+        render chapter to bytes w/ the given settings
+        """
+        etree = self.cleanup_html(chapter.content)
+        ctx   = RenderCtx(log, chapter, etree, *args, **kwargs)
+        self.hydrate(ctx)
+        return self.finalize(ctx)
 
-    def __init__(self, title: str, content: str, url: Optional[str] = None):
+class SimpleChapterFactory(ChapterFactory):
+    """Simple Chapter Factory Implementation"""
+
+    def cleanup_html(self, content: bytes) -> HtmlElement:
+        """
+        cleanup html content to only include supported tags
         """
-        :param title:   title of the chapter
-        :param content: content contained within the chapter
-        :param url:     url from where the chapter content came from
-        """
-        validate('title', title, str)
-        validate('content', content, str)
-        self.title      = title
-        self.content    = content
-        self.url        = url
-        self.html_title = html.escape(title)
-        # additional attributes filled out by epub
-        self.id         = None
-        self.link       = None
-        self.play_order = None
-        self.etree      = None
-
-    def _assign(self, id: int, link: str):
-        """assign addtional epub specific attributes"""
-        self.id         = 'page_%d' % id
-        self.link       = link
-        self.play_order = id
-        self.etree      = self.parse_etree()
-
-    def parse_etree(self) -> Optional[lxml.html.HtmlElement]:
-        """generate new filtered element-tree"""
-        etree = lxml.html.fromstring(self.content)
+        content = content.decode('utf-8', 'replace').translate(REPLACE).encode()
         # check if we can minimalize the scope
+        etree   = pyxml.html.fromstring(content)
         body    = etree.xpath('.//body')
         etree   = body[0] if body else etree
         article = etree.xpath('.//article')
         etree   = article[0] if article else etree
         # iterate elements in tree and delete/modify them
         for elem in [elem for elem in etree.iter()][1:]:
             # if element tag is supported
             if elem.tag in SUPPORTED_TAGS:
                 # remove attributes not approved for specific tag
-                for attr in elem.attrib:
+                for attr in list(elem.attrib.keys()):
                     if attr not in SUPPORTED_TAGS[elem.tag]:
                         elem.attrib.pop(attr)
             # if element is not supported, append children to parent
             else:
                 parent = elem.getparent()
                 for child in elem.getchildren():
                     parent.append(child)
@@ -183,80 +241,32 @@
         # ensure all images with no src are removed
         for img in etree.xpath('.//img'):
             if 'src' not in img.attrib:
                 img.getparent().remove(img)
         # return new element-tree
         return etree
 
-    def replace_images(self, image_dir: str, timeout: int = 10):
-        """replace image references w/ local downloaded ones"""
-        _downloads = set()
-        for img in self.etree.xpath('.//img[@src]'):
-            # get full link for relative paths
-            link = img.attrib['src'].rsplit('?', 1)[0]
-            url  = urllib.parse.urljoin(self.url, link)
-            # skip already completed downloads
-            if url in _downloads:
-                continue
-            # attempt to download from url
-            (head, fname, file) = (True, None, None)
-            try:
-                log.debug('chapter[%s] download img: %s' % (self.title, url))
-                with urllib.request.urlopen(url, timeout=timeout) as r:
-                    # check status of response
-                    if r.status is not None and r.status != 200:
-                        raise RuntimeError(
-                            f'Url: {url!r}, Invalid Status: {r.status!r}')
-                    # read content in chunks
-                    while True:
-                        # read next chunk from request
-                        chunk = r.read(8192)
-                        if not chunk:
-                            break
-                        # check image-type on first chunk
-                        if head:
-                            head = False
-                            mime = imghdr.what(None, h=chunk)
-                            if not mime:
-                                break
-                            fname = '%s.%s' % (uuid.uuid4(), mime)
-                            fpath = os.path.join(image_dir, fname)
-                            file  = open(fpath, 'wb')
-                        # write chunks to file if head was accepted
-                        file.write(chunk)
-            finally:
-                if fname:
-                    _downloads.add(url)
-                    img.attrib['src'] = os.path.join('images/', fname)
-                if file:
-                    file.close()
-   
-    @staticmethod
-    def prettify(elem: lxml.html.HtmlElement):
+    def hydrate(self, ctx: RenderCtx):
         """
-        chapter xml prettify function (available as method to allow override)
-
-        :param elem: html-element to be prettified
+        modify chapter element-tree to render images
         """
-        xmlprettify(elem)
-
-    def render(self, template: Template, image_dir: str, **kw: str) -> bytes:
+        render_images(ctx)
+    
+    def prettify(self, root: HtmlElement):
         """
-        render chapter content and attach it to the template
+        simple xml prettify function
+        """
+        xmlprettify(root)
 
-        :param template:  jinja2 template used to render chapter content
-        :param image_dir: chapter directory to assign images to
-        :param kw:        additional arguments to pass to jinaj2 renderer
-        :return:          rendered chapter as bytestring
+    def finalize(self, ctx: RenderCtx) -> bytes:
+        """
+        render chapter content w/ specified template
         """
-        # replace images in etree
-        self.replace_images(image_dir)
-        # render template and xml tree to attach elements to
-        content = template.render(**kw, chapter=vars(self))
-        etree   = lxml.html.fromstring(content.encode())
-        # attach elements from chapter tree to complete template
-        body = etree.xpath('.//body')[0]
-        for elem in self.etree.getchildren():
+        content = ctx.template.render(**ctx.render_kwargs)
+        # attach elements from chapter etree to content etree
+        etree = pyxml.html.fromstring(content.encode())
+        body  = etree.xpath('.//body')[0]
+        for elem in ctx.etree.getchildren():
             body.append(elem)
         # return html as string to be written
-        self.prettify(elem)
-        return lxml.html.tostring(etree, method='xml')
+        self.prettify(etree)
+        return htmltostring(etree)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pypub3-1.0.2/pypub/static/coverpage.xhtml` & `pypub3-2.0.0/pypub/static/coverpage.xhtml`

 * *Files identical despite different names*

### Comparing `pypub3-1.0.2/pypub/static/fonts/free_mono.ttf` & `pypub3-2.0.0/pypub/static/fonts/free_mono.ttf`

 * *Files identical despite different names*

### Comparing `pypub3-1.0.2/pypub/static/img/cover.png` & `pypub3-2.0.0/pypub/static/img/cover.png`

 * *Files identical despite different names*

### Comparing `pypub3-1.0.2/pypub/templates/book.ncx.xml.j2` & `pypub3-2.0.0/pypub/templates/book.ncx.j2`

 * *Files 23% similar despite different names*

#### Comparing `pypub3-1.0.2/pypub/templates/book.ncx.xml.j2` & `pypub3-2.0.0/pypub/templates/book.ncx.j2`

```diff
@@ -3,23 +3,23 @@
   <head>
     <meta name="dtb:uid" content="{{ uid }}"/>
     <meta name="dtb:depth" content="1"/>
     <meta name="dtb:totalPageCount" content="0"/>
     <meta name="dtb:maxPageNumber" content="0"/>
   </head>
   <docTitle>
-    <text>{{ title }}</text>
+    <text>{{ epub.title }}</text>
   </docTitle>
   <docAuthor>
-    <text>{{ creator }}</text>
+    <text>{{ epub.creator }}</text>
   </docAuthor>
   <navMap>
-    {%- for chapter in chapters %}
-    <navPoint id="{{ chapter.id }}" playOrder="{{ chapter.play_order }}">
+    {%- for (assign, chapter) in chapters %}
+    <navPoint id="{{ assign.id }}" playOrder="{{ assign.play_order }}">
       <navLabel>
         <text>{{ chapter.title }}</text>
       </navLabel>
-      <content src="{{ chapter.link }}"/>
+      <content src="{{ assign.link }}"/>
     </navPoint>
     {%- endfor %}
   </navMap>
 </ncx>
```

### Comparing `pypub3-1.0.2/pypub/templates/book.opf.xml.j2` & `pypub3-2.0.0/pypub/templates/book.opf.j2`

 * *Files 9% similar despite different names*

#### Comparing `pypub3-1.0.2/pypub/templates/book.opf.xml.j2` & `pypub3-2.0.0/pypub/templates/book.opf.j2`

```diff
@@ -1,43 +1,43 @@
 <?xml version="1.0" encoding="utf-8"?>
 <package xmlns="http://www.idpf.org/2007/opf" version="2.0" unique-identifier="BookId">
   <metadata xmlns:dc="http://purl.org/dc/elements/1.1/" xmlns:opf="http://www.idpf.org/2007/opf">
-    <dc:title>{{ title }}</dc:title>
-    <dc:creator opf:role="aut">{{ creator }}</dc:creator>
-    <dc:language>{{ language }}</dc:language>
-    <dc:rights>{{ rights }}</dc:rights>
-    <dc:publisher>{{ publisher }}</dc:publisher>
-    <dc:identifier id="BookId" opf:scheme="UUID">{{ uid }}</dc:identifier>
-    <dc:date opf:event="publication">{{ date }}</dc:date>
+    <dc:title>{{ epub.title }}</dc:title>
+    <dc:creator opf:role="aut">{{ epub.creator }}</dc:creator>
+    <dc:language>{{ epub.language }}</dc:language>
+    <dc:rights>{{ epub.rights }}</dc:rights>
+    <dc:publisher>{{ epub.publisher }}</dc:publisher>
+    <dc:identifier id="BookId" opf:scheme="UUID">{{ epub.uid }}</dc:identifier>
+    <dc:date opf:event="publication">{{ epub.date.isoformat() }}</dc:date>
     <meta name="cover" content="cover_img"/>
     <meta name="generator" content="PYPUB ePub Generator {{ version }}"/>
   </metadata>
   <manifest>
     <!-- static references -->
     <item href="book.ncx" id="ncx" media-type="application/x-dtbncx+xml"/>
     <item href="toc.xhtml" id="toc" media-type="application/xhtml+xml"/>
     <item href="coverpage.xhtml" id="cover_page" media-type="application/xhtml+xml"/>
     <!-- styles references -->
-    {%- for id, css in styles %}
-    <item id="css_{{ id }}" href="styles/{{ css }}" media-type="text/css"/>
+    {%- for css in styles %}
+    <item id="css_{{ loop.index }}" href="styles/{{ css }}" media-type="text/css"/>
     {%- endfor %}
     <!-- images references -->
-    <item id="cover_img" href="images/{{ cover_img }}" media-type="image/{{ cover_ext }}"/>
-    {%- for ext, image in images %}
-    <item id="{{ image }}" href="images/{{ image }}" media-type="image/{{ ext }}"/>
+    <item id="cover_img" href="images/{{ cover.name }}" media-type="image/{{ cover.mime }}"/>
+    {%- for image in images %}
+    <item id="{{ image.name }}" href="images/{{ image.name }}" media-type="image/{{ image.mime }}"/>
     {%- endfor %}
     <!-- chapter inclusions -->
-    {%- for chapter in chapters %}
-    <item href="{{ chapter.link }}" id="{{ chapter.id }}" media-type="application/xhtml+xml"/>
+    {%- for (assign, _) in chapters %}
+    <item href="{{ assign.link }}" id="{{ assign.id }}" media-type="application/xhtml+xml"/>
     {%- endfor %}
   </manifest>
   <spine toc="ncx">
     <itemref idref="cover_page"/>
     <itemref idref="toc"/>
-    {%- for chapter in chapters %}
-    <itemref idref="{{ chapter.id }}"/>
+    {%- for (assign, _) in chapters %}
+    <itemref idref="{{ assign.id }}"/>
     {%- endfor %}
   </spine>
   <guide>
     <reference type="toc" title="Table of Contents" href="toc.xhtml"/>
   </guide>
 </package>
```

### Comparing `pypub3-1.0.2/pypub/templates/toc.xhtml.xml.j2` & `pypub3-2.0.0/pypub/templates/toc.xhtml.j2`

 * *Files 20% similar despite different names*

#### Comparing `pypub3-1.0.2/pypub/templates/toc.xhtml.xml.j2` & `pypub3-2.0.0/pypub/templates/toc.xhtml.j2`

```diff
@@ -7,15 +7,15 @@
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8"/>
     <title>Table of Contents</title>
   </head>
   <body>
     <h2>Table of Contents</h2>
     <hr/>
     <div id="chapters">
-      {%- for chapter in chapters %}
+      {%- for (assign, chapter) in chapters %}
       <p>
-        <a href="{{ chapter.link }}">{{ chapter.html_title }}</a>
+        <a href="{{ assign.link }}">{{ chapter.title | e }}</a>
       </p>
       {%- endfor %}
     </div>
   </body>
 </html>
```

### Comparing `pypub3-1.0.2/pypub/tests/profile_test.py` & `pypub3-2.0.0/pypub/tests/profile.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 #** Functions **#
 
 def _create_epub():
     try:
         epub    = Epub('My First Epub')
         chapter = create_chapter_from_url('https://en.wikipedia.org/wiki/Grand_Teton_National_Park')
         epub.add_chapter(chapter)
-        epub.create_epub('.', 'profile-test.epub')
+        epub.create('./profile-test.epub')
     finally:
         try:
             os.remove('./profile-test.epub')
         except Exception:
             pass
 
 #** Tests **#
```

### Comparing `pypub3-1.0.2/setup.py` & `pypub3-2.0.0/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     readme = f.read()
 
 setup(
     name='pypub3',
-    version='1.0.2',
+    version='2.0.0',
     license='MIT',
     author='Andrew Scott',
     author_email='imgurbot12@gmail.com',
     url='https://github.com/imgurbot12/pypub',
     description="A python3 library to generate custom epub books.",
     long_description=readme,
     long_description_content_type="text/markdown",
     python_requires='>=3.6',
     packages=find_packages(),
     install_requires=[
         'jinja2',
-        'lxml',
-        'pillow'
+        'pyxml3',
+        'pillow',
+        'dataclasses',
     ],
     package_data={
         'pypub': [
             'templates/*', 
             'static/*', 
             'static/css/*', 
             'static/img/*',
```

