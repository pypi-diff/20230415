# Comparing `tmp/ttp-0.9.2.tar.gz` & `tmp/ttp-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ttp-0.9.2.tar", max compression
+gzip compressed data, was "ttp-0.9.3.tar", max compression
```

## Comparing `ttp-0.9.2.tar` & `ttp-0.9.3.tar`

### file list

```diff
@@ -1,91 +1,90 @@
--rw-r--r--   0        0        0     1065 2022-10-02 22:27:01.097014 ttp-0.9.2/LICENSE
--rw-r--r--   0        0        0     4036 2022-12-04 01:27:17.358548 ttp-0.9.2/pyproject.toml
--rw-r--r--   0        0        0     6414 2022-10-02 12:16:11.776605 ttp-0.9.2/README.md
--rw-r--r--   0        0        0      428 2022-12-04 01:28:12.958766 ttp-0.9.2/ttp/__init__.py
--rw-r--r--   0        0        0        0 2022-10-02 11:16:02.806688 ttp-0.9.2/ttp/formatters/__init__.py
--rw-r--r--   0        0        0      891 2022-10-02 22:39:44.441452 ttp-0.9.2/ttp/formatters/csv_formatter.py
--rw-r--r--   0        0        0     2519 2022-10-02 12:39:58.451379 ttp-0.9.2/ttp/formatters/excel_formatter.py
--rw-r--r--   0        0        0      777 2022-10-02 22:32:58.697313 ttp-0.9.2/ttp/formatters/jinja2_formatter.py
--rw-r--r--   0        0        0      243 2022-10-02 12:00:55.767339 ttp-0.9.2/ttp/formatters/json_formatter.py
--rw-r--r--   0        0        0     1545 2022-10-02 22:05:37.297996 ttp-0.9.2/ttp/formatters/n2g_formatter.py
--rw-r--r--   0        0        0      201 2022-10-02 11:46:07.107045 ttp-0.9.2/ttp/formatters/pprint_formatter.py
--rw-r--r--   0        0        0      115 2022-10-02 11:24:00.008627 ttp-0.9.2/ttp/formatters/raw_formatter.py
--rw-r--r--   0        0        0     2092 2022-10-02 21:54:55.247354 ttp-0.9.2/ttp/formatters/table_formatter.py
--rw-r--r--   0        0        0      812 2022-10-02 22:35:06.089841 ttp-0.9.2/ttp/formatters/tabulate_formatter.py
--rw-r--r--   0        0        0      493 2022-10-02 22:06:16.739838 ttp-0.9.2/ttp/formatters/yaml_formatter.py
--rw-r--r--   0        0        0        0 2022-10-02 11:16:02.810438 ttp-0.9.2/ttp/group/__init__.py
--rw-r--r--   0        0        0      358 2022-10-02 12:32:17.655647 ttp-0.9.2/ttp/group/contains.py
--rw-r--r--   0        0        0      338 2022-10-02 12:28:09.118285 ttp-0.9.2/ttp/group/contains_val.py
--rw-r--r--   0        0        0      376 2022-10-02 12:36:13.997743 ttp-0.9.2/ttp/group/containsall.py
--rw-r--r--   0        0        0      173 2022-10-02 11:36:49.239728 ttp-0.9.2/ttp/group/delete.py
--rw-r--r--   0        0        0      323 2022-10-02 12:24:23.165655 ttp-0.9.2/ttp/group/equal.py
--rw-r--r--   0        0        0      261 2022-10-02 12:06:43.385622 ttp-0.9.2/ttp/group/exclude.py
--rw-r--r--   0        0        0      415 2022-12-03 01:59:53.792168 ttp-0.9.2/ttp/group/exclude_val.py
--rw-r--r--   0        0        0      366 2022-10-02 12:34:00.830761 ttp-0.9.2/ttp/group/excludeall.py
--rw-r--r--   0        0        0      727 2022-10-02 22:29:03.282400 ttp-0.9.2/ttp/group/expand.py
--rw-r--r--   0        0        0     1303 2022-10-02 22:14:41.018871 ttp-0.9.2/ttp/group/itemize.py
--rw-r--r--   0        0        0      361 2022-10-02 12:32:57.284988 ttp-0.9.2/ttp/group/items2dict.py
--rw-r--r--   0        0        0     2526 2022-10-02 12:39:48.142079 ttp-0.9.2/ttp/group/lookup.py
--rw-r--r--   0        0        0      512 2022-10-02 22:09:01.851973 ttp-0.9.2/ttp/group/macro.py
--rw-r--r--   0        0        0      421 2022-10-02 21:54:34.639907 ttp-0.9.2/ttp/group/record.py
--rw-r--r--   0        0        0      686 2022-10-02 22:25:48.517202 ttp-0.9.2/ttp/group/set_.py
--rw-r--r--   0        0        0      671 2022-10-02 22:24:36.018618 ttp-0.9.2/ttp/group/sformat.py
--rw-r--r--   0        0        0      686 2022-10-02 22:25:49.107690 ttp-0.9.2/ttp/group/to_converters.py
--rw-r--r--   0        0        0      386 2022-10-02 12:38:04.642781 ttp-0.9.2/ttp/group/to_ip.py
--rw-r--r--   0        0        0     2768 2022-12-03 02:00:16.317825 ttp-0.9.2/ttp/group/validate_cerberus.py
--rw-r--r--   0        0        0       79 2022-10-02 11:21:04.435047 ttp-0.9.2/ttp/group/void.py
--rw-r--r--   0        0        0        0 2022-10-02 11:16:02.790022 ttp-0.9.2/ttp/input/__init__.py
--rw-r--r--   0        0        0      606 2022-10-02 22:19:20.241356 ttp-0.9.2/ttp/input/commands.py
--rw-r--r--   0        0        0      350 2022-10-02 12:30:51.321783 ttp-0.9.2/ttp/input/macro.py
--rw-r--r--   0        0        0      124 2022-10-02 11:25:45.007132 ttp-0.9.2/ttp/input/test.py
--rw-r--r--   0        0        0        0 2022-10-02 11:16:02.776895 ttp-0.9.2/ttp/lookup/__init__.py
--rw-r--r--   0        0        0     1482 2022-10-02 22:07:38.694082 ttp-0.9.2/ttp/lookup/geoip2.py
--rw-r--r--   0        0        0        0 2022-10-02 11:16:02.799997 ttp-0.9.2/ttp/match/__init__.py
--rw-r--r--   0        0        0      153 2022-12-03 11:52:49.025726 ttp-0.9.2/ttp/match/copy_.py
--rw-r--r--   0        0        0      347 2022-12-03 01:58:48.838563 ttp-0.9.2/ttp/match/count.py
--rw-r--r--   0        0        0     2401 2022-10-02 12:41:34.803860 ttp-0.9.2/ttp/match/dns_lookups.py
--rw-r--r--   0        0        0     2975 2022-10-02 12:35:10.123040 ttp-0.9.2/ttp/match/geoip_lookup.py
--rw-r--r--   0        0        0     6080 2022-12-03 01:58:26.560255 ttp-0.9.2/ttp/match/ip.py
--rw-r--r--   0        0        0      697 2022-10-02 22:26:47.115914 ttp-0.9.2/ttp/match/item.py
--rw-r--r--   0        0        0       64 2022-10-02 11:20:31.576928 ttp-0.9.2/ttp/match/joinmatches.py
--rw-r--r--   0        0        0      248 2022-10-02 12:02:47.361627 ttp-0.9.2/ttp/match/let.py
--rw-r--r--   0        0        0     4237 2022-12-03 01:57:42.950828 ttp-0.9.2/ttp/match/lookup.py
--rw-r--r--   0        0        0      799 2022-10-02 22:34:23.774520 ttp-0.9.2/ttp/match/mac_eui.py
--rw-r--r--   0        0        0      522 2022-10-02 22:10:07.904632 ttp-0.9.2/ttp/match/macro.py
--rw-r--r--   0        0        0      110 2022-10-02 11:23:17.673227 ttp-0.9.2/ttp/match/raise_.py
--rw-r--r--   0        0        0     2084 2022-12-03 01:56:47.519349 ttp-0.9.2/ttp/match/re_.py
--rw-r--r--   0        0        0      141 2022-12-03 01:57:08.150264 ttp-0.9.2/ttp/match/record.py
--rw-r--r--   0        0        0      424 2022-12-03 01:57:21.703876 ttp-0.9.2/ttp/match/set_.py
--rw-r--r--   0        0        0     3251 2022-12-03 02:02:43.751562 ttp-0.9.2/ttp/match/string.py
--rw-r--r--   0        0        0     1036 2022-10-02 22:29:14.953215 ttp-0.9.2/ttp/match/to.py
--rw-r--r--   0        0        0     1249 2022-10-02 22:17:14.438625 ttp-0.9.2/ttp/match/unrange.py
--rw-r--r--   0        0        0     2560 2022-10-02 12:39:24.202585 ttp-0.9.2/ttp/match/uptimeparse.py
--rw-r--r--   0        0        0       79 2022-10-02 11:21:02.412304 ttp-0.9.2/ttp/match/void.py
--rw-r--r--   0        0        0        0 2022-10-02 11:16:02.802945 ttp-0.9.2/ttp/output/__init__.py
--rw-r--r--   0        0        0     3357 2022-10-02 12:32:02.924852 ttp-0.9.2/ttp/output/deepdiffer.py
--rw-r--r--   0        0        0      507 2022-10-02 22:08:21.766679 ttp-0.9.2/ttp/output/is_equal.py
--rw-r--r--   0        0        0      230 2022-10-02 11:56:47.370840 ttp-0.9.2/ttp/output/macro.py
--rw-r--r--   0        0        0     2210 2022-10-02 12:43:48.102403 ttp-0.9.2/ttp/output/transform.py
--rw-r--r--   0        0        0     2011 2022-10-02 21:56:01.269058 ttp-0.9.2/ttp/output/validate_cerberus.py
--rw-r--r--   0        0        0     8469 2022-10-02 12:10:13.579428 ttp-0.9.2/ttp/output/validate_yangson.py
--rw-r--r--   0        0        0        0 2022-10-02 11:16:02.787032 ttp-0.9.2/ttp/patterns/__init__.py
--rw-r--r--   0        0        0      593 2022-10-02 22:17:58.693165 ttp-0.9.2/ttp/patterns/get_pattern.py
--rw-r--r--   0        0        0        0 2022-10-02 11:16:02.793015 ttp-0.9.2/ttp/returners/__init__.py
--rw-r--r--   0        0        0     1680 2022-10-02 22:02:36.320460 ttp-0.9.2/ttp/returners/file_returner.py
--rw-r--r--   0        0        0      197 2022-10-02 11:44:50.079655 ttp-0.9.2/ttp/returners/self_returner.py
--rw-r--r--   0        0        0     2938 2022-10-02 12:35:24.240884 ttp-0.9.2/ttp/returners/syslog_returner.py
--rw-r--r--   0        0        0     1882 2022-10-02 21:58:21.128182 ttp-0.9.2/ttp/returners/terminal_returner.py
--rw-r--r--   0        0        0   155193 2022-12-04 01:28:20.833598 ttp-0.9.2/ttp/ttp.py
--rw-r--r--   0        0        0        0 2022-10-02 11:16:02.769368 ttp-0.9.2/ttp/utils/__init__.py
--rw-r--r--   0        0        0     2778 2022-10-02 12:36:46.909720 ttp-0.9.2/ttp/utils/get_attributes.py
--rw-r--r--   0        0        0      157 2022-10-02 11:32:16.246029 ttp-0.9.2/ttp/utils/guess.py
--rw-r--r--   0        0        0     1157 2022-10-02 22:21:07.735695 ttp-0.9.2/ttp/utils/load_python_exec_py2.py
--rw-r--r--   0        0        0      955 2022-10-02 22:36:33.000288 ttp-0.9.2/ttp/utils/load_python_exec_py3.py
--rw-r--r--   0        0        0    10511 2022-10-02 12:06:18.417379 ttp-0.9.2/ttp/utils/loaders.py
--rw-r--r--   0        0        0     1454 2022-10-02 22:08:49.259463 ttp-0.9.2/ttp/utils/quick_parse.py
--rw-r--r--   0        0        0        0 2022-10-02 11:16:02.814177 ttp-0.9.2/ttp/variable/__init__.py
--rw-r--r--   0        0        0       88 2022-10-02 11:21:26.955490 ttp-0.9.2/ttp/variable/getfilename.py
--rw-r--r--   0        0        0     1792 2022-10-02 21:59:56.076938 ttp-0.9.2/ttp/variable/gethostname.py
--rw-r--r--   0        0        0     1107 2022-10-02 22:24:21.974076 ttp-0.9.2/ttp/variable/time_funcs.py
--rw-r--r--   0        0        0     8579 2022-12-04 01:29:14.345458 ttp-0.9.2/setup.py
--rw-r--r--   0        0        0     9198 2022-12-04 01:29:14.345458 ttp-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2022-10-02 22:27:01.097014 ttp-0.9.3/LICENSE
+-rw-r--r--   0        0        0     4035 2023-04-15 08:58:06.792729 ttp-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0     6414 2022-10-02 12:16:11.776605 ttp-0.9.3/README.md
+-rw-r--r--   0        0        0      428 2023-04-14 23:57:06.307808 ttp-0.9.3/ttp/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-02 11:16:02.806688 ttp-0.9.3/ttp/formatters/__init__.py
+-rw-r--r--   0        0        0      891 2022-10-02 22:39:44.441452 ttp-0.9.3/ttp/formatters/csv_formatter.py
+-rw-r--r--   0        0        0     2519 2022-10-02 12:39:58.451379 ttp-0.9.3/ttp/formatters/excel_formatter.py
+-rw-r--r--   0        0        0      777 2022-10-02 22:32:58.697313 ttp-0.9.3/ttp/formatters/jinja2_formatter.py
+-rw-r--r--   0        0        0      243 2022-10-02 12:00:55.767339 ttp-0.9.3/ttp/formatters/json_formatter.py
+-rw-r--r--   0        0        0     1545 2022-10-02 22:05:37.297996 ttp-0.9.3/ttp/formatters/n2g_formatter.py
+-rw-r--r--   0        0        0      201 2022-10-02 11:46:07.107045 ttp-0.9.3/ttp/formatters/pprint_formatter.py
+-rw-r--r--   0        0        0      115 2022-10-02 11:24:00.008627 ttp-0.9.3/ttp/formatters/raw_formatter.py
+-rw-r--r--   0        0        0     2092 2022-10-02 21:54:55.247354 ttp-0.9.3/ttp/formatters/table_formatter.py
+-rw-r--r--   0        0        0      812 2022-10-02 22:35:06.089841 ttp-0.9.3/ttp/formatters/tabulate_formatter.py
+-rw-r--r--   0        0        0      493 2022-10-02 22:06:16.739838 ttp-0.9.3/ttp/formatters/yaml_formatter.py
+-rw-r--r--   0        0        0        0 2022-10-02 11:16:02.810438 ttp-0.9.3/ttp/group/__init__.py
+-rw-r--r--   0        0        0      358 2022-10-02 12:32:17.655647 ttp-0.9.3/ttp/group/contains.py
+-rw-r--r--   0        0        0      338 2022-10-02 12:28:09.118285 ttp-0.9.3/ttp/group/contains_val.py
+-rw-r--r--   0        0        0      376 2022-10-02 12:36:13.997743 ttp-0.9.3/ttp/group/containsall.py
+-rw-r--r--   0        0        0      173 2022-10-02 11:36:49.239728 ttp-0.9.3/ttp/group/delete.py
+-rw-r--r--   0        0        0      323 2022-10-02 12:24:23.165655 ttp-0.9.3/ttp/group/equal.py
+-rw-r--r--   0        0        0      261 2022-10-02 12:06:43.385622 ttp-0.9.3/ttp/group/exclude.py
+-rw-r--r--   0        0        0      415 2022-12-03 01:59:53.792168 ttp-0.9.3/ttp/group/exclude_val.py
+-rw-r--r--   0        0        0      366 2022-10-02 12:34:00.830761 ttp-0.9.3/ttp/group/excludeall.py
+-rw-r--r--   0        0        0      727 2022-10-02 22:29:03.282400 ttp-0.9.3/ttp/group/expand.py
+-rw-r--r--   0        0        0     1303 2022-10-02 22:14:41.018871 ttp-0.9.3/ttp/group/itemize.py
+-rw-r--r--   0        0        0      361 2022-10-02 12:32:57.284988 ttp-0.9.3/ttp/group/items2dict.py
+-rw-r--r--   0        0        0     2526 2022-10-02 12:39:48.142079 ttp-0.9.3/ttp/group/lookup.py
+-rw-r--r--   0        0        0      512 2022-10-02 22:09:01.851973 ttp-0.9.3/ttp/group/macro.py
+-rw-r--r--   0        0        0      421 2022-10-02 21:54:34.639907 ttp-0.9.3/ttp/group/record.py
+-rw-r--r--   0        0        0      686 2022-10-02 22:25:48.517202 ttp-0.9.3/ttp/group/set_.py
+-rw-r--r--   0        0        0      671 2022-10-02 22:24:36.018618 ttp-0.9.3/ttp/group/sformat.py
+-rw-r--r--   0        0        0      686 2022-10-02 22:25:49.107690 ttp-0.9.3/ttp/group/to_converters.py
+-rw-r--r--   0        0        0      386 2022-10-02 12:38:04.642781 ttp-0.9.3/ttp/group/to_ip.py
+-rw-r--r--   0        0        0     2768 2022-12-03 02:00:16.317825 ttp-0.9.3/ttp/group/validate_cerberus.py
+-rw-r--r--   0        0        0       79 2022-10-02 11:21:04.435047 ttp-0.9.3/ttp/group/void.py
+-rw-r--r--   0        0        0        0 2022-10-02 11:16:02.790022 ttp-0.9.3/ttp/input/__init__.py
+-rw-r--r--   0        0        0      606 2022-10-02 22:19:20.241356 ttp-0.9.3/ttp/input/commands.py
+-rw-r--r--   0        0        0      350 2022-10-02 12:30:51.321783 ttp-0.9.3/ttp/input/macro.py
+-rw-r--r--   0        0        0      124 2022-10-02 11:25:45.007132 ttp-0.9.3/ttp/input/test.py
+-rw-r--r--   0        0        0        0 2022-10-02 11:16:02.776895 ttp-0.9.3/ttp/lookup/__init__.py
+-rw-r--r--   0        0        0     1482 2022-10-02 22:07:38.694082 ttp-0.9.3/ttp/lookup/geoip2.py
+-rw-r--r--   0        0        0        0 2022-10-02 11:16:02.799997 ttp-0.9.3/ttp/match/__init__.py
+-rw-r--r--   0        0        0      153 2022-12-03 11:52:49.025726 ttp-0.9.3/ttp/match/copy_.py
+-rw-r--r--   0        0        0      347 2022-12-03 01:58:48.838563 ttp-0.9.3/ttp/match/count.py
+-rw-r--r--   0        0        0     2401 2022-10-02 12:41:34.803860 ttp-0.9.3/ttp/match/dns_lookups.py
+-rw-r--r--   0        0        0     2975 2022-10-02 12:35:10.123040 ttp-0.9.3/ttp/match/geoip_lookup.py
+-rw-r--r--   0        0        0     6080 2022-12-03 01:58:26.560255 ttp-0.9.3/ttp/match/ip.py
+-rw-r--r--   0        0        0      697 2022-10-02 22:26:47.115914 ttp-0.9.3/ttp/match/item.py
+-rw-r--r--   0        0        0       64 2022-10-02 11:20:31.576928 ttp-0.9.3/ttp/match/joinmatches.py
+-rw-r--r--   0        0        0      248 2022-10-02 12:02:47.361627 ttp-0.9.3/ttp/match/let.py
+-rw-r--r--   0        0        0     4237 2022-12-03 01:57:42.950828 ttp-0.9.3/ttp/match/lookup.py
+-rw-r--r--   0        0        0      799 2022-10-02 22:34:23.774520 ttp-0.9.3/ttp/match/mac_eui.py
+-rw-r--r--   0        0        0      522 2022-10-02 22:10:07.904632 ttp-0.9.3/ttp/match/macro.py
+-rw-r--r--   0        0        0      110 2022-10-02 11:23:17.673227 ttp-0.9.3/ttp/match/raise_.py
+-rw-r--r--   0        0        0     2084 2022-12-03 01:56:47.519349 ttp-0.9.3/ttp/match/re_.py
+-rw-r--r--   0        0        0      141 2022-12-03 01:57:08.150264 ttp-0.9.3/ttp/match/record.py
+-rw-r--r--   0        0        0      424 2022-12-03 01:57:21.703876 ttp-0.9.3/ttp/match/set_.py
+-rw-r--r--   0        0        0     3251 2022-12-03 02:02:43.751562 ttp-0.9.3/ttp/match/string.py
+-rw-r--r--   0        0        0     1036 2022-10-02 22:29:14.953215 ttp-0.9.3/ttp/match/to.py
+-rw-r--r--   0        0        0     1249 2022-10-02 22:17:14.438625 ttp-0.9.3/ttp/match/unrange.py
+-rw-r--r--   0        0        0     2560 2022-10-02 12:39:24.202585 ttp-0.9.3/ttp/match/uptimeparse.py
+-rw-r--r--   0        0        0       79 2022-10-02 11:21:02.412304 ttp-0.9.3/ttp/match/void.py
+-rw-r--r--   0        0        0        0 2022-10-02 11:16:02.802945 ttp-0.9.3/ttp/output/__init__.py
+-rw-r--r--   0        0        0     3357 2022-10-02 12:32:02.924852 ttp-0.9.3/ttp/output/deepdiffer.py
+-rw-r--r--   0        0        0      507 2022-10-02 22:08:21.766679 ttp-0.9.3/ttp/output/is_equal.py
+-rw-r--r--   0        0        0      230 2022-10-02 11:56:47.370840 ttp-0.9.3/ttp/output/macro.py
+-rw-r--r--   0        0        0     2210 2022-10-02 12:43:48.102403 ttp-0.9.3/ttp/output/transform.py
+-rw-r--r--   0        0        0     2011 2022-10-02 21:56:01.269058 ttp-0.9.3/ttp/output/validate_cerberus.py
+-rw-r--r--   0        0        0     8469 2022-10-02 12:10:13.579428 ttp-0.9.3/ttp/output/validate_yangson.py
+-rw-r--r--   0        0        0        0 2022-10-02 11:16:02.787032 ttp-0.9.3/ttp/patterns/__init__.py
+-rw-r--r--   0        0        0      593 2022-10-02 22:17:58.693165 ttp-0.9.3/ttp/patterns/get_pattern.py
+-rw-r--r--   0        0        0        0 2022-10-02 11:16:02.793015 ttp-0.9.3/ttp/returners/__init__.py
+-rw-r--r--   0        0        0     1680 2022-10-02 22:02:36.320460 ttp-0.9.3/ttp/returners/file_returner.py
+-rw-r--r--   0        0        0      197 2022-10-02 11:44:50.079655 ttp-0.9.3/ttp/returners/self_returner.py
+-rw-r--r--   0        0        0     2938 2022-10-02 12:35:24.240884 ttp-0.9.3/ttp/returners/syslog_returner.py
+-rw-r--r--   0        0        0     1882 2022-10-02 21:58:21.128182 ttp-0.9.3/ttp/returners/terminal_returner.py
+-rw-r--r--   0        0        0   156114 2023-04-15 08:28:46.606730 ttp-0.9.3/ttp/ttp.py
+-rw-r--r--   0        0        0        0 2022-10-02 11:16:02.769368 ttp-0.9.3/ttp/utils/__init__.py
+-rw-r--r--   0        0        0     2778 2022-10-02 12:36:46.909720 ttp-0.9.3/ttp/utils/get_attributes.py
+-rw-r--r--   0        0        0      157 2022-10-02 11:32:16.246029 ttp-0.9.3/ttp/utils/guess.py
+-rw-r--r--   0        0        0     1157 2022-10-02 22:21:07.735695 ttp-0.9.3/ttp/utils/load_python_exec_py2.py
+-rw-r--r--   0        0        0      955 2022-10-02 22:36:33.000288 ttp-0.9.3/ttp/utils/load_python_exec_py3.py
+-rw-r--r--   0        0        0    10511 2022-10-02 12:06:18.417379 ttp-0.9.3/ttp/utils/loaders.py
+-rw-r--r--   0        0        0     1454 2022-10-02 22:08:49.259463 ttp-0.9.3/ttp/utils/quick_parse.py
+-rw-r--r--   0        0        0        0 2022-10-02 11:16:02.814177 ttp-0.9.3/ttp/variable/__init__.py
+-rw-r--r--   0        0        0       88 2022-10-02 11:21:26.955490 ttp-0.9.3/ttp/variable/getfilename.py
+-rw-r--r--   0        0        0     1792 2022-10-02 21:59:56.076938 ttp-0.9.3/ttp/variable/gethostname.py
+-rw-r--r--   0        0        0     1107 2022-10-02 22:24:21.974076 ttp-0.9.3/ttp/variable/time_funcs.py
+-rw-r--r--   0        0        0     9570 1970-01-01 00:00:00.000000 ttp-0.9.3/PKG-INFO
```

### Comparing `ttp-0.9.2/LICENSE` & `ttp-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ttp-0.9.2/pyproject.toml` & `ttp-0.9.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ttp"
-version = "0.9.2"
+version = "0.9.3"
 description = "Template Text Parser"
 authors = ["Denis Mulyalin <d.mulyalin@gmail.com>"]
 maintainers = ["Denis Mulyalin <d.mulyalin@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/dmulyalin/ttp"
 repository = "https://github.com/dmulyalin/ttp"
@@ -52,15 +52,15 @@
 [tool.poetry.dev-dependencies]
 bandit = { version = "*", markers = "python_version >= '3.7'" }
 black = { version = "*", markers = "python_version >= '3.7'" }
 flake8 = { version = "*", markers = "python_version >= '3.7'" }
 pre-commit = { version = "*", markers = "python_version >= '3.7'" }
 pyenchant = { version = "*", markers = "python_version >= '3.7'" }
 pylint = { version = "*", markers = "python_version >= '3.7'" }
-pytest = { version = "^7.1.*", markers = "python_version >= '3.7'" }
+pytest = { version = ">=7.1", markers = "python_version >= '3.7'" }
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 ttp = 'ttp.ttp:cli_tool'
```

### Comparing `ttp-0.9.2/README.md` & `ttp-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `ttp-0.9.2/ttp/formatters/csv_formatter.py` & `ttp-0.9.3/ttp/formatters/csv_formatter.py`

 * *Files identical despite different names*

### Comparing `ttp-0.9.2/ttp/formatters/excel_formatter.py` & `ttp-0.9.3/ttp/formatters/excel_formatter.py`

 * *Files identical despite different names*

### Comparing `ttp-0.9.2/ttp/formatters/jinja2_formatter.py` & `ttp-0.9.3/ttp/formatters/jinja2_formatter.py`

 * *Files identical despite different names*

### Comparing `ttp-0.9.2/ttp/formatters/n2g_formatter.py` & `ttp-0.9.3/ttp/formatters/n2g_formatter.py`

 * *Files identical despite different names*

### Comparing `ttp-0.9.2/ttp/formatters/table_formatter.py` & `ttp-0.9.3/ttp/formatters/table_formatter.py`

 * *Files identical despite different names*

### Comparing `ttp-0.9.2/ttp/formatters/tabulate_formatter.py` & `ttp-0.9.3/ttp/formatters/tabulate_formatter.py`

 * *Files identical despite different names*

### Comparing `ttp-0.9.2/ttp/group/expand.py` & `ttp-0.9.3/ttp/group/expand.py`

 * *Files identical despite different names*

### Comparing `ttp-0.9.2/ttp/group/itemize.py` & `ttp-0.9.3/ttp/group/itemize.py`

 * *Files identical despite different names*

### Comparing `ttp-0.9.2/ttp/group/lookup.py` & `ttp-0.9.3/ttp/group/lookup.py`

 * *Files identical despite different names*

### Comparing `ttp-0.9.2/ttp/group/macro.py` & `ttp-0.9.3/ttp/group/macro.py`

 * *Files identical despite different names*

### Comparing `ttp-0.9.2/ttp/group/set_.py` & `ttp-0.9.3/ttp/group/set_.py`

 * *Files identical despite different names*

### Comparing `ttp-0.9.2/ttp/group/sformat.py` & `ttp-0.9.3/ttp/group/sformat.py`

 * *Files identical despite different names*

### Comparing `ttp-0.9.2/ttp/group/to_converters.py` & `ttp-0.9.3/ttp/group/to_converters.py`

 * *Files identical despite different names*

### Comparing `ttp-0.9.2/ttp/group/validate_cerberus.py` & `ttp-0.9.3/ttp/group/validate_cerberus.py`

 * *Files identical despite different names*

### Comparing `ttp-0.9.2/ttp/input/commands.py` & `ttp-0.9.3/ttp/input/commands.py`

 * *Files identical despite different names*

### Comparing `ttp-0.9.2/ttp/lookup/geoip2.py` & `ttp-0.9.3/ttp/lookup/geoip2.py`

 * *Files identical despite different names*

### Comparing `ttp-0.9.2/ttp/match/dns_lookups.py` & `ttp-0.9.3/ttp/match/dns_lookups.py`

 * *Files identical despite different names*

### Comparing `ttp-0.9.2/ttp/match/geoip_lookup.py` & `ttp-0.9.3/ttp/match/geoip_lookup.py`

 * *Files identical despite different names*

### Comparing `ttp-0.9.2/ttp/match/ip.py` & `ttp-0.9.3/ttp/match/ip.py`

 * *Files identical despite different names*

### Comparing `ttp-0.9.2/ttp/match/item.py` & `ttp-0.9.3/ttp/match/item.py`

 * *Files identical despite different names*

### Comparing `ttp-0.9.2/ttp/match/lookup.py` & `ttp-0.9.3/ttp/match/lookup.py`

 * *Files identical despite different names*

### Comparing `ttp-0.9.2/ttp/match/mac_eui.py` & `ttp-0.9.3/ttp/match/mac_eui.py`

 * *Files identical despite different names*

### Comparing `ttp-0.9.2/ttp/match/macro.py` & `ttp-0.9.3/ttp/match/macro.py`

 * *Files identical despite different names*

### Comparing `ttp-0.9.2/ttp/match/re_.py` & `ttp-0.9.3/ttp/match/re_.py`

 * *Files identical despite different names*

### Comparing `ttp-0.9.2/ttp/match/string.py` & `ttp-0.9.3/ttp/match/string.py`

 * *Files identical despite different names*

### Comparing `ttp-0.9.2/ttp/match/to.py` & `ttp-0.9.3/ttp/match/to.py`

 * *Files identical despite different names*

### Comparing `ttp-0.9.2/ttp/match/unrange.py` & `ttp-0.9.3/ttp/match/unrange.py`

 * *Files identical despite different names*

### Comparing `ttp-0.9.2/ttp/match/uptimeparse.py` & `ttp-0.9.3/ttp/match/uptimeparse.py`

 * *Files identical despite different names*

### Comparing `ttp-0.9.2/ttp/output/deepdiffer.py` & `ttp-0.9.3/ttp/output/deepdiffer.py`

 * *Files identical despite different names*

### Comparing `ttp-0.9.2/ttp/output/transform.py` & `ttp-0.9.3/ttp/output/transform.py`

 * *Files identical despite different names*

### Comparing `ttp-0.9.2/ttp/output/validate_cerberus.py` & `ttp-0.9.3/ttp/output/validate_cerberus.py`

 * *Files identical despite different names*

### Comparing `ttp-0.9.2/ttp/output/validate_yangson.py` & `ttp-0.9.3/ttp/output/validate_yangson.py`

 * *Files identical despite different names*

### Comparing `ttp-0.9.2/ttp/patterns/get_pattern.py` & `ttp-0.9.3/ttp/patterns/get_pattern.py`

 * *Files identical despite different names*

### Comparing `ttp-0.9.2/ttp/returners/file_returner.py` & `ttp-0.9.3/ttp/returners/file_returner.py`

 * *Files identical despite different names*

### Comparing `ttp-0.9.2/ttp/returners/syslog_returner.py` & `ttp-0.9.3/ttp/returners/syslog_returner.py`

 * *Files identical despite different names*

### Comparing `ttp-0.9.2/ttp/returners/terminal_returner.py` & `ttp-0.9.3/ttp/returners/terminal_returner.py`

 * *Files identical despite different names*

### Comparing `ttp-0.9.2/ttp/ttp.py` & `ttp-0.9.3/ttp/ttp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-__version__ = "0.9.2"
+__version__ = "0.9.3"
 
 import re
 import os
 import logging
 import copy
 import ast
 import pickle
@@ -963,16 +963,18 @@
             [input.debug() for input in self.inputs.values()]
             [group.debug() for group in self.groups]
             [output_obj.debug() for output_obj in self.outputs]
 
     def debug(self):
         from pprint import pformat
 
+        attributes = dict(vars(self))
+        _ = attributes.pop("_ttp_")
         text = "Template Object {}, Template name '{}' content:\n{}".format(
-            self, self.name, pformat(vars(self), indent=4)
+            self, self.name, pformat(attributes, indent=4)
         )
         log.debug(text)
 
     def add_lookup(self, data):
         """Method to load lookup data"""
         self.lookups.update(data)
         [template.add_lookup(data) for template in self.templates]
@@ -1926,16 +1928,18 @@
         # run recursion for children:
         for child in self.children:
             child.update_runs(data)
 
     def debug(self):
         from pprint import pformat
 
+        attributes = dict(vars(self))
+        _ = attributes.pop("_ttp_")
         text = "Group object {}, Group name '{}' content:\n{}".format(
-            self, self.name, pformat(vars(self), indent=4)
+            self, self.name, pformat(attributes, indent=4)
         )
         log.debug(text)
         for re_dict in self.start_re:
             for var_name, var_obj in re_dict["VARIABLES"].items():
                 var_obj.debug()
         for re_dict in self.re:
             for var_name, var_obj in re_dict["VARIABLES"].items():
@@ -2324,16 +2328,18 @@
             del self.LINE, self.skip_defaults
             del self.var_dict, self.var_res
         return self.regex
 
     def debug(self):
         from pprint import pformat
 
+        attributes = dict(vars(self))
+        _ = attributes.pop("_ttp_") # remove _ttp_ dictionary to not clutter the output
         text = "Variable object {}, Variable name '{}' content:\n{}".format(
-            self, self.var_name, pformat(vars(self), indent=4)
+            self, self.var_name, pformat(attributes, indent=4)
         )
         log.debug(text)
 
 
 """
 ==============================================================================
 TTP PARSER OBJECT
@@ -2877,28 +2883,26 @@
             DATA (dict): data to add to the DATA
             PATH (list): list of path keys
             result : dict or list that contains results
         Returns:
             transformed DATA with list at given PATH and appended results to it
         """
         if PATH:
-            name = PATH[0].rstrip("*")
+            name = PATH[0][0]
             # add support for null path
             if name == "_":
                 if len(PATH) == 1:  # reached end of PATH, process DATA and return it
                     if isinstance(DATA, dict):
                         DATA.update(result)
                     elif isinstance(DATA, list):
                         DATA[-1].update(result)
                     return DATA
                 else:  # have more path items, need to skip null path,
                     _ = PATH.pop(0)  # remove null path item to skip it
-                    name = PATH[0].rstrip(
-                        "*"
-                    )  # continue processing remaining PATH items
+                    name = PATH[0][0]
             if isinstance(DATA, dict):
                 if name in DATA:
                     DATA[name] = self.value_to_list(DATA[name], PATH[1:], result)
                     return DATA
             elif isinstance(DATA, list):
                 if name in DATA[-1]:
                     DATA[-1][name] = self.value_to_list(
@@ -2925,22 +2929,20 @@
         if KEYS:  # check if list is not empty:
             # add support for null path
             if KEYS[0] == "_":
                 if len(KEYS) == 1:
                     return {}
                 else:
                     _ = KEYS.pop(0)
-            name = str(KEYS[0]).rstrip("*")  # get the name of first item in PATH keys
-            stars_count = len(KEYS[0]) - len(
-                name
-            )  # get the number of "*" key ends with
+            name = KEYS[0][0]
+            asterisk_count = KEYS[0][1]
             if self._ttp_["dynamic_path_key_to_int"]:
                 # convert key to integer if it is integer
                 name = int(name) if name.isdigit() else name
-            if stars_count == 1:  # if one * at the end - make a list
+            if asterisk_count == "*":  # if one * at the end - make a list
                 if len(KEYS) == 1:  # if KEYS=[1,2,3,4*], returns {1:{2:{3:{4:[{}]}}}}
                     return {name: []}  # if last item in PATH - return emplty list
                 else:  # if KEYS=[1,2,3*,4], returns {1:{2:{3:[{4:{}}]}}}
                     return {
                         name: [self.list_to_dict_fwd(KEYS[1:])]
                     }  # run recursion if PATH has more than one element
             else:  # if KEYS=[1,2,3,4], returns {1:{2:{3:{4:{}}}}}
@@ -2954,27 +2956,25 @@
             ELEMENT: nested list, list of dictionaries or dictionary to get element from
         Returns:
             last element at given PATH of transformed ELEMENT dictionary
         """
         if PATH == []:
             return ELEMENT  # check if PATH is empty, if so - stop and return ELEMENT
         elif isinstance(ELEMENT, dict):
-            name = PATH[0].rstrip("*")
+            name = PATH[0][0]
             if self._ttp_["dynamic_path_key_to_int"]:
                 # convert key to integer if it is integer
                 name = int(name) if name.isdigit() else name
             # add support for null path
             if name == "_":
                 if len(PATH) == 1:  # reached end of PATH, need to return ELEMENT
                     return ELEMENT
                 else:  # have more path items, need to skip null path,
                     _ = PATH.pop(0)  # remove null path item to skip it
-                    name = PATH[0].rstrip(
-                        "*"
-                    )  # continue processing remaining PATH items
+                    name = PATH[0][0]
             if name in ELEMENT:  # check if first element of the list is in ELEMENT
                 return self.dict_by_path(
                     PATH[1:], ELEMENT[name]
                 )  # run recursion with moving forward in both - PATH and ELEMENT
             else:  # if first element not in dict - we found new key, update it into the dict
                 ELEMENT.update(
                     self.list_to_dict_fwd(PATH)
@@ -3015,15 +3015,15 @@
                 self._merge_recursively(E[-1], result_data)
             else:
                 E.append(result_data)
         elif isinstance(E, dict):
             if self.record.get("merge_with_last"):
                 self._merge_recursively(E, result_data)
             # check if result_path endswith "**" - update result's ELEMENET without converting it into list:
-            elif len(result_path[-1]) - len(result_path[-1].rstrip("*")) == 2:
+            elif result_path[-1][1] == "**":
                 result_data.update(E)
                 E.update(result_data)
             # to match all the other cases, like templates without "**" in path:
             elif E != {}:
                 # transform ELEMENT dict to list and append data to it:
                 self.results = self.value_to_list(
                     DATA=self.results, PATH=result_path, result=result_data
@@ -3179,32 +3179,45 @@
             REDICT["GROUP"].group_id == self.started_groups[-1]
         ):
             return
         # action to end current group by adding it to ended groups
         self.ended_groups.add(REDICT["GROUP"].group_id)
 
     def form_path(self, path):
-        """Method to form dynamic path"""
+        """
+        Method to form dynamic path transforming it into a list of tuples,
+        where each tuple first element is a path item value and second 
+        element is a number of asterisks, need to keep asterisks count 
+        separatefrom path item value becasue match result value can end 
+        with asterisk - issue #97
+        """
         for index, path_item in enumerate(path):
+            asterisk_count = len(path_item) - len(path_item.rstrip("*"))
+            path_item = path_item.rstrip("*")
             match = re.findall(r"{{\s*(\S+)\s*}}", path_item)
-            if not match:
-                continue
-            for m in match:
-                pattern = r"{{\s*" + m + r"\s*}}"
-                if m in self.record["result"]:
-                    self.dyn_path_cache[m] = self.record["result"][m]
-                    repl = str(self.record["result"].pop(m))
-                    path_item = re.sub(pattern, repl, path_item)
-                elif m in self.dyn_path_cache:
-                    path_item = re.sub(pattern, self.dyn_path_cache[m], path_item)
-                elif m in self.variables:
-                    path_item = re.sub(pattern, str(self.variables[m]), path_item)
-                else:
-                    return False
-            path[index] = path_item
+            if match:
+                for m in match:
+                    pattern = r"{{\s*" + m + r"\s*}}"
+                    if m in self.record["result"]:
+                        self.dyn_path_cache[m] = self.record["result"][m]
+                        repl = str(self.record["result"].pop(m))
+                        # try re replacement first
+                        try:
+                            path_item = re.sub(pattern, repl, path_item)
+                        # might fail if match contains '\', try string replace
+                        except re.error:
+                            path_item = re.sub(pattern, "__replace_me__", path_item)
+                            path_item = path_item.replace("__replace_me__", repl)
+                    elif m in self.dyn_path_cache:
+                        path_item = re.sub(pattern, self.dyn_path_cache[m], path_item)
+                    elif m in self.variables:
+                        path_item = re.sub(pattern, str(self.variables[m]), path_item)
+                    else:
+                        return False
+            path[index] = (path_item, asterisk_count * "*",)
         return path
 
     def processgrp(self):
         """Method to process group results"""
         # add default values to group results
         for k, v in self.record["DEFAULTS"].items():
             self.record["result"].setdefault(k, v)
@@ -3213,16 +3226,18 @@
             func_name = item["name"]
             args = item.get("args", [])
             kwargs = item.get("kwargs", {})
             # run group functions
             self.record["result"], flags = self._ttp_["group"][func_name](
                 self.record["result"], *args, **kwargs
             )
-            # if conditions check been false, return False:
-            if flags == False:
+            # if conditions check been false, return False except when
+            # results marked as merge_with_last, this logic is weak but 
+            # simplest to fix issue #103
+            if flags == False and self.record.get("merge_with_last") != True:
                 return False
         processed_path = self.form_path(self.record["PATH"])
         if processed_path:
             self.record["PATH"] = processed_path
         else:
             return False
```

### Comparing `ttp-0.9.2/ttp/utils/get_attributes.py` & `ttp-0.9.3/ttp/utils/get_attributes.py`

 * *Files identical despite different names*

### Comparing `ttp-0.9.2/ttp/utils/load_python_exec_py2.py` & `ttp-0.9.3/ttp/utils/load_python_exec_py2.py`

 * *Files identical despite different names*

### Comparing `ttp-0.9.2/ttp/utils/load_python_exec_py3.py` & `ttp-0.9.3/ttp/utils/load_python_exec_py3.py`

 * *Files identical despite different names*

### Comparing `ttp-0.9.2/ttp/utils/loaders.py` & `ttp-0.9.3/ttp/utils/loaders.py`

 * *Files identical despite different names*

### Comparing `ttp-0.9.2/ttp/utils/quick_parse.py` & `ttp-0.9.3/ttp/utils/quick_parse.py`

 * *Files identical despite different names*

### Comparing `ttp-0.9.2/ttp/variable/gethostname.py` & `ttp-0.9.3/ttp/variable/gethostname.py`

 * *Files identical despite different names*

### Comparing `ttp-0.9.2/ttp/variable/time_funcs.py` & `ttp-0.9.3/ttp/variable/time_funcs.py`

 * *Files identical despite different names*

### Comparing `ttp-0.9.2/setup.py` & `ttp-0.9.3/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,63 +1,251 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: ttp
+Version: 0.9.3
+Summary: Template Text Parser
+Home-page: https://github.com/dmulyalin/ttp
+License: MIT
+Keywords: Parsing,TTP,regex
+Author: Denis Mulyalin
+Author-email: d.mulyalin@gmail.com
+Maintainer: Denis Mulyalin
+Maintainer-email: d.mulyalin@gmail.com
+Requires-Python: >=2.7,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python :: 2
+Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Utilities
+Provides-Extra: docs
+Provides-Extra: full
+Requires-Dist: Sphinx (==4.3.0) ; (python_version >= "3.7") and (extra == "docs")
+Requires-Dist: cerberus (>=1.3.0,<1.4.0) ; (python_version >= "3.7") and (extra == "full")
+Requires-Dist: deepdiff (>=5.8.0,<5.9.0) ; (python_version >= "3.7") and (extra == "full")
+Requires-Dist: jinja2 (>=3.0.0,<3.1.0) ; (python_version >= "3.7") and (extra == "full")
+Requires-Dist: n2g (>=0.2.0,<0.3.0) ; (python_version >= "3.7") and (extra == "full")
+Requires-Dist: openpyxl (>=3.0.0,<3.1.0) ; (python_version >= "3.7") and (extra == "full")
+Requires-Dist: pyyaml (==6.0) ; (python_version >= "3.7") and (extra == "full")
+Requires-Dist: readthedocs-sphinx-search (==0.1.1) ; (python_version >= "3.7") and (extra == "docs")
+Requires-Dist: sphinx_rtd_theme (==1.0.0) ; (python_version >= "3.7") and (extra == "docs")
+Requires-Dist: sphinxcontrib-applehelp (==1.0.1) ; (python_version >= "3.7") and (extra == "docs")
+Requires-Dist: sphinxcontrib-devhelp (==1.0.1) ; (python_version >= "3.7") and (extra == "docs")
+Requires-Dist: sphinxcontrib-htmlhelp (==2.0.0) ; (python_version >= "3.7") and (extra == "docs")
+Requires-Dist: sphinxcontrib-jsmath (==1.0.1) ; (python_version >= "3.7") and (extra == "docs")
+Requires-Dist: sphinxcontrib-napoleon (==0.7) ; (python_version >= "3.7") and (extra == "docs")
+Requires-Dist: sphinxcontrib-qthelp (==1.0.2) ; (python_version >= "3.7") and (extra == "docs")
+Requires-Dist: sphinxcontrib-serializinghtml (==1.1.5) ; (python_version >= "3.7") and (extra == "docs")
+Requires-Dist: sphinxcontrib-spelling (==7.2.1) ; (python_version >= "3.7") and (extra == "docs")
+Requires-Dist: tabulate (>=0.8.0,<0.9.0) ; (python_version >= "3.7") and (extra == "full")
+Requires-Dist: ttp_templates (<1.0.0) ; (python_version >= "3.7") and (extra == "full")
+Requires-Dist: yangson (>=1.4.0,<1.5.0) ; (python_version >= "3.7") and (extra == "full")
+Project-URL: Documentation, https://ttp.readthedocs.io/
+Project-URL: Repository, https://github.com/dmulyalin/ttp
+Description-Content-Type: text/markdown
+
+[![Downloads](https://pepy.tech/badge/ttp)](https://pepy.tech/project/ttp)
+[![PyPI versions](https://img.shields.io/pypi/pyversions/ttp.svg)](https://pypi.python.org/pypi/ttp/)
+[![Documentation status](https://readthedocs.org/projects/ttp/badge/?version=latest)](http://ttp.readthedocs.io/?badge=latest)
+
+# Template Text Parser
+
+TTP is a Python library for semi-structured text parsing using templates.
+
+## Why?
+
+To save ones time on transforming raw text into structured data and beyond.
+
+## How?
+
+Regexes, regexes everywhere... but, dynamically formed out of TTP templates with added capabilities to simplify the  process of getting desired outcome.
+
+## What?
+
+In essence TTP can help to:
+  - Prepare, sort and load text data for parsing
+  - Parse text using regexes dynamically derived out of templates
+  - Process matches on the fly using broad set of built-in or custom functions
+  - Combine match results in a structure with arbitrary hierarchy
+  - Transform results in desired format to ease consumption by humans or machines
+  - Return results to various destinations for storage or further processing
+
+Reference [documentation](https://ttp.readthedocs.io) for more information.
+
+TTP [Networktocode Slack channel](https://networktocode.slack.com/archives/C018HMJQECB)
+
+Collection of [TTP Templates](https://github.com/dmulyalin/ttp_templates)
+
+## Example - as simple as it can be
+
+Simple interfaces configuration parsing example
+
+<details><summary>Code</summary>
+
+```python
+from ttp import ttp
+import pprint
+
+data = """
+interface Loopback0
+ description Router-id-loopback
+ ip address 192.168.0.113/24
+!
+interface Vlan778
+ description CPE_Acces_Vlan
+ ip address 2002::fd37/124
+ ip vrf CPE1
+!
+"""
+
+template = """
+interface {{ interface }}
+ ip address {{ ip }}/{{ mask }}
+ description {{ description }}
+ ip vrf {{ vrf }}
+"""
+
+parser = ttp(data, template)
+parser.parse()
+pprint.pprint(parser.result(), width=100)
+
+# prints:
+# [[[{'description': 'Router-id-loopback',
+#     'interface': 'Loopback0',
+#     'ip': '192.168.0.113',
+#     'mask': '24'},
+#    {'description': 'CPE_Acces_Vlan',
+#     'interface': 'Vlan778',
+#     'ip': '2002::fd37',
+#     'mask': '124',
+#     'vrf': 'CPE1'}]]]
+```
+</details>
+
+## Example - a bit more complicated
+
+For this example lets say we want to parse BGP peerings output, but combine state with configuration data, at the end we want to get pretty looking text table printed to screen.
+
+<details><summary>Code</summary>
+
+```python
+template="""
+<doc>
+This template first parses "show bgp vrf CUST-1 vpnv4 unicast summary" commands
+output, forming results for "bgp_state" dictionary, where peer ip is a key.
+
+Following that, "show run | section bgp" output parsed by group "bgp_cfg". That
+group uses nested groups to form results structure, including absolute path
+"/bgp_peers*" with path formatter to produce a list of peers under "bgp_peers"
+path.
+
+For each peer "hostname" and local bgp "local_asn" added using previous matches.
+Additionally, group lookup function used to lookup peer state from "bgp_state"
+group results, adding found data to peer results.
+
+Finally, "bgp_peers" section of results passed via "tabulate_outputter" to
+from and print this table to terminal:
+
+hostname           local_asn    vrf_name    peer_ip    peer_asn    uptime    state    description    afi    rpl_in           rpl_out
+-----------------  -----------  ----------  ---------  ----------  --------  -------  -------------  -----  ---------------  ---------------
+ucs-core-switch-1  65100        CUST-1      192.0.2.1  65101       00:12:33  300      peer-1         ipv4   RPL-1-IMPORT-v4  RPL-1-EXPORT-V4
+ucs-core-switch-1  65100        CUST-1      192.0.2.2  65102       03:55:01  idle     peer-2         ipv4   RPL-2-IMPORT-V6  RPL-2-EXPORT-V6
+
+Run this script with "python filename.py"
+</doc>
+
+<vars>
+hostname="gethostname"
+chain_1 = [
+    "set('vrf_name')",
+    "lookup('peer_ip', group='bgp_state', update=True)"
+]
+</vars>
+
+<group name="bgp_state.{{ peer }}" input="bgp_state">
+{{ peer }}  4 65101      20      21       43    0    0 {{ uptime }} {{ state }}
+</group>
+
+<group name="bgp_cfg" input="bgp_config">
+router bgp {{ asn | record(asn) }}
+  <group name="vrfs.{{ vrf_name }}" record="vrf_name">
+  vrf {{ vrf_name }}
+    <group name="/bgp_peers*" chain="chain_1">
+    neighbor {{ peer_ip }}
+      {{ local_asn | set(asn) }}
+      {{ hostname | set(hostname) }}
+      remote-as {{ peer_asn }}
+      description {{ description }}
+      address-family {{ afi }} unicast
+        route-map {{ rpl_in }} in
+        route-map {{ rpl_out }} out
+	</group>
+  </group>
+</group>
+
+<output
+name="tabulate_outputter"
+format="tabulate"
+path="bgp_peers"
+returner="terminal"
+headers="hostname, local_asn, vrf_name, peer_ip, peer_asn, uptime, state, description, afi, rpl_in, rpl_out"
+/>
+"""
+
+data_bgp_state = """
+ucs-core-switch-1#show bgp vrf CUST-1 vpnv4 unicast summary
+Neighbor   V    AS MsgRcvd MsgSent   TblVer  InQ OutQ Up/Down  State/PfxRcd
+192.0.2.1  4 65101      32      54       42    0    0 00:12:33       300
+192.0.2.2  4 65101      11      45       99    0    0 03:55:01       idle
+"""
+
+data_bgp_config = """
+ucs-core-switch-1#show run | section bgp
+router bgp 65100
+  vrf CUST-1
+    neighbor 192.0.2.1
+      remote-as 65101
+      description peer-1
+      address-family ipv4 unicast
+        route-map RPL-1-IMPORT-v4 in
+        route-map RPL-1-EXPORT-V4 out
+    neighbor 192.0.2.2
+      remote-as 65102
+      description peer-2
+      address-family ipv4 unicast
+        route-map RPL-2-IMPORT-V6 in
+        route-map RPL-2-EXPORT-V6 out
+"""
+
+from ttp import ttp
+
+parser = ttp()
+parser.add_template(template)
+parser.add_input(data=data_bgp_state, input_name="bgp_state")
+parser.add_input(data=data_bgp_config, input_name="bgp_config")
+parser.parse()
+```
+</details>
+
+# Contributions
+Feel free to submit an issue, report a bug or ask a question, feature requests are welcomed. Or [buy](https://paypal.me/dmulyalin) Author a coffee
 
-packages = \
-['ttp',
- 'ttp.formatters',
- 'ttp.group',
- 'ttp.input',
- 'ttp.lookup',
- 'ttp.match',
- 'ttp.output',
- 'ttp.patterns',
- 'ttp.returners',
- 'ttp.utils',
- 'ttp.variable']
-
-package_data = \
-{'': ['*']}
-
-extras_require = \
-{'docs:python_version >= "3.7"': ['readthedocs-sphinx-search==0.1.1',
-                                  'Sphinx==4.3.0',
-                                  'sphinx_rtd_theme==1.0.0',
-                                  'sphinxcontrib-applehelp==1.0.1',
-                                  'sphinxcontrib-devhelp==1.0.1',
-                                  'sphinxcontrib-htmlhelp==2.0.0',
-                                  'sphinxcontrib-jsmath==1.0.1',
-                                  'sphinxcontrib-napoleon==0.7',
-                                  'sphinxcontrib-qthelp==1.0.2',
-                                  'sphinxcontrib-serializinghtml==1.1.5',
-                                  'sphinxcontrib-spelling==7.2.1'],
- 'full:python_version >= "3.7"': ['cerberus>=1.3.0,<1.4.0',
-                                  'jinja2>=3.0.0,<3.1.0',
-                                  'pyyaml==6.0',
-                                  'deepdiff>=5.8.0,<5.9.0',
-                                  'openpyxl>=3.0.0,<3.1.0',
-                                  'tabulate>=0.8.0,<0.9.0',
-                                  'ttp_templates<1.0.0',
-                                  'yangson>=1.4.0,<1.5.0',
-                                  'n2g>=0.2.0,<0.3.0']}
-
-entry_points = \
-{'console_scripts': ['ttp = ttp.ttp:cli_tool']}
-
-setup_kwargs = {
-    'name': 'ttp',
-    'version': '0.9.2',
-    'description': 'Template Text Parser',
-    'long_description': '[![Downloads](https://pepy.tech/badge/ttp)](https://pepy.tech/project/ttp)\n[![PyPI versions](https://img.shields.io/pypi/pyversions/ttp.svg)](https://pypi.python.org/pypi/ttp/)\n[![Documentation status](https://readthedocs.org/projects/ttp/badge/?version=latest)](http://ttp.readthedocs.io/?badge=latest)\n\n# Template Text Parser\n\nTTP is a Python library for semi-structured text parsing using templates.\n\n## Why?\n\nTo save ones time on transforming raw text into structured data and beyond.\n\n## How?\n\nRegexes, regexes everywhere... but, dynamically formed out of TTP templates with added capabilities to simplify the  process of getting desired outcome.\n\n## What?\n\nIn essence TTP can help to:\n  - Prepare, sort and load text data for parsing\n  - Parse text using regexes dynamically derived out of templates\n  - Process matches on the fly using broad set of built-in or custom functions\n  - Combine match results in a structure with arbitrary hierarchy\n  - Transform results in desired format to ease consumption by humans or machines\n  - Return results to various destinations for storage or further processing\n\nReference [documentation](https://ttp.readthedocs.io) for more information.\n\nTTP [Networktocode Slack channel](https://networktocode.slack.com/archives/C018HMJQECB)\n\nCollection of [TTP Templates](https://github.com/dmulyalin/ttp_templates)\n\n## Example - as simple as it can be\n\nSimple interfaces configuration parsing example\n\n<details><summary>Code</summary>\n\n```python\nfrom ttp import ttp\nimport pprint\n\ndata = """\ninterface Loopback0\n description Router-id-loopback\n ip address 192.168.0.113/24\n!\ninterface Vlan778\n description CPE_Acces_Vlan\n ip address 2002::fd37/124\n ip vrf CPE1\n!\n"""\n\ntemplate = """\ninterface {{ interface }}\n ip address {{ ip }}/{{ mask }}\n description {{ description }}\n ip vrf {{ vrf }}\n"""\n\nparser = ttp(data, template)\nparser.parse()\npprint.pprint(parser.result(), width=100)\n\n# prints:\n# [[[{\'description\': \'Router-id-loopback\',\n#     \'interface\': \'Loopback0\',\n#     \'ip\': \'192.168.0.113\',\n#     \'mask\': \'24\'},\n#    {\'description\': \'CPE_Acces_Vlan\',\n#     \'interface\': \'Vlan778\',\n#     \'ip\': \'2002::fd37\',\n#     \'mask\': \'124\',\n#     \'vrf\': \'CPE1\'}]]]\n```\n</details>\n\n## Example - a bit more complicated\n\nFor this example lets say we want to parse BGP peerings output, but combine state with configuration data, at the end we want to get pretty looking text table printed to screen.\n\n<details><summary>Code</summary>\n\n```python\ntemplate="""\n<doc>\nThis template first parses "show bgp vrf CUST-1 vpnv4 unicast summary" commands\noutput, forming results for "bgp_state" dictionary, where peer ip is a key.\n\nFollowing that, "show run | section bgp" output parsed by group "bgp_cfg". That\ngroup uses nested groups to form results structure, including absolute path\n"/bgp_peers*" with path formatter to produce a list of peers under "bgp_peers"\npath.\n\nFor each peer "hostname" and local bgp "local_asn" added using previous matches.\nAdditionally, group lookup function used to lookup peer state from "bgp_state"\ngroup results, adding found data to peer results.\n\nFinally, "bgp_peers" section of results passed via "tabulate_outputter" to\nfrom and print this table to terminal:\n\nhostname           local_asn    vrf_name    peer_ip    peer_asn    uptime    state    description    afi    rpl_in           rpl_out\n-----------------  -----------  ----------  ---------  ----------  --------  -------  -------------  -----  ---------------  ---------------\nucs-core-switch-1  65100        CUST-1      192.0.2.1  65101       00:12:33  300      peer-1         ipv4   RPL-1-IMPORT-v4  RPL-1-EXPORT-V4\nucs-core-switch-1  65100        CUST-1      192.0.2.2  65102       03:55:01  idle     peer-2         ipv4   RPL-2-IMPORT-V6  RPL-2-EXPORT-V6\n\nRun this script with "python filename.py"\n</doc>\n\n<vars>\nhostname="gethostname"\nchain_1 = [\n    "set(\'vrf_name\')",\n    "lookup(\'peer_ip\', group=\'bgp_state\', update=True)"\n]\n</vars>\n\n<group name="bgp_state.{{ peer }}" input="bgp_state">\n{{ peer }}  4 65101      20      21       43    0    0 {{ uptime }} {{ state }}\n</group>\n\n<group name="bgp_cfg" input="bgp_config">\nrouter bgp {{ asn | record(asn) }}\n  <group name="vrfs.{{ vrf_name }}" record="vrf_name">\n  vrf {{ vrf_name }}\n    <group name="/bgp_peers*" chain="chain_1">\n    neighbor {{ peer_ip }}\n      {{ local_asn | set(asn) }}\n      {{ hostname | set(hostname) }}\n      remote-as {{ peer_asn }}\n      description {{ description }}\n      address-family {{ afi }} unicast\n        route-map {{ rpl_in }} in\n        route-map {{ rpl_out }} out\n\t</group>\n  </group>\n</group>\n\n<output\nname="tabulate_outputter"\nformat="tabulate"\npath="bgp_peers"\nreturner="terminal"\nheaders="hostname, local_asn, vrf_name, peer_ip, peer_asn, uptime, state, description, afi, rpl_in, rpl_out"\n/>\n"""\n\ndata_bgp_state = """\nucs-core-switch-1#show bgp vrf CUST-1 vpnv4 unicast summary\nNeighbor   V    AS MsgRcvd MsgSent   TblVer  InQ OutQ Up/Down  State/PfxRcd\n192.0.2.1  4 65101      32      54       42    0    0 00:12:33       300\n192.0.2.2  4 65101      11      45       99    0    0 03:55:01       idle\n"""\n\ndata_bgp_config = """\nucs-core-switch-1#show run | section bgp\nrouter bgp 65100\n  vrf CUST-1\n    neighbor 192.0.2.1\n      remote-as 65101\n      description peer-1\n      address-family ipv4 unicast\n        route-map RPL-1-IMPORT-v4 in\n        route-map RPL-1-EXPORT-V4 out\n    neighbor 192.0.2.2\n      remote-as 65102\n      description peer-2\n      address-family ipv4 unicast\n        route-map RPL-2-IMPORT-V6 in\n        route-map RPL-2-EXPORT-V6 out\n"""\n\nfrom ttp import ttp\n\nparser = ttp()\nparser.add_template(template)\nparser.add_input(data=data_bgp_state, input_name="bgp_state")\nparser.add_input(data=data_bgp_config, input_name="bgp_config")\nparser.parse()\n```\n</details>\n\n# Contributions\nFeel free to submit an issue, report a bug or ask a question, feature requests are welcomed. Or [buy](https://paypal.me/dmulyalin) Author a coffee\n\n# Additional resources\n\nList of additional resources:\n\n- Sandbox to test TTP templates - http://textfsm.nornir.tech/ by [tbotnz](https://github.com/tbotnz)\n- Videos on TTP - https://pynet.twb-tech.com/videos/ttp/ttp.html by [Kirk Byers](https://github.com/ktbyers)\n',
-    'author': 'Denis Mulyalin',
-    'author_email': 'd.mulyalin@gmail.com',
-    'maintainer': 'Denis Mulyalin',
-    'maintainer_email': 'd.mulyalin@gmail.com',
-    'url': 'https://github.com/dmulyalin/ttp',
-    'packages': packages,
-    'package_data': package_data,
-    'extras_require': extras_require,
-    'entry_points': entry_points,
-    'python_requires': '>=2.7,<4.0',
-}
+# Additional resources
 
+List of additional resources:
+
+- Sandbox to test TTP templates - http://textfsm.nornir.tech/ by [tbotnz](https://github.com/tbotnz)
+- Videos on TTP - https://pynet.twb-tech.com/videos/ttp/ttp.html by [Kirk Byers](https://github.com/ktbyers)
 
-setup(**setup_kwargs)
```

