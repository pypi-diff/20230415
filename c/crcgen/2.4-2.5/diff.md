# Comparing `tmp/crcgen-2.4.tar.gz` & `tmp/crcgen-2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crcgen-2.4.tar", last modified: Sat Nov 26 19:37:11 2022, max compression
+gzip compressed data, was "crcgen-2.5.tar", last modified: Sat Apr 15 21:49:43 2023, max compression
```

## Comparing `crcgen-2.4.tar` & `crcgen-2.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-26 19:37:11.485718 crcgen-2.4/
--rw-r--r--   0 root         (0) root         (0)    18092 2022-11-26 19:37:10.000000 crcgen-2.4/COPYING
--rw-r--r--   0 root         (0) root         (0)       78 2022-11-26 19:37:10.000000 crcgen-2.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3895 2022-11-26 19:37:11.485718 crcgen-2.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3257 2022-11-26 19:37:10.000000 crcgen-2.4/README.html
--rw-r--r--   0 root         (0) root         (0)     2723 2022-11-26 19:37:10.000000 crcgen-2.4/README.rst
--rwxr-xr-x   0 root         (0) root         (0)      955 2022-11-26 19:37:10.000000 crcgen-2.4/crcgen
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-26 19:37:11.485718 crcgen-2.4/crcgen.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3895 2022-11-26 19:37:11.000000 crcgen-2.4/crcgen.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      392 2022-11-26 19:37:11.000000 crcgen-2.4/crcgen.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-26 19:37:11.000000 crcgen-2.4/crcgen.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       10 2022-11-26 19:37:11.000000 crcgen-2.4/crcgen.egg-info/top_level.txt
--rwxr-xr-x   0 root         (0) root         (0)    13365 2022-11-26 19:37:10.000000 crcgen-2.4/crcgen_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-26 19:37:11.485718 crcgen-2.4/libcrcgen/
--rw-r--r--   0 root         (0) root         (0)      119 2022-11-26 19:37:10.000000 crcgen-2.4/libcrcgen/__init__.py
--rw-r--r--   0 root         (0) root         (0)      932 2022-11-26 19:37:10.000000 crcgen-2.4/libcrcgen/__main__.py
--rw-r--r--   0 root         (0) root         (0)    15101 2022-11-26 19:37:10.000000 crcgen-2.4/libcrcgen/generator.py
--rw-r--r--   0 root         (0) root         (0)     3289 2022-11-26 19:37:10.000000 crcgen-2.4/libcrcgen/generator_test.py
--rw-r--r--   0 root         (0) root         (0)     7112 2022-11-26 19:37:10.000000 crcgen-2.4/libcrcgen/main.py
--rw-r--r--   0 root         (0) root         (0)     1613 2022-11-26 19:37:10.000000 crcgen-2.4/libcrcgen/parameters.py
--rw-r--r--   0 root         (0) root         (0)     2169 2022-11-26 19:37:10.000000 crcgen-2.4/libcrcgen/reference.py
--rw-r--r--   0 root         (0) root         (0)     2427 2022-11-26 19:37:10.000000 crcgen-2.4/libcrcgen/util.py
--rw-r--r--   0 root         (0) root         (0)     1060 2022-11-26 19:37:10.000000 crcgen-2.4/libcrcgen/version.py
--rw-r--r--   0 root         (0) root         (0)       38 2022-11-26 19:37:11.485718 crcgen-2.4/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     1550 2022-11-26 19:37:10.000000 crcgen-2.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 21:49:43.703232 crcgen-2.5/
+-rw-r--r--   0 root         (0) root         (0)    18092 2023-04-15 21:49:42.000000 crcgen-2.5/COPYING
+-rw-r--r--   0 root         (0) root         (0)       78 2023-04-15 21:49:42.000000 crcgen-2.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3918 2023-04-15 21:49:43.703232 crcgen-2.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3533 2023-04-15 21:49:43.000000 crcgen-2.5/README.html
+-rw-r--r--   0 root         (0) root         (0)     2723 2023-04-15 21:49:42.000000 crcgen-2.5/README.rst
+-rwxr-xr-x   0 root         (0) root         (0)      955 2023-04-15 21:49:42.000000 crcgen-2.5/crcgen
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 21:49:43.703232 crcgen-2.5/crcgen.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3918 2023-04-15 21:49:43.000000 crcgen-2.5/crcgen.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      392 2023-04-15 21:49:43.000000 crcgen-2.5/crcgen.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-15 21:49:43.000000 crcgen-2.5/crcgen.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-04-15 21:49:43.000000 crcgen-2.5/crcgen.egg-info/top_level.txt
+-rwxr-xr-x   0 root         (0) root         (0)    13365 2023-04-15 21:49:42.000000 crcgen-2.5/crcgen_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 21:49:43.703232 crcgen-2.5/libcrcgen/
+-rw-r--r--   0 root         (0) root         (0)      119 2023-04-15 21:49:42.000000 crcgen-2.5/libcrcgen/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      932 2023-04-15 21:49:42.000000 crcgen-2.5/libcrcgen/__main__.py
+-rw-r--r--   0 root         (0) root         (0)    15433 2023-04-15 21:49:42.000000 crcgen-2.5/libcrcgen/generator.py
+-rw-r--r--   0 root         (0) root         (0)     3289 2023-04-15 21:49:42.000000 crcgen-2.5/libcrcgen/generator_test.py
+-rw-r--r--   0 root         (0) root         (0)     7753 2023-04-15 21:49:42.000000 crcgen-2.5/libcrcgen/main.py
+-rw-r--r--   0 root         (0) root         (0)     1613 2023-04-15 21:49:42.000000 crcgen-2.5/libcrcgen/parameters.py
+-rw-r--r--   0 root         (0) root         (0)     2161 2023-04-15 21:49:42.000000 crcgen-2.5/libcrcgen/reference.py
+-rw-r--r--   0 root         (0) root         (0)     2427 2023-04-15 21:49:42.000000 crcgen-2.5/libcrcgen/util.py
+-rw-r--r--   0 root         (0) root         (0)     1060 2023-04-15 21:49:42.000000 crcgen-2.5/libcrcgen/version.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-15 21:49:43.703232 crcgen-2.5/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     1513 2023-04-15 21:49:42.000000 crcgen-2.5/setup.py
```

### Comparing `crcgen-2.4/COPYING` & `crcgen-2.5/COPYING`

 * *Files identical despite different names*

### Comparing `crcgen-2.4/PKG-INFO` & `crcgen-2.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: crcgen
-Version: 2.4
+Version: 2.5
 Summary: CRC algorithm HDL code generator (VHDL, Verilog, MyHDL)
 Home-page: https://bues.ch/h/crcgen
-Author: Michael Buesch
+Author: Michael Büsch
 Author-email: m@bues.ch
 License: GNU General Public License v2 or later
 Keywords: CRC Verilog VHDL MyHDL FPGA codegenerator
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
@@ -20,14 +20,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Education
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Utilities
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: COPYING
 
 CRC algorithm HDL code generator (VHDL, Verilog, MyHDL)
 =======================================================
 
 `Homepage <https://bues.ch/h/crcgen>`_
@@ -98,14 +99,14 @@
 NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF OR IN CONNECTION WITH THE
 USE OR PERFORMANCE OF THIS SOFTWARE.
 
 
 License of the generator
 ========================
 
-Copyright (c) 2019-2022 Michael Büsch <m@bues.ch>
+Copyright (c) 2019-2023 Michael Büsch <m@bues.ch>
 
 This program is free software; you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation; either version 2 of the License, or (at your option) any later version.
 
 This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License along with this program; if not, write to the Free Software Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
