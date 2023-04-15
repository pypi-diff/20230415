# Comparing `tmp/cubao_pybind-0.0.1-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip` & `tmp/cubao_pybind-0.0.2-cp311-cp311-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,10 @@
-Zip file size: 72091 bytes, number of entries: 11
-drwxrwxrwx  2.0 unx        0 b- stor 23-Apr-15 16:31 cubao_pybind-0.0.1.dist-info/
-drwxrwxrwx  2.0 unx        0 b- stor 23-Apr-15 16:31 cubao_pybind/
-drwxrwxrwx  2.0 unx        0 b- stor 23-Apr-15 16:31 cubao_pybind.libs/
--rwxrwxrwx  2.0 unx   175896 b- defN 23-Apr-15 16:31 _cubao_pybind.cpython-310-x86_64-linux-gnu.so
--rw-rw-rw-  2.0 unx       13 b- defN 23-Apr-15 16:31 cubao_pybind-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     2182 b- defN 23-Apr-15 16:31 cubao_pybind-0.0.1.dist-info/LICENSE
--rw-rw-rw-  2.0 unx      948 b- defN 23-Apr-15 16:31 cubao_pybind-0.0.1.dist-info/METADATA
--rw-rw-r--  2.0 unx      683 b- defN 23-Apr-15 16:31 cubao_pybind-0.0.1.dist-info/RECORD
--rw-rw-rw-  2.0 unx      152 b- defN 23-Apr-15 16:31 cubao_pybind-0.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 unx      264 b- defN 23-Apr-15 16:31 cubao_pybind/__init__.py
--rw-rw-rw-  2.0 unx      190 b- defN 23-Apr-15 16:31 cubao_pybind/__main__.py
-11 files, 180328 bytes uncompressed, 70559 bytes compressed:  60.9%
+Zip file size: 54173 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat   107520 b- defN 23-Apr-15 16:42 _cubao_pybind.cp311-win_amd64.pyd
+-rw-rw-rw-  2.0 fat      274 b- defN 23-Apr-15 16:35 cubao_pybind/__init__.py
+-rw-rw-rw-  2.0 fat      197 b- defN 23-Apr-15 16:35 cubao_pybind/__main__.py
+-rw-rw-rw-  2.0 fat     2218 b- defN 23-Apr-15 16:42 cubao_pybind-0.0.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      995 b- defN 23-Apr-15 16:42 cubao_pybind-0.0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      102 b- defN 23-Apr-15 16:42 cubao_pybind-0.0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       13 b- defN 23-Apr-15 16:42 cubao_pybind-0.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      663 b- defN 23-Apr-15 16:42 cubao_pybind-0.0.2.dist-info/RECORD
+8 files, 111982 bytes uncompressed, 53013 bytes compressed:  52.7%
```

## zipnote {}

```diff
@@ -1,34 +1,25 @@
-Filename: cubao_pybind-0.0.1.dist-info/
+Filename: _cubao_pybind.cp311-win_amd64.pyd
 Comment: 
 
-Filename: cubao_pybind/
-Comment: 
-
-Filename: cubao_pybind.libs/
-Comment: 
-
-Filename: _cubao_pybind.cpython-310-x86_64-linux-gnu.so
-Comment: 
-
-Filename: cubao_pybind-0.0.1.dist-info/top_level.txt
+Filename: cubao_pybind/__init__.py
 Comment: 
 
-Filename: cubao_pybind-0.0.1.dist-info/LICENSE
+Filename: cubao_pybind/__main__.py
 Comment: 
 
-Filename: cubao_pybind-0.0.1.dist-info/METADATA
+Filename: cubao_pybind-0.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: cubao_pybind-0.0.1.dist-info/RECORD
+Filename: cubao_pybind-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: cubao_pybind-0.0.1.dist-info/WHEEL
+Filename: cubao_pybind-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: cubao_pybind/__init__.py
+Filename: cubao_pybind-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: cubao_pybind/__main__.py
+Filename: cubao_pybind-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=store
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## cubao_pybind/__init__.py

 * *Ordering differences only*

```diff
@@ -1,10 +1,10 @@
-from _cubao_pybind import *  # noqa: F403
-from _cubao_pybind import __version__  # noqa: F401
-
-
-def pure_python_func(
-    arg1: int = 42,
-    arg2: float = 3.14,
-    arg3: str = "you shall not pass",
-) -> str:
-    return f"int: {arg1}, float: {arg2}, str: {arg3}"
+from _cubao_pybind import *  # noqa: F403
+from _cubao_pybind import __version__  # noqa: F401
+
+
+def pure_python_func(
+    arg1: int = 42,
+    arg2: float = 3.14,
+    arg3: str = "you shall not pass",
+) -> str:
+    return f"int: {arg1}, float: {arg2}, str: {arg3}"
```

## cubao_pybind/__main__.py

 * *Ordering differences only*

