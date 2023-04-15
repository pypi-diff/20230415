# Comparing `tmp/unireedsolomon-1.0.5.tar.gz` & `tmp/unireedsolomon-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\unireedsolomon-1.0.5.tar", last modified: Wed Jan  6 05:49:50 2021, max compression
+gzip compressed data, was "unireedsolomon-1.0.6.tar", last modified: Sat Apr 15 01:14:53 2023, max compression
```

## Comparing `unireedsolomon-1.0.5.tar` & `unireedsolomon-1.0.6.tar`

### file list

```diff
@@ -1,29 +1,34 @@
-drwxrwxrwx   0        0        0        0 2021-01-06 05:49:50.137613 unireedsolomon-1.0.5/
--rw-rw-rw-   0        0        0     1121 2020-03-01 22:54:38.000000 unireedsolomon-1.0.5/LICENSE.txt
--rw-rw-rw-   0        0        0      213 2020-03-01 22:54:38.000000 unireedsolomon-1.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0    21600 2021-01-06 05:49:50.134622 unireedsolomon-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0    17058 2021-01-06 05:48:06.000000 unireedsolomon-1.0.5/README.rst
--rw-rw-rw-   0        0        0     1061 2020-03-01 22:54:38.000000 unireedsolomon-1.0.5/notes.txt
--rw-rw-rw-   0        0        0       42 2021-01-06 05:49:50.138610 unireedsolomon-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0     4544 2021-01-06 03:25:06.000000 unireedsolomon-1.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2021-01-06 05:49:50.087747 unireedsolomon-1.0.5/unireedsolomon/
--rw-rw-rw-   0        0        0       77 2020-03-01 22:54:38.000000 unireedsolomon-1.0.5/unireedsolomon/__init__.py
--rw-rw-rw-   0        0        0      466 2020-03-01 22:54:38.000000 unireedsolomon-1.0.5/unireedsolomon/_compat.py
--rw-rw-rw-   0        0        0    24980 2020-03-01 22:54:38.000000 unireedsolomon-1.0.5/unireedsolomon/cff.pyx
--rw-rw-rw-   0        0        0    20285 2020-03-01 22:54:38.000000 unireedsolomon-1.0.5/unireedsolomon/cpolynomial.pyx
--rw-rw-rw-   0        0        0    23474 2021-01-06 01:53:33.000000 unireedsolomon-1.0.5/unireedsolomon/ff.py
--rw-rw-rw-   0        0        0     1754 2020-03-01 22:54:38.000000 unireedsolomon-1.0.5/unireedsolomon/imageencode.py
--rw-rw-rw-   0        0        0    20578 2020-03-01 22:54:38.000000 unireedsolomon-1.0.5/unireedsolomon/polynomial.py
--rw-rw-rw-   0        0        0    68868 2020-03-01 22:54:38.000000 unireedsolomon-1.0.5/unireedsolomon/rs.py
-drwxrwxrwx   0        0        0        0 2021-01-06 05:49:50.126641 unireedsolomon-1.0.5/unireedsolomon/tests/
--rw-rw-rw-   0        0        0        1 2020-03-01 22:54:38.000000 unireedsolomon-1.0.5/unireedsolomon/tests/__init__.py
--rw-rw-rw-   0        0        0    11533 2020-03-01 22:54:38.000000 unireedsolomon-1.0.5/unireedsolomon/tests/test_cff.py
--rw-rw-rw-   0        0        0     9289 2020-03-01 22:54:38.000000 unireedsolomon-1.0.5/unireedsolomon/tests/test_cpolynomial.py
--rw-rw-rw-   0        0        0    10773 2020-03-01 22:54:38.000000 unireedsolomon-1.0.5/unireedsolomon/tests/test_ff.py
--rw-rw-rw-   0        0        0     8085 2020-03-01 22:54:38.000000 unireedsolomon-1.0.5/unireedsolomon/tests/test_polynomial.py
--rw-rw-rw-   0        0        0    22003 2020-03-01 22:54:38.000000 unireedsolomon-1.0.5/unireedsolomon/tests/test_rs.py
-drwxrwxrwx   0        0        0        0 2021-01-06 05:49:50.102706 unireedsolomon-1.0.5/unireedsolomon.egg-info/
--rw-rw-rw-   0        0        0    21600 2021-01-06 05:49:49.000000 unireedsolomon-1.0.5/unireedsolomon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      624 2021-01-06 05:49:49.000000 unireedsolomon-1.0.5/unireedsolomon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-01-06 05:49:49.000000 unireedsolomon-1.0.5/unireedsolomon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2021-01-06 05:49:49.000000 unireedsolomon-1.0.5/unireedsolomon.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-15 01:14:53.264032 unireedsolomon-1.0.6/
+-rw-rw-rw-   0        0        0     1187 2023-04-15 00:33:07.000000 unireedsolomon-1.0.6/LICENSE.txt
+-rw-rw-rw-   0        0        0      208 2023-04-15 00:16:40.000000 unireedsolomon-1.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0    21685 2023-04-15 01:14:53.261040 unireedsolomon-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0    18981 2023-04-15 00:29:34.000000 unireedsolomon-1.0.6/README.rst
+-rw-rw-rw-   0        0        0     1061 2020-03-01 22:54:38.000000 unireedsolomon-1.0.6/notes.txt
+-rw-rw-rw-   0        0        0     8274 2023-04-15 01:14:04.000000 unireedsolomon-1.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-15 01:14:53.265030 unireedsolomon-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     3475 2023-04-15 00:42:32.000000 unireedsolomon-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 01:14:53.088136 unireedsolomon-1.0.6/src/
+drwxrwxrwx   0        0        0        0 2023-04-15 01:14:53.191227 unireedsolomon-1.0.6/src/unireedsolomon/
+-rw-rw-rw-   0        0        0       77 2023-04-15 00:16:40.000000 unireedsolomon-1.0.6/src/unireedsolomon/__init__.py
+-rw-rw-rw-   0        0        0      466 2023-04-15 00:16:40.000000 unireedsolomon-1.0.6/src/unireedsolomon/_compat.py
+-rw-rw-rw-   0        0        0  1286852 2023-04-15 01:14:52.000000 unireedsolomon-1.0.6/src/unireedsolomon/cff.c
+-rw-rw-rw-   0        0        0    25011 2023-04-15 00:32:25.000000 unireedsolomon-1.0.6/src/unireedsolomon/cff.pyx
+-rw-rw-rw-   0        0        0   591235 2023-04-15 01:14:48.000000 unireedsolomon-1.0.6/src/unireedsolomon/cpolynomial.c
+-rw-rw-rw-   0        0        0    20316 2023-04-15 00:32:21.000000 unireedsolomon-1.0.6/src/unireedsolomon/cpolynomial.pyx
+-rw-rw-rw-   0        0        0    23474 2023-04-15 00:16:40.000000 unireedsolomon-1.0.6/src/unireedsolomon/ff.py
+-rw-rw-rw-   0        0        0     1754 2023-04-15 00:16:40.000000 unireedsolomon-1.0.6/src/unireedsolomon/imageencode.py
+-rw-rw-rw-   0        0        0    20578 2023-04-15 00:16:40.000000 unireedsolomon-1.0.6/src/unireedsolomon/polynomial.py
+-rw-rw-rw-   0        0        0    68868 2023-04-15 00:16:40.000000 unireedsolomon-1.0.6/src/unireedsolomon/rs.py
+drwxrwxrwx   0        0        0        0 2023-04-15 01:14:53.255056 unireedsolomon-1.0.6/src/unireedsolomon/tests/
+-rw-rw-rw-   0        0        0        1 2023-04-15 00:16:40.000000 unireedsolomon-1.0.6/src/unireedsolomon/tests/__init__.py
+-rw-rw-rw-   0        0        0    11533 2023-04-15 00:16:40.000000 unireedsolomon-1.0.6/src/unireedsolomon/tests/test_cff.py
+-rw-rw-rw-   0        0        0     9289 2023-04-15 00:16:40.000000 unireedsolomon-1.0.6/src/unireedsolomon/tests/test_cpolynomial.py
+-rw-rw-rw-   0        0        0    10773 2023-04-15 00:16:40.000000 unireedsolomon-1.0.6/src/unireedsolomon/tests/test_ff.py
+-rw-rw-rw-   0        0        0     8085 2023-04-15 00:16:40.000000 unireedsolomon-1.0.6/src/unireedsolomon/tests/test_polynomial.py
+-rw-rw-rw-   0        0        0    22003 2023-04-15 00:16:40.000000 unireedsolomon-1.0.6/src/unireedsolomon/tests/test_rs.py
+drwxrwxrwx   0        0        0        0 2023-04-15 01:14:53.219154 unireedsolomon-1.0.6/src/unireedsolomon.egg-info/
+-rw-rw-rw-   0        0        0    21685 2023-04-15 01:14:53.000000 unireedsolomon-1.0.6/src/unireedsolomon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      810 2023-04-15 01:14:53.000000 unireedsolomon-1.0.6/src/unireedsolomon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 01:14:53.000000 unireedsolomon-1.0.6/src/unireedsolomon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      100 2023-04-15 01:14:53.000000 unireedsolomon-1.0.6/src/unireedsolomon.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-15 01:14:53.000000 unireedsolomon-1.0.6/src/unireedsolomon.egg-info/top_level.txt
```

### Comparing `unireedsolomon-1.0.5/LICENSE.txt` & `unireedsolomon-1.0.6/LICENSE.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 The MIT License (MIT)
 
 Copyright (c) 2010 Andrew Brown <brownan@cs.duke.edu, brownan@gmail.com>
+Copyright (c) 2015-2023 Stephen Karl Larroque <lrq3000@gmail.com>
 
 Permission is hereby granted, free of charge, to any person
 obtaining a copy of this software and associated documentation
 files (the "Software"), to deal in the Software without
 restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the
```

### Comparing `unireedsolomon-1.0.5/PKG-INFO` & `unireedsolomon-1.0.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,374 +1,410 @@
 Metadata-Version: 2.1
 Name: unireedsolomon
