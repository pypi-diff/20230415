# Comparing `tmp/systempath-1.0.6-py3-none-any.whl.zip` & `tmp/systempath-1.0a8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 26253 bytes, number of entries: 7
--rw-r--r--  2.0 unx    63591 b- defN 23-Apr-15 04:52 systempath/__init__.py
--rw-r--r--  2.0 unx    39953 b- defN 23-Apr-15 04:52 systempath/i systempath.py
--rw-r--r--  2.0 unx    11389 b- defN 23-Apr-15 04:52 systempath-1.0.6.dist-info/LICENSE
--rw-r--r--  2.0 unx     2083 b- defN 23-Apr-15 04:52 systempath-1.0.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-15 04:52 systempath-1.0.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Apr-15 04:52 systempath-1.0.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      566 b- defN 23-Apr-15 04:52 systempath-1.0.6.dist-info/RECORD
-7 files, 117685 bytes uncompressed, 25255 bytes compressed:  78.5%
+Zip file size: 27097 bytes, number of entries: 7
+-rw-r--r--  2.0 unx    66968 b- defN 23-Feb-11 00:51 systempath/__init__.py
+-rw-r--r--  2.0 unx    39467 b- defN 23-Feb-11 00:51 systempath/gqylpy systempath.py
+-rw-r--r--  2.0 unx    11389 b- defN 23-Feb-11 00:52 systempath-1.0a8.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2083 b- defN 23-Feb-11 00:52 systempath-1.0a8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Feb-11 00:52 systempath-1.0a8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Feb-11 00:52 systempath-1.0a8.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      571 b- defN 23-Feb-11 00:52 systempath-1.0a8.dist-info/RECORD
+7 files, 120581 bytes uncompressed, 26089 bytes compressed:  78.4%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: systempath/__init__.py
 Comment: 
 
-Filename: systempath/i systempath.py
+Filename: systempath/gqylpy systempath.py
 Comment: 
 
-Filename: systempath-1.0.6.dist-info/LICENSE
+Filename: systempath-1.0a8.dist-info/LICENSE
 Comment: 
 
-Filename: systempath-1.0.6.dist-info/METADATA
+Filename: systempath-1.0a8.dist-info/METADATA
 Comment: 
 
-Filename: systempath-1.0.6.dist-info/WHEEL
+Filename: systempath-1.0a8.dist-info/WHEEL
 Comment: 
 
-Filename: systempath-1.0.6.dist-info/top_level.txt
+Filename: systempath-1.0a8.dist-info/top_level.txt
 Comment: 
 
-Filename: systempath-1.0.6.dist-info/RECORD
+Filename: systempath-1.0a8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## systempath/__init__.py

