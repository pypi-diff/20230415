# Comparing `tmp/langful-0.22-py2.py3-none-any.whl.zip` & `tmp/langful-0.23-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 6765 bytes, number of entries: 9
--rw-rw-rw-  2.0 fat     1469 b- defN 23-Apr-13 11:45 langful/__init__.py
--rw-rw-rw-  2.0 fat      352 b- defN 23-Apr-13 11:13 langful/define.py
--rw-rw-rw-  2.0 fat     1556 b- defN 23-Mar-25 12:16 langful/functions.py
--rw-rw-rw-  2.0 fat     8834 b- defN 23-Apr-13 11:41 langful/lang.py
--rw-rw-rw-  2.0 fat     1064 b- defN 23-Apr-13 12:40 langful-0.22.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2605 b- defN 23-Apr-13 12:40 langful-0.22.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-Apr-13 12:40 langful-0.22.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Apr-13 12:40 langful-0.22.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      679 b- defN 23-Apr-13 12:40 langful-0.22.dist-info/RECORD
-9 files, 16677 bytes uncompressed, 5609 bytes compressed:  66.4%
+Zip file size: 7310 bytes, number of entries: 9
+-rw-rw-rw-  2.0 fat     1507 b- defN 23-Apr-15 03:44 langful/__init__.py
+-rw-rw-rw-  2.0 fat      340 b- defN 23-Apr-15 04:33 langful/define.py
+-rw-rw-rw-  2.0 fat     1590 b- defN 23-Apr-15 03:46 langful/function.py
+-rw-rw-rw-  2.0 fat    11341 b- defN 23-Apr-15 05:31 langful/lang.py
+-rw-rw-rw-  2.0 fat     1064 b- defN 23-Apr-15 05:32 langful-0.23.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2603 b- defN 23-Apr-15 05:32 langful-0.23.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-Apr-15 05:32 langful-0.23.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Apr-15 05:32 langful-0.23.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      679 b- defN 23-Apr-15 05:32 langful-0.23.dist-info/RECORD
+9 files, 19242 bytes uncompressed, 6156 bytes compressed:  68.0%
```

## zipnote {}

```diff
@@ -1,28 +1,28 @@
 Filename: langful/__init__.py
 Comment: 
 
 Filename: langful/define.py
 Comment: 
 
-Filename: langful/functions.py
+Filename: langful/function.py
 Comment: 
 
 Filename: langful/lang.py
 Comment: 
 
-Filename: langful-0.22.dist-info/LICENSE
+Filename: langful-0.23.dist-info/LICENSE
 Comment: 
 
-Filename: langful-0.22.dist-info/METADATA
+Filename: langful-0.23.dist-info/METADATA
 Comment: 
 
-Filename: langful-0.22.dist-info/WHEEL
+Filename: langful-0.23.dist-info/WHEEL
 Comment: 
 
-Filename: langful-0.22.dist-info/top_level.txt
+Filename: langful-0.23.dist-info/top_level.txt
 Comment: 
 
-Filename: langful-0.22.dist-info/RECORD
+Filename: langful-0.23.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## langful/__init__.py

```diff
@@ -83,9 +83,11 @@
 pypi: https://pypi.org/project/langful
 
 issues: https://github.com/cueavyqwp/langful/issues
 """
 
 # 'lang' object
 from langful.lang import *
-# Some functions for 'langful'
-from langful.functions import *
+# Some function for 'langful'
+from langful.function import *
+# define
+from langful.define import *
```

## langful/define.py

```diff
@@ -1,14 +1,20 @@
+"""
+# define
+"""
+
+# type
+JSON = "json"
+LANG = "lang"
+
 FILE = "file"
 DICT = "dict"
-
+# encode/decode
 UTF8 = "utf-8"
 
-def TheTypeError( obj , message : str = "" ) -> None : raise TypeError(f"{ message }can't use type { type( obj ) }")
-
 def get_type( obj ) -> str :
     if isinstance( obj , str ) :
         return FILE
     elif isinstance( obj , dict ) :
         return DICT
     else :
-        TheTypeError( obj )
+        raise TypeError(f"can't use type { type( obj ) }")
```

## langful/lang.py

