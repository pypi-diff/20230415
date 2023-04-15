# Comparing `tmp/rustplus-5.5.7.tar.gz` & `tmp/rustplus-5.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rustplus-5.5.7.tar", last modified: Wed Mar 15 09:26:38 2023, max compression
+gzip compressed data, was "rustplus-5.5.8.tar", last modified: Wed Mar 15 22:08:54 2023, max compression
```

## Comparing `rustplus-5.5.7.tar` & `rustplus-5.5.8.tar`

### file list

```diff
@@ -1,116 +1,116 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 09:26:38.389912 rustplus-5.5.7/
--rw-r--r--   0 runner    (1001) docker     (122)     1075 2023-03-15 09:26:24.000000 rustplus-5.5.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       32 2023-03-15 09:26:24.000000 rustplus-5.5.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     2355 2023-03-15 09:26:38.389912 rustplus-5.5.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2005 2023-03-15 09:26:24.000000 rustplus-5.5.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 09:26:38.369912 rustplus-5.5.7/rustplus/
--rw-r--r--   0 runner    (1001) docker     (122)      775 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 09:26:38.373912 rustplus-5.5.7/rustplus/api/
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    19720 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/api/base_rust_api.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 09:26:38.377912 rustplus-5.5.7/rustplus/api/icons/
--rw-r--r--   0 runner    (1001) docker     (122)       16 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/api/icons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    23598 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/api/icons/airfield.png
--rw-r--r--   0 runner    (1001) docker     (122)    13944 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/api/icons/arctic_base.png
--rw-r--r--   0 runner    (1001) docker     (122)     3475 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/api/icons/bandit.png
--rw-r--r--   0 runner    (1001) docker     (122)    35348 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/api/icons/barn.png
--rw-r--r--   0 runner    (1001) docker     (122)     2553 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/api/icons/cargo.png
--rw-r--r--   0 runner    (1001) docker     (122)     2058 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/api/icons/chinook.png
--rw-r--r--   0 runner    (1001) docker     (122)     4228 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/api/icons/chinook_blades.png
--rw-r--r--   0 runner    (1001) docker     (122)    23420 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/api/icons/crate.png
--rw-r--r--   0 runner    (1001) docker     (122)    12339 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/api/icons/desert_base.png
--rw-r--r--   0 runner    (1001) docker     (122)    34156 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/api/icons/dome.png
--rw-r--r--   0 runner    (1001) docker     (122)    34662 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/api/icons/excavator.png
--rw-r--r--   0 runner    (1001) docker     (122)     4934 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/api/icons/explosion.png
--rw-r--r--   0 runner    (1001) docker     (122)    24176 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/api/icons/fishing.png
--rw-r--r--   0 runner    (1001) docker     (122)     2882 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/api/icons/harbour.png
--rw-r--r--   0 runner    (1001) docker     (122)    12195 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/api/icons/icon.png
--rw-r--r--   0 runner    (1001) docker     (122)    41087 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/api/icons/junkyard.png
--rw-r--r--   0 runner    (1001) docker     (122)     9091 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/api/icons/large_oil_rig.png
--rw-r--r--   0 runner    (1001) docker     (122)    23696 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/api/icons/launchsite.png
--rw-r--r--   0 runner    (1001) docker     (122)    27391 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/api/icons/lighthouse.png
--rw-r--r--   0 runner    (1001) docker     (122)    23532 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/api/icons/military_tunnels.png
--rw-r--r--   0 runner    (1001) docker     (122)    27923 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/api/icons/mining_outpost.png
--rw-r--r--   0 runner    (1001) docker     (122)    30573 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/api/icons/outpost.png
--rw-r--r--   0 runner    (1001) docker     (122)     2384 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/api/icons/oxums.png
--rw-r--r--   0 runner    (1001) docker     (122)     2742 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/api/icons/patrol.png
--rw-r--r--   0 runner    (1001) docker     (122)    23513 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/api/icons/power_plant.png
--rw-r--r--   0 runner    (1001) docker     (122)    36433 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/api/icons/quarry.png
--rw-r--r--   0 runner    (1001) docker     (122)    28365 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/api/icons/satellite.png
--rw-r--r--   0 runner    (1001) docker     (122)    17804 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/api/icons/sewer.png
--rw-r--r--   0 runner    (1001) docker     (122)     8114 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/api/icons/small_oil_rig.png
--rw-r--r--   0 runner    (1001) docker     (122)    30710 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/api/icons/stable.png
--rw-r--r--   0 runner    (1001) docker     (122)    28458 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/api/icons/supermarket.png
--rw-r--r--   0 runner    (1001) docker     (122)     2049 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/api/icons/swamp.png
--rw-r--r--   0 runner    (1001) docker     (122)     5300 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/api/icons/train.png
--rw-r--r--   0 runner    (1001) docker     (122)    20587 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/api/icons/train_yard.png
--rw-r--r--   0 runner    (1001) docker     (122)     3066 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/api/icons/underwater_lab.png
--rw-r--r--   0 runner    (1001) docker     (122)     5705 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/api/icons/vending_machine.png
--rw-r--r--   0 runner    (1001) docker     (122)    23907 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/api/icons/water_treatment.png
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 09:26:38.381912 rustplus-5.5.7/rustplus/api/remote/
--rw-r--r--   0 runner    (1001) docker     (122)      341 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/api/remote/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 09:26:38.381912 rustplus-5.5.7/rustplus/api/remote/camera/
--rw-r--r--   0 runner    (1001) docker     (122)      147 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/api/remote/camera/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)   118649 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/api/remote/camera/camera_constants.py
--rw-r--r--   0 runner    (1001) docker     (122)     3513 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/api/remote/camera/camera_manager.py
--rw-r--r--   0 runner    (1001) docker     (122)     6469 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/api/remote/camera/camera_parser.py
--rw-r--r--   0 runner    (1001) docker     (122)     2416 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/api/remote/camera/structures.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 09:26:38.381912 rustplus-5.5.7/rustplus/api/remote/events/
--rw-r--r--   0 runner    (1001) docker     (122)      183 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/api/remote/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2141 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/api/remote/events/event_handler.py
--rw-r--r--   0 runner    (1001) docker     (122)      684 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/api/remote/events/event_loop_manager.py
--rw-r--r--   0 runner    (1001) docker     (122)     3195 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/api/remote/events/events.py
--rw-r--r--   0 runner    (1001) docker     (122)     2286 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/api/remote/events/handler_list.py
--rw-r--r--   0 runner    (1001) docker     (122)     3105 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/api/remote/events/map_event_listener.py
--rw-r--r--   0 runner    (1001) docker     (122)      738 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/api/remote/events/registered_listener.py
--rw-r--r--   0 runner    (1001) docker     (122)     1841 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/api/remote/expo_bundle_handler.py
--rw-r--r--   0 runner    (1001) docker     (122)      665 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/api/remote/fcm_listener.py
--rw-r--r--   0 runner    (1001) docker     (122)      806 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/api/remote/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (122)     4123 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/api/remote/ratelimiter.py
--rw-r--r--   0 runner    (1001) docker     (122)     8261 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/api/remote/rust_remote_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 09:26:38.381912 rustplus-5.5.7/rustplus/api/remote/rustplus_proto/
--rw-r--r--   0 runner    (1001) docker     (122)     3946 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/api/remote/rustplus_proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    18568 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/api/remote/rustplus_proto/rustplus_pb2.py
--rw-r--r--   0 runner    (1001) docker     (122)    11412 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/api/remote/rustws.py
--rw-r--r--   0 runner    (1001) docker     (122)      781 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/api/remote/server_checker.py
--rw-r--r--   0 runner    (1001) docker     (122)    13311 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/api/rust_api.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 09:26:38.385913 rustplus-5.5.7/rustplus/api/structures/
--rw-r--r--   0 runner    (1001) docker     (122)      390 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/api/structures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      824 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/api/structures/rust_chat_message.py
--rw-r--r--   0 runner    (1001) docker     (122)      852 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/api/structures/rust_contents.py
--rw-r--r--   0 runner    (1001) docker     (122)     1948 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/api/structures/rust_entity_info.py
--rw-r--r--   0 runner    (1001) docker     (122)     1943 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/api/structures/rust_info.py
--rw-r--r--   0 runner    (1001) docker     (122)      780 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/api/structures/rust_item.py
--rw-r--r--   0 runner    (1001) docker     (122)     1759 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/api/structures/rust_map.py
--rw-r--r--   0 runner    (1001) docker     (122)     4676 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/api/structures/rust_marker.py
--rw-r--r--   0 runner    (1001) docker     (122)     2864 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/api/structures/rust_team_info.py
--rw-r--r--   0 runner    (1001) docker     (122)     1110 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/api/structures/rust_time.py
--rw-r--r--   0 runner    (1001) docker     (122)       93 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/api/structures/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 09:26:38.385913 rustplus-5.5.7/rustplus/commands/
--rw-r--r--   0 runner    (1001) docker     (122)      130 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      542 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/commands/command.py
--rw-r--r--   0 runner    (1001) docker     (122)      522 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/commands/command_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     2963 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/commands/command_handler.py
--rw-r--r--   0 runner    (1001) docker     (122)      445 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/commands/command_options.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 09:26:38.385913 rustplus-5.5.7/rustplus/conversation/
--rw-r--r--   0 runner    (1001) docker     (122)      145 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/conversation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1882 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/conversation/conversation.py
--rw-r--r--   0 runner    (1001) docker     (122)     1551 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/conversation/conversation_factory.py
--rw-r--r--   0 runner    (1001) docker     (122)      289 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/conversation/conversation_prompt.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 09:26:38.385913 rustplus-5.5.7/rustplus/exceptions/
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1158 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/exceptions/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 09:26:38.385913 rustplus-5.5.7/rustplus/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      139 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      925 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/utils/deprecated.py
--rw-r--r--   0 runner    (1001) docker     (122)    26442 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/utils/grab_items.py
--rw-r--r--   0 runner    (1001) docker     (122)     5322 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/utils/rust_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      752 2023-03-15 09:26:24.000000 rustplus-5.5.7/rustplus/utils/server_id.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 09:26:38.373912 rustplus-5.5.7/rustplus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2355 2023-03-15 09:26:38.000000 rustplus-5.5.7/rustplus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3433 2023-03-15 09:26:38.000000 rustplus-5.5.7/rustplus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-15 09:26:38.000000 rustplus-5.5.7/rustplus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       95 2023-03-15 09:26:38.000000 rustplus-5.5.7/rustplus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-03-15 09:26:38.000000 rustplus-5.5.7/rustplus.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-03-15 09:26:38.389912 rustplus-5.5.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1081 2023-03-15 09:26:24.000000 rustplus-5.5.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 22:08:54.011145 rustplus-5.5.8/
+-rw-r--r--   0 runner    (1001) docker     (122)     1075 2023-03-15 22:08:43.000000 rustplus-5.5.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-03-15 22:08:43.000000 rustplus-5.5.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     2355 2023-03-15 22:08:54.011145 rustplus-5.5.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2005 2023-03-15 22:08:43.000000 rustplus-5.5.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 22:08:54.003145 rustplus-5.5.8/rustplus/
+-rw-r--r--   0 runner    (1001) docker     (122)      775 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 22:08:54.003145 rustplus-5.5.8/rustplus/api/
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19720 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/base_rust_api.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 22:08:54.007145 rustplus-5.5.8/rustplus/api/icons/
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/icons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23598 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/icons/airfield.png
+-rw-r--r--   0 runner    (1001) docker     (122)    13944 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/icons/arctic_base.png
+-rw-r--r--   0 runner    (1001) docker     (122)     3475 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/icons/bandit.png
+-rw-r--r--   0 runner    (1001) docker     (122)    35348 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/icons/barn.png
+-rw-r--r--   0 runner    (1001) docker     (122)     2553 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/icons/cargo.png
+-rw-r--r--   0 runner    (1001) docker     (122)     2058 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/icons/chinook.png
+-rw-r--r--   0 runner    (1001) docker     (122)     4228 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/icons/chinook_blades.png
+-rw-r--r--   0 runner    (1001) docker     (122)    23420 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/icons/crate.png
+-rw-r--r--   0 runner    (1001) docker     (122)    12339 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/icons/desert_base.png
+-rw-r--r--   0 runner    (1001) docker     (122)    34156 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/icons/dome.png
+-rw-r--r--   0 runner    (1001) docker     (122)    34662 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/icons/excavator.png
+-rw-r--r--   0 runner    (1001) docker     (122)     4934 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/icons/explosion.png
+-rw-r--r--   0 runner    (1001) docker     (122)    24176 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/icons/fishing.png
+-rw-r--r--   0 runner    (1001) docker     (122)     2882 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/icons/harbour.png
+-rw-r--r--   0 runner    (1001) docker     (122)    12195 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/icons/icon.png
+-rw-r--r--   0 runner    (1001) docker     (122)    41087 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/icons/junkyard.png
+-rw-r--r--   0 runner    (1001) docker     (122)     9091 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/icons/large_oil_rig.png
+-rw-r--r--   0 runner    (1001) docker     (122)    23696 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/icons/launchsite.png
+-rw-r--r--   0 runner    (1001) docker     (122)    27391 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/icons/lighthouse.png
+-rw-r--r--   0 runner    (1001) docker     (122)    23532 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/icons/military_tunnels.png
+-rw-r--r--   0 runner    (1001) docker     (122)    27923 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/icons/mining_outpost.png
+-rw-r--r--   0 runner    (1001) docker     (122)    30573 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/icons/outpost.png
+-rw-r--r--   0 runner    (1001) docker     (122)     2384 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/icons/oxums.png
+-rw-r--r--   0 runner    (1001) docker     (122)     2742 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/icons/patrol.png
+-rw-r--r--   0 runner    (1001) docker     (122)    23513 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/icons/power_plant.png
+-rw-r--r--   0 runner    (1001) docker     (122)    36433 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/icons/quarry.png
+-rw-r--r--   0 runner    (1001) docker     (122)    28365 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/icons/satellite.png
+-rw-r--r--   0 runner    (1001) docker     (122)    17804 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/icons/sewer.png
+-rw-r--r--   0 runner    (1001) docker     (122)     8114 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/icons/small_oil_rig.png
+-rw-r--r--   0 runner    (1001) docker     (122)    30710 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/icons/stable.png
+-rw-r--r--   0 runner    (1001) docker     (122)    28458 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/icons/supermarket.png
+-rw-r--r--   0 runner    (1001) docker     (122)     2049 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/icons/swamp.png
+-rw-r--r--   0 runner    (1001) docker     (122)     5300 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/icons/train.png
+-rw-r--r--   0 runner    (1001) docker     (122)    20587 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/icons/train_yard.png
+-rw-r--r--   0 runner    (1001) docker     (122)     3066 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/icons/underwater_lab.png
+-rw-r--r--   0 runner    (1001) docker     (122)     5705 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/icons/vending_machine.png
+-rw-r--r--   0 runner    (1001) docker     (122)    23907 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/icons/water_treatment.png
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 22:08:54.007145 rustplus-5.5.8/rustplus/api/remote/
+-rw-r--r--   0 runner    (1001) docker     (122)      341 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/remote/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 22:08:54.007145 rustplus-5.5.8/rustplus/api/remote/camera/
+-rw-r--r--   0 runner    (1001) docker     (122)      147 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/remote/camera/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)   118649 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/remote/camera/camera_constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3629 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/remote/camera/camera_manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6029 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/remote/camera/camera_parser.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2479 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/remote/camera/structures.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 22:08:54.007145 rustplus-5.5.8/rustplus/api/remote/events/
+-rw-r--r--   0 runner    (1001) docker     (122)      183 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/remote/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2141 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/remote/events/event_handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)      684 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/remote/events/event_loop_manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3195 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/remote/events/events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2286 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/remote/events/handler_list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3105 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/remote/events/map_event_listener.py
+-rw-r--r--   0 runner    (1001) docker     (122)      738 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/remote/events/registered_listener.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1841 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/remote/expo_bundle_handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)      665 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/remote/fcm_listener.py
+-rw-r--r--   0 runner    (1001) docker     (122)      806 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/remote/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4123 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/remote/ratelimiter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8293 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/remote/rust_remote_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 22:08:54.007145 rustplus-5.5.8/rustplus/api/remote/rustplus_proto/
+-rw-r--r--   0 runner    (1001) docker     (122)     3946 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/remote/rustplus_proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18568 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/remote/rustplus_proto/rustplus_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11412 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/remote/rustws.py
+-rw-r--r--   0 runner    (1001) docker     (122)      781 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/remote/server_checker.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13311 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/rust_api.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 22:08:54.007145 rustplus-5.5.8/rustplus/api/structures/
+-rw-r--r--   0 runner    (1001) docker     (122)      390 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/structures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      824 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/structures/rust_chat_message.py
+-rw-r--r--   0 runner    (1001) docker     (122)      852 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/structures/rust_contents.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1948 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/structures/rust_entity_info.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1943 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/structures/rust_info.py
+-rw-r--r--   0 runner    (1001) docker     (122)      780 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/structures/rust_item.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1759 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/structures/rust_map.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4676 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/structures/rust_marker.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2864 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/structures/rust_team_info.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1110 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/structures/rust_time.py
+-rw-r--r--   0 runner    (1001) docker     (122)       93 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/api/structures/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 22:08:54.007145 rustplus-5.5.8/rustplus/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)      130 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      542 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/commands/command.py
+-rw-r--r--   0 runner    (1001) docker     (122)      522 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/commands/command_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2963 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/commands/command_handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)      445 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/commands/command_options.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 22:08:54.011145 rustplus-5.5.8/rustplus/conversation/
+-rw-r--r--   0 runner    (1001) docker     (122)      145 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/conversation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1882 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/conversation/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1551 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/conversation/conversation_factory.py
+-rw-r--r--   0 runner    (1001) docker     (122)      289 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/conversation/conversation_prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 22:08:54.011145 rustplus-5.5.8/rustplus/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1158 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/exceptions/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 22:08:54.011145 rustplus-5.5.8/rustplus/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      139 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      925 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/utils/deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26442 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/utils/grab_items.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5322 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/utils/rust_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      752 2023-03-15 22:08:43.000000 rustplus-5.5.8/rustplus/utils/server_id.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 22:08:54.003145 rustplus-5.5.8/rustplus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2355 2023-03-15 22:08:53.000000 rustplus-5.5.8/rustplus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3433 2023-03-15 22:08:53.000000 rustplus-5.5.8/rustplus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-15 22:08:53.000000 rustplus-5.5.8/rustplus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       95 2023-03-15 22:08:53.000000 rustplus-5.5.8/rustplus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-03-15 22:08:53.000000 rustplus-5.5.8/rustplus.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-03-15 22:08:54.011145 rustplus-5.5.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1081 2023-03-15 22:08:43.000000 rustplus-5.5.8/setup.py
```

### Comparing `rustplus-5.5.7/LICENSE` & `rustplus-5.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.7/PKG-INFO` & `rustplus-5.5.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rustplus
-Version: 5.5.7
+Version: 5.5.8
 Summary: A python wrapper for the Rust Plus API
 Home-page: https://github.com/olijeffers0n/rustplus
 Author: olijeffers0n
 License: MIT
 Project-URL: Issue tracker, https://github.com/olijeffers0n/rustplus/issues
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
```

### Comparing `rustplus-5.5.7/README.md` & `rustplus-5.5.8/README.md`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.7/rustplus/__init__.py` & `rustplus-5.5.8/rustplus/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,9 +18,9 @@
 from .commands import CommandOptions, Command
 from .exceptions import *
 from .conversation import ConversationFactory, Conversation, ConversationPrompt
 from .utils import *
 
 __name__ = "rustplus"
 __author__ = "olijeffers0n"
-__version__ = "5.5.7"
+__version__ = "5.5.8"
 __support__ = "Discord: https://discord.gg/nQqJe8qvP8"
```

