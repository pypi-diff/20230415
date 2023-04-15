# Comparing `tmp/FlexGet-3.6.2.tar.gz` & `tmp/FlexGet-3.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/Flexget/Flexget/dist/.tmp-ow70lenx/FlexGet-3.6.2.tar", last modified: Wed Apr 12 15:13:40 2023, max compression
+gzip compressed data, was "/home/runner/work/Flexget/Flexget/dist/.tmp-jtyvx3uw/FlexGet-3.6.3.tar", last modified: Sat Apr 15 15:12:14 2023, max compression
```

## Comparing `FlexGet-3.6.2.tar` & `FlexGet-3.6.3.tar`

### file list

```diff
@@ -1,981 +1,981 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/FlexGet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-04-12 15:13:40.000000 FlexGet-3.6.2/FlexGet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    39106 2023-04-12 15:13:40.000000 FlexGet-3.6.2/FlexGet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 15:13:40.000000 FlexGet-3.6.2/FlexGet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-12 15:13:40.000000 FlexGet-3.6.2/FlexGet.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-04-12 15:13:40.000000 FlexGet-3.6.2/FlexGet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-12 15:13:40.000000 FlexGet-3.6.2/FlexGet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-04-12 15:13:10.000000 FlexGet-3.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-12 15:13:10.000000 FlexGet-3.6.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-04-12 15:13:40.000000 FlexGet-3.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-04-12 15:13:10.000000 FlexGet-3.6.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-04-12 15:13:10.000000 FlexGet-3.6.2/dev-requirements-extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-04-12 15:13:10.000000 FlexGet-3.6.2/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-12 15:13:34.000000 FlexGet-3.6.2/flexget/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/api/
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15580 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/api/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/api/core/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/api/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/api/core/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/api/core/cached.py
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/api/core/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/api/core/format_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/api/core/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/api/core/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    20589 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/api/core/server.py
--rw-r--r--   0 runner    (1001) docker     (123)    22039 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/api/core/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/api/core/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/api/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     7051 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/api/templates/api_response.html
--rw-r--r--   0 runner    (1001) docker     (123)    10279 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/api/templates/swagger-ui.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/components/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/components/archive/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/archive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/archive/archive.py
--rw-r--r--   0 runner    (1001) docker     (123)    10509 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/archive/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6014 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/archive/db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/components/archives/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/archives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/archives/archives.py
--rw-r--r--   0 runner    (1001) docker     (123)     7526 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/archives/decompress.py
--rw-r--r--   0 runner    (1001) docker     (123)     7337 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/archives/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/components/backlog/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/backlog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/backlog/backlog.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/backlog/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/backlog/db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/components/bittorrent/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/bittorrent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/bittorrent/convert_magnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/bittorrent/magnet_info_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/bittorrent/private_torrents.py
--rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/bittorrent/torrent.py
--rw-r--r--   0 runner    (1001) docker     (123)    10080 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/bittorrent/torrent_alive.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/bittorrent/torrent_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     8533 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/bittorrent/torrent_match.py
--rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/bittorrent/torrent_scrub.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/bittorrent/torrent_size.py
--rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/bittorrent/trackers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/components/emby/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/emby/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    83287 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/emby/api_emby.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/emby/emby_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/emby/emby_lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/emby/emby_refresh.py
--rw-r--r--   0 runner    (1001) docker     (123)     4954 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/emby/emby_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/emby/from_emby.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/components/estimate_release/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/estimate_release/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/estimate_release/estimate_release.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/components/estimate_release/estimators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/estimate_release/estimators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/estimate_release/estimators/est_movies_bluray.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/estimate_release/estimators/est_released_movies.py
--rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/estimate_release/estimators/est_series_tvmaze.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/components/failed/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/failed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/failed/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/failed/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/failed/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/failed/retry_failed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/components/ftp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/ftp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8431 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/ftp/ftp_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/ftp/ftp_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    15674 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/ftp/sftp.py
--rw-r--r--   0 runner    (1001) docker     (123)    23191 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/ftp/sftp_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/components/history/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/history/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/history/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/history/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/history/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/history/history.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/components/imdb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/imdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/imdb/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6883 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/imdb/db.py
--rw-r--r--   0 runner    (1001) docker     (123)    12539 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/imdb/from_imdb.py
--rw-r--r--   0 runner    (1001) docker     (123)    10772 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/imdb/imdb.py
--rw-r--r--   0 runner    (1001) docker     (123)    13034 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/imdb/imdb_lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/imdb/imdb_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     9694 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/imdb/imdb_watchlist.py
--rw-r--r--   0 runner    (1001) docker     (123)    14832 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/imdb/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/components/irc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/irc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/irc/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/irc/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    43486 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/irc/irc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/components/managed_lists/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/managed_lists/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/managed_lists/list_add.py
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/managed_lists/list_clear.py
--rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/managed_lists/list_match.py
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/managed_lists/list_remove.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/components/managed_lists/lists/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/managed_lists/lists/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10612 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/managed_lists/lists/couchpotato_list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/components/managed_lists/lists/entry_list/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/managed_lists/lists/entry_list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11177 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/managed_lists/lists/entry_list/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8582 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/managed_lists/lists/entry_list/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8811 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/managed_lists/lists/entry_list/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/managed_lists/lists/entry_list/entry_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    20355 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/managed_lists/lists/imdb_list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/components/managed_lists/lists/movie_list/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/managed_lists/lists/movie_list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12836 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/managed_lists/lists/movie_list/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     9189 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/managed_lists/lists/movie_list/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/managed_lists/lists/movie_list/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     6656 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/managed_lists/lists/movie_list/movie_list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/components/managed_lists/lists/pending_list/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/managed_lists/lists/pending_list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13350 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/managed_lists/lists/pending_list/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10862 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/managed_lists/lists/pending_list/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5669 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/managed_lists/lists/pending_list/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/managed_lists/lists/pending_list/pending_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     6313 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/managed_lists/lists/plex_watchlist.py
--rw-r--r--   0 runner    (1001) docker     (123)    22641 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/managed_lists/lists/radarr_list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/components/managed_lists/lists/regexp_list/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/managed_lists/lists/regexp_list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4773 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/managed_lists/lists/regexp_list/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/managed_lists/lists/regexp_list/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/managed_lists/lists/regexp_list/regexp_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    11335 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/managed_lists/lists/sonarr_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    14611 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/managed_lists/lists/subtitle_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/managed_lists/lists/thetvdb_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5943 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/managed_lists/lists/yaml_list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/components/notify/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/notify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/notify/notification_framework.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/components/notify/notifiers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/notify/notifiers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/notify/notifiers/bark.py
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/notify/notifiers/cronitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/notify/notifiers/discord.py
--rw-r--r--   0 runner    (1001) docker     (123)     6903 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/notify/notifiers/email.py
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/notify/notifiers/gotify.py
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/notify/notifiers/ifttt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/notify/notifiers/join.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/notify/notifiers/matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/notify/notifiers/microsoftteams.py
--rw-r--r--   0 runner    (1001) docker     (123)     9733 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/notify/notifiers/mqtt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/notify/notifiers/notifymyandroid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/notify/notifiers/ntfysh.py
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/notify/notifiers/prowl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/notify/notifiers/pushalot.py
--rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/notify/notifiers/pushbullet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/notify/notifiers/pushover.py
--rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/notify/notifiers/pushsafer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/notify/notifiers/rapidpush.py
--rw-r--r--   0 runner    (1001) docker     (123)     4976 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/notify/notifiers/slack.py
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/notify/notifiers/sms_ru.py
--rw-r--r--   0 runner    (1001) docker     (123)    19396 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/notify/notifiers/telegram.py
--rw-r--r--   0 runner    (1001) docker     (123)     5978 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/notify/notifiers/toast.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/notify/notifiers/xmpp.py
--rw-r--r--   0 runner    (1001) docker     (123)     6701 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/notify/notify.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/components/parsing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/parsing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/components/parsing/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/parsing/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6859 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/parsing/parsers/parser_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    18622 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/parsing/parsers/parser_guessit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/parsing/parsers/parser_internal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/parsing/plugin_parsing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/components/pending_approval/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/pending_approval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/pending_approval/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/pending_approval/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/pending_approval/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/pending_approval/pending_approval.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/components/rejected/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/rejected/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/rejected/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/rejected/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/rejected/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/rejected/remember_rejected.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/components/scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6652 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/scheduler/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/scheduler/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/components/seen/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/seen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5755 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/seen/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/seen/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     9737 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/seen/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     5422 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/seen/seen.py
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/seen/seen_info_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/seen/seen_movies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/components/series/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/series/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/series/all_series.py
--rw-r--r--   0 runner    (1001) docker     (123)    47046 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/series/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    16878 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/series/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/series/configure_series.py
--rw-r--r--   0 runner    (1001) docker     (123)    56924 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/series/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/series/gen_series.py
--rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/series/internal_estimator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/series/metainfo_series.py
--rw-r--r--   0 runner    (1001) docker     (123)    13829 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/series/next_series_episodes.py
--rw-r--r--   0 runner    (1001) docker     (123)    11235 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/series/next_series_seasons.py
--rw-r--r--   0 runner    (1001) docker     (123)    53384 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/series/series.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/series/series_begin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/series/series_premiere.py
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/series/series_remove.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/series/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/components/sites/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/sites/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/components/sites/sites/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/sites/sites/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/sites/sites/allyoulike.py
--rw-r--r--   0 runner    (1001) docker     (123)    11581 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/sites/sites/alpharatio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/sites/sites/animeindex.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/sites/sites/anirena.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/sites/sites/archetorrent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/sites/sites/argenteam.py
--rw-r--r--   0 runner    (1001) docker     (123)     5307 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/sites/sites/awesomehd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/sites/sites/bakabt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5977 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/sites/sites/btn.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/sites/sites/cinemageddon.py
--rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/sites/sites/cpasbien.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/sites/sites/deadfrog.py
--rw-r--r--   0 runner    (1001) docker     (123)     5254 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/sites/sites/descargas2020.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/sites/sites/ettv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/sites/sites/eztv.py
--rw-r--r--   0 runner    (1001) docker     (123)     9975 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/sites/sites/filelist.py
--rw-r--r--   0 runner    (1001) docker     (123)     5528 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/sites/sites/filelist_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/sites/sites/frenchtorrentdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     6067 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/sites/sites/fuzer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/sites/sites/google_cse.py
--rw-r--r--   0 runner    (1001) docker     (123)     5406 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/sites/sites/hebits.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/sites/sites/hliang.py
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/sites/sites/horriblesubs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8019 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/sites/sites/iptorrents.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/sites/sites/koreus.py
--rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/sites/sites/limetorrents.py
--rw-r--r--   0 runner    (1001) docker     (123)    26068 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/sites/sites/lostfilm.py
--rw-r--r--   0 runner    (1001) docker     (123)     6590 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/sites/sites/magnetdl.py
--rw-r--r--   0 runner    (1001) docker     (123)    10175 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/sites/sites/morethantv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/sites/sites/ncore.py
--rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/sites/sites/newtorrents.py
--rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/sites/sites/newznab.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/sites/sites/nnmclub.py
--rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/sites/sites/nyaa.py
--rw-r--r--   0 runner    (1001) docker     (123)    12146 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/sites/sites/passthepopcorn.py
--rw-r--r--   0 runner    (1001) docker     (123)     7554 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/sites/sites/piratebay.py
--rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/sites/sites/ptn.py
--rw-r--r--   0 runner    (1001) docker     (123)     8007 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/sites/sites/rarbg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/sites/sites/redirect.py
--rw-r--r--   0 runner    (1001) docker     (123)     6621 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/sites/sites/rlsbb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/sites/sites/rmz.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/sites/sites/rss.py
--rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/sites/sites/rutracker.py
--rw-r--r--   0 runner    (1001) docker     (123)     7556 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/sites/sites/serienjunkies.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/sites/sites/shortened.py
--rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/sites/sites/site_1337x.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/sites/sites/site_rutracker.py
--rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/sites/sites/solidtorrents.py
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/sites/sites/torrent_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/sites/sites/torrentday.py
--rw-r--r--   0 runner    (1001) docker     (123)     6106 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/sites/sites/torrentleech.py
--rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/sites/sites/torrentz.py
--rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/sites/sites/wordpress.py
--rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/sites/sites/yts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/sites/urlrewrite.py
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/sites/urlrewrite_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/sites/urlrewriting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/sites/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/components/status/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/status/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8579 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/status/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/status/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5803 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/status/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/status/status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/components/thetvdb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/thetvdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9060 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/thetvdb/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    30428 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/thetvdb/api_tvdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     8196 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/thetvdb/thetvdb_lookup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/components/tmdb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/tmdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/tmdb/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    15019 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/tmdb/api_tmdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/tmdb/tmdb_lookup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/components/trakt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/trakt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8529 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/trakt/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    17362 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/trakt/api_trakt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4248 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/trakt/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    42255 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/trakt/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     7095 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/trakt/next_trakt_episodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/trakt/trakt_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)    20878 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/trakt/trakt_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    13173 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/trakt/trakt_lookup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/components/tvmaze/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/tvmaze/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6374 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/tvmaze/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    26621 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/tvmaze/api_tvmaze.py
--rw-r--r--   0 runner    (1001) docker     (123)     8022 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/tvmaze/tvmaze_lookup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/components/variables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/variables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/variables/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/components/variables/variables.py
--rw-r--r--   0 runner    (1001) docker     (123)    16595 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/config_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    10241 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/db_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    16260 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     6851 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ipc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6662 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    42917 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    23343 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/options.py
--rw-r--r--   0 runner    (1001) docker     (123)    22867 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/plugins/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/cli/check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/cli/cli_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/cli/database.py
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/cli/debug_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/cli/doc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/cli/explain_sql.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/cli/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/cli/inject.py
--rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/cli/perf_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/cli/performance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/cli/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/cli/templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/cli/try_regexp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/cli/web.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/cli/wiki_qualities.py
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/cli/win32_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/plugins/clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12215 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/clients/aria2.py
--rw-r--r--   0 runner    (1001) docker     (123)    31634 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/clients/deluge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/clients/nzbget.py
--rw-r--r--   0 runner    (1001) docker     (123)     9570 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/clients/pyload.py
--rw-r--r--   0 runner    (1001) docker     (123)    15834 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/clients/qbittorrent.py
--rw-r--r--   0 runner    (1001) docker     (123)    25926 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/clients/rtorrent.py
--rw-r--r--   0 runner    (1001) docker     (123)    40090 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/clients/transmission.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/plugins/daemon/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/daemon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/daemon/web_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/plugins/filter/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/filter/abort_if_exists.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/filter/accept_all.py
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/filter/age.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/filter/best_quality.py
--rw-r--r--   0 runner    (1001) docker     (123)     5650 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/filter/content_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/filter/content_size.py
--rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/filter/crossmatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/filter/delay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/filter/duplicates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/filter/exists.py
--rw-r--r--   0 runner    (1001) docker     (123)     7837 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/filter/exists_movie.py
--rw-r--r--   0 runner    (1001) docker     (123)     5901 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/filter/exists_series.py
--rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/filter/if_condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/filter/limit_new.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/filter/magnets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/filter/only_new.py
--rw-r--r--   0 runner    (1001) docker     (123)     6631 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/filter/proper_movies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/filter/quality.py
--rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/filter/regexp.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/filter/require_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     9208 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/filter/rottentomatoes.py
--rw-r--r--   0 runner    (1001) docker     (123)     8190 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/filter/thetvdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     7626 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/filter/timeframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/filter/unique.py
--rw-r--r--   0 runner    (1001) docker     (123)     8431 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/filter/upgrade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/plugins/generic/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/generic/cron_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/generic/db_analyze.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/generic/db_vacuum.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/generic/log_start.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/generic/urlfix.py
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/generic/welcome.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/plugins/input/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/input/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/input/anidb_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    10209 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/input/anilist.py
--rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/input/apple_trailers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/input/betaseries_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    13191 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/input/discover.py
--rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/input/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/input/filmweb_watchlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/input/from_piratebay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/input/from_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     8305 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/input/from_telegram.py
--rw-r--r--   0 runner    (1001) docker     (123)    18418 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/input/gazelle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/input/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)    12035 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/input/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/input/input_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/input/inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/input/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     6361 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/input/kitsu.py
--rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/input/letterboxd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/input/limit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/input/medusa.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/input/mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/input/my_anime_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/input/myepisodes_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/input/next_sonarr_episodes.py
--rw-r--r--   0 runner    (1001) docker     (123)    14811 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/input/npo_watchlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/input/parameterize.py
--rw-r--r--   0 runner    (1001) docker     (123)    18269 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/input/plex.py
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/input/pogcal.py
--rw-r--r--   0 runner    (1001) docker     (123)     7380 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/input/regexp_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/input/rlslog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/input/rottentomatoes_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    24984 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/input/rss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/input/sceper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/input/sickbeard.py
--rw-r--r--   0 runner    (1001) docker     (123)     6800 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/input/tail.py
--rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/input/text.py
--rw-r--r--   0 runner    (1001) docker     (123)    11818 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/input/torznab.py
--rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/input/twitterfeed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/plugins/internal/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10399 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/internal/api_bluray.py
--rw-r--r--   0 runner    (1001) docker     (123)    24482 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/internal/api_rottentomatoes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/internal/change_warn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/plugins/metainfo/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/metainfo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/metainfo/assume_quality.py
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/metainfo/bluray_lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/metainfo/content_size.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/metainfo/media_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/metainfo/metainfo_movie.py
--rw-r--r--   0 runner    (1001) docker     (123)     9551 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/metainfo/nfo_lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/metainfo/nzb_size.py
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/metainfo/quality.py
--rw-r--r--   0 runner    (1001) docker     (123)     4268 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/metainfo/rottentomatoes_lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/metainfo/subtitles_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/metainfo/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/plugins/modify/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/modify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/modify/extension.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/modify/headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6133 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/modify/manipulate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/modify/path_by_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/modify/path_by_space.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/modify/plugin_priority.py
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/modify/regex_extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/modify/reorder_quality.py
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/modify/set_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/modify/sort_by.py
--rw-r--r--   0 runner    (1001) docker     (123)    12213 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/modify/sort_by_weight.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/plugins/operate/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/operate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/operate/abort.py
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/operate/cfscraper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6337 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/operate/cookies.py
--rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/operate/debug_db_sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/operate/debug_warnings.py
--rw-r--r--   0 runner    (1001) docker     (123)     5897 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/operate/digest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/operate/disable.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/operate/disable_phases.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/operate/domain_delay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/operate/entry_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/operate/formlogin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4493 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/operate/free_space.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/operate/include.py
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/operate/interval.py
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/operate/log_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/operate/manual.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/operate/max_reruns.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/operate/pathscrub.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/operate/priority.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/operate/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/operate/rerun.py
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/operate/run_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/operate/sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/operate/sleep.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/operate/spy_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4756 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/operate/template.py
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/operate/verbose.py
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/operate/verbose_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/operate/verify_ssl_certificates.py
--rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/operate/version_checker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/plugins/output/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/output/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    22420 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/output/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/output/download_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/output/dump.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/output/dump_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8469 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/output/exec.py
--rw-r--r--   0 runner    (1001) docker     (123)    14640 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/output/file_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/output/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/output/memusage.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/output/mock_output.py
--rw-r--r--   0 runner    (1001) docker     (123)    10416 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/output/rss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/output/rtorrent_magnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/output/sabnzbd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/output/sns.py
--rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/output/subtitles.py
--rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/output/subtitles_periscope.py
--rw-r--r--   0 runner    (1001) docker     (123)    12628 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/output/subtitles_subliminal.py
--rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/output/symlink.py
--rw-r--r--   0 runner    (1001) docker     (123)     6243 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/output/utorrent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/plugins/services/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/services/kodi_library.py
--rw-r--r--   0 runner    (1001) docker     (123)    10140 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/services/myepisodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/plugins/services/pogcal_acquired.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/resources/
--rw-r--r--   0 runner    (1001) docker     (123)    21065 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/resources/flexget.png
--rw-r--r--   0 runner    (1001) docker     (123)    28391 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/task_queue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/templates/entry/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/templates/entry/default.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/templates/task/
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/templates/task/default.template
--rw-r--r--   0 runner    (1001) docker     (123)     9252 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/templates/task/html.template
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/templates/task/rss.template
--rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/terminal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3513 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/tray_icon.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/ui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/ui/v1/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/ui/v1/app/
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-04-12 15:13:35.000000 FlexGet-3.6.2/flexget/ui/v1/app/app.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/ui/v1/app/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/ui/v1/app/assets/images/
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-04-12 15:13:35.000000 FlexGet-3.6.2/flexget/ui/v1/app/assets/images/header.png
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-04-12 15:13:35.000000 FlexGet-3.6.2/flexget/ui/v1/app/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/ui/v1/app/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)   124988 2023-04-12 15:13:35.000000 FlexGet-3.6.2/flexget/ui/v1/app/fonts/FontAwesome.otf
--rw-r--r--   0 runner    (1001) docker     (123)    76518 2023-04-12 15:13:35.000000 FlexGet-3.6.2/flexget/ui/v1/app/fonts/fontawesome-webfont.eot
--rw-r--r--   0 runner    (1001) docker     (123)   391622 2023-04-12 15:13:35.000000 FlexGet-3.6.2/flexget/ui/v1/app/fonts/fontawesome-webfont.svg
--rw-r--r--   0 runner    (1001) docker     (123)   152796 2023-04-12 15:13:35.000000 FlexGet-3.6.2/flexget/ui/v1/app/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    90412 2023-04-12 15:13:35.000000 FlexGet-3.6.2/flexget/ui/v1/app/fonts/fontawesome-webfont.woff
--rw-r--r--   0 runner    (1001) docker     (123)    71896 2023-04-12 15:13:35.000000 FlexGet-3.6.2/flexget/ui/v1/app/fonts/fontawesome-webfont.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     8728 2023-04-12 15:13:35.000000 FlexGet-3.6.2/flexget/ui/v1/app/fonts/ui-grid.eot
--rw-r--r--   0 runner    (1001) docker     (123)     9065 2023-04-12 15:13:35.000000 FlexGet-3.6.2/flexget/ui/v1/app/fonts/ui-grid.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8564 2023-04-12 15:13:35.000000 FlexGet-3.6.2/flexget/ui/v1/app/fonts/ui-grid.ttf
--rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-04-12 15:13:35.000000 FlexGet-3.6.2/flexget/ui/v1/app/fonts/ui-grid.woff
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/ui/v1/app/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)   167898 2023-04-12 15:13:35.000000 FlexGet-3.6.2/flexget/ui/v1/app/scripts/app.js
--rw-r--r--   0 runner    (1001) docker     (123)    10051 2023-04-12 15:13:35.000000 FlexGet-3.6.2/flexget/ui/v1/app/scripts/splash.js
--rw-r--r--   0 runner    (1001) docker     (123)  6142562 2023-04-12 15:13:35.000000 FlexGet-3.6.2/flexget/ui/v1/app/scripts/vendor.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/ui/v1/app/styles/
--rw-r--r--   0 runner    (1001) docker     (123)   374613 2023-04-12 15:13:35.000000 FlexGet-3.6.2/flexget/ui/v1/app/styles/app.css
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-04-12 15:13:35.000000 FlexGet-3.6.2/flexget/ui/v1/app/styles/splash.css
--rw-r--r--   0 runner    (1001) docker     (123)    86217 2023-04-12 15:13:35.000000 FlexGet-3.6.2/flexget/ui/v1/app/styles/vendor.css
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/bower.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/ui/v1/gulp/
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/gulp/build.js
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/gulp/inject.js
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/gulp/lint.js
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/gulp/proxy.js
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/gulp/scripts.js
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/gulp/server.js
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/gulp/styles.js
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/gulp/test.js
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/gulp/watch.js
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/gulpfile.js
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/karma.conf.js
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/load.failure.html
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/package.json
--rw-r--r--   0 runner    (1001) docker     (123)    18741 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/specs.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/ui/v1/src/
--rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/app.html
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/app.loading.js
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/app.module.js
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/app.scss
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/app.utils.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/ui/v1/src/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/ui/v1/src/assets/icons/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/assets/icons/ic_movie_black_24px.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/ui/v1/src/assets/images/
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/assets/images/header.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/ui/v1/src/blocks/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/ui/v1/src/blocks/error/
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/blocks/error/_error-dialog.scss
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/blocks/error/error-dialog.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/blocks/error/error-dialog.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/blocks/error/error-dialog.tmpl.html
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/blocks/error/error.module.js
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/blocks/error/error.service.js
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/blocks/error/error.service.spec.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/ui/v1/src/blocks/exception/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/blocks/exception/exception.module.js
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/blocks/exception/exception.service.js
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/blocks/exception/exception.service.spec.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/ui/v1/src/blocks/pagination/
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/blocks/pagination/_pagination.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/blocks/pagination/pagination.component.js
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/blocks/pagination/pagination.filter.js
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/blocks/pagination/pagination.module.js
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/blocks/pagination/pagination.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/ui/v1/src/blocks/router/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/blocks/router/router-helper.module.js
--rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/blocks/router/router-helper.provider.js
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/blocks/router/router-helper.provider.spec.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/ui/v1/src/blocks/url-interceptor/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/blocks/url-interceptor/url-interceptor.config.js
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/blocks/url-interceptor/url-interceptor.module.js
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/blocks/url-interceptor/url-interceptor.service.js
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/blocks/url-interceptor/url-interceptor.service.spec.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/ui/v1/src/components/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/ui/v1/src/components/404/
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/components/404/404.component.js
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/components/404/404.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/components/404/404.module.js
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/components/404/404.route.js
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/components/404/404.route.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/components/404/404.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/ui/v1/src/components/auth/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/components/auth/_login.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/components/auth/auth.config.js
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/components/auth/auth.config.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/components/auth/auth.module.js
--rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/components/auth/auth.service.js
--rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/components/auth/auth.service.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/components/auth/login.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/components/auth/login.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/components/auth/login.route.js
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/components/auth/login.route.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/components/auth/login.tmpl.html
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/components/components.module.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/ui/v1/src/components/core/
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/components/core/core.config.js
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/components/core/core.module.js
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/components/core/core.provider.js
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/components/core/core.route.js
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/components/core/core.route.spec.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/ui/v1/src/components/database/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/components/database/_database.scss
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/components/database/database.component.js
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/components/database/database.config.js
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/components/database/database.module.js
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/components/database/database.service.js
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/components/database/database.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/ui/v1/src/components/home/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/components/home/home.component.js
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/components/home/home.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/components/home/home.module.js
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/components/home/home.route.js
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/components/home/home.route.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/components/home/home.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/ui/v1/src/components/sidenav/
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/components/sidenav/_sidenav.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/components/sidenav/sidenav.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/components/sidenav/sidenav.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/components/sidenav/sidenav.module.js
--rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/components/sidenav/sidenav.semver.js
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/components/sidenav/sidenav.service.js
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/components/sidenav/sidenav.service.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/components/sidenav/sidenav.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/ui/v1/src/components/toolbar/
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/components/toolbar/toolbar.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/components/toolbar/toolbar.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/components/toolbar/toolbar.config.js
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/components/toolbar/toolbar.module.js
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/components/toolbar/toolbar.provider.js
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/components/toolbar/toolbar.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/ui/v1/src/components/user/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/components/user/user.module.js
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/construction.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/ui/v1/src/directives/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/directives/directives.module.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/ui/v1/src/directives/palette-background/
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/directives/palette-background/palette-background.directive.js
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/layout.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/config/
--rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/config/config.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/config/config.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/config/config.module.js
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/config/config.route.js
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/config/config.route.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/config/config.service.js
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/config/config.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/execute/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/execute/components/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/execute/components/execute-input/
--rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/execute/components/execute-input/execute-input.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/execute/components/execute-input/execute-input.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/execute/components/execute-input/execute-input.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/execute/components/execute-stream/
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/execute/components/execute-stream/execute-stream.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/execute/components/execute-stream/execute-stream.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/execute/components/execute-stream/execute-stream.tmpl.html
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/execute/execute.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/execute/execute.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/execute/execute.filter.js
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/execute/execute.filter.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/execute/execute.module.js
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/execute/execute.route.js
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/execute/execute.route.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/execute/execute.service.js
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/execute/execute.service.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/execute/execute.tmpl.html
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/execute/execute.tmpl.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/history/
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/history/history.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/history/history.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/history/history.module.js
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/history/history.route.js
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/history/history.route.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/history/history.service.js
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/history/history.service.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/history/history.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/log/
--rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/log/log.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/log/log.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/log/log.module.js
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/log/log.route.js
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/log/log.route.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/log/log.service.js
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/log/log.tmpl.html
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/log/log.tmpl.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/movies/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/movies/components/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/movies/components/add-movie/
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie-input.directive.js
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie-item.component.js
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie-item.tmpl.html
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie.controller.js
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie.service.js
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/movies/components/movie-entry/
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/movies/components/movie-list/
--rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/movies/components/movie-list/movie-list.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/movies/components/movie-list/movie-list.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/movies/components/movie-list/movie-list.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/movies/components/new-list/
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/movies/components/new-list/new-list.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/movies/components/new-list/new-list.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/movies/components/new-list/new-list.tmpl.html
--rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/movies/movies.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/movies/movies.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/movies/movies.module.js
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/movies/movies.route.js
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/movies/movies.route.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/movies/movies.service.js
--rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/movies/movies.service.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/movies/movies.tmpl.html
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/movies/movies.tmpl.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/pending/
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/pending/pending.component.js
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/pending/pending.module.js
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/pending/pending.route.js
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/pending/pending.scss
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/pending/pending.service.js
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/pending/pending.tmpl.html
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/plugins.module.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/schedule/
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/schedule/schedule.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/schedule/schedule.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/schedule/schedule.module.js
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/schedule/schedule.route.js
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/schedule/schedule.route.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/schedule/schedule.service.js
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/schedule/schedule.service.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/schedule/schedule.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/seen/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/seen/components/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/seen/components/seen-entry/
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/seen/components/seen-entry/seen-entry.component.js
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/seen/components/seen-entry/seen-entry.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/seen/components/seen-entry/seen-entry.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/seen/components/seen-field/
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/seen/components/seen-field/seen-field.component.js
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/seen/components/seen-field/seen-field.tmpl.html
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/seen/seen.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/seen/seen.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/seen/seen.module.js
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/seen/seen.route.js
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/seen/seen.route.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/seen/seen.service.js
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/seen/seen.service.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/seen/seen.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/series/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/series/components/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/series/components/episode-release/
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/series/components/episode-release/episode-release.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/series/components/episode-release/episode-release.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/series/components/episode-release/episode-release.scss
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/series/components/episode-release/episode-release.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/series/components/episode-releases/
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/series/components/episode-releases/episode-releases.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/series/components/episode-releases/episode-releases.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/series/components/episode-releases/episode-releases.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/series/components/series-begin-dialog/
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/series/components/series-begin-dialog/series-begin-dialog.component.js
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/series/components/series-begin-dialog/series-begin-dialog.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/series/components/series-entry/
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/series/components/series-entry/series-entry.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/series/components/series-entry/series-entry.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/series/components/series-entry/series-entry.scss
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/series/components/series-entry/series-entry.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/series/components/series-episode/
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/series/components/series-episode/series-episode.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/series/components/series-episode/series-episode.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/series/components/series-episode/series-episode.scss
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/series/components/series-episode/series-episode.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/series/components/series-episodes/
--rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.scss
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.tmpl.html
--rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/series/series.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/series/series.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/series/series.module.js
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/series/series.route.js
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/series/series.route.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/series/series.service.js
--rw-r--r--   0 runner    (1001) docker     (123)    11141 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/series/series.service.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/series/series.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/server/
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/server/loading-dialog.component.js
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/server/loading-dialog.tmpl.html
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/server/server.config.js
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/server/server.module.js
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/server/server.service.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/status/
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/status/status.component.js
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/status/status.module.js
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/status/status.route.js
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/status/status.service.js
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/status/status.tmpl.html
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/plugins/status/status.tmpl.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/ui/v1/src/scss/
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/scss/_header.scss
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/scss/_loading-bar.scss
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/scss/_variables.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/scss/flexget.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/ui/v1/src/services/
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/src/services/schema.service.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/ui/v1/tests-mock-data/
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/tests-mock-data/config.js
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/tests-mock-data/execute.js
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/tests-mock-data/history.js
--rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/tests-mock-data/movie_list.js
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/tests-mock-data/registerPlugin.js
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/tests-mock-data/schedules.js
--rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/tests-mock-data/seen.js
--rw-r--r--   0 runner    (1001) docker     (123)    11128 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/tests-mock-data/series.js
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v1/tests-mock-data/states.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/ui/v2/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/ui/v2/dist/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/ui/v2/dist/assets/
--rw-r--r--   0 runner    (1001) docker     (123)    15872 2023-04-12 15:13:36.000000 FlexGet-3.6.2/flexget/ui/v2/dist/assets/020c97dc8e0463259c2f9df929bb0c69.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     8658 2023-04-12 15:13:36.000000 FlexGet-3.6.2/flexget/ui/v2/dist/assets/14.18cf3ab07df2cff9c980.js
--rw-r--r--   0 runner    (1001) docker     (123)    12291 2023-04-12 15:13:36.000000 FlexGet-3.6.2/flexget/ui/v2/dist/assets/14.18cf3ab07df2cff9c980.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    17448 2023-04-12 15:13:36.000000 FlexGet-3.6.2/flexget/ui/v2/dist/assets/14286f3ba79c6627433572dfa925202e.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     8363 2023-04-12 15:13:36.000000 FlexGet-3.6.2/flexget/ui/v2/dist/assets/15.df643f032866e7897440.js
--rw-r--r--   0 runner    (1001) docker     (123)    33576 2023-04-12 15:13:36.000000 FlexGet-3.6.2/flexget/ui/v2/dist/assets/15.df643f032866e7897440.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-04-12 15:13:36.000000 FlexGet-3.6.2/flexget/ui/v2/dist/assets/16.d99413fe0332d02516c9.js
--rw-r--r--   0 runner    (1001) docker     (123)    10089 2023-04-12 15:13:36.000000 FlexGet-3.6.2/flexget/ui/v2/dist/assets/16.d99413fe0332d02516c9.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    15816 2023-04-12 15:13:36.000000 FlexGet-3.6.2/flexget/ui/v2/dist/assets/2735a3a69b509faf3577afd25bdf552e.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    22020 2023-04-12 15:13:36.000000 FlexGet-3.6.2/flexget/ui/v2/dist/assets/288ad9c6e8b43cf02443a1f499bdf67e.woff
--rw-r--r--   0 runner    (1001) docker     (123)    22304 2023-04-12 15:13:36.000000 FlexGet-3.6.2/flexget/ui/v2/dist/assets/28f9151055c950874d2c6803a39b425b.woff
--rw-r--r--   0 runner    (1001) docker     (123)    47404 2023-04-12 15:13:36.000000 FlexGet-3.6.2/flexget/ui/v2/dist/assets/35bb8d560db5205616671eab8c4d0303.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    15736 2023-04-12 15:13:36.000000 FlexGet-3.6.2/flexget/ui/v2/dist/assets/479970ffb74f2117317f9d24d9e317fe.woff2
--rw-r--r--   0 runner    (1001) docker     (123)  1150672 2023-04-12 15:13:36.000000 FlexGet-3.6.2/flexget/ui/v2/dist/assets/4cb446d4c3b18f2f69df.worker.js
--rw-r--r--   0 runner    (1001) docker     (123)  4396877 2023-04-12 15:13:36.000000 FlexGet-3.6.2/flexget/ui/v2/dist/assets/4cb446d4c3b18f2f69df.worker.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    22204 2023-04-12 15:13:36.000000 FlexGet-3.6.2/flexget/ui/v2/dist/assets/4df32891a5f2f98a363314f595482e08.woff
--rw-r--r--   0 runner    (1001) docker     (123)    17324 2023-04-12 15:13:36.000000 FlexGet-3.6.2/flexget/ui/v2/dist/assets/51521a2a8da71e50d871ac6fd2187e87.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    20368 2023-04-12 15:13:36.000000 FlexGet-3.6.2/flexget/ui/v2/dist/assets/5cb7edfceb233100075dc9a1e12e8da3.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20268 2023-04-12 15:13:36.000000 FlexGet-3.6.2/flexget/ui/v2/dist/assets/60fa3c0614b8fb2f394fa29944c21540.woff
--rw-r--r--   0 runner    (1001) docker     (123)   126767 2023-04-12 15:13:36.000000 FlexGet-3.6.2/flexget/ui/v2/dist/assets/68c852c85ea688dfa942.worker.js
--rw-r--r--   0 runner    (1001) docker     (123)   560902 2023-04-12 15:13:36.000000 FlexGet-3.6.2/flexget/ui/v2/dist/assets/68c852c85ea688dfa942.worker.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    15808 2023-04-12 15:13:36.000000 FlexGet-3.6.2/flexget/ui/v2/dist/assets/7370c3679472e9560965ff48a4399d0b.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    21588 2023-04-12 15:13:36.000000 FlexGet-3.6.2/flexget/ui/v2/dist/assets/81f57861ed4ac74741f5671e1dff2fd9.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20464 2023-04-12 15:13:36.000000 FlexGet-3.6.2/flexget/ui/v2/dist/assets/87284894879f5b1c229cb49c8ff6decc.woff
--rw-r--r--   0 runner    (1001) docker     (123)    15712 2023-04-12 15:13:36.000000 FlexGet-3.6.2/flexget/ui/v2/dist/assets/9b3766ef4a402ad3fdeef7501a456512.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    70594 2023-04-12 15:13:36.000000 FlexGet-3.6.2/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.css
--rw-r--r--   0 runner    (1001) docker     (123)    91826 2023-04-12 15:13:36.000000 FlexGet-3.6.2/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.css.map
--rw-r--r--   0 runner    (1001) docker     (123)   562036 2023-04-12 15:13:36.000000 FlexGet-3.6.2/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.js
--rw-r--r--   0 runner    (1001) docker     (123)  2069487 2023-04-12 15:13:36.000000 FlexGet-3.6.2/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-04-12 15:13:36.000000 FlexGet-3.6.2/flexget/ui/v2/dist/assets/EntryListPlugin.c4b35103ad1660e69c44.js
--rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-04-12 15:13:36.000000 FlexGet-3.6.2/flexget/ui/v2/dist/assets/EntryListPlugin.c4b35103ad1660e69c44.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    24029 2023-04-12 15:13:36.000000 FlexGet-3.6.2/flexget/ui/v2/dist/assets/HistoryPlugin.0201ee39aecaa7452270.js
--rw-r--r--   0 runner    (1001) docker     (123)    41804 2023-04-12 15:13:36.000000 FlexGet-3.6.2/flexget/ui/v2/dist/assets/HistoryPlugin.0201ee39aecaa7452270.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-04-12 15:13:36.000000 FlexGet-3.6.2/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.css
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-04-12 15:13:36.000000 FlexGet-3.6.2/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.css.map
--rw-r--r--   0 runner    (1001) docker     (123)   148218 2023-04-12 15:13:36.000000 FlexGet-3.6.2/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.js
--rw-r--r--   0 runner    (1001) docker     (123)   618494 2023-04-12 15:13:36.000000 FlexGet-3.6.2/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-04-12 15:13:36.000000 FlexGet-3.6.2/flexget/ui/v2/dist/assets/MovieListPlugin.17e519c9d031c1cd9477.js
--rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-04-12 15:13:36.000000 FlexGet-3.6.2/flexget/ui/v2/dist/assets/MovieListPlugin.17e519c9d031c1cd9477.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     6581 2023-04-12 15:13:36.000000 FlexGet-3.6.2/flexget/ui/v2/dist/assets/PendingListPlugin.7ddbee4abf831e808220.js
--rw-r--r--   0 runner    (1001) docker     (123)    10858 2023-04-12 15:13:36.000000 FlexGet-3.6.2/flexget/ui/v2/dist/assets/PendingListPlugin.7ddbee4abf831e808220.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    39851 2023-04-12 15:13:36.000000 FlexGet-3.6.2/flexget/ui/v2/dist/assets/SeriesPlugin.f46122b2f63739898cd5.js
--rw-r--r--   0 runner    (1001) docker     (123)    71452 2023-04-12 15:13:36.000000 FlexGet-3.6.2/flexget/ui/v2/dist/assets/SeriesPlugin.f46122b2f63739898cd5.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-04-12 15:13:36.000000 FlexGet-3.6.2/flexget/ui/v2/dist/assets/TasksHomeCard.0f1a9b4992c80e636a4f.js
--rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-04-12 15:13:36.000000 FlexGet-3.6.2/flexget/ui/v2/dist/assets/TasksHomeCard.0f1a9b4992c80e636a4f.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    57772 2023-04-12 15:13:36.000000 FlexGet-3.6.2/flexget/ui/v2/dist/assets/TasksPlugin.78a8bc05a72c9f25d7c3.js
--rw-r--r--   0 runner    (1001) docker     (123)   225286 2023-04-12 15:13:36.000000 FlexGet-3.6.2/flexget/ui/v2/dist/assets/TasksPlugin.78a8bc05a72c9f25d7c3.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    20356 2023-04-12 15:13:36.000000 FlexGet-3.6.2/flexget/ui/v2/dist/assets/adcde98f1d584de52060ad7b16373da3.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20348 2023-04-12 15:13:36.000000 FlexGet-3.6.2/flexget/ui/v2/dist/assets/b00849e00f4c2331cddd8ffb44a6720b.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20392 2023-04-12 15:13:36.000000 FlexGet-3.6.2/flexget/ui/v2/dist/assets/bb1e4dc6333675d11ada2e857e7f95d7.woff
--rw-r--r--   0 runner    (1001) docker     (123)    17020 2023-04-12 15:13:36.000000 FlexGet-3.6.2/flexget/ui/v2/dist/assets/da0e717829e033a69dec97f1e155ae42.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    17316 2023-04-12 15:13:36.000000 FlexGet-3.6.2/flexget/ui/v2/dist/assets/db4a2a231f52e497c0191e8966b0ee58.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    46199 2023-04-12 15:13:36.000000 FlexGet-3.6.2/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin.5c83b88e8b99cf5955dd.js
--rw-r--r--   0 runner    (1001) docker     (123)    91316 2023-04-12 15:13:36.000000 FlexGet-3.6.2/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin.5c83b88e8b99cf5955dd.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    50808 2023-04-12 15:13:36.000000 FlexGet-3.6.2/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~SeriesPlugin.82114e5d38c3136caad1.js
--rw-r--r--   0 runner    (1001) docker     (123)   136381 2023-04-12 15:13:36.000000 FlexGet-3.6.2/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~SeriesPlugin.82114e5d38c3136caad1.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    11083 2023-04-12 15:13:36.000000 FlexGet-3.6.2/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~TasksPlugin.17910c3356c98ded086b.js
--rw-r--r--   0 runner    (1001) docker     (123)    52623 2023-04-12 15:13:36.000000 FlexGet-3.6.2/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~TasksPlugin.17910c3356c98ded086b.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    17520 2023-04-12 15:13:36.000000 FlexGet-3.6.2/flexget/ui/v2/dist/assets/ebf6d1640ccddb99fb49f73c052c55a8.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    15784 2023-04-12 15:13:36.000000 FlexGet-3.6.2/flexget/ui/v2/dist/assets/ef7c6637c68f269a882e73bcb57a7f6a.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    17008 2023-04-12 15:13:36.000000 FlexGet-3.6.2/flexget/ui/v2/dist/assets/f8b1df51ba843179fa1cc9b53d58127a.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    21704 2023-04-12 15:13:36.000000 FlexGet-3.6.2/flexget/ui/v2/dist/assets/f9e8e590b4e0f1ff83469bb2a55b8488.woff
--rw-r--r--   0 runner    (1001) docker     (123)    21952 2023-04-12 15:13:36.000000 FlexGet-3.6.2/flexget/ui/v2/dist/assets/fe65b8335ee19dd944289f9ed3178c78.woff
--rw-r--r--   0 runner    (1001) docker     (123)    88547 2023-04-12 15:13:36.000000 FlexGet-3.6.2/flexget/ui/v2/dist/assets/main.cce4d52f6988bfadab4f.js
--rw-r--r--   0 runner    (1001) docker     (123)   130389 2023-04-12 15:13:36.000000 FlexGet-3.6.2/flexget/ui/v2/dist/assets/main.cce4d52f6988bfadab4f.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    77360 2023-04-12 15:13:36.000000 FlexGet-3.6.2/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.css
--rw-r--r--   0 runner    (1001) docker     (123)    95799 2023-04-12 15:13:36.000000 FlexGet-3.6.2/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.css.map
--rw-r--r--   0 runner    (1001) docker     (123)  2285898 2023-04-12 15:13:36.000000 FlexGet-3.6.2/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.js
--rw-r--r--   0 runner    (1001) docker     (123)  9410938 2023-04-12 15:13:36.000000 FlexGet-3.6.2/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-04-12 15:13:36.000000 FlexGet-3.6.2/flexget/ui/v2/dist/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/ui/v2/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12447 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/utils/bittorrent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     9149 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/utils/cached_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     6458 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/utils/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/utils/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     4616 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/utils/lazy_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/utils/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:13:40.000000 FlexGet-3.6.2/flexget/utils/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/utils/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/utils/parsers/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/utils/parsers/movie.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/utils/parsers/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    28532 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/utils/parsers/series.py
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/utils/pathscrub.py
--rw-r--r--   0 runner    (1001) docker     (123)    19242 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/utils/qualities.py
--rw-r--r--   0 runner    (1001) docker     (123)    11247 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/utils/requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     8048 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/utils/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     8202 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/utils/simple_persistence.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/utils/soup.py
--rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/utils/sqlalchemy_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11466 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/utils/template.py
--rw-r--r--   0 runner    (1001) docker     (123)    16990 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/utils/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     7817 2023-04-12 15:13:10.000000 FlexGet-3.6.2/flexget/webserver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3850 2023-04-12 15:13:10.000000 FlexGet-3.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     6548 2023-04-12 15:13:10.000000 FlexGet-3.6.2/requirements-docker.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-04-12 15:13:10.000000 FlexGet-3.6.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 15:13:40.000000 FlexGet-3.6.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/FlexGet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-04-15 15:12:14.000000 FlexGet-3.6.3/FlexGet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    39106 2023-04-15 15:12:14.000000 FlexGet-3.6.3/FlexGet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 15:12:14.000000 FlexGet-3.6.3/FlexGet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-15 15:12:14.000000 FlexGet-3.6.3/FlexGet.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-04-15 15:12:14.000000 FlexGet-3.6.3/FlexGet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-15 15:12:14.000000 FlexGet-3.6.3/FlexGet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-04-15 15:11:46.000000 FlexGet-3.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-15 15:11:46.000000 FlexGet-3.6.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-04-15 15:12:14.000000 FlexGet-3.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-04-15 15:11:46.000000 FlexGet-3.6.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-04-15 15:11:46.000000 FlexGet-3.6.3/dev-requirements-extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-04-15 15:11:46.000000 FlexGet-3.6.3/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-15 15:12:08.000000 FlexGet-3.6.3/flexget/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15579 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/api/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/api/core/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/api/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/api/core/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/api/core/cached.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/api/core/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/api/core/format_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/api/core/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/api/core/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20576 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/api/core/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22039 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/api/core/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/api/core/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/api/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     7051 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/api/templates/api_response.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10279 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/api/templates/swagger-ui.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/components/archive/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/archive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/archive/archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10506 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/archive/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6014 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/archive/db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/components/archives/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/archives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/archives/archives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7517 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/archives/decompress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7337 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/archives/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/components/backlog/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/backlog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/backlog/backlog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/backlog/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/backlog/db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/components/bittorrent/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/bittorrent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/bittorrent/convert_magnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/bittorrent/magnet_info_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/bittorrent/private_torrents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/bittorrent/torrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10080 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/bittorrent/torrent_alive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/bittorrent/torrent_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8533 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/bittorrent/torrent_match.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/bittorrent/torrent_scrub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/bittorrent/torrent_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/bittorrent/trackers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/components/emby/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/emby/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83287 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/emby/api_emby.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/emby/emby_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/emby/emby_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/emby/emby_refresh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4954 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/emby/emby_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/emby/from_emby.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/components/estimate_release/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/estimate_release/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/estimate_release/estimate_release.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/components/estimate_release/estimators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/estimate_release/estimators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/estimate_release/estimators/est_movies_bluray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/estimate_release/estimators/est_released_movies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/estimate_release/estimators/est_series_tvmaze.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/components/failed/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/failed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/failed/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/failed/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/failed/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/failed/retry_failed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/components/ftp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/ftp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8431 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/ftp/ftp_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/ftp/ftp_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15674 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/ftp/sftp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23191 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/ftp/sftp_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/components/history/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/history/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/history/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/history/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/history/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/history/history.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/components/imdb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/imdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/imdb/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6883 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/imdb/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12539 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/imdb/from_imdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10772 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/imdb/imdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13043 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/imdb/imdb_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/imdb/imdb_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9686 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/imdb/imdb_watchlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14832 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/imdb/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/components/irc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/irc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/irc/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/irc/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43513 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/irc/irc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/components/managed_lists/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/managed_lists/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/managed_lists/list_add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/managed_lists/list_clear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/managed_lists/list_match.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/managed_lists/list_remove.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/components/managed_lists/lists/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/managed_lists/lists/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10612 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/managed_lists/lists/couchpotato_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/components/managed_lists/lists/entry_list/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/managed_lists/lists/entry_list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11177 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/managed_lists/lists/entry_list/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8582 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/managed_lists/lists/entry_list/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8811 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/managed_lists/lists/entry_list/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/managed_lists/lists/entry_list/entry_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20345 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/managed_lists/lists/imdb_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/components/managed_lists/lists/movie_list/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/managed_lists/lists/movie_list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12836 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/managed_lists/lists/movie_list/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9189 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/managed_lists/lists/movie_list/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7060 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/managed_lists/lists/movie_list/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6656 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/managed_lists/lists/movie_list/movie_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/components/managed_lists/lists/pending_list/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/managed_lists/lists/pending_list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13350 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/managed_lists/lists/pending_list/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10862 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/managed_lists/lists/pending_list/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5669 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/managed_lists/lists/pending_list/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/managed_lists/lists/pending_list/pending_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6305 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/managed_lists/lists/plex_watchlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22641 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/managed_lists/lists/radarr_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/components/managed_lists/lists/regexp_list/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/managed_lists/lists/regexp_list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4773 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/managed_lists/lists/regexp_list/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/managed_lists/lists/regexp_list/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/managed_lists/lists/regexp_list/regexp_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11335 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/managed_lists/lists/sonarr_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14611 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/managed_lists/lists/subtitle_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/managed_lists/lists/thetvdb_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/managed_lists/lists/yaml_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/components/notify/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/notify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/notify/notification_framework.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/components/notify/notifiers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/notify/notifiers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/notify/notifiers/bark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/notify/notifiers/cronitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/notify/notifiers/discord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6903 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/notify/notifiers/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/notify/notifiers/gotify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/notify/notifiers/ifttt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/notify/notifiers/join.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/notify/notifiers/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/notify/notifiers/microsoftteams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9758 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/notify/notifiers/mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/notify/notifiers/notifymyandroid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/notify/notifiers/ntfysh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/notify/notifiers/prowl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/notify/notifiers/pushalot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/notify/notifiers/pushbullet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/notify/notifiers/pushover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/notify/notifiers/pushsafer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/notify/notifiers/rapidpush.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4976 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/notify/notifiers/slack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/notify/notifiers/sms_ru.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19376 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/notify/notifiers/telegram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5846 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/notify/notifiers/toast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/notify/notifiers/xmpp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6701 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/notify/notify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/components/parsing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/parsing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/components/parsing/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/parsing/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6859 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/parsing/parsers/parser_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18674 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/parsing/parsers/parser_guessit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/parsing/parsers/parser_internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/parsing/plugin_parsing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/components/pending_approval/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/pending_approval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7055 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/pending_approval/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/pending_approval/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/pending_approval/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/pending_approval/pending_approval.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/components/rejected/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/rejected/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/rejected/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/rejected/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/rejected/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/rejected/remember_rejected.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/components/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6652 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/scheduler/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6700 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/scheduler/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/components/seen/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/seen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5755 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/seen/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/seen/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9699 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/seen/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5422 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/seen/seen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/seen/seen_info_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/seen/seen_movies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/components/series/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/series/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/series/all_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47045 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/series/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16878 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/series/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/series/configure_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57010 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/series/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/series/gen_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/series/internal_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/series/metainfo_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13829 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/series/next_series_episodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11235 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/series/next_series_seasons.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53410 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/series/series.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/series/series_begin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/series/series_premiere.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/series/series_remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/series/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/components/sites/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/sites/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/components/sites/sites/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/sites/sites/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/sites/sites/allyoulike.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11547 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/sites/sites/alpharatio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/sites/sites/animeindex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/sites/sites/anirena.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/sites/sites/archetorrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/sites/sites/argenteam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5307 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/sites/sites/awesomehd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/sites/sites/bakabt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5977 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/sites/sites/btn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/sites/sites/cinemageddon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/sites/sites/cpasbien.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/sites/sites/deadfrog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5254 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/sites/sites/descargas2020.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/sites/sites/ettv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/sites/sites/eztv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9937 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/sites/sites/filelist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5528 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/sites/sites/filelist_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/sites/sites/frenchtorrentdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6067 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/sites/sites/fuzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/sites/sites/google_cse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5406 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/sites/sites/hebits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/sites/sites/hliang.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/sites/sites/horriblesubs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7992 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/sites/sites/iptorrents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/sites/sites/koreus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/sites/sites/limetorrents.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26049 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/sites/sites/lostfilm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6559 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/sites/sites/magnetdl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10141 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/sites/sites/morethantv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/sites/sites/ncore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/sites/sites/newtorrents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/sites/sites/newznab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/sites/sites/nnmclub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/sites/sites/nyaa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12112 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/sites/sites/passthepopcorn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/sites/sites/piratebay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/sites/sites/ptn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8007 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/sites/sites/rarbg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/sites/sites/redirect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6621 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/sites/sites/rlsbb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/sites/sites/rmz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/sites/sites/rss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/sites/sites/rutracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7556 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/sites/sites/serienjunkies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/sites/sites/shortened.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/sites/sites/site_1337x.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/sites/sites/site_rutracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/sites/sites/solidtorrents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/sites/sites/torrent_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/sites/sites/torrentday.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6106 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/sites/sites/torrentleech.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/sites/sites/torrentz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/sites/sites/wordpress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/sites/sites/yts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/sites/urlrewrite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/sites/urlrewrite_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/sites/urlrewriting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/sites/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/components/status/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/status/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8579 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/status/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/status/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5803 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/status/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/status/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/components/thetvdb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/thetvdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9060 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/thetvdb/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30407 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/thetvdb/api_tvdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8205 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/thetvdb/thetvdb_lookup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/components/tmdb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/tmdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/tmdb/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15012 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/tmdb/api_tmdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/tmdb/tmdb_lookup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/components/trakt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/trakt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8529 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/trakt/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17362 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/trakt/api_trakt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/trakt/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42255 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/trakt/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7095 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/trakt/next_trakt_episodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/trakt/trakt_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20878 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/trakt/trakt_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13150 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/trakt/trakt_lookup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/components/tvmaze/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/tvmaze/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6374 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/tvmaze/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26621 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/tvmaze/api_tvmaze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/tvmaze/tvmaze_lookup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/components/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/variables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/variables/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/components/variables/variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16575 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/config_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10241 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/db_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16254 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6851 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ipc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42711 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23353 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22842 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/plugins/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/cli/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/cli/cli_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/cli/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/cli/debug_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/cli/doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/cli/explain_sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/cli/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/cli/inject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/cli/perf_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/cli/performance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/cli/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/cli/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/cli/try_regexp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/cli/web.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/cli/wiki_qualities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/cli/win32_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/plugins/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12254 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/clients/aria2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31634 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/clients/deluge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/clients/nzbget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9570 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/clients/pyload.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15829 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/clients/qbittorrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25915 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/clients/rtorrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40075 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/clients/transmission.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/plugins/daemon/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/daemon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/daemon/web_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/plugins/filter/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/filter/abort_if_exists.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/filter/accept_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/filter/age.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/filter/best_quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5650 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/filter/content_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/filter/content_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/filter/crossmatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/filter/delay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/filter/duplicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/filter/exists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7837 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/filter/exists_movie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5901 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/filter/exists_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/filter/if_condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/filter/limit_new.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/filter/magnets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/filter/only_new.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6631 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/filter/proper_movies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/filter/quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/filter/regexp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/filter/require_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9208 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/filter/rottentomatoes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8190 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/filter/thetvdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7626 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/filter/timeframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/filter/unique.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8431 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/filter/upgrade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/plugins/generic/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/generic/cron_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/generic/db_analyze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/generic/db_vacuum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/generic/log_start.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/generic/urlfix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/generic/welcome.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/plugins/input/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/input/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/input/anidb_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10209 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/input/anilist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/input/apple_trailers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/input/betaseries_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13179 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/input/discover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/input/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/input/filmweb_watchlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/input/from_piratebay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/input/from_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8287 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/input/from_telegram.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18418 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/input/gazelle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/input/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12035 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/input/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/input/input_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/input/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/input/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6361 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/input/kitsu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/input/letterboxd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/input/limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/input/medusa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/input/mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/input/my_anime_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/input/myepisodes_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/input/next_sonarr_episodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14774 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/input/npo_watchlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/input/parameterize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18273 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/input/plex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/input/pogcal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7380 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/input/regexp_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/input/rlslog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/input/rottentomatoes_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24984 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/input/rss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/input/sceper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/input/sickbeard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6800 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/input/tail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/input/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11818 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/input/torznab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/input/twitterfeed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/plugins/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10389 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/internal/api_bluray.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24482 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/internal/api_rottentomatoes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/internal/change_warn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/plugins/metainfo/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/metainfo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/metainfo/assume_quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/metainfo/bluray_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/metainfo/content_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/metainfo/media_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/metainfo/metainfo_movie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9551 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/metainfo/nfo_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/metainfo/nzb_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/metainfo/quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/metainfo/rottentomatoes_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/metainfo/subtitles_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/metainfo/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/plugins/modify/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/modify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/modify/extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/modify/headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6133 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/modify/manipulate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/modify/path_by_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/modify/path_by_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/modify/plugin_priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/modify/regex_extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/modify/reorder_quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/modify/set_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/modify/sort_by.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12209 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/modify/sort_by_weight.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/plugins/operate/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/operate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/operate/abort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/operate/cfscraper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6347 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/operate/cookies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/operate/debug_db_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/operate/debug_warnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5897 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/operate/digest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/operate/disable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/operate/disable_phases.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/operate/domain_delay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/operate/entry_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/operate/formlogin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4493 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/operate/free_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/operate/include.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/operate/interval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/operate/log_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/operate/manual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/operate/max_reruns.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/operate/pathscrub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/operate/priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/operate/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/operate/rerun.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/operate/run_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/operate/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/operate/sleep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/operate/spy_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4756 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/operate/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/operate/verbose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/operate/verbose_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/operate/verify_ssl_certificates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/operate/version_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/plugins/output/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/output/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22419 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/output/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/output/download_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/output/dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/output/dump_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8469 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/output/exec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14640 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/output/file_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/output/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/output/memusage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/output/mock_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10416 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/output/rss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/output/rtorrent_magnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/output/sabnzbd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/output/sns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/output/subtitles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/output/subtitles_periscope.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12628 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/output/subtitles_subliminal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5962 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/output/symlink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6238 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/output/utorrent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/plugins/services/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/services/kodi_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10140 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/services/myepisodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/plugins/services/pogcal_acquired.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)    21065 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/resources/flexget.png
+-rw-r--r--   0 runner    (1001) docker     (123)    28358 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/task_queue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/templates/entry/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/templates/entry/default.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/templates/task/
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/templates/task/default.template
+-rw-r--r--   0 runner    (1001) docker     (123)     9252 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/templates/task/html.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/templates/task/rss.template
+-rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/terminal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/tray_icon.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/ui/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/ui/v1/app/
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-04-15 15:12:09.000000 FlexGet-3.6.3/flexget/ui/v1/app/app.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/ui/v1/app/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/ui/v1/app/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-04-15 15:12:09.000000 FlexGet-3.6.3/flexget/ui/v1/app/assets/images/header.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-04-15 15:12:09.000000 FlexGet-3.6.3/flexget/ui/v1/app/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/ui/v1/app/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   124988 2023-04-15 15:12:09.000000 FlexGet-3.6.3/flexget/ui/v1/app/fonts/FontAwesome.otf
+-rw-r--r--   0 runner    (1001) docker     (123)    76518 2023-04-15 15:12:09.000000 FlexGet-3.6.3/flexget/ui/v1/app/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   391622 2023-04-15 15:12:09.000000 FlexGet-3.6.3/flexget/ui/v1/app/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   152796 2023-04-15 15:12:09.000000 FlexGet-3.6.3/flexget/ui/v1/app/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    90412 2023-04-15 15:12:09.000000 FlexGet-3.6.3/flexget/ui/v1/app/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    71896 2023-04-15 15:12:09.000000 FlexGet-3.6.3/flexget/ui/v1/app/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     8728 2023-04-15 15:12:09.000000 FlexGet-3.6.3/flexget/ui/v1/app/fonts/ui-grid.eot
+-rw-r--r--   0 runner    (1001) docker     (123)     9065 2023-04-15 15:12:09.000000 FlexGet-3.6.3/flexget/ui/v1/app/fonts/ui-grid.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8564 2023-04-15 15:12:09.000000 FlexGet-3.6.3/flexget/ui/v1/app/fonts/ui-grid.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-04-15 15:12:09.000000 FlexGet-3.6.3/flexget/ui/v1/app/fonts/ui-grid.woff
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/ui/v1/app/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)   167898 2023-04-15 15:12:09.000000 FlexGet-3.6.3/flexget/ui/v1/app/scripts/app.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10051 2023-04-15 15:12:09.000000 FlexGet-3.6.3/flexget/ui/v1/app/scripts/splash.js
+-rw-r--r--   0 runner    (1001) docker     (123)  6142562 2023-04-15 15:12:09.000000 FlexGet-3.6.3/flexget/ui/v1/app/scripts/vendor.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/ui/v1/app/styles/
+-rw-r--r--   0 runner    (1001) docker     (123)   374613 2023-04-15 15:12:09.000000 FlexGet-3.6.3/flexget/ui/v1/app/styles/app.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-04-15 15:12:09.000000 FlexGet-3.6.3/flexget/ui/v1/app/styles/splash.css
+-rw-r--r--   0 runner    (1001) docker     (123)    86217 2023-04-15 15:12:09.000000 FlexGet-3.6.3/flexget/ui/v1/app/styles/vendor.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/bower.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/ui/v1/gulp/
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/gulp/build.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/gulp/inject.js
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/gulp/lint.js
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/gulp/proxy.js
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/gulp/scripts.js
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/gulp/server.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/gulp/styles.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/gulp/test.js
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/gulp/watch.js
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/gulpfile.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/karma.conf.js
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/load.failure.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18741 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/specs.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/ui/v1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/app.html
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/app.loading.js
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/app.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/app.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/app.utils.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/ui/v1/src/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/ui/v1/src/assets/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/assets/icons/ic_movie_black_24px.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/ui/v1/src/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/assets/images/header.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/ui/v1/src/blocks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/ui/v1/src/blocks/error/
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/blocks/error/_error-dialog.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/blocks/error/error-dialog.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/blocks/error/error-dialog.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/blocks/error/error-dialog.tmpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/blocks/error/error.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/blocks/error/error.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/blocks/error/error.service.spec.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/ui/v1/src/blocks/exception/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/blocks/exception/exception.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/blocks/exception/exception.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/blocks/exception/exception.service.spec.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/ui/v1/src/blocks/pagination/
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/blocks/pagination/_pagination.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/blocks/pagination/pagination.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/blocks/pagination/pagination.filter.js
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/blocks/pagination/pagination.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/blocks/pagination/pagination.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/ui/v1/src/blocks/router/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/blocks/router/router-helper.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/blocks/router/router-helper.provider.js
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/blocks/router/router-helper.provider.spec.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/ui/v1/src/blocks/url-interceptor/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/blocks/url-interceptor/url-interceptor.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/blocks/url-interceptor/url-interceptor.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/blocks/url-interceptor/url-interceptor.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/blocks/url-interceptor/url-interceptor.service.spec.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/ui/v1/src/components/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/ui/v1/src/components/404/
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/components/404/404.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/components/404/404.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/components/404/404.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/components/404/404.route.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/components/404/404.route.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/components/404/404.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/ui/v1/src/components/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/components/auth/_login.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/components/auth/auth.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/components/auth/auth.config.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/components/auth/auth.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/components/auth/auth.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/components/auth/auth.service.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/components/auth/login.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/components/auth/login.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/components/auth/login.route.js
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/components/auth/login.route.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/components/auth/login.tmpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/components/components.module.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/ui/v1/src/components/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/components/core/core.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/components/core/core.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/components/core/core.provider.js
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/components/core/core.route.js
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/components/core/core.route.spec.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/ui/v1/src/components/database/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/components/database/_database.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/components/database/database.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/components/database/database.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/components/database/database.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/components/database/database.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/components/database/database.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/ui/v1/src/components/home/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/components/home/home.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/components/home/home.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/components/home/home.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/components/home/home.route.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/components/home/home.route.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/components/home/home.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/ui/v1/src/components/sidenav/
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/components/sidenav/_sidenav.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/components/sidenav/sidenav.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/components/sidenav/sidenav.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/components/sidenav/sidenav.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/components/sidenav/sidenav.semver.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/components/sidenav/sidenav.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/components/sidenav/sidenav.service.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/components/sidenav/sidenav.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/ui/v1/src/components/toolbar/
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/components/toolbar/toolbar.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/components/toolbar/toolbar.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/components/toolbar/toolbar.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/components/toolbar/toolbar.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/components/toolbar/toolbar.provider.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/components/toolbar/toolbar.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/ui/v1/src/components/user/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/components/user/user.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/construction.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/ui/v1/src/directives/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/directives/directives.module.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/ui/v1/src/directives/palette-background/
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/directives/palette-background/palette-background.directive.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/layout.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/config/config.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/config/config.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/config/config.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/config/config.route.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/config/config.route.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/config/config.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/config/config.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/execute/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/execute/components/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/execute/components/execute-input/
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/execute/components/execute-input/execute-input.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/execute/components/execute-input/execute-input.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/execute/components/execute-input/execute-input.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/execute/components/execute-stream/
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/execute/components/execute-stream/execute-stream.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/execute/components/execute-stream/execute-stream.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/execute/components/execute-stream/execute-stream.tmpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/execute/execute.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/execute/execute.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/execute/execute.filter.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/execute/execute.filter.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/execute/execute.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/execute/execute.route.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/execute/execute.route.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/execute/execute.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/execute/execute.service.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/execute/execute.tmpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/execute/execute.tmpl.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/history/
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/history/history.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/history/history.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/history/history.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/history/history.route.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/history/history.route.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/history/history.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/history/history.service.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/history/history.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/log/
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/log/log.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/log/log.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/log/log.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/log/log.route.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/log/log.route.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/log/log.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/log/log.tmpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/log/log.tmpl.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/movies/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/movies/components/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/movies/components/add-movie/
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie-input.directive.js
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie-item.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie-item.tmpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie.controller.js
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/movies/components/movie-entry/
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/movies/components/movie-list/
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/movies/components/movie-list/movie-list.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/movies/components/movie-list/movie-list.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/movies/components/movie-list/movie-list.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/movies/components/new-list/
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/movies/components/new-list/new-list.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/movies/components/new-list/new-list.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/movies/components/new-list/new-list.tmpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/movies/movies.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/movies/movies.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/movies/movies.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/movies/movies.route.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/movies/movies.route.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/movies/movies.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/movies/movies.service.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/movies/movies.tmpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/movies/movies.tmpl.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/pending/
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/pending/pending.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/pending/pending.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/pending/pending.route.js
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/pending/pending.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/pending/pending.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/pending/pending.tmpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/plugins.module.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/schedule/
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/schedule/schedule.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/schedule/schedule.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/schedule/schedule.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/schedule/schedule.route.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/schedule/schedule.route.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/schedule/schedule.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/schedule/schedule.service.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/schedule/schedule.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/seen/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/seen/components/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/seen/components/seen-entry/
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/seen/components/seen-entry/seen-entry.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/seen/components/seen-entry/seen-entry.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/seen/components/seen-entry/seen-entry.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/seen/components/seen-field/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/seen/components/seen-field/seen-field.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/seen/components/seen-field/seen-field.tmpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/seen/seen.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/seen/seen.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/seen/seen.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/seen/seen.route.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/seen/seen.route.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/seen/seen.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/seen/seen.service.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/seen/seen.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/series/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/series/components/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/series/components/episode-release/
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/series/components/episode-release/episode-release.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/series/components/episode-release/episode-release.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/series/components/episode-release/episode-release.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/series/components/episode-release/episode-release.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/series/components/episode-releases/
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/series/components/episode-releases/episode-releases.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/series/components/episode-releases/episode-releases.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/series/components/episode-releases/episode-releases.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/series/components/series-begin-dialog/
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/series/components/series-begin-dialog/series-begin-dialog.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/series/components/series-begin-dialog/series-begin-dialog.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/series/components/series-entry/
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/series/components/series-entry/series-entry.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/series/components/series-entry/series-entry.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/series/components/series-entry/series-entry.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/series/components/series-entry/series-entry.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/series/components/series-episode/
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/series/components/series-episode/series-episode.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/series/components/series-episode/series-episode.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/series/components/series-episode/series-episode.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/series/components/series-episode/series-episode.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/series/components/series-episodes/
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.tmpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/series/series.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/series/series.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/series/series.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/series/series.route.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/series/series.route.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/series/series.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11141 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/series/series.service.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/series/series.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/server/
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/server/loading-dialog.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/server/loading-dialog.tmpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/server/server.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/server/server.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/server/server.service.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/status/
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/status/status.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/status/status.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/status/status.route.js
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/status/status.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/status/status.tmpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/plugins/status/status.tmpl.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/ui/v1/src/scss/
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/scss/_header.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/scss/_loading-bar.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/scss/_variables.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/scss/flexget.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/ui/v1/src/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/src/services/schema.service.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/ui/v1/tests-mock-data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/tests-mock-data/config.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/tests-mock-data/execute.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/tests-mock-data/history.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/tests-mock-data/movie_list.js
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/tests-mock-data/registerPlugin.js
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/tests-mock-data/schedules.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/tests-mock-data/seen.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11128 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/tests-mock-data/series.js
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v1/tests-mock-data/states.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/ui/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/ui/v2/dist/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/ui/v2/dist/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    15872 2023-04-15 15:12:10.000000 FlexGet-3.6.3/flexget/ui/v2/dist/assets/020c97dc8e0463259c2f9df929bb0c69.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     8658 2023-04-15 15:12:10.000000 FlexGet-3.6.3/flexget/ui/v2/dist/assets/14.18cf3ab07df2cff9c980.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12291 2023-04-15 15:12:10.000000 FlexGet-3.6.3/flexget/ui/v2/dist/assets/14.18cf3ab07df2cff9c980.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    17448 2023-04-15 15:12:10.000000 FlexGet-3.6.3/flexget/ui/v2/dist/assets/14286f3ba79c6627433572dfa925202e.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     8363 2023-04-15 15:12:10.000000 FlexGet-3.6.3/flexget/ui/v2/dist/assets/15.df643f032866e7897440.js
+-rw-r--r--   0 runner    (1001) docker     (123)    33576 2023-04-15 15:12:10.000000 FlexGet-3.6.3/flexget/ui/v2/dist/assets/15.df643f032866e7897440.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-04-15 15:12:10.000000 FlexGet-3.6.3/flexget/ui/v2/dist/assets/16.d99413fe0332d02516c9.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10089 2023-04-15 15:12:10.000000 FlexGet-3.6.3/flexget/ui/v2/dist/assets/16.d99413fe0332d02516c9.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    15816 2023-04-15 15:12:10.000000 FlexGet-3.6.3/flexget/ui/v2/dist/assets/2735a3a69b509faf3577afd25bdf552e.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    22020 2023-04-15 15:12:10.000000 FlexGet-3.6.3/flexget/ui/v2/dist/assets/288ad9c6e8b43cf02443a1f499bdf67e.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    22304 2023-04-15 15:12:10.000000 FlexGet-3.6.3/flexget/ui/v2/dist/assets/28f9151055c950874d2c6803a39b425b.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    47404 2023-04-15 15:12:10.000000 FlexGet-3.6.3/flexget/ui/v2/dist/assets/35bb8d560db5205616671eab8c4d0303.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    15736 2023-04-15 15:12:10.000000 FlexGet-3.6.3/flexget/ui/v2/dist/assets/479970ffb74f2117317f9d24d9e317fe.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)  1150672 2023-04-15 15:12:10.000000 FlexGet-3.6.3/flexget/ui/v2/dist/assets/4cb446d4c3b18f2f69df.worker.js
+-rw-r--r--   0 runner    (1001) docker     (123)  4396877 2023-04-15 15:12:10.000000 FlexGet-3.6.3/flexget/ui/v2/dist/assets/4cb446d4c3b18f2f69df.worker.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    22204 2023-04-15 15:12:10.000000 FlexGet-3.6.3/flexget/ui/v2/dist/assets/4df32891a5f2f98a363314f595482e08.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    17324 2023-04-15 15:12:10.000000 FlexGet-3.6.3/flexget/ui/v2/dist/assets/51521a2a8da71e50d871ac6fd2187e87.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    20368 2023-04-15 15:12:10.000000 FlexGet-3.6.3/flexget/ui/v2/dist/assets/5cb7edfceb233100075dc9a1e12e8da3.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20268 2023-04-15 15:12:10.000000 FlexGet-3.6.3/flexget/ui/v2/dist/assets/60fa3c0614b8fb2f394fa29944c21540.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   126767 2023-04-15 15:12:10.000000 FlexGet-3.6.3/flexget/ui/v2/dist/assets/68c852c85ea688dfa942.worker.js
+-rw-r--r--   0 runner    (1001) docker     (123)   560902 2023-04-15 15:12:10.000000 FlexGet-3.6.3/flexget/ui/v2/dist/assets/68c852c85ea688dfa942.worker.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    15808 2023-04-15 15:12:10.000000 FlexGet-3.6.3/flexget/ui/v2/dist/assets/7370c3679472e9560965ff48a4399d0b.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    21588 2023-04-15 15:12:10.000000 FlexGet-3.6.3/flexget/ui/v2/dist/assets/81f57861ed4ac74741f5671e1dff2fd9.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20464 2023-04-15 15:12:10.000000 FlexGet-3.6.3/flexget/ui/v2/dist/assets/87284894879f5b1c229cb49c8ff6decc.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    15712 2023-04-15 15:12:10.000000 FlexGet-3.6.3/flexget/ui/v2/dist/assets/9b3766ef4a402ad3fdeef7501a456512.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    70594 2023-04-15 15:12:10.000000 FlexGet-3.6.3/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.css
+-rw-r--r--   0 runner    (1001) docker     (123)    91826 2023-04-15 15:12:10.000000 FlexGet-3.6.3/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)   562036 2023-04-15 15:12:10.000000 FlexGet-3.6.3/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.js
+-rw-r--r--   0 runner    (1001) docker     (123)  2069487 2023-04-15 15:12:10.000000 FlexGet-3.6.3/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-04-15 15:12:10.000000 FlexGet-3.6.3/flexget/ui/v2/dist/assets/EntryListPlugin.c4b35103ad1660e69c44.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-04-15 15:12:10.000000 FlexGet-3.6.3/flexget/ui/v2/dist/assets/EntryListPlugin.c4b35103ad1660e69c44.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    24029 2023-04-15 15:12:10.000000 FlexGet-3.6.3/flexget/ui/v2/dist/assets/HistoryPlugin.0201ee39aecaa7452270.js
+-rw-r--r--   0 runner    (1001) docker     (123)    41804 2023-04-15 15:12:10.000000 FlexGet-3.6.3/flexget/ui/v2/dist/assets/HistoryPlugin.0201ee39aecaa7452270.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-04-15 15:12:10.000000 FlexGet-3.6.3/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-04-15 15:12:10.000000 FlexGet-3.6.3/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)   148218 2023-04-15 15:12:10.000000 FlexGet-3.6.3/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.js
+-rw-r--r--   0 runner    (1001) docker     (123)   618494 2023-04-15 15:12:10.000000 FlexGet-3.6.3/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-04-15 15:12:10.000000 FlexGet-3.6.3/flexget/ui/v2/dist/assets/MovieListPlugin.17e519c9d031c1cd9477.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-04-15 15:12:10.000000 FlexGet-3.6.3/flexget/ui/v2/dist/assets/MovieListPlugin.17e519c9d031c1cd9477.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     6581 2023-04-15 15:12:10.000000 FlexGet-3.6.3/flexget/ui/v2/dist/assets/PendingListPlugin.7ddbee4abf831e808220.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10858 2023-04-15 15:12:10.000000 FlexGet-3.6.3/flexget/ui/v2/dist/assets/PendingListPlugin.7ddbee4abf831e808220.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    39851 2023-04-15 15:12:10.000000 FlexGet-3.6.3/flexget/ui/v2/dist/assets/SeriesPlugin.f46122b2f63739898cd5.js
+-rw-r--r--   0 runner    (1001) docker     (123)    71452 2023-04-15 15:12:10.000000 FlexGet-3.6.3/flexget/ui/v2/dist/assets/SeriesPlugin.f46122b2f63739898cd5.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-04-15 15:12:10.000000 FlexGet-3.6.3/flexget/ui/v2/dist/assets/TasksHomeCard.0f1a9b4992c80e636a4f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-04-15 15:12:10.000000 FlexGet-3.6.3/flexget/ui/v2/dist/assets/TasksHomeCard.0f1a9b4992c80e636a4f.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    57772 2023-04-15 15:12:10.000000 FlexGet-3.6.3/flexget/ui/v2/dist/assets/TasksPlugin.78a8bc05a72c9f25d7c3.js
+-rw-r--r--   0 runner    (1001) docker     (123)   225286 2023-04-15 15:12:10.000000 FlexGet-3.6.3/flexget/ui/v2/dist/assets/TasksPlugin.78a8bc05a72c9f25d7c3.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    20356 2023-04-15 15:12:10.000000 FlexGet-3.6.3/flexget/ui/v2/dist/assets/adcde98f1d584de52060ad7b16373da3.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20348 2023-04-15 15:12:10.000000 FlexGet-3.6.3/flexget/ui/v2/dist/assets/b00849e00f4c2331cddd8ffb44a6720b.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20392 2023-04-15 15:12:10.000000 FlexGet-3.6.3/flexget/ui/v2/dist/assets/bb1e4dc6333675d11ada2e857e7f95d7.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    17020 2023-04-15 15:12:10.000000 FlexGet-3.6.3/flexget/ui/v2/dist/assets/da0e717829e033a69dec97f1e155ae42.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    17316 2023-04-15 15:12:10.000000 FlexGet-3.6.3/flexget/ui/v2/dist/assets/db4a2a231f52e497c0191e8966b0ee58.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    46199 2023-04-15 15:12:10.000000 FlexGet-3.6.3/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin.5c83b88e8b99cf5955dd.js
+-rw-r--r--   0 runner    (1001) docker     (123)    91316 2023-04-15 15:12:10.000000 FlexGet-3.6.3/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin.5c83b88e8b99cf5955dd.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    50808 2023-04-15 15:12:10.000000 FlexGet-3.6.3/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~SeriesPlugin.82114e5d38c3136caad1.js
+-rw-r--r--   0 runner    (1001) docker     (123)   136381 2023-04-15 15:12:10.000000 FlexGet-3.6.3/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~SeriesPlugin.82114e5d38c3136caad1.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    11083 2023-04-15 15:12:10.000000 FlexGet-3.6.3/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~TasksPlugin.17910c3356c98ded086b.js
+-rw-r--r--   0 runner    (1001) docker     (123)    52623 2023-04-15 15:12:10.000000 FlexGet-3.6.3/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~TasksPlugin.17910c3356c98ded086b.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    17520 2023-04-15 15:12:10.000000 FlexGet-3.6.3/flexget/ui/v2/dist/assets/ebf6d1640ccddb99fb49f73c052c55a8.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    15784 2023-04-15 15:12:10.000000 FlexGet-3.6.3/flexget/ui/v2/dist/assets/ef7c6637c68f269a882e73bcb57a7f6a.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    17008 2023-04-15 15:12:10.000000 FlexGet-3.6.3/flexget/ui/v2/dist/assets/f8b1df51ba843179fa1cc9b53d58127a.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    21704 2023-04-15 15:12:10.000000 FlexGet-3.6.3/flexget/ui/v2/dist/assets/f9e8e590b4e0f1ff83469bb2a55b8488.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    21952 2023-04-15 15:12:10.000000 FlexGet-3.6.3/flexget/ui/v2/dist/assets/fe65b8335ee19dd944289f9ed3178c78.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    88547 2023-04-15 15:12:10.000000 FlexGet-3.6.3/flexget/ui/v2/dist/assets/main.cce4d52f6988bfadab4f.js
+-rw-r--r--   0 runner    (1001) docker     (123)   130389 2023-04-15 15:12:10.000000 FlexGet-3.6.3/flexget/ui/v2/dist/assets/main.cce4d52f6988bfadab4f.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    77360 2023-04-15 15:12:10.000000 FlexGet-3.6.3/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.css
+-rw-r--r--   0 runner    (1001) docker     (123)    95799 2023-04-15 15:12:10.000000 FlexGet-3.6.3/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)  2285898 2023-04-15 15:12:10.000000 FlexGet-3.6.3/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.js
+-rw-r--r--   0 runner    (1001) docker     (123)  9410938 2023-04-15 15:12:10.000000 FlexGet-3.6.3/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-04-15 15:12:10.000000 FlexGet-3.6.3/flexget/ui/v2/dist/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/ui/v2/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12440 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/utils/bittorrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9149 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/utils/cached_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6458 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/utils/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/utils/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4616 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/utils/lazy_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/utils/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:12:14.000000 FlexGet-3.6.3/flexget/utils/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/utils/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/utils/parsers/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/utils/parsers/movie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/utils/parsers/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28532 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/utils/parsers/series.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/utils/pathscrub.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19296 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/utils/qualities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11247 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/utils/requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8048 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/utils/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8197 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/utils/simple_persistence.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/utils/soup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/utils/sqlalchemy_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11421 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/utils/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16980 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/utils/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7818 2023-04-15 15:11:46.000000 FlexGet-3.6.3/flexget/webserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-04-15 15:11:46.000000 FlexGet-3.6.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     6548 2023-04-15 15:11:46.000000 FlexGet-3.6.3/requirements-docker.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-04-15 15:11:46.000000 FlexGet-3.6.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 15:12:14.000000 FlexGet-3.6.3/setup.cfg
```

### Comparing `FlexGet-3.6.2/FlexGet.egg-info/PKG-INFO` & `FlexGet-3.6.3/FlexGet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlexGet
-Version: 3.6.2
+Version: 3.6.3
 Summary: FlexGet is a program aimed to automate downloading or processing content (torrents, podcasts, etc.) from different sources like RSS-feeds, html-pages, various sites and more.
 Author-email: Marko Koivusalo <marko.koivusalo@gmail.com>, Chase Sterling <chase.sterling@gmail.com>
 License: 
         The MIT License
         
         Copyright (C) 2006, Riku 'Shrike' Lindblad
         Copyright (C) 2007, Marko Koivusalo
