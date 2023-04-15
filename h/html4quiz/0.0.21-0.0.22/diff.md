# Comparing `tmp/html4quiz-0.0.21.tar.gz` & `tmp/html4quiz-0.0.22.tar.gz`

## Comparing `html4quiz-0.0.21.tar` & `html4quiz-0.0.22.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 html4quiz-0.0.21/Embedding Images in HTMLs.url
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 html4quiz-0.0.21/Packaging.url
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 html4quiz-0.0.21/certutil -encode mypicture.png mypicture.txt.txt
--rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 html4quiz-0.0.21/up8c18p01.png
--rw-r--r--   0        0        0     2850 2020-02-02 00:00:00.000000 html4quiz-0.0.21/up8c18p01.txt
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 html4quiz-0.0.21/updatePackage.txt
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 html4quiz-0.0.21/src/html4quiz/__init__.py
--rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 html4quiz-0.0.21/src/html4quiz/_common.py
--rw-r--r--   0        0        0    11158 2020-02-02 00:00:00.000000 html4quiz-0.0.21/src/html4quiz/_generateEm.py
--rw-r--r--   0        0        0    17875 2020-02-02 00:00:00.000000 html4quiz-0.0.21/src/html4quiz/_generateMakeHTMLs.py
--rw-r--r--   0        0        0     9951 2020-02-02 00:00:00.000000 html4quiz-0.0.21/src/html4quiz/_scoreEm.py
--rw-r--r--   0        0        0    14972 2020-02-02 00:00:00.000000 html4quiz-0.0.21/src/html4quiz/makeChoices.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 html4quiz-0.0.21/LICENSE.txt
--rw-r--r--   0        0        0     3647 2020-02-02 00:00:00.000000 html4quiz-0.0.21/README.md
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 html4quiz-0.0.21/pyproject.toml
--rw-r--r--   0        0        0     4372 2020-02-02 00:00:00.000000 html4quiz-0.0.21/PKG-INFO
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 html4quiz-0.0.22/updatePackage.txt
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 html4quiz-0.0.22/src/html4quiz/__init__.py
+-rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 html4quiz-0.0.22/src/html4quiz/_common.py
+-rw-r--r--   0        0        0    26651 2020-02-02 00:00:00.000000 html4quiz-0.0.22/src/html4quiz/_generateEm.py
+-rw-r--r--   0        0        0    11135 2020-02-02 00:00:00.000000 html4quiz-0.0.22/src/html4quiz/_scoreEm.py
+-rw-r--r--   0        0        0    14972 2020-02-02 00:00:00.000000 html4quiz-0.0.22/src/html4quiz/makeChoices.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 html4quiz-0.0.22/src - 0.0.21/html4quiz/__init__.py
+-rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 html4quiz-0.0.22/src - 0.0.21/html4quiz/_common.py
+-rw-r--r--   0        0        0    11158 2020-02-02 00:00:00.000000 html4quiz-0.0.22/src - 0.0.21/html4quiz/_generateEm.py
+-rw-r--r--   0        0        0    17875 2020-02-02 00:00:00.000000 html4quiz-0.0.22/src - 0.0.21/html4quiz/_generateMakeHTMLs.py
+-rw-r--r--   0        0        0    10486 2020-02-02 00:00:00.000000 html4quiz-0.0.22/src - 0.0.21/html4quiz/_scoreEm.py
+-rw-r--r--   0        0        0    14972 2020-02-02 00:00:00.000000 html4quiz-0.0.22/src - 0.0.21/html4quiz/makeChoices.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 html4quiz-0.0.22/LICENSE.txt
+-rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 html4quiz-0.0.22/README.md
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 html4quiz-0.0.22/pyproject.toml
+-rw-r--r--   0        0        0     4703 2020-02-02 00:00:00.000000 html4quiz-0.0.22/PKG-INFO
```

### Comparing `html4quiz-0.0.21/src/html4quiz/_common.py` & `html4quiz-0.0.22/src - 0.0.21/html4quiz/_common.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,24 @@
 import math, random, re, json
 from urllib.request import urlopen
+import urllib
 
 def getFigure(file: str):
