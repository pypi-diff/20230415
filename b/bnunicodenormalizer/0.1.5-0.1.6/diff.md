# Comparing `tmp/bnunicodenormalizer-0.1.5.tar.gz` & `tmp/bnunicodenormalizer-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bnunicodenormalizer-0.1.5.tar", last modified: Sat Dec 31 20:16:24 2022, max compression
+gzip compressed data, was "bnunicodenormalizer-0.1.6.tar", last modified: Sat Apr 15 15:18:24 2023, max compression
```

## Comparing `bnunicodenormalizer-0.1.5.tar` & `bnunicodenormalizer-0.1.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 ansary    (1000) ansary    (1000)        0 2022-12-31 20:16:24.684518 bnunicodenormalizer-0.1.5/
--rw-rw-r--   0 ansary    (1000) ansary    (1000)     2726 2022-12-31 20:00:33.000000 bnunicodenormalizer-0.1.5/CHANGELOG.txt
--rw-rw-r--   0 ansary    (1000) ansary    (1000)     1067 2022-02-15 05:44:06.000000 bnunicodenormalizer-0.1.5/LICENSE
--rw-rw-r--   0 ansary    (1000) ansary    (1000)       25 2022-02-12 04:15:33.000000 bnunicodenormalizer-0.1.5/MANIFEST.in
--rw-rw-r--   0 ansary    (1000) ansary    (1000)    20474 2022-12-31 20:16:24.684518 bnunicodenormalizer-0.1.5/PKG-INFO
--rw-rw-r--   0 ansary    (1000) ansary    (1000)    17137 2022-12-31 19:51:24.000000 bnunicodenormalizer-0.1.5/README.md
-drwxrwxr-x   0 ansary    (1000) ansary    (1000)        0 2022-12-31 20:16:24.680519 bnunicodenormalizer-0.1.5/bnunicodenormalizer/
--rw-rw-r--   0 ansary    (1000) ansary    (1000)      190 2022-10-21 00:24:37.000000 bnunicodenormalizer-0.1.5/bnunicodenormalizer/__init__.py
--rw-rw-r--   0 ansary    (1000) ansary    (1000)    13947 2022-10-21 03:53:23.000000 bnunicodenormalizer-0.1.5/bnunicodenormalizer/base.py
--rw-rw-r--   0 ansary    (1000) ansary    (1000)     1923 2022-12-31 19:53:42.000000 bnunicodenormalizer-0.1.5/bnunicodenormalizer/indic.py
--rw-rw-r--   0 ansary    (1000) ansary    (1000)    43385 2022-12-31 20:11:20.000000 bnunicodenormalizer-0.1.5/bnunicodenormalizer/langs.py
--rw-rw-r--   0 ansary    (1000) ansary    (1000)    20282 2022-09-10 06:09:29.000000 bnunicodenormalizer-0.1.5/bnunicodenormalizer/normalizer.py
-drwxrwxr-x   0 ansary    (1000) ansary    (1000)        0 2022-12-31 20:16:24.684518 bnunicodenormalizer-0.1.5/bnunicodenormalizer.egg-info/
--rw-rw-r--   0 ansary    (1000) ansary    (1000)    20474 2022-12-31 20:16:24.000000 bnunicodenormalizer-0.1.5/bnunicodenormalizer.egg-info/PKG-INFO
--rw-rw-r--   0 ansary    (1000) ansary    (1000)      438 2022-12-31 20:16:24.000000 bnunicodenormalizer-0.1.5/bnunicodenormalizer.egg-info/SOURCES.txt
--rw-rw-r--   0 ansary    (1000) ansary    (1000)        1 2022-12-31 20:16:24.000000 bnunicodenormalizer-0.1.5/bnunicodenormalizer.egg-info/dependency_links.txt
--rw-rw-r--   0 ansary    (1000) ansary    (1000)       20 2022-12-31 20:16:24.000000 bnunicodenormalizer-0.1.5/bnunicodenormalizer.egg-info/top_level.txt
-drwxrwxr-x   0 ansary    (1000) ansary    (1000)        0 2022-12-31 20:16:24.684518 bnunicodenormalizer-0.1.5/extra/
--rw-rw-r--   0 ansary    (1000) ansary    (1000)    57070 2022-10-21 02:59:20.000000 bnunicodenormalizer-0.1.5/extra/conjuncts.py
--rw-rw-r--   0 ansary    (1000) ansary    (1000)     3002 2022-06-15 05:35:07.000000 bnunicodenormalizer-0.1.5/extra/missing.txt
--rw-rw-r--   0 ansary    (1000) ansary    (1000)       38 2022-12-31 20:16:24.684518 bnunicodenormalizer-0.1.5/setup.cfg
--rw-rw-r--   0 ansary    (1000) ansary    (1000)     1044 2022-12-31 20:00:39.000000 bnunicodenormalizer-0.1.5/setup.py
-drwxrwxr-x   0 ansary    (1000) ansary    (1000)        0 2022-12-31 20:16:24.684518 bnunicodenormalizer-0.1.5/tests/
--rw-rw-r--   0 ansary    (1000) ansary    (1000)     5521 2022-09-10 17:59:24.000000 bnunicodenormalizer-0.1.5/tests/test_normalizer.py
+drwxrwxr-x   0 ansary    (1000) ansary    (1000)        0 2023-04-15 15:18:24.621163 bnunicodenormalizer-0.1.6/
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)     2793 2023-04-15 15:16:57.000000 bnunicodenormalizer-0.1.6/CHANGELOG.txt
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)     1067 2022-02-15 05:44:06.000000 bnunicodenormalizer-0.1.6/LICENSE
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)       25 2022-02-12 04:15:33.000000 bnunicodenormalizer-0.1.6/MANIFEST.in
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)    20541 2023-04-15 15:18:24.621163 bnunicodenormalizer-0.1.6/PKG-INFO
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)    17137 2022-12-31 19:51:24.000000 bnunicodenormalizer-0.1.6/README.md
+drwxrwxr-x   0 ansary    (1000) ansary    (1000)        0 2023-04-15 15:18:24.617163 bnunicodenormalizer-0.1.6/bnunicodenormalizer/
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)      190 2022-10-21 00:24:37.000000 bnunicodenormalizer-0.1.6/bnunicodenormalizer/__init__.py
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)    13947 2022-10-21 03:53:23.000000 bnunicodenormalizer-0.1.6/bnunicodenormalizer/base.py
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)     1923 2022-12-31 19:53:42.000000 bnunicodenormalizer-0.1.6/bnunicodenormalizer/indic.py
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)    43487 2023-04-15 15:16:57.000000 bnunicodenormalizer-0.1.6/bnunicodenormalizer/langs.py
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)    20883 2023-04-15 15:16:57.000000 bnunicodenormalizer-0.1.6/bnunicodenormalizer/normalizer.py
+drwxrwxr-x   0 ansary    (1000) ansary    (1000)        0 2023-04-15 15:18:24.617163 bnunicodenormalizer-0.1.6/bnunicodenormalizer.egg-info/
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)    20541 2023-04-15 15:18:24.000000 bnunicodenormalizer-0.1.6/bnunicodenormalizer.egg-info/PKG-INFO
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)      438 2023-04-15 15:18:24.000000 bnunicodenormalizer-0.1.6/bnunicodenormalizer.egg-info/SOURCES.txt
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)        1 2023-04-15 15:18:24.000000 bnunicodenormalizer-0.1.6/bnunicodenormalizer.egg-info/dependency_links.txt
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)       20 2023-04-15 15:18:24.000000 bnunicodenormalizer-0.1.6/bnunicodenormalizer.egg-info/top_level.txt
+drwxrwxr-x   0 ansary    (1000) ansary    (1000)        0 2023-04-15 15:18:24.621163 bnunicodenormalizer-0.1.6/extra/
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)    57070 2022-10-21 02:59:20.000000 bnunicodenormalizer-0.1.6/extra/conjuncts.py
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)     3002 2022-06-15 05:35:07.000000 bnunicodenormalizer-0.1.6/extra/missing.txt
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)       38 2023-04-15 15:18:24.621163 bnunicodenormalizer-0.1.6/setup.cfg
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)     1044 2023-04-15 15:16:57.000000 bnunicodenormalizer-0.1.6/setup.py
+drwxrwxr-x   0 ansary    (1000) ansary    (1000)        0 2023-04-15 15:18:24.621163 bnunicodenormalizer-0.1.6/tests/
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)     5521 2022-09-10 17:59:24.000000 bnunicodenormalizer-0.1.6/tests/test_normalizer.py
```

### Comparing `bnunicodenormalizer-0.1.5/CHANGELOG.txt` & `bnunicodenormalizer-0.1.6/CHANGELOG.txt`

 * *Files 2% similar despite different names*

```diff
@@ -131,8 +131,12 @@
 
 0.1.4 (01/01/23)
 -------------------
 - added sylhetinagri 
 
 0.1.5 (01/01/23)
 -------------------
