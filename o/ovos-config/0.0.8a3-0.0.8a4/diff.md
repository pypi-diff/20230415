# Comparing `tmp/ovos_config-0.0.8a3-py3-none-any.whl.zip` & `tmp/ovos_config-0.0.8a4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
 Zip file size: 26211 bytes, number of entries: 16
--rw-r--r--  2.0 unx      430 b- defN 23-Apr-05 19:57 ovos_config/__init__.py
--rw-r--r--  2.0 unx    11830 b- defN 23-Apr-05 19:57 ovos_config/__main__.py
--rw-r--r--  2.0 unx    14538 b- defN 23-Apr-05 19:57 ovos_config/config.py
--rw-r--r--  2.0 unx     2694 b- defN 23-Apr-05 19:57 ovos_config/locale.py
--rw-r--r--  2.0 unx     5734 b- defN 23-Apr-05 19:57 ovos_config/locations.py
--rw-r--r--  2.0 unx     7102 b- defN 23-Apr-05 19:57 ovos_config/meta.py
--rw-r--r--  2.0 unx     6423 b- defN 23-Apr-05 19:57 ovos_config/models.py
--rw-r--r--  2.0 unx    24137 b- defN 23-Apr-05 19:57 ovos_config/mycroft.conf
--rw-r--r--  2.0 unx      151 b- defN 23-Apr-05 19:57 ovos_config/ovos.py
--rw-r--r--  2.0 unx       82 b- defN 23-Apr-05 19:57 ovos_config/utils.py
--rw-r--r--  2.0 unx      114 b- defN 23-Apr-05 19:57 ovos_config/version.py
--rw-r--r--  2.0 unx      484 b- defN 23-Apr-05 19:57 ovos_config-0.0.8a3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-05 19:57 ovos_config-0.0.8a3.dist-info/WHEEL
--rw-r--r--  2.0 unx       61 b- defN 23-Apr-05 19:57 ovos_config-0.0.8a3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       12 b- defN 23-Apr-05 19:57 ovos_config-0.0.8a3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1284 b- defN 23-Apr-05 19:57 ovos_config-0.0.8a3.dist-info/RECORD
-16 files, 75168 bytes uncompressed, 24103 bytes compressed:  67.9%
+-rw-r--r--  2.0 unx      430 b- defN 23-Apr-14 22:02 ovos_config/__init__.py
+-rw-r--r--  2.0 unx    11830 b- defN 23-Apr-14 22:02 ovos_config/__main__.py
+-rw-r--r--  2.0 unx    14538 b- defN 23-Apr-14 22:02 ovos_config/config.py
+-rw-r--r--  2.0 unx     2694 b- defN 23-Apr-14 22:02 ovos_config/locale.py
+-rw-r--r--  2.0 unx     5734 b- defN 23-Apr-14 22:02 ovos_config/locations.py
+-rw-r--r--  2.0 unx     7102 b- defN 23-Apr-14 22:02 ovos_config/meta.py
+-rw-r--r--  2.0 unx     6423 b- defN 23-Apr-14 22:02 ovos_config/models.py
+-rw-r--r--  2.0 unx    24138 b- defN 23-Apr-14 22:02 ovos_config/mycroft.conf
+-rw-r--r--  2.0 unx      151 b- defN 23-Apr-14 22:02 ovos_config/ovos.py
+-rw-r--r--  2.0 unx       82 b- defN 23-Apr-14 22:02 ovos_config/utils.py
+-rw-r--r--  2.0 unx      114 b- defN 23-Apr-14 22:02 ovos_config/version.py
+-rw-r--r--  2.0 unx      484 b- defN 23-Apr-14 22:03 ovos_config-0.0.8a4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-14 22:03 ovos_config-0.0.8a4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       61 b- defN 23-Apr-14 22:03 ovos_config-0.0.8a4.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       12 b- defN 23-Apr-14 22:03 ovos_config-0.0.8a4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1284 b- defN 23-Apr-14 22:03 ovos_config-0.0.8a4.dist-info/RECORD
+16 files, 75169 bytes uncompressed, 24103 bytes compressed:  67.9%
```

## zipnote {}

```diff
@@ -27,23 +27,23 @@
 
 Filename: ovos_config/utils.py
 Comment: 
 
 Filename: ovos_config/version.py
 Comment: 
 
-Filename: ovos_config-0.0.8a3.dist-info/METADATA
+Filename: ovos_config-0.0.8a4.dist-info/METADATA
 Comment: 
 
-Filename: ovos_config-0.0.8a3.dist-info/WHEEL
+Filename: ovos_config-0.0.8a4.dist-info/WHEEL
 Comment: 
 
-Filename: ovos_config-0.0.8a3.dist-info/entry_points.txt
+Filename: ovos_config-0.0.8a4.dist-info/entry_points.txt
 Comment: 
 
