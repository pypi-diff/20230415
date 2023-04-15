# Comparing `tmp/xontrib-pm-0.3.0.tar.gz` & `tmp/xontrib-pm-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xontrib-pm-0.3.0.tar", last modified: Sun Mar 26 16:23:45 2023, max compression
+gzip compressed data, was "xontrib-pm-0.3.1.tar", last modified: Sat Apr 15 07:33:07 2023, max compression
```

## Comparing `xontrib-pm-0.3.0.tar` & `xontrib-pm-0.3.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 16:23:45.021229 xontrib-pm-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-03-26 16:23:33.000000 xontrib-pm-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-03-26 16:23:45.021229 xontrib-pm-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-03-26 16:23:33.000000 xontrib-pm-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-03-26 16:23:33.000000 xontrib-pm-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-26 16:23:45.021229 xontrib-pm-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-26 16:23:33.000000 xontrib-pm-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 16:23:45.021229 xontrib-pm-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-03-26 16:23:33.000000 xontrib-pm-0.3.0/tests/test_xontrib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 16:23:45.021229 xontrib-pm-0.3.0/xontrib/
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-03-26 16:23:33.000000 xontrib-pm-0.3.0/xontrib/pm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 16:23:45.021229 xontrib-pm-0.3.0/xontrib_pm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-03-26 16:23:45.000000 xontrib-pm-0.3.0/xontrib_pm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-03-26 16:23:45.000000 xontrib-pm-0.3.0/xontrib_pm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-26 16:23:45.000000 xontrib-pm-0.3.0/xontrib_pm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-26 16:23:45.000000 xontrib-pm-0.3.0/xontrib_pm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-26 16:23:45.000000 xontrib-pm-0.3.0/xontrib_pm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 07:33:07.101290 xontrib-pm-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-15 07:32:50.000000 xontrib-pm-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-04-15 07:33:07.101290 xontrib-pm-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-04-15 07:32:50.000000 xontrib-pm-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-04-15 07:32:50.000000 xontrib-pm-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 07:33:07.101290 xontrib-pm-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-15 07:32:50.000000 xontrib-pm-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 07:33:07.101290 xontrib-pm-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-15 07:32:50.000000 xontrib-pm-0.3.1/tests/test_xontrib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 07:33:07.101290 xontrib-pm-0.3.1/xontrib/
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-04-15 07:32:50.000000 xontrib-pm-0.3.1/xontrib/pm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 07:33:07.101290 xontrib-pm-0.3.1/xontrib_pm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-04-15 07:33:07.000000 xontrib-pm-0.3.1/xontrib_pm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-15 07:33:07.000000 xontrib-pm-0.3.1/xontrib_pm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 07:33:07.000000 xontrib-pm-0.3.1/xontrib_pm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-15 07:33:07.000000 xontrib-pm-0.3.1/xontrib_pm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-15 07:33:07.000000 xontrib-pm-0.3.1/xontrib_pm.egg-info/top_level.txt
```

### Comparing `xontrib-pm-0.3.0/LICENSE` & `xontrib-pm-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xontrib-pm-0.3.0/PKG-INFO` & `xontrib-pm-0.3.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xontrib-pm
-Version: 0.3.0
+Version: 0.3.1
 Summary: Copy output to clipboard.
 Author-email: anki-code <no@no.no>
 License: MIT License
         
         Copyright (c) 2023, anki-code
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -64,29 +64,33 @@
 
 ```xsh
 xontrib load pm
 pm
 # pacman, brew
 
 # Type `pacman-` and press Tab
-pacman-search vim  # sudo pacman -Ss vim
-pacman-install vim  # sudo pacman -Sy vim
+pacman-search vim    # sudo pacman -Ss vim
+pacman-install vim   # sudo pacman -Sy vim
 ```
 
 Feel free to extand the list of known package managers.
 
+## Supported package managers
+
+PMs: `apt`, `brew`, `guix`, `pacman`, `port`, `yum`, `zap`. Feel free to add more, PR is welcome!
+
 ## Commands
 
-The list of commands that need to have the package manager:
+The list of commands that need to have the package manager aliases i.e. `<package_manager>-<command>`:
 * `search` - serach the package
 * `install` - install the package
 * `uninstall` - uninstall the package
 
 Optinally:
-* `instally` - install without user confirmation
+* `instally` (install and say yes) - install without user confirmation
 * `installed` - list of installed packages
 * Any other useful aliases e.g. `pacman-upgrade-everything`.
 
 ## Credits
 
 * [Package manager-independent bash aliases](https://gist.github.com/rroblak/8137276)
 * This package was created with [xontrib template](https://github.com/xonsh/xontrib-template).
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: xontrib-pm Version: 0.3.0 Summary: Copy output to
+Metadata-Version: 2.1 Name: xontrib-pm Version: 0.3.1 Summary: Copy output to
 clipboard. Author-email: anki-code
 no.no> License: MIT License Copyright (c) 2023, anki-code Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
@@ -30,15 +30,17 @@
 install -U git+https://github.com/anki-code/xontrib-pm ``` ## Usage After
 loading xontrib-pm is searching the known package managers. If the package
 manager installed (e.g. `pacman`) the xontrib adds the aliases e.g. `pacman-
 install`, `pacman-search`, etc. The `pm` command returns the list of known
 installed package managers. ```xsh xontrib load pm pm # pacman, brew # Type
 `pacman-` and press Tab pacman-search vim # sudo pacman -Ss vim pacman-install
 vim # sudo pacman -Sy vim ``` Feel free to extand the list of known package
-managers. ## Commands The list of commands that need to have the package
-manager: * `search` - serach the package * `install` - install the package *
-`uninstall` - uninstall the package Optinally: * `instally` - install without
-user confirmation * `installed` - list of installed packages * Any other useful
-aliases e.g. `pacman-upgrade-everything`. ## Credits * [Package manager-
-independent bash aliases](https://gist.github.com/rroblak/8137276) * This
-package was created with [xontrib template](https://github.com/xonsh/xontrib-
-template).
+managers. ## Supported package managers PMs: `apt`, `brew`, `guix`, `pacman`,
+`port`, `yum`, `zap`. Feel free to add more, PR is welcome! ## Commands The
+list of commands that need to have the package manager aliases i.e. `-`: *
+`search` - serach the package * `install` - install the package * `uninstall` -
+uninstall the package Optinally: * `instally` (install and say yes) - install
+without user confirmation * `installed` - list of installed packages * Any
+other useful aliases e.g. `pacman-upgrade-everything`. ## Credits * [Package
+manager-independent bash aliases](https://gist.github.com/rroblak/8137276) *
+This package was created with [xontrib template](https://github.com/xonsh/
+xontrib-template).
```

### Comparing `xontrib-pm-0.3.0/README.md` & `xontrib-pm-0.3.1/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -21,29 +21,33 @@
 
 ```xsh
 xontrib load pm
 pm
 # pacman, brew
 
 # Type `pacman-` and press Tab
-pacman-search vim  # sudo pacman -Ss vim
-pacman-install vim  # sudo pacman -Sy vim
+pacman-search vim    # sudo pacman -Ss vim
+pacman-install vim   # sudo pacman -Sy vim
 ```
 
 Feel free to extand the list of known package managers.
 
+## Supported package managers
+
+PMs: `apt`, `brew`, `guix`, `pacman`, `port`, `yum`, `zap`. Feel free to add more, PR is welcome!
+
 ## Commands
 
-The list of commands that need to have the package manager:
+The list of commands that need to have the package manager aliases i.e. `<package_manager>-<command>`:
 * `search` - serach the package
 * `install` - install the package
 * `uninstall` - uninstall the package
 
 Optinally:
-* `instally` - install without user confirmation
+* `instally` (install and say yes) - install without user confirmation
 * `installed` - list of installed packages
 * Any other useful aliases e.g. `pacman-upgrade-everything`.
 
 ## Credits
 
 * [Package manager-independent bash aliases](https://gist.github.com/rroblak/8137276)
 * This package was created with [xontrib template](https://github.com/xonsh/xontrib-template).
```

#### html2text {}

```diff
@@ -4,15 +4,17 @@
 install -U git+https://github.com/anki-code/xontrib-pm ``` ## Usage After
 loading xontrib-pm is searching the known package managers. If the package
 manager installed (e.g. `pacman`) the xontrib adds the aliases e.g. `pacman-
 install`, `pacman-search`, etc. The `pm` command returns the list of known
 installed package managers. ```xsh xontrib load pm pm # pacman, brew # Type
 `pacman-` and press Tab pacman-search vim # sudo pacman -Ss vim pacman-install
 vim # sudo pacman -Sy vim ``` Feel free to extand the list of known package
-managers. ## Commands The list of commands that need to have the package
-manager: * `search` - serach the package * `install` - install the package *
-`uninstall` - uninstall the package Optinally: * `instally` - install without
-user confirmation * `installed` - list of installed packages * Any other useful
-aliases e.g. `pacman-upgrade-everything`. ## Credits * [Package manager-
-independent bash aliases](https://gist.github.com/rroblak/8137276) * This
-package was created with [xontrib template](https://github.com/xonsh/xontrib-
-template).
+managers. ## Supported package managers PMs: `apt`, `brew`, `guix`, `pacman`,
+`port`, `yum`, `zap`. Feel free to add more, PR is welcome! ## Commands The
+list of commands that need to have the package manager aliases i.e. `-`: *
+`search` - serach the package * `install` - install the package * `uninstall` -
+uninstall the package Optinally: * `instally` (install and say yes) - install
+without user confirmation * `installed` - list of installed packages * Any
+other useful aliases e.g. `pacman-upgrade-everything`. ## Credits * [Package
+manager-independent bash aliases](https://gist.github.com/rroblak/8137276) *
+This package was created with [xontrib template](https://github.com/xonsh/
+xontrib-template).
```

### Comparing `xontrib-pm-0.3.0/pyproject.toml` & `xontrib-pm-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [project]
 name = "xontrib-pm"
-version = "0.3.0"
+version = "0.3.1"
 license = {file = "LICENSE"}
 description = "Copy output to clipboard."
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Topic :: System :: Shells",
```

### Comparing `xontrib-pm-0.3.0/xontrib/pm.py` & `xontrib-pm-0.3.1/xontrib/pm.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,15 +33,22 @@
         'instally': 'sudo yum install -y',
         'uninstall': 'sudo yum uninstall',
         'search': 'sudo yum search',
     },
     'zap': { # https://github.com/srevinsaju/zap
         'install': 'sudo zap install',
         'search': 'sudo zap search',
-    }
+    },
+    'guix': {
+        'install': 'guix install',
+        'uninstall': 'guix remove',
+        'search': 'guix search',
+        'upgrade-everything': 'guix upgrade',
+        'package-info': 'guix show',
+    },
 }
 
 
 _found_pm = []
 for p in _pm.keys():
     if _which(p):
         _found_pm.append(p)
```

### Comparing `xontrib-pm-0.3.0/xontrib_pm.egg-info/PKG-INFO` & `xontrib-pm-0.3.1/xontrib_pm.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xontrib-pm
-Version: 0.3.0
+Version: 0.3.1
 Summary: Copy output to clipboard.
 Author-email: anki-code <no@no.no>
 License: MIT License
         
         Copyright (c) 2023, anki-code
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -64,29 +64,33 @@
 
 ```xsh
 xontrib load pm
 pm
 # pacman, brew
 
 # Type `pacman-` and press Tab
-pacman-search vim  # sudo pacman -Ss vim
-pacman-install vim  # sudo pacman -Sy vim
+pacman-search vim    # sudo pacman -Ss vim
+pacman-install vim   # sudo pacman -Sy vim
 ```
 
 Feel free to extand the list of known package managers.
 
+## Supported package managers
+
+PMs: `apt`, `brew`, `guix`, `pacman`, `port`, `yum`, `zap`. Feel free to add more, PR is welcome!
+
 ## Commands
 
-The list of commands that need to have the package manager:
+The list of commands that need to have the package manager aliases i.e. `<package_manager>-<command>`:
 * `search` - serach the package
 * `install` - install the package
 * `uninstall` - uninstall the package
 
 Optinally:
-* `instally` - install without user confirmation
+* `instally` (install and say yes) - install without user confirmation
 * `installed` - list of installed packages
 * Any other useful aliases e.g. `pacman-upgrade-everything`.
 
 ## Credits
 
 * [Package manager-independent bash aliases](https://gist.github.com/rroblak/8137276)
 * This package was created with [xontrib template](https://github.com/xonsh/xontrib-template).
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: xontrib-pm Version: 0.3.0 Summary: Copy output to
+Metadata-Version: 2.1 Name: xontrib-pm Version: 0.3.1 Summary: Copy output to
 clipboard. Author-email: anki-code
 no.no> License: MIT License Copyright (c) 2023, anki-code Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
@@ -30,15 +30,17 @@
 install -U git+https://github.com/anki-code/xontrib-pm ``` ## Usage After
 loading xontrib-pm is searching the known package managers. If the package
 manager installed (e.g. `pacman`) the xontrib adds the aliases e.g. `pacman-
 install`, `pacman-search`, etc. The `pm` command returns the list of known
 installed package managers. ```xsh xontrib load pm pm # pacman, brew # Type
 `pacman-` and press Tab pacman-search vim # sudo pacman -Ss vim pacman-install
 vim # sudo pacman -Sy vim ``` Feel free to extand the list of known package
-managers. ## Commands The list of commands that need to have the package
-manager: * `search` - serach the package * `install` - install the package *
-`uninstall` - uninstall the package Optinally: * `instally` - install without
-user confirmation * `installed` - list of installed packages * Any other useful
-aliases e.g. `pacman-upgrade-everything`. ## Credits * [Package manager-
-independent bash aliases](https://gist.github.com/rroblak/8137276) * This
-package was created with [xontrib template](https://github.com/xonsh/xontrib-
-template).
+managers. ## Supported package managers PMs: `apt`, `brew`, `guix`, `pacman`,
+`port`, `yum`, `zap`. Feel free to add more, PR is welcome! ## Commands The
+list of commands that need to have the package manager aliases i.e. `-`: *
+`search` - serach the package * `install` - install the package * `uninstall` -
+uninstall the package Optinally: * `instally` (install and say yes) - install
+without user confirmation * `installed` - list of installed packages * Any
+other useful aliases e.g. `pacman-upgrade-everything`. ## Credits * [Package
+manager-independent bash aliases](https://gist.github.com/rroblak/8137276) *
+This package was created with [xontrib template](https://github.com/xonsh/
+xontrib-template).
```

