# Comparing `tmp/get-spotlights-3.1.tar.gz` & `tmp/get-spotlights-3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\get-spotlights-3.1.tar", last modified: Sun Sep 29 01:34:37 2019, max compression
+gzip compressed data, was "D:\projects\python\get-spotlights\dist\.tmp-2ab_ruyb\get-spotlights-3.2.tar", last modified: Sat Apr 15 06:48:16 2023, max compression
```

## Comparing `get-spotlights-3.1.tar` & `get-spotlights-3.2.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2019-09-29 01:34:37.000000 get-spotlights-3.1/
--rw-rw-rw-   0        0        0     2394 2019-09-29 01:34:37.000000 get-spotlights-3.1/PKG-INFO
--rw-rw-rw-   0        0        0     1554 2019-09-29 01:32:24.000000 get-spotlights-3.1/README.md
-drwxrwxrwx   0        0        0        0 2019-09-29 01:34:37.000000 get-spotlights-3.1/copy_spotlights/
--rw-rw-rw-   0        0        0      104 2019-09-02 09:37:16.000000 get-spotlights-3.1/copy_spotlights/__init__.py
--rw-rw-rw-   0        0        0     1898 2019-09-02 09:37:16.000000 get-spotlights-3.1/copy_spotlights/command_line.py
--rw-rw-rw-   0        0        0     3912 2019-09-02 09:37:16.000000 get-spotlights-3.1/copy_spotlights/copy_spotlights.py
--rw-rw-rw-   0        0        0     4142 2019-09-02 09:37:16.000000 get-spotlights-3.1/copy_spotlights/gui.py
-drwxrwxrwx   0        0        0        0 2019-09-29 01:34:37.000000 get-spotlights-3.1/get_spotlights.egg-info/
--rw-rw-rw-   0        0        0     2394 2019-09-29 01:34:36.000000 get-spotlights-3.1/get_spotlights.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      366 2019-09-29 01:34:37.000000 get-spotlights-3.1/get_spotlights.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2019-09-29 01:34:36.000000 get-spotlights-3.1/get_spotlights.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      131 2019-09-29 01:34:36.000000 get-spotlights-3.1/get_spotlights.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        7 2019-09-29 01:34:36.000000 get-spotlights-3.1/get_spotlights.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2019-09-29 01:34:36.000000 get-spotlights-3.1/get_spotlights.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2019-09-29 01:34:37.000000 get-spotlights-3.1/setup.cfg
--rw-rw-rw-   0        0        0      978 2019-09-29 00:01:04.000000 get-spotlights-3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 06:48:16.000000 get-spotlights-3.2/
+-rw-rw-rw-   0        0        0     3670 2023-04-12 09:14:10.000000 get-spotlights-3.2/LICENSE
+-rw-rw-rw-   0        0        0     2104 2023-04-15 06:48:16.000000 get-spotlights-3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1570 2023-04-15 06:31:12.000000 get-spotlights-3.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-15 06:48:16.000000 get-spotlights-3.2/copy_spotlights/
+-rw-rw-rw-   0        0        0      106 2023-04-15 06:28:04.000000 get-spotlights-3.2/copy_spotlights/__init__.py
+-rw-rw-rw-   0        0        0     2287 2023-04-15 06:25:39.000000 get-spotlights-3.2/copy_spotlights/command_line.py
+-rw-rw-rw-   0        0        0     4221 2023-04-15 06:27:52.000000 get-spotlights-3.2/copy_spotlights/copy_spotlights.py
+-rw-rw-rw-   0        0        0     4582 2023-04-15 06:29:46.000000 get-spotlights-3.2/copy_spotlights/gui.py
+drwxrwxrwx   0        0        0        0 2023-04-15 06:48:16.000000 get-spotlights-3.2/get_spotlights.egg-info/
+-rw-rw-rw-   0        0        0     2104 2023-04-15 06:48:16.000000 get-spotlights-3.2/get_spotlights.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      374 2023-04-15 06:48:16.000000 get-spotlights-3.2/get_spotlights.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 06:48:16.000000 get-spotlights-3.2/get_spotlights.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      130 2023-04-15 06:48:16.000000 get-spotlights-3.2/get_spotlights.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        7 2023-04-15 06:48:16.000000 get-spotlights-3.2/get_spotlights.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-04-15 06:48:16.000000 get-spotlights-3.2/get_spotlights.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-15 06:48:16.000000 get-spotlights-3.2/setup.cfg
+-rw-rw-rw-   0        0        0     1005 2023-04-14 18:51:07.000000 get-spotlights-3.2/setup.py
```

### Comparing `get-spotlights-3.1/PKG-INFO` & `get-spotlights-3.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,33 @@
-Metadata-Version: 2.1
-Name: get-spotlights
-Version: 3.1
-Summary: Love windows 10 spotlight images that show up on lock-screen. Then here's a simple program to copy those images and get them in your preferred directory.
-Home-page: https://github.com/ksharshveer/copy-windows10-spotlight-images
-Author: Harshveer Singh
-Author-email: ksharshveer@gmail.com
-License: MIT
-Description: # copy-windows10-spotlight-images
-        ## Description
-        Love windows 10 spotlight images that show up on lock-screen. Then here's a simple program to copy those images and get them in your preferred directory.
-        
-        ## Installation
-        #### Installing python
-        You will need python 3 installed and available on PATH.<br>
-        To do that click [here](https://www.python.org/downloads/) to go to python downloads page, and download python.<br>
-        Now, open the downloaded installer, select `Add Python 3.* to PATH` as shown below, and click `Install Now`<br>
-        ![Add to PATH screenshot](images/python-addtopath.PNG)<br>
-        
-        #### Installing spotlights app
-        Now, Open command prompt, by searching `cmd` and pressing enter as follows<br>
-        ![search-cmd-screenshot](images/search-cmd.PNG)<br>
-        Enter <code>python -m pip install get-spotlights</code> inside it.<br>
-        ![install-app-command-screenshot](images/get-spotlights-installed.PNG)<br>
-        
-        <br>All set!
-        
-        ## Usage
-        Inside command prompt,<br>
-        * Enter <code>get-spotlights-gui</code> to start the app.<br>
-        ![App's gui screenshot](images/gui.PNG)<br>
-        If default settings seem sound to you, go ahead and click `Get Spotlights` button.
-        
-        * Enter <code>get-spotlights --help</code> to get help if you wish to use it completely from command line.<br>
-        ![command-line-screenshot](images/cmd.PNG)<br>
-        * Command line usage examples -
-          * <code>get-spotlights "C:/Users/YourUserName/Pictures/"</code>
-          ![result1](images/cmdusage1.PNG)<br>
-          
-          * <code>get-spotlights "C:/Users/YourUserName/Pictures/" --no-split</code>
-          ![result2](images/cmdusage2.PNG)<br>
-        
-Keywords: copy extract get windows 10 spotlight spotlights image images lockscreen wallpaper
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
+# Get Spotlights
+## Description
+Love windows 10 spotlight images that show up on lock-screen. Then here's a simple program to copy those images and get them in your preferred directory.
+
+## Installation
+#### Installing python
+You will need python 3 installed and available on PATH.<br>
+To do that click [here](https://www.python.org/downloads/) to go to python downloads page, and download python.<br>
+Now, open the downloaded installer, select `Add Python 3.* to PATH` as shown below, and click `Install Now`<br>
+![Add to PATH screenshot](images/python-addtopath.PNG)<br>
+
+#### Installing spotlights app
+Now, Open command prompt, by searching `cmd` and pressing enter as follows<br>
+![search-cmd-screenshot](images/search-cmd.PNG)<br>
+Enter <code>python -m pip install get-spotlights</code> inside it.<br>
+![install-app-command-screenshot](images/get-spotlights-installed.PNG)<br>
+
+<br>All set!
+
+## Usage
+Inside command prompt,<br>
+* Enter <code>get-spotlights-gui</code> to start the app.<br>
+![App's gui screenshot](images/gui.PNG)<br>
+If default settings seem sound to you, go ahead and click `Get Spotlights` button.
+
+* Enter <code>get-spotlights --help</code> to get help if you wish to use it completely from command line.<br>
+![command-line-screenshot](images/cmd.PNG)<br>
+* Command line usage examples -
+  * <code>get-spotlights "C:/Users/YourUserName/Pictures/"</code>
+  ![result1](images/cmdusage1.PNG)<br>
+  
+  * <code>get-spotlights "C:/Users/YourUserName/Pictures/" --no-split</code>
+  ![result2](images/cmdusage2.PNG)<br>
```

### Comparing `get-spotlights-3.1/README.md` & `get-spotlights-3.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,33 +1,45 @@
-# copy-windows10-spotlight-images
-## Description
-Love windows 10 spotlight images that show up on lock-screen. Then here's a simple program to copy those images and get them in your preferred directory.
-
-## Installation
-#### Installing python
-You will need python 3 installed and available on PATH.<br>
-To do that click [here](https://www.python.org/downloads/) to go to python downloads page, and download python.<br>
-Now, open the downloaded installer, select `Add Python 3.* to PATH` as shown below, and click `Install Now`<br>
-![Add to PATH screenshot](images/python-addtopath.PNG)<br>
-
-#### Installing spotlights app
-Now, Open command prompt, by searching `cmd` and pressing enter as follows<br>
-![search-cmd-screenshot](images/search-cmd.PNG)<br>
-Enter <code>python -m pip install get-spotlights</code> inside it.<br>
-![install-app-command-screenshot](images/get-spotlights-installed.PNG)<br>
-
-<br>All set!
-
-## Usage
-Inside command prompt,<br>
-* Enter <code>get-spotlights-gui</code> to start the app.<br>
-![App's gui screenshot](images/gui.PNG)<br>
-If default settings seem sound to you, go ahead and click `Get Spotlights` button.
-
-* Enter <code>get-spotlights --help</code> to get help if you wish to use it completely from command line.<br>
-![command-line-screenshot](images/cmd.PNG)<br>
-* Command line usage examples -
-  * <code>get-spotlights "C:/Users/YourUserName/Pictures/"</code>
-  ![result1](images/cmdusage1.PNG)<br>
-  
-  * <code>get-spotlights "C:/Users/YourUserName/Pictures/" --no-split</code>
-  ![result2](images/cmdusage2.PNG)<br>
+Metadata-Version: 2.1
+Name: get-spotlights
+Version: 3.2
+Summary: Love windows 10 spotlight images that show up on lock-screen. Then here's a simple program to copy those images and get them in your preferred directory.
+Home-page: https://github.com/ksharshveer/copy-windows10-spotlight-images
+Author: Harshveer Singh
+Author-email: ksharshveer@gmail.com
+License: MIT
+Keywords: copy extract get windows 10 spotlight spotlights image images lockscreen wallpaper
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Get Spotlights
+## Description
+Love windows 10 spotlight images that show up on lock-screen. Then here's a simple program to copy those images and get them in your preferred directory.
+
+## Installation
+#### Installing python
+You will need python 3 installed and available on PATH.<br>
+To do that click [here](https://www.python.org/downloads/) to go to python downloads page, and download python.<br>
+Now, open the downloaded installer, select `Add Python 3.* to PATH` as shown below, and click `Install Now`<br>
+![Add to PATH screenshot](images/python-addtopath.PNG)<br>
+
+#### Installing spotlights app
+Now, Open command prompt, by searching `cmd` and pressing enter as follows<br>
+![search-cmd-screenshot](images/search-cmd.PNG)<br>
+Enter <code>python -m pip install get-spotlights</code> inside it.<br>
+![install-app-command-screenshot](images/get-spotlights-installed.PNG)<br>
+
+<br>All set!
+
+## Usage
+Inside command prompt,<br>
+* Enter <code>get-spotlights-gui</code> to start the app.<br>
+![App's gui screenshot](images/gui.PNG)<br>
+If default settings seem sound to you, go ahead and click `Get Spotlights` button.
+
+* Enter <code>get-spotlights --help</code> to get help if you wish to use it completely from command line.<br>
+![command-line-screenshot](images/cmd.PNG)<br>
+* Command line usage examples -
+  * <code>get-spotlights "C:/Users/YourUserName/Pictures/"</code>
+  ![result1](images/cmdusage1.PNG)<br>
+  
+  * <code>get-spotlights "C:/Users/YourUserName/Pictures/" --no-split</code>
+  ![result2](images/cmdusage2.PNG)<br>
```

### Comparing `get-spotlights-3.1/copy_spotlights/command_line.py` & `get-spotlights-3.2/copy_spotlights/command_line.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,73 @@
-#!/usr/bin/env python3
-from copy_spotlights import copy_spotlights_images
-from argparse import ArgumentParser
-from pathlib import Path
-
-
-def main():
-
-    # Argument Parser to enable use of this program using bash terminal
-    parser = ArgumentParser()
-    parser.add_argument("save_dir", type=str, help="directory location where spotlight images will be copied to")
-    parser.add_argument("--no-split", dest="no_split", action="store_true", help="portrait and landscape images will not be placed into separate folders")
-    parser.add_argument("--min-res", dest="min_res", type=int, help="ignore images with horizontal or vertical resolution lower than min_res value, default:1920", default=1920)
-    parser.add_argument("--dir-land", dest="dir_land", type=str, help="directory name in which to store landscape images, default:landscape", default="landscape")
-    parser.add_argument("--dir-port", dest="dir_port", type=str, help="directory name in which to store portrait images, default:portrait", default="portrait")
-    parser.add_argument("--dir-other", dest="dir_other", type=str, help="directory name in which to store images of equal resolution, default:other", default="other")
-    args = parser.parse_args()
-
-    # Known directory location path where windows stores spotlight images
-    home = Path.home()
-    spotlight_dir = Path.joinpath(home, Path('AppData/Local/Packages/Microsoft.Windows.ContentDeliveryManager_cw5n1h2txyewy/LocalState/Assets'))
-
-    save_dir = args.__getattribute__("save_dir")
-    split = not args.__getattribute__("no_split")
-    min_res = args.__getattribute__("min_res")
-    dir_land = args.__getattribute__("dir_land")
-    dir_port = args.__getattribute__("dir_port")
-    dir_other = args.__getattribute__("dir_other")
-
-    copy_spotlights_images(spotlight_dir, save_dir, split, min_res, dir_land, dir_port, dir_other)
-
-
-if __name__ == "__main__":
-    main()
+#!/usr/bin/env python3
+from copy_spotlights import copy_spotlights_images
+from argparse import ArgumentParser
+from pathlib import Path
+
+
+def main():
+    # Argument Parser to enable use of this program using bash terminal
+    parser = ArgumentParser()
+    parser.add_argument(
+        "save_dir",
+        type=str,
+        help="directory location where spotlight images will be copied to",
+    )
+    parser.add_argument(
+        "--no-split",
+        dest="no_split",
+        action="store_true",
+        help="portrait and landscape images will not be placed into separate folders",
+    )
+    parser.add_argument(
+        "--min-res",
+        dest="min_res",
+        type=int,
+        help="ignore images with horizontal or vertical resolution lower than min_res value, default:1920",
+        default=1920,
+    )
+    parser.add_argument(
+        "--dir-land",
+        dest="dir_land",
+        type=str,
+        help="directory name in which to store landscape images, default:landscape",
+        default="landscape",
+    )
+    parser.add_argument(
+        "--dir-port",
+        dest="dir_port",
+        type=str,
+        help="directory name in which to store portrait images, default:portrait",
+        default="portrait",
+    )
+    parser.add_argument(
+        "--dir-other",
+        dest="dir_other",
+        type=str,
+        help="directory name in which to store images of equal resolution, default:other",
+        default="other",
+    )
+    args = parser.parse_args()
+
+    # Known directory location path where windows stores spotlight images
+    home = Path.home()
+    spotlight_dir = Path.joinpath(
+        home,
+        Path(
+            "AppData/Local/Packages/Microsoft.Windows.ContentDeliveryManager_cw5n1h2txyewy/LocalState/Assets"
+        ),
+    )
+
+    save_dir = args.__getattribute__("save_dir")
+    split = not args.__getattribute__("no_split")
+    min_res = args.__getattribute__("min_res")
+    dir_land = args.__getattribute__("dir_land")
+    dir_port = args.__getattribute__("dir_port")
+    dir_other = args.__getattribute__("dir_other")
+
+    copy_spotlights_images(
+        spotlight_dir, save_dir, split, min_res, dir_land, dir_port, dir_other
+    )
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `get-spotlights-3.1/copy_spotlights/copy_spotlights.py` & `get-spotlights-3.2/copy_spotlights/copy_spotlights.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,99 +1,117 @@
-from os import path, makedirs, listdir
-from shutil import copy
-
-from PIL import Image
-
-
-def find_images(dir):
-    """Given a directory, finds out which files in the root of the directory are images
-
-    Arguments:
-      dir {str} -- directory location to scan for image files
-
-    Raises:
-      AssertionError -- if given directory is not valid
-
-    Returns:
-      list -- list of filenames found in the given directory which are images
-    """
-    assert path.isdir(dir)==True
-
-    im_files = []
-
-    for item in listdir(dir):
-        item_path = path.normpath(path.join(dir, item))
-
-        if path.isfile(item_path):
-            try:
-                Image.open(item_path)
-                im_files.append(item)
-            except IOError:
-                pass
-
-    return im_files
-
-
-def copy_spotlights_images(spotlights_dir, save_dir, split=True, min_res=1920, dir_land="landscape", dir_port="portrait", dir_other="other"):
-    """For Windows 10 users, copies beautiful images stored on their machine, called 'Windows Spotlights' to a directory of their choice.
-
-    Arguments:
-      spotlights_dir {str} -- directory location where windows 10 stores spotlight images
-      save_dir {str} -- directory location where spotlight images will be copied to
-
-    Keyword Arguments:
-      split {bool} -- split images into different folders based on types such as landscape and portrait (default: {True})
-      min_res {int} -- only include images with width or height greater than or equal to {min_res}
-      dir_land {str} -- directory name in which to store landscape images (default: {"landscape"})
-      dir_port {str} -- directory name in which to store portrait images (default: {"portrait"})
-      dir_other {str} -- directory name in which to store images other than portrait or landscape type (default: {"other"})
-
-    Raises:
-      Exception -- raises exception if save_dir is not valid
-    """
-    if not path.isdir(save_dir):
-        raise Exception(f"'{save_dir}' does not seem to be a valid directory!")
-    min_res = int(min_res)
-
-    complete_landscape_path, complete_portrait_path, complete_other_path = "", "", ""
-
-    if split:
-        # get complete paths to landscape, portrait, and other directories inside the save directory
-        complete_landscape_path = path.normpath(path.join(save_dir, dir_land))
-        complete_portrait_path = path.normpath(path.join(save_dir, dir_port))
-        complete_other_path = path.normpath(path.join(save_dir, dir_other))
-
-        # make required directories if they don't exist
-        if not path.isdir(complete_landscape_path):
-            makedirs(complete_landscape_path)
-        if not path.isdir(complete_portrait_path):
-            makedirs(complete_portrait_path)
-        if not path.isdir(complete_other_path):
-            makedirs(complete_other_path)
-
-    else:
-        # don't copy spotlight images into different folders
-        complete_landscape_path, complete_portrait_path, complete_other_path = save_dir, save_dir, save_dir
-
-    for image_file in find_images(spotlights_dir):
-        image_file_full_path = path.normpath(path.join(spotlights_dir, image_file))
-
-        im = Image.open(image_file_full_path)
-
-        # save image with an extension as read by PIL.Image module
-        save_image_file_name = image_file + "." + im.format
-        where = None
-
-        im_width, im_height = int(im.size[0]), int(im.size[1])
-
-        if im_width >= min_res or im_height >= min_res:
-            if (im_height < im_width):
-                where = path.normpath(path.join(complete_landscape_path, save_image_file_name))
-
-            elif (im_width < im_height):
-                where = path.normpath(path.join(complete_portrait_path, save_image_file_name))
-
-            else:
-                where = path.normpath(path.join(complete_other_path, save_image_file_name))
-
-        if where is not None:
-            copy(image_file_full_path, where)
+from os import path, makedirs, listdir
+from shutil import copy
+
+from PIL import Image
+
+
+def find_images(dir):
+    """Given a directory, finds out which files in the root of the directory are images
+
+    Arguments:
+      dir {str} -- directory location to scan for image files
+
+    Raises:
+      AssertionError -- if given directory is not valid
+
+    Returns:
+      list -- list of filenames found in the given directory which are images
+    """
+    assert path.isdir(dir) == True
+
+    im_files = []
+
+    for item in listdir(dir):
+        item_path = path.normpath(path.join(dir, item))
+
+        if path.isfile(item_path):
+            try:
+                Image.open(item_path)
+                im_files.append(item)
+            except IOError:
+                pass
+
+    return im_files
+
+
+def copy_spotlights_images(
+    spotlights_dir,
+    save_dir,
+    split=True,
+    min_res=1920,
+    dir_land="landscape",
+    dir_port="portrait",
+    dir_other="other",
+):
+    """For Windows 10 users, copies beautiful images stored on their machine, called 'Windows Spotlights' to a directory of their choice.
+
+    Arguments:
+      spotlights_dir {str} -- directory location where windows 10 stores spotlight images
+      save_dir {str} -- directory location where spotlight images will be copied to
+
+    Keyword Arguments:
+      split {bool} -- split images into different folders based on types such as landscape and portrait (default: {True})
+      min_res {int} -- only include images with width or height greater than or equal to {min_res}
+      dir_land {str} -- directory name in which to store landscape images (default: {"landscape"})
+      dir_port {str} -- directory name in which to store portrait images (default: {"portrait"})
+      dir_other {str} -- directory name in which to store images other than portrait or landscape type (default: {"other"})
+
+    Raises:
+      Exception -- raises exception if save_dir is not valid
+    """
+    if not path.isdir(save_dir):
+        raise Exception(f"'{save_dir}' does not seem to be a valid directory!")
+    min_res = int(min_res)
+
+    complete_landscape_path, complete_portrait_path, complete_other_path = "", "", ""
+
+    if split:
+        # get complete paths to landscape, portrait, and other directories inside the save directory
+        complete_landscape_path = path.normpath(path.join(save_dir, dir_land))
+        complete_portrait_path = path.normpath(path.join(save_dir, dir_port))
+        complete_other_path = path.normpath(path.join(save_dir, dir_other))
+
+        # make required directories if they don't exist
+        if not path.isdir(complete_landscape_path):
+            makedirs(complete_landscape_path)
+        if not path.isdir(complete_portrait_path):
+            makedirs(complete_portrait_path)
+        if not path.isdir(complete_other_path):
+            makedirs(complete_other_path)
+
+    else:
+        # don't copy spotlight images into different folders
+        complete_landscape_path, complete_portrait_path, complete_other_path = (
+            save_dir,
+            save_dir,
+            save_dir,
+        )
+
+    for image_file in find_images(spotlights_dir):
+        image_file_full_path = path.normpath(path.join(spotlights_dir, image_file))
+
+        im = Image.open(image_file_full_path)
+
+        # save image with an extension as read by PIL.Image module
+        save_image_file_name = image_file + "." + im.format
+        where = None
+
+        im_width, im_height = int(im.size[0]), int(im.size[1])
+
+        if im_width >= min_res or im_height >= min_res:
+            if im_height < im_width:
+                where = path.normpath(
+                    path.join(complete_landscape_path, save_image_file_name)
+                )
+
+            elif im_width < im_height:
+                where = path.normpath(
+                    path.join(complete_portrait_path, save_image_file_name)
+                )
+
+            else:
+                where = path.normpath(
+                    path.join(complete_other_path, save_image_file_name)
+                )
+
+        if where is not None:
+            copy(image_file_full_path, where)
```

### Comparing `get-spotlights-3.1/copy_spotlights/gui.py` & `get-spotlights-3.2/copy_spotlights/gui.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,106 +1,130 @@
-from tkinter import Tk, Label, Button, Entry, Checkbutton, filedialog
-from pathlib import Path
-from copy_spotlights import copy_spotlights_images
-
-# default padding settings
-px = 20
-py = 10
-
-
-class MyGui:
-
-    def __init__(self):
-
-        self.window = Tk()
-        self.window.title('Extract Spotlight Images')
-
-        # setting default values for variables
-        self.home = Path.home()
-        self.source_location = Path.joinpath(self.home, Path('AppData/Local/Packages/Microsoft.Windows.ContentDeliveryManager_cw5n1h2txyewy/LocalState/Assets'))
-        self.save_location = Path.joinpath(self.home, Path('Desktop'))
-        self.split = True
-        self.min_res = 1920
-
-        # setting up buttons and their actions
-        self.b_save = Button(self.window, text="Save Location", command=self.set_save_location)
-        self.b_source = Button(self.window, text="Spotlights source", command=self.set_source_location)
-        self.b_reset = Button(self.window, text="Set Defaults", command=self.reset)
-        self.b_split = Checkbutton(self.window, text="Don't split", command=self.toggle_split)
-        self.b_min_res = Entry(self.window, textvariable=self.min_res)
-        self.b_main = Button(self.window, text="Get Spotlights", command=self.copy_spotlights, fg="white", bg="green", bd=4)
-
-        # setting up labels to represent button actions
-        self.l_save = Label(self.window, text=self.save_location)
-        self.l_source = Label(self.window, text=self.source_location)
-        self.l_settings = Label(self.window, text="Advanced Settings below :")
-        self.l_split = Label(self.window, text="If checked, landscape and portrait image will not be separated")
-        self.l_min_res = Label(self.window, text="Only include images with width or height greater than or equal to this value")
-
-        self.setup_button_layouts()
-        self.setup_label_layouts()
-
-        self.window.mainloop()
-
-    def setup_button_layouts(self):
-        self.b_save.grid(row=0, column=0, padx=px, pady=py)
-        self.b_source.grid(row=3, column=0, padx=px, pady=py)
-        self.b_min_res.grid(row=5, column=0, padx=px, pady=py)
-        self.b_min_res.insert(0, self.min_res)
-        self.b_reset.grid(row=6, column=0, padx=px, pady=py)
-        self.b_split.grid(row=4, column=0, padx=px, pady=py)
-        self.b_main.grid(row=1, columnspan=2, padx=2*px, pady=2*py)
-
-    def setup_label_layouts(self):
-        self.l_save.grid(row=0, column=1, padx=px, pady=py)
-        self.l_source.grid(row=3, column=1, padx=px, pady=py)
-        self.l_split.grid(row=4, column=1, padx=px, pady=py)
-        self.l_settings.grid(row=2, column=0, padx=px, pady=py)
-        self.l_source.grid(row=3, column=1, padx=px, pady=py)
-        self.l_min_res.grid(row=5, column=1, padx=px, pady=py)
-
-    def update_labels(self):
-        self.l_save.destroy()
-        self.l_save = Label(self.window, text=self.save_location)
-        self.l_source.destroy()
-        self.l_source = Label(self.window, text=self.source_location)
-        self.setup_label_layouts()
-
-    def set_source_location(self):
-        source_location = filedialog.askdirectory()
-        if source_location:
-            self.source_location = source_location
-        self.update_labels()
-
-    def set_save_location(self):
-        save_location = filedialog.askdirectory()
-        if save_location:
-            self.save_location = save_location
-        self.update_labels()
-
-    def toggle_split(self):
-        self.split = False if self.split else True
-
-    def copy_spotlights(self):
-        min_res = self.b_min_res.get()
-        if min_res:
-            self.min_res = min_res
-        copy_spotlights_images(self.source_location, self.save_location, self.split, self.min_res)
-        self.popup_finished()
-
-    @staticmethod
-    def popup_finished():
-        done = Tk()
-        Label(done, text="Finished!").grid(row=0, columnspan=3, padx=2*px, pady=py)
-        Button(done, text="Ok", command=done.destroy).grid(row=1, column=1, padx=px)
-
-    def reset(self):
-        self.window.destroy()
-        self.__init__()
-
-
-def main():
-    MyGui()
-
-
-if __name__ == '__main__':
-    main()
+from tkinter import Tk, Label, Button, Entry, Checkbutton, filedialog
+from pathlib import Path
+from copy_spotlights import copy_spotlights_images
+
+# default padding settings
+px = 20
+py = 10
+
+
+class MyGui:
+    def __init__(self):
+        self.window = Tk()
+        self.window.title("Extract Spotlight Images")
+
+        # setting default values for variables
+        self.home = Path.home()
+        self.source_location = Path.joinpath(
+            self.home,
+            Path(
+                "AppData/Local/Packages/Microsoft.Windows.ContentDeliveryManager_cw5n1h2txyewy/LocalState/Assets"
+            ),
+        )
+        self.save_location = Path.joinpath(self.home, Path("Desktop"))
+        self.split = True
+        self.min_res = 1920
+
+        # setting up buttons and their actions
+        self.b_save = Button(
+            self.window, text="Save Location", command=self.set_save_location
+        )
+        self.b_source = Button(
+            self.window, text="Spotlights source", command=self.set_source_location
+        )
+        self.b_reset = Button(self.window, text="Set Defaults", command=self.reset)
+        self.b_split = Checkbutton(
+            self.window, text="Don't split", command=self.toggle_split
+        )
+        self.b_min_res = Entry(self.window, textvariable=self.min_res)
+        self.b_main = Button(
+            self.window,
+            text="Get Spotlights",
+            command=self.copy_spotlights,
+            fg="white",
+            bg="green",
+            bd=4,
+        )
+
+        # setting up labels to represent button actions
+        self.l_save = Label(self.window, text=self.save_location)
+        self.l_source = Label(self.window, text=self.source_location)
+        self.l_settings = Label(self.window, text="Advanced Settings below :")
+        self.l_split = Label(
+            self.window,
+            text="If checked, landscape and portrait image will not be separated",
+        )
+        self.l_min_res = Label(
+            self.window,
+            text="Only include images with width or height greater than or equal to this value",
+        )
+
+        self.setup_button_layouts()
+        self.setup_label_layouts()
+
+        self.window.mainloop()
+
+    def setup_button_layouts(self):
+        self.b_save.grid(row=0, column=0, padx=px, pady=py)
+        self.b_source.grid(row=3, column=0, padx=px, pady=py)
+        self.b_min_res.grid(row=5, column=0, padx=px, pady=py)
+        self.b_min_res.insert(0, self.min_res)
+        self.b_reset.grid(row=6, column=0, padx=px, pady=py)
+        self.b_split.grid(row=4, column=0, padx=px, pady=py)
+        self.b_main.grid(row=1, columnspan=2, padx=2 * px, pady=2 * py)
+
+    def setup_label_layouts(self):
+        self.l_save.grid(row=0, column=1, padx=px, pady=py)
+        self.l_source.grid(row=3, column=1, padx=px, pady=py)
+        self.l_split.grid(row=4, column=1, padx=px, pady=py)
+        self.l_settings.grid(row=2, column=0, padx=px, pady=py)
+        self.l_source.grid(row=3, column=1, padx=px, pady=py)
+        self.l_min_res.grid(row=5, column=1, padx=px, pady=py)
+
+    def update_labels(self):
+        self.l_save.destroy()
+        self.l_save = Label(self.window, text=self.save_location)
+        self.l_source.destroy()
+        self.l_source = Label(self.window, text=self.source_location)
+        self.setup_label_layouts()
+
+    def set_source_location(self):
+        source_location = filedialog.askdirectory()
+        if source_location:
+            self.source_location = source_location
+        self.update_labels()
+
+    def set_save_location(self):
+        save_location = filedialog.askdirectory()
+        if save_location:
+            self.save_location = save_location
+        self.update_labels()
+
+    def toggle_split(self):
+        self.split = False if self.split else True
+
+    def copy_spotlights(self):
+        min_res = self.b_min_res.get()
+        if min_res:
+            self.min_res = min_res
+        copy_spotlights_images(
+            self.source_location, self.save_location, self.split, self.min_res
+        )
+        self.popup_finished()
+
+    @staticmethod
+    def popup_finished():
+        done = Tk()
+        Label(done, text="Finished!").grid(row=0, columnspan=3, padx=2 * px, pady=py)
+        Button(done, text="Ok", command=done.destroy).grid(row=1, column=1, padx=px)
+
+    def reset(self):
+        self.window.destroy()
+        self.__init__()
+
+
+def main():
+    MyGui()
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `get-spotlights-3.1/get_spotlights.egg-info/PKG-INFO` & `get-spotlights-3.2/get_spotlights.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 Metadata-Version: 2.1
 Name: get-spotlights
-Version: 3.1
+Version: 3.2
 Summary: Love windows 10 spotlight images that show up on lock-screen. Then here's a simple program to copy those images and get them in your preferred directory.
 Home-page: https://github.com/ksharshveer/copy-windows10-spotlight-images
 Author: Harshveer Singh
 Author-email: ksharshveer@gmail.com
 License: MIT
-Description: # copy-windows10-spotlight-images
-        ## Description
-        Love windows 10 spotlight images that show up on lock-screen. Then here's a simple program to copy those images and get them in your preferred directory.
-        
-        ## Installation
-        #### Installing python
-        You will need python 3 installed and available on PATH.<br>
-        To do that click [here](https://www.python.org/downloads/) to go to python downloads page, and download python.<br>
-        Now, open the downloaded installer, select `Add Python 3.* to PATH` as shown below, and click `Install Now`<br>
-        ![Add to PATH screenshot](images/python-addtopath.PNG)<br>
-        
-        #### Installing spotlights app
-        Now, Open command prompt, by searching `cmd` and pressing enter as follows<br>
-        ![search-cmd-screenshot](images/search-cmd.PNG)<br>
-        Enter <code>python -m pip install get-spotlights</code> inside it.<br>
-        ![install-app-command-screenshot](images/get-spotlights-installed.PNG)<br>
-        
-        <br>All set!
-        
-        ## Usage
-        Inside command prompt,<br>
-        * Enter <code>get-spotlights-gui</code> to start the app.<br>
-        ![App's gui screenshot](images/gui.PNG)<br>
-        If default settings seem sound to you, go ahead and click `Get Spotlights` button.
-        
-        * Enter <code>get-spotlights --help</code> to get help if you wish to use it completely from command line.<br>
-        ![command-line-screenshot](images/cmd.PNG)<br>
-        * Command line usage examples -
-          * <code>get-spotlights "C:/Users/YourUserName/Pictures/"</code>
-          ![result1](images/cmdusage1.PNG)<br>
-          
-          * <code>get-spotlights "C:/Users/YourUserName/Pictures/" --no-split</code>
-          ![result2](images/cmdusage2.PNG)<br>
-        
 Keywords: copy extract get windows 10 spotlight spotlights image images lockscreen wallpaper
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Get Spotlights
+## Description
+Love windows 10 spotlight images that show up on lock-screen. Then here's a simple program to copy those images and get them in your preferred directory.
+
+## Installation
+#### Installing python
+You will need python 3 installed and available on PATH.<br>
+To do that click [here](https://www.python.org/downloads/) to go to python downloads page, and download python.<br>
+Now, open the downloaded installer, select `Add Python 3.* to PATH` as shown below, and click `Install Now`<br>
+![Add to PATH screenshot](images/python-addtopath.PNG)<br>
+
+#### Installing spotlights app
+Now, Open command prompt, by searching `cmd` and pressing enter as follows<br>
+![search-cmd-screenshot](images/search-cmd.PNG)<br>
+Enter <code>python -m pip install get-spotlights</code> inside it.<br>
+![install-app-command-screenshot](images/get-spotlights-installed.PNG)<br>
+
+<br>All set!
+
+## Usage
+Inside command prompt,<br>
+* Enter <code>get-spotlights-gui</code> to start the app.<br>
+![App's gui screenshot](images/gui.PNG)<br>
+If default settings seem sound to you, go ahead and click `Get Spotlights` button.
+
+* Enter <code>get-spotlights --help</code> to get help if you wish to use it completely from command line.<br>
+![command-line-screenshot](images/cmd.PNG)<br>
+* Command line usage examples -
+  * <code>get-spotlights "C:/Users/YourUserName/Pictures/"</code>
+  ![result1](images/cmdusage1.PNG)<br>
+  
+  * <code>get-spotlights "C:/Users/YourUserName/Pictures/" --no-split</code>
+  ![result2](images/cmdusage2.PNG)<br>
```

### Comparing `get-spotlights-3.1/setup.py` & `get-spotlights-3.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from setuptools import setup
-
-with open("README.md", "r") as fh:
-    long_description = fh.read()
-
-setup(
-    name='get-spotlights',
-    version='3.1',
-    install_requires='pillow',
-    packages=['copy_spotlights'],
-    entry_points = {
-        "console_scripts": [
-            "get-spotlights = copy_spotlights.command_line:main",
-        ],
-        "gui_scripts": [
-            "get-spotlights-gui = copy_spotlights.gui:main",
-        ],
-    },
-    url='https://github.com/ksharshveer/copy-windows10-spotlight-images',
-    license='MIT',
-    author='Harshveer Singh',
-    author_email='ksharshveer@gmail.com',
-    description='Love windows 10 spotlight images that show up on lock-screen. Then here\'s a simple program to copy those images and get them in your preferred directory.',
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    keywords='copy extract get windows 10 spotlight spotlights image images lockscreen wallpaper',
-)
+from setuptools import setup
+
+with open("README.md", "r") as fh:
+    long_description = fh.read()
+
+setup(
+    name='get-spotlights',
+    version='3.2',
+    install_requires='pillow',
+    packages=['copy_spotlights'],
+    entry_points = {
+        "console_scripts": [
+            "get-spotlights = copy_spotlights.command_line:main",
+        ],
+        "gui_scripts": [
+            "get-spotlights-gui = copy_spotlights.gui:main",
+        ],
+    },
+    url='https://github.com/ksharshveer/copy-windows10-spotlight-images',
+    license='MIT',
+    author='Harshveer Singh',
+    author_email='ksharshveer@gmail.com',
+    description='Love windows 10 spotlight images that show up on lock-screen. Then here\'s a simple program to copy those images and get them in your preferred directory.',
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    keywords='copy extract get windows 10 spotlight spotlights image images lockscreen wallpaper',
+)
```