-- cleaned panjabi double quotes in diac map 
+- cleaned panjabi double quotes in diac map 
+
+0.1.6 (15/04/23)
+-------------------
+- added bangla punctuations
```

### Comparing `bnunicodenormalizer-0.1.5/LICENSE` & `bnunicodenormalizer-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `bnunicodenormalizer-0.1.5/PKG-INFO` & `bnunicodenormalizer-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bnunicodenormalizer
-Version: 0.1.5
+Version: 0.1.6
 Summary: Bangla Unicode Normalization Toolkit
 Home-page: https://github.com/mnansary/bnUnicodeNormalizer
 Author: Bengali.AI
 Author-email: research.bengaliai@gmail.com
 License: MIT
 Keywords: bangla,unicode,text normalization,indic
 Platform: UNKNOWN
@@ -545,7 +545,11 @@
 -------------------
 - added sylhetinagri 
 
 0.1.5 (01/01/23)
 -------------------
 - cleaned panjabi double quotes in diac map 
 
+0.1.6 (15/04/23)
+-------------------
+- added bangla punctuations 
+
```

### Comparing `bnunicodenormalizer-0.1.5/README.md` & `bnunicodenormalizer-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `bnunicodenormalizer-0.1.5/bnunicodenormalizer/base.py` & `bnunicodenormalizer-0.1.6/bnunicodenormalizer/base.py`

 * *Files identical despite different names*

