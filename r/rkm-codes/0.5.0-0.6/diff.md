# Comparing `tmp/rkm_codes-0.5.0.tar.gz` & `tmp/rkm_codes-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rkm_codes-0.5.0.tar", last modified: Wed Mar  4 06:53:35 2020, max compression
+gzip compressed data, was "rkm_codes-0.6.tar", last modified: Fri Apr 14 23:38:59 2023, max compression
```

## Comparing `rkm_codes-0.5.0.tar` & `rkm_codes-0.6.tar`

### file list

```diff
@@ -1,15 +1,5 @@
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2020-03-04 06:53:35.275826 rkm_codes-0.5.0/
--rw-rw-r--   0 ken       (1000) ken       (1000)    16738 2020-03-04 06:53:35.274826 rkm_codes-0.5.0/PKG-INFO
--rw-rw-r--   0 ken       (1000) ken       (1000)    12864 2020-03-04 06:51:29.000000 rkm_codes-0.5.0/README.rst
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2020-03-04 06:53:35.274826 rkm_codes-0.5.0/rkm_codes/
--rw-rw-r--   0 ken       (1000) ken       (1000)      162 2020-03-04 06:51:29.000000 rkm_codes-0.5.0/rkm_codes/__init__.py
--rw-rw-r--   0 ken       (1000) ken       (1000)    12953 2020-03-04 06:51:29.000000 rkm_codes-0.5.0/rkm_codes/rkm_codes.py
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2020-03-04 06:53:35.274826 rkm_codes-0.5.0/rkm_codes.egg-info/
--rw-rw-r--   0 ken       (1000) ken       (1000)    16738 2020-03-04 06:53:35.000000 rkm_codes-0.5.0/rkm_codes.egg-info/PKG-INFO
--rw-rw-r--   0 ken       (1000) ken       (1000)      256 2020-03-04 06:53:35.000000 rkm_codes-0.5.0/rkm_codes.egg-info/SOURCES.txt
--rw-rw-r--   0 ken       (1000) ken       (1000)        1 2020-03-04 06:53:35.000000 rkm_codes-0.5.0/rkm_codes.egg-info/dependency_links.txt
--rw-rw-r--   0 ken       (1000) ken       (1000)       15 2020-03-04 06:53:35.000000 rkm_codes-0.5.0/rkm_codes.egg-info/requires.txt
--rw-rw-r--   0 ken       (1000) ken       (1000)       10 2020-03-04 06:53:35.000000 rkm_codes-0.5.0/rkm_codes.egg-info/top_level.txt
--rw-rw-r--   0 ken       (1000) ken       (1000)        1 2020-03-04 06:53:35.000000 rkm_codes-0.5.0/rkm_codes.egg-info/zip-safe
--rw-rw-r--   0 ken       (1000) ken       (1000)       38 2020-03-04 06:53:35.275826 rkm_codes-0.5.0/setup.cfg
--rw-rw-r--   0 ken       (1000) ken       (1000)     1456 2020-03-04 06:53:28.000000 rkm_codes-0.5.0/setup.py
+-rw-r--r--   0        0        0    13372 2023-04-14 23:37:47.564116 rkm_codes-0.6/README.rst
+-rw-r--r--   0        0        0      858 2023-04-14 23:33:06.181170 rkm_codes-0.6/pyproject.toml
+-rw-r--r--   0        0        0      160 2023-04-14 23:33:06.184170 rkm_codes-0.6/rkm_codes/__init__.py
+-rw-r--r--   0        0        0    13130 2023-04-14 23:33:06.183170 rkm_codes-0.6/rkm_codes/rkm_codes.py
+-rw-r--r--   0        0        0    14136 1970-01-01 00:00:00.000000 rkm_codes-0.6/PKG-INFO
```

### Comparing `rkm_codes-0.5.0/PKG-INFO` & `rkm_codes-0.6/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,396 +1,405 @@
 Metadata-Version: 2.1
 Name: rkm_codes
-Version: 0.5.0
+Version: 0.6
 Summary: QuantiPhy support for RKM codes.
-Home-page: https://nurdletech.com/linux-utilities/rkm_codes
+Keywords: quantiphy,rkm
 Author: Ken Kundert
 Author-email: rkm_codes@nurdletech.com