```

### Comparing `crcgen-2.4/README.html` & `crcgen-2.5/README.rst`

 * *Files 21% similar despite different names*

```diff
@@ -1,204 +1,171 @@
-00000000: 3c73 6563 7469 6f6e 2069 643d 2263 7263  <section id="crc
-00000010: 2d61 6c67 6f72 6974 686d 2d68 646c 2d63  -algorithm-hdl-c
-00000020: 6f64 652d 6765 6e65 7261 746f 722d 7668  ode-generator-vh
-00000030: 646c 2d76 6572 696c 6f67 2d6d 7968 646c  dl-verilog-myhdl
-00000040: 223e 0a3c 6832 3e43 5243 2061 6c67 6f72  ">.<h2>CRC algor
-00000050: 6974 686d 2048 444c 2063 6f64 6520 6765  ithm HDL code ge
-00000060: 6e65 7261 746f 7220 2856 4844 4c2c 2056  nerator (VHDL, V
-00000070: 6572 696c 6f67 2c20 4d79 4844 4c29 3c2f  erilog, MyHDL)</
-00000080: 6832 3e0a 3c70 3e3c 6120 6872 6566 3d22  h2>.<p><a href="
-00000090: 6874 7470 733a 2f2f 6275 6573 2e63 682f  https://bues.ch/
-000000a0: 682f 6372 6367 656e 2220 7265 6c3d 226e  h/crcgen" rel="n
-000000b0: 6f66 6f6c 6c6f 7722 3e48 6f6d 6570 6167  ofollow">Homepag
-000000c0: 653c 2f61 3e3c 2f70 3e0a 3c70 3e3c 6120  e</a></p>.<p><a 
-000000d0: 6872 6566 3d22 6874 7470 733a 2f2f 6275  href="https://bu
-000000e0: 6573 2e63 682f 6367 6974 2f63 7263 6765  es.ch/cgit/crcge
-000000f0: 6e2e 6769 7422 2072 656c 3d22 6e6f 666f  n.git" rel="nofo
-00000100: 6c6c 6f77 223e 4769 7420 7265 706f 7369  llow">Git reposi
-00000110: 746f 7279 3c2f 613e 3c2f 703e 0a3c 703e  tory</a></p>.<p>
-00000120: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-00000130: 2f67 6974 6875 622e 636f 6d2f 6d62 7565  /github.com/mbue
-00000140: 7363 682f 6372 6367 656e 2220 7265 6c3d  sch/crcgen" rel=
-00000150: 226e 6f66 6f6c 6c6f 7722 3e47 6974 6875  "nofollow">Githu
-00000160: 6220 7265 706f 7369 746f 7279 3c2f 613e  b repository</a>
-00000170: 3c2f 703e 0a3c 703e 5468 6973 2074 6f6f  </p>.<p>This too
-00000180: 6c20 6765 6e65 7261 7465 7320 5648 444c  l generates VHDL
-00000190: 2c20 5665 7269 6c6f 6720 6f72 204d 7948  , Verilog or MyH
-000001a0: 444c 2063 6f64 6520 666f 7220 7573 6520  DL code for use 
-000001b0: 696e 2046 5047 4173 2074 6f20 6361 6c63  in FPGAs to calc
-000001c0: 756c 6174 6520 4352 4320 2843 7963 6c69  ulate CRC (Cycli
-000001d0: 6320 5265 6475 6e64 616e 6379 2043 6865  c Redundancy Che
-000001e0: 636b 2920 6368 6563 6b73 756d 732e 3c2f  ck) checksums.</
-000001f0: 703e 0a3c 703e 5468 6520 6765 6e65 7261  p>.<p>The genera
-00000200: 7465 6420 4844 4c20 636f 6465 2069 7320  ted HDL code is 
-00000210: 7379 6e74 6865 7369 7a61 626c 6520 616e  synthesizable an
-00000220: 6420 636f 6d62 696e 6174 6f72 6961 6c2e  d combinatorial.
-00000230: 2054 6861 7420 6d65 616e 7320 7468 6520   That means the 
-00000240: 6361 6c63 756c 6174 696f 6e20 7275 6e73  calculation runs
-00000250: 2069 6e20 6f6e 6520 636c 6f63 6b20 6379   in one clock cy
-00000260: 636c 6520 6f6e 2061 6e20 4650 4741 2e3c  cle on an FPGA.<
-00000270: 2f70 3e0a 3c70 3e41 6e79 2063 6f6d 6269  /p>.<p>Any combi
-00000280: 6e61 7469 6f6e 206f 6620 4352 4320 616c  nation of CRC al
-00000290: 676f 7269 7468 6d20 7061 7261 6d65 7465  gorithm paramete
-000002a0: 7273 2061 6e64 2070 6f6c 796e 6f6d 6961  rs and polynomia
-000002b0: 6c20 636f 6566 6669 6369 656e 7473 2063  l coefficients c
-000002c0: 616e 2062 6520 7365 6c65 6374 6564 2e3c  an be selected.<
-000002d0: 2f70 3e0a 3c2f 7365 6374 696f 6e3e 0a3c  /p>.</section>.<
-000002e0: 7365 6374 696f 6e20 6964 3d22 6578 616d  section id="exam
-000002f0: 706c 652d 7573 6167 6522 3e0a 3c68 323e  ple-usage">.<h2>
-00000300: 4578 616d 706c 6520 7573 6167 653c 2f68  Example usage</h
-00000310: 323e 0a3c 703e 4469 7370 6c61 7920 616c  2>.<p>Display al
-00000320: 6c20 6f70 7469 6f6e 733a 3c2f 703e 0a3c  l options:</p>.<
-00000330: 7072 653e 3c63 6f64 653e 6372 6367 656e  pre><code>crcgen
-00000340: 202d 683c 2f63 6f64 653e 3c2f 7072 653e   -h</code></pre>
-00000350: 0a3c 703e 4765 6e65 7261 7465 2056 6572  .<p>Generate Ver
-00000360: 696c 6f67 2063 6f64 6520 666f 7220 4352  ilog code for CR
-00000370: 432d 3332 3a3c 2f70 3e0a 3c70 7265 3e3c  C-32:</p>.<pre><
-00000380: 636f 6465 3e63 7263 6765 6e20 2d61 2043  code>crcgen -a C
-00000390: 5243 2d33 3220 2d76 3c2f 636f 6465 3e3c  RC-32 -v</code><
-000003a0: 2f70 7265 3e0a 3c70 3e47 656e 6572 6174  /pre>.<p>Generat
-000003b0: 6520 5648 444c 2063 6f64 6520 666f 7220  e VHDL code for 
-000003c0: 4352 432d 3332 3a3c 2f70 3e0a 3c70 7265  CRC-32:</p>.<pre
-000003d0: 3e3c 636f 6465 3e63 7263 6765 6e20 2d61  ><code>crcgen -a
-000003e0: 2043 5243 2d33 3220 2d56 3c2f 636f 6465   CRC-32 -V</code
-000003f0: 3e3c 2f70 7265 3e0a 3c70 3e47 656e 6572  ></pre>.<p>Gener
-00000400: 6174 6520 5665 7269 6c6f 6720 636f 6465  ate Verilog code
-00000410: 2066 6f72 2061 2063 7573 746f 6d20 6e6f   for a custom no
-00000420: 6e2d 7374 616e 6461 7264 2043 5243 206f  n-standard CRC o
-00000430: 7220 616e 7920 7374 616e 6461 7264 2061  r any standard a
-00000440: 6c67 6f72 6974 686d 2074 6861 74e2 8099  lgorithm that...
-00000450: 7320 6e6f 7420 696e 636c 7564 6564 2069  s not included i
-00000460: 6e20 6372 6367 656e e280 9973 202d 6120  n crcgen...s -a 
-00000470: 6c69 7374 3a3c 2f70 3e0a 3c70 7265 3e3c  list:</p>.<pre><
-00000480: 636f 6465 3e63 7263 6765 6e20 2d50 203c  code>crcgen -P <
-00000490: 7370 616e 2063 6c61 7373 3d22 7332 223e  span class="s2">
-000004a0: 2671 756f 743b 785e 3820 2b20 785e 3720  &quot;x^8 + x^7 
-000004b0: 2b20 785e 3520 2b20 785e 3420 2b20 785e  + x^5 + x^4 + x^
-000004c0: 3220 2b20 7820 2b20 3126 7175 6f74 3b3c  2 + x + 1&quot;<
-000004d0: 2f73 7061 6e3e 202d 4231 3620 2d52 202d  /span> -B16 -R -
-000004e0: 763c 2f63 6f64 653e 3c2f 7072 653e 0a3c  v</code></pre>.<
-000004f0: 2f73 6563 7469 6f6e 3e0a 3c73 6563 7469  /section>.<secti
-00000500: 6f6e 2069 643d 226f 6e6c 696e 652d 6372  on id="online-cr
-00000510: 6367 656e 223e 0a3c 6832 3e4f 6e6c 696e  cgen">.<h2>Onlin
-00000520: 6520 6372 6367 656e 3c2f 6832 3e0a 3c70  e crcgen</h2>.<p
-00000530: 3e41 6e20 6561 7379 2074 6f20 7573 6520  >An easy to use 
-00000540: 6f6e 6c69 6e65 2076 6572 7369 6f6e 206f  online version o
-00000550: 6620 6372 6367 656e 2074 6861 7420 6361  f crcgen that ca
-00000560: 6e20 6265 2075 7365 6420 7769 7468 6f75  n be used withou
-00000570: 7420 696e 7374 616c 6c69 6e67 206f 7220  t installing or 
-00000580: 646f 776e 6c6f 6164 696e 6720 616e 7974  downloading anyt
-00000590: 6869 6e67 2074 6f20 796f 7572 206d 6163  hing to your mac
-000005a0: 6869 6e65 2069 7320 6176 6169 6c61 626c  hine is availabl
-000005b0: 6520 6865 7265 3a3c 2f70 3e0a 3c70 3e3c  e here:</p>.<p><
-000005c0: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
-000005d0: 6275 6573 2e63 682f 682f 6372 6367 656e  bues.ch/h/crcgen
-000005e0: 2220 7265 6c3d 226e 6f66 6f6c 6c6f 7722  " rel="nofollow"
-000005f0: 3e4f 6e6c 696e 6520 6372 6367 656e 3c2f  >Online crcgen</
-00000600: 613e 3c2f 703e 0a3c 2f73 6563 7469 6f6e  a></p>.</section
-00000610: 3e0a 3c73 6563 7469 6f6e 2069 643d 226c  >.<section id="l
-00000620: 6963 656e 7365 2d6f 662d 7468 652d 6765  icense-of-the-ge
-00000630: 6e65 7261 7465 642d 6864 6c2d 636f 6465  nerated-hdl-code
-00000640: 223e 0a3c 6832 3e4c 6963 656e 7365 206f  ">.<h2>License o
-00000650: 6620 7468 6520 6765 6e65 7261 7465 6420  f the generated 
-00000660: 4844 4c20 636f 6465 3c2f 6832 3e0a 3c70  HDL code</h2>.<p
-00000670: 3e54 6865 2067 656e 6572 6174 6564 2063  >The generated c
-00000680: 6f64 6520 6973 2050 7562 6c69 6320 446f  ode is Public Do
-00000690: 6d61 696e 2e3c 2f70 3e0a 3c70 3e50 6572  main.</p>.<p>Per
-000006a0: 6d69 7373 696f 6e20 746f 2075 7365 2c20  mission to use, 
-000006b0: 636f 7079 2c20 6d6f 6469 6679 2c20 616e  copy, modify, an
-000006c0: 642f 6f72 2064 6973 7472 6962 7574 6520  d/or distribute 
-000006d0: 7468 6973 2073 6f66 7477 6172 6520 666f  this software fo
-000006e0: 7220 616e 790a 7075 7270 6f73 6520 7769  r any.purpose wi
-000006f0: 7468 206f 7220 7769 7468 6f75 7420 6665  th or without fe
-00000700: 6520 6973 2068 6572 6562 7920 6772 616e  e is hereby gran
-00000710: 7465 642e 3c2f 703e 0a3c 703e 5448 4520  ted.</p>.<p>THE 
-00000720: 534f 4654 5741 5245 2049 5320 5052 4f56  SOFTWARE IS PROV
-00000730: 4944 4544 20e2 809c 4153 2049 53e2 809d  IDED ...AS IS...
-00000740: 2041 4e44 2054 4845 2041 5554 484f 5220   AND THE AUTHOR 
-00000750: 4449 5343 4c41 494d 5320 414c 4c20 5741  DISCLAIMS ALL WA
-00000760: 5252 414e 5449 4553 0a57 4954 4820 5245  RRANTIES.WITH RE
-00000770: 4741 5244 2054 4f20 5448 4953 2053 4f46  GARD TO THIS SOF
-00000780: 5457 4152 4520 494e 434c 5544 494e 4720  TWARE INCLUDING 
-00000790: 414c 4c20 494d 504c 4945 4420 5741 5252  ALL IMPLIED WARR
-000007a0: 414e 5449 4553 204f 460a 4d45 5243 4841  ANTIES OF.MERCHA
-000007b0: 4e54 4142 494c 4954 5920 414e 4420 4649  NTABILITY AND FI
-000007c0: 544e 4553 532e 2049 4e20 4e4f 2045 5645  TNESS. IN NO EVE
-000007d0: 4e54 2053 4841 4c4c 2054 4845 2041 5554  NT SHALL THE AUT
-000007e0: 484f 5220 4245 204c 4941 424c 4520 464f  HOR BE LIABLE FO
-000007f0: 5220 414e 590a 5350 4543 4941 4c2c 2044  R ANY.SPECIAL, D
-00000800: 4952 4543 542c 2049 4e44 4952 4543 542c  IRECT, INDIRECT,
-00000810: 204f 5220 434f 4e53 4551 5545 4e54 4941   OR CONSEQUENTIA
-00000820: 4c20 4441 4d41 4745 5320 4f52 2041 4e59  L DAMAGES OR ANY
-00000830: 2044 414d 4147 4553 2057 4841 5453 4f45   DAMAGES WHATSOE
-00000840: 5645 520a 5245 5355 4c54 494e 4720 4652  VER.RESULTING FR
-00000850: 4f4d 204c 4f53 5320 4f46 2055 5345 2c20  OM LOSS OF USE, 
-00000860: 4441 5441 204f 5220 5052 4f46 4954 532c  DATA OR PROFITS,
-00000870: 2057 4845 5448 4552 2049 4e20 414e 2041   WHETHER IN AN A
-00000880: 4354 494f 4e20 4f46 2043 4f4e 5452 4143  CTION OF CONTRAC
-00000890: 542c 0a4e 4547 4c49 4745 4e43 4520 4f52  T,.NEGLIGENCE OR
-000008a0: 204f 5448 4552 2054 4f52 5449 4f55 5320   OTHER TORTIOUS 
-000008b0: 4143 5449 4f4e 2c20 4152 4953 494e 4720  ACTION, ARISING 
-000008c0: 4f55 5420 4f46 204f 5220 494e 2043 4f4e  OUT OF OR IN CON
-000008d0: 4e45 4354 494f 4e20 5749 5448 2054 4845  NECTION WITH THE
-000008e0: 0a55 5345 204f 5220 5045 5246 4f52 4d41  .USE OR PERFORMA
-000008f0: 4e43 4520 4f46 2054 4849 5320 534f 4654  NCE OF THIS SOFT
-00000900: 5741 5245 2e3c 2f70 3e0a 3c2f 7365 6374  WARE.</p>.</sect
-00000910: 696f 6e3e 0a3c 7365 6374 696f 6e20 6964  ion>.<section id
-00000920: 3d22 6c69 6365 6e73 652d 6f66 2d74 6865  ="license-of-the
-00000930: 2d67 656e 6572 6174 6f72 223e 0a3c 6832  -generator">.<h2
-00000940: 3e4c 6963 656e 7365 206f 6620 7468 6520  >License of the 
-00000950: 6765 6e65 7261 746f 723c 2f68 323e 0a3c  generator</h2>.<
-00000960: 703e 436f 7079 7269 6768 7420 2863 2920  p>Copyright (c) 
-00000970: 3230 3139 2d32 3032 3220 4d69 6368 6165  2019-2022 Michae
-00000980: 6c20 42c3 bc73 6368 2026 6c74 3b3c 6120  l B..sch &lt;<a 
-00000990: 6872 6566 3d22 6d61 696c 746f 3a6d 2623  href="mailto:m&#
-000009a0: 3337 3b26 2335 323b 2623 3438 3b62 7565  37;&#52;&#48;bue
-000009b0: 7326 2334 363b 6368 223e 6d3c 7370 616e  s&#46;ch">m<span
-000009c0: 3e26 2336 343b 3c2f 7370 616e 3e62 7565  >&#64;</span>bue
-000009d0: 733c 7370 616e 3e26 2334 363b 3c2f 7370  s<span>&#46;</sp
-000009e0: 616e 3e63 683c 2f61 3e26 6774 3b3c 2f70  an>ch</a>&gt;</p
-000009f0: 3e0a 3c70 3e54 6869 7320 7072 6f67 7261  >.<p>This progra
-00000a00: 6d20 6973 2066 7265 6520 736f 6674 7761  m is free softwa
-00000a10: 7265 3b20 796f 7520 6361 6e20 7265 6469  re; you can redi
-00000a20: 7374 7269 6275 7465 2069 7420 616e 642f  stribute it and/
-00000a30: 6f72 206d 6f64 6966 7920 6974 2075 6e64  or modify it und
-00000a40: 6572 2074 6865 2074 6572 6d73 206f 6620  er the terms of 
-00000a50: 7468 6520 474e 5520 4765 6e65 7261 6c20  the GNU General 
-00000a60: 5075 626c 6963 204c 6963 656e 7365 2061  Public License a
-00000a70: 7320 7075 626c 6973 6865 6420 6279 2074  s published by t
-00000a80: 6865 2046 7265 6520 536f 6674 7761 7265  he Free Software
-00000a90: 2046 6f75 6e64 6174 696f 6e3b 2065 6974   Foundation; eit
-00000aa0: 6865 7220 7665 7273 696f 6e20 3220 6f66  her version 2 of
-00000ab0: 2074 6865 204c 6963 656e 7365 2c20 6f72   the License, or
-00000ac0: 2028 6174 2079 6f75 7220 6f70 7469 6f6e   (at your option
-00000ad0: 2920 616e 7920 6c61 7465 7220 7665 7273  ) any later vers
-00000ae0: 696f 6e2e 3c2f 703e 0a3c 703e 5468 6973  ion.</p>.<p>This
-00000af0: 2070 726f 6772 616d 2069 7320 6469 7374   program is dist
-00000b00: 7269 6275 7465 6420 696e 2074 6865 2068  ributed in the h
-00000b10: 6f70 6520 7468 6174 2069 7420 7769 6c6c  ope that it will
-00000b20: 2062 6520 7573 6566 756c 2c20 6275 7420   be useful, but 
-00000b30: 5749 5448 4f55 5420 414e 5920 5741 5252  WITHOUT ANY WARR
-00000b40: 414e 5459 3b20 7769 7468 6f75 7420 6576  ANTY; without ev
-00000b50: 656e 2074 6865 2069 6d70 6c69 6564 2077  en the implied w
-00000b60: 6172 7261 6e74 7920 6f66 204d 4552 4348  arranty of MERCH
-00000b70: 414e 5441 4249 4c49 5459 206f 7220 4649  ANTABILITY or FI
-00000b80: 544e 4553 5320 464f 5220 4120 5041 5254  TNESS FOR A PART
-00000b90: 4943 554c 4152 2050 5552 504f 5345 2e20  ICULAR PURPOSE. 
-00000ba0: 2053 6565 2074 6865 2047 4e55 2047 656e   See the GNU Gen
-00000bb0: 6572 616c 2050 7562 6c69 6320 4c69 6365  eral Public Lice
-00000bc0: 6e73 6520 666f 7220 6d6f 7265 2064 6574  nse for more det
-00000bd0: 6169 6c73 2e3c 2f70 3e0a 3c70 3e59 6f75  ails.</p>.<p>You
-00000be0: 2073 686f 756c 6420 6861 7665 2072 6563   should have rec
-00000bf0: 6569 7665 6420 6120 636f 7079 206f 6620  eived a copy of 
-00000c00: 7468 6520 474e 5520 4765 6e65 7261 6c20  the GNU General 
-00000c10: 5075 626c 6963 204c 6963 656e 7365 2061  Public License a
-00000c20: 6c6f 6e67 2077 6974 6820 7468 6973 2070  long with this p
-00000c30: 726f 6772 616d 3b20 6966 206e 6f74 2c20  rogram; if not, 
-00000c40: 7772 6974 6520 746f 2074 6865 2046 7265  write to the Fre
-00000c50: 6520 536f 6674 7761 7265 2046 6f75 6e64  e Software Found
-00000c60: 6174 696f 6e2c 2049 6e63 2e2c 2035 3120  ation, Inc., 51 
-00000c70: 4672 616e 6b6c 696e 2053 7472 6565 742c  Franklin Street,
-00000c80: 2046 6966 7468 2046 6c6f 6f72 2c20 426f   Fifth Floor, Bo
-00000c90: 7374 6f6e 2c20 4d41 2030 3231 3130 2d31  ston, MA 02110-1
-00000ca0: 3330 3120 5553 412e 3c2f 703e 0a3c 2f73  301 USA.</p>.</s
-00000cb0: 6563 7469 6f6e 3e0a 0a                   ection>..
+00000000: 4352 4320 616c 676f 7269 7468 6d20 4844  CRC algorithm HD
+00000010: 4c20 636f 6465 2067 656e 6572 6174 6f72  L code generator
+00000020: 2028 5648 444c 2c20 5665 7269 6c6f 672c   (VHDL, Verilog,
+00000030: 204d 7948 444c 290a 3d3d 3d3d 3d3d 3d3d   MyHDL).========
+00000040: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00000050: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00000060: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a  ===============.
+00000070: 0a60 486f 6d65 7061 6765 203c 6874 7470  .`Homepage <http
+00000080: 733a 2f2f 6275 6573 2e63 682f 682f 6372  s://bues.ch/h/cr
+00000090: 6367 656e 3e60 5f0a 0a60 4769 7420 7265  cgen>`_..`Git re
+000000a0: 706f 7369 746f 7279 203c 6874 7470 733a  pository <https:
+000000b0: 2f2f 6275 6573 2e63 682f 6367 6974 2f63  //bues.ch/cgit/c
+000000c0: 7263 6765 6e2e 6769 743e 605f 0a0a 6047  rcgen.git>`_..`G
+000000d0: 6974 6875 6220 7265 706f 7369 746f 7279  ithub repository
+000000e0: 203c 6874 7470 733a 2f2f 6769 7468 7562   <https://github
+000000f0: 2e63 6f6d 2f6d 6275 6573 6368 2f63 7263  .com/mbuesch/crc
+00000100: 6765 6e3e 605f 0a0a 5468 6973 2074 6f6f  gen>`_..This too
+00000110: 6c20 6765 6e65 7261 7465 7320 5648 444c  l generates VHDL
+00000120: 2c20 5665 7269 6c6f 6720 6f72 204d 7948  , Verilog or MyH
+00000130: 444c 2063 6f64 6520 666f 7220 7573 6520  DL code for use 
+00000140: 696e 2046 5047 4173 2074 6f20 6361 6c63  in FPGAs to calc
+00000150: 756c 6174 6520 4352 4320 2843 7963 6c69  ulate CRC (Cycli
+00000160: 6320 5265 6475 6e64 616e 6379 2043 6865  c Redundancy Che
+00000170: 636b 2920 6368 6563 6b73 756d 732e 0a0a  ck) checksums...
+00000180: 5468 6520 6765 6e65 7261 7465 6420 4844  The generated HD
+00000190: 4c20 636f 6465 2069 7320 7379 6e74 6865  L code is synthe
+000001a0: 7369 7a61 626c 6520 616e 6420 636f 6d62  sizable and comb
+000001b0: 696e 6174 6f72 6961 6c2e 2054 6861 7420  inatorial. That 
+000001c0: 6d65 616e 7320 7468 6520 6361 6c63 756c  means the calcul
+000001d0: 6174 696f 6e20 7275 6e73 2069 6e20 6f6e  ation runs in on
+000001e0: 6520 636c 6f63 6b20 6379 636c 6520 6f6e  e clock cycle on
+000001f0: 2061 6e20 4650 4741 2e0a 0a41 6e79 2063   an FPGA...Any c
+00000200: 6f6d 6269 6e61 7469 6f6e 206f 6620 4352  ombination of CR
+00000210: 4320 616c 676f 7269 7468 6d20 7061 7261  C algorithm para
+00000220: 6d65 7465 7273 2061 6e64 2070 6f6c 796e  meters and polyn
+00000230: 6f6d 6961 6c20 636f 6566 6669 6369 656e  omial coefficien
+00000240: 7473 2063 616e 2062 6520 7365 6c65 6374  ts can be select
+00000250: 6564 2e0a 0a0a 4578 616d 706c 6520 7573  ed....Example us
+00000260: 6167 650a 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  age.============
+00000270: 3d0a 0a44 6973 706c 6179 2061 6c6c 206f  =..Display all o
+00000280: 7074 696f 6e73 3a0a 0a2e 2e20 636f 6465  ptions:.... code
+00000290: 3a3a 2073 680a 0a09 6372 6367 656e 202d  :: sh...crcgen -
+000002a0: 680a 0a0a 4765 6e65 7261 7465 2056 6572  h...Generate Ver
+000002b0: 696c 6f67 2063 6f64 6520 666f 7220 4352  ilog code for CR
+000002c0: 432d 3332 3a0a 0a2e 2e20 636f 6465 3a3a  C-32:.... code::
+000002d0: 2073 680a 0a09 6372 6367 656e 202d 6120   sh...crcgen -a 
+000002e0: 4352 432d 3332 202d 760a 0a0a 4765 6e65  CRC-32 -v...Gene
+000002f0: 7261 7465 2056 4844 4c20 636f 6465 2066  rate VHDL code f
+00000300: 6f72 2043 5243 2d33 323a 0a0a 2e2e 2063  or CRC-32:.... c
+00000310: 6f64 653a 3a20 7368 0a0a 0963 7263 6765  ode:: sh...crcge
+00000320: 6e20 2d61 2043 5243 2d33 3220 2d56 0a0a  n -a CRC-32 -V..
+00000330: 0a47 656e 6572 6174 6520 5665 7269 6c6f  .Generate Verilo
+00000340: 6720 636f 6465 2066 6f72 2061 2063 7573  g code for a cus
+00000350: 746f 6d20 6e6f 6e2d 7374 616e 6461 7264  tom non-standard
+00000360: 2043 5243 206f 7220 616e 7920 7374 616e   CRC or any stan
+00000370: 6461 7264 2061 6c67 6f72 6974 686d 2074  dard algorithm t
+00000380: 6861 7427 7320 6e6f 7420 696e 636c 7564  hat's not includ
+00000390: 6564 2069 6e20 6372 6367 656e 2773 202d  ed in crcgen's -
+000003a0: 6120 6c69 7374 3a0a 0a2e 2e20 636f 6465  a list:.... code
+000003b0: 3a3a 2073 680a 0a09 6372 6367 656e 202d  :: sh...crcgen -
+000003c0: 5020 2278 5e38 202b 2078 5e37 202b 2078  P "x^8 + x^7 + x
+000003d0: 5e35 202b 2078 5e34 202b 2078 5e32 202b  ^5 + x^4 + x^2 +
+000003e0: 2078 202b 2031 2220 2d42 3136 202d 5220   x + 1" -B16 -R 
+000003f0: 2d76 0a0a 0a4f 6e6c 696e 6520 6372 6367  -v...Online crcg
+00000400: 656e 0a3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  en.=============
+00000410: 0a0a 416e 2065 6173 7920 746f 2075 7365  ..An easy to use
+00000420: 206f 6e6c 696e 6520 7665 7273 696f 6e20   online version 
+00000430: 6f66 2063 7263 6765 6e20 7468 6174 2063  of crcgen that c
+00000440: 616e 2062 6520 7573 6564 2077 6974 686f  an be used witho
+00000450: 7574 2069 6e73 7461 6c6c 696e 6720 6f72  ut installing or
+00000460: 2064 6f77 6e6c 6f61 6469 6e67 2061 6e79   downloading any
+00000470: 7468 696e 6720 746f 2079 6f75 7220 6d61  thing to your ma
+00000480: 6368 696e 6520 6973 2061 7661 696c 6162  chine is availab
+00000490: 6c65 2068 6572 653a 0a0a 604f 6e6c 696e  le here:..`Onlin
+000004a0: 6520 6372 6367 656e 203c 6874 7470 733a  e crcgen <https:
+000004b0: 2f2f 6275 6573 2e63 682f 682f 6372 6367  //bues.ch/h/crcg
+000004c0: 656e 3e60 5f0a 0a0a 4c69 6365 6e73 6520  en>`_...License 
+000004d0: 6f66 2074 6865 2067 656e 6572 6174 6564  of the generated
+000004e0: 2048 444c 2063 6f64 650a 3d3d 3d3d 3d3d   HDL code.======
+000004f0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00000500: 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a 0a54 6865  ===========..The
+00000510: 2067 656e 6572 6174 6564 2063 6f64 6520   generated code 
+00000520: 6973 2050 7562 6c69 6320 446f 6d61 696e  is Public Domain
+00000530: 2e0a 0a50 6572 6d69 7373 696f 6e20 746f  ...Permission to
+00000540: 2075 7365 2c20 636f 7079 2c20 6d6f 6469   use, copy, modi
+00000550: 6679 2c20 616e 642f 6f72 2064 6973 7472  fy, and/or distr
+00000560: 6962 7574 6520 7468 6973 2073 6f66 7477  ibute this softw
+00000570: 6172 6520 666f 7220 616e 790a 7075 7270  are for any.purp
+00000580: 6f73 6520 7769 7468 206f 7220 7769 7468  ose with or with
+00000590: 6f75 7420 6665 6520 6973 2068 6572 6562  out fee is hereb
+000005a0: 7920 6772 616e 7465 642e 0a0a 5448 4520  y granted...THE 
+000005b0: 534f 4654 5741 5245 2049 5320 5052 4f56  SOFTWARE IS PROV
+000005c0: 4944 4544 2022 4153 2049 5322 2041 4e44  IDED "AS IS" AND
+000005d0: 2054 4845 2041 5554 484f 5220 4449 5343   THE AUTHOR DISC
+000005e0: 4c41 494d 5320 414c 4c20 5741 5252 414e  LAIMS ALL WARRAN
+000005f0: 5449 4553 0a57 4954 4820 5245 4741 5244  TIES.WITH REGARD
+00000600: 2054 4f20 5448 4953 2053 4f46 5457 4152   TO THIS SOFTWAR
+00000610: 4520 494e 434c 5544 494e 4720 414c 4c20  E INCLUDING ALL 
+00000620: 494d 504c 4945 4420 5741 5252 414e 5449  IMPLIED WARRANTI
+00000630: 4553 204f 460a 4d45 5243 4841 4e54 4142  ES OF.MERCHANTAB
+00000640: 494c 4954 5920 414e 4420 4649 544e 4553  ILITY AND FITNES
+00000650: 532e 2049 4e20 4e4f 2045 5645 4e54 2053  S. IN NO EVENT S
+00000660: 4841 4c4c 2054 4845 2041 5554 484f 5220  HALL THE AUTHOR 
+00000670: 4245 204c 4941 424c 4520 464f 5220 414e  BE LIABLE FOR AN
+00000680: 590a 5350 4543 4941 4c2c 2044 4952 4543  Y.SPECIAL, DIREC
+00000690: 542c 2049 4e44 4952 4543 542c 204f 5220  T, INDIRECT, OR 
+000006a0: 434f 4e53 4551 5545 4e54 4941 4c20 4441  CONSEQUENTIAL DA
+000006b0: 4d41 4745 5320 4f52 2041 4e59 2044 414d  MAGES OR ANY DAM
+000006c0: 4147 4553 2057 4841 5453 4f45 5645 520a  AGES WHATSOEVER.
+000006d0: 5245 5355 4c54 494e 4720 4652 4f4d 204c  RESULTING FROM L
+000006e0: 4f53 5320 4f46 2055 5345 2c20 4441 5441  OSS OF USE, DATA
+000006f0: 204f 5220 5052 4f46 4954 532c 2057 4845   OR PROFITS, WHE
+00000700: 5448 4552 2049 4e20 414e 2041 4354 494f  THER IN AN ACTIO
+00000710: 4e20 4f46 2043 4f4e 5452 4143 542c 0a4e  N OF CONTRACT,.N
+00000720: 4547 4c49 4745 4e43 4520 4f52 204f 5448  EGLIGENCE OR OTH
+00000730: 4552 2054 4f52 5449 4f55 5320 4143 5449  ER TORTIOUS ACTI
+00000740: 4f4e 2c20 4152 4953 494e 4720 4f55 5420  ON, ARISING OUT 
+00000750: 4f46 204f 5220 494e 2043 4f4e 4e45 4354  OF OR IN CONNECT
+00000760: 494f 4e20 5749 5448 2054 4845 0a55 5345  ION WITH THE.USE
+00000770: 204f 5220 5045 5246 4f52 4d41 4e43 4520   OR PERFORMANCE 
+00000780: 4f46 2054 4849 5320 534f 4654 5741 5245  OF THIS SOFTWARE
+00000790: 2e0a 0a0a 4c69 6365 6e73 6520 6f66 2074  ....License of t
+000007a0: 6865 2067 656e 6572 6174 6f72 0a3d 3d3d  he generator.===
+000007b0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000007c0: 3d3d 3d3d 3d0a 0a43 6f70 7972 6967 6874  =====..Copyright
+000007d0: 2028 6329 2032 3031 392d 3230 3233 204d   (c) 2019-2023 M
+000007e0: 6963 6861 656c 2042 c3bc 7363 6820 3c6d  ichael B..sch <m
+000007f0: 4062 7565 732e 6368 3e0a 0a54 6869 7320  @bues.ch>..This 
+00000800: 7072 6f67 7261 6d20 6973 2066 7265 6520  program is free 
+00000810: 736f 6674 7761 7265 3b20 796f 7520 6361  software; you ca
+00000820: 6e20 7265 6469 7374 7269 6275 7465 2069  n redistribute i
+00000830: 7420 616e 642f 6f72 206d 6f64 6966 7920  t and/or modify 
+00000840: 6974 2075 6e64 6572 2074 6865 2074 6572  it under the ter
+00000850: 6d73 206f 6620 7468 6520 474e 5520 4765  ms of the GNU Ge
+00000860: 6e65 7261 6c20 5075 626c 6963 204c 6963  neral Public Lic
+00000870: 656e 7365 2061 7320 7075 626c 6973 6865  ense as publishe
+00000880: 6420 6279 2074 6865 2046 7265 6520 536f  d by the Free So
+00000890: 6674 7761 7265 2046 6f75 6e64 6174 696f  ftware Foundatio
+000008a0: 6e3b 2065 6974 6865 7220 7665 7273 696f  n; either versio
+000008b0: 6e20 3220 6f66 2074 6865 204c 6963 656e  n 2 of the Licen
+000008c0: 7365 2c20 6f72 2028 6174 2079 6f75 7220  se, or (at your 
+000008d0: 6f70 7469 6f6e 2920 616e 7920 6c61 7465  option) any late
+000008e0: 7220 7665 7273 696f 6e2e 0a0a 5468 6973  r version...This
+000008f0: 2070 726f 6772 616d 2069 7320 6469 7374   program is dist
+00000900: 7269 6275 7465 6420 696e 2074 6865 2068  ributed in the h
+00000910: 6f70 6520 7468 6174 2069 7420 7769 6c6c  ope that it will
+00000920: 2062 6520 7573 6566 756c 2c20 6275 7420   be useful, but 
+00000930: 5749 5448 4f55 5420 414e 5920 5741 5252  WITHOUT ANY WARR
+00000940: 414e 5459 3b20 7769 7468 6f75 7420 6576  ANTY; without ev
+00000950: 656e 2074 6865 2069 6d70 6c69 6564 2077  en the implied w
+00000960: 6172 7261 6e74 7920 6f66 204d 4552 4348  arranty of MERCH
+00000970: 414e 5441 4249 4c49 5459 206f 7220 4649  ANTABILITY or FI
+00000980: 544e 4553 5320 464f 5220 4120 5041 5254  TNESS FOR A PART
+00000990: 4943 554c 4152 2050 5552 504f 5345 2e20  ICULAR PURPOSE. 
+000009a0: 2053 6565 2074 6865 2047 4e55 2047 656e   See the GNU Gen
+000009b0: 6572 616c 2050 7562 6c69 6320 4c69 6365  eral Public Lice
+000009c0: 6e73 6520 666f 7220 6d6f 7265 2064 6574  nse for more det
+000009d0: 6169 6c73 2e0a 0a59 6f75 2073 686f 756c  ails...You shoul
+000009e0: 6420 6861 7665 2072 6563 6569 7665 6420  d have received 
+000009f0: 6120 636f 7079 206f 6620 7468 6520 474e  a copy of the GN
+00000a00: 5520 4765 6e65 7261 6c20 5075 626c 6963  U General Public
+00000a10: 204c 6963 656e 7365 2061 6c6f 6e67 2077   License along w
+00000a20: 6974 6820 7468 6973 2070 726f 6772 616d  ith this program
+00000a30: 3b20 6966 206e 6f74 2c20 7772 6974 6520  ; if not, write 
+00000a40: 746f 2074 6865 2046 7265 6520 536f 6674  to the Free Soft
+00000a50: 7761 7265 2046 6f75 6e64 6174 696f 6e2c  ware Foundation,
+00000a60: 2049 6e63 2e2c 2035 3120 4672 616e 6b6c   Inc., 51 Frankl
+00000a70: 696e 2053 7472 6565 742c 2046 6966 7468  in Street, Fifth
+00000a80: 2046 6c6f 6f72 2c20 426f 7374 6f6e 2c20   Floor, Boston, 
+00000a90: 4d41 2030 3231 3130 2d31 3330 3120 5553  MA 02110-1301 US
+00000aa0: 412e 0a                                  A..
```

### Comparing `crcgen-2.4/crcgen` & `crcgen-2.5/libcrcgen/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-#!/usr/bin/env python3
 # vim: ts=8 sw=8 noexpandtab
 #
 #   CRC code generator
 #
