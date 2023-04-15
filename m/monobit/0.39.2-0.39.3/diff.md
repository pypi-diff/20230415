# Comparing `tmp/monobit-0.39.2.tar.gz` & `tmp/monobit-0.39.3.tar.gz`

## Comparing `monobit-0.39.2.tar` & `monobit-0.39.3.tar`

### file list

```diff
@@ -1,498 +1,500 @@
--rw-r--r--   0        0        0    26365 2020-02-02 00:00:00.000000 monobit-0.39.2/YAFF.md
--rwxr-xr-x   0        0        0       70 2020-02-02 00:00:00.000000 monobit-0.39.2/banner.py
--rwxr-xr-x   0        0        0       71 2020-02-02 00:00:00.000000 monobit-0.39.2/convert.py
--rwxr-xr-x   0        0        0     7145 2020-02-02 00:00:00.000000 monobit-0.39.2/explore.py
--rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/__init__.py
--rw-r--r--   0        0        0     2986 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/basetypes.py
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/binary.py
--rw-r--r--   0        0        0     3907 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/canvas.py
--rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/chart.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/constants.py
--rw-r--r--   0        0        0    57985 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/encoding.py
--rw-r--r--   0        0        0    48019 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/font.py
--rw-r--r--   0        0        0    29683 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/glyph.py
--rw-r--r--   0        0        0     9318 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/labels.py
--rw-r--r--   0        0        0    10103 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/magic.py
--rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/pack.py
--rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/properties.py
--rw-r--r--   0        0        0    20082 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/raster.py
--rw-r--r--   0        0        0    13621 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/renderer.py
--rw-r--r--   0        0        0    11363 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/scripting.py
--rw-r--r--   0        0        0    10357 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/storage.py
--rw-r--r--   0        0        0     7711 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/streams.py
--rw-r--r--   0        0        0     9363 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/struct.py
--rw-r--r--   0        0        0     5878 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/taggers.py
--rw-r--r--   0        0        0     3505 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/vector.py
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/adobe/ReadMe.txt
--rw-r--r--   0        0        0     8143 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/adobe/stdenc.txt
--rw-r--r--   0        0        0    10489 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/adobe/symbol.txt
--rw-r--r--   0        0        0    12033 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/adobe/zdingbat.txt
--rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/agl/LICENSE.md
--rw-r--r--   0        0        0     3623 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/agl/README.md
--rw-r--r--   0        0        0    27655 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/agl/aglfn.txt
--rw-r--r--   0        0        0    78060 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/agl/glyphlist.txt
--rw-r--r--   0        0        0    24830 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/apple/ARABIC.TXT
--rw-r--r--   0        0        0    13008 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/apple/CELTIC.TXT
--rw-r--r--   0        0        0    13065 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/apple/CENTEURO.TXT
--rw-r--r--   0        0        0   197055 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/apple/CHINSIMP.TXT
--rw-r--r--   0        0        0   323716 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/apple/CHINTRAD.TXT
--rw-r--r--   0        0        0    26610 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/apple/CORPCHAR.TXT
--rw-r--r--   0        0        0    13388 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/apple/CROATIAN.TXT
--rw-r--r--   0        0        0    13497 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/apple/CYRILLIC.TXT
--rw-r--r--   0        0        0    17540 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/apple/DEVANAGA.TXT
--rw-r--r--   0        0        0    14320 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/apple/DINGBATS.TXT
--rw-r--r--   0        0        0    23987 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/apple/FARSI.TXT
--rw-r--r--   0        0        0    14055 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/apple/GAELIC.TXT
--rw-r--r--   0        0        0    14042 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/apple/GREEK.TXT
--rw-r--r--   0        0        0    13940 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/apple/GUJARATI.TXT
--rw-r--r--   0        0        0    16096 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/apple/GURMUKHI.TXT
--rw-r--r--   0        0        0    27034 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/apple/HEBREW.TXT
--rw-r--r--   0        0        0    14021 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/apple/ICELAND.TXT
--rw-r--r--   0        0        0    11800 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/apple/INUIT.TXT
--rw-r--r--   0        0        0   198175 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/apple/JAPANESE.TXT
--rw-r--r--   0        0        0    10252 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/apple/KEYBOARD.TXT
--rw-r--r--   0        0        0   369061 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/apple/KOREAN.TXT
--rw-r--r--   0        0        0    14385 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/apple/ROMAN.TXT
--rw-r--r--   0        0        0    14153 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/apple/ROMANIAN.TXT
--rw-r--r--   0        0        0    28151 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/apple/ReadMe.txt
--rw-r--r--   0        0        0    16882 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/apple/SYMBOL.TXT
--rw-r--r--   0        0        0    15564 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/apple/THAI.TXT
--rw-r--r--   0        0        0    12808 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/apple/TURKISH.TXT
--rw-r--r--   0        0        0     4624 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/apple/UKRAINE.TXT
--rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/czyborra/README.md
--rw-r--r--   0        0        0     7380 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/czyborra/bulgarian-mik.txt
--rw-r--r--   0        0        0     7866 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/czyborra/cp866.txt
--rw-r--r--   0        0        0     5272 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/czyborra/gost19768-87.txt
--rw-r--r--   0        0        0     6552 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/czyborra/hp-roman8.txt
--rw-r--r--   0        0        0     5806 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/czyborra/koi-0.txt
--rw-r--r--   0        0        0     2969 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/czyborra/koi-7.txt
--rw-r--r--   0        0        0     5104 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/czyborra/koi8-a.txt
--rw-r--r--   0        0        0     5221 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/czyborra/koi8-b.txt
--rw-r--r--   0        0        0     6374 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/czyborra/koi8-e.txt
--rw-r--r--   0        0        0     7555 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/czyborra/koi8-f.txt
--rw-r--r--   0        0        0     7801 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/czyborra/koi8-r.txt
--rw-r--r--   0        0        0     7746 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/czyborra/koi8-u.txt
--rw-r--r--   0        0        0    12047 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/dkuug/iso646-ca
--rw-r--r--   0        0        0    12034 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/dkuug/iso646-ca2
--rw-r--r--   0        0        0    11838 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/dkuug/iso646-cn
--rw-r--r--   0        0        0    11910 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/dkuug/iso646-cu
--rw-r--r--   0        0        0    11978 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/dkuug/iso646-de
--rw-r--r--   0        0        0    11938 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/dkuug/iso646-dk
--rw-r--r--   0        0        0    11868 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/dkuug/iso646-es
--rw-r--r--   0        0        0    11888 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/dkuug/iso646-es2
--rw-r--r--   0        0        0    11903 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/dkuug/iso646-fr
--rw-r--r--   0        0        0    11847 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/dkuug/iso646-gb
--rw-r--r--   0        0        0    11997 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/dkuug/iso646-hu
--rw-r--r--   0        0        0    11926 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/dkuug/iso646-it
--rw-r--r--   0        0        0    11841 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/dkuug/iso646-jp
--rw-r--r--   0        0        0    11770 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/dkuug/iso646-jp-ocr-b
--rw-r--r--   0        0        0    11773 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/dkuug/iso646-kr
--rw-r--r--   0        0        0    11949 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/dkuug/iso646-us
--rw-r--r--   0        0        0    12023 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/dkuug/iso646-yu
--rw-r--r--   0        0        0    17534 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/dkuug/jis_x0201
--rw-r--r--   0        0        0    10319 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/dkuug/x0201-7
--rw-r--r--   0        0        0     4900 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/emacs/MULE-ethiopic.map
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/emacs/MULE-ipa.map
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/emacs/MULE-is13194.map
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/emacs/MULE-lviscii.map
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/emacs/MULE-sisheng.map
--rw-r--r--   0        0        0     2772 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/emacs/MULE-tibetan.map
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/emacs/MULE-uviscii.map
--rw-r--r--   0        0        0     2919 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/emacs/README.md
--rw-r--r--   0        0        0    10137 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/evertype/ARMENIAN.TXT
--rw-r--r--   0        0        0     9763 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/evertype/GEORGIAN.TXT
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/evertype/README.md
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/1116.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/1117.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/1118.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/1119.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/1125.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/113.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/1131.ucp
--rw-r--r--   0        0        0     2057 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/30000.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/30001.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/30002.ucp
--rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/30003.ucp
--rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/30004.ucp
--rw-r--r--   0        0        0     3026 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/30005.ucp
--rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/30006.ucp
--rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/30007.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/30008.ucp
--rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/30009.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/30010.ucp
--rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/30011.ucp
--rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/30012.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/30013.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/30014.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/30015.ucp
--rw-r--r--   0        0        0     2794 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/30016.ucp
--rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/30017.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/30018.ucp
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/30019.ucp
--rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/30020.ucp
--rw-r--r--   0        0        0     2346 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/30021.ucp
--rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/30022.ucp
--rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/30023.ucp
--rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/30024.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/30025.ucp
--rw-r--r--   0        0        0     2596 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/30026.ucp
--rw-r--r--   0        0        0     2433 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/30027.ucp
--rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/30028.ucp
--rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/30029.ucp
--rw-r--r--   0        0        0     3454 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/30030.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/30031.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/30032.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/30033.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/30034.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/30039.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/30040.ucp
--rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/3012.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/3021.ucp
--rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/3845.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/3846.ucp
--rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/3848.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/437.ucp
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/57781.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/58152.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/58210.ucp
--rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/58335.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/59234.ucp
--rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/59829.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/60258.ucp
--rw-r--r--   0        0        0     2189 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/60853.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/61282.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/62306.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/667.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/668.ucp
--rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/737.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/770.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/771.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/772.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/773.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/774.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/775.ucp
--rw-r--r--   0        0        0     3970 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/777.ucp
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/778.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/790.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/808.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/848.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/849.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/850.ucp
--rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/851.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/852.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/853.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/855.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/856.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/857.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/858.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/859.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/860.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/861.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/862.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/863.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/864.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/865.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/866.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/867.ucp
--rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/869.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/872.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/895.ucp
--rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/899.ucp
--rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/991.ucp
--rw-r--r--   0        0        0     5269 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/freedos/README.md
--rw-r--r--   0        0        0     9255 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/iana/Amiga-1251
--rw-r--r--   0        0        0    13371 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/iana/PTCP154
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/iana/README.md
--rw-r--r--   0        0        0    14491 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/ibm-cdra/037B34B0.UPMAP100
--rw-r--r--   0        0        0    11755 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/ibm-cdra/038834B0.UPMAP100
--rw-r--r--   0        0        0   323573 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/ibm-cdra/039E44B0.UPMAP101
--rw-r--r--   0        0        0   973501 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/ibm-cdra/039F34B0.UPMAP100
--rw-r--r--   0        0        0    17655 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/ibm-cdra/readme.txt
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/icu/README.md
--rw-r--r--   0        0        0   177606 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/icu/aix-KSC5601.1987_0-4.3.6.ucm
--rw-r--r--   0        0        0  1348868 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/icu/cns-11643-1992.ucm
--rw-r--r--   0        0        0     7072 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/icu/ibm-1125_P100-1997.ucm
--rw-r--r--   0        0        0   433127 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/icu/ibm-1375_P100-2008.ucm
--rw-r--r--   0        0        0     6350 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/icu/ibm-720_P100-1997.ucm
--rw-r--r--   0        0        0     5972 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/icu/ibm-806_P100-1998.ucm
--rw-r--r--   0        0        0     7054 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/icu/ibm-851_P100-1995.ucm
--rw-r--r--   0        0        0     7054 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/icu/ibm-858_P100-1997.ucm
--rw-r--r--   0        0        0     8451 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/icu/ibm-868_P100-1995.ucm
--rw-r--r--   0        0        0   199596 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/icu/ibm-932_P120-1999.ucm
--rw-r--r--   0        0        0   351895 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/icu/windows-1361-2000.ucm
--rw-r--r--   0        0        0   490901 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/icu/windows-936-2000.ucm
--rw-r--r--   0        0        0     9995 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/iso-8859/8859-1.TXT
--rw-r--r--   0        0        0    10385 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/iso-8859/8859-10.TXT
--rw-r--r--   0        0        0     9192 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/iso-8859/8859-11.TXT
--rw-r--r--   0        0        0    10026 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/iso-8859/8859-13.TXT
--rw-r--r--   0        0        0    10459 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/iso-8859/8859-14.TXT
--rw-r--r--   0        0        0    10039 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/iso-8859/8859-15.TXT
--rw-r--r--   0        0        0    10390 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/iso-8859/8859-16.TXT
--rw-r--r--   0        0        0    10219 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/iso-8859/8859-2.TXT
--rw-r--r--   0        0        0     9901 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/iso-8859/8859-3.TXT
--rw-r--r--   0        0        0    10195 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/iso-8859/8859-4.TXT
--rw-r--r--   0        0        0     9830 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/iso-8859/8859-5.TXT
--rw-r--r--   0        0        0     7723 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/iso-8859/8859-6.TXT
--rw-r--r--   0        0        0    10053 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/iso-8859/8859-7.TXT
--rw-r--r--   0        0        0     7943 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/iso-8859/8859-8.TXT
--rw-r--r--   0        0        0    10030 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/iso-8859/8859-9.TXT
--rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/iso-8859/ReadMe.txt
--rw-r--r--   0        0        0     4540 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/kreativekorp/ADAMOS7.TXT
--rw-r--r--   0        0        0     4506 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/kreativekorp/ADAMSWTR.TXT
--rw-r--r--   0        0        0     8879 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/kreativekorp/AMSCPC.TXT
--rw-r--r--   0        0        0    10266 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/kreativekorp/AMSCPM.TXT
--rw-r--r--   0        0        0    10898 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/kreativekorp/APL2ALT1.TXT
--rw-r--r--   0        0        0    10929 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/kreativekorp/APL2ALT2.TXT
--rw-r--r--   0        0        0     6461 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/kreativekorp/APL2ICHG.TXT
--rw-r--r--   0        0        0    11100 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/kreativekorp/APL2PRIM.TXT
--rw-r--r--   0        0        0    10985 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/kreativekorp/ATARI8IG.TXT
--rw-r--r--   0        0        0    11148 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/kreativekorp/ATARI8II.TXT
--rw-r--r--   0        0        0    11734 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/kreativekorp/ATARI8VG.TXT
--rw-r--r--   0        0        0    12144 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/kreativekorp/ATARI8VI.TXT
--rw-r--r--   0        0        0     8280 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/kreativekorp/ATARISTI.TXT
--rw-r--r--   0        0        0     9561 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/kreativekorp/ATARISTV.TXT
--rw-r--r--   0        0        0     7277 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/kreativekorp/C64IALT.TXT
--rw-r--r--   0        0        0     7795 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/kreativekorp/C64IPRI.TXT
--rw-r--r--   0        0        0    11514 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/kreativekorp/C64VALT.TXT
--rw-r--r--   0        0        0    12009 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/kreativekorp/C64VPRI.TXT
--rw-r--r--   0        0        0     9648 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/kreativekorp/COCOICHG.TXT
--rw-r--r--   0        0        0    11149 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/kreativekorp/COCOSGR4.TXT
--rw-r--r--   0        0        0     4792 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/kreativekorp/COCOSGR6.TXT
--rw-r--r--   0        0        0     7263 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/kreativekorp/CPETIALT.TXT
--rw-r--r--   0        0        0     7797 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/kreativekorp/CPETIPRI.TXT
--rw-r--r--   0        0        0    11521 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/kreativekorp/CPETVALT.TXT
--rw-r--r--   0        0        0    12016 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/kreativekorp/CPETVPRI.TXT
--rw-r--r--   0        0        0     7261 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/kreativekorp/CVICIALT.TXT
--rw-r--r--   0        0        0     7795 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/kreativekorp/CVICIPRI.TXT
--rw-r--r--   0        0        0    11514 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/kreativekorp/CVICVALT.TXT
--rw-r--r--   0        0        0    12009 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/kreativekorp/CVICVPRI.TXT
--rw-r--r--   0        0        0     8974 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/kreativekorp/IBMPCICH.TXT
--rw-r--r--   0        0        0    10018 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/kreativekorp/IBMPCVID.TXT
--rw-r--r--   0        0        0     6045 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/kreativekorp/MINITLG0.TXT
--rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/kreativekorp/MINITLG1.TXT
--rw-r--r--   0        0        0     9910 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/kreativekorp/MSX.TXT
--rw-r--r--   0        0        0     3292 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/kreativekorp/ORICG0.TXT
--rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/kreativekorp/ORICG1.TXT
--rw-r--r--   0        0        0     8650 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/kreativekorp/RISCEFF.TXT
--rw-r--r--   0        0        0     8478 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/kreativekorp/RISCOSB.TXT
--rw-r--r--   0        0        0     8363 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/kreativekorp/RISCOSI.TXT
--rw-r--r--   0        0        0    10499 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/kreativekorp/RISCOSV.TXT
--rw-r--r--   0        0        0    14920 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/kreativekorp/ReadMe.txt
--rw-r--r--   0        0        0     9603 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/kreativekorp/SINCLRQL.TXT
--rw-r--r--   0        0        0     3332 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/kreativekorp/TELTXTG0.TXT
--rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/kreativekorp/TELTXTG1.TXT
--rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/kreativekorp/TELTXTG2.TXT
--rw-r--r--   0        0        0     6062 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/kreativekorp/TELTXTG3.TXT
--rw-r--r--   0        0        0     3825 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/kreativekorp/TI994A.TXT
--rw-r--r--   0        0        0     5639 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/kreativekorp/TRSM1ICH.TXT
--rw-r--r--   0        0        0     9089 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/kreativekorp/TRSM1ORG.TXT
--rw-r--r--   0        0        0     9064 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/kreativekorp/TRSM1REV.TXT
--rw-r--r--   0        0        0     7983 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/kreativekorp/TRSM3IIN.TXT
--rw-r--r--   0        0        0     8497 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/kreativekorp/TRSM3IJP.TXT
--rw-r--r--   0        0        0    10398 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/kreativekorp/TRSM3IRV.TXT
--rw-r--r--   0        0        0     9363 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/kreativekorp/TRSM3VIN.TXT
--rw-r--r--   0        0        0     9877 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/kreativekorp/TRSM3VJP.TXT
--rw-r--r--   0        0        0    11778 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/kreativekorp/TRSM3VRV.TXT
--rw-r--r--   0        0        0     8379 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/kreativekorp/TRSM4AIA.TXT
--rw-r--r--   0        0        0     7974 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/kreativekorp/TRSM4AIP.TXT
--rw-r--r--   0        0        0    10398 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/kreativekorp/TRSM4AIR.TXT
--rw-r--r--   0        0        0     9808 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/kreativekorp/TRSM4AVA.TXT
--rw-r--r--   0        0        0     9402 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/kreativekorp/TRSM4AVP.TXT
--rw-r--r--   0        0        0    11826 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/kreativekorp/TRSM4AVR.TXT
--rw-r--r--   0        0        0     5587 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/kreativekorp/ZX80.TXT
--rw-r--r--   0        0        0     5587 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/kreativekorp/ZX81.TXT
--rw-r--r--   0        0        0     4746 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/kreativekorp/ZXDESKTP.TXT
--rw-r--r--   0        0        0     6617 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/kreativekorp/ZXFZXKOI.TXT
--rw-r--r--   0        0        0     7553 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/kreativekorp/ZXFZXLT1.TXT
--rw-r--r--   0        0        0     7590 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/kreativekorp/ZXFZXLT5.TXT
--rw-r--r--   0        0        0     5083 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/kreativekorp/ZXFZXPUA.TXT
--rw-r--r--   0        0        0     8813 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/kreativekorp/ZXFZXSLT.TXT
--rw-r--r--   0        0        0     4331 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/kreativekorp/ZXSPCTRM.TXT
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/manual/currency-sign-0x9c.ucp
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/manual/currency-sign-0xdb.ucp
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/manual/dec-vt100.ucp
--rw-r--r--   0        0        0     8428 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/manual/hp48.txt
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/manual/ibm897graph.ucp
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/manual/mac-cyrillic-pre9.0.ucp
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/manual/mac-system.ucp
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/manual/mac-ukrainian-pre9.0.ucp
--rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/manual/ms-linedraw.txt
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/manual/russup3.ucp
--rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/manual/russup4ac.ucp
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/manual/russup4na.ucp
--rw-r--r--   0        0        0     7901 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/manual/windows-1.0.txt
--rw-r--r--   0        0        0     8028 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/manual/windows-2.0.txt
--rw-r--r--   0        0        0     9006 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/manual/windows-3.1.txt
--rw-r--r--   0        0        0     9000 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/microsoft/EBCDIC/CP037.TXT
--rw-r--r--   0        0        0     9012 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/microsoft/EBCDIC/CP1026.TXT
--rw-r--r--   0        0        0     9027 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/microsoft/EBCDIC/CP500.TXT
--rw-r--r--   0        0        0     8721 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/microsoft/EBCDIC/CP875.TXT
--rw-r--r--   0        0        0     9177 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/microsoft/MAC/CYRILLIC.TXT
--rw-r--r--   0        0        0     9413 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/microsoft/MAC/GREEK.TXT
--rw-r--r--   0        0        0     9253 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/microsoft/MAC/ICELAND.TXT
--rw-r--r--   0        0        0     9862 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/microsoft/MAC/LATIN2.TXT
--rw-r--r--   0        0        0     9229 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/microsoft/MAC/ROMAN.TXT
--rw-r--r--   0        0        0     9251 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/microsoft/MAC/TURKISH.TXT
--rw-r--r--   0        0        0     9794 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/microsoft/PC/CP437.TXT
--rw-r--r--   0        0        0     9827 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/microsoft/PC/CP737.TXT
--rw-r--r--   0        0        0     9766 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/microsoft/PC/CP775.TXT
--rw-r--r--   0        0        0     9640 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/microsoft/PC/CP850.TXT
--rw-r--r--   0        0        0     9939 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/microsoft/PC/CP852.TXT
--rw-r--r--   0        0        0     9562 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/microsoft/PC/CP855.TXT
--rw-r--r--   0        0        0     9617 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/microsoft/PC/CP857.TXT
--rw-r--r--   0        0        0     9845 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/microsoft/PC/CP860.TXT
--rw-r--r--   0        0        0     9826 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/microsoft/PC/CP861.TXT
--rw-r--r--   0        0        0     9396 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/microsoft/PC/CP862.TXT
--rw-r--r--   0        0        0     9693 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/microsoft/PC/CP863.TXT
--rw-r--r--   0        0        0     9560 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/microsoft/PC/CP864.TXT
--rw-r--r--   0        0        0     9812 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/microsoft/PC/CP865.TXT
--rw-r--r--   0        0        0     9765 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/microsoft/PC/CP866.TXT
--rw-r--r--   0        0        0     9318 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/microsoft/PC/CP869.TXT
--rw-r--r--   0        0        0     8452 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/microsoft/PC/CP874.TXT
--rw-r--r--   0        0        0     9530 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/microsoft/WINDOWS/CP1250.TXT
--rw-r--r--   0        0        0     9205 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/microsoft/WINDOWS/CP1251.TXT
--rw-r--r--   0        0        0     9355 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/microsoft/WINDOWS/CP1252.TXT
--rw-r--r--   0        0        0     8938 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/microsoft/WINDOWS/CP1253.TXT
--rw-r--r--   0        0        0     9346 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/microsoft/WINDOWS/CP1254.TXT
--rw-r--r--   0        0        0     8304 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/microsoft/WINDOWS/CP1255.TXT
--rw-r--r--   0        0        0     8657 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/microsoft/WINDOWS/CP1256.TXT
--rw-r--r--   0        0        0     9218 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/microsoft/WINDOWS/CP1257.TXT
--rw-r--r--   0        0        0     9208 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/microsoft/WINDOWS/CP1258.TXT
--rw-r--r--   0        0        0     8439 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/microsoft/WINDOWS/CP874.TXT
--rw-r--r--   0        0        0   295324 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/microsoft/WINDOWS/CP932.TXT
--rw-r--r--   0        0        0   817310 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/microsoft/WINDOWS/CP936.TXT
--rw-r--r--   0        0        0   790736 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/microsoft/WINDOWS/CP949.TXT
--rw-r--r--   0        0        0   508978 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/microsoft/WINDOWS/CP950.TXT
--rw-r--r--   0        0        0    11537 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/misc/APL-ISO-IR-68.TXT
--rw-r--r--   0        0        0    21171 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/misc/ATARIST.TXT
--rw-r--r--   0        0        0    10895 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/misc/CP1006.TXT
--rw-r--r--   0        0        0     8978 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/misc/CP424.TXT
--rw-r--r--   0        0        0     9281 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/misc/CP856.TXT
--rw-r--r--   0        0        0     8707 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/misc/GSM0338.TXT
--rw-r--r--   0        0        0     3748 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/misc/IBMGRAPH.TXT
--rw-r--r--   0        0        0   210734 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/misc/JIS0208.TXT
--rw-r--r--   0        0        0    10692 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/misc/KOI8-R.TXT
--rw-r--r--   0        0        0    11041 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/misc/KOI8-U.TXT
--rw-r--r--   0        0        0   784637 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/misc/KPS9566.TXT
--rw-r--r--   0        0        0    10532 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/misc/KZ1048.TXT
--rw-r--r--   0        0        0     7093 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/misc/NEXTSTEP.TXT
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/misc/README.md
--rw-r--r--   0        0        0    49569 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/misc/SGML.TXT
--rw-r--r--   0        0        0     7054 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/misc/US-ASCII-QUOTES.TXT
--rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/misc/dashen-map.txt
--rw-r--r--   0        0        0    92930 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/misc/ibm-ugl.txt
--rw-r--r--   0        0        0     9996 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/mleisher/ALTVAR.TXT
--rw-r--r--   0        0        0     4788 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/mleisher/ARMSCII-7.TXT
--rw-r--r--   0        0        0     8606 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/mleisher/ARMSCII-8.TXT
--rw-r--r--   0        0        0     9049 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/mleisher/ARMSCII-8A.TXT
--rw-r--r--   0        0        0     8120 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/mleisher/DECMCS.TXT
--rw-r--r--   0        0        0     9870 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/mleisher/GEO-ITA.TXT
--rw-r--r--   0        0        0     9758 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/mleisher/GEO-PS.TXT
--rw-r--r--   0        0        0    13439 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/mleisher/IRANSYSTEM.TXT
--rw-r--r--   0        0        0    10796 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/mleisher/KOI8RU.TXT
--rw-r--r--   0        0        0     9607 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/mleisher/OSNOVAR.TXT
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/mleisher/README.md
--rw-r--r--   0        0        0     9566 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/mleisher/TIS620.TXT
--rw-r--r--   0        0        0   274176 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/moztw/big5_2003-b2u.txt
--rw-r--r--   0        0        0   340277 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/moztw/eten.txt
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/moztw/url
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/python/README.md
--rw-r--r--   0        0        0    11789 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/python/TCVN5712-1.TXT
--rw-r--r--   0        0        0    10621 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/python/TCVN5712-2.TXT
--rw-r--r--   0        0        0     9998 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/python/TCVN5712-3.TXT
--rw-r--r--   0        0        0    10088 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/vietstd/unicode.html
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/vietstd/url
--rw-r--r--   0        0        0     7055 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/vietstd/viscii1.1.txt
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/wikipedia/README.md
--rw-r--r--   0        0        0   156347 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/wikipedia/abicomp.html
--rw-r--r--   0        0        0   180593 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/wikipedia/brascii.html
--rw-r--r--   0        0        0   144572 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/wikipedia/cp853.html
--rw-r--r--   0        0        0   156279 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/wikipedia/cwi2.html
--rw-r--r--   0        0        0   134679 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/wikipedia/dec-special.html
--rw-r--r--   0        0        0   153445 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/wikipedia/dec-technical.html
--rw-r--r--   0        0        0   192405 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/wikipedia/gem.html
--rw-r--r--   0        0        0   172501 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/wikipedia/kamenicky.html
--rw-r--r--   0        0        0   216297 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/wikipedia/lics.html
--rw-r--r--   0        0        0   150793 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/wikipedia/mattel-aquarius.html
--rw-r--r--   0        0        0   159296 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/wikipedia/mazovia.html
--rw-r--r--   0        0        0   167964 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/wikipedia/pascii.html
--rw-r--r--   0        0        0   217224 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/wikipedia/ventura.html
--rw-r--r--   0        0        0   254035 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/wikipedia/windows-1252.html
--rw-r--r--   0        0        0   245126 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/wikipedia/wingdings.html
--rw-r--r--   0        0        0   160779 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/wikipedia/wiscii.html
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/xfonts/README.md
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/xfonts/mulearabic-0.enc
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/xfonts/mulearabic-1.enc
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/xfonts/mulearabic-2.enc
--rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/xfonts/mulelao-1.enc
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/xfonts/suneu-greek.enc
--rw-r--r--   0        0        0     7477 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/charmaps/xfonts/viscii1.1-1.enc
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/containers/__init__.py
--rw-r--r--   0        0        0     3897 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/containers/compressors.py
--rw-r--r--   0        0        0     5573 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/containers/container.py
--rw-r--r--   0        0        0     3224 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/containers/directory.py
--rw-r--r--   0        0        0    11164 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/containers/mac.py
--rw-r--r--   0        0        0    14707 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/containers/source.py
--rw-r--r--   0        0        0     4037 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/containers/tar.py
--rw-r--r--   0        0        0     3772 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/containers/zip.py
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/formats/__init__.py
--rw-r--r--   0        0        0    14368 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/formats/amiga.py
--rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/formats/bbc.py
--rw-r--r--   0        0        0    41624 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/formats/bdf.py
--rw-r--r--   0        0        0    41746 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/formats/bmfont.py
--rw-r--r--   0        0        0     8295 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/formats/borland.py
--rw-r--r--   0        0        0    22614 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/formats/cpi.py
--rw-r--r--   0        0        0     6873 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/formats/daisydot.py
--rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/formats/dashen.py
--rw-r--r--   0        0        0    13468 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/formats/dec.py
--rw-r--r--   0        0        0     4052 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/formats/dosstart.py
--rw-r--r--   0        0        0    11129 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/formats/figlet.py
--rw-r--r--   0        0        0     6312 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/formats/fontx.py
--rw-r--r--   0        0        0    11729 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/formats/fzx.py
--rw-r--r--   0        0        0    26397 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/formats/gdos.py
--rw-r--r--   0        0        0    12688 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/formats/geos.py
--rw-r--r--   0        0        0    18471 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/formats/hbf.py
--rw-r--r--   0        0        0     7349 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/formats/hex.py
--rw-r--r--   0        0        0     4489 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/formats/hexdraw.py
--rw-r--r--   0        0        0     3631 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/formats/hurt.py
--rw-r--r--   0        0        0    10383 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/formats/image.py
--rw-r--r--   0        0        0     2435 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/formats/mousegraphics.py
--rw-r--r--   0        0        0     4393 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/formats/mzfon.py
--rw-r--r--   0        0        0    10427 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/formats/nearlyraw.py
--rw-r--r--   0        0        0     8294 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/formats/palm.py
--rw-r--r--   0        0        0    29954 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/formats/pcl.py
--rw-r--r--   0        0        0     7598 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/formats/pcpaint.py
--rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/formats/pdf.py
--rw-r--r--   0        0        0    12848 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/formats/pkfont.py
--rw-r--r--   0        0        0     2898 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/formats/printshop.py
--rw-r--r--   0        0        0     5708 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/formats/psf.py
--rw-r--r--   0        0        0     8138 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/formats/raw.py
--rw-r--r--   0        0        0    28660 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/formats/sfnt.py
--rw-r--r--   0        0        0     4934 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/formats/signum.py
--rw-r--r--   0        0        0     8490 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/formats/svg.py
--rw-r--r--   0        0        0     6516 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/formats/vfont.py
--rw-r--r--   0        0        0    14232 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/formats/yaff.py
--rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/formats/mac/__init__.py
--rw-r--r--   0        0        0    10477 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/formats/mac/dfont.py
--rw-r--r--   0        0        0    12772 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/formats/mac/fond.py
--rw-r--r--   0        0        0     5312 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/formats/mac/iigs.py
--rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/formats/mac/lisa.py
--rw-r--r--   0        0        0    22316 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/formats/mac/nfnt.py
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/formats/os2/__init__.py
--rw-r--r--   0        0        0    21098 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/formats/os2/gpifont.py
--rw-r--r--   0        0        0    11032 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/formats/os2/lx.py
--rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/formats/os2/ne.py
--rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/formats/windows/LICENSE.md
--rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/formats/windows/__init__.py
--rw-r--r--   0        0        0    33202 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/formats/windows/fnt.py
--rw-r--r--   0        0        0     3027 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/formats/windows/mz.py
--rw-r--r--   0        0        0    14167 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/formats/windows/ne.py
--rw-r--r--   0        0        0     5394 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/formats/windows/pe.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/scripts/__init__.py
--rwxr-xr-x   0        0        0     9148 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/scripts/banner.py
--rwxr-xr-x   0        0        0     3671 2020-02-02 00:00:00.000000 monobit-0.39.2/monobit/scripts/convert.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 monobit-0.39.2/.gitignore
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 monobit-0.39.2/LICENSE
--rw-r--r--   0        0        0    17179 2020-02-02 00:00:00.000000 monobit-0.39.2/README.md
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 monobit-0.39.2/pyproject.toml
--rw-r--r--   0        0        0    19132 2020-02-02 00:00:00.000000 monobit-0.39.2/PKG-INFO
+-rw-r--r--   0        0        0    26365 2020-02-02 00:00:00.000000 monobit-0.39.3/YAFF.md
+-rwxr-xr-x   0        0        0       70 2020-02-02 00:00:00.000000 monobit-0.39.3/banner.py
+-rwxr-xr-x   0        0        0       71 2020-02-02 00:00:00.000000 monobit-0.39.3/convert.py
+-rwxr-xr-x   0        0        0     7145 2020-02-02 00:00:00.000000 monobit-0.39.3/explore.py
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/__init__.py
+-rw-r--r--   0        0        0     2986 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/basetypes.py
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/binary.py
+-rw-r--r--   0        0        0     3907 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/canvas.py
+-rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/chart.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/constants.py
+-rw-r--r--   0        0        0    57985 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/encoding.py
+-rw-r--r--   0        0        0    47781 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/font.py
+-rw-r--r--   0        0        0    29683 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/glyph.py
+-rw-r--r--   0        0        0     9505 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/labels.py
+-rw-r--r--   0        0        0    10103 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/magic.py
+-rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/pack.py
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/properties.py
+-rw-r--r--   0        0        0    20080 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/raster.py
+-rw-r--r--   0        0        0    13621 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/renderer.py
+-rw-r--r--   0        0        0    11363 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/scripting.py
+-rw-r--r--   0        0        0    10357 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/storage.py
+-rw-r--r--   0        0        0     7711 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/streams.py
+-rw-r--r--   0        0        0     9363 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/struct.py
+-rw-r--r--   0        0        0     5878 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/taggers.py
+-rw-r--r--   0        0        0     3555 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/vector.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/__init__.py
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/adobe/ReadMe.txt
+-rw-r--r--   0        0        0     8143 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/adobe/stdenc.txt
+-rw-r--r--   0        0        0    10489 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/adobe/symbol.txt
+-rw-r--r--   0        0        0    12033 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/adobe/zdingbat.txt
+-rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/agl/LICENSE.md
+-rw-r--r--   0        0        0     3623 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/agl/README.md
+-rw-r--r--   0        0        0    27655 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/agl/aglfn.txt
+-rw-r--r--   0        0        0    78060 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/agl/glyphlist.txt
+-rw-r--r--   0        0        0    24830 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/apple/ARABIC.TXT
+-rw-r--r--   0        0        0    13008 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/apple/CELTIC.TXT
+-rw-r--r--   0        0        0    13065 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/apple/CENTEURO.TXT
+-rw-r--r--   0        0        0   197055 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/apple/CHINSIMP.TXT
+-rw-r--r--   0        0        0   323716 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/apple/CHINTRAD.TXT
+-rw-r--r--   0        0        0    26610 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/apple/CORPCHAR.TXT
+-rw-r--r--   0        0        0    13388 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/apple/CROATIAN.TXT
+-rw-r--r--   0        0        0    13497 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/apple/CYRILLIC.TXT
+-rw-r--r--   0        0        0    17540 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/apple/DEVANAGA.TXT
+-rw-r--r--   0        0        0    14320 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/apple/DINGBATS.TXT
+-rw-r--r--   0        0        0    23987 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/apple/FARSI.TXT
+-rw-r--r--   0        0        0    14055 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/apple/GAELIC.TXT
+-rw-r--r--   0        0        0    14042 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/apple/GREEK.TXT
+-rw-r--r--   0        0        0    13940 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/apple/GUJARATI.TXT
+-rw-r--r--   0        0        0    16096 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/apple/GURMUKHI.TXT
+-rw-r--r--   0        0        0    27034 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/apple/HEBREW.TXT
+-rw-r--r--   0        0        0    14021 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/apple/ICELAND.TXT
+-rw-r--r--   0        0        0    11800 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/apple/INUIT.TXT
+-rw-r--r--   0        0        0   198175 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/apple/JAPANESE.TXT
+-rw-r--r--   0        0        0    10252 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/apple/KEYBOARD.TXT
+-rw-r--r--   0        0        0   369061 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/apple/KOREAN.TXT
+-rw-r--r--   0        0        0    14385 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/apple/ROMAN.TXT
+-rw-r--r--   0        0        0    14153 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/apple/ROMANIAN.TXT
+-rw-r--r--   0        0        0    28151 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/apple/ReadMe.txt
+-rw-r--r--   0        0        0    16882 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/apple/SYMBOL.TXT
+-rw-r--r--   0        0        0    15564 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/apple/THAI.TXT
+-rw-r--r--   0        0        0    12808 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/apple/TURKISH.TXT
+-rw-r--r--   0        0        0     4624 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/apple/UKRAINE.TXT
+-rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/czyborra/README.md
+-rw-r--r--   0        0        0     7380 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/czyborra/bulgarian-mik.txt
+-rw-r--r--   0        0        0     7866 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/czyborra/cp866.txt
+-rw-r--r--   0        0        0     5272 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/czyborra/gost19768-87.txt
+-rw-r--r--   0        0        0     6552 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/czyborra/hp-roman8.txt
+-rw-r--r--   0        0        0     5806 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/czyborra/koi-0.txt
+-rw-r--r--   0        0        0     2969 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/czyborra/koi-7.txt
+-rw-r--r--   0        0        0     5104 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/czyborra/koi8-a.txt
+-rw-r--r--   0        0        0     5221 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/czyborra/koi8-b.txt
+-rw-r--r--   0        0        0     6374 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/czyborra/koi8-e.txt
+-rw-r--r--   0        0        0     7555 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/czyborra/koi8-f.txt
+-rw-r--r--   0        0        0     7801 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/czyborra/koi8-r.txt
+-rw-r--r--   0        0        0     7746 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/czyborra/koi8-u.txt
+-rw-r--r--   0        0        0    12047 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/dkuug/iso646-ca
+-rw-r--r--   0        0        0    12034 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/dkuug/iso646-ca2
+-rw-r--r--   0        0        0    11838 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/dkuug/iso646-cn
+-rw-r--r--   0        0        0    11910 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/dkuug/iso646-cu
+-rw-r--r--   0        0        0    11978 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/dkuug/iso646-de
+-rw-r--r--   0        0        0    11938 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/dkuug/iso646-dk
+-rw-r--r--   0        0        0    11868 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/dkuug/iso646-es
+-rw-r--r--   0        0        0    11888 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/dkuug/iso646-es2
+-rw-r--r--   0        0        0    11903 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/dkuug/iso646-fr
+-rw-r--r--   0        0        0    11847 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/dkuug/iso646-gb
+-rw-r--r--   0        0        0    11997 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/dkuug/iso646-hu
+-rw-r--r--   0        0        0    11926 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/dkuug/iso646-it
+-rw-r--r--   0        0        0    11841 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/dkuug/iso646-jp
+-rw-r--r--   0        0        0    11770 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/dkuug/iso646-jp-ocr-b
+-rw-r--r--   0        0        0    11773 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/dkuug/iso646-kr
+-rw-r--r--   0        0        0    11949 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/dkuug/iso646-us
+-rw-r--r--   0        0        0    12023 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/dkuug/iso646-yu
+-rw-r--r--   0        0        0    17534 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/dkuug/jis_x0201
+-rw-r--r--   0        0        0    10319 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/dkuug/x0201-7
+-rw-r--r--   0        0        0     4900 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/emacs/MULE-ethiopic.map
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/emacs/MULE-ipa.map
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/emacs/MULE-is13194.map
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/emacs/MULE-lviscii.map
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/emacs/MULE-sisheng.map
+-rw-r--r--   0        0        0     2772 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/emacs/MULE-tibetan.map
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/emacs/MULE-uviscii.map
+-rw-r--r--   0        0        0     2919 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/emacs/README.md
+-rw-r--r--   0        0        0    10137 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/evertype/ARMENIAN.TXT
+-rw-r--r--   0        0        0     9763 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/evertype/GEORGIAN.TXT
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/evertype/README.md
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/1116.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/1117.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/1118.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/1119.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/1125.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/113.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/1131.ucp
+-rw-r--r--   0        0        0     2057 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/30000.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/30001.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/30002.ucp
+-rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/30003.ucp
+-rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/30004.ucp
+-rw-r--r--   0        0        0     3026 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/30005.ucp
+-rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/30006.ucp
+-rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/30007.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/30008.ucp
+-rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/30009.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/30010.ucp
+-rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/30011.ucp
+-rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/30012.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/30013.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/30014.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/30015.ucp
+-rw-r--r--   0        0        0     2794 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/30016.ucp
+-rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/30017.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/30018.ucp
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/30019.ucp
+-rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/30020.ucp
+-rw-r--r--   0        0        0     2346 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/30021.ucp
+-rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/30022.ucp
+-rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/30023.ucp
+-rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/30024.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/30025.ucp
+-rw-r--r--   0        0        0     2596 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/30026.ucp
+-rw-r--r--   0        0        0     2433 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/30027.ucp
+-rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/30028.ucp
+-rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/30029.ucp
+-rw-r--r--   0        0        0     3454 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/30030.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/30031.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/30032.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/30033.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/30034.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/30039.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/30040.ucp
+-rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/3012.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/3021.ucp
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/3845.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/3846.ucp
+-rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/3848.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/437.ucp
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/57781.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/58152.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/58210.ucp
+-rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/58335.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/59234.ucp
+-rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/59829.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/60258.ucp
+-rw-r--r--   0        0        0     2189 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/60853.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/61282.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/62306.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/667.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/668.ucp
+-rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/737.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/770.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/771.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/772.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/773.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/774.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/775.ucp
+-rw-r--r--   0        0        0     3970 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/777.ucp
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/778.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/790.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/808.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/848.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/849.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/850.ucp
+-rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/851.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/852.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/853.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/855.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/856.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/857.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/858.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/859.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/860.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/861.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/862.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/863.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/864.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/865.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/866.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/867.ucp
+-rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/869.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/872.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/895.ucp
+-rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/899.ucp
+-rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/991.ucp
+-rw-r--r--   0        0        0     5269 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/README.md
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/__init__.py
+-rw-r--r--   0        0        0     9255 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/iana/Amiga-1251
+-rw-r--r--   0        0        0    13371 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/iana/PTCP154
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/iana/README.md
+-rw-r--r--   0        0        0    14491 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/ibm-cdra/037B34B0.UPMAP100
+-rw-r--r--   0        0        0    11755 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/ibm-cdra/038834B0.UPMAP100
+-rw-r--r--   0        0        0   323573 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/ibm-cdra/039E44B0.UPMAP101
+-rw-r--r--   0        0        0   973501 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/ibm-cdra/039F34B0.UPMAP100
+-rw-r--r--   0        0        0    17655 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/ibm-cdra/readme.txt
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/icu/README.md
+-rw-r--r--   0        0        0   177606 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/icu/aix-KSC5601.1987_0-4.3.6.ucm
+-rw-r--r--   0        0        0  1348868 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/icu/cns-11643-1992.ucm
+-rw-r--r--   0        0        0     7072 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/icu/ibm-1125_P100-1997.ucm
+-rw-r--r--   0        0        0   433127 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/icu/ibm-1375_P100-2008.ucm
+-rw-r--r--   0        0        0     6350 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/icu/ibm-720_P100-1997.ucm
+-rw-r--r--   0        0        0     5972 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/icu/ibm-806_P100-1998.ucm
+-rw-r--r--   0        0        0     7054 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/icu/ibm-851_P100-1995.ucm
+-rw-r--r--   0        0        0     7054 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/icu/ibm-858_P100-1997.ucm
+-rw-r--r--   0        0        0     8451 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/icu/ibm-868_P100-1995.ucm
+-rw-r--r--   0        0        0   199596 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/icu/ibm-932_P120-1999.ucm
+-rw-r--r--   0        0        0   351895 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/icu/windows-1361-2000.ucm
+-rw-r--r--   0        0        0   490901 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/icu/windows-936-2000.ucm
+-rw-r--r--   0        0        0     9995 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/iso-8859/8859-1.TXT
+-rw-r--r--   0        0        0    10385 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/iso-8859/8859-10.TXT
+-rw-r--r--   0        0        0     9192 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/iso-8859/8859-11.TXT
+-rw-r--r--   0        0        0    10026 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/iso-8859/8859-13.TXT
+-rw-r--r--   0        0        0    10459 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/iso-8859/8859-14.TXT
+-rw-r--r--   0        0        0    10039 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/iso-8859/8859-15.TXT
+-rw-r--r--   0        0        0    10390 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/iso-8859/8859-16.TXT
+-rw-r--r--   0        0        0    10219 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/iso-8859/8859-2.TXT
+-rw-r--r--   0        0        0     9901 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/iso-8859/8859-3.TXT
+-rw-r--r--   0        0        0    10195 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/iso-8859/8859-4.TXT
+-rw-r--r--   0        0        0     9830 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/iso-8859/8859-5.TXT
+-rw-r--r--   0        0        0     7723 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/iso-8859/8859-6.TXT
+-rw-r--r--   0        0        0    10053 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/iso-8859/8859-7.TXT
+-rw-r--r--   0        0        0     7943 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/iso-8859/8859-8.TXT
+-rw-r--r--   0        0        0    10030 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/iso-8859/8859-9.TXT
+-rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/iso-8859/ReadMe.txt
+-rw-r--r--   0        0        0     4540 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/ADAMOS7.TXT
+-rw-r--r--   0        0        0     4506 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/ADAMSWTR.TXT
+-rw-r--r--   0        0        0     8879 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/AMSCPC.TXT
+-rw-r--r--   0        0        0    10266 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/AMSCPM.TXT
+-rw-r--r--   0        0        0    10898 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/APL2ALT1.TXT
+-rw-r--r--   0        0        0    10929 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/APL2ALT2.TXT
+-rw-r--r--   0        0        0     6461 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/APL2ICHG.TXT
+-rw-r--r--   0        0        0    11100 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/APL2PRIM.TXT
+-rw-r--r--   0        0        0    10985 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/ATARI8IG.TXT
+-rw-r--r--   0        0        0    11148 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/ATARI8II.TXT
+-rw-r--r--   0        0        0    11734 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/ATARI8VG.TXT
+-rw-r--r--   0        0        0    12144 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/ATARI8VI.TXT
+-rw-r--r--   0        0        0     8280 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/ATARISTI.TXT
+-rw-r--r--   0        0        0     9561 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/ATARISTV.TXT
+-rw-r--r--   0        0        0     7277 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/C64IALT.TXT
+-rw-r--r--   0        0        0     7795 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/C64IPRI.TXT
+-rw-r--r--   0        0        0    11514 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/C64VALT.TXT
+-rw-r--r--   0        0        0    12009 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/C64VPRI.TXT
+-rw-r--r--   0        0        0     9648 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/COCOICHG.TXT
+-rw-r--r--   0        0        0    11149 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/COCOSGR4.TXT
+-rw-r--r--   0        0        0     4792 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/COCOSGR6.TXT
+-rw-r--r--   0        0        0     7263 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/CPETIALT.TXT
+-rw-r--r--   0        0        0     7797 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/CPETIPRI.TXT
+-rw-r--r--   0        0        0    11521 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/CPETVALT.TXT
+-rw-r--r--   0        0        0    12016 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/CPETVPRI.TXT
+-rw-r--r--   0        0        0     7261 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/CVICIALT.TXT
+-rw-r--r--   0        0        0     7795 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/CVICIPRI.TXT
+-rw-r--r--   0        0        0    11514 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/CVICVALT.TXT
+-rw-r--r--   0        0        0    12009 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/CVICVPRI.TXT
+-rw-r--r--   0        0        0     8974 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/IBMPCICH.TXT
+-rw-r--r--   0        0        0    10018 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/IBMPCVID.TXT
+-rw-r--r--   0        0        0     6045 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/MINITLG0.TXT
+-rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/MINITLG1.TXT
+-rw-r--r--   0        0        0     9910 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/MSX.TXT
+-rw-r--r--   0        0        0     3292 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/ORICG0.TXT
+-rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/ORICG1.TXT
+-rw-r--r--   0        0        0     8650 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/RISCEFF.TXT
+-rw-r--r--   0        0        0     8478 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/RISCOSB.TXT
+-rw-r--r--   0        0        0     8363 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/RISCOSI.TXT
+-rw-r--r--   0        0        0    10499 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/RISCOSV.TXT
+-rw-r--r--   0        0        0    14920 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/ReadMe.txt
+-rw-r--r--   0        0        0     9603 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/SINCLRQL.TXT
+-rw-r--r--   0        0        0     3332 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/TELTXTG0.TXT
+-rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/TELTXTG1.TXT
+-rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/TELTXTG2.TXT
+-rw-r--r--   0        0        0     6062 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/TELTXTG3.TXT
+-rw-r--r--   0        0        0     3825 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/TI994A.TXT
+-rw-r--r--   0        0        0     5639 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/TRSM1ICH.TXT
+-rw-r--r--   0        0        0     9089 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/TRSM1ORG.TXT
+-rw-r--r--   0        0        0     9064 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/TRSM1REV.TXT
+-rw-r--r--   0        0        0     7983 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/TRSM3IIN.TXT
+-rw-r--r--   0        0        0     8497 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/TRSM3IJP.TXT
+-rw-r--r--   0        0        0    10398 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/TRSM3IRV.TXT
+-rw-r--r--   0        0        0     9363 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/TRSM3VIN.TXT
+-rw-r--r--   0        0        0     9877 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/TRSM3VJP.TXT
+-rw-r--r--   0        0        0    11778 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/TRSM3VRV.TXT
+-rw-r--r--   0        0        0     8379 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/TRSM4AIA.TXT
+-rw-r--r--   0        0        0     7974 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/TRSM4AIP.TXT
+-rw-r--r--   0        0        0    10398 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/TRSM4AIR.TXT
+-rw-r--r--   0        0        0     9808 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/TRSM4AVA.TXT
+-rw-r--r--   0        0        0     9402 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/TRSM4AVP.TXT
+-rw-r--r--   0        0        0    11826 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/TRSM4AVR.TXT
+-rw-r--r--   0        0        0     5587 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/ZX80.TXT
+-rw-r--r--   0        0        0     5587 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/ZX81.TXT
+-rw-r--r--   0        0        0     4746 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/ZXDESKTP.TXT
+-rw-r--r--   0        0        0     6617 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/ZXFZXKOI.TXT
+-rw-r--r--   0        0        0     7553 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/ZXFZXLT1.TXT
+-rw-r--r--   0        0        0     7590 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/ZXFZXLT5.TXT
+-rw-r--r--   0        0        0     5083 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/ZXFZXPUA.TXT
+-rw-r--r--   0        0        0     8813 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/ZXFZXSLT.TXT
+-rw-r--r--   0        0        0     4331 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/ZXSPCTRM.TXT
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/manual/currency-sign-0x9c.ucp
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/manual/currency-sign-0xdb.ucp
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/manual/dec-vt100.ucp
+-rw-r--r--   0        0        0     8428 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/manual/hp48.txt
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/manual/ibm897graph.ucp
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/manual/mac-cyrillic-pre9.0.ucp
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/manual/mac-system.ucp
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/manual/mac-ukrainian-pre9.0.ucp
+-rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/manual/ms-linedraw.txt
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/manual/russup3.ucp
+-rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/manual/russup4ac.ucp
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/manual/russup4na.ucp
+-rw-r--r--   0        0        0     7901 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/manual/windows-1.0.txt
+-rw-r--r--   0        0        0     8028 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/manual/windows-2.0.txt
+-rw-r--r--   0        0        0     9006 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/manual/windows-3.1.txt
+-rw-r--r--   0        0        0     9000 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/microsoft/EBCDIC/CP037.TXT
+-rw-r--r--   0        0        0     9012 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/microsoft/EBCDIC/CP1026.TXT
+-rw-r--r--   0        0        0     9027 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/microsoft/EBCDIC/CP500.TXT
+-rw-r--r--   0        0        0     8721 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/microsoft/EBCDIC/CP875.TXT
+-rw-r--r--   0        0        0     9177 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/microsoft/MAC/CYRILLIC.TXT
+-rw-r--r--   0        0        0     9413 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/microsoft/MAC/GREEK.TXT
+-rw-r--r--   0        0        0     9253 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/microsoft/MAC/ICELAND.TXT
+-rw-r--r--   0        0        0     9862 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/microsoft/MAC/LATIN2.TXT
+-rw-r--r--   0        0        0     9229 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/microsoft/MAC/ROMAN.TXT
+-rw-r--r--   0        0        0     9251 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/microsoft/MAC/TURKISH.TXT
+-rw-r--r--   0        0        0     9794 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/microsoft/PC/CP437.TXT
+-rw-r--r--   0        0        0     9827 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/microsoft/PC/CP737.TXT
+-rw-r--r--   0        0        0     9766 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/microsoft/PC/CP775.TXT
+-rw-r--r--   0        0        0     9640 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/microsoft/PC/CP850.TXT
+-rw-r--r--   0        0        0     9939 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/microsoft/PC/CP852.TXT
+-rw-r--r--   0        0        0     9562 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/microsoft/PC/CP855.TXT
+-rw-r--r--   0        0        0     9617 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/microsoft/PC/CP857.TXT
+-rw-r--r--   0        0        0     9845 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/microsoft/PC/CP860.TXT
+-rw-r--r--   0        0        0     9826 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/microsoft/PC/CP861.TXT
+-rw-r--r--   0        0        0     9396 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/microsoft/PC/CP862.TXT
+-rw-r--r--   0        0        0     9693 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/microsoft/PC/CP863.TXT
+-rw-r--r--   0        0        0     9560 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/microsoft/PC/CP864.TXT
+-rw-r--r--   0        0        0     9812 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/microsoft/PC/CP865.TXT
+-rw-r--r--   0        0        0     9765 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/microsoft/PC/CP866.TXT
+-rw-r--r--   0        0        0     9318 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/microsoft/PC/CP869.TXT
+-rw-r--r--   0        0        0     8452 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/microsoft/PC/CP874.TXT
+-rw-r--r--   0        0        0     9530 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/microsoft/WINDOWS/CP1250.TXT
+-rw-r--r--   0        0        0     9205 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/microsoft/WINDOWS/CP1251.TXT
+-rw-r--r--   0        0        0     9355 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/microsoft/WINDOWS/CP1252.TXT
+-rw-r--r--   0        0        0     8938 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/microsoft/WINDOWS/CP1253.TXT
+-rw-r--r--   0        0        0     9346 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/microsoft/WINDOWS/CP1254.TXT
+-rw-r--r--   0        0        0     8304 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/microsoft/WINDOWS/CP1255.TXT
+-rw-r--r--   0        0        0     8657 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/microsoft/WINDOWS/CP1256.TXT
+-rw-r--r--   0        0        0     9218 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/microsoft/WINDOWS/CP1257.TXT
+-rw-r--r--   0        0        0     9208 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/microsoft/WINDOWS/CP1258.TXT
+-rw-r--r--   0        0        0     8439 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/microsoft/WINDOWS/CP874.TXT
+-rw-r--r--   0        0        0   295324 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/microsoft/WINDOWS/CP932.TXT
+-rw-r--r--   0        0        0   817310 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/microsoft/WINDOWS/CP936.TXT
+-rw-r--r--   0        0        0   790736 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/microsoft/WINDOWS/CP949.TXT
+-rw-r--r--   0        0        0   508978 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/microsoft/WINDOWS/CP950.TXT
+-rw-r--r--   0        0        0    11537 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/misc/APL-ISO-IR-68.TXT
+-rw-r--r--   0        0        0    21171 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/misc/ATARIST.TXT
+-rw-r--r--   0        0        0    10895 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/misc/CP1006.TXT
+-rw-r--r--   0        0        0     8978 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/misc/CP424.TXT
+-rw-r--r--   0        0        0     9281 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/misc/CP856.TXT
+-rw-r--r--   0        0        0     8707 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/misc/GSM0338.TXT
+-rw-r--r--   0        0        0     3748 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/misc/IBMGRAPH.TXT
+-rw-r--r--   0        0        0   210734 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/misc/JIS0208.TXT
+-rw-r--r--   0        0        0    10692 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/misc/KOI8-R.TXT
+-rw-r--r--   0        0        0    11041 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/misc/KOI8-U.TXT
+-rw-r--r--   0        0        0   784637 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/misc/KPS9566.TXT
+-rw-r--r--   0        0        0    10532 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/misc/KZ1048.TXT
+-rw-r--r--   0        0        0     7093 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/misc/NEXTSTEP.TXT
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/misc/README.md
+-rw-r--r--   0        0        0    49569 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/misc/SGML.TXT
+-rw-r--r--   0        0        0     7054 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/misc/US-ASCII-QUOTES.TXT
+-rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/misc/dashen-map.txt
+-rw-r--r--   0        0        0    92930 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/misc/ibm-ugl.txt
+-rw-r--r--   0        0        0     9996 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/mleisher/ALTVAR.TXT
+-rw-r--r--   0        0        0     4788 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/mleisher/ARMSCII-7.TXT
+-rw-r--r--   0        0        0     8606 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/mleisher/ARMSCII-8.TXT
+-rw-r--r--   0        0        0     9049 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/mleisher/ARMSCII-8A.TXT
+-rw-r--r--   0        0        0     8120 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/mleisher/DECMCS.TXT
+-rw-r--r--   0        0        0     9870 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/mleisher/GEO-ITA.TXT
+-rw-r--r--   0        0        0     9758 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/mleisher/GEO-PS.TXT
+-rw-r--r--   0        0        0    13439 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/mleisher/IRANSYSTEM.TXT
+-rw-r--r--   0        0        0    10796 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/mleisher/KOI8RU.TXT
+-rw-r--r--   0        0        0     9607 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/mleisher/OSNOVAR.TXT
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/mleisher/README.md
+-rw-r--r--   0        0        0     9566 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/mleisher/TIS620.TXT
+-rw-r--r--   0        0        0   274176 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/moztw/big5_2003-b2u.txt
+-rw-r--r--   0        0        0   340277 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/moztw/eten.txt
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/moztw/url
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/python/README.md
+-rw-r--r--   0        0        0    11789 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/python/TCVN5712-1.TXT
+-rw-r--r--   0        0        0    10621 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/python/TCVN5712-2.TXT
+-rw-r--r--   0        0        0     9998 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/python/TCVN5712-3.TXT
+-rw-r--r--   0        0        0    10088 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/vietstd/unicode.html
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/vietstd/url
+-rw-r--r--   0        0        0     7055 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/vietstd/viscii1.1.txt
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/wikipedia/README.md
+-rw-r--r--   0        0        0   156347 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/wikipedia/abicomp.html
+-rw-r--r--   0        0        0   180593 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/wikipedia/brascii.html
+-rw-r--r--   0        0        0   144572 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/wikipedia/cp853.html
+-rw-r--r--   0        0        0   156279 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/wikipedia/cwi2.html
+-rw-r--r--   0        0        0   134679 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/wikipedia/dec-special.html
+-rw-r--r--   0        0        0   153445 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/wikipedia/dec-technical.html
+-rw-r--r--   0        0        0   192405 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/wikipedia/gem.html
+-rw-r--r--   0        0        0   172501 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/wikipedia/kamenicky.html
+-rw-r--r--   0        0        0   216297 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/wikipedia/lics.html
+-rw-r--r--   0        0        0   150793 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/wikipedia/mattel-aquarius.html
+-rw-r--r--   0        0        0   159296 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/wikipedia/mazovia.html
+-rw-r--r--   0        0        0   167964 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/wikipedia/pascii.html
+-rw-r--r--   0        0        0   217224 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/wikipedia/ventura.html
+-rw-r--r--   0        0        0   254035 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/wikipedia/windows-1252.html
+-rw-r--r--   0        0        0   245126 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/wikipedia/wingdings.html
+-rw-r--r--   0        0        0   160779 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/wikipedia/wiscii.html
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/xfonts/README.md
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/xfonts/mulearabic-0.enc
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/xfonts/mulearabic-1.enc
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/xfonts/mulearabic-2.enc
+-rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/xfonts/mulelao-1.enc
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/xfonts/suneu-greek.enc
+-rw-r--r--   0        0        0     7477 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/xfonts/viscii1.1-1.enc
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/containers/__init__.py
+-rw-r--r--   0        0        0     3897 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/containers/compressors.py
+-rw-r--r--   0        0        0     5573 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/containers/container.py
+-rw-r--r--   0        0        0     3224 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/containers/directory.py
+-rw-r--r--   0        0        0    11164 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/containers/mac.py
+-rw-r--r--   0        0        0    14707 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/containers/source.py
+-rw-r--r--   0        0        0     4037 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/containers/tar.py
+-rw-r--r--   0        0        0     3772 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/containers/zip.py
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/__init__.py
+-rw-r--r--   0        0        0    14368 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/amiga.py
+-rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/bbc.py
+-rw-r--r--   0        0        0    41624 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/bdf.py
+-rw-r--r--   0        0        0    41746 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/bmfont.py
+-rw-r--r--   0        0        0     8295 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/borland.py
+-rw-r--r--   0        0        0    22614 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/cpi.py
+-rw-r--r--   0        0        0     6873 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/daisydot.py
+-rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/dashen.py
+-rw-r--r--   0        0        0    13468 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/dec.py
+-rw-r--r--   0        0        0     4052 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/dosstart.py
+-rw-r--r--   0        0        0    11129 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/figlet.py
+-rw-r--r--   0        0        0     6312 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/fontx.py
+-rw-r--r--   0        0        0    11734 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/fzx.py
+-rw-r--r--   0        0        0    26397 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/gdos.py
+-rw-r--r--   0        0        0    12688 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/geos.py
+-rw-r--r--   0        0        0    18471 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/hbf.py
+-rw-r--r--   0        0        0     7349 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/hex.py
+-rw-r--r--   0        0        0     4489 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/hexdraw.py
+-rw-r--r--   0        0        0     3631 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/hurt.py
+-rw-r--r--   0        0        0    10383 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/image.py
+-rw-r--r--   0        0        0     2435 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/mousegraphics.py
+-rw-r--r--   0        0        0     4393 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/mzfon.py
+-rw-r--r--   0        0        0    10427 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/nearlyraw.py
+-rw-r--r--   0        0        0     8294 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/palm.py
+-rw-r--r--   0        0        0    29954 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/pcl.py
+-rw-r--r--   0        0        0     7598 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/pcpaint.py
+-rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/pdf.py
+-rw-r--r--   0        0        0    12848 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/pkfont.py
+-rw-r--r--   0        0        0     2898 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/printshop.py
+-rw-r--r--   0        0        0     5708 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/psf.py
+-rw-r--r--   0        0        0     8138 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/raw.py
+-rw-r--r--   0        0        0    28660 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/sfnt.py
+-rw-r--r--   0        0        0     4934 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/signum.py
+-rw-r--r--   0        0        0     8490 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/svg.py
+-rw-r--r--   0        0        0     6516 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/vfont.py
+-rw-r--r--   0        0        0    14603 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/yaff.py
+-rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/mac/__init__.py
+-rw-r--r--   0        0        0    10477 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/mac/dfont.py
+-rw-r--r--   0        0        0    12772 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/mac/fond.py
+-rw-r--r--   0        0        0     5312 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/mac/iigs.py
+-rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/mac/lisa.py
+-rw-r--r--   0        0        0    22316 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/mac/nfnt.py
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/os2/__init__.py
+-rw-r--r--   0        0        0    21098 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/os2/gpifont.py
+-rw-r--r--   0        0        0    11032 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/os2/lx.py
+-rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/os2/ne.py
+-rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/windows/LICENSE.md
+-rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/windows/__init__.py
+-rw-r--r--   0        0        0    33202 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/windows/fnt.py
+-rw-r--r--   0        0        0     3027 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/windows/mz.py
+-rw-r--r--   0        0        0    14167 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/windows/ne.py
+-rw-r--r--   0        0        0     5394 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/windows/pe.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/scripts/__init__.py
+-rwxr-xr-x   0        0        0     9148 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/scripts/banner.py
+-rwxr-xr-x   0        0        0     3671 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/scripts/convert.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 monobit-0.39.3/.gitignore
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 monobit-0.39.3/LICENSE
+-rw-r--r--   0        0        0    17179 2020-02-02 00:00:00.000000 monobit-0.39.3/README.md
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 monobit-0.39.3/pyproject.toml
+-rw-r--r--   0        0        0    19132 2020-02-02 00:00:00.000000 monobit-0.39.3/PKG-INFO
```