### Comparing `bnunicodenormalizer-0.1.5/bnunicodenormalizer/indic.py` & `bnunicodenormalizer-0.1.6/bnunicodenormalizer/indic.py`

 * *Files identical despite different names*

### Comparing `bnunicodenormalizer-0.1.5/bnunicodenormalizer/langs.py` & `bnunicodenormalizer-0.1.6/bnunicodenormalizer/langs.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     nukta                  =   '়'
     vowels                 =   ['অ', 'আ', 'ই', 'ঈ', 'উ', 'ঊ', 'ঋ', 'এ', 'ঐ', 'ও', 'ঔ']
     consonants             =   ['ক', 'খ', 'গ', 'ঘ', 'ঙ', 'চ', 'ছ','জ', 'ঝ', 'ঞ', 'ট', 'ঠ', 'ড', 'ঢ', 'ণ', 'ত', 'থ', 'দ', 'ধ', 'ন', 
                                 'প', 'ফ', 'ব', 'ভ', 'ম', 'য', 'র', 'ল', 'শ', 'ষ', 'স', 'হ','ড়', 'ঢ়', 'য়','ৎ']
     vowel_diacritics       =   ['া', 'ি', 'ী', 'ু', 'ূ', 'ৃ', 'ে', 'ৈ', 'ো', 'ৌ']
     consonant_diacritics   =   ['ঁ', 'ং', 'ঃ']
     numbers                =   ['০', '১', '২', '৩', '৪', '৫', '৬', '৭', '৮', '৯']