-#   Copyright (c) 2019-2021 Michael Buesch <m@bues.ch>
+#   Copyright (c) 2019-2023 Michael Büsch <m@bues.ch>
 #
 #   This program is free software; you can redistribute it and/or modify
 #   it under the terms of the GNU General Public License as published by
 #   the Free Software Foundation; either version 2 of the License, or
 #   (at your option) any later version.
 #
 #   This program is distributed in the hope that it will be useful,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `crcgen-2.4/crcgen.egg-info/PKG-INFO` & `crcgen-2.5/crcgen.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: crcgen
-Version: 2.4
+Version: 2.5
 Summary: CRC algorithm HDL code generator (VHDL, Verilog, MyHDL)
 Home-page: https://bues.ch/h/crcgen
-Author: Michael Buesch
+Author: Michael Büsch
 Author-email: m@bues.ch
 License: GNU General Public License v2 or later
 Keywords: CRC Verilog VHDL MyHDL FPGA codegenerator
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
@@ -20,14 +20,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Education
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Utilities
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: COPYING
 
 CRC algorithm HDL code generator (VHDL, Verilog, MyHDL)
 =======================================================
 
 `Homepage <https://bues.ch/h/crcgen>`_
@@ -98,14 +99,14 @@
 NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF OR IN CONNECTION WITH THE
 USE OR PERFORMANCE OF THIS SOFTWARE.
 
 
 License of the generator
 ========================
 
