# Comparing `tmp/fabric_fim-1.4.7.tar.gz` & `tmp/fabric_fim-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabric_fim-1.4.7.tar", last modified: Fri Apr  7 20:53:02 2023, max compression
+gzip compressed data, was "fabric_fim-1.4.9.tar", last modified: Sat Apr  8 04:38:05 2023, max compression
```

## Comparing `fabric_fim-1.4.7.tar` & `fabric_fim-1.4.9.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-04-07 20:53:02.673249 fabric_fim-1.4.7/
--rw-r--r--   0 ibaldin    (502) staff       (20)       26 2020-07-24 21:42:44.000000 fabric_fim-1.4.7/AUTHORS
--rw-r--r--   0 ibaldin    (502) staff       (20)     1071 2020-07-14 22:09:49.000000 fabric_fim-1.4.7/LICENSE
--rw-r--r--   0 ibaldin    (502) staff       (20)      146 2022-04-27 22:22:19.000000 fabric_fim-1.4.7/MANIFEST.in
--rw-r--r--   0 ibaldin    (502) staff       (20)    11437 2023-04-07 20:53:02.672887 fabric_fim-1.4.7/PKG-INFO
--rw-r--r--   0 ibaldin    (502) staff       (20)    10990 2023-04-05 20:55:22.000000 fabric_fim-1.4.7/README.md
-drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-04-07 20:53:02.533814 fabric_fim-1.4.7/fabric_fim.egg-info/
--rw-r--r--   0 ibaldin    (502) staff       (20)    11437 2023-04-07 20:53:02.000000 fabric_fim-1.4.7/fabric_fim.egg-info/PKG-INFO
--rw-r--r--   0 ibaldin    (502) staff       (20)     2324 2023-04-07 20:53:02.000000 fabric_fim-1.4.7/fabric_fim.egg-info/SOURCES.txt
--rw-r--r--   0 ibaldin    (502) staff       (20)        1 2023-04-07 20:53:02.000000 fabric_fim-1.4.7/fabric_fim.egg-info/dependency_links.txt
--rw-r--r--   0 ibaldin    (502) staff       (20)      118 2023-04-07 20:53:02.000000 fabric_fim-1.4.7/fabric_fim.egg-info/requires.txt
--rw-r--r--   0 ibaldin    (502) staff       (20)        4 2023-04-07 20:53:02.000000 fabric_fim-1.4.7/fabric_fim.egg-info/top_level.txt
-drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-04-07 20:53:02.535369 fabric_fim-1.4.7/fim/
--rw-r--r--   0 ibaldin    (502) staff       (20)       22 2023-04-05 20:55:22.000000 fabric_fim-1.4.7/fim/__init__.py
-drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-04-07 20:53:02.537180 fabric_fim-1.4.7/fim/authz/
--rw-r--r--   0 ibaldin    (502) staff       (20)        1 2022-04-27 22:22:19.000000 fabric_fim-1.4.7/fim/authz/__init__.py
--rw-r--r--   0 ibaldin    (502) staff       (20)    16139 2023-02-02 01:41:56.000000 fabric_fim-1.4.7/fim/authz/attribute_collector.py
-drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-04-07 20:53:02.608058 fabric_fim-1.4.7/fim/graph/
--rw-r--r--   0 ibaldin    (502) staff       (20)        1 2020-09-02 18:31:38.000000 fabric_fim-1.4.7/fim/graph/__init__.py
--rw-r--r--   0 ibaldin    (502) staff       (20)    69693 2023-04-05 20:55:22.000000 fabric_fim-1.4.7/fim/graph/abc_property_graph.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     4093 2023-02-02 01:41:56.000000 fabric_fim-1.4.7/fim/graph/abc_property_graph_constants.py
-drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-04-07 20:53:02.621201 fabric_fim-1.4.7/fim/graph/data/
--rw-r--r--   0 ibaldin    (502) staff       (20)        1 2020-08-18 21:34:07.000000 fabric_fim-1.4.7/fim/graph/data/__init__.py
--rw-r--r--   0 ibaldin    (502) staff       (20)      283 2020-09-03 22:10:53.000000 fabric_fim-1.4.7/fim/graph/data/capacity_types.json
--rw-r--r--   0 ibaldin    (502) staff       (20)      100 2020-08-27 20:41:23.000000 fabric_fim-1.4.7/fim/graph/data/constraint_types.json
--rw-r--r--   0 ibaldin    (502) staff       (20)     3829 2023-04-05 20:55:22.000000 fabric_fim-1.4.7/fim/graph/data/graph_validation_rules.json
--rw-r--r--   0 ibaldin    (502) staff       (20)      547 2020-09-03 22:10:39.000000 fabric_fim-1.4.7/fim/graph/data/label_types.json
--rw-r--r--   0 ibaldin    (502) staff       (20)       91 2020-08-27 20:40:54.000000 fabric_fim-1.4.7/fim/graph/data/location_types.json
--rw-r--r--   0 ibaldin    (502) staff       (20)      367 2021-05-25 21:09:37.000000 fabric_fim-1.4.7/fim/graph/data/neo4j_indexes.json
--rw-r--r--   0 ibaldin    (502) staff       (20)    43467 2023-04-05 20:55:22.000000 fabric_fim-1.4.7/fim/graph/neo4j_property_graph.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     6160 2022-10-06 17:38:08.000000 fabric_fim-1.4.7/fim/graph/networkx_mixin.py
--rw-r--r--   0 ibaldin    (502) staff       (20)    42040 2023-04-05 20:55:22.000000 fabric_fim-1.4.7/fim/graph/networkx_property_graph.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     8354 2022-10-07 03:05:34.000000 fabric_fim-1.4.7/fim/graph/networkx_property_graph_disjoint.py
-drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-04-07 20:53:02.631858 fabric_fim-1.4.7/fim/graph/resources/
--rw-r--r--   0 ibaldin    (502) staff       (20)        1 2020-09-02 18:32:04.000000 fabric_fim-1.4.7/fim/graph/resources/__init__.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     4484 2021-05-25 21:09:37.000000 fabric_fim-1.4.7/fim/graph/resources/abc_adm.py
--rw-r--r--   0 ibaldin    (502) staff       (20)    13570 2023-04-05 20:55:22.000000 fabric_fim-1.4.7/fim/graph/resources/abc_arm.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     2991 2022-02-18 19:27:15.000000 fabric_fim-1.4.7/fim/graph/resources/abc_bqm.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     4547 2021-03-31 01:14:29.000000 fabric_fim-1.4.7/fim/graph/resources/abc_cbm.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     2297 2021-03-07 22:42:30.000000 fabric_fim-1.4.7/fim/graph/resources/neo4j_adm.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     2106 2021-05-25 21:09:37.000000 fabric_fim-1.4.7/fim/graph/resources/neo4j_arm.py
--rw-r--r--   0 ibaldin    (502) staff       (20)    18425 2023-04-05 20:55:22.000000 fabric_fim-1.4.7/fim/graph/resources/neo4j_cbm.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     5017 2022-02-18 19:27:15.000000 fabric_fim-1.4.7/fim/graph/resources/networkx_abqm.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     2341 2021-03-07 22:42:30.000000 fabric_fim-1.4.7/fim/graph/resources/networkx_adm.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     2122 2021-05-25 21:09:37.000000 fabric_fim-1.4.7/fim/graph/resources/networkx_arm.py
-drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-04-07 20:53:02.640574 fabric_fim-1.4.7/fim/graph/slices/
--rw-r--r--   0 ibaldin    (502) staff       (20)        1 2020-09-02 18:32:24.000000 fabric_fim-1.4.7/fim/graph/slices/__init__.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     8223 2022-02-18 19:27:15.000000 fabric_fim-1.4.7/fim/graph/slices/abc_asm.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     3713 2021-06-04 19:43:14.000000 fabric_fim-1.4.7/fim/graph/slices/neo4j_asm.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     4298 2021-06-04 19:43:14.000000 fabric_fim-1.4.7/fim/graph/slices/networkx_asm.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     8615 2021-03-03 19:57:54.000000 fabric_fim-1.4.7/fim/graph/typed_tuples.py
-drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-04-07 20:53:02.641525 fabric_fim-1.4.7/fim/logging/
--rw-r--r--   0 ibaldin    (502) staff       (20)        0 2023-02-02 01:41:56.000000 fabric_fim-1.4.7/fim/logging/__init__.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     9071 2023-02-02 01:41:56.000000 fabric_fim-1.4.7/fim/logging/log_collector.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     9555 2021-03-24 00:18:51.000000 fabric_fim-1.4.7/fim/pluggable.py
-drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-04-07 20:53:02.659857 fabric_fim-1.4.7/fim/slivers/
--rw-r--r--   0 ibaldin    (502) staff       (20)      217 2021-06-14 18:36:21.000000 fabric_fim-1.4.7/fim/slivers/__init__.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     3641 2023-02-02 01:41:56.000000 fabric_fim-1.4.7/fim/slivers/attached_components.py
--rw-r--r--   0 ibaldin    (502) staff       (20)    13021 2023-02-02 01:41:56.000000 fabric_fim-1.4.7/fim/slivers/base_sliver.py
--rw-r--r--   0 ibaldin    (502) staff       (20)    24088 2023-04-05 22:29:04.000000 fabric_fim-1.4.7/fim/slivers/capacities_labels.py
--rw-r--r--   0 ibaldin    (502) staff       (20)    11269 2023-04-05 20:55:22.000000 fabric_fim-1.4.7/fim/slivers/component_catalog.py
-drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-04-07 20:53:02.661737 fabric_fim-1.4.7/fim/slivers/data/
--rw-r--r--   0 ibaldin    (502) staff       (20)        1 2021-03-03 19:57:54.000000 fabric_fim-1.4.7/fim/slivers/data/__init__.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     1657 2023-04-05 20:55:22.000000 fabric_fim-1.4.7/fim/slivers/data/component_catalog.json
--rw-r--r--   0 ibaldin    (502) staff       (20)    76943 2022-09-10 21:18:41.000000 fabric_fim-1.4.7/fim/slivers/data/instance_sizes.json
--rw-r--r--   0 ibaldin    (502) staff       (20)    23524 2022-02-18 19:27:15.000000 fabric_fim-1.4.7/fim/slivers/delegations.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     3593 2022-02-18 19:27:15.000000 fabric_fim-1.4.7/fim/slivers/gateway.py
--rw-r--r--   0 ibaldin    (502) staff       (20)      919 2021-06-29 20:04:13.000000 fabric_fim-1.4.7/fim/slivers/identifiers.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     3444 2022-02-18 19:27:15.000000 fabric_fim-1.4.7/fim/slivers/instance_catalog.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     3225 2023-02-02 01:41:56.000000 fabric_fim-1.4.7/fim/slivers/interface_info.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     2702 2021-09-22 14:46:40.000000 fabric_fim-1.4.7/fim/slivers/json.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     3869 2023-02-02 01:41:56.000000 fabric_fim-1.4.7/fim/slivers/json_data.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     5983 2023-02-02 01:41:56.000000 fabric_fim-1.4.7/fim/slivers/maintenance_mode.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     1566 2021-03-03 19:57:54.000000 fabric_fim-1.4.7/fim/slivers/network_attached_storage.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     3910 2023-02-02 01:41:56.000000 fabric_fim-1.4.7/fim/slivers/network_link.py
--rw-r--r--   0 ibaldin    (502) staff       (20)    10209 2023-02-02 01:41:56.000000 fabric_fim-1.4.7/fim/slivers/network_node.py
--rw-r--r--   0 ibaldin    (502) staff       (20)    22042 2023-04-05 22:02:35.000000 fabric_fim-1.4.7/fim/slivers/network_service.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     6795 2021-06-04 19:43:14.000000 fabric_fim-1.4.7/fim/slivers/path_info.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     3024 2022-02-18 19:27:15.000000 fabric_fim-1.4.7/fim/slivers/tags.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     2622 2023-02-02 01:41:56.000000 fabric_fim-1.4.7/fim/slivers/topology_diff.py
-drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-04-07 20:53:02.670754 fabric_fim-1.4.7/fim/user/
--rw-r--r--   0 ibaldin    (502) staff       (20)     1914 2023-02-02 01:41:56.000000 fabric_fim-1.4.7/fim/user/__init__.py
--rw-r--r--   0 ibaldin    (502) staff       (20)    11730 2022-09-10 21:18:41.000000 fabric_fim-1.4.7/fim/user/component.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     5668 2022-09-10 21:18:41.000000 fabric_fim-1.4.7/fim/user/composite_node.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     7660 2023-02-02 01:41:56.000000 fabric_fim-1.4.7/fim/user/interface.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     8381 2022-09-10 21:18:41.000000 fabric_fim-1.4.7/fim/user/link.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     1219 2021-03-03 19:57:54.000000 fabric_fim-1.4.7/fim/user/measurement.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     9668 2023-04-05 18:48:29.000000 fabric_fim-1.4.7/fim/user/model_element.py
--rw-r--r--   0 ibaldin    (502) staff       (20)    29219 2023-04-05 22:02:45.000000 fabric_fim-1.4.7/fim/user/network_service.py
--rw-r--r--   0 ibaldin    (502) staff       (20)    22636 2023-02-14 21:58:39.000000 fabric_fim-1.4.7/fim/user/node.py
--rw-r--r--   0 ibaldin    (502) staff       (20)    58158 2023-02-14 21:58:39.000000 fabric_fim-1.4.7/fim/user/topology.py
--rw-r--r--   0 ibaldin    (502) staff       (20)      595 2021-03-13 20:40:37.000000 fabric_fim-1.4.7/fim/view_only_dict.py
--rw-r--r--   0 ibaldin    (502) staff       (20)      118 2023-02-02 01:41:56.000000 fabric_fim-1.4.7/requirements.txt
--rw-r--r--   0 ibaldin    (502) staff       (20)       38 2023-04-07 20:53:02.673324 fabric_fim-1.4.7/setup.cfg
--rw-r--r--   0 ibaldin    (502) staff       (20)      874 2023-02-02 01:41:56.000000 fabric_fim-1.4.7/setup.py
-drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-04-07 20:53:02.671686 fabric_fim-1.4.7/test/
--rw-r--r--   0 ibaldin    (502) staff       (20)      654 2022-02-18 19:27:15.000000 fabric_fim-1.4.7/test/test_load.py
-drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-04-07 20:53:02.672244 fabric_fim-1.4.7/util/
--rw-r--r--   0 ibaldin    (502) staff       (20)    14115 2023-04-05 20:55:22.000000 fabric_fim-1.4.7/util/fim_util.py
+drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-04-08 04:38:05.352826 fabric_fim-1.4.9/
+-rw-r--r--   0 ibaldin    (502) staff       (20)       26 2020-07-24 21:42:44.000000 fabric_fim-1.4.9/AUTHORS
+-rw-r--r--   0 ibaldin    (502) staff       (20)     1071 2020-07-14 22:09:49.000000 fabric_fim-1.4.9/LICENSE
+-rw-r--r--   0 ibaldin    (502) staff       (20)      146 2022-04-27 22:22:19.000000 fabric_fim-1.4.9/MANIFEST.in
+-rw-r--r--   0 ibaldin    (502) staff       (20)    11437 2023-04-08 04:38:05.352150 fabric_fim-1.4.9/PKG-INFO
+-rw-r--r--   0 ibaldin    (502) staff       (20)    10990 2023-04-05 20:55:22.000000 fabric_fim-1.4.9/README.md
+drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-04-08 04:38:05.300879 fabric_fim-1.4.9/fabric_fim.egg-info/
+-rw-r--r--   0 ibaldin    (502) staff       (20)    11437 2023-04-08 04:38:05.000000 fabric_fim-1.4.9/fabric_fim.egg-info/PKG-INFO
+-rw-r--r--   0 ibaldin    (502) staff       (20)     2324 2023-04-08 04:38:05.000000 fabric_fim-1.4.9/fabric_fim.egg-info/SOURCES.txt
+-rw-r--r--   0 ibaldin    (502) staff       (20)        1 2023-04-08 04:38:05.000000 fabric_fim-1.4.9/fabric_fim.egg-info/dependency_links.txt
+-rw-r--r--   0 ibaldin    (502) staff       (20)      118 2023-04-08 04:38:05.000000 fabric_fim-1.4.9/fabric_fim.egg-info/requires.txt
+-rw-r--r--   0 ibaldin    (502) staff       (20)        4 2023-04-08 04:38:05.000000 fabric_fim-1.4.9/fabric_fim.egg-info/top_level.txt
+drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-04-08 04:38:05.302372 fabric_fim-1.4.9/fim/
+-rw-r--r--   0 ibaldin    (502) staff       (20)       22 2023-04-08 04:37:46.000000 fabric_fim-1.4.9/fim/__init__.py
+drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-04-08 04:38:05.304078 fabric_fim-1.4.9/fim/authz/
+-rw-r--r--   0 ibaldin    (502) staff       (20)        1 2022-04-27 22:22:19.000000 fabric_fim-1.4.9/fim/authz/__init__.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)    16139 2023-02-02 01:41:56.000000 fabric_fim-1.4.9/fim/authz/attribute_collector.py
+drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-04-08 04:38:05.311071 fabric_fim-1.4.9/fim/graph/
+-rw-r--r--   0 ibaldin    (502) staff       (20)        1 2020-09-02 18:31:38.000000 fabric_fim-1.4.9/fim/graph/__init__.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)    69794 2023-04-08 04:33:53.000000 fabric_fim-1.4.9/fim/graph/abc_property_graph.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)     4093 2023-02-02 01:41:56.000000 fabric_fim-1.4.9/fim/graph/abc_property_graph_constants.py
+drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-04-08 04:38:05.315925 fabric_fim-1.4.9/fim/graph/data/
+-rw-r--r--   0 ibaldin    (502) staff       (20)        1 2020-08-18 21:34:07.000000 fabric_fim-1.4.9/fim/graph/data/__init__.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)      283 2020-09-03 22:10:53.000000 fabric_fim-1.4.9/fim/graph/data/capacity_types.json
+-rw-r--r--   0 ibaldin    (502) staff       (20)      100 2020-08-27 20:41:23.000000 fabric_fim-1.4.9/fim/graph/data/constraint_types.json
+-rw-r--r--   0 ibaldin    (502) staff       (20)     3829 2023-04-05 20:55:22.000000 fabric_fim-1.4.9/fim/graph/data/graph_validation_rules.json
+-rw-r--r--   0 ibaldin    (502) staff       (20)      547 2020-09-03 22:10:39.000000 fabric_fim-1.4.9/fim/graph/data/label_types.json
+-rw-r--r--   0 ibaldin    (502) staff       (20)       91 2020-08-27 20:40:54.000000 fabric_fim-1.4.9/fim/graph/data/location_types.json
+-rw-r--r--   0 ibaldin    (502) staff       (20)      367 2021-05-25 21:09:37.000000 fabric_fim-1.4.9/fim/graph/data/neo4j_indexes.json
+-rw-r--r--   0 ibaldin    (502) staff       (20)    43529 2023-04-08 04:34:03.000000 fabric_fim-1.4.9/fim/graph/neo4j_property_graph.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)     6160 2022-10-06 17:38:08.000000 fabric_fim-1.4.9/fim/graph/networkx_mixin.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)    42098 2023-04-08 04:33:57.000000 fabric_fim-1.4.9/fim/graph/networkx_property_graph.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)     8354 2022-10-07 03:05:34.000000 fabric_fim-1.4.9/fim/graph/networkx_property_graph_disjoint.py
+drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-04-08 04:38:05.326417 fabric_fim-1.4.9/fim/graph/resources/
+-rw-r--r--   0 ibaldin    (502) staff       (20)        1 2020-09-02 18:32:04.000000 fabric_fim-1.4.9/fim/graph/resources/__init__.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)     4484 2021-05-25 21:09:37.000000 fabric_fim-1.4.9/fim/graph/resources/abc_adm.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)    13570 2023-04-05 20:55:22.000000 fabric_fim-1.4.9/fim/graph/resources/abc_arm.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)     2991 2022-02-18 19:27:15.000000 fabric_fim-1.4.9/fim/graph/resources/abc_bqm.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)     4547 2021-03-31 01:14:29.000000 fabric_fim-1.4.9/fim/graph/resources/abc_cbm.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)     2297 2021-03-07 22:42:30.000000 fabric_fim-1.4.9/fim/graph/resources/neo4j_adm.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)     2106 2021-05-25 21:09:37.000000 fabric_fim-1.4.9/fim/graph/resources/neo4j_arm.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)    18425 2023-04-05 20:55:22.000000 fabric_fim-1.4.9/fim/graph/resources/neo4j_cbm.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)     5017 2022-02-18 19:27:15.000000 fabric_fim-1.4.9/fim/graph/resources/networkx_abqm.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)     2341 2021-03-07 22:42:30.000000 fabric_fim-1.4.9/fim/graph/resources/networkx_adm.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)     2122 2021-05-25 21:09:37.000000 fabric_fim-1.4.9/fim/graph/resources/networkx_arm.py
+drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-04-08 04:38:05.329026 fabric_fim-1.4.9/fim/graph/slices/
+-rw-r--r--   0 ibaldin    (502) staff       (20)        1 2020-09-02 18:32:24.000000 fabric_fim-1.4.9/fim/graph/slices/__init__.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)     8223 2022-02-18 19:27:15.000000 fabric_fim-1.4.9/fim/graph/slices/abc_asm.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)     3713 2021-06-04 19:43:14.000000 fabric_fim-1.4.9/fim/graph/slices/neo4j_asm.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)     4298 2021-06-04 19:43:14.000000 fabric_fim-1.4.9/fim/graph/slices/networkx_asm.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)     8615 2021-03-03 19:57:54.000000 fabric_fim-1.4.9/fim/graph/typed_tuples.py
+drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-04-08 04:38:05.329524 fabric_fim-1.4.9/fim/logging/
+-rw-r--r--   0 ibaldin    (502) staff       (20)        0 2023-02-02 01:41:56.000000 fabric_fim-1.4.9/fim/logging/__init__.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)     9071 2023-02-02 01:41:56.000000 fabric_fim-1.4.9/fim/logging/log_collector.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)     9555 2021-03-24 00:18:51.000000 fabric_fim-1.4.9/fim/pluggable.py
+drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-04-08 04:38:05.340823 fabric_fim-1.4.9/fim/slivers/
+-rw-r--r--   0 ibaldin    (502) staff       (20)      217 2021-06-14 18:36:21.000000 fabric_fim-1.4.9/fim/slivers/__init__.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)     3641 2023-02-02 01:41:56.000000 fabric_fim-1.4.9/fim/slivers/attached_components.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)    13021 2023-02-02 01:41:56.000000 fabric_fim-1.4.9/fim/slivers/base_sliver.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)    24078 2023-04-08 04:20:22.000000 fabric_fim-1.4.9/fim/slivers/capacities_labels.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)    11269 2023-04-05 20:55:22.000000 fabric_fim-1.4.9/fim/slivers/component_catalog.py
+drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-04-08 04:38:05.342257 fabric_fim-1.4.9/fim/slivers/data/
+-rw-r--r--   0 ibaldin    (502) staff       (20)        1 2021-03-03 19:57:54.000000 fabric_fim-1.4.9/fim/slivers/data/__init__.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)     1657 2023-04-05 20:55:22.000000 fabric_fim-1.4.9/fim/slivers/data/component_catalog.json
+-rw-r--r--   0 ibaldin    (502) staff       (20)    76943 2022-09-10 21:18:41.000000 fabric_fim-1.4.9/fim/slivers/data/instance_sizes.json
+-rw-r--r--   0 ibaldin    (502) staff       (20)    23524 2022-02-18 19:27:15.000000 fabric_fim-1.4.9/fim/slivers/delegations.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)     3593 2022-02-18 19:27:15.000000 fabric_fim-1.4.9/fim/slivers/gateway.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)      919 2021-06-29 20:04:13.000000 fabric_fim-1.4.9/fim/slivers/identifiers.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)     3444 2022-02-18 19:27:15.000000 fabric_fim-1.4.9/fim/slivers/instance_catalog.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)     3225 2023-02-02 01:41:56.000000 fabric_fim-1.4.9/fim/slivers/interface_info.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)     2702 2021-09-22 14:46:40.000000 fabric_fim-1.4.9/fim/slivers/json.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)     3869 2023-02-02 01:41:56.000000 fabric_fim-1.4.9/fim/slivers/json_data.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)     5983 2023-02-02 01:41:56.000000 fabric_fim-1.4.9/fim/slivers/maintenance_mode.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)     1566 2021-03-03 19:57:54.000000 fabric_fim-1.4.9/fim/slivers/network_attached_storage.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)     3910 2023-02-02 01:41:56.000000 fabric_fim-1.4.9/fim/slivers/network_link.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)    10209 2023-02-02 01:41:56.000000 fabric_fim-1.4.9/fim/slivers/network_node.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)    22042 2023-04-05 22:02:35.000000 fabric_fim-1.4.9/fim/slivers/network_service.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)     6795 2021-06-04 19:43:14.000000 fabric_fim-1.4.9/fim/slivers/path_info.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)     3024 2022-02-18 19:27:15.000000 fabric_fim-1.4.9/fim/slivers/tags.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)     2622 2023-02-02 01:41:56.000000 fabric_fim-1.4.9/fim/slivers/topology_diff.py
+drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-04-08 04:38:05.349853 fabric_fim-1.4.9/fim/user/
+-rw-r--r--   0 ibaldin    (502) staff       (20)     1914 2023-02-02 01:41:56.000000 fabric_fim-1.4.9/fim/user/__init__.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)    11730 2022-09-10 21:18:41.000000 fabric_fim-1.4.9/fim/user/component.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)     5668 2022-09-10 21:18:41.000000 fabric_fim-1.4.9/fim/user/composite_node.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)     7660 2023-02-02 01:41:56.000000 fabric_fim-1.4.9/fim/user/interface.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)     8381 2022-09-10 21:18:41.000000 fabric_fim-1.4.9/fim/user/link.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)     1219 2021-03-03 19:57:54.000000 fabric_fim-1.4.9/fim/user/measurement.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)     9668 2023-04-05 18:48:29.000000 fabric_fim-1.4.9/fim/user/model_element.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)    29219 2023-04-05 22:02:45.000000 fabric_fim-1.4.9/fim/user/network_service.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)    22636 2023-02-14 21:58:39.000000 fabric_fim-1.4.9/fim/user/node.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)    58158 2023-02-14 21:58:39.000000 fabric_fim-1.4.9/fim/user/topology.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)      595 2021-03-13 20:40:37.000000 fabric_fim-1.4.9/fim/view_only_dict.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)      118 2023-02-02 01:41:56.000000 fabric_fim-1.4.9/requirements.txt
+-rw-r--r--   0 ibaldin    (502) staff       (20)       38 2023-04-08 04:38:05.352946 fabric_fim-1.4.9/setup.cfg
+-rw-r--r--   0 ibaldin    (502) staff       (20)      874 2023-02-02 01:41:56.000000 fabric_fim-1.4.9/setup.py
+drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-04-08 04:38:05.350899 fabric_fim-1.4.9/test/
+-rw-r--r--   0 ibaldin    (502) staff       (20)      654 2022-02-18 19:27:15.000000 fabric_fim-1.4.9/test/test_load.py
+drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-04-08 04:38:05.351453 fabric_fim-1.4.9/util/
+-rw-r--r--   0 ibaldin    (502) staff       (20)    14115 2023-04-05 20:55:22.000000 fabric_fim-1.4.9/util/fim_util.py
```

### Comparing `fabric_fim-1.4.7/LICENSE` & `fabric_fim-1.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.7/PKG-INFO` & `fabric_fim-1.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fabric_fim
-Version: 1.4.7
+Version: 1.4.9
 Summary: FABRIC Information Model Library
 Home-page: https://github.com/fabric-testbed/InformationModel
 Author: Ilya Baldin, Komal Thareja
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `fabric_fim-1.4.7/README.md` & `fabric_fim-1.4.9/README.md`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.7/fabric_fim.egg-info/PKG-INFO` & `fabric_fim-1.4.9/fabric_fim.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fabric-fim
-Version: 1.4.7
+Version: 1.4.9
 Summary: FABRIC Information Model Library
 Home-page: https://github.com/fabric-testbed/InformationModel
 Author: Ilya Baldin, Komal Thareja
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `fabric_fim-1.4.7/fabric_fim.egg-info/SOURCES.txt` & `fabric_fim-1.4.9/fabric_fim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.7/fim/authz/attribute_collector.py` & `fabric_fim-1.4.9/fim/authz/attribute_collector.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.7/fim/graph/abc_property_graph.py` & `fabric_fim-1.4.9/fim/graph/abc_property_graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,17 +125,18 @@
         else:
             self.log = logger
 
     def get_graph_id(self):
         return self.graph_id
 
     @abstractmethod
-    def validate_graph(self) -> None:
+    def validate_graph(self, validate_json: bool = True) -> None:
         """
         validate graph according to a built-in set of rules
+        :validate_json: - should JSON fields be validated? defaults True
         :return: - None,
         """
 
     @abstractmethod
     def delete_graph(self) -> None:
         """
         delete a graph from the database
```