-Version: 1.0.5
-Summary: Universal errors-and-erasures Reed Solomon codec (error correcting code) in pure Python with extensive documentation
-Home-page: https://github.com/lrq3000/unireedsolomon
-Author: Andrew Brown, Stephen Larroque
-Author-email: lrq3000@gmail.com
-License: MIT
-Description: UniReedSolomon
-        ==============
-        
-        |PyPI-Status| |PyPI-Versions| |PyPI-Downloads|
-        
-        |Build-Status| |Coverage|
-        
-        UniReedSolomon is a pure-Python universal Reed-Solomon error correction codec with fully documented code and mathematical nomenclatura, compatible with Python 2.7 up to 3.8 and also PyPy 2 and 3.
-        
-        If you are just starting with Reed-Solomon error correction codes, please see the `Wikiversity tutorial <https://en.wikiversity.org/wiki/Reed%E2%80%93Solomon_codes_for_coders>`_.
-        
-        ------------------------------------
-        
-        .. contents:: Table of contents
-           :backlinks: top
-           :local:
-        
-        
-        Installation
-        ------------
-        
-        .. code:: sh
-        
-            pip install --upgrade unireedsolomon
-        
-        .. note::
-        
-            When installing from source using ``python setup.py install``, the setup.py will try to build the Cython optimized module ``cff.pyx`` and ``cpolynomial.pyx`` if both Cython and a C compiler (eg, gcc) are installed, which provides ~4x speed boost during encoding. Although it should be done by default if Cython is installed, the compilation of Cython modules can be forced with ``python setup.py build_ext --inplace``. You can override this behavior by typing: ``python setup.py install --nocython`` to force the install only the pure python module without building the Cython modules.
-        
-            Pre-transpiled ``cff.c`` and ``cpolynomial.c`` files are also available, and can be compiled with a C compiler without Cython by typing: ``python setup.py install --compile``.
-        
-        Quickstart
-        ----------
-        >>> import unireedsolomon as rs
-        >>> coder = rs.RSCoder(20,13)
-        >>> c = coder.encode("Hello, world!")
-        >>> print repr(c)
-        'Hello, world!\x8d\x13\xf4\xf9C\x10\xe5'
-        >>>
-        >>> r = "\0"*3 + c[3:]
-        >>> print repr(r)
-        '\x00\x00\x00lo, world!\x8d\x13\xf4\xf9C\x10\xe5'
-        >>>
-        >>> coder.decode(r)
-        'Hello, world!'
-        
-        Description
-        -----------
-        This library implements a pure-Python documented universal Reed-Solomon
-        error correction codec with a mathematical nomenclatura, compatible with
-        Python 2.7 up to 3.7+ and also with PyPy 2 and PyPy 3.
-        
-        The project aims to keep a well commented and organized code with
-        an extensive documentation and mathematical clarity of the various
-        arithmetic operations.
-        
-        How does this library differs from other Reed-Solomon libraries?
-        
-        * **universal**: compatibility with (almost) any other Reed-Solomon codec. This means that you can choose the parameters so that you can either encode data and decode it with another RS codec, or on the opposite encode data with another RS codec and decode this data with this library.
-        * **errors-and-erasures decoding** allows to decode both erasures (where you know the position of the corrupted characters) and errors (where you don't know where are the corrupted characters) at the same time (because you can decode more erasures than errors, so if you can provide even a few know corrupted characters positions, this can help a lot the decoder to repair the message).
-        * **documented**: following literate programming guidelines, you should understand everything you need about RS by reading the code and the comments.
-        * **mathematical nomenclatura**: for example, contrary to most other RS libraries, you will see a clear distinction between the different mathematical constructs, such as the Galois Fields numbers are clearly separated from the generic Polynomial objects, and both are separated from the Reed-Solomon algorithm, which makes use of both of those constructs. For this purpose, object-oriented programming was chosen to design the architecture of the library, although obviously at the expense of a bit of performance. However, this library favors mathematical clarity and documentation over performance (even if performance is optimized whenever possible).
-        * **pure-Python** means that there are no dependencies whatsoever apart from the Python interpreter. This means that this library should be resilient in the future (since it doesn't depend on external libraries who can become broken with time, see software rot), and you can use it on any system where Python can be installed (including online cloud services).
-        
-        The authors tried their best to extensively document the algorithms.
-        However, a lot of the math involved is non-trivial and we can't explain it all
-        in the comments. To learn more about the algorithms, see these resources:
-        
-        * `<http://en.wikipedia.org/wiki/Reedâ€“Solomon_error_correction>`_
-        * `<http://www.cs.duke.edu/courses/spring10/cps296.3/rs_scribe.pdf>`_
-        * `<http://www.cs.duke.edu/courses/spring10/cps296.3/decoding_rs_scribe.pdf>`_
-        * `<http://www.cs.cmu.edu/afs/cs.cmu.edu/project/pscico-guyb/realworld/www/reed_solomon.ps>`_
-        * `<http://www.cs.cmu.edu/afs/cs.cmu.edu/project/pscico-guyb/realworld/www/rs_decode.ps>`_
-        
-        Also, here's a copy of the presentation one of the authors gave to the class Spring 2010 on his
-        experience implementing this library. The LaTeX source is in the presentation directory.
-        
-        `<http://www.cs.duke.edu/courses/spring10/cps296.3/decoding_rs.pdf>`_
-        
-        The code was lately updated to support errors-and-erasures decoding (both at the same
-        time), and to be universal (you can supply the parameters to be compatible with almost
-        any other RS codec).
-        
-        The codec has decent performances if you use PyPy with the fast methods (~1 MB/s),
-        but it would be faster if we drop the object-oriented design (implementing everything in
-        functions), but this would be at the expense of mathematical clarity. If you are interested,
-        see the reedsolo library by Tomer Filiba, which is exactly the same implementation but
-        only functional without objects (results in about 5x speedup).
-        
-        Files
-        -----
-        rs.py
-            Holds the Reed-Solomon Encoder/Decoder object
-        
-        polynomial.py
-            Contains the Polynomial object (pure-python)
-        
-        ff.py
-            Contains the GF2int object representing an element of the GF(2^p) field, with p being 8 by default (pure-python)
-        
-        polynomial.pyx
-            Cython implementation of polynomial.py with equivalent functions (optional)
-        
-        ff.pyx
-            Cython implementation of ff.py with equivalent functions (optional)
-        
-        Documentation
-        -------------
-        unireedsolomon.rs.RSCoder(n, k, generator=3, prim=0x11b, fcr=1, c_exp=8)
-            Creates a new Reed-Solomon Encoder/Decoder object configured with
-            the given n and k values.
-            n is the length of a codeword, must be less than 256
-            k is the length of the message, must be less than n
-            generator, prim and fcr parametrize the Galois Field that will be built
-            c_exp is the Galois Field range (ie, 8 means GF(2^8) = GF(256)), which is both the limit for one symbol's value, and the maximum length of a message+ecc.
-        
-            The code will have error correcting power (ie, maximum number of repairable symbols) of `2*e+v <= (n-k)`, where e is the number of errors and v the number of erasures.
-        
-            The typical RSCoder is RSCoder(255, 223)
-        
-        RSCoder.encode(message, poly=False, k=None)
-            Encode a given string with reed-solomon encoding. Returns a byte
-            string with the k message bytes and n-k parity bytes at the end.
-        
-            If a message is < k bytes long, it is assumed to be padded at the front
-            with null bytes (ie, a shortened Reed-Solomon code).
-        
-            The sequence returned is always n bytes long.
-        
-            If poly is not False, returns the encoded Polynomial object instead of
-            the polynomial translated back to a string (useful for debugging)
-        
-            You can change the length (number) of parity/ecc bytes at encoding
-            by setting k to any value between [1, n-1]. This allows to create only
-            one RSCoder and then use it with a variable redundancy rate.
-        
-        RSCoder.encode_fast(message, poly=False, k=None)
-            Same as encode() but using faster algorithms and optimization tricks.
-        
-        RSCoder.decode(message_ecc, nostrip=False, k=None, erasures_pos=None, only_erasures=False):
-            Given a received string or byte array message_ecc (composed of
-            a message string + ecc symbols at the end), attempts to decode it.
-            If it's a valid codeword, or if there are no more than `2*e+v <= (n-k)` erratas
-            (called the Singleton bound), the message is returned.
-        
-            You can provide the erasures positions as a list to erasures_pos.
-            For example, if you have "hella warld" and you know that `a` is an erasure,
-            you can provide the list erasures_pos=[4, 7]. You can correct twice as many
-            erasures than errors, and if some provided erasures are wrong (they are correct
-            symbols), then there's no problem, they will be repaired just fine (but will count
-            towards the Singleton bound). You can also specify that you are sure there are
-            only erasures and no errors at all by setting only_erasures=True.
-        
-            A message always has k bytes, if a message contained less it is left
-            padded with null bytes (punctured RS code). When decoded, these leading
-            null bytes are stripped, but that can cause problems if decoding binary data.
-            When nostrip is True, messages returned are always k bytes long. This is
-            useful to make sure no data is lost when decoding binary data.
-        
-            Note that RS can correct errors both in the message and the ecc symbols.
-        
-        RSCoder.decode_fast(message_ecc, nostrip=False, k=None, erasures_pos=None, only_erasures=False):
-            Same as decode() but using faster algorithms and optimization tricks.
-        
-        RSCoder.check(message_ecc, k=None)
-            Verifies the codeword (message + ecc symbols at the end) is valid by testing
-            that the code as a polynomial code divides g, or that the syndrome is
-            all 0 coefficients. The result is not foolproof: if it's False, you're sure the
-            message was corrupted (or that you used the wrong RS parameters),
-            but if it's True, it's either that the message is correct, or that there are
-            too many errors (ie, more than the Singleton bound) for RS to do anything about it.
-            returns True/False
-        
-        RSCoder.check_fast(message_ecc, k=None)
-            Same as check() but using faster algorithms and optimization tricks.
-        
-        unireedsolomon.ff.find_prime_polynomials(generator=2, c_exp=8, fast_primes=False, single=False)
-            Compute the list of prime polynomials for the given generator and
-            galois field characteristic exponent. You can then use this prime polynomial
-            to specify the mandatory "prim" parameter, particularly if you are using
-            a larger Galois Field (eg, 2^16).
-        
-        
-        Internal API
-        -------------
-        Besides the main RSCoder object, two other objects are used in this
-        implementation: Polynomial and GF2int. Their use is not specifically tied
-        to the coder or even to the Reed-Solomon algorithm, they are just generic
-        mathematical constructs respectively representing polynomials and
-        Galois field's number of base 2.
-        
-        You do not need to know about the internal API to use the RS codec,
-        this is just left as a documentation for the reader interested into dwelling
-        inside the mathematical constructs.
-        
-        polynomial.Polynomial(coefficients=[], \**sparse)
-            There are three ways to initialize a Polynomial object.
-            1) With a list, tuple, or other iterable, creates a polynomial using
-            the items as coefficients in order of decreasing power
-        
-            2) With keyword arguments such as for example x3=5, sets the
-            coefficient of x^3 to be 5
-        
-            3) With no arguments, creates an empty polynomial, equivalent to
-            Polynomial([0])
-        
-            >>> print Polynomial([5, 0, 0, 0, 0, 0])
-            5x^5
-        
-            >>> print Polynomial(x32=5, x64=8)
-            8x^64 + 5x^32
-        
-            >>> print Polynomial(x5=5, x9=4, x0=2) 
-            4x^9 + 5x^5 + 2
-        
-        Polynomial objects export the following standard functions that perform the
-        expected operations using polynomial arithmetic. Arithmetic of the coefficients
-        is determined by the type passed in, so integers or GF2int objects could be
-        used, the Polynomial class is agnostic to the type of the coefficients.
-        
-        ::
-        
-            __add__
-            __divmod__
-            __eq__
-            __floordiv__
-            __hash__
-            __len__
-            __mod__
-            __mul__
-            __ne__
-            __neg__
-            __sub__
-            evaluate(x)
-            degree()
-                Returns the degree of the polynomial
-            get_coefficient(degree)
-                Returns the coefficient of the specified term
-        
-        ff.GF2int(value)
-            Instances of this object are elements of the field GF(2^p) and instances are integers
-            in the range 0 to `(2^p)-1`.
-            By default, the field is GF(2^8) and instances are integers in the range 0 to 255
-            and is defined using the irreducable polynomial 0x11b or in binary form:
-            x^8 + x^4 + x^3 + x + 1
-            and using 3 as the generator for the exponent table and log table.
-            
-            You can however use other parameters for the Galois Field, using the
-            init_lut() function.
-        
-        ff.find_prime_polynomials(generator=2, c_exp=8, fast_primes=False, single=False)
-            Find the list of prime polynomials to use to generate the look-up tables
-            for your field.
-        
-        ff.init_lut(generator=3, prim=0x11b, c_exp=8)
-            Generate the look-up tables given the parameters. This effectively parametrize
-            your Galois Field (ie, generator=2, prim=0x1002d, c_exp=16) will generate
-            a GF(2^16) field.
-        
-        The GF2int class inherits from int and supports all the usual integer
-        operations. The following methods are overridden for arithmetic in the finite
-        field GF(2^p)
-        
-        ::
-        
-            __add__
-            __div__
-            __mul__
-            __neg__
-            __pow__
-            __radd__
-            __rdiv__
-            __rmul__
-            __rsub__
-            __sub__
-            inverse()
-                Multiplicative inverse in GF(2^p)
-        
-        Example implementations
-        -----------------------
-        
-        Image Encoder
-        ~~~~~~~~~~~~~
-        imageencode.py is an example script that encodes codewords as rows in an image.
-        It requires PIL to run.
-        
-        Usage: python imageencode.py [-d] <image file>
-        
-        Without the -d flag, imageencode.py will encode text from standard in and
-        output it to the image file. With -d, imageencode.py will read in the data from
-        the image and output to standard out the decoded text.
-        
-        An example is included: ``exampleimage.png``. Try decoding it as-is, then open
-        it up in an image editor and paint some vertical stripes on it. As long as no
-        more than 16 pixels per row are disturbed, the text will be decoded correctly.
-        Then draw more stripes such that more than 16 pixels per row are disturbed and
-        verify that the message is decoded improperly.
-        
-        Notice how the parity data looks different--the last 32 pixels of each row are
-        colored differently. That's because this particular image contains encoded
-        ASCII text, which generally only has bytes from a small range (the alphabet and
-        printable punctuation). The parity data, however, is binary and contains bytes
-        from the full range 0-255. Also note that either the data area or the parity
-        area (or both!) can be disturbed as long as no more than 16 bytes per row are
-        disturbed.
-        
-        Cython implementation
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        If either a C compiler or Cython is found, rs.py will automatically load the Cython implementations
-        (the \*.pyx files).
-        These are provided as optimized versions of the pure-python implementations, with equivalent
-        functionalities. The goal was to get a speedup, which is the case, but using PyPy on the pure-python
-        implementation provides a significantly higher speedup than the Cython implementation.
-        The Cython implementations are still provided for the interested reader, but the casual user is
-        not advised to use them. If you want to encode and decode fast, use PyPy.
-        
-        Recommended reading
-        -------------------
-        
-        * "`Reed-Solomon codes for coders <https://en.wikiversity.org/wiki/Reed%E2%80%93Solomon_codes_for_coders>`_", free practical beginner's tutorial with Python code examples on WikiVersity. Partially written by one of the authors of the present software.
-        * "Algebraic codes for data transmission", Blahut, Richard E., 2003, Cambridge university press. `Readable online on Google Books <https://books.google.fr/books?id=eQs2i-R9-oYC&lpg=PR11&ots=atCPQJm3OJ&dq=%22Algebraic%20codes%20for%20data%20transmission%22%2C%20Blahut%2C%20Richard%20E.%2C%202003%2C%20Cambridge%20university%20press.&lr&hl=fr&pg=PA193#v=onepage&q=%22Algebraic%20codes%20for%20data%20transmission%22,%20Blahut,%20Richard%20E.,%202003,%20Cambridge%20university%20press.&f=false>`_. This book was pivotal in helping to understand the intricacies of the universal Berlekamp-Massey algorithm (see figures 7.5 and 7.10).
-        
-        Authors and licence
-        -------------------
-        Written from scratch by Andrew Brown <brownan@gmail.com> <brownan@cs.duke.edu>
-        (c) 2010.
-        
-        Upgraded and maintained by Stephen Karl Larroque <LRQ3000@gmail.com> in 2015-2020.
-        
-        Licensed under the MIT License.
-        
-        
-        .. |PyPI-Status| image:: https://img.shields.io/pypi/v/unireedsolomon.svg
-           :target: https://pypi.org/project/unireedsolomon
-        .. |PyPI-Versions| image:: https://img.shields.io/pypi/pyversions/unireedsolomon.svg?logo=python&logoColor=white
-           :target: https://pypi.org/project/unireedsolomon
-        .. |PyPI-Downloads| image:: https://img.shields.io/pypi/dm/unireedsolomon.svg?label=pypi%20downloads&logo=python&logoColor=white
-           :target: https://pypi.org/project/unireedsolomon
-        .. |Build-Status| image:: https://travis-ci.org/lrq3000/unireedsolomon.svg?branch=master
-            :target: https://travis-ci.org/lrq3000/unireedsolomon
-        .. |Coverage| image:: https://coveralls.io/repos/lrq3000/unireedsolomon/badge.svg?branch=master&service=github
-          :target: https://coveralls.io/github/lrq3000/unireedsolomon?branch=master
-        
-Keywords: error correction erasure reed solomon repair file network packet
-Platform: any
+Version: 1.0.6
+Summary: Universal errors-and-erasures Reed Solomon codec (error correcting code) in pure Python with extensive documentation and an object-oriented design.
+Author-email: Andrew Brown <brownan@gmail.com>, Stephen Karl Larroque <lrq3000@gmail.com>
+Maintainer-email: Stephen Karl Larroque <lrq3000@gmail.com>
+License: MIT License
+Project-URL: Homepage, https://github.com/lrq3000/unireedsolomon
+Project-URL: Documentation, https://github.com/lrq3000/unireedsolomon/blob/master/README.rst
+Project-URL: Source, https://github.com/lrq3000/unireedsolomon
+Project-URL: Tracker, https://github.com/lrq3000/unireedsolomon/issues
+Project-URL: Download, https://github.com/lrq3000/unireedsolomon/releases
+Keywords: data,protection,correction,recovery,restore,save,data recovery,reed-solomon,error correction code,qr,qr codes,barcodes,error correction,erasure,reed solomon,repair file,network packet
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Programming Language :: Cython
 Classifier: Topic :: Communications
 Classifier: Topic :: Scientific/Engineering :: Mathematics
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: System :: Archiving
 Classifier: Topic :: System :: Archiving :: Backup
 Classifier: Topic :: System :: Recovery Tools