### Comparing `monobit-0.39.2/YAFF.md` & `monobit-0.39.3/YAFF.md`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/explore.py` & `monobit-0.39.3/explore.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/__init__.py` & `monobit-0.39.3/monobit/__init__.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/basetypes.py` & `monobit-0.39.3/monobit/basetypes.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/binary.py` & `monobit-0.39.3/monobit/binary.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/canvas.py` & `monobit-0.39.3/monobit/canvas.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/chart.py` & `monobit-0.39.3/monobit/chart.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/encoding.py` & `monobit-0.39.3/monobit/encoding.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/font.py` & `monobit-0.39.3/monobit/font.py`

 * *Files 0% similar despite different names*

```diff
@@ -904,24 +904,16 @@
             raise ValueError('get_index() takes exactly one parameter.')
         if char is not None:
             label = Char(char)
         elif codepoint is not None:
             label = Codepoint(codepoint)
         elif tag is not None:
             label = Tag(tag)
-        elif isinstance(label, str):
-            # first look for char - expected to be shorter - then tags
-            try:
-                return self._labels[Char(label)]
-            except KeyError:
-                pass
-            try:
-                return self._labels[Tag(label)]
-            except KeyError:
-                pass
+        elif isinstance(label, Label):
+            pass
         # do we have the input string directly as a char or tag?
         elif label is not None:
             # convert strings, numerics through standard rules
             label = to_label(label)
         try:
             return self._labels[label]
         except KeyError:
@@ -1010,14 +1002,15 @@
             if char_from:
                 encoding = char_from.name
             elif codepoint_from:
                 encoding = codepoint_from.name
         kwargs = dict(
             overwrite=overwrite,
             match_whitespace=match_whitespace,
+            match_graphical=match_graphical,
         )
         if codepoint_from:
             kwargs.update(dict(codepoint_from=codepoint_from))
         elif char_from:
             kwargs.update(dict(char_from=char_from))
         elif tag_from:
             kwargs.update(dict(tag_from=tag_from))
```

