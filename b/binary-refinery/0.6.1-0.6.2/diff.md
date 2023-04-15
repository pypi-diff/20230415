# Comparing `tmp/binary-refinery-0.6.1.tar.gz` & `tmp/binary-refinery-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/refinery/refinery/dist/.tmp-oqnujb9d/binary-refinery-0.6.1.tar", last modified: Thu Apr  6 16:48:45 2023, max compression
+gzip compressed data, was "/home/runner/work/refinery/refinery/dist/.tmp-uvy8i5d_/binary-refinery-0.6.2.tar", last modified: Sat Apr 15 13:02:36 2023, max compression
```

## Comparing `binary-refinery-0.6.1.tar` & `binary-refinery-0.6.2.tar`

### file list

```diff
@@ -1,378 +1,378 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 16:48:45.000000 binary-refinery-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    17578 2023-04-06 16:48:45.000000 binary-refinery-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15746 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 16:48:45.000000 binary-refinery-0.6.1/binary_refinery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17578 2023-04-06 16:48:45.000000 binary-refinery-0.6.1/binary_refinery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11708 2023-04-06 16:48:45.000000 binary-refinery-0.6.1/binary_refinery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 16:48:45.000000 binary-refinery-0.6.1/binary_refinery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14980 2023-04-06 16:48:45.000000 binary-refinery-0.6.1/binary_refinery.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-04-06 16:48:45.000000 binary-refinery-0.6.1/binary_refinery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-06 16:48:45.000000 binary-refinery-0.6.1/binary_refinery.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 16:48:45.000000 binary-refinery-0.6.1/refinery/
--rw-r--r--   0 runner    (1001) docker     (123)    14608 2023-04-06 16:48:45.000000 binary-refinery-0.6.1/refinery/__init__.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     6758 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 16:48:45.000000 binary-refinery-0.6.1/refinery/data/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48618 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/data/rich.json
--rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/explore.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 16:48:45.000000 binary-refinery-0.6.1/refinery/lib/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    59012 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/lib/argformats.py
--rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/lib/argparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/lib/chunks.py
--rw-r--r--   0 runner    (1001) docker     (123)    15904 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/lib/crypto.py
--rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/lib/decompression.py
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/lib/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/lib/deobfuscation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/lib/dex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 16:48:45.000000 binary-refinery-0.6.1/refinery/lib/dotnet/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/lib/dotnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13791 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/lib/dotnet/deserialize.py
--rw-r--r--   0 runner    (1001) docker     (123)    30549 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/lib/dotnet/header.py
--rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/lib/dotnet/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)    10738 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/lib/dotnet/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/lib/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)    19041 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/lib/executable.py
--rw-r--r--   0 runner    (1001) docker     (123)    23050 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/lib/frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     7517 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/lib/inline.py
--rw-r--r--   0 runner    (1001) docker     (123)    23540 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/lib/java.py
--rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/lib/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/lib/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/lib/magic.py
--rw-r--r--   0 runner    (1001) docker     (123)    34226 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/lib/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     9531 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/lib/mime.py
--rw-r--r--   0 runner    (1001) docker     (123)     9966 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/lib/mscrypto.py
--rw-r--r--   0 runner    (1001) docker     (123)     8685 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/lib/murmur.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 16:48:45.000000 binary-refinery-0.6.1/refinery/lib/patterns/
--rw-r--r--   0 runner    (1001) docker     (123)    15942 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/lib/patterns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18566 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/lib/patterns/tlds.py
--rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/lib/powershell.py
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/lib/ripemd128.py
--rw-r--r--   0 runner    (1001) docker     (123)    10358 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/lib/serpent.py
--rw-r--r--   0 runner    (1001) docker     (123)    23138 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/lib/structures.py
--rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/lib/suffixtree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 16:48:45.000000 binary-refinery-0.6.1/refinery/lib/thirdparty/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/lib/thirdparty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   163388 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/lib/thirdparty/acefile.py
--rw-r--r--   0 runner    (1001) docker     (123)    16823 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/lib/thirdparty/batch_interpreter.py
--rw-r--r--   0 runner    (1001) docker     (123)   127576 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/lib/thirdparty/pcode2code.py
--rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/lib/thirdparty/xxhash.py
--rw-r--r--   0 runner    (1001) docker     (123)    10315 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/lib/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/lib/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     7044 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/lib/vfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/lib/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 16:48:45.000000 binary-refinery-0.6.1/refinery/units/
--rw-r--r--   0 runner    (1001) docker     (123)    68777 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 16:48:45.000000 binary-refinery-0.6.1/refinery/units/blockwise/
--rw-r--r--   0 runner    (1001) docker     (123)     7915 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/blockwise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/blockwise/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     5098 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/blockwise/alu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/blockwise/bitrev.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/blockwise/byteswap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/blockwise/map.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/blockwise/neg.py
--rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/blockwise/pack.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/blockwise/rev.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/blockwise/rotl.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/blockwise/rotr.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/blockwise/shl.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/blockwise/shr.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/blockwise/sub.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/blockwise/terminate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/blockwise/transpose.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/blockwise/xor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 16:48:45.000000 binary-refinery-0.6.1/refinery/units/compression/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/compression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8262 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/compression/ap.py
--rw-r--r--   0 runner    (1001) docker     (123)     9918 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/compression/blz.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/compression/bz2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5866 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/compression/decompress.py
--rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/compression/jcalg.py
--rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/compression/lz.py
--rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/compression/lz4.py
--rw-r--r--   0 runner    (1001) docker     (123)     5656 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/compression/lzf.py
--rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/compression/lzg.py
--rw-r--r--   0 runner    (1001) docker     (123)    13795 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/compression/lzip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/compression/lzjb.py
--rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/compression/lznt1.py
--rw-r--r--   0 runner    (1001) docker     (123)     9976 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/compression/lzo.py
--rw-r--r--   0 runner    (1001) docker     (123)    10404 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/compression/mscf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/compression/qlz.py
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/compression/szdd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/compression/zl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 16:48:45.000000 binary-refinery-0.6.1/refinery/units/crypto/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/crypto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 16:48:45.000000 binary-refinery-0.6.1/refinery/units/crypto/cipher/
--rw-r--r--   0 runner    (1001) docker     (123)    14404 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/crypto/cipher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/crypto/cipher/aes.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/crypto/cipher/blowfish.py
--rw-r--r--   0 runner    (1001) docker     (123)     7598 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/crypto/cipher/camellia.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/crypto/cipher/cast.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/crypto/cipher/chacha.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/crypto/cipher/des.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/crypto/cipher/des3.py
--rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/crypto/cipher/gost.py
--rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/crypto/cipher/hc128.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/crypto/cipher/isaac.py
--rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/crypto/cipher/rabbit.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/crypto/cipher/rc2.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/crypto/cipher/rc4.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/crypto/cipher/rc4mod.py
--rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/crypto/cipher/rc5.py
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/crypto/cipher/rc6.py
--rw-r--r--   0 runner    (1001) docker     (123)    48363 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/crypto/cipher/rijndael.py
--rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/crypto/cipher/rncrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/crypto/cipher/rot.py
--rw-r--r--   0 runner    (1001) docker     (123)     9683 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/crypto/cipher/rsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/crypto/cipher/rsakey.py
--rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/crypto/cipher/salsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     5771 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/crypto/cipher/seal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/crypto/cipher/secstr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/crypto/cipher/serpent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/crypto/cipher/tea.py
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/crypto/cipher/vigenere.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/crypto/cipher/xtea.py
--rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/crypto/cipher/xxtea.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 16:48:45.000000 binary-refinery-0.6.1/refinery/units/crypto/hash/
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/crypto/hash/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/crypto/hash/checksums.py
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/crypto/hash/cryptographic.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/crypto/hash/imphash.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/crypto/hash/murmur.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/crypto/hash/password_hashes.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/crypto/hash/xxhash.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 16:48:45.000000 binary-refinery-0.6.1/refinery/units/crypto/keyderive/
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/crypto/keyderive/CryptDeriveKey.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/crypto/keyderive/DESDerive.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/crypto/keyderive/PasswordDeriveBytes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/crypto/keyderive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/crypto/keyderive/hkdf.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/crypto/keyderive/hmac.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/crypto/keyderive/kblob.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/crypto/keyderive/pbkdf1.py
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/crypto/keyderive/pbkdf2.py
--rw-r--r--   0 runner    (1001) docker     (123)    19518 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/crypto/keyderive/unixcrypt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 16:48:45.000000 binary-refinery-0.6.1/refinery/units/encoding/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/encoding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/encoding/atbash.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/encoding/b32.py
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/encoding/b58.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/encoding/b64.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/encoding/b85.py
--rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/encoding/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/encoding/cp1252.py
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/encoding/esc.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/encoding/hex.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/encoding/htmlesc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/encoding/netbios.py
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/encoding/ps1str.py
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/encoding/recode.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/encoding/u16.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/encoding/url.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/encoding/uuenc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8570 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/encoding/wshenc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 16:48:45.000000 binary-refinery-0.6.1/refinery/units/formats/
--rw-r--r--   0 runner    (1001) docker     (123)     8207 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/formats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23118 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/formats/a3x.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 16:48:45.000000 binary-refinery-0.6.1/refinery/units/formats/archive/
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/formats/archive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/formats/archive/xt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/formats/archive/xt7z.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/formats/archive/xtace.py
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/formats/archive/xtasar.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/formats/archive/xtcab.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/formats/archive/xtcpio.py
--rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/formats/archive/xtiso.py
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/formats/archive/xtiss.py
--rw-r--r--   0 runner    (1001) docker     (123)    46905 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/formats/archive/xtnsis.py
--rw-r--r--   0 runner    (1001) docker     (123)    20487 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/formats/archive/xtpyi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/formats/archive/xttar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/formats/archive/xtzip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/formats/bat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/formats/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/formats/deserialize_php.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/formats/dexstr.py
--rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/formats/email.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/formats/evtx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 16:48:45.000000 binary-refinery-0.6.1/refinery/units/formats/exe/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/formats/exe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/formats/exe/vaddr.py
--rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/formats/exe/vmemref.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/formats/exe/vsect.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/formats/exe/vsnip.py
--rw-r--r--   0 runner    (1001) docker     (123)    10787 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/formats/exe/vstack.py
--rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/formats/hexload.py
--rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/formats/html.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/formats/httpresponse.py
--rw-r--r--   0 runner    (1001) docker     (123)    30158 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/formats/ifps.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/formats/ifpsstr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 16:48:45.000000 binary-refinery-0.6.1/refinery/units/formats/java/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/formats/java/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/formats/java/deserialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/formats/java/jvdasm.py
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/formats/java/jvstr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/formats/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/formats/lnk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/formats/msgpack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 16:48:45.000000 binary-refinery-0.6.1/refinery/units/formats/office/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/formats/office/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/formats/office/doctxt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/formats/office/officecrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/formats/office/vbapc.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/formats/office/vbastr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/formats/office/xlmdeobf.py
--rw-r--r--   0 runner    (1001) docker     (123)     9301 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/formats/office/xlxtr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/formats/office/xtdoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/formats/office/xtone.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/formats/office/xtrtf.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/formats/office/xtvba.py
--rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/formats/pcap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/formats/pcap_http.py
--rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/formats/pdf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 16:48:45.000000 binary-refinery-0.6.1/refinery/units/formats/pe/
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/formats/pe/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 16:48:45.000000 binary-refinery-0.6.1/refinery/units/formats/pe/dotnet/
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/formats/pe/dotnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/formats/pe/dotnet/dnblob.py
--rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/formats/pe/dotnet/dncfx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/formats/pe/dotnet/dnds.py
--rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/formats/pe/dotnet/dnfields.py
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/formats/pe/dotnet/dnhdr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/formats/pe/dotnet/dnmr.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/formats/pe/dotnet/dnrc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/formats/pe/dotnet/dnstr.py
--rw-r--r--   0 runner    (1001) docker     (123)    30943 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/formats/pe/pemeta.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/formats/pe/peoverlay.py
--rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/formats/pe/perc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/formats/pe/pesig.py
--rw-r--r--   0 runner    (1001) docker     (123)    11548 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/formats/pe/pestrip.py
--rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/formats/pkcs7.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/formats/pkcs7sig.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/formats/stego.py
--rw-r--r--   0 runner    (1001) docker     (123)     5594 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/formats/winreg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/formats/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 16:48:45.000000 binary-refinery-0.6.1/refinery/units/malware/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/malware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/malware/n40.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 16:48:45.000000 binary-refinery-0.6.1/refinery/units/meta/
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/meta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/meta/chop.py
--rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/meta/cm.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/meta/cull.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/meta/dedup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/meta/eat.py
--rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/meta/ef.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/meta/emit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/meta/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/meta/groupby.py
--rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/meta/iff.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/meta/iffp.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/meta/iffs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/meta/iffx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/meta/max.py
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/meta/min.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/meta/mvc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/meta/mvg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/meta/pad.py
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/meta/pick.py
--rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/meta/pop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/meta/push.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/meta/put.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/meta/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/meta/reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/meta/scope.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/meta/sep.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/meta/sorted.py
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/meta/swap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/meta/xfcc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 16:48:45.000000 binary-refinery-0.6.1/refinery/units/misc/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/misc/autoxor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/misc/couple.py
--rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/misc/datefix.py
--rw-r--r--   0 runner    (1001) docker     (123)     7332 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/misc/drp.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/misc/nop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/misc/urlfix.py
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/misc/xkey.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 16:48:45.000000 binary-refinery-0.6.1/refinery/units/obfuscation/
--rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/obfuscation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 16:48:45.000000 binary-refinery-0.6.1/refinery/units/obfuscation/js/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/obfuscation/js/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/obfuscation/js/arrays.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/obfuscation/js/getattr.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/obfuscation/js/tuples.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 16:48:45.000000 binary-refinery-0.6.1/refinery/units/obfuscation/ps1/
--rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/obfuscation/ps1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/obfuscation/ps1/all.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/obfuscation/ps1/brackets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/obfuscation/ps1/cases.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/obfuscation/ps1/concat.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/obfuscation/ps1/escape.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/obfuscation/ps1/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/obfuscation/ps1/invoke.py
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/obfuscation/ps1/securestring.py
--rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/obfuscation/ps1/stringreplace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/obfuscation/ps1/typecast.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/obfuscation/ps1/uncurly.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 16:48:45.000000 binary-refinery-0.6.1/refinery/units/obfuscation/vba/
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/obfuscation/vba/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/obfuscation/vba/all.py
--rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/obfuscation/vba/arithmetic.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/obfuscation/vba/brackets.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/obfuscation/vba/char.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/obfuscation/vba/comments.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/obfuscation/vba/concat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/obfuscation/vba/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/obfuscation/vba/dummies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/obfuscation/vba/stringreplace.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/obfuscation/vba/stringreverse.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/obfuscation/vba/vba.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 16:48:45.000000 binary-refinery-0.6.1/refinery/units/pattern/
--rw-r--r--   0 runner    (1001) docker     (123)     6639 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/pattern/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/pattern/carve.py
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/pattern/carve_7z.py
--rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/pattern/carve_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/pattern/carve_lnk.py
--rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/pattern/carve_pe.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/pattern/carve_rtf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/pattern/carve_xml.py
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/pattern/carve_zip.py
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/pattern/defang.py
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/pattern/dnsdomain.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/pattern/mimewords.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/pattern/resplit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/pattern/resub.py
--rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/pattern/rex.py
--rw-r--r--   0 runner    (1001) docker     (123)     9282 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/pattern/struct_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/pattern/subfiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/pattern/urlguards.py
--rw-r--r--   0 runner    (1001) docker     (123)    14161 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/pattern/xtp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/pattern/xtw.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 16:48:45.000000 binary-refinery-0.6.1/refinery/units/sinks/
--rw-r--r--   0 runner    (1001) docker     (123)     7614 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/sinks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8489 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/sinks/asm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7171 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/sinks/dump.py
--rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/sinks/iemap.py
--rw-r--r--   0 runner    (1001) docker     (123)    10509 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/sinks/peek.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/sinks/ppjscript.py
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/sinks/ppjson.py
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/sinks/ppxml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 16:48:45.000000 binary-refinery-0.6.1/refinery/units/strings/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/strings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/strings/cca.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/strings/ccp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/strings/cfmt.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/strings/clower.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/strings/cswap.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/strings/cupper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/strings/rep.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/strings/repl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/strings/snip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/strings/stretch.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/strings/termfit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/refinery/units/strings/trim.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-06 16:48:45.000000 binary-refinery-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-04-06 16:48:28.000000 binary-refinery-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:02:36.000000 binary-refinery-0.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    17604 2023-04-15 13:02:36.000000 binary-refinery-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15746 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:02:36.000000 binary-refinery-0.6.2/binary_refinery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17604 2023-04-15 13:02:36.000000 binary-refinery-0.6.2/binary_refinery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11708 2023-04-15 13:02:36.000000 binary-refinery-0.6.2/binary_refinery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 13:02:36.000000 binary-refinery-0.6.2/binary_refinery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14980 2023-04-15 13:02:36.000000 binary-refinery-0.6.2/binary_refinery.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-04-15 13:02:36.000000 binary-refinery-0.6.2/binary_refinery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-15 13:02:36.000000 binary-refinery-0.6.2/binary_refinery.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:02:36.000000 binary-refinery-0.6.2/refinery/
+-rw-r--r--   0 runner    (1001) docker     (123)    14608 2023-04-15 13:02:36.000000 binary-refinery-0.6.2/refinery/__init__.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     6758 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:02:36.000000 binary-refinery-0.6.2/refinery/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49846 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/data/rich.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/explore.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:02:36.000000 binary-refinery-0.6.2/refinery/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59012 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/lib/argformats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/lib/argparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/lib/chunks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16375 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/lib/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/lib/decompression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/lib/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/lib/deobfuscation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/lib/dex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:02:36.000000 binary-refinery-0.6.2/refinery/lib/dotnet/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/lib/dotnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13791 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/lib/dotnet/deserialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30549 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/lib/dotnet/header.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/lib/dotnet/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10738 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/lib/dotnet/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/lib/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19041 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/lib/executable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23050 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/lib/frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7517 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/lib/inline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23540 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/lib/java.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/lib/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/lib/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/lib/magic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34226 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/lib/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9531 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/lib/mime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9966 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/lib/mscrypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8685 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/lib/murmur.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:02:36.000000 binary-refinery-0.6.2/refinery/lib/patterns/
+-rw-r--r--   0 runner    (1001) docker     (123)    15942 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/lib/patterns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18566 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/lib/patterns/tlds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/lib/powershell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/lib/ripemd128.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10358 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/lib/serpent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23138 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/lib/structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/lib/suffixtree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:02:36.000000 binary-refinery-0.6.2/refinery/lib/thirdparty/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/lib/thirdparty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   163388 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/lib/thirdparty/acefile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16823 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/lib/thirdparty/batch_interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (123)   127576 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/lib/thirdparty/pcode2code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/lib/thirdparty/xxhash.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10315 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/lib/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/lib/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7044 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/lib/vfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/lib/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:02:36.000000 binary-refinery-0.6.2/refinery/units/
+-rw-r--r--   0 runner    (1001) docker     (123)    69008 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:02:36.000000 binary-refinery-0.6.2/refinery/units/blockwise/
+-rw-r--r--   0 runner    (1001) docker     (123)     7915 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/blockwise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/blockwise/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5098 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/blockwise/alu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/blockwise/bitrev.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/blockwise/byteswap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/blockwise/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/blockwise/neg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/blockwise/pack.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/blockwise/rev.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/blockwise/rotl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/blockwise/rotr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/blockwise/shl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/blockwise/shr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/blockwise/sub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/blockwise/terminate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/blockwise/transpose.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/blockwise/xor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:02:36.000000 binary-refinery-0.6.2/refinery/units/compression/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/compression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8262 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/compression/ap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9918 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/compression/blz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/compression/bz2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5866 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/compression/decompress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/compression/jcalg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/compression/lz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/compression/lz4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5656 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/compression/lzf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/compression/lzg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13795 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/compression/lzip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/compression/lzjb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/compression/lznt1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9976 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/compression/lzo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10404 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/compression/mscf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/compression/qlz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/compression/szdd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/compression/zl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:02:36.000000 binary-refinery-0.6.2/refinery/units/crypto/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:02:36.000000 binary-refinery-0.6.2/refinery/units/crypto/cipher/
+-rw-r--r--   0 runner    (1001) docker     (123)    14404 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/cipher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/cipher/aes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/cipher/blowfish.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7598 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/cipher/camellia.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/cipher/cast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/cipher/chacha.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/cipher/des.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/cipher/des3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/cipher/gost.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/cipher/hc128.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/cipher/isaac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/cipher/rabbit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/cipher/rc2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/cipher/rc4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/cipher/rc4mod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/cipher/rc5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/cipher/rc6.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48363 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/cipher/rijndael.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/cipher/rncrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/cipher/rot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9683 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/cipher/rsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/cipher/rsakey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/cipher/salsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5771 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/cipher/seal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/cipher/secstr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/cipher/serpent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/cipher/tea.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/cipher/vigenere.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/cipher/xtea.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/cipher/xxtea.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:02:36.000000 binary-refinery-0.6.2/refinery/units/crypto/hash/
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/hash/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/hash/checksums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/hash/cryptographic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/hash/imphash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/hash/murmur.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/hash/password_hashes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/hash/xxhash.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:02:36.000000 binary-refinery-0.6.2/refinery/units/crypto/keyderive/
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/keyderive/CryptDeriveKey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/keyderive/DESDerive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/keyderive/PasswordDeriveBytes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/keyderive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/keyderive/hkdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/keyderive/hmac.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/keyderive/kblob.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/keyderive/pbkdf1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/keyderive/pbkdf2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19518 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/crypto/keyderive/unixcrypt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:02:36.000000 binary-refinery-0.6.2/refinery/units/encoding/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/encoding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/encoding/atbash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/encoding/b32.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/encoding/b58.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/encoding/b64.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/encoding/b85.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/encoding/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/encoding/cp1252.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/encoding/esc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/encoding/hex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/encoding/htmlesc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/encoding/netbios.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/encoding/ps1str.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/encoding/recode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/encoding/u16.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/encoding/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/encoding/uuenc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8570 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/encoding/wshenc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:02:36.000000 binary-refinery-0.6.2/refinery/units/formats/
+-rw-r--r--   0 runner    (1001) docker     (123)     8207 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23253 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/a3x.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:02:36.000000 binary-refinery-0.6.2/refinery/units/formats/archive/
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/archive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/archive/xt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/archive/xt7z.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/archive/xtace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/archive/xtasar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/archive/xtcab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/archive/xtcpio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/archive/xtiso.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/archive/xtiss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46905 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/archive/xtnsis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20487 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/archive/xtpyi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/archive/xttar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/archive/xtzip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/bat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/deserialize_php.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/dexstr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/evtx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:02:36.000000 binary-refinery-0.6.2/refinery/units/formats/exe/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/exe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/exe/vaddr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/exe/vmemref.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/exe/vsect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/exe/vsnip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10787 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/exe/vstack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/hexload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/httpresponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30158 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/ifps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/ifpsstr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:02:36.000000 binary-refinery-0.6.2/refinery/units/formats/java/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/java/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/java/deserialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/java/jvdasm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/java/jvstr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/lnk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/msgpack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:02:36.000000 binary-refinery-0.6.2/refinery/units/formats/office/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/office/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/office/doctxt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/office/officecrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/office/vbapc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/office/vbastr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/office/xlmdeobf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9301 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/office/xlxtr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/office/xtdoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/office/xtone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/office/xtrtf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/office/xtvba.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/pcap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/pcap_http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/pdf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:02:36.000000 binary-refinery-0.6.2/refinery/units/formats/pe/
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/pe/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:02:36.000000 binary-refinery-0.6.2/refinery/units/formats/pe/dotnet/
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/pe/dotnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/pe/dotnet/dnblob.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/pe/dotnet/dncfx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/pe/dotnet/dnds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/pe/dotnet/dnfields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/pe/dotnet/dnhdr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/pe/dotnet/dnmr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/pe/dotnet/dnrc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/pe/dotnet/dnstr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30943 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/pe/pemeta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/pe/peoverlay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/pe/perc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/pe/pesig.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11548 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/pe/pestrip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/pkcs7.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/pkcs7sig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/stego.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5594 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/winreg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/formats/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:02:36.000000 binary-refinery-0.6.2/refinery/units/malware/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/malware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/malware/n40.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:02:36.000000 binary-refinery-0.6.2/refinery/units/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/meta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/meta/chop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/meta/cm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/meta/cull.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/meta/dedup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/meta/eat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/meta/ef.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/meta/emit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/meta/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/meta/groupby.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/meta/iff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/meta/iffp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/meta/iffs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/meta/iffx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/meta/max.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/meta/min.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/meta/mvc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/meta/mvg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/meta/pad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/meta/pick.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/meta/pop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/meta/push.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/meta/put.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/meta/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/meta/reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/meta/scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/meta/sep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/meta/sorted.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/meta/swap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/meta/xfcc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:02:36.000000 binary-refinery-0.6.2/refinery/units/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/misc/autoxor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/misc/couple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/misc/datefix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7332 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/misc/drp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/misc/nop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/misc/urlfix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/misc/xkey.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:02:36.000000 binary-refinery-0.6.2/refinery/units/obfuscation/
+-rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/obfuscation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:02:36.000000 binary-refinery-0.6.2/refinery/units/obfuscation/js/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/obfuscation/js/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/obfuscation/js/arrays.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/obfuscation/js/getattr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/obfuscation/js/tuples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:02:36.000000 binary-refinery-0.6.2/refinery/units/obfuscation/ps1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/obfuscation/ps1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/obfuscation/ps1/all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/obfuscation/ps1/brackets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/obfuscation/ps1/cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/obfuscation/ps1/concat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/obfuscation/ps1/escape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/obfuscation/ps1/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/obfuscation/ps1/invoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/obfuscation/ps1/securestring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/obfuscation/ps1/stringreplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/obfuscation/ps1/typecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/obfuscation/ps1/uncurly.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:02:36.000000 binary-refinery-0.6.2/refinery/units/obfuscation/vba/
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/obfuscation/vba/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/obfuscation/vba/all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/obfuscation/vba/arithmetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/obfuscation/vba/brackets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/obfuscation/vba/char.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/obfuscation/vba/comments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/obfuscation/vba/concat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/obfuscation/vba/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/obfuscation/vba/dummies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/obfuscation/vba/stringreplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/obfuscation/vba/stringreverse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/obfuscation/vba/vba.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:02:36.000000 binary-refinery-0.6.2/refinery/units/pattern/
+-rw-r--r--   0 runner    (1001) docker     (123)     6639 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/pattern/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/pattern/carve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/pattern/carve_7z.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/pattern/carve_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/pattern/carve_lnk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/pattern/carve_pe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/pattern/carve_rtf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/pattern/carve_xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/pattern/carve_zip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/pattern/defang.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/pattern/dnsdomain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/pattern/mimewords.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/pattern/resplit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/pattern/resub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/pattern/rex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9282 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/pattern/struct_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/pattern/subfiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/pattern/urlguards.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14161 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/pattern/xtp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/pattern/xtw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:02:36.000000 binary-refinery-0.6.2/refinery/units/sinks/
+-rw-r--r--   0 runner    (1001) docker     (123)     7614 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/sinks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8489 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/sinks/asm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7171 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/sinks/dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/sinks/iemap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10571 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/sinks/peek.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/sinks/ppjscript.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/sinks/ppjson.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/sinks/ppxml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:02:36.000000 binary-refinery-0.6.2/refinery/units/strings/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/strings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/strings/cca.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/strings/ccp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/strings/cfmt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/strings/clower.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/strings/cswap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/strings/cupper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/strings/rep.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/strings/repl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/strings/snip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/strings/stretch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/strings/termfit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/refinery/units/strings/trim.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-15 13:02:36.000000 binary-refinery-0.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-04-15 13:02:21.000000 binary-refinery-0.6.2/setup.py
```

### Comparing `binary-refinery-0.6.1/LICENSE` & `binary-refinery-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/PKG-INFO` & `binary-refinery-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: binary-refinery
-Version: 0.6.1
+Version: 0.6.2
 Summary: A toolkit to transform and refine (mostly) binary data.
 Home-page: https://github.com/binref/refinery/
 Author: Jesko Huettenhain
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -21,14 +21,15 @@
 Provides-Extra: bitrev
 Provides-Extra: neg
 Provides-Extra: rotl
 Provides-Extra: rotr
 Provides-Extra: shl
 Provides-Extra: shr
 Provides-Extra: sub