+Classifier: Topic :: Utilities
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
+Classifier: Intended Audience :: System Administrators
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
+Provides-Extra: test
+Provides-Extra: testmeta
+License-File: LICENSE.txt
+
+UniReedSolomon
+==============
+
+|PyPI-Status| |PyPI-Versions| |PyPI-Downloads|
+
+|Build-Status| |Coverage|
+
+UniReedSolomon is a pure-Python universal Reed-Solomon error correction codec with fully documented code and mathematical nomenclatura, compatible with Python 3.7+ and also PyPy 3.
+
+If you are just starting with Reed-Solomon error correction codes, please see the `Wikiversity tutorial <https://en.wikiversity.org/wiki/Reed%E2%80%93Solomon_codes_for_coders>`_.
+
+Please also check out the more mature and faster `Reedsolo <https://github.com/tomerfiliba/reedsolomon>`_ module, a sibling project using a functional oriented approach instead of object oriented, and maintained by one of the co-authors of this project.
+
+------------------------------------
+
+.. contents:: Table of contents
+   :backlinks: top
+   :local:
+
+
+Installation
+------------
+
+For Python 3.7+:
+
+.. code:: sh
+
+    pip install --upgrade unireedsolomon
+
+For Python 2.7 and <= 3.6:
+
+.. code:: sh
+
+    pip install --upgrade unireedsolomon==1.0.5
+
+To install and compile the Cython speed-optimized modules ``cff.pyx`` and ``cpolynomial.pyx``, which provide a ~4x speed boost during encoding, install Cython 0.29.x and then type:
+
+.. code:: sh
+
+    pip install --upgrade unireedsolomon --config-setting="--build-option=--cythonize"
+
+Quickstart
+----------
+>>> import unireedsolomon as rs
+>>> coder = rs.RSCoder(20,13)
+>>> c = coder.encode("Hello, world!")
+>>> print repr(c)
+'Hello, world!\x8d\x13\xf4\xf9C\x10\xe5'
+>>>
+>>> r = "\0"*3 + c[3:]
+>>> print repr(r)
+'\x00\x00\x00lo, world!\x8d\x13\xf4\xf9C\x10\xe5'
+>>>
+>>> coder.decode(r)
+'Hello, world!'
+
+Description
+-----------
+This library implements a pure-Python documented universal Reed-Solomon
+error correction codec with a mathematical nomenclatura, compatible with
+Python 3.7+ and also with PyPy 3.
+
+The project aims to keep a well commented and organized code with
+an extensive documentation and mathematical clarity of the various
+arithmetic operations.
+
+How does this library differs from other Reed-Solomon libraries?
+
+* **universal**: compatibility with (almost) any other Reed-Solomon codec. This means that you can choose the parameters so that you can either encode data and decode it with another RS codec, or on the opposite encode data with another RS codec and decode this data with this library.
+* **errors-and-erasures decoding** allows to decode both erasures (where you know the position of the corrupted characters) and errors (where you don't know where are the corrupted characters) at the same time (because you can decode more erasures than errors, so if you can provide even a few know corrupted characters positions, this can help a lot the decoder to repair the message).
+* **documented**: following literate programming guidelines, you should understand everything you need about RS by reading the code and the comments.
+* **mathematical nomenclatura**: for example, contrary to most other RS libraries, you will see a clear distinction between the different mathematical constructs, such as the Galois Fields numbers are clearly separated from the generic Polynomial objects, and both are separated from the Reed-Solomon algorithm, which makes use of both of those constructs. For this purpose, object-oriented programming was chosen to design the architecture of the library, although obviously at the expense of a bit of performance. However, this library favors mathematical clarity and documentation over performance (even if performance is optimized whenever possible).
+* **pure-Python** means that there are no dependencies whatsoever apart from the Python interpreter. This means that this library should be resilient in the future (since it doesn't depend on external libraries who can become broken with time, see software rot), and you can use it on any system where Python can be installed (including online cloud services).
+
+The authors tried their best to extensively document the algorithms.
+However, a lot of the math involved is non-trivial and we can't explain it all
+in the comments. To learn more about the algorithms, see these resources:
+
+* `<http://en.wikipedia.org/wiki/Reed–Solomon_error_correction>`_
+* `<http://www.cs.duke.edu/courses/spring10/cps296.3/rs_scribe.pdf>`_
+* `<http://www.cs.duke.edu/courses/spring10/cps296.3/decoding_rs_scribe.pdf>`_
+* `<http://www.cs.cmu.edu/afs/cs.cmu.edu/project/pscico-guyb/realworld/www/reed_solomon.ps>`_
+* `<http://www.cs.cmu.edu/afs/cs.cmu.edu/project/pscico-guyb/realworld/www/rs_decode.ps>`_
+
+Also, here's a copy of the presentation one of the authors gave to the class Spring 2010 on his
+experience implementing this library. The LaTeX source is in the presentation directory.
+
+`<http://www.cs.duke.edu/courses/spring10/cps296.3/decoding_rs.pdf>`_
+
+The code was lately updated to support errors-and-erasures decoding (both at the same
+time), and to be universal (you can supply the parameters to be compatible with almost
+any other RS codec).
+
+The codec has decent performances if you use PyPy with the fast methods (~1 MB/s),
+but it would be faster if we drop the object-oriented design (implementing everything in
+functions), but this would be at the expense of mathematical clarity. If you are interested,
+see the reedsolo library by Tomer Filiba, which is exactly the same implementation but
+only functional without objects (results in about 5x speedup).
+
+Files
+-----
+rs.py
+    Holds the Reed-Solomon Encoder/Decoder object
+
+polynomial.py
+    Contains the Polynomial object (pure-python)
+
+ff.py
+    Contains the GF2int object representing an element of the GF(2^p) field, with p being 8 by default (pure-python)
+
+polynomial.pyx
+    Cython implementation of polynomial.py with equivalent functions (optional)
+
+ff.pyx
+    Cython implementation of ff.py with equivalent functions (optional)
+
+Documentation
+-------------
+unireedsolomon.rs.RSCoder(n, k, generator=3, prim=0x11b, fcr=1, c_exp=8)
+    Creates a new Reed-Solomon Encoder/Decoder object configured with
+    the given n and k values.
+    n is the length of a codeword, must be less than 256
+    k is the length of the message, must be less than n
+    generator, prim and fcr parametrize the Galois Field that will be built
+    c_exp is the Galois Field range (ie, 8 means GF(2^8) = GF(256)), which is both the limit for one symbol's value, and the maximum length of a message+ecc.
+
+    The code will have error correcting power (ie, maximum number of repairable symbols) of `2*e+v <= (n-k)`, where e is the number of errors and v the number of erasures.
+
+    The typical RSCoder is RSCoder(255, 223)
+
+RSCoder.encode(message, poly=False, k=None)
+    Encode a given string with reed-solomon encoding. Returns a byte
+    string with the k message bytes and n-k parity bytes at the end.
+
+    If a message is < k bytes long, it is assumed to be padded at the front
+    with null bytes (ie, a shortened Reed-Solomon code).
+
+    The sequence returned is always n bytes long.
+
+    If poly is not False, returns the encoded Polynomial object instead of
+    the polynomial translated back to a string (useful for debugging)
+
+    You can change the length (number) of parity/ecc bytes at encoding
+    by setting k to any value between [1, n-1]. This allows to create only
+    one RSCoder and then use it with a variable redundancy rate.
+
+RSCoder.encode_fast(message, poly=False, k=None)
+    Same as encode() but using faster algorithms and optimization tricks.
+
+RSCoder.decode(message_ecc, nostrip=False, k=None, erasures_pos=None, only_erasures=False):
+    Given a received string or byte array message_ecc (composed of
+    a message string + ecc symbols at the end), attempts to decode it.
+    If it's a valid codeword, or if there are no more than `2*e+v <= (n-k)` erratas
+    (called the Singleton bound), the message is returned.
+
+    You can provide the erasures positions as a list to erasures_pos.
+    For example, if you have "hella warld" and you know that `a` is an erasure,
+    you can provide the list erasures_pos=[4, 7]. You can correct twice as many
+    erasures than errors, and if some provided erasures are wrong (they are correct
+    symbols), then there's no problem, they will be repaired just fine (but will count
+    towards the Singleton bound). You can also specify that you are sure there are
+    only erasures and no errors at all by setting only_erasures=True.
+
+    A message always has k bytes, if a message contained less it is left
+    padded with null bytes (punctured RS code). When decoded, these leading
+    null bytes are stripped, but that can cause problems if decoding binary data.
+    When nostrip is True, messages returned are always k bytes long. This is
+    useful to make sure no data is lost when decoding binary data.
+
+    Note that RS can correct errors both in the message and the ecc symbols.
+
+RSCoder.decode_fast(message_ecc, nostrip=False, k=None, erasures_pos=None, only_erasures=False):
+    Same as decode() but using faster algorithms and optimization tricks.
+
+RSCoder.check(message_ecc, k=None)
+    Verifies the codeword (message + ecc symbols at the end) is valid by testing
+    that the code as a polynomial code divides g, or that the syndrome is
+    all 0 coefficients. The result is not foolproof: if it's False, you're sure the
+    message was corrupted (or that you used the wrong RS parameters),
+    but if it's True, it's either that the message is correct, or that there are
+    too many errors (ie, more than the Singleton bound) for RS to do anything about it.
+    returns True/False
+
+RSCoder.check_fast(message_ecc, k=None)
+    Same as check() but using faster algorithms and optimization tricks.
+
+unireedsolomon.ff.find_prime_polynomials(generator=2, c_exp=8, fast_primes=False, single=False)
+    Compute the list of prime polynomials for the given generator and
+    galois field characteristic exponent. You can then use this prime polynomial
+    to specify the mandatory "prim" parameter, particularly if you are using
+    a larger Galois Field (eg, 2^16).
+
+
+Internal API
+-------------
+Besides the main RSCoder object, two other objects are used in this
+implementation: Polynomial and GF2int. Their use is not specifically tied
+to the coder or even to the Reed-Solomon algorithm, they are just generic
+mathematical constructs respectively representing polynomials and
+Galois field's number of base 2.
+
+You do not need to know about the internal API to use the RS codec,
+this is just left as a documentation for the reader interested into dwelling
+inside the mathematical constructs.
+
+polynomial.Polynomial(coefficients=[], \**sparse)
+    There are three ways to initialize a Polynomial object.
+    1) With a list, tuple, or other iterable, creates a polynomial using
+    the items as coefficients in order of decreasing power
+
+    2) With keyword arguments such as for example x3=5, sets the
+    coefficient of x^3 to be 5
+
+    3) With no arguments, creates an empty polynomial, equivalent to
+    Polynomial([0])
+
+    >>> print Polynomial([5, 0, 0, 0, 0, 0])
+    5x^5
+
+    >>> print Polynomial(x32=5, x64=8)
+    8x^64 + 5x^32
+
+    >>> print Polynomial(x5=5, x9=4, x0=2) 
+    4x^9 + 5x^5 + 2
+
+Polynomial objects export the following standard functions that perform the
+expected operations using polynomial arithmetic. Arithmetic of the coefficients
+is determined by the type passed in, so integers or GF2int objects could be
+used, the Polynomial class is agnostic to the type of the coefficients.
+
+::
+
+    __add__
+    __divmod__
+    __eq__
+    __floordiv__
+    __hash__
+    __len__
+    __mod__
+    __mul__
+    __ne__
+    __neg__
+    __sub__
+    evaluate(x)
+    degree()
+        Returns the degree of the polynomial
+    get_coefficient(degree)
+        Returns the coefficient of the specified term
+
+ff.GF2int(value)
+    Instances of this object are elements of the field GF(2^p) and instances are integers
+    in the range 0 to `(2^p)-1`.
+    By default, the field is GF(2^8) and instances are integers in the range 0 to 255
+    and is defined using the irreducable polynomial 0x11b or in binary form:
+    x^8 + x^4 + x^3 + x + 1
+    and using 3 as the generator for the exponent table and log table.
+    
+    You can however use other parameters for the Galois Field, using the
+    init_lut() function.
+
+ff.find_prime_polynomials(generator=2, c_exp=8, fast_primes=False, single=False)
+    Find the list of prime polynomials to use to generate the look-up tables
+    for your field.
+
+ff.init_lut(generator=3, prim=0x11b, c_exp=8)
+    Generate the look-up tables given the parameters. This effectively parametrize
+    your Galois Field (ie, generator=2, prim=0x1002d, c_exp=16) will generate
+    a GF(2^16) field.
+
+The GF2int class inherits from int and supports all the usual integer
+operations. The following methods are overridden for arithmetic in the finite
+field GF(2^p)
+
+::
+
+    __add__
+    __div__
+    __mul__
+    __neg__
+    __pow__
+    __radd__
+    __rdiv__
+    __rmul__
+    __rsub__
+    __sub__
+    inverse()
+        Multiplicative inverse in GF(2^p)
+
+Edge cases
+-------------
+
+Although sanity checks are implemented whenever possible and when they are not too much resource consuming, there are a few cases where messages will not be decoded correctly without raising an exception:
+
+* If an incorrect erasure location is provided, the decoding algorithm will just trust the provided locations and create a syndrome that will be wrong, resulting in an incorrect decoded message. In case reliability is critical, always use the check() method after decoding to check the decoding did not go wrong.
+
+* Reed-Solomon algorithm is limited by the Singleton Bound, which limits not only its capacity to correct errors and erasures relatively to the number of error correction symbols, but also its ability to check if the message can be decoded or not. Indeed, if the number of errors and erasures are greater than the Singleton Bound, the decoder has no way to mathematically know for sure whether there is an error at all, it may very well be a valid message (although not the message you expect, but mathematically valid nevertheless). Hence, when the message is tampered beyond the Singleton Bound, the decoder may raise an exception, but it may also return a mathematically valid but still tampered message. Using the check() method cannot fix that either. To work around this issue, a solution is to use parity or hashing functions in parallel to the Reed-Solomon codec: use the Reed-Solomon codec to repair messages, use the parity or hashing function to check if there is any error. Due to how parity and hashing functions work, they are much less likely to produce a false negative than the Reed-Solomon algorithm. This is a general rule: error correction codes are efficient at correcting messages but not at detecting errors, hashing and parity functions are the adequate tool for this purpose.
+
+Example implementations
+-----------------------
+
+Image Encoder
+~~~~~~~~~~~~~
+imageencode.py is an example script that encodes codewords as rows in an image.
+It requires PIL to run.
+
+Usage: python imageencode.py [-d] <image file>
+
+Without the -d flag, imageencode.py will encode text from standard in and
+output it to the image file. With -d, imageencode.py will read in the data from
+the image and output to standard out the decoded text.
+
+An example is included: ``exampleimage.png``. Try decoding it as-is, then open
+it up in an image editor and paint some vertical stripes on it. As long as no
+more than 16 pixels per row are disturbed, the text will be decoded correctly.
+Then draw more stripes such that more than 16 pixels per row are disturbed and
+verify that the message is decoded improperly.
+
+Notice how the parity data looks different--the last 32 pixels of each row are
+colored differently. That's because this particular image contains encoded
+ASCII text, which generally only has bytes from a small range (the alphabet and
+printable punctuation). The parity data, however, is binary and contains bytes
+from the full range 0-255. Also note that either the data area or the parity
+area (or both!) can be disturbed as long as no more than 16 bytes per row are
+disturbed.
+
+Cython implementation
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+If either a C compiler or Cython is found, rs.py will automatically load the Cython implementations
+(the \*.pyx files).
+These are provided as optimized versions of the pure-python implementations, with equivalent
+functionalities. The goal was to get a speedup, which is the case, but using PyPy on the pure-python
+implementation provides a significantly higher speedup than the Cython implementation.
+The Cython implementations are still provided for the interested reader, but the casual user is
+not advised to use them. If you want to encode and decode fast, use PyPy.
+
+Projects using unireedsolomon
+-----------------------------
+
+* Several academic publications used unireedsolomon, see `this list <https://scholar.google.com/scholar?q=unireedsolomon>`_.
+
+Recommended reading
+-------------------
+
+* "`Reed-Solomon codes for coders <https://en.wikiversity.org/wiki/Reed%E2%80%93Solomon_codes_for_coders>`_", free practical beginner's tutorial with Python code examples on WikiVersity. Partially written by one of the authors of the present software.
+* "Algebraic codes for data transmission", Blahut, Richard E., 2003, Cambridge university press. `Readable online on Google Books <https://books.google.fr/books?id=eQs2i-R9-oYC&lpg=PR11&ots=atCPQJm3OJ&dq=%22Algebraic%20codes%20for%20data%20transmission%22%2C%20Blahut%2C%20Richard%20E.%2C%202003%2C%20Cambridge%20university%20press.&lr&hl=fr&pg=PA193#v=onepage&q=%22Algebraic%20codes%20for%20data%20transmission%22,%20Blahut,%20Richard%20E.,%202003,%20Cambridge%20university%20press.&f=false>`_. This book was pivotal in helping to understand the intricacies of the universal Berlekamp-Massey algorithm (see figures 7.5 and 7.10).
+
+Authors and licence
+-------------------
+Written from scratch by Andrew Brown <brownan@gmail.com> <brownan@cs.duke.edu>
+(c) 2010.
+
+Upgraded and maintained by Stephen Karl Larroque <LRQ3000@gmail.com> in 2015-2020.
+
+Licensed under the MIT License.
+
+
+.. |PyPI-Status| image:: https://img.shields.io/pypi/v/unireedsolomon.svg
+   :target: https://pypi.org/project/unireedsolomon
+.. |PyPI-Versions| image:: https://img.shields.io/pypi/pyversions/unireedsolomon.svg?logo=python&logoColor=white
+   :target: https://pypi.org/project/unireedsolomon
+.. |PyPI-Downloads| image:: https://img.shields.io/pypi/dm/unireedsolomon.svg?label=pypi%20downloads&logo=python&logoColor=white
+   :target: https://pypi.org/project/unireedsolomon
+.. |Build-Status| image:: https://github.com/lrq3000/unireedsolomon/actions/workflows/ci-build.yml/badge.svg?event=push
+    :target: https://github.com/lrq3000/unireedsolomon/actions/workflows/ci-build.yml
+.. |Coverage| image:: https://coveralls.io/repos/lrq3000/unireedsolomon/badge.svg?branch=master&service=github
+  :target: https://coveralls.io/github/lrq3000/unireedsolomon?branch=master
```

### Comparing `unireedsolomon-1.0.5/README.rst` & `unireedsolomon-1.0.6/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,37 +1,47 @@
 UniReedSolomon
 ==============
 
 |PyPI-Status| |PyPI-Versions| |PyPI-Downloads|
 
 |Build-Status| |Coverage|
 