```diff
@@ -1,7 +1,7 @@
-from cubao_pybind import *  # noqa: F403
-
-if __name__ == "__main__":
-    import fire
-
-    fire.core.Display = lambda lines, out: print(*lines, file=out)  # no pager for fire
-    fire.Fire()
+from cubao_pybind import *  # noqa: F403
+
+if __name__ == "__main__":
+    import fire
+
+    fire.core.Display = lambda lines, out: print(*lines, file=out)  # no pager for fire
+    fire.Fire()
```

## Comparing `cubao_pybind-0.0.1.dist-info/LICENSE` & `cubao_pybind-0.0.2.dist-info/LICENSE`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-Copyright (c) 2016 The Pybind Development Team, All rights reserved.
-
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are met:
-
-1. Redistributions of source code must retain the above copyright notice, this
-   list of conditions and the following disclaimer.
-
-2. Redistributions in binary form must reproduce the above copyright notice,
-   this list of conditions and the following disclaimer in the documentation
-   and/or other materials provided with the distribution.
-
-3. Neither the name of the copyright holder nor the names of its contributors
-   may be used to endorse or promote products derived from this software
-   without specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
-ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
-WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-
-You are under no obligation whatsoever to provide any bug fixes, patches, or
-upgrades to the features, functionality or performance of the source code
-("Enhancements") to anyone; however, if you choose to make your Enhancements
-available either publicly, or directly to the author of this software, without
-imposing a separate written license agreement for such Enhancements, then you
-hereby grant the following license: a non-exclusive, royalty-free perpetual
-license to install, use, modify, prepare derivative works, incorporate into
-other computer software, distribute, and sublicense such enhancements or
-derivative works thereof, in binary and source code form.
+Copyright (c) 2016 The Pybind Development Team, All rights reserved.
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
+
+1. Redistributions of source code must retain the above copyright notice, this
+   list of conditions and the following disclaimer.
+
+2. Redistributions in binary form must reproduce the above copyright notice,
+   this list of conditions and the following disclaimer in the documentation
+   and/or other materials provided with the distribution.
+
+3. Neither the name of the copyright holder nor the names of its contributors
+   may be used to endorse or promote products derived from this software
+   without specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
+ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
+WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+
+You are under no obligation whatsoever to provide any bug fixes, patches, or
+upgrades to the features, functionality or performance of the source code
+("Enhancements") to anyone; however, if you choose to make your Enhancements
+available either publicly, or directly to the author of this software, without
+imposing a separate written license agreement for such Enhancements, then you
+hereby grant the following license: a non-exclusive, royalty-free perpetual
+license to install, use, modify, prepare derivative works, incorporate into
+other computer software, distribute, and sublicense such enhancements or
+derivative works thereof, in binary and source code form.
```

## Comparing `cubao_pybind-0.0.1.dist-info/METADATA` & `cubao_pybind-0.0.2.dist-info/METADATA`

 * *Files 27% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-Metadata-Version: 2.1
-Name: cubao-pybind
-Version: 0.0.1
-Summary: misc c++ code in cubao
-Home-page: https://cubao-pybind.readthedocs.io
-Author: tzx
-Author-email: dvorak4tzx@gmail.com
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: fire
-Requires-Dist: loguru
-Requires-Dist: tqdm
-Provides-Extra: test
-Requires-Dist: pytest (>=6.0) ; extra == 'test'
-
-# cubao-pybind
-
-Online document: **[readthedocs](http://cubao-pybind.readthedocs.io/)**
-
-<!--intro-start-->
-
-## Usage
-
-Install:
-
-```bash
-python3 -m pip install cubao_pybind # install from pypi
-python3 -c 'import cubao_pybind; print(cubao_pybind.add(1, 2))'
-```
-
-CLI interface: (created with [python-fire](https://github.com/google/python-fire))
-
-```bash
-python3 -m cubao_pybind add 1 2
-python3 -m cubao_pybind subtract 9 4
-```
-
-Help:
-
-```bash
-$ python3 -m cubao_pybind --help
-
-$ python3 -m cubao_pybind pure_python_func --help
-```
-
-<!--intro-end-->
+Metadata-Version: 2.1
+Name: cubao-pybind
+Version: 0.0.2
+Summary: misc c++ code in cubao
+Home-page: https://cubao-pybind.readthedocs.io
+Author: tzx
+Author-email: dvorak4tzx@gmail.com
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: fire
+Requires-Dist: loguru
+Requires-Dist: tqdm
+Provides-Extra: test
+Requires-Dist: pytest (>=6.0) ; extra == 'test'
+
+# cubao-pybind
+
+Online document: **[readthedocs](http://cubao-pybind.readthedocs.io/)**
+
+<!--intro-start-->
+
+## Usage
+
+Install:
+
+```bash
+python3 -m pip install cubao_pybind # install from pypi
+python3 -c 'import cubao_pybind; print(cubao_pybind.add(1, 2))'
+```
+
+CLI interface: (created with [python-fire](https://github.com/google/python-fire))
+
+```bash
+python3 -m cubao_pybind add 1 2
+python3 -m cubao_pybind subtract 9 4
+```
+
+Help:
+
+```bash
+$ python3 -m cubao_pybind --help
+
+$ python3 -m cubao_pybind pure_python_func --help
+```
+
+<!--intro-end-->
```