+Provides-Extra: transpose
 Provides-Extra: xor
 Provides-Extra: chacha
 Provides-Extra: hc128
 Provides-Extra: isaac
 Provides-Extra: rabbit
 Provides-Extra: rc4mod
 Provides-Extra: salsa
```

### Comparing `binary-refinery-0.6.1/README.md` & `binary-refinery-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/binary_refinery.egg-info/PKG-INFO` & `binary-refinery-0.6.2/binary_refinery.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: binary-refinery
-Version: 0.6.1
+Version: 0.6.2
 Summary: A toolkit to transform and refine (mostly) binary data.
 Home-page: https://github.com/binref/refinery/
 Author: Jesko Huettenhain
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -21,14 +21,15 @@
 Provides-Extra: bitrev
 Provides-Extra: neg
 Provides-Extra: rotl
 Provides-Extra: rotr
 Provides-Extra: shl
 Provides-Extra: shr
 Provides-Extra: sub
+Provides-Extra: transpose
 Provides-Extra: xor
 Provides-Extra: chacha
 Provides-Extra: hc128
 Provides-Extra: isaac
 Provides-Extra: rabbit
 Provides-Extra: rc4mod
 Provides-Extra: salsa
```

### Comparing `binary-refinery-0.6.1/binary_refinery.egg-info/SOURCES.txt` & `binary-refinery-0.6.2/binary_refinery.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/binary_refinery.egg-info/entry_points.txt` & `binary-refinery-0.6.2/binary_refinery.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/binary_refinery.egg-info/requires.txt` & `binary-refinery-0.6.2/binary_refinery.egg-info/requires.txt`

 * *Files 5% similar despite different names*

```diff
@@ -5,54 +5,54 @@
 pefile
 pycryptodome
 pyelftools
 setuptools
 toml
 wheel
 python-magic