-UniReedSolomon is a pure-Python universal Reed-Solomon error correction codec with fully documented code and mathematical nomenclatura, compatible with Python 2.7 up to 3.8 and also PyPy 2 and 3.
+UniReedSolomon is a pure-Python universal Reed-Solomon error correction codec with fully documented code and mathematical nomenclatura, compatible with Python 3.7+ and also PyPy 3.
 
 If you are just starting with Reed-Solomon error correction codes, please see the `Wikiversity tutorial <https://en.wikiversity.org/wiki/Reed%E2%80%93Solomon_codes_for_coders>`_.
 
+Please also check out the more mature and faster `Reedsolo <https://github.com/tomerfiliba/reedsolomon>`_ module, a sibling project using a functional oriented approach instead of object oriented, and maintained by one of the co-authors of this project.
+
 ------------------------------------
 
 .. contents:: Table of contents
    :backlinks: top
    :local:
 
 
 Installation
 ------------
 
+For Python 3.7+:
+
 .. code:: sh
 
     pip install --upgrade unireedsolomon
 
-.. note::
+For Python 2.7 and <= 3.6:
+
+.. code:: sh
 
-    When installing from source using ``python setup.py install``, the setup.py will try to build the Cython optimized module ``cff.pyx`` and ``cpolynomial.pyx`` if both Cython and a C compiler (eg, gcc) are installed, which provides ~4x speed boost during encoding. Although it should be done by default if Cython is installed, the compilation of Cython modules can be forced with ``python setup.py build_ext --inplace``. You can override this behavior by typing: ``python setup.py install --nocython`` to force the install only the pure python module without building the Cython modules.
+    pip install --upgrade unireedsolomon==1.0.5
+
+To install and compile the Cython speed-optimized modules ``cff.pyx`` and ``cpolynomial.pyx``, which provide a ~4x speed boost during encoding, install Cython 0.29.x and then type:
+
+.. code:: sh
 