-License: GPLv3+
-Download-URL: https://github.com/kenkundert/rkm_codes/tarball/master
-Description: .. initialize RKM codes
-        
-            >>> from rkm_codes import set_prefs
-            >>> set_prefs(
-            ...     rkm_maps=None, units_to_rkm_base_code=None, map_sf=None,
-            ...     show_units=None, strip_zeros=None, minus_sign=None, prec=None
-            ... )
-        
-        RKM codes
-        =========
-        
-        | Version: 0.5.0
-        | Released: 2020-03-03
-        |
-        
-        .. image:: https://img.shields.io/travis/KenKundert/rkm_codes/master.svg
-            :target: https://travis-ci.org/KenKundert/rkm_codes
-        
-        .. image:: https://img.shields.io/coveralls/KenKundert/rkm_codes.svg
-            :target: https://coveralls.io/r/KenKundert/rkm_codes
-        
-        .. image:: https://img.shields.io/pypi/v/rkm_codes.svg
-            :target: https://pypi.python.org/pypi/rkm_codes
-        
-        .. image:: https://img.shields.io/pypi/pyversions/rkm_codes.svg
-            :target: https://pypi.python.org/pypi/rkm_codes/
-        
-        RKM codes are used to represent electrical quantities in labels, particularly on
-        schematics and on the components themselves.  They are standardized in various
-        national and international standards, including: IEC 60062 (1952) (formerly IEC 62),
-        DIN 40825 (1973), BS 1852 (1974), IS 8186 (1976) and EN 60062 (1993).
-        IEC-60062 was significantly updated in 2016.
-        
-        RKM codes were originally used as part marking codes.  This shorthand
-        notation is widely used in electrical engineering to denote the values of
-        resistors and capacitors in circuit diagrams and in the production of electronic
-        circuits (for example in bills of material and in silk screens). This method
-        avoids overlooking the decimal separator, which may not be rendered reliably on
-        components or when duplicating documents.  They also provide the benefit that
-        the characters within a RKM code are either letters or digits, and so can be
-        embedded within identifiers without introducing invalid characters.
-        
-        IEC 60062 is described in https://en.wikipedia.org/wiki/RKM_code.
-        
-        Essentially an RKM version of a number is the number with a scale factor where
-        the decimal point replaced by the scale factor. For example, a resistance of
-        4.7kΩ becomes 4k7. If there is no scale factor, the decimal point is replaced by
-        a letter that signifies the type of the component.  For example, a resistance of
-        4.7Ω becomes 4r7.
-        
-        Resistance examples:
-        
-            | R47 → 0.47 Ω
-            | 4R7 → 4.7 Ω
-            | 470R → 470 Ω
-            | 4K7 → 4.7 kΩ
-            | 47K → 47 kΩ
-            | 47K3 → 47.3 kΩ
-            | 470K → 470 kΩ
-            | 4M7 → 4.7 MΩ
-        
-        In the standard, large values are assumed to be resistances and small values are
-        assumed to be capacitances.  So 4k7 is a resistance and 2n5 is a capacitance.
-        However, this package also supports a version of RKM codes where the units are
-        not implied by the value, making RKM codes suitable for a wider variety of value
-        types, such as voltage, current, and inductance.
-        
-        
-        Installing
-        ----------
-        
-        This package converts RKM codes to `QuantiPhy Quantities
-        <https://quantiphy.readthedocs.io>`_ and Quantities to RKM codes.
-        
-        Install with::
-        
-            pip3 install --user rkm_codes
-        
-        Requires Python3.4 or better.
-        
-        
-        Converting to and from RKM Codes
-        --------------------------------
-        
-        The following is a simple example of how to convert back and forth between RKM
-        codes and Quantities::
-        
-            >>> from rkm_codes import from_rkm, to_rkm
-            >>> r = from_rkm('6K8')
-            >>> r
-            Quantity('6.8k')
-        
-            >>> to_rkm(r)
-            '6K8'
-        
-        Notice that in this case the quantity does not include units. That is because by
-        default *rkm_codes* assumes unitless numbers. You can change this behavior.  Out
-        of the box *rkm_codes* supports two kinds of numbers, unitless and those that
-        follow the IEC60062 standard. You can switch between those two kinds of numbers
-        using something like this::
-        
-            >>> from rkm_codes import set_prefs, IEC60062_MAPS, UNITLESS_MAPS
-            >>> r = from_rkm('6k8')
-            >>> r
-            Quantity('6.8k')
-        
-            >>> set_prefs(rkm_maps=IEC60062_MAPS)
-            >>> from_rkm('6k8')
-            Quantity('6.8 kΩ')
-        
-            >>> set_prefs(rkm_maps=UNITLESS_MAPS)
-            >>> from_rkm('6k8')
-            Quantity('6.8k')
-        
-        In either case, *rkm_codes* allows you to explicitly specify the units, which
-        always overrides any implied units::
-        
-            >>> set_prefs(rkm_maps=UNITLESS_MAPS)
-            >>> from_rkm('6kΩ8')
-            Quantity('6.8 kΩ')
-        
-            >>> i = from_rkm('2uA5')
-            >>> i
-            Quantity('2.5 uA')
-        
-        The primary argument for *to_rkm* can be a string, a float, or a quantity::
-        
-            >>> print(to_rkm('12.5 nA', prec=2))
-            12n5
-        
-            >>> print(to_rkm(12.5e-9, prec=2))
-            12n5
-        
-            >>> from quantiphy import Quantity
-            >>> print(to_rkm(Quantity('12.5 nA'), prec=2))
-            12n5
-        
-        When converting to an RKM code, you can instruct that the units be included::
-        
-            >>> to_rkm(i, show_units=True)
-            '2µA5'
-        
-        You can also indicate how many digits should be included::
-        
-            >>> to_rkm(i.add(1e-9), prec=5, show_units=True)
-            '2µA501'
-        
-        Normally, any excess zeros are removed, but you can change that too::
-        
-            >>> to_rkm(i.add(1e-9), prec=5, show_units=True, strip_zeros=False)
-            '2µA50100'
-        
-        To shorten the output code it is possible to remove the base code when it is
-        extraneous::
-        
-            >>> from quantiphy import Quantity
-            >>> to_rkm(Quantity('470Ω'), show_units=False)
-            '470'
-        
-            >>> to_rkm(Quantity('470Ω'), show_units=False, strip_code=False)
-            '470r'
-        
-        Here is a short program that illustrates some of the options of *to_rkm*::
-        
-            >>> from rkm_codes import from_rkm, to_rkm, set_prefs, IEC60062_MAPS
-        
-            >>> set_prefs(prec=4)
-        
-            >>> q = from_rkm('0μΩ47')
-            >>> while q < 1e6:
-            ...     vals = [
-            ...         q,
-            ...         to_rkm(q),
-            ...         to_rkm(q, strip_code=False),
-            ...         to_rkm(q, show_units=True),
-            ...         to_rkm(q, strip_zeros=False)
-            ...     ]
-            ...     print(' '.join(['  {:<9}'.format(v) for v in vals]).strip())
-            ...     q = q.scale(10)
-            470 nΩ      470n        470n        470nΩ       470n00
-            4.7 uΩ      4µ7         4µ7         4µΩ7        4µ7000
-            47 uΩ       47µ         47µ         47µΩ        47µ000
-            470 uΩ      470µ        470µ        470µΩ       470µ00
-            4.7 mΩ      4m7         4m7         4mΩ7        4m7000
-            47 mΩ       47m         47m         47mΩ        47m000
-            470 mΩ      470m        470m        470mΩ       470m00
-            4.7 Ω       4r7         4r7         4Ω7         4r7000
-            47 Ω        47          47r         47Ω         47r000
-            470 Ω       470         470r        470Ω        470r00
-            4.7 kΩ      4K7         4K7         4KΩ7        4K7000
-            47 kΩ       47K         47K         47KΩ        47K000
-            470 kΩ      470K        470K        470KΩ       470K00
-        
-        If you prefer not to use the small SI scale factors, which would be more in
-        keeping with IEC60062 for resistors, you can specify that ``quantiphy.Quantity``
-        use a restricted ``output_sf``::
-        
-            >>> q = from_rkm('0μΩ47')
-            >>> q.output_sf = 'TGMk'   # this line is new
-            >>> while q < 1e6:
-            ...     vals = [
-            ...         q,
-            ...         to_rkm(q),
-            ...         to_rkm(q, strip_code=False),
-            ...         to_rkm(q, show_units=True),
-            ...         to_rkm(q, strip_zeros=False)
-            ...     ]
-            ...     print(' '.join(['  {:<9}'.format(v) for v in vals]).strip())
-            ...     q = q.scale(10)
-            470e-9 Ω    0           0r          0Ω          r0000
-            4.7e-6 Ω    0           0r          0Ω          r0000
-            47e-6 Ω     0           0r          0Ω          r0000
-            470e-6 Ω    r0005       r0005       Ω0005       r0005
-            4.7e-3 Ω    r0047       r0047       Ω0047       r0047
-            47e-3 Ω     r047        r047        Ω047        r0470
-            470e-3 Ω    r47         r47         Ω47         r4700
-            4.7 Ω       4r7         4r7         4Ω7         4r7000
-            47 Ω        47          47r         47Ω         47r000
-            470 Ω       470         470r        470Ω        470r00
-            4.7 kΩ      4K7         4K7         4KΩ7        4K7000
-            47 kΩ       47K         47K         47KΩ        47K000
-            470 kΩ      470K        470K        470KΩ       470K00
-        
-        You can create your own maps by passing in a dictionary that maps a RKM base
-        code character into a scale factor and units. For example, you could create
-        a map that uses 'd' or 'D' to represent the decimal point in numbers without
-        scale factors rather than 'r', 'c', etc.  For example::
-        
-            >>> set_prefs(rkm_maps=dict(d=('', ''), D=('', '')))
-            >>> from_rkm('6d8')
-            Quantity('6.8')
-        
-            >>> from_rkm('2d5')
-            Quantity('2.5')
-        
-        Passing *None* for the value of a map returns it to its default value.
-        
-        If *rkm_codes* encounters a RKM base code character that is not in the map, it
-        simply uses that character. In this way, scale factors are handled::
-        
-            >>> from_rkm('6k8')
-            Quantity('6.8k')
-        
-        When converting from Quantities to RKM codes, you can override the default
-        mappings from units to RKM base code characters. The default mapping maps 'Ω'
-        and 'Ohm' to 'r', 'F' to 'c', 'H' to 'l', 'V' to 'v', and 'A' to 'i'.  However,
-        you may prefer uppercase base characters, which is more in alignment with the
-        original standard. To get that, you can use something like this::
-        
-            >>> rkm_base_code_mappings = {
-            ...     'Ω': 'R',
-            ...     'Ohm': 'R',
-            ...     'F': 'C',
-            ...     'H': 'L',
-            ...     'V': 'V',
-            ...     'A': 'I',
-            ... }
-            >>> set_prefs(rkm_maps=IEC60062_MAPS, units_to_rkm_base_code=rkm_base_code_mappings)
-            >>> r = from_rkm('k0012')
-            >>> to_rkm(r)
-            '1R2'
-        
-        You can control the scale factors used by to_rkm() by setting *map_sf* using
-        *set_prefs*. The default maps 'u' to 'μ' and 'k' to 'K'. You might wish to
-        prevent the use of 'μ' while retaining the use of 'K', which you can do with::
-        
-            >>> set_prefs(map_sf=dict(u='µ'))
-            >>> c = from_rkm('5u')
-            >>> to_rkm(c)
-            '5µ'
-        
-        
-        Finding RKM Codes
-        -----------------
-        
-        *find_rkm* is available for finding the RKM codes embedded in text strings.
-        Using it, you can iterate through all the numbers specified using RKM:
-        
-            >>> from rkm_codes import find_rkm
-        
-            >>> text = '''
-            ...     An RKM code that may include explicitly specified. Examples of
-            ...     acceptable RKM codes for resistance include:   R47 (0.47 Ω), 4R7
-            ...     (4.7 Ω), 470R (470 Ω), 4K7 (4.7 kΩ), 47K (47 kΩ), 47K3 (47.3 kΩ),
-            ...     470K (470 kΩ), and 4M7 (4.7 MΩ).
-            ... '''
-            >>> for num in find_rkm(text):
-            ...     print(num)
-            470 mΩ
-            4.7 Ω
-            470 Ω
-            4.7 kΩ
-            47 kΩ
-            47.3 kΩ
-            470 kΩ
-            4.7 MΩ
-        
-        When the RKM code is not isolated by punctuation or spaces it can get confused
-        by leading and trailing text.  You can often resolve this issue by restricting
-        the matches to either the leading or trailing digit forms of the RKM code. Do so
-        by specifying either 'ld' or 'td' as a second argument.  For example:
-        
-            >>> for num in find_rkm('sink200nA'):
-            ...     print(num)
-            200 msink
-        
-            >>> for num in find_rkm('sink200nA', 'ld'):
-            ...     print(num)
-            200 nA
-        
-        
-        Pin Name Generator Example
-        --------------------------
-        
-        As a practical example of the use of RKM codes, imagine wanting a program that
-        creates pin names for an electrical circuit based on a naming convention.  It
-        would take a table of pin characteristics that are used to create the names.
-        For example::
-        
-            >>> from quantiphy import Quantity
-            >>> from rkm_codes import to_rkm, set_prefs as set_rkm_prefs
-        
-            >>> pins = [
-            ...     dict(kind='ibias', direction='out', polarity='sink', dest='dac', value='250nA'),
-            ...     dict(kind='ibias', direction='out', polarity='src', dest='rampgen', value='2.5μA'),
-            ...     dict(kind='vref', direction='out', dest='dac', value='1.25V'),
-            ...     dict(kind='vdda', direction='in', value='2.5V'),
-            ... ]
-            >>> set_rkm_prefs(map_sf={}, units_to_rkm_base_code=None, show_units=True, prec=2)
-        
-            >>> for pin in pins:
-            ...     components = []
-            ...     if 'value' in pin:
-            ...         pin['VALUE'] = to_rkm(Quantity(pin['value']))
-            ...     for name in ['dest', 'kind', 'direction', 'VALUE', 'polarity']:
-            ...         if name in pin:
-            ...             components.append(pin[name])
-            ...     print('_'.join(components))
-            dac_ibias_out_250nA_sink
-            rampgen_ibias_out_2uA5_src
-            dac_vref_out_1V25
-            vdda_in_2V5
-        
-        
-        Releases
-        --------
-        
-        **Latest development release**:
-            | Version: 0.5.0
-            | Released: 2020-03-03
-        
-        **0.5 (2020-02-01)**:
-            - Allow argument to *to_rkm()* to be a string or simple number
-            - Added *strip_code* preference
-            - With small numbers show 0 rather than exponent
-        
-        **0.4 (2019-08-29)**:
-            - added *find_rkm()*
-        
-        **0.3 (2019-08-23)**:
-            - move the units to the middle of the number with the scale factor
-            - added support for signed numbers
-            - added *show_units*, *strip_zeros*, *minus_sign*, and *prec* to preferences
-            - this release is not backward compatible; units at the end of the number
-              are no longer supported
-        
-        **0.2 (2018-09-14)**:
-            - fixed issue in *set_prefs()*
-        
-        **0.1 (2018-09-12)**:
-            - initial release
-        
-        
-        
-Keywords: rkm codes,quantiphy
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
+Requires-Python: >=3.6
+Description-Content-Type: text/x-rst
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Utilities
-Description-Content-Type: text/x-rst
+Requires-Dist: quantiphy>=2.4
+Project-URL: changelog, https://emborg.readthedocs.io/en/latest/releases.html
+Project-URL: repository, https://github.com/kenkundert/rkm_codes
+
+.. initialize RKM codes
+
+    >>> from rkm_codes import set_prefs
+    >>> set_prefs(
+    ...     rkm_maps=None, units_to_rkm_base_code=None, map_sf=None,
+    ...     show_units=None, strip_zeros=None, minus_sign=None, prec=None
+    ... )
+
+RKM codes
+=========
+
+| Version: 0.6
+| Released: 2023-04-14
+|
+
+.. image:: https://pepy.tech/badge/rkm_codes/month
+    :target: https://pepy.tech/project/rkm_codes
+
+..  image:: https://github.com/KenKundert/rkm_codes/actions/workflows/build.yaml/badge.svg
+    :target: https://github.com/KenKundert/rkm_codes/actions/workflows/build.yaml
+
+.. image:: https://img.shields.io/coveralls/KenKundert/rkm_codes.svg
+    :target: https://coveralls.io/r/KenKundert/rkm_codes
+
+.. image:: https://img.shields.io/pypi/v/rkm_codes.svg
+    :target: https://pypi.python.org/pypi/rkm_codes
+
+.. image:: https://img.shields.io/pypi/pyversions/rkm_codes.svg
+    :target: https://pypi.python.org/pypi/rkm_codes/
+
+RKM codes are used to represent electrical quantities in labels, particularly on
+schematics and on the components themselves.  They are standardized in various
+national and international standards, including: IEC 60062 (1952) (formerly IEC 62),
+DIN 40825 (1973), BS 1852 (1974), IS 8186 (1976) and EN 60062 (1993).
+IEC-60062 was significantly updated in 2016.
+
+RKM codes were originally used as part marking codes.  This shorthand
+notation is widely used in electrical engineering to denote the values of
+resistors and capacitors in circuit diagrams and in the production of electronic
+circuits (for example in bills of material and in silk screens). This method
+avoids overlooking the decimal separator, which may not be rendered reliably on
+components or when duplicating documents.
+
+The popularity of RKM codes was fading because they address a problem that is 
+less common today. However they are making something of a come back as all the 
+characters in a RKM code are either letters or digits and so they can be 
+embedded in a software identifier without introducing illegal characters.
+
+IEC 60062 is described in https://en.wikipedia.org/wiki/RKM_code.
+
+Essentially an RKM version of a number is the number with a scale factor where
+the decimal point is replaced by the scale factor. For example, a resistance of
+4.7kΩ becomes 4k7. If there is no scale factor, the decimal point is replaced by
+a letter that signifies the type of the component.  For example, a resistance of
+4.7Ω becomes 4r7.
+
+Resistance examples::
+
+    R47 → 0.47 Ω
+    4R7 → 4.7 Ω
+    470R → 470 Ω
+    4K7 → 4.7 kΩ
+    47K → 47 kΩ
+    47K3 → 47.3 kΩ
+    470K → 470 kΩ
+    4M7 → 4.7 MΩ
+
+In the standard, large values are assumed to be resistances and small values are
+assumed to be capacitances.  So 4k7 is a resistance and 2n5 is a capacitance.
+However, this package also supports a version of RKM codes where the units are
+not implied by the value, making RKM codes suitable for a wider variety of value
+types, such as voltage, current, and inductance.
+
+
+Installing
+----------
+
+This package converts RKM codes to `QuantiPhy Quantities
+<https://quantiphy.readthedocs.io>`_ and Quantities to RKM codes.
+
+Install with::
+
+    pip3 install --user rkm_codes
+
+Requires Python 3.6 or better.
+
+
+Converting to and from RKM Codes
+--------------------------------
+
+The following is a simple example of how to convert back and forth between RKM
+codes and Quantities::
+
+    >>> from rkm_codes import from_rkm, to_rkm
+    >>> r = from_rkm('6K8')
+    >>> r
+    Quantity('6.8k')
+
+    >>> to_rkm(r)
+    '6K8'
+
+Notice that in this case the quantity does not include units. That is because by
+default *rkm_codes* assumes unitless numbers. You can change this behavior.  Out
+of the box *rkm_codes* supports two kinds of numbers, unitless and those that
+follow the IEC60062 standard. You can switch between those two kinds of numbers
+using something like this::
+
+    >>> from rkm_codes import set_prefs, IEC60062_MAPS, UNITLESS_MAPS
+    >>> r = from_rkm('6k8')
+    >>> r
+    Quantity('6.8k')
+
+    >>> set_prefs(rkm_maps=IEC60062_MAPS)
+    >>> from_rkm('6k8')
+    Quantity('6.8 kΩ')
+
+    >>> set_prefs(rkm_maps=UNITLESS_MAPS)
+    >>> from_rkm('6k8')
+    Quantity('6.8k')
+
+In either case, *rkm_codes* allows you to explicitly specify the units, which
+always overrides any implied units::
+
+    >>> set_prefs(rkm_maps=UNITLESS_MAPS)
+    >>> from_rkm('6kΩ8')
+    Quantity('6.8 kΩ')
+
+    >>> i = from_rkm('2uA5')
+    >>> i
+    Quantity('2.5 uA')
+
+The primary argument for *to_rkm* can be a string, a float, or a quantity::
+
+    >>> print(to_rkm('12.5 nA', prec=2))
+    12n5
+
+    >>> print(to_rkm(12.5e-9, prec=2))
+    12n5
+
+    >>> from quantiphy import Quantity
+    >>> print(to_rkm(Quantity('12.5 nA'), prec=2))
+    12n5
+
+When converting to an RKM code, you can instruct that the units be included::
+
+    >>> to_rkm(i, show_units=True)
+    '2µA5'
+
+You can also indicate how many digits should be included::
+
+    >>> to_rkm(i.add(1e-9), prec=5, show_units=True)
+    '2µA501'
+
+Normally, any excess zeros are removed, but you can change that too::
+
+    >>> to_rkm(i.add(1e-9), prec=5, show_units=True, strip_zeros=False)
+    '2µA50100'
+
+To shorten the output code it is possible to remove the base code when it is
+extraneous::
+
+    >>> from quantiphy import Quantity
+    >>> to_rkm(Quantity('470Ω'), show_units=False)
+    '470'
+
+    >>> to_rkm(Quantity('470Ω'), show_units=False, strip_code=False)
+    '470r'
+
+Here is a short program that illustrates some of the options of *to_rkm*::
+
+    >>> from rkm_codes import from_rkm, to_rkm, set_prefs, IEC60062_MAPS
+
+    >>> set_prefs(prec=4)
+
+    >>> q = from_rkm('0μΩ47')
+    >>> while q < 1e6:
+    ...     vals = [
+    ...         q,
+    ...         to_rkm(q),
+    ...         to_rkm(q, strip_code=False),
+    ...         to_rkm(q, show_units=True),
+    ...         to_rkm(q, strip_zeros=False)
+    ...     ]
+    ...     print(' '.join(['  {:<9}'.format(v) for v in vals]).strip())
+    ...     q = q.scale(10)
+    470 nΩ      470n        470n        470nΩ       470n00
+    4.7 uΩ      4µ7         4µ7         4µΩ7        4µ7000
+    47 uΩ       47µ         47µ         47µΩ        47µ000
+    470 uΩ      470µ        470µ        470µΩ       470µ00
+    4.7 mΩ      4m7         4m7         4mΩ7        4m7000
+    47 mΩ       47m         47m         47mΩ        47m000
+    470 mΩ      470m        470m        470mΩ       470m00
+    4.7 Ω       4r7         4r7         4Ω7         4r7000
+    47 Ω        47          47r         47Ω         47r000
+    470 Ω       470         470r        470Ω        470r00
+    4.7 kΩ      4K7         4K7         4KΩ7        4K7000
+    47 kΩ       47K         47K         47KΩ        47K000
+    470 kΩ      470K        470K        470KΩ       470K00
+
+If you prefer not to use the small SI scale factors, which would be more in
+keeping with IEC60062 for resistors, you can specify that ``quantiphy.Quantity``
+use a restricted ``output_sf``::
+
+    >>> q = from_rkm('0μΩ47')
+    >>> q.output_sf = 'TGMk'   # this line is new
+    >>> while q < 1e6:
+    ...     vals = [
+    ...         q,
+    ...         to_rkm(q),
+    ...         to_rkm(q, strip_code=False),
+    ...         to_rkm(q, show_units=True),
+    ...         to_rkm(q, strip_zeros=False)
+    ...     ]
+    ...     print(' '.join(['  {:<9}'.format(v) for v in vals]).strip())
+    ...     q = q.scale(10)
+    470e-9 Ω    0           0r          0Ω          r0000
+    4.7e-6 Ω    0           0r          0Ω          r0000
+    47e-6 Ω     0           0r          0Ω          r0000
+    470e-6 Ω    r0005       r0005       Ω0005       r0005
+    4.7e-3 Ω    r0047       r0047       Ω0047       r0047
+    47e-3 Ω     r047        r047        Ω047        r0470
+    470e-3 Ω    r47         r47         Ω47         r4700
+    4.7 Ω       4r7         4r7         4Ω7         4r7000
+    47 Ω        47          47r         47Ω         47r000
+    470 Ω       470         470r        470Ω        470r00
+    4.7 kΩ      4K7         4K7         4KΩ7        4K7000
+    47 kΩ       47K         47K         47KΩ        47K000
+    470 kΩ      470K        470K        470KΩ       470K00
+
+You can create your own maps by passing in a dictionary that maps a RKM base
+code character into a scale factor and units. For example, you could create
+a map that uses 'd' or 'D' to represent the decimal point in numbers without
+scale factors rather than 'r', 'c', etc.  For example::
+
+    >>> set_prefs(rkm_maps=dict(d=('', ''), D=('', '')))
+    >>> from_rkm('6d8')
+    Quantity('6.8')
+
+    >>> from_rkm('2d5')
+    Quantity('2.5')
+
+Passing *None* for the value of a map returns it to its default value.
+
+If *rkm_codes* encounters a RKM base code character that is not in the map, it
+simply uses that character. In this way, scale factors are handled::
+
+    >>> from_rkm('6k8')
+    Quantity('6.8k')
+
+When converting from Quantities to RKM codes, you can override the default
+mappings from units to RKM base code characters. The default mapping maps 'Ω'
+and 'Ohm' to 'r', 'F' to 'c', 'H' to 'l', 'V' to 'v', and 'A' to 'i'.  However,
+you may prefer uppercase base characters, which is more in alignment with the
+original standard. To get that, you can use something like this::
+
+    >>> rkm_base_code_mappings = {
+    ...     'Ω': 'R',
+    ...     'Ohm': 'R',
+    ...     'F': 'C',
+    ...     'H': 'L',
+    ...     'V': 'V',
+    ...     'A': 'I',
+    ... }
+    >>> set_prefs(rkm_maps=IEC60062_MAPS, units_to_rkm_base_code=rkm_base_code_mappings)
+    >>> r = from_rkm('k0012')
+    >>> to_rkm(r)
+    '1R2'
+
+You can control the scale factors used by to_rkm() by setting *map_sf* using
+*set_prefs*. The default maps 'u' to 'μ' and 'k' to 'K'. You might wish to
+prevent the use of 'μ' while retaining the use of 'K', which you can do with::
+
+    >>> set_prefs(map_sf=dict(u='µ'))
+    >>> c = from_rkm('5u')
+    >>> to_rkm(c)
+    '5µ'
+
+
+Finding RKM Codes
+-----------------
+
+*find_rkm* is available for finding the RKM codes embedded in text strings.
+Using it, you can iterate through all the numbers specified using RKM::
+
+    >>> from rkm_codes import find_rkm
+
+    >>> text = '''
+    ...     An RKM code that may include explicitly specified. Examples of
+    ...     acceptable RKM codes for resistance include:   R47 (0.47 Ω), 4R7
+    ...     (4.7 Ω), 470R (470 Ω), 4K7 (4.7 kΩ), 47K (47 kΩ), 47K3 (47.3 kΩ),
+    ...     470K (470 kΩ), and 4M7 (4.7 MΩ).
+    ... '''
+    >>> for num in find_rkm(text):
+    ...     print(num)
+    470 mΩ
+    4.7 Ω
+    470 Ω
+    4.7 kΩ
+    47 kΩ
+    47.3 kΩ
+    470 kΩ
+    4.7 MΩ
+
+When the RKM code is not isolated by punctuation or spaces it can get confused
+by leading and trailing text.  You can often resolve this issue by restricting
+the matches to either the leading or trailing digit forms of the RKM code. Do so
+by specifying either 'ld' or 'td' as a second argument.  For example::
+
+    >>> for num in find_rkm('sink200nA'):
+    ...     print(num)
+    200 msink
+
+    >>> for num in find_rkm('sink200nA', 'ld'):
+    ...     print(num)
+    200 nA
+
+
+Pin Name Generator Example
+--------------------------
+
+As a practical example of the use of RKM codes, imagine wanting a program that
+creates pin names for an electrical circuit based on a naming convention.  It
+would take a table of pin characteristics that are used to create the names.
+For example::
+
+    >>> from quantiphy import Quantity
+    >>> from rkm_codes import to_rkm, set_prefs as set_rkm_prefs
+
+    >>> pins = [
+    ...     dict(kind='ibias', direction='out', polarity='sink', dest='dac', value='250nA'),
+    ...     dict(kind='ibias', direction='out', polarity='src', dest='rampgen', value='2.5μA'),
+    ...     dict(kind='vref', direction='out', dest='dac', value='1.25V'),
+    ...     dict(kind='vdda', direction='in', value='2.5V'),
+    ... ]
+    >>> set_rkm_prefs(map_sf={}, units_to_rkm_base_code=None, show_units=True, prec=2)
+
+    >>> for pin in pins:
+    ...     components = []
+    ...     if 'value' in pin:
+    ...         pin['VALUE'] = to_rkm(Quantity(pin['value']))
+    ...     for name in ['dest', 'kind', 'direction', 'VALUE', 'polarity']:
+    ...         if name in pin:
+    ...             components.append(pin[name])
+    ...     print('_'.join(components))
+    dac_ibias_out_250nA_sink
+    rampgen_ibias_out_2uA5_src
+    dac_vref_out_1V25
+    vdda_in_2V5
+
+
+Releases
+--------
+
+**Latest development release**:
+    | Version: 0.6
+    | Released: 2023-04-14
+
+**0.6 (2023-04-14)**:
+    - Suppress *rkm_code*’s use of the new SI scale factors in `QuantiPhy 
+      <https://quantiphy.readthedocs.io>`_ so that ``R`` is no longer treated as 
+      a scale factor when using the latest version of *QuantiPhy*.
+
+**0.5 (2020-02-01)**:
+    - Allow argument to *to_rkm()* to be a string or simple number
+    - Added *strip_code* preference
+    - With small numbers show 0 rather than exponent
+
+**0.4 (2019-08-29)**:
+    - added *find_rkm()*
+
+**0.3 (2019-08-23)**:
+    - move the units to the middle of the number with the scale factor
+    - added support for signed numbers
+    - added *show_units*, *strip_zeros*, *minus_sign*, and *prec* to preferences
+    - this release is not backward compatible; units at the end of the number
+      are no longer supported
+
+**0.2 (2018-09-14)**:
+    - fixed issue in *set_prefs()*
+
+**0.1 (2018-09-12)**:
+    - initial release
+
+
+
```

### Comparing `rkm_codes-0.5.0/README.rst` & `rkm_codes-0.6/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -5,20 +5,23 @@
     ...     rkm_maps=None, units_to_rkm_base_code=None, map_sf=None,
     ...     show_units=None, strip_zeros=None, minus_sign=None, prec=None
     ... )
 
 RKM codes
 =========
 
