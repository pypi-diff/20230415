# Comparing `tmp/sentry-auth-ldap-21.9.8.tar.gz` & `tmp/sentry-auth-ldap-21.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentry-auth-ldap-21.9.8.tar", last modified: Thu Mar 16 09:01:39 2023, max compression
+gzip compressed data, was "sentry-auth-ldap-21.9.9.tar", last modified: Thu Mar 16 10:48:40 2023, max compression
```

## Comparing `sentry-auth-ldap-21.9.8.tar` & `sentry-auth-ldap-21.9.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:01:39.669609 sentry-auth-ldap-21.9.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-03-16 09:01:25.000000 sentry-auth-ldap-21.9.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7252 2023-03-16 09:01:39.669609 sentry-auth-ldap-21.9.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6271 2023-03-16 09:01:25.000000 sentry-auth-ldap-21.9.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:01:39.669609 sentry-auth-ldap-21.9.8/sentry_auth_ldap/
--rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-03-16 09:01:25.000000 sentry-auth-ldap-21.9.8/sentry_auth_ldap/backend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:01:39.669609 sentry-auth-ldap-21.9.8/sentry_auth_ldap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7252 2023-03-16 09:01:39.000000 sentry-auth-ldap-21.9.8/sentry_auth_ldap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-03-16 09:01:39.000000 sentry-auth-ldap-21.9.8/sentry_auth_ldap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 09:01:39.000000 sentry-auth-ldap-21.9.8/sentry_auth_ldap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 09:01:39.000000 sentry-auth-ldap-21.9.8/sentry_auth_ldap.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-03-16 09:01:39.000000 sentry-auth-ldap-21.9.8/sentry_auth_ldap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-16 09:01:39.000000 sentry-auth-ldap-21.9.8/sentry_auth_ldap.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-16 09:01:39.669609 sentry-auth-ldap-21.9.8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1604 2023-03-16 09:01:25.000000 sentry-auth-ldap-21.9.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 10:48:40.478174 sentry-auth-ldap-21.9.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-03-16 10:48:27.000000 sentry-auth-ldap-21.9.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7252 2023-03-16 10:48:40.478174 sentry-auth-ldap-21.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6271 2023-03-16 10:48:27.000000 sentry-auth-ldap-21.9.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 10:48:40.474174 sentry-auth-ldap-21.9.9/sentry_auth_ldap/
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-03-16 10:48:27.000000 sentry-auth-ldap-21.9.9/sentry_auth_ldap/backend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 10:48:40.478174 sentry-auth-ldap-21.9.9/sentry_auth_ldap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7252 2023-03-16 10:48:40.000000 sentry-auth-ldap-21.9.9/sentry_auth_ldap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-03-16 10:48:40.000000 sentry-auth-ldap-21.9.9/sentry_auth_ldap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 10:48:40.000000 sentry-auth-ldap-21.9.9/sentry_auth_ldap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 10:48:40.000000 sentry-auth-ldap-21.9.9/sentry_auth_ldap.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-03-16 10:48:40.000000 sentry-auth-ldap-21.9.9/sentry_auth_ldap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-16 10:48:40.000000 sentry-auth-ldap-21.9.9/sentry_auth_ldap.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-16 10:48:40.478174 sentry-auth-ldap-21.9.9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1604 2023-03-16 10:48:27.000000 sentry-auth-ldap-21.9.9/setup.py
```

### Comparing `sentry-auth-ldap-21.9.8/LICENSE.txt` & `sentry-auth-ldap-21.9.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sentry-auth-ldap-21.9.8/PKG-INFO` & `sentry-auth-ldap-21.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentry-auth-ldap
-Version: 21.9.8
+Version: 21.9.9
 Summary: A Sentry extension to add an LDAP server as an authentication source.
 Home-page: https://github.com/PMExtra/sentry-auth-ldap
 Download-URL: https://github.com/PMExtra/sentry-auth-ldap
 Author: Chad Killingsworth <chad.killingsworth@banno.com>, Barron Hagerman <barron.hagerman@banno.com>, PM Extra <pm@jubeat.net>
 Author-email: pm@jubeat.net
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/PMExtra/sentry-auth-ldap/issues
```

### Comparing `sentry-auth-ldap-21.9.8/README.md` & `sentry-auth-ldap-21.9.9/README.md`

 * *Files identical despite different names*

### Comparing `sentry-auth-ldap-21.9.8/sentry_auth_ldap/backend.py` & `sentry-auth-ldap-21.9.9/sentry_auth_ldap/backend.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,34 +4,35 @@
     Organization,
     OrganizationMember,
     UserEmail,
     UserOption,
 )
 
 