-    Pre-transpiled ``cff.c`` and ``cpolynomial.c`` files are also available, and can be compiled with a C compiler without Cython by typing: ``python setup.py install --compile``.
+    pip install --upgrade unireedsolomon --config-setting="--build-option=--cythonize"
 
 Quickstart
 ----------
 >>> import unireedsolomon as rs
 >>> coder = rs.RSCoder(20,13)
 >>> c = coder.encode("Hello, world!")
 >>> print repr(c)
@@ -44,15 +54,15 @@
 >>> coder.decode(r)
 'Hello, world!'
 
 Description
 -----------
 This library implements a pure-Python documented universal Reed-Solomon
 error correction codec with a mathematical nomenclatura, compatible with
-Python 2.7 up to 3.7+ and also with PyPy 2 and PyPy 3.
+Python 3.7+ and also with PyPy 3.
 
 The project aims to keep a well commented and organized code with
 an extensive documentation and mathematical clarity of the various
 arithmetic operations.
 
 How does this library differs from other Reed-Solomon libraries?
 
@@ -272,14 +282,23 @@
     __rdiv__
     __rmul__
     __rsub__
     __sub__
     inverse()
         Multiplicative inverse in GF(2^p)
 
+Edge cases
+-------------
+
+Although sanity checks are implemented whenever possible and when they are not too much resource consuming, there are a few cases where messages will not be decoded correctly without raising an exception:
+
+* If an incorrect erasure location is provided, the decoding algorithm will just trust the provided locations and create a syndrome that will be wrong, resulting in an incorrect decoded message. In case reliability is critical, always use the check() method after decoding to check the decoding did not go wrong.
+
+* Reed-Solomon algorithm is limited by the Singleton Bound, which limits not only its capacity to correct errors and erasures relatively to the number of error correction symbols, but also its ability to check if the message can be decoded or not. Indeed, if the number of errors and erasures are greater than the Singleton Bound, the decoder has no way to mathematically know for sure whether there is an error at all, it may very well be a valid message (although not the message you expect, but mathematically valid nevertheless). Hence, when the message is tampered beyond the Singleton Bound, the decoder may raise an exception, but it may also return a mathematically valid but still tampered message. Using the check() method cannot fix that either. To work around this issue, a solution is to use parity or hashing functions in parallel to the Reed-Solomon codec: use the Reed-Solomon codec to repair messages, use the parity or hashing function to check if there is any error. Due to how parity and hashing functions work, they are much less likely to produce a false negative than the Reed-Solomon algorithm. This is a general rule: error correction codes are efficient at correcting messages but not at detecting errors, hashing and parity functions are the adequate tool for this purpose.
+
 Example implementations
 -----------------------
 
 Image Encoder
 ~~~~~~~~~~~~~
 imageencode.py is an example script that encodes codewords as rows in an image.
 It requires PIL to run.
@@ -311,14 +330,19 @@
 (the \*.pyx files).
 These are provided as optimized versions of the pure-python implementations, with equivalent
 functionalities. The goal was to get a speedup, which is the case, but using PyPy on the pure-python
 implementation provides a significantly higher speedup than the Cython implementation.
 The Cython implementations are still provided for the interested reader, but the casual user is
 not advised to use them. If you want to encode and decode fast, use PyPy.
 
+Projects using unireedsolomon
+-----------------------------
+
+* Several academic publications used unireedsolomon, see `this list <https://scholar.google.com/scholar?q=unireedsolomon>`_.
+
 Recommended reading
 -------------------
 
 * "`Reed-Solomon codes for coders <https://en.wikiversity.org/wiki/Reed%E2%80%93Solomon_codes_for_coders>`_", free practical beginner's tutorial with Python code examples on WikiVersity. Partially written by one of the authors of the present software.
 * "Algebraic codes for data transmission", Blahut, Richard E., 2003, Cambridge university press. `Readable online on Google Books <https://books.google.fr/books?id=eQs2i-R9-oYC&lpg=PR11&ots=atCPQJm3OJ&dq=%22Algebraic%20codes%20for%20data%20transmission%22%2C%20Blahut%2C%20Richard%20E.%2C%202003%2C%20Cambridge%20university%20press.&lr&hl=fr&pg=PA193#v=onepage&q=%22Algebraic%20codes%20for%20data%20transmission%22,%20Blahut,%20Richard%20E.,%202003,%20Cambridge%20university%20press.&f=false>`_. This book was pivotal in helping to understand the intricacies of the universal Berlekamp-Massey algorithm (see figures 7.5 and 7.10).
 
 Authors and licence
@@ -333,11 +357,11 @@
 
 .. |PyPI-Status| image:: https://img.shields.io/pypi/v/unireedsolomon.svg
    :target: https://pypi.org/project/unireedsolomon
 .. |PyPI-Versions| image:: https://img.shields.io/pypi/pyversions/unireedsolomon.svg?logo=python&logoColor=white
    :target: https://pypi.org/project/unireedsolomon
 .. |PyPI-Downloads| image:: https://img.shields.io/pypi/dm/unireedsolomon.svg?label=pypi%20downloads&logo=python&logoColor=white
    :target: https://pypi.org/project/unireedsolomon
-.. |Build-Status| image:: https://travis-ci.org/lrq3000/unireedsolomon.svg?branch=master
-    :target: https://travis-ci.org/lrq3000/unireedsolomon
+.. |Build-Status| image:: https://github.com/lrq3000/unireedsolomon/actions/workflows/ci-build.yml/badge.svg?event=push
+    :target: https://github.com/lrq3000/unireedsolomon/actions/workflows/ci-build.yml
 .. |Coverage| image:: https://coveralls.io/repos/lrq3000/unireedsolomon/badge.svg?branch=master&service=github
   :target: https://coveralls.io/github/lrq3000/unireedsolomon?branch=master
```

### Comparing `unireedsolomon-1.0.5/notes.txt` & `unireedsolomon-1.0.6/notes.txt`

 * *Files identical despite different names*

### Comparing `unireedsolomon-1.0.5/unireedsolomon/cff.pyx` & `unireedsolomon-1.0.6/src/unireedsolomon/cff.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # -*- coding: utf-8 -*-
+#cython: language_level=2
 
 # Copyright (c) 2010 Andrew Brown <brownan@cs.duke.edu, brownan@gmail.com>
-# Copyright (c) 2015 Stephen Larroque <LRQ3000@gmail.com>
+# Copyright (c) 2015-2023 Stephen Larroque <LRQ3000@gmail.com>
 # See LICENSE.txt for license terms
 
 # For fast software computation in Finite Fields, see the excellent paper: Huang, Cheng, and Lihao Xu. "Fast software implementation of finite field operations." Washington University in St. Louis, Tech. Rep (2003).
 # to understand the basic mathematical notions behind finite fields, see the excellent tutorial: http://research.swtch.com/field
 
 import cython
 cimport cython
```

### Comparing `unireedsolomon-1.0.5/unireedsolomon/cpolynomial.pyx` & `unireedsolomon-1.0.6/src/unireedsolomon/cpolynomial.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # -*- coding: utf-8 -*-
+#cython: language_level=2
 
 # Copyright (c) 2010 Andrew Brown <brownan@cs.duke.edu, brownan@gmail.com>
-# Copyright (c) 2015 Stephen Larroque <LRQ3000@gmail.com>
+# Copyright (c) 2015-2023 Stephen Larroque <LRQ3000@gmail.com>
 # See LICENSE.txt for license terms
 
 import cython
 cimport cython
 
 from ._compat import _range, _StringIO
```

### Comparing `unireedsolomon-1.0.5/unireedsolomon/ff.py` & `unireedsolomon-1.0.6/src/unireedsolomon/ff.py`

 * *Files identical despite different names*

### Comparing `unireedsolomon-1.0.5/unireedsolomon/imageencode.py` & `unireedsolomon-1.0.6/src/unireedsolomon/imageencode.py`

 * *Files identical despite different names*

### Comparing `unireedsolomon-1.0.5/unireedsolomon/polynomial.py` & `unireedsolomon-1.0.6/src/unireedsolomon/polynomial.py`

 * *Files identical despite different names*

### Comparing `unireedsolomon-1.0.5/unireedsolomon/rs.py` & `unireedsolomon-1.0.6/src/unireedsolomon/rs.py`

 * *Files identical despite different names*

### Comparing `unireedsolomon-1.0.5/unireedsolomon/tests/test_cff.py` & `unireedsolomon-1.0.6/src/unireedsolomon/tests/test_cff.py`

 * *Files identical despite different names*

### Comparing `unireedsolomon-1.0.5/unireedsolomon/tests/test_cpolynomial.py` & `unireedsolomon-1.0.6/src/unireedsolomon/tests/test_cpolynomial.py`

 * *Files identical despite different names*

### Comparing `unireedsolomon-1.0.5/unireedsolomon/tests/test_ff.py` & `unireedsolomon-1.0.6/src/unireedsolomon/tests/test_ff.py`

 * *Files identical despite different names*

### Comparing `unireedsolomon-1.0.5/unireedsolomon/tests/test_polynomial.py` & `unireedsolomon-1.0.6/src/unireedsolomon/tests/test_polynomial.py`

 * *Files identical despite different names*

### Comparing `unireedsolomon-1.0.5/unireedsolomon/tests/test_rs.py` & `unireedsolomon-1.0.6/src/unireedsolomon/tests/test_rs.py`

 * *Files identical despite different names*

### Comparing `unireedsolomon-1.0.5/unireedsolomon.egg-info/PKG-INFO` & `unireedsolomon-1.0.6/src/unireedsolomon.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,374 +1,410 @@
 Metadata-Version: 2.1
 Name: unireedsolomon