```

### Comparing `FlexGet-3.6.2/FlexGet.egg-info/SOURCES.txt` & `FlexGet-3.6.3/FlexGet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/FlexGet.egg-info/requires.txt` & `FlexGet-3.6.3/FlexGet.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/LICENSE` & `FlexGet-3.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/PKG-INFO` & `FlexGet-3.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlexGet
-Version: 3.6.2
+Version: 3.6.3
 Summary: FlexGet is a program aimed to automate downloading or processing content (torrents, podcasts, etc.) from different sources like RSS-feeds, html-pages, various sites and more.
 Author-email: Marko Koivusalo <marko.koivusalo@gmail.com>, Chase Sterling <chase.sterling@gmail.com>
 License: 
         The MIT License
         
         Copyright (C) 2006, Riku 'Shrike' Lindblad
         Copyright (C) 2007, Marko Koivusalo
```

### Comparing `FlexGet-3.6.2/README.rst` & `FlexGet-3.6.3/README.rst`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/dev-requirements-extras.txt` & `FlexGet-3.6.3/dev-requirements-extras.txt`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/dev-requirements.txt` & `FlexGet-3.6.3/dev-requirements.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 alabaster==0.7.12 ; python_version >= "3.7" and python_version < "4.0"
-astroid==2.11.7 ; python_version >= "3.7" and python_version < "4.0"
 attrs==22.1.0 ; python_version >= "3.7" and python_version < "4.0"
 babel==2.11.0 ; python_version >= "3.7" and python_version < "4.0"
 black==22.12.0 ; python_version >= "3.7" and python_version < "4.0"
 bleach==5.0.1 ; python_version >= "3.7" and python_version < "4.0"
 build==0.9.0 ; python_version >= "3.7" and python_version < "4.0"
 certifi==2022.12.7 ; python_version >= "3.7" and python_version < "4"
 cffi==1.15.1 ; python_version >= "3.7" and python_version < "4.0" and sys_platform == "linux"