### Comparing `fabric_fim-1.4.7/fim/graph/abc_property_graph_constants.py` & `fabric_fim-1.4.9/fim/graph/abc_property_graph_constants.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.7/fim/graph/data/graph_validation_rules.json` & `fabric_fim-1.4.9/fim/graph/data/graph_validation_rules.json`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.7/fim/graph/data/label_types.json` & `fabric_fim-1.4.9/fim/graph/data/label_types.json`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.7/fim/graph/neo4j_property_graph.py` & `fabric_fim-1.4.9/fim/graph/neo4j_property_graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,23 +74,24 @@
                 if single is None:
                     return
                 v = single.value()
                 # print("Rule {}, value {}".format(r['msg'], v))
                 if v is False:
                     raise PropertyGraphImportException(graph_id=self.graph_id, msg=r['msg'])
 
-    def validate_graph(self) -> None:
+    def validate_graph(self, validate_json: bool = True) -> None:
         """
         validate a graph from a built-in set of rules
         :return:
         """
         self.log.info(f'Applying validation rules to graph {self.graph_id}')
         self._validate_graph(os.path.join(os.path.dirname(__file__), 'data', 'graph_validation_rules.json'))
-        self.log.info(f'Checking JSON properties of graph {self.graph_id}')
-        self._validate_all_json_properties()
+        if validate_json:
+            self.log.info(f'Checking JSON properties of graph {self.graph_id}')
+            self._validate_all_json_properties()
 
     def delete_graph(self) -> None:
         """
         Delete a graph from Neo4j
         :return:
         """
         self.log.debug(f'Deleting graph {self.graph_id}')