-| Version: 0.5.0
-| Released: 2020-03-03
+| Version: 0.6
+| Released: 2023-04-14
 |
 
-.. image:: https://img.shields.io/travis/KenKundert/rkm_codes/master.svg
-    :target: https://travis-ci.org/KenKundert/rkm_codes
+.. image:: https://pepy.tech/badge/rkm_codes/month
+    :target: https://pepy.tech/project/rkm_codes
+
+..  image:: https://github.com/KenKundert/rkm_codes/actions/workflows/build.yaml/badge.svg
+    :target: https://github.com/KenKundert/rkm_codes/actions/workflows/build.yaml
 
 .. image:: https://img.shields.io/coveralls/KenKundert/rkm_codes.svg
     :target: https://coveralls.io/r/KenKundert/rkm_codes
 
 .. image:: https://img.shields.io/pypi/v/rkm_codes.svg
     :target: https://pypi.python.org/pypi/rkm_codes
 
@@ -32,36 +35,39 @@
 IEC-60062 was significantly updated in 2016.
 
 RKM codes were originally used as part marking codes.  This shorthand
 notation is widely used in electrical engineering to denote the values of
 resistors and capacitors in circuit diagrams and in the production of electronic
 circuits (for example in bills of material and in silk screens). This method
 avoids overlooking the decimal separator, which may not be rendered reliably on