+pyperclip
 asn1crypto
-capstone
-py7zr
-phpserialize
-xlrd2
-python-registry
+uncompyle6
+extract_msg
 xdis
-pyxlsb2
-openpyxl
 pycdlib
-LnkParse3
+msoffcrypto-tool
+pyonenote
+Pillow
+phpserialize
+chardet
 olefile
-uncompyle6
+xlrd2
+capstone
+LnkParse3
 decompyle3
-extract_msg
-PyPDF2>=3.0.0
+python-registry
+javaobj-py3>=0.4.0.1
+pyxlsb2
 cabarchive
-pyperclip
+openpyxl
+py7zr
 XLMMacroDeobfuscator
-javaobj-py3>=0.4.0.1
-Pillow
-pyonenote
-chardet
-msoffcrypto-tool
+PyPDF2>=3.0.0
 
 [add]
 numpy
 
 [all]
 capstone
-pypcapkit[scapy]<0.16.0
-numpy
-intervaltree
-jsbeautifier
-oletools
+colorama
 angr
 python-evtx
 chardet
-colorama
+oletools
+numpy
+pypcapkit[scapy]<0.16.0
+intervaltree
 unicorn
+jsbeautifier
 
 [alu]
 numpy
 
 [asm]
 angr
 
@@ -109,27 +109,30 @@
 
 [shr]
 numpy
 
 [sub]
 numpy
 
