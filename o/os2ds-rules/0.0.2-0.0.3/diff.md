# Comparing `tmp/os2ds-rules-0.0.2.tar.gz` & `tmp/os2ds-rules-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "os2ds-rules-0.0.2.tar", last modified: Thu Apr 13 11:13:23 2023, max compression
+gzip compressed data, was "os2ds-rules-0.0.3.tar", last modified: Sat Apr 15 10:09:14 2023, max compression
```

## Comparing `os2ds-rules-0.0.2.tar` & `os2ds-rules-0.0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:13:23.030611 os2ds-rules-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-04-13 11:13:15.000000 os2ds-rules-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-13 11:13:15.000000 os2ds-rules-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    25239 2023-04-13 11:13:23.030611 os2ds-rules-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5056 2023-04-13 11:13:15.000000 os2ds-rules-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:13:23.030611 os2ds-rules-0.0.2/include/
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-04-13 11:13:15.000000 os2ds-rules-0.0.2/include/cpr-detector.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:13:23.030611 os2ds-rules-0.0.2/lib/
--rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-04-13 11:13:15.000000 os2ds-rules-0.0.2/lib/address_rule.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7897 2023-04-13 11:13:15.000000 os2ds-rules-0.0.2/lib/cpr-detector.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-04-13 11:13:15.000000 os2ds-rules-0.0.2/lib/name_rule.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-13 11:13:15.000000 os2ds-rules-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 11:13:23.030611 os2ds-rules-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-04-13 11:13:15.000000 os2ds-rules-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:13:23.030611 os2ds-rules-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:13:23.030611 os2ds-rules-0.0.2/src/os2ds_rules/
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-04-13 11:13:15.000000 os2ds-rules-0.0.2/src/os2ds_rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-04-13 11:13:15.000000 os2ds-rules-0.0.2/src/os2ds_rules/address_rule.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-04-13 11:13:15.000000 os2ds-rules-0.0.2/src/os2ds_rules/cpr.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-04-13 11:13:15.000000 os2ds-rules-0.0.2/src/os2ds_rules/name_rule.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:13:23.030611 os2ds-rules-0.0.2/src/os2ds_rules.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25239 2023-04-13 11:13:23.000000 os2ds-rules-0.0.2/src/os2ds_rules.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-04-13 11:13:23.000000 os2ds-rules-0.0.2/src/os2ds_rules.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 11:13:23.000000 os2ds-rules-0.0.2/src/os2ds_rules.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-13 11:13:23.000000 os2ds-rules-0.0.2/src/os2ds_rules.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:09:14.493536 os2ds-rules-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-04-15 10:09:02.000000 os2ds-rules-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-15 10:09:02.000000 os2ds-rules-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    25239 2023-04-15 10:09:14.493536 os2ds-rules-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5056 2023-04-15 10:09:02.000000 os2ds-rules-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:09:14.489535 os2ds-rules-0.0.3/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-04-15 10:09:02.000000 os2ds-rules-0.0.3/include/cpr-detector.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:09:14.493536 os2ds-rules-0.0.3/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-04-15 10:09:02.000000 os2ds-rules-0.0.3/lib/address_rule.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8928 2023-04-15 10:09:02.000000 os2ds-rules-0.0.3/lib/cpr-detector.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-04-15 10:09:02.000000 os2ds-rules-0.0.3/lib/name_rule.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-15 10:09:02.000000 os2ds-rules-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 10:09:14.493536 os2ds-rules-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-04-15 10:09:02.000000 os2ds-rules-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:09:14.489535 os2ds-rules-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:09:14.493536 os2ds-rules-0.0.3/src/os2ds_rules/
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-04-15 10:09:02.000000 os2ds-rules-0.0.3/src/os2ds_rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-04-15 10:09:02.000000 os2ds-rules-0.0.3/src/os2ds_rules/address_rule.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-04-15 10:09:02.000000 os2ds-rules-0.0.3/src/os2ds_rules/cpr.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-04-15 10:09:02.000000 os2ds-rules-0.0.3/src/os2ds_rules/name_rule.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:09:14.493536 os2ds-rules-0.0.3/src/os2ds_rules.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    25239 2023-04-15 10:09:14.000000 os2ds-rules-0.0.3/src/os2ds_rules.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-04-15 10:09:14.000000 os2ds-rules-0.0.3/src/os2ds_rules.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 10:09:14.000000 os2ds-rules-0.0.3/src/os2ds_rules.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-15 10:09:14.000000 os2ds-rules-0.0.3/src/os2ds_rules.egg-info/top_level.txt
```

### Comparing `os2ds-rules-0.0.2/LICENSE` & `os2ds-rules-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `os2ds-rules-0.0.2/PKG-INFO` & `os2ds-rules-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: os2ds-rules
-Version: 0.0.2
+Version: 0.0.3
 Summary: Text processing tool for detecting Danish CPR-numbers.
 Author-email: HackTheOxidation <tomas.hagenau@protonmail.ch>
 License: Mozilla Public License Version 2.0
         ==================================
         
         1. Definitions
         --------------
```

### Comparing `os2ds-rules-0.0.2/README.md` & `os2ds-rules-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `os2ds-rules-0.0.2/include/cpr-detector.hpp` & `os2ds-rules-0.0.3/include/cpr-detector.hpp`

 * *Files 7% similar despite different names*