-Version: 1.0.5
-Summary: Universal errors-and-erasures Reed Solomon codec (error correcting code) in pure Python with extensive documentation
-Home-page: https://github.com/lrq3000/unireedsolomon
-Author: Andrew Brown, Stephen Larroque
-Author-email: lrq3000@gmail.com
-License: MIT
-Description: UniReedSolomon
-        ==============
-        
-        |PyPI-Status| |PyPI-Versions| |PyPI-Downloads|
-        
-        |Build-Status| |Coverage|
-        
-        UniReedSolomon is a pure-Python universal Reed-Solomon error correction codec with fully documented code and mathematical nomenclatura, compatible with Python 2.7 up to 3.8 and also PyPy 2 and 3.
-        
-        If you are just starting with Reed-Solomon error correction codes, please see the `Wikiversity tutorial <https://en.wikiversity.org/wiki/Reed%E2%80%93Solomon_codes_for_coders>`_.
-        
-        ------------------------------------
-        
-        .. contents:: Table of contents
-           :backlinks: top
-           :local:
-        
-        
-        Installation
-        ------------
-        
-        .. code:: sh
-        
-            pip install --upgrade unireedsolomon
-        
-        .. note::
-        
-            When installing from source using ``python setup.py install``, the setup.py will try to build the Cython optimized module ``cff.pyx`` and ``cpolynomial.pyx`` if both Cython and a C compiler (eg, gcc) are installed, which provides ~4x speed boost during encoding. Although it should be done by default if Cython is installed, the compilation of Cython modules can be forced with ``python setup.py build_ext --inplace``. You can override this behavior by typing: ``python setup.py install --nocython`` to force the install only the pure python module without building the Cython modules.
-        
-            Pre-transpiled ``cff.c`` and ``cpolynomial.c`` files are also available, and can be compiled with a C compiler without Cython by typing: ``python setup.py install --compile``.
-        
-        Quickstart
-        ----------
-        >>> import unireedsolomon as rs
-        >>> coder = rs.RSCoder(20,13)
-        >>> c = coder.encode("Hello, world!")
-        >>> print repr(c)
-        'Hello, world!\x8d\x13\xf4\xf9C\x10\xe5'
-        >>>
-        >>> r = "\0"*3 + c[3:]
-        >>> print repr(r)
-        '\x00\x00\x00lo, world!\x8d\x13\xf4\xf9C\x10\xe5'
-        >>>
-        >>> coder.decode(r)
-        'Hello, world!'
-        
-        Description
-        -----------
-        This library implements a pure-Python documented universal Reed-Solomon
-        error correction codec with a mathematical nomenclatura, compatible with
-        Python 2.7 up to 3.7+ and also with PyPy 2 and PyPy 3.
-        
-        The project aims to keep a well commented and organized code with
-        an extensive documentation and mathematical clarity of the various
-        arithmetic operations.
-        
-        How does this library differs from other Reed-Solomon libraries?
-        
-        * **universal**: compatibility with (almost) any other Reed-Solomon codec. This means that you can choose the parameters so that you can either encode data and decode it with another RS codec, or on the opposite encode data with another RS codec and decode this data with this library.
-        * **errors-and-erasures decoding** allows to decode both erasures (where you know the position of the corrupted characters) and errors (where you don't know where are the corrupted characters) at the same time (because you can decode more erasures than errors, so if you can provide even a few know corrupted characters positions, this can help a lot the decoder to repair the message).
-        * **documented**: following literate programming guidelines, you should understand everything you need about RS by reading the code and the comments.
-        * **mathematical nomenclatura**: for example, contrary to most other RS libraries, you will see a clear distinction between the different mathematical constructs, such as the Galois Fields numbers are clearly separated from the generic Polynomial objects, and both are separated from the Reed-Solomon algorithm, which makes use of both of those constructs. For this purpose, object-oriented programming was chosen to design the architecture of the library, although obviously at the expense of a bit of performance. However, this library favors mathematical clarity and documentation over performance (even if performance is optimized whenever possible).
-        * **pure-Python** means that there are no dependencies whatsoever apart from the Python interpreter. This means that this library should be resilient in the future (since it doesn't depend on external libraries who can become broken with time, see software rot), and you can use it on any system where Python can be installed (including online cloud services).
-        
-        The authors tried their best to extensively document the algorithms.
-        However, a lot of the math involved is non-trivial and we can't explain it all
-        in the comments. To learn more about the algorithms, see these resources:
-        
-        * `<http://en.wikipedia.org/wiki/Reedâ€“Solomon_error_correction>`_
-        * `<http://www.cs.duke.edu/courses/spring10/cps296.3/rs_scribe.pdf>`_
-        * `<http://www.cs.duke.edu/courses/spring10/cps296.3/decoding_rs_scribe.pdf>`_
-        * `<http://www.cs.cmu.edu/afs/cs.cmu.edu/project/pscico-guyb/realworld/www/reed_solomon.ps>`_
-        * `<http://www.cs.cmu.edu/afs/cs.cmu.edu/project/pscico-guyb/realworld/www/rs_decode.ps>`_
-        
-        Also, here's a copy of the presentation one of the authors gave to the class Spring 2010 on his
-        experience implementing this library. The LaTeX source is in the presentation directory.
-        
-        `<http://www.cs.duke.edu/courses/spring10/cps296.3/decoding_rs.pdf>`_
-        
-        The code was lately updated to support errors-and-erasures decoding (both at the same
-        time), and to be universal (you can supply the parameters to be compatible with almost
-        any other RS codec).
-        
-        The codec has decent performances if you use PyPy with the fast methods (~1 MB/s),
-        but it would be faster if we drop the object-oriented design (implementing everything in
-        functions), but this would be at the expense of mathematical clarity. If you are interested,
-        see the reedsolo library by Tomer Filiba, which is exactly the same implementation but
-        only functional without objects (results in about 5x speedup).
-        
-        Files
-        -----
-        rs.py
-            Holds the Reed-Solomon Encoder/Decoder object
-        
-        polynomial.py
-            Contains the Polynomial object (pure-python)
-        
-        ff.py
-            Contains the GF2int object representing an element of the GF(2^p) field, with p being 8 by default (pure-python)
-        
-        polynomial.pyx
-            Cython implementation of polynomial.py with equivalent functions (optional)
-        
-        ff.pyx
-            Cython implementation of ff.py with equivalent functions (optional)
-        
-        Documentation
-        -------------
-        unireedsolomon.rs.RSCoder(n, k, generator=3, prim=0x11b, fcr=1, c_exp=8)
-            Creates a new Reed-Solomon Encoder/Decoder object configured with
-            the given n and k values.
-            n is the length of a codeword, must be less than 256
-            k is the length of the message, must be less than n
-            generator, prim and fcr parametrize the Galois Field that will be built
-            c_exp is the Galois Field range (ie, 8 means GF(2^8) = GF(256)), which is both the limit for one symbol's value, and the maximum length of a message+ecc.
-        
-            The code will have error correcting power (ie, maximum number of repairable symbols) of `2*e+v <= (n-k)`, where e is the number of errors and v the number of erasures.
-        
-            The typical RSCoder is RSCoder(255, 223)
-        
-        RSCoder.encode(message, poly=False, k=None)
-            Encode a given string with reed-solomon encoding. Returns a byte
-            string with the k message bytes and n-k parity bytes at the end.
-        
-            If a message is < k bytes long, it is assumed to be padded at the front
-            with null bytes (ie, a shortened Reed-Solomon code).
-        
-            The sequence returned is always n bytes long.
-        
-            If poly is not False, returns the encoded Polynomial object instead of
-            the polynomial translated back to a string (useful for debugging)
-        
-            You can change the length (number) of parity/ecc bytes at encoding
-            by setting k to any value between [1, n-1]. This allows to create only
-            one RSCoder and then use it with a variable redundancy rate.
-        
-        RSCoder.encode_fast(message, poly=False, k=None)
-            Same as encode() but using faster algorithms and optimization tricks.
-        
-        RSCoder.decode(message_ecc, nostrip=False, k=None, erasures_pos=None, only_erasures=False):
-            Given a received string or byte array message_ecc (composed of
-            a message string + ecc symbols at the end), attempts to decode it.
-            If it's a valid codeword, or if there are no more than `2*e+v <= (n-k)` erratas
-            (called the Singleton bound), the message is returned.
-        
-            You can provide the erasures positions as a list to erasures_pos.
-            For example, if you have "hella warld" and you know that `a` is an erasure,
-            you can provide the list erasures_pos=[4, 7]. You can correct twice as many
-            erasures than errors, and if some provided erasures are wrong (they are correct
-            symbols), then there's no problem, they will be repaired just fine (but will count
-            towards the Singleton bound). You can also specify that you are sure there are
-            only erasures and no errors at all by setting only_erasures=True.
-        
-            A message always has k bytes, if a message contained less it is left
-            padded with null bytes (punctured RS code). When decoded, these leading
-            null bytes are stripped, but that can cause problems if decoding binary data.
-            When nostrip is True, messages returned are always k bytes long. This is
-            useful to make sure no data is lost when decoding binary data.
-        
-            Note that RS can correct errors both in the message and the ecc symbols.
-        
-        RSCoder.decode_fast(message_ecc, nostrip=False, k=None, erasures_pos=None, only_erasures=False):
-            Same as decode() but using faster algorithms and optimization tricks.
-        
-        RSCoder.check(message_ecc, k=None)
-            Verifies the codeword (message + ecc symbols at the end) is valid by testing
-            that the code as a polynomial code divides g, or that the syndrome is
-            all 0 coefficients. The result is not foolproof: if it's False, you're sure the
-            message was corrupted (or that you used the wrong RS parameters),
-            but if it's True, it's either that the message is correct, or that there are
-            too many errors (ie, more than the Singleton bound) for RS to do anything about it.
-            returns True/False
-        
-        RSCoder.check_fast(message_ecc, k=None)
-            Same as check() but using faster algorithms and optimization tricks.
-        
-        unireedsolomon.ff.find_prime_polynomials(generator=2, c_exp=8, fast_primes=False, single=False)
-            Compute the list of prime polynomials for the given generator and
-            galois field characteristic exponent. You can then use this prime polynomial
-            to specify the mandatory "prim" parameter, particularly if you are using
-            a larger Galois Field (eg, 2^16).
-        
-        
-        Internal API
-        -------------
-        Besides the main RSCoder object, two other objects are used in this
-        implementation: Polynomial and GF2int. Their use is not specifically tied
-        to the coder or even to the Reed-Solomon algorithm, they are just generic
-        mathematical constructs respectively representing polynomials and
-        Galois field's number of base 2.
-        
-        You do not need to know about the internal API to use the RS codec,
-        this is just left as a documentation for the reader interested into dwelling
-        inside the mathematical constructs.
-        
-        polynomial.Polynomial(coefficients=[], \**sparse)
-            There are three ways to initialize a Polynomial object.
-            1) With a list, tuple, or other iterable, creates a polynomial using
-            the items as coefficients in order of decreasing power
-        
-            2) With keyword arguments such as for example x3=5, sets the
-            coefficient of x^3 to be 5
-        
-            3) With no arguments, creates an empty polynomial, equivalent to
-            Polynomial([0])
-        
-            >>> print Polynomial([5, 0, 0, 0, 0, 0])
-            5x^5
-        
-            >>> print Polynomial(x32=5, x64=8)
-            8x^64 + 5x^32
-        
-            >>> print Polynomial(x5=5, x9=4, x0=2) 
-            4x^9 + 5x^5 + 2
-        
-        Polynomial objects export the following standard functions that perform the
-        expected operations using polynomial arithmetic. Arithmetic of the coefficients
-        is determined by the type passed in, so integers or GF2int objects could be
-        used, the Polynomial class is agnostic to the type of the coefficients.
-        
-        ::
-        
-            __add__
-            __divmod__
-            __eq__
-            __floordiv__
-            __hash__
-            __len__
-            __mod__
-            __mul__
-            __ne__
-            __neg__
-            __sub__
-            evaluate(x)
-            degree()
-                Returns the degree of the polynomial
-            get_coefficient(degree)
-                Returns the coefficient of the specified term
-        
-        ff.GF2int(value)
-            Instances of this object are elements of the field GF(2^p) and instances are integers
-            in the range 0 to `(2^p)-1`.
-            By default, the field is GF(2^8) and instances are integers in the range 0 to 255
-            and is defined using the irreducable polynomial 0x11b or in binary form:
-            x^8 + x^4 + x^3 + x + 1
-            and using 3 as the generator for the exponent table and log table.
-            
-            You can however use other parameters for the Galois Field, using the
-            init_lut() function.
-        
-        ff.find_prime_polynomials(generator=2, c_exp=8, fast_primes=False, single=False)
-            Find the list of prime polynomials to use to generate the look-up tables
-            for your field.
-        
-        ff.init_lut(generator=3, prim=0x11b, c_exp=8)
-            Generate the look-up tables given the parameters. This effectively parametrize
-            your Galois Field (ie, generator=2, prim=0x1002d, c_exp=16) will generate
-            a GF(2^16) field.
-        
-        The GF2int class inherits from int and supports all the usual integer
-        operations. The following methods are overridden for arithmetic in the finite
-        field GF(2^p)
-        
-        ::
-        
-            __add__
-            __div__
-            __mul__
-            __neg__
-            __pow__
-            __radd__
-            __rdiv__
-            __rmul__
-            __rsub__
-            __sub__
-            inverse()
-                Multiplicative inverse in GF(2^p)
-        
-        Example implementations
-        -----------------------
-        
-        Image Encoder
-        ~~~~~~~~~~~~~
-        imageencode.py is an example script that encodes codewords as rows in an image.
-        It requires PIL to run.
-        
-        Usage: python imageencode.py [-d] <image file>
-        
-        Without the -d flag, imageencode.py will encode text from standard in and
-        output it to the image file. With -d, imageencode.py will read in the data from
-        the image and output to standard out the decoded text.
-        
-        An example is included: ``exampleimage.png``. Try decoding it as-is, then open
-        it up in an image editor and paint some vertical stripes on it. As long as no
-        more than 16 pixels per row are disturbed, the text will be decoded correctly.
-        Then draw more stripes such that more than 16 pixels per row are disturbed and
-        verify that the message is decoded improperly.
-        
-        Notice how the parity data looks different--the last 32 pixels of each row are
-        colored differently. That's because this particular image contains encoded
-        ASCII text, which generally only has bytes from a small range (the alphabet and
-        printable punctuation). The parity data, however, is binary and contains bytes
-        from the full range 0-255. Also note that either the data area or the parity
-        area (or both!) can be disturbed as long as no more than 16 bytes per row are
-        disturbed.
-        
-        Cython implementation
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        If either a C compiler or Cython is found, rs.py will automatically load the Cython implementations
-        (the \*.pyx files).
-        These are provided as optimized versions of the pure-python implementations, with equivalent
-        functionalities. The goal was to get a speedup, which is the case, but using PyPy on the pure-python
-        implementation provides a significantly higher speedup than the Cython implementation.
-        The Cython implementations are still provided for the interested reader, but the casual user is
-        not advised to use them. If you want to encode and decode fast, use PyPy.
-        
-        Recommended reading
-        -------------------
-        
-        * "`Reed-Solomon codes for coders <https://en.wikiversity.org/wiki/Reed%E2%80%93Solomon_codes_for_coders>`_", free practical beginner's tutorial with Python code examples on WikiVersity. Partially written by one of the authors of the present software.
-        * "Algebraic codes for data transmission", Blahut, Richard E., 2003, Cambridge university press. `Readable online on Google Books <https://books.google.fr/books?id=eQs2i-R9-oYC&lpg=PR11&ots=atCPQJm3OJ&dq=%22Algebraic%20codes%20for%20data%20transmission%22%2C%20Blahut%2C%20Richard%20E.%2C%202003%2C%20Cambridge%20university%20press.&lr&hl=fr&pg=PA193#v=onepage&q=%22Algebraic%20codes%20for%20data%20transmission%22,%20Blahut,%20Richard%20E.,%202003,%20Cambridge%20university%20press.&f=false>`_. This book was pivotal in helping to understand the intricacies of the universal Berlekamp-Massey algorithm (see figures 7.5 and 7.10).
-        
-        Authors and licence
-        -------------------
-        Written from scratch by Andrew Brown <brownan@gmail.com> <brownan@cs.duke.edu>
-        (c) 2010.
-        
-        Upgraded and maintained by Stephen Karl Larroque <LRQ3000@gmail.com> in 2015-2020.
-        
-        Licensed under the MIT License.
-        
-        
-        .. |PyPI-Status| image:: https://img.shields.io/pypi/v/unireedsolomon.svg
-           :target: https://pypi.org/project/unireedsolomon
-        .. |PyPI-Versions| image:: https://img.shields.io/pypi/pyversions/unireedsolomon.svg?logo=python&logoColor=white
-           :target: https://pypi.org/project/unireedsolomon
-        .. |PyPI-Downloads| image:: https://img.shields.io/pypi/dm/unireedsolomon.svg?label=pypi%20downloads&logo=python&logoColor=white
-           :target: https://pypi.org/project/unireedsolomon
-        .. |Build-Status| image:: https://travis-ci.org/lrq3000/unireedsolomon.svg?branch=master
-            :target: https://travis-ci.org/lrq3000/unireedsolomon
-        .. |Coverage| image:: https://coveralls.io/repos/lrq3000/unireedsolomon/badge.svg?branch=master&service=github
-          :target: https://coveralls.io/github/lrq3000/unireedsolomon?branch=master
-        
-Keywords: error correction erasure reed solomon repair file network packet
-Platform: any
+Version: 1.0.6
+Summary: Universal errors-and-erasures Reed Solomon codec (error correcting code) in pure Python with extensive documentation and an object-oriented design.
+Author-email: Andrew Brown <brownan@gmail.com>, Stephen Karl Larroque <lrq3000@gmail.com>
+Maintainer-email: Stephen Karl Larroque <lrq3000@gmail.com>
+License: MIT License
+Project-URL: Homepage, https://github.com/lrq3000/unireedsolomon
+Project-URL: Documentation, https://github.com/lrq3000/unireedsolomon/blob/master/README.rst
+Project-URL: Source, https://github.com/lrq3000/unireedsolomon
+Project-URL: Tracker, https://github.com/lrq3000/unireedsolomon/issues
+Project-URL: Download, https://github.com/lrq3000/unireedsolomon/releases
+Keywords: data,protection,correction,recovery,restore,save,data recovery,reed-solomon,error correction code,qr,qr codes,barcodes,error correction,erasure,reed solomon,repair file,network packet
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Programming Language :: Cython
 Classifier: Topic :: Communications
 Classifier: Topic :: Scientific/Engineering :: Mathematics
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: System :: Archiving
 Classifier: Topic :: System :: Archiving :: Backup
 Classifier: Topic :: System :: Recovery Tools
