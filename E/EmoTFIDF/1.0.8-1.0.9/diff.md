# Comparing `tmp/EmoTFIDF-1.0.8.tar.gz` & `tmp/EmoTFIDF-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\EmoTFIDF-1.0.8.tar", last modified: Fri Mar  5 10:15:14 2021, max compression
+gzip compressed data, was "dist\EmoTFIDF-1.0.9.tar", last modified: Fri Mar  5 10:20:46 2021, max compression
```

## Comparing `EmoTFIDF-1.0.8.tar` & `EmoTFIDF-1.0.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2021-03-05 10:15:14.000000 EmoTFIDF-1.0.8/
-drwxrwxrwx   0        0        0        0 2021-03-05 10:15:14.000000 EmoTFIDF-1.0.8/EmoTFIDF.egg-info/
--rw-rw-rw-   0        0        0        1 2021-03-05 10:15:13.000000 EmoTFIDF-1.0.8/EmoTFIDF.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     3258 2021-03-05 10:15:13.000000 EmoTFIDF-1.0.8/EmoTFIDF.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0        5 2021-03-05 10:15:13.000000 EmoTFIDF-1.0.8/EmoTFIDF.egg-info/requires.txt
--rw-rw-rw-   0        0        0      189 2021-03-05 10:15:13.000000 EmoTFIDF-1.0.8/EmoTFIDF.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        9 2021-03-05 10:15:13.000000 EmoTFIDF-1.0.8/EmoTFIDF.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4938 2021-03-05 10:13:22.000000 EmoTFIDF-1.0.8/emotfidf.py
--rw-rw-rw-   0        0        0     3258 2021-03-05 10:15:14.000000 EmoTFIDF-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     1996 2021-03-05 10:15:05.000000 EmoTFIDF-1.0.8/README.md
--rw-rw-rw-   0        0        0       42 2021-03-05 10:15:14.000000 EmoTFIDF-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1363 2021-03-05 10:13:41.000000 EmoTFIDF-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2021-03-05 10:20:46.000000 EmoTFIDF-1.0.9/
+drwxrwxrwx   0        0        0        0 2021-03-05 10:20:46.000000 EmoTFIDF-1.0.9/EmoTFIDF.egg-info/
+-rw-rw-rw-   0        0        0        1 2021-03-05 10:20:46.000000 EmoTFIDF-1.0.9/EmoTFIDF.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     3258 2021-03-05 10:20:46.000000 EmoTFIDF-1.0.9/EmoTFIDF.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0        5 2021-03-05 10:20:46.000000 EmoTFIDF-1.0.9/EmoTFIDF.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      189 2021-03-05 10:20:46.000000 EmoTFIDF-1.0.9/EmoTFIDF.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        9 2021-03-05 10:20:46.000000 EmoTFIDF-1.0.9/EmoTFIDF.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5013 2021-03-05 10:18:45.000000 EmoTFIDF-1.0.9/emotfidf.py
+-rw-rw-rw-   0        0        0     3258 2021-03-05 10:20:46.000000 EmoTFIDF-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1996 2021-03-05 10:15:05.000000 EmoTFIDF-1.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2021-03-05 10:20:46.000000 EmoTFIDF-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1363 2021-03-05 10:20:33.000000 EmoTFIDF-1.0.9/setup.py
```

### Comparing `EmoTFIDF-1.0.8/EmoTFIDF.egg-info/PKG-INFO` & `EmoTFIDF-1.0.9/EmoTFIDF.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EmoTFIDF
-Version: 1.0.8
+Version: 1.0.9
 Summary: A library to extract emotions using two methods, 1- Using lexicon based, counting frequency of emotion2- Integrating TFIDF to add a contextNote that lexicon license is for research purposes only.
 Home-page: https://github.com/mmsa/emotfidf
 Author: mmsa12
 Author-email: mmsa12@gmail.com
 License: UNKNOWN
 Description: EmoTFIDF is an emotion detection library (Lexicon approach) based in the National Research Council Canada (NRC) and this package is for research purposes only. Source: [lexicons for research] (http://sentiment.nrc.ca/lexicons-for-research/)
```

### Comparing `EmoTFIDF-1.0.8/emotfidf.py` & `EmoTFIDF-1.0.9/emotfidf.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,16 @@
             em_dict.update({word: self.lexicon[word]})
     for word in em_list:
         em_frequencies[word] += 1
     sum_values = sum(em_frequencies.values())
     em_percent = {'fear': 0.0, 'anger': 0.0, 'anticipation': 0.0, 'trust': 0.0, 'surprise': 0.0, 'positive': 0.0,
                   'negative': 0.0, 'sadness': 0.0, 'disgust': 0.0, 'joy': 0.0}
     if self.sent_flag == 1:
-        em_percent = {'fear': 0.0, 'anger': 0.0, 'anticipation': 0.0, 'trust': 0.0, 'surprise': 0.0, 'sadness': 0.0, 'disgust': 0.0, 'joy': 0.0}
+        em_percent = {'fear': 0.0, 'anger': 0.0, 'anticipation': 0.0, 'trust': 0.0, 'surprise': 0.0, 'sadness': 0.0,
+                      'disgust': 0.0, 'joy': 0.0}
     for key in em_frequencies.keys():
         em_percent.update({key: float(em_frequencies[key]) / float(sum_values)})
     self.em_list = em_list
     self.em_dict = em_dict
     self.emotion_scores = dict(em_frequencies)
     self.em_frequencies = em_percent
 
@@ -57,28 +58,29 @@
     with urllib.request.urlopen("https://raw.githubusercontent.com/mmsa/EmoTFIDF/main/emotions_lex.json") as url:
         lexicon = json.loads(url.read().decode())
 
     def set_text(self, text):
         self.text = process_message(text)
         self.words = list(nltk.word_tokenize(self.text))
         self.sentences = list(nltk.sent_tokenize(self.text))
+        self.sent_flag = 0
         get_emotions(self)
 
-    def set_lexicon_path(self,path):
+    def set_lexicon_path(self, path):
         self.path = path
-        if path!=' ' and path!=0:
+        if path != ' ' and path != 0:
             with open(path) as jsonfile:
                 self.lexicon = json.load(jsonfile)
         else:
-            with urllib.request.urlopen("https://raw.githubusercontent.com/mmsa/EmoTFIDF/main/emotions_lex.json") as url:
+            with urllib.request.urlopen(
+                    "https://raw.githubusercontent.com/mmsa/EmoTFIDF/main/emotions_lex.json") as url:
                 self.lexicon = json.loads(url.read().decode())
 
-
-    def remove_sentiments(self,sent_flag):
-        self.sent_flag=sent_flag
+    def remove_sentiments(self, sent_flag):
+        self.sent_flag = sent_flag
 
     def computeTFIDF(self, docs):
         vectorizer = TfidfVectorizer(max_features=200, stop_words=stopwords.words('english'),
                                      token_pattern=r'(?u)\b[A-Za-z]+\b')
         vectors = vectorizer.fit_transform(docs)
         feature_names = vectorizer.get_feature_names()
         dense = vectors.todense()
@@ -97,22 +99,20 @@
     def get_emotfidf(self):
         self.get_ifidf_for_words()
         em_percent = {'fear': 0.0, 'anger': 0.0, 'anticipation': 0.0, 'trust': 0.0, 'surprise': 0.0, 'positive': 0.0,
                       'negative': 0.0, 'sadness': 0.0, 'disgust': 0.0, 'joy': 0.0}
         if self.sent_flag == 1:
             em_percent = {'fear': 0.0, 'anger': 0.0, 'anticipation': 0.0, 'trust': 0.0, 'surprise': 0.0, 'sadness': 0.0,
                           'disgust': 0.0, 'joy': 0.0}
-
         em_frequencies = Counter()
         for word in self.em_list:
             em_frequencies[word] += 1
         for e in self.em_dict.keys():
             if e in self.ifidf_for_words:
                 tfidf_weight = self.ifidf_for_words[e]
                 for a in self.em_dict[e]:
                     new_fre = round(em_frequencies[a] / tfidf_weight, 2)
                     em_frequencies[a] = new_fre
         sum_values = sum(em_frequencies.values())
         for key in em_frequencies.keys():
             em_percent.update({key: round(float(em_frequencies[key]) / float(sum_values), 3)})
         self.em_tfidf = em_percent
-
```

### Comparing `EmoTFIDF-1.0.8/PKG-INFO` & `EmoTFIDF-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EmoTFIDF
-Version: 1.0.8
+Version: 1.0.9
 Summary: A library to extract emotions using two methods, 1- Using lexicon based, counting frequency of emotion2- Integrating TFIDF to add a contextNote that lexicon license is for research purposes only.
 Home-page: https://github.com/mmsa/emotfidf
 Author: mmsa12
 Author-email: mmsa12@gmail.com
 License: UNKNOWN
 Description: EmoTFIDF is an emotion detection library (Lexicon approach) based in the National Research Council Canada (NRC) and this package is for research purposes only. Source: [lexicons for research] (http://sentiment.nrc.ca/lexicons-for-research/)
```

### Comparing `EmoTFIDF-1.0.8/README.md` & `EmoTFIDF-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `EmoTFIDF-1.0.8/setup.py` & `EmoTFIDF-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         nltk.download('wordnet')
         nltk.download('punkt')
         nltk.download('stopwords')
 
 
 setuptools.setup(
     name="EmoTFIDF",
-    version="1.0.8",
+    version="1.0.9",
     author="mmsa12",
     author_email="mmsa12@gmail.com",
     description="A library to extract emotions using two methods, 1- Using lexicon based, counting frequency of emotion"
                 "2- Integrating TFIDF to add a context"
                 "Note that lexicon license is for research purposes only.",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