-Copyright (c) 2019-2022 Michael Büsch <m@bues.ch>
+Copyright (c) 2019-2023 Michael Büsch <m@bues.ch>
 
 This program is free software; you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation; either version 2 of the License, or (at your option) any later version.
 
 This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License along with this program; if not, write to the Free Software Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
```

### Comparing `crcgen-2.4/crcgen_test.py` & `crcgen-2.5/crcgen_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 #
 #  Test of CRC generator.
 #
-#   Copyright (C) 2020-2022 Michael Buesch <m@bues.ch>
+#   Copyright (C) 2020-2023 Michael Büsch <m@bues.ch>
 #
 #  Some CRC implementations are derived from AVR-libc.
 #  These copyright notices apply to the AVR-libc parts:
 #
 #   Copyright (c) 2002, 2003, 2004  Marek Michalkiewicz
 #   Copyright (c) 2005, 2007 Joerg Wunsch
 #   Copyright (c) 2013 Dave Hylands
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `crcgen-2.4/libcrcgen/__main__.py` & `crcgen-2.5/crcgen`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+#!/usr/bin/env python3
 # vim: ts=8 sw=8 noexpandtab
 #
 #   CRC code generator
 #
-#   Copyright (c) 2019-2021 Michael Buesch <m@bues.ch>
+#   Copyright (c) 2019-2023 Michael Büsch <m@bues.ch>
 #
 #   This program is free software; you can redistribute it and/or modify
 #   it under the terms of the GNU General Public License as published by
 #   the Free Software Foundation; either version 2 of the License, or
 #   (at your option) any later version.
 #
 #   This program is distributed in the hope that it will be useful,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `crcgen-2.4/libcrcgen/generator.py` & `crcgen-2.5/libcrcgen/generator.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # vim: ts=8 sw=8 noexpandtab
 #
 #   CRC code generator
 #