### Comparing `rustplus-5.5.7/rustplus/api/base_rust_api.py` & `rustplus-5.5.8/rustplus/api/base_rust_api.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.7/rustplus/api/icons/airfield.png` & `rustplus-5.5.8/rustplus/api/icons/airfield.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.7/rustplus/api/icons/arctic_base.png` & `rustplus-5.5.8/rustplus/api/icons/arctic_base.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.7/rustplus/api/icons/bandit.png` & `rustplus-5.5.8/rustplus/api/icons/bandit.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.7/rustplus/api/icons/barn.png` & `rustplus-5.5.8/rustplus/api/icons/barn.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.7/rustplus/api/icons/cargo.png` & `rustplus-5.5.8/rustplus/api/icons/cargo.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.7/rustplus/api/icons/chinook.png` & `rustplus-5.5.8/rustplus/api/icons/chinook.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.7/rustplus/api/icons/chinook_blades.png` & `rustplus-5.5.8/rustplus/api/icons/chinook_blades.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.7/rustplus/api/icons/crate.png` & `rustplus-5.5.8/rustplus/api/icons/crate.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.7/rustplus/api/icons/desert_base.png` & `rustplus-5.5.8/rustplus/api/icons/desert_base.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.7/rustplus/api/icons/dome.png` & `rustplus-5.5.8/rustplus/api/icons/dome.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.7/rustplus/api/icons/excavator.png` & `rustplus-5.5.8/rustplus/api/icons/excavator.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.7/rustplus/api/icons/explosion.png` & `rustplus-5.5.8/rustplus/api/icons/explosion.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.7/rustplus/api/icons/fishing.png` & `rustplus-5.5.8/rustplus/api/icons/fishing.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.7/rustplus/api/icons/harbour.png` & `rustplus-5.5.8/rustplus/api/icons/harbour.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.7/rustplus/api/icons/icon.png` & `rustplus-5.5.8/rustplus/api/icons/icon.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.7/rustplus/api/icons/junkyard.png` & `rustplus-5.5.8/rustplus/api/icons/junkyard.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.7/rustplus/api/icons/large_oil_rig.png` & `rustplus-5.5.8/rustplus/api/icons/large_oil_rig.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.7/rustplus/api/icons/launchsite.png` & `rustplus-5.5.8/rustplus/api/icons/launchsite.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.7/rustplus/api/icons/lighthouse.png` & `rustplus-5.5.8/rustplus/api/icons/lighthouse.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.7/rustplus/api/icons/military_tunnels.png` & `rustplus-5.5.8/rustplus/api/icons/military_tunnels.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.7/rustplus/api/icons/mining_outpost.png` & `rustplus-5.5.8/rustplus/api/icons/mining_outpost.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.7/rustplus/api/icons/outpost.png` & `rustplus-5.5.8/rustplus/api/icons/outpost.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.7/rustplus/api/icons/oxums.png` & `rustplus-5.5.8/rustplus/api/icons/oxums.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.7/rustplus/api/icons/patrol.png` & `rustplus-5.5.8/rustplus/api/icons/patrol.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.7/rustplus/api/icons/power_plant.png` & `rustplus-5.5.8/rustplus/api/icons/power_plant.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.7/rustplus/api/icons/quarry.png` & `rustplus-5.5.8/rustplus/api/icons/quarry.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.7/rustplus/api/icons/satellite.png` & `rustplus-5.5.8/rustplus/api/icons/satellite.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.7/rustplus/api/icons/sewer.png` & `rustplus-5.5.8/rustplus/api/icons/sewer.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.7/rustplus/api/icons/small_oil_rig.png` & `rustplus-5.5.8/rustplus/api/icons/small_oil_rig.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.7/rustplus/api/icons/stable.png` & `rustplus-5.5.8/rustplus/api/icons/stable.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.7/rustplus/api/icons/supermarket.png` & `rustplus-5.5.8/rustplus/api/icons/supermarket.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.7/rustplus/api/icons/swamp.png` & `rustplus-5.5.8/rustplus/api/icons/swamp.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.7/rustplus/api/icons/train.png` & `rustplus-5.5.8/rustplus/api/icons/train.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.7/rustplus/api/icons/train_yard.png` & `rustplus-5.5.8/rustplus/api/icons/train_yard.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.7/rustplus/api/icons/underwater_lab.png` & `rustplus-5.5.8/rustplus/api/icons/underwater_lab.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.7/rustplus/api/icons/vending_machine.png` & `rustplus-5.5.8/rustplus/api/icons/vending_machine.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.7/rustplus/api/icons/water_treatment.png` & `rustplus-5.5.8/rustplus/api/icons/water_treatment.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.7/rustplus/api/remote/camera/camera_constants.py` & `rustplus-5.5.8/rustplus/api/remote/camera/camera_constants.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.7/rustplus/api/remote/camera/camera_manager.py` & `rustplus-5.5.8/rustplus/api/remote/camera/camera_manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -85,19 +85,22 @@
         app_request = self.rust_socket._generate_protobuf()
         app_request.cameraUnsubscribe.CopyFrom(AppEmpty())
 
         await self.rust_socket.remote.send_message(app_request)
         self.rust_socket.remote.ignored_responses.append(app_request.seq)
 
         self._open = False