### Comparing `monobit-0.39.2/monobit/glyph.py` & `monobit-0.39.3/monobit/glyph.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/labels.py` & `monobit-0.39.3/monobit/labels.py`

 * *Files 7% similar despite different names*

```diff
@@ -41,48 +41,54 @@
         return value
     if not isinstance(value, str):
         # only Codepoint can have non-str argument
         return Codepoint(value)
     if not value:
         return Char()
     # protect commas, pluses etc. if enclosed
-    if is_enclosed(value, '"'):
+    try:
         # strip matching double quotes
         # this allows to set a label starting with a digit by quoting it
-        return Tag(value[1:-1])
-    if is_enclosed(value, "'"):
-        return Char(value[1:-1])
+        return Tag(strip_matching(value, '"', allow_no_match=False))
+    except ValueError:
+        pass
+    try:
+        return Char(strip_matching(value, "'", allow_no_match=False))
+    except ValueError:
+        pass
     # codepoints start with an ascii digit
     try:
         return Codepoint(value)
     except ValueError:
         pass
     # length-one -> always a character
     if len(value) == 1:
         return Char(value)
-    # unquoted non-ascii -> always a character
+    # unquoted non-ascii -> always a character (this is to cover grapheme sequences)
     # note that this includes non-printables such as controls but these should not be used.
     if any(ord(_c) > 0x7f for _c in value):
         return Char(value)
-    # deal with other options such as single-quoted, u+codepoint and sequences
+    # deal with other options such as u+codepoint and comma-separated sequences
     try:
         return Char(''.join(
             _convert_char_element(_elem)
             for _elem in value.split(',') if _elem
         ))
     except ValueError:
         pass
     return Tag(value.strip())
 
 def _convert_char_element(element):
     """Convert character label element to char if possible."""
     # string delimited by single quotes denotes a character or sequence
     element = element.strip()
-    if is_enclosed(element, "'"):
-        return element[1:-1]
+    try:
+        return strip_matching(element, "'", allow_no_match=False)
+    except ValueError:
+        pass
     # not a delimited char
     element = element.lower()
     if not element.startswith('u+'):
         raise ValueError(element)
     # convert to sequence of chars
     # this will raise ValueError if not possible
     cp_ord = int(element.strip()[2:], 16)
```