-#   Copyright (c) 2020-2022 Michael Buesch <m@bues.ch>
+#   Copyright (c) 2020-2023 Michael Büsch <m@bues.ch>
 #
 #   This program is free software; you can redistribute it and/or modify
 #   it under the terms of the GNU General Public License as published by
 #   the Free Software Foundation; either version 2 of the License, or
 #   (at your option) any later version.
 #
 #   This program is distributed in the hope that it will be useful,
@@ -24,82 +24,86 @@
 
 __all__ = [
 	"CrcGen",
 	"CrcGenError",
 ]
 
 @dataclass(frozen=True)
-class AbstractBit(object):
+class AbstractBit:
 	def flatten(self):
 		return [self, ]
 
 	def optimize(self, sortLex):
 		pass
 
 @dataclass(frozen=True)
 class Bit(AbstractBit):
 	name: str
 	index: int
 
-	def gen_python(self):
+	def gen_python(self, level=0):
 		return f"{self.name}[{self.index}]"
 
-	def gen_c(self):
+	def gen_c(self, level=0):
 		return f"b({self.name}, {self.index})"
 
-	def gen_verilog(self):
+	def gen_verilog(self, level=0):
 		return f"{self.name}[{self.index}]"
 
-	def gen_vhdl(self):
+	def gen_vhdl(self, level=0):
 		return f"{self.name}({self.index})"
 