-        self._last_packets = None
+        self._last_packets.clear()
 
     async def resubscribe(self) -> None:
         await self.rust_socket.remote.subscribe_to_camera(self._cam_id, True)
         self.time_since_last_subscribe = time.time()
+        self._open = True
+        self._last_packets.clear()
+        self.rust_socket.remote.camera_manager = self
 
     async def get_entities_in_frame(self) -> List[Entity]:
         if self._last_packets is None:
             return []
 
         if len(self._last_packets) == 0:
             return []
```

### Comparing `rustplus-5.5.7/rustplus/api/remote/camera/camera_parser.py` & `rustplus-5.5.8/rustplus/api/remote/camera/camera_parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import dataclasses
 from typing import Union, Tuple, List
 from PIL import Image
 
 from .camera_constants import LOOKUP_CONSTANTS
-from .structures import RayPacket
 
 
 @dataclasses.dataclass
 class RayData:
     distance: float
     alignment: float
     material: int
@@ -25,15 +24,15 @@
             [0.5, 0.5, 0.5],
             [0.8, 0.7, 0.7],
             [0.3, 0.7, 1],
             [0.6, 0.6, 0.6],
             [0.7, 0.7, 0.7],
             [0.8, 0.6, 0.4],
             [1, 0.4, 0.4],