### Comparing `monobit-0.39.2/monobit/magic.py` & `monobit-0.39.3/monobit/magic.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/pack.py` & `monobit-0.39.3/monobit/pack.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/properties.py` & `monobit-0.39.3/monobit/properties.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/raster.py` & `monobit-0.39.3/monobit/raster.py`

 * *Files 1% similar despite different names*

```diff
@@ -227,16 +227,16 @@
         if align.startswith('r'):
             offset = stride - width
         else:
             offset = 0
         excess = len(bitseq) % stride
         if excess:
             if _1 in bitseq[-excess:]:
-                logging.warning(
-                    'Bit string will be truncated by %d bits. Dropping [%s].',
+                raise ValueError(
+                    'Bit string overruns by nonzero %d-bit sequence [%s].',
                     excess, bitseq[-excess:]
                 )
             bitseq = bitseq[:-excess]
         if height is NOT_SET:
             # used as slice bound, None means all
             height = None
         rows = tuple(
```

### Comparing `monobit-0.39.2/monobit/renderer.py` & `monobit-0.39.3/monobit/renderer.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/scripting.py` & `monobit-0.39.3/monobit/scripting.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/storage.py` & `monobit-0.39.3/monobit/storage.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/streams.py` & `monobit-0.39.3/monobit/streams.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/struct.py` & `monobit-0.39.3/monobit/struct.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/taggers.py` & `monobit-0.39.3/monobit/taggers.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/vector.py` & `monobit-0.39.3/monobit/vector.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,16 @@
     @classmethod
     def from_string(cls, pathstr):
         """Build from string representation."""
         elements = pathstr.split()
         # group in triplets
         args = [iter(elements)] * 3
         # raise an error if the path does not cleanly split