```diff
@@ -14,15 +14,15 @@
     >>> file: File = home['alpha.txt']
     >>> file
     /home/gqylpy/alpha.txt
 
     >>> file.open.rb().read()
     b'GQYLPY \xe6\x94\xb9\xe5\x8f\x98\xe4\xb8\x96\xe7\x95\x8c'
 
-    @version: 1.0.6
+    @version: 1.0.alpha8
     @author: 竹永康 <gqylpy@outlook.com>
     @source: https://github.com/gqylpy/systempath
 
 ────────────────────────────────────────────────────────────────────────────────
 Copyright (c) 2022, 2023 GQYLPY <http://gqylpy.com>. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
@@ -63,15 +63,16 @@
             dir_fd:          Optional[int]  = None,
             follow_symlinks: Optional[bool] = None
     ):
         """
         @param name
             A path link, hopefully absolute. If it is a relative path, the
             current working directory is used as the parent directory (the
-            return value of `os.getcwd()`).
+            return value of `os.getcwd()`). The current working directory is
+            used by default.
 
         @param autoabs
             Automatically normalize the path link and convert to absolute path,
             at initialization. Default False. It is always recommended that you
             enable the parameter when the passed path is a relative path.
 
         @param strict
@@ -737,34 +738,32 @@
         try:
             return self[name]
         except SystemPathNotFoundError:
             raise AttributeError
 
     def __getitem__(
             self, name: BytesOrStr
-    ) -> Union['SystemPath', 'Directory', 'File', Path]:
+    ) -> Union['SystemPath', 'Directory', 'File']:
         path: PathLink = os.path.join(self.name, name)
 
         if self.strict:
             if os.path.isdir(path):
                 return Directory(path, strict=self.strict)
             if os.path.isfile(path):
                 return File(path)
-            if os.path.exists(name):
-                return Path(name)
-            else:
+            if not os.path.exists(path):
                 raise SystemPathNotFoundError
         else:
             return SystemPath(path)
 
     def __delitem__(self, name: BytesOrStr) -> None:
         Path(os.path.join(self.name, name)).delete()
 
     def __iter__(self) -> Generator:
-        return self.subpaths
+        return self.subpath
 
     @staticmethod
     def home(
             *,
             strict:          Optional[bool] = None,
             follow_symlinks: Optional[bool] = None
     ) -> 'Directory':
@@ -774,15 +773,15 @@
 
     @property
     def subpaths(self) -> Generator:
         """Get the instances of `Directory` or `File` for all subpaths (single
         layer) in the directory."""
 
     @property
-    def subpath_names(self) -> List[BytesOrStr]:
+    def subpaths_names(self) -> List[BytesOrStr]:
         """Get the names of all subpaths (single layer) in the directory. Call
         `os.listdir` internally."""
 
     def scandir(self) -> Iterator[os.DirEntry]:
         """Get instances of `os.DirEntry` for all files and subdirectories
         (single layer) in the directory, call `os.scandir` internally."""
 
@@ -1050,15 +1049,15 @@
         @param bufsize
             The buffer size, the length of each copy, default is 64K (if your
             platform is Windows then 1M). Passing -1 turns off buffering.
 
         @return: The parameter `dst` is passed in, without any modification.
         """
         warnings.warn(
-            f'will be deprecated soon, replaced to {self.contents.copy}.',
+            f'will be deprecated soon, replaced to {self.content.copy}.',
             DeprecationWarning
         )
 
     def link(self, dst: Union['File', PathLink], /) -> Union['File', PathLink]:
         """
         Create a hard link to the file, call `os.link` internally.
 
@@ -1081,18 +1080,18 @@
         os.truncate(self.name, length)
 
     def clear(self) -> None:
         self.truncate(0)
 
     def mknod(
             self,
-            mode:          Optional[int]  = None,
+            mode:          int  = None,
             *,
-            device:        Optional[int]  = None,
-            ignore_exists: Optional[bool] = None
+            device:        int  = None,
+            ignore_exists: bool = None
     ) -> None:
         """
         Create the file, call `os.mknod` internally, but if your platform is
         Windows then internally call `open(self.name, 'x')`.
 
         @param mode
             Specify the access permissions of the file, can be a permission
@@ -1108,48 +1107,50 @@
             If the file already exists, call this method will raise
             `FileExistsError`. But, if this parameter is set to True then
             silently skip. Default False.
         """
 
     def mknods(
             self,
-            mode:          Optional[int]  = None,
+            mode:          int  = None,
             *,
-            device:        Optional[int]  = None,
-            ignore_exists: Optional[bool] = None
+            device:        int  = None,
+            ignore_exists: bool = None
     ) -> None:
         """Create the file and all intermediate paths, super version of
         `self.mknod`."""
-        self.dirname.makedirs(mode, exist_ok=True)
+        parentdir = Directory(self.dirname)
+        if not parentdir.exists:
+            parentdir.makedirs(mode)
         self.mknod(mode, device=device, ignore_exists=ignore_exists)
 
     def remove(self, *, ignore_errors: Optional[bool] = None) -> None:
         """
         Remove the file, call `os.remove` internally.
 
         @param ignore_errors
             If the file does not exist will raise `FileNotFoundError`, can set
             this parameter to True to silence the exception. Default False.
         """
 
     def unlink(self) -> None:
-        """Remove the file, like `self.remove`, call `os.unlink` internally."""
+        os.unlink(self.name, dir_fd=self.dir_fd)
 
 
 class Open:
     """
     Open a file and return a file stream (or called handle).
 
     >>> f: BinaryIO = Open('alpha.bin').rb()  # open for reading in binary mode.
     >>> f: TextIO   = Open('alpha.txt').r()   # open for reading in text mode.
 
-    Pass in an instance of `File` (or a file path link) at instantiation time.
-    At instantiation time (do nothing) the file will not be opened, only when
-    you call one of the following methods, the file will be opened (call once,
-    open once), open mode equals method name (where method `rb_plus` equals mode
+    Pass in an instance of `File` (or a file path) at instantiation time. At
+    instantiation time (do nothing) the file will not be opened, only when you
+    call one of the following methods, the file will be opened (call once, open
+    once), open mode equals method name (where method `rb_plus` equals mode
     "rb+").
 
     ============================== IN BINARY MODE ==============================
     | Method  | Description                                                    |
     ----------------------------------------------------------------------------
     | rb      | open to read, if the file does not exist then raise            |
     |         | `FileNotFoundError`                                            |
@@ -1460,15 +1461,15 @@
     def read(self, size: int = -1, /) -> bytes:
         return Open(self.file).rb().read(size)
 
     def overwrite(self, content: Union['Content', bytes], /) -> None:
         """Overwrite the current file content from another file content (or a
         bytes object)."""
 
-    def append(self, content: Union['Content', bytes], /) -> None:
+    def append(self, content: Union['Content', bytes]) -> None:
         """Append the another file contents (or a bytes object) to the current
         file."""
 
     def copy(
             self,
             dst:     Union['Content', BinaryIO],
             /, *,
@@ -1538,35 +1539,85 @@
 
 
 class SystemPath(Directory, File):
 
     def __init__(
             self,
             root:    Optional[PathLink] = None,
-            /, *,
-            autoabs: Optional[bool]     = None,
-            strict:  Optional[bool]     = None
+            /,
+            autoabs: Optional[bool]     = False,
+            strict:  Optional[bool]     = False
     ):
         super().__init__(
-            '.' if root in (None, '') else b'.' if root == b'' else root,
+            '.' if root == '' else b'.' if root == b'' else root,
             autoabs=autoabs,
             strict =strict
         )
 
 
 class _xe6_xad_x8c_xe7_x90_xaa_xe6_x80_xa1_xe7_x8e_xb2_xe8_x90_x8d_xe4_xba_x91:
-    gpath = f'{__name__}.i {__name__}'
+    """  QYYYQLLYYYYYYYQLYYQYYQQQYQQYQQQQQQQQQQQQQQQQQQQQQQYYYQQQQQQYL
+        YYYYQYLLQYLLYYQYYYYYYYQQYQYQYQQQQQQQQQQQQQQQQQQQQQQQYYYQQQQQQ
+        QYYYYLPQYLPLYYYLLYYYYYYYYQQQYQQQQQQQQQQQQQQQQQQQQQQQYYYYQQQQQP
+        QYYQLPLQYLLYYQPLLLYYYYYYQYYQYQQQQQQQQQQQQQQYQQQQQQQQYYQYQQQQQQP
+       QYYQYLLYYYLLYQYLLYYYYYYYYQYYQYQYYYQQQQQQQQQQYQQQQQQYQQYQYYQQQQQYP
+      LQYQYYYYQYYYYYQYYYYYYYYYYYYYYYQQYYYYYYYYYQQQQYQQQQQQYQQYQYYQQQQQQ P
+      QYQQYYYYQYYYQQQYYYYYYYYQYQYYYYQQYYYQYQYYQQQQYQQQQQQQYQQYQYYQQQQQQ P
+      QYQQYYYYQYYYQQQYYYYYYYYQYQYYYYYQYYYYQYYYQQQQYQQQQQQQYQQYQQYQQQQYYP
+      QYQYYYYYQYYYQQQ PYLLLYP PLYYYYYYQYYYYYYQQQQYYQQQQQQYQQYQQQYQQQQYQ
+      PQQYYYYYQYYQQYQQQQQQQQQQYP        PPLYQYQYQYQLQQQQQYQQYQQQYYQQQYY
+       QQYYYYYQQYQLYQQPQQQQQL QYL           PPYYLYYLQYQQYYQYQQQQYYQPQYL
+       YQYYYYQQQYQ  LYLQQQQQQYQQ           YQQQQQGQQQQQQYQYYQQQQYQPQYQ P
+      L QYYYYQQLYQ   Y YPYQQQQQ           LQQQQQL YQQQQYQQYQYQQYYQQYQP P
+        YYQYYQQ  Q    LQQQQQQY            YQYQQQQQQYYQYLQYQQYQQYYQYQL P
+     Y  LYQLQQPL Y     P  P                QLLQQQQQ Q  PQQQQYQQYYQQL P
+    P   PYQYQQQQPQ                         PQQQQQQY    QQYQYYQQYYQPP
+    L    QQQYQ YYYY              PQ           L  P    LPQYQYYQQLQ P
+    Y   PPQQYYL LYQL                                 PQLQYQQYQYQ  L
+    Y     QQYQPP PYQY        PQ                      Q  QQYQYQYL  L
+    Y     QQYYQ L  QYQP         PLLLLLYL           LQQ LQYYQQQP P L
+     L   PPLQYYQ Y  LQQQ                         LQYQ  QYYYQQ     P
+      L    Q  QYQ  Y  QQPYL                   PQYYYYPPQYYQQQP    L
+       L    L  PQQL   LYQ  PQP             QL PYYYPLQLYQ  QY P   Y
+         P   P    PQQP  QY  QLLQQP   LYYLQ   PQYPQQQP P  QY P   L
+                       PYQYYY           PQ  PQ      L   Q P    L
+              PQYLYYYPQ PLPL             L QY YQYYQYLYQQQ    P
+            PYLLLLLYYYQ P  L    P         PYL  PQYYLLLLLLLQ
+           LYPLLLLLLYYYY   Y  YQY     LLLPPY   LYYYLLLLLLLLY
+           YLLLYLLLLLLYYQ  Q              PQ  YYYLLLLLLLLLLYP
+          YLLLLLLLLLLLLLLYQQ              PYYQYYLLLLLLLLYYYLQ
+          QLLLLLLLLLLLLLLLLLYYQYP        YQYYLLLLLLLLLLLLLLLQ
+          YLLLLLLLLLLLLLLLLLLLYYYLLYYYLLLLLLLLLLLLLLLLLLLLLLYP
+         PLLLLLLLLLLLLLLLLLLLLLLLYLLLLLLLLLLLLLLLLLLLLLLLYLYLL
+         LLLLLLLLLLYYLLLLLLYLLLLLLLLLLLLLLLL GQYLPY LLLYLYLLLY
+         QLLLLYYLYLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLQYYYYLLQ
+         QLLLLLYYQYLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLQLYYLLLQ
+        LYLLYLLLQYYLLLLLLLLLLLLLLLLLLLLLLLLLLLLLYLLLLLQYYYYYLYQ
+        YLLLYYLLYQYLLLLLLLLLLLLLLLLLLLLLLLLLLLLYLLLLLYYYYQLLLLY
+        QLLLYYYYYQLLLLLLLLLLLLLLYLLLLLLLLLLLLLLLLLLLLYYYLQLLPLLQ
+        YLYLLQYYYQLLLLLLLLLLLLLLLLLLLLLLLLLLLLYYLLLLLYYQYYLLLLLQ
+       LYLLLLLYYYQLLYLLLLLLLLLLLLYLYLLYYLLLLYLLLLLLLYYYQQLLLLLLLY
+       YLLLLLLYYYQLLYLLLLLLLYLYLLLLLLLLLLLLLLLLLLLLYYYYQQLYLLLLLQ
+       QLLLYLLLQYQLQLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLYYYQYYLLLLLLLY
+       QLLLLLLLLQQYQLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLQYYQYYLLLLLLLQ
+       QLLLLLLLLLQQYLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLYYYYLLLLLLLLLYL
+       QLLLLYLYYLYQLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLQYYYLLLLLLLLLQ
+       YLLLLLLLYYLQLLLLLLLLLLLLLLLLLLLLLLLLLYLLLLLLLLYQYYLLLLLLLLLQ
+       QLLLLLYLYYYYLLLLLPLLLLLLLYLYLLLLLLLLLLLLLLLLLLLQYYLLLLLLLLYP
+       YYLYYLLYYYQLLLLLLLLYLLLLLLLLLLLLLLLLLLLLLLYLYLLYQYYLLLLLLYL
+        QLLLLLLYQYLLLLLLLLLLLLLLLLLLLLLYYLYLLLLLLLLLLLYQQQQQQQLYL  """
+    gpath = f'{__name__}.gqylpy {__name__}'
     __import__(gpath)
 
     gpack = sys.modules[__name__]
-    gcode = globals()[f'i {__name__}']
+    gcode = globals()[f'gqylpy {__name__}']
 
     for gname in globals():
-        try:
-            assert gname[0] != '_'
-            gfunc = getattr(gcode, gname)
-            assert gfunc.__module__ == gpath
-        except (AssertionError, AttributeError):
-            continue
-        gfunc.__module__ = __package__
-        gfunc.__doc__ = getattr(gpack, gname).__doc__
-        setattr(gpack, gname, gfunc)
+        if gname[0] != '_':
+            try:
+                gfunc = getattr(gcode, gname)
+                if gfunc.__module__ is gpath:
+                    gfunc.__module__ = __package__
+                    gfunc.__doc__ = getattr(gpack, gname).__doc__
+                    setattr(gpack, gname, gfunc)
+            except AttributeError:
+                pass
```

