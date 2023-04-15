# Comparing `tmp/phpdiscord-1.0.2.tar.gz` & `tmp/phpdiscord-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phpdiscord-1.0.2.tar", last modified: Sat Apr 15 06:01:11 2023, max compression
+gzip compressed data, was "phpdiscord-1.0.3.tar", last modified: Sat Apr 15 14:09:03 2023, max compression
```

## Comparing `phpdiscord-1.0.2.tar` & `phpdiscord-1.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-15 06:01:11.789251 phpdiscord-1.0.2/
--rw-rw----   0 root         (0) everybody  (9997)     2854 2023-04-15 06:01:11.757251 phpdiscord-1.0.2/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)     2600 2023-04-15 06:00:34.000000 phpdiscord-1.0.2/README.md
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-15 06:01:11.701251 phpdiscord-1.0.2/phpdiscord/
--rw-rw----   0 root         (0) everybody  (9997)     4222 2023-04-15 05:55:00.000000 phpdiscord-1.0.2/phpdiscord/phpdiscord.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-15 06:01:11.749251 phpdiscord-1.0.2/phpdiscord.egg-info/
--rw-rw----   0 root         (0) everybody  (9997)     2854 2023-04-15 06:01:11.000000 phpdiscord-1.0.2/phpdiscord.egg-info/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      179 2023-04-15 06:01:11.000000 phpdiscord-1.0.2/phpdiscord.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-04-15 06:01:11.000000 phpdiscord-1.0.2/phpdiscord.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) everybody  (9997)       11 2023-04-15 06:01:11.000000 phpdiscord-1.0.2/phpdiscord.egg-info/top_level.txt
--rw-rw----   0 root         (0) everybody  (9997)       38 2023-04-15 06:01:11.793251 phpdiscord-1.0.2/setup.cfg
--rw-rw----   0 root         (0) everybody  (9997)      334 2023-04-15 04:57:11.000000 phpdiscord-1.0.2/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-15 14:09:03.085412 phpdiscord-1.0.3/
+-rw-rw----   0 root         (0) everybody  (9997)     2903 2023-04-15 14:09:03.077412 phpdiscord-1.0.3/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)     2649 2023-04-15 14:07:14.000000 phpdiscord-1.0.3/README.md
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-15 14:09:03.021412 phpdiscord-1.0.3/phpdiscord/
+-rw-rw----   0 root         (0) everybody  (9997)     7193 2023-04-15 14:08:25.000000 phpdiscord-1.0.3/phpdiscord/phpdiscord.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-15 14:09:03.069413 phpdiscord-1.0.3/phpdiscord.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)     2903 2023-04-15 14:09:02.000000 phpdiscord-1.0.3/phpdiscord.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      179 2023-04-15 14:09:02.000000 phpdiscord-1.0.3/phpdiscord.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-04-15 14:09:02.000000 phpdiscord-1.0.3/phpdiscord.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)       11 2023-04-15 14:09:02.000000 phpdiscord-1.0.3/phpdiscord.egg-info/top_level.txt
+-rw-rw----   0 root         (0) everybody  (9997)       38 2023-04-15 14:09:03.085412 phpdiscord-1.0.3/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)      334 2023-04-15 14:07:23.000000 phpdiscord-1.0.3/setup.py
```

### Comparing `phpdiscord-1.0.2/PKG-INFO` & `phpdiscord-1.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phpdiscord
-Version: 1.0.2
+Version: 1.0.3
 Summary: phpdiscord its discord py for newbiers!
 Home-page: UNKNOWN
 Author: NouName
 Author-email: duaneskalanak@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -83,14 +83,16 @@
     reason = interaction.options["reason"].value if "reason" in interaction.options else None
     mention = f"<@{user.id}>"
     response = f"{mention} has been kicked"
     if reason:
         response += f" for {reason}"
     interaction.response.send_message(response)
 
-client.run()```
+client.run()
 
 Phpdiscord ussing class Discord for inclusion your bot !
 
 Dont forget <your-
 bot-token> change to your token.
 
+New class Selfbot , his inits Self, Prefix, Token 
+
```

### Comparing `phpdiscord-1.0.2/README.md` & `phpdiscord-1.0.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -72,13 +72,15 @@
     reason = interaction.options["reason"].value if "reason" in interaction.options else None
     mention = f"<@{user.id}>"
     response = f"{mention} has been kicked"
     if reason:
         response += f" for {reason}"
     interaction.response.send_message(response)
 
-client.run()```
+client.run()
 
 Phpdiscord ussing class Discord for inclusion your bot !
 
 Dont forget <your-
-bot-token> change to your token.
+bot-token> change to your token.
+
+New class Selfbot , his inits Self, Prefix, Token
```

### Comparing `phpdiscord-1.0.2/phpdiscord.egg-info/PKG-INFO` & `phpdiscord-1.0.3/phpdiscord.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phpdiscord
-Version: 1.0.2
+Version: 1.0.3
 Summary: phpdiscord its discord py for newbiers!
 Home-page: UNKNOWN
 Author: NouName
 Author-email: duaneskalanak@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -83,14 +83,16 @@
     reason = interaction.options["reason"].value if "reason" in interaction.options else None
     mention = f"<@{user.id}>"
     response = f"{mention} has been kicked"
     if reason:
         response += f" for {reason}"
     interaction.response.send_message(response)
 
-client.run()```
+client.run()
 
 Phpdiscord ussing class Discord for inclusion your bot !
 
 Dont forget <your-
 bot-token> change to your token.
 
+New class Selfbot , his inits Self, Prefix, Token 
+
```