+[transpose]
+numpy
+
 [vbapc]
 oletools
 
 [vbastr]
 oletools
 
 [vmemref]
 angr
 
 [vstack]
+intervaltree
 capstone
 unicorn
-intervaltree
 
 [xor]
 numpy
 
 [xtrtf]
 oletools
```

### Comparing `binary-refinery-0.6.1/refinery/__init__.pkl` & `binary-refinery-0.6.2/refinery/__init__.pkl`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/__init__.py` & `binary-refinery-0.6.2/refinery/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 1. `refinery.lib.frame`: framing syntax for working on lists of binary chunks
 2. `refinery.lib.argformats`: the multibin syntax for refinery arguments
 3. `refinery.lib.meta`: defining and using metadata variables within frames
 4. `refinery.units`: writing custom units, add command-line arguments, and how to use refinery
    units within Python code.
 """
-__version__ = '0.6.1'
+__version__ = '0.6.2'
 __distribution__ = 'binary-refinery'
 
 from typing import Dict, List, Optional, Type
 from importlib import resources
 from datetime import datetime
 
 import pickle
```

### Comparing `binary-refinery-0.6.1/refinery/data/rich.json` & `binary-refinery-0.6.2/refinery/data/rich.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9914001937984496%*

 * *Differences: {"'ver'": "{'7B8D': {'ide': 'Visual Studio 2015', 'ver': '14.0'}, '673C': {'ide': 'Visual Studio "*

 * *          "2015', 'ver': '14.0'}, '1168': OrderedDict([('ide', 'Visual Studio 6.0'), ('ver', "*

 * *          "'6.0')]), '18D9': OrderedDict([('ide', 'Visual Studio 6.0'), ('ver', '6.0')]), '112D': "*

 * *          "OrderedDict([('ide', 'Visual Studio'), ('ver', '')]), '1137': OrderedDict([('ide', "*

 * *          "'Visual Studio'), ('ver', '')]), '1140': OrderedDict([('ide', 'Visual Studio'), ('ver', "*

 * *          "'')]), '11 […]*

```diff
@@ -273,14 +273,17 @@
         "010E": "Utc1900_POGO_O_CPP"
     },
     "ver": {
         "0000": {
             "ide": "Visual Studio",
             "ver": ""
         },
+        "0001": {
+            "ide": "CVTPGD (VS2019?)"
+        },
         "041F": {
             "ide": ".NET Framework",
             "ver": "4.6"
         },
         "042F": {
             "ide": "Visual Studio 2003",
             "ver": "7.10"
@@ -405,22 +408,78 @@
             "ide": "Visual Studio 2003",
             "ver": "7.10 SDK"
         },
         "10E2": {
             "ide": ".NET Framework",
             "ver": "1.1"
         },
+        "112D": {
+            "ide": "Visual Studio",
+            "ver": ""
+        },
+        "1137": {
+            "ide": "Visual Studio",
+            "ver": ""
+        },
+        "1140": {
+            "ide": "Visual Studio",
+            "ver": ""
+        },
+        "114A": {
+            "ide": "Visual Studio",
+            "ver": ""
+        },
+        "1154": {
+            "ide": "Visual Studio",
+            "ver": ""
+        },
+        "115E": {
+            "ide": "Visual Studio",
+            "ver": ""
+        },
+        "1168": {
+            "ide": "Visual Studio 6.0",
+            "ver": "6.0"
+        },
+        "1171": {
+            "ide": "Visual Studio",
+            "ver": ""
+        },
         "178E": {
             "ide": "Visual Studio 2003",
             "ver": "7.10 SP1"
         },
         "17D5": {
             "ide": "Visual Studio 2003",
             "ver": "7.10 SP1"
         },
+        "18A8": {
+            "ide": "Visual Studio",
+            "ver": ""
+        },
+        "18B1": {
+            "ide": "Visual Studio",
+            "ver": ""
+        },
+        "18BB": {
+            "ide": "Visual Studio",
+            "ver": ""
+        },
+        "18C5": {
+            "ide": "Visual Studio",
+            "ver": ""
+        },
+        "18CF": {
+            "ide": "Visual Studio",
+            "ver": ""
+        },
+        "18D9": {
+            "ide": "Visual Studio 6.0",
+            "ver": "6.0"
+        },
         "18EA": {
             "ide": "Visual Studio 2002",
             "ver": "7.0"
         },
         "1A30": {
             "ide": "Visual Studio 2002",
             "ver": "7.0"
@@ -1051,15 +1110,16 @@
             "ver": "15.2.0 preview 2"
         },
         "6738": {
             "ide": "Visual Studio 2017",
             "ver": "15.2.0 preview 3"
         },
         "673C": {
-            "ide": "VS2017 v15.7.1 build 26428 (*)"
+            "ide": "Visual Studio 2015",
+            "ver": "14.0"
         },
         "673D": {
             "ide": "VS2017 v15.7.2 build 26429 (*)"
         },
         "673E": {
             "ide": "Visual Studio 2017",
             "ver": "15.2.x"
@@ -1902,15 +1962,16 @@
         "7B8B": {
             "ide": "VS2022 v17.3.0 pre 3.0 build 31627"
         },
         "7B8C": {
             "ide": "VS2022 v17.3.0 pre 4.0 build 31628 (*)"
         },
         "7B8D": {
-            "ide": "VS2022 v17.3.0 build 31629"
+            "ide": "Visual Studio 2015",
+            "ver": "14.0"
         },
         "7B8E": {
             "ide": "Visual Studio 2015",
             "ver": "14.0"
         },
         "7BE9": {
             "ide": "VS2022 v17.4.0 pre 1.0 build 31721"
@@ -1947,17 +2008,23 @@
         },
         "7DD5": {
             "ide": "VS2022 v17.5.0 pre 4.0 build 32213"
         },
         "7DD7": {
             "ide": "VS2022 v17.5.0 build 32215"
         },
+        "7DD8": {
+            "ide": "VS2022 v17.5.3 build 32216"
+        },
         "7E43": {
             "ide": "VS2022 v17.6.0 pre 1.0 build 32323"
         },
+        "7EF6": {
+            "ide": "VS2022 v17.6.0 pre 2.0 build 32502"
+        },
         "9CB3": {
             "ide": "Visual Studio 2013",
             "ver": "12.10"
         },
         "9CB4": {
             "ide": "Visual Studio 2013",
             "ver": "12.10"
```

### Comparing `binary-refinery-0.6.1/refinery/explore.py` & `binary-refinery-0.6.2/refinery/explore.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/lib/argformats.py` & `binary-refinery-0.6.2/refinery/lib/argformats.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/lib/argparser.py` & `binary-refinery-0.6.2/refinery/lib/argparser.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/lib/chunks.py` & `binary-refinery-0.6.2/refinery/lib/chunks.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/lib/crypto.py` & `binary-refinery-0.6.2/refinery/lib/crypto.py`

 * *Files 5% similar despite different names*

```diff
@@ -459,23 +459,31 @@
             setattr(self, F'MODE_{name}', mode._identifier)
             self._modes.append(mode)
 
     def new(self, key, mode=None, **args) -> CipherInterface:
         if mode is not None:
             mode = self._modes[mode]
         mode_arguments = {}
+        cipher = self.cipher
         for arg in ('iv', 'counter', 'initial_value', 'nonce', 'mode', 'segment_size'):
             try:
                 mode_arguments[arg] = args.pop(arg)
             except KeyError:
                 pass
         if mode is CTR:
-            mode_arguments.update(block_size=self.cipher.block_size)
+            block_size = cipher.block_size
+            if not isinstance(block_size, int):
+                # This happens for ciphers that do not have a fixed block size, i.e. the
+                # block size is truly an instance attribute and not a class property.
+                # In this case, we create a temporary cipher object and use it to obtain
+                # the true block size.
+                block_size = cipher(key, ECB, **args).block_size
+            mode_arguments.update(block_size=block_size)
         mode = mode(**mode_arguments)
-        return self.cipher(key, mode, **args)
+        return cipher(key, mode, **args)
 
     @property
     def name(self):
         return self.cipher.__name__
 
     @property
     def key_size(self):
```

### Comparing `binary-refinery-0.6.1/refinery/lib/decompression.py` & `binary-refinery-0.6.2/refinery/lib/decompression.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/lib/decorators.py` & `binary-refinery-0.6.2/refinery/lib/decorators.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/lib/deobfuscation.py` & `binary-refinery-0.6.2/refinery/lib/deobfuscation.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/lib/dex.py` & `binary-refinery-0.6.2/refinery/lib/dex.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/lib/dotnet/deserialize.py` & `binary-refinery-0.6.2/refinery/lib/dotnet/deserialize.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/lib/dotnet/header.py` & `binary-refinery-0.6.2/refinery/lib/dotnet/header.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/lib/dotnet/resources.py` & `binary-refinery-0.6.2/refinery/lib/dotnet/resources.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/lib/dotnet/types.py` & `binary-refinery-0.6.2/refinery/lib/dotnet/types.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/lib/environment.py` & `binary-refinery-0.6.2/refinery/lib/environment.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/lib/executable.py` & `binary-refinery-0.6.2/refinery/lib/executable.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/lib/frame.py` & `binary-refinery-0.6.2/refinery/lib/frame.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/lib/inline.py` & `binary-refinery-0.6.2/refinery/lib/inline.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/lib/java.py` & `binary-refinery-0.6.2/refinery/lib/java.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/lib/json.py` & `binary-refinery-0.6.2/refinery/lib/json.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/lib/loader.py` & `binary-refinery-0.6.2/refinery/lib/loader.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/lib/magic.py` & `binary-refinery-0.6.2/refinery/lib/magic.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/lib/meta.py` & `binary-refinery-0.6.2/refinery/lib/meta.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/lib/mime.py` & `binary-refinery-0.6.2/refinery/lib/mime.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/lib/mscrypto.py` & `binary-refinery-0.6.2/refinery/lib/mscrypto.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/lib/murmur.py` & `binary-refinery-0.6.2/refinery/lib/murmur.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/lib/patterns/__init__.py` & `binary-refinery-0.6.2/refinery/lib/patterns/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/lib/patterns/tlds.py` & `binary-refinery-0.6.2/refinery/lib/patterns/tlds.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/lib/powershell.py` & `binary-refinery-0.6.2/refinery/lib/powershell.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/lib/ripemd128.py` & `binary-refinery-0.6.2/refinery/lib/ripemd128.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/lib/serpent.py` & `binary-refinery-0.6.2/refinery/lib/serpent.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/lib/structures.py` & `binary-refinery-0.6.2/refinery/lib/structures.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/lib/suffixtree.py` & `binary-refinery-0.6.2/refinery/lib/suffixtree.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/lib/thirdparty/acefile.py` & `binary-refinery-0.6.2/refinery/lib/thirdparty/acefile.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/lib/thirdparty/batch_interpreter.py` & `binary-refinery-0.6.2/refinery/lib/thirdparty/batch_interpreter.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/lib/thirdparty/pcode2code.py` & `binary-refinery-0.6.2/refinery/lib/thirdparty/pcode2code.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/lib/thirdparty/xxhash.py` & `binary-refinery-0.6.2/refinery/lib/thirdparty/xxhash.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/lib/tools.py` & `binary-refinery-0.6.2/refinery/lib/tools.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/lib/types.py` & `binary-refinery-0.6.2/refinery/lib/types.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/lib/vfs.py` & `binary-refinery-0.6.2/refinery/lib/vfs.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/lib/xml.py` & `binary-refinery-0.6.2/refinery/lib/xml.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/__init__.py` & `binary-refinery-0.6.2/refinery/units/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1100,49 +1100,58 @@
     def finish(self) -> Iterable[Chunk]:
         """
         Child classes of `refinery.units.Unit` can overwrite this method to generate a
         stream of chunks to be processed after the last frame has been processed.
         """
 
 
+class requirement(property):
+    pass
+
+
 class Unit(UnitBase, abstract=True):
     """
     The base class for all refinery units. It implements a small set of globally
     available options and the handling for multiple inputs and outputs. All units
     implement the _framing_ syntax for producing multiple outputs and ingesting
     multiple inputs in a common format. For more details, see `refinery.lib.frame`.
     """
     Arg = Arg
 
     optional_dependencies: Optional[Set[str]] = None
     required_dependencies: Optional[Set[str]] = None
 
     @staticmethod
     def Requires(distribution: str, optional: bool = True):
-        class Requirement(property):
+        class Requirement(requirement):
             dependency = distribution
-            prefix = 'optional' if optional else 'required'
+            required = not optional
 
             def __init__(self, importer: Callable):
                 super().__init__(importer)
                 self.module = None
 
             def __set_name__(self, unit: Type[Unit], name: str):
-                bucket = F'{self.prefix}_dependencies'
-                dep = getattr(unit, bucket)
-                if dep is None:
-                    dep = set()
-                    setattr(unit, bucket, dep)
-                dep.add(self.dependency)
+                if self.required:
+                    bucket = unit.required_dependencies
+                else:
+                    bucket = unit.optional_dependencies
+                if bucket is None:
+                    bucket = set()
+                    if self.required:
+                        unit.required_dependencies = bucket
+                    else:
+                        unit.optional_dependencies = bucket
+                bucket.add(self.dependency)
 
             def __get__(self, unit: Optional[Type[Unit]], tp: Optional[Type[Executable]] = None):
                 if self.module is not None:
                     return self.module
                 try:
-                    self.module = module = super().fget()
+                    self.module = module = self.fget()
                 except ImportError as E:
                     args = unit.optional_dependencies or (self.dependency,)
                     raise RefineryImportMissing(*args) from E
                 except Exception as E:
                     raise AttributeError(F'module import for distribution "{distribution}" failed: {E!s}')
                 else:
                     return module
```

### Comparing `binary-refinery-0.6.1/refinery/units/blockwise/__init__.py` & `binary-refinery-0.6.2/refinery/units/blockwise/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/blockwise/alu.py` & `binary-refinery-0.6.2/refinery/units/blockwise/alu.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/blockwise/bitrev.py` & `binary-refinery-0.6.2/refinery/units/blockwise/bitrev.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/blockwise/byteswap.py` & `binary-refinery-0.6.2/refinery/units/blockwise/byteswap.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/blockwise/map.py` & `binary-refinery-0.6.2/refinery/units/blockwise/map.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/blockwise/pack.py` & `binary-refinery-0.6.2/refinery/units/blockwise/pack.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/blockwise/rev.py` & `binary-refinery-0.6.2/refinery/units/blockwise/rev.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/blockwise/terminate.py` & `binary-refinery-0.6.2/refinery/units/blockwise/terminate.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/blockwise/xor.py` & `binary-refinery-0.6.2/refinery/units/blockwise/xor.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/compression/ap.py` & `binary-refinery-0.6.2/refinery/units/compression/ap.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/compression/blz.py` & `binary-refinery-0.6.2/refinery/units/compression/blz.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/compression/bz2.py` & `binary-refinery-0.6.2/refinery/units/compression/bz2.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/compression/decompress.py` & `binary-refinery-0.6.2/refinery/units/compression/decompress.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/compression/jcalg.py` & `binary-refinery-0.6.2/refinery/units/compression/jcalg.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/compression/lz.py` & `binary-refinery-0.6.2/refinery/units/compression/lz.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/compression/lz4.py` & `binary-refinery-0.6.2/refinery/units/compression/lz4.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/compression/lzf.py` & `binary-refinery-0.6.2/refinery/units/compression/lzf.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/compression/lzg.py` & `binary-refinery-0.6.2/refinery/units/compression/lzg.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/compression/lzip.py` & `binary-refinery-0.6.2/refinery/units/compression/lzip.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/compression/lzjb.py` & `binary-refinery-0.6.2/refinery/units/compression/lzjb.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/compression/lznt1.py` & `binary-refinery-0.6.2/refinery/units/compression/lznt1.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/compression/lzo.py` & `binary-refinery-0.6.2/refinery/units/compression/lzo.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/compression/mscf.py` & `binary-refinery-0.6.2/refinery/units/compression/mscf.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/compression/qlz.py` & `binary-refinery-0.6.2/refinery/units/compression/qlz.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/compression/szdd.py` & `binary-refinery-0.6.2/refinery/units/compression/szdd.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/compression/zl.py` & `binary-refinery-0.6.2/refinery/units/compression/zl.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/crypto/cipher/__init__.py` & `binary-refinery-0.6.2/refinery/units/crypto/cipher/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/crypto/cipher/camellia.py` & `binary-refinery-0.6.2/refinery/units/crypto/cipher/camellia.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/crypto/cipher/chacha.py` & `binary-refinery-0.6.2/refinery/units/crypto/cipher/chacha.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/crypto/cipher/gost.py` & `binary-refinery-0.6.2/refinery/units/crypto/cipher/gost.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/crypto/cipher/hc128.py` & `binary-refinery-0.6.2/refinery/units/crypto/cipher/hc128.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/crypto/cipher/isaac.py` & `binary-refinery-0.6.2/refinery/units/crypto/cipher/isaac.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/crypto/cipher/rabbit.py` & `binary-refinery-0.6.2/refinery/units/crypto/cipher/rabbit.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/crypto/cipher/rc2.py` & `binary-refinery-0.6.2/refinery/units/crypto/cipher/rc2.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/crypto/cipher/rc4mod.py` & `binary-refinery-0.6.2/refinery/units/crypto/cipher/rc4mod.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/crypto/cipher/rc5.py` & `binary-refinery-0.6.2/refinery/units/crypto/cipher/rc5.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/crypto/cipher/rc6.py` & `binary-refinery-0.6.2/refinery/units/crypto/cipher/rc6.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/crypto/cipher/rijndael.py` & `binary-refinery-0.6.2/refinery/units/crypto/cipher/rijndael.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/crypto/cipher/rncrypt.py` & `binary-refinery-0.6.2/refinery/units/crypto/cipher/rncrypt.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/crypto/cipher/rot.py` & `binary-refinery-0.6.2/refinery/units/crypto/cipher/rot.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/crypto/cipher/rsa.py` & `binary-refinery-0.6.2/refinery/units/crypto/cipher/rsa.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/crypto/cipher/rsakey.py` & `binary-refinery-0.6.2/refinery/units/crypto/cipher/rsakey.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/crypto/cipher/salsa.py` & `binary-refinery-0.6.2/refinery/units/crypto/cipher/salsa.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/crypto/cipher/seal.py` & `binary-refinery-0.6.2/refinery/units/crypto/cipher/seal.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/crypto/cipher/secstr.py` & `binary-refinery-0.6.2/refinery/units/crypto/cipher/secstr.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/crypto/cipher/serpent.py` & `binary-refinery-0.6.2/refinery/units/crypto/cipher/serpent.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/crypto/cipher/tea.py` & `binary-refinery-0.6.2/refinery/units/crypto/cipher/tea.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/crypto/cipher/vigenere.py` & `binary-refinery-0.6.2/refinery/units/crypto/cipher/vigenere.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/crypto/cipher/xtea.py` & `binary-refinery-0.6.2/refinery/units/crypto/cipher/xtea.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/crypto/cipher/xxtea.py` & `binary-refinery-0.6.2/refinery/units/crypto/cipher/xxtea.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/crypto/hash/__init__.py` & `binary-refinery-0.6.2/refinery/units/crypto/hash/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/crypto/hash/checksums.py` & `binary-refinery-0.6.2/refinery/units/crypto/hash/checksums.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/crypto/hash/cryptographic.py` & `binary-refinery-0.6.2/refinery/units/crypto/hash/cryptographic.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/crypto/hash/imphash.py` & `binary-refinery-0.6.2/refinery/units/crypto/hash/imphash.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/crypto/hash/murmur.py` & `binary-refinery-0.6.2/refinery/units/crypto/hash/murmur.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/crypto/hash/xxhash.py` & `binary-refinery-0.6.2/refinery/units/crypto/hash/xxhash.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/crypto/keyderive/CryptDeriveKey.py` & `binary-refinery-0.6.2/refinery/units/crypto/keyderive/CryptDeriveKey.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/crypto/keyderive/DESDerive.py` & `binary-refinery-0.6.2/refinery/units/crypto/keyderive/DESDerive.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/crypto/keyderive/PasswordDeriveBytes.py` & `binary-refinery-0.6.2/refinery/units/crypto/keyderive/PasswordDeriveBytes.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/crypto/keyderive/__init__.py` & `binary-refinery-0.6.2/refinery/units/crypto/keyderive/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/crypto/keyderive/kblob.py` & `binary-refinery-0.6.2/refinery/units/crypto/keyderive/kblob.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/crypto/keyderive/pbkdf1.py` & `binary-refinery-0.6.2/refinery/units/crypto/keyderive/pbkdf1.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/crypto/keyderive/pbkdf2.py` & `binary-refinery-0.6.2/refinery/units/crypto/keyderive/pbkdf2.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/crypto/keyderive/unixcrypt.py` & `binary-refinery-0.6.2/refinery/units/crypto/keyderive/unixcrypt.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/encoding/atbash.py` & `binary-refinery-0.6.2/refinery/units/encoding/atbash.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/encoding/b32.py` & `binary-refinery-0.6.2/refinery/units/encoding/b32.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/encoding/b64.py` & `binary-refinery-0.6.2/refinery/units/encoding/b64.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/encoding/base.py` & `binary-refinery-0.6.2/refinery/units/encoding/base.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/encoding/esc.py` & `binary-refinery-0.6.2/refinery/units/encoding/esc.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/encoding/hex.py` & `binary-refinery-0.6.2/refinery/units/encoding/hex.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/encoding/netbios.py` & `binary-refinery-0.6.2/refinery/units/encoding/netbios.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/encoding/ps1str.py` & `binary-refinery-0.6.2/refinery/units/encoding/ps1str.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/encoding/recode.py` & `binary-refinery-0.6.2/refinery/units/encoding/recode.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/encoding/url.py` & `binary-refinery-0.6.2/refinery/units/encoding/url.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/encoding/uuenc.py` & `binary-refinery-0.6.2/refinery/units/encoding/uuenc.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/encoding/wshenc.py` & `binary-refinery-0.6.2/refinery/units/encoding/wshenc.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/formats/__init__.py` & `binary-refinery-0.6.2/refinery/units/formats/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/formats/a3x.py` & `binary-refinery-0.6.2/refinery/units/formats/a3x.py`

 * *Files 2% similar despite different names*

```diff
@@ -468,27 +468,27 @@
     'WinWait',
     'WinWaitActive',
     'WinWaitClose',
     'WinWaitNotActive',
 ]
 
 A3X_OPCODES = {
-    0x00: '{k}',
-    0x01: '{a}',
-    0x05: '{i}',
-    0x10: '{q}',
-    0x20: '{d}',
-    0x30: '{s}',
-    0x31: '{s}',
-    0x32: '@{s}',
-    0x33: '${s}',
-    0x34: '{s}',
-    0x35: '.{s}',
-    0x36: '{r}',
-    0x37: '{s}',
+    0x00: R'{k}',  # KEYWORD
+    0x01: R'{a}',  # API
+    0x05: R'{i}',  # INT
+    0x10: R'{q}',  # INT64
+    0x20: R'{d}',  # DOUBLE
+    0x30: R'{s}',  # CONSTRUCT
+    0x31: R'{s}',  # COMMAND
+    0x32: '@{s}',  # MACRO
+    0x33: '${s}',  # VAR
+    0x34: R'{s}',  # FUNC
+    0x35: '.{s}',  # OBJECT
+    0x36: R'{r}',  # STRING
+    0x37: R'{s}',  # DIRECTIVE
     0x40: ',',
     0x41: '=',
     0x42: '>',
     0x43: '<',
     0x44: '<>',
     0x45: '>=',
     0x46: '<=',
```

### Comparing `binary-refinery-0.6.1/refinery/units/formats/archive/__init__.py` & `binary-refinery-0.6.2/refinery/units/formats/archive/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/formats/archive/xt.py` & `binary-refinery-0.6.2/refinery/units/formats/archive/xt.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/formats/archive/xt7z.py` & `binary-refinery-0.6.2/refinery/units/formats/archive/xt7z.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/formats/archive/xtace.py` & `binary-refinery-0.6.2/refinery/units/formats/archive/xtace.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/formats/archive/xtasar.py` & `binary-refinery-0.6.2/refinery/units/formats/archive/xtasar.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/formats/archive/xtcab.py` & `binary-refinery-0.6.2/refinery/units/formats/archive/xtcab.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/formats/archive/xtcpio.py` & `binary-refinery-0.6.2/refinery/units/formats/archive/xtcpio.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/formats/archive/xtiso.py` & `binary-refinery-0.6.2/refinery/units/formats/archive/xtiso.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/formats/archive/xtiss.py` & `binary-refinery-0.6.2/refinery/units/formats/archive/xtiss.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/formats/archive/xtnsis.py` & `binary-refinery-0.6.2/refinery/units/formats/archive/xtnsis.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/formats/archive/xtpyi.py` & `binary-refinery-0.6.2/refinery/units/formats/archive/xtpyi.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/formats/archive/xttar.py` & `binary-refinery-0.6.2/refinery/units/formats/archive/xttar.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/formats/archive/xtzip.py` & `binary-refinery-0.6.2/refinery/units/formats/archive/xtzip.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/formats/bat.py` & `binary-refinery-0.6.2/refinery/units/formats/bat.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/formats/csv.py` & `binary-refinery-0.6.2/refinery/units/formats/csv.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/formats/deserialize_php.py` & `binary-refinery-0.6.2/refinery/units/formats/deserialize_php.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/formats/email.py` & `binary-refinery-0.6.2/refinery/units/formats/email.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/formats/evtx.py` & `binary-refinery-0.6.2/refinery/units/formats/evtx.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/formats/exe/vaddr.py` & `binary-refinery-0.6.2/refinery/units/formats/exe/vaddr.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/formats/exe/vmemref.py` & `binary-refinery-0.6.2/refinery/units/formats/exe/vmemref.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/formats/exe/vsect.py` & `binary-refinery-0.6.2/refinery/units/formats/exe/vsect.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/formats/exe/vsnip.py` & `binary-refinery-0.6.2/refinery/units/formats/exe/vsnip.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/formats/exe/vstack.py` & `binary-refinery-0.6.2/refinery/units/formats/exe/vstack.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/formats/hexload.py` & `binary-refinery-0.6.2/refinery/units/formats/hexload.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/formats/html.py` & `binary-refinery-0.6.2/refinery/units/formats/html.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/formats/httpresponse.py` & `binary-refinery-0.6.2/refinery/units/formats/httpresponse.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/formats/ifps.py` & `binary-refinery-0.6.2/refinery/units/formats/ifps.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/formats/ifpsstr.py` & `binary-refinery-0.6.2/refinery/units/formats/ifpsstr.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/formats/java/deserialize.py` & `binary-refinery-0.6.2/refinery/units/formats/java/deserialize.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/formats/java/jvdasm.py` & `binary-refinery-0.6.2/refinery/units/formats/java/jvdasm.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/formats/json.py` & `binary-refinery-0.6.2/refinery/units/formats/json.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/formats/lnk.py` & `binary-refinery-0.6.2/refinery/units/formats/lnk.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/formats/msgpack.py` & `binary-refinery-0.6.2/refinery/units/formats/msgpack.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/formats/office/doctxt.py` & `binary-refinery-0.6.2/refinery/units/formats/office/doctxt.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/formats/office/officecrypt.py` & `binary-refinery-0.6.2/refinery/units/formats/office/officecrypt.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/formats/office/vbapc.py` & `binary-refinery-0.6.2/refinery/units/formats/office/vbapc.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/formats/office/vbastr.py` & `binary-refinery-0.6.2/refinery/units/formats/office/vbastr.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/formats/office/xlmdeobf.py` & `binary-refinery-0.6.2/refinery/units/formats/office/xlmdeobf.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/formats/office/xlxtr.py` & `binary-refinery-0.6.2/refinery/units/formats/office/xlxtr.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/formats/office/xtdoc.py` & `binary-refinery-0.6.2/refinery/units/formats/office/xtdoc.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/formats/office/xtone.py` & `binary-refinery-0.6.2/refinery/units/formats/office/xtone.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/formats/office/xtrtf.py` & `binary-refinery-0.6.2/refinery/units/formats/office/xtrtf.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/formats/office/xtvba.py` & `binary-refinery-0.6.2/refinery/units/formats/office/xtvba.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/formats/pcap.py` & `binary-refinery-0.6.2/refinery/units/formats/pcap.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/formats/pcap_http.py` & `binary-refinery-0.6.2/refinery/units/formats/pcap_http.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         def lookup(src, dst):
             for k, request in enumerate(requests):
                 if request.src == dst and request.dst == src:
                     requests.pop(k)
                     return self.labelled(data, url=request.url)
             return None
 
-        for stream in self.pcap.process(data):
+        for stream in data | pcap:
             try:
                 data = http_parser.process(stream)
             except Exception:
                 with suppress(Exception):
                     rq = _parse_http_request(stream)
                     requests.append(rq)
                 continue
```

### Comparing `binary-refinery-0.6.1/refinery/units/formats/pdf.py` & `binary-refinery-0.6.2/refinery/units/formats/pdf.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/formats/pe/__init__.py` & `binary-refinery-0.6.2/refinery/units/formats/pe/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/formats/pe/dotnet/__init__.py` & `binary-refinery-0.6.2/refinery/units/formats/pe/dotnet/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/formats/pe/dotnet/dncfx.py` & `binary-refinery-0.6.2/refinery/units/formats/pe/dotnet/dncfx.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/formats/pe/dotnet/dnds.py` & `binary-refinery-0.6.2/refinery/units/formats/pe/dotnet/dnds.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/formats/pe/dotnet/dnfields.py` & `binary-refinery-0.6.2/refinery/units/formats/pe/dotnet/dnfields.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/formats/pe/dotnet/dnhdr.py` & `binary-refinery-0.6.2/refinery/units/formats/pe/dotnet/dnhdr.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/formats/pe/dotnet/dnmr.py` & `binary-refinery-0.6.2/refinery/units/formats/pe/dotnet/dnmr.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/formats/pe/dotnet/dnrc.py` & `binary-refinery-0.6.2/refinery/units/formats/pe/dotnet/dnrc.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/formats/pe/dotnet/dnstr.py` & `binary-refinery-0.6.2/refinery/units/formats/pe/dotnet/dnstr.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/formats/pe/pemeta.py` & `binary-refinery-0.6.2/refinery/units/formats/pe/pemeta.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/formats/pe/peoverlay.py` & `binary-refinery-0.6.2/refinery/units/formats/pe/peoverlay.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/formats/pe/perc.py` & `binary-refinery-0.6.2/refinery/units/formats/pe/perc.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/formats/pe/pesig.py` & `binary-refinery-0.6.2/refinery/units/formats/pe/pesig.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/formats/pe/pestrip.py` & `binary-refinery-0.6.2/refinery/units/formats/pe/pestrip.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/formats/pkcs7.py` & `binary-refinery-0.6.2/refinery/units/formats/pkcs7.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/formats/pkcs7sig.py` & `binary-refinery-0.6.2/refinery/units/formats/pkcs7sig.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/formats/stego.py` & `binary-refinery-0.6.2/refinery/units/formats/stego.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/formats/winreg.py` & `binary-refinery-0.6.2/refinery/units/formats/winreg.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/formats/xml.py` & `binary-refinery-0.6.2/refinery/units/formats/xml.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/malware/n40.py` & `binary-refinery-0.6.2/refinery/units/malware/n40.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/meta/__init__.py` & `binary-refinery-0.6.2/refinery/units/meta/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/meta/chop.py` & `binary-refinery-0.6.2/refinery/units/meta/chop.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/meta/cm.py` & `binary-refinery-0.6.2/refinery/units/meta/cm.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/meta/cull.py` & `binary-refinery-0.6.2/refinery/units/meta/cull.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/meta/dedup.py` & `binary-refinery-0.6.2/refinery/units/meta/dedup.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/meta/eat.py` & `binary-refinery-0.6.2/refinery/units/meta/eat.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/meta/ef.py` & `binary-refinery-0.6.2/refinery/units/meta/ef.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/meta/emit.py` & `binary-refinery-0.6.2/refinery/units/meta/emit.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/meta/group.py` & `binary-refinery-0.6.2/refinery/units/meta/group.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/meta/groupby.py` & `binary-refinery-0.6.2/refinery/units/meta/groupby.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/meta/iff.py` & `binary-refinery-0.6.2/refinery/units/meta/iff.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/meta/iffp.py` & `binary-refinery-0.6.2/refinery/units/meta/iffp.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/meta/iffs.py` & `binary-refinery-0.6.2/refinery/units/meta/iffs.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/meta/iffx.py` & `binary-refinery-0.6.2/refinery/units/meta/iffx.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/meta/max.py` & `binary-refinery-0.6.2/refinery/units/meta/max.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/meta/min.py` & `binary-refinery-0.6.2/refinery/units/meta/min.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/meta/mvc.py` & `binary-refinery-0.6.2/refinery/units/meta/mvc.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/meta/mvg.py` & `binary-refinery-0.6.2/refinery/units/meta/mvg.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/meta/pad.py` & `binary-refinery-0.6.2/refinery/units/meta/pad.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/meta/pick.py` & `binary-refinery-0.6.2/refinery/units/meta/pick.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/meta/pop.py` & `binary-refinery-0.6.2/refinery/units/meta/pop.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/meta/push.py` & `binary-refinery-0.6.2/refinery/units/meta/push.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/meta/put.py` & `binary-refinery-0.6.2/refinery/units/meta/put.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/meta/queue.py` & `binary-refinery-0.6.2/refinery/units/meta/queue.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/meta/reduce.py` & `binary-refinery-0.6.2/refinery/units/meta/reduce.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/meta/scope.py` & `binary-refinery-0.6.2/refinery/units/meta/scope.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/meta/sep.py` & `binary-refinery-0.6.2/refinery/units/meta/sep.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/meta/sorted.py` & `binary-refinery-0.6.2/refinery/units/meta/sorted.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/meta/swap.py` & `binary-refinery-0.6.2/refinery/units/meta/swap.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/meta/xfcc.py` & `binary-refinery-0.6.2/refinery/units/meta/xfcc.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/misc/autoxor.py` & `binary-refinery-0.6.2/refinery/units/misc/autoxor.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/misc/couple.py` & `binary-refinery-0.6.2/refinery/units/misc/couple.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/misc/datefix.py` & `binary-refinery-0.6.2/refinery/units/misc/datefix.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/misc/drp.py` & `binary-refinery-0.6.2/refinery/units/misc/drp.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/misc/nop.py` & `binary-refinery-0.6.2/refinery/units/misc/nop.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/misc/urlfix.py` & `binary-refinery-0.6.2/refinery/units/misc/urlfix.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/misc/xkey.py` & `binary-refinery-0.6.2/refinery/units/misc/xkey.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/obfuscation/__init__.py` & `binary-refinery-0.6.2/refinery/units/obfuscation/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/obfuscation/js/arrays.py` & `binary-refinery-0.6.2/refinery/units/obfuscation/js/arrays.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/obfuscation/js/getattr.py` & `binary-refinery-0.6.2/refinery/units/obfuscation/js/getattr.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/obfuscation/js/tuples.py` & `binary-refinery-0.6.2/refinery/units/obfuscation/js/tuples.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/obfuscation/ps1/__init__.py` & `binary-refinery-0.6.2/refinery/units/obfuscation/ps1/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/obfuscation/ps1/all.py` & `binary-refinery-0.6.2/refinery/units/obfuscation/ps1/all.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/obfuscation/ps1/brackets.py` & `binary-refinery-0.6.2/refinery/units/obfuscation/ps1/brackets.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/obfuscation/ps1/cases.py` & `binary-refinery-0.6.2/refinery/units/obfuscation/ps1/cases.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/obfuscation/ps1/concat.py` & `binary-refinery-0.6.2/refinery/units/obfuscation/ps1/concat.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/obfuscation/ps1/format.py` & `binary-refinery-0.6.2/refinery/units/obfuscation/ps1/format.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/obfuscation/ps1/invoke.py` & `binary-refinery-0.6.2/refinery/units/obfuscation/ps1/invoke.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/obfuscation/ps1/securestring.py` & `binary-refinery-0.6.2/refinery/units/obfuscation/ps1/securestring.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/obfuscation/ps1/stringreplace.py` & `binary-refinery-0.6.2/refinery/units/obfuscation/ps1/stringreplace.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/obfuscation/ps1/typecast.py` & `binary-refinery-0.6.2/refinery/units/obfuscation/ps1/typecast.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/obfuscation/ps1/uncurly.py` & `binary-refinery-0.6.2/refinery/units/obfuscation/ps1/uncurly.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/obfuscation/vba/all.py` & `binary-refinery-0.6.2/refinery/units/obfuscation/vba/all.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/obfuscation/vba/arithmetic.py` & `binary-refinery-0.6.2/refinery/units/obfuscation/vba/arithmetic.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/obfuscation/vba/brackets.py` & `binary-refinery-0.6.2/refinery/units/obfuscation/vba/brackets.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/obfuscation/vba/char.py` & `binary-refinery-0.6.2/refinery/units/obfuscation/vba/char.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/obfuscation/vba/concat.py` & `binary-refinery-0.6.2/refinery/units/obfuscation/vba/concat.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/obfuscation/vba/constants.py` & `binary-refinery-0.6.2/refinery/units/obfuscation/vba/constants.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/obfuscation/vba/dummies.py` & `binary-refinery-0.6.2/refinery/units/obfuscation/vba/dummies.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/obfuscation/vba/stringreplace.py` & `binary-refinery-0.6.2/refinery/units/obfuscation/vba/stringreplace.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/obfuscation/vba/stringreverse.py` & `binary-refinery-0.6.2/refinery/units/obfuscation/vba/stringreverse.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/pattern/__init__.py` & `binary-refinery-0.6.2/refinery/units/pattern/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/pattern/carve.py` & `binary-refinery-0.6.2/refinery/units/pattern/carve.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/pattern/carve_7z.py` & `binary-refinery-0.6.2/refinery/units/pattern/carve_7z.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/pattern/carve_json.py` & `binary-refinery-0.6.2/refinery/units/pattern/carve_json.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/pattern/carve_lnk.py` & `binary-refinery-0.6.2/refinery/units/pattern/carve_lnk.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/pattern/carve_pe.py` & `binary-refinery-0.6.2/refinery/units/pattern/carve_pe.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/pattern/carve_rtf.py` & `binary-refinery-0.6.2/refinery/units/pattern/carve_rtf.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/pattern/carve_xml.py` & `binary-refinery-0.6.2/refinery/units/pattern/carve_xml.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/pattern/carve_zip.py` & `binary-refinery-0.6.2/refinery/units/pattern/carve_zip.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/pattern/defang.py` & `binary-refinery-0.6.2/refinery/units/pattern/defang.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/pattern/dnsdomain.py` & `binary-refinery-0.6.2/refinery/units/pattern/dnsdomain.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/pattern/mimewords.py` & `binary-refinery-0.6.2/refinery/units/pattern/mimewords.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/pattern/resplit.py` & `binary-refinery-0.6.2/refinery/units/pattern/resplit.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/pattern/resub.py` & `binary-refinery-0.6.2/refinery/units/pattern/resub.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/pattern/rex.py` & `binary-refinery-0.6.2/refinery/units/pattern/rex.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/pattern/struct_parser.py` & `binary-refinery-0.6.2/refinery/units/pattern/struct_parser.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/pattern/subfiles.py` & `binary-refinery-0.6.2/refinery/units/pattern/subfiles.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/pattern/urlguards.py` & `binary-refinery-0.6.2/refinery/units/pattern/urlguards.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/pattern/xtp.py` & `binary-refinery-0.6.2/refinery/units/pattern/xtp.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/pattern/xtw.py` & `binary-refinery-0.6.2/refinery/units/pattern/xtw.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/sinks/__init__.py` & `binary-refinery-0.6.2/refinery/units/sinks/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/sinks/asm.py` & `binary-refinery-0.6.2/refinery/units/sinks/asm.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/sinks/dump.py` & `binary-refinery-0.6.2/refinery/units/sinks/dump.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/sinks/iemap.py` & `binary-refinery-0.6.2/refinery/units/sinks/iemap.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/sinks/peek.py` & `binary-refinery-0.6.2/refinery/units/sinks/peek.py`

 * *Files 2% similar despite different names*

```diff
@@ -268,15 +268,18 @@
                     brief = F'#{index:03d}: {brief}'
                 yield brief
 
         if final and not empty:
             yield separator()
 
     def filter(self, chunks):
-        self._colorama.init(wrap=False)
+        try:
+            self._colorama.init(wrap=False)
+        except ImportError:
+            pass
         discarded = 0
         for final, item in lookahead(chunks):
             item.temp = final
             if not item.visible and self.isatty:
                 discarded += 1
             else:
                 yield item
```

### Comparing `binary-refinery-0.6.1/refinery/units/sinks/ppjscript.py` & `binary-refinery-0.6.2/refinery/units/sinks/ppjscript.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/sinks/ppjson.py` & `binary-refinery-0.6.2/refinery/units/sinks/ppjson.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/sinks/ppxml.py` & `binary-refinery-0.6.2/refinery/units/sinks/ppxml.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/strings/cfmt.py` & `binary-refinery-0.6.2/refinery/units/strings/cfmt.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/strings/cswap.py` & `binary-refinery-0.6.2/refinery/units/strings/cswap.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/strings/rep.py` & `binary-refinery-0.6.2/refinery/units/strings/rep.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/strings/repl.py` & `binary-refinery-0.6.2/refinery/units/strings/repl.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/strings/snip.py` & `binary-refinery-0.6.2/refinery/units/strings/snip.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/strings/stretch.py` & `binary-refinery-0.6.2/refinery/units/strings/stretch.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/strings/termfit.py` & `binary-refinery-0.6.2/refinery/units/strings/termfit.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/refinery/units/strings/trim.py` & `binary-refinery-0.6.2/refinery/units/strings/trim.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.1/setup.py` & `binary-refinery-0.6.2/setup.py`

 * *Files identical despite different names*