-components or when duplicating documents.  They also provide the benefit that
-the characters within a RKM code are either letters or digits, and so can be
-embedded within identifiers without introducing invalid characters.
+components or when duplicating documents.
+
+The popularity of RKM codes was fading because they address a problem that is 
+less common today. However they are making something of a come back as all the 
+characters in a RKM code are either letters or digits and so they can be 
+embedded in a software identifier without introducing illegal characters.
 
 IEC 60062 is described in https://en.wikipedia.org/wiki/RKM_code.
 
 Essentially an RKM version of a number is the number with a scale factor where
-the decimal point replaced by the scale factor. For example, a resistance of
+the decimal point is replaced by the scale factor. For example, a resistance of
 4.7kΩ becomes 4k7. If there is no scale factor, the decimal point is replaced by
 a letter that signifies the type of the component.  For example, a resistance of
 4.7Ω becomes 4r7.
 
-Resistance examples:
+Resistance examples::
 
-    | R47 → 0.47 Ω
-    | 4R7 → 4.7 Ω
-    | 470R → 470 Ω
-    | 4K7 → 4.7 kΩ
-    | 47K → 47 kΩ
-    | 47K3 → 47.3 kΩ
-    | 470K → 470 kΩ
-    | 4M7 → 4.7 MΩ
+    R47 → 0.47 Ω
+    4R7 → 4.7 Ω
+    470R → 470 Ω
+    4K7 → 4.7 kΩ
+    47K → 47 kΩ
+    47K3 → 47.3 kΩ
+    470K → 470 kΩ
+    4M7 → 4.7 MΩ
 
 In the standard, large values are assumed to be resistances and small values are
 assumed to be capacitances.  So 4k7 is a resistance and 2n5 is a capacitance.
 However, this package also supports a version of RKM codes where the units are
 not implied by the value, making RKM codes suitable for a wider variety of value
 types, such as voltage, current, and inductance.
 