+Classifier: Topic :: Utilities
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
+Classifier: Intended Audience :: System Administrators
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
+Provides-Extra: test
+Provides-Extra: testmeta
+License-File: LICENSE.txt
+
+UniReedSolomon
+==============
+
+|PyPI-Status| |PyPI-Versions| |PyPI-Downloads|
+
+|Build-Status| |Coverage|
+
+UniReedSolomon is a pure-Python universal Reed-Solomon error correction codec with fully documented code and mathematical nomenclatura, compatible with Python 3.7+ and also PyPy 3.
+
+If you are just starting with Reed-Solomon error correction codes, please see the `Wikiversity tutorial <https://en.wikiversity.org/wiki/Reed%E2%80%93Solomon_codes_for_coders>`_.
+
+Please also check out the more mature and faster `Reedsolo <https://github.com/tomerfiliba/reedsolomon>`_ module, a sibling project using a functional oriented approach instead of object oriented, and maintained by one of the co-authors of this project.
+
+------------------------------------
+
+.. contents:: Table of contents
+   :backlinks: top
+   :local:
+
+
+Installation
+------------
+
+For Python 3.7+:
+
+.. code:: sh
+
+    pip install --upgrade unireedsolomon
+
+For Python 2.7 and <= 3.6:
+
+.. code:: sh
+
+    pip install --upgrade unireedsolomon==1.0.5
+
+To install and compile the Cython speed-optimized modules ``cff.pyx`` and ``cpolynomial.pyx``, which provide a ~4x speed boost during encoding, install Cython 0.29.x and then type:
+
+.. code:: sh
+
+    pip install --upgrade unireedsolomon --config-setting="--build-option=--cythonize"
+
+Quickstart
+----------
+>>> import unireedsolomon as rs
+>>> coder = rs.RSCoder(20,13)
+>>> c = coder.encode("Hello, world!")
+>>> print repr(c)
+'Hello, world!\x8d\x13\xf4\xf9C\x10\xe5'
+>>>
+>>> r = "\0"*3 + c[3:]
+>>> print repr(r)
+'\x00\x00\x00lo, world!\x8d\x13\xf4\xf9C\x10\xe5'
+>>>
+>>> coder.decode(r)
+'Hello, world!'
+
+Description
+-----------
+This library implements a pure-Python documented universal Reed-Solomon
+error correction codec with a mathematical nomenclatura, compatible with
+Python 3.7+ and also with PyPy 3.
+
+The project aims to keep a well commented and organized code with
+an extensive documentation and mathematical clarity of the various
+arithmetic operations.
+
+How does this library differs from other Reed-Solomon libraries?
+
+* **universal**: compatibility with (almost) any other Reed-Solomon codec. This means that you can choose the parameters so that you can either encode data and decode it with another RS codec, or on the opposite encode data with another RS codec and decode this data with this library.
+* **errors-and-erasures decoding** allows to decode both erasures (where you know the position of the corrupted characters) and errors (where you don't know where are the corrupted characters) at the same time (because you can decode more erasures than errors, so if you can provide even a few know corrupted characters positions, this can help a lot the decoder to repair the message).
+* **documented**: following literate programming guidelines, you should understand everything you need about RS by reading the code and the comments.
+* **mathematical nomenclatura**: for example, contrary to most other RS libraries, you will see a clear distinction between the different mathematical constructs, such as the Galois Fields numbers are clearly separated from the generic Polynomial objects, and both are separated from the Reed-Solomon algorithm, which makes use of both of those constructs. For this purpose, object-oriented programming was chosen to design the architecture of the library, although obviously at the expense of a bit of performance. However, this library favors mathematical clarity and documentation over performance (even if performance is optimized whenever possible).
+* **pure-Python** means that there are no dependencies whatsoever apart from the Python interpreter. This means that this library should be resilient in the future (since it doesn't depend on external libraries who can become broken with time, see software rot), and you can use it on any system where Python can be installed (including online cloud services).
+
+The authors tried their best to extensively document the algorithms.
+However, a lot of the math involved is non-trivial and we can't explain it all
+in the comments. To learn more about the algorithms, see these resources:
+
+* `<http://en.wikipedia.org/wiki/Reed–Solomon_error_correction>`_
+* `<http://www.cs.duke.edu/courses/spring10/cps296.3/rs_scribe.pdf>`_
+* `<http://www.cs.duke.edu/courses/spring10/cps296.3/decoding_rs_scribe.pdf>`_
+* `<http://www.cs.cmu.edu/afs/cs.cmu.edu/project/pscico-guyb/realworld/www/reed_solomon.ps>`_
+* `<http://www.cs.cmu.edu/afs/cs.cmu.edu/project/pscico-guyb/realworld/www/rs_decode.ps>`_
+
+Also, here's a copy of the presentation one of the authors gave to the class Spring 2010 on his
+experience implementing this library. The LaTeX source is in the presentation directory.
+
+`<http://www.cs.duke.edu/courses/spring10/cps296.3/decoding_rs.pdf>`_
+
+The code was lately updated to support errors-and-erasures decoding (both at the same
+time), and to be universal (you can supply the parameters to be compatible with almost
+any other RS codec).
+
+The codec has decent performances if you use PyPy with the fast methods (~1 MB/s),
+but it would be faster if we drop the object-oriented design (implementing everything in
+functions), but this would be at the expense of mathematical clarity. If you are interested,
+see the reedsolo library by Tomer Filiba, which is exactly the same implementation but
+only functional without objects (results in about 5x speedup).
+
+Files
+-----
+rs.py
+    Holds the Reed-Solomon Encoder/Decoder object
+
+polynomial.py
+    Contains the Polynomial object (pure-python)
+
+ff.py
+    Contains the GF2int object representing an element of the GF(2^p) field, with p being 8 by default (pure-python)
+
+polynomial.pyx
+    Cython implementation of polynomial.py with equivalent functions (optional)
+
+ff.pyx
+    Cython implementation of ff.py with equivalent functions (optional)
+
+Documentation
+-------------
+unireedsolomon.rs.RSCoder(n, k, generator=3, prim=0x11b, fcr=1, c_exp=8)
+    Creates a new Reed-Solomon Encoder/Decoder object configured with
+    the given n and k values.
+    n is the length of a codeword, must be less than 256
+    k is the length of the message, must be less than n
+    generator, prim and fcr parametrize the Galois Field that will be built
+    c_exp is the Galois Field range (ie, 8 means GF(2^8) = GF(256)), which is both the limit for one symbol's value, and the maximum length of a message+ecc.
+
+    The code will have error correcting power (ie, maximum number of repairable symbols) of `2*e+v <= (n-k)`, where e is the number of errors and v the number of erasures.
+
+    The typical RSCoder is RSCoder(255, 223)
+
+RSCoder.encode(message, poly=False, k=None)
+    Encode a given string with reed-solomon encoding. Returns a byte
+    string with the k message bytes and n-k parity bytes at the end.
+
+    If a message is < k bytes long, it is assumed to be padded at the front
+    with null bytes (ie, a shortened Reed-Solomon code).
+
+    The sequence returned is always n bytes long.
+
+    If poly is not False, returns the encoded Polynomial object instead of
+    the polynomial translated back to a string (useful for debugging)
+
+    You can change the length (number) of parity/ecc bytes at encoding
+    by setting k to any value between [1, n-1]. This allows to create only
+    one RSCoder and then use it with a variable redundancy rate.
+
+RSCoder.encode_fast(message, poly=False, k=None)
+    Same as encode() but using faster algorithms and optimization tricks.
+
+RSCoder.decode(message_ecc, nostrip=False, k=None, erasures_pos=None, only_erasures=False):
+    Given a received string or byte array message_ecc (composed of
+    a message string + ecc symbols at the end), attempts to decode it.
+    If it's a valid codeword, or if there are no more than `2*e+v <= (n-k)` erratas
+    (called the Singleton bound), the message is returned.
+
+    You can provide the erasures positions as a list to erasures_pos.
+    For example, if you have "hella warld" and you know that `a` is an erasure,
+    you can provide the list erasures_pos=[4, 7]. You can correct twice as many
+    erasures than errors, and if some provided erasures are wrong (they are correct
+    symbols), then there's no problem, they will be repaired just fine (but will count
+    towards the Singleton bound). You can also specify that you are sure there are
+    only erasures and no errors at all by setting only_erasures=True.
+
+    A message always has k bytes, if a message contained less it is left
+    padded with null bytes (punctured RS code). When decoded, these leading
+    null bytes are stripped, but that can cause problems if decoding binary data.
+    When nostrip is True, messages returned are always k bytes long. This is
+    useful to make sure no data is lost when decoding binary data.
+
+    Note that RS can correct errors both in the message and the ecc symbols.
+
+RSCoder.decode_fast(message_ecc, nostrip=False, k=None, erasures_pos=None, only_erasures=False):
+    Same as decode() but using faster algorithms and optimization tricks.
+
+RSCoder.check(message_ecc, k=None)
+    Verifies the codeword (message + ecc symbols at the end) is valid by testing
+    that the code as a polynomial code divides g, or that the syndrome is
+    all 0 coefficients. The result is not foolproof: if it's False, you're sure the
+    message was corrupted (or that you used the wrong RS parameters),
+    but if it's True, it's either that the message is correct, or that there are
+    too many errors (ie, more than the Singleton bound) for RS to do anything about it.
+    returns True/False
+
+RSCoder.check_fast(message_ecc, k=None)
+    Same as check() but using faster algorithms and optimization tricks.
+
+unireedsolomon.ff.find_prime_polynomials(generator=2, c_exp=8, fast_primes=False, single=False)
+    Compute the list of prime polynomials for the given generator and
+    galois field characteristic exponent. You can then use this prime polynomial
+    to specify the mandatory "prim" parameter, particularly if you are using
+    a larger Galois Field (eg, 2^16).
+
+
+Internal API
+-------------
+Besides the main RSCoder object, two other objects are used in this
+implementation: Polynomial and GF2int. Their use is not specifically tied
+to the coder or even to the Reed-Solomon algorithm, they are just generic
+mathematical constructs respectively representing polynomials and
+Galois field's number of base 2.
+
+You do not need to know about the internal API to use the RS codec,
+this is just left as a documentation for the reader interested into dwelling
+inside the mathematical constructs.
+
+polynomial.Polynomial(coefficients=[], \**sparse)
+    There are three ways to initialize a Polynomial object.
+    1) With a list, tuple, or other iterable, creates a polynomial using
+    the items as coefficients in order of decreasing power
+
+    2) With keyword arguments such as for example x3=5, sets the
+    coefficient of x^3 to be 5
+
+    3) With no arguments, creates an empty polynomial, equivalent to
+    Polynomial([0])
+
+    >>> print Polynomial([5, 0, 0, 0, 0, 0])
+    5x^5
+
+    >>> print Polynomial(x32=5, x64=8)
+    8x^64 + 5x^32
+
+    >>> print Polynomial(x5=5, x9=4, x0=2) 
+    4x^9 + 5x^5 + 2
+
+Polynomial objects export the following standard functions that perform the
+expected operations using polynomial arithmetic. Arithmetic of the coefficients
+is determined by the type passed in, so integers or GF2int objects could be
+used, the Polynomial class is agnostic to the type of the coefficients.
+
+::
+
+    __add__
+    __divmod__
+    __eq__
+    __floordiv__
+    __hash__
+    __len__
+    __mod__
+    __mul__
+    __ne__
+    __neg__
+    __sub__
+    evaluate(x)
+    degree()
+        Returns the degree of the polynomial
+    get_coefficient(degree)
+        Returns the coefficient of the specified term
+
+ff.GF2int(value)
+    Instances of this object are elements of the field GF(2^p) and instances are integers
+    in the range 0 to `(2^p)-1`.
+    By default, the field is GF(2^8) and instances are integers in the range 0 to 255
+    and is defined using the irreducable polynomial 0x11b or in binary form:
+    x^8 + x^4 + x^3 + x + 1
+    and using 3 as the generator for the exponent table and log table.
+    
+    You can however use other parameters for the Galois Field, using the
+    init_lut() function.
+
+ff.find_prime_polynomials(generator=2, c_exp=8, fast_primes=False, single=False)
+    Find the list of prime polynomials to use to generate the look-up tables
+    for your field.
+
+ff.init_lut(generator=3, prim=0x11b, c_exp=8)
+    Generate the look-up tables given the parameters. This effectively parametrize
+    your Galois Field (ie, generator=2, prim=0x1002d, c_exp=16) will generate
+    a GF(2^16) field.
+
+The GF2int class inherits from int and supports all the usual integer
+operations. The following methods are overridden for arithmetic in the finite
+field GF(2^p)
+
+::
+
+    __add__
+    __div__
+    __mul__
+    __neg__
+    __pow__
+    __radd__
+    __rdiv__
+    __rmul__
+    __rsub__
+    __sub__
+    inverse()
+        Multiplicative inverse in GF(2^p)
+
+Edge cases
+-------------
+
+Although sanity checks are implemented whenever possible and when they are not too much resource consuming, there are a few cases where messages will not be decoded correctly without raising an exception:
+
+* If an incorrect erasure location is provided, the decoding algorithm will just trust the provided locations and create a syndrome that will be wrong, resulting in an incorrect decoded message. In case reliability is critical, always use the check() method after decoding to check the decoding did not go wrong.
+
+* Reed-Solomon algorithm is limited by the Singleton Bound, which limits not only its capacity to correct errors and erasures relatively to the number of error correction symbols, but also its ability to check if the message can be decoded or not. Indeed, if the number of errors and erasures are greater than the Singleton Bound, the decoder has no way to mathematically know for sure whether there is an error at all, it may very well be a valid message (although not the message you expect, but mathematically valid nevertheless). Hence, when the message is tampered beyond the Singleton Bound, the decoder may raise an exception, but it may also return a mathematically valid but still tampered message. Using the check() method cannot fix that either. To work around this issue, a solution is to use parity or hashing functions in parallel to the Reed-Solomon codec: use the Reed-Solomon codec to repair messages, use the parity or hashing function to check if there is any error. Due to how parity and hashing functions work, they are much less likely to produce a false negative than the Reed-Solomon algorithm. This is a general rule: error correction codes are efficient at correcting messages but not at detecting errors, hashing and parity functions are the adequate tool for this purpose.
+
+Example implementations
+-----------------------
+
+Image Encoder
+~~~~~~~~~~~~~
+imageencode.py is an example script that encodes codewords as rows in an image.
+It requires PIL to run.
+
+Usage: python imageencode.py [-d] <image file>
+
+Without the -d flag, imageencode.py will encode text from standard in and
+output it to the image file. With -d, imageencode.py will read in the data from
+the image and output to standard out the decoded text.
+
+An example is included: ``exampleimage.png``. Try decoding it as-is, then open
+it up in an image editor and paint some vertical stripes on it. As long as no
+more than 16 pixels per row are disturbed, the text will be decoded correctly.
+Then draw more stripes such that more than 16 pixels per row are disturbed and
+verify that the message is decoded improperly.
+
+Notice how the parity data looks different--the last 32 pixels of each row are
+colored differently. That's because this particular image contains encoded
+ASCII text, which generally only has bytes from a small range (the alphabet and
+printable punctuation). The parity data, however, is binary and contains bytes
+from the full range 0-255. Also note that either the data area or the parity
+area (or both!) can be disturbed as long as no more than 16 bytes per row are
+disturbed.
+
+Cython implementation
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+If either a C compiler or Cython is found, rs.py will automatically load the Cython implementations
+(the \*.pyx files).
+These are provided as optimized versions of the pure-python implementations, with equivalent
+functionalities. The goal was to get a speedup, which is the case, but using PyPy on the pure-python
+implementation provides a significantly higher speedup than the Cython implementation.
+The Cython implementations are still provided for the interested reader, but the casual user is
+not advised to use them. If you want to encode and decode fast, use PyPy.
+
+Projects using unireedsolomon
+-----------------------------
+
+* Several academic publications used unireedsolomon, see `this list <https://scholar.google.com/scholar?q=unireedsolomon>`_.
+
+Recommended reading
+-------------------
+
+* "`Reed-Solomon codes for coders <https://en.wikiversity.org/wiki/Reed%E2%80%93Solomon_codes_for_coders>`_", free practical beginner's tutorial with Python code examples on WikiVersity. Partially written by one of the authors of the present software.
+* "Algebraic codes for data transmission", Blahut, Richard E., 2003, Cambridge university press. `Readable online on Google Books <https://books.google.fr/books?id=eQs2i-R9-oYC&lpg=PR11&ots=atCPQJm3OJ&dq=%22Algebraic%20codes%20for%20data%20transmission%22%2C%20Blahut%2C%20Richard%20E.%2C%202003%2C%20Cambridge%20university%20press.&lr&hl=fr&pg=PA193#v=onepage&q=%22Algebraic%20codes%20for%20data%20transmission%22,%20Blahut,%20Richard%20E.,%202003,%20Cambridge%20university%20press.&f=false>`_. This book was pivotal in helping to understand the intricacies of the universal Berlekamp-Massey algorithm (see figures 7.5 and 7.10).
+
+Authors and licence
+-------------------
+Written from scratch by Andrew Brown <brownan@gmail.com> <brownan@cs.duke.edu>
+(c) 2010.
+
+Upgraded and maintained by Stephen Karl Larroque <LRQ3000@gmail.com> in 2015-2020.
+
+Licensed under the MIT License.
+
+
+.. |PyPI-Status| image:: https://img.shields.io/pypi/v/unireedsolomon.svg
+   :target: https://pypi.org/project/unireedsolomon
+.. |PyPI-Versions| image:: https://img.shields.io/pypi/pyversions/unireedsolomon.svg?logo=python&logoColor=white
+   :target: https://pypi.org/project/unireedsolomon
+.. |PyPI-Downloads| image:: https://img.shields.io/pypi/dm/unireedsolomon.svg?label=pypi%20downloads&logo=python&logoColor=white
+   :target: https://pypi.org/project/unireedsolomon
+.. |Build-Status| image:: https://github.com/lrq3000/unireedsolomon/actions/workflows/ci-build.yml/badge.svg?event=push
+    :target: https://github.com/lrq3000/unireedsolomon/actions/workflows/ci-build.yml
+.. |Coverage| image:: https://coveralls.io/repos/lrq3000/unireedsolomon/badge.svg?branch=master&service=github
+  :target: https://coveralls.io/github/lrq3000/unireedsolomon?branch=master
```

### Comparing `unireedsolomon-1.0.5/unireedsolomon.egg-info/SOURCES.txt` & `unireedsolomon-1.0.6/src/unireedsolomon.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 LICENSE.txt
 MANIFEST.in
 README.rst
 notes.txt