-            [0.5, 0.5, 0.5],
+            [1, 0.1, 0.1],
         ]
 
         self.output = [None for _ in range(self.width * self.height)]
 
     async def handle_camera_ray_data(self, data) -> None:
         self._rays = data
         self.data_pointer = 0
@@ -41,15 +40,15 @@
         while self._sample_offset >= 2 * self.width * self.height:
             self._sample_offset -= 2 * self.width * self.height
         self._ray_lookback = [[0 for _ in range(3)] for _ in range(64)]
 
     async def step(self) -> None:
 
         if self._rays is None:
-            return None
+            return
 
         while True:
             if await self.process_rays_batch():
                 self._rays = None
                 break
 
     async def process_rays_batch(self) -> bool:
@@ -170,39 +169,29 @@
             if ray.distance == 1 and alignment == 0 and material == 0:
                 continue
 
             colour = self.colours[material]
             image.putpixel(
                 (i % self.width, self.height - 1 - (i // self.width)),
                 await self._convert_colour(
-                    (
-                        int(colour[0] * 255),
-                        int(colour[1] * 255),
-                        int(colour[2] * 255),
-                        int(alignment * 255),
-                    )
+                    (colour[0], colour[1], colour[2], alignment)
                 ),
             )
 
         return image
 
     @staticmethod
     async def _convert_colour(
-        colour: Tuple[int, int, int, int], background: Tuple[int, int, int] = (0, 0, 0)
+        colour: Tuple[float, float, float, float],
+        background: Tuple[int, int, int] = (0, 0, 0),
     ) -> Tuple[int, int, int]:
-        normalised_colour = (
-            colour[0] / 255,
-            colour[1] / 255,
-            colour[2] / 255,
-            colour[3] / 255,
-        )
         target_colour = (
-            ((1 - normalised_colour[3]) * background[0]) + (normalised_colour[3] * normalised_colour[0]),
-            ((1 - normalised_colour[3]) * background[1]) + (normalised_colour[3] * normalised_colour[1]),
-            ((1 - normalised_colour[3]) * background[2]) + (normalised_colour[3] * normalised_colour[2])
+            ((1 - colour[3]) * background[0]) + (colour[3] * colour[0]),
+            ((1 - colour[3]) * background[1]) + (colour[3] * colour[1]),
+            ((1 - colour[3]) * background[2]) + (colour[3] * colour[2]),
         )
 
         return (
             min(255, int(target_colour[0] * 255)),
             min(255, int(target_colour[1] * 255)),
-            min(255, int(target_colour[2] * 255))
+            min(255, int(target_colour[2] * 255)),
         )
```

### Comparing `rustplus-5.5.7/rustplus/api/remote/camera/structures.py` & `rustplus-5.5.8/rustplus/api/remote/camera/structures.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 class Entity:
     def __init__(self, entity_data) -> None:
         self.entity_id = entity_data.entityId
         self.type = entity_data.type
         self.position = entity_data.position
         self.rotation = entity_data.rotation
         self.size = entity_data.size
-        self.name = entity_data.name
+        self.name: str = entity_data.name
 
     def __str__(self) -> str:
         return (
             f"Entity(entity_id={self.entity_id}, type={self.type}, position={self.position}, "
             f"rotation={self.rotation}, size={self.size}, name={self.name})"
         )
 
@@ -68,9 +68,12 @@
 
     def get_last(self) -> Any:
         return self._queue[-1]
 
     def pop(self) -> Any:
         return self._queue.pop(0)
 
+    def clear(self) -> None:
+        self._queue.clear()
+
     def __len__(self) -> int:
         return len(self._queue)
```

### Comparing `rustplus-5.5.7/rustplus/api/remote/events/event_handler.py` & `rustplus-5.5.8/rustplus/api/remote/events/event_handler.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.7/rustplus/api/remote/events/event_loop_manager.py` & `rustplus-5.5.8/rustplus/api/remote/events/event_loop_manager.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.7/rustplus/api/remote/events/events.py` & `rustplus-5.5.8/rustplus/api/remote/events/events.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.7/rustplus/api/remote/events/handler_list.py` & `rustplus-5.5.8/rustplus/api/remote/events/handler_list.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.7/rustplus/api/remote/events/map_event_listener.py` & `rustplus-5.5.8/rustplus/api/remote/events/map_event_listener.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.7/rustplus/api/remote/events/registered_listener.py` & `rustplus-5.5.8/rustplus/api/remote/events/registered_listener.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.7/rustplus/api/remote/expo_bundle_handler.py` & `rustplus-5.5.8/rustplus/api/remote/expo_bundle_handler.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.7/rustplus/api/remote/fcm_listener.py` & `rustplus-5.5.8/rustplus/api/remote/fcm_listener.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.7/rustplus/api/remote/heartbeat.py` & `rustplus-5.5.8/rustplus/api/remote/heartbeat.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.7/rustplus/api/remote/ratelimiter.py` & `rustplus-5.5.8/rustplus/api/remote/ratelimiter.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.7/rustplus/api/remote/rust_remote_interface.py` & `rustplus-5.5.8/rustplus/api/remote/rust_remote_interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -222,24 +222,26 @@
             )
 
         future = asyncio.run_coroutine_threadsafe(
             get_entity_info(self, entity_id), EventLoopManager.get_loop(self.server_id)
         )
         future.add_done_callback(entity_event_callback)
 
-    async def subscribe_to_camera(self, entity_id: int, ignore: bool = False) -> AppRequest:
+    async def subscribe_to_camera(
+        self, entity_id: int, ignore_response: bool = False
+    ) -> AppRequest:
         await self.api._handle_ratelimit()
         app_request = self.api._generate_protobuf()
         subscribe = AppCameraSubscribe()
         subscribe.cameraId = entity_id
         app_request.cameraSubscribe.CopyFrom(subscribe)
 
         await self.send_message(app_request)
 
-        if ignore:
+        if ignore_response:
             self.ignored_responses.append(app_request.seq)
 
         return app_request
 
     async def create_camera_manager(self, cam_id) -> CameraManager:
 
         if self.camera_manager is not None:
```

### Comparing `rustplus-5.5.7/rustplus/api/remote/rustplus_proto/__init__.py` & `rustplus-5.5.8/rustplus/api/remote/rustplus_proto/__init__.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.7/rustplus/api/remote/rustplus_proto/rustplus_pb2.py` & `rustplus-5.5.8/rustplus/api/remote/rustplus_proto/rustplus_pb2.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.7/rustplus/api/remote/rustws.py` & `rustplus-5.5.8/rustplus/api/remote/rustws.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.7/rustplus/api/remote/server_checker.py` & `rustplus-5.5.8/rustplus/api/remote/server_checker.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.7/rustplus/api/rust_api.py` & `rustplus-5.5.8/rustplus/api/rust_api.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.7/rustplus/api/structures/rust_chat_message.py` & `rustplus-5.5.8/rustplus/api/structures/rust_chat_message.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.7/rustplus/api/structures/rust_contents.py` & `rustplus-5.5.8/rustplus/api/structures/rust_contents.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.7/rustplus/api/structures/rust_entity_info.py` & `rustplus-5.5.8/rustplus/api/structures/rust_entity_info.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.7/rustplus/api/structures/rust_info.py` & `rustplus-5.5.8/rustplus/api/structures/rust_info.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.7/rustplus/api/structures/rust_item.py` & `rustplus-5.5.8/rustplus/api/structures/rust_item.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.7/rustplus/api/structures/rust_map.py` & `rustplus-5.5.8/rustplus/api/structures/rust_map.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.7/rustplus/api/structures/rust_marker.py` & `rustplus-5.5.8/rustplus/api/structures/rust_marker.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.7/rustplus/api/structures/rust_team_info.py` & `rustplus-5.5.8/rustplus/api/structures/rust_team_info.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.7/rustplus/api/structures/rust_time.py` & `rustplus-5.5.8/rustplus/api/structures/rust_time.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.7/rustplus/commands/command.py` & `rustplus-5.5.8/rustplus/commands/command.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.7/rustplus/commands/command_data.py` & `rustplus-5.5.8/rustplus/commands/command_data.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.7/rustplus/commands/command_handler.py` & `rustplus-5.5.8/rustplus/commands/command_handler.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.7/rustplus/conversation/conversation.py` & `rustplus-5.5.8/rustplus/conversation/conversation.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.7/rustplus/conversation/conversation_factory.py` & `rustplus-5.5.8/rustplus/conversation/conversation_factory.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.7/rustplus/exceptions/exceptions.py` & `rustplus-5.5.8/rustplus/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.7/rustplus/utils/deprecated.py` & `rustplus-5.5.8/rustplus/utils/deprecated.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.7/rustplus/utils/grab_items.py` & `rustplus-5.5.8/rustplus/utils/grab_items.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.7/rustplus/utils/rust_utils.py` & `rustplus-5.5.8/rustplus/utils/rust_utils.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.7/rustplus/utils/server_id.py` & `rustplus-5.5.8/rustplus/utils/server_id.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.7/rustplus.egg-info/PKG-INFO` & `rustplus-5.5.8/rustplus.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rustplus
-Version: 5.5.7
+Version: 5.5.8
 Summary: A python wrapper for the Rust Plus API
 Home-page: https://github.com/olijeffers0n/rustplus
 Author: olijeffers0n
 License: MIT
 Project-URL: Issue tracker, https://github.com/olijeffers0n/rustplus/issues
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
```

### Comparing `rustplus-5.5.7/rustplus.egg-info/SOURCES.txt` & `rustplus-5.5.8/rustplus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rustplus-5.5.7/setup.py` & `rustplus-5.5.8/setup.py`

 * *Files identical despite different names*