```

### Comparing `fabric_fim-1.4.7/fim/graph/networkx_mixin.py` & `fabric_fim-1.4.9/fim/graph/networkx_mixin.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.7/fim/graph/networkx_property_graph.py` & `fabric_fim-1.4.9/fim/graph/networkx_property_graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,20 +56,21 @@
         :param importer: should be an instance of NetworkXGraphImporter
         :param logger: optional
         """
         super().__init__(graph_id=graph_id, importer=importer, logger=logger)
         assert isinstance(importer, NetworkXGraphImporter)
         self.storage = importer.storage
 
-    def validate_graph(self) -> None:
+    def validate_graph(self, validate_json: bool = True) -> None:
         """
         NetworkX offers limited opportunities for query/validation
         :return:
         """
-        self._validate_all_json_properties()
+        if validate_json:
+            self._validate_all_json_properties()
         # check that all nodes and links have 'Class' property
         for n in self.storage.get_graph(self.graph_id).nodes:
             if self.storage.get_graph(self.graph_id).nodes[n].get(ABCPropertyGraph.PROP_CLASS, None) is None:
                 raise PropertyGraphImportException(graph_id=self.graph_id,
                                                    msg="Some nodes are missing 'Class' property")
         for e in self.storage.get_graph(self.graph_id).edges:
             if self.storage.get_graph(self.graph_id).edges[e].get(ABCPropertyGraph.PROP_CLASS, None) is None:
```

### Comparing `fabric_fim-1.4.7/fim/graph/networkx_property_graph_disjoint.py` & `fabric_fim-1.4.9/fim/graph/networkx_property_graph_disjoint.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.7/fim/graph/resources/abc_adm.py` & `fabric_fim-1.4.9/fim/graph/resources/abc_adm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.7/fim/graph/resources/abc_arm.py` & `fabric_fim-1.4.9/fim/graph/resources/abc_arm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.7/fim/graph/resources/abc_bqm.py` & `fabric_fim-1.4.9/fim/graph/resources/abc_bqm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.7/fim/graph/resources/abc_cbm.py` & `fabric_fim-1.4.9/fim/graph/resources/abc_cbm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.7/fim/graph/resources/neo4j_adm.py` & `fabric_fim-1.4.9/fim/graph/resources/neo4j_adm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.7/fim/graph/resources/neo4j_arm.py` & `fabric_fim-1.4.9/fim/graph/resources/neo4j_arm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.7/fim/graph/resources/neo4j_cbm.py` & `fabric_fim-1.4.9/fim/graph/resources/neo4j_cbm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.7/fim/graph/resources/networkx_abqm.py` & `fabric_fim-1.4.9/fim/graph/resources/networkx_abqm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.7/fim/graph/resources/networkx_adm.py` & `fabric_fim-1.4.9/fim/graph/resources/networkx_adm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.7/fim/graph/resources/networkx_arm.py` & `fabric_fim-1.4.9/fim/graph/resources/networkx_arm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.7/fim/graph/slices/abc_asm.py` & `fabric_fim-1.4.9/fim/graph/slices/abc_asm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.7/fim/graph/slices/neo4j_asm.py` & `fabric_fim-1.4.9/fim/graph/slices/neo4j_asm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.7/fim/graph/slices/networkx_asm.py` & `fabric_fim-1.4.9/fim/graph/slices/networkx_asm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.7/fim/graph/typed_tuples.py` & `fabric_fim-1.4.9/fim/graph/typed_tuples.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.7/fim/logging/log_collector.py` & `fabric_fim-1.4.9/fim/logging/log_collector.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.7/fim/pluggable.py` & `fabric_fim-1.4.9/fim/pluggable.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.7/fim/slivers/attached_components.py` & `fabric_fim-1.4.9/fim/slivers/attached_components.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.7/fim/slivers/base_sliver.py` & `fabric_fim-1.4.9/fim/slivers/base_sliver.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.7/fim/slivers/capacities_labels.py` & `fabric_fim-1.4.9/fim/slivers/capacities_labels.py`

 * *Files 0% similar despite different names*

```diff
@@ -581,15 +581,15 @@
     """
     JSON-ified representation of various flags that can be attached to slivers
     """
     def __init__(self, **kwargs):
         self.auto_config = False # primarily for interfaces
         self.auto_mount = False # primarily for storage components
         self.ipv4_management = False # request ipv4 management IP
-        self.ptp_available = False # for advertisements of nodes/sites
+        self.ptp = False # for advertisements of nodes/sites
         self._set_fields(**kwargs)
 
     def _set_fields(self, **kwargs):
         for k, v in kwargs.items():
             assert v is not None
             assert isinstance(v, bool)
             try:
```

### Comparing `fabric_fim-1.4.7/fim/slivers/component_catalog.py` & `fabric_fim-1.4.9/fim/slivers/component_catalog.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.7/fim/slivers/data/component_catalog.json` & `fabric_fim-1.4.9/fim/slivers/data/component_catalog.json`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.7/fim/slivers/data/instance_sizes.json` & `fabric_fim-1.4.9/fim/slivers/data/instance_sizes.json`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.7/fim/slivers/delegations.py` & `fabric_fim-1.4.9/fim/slivers/delegations.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.7/fim/slivers/gateway.py` & `fabric_fim-1.4.9/fim/slivers/gateway.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.7/fim/slivers/identifiers.py` & `fabric_fim-1.4.9/fim/slivers/identifiers.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.7/fim/slivers/instance_catalog.py` & `fabric_fim-1.4.9/fim/slivers/instance_catalog.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.7/fim/slivers/interface_info.py` & `fabric_fim-1.4.9/fim/slivers/interface_info.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.7/fim/slivers/json.py` & `fabric_fim-1.4.9/fim/slivers/json.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.7/fim/slivers/json_data.py` & `fabric_fim-1.4.9/fim/slivers/json_data.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.7/fim/slivers/maintenance_mode.py` & `fabric_fim-1.4.9/fim/slivers/maintenance_mode.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.7/fim/slivers/network_attached_storage.py` & `fabric_fim-1.4.9/fim/slivers/network_attached_storage.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.7/fim/slivers/network_link.py` & `fabric_fim-1.4.9/fim/slivers/network_link.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.7/fim/slivers/network_node.py` & `fabric_fim-1.4.9/fim/slivers/network_node.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.7/fim/slivers/network_service.py` & `fabric_fim-1.4.9/fim/slivers/network_service.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.7/fim/slivers/path_info.py` & `fabric_fim-1.4.9/fim/slivers/path_info.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.7/fim/slivers/tags.py` & `fabric_fim-1.4.9/fim/slivers/tags.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.7/fim/slivers/topology_diff.py` & `fabric_fim-1.4.9/fim/slivers/topology_diff.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.7/fim/user/__init__.py` & `fabric_fim-1.4.9/fim/user/__init__.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.7/fim/user/component.py` & `fabric_fim-1.4.9/fim/user/component.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.7/fim/user/composite_node.py` & `fabric_fim-1.4.9/fim/user/composite_node.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.7/fim/user/interface.py` & `fabric_fim-1.4.9/fim/user/interface.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.7/fim/user/link.py` & `fabric_fim-1.4.9/fim/user/link.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.7/fim/user/measurement.py` & `fabric_fim-1.4.9/fim/user/measurement.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.7/fim/user/model_element.py` & `fabric_fim-1.4.9/fim/user/model_element.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.7/fim/user/network_service.py` & `fabric_fim-1.4.9/fim/user/network_service.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.7/fim/user/node.py` & `fabric_fim-1.4.9/fim/user/node.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.7/fim/user/topology.py` & `fabric_fim-1.4.9/fim/user/topology.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.7/fim/view_only_dict.py` & `fabric_fim-1.4.9/fim/view_only_dict.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.7/setup.py` & `fabric_fim-1.4.9/setup.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.7/test/test_load.py` & `fabric_fim-1.4.9/test/test_load.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.7/util/fim_util.py` & `fabric_fim-1.4.9/util/fim_util.py`

 * *Files identical despite different names*