-    return json.loads(urlopen(f'https://generateNscore.github.io/html4quiz/JS/{file}.json').read())
+    try:
+        return json.loads(urlopen(f'https://generateNscore.github.io/html4quiz/JS/{file}.json').read())
+    except urllib.error.HTTPError:
+        return 'HTTP Error 404: Not Found'
+
+
+def getEtc(file: str):
+    try:
+        return json.loads(urlopen(f'https://generateNscore.github.io/html4quiz/Etc/{file}.json').read())
+    except urllib.error.HTTPError:
+        return 'HTTP Error 404: Not Found'
+
 
 def round2MSF(a):
     if not a or (isinstance(a, int) and abs(a)<1000) : return a
 
     sfN=3
     signFlag=False
     if a<0: a=-a; signFlag=True
```

### Comparing `html4quiz-0.0.21/src/html4quiz/_generateEm.py` & `html4quiz-0.0.22/src - 0.0.21/html4quiz/_generateEm.py`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.21/src/html4quiz/_generateMakeHTMLs.py` & `html4quiz-0.0.22/src - 0.0.21/html4quiz/_generateMakeHTMLs.py`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.21/src/html4quiz/_scoreEm.py` & `html4quiz-0.0.22/src - 0.0.21/html4quiz/_scoreEm.py`

 * *Files 6% similar despite different names*

```diff
@@ -82,16 +82,18 @@
             if ':' not in line: continue
             hdr, *hdrValue=line.strip().split(':')
             hdr=hdr.strip()
             hdrValue=':'.join(hdrValue)
             if hdr.isnumeric() and int(hdr)<=self.nProblems and hdrValue:
                 try:
                     answersFromTxt[int(hdr)-1]=eval(hdrValue)
+                except SyntaxError: # 2023-04-14 added
+                    answersFromTxt[int(hdr)-1]=hdrValue.strip() # 2023-04-14 added
                 except Exception as err:
-                    answersFromTxt[int(hdr)-1]=f'Error({err}) in ({hdrValue})'
+                    answersFromTxt[int(hdr)-1]=f'Error({err}) in ({hdrValue}) @ Ln90'
 
         return answersFromTxt
 
 
     def getFiles(self):
         fileList=[f for f in os.listdir(self.path4files) if 'Scores' not in f and f.endswith(self.ext)]
         mtime=[str(datetime.datetime.fromtimestamp(os.stat(self.path4files+f'/{f}').st_mtime))[5:] for f in fileList]
@@ -131,15 +133,15 @@
                             wv=evalPyCode(ans2match, v['py'][nChecked][2])
                         except Exception as err:
                             v['ox'][nChecked]='X'+f'Error({err})'
                             continue
                         v['ox'][nChecked] = self.compare(wv, ans2match['ret'])
 
                 elif isinstance(ans2match, str) and ans2match.startswith('code:'):
-                    if checkAnswerCode(wv, ans2match.split('code:')[-1]): # 반환값: T/F
+                    if self.checkAnswerCode(wv, ans2match.split('code:')[-1]): # 반환값: T/F 2023-04-15 self.추
                         v['ox'][nChecked] = 'O'
                     else:
                         v['ox'][nChecked] = 'Xincorrect arb. value'
 
                 else:
                     v['ox'][nChecked] = self.compare(wv, ans2match)
 
@@ -236,12 +238,22 @@
             elif isinstance(B, float):
                 if round2MSF(A) == round2MSF(B):
                     return 'O'
                 else:
                     #print(round2MSF(A), round2MSF(B))
                     return 'Xrounding error'
             else:
+                #print(f'학생답: ++{A}++', type(A)) # 2023-04-14 added
+                #print(f'정답: ++{B}++', type(B)) # 2023-04-14 added
                 return 'Xwrong Answer'
         else:
             return 'Xwrong type'
 
 