-        path = zip(*args, strict=True)
+        #path = zip(*args, strict=True) # python3.10 and above
+        path = zip(*args)
         path = (StrokeMove(_ink, int(_x), int(_y)) for _ink, _x, _y in path)
         return cls(path)
 
     def flip(self):
         """Flip vertically about path origin."""
         return type(self)((_ink, _x, -_y) for _ink, _x, _y in self._path)
```

### Comparing `monobit-0.39.2/monobit/charmaps/adobe/ReadMe.txt` & `monobit-0.39.3/monobit/charmaps/adobe/ReadMe.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/adobe/stdenc.txt` & `monobit-0.39.3/monobit/charmaps/adobe/stdenc.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/adobe/symbol.txt` & `monobit-0.39.3/monobit/charmaps/adobe/symbol.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/adobe/zdingbat.txt` & `monobit-0.39.3/monobit/charmaps/adobe/zdingbat.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/agl/LICENSE.md` & `monobit-0.39.3/monobit/charmaps/agl/LICENSE.md`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/agl/README.md` & `monobit-0.39.3/monobit/charmaps/agl/README.md`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/agl/aglfn.txt` & `monobit-0.39.3/monobit/charmaps/agl/aglfn.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/agl/glyphlist.txt` & `monobit-0.39.3/monobit/charmaps/agl/glyphlist.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/apple/ARABIC.TXT` & `monobit-0.39.3/monobit/charmaps/apple/ARABIC.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/apple/CELTIC.TXT` & `monobit-0.39.3/monobit/charmaps/apple/CELTIC.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/apple/CENTEURO.TXT` & `monobit-0.39.3/monobit/charmaps/apple/CENTEURO.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/apple/CHINSIMP.TXT` & `monobit-0.39.3/monobit/charmaps/apple/CHINSIMP.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/apple/CHINTRAD.TXT` & `monobit-0.39.3/monobit/charmaps/apple/CHINTRAD.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/apple/CORPCHAR.TXT` & `monobit-0.39.3/monobit/charmaps/apple/CORPCHAR.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/apple/CROATIAN.TXT` & `monobit-0.39.3/monobit/charmaps/apple/CROATIAN.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/apple/CYRILLIC.TXT` & `monobit-0.39.3/monobit/charmaps/apple/CYRILLIC.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/apple/DEVANAGA.TXT` & `monobit-0.39.3/monobit/charmaps/apple/DEVANAGA.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/apple/DINGBATS.TXT` & `monobit-0.39.3/monobit/charmaps/apple/DINGBATS.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/apple/FARSI.TXT` & `monobit-0.39.3/monobit/charmaps/apple/FARSI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/apple/GAELIC.TXT` & `monobit-0.39.3/monobit/charmaps/apple/GAELIC.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/apple/GREEK.TXT` & `monobit-0.39.3/monobit/charmaps/apple/GREEK.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/apple/GUJARATI.TXT` & `monobit-0.39.3/monobit/charmaps/apple/GUJARATI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/apple/GURMUKHI.TXT` & `monobit-0.39.3/monobit/charmaps/apple/GURMUKHI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/apple/HEBREW.TXT` & `monobit-0.39.3/monobit/charmaps/apple/HEBREW.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/apple/ICELAND.TXT` & `monobit-0.39.3/monobit/charmaps/apple/ICELAND.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/apple/INUIT.TXT` & `monobit-0.39.3/monobit/charmaps/apple/INUIT.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/apple/JAPANESE.TXT` & `monobit-0.39.3/monobit/charmaps/apple/JAPANESE.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/apple/KEYBOARD.TXT` & `monobit-0.39.3/monobit/charmaps/apple/KEYBOARD.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/apple/KOREAN.TXT` & `monobit-0.39.3/monobit/charmaps/apple/KOREAN.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/apple/ROMAN.TXT` & `monobit-0.39.3/monobit/charmaps/apple/ROMAN.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/apple/ROMANIAN.TXT` & `monobit-0.39.3/monobit/charmaps/apple/ROMANIAN.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/apple/ReadMe.txt` & `monobit-0.39.3/monobit/charmaps/apple/ReadMe.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/apple/SYMBOL.TXT` & `monobit-0.39.3/monobit/charmaps/apple/SYMBOL.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/apple/THAI.TXT` & `monobit-0.39.3/monobit/charmaps/apple/THAI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/apple/TURKISH.TXT` & `monobit-0.39.3/monobit/charmaps/apple/TURKISH.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/apple/UKRAINE.TXT` & `monobit-0.39.3/monobit/charmaps/apple/UKRAINE.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/czyborra/README.md` & `monobit-0.39.3/monobit/charmaps/czyborra/README.md`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/czyborra/bulgarian-mik.txt` & `monobit-0.39.3/monobit/charmaps/czyborra/bulgarian-mik.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/czyborra/cp866.txt` & `monobit-0.39.3/monobit/charmaps/czyborra/cp866.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/czyborra/gost19768-87.txt` & `monobit-0.39.3/monobit/charmaps/czyborra/gost19768-87.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/czyborra/hp-roman8.txt` & `monobit-0.39.3/monobit/charmaps/czyborra/hp-roman8.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/czyborra/koi-0.txt` & `monobit-0.39.3/monobit/charmaps/czyborra/koi-0.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/czyborra/koi-7.txt` & `monobit-0.39.3/monobit/charmaps/czyborra/koi-7.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/czyborra/koi8-a.txt` & `monobit-0.39.3/monobit/charmaps/czyborra/koi8-a.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/czyborra/koi8-b.txt` & `monobit-0.39.3/monobit/charmaps/czyborra/koi8-b.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/czyborra/koi8-e.txt` & `monobit-0.39.3/monobit/charmaps/czyborra/koi8-e.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/czyborra/koi8-f.txt` & `monobit-0.39.3/monobit/charmaps/czyborra/koi8-f.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/czyborra/koi8-r.txt` & `monobit-0.39.3/monobit/charmaps/czyborra/koi8-r.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/czyborra/koi8-u.txt` & `monobit-0.39.3/monobit/charmaps/czyborra/koi8-u.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/dkuug/iso646-ca` & `monobit-0.39.3/monobit/charmaps/dkuug/iso646-ca`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/dkuug/iso646-ca2` & `monobit-0.39.3/monobit/charmaps/dkuug/iso646-ca2`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/dkuug/iso646-cn` & `monobit-0.39.3/monobit/charmaps/dkuug/iso646-cn`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/dkuug/iso646-cu` & `monobit-0.39.3/monobit/charmaps/dkuug/iso646-cu`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/dkuug/iso646-de` & `monobit-0.39.3/monobit/charmaps/dkuug/iso646-de`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/dkuug/iso646-dk` & `monobit-0.39.3/monobit/charmaps/dkuug/iso646-dk`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/dkuug/iso646-es` & `monobit-0.39.3/monobit/charmaps/dkuug/iso646-es`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/dkuug/iso646-es2` & `monobit-0.39.3/monobit/charmaps/dkuug/iso646-es2`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/dkuug/iso646-fr` & `monobit-0.39.3/monobit/charmaps/dkuug/iso646-fr`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/dkuug/iso646-gb` & `monobit-0.39.3/monobit/charmaps/dkuug/iso646-gb`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/dkuug/iso646-hu` & `monobit-0.39.3/monobit/charmaps/dkuug/iso646-hu`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/dkuug/iso646-it` & `monobit-0.39.3/monobit/charmaps/dkuug/iso646-it`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/dkuug/iso646-jp` & `monobit-0.39.3/monobit/charmaps/dkuug/iso646-jp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/dkuug/iso646-jp-ocr-b` & `monobit-0.39.3/monobit/charmaps/dkuug/iso646-jp-ocr-b`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/dkuug/iso646-kr` & `monobit-0.39.3/monobit/charmaps/dkuug/iso646-kr`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/dkuug/iso646-us` & `monobit-0.39.3/monobit/charmaps/dkuug/iso646-us`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/dkuug/iso646-yu` & `monobit-0.39.3/monobit/charmaps/dkuug/iso646-yu`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/dkuug/jis_x0201` & `monobit-0.39.3/monobit/charmaps/dkuug/jis_x0201`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/dkuug/x0201-7` & `monobit-0.39.3/monobit/charmaps/dkuug/x0201-7`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/emacs/MULE-ethiopic.map` & `monobit-0.39.3/monobit/charmaps/emacs/MULE-ethiopic.map`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/emacs/MULE-ipa.map` & `monobit-0.39.3/monobit/charmaps/emacs/MULE-ipa.map`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/emacs/MULE-is13194.map` & `monobit-0.39.3/monobit/charmaps/emacs/MULE-is13194.map`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/emacs/MULE-lviscii.map` & `monobit-0.39.3/monobit/charmaps/emacs/MULE-lviscii.map`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/emacs/MULE-sisheng.map` & `monobit-0.39.3/monobit/charmaps/emacs/MULE-sisheng.map`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/emacs/MULE-tibetan.map` & `monobit-0.39.3/monobit/charmaps/emacs/MULE-tibetan.map`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/emacs/MULE-uviscii.map` & `monobit-0.39.3/monobit/charmaps/emacs/MULE-uviscii.map`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/emacs/README.md` & `monobit-0.39.3/monobit/charmaps/emacs/README.md`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/evertype/ARMENIAN.TXT` & `monobit-0.39.3/monobit/charmaps/evertype/ARMENIAN.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/evertype/GEORGIAN.TXT` & `monobit-0.39.3/monobit/charmaps/evertype/GEORGIAN.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/evertype/README.md` & `monobit-0.39.3/monobit/charmaps/evertype/README.md`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/1116.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/1116.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/1117.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/1117.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/1118.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/1118.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/1119.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/1119.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/1125.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/1125.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/113.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/113.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/1131.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/1131.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/30000.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/30000.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/30001.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/30001.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/30002.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/30002.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/30003.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/30003.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/30004.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/30004.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/30005.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/30005.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/30006.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/30006.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/30007.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/30007.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/30008.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/30008.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/30009.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/30009.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/30010.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/30010.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/30011.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/30011.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/30012.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/30012.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/30013.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/30013.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/30014.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/30014.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/30015.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/30015.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/30016.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/30016.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/30017.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/30017.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/30018.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/30018.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/30019.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/30019.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/30020.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/30020.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/30021.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/30021.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/30022.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/30022.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/30023.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/30023.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/30024.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/30024.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/30025.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/30025.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/30026.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/30026.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/30027.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/30027.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/30028.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/30028.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/30029.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/30029.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/30030.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/30030.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/30031.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/30031.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/30032.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/30032.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/30033.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/30033.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/30034.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/30034.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/30039.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/30039.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/30040.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/30040.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/3012.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/3012.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/3021.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/3021.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/3845.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/3845.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/3846.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/3846.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/3848.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/3848.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/437.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/437.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/57781.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/57781.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/58152.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/58152.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/58210.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/58210.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/58335.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/58335.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/59234.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/59234.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/59829.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/59829.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/60258.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/60258.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/60853.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/60853.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/61282.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/61282.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/62306.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/62306.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/667.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/667.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/668.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/668.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/737.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/737.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/770.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/770.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/771.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/771.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/772.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/772.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/773.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/773.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/774.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/774.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/775.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/775.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/777.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/777.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/778.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/778.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/790.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/790.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/808.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/808.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/848.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/848.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/849.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/849.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/850.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/850.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/851.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/851.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/852.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/852.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/853.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/853.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/855.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/855.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/856.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/856.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/857.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/857.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/858.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/858.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/859.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/859.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/860.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/860.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/861.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/861.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/862.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/862.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/863.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/863.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/864.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/864.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/865.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/865.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/866.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/866.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/867.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/867.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/869.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/869.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/872.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/872.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/895.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/895.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/899.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/899.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/991.ucp` & `monobit-0.39.3/monobit/charmaps/freedos/991.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/freedos/README.md` & `monobit-0.39.3/monobit/charmaps/freedos/README.md`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/iana/Amiga-1251` & `monobit-0.39.3/monobit/charmaps/iana/Amiga-1251`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/iana/PTCP154` & `monobit-0.39.3/monobit/charmaps/iana/PTCP154`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/ibm-cdra/037B34B0.UPMAP100` & `monobit-0.39.3/monobit/charmaps/ibm-cdra/037B34B0.UPMAP100`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/ibm-cdra/038834B0.UPMAP100` & `monobit-0.39.3/monobit/charmaps/ibm-cdra/038834B0.UPMAP100`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/ibm-cdra/039E44B0.UPMAP101` & `monobit-0.39.3/monobit/charmaps/ibm-cdra/039E44B0.UPMAP101`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/ibm-cdra/039F34B0.UPMAP100` & `monobit-0.39.3/monobit/charmaps/ibm-cdra/039F34B0.UPMAP100`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/ibm-cdra/readme.txt` & `monobit-0.39.3/monobit/charmaps/ibm-cdra/readme.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/icu/README.md` & `monobit-0.39.3/monobit/charmaps/icu/README.md`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/icu/aix-KSC5601.1987_0-4.3.6.ucm` & `monobit-0.39.3/monobit/charmaps/icu/aix-KSC5601.1987_0-4.3.6.ucm`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/icu/cns-11643-1992.ucm` & `monobit-0.39.3/monobit/charmaps/icu/cns-11643-1992.ucm`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/icu/ibm-1125_P100-1997.ucm` & `monobit-0.39.3/monobit/charmaps/icu/ibm-1125_P100-1997.ucm`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/icu/ibm-1375_P100-2008.ucm` & `monobit-0.39.3/monobit/charmaps/icu/ibm-1375_P100-2008.ucm`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/icu/ibm-720_P100-1997.ucm` & `monobit-0.39.3/monobit/charmaps/icu/ibm-720_P100-1997.ucm`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/icu/ibm-806_P100-1998.ucm` & `monobit-0.39.3/monobit/charmaps/icu/ibm-806_P100-1998.ucm`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/icu/ibm-851_P100-1995.ucm` & `monobit-0.39.3/monobit/charmaps/icu/ibm-851_P100-1995.ucm`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/icu/ibm-858_P100-1997.ucm` & `monobit-0.39.3/monobit/charmaps/icu/ibm-858_P100-1997.ucm`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/icu/ibm-868_P100-1995.ucm` & `monobit-0.39.3/monobit/charmaps/icu/ibm-868_P100-1995.ucm`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/icu/ibm-932_P120-1999.ucm` & `monobit-0.39.3/monobit/charmaps/icu/ibm-932_P120-1999.ucm`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/icu/windows-1361-2000.ucm` & `monobit-0.39.3/monobit/charmaps/icu/windows-1361-2000.ucm`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/icu/windows-936-2000.ucm` & `monobit-0.39.3/monobit/charmaps/icu/windows-936-2000.ucm`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/iso-8859/8859-1.TXT` & `monobit-0.39.3/monobit/charmaps/iso-8859/8859-1.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/iso-8859/8859-10.TXT` & `monobit-0.39.3/monobit/charmaps/iso-8859/8859-10.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/iso-8859/8859-11.TXT` & `monobit-0.39.3/monobit/charmaps/iso-8859/8859-11.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/iso-8859/8859-13.TXT` & `monobit-0.39.3/monobit/charmaps/iso-8859/8859-13.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/iso-8859/8859-14.TXT` & `monobit-0.39.3/monobit/charmaps/iso-8859/8859-14.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/iso-8859/8859-15.TXT` & `monobit-0.39.3/monobit/charmaps/iso-8859/8859-15.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/iso-8859/8859-16.TXT` & `monobit-0.39.3/monobit/charmaps/iso-8859/8859-16.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/iso-8859/8859-2.TXT` & `monobit-0.39.3/monobit/charmaps/iso-8859/8859-2.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/iso-8859/8859-3.TXT` & `monobit-0.39.3/monobit/charmaps/iso-8859/8859-3.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/iso-8859/8859-4.TXT` & `monobit-0.39.3/monobit/charmaps/iso-8859/8859-4.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/iso-8859/8859-5.TXT` & `monobit-0.39.3/monobit/charmaps/iso-8859/8859-5.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/iso-8859/8859-6.TXT` & `monobit-0.39.3/monobit/charmaps/iso-8859/8859-6.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/iso-8859/8859-7.TXT` & `monobit-0.39.3/monobit/charmaps/iso-8859/8859-7.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/iso-8859/8859-8.TXT` & `monobit-0.39.3/monobit/charmaps/iso-8859/8859-8.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/iso-8859/8859-9.TXT` & `monobit-0.39.3/monobit/charmaps/iso-8859/8859-9.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/iso-8859/ReadMe.txt` & `monobit-0.39.3/monobit/charmaps/iso-8859/ReadMe.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/kreativekorp/ADAMOS7.TXT` & `monobit-0.39.3/monobit/charmaps/kreativekorp/ADAMOS7.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/kreativekorp/ADAMSWTR.TXT` & `monobit-0.39.3/monobit/charmaps/kreativekorp/ADAMSWTR.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/kreativekorp/AMSCPC.TXT` & `monobit-0.39.3/monobit/charmaps/kreativekorp/AMSCPC.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/kreativekorp/AMSCPM.TXT` & `monobit-0.39.3/monobit/charmaps/kreativekorp/AMSCPM.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/kreativekorp/APL2ALT1.TXT` & `monobit-0.39.3/monobit/charmaps/kreativekorp/APL2ALT1.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/kreativekorp/APL2ALT2.TXT` & `monobit-0.39.3/monobit/charmaps/kreativekorp/APL2ALT2.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/kreativekorp/APL2ICHG.TXT` & `monobit-0.39.3/monobit/charmaps/kreativekorp/APL2ICHG.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/kreativekorp/APL2PRIM.TXT` & `monobit-0.39.3/monobit/charmaps/kreativekorp/APL2PRIM.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/kreativekorp/ATARI8IG.TXT` & `monobit-0.39.3/monobit/charmaps/kreativekorp/ATARI8IG.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/kreativekorp/ATARI8II.TXT` & `monobit-0.39.3/monobit/charmaps/kreativekorp/ATARI8II.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/kreativekorp/ATARI8VG.TXT` & `monobit-0.39.3/monobit/charmaps/kreativekorp/ATARI8VG.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/kreativekorp/ATARI8VI.TXT` & `monobit-0.39.3/monobit/charmaps/kreativekorp/ATARI8VI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/kreativekorp/ATARISTI.TXT` & `monobit-0.39.3/monobit/charmaps/kreativekorp/ATARISTI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/kreativekorp/ATARISTV.TXT` & `monobit-0.39.3/monobit/charmaps/kreativekorp/ATARISTV.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/kreativekorp/C64IALT.TXT` & `monobit-0.39.3/monobit/charmaps/kreativekorp/C64IALT.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/kreativekorp/C64IPRI.TXT` & `monobit-0.39.3/monobit/charmaps/kreativekorp/C64IPRI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/kreativekorp/C64VALT.TXT` & `monobit-0.39.3/monobit/charmaps/kreativekorp/C64VALT.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/kreativekorp/C64VPRI.TXT` & `monobit-0.39.3/monobit/charmaps/kreativekorp/C64VPRI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/kreativekorp/COCOICHG.TXT` & `monobit-0.39.3/monobit/charmaps/kreativekorp/COCOICHG.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/kreativekorp/COCOSGR4.TXT` & `monobit-0.39.3/monobit/charmaps/kreativekorp/COCOSGR4.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/kreativekorp/COCOSGR6.TXT` & `monobit-0.39.3/monobit/charmaps/kreativekorp/COCOSGR6.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/kreativekorp/CPETIALT.TXT` & `monobit-0.39.3/monobit/charmaps/kreativekorp/CPETIALT.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/kreativekorp/CPETIPRI.TXT` & `monobit-0.39.3/monobit/charmaps/kreativekorp/CPETIPRI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/kreativekorp/CPETVALT.TXT` & `monobit-0.39.3/monobit/charmaps/kreativekorp/CPETVALT.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/kreativekorp/CPETVPRI.TXT` & `monobit-0.39.3/monobit/charmaps/kreativekorp/CPETVPRI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/kreativekorp/CVICIALT.TXT` & `monobit-0.39.3/monobit/charmaps/kreativekorp/CVICIALT.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/kreativekorp/CVICIPRI.TXT` & `monobit-0.39.3/monobit/charmaps/kreativekorp/CVICIPRI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/kreativekorp/CVICVALT.TXT` & `monobit-0.39.3/monobit/charmaps/kreativekorp/CVICVALT.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/kreativekorp/CVICVPRI.TXT` & `monobit-0.39.3/monobit/charmaps/kreativekorp/CVICVPRI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/kreativekorp/IBMPCICH.TXT` & `monobit-0.39.3/monobit/charmaps/kreativekorp/IBMPCICH.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/kreativekorp/IBMPCVID.TXT` & `monobit-0.39.3/monobit/charmaps/kreativekorp/IBMPCVID.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/kreativekorp/MINITLG0.TXT` & `monobit-0.39.3/monobit/charmaps/kreativekorp/MINITLG0.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/kreativekorp/MINITLG1.TXT` & `monobit-0.39.3/monobit/charmaps/kreativekorp/MINITLG1.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/kreativekorp/MSX.TXT` & `monobit-0.39.3/monobit/charmaps/kreativekorp/MSX.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/kreativekorp/ORICG0.TXT` & `monobit-0.39.3/monobit/charmaps/kreativekorp/ORICG0.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/kreativekorp/ORICG1.TXT` & `monobit-0.39.3/monobit/charmaps/kreativekorp/ORICG1.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/kreativekorp/RISCEFF.TXT` & `monobit-0.39.3/monobit/charmaps/kreativekorp/RISCEFF.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/kreativekorp/RISCOSB.TXT` & `monobit-0.39.3/monobit/charmaps/kreativekorp/RISCOSB.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/kreativekorp/RISCOSI.TXT` & `monobit-0.39.3/monobit/charmaps/kreativekorp/RISCOSI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/kreativekorp/RISCOSV.TXT` & `monobit-0.39.3/monobit/charmaps/kreativekorp/RISCOSV.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/kreativekorp/ReadMe.txt` & `monobit-0.39.3/monobit/charmaps/kreativekorp/ReadMe.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/kreativekorp/SINCLRQL.TXT` & `monobit-0.39.3/monobit/charmaps/kreativekorp/SINCLRQL.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/kreativekorp/TELTXTG0.TXT` & `monobit-0.39.3/monobit/charmaps/kreativekorp/TELTXTG0.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/kreativekorp/TELTXTG1.TXT` & `monobit-0.39.3/monobit/charmaps/kreativekorp/TELTXTG1.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/kreativekorp/TELTXTG2.TXT` & `monobit-0.39.3/monobit/charmaps/kreativekorp/TELTXTG2.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/kreativekorp/TELTXTG3.TXT` & `monobit-0.39.3/monobit/charmaps/kreativekorp/TELTXTG3.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/kreativekorp/TI994A.TXT` & `monobit-0.39.3/monobit/charmaps/kreativekorp/TI994A.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/kreativekorp/TRSM1ICH.TXT` & `monobit-0.39.3/monobit/charmaps/kreativekorp/TRSM1ICH.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/kreativekorp/TRSM1ORG.TXT` & `monobit-0.39.3/monobit/charmaps/kreativekorp/TRSM1ORG.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/kreativekorp/TRSM1REV.TXT` & `monobit-0.39.3/monobit/charmaps/kreativekorp/TRSM1REV.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/kreativekorp/TRSM3IIN.TXT` & `monobit-0.39.3/monobit/charmaps/kreativekorp/TRSM3IIN.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/kreativekorp/TRSM3IJP.TXT` & `monobit-0.39.3/monobit/charmaps/kreativekorp/TRSM3IJP.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/kreativekorp/TRSM3IRV.TXT` & `monobit-0.39.3/monobit/charmaps/kreativekorp/TRSM3IRV.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/kreativekorp/TRSM3VIN.TXT` & `monobit-0.39.3/monobit/charmaps/kreativekorp/TRSM3VIN.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/kreativekorp/TRSM3VJP.TXT` & `monobit-0.39.3/monobit/charmaps/kreativekorp/TRSM3VJP.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/kreativekorp/TRSM3VRV.TXT` & `monobit-0.39.3/monobit/charmaps/kreativekorp/TRSM3VRV.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/kreativekorp/TRSM4AIA.TXT` & `monobit-0.39.3/monobit/charmaps/kreativekorp/TRSM4AIA.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/kreativekorp/TRSM4AIP.TXT` & `monobit-0.39.3/monobit/charmaps/kreativekorp/TRSM4AIP.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/kreativekorp/TRSM4AIR.TXT` & `monobit-0.39.3/monobit/charmaps/kreativekorp/TRSM4AIR.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/kreativekorp/TRSM4AVA.TXT` & `monobit-0.39.3/monobit/charmaps/kreativekorp/TRSM4AVA.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/kreativekorp/TRSM4AVP.TXT` & `monobit-0.39.3/monobit/charmaps/kreativekorp/TRSM4AVP.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/kreativekorp/TRSM4AVR.TXT` & `monobit-0.39.3/monobit/charmaps/kreativekorp/TRSM4AVR.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/kreativekorp/ZX80.TXT` & `monobit-0.39.3/monobit/charmaps/kreativekorp/ZX80.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/kreativekorp/ZX81.TXT` & `monobit-0.39.3/monobit/charmaps/kreativekorp/ZX81.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/kreativekorp/ZXDESKTP.TXT` & `monobit-0.39.3/monobit/charmaps/kreativekorp/ZXDESKTP.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/kreativekorp/ZXFZXKOI.TXT` & `monobit-0.39.3/monobit/charmaps/kreativekorp/ZXFZXKOI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/kreativekorp/ZXFZXLT1.TXT` & `monobit-0.39.3/monobit/charmaps/kreativekorp/ZXFZXLT1.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/kreativekorp/ZXFZXLT5.TXT` & `monobit-0.39.3/monobit/charmaps/kreativekorp/ZXFZXLT5.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/kreativekorp/ZXFZXPUA.TXT` & `monobit-0.39.3/monobit/charmaps/kreativekorp/ZXFZXPUA.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/kreativekorp/ZXFZXSLT.TXT` & `monobit-0.39.3/monobit/charmaps/kreativekorp/ZXFZXSLT.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/kreativekorp/ZXSPCTRM.TXT` & `monobit-0.39.3/monobit/charmaps/kreativekorp/ZXSPCTRM.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/manual/dec-vt100.ucp` & `monobit-0.39.3/monobit/charmaps/manual/dec-vt100.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/manual/hp48.txt` & `monobit-0.39.3/monobit/charmaps/manual/hp48.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/manual/ibm897graph.ucp` & `monobit-0.39.3/monobit/charmaps/manual/ibm897graph.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/manual/mac-system.ucp` & `monobit-0.39.3/monobit/charmaps/manual/mac-system.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/manual/ms-linedraw.txt` & `monobit-0.39.3/monobit/charmaps/manual/ms-linedraw.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/manual/russup3.ucp` & `monobit-0.39.3/monobit/charmaps/manual/russup3.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/manual/russup4ac.ucp` & `monobit-0.39.3/monobit/charmaps/manual/russup4ac.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/manual/russup4na.ucp` & `monobit-0.39.3/monobit/charmaps/manual/russup4na.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/manual/windows-1.0.txt` & `monobit-0.39.3/monobit/charmaps/manual/windows-1.0.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/manual/windows-2.0.txt` & `monobit-0.39.3/monobit/charmaps/manual/windows-2.0.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/manual/windows-3.1.txt` & `monobit-0.39.3/monobit/charmaps/manual/windows-3.1.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/microsoft/EBCDIC/CP037.TXT` & `monobit-0.39.3/monobit/charmaps/microsoft/EBCDIC/CP037.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/microsoft/EBCDIC/CP1026.TXT` & `monobit-0.39.3/monobit/charmaps/microsoft/EBCDIC/CP1026.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/microsoft/EBCDIC/CP500.TXT` & `monobit-0.39.3/monobit/charmaps/microsoft/EBCDIC/CP500.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/microsoft/EBCDIC/CP875.TXT` & `monobit-0.39.3/monobit/charmaps/microsoft/EBCDIC/CP875.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/microsoft/MAC/CYRILLIC.TXT` & `monobit-0.39.3/monobit/charmaps/microsoft/MAC/CYRILLIC.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/microsoft/MAC/GREEK.TXT` & `monobit-0.39.3/monobit/charmaps/microsoft/MAC/GREEK.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/microsoft/MAC/ICELAND.TXT` & `monobit-0.39.3/monobit/charmaps/microsoft/MAC/ICELAND.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/microsoft/MAC/LATIN2.TXT` & `monobit-0.39.3/monobit/charmaps/microsoft/MAC/LATIN2.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/microsoft/MAC/ROMAN.TXT` & `monobit-0.39.3/monobit/charmaps/microsoft/MAC/ROMAN.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/microsoft/MAC/TURKISH.TXT` & `monobit-0.39.3/monobit/charmaps/microsoft/MAC/TURKISH.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/microsoft/PC/CP437.TXT` & `monobit-0.39.3/monobit/charmaps/microsoft/PC/CP437.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/microsoft/PC/CP737.TXT` & `monobit-0.39.3/monobit/charmaps/microsoft/PC/CP737.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/microsoft/PC/CP775.TXT` & `monobit-0.39.3/monobit/charmaps/microsoft/PC/CP775.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/microsoft/PC/CP850.TXT` & `monobit-0.39.3/monobit/charmaps/microsoft/PC/CP850.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/microsoft/PC/CP852.TXT` & `monobit-0.39.3/monobit/charmaps/microsoft/PC/CP852.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/microsoft/PC/CP855.TXT` & `monobit-0.39.3/monobit/charmaps/microsoft/PC/CP855.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/microsoft/PC/CP857.TXT` & `monobit-0.39.3/monobit/charmaps/microsoft/PC/CP857.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/microsoft/PC/CP860.TXT` & `monobit-0.39.3/monobit/charmaps/microsoft/PC/CP860.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/microsoft/PC/CP861.TXT` & `monobit-0.39.3/monobit/charmaps/microsoft/PC/CP861.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/microsoft/PC/CP862.TXT` & `monobit-0.39.3/monobit/charmaps/microsoft/PC/CP862.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/microsoft/PC/CP863.TXT` & `monobit-0.39.3/monobit/charmaps/microsoft/PC/CP863.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/microsoft/PC/CP864.TXT` & `monobit-0.39.3/monobit/charmaps/microsoft/PC/CP864.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/microsoft/PC/CP865.TXT` & `monobit-0.39.3/monobit/charmaps/microsoft/PC/CP865.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/microsoft/PC/CP866.TXT` & `monobit-0.39.3/monobit/charmaps/microsoft/PC/CP866.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/microsoft/PC/CP869.TXT` & `monobit-0.39.3/monobit/charmaps/microsoft/PC/CP869.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/microsoft/PC/CP874.TXT` & `monobit-0.39.3/monobit/charmaps/microsoft/PC/CP874.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/microsoft/WINDOWS/CP1250.TXT` & `monobit-0.39.3/monobit/charmaps/microsoft/WINDOWS/CP1250.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/microsoft/WINDOWS/CP1251.TXT` & `monobit-0.39.3/monobit/charmaps/microsoft/WINDOWS/CP1251.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/microsoft/WINDOWS/CP1252.TXT` & `monobit-0.39.3/monobit/charmaps/microsoft/WINDOWS/CP1252.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/microsoft/WINDOWS/CP1253.TXT` & `monobit-0.39.3/monobit/charmaps/microsoft/WINDOWS/CP1253.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/microsoft/WINDOWS/CP1254.TXT` & `monobit-0.39.3/monobit/charmaps/microsoft/WINDOWS/CP1254.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/microsoft/WINDOWS/CP1255.TXT` & `monobit-0.39.3/monobit/charmaps/microsoft/WINDOWS/CP1255.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/microsoft/WINDOWS/CP1256.TXT` & `monobit-0.39.3/monobit/charmaps/microsoft/WINDOWS/CP1256.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/microsoft/WINDOWS/CP1257.TXT` & `monobit-0.39.3/monobit/charmaps/microsoft/WINDOWS/CP1257.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/microsoft/WINDOWS/CP1258.TXT` & `monobit-0.39.3/monobit/charmaps/microsoft/WINDOWS/CP1258.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/microsoft/WINDOWS/CP874.TXT` & `monobit-0.39.3/monobit/charmaps/microsoft/WINDOWS/CP874.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/microsoft/WINDOWS/CP932.TXT` & `monobit-0.39.3/monobit/charmaps/microsoft/WINDOWS/CP932.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/microsoft/WINDOWS/CP936.TXT` & `monobit-0.39.3/monobit/charmaps/microsoft/WINDOWS/CP936.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/microsoft/WINDOWS/CP949.TXT` & `monobit-0.39.3/monobit/charmaps/microsoft/WINDOWS/CP949.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/microsoft/WINDOWS/CP950.TXT` & `monobit-0.39.3/monobit/charmaps/microsoft/WINDOWS/CP950.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/misc/APL-ISO-IR-68.TXT` & `monobit-0.39.3/monobit/charmaps/misc/APL-ISO-IR-68.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/misc/ATARIST.TXT` & `monobit-0.39.3/monobit/charmaps/misc/ATARIST.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/misc/CP1006.TXT` & `monobit-0.39.3/monobit/charmaps/misc/CP1006.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/misc/CP424.TXT` & `monobit-0.39.3/monobit/charmaps/misc/CP424.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/misc/CP856.TXT` & `monobit-0.39.3/monobit/charmaps/misc/CP856.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/misc/GSM0338.TXT` & `monobit-0.39.3/monobit/charmaps/misc/GSM0338.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/misc/IBMGRAPH.TXT` & `monobit-0.39.3/monobit/charmaps/misc/IBMGRAPH.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/misc/JIS0208.TXT` & `monobit-0.39.3/monobit/charmaps/misc/JIS0208.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/misc/KOI8-R.TXT` & `monobit-0.39.3/monobit/charmaps/misc/KOI8-R.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/misc/KOI8-U.TXT` & `monobit-0.39.3/monobit/charmaps/misc/KOI8-U.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/misc/KPS9566.TXT` & `monobit-0.39.3/monobit/charmaps/misc/KPS9566.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/misc/KZ1048.TXT` & `monobit-0.39.3/monobit/charmaps/misc/KZ1048.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/misc/NEXTSTEP.TXT` & `monobit-0.39.3/monobit/charmaps/misc/NEXTSTEP.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/misc/SGML.TXT` & `monobit-0.39.3/monobit/charmaps/misc/SGML.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/misc/US-ASCII-QUOTES.TXT` & `monobit-0.39.3/monobit/charmaps/misc/US-ASCII-QUOTES.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/misc/dashen-map.txt` & `monobit-0.39.3/monobit/charmaps/misc/dashen-map.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/misc/ibm-ugl.txt` & `monobit-0.39.3/monobit/charmaps/misc/ibm-ugl.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/mleisher/ALTVAR.TXT` & `monobit-0.39.3/monobit/charmaps/mleisher/ALTVAR.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/mleisher/ARMSCII-7.TXT` & `monobit-0.39.3/monobit/charmaps/mleisher/ARMSCII-7.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/mleisher/ARMSCII-8.TXT` & `monobit-0.39.3/monobit/charmaps/mleisher/ARMSCII-8.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/mleisher/ARMSCII-8A.TXT` & `monobit-0.39.3/monobit/charmaps/mleisher/ARMSCII-8A.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/mleisher/DECMCS.TXT` & `monobit-0.39.3/monobit/charmaps/mleisher/DECMCS.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/mleisher/GEO-ITA.TXT` & `monobit-0.39.3/monobit/charmaps/mleisher/GEO-ITA.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/mleisher/GEO-PS.TXT` & `monobit-0.39.3/monobit/charmaps/mleisher/GEO-PS.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/mleisher/IRANSYSTEM.TXT` & `monobit-0.39.3/monobit/charmaps/mleisher/IRANSYSTEM.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/mleisher/KOI8RU.TXT` & `monobit-0.39.3/monobit/charmaps/mleisher/KOI8RU.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/mleisher/OSNOVAR.TXT` & `monobit-0.39.3/monobit/charmaps/mleisher/OSNOVAR.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/mleisher/README.md` & `monobit-0.39.3/monobit/charmaps/mleisher/README.md`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/mleisher/TIS620.TXT` & `monobit-0.39.3/monobit/charmaps/mleisher/TIS620.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/moztw/big5_2003-b2u.txt` & `monobit-0.39.3/monobit/charmaps/moztw/big5_2003-b2u.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/moztw/eten.txt` & `monobit-0.39.3/monobit/charmaps/moztw/eten.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/python/TCVN5712-1.TXT` & `monobit-0.39.3/monobit/charmaps/python/TCVN5712-1.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/python/TCVN5712-2.TXT` & `monobit-0.39.3/monobit/charmaps/python/TCVN5712-2.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/python/TCVN5712-3.TXT` & `monobit-0.39.3/monobit/charmaps/python/TCVN5712-3.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/vietstd/unicode.html` & `monobit-0.39.3/monobit/charmaps/vietstd/unicode.html`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/vietstd/viscii1.1.txt` & `monobit-0.39.3/monobit/charmaps/vietstd/viscii1.1.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/wikipedia/abicomp.html` & `monobit-0.39.3/monobit/charmaps/wikipedia/abicomp.html`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/wikipedia/brascii.html` & `monobit-0.39.3/monobit/charmaps/wikipedia/brascii.html`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/wikipedia/cp853.html` & `monobit-0.39.3/monobit/charmaps/wikipedia/cp853.html`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/wikipedia/cwi2.html` & `monobit-0.39.3/monobit/charmaps/wikipedia/cwi2.html`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/wikipedia/dec-special.html` & `monobit-0.39.3/monobit/charmaps/wikipedia/dec-special.html`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/wikipedia/dec-technical.html` & `monobit-0.39.3/monobit/charmaps/wikipedia/dec-technical.html`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/wikipedia/gem.html` & `monobit-0.39.3/monobit/charmaps/wikipedia/gem.html`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/wikipedia/kamenicky.html` & `monobit-0.39.3/monobit/charmaps/wikipedia/kamenicky.html`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/wikipedia/lics.html` & `monobit-0.39.3/monobit/charmaps/wikipedia/lics.html`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/wikipedia/mattel-aquarius.html` & `monobit-0.39.3/monobit/charmaps/wikipedia/mattel-aquarius.html`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/wikipedia/mazovia.html` & `monobit-0.39.3/monobit/charmaps/wikipedia/mazovia.html`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/wikipedia/pascii.html` & `monobit-0.39.3/monobit/charmaps/wikipedia/pascii.html`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/wikipedia/ventura.html` & `monobit-0.39.3/monobit/charmaps/wikipedia/ventura.html`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/wikipedia/windows-1252.html` & `monobit-0.39.3/monobit/charmaps/wikipedia/windows-1252.html`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/wikipedia/wingdings.html` & `monobit-0.39.3/monobit/charmaps/wikipedia/wingdings.html`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/wikipedia/wiscii.html` & `monobit-0.39.3/monobit/charmaps/wikipedia/wiscii.html`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/xfonts/mulearabic-1.enc` & `monobit-0.39.3/monobit/charmaps/xfonts/mulearabic-1.enc`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/xfonts/mulearabic-2.enc` & `monobit-0.39.3/monobit/charmaps/xfonts/mulearabic-2.enc`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/xfonts/mulelao-1.enc` & `monobit-0.39.3/monobit/charmaps/xfonts/mulelao-1.enc`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/xfonts/suneu-greek.enc` & `monobit-0.39.3/monobit/charmaps/xfonts/suneu-greek.enc`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/charmaps/xfonts/viscii1.1-1.enc` & `monobit-0.39.3/monobit/charmaps/xfonts/viscii1.1-1.enc`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/containers/compressors.py` & `monobit-0.39.3/monobit/containers/compressors.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/containers/container.py` & `monobit-0.39.3/monobit/containers/container.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/containers/directory.py` & `monobit-0.39.3/monobit/containers/directory.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/containers/mac.py` & `monobit-0.39.3/monobit/containers/mac.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/containers/source.py` & `monobit-0.39.3/monobit/containers/source.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/containers/tar.py` & `monobit-0.39.3/monobit/containers/tar.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/containers/zip.py` & `monobit-0.39.3/monobit/containers/zip.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/formats/amiga.py` & `monobit-0.39.3/monobit/formats/amiga.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/formats/bbc.py` & `monobit-0.39.3/monobit/formats/bbc.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/formats/bdf.py` & `monobit-0.39.3/monobit/formats/bdf.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/formats/bmfont.py` & `monobit-0.39.3/monobit/formats/bmfont.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/formats/borland.py` & `monobit-0.39.3/monobit/formats/borland.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/formats/cpi.py` & `monobit-0.39.3/monobit/formats/cpi.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/formats/daisydot.py` & `monobit-0.39.3/monobit/formats/daisydot.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/formats/dashen.py` & `monobit-0.39.3/monobit/formats/dashen.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/formats/dec.py` & `monobit-0.39.3/monobit/formats/dec.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/formats/dosstart.py` & `monobit-0.39.3/monobit/formats/dosstart.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/formats/figlet.py` & `monobit-0.39.3/monobit/formats/figlet.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/formats/fontx.py` & `monobit-0.39.3/monobit/formats/fontx.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/formats/fzx.py` & `monobit-0.39.3/monobit/formats/fzx.py`

 * *Files 2% similar despite different names*