-Filename: ovos_config-0.0.8a3.dist-info/top_level.txt
+Filename: ovos_config-0.0.8a4.dist-info/top_level.txt
 Comment: 
 
-Filename: ovos_config-0.0.8a3.dist-info/RECORD
+Filename: ovos_config-0.0.8a4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ovos_config/mycroft.conf

```diff
@@ -18,15 +18,15 @@
   // individual systems can still apply changes at the SYSTEM or USER levels.
 
   // Language used for speech-to-text and text-to-speech.
   // Code is a BCP-47 identifier (https://tools.ietf.org/html/bcp47), lowercased
   // TODO: save unmodified, lowercase upon demand
   "lang": "en-us",
 
-  // Measurement units, either 'metric' or 'english'
+  // Measurement units, either 'metric' or 'imperial'
   // Override: REMOTE
   "system_unit": "metric",
 
   // Time format, either 'half' (e.g. "11:37 pm") or 'full' (e.g. "23:37")
   // Override: REMOTE
   "time_format": "half",
```

## ovos_config/version.py

```diff
@@ -1,6 +1,6 @@
 # START_VERSION_BLOCK
 VERSION_MAJOR = 0
 VERSION_MINOR = 0
 VERSION_BUILD = 8
-VERSION_ALPHA = 3
+VERSION_ALPHA = 4
 # END_VERSION_BLOCK
```

## Comparing `ovos_config-0.0.8a3.dist-info/RECORD` & `ovos_config-0.0.8a4.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 ovos_config/__init__.py,sha256=g2dV7vVqF1VxpY5DUzBShJJK5Um5qgQ3x-73DYZP6C4,430
 ovos_config/__main__.py,sha256=g7Sjvrqg4iiFDa9CbooGfRDd07Uzd4qKJL0XZtkeX4Y,11830
 ovos_config/config.py,sha256=uOtz6pBSNuX11QRH0IE37PH90qUWGojvKBIjJlqCKks,14538
 ovos_config/locale.py,sha256=1D6-pK6uoMf224Wcf7MxdUXYkN6oAowvykCN8p1dp0M,2694
 ovos_config/locations.py,sha256=BaCQEj5d7cwDc84ZifEnIXWLBLdkpOn0Remy7Wf3wTY,5734
 ovos_config/meta.py,sha256=nzzkt-so18IWbYjIu8RP-5o_lce755DIhGAsH6T6zHw,7102
 ovos_config/models.py,sha256=bXk06hnAUmanHNf88jx-M9j6gc3JDSgwNJ4wTe2Q6vA,6423
-ovos_config/mycroft.conf,sha256=1-qXtPLqxhkrvAzgenMAhdYPAMSMY31T_NvigKmQXlE,24137
+ovos_config/mycroft.conf,sha256=bbhikIzU8plecX88yRDLGJDKsgk4fuTxkwePkq5gG-8,24138
 ovos_config/ovos.py,sha256=6g6p7c24s5R5KOi6Nlpz-rAEqWs3k6eJzT_OfkpKEyM,151
 ovos_config/utils.py,sha256=roU_l8QwnMqpkfglvBaH6d-JDSccrQ_C4AqvI16DFv4,82
-ovos_config/version.py,sha256=XjPMD99mqbLwdSWh1oJXd6AtRScf5kBvDbO2ZKHf-v4,114
-ovos_config-0.0.8a3.dist-info/METADATA,sha256=5eNjxBTvoJ2LR4uR84OhAvbgjKtMdy0NxO5BdSFjTBo,484
-ovos_config-0.0.8a3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-ovos_config-0.0.8a3.dist-info/entry_points.txt,sha256=Ik2osmXLMHXaN39r9up9GzkLXSx6nS7eAiB_FI_YW5s,61
-ovos_config-0.0.8a3.dist-info/top_level.txt,sha256=Yl0O4b4iwQpernznu7fSfyjUAGW7V7pNPZQu-Easrko,12
-ovos_config-0.0.8a3.dist-info/RECORD,,
+ovos_config/version.py,sha256=8vcWNeeehecYZfMbwB4RCyRF_YuhWt-34Qa7wm1OVFs,114
+ovos_config-0.0.8a4.dist-info/METADATA,sha256=Fn9cNEeoHXt9Kr9XAFZSVBZUUBtrWnGQrUeZnqEo_m8,484
+ovos_config-0.0.8a4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+ovos_config-0.0.8a4.dist-info/entry_points.txt,sha256=Ik2osmXLMHXaN39r9up9GzkLXSx6nS7eAiB_FI_YW5s,61
+ovos_config-0.0.8a4.dist-info/top_level.txt,sha256=Yl0O4b4iwQpernznu7fSfyjUAGW7V7pNPZQu-Easrko,12
+ovos_config-0.0.8a4.dist-info/RECORD,,
```

