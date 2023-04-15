# Comparing `tmp/cpct-0.1.9.tar.gz` & `tmp/cpct-0.2.1.tar.gz`

## Comparing `cpct-0.1.9.tar` & `cpct-0.2.1.tar`

### file list

```diff
@@ -1,24 +1,26 @@
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 cpct-0.1.9/cpct/__about__.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 cpct-0.1.9/cpct/__init__.py
--rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 cpct-0.1.9/cpct/base_types.py
--rw-r--r--   0        0        0    21073 2020-02-02 00:00:00.000000 cpct-0.1.9/cpct/cpct.py
--rwxr-xr-x   0        0        0      111 2020-02-02 00:00:00.000000 cpct-0.1.9/cpct/cpct_START_HERE.cmd
--rwxr-xr-x   0        0        0       92 2020-02-02 00:00:00.000000 cpct-0.1.9/cpct/cpct_download.bat
--rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 cpct-0.1.9/cpct/cpct_install_requirements.py
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 cpct-0.1.9/cpct/discord.py
--rw-r--r--   0        0        0    20925 2020-02-02 00:00:00.000000 cpct-0.1.9/cpct/poepy.py
--rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 cpct-0.1.9/cpct/user_info.py
--rw-r--r--   0        0        0   329881 2020-02-02 00:00:00.000000 cpct-0.1.9/cpct/img/ChipyLogo.png
--rw-r--r--   0        0        0  1621531 2020-02-02 00:00:00.000000 cpct-0.1.9/cpct/img/ChipyLogo.psd
--rw-r--r--   0        0        0   329881 2020-02-02 00:00:00.000000 cpct-0.1.9/cpct/img/cpct_logo.png
--rw-r--r--   0        0        0    31307 2020-02-02 00:00:00.000000 cpct-0.1.9/cpct/img/ctcp_gui.png
--rw-r--r--   0        0        0     4116 2020-02-02 00:00:00.000000 cpct-0.1.9/cpct/img/dropper.png
--rw-r--r--   0        0        0   678371 2020-02-02 00:00:00.000000 cpct-0.1.9/cpct/img/poe.png
--rwxr-xr-x   0        0        0       38 2020-02-02 00:00:00.000000 cpct-0.1.9/cpct/qt/build_gui.bat
--rw-r--r--   0        0        0    33527 2020-02-02 00:00:00.000000 cpct-0.1.9/cpct/qt/main_gui.py
--rw-r--r--   0        0        0    34751 2020-02-02 00:00:00.000000 cpct-0.1.9/cpct/qt/main_gui.ui
--rw-r--r--   0        0        0     1975 2020-02-02 00:00:00.000000 cpct-0.1.9/.gitignore
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 cpct-0.1.9/LICENSE.txt
--rw-r--r--   0        0        0     4707 2020-02-02 00:00:00.000000 cpct-0.1.9/README.md
--rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 cpct-0.1.9/pyproject.toml
--rw-r--r--   0        0        0     5628 2020-02-02 00:00:00.000000 cpct-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 cpct-0.2.1/cpct/__about__.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 cpct-0.2.1/cpct/__init__.py
+-rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 cpct-0.2.1/cpct/base_types.py
+-rw-r--r--   0        0        0    24866 2020-02-02 00:00:00.000000 cpct-0.2.1/cpct/cpct.py
+-rwxr-xr-x   0        0        0      141 2020-02-02 00:00:00.000000 cpct-0.2.1/cpct/cpct_START_HERE.cmd
+-rwxr-xr-x   0        0        0      124 2020-02-02 00:00:00.000000 cpct-0.2.1/cpct/cpct_download.bat
+-rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 cpct-0.2.1/cpct/cpct_install_requirements.py
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 cpct-0.2.1/cpct/discord.py
+-rw-r--r--   0        0        0    30949 2020-02-02 00:00:00.000000 cpct-0.2.1/cpct/poepy.py
+-rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 cpct-0.2.1/cpct/user_info.py
+-rw-r--r--   0        0        0   329881 2020-02-02 00:00:00.000000 cpct-0.2.1/cpct/img/ChipyLogo.png
+-rw-r--r--   0        0        0  1621531 2020-02-02 00:00:00.000000 cpct-0.2.1/cpct/img/ChipyLogo.psd
+-rw-r--r--   0        0        0   329881 2020-02-02 00:00:00.000000 cpct-0.2.1/cpct/img/cpct_logo.png
+-rw-r--r--   0        0        0    31307 2020-02-02 00:00:00.000000 cpct-0.2.1/cpct/img/ctcp_gui.png
+-rw-r--r--   0        0        0     4116 2020-02-02 00:00:00.000000 cpct-0.2.1/cpct/img/dropper.png
+-rw-r--r--   0        0        0   678371 2020-02-02 00:00:00.000000 cpct-0.2.1/cpct/img/poe.png
+-rwxr-xr-x   0        0        0       84 2020-02-02 00:00:00.000000 cpct-0.2.1/cpct/qt/build_gui.bat
+-rw-r--r--   0        0        0    34674 2020-02-02 00:00:00.000000 cpct-0.2.1/cpct/qt/main_gui.py
+-rw-r--r--   0        0        0    36114 2020-02-02 00:00:00.000000 cpct-0.2.1/cpct/qt/main_gui.ui
+-rw-r--r--   0        0        0    20329 2020-02-02 00:00:00.000000 cpct-0.2.1/cpct/qt/stash_overlay.py
+-rw-r--r--   0        0        0    28379 2020-02-02 00:00:00.000000 cpct-0.2.1/cpct/qt/stash_overlay.ui
+-rw-r--r--   0        0        0     1975 2020-02-02 00:00:00.000000 cpct-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 cpct-0.2.1/LICENSE.txt
+-rw-r--r--   0        0        0     5350 2020-02-02 00:00:00.000000 cpct-0.2.1/README.md
+-rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 cpct-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     6346 2020-02-02 00:00:00.000000 cpct-0.2.1/PKG-INFO
```

### Comparing `cpct-0.1.9/cpct/base_types.py` & `cpct-0.2.1/cpct/base_types.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import requests
 
 # announce start
 print("Fetching basetype info . . .",end=" ")
 
 # base weapons names 
-WEAPON_LIST = ["Sword", "Axe", "Dagger", "Staff", "Bow", "Wand", "Mace"]
+WEAPON_LIST = ["Sword", "Axe", "Dagger", "Staff", "Bow", "Wand", "Mace", "Sceptre", "Claw"]
 ITEM_BASE_TYPES_URL = "https://raw.githubusercontent.com/brather1ng/RePoE/master/RePoE/data/base_items.json"
 
 # combind slots for all weapon types to have a single slot "weapons"
 def slot_sub(key,value):
     if any(item in value for item in WEAPON_LIST):
         value = "Weapon"
     return [key,value]
@@ -17,20 +17,27 @@
 # fetch basetypes
 r = requests.get(ITEM_BASE_TYPES_URL)
 base_type_dict = dict(json.loads(r.content))
 
 # concat into list of basetype&class
 BASE_TYPES = dict([[base_type_dict[base_type]["name"],base_type_dict[base_type]["item_class"]] for base_type in base_type_dict if base_type_dict[base_type]["domain"] == "item"])
 
-# build slot list
+# build slot lookup table
 SLOT_LOOKUP = dict([slot_sub(k,v) for k,v in BASE_TYPES.items()])
 
+# build slot list
+SLOT_LIST = {v[1] for v in SLOT_LOOKUP.items()}
+
 # TODO reduce excess string check by narrowing down this list 
-"""Body Armour"""
 WEAPON_CLASSES = [v for v in BASE_TYPES.items() if any(item in v for item in WEAPON_LIST)]
 
 print("done")
 
 if __name__ == "__main__":
     # print(SLOT_LOOKUP)
     # print(base_type_dict)
-    print(WEAPON_CLASSES)
+    print(BASE_TYPES)
+
+
+
+
+
```

### Comparing `cpct-0.1.9/cpct/cpct.py` & `cpct-0.2.1/cpct/cpct.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,75 +2,82 @@
 import datetime
 import os
 import sys
 import time
 import webbrowser
 from PyQt5.QtWidgets import QMainWindow, QFileDialog, QApplication, QColorDialog, QInputDialog, QWidget
 from PyQt5 import QtGui
-from PyQt5.QtCore import QTimer
+from PyQt5.QtCore import QTimer, Qt
 import qt.main_gui
 import ctypes
 import poepy
 import user_info
 from __about__ import __version__
 
 # PoE dev Docs for ref
 # https://www.pathofexile.com/developer/docs
 # TYPE/Structures
 # https://www.pathofexile.com/developer/docs/reference#type-Item
 
 # type checking block (AND RUFF INFO)
 # https://www.youtube.com/watch?v=bcAqceZkZRQ
 if typing.TYPE_CHECKING:
-    ...
+    api:poepy.PoeApiHandler
+    parser:poepy.DataParser
+    gui:qt.main_gui.MainWindow
 
 # set statics
+IMG_FOLDER = os.path.realpath(__file__)[:-7]+"img\\"
 ASYNC_INTERVAL_MS = 1000
 PROGRESS_BAR_STYLE = """
 QProgressBar {
 	text-align: center;
 	border-radius: 8px;
 }
 QProgressBar::chunk {
 	background-color: #05B8CC;
 	border-radius: 6px;
 }
 """
 
-api:poepy.PoeApiHandler
-parser:poepy.DataParser
-
 # variables for searching log files to detect new zone
 modified = 0
 async_time = time.time()
 previous = 0
+zone_log = []
+filter_updated = False
+slot_count = None
 refresh_off_cooldown = True
+recipe_handler = None
 
 class AsyncMainWindow(QMainWindow):
     log_timer = QTimer()
     def __init__(self):
         super().__init__()
         self.init_async()
 
     def init_async(self):
         print("Initializing . . . ", end="")
         self.log_timer.timeout.connect(async_two)
         self.log_timer.start(ASYNC_INTERVAL_MS)
         print("Started")
 
+def timestamp():
+    return time.strftime("%H:%M:%S")
+
 def try_wrapper(function):
     """Simple wrapper that includes a TRY loop
     Args:
         function (Func): Returns the provided function wrapped Try
     """
     def wrapper(*args, **kwargs):
         try:
             return function(*args, **kwargs)
         except Exception as e:
-            print(function.__name__, "=> FAILED:", e)
+            print(timestamp(), function.__name__, "=> FAILED:", e)
             return False
     return wrapper  
 
 def timed_try_wrapper(function):
     """Simple timing wrapper that also includes a TRY loop
     Args:
         function (Func): Returns the provided function wrapped with Time and Try
@@ -80,127 +87,124 @@
         try:
             result = function(*args, **kwargs)
             end = time.time()
             print(function.__name__, "=> RunTime:",end-start)
             return result
         except Exception as e:
             end = time.time()
-            print(function.__name__, "=> FAILED:",end-start, e)
+            print(timestamp(), function.__name__, "=> FAILED:",end-start, e)
             result = False
     return wrapper    
 
-def apply_ui_defaults():
-    global gui_main
+def apply_ui_defaults(gui_obj, window_obj, app_obj):
+
+    # set window Icons
+    app_obj.setWindowIcon(QtGui.QIcon(IMG_FOLDER+'cpct_logo.png'))
+    window_obj.setWindowTitle(f"Chipy's PoE Chaos Tool (v{__version__})")
+    
+    # set login icon (this is to fix the image path issue)
+    icon = QtGui.QIcon()
+    icon.addPixmap(QtGui.QPixmap(IMG_FOLDER+"poe.png"), QtGui.QIcon.Normal, QtGui.QIcon.Off)
+    gui_obj.login_link.setIcon(icon)
+    print(IMG_FOLDER+"dropper.png")
+    icon.addPixmap(QtGui.QPixmap(IMG_FOLDER+"dropper.png"), QtGui.QIcon.Normal, QtGui.QIcon.Off)
+    gui_obj.color_link_rings.setIcon(icon)
+    gui_obj.color_link_amulets.setIcon(icon)
+    gui_obj.color_link_belts.setIcon(icon)
+    gui_obj.color_link_bodies.setIcon(icon)
+    gui_obj.color_link_boots.setIcon(icon)
+    gui_obj.color_link_helmets.setIcon(icon)
+    gui_obj.color_link_weapons.setIcon(icon)
+    gui_obj.color_link_gloves.setIcon(icon)
 
     # set previous selections
-    gui_main.item_filter_browse.setText(os.path.split(user_info.get("form", "filter_name"))[1])
-    gui_main.client_secret_input.setText(user_info.get("api","client_secret"))
-    gui_main.client_path_browse.setText(user_info.get("form", "client_path")[0:22]+"..."+user_info.get("form", "client_path")[-13:])
-    gui_main.sets_target.setValue(int(user_info.get("form", "sets_goal")))
+    gui_obj.item_filter_browse.setText(os.path.split(user_info.get("form", "filter_name"))[1])
+    gui_obj.client_secret_input.setText(user_info.get("api","client_secret"))
+    gui_obj.client_path_browse.setText(user_info.get("form", "client_path")[0:22]+"..."+user_info.get("form", "client_path")[-13:])
+    gui_obj.sets_target.setValue(int(user_info.get("form", "sets_goal")))
 
     # set previous colours
-    gui_main.count_amulets.setStyleSheet(style_sheet_new_color(PROGRESS_BAR_STYLE, user_info.get("form", "color_amulets")))
-    gui_main.count_belts.setStyleSheet(style_sheet_new_color(PROGRESS_BAR_STYLE, user_info.get("form", "color_amulets")))
-    gui_main.count_bodies.setStyleSheet(style_sheet_new_color(PROGRESS_BAR_STYLE, user_info.get("form", "color_bodies")))
-    gui_main.count_boots.setStyleSheet(style_sheet_new_color(PROGRESS_BAR_STYLE, user_info.get("form", "color_boots")))
-    gui_main.count_gloves.setStyleSheet(style_sheet_new_color(PROGRESS_BAR_STYLE, user_info.get("form", "color_gloves")))
-    gui_main.count_helmets.setStyleSheet(style_sheet_new_color(PROGRESS_BAR_STYLE, user_info.get("form", "color_helmets")))
-    gui_main.count_rings.setStyleSheet(style_sheet_new_color(PROGRESS_BAR_STYLE, user_info.get("form", "color_rings")))
-    gui_main.count_weapons.setStyleSheet(style_sheet_new_color(PROGRESS_BAR_STYLE, user_info.get("form", "color_weapons")))
+    gui_obj.count_amulets.setStyleSheet(style_sheet_new_color(PROGRESS_BAR_STYLE, user_info.get("form", "color_amulet_rgba")))
+    gui_obj.count_belts.setStyleSheet(style_sheet_new_color(PROGRESS_BAR_STYLE, user_info.get("form", "color_belt_rgba")))
+    gui_obj.count_bodies.setStyleSheet(style_sheet_new_color(PROGRESS_BAR_STYLE, user_info.get("form", "color_body_armour_rgba")))
+    gui_obj.count_boots.setStyleSheet(style_sheet_new_color(PROGRESS_BAR_STYLE, user_info.get("form", "color_boots_rgba")))
+    gui_obj.count_gloves.setStyleSheet(style_sheet_new_color(PROGRESS_BAR_STYLE, user_info.get("form", "color_gloves_rgba")))
+    gui_obj.count_helmets.setStyleSheet(style_sheet_new_color(PROGRESS_BAR_STYLE, user_info.get("form", "color_helmet_rgba")))
+    gui_obj.count_rings.setStyleSheet(style_sheet_new_color(PROGRESS_BAR_STYLE, user_info.get("form", "color_ring_rgba")))
+    gui_obj.count_weapons.setStyleSheet(style_sheet_new_color(PROGRESS_BAR_STYLE, user_info.get("form", "color_weapon_rgba")))
 
     # defaults for item_filter modes
-    gui_main.filter_mode.addItems(["Default","FilterBlade","Custom","Disabled"])
+    gui_obj.filter_mode.addItems(["Default","FilterBlade","Custom","Disabled"])
     
-def apply_ui_connections():
+def apply_ui_connections(gui_obj, parser):
     """Overlay that connects up the GUI so that we can modularly replace the gui.py from QT5
     https://www.geeksforgeeks.org/function-wrappers-in-python/
     Args:
         gui_obj (gui.Ui_MainWindow): Main window GUI object
     """
-    global gui_main, MainWindow, parser
-
-    # set window Icons
-    app.setWindowIcon(QtGui.QIcon('./cpct/cpct/img/ChipyLogo.png'))
-    MainWindow.setWindowTitle(f"Chipy's PoE Chaos Tool (v{__version__})")
-    
-    # set login icon (this is to fix the image path issue)
-    icon = QtGui.QIcon()
-    icon.addPixmap(QtGui.QPixmap("./cpct/cpct/img/poe.png"), QtGui.QIcon.Normal, QtGui.QIcon.Off)
-    gui_main.login_link.setIcon(icon)
-    icon.addPixmap(QtGui.QPixmap("./cpct/cpct/img/dropper.png"), QtGui.QIcon.Normal, QtGui.QIcon.Off)
-    gui_main.color_link_rings.setIcon(icon)
-    gui_main.color_link_amulets.setIcon(icon)
-    gui_main.color_link_belts.setIcon(icon)
-    gui_main.color_link_bodies.setIcon(icon)
-    gui_main.color_link_boots.setIcon(icon)
-    gui_main.color_link_helmets.setIcon(icon)
-    gui_main.color_link_weapons.setIcon(icon)
-    gui_main.color_link_gloves.setIcon(icon)
-
     # Link ColorPickers
-    gui_main.color_link_amulets.clicked.connect(lambda: pick_color(gui_main, gui_main.count_amulets, "color_amulets"))
-    gui_main.color_link_belts.clicked.connect(lambda: pick_color(gui_main, gui_main.count_belts, "color_belts"))
-    gui_main.color_link_bodies.clicked.connect(lambda: pick_color(gui_main, gui_main.count_bodies, "color_bodies"))
-    gui_main.color_link_boots.clicked.connect(lambda: pick_color(gui_main, gui_main.count_boots, "color_boots"))
-    gui_main.color_link_gloves.clicked.connect(lambda: pick_color(gui_main, gui_main.count_gloves, "color_gloves"))
-    gui_main.color_link_helmets.clicked.connect(lambda: pick_color(gui_main, gui_main.count_helmets, "color_helmets"))
-    gui_main.color_link_rings.clicked.connect(lambda: pick_color(gui_main, gui_main.count_rings, "color_rings"))
-    gui_main.color_link_weapons.clicked.connect(lambda: pick_color(gui_main, gui_main.count_weapons, "color_weapons"))
+    gui_obj.color_link_amulets.clicked.connect(lambda: pick_color(gui_obj, gui_obj.count_amulets, "color_amulet_rgba"))
+    gui_obj.color_link_belts.clicked.connect(lambda: pick_color(gui_obj, gui_obj.count_belts, "color_belt_rgba"))
+    gui_obj.color_link_bodies.clicked.connect(lambda: pick_color(gui_obj, gui_obj.count_bodies, "color_body_armour_rgba"))
+    gui_obj.color_link_boots.clicked.connect(lambda: pick_color(gui_obj, gui_obj.count_boots, "color_boots_rgba"))
+    gui_obj.color_link_gloves.clicked.connect(lambda: pick_color(gui_obj, gui_obj.count_gloves, "color_gloves_rgba"))
+    gui_obj.color_link_helmets.clicked.connect(lambda: pick_color(gui_obj, gui_obj.count_helmets, "color_helmet_rgba"))
+    gui_obj.color_link_rings.clicked.connect(lambda: pick_color(gui_obj, gui_obj.count_rings, "color_ring_rgba"))
+    gui_obj.color_link_weapons.clicked.connect(lambda: pick_color(gui_obj, gui_obj.count_weapons, "color_weapon_rgba"))
 
     # # link menus
-    gui_main.actionChipy_dev.triggered.connect(lambda: webbrowser.open("www.chipy.dev/me.html"))
-    gui_main.actionGitHub.triggered.connect(lambda: webbrowser.open("https://github.com/iamchipy/chipys-pathofexile-chaos-tool/tree/main/cpct"))
-    gui_main.actionFilterblade_xyz.triggered.connect(lambda: webbrowser.open("https://www.filterblade.xyz/") )
-    gui_main.actionCraftOfExile_com.triggered.connect(lambda: webbrowser.open("https://www.craftofexile.com/en/") )
-    gui_main.actionMap_RegEx.triggered.connect(lambda: webbrowser.open("https://poe.re/#/maps") )
-    gui_main.actionPathOfBuilding_com.triggered.connect(lambda: webbrowser.open("https://pathofbuilding.community/") )
-    gui_main.actionPathOfExile_com.triggered.connect(lambda: webbrowser.open("https://www.pathofexile.com") )
-    gui_main.actionPoE_Lab.triggered.connect(lambda: webbrowser.open("https://www.poelab.com/") )
-    gui_main.actionPoE_Ninja.triggered.connect(lambda: webbrowser.open("https://www.poe.ninja") )
-    gui_main.actionVorici_Calculator.triggered.connect(lambda: webbrowser.open("https://siveran.github.io/calc.html") )
-    gui_main.actionAwakened_PoE_Trade.triggered.connect(lambda: webbrowser.open("https://github.com/SnosMe/awakened-poe-trade") )
-    gui_main.actionPatreon.triggered.connect(lambda: webbrowser.open("https://www.patreon.com/chipysPoEChaosTool") )
-    gui_main.actionInput_ClientSecret.triggered.connect(lambda: request_client_secret() )
+    gui_obj.actionChipy_dev.triggered.connect(lambda: webbrowser.open("www.chipy.dev/me.html"))
+    gui_obj.actionGitHub.triggered.connect(lambda: webbrowser.open("https://github.com/iamchipy/chipys-pathofexile-chaos-tool/tree/main/cpct"))
+    gui_obj.actionFilterblade_xyz.triggered.connect(lambda: webbrowser.open("https://www.filterblade.xyz/") )
+    gui_obj.actionCraftOfExile_com.triggered.connect(lambda: webbrowser.open("https://www.craftofexile.com/en/") )
+    gui_obj.actionMap_RegEx.triggered.connect(lambda: webbrowser.open("https://poe.re/#/maps") )
+    gui_obj.actionPathOfBuilding_com.triggered.connect(lambda: webbrowser.open("https://pathofbuilding.community/") )
+    gui_obj.actionPathOfExile_com.triggered.connect(lambda: webbrowser.open("https://www.pathofexile.com") )
+    gui_obj.actionPoE_Lab.triggered.connect(lambda: webbrowser.open("https://www.poelab.com/") )
+    gui_obj.actionPoE_Ninja.triggered.connect(lambda: webbrowser.open("https://www.poe.ninja") )
+    gui_obj.actionVorici_Calculator.triggered.connect(lambda: webbrowser.open("https://siveran.github.io/calc.html") )
+    gui_obj.actionAwakened_PoE_Trade.triggered.connect(lambda: webbrowser.open("https://github.com/SnosMe/awakened-poe-trade") )
+    gui_obj.actionPatreon.triggered.connect(lambda: webbrowser.open("https://www.patreon.com/chipysPoEChaosTool") )
+    gui_obj.actionInput_ClientSecret.triggered.connect(lambda: request_client_secret() )
+    gui_obj.actiondev_button.triggered.connect(lambda: dev_button(gui_obj, parser) )
     
     #ClientSecrect Menu
-    # gui_main.actionInput_ClientSecret.triggered.connect(lambda: receive_client_secret(gui_main) )
+    # gui_obj.actionInput_ClientSecret.triggered.connect(lambda: receive_client_secret(gui_obj) )
 
     # # link buttons
-    gui_main.login_link.clicked.connect(lambda: action_login_link(gui_main))
-    gui_main.refresh_link.clicked.connect(lambda: count_unid_rares(gui_main, True))
-    gui_main.item_filter_browse.clicked.connect(lambda: browser_item_filters(gui_main))
-    gui_main.client_path_browse.clicked.connect(lambda: browser_client_folder(gui_main))
+    gui_obj.login_link.clicked.connect(lambda: action_login_link(gui_obj, parser))
+    gui_obj.refresh_link.clicked.connect(lambda: update_item_filter(gui_obj, parser, True))
+    gui_obj.item_filter_browse.clicked.connect(lambda: browser_item_filters(gui_obj))
+    gui_obj.client_path_browse.clicked.connect(lambda: browser_client_folder(gui_obj))
 
     # Link ComboBoxes
-    gui_main.select_league.currentIndexChanged.connect(lambda: action_set_league(gui_main))
-    gui_main.select_tab.currentIndexChanged.connect(lambda: action_set_tab(gui_main))
-    gui_main.filter_mode.currentIndexChanged.connect(lambda: update_item_filter(gui_main))
-    gui_main.sets_target.valueChanged.connect(lambda: change_target_count(gui_main))
+    gui_obj.select_league.activated.connect(lambda: action_set_league(gui_obj, parser))
+    # gui_obj.select_league.currentIndexChanged.connect(lambda: action_set_league(gui_obj))
+    gui_obj.select_tab.activated.connect(lambda: action_set_tab(gui_obj))
+    gui_obj.filter_mode.activated.connect(lambda: update_item_filter(gui_obj, parser))
+    gui_obj.sets_target.valueChanged.connect(lambda: change_target_count(gui_obj))
 
     # Link Text
-    gui_main.client_secret_input.textChanged.connect(lambda: receive_client_secret(gui_main))
+    gui_obj.client_secret_input.textChanged.connect(lambda: receive_client_secret(gui_obj))
 
 @timed_try_wrapper
-def action_login_link(gui):
-    global api, parser, gui_main
-    api = poepy.PoeApiHandler(client_id=user_info.cfg["api"]["CLIENT_ID"],
-                                    client_secret=user_info.cfg["api"]["CLIENT_SECRET"],
-                                    scope=user_info.cfg["api"]["SCOPE"],
-                                    uri=user_info.cfg["api"]["REDIRECT_URI"],
-                                    manual_token=user_info.cfg["api"]["TOKEN"]
-                                    )
-    parser = poepy.DataParser(api_handler = api)
+def action_login_link(gui, parser):
+    parser.connect( client_id=user_info.cfg["api"]["CLIENT_ID"],
+                    client_secret=user_info.cfg["api"]["CLIENT_SECRET"],
+                    scope=user_info.cfg["api"]["SCOPE"],
+                    uri=user_info.cfg["api"]["REDIRECT_URI"],
+                    manual_token=user_info.cfg["api"]["TOKEN"]
+                    )
 
     # save any token changes
-    user_info.set("api","TOKEN", api.token)
+    user_info.set("api","TOKEN", parser.api_handler.token)
     user_info.set("form","username", parser.get_username())
     # gui_main.client_secret_input.isEnabled = False
     gui_main.client_secret_input.setEnabled(False)
 
-
     # set login name
     gui.login_link.setText(user_info.get("form","username"))
     gui.login_link.setDisabled(True)
     gui.select_league.setCurrentText( user_info.get("form","league"))
     gui.select_tab.setCurrentText( user_info.get("form","tab"))
 
     # continue the loading chain
@@ -215,100 +219,121 @@
     leagues = parser.get_leagues()
 
     # clear the box and repop
     gui.select_league.clear()
     gui.select_tab.clear()
     gui.select_league.addItems(leagues)
 
-    # set previous league
-    gui_main.select_league.setCurrentText(user_info.get("form","league"))
+    # load previous league
+    gui.select_league.setCurrentText(user_info.get("form","league"))
     
 @timed_try_wrapper
-def action_set_league(gui):
+def action_set_league(gui, parser):
     # load current selection for league
     league = gui.select_league.currentText()
-    # print("League:",league)
-    if league != "":
-        try:
-            previous = user_info.get("form", "league")
-            # print("previous:",previous)
-            action_load_tabs(gui, previous)
-        except Exception as e:
-            print("action_set_league::>",e)
-            user_info.set("form", "league",gui.select_league.currentText()) 
-            action_load_tabs(gui, league)
+
+    # try pull the league
+    action_load_tabs(gui, league, parser)
+
+    # now save changes 
+    user_info.set("form", "league",gui.select_league.currentText()) 
 
 @timed_try_wrapper
-def action_load_tabs(gui, league):
-    global parser, gui_main
+def action_load_tabs(gui, league, parser):
     tabs = parser.get_tab_names(league).keys()
+
     # clear the box and repop
     gui.select_tab.clear()
     gui.select_tab.addItems(tabs)
-    
+
+    # select previous tab
+    gui.select_tab.setCurrentText(user_info.get("form","tab"))    
+
 @timed_try_wrapper
 def action_set_tab(gui, force_recache:bool=False):
-    global parser, gui_main
     user_info.set("form", "tab", gui.select_tab.currentText())
   
-@timed_try_wrapper
-def count_unid_rares(gui, force_recache:bool=False)->list[list, int]:
-    global refresh_off_cooldown, parser
+def count_unid_rares(gui, parser, force_recache:bool=False, min_ilvl:int=60)->dict:
+    """Function to count unidentified rare items of ilevel
+
+    Args:
+        gui (_type_): gui object used for display and update
+        force_recache (bool, optional): force a fresh fetch for POE. Defaults to False.
+
+    Returns:
+        dict: returns list of count %s (0-100)
+    """
+    # TODO REMOVE GLOBAL REFERENCE 
+    global refresh_off_cooldown, recipe_handler
     league_of_interest = gui.select_league.currentText()
 
     # put the manual refresh button on cooldown
     refresh_off_cooldown = False
     gui_main.refresh_link.setEnabled(refresh_off_cooldown)
 
-    # TODO Auto filter reload "/itemfilter 0PKKgH0"
-
     try:
         # tab_of_interes
-        tabs_of_interest = poepy.validate_tab(parser, league_of_interest, gui.select_tab.currentText())
-        print("tabs_of_interest>",type(tabs_of_interest))
+        tab_of_interest = poepy.validate_tab(parser, league_of_interest, gui.select_tab.currentText())
+        print("tab_of_interest>",type(tab_of_interest))
 
         # list of items
-        items_of_interest = parser.get_items(tabs_of_interest, league_of_interest, force_recache)
-        print("items_of_interest>",type(items_of_interest))
+        items_of_interest = parser.get_items(tab_of_interest, league_of_interest, force_recache)
+        # print("items_of_interest>",type(items_of_interest))
 
         # filter for unid
         items_unidentified = parser.filter_identified(items_of_interest)
-        print("items_unidentified>",items_unidentified)
+        # print("items_unidentified>",items_unidentified)
 
         # filter for ilevel
-        items_unidentified_ilvl = parser.filter_ilvl(items_unidentified)
-        print("items_unidentified_ilvl>",items_unidentified_ilvl)
+        items_unidentified_ilvl = parser.filter_ilvl(items_unidentified,min_ilvl)
+        # print("items_unidentified_ilvl>",items_unidentified_ilvl)
 
         # filter for rares
         items_unidentified_ilvl_rare = parser.filter_rarity(items_unidentified_ilvl, rarity="rare")
-        print("items_unidentified_ilvl_rare>",items_unidentified_ilvl_rare)
+        # print("items_unidentified_ilvl_rare>",items_unidentified_ilvl_rare)
         
+        # load recipes
+        recipe_handler = poepy.RecipeHandler(items_of_interest)
+        assert isinstance(recipe_handler,poepy.RecipeHandler)
+        #TODO replace slot_counter with RecipeHandler
+
         # loop and count unids
         count = poepy.count_slots(parser, items_unidentified_ilvl_rare)
         # gui_main.count_report_string.setText(f"Count Total: {count['Total']}")
 
         # Set scales and mutlipliers
         target = gui.sets_target.value()
-        multiplier = 100//target
+        multiplier = 100/target
+
+        # convert counts to %
+        count["Weapon"] = round(min(100,(count["Weapon"]*multiplier)//2))
+        count["Ring"] = round(min(100,(count["Ring"]*multiplier)//2))
+        
+        count["Helmet"] = round(min(100,count["Helmet"]*multiplier))
+        count["Body Armour"] = round(min(100,count["Body Armour"]*multiplier))
+        count["Boots"] = round(min(100,count["Boots"]*multiplier))
+        count["Gloves"] = round(min(100,count["Gloves"]*multiplier))
+        count["Belt"] = round(min(100,count["Belt"]*multiplier))
+        count["Amulet"] = round(min(100,count["Amulet"]*multiplier))
+        
 
         # set GUI element values
-        gui_main.count_weapons.setValue(count["Weapon"]*multiplier)
-        gui_main.count_helmets.setValue(count["Helmet"]*multiplier)
-        gui_main.count_bodies.setValue(count["Body Armor"]*multiplier)
-        gui_main.count_boots.setValue(count["Boot"]*multiplier)
-        gui_main.count_gloves.setValue(count["Glove"]*multiplier)
-        gui_main.count_belts.setValue(count["Belt"]*multiplier)
-        gui_main.count_amulets.setValue(count["Amulet"]*multiplier)
-        gui_main.count_rings.setValue((count["Ring"]*multiplier)//2)
+        gui_main.count_weapons.setValue(count["Weapon"])
+        gui_main.count_helmets.setValue(count["Helmet"])
+        gui_main.count_bodies.setValue(count["Body Armour"])
+        gui_main.count_boots.setValue(count["Boots"])
+        gui_main.count_gloves.setValue(count["Gloves"])
+        gui_main.count_belts.setValue(count["Belt"])
+        gui_main.count_amulets.setValue(count["Amulet"])
+        gui_main.count_rings.setValue(count["Ring"])
         
         # report
-        return [count, target]
+        return count
     except Exception as e:
-        t = str(time.time())[-1:]
-        gui.count_report_string.setText("ERR:"+str(e)+f"[{t}]")
+        print(timestamp(),"count_unid_rares() Error:"+str(e))
         return [False, False]
 
 def async_two():
     global refresh_off_cooldown, gui_main, async_time
     elapsed = time.time() - async_time
     # Entry point to secondary exec chain
     log_search()
@@ -319,33 +344,37 @@
     if elapsed > 10:
         async_time = time.time()
 
 @try_wrapper
 def log_search():
     """Checks the ClientLog for a maching zone change with timestamp in the current minute
     """
-    global modified, previous, gui_main, parser
+    global modified, previous, gui_main, parser, zone_log, filter_updated
     # 2023/03/30 09:11     
     # 2023/03/30 09:26:41 1117798968 cffb0734 [INFO Client 31504] : You have entered Aspirants' Plaza.     
     snippet = " : You have entered"
     path = user_info.get("form","client_path") + "\logs\Client.txt"
     if not os.path.exists(path):
         return False
     modified = os.path.getmtime(path)
     if modified > previous:
         previous = modified
         # print("Last modified: %s" % time.ctime(modified))
         # gui_main.count_report_string.setText("Reading...")
         stamp = datetime.datetime.now().strftime("%Y/%m/%d %H:%M")
+        # TODO rebuild this to always look only at X recent lines for speed
+
         with open(path, "r", encoding="utf-8") as file:
             for line in file:
-                if stamp in line and snippet in line:
+                if stamp in line and snippet in line and line not in zone_log:
                         print(line)
+                        filter_updated = False
+                        zone_log.append(line)
                         gui_main.count_report_string.setText(line[78:])
-                        count_unid_rares(gui_main)
+                        update_item_filter(gui_main, parser, force_recache=True)
                         return
         # gui_main.count_report_string.setText("Reading... Done")
 
 @timed_try_wrapper
 def browser_item_filters(gui):
     global MainWindow, gui_main
     #C:\Users\chipy\Documents\My Games\Path of Exile\
@@ -369,40 +398,71 @@
     
 def receive_client_secret(gui):
     global gui_main
     user_info.set("api","client_secret",gui_main.client_secret_input.text())
 
 @timed_try_wrapper
 def pick_color(gui, target_object, save_name):
-    current_color = QtGui.QColor(user_info.get("form", save_name))
+    rgba = user_info.get("form", save_name)
+    print(type(rgba),rgba)
+    current_color = QtGui.QColor(int(rgba[0]),int(rgba[1]),int(rgba[2]),int(rgba[3]))
     new_color = QColorDialog.getColor(current_color, title=f"Pick a new color for {save_name}")
     if new_color.isValid():
-        user_info.set("form", save_name, new_color.name())
-        user_info.set("form", save_name+"_rgb", str(list(new_color.getRgb())))
-        target_object.setStyleSheet(style_sheet_new_color(PROGRESS_BAR_STYLE,new_color.name()))
-        update_item_filter(gui)
-
-def style_sheet_new_color(base_style:str,new_color:str) -> str:
+        new_rgba = list(new_color.getRgb())
+        user_info.set("form", save_name, str(new_rgba))
+        target_object.setStyleSheet(style_sheet_new_color(PROGRESS_BAR_STYLE,new_rgba))
+        print(type(new_rgba),new_rgba)
+
+def style_sheet_new_color(base_style:str,new_rgba_color:list) -> str:
+    def rgba_t0_hex(rgba:list) -> str:
+        r = hex(int(rgba[0]))[2:] 
+        g = hex(int(rgba[1]))[2:]
+        b = hex(int(rgba[2]))[2:]
+        return f"#{r.zfill(2)}{g.zfill(2)}{b.zfill(2)}"
     return_string = ""
+    new_hex_color = rgba_t0_hex(new_rgba_color)
     i = base_style.find("background-color: ")
     current_color = base_style[i+18:i+25]
-    return_string = base_style.replace(current_color, new_color) 
+    return_string = base_style.replace(current_color, new_hex_color) 
     return return_string
 
 @timed_try_wrapper
-def update_item_filter(gui):
-    global gui_main
+def update_item_filter(gui, parser, force_recache:bool=False, always_show_rings:bool=True, always_show_amulets:bool=True):
+    global gui_main, filter_updated, slot_count
     header = poepy.ITEM_FILTER_TITLE_START
     footer = poepy.ITEM_FILTER_TITLE_END
     path = user_info.cfg.get("form","filter_name")
     mode = gui_main.filter_mode.currentText()
-    slot_count, target = count_unid_rares(gui)
+    target = 100  # 100% of the goal
+    slot_count_percent = count_unid_rares(gui, parser, force_recache)
+
+    if mode == "Disabled":
+        return
+
+    # assert isinstance(slot_count_percent, dict)  # If this isn't a dict something didn't pull right from tabs
+    if not isinstance(slot_count_percent, dict):
+        return False
+
+    # check if filter needs changing
+    for key, value in slot_count_percent.items():
+        # skip totals
+        if key == "Total":
+            continue
+        if value > 99 and isinstance(slot_count,dict) and slot_count[key] < 100:
+            filter_updated = True
+            break
+    slot_count = slot_count_percent
+
+    # exit case if we don't have a parser object yet
+    if not parser or not isinstance(parser, poepy.DataParser):
+        return False
 
     # exit case for when counts could not be found
-    if not slot_count:
+    if not slot_count_percent:
+        print(f"Failed to recieve item counts [slot_count = {slot_count_percent}]")
         return False
 
     # read data without mod section
     current_filter = ""
     is_section_to_replace=False
     with open(path, "r") as f:
         for line in f:
@@ -412,37 +472,48 @@
                 is_section_to_replace = False
             if not is_section_to_replace and footer not in line:
                 current_filter += line
 
     # rebuild filter text adding back in slots as needed   
     prefix = header
     if "Disabled" not in mode:
-        print(slot_count)
-        if slot_count["Weapon"] >= target:
-            prefix += poepy.ItemFilterEntry("Weapon",user_info.cfg.get("form","color_weapons_rgb"),width="= 1").to_str()
-        if slot_count["Helmet"] >= target:
-            prefix += poepy.ItemFilterEntry("Helmet",user_info.cfg.get("form","color_helmets_rgb")).to_str()
-        if slot_count["Body Armor"] >= target:
-            prefix += poepy.ItemFilterEntry("Body Armour",user_info.cfg.get("form","color_bodies_rgb")).to_str()   
-        if slot_count["Boot"] >= target:
-            prefix += poepy.ItemFilterEntry("Boot",user_info.cfg.get("form","color_boots_rgb")).to_str()
-        if slot_count["Glove"] >= target:
-            prefix += poepy.ItemFilterEntry("Glove",user_info.cfg.get("form","color_gloves_rgb")).to_str()
-        if slot_count["Amulet"] >= target:
-            prefix += poepy.ItemFilterEntry("Amulet",user_info.cfg.get("form","color_amulets_rgb")).to_str()
-        if slot_count["Ring"] >= target:
-            prefix += poepy.ItemFilterEntry("Ring",user_info.cfg.get("form","color_rings_rgb")).to_str()
+        print(slot_count_percent)
+        if slot_count_percent["Weapon"] < target:
+            prefix += poepy.ItemFilterEntry("Weapon",user_info.cfg.get("form","color_weapon_rgba"),width="= 1").to_str()
+        if slot_count_percent["Helmet"] < target:
+            prefix += poepy.ItemFilterEntry("Helmet",user_info.cfg.get("form","color_helmet_rgba")).to_str()
+        if slot_count_percent["Body Armour"] < target:
+            prefix += poepy.ItemFilterEntry("Body Armour",user_info.cfg.get("form","color_body_armour_rgba")).to_str()   
+        if slot_count_percent["Boots"] < target:
+            prefix += poepy.ItemFilterEntry("Boots",user_info.cfg.get("form","color_boots_rgba")).to_str()
+        if slot_count_percent["Gloves"] < target:
+            prefix += poepy.ItemFilterEntry("Gloves",user_info.cfg.get("form","color_gloves_rgba")).to_str()
+        if slot_count_percent["Belt"] < target:
+            prefix += poepy.ItemFilterEntry("Belt",user_info.cfg.get("form","color_belt_rgba")).to_str()          
+        if always_show_amulets or slot_count_percent["Amulet"] < target:
+            prefix += poepy.ItemFilterEntry("Amulet",user_info.cfg.get("form","color_amulet_rgba")).to_str()          
+        if always_show_rings or slot_count_percent["Ring"] < target:
+            prefix += poepy.ItemFilterEntry("Ring",user_info.cfg.get("form","color_ring_rgba")).to_str()
     prefix += footer
 
     # write
     with open(path, "w") as f:
         f.write(prefix+current_filter)
     
     # announce update
-    gui_main.count_report_string.setText("Filter updated . . .")
+    t = timestamp()
+    n =  os.path.split(path)[1]
+    txt = f"{t} '{n}' updated!"
+    print(txt)
+    gui_main.count_report_string.setText(txt)
+
+    if filter_updated:
+        filter_name = str(os.path.split(user_info.get("form", "filter_name"))[1]).split(".")[0]
+        path = user_info.get("form","client_path")
+        poepy.poe_chat(f"/itemfilter {filter_name}", f"{path}\PathOfExile.exe")
             
 @timed_try_wrapper
 def request_client_secret():
     global gui_main
     promt_obj = QWidget()
     discord_name, ok = QInputDialog.getText(promt_obj, 'Send Discord Request?', 'Please provide the Discord name (including full "name#1234") to send the secret to')
     if ok:
@@ -452,31 +523,43 @@
             gui_main.count_report_string.setText('Request has been send please look out for a friend request on Discord')
             # QInputDialog.getText(promt_obj, 'Request Sent', 'Request has been send please look out for a friend request on Discord')
 
 @timed_try_wrapper
 def change_target_count(gui):
     user_info.set("form","sets_goal", str(gui.sets_target.value()))
 
-if __name__ == "__main__":
-    # load user file
-    user_info.load()
+def dev_button(gui:qt.main_gui.Ui_MainWindow, parser:poepy.DataParser):
+    global recipe_handler
+    recipe_handler.click_items_in_stash(sleep_sec=.01)
 
+if __name__ == "__main__":
     # required for Windows to recognize a Python script as it's own applications and thus have a unique Taskbar Icon
     # https://stackoverflow.com/questions/1551605/how-to-set-applications-taskbar-icon-in-windows-7/1552105#1552105
     myappid = u'chipy.PoE.chaos.tool' # arbitrary string
     ctypes.windll.shell32.SetCurrentProcessExplicitAppUserModelID(myappid)
 
+    # load user file
+    user_info.load()
+
+    # build the api/parser object
+    api = poepy.PoeApiHandler()
+    parser = poepy.DataParser(api_handler = api)
+
     # build main GUI
     app = QApplication(sys.argv)
     app.setStyle('Fusion')
     MainWindow = AsyncMainWindow()
     MainWindow.show()
     gui_main = qt.main_gui.Ui_MainWindow()
     gui_main.setupUi(MainWindow)
 
+    # MainWindow.setWindowFlags(MainWindow.windowFlags() | Qt.WindowStaysOnTopHint)
+    # MainWindow.setAttribute(Qt.WA_TranslucentBackground)
+    # MainWindow.setWindowFlags(Qt.FramelessWindowHint)
+
     # Modify the gui with connections and links
-    apply_ui_connections()  # here we modify actions to the GUI
-    apply_ui_defaults()  # set default values for the form when it's made
+    apply_ui_connections(gui_main, parser)  # here we modify actions to the GUI
+    apply_ui_defaults(gui_main, MainWindow, app)  # set default values for the form when it's made
 
     # run app as the last thing in the script
     sys.exit(app.exec_())
```

### Comparing `cpct-0.1.9/cpct/cpct_install_requirements.py` & `cpct-0.2.1/cpct/cpct_install_requirements.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import subprocess
 
 SCRIPT_NAME = "Chipy's PathOfExile Chaos Tool"
 installDependencyErrors = 0
 installDependencyMessage = ""
 
 # List of packages to install with pip
-dependenciesInstall = ["requests","PyQt5", "websockets"]
+dependenciesInstall = ["requests","PyQt5", "websockets", "pywinauto", "pyautogui", "psutil"]
 
 # List of packages to update with pip
 dependenciesUpdate = ["PyQt5"]
 
 # Make sure pip is updated
 print("Checking pip is updated...")
 try:
```

### Comparing `cpct-0.1.9/cpct/img/ChipyLogo.png` & `cpct-0.2.1/cpct/img/ChipyLogo.png`

 * *Files identical despite different names*

### Comparing `cpct-0.1.9/cpct/img/ChipyLogo.psd` & `cpct-0.2.1/cpct/img/ChipyLogo.psd`

 * *Files identical despite different names*

### Comparing `cpct-0.1.9/cpct/img/cpct_logo.png` & `cpct-0.2.1/cpct/img/cpct_logo.png`

 * *Files identical despite different names*

### Comparing `cpct-0.1.9/cpct/img/ctcp_gui.png` & `cpct-0.2.1/cpct/img/ctcp_gui.png`

 * *Files identical despite different names*

### Comparing `cpct-0.1.9/cpct/img/dropper.png` & `cpct-0.2.1/cpct/img/dropper.png`

 * *Files identical despite different names*

### Comparing `cpct-0.1.9/cpct/img/poe.png` & `cpct-0.2.1/cpct/img/poe.png`

 * *Files identical despite different names*

### Comparing `cpct-0.1.9/cpct/qt/main_gui.py` & `cpct-0.2.1/cpct/qt/main_gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -219,14 +219,15 @@
         self.count_rings.setObjectName("count_rings")
         self.sets_target = QtWidgets.QSpinBox(self.centralwidget)
         self.sets_target.setGeometry(QtCore.QRect(280, 230, 51, 22))
         font = QtGui.QFont()
         font.setFamily("Roboto")
         font.setPointSize(12)
         self.sets_target.setFont(font)
+        self.sets_target.setMinimum(2)
         self.sets_target.setProperty("value", 8)
         self.sets_target.setObjectName("sets_target")
         self.label_11 = QtWidgets.QLabel(self.centralwidget)
         self.label_11.setGeometry(QtCore.QRect(200, 230, 71, 21))
         font = QtGui.QFont()
         font.setFamily("Roboto")
         font.setPointSize(12)
@@ -252,35 +253,35 @@
         self.filter_mode.setGeometry(QtCore.QRect(110, 200, 221, 22))
         font = QtGui.QFont()
         font.setFamily("Roboto")
         font.setPointSize(12)
         self.filter_mode.setFont(font)
         self.filter_mode.setObjectName("filter_mode")
         self.item_2 = QtWidgets.QLabel(self.centralwidget)
-        self.item_2.setEnabled(False)
+        self.item_2.setEnabled(True)
         self.item_2.setGeometry(QtCore.QRect(10, 230, 111, 21))
         font = QtGui.QFont()
         font.setFamily("Roboto")
         font.setPointSize(12)
         self.item_2.setFont(font)
         self.item_2.setObjectName("item_2")
         self.recipe_chaos = QtWidgets.QRadioButton(self.centralwidget)
-        self.recipe_chaos.setEnabled(False)
+        self.recipe_chaos.setEnabled(True)
         self.recipe_chaos.setGeometry(QtCore.QRect(70, 230, 91, 17))
         font = QtGui.QFont()
         font.setFamily("Roboto")
         font.setPointSize(10)
         self.recipe_chaos.setFont(font)
         self.recipe_chaos.setChecked(True)
         self.recipe_chaos.setObjectName("recipe_chaos")
         self.recipe_type = QtWidgets.QButtonGroup(MainWindow)
         self.recipe_type.setObjectName("recipe_type")
         self.recipe_type.addButton(self.recipe_chaos)
         self.recipe_regal = QtWidgets.QRadioButton(self.centralwidget)
-        self.recipe_regal.setEnabled(False)
+        self.recipe_regal.setEnabled(True)
         self.recipe_regal.setGeometry(QtCore.QRect(70, 250, 91, 17))
         font = QtGui.QFont()
         font.setFamily("Roboto")
         font.setPointSize(10)
         self.recipe_regal.setFont(font)
         self.recipe_regal.setObjectName("recipe_regal")
         self.recipe_type.addButton(self.recipe_regal)
@@ -489,28 +490,45 @@
         self.color_link_weapons.setFocusPolicy(QtCore.Qt.StrongFocus)
         self.color_link_weapons.setLayoutDirection(QtCore.Qt.LeftToRight)
         self.color_link_weapons.setAutoFillBackground(False)
         self.color_link_weapons.setIcon(icon1)
         self.color_link_weapons.setIconSize(QtCore.QSize(20, 20))
         self.color_link_weapons.setAutoRepeatDelay(1000)
         self.color_link_weapons.setObjectName("color_link_weapons")
+        self.label_12 = QtWidgets.QLabel(self.centralwidget)
+        self.label_12.setGeometry(QtCore.QRect(200, 250, 71, 21))
+        font = QtGui.QFont()
+        font.setFamily("Roboto")
+        font.setPointSize(12)
+        self.label_12.setFont(font)
+        self.label_12.setObjectName("label_12")
+        self.set_delay = QtWidgets.QDoubleSpinBox(self.centralwidget)
+        self.set_delay.setGeometry(QtCore.QRect(270, 250, 61, 22))
+        font = QtGui.QFont()
+        font.setPointSize(12)
+        self.set_delay.setFont(font)
+        self.set_delay.setMinimum(0.01)
+        self.set_delay.setMaximum(9.99)
+        self.set_delay.setSingleStep(0.01)
+        self.set_delay.setProperty("value", 0.04)
+        self.set_delay.setObjectName("set_delay")
         MainWindow.setCentralWidget(self.centralwidget)
+        self.statusbar = QtWidgets.QStatusBar(MainWindow)
+        self.statusbar.setObjectName("statusbar")
+        MainWindow.setStatusBar(self.statusbar)
         self.menubar = QtWidgets.QMenuBar(MainWindow)
         self.menubar.setGeometry(QtCore.QRect(0, 0, 717, 21))
         self.menubar.setObjectName("menubar")
         self.menuLinks = QtWidgets.QMenu(self.menubar)
         self.menuLinks.setObjectName("menuLinks")
         self.menuSettings = QtWidgets.QMenu(self.menubar)
         self.menuSettings.setObjectName("menuSettings")
         self.menuAbout = QtWidgets.QMenu(self.menubar)
         self.menuAbout.setObjectName("menuAbout")
         MainWindow.setMenuBar(self.menubar)
-        self.statusbar = QtWidgets.QStatusBar(MainWindow)
-        self.statusbar.setObjectName("statusbar")
-        MainWindow.setStatusBar(self.statusbar)
         self.actionFilterblade_xyz = QtWidgets.QAction(MainWindow)
         self.actionFilterblade_xyz.setObjectName("actionFilterblade_xyz")
         self.actionChipy_dev = QtWidgets.QAction(MainWindow)
         self.actionChipy_dev.setObjectName("actionChipy_dev")
         self.actionPathOfExile_com = QtWidgets.QAction(MainWindow)
         self.actionPathOfExile_com.setObjectName("actionPathOfExile_com")
         self.actionPathOfBuilding_com = QtWidgets.QAction(MainWindow)
@@ -532,26 +550,29 @@
         self.actionInput_ClientSecret.setObjectName("actionInput_ClientSecret")
         self.actionGitHub = QtWidgets.QAction(MainWindow)
         self.actionGitHub.setObjectName("actionGitHub")
         self.actionPatreon = QtWidgets.QAction(MainWindow)
         self.actionPatreon.setObjectName("actionPatreon")
         self.action_NOT_AFFILIATED_WITH_ANY = QtWidgets.QAction(MainWindow)
         self.action_NOT_AFFILIATED_WITH_ANY.setObjectName("action_NOT_AFFILIATED_WITH_ANY")
+        self.actiondev_button = QtWidgets.QAction(MainWindow)
+        self.actiondev_button.setObjectName("actiondev_button")
         self.menuLinks.addAction(self.action_NOT_AFFILIATED_WITH_ANY)
         self.menuLinks.addSeparator()
         self.menuLinks.addAction(self.actionPathOfExile_com)
         self.menuLinks.addAction(self.actionPathOfBuilding_com)
         self.menuLinks.addAction(self.actionCraftOfExile_com)
         self.menuLinks.addAction(self.actionFilterblade_xyz)
         self.menuLinks.addAction(self.actionMap_RegEx)
         self.menuLinks.addAction(self.actionVorici_Calculator)
         self.menuLinks.addAction(self.actionPoE_Ninja)
         self.menuLinks.addAction(self.actionPoE_Lab)
         self.menuLinks.addAction(self.actionAwakened_PoE_Trade)
         self.menuSettings.addAction(self.actionInput_ClientSecret)
+        self.menuSettings.addAction(self.actiondev_button)
         self.menuAbout.addAction(self.actionChipy_dev)
         self.menuAbout.addAction(self.actionGitHub)
         self.menuAbout.addAction(self.actionPatreon)
         self.menubar.addAction(self.menuSettings.menuAction())
         self.menubar.addAction(self.menuLinks.menuAction())
         self.menubar.addAction(self.menuAbout.menuAction())
 
@@ -573,15 +594,15 @@
         self.item_.setText(_translate("MainWindow", "Item Fitler:"))
         self.item_1.setText(_translate("MainWindow", "Filter Mode:"))
         self.filter_mode.setStatusTip(_translate("MainWindow", "How to interact with filter (Disabled to leave filters alone)"))
         self.item_2.setText(_translate("MainWindow", "Recipe:"))
         self.recipe_chaos.setStatusTip(_translate("MainWindow", "Chaos Recipe: Unidentified set of all items iLevel +60"))
         self.recipe_chaos.setText(_translate("MainWindow", "Chaos (i60+)"))
         self.recipe_regal.setStatusTip(_translate("MainWindow", "Regal Recipe: Unidentified set of all items iLevel +70"))
-        self.recipe_regal.setText(_translate("MainWindow", "Regal (i70+)"))
+        self.recipe_regal.setText(_translate("MainWindow", "Regal (i75+)"))
         self.item_filter_browse.setStatusTip(_translate("MainWindow", "Select the item filter you use or what to modify for Chaos Recipe"))
         self.item_filter_browse.setText(_translate("MainWindow", "Browse"))
         self.client_secret_input.setStatusTip(_translate("MainWindow", "Your client secret, never share this!"))
         self.label_13.setText(_translate("MainWindow", "SECRET:"))
         self.client_path_browse.setStatusTip(_translate("MainWindow", "Browse to your \'Path of Exile\' folder install location"))
         self.client_path_browse.setText(_translate("MainWindow", "Browse"))
         self.item_3.setText(_translate("MainWindow", "PoE Folder:"))
@@ -597,14 +618,15 @@
         self.color_link_helmets.setText(_translate("MainWindow", "Helmets"))
         self.color_link_bodies.setStatusTip(_translate("MainWindow", "Select the base background color to use in itemFilter"))
         self.color_link_bodies.setText(_translate("MainWindow", "Bodies"))
         self.color_link_boots.setStatusTip(_translate("MainWindow", "Select the base background color to use in itemFilter"))
         self.color_link_boots.setText(_translate("MainWindow", "Boots"))
         self.color_link_weapons.setStatusTip(_translate("MainWindow", "Select the base background color to use in itemFilter"))
         self.color_link_weapons.setText(_translate("MainWindow", "Weapons"))
+        self.label_12.setText(_translate("MainWindow", "Delay:"))
         self.menuLinks.setTitle(_translate("MainWindow", "Community Tools"))
         self.menuSettings.setTitle(_translate("MainWindow", "Settings"))
         self.menuAbout.setTitle(_translate("MainWindow", "About"))
         self.actionFilterblade_xyz.setText(_translate("MainWindow", "Filterblade.xyz"))
         self.actionChipy_dev.setText(_translate("MainWindow", "Chipy.dev"))
         self.actionPathOfExile_com.setText(_translate("MainWindow", "Path of Exile (Official)"))
         self.actionPathOfBuilding_com.setText(_translate("MainWindow", "Path of Building"))
@@ -614,14 +636,15 @@
         self.actionPoE_Ninja.setText(_translate("MainWindow", "PoE Ninja"))
         self.actionPoE_Lab.setText(_translate("MainWindow", "PoE Lab"))
         self.actionAwakened_PoE_Trade.setText(_translate("MainWindow", "Awakened PoE Trade"))
         self.actionInput_ClientSecret.setText(_translate("MainWindow", "Request ClientSecret"))
         self.actionGitHub.setText(_translate("MainWindow", "GitHub"))
         self.actionPatreon.setText(_translate("MainWindow", "Patreon"))
         self.action_NOT_AFFILIATED_WITH_ANY.setText(_translate("MainWindow", "*NOT AFFILIATED"))
+        self.actiondev_button.setText(_translate("MainWindow", "dev_button"))
 
 
 if __name__ == "__main__":
     import sys
     app = QtWidgets.QApplication(sys.argv)
     MainWindow = QtWidgets.QMainWindow()
     ui = Ui_MainWindow()
```

### Comparing `cpct-0.1.9/cpct/qt/main_gui.ui` & `cpct-0.2.1/cpct/qt/main_gui.ui`

 * *Files 0% similar despite different names*

#### Comparing `cpct-0.1.9/cpct/qt/main_gui.ui` & `cpct-0.2.1/cpct/qt/main_gui.ui`

```diff
@@ -450,14 +450,17 @@
             <family>Roboto</family>
             <pointsize>12</pointsize>
           </font>
         </property>
         <property name="statusTip">
           <string>Number of sets to be collecting (for show progress)</string>
         </property>
+        <property name="minimum">
+          <number>2</number>
+        </property>
         <property name="value">
           <number>8</number>
         </property>
       </widget>
       <widget class="QLabel" name="label_11">
         <property name="geometry">
           <rect>
@@ -538,15 +541,15 @@
         </property>
         <property name="statusTip">
           <string>How to interact with filter (Disabled to leave filters alone)</string>
         </property>
       </widget>
       <widget class="QLabel" name="item_2">
         <property name="enabled">
-          <bool>false</bool>
+          <bool>true</bool>
         </property>
         <property name="geometry">
           <rect>
             <x>10</x>
             <y>230</y>
             <width>111</width>
             <height>21</height>
@@ -560,15 +563,15 @@
         </property>
         <property name="text">
           <string>Recipe:</string>
         </property>
       </widget>
       <widget class="QRadioButton" name="recipe_chaos">
         <property name="enabled">
-          <bool>false</bool>
+          <bool>true</bool>
         </property>
         <property name="geometry">
           <rect>
             <x>70</x>
             <y>230</y>
             <width>91</width>
             <height>17</height>
@@ -591,15 +594,15 @@
         </property>
         <attribute name="buttonGroup">
           <string notr="true">recipe_type</string>
         </attribute>
       </widget>
       <widget class="QRadioButton" name="recipe_regal">
         <property name="enabled">
-          <bool>false</bool>
+          <bool>true</bool>
         </property>
         <property name="geometry">
           <rect>
             <x>70</x>
             <y>250</y>
             <width>91</width>
             <height>17</height>
@@ -611,15 +614,15 @@
             <pointsize>10</pointsize>
           </font>
         </property>
         <property name="statusTip">
           <string>Regal Recipe: Unidentified set of all items iLevel +70</string>
         </property>
         <property name="text">
-          <string>Regal (i70+)</string>
+          <string>Regal (i75+)</string>
         </property>
         <attribute name="buttonGroup">
           <string notr="true">recipe_type</string>
         </attribute>
       </widget>
       <widget class="QPushButton" name="item_filter_browse">
         <property name="geometry">
@@ -1240,15 +1243,62 @@
             <height>20</height>
           </size>
         </property>
         <property name="autoRepeatDelay">
           <number>1000</number>
         </property>
       </widget>
+      <widget class="QLabel" name="label_12">
+        <property name="geometry">
+          <rect>
+            <x>200</x>
+            <y>250</y>
+            <width>71</width>
+            <height>21</height>
+          </rect>
+        </property>
+        <property name="font">
+          <font>
+            <family>Roboto</family>
+            <pointsize>12</pointsize>
+          </font>
+        </property>
+        <property name="text">
+          <string>Delay:</string>
+        </property>
+      </widget>
+      <widget class="QDoubleSpinBox" name="set_delay">
+        <property name="geometry">
+          <rect>
+            <x>270</x>
+            <y>250</y>
+            <width>61</width>
+            <height>22</height>
+          </rect>
+        </property>
+        <property name="font">
+          <font>
+            <pointsize>12</pointsize>
+          </font>
+        </property>
+        <property name="minimum">
+          <double>0.010000000000000</double>
+        </property>
+        <property name="maximum">
+          <double>9.990000000000000</double>
+        </property>
+        <property name="singleStep">
+          <double>0.010000000000000</double>
+        </property>
+        <property name="value">
+          <double>0.040000000000000</double>
+        </property>
+      </widget>
     </widget>
+    <widget class="QStatusBar" name="statusbar"/>
     <widget class="QMenuBar" name="menubar">
       <property name="geometry">
         <rect>
           <x>0</x>
           <y>0</y>
           <width>717</width>
           <height>21</height>
@@ -1271,28 +1321,28 @@
         <addaction name="actionAwakened_PoE_Trade"/>
       </widget>
       <widget class="QMenu" name="menuSettings">
         <property name="title">
           <string>Settings</string>
         </property>
         <addaction name="actionInput_ClientSecret"/>
+        <addaction name="actiondev_button"/>
       </widget>
       <widget class="QMenu" name="menuAbout">
         <property name="title">
           <string>About</string>
         </property>
         <addaction name="actionChipy_dev"/>
         <addaction name="actionGitHub"/>
         <addaction name="actionPatreon"/>
       </widget>
       <addaction name="menuSettings"/>
       <addaction name="menuLinks"/>
       <addaction name="menuAbout"/>
     </widget>
-    <widget class="QStatusBar" name="statusbar"/>
     <action name="actionFilterblade_xyz">
       <property name="text">
         <string>Filterblade.xyz</string>
       </property>
     </action>
     <action name="actionChipy_dev">
       <property name="text">
@@ -1358,14 +1408,19 @@
       </property>
     </action>
     <action name="action_NOT_AFFILIATED_WITH_ANY">
       <property name="text">
         <string>*NOT AFFILIATED</string>
       </property>
     </action>
+    <action name="actiondev_button">
+      <property name="text">
+        <string>dev_button</string>
+      </property>
+    </action>
   </widget>
   <resources>
     <include location="color-picker-dropper-colour-svgrepo-com.svg"/>
   </resources>
   <connections/>
   <buttongroups>
     <buttongroup name="recipe_type"/>
```

### Comparing `cpct-0.1.9/.gitignore` & `cpct-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `cpct-0.1.9/LICENSE.txt` & `cpct-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cpct-0.1.9/README.md` & `cpct-0.2.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -4,14 +4,17 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/cpct.svg)](https://pypi.org/project/cpct)
 
 -----
 
 **Table of Contents**
 
 - [Installation](#installation)
+- [Why Chaos Recipe](#Why_Chaos_Recipe)
+- [Features](#Features)
+- [Features Requests](#FeaturesRequests)
 - [License](#license)
 - [chipy.dev](https://chipy.dev)
 
 ## Installation
 
 *PIP install method*
 ```console
@@ -82,16 +85,29 @@
 - Default will add it's recipe items colors to existing filter
 - Disabled will no affect your filter at all
 - *PLANNED* FilterBlade will edit the chaos recipe section of a filterblade filter
 
 
 ## Feature Requests
 
-- Integration with FilterBlade filters (rather than just added it's own)
-- Integration with Online filters (if possible)
-- Additional filter color/font/size customization options
+[ ] Integration with FilterBlade filters (rather than just added it's own)
+[ ] Integration with Online filters (if possible)
+[ ] Additional filter color/font/size customization options
+[ ] Add alpha slider to picker
+[ ] Rebuild item reading system into ENUM to easy class changes
+[ ] Add 2-H weapon options to filter
+[ ] Add league and tab memory
+[ ] Add never hide rings/ammy options
+[ ] Add sets ready counters (with ilvl checking)
+[ ] Add feature to indicate next items
+[ ] Fix auto refresh not renewing the list in the GUI display
+[ ] Add auto check limiter to read and log last checked zone entry
+[ ] Fix GUI and regal filter to be i75 (not 70)
+[ ] Write for Steam Version and path options!
+
+ 
 
 ## License
 `cpct` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
 
 ## DISCLAIMER:
-This product isn't affiliated with or endorsed by Grinding Gear Games in any way.
+This product isn't affiliated with or endorsed by Grinding Gear Games in any way.
```

### Comparing `cpct-0.1.9/pyproject.toml` & `cpct-0.2.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -30,15 +30,15 @@
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
-dependencies = ["requests","PyQt5", "websockets"]
+dependencies = ["requests", "PyQt5", "PyQt", "websockets", "pywinauto", "pyautogui", "psutil"]
 dynamic = ["version"]
 
 [project.urls]
 Documentation = "https://github.com/unknown/cpct#readme"
 Issues = "https://github.com/unknown/cpct/issues"
 Source = "https://github.com/unknown/cpct"
```

### Comparing `cpct-0.1.9/PKG-INFO` & `cpct-0.2.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpct
-Version: 0.1.9
+Version: 0.2.1
 Summary: Chipys PathOfExile Chaos Tool
 Project-URL: Documentation, https://github.com/unknown/cpct#readme
 Project-URL: Issues, https://github.com/unknown/cpct/issues
 Project-URL: Source, https://github.com/unknown/cpct
 Author-email: Chipy <iamchipy@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -15,29 +15,36 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
+Requires-Dist: psutil
+Requires-Dist: pyautogui
+Requires-Dist: pyqt
 Requires-Dist: pyqt5
+Requires-Dist: pywinauto
 Requires-Dist: requests
 Requires-Dist: websockets
 Description-Content-Type: text/markdown
 
 # cpct (Chipy's PathOfExile Chaos Tool)
 
 [![PyPI - Version](https://img.shields.io/pypi/v/cpct.svg)](https://pypi.org/project/cpct)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/cpct.svg)](https://pypi.org/project/cpct)
 
 -----
 
 **Table of Contents**
 
 - [Installation](#installation)
+- [Why Chaos Recipe](#Why_Chaos_Recipe)
+- [Features](#Features)
+- [Features Requests](#FeaturesRequests)
 - [License](#license)
 - [chipy.dev](https://chipy.dev)
 
 ## Installation
 
 *PIP install method*
 ```console
@@ -108,16 +115,29 @@
 - Default will add it's recipe items colors to existing filter
 - Disabled will no affect your filter at all
 - *PLANNED* FilterBlade will edit the chaos recipe section of a filterblade filter
 
 
 ## Feature Requests
 
-- Integration with FilterBlade filters (rather than just added it's own)
-- Integration with Online filters (if possible)
-- Additional filter color/font/size customization options
+[ ] Integration with FilterBlade filters (rather than just added it's own)
+[ ] Integration with Online filters (if possible)
+[ ] Additional filter color/font/size customization options
+[ ] Add alpha slider to picker
+[ ] Rebuild item reading system into ENUM to easy class changes
+[ ] Add 2-H weapon options to filter
+[ ] Add league and tab memory
+[ ] Add never hide rings/ammy options
+[ ] Add sets ready counters (with ilvl checking)
+[ ] Add feature to indicate next items
+[ ] Fix auto refresh not renewing the list in the GUI display
+[ ] Add auto check limiter to read and log last checked zone entry
+[ ] Fix GUI and regal filter to be i75 (not 70)
+[ ] Write for Steam Version and path options!
+
+ 
 
 ## License
 `cpct` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
 
 ## DISCLAIMER:
-This product isn't affiliated with or endorsed by Grinding Gear Games in any way.
+This product isn't affiliated with or endorsed by Grinding Gear Games in any way.
```