-	def gen_myhdl(self):
+	def gen_myhdl(self, level=0):
 		return f"{self.name}[{self.index}]"
 
 	def sortKey(self):
 		return f"{self.name}_{self.index:07}"
 
 @dataclass(frozen=True)
 class ConstBit(AbstractBit):
 	value: int
 
-	def gen_python(self):
+	def gen_python(self, level=0):
 		return "1" if self.value else "0"
 
-	def gen_c(self):
+	def gen_c(self, level=0):
 		return "1u" if self.value else "0u"
 
-	def gen_verilog(self):
+	def gen_verilog(self, level=0):
 		return "1'b1" if self.value else "1'b0"
 
-	def gen_vhdl(self):
+	def gen_vhdl(self, level=0):
 		return 'b"1"' if self.value else 'b"0"'
 
-	def gen_myhdl(self):
+	def gen_myhdl(self, level=0):
 		return "1" if self.value else "0"
 
 	def sortKey(self):
 		return "1" if self.value else "0"
 
-class XOR(object):
+class XOR:
+	__slots__ = (
+		"__items",
+	)
+
 	def __init__(self, *items):
-		self.items = items
+		self.__items = items
 
 	def flatten(self):
 		newItems = [ item
-			     for subItem in self.items
+			     for subItem in self.__items
 			     for item in subItem.flatten() ]
