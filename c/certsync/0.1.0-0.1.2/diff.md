# Comparing `tmp/certsync-0.1.0.tar.gz` & `tmp/certsync-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "certsync-0.1.0.tar", last modified: Fri Feb  3 13:28:45 2023, max compression
+gzip compressed data, was "certsync-0.1.2.tar", max compression
```

## Comparing `certsync-0.1.0.tar` & `certsync-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,6 @@
-drwxrwxr-x   0 tse       (1000) tse       (1000)        0 2023-02-03 13:28:45.192734 certsync-0.1.0/
--rw-rw-r--   0 tse       (1000) tse       (1000)     1066 2023-02-03 08:27:33.000000 certsync-0.1.0/LICENSE
--rw-rw-r--   0 tse       (1000) tse       (1000)      342 2023-02-03 13:28:45.192734 certsync-0.1.0/PKG-INFO
--rw-rw-r--   0 tse       (1000) tse       (1000)     6622 2023-02-03 09:03:02.000000 certsync-0.1.0/README.md
-drwxrwxr-x   0 tse       (1000) tse       (1000)        0 2023-02-03 13:28:45.188734 certsync-0.1.0/certsync/
--rw-rw-r--   0 tse       (1000) tse       (1000)        0 2023-02-03 08:27:33.000000 certsync-0.1.0/certsync/__init__.py
--rw-rw-r--   0 tse       (1000) tse       (1000)    20330 2023-02-03 13:16:34.000000 certsync-0.1.0/certsync/entry.py
-drwxrwxr-x   0 tse       (1000) tse       (1000)        0 2023-02-03 13:28:45.192734 certsync-0.1.0/certsync.egg-info/
--rw-rw-r--   0 tse       (1000) tse       (1000)      342 2023-02-03 13:28:45.000000 certsync-0.1.0/certsync.egg-info/PKG-INFO
--rw-rw-r--   0 tse       (1000) tse       (1000)      259 2023-02-03 13:28:45.000000 certsync-0.1.0/certsync.egg-info/SOURCES.txt
--rw-rw-r--   0 tse       (1000) tse       (1000)        1 2023-02-03 13:28:45.000000 certsync-0.1.0/certsync.egg-info/dependency_links.txt
--rw-rw-r--   0 tse       (1000) tse       (1000)       50 2023-02-03 13:28:45.000000 certsync-0.1.0/certsync.egg-info/entry_points.txt
--rw-rw-r--   0 tse       (1000) tse       (1000)       23 2023-02-03 13:28:45.000000 certsync-0.1.0/certsync.egg-info/requires.txt
--rw-rw-r--   0 tse       (1000) tse       (1000)        9 2023-02-03 13:28:45.000000 certsync-0.1.0/certsync.egg-info/top_level.txt
--rw-rw-r--   0 tse       (1000) tse       (1000)       38 2023-02-03 13:28:45.192734 certsync-0.1.0/setup.cfg
--rw-rw-r--   0 tse       (1000) tse       (1000)      598 2023-02-03 13:19:07.000000 certsync-0.1.0/setup.py
+-rw-r--r--   0        0        0     1066 2023-04-15 14:59:30.740372 certsync-0.1.2/LICENSE
+-rw-r--r--   0        0        0     6623 2023-04-15 14:59:30.740372 certsync-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-04-15 14:59:30.740372 certsync-0.1.2/certsync/__init__.py
+-rw-r--r--   0        0        0    20331 2023-04-15 14:59:30.740372 certsync-0.1.2/certsync/entry.py
+-rw-r--r--   0        0        0      790 2023-04-15 14:59:30.740372 certsync-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     7568 1970-01-01 00:00:00.000000 certsync-0.1.2/PKG-INFO
```

### Comparing `certsync-0.1.0/LICENSE` & `certsync-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `certsync-0.1.0/README.md` & `certsync-0.1.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # certsync
 
-`certsync` is a new technique in order to dump NTDS remotely, but this time **without DSRUAPI**: it uses [golden certificate](https://cyberstoph.org/posts/2019/12/an-introduction-to-golden-certificates/) and [UnPAC the hash](https://www.thehacker.recipes/ad/movement/kerberos/unpac-the-hash).
+`certsync` is a new technique in order to dump NTDS remotely, but this time **without DRSUAPI**: it uses [golden certificate](https://cyberstoph.org/posts/2019/12/an-introduction-to-golden-certificates/) and [UnPAC the hash](https://www.thehacker.recipes/ad/movement/kerberos/unpac-the-hash).
 It works in several steps:
 
 1. Dump user list, CA informations and CRL from LDAP
 2. Dump CA certificate and private key
 3. Forge offline a certificate for every user
 4. UnPAC the hash for every user in order to get nt and lm hashes
 
@@ -132,8 +132,8 @@
 - `-randomize`: By default, every forged user certificates will have the same private key, serial number and validity dates. This parameter will randomize them, but the forging will take longer. 
 
 ## Credits
 
 - [Olivier Lyak](https://twitter.com/ly4k_) for all his work on ADCS and [certipy](https://github.com/ly4k/Certipy).
 - [Benjamin Delpy](https://twitter.com/gentilkiwi) for the unPAC the hash technique.
 - [Will Schroeder](https://twitter.com/harmj0y) and [Lee Christensen](https://twitter.com/tifkin_) for [Certified Pre-Owned](https://www.specterops.io/assets/resources/Certified_Pre-Owned.pdf) and [Certify](https://github.com/GhostPack/Certify).
-- [Mayfly](https://twitter.com/M4yFly) for his great lab: [GOAD](https://github.com/Orange-Cyberdefense/GOAD).
+- [Mayfly](https://twitter.com/M4yFly) for his great lab: [GOAD](https://github.com/Orange-Cyberdefense/GOAD).
```

### Comparing `certsync-0.1.0/certsync/entry.py` & `certsync-0.1.2/certsync/entry.py`

 * *Files 0% similar despite different names*

```diff
@@ -205,15 +205,15 @@
             logging.info("Dumping CA certificate and private key")
             ca_target = Target.create(
                 domain = self.target.domain,
                 username = self.target.username,
                 password = self.target.password,
                 dc_ip = self.target.dc_ip,
                 do_kerberos = self.target.do_kerberos,
-                hashes = self.target.hashes,
+                hashes = self.options.hashes,
                 aes = self.target.aes,
                 remote_name = self.ca_ip_address)
 
             ca_module = CA(target=ca_target, ca=self.ca_name)
             self.backup_ca_pki(ca_module)
         else:
             logging.info("Loading CA certificate and private key from %s" % self.options.ca_pfx)
```