```diff
@@ -269,27 +269,30 @@
             left=max(0, _glyph.left_bearing),
             top=max(0, font.line_height-_glyph.shift_up-_glyph.height-15),
             adjust_metrics=True
         )
         for _glyph in glyphs
     )
     common_right_bearing = min(_glyph.right_bearing for _glyph in glyphs)
+    # absorb per-glyph right_bearing by extending width
+    glyphs = (
+        _g.expand(right=_g.right_bearing - common_right_bearing)
+        for _g in glyphs
+    )
+    # make zero-width glyphs into 1-width glyphs with 1 step back
+    # as we can't store zero width
+    glyphs = (_g.expand(left=1) if _g.width == 0 else _g for _g in glyphs)
     # set glyph FZX properties
     fzx_glyphs = tuple(
-        # make zero-width glyphs into 1-width glyphs with 1 step back
-        # as we can't store zero width
-        Glyph(fzx_kern=1, fzx_shift=font.line_height, fzx_width=0)
-        if not _glyph.width else
         _glyph.modify(
             fzx_kern=-_glyph.left_bearing,
             # line height includes leading
             fzx_shift=font.line_height-_glyph.shift_up-_glyph.height,
-            # absorb per-glyph right_bearing by extending fzx width
-            fzx_width=_glyph.width + _glyph.right_bearing - common_right_bearing - 1,
-        ).drop('left-bearing', 'right-bearing', 'shift-up')
+            fzx_width=_glyph.width-1,
+        ).drop('left-bearing', 'shift-up')
         for _glyph in glyphs
     )
     # check glyph dimensions / bitfield ranges
     if any(_glyph.fzx_width < 0 or _glyph.fzx_width > 15 for _glyph in fzx_glyphs):
         raise FileFormatError('FZX format: glyphs must be from 1 to 16 pixels wide.')
     if any(_glyph.fzx_kern < 0 or _glyph.fzx_kern > 3 for _glyph in fzx_glyphs):
         raise FileFormatError('FZX format: left-bearing must be in range -3--0.')
@@ -300,10 +303,10 @@
         )
     if common_right_bearing < -128 or common_right_bearing > 127:
         raise FileFormatError('FZX format: right-bearing must be in range -128--127.')
     # set font FZX properties
     fzx_props = Props(
         tracking=common_right_bearing,
         height=font.line_height,
-        lastchar=len(glyphs) + min(_FZX_RANGE) - 1
+        lastchar=len(fzx_glyphs) + min(_FZX_RANGE) - 1
     )
     return fzx_props, fzx_glyphs
```