-		self.items = newItems
+		self.__items = newItems
 		return newItems
 
 	def optimize(self, sortLex):
 		newItems = []
 		haveBits = {}
 		constOnes = []
-		for item in self.items:
+		for item in self.__items:
 			if isinstance(item, Bit):
 				# Store bit for even/uneven count analysis.
 				haveBits[item] = haveBits.get(item, 0) + 1
 			elif isinstance(item, ConstBit):
 				# Constant 0 does not change the XOR result. Remove it.
 				if item.value:
 					constOnes.append(item)
@@ -116,58 +120,64 @@
 		if sortLex:
 			# XOR can be arranged in any order.
 			newItems.sort(key=lambda item: item.sortKey())
 		if not newItems:
 			# All items have been optimized out.
 			# This term shall be zero.
 			newItems.append(ConstBit(0))
-		self.items = newItems
+		self.__items = newItems
 
-	def gen_python(self):
-		return self.__gen("(", ")", " ^ ", lambda item: item.gen_python())
+	def gen_python(self, level=0):
+		return self.__gen("(", ")", level, " ^ ", lambda item: item.gen_python(level + 1))
 
-	def gen_c(self):
-		return self.__gen("(", ")", " ^ ", lambda item: item.gen_c())
+	def gen_c(self, level=0):
+		return self.__gen("(", ")", level, " ^ ", lambda item: item.gen_c(level + 1))
 
-	def gen_verilog(self):
-		return self.__gen("(", ")", " ^ ", lambda item: item.gen_verilog())
+	def gen_verilog(self, level=0):
+		return self.__gen("(", ")", level, " ^ ", lambda item: item.gen_verilog(level + 1))
 
-	def gen_vhdl(self):
-		return self.__gen("(", ")", " xor ", lambda item: item.gen_vhdl())
+	def gen_vhdl(self, level=0):
+		return self.__gen("(", ")", level, " xor ", lambda item: item.gen_vhdl(level + 1))
 
-	def gen_myhdl(self):
-		return self.__gen("(", ")", " ^ ", lambda item: item.gen_myhdl())
+	def gen_myhdl(self, level=0):
+		return self.__gen("(", ")", level, " ^ ", lambda item: item.gen_myhdl(level + 1))
 
-	def __gen(self, prefix, suffix, oper, itemGen):
-		assert(self.items)
-		return prefix + (oper.join(itemGen(item) for item in self.items)) + suffix
+	def __gen(self, prefix, suffix, level, oper, itemGen):
+		assert self.__items, "Empty XOR."
+		if level == 0:
+			prefix = suffix = ""
+		return prefix + (oper.join(itemGen(item) for item in self.__items)) + suffix
 
 	def sortKey(self):
-		return "__".join(item.sortKey() for item in self.items)
+		return "__".join(item.sortKey() for item in self.__items)
+
+class Word:
+	__slots__ = (
+		"__items",
+	)
 
-class Word(object):
 	def __init__(self, *items):
 		# items must be LSB first.
-		self.items = list(items)
+		self.__items = list(items)
 
 	def __getitem__(self, index):
-		return self.items[index]
+		return self.__items[index]
 
 	def flatten(self):
-		for item in self.items:
+		for item in self.__items:
 			item.flatten()
 
 	def optimize(self, sortLex):
-		for item in self.items:
+		for item in self.__items:
 			item.optimize(sortLex)
 
 class CrcGenError(Exception):
 	pass
 
-class CrcGen(object):
+class CrcGen:
 	"""Combinatorial CRC algorithm generator.
 	"""
 
 	OPT_FLATTEN	= 1 << 0 # Flatten the bit operation tree
 	OPT_ELIMINATE	= 1 << 1 # Eliminate redundant operations
 	OPT_LEX		= 1 << 2 # Sort the operands in lexicographical order where possible
 
@@ -293,15 +303,15 @@
 		ret.extend("# " + l for l in self.__algDescription().splitlines())
 		ret.append("")
 		ret.append(f"def {funcName}({crcVarName}, {dataVarName}):")
 		ret.append(f"    class bitwrapper:")
 		ret.append(f"        def __init__(self, x):")
 		ret.append(f"            self.x = x")
 		ret.append(f"        def __getitem__(self, i):")
-		ret.append(f"            return ((self.x >> i) & 1)")
+		ret.append(f"            return (self.x >> i) & 1")
 		ret.append(f"        def __setitem__(self, i, x):")
 		ret.append(f"            self.x = (self.x | (1 << i)) if x else (self.x & ~(1 << i))")
 		ret.append(f"    {crcVarName} = bitwrapper({crcVarName})")
 		ret.append(f"    {dataVarName} = bitwrapper({dataVarName})")
 		ret.append(f"    ret = bitwrapper(0)")
 		for i, bit in enumerate(word):
 			ret.append(f"    ret[{i}] = {bit.gen_python()}")
@@ -468,15 +478,15 @@
 		ret.append(f"{extern}{static}{inline}{cCrcType} "
 			   f"{funcName}({cCrcType} {crcVarName}, {cDataType} {dataVarName}){end}")
 		if not declOnly:
 			ret.append("{")
 			ret.append(f"    {cCrcType} ret;")
 			for i, bit in enumerate(word):
 				operator = "|=" if i > 0 else " ="
-				ret.append(f"    ret {operator} ({cCrcType}){bit.gen_c()} << {i};")
+				ret.append(f"    ret {operator} ({cCrcType})({bit.gen_c()}) << {i};")
 			ret.append("    return ret;")
 			ret.append("}")
 			ret.append("#undef b")
 		if includeGuards:
 			ret.append("")
 			ret.append(f"#endif /* {funcName.upper()}_H_ */")
 		return "\n".join(ret)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `crcgen-2.4/libcrcgen/generator_test.py` & `crcgen-2.5/libcrcgen/generator_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # vim: ts=8 sw=8 noexpandtab
 #
 #   CRC code generator
 #
-#   Copyright (c) 2020-2022 Michael Buesch <m@bues.ch>
+#   Copyright (c) 2020-2023 Michael Büsch <m@bues.ch>
 #
 #   This program is free software; you can redistribute it and/or modify
 #   it under the terms of the GNU General Public License as published by
 #   the Free Software Foundation; either version 2 of the License, or
 #   (at your option) any later version.
 #
 #   This program is distributed in the hope that it will be useful,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `crcgen-2.4/libcrcgen/main.py` & `crcgen-2.5/libcrcgen/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # vim: ts=8 sw=8 noexpandtab
 #
 #   CRC code generator
 #