-def _get_effective_sentry_role(group_names):
+def _get_effective_sentry_role(ldap_user):
     role_priority_order = [
         'member',
         'admin',
         'manager',
         'owner',
     ]
 
     role_mapping = getattr(settings, 'AUTH_LDAP_SENTRY_GROUP_ROLE_MAPPING', None)
+    if not role_mapping:
+        return None
 
-    if not group_names or not role_mapping:
+    group_names = ldap_user.group_names
+    if not group_names:
         return None
 
     applicable_roles = [role for role, groups in role_mapping.items() if group_names.intersection(groups)]
-
     if not applicable_roles:
         return None
 
     highest_role = [role for role in role_priority_order if role in applicable_roles][-1]
-
     return highest_role
 
 
 class SentryLdapBackend(LDAPBackend):
     def get_or_build_user(self, username, ldap_user):
         (user, built) = super().get_or_build_user(username, ldap_user)
 
@@ -75,17 +76,15 @@
             organizations = Organization.objects.filter(name=organization_name)
         else:
             return (user, built)
 
         if not organizations or len(organizations) < 1:
             return (user, built)
 
-        member_role = _get_effective_sentry_role(ldap_user.group_names)
-        if not member_role:
-            member_role = getattr(settings, 'AUTH_LDAP_SENTRY_ORGANIZATION_ROLE_TYPE', None)
+        member_role = _get_effective_sentry_role(ldap_user) or getattr(settings, 'AUTH_LDAP_SENTRY_ORGANIZATION_ROLE_TYPE', None)
 
         has_global_access = getattr(settings, 'AUTH_LDAP_SENTRY_ORGANIZATION_GLOBAL_ACCESS', False)
 
         # Add the user to the organization with global access
         OrganizationMember.objects.create(
             organization=organizations[0],
             user=user,
```

### Comparing `sentry-auth-ldap-21.9.8/sentry_auth_ldap.egg-info/PKG-INFO` & `sentry-auth-ldap-21.9.9/sentry_auth_ldap.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentry-auth-ldap
-Version: 21.9.8
+Version: 21.9.9
 Summary: A Sentry extension to add an LDAP server as an authentication source.
 Home-page: https://github.com/PMExtra/sentry-auth-ldap
 Download-URL: https://github.com/PMExtra/sentry-auth-ldap
 Author: Chad Killingsworth <chad.killingsworth@banno.com>, Barron Hagerman <barron.hagerman@banno.com>, PM Extra <pm@jubeat.net>
 Author-email: pm@jubeat.net
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/PMExtra/sentry-auth-ldap/issues
```

### Comparing `sentry-auth-ldap-21.9.8/setup.py` & `sentry-auth-ldap-21.9.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 install_requires = [
     'django-auth-ldap==4.1.0',
     'sentry>=21.9.0',
 ]
 
 setup(
     name='sentry-auth-ldap',
-    version='21.9.8',
+    version='21.9.9',
     author='Chad Killingsworth <chad.killingsworth@banno.com>, Barron Hagerman <barron.hagerman@banno.com>, PM Extra <pm@jubeat.net>',
     author_email='pm@jubeat.net',
     url='https://github.com/PMExtra/sentry-auth-ldap',
     description='A Sentry extension to add an LDAP server as an authentication source.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_namespace_packages(),
```