+    @staticmethod
+    def checkAnswerCode(StudentValue, ansCode):  # 2023-04-14 added incomplete
+        try:
+            tmp=eval(ansCode)
+        except Exception:
+            tmp=False
+        return tmp
+
```

### Comparing `html4quiz-0.0.21/src/html4quiz/makeChoices.py` & `html4quiz-0.0.22/src/html4quiz/makeChoices.py`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.21/LICENSE.txt` & `html4quiz-0.0.22/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.21/README.md` & `html4quiz-0.0.22/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -8,20 +8,20 @@
 <ul>
 <li><a href="https://github.com/generateNscore/html4quiz/wiki">Documentation</a></li>
 </ul>
 
 ## Features
 <ul>
 <li>Generates as many personalized question sheets in HTML files as one wants with a few strings of text.</li>
-<li>The amount of random personalization is under total control of users.</li>
+<li>The amount of random personalization is under full control of users.</li>
 <li>Each HTML file with a name corresponding to the identification number.</li>
 <li>Multi-choice as well as short, default, questions can be made.</li>
 <li>A figure, although a pre-made image can be used, can be varied as well as questions.</li>
 <li>Mathematical equations can be included in questions with Latex.</li>
-<li>User defined functions can be used.</li>
+<li>User defined functions can be easily added.</li>
 <li>With the question sheets in HTML files, students require only a web browser to answer and send text files including the answers over the network.</li>
 <li>Scoring all different answers in text files submitted can be done in a second.</li>
 </ul>
 
 ## Where to get it
 <ul>
 <li>The source code is currently hosted on GitHub at: <a href="https://github.com/generateNscore/html4quiz">https://github.com/generateNscore/html4quiz</a></li>
@@ -34,14 +34,20 @@
 
 ## Dependencies
 <ul><li>None</li></ul>
 
 
 ## Changes
 
+<li>Version 0.0.22</li>
+<ul><li>Added "res" folder to GitHub for the Javascript scripts of figures and additional data saved in JSON format.</li>
+<li>Added a "getResource()" function to the package to access the data.</li>
+<li>Some procedures of calling functions were removed to simplify the usages of package.</li>
+</ul>
+
 <li>Version 0.0.21</li>
 <ul><li>Package name has been changed from htmlfilesforquiz to html4quiz</li>
 <li>So is the name of repository in GitHub.</li></ul>
 
 <li>Version 0.0.20</li>
 
 <ul><li>Finallized a way to upload/download Javascript scripts saved in JSON files for figures.<a href="https://github.com/generateNscore/html4quiz/wiki#h-download-json-file-of-javascript-code-for-figure-contents">H. Download Json file of Javascript code for figure contents</a></li></ul>
```

#### html2text {}

```diff
@@ -1,34 +1,40 @@
 # html4quiz ## What is it? html4quiz is a package that generates question
 papers as HTML files to be distributed over the network and grades the answers
 in text files submitted by students. ## Help
     * Documentation
 ## Features
     * Generates as many personalized question sheets in HTML files as one wants
       with a few strings of text.
-    * The amount of random personalization is under total control of users.
+    * The amount of random personalization is under full control of users.
     * Each HTML file with a name corresponding to the identification number.
     * Multi-choice as well as short, default, questions can be made.
     * A figure, although a pre-made image can be used, can be varied as well as
       questions.
     * Mathematical equations can be included in questions with Latex.
-    * User defined functions can be used.
+    * User defined functions can be easily added.
     * With the question sheets in HTML files, students require only a web
       browser to answer and send text files including the answers over the
       network.
     * Scoring all different answers in text files submitted can be done in a
       second.
 ## Where to get it
     * The source code is currently hosted on GitHub at: https://github.com/
       generateNscore/html4quiz
     *
       pip install html4quiz
 ## Dependencies
     * None
 ## Changes
+Version 0.0.22
+    * Added "res" folder to GitHub for the Javascript scripts of figures and
+      additional data saved in JSON format.
+    * Added a "getResource()" function to the package to access the data.
+    * Some procedures of calling functions were removed to simplify the usages
+      of package.
 Version 0.0.21
     * Package name has been changed from htmlfilesforquiz to html4quiz
     * So is the name of repository in GitHub.
 Version 0.0.20
     * Finallized a way to upload/download Javascript scripts saved in JSON
       files for figures.H._Download_Json_file_of_Javascript_code_for_figure
       contents
```