-#   Copyright (c) 2019-2022 Michael Buesch <m@bues.ch>
+#   Copyright (c) 2019-2023 Michael Büsch <m@bues.ch>
 #
 #   This program is free software; you can redistribute it and/or modify
 #   it under the terms of the GNU General Public License as published by
 #   the Free Software Foundation; either version 2 of the License, or
 #   (at your option) any later version.
 #
 #   This program is distributed in the hope that it will be useful,
@@ -15,30 +15,63 @@
 #   GNU General Public License for more details.
 #
 #   You should have received a copy of the GNU General Public License along
 #   with this program; if not, write to the Free Software Foundation, Inc.,
 #   51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
 #
 
-from libcrcgen import CrcGen, CrcGenError, CRC_PARAMETERS, poly2int
+from libcrcgen import CrcGen, CrcGenError, CRC_PARAMETERS, poly2int, int2poly
 
 import sys
 import argparse
 
 __all__ = [
 	"main",
 ]
 
+def poly_convert(p, nr_crc_bits, shift_right):
+	if nr_crc_bits is None:
+		raise CrcGenError("-B|--nr-crc-bits is required for -T|--polynomial-convert")
+	p = p.strip()
+	try:
+		# Hex format
+		if not p.startswith("0x"):
+			raise ValueError
+		p = int(p[2:], 16)
+		p = int2poly(p, nr_crc_bits, shift_right)
+		print(p)
+		return 0
+	except ValueError:
+		pass
+	try:
+		# Decimal format
+		p = int(p, 10)
+		p = int2poly(p, nr_crc_bits, shift_right)
+		print(p)
+		return 0
+	except ValueError:
+		pass
+	try:
+		# Polynomial coefficient format
+		p = poly2int(p, nr_crc_bits, shift_right)
+		print(f"0x{p:X}")
+		return 0
+	except ValueError:
+		pass
+	raise CrcGenError("-T|--polynomial-convert: Invalid polynomial")
+
 def main():
 	try:
 		def argInt(string):
 			if string.startswith("0x"):
 				return int(string[2:], 16)
 			return int(string)
-		p = argparse.ArgumentParser()
+		p = argparse.ArgumentParser(
+			description="CRC algorithm HDL code generator (VHDL, Verilog, MyHDL)"
+		)
 		g = p.add_mutually_exclusive_group(required=True)
 		g.add_argument("-v", "--verilog-function", action="store_true",
 			       help="Generate Verilog function")
 		g.add_argument("-m", "--verilog-module", action="store_true",
 			       help="Generate Verilog module")
 		g.add_argument("-V", "--vhdl", action="store_true",
 			       help="Generate VHDL module")
@@ -92,21 +125,17 @@
 		if (args.nr_crc_bits is not None and
 		    args.nr_crc_bits < 1):
 			raise CrcGenError("Invalid -B|--nr-crc-bits argument.")
 		if args.nr_data_bits < 1:
 			raise CrcGenError("Invalid -b|--nr-data-bits argument.")
 
 		if args.polynomial_convert is not None:
-			if args.nr_crc_bits is None:
-				raise CrcGenError("-B|--nr-crc-bits is required for -T|--polynomial-convert")
-			p = poly2int(args.polynomial_convert,
-				     args.nr_crc_bits,
-				     args.shift_right)
-			print(f"0x{p:X}")
-			return 0
+			return poly_convert(args.polynomial_convert,
+					    args.nr_crc_bits,
+					    args.shift_right)
 
 		crcParameters = CRC_PARAMETERS[args.algorithm].copy()
 		if args.nr_crc_bits is not None:
 			crcParameters["nrBits"] = args.nr_crc_bits
 		if args.shift_right:
 			crcParameters["shiftRight"] = True
 		if args.shift_left:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `crcgen-2.4/libcrcgen/parameters.py` & `crcgen-2.5/libcrcgen/parameters.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # vim: ts=8 sw=8 noexpandtab
 #
 #   CRC code generator
 #
-#   Copyright (c) 2019-2021 Michael Buesch <m@bues.ch>
+#   Copyright (c) 2019-2023 Michael Büsch <m@bues.ch>
 #
 #   This program is free software; you can redistribute it and/or modify
 #   it under the terms of the GNU General Public License as published by
 #   the Free Software Foundation; either version 2 of the License, or
 #   (at your option) any later version.
 #
 #   This program is distributed in the hope that it will be useful,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `crcgen-2.4/libcrcgen/reference.py` & `crcgen-2.5/libcrcgen/reference.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # vim: ts=8 sw=8 noexpandtab
 #
 #   CRC code generator
 #
-#   Copyright (c) 2019-2021 Michael Buesch <m@bues.ch>
+#   Copyright (c) 2019-2023 Michael Büsch <m@bues.ch>
 #
 #   This program is free software; you can redistribute it and/or modify
 #   it under the terms of the GNU General Public License as published by
 #   the Free Software Foundation; either version 2 of the License, or
 #   (at your option) any later version.
 #
 #   This program is distributed in the hope that it will be useful,
@@ -21,15 +21,15 @@
 
 __all__ = [
 	"CrcReference",
 ]
 
 from typing import Iterable
 
-class CrcReference(object):
+class CrcReference:
 	"""Generic CRC reference implementation.
 	"""
 
 	@classmethod
 	def crc(cls,
 		crc: int,
 		data: int,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `crcgen-2.4/libcrcgen/util.py` & `crcgen-2.5/libcrcgen/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # vim: ts=8 sw=8 noexpandtab
 #
 #   CRC code generator
 #
-#   Copyright (c) 2019-2022 Michael Buesch <m@bues.ch>
+#   Copyright (c) 2019-2023 Michael Büsch <m@bues.ch>
 #
 #   This program is free software; you can redistribute it and/or modify
 #   it under the terms of the GNU General Public License as published by
 #   the Free Software Foundation; either version 2 of the License, or
 #   (at your option) any later version.
 #
 #   This program is distributed in the hope that it will be useful,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `crcgen-2.4/libcrcgen/version.py` & `crcgen-2.5/libcrcgen/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # vim: ts=8 sw=8 noexpandtab
 #
 #   CRC code generator
 #
-#   Copyright (c) 2019-2022 Michael Buesch <m@bues.ch>
+#   Copyright (c) 2019-2023 Michael Büsch <m@bues.ch>
 #
 #   This program is free software; you can redistribute it and/or modify
 #   it under the terms of the GNU General Public License as published by
 #   the Free Software Foundation; either version 2 of the License, or
 #   (at your option) any later version.
 #
 #   This program is distributed in the hope that it will be useful,
@@ -23,10 +23,10 @@
 	"VERSION_MAJOR",
 	"VERSION_MINOR",
 	"VERSION_EXTRA",
 	"VERSION_STRING",
 ]
 
 VERSION_MAJOR = 2
-VERSION_MINOR = 4
+VERSION_MINOR = 5
 VERSION_EXTRA = ""
 VERSION_STRING = "%d.%d%s" % (VERSION_MAJOR, VERSION_MINOR, VERSION_EXTRA)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `crcgen-2.4/setup.py` & `crcgen-2.5/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 #!/usr/bin/env python3
 
-import sys, os
+import os
 basedir = os.path.abspath(os.path.dirname(__file__))
 
 from libcrcgen.version import VERSION_STRING
 from setuptools import setup
-import warnings
-
-warnings.filterwarnings("ignore", r".*'long_description_content_type'.*")
 
 with open(os.path.join(basedir, "README.rst"), "rb") as fd:
 	readmeText = fd.read().decode("UTF-8")
 
-setup(	name		= "crcgen",
+setup(
+	name		= "crcgen",
 	version		= VERSION_STRING,
 	description	= "CRC algorithm HDL code generator (VHDL, Verilog, MyHDL)",
 	license		= "GNU General Public License v2 or later",
-	author		= "Michael Buesch",
+	author		= "Michael Büsch",
 	author_email	= "m@bues.ch",
 	url		= "https://bues.ch/h/crcgen",
+	python_requires = ">=3.7",
 	scripts		= [
 		"crcgen",
 	],
 	packages	= [
 		"libcrcgen",
 	],
 	keywords	= "CRC Verilog VHDL MyHDL FPGA codegenerator",
@@ -44,7 +43,9 @@
 		"Topic :: Software Development",
 		"Topic :: Software Development :: Code Generators",
 		"Topic :: Utilities",
 	],
 	long_description=readmeText,
 	long_description_content_type="text/x-rst",
 )
+
+# vim: ts=8 sw=8 noexpandtab
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