## Comparing `systempath/i systempath.py` & `systempath/gqylpy systempath.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,19 +28,16 @@
     getcwd,  getcwdb
 )
 
 if sys.platform != 'win32':
     from os import mknod, chown, system, popen
 
     if sys.platform == 'linux':
-        try:
-            from os import getxattr, setxattr, listxattr, removexattr
-        except ImportError:
-            def getxattr(*a, **kw): raise NotImplementedError
-            setxattr = listxattr = removexattr = getxattr
+        from os import getxattr, setxattr, listxattr, removexattr
+
     try:
         from os import lchmod, lchown, chflags, lchflags
     except ImportError:
         def lchmod(*a, **kw): raise NotImplementedError
         lchown = chflags = lchflags = lchmod
     try:
         from pwd import getpwuid
@@ -646,25 +643,21 @@
             return self[name]
         except ge.SystemPathNotFoundError:
             raise AttributeError(
                 f"'{self.__class__.__name__}' object has no attribute '{name}'"
             ) from None
 
     @joinpath
-    def __getitem__(
-            self, name: PathLink
-    ) -> Union['SystemPath', 'Directory', 'File', Path]:
+    def __getitem__(self, name: PathLink) -> Union['Path', 'Directory', 'File']:
         if self.strict:
             if isdir(name):
                 return Directory(name, strict=self.strict)
             if isfile(name):
                 return File(name)