@@ -72,15 +78,15 @@
 This package converts RKM codes to `QuantiPhy Quantities
 <https://quantiphy.readthedocs.io>`_ and Quantities to RKM codes.
 
 Install with::
 
     pip3 install --user rkm_codes
 
-Requires Python3.4 or better.
+Requires Python 3.6 or better.
 
 
 Converting to and from RKM Codes
 --------------------------------
 
 The following is a simple example of how to convert back and forth between RKM
 codes and Quantities::
@@ -270,15 +276,15 @@
     '5µ'
 
 
 Finding RKM Codes
 -----------------
 
 *find_rkm* is available for finding the RKM codes embedded in text strings.
-Using it, you can iterate through all the numbers specified using RKM:
+Using it, you can iterate through all the numbers specified using RKM::
 
     >>> from rkm_codes import find_rkm
 
     >>> text = '''
     ...     An RKM code that may include explicitly specified. Examples of
     ...     acceptable RKM codes for resistance include:   R47 (0.47 Ω), 4R7
     ...     (4.7 Ω), 470R (470 Ω), 4K7 (4.7 kΩ), 47K (47 kΩ), 47K3 (47.3 kΩ),
@@ -294,15 +300,15 @@
     47.3 kΩ
     470 kΩ
     4.7 MΩ
 
 When the RKM code is not isolated by punctuation or spaces it can get confused
 by leading and trailing text.  You can often resolve this issue by restricting
 the matches to either the leading or trailing digit forms of the RKM code. Do so
-by specifying either 'ld' or 'td' as a second argument.  For example:
+by specifying either 'ld' or 'td' as a second argument.  For example::
 
     >>> for num in find_rkm('sink200nA'):
     ...     print(num)
     200 msink
 
     >>> for num in find_rkm('sink200nA', 'ld'):
     ...     print(num)
@@ -342,16 +348,21 @@
     vdda_in_2V5
 
 
 Releases
 --------
 
 **Latest development release**:
-    | Version: 0.5.0
-    | Released: 2020-03-03
+    | Version: 0.6
+    | Released: 2023-04-14
+
+**0.6 (2023-04-14)**:
+    - Suppress *rkm_code*’s use of the new SI scale factors in `QuantiPhy 
+      <https://quantiphy.readthedocs.io>`_ so that ``R`` is no longer treated as 
+      a scale factor when using the latest version of *QuantiPhy*.
 
 **0.5 (2020-02-01)**:
     - Allow argument to *to_rkm()* to be a string or simple number
     - Added *strip_code* preference
     - With small numbers show 0 rather than exponent
 
 **0.4 (2019-08-29)**:
```

### Comparing `rkm_codes-0.5.0/rkm_codes/rkm_codes.py` & `rkm_codes-0.6/rkm_codes/rkm_codes.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 assumed to be capacitances.  So 4k7 is a resistance and 2n5 is a capacitance.
 However, this package also supports a version of RKM codes where the units are
 not implied by the value, making RKM codes suitable for a wider variety of value
 types, such as voltage, current, and inductance.
 """
 
 # license {{{1
-# Copyright (C) 2018-2020 Kenneth S. Kundert
+# Copyright (C) 2018-2023 Kenneth S. Kundert
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -52,16 +52,16 @@
 
 # imports {{{1
 import re
 from quantiphy import Quantity
 
 # constants {{{1
 # version {{{2
-__version__ = '0.5.0'
-__released__ = '2020-03-03'
+__version__ = '0.6'
+__released__ = '2023-04-14'
 
 # IEC60062 maps {{{2
 IEC60062_MAPS = {
     # These maps conform to the latest recommended mappings as defined in the 
     # IEC-60062 standard. They apply assume only resistors and capacitors. Small 
     # values are associated with capacitors and large values with resistors. The 
     # units can be inferred by the scale factors and so it is unnecessary to 
@@ -118,24 +118,25 @@
     'h': ('', ''),
 }
 
 # map units to rkm base code {{{2
 # Controls the base code produced by to_rkm().
 UNITS_TO_RKM_BASE_CODE = {
     'Ω': 'r',
+    'Ω': 'r',
     'Ohm': 'r',
     'F': 'c',
     'H': 'l',
     'V': 'v',
     'A': 'i',
 }
 
 # map scale factors {{{2
 # Controls the scale factors produced by to_rkm().
-#MAP_SF = dict(u='μ', k='K')  # this is mu
+# MAP_SF = dict(u='μ', k='K')  # this is mu
 MAP_SF = dict(u='µ', k='K')  # this is micro
 
 # others {{{2
 MINUS_SIGN = 'n'
 SHOW_UNITS = False
 STRIP_ZEROS = True
 STRIP_CODE = True
@@ -152,22 +153,26 @@
 _map_sf = MAP_SF
 _minus_sign = MINUS_SIGN
 _show_units = SHOW_UNITS
 _prec = PREC
 _strip_zeros = STRIP_ZEROS
 _strip_code = STRIP_CODE
 
+# get rid of the new scale factors (QRrq) because the R scale factor interferes
+# with using R as a unit.
+Quantity.set_prefs(input_sf='YZEPTGMKk_cmuµμnpfazy')
+
 def set_prefs(
     rkm_maps=False, units_to_rkm_base_code=False, map_sf=False,
     show_units='', strip_zeros='', strip_code='', minus_sign=False, prec=False
 ):
     '''Set Preferences
 
     Use to set values that control the behavior of the RKM code.