@@ -12,62 +11,58 @@
 click==8.1.3 ; python_version >= "3.7" and python_version < "4.0"
 codacy-coverage==1.3.11 ; python_version >= "3.7" and python_version < "4.0"
 colorama==0.4.6 ; python_version >= "3.7" and python_version < "4.0" and os_name == "nt" or python_version >= "3.7" and python_version < "4.0" and platform_system == "Windows" or python_version >= "3.7" and python_version < "4.0" and sys_platform == "win32"
 commonmark==0.9.1 ; python_version >= "3.7" and python_version < "4.0"
 coverage==6.5.0 ; python_version >= "3.7" and python_version < "4.0"
 coverage[toml]==6.5.0 ; python_version >= "3.7" and python_version < "4.0"
 cryptography==38.0.4 ; python_version >= "3.7" and python_version < "4.0" and sys_platform == "linux"
-dill==0.3.6 ; python_version >= "3.7" and python_version < "4.0"
 distlib==0.3.6 ; python_version >= "3.7" and python_version < "4.0"
 docutils==0.19 ; python_version >= "3.7" and python_version < "4.0"
 exceptiongroup==1.0.4 ; python_version >= "3.7" and python_version < "3.11"
 execnet==1.9.0 ; python_version >= "3.7" and python_version < "4.0"
 filelock==3.8.2 ; python_version >= "3.7" and python_version < "4.0"
 gitdb==4.0.10 ; python_version >= "3.7" and python_version < "4.0"
 gitpython==3.1.29 ; python_version >= "3.7" and python_version < "4.0"
 identify==2.5.9 ; python_version >= "3.7" and python_version < "4.0"
 idna==3.4 ; python_version >= "3.7" and python_version < "4"
 imagesize==1.4.1 ; python_version >= "3.7" and python_version < "4.0"
 importlib-metadata==6.1.0 ; python_version >= "3.7" and python_version < "4.0"
 iniconfig==1.1.1 ; python_version >= "3.7" and python_version < "4.0"
-isort==5.10.1 ; python_version >= "3.7" and python_version < "4.0"
 jaraco-classes==3.2.3 ; python_version >= "3.7" and python_version < "4.0"
 jeepney==0.8.0 ; python_version >= "3.7" and python_version < "4.0" and sys_platform == "linux"
 jinja2==3.1.2 ; python_version >= "3.7" and python_version < "4.0"
 keyring==23.11.0 ; python_version >= "3.7" and python_version < "4.0"
-lazy-object-proxy==1.8.0 ; python_version >= "3.7" and python_version < "4.0"
 markupsafe==2.1.1 ; python_version >= "3.7" and python_version < "4.0"
-mccabe==0.7.0 ; python_version >= "3.7" and python_version < "4.0"
 more-itertools==9.0.0 ; python_version >= "3.7" and python_version < "4.0"
 multidict==6.0.3 ; python_version >= "3.7" and python_version < "4.0"
 mypy-extensions==0.4.3 ; python_version >= "3.7" and python_version < "4.0"
 mypy==0.991 ; python_version >= "3.7" and python_version < "4.0"
 nodeenv==1.7.0 ; python_version >= "3.7" and python_version < "4.0"
 packaging==22.0 ; python_version >= "3.7" and python_version < "4.0"
 pathspec==0.10.3 ; python_version >= "3.7" and python_version < "4.0"
 pep517==0.13.0 ; python_version >= "3.7" and python_version < "4.0"
 pkginfo==1.9.2 ; python_version >= "3.7" and python_version < "4.0"
 platformdirs==2.6.0 ; python_version >= "3.7" and python_version < "4.0"
 pluggy==1.0.0 ; python_version >= "3.7" and python_version < "4.0"
 pre-commit==2.20.0 ; python_version >= "3.7" and python_version < "4.0"
 pycparser==2.21 ; python_version >= "3.7" and python_version < "4.0" and sys_platform == "linux"
 pygments==2.13.0 ; python_version >= "3.7" and python_version < "4.0"
-pylint==2.13.9 ; python_version >= "3.7" and python_version < "4.0"
 pytest-cov==4.0.0 ; python_version >= "3.7" and python_version < "4.0"
 pytest-runner==6.0.0 ; python_version >= "3.7" and python_version < "4.0"
 pytest-xdist==3.1.0 ; python_version >= "3.7" and python_version < "4.0"
 pytest==7.2.0 ; python_version >= "3.7" and python_version < "4.0"
 pytz==2022.6 ; python_version >= "3.7" and python_version < "4.0"
 pywin32-ctypes==0.2.0 ; python_version >= "3.7" and python_version < "4.0" and sys_platform == "win32"
 pyyaml==6.0 ; python_version >= "3.7" and python_version < "4.0"
 readme-renderer==37.3 ; python_version >= "3.7" and python_version < "4.0"
 requests-toolbelt==0.10.1 ; python_version >= "3.7" and python_version < "4.0"
 requests==2.28.1 ; python_version >= "3.7" and python_version < "4"
 rfc3986==2.0.0 ; python_version >= "3.7" and python_version < "4.0"
 rich==12.6.0 ; python_version >= "3.7" and python_version < "4.0"
+ruff==0.0.261 ; python_version >= "3.7" and python_version < "4.0"
 secretstorage==3.3.3 ; python_version >= "3.7" and python_version < "4.0" and sys_platform == "linux"
 setuptools==65.6.3 ; python_version >= "3.7" and python_version < "4.0"
 six==1.16.0 ; python_version >= "3.7" and python_version < "4.0"
 smmap==5.0.0 ; python_version >= "3.7" and python_version < "4.0"
 snowballstemmer==2.2.0 ; python_version >= "3.7" and python_version < "4.0"
 sphinx==5.3.0 ; python_version >= "3.7" and python_version < "4.0"
 sphinxcontrib-applehelp==1.0.2 ; python_version >= "3.7" and python_version < "4.0"
```

### Comparing `FlexGet-3.6.2/flexget/__init__.py` & `FlexGet-3.6.3/flexget/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import sys
 from typing import Sequence
 
 # __version__ import need to be first in order to avoid circular import within logger
 from ._version import __version__  # noqa
 
 # isort: split
-from flexget import log  # noqa
-from flexget.manager import Manager  # noqa
+from flexget import log
+from flexget.manager import Manager
 
 
 def main(args: Sequence[str] = None):
     """Main entry point for Command Line Interface"""
 
     if args is None:
         args = sys.argv[1:]
```

### Comparing `FlexGet-3.6.2/flexget/api/app.py` & `FlexGet-3.6.3/flexget/api/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
     def __getattr__(self, item: str) -> 'APIEndpoint':
         return APIEndpoint('/api/' + item, self.get_endpoint)
 
     def get_endpoint(self, url: str, data=None, method: str = None):
         if method is None:
             method = 'POST' if data is not None else 'GET'
-        auth_header = dict(Authorization='Token %s' % api_key())
+        auth_header = {'Authorization': 'Token %s' % api_key()}
         response = self.app.open(
             url, data=data, follow_redirects=True, method=method, headers=auth_header
         )
         result = json.loads(response.get_data(as_text=True))
         # TODO: Proper exceptions
         if 200 > response.status_code >= 300:
             raise Exception(result['error'])
```

### Comparing `FlexGet-3.6.2/flexget/api/core/authentication.py` & `FlexGet-3.6.3/flexget/api/core/authentication.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/api/core/cached.py` & `FlexGet-3.6.3/flexget/api/core/cached.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/api/core/database.py` & `FlexGet-3.6.3/flexget/api/core/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,8 +57,8 @@
 
 
 @db_api.route('/plugins/')
 class DBCleanup(APIResource):
     @api.response(200, model=plugins_schema)
     def get(self, session: Session = None) -> Response:
         """List resettable DB plugins"""
-        return jsonify(sorted(list(plugin_schemas)))
+        return jsonify(sorted(plugin_schemas))
```

### Comparing `FlexGet-3.6.2/flexget/api/core/format_checker.py` & `FlexGet-3.6.3/flexget/api/core/format_checker.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/api/core/plugins.py` & `FlexGet-3.6.3/flexget/api/core/plugins.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,15 +84,15 @@
         'name': plugin.name,
         'api_ver': plugin.api_ver,
         'builtin': plugin.builtin,
         'category': plugin.category,
         'debug': plugin.debug,
         'interfaces': plugin.interfaces,
         'phase_handlers': [
-            dict(phase=handler, priority=event.priority)
+            {'phase': handler, 'priority': event.priority}
             for handler, event in plugin.phase_handlers.items()
         ],
     }
 
 
 @plugins_api.route('/')
 class PluginsAPI(APIResource):
```

### Comparing `FlexGet-3.6.2/flexget/api/core/schema.py` & `FlexGet-3.6.3/flexget/api/core/schema.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/api/core/server.py` & `FlexGet-3.6.3/flexget/api/core/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,23 +34,24 @@
     rest_of_line,
 )
 from sqlalchemy.orm import Session
 from yaml.error import MarkedYAMLError, YAMLError
 
 from flexget._version import __version__
 from flexget.api import APIResource, api
-from flexget.api.app import APIError, BadRequest
-from flexget.api.app import __version__ as __api_version__
 from flexget.api.app import (
+    APIError,
+    BadRequest,
     base_message,
     base_message_schema,
     empty_response,
     etag,
     success_response,
 )
+from flexget.api.app import __version__ as __api_version__
 from flexget.config_schema import ConfigError
 from flexget.utils.tools import get_latest_flexget_version_number
 
 logger = logger.bind(name='api.server')
 
 server_api = api.namespace('server', description='Manage Daemon')
 
@@ -390,16 +391,16 @@
                     # Read in reverse for efficiency
                     for line in reverse_readline(fh, start_byte=end_byte):
                         if len(lines_found) >= lines:
                             break
                         if log_parser.matches(line):
                             lines_found.append(log_parser.json_string(line))
 
-                    for l in reversed(lines_found):
-                        yield l + ',\n'
+                    for line in reversed(lines_found):
+                        yield line + ',\n'
 
             # We need to track the inode in case the log file is rotated
             current_inode = file_inode(base_log_file)
 
             while True:
                 # If the server is shutting down then end the stream nicely
                 if cherrypy.engine.state != cherrypy.engine.states.STARTED:
```

### Comparing `FlexGet-3.6.2/flexget/api/core/tasks.py` & `FlexGet-3.6.3/flexget/api/core/tasks.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/api/core/user.py` & `FlexGet-3.6.3/flexget/api/core/user.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/api/templates/api_response.html` & `FlexGet-3.6.3/flexget/api/templates/api_response.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/api/templates/swagger-ui.html` & `FlexGet-3.6.3/flexget/api/templates/swagger-ui.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/archive/archive.py` & `FlexGet-3.6.3/flexget/components/archive/archive.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/archive/cli.py` & `FlexGet-3.6.3/flexget/components/archive/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -253,15 +253,15 @@
     )
     inject_parser.add_argument(
         'ids', nargs='+', type=int, metavar='ID', help='Archive ID of an item to inject'
     )
     inject_parser.add_argument(
         '--immortal',
         action='store_true',
-        help='Injected entries will not be able to be ' 'rejected by any plugins',
+        help='Injected entries will not be able to be rejected by any plugins',
     )
     exec_group = inject_parser.add_argument_group('execute arguments')
     exec_group.add_argument(
         'execute_options', action=ParseExtrasAction, parser=get_parser('execute')
     )
     tag_parser = archive_parser.add_subparser(
         'tag-source', help='Tag all archived entries within a given source'
```

### Comparing `FlexGet-3.6.2/flexget/components/archive/db.py` & `FlexGet-3.6.3/flexget/components/archive/db.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/archives/archives.py` & `FlexGet-3.6.3/flexget/components/archives/archives.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/archives/decompress.py` & `FlexGet-3.6.3/flexget/components/archives/decompress.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
         logger.info('Would extract: {} to {}', info.filename, destination)
         return
     logger.debug('Attempting to extract: {} to {}', info.filename, destination)
     try:
         info.extract(archive, destination)
     except archiveutil.FSError as error:
         logger.error('OS error while creating file: {} ({})', destination, error)
-    except archiveutil.FileAlreadyExists as error:
+    except archiveutil.FileAlreadyExists:
         logger.warning('File already exists: {}', destination)
     except archiveutil.ArchiveError as error:
         logger.error('Failed to extract file: {} from {} ({})', info.filename, archive.path, error)
 
 
 def get_destination_path(info, to, keep_dirs):
     """Generate the destination path for a given file"""
```

### Comparing `FlexGet-3.6.2/flexget/components/archives/utils.py` & `FlexGet-3.6.3/flexget/components/archives/utils.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/backlog/backlog.py` & `FlexGet-3.6.3/flexget/components/backlog/backlog.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/backlog/cli.py` & `FlexGet-3.6.3/flexget/components/backlog/cli.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/backlog/db.py` & `FlexGet-3.6.3/flexget/components/backlog/db.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/bittorrent/convert_magnet.py` & `FlexGet-3.6.3/flexget/components/bittorrent/convert_magnet.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/bittorrent/magnet_info_hash.py` & `FlexGet-3.6.3/flexget/components/bittorrent/magnet_info_hash.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
     def on_task_metainfo(self, task, config):
         if config is False:
             return
         for entry in task.all_entries:
             if entry.get('torrent_info_hash'):
                 continue
-            for url in [entry['url']] + entry.get('urls', []):
+            for url in [entry['url'], *entry.get('urls', [])]:
                 if url.startswith('magnet:'):
                     # find base16 encoded
                     info_hash_search = re.search('btih:([0-9a-f]{40})', url, re.IGNORECASE)
                     if info_hash_search:
                         entry['torrent_info_hash'] = info_hash_search.group(1).upper()
                         break
                     # find base32 encoded
```

### Comparing `FlexGet-3.6.2/flexget/components/bittorrent/private_torrents.py` & `FlexGet-3.6.3/flexget/components/bittorrent/private_torrents.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/bittorrent/torrent.py` & `FlexGet-3.6.3/flexget/components/bittorrent/torrent.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/bittorrent/torrent_alive.py` & `FlexGet-3.6.3/flexget/components/bittorrent/torrent_alive.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/bittorrent/torrent_files.py` & `FlexGet-3.6.3/flexget/components/bittorrent/torrent_files.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/bittorrent/torrent_match.py` & `FlexGet-3.6.3/flexget/components/bittorrent/torrent_match.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/bittorrent/torrent_scrub.py` & `FlexGet-3.6.3/flexget/components/bittorrent/torrent_scrub.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/bittorrent/torrent_size.py` & `FlexGet-3.6.3/flexget/components/bittorrent/torrent_size.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/bittorrent/trackers.py` & `FlexGet-3.6.3/flexget/components/bittorrent/trackers.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/emby/api_emby.py` & `FlexGet-3.6.3/flexget/components/emby/api_emby.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,15 @@
                 if isinstance(source[key], str):
                     source[key] = [source[key]]
 
                 if source[key][0] and source[key][0].find(EmbyApiBase.EMBY_PREF) < 0:
                     source[key].insert(0, f'{EmbyApiBase.EMBY_PREF}{source[key][0]}')
 
                 for value_source in source[key]:
-                    if not value_source in destination[key]:
+                    if value_source not in destination[key]:
                         destination[key].append(value_source)
 
         return destination
 
     @staticmethod
     def update_using_map(target, field_map: dict, source_item, **kwargs):
         """
@@ -213,17 +213,17 @@
                     args = {'nameOrEmail': self._username, 'rawpw': self._password}
                     connect_data = EmbyApi.resquest_emby(
                         EMBY_ENDPOINT_CONNECT_LOGIN, self, 'POST', emby_connect=True, **args
                     )
 
                     if (
                         not connect_data
-                        or not 'AccessToken' in connect_data
-                        or not 'User' in connect_data
-                        or not 'Id' in connect_data['User']
+                        or 'AccessToken' not in connect_data
+                        or 'User' not in connect_data
+                        or 'Id' not in connect_data['User']
                     ):
                         raise PluginError(
                             f'Could not login to Emby Connect account `{self._connect_username}`'
                         )
 
                     self._connect_token = connect_data['AccessToken']
 
@@ -234,42 +234,42 @@
                     )
                     if not isinstance(connect_servers, list):
                         raise PluginError(
                             f'Could not login to Emby Connect account `{self._connect_username}`, no server list'
                         )
 
                     for server in connect_servers:
-                        if not 'Name' in server:
+                        if 'Name' not in server:
                             raise PluginError(
                                 f'Could not login to Emby Connect account `{self._connect_username}`, no server list'
                             )
                         if server['Name'].lower() == self.host.lower():
                             connect_server = server
                             break
                     else:
                         raise PluginError(
                             f'No server with name `{self.host}`` on `{self._connect_username}` account'
                         )
 
-                    if not 'AccessKey' in connect_server or not 'Url' in connect_server:
+                    if 'AccessKey' not in connect_server or 'Url' not in connect_server:
                         raise PluginError(
                             f'Could not login to Emby Connect account `{self._connect_username}`, no server list'
                         )
 
                     self._connect_token_link = connect_server['AccessKey']
                     self.host = connect_server['Url']
 
                     args = {'format': 'json', 'ConnectUserId': connect_data['User']['Id']}
                     connect_exchange = EmbyApi.resquest_emby(
                         EMBY_ENDPOINT_CONNECT_EXCHANGE, self, 'GET', **args
                     )
 
                     if (
-                        not 'LocalUserId' in connect_exchange
-                        or not 'AccessToken' in connect_exchange
+                        'LocalUserId' not in connect_exchange
+                        or 'AccessToken' not in connect_exchange
                     ):
                         raise PluginError(
                             f'Could not login with Emby Connect to server `{self.host}`'
                         )
 
                     self._userid = connect_exchange['LocalUserId']
                     self._token = connect_exchange['AccessToken']
@@ -1552,15 +1552,15 @@
     @classmethod
     def get_from_child(cls, child: "EmbyApiMedia") -> "EmbyApiMedia":
         parents = cls._get_parents(child)
         if not parents:
             return None
 
         for parent in parents:
-            if not 'Type' in parent or parent['Type'].lower() != cls.TYPE:
+            if 'Type' not in parent or parent['Type'].lower() != cls.TYPE:
                 continue
             season = cls.cast(**parent)
             if isinstance(season, cls):
                 return season
 
     @staticmethod
     def cast(**kwargs) -> 'EmbyApiMedia':
```

### Comparing `FlexGet-3.6.2/flexget/components/emby/emby_list.py` & `FlexGet-3.6.3/flexget/components/emby/emby_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/emby/emby_lookup.py` & `FlexGet-3.6.3/flexget/components/emby/emby_lookup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from loguru import logger
 
-from flexget import entry, plugin
+from flexget import plugin
 from flexget.components.emby.api_emby import EmbyApi, EmbyAuth
 from flexget.components.emby.emby_util import SCHEMA_SERVER, get_field_map
+from flexget.entry import register_lazy_lookup
 from flexget.event import event
 
 logger = logger.bind(name='emby_lookup')
 
 
 class EmbyLookup:
     """
@@ -31,15 +32,15 @@
         self.auth = EmbyAuth(**config)
 
         try:
             self.auth.login(False)
         except plugin.PluginError as e:
             logger.error('Not possible to login to emby: {}', e)
 
-    @entry.register_lazy_lookup('emby_lookup')
+    @register_lazy_lookup('emby_lookup')
     def lazy_loader(self, entry, auth):
         if not auth:
             return
 
         if not auth.logged:
             auth.login()
```

### Comparing `FlexGet-3.6.2/flexget/components/emby/emby_refresh.py` & `FlexGet-3.6.3/flexget/components/emby/emby_refresh.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/emby/emby_util.py` & `FlexGet-3.6.3/flexget/components/emby/emby_util.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/emby/from_emby.py` & `FlexGet-3.6.3/flexget/components/emby/from_emby.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/estimate_release/estimate_release.py` & `FlexGet-3.6.3/flexget/components/estimate_release/estimate_release.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/estimate_release/estimators/est_movies_bluray.py` & `FlexGet-3.6.3/flexget/components/estimate_release/estimators/est_movies_bluray.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/estimate_release/estimators/est_released_movies.py` & `FlexGet-3.6.3/flexget/components/estimate_release/estimators/est_released_movies.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/estimate_release/estimators/est_series_tvmaze.py` & `FlexGet-3.6.3/flexget/components/estimate_release/estimators/est_series_tvmaze.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 
         if entity_data['data_exists'] == False:
             # Make Lookup to series to see if failed because of no episode or no data
             lookup = api_tvmaze.series_lookup
             series = {}
             try:
                 series = lookup(**kwargs)
-            except LookupError as e:
+            except LookupError:
                 entity_data['data_exists'] = False
 
             if not series:
                 logger.debug('No data in tvmaze for series: {}', series_name)
                 entity_data['data_exists'] = False
             else:
                 logger.debug(
```

### Comparing `FlexGet-3.6.2/flexget/components/failed/api.py` & `FlexGet-3.6.3/flexget/components/failed/api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/failed/cli.py` & `FlexGet-3.6.3/flexget/components/failed/cli.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/failed/db.py` & `FlexGet-3.6.3/flexget/components/failed/db.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/failed/retry_failed.py` & `FlexGet-3.6.3/flexget/components/failed/retry_failed.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/ftp/ftp_download.py` & `FlexGet-3.6.3/flexget/components/ftp/ftp_download.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/ftp/ftp_list.py` & `FlexGet-3.6.3/flexget/components/ftp/ftp_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/ftp/sftp.py` & `FlexGet-3.6.3/flexget/components/ftp/sftp.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/ftp/sftp_client.py` & `FlexGet-3.6.3/flexget/components/ftp/sftp_client.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/history/api.py` & `FlexGet-3.6.3/flexget/components/history/api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/history/cli.py` & `FlexGet-3.6.3/flexget/components/history/cli.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/history/db.py` & `FlexGet-3.6.3/flexget/components/history/db.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/history/history.py` & `FlexGet-3.6.3/flexget/components/history/history.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/imdb/api.py` & `FlexGet-3.6.3/flexget/components/imdb/api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/imdb/db.py` & `FlexGet-3.6.3/flexget/components/imdb/db.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/imdb/from_imdb.py` & `FlexGet-3.6.3/flexget/components/imdb/from_imdb.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/imdb/imdb.py` & `FlexGet-3.6.3/flexget/components/imdb/imdb.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/imdb/imdb_lookup.py` & `FlexGet-3.6.3/flexget/components/imdb/imdb_lookup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from datetime import datetime
 
 from loguru import logger
 
-from flexget import entry, plugin
+from flexget import plugin
 from flexget.components.imdb.utils import ImdbParser, ImdbSearch, extract_id, make_url
-from flexget.entry import Entry
+from flexget.entry import Entry, register_lazy_lookup
 from flexget.event import event
 from flexget.utils.database import with_session
 from flexget.utils.log import log_once
 
 from . import db
 
 logger = logger.bind(name='imdb_lookup')
@@ -56,15 +56,15 @@
     @plugin.priority(130)
     def on_task_metainfo(self, task, config):
         if not config:
             return
         for entry in task.entries:
             entry.add_lazy_fields(self.lazy_loader, self.field_map)
 
-    @entry.register_lazy_lookup('imdb_lookup')
+    @register_lazy_lookup('imdb_lookup')
     def lazy_loader(self, entry):
         """Does the lookup for this entry and populates the entry fields."""
         try:
             self.lookup(entry)
         except plugin.PluginError as e:
             log_once(str(e.value).capitalize(), logger=logger)
```

### Comparing `FlexGet-3.6.2/flexget/components/imdb/imdb_url.py` & `FlexGet-3.6.3/flexget/components/imdb/imdb_url.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/imdb/imdb_watchlist.py` & `FlexGet-3.6.3/flexget/components/imdb/imdb_watchlist.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,17 +117,17 @@
         page = self.fetch_page(task, url, params, headers)
         try:
             json_vars = json.loads(
                 re.search(r'IMDbReactInitialState.push\((.+?)\);\n', page.text).group(1)
             )
         except (TypeError, AttributeError, ValueError) as e:
             raise plugin.PluginError(
-                'Unable to get imdb list from imdb react widget.'
-                + ' Either the list is empty or the imdb parser of the imdb_watchlist plugin is broken.'
-                + ' Original error: %s.' % str(e)
+                'Unable to get imdb list from imdb react widget. '
+                'Either the list is empty or the imdb parser of the imdb_watchlist plugin is broken. '
+                'Original error: %s.' % str(e)
             )
         total_item_count = 0
         if 'list' in json_vars and 'items' in json_vars['list']:
             total_item_count = len(json_vars['list']['items'])
         if not total_item_count:
             logger.verbose('No movies were found in imdb list: {}', config['list'])
             return []
@@ -137,17 +137,17 @@
                 imdb_ids.append(item['const'])
         params = {'ids': ','.join(imdb_ids)}
         url = 'http://www.imdb.com/title/data'
         try:
             json_data = self.fetch_page(task, url, params, headers).json()
         except (ValueError, TypeError) as e:
             raise plugin.PluginError(
-                'Unable to get imdb list from imdb JSON API.'
-                + ' Either the list is empty or the imdb parser of the imdb_watchlist plugin is broken.'
-                + ' Original error: %s.' % str(e)
+                'Unable to get imdb list from imdb JSON API. '
+                'Either the list is empty or the imdb parser of the imdb_watchlist plugin is broken. '
+                'Original error: %s.' % str(e)
             )
         logger.verbose('imdb list contains {} items', len(json_data))
         logger.debug(
             'First entry (imdb id: {}) looks like this: {}', imdb_ids[0], json_data[imdb_ids[0]]
         )
         entries = []
         for imdb_id in imdb_ids:
```

### Comparing `FlexGet-3.6.2/flexget/components/imdb/utils.py` & `FlexGet-3.6.3/flexget/components/imdb/utils.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/irc/api.py` & `FlexGet-3.6.3/flexget/components/irc/api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/irc/cli.py` & `FlexGet-3.6.3/flexget/components/irc/cli.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/irc/irc.py` & `FlexGet-3.6.3/flexget/components/irc/irc.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from flexget.manager import manager
 from flexget.utils import requests
 from flexget.utils.tools import get_config_hash
 
 try:
     from irc_bot import utils as irc_bot
     from irc_bot.simple_irc_bot import SimpleIRCBot, partial
-except ImportError as e:
+except ImportError:
     irc_bot = None
     SimpleIRCBot = object
 
 logger = logger.bind(name='irc')
 
 MESSAGE_CLEAN = re.compile(
     r"\x0f|\x1f|\x02|\x03(?:[\d]{1,2}(?:,[\d]{1,2})?)?", re.MULTILINE | re.UNICODE
@@ -783,23 +783,23 @@
             entry = Entry()
             raw_message = ''
             matched_lines = []
             for idx, (rx, vals, optional) in enumerate(self.multilinepatterns):
                 logger.debug('Using pattern {} to parse message vars', rx.pattern)
                 # find the next candidate line
                 line = ''
-                for l in list(lines):
+                for candidate in list(lines):
                     # skip ignored lines
                     for ignore_rx, expected in self.ignore_lines:
-                        if ignore_rx.match(l) and expected:
+                        if ignore_rx.match(candidate) and expected:
                             logger.debug('Ignoring message: matched ignore line')
-                            lines.remove(l)
+                            lines.remove(candidate)
                             break
                     else:
-                        line = l
+                        line = candidate
                         break
 
                 raw_message += '\n' + line
                 match = self.match_message_patterns([(rx, vals, optional)], line)
                 if match:
                     entry.update(match)
                     matched_lines.append(line)
```

### Comparing `FlexGet-3.6.2/flexget/components/managed_lists/list_add.py` & `FlexGet-3.6.3/flexget/components/managed_lists/list_add.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/managed_lists/list_clear.py` & `FlexGet-3.6.3/flexget/components/managed_lists/list_clear.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/managed_lists/list_match.py` & `FlexGet-3.6.3/flexget/components/managed_lists/list_match.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/managed_lists/list_remove.py` & `FlexGet-3.6.3/flexget/components/managed_lists/list_remove.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/managed_lists/lists/couchpotato_list.py` & `FlexGet-3.6.3/flexget/components/managed_lists/lists/couchpotato_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/managed_lists/lists/entry_list/api.py` & `FlexGet-3.6.3/flexget/components/managed_lists/lists/entry_list/api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/managed_lists/lists/entry_list/cli.py` & `FlexGet-3.6.3/flexget/components/managed_lists/lists/entry_list/cli.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/managed_lists/lists/entry_list/db.py` & `FlexGet-3.6.3/flexget/components/managed_lists/lists/entry_list/db.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/managed_lists/lists/entry_list/entry_list.py` & `FlexGet-3.6.3/flexget/components/managed_lists/lists/entry_list/entry_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/managed_lists/lists/imdb_list.py` & `FlexGet-3.6.3/flexget/components/managed_lists/lists/imdb_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,15 +109,15 @@
             raise PluginError('Please inform the login cookies')
 
         if isinstance(cookies, dict):
             new_cookie = cookies
         elif isinstance(cookies, str):
             try:
                 new_cookie = json_loads(cookies)
-            except JSONDecodeError as e:
+            except JSONDecodeError:
                 new_cookie = self.parse_cookies_file(cookies)
 
         if not new_cookie:
             raise PluginError(
                 'Invalid cookies format, please add a dict, a string in json or a path to a file in json'
             )
 
@@ -131,15 +131,15 @@
         file = Path(path)
         if not file.exists():
             raise PluginError('Invalid cookies file format, file does not exist')
 
         with file.open(encoding='utf-8') as data:
             try:
                 contents = json_load(data)
-            except JSONDecodeError as e:
+            except JSONDecodeError:
                 raise PluginError('Invalid cookies file format, file not in json')
 
         return contents
 
     @property
     def session(self):
         if not self._authenticated:
```

### Comparing `FlexGet-3.6.2/flexget/components/managed_lists/lists/movie_list/api.py` & `FlexGet-3.6.3/flexget/components/managed_lists/lists/movie_list/api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/managed_lists/lists/movie_list/cli.py` & `FlexGet-3.6.3/flexget/components/managed_lists/lists/movie_list/cli.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/managed_lists/lists/movie_list/db.py` & `FlexGet-3.6.3/flexget/components/managed_lists/lists/movie_list/db.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,20 +5,14 @@
 from sqlalchemy.orm import relationship
 from sqlalchemy.sql.elements import and_
 
 from flexget import plugin
 from flexget.db_schema import versioned_base, with_session
 from flexget.entry import Entry
 
-try:
-    # NOTE: Importing other plugins is discouraged!
-    from flexget.components.parsing.parsers import parser_common as plugin_parser_common
-except ImportError:
-    raise plugin.DependencyError(issued_by=__name__, missing='parser_common')
-
 logger = logger.bind(name='movie_list')
 Base = versioned_base('movie_list', 0)
 
 
 class MovieListBase:
     """
     Class that contains helper methods for movie list as well as plugins that use it,
```

### Comparing `FlexGet-3.6.2/flexget/components/managed_lists/lists/movie_list/movie_list.py` & `FlexGet-3.6.3/flexget/components/managed_lists/lists/movie_list/movie_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/managed_lists/lists/pending_list/api.py` & `FlexGet-3.6.3/flexget/components/managed_lists/lists/pending_list/api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/managed_lists/lists/pending_list/cli.py` & `FlexGet-3.6.3/flexget/components/managed_lists/lists/pending_list/cli.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/managed_lists/lists/pending_list/db.py` & `FlexGet-3.6.3/flexget/components/managed_lists/lists/pending_list/db.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/managed_lists/lists/pending_list/pending_list.py` & `FlexGet-3.6.3/flexget/components/managed_lists/lists/pending_list/pending_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/managed_lists/lists/plex_watchlist.py` & `FlexGet-3.6.3/flexget/components/managed_lists/lists/plex_watchlist.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 if typing.TYPE_CHECKING:
     from plexapi.myplex import MyPlexAccount
     from plexapi.video import Movie, Show
 
 
 def import_plexaccount() -> "Type[MyPlexAccount]":
     try:
-        from plexapi.myplex import MyPlexAccount  # noqa
+        from plexapi.myplex import MyPlexAccount
 
         return MyPlexAccount
     except ImportError:
         raise plugin.DependencyError('plex_watchlist', 'plexapi', 'plexapi package required')
 
 
 def to_entry(plex_item: "Union[Movie, Show]") -> Entry:
```

### Comparing `FlexGet-3.6.2/flexget/components/managed_lists/lists/radarr_list.py` & `FlexGet-3.6.3/flexget/components/managed_lists/lists/radarr_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -271,15 +271,15 @@
     """
     Translates the provided Radarr quality string to a Flexget Requirement instance.
     Returns None if translation is unsuccessful
     """
 
     # QUALITIES_MAP has its keys in lower case
     radarr_quality = radarr_quality.lower()
-    if not radarr_quality in QUALITIES_MAP:
+    if radarr_quality not in QUALITIES_MAP:
         logger.warning(
             "Did not find a suitible translation for Radarr quality '{}'", radarr_quality
         )
         return None
 
     flexget_quality_req_string = QUALITIES_MAP[radarr_quality]
```

### Comparing `FlexGet-3.6.2/flexget/components/managed_lists/lists/regexp_list/cli.py` & `FlexGet-3.6.3/flexget/components/managed_lists/lists/regexp_list/cli.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/managed_lists/lists/regexp_list/db.py` & `FlexGet-3.6.3/flexget/components/managed_lists/lists/regexp_list/db.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/managed_lists/lists/regexp_list/regexp_list.py` & `FlexGet-3.6.3/flexget/components/managed_lists/lists/regexp_list/regexp_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/managed_lists/lists/sonarr_list.py` & `FlexGet-3.6.3/flexget/components/managed_lists/lists/sonarr_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/managed_lists/lists/subtitle_list.py` & `FlexGet-3.6.3/flexget/components/managed_lists/lists/subtitle_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/managed_lists/lists/thetvdb_list.py` & `FlexGet-3.6.3/flexget/components/managed_lists/lists/thetvdb_list.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         return set(it)
 
     def __init__(self, config):
         self.config = config
         self._items = None
 
     def __iter__(self):
-        return iter([item for item in self.items])
+        return iter(list(self.items))
 
     def __len__(self):
         return len(self.items)
 
     def __contains__(self, entry):
         return self._find_entry(entry) is not None
```

### Comparing `FlexGet-3.6.2/flexget/components/managed_lists/lists/yaml_list.py` & `FlexGet-3.6.3/flexget/components/managed_lists/lists/yaml_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         self.filename = path
         self.fields = fields
         self.encoding = encoding
 
         self.entries = []
         try:
             content = open(self.filename, encoding=self.encoding)
-        except FileNotFoundError as exc:
+        except FileNotFoundError:
             entries = []
             pass
         else:
             try:
                 # TODO: use the load from our serialization system if that goes in
                 entries = load_yaml(content)
             except Exception as exc:
```

### Comparing `FlexGet-3.6.2/flexget/components/notify/notification_framework.py` & `FlexGet-3.6.3/flexget/components/notify/notification_framework.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/notify/notifiers/bark.py` & `FlexGet-3.6.3/flexget/components/notify/notifiers/bark.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/notify/notifiers/cronitor.py` & `FlexGet-3.6.3/flexget/components/notify/notifiers/cronitor.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/notify/notifiers/discord.py` & `FlexGet-3.6.3/flexget/components/notify/notifiers/discord.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/notify/notifiers/email.py` & `FlexGet-3.6.3/flexget/components/notify/notifiers/email.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/notify/notifiers/gotify.py` & `FlexGet-3.6.3/flexget/components/notify/notifiers/gotify.py`

 * *Files 5% similar despite different names*

```diff
@@ -59,15 +59,15 @@
             'title': title,
             'message': message,
             'priority': priority,
             'extras': {'client::display': {'contentType': content_type}},
         }
         # Make the request
         try:
-            response = requests.post(url, params=params, json=notification)
+            requests.post(url, params=params, json=notification)
         except RequestException as e:
             if e.response is not None:
                 if e.response.status_code in (HTTPStatus.UNAUTHORIZED, HTTPStatus.FORBIDDEN):
                     message = 'Invalid Gotify access token'
                 else:
                     message = e.response.json()['error']['message']
             else:
```

### Comparing `FlexGet-3.6.2/flexget/components/notify/notifiers/ifttt.py` & `FlexGet-3.6.3/flexget/components/notify/notifiers/ifttt.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/notify/notifiers/join.py` & `FlexGet-3.6.3/flexget/components/notify/notifiers/join.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/notify/notifiers/matrix.py` & `FlexGet-3.6.3/flexget/components/notify/notifiers/matrix.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 def urljoin(*args):
     """
     Author: Rune Kaagaard
     Joins given arguments into an url. Trailing but not leading slashes are
     stripped for each argument.
     """
-    return "/".join(map(lambda x: str(x).rstrip('/'), args))
+    return "/".join(str(x).rstrip('/') for x in args)
 
 
 class MatrixNotifier:
     """
     Sends messages via Matrix. The MatrixHttpApi library is required to be installed.
     Install it with: `pip install matrix_client`
```

### Comparing `FlexGet-3.6.2/flexget/components/notify/notifiers/microsoftteams.py` & `FlexGet-3.6.3/flexget/components/notify/notifiers/microsoftteams.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/notify/notifiers/mqtt.py` & `FlexGet-3.6.3/flexget/components/notify/notifiers/mqtt.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,15 +144,15 @@
         client.on_disconnect = on_disconnect_cb
 
         # Handle SSL/TLS communication w/out certificate authentication
         if not config.get('certificates', {}).get('client_cert') and config.get(
             'encrypted_communication'
         ):
             client.tls_set(
-                ca_certs=certs.get('broker_ca_cert'),
+                ca_certs=config.get('certificates', {}).get('broker_ca_cert'),
                 certfile=None,
                 keyfile=None,
                 cert_reqs=ssl.CERT_NONE,
             )
 
             client.tls_insecure_set(True)
```

### Comparing `FlexGet-3.6.2/flexget/components/notify/notifiers/notifymyandroid.py` & `FlexGet-3.6.3/flexget/components/notify/notifiers/notifymyandroid.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/notify/notifiers/ntfysh.py` & `FlexGet-3.6.3/flexget/components/notify/notifiers/ntfysh.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 
         if 'delay' in config:
             req['params']['delay'] = config['delay']
         if 'tags' in config:
             req['params']['tags'] = config['tags']
 
         try:
-            response = requests.post(**req)
+            requests.post(**req)
         except RequestException as e:
             if e.response is not None:
                 if e.response.status_code in (HTTPStatus.UNAUTHORIZED, HTTPStatus.FORBIDDEN):
                     message = 'Invalid username and password'
                 else:
                     message = e.response.text()
             else:
```

### Comparing `FlexGet-3.6.2/flexget/components/notify/notifiers/prowl.py` & `FlexGet-3.6.3/flexget/components/notify/notifiers/prowl.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/notify/notifiers/pushalot.py` & `FlexGet-3.6.3/flexget/components/notify/notifiers/pushalot.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/notify/notifiers/pushbullet.py` & `FlexGet-3.6.3/flexget/components/notify/notifiers/pushbullet.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/notify/notifiers/pushover.py` & `FlexGet-3.6.3/flexget/components/notify/notifiers/pushover.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/notify/notifiers/pushsafer.py` & `FlexGet-3.6.3/flexget/components/notify/notifiers/pushsafer.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/notify/notifiers/rapidpush.py` & `FlexGet-3.6.3/flexget/components/notify/notifiers/rapidpush.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/notify/notifiers/slack.py` & `FlexGet-3.6.3/flexget/components/notify/notifiers/slack.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/notify/notifiers/sms_ru.py` & `FlexGet-3.6.3/flexget/components/notify/notifiers/sms_ru.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/notify/notifiers/telegram.py` & `FlexGet-3.6.3/flexget/components/notify/notifiers/telegram.py`

 * *Files 3% similar despite different names*

```diff
@@ -287,15 +287,15 @@
                 old_data = session.query(ChatIdEntry).filter(ChatIdEntry.id == old_id).first()
                 session.delete(old_data)
                 entry = ChatIdEntry(id=grp.id, group=grp.title)
                 self._update_db(session, [entry])
                 break
 
     def _send_msgs(self, msg, chat_ids, session):
-        kwargs = dict()
+        kwargs = {}
         if self._parse_mode == 'markdown':
             kwargs['parse_mode'] = telegram.ParseMode.MARKDOWN
         elif self._parse_mode == 'html':
             kwargs['parse_mode'] = telegram.ParseMode.HTML
         kwargs['disable_web_page_preview'] = self._disable_previews
         for chat_id in (x.id for x in chat_ids):
             try:
@@ -390,15 +390,15 @@
         :type session: sqlalchemy.orm.Session
         :type usernames: list[str]
         :type fullnames: list[tuple[str, str]]
         :type groups: list[str]
         :rtype: list[ChatIdEntry]
 
         """
-        chat_ids = list()
+        chat_ids = []
         cached_usernames = {
             x.username: x
             for x in session.query(ChatIdEntry).filter(ChatIdEntry.username != None).all()
         }
         cached_fullnames = {
             (x.firstname, x.surname): x
             for x in session.query(ChatIdEntry).filter(ChatIdEntry.firstname != None).all()
@@ -487,17 +487,17 @@
         while 1:
             ups = self._bot.getUpdates(last_upd, limit=100)
             updates.extend(ups)
             if len(ups) < 100:
                 break
             last_upd = ups[-1].update_id
 
-        usernames = dict()
-        fullnames = dict()
-        groups = dict()
+        usernames = {}
+        fullnames = {}
+        groups = {}
         for update in updates:
             if update.message:
                 chat = update.message.chat
             elif update.edited_message:
                 chat = update.edited_message.chat
             elif update.channel_post:
                 chat = update.channel_post.chat
```

### Comparing `FlexGet-3.6.2/flexget/components/notify/notifiers/toast.py` & `FlexGet-3.6.3/flexget/components/notify/notifiers/toast.py`

 * *Files 3% similar despite different names*

```diff
@@ -100,37 +100,33 @@
 
         if not n.show():
             raise PluginWarning('Unable to send notification for %s' % title)
 
     def windows_notify(self, title, message, config):
         config = self.prepare_config(config)
         try:
-            from win32api import GetModuleHandle, PostQuitMessage
+            from win32api import GetModuleHandle
             from win32con import (
                 CW_USEDEFAULT,
                 IDI_APPLICATION,
                 IMAGE_ICON,
                 LR_DEFAULTSIZE,
                 LR_LOADFROMFILE,
-                WM_DESTROY,
                 WM_USER,
                 WS_OVERLAPPED,
                 WS_SYSMENU,
             )
             from win32gui import (
                 NIF_ICON,
                 NIF_INFO,
                 NIF_MESSAGE,
                 NIF_TIP,
                 NIM_ADD,
-                NIM_DELETE,
-                NIM_MODIFY,
                 WNDCLASS,
                 CreateWindow,
-                DestroyWindow,
                 LoadIcon,
                 LoadImage,
                 RegisterClass,
                 Shell_NotifyIcon,
                 UpdateWindow,
             )
         except ImportError:
```

### Comparing `FlexGet-3.6.2/flexget/components/notify/notifiers/xmpp.py` & `FlexGet-3.6.3/flexget/components/notify/notifiers/xmpp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 
 from loguru import logger
 
 from flexget import plugin
 from flexget.config_schema import one_or_more
 from flexget.event import event
-from flexget.plugin import DependencyError, PluginWarning
+from flexget.plugin import DependencyError
 
 plugin_name = 'xmpp'
 
 logger = logger.bind(name=plugin_name)
 
 
 class XMPPNotifier:
@@ -41,15 +41,15 @@
         'additionalProperties': False,
     }
 
     __version__ = '1.0'
 
     def notify(self, title, message, config):
         try:
-            import sleekxmpp  # noqa
+            import sleekxmpp
         except ImportError as e:
             logger.debug('Error importing SleekXMPP: {}', e)
             raise DependencyError(
                 plugin_name, 'sleekxmpp', 'SleekXMPP module required. ImportError: %s' % e
             )
         try:
             import dns  # noqa
```

### Comparing `FlexGet-3.6.2/flexget/components/notify/notify.py` & `FlexGet-3.6.3/flexget/components/notify/notify.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/parsing/parsers/parser_common.py` & `FlexGet-3.6.3/flexget/components/parsing/parsers/parser_common.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/parsing/parsers/parser_guessit.py` & `FlexGet-3.6.3/flexget/components/parsing/parsers/parser_guessit.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 from flexget.utils.tools import ReList
 
 from .parser_common import MovieParseResult, SeriesParseResult
 
 # rebulk (that underlies guessit) will use the 'regex' module rather than 're' if installed.
 # For consistency, prevent that unless env variable is explicitly already enabling it.
 os.environ.setdefault('REGEX_DISABLED', 'true')  # isort:skip
-from guessit.api import GuessItApi, GuessitException  # isort:skip
-from guessit.rules import rebulk_builder  # isort:skip
-from rebulk import Rebulk  # isort:skip
-from rebulk.pattern import RePattern  # isort:skip
+from guessit.api import GuessItApi, GuessitException  # isort:skip # noqa: E402
+from guessit.rules import rebulk_builder  # isort:skip # noqa: E402
+from rebulk import Rebulk  # isort:skip # noqa: E402
+from rebulk.pattern import RePattern  # isort:skip # noqa: E402
 
 
 logger = logger.bind(name='parser_guessit')
 
 logging.getLogger('rebulk').setLevel(logging.WARNING)
 logging.getLogger('guessit').setLevel(logging.WARNING)
 
@@ -412,15 +412,15 @@
         # regexp name matching
         re_from_name = False
         name_regexps = ReList(guessit_options.get('name_regexps', []))
         if not name_regexps:
             # if we don't have name_regexps, generate one from the name
             name_regexps = ReList(
                 name_to_re(name, default_ignore_prefixes, None)
-                for name in [guessit_options['name']] + guessit_options.get('alternate_names', [])
+                for name in [guessit_options['name'], *guessit_options.get('alternate_names', [])]
             )
             # With auto regex generation, the first regex group captures the name
             re_from_name = True
         # try all specified regexps on this data
         for name_re in name_regexps:
             match = re.search(name_re, data)
             if match:
```

### Comparing `FlexGet-3.6.2/flexget/components/parsing/parsers/parser_internal.py` & `FlexGet-3.6.3/flexget/components/parsing/parsers/parser_internal.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/parsing/plugin_parsing.py` & `FlexGet-3.6.3/flexget/components/parsing/plugin_parsing.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/pending_approval/api.py` & `FlexGet-3.6.3/flexget/components/pending_approval/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,15 +165,15 @@
         deleted = session.query(db.PendingEntry)
         if task_name:
             deleted = deleted.filter(db.PendingEntry.task_name == task_name)
         if approved:
             deleted = deleted.filter(db.PendingEntry.approved == approved)
         deleted = deleted.delete()
 
-        return success_response(f'deleted %s pending entries')
+        return success_response(f'deleted {deleted} pending entries')
 
 
 @pending_api.route('/<int:entry_id>/')
 @api.doc(params={'entry_id': 'ID of the entry'})
 @api.response(NotFoundError)
 class PendingEntryAPI(APIResource):
     @etag
```

### Comparing `FlexGet-3.6.2/flexget/components/pending_approval/cli.py` & `FlexGet-3.6.3/flexget/components/pending_approval/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         if value != 'all':
             raise ArgumentTypeError('Must select \'all\' or valid entry ID')
     return value
 
 
 def do_cli(manager, options):
     if hasattr(options, 'table_type') and options.table_type == 'porcelain':
-        disable_all_colors()
+        disable_colors()
 
     if options.action == 'list':
         list_entries(options)
     elif options.action == 'approve':
         manage_entries(options, options.selection, True)
     elif options.action == 'reject':
         manage_entries(options, options.selection, False)
```

### Comparing `FlexGet-3.6.2/flexget/components/pending_approval/db.py` & `FlexGet-3.6.3/flexget/components/pending_approval/db.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/pending_approval/pending_approval.py` & `FlexGet-3.6.3/flexget/components/pending_approval/pending_approval.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/rejected/api.py` & `FlexGet-3.6.3/flexget/components/rejected/api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/rejected/cli.py` & `FlexGet-3.6.3/flexget/components/rejected/cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,14 @@
-from flexget import options, plugin
+from flexget import options
 from flexget.event import event
 from flexget.manager import Session
 from flexget.terminal import TerminalTable, console, table_parser
 
 from . import db
 
-try:
-    # NOTE: Importing other plugins is discouraged!
-    from flexget.components.rejected import remember_rejected as plugin_remember_rejected
-except ImportError:
-    raise plugin.DependencyError(issued_by=__name__, missing='remember_rejected')
-
 
 def do_cli(manager, options):
     if options.rejected_action == 'list':
         list_rejected(options)
     elif options.rejected_action == 'clear':
         clear_rejected(manager)
```

### Comparing `FlexGet-3.6.2/flexget/components/rejected/db.py` & `FlexGet-3.6.3/flexget/components/rejected/db.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/rejected/remember_rejected.py` & `FlexGet-3.6.3/flexget/components/rejected/remember_rejected.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/scheduler/api.py` & `FlexGet-3.6.3/flexget/components/scheduler/api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/scheduler/scheduler.py` & `FlexGet-3.6.3/flexget/components/scheduler/scheduler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import hashlib
 import logging
 import os
-import struct
 
 from apscheduler.jobstores.sqlalchemy import SQLAlchemyJobStore
 from apscheduler.schedulers.background import BackgroundScheduler
 from apscheduler.triggers.cron import CronTrigger
 from loguru import logger
 
 from flexget.config_schema import format_checker, register_config_key, register_schema
```

### Comparing `FlexGet-3.6.2/flexget/components/seen/api.py` & `FlexGet-3.6.3/flexget/components/seen/api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/seen/cli.py` & `FlexGet-3.6.3/flexget/components/seen/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         if imdb_id:
             seen_name = imdb_id
         else:
             console("Could not parse IMDB ID")
 
     task = DEFAULT_TASK
     local = None
-    if options.task and not options.task in manager.tasks:
+    if options.task and options.task not in manager.tasks:
         console(f"Task `{options.task}` not in config")
         return
     else:
         task = options.task
         local = True
 
     db.add(seen_name, task, {'cli_add': seen_name}, local=local)
```

### Comparing `FlexGet-3.6.2/flexget/components/seen/db.py` & `FlexGet-3.6.3/flexget/components/seen/db.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,17 +3,15 @@
 
 forget (string)
 
     Given string can be task name, remembered field (url, imdb_url) or a title. If given value is a
     task name then everything in that task will be forgotten. With title all learned fields from it and the
     title will be forgotten. With field value only that particular field is forgotten.
 """
-import string
 from datetime import datetime
-from glob import escape
 
 from loguru import logger
 from sqlalchemy import (
     Boolean,
     Column,
     DateTime,
     ForeignKey,
@@ -212,15 +210,15 @@
                 )
             else:
                 logger.debug('forgetting {}', se)
                 session.delete(se)
 
         for sf in query_sf.all():
             se = session.query(SeenEntry).filter(SeenEntry.id == sf.seen_entry_id).first()
-            if tasks and not se.task in tasks:
+            if tasks and se.task not in tasks:
                 continue
             field_count += len(se.fields)
             count += 1
 
             if test:
                 logger.info(
                     f'Testing: would forget entry `{se.title}` of task `{se.task}` based on field `{sf.field}` with value `{sf.value}`'
```

### Comparing `FlexGet-3.6.2/flexget/components/seen/seen.py` & `FlexGet-3.6.3/flexget/components/seen/seen.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/seen/seen_info_hash.py` & `FlexGet-3.6.3/flexget/components/seen/seen_info_hash.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/seen/seen_movies.py` & `FlexGet-3.6.3/flexget/components/seen/seen_movies.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/series/all_series.py` & `FlexGet-3.6.3/flexget/components/series/all_series.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/series/api.py` & `FlexGet-3.6.3/flexget/components/series/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -520,15 +520,15 @@
         return success_response('successfully removed all series %s seasons from DB' % show_id)
 
 
 @api.response(NotFoundError)
 @api.response(BadRequest)
 @series_api.route('/<int:show_id>/seasons/<int:season_id>/')
 @api.doc(params={'show_id': 'ID of the show', 'season_id': 'Season ID'})
-class SeriesSeasonsAPI(APIResource):
+class SeriesSeasonAPI(APIResource):
     @etag
     @api.response(200, 'Season retrieved successfully for show', season_schema)
     @api.doc(description='Get a specific season via its ID and show ID')
     def get(self, show_id, season_id, session):
         """Get season by show ID and season ID"""
         try:
             db.show_by_id(show_id, session=session)
```

### Comparing `FlexGet-3.6.2/flexget/components/series/cli.py` & `FlexGet-3.6.3/flexget/components/series/cli.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/series/configure_series.py` & `FlexGet-3.6.3/flexget/components/series/configure_series.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/series/db.py` & `FlexGet-3.6.3/flexget/components/series/db.py`

 * *Files 1% similar despite different names*

```diff
@@ -766,16 +766,18 @@
     for alt_name in alt_names:
         db_series_alt = (
             session.query(AlternateNames).filter(AlternateNames.alt_name == alt_name).first()
         )
         if db_series_alt:
             if not db_series_alt.series_id == db_series.id:
                 raise plugin.PluginError(
-                    'Error adding alternate name for `%s`: `%s` is already associated with `%s`. '
-                    'Check your settings.' % (db_series.name, alt_name, db_series_alt.series.name)
+                    'Error adding alternate name for `{}`: `{}` is already associated with `{}`. '
+                    'Check your settings.'.format(
+                        db_series.name, alt_name, db_series_alt.series.name
+                    )
                 )
             else:
                 logger.debug(
                     'alternate name `{}` already associated with series `{}`, no change needed',
                     alt_name,
                     db_series.name,
                 )
@@ -806,17 +808,23 @@
 
 def get_all_entities(
     series: Series, session: Session, sort_by: str = 'age', reverse: bool = False
 ) -> List[Union[Episode, Season]]:
     episodes = show_episodes(series, session=session)
     seasons = show_seasons(series, session=session)
     if sort_by == 'identifier':
-        key = lambda e: e.identifier
+
+        def key(e):
+            return e.identifier
+
     else:
-        key = lambda e: (e.first_seen or datetime.min, e.identifier)
+
+        def key(e):
+            return e.first_seen or datetime.min, e.identifier
+
     return sorted(episodes + seasons, key=key, reverse=reverse)
 
 
 def get_episode_releases(
     episode: Episode,
     downloaded: bool = None,
     start: int = None,
@@ -907,16 +915,16 @@
                 alt,
                 series_name,
             )
             db_series.alternate_names.append(db_series_alt)
         else:
             # Alternate name already exists for another series. Not good.
             raise plugin.PluginError(
-                'Error adding alternate name for `%s`: `%s` is already associated with `%s`. '
-                'Check your settings.' % (series_name, alt, db_series_alt.series.name)
+                'Error adding alternate name for `{}`: `{}` is already associated with `{}`. '
+                'Check your settings.'.format(series_name, alt, db_series_alt.series.name)
             )
     else:
         logger.debug('adding alternate name `{}` for `{}` into db', alt, series_name)
         db_series_alt = AlternateNames(alt)
         db_series.alternate_names.append(db_series_alt)
         logger.debug('-> added {}', db_series_alt)
```

### Comparing `FlexGet-3.6.2/flexget/components/series/gen_series.py` & `FlexGet-3.6.3/flexget/components/series/gen_series.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/series/internal_estimator.py` & `FlexGet-3.6.3/flexget/components/series/internal_estimator.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/series/metainfo_series.py` & `FlexGet-3.6.3/flexget/components/series/metainfo_series.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/series/next_series_episodes.py` & `FlexGet-3.6.3/flexget/components/series/next_series_episodes.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/series/next_series_seasons.py` & `FlexGet-3.6.3/flexget/components/series/next_series_seasons.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/series/series.py` & `FlexGet-3.6.3/flexget/components/series/series.py`

 * *Files 2% similar despite different names*

```diff
@@ -573,26 +573,26 @@
 
         # set parser flags flags based on config / database
         identified_by = config.get('identified_by', 'auto')
         if identified_by == 'auto':
             # set flag from database
             identified_by = db_identified_by or 'auto'
 
-        params = dict(
-            identified_by=identified_by,
-            alternate_names=get_config_as_array(config, 'alternate_name'),
-            name_regexps=get_config_as_array(config, 'name_regexp'),
-            strict_name=config.get('exact', False),
-            allow_groups=get_config_as_array(config, 'from_group'),
-            date_yearfirst=config.get('date_yearfirst'),
-            date_dayfirst=config.get('date_dayfirst'),
-            special_ids=get_config_as_array(config, 'special_ids'),
-            prefer_specials=config.get('prefer_specials'),
-            assume_special=config.get('assume_special'),
-        )
+        params = {
+            'identified_by': identified_by,
+            'alternate_names': get_config_as_array(config, 'alternate_name'),
+            'name_regexps': get_config_as_array(config, 'name_regexp'),
+            'strict_name': config.get('exact', False),
+            'allow_groups': get_config_as_array(config, 'from_group'),
+            'date_yearfirst': config.get('date_yearfirst'),
+            'date_dayfirst': config.get('date_dayfirst'),
+            'special_ids': get_config_as_array(config, 'special_ids'),
+            'prefer_specials': config.get('prefer_specials'),
+            'assume_special': config.get('assume_special'),
+        }
         for id_type in plugin_parser_common.SERIES_ID_TYPES:
             params[id_type + '_regexps'] = get_config_as_array(config, id_type + '_regexp')
 
         parser = plugin.get('parsing', self)
         for entry in entries:
             # skip processed entries
             if (
```

### Comparing `FlexGet-3.6.2/flexget/components/series/series_begin.py` & `FlexGet-3.6.3/flexget/components/series/series_begin.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/series/series_premiere.py` & `FlexGet-3.6.3/flexget/components/series/series_premiere.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/series/series_remove.py` & `FlexGet-3.6.3/flexget/components/series/series_remove.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/sites/sites/allyoulike.py` & `FlexGet-3.6.3/flexget/components/sites/sites/allyoulike.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/sites/sites/alpharatio.py` & `FlexGet-3.6.3/flexget/components/sites/sites/alpharatio.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,17 +7,16 @@
 
 from flexget import db_schema, plugin
 from flexget.config_schema import one_or_more
 from flexget.entry import Entry
 from flexget.event import event
 from flexget.manager import Session
 from flexget.utils.database import json_synonym
-from flexget.utils.requests import RequestException
+from flexget.utils.requests import RequestException, TimedLimiter
 from flexget.utils.requests import Session as RequestSession
-from flexget.utils.requests import TimedLimiter
 from flexget.utils.soup import get_soup
 from flexget.utils.tools import parse_filesize
 
 logger = logger.bind(name='alpharatio')
 Base = db_schema.versioned_base('alpharatio', 0)
 
 requests = RequestSession()
@@ -304,15 +303,15 @@
                 mappings_int = {
                     'torrent_snatches': snatches_idx,
                     'torrent_seeds': seeds_idx,
                     'torrent_leeches': leeches_idx,
                 }
 
                 for dest, src in mappings_int.items():
-                    if not src in torrent_info:
+                    if src not in torrent_info:
                         continue
 
                     # Some values are tagged with a ',' insted of a '.', replace them
                     value = torrent_info[src].text.replace(',', '.')
 
                     try:
                         e[dest] = int(value)
```

### Comparing `FlexGet-3.6.2/flexget/components/sites/sites/animeindex.py` & `FlexGet-3.6.3/flexget/components/sites/sites/animeindex.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/sites/sites/anirena.py` & `FlexGet-3.6.3/flexget/components/sites/sites/anirena.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/sites/sites/archetorrent.py` & `FlexGet-3.6.3/flexget/components/sites/sites/archetorrent.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/sites/sites/argenteam.py` & `FlexGet-3.6.3/flexget/components/sites/sites/argenteam.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/sites/sites/awesomehd.py` & `FlexGet-3.6.3/flexget/components/sites/sites/awesomehd.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/sites/sites/bakabt.py` & `FlexGet-3.6.3/flexget/components/sites/sites/bakabt.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/sites/sites/btn.py` & `FlexGet-3.6.3/flexget/components/sites/sites/btn.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/sites/sites/cinemageddon.py` & `FlexGet-3.6.3/flexget/components/sites/sites/cinemageddon.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/sites/sites/cpasbien.py` & `FlexGet-3.6.3/flexget/components/sites/sites/cpasbien.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/sites/sites/deadfrog.py` & `FlexGet-3.6.3/flexget/components/sites/sites/deadfrog.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/sites/sites/descargas2020.py` & `FlexGet-3.6.3/flexget/components/sites/sites/descargas2020.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/sites/sites/ettv.py` & `FlexGet-3.6.3/flexget/components/sites/sites/ettv.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/sites/sites/eztv.py` & `FlexGet-3.6.3/flexget/components/sites/sites/eztv.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         url = entry['url']
         page = None
         for scheme, netloc in EZTV_MIRRORS:
             try:
                 _, _, path, params, query, fragment = urlparse(url)
                 url = urlunparse((scheme, netloc, path, params, query, fragment))
                 page = task.requests.get(url).content
-            except RequestException as e:
+            except RequestException:
                 logger.debug('Eztv mirror `{}` seems to be down', url)
                 continue
             break
 
         if not page:
             raise UrlRewritingError('No mirrors found for url %s' % entry['url'])
```

### Comparing `FlexGet-3.6.2/flexget/components/sites/sites/filelist.py` & `FlexGet-3.6.3/flexget/components/sites/sites/filelist.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,17 +5,16 @@
 from sqlalchemy import Column, DateTime, Unicode
 
 from flexget import db_schema, plugin
 from flexget.entry import Entry
 from flexget.event import event
 from flexget.manager import Session
 from flexget.utils.database import json_synonym
-from flexget.utils.requests import RequestException
+from flexget.utils.requests import RequestException, TimedLimiter
 from flexget.utils.requests import Session as RequestSession
-from flexget.utils.requests import TimedLimiter
 from flexget.utils.soup import get_soup
 from flexget.utils.tools import parse_filesize
 
 logger = logger.bind(name='filelist')
 Base = db_schema.versioned_base('filelist', 0)
 
 requests = RequestSession()
@@ -190,15 +189,15 @@
             return cookie.cookie
 
     @plugin.internet(logger)
     def search(self, task, entry, config):
         """
         Search for entries on FileList.ro
         """
-        entries = list()
+        entries = []
 
         params = {
             'cat': CATEGORIES[config['category']],
             'incldead': int(config['include_dead']),
             'order_by': SORTING[config['order_by']],
             'searchin': SEARCH_IN[config['search_in']],
             'asc': int(config['order_ascending']),
```

### Comparing `FlexGet-3.6.2/flexget/components/sites/sites/filelist_api.py` & `FlexGet-3.6.3/flexget/components/sites/sites/filelist_api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/sites/sites/frenchtorrentdb.py` & `FlexGet-3.6.3/flexget/components/sites/sites/frenchtorrentdb.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/sites/sites/fuzer.py` & `FlexGet-3.6.3/flexget/components/sites/sites/fuzer.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/sites/sites/google_cse.py` & `FlexGet-3.6.3/flexget/components/sites/sites/google_cse.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/sites/sites/hebits.py` & `FlexGet-3.6.3/flexget/components/sites/sites/hebits.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/sites/sites/hliang.py` & `FlexGet-3.6.3/flexget/components/sites/sites/hliang.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/sites/sites/horriblesubs.py` & `FlexGet-3.6.3/flexget/components/sites/sites/horriblesubs.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/sites/sites/iptorrents.py` & `FlexGet-3.6.3/flexget/components/sites/sites/iptorrents.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,15 +148,15 @@
 
         if not task.requests.domain_limiters.get(DOMAIN, None):
             logger.debug('limiting requests with a delay of {}', DELAY)
             rate_limiter = requests.TokenBucketLimiter(DOMAIN, 1, DELAY, True)
             task.requests.add_domain_limiter(rate_limiter)
 
         for search_string in entry.get('search_strings', [entry['title']]):
-            search_params = {key: value for (key, value) in category_params.items()}
+            search_params = dict(category_params.items())
 
             query = normalize_unicode(search_string)
             search_params.update({'q': query, 'qf': ''})
 
             logger.debug('searching with params: {}', search_params)
             if config.get('free'):
                 req = task.requests.get(
```

### Comparing `FlexGet-3.6.2/flexget/components/sites/sites/koreus.py` & `FlexGet-3.6.3/flexget/components/sites/sites/koreus.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/sites/sites/limetorrents.py` & `FlexGet-3.6.3/flexget/components/sites/sites/limetorrents.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/sites/sites/lostfilm.py` & `FlexGet-3.6.3/flexget/components/sites/sites/lostfilm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import re
 from urllib.request import ProxyHandler
 
 import feedparser
 from loguru import logger
 
-from flexget import entry, plugin
+from flexget import plugin
 from flexget.components.sites.utils import normalize_unicode
 from flexget.entry import Entry
 from flexget.event import event
 from flexget.plugin import PluginError
 from flexget.utils import qualities
 from flexget.utils.requests import RequestException
 from flexget.utils.soup import get_soup
@@ -115,15 +115,15 @@
             },
         },
         'additionalProperties': False,
     }
 
     def build_config(self, config):
         """Set defaults to config"""
-        cfg = dict()
+        cfg = {}
         if isinstance(config, bool):
             cfg['enabled'] = bool(config)
         elif isinstance(config, str):
             cfg['lf_session'] = str(config)
             cfg['enabled'] = True
         else:
             cfg = dict(config)
@@ -230,15 +230,15 @@
             # It's better to process an extra item which will be filtered later by
             # series plugin than throw out actually needed item because incorrectly
             # matched name was not found in the pre-filter list.
             if prefilter_list:
                 if perfect_match:
                     try:
                         folded_name = self._simplify_name(series_name_org)
-                    except TextProcessingError as e:
+                    except TextProcessingError:
                         logger.warning('RSS item series name "{}" could be wrong', series_name_org)
                         folded_name = None
                     if folded_name and folded_name not in prefilter_list:
                         if idx != len(rss.entries) or entries or task.no_entries_ok:
                             logger.debug(
                                 'Skipping "{}" as "{}" was not found in the list of configured series',
                                 item['title'],
@@ -436,15 +436,15 @@
                             ),
                             int(info_match['season']),
                             int(info_match['episode']),
                             season_num,
                             episode_num,
                         )
                         season_num = int(info_match['season'])
-                        eposode_num = int(info_match['episode'])
+                        episode_num = int(info_match['episode'])
                     if info_match['ep_org'] is not None:
                         episode_name_org = info_match['ep_org'].strip()
                     if (
                         not perfect_match
                         and info_match['ep_rus'] is not None
                         and info_match['ep_rus'].strip()
                     ):
@@ -612,14 +612,14 @@
                         # A list of alternate names
                         for a_name in s_cfg['alternate_name']:
                             names_list.add(LostFilm._simplify_name(a_name))
                     else:
                         raise PluginError(f'Cannot read series "alternate_name" for "{s_name:s}"')
             else:
                 raise PluginError(
-                    'Series configuration list item has ' 'unsupported type: %s' % type(s_item)
+                    'Series configuration list item has unsupported type: %s' % type(s_item)
                 )
 
 
 @event('plugin.register')
 def register_plugin():
     plugin.register(LostFilm, 'lostfilm', api_ver=2)
```

### Comparing `FlexGet-3.6.2/flexget/components/sites/sites/magnetdl.py` & `FlexGet-3.6.3/flexget/components/sites/sites/magnetdl.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import random
 import re
 import time
 import unicodedata
-from urllib.parse import quote
 
 from loguru import logger
 from requests import RequestException
 
 from flexget import plugin
 from flexget.entry import Entry
 from flexget.event import event
```

### Comparing `FlexGet-3.6.2/flexget/components/sites/sites/morethantv.py` & `FlexGet-3.6.3/flexget/components/sites/sites/morethantv.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,17 +7,16 @@
 
 from flexget import db_schema, plugin
 from flexget.config_schema import one_or_more
 from flexget.entry import Entry
 from flexget.event import event
 from flexget.manager import Session
 from flexget.utils.database import json_synonym
-from flexget.utils.requests import RequestException
+from flexget.utils.requests import RequestException, TimedLimiter
 from flexget.utils.requests import Session as RequestSession
-from flexget.utils.requests import TimedLimiter
 from flexget.utils.soup import get_soup
 from flexget.utils.tools import parse_filesize
 
 SITE_DOMAIN = 'morethantv.me'
 SITE_URL = f'https://www.{SITE_DOMAIN}/'
 
 logger = logger.bind(name='morethantv')
```

### Comparing `FlexGet-3.6.2/flexget/components/sites/sites/ncore.py` & `FlexGet-3.6.3/flexget/components/sites/sites/ncore.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import re
 
 from loguru import logger
 
 from flexget import plugin
-from flexget.components.sites.urlrewriting import UrlRewritingError
 from flexget.components.sites.utils import torrent_availability
 from flexget.entry import Entry
 from flexget.event import event
 from flexget.utils.requests import TokenBucketLimiter
 from flexget.utils.soup import get_soup
 
 logger = logger.bind(name='nCore')
@@ -83,16 +82,14 @@
         }
 
         page = task.requests.post(URL + "/login.php", data=data, headers=HEADERS)
         soup = get_soup(page.content)
         passkey_line = str(soup.find('link', href=re.compile(r'rss\.php\?key=')))
         PASSKEY = passkey_line[passkey_line.find("key=") : passkey_line.find('"', 20, 90)]
 
-        entries = set()
-
         for search_string in entry.get('search_strings', [entry['title']]):
             data = {
                 "mire": search_string,
                 "miben": "name",
                 "miszerint": SORT[config.get('sort_by')],
             }
```

### Comparing `FlexGet-3.6.2/flexget/components/sites/sites/newtorrents.py` & `FlexGet-3.6.3/flexget/components/sites/sites/newtorrents.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     # UrlRewriter plugin API
     def url_rewritable(self, task, entry):
         # Return true only for urls that can and should be resolved
         if entry['url'].startswith('http://www.newtorrents.info/down.php?'):
             return False
         return (
             entry['url'].startswith('http://www.newtorrents.info')
-            and not entry['url'] in self.resolved
+            and entry['url'] not in self.resolved
         )
 
     # UrlRewriter plugin API
     def url_rewrite(self, task, entry):
         url = entry['url']
         if url.startswith('http://www.newtorrents.info/?q=') or url.startswith(
             'http://www.newtorrents.info/search'
```

### Comparing `FlexGet-3.6.2/flexget/components/sites/sites/newznab.py` & `FlexGet-3.6.3/flexget/components/sites/sites/newznab.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/sites/sites/nnmclub.py` & `FlexGet-3.6.3/flexget/components/sites/sites/nnmclub.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/sites/sites/nyaa.py` & `FlexGet-3.6.3/flexget/components/sites/sites/nyaa.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/sites/sites/passthepopcorn.py` & `FlexGet-3.6.3/flexget/components/sites/sites/passthepopcorn.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,17 +7,16 @@
 
 from flexget import db_schema, plugin
 from flexget.config_schema import one_or_more
 from flexget.entry import Entry
 from flexget.event import event
 from flexget.manager import Session
 from flexget.utils.database import json_synonym
-from flexget.utils.requests import RequestException
+from flexget.utils.requests import RequestException, TimedLimiter
 from flexget.utils.requests import Session as RequestSession
-from flexget.utils.requests import TimedLimiter
 from flexget.utils.tools import parse_filesize
 
 logger = logger.bind(name='passthepopcorn')
 Base = db_schema.versioned_base('passthepopcorn', 1)
 
 requests = RequestSession()
 requests.add_domain_limiter(TimedLimiter('passthepopcorn.me', '5 seconds'))
```

### Comparing `FlexGet-3.6.2/flexget/components/sites/sites/piratebay.py` & `FlexGet-3.6.3/flexget/components/sites/sites/piratebay.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,15 +146,15 @@
         entries = set()
         for search_string in entry.get('search_strings', [entry['title']]):
             # query = normalize_unicode(search_string)
             params = {'q': search_string, 'cat': category}
             url = f'{self.url}/q.php'
             try:
                 json_results = task.requests.get(url, params=params).json()
-            except JSONDecodeError as e:
+            except JSONDecodeError:
                 raise plugin.PluginError(
                     f'Error while searching piratebay for {search_string}, invalid json response',
                 )
 
             if not json_results:
                 raise plugin.PluginError(f'Error while searching piratebay for {search_string}.')
             for result in json_results:
```

### Comparing `FlexGet-3.6.2/flexget/components/sites/sites/ptn.py` & `FlexGet-3.6.3/flexget/components/sites/sites/ptn.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,15 @@
         'required': ['username', 'login_key', 'password'],
         'additionalProperties': False,
     }
 
     def create_entries(self, soup, imdb_id=None):
         entries = []
         links = soup.findAll('a', attrs={'href': re.compile(r'download\.php\?torrent=\d+')})
-        rows = [l.find_parent('tr') for l in links]
+        rows = [link.find_parent('tr') for link in links]
         for row in rows:
             entry = Entry()
             entry['title'] = row.find('a', attrs={'href': re.compile(r'detail\.php\?id')}).text
             dl_href = row.find('a', attrs={'href': re.compile(r'download\.php\?torrent=\d+')}).get(
                 'href'
             )
             entry['url'] = 'http://piratethenet.org' + dl_href
```

### Comparing `FlexGet-3.6.2/flexget/components/sites/sites/rarbg.py` & `FlexGet-3.6.3/flexget/components/sites/sites/rarbg.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/sites/sites/redirect.py` & `FlexGet-3.6.3/flexget/components/sites/sites/redirect.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/sites/sites/rlsbb.py` & `FlexGet-3.6.3/flexget/components/sites/sites/rlsbb.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/sites/sites/rmz.py` & `FlexGet-3.6.3/flexget/components/sites/sites/rmz.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/sites/sites/rss.py` & `FlexGet-3.6.3/flexget/components/sites/sites/rss.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/sites/sites/rutracker.py` & `FlexGet-3.6.3/flexget/components/sites/sites/rutracker.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/sites/sites/serienjunkies.py` & `FlexGet-3.6.3/flexget/components/sites/sites/serienjunkies.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/sites/sites/shortened.py` & `FlexGet-3.6.3/flexget/components/sites/sites/shortened.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/sites/sites/site_1337x.py` & `FlexGet-3.6.3/flexget/components/sites/sites/site_1337x.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/sites/sites/site_rutracker.py` & `FlexGet-3.6.3/flexget/components/sites/sites/site_rutracker.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/sites/sites/solidtorrents.py` & `FlexGet-3.6.3/flexget/components/sites/sites/solidtorrents.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from datetime import datetime
 from urllib.parse import urlparse
 
 from loguru import logger
 
 from flexget import plugin
 from flexget.components.sites.urlrewriting import UrlRewritingError
-from flexget.components.sites.utils import normalize_unicode, torrent_availability
+from flexget.components.sites.utils import torrent_availability
 from flexget.entry import Entry
 from flexget.event import event
 
 logger = logger.bind(name='solidtorrents')
 
 URL = 'https://solidtorrents.net/'
 
@@ -100,15 +100,15 @@
             entry['url'] = results[0]['url']
         else:
             torrent_id = self.url_match(entry['url']).group(1)
             url = f"{self.url}/api/v1/torrents/{torrent_id}"
             logger.debug('Getting info for torrent ID {}', torrent_id)
             json_result = task.requests.get(url).json()
             # if json_result['error'] == '404':
-            if not 'result' in json_result:
+            if 'result' not in json_result:
                 raise UrlRewritingError("Torrent with ID %s does not exist." % torrent_id)
             entry['url'] = json_result['result']['rating']['magnet']
 
     @plugin.internet(logger)
     def search(self, task, entry, config=None):
         """
         Search for name from solidtorrents.
@@ -117,30 +117,30 @@
             config = {}
         self.set_urls(config.get('url', URL))
         sort = config.get('sort_by', 'seeders')
         reverse = bool(config.get('reverse', 'False'))
         remove_potentially_unsafe = bool(config.get('remove_potentially_unsafe', 'True'))
         category = config.get('category', 'all')
 
-        entries = list()
+        entries = []
         for search_string in entry.get('search_strings', [entry['title']]):
             # query = normalize_unicode(search_string)
             params = {
                 'q': search_string,
                 'cat': category,
                 'sort': sort,
                 'fuv': remove_potentially_unsafe,
             }
             url = f"{self.url}/api/v1/search"
             json_results = task.requests.get(url, params=params).json()
             if not json_results:
                 raise plugin.PluginError(
                     "Error while searching solidtorrents for %s.", search_string
                 )
-            if not 'results' in json_results:
+            if 'results' not in json_results:
                 logger.info(
                     "No result founds while searching solidtorrents for %s.", search_string
                 )
                 continue
             for result in json_results['results']:
                 entry = self.json_to_entry(result)
                 entries.append(entry)
```

### Comparing `FlexGet-3.6.2/flexget/components/sites/sites/torrent_cache.py` & `FlexGet-3.6.3/flexget/components/sites/sites/torrent_cache.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/sites/sites/torrentday.py` & `FlexGet-3.6.3/flexget/components/sites/sites/torrentday.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/sites/sites/torrentleech.py` & `FlexGet-3.6.3/flexget/components/sites/sites/torrentleech.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/sites/sites/torrentz.py` & `FlexGet-3.6.3/flexget/components/sites/sites/torrentz.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/sites/sites/wordpress.py` & `FlexGet-3.6.3/flexget/components/sites/sites/wordpress.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/sites/sites/yts.py` & `FlexGet-3.6.3/flexget/components/sites/sites/yts.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/sites/urlrewrite.py` & `FlexGet-3.6.3/flexget/components/sites/urlrewrite.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/sites/urlrewrite_search.py` & `FlexGet-3.6.3/flexget/components/sites/urlrewrite_search.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/sites/urlrewriting.py` & `FlexGet-3.6.3/flexget/components/sites/urlrewriting.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/sites/utils.py` & `FlexGet-3.6.3/flexget/components/sites/utils.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/status/api.py` & `FlexGet-3.6.3/flexget/components/status/api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/status/cli.py` & `FlexGet-3.6.3/flexget/components/status/cli.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/status/db.py` & `FlexGet-3.6.3/flexget/components/status/db.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/status/status.py` & `FlexGet-3.6.3/flexget/components/status/status.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/thetvdb/api.py` & `FlexGet-3.6.3/flexget/components/thetvdb/api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/thetvdb/api_tvdb.py` & `FlexGet-3.6.3/flexget/components/thetvdb/api_tvdb.py`

 * *Files 0% similar despite different names*

```diff
@@ -275,15 +275,15 @@
                 else:
                     raise LookupError(f'Error updating posters from tvdb: {e}')
 
         return [TVDBRequest.BANNER_URL + p for p in self.posters_list[:5]]
 
     def to_dict(self):
         return {
-            'aliases': [a for a in self.aliases],
+            'aliases': list(self.aliases),
             'tvdb_id': self.id,
             'last_updated': datetime.fromtimestamp(self.last_updated).strftime(
                 '%Y-%m-%d %H:%M:%S'
             ),
             'expired': self.expired,
             'series_name': self.name,
             'language': self.language,
@@ -295,15 +295,15 @@
             'content_rating': self.content_rating,
             'network': self.network,
             'overview': self.overview,
             'imdb_id': self.imdb_id,
             'zap2it_id': self.zap2it_id,
             'banner': self.banner,
             'posters': self.posters,
-            'genres': [g for g in self.genres],
+            'genres': list(self.genres),
             'first_aired': self.first_aired,
         }
 
 
 class TVDBGenre(Base):
     __tablename__ = 'tvdb_genres'
     id = Column(Unicode, primary_key=True)
@@ -444,15 +444,15 @@
     @property
     def banner(self):
         if self._banner:
             return TVDBRequest.BANNER_URL + self._banner
 
     def to_dict(self):
         return {
-            'aliases': [a for a in self.aliases],
+            'aliases': list(self.aliases),
             'banner': self.banner,
             'first_aired': self.first_aired,
             'tvdb_id': self.id,
             'network': self.network,
             'overview': self.overview,
             'series_name': self.name,
             'status': self.status,
@@ -518,15 +518,15 @@
     return series[0]['id']
 
 
 def _update_search_strings(series, session, search=None):
     search_strings = series.search_strings
     aliases = [a.lower() for a in series.aliases] if series.aliases else []
     searches = [search.lower()] if search else []
-    add = [series.name.lower()] + aliases + searches
+    add = [series.name.lower(), *aliases, *searches]
     for name in set(add):
         if name not in search_strings:
             search_result = (
                 session.query(TVDBSearchResult).filter(TVDBSearchResult.search == name).first()
             )
             if not search_result:
                 search_result = TVDBSearchResult(search=name)
```

### Comparing `FlexGet-3.6.2/flexget/components/thetvdb/thetvdb_lookup.py` & `FlexGet-3.6.3/flexget/components/thetvdb/thetvdb_lookup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from loguru import logger
 
-from flexget import entry, plugin
+from flexget import plugin
+from flexget.entry import register_lazy_lookup
 from flexget.event import event
 from flexget.utils.database import with_session
 
 try:
     # NOTE: Importing other plugins is discouraged!
     from flexget.components.thetvdb import api_tvdb as plugin_api_tvdb
 except ImportError:
@@ -59,15 +60,15 @@
         'tvdb_series_name': 'name',
         'tvdb_rating': 'rating',
         'tvdb_status': 'status',
         'tvdb_runtime': 'runtime',
         'tvdb_first_air_date': 'first_aired',
         'tvdb_air_time': 'airs_time',
         'tvdb_content_rating': 'content_rating',
-        'tvdb_genres': lambda series: [g for g in series.genres],
+        'tvdb_genres': lambda series: list(series.genres),
         'tvdb_network': 'network',
         'tvdb_overview': 'overview',
         'tvdb_banner': 'banner',
         'tvdb_language': 'language',
         'tvdb_airs_day_of_week': 'airs_dayofweek',
         'imdb_url': lambda series: series.imdb_id
         and f'http://www.imdb.com/title/{series.imdb_id}',
@@ -113,27 +114,27 @@
             entry.update_using_map(field_map, series)
         except LookupError as e:
             logger.debug(
                 'Error looking up tvdb series information for {}: {}', entry['title'], e.args[0]
             )
         return entry
 
-    @entry.register_lazy_lookup('tvdb_series_lookup')
+    @register_lazy_lookup('tvdb_series_lookup')
     def lazy_series_lookup(self, entry, language):
         return self.series_lookup(entry, language, self.series_map)
 
-    @entry.register_lazy_lookup('tvdb_series_actor_lookup')
+    @register_lazy_lookup('tvdb_series_actor_lookup')
     def lazy_series_actor_lookup(self, entry, language):
         return self.series_lookup(entry, language, self.series_actor_map)
 
-    @entry.register_lazy_lookup('tvdb_series_poster_lookup')
+    @register_lazy_lookup('tvdb_series_poster_lookup')
     def lazy_series_poster_lookup(self, entry, language):
         return self.series_lookup(entry, language, self.series_poster_map)
 
-    @entry.register_lazy_lookup('tvdb_episode_lookup')
+    @register_lazy_lookup('tvdb_episode_lookup')
     def lazy_episode_lookup(self, entry, language):
         try:
             season_offset = entry.get('thetvdb_lookup_season_offset', 0)
             episode_offset = entry.get('thetvdb_lookup_episode_offset', 0)
             if not isinstance(season_offset, int):
                 logger.error('thetvdb_lookup_season_offset must be an integer')
                 season_offset = 0
```

### Comparing `FlexGet-3.6.2/flexget/components/tmdb/api.py` & `FlexGet-3.6.3/flexget/components/tmdb/api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/tmdb/api_tmdb.py` & `FlexGet-3.6.3/flexget/components/tmdb/api_tmdb.py`

 * *Files 0% similar despite different names*

```diff
@@ -199,15 +199,15 @@
             'rating': self.rating,
             'votes': self.votes,
             'popularity': self.popularity,
             'adult': self.adult,
             'budget': self.budget,
             'revenue': self.revenue,
             'homepage': self.homepage,
-            'genres': [g for g in self.genres],
+            'genres': list(self.genres),
             'updated': self.updated,
             'lookup_language': self.lookup_language,
         }
 
 
 class TMDBGenre(Base):
     __tablename__ = 'tmdb_genres'
```

### Comparing `FlexGet-3.6.2/flexget/components/tmdb/tmdb_lookup.py` & `FlexGet-3.6.3/flexget/components/tmdb/tmdb_lookup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from loguru import logger
 
-from flexget import entry, plugin
+from flexget import plugin
+from flexget.entry import register_lazy_lookup
 from flexget.event import event
 from flexget.manager import Session
 from flexget.utils.log import log_once
 
 try:
     # NOTE: Importing other plugins is discouraged!
     from flexget.components.imdb.utils import extract_id
@@ -51,15 +52,15 @@
     schema = {
         'oneOf': [
             {'type': 'boolean'},
             {'type': 'object', 'properties': {'language': {'type': 'string', 'default': 'en'}}},
         ]
     }
 
-    @entry.register_lazy_lookup('tmdb_lookup')
+    @register_lazy_lookup('tmdb_lookup')
     def lazy_loader(self, entry, language):
         """Does the lookup for this entry and populates the entry fields."""
         lookup = plugin.get('api_tmdb', self).lookup
 
         imdb_id = entry.get('imdb_id', eval_lazy=False) or extract_id(
             entry.get('imdb_url', eval_lazy=False)
         )
```

### Comparing `FlexGet-3.6.2/flexget/components/trakt/api.py` & `FlexGet-3.6.3/flexget/components/trakt/api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/trakt/api_trakt.py` & `FlexGet-3.6.3/flexget/components/trakt/api_trakt.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/trakt/cli.py` & `FlexGet-3.6.3/flexget/components/trakt/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,15 +115,15 @@
         'they will automatically refresh when expired)',
         parents=[table_parser],
     )
     show_parser.add_argument('account', metavar='<account>', nargs='?', help=acc_text)
 
     refresh_parser = subparsers.add_parser(
         'refresh',
-        help='Manually refresh your access token associated with your' ' --account <name>',
+        help='Manually refresh your access token associated with your --account <name>',
     )
     refresh_parser.add_argument('account', metavar='<account>', help=acc_text)
 
     delete_parser = subparsers.add_parser(
         'delete', help='Delete the specified <account> name from local database'
     )
     delete_parser.add_argument('account', metavar='<account>', help=acc_text)
```

### Comparing `FlexGet-3.6.2/flexget/components/trakt/db.py` & `FlexGet-3.6.3/flexget/components/trakt/db.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/trakt/next_trakt_episodes.py` & `FlexGet-3.6.3/flexget/components/trakt/next_trakt_episodes.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/trakt/trakt_calendar.py` & `FlexGet-3.6.3/flexget/components/trakt/trakt_calendar.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import datetime
-import math
 
 from loguru import logger
 from requests import RequestException
 
 from flexget import plugin
 from flexget.entry import Entry
 from flexget.event import event
```

### Comparing `FlexGet-3.6.2/flexget/components/trakt/trakt_list.py` & `FlexGet-3.6.3/flexget/components/trakt/trakt_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/trakt/trakt_lookup.py` & `FlexGet-3.6.3/flexget/components/trakt/trakt_lookup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,55 +1,56 @@
 from typing import Optional
 
 from loguru import logger
 
-from flexget import entry, plugin
+from flexget import plugin
+from flexget.entry import Entry, register_lazy_lookup
 from flexget.event import event
 from flexget.manager import Session
 
 from . import api_trakt as plugin_api_trakt
 from . import db
 
 # TODO: not very nice ..
 lookup_series = plugin_api_trakt.ApiTrakt.lookup_series
 lookup_movie = plugin_api_trakt.ApiTrakt.lookup_movie
 
 
 logger = logger.bind(name='trakt_lookup')
 
 
-def is_show(entry: entry.Entry) -> bool:
+def is_show(entry: Entry) -> bool:
     return entry.get('series_name') or entry.get('tvdb_id', eval_lazy=False)
 
 
-def is_episode(entry: entry.Entry) -> bool:
+def is_episode(entry: Entry) -> bool:
     return entry.get('series_season') and entry.get('series_episode')
 
 
-def is_season(entry: entry.Entry) -> bool:
+def is_season(entry: Entry) -> bool:
     return entry.get('series_season') and not is_episode(entry)
 
 
-def is_movie(entry: entry.Entry) -> bool:
+def is_movie(entry: Entry) -> bool:
     return bool(entry.get('movie_name'))
 
 
-def get_media_type_for_entry(entry: entry.Entry) -> Optional[str]:
+def get_media_type_for_entry(entry: Entry) -> Optional[str]:
     if is_episode(entry):
         return 'episode'
     elif is_season(entry):
         return 'season'
     elif is_show(entry):
         return 'show'
     elif is_movie(entry):
         return 'movie'
     return None
 
 
-@entry.register_lazy_lookup('trakt_user_data_lookup')
+@register_lazy_lookup('trakt_user_data_lookup')
 def trakt_user_data_lookup(entry, field_name, data_type, media_type, username, account):
     trakt = plugin_api_trakt.ApiTrakt(username=username, account=account)
     user_data_lookup = trakt.lookup_map[data_type][media_type]
 
     try:
         with Session() as session:
             result = user_data_lookup(get_db_data_for(media_type, entry, session), entry['title'])
@@ -57,15 +58,15 @@
         logger.debug(e)
     else:
         entry[field_name] = result
 
     return entry
 
 
-def _get_lookup_args(entry: entry.Entry) -> dict:
+def _get_lookup_args(entry: Entry) -> dict:
     args = {
         'title': entry.get('series_name', eval_lazy=False) or entry.get('title', eval_lazy=False),
         'year': entry.get('year', eval_lazy=False) or entry.get('movie_year', eval_lazy=False),
         'trakt_slug': (
             entry.get('trakt_show_slug', eval_lazy=False)
             or entry.get('trakt_movie_slug', eval_lazy=False)
         ),
@@ -83,15 +84,15 @@
         args['trakt_id'] = entry['trakt_movie_id']
     elif entry.get('trakt_show_id', eval_lazy=True):
         args['trakt_id'] = entry['trakt_show_id']
 
     return args
 
 
-def get_db_data_for(data_type: str, entry: entry.Entry, session: Session):
+def get_db_data_for(data_type: str, entry: Entry, session: Session):
     if data_type == 'movie':
         movie_lookup_args = _get_lookup_args(entry)
         return lookup_movie(session=session, **movie_lookup_args)
     series_lookup_args = _get_lookup_args(entry)
     show = lookup_series(session=session, **series_lookup_args)
     if data_type == 'show':
         return show
@@ -188,27 +189,27 @@
     'movie_actors': {'trakt_actors': lambda movie: db.list_actors(movie.actors)},
     'movie_translations': {
         'trakt_translations': lambda movie: db.get_translations_dict(movie.translations, 'movie')
     },
 }
 
 
-@entry.register_lazy_lookup('trakt_lazy_lookup')
+@register_lazy_lookup('trakt_lazy_lookup')
 def lazy_lookup(entry, lazy_lookup_name, media_type):
     with Session() as session:
         try:
             db_data = get_db_data_for(media_type, entry, session)
         except LookupError as e:
             logger.debug(e)
         else:
             entry.update_using_map(lazy_lookup_types[lazy_lookup_name], db_data)
     return entry
 
 
-def add_lazy_fields(entry: entry.Entry, lazy_lookup_name: str, media_type: str) -> None:
+def add_lazy_fields(entry: Entry, lazy_lookup_name: str, media_type: str) -> None:
     """
     Adds lazy fields for one of the lookups in our `lazy_lookup_types` dict.
 
     :param entry: The entry to add lazy fields to.
     :param lazy_lookup_name: One of the keys in `lazy_lookup_types` dict.
     :param media_type: show/season/episode/movie (the type of db data needed for this lazy lookup)
     """
@@ -226,15 +227,15 @@
         'episode': 'trakt_ep_user_rating',
         'movie': 'trakt_movie_user_rating',
     },
 }
 
 
 def add_lazy_user_fields(
-    entry: entry.Entry, data_type: str, media_type: str, username: str, account: str
+    entry: Entry, data_type: str, media_type: str, username: str, account: str
 ) -> None:
     """
     Adds one of the user field lazy lookups to an entry.
 
     :param entry: Entry to add lazy fields to
     :param data_type: ratings/collected/watched (one of the keys in `user_data_fields` dict.)
     :param media_type: show/season/episode/movie
@@ -318,15 +319,15 @@
     # Run after series and metainfo series
     @plugin.priority(110)
     def on_task_metainfo(self, task, config):
         if not config:
             return
 
         if isinstance(config, bool):
-            config = dict()
+            config = {}
 
         for entry in task.entries:
             if is_show(entry):
                 add_lazy_fields(entry, 'show', media_type='show')
                 add_lazy_fields(entry, 'show_actors', media_type='show')
                 add_lazy_fields(entry, 'show_translations', media_type='show')
                 if is_episode(entry):
```

### Comparing `FlexGet-3.6.2/flexget/components/tvmaze/api.py` & `FlexGet-3.6.3/flexget/components/tvmaze/api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/tvmaze/api_tvmaze.py` & `FlexGet-3.6.3/flexget/components/tvmaze/api_tvmaze.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/tvmaze/tvmaze_lookup.py` & `FlexGet-3.6.3/flexget/components/tvmaze/tvmaze_lookup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from loguru import logger
 
-from flexget import entry, plugin
+from flexget import plugin
+from flexget.entry import register_lazy_lookup
 from flexget.event import event
 from flexget.manager import Session
 
 logger = logger.bind(name='tvmaze_lookup')
 
 
 class PluginTVMazeLookup:
@@ -117,15 +118,15 @@
         'tvmaze_episode_medium_image': 'medium_image',
         'tvmaze_episode_airstamp': 'airstamp',
         'tvmaze_episode_runtime': 'runtime',
     }
 
     schema = {'type': 'boolean'}
 
-    @entry.register_lazy_lookup('tvmaze_series_lookup')
+    @register_lazy_lookup('tvmaze_series_lookup')
     def lazy_series_lookup(self, entry):
         """Does the lookup for this entry and populates the entry fields."""
         series_lookup = plugin.get('api_tvmaze', self).series_lookup
         with Session() as session:
             lookupargs = {
                 'title': entry.get('series_name', eval_lazy=False),
                 'year': entry.get('year', eval_lazy=False),
@@ -138,15 +139,15 @@
                 series = series_lookup(**lookupargs)
             except LookupError as e:
                 logger.debug(e)
             else:
                 entry.update_using_map(self.series_map, series)
         return entry
 
-    @entry.register_lazy_lookup('tvmaze_season_lookup')
+    @register_lazy_lookup('tvmaze_season_lookup')
     def lazy_season_lookup(self, entry):
         season_lookup = plugin.get('api_tvmaze', self).season_lookup
         with Session(expire_on_commit=False) as session:
             lookupargs = {
                 'title': entry.get('series_name', eval_lazy=False),
                 'year': entry.get('year', eval_lazy=False),
                 'tvmaze_id': entry.get('tvmaze_id', eval_lazy=False),
@@ -159,15 +160,15 @@
                 season = season_lookup(**lookupargs)
             except LookupError as e:
                 logger.debug(e)
             else:
                 entry.update_using_map(self.season_map, season)
         return entry
 
-    @entry.register_lazy_lookup('tvmaze_episode_lookup')
+    @register_lazy_lookup('tvmaze_episode_lookup')
     def lazy_episode_lookup(self, entry):
         episode_lookup = plugin.get('api_tvmaze', self).episode_lookup
         with Session(expire_on_commit=False) as session:
             lookupargs = {
                 'title': entry.get('series_name', eval_lazy=False),
                 'year': entry.get('year', eval_lazy=False),
                 'tvmaze_id': entry.get('tvmaze_id', eval_lazy=False),
```

### Comparing `FlexGet-3.6.2/flexget/components/variables/api.py` & `FlexGet-3.6.3/flexget/components/variables/api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/components/variables/variables.py` & `FlexGet-3.6.3/flexget/components/variables/variables.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,15 @@
 def _process(element, environment):
     if isinstance(element, dict):
         for k, v in list(element.items()):
             new_key = _process(k, environment)
             if new_key:
                 element[new_key] = element.pop(k)
                 k = new_key
-            val = _process(element[k], environment)
+            val = _process(v, environment)
             if val:
                 element[k] = val
     elif isinstance(element, list):
         for i, v in enumerate(element):
             val = _process(v, environment)
             if val:
                 element[i] = val
```

### Comparing `FlexGet-3.6.2/flexget/config_schema.py` & `FlexGet-3.6.3/flexget/config_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -323,16 +323,16 @@
 
 @format_checker.checks('json', raises=ValueError)
 def is_json(instance) -> bool:
     if not isinstance(instance, str):
         return False
 
     try:
-        decoded_json = json_loads(instance)
-    except JSONDecodeError as e:
+        json_loads(instance)
+    except JSONDecodeError:
         raise ValueError('`%s` is not a valid json' % instance)
 
     return True
 
 
 def set_error_message(error: jsonschema.ValidationError) -> None:
     """
```

### Comparing `FlexGet-3.6.2/flexget/db_schema.py` & `FlexGet-3.6.3/flexget/db_schema.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/entry.py` & `FlexGet-3.6.3/flexget/entry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import functools
 import types
 import warnings
 from enum import Enum
-from typing import Callable, Dict, Iterable, Mapping, Optional, Sequence, Union
+from typing import Callable, Iterable, Mapping, Optional, Sequence, Union
 
 from loguru import logger
 
 from flexget import plugin
 from flexget.utils.lazy_dict import LazyDict, LazyLookup
 from flexget.utils.serialization import Serializer, deserialize, serialize
 from flexget.utils.template import FlexGetTemplate, render_from_entry
```

### Comparing `FlexGet-3.6.2/flexget/event.py` & `FlexGet-3.6.3/flexget/event.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ipc.py` & `FlexGet-3.6.3/flexget/ipc.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/log.py` & `FlexGet-3.6.3/flexget/log.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,18 +9,15 @@
 import uuid
 import warnings
 from typing import Callable, Deque, Iterator, List, Optional, Union
 
 import loguru
 from loguru import logger
 
-import flexget
 from flexget import __version__
-from flexget.event import event
-from flexget.utils.tools import io_encoding
 
 # A level more detailed than INFO
 VERBOSE = 15
 # environment variables to modify rotating log parameters from defaults of 1 MB and 9 files
 ENV_MAXBYTES = 'FLEXGET_LOG_MAXBYTES'
 ENV_MAXCOUNT = 'FLEXGET_LOG_MAXCOUNT'
```

### Comparing `FlexGet-3.6.2/flexget/manager.py` & `FlexGet-3.6.3/flexget/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-import argparse  # noqa
-import atexit  # noqa
-import codecs  # noqa
+import argparse
+import atexit
+import codecs
 import collections
-import copy  # noqa
-import errno  # noqa
-import fnmatch  # noqa
-import hashlib  # noqa
-import os  # noqa
-import shutil  # noqa
-import signal  # noqa
-import sys  # noqa
-import threading  # noqa
-import traceback  # noqa
-from contextlib import contextmanager  # noqa
-from datetime import datetime, timedelta  # noqa
-from typing import (  # noqa
+import copy
+import errno
+import fnmatch
+import hashlib
+import os
+import shutil
+import signal
+import sys
+import threading
+import traceback
+from contextlib import contextmanager
+from datetime import datetime, timedelta
+from typing import (
     TYPE_CHECKING,
     Dict,
     Iterator,
     List,
     Optional,
     Sequence,
     Tuple,
     Type,
     Union,
 )
 
-import sqlalchemy  # noqa
-import yaml  # noqa
-from loguru import logger  # noqa
+import sqlalchemy
+import yaml
+from loguru import logger
 from sqlalchemy.engine import Engine
-from sqlalchemy.exc import OperationalError  # noqa
-from sqlalchemy.ext.declarative import declarative_base  # noqa
-from sqlalchemy.orm import sessionmaker  # noqa
+from sqlalchemy.exc import OperationalError
+from sqlalchemy.ext.declarative import declarative_base
+from sqlalchemy.orm import sessionmaker
 
 # These need to be declared before we start importing from other flexget modules, since they might import them
 from flexget.config_schema import ConfigError
-from flexget.utils.sqlalchemy_utils import ContextSession  # noqa
-from flexget.utils.tools import get_current_flexget_version, io_encoding, pid_exists  # noqa
+from flexget.utils.sqlalchemy_utils import ContextSession
+from flexget.utils.tools import get_current_flexget_version, io_encoding, pid_exists
 
 Base = declarative_base()
 Session: Type[ContextSession] = sessionmaker(class_=ContextSession)
 
 import flexget.log  # noqa
 from flexget import config_schema, db_schema, plugin  # noqa
 from flexget.event import fire_event  # noqa
@@ -473,15 +473,15 @@
                 self.ipc_server.start()
                 self.task_queue.wait()
                 fire_event('manager.daemon.completed', self)
                 if tray_icon:
                     tray_icon.stop()
 
             if options.tray_icon:
-                from flexget.tray_icon import tray_icon  # noqa
+                from flexget.tray_icon import tray_icon
 
                 self._add_tray_icon_items(tray_icon)
 
                 # Tray icon must be run in the main thread.
                 m = threading.Thread(target=run_daemon, args=(tray_icon,))
                 m.start()
                 tray_icon.run()
@@ -521,17 +521,17 @@
         self.shutdown(finish_queue=False)
 
     def setup_yaml(self) -> None:
         """Customize the yaml loader/dumper behavior"""
 
         # Represent OrderedDict as a regular dict (but don't sort it alphabetically)
         # This lets us order a dict in a yaml file for easier human consumption
-        represent_dict_order = lambda self, data: self.represent_mapping(
-            'tag:yaml.org,2002:map', data.items()
-        )
+        def represent_dict_order(self, data):
+            return self.represent_mapping('tag:yaml.org,2002:map', data.items())
+
         yaml.add_representer(collections.OrderedDict, represent_dict_order)
 
         # Set up the dumper to increase the indent for lists
         def increase_indent_wrapper(func):
             def increase_indent(self, flow=False, indentless=False):
                 func(self, flow, False)
```

### Comparing `FlexGet-3.6.2/flexget/options.py` & `FlexGet-3.6.3/flexget/options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,23 @@
 import copy
 import random
 import string
 import sys
-from argparse import _UNRECOGNIZED_ARGS_ATTR, PARSER, REMAINDER, SUPPRESS, Action, ArgumentError
+from argparse import (
+    _UNRECOGNIZED_ARGS_ATTR,
+    PARSER,
+    REMAINDER,
+    SUPPRESS,
+    Action,
+    ArgumentError,
+    Namespace,
+    _SubParsersAction,
+    _VersionAction,
+)
 from argparse import ArgumentParser as ArgParser
-from argparse import Namespace, _SubParsersAction, _VersionAction
 from typing import IO, Any, Callable, List, Optional, TextIO
 
 import flexget
 from flexget.entry import Entry
 from flexget.event import fire_event
 from flexget.utils.tools import get_current_flexget_version, get_latest_flexget_version_number
 
@@ -123,15 +132,15 @@
             )
         if 'force' in [v.lower() for v in values]:
             kwargs['immortal'] = True
         entry = Entry(**kwargs)
         if 'accept' in [v.lower() for v in values]:
             entry.accept(reason='accepted by --inject')
         existing = getattr(namespace, self.dest, None) or []
-        setattr(namespace, self.dest, existing + [entry])
+        setattr(namespace, self.dest, [*existing, entry])
 
 
 class ParseExtrasAction(Action):
     """This action will take extra arguments, and parser them with a different parser."""
 
     def __init__(self, option_strings, parser, help=None, metavar=None, dest=None, required=False):
         if metavar is None:
@@ -585,9 +594,9 @@
         # Make sure we always have execute parser settings even when other commands called
         if not result.cli_command == 'execute':
             exec_options = get_parser('execute').parse_args([])
             if hasattr(result, 'execute'):
                 exec_options.__dict__.update(result.execute.__dict__)
             result.execute = exec_options
         # Set the 'allow_manual' flag to True for any usage of the CLI
-        setattr(result, 'allow_manual', True)
+        result.allow_manual = True
         return result
```

### Comparing `FlexGet-3.6.2/flexget/plugin.py` & `FlexGet-3.6.3/flexget/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,17 +11,16 @@
 import loguru
 import pkg_resources
 from requests import RequestException
 
 from flexget import components as components_pkg
 from flexget import config_schema
 from flexget import plugins as plugins_pkg
-from flexget.event import Event
+from flexget.event import Event, event, fire_event, remove_event_handlers
 from flexget.event import add_event_handler as add_phase_handler
-from flexget.event import event, fire_event, remove_event_handlers
 
 logger = loguru.logger.bind(name='plugin')
 
 PRIORITY_DEFAULT = 128
 PRIORITY_LAST = -255
 PRIORITY_FIRST = 255
 
@@ -459,15 +458,15 @@
             if plugin_path.name == '__init__.py':
                 continue
             # Split the relative path from the plugins dir to current file's parent dir to find subpackage names
             plugin_subpackages = [
                 _f for _f in plugin_path.relative_to(plugins_dir).parent.parts if _f
             ]
             module_name = '.'.join(
-                [plugins_pkg.__name__] + plugin_subpackages + [plugin_path.stem]
+                [plugins_pkg.__name__, *plugin_subpackages] + [plugin_path.stem]
             )
             _import_plugin(module_name, plugin_path)
     _check_phase_queue()
 
 
 # TODO: this is now identical to _load_plugins_from_dirs, REMOVE
 def _load_components_from_dirs(dirs: List[str]) -> None:
@@ -481,15 +480,15 @@
             if component_path.name == '__init__.py':
                 continue
             # Split the relative path from the plugins dir to current file's parent dir to find subpackage names
             plugin_subpackages = [
                 _f for _f in component_path.relative_to(component_dir).parent.parts if _f
             ]
             package_name = '.'.join(
-                [components_pkg.__name__] + plugin_subpackages + [component_path.stem]
+                [components_pkg.__name__, *plugin_subpackages] + [component_path.stem]
             )
             _import_plugin(package_name, component_path)
     _check_phase_queue()
 
 
 def _load_plugins_from_packages() -> None:
     """Load plugins installed via PIP"""
```

### Comparing `FlexGet-3.6.2/flexget/plugins/cli/check.py` & `FlexGet-3.6.3/flexget/plugins/cli/check.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/cli/cli_config.py` & `FlexGet-3.6.3/flexget/plugins/cli/cli_config.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/cli/database.py` & `FlexGet-3.6.3/flexget/plugins/cli/database.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/cli/debug_info.py` & `FlexGet-3.6.3/flexget/plugins/cli/debug_info.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/cli/doc.py` & `FlexGet-3.6.3/flexget/plugins/cli/doc.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/cli/explain_sql.py` & `FlexGet-3.6.3/flexget/plugins/cli/explain_sql.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/cli/filters.py` & `FlexGet-3.6.3/flexget/plugins/cli/filters.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from flexget.utils.template import get_filters
 
 
 def do_cli(manager, options):
     header = ['Name', 'Description']
     table = TerminalTable(*header, table_type=options.table_type, show_lines=True)
     for filter_name, filter in get_filters().items():
-        if options.name and not options.name in filter_name:
+        if options.name and options.name not in filter_name:
             continue
         filter_doc = inspect.getdoc(filter) or ''
         table.add_row(filter_name, filter_doc)
     console(table)
 
 
 @event('options.register')
```

### Comparing `FlexGet-3.6.2/flexget/plugins/cli/inject.py` & `FlexGet-3.6.3/flexget/plugins/cli/inject.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/cli/perf_tests.py` & `FlexGet-3.6.3/flexget/plugins/cli/perf_tests.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/cli/performance.py` & `FlexGet-3.6.3/flexget/plugins/cli/performance.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/cli/plugins.py` & `FlexGet-3.6.3/flexget/plugins/cli/plugins.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/cli/templates.py` & `FlexGet-3.6.3/flexget/plugins/cli/templates.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         'Use with',
         TerminalTable.Column('Full Path', overflow='fold'),
         TerminalTable.Column('Contents', overflow='ignore'),
     ]
     table = TerminalTable(*header, table_type=options.table_type, show_lines=True)
     console('Fetching all file templates, stand by...')
     for template_name in list_templates(extensions=['template']):
-        if options.name and not options.name in template_name:
+        if options.name and options.name not in template_name:
             continue
         template = get_template(template_name)
         if 'entries' in template_name:
             plugin = 'notify_entries'
         elif 'task' in template_name:
             plugin = 'notify_task'
         else:
```

### Comparing `FlexGet-3.6.2/flexget/plugins/cli/try_regexp.py` & `FlexGet-3.6.3/flexget/plugins/cli/try_regexp.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/cli/web.py` & `FlexGet-3.6.3/flexget/plugins/cli/web.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/cli/wiki_qualities.py` & `FlexGet-3.6.3/flexget/plugins/cli/wiki_qualities.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,13 +19,13 @@
         table.add_row(*[str(i) for i in row])
     console(table)
 
 
 @event('options.register')
 def register_parser_arguments():
     # Register subcommand
-    parser = options.register_command(
+    options.register_command(
         'wiki-qualities',
         do_cli,
         # If we don't specify the help argument, this won't show up in --help, which is good because it's not for users
         # help='Generate the list of qualities for exporting to the wiki.',
     )
```

### Comparing `FlexGet-3.6.2/flexget/plugins/cli/win32_service.py` & `FlexGet-3.6.3/flexget/plugins/cli/win32_service.py`

 * *Files 5% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 
     argv = options.args
     if options.help:
         argv = []
 
     # Hack sys.argv a bit so that we get a better usage message
     sys.argv[0] = 'flexget service'
-    win32serviceutil.HandleCommandLine(AppServerSvc, argv=['flexget service'] + argv)
+    win32serviceutil.HandleCommandLine(AppServerSvc, argv=['flexget service', *argv])
 
 
 @event('options.register')
 def register_parser_arguments():
     if not sys.platform.startswith('win'):
         return
     # Still not fully working. Hidden for now.
```

### Comparing `FlexGet-3.6.2/flexget/plugins/clients/aria2.py` & `FlexGet-3.6.3/flexget/plugins/clients/aria2.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import json
 import os
 import re
 import ssl
 import xmlrpc.client
-from socket import error as socket_error
 
 import requests
 from loguru import logger
 
 from flexget import plugin
 from flexget.event import event
+from flexget.plugin import PluginError
 from flexget.utils.template import RenderError
 
 logger = logger.bind(name='aria2')
 
 
 class RpcClient:
     def __init__(self, server, port, scheme, rpc_path, username, password, secret):
@@ -81,15 +81,14 @@
 
     def add_uri(self, uris, options):
         # https://aria2.github.io/manual/en/html/aria2c.html#aria2.addUri
         return self._post(JsonRpcClient.ADDURI_METHOD, params=[[uris], options])
 
     def add_torrent(self, torrent, options):
         # https://aria2.github.io/manual/en/html/aria2c.html#aria2.addTorrent
-        params = [torrent]
         return self._post(JsonRpcClient.ADDTORRENT_METHOD, params=[torrent, options])
 
     def get_global_stat(self):
         # https://aria2.github.io/manual/en/html/aria2c.html#aria2.getGlobalStat
         return self._post(JsonRpcClient.GETGLOBALSTAT_METHOD, params=[])
 
 
@@ -97,35 +96,35 @@
     def __init__(self, server, port, scheme, rpc_path, username=None, password=None, secret=None):
         schemes = {'http': None, 'https': ssl.SSLContext()}
         if scheme not in schemes:
             raise plugin.PluginError('Unknown scheme: %s' % (scheme), logger)
         super().__init__(server, port, scheme, rpc_path, username, password, secret)
         try:
             self._aria2 = xmlrpc.client.ServerProxy(self.url, context=schemes[scheme]).aria2
-        except xmlrpc.client.ProtocolError as err:
+        except xmlrpc.client.ProtocolError as exc:
             raise plugin.PluginError(
                 'Could not connect to aria2 at %s. Protocol error %s: %s'
-                % (self.url, err.errcode, err.errmsg),
+                % (self.url, exc.errcode, exc.errmsg),
                 logger,
-            )
-        except xmlrpc.client.Fault as err:
+            ) from exc
+        except xmlrpc.client.Fault as exc:
             raise plugin.PluginError(
                 'XML-RPC fault: Unable to connect to aria2 daemon at %s: %s'
-                % (self.url, err.faultString),
+                % (self.url, exc.faultString),
                 logger,
-            )
-        except socket_error as e:
+            ) from exc
+        except OSError as exc:
             raise plugin.PluginError(
-                f'Socket connection issue with aria2 daemon at {self.url}: {e}', logger
-            )
-        except:
+                f'Socket connection issue with aria2 daemon at {self.url}: {exc}', logger
+            ) from exc
+        except Exception as exc:
             logger.opt(exception=True).debug('Unexpected error during aria2 connection')
             raise plugin.PluginError(
                 'Unidentified error during connection to aria2 daemon', logger
-            )
+            ) from exc
 
     def add_uri(self, uris, options):
         # https://aria2.github.io/manual/en/html/aria2c.html#aria2.addUri
         params = [[uris]]
         if options:
             params.append(options)
         if self.token:
@@ -138,14 +137,17 @@
         if options:
             params.append(options)
         if self.token:
             params.insert(0, self.token)
         return self._aria2.addTorrent(*params)
 
 
+RPC_CLIENTS = {'xml': XmlRpcClient, 'json': JsonRpcClient}
+
+
 class OutputAria2:
     """
     Simple Aria2 output
 
     Example::
 
         aria2:
@@ -160,15 +162,15 @@
             'port': {'type': 'integer', 'default': 6800},
             'secret': {'type': 'string', 'default': ''},
             # NOTE: To be deprecated by aria2
             'username': {'type': 'string', 'default': ''},
             'password': {'type': 'string', 'default': ''},
             'scheme': {'type': 'string', 'default': 'http'},
             # NOTE: xml/json
-            'rpc_mode': {'type': 'string', 'default': 'xml'},
+            'rpc_mode': {'type': 'string', 'default': 'xml', 'enum': list(RPC_CLIENTS)},
             'rpc_path': {'type': 'string', 'default': 'rpc'},
             'path': {'type': 'string'},
             'filename': {'type': 'string'},
             'add_extension': {
                 'oneOf': [
                     {'type': 'string'},
                     {'type': 'boolean'},
@@ -206,18 +208,17 @@
         return config
 
     def on_task_output(self, task, config):
         # don't add when learning
         if task.options.learn:
             return
         config = self.prepare_config(config)
-        rpc_clients = {'xml': XmlRpcClient, 'json': JsonRpcClient}
-        if config['rpc_mode'] not in rpc_clients:
-            entry.fail('Unknown rpc_mode: %s' % config['rpc_mode'])
-        aria2 = rpc_clients[config['rpc_mode']](
+        if config['rpc_mode'] not in RPC_CLIENTS:
+            raise PluginError(f'Unknown rpc_mode: {config["rpc_mode"]}')
+        aria2 = RPC_CLIENTS[config['rpc_mode']](
             config['server'],
             config['port'],
             config['scheme'],
             config['rpc_path'],
             config['username'],
             config['password'],
             config['secret'],
@@ -225,15 +226,15 @@
 
         for entry in task.accepted:
             if task.options.test:
                 logger.verbose('Would add `{}` to aria2.', entry['title'])
                 continue
             try:
                 self.add_entry(aria2, entry, config, task)
-            except socket_error as se:
+            except OSError as se:
                 entry.fail('Unable to reach Aria2: %s' % se)
             except xmlrpc.client.Fault as err:
                 logger.critical('Fault code {} message {}', err.faultCode, err.faultString)
                 entry.fail('Aria2 communication Fault')
             except Exception as e:
                 logger.opt(exception=True).debug('Exception type {}', type(e))
                 raise
@@ -260,15 +261,15 @@
                     logger.debug('Getting filename from `{}`', entry['url'])
                     content_disposition = None
                     try:
                         with task.requests.get(
                             entry['url'], headers=None, stream=True
                         ) as response:
                             content_disposition = response.headers.get('content-disposition', None)
-                    except Exception as e:
+                    except Exception:
                         logger.warning('Not possible to retrive file info from `{}`', entry['url'])
                         entry.fail('Not possible to retrive file info from `%s`' % entry['url'])
                         return
 
                     if content_disposition:
                         fname_match = re.findall(
                             r'filename=["\']?([^"\']+)["\']?', content_disposition
```

### Comparing `FlexGet-3.6.2/flexget/plugins/clients/deluge.py` & `FlexGet-3.6.3/flexget/plugins/clients/deluge.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/clients/nzbget.py` & `FlexGet-3.6.3/flexget/plugins/clients/nzbget.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/clients/pyload.py` & `FlexGet-3.6.3/flexget/plugins/clients/pyload.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/clients/qbittorrent.py` & `FlexGet-3.6.3/flexget/plugins/clients/qbittorrent.py`

 * *Files 0% similar despite different names*

```diff
@@ -145,15 +145,15 @@
         try:
             respose = self.session.request(
                 'get',
                 url,
                 params=params,
                 verify=verify_cert,
             )
-        except RequestException as e:
+        except RequestException:
             logger.error('Error getting torrent info, request to hash {} failed', hash_torrent)
             return False
 
         if respose.status_code != 200:
             logger.error(
                 'Error getting torrent info, hash {} search returned',
                 hash_torrent,
```

### Comparing `FlexGet-3.6.2/flexget/plugins/clients/rtorrent.py` & `FlexGet-3.6.3/flexget/plugins/clients/rtorrent.py`

 * *Files 1% similar despite different names*

```diff
@@ -301,15 +301,15 @@
 
         for field in fields:
             method_name = 'd.%s' % field
             getattr(multi_call, method_name)(info_hash)
 
         resp = multi_call()
         # TODO: Maybe we should return a named tuple or a Torrent class?
-        return dict(list(zip(self._clean_fields(fields, reverse=True), [val for val in resp])))
+        return dict(list(zip(self._clean_fields(fields, reverse=True), list(resp))))
 
     def torrents(self, view='main', fields=None):
         if not fields:
             fields = list(self.default_fields)
         fields = self._clean_fields(fields)
 
         params = ['d.%s=' % field for field in fields]
```

### Comparing `FlexGet-3.6.2/flexget/plugins/clients/transmission.py` & `FlexGet-3.6.3/flexget/plugins/clients/transmission.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,23 +91,23 @@
                 host=urlo.hostname,
                 port=port,
                 path=path,
                 username=user,
                 password=password,
                 timeout=30,
             )
-        except TransmissionAuthError as e:
+        except TransmissionAuthError:
             raise plugin.PluginError(
                 "Username/password for transmission is incorrect. Cannot connect."
             )
-        except TransmissionTimeoutError as e:
+        except TransmissionTimeoutError:
             raise plugin.PluginError("Cannot connect to transmission: Connection timed out.")
         except TransmissionConnectError as e:
             raise plugin.PluginError("Error connecting to transmission: %s" % e.args[0].reason)
-        except TransmissionError as e:
+        except TransmissionError:
             raise plugin.PluginError("Error connecting to transmission")
         return cli
 
     def torrent_info(self, torrent: 'Torrent', config):
         done = torrent.total_size > 0
         vloc = None
         best = None
```

### Comparing `FlexGet-3.6.2/flexget/plugins/daemon/web_server.py` & `FlexGet-3.6.3/flexget/plugins/daemon/web_server.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/filter/abort_if_exists.py` & `FlexGet-3.6.3/flexget/plugins/filter/abort_if_exists.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/filter/accept_all.py` & `FlexGet-3.6.3/flexget/plugins/filter/accept_all.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/filter/age.py` & `FlexGet-3.6.3/flexget/plugins/filter/age.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/filter/best_quality.py` & `FlexGet-3.6.3/flexget/plugins/filter/best_quality.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/filter/content_filter.py` & `FlexGet-3.6.3/flexget/plugins/filter/content_filter.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/filter/content_size.py` & `FlexGet-3.6.3/flexget/plugins/filter/content_size.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/filter/crossmatch.py` & `FlexGet-3.6.3/flexget/plugins/filter/crossmatch.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/filter/delay.py` & `FlexGet-3.6.3/flexget/plugins/filter/delay.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/filter/duplicates.py` & `FlexGet-3.6.3/flexget/plugins/filter/duplicates.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/filter/exists.py` & `FlexGet-3.6.3/flexget/plugins/filter/exists.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/filter/exists_movie.py` & `FlexGet-3.6.3/flexget/plugins/filter/exists_movie.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/filter/exists_series.py` & `FlexGet-3.6.3/flexget/plugins/filter/exists_series.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/filter/if_condition.py` & `FlexGet-3.6.3/flexget/plugins/filter/if_condition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import datetime
 from copy import copy
 
 from jinja2 import UndefinedError
 from loguru import logger
 
 from flexget import plugin
 from flexget.entry import Entry
```

### Comparing `FlexGet-3.6.2/flexget/plugins/filter/limit_new.py` & `FlexGet-3.6.3/flexget/plugins/filter/limit_new.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/filter/magnets.py` & `FlexGet-3.6.3/flexget/plugins/filter/magnets.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/filter/only_new.py` & `FlexGet-3.6.3/flexget/plugins/filter/only_new.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/filter/proper_movies.py` & `FlexGet-3.6.3/flexget/plugins/filter/proper_movies.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/filter/quality.py` & `FlexGet-3.6.3/flexget/plugins/filter/quality.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/filter/regexp.py` & `FlexGet-3.6.3/flexget/plugins/filter/regexp.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/filter/require_field.py` & `FlexGet-3.6.3/flexget/plugins/filter/require_field.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/filter/rottentomatoes.py` & `FlexGet-3.6.3/flexget/plugins/filter/rottentomatoes.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/filter/thetvdb.py` & `FlexGet-3.6.3/flexget/plugins/filter/thetvdb.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/filter/timeframe.py` & `FlexGet-3.6.3/flexget/plugins/filter/timeframe.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/filter/unique.py` & `FlexGet-3.6.3/flexget/plugins/filter/unique.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/filter/upgrade.py` & `FlexGet-3.6.3/flexget/plugins/filter/upgrade.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/generic/cron_env.py` & `FlexGet-3.6.3/flexget/plugins/generic/cron_env.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/generic/db_vacuum.py` & `FlexGet-3.6.3/flexget/plugins/generic/db_vacuum.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/generic/log_start.py` & `FlexGet-3.6.3/flexget/plugins/generic/log_start.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/generic/urlfix.py` & `FlexGet-3.6.3/flexget/plugins/generic/urlfix.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/generic/welcome.py` & `FlexGet-3.6.3/flexget/plugins/generic/welcome.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/input/anidb_list.py` & `FlexGet-3.6.3/flexget/plugins/input/anidb_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/input/anilist.py` & `FlexGet-3.6.3/flexget/plugins/input/anilist.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/input/apple_trailers.py` & `FlexGet-3.6.3/flexget/plugins/input/apple_trailers.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/input/betaseries_list.py` & `FlexGet-3.6.3/flexget/plugins/input/betaseries_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/input/discover.py` & `FlexGet-3.6.3/flexget/plugins/input/discover.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,15 @@
             entry_results = []
             for item in config['from']:
                 if isinstance(item, dict):
                     plugin_name, plugin_config = list(item.items())[0]
                 else:
                     plugin_name, plugin_config = item, None
                 search = plugin.get(plugin_name, self)
-                if not callable(getattr(search, 'search')):
+                if not callable(search.search):
                     logger.critical(
                         'Search plugin {} does not implement search method', plugin_name
                     )
                     continue
                 logger.verbose(
                     'Searching for `{}` with plugin `{}` ({} of {})',
                     entry['title'],
```

### Comparing `FlexGet-3.6.2/flexget/plugins/input/filesystem.py` & `FlexGet-3.6.3/flexget/plugins/input/filesystem.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/input/filmweb_watchlist.py` & `FlexGet-3.6.3/flexget/plugins/input/filmweb_watchlist.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/input/from_piratebay.py` & `FlexGet-3.6.3/flexget/plugins/input/from_piratebay.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/input/from_task.py` & `FlexGet-3.6.3/flexget/plugins/input/from_task.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/input/from_telegram.py` & `FlexGet-3.6.3/flexget/plugins/input/from_telegram.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Plugin for telegram input"""
 import re
 
 from loguru import logger
-from requests.exceptions import HTTPError, RequestException
+from requests.exceptions import HTTPError
 
 from flexget import plugin
 from flexget.config_schema import one_or_more
 from flexget.entry import Entry
 from flexget.event import event
 
 logger = logger.bind(name='from_telegram')
```

### Comparing `FlexGet-3.6.2/flexget/plugins/input/gazelle.py` & `FlexGet-3.6.3/flexget/plugins/input/gazelle.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/input/generate.py` & `FlexGet-3.6.3/flexget/plugins/input/generate.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/input/html.py` & `FlexGet-3.6.3/flexget/plugins/input/html.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/input/input_csv.py` & `FlexGet-3.6.3/flexget/plugins/input/input_csv.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/input/inputs.py` & `FlexGet-3.6.3/flexget/plugins/input/inputs.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/input/json.py` & `FlexGet-3.6.3/flexget/plugins/input/json.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/input/kitsu.py` & `FlexGet-3.6.3/flexget/plugins/input/kitsu.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
                         continue
                     if status == 'finished' and anime['attributes']['endDate'] is None:
                         continue
 
                 types = config.get('type')
                 if types is not None:
                     subType = anime['attributes']['subtype']
-                    if subType is None or not subType.lower() in types:
+                    if subType is None or subType.lower() not in types:
                         continue
 
                 entry = Entry()
                 entry['title'] = anime['attributes']['canonicalTitle']
                 titles_en = anime['attributes']['titles'].get('en')
                 if titles_en:
                     entry['kitsu_title_en'] = titles_en
```

### Comparing `FlexGet-3.6.2/flexget/plugins/input/letterboxd.py` & `FlexGet-3.6.3/flexget/plugins/input/letterboxd.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/input/limit.py` & `FlexGet-3.6.3/flexget/plugins/input/limit.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/input/medusa.py` & `FlexGet-3.6.3/flexget/plugins/input/medusa.py`

 * *Files 5% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         depending on your usage.
         """
         parsed_url = urlparse(config.get('base_url'))
         base_url = '{scheme}://{url}:{port}/api/v2'.format(
             scheme=parsed_url.scheme, url=parsed_url.netloc, port=config.get('port')
         )
 
-        body_auth = dict(username=config.get('username'), password=config.get('password'))
+        body_auth = {'username': config.get('username'), 'password': config.get('password')}
 
         api_key = task.requests.post(f'{base_url}/authenticate', json=body_auth).json()['token']
 
         headers = {'x-auth': 'Bearer ' + api_key}
 
         params = {'limit': 1000}
```

### Comparing `FlexGet-3.6.2/flexget/plugins/input/mock.py` & `FlexGet-3.6.3/flexget/plugins/input/mock.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/input/my_anime_list.py` & `FlexGet-3.6.3/flexget/plugins/input/my_anime_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/input/myepisodes_list.py` & `FlexGet-3.6.3/flexget/plugins/input/myepisodes_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/input/next_sonarr_episodes.py` & `FlexGet-3.6.3/flexget/plugins/input/next_sonarr_episodes.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/input/npo_watchlist.py` & `FlexGet-3.6.3/flexget/plugins/input/npo_watchlist.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,26 +101,26 @@
             login_page = get_soup(login_response.content)
             token = login_page.find('input', attrs={'name': '__RequestVerificationToken'})['value']
             return_url = login_page.find('input', attrs={'name': 'ReturnUrl'})['value']
 
             email = config.get('email')
             password = config.get('password')
 
-            npoid_response = requests.post(
+            requests.post(
                 npoid_login_url,
                 {
                     'button': 'login',
                     '__RequestVerificationToken': token,
                     'ReturnUrl': return_url,
                     'EmailAddress': email,
                     'Password': password,
                 },
             )
 
-            npostart_response = requests.get(npoid_base + return_url)
+            requests.get(npoid_base + return_url)
 
             if 'isAuthenticatedUser' not in requests.cookies:
                 raise plugin.PluginError('Failed to login. Check username and password.')
             logger.debug('Succesfully logged in: {}', email)
         except RequestException as e:
             raise plugin.PluginError('Request error: %s' % str(e))
```

### Comparing `FlexGet-3.6.2/flexget/plugins/input/parameterize.py` & `FlexGet-3.6.3/flexget/plugins/input/parameterize.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/input/plex.py` & `FlexGet-3.6.3/flexget/plugins/input/plex.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,15 +139,15 @@
         try:
             r = requests.get(
                 "https://my.plexapp.com/pms/servers?X-Plex-Token=%s" % globalaccesstoken
             )
         except requests.RequestException as e:
             raise plugin.PluginError(
                 "Could not get servers from my.plexapp.com using "
-                "authentication-token: %s. (%s)" % (globalaccesstoken, e)
+                "authentication-token: {}. ({})".format(globalaccesstoken, e)
             )
         dom = parseString(r.text)
         for node in dom.getElementsByTagName('Server'):
             if config['server'] in (
                 node.getAttribute('address'),
                 node.getAttribute('localAddresses'),
             ):
```

### Comparing `FlexGet-3.6.2/flexget/plugins/input/pogcal.py` & `FlexGet-3.6.3/flexget/plugins/input/pogcal.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/input/regexp_parse.py` & `FlexGet-3.6.3/flexget/plugins/input/regexp_parse.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/input/rlslog.py` & `FlexGet-3.6.3/flexget/plugins/input/rlslog.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/input/rottentomatoes_list.py` & `FlexGet-3.6.3/flexget/plugins/input/rottentomatoes_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/input/rss.py` & `FlexGet-3.6.3/flexget/plugins/input/rss.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/input/sceper.py` & `FlexGet-3.6.3/flexget/plugins/input/sceper.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/input/sickbeard.py` & `FlexGet-3.6.3/flexget/plugins/input/sickbeard.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/input/tail.py` & `FlexGet-3.6.3/flexget/plugins/input/tail.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/input/text.py` & `FlexGet-3.6.3/flexget/plugins/input/text.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/input/torznab.py` & `FlexGet-3.6.3/flexget/plugins/input/torznab.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/input/twitterfeed.py` & `FlexGet-3.6.3/flexget/plugins/input/twitterfeed.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/internal/api_bluray.py` & `FlexGet-3.6.3/flexget/plugins/internal/api_bluray.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 def bluray_request(endpoint, **params) -> Any:
     full_url = BASE_URL + endpoint
     response = requests.get(full_url, params=params)
     if response.content:
         try:
             return response.json(strict=False)
-        except JSONDecodeError as e:
+        except JSONDecodeError:
             raise PluginError('Could decode json from response blu-ray api')
 
 
 def extract_release_date(bluray_entry: Dict[str, Any]) -> date:
     release_date = bluray_entry.get('reldate')
     if not release_date or release_date.lower() == 'no release date':
         try:
@@ -123,15 +123,15 @@
             self.bluray_rating = int(result['rating']) if result['rating'] else None
 
             # Used for parsing some more data, sadly with soup
             self.url = result['url']
 
             try:
                 movie_info_response = requests.get(self.url).content
-            except (requests.RequestException, ConnectionError) as e:
+            except (requests.RequestException, ConnectionError):
                 raise LookupError("Couldn't connect to blu-ray.com. %s" % self.url)
 
             movie_info = get_soup(movie_info_response)
 
             # runtime and rating, should be the last span tag with class subheading
             bluray_info = movie_info.find('div', attrs={'class': 'bluray'})
             bluray_info = bluray_info.find_all('span', attrs={'class': 'subheading'})[
```

### Comparing `FlexGet-3.6.2/flexget/plugins/internal/api_rottentomatoes.py` & `FlexGet-3.6.3/flexget/plugins/internal/api_rottentomatoes.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/internal/change_warn.py` & `FlexGet-3.6.3/flexget/plugins/internal/change_warn.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/metainfo/assume_quality.py` & `FlexGet-3.6.3/flexget/plugins/metainfo/assume_quality.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/metainfo/bluray_lookup.py` & `FlexGet-3.6.3/flexget/plugins/metainfo/bluray_lookup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from loguru import logger
 
-from flexget import entry, plugin
+from flexget import plugin
+from flexget.entry import register_lazy_lookup
 from flexget.event import event
 from flexget.manager import Session
 from flexget.utils.log import log_once
 from flexget.utils.tools import split_title_year
 
 logger = logger.bind(name='bluray_lookup')
 
@@ -32,15 +33,15 @@
         # Generic fields filled by all movie lookup plugins:
         'movie_name': 'name',
         'movie_year': 'year',
     }
 
     schema = {'type': 'boolean'}
 
-    @entry.register_lazy_lookup('bluray_lookup')
+    @register_lazy_lookup('bluray_lookup')
     def lazy_loader(self, entry):
         """Does the lookup for this entry and populates the entry fields."""
         lookup = plugin.get('api_bluray', self).lookup
 
         try:
             with Session() as session:
                 title, year = split_title_year(entry['title'])
```

### Comparing `FlexGet-3.6.2/flexget/plugins/metainfo/content_size.py` & `FlexGet-3.6.3/flexget/plugins/metainfo/content_size.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
                 try:
                     if location.is_file():
                         amount = os.path.getsize(entry['location'])
                         amount = int(amount / (1024 * 1024))
                         logger.trace('setting content size to {}', amount)
                         entry['content_size'] = amount
                         continue
-                except OSError as e:
+                except OSError:
                     # is_file can throw OSError for invalid paths (at least on windows)
                     continue
 
         if count:
             logger.debug('Found content size information from {} entries', count)
```

### Comparing `FlexGet-3.6.2/flexget/plugins/metainfo/media_id.py` & `FlexGet-3.6.3/flexget/plugins/metainfo/media_id.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from loguru import logger
 
-from flexget import entry, plugin
+from flexget import plugin
+from flexget.entry import register_lazy_lookup
 from flexget.event import event
 
 logger = logger.bind(name='metainfo_media_id')
 
 
 class MetainfoMediaId:
     """
@@ -17,15 +18,15 @@
     def on_task_metainfo(self, task, config):
         # Don't run if we are disabled
         if config is False:
             return
         for entry in task.entries:
             entry.add_lazy_fields(self.get_media_id, ['media_id'])
 
-    @entry.register_lazy_lookup('media_id')
+    @register_lazy_lookup('media_id')
     def get_media_id(self, entry):
         # Try to generate a media id based on available parser fields
         media_id = None
         if entry.get('movie_name'):
             media_id = entry['movie_name']
             if entry.get('movie_year'):
                 media_id = f'{media_id} {entry["movie_year"]}'
```

### Comparing `FlexGet-3.6.2/flexget/plugins/metainfo/metainfo_movie.py` & `FlexGet-3.6.3/flexget/plugins/metainfo/metainfo_movie.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/metainfo/nfo_lookup.py` & `FlexGet-3.6.3/flexget/plugins/metainfo/nfo_lookup.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/metainfo/nzb_size.py` & `FlexGet-3.6.3/flexget/plugins/metainfo/nzb_size.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/metainfo/quality.py` & `FlexGet-3.6.3/flexget/plugins/metainfo/quality.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from loguru import logger
 
-from flexget import entry, plugin
+from flexget import plugin
+from flexget.entry import register_lazy_lookup
 from flexget.event import event
 from flexget.utils import qualities
 
 logger = logger.bind(name='metainfo_quality')
 
 
 class MetainfoQuality:
@@ -28,15 +29,15 @@
                     entry['quality'],
                     entry['title'],
                 )
                 entry['quality'] = qualities.Quality(entry.get('quality', eval_lazy=False))
             else:
                 entry.add_lazy_fields(self.get_quality, ['quality'])
 
-    @entry.register_lazy_lookup('quality')
+    @register_lazy_lookup('quality')
     def get_quality(self, entry):
         if entry.get('quality', eval_lazy=False):
             logger.debug(
                 'Quality is already set to {} for {}, skipping quality detection.',
                 entry['quality'],
                 entry['title'],
             )
```

### Comparing `FlexGet-3.6.2/flexget/plugins/metainfo/rottentomatoes_lookup.py` & `FlexGet-3.6.3/flexget/plugins/metainfo/rottentomatoes_lookup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from loguru import logger
 
-from flexget import entry, plugin
+from flexget import plugin
+from flexget.entry import register_lazy_lookup
 from flexget.event import event
 from flexget.utils.log import log_once
 
 try:
     # NOTE: Importing other plugins is discouraged!
     from flexget.plugins.internal import api_rottentomatoes as plugin_api_rottentomatoes
 except ImportError:
@@ -63,15 +64,15 @@
             {'type': 'string', 'description': 'provide a custom api key'},
         ]
     }
 
     def __init__(self):
         self.key = None
 
-    @entry.register_lazy_lookup('rottentomatoes_lookup')
+    @register_lazy_lookup('rottentomatoes_lookup')
     def lazy_loader(self, entry):
         """Does the lookup for this entry and populates the entry fields.
 
         :param entry: entry to perform lookup on
         :returns: the field value
         """
         try:
```

### Comparing `FlexGet-3.6.2/flexget/plugins/metainfo/subtitles_check.py` & `FlexGet-3.6.3/flexget/plugins/metainfo/subtitles_check.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import logging
 import os
 import tempfile
 
 from loguru import logger
 
-from flexget import entry, plugin
+from flexget import plugin
+from flexget.entry import register_lazy_lookup
 from flexget.event import event
 
 logger = logger.bind(name='check_subtitles')
 
 
 class MetainfoSubs:
     """
@@ -48,19 +49,19 @@
     def on_task_metainfo(self, task, config):
         # check if explicitly disabled (value set to false)
         if config is False:
             return
         for entry in task.entries:
             entry.add_lazy_fields(self.get_subtitles, ['subtitles'])
 
-    @entry.register_lazy_lookup('subtitles_check')
+    @register_lazy_lookup('subtitles_check')
     def get_subtitles(self, entry):
         if (
             entry.get('subtitles', eval_lazy=False)
-            or not ('location' in entry)
+            or 'location' not in entry
             or ('$RECYCLE.BIN' in entry['location'])
             or not os.path.exists(entry['location'])
         ):
             return
         from subliminal import scan_video
         from subliminal.core import refine, search_external_subtitles
 
@@ -69,15 +70,15 @@
             # grab external and internal subtitles
             subtitles = video.subtitle_languages
             refiner = ('metadata',)
             refine(video, episode_refiners=refiner, movie_refiners=refiner)
             subtitles |= set(search_external_subtitles(entry['location']).values())
             if subtitles:
                 # convert to human-readable strings
-                subtitles = [str(l) for l in subtitles]
+                subtitles = [str(s) for s in subtitles]
                 entry['subtitles'] = subtitles
                 logger.debug('Found subtitles {} for {}', '/'.join(subtitles), entry['title'])
         except Exception as e:
             logger.error('Error checking local subtitles for {}: {}', entry['title'], e)
 
 
 @event('plugin.register')
```

### Comparing `FlexGet-3.6.2/flexget/plugins/metainfo/task.py` & `FlexGet-3.6.3/flexget/plugins/metainfo/task.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/modify/extension.py` & `FlexGet-3.6.3/flexget/plugins/modify/extension.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/modify/headers.py` & `FlexGet-3.6.3/flexget/plugins/modify/headers.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/modify/manipulate.py` & `FlexGet-3.6.3/flexget/plugins/modify/manipulate.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/modify/path_by_ext.py` & `FlexGet-3.6.3/flexget/plugins/modify/path_by_ext.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/modify/path_by_space.py` & `FlexGet-3.6.3/flexget/plugins/modify/path_by_space.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/modify/plugin_priority.py` & `FlexGet-3.6.3/flexget/plugins/modify/plugin_priority.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/modify/regex_extract.py` & `FlexGet-3.6.3/flexget/plugins/modify/regex_extract.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/modify/reorder_quality.py` & `FlexGet-3.6.3/flexget/plugins/modify/reorder_quality.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/modify/set_field.py` & `FlexGet-3.6.3/flexget/plugins/modify/set_field.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from loguru import logger
 
-from flexget import entry, plugin
+from flexget import plugin
+from flexget.entry import register_lazy_lookup
 from flexget.event import event
 from flexget.utils.template import RenderError
 
 logger = logger.bind(name='set')
 
 # Use a string for this sentinel, so it survives serialization
 UNSET = '__unset__'
@@ -47,15 +48,15 @@
                         'config': config,
                         'field': field,
                         'orig_field_value': orig_value,
                         'errors': errors,
                     },
                 )
 
-    @entry.register_lazy_lookup('set_field')
+    @register_lazy_lookup('set_field')
     def lazy_set(self, entry, config, field, orig_field_value, errors=True):
         level = 'ERROR' if errors else 'DEBUG'
         if orig_field_value is not UNSET:
             entry[field] = orig_field_value
         try:
             entry[field] = entry.render(config[field], native=True)
         except RenderError as e:
```

### Comparing `FlexGet-3.6.2/flexget/plugins/modify/sort_by.py` & `FlexGet-3.6.3/flexget/plugins/modify/sort_by.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/modify/sort_by_weight.py` & `FlexGet-3.6.3/flexget/plugins/modify/sort_by_weight.py`

 * *Files 0% similar despite different names*

```diff
@@ -252,15 +252,15 @@
 
                 weight = int(max(weight, 0))
                 entry[ENTRY_WEIGHT_FIELD_NAME] += weight
                 # self._add_debug_info(key, entry, weight, entry[key], value)  # debug only
 
     def _add_debug_info(self, key, entry, weight, *args):
         if 'weights' not in entry:
-            entry['weights'] = dict()
+            entry['weights'] = {}
         short_args = []
         for arg in args:
             if isinstance(arg, timedelta):
                 short_args.append(arg.days)
             elif isinstance(arg, datetime):
                 date = arg.date()
                 short_args.append(f'{date.year}-{date.month}-{date.day}')
```

### Comparing `FlexGet-3.6.2/flexget/plugins/operate/cfscraper.py` & `FlexGet-3.6.3/flexget/plugins/operate/cfscraper.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/operate/cookies.py` & `FlexGet-3.6.3/flexget/plugins/operate/cookies.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
                 from sqlite3 import dbapi2 as sqlite  # try the 2.5+ stdlib
             except ImportError:
                 raise plugin.PluginWarning('Unable to use sqlite3 or pysqlite2', logger)
 
         logger.debug('connecting: {}', filename)
         try:
             con = sqlite.connect(filename)
-        except:
+        except Exception:
             raise plugin.PluginError('Unable to open cookies sqlite database')
 
         cur = con.cursor()
         try:
             cur.execute('select host, path, isSecure, expiry, name, value from moz_cookies')
         except sqlite.Error:
             raise plugin.PluginError(
```

### Comparing `FlexGet-3.6.2/flexget/plugins/operate/debug_db_sessions.py` & `FlexGet-3.6.3/flexget/plugins/operate/debug_db_sessions.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     for frame in stack:
         # We don't care about sqlalchemy internals
         module = inspect.getmodule(frame[0])
         if not hasattr(module, '__name__'):
             continue
         if module.__name__.startswith('sqlalchemy'):
             continue
-        return (module.__name__,) + tuple(frame[2:4]) + (frame[4][0].strip(),)
+        return (module.__name__, *tuple(frame[2:4])) + (frame[4][0].strip(),)
     logger.warning('Transaction from unknown origin')
     return None, None, None, None
 
 
 def after_begin(session, transaction, connection):
     caller_info = find_caller(inspect.stack()[1:])
     with open_transactions_lock:
@@ -47,15 +47,15 @@
                 id(transaction),
                 caller_info,
                 open_transactions,
             )
         else:
             logger.debug('Transaction 0x{:08X} opened {}', id(transaction), caller_info)
         # Store information about this transaction
-        open_transactions[transaction] = (time.time(), connection.connection) + caller_info
+        open_transactions[transaction] = (time.time(), connection.connection, *caller_info)
 
 
 def after_flush(session, flush_context):
     if session.new or session.deleted or session.dirty:
         caller_info = find_caller(inspect.stack()[1:])
         with open_transactions_lock:
             # Dirty hack to support SQLAlchemy 1.1 without breaking backwards compatibility
```

### Comparing `FlexGet-3.6.2/flexget/plugins/operate/debug_warnings.py` & `FlexGet-3.6.3/flexget/plugins/operate/debug_warnings.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/operate/digest.py` & `FlexGet-3.6.3/flexget/plugins/operate/digest.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/operate/disable.py` & `FlexGet-3.6.3/flexget/plugins/operate/disable.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/operate/disable_phases.py` & `FlexGet-3.6.3/flexget/plugins/operate/disable_phases.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/operate/domain_delay.py` & `FlexGet-3.6.3/flexget/plugins/operate/domain_delay.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/operate/entry_trace.py` & `FlexGet-3.6.3/flexget/plugins/operate/entry_trace.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/operate/formlogin.py` & `FlexGet-3.6.3/flexget/plugins/operate/formlogin.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/operate/free_space.py` & `FlexGet-3.6.3/flexget/plugins/operate/free_space.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/operate/include.py` & `FlexGet-3.6.3/flexget/plugins/operate/include.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/operate/interval.py` & `FlexGet-3.6.3/flexget/plugins/operate/interval.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/operate/log_filter.py` & `FlexGet-3.6.3/flexget/plugins/operate/log_filter.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/operate/manual.py` & `FlexGet-3.6.3/flexget/plugins/operate/manual.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/operate/max_reruns.py` & `FlexGet-3.6.3/flexget/plugins/operate/max_reruns.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/operate/pathscrub.py` & `FlexGet-3.6.3/flexget/plugins/operate/pathscrub.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/operate/priority.py` & `FlexGet-3.6.3/flexget/plugins/operate/priority.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/operate/proxy.py` & `FlexGet-3.6.3/flexget/plugins/operate/proxy.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/operate/rerun.py` & `FlexGet-3.6.3/flexget/plugins/operate/rerun.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/operate/run_task.py` & `FlexGet-3.6.3/flexget/plugins/operate/run_task.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/operate/sequence.py` & `FlexGet-3.6.3/flexget/plugins/operate/sequence.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/operate/sleep.py` & `FlexGet-3.6.3/flexget/plugins/operate/sleep.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/operate/spy_headers.py` & `FlexGet-3.6.3/flexget/plugins/operate/spy_headers.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/operate/template.py` & `FlexGet-3.6.3/flexget/plugins/operate/template.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/operate/verbose.py` & `FlexGet-3.6.3/flexget/plugins/operate/verbose.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/operate/verbose_details.py` & `FlexGet-3.6.3/flexget/plugins/operate/verbose_details.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/operate/verify_ssl_certificates.py` & `FlexGet-3.6.3/flexget/plugins/operate/verify_ssl_certificates.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/operate/version_checker.py` & `FlexGet-3.6.3/flexget/plugins/operate/version_checker.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/output/download.py` & `FlexGet-3.6.3/flexget/plugins/output/download.py`

 * *Files 1% similar despite different names*

```diff
@@ -439,15 +439,15 @@
                 return
 
             # make path
             if not os.path.isdir(path):
                 logger.debug('Creating directory {}', path)
                 try:
                     os.makedirs(path)
-                except:
+                except Exception:
                     raise plugin.PluginError('Cannot create path %s' % path, logger)
 
             # check that temp file is present
             if not os.path.exists(entry['file']):
                 logger.debug('entry: {}', entry)
                 raise plugin.PluginWarning(
                     'Downloaded temp file `%s` doesn\'t exist!?' % entry['file']
@@ -503,15 +503,15 @@
                     return
             else:
                 # move temp file
                 logger.debug('moving {} to {}', entry['file'], destfile)
 
                 try:
                     shutil.move(entry['file'], destfile)
-                except (OSError, OSError) as err:
+                except OSError as err:
                     # ignore permission errors, see ticket #555
                     import errno
 
                     if not os.path.exists(destfile):
                         raise plugin.PluginError(f'Unable to write {destfile}: {err}')
                     if err.errno != errno.EPERM and err.errno != errno.EACCES:
                         raise
```

### Comparing `FlexGet-3.6.2/flexget/plugins/output/download_auth.py` & `FlexGet-3.6.3/flexget/plugins/output/download_auth.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/output/dump.py` & `FlexGet-3.6.3/flexget/plugins/output/dump.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/output/dump_config.py` & `FlexGet-3.6.3/flexget/plugins/output/dump_config.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/output/exec.py` & `FlexGet-3.6.3/flexget/plugins/output/exec.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/output/file_operations.py` & `FlexGet-3.6.3/flexget/plugins/output/file_operations.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/output/html.py` & `FlexGet-3.6.3/flexget/plugins/output/html.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/output/memusage.py` & `FlexGet-3.6.3/flexget/plugins/output/memusage.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/output/mock_output.py` & `FlexGet-3.6.3/flexget/plugins/output/mock_output.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/output/rss.py` & `FlexGet-3.6.3/flexget/plugins/output/rss.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/output/rtorrent_magnet.py` & `FlexGet-3.6.3/flexget/plugins/output/rtorrent_magnet.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/output/sabnzbd.py` & `FlexGet-3.6.3/flexget/plugins/output/sabnzbd.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/output/sns.py` & `FlexGet-3.6.3/flexget/plugins/output/sns.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/output/subtitles.py` & `FlexGet-3.6.3/flexget/plugins/output/subtitles.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/output/subtitles_periscope.py` & `FlexGet-3.6.3/flexget/plugins/output/subtitles_periscope.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/output/subtitles_subliminal.py` & `FlexGet-3.6.3/flexget/plugins/output/subtitles_subliminal.py`

 * *Files 1% similar despite different names*

```diff
@@ -246,15 +246,15 @@
                             if subtitles:
                                 downloaded_subtitles[video].extend(subtitles)
                                 entry.reject('subtitles found for a second-choice language.')
                             else:
                                 entry.reject('cannot find any subtitles for now.')
 
                         downloaded_languages = {
-                            Language.fromietf(str(l.language)) for l in subtitles
+                            Language.fromietf(str(s.language)) for s in subtitles
                         }
                         if entry_languages:
                             entry['subtitles_missing'] = entry_languages - downloaded_languages
                             if len(entry['subtitles_missing']) > 0:
                                 entry.reject('Subtitles for all primary languages not found')
                 except ValueError as e:
                     logger.error('subliminal error: {}', e)
@@ -268,15 +268,15 @@
                 if subtitle:
                     _directory = config.get('directory')
                     if _directory:
                         _directory = os.path.expanduser(_directory)
                     if task.options.test:
                         logger.verbose(
                             '     FOUND LANGUAGES {} for {}',
-                            [str(l.language) for l in subtitle],
+                            [str(s.language) for s in subtitle],
                             video.name,
                         )
                         continue
                     save_subtitles(video, subtitle, single=single_mode, directory=_directory)
 
 
 @event('plugin.register')
```

### Comparing `FlexGet-3.6.2/flexget/plugins/output/symlink.py` & `FlexGet-3.6.3/flexget/plugins/output/symlink.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 
 from loguru import logger
 
 from flexget import plugin
 from flexget.event import event
 from flexget.utils.pathscrub import pathscrub
-from flexget.utils.template import RenderError, render_from_entry
+from flexget.utils.template import RenderError
 
 logger = logger.bind(name='symlink')
 
 
 class Symlink:
     schema = {
         'oneOf': [
```

### Comparing `FlexGet-3.6.2/flexget/plugins/output/utorrent.py` & `FlexGet-3.6.3/flexget/plugins/output/utorrent.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
         for entry in task.accepted:
             # bunch of urls now going to check
 
             folder = 0
             path = entry.get('path', config.get('path', ''))
             try:
                 path = os.path.expanduser(entry.render(path))
-            except RenderError as e:
+            except RenderError:
                 logger.error(
                     'Could not render path for `{}` downloading to default directory.',
                     entry['title'],
                 )
                 # Add to default folder
                 path = ''
             if path:
```

### Comparing `FlexGet-3.6.2/flexget/plugins/services/kodi_library.py` & `FlexGet-3.6.3/flexget/plugins/services/kodi_library.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/services/myepisodes.py` & `FlexGet-3.6.3/flexget/plugins/services/myepisodes.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/plugins/services/pogcal_acquired.py` & `FlexGet-3.6.3/flexget/plugins/services/pogcal_acquired.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/resources/flexget.png` & `FlexGet-3.6.3/flexget/resources/flexget.png`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/task.py` & `FlexGet-3.6.3/flexget/task.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,17 +19,17 @@
 from flexget.plugin import (
     DependencyError,
     PluginError,
     PluginWarning,
     get_plugins,
     phase_methods,
     plugin_schemas,
+    task_phases,
 )
 from flexget.plugin import plugins as all_plugins
-from flexget.plugin import task_phases
 from flexget.terminal import capture_console
 from flexget.utils import requests
 from flexget.utils.database import with_session
 from flexget.utils.simple_persistence import SimpleTaskPersistence
 from flexget.utils.sqlalchemy_utils import ContextSession
 from flexget.utils.template import FlexGetTemplate, render_from_task
 from flexget.utils.tools import MergeException, get_config_hash, merge_dict_from_to
@@ -239,15 +239,15 @@
             options = copy.copy(self.manager.options.execute)
         elif isinstance(options, dict):
             options_namespace = copy.copy(self.manager.options.execute)
             options_namespace.__dict__.update(options)
             options = options_namespace
         # If execution hasn't specifically set the `allow_manual` flag, set it to False by default
         if not hasattr(options, 'allow_manual'):
-            setattr(options, 'allow_manual', False)
+            options.allow_manual = False
         self.options = options
         self.output = output
         self.session_id = session_id
         self.suppress_warnings = suppress_warnings or []
         if priority is None:
             self.priority = 10 if self.options.cron else 0
         else:
```

### Comparing `FlexGet-3.6.2/flexget/task_queue.py` & `FlexGet-3.6.3/flexget/task_queue.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import queue
-import sys
 import threading
 import time
 from typing import Optional
 
 from loguru import logger
 from sqlalchemy.exc import OperationalError, ProgrammingError
```

### Comparing `FlexGet-3.6.2/flexget/templates/task/default.template` & `FlexGet-3.6.3/flexget/templates/task/default.template`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/templates/task/html.template` & `FlexGet-3.6.3/flexget/templates/task/html.template`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/templates/task/rss.template` & `FlexGet-3.6.3/flexget/templates/task/rss.template`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/terminal.py` & `FlexGet-3.6.3/flexget/terminal.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/tray_icon.py` & `FlexGet-3.6.3/flexget/tray_icon.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         index: int = None,
         **kwargs,
     ):
         """
         Add a menu item byt passing its text and function, or pass a created MenuItem. Force position by sending index
         """
         if not any(v for v in (menu_item, text)):
-            raise ValueError(f"Either 'text' or 'menu_item' are required")
+            raise ValueError("Either 'text' or 'menu_item' are required")
 
         menu_item = menu_item or MenuItem(text=text, action=action, **kwargs)
         if index is not None:
             self.menu_items.insert(index, menu_item)
         else:
             self.menu_items.append(menu_item)
```

### Comparing `FlexGet-3.6.2/flexget/ui/v1/__init__.py` & `FlexGet-3.6.3/flexget/ui/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/app/app.html` & `FlexGet-3.6.3/flexget/ui/v1/app/app.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/app/assets/images/header.png` & `FlexGet-3.6.3/flexget/ui/v1/app/assets/images/header.png`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/app/favicon.ico` & `FlexGet-3.6.3/flexget/ui/v1/app/favicon.ico`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/app/fonts/FontAwesome.otf` & `FlexGet-3.6.3/flexget/ui/v1/app/fonts/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/app/fonts/fontawesome-webfont.eot` & `FlexGet-3.6.3/flexget/ui/v1/app/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/app/fonts/fontawesome-webfont.svg` & `FlexGet-3.6.3/flexget/ui/v1/app/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/app/fonts/fontawesome-webfont.ttf` & `FlexGet-3.6.3/flexget/ui/v1/app/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/app/fonts/fontawesome-webfont.woff` & `FlexGet-3.6.3/flexget/ui/v1/app/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/app/fonts/fontawesome-webfont.woff2` & `FlexGet-3.6.3/flexget/ui/v1/app/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/app/fonts/ui-grid.eot` & `FlexGet-3.6.3/flexget/ui/v1/app/fonts/ui-grid.eot`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/app/fonts/ui-grid.svg` & `FlexGet-3.6.3/flexget/ui/v1/app/fonts/ui-grid.svg`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/app/fonts/ui-grid.ttf` & `FlexGet-3.6.3/flexget/ui/v1/app/fonts/ui-grid.ttf`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/app/fonts/ui-grid.woff` & `FlexGet-3.6.3/flexget/ui/v1/app/fonts/ui-grid.woff`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/app/scripts/app.js` & `FlexGet-3.6.3/flexget/ui/v1/app/scripts/app.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/app/scripts/splash.js` & `FlexGet-3.6.3/flexget/ui/v1/app/scripts/splash.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/app/scripts/vendor.js` & `FlexGet-3.6.3/flexget/ui/v1/app/scripts/vendor.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/app/styles/app.css` & `FlexGet-3.6.3/flexget/ui/v1/app/styles/app.css`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/app/styles/splash.css` & `FlexGet-3.6.3/flexget/ui/v1/app/styles/splash.css`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/app/styles/vendor.css` & `FlexGet-3.6.3/flexget/ui/v1/app/styles/vendor.css`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/bower.json` & `FlexGet-3.6.3/flexget/ui/v1/bower.json`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/gulp/build.js` & `FlexGet-3.6.3/flexget/ui/v1/gulp/build.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/gulp/inject.js` & `FlexGet-3.6.3/flexget/ui/v1/gulp/inject.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/gulp/lint.js` & `FlexGet-3.6.3/flexget/ui/v1/gulp/lint.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/gulp/proxy.js` & `FlexGet-3.6.3/flexget/ui/v1/gulp/proxy.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/gulp/server.js` & `FlexGet-3.6.3/flexget/ui/v1/gulp/server.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/gulp/styles.js` & `FlexGet-3.6.3/flexget/ui/v1/gulp/styles.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/gulp/test.js` & `FlexGet-3.6.3/flexget/ui/v1/gulp/test.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/gulp/watch.js` & `FlexGet-3.6.3/flexget/ui/v1/gulp/watch.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/karma.conf.js` & `FlexGet-3.6.3/flexget/ui/v1/karma.conf.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/package.json` & `FlexGet-3.6.3/flexget/ui/v1/package.json`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/specs.html` & `FlexGet-3.6.3/flexget/ui/v1/specs.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/app.html` & `FlexGet-3.6.3/flexget/ui/v1/src/app.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/app.module.js` & `FlexGet-3.6.3/flexget/ui/v1/src/app.module.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/app.scss` & `FlexGet-3.6.3/flexget/ui/v1/src/app.scss`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/assets/images/header.png` & `FlexGet-3.6.3/flexget/ui/v1/src/assets/images/header.png`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/blocks/error/error-dialog.component.js` & `FlexGet-3.6.3/flexget/ui/v1/src/blocks/error/error-dialog.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/blocks/error/error-dialog.component.spec.js` & `FlexGet-3.6.3/flexget/ui/v1/src/blocks/error/error-dialog.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/blocks/error/error-dialog.tmpl.html` & `FlexGet-3.6.3/flexget/ui/v1/src/blocks/error/error-dialog.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/blocks/error/error.service.js` & `FlexGet-3.6.3/flexget/ui/v1/src/blocks/error/error.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/blocks/error/error.service.spec.js` & `FlexGet-3.6.3/flexget/ui/v1/src/blocks/error/error.service.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/blocks/exception/exception.service.js` & `FlexGet-3.6.3/flexget/ui/v1/src/blocks/exception/exception.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/blocks/exception/exception.service.spec.js` & `FlexGet-3.6.3/flexget/ui/v1/src/blocks/exception/exception.service.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/blocks/pagination/_pagination.scss` & `FlexGet-3.6.3/flexget/ui/v1/src/blocks/pagination/_pagination.scss`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/blocks/pagination/pagination.component.js` & `FlexGet-3.6.3/flexget/ui/v1/src/blocks/pagination/pagination.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/blocks/pagination/pagination.tmpl.html` & `FlexGet-3.6.3/flexget/ui/v1/src/blocks/pagination/pagination.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/blocks/router/router-helper.provider.js` & `FlexGet-3.6.3/flexget/ui/v1/src/blocks/router/router-helper.provider.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/blocks/url-interceptor/url-interceptor.service.js` & `FlexGet-3.6.3/flexget/ui/v1/src/blocks/url-interceptor/url-interceptor.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/blocks/url-interceptor/url-interceptor.service.spec.js` & `FlexGet-3.6.3/flexget/ui/v1/src/blocks/url-interceptor/url-interceptor.service.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/components/404/404.component.spec.js` & `FlexGet-3.6.3/flexget/ui/v1/src/components/404/404.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/components/404/404.route.js` & `FlexGet-3.6.3/flexget/ui/v1/src/components/404/404.route.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/components/404/404.route.spec.js` & `FlexGet-3.6.3/flexget/ui/v1/src/components/404/404.route.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/components/404/404.tmpl.html` & `FlexGet-3.6.3/flexget/ui/v1/src/components/404/404.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/components/auth/auth.config.js` & `FlexGet-3.6.3/flexget/ui/v1/src/components/auth/auth.config.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/components/auth/auth.config.spec.js` & `FlexGet-3.6.3/flexget/ui/v1/src/components/auth/auth.config.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/components/auth/auth.service.js` & `FlexGet-3.6.3/flexget/ui/v1/src/components/auth/auth.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/components/auth/auth.service.spec.js` & `FlexGet-3.6.3/flexget/ui/v1/src/components/auth/auth.service.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/components/auth/login.component.js` & `FlexGet-3.6.3/flexget/ui/v1/src/components/auth/login.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/components/auth/login.component.spec.js` & `FlexGet-3.6.3/flexget/ui/v1/src/components/auth/login.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/components/auth/login.route.js` & `FlexGet-3.6.3/flexget/ui/v1/src/components/auth/login.route.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/components/auth/login.route.spec.js` & `FlexGet-3.6.3/flexget/ui/v1/src/components/auth/login.route.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/components/auth/login.tmpl.html` & `FlexGet-3.6.3/flexget/ui/v1/src/components/auth/login.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/components/core/core.config.js` & `FlexGet-3.6.3/flexget/ui/v1/src/components/core/core.config.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/components/core/core.provider.js` & `FlexGet-3.6.3/flexget/ui/v1/src/components/core/core.provider.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/components/database/database.component.js` & `FlexGet-3.6.3/flexget/ui/v1/src/components/database/database.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/components/database/database.config.js` & `FlexGet-3.6.3/flexget/ui/v1/src/components/database/database.config.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/components/database/database.service.js` & `FlexGet-3.6.3/flexget/ui/v1/src/components/database/database.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/components/database/database.tmpl.html` & `FlexGet-3.6.3/flexget/ui/v1/src/components/database/database.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/components/home/home.route.js` & `FlexGet-3.6.3/flexget/ui/v1/src/components/home/home.route.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/components/home/home.route.spec.js` & `FlexGet-3.6.3/flexget/ui/v1/src/components/home/home.route.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/components/home/home.tmpl.html` & `FlexGet-3.6.3/flexget/ui/v1/src/components/home/home.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/components/sidenav/_sidenav.scss` & `FlexGet-3.6.3/flexget/ui/v1/src/components/sidenav/_sidenav.scss`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/components/sidenav/sidenav.component.js` & `FlexGet-3.6.3/flexget/ui/v1/src/components/sidenav/sidenav.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/components/sidenav/sidenav.component.spec.js` & `FlexGet-3.6.3/flexget/ui/v1/src/components/sidenav/sidenav.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/components/sidenav/sidenav.semver.js` & `FlexGet-3.6.3/flexget/ui/v1/src/components/sidenav/sidenav.semver.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/components/sidenav/sidenav.service.js` & `FlexGet-3.6.3/flexget/ui/v1/src/components/sidenav/sidenav.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/components/sidenav/sidenav.service.spec.js` & `FlexGet-3.6.3/flexget/ui/v1/src/components/sidenav/sidenav.service.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/components/sidenav/sidenav.tmpl.html` & `FlexGet-3.6.3/flexget/ui/v1/src/components/sidenav/sidenav.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/components/toolbar/toolbar.component.js` & `FlexGet-3.6.3/flexget/ui/v1/src/components/toolbar/toolbar.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/components/toolbar/toolbar.component.spec.js` & `FlexGet-3.6.3/flexget/ui/v1/src/components/toolbar/toolbar.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/components/toolbar/toolbar.provider.js` & `FlexGet-3.6.3/flexget/ui/v1/src/components/toolbar/toolbar.provider.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/components/toolbar/toolbar.tmpl.html` & `FlexGet-3.6.3/flexget/ui/v1/src/components/toolbar/toolbar.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/construction.tmpl.html` & `FlexGet-3.6.3/flexget/ui/v1/src/construction.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/directives/palette-background/palette-background.directive.js` & `FlexGet-3.6.3/flexget/ui/v1/src/directives/palette-background/palette-background.directive.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/favicon.ico` & `FlexGet-3.6.3/flexget/ui/v1/src/favicon.ico`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/config/config.component.js` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/config/config.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/config/config.component.spec.js` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/config/config.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/config/config.route.js` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/config/config.route.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/config/config.route.spec.js` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/config/config.route.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/config/config.service.js` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/config/config.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/config/config.tmpl.html` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/config/config.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/execute/components/execute-input/execute-input.component.js` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/execute/components/execute-input/execute-input.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/execute/components/execute-input/execute-input.component.spec.js` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/execute/components/execute-input/execute-input.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/execute/components/execute-input/execute-input.tmpl.html` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/execute/components/execute-input/execute-input.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/execute/components/execute-stream/execute-stream.component.js` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/execute/components/execute-stream/execute-stream.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/execute/components/execute-stream/execute-stream.component.spec.js` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/execute/components/execute-stream/execute-stream.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/execute/components/execute-stream/execute-stream.tmpl.html` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/execute/components/execute-stream/execute-stream.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/execute/execute.component.js` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/execute/execute.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/execute/execute.component.spec.js` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/execute/execute.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/execute/execute.filter.js` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/execute/execute.filter.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/execute/execute.filter.spec.js` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/execute/execute.filter.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/execute/execute.route.js` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/execute/execute.route.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/execute/execute.route.spec.js` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/execute/execute.route.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/execute/execute.service.js` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/execute/execute.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/execute/execute.service.spec.js` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/execute/execute.service.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/history/history.component.js` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/history/history.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/history/history.component.spec.js` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/history/history.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/history/history.route.js` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/history/history.route.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/history/history.route.spec.js` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/history/history.route.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/history/history.service.js` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/history/history.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/history/history.service.spec.js` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/history/history.service.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/history/history.tmpl.html` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/history/history.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/log/log.component.js` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/log/log.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/log/log.component.spec.js` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/log/log.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/log/log.route.js` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/log/log.route.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/log/log.route.spec.js` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/log/log.route.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/log/log.service.js` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/log/log.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/log/log.tmpl.html` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/log/log.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/log/log.tmpl.scss` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/log/log.tmpl.scss`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie-input.directive.js` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie-input.directive.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie-item.component.js` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie-item.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie-item.tmpl.html` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie-item.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie.controller.js` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie.controller.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie.service.js` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie.tmpl.html` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.component.js` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.component.spec.js` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.scss` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.scss`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.tmpl.html` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/movies/components/movie-list/movie-list.component.js` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/movies/components/movie-list/movie-list.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/movies/components/movie-list/movie-list.component.spec.js` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/movies/components/movie-list/movie-list.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/movies/components/movie-list/movie-list.tmpl.html` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/movies/components/movie-list/movie-list.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/movies/components/new-list/new-list.component.js` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/movies/components/new-list/new-list.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/movies/components/new-list/new-list.component.spec.js` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/movies/components/new-list/new-list.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/movies/components/new-list/new-list.tmpl.html` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/movies/components/new-list/new-list.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/movies/movies.component.js` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/movies/movies.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/movies/movies.component.spec.js` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/movies/movies.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/movies/movies.route.js` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/movies/movies.route.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/movies/movies.route.spec.js` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/movies/movies.route.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/movies/movies.service.js` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/movies/movies.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/movies/movies.service.spec.js` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/movies/movies.service.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/movies/movies.tmpl.html` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/movies/movies.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/movies/movies.tmpl.scss` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/movies/movies.tmpl.scss`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/pending/pending.component.js` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/pending/pending.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/pending/pending.route.js` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/pending/pending.route.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/pending/pending.service.js` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/pending/pending.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/pending/pending.tmpl.html` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/pending/pending.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/schedule/schedule.component.js` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/schedule/schedule.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/schedule/schedule.component.spec.js` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/schedule/schedule.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/schedule/schedule.route.js` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/schedule/schedule.route.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/schedule/schedule.route.spec.js` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/schedule/schedule.route.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/schedule/schedule.service.js` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/schedule/schedule.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/schedule/schedule.service.spec.js` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/schedule/schedule.service.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/seen/components/seen-entry/seen-entry.tmpl.html` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/seen/components/seen-entry/seen-entry.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/seen/seen.component.js` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/seen/seen.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/seen/seen.component.spec.js` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/seen/seen.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/seen/seen.route.js` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/seen/seen.route.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/seen/seen.route.spec.js` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/seen/seen.route.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/seen/seen.service.js` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/seen/seen.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/seen/seen.service.spec.js` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/seen/seen.service.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/series/components/episode-release/episode-release.component.js` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/series/components/episode-release/episode-release.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/series/components/episode-release/episode-release.component.spec.js` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/series/components/episode-release/episode-release.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/series/components/episode-release/episode-release.tmpl.html` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/series/components/episode-release/episode-release.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/series/components/episode-releases/episode-releases.component.js` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/series/components/episode-releases/episode-releases.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/series/components/episode-releases/episode-releases.component.spec.js` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/series/components/episode-releases/episode-releases.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/series/components/episode-releases/episode-releases.tmpl.html` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/series/components/episode-releases/episode-releases.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/series/components/series-begin-dialog/series-begin-dialog.component.js` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/series/components/series-begin-dialog/series-begin-dialog.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/series/components/series-begin-dialog/series-begin-dialog.tmpl.html` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/series/components/series-begin-dialog/series-begin-dialog.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/series/components/series-entry/series-entry.component.js` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/series/components/series-entry/series-entry.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/series/components/series-entry/series-entry.component.spec.js` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/series/components/series-entry/series-entry.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/series/components/series-entry/series-entry.tmpl.html` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/series/components/series-entry/series-entry.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/series/components/series-episode/series-episode.component.js` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/series/components/series-episode/series-episode.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/series/components/series-episode/series-episode.component.spec.js` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/series/components/series-episode/series-episode.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/series/components/series-episode/series-episode.tmpl.html` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/series/components/series-episode/series-episode.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.component.js` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.component.spec.js` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.scss` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.scss`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.tmpl.html` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/series/series.component.js` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/series/series.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/series/series.component.spec.js` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/series/series.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/series/series.route.js` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/series/series.route.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/series/series.route.spec.js` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/series/series.route.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/series/series.service.js` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/series/series.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/series/series.service.spec.js` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/series/series.service.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/series/series.tmpl.html` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/series/series.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/server/loading-dialog.component.js` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/server/loading-dialog.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/server/loading-dialog.tmpl.html` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/server/loading-dialog.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/server/server.config.js` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/server/server.config.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/server/server.service.js` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/server/server.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/status/status.component.js` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/status/status.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/status/status.route.js` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/status/status.route.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/status/status.service.js` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/status/status.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/plugins/status/status.tmpl.html` & `FlexGet-3.6.3/flexget/ui/v1/src/plugins/status/status.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/scss/_header.scss` & `FlexGet-3.6.3/flexget/ui/v1/src/scss/_header.scss`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/scss/flexget.scss` & `FlexGet-3.6.3/flexget/ui/v1/src/scss/flexget.scss`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/src/services/schema.service.js` & `FlexGet-3.6.3/flexget/ui/v1/src/services/schema.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/tests-mock-data/config.js` & `FlexGet-3.6.3/flexget/ui/v1/tests-mock-data/config.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/tests-mock-data/execute.js` & `FlexGet-3.6.3/flexget/ui/v1/tests-mock-data/execute.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/tests-mock-data/history.js` & `FlexGet-3.6.3/flexget/ui/v1/tests-mock-data/history.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/tests-mock-data/movie_list.js` & `FlexGet-3.6.3/flexget/ui/v1/tests-mock-data/movie_list.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/tests-mock-data/seen.js` & `FlexGet-3.6.3/flexget/ui/v1/tests-mock-data/seen.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/tests-mock-data/series.js` & `FlexGet-3.6.3/flexget/ui/v1/tests-mock-data/series.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v1/tests-mock-data/states.js` & `FlexGet-3.6.3/flexget/ui/v1/tests-mock-data/states.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v2/__init__.py` & `FlexGet-3.6.3/flexget/ui/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v2/dist/assets/020c97dc8e0463259c2f9df929bb0c69.woff2` & `FlexGet-3.6.3/flexget/ui/v2/dist/assets/020c97dc8e0463259c2f9df929bb0c69.woff2`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v2/dist/assets/14.18cf3ab07df2cff9c980.js` & `FlexGet-3.6.3/flexget/ui/v2/dist/assets/14.18cf3ab07df2cff9c980.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v2/dist/assets/14.18cf3ab07df2cff9c980.js.map` & `FlexGet-3.6.3/flexget/ui/v2/dist/assets/14.18cf3ab07df2cff9c980.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v2/dist/assets/14286f3ba79c6627433572dfa925202e.woff2` & `FlexGet-3.6.3/flexget/ui/v2/dist/assets/14286f3ba79c6627433572dfa925202e.woff2`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v2/dist/assets/15.df643f032866e7897440.js` & `FlexGet-3.6.3/flexget/ui/v2/dist/assets/15.df643f032866e7897440.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v2/dist/assets/15.df643f032866e7897440.js.map` & `FlexGet-3.6.3/flexget/ui/v2/dist/assets/15.df643f032866e7897440.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v2/dist/assets/16.d99413fe0332d02516c9.js` & `FlexGet-3.6.3/flexget/ui/v2/dist/assets/16.d99413fe0332d02516c9.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v2/dist/assets/16.d99413fe0332d02516c9.js.map` & `FlexGet-3.6.3/flexget/ui/v2/dist/assets/16.d99413fe0332d02516c9.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v2/dist/assets/2735a3a69b509faf3577afd25bdf552e.woff2` & `FlexGet-3.6.3/flexget/ui/v2/dist/assets/2735a3a69b509faf3577afd25bdf552e.woff2`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v2/dist/assets/288ad9c6e8b43cf02443a1f499bdf67e.woff` & `FlexGet-3.6.3/flexget/ui/v2/dist/assets/288ad9c6e8b43cf02443a1f499bdf67e.woff`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v2/dist/assets/28f9151055c950874d2c6803a39b425b.woff` & `FlexGet-3.6.3/flexget/ui/v2/dist/assets/28f9151055c950874d2c6803a39b425b.woff`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v2/dist/assets/35bb8d560db5205616671eab8c4d0303.ttf` & `FlexGet-3.6.3/flexget/ui/v2/dist/assets/35bb8d560db5205616671eab8c4d0303.ttf`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v2/dist/assets/479970ffb74f2117317f9d24d9e317fe.woff2` & `FlexGet-3.6.3/flexget/ui/v2/dist/assets/479970ffb74f2117317f9d24d9e317fe.woff2`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v2/dist/assets/4cb446d4c3b18f2f69df.worker.js` & `FlexGet-3.6.3/flexget/ui/v2/dist/assets/4cb446d4c3b18f2f69df.worker.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v2/dist/assets/4cb446d4c3b18f2f69df.worker.js.map` & `FlexGet-3.6.3/flexget/ui/v2/dist/assets/4cb446d4c3b18f2f69df.worker.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v2/dist/assets/4df32891a5f2f98a363314f595482e08.woff` & `FlexGet-3.6.3/flexget/ui/v2/dist/assets/4df32891a5f2f98a363314f595482e08.woff`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v2/dist/assets/51521a2a8da71e50d871ac6fd2187e87.woff2` & `FlexGet-3.6.3/flexget/ui/v2/dist/assets/51521a2a8da71e50d871ac6fd2187e87.woff2`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v2/dist/assets/5cb7edfceb233100075dc9a1e12e8da3.woff` & `FlexGet-3.6.3/flexget/ui/v2/dist/assets/5cb7edfceb233100075dc9a1e12e8da3.woff`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v2/dist/assets/60fa3c0614b8fb2f394fa29944c21540.woff` & `FlexGet-3.6.3/flexget/ui/v2/dist/assets/60fa3c0614b8fb2f394fa29944c21540.woff`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v2/dist/assets/68c852c85ea688dfa942.worker.js` & `FlexGet-3.6.3/flexget/ui/v2/dist/assets/68c852c85ea688dfa942.worker.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v2/dist/assets/68c852c85ea688dfa942.worker.js.map` & `FlexGet-3.6.3/flexget/ui/v2/dist/assets/68c852c85ea688dfa942.worker.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v2/dist/assets/7370c3679472e9560965ff48a4399d0b.woff2` & `FlexGet-3.6.3/flexget/ui/v2/dist/assets/7370c3679472e9560965ff48a4399d0b.woff2`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v2/dist/assets/81f57861ed4ac74741f5671e1dff2fd9.woff` & `FlexGet-3.6.3/flexget/ui/v2/dist/assets/81f57861ed4ac74741f5671e1dff2fd9.woff`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v2/dist/assets/87284894879f5b1c229cb49c8ff6decc.woff` & `FlexGet-3.6.3/flexget/ui/v2/dist/assets/87284894879f5b1c229cb49c8ff6decc.woff`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v2/dist/assets/9b3766ef4a402ad3fdeef7501a456512.woff2` & `FlexGet-3.6.3/flexget/ui/v2/dist/assets/9b3766ef4a402ad3fdeef7501a456512.woff2`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.css` & `FlexGet-3.6.3/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.css`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.css.map` & `FlexGet-3.6.3/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.css.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.js` & `FlexGet-3.6.3/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.js.map` & `FlexGet-3.6.3/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v2/dist/assets/EntryListPlugin.c4b35103ad1660e69c44.js` & `FlexGet-3.6.3/flexget/ui/v2/dist/assets/EntryListPlugin.c4b35103ad1660e69c44.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v2/dist/assets/EntryListPlugin.c4b35103ad1660e69c44.js.map` & `FlexGet-3.6.3/flexget/ui/v2/dist/assets/EntryListPlugin.c4b35103ad1660e69c44.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v2/dist/assets/HistoryPlugin.0201ee39aecaa7452270.js` & `FlexGet-3.6.3/flexget/ui/v2/dist/assets/HistoryPlugin.0201ee39aecaa7452270.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v2/dist/assets/HistoryPlugin.0201ee39aecaa7452270.js.map` & `FlexGet-3.6.3/flexget/ui/v2/dist/assets/HistoryPlugin.0201ee39aecaa7452270.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.css` & `FlexGet-3.6.3/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.css`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.css.map` & `FlexGet-3.6.3/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.css.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.js` & `FlexGet-3.6.3/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.js.map` & `FlexGet-3.6.3/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v2/dist/assets/MovieListPlugin.17e519c9d031c1cd9477.js` & `FlexGet-3.6.3/flexget/ui/v2/dist/assets/MovieListPlugin.17e519c9d031c1cd9477.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v2/dist/assets/MovieListPlugin.17e519c9d031c1cd9477.js.map` & `FlexGet-3.6.3/flexget/ui/v2/dist/assets/MovieListPlugin.17e519c9d031c1cd9477.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v2/dist/assets/PendingListPlugin.7ddbee4abf831e808220.js` & `FlexGet-3.6.3/flexget/ui/v2/dist/assets/PendingListPlugin.7ddbee4abf831e808220.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v2/dist/assets/PendingListPlugin.7ddbee4abf831e808220.js.map` & `FlexGet-3.6.3/flexget/ui/v2/dist/assets/PendingListPlugin.7ddbee4abf831e808220.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v2/dist/assets/SeriesPlugin.f46122b2f63739898cd5.js` & `FlexGet-3.6.3/flexget/ui/v2/dist/assets/SeriesPlugin.f46122b2f63739898cd5.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v2/dist/assets/SeriesPlugin.f46122b2f63739898cd5.js.map` & `FlexGet-3.6.3/flexget/ui/v2/dist/assets/SeriesPlugin.f46122b2f63739898cd5.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v2/dist/assets/TasksHomeCard.0f1a9b4992c80e636a4f.js` & `FlexGet-3.6.3/flexget/ui/v2/dist/assets/TasksHomeCard.0f1a9b4992c80e636a4f.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v2/dist/assets/TasksHomeCard.0f1a9b4992c80e636a4f.js.map` & `FlexGet-3.6.3/flexget/ui/v2/dist/assets/TasksHomeCard.0f1a9b4992c80e636a4f.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v2/dist/assets/TasksPlugin.78a8bc05a72c9f25d7c3.js` & `FlexGet-3.6.3/flexget/ui/v2/dist/assets/TasksPlugin.78a8bc05a72c9f25d7c3.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v2/dist/assets/TasksPlugin.78a8bc05a72c9f25d7c3.js.map` & `FlexGet-3.6.3/flexget/ui/v2/dist/assets/TasksPlugin.78a8bc05a72c9f25d7c3.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v2/dist/assets/adcde98f1d584de52060ad7b16373da3.woff` & `FlexGet-3.6.3/flexget/ui/v2/dist/assets/adcde98f1d584de52060ad7b16373da3.woff`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v2/dist/assets/b00849e00f4c2331cddd8ffb44a6720b.woff` & `FlexGet-3.6.3/flexget/ui/v2/dist/assets/b00849e00f4c2331cddd8ffb44a6720b.woff`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v2/dist/assets/bb1e4dc6333675d11ada2e857e7f95d7.woff` & `FlexGet-3.6.3/flexget/ui/v2/dist/assets/bb1e4dc6333675d11ada2e857e7f95d7.woff`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v2/dist/assets/da0e717829e033a69dec97f1e155ae42.woff2` & `FlexGet-3.6.3/flexget/ui/v2/dist/assets/da0e717829e033a69dec97f1e155ae42.woff2`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v2/dist/assets/db4a2a231f52e497c0191e8966b0ee58.woff2` & `FlexGet-3.6.3/flexget/ui/v2/dist/assets/db4a2a231f52e497c0191e8966b0ee58.woff2`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin.5c83b88e8b99cf5955dd.js` & `FlexGet-3.6.3/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin.5c83b88e8b99cf5955dd.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin.5c83b88e8b99cf5955dd.js.map` & `FlexGet-3.6.3/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin.5c83b88e8b99cf5955dd.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~SeriesPlugin.82114e5d38c3136caad1.js` & `FlexGet-3.6.3/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~SeriesPlugin.82114e5d38c3136caad1.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~SeriesPlugin.82114e5d38c3136caad1.js.map` & `FlexGet-3.6.3/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~SeriesPlugin.82114e5d38c3136caad1.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~TasksPlugin.17910c3356c98ded086b.js` & `FlexGet-3.6.3/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~TasksPlugin.17910c3356c98ded086b.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~TasksPlugin.17910c3356c98ded086b.js.map` & `FlexGet-3.6.3/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~TasksPlugin.17910c3356c98ded086b.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v2/dist/assets/ebf6d1640ccddb99fb49f73c052c55a8.woff2` & `FlexGet-3.6.3/flexget/ui/v2/dist/assets/ebf6d1640ccddb99fb49f73c052c55a8.woff2`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v2/dist/assets/ef7c6637c68f269a882e73bcb57a7f6a.woff2` & `FlexGet-3.6.3/flexget/ui/v2/dist/assets/ef7c6637c68f269a882e73bcb57a7f6a.woff2`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v2/dist/assets/f8b1df51ba843179fa1cc9b53d58127a.woff2` & `FlexGet-3.6.3/flexget/ui/v2/dist/assets/f8b1df51ba843179fa1cc9b53d58127a.woff2`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v2/dist/assets/f9e8e590b4e0f1ff83469bb2a55b8488.woff` & `FlexGet-3.6.3/flexget/ui/v2/dist/assets/f9e8e590b4e0f1ff83469bb2a55b8488.woff`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v2/dist/assets/fe65b8335ee19dd944289f9ed3178c78.woff` & `FlexGet-3.6.3/flexget/ui/v2/dist/assets/fe65b8335ee19dd944289f9ed3178c78.woff`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v2/dist/assets/main.cce4d52f6988bfadab4f.js` & `FlexGet-3.6.3/flexget/ui/v2/dist/assets/main.cce4d52f6988bfadab4f.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v2/dist/assets/main.cce4d52f6988bfadab4f.js.map` & `FlexGet-3.6.3/flexget/ui/v2/dist/assets/main.cce4d52f6988bfadab4f.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.css` & `FlexGet-3.6.3/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.css`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.css.map` & `FlexGet-3.6.3/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.css.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.js` & `FlexGet-3.6.3/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.js.map` & `FlexGet-3.6.3/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/ui/v2/dist/index.html` & `FlexGet-3.6.3/flexget/ui/v2/dist/index.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/utils/bittorrent.py` & `FlexGet-3.6.3/flexget/utils/bittorrent.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Torrenting utils, mostly for handling bencoding and torrent files."""
 # Torrent decoding is a short fragment from effbot.org. Site copyright says:
 # Test scripts and other short code fragments can be considered as being in the public domain.
 import binascii
 import re
 from contextlib import suppress
-from typing import Any, Callable, Dict, Generator, Iterator, List, Match, Union
+from typing import Any, Callable, Dict, Generator, Iterator, List, Union
 
 from loguru import logger
 
 logger = logger.bind(name='torrent')
 
 # Magic indicator used to quickly recognize torrent files
 TORRENT_RE = re.compile(br'^d\d{1,3}:')
@@ -309,15 +309,15 @@
         trackers = []
         # the spec says, if announce-list present use ONLY that
         # funny iteration because of nesting, ie:
         # [ [ tracker1, tracker2 ], [backup1] ]
         for tl in self.content.get('announce-list', []):
             for t in tl:
                 trackers.append(t)
-        if not self.content.get('announce') in trackers:
+        if self.content.get('announce') not in trackers:
             trackers.append(self.content.get('announce'))
         return trackers
 
     @property
     def info_hash(self) -> str:
         """Return Torrent info hash"""
         import hashlib
```

### Comparing `FlexGet-3.6.2/flexget/utils/cache.py` & `FlexGet-3.6.3/flexget/utils/cache.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/utils/cached_input.py` & `FlexGet-3.6.3/flexget/utils/cached_input.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/utils/database.py` & `FlexGet-3.6.3/flexget/utils/database.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/utils/json.py` & `FlexGet-3.6.3/flexget/utils/json.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/utils/lazy_dict.py` & `FlexGet-3.6.3/flexget/utils/lazy_dict.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/utils/log.py` & `FlexGet-3.6.3/flexget/utils/log.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/utils/parsers/generic.py` & `FlexGet-3.6.3/flexget/utils/parsers/generic.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/utils/parsers/movie.py` & `FlexGet-3.6.3/flexget/utils/parsers/movie.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/utils/parsers/parser.py` & `FlexGet-3.6.3/flexget/utils/parsers/parser.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,36 +8,34 @@
 
     editions = ['dc', 'extended', 'uncut', 'remastered', 'unrated', 'theatrical', 'chrono', 'se']
 
     # TODO: All of the quality related keywords can probably be removed from here, as the quality module handles them
     codecs = ['x264', 'x.264', 'h264', 'h.264', 'XViD']
 
     # lowercase required
-    cutoffs = (
-        [
-            'limited',
-            'xvid',
-            'h264',
-            'x264',
-            'h.264',
-            'x.264',
-            'screener',
-            'unrated',
-            '3d',
-            'extended',
-            'directors',
-            'director\'s',
-            'multisubs',
-            'dubbed',
-            'subbed',
-            'multi',
-        ]
-        + specials
-        + editions
-    )
+    cutoffs = [
+        'limited',
+        'xvid',
+        'h264',
+        'x264',
+        'h.264',
+        'x.264',
+        'screener',
+        'unrated',
+        '3d',
+        'extended',
+        'directors',
+        "director's",
+        'multisubs',
+        'dubbed',
+        'subbed',
+        'multi',
+        *specials,
+        *editions,
+    ]
 
     remove = ['imax']
 
     sounds = ['AC3', 'DD5.1', 'DTS']
 
     @staticmethod
     def re_not_in_word(regexp):
```

### Comparing `FlexGet-3.6.2/flexget/utils/parsers/series.py` & `FlexGet-3.6.3/flexget/utils/parsers/series.py`

 * *Files 0% similar despite different names*

```diff
@@ -262,15 +262,15 @@
         name_end = 0
 
         # regexp name matching
         if not self.name_regexps:
             # if we don't have name_regexps, generate one from the name
             self.name_regexps = ReList(
                 name_to_re(name, self.ignore_prefixes, self)
-                for name in [self.name] + self.alternate_names
+                for name in [self.name, *self.alternate_names]
             )
             # With auto regex generation, the first regex group captures the name
             self.re_from_name = True
         # try all specified regexps on this data
         for name_re in self.name_regexps:
             match = re.search(name_re, self.data)
             if match:
```

### Comparing `FlexGet-3.6.2/flexget/utils/pathscrub.py` & `FlexGet-3.6.3/flexget/utils/pathscrub.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/utils/qualities.py` & `FlexGet-3.6.3/flexget/utils/qualities.py`

 * *Files 5% similar despite different names*

```diff
@@ -85,28 +85,28 @@
             return self.value < other.value
         else:
             raise TypeError(f'Cannot compare {self.type} and {other.type}')
 
     def __add__(self, other):
         if not isinstance(other, int):
             raise TypeError()
-        l = globals().get('_' + self.type + 's')
-        index = l.index(self) + other
-        if index >= len(l):
+        component_list = globals().get('_' + self.type + 's')
+        index = component_list.index(self) + other
+        if index >= len(component_list):
             index = -1
-        return l[index]
+        return component_list[index]
 
     def __sub__(self, other):
         if not isinstance(other, int):
             raise TypeError()
-        l = globals().get('_' + self.type + 's')
-        index = l.index(self) - other
+        component_list = globals().get('_' + self.type + 's')
+        index = component_list.index(self) - other
         if index < 0:
             index = 0
-        return l[index]
+        return component_list[index]
 
     def __repr__(self) -> str:
         return f'<{self.type.title()}(name={self.name},value={self.value})>'
 
     def __str__(self) -> str:
         return self.name
 
@@ -279,15 +279,15 @@
     @classmethod
     def deserialize(cls, data: str, version: int) -> 'Quality':
         return cls(data)
 
     @property
     def _comparator(self) -> List:
         modifier = sum(c.modifier for c in self.components if c.modifier)
-        return [modifier] + self.components
+        return [modifier, *self.components]
 
     def __contains__(self, other):
         if isinstance(other, str):
             other = Quality(other)
         if not other or not self:
             return False
         for cat in ('resolution', 'source', 'audio', 'color_range', 'codec'):
@@ -426,17 +426,15 @@
             other.max,
             other.acceptable,
             other.none_of,
         )
 
     def __hash__(self) -> int:
         return hash(
-            tuple(
-                [self.min, self.max, tuple(sorted(self.acceptable)), tuple(sorted(self.none_of))]
-            )
+            (self.min, self.max, tuple(sorted(self.acceptable)), tuple(sorted(self.none_of)))
         )
 
 
 class Requirements:
     """Represents requirements for allowable qualities. Can determine whether a given Quality passes requirements."""
 
     def __init__(self, req: str = '') -> None:
```

### Comparing `FlexGet-3.6.2/flexget/utils/requests.py` & `FlexGet-3.6.3/flexget/utils/requests.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/utils/serialization.py` & `FlexGet-3.6.3/flexget/utils/serialization.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/flexget/utils/simple_persistence.py` & `FlexGet-3.6.3/flexget/utils/simple_persistence.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,30 +67,30 @@
             try:
                 p = pickle.loads(row['value'])
                 session.execute(
                     table.update()
                     .where(table.c.id == row['id'])
                     .values(json=json.dumps(p, encode_datetime=True))
                 )
-            except Exception as e:
+            except Exception:
                 failures += 1
         if failures > 0:
             logger.error(
                 'Error upgrading {} simple_persistence pickle objects. Some information has been lost.',
                 failures,
             )
         ver = 4
     return ver
 
 
 @event('manager.db_cleanup')
 def db_cleanup(manager, session):
     """Clean up values in the db from tasks which no longer exist."""
     # SKVs not associated with any task use None as task tame
-    existing_tasks = list(manager.tasks) + [None]
+    existing_tasks = [*list(manager.tasks), None]
     session.query(SimpleKeyValue).filter(~SimpleKeyValue.task.in_(existing_tasks)).delete(
         synchronize_session=False
     )
 
 
 class SimpleKeyValue(Base):
     __tablename__ = 'simple_persistence'
```

### Comparing `FlexGet-3.6.2/flexget/utils/sqlalchemy_utils.py` & `FlexGet-3.6.3/flexget/utils/sqlalchemy_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,15 +121,15 @@
     """
     Creates an index on specified `columns` in `table_name`
 
     :param table_name: Name of table to create the index on.
     :param session: Session object which should be used
     :param column_names: The names of the columns that should belong to this index.
     """
-    index_name = '_'.join(['ix', table_name] + list(column_names))
+    index_name = '_'.join(['ix', table_name, *list(column_names)])
     table = table_schema(table_name, session)
     columns = [getattr(table.c, column) for column in column_names]
     try:
         Index(index_name, *columns).create(bind=session.bind)
     except OperationalError:
         logger.opt(exception=True).debug('Error creating index.')
```

### Comparing `FlexGet-3.6.2/flexget/utils/template.py` & `FlexGet-3.6.3/flexget/utils/template.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,14 @@
     if result:
         return result.group(0)
     return ''
 
 
 def filter_formatdate(val, format_str):
     """Returns a string representation of a datetime object according to format string."""
-    encoding = locale.getpreferredencoding()
     if not isinstance(val, (datetime, date, time)):
         return val
     return val.strftime(format_str)
 
 
 def filter_parsedate(val):
     """Attempts to parse a date according to the rules in ISO 8601 and RFC 2822"""
```

### Comparing `FlexGet-3.6.2/flexget/utils/tools.py` & `FlexGet-3.6.3/flexget/utils/tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Contains miscellaneous helpers"""
 import ast
 import copy
 import hashlib
 import locale
 import operator
-import os
 import queue
 import re
 import sys
 import weakref
 from collections import OrderedDict, defaultdict
 from collections.abc import MutableMapping
 from datetime import datetime, timedelta
```

### Comparing `FlexGet-3.6.2/flexget/webserver.py` & `FlexGet-3.6.3/flexget/webserver.py`

 * *Files 0% similar despite different names*

```diff
@@ -171,15 +171,15 @@
                 base_url=self.base_url,
             )
         threading.Thread.start(self)
 
     def _start_server(self):
         # Mount the WSGI callable object (app) on the root directory
         cherrypy.tree.graft(_default_app, '/')
-        for path, (registered_app, name) in _app_register.items():
+        for path, (registered_app, _name) in _app_register.items():
             cherrypy.tree.graft(registered_app, self.base_url + path)
 
         cherrypy.log.error_log.propagate = False
         cherrypy.log.access_log.propagate = False
 
         # Set the configuration of the web server
         cherrypy.config.update(
```

### Comparing `FlexGet-3.6.2/pyproject.toml` & `FlexGet-3.6.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -91,21 +91,20 @@
 [tool.poetry.group.dev.dependencies]
 black = ">=18.9b0"
 build = ">=0.9.0"
 click = ">=8.1.3"
 codacy-coverage = ">=1.2.18"
 coverage = ">=6.0"
 gitpython = ">=3.1.18"
-isort = ">=5.5.1"
 pre-commit = ">=2.9.0"
-pylint = ">=2.6.0"
 pytest-cov = ">=3.0.0"
 pytest-runner = "^6.0.0"
 pytest-xdist = ">=2.4.0"
 pytest = ">=6.2.4"
+ruff = ">=0.0.261"
 sphinx = ">=5.0.0"
 sqlalchemy-stubs = "^0.4"
 twine = ">=3.6.0"
 vcrpy = ">=4.1.1"
 
 [tool.poetry.group.plugin-test.dependencies]
 # These are optional dependencies for plugins that have tests in the test suite
@@ -147,14 +146,23 @@
     | \.idea
     | dist
     | flexget/ui
   )/
 )
 '''
 
-[tool.isort]
-profile = 'black'
-line_length = 99
-known_first_party = ['flexget']
+[tool.ruff]
+line-length = 99
+select = ["C4", "E", "F", "I", "ISC", "PLE", "RUF", "UP"]
+
+ignore = [
+    "E501",  # We leave line length up to black
+    "E711", "E712",  # Comparisons to True/False/None are valid for sqlalchemy
+    "PLE1205",  # Thinks we are using stdlib logging rather than loguru
+    "RUF001",  # Some of these ambiguous unicode are in tests on purpose
+]
+
+[tool.ruff.isort]
+known-first-party = ['flexget']
 
 [tool.mypy]
 plugins = ["sqlmypy"]
```

### Comparing `FlexGet-3.6.2/requirements-docker.txt` & `FlexGet-3.6.3/requirements-docker.txt`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.2/requirements.txt` & `FlexGet-3.6.3/requirements.txt`

 * *Files identical despite different names*