```diff
@@ -1,70 +1,90 @@
+"""
+# lang
+"""
+import traceback
 import locale
 import json
 import os
 
 from langful.__init__ import *
 from langful.define import *
 
 class lang :
 
-    def __init__( self , lang_dir = "lang" , default_lang : str = "en_us" , file_suffix : str = ".json" , change : str = "%" ) -> None :
+    def __init__( self , lang_dir = "lang" , default_lang : str = "en_us" , file_type : str = JSON , change : str = "%" ) -> None :
         """
         # lang object
 
         ---
 
         lang_dir: Translation file storage directory / Translation file dictionary
 
         default_lang: Default translation
 
-        file_suffix: Such as '.json' or '.lang'
+        file_type: 'json' or 'lang'
 
         change: Specifies what character to use for substitution , default is '%'
 
         ---
 
         lang_dir: 翻译文件的存放目录 / 翻译文件字典
 
         default_lang: 默认使用的翻译
 
-        file_suffix: 文件后缀 例如 '.json' '.lang' '.txt' 等等
+        file_type: 文件后缀 'json' 或 'lang'
 
         change: 选择用什么符号做替换 默认为'%'
 
         """
 
         default_locale = locale.getdefaultlocale()[0].lower() # 默认语言
         self.type = get_type( lang_dir )
 
         if self.type == FILE :
 
+            file_suffix = f".{file_type}"
+
             if not os.path.exists( lang_dir ) : # 判断lang文件夹是否存在
                 raise KeyError( f"'{lang_dir}' dir not find" )
             if not len( os.listdir(lang_dir) ) :
                 raise FileNotFoundError( f"'{lang_dir}' has no file!" ) # lang文件夹里没有语言文件
             if not os.path.exists( os.path.join( lang_dir , default_lang + file_suffix ) ) : # 判断default_lang文件是否存在
                 raise KeyError( f"'{default_lang}' not find" )
 
             lang_file = os.path.join( lang_dir , default_locale + file_suffix )
-            file_suffix_len=len(file_suffix)
+            file_suffix_len = len( file_suffix )
             lang_file_list = []
             language_dict = {}
             use_locale = default_locale
             if not os.path.exists( lang_file ) : # 若默认语言不存在对应的本地化 那么就选用默认语言文件
                 use_locale = default_lang
                 lang_file = default_lang + file_suffix
 
             for filename in os.listdir(lang_dir): # 尝试加载所有能加载的模块
-                if len( filename ) > file_suffix_len and filename[-file_suffix_len:] == file_suffix :
+                if len( filename ) > file_suffix_len and filename[ -file_suffix_len: ] == file_suffix :
                     try :
                         with open( os.path.join( lang_dir , filename ) , encoding = UTF8 ) as file :
-                            language_dict[ filename[ :-file_suffix_len ] ] = json.load( file ) # 加载文件
+                            if file_type == JSON :
+                                l = json.load( file ) # 直接加载JSON文件
+                            elif file_type == LANG :
+                                l = {}
+                                for i in file.read().split( "\n" ) : # 去换行
+                                    if i :
+                                        k , v = i.split( "=" ) # 键 = 值
+                                        if v and v[0] == " " : # 去空格
+                                            v = v[ 1: ]
+                                        l[ "".join( k.split() ) ] = v
+                            else :
+                                raise TypeError( f"can't use type '{file_type}'" )
+                        language_dict[ filename[ :-file_suffix_len ] ] = l # 加载文件
                         lang_file_list.append( filename )
-                    except : pass
+                    except Exception as e :
+                        print( f"{e}\n" )
+                        traceback.print_exc()
 
         elif self.type == DICT :
             use_locale = default_lang
             if default_lang not in lang_dir :
                 raise KeyError( f"'{default_lang}' not find" )
             if default_locale in lang_dir :
                 use_locale = default_locale
@@ -86,17 +106,17 @@
         # use_locale: 选定的语言
         self.use_locale = use_locale
         # change: Specifies what character to use for substitution , default is '%'
         # change: 选择用什么符号做替换 默认为'%'
         self.change = change
 
         if self.type == FILE :
-            #file_suffix: Such as '.json' '.lang'
-            #file_suffix: 文件后缀 例如 '.json' '.lang'
-            self.file_suffix = file_suffix
+            #file_type: 'json' or 'lang'
+            #file_type: 'json' 或 'lang'
+            self.file_type = file_type
             # lang_file: Choose to use's language file
             # lang_file: 选择使用的语言文件
             self.lang_file = lang_file
             # lang_file_list: All can find's language file
             # lang_file_list: 所有能找到的语言文件
             self.lang_file_list = lang_file_list
 
@@ -106,17 +126,48 @@
         # lang_str_list: All can find's language file's name
         # lang_str_list: 所有能找到的语言文件的名字
         self.lang_str_list = list( self.language_dict.keys() )
     def _language_reload( self ) -> None :
         # language: Load need's language file
         # language: 加载需要的语言文件
         self.language = self.language_dict[ self.use_locale ]
+    def _file_suffix_reload( self ) -> None :
+        #file_suffix: Such as '.json' '.lang'
+        #file_suffix: 文件后缀 例如 '.json' '.lang'
+        if self.type == FILE :
+            self.file_suffix = "." + self.file_type
     def _reload( self ) -> None :
         self._lang_str_list_reload()
         self._language_reload()
+        self._file_suffix_reload()
+
+    def _lang_str_to_language( self , lang_str ) -> dict :
+        if not lang_str :
+            lang_str = self.use_locale
+        if lang_str in self.lang_str_list :
+            return self.language_dict[ lang_str ]
+        else :
+            raise KeyError( f"lang '{lang_str}' has not find!" )
+
+    def save( self ) -> None :
+        if self.type == FILE :
+            for k , v in self.language_dict.items() :
+                try :
+                    with open( os.path.join( self.lang_dir , k + self.file_suffix ) , "w+" , encoding = UTF8 ) as file :
+                        if self.file_type == JSON :
+                            file.write( json.dumps( v , indent=4 , ensure_ascii = False ) )
+                        elif self.file_type == LANG :
+                            for i_k , i_v in v.items() :
+                                s = f"{i_k} = {i_v}\n"
+                                file.write( s )
+                except Exception as e :
+                    print( f"{e}\n" )
+                    traceback.print_exc()
+        else :
+            raise TypeError( f"{self.type} can't to save" )
 
     def get( self , key:str , lang_str:str = None ) -> str : # 输入键 获取对应的值
         """
 
         # get
 
         Get one value in some one dictionary
@@ -179,49 +230,68 @@
 
         if lang_str in self.lang_str_list :
             self.language_dict[ lang_str ] [ key ] = value
 
         else :
             raise KeyError( f"lang '{lang_str}' has not find!" )
 
-    def add( self , lang_str : str , set : dict = {} ) -> None :
+    def add( self , lang_str : str , set : dict = {} , change_file : bool = False ) -> None :
         """
 
         # add a new language
 
         lang_str: the language's name
 
         set: the language dictionary
 
-        ps: It can't change the file
+        change_file: modify the file
 
         ---
 
         # 添加新语言
 
         lang_str: 语言名称
 
         set: 语言字典
 
-        ps: 它不会影响文件
+        change_file: 是否修改文件
 
         """
         self.language_dict[ lang_str ] = set
         if lang_str == self.default_locale :
             self.use_locale = lang_str
+        if self.type == FILE and change_file :
+            self.save()
         self._reload()
 
-    def remove( self , lang_str : str ) -> None : #todo
+    def remove( self , lang_str : str , change_file : bool = False ) -> None :
         """
-        # todo
+
+        # remove a language
+
+        lang_str: the language's name
+
+        change_file: modify the file
+
+        ---
+
+        # 移除语言
+
+        lang_str: 语言名称
+
+        change_file: 是否修改文件
+
         """
         if lang_str == self.use_locale or lang_str == self.default_lang or lang_str == self.default_locale :
             raise RuntimeError( f"can't remove '{lang_str}' " )
         del self.language_dict[ lang_str ]
         del self.lang_str_list[ self.lang_str_list.index( lang_str ) ]
+        if self.type == FILE and change_file :
+            self.save()
+        self._reload()
 
     def replace( self , * args : str , lang_str : str = None , change : str = None ) -> str : # 替换字符串 使用%号
         """
 
         Replace string with some one dictionary
 
         用某个字典替换字符串
@@ -247,26 +317,18 @@
         lang_str: 例如 'zh_cn' 或 'en_us' 等等
 
         change: 选择用什么符号做替换 默认为'%'
         """
         if not change :
             change = self.change
 
-        if not lang_str :
-            lang_str = self.use_locale
-
-        if lang_str in self.lang_str_list :
-            language = self.language_dict[ lang_str ]
-
-        else :
-            raise KeyError( f"lang '{lang_str}' has not find!" )
-
         i = 0
         Ret = ""
         text = "".join( args ).split( change )
+        language = self._lang_str_to_language( lang_str )
 
         for I in text :
             if i % 2 :
                 if I in language :
                     Ret += language[I]
                 elif not I :
                     Ret += change
```

## Comparing `langful-0.22.dist-info/LICENSE` & `langful-0.23.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `langful-0.22.dist-info/METADATA` & `langful-0.23.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langful
-Version: 0.22
+Version: 0.23
 Home-page: https://github.com/cueavyqwp/langful
 Author: cueavyqwp
 Author-email: cueavyqwp@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: > 3.6
@@ -28,15 +28,14 @@
     </a>
     <a href="https://github.com/cueavyqwp/langful">
         <img alt="Github issues" src="https://img.shields.io/github/issues/cueavyqwp/langful?color=blue">
     </a>
 
 </p>
 
-
 # install
 
 Use `pip` to install `pip install langful` or `pip3 install langful`
 
 # example
 
 - test.py
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: langful Version: 0.22 Home-page: https://
+Metadata-Version: 2.1 Name: langful Version: 0.23 Home-page: https://
 github.com/cueavyqwp/langful Author: cueavyqwp Author-email:
 cueavyqwp@outlook.com Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: > 3.6 Description-Content-Type: text/
 markdown License-File: LICENSE # langful
    [PyPI_version] [Python_version] [license] [Github_stars] [Github_issues]
 # install Use `pip` to install `pip install langful` or `pip3 install langful`
```