+pyproject.toml
 setup.py
-unireedsolomon/__init__.py
-unireedsolomon/_compat.py
-unireedsolomon/cff.pyx
-unireedsolomon/cpolynomial.pyx
-unireedsolomon/ff.py
-unireedsolomon/imageencode.py
-unireedsolomon/polynomial.py
-unireedsolomon/rs.py
-unireedsolomon.egg-info/PKG-INFO
-unireedsolomon.egg-info/SOURCES.txt
-unireedsolomon.egg-info/dependency_links.txt
-unireedsolomon.egg-info/top_level.txt
-unireedsolomon/tests/__init__.py
-unireedsolomon/tests/test_cff.py
-unireedsolomon/tests/test_cpolynomial.py
-unireedsolomon/tests/test_ff.py
-unireedsolomon/tests/test_polynomial.py
-unireedsolomon/tests/test_rs.py
+src/unireedsolomon/__init__.py
+src/unireedsolomon/_compat.py
+src/unireedsolomon/cff.c
+src/unireedsolomon/cff.pyx
+src/unireedsolomon/cpolynomial.c
+src/unireedsolomon/cpolynomial.pyx
+src/unireedsolomon/ff.py
+src/unireedsolomon/imageencode.py
+src/unireedsolomon/polynomial.py
+src/unireedsolomon/rs.py
+src/unireedsolomon.egg-info/PKG-INFO
+src/unireedsolomon.egg-info/SOURCES.txt
+src/unireedsolomon.egg-info/dependency_links.txt
+src/unireedsolomon.egg-info/requires.txt
+src/unireedsolomon.egg-info/top_level.txt
+src/unireedsolomon/tests/__init__.py
+src/unireedsolomon/tests/test_cff.py
+src/unireedsolomon/tests/test_cpolynomial.py
+src/unireedsolomon/tests/test_ff.py
+src/unireedsolomon/tests/test_polynomial.py
+src/unireedsolomon/tests/test_rs.py
```