### Comparing `monobit-0.39.2/monobit/formats/gdos.py` & `monobit-0.39.3/monobit/formats/gdos.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/formats/geos.py` & `monobit-0.39.3/monobit/formats/geos.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/formats/hbf.py` & `monobit-0.39.3/monobit/formats/hbf.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/formats/hex.py` & `monobit-0.39.3/monobit/formats/hex.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/formats/hexdraw.py` & `monobit-0.39.3/monobit/formats/hexdraw.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/formats/hurt.py` & `monobit-0.39.3/monobit/formats/hurt.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/formats/image.py` & `monobit-0.39.3/monobit/formats/image.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/formats/mousegraphics.py` & `monobit-0.39.3/monobit/formats/mousegraphics.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/formats/mzfon.py` & `monobit-0.39.3/monobit/formats/mzfon.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/formats/nearlyraw.py` & `monobit-0.39.3/monobit/formats/nearlyraw.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/formats/palm.py` & `monobit-0.39.3/monobit/formats/palm.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/formats/pcl.py` & `monobit-0.39.3/monobit/formats/pcl.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/formats/pcpaint.py` & `monobit-0.39.3/monobit/formats/pcpaint.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/formats/pdf.py` & `monobit-0.39.3/monobit/formats/pdf.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/formats/pkfont.py` & `monobit-0.39.3/monobit/formats/pkfont.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/formats/printshop.py` & `monobit-0.39.3/monobit/formats/printshop.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/formats/psf.py` & `monobit-0.39.3/monobit/formats/psf.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/formats/raw.py` & `monobit-0.39.3/monobit/formats/raw.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/formats/sfnt.py` & `monobit-0.39.3/monobit/formats/sfnt.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/formats/signum.py` & `monobit-0.39.3/monobit/formats/signum.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/formats/svg.py` & `monobit-0.39.3/monobit/formats/svg.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/formats/vfont.py` & `monobit-0.39.3/monobit/formats/vfont.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/formats/yaff.py` & `monobit-0.39.3/monobit/formats/yaff.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,17 @@
 
 from ..storage import loaders, savers
 from ..encoding import charmaps
 from ..magic import FileFormatError
 from ..font import Font
 from ..glyph import Glyph
 from ..raster import Raster