-    punctuations           =   [',',';','।','?','!',':','—',':-',"'",'”','(', ')','{', '}','[',']','√','<','>','=','...','.','-']
+    punctuations           =   ['!', '"', "'", '(', ')', ',', '-', '.', '...', ':', ':-', ';', '<', '=', '>', '?', '[', ']', '{', '}', '।', '৷', '–', '—', '”', '√']
     symbols                =   ['৳']
     connector              =   '্'
     
     # based on unicode range : \u0980-\u09FF
     non_gylph_unicodes     =   ['\u0984', '\u098d','\u098e','\u0991','\u0992','\u09a9','\u09b1','\u09b3','\u09b4','\u09b5',
                                 '\u09ba','\u09bb', '\u09c5','\u09c6','\u09c9','\u09ca','\u09cf','\u09d0','\u09d1','\u09d2',
                                 '\u09d3','\u09d4','\u09d5','\u09d6', '\u09d8','\u09d9','\u09da','\u09db','\u09de', '\u09e4',
@@ -552,15 +552,16 @@
     #---------------------------------------------------changeables----------------------------------------------------------------
     conjuncts              =   []
     # this is a customizeable map : this map is purely based on visual similiarity
     legacy_maps            =   {}
     #---------------------------------------------------changeables----------------------------------------------------------------
     #---------------------------------------------------normalization maps---------------------------------------------------------
     nukta_map              =   {}
-    diacritic_map          =   {}
+    diacritic_map           =   {'ꠦꠣ':'ꠧ',
+                                'ꠣꠦ':'ꠧ'}
     #---------------------------------------------------normalization maps---------------------------------------------------------
     diacritics             =   sorted(vowel_diacritics+consonant_diacritics)
     used                   =   sorted(vowels+consonants+vowel_diacritics+consonant_diacritics+numbers)
     valid                  =   sorted([' ']+used+punctuations+[connector]+["\u200d","\u200c"])
     complex_roots          =   sorted([' ']+vowels+consonants+numbers+punctuations+symbols+conjuncts)
     # these unicodes can not start a word
     invalid_starts         =   sorted(diacritics+[connector])
```

### Comparing `bnunicodenormalizer-0.1.5/bnunicodenormalizer/normalizer.py` & `bnunicodenormalizer-0.1.6/bnunicodenormalizer/normalizer.py`

 * *Files 3% similar despite different names*

```diff
@@ -82,20 +82,27 @@
 
         super(Normalizer,self).__init__(language="bangla",
                                         allow_english=allow_english,
                                         keep_legacy_symbols=keep_legacy_symbols,
                                         legacy_maps=legacy_maps)
         #-------------------------------------------------extended ops----------------------
         # assemese 
-        self.assamese_map={'ৰ':'র','ৱ':'ব'}
+        self.assamese_map                               =       {'ৰ':'র','ৱ':'ব'}
         self.word_level_ops["AssameseReplacement"]      =       self.replaceAssamese
+        # punctuations
+        self.punctuations_map                           =   {'"': '"' ,
+                                                            '৷' : '।',
+                                                            '–' : '-',
+                                                            "'" : "'",
+                                                            "'" : "'"}
+        self.word_level_ops["PunctuationReplacement"]   =       self.replacePunctuations
         
         # to+hosonto case
         '''
-
+n
             case-1:     if 'ত'+hosonto is followed by anything other than a consonant the word is an invalid word
 
             case-2:     The ত্‍ symbol which should be replaced by a 'ৎ' occurs for all consonants except:ত,থ,ন,ব,ম,য,র
                         # code to verify this manually 
                         for c in self.consonants:
                             print('ত'+ self.lang.connector+c)
  
@@ -111,14 +118,17 @@
         # complex root cleanup 
         self.decomp_level_ops["ComplexRootNormalization"]          =       self.convertComplexRoots
 
         
 #-------------------------word ops----------------------------------------------------------------------------- 
     def replaceAssamese(self):
         self.replaceMaps(self.assamese_map)
+    
+    def replacePunctuations(self):
+        self.replaceMaps(self.punctuations_map)
                         
 #-------------------------unicode ops-----------------------------------------------------------------------------    
     def cleanConsonantDiacritics(self):
         # consonant diacritics
         for idx,d in enumerate(self.decomp):
             if idx<len(self.decomp)-1:
                 if d in self.lang.consonant_diacritics and self.decomp[idx+1] in self.lang.consonant_diacritics:
```

### Comparing `bnunicodenormalizer-0.1.5/bnunicodenormalizer.egg-info/PKG-INFO` & `bnunicodenormalizer-0.1.6/bnunicodenormalizer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bnunicodenormalizer
-Version: 0.1.5
+Version: 0.1.6
 Summary: Bangla Unicode Normalization Toolkit
 Home-page: https://github.com/mnansary/bnUnicodeNormalizer
 Author: Bengali.AI
 Author-email: research.bengaliai@gmail.com
 License: MIT
 Keywords: bangla,unicode,text normalization,indic
 Platform: UNKNOWN
@@ -545,7 +545,11 @@
 -------------------
 - added sylhetinagri 
 
 0.1.5 (01/01/23)
 -------------------
 - cleaned panjabi double quotes in diac map 
 
+0.1.6 (15/04/23)
+-------------------
+- added bangla punctuations 
+
```

### Comparing `bnunicodenormalizer-0.1.5/extra/conjuncts.py` & `bnunicodenormalizer-0.1.6/extra/conjuncts.py`

 * *Files identical despite different names*

### Comparing `bnunicodenormalizer-0.1.5/extra/missing.txt` & `bnunicodenormalizer-0.1.6/extra/missing.txt`

 * *Files identical despite different names*

### Comparing `bnunicodenormalizer-0.1.5/setup.py` & `bnunicodenormalizer-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
   'Operating System :: OS Independent',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='bnunicodenormalizer',
-  version='0.1.5',
+  version='0.1.6',
   description='Bangla Unicode Normalization Toolkit',
   long_description=open('README.md',encoding='utf-8').read() + '\n\n' + open('CHANGELOG.txt',encoding='utf-8').read(),
   long_description_content_type='text/markdown',
   url='https://github.com/mnansary/bnUnicodeNormalizer',  
   author='Bengali.AI',
   author_email='research.bengaliai@gmail.com',
   license='MIT',
```

### Comparing `bnunicodenormalizer-0.1.5/tests/test_normalizer.py` & `bnunicodenormalizer-0.1.6/tests/test_normalizer.py`

 * *Files identical despite different names*