-            if exists(name):
-                return Path(name)
-            else:
+            if not exists(name):
                 raise ge.SystemPathNotFoundError(
                     f'system path {repr(name)} does not exist.'
                 )
         else:
             return SystemPath(name)
 
     @joinpath
@@ -686,15 +679,15 @@
         )
 
     @property
     def subpaths(self) -> Generator:
         return self.__iter__()
 
     @property
-    def subpath_names(self) -> List[BytesOrStr]:
+    def subpaths_names(self) -> List[BytesOrStr]:
         return listdir(self.name)
 
     def scandir(self) -> Iterator:
         return scandir(self.name)
 
     def tree(
             self,
@@ -1113,15 +1106,15 @@
 
     def read(self, size: int = -1, /) -> bytes:
         return self.rb().read(size)
 
     def overwrite(self, content: Union['Content', bytes], /) -> None:
         self.__ior__(content)
 
-    def append(self, content: Union['Content', bytes], /) -> None:
+    def append(self, content: Union['Content', bytes]) -> None:
         self.__iadd__(content)
 
     def copy(
             self,
             other:   Union['Content', FileIO],
             /, *,
             bufsize: int                      = READ_BUFFER_SIZE
@@ -1244,22 +1237,18 @@
 
 
 class SystemPath(Directory, File):
     __new__ = Directory.__new__
 
     def __init__(
             self,
-            root:            PathLink      = '.',
-            /, *,
-            autoabs:         bool          = False,
-            strict:          bool          = False,
-            dir_fd:          Optional[int] = None,
-            follow_symlinks: bool          = True
+            root:    PathLink = '.',
+            /,
+            autoabs: bool     = False,
+            strict:  bool     = False
     ):
         Path.__init__(
             self,
             '.' if root == '' else b'.' if root == b'' else root,
-            autoabs        =autoabs,
-            strict         =strict,
-            dir_fd         =dir_fd,
-            follow_symlinks=follow_symlinks
+            autoabs=autoabs,
+            strict=strict
         )
```

## Comparing `systempath-1.0.6.dist-info/LICENSE` & `systempath-1.0a8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `systempath-1.0.6.dist-info/METADATA` & `systempath-1.0a8.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: systempath
-Version: 1.0.6
+Version: 1.0a8
 Summary: Operating system paths and files.
 Home-page: http://gqylpy.com
 Author: 竹永康
 Author-email: <gqylpy@outlook.com>
 License: Apache 2.0
 Project-URL: Source, https://github.com/gqylpy/systempath
 Classifier: Environment :: Web Environment
```