```diff
@@ -65,14 +65,15 @@
   void reset(CPRDetectorState &state) noexcept;
   char update(char, CPRDetectorState, CPRDetectorState &, Predicate) noexcept;
   bool check_day_month(const std::string &, CPRDetectorState &) noexcept;
   void check_leap_year(const std::string &, CPRDetectorState &) noexcept;
   void check_and_append_cpr(std::string &, MatchResults &, size_t,
                             size_t) noexcept;
   bool check_mod11(const MatchResult &) noexcept;
+  bool examine_context(const std::string &) noexcept;
 
 public:
   constexpr CPRDetector(bool check_mod11 = false,
                         bool examine_context = false) noexcept
       : check_mod11_(check_mod11), examine_context_(examine_context) {}
 
   constexpr CPRDetector(const CPRDetector &) noexcept = default;
```

### Comparing `os2ds-rules-0.0.2/lib/address_rule.cpp` & `os2ds-rules-0.0.3/lib/address_rule.cpp`

 * *Files identical despite different names*

### Comparing `os2ds-rules-0.0.2/lib/cpr-detector.cpp` & `os2ds-rules-0.0.3/lib/cpr-detector.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -20,14 +20,34 @@
      "bilagsnummer", "order number", "ordrenummer", "fakturanummer", "faknr",
      "fak-nr", "tullstatistisk", "tullstatistik", "test report no",
      "protocol no.", "dhk:tx"});
 
 static const auto blacklist_words_set = FrozenHashSet(blacklist_words);
 }; // namespace
 
+static bool find_blacklisted_words(const std::string &content, const std::array<std::size_t, 4> indices) noexcept {
+
+  for (std::size_t i = 1; i < 4; ++i) {
+    for (std::size_t j = 0; j < i; ++j) {
+      auto begin = indices[j];
+      auto end = indices[i] - begin;
+
+      if (end > content.size())
+	end = content.size() - begin - 1;
+
+      std::string target = content.substr(begin, end);
+
+      if (blacklist_words_set.contains(target))
+	return true;
+    }
+  }
+
+  return false;
+}
+
 void CPRDetector::reset(CPRDetectorState &state) noexcept {
   // Set the detector state to Empty.
   state = CPRDetectorState::Empty;
 }
 
 char CPRDetector::update(char c, CPRDetectorState new_state,
                          CPRDetectorState &old_state,
@@ -110,22 +130,46 @@
   // Take the sum of all factors.
   auto sum = std::accumulate(std::begin(factors), std::end(factors), 0);
 
   // Check that the sum is ok.
   return sum % 11 == 0;
 }
 
+bool CPRDetector::examine_context(const std::string &content) noexcept {
+  std::size_t spaces = 3;
+  std::array<std::size_t, 4> indices = {0, 0, 0, 0};
+
+  for (std::size_t i = 0; i < content.size(); ++i) {
+    if (content[i] == ' ') {
+      indices[4 - spaces] = i;
+      --spaces;
+      if (spaces == 0) {
+	if (find_blacklisted_words(content, indices))
+	  return true;
+	
+	spaces = 3;
+	indices[0] = indices[3] + 1;
+      }
+    }
+  }
+
+  if (find_blacklisted_words(content, indices))
+    return true;
+
+  return false;
+}
+
 MatchResults CPRDetector::find_matches(const std::string &content) noexcept {
   MatchResults results;
 
   if (content.size() < 10) {
     return results;
   }
 
-  if (examine_context_) {
+  if (examine_context_ && examine_context(content)) {
     return results;
   }
 
   // Initialize.
   CPRDetectorState state = CPRDetectorState::Empty;
   std::string cpr(10, 0);
   char previous = 0;
```

### Comparing `os2ds-rules-0.0.2/lib/name_rule.cpp` & `os2ds-rules-0.0.3/lib/name_rule.cpp`

 * *Files identical despite different names*

### Comparing `os2ds-rules-0.0.2/pyproject.toml` & `os2ds-rules-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=62"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "os2ds-rules"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="HackTheOxidation", email="tomas.hagenau@protonmail.ch" },
 ]
 description = "Text processing tool for detecting Danish CPR-numbers."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.9"
@@ -22,8 +22,8 @@
 
 [tool.cibuildwheel]
 skip = ["*win32*", "*macos*", "*i686", "*aarch64", "*ppc64le", "*s390x", "*universal2", "*musl*"]
 
 archs = ["auto64"]
 build-frontend = "pip"
 
-manylinux-x86_64-image = "manylinux_2_28"
+manylinux-x86_64-image = "manylinux_2_28"
```

### Comparing `os2ds-rules-0.0.2/setup.py` & `os2ds-rules-0.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `os2ds-rules-0.0.2/src/os2ds_rules/__init__.py` & `os2ds-rules-0.0.3/src/os2ds_rules/__init__.py`

 * *Files identical despite different names*

### Comparing `os2ds-rules-0.0.2/src/os2ds_rules/address_rule.cpp` & `os2ds-rules-0.0.3/src/os2ds_rules/address_rule.cpp`

 * *Files identical despite different names*

### Comparing `os2ds-rules-0.0.2/src/os2ds_rules/cpr.cpp` & `os2ds-rules-0.0.3/src/os2ds_rules/cpr.cpp`

 * *Files identical despite different names*

### Comparing `os2ds-rules-0.0.2/src/os2ds_rules/name_rule.cpp` & `os2ds-rules-0.0.3/src/os2ds_rules/name_rule.cpp`

 * *Files identical despite different names*

### Comparing `os2ds-rules-0.0.2/src/os2ds_rules.egg-info/PKG-INFO` & `os2ds-rules-0.0.3/src/os2ds_rules.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: os2ds-rules
-Version: 0.0.2
+Version: 0.0.3
 Summary: Text processing tool for detecting Danish CPR-numbers.
 Author-email: HackTheOxidation <tomas.hagenau@protonmail.ch>
 License: Mozilla Public License Version 2.0
         ==================================
         
         1. Definitions
         --------------
```