-from ..labels import strip_matching
+from ..labels import Label, strip_matching
 from ..properties import normalise_property
+from ..basetypes import passthrough
 
 
 ##############################################################################
 # interface
 
 
 @loaders.register(
@@ -373,32 +374,38 @@
         outstream.write('\n')
     outstream.write('\n')
 
 def _write_property(outstream, key, value, comments, indent=''):
     """Write out a property."""
     if value is None:
         return
-    # this may use custom string converter (e.g codepoint labels)
-    value = str(value)
     # write property comment
     if comments:
         outstream.write(
             f'\n{indent}{format_comment(comments, YaffParams.comment)}\n'
         )
     if not key.startswith('_'):
         key = key.replace('_', '-')
     # write key-value pair
+    if isinstance(value, Label) or not isinstance(value, str):
+        # do not quote converted non-strings (plus Tag and Char which are str)
+        # FIXME: reader will strip quotes and misinterpret some labels
+        # so non-ascii or single-char tags will be converted to Char not Tag
+        # common cases (.notdef, missing, default, uniFFFD) will be OK
+        quoter = passthrough
+    else:
+        quoter = _quote_if_needed
+    value = str(value)
     if '\n' not in value:
-        outstream.write(f'{indent}{key}: {_quote_if_needed(value)}\n')
+        outstream.write(f'{indent}{key}: {quoter(value)}\n')
     else:
         outstream.write(
             f'{indent}{key}:\n{indent}{YaffParams.tab}' + '{}\n'.format(
                 f'\n{indent}{YaffParams.tab}'.join(
-                    _quote_if_needed(_line)
-                    for _line in value.splitlines()
+                    quoter(_line) for _line in value.splitlines()
                 )
             )
         )
 
 def _quote_if_needed(value):
     """See if string value needs double quotes."""
     value = str(value)
```

### Comparing `monobit-0.39.2/monobit/formats/mac/__init__.py` & `monobit-0.39.3/monobit/formats/mac/__init__.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/formats/mac/dfont.py` & `monobit-0.39.3/monobit/formats/mac/dfont.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/formats/mac/fond.py` & `monobit-0.39.3/monobit/formats/mac/fond.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/formats/mac/iigs.py` & `monobit-0.39.3/monobit/formats/mac/iigs.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/formats/mac/lisa.py` & `monobit-0.39.3/monobit/formats/mac/lisa.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/formats/mac/nfnt.py` & `monobit-0.39.3/monobit/formats/mac/nfnt.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/formats/os2/__init__.py` & `monobit-0.39.3/monobit/formats/os2/__init__.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/formats/os2/gpifont.py` & `monobit-0.39.3/monobit/formats/os2/gpifont.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/formats/os2/lx.py` & `monobit-0.39.3/monobit/formats/os2/lx.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/formats/os2/ne.py` & `monobit-0.39.3/monobit/formats/os2/ne.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/formats/windows/LICENSE.md` & `monobit-0.39.3/monobit/formats/windows/LICENSE.md`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/formats/windows/__init__.py` & `monobit-0.39.3/monobit/formats/windows/__init__.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/formats/windows/fnt.py` & `monobit-0.39.3/monobit/formats/windows/fnt.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/formats/windows/mz.py` & `monobit-0.39.3/monobit/formats/windows/mz.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/formats/windows/ne.py` & `monobit-0.39.3/monobit/formats/windows/ne.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/formats/windows/pe.py` & `monobit-0.39.3/monobit/formats/windows/pe.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/scripts/banner.py` & `monobit-0.39.3/monobit/scripts/banner.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/monobit/scripts/convert.py` & `monobit-0.39.3/monobit/scripts/convert.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/LICENSE` & `monobit-0.39.3/LICENSE`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/README.md` & `monobit-0.39.3/README.md`

 * *Files identical despite different names*

### Comparing `monobit-0.39.2/pyproject.toml` & `monobit-0.39.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [project]
 name = "monobit"
-version = "0.39.2"
+version = "0.39.3"
 authors = [
     { name = "Rob Hagemans", email = "rob.hagemans@hotmail.com" },
 ]
 description = "Tools for working with monochrome bitmap fonts."
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.9"
```

### Comparing `monobit-0.39.2/PKG-INFO` & `monobit-0.39.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monobit
-Version: 0.39.2
+Version: 0.39.3
 Summary: Tools for working with monochrome bitmap fonts.
 Project-URL: Homepage, https://github.com/robhagemans/monobit
 Author-email: Rob Hagemans <rob.hagemans@hotmail.com>
 License: MIT License
         
         Copyright (c) 2019--2023 Rob Hagemans
```