-    Any values not passed in a left alone.
+    Any values not passed in are left alone.
     Pass in *None* to reset a preference to its default value.
 
     Args:
         rkm_maps (dictionary of tuples):
             A dictionary that maps a base code or scale factor into a scale
             factor and units. Used to affect the behavior or *from_rkm()*.
             Generally set to rkm_codes.IEC60062_MAPS, which encourages
@@ -239,16 +244,16 @@
         _prec = PREC
     elif prec is not False:
         _prec = prec
 
 # RKM code patterns {{{1
 # regex1 matches rkm codes that start with a digit.
 # regex2 matches rkm codes that end with a digit.
-ld_regex = r'([pmn]?)([0-9]+)([a-zµμΩ℧]+)([0-9]*)'
-td_regex = r'([pmn]?)([0-9]*)([a-zµμΩ℧]+)([0-9]+)'
+ld_regex = r'([pmn]?)([0-9]+)([a-zµμΩƱ]+)([0-9]*)'
+td_regex = r'([pmn]?)([0-9]*)([a-zµμΩƱ]+)([0-9]+)'
 combined_regex = '(?:{})|(?:{})'.format(ld_regex, td_regex)
 ld_matcher = re.compile(ld_regex, re.I)
 td_matcher = re.compile(td_regex, re.I)
 combined_matcher = re.compile(combined_regex, re.I)
 
 # from_rkm {{{1
 def from_rkm(code):
```