### Comparing `html4quiz-0.0.21/pyproject.toml` & `html4quiz-0.0.22/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "html4quiz"
-version = "0.0.21"
+version = "0.0.22"
 authors = [
   { name="Sukmock Lee", email="smlee@inha.ac.kr" },
 ]
 description = "A package that generates question papers as HTML files to be distributed over the network and grades the answers in text files submitted by students."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `html4quiz-0.0.21/PKG-INFO` & `html4quiz-0.0.22/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: html4quiz
-Version: 0.0.21
+Version: 0.0.22
 Summary: A package that generates question papers as HTML files to be distributed over the network and grades the answers in text files submitted by students.
 Project-URL: Homepage, https://github.com/generateNscore/html4quiz
 Project-URL: Bug Tracker, https://github.com/generateNscore/html4quiz/issues
 Author-email: Sukmock Lee <smlee@inha.ac.kr>
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
@@ -26,20 +26,20 @@
 <ul>
 <li><a href="https://github.com/generateNscore/html4quiz/wiki">Documentation</a></li>
 </ul>
 
 ## Features
 <ul>
 <li>Generates as many personalized question sheets in HTML files as one wants with a few strings of text.</li>
-<li>The amount of random personalization is under total control of users.</li>
+<li>The amount of random personalization is under full control of users.</li>
 <li>Each HTML file with a name corresponding to the identification number.</li>
 <li>Multi-choice as well as short, default, questions can be made.</li>
 <li>A figure, although a pre-made image can be used, can be varied as well as questions.</li>
 <li>Mathematical equations can be included in questions with Latex.</li>
-<li>User defined functions can be used.</li>
+<li>User defined functions can be easily added.</li>
 <li>With the question sheets in HTML files, students require only a web browser to answer and send text files including the answers over the network.</li>
 <li>Scoring all different answers in text files submitted can be done in a second.</li>
 </ul>
 
 ## Where to get it
 <ul>
 <li>The source code is currently hosted on GitHub at: <a href="https://github.com/generateNscore/html4quiz">https://github.com/generateNscore/html4quiz</a></li>
@@ -52,14 +52,20 @@
 
 ## Dependencies
 <ul><li>None</li></ul>
 
 
 ## Changes
 
+<li>Version 0.0.22</li>
+<ul><li>Added "res" folder to GitHub for the Javascript scripts of figures and additional data saved in JSON format.</li>
+<li>Added a "getResource()" function to the package to access the data.</li>
+<li>Some procedures of calling functions were removed to simplify the usages of package.</li>
+</ul>
+
 <li>Version 0.0.21</li>
 <ul><li>Package name has been changed from htmlfilesforquiz to html4quiz</li>
 <li>So is the name of repository in GitHub.</li></ul>
 
 <li>Version 0.0.20</li>
 
 <ul><li>Finallized a way to upload/download Javascript scripts saved in JSON files for figures.<a href="https://github.com/generateNscore/html4quiz/wiki#h-download-json-file-of-javascript-code-for-figure-contents">H. Download Json file of Javascript code for figure contents</a></li></ul>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: html4quiz Version: 0.0.21 Summary: A package that
+Metadata-Version: 2.1 Name: html4quiz Version: 0.0.22 Summary: A package that
 generates question papers as HTML files to be distributed over the network and
 grades the answers in text files submitted by students. Project-URL: Homepage,
 https://github.com/generateNscore/html4quiz Project-URL: Bug Tracker, https://
 github.com/generateNscore/html4quiz/issues Author-email: Sukmock Lee
 inha.ac.kr> License-File: LICENSE.txt Classifier: Development Status :: 4 -
 Beta Classifier: Intended Audience :: Education Classifier: Intended Audience
 :: End Users/Desktop Classifier: License :: OSI Approved :: MIT License
@@ -11,34 +11,40 @@
 Description-Content-Type: text/markdown # html4quiz ## What is it? html4quiz is
 a package that generates question papers as HTML files to be distributed over
 the network and grades the answers in text files submitted by students. ## Help
     * Documentation
 ## Features
     * Generates as many personalized question sheets in HTML files as one wants
       with a few strings of text.
-    * The amount of random personalization is under total control of users.
+    * The amount of random personalization is under full control of users.
     * Each HTML file with a name corresponding to the identification number.
     * Multi-choice as well as short, default, questions can be made.
     * A figure, although a pre-made image can be used, can be varied as well as
       questions.
     * Mathematical equations can be included in questions with Latex.
-    * User defined functions can be used.
+    * User defined functions can be easily added.
     * With the question sheets in HTML files, students require only a web
       browser to answer and send text files including the answers over the
       network.
     * Scoring all different answers in text files submitted can be done in a
       second.
 ## Where to get it
     * The source code is currently hosted on GitHub at: https://github.com/
       generateNscore/html4quiz
     *
       pip install html4quiz
 ## Dependencies
     * None
 ## Changes
+Version 0.0.22
+    * Added "res" folder to GitHub for the Javascript scripts of figures and
+      additional data saved in JSON format.
+    * Added a "getResource()" function to the package to access the data.
+    * Some procedures of calling functions were removed to simplify the usages
+      of package.
 Version 0.0.21
     * Package name has been changed from htmlfilesforquiz to html4quiz
     * So is the name of repository in GitHub.
 Version 0.0.20
     * Finallized a way to upload/download Javascript scripts saved in JSON
       files for figures.H._Download_Json_file_of_Javascript_code_for_figure
       contents
```

