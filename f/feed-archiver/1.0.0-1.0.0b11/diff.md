# Comparing `tmp/feed-archiver-1.0.0.tar.gz` & `tmp/feed-archiver-1.0.0b11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feed-archiver-1.0.0.tar", last modified: Fri Dec 16 13:59:03 2022, max compression
+gzip compressed data, was "feed-archiver-1.0.0b11.tar", last modified: Sat Apr 15 21:33:28 2023, max compression
```

## Comparing `feed-archiver-1.0.0.tar` & `feed-archiver-1.0.0b11.tar`

### file list

```diff
@@ -1,186 +1,251 @@
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2022-12-16 13:59:03.807445 feed-archiver-1.0.0/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      322 2022-12-16 13:55:39.000000 feed-archiver-1.0.0/.dir-locals.el.in
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1700 2022-12-16 13:55:39.000000 feed-archiver-1.0.0/.dockerignore
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      869 2022-12-16 13:55:39.000000 feed-archiver-1.0.0/.env.in
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2022-12-16 13:59:03.781443 feed-archiver-1.0.0/.github/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2022-12-16 13:59:03.793444 feed-archiver-1.0.0/.github/workflows/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     4236 2022-12-16 13:55:39.000000 feed-archiver-1.0.0/.github/workflows/ci-cd.yml
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1700 2022-12-16 13:55:39.000000 feed-archiver-1.0.0/.gitignore
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2695 2022-12-16 13:55:39.000000 feed-archiver-1.0.0/.gitlab-ci.yml
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      555 2022-12-16 13:55:39.000000 feed-archiver-1.0.0/.pre-commit-config.yaml
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3460 2022-12-16 13:55:39.000000 feed-archiver-1.0.0/CONTRIBUTING.rst
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1820 2022-12-16 13:55:39.000000 feed-archiver-1.0.0/Dockerfile
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2393 2022-12-16 13:55:39.000000 feed-archiver-1.0.0/Dockerfile.devel
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1081 2022-12-16 13:55:39.000000 feed-archiver-1.0.0/LICENSE
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    24908 2022-12-16 13:55:39.000000 feed-archiver-1.0.0/Makefile
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1365 2022-12-16 13:57:28.000000 feed-archiver-1.0.0/NEWS.rst
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)    19411 2022-12-16 13:59:03.807445 feed-archiver-1.0.0/PKG-INFO
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    18531 2022-12-16 13:55:39.000000 feed-archiver-1.0.0/README.rst
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3086 2022-12-16 13:55:39.000000 feed-archiver-1.0.0/TODO.rst
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2022-12-16 13:59:03.793444 feed-archiver-1.0.0/bin/
--rwxrwxrwx   0 feed-archiver  (1001) feed-archiver  (1001)      905 2022-12-16 13:55:39.000000 feed-archiver-1.0.0/bin/entrypoint
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3430 2022-12-16 13:55:39.000000 feed-archiver-1.0.0/docker-compose.override.yml
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1420 2022-12-16 13:55:39.000000 feed-archiver-1.0.0/docker-compose.yml
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2022-12-16 13:59:03.794444 feed-archiver-1.0.0/home/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       65 2022-12-16 13:55:39.000000 feed-archiver-1.0.0/home/.gitignore
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      327 2022-12-16 13:55:39.000000 feed-archiver-1.0.0/home/.pypirc.in
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2022-12-16 13:59:03.781443 feed-archiver-1.0.0/nginx/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2022-12-16 13:59:03.794444 feed-archiver-1.0.0/nginx/templates/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1064 2022-12-16 13:55:39.000000 feed-archiver-1.0.0/nginx/templates/default.conf.template
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2135 2022-12-16 13:57:28.000000 feed-archiver-1.0.0/pyproject.toml
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2680 2022-12-16 13:55:39.000000 feed-archiver-1.0.0/requirements-build.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      766 2022-12-16 13:55:39.000000 feed-archiver-1.0.0/requirements-build.txt.in
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     4543 2022-12-16 13:55:39.000000 feed-archiver-1.0.0/requirements-devel.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      833 2022-12-16 13:57:28.000000 feed-archiver-1.0.0/requirements.txt
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2022-12-16 13:59:03.794444 feed-archiver-1.0.0/server/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3963 2022-12-16 13:55:39.000000 feed-archiver-1.0.0/server/docker-compose.yml
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1867 2022-12-16 13:59:03.808445 feed-archiver-1.0.0/setup.cfg
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2022-12-16 13:59:03.782443 feed-archiver-1.0.0/src/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2022-12-16 13:59:03.795444 feed-archiver-1.0.0/src/feed_archiver.egg-info/
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)    19411 2022-12-16 13:59:03.000000 feed-archiver-1.0.0/src/feed_archiver.egg-info/PKG-INFO
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)     5700 2022-12-16 13:59:03.000000 feed-archiver-1.0.0/src/feed_archiver.egg-info/SOURCES.txt
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)        1 2022-12-16 13:59:03.000000 feed-archiver-1.0.0/src/feed_archiver.egg-info/dependency_links.txt
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)      270 2022-12-16 13:59:03.000000 feed-archiver-1.0.0/src/feed_archiver.egg-info/entry_points.txt
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)      266 2022-12-16 13:59:03.000000 feed-archiver-1.0.0/src/feed_archiver.egg-info/requires.txt
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)       13 2022-12-16 13:59:03.000000 feed-archiver-1.0.0/src/feed_archiver.egg-info/top_level.txt
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2022-12-16 13:59:03.796444 feed-archiver-1.0.0/src/feedarchiver/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     4155 2022-12-16 13:55:39.000000 feed-archiver-1.0.0/src/feedarchiver/__init__.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      212 2022-12-16 13:55:39.000000 feed-archiver-1.0.0/src/feedarchiver/__main__.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     9865 2022-12-16 13:55:39.000000 feed-archiver-1.0.0/src/feedarchiver/archive.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    29693 2022-12-16 13:55:39.000000 feed-archiver-1.0.0/src/feedarchiver/feed.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     7029 2022-12-16 13:55:39.000000 feed-archiver-1.0.0/src/feedarchiver/formats.py
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2022-12-16 13:59:03.797444 feed-archiver-1.0.0/src/feedarchiver/linkpaths/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3448 2022-12-16 13:55:39.000000 feed-archiver-1.0.0/src/feedarchiver/linkpaths/__init__.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     7839 2022-12-16 13:55:39.000000 feed-archiver-1.0.0/src/feedarchiver/linkpaths/servarr.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1907 2022-12-16 13:55:39.000000 feed-archiver-1.0.0/src/feedarchiver/linkpaths/template.py
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2022-12-16 13:59:03.797444 feed-archiver-1.0.0/src/feedarchiver/newsfragments/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       91 2022-12-16 13:55:39.000000 feed-archiver-1.0.0/src/feedarchiver/newsfragments/.gitignore
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2022-12-16 13:59:03.798444 feed-archiver-1.0.0/src/feedarchiver/tests/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     9171 2022-12-16 13:55:39.000000 feed-archiver-1.0.0/src/feedarchiver/tests/__init__.py
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2022-12-16 13:59:03.782443 feed-archiver-1.0.0/src/feedarchiver/tests/archives/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2022-12-16 13:59:03.798444 feed-archiver-1.0.0/src/feedarchiver/tests/archives/downloads/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      872 2022-12-16 13:55:39.000000 feed-archiver-1.0.0/src/feedarchiver/tests/archives/downloads/.feed-archiver.yml
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2022-12-16 13:59:03.798444 feed-archiver-1.0.0/src/feedarchiver/tests/archives/end-to-end/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      891 2022-12-16 13:55:39.000000 feed-archiver-1.0.0/src/feedarchiver/tests/archives/end-to-end/.feed-archiver.yml.in
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2022-12-16 13:59:03.799444 feed-archiver-1.0.0/src/feedarchiver/tests/archives/simple/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      228 2022-12-16 13:55:39.000000 feed-archiver-1.0.0/src/feedarchiver/tests/archives/simple/.feed-archiver.yml
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2022-12-16 13:59:03.784443 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2022-12-16 13:59:03.783443 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/downloads/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2022-12-16 13:59:03.783443 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/downloads/orig/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2022-12-16 13:59:03.783443 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/downloads/orig/http/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2022-12-16 13:59:03.783443 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2022-12-16 13:59:03.783443 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2022-12-16 13:59:03.799444 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       83 2022-12-16 13:55:39.000000 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/episode%3Fapikey=secret%26seriesId=7
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      112 2022-12-16 13:55:39.000000 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/episodeFile%3Fapikey=secret%26seriesId=7
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2022-12-16 13:59:03.799444 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/series/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       91 2022-12-16 13:55:39.000000 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/series/7%3Fapikey=secret
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      105 2022-12-16 13:55:39.000000 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/series%3Fapikey=secret
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2022-12-16 13:59:03.784443 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/downloads/orig/https/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2022-12-16 13:59:03.783443 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2022-12-16 13:59:03.800444 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/media/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 2022-12-16 13:55:39.000000 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/media/common-id.mp3
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 2022-12-16 13:55:39.000000 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/media/el-ni%25C3%25B1o.mp3
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2022-12-16 13:59:03.784443 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2022-12-16 13:59:03.800444 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 2022-12-16 13:55:39.000000 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/common-id.mp3
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2022-12-16 13:59:03.784443 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2022-12-16 13:59:03.801444 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 2022-12-16 13:55:39.000000 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/download
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3435 2022-12-16 13:55:39.000000 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/el-ni%25C3%25B1o.png
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2022-12-16 13:55:39.000000 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/index.html
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2022-12-16 13:59:03.801444 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/fred-episode-title/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 2022-12-16 13:55:39.000000 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/fred-episode-title/download
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     4031 2022-12-16 13:55:39.000000 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/feed.rss
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3435 2022-12-16 13:55:39.000000 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/image.png
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2022-12-16 13:55:39.000000 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/index.html
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2022-12-16 13:59:03.788443 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2022-12-16 13:59:03.785443 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/added-item/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2022-12-16 13:59:03.784443 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/added-item/http/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2022-12-16 13:59:03.801444 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2022-12-16 13:59:03.785443 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2022-12-16 13:59:03.802444 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2022-12-16 13:55:39.000000 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/1
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2022-12-16 13:55:39.000000 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/2
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2022-12-16 13:55:39.000000 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/3
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2022-12-16 13:55:39.000000 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/main.html
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2022-12-16 13:59:03.785443 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/added-item/https/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2022-12-16 13:59:03.785443 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/added-item/https/foo-username%3Asecret@grault.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2022-12-16 13:59:03.802444 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/added-item/https/foo-username%3Asecret@grault.example.com/feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1186 2022-12-16 13:55:39.000000 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/added-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2022-12-16 13:59:03.785443 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/added-item/https/waldo.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2022-12-16 13:59:03.802444 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/added-item/https/waldo.example.com/feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1102 2022-12-16 13:55:39.000000 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/added-item/https/waldo.example.com/feeds/waldo
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2022-12-16 13:59:03.786443 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/empty/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2022-12-16 13:59:03.785443 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/empty/http/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2022-12-16 13:59:03.802444 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2022-12-16 13:59:03.786443 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2022-12-16 13:59:03.803444 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2022-12-16 13:55:39.000000 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/1
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2022-12-16 13:55:39.000000 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/2
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2022-12-16 13:55:39.000000 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/3
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2022-12-16 13:55:39.000000 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/main.html
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2022-12-16 13:59:03.786443 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/empty/https/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2022-12-16 13:59:03.786443 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/empty/https/foo-username%3Asecret@grault.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2022-12-16 13:59:03.803444 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/empty/https/foo-username%3Asecret@grault.example.com/feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       92 2022-12-16 13:55:39.000000 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/empty/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2022-12-16 13:59:03.786443 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/empty/https/waldo.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2022-12-16 13:59:03.803444 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/empty/https/waldo.example.com/feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1102 2022-12-16 13:55:39.000000 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/empty/https/waldo.example.com/feeds/waldo
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2022-12-16 13:59:03.787443 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/orig/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2022-12-16 13:59:03.786443 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/orig/http/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2022-12-16 13:59:03.804444 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2022-12-16 13:59:03.787443 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2022-12-16 13:59:03.804444 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2022-12-16 13:55:39.000000 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/1
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2022-12-16 13:55:39.000000 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/2
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2022-12-16 13:55:39.000000 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/3
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2022-12-16 13:55:39.000000 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/main.html
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2022-12-16 13:59:03.787443 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/orig/https/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2022-12-16 13:59:03.787443 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/orig/https/foo-username%3Asecret@grault.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2022-12-16 13:59:03.804444 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/orig/https/foo-username%3Asecret@grault.example.com/feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      831 2022-12-16 13:55:39.000000 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/orig/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2022-12-16 13:59:03.787443 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/orig/https/waldo.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2022-12-16 13:59:03.804444 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/orig/https/waldo.example.com/feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1102 2022-12-16 13:55:39.000000 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/orig/https/waldo.example.com/feeds/waldo
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2022-12-16 13:59:03.788443 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/removed-item/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2022-12-16 13:59:03.787443 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/removed-item/http/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2022-12-16 13:59:03.805444 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2022-12-16 13:59:03.788443 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2022-12-16 13:59:03.805444 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2022-12-16 13:55:39.000000 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/1
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2022-12-16 13:55:39.000000 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/2
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2022-12-16 13:55:39.000000 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/3
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2022-12-16 13:55:39.000000 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/main.html
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2022-12-16 13:59:03.788443 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/removed-item/https/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2022-12-16 13:59:03.788443 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/removed-item/https/foo-username%3Asecret@grault.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2022-12-16 13:59:03.805444 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/removed-item/https/foo-username%3Asecret@grault.example.com/feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      841 2022-12-16 13:55:39.000000 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/removed-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2022-12-16 13:59:03.788443 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/removed-item/https/waldo.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2022-12-16 13:59:03.805444 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/removed-item/https/waldo.example.com/feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1102 2022-12-16 13:55:39.000000 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/removed-item/https/waldo.example.com/feeds/waldo
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2022-12-16 13:59:03.789443 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/reordered-item/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2022-12-16 13:59:03.788443 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/reordered-item/http/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2022-12-16 13:59:03.806445 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2022-12-16 13:59:03.789443 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2022-12-16 13:59:03.806445 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2022-12-16 13:55:39.000000 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/1
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2022-12-16 13:55:39.000000 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/2
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2022-12-16 13:55:39.000000 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/3
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2022-12-16 13:55:39.000000 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/main.html
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2022-12-16 13:59:03.789443 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/reordered-item/https/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2022-12-16 13:59:03.789443 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/reordered-item/https/foo-username%3Asecret@grault.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2022-12-16 13:59:03.806445 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/reordered-item/https/foo-username%3Asecret@grault.example.com/feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1550 2022-12-16 13:55:39.000000 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/reordered-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2022-12-16 13:59:03.789443 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/reordered-item/https/waldo.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2022-12-16 13:59:03.807445 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/reordered-item/https/waldo.example.com/feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1102 2022-12-16 13:55:39.000000 feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/reordered-item/https/waldo.example.com/feeds/waldo
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2208 2022-12-16 13:55:39.000000 feed-archiver-1.0.0/src/feedarchiver/tests/test_archive.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3790 2022-12-16 13:55:39.000000 feed-archiver-1.0.0/src/feedarchiver/tests/test_cli.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    10891 2022-12-16 13:55:39.000000 feed-archiver-1.0.0/src/feedarchiver/tests/test_download.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    13867 2022-12-16 13:55:39.000000 feed-archiver-1.0.0/src/feedarchiver/tests/test_feed.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2078 2022-12-16 13:55:39.000000 feed-archiver-1.0.0/src/feedarchiver/tests/test_linking.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2167 2022-12-16 13:55:39.000000 feed-archiver-1.0.0/src/feedarchiver/tests/test_urls.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     5383 2022-12-16 13:55:39.000000 feed-archiver-1.0.0/src/feedarchiver/utils.py
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)      176 2022-12-16 13:59:03.000000 feed-archiver-1.0.0/src/feedarchiver/version.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2047 2022-12-16 13:55:39.000000 feed-archiver-1.0.0/tox.ini
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.837655 feed-archiver-1.0.0b11/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      543 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/.dir-locals.el.in
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1661 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/.dockerignore
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1115 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/.env.in
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/.github/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.833655 feed-archiver-1.0.0b11/.github/workflows/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     4582 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/.github/workflows/build-test.yml
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1661 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/.gitignore
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     5189 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/.gitlab-ci.yml
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      779 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/.pre-commit-config.yaml
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2442 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/.prospector.yaml
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     4121 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/CONTRIBUTING.rst
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2482 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/Dockerfile
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2747 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/Dockerfile.devel
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1081 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/LICENSE
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    60978 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/Makefile
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      205 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/NEWS-VERSION.rst
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3447 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/NEWS.rst
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)    22912 2023-04-15 21:33:28.837655 feed-archiver-1.0.0b11/PKG-INFO
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    21851 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/README.rst
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3876 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/TODO.rst
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.833655 feed-archiver-1.0.0b11/bin/
+-rwxrwxrwx   0 feed-archiver  (1001) feed-archiver  (1001)     2792 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/bin/cz-check-bump
+-rwxrwxrwx   0 feed-archiver  (1001) feed-archiver  (1001)      936 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/bin/entrypoint
+-rwxrwxrwx   0 feed-archiver  (1001) feed-archiver  (1001)     1101 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/bin/get-base-version
+-rwxrwxrwx   0 feed-archiver  (1001) feed-archiver  (1001)      321 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/bin/hadolint
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.833655 feed-archiver-1.0.0b11/build-host/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2002 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/build-host/Dockerfile
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1476 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/build-host/Makefile
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      746 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/build-host/README.rst
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.833655 feed-archiver-1.0.0b11/build-host/bin/
+-rwxrwxrwx   0 feed-archiver  (1001) feed-archiver  (1001)     2047 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/build-host/bin/entrypoint
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      731 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/build-host/requirements-py310.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      674 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/build-host/requirements-py311.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      948 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/build-host/requirements-py37.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      729 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/build-host/requirements-py38.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      729 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/build-host/requirements-py39.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)        4 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/build-host/requirements.txt.in
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.833655 feed-archiver-1.0.0b11/dist/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      122 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/dist/.gitignore
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      954 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/docker-compose-servarr.yml
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     5675 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/docker-compose.override.yml
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      927 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/docker-compose.yml
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.833655 feed-archiver-1.0.0b11/gitlab-runner/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       46 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/gitlab-runner/.gitignore
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.833655 feed-archiver-1.0.0b11/gitlab-runner/config/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1323 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/gitlab-runner/config/config.toml.in
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.833655 feed-archiver-1.0.0b11/home/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       64 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/home/.gitignore
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      327 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/home/.pypirc.in
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      111 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/link-fallbacks.feature.rst
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/nginx/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.833655 feed-archiver-1.0.0b11/nginx/templates/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1086 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/nginx/templates/default.conf.template
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2941 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/pyproject.toml
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.833655 feed-archiver-1.0.0b11/requirements/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      578 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/requirements/build.txt.in
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.833655 feed-archiver-1.0.0b11/requirements/py310/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2414 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/requirements/py310/build.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     6331 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/requirements/py310/devel.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1183 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/requirements/py310/user.txt
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.833655 feed-archiver-1.0.0b11/requirements/py311/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2414 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/requirements/py311/build.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     6082 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/requirements/py311/devel.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1183 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/requirements/py311/user.txt
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.833655 feed-archiver-1.0.0b11/requirements/py37/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2645 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/requirements/py37/build.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     7030 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/requirements/py37/devel.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1530 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/requirements/py37/user.txt
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.833655 feed-archiver-1.0.0b11/requirements/py38/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2515 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/requirements/py38/build.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     6371 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/requirements/py38/devel.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1181 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/requirements/py38/user.txt
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.833655 feed-archiver-1.0.0b11/requirements/py39/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2412 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/requirements/py39/build.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     6358 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/requirements/py39/devel.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1181 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/requirements/py39/user.txt
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.833655 feed-archiver-1.0.0b11/server/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     4397 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/server/docker-compose.yml
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2120 2023-04-15 21:33:28.837655 feed-archiver-1.0.0b11/setup.cfg
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.833655 feed-archiver-1.0.0b11/src/feed_archiver.egg-info/
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)    22912 2023-04-15 21:33:28.000000 feed-archiver-1.0.0b11/src/feed_archiver.egg-info/PKG-INFO
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)     7365 2023-04-15 21:33:28.000000 feed-archiver-1.0.0b11/src/feed_archiver.egg-info/SOURCES.txt
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)        1 2023-04-15 21:33:28.000000 feed-archiver-1.0.0b11/src/feed_archiver.egg-info/dependency_links.txt
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)      277 2023-04-15 21:33:28.000000 feed-archiver-1.0.0b11/src/feed_archiver.egg-info/entry_points.txt
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)      345 2023-04-15 21:33:28.000000 feed-archiver-1.0.0b11/src/feed_archiver.egg-info/requires.txt
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)       13 2023-04-15 21:33:28.000000 feed-archiver-1.0.0b11/src/feed_archiver.egg-info/top_level.txt
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.833655 feed-archiver-1.0.0b11/src/feedarchiver/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     5287 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/src/feedarchiver/__init__.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      201 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/__main__.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    11802 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/src/feedarchiver/archive.py
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.833655 feed-archiver-1.0.0b11/src/feedarchiver/enclosures/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3371 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/src/feedarchiver/enclosures/__init__.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     8155 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/src/feedarchiver/enclosures/servarr.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1968 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/src/feedarchiver/enclosures/template.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    34925 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/src/feedarchiver/feed.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     7074 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/src/feedarchiver/formats.py
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.833655 feed-archiver-1.0.0b11/src/feedarchiver/newsfragments/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       91 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/newsfragments/.gitignore
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       58 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/src/feedarchiver/newsfragments/request-timeouts.fix.rst
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.833655 feed-archiver-1.0.0b11/src/feedarchiver/tests/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     9888 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/__init__.py
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/archives/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.833655 feed-archiver-1.0.0b11/src/feedarchiver/tests/archives/downloads/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1349 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/archives/downloads/.feed-archiver.yml
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.833655 feed-archiver-1.0.0b11/src/feedarchiver/tests/archives/empty/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       32 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/archives/empty/.gitignore
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.837655 feed-archiver-1.0.0b11/src/feedarchiver/tests/archives/empty-feeds/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       60 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/archives/empty-feeds/.feed-archiver.yml
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.837655 feed-archiver-1.0.0b11/src/feedarchiver/tests/archives/empty-items/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      337 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/archives/empty-items/.feed-archiver.yml
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.837655 feed-archiver-1.0.0b11/src/feedarchiver/tests/archives/end-to-end/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      962 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/archives/end-to-end/.feed-archiver.yml.in
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.837655 feed-archiver-1.0.0b11/src/feedarchiver/tests/archives/relink/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      936 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/archives/relink/.feed-archiver.yml
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.837655 feed-archiver-1.0.0b11/src/feedarchiver/tests/archives/relink-wo-suffix/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      932 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/archives/relink-wo-suffix/.feed-archiver.yml
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.837655 feed-archiver-1.0.0b11/src/feedarchiver/tests/archives/simple/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      228 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/archives/simple/.feed-archiver.yml
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/http/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.837655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      243 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/episode%3Fapikey=secret%26seriesId=7
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      224 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/episodeFile%3Fapikey=secret%26seriesId=7
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.837655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/series/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       91 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/series/7%3Fapikey=secret
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      105 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/series%3Fapikey=secret
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/https/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.837655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/media/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/media/common-id.mp3
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/media/el-ni%25C3%25B1o.mp3
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.837655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/common-id.mp3
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.837655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/bah-episode-title/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/bah-episode-title/download.mp3
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/bah-episode-title/index.html
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.837655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/download
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3435 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/el-ni%25C3%25B1o.png
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/index.html
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.837655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/fred-episode-title/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/fred-episode-title/download
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.837655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/garply-bonus-episode/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/garply-bonus-episode/download.mp3
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     5617 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/feed.rss
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3435 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/image.png
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/index.html
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/empty-items/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/empty-items/orig/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/empty-items/orig/https/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/empty-items/orig/https/foo.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.837655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/empty-items/orig/https/foo.example.com/podcast/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      405 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/empty-items/orig/https/foo.example.com/podcast/empty.rss
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/added-item/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/added-item/http/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.837655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.837655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/1
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/2
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/3
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/main.html
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/added-item/https/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/added-item/https/foo-username%3Asecret@grault.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.837655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/added-item/https/foo-username%3Asecret@grault.example.com/feeds/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1186 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/added-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/added-item/https/waldo.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.837655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/added-item/https/waldo.example.com/feeds/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1102 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/added-item/https/waldo.example.com/feeds/waldo
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/empty/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/empty/http/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.837655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.837655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/1
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/2
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/3
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/main.html
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/empty/https/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/empty/https/foo-username%3Asecret@grault.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.837655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/empty/https/foo-username%3Asecret@grault.example.com/feeds/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       92 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/empty/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/empty/https/waldo.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.837655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/empty/https/waldo.example.com/feeds/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1102 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/empty/https/waldo.example.com/feeds/waldo
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/orig/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/orig/http/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.837655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.837655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/1
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/2
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/3
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/main.html
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/orig/https/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/orig/https/foo-username%3Asecret@grault.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.837655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/orig/https/foo-username%3Asecret@grault.example.com/feeds/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      831 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/orig/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/orig/https/waldo.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.837655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/orig/https/waldo.example.com/feeds/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1102 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/orig/https/waldo.example.com/feeds/waldo
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/removed-item/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/removed-item/http/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.837655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.837655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/1
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/2
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/3
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/main.html
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/removed-item/https/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/removed-item/https/foo-username%3Asecret@grault.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.837655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/removed-item/https/foo-username%3Asecret@grault.example.com/feeds/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      841 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/removed-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/removed-item/https/waldo.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.837655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/removed-item/https/waldo.example.com/feeds/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1102 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/removed-item/https/waldo.example.com/feeds/waldo
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/reordered-item/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/reordered-item/http/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.837655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.837655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/1
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/2
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/3
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/main.html
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/reordered-item/https/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/reordered-item/https/foo-username%3Asecret@grault.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.837655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/reordered-item/https/foo-username%3Asecret@grault.example.com/feeds/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1550 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/reordered-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/reordered-item/https/waldo.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.837655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/reordered-item/https/waldo.example.com/feeds/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1102 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/reordered-item/https/waldo.example.com/feeds/waldo
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3286 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/test_archive.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     4257 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/test_cli.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    10833 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/test_download.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    15051 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/test_feed.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     7436 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/test_linking.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2165 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/test_urls.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     8147 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/src/feedarchiver/utils.py
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)      163 2023-04-15 21:33:28.000000 feed-archiver-1.0.0b11/src/feedarchiver/version.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3362 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/tox.ini
```

### Comparing `feed-archiver-1.0.0/.dockerignore` & `feed-archiver-1.0.0b11/.dockerignore`

 * *Files 13% similar despite different names*

```diff
@@ -17,24 +17,22 @@
 **/.so
 
 # Distribution / packaging
 .Python
 env/
 build/
 develop-eggs/
-dist/
-/downloads/
+downloads/
 eggs/
 .eggs/
 lib/
 lib64/
 parts/
 sdist/
 var/
-var-*/
 *.egg-info
 **/*.egg-info
 .installed.cfg
 *.egg
 **/.egg
 /src/*/version.py
 
@@ -50,15 +48,14 @@
 pip-log.txt
 pip-delete-this-directory.txt
 
 # Unit test / coverage reports
 htmlcov/
 .tox
 **/.tox
-.tox-*
 .coverage
 .coverage.*
 coverage.*
 .cache
 **/.cache
 nosetests.xml
 pytest-junit.xml
@@ -116,15 +113,14 @@
 .ropeproject
 
 # Emacs editor settings
 /.dir-locals.el
 
 # Project-specific build artifacts
 /README.md
-/NEWS-release.rst
 # Local, development `$ docker compose ...` end-to-end stack
 /src/feedarchiver/tests/archives/end-to-end/*
 !/src/feedarchiver/tests/archives/end-to-end/.feed-archiver.yml.in
 /sonarr
 /server/.htpasswd
 
 # Explicit ignores for the Docker build context.
```

### Comparing `feed-archiver-1.0.0/.env.in` & `feed-archiver-1.0.0b11/.env.in`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 # Make non-default `./docker-compose*.yml` files the default
 # https://pscheit.medium.com/docker-compose-advanced-configuration-541356d121de#9aa6
 COMPOSE_PATH_SEPARATOR=:
-COMPOSE_FILE=./docker-compose.yml:./server/docker-compose.yml:./docker-compose.override.yml
+COMPOSE_FILE=./docker-compose.yml:./docker-compose-servarr.yml:./server/docker-compose.yml:./docker-compose.override.yml
 
 # Capture local values specific to this checkout
+TZ=${TZ}
 PUID=${PUID}
 PGID=${PGID}
 # Absolute path of the git repo checkout, useful where relative paths can't be used
-CHECKOUT_DIR=${PWD}
+CHECKOUT_DIR=${CHECKOUT_DIR}
 
 # Release variables
-DOCKER_USER=merpatterson
+DOCKER_USER=${DOCKER_USER}
 # Best to create and use a token.  Note that the token must have the `admin`/"Read,
 # Write, Delete" scope, aka "ACCESS PERMISSIONS":
 # https://hub.docker.com/settings/security?generateToken=true
 DOCKER_PASS=${DOCKER_PASS}
+# Project host credentials used here and in CI/CD to support local testing/debugging:
+CI_REGISTRY_PASSWORD=${CI_REGISTRY_PASSWORD}
+PROJECT_GITHUB_PAT=${PROJECT_GITHUB_PAT}
 
 # Define common, shared values in one location
 FEED_ARCHIVE=$${__}{CHECKOUT_DIR}/src/feedarchiver/tests/archives/end-to-end
 NGINX_ROOT=$${__}{FEED_ARCHIVE}
+NGINX_PORT=${NGINX_PORT}
```

### Comparing `feed-archiver-1.0.0/.github/workflows/ci-cd.yml` & `feed-archiver-1.0.0b11/.github/workflows/build-test.yml`

 * *Files 22% similar despite different names*

```diff
@@ -1,118 +1,132 @@
-name: "CI/CD"
+name: "Build and Test"
+
+# TEMPLATE: If using GitHub Actions, then add the following secrets to the project:
+# - `CODECOV_TOKEN`:
+#   Add your project to https://app.codecov.io/gl and use the generated token
+# - `DOCKER_PASS`:
+#   A Docker Hub Personal Access Token
+# - `GPG_PASSPHRASE`:
+#   See the comments towards the bottom of the `./Makefile`
+# - `GPG_SIGNING_PRIVATE_KEY`:
+#   See the comments towards the bottom of the `./Makefile`
+# - `PROJECT_GITHUB_PAT`:
+#   A GitHub "Classic" Personal Access Token with scopes: `repo`, `workflow`,
+#   `packages`, and `project`
+# - `PYPI_PASSWORD`:
+#   A PyPI API token
+# - `TEST_PYPI_PASSWORD`:
+#   A PyPI API token
 
 on:
-  # Only run when branches are pushed, and not when tags are pushed, to allow manual
-  # creation of tags to manually control bumped versions:
+  # Only run on branches, not tags:
   # https://github.com/orgs/community/discussions/25615#discussioncomment-3397691
   push:
     branches:
       - "**"
     tags:
       - "!**"
+      # Also run for open pull requests, including when pushed to:
+  pull_request: {}
 
 jobs:
 
-  ci-cd:
+  build-test:
     runs-on: "ubuntu-latest"
+    container:
+      image: "ghcr.io/rpatterson/feed-archiver:build-host"
+      env:
+        PUID: "1001"
+        PGID: "123"
+        CHECKOUT_DIR: "${{ github.workspace }}"
+        # Requires the secrets to be added to GitHub either through the web UI or the
+        # GitHub CLI tool:
+        # https://docs.github.com/en/actions/security-guides/encrypted-secrets#creating-encrypted-secrets-for-a-repository
+        GPG_PASSPHRASE: "${{ secrets.GPG_PASSPHRASE }}"
+        GPG_SIGNING_PRIVATE_KEY: "${{ secrets.GPG_SIGNING_PRIVATE_KEY }}"
+        DOCKER_PASS: "${{ secrets.DOCKER_PASS }}"
+        # Enable the GitHub CLI
+        PROJECT_GITHUB_PAT: "${{ secrets.PROJECT_GITHUB_PAT }}"
+        # Tell the `./Makefile` about GitHub specific environment details:
+        CI_IS_FORK: >-
+          ${{
+            (
+              (
+                (github.repository_owner != 'rpatterson')
+                || (github.event.pull_request.head.repo.owner.login != 'rpatterson')
+              ) && 'true'
+            ) || 'false'
+          }}
+    permissions:
+      packages: "write"
+      checks: "write"
     strategy:
       matrix:
-        python-version: ["3.11"]
+        PYTHON_MINORS:
+          - "3.11"
+          - "3.10"
+          - "3.9"
+          - "3.8"
+          - "3.7"
+    name: "build-test (python${{ matrix.PYTHON_MINORS }})"
     steps:
 
-      # Global set up
-
+      # Shared/common set up:
       - name: "Checkout source from VCS"
         uses: "actions/checkout@master"
-      # https://github.com/actions/checkout/issues/701#issuecomment-1139627817
-      - name: "Fetch versions from VCS"
-        run: "git fetch --tags origin"
-
-      - name: "Add user installs to PATH"
-        run: |
-          echo "$HOME/.local/bin" >> $GITHUB_PATH
-
-      # Cache build artifacts to speed up CI runs
-
-      - name: "Cache tox virtual environments"
-        if: "github.ref != 'refs/heads/master'"
-        uses: "actions/cache@master"
-        env:
-          # Increment to force clearing the cache
-          cache-name: "tox-v1"
-        with:
-          path: |
-            ~/.local
-            ./.tox
-            ./.tox-*
-            ./var/log
-          # Never get a cache hit to force always caching any upgraded dependencies
-          # Use hashFiles to force venv recreation when dependencies change
-          key: >-
-            ${{ env.cache-name }}-${{ runner.os }}-${{ matrix.python-version }}-${{ hashFiles('pyproject.*') }}-${{ hashFiles('setup.*') }}-${{ hashFiles('tox.ini') }}-${{ github.sha }}
-          # Always re-use the cache and then upgrade
-          restore-keys: >-
-            ${{ env.cache-name }}-${{ runner.os }}-${{ matrix.python-version }}-${{ hashFiles('pyproject.*') }}-${{ hashFiles('setup.*') }}-${{ hashFiles('requirements*.txt') }}-${{ hashFiles('tox.ini') }}-
-
-      # Delegate the rest to the `./Makefile` to keep as much portable between CI
-      # platforms
-
-      - name: "Build the container image in which to run the tests"
-        env:
-          GPG_PASSPHRASE: "${{ secrets.GPG_PASSPHRASE }}"
-          GPG_SIGNING_PRIVATE_KEY: "${{ secrets.GPG_SIGNING_PRIVATE_KEY }}"
-          DOCKER_PASS: "${{ secrets.DOCKER_PASS }}"
-        run: "make -e build-bump build-docker"
-
-      - name: "Run the tests and code checks inside the built container"
-        run: "make test-docker"
+      # TODO: Debug stale venv issues and restore cache once fixed
+      - name: "Change checkout owner"
+        # https://stackoverflow.com/a/58474340/624787
+        run: >-
+          chown -R ${PUID}:${PGID} ./ &&
+          git config --global --add safe.directory
+          /__w/${{ github.event.repository.name }}/${{ github.event.repository.name }}
+
+      # Delegate steps agnostic of the CI/CD platform to the `./Makefile`:
+      - name: "Build image and run tests and checks in a container"
+        run: >-
+          entrypoint make -e PYTHON_MINORS=${{ matrix.PYTHON_MINORS }}
+          test-push build-docker-${{ matrix.PYTHON_MINORS }}
+          test-docker-${{ matrix.PYTHON_MINORS }} test-clean
 
-      # Upload build artifacts
+      # Upload build artifacts:
       # https://github.com/actions/upload-artifact#usage
-
       - name: "Archive test suite reports"
         uses: "actions/upload-artifact@master"
         with:
           name: "test-suite-reports"
           path: |
-            ./pytest*
+            ./build/*/pytest*
       # https://github.com/marketplace/actions/test-reporter#example
       - name: "Publish test suite report"
         uses: "dorny/test-reporter@main"
-        if: "success() || failure()"    # run this step even if previous step failed
+        # run this step even if previous step failed
+        if: >-
+          (success() || failure())
+          && (
+            (! github.event.pull_request)
+            || ! (
+              (github.repository_owner == 'rpatterson')
+              && (github.event.pull_request.head.repo.owner.login != 'rpatterson')
+            )
+          )
         with:
-          name: "PyTest Test Suite"
-          path: |
-            ./pytest-junit.xml
+          name: "PyTest Test Suite (python${{ matrix.PYTHON_MINORS }})"
+          path: >-
+            ./build/*/pytest-junit.xml,
+            ./build/*/prospector-xunit.xml
           reporter: "java-junit"
-
       - name: "Archive code coverage reports"
         uses: "actions/upload-artifact@master"
         with:
           name: "code-coverage-reports"
           path: |
-            ./coverage*
-            ./htmlcov
-
+            ./build/*/.coverage*
+            ./build/*/coverage*
+            ./build/*/htmlcov*
       - name: "Archive linter reports"
         uses: "actions/upload-artifact@master"
         with:
           name: "linter-reports"
           path: |
-            ./pylint*
-
-      # Release and publish
-
-      - name: "Bump version and publish release artifacts if on `master`/`develop`"
-        env:
-          CODECOV_TOKEN: "${{ secrets.CODECOV_TOKEN }}"
-          # Enable the GitHub CLI
-          GITHUB_TOKEN: "${{ secrets.GITHUB_TOKEN }}"
-          # Requires the secrets to be added to GitHub either through the web UI or the
-          # GitHub CLI tool:
-          # https://docs.github.com/en/actions/security-guides/encrypted-secrets#creating-encrypted-secrets-for-a-repository
-          GPG_PASSPHRASE: "${{ secrets.GPG_PASSPHRASE }}"
-          GPG_SIGNING_PRIVATE_KEY: "${{ secrets.GPG_SIGNING_PRIVATE_KEY }}"
-          PYPI_PASSWORD: "${{ secrets.PYPI_PASSWORD }}"
-          TEST_PYPI_PASSWORD: "${{ secrets.TEST_PYPI_PASSWORD }}"
-          DOCKER_PASS: "${{ secrets.DOCKER_PASS }}"
-        run: "make -e release"
+            ./build/*/prospector*
+            ./build/*/pylint*
```

### Comparing `feed-archiver-1.0.0/.gitignore` & `feed-archiver-1.0.0b11/.gitignore`

 * *Files 13% similar despite different names*

```diff
@@ -17,24 +17,22 @@
 **/.so
 
 # Distribution / packaging
 .Python
 env/
 build/
 develop-eggs/
-dist/
-/downloads/
+downloads/
 eggs/
 .eggs/
 lib/
 lib64/
 parts/
 sdist/
 var/
-var-*/
 *.egg-info
 **/*.egg-info
 .installed.cfg
 *.egg
 **/.egg
 /src/*/version.py
 
@@ -50,15 +48,14 @@
 pip-log.txt
 pip-delete-this-directory.txt
 
 # Unit test / coverage reports
 htmlcov/
 .tox
 **/.tox
-.tox-*
 .coverage
 .coverage.*
 coverage.*
 .cache
 **/.cache
 nosetests.xml
 pytest-junit.xml
@@ -116,15 +113,14 @@
 .ropeproject
 
 # Emacs editor settings
 /.dir-locals.el
 
 # Project-specific build artifacts
 /README.md
-/NEWS-release.rst
 # Local, development `$ docker compose ...` end-to-end stack
 /src/feedarchiver/tests/archives/end-to-end/*
 !/src/feedarchiver/tests/archives/end-to-end/.feed-archiver.yml.in
 /sonarr
 /server/.htpasswd
 
 # Explicit ignores for the Docker build context.
```

### Comparing `feed-archiver-1.0.0/CONTRIBUTING.rst` & `feed-archiver-1.0.0b11/CONTRIBUTING.rst`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-************
+########################################################################################
 CONTRIBUTING
-************
+########################################################################################
 
 Development requires fairly standard development tools, but ``git`` and ``make`` to
 bootstrap the local development environment.  Once installed, clone the repository::
 
   $ git clone "https://gitlab.com/rpatterson/feed-archiver"
 
 Then hand the rest over to the `Makefile`_ to install the VCS hooks the rest of the set
@@ -12,19 +12,19 @@
 
   $ make
 
 If there's not already `an issue/ticket`_ for the changes you'll be making, create one.
 Regardless, take note of the issue/ticket number, e.g. ``#123``.  Then create a
 branch/fork off of the ``develop`` branch::
 
-  $ git checkout -b feat-123-foo-bar origin/develop
+  $ git switch -c feat-123-foo-bar origin/develop
 
 This project uses `towncrier`_ to manage it's release notes, AKA changelog and thus
 requires at least one `news fragment`_ before merging back into ``develop``.  The VCS
-hooks enforce this when pushing to ``develop`` or ``master``::
+hooks enforce this when pushing to ``develop`` or ``main``::
 
   $ towncrier create 123.feature
 
 From there you can begin writing your tests or making other changes and run the tests to
 check your work.  For reproducibility and to expose clean build issues, the tests can be
 run inside the development container.  This is the command run by the VCS hooks and the
 ``$ make test`` target as well::
@@ -40,37 +40,43 @@
 also runs locally directly on your development host::
 
   $ make test-debug
 
 The ``$ make test`` target also runs the ``$ make format`` target to format code
 according to this project's guidelines and rules.
 
-Once work is finished and all the tests are passing locally, open a PR and push your
-changes there.  Address any issues revealed by any failed CI/CD jobs for your PR
-branch/fork.  Once all CI/CD checks are green, project maintainers can merge your work
-into the ``develop`` branch where CI/CD will publish a pre-release for your changes.
-When the project maintainers think it's time to make a final release with all the
-outstanding work on ``develop``, they can merge ``develop`` into ``master`` and CI/CD
-will then publish a final release including container images and PyPI packages.  Project
-maintainers may test the release process locally using the `Makefile`_::
-
-  $ make build-bump test-docker release
+Contributions should be pushed to feature branches or forks off of the upstream
+``develop`` branch.  Once work is finished and all the tests are passing locally, open a
+merge/pull request (MR) against the upstream ``develop`` branch.  Address any issues
+revealed by any failed CI/CD jobs for your MR.  Once all CI/CD checks are green, project
+maintainers can merge your work where CI/CD will publish a pre-release for your changes
+including container images and PyPI packages.  Contributors should then test the
+pre-release, preferably with as many users and use cases as possible.  Once everything
+looks good and the project maintainers think it's time to make a final release with all
+the outstanding work on ``develop``, they can merge ``develop`` into ``main`` and CI/CD
+will then publish a final release.
 
 The versions for this project's dependencies and development tools are frozen/fixed for
-reproducibility in ``./requirements*.txt``. The `Makefile`_ will update those versions
-as the dependencies change in ``./setup.cfg`` and ``./requirements-build.txt.in``.  Note
+reproducibility in ``./requirements/**.txt``. The `Makefile`_ will update those versions
+as the dependencies change in ``./setup.cfg`` and ``./requirements/build.txt.in``.  Note
 that this means other versions may be updated as the published versions for dependencies
 are updated on remote indexes/registries.  Maintainers can also update all dependencies
 to the latest versions::
 
-  $ make upgrade
+  $ make devel-upgrade
 
 See also `the ./TODO.rst file`_ which lists known bugs and desirable features for which
 contributions are most welcome.
 
+If changes to development processes, such as build or release processes, are required,
+they should be captured in the `Makefile`_.  Similarly, if a development task is
+important enough to include in the documentation, then it's important enough to capture
+in executable form in the `Makefile`_.  See the philosophy commentary at the bottom of
+the `Makefile`_ for guidance on making contributions there.
+
 
 .. _`Python's post-mortem debugger`:
    https://docs.python.org/3/library/pdb.html#pdb.post_mortem
 
 .. _`towncrier`: https://towncrier.readthedocs.io/en/stable/#philosophy
 .. _`news fragment`: https://towncrier.readthedocs.io/en/stable/quickstart.html#creating-news-fragments
```

### Comparing `feed-archiver-1.0.0/Dockerfile` & `feed-archiver-1.0.0b11/build-host/Dockerfile`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,50 @@
-## Container image for use by end users
+## Container image in which to build, test, and release the project
 
-# Stay as close to a vanilla Python environment as possible
-FROM python:3
+# I *want* something to break to let me know if something changes in the latest version
+# of the base image changes something:
+# hadolint ignore=DL3007
+FROM docker:latest
+
+# Install the minimum OS packages needed to use the `./Makefile`.  Also install any OS
+# packages the `./Makefile` might install to optimize build times.
+# hadolint ignore=DL3018
+RUN \
+    apk add --no-cache \
+    "make" \
+    "bash" \
+    "su-exec" \
+    "git" \
+    "gettext" \
+    "py3-pip" \
+    "gnupg" \
+    "curl" \
+    "tar" \
+    "github-cli" \
+    && rm -rf /var/cache/apk/*
 
-ARG VERSION=
+# Find the same home directory even when run as another user, e.g. `root`.
+ENV HOME="/home/runner"
+# Add user installs to PATH
+ENV PATH="${HOME}/.local/bin:${PATH}"
+
+COPY [ "./requirements-py310.txt", "${HOME}/.local/lib/" ]
+RUN mkdir -pv "${HOME}/.local/var/log/" && \
+    pip install --no-cache-dir --user -r "${HOME}/.local/lib/requirements-py310.txt" \
+    >"${HOME}/.local/var/log/feed-archiver-host-install.log"
 
-# Put the `ENTRYPOINT` on the `$PATH`
-RUN apt-get update && apt-get install -y gosu && rm -rf /var/lib/apt/lists/*
 COPY [ "./bin/entrypoint", "/usr/local/bin/entrypoint" ]
-
-WORKDIR "/usr/local/src/feed-archiver/"
-# Install dependencies with fixed versions in a separate layer to optimize build times
-# because this step takes the most time and changes the least frequently.
-COPY [ "./requirements.txt", "./" ]
-RUN pip install --no-cache-dir -r "./requirements.txt"
-# Install this package in the most common/standard Python way while still being able to
-# build the image locally.
-RUN --mount=source=./,target=./,rw,type=bind pip install --no-cache-dir "./"
-
-# Find the same home directory even when run as another user, e.g. `root`.
-ENV HOME="/home/feed-archiver"
-WORKDIR "/home/feed-archiver/"
-ENTRYPOINT [ "entrypoint" ]
-CMD [ "feed-archiver", "update" ]
+ENTRYPOINT [ "docker-entrypoint.sh", "entrypoint" ]
+CMD [ "make", "-e", "build-docker" ]
 
 # https://github.com/opencontainers/image-spec/blob/main/annotations.md#pre-defined-annotation-keys
 LABEL org.opencontainers.image.url="https://gitlab.com/rpatterson/feed-archiver"
 LABEL org.opencontainers.image.documentation="https://gitlab.com/rpatterson/feed-archiver"
 LABEL org.opencontainers.image.source="https://gitlab.com/rpatterson/feed-archiver"
-LABEL org.opencontainers.image.title="feed-archiver"
-LABEL org.opencontainers.image.description="feed archiver foundation or template, CLI console scripts."
+LABEL org.opencontainers.image.title="Feed Archiver Build Host"
+LABEL org.opencontainers.image.description="Feed Archiver build host"
 LABEL org.opencontainers.image.licenses="MIT"
 LABEL org.opencontainers.image.authors="Ross Patterson <me@rpatterson.net>"
 LABEL org.opencontainers.image.vendor="rpatterson.net"
-LABEL org.opencontainers.image.base.name="docker.io/library/python:3"
+LABEL org.opencontainers.image.base.name="docker.io/library/docker:latest"
 # Build-time `LABEL`s
-LABEL org.opencontainers.image.version=${VERSION}
+LABEL org.opencontainers.image.version=0.0.1
```

### Comparing `feed-archiver-1.0.0/LICENSE` & `feed-archiver-1.0.0b11/LICENSE`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0/PKG-INFO` & `feed-archiver-1.0.0b11/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,91 +1,95 @@
 Metadata-Version: 2.1
 Name: feed-archiver
-Version: 1.0.0
+Version: 1.0.0b11
 Summary: Archive the full contents of RSS/Atom syndication feeds including enclosures and assets.
 Home-page: https://gitlab.com/rpatterson/feed-archiver
 Author: Ross Patterson
 Author-email: me@rpatterson.net
 License: MIT
+Keywords: template,structure
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Utilities
-Requires-Python: >=3.10
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: devel
 License-File: LICENSE
 
 ########################################################################################
 feed-archiver
 ########################################################################################
 Archive the full contents of RSS/Atom syndication feeds including enclosures and assets.
 ****************************************************************************************
 
 .. list-table::
    :class: borderless align-right
 
    * - .. figure:: https://img.shields.io/pypi/v/feed-archiver.svg?logo=pypi&label=PyPI&logoColor=gold
-          :alt: PyPI latest release version
-          :target: https://pypi.org/project/feed-archiver/
+	  :alt: PyPI latest release version
+	  :target: https://pypi.org/project/feed-archiver/
        .. figure:: https://img.shields.io/pypi/dm/feed-archiver.svg?color=blue&label=Downloads&logo=pypi&logoColor=gold
-          :alt: PyPI downloads per month
-          :target: https://pypi.org/project/feed-archiver/
+	  :alt: PyPI downloads per month
+	  :target: https://pypi.org/project/feed-archiver/
        .. figure:: https://img.shields.io/pypi/pyversions/feed-archiver.svg?logo=python&label=Python&logoColor=gold
-          :alt: PyPI Python versions
-          :target: https://pypi.org/project/feed-archiver/
+	  :alt: PyPI Python versions
+	  :target: https://pypi.org/project/feed-archiver/
        .. figure:: https://img.shields.io/badge/code%20style-black-000000.svg
-          :alt: Python code style
-          :target: https://github.com/psf/black
+	  :alt: Python code style
+	  :target: https://github.com/psf/black
 
      - .. figure:: https://gitlab.com/rpatterson/feed-archiver/-/badges/release.svg
 	  :alt: GitLab latest release
 	  :target: https://gitlab.com/rpatterson/feed-archiver/-/releases
-       .. figure:: https://gitlab.com/rpatterson/feed-archiver/badges/master/pipeline.svg
+       .. figure:: https://gitlab.com/rpatterson/feed-archiver/badges/main/pipeline.svg
           :alt: GitLab CI/CD pipeline status
-          :target: https://gitlab.com/rpatterson/feed-archiver/-/commits/master
-       .. figure:: https://gitlab.com/rpatterson/feed-archiver/badges/master/coverage.svg
+          :target: https://gitlab.com/rpatterson/feed-archiver/-/commits/main
+       .. figure:: https://gitlab.com/rpatterson/feed-archiver/badges/main/coverage.svg
           :alt: GitLab coverage report
-	  :target: https://gitlab.com/rpatterson/feed-archiver/-/commits/master
+	  :target: https://gitlab.com/rpatterson/feed-archiver/-/commits/main
        .. figure:: https://img.shields.io/gitlab/stars/rpatterson/feed-archiver?gitlab_url=https%3A%2F%2Fgitlab.com&logo=gitlab
 	  :alt: GitLab repo stars
 	  :target: https://gitlab.com/rpatterson/feed-archiver
 
      - .. figure:: https://img.shields.io/github/v/release/rpatterson/feed-archiver?logo=github
 	  :alt: GitHub release (latest SemVer)
 	  :target: https://github.com/rpatterson/feed-archiver/releases
-       .. figure:: https://github.com/rpatterson/feed-archiver/actions/workflows/ci-cd.yml/badge.svg
+       .. figure:: https://github.com/rpatterson/feed-archiver/actions/workflows/build-test.yml/badge.svg
           :alt: GitHub Actions status
-          :target: https://github.com/rpatterson/feed-archiver/
-       .. figure:: https://codecov.io/github/rpatterson/feed-archiver/branch/master/graph/badge.svg?token=GNKVQ8VYOU 
+          :target: https://github.com/rpatterson/feed-archiver/actions/workflows/build-test.yml
+       .. figure:: https://codecov.io/github/rpatterson/feed-archiver/branch/main/graph/badge.svg?token=GNKVQ8VYOU
           :alt: Codecov test coverage
 	  :target: https://codecov.io/github/rpatterson/feed-archiver
        .. figure:: https://img.shields.io/github/stars/rpatterson/feed-archiver?logo=github
 	  :alt: GitHub repo stars
 	  :target: https://github.com/rpatterson/feed-archiver/
 
-     - .. figure:: https://img.shields.io/docker/v/merpatterson/feed-archiver?sort=semver&logo=docker
+     - .. figure:: https://img.shields.io/docker/v/merpatterson/feed-archiver/main?sort=semver&logo=docker
           :alt: Docker Hub image version (latest semver)
           :target: https://hub.docker.com/r/merpatterson/feed-archiver
        .. figure:: https://img.shields.io/docker/pulls/merpatterson/feed-archiver?logo=docker
           :alt: Docker Hub image pulls count
           :target: https://hub.docker.com/r/merpatterson/feed-archiver
        .. figure:: https://img.shields.io/docker/stars/merpatterson/feed-archiver?logo=docker
 	  :alt: Docker Hub stars
-          :target: https://hub.docker.com/r/merpatterson/feed-archiver
+	  :target: https://hub.docker.com/r/merpatterson/feed-archiver
        .. figure:: https://img.shields.io/docker/image-size/merpatterson/feed-archiver?logo=docker
 	  :alt: Docker Hub image size (latest semver)
-          :target: https://hub.docker.com/r/merpatterson/feed-archiver
+	  :target: https://hub.docker.com/r/merpatterson/feed-archiver
 
 The ``$ feed-archiver`` command aims to archive RSS/Atom feeds as fully as possible in
 such a way that the archive can serve (at least) 2 use cases:
 
 #. `Mirror of Feed Enclosures and Assets`_
 
     A mirror of the archived feeds that can be in turn served onto onto feed
@@ -158,34 +162,36 @@
 as `external alternative audio tracks`_ next to the corresponding TV episode video file.
 Multiple linking paths can be configured such that feed item enclosures can be ingested
 in multiple locations in media libraries.
 
 Because syndication feeds may have a number of different ways to correspond to library
 media, this functionality needs to be highly configurable and in order to be highly
 configurable it is more complex to customize to a specific goal.  As such, using this
-feature requires using `a link path plugin`_, or the skill level of a junior developer,
+feature requires using `an enclosure plugin`_, or the skill level of a junior developer,
 or someone who is comfortable reading and interpreting technical documentation, or
 re-using example configurations known to work by others.
 
 
-************
+****************************************************************************************
 Installation
-************
+****************************************************************************************
 
 Install using any tool for installing standard Python 3 distributions such as `pip`_::
 
   $ sudo pip3 install feed-archiver
 
+Optional shell tab completion is available via `argcomplete`_.
+
 Or use `the Docker image`_.  See `the example ./docker-compose.yml file`_ for usage
 details.
 
 
-*****
+****************************************************************************************
 Usage
-*****
+****************************************************************************************
 
 Create a ``./.feed-archiver.yml`` YAML file in a directory to serve as the root
 directory for all feeds to be archived.  The YAML file must have a top-level
 ``defaults`` key whose value is an object defining default or global options.  In
 particular, the ``base-url`` key in that section whose value must be a string which
 defines the external base URL at which the archive is served to clients and is used to
 assemble absolute URLs where relative URLs can't be used.  The file must also have a
@@ -193,201 +199,253 @@
 feeds to archive in this directory.  Each feed object must contain a ``remote-url`` key
 whose value is a string that contains the URL of an individual feed to archive.  In the
 simplest form, this can just be a file like so::
 
   defaults:
     base-url: "https://feeds.example.com"
   feeds:
-    - remote-url:
-	"https://foo-username:secret@grault.example.com/feeds/garply.rss?bar=qux%2Fbaz#corge"
+    - title: "Garply Podcast Title"
+      remote-url: "\
+      https://foo-username:secret@grault.example.com\
+      /feeds/garply.rss?bar=qux%2Fbaz#corge"
   ...
 
-Then simple run the ``$ feed-archiver`` command in that directory to update the archive
-from the current version of the feeds::
+Then run the ``$ feed-archiver`` command in that directory to update the archive from
+the current version of the feeds and write an HTML index with links to the archived
+feeds::
 
   $ cd "/var/www/html/feeds/"
   $ feed-archiver
   INFO:Retrieving feed URL: https://foo-username:secret@grault.example.com/feeds/garply.rss
   ...
+  INFO:Writing HTML index: /var/www/html/feeds/index.html
 
 See also the command-line help for details on options and arguments::
 
-  $ usage: feed-archiver [-h] [archive-dir...]
+  $ feed-archiver --help
+  usage: feed-archiver [-h] [--log-level {CRITICAL,FATAL,ERROR,WARN,WARNING,INFO,DEBUG,NOTSET}]
+		       [--archive-dir [ARCHIVE_DIR]]
+		       {update,relink} ...
 
-  Archive the full contents of RSS/Atom syndication feeds including enclosures and
-  assets.
+  Archive RSS/Atom syndication feeds and their enclosures and assets.
 
   positional arguments:
-    archive-dir  filesystem path to the root of an archive of feeds (default: ./)
-
-  optional arguments:
-    -h, --help  show this help message and exit
-
-  ...
-
-To link feed items into an `alternate hierarchy`_, such as in a media library, add a
-``link-paths`` key to the feed configuration whose value is an list/array of objects
-each defining one alternative path to link to the feed item enclosure.  Any
-``link-paths`` defined in the top-level ``defaults`` key will be used for all feeds.
-Configuration to be shared across multiple ``link-paths`` configurations may be placed
-in the corresponding ``defaults`` / ``plugins`` / ``link-paths`` / ``{plugin_name}``
+    {update,relink}       sub-command
+      update              Request the URL of each feed in the archive and update contents accordingly.
+      relink              Re-link enclosures to the correct locations for the current configuration.
+
+  options:
+    -h, --help            show this help message and exit
+    --log-level {CRITICAL,FATAL,ERROR,WARN,WARNING,INFO,DEBUG,NOTSET}
+			  Select logging verbosity. (default: INFO)
+    --archive-dir [ARCHIVE_DIR], -a [ARCHIVE_DIR]
+			  the archive root directory into which all feeds, their enclosures and assets
+			  will be downloaded (default: .)
+
+To link feed item enclosures into an `alternate hierarchy`_, such as in a media library,
+add a ``enclosures`` key to the feed configuration whose value is an list/array of
+objects each defining one alternative path to link to the feed item enclosure.  Any
+``enclosures`` defined in the top-level ``defaults`` key will be used for all feeds.
+Configuration to be shared across multiple ``enclosures`` configurations may be placed
+in the corresponding ``defaults`` / ``plugins`` / ``enclosures`` / ``{plugin_name}``
 object.  The actual linking of enclosures is delegated to `plugins`_.
 
+When updating the archive from the remote feed URLs using the ``$ feed-archiver
+update`` sub-command, the enclosures of new items are linked as configured.  If the
+``enclosures`` configuration changes or any of the used plugins refer to external
+resources that may change, such as the with the ``sonarr`` plugin when `Sonarr`_ has
+upgraded or renamed the corresponding video files, use the  ``$ feed-archiver relink``
+command to update all existing links.
+
 
 *******
 Plugins
 *******
 
 How feed item enclosures are linked into a media library is delegated to plugins or
-add-ons.  Specifically, the ``plugin`` key in a ``link-paths`` configuration must be a
+add-ons.  Specifically, the ``plugin`` key in a ``enclosures`` configuration must be a
 string which is the name of `a Python entry point`_ registered in the
-``feedarchiver.linkpaths`` group.  The entry point object reference must point to a
-``feedarchiver.linkpaths.LinkPathPlugin`` subclass which accepts the following arguments
+``feedarchiver.enclosures`` group.  The entry point object reference must point to a
+``feedarchiver.enclosures.EnclosurePlugin`` subclass which accepts the following arguments
 when instantiated:
 
 #. ``parent=dict``
 
    The ``feedarchiver.archive.Archive`` if the plugin is configured in ``defaults`` for
    all feeds or the ``feedarchiver.feed.ArchiveFeed`` if defined for a specific feed.
 
 #. ``config=dict``
 
    The Python dictionary object from the de-serialized archive configuration YAML for
-   this specific link path configuration.
+   this specific enclosure configuration.
 
 and whose instances must be callable and accept the following arguments when called:
 
 #. ``archive_feed=feedarchiver.feed.ArchiveFeed``
 
    The object ``feedarchiver`` uses internally to represent an individual feed in the
    archive.
 
-#. ``feed_elem=xml.etree.ElementTree.Element``
+#. ``feed_elem=xml.etree.ElementTree.Element``,
+   ``item_elem=xml.etree.ElementTree.Element``
 
-   The `Python XML element object`_ representing the whole feed.  For RSS this is the
-   ``<channel>`` child element while for Atom this is the root ``<feed>`` element.
+   The `Python XML element object`_ representing the whole feed, for RSS this is the
+   ``<channel>`` child element while for Atom this is the root ``<feed>`` element, and
+   the a similar object representing the specific feed item.
 
-#. ``item_elem=xml.etree.ElementTree.Element``
+#. ``feed_parsed=feedparser.util.FeedParserDict``,
+   ``item_parsed=feedparser.util.FeedParserDict``
 
-   The `Python XML element object`_ representing the specific feed item.
+   The `feedparser`_ object representing the whole feed and the specific feed item.
 
 #. ``url_result=lxml.etree._ElementUnicodeResult``
 
    The `lmxl special string object`_ that contains the URL of the specific enclosure.
    Can be used to access the specific enclosure element.
 
-#. ``basename=str``
+#. ``enclosure_path=pathlib.Path``
 
-  The best guess at the most correct file basename, including the suffix or extension,
-  for the given enclosure.  This suffix takes into account the suffix from the enclosure
-  URL, the ``Content-Type`` header of the response to the enclosure URL request, and
-  finally the value of any ``type`` attribute of the enclosure element XML.
+   The path to the enclosure in the archive as a `Python pathlib.Path`_ object with the
+   best guess at the most correct file basename, including the suffix or extension, for
+   the given enclosure.  This suffix takes into account the suffix from the enclosure
+   URL, the ``Content-Type`` header of the response to the enclosure URL request, and
+   finally the value of any ``type`` attribute of the enclosure element XML.
 
 #. ``match=re.Match``
 
    The `Python regular expression match object`_ if the ``match-pattern`` matched the
    string expanded from the `Python format string`_ in the ``match-string`` key.
    Particularly useful to designate `regular expression groups`_ in the
    ``match-pattern`` and then use the parts of ``match-string`` that matched those
    groups in the format ``template``.  If the ``match-pattern`` doesn't match then the
-   enclosure will not be linked.  If no ``match-string`` is provided a default is used
-   combining the feed title, item title, and enclosure basename with extension::
+   enclosure will not be linked. If there are `symbolic group names`_,
+   e.g. ``(?P<foo_group_name>.*)`` in the pattern, then they are also available by name
+   in the format string, e.g ``{foo_group_name.lower()}``.  If no ``match-string`` is
+   provided a default is used combining the feed title, item title, and enclosure
+   basename with extension::
 
-     {feed_elem.find('title').text.strip()}/{item_elem.find('title').text.strip()}/{basename}
+     {utils.quote_sep(feed_parsed.feed.title).strip()}/{utils.quote_sep(item_parsed.title).strip()}{enclosure_path.suffix}
 
 If the plugin returns a value, it must be a list of strings and will be used as the
 target paths at which to link the enclosure.  Relative paths are resolved against the
 archive root.  These paths are not escaped, so if escaping is needed it must be a part
-of the plugin configuration.  Here's an example ``link-paths`` definition::
+of the plugin configuration. If no plugins link a given enclosure, then any plugins
+whose ``fallback`` key is ``true`` will be applied. Here's an example ``enclosures``
+definition::
 
   defaults:
     base-url: "https://feeds.example.com"
     plugins:
-      link-paths:
-        sonarr:
-          url: "http://localhost:8989"
-          api-key: "????????????????????????????????"
-    link-paths:
-      # Link all feed item enclosures into the media library under the podcasts directory
-      - template: "/media/Library/Music/Podcasts/{feed_elem.find('title').text.strip()}/{item_elem.find('title').text.strip()})/{basename}"
+      enclosures:
+	sonarr:
+	  url: "http://localhost:8989"
+	  api-key: "????????????????????????????????"
+    enclosures:
+      # Link all feed item enclosures into the media library under the podcasts
+      # directory.  Link items into an album directory named by series title if
+      # matching.
+      - template: "\
+	/media/Library/Music/Podcasts\
+	/{utils.quote_sep(feed_parsed.feed.title).strip()}\
+	/{series_title}\
+	/{utils.quote_sep(item_parsed.title).strip()}{enclosure_path.suffix}"
+	match-string: "{utils.quote_sep(item_parsed.title).strip()}"
+	match-pattern: "\
+	(?P<item_title>.+) \\((?P<series_title>.+) \
+	(?P<season_number>[0-9])(?P<episode_numbers>[0-9]+[0-9Ee& -]*)\\)"
+      # Otherwise link into "self-titled" album directories of the same name as the
+      # feed.
+      - template: "\
+        /media/Library/Music/Podcasts\
+        /{utils.quote_sep(feed_parsed.feed.title).strip()}\
+        /{utils.quote_sep(feed_parsed.feed.title).strip()}\
+        /{utils.quote_sep(item_parsed.title).strip()}{enclosure_path.suffix}"
+	fallback: true
   feeds:
-    - remote-url:
-	"https://foo-username:secret@grault.example.com/feeds/garply.rss?bar=qux%2Fbaz#corge"
-      link-paths:
+    - remote-url: "\
+      https://foo-username:secret@grault.example.com\
+      /feeds/garply.rss?bar=qux%2Fbaz#corge"
+      enclosures:
 	# This particular feed is a podcast about a TV series/show.  Link enclosures
 	# from feed items about an individual episode next to the episode video file as
 	# an external audio track using a non-default plugin.
 	- plugin: "sonarr"
-	  match-string: "{item_elem.find('title').text.strip()}"
-	  match-pattern: "(?P<item_title>.+) \\((?P<series_title>.+) (?P<season_number>[0-9])(?P<episode_numbers>[0-9]+[0-9Ee& -]*)\\)"
+	  match-string: "{utils.quote_sep(item_parsed.title).strip()}"
+	  match-pattern: "\
+	  (?P<item_title>.+) \\((?P<series_title>.+) \
+	  (?P<season_number>[0-9])(?P<episode_numbers>[0-9]+[0-9Ee& -]*)\\)"
 	  stem-append: "-garply"
   ...
 
 Default Template Plugin
 =======================
 
 If no ``plugin`` key is specified, the ``template`` plugin is used.  The link
 path config may include the ``template`` key containing a `Python format string`_ which
 will be expanded to determine where the feed item enclosure should be linked to.  The
 default ``template`` is::
 
-  ./Feeds/{feed_elem.find('title').text.strip()}/{item_elem.find('title').text.strip()}/{basename}
+  ./Feeds/{utils.quote_sep(feed_parsed.feed.title).strip()}/{utils.quote_sep(item_parsed.title).strip()}{enclosure_path.suffix}
 
-The format strings may reference any of `the arguments passed into link path plugins`_.
+The format strings may reference any of `the arguments passed into enclosure plugins`_.
 
 Sonarr TV Series Plugin
 =======================
 
-The ``sonarr`` plugin uses values from the link path configuration and/or the ``match``
+The ``sonarr`` plugin uses values from the enclosure configuration and/or the ``match``
 groups to lookup a TV series/show managed by `Sonarr`_, then lookup an episode video
-file that corresponds to the feed item enclosure/content, and link the enclosure/content
-next to that video file.  The ``link-paths`` configuration or ``match`` groups must
-contain:
+file that corresponds to the feed item enclosure, and link the enclosure next to that
+video file.  The ``enclosures`` configuration or ``match`` groups must contain:
 
 - ``url`` and ``api-key`` used to `connect to the Sonarr API`_
 - ``series_id`` or ``series_title`` used to `look up the TV show/series`_, note that
   using ``series_id`` saves on Sonarr API request per update
 - ``season_number`` used to `lookup the episode file`_
 - ``episode_numbers`` used to `lookup the episode file`_, plural to support
   multi-episode files
 
 They may also include:
 
 - ``stem-append`` containing a string to append to the episode file stem before the
-  enclosure/content suffix/extension
+  enclosure suffix/extension
 
 
-************
+****************************************************************************************
 CONTRIBUTING
-************
+****************************************************************************************
 
 NOTE: `This project is hosted on GitLab`_.  There's `a mirror on GitHub`_ but please use
 GitLab for reporting issues, submitting PRs/MRs and any other development or maintenance
 activity.
 
 See `the ./CONTRIBUTING.rst file`_ for more details on how to get started with
 development.
 
 
 .. _alternate hierarchy: `Ingest Feed Enclosures Into Media Libraries`_
-.. _a link path plugin: `Plugins`_
-.. _the arguments passed into link path plugins: `Plugins`_
+.. _an enclosure plugin: `Plugins`_
+.. _the arguments passed into enclosure plugins: `Plugins`_
 
 .. _pip: https://pip.pypa.io/en/stable/installation/
+.. _argcomplete: https://kislyuk.github.io/argcomplete/#installation
 .. _a Python entry point:
    https://packaging.python.org/en/latest/specifications/entry-points/#data-model
 .. _Python format string: https://docs.python.org/3/library/string.html#formatstrings
 .. _Python regular expression match object:
    https://docs.python.org/3/library/re.html#match-objects
 .. _regular expression groups: https://docs.python.org/3/library/re.html#index-17
+.. _symbolic group names: https://docs.python.org/3/library/re.html#index-18
 .. _Python's urllib.parse.quote:
    https://docs.python.org/3/library/urllib.parse.html#urllib.parse.quote
+.. _Python pathlib.path:
+   https://docs.python.org/3/library/pathlib.html#accessing-individual-parts
 .. _Python XML element object:
     https://docs.python.org/3/library/xml.etree.elementtree.html#element-objects
 .. _lmxl special string object: https://lxml.de/xpathxslt.html#xpath-return-values
+.. _feedparser: https://pythonhosted.org/feedparser/index.html
 
 .. _nginx: https://nginx.org/en/docs/
 .. _nginx server_name: https://www.nginx.com/resources/wiki/start/topics/examples/server_blocks/
 
 .. _Jellyfin: https://jellyfin.org/
 .. _external alternative audio tracks:
    https://jellyfin.org/docs/general/server/media/external-audio-files.html
@@ -401,8 +459,8 @@
    https://gitlab.com/rpatterson/feed-archiver/blob/master/docker-compose.yml
 
 .. _`This project is hosted on GitLab`:
    https://gitlab.com/rpatterson/feed-archiver
 .. _`a mirror on GitHub`:
    https://github.com/rpatterson/feed-archiver
 .. _`the ./CONTRIBUTING.rst file`:
-   https://gitlab.com/rpatterson/feed-archiver/blob/master/CONTRIBUTING.rst
+   https://gitlab.com/rpatterson/feed-archiver/blob/main/CONTRIBUTING.rst
```

### Comparing `feed-archiver-1.0.0/README.rst` & `feed-archiver-1.0.0b11/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -4,64 +4,64 @@
 Archive the full contents of RSS/Atom syndication feeds including enclosures and assets.
 ****************************************************************************************
 
 .. list-table::
    :class: borderless align-right
 
    * - .. figure:: https://img.shields.io/pypi/v/feed-archiver.svg?logo=pypi&label=PyPI&logoColor=gold
-          :alt: PyPI latest release version
-          :target: https://pypi.org/project/feed-archiver/
+	  :alt: PyPI latest release version
+	  :target: https://pypi.org/project/feed-archiver/
        .. figure:: https://img.shields.io/pypi/dm/feed-archiver.svg?color=blue&label=Downloads&logo=pypi&logoColor=gold
-          :alt: PyPI downloads per month
-          :target: https://pypi.org/project/feed-archiver/
+	  :alt: PyPI downloads per month
+	  :target: https://pypi.org/project/feed-archiver/
        .. figure:: https://img.shields.io/pypi/pyversions/feed-archiver.svg?logo=python&label=Python&logoColor=gold
-          :alt: PyPI Python versions
-          :target: https://pypi.org/project/feed-archiver/
+	  :alt: PyPI Python versions
+	  :target: https://pypi.org/project/feed-archiver/
        .. figure:: https://img.shields.io/badge/code%20style-black-000000.svg
-          :alt: Python code style
-          :target: https://github.com/psf/black
+	  :alt: Python code style
+	  :target: https://github.com/psf/black
 
      - .. figure:: https://gitlab.com/rpatterson/feed-archiver/-/badges/release.svg
 	  :alt: GitLab latest release
 	  :target: https://gitlab.com/rpatterson/feed-archiver/-/releases
-       .. figure:: https://gitlab.com/rpatterson/feed-archiver/badges/master/pipeline.svg
+       .. figure:: https://gitlab.com/rpatterson/feed-archiver/badges/main/pipeline.svg
           :alt: GitLab CI/CD pipeline status
-          :target: https://gitlab.com/rpatterson/feed-archiver/-/commits/master
-       .. figure:: https://gitlab.com/rpatterson/feed-archiver/badges/master/coverage.svg
+          :target: https://gitlab.com/rpatterson/feed-archiver/-/commits/main
+       .. figure:: https://gitlab.com/rpatterson/feed-archiver/badges/main/coverage.svg
           :alt: GitLab coverage report
-	  :target: https://gitlab.com/rpatterson/feed-archiver/-/commits/master
+	  :target: https://gitlab.com/rpatterson/feed-archiver/-/commits/main
        .. figure:: https://img.shields.io/gitlab/stars/rpatterson/feed-archiver?gitlab_url=https%3A%2F%2Fgitlab.com&logo=gitlab
 	  :alt: GitLab repo stars
 	  :target: https://gitlab.com/rpatterson/feed-archiver
 
      - .. figure:: https://img.shields.io/github/v/release/rpatterson/feed-archiver?logo=github
 	  :alt: GitHub release (latest SemVer)
 	  :target: https://github.com/rpatterson/feed-archiver/releases
-       .. figure:: https://github.com/rpatterson/feed-archiver/actions/workflows/ci-cd.yml/badge.svg
+       .. figure:: https://github.com/rpatterson/feed-archiver/actions/workflows/build-test.yml/badge.svg
           :alt: GitHub Actions status
-          :target: https://github.com/rpatterson/feed-archiver/
-       .. figure:: https://codecov.io/github/rpatterson/feed-archiver/branch/master/graph/badge.svg?token=GNKVQ8VYOU 
+          :target: https://github.com/rpatterson/feed-archiver/actions/workflows/build-test.yml
+       .. figure:: https://codecov.io/github/rpatterson/feed-archiver/branch/main/graph/badge.svg?token=GNKVQ8VYOU
           :alt: Codecov test coverage
 	  :target: https://codecov.io/github/rpatterson/feed-archiver
        .. figure:: https://img.shields.io/github/stars/rpatterson/feed-archiver?logo=github
 	  :alt: GitHub repo stars
 	  :target: https://github.com/rpatterson/feed-archiver/
 
-     - .. figure:: https://img.shields.io/docker/v/merpatterson/feed-archiver?sort=semver&logo=docker
+     - .. figure:: https://img.shields.io/docker/v/merpatterson/feed-archiver/main?sort=semver&logo=docker
           :alt: Docker Hub image version (latest semver)
           :target: https://hub.docker.com/r/merpatterson/feed-archiver
        .. figure:: https://img.shields.io/docker/pulls/merpatterson/feed-archiver?logo=docker
           :alt: Docker Hub image pulls count
           :target: https://hub.docker.com/r/merpatterson/feed-archiver
        .. figure:: https://img.shields.io/docker/stars/merpatterson/feed-archiver?logo=docker
 	  :alt: Docker Hub stars
-          :target: https://hub.docker.com/r/merpatterson/feed-archiver
+	  :target: https://hub.docker.com/r/merpatterson/feed-archiver
        .. figure:: https://img.shields.io/docker/image-size/merpatterson/feed-archiver?logo=docker
 	  :alt: Docker Hub image size (latest semver)
-          :target: https://hub.docker.com/r/merpatterson/feed-archiver
+	  :target: https://hub.docker.com/r/merpatterson/feed-archiver
 
 The ``$ feed-archiver`` command aims to archive RSS/Atom feeds as fully as possible in
 such a way that the archive can serve (at least) 2 use cases:
 
 #. `Mirror of Feed Enclosures and Assets`_
 
     A mirror of the archived feeds that can be in turn served onto onto feed
@@ -134,34 +134,36 @@
 as `external alternative audio tracks`_ next to the corresponding TV episode video file.
 Multiple linking paths can be configured such that feed item enclosures can be ingested
 in multiple locations in media libraries.
 
 Because syndication feeds may have a number of different ways to correspond to library
 media, this functionality needs to be highly configurable and in order to be highly
 configurable it is more complex to customize to a specific goal.  As such, using this
-feature requires using `a link path plugin`_, or the skill level of a junior developer,
+feature requires using `an enclosure plugin`_, or the skill level of a junior developer,
 or someone who is comfortable reading and interpreting technical documentation, or
 re-using example configurations known to work by others.
 
 
-************
+****************************************************************************************
 Installation
-************
+****************************************************************************************
 
 Install using any tool for installing standard Python 3 distributions such as `pip`_::
 
   $ sudo pip3 install feed-archiver
 
+Optional shell tab completion is available via `argcomplete`_.
+
 Or use `the Docker image`_.  See `the example ./docker-compose.yml file`_ for usage
 details.
 
 
-*****
+****************************************************************************************
 Usage
-*****
+****************************************************************************************
 
 Create a ``./.feed-archiver.yml`` YAML file in a directory to serve as the root
 directory for all feeds to be archived.  The YAML file must have a top-level
 ``defaults`` key whose value is an object defining default or global options.  In
 particular, the ``base-url`` key in that section whose value must be a string which
 defines the external base URL at which the archive is served to clients and is used to
 assemble absolute URLs where relative URLs can't be used.  The file must also have a
@@ -169,201 +171,253 @@
 feeds to archive in this directory.  Each feed object must contain a ``remote-url`` key
 whose value is a string that contains the URL of an individual feed to archive.  In the
 simplest form, this can just be a file like so::
 
   defaults:
     base-url: "https://feeds.example.com"
   feeds:
-    - remote-url:
-	"https://foo-username:secret@grault.example.com/feeds/garply.rss?bar=qux%2Fbaz#corge"
+    - title: "Garply Podcast Title"
+      remote-url: "\
+      https://foo-username:secret@grault.example.com\
+      /feeds/garply.rss?bar=qux%2Fbaz#corge"
   ...
 
-Then simple run the ``$ feed-archiver`` command in that directory to update the archive
-from the current version of the feeds::
+Then run the ``$ feed-archiver`` command in that directory to update the archive from
+the current version of the feeds and write an HTML index with links to the archived
+feeds::
 
   $ cd "/var/www/html/feeds/"
   $ feed-archiver
   INFO:Retrieving feed URL: https://foo-username:secret@grault.example.com/feeds/garply.rss
   ...
+  INFO:Writing HTML index: /var/www/html/feeds/index.html
 
 See also the command-line help for details on options and arguments::
 
-  $ usage: feed-archiver [-h] [archive-dir...]
+  $ feed-archiver --help
+  usage: feed-archiver [-h] [--log-level {CRITICAL,FATAL,ERROR,WARN,WARNING,INFO,DEBUG,NOTSET}]
+		       [--archive-dir [ARCHIVE_DIR]]
+		       {update,relink} ...
 
-  Archive the full contents of RSS/Atom syndication feeds including enclosures and
-  assets.
+  Archive RSS/Atom syndication feeds and their enclosures and assets.
 
   positional arguments:
-    archive-dir  filesystem path to the root of an archive of feeds (default: ./)
-
-  optional arguments:
-    -h, --help  show this help message and exit
-
-  ...
-
-To link feed items into an `alternate hierarchy`_, such as in a media library, add a
-``link-paths`` key to the feed configuration whose value is an list/array of objects
-each defining one alternative path to link to the feed item enclosure.  Any
-``link-paths`` defined in the top-level ``defaults`` key will be used for all feeds.
-Configuration to be shared across multiple ``link-paths`` configurations may be placed
-in the corresponding ``defaults`` / ``plugins`` / ``link-paths`` / ``{plugin_name}``
+    {update,relink}       sub-command
+      update              Request the URL of each feed in the archive and update contents accordingly.
+      relink              Re-link enclosures to the correct locations for the current configuration.
+
+  options:
+    -h, --help            show this help message and exit
+    --log-level {CRITICAL,FATAL,ERROR,WARN,WARNING,INFO,DEBUG,NOTSET}
+			  Select logging verbosity. (default: INFO)
+    --archive-dir [ARCHIVE_DIR], -a [ARCHIVE_DIR]
+			  the archive root directory into which all feeds, their enclosures and assets
+			  will be downloaded (default: .)
+
+To link feed item enclosures into an `alternate hierarchy`_, such as in a media library,
+add a ``enclosures`` key to the feed configuration whose value is an list/array of
+objects each defining one alternative path to link to the feed item enclosure.  Any
+``enclosures`` defined in the top-level ``defaults`` key will be used for all feeds.
+Configuration to be shared across multiple ``enclosures`` configurations may be placed
+in the corresponding ``defaults`` / ``plugins`` / ``enclosures`` / ``{plugin_name}``
 object.  The actual linking of enclosures is delegated to `plugins`_.
 
+When updating the archive from the remote feed URLs using the ``$ feed-archiver
+update`` sub-command, the enclosures of new items are linked as configured.  If the
+``enclosures`` configuration changes or any of the used plugins refer to external
+resources that may change, such as the with the ``sonarr`` plugin when `Sonarr`_ has
+upgraded or renamed the corresponding video files, use the  ``$ feed-archiver relink``
+command to update all existing links.
+
 
 *******
 Plugins
 *******
 
 How feed item enclosures are linked into a media library is delegated to plugins or
-add-ons.  Specifically, the ``plugin`` key in a ``link-paths`` configuration must be a
+add-ons.  Specifically, the ``plugin`` key in a ``enclosures`` configuration must be a
 string which is the name of `a Python entry point`_ registered in the
-``feedarchiver.linkpaths`` group.  The entry point object reference must point to a
-``feedarchiver.linkpaths.LinkPathPlugin`` subclass which accepts the following arguments
+``feedarchiver.enclosures`` group.  The entry point object reference must point to a
+``feedarchiver.enclosures.EnclosurePlugin`` subclass which accepts the following arguments
 when instantiated:
 
 #. ``parent=dict``
 
    The ``feedarchiver.archive.Archive`` if the plugin is configured in ``defaults`` for
    all feeds or the ``feedarchiver.feed.ArchiveFeed`` if defined for a specific feed.
 
 #. ``config=dict``
 
    The Python dictionary object from the de-serialized archive configuration YAML for
-   this specific link path configuration.
+   this specific enclosure configuration.
 
 and whose instances must be callable and accept the following arguments when called:
 
 #. ``archive_feed=feedarchiver.feed.ArchiveFeed``
 
    The object ``feedarchiver`` uses internally to represent an individual feed in the
    archive.
 
-#. ``feed_elem=xml.etree.ElementTree.Element``
+#. ``feed_elem=xml.etree.ElementTree.Element``,
+   ``item_elem=xml.etree.ElementTree.Element``
 
-   The `Python XML element object`_ representing the whole feed.  For RSS this is the
-   ``<channel>`` child element while for Atom this is the root ``<feed>`` element.
+   The `Python XML element object`_ representing the whole feed, for RSS this is the
+   ``<channel>`` child element while for Atom this is the root ``<feed>`` element, and
+   the a similar object representing the specific feed item.
 
-#. ``item_elem=xml.etree.ElementTree.Element``
+#. ``feed_parsed=feedparser.util.FeedParserDict``,
+   ``item_parsed=feedparser.util.FeedParserDict``
 
-   The `Python XML element object`_ representing the specific feed item.
+   The `feedparser`_ object representing the whole feed and the specific feed item.
 
 #. ``url_result=lxml.etree._ElementUnicodeResult``
 
    The `lmxl special string object`_ that contains the URL of the specific enclosure.
    Can be used to access the specific enclosure element.
 
-#. ``basename=str``
+#. ``enclosure_path=pathlib.Path``
 
-  The best guess at the most correct file basename, including the suffix or extension,
-  for the given enclosure.  This suffix takes into account the suffix from the enclosure
-  URL, the ``Content-Type`` header of the response to the enclosure URL request, and
-  finally the value of any ``type`` attribute of the enclosure element XML.
+   The path to the enclosure in the archive as a `Python pathlib.Path`_ object with the
+   best guess at the most correct file basename, including the suffix or extension, for
+   the given enclosure.  This suffix takes into account the suffix from the enclosure
+   URL, the ``Content-Type`` header of the response to the enclosure URL request, and
+   finally the value of any ``type`` attribute of the enclosure element XML.
 
 #. ``match=re.Match``
 
    The `Python regular expression match object`_ if the ``match-pattern`` matched the
    string expanded from the `Python format string`_ in the ``match-string`` key.
    Particularly useful to designate `regular expression groups`_ in the
    ``match-pattern`` and then use the parts of ``match-string`` that matched those
    groups in the format ``template``.  If the ``match-pattern`` doesn't match then the
-   enclosure will not be linked.  If no ``match-string`` is provided a default is used
-   combining the feed title, item title, and enclosure basename with extension::
+   enclosure will not be linked. If there are `symbolic group names`_,
+   e.g. ``(?P<foo_group_name>.*)`` in the pattern, then they are also available by name
+   in the format string, e.g ``{foo_group_name.lower()}``.  If no ``match-string`` is
+   provided a default is used combining the feed title, item title, and enclosure
+   basename with extension::
 
-     {feed_elem.find('title').text.strip()}/{item_elem.find('title').text.strip()}/{basename}
+     {utils.quote_sep(feed_parsed.feed.title).strip()}/{utils.quote_sep(item_parsed.title).strip()}{enclosure_path.suffix}
 
 If the plugin returns a value, it must be a list of strings and will be used as the
 target paths at which to link the enclosure.  Relative paths are resolved against the
 archive root.  These paths are not escaped, so if escaping is needed it must be a part
-of the plugin configuration.  Here's an example ``link-paths`` definition::
+of the plugin configuration. If no plugins link a given enclosure, then any plugins
+whose ``fallback`` key is ``true`` will be applied. Here's an example ``enclosures``
+definition::
 
   defaults:
     base-url: "https://feeds.example.com"
     plugins:
-      link-paths:
-        sonarr:
-          url: "http://localhost:8989"
-          api-key: "????????????????????????????????"
-    link-paths:
-      # Link all feed item enclosures into the media library under the podcasts directory
-      - template: "/media/Library/Music/Podcasts/{feed_elem.find('title').text.strip()}/{item_elem.find('title').text.strip()})/{basename}"
+      enclosures:
+	sonarr:
+	  url: "http://localhost:8989"
+	  api-key: "????????????????????????????????"
+    enclosures:
+      # Link all feed item enclosures into the media library under the podcasts
+      # directory.  Link items into an album directory named by series title if
+      # matching.
+      - template: "\
+	/media/Library/Music/Podcasts\
+	/{utils.quote_sep(feed_parsed.feed.title).strip()}\
+	/{series_title}\
+	/{utils.quote_sep(item_parsed.title).strip()}{enclosure_path.suffix}"
+	match-string: "{utils.quote_sep(item_parsed.title).strip()}"
+	match-pattern: "\
+	(?P<item_title>.+) \\((?P<series_title>.+) \
+	(?P<season_number>[0-9])(?P<episode_numbers>[0-9]+[0-9Ee& -]*)\\)"
+      # Otherwise link into "self-titled" album directories of the same name as the
+      # feed.
+      - template: "\
+        /media/Library/Music/Podcasts\
+        /{utils.quote_sep(feed_parsed.feed.title).strip()}\
+        /{utils.quote_sep(feed_parsed.feed.title).strip()}\
+        /{utils.quote_sep(item_parsed.title).strip()}{enclosure_path.suffix}"
+	fallback: true
   feeds:
-    - remote-url:
-	"https://foo-username:secret@grault.example.com/feeds/garply.rss?bar=qux%2Fbaz#corge"
-      link-paths:
+    - remote-url: "\
+      https://foo-username:secret@grault.example.com\
+      /feeds/garply.rss?bar=qux%2Fbaz#corge"
+      enclosures:
 	# This particular feed is a podcast about a TV series/show.  Link enclosures
 	# from feed items about an individual episode next to the episode video file as
 	# an external audio track using a non-default plugin.
 	- plugin: "sonarr"
-	  match-string: "{item_elem.find('title').text.strip()}"
-	  match-pattern: "(?P<item_title>.+) \\((?P<series_title>.+) (?P<season_number>[0-9])(?P<episode_numbers>[0-9]+[0-9Ee& -]*)\\)"
+	  match-string: "{utils.quote_sep(item_parsed.title).strip()}"
+	  match-pattern: "\
+	  (?P<item_title>.+) \\((?P<series_title>.+) \
+	  (?P<season_number>[0-9])(?P<episode_numbers>[0-9]+[0-9Ee& -]*)\\)"
 	  stem-append: "-garply"
   ...
 
 Default Template Plugin
 =======================
 
 If no ``plugin`` key is specified, the ``template`` plugin is used.  The link
 path config may include the ``template`` key containing a `Python format string`_ which
 will be expanded to determine where the feed item enclosure should be linked to.  The
 default ``template`` is::
 
-  ./Feeds/{feed_elem.find('title').text.strip()}/{item_elem.find('title').text.strip()}/{basename}
+  ./Feeds/{utils.quote_sep(feed_parsed.feed.title).strip()}/{utils.quote_sep(item_parsed.title).strip()}{enclosure_path.suffix}
 
-The format strings may reference any of `the arguments passed into link path plugins`_.
+The format strings may reference any of `the arguments passed into enclosure plugins`_.
 
 Sonarr TV Series Plugin
 =======================
 
-The ``sonarr`` plugin uses values from the link path configuration and/or the ``match``
+The ``sonarr`` plugin uses values from the enclosure configuration and/or the ``match``
 groups to lookup a TV series/show managed by `Sonarr`_, then lookup an episode video
-file that corresponds to the feed item enclosure/content, and link the enclosure/content
-next to that video file.  The ``link-paths`` configuration or ``match`` groups must
-contain:
+file that corresponds to the feed item enclosure, and link the enclosure next to that
+video file.  The ``enclosures`` configuration or ``match`` groups must contain:
 
 - ``url`` and ``api-key`` used to `connect to the Sonarr API`_
 - ``series_id`` or ``series_title`` used to `look up the TV show/series`_, note that
   using ``series_id`` saves on Sonarr API request per update
 - ``season_number`` used to `lookup the episode file`_
 - ``episode_numbers`` used to `lookup the episode file`_, plural to support
   multi-episode files
 
 They may also include:
 
 - ``stem-append`` containing a string to append to the episode file stem before the
-  enclosure/content suffix/extension
+  enclosure suffix/extension
 
 
-************
+****************************************************************************************
 CONTRIBUTING
-************
+****************************************************************************************
 
 NOTE: `This project is hosted on GitLab`_.  There's `a mirror on GitHub`_ but please use
 GitLab for reporting issues, submitting PRs/MRs and any other development or maintenance
 activity.
 
 See `the ./CONTRIBUTING.rst file`_ for more details on how to get started with
 development.
 
 
 .. _alternate hierarchy: `Ingest Feed Enclosures Into Media Libraries`_
-.. _a link path plugin: `Plugins`_
-.. _the arguments passed into link path plugins: `Plugins`_
+.. _an enclosure plugin: `Plugins`_
+.. _the arguments passed into enclosure plugins: `Plugins`_
 
 .. _pip: https://pip.pypa.io/en/stable/installation/
+.. _argcomplete: https://kislyuk.github.io/argcomplete/#installation
 .. _a Python entry point:
    https://packaging.python.org/en/latest/specifications/entry-points/#data-model
 .. _Python format string: https://docs.python.org/3/library/string.html#formatstrings
 .. _Python regular expression match object:
    https://docs.python.org/3/library/re.html#match-objects
 .. _regular expression groups: https://docs.python.org/3/library/re.html#index-17
+.. _symbolic group names: https://docs.python.org/3/library/re.html#index-18
 .. _Python's urllib.parse.quote:
    https://docs.python.org/3/library/urllib.parse.html#urllib.parse.quote
+.. _Python pathlib.path:
+   https://docs.python.org/3/library/pathlib.html#accessing-individual-parts
 .. _Python XML element object:
     https://docs.python.org/3/library/xml.etree.elementtree.html#element-objects
 .. _lmxl special string object: https://lxml.de/xpathxslt.html#xpath-return-values
+.. _feedparser: https://pythonhosted.org/feedparser/index.html
 
 .. _nginx: https://nginx.org/en/docs/
 .. _nginx server_name: https://www.nginx.com/resources/wiki/start/topics/examples/server_blocks/
 
 .. _Jellyfin: https://jellyfin.org/
 .. _external alternative audio tracks:
    https://jellyfin.org/docs/general/server/media/external-audio-files.html
@@ -377,8 +431,8 @@
    https://gitlab.com/rpatterson/feed-archiver/blob/master/docker-compose.yml
 
 .. _`This project is hosted on GitLab`:
    https://gitlab.com/rpatterson/feed-archiver
 .. _`a mirror on GitHub`:
    https://github.com/rpatterson/feed-archiver
 .. _`the ./CONTRIBUTING.rst file`:
-   https://gitlab.com/rpatterson/feed-archiver/blob/master/CONTRIBUTING.rst
+   https://gitlab.com/rpatterson/feed-archiver/blob/main/CONTRIBUTING.rst
```

### Comparing `feed-archiver-1.0.0/TODO.rst` & `feed-archiver-1.0.0b11/TODO.rst`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,27 @@
-###########################################################################
+########################################################################################
 Seeking Contributions
-###########################################################################
+########################################################################################
 
 Known bugs and desirable features for which contributions are most welcome.
 
+TEMPLATE: Remove any of the following TODOs from the template that your project doesn't
+care about and add your own.
 
-********
+
+****************************************************************************************
 Required
-********
+****************************************************************************************
 
 
-*************
+****************************************************************************************
 High Priority
-*************
+****************************************************************************************
+
+#. Add an enclosure plugin to create playlists.
 
 #. Any documentation improvements!
 
    Documentation benefits perhaps most from the attention of fresh eyes.  If you find
    anything confusing, please ask for clarification and once you understand what you
    didn't before, please do contribute changes to the documentation to spare future
    users the same confusion.
@@ -40,17 +45,17 @@
    - https://toolbelt.readthedocs.io/en/latest/threading.html
    - https://www.python-httpx.org/async/
 
 #. Determine if HTTP/2 is a significant performance improvement for serving large media
    files and integrate into the Traefik -> Nginx stack if yes.
 
 
-************
+****************************************************************************************
 Nice to Have
-************
+****************************************************************************************
 
 #. Feed config option to override downloads XPath expression.
 
 #. Option to re-download enclosures/assets if
    Last-Modified/If-Modified-Since/If-Unmodified-Since
 
 #. Option to re-download enclosures/assets if Content-Length is different
@@ -63,16 +68,14 @@
    file.
 
 #. Order new items based on which siblings they're next to in the previous feed version.
 
 #. Extension point (setuptools entry points?) for selecting specialized download
    handlers based on MIME type (e.g. HTML page assets/resources below).
 
-#. Playlist creation for media enclosures.
-
 #. Also download all assets/resources for HTML downloads, possibly with `pywebcopy
    <https://stackoverflow.com/a/51544575/624787>`_.
 
 #. Cleanup embedded enclosure metadata (e.g. ID3 tags in MP3) based on item data.  For
    example, add missing ID3 tag with title from the item XML.
 
 #. Improve XML namespace map/prefix for custom attributes.
@@ -80,7 +83,11 @@
 #. Archive config option to specify the list of safe characters for quoting.
 
 #. Maybe allow Unicode in filesystem path escaping?  Do most filesystems support
    Unicode, for instance?  How do static file servers handle Unicode in filesystem
    paths?
 
 #. Option to use hard links instead of symlinks.
+
+#. More examples of template configurations to match feed metadata: e.g. prepending
+   ``<itunes:episode>`` to link basename, extracting album directory from feed item
+   title.
```

### Comparing `feed-archiver-1.0.0/bin/entrypoint` & `feed-archiver-1.0.0b11/bin/entrypoint`

 * *Files 22% similar despite different names*

```diff
@@ -1,45 +1,44 @@
 #!/bin/bash
 #
 # Perform any required volatile run-time initialization
 
 set -eu -o pipefail
 shopt -s inherit_errexit
-if [ ! -z "${DEBUG:=}" ]
+if [ "${DEBUG:=false}" = "true" ]
 then
     # Echo commands for easier debugging
-    PS4='$0:$LINENO+'
     set -x
+    PS4='$0:$LINENO+'
 fi
 
 
 main() {
-    if [ ! -z "${PUID:-}" ]
+    if [ -n "${PUID:-}" ]
     then
 	if (( $(id -u) != 0 ))
 	then
 	    set +x
 	    echo "ERROR: Can't create a user when not run as root" 1>&2
 	    false
 	fi
-	if ! id ${PUID}
+	if ! id "${PUID}" >"/dev/null" 2>&1
 	then
 	    # Add a user to the `passwd` DB so that the `~feed-archiver/`
 	    # HOME directory can be looked up.
 	    adduser --uid "${PUID}" --disabled-password --gecos \
-		    "Feed Archiver,,," "feed-archiver" 1>&2
+		    "Feed Archiver,,," "feed-archiver" >"/dev/null"
 	fi
 	# Fix the TTY ownership if the session is interactive
 	if tty_dev=$(tty)
 	then
-	    chown -c "${PUID}" "${tty_dev}"
+	    chown "${PUID}" "${tty_dev}"
 	fi
 	# Delegate the rest to the `CMD`
 	exec gosu "${PUID}:${PGID:-${PUID}}" "${@}"
     fi
 
     # Delegate the rest to the `CMD`
     exec "$@"
 }
 
-
 main "$@"
```

### Comparing `feed-archiver-1.0.0/nginx/templates/default.conf.template` & `feed-archiver-1.0.0b11/nginx/templates/default.conf.template`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 server {
     # FIXME: Should we find a way to switch to HTTPS so we can use HTTP/2
-    listen 80 default_server;
-    listen [::]:80 default_server;
+    listen ${NGINX_PORT} default_server;
+    listen [::]:${NGINX_PORT} default_server;
     server_name ${NGINX_HOST};
 
     # Make browsing/discovery easier, serve indexes of directories:
     # https://docs.nginx.com/nginx/admin-guide/web-server/serving-static-content/#root-directory-and-index-files
-    root /var/www/html;
+    root ${NGINX_ROOT};
     autoindex on;
 
     location / {
         # First attempt to serve request as file, then as directory, then as a
         # corresponding `*.html` file, then fall back to displaying a 404:
         # https://docs.nginx.com/nginx/admin-guide/web-server/serving-static-content/#trying-several-options
         try_files $uri $uri/ $uri.html $uri.htm =404;
```

### Comparing `feed-archiver-1.0.0/pyproject.toml` & `feed-archiver-1.0.0b11/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -12,33 +12,37 @@
 # local_scheme = "no-local-version"
 [tool.commitizen]
 # Parse commit messages according to conventional commits to decide wether the next
 # versin tag should be a major, minor or patch bump and create the VCS tag.  Also
 # provides VCS hooks to enforce that commit messages comply with conventional commits:
 # https://commitizen-tools.github.io/commitizen/
 name = "cz_conventional_commits"
-version = "1.0.0"
+changelog_start_rev = "v0.0.0"
+version = "1.0.0b11"
 tag_format = "v$version"
 annotated_tag = true
+gpg_sign = true
 bump_message = """\
 build(release): Version $current_version → $new_version
 
 [actions skip]
+[ci release]
 """
 [tool.towncrier]
 # https://towncrier.readthedocs.io/en/stable/#quick-start
 package = "feedarchiver"
 package_dir = "src"
+name = "feed-archiver"
 
 [tool.pylint.MASTER]
-# Auto-detect the number of processors available to use from:
-#     $ pylint --generate-rcfile
-jobs = 0
+# Ensure `duplicate-code` and any other errors that depend on not runnining in parallel
+# are reported:
+jobs = 1
 enable-all-extensions = true
-output-format = "colorized,json:pylint.json"
+output-format = "colorized"
 ignore-paths = [
 # Managed by tools, best to use `# pylint: disable=...` inline comments for any other
 # ignores.
     "src/.+/version.py",
     ".*/src/.+/version.py",
 ]
 # Extend linting to usage of trusted extension packages
@@ -46,16 +50,38 @@
 [tool.pylint.TYPECHECK]
 # Ignore false negatives from external packages
 ignored-classes = ["lxml.etree.QName.localname"]
 # Match Black's defaults
 # https://black.readthedocs.io/en/stable/guides/using_black_with_other_tools.html#pylint
 [tool.pylint.format]
 max-line-length = "88"
+[tool.pylint."messages control"]
+disable = [
+    # Workaround Prospector bug with PyLint:
+    # https://github.com/PyCQA/prospector/issues/596#issue-1592499675
+    "relative-beyond-top-level",
+    # I'm not sure I agree with PyLiint here.  I prefer my `TODO`s to be in the the most
+    # appropriate context where the change should happen.  It helps my recall.  If someone
+    # else wants to take the time to move the `TODO`s into `./TODO.rst`, I won't object as
+    # long as sufficient context comes along with them.
+    "fixme",
+]
+
 [[tool.mypy.overrides]]
-module = ["user_agent", "arrapi", "requests_toolbelt.*"]
+module = [
+    "importlib_metadata",
+    "argcomplete",
+    "user_agent",
+    "arrapi",
+    "requests_toolbelt.*",
+    "feedparser",
+]
 ignore_missing_imports = true
 
+[tool.vulture]
+# https://github.com/jendrikseipp/vulture#ignoring-files
+exclude = ["src/feedarchiver/version.py"]
 
 [tool.isort]
 # Match Black's defaults
 # https://black.readthedocs.io/en/stable/guides/using_black_with_other_tools.html#isort
 profile = "black"
```

### Comparing `feed-archiver-1.0.0/requirements-build.txt` & `feed-archiver-1.0.0b11/requirements/py37/build.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,140 +1,135 @@
 #
-# This file is autogenerated by pip-compile with Python 3.10
+# This file is autogenerated by pip-compile with Python 3.7
 # by the following command:
 #
-#    pip-compile --output-file=./requirements-build.txt --resolver=backtracking ./requirements-build.txt.in
+#    pip-compile --output-file=requirements/py37/build.txt --resolver=backtracking requirements/build.txt.in
 #
-argcomplete==2.0.0
+argcomplete==2.0.6
     # via commitizen
-bleach==5.0.1
+bleach==6.0.0
     # via readme-renderer
-build==0.9.0
-    # via pip-tools
 certifi==2022.12.7
     # via requests
 cffi==1.15.1
     # via cryptography
 cfgv==3.3.1
     # via pre-commit
 charset-normalizer==2.1.1
     # via
     #   commitizen
     #   requests
-click==8.1.3
-    # via pip-tools
 colorama==0.4.6
     # via commitizen
-commitizen==2.38.0
-    # via -r ./requirements-build.txt.in
-commonmark==0.9.1
-    # via rich
-cryptography==38.0.4
+commitizen==2.42.1
+    # via -r requirements/build.txt.in
+cryptography==40.0.2
     # via secretstorage
 decli==0.5.2
     # via commitizen
 distlib==0.3.6
     # via virtualenv
 docutils==0.19
     # via readme-renderer
-filelock==3.8.2
+filelock==3.11.0
     # via virtualenv
-identify==2.5.10
+identify==2.5.22
     # via pre-commit
 idna==3.4
     # via requests
-importlib-metadata==5.1.0
+importlib-metadata==5.2.0
     # via
+    #   argcomplete
     #   keyring
+    #   pre-commit
     #   twine
+    #   virtualenv
+importlib-resources==5.12.0
+    # via keyring
 jaraco-classes==3.2.3
     # via keyring
 jeepney==0.8.0
     # via
     #   keyring
     #   secretstorage
 jinja2==3.1.2
     # via commitizen
-keyring==23.11.0
+keyring==23.13.1
     # via twine
-markupsafe==2.1.1
+markdown-it-py==2.2.0
+    # via rich
+markupsafe==2.1.2
     # via jinja2
-more-itertools==9.0.0
+mdurl==0.1.2
+    # via markdown-it-py
+more-itertools==9.1.0
     # via jaraco-classes
 nodeenv==1.7.0
     # via pre-commit
-packaging==22.0
-    # via
-    #   build
-    #   commitizen
-pep517==0.13.0
-    # via build
-pip-tools==6.12.0
-    # via -r ./requirements-build.txt.in
-pkginfo==1.9.2
+packaging==23.1
+    # via commitizen
+pkginfo==1.9.6
     # via twine
-platformdirs==2.6.0
+platformdirs==3.2.0
     # via virtualenv
-pre-commit==2.20.0
-    # via -r ./requirements-build.txt.in
-prompt-toolkit==3.0.36
+pre-commit==2.21.0
+    # via -r requirements/build.txt.in
+prompt-toolkit==3.0.38
     # via questionary
 pycparser==2.21
     # via cffi
-pygments==2.13.0
+pygments==2.15.0
     # via
     #   readme-renderer
     #   rich
 pyyaml==6.0
     # via
     #   commitizen
     #   pre-commit
 questionary==1.10.0
     # via commitizen
 readme-renderer==37.3
     # via twine
-requests==2.28.1
+requests==2.28.2
     # via
     #   requests-toolbelt
     #   twine
 requests-toolbelt==0.10.1
     # via twine
 rfc3986==2.0.0
     # via twine
-rich==12.6.0
+rich==13.3.4
     # via twine
 secretstorage==3.3.3
     # via keyring
 six==1.16.0
     # via bleach
-termcolor==2.1.1
+termcolor==2.2.0
     # via commitizen
-toml==0.10.2
-    # via pre-commit
-tomli==2.0.1
-    # via
-    #   build
-    #   pep517
-tomlkit==0.11.6
+tomlkit==0.11.7
     # via commitizen
 twine==4.0.2
-    # via -r ./requirements-build.txt.in
-typing-extensions==4.4.0
-    # via commitizen
-urllib3==1.26.13
+    # via -r requirements/build.txt.in
+typing-extensions==4.5.0
+    # via
+    #   commitizen
+    #   importlib-metadata
+    #   markdown-it-py
+    #   platformdirs
+    #   rich
+urllib3==1.26.15
     # via
     #   requests
     #   twine
-virtualenv==20.17.1
+virtualenv==20.21.0
     # via pre-commit
-wcwidth==0.2.5
+wcwidth==0.2.6
     # via prompt-toolkit
 webencodings==0.5.1
     # via bleach
-wheel==0.38.4
-    # via pip-tools
-zipp==3.11.0
-    # via importlib-metadata
+zipp==3.15.0
+    # via
+    #   importlib-metadata
+    #   importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
-# pip
 # setuptools
```

### Comparing `feed-archiver-1.0.0/server/docker-compose.yml` & `feed-archiver-1.0.0b11/server/docker-compose.yml`

 * *Files 12% similar despite different names*

```diff
@@ -176,73 +176,100 @@
 00000af0: 544c 532f 5353 4c2c 2065 7463 2e2c 2069  TLS/SSL, etc., i
 00000b00: 6e20 6120 636f 6e74 6169 6e65 722d 6e61  n a container-na
 00000b10: 7469 7665 2070 726f 7879 2073 7563 680a  tive proxy such.
 00000b20: 2020 2320 6173 2054 7261 6566 696b 2e0a    # as Traefik..
 00000b30: 2020 6e67 696e 783a 0a20 2020 2069 6d61    nginx:.    ima
 00000b40: 6765 3a20 226e 6769 6e78 220a 2020 2020  ge: "nginx".    
 00000b50: 636f 6e74 6169 6e65 725f 6e61 6d65 3a20  container_name: 
-00000b60: 226e 6769 6e78 220a 2020 2020 766f 6c75  "nginx".    volu
-00000b70: 6d65 733a 0a20 2020 2020 202d 2022 2e2f  mes:.      - "./
-00000b80: 6e67 696e 782f 7465 6d70 6c61 7465 732f  nginx/templates/
-00000b90: 3a2f 6574 632f 6e67 696e 782f 7465 6d70  :/etc/nginx/temp
-00000ba0: 6c61 7465 732f 220a 2020 2020 2020 2d20  lates/".      - 
-00000bb0: 2224 7b46 4545 445f 4152 4348 4956 457d  "${FEED_ARCHIVE}
-00000bc0: 3a2f 7661 722f 7777 772f 6874 6d6c 220a  :/var/www/html".
-00000bd0: 2020 2020 706f 7274 733a 0a20 2020 2020      ports:.     
-00000be0: 2d20 2239 3038 303a 3830 220a 2020 2020  - "9080:80".    
-00000bf0: 656e 765f 6669 6c65 3a0a 2020 2020 2020  env_file:.      
-00000c00: 2d20 222e 2f2e 656e 7622 0a20 2020 2065  - "./.env".    e
-00000c10: 6e76 6972 6f6e 6d65 6e74 3a0a 2020 2020  nvironment:.    
-00000c20: 2020 4e47 494e 585f 484f 5354 3a20 2266    NGINX_HOST: "f
-00000c30: 6565 6473 2e65 7861 6d70 6c65 2e63 6f6d  eeds.example.com
-00000c40: 220a 2020 2020 6c61 6265 6c73 3a0a 2020  ".    labels:.  
-00000c50: 2020 2020 2320 6874 7470 733a 2f2f 646f      # https://do
-00000c60: 632e 7472 6165 6669 6b2e 696f 2f74 7261  c.traefik.io/tra
-00000c70: 6566 696b 2f75 7365 722d 6775 6964 6573  efik/user-guides
-00000c80: 2f64 6f63 6b65 722d 636f 6d70 6f73 652f  /docker-compose/
-00000c90: 6163 6d65 2d74 6c73 2f23 7365 7475 700a  acme-tls/#setup.
-00000ca0: 2020 2020 2020 7472 6165 6669 6b2e 656e        traefik.en
-00000cb0: 6162 6c65 3a20 7472 7565 0a20 2020 2020  able: true.     
-00000cc0: 2074 7261 6566 696b 2e68 7474 702e 726f   traefik.http.ro
-00000cd0: 7574 6572 732e 6e67 696e 782e 7275 6c65  uters.nginx.rule
-00000ce0: 3a20 2248 6f73 7428 6066 6565 6473 2e65  : "Host(`feeds.e
-00000cf0: 7861 6d70 6c65 2e63 6f6d 6029 220a 2020  xample.com`)".  
-00000d00: 2020 2020 7472 6165 6669 6b2e 6874 7470      traefik.http
-00000d10: 2e73 6572 7669 6365 732e 6e67 696e 782e  .services.nginx.
-00000d20: 6c6f 6164 6261 6c61 6e63 6572 2e73 6572  loadbalancer.ser
-00000d30: 7665 722e 706f 7274 3a20 3830 0a20 2020  ver.port: 80.   
-00000d40: 2020 2074 7261 6566 696b 2e68 7474 702e     traefik.http.
-00000d50: 726f 7574 6572 732e 6e67 696e 782e 656e  routers.nginx.en
-00000d60: 7472 7970 6f69 6e74 733a 2022 7765 6273  trypoints: "webs
-00000d70: 6563 7572 6522 0a20 2020 2020 2074 7261  ecure".      tra
-00000d80: 6566 696b 2e68 7474 702e 726f 7574 6572  efik.http.router
-00000d90: 732e 6e67 696e 782e 746c 732e 6365 7274  s.nginx.tls.cert
-00000da0: 7265 736f 6c76 6572 3a20 226c 6574 7365  resolver: "letse
-00000db0: 6e63 7279 7074 220a 2020 2020 2020 7472  ncrypt".      tr
-00000dc0: 6165 6669 6b2e 6874 7470 2e6d 6964 646c  aefik.http.middl
-00000dd0: 6577 6172 6573 2e66 6565 6473 2d61 7574  ewares.feeds-aut
-00000de0: 682e 6261 7369 6361 7574 682e 7573 6572  h.basicauth.user
-00000df0: 7366 696c 653a 2022 2e2f 7365 7276 6572  sfile: "./server
-00000e00: 2f2e 6874 7061 7373 7764 220a 2020 2020  /.htpasswd".    
-00000e10: 2020 7472 6165 6669 6b2e 6874 7470 2e72    traefik.http.r
-00000e20: 6f75 7465 7273 2e6e 6769 6e78 2e6d 6964  outers.nginx.mid
-00000e30: 646c 6577 6172 6573 3a20 2266 6565 6473  dlewares: "feeds
-00000e40: 2d61 7574 6822 0a0a 2020 2320 436f 6e74  -auth"..  # Cont
-00000e50: 6169 6e65 722d 6e61 7469 7665 2062 7574  ainer-native but
-00000e60: 206f 7263 6865 7374 7261 746f 7220 696e   orchestrator in
-00000e70: 6465 7065 6e64 656e 7420 7065 7269 6f64  dependent period
-00000e80: 6963 2074 6173 6b73 0a20 2023 2068 7474  ic tasks.  # htt
-00000e90: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000ea0: 6d63 7561 6472 6f73 2f6f 6665 6c69 6123  mcuadros/ofelia#
-00000eb0: 646f 636b 6572 2d6c 6162 656c 732d 636f  docker-labels-co
-00000ec0: 6e66 6967 7572 6174 696f 6e73 0a20 206f  nfigurations.  o
-00000ed0: 6665 6c69 613a 0a20 2020 2069 6d61 6765  felia:.    image
-00000ee0: 3a20 226d 6375 6164 726f 732f 6f66 656c  : "mcuadros/ofel
-00000ef0: 6961 3a6c 6174 6573 7422 0a20 2020 2063  ia:latest".    c
-00000f00: 6f6e 7461 696e 6572 5f6e 616d 653a 2022  ontainer_name: "
-00000f10: 6f66 656c 6961 220a 2020 2020 636f 6d6d  ofelia".    comm
-00000f20: 616e 643a 2022 6461 656d 6f6e 202d 2d64  and: "daemon --d
-00000f30: 6f63 6b65 7222 0a20 2020 2076 6f6c 756d  ocker".    volum
-00000f40: 6573 3a0a 2020 2020 2020 2d20 222f 7661  es:.      - "/va
-00000f50: 722f 7275 6e2f 646f 636b 6572 2e73 6f63  r/run/docker.soc
-00000f60: 6b3a 2f76 6172 2f72 756e 2f64 6f63 6b65  k:/var/run/docke
-00000f70: 722e 736f 636b 3a72 6f22 0a              r.sock:ro".
+00000b60: 226e 6769 6e78 220a 2020 2020 7265 7374  "nginx".    rest
+00000b70: 6172 743a 2022 756e 6c65 7373 2d73 746f  art: "unless-sto
+00000b80: 7070 6564 220a 2020 2020 2320 766f 6c75  pped".    # volu
+00000b90: 6d65 733a 0a20 2020 2020 2023 2055 6e63  mes:.      # Unc
+00000ba0: 6f6d 6d65 6e74 2074 6f20 7573 6520 7468  omment to use th
+00000bb0: 6520 6465 6661 756c 7420 636f 6e66 6967  e default config
+00000bc0: 7572 6174 696f 6e3a 0a20 2020 2020 2023  uration:.      #
+00000bd0: 202d 2022 2e2f 6e67 696e 782f 7465 6d70   - "./nginx/temp
+00000be0: 6c61 7465 732f 3a2f 6574 632f 6e67 696e  lates/:/etc/ngin
+00000bf0: 782f 7465 6d70 6c61 7465 732f 220a 2020  x/templates/".  
+00000c00: 2020 2020 2320 4164 6420 7468 6520 6170      # Add the ap
+00000c10: 7072 6f70 7269 6174 6520 766f 6c75 6d65  propriate volume
+00000c20: 2066 6f72 2079 6f75 7220 656e 7669 726f   for your enviro
+00000c30: 6e6d 656e 7420 7468 6174 2077 696c 6c20  nment that will 
+00000c40: 6d61 6b65 2060 247b 4e47 494e 585f 524f  make `${NGINX_RO
+00000c50: 4f54 7d60 0a20 2020 2020 2023 2061 6363  OT}`.      # acc
+00000c60: 6573 7369 626c 6520 7769 7468 696e 2074  essible within t
+00000c70: 6865 2063 6f6e 7461 696e 6572 3a0a 2020  he container:.  
+00000c80: 2020 2020 2320 2d20 2224 7b4e 4749 4e58      # - "${NGINX
+00000c90: 5f52 4f4f 543a 2d2f 6d65 6469 612f 4c69  _ROOT:-/media/Li
+00000ca0: 6272 6172 792f 6665 6564 732f 7d3a 247b  brary/feeds/}:${
+00000cb0: 4e47 494e 585f 524f 4f54 3a2d 2f6d 6564  NGINX_ROOT:-/med
+00000cc0: 6961 2f4c 6962 7261 7279 2f66 6565 6473  ia/Library/feeds
+00000cd0: 2f7d 220a 2020 2020 706f 7274 733a 0a20  /}".    ports:. 
+00000ce0: 2020 2020 2d20 2239 3038 303a 247b 4e47      - "9080:${NG
+00000cf0: 494e 585f 504f 5254 3a2d 3830 7d22 0a20  INX_PORT:-80}". 
+00000d00: 2020 2065 6e76 5f66 696c 653a 0a20 2020     env_file:.   
+00000d10: 2020 202d 2022 2e2f 2e65 6e76 220a 2020     - "./.env".  
+00000d20: 2020 656e 7669 726f 6e6d 656e 743a 0a20    environment:. 
+00000d30: 2020 2020 204e 4749 4e58 5f50 4f52 543a       NGINX_PORT:
+00000d40: 2022 247b 4e47 494e 585f 504f 5254 3a2d   "${NGINX_PORT:-
+00000d50: 3830 7d22 0a20 2020 2020 204e 4749 4e58  80}".      NGINX
+00000d60: 5f48 4f53 543a 2022 6665 6564 732e 6578  _HOST: "feeds.ex
+00000d70: 616d 706c 652e 636f 6d22 0a20 2020 2068  ample.com".    h
+00000d80: 6561 6c74 6863 6865 636b 3a0a 2020 2020  ealthcheck:.    
+00000d90: 2020 7465 7374 3a20 3e2d 0a20 2020 2020    test: >-.     
+00000da0: 2020 2063 7572 6c20 2d4c 7620 2268 7474     curl -Lv "htt
+00000db0: 703a 2f2f 6c6f 6361 6c68 6f73 743a 3830  p://localhost:80
+00000dc0: 2220 7c20 6772 6570 2027 3c74 6974 6c65  " | grep '<title
+00000dd0: 3e49 6e64 6578 206f 6620 2f3c 2f74 6974  >Index of /</tit
+00000de0: 6c65 3e27 0a20 2020 206c 6162 656c 733a  le>'.    labels:
+00000df0: 0a20 2020 2020 2023 2068 7474 7073 3a2f  .      # https:/
+00000e00: 2f64 6f63 2e74 7261 6566 696b 2e69 6f2f  /doc.traefik.io/
+00000e10: 7472 6165 6669 6b2f 7573 6572 2d67 7569  traefik/user-gui
+00000e20: 6465 732f 646f 636b 6572 2d63 6f6d 706f  des/docker-compo
+00000e30: 7365 2f61 636d 652d 746c 732f 2373 6574  se/acme-tls/#set
+00000e40: 7570 0a20 2020 2020 2074 7261 6566 696b  up.      traefik
+00000e50: 2e65 6e61 626c 653a 2074 7275 650a 2020  .enable: true.  
+00000e60: 2020 2020 7472 6165 6669 6b2e 6874 7470      traefik.http
+00000e70: 2e72 6f75 7465 7273 2e6e 6769 6e78 2e72  .routers.nginx.r
+00000e80: 756c 653a 2022 486f 7374 2860 6665 6564  ule: "Host(`feed
+00000e90: 732e 6578 616d 706c 652e 636f 6d60 2922  s.example.com`)"
+00000ea0: 0a20 2020 2020 2074 7261 6566 696b 2e68  .      traefik.h
+00000eb0: 7474 702e 7365 7276 6963 6573 2e6e 6769  ttp.services.ngi
+00000ec0: 6e78 2e6c 6f61 6462 616c 616e 6365 722e  nx.loadbalancer.
+00000ed0: 7365 7276 6572 2e70 6f72 743a 2024 7b4e  server.port: ${N
+00000ee0: 4749 4e58 5f50 4f52 543a 2d38 307d 0a20  GINX_PORT:-80}. 
+00000ef0: 2020 2020 2074 7261 6566 696b 2e68 7474       traefik.htt
+00000f00: 702e 726f 7574 6572 732e 6e67 696e 782e  p.routers.nginx.
+00000f10: 656e 7472 7970 6f69 6e74 733a 2022 7765  entrypoints: "we
+00000f20: 6273 6563 7572 6522 0a20 2020 2020 2074  bsecure".      t
+00000f30: 7261 6566 696b 2e68 7474 702e 726f 7574  raefik.http.rout
+00000f40: 6572 732e 6e67 696e 782e 746c 732e 6365  ers.nginx.tls.ce
+00000f50: 7274 7265 736f 6c76 6572 3a20 226c 6574  rtresolver: "let
+00000f60: 7365 6e63 7279 7074 220a 2020 2020 2020  sencrypt".      
+00000f70: 7472 6165 6669 6b2e 6874 7470 2e6d 6964  traefik.http.mid
+00000f80: 646c 6577 6172 6573 2e66 6565 6473 2d61  dlewares.feeds-a
+00000f90: 7574 682e 6261 7369 6361 7574 682e 7573  uth.basicauth.us
+00000fa0: 6572 7366 696c 653a 2022 2e2f 7365 7276  ersfile: "./serv
+00000fb0: 6572 2f2e 6874 7061 7373 7764 220a 2020  er/.htpasswd".  
+00000fc0: 2020 2020 7472 6165 6669 6b2e 6874 7470      traefik.http
+00000fd0: 2e72 6f75 7465 7273 2e6e 6769 6e78 2e6d  .routers.nginx.m
+00000fe0: 6964 646c 6577 6172 6573 3a20 2266 6565  iddlewares: "fee
+00000ff0: 6473 2d61 7574 6822 0a0a 2020 2320 436f  ds-auth"..  # Co
+00001000: 6e74 6169 6e65 722d 6e61 7469 7665 2062  ntainer-native b
+00001010: 7574 206f 7263 6865 7374 7261 746f 7220  ut orchestrator 
+00001020: 696e 6465 7065 6e64 656e 7420 7065 7269  independent peri
+00001030: 6f64 6963 2074 6173 6b73 0a20 2023 2068  odic tasks.  # h
+00001040: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00001050: 6d2f 6d63 7561 6472 6f73 2f6f 6665 6c69  m/mcuadros/ofeli
+00001060: 6123 646f 636b 6572 2d6c 6162 656c 732d  a#docker-labels-
+00001070: 636f 6e66 6967 7572 6174 696f 6e73 0a20  configurations. 
+00001080: 206f 6665 6c69 613a 0a20 2020 2069 6d61   ofelia:.    ima
+00001090: 6765 3a20 226d 6375 6164 726f 732f 6f66  ge: "mcuadros/of
+000010a0: 656c 6961 3a6c 6174 6573 7422 0a20 2020  elia:latest".   
+000010b0: 2063 6f6e 7461 696e 6572 5f6e 616d 653a   container_name:
+000010c0: 2022 6f66 656c 6961 220a 2020 2020 636f   "ofelia".    co
+000010d0: 6d6d 616e 643a 2022 6461 656d 6f6e 202d  mmand: "daemon -
+000010e0: 2d64 6f63 6b65 7222 0a20 2020 2076 6f6c  -docker".    vol
+000010f0: 756d 6573 3a0a 2020 2020 2020 2d20 222f  umes:.      - "/
+00001100: 7661 722f 7275 6e2f 646f 636b 6572 2e73  var/run/docker.s
+00001110: 6f63 6b3a 2f76 6172 2f72 756e 2f64 6f63  ock:/var/run/doc
+00001120: 6b65 722e 736f 636b 3a72 6f22 0a         ker.sock:ro".
```

### Comparing `feed-archiver-1.0.0/src/feed_archiver.egg-info/PKG-INFO` & `feed-archiver-1.0.0b11/src/feed_archiver.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,91 +1,95 @@
 Metadata-Version: 2.1
 Name: feed-archiver
-Version: 1.0.0
+Version: 1.0.0b11
 Summary: Archive the full contents of RSS/Atom syndication feeds including enclosures and assets.
 Home-page: https://gitlab.com/rpatterson/feed-archiver
 Author: Ross Patterson
 Author-email: me@rpatterson.net
 License: MIT
+Keywords: template,structure
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Utilities
-Requires-Python: >=3.10
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: devel
 License-File: LICENSE
 
 ########################################################################################
 feed-archiver
 ########################################################################################
 Archive the full contents of RSS/Atom syndication feeds including enclosures and assets.
 ****************************************************************************************
 
 .. list-table::
    :class: borderless align-right
 
    * - .. figure:: https://img.shields.io/pypi/v/feed-archiver.svg?logo=pypi&label=PyPI&logoColor=gold
-          :alt: PyPI latest release version
-          :target: https://pypi.org/project/feed-archiver/
+	  :alt: PyPI latest release version
+	  :target: https://pypi.org/project/feed-archiver/
        .. figure:: https://img.shields.io/pypi/dm/feed-archiver.svg?color=blue&label=Downloads&logo=pypi&logoColor=gold
-          :alt: PyPI downloads per month
-          :target: https://pypi.org/project/feed-archiver/
+	  :alt: PyPI downloads per month
+	  :target: https://pypi.org/project/feed-archiver/
        .. figure:: https://img.shields.io/pypi/pyversions/feed-archiver.svg?logo=python&label=Python&logoColor=gold
-          :alt: PyPI Python versions
-          :target: https://pypi.org/project/feed-archiver/
+	  :alt: PyPI Python versions
+	  :target: https://pypi.org/project/feed-archiver/
        .. figure:: https://img.shields.io/badge/code%20style-black-000000.svg
-          :alt: Python code style
-          :target: https://github.com/psf/black
+	  :alt: Python code style
+	  :target: https://github.com/psf/black
 
      - .. figure:: https://gitlab.com/rpatterson/feed-archiver/-/badges/release.svg
 	  :alt: GitLab latest release
 	  :target: https://gitlab.com/rpatterson/feed-archiver/-/releases
-       .. figure:: https://gitlab.com/rpatterson/feed-archiver/badges/master/pipeline.svg
+       .. figure:: https://gitlab.com/rpatterson/feed-archiver/badges/main/pipeline.svg
           :alt: GitLab CI/CD pipeline status
-          :target: https://gitlab.com/rpatterson/feed-archiver/-/commits/master
-       .. figure:: https://gitlab.com/rpatterson/feed-archiver/badges/master/coverage.svg
+          :target: https://gitlab.com/rpatterson/feed-archiver/-/commits/main
+       .. figure:: https://gitlab.com/rpatterson/feed-archiver/badges/main/coverage.svg
           :alt: GitLab coverage report
-	  :target: https://gitlab.com/rpatterson/feed-archiver/-/commits/master
+	  :target: https://gitlab.com/rpatterson/feed-archiver/-/commits/main
        .. figure:: https://img.shields.io/gitlab/stars/rpatterson/feed-archiver?gitlab_url=https%3A%2F%2Fgitlab.com&logo=gitlab
 	  :alt: GitLab repo stars
 	  :target: https://gitlab.com/rpatterson/feed-archiver
 
      - .. figure:: https://img.shields.io/github/v/release/rpatterson/feed-archiver?logo=github
 	  :alt: GitHub release (latest SemVer)
 	  :target: https://github.com/rpatterson/feed-archiver/releases
-       .. figure:: https://github.com/rpatterson/feed-archiver/actions/workflows/ci-cd.yml/badge.svg
+       .. figure:: https://github.com/rpatterson/feed-archiver/actions/workflows/build-test.yml/badge.svg
           :alt: GitHub Actions status
-          :target: https://github.com/rpatterson/feed-archiver/
-       .. figure:: https://codecov.io/github/rpatterson/feed-archiver/branch/master/graph/badge.svg?token=GNKVQ8VYOU 
+          :target: https://github.com/rpatterson/feed-archiver/actions/workflows/build-test.yml
+       .. figure:: https://codecov.io/github/rpatterson/feed-archiver/branch/main/graph/badge.svg?token=GNKVQ8VYOU
           :alt: Codecov test coverage
 	  :target: https://codecov.io/github/rpatterson/feed-archiver
        .. figure:: https://img.shields.io/github/stars/rpatterson/feed-archiver?logo=github
 	  :alt: GitHub repo stars
 	  :target: https://github.com/rpatterson/feed-archiver/
 
-     - .. figure:: https://img.shields.io/docker/v/merpatterson/feed-archiver?sort=semver&logo=docker
+     - .. figure:: https://img.shields.io/docker/v/merpatterson/feed-archiver/main?sort=semver&logo=docker
           :alt: Docker Hub image version (latest semver)
           :target: https://hub.docker.com/r/merpatterson/feed-archiver
        .. figure:: https://img.shields.io/docker/pulls/merpatterson/feed-archiver?logo=docker
           :alt: Docker Hub image pulls count
           :target: https://hub.docker.com/r/merpatterson/feed-archiver
        .. figure:: https://img.shields.io/docker/stars/merpatterson/feed-archiver?logo=docker
 	  :alt: Docker Hub stars
-          :target: https://hub.docker.com/r/merpatterson/feed-archiver
+	  :target: https://hub.docker.com/r/merpatterson/feed-archiver
        .. figure:: https://img.shields.io/docker/image-size/merpatterson/feed-archiver?logo=docker
 	  :alt: Docker Hub image size (latest semver)
-          :target: https://hub.docker.com/r/merpatterson/feed-archiver
+	  :target: https://hub.docker.com/r/merpatterson/feed-archiver
 
 The ``$ feed-archiver`` command aims to archive RSS/Atom feeds as fully as possible in
 such a way that the archive can serve (at least) 2 use cases:
 
 #. `Mirror of Feed Enclosures and Assets`_
 
     A mirror of the archived feeds that can be in turn served onto onto feed
@@ -158,34 +162,36 @@
 as `external alternative audio tracks`_ next to the corresponding TV episode video file.
 Multiple linking paths can be configured such that feed item enclosures can be ingested
 in multiple locations in media libraries.
 
 Because syndication feeds may have a number of different ways to correspond to library
 media, this functionality needs to be highly configurable and in order to be highly
 configurable it is more complex to customize to a specific goal.  As such, using this
-feature requires using `a link path plugin`_, or the skill level of a junior developer,
+feature requires using `an enclosure plugin`_, or the skill level of a junior developer,
 or someone who is comfortable reading and interpreting technical documentation, or
 re-using example configurations known to work by others.
 
 
-************
+****************************************************************************************
 Installation
-************
+****************************************************************************************
 
 Install using any tool for installing standard Python 3 distributions such as `pip`_::
 
   $ sudo pip3 install feed-archiver
 
+Optional shell tab completion is available via `argcomplete`_.
+
 Or use `the Docker image`_.  See `the example ./docker-compose.yml file`_ for usage
 details.
 
 
-*****
+****************************************************************************************
 Usage
-*****
+****************************************************************************************
 
 Create a ``./.feed-archiver.yml`` YAML file in a directory to serve as the root
 directory for all feeds to be archived.  The YAML file must have a top-level
 ``defaults`` key whose value is an object defining default or global options.  In
 particular, the ``base-url`` key in that section whose value must be a string which
 defines the external base URL at which the archive is served to clients and is used to
 assemble absolute URLs where relative URLs can't be used.  The file must also have a
@@ -193,201 +199,253 @@
 feeds to archive in this directory.  Each feed object must contain a ``remote-url`` key
 whose value is a string that contains the URL of an individual feed to archive.  In the
 simplest form, this can just be a file like so::
 
   defaults:
     base-url: "https://feeds.example.com"
   feeds:
-    - remote-url:
-	"https://foo-username:secret@grault.example.com/feeds/garply.rss?bar=qux%2Fbaz#corge"
+    - title: "Garply Podcast Title"
+      remote-url: "\
+      https://foo-username:secret@grault.example.com\
+      /feeds/garply.rss?bar=qux%2Fbaz#corge"
   ...
 
-Then simple run the ``$ feed-archiver`` command in that directory to update the archive
-from the current version of the feeds::
+Then run the ``$ feed-archiver`` command in that directory to update the archive from
+the current version of the feeds and write an HTML index with links to the archived
+feeds::
 
   $ cd "/var/www/html/feeds/"
   $ feed-archiver
   INFO:Retrieving feed URL: https://foo-username:secret@grault.example.com/feeds/garply.rss
   ...
+  INFO:Writing HTML index: /var/www/html/feeds/index.html
 
 See also the command-line help for details on options and arguments::
 
-  $ usage: feed-archiver [-h] [archive-dir...]
+  $ feed-archiver --help
+  usage: feed-archiver [-h] [--log-level {CRITICAL,FATAL,ERROR,WARN,WARNING,INFO,DEBUG,NOTSET}]
+		       [--archive-dir [ARCHIVE_DIR]]
+		       {update,relink} ...
 
-  Archive the full contents of RSS/Atom syndication feeds including enclosures and
-  assets.
+  Archive RSS/Atom syndication feeds and their enclosures and assets.
 
   positional arguments:
-    archive-dir  filesystem path to the root of an archive of feeds (default: ./)
-
-  optional arguments:
-    -h, --help  show this help message and exit
-
-  ...
-
-To link feed items into an `alternate hierarchy`_, such as in a media library, add a
-``link-paths`` key to the feed configuration whose value is an list/array of objects
-each defining one alternative path to link to the feed item enclosure.  Any
-``link-paths`` defined in the top-level ``defaults`` key will be used for all feeds.
-Configuration to be shared across multiple ``link-paths`` configurations may be placed
-in the corresponding ``defaults`` / ``plugins`` / ``link-paths`` / ``{plugin_name}``
+    {update,relink}       sub-command
+      update              Request the URL of each feed in the archive and update contents accordingly.
+      relink              Re-link enclosures to the correct locations for the current configuration.
+
+  options:
+    -h, --help            show this help message and exit
+    --log-level {CRITICAL,FATAL,ERROR,WARN,WARNING,INFO,DEBUG,NOTSET}
+			  Select logging verbosity. (default: INFO)
+    --archive-dir [ARCHIVE_DIR], -a [ARCHIVE_DIR]
+			  the archive root directory into which all feeds, their enclosures and assets
+			  will be downloaded (default: .)
+
+To link feed item enclosures into an `alternate hierarchy`_, such as in a media library,
+add a ``enclosures`` key to the feed configuration whose value is an list/array of
+objects each defining one alternative path to link to the feed item enclosure.  Any
+``enclosures`` defined in the top-level ``defaults`` key will be used for all feeds.
+Configuration to be shared across multiple ``enclosures`` configurations may be placed
+in the corresponding ``defaults`` / ``plugins`` / ``enclosures`` / ``{plugin_name}``
 object.  The actual linking of enclosures is delegated to `plugins`_.
 
+When updating the archive from the remote feed URLs using the ``$ feed-archiver
+update`` sub-command, the enclosures of new items are linked as configured.  If the
+``enclosures`` configuration changes or any of the used plugins refer to external
+resources that may change, such as the with the ``sonarr`` plugin when `Sonarr`_ has
+upgraded or renamed the corresponding video files, use the  ``$ feed-archiver relink``
+command to update all existing links.
+
 
 *******
 Plugins
 *******
 
 How feed item enclosures are linked into a media library is delegated to plugins or
-add-ons.  Specifically, the ``plugin`` key in a ``link-paths`` configuration must be a
+add-ons.  Specifically, the ``plugin`` key in a ``enclosures`` configuration must be a
 string which is the name of `a Python entry point`_ registered in the
-``feedarchiver.linkpaths`` group.  The entry point object reference must point to a
-``feedarchiver.linkpaths.LinkPathPlugin`` subclass which accepts the following arguments
+``feedarchiver.enclosures`` group.  The entry point object reference must point to a
+``feedarchiver.enclosures.EnclosurePlugin`` subclass which accepts the following arguments
 when instantiated:
 
 #. ``parent=dict``
 
    The ``feedarchiver.archive.Archive`` if the plugin is configured in ``defaults`` for
    all feeds or the ``feedarchiver.feed.ArchiveFeed`` if defined for a specific feed.
 
 #. ``config=dict``
 
    The Python dictionary object from the de-serialized archive configuration YAML for
-   this specific link path configuration.
+   this specific enclosure configuration.
 
 and whose instances must be callable and accept the following arguments when called:
 
 #. ``archive_feed=feedarchiver.feed.ArchiveFeed``
 
    The object ``feedarchiver`` uses internally to represent an individual feed in the
    archive.
 
-#. ``feed_elem=xml.etree.ElementTree.Element``
+#. ``feed_elem=xml.etree.ElementTree.Element``,
+   ``item_elem=xml.etree.ElementTree.Element``
 
-   The `Python XML element object`_ representing the whole feed.  For RSS this is the
-   ``<channel>`` child element while for Atom this is the root ``<feed>`` element.
+   The `Python XML element object`_ representing the whole feed, for RSS this is the
+   ``<channel>`` child element while for Atom this is the root ``<feed>`` element, and
+   the a similar object representing the specific feed item.
 
-#. ``item_elem=xml.etree.ElementTree.Element``
+#. ``feed_parsed=feedparser.util.FeedParserDict``,
+   ``item_parsed=feedparser.util.FeedParserDict``
 
-   The `Python XML element object`_ representing the specific feed item.
+   The `feedparser`_ object representing the whole feed and the specific feed item.
 
 #. ``url_result=lxml.etree._ElementUnicodeResult``
 
    The `lmxl special string object`_ that contains the URL of the specific enclosure.
    Can be used to access the specific enclosure element.
 
-#. ``basename=str``
+#. ``enclosure_path=pathlib.Path``
 
-  The best guess at the most correct file basename, including the suffix or extension,
-  for the given enclosure.  This suffix takes into account the suffix from the enclosure
-  URL, the ``Content-Type`` header of the response to the enclosure URL request, and
-  finally the value of any ``type`` attribute of the enclosure element XML.
+   The path to the enclosure in the archive as a `Python pathlib.Path`_ object with the
+   best guess at the most correct file basename, including the suffix or extension, for
+   the given enclosure.  This suffix takes into account the suffix from the enclosure
+   URL, the ``Content-Type`` header of the response to the enclosure URL request, and
+   finally the value of any ``type`` attribute of the enclosure element XML.
 
 #. ``match=re.Match``
 
    The `Python regular expression match object`_ if the ``match-pattern`` matched the
    string expanded from the `Python format string`_ in the ``match-string`` key.
    Particularly useful to designate `regular expression groups`_ in the
    ``match-pattern`` and then use the parts of ``match-string`` that matched those
    groups in the format ``template``.  If the ``match-pattern`` doesn't match then the
-   enclosure will not be linked.  If no ``match-string`` is provided a default is used
-   combining the feed title, item title, and enclosure basename with extension::
+   enclosure will not be linked. If there are `symbolic group names`_,
+   e.g. ``(?P<foo_group_name>.*)`` in the pattern, then they are also available by name
+   in the format string, e.g ``{foo_group_name.lower()}``.  If no ``match-string`` is
+   provided a default is used combining the feed title, item title, and enclosure
+   basename with extension::
 
-     {feed_elem.find('title').text.strip()}/{item_elem.find('title').text.strip()}/{basename}
+     {utils.quote_sep(feed_parsed.feed.title).strip()}/{utils.quote_sep(item_parsed.title).strip()}{enclosure_path.suffix}
 
 If the plugin returns a value, it must be a list of strings and will be used as the
 target paths at which to link the enclosure.  Relative paths are resolved against the
 archive root.  These paths are not escaped, so if escaping is needed it must be a part
-of the plugin configuration.  Here's an example ``link-paths`` definition::
+of the plugin configuration. If no plugins link a given enclosure, then any plugins
+whose ``fallback`` key is ``true`` will be applied. Here's an example ``enclosures``
+definition::
 
   defaults:
     base-url: "https://feeds.example.com"
     plugins:
-      link-paths:
-        sonarr:
-          url: "http://localhost:8989"
-          api-key: "????????????????????????????????"
-    link-paths:
-      # Link all feed item enclosures into the media library under the podcasts directory
-      - template: "/media/Library/Music/Podcasts/{feed_elem.find('title').text.strip()}/{item_elem.find('title').text.strip()})/{basename}"
+      enclosures:
+	sonarr:
+	  url: "http://localhost:8989"
+	  api-key: "????????????????????????????????"
+    enclosures:
+      # Link all feed item enclosures into the media library under the podcasts
+      # directory.  Link items into an album directory named by series title if
+      # matching.
+      - template: "\
+	/media/Library/Music/Podcasts\
+	/{utils.quote_sep(feed_parsed.feed.title).strip()}\
+	/{series_title}\
+	/{utils.quote_sep(item_parsed.title).strip()}{enclosure_path.suffix}"
+	match-string: "{utils.quote_sep(item_parsed.title).strip()}"
+	match-pattern: "\
+	(?P<item_title>.+) \\((?P<series_title>.+) \
+	(?P<season_number>[0-9])(?P<episode_numbers>[0-9]+[0-9Ee& -]*)\\)"
+      # Otherwise link into "self-titled" album directories of the same name as the
+      # feed.
+      - template: "\
+        /media/Library/Music/Podcasts\
+        /{utils.quote_sep(feed_parsed.feed.title).strip()}\
+        /{utils.quote_sep(feed_parsed.feed.title).strip()}\
+        /{utils.quote_sep(item_parsed.title).strip()}{enclosure_path.suffix}"
+	fallback: true
   feeds:
-    - remote-url:
-	"https://foo-username:secret@grault.example.com/feeds/garply.rss?bar=qux%2Fbaz#corge"
-      link-paths:
+    - remote-url: "\
+      https://foo-username:secret@grault.example.com\
+      /feeds/garply.rss?bar=qux%2Fbaz#corge"
+      enclosures:
 	# This particular feed is a podcast about a TV series/show.  Link enclosures
 	# from feed items about an individual episode next to the episode video file as
 	# an external audio track using a non-default plugin.
 	- plugin: "sonarr"
-	  match-string: "{item_elem.find('title').text.strip()}"
-	  match-pattern: "(?P<item_title>.+) \\((?P<series_title>.+) (?P<season_number>[0-9])(?P<episode_numbers>[0-9]+[0-9Ee& -]*)\\)"
+	  match-string: "{utils.quote_sep(item_parsed.title).strip()}"
+	  match-pattern: "\
+	  (?P<item_title>.+) \\((?P<series_title>.+) \
+	  (?P<season_number>[0-9])(?P<episode_numbers>[0-9]+[0-9Ee& -]*)\\)"
 	  stem-append: "-garply"
   ...
 
 Default Template Plugin
 =======================
 
 If no ``plugin`` key is specified, the ``template`` plugin is used.  The link
 path config may include the ``template`` key containing a `Python format string`_ which
 will be expanded to determine where the feed item enclosure should be linked to.  The
 default ``template`` is::
 
-  ./Feeds/{feed_elem.find('title').text.strip()}/{item_elem.find('title').text.strip()}/{basename}
+  ./Feeds/{utils.quote_sep(feed_parsed.feed.title).strip()}/{utils.quote_sep(item_parsed.title).strip()}{enclosure_path.suffix}
 
-The format strings may reference any of `the arguments passed into link path plugins`_.
+The format strings may reference any of `the arguments passed into enclosure plugins`_.
 
 Sonarr TV Series Plugin
 =======================
 
-The ``sonarr`` plugin uses values from the link path configuration and/or the ``match``
+The ``sonarr`` plugin uses values from the enclosure configuration and/or the ``match``
 groups to lookup a TV series/show managed by `Sonarr`_, then lookup an episode video
-file that corresponds to the feed item enclosure/content, and link the enclosure/content
-next to that video file.  The ``link-paths`` configuration or ``match`` groups must
-contain:
+file that corresponds to the feed item enclosure, and link the enclosure next to that
+video file.  The ``enclosures`` configuration or ``match`` groups must contain:
 
 - ``url`` and ``api-key`` used to `connect to the Sonarr API`_
 - ``series_id`` or ``series_title`` used to `look up the TV show/series`_, note that
   using ``series_id`` saves on Sonarr API request per update
 - ``season_number`` used to `lookup the episode file`_
 - ``episode_numbers`` used to `lookup the episode file`_, plural to support
   multi-episode files
 
 They may also include:
 
 - ``stem-append`` containing a string to append to the episode file stem before the
-  enclosure/content suffix/extension
+  enclosure suffix/extension
 
 
-************
+****************************************************************************************
 CONTRIBUTING
-************
+****************************************************************************************
 
 NOTE: `This project is hosted on GitLab`_.  There's `a mirror on GitHub`_ but please use
 GitLab for reporting issues, submitting PRs/MRs and any other development or maintenance
 activity.
 
 See `the ./CONTRIBUTING.rst file`_ for more details on how to get started with
 development.
 
 
 .. _alternate hierarchy: `Ingest Feed Enclosures Into Media Libraries`_
-.. _a link path plugin: `Plugins`_
-.. _the arguments passed into link path plugins: `Plugins`_
+.. _an enclosure plugin: `Plugins`_
+.. _the arguments passed into enclosure plugins: `Plugins`_
 
 .. _pip: https://pip.pypa.io/en/stable/installation/
+.. _argcomplete: https://kislyuk.github.io/argcomplete/#installation
 .. _a Python entry point:
    https://packaging.python.org/en/latest/specifications/entry-points/#data-model
 .. _Python format string: https://docs.python.org/3/library/string.html#formatstrings
 .. _Python regular expression match object:
    https://docs.python.org/3/library/re.html#match-objects
 .. _regular expression groups: https://docs.python.org/3/library/re.html#index-17
+.. _symbolic group names: https://docs.python.org/3/library/re.html#index-18
 .. _Python's urllib.parse.quote:
    https://docs.python.org/3/library/urllib.parse.html#urllib.parse.quote
+.. _Python pathlib.path:
+   https://docs.python.org/3/library/pathlib.html#accessing-individual-parts
 .. _Python XML element object:
     https://docs.python.org/3/library/xml.etree.elementtree.html#element-objects
 .. _lmxl special string object: https://lxml.de/xpathxslt.html#xpath-return-values
+.. _feedparser: https://pythonhosted.org/feedparser/index.html
 
 .. _nginx: https://nginx.org/en/docs/
 .. _nginx server_name: https://www.nginx.com/resources/wiki/start/topics/examples/server_blocks/
 
 .. _Jellyfin: https://jellyfin.org/
 .. _external alternative audio tracks:
    https://jellyfin.org/docs/general/server/media/external-audio-files.html
@@ -401,8 +459,8 @@
    https://gitlab.com/rpatterson/feed-archiver/blob/master/docker-compose.yml
 
 .. _`This project is hosted on GitLab`:
    https://gitlab.com/rpatterson/feed-archiver
 .. _`a mirror on GitHub`:
    https://github.com/rpatterson/feed-archiver
 .. _`the ./CONTRIBUTING.rst file`:
-   https://gitlab.com/rpatterson/feed-archiver/blob/master/CONTRIBUTING.rst
+   https://gitlab.com/rpatterson/feed-archiver/blob/main/CONTRIBUTING.rst
```

### Comparing `feed-archiver-1.0.0/src/feed_archiver.egg-info/SOURCES.txt` & `feed-archiver-1.0.0b11/src/feed_archiver.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,77 +1,119 @@
 .dir-locals.el.in
 .dockerignore
 .env.in
 .gitignore
 .gitlab-ci.yml
 .pre-commit-config.yaml
+.prospector.yaml
 CONTRIBUTING.rst
 Dockerfile
 Dockerfile.devel
 LICENSE
 Makefile
+NEWS-VERSION.rst
 NEWS.rst
 README.rst
 TODO.rst
+docker-compose-servarr.yml
 docker-compose.override.yml
 docker-compose.yml
+link-fallbacks.feature.rst
 pyproject.toml
-requirements-build.txt
-requirements-build.txt.in
-requirements-devel.txt
-requirements.txt
 setup.cfg
 tox.ini
-.github/workflows/ci-cd.yml
+.github/workflows/build-test.yml
+bin/cz-check-bump
 bin/entrypoint
+bin/get-base-version
+bin/hadolint
+build-host/Dockerfile
+build-host/Makefile
+build-host/README.rst
+build-host/requirements-py310.txt
+build-host/requirements-py311.txt
+build-host/requirements-py37.txt
+build-host/requirements-py38.txt
+build-host/requirements-py39.txt
+build-host/requirements.txt.in
+build-host/bin/entrypoint
+dist/.gitignore
+gitlab-runner/.gitignore
+gitlab-runner/config/config.toml.in
 home/.gitignore
 home/.pypirc.in
 nginx/templates/default.conf.template
+requirements/build.txt.in
+requirements/py310/build.txt
+requirements/py310/devel.txt
+requirements/py310/user.txt
+requirements/py311/build.txt
+requirements/py311/devel.txt
+requirements/py311/user.txt
+requirements/py37/build.txt
+requirements/py37/devel.txt
+requirements/py37/user.txt
+requirements/py38/build.txt
+requirements/py38/devel.txt
+requirements/py38/user.txt
+requirements/py39/build.txt
+requirements/py39/devel.txt
+requirements/py39/user.txt
 server/docker-compose.yml
 src/feed_archiver.egg-info/PKG-INFO
 src/feed_archiver.egg-info/SOURCES.txt
 src/feed_archiver.egg-info/dependency_links.txt
 src/feed_archiver.egg-info/entry_points.txt
 src/feed_archiver.egg-info/requires.txt
 src/feed_archiver.egg-info/top_level.txt
 src/feedarchiver/__init__.py
 src/feedarchiver/__main__.py
 src/feedarchiver/archive.py
 src/feedarchiver/feed.py
 src/feedarchiver/formats.py
 src/feedarchiver/utils.py
 src/feedarchiver/version.py
-src/feedarchiver/linkpaths/__init__.py
-src/feedarchiver/linkpaths/servarr.py
-src/feedarchiver/linkpaths/template.py
+src/feedarchiver/enclosures/__init__.py
+src/feedarchiver/enclosures/servarr.py
+src/feedarchiver/enclosures/template.py
 src/feedarchiver/newsfragments/.gitignore
+src/feedarchiver/newsfragments/request-timeouts.fix.rst
 src/feedarchiver/tests/__init__.py
 src/feedarchiver/tests/test_archive.py
 src/feedarchiver/tests/test_cli.py
 src/feedarchiver/tests/test_download.py
 src/feedarchiver/tests/test_feed.py
 src/feedarchiver/tests/test_linking.py
 src/feedarchiver/tests/test_urls.py
 src/feedarchiver/tests/archives/downloads/.feed-archiver.yml
+src/feedarchiver/tests/archives/empty/.gitignore
+src/feedarchiver/tests/archives/empty-feeds/.feed-archiver.yml
+src/feedarchiver/tests/archives/empty-items/.feed-archiver.yml
 src/feedarchiver/tests/archives/end-to-end/.feed-archiver.yml.in
+src/feedarchiver/tests/archives/relink/.feed-archiver.yml
+src/feedarchiver/tests/archives/relink-wo-suffix/.feed-archiver.yml
 src/feedarchiver/tests/archives/simple/.feed-archiver.yml
 src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/episode%3Fapikey=secret%26seriesId=7
 src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/episodeFile%3Fapikey=secret%26seriesId=7
 src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/series%3Fapikey=secret
 src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/series/7%3Fapikey=secret
 src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/media/common-id.mp3
 src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/media/el-ni%25C3%25B1o.mp3
 src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/common-id.mp3
 src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/feed.rss
 src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/image.png
 src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/index.html
+src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/bah-episode-title/download.mp3
+src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/bah-episode-title/index.html
 src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/download
 src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/el-ni%25C3%25B1o.png
 src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/index.html
 src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/fred-episode-title/download
+src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/garply-bonus-episode/download.mp3
+src/feedarchiver/tests/remotes/empty-items/orig/https/foo.example.com/podcast/empty.rss
 src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/main.html
 src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/1
 src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/2
 src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/3
 src/feedarchiver/tests/remotes/simple/added-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss
 src/feedarchiver/tests/remotes/simple/added-item/https/waldo.example.com/feeds/waldo
 src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/main.html
```

### Comparing `feed-archiver-1.0.0/src/feedarchiver/archive.py` & `feed-archiver-1.0.0b11/src/feedarchiver/archive.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,22 +3,25 @@
 """
 
 import os
 import pathlib
 import urllib.parse
 import logging
 import tracemalloc
+import pdb
 
 import yaml
-import requests
+import httpx
 import user_agent
+from lxml import etree  # nosec B410
+from lxml.html import builder  # nosec B410
 
 from . import utils
 from . import feed
-from . import linkpaths
+from . import enclosures
 from .utils import mimetypes
 
 logger = logging.getLogger(__name__)
 
 
 class Archive:  # pylint: disable=too-many-instance-attributes
     """
@@ -27,15 +30,16 @@
 
     INDEX_BASENAME = "index.html"
 
     FEED_CONFIGS_BASENAME = ".feed-archiver.yml"
 
     # Initialized when the configuration is loaded prior to update
     global_config = None
-    link_path_plugins = None
+    enclosure_plugins = None
+    enclosure_fallack_plugins = None
     # The default base URL for assembling absolute URLs
     url = url_split = None
     archive_feeds = None
 
     def __init__(self, root_dir, recreate=False):
         """
         Instantiate a representation of an archive from a file-system path.
@@ -43,43 +47,45 @@
         if utils.PYTHONTRACEMALLOC:  # pragma: no cover
             # Optionally initialize memory profiling
             self.tracemalloc_snapshot = tracemalloc.take_snapshot()
 
         self.root_path = pathlib.Path(root_dir)
         self.root_stat = os.statvfs(self.root_path)
         self.config_path = self.root_path / self.FEED_CONFIGS_BASENAME
-        assert (
-            self.config_path.is_file()
-        ), f"Feeds definition path is not a file: {self.config_path}"
+        if not self.config_path.is_file():
+            raise ValueError(f"Feeds definition path is not a file: {self.config_path}")
 
         self.recreate = recreate
 
-        self.requests = requests.Session()
+        self.client = httpx.Client(follow_redirects=True)
         # Avoid bot detection, real-world `User-Agent` HTTP header values
-        self.requests.headers.update({"User-Agent": user_agent.generate_user_agent()})
+        self.client.headers.update({"User-Agent": user_agent.generate_user_agent()})
 
     def load_config(self):
         """
         Read and deserialize the archive feed configs and do necessary pre-processing.
         """
         logger.debug(
             "Retrieving feed configurations: %r",
             str(self.config_path),
         )
-        with self.config_path.open() as feeds_opened:
+        with self.config_path.open(encoding="utf-8") as feeds_opened:
             archive_config = yaml.safe_load(feeds_opened)
 
         # The first row after the header defines defaults and/or global options
         self.global_config = archive_config["defaults"]
         self.url = self.global_config["base-url"]
         self.url_split = urllib.parse.urlsplit(self.global_config["base-url"])
-        self.link_path_plugins = list(linkpaths.load_plugins(self, self.global_config))
+        (
+            self.enclosure_plugins,
+            self.enclosure_fallack_plugins,
+        ) = enclosures.load_plugins(self, self.global_config)
 
         feed_configs = archive_config["feeds"]
-        if not feed_configs:  # pragma: no cover
+        if not feed_configs:
             raise ValueError(f"No feeds defined: {str(self.config_path)!r}")
 
         self.archive_feeds = []
         for feed_config in feed_configs:
             archive_feed = feed.ArchiveFeed(
                 archive=self,
                 config=feed_config,
@@ -104,15 +110,15 @@
         doesn't match a `Content-Type` header.
         """
         if request is None:  # pragma: no cover
             if url_response.history:
                 request = url_response.history[0].request
             else:
                 request = url_response.request
-        url_path = self.url_to_path(request.url)
+        url_path = self.url_to_path(str(request.url))
         mime_type = None
 
         # First try to get the MIME type from the response headers
         if url_response.headers.get("Content-Type"):
             mime_type = utils.parse_content_type(
                 url_response.headers["Content-Type"],
             )
@@ -158,39 +164,40 @@
             pathlib.Path(
                 utils.quote_basename(split_url.scheme),
                 utils.quote_basename(split_url.netloc),
             )
             / pathlib.Path(
                 *(utils.quote_basename(part) for part in url_path.parent.parts),
             )
-            / url_path.with_stem(
-                # Place the query and fragment from the URL before the extension/suffix
-                # in the path
+            # Place the query and fragment from the URL before the extension/suffix in
+            # the path
+            / (
                 utils.quote_basename(
                     split_url._replace(
-                        scheme="", netloc="", path=url_path.stem
+                        scheme="",
+                        netloc="",
+                        path=url_path.stem,
                     ).geturl(),
                 )
-            ).name
+                + url_path.suffix
+            )
         )
         # Translate back to platform-native filesystem path separators/slashes
         return self.truncate_path_parts(archive_path)
 
     def truncate_path_parts(self, path):
         """
         Truncate the basenames of each part of the path to the filesystem maximum.
         """
         truncated_path = pathlib.Path()
         for part in path.parts:
             part_path = pathlib.Path(part)
-            truncated_path = (
-                truncated_path
-                / part_path.with_stem(
-                    part_path.stem[: self.root_stat.f_namemax - len(part_path.suffix)],
-                ).name
+            truncated_path = truncated_path / (
+                part_path.stem[: self.root_stat.f_namemax - len(part_path.suffix)]
+                + part_path.suffix
             )
         return truncated_path
 
     def path_to_url(self, path):
         """
         Un-escape the safe file-system path within the archive to a URL.
         """
@@ -220,30 +227,81 @@
         split_url = stem_split._replace(
             scheme=urllib.parse.unquote(archive_path.parts[0]),
             netloc=urllib.parse.unquote(archive_path.parts[1]),
             path=url_relative,
         )
         return split_url.geturl()
 
-    def update(self):
+    def run_feeds_command(self, command, *args, **kwargs):
         """
-        Request the URL of each feed in the archive and update contents accordingly.
+        Call the sub-command for each feed handling exceptions and aggregating results.
         """
         self.load_config()
-        updated_feeds = {}
+        results = {}
         for archive_feed in self.archive_feeds:
+            feed_command = getattr(archive_feed, command)
             try:
-                updated_items, download_paths = archive_feed.update()
-            except Exception:  # pragma: no cover, pylint: disable=broad-except
+                feed_results = feed_command(*args, **kwargs)
+            except Exception:  # pylint: disable=broad-except
                 logger.exception(
                     "Unhandled exception updating feed: %r",
                     archive_feed.url,
                 )
                 if utils.POST_MORTEM:  # pragma: no cover
-                    raise
+                    pdb.post_mortem()
                 continue
-            if updated_items or download_paths:  # pragma: no cover
-                updated_feeds[archive_feed.url] = updated_items, download_paths
+            if feed_results:
+                results[archive_feed.url] = feed_results
             if utils.PYTHONTRACEMALLOC:  # pragma: no cover
                 # Optionally compare memory consumption
                 self.tracemalloc_snapshot = utils.compare_memory_snapshots(archive_feed)
-        return updated_feeds
+        if results:
+            return results
+        return None
+
+    # Sub-commands
+
+    def update(self):
+        """
+        Request the URL of each feed in the archive and update contents accordingly.
+        """
+        feeds_results = self.run_feeds_command("update")
+        html = builder.HTML(
+            builder.HEAD(
+                builder.TITLE("Feed Archive Index"),
+            ),
+            builder.BODY(
+                builder.H1("Feed Archive Index"),
+                builder.P(
+                    "Use the links below to subscribe to the feeds archived here:",
+                ),
+                builder.UL(
+                    *(
+                        builder.LI(
+                            builder.A(
+                                archive_feed.config.get(
+                                    "title",
+                                    archive_feed.config.get(
+                                        "name",
+                                        str(archive_feed.path),
+                                    ),
+                                ),
+                                href=str(archive_feed.path),
+                            ),
+                        )
+                        for archive_feed in self.archive_feeds
+                    )
+                ),
+            ),
+        )
+        logger.info(
+            "Writing HTML index: %s",
+            self.root_path / "index.html",
+        )
+        etree.ElementTree(html).write(self.root_path / "index.html", pretty_print=True)
+        return feeds_results
+
+    def relink(self):
+        """
+        Re-link enclosures to the correct locations for the current configuration.
+        """
+        return self.run_feeds_command("relink")
```

### Comparing `feed-archiver-1.0.0/src/feedarchiver/feed.py` & `feed-archiver-1.0.0b11/src/feedarchiver/feed.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,41 +1,42 @@
-# pylint: disable=too-many-lines
 """
 An RSS/Atom syndication feed in an archive.
 """
 
 import os
 import copy
 import re
 import urllib
 import email.utils
 import pathlib
 import logging
+import pdb
 
-from lxml import etree
-from requests_toolbelt.downloadutils import stream
+from lxml import etree  # nosec B410
 
 from . import utils
+from .utils import mimetypes
 from . import formats
-from . import linkpaths
+from . import enclosures
 
 logger = logging.getLogger(__name__)
 
 
 class ArchiveFeed:
     """
     An RSS/Atom syndication feed in an archive.
     """
 
     URL_SCHEME_RE = re.compile(r"^(?P<scheme>[a-zA-Z][a-zA-Z0-9+.-]*):$")
     NAMESPACE = "https://github.com/rpatterson/feed-archiver"
 
     # Initialized when the configuration is loaded prior to update
     url = None
-    link_path_plugins = None
+    enclosure_plugins = None
+    enclosure_fallack_plugins = None
     # Initialized on update from the response to the request for the URL from the feed
     # config in order to use response headers to derrive the best path.
     path = None
 
     def __init__(self, archive, config):
         """
         Instantiate a representation of an archive from a file-system path.
@@ -48,47 +49,55 @@
         self.config = config
 
     def load_config(self):
         """
         Pre-process and validate the feed config prior to running the actual update.
         """
         self.url = self.config["remote-url"]
-        self.link_path_plugins = self.archive.link_path_plugins + list(
-            linkpaths.load_plugins(self, self.config),
+        self.enclosure_plugins = self.archive.enclosure_plugins[:]
+        self.enclosure_fallack_plugins = self.archive.enclosure_fallack_plugins[:]
+        enclosure_plugins, enclosure_fallack_plugins = enclosures.load_plugins(
+            self,
+            self.config,
         )
+        self.enclosure_plugins.extend(enclosure_plugins)
+        self.enclosure_fallack_plugins.extend(enclosure_fallack_plugins)
 
-    def update(
+    # Sub-commands
+
+    # TODO: Refactor to reduce complexity and improve readability and testibility
+    def update(  # noqa: MC0001
         self,
     ):  # pylint: disable=too-many-locals,too-many-statements,too-many-branches
         """
         Request the URL of one feed in the archive and update contents accordingly.
         """
-        logger.info("Requesting feed: %r", self.url)
-        remote_response = self.archive.requests.get(self.url)
+        logger.debug("Requesting feed: %r", self.url)
+        remote_response = self.archive.client.get(self.url)
         # Maybe update the extension based on the headers
         self.path = self.archive.root_path / self.archive.response_to_path(
             remote_response,
         )
         remote_tree = self.load_remote_tree(remote_response)
         remote_root = remote_tree.getroot()
         remote_format = formats.FeedFormat.from_tree(self, remote_tree)
 
         # Assemble the archive version of the feed XML
         download_paths = {}
-        archive_tree = self.load_archive_tree(
-            remote_format,
+        archive_tree = self.get_archive_tree(
             remote_tree,
             download_paths,
+            remote_format=remote_format,
         )
         archive_root = archive_tree.getroot()
         archived_items_parent = remote_format.get_items_parent(archive_root)
 
         remote_item_elems = list(remote_format.iter_items(remote_root))
         archive_item_elems = list(remote_format.iter_items(archive_root))
-        if (len(remote_item_elems) - len(archive_item_elems)) > 4:  # pragma: no cover
+        if (len(remote_item_elems) - len(archive_item_elems)) > 4:
             logger.warning(
                 "Many more items in remote than archive: %s > %s",
                 len(remote_item_elems),
                 len(archive_item_elems),
             )
 
         logger.info(
@@ -154,79 +163,153 @@
                 # by adding this remote item.
                 logger.info(
                     "Adding feed item to archive: %r -> %r",
                     remote_item_id,
                     str(self.path),
                 )
 
-                item_download_paths = self.download_item_content(
+                item_download_paths = self.download_item_enclosures(
                     remote_format,
                     remote_item_elem,
                     remote_item_id,
                 )
-                if item_download_paths is None:  # pragma: no cover
+                if item_download_paths is None:
                     continue
                 (
-                    item_download_asset_paths,
-                    item_download_content_paths,
+                    item_asset_paths,
+                    item_enclosure_paths,
                 ) = item_download_paths
-                download_paths.update(item_download_asset_paths)
-                download_paths.update(item_download_content_paths)
+                download_paths.update(item_asset_paths)
+                download_paths.update(item_enclosure_paths)
                 updated_items[remote_item_id] = remote_item_elem
 
-                self.link_item_content(
+                self.link_item_enclosures(
+                    remote_format=remote_format,
                     feed_elem=archived_items_parent,
                     item_elem=remote_item_elem,
-                    item_content_paths=item_download_content_paths,
+                    item_enclosure_paths=item_enclosure_paths,
                 )
 
                 archived_items_parent.insert(first_item_idx, remote_item_elem)
-                if updated_items or download_paths:  # pragma: no cover
-                    # Pretty format the feed for readability
-                    etree.indent(archive_tree)
-                    # Update the archived feed file
-                    archive_tree.write(str(self.path))
+                # Pretty format the feed for readability
+                etree.indent(archive_tree)
+                # Update the archived feed file
+                archive_tree.write(str(self.path))
 
         update_download_metadata(remote_response, self.path)
 
-        return list(updated_items.keys()), {
-            # Return values fit for CLI output
-            download_url: str(download_path)
-            for download_url, download_path in download_paths.items()
-        }
+        if updated_items or download_paths:
+            return list(updated_items.keys()), {
+                # Return values fit for CLI output
+                download_url: str(download_path)
+                for download_url, download_path in download_paths.items()
+            }
+        return None
+
+    # TODO: Refactor to reduce complexity and improve readability and testibility
+    def relink(self):  # noqa: MC0001
+        """
+        Re-link enclosures to the correct locations for this feed.
+        """
+        # Parse this feed's archive XML
+        self.path = self.find_archive_path()
+        archive_tree = self.load_archive_tree()
+        archive_format = formats.FeedFormat.from_tree(self, archive_tree)
+        attr_prefixes = [
+            f"{{{self.NAMESPACE}}}enclosure-link-",
+            # BBB: old format compatibility
+            f"{{{self.NAMESPACE}}}content-link-",
+        ]
 
-    def download_item_content(self, remote_format, remote_item_elem, remote_item_id):
+        # Update the links for each item in this feed
+        is_modified = False
+        linked_enclosures = {}
+        for archive_item_elem in archive_format.iter_items(archive_tree.getroot()):
+            item_enclosure_paths = {}
+            for url_result in formats.all_xpaths_results(
+                archive_item_elem,
+                archive_format.DOWNLOAD_ITEM_ENCLOSURE_URLS_XPATHS,
+            ):
+                for attr, attr_value in list(url_result.getparent().attrib.items()):
+                    for attr_prefix in attr_prefixes:
+                        if attr.startswith(attr_prefix):
+                            break
+                    else:
+                        continue
+                    enclosure_path = pathlib.Path(attr_value)
+                    if enclosure_path.is_symlink():
+                        logger.info(
+                            "Deleting existing enclosure link: %r -> %r",
+                            str(enclosure_path),
+                            str(os.readlink(enclosure_path)),
+                        )
+                        enclosure_path.unlink()
+                    del url_result.getparent().attrib[attr]
+                    is_modified = True
+                item_enclosure_paths[url_result] = pathlib.Path(
+                    urllib.parse.unquote(
+                        urllib.parse.urlsplit(url_result).path.lstrip("/"),
+                    ),
+                )
+            item_enclosures = self.link_item_enclosures(
+                remote_format=archive_format,
+                feed_elem=archive_format.get_items_parent(archive_tree.getroot()),
+                item_elem=archive_item_elem,
+                item_enclosure_paths=item_enclosure_paths,
+            )
+            if item_enclosures:
+                is_modified = True
+            if is_modified:  # pragma: no cover
+                # Pretty format the feed for readability
+                etree.indent(archive_tree)
+                # Update the archived feed file
+                archive_tree.write(str(self.path))
+            linked_enclosures.update(
+                (
+                    url_result,
+                    # Make results JSON serializable for CLI stdout
+                    [str(enclosure_path) for enclosure_path in enclosure_paths],
+                )
+                for url_result, enclosure_paths in item_enclosures.items()
+            )
+        if linked_enclosures:
+            return linked_enclosures
+        return None
+
+    # Other methods
+
+    def download_item_enclosures(self, remote_format, remote_item_elem, remote_item_id):
         """
-        Download all the enclosures/content from a feed item.
+        Download all the enclosures from a feed item.
         """
-        item_download_asset_urls = formats.all_xpaths_results(
+        item_asset_urls = formats.all_xpaths_results(
             remote_item_elem,
             remote_format.DOWNLOAD_ITEM_ASSET_URLS_XPATHS,
         )
-        item_download_content_urls = formats.all_xpaths_results(
+        item_enclosure_urls = formats.all_xpaths_results(
             remote_item_elem,
-            remote_format.DOWNLOAD_ITEM_CONTENT_URLS_XPATHS,
+            remote_format.DOWNLOAD_ITEM_ENCLOSURE_URLS_XPATHS,
         )
         try:
             # Download enclosures and assets only for this item.
-            item_download_asset_paths = self.download_urls(
-                item_download_asset_urls,
+            item_asset_paths = self.download_urls(
+                item_asset_urls,
             )
-            item_download_content_paths = self.download_urls(
-                item_download_content_urls,
+            item_enclosure_paths = self.download_urls(
+                item_enclosure_urls,
             )
-        except Exception:  # pragma: no cover, pylint: disable=broad-except
+        except Exception:  # pylint: disable=broad-except
             logger.exception(
                 "Problem downloading item URLs, continuing to next: %r",
                 remote_item_id,
             )
-            if utils.POST_MORTEM:
-                raise
+            if utils.POST_MORTEM:  # pragma: no cover
+                pdb.post_mortem()
             return None
-        return item_download_asset_paths, item_download_content_paths
+        return item_asset_paths, item_enclosure_paths
 
     def update_self(self, feed_format, archive_root):
         """
         Update the `<link rel="self" href="..." ...` URL in the archived feed.
 
         Use the absolute URL so that it can be used as a base URL for other URLs in the
         feed XML.
@@ -246,63 +329,99 @@
     def load_remote_tree(self, remote_response):
         """
         Request the feed from the remote URL, parse the XML, and return the tree.
 
         Also do any pre-processing needed to start updating the archive.
         """
         logger.debug("Parsing remote XML: %r", self.url)
-        remote_root = etree.fromstring(
+        remote_root = etree.fromstring(  # nosec: B320
             remote_response.content,
-            base_url=remote_response.url,
+            base_url=str(remote_response.url),
+            parser=utils.XML_PARSER,
         )
         return etree.ElementTree(remote_root)
 
-    def load_archive_tree(self, remote_format, remote_tree, download_paths):
+    def find_archive_path(self):
         """
-        Parse the local feed XML in the archive and return the tree.
-
-        If there is no local feed XML in the archive, such as the first time the feed is
-        updated, then initialize the archive tree from the remote tree.
+        Locate this feed's file in the archive.
+        """
+        path = self.archive.root_path / self.archive.url_to_path(self.url)
+        if not path.exists():
+            archive_files = []
+            for archive_file in path.parent.glob(f"{path.stem}.*"):
+                guessed_type, _ = mimetypes.guess_type(archive_file)
+                if guessed_type is not None and (
+                    guessed_type.endswith("/xml") or guessed_type.endswith("+xml")
+                ):
+                    archive_files.append(archive_file)
+            if not archive_files:
+                raise ValueError(f"Could not locate feed in archive: {self.url}")
+            if len(archive_files) > 1:
+                logger.warning(
+                    "Multiple XML files found for feed, using first: %s\n%s",
+                    self.url,
+                    "\n  ".join([str(archive_file) for archive_file in archive_files]),
+                )
+            path = archive_files[0]
+        return path
 
-        Also do any pre-processing needed to start updating the archive.
+    def load_archive_tree(self):
+        """
+        Parse the local feed XML in the archive and return the tree.
         """
         archive_tree = None
         if (
             not self.archive.recreate
             and self.path.exists()
             and self.path.read_text().strip()
         ):
             logger.debug("Parsing archive XML: %r", self.url)
             with self.path.open() as feed_archive_opened:
                 # Try to parse the local archive version of the feed if possible.  If
                 # there are errors parsing it, then treat it as if it's the first time
                 # archiving this feed.
                 try:
-                    archive_tree = etree.parse(feed_archive_opened)
+                    archive_tree = etree.parse(  # nosec B320
+                        feed_archive_opened,
+                        parser=utils.XML_PARSER,
+                    )
                 except SyntaxError:
                     logger.exception(
                         "Unhandled exception parsing archive feed: %r",
                         self.url,
                     )
                     if utils.POST_MORTEM:  # pragma: no cover
-                        raise
-            if archive_tree is not None:
-                archive_format = formats.FeedFormat.from_tree(self, remote_tree)
+                        pdb.post_mortem()
+        return archive_tree
+
+    def get_archive_tree(self, remote_tree, download_paths, remote_format=None):
+        """
+        Parse the archive feed XML if it exists or initialize an empty archive feed.
+
+        If there is no local feed XML in the archive, such as the first time the feed is
+        updated, then initialize the archive tree from the remote tree.
+
+        Also do any pre-processing needed to start updating the archive.
+        """
+        archive_tree = self.load_archive_tree()
+        if archive_tree is not None:
+            if remote_format is not None:  # pragma: no cover
+                archive_format = formats.FeedFormat.from_tree(self, archive_tree)
                 if not isinstance(
                     archive_format,
                     type(remote_format),
                 ):  # pragma: no cover
                     raise NotImplementedError(
                         f"Remote feed format, {type(remote_format).__name__!r}, is "
                         "different from archive format, "
                         f"{type(archive_format).__name__!r}."
                     )
-                archive_root = archive_tree.getroot()
-                archived_items_parent = remote_format.get_items_parent(archive_root)
-        if archive_tree is None:
+            archive_root = archive_tree.getroot()
+            archived_items_parent = remote_format.get_items_parent(archive_root)
+        else:
             # First time requesting this feed, copy the remote feed, minus the items to
             # the archive and download the feed-level assets.
             logger.info(
                 "Initializing feed in archive: %r -> %r",
                 self.url,
                 str(self.path),
             )
@@ -341,15 +460,19 @@
                 str(self.path),
             )
             etree.indent(archive_tree)
             archive_tree.write(str(self.path))
 
         return archive_tree
 
-    def download_urls(self, url_results):  # pylint: disable=too-many-branches
+    # TODO: Refactor to reduce complexity and improve readability and testibility
+    def download_urls(  # noqa: MC0001
+        self,
+        url_results,
+    ):  # pylint: disable=too-many-branches
         """
         Escape URLs to archive paths, download if new, and update URLs.
         """
         downloaded_paths = {}
         excs = {}
         for url_result in url_results:
             if url_result == self.url:
@@ -363,77 +486,69 @@
                 logger.debug("Duplicate URL, skipping download: %r", url_result)
                 # Proceed below to update the URLs in the duplicate XML element
                 download_path = self.archive.root_path / downloaded_paths[url_result]
             else:
                 # Download the URL to the escaped local path in the archive
                 try:
                     download_path = self.download_url(url_result)
-                except (
-                    Exception  # pylint: disable=broad-except
-                ) as exc:  # pragma: no cover
+                except Exception as exc:  # pylint: disable=broad-except
                     excs[url_result] = exc
                     logger.exception(
                         "Problem downloading URL, removing from archive: %r",
                         url_result,
                     )
-                    if download_path is not None:
+                    if download_path is not None:  # pragma: no cover
                         download_path.unlink()
                     if utils.POST_MORTEM:  # pragma: no cover
-                        raise
+                        pdb.post_mortem()
                     continue
                 downloaded_paths[url_result] = download_path.relative_to(
                     self.archive.root_path,
                 )
 
             # Update the URL in the feed XML to the relative archive path.
             # Update only after successful download to minimize inconsistent state on
             # errors.
-            if hasattr(url_result, "getparent") and hasattr(url_result, "attrname"):
-                url_parent = url_result.getparent()
-                download_relative = downloaded_paths[url_result]
-                if download_relative.name == self.archive.INDEX_BASENAME:
-                    download_relative = download_relative.parent
-                download_url_split = self.archive.url_split._replace(
-                    # Let pathlib normalize the relative path
-                    path=str(
-                        pathlib.PurePosixPath(self.archive.url_split.path)
-                        / urllib.parse.quote(str(download_relative))
-                    ),
-                )
-                if url_result.attrname:
-                    logger.debug(
-                        'Updating feed URL: <%s %s="%s"...>',
-                        url_result.getparent().tag,
-                        url_result.attrname,
-                        download_url_split.geturl(),
-                    )
-                    # Store the original remote URL in a namespace attribute
-                    url_parent.attrib[
-                        f"{{{self.NAMESPACE}}}attribute-{url_result.attrname}"
-                    ] = url_result
-                    # Update the archived URL to the local, relative URL
-                    url_parent.attrib[url_result.attrname] = download_url_split.geturl()
-                else:
-                    logger.debug(
-                        "Updating feed URL: <%s>%s</%s>",
-                        url_result.getparent().tag,
-                        download_url_split.geturl(),
-                        url_result.getparent().tag,
-                    )
-                    # Store the original remote URL in a namespace attribute
-                    url_parent.attrib[f"{{{self.NAMESPACE}}}text"] = url_result
-                    # Update the URL in the archive XML to the local, relative URL
-                    url_parent.text = download_url_split.geturl()
-            else:  # pragma: no coverx
-                raise NotImplementedError(
-                    f"Escaping URLs in {type(url_result)!r} text nodes"
-                    " not implemented yet",
-                )
+            url_parent = url_result.getparent()
+            download_relative = downloaded_paths[url_result]
+            if download_relative.name == self.archive.INDEX_BASENAME:
+                download_relative = download_relative.parent
+            download_url_split = self.archive.url_split._replace(
+                # Let pathlib normalize the relative path
+                path=str(
+                    pathlib.PurePosixPath(self.archive.url_split.path)
+                    / urllib.parse.quote(str(download_relative))
+                ),
+            )
+            if url_result.attrname:
+                logger.debug(
+                    'Updating feed URL: <%s %s="%s"...>',
+                    url_result.getparent().tag,
+                    url_result.attrname,
+                    download_url_split.geturl(),
+                )
+                # Store the original remote URL in a namespace attribute
+                url_parent.attrib[
+                    f"{{{self.NAMESPACE}}}attribute-{url_result.attrname}"
+                ] = url_result
+                # Update the archived URL to the local, relative URL
+                url_parent.attrib[url_result.attrname] = download_url_split.geturl()
+            else:
+                logger.debug(
+                    "Updating feed URL: <%s>%s</%s>",
+                    url_result.getparent().tag,
+                    download_url_split.geturl(),
+                    url_result.getparent().tag,
+                )
+                # Store the original remote URL in a namespace attribute
+                url_parent.attrib[f"{{{self.NAMESPACE}}}text"] = url_result
+                # Update the URL in the archive XML to the local, relative URL
+                url_parent.text = download_url_split.geturl()
 
-        if excs:  # pragma: no cover
+        if excs:
             # Ensure the feed item is processed again if any problem occurred with with
             # it's downloads
             raise list(excs.values())[0]
         return downloaded_paths
 
     def resolve_url(self, url):
         """
@@ -477,250 +592,269 @@
 
     def download_url(self, url_result):
         """
         Request a URL and stream the response to the file.
         """
         logger.info("Downloading URL into archive: %r", url_result)
         url_split = self.resolve_url(url_result)
-        with self.archive.requests.get(
+        with self.archive.client.stream(
+            "GET",
             url_split.geturl(),
-            stream=True,
         ) as download_response:
             download_path = self.archive.root_path / self.archive.response_to_path(
                 download_response,
                 url_result,
             )
             download_relative = download_path.relative_to(self.archive.root_path)
             if download_path.exists():
                 logger.debug(
                     "Skipping download already in archive: %r",
                     str(download_relative),
                 )
                 return download_path
             logger.debug("Writing download into archive: %r", str(download_relative))
             download_path.parent.mkdir(parents=True, exist_ok=True)
-            stream.stream_response_to_file(download_response, path=download_path)
-        download_stat = download_path.stat()
+            with download_path.open("wb") as download_opened:
+                for data in download_response.iter_bytes():
+                    download_opened.write(data)
 
         update_download_metadata(download_response, download_path)
 
-        if (
-            download_response.headers.get(
-                "Content-Encoding",
-                "binary",
-            )
-            .strip()
-            .lower()
-            == "binary"
-            and "Content-Length" in download_response.headers
-        ):
-            try:
-                remote_content_length = int(
-                    download_response.headers["Content-Length"].strip(),
-                )
-            except ValueError:  # pragma: no cover
-                pass
-            else:
-                if download_stat.st_size != remote_content_length:  # pragma: no cover
-                    logger.error(
-                        "Downloaded content size different from remote: %r -> %r",
-                        download_stat.st_size,
-                        remote_content_length,
-                    )
-
         return download_path
 
-    def link_item_content(
+    def link_item_enclosures(
         self,
+        remote_format,
         feed_elem,
         item_elem,
-        item_content_paths,
-    ):  # pylint: disable=too-many-branches
+        item_enclosure_paths,
+    ):
         """
-        Link item content/enclosures into media library hierarchies using plugins.
+        Link item enclosures into media library hierarchies using plugins.
         """
-        content_link_paths = {}
+        link_paths = {}
+        if not self.enclosure_plugins and not self.enclosure_fallack_plugins:
+            # Avoid unnecessary work when no link plugins are configured, particularly
+            # parsing the item with `feedparser`.
+            return link_paths
+
+        feed_parsed = utils.parse_item_feed(remote_format, feed_elem, item_elem)
+        (item_parsed,) = feed_parsed.entries
         for (
             url_result,
-            content_archive_relative,
-        ) in item_content_paths.items():
-            basename = content_archive_relative.name
+            enclosure_path,
+        ) in item_enclosure_paths.items():
             link_idx = 0
-            for link_path_plugin in self.link_path_plugins:
-                for content_link_path in self.list_item_content_link_plugin_paths(
+            for enclosure_plugin in self.enclosure_plugins:
+                for link_path in self.list_plugin_enclosure_links(
                     feed_elem,
+                    feed_parsed,
                     item_elem,
+                    item_parsed,
                     url_result,
-                    basename,
-                    content_archive_relative,
-                    link_path_plugin,
+                    enclosure_path,
+                    enclosure_plugin,
                 ):
-                    content_link_paths.setdefault(url_result, []).append(
+                    link_paths.setdefault(url_result, []).append(
                         self.link_plugin_file(
                             url_result,
-                            content_archive_relative,
-                            content_link_path,
+                            enclosure_path,
+                            link_path,
                             link_idx,
                         )
                     )
                     link_idx += 1
-        return content_link_paths
+            if link_idx > 0:
+                # At least one plugin linked the enclosure, skip the fallbacks
+                continue
+            # Link and fallback configurations for this enclosure
+            for enclosure_plugin in self.enclosure_fallack_plugins:
+                for link_path in self.list_plugin_enclosure_links(
+                    feed_elem,
+                    feed_parsed,
+                    item_elem,
+                    item_parsed,
+                    url_result,
+                    enclosure_path,
+                    enclosure_plugin,
+                ):
+                    link_paths.setdefault(url_result, []).append(
+                        self.link_plugin_file(
+                            url_result,
+                            enclosure_path,
+                            link_path,
+                            link_idx,
+                        )
+                    )
+                    link_idx += 1
+        return link_paths
 
-    def list_item_content_link_plugin_paths(
+    def list_plugin_enclosure_links(
         self,
         feed_elem,
+        feed_parsed,
         item_elem,
+        item_parsed,
         url_result,
-        basename,
-        content_archive_relative,
-        link_path_plugin,
+        enclosure_path,
+        enclosure_plugin,
     ):  # pylint: disable=too-many-arguments
         """
-        Return the content link paths for an individual download and plugin.
+        Return the links for an individual enclosure and plugin.
         """
+        kwargs = {}
         match = None
-        if "match-re" in link_path_plugin.config:
+        if "match-re" in enclosure_plugin.config:
             match_kwargs = locals().copy()
             del match_kwargs["self"]
             match = self.link_item_plugin_match(**match_kwargs)
             if match is None:
                 return []
+            kwargs.update(match.groupdict())
 
         # Delegate to the plugin
         logger.debug(
-            "Linking item content with %r plugin: %s",
-            type(link_path_plugin),
-            str(content_archive_relative),
+            "Linking item enclosure with %r plugin: %s",
+            type(enclosure_plugin),
+            str(enclosure_path),
         )
         try:
-            content_link_strs = link_path_plugin(
+            link_strs = enclosure_plugin(
                 archive_feed=self,
                 feed_elem=feed_elem,
+                feed_parsed=feed_parsed,
                 item_elem=item_elem,
+                item_parsed=item_parsed,
                 url_result=url_result,
-                basename=basename,
+                enclosure_path=enclosure_path,
                 match=match,
+                **kwargs,
             )
-        except Exception:  # pragma: no cover, pylint: disable=broad-except
+        except Exception:  # pylint: disable=broad-except
             logger.exception(
-                "Problem linking item content with %r, continuing to next: %s",
-                type(link_path_plugin),
-                str(content_archive_relative),
+                "Problem linking item enclosure with %r, continuing to next: %s",
+                type(enclosure_plugin),
+                str(enclosure_path),
             )
             if utils.POST_MORTEM:  # pragma: no cover
-                raise
-            content_link_strs = []
-        if content_link_strs is None:  # pragma: no cover
+                pdb.post_mortem()
+            link_strs = []
+        if link_strs is None:  # pragma: no cover
             # Plugin handled any linking itself
-            content_link_strs = []
-        if isinstance(content_link_strs, str):  # pragma: no cover
-            content_link_strs = [content_link_strs]
+            link_strs = []
+        if isinstance(link_strs, str):  # pragma: no cover
+            link_strs = [link_strs]
+        # Filter out duplicate paths but preserve order
+        uniq_link_strs = []
+        for enclosure_link_str in link_strs:
+            if enclosure_link_str not in uniq_link_strs:
+                uniq_link_strs.append(enclosure_link_str)
         return [
             self.archive.root_path
             / pathlib.Path(
-                utils.quote_path(content_link_str),
+                utils.quote_path(enclosure_link_str),
             )
-            for content_link_str in content_link_strs
+            for enclosure_link_str in uniq_link_strs
         ]
 
     def link_item_plugin_match(self, **kwargs):
         """
         If configured, check for a regular expression match for a feed item enclosure.
         """
-        link_path_plugin = kwargs["link_path_plugin"]
+        enclosure_plugin = kwargs["enclosure_plugin"]
         kwargs["self"] = self
         try:
-            match_string = eval(  # pylint: disable=eval-used
-                f"f{link_path_plugin.config['match-string']!r}",
+            match_string = eval(  # nosec B307, pylint: disable=eval-used
+                f"f{enclosure_plugin.config['match-string']!r}",
                 globals(),
                 kwargs,
             )
-        except Exception:  # pragma: no cover, pylint: disable=broad-except
+        except Exception:  # pylint: disable=broad-except
             logger.exception(
                 "Problem expanding `match-string` template for %r: %r",
-                type(link_path_plugin),
-                link_path_plugin.config["match-string"],
+                type(enclosure_plugin),
+                enclosure_plugin.config["match-string"],
             )
             if utils.POST_MORTEM:  # pragma: no cover
-                raise
+                pdb.post_mortem()
             return None
         try:
-            match = link_path_plugin.config["match-re"].match(match_string)
+            match = enclosure_plugin.config["match-re"].match(match_string)
         except Exception:  # pragma: no cover, pylint: disable=broad-except
             logger.exception(
                 "Problem matching `match-pattern` for %r: %r",
-                type(link_path_plugin),
-                link_path_plugin.config["match-string"],
+                type(enclosure_plugin),
+                enclosure_plugin.config["match-string"],
             )
             if utils.POST_MORTEM:  # pragma: no cover
-                raise
+                pdb.post_mortem()
             return None
-        if match is None:  # pragma: no cover
-            logger.info(
+        if match is None:
+            logger.debug(
                 "The %r plugin `match-pattern` did not match: %r",
-                type(link_path_plugin),
+                type(enclosure_plugin),
                 match_string,
             )
             return None
         return match
 
     def link_plugin_file(
         self,
         url_result,
-        content_archive_relative,
-        content_link_path,
+        enclosure_archive_relative,
+        link_path,
         link_idx,
     ):
         """
-        Link an item content/enclosure to a filesystem path returned by a plugin.
+        Link an item enclosure to a filesystem path returned by a plugin.
         """
         # Make the link relative
-        content_link_target = pathlib.Path(
+        enclosure_link_target = pathlib.Path(
             os.path.relpath(
-                self.archive.root_path / content_archive_relative,
-                content_link_path.parent,
+                self.archive.root_path / enclosure_archive_relative,
+                link_path.parent,
             ),
         )
 
-        # Append numerical index if there are multiple content downloads for this
+        # Append numerical index if there are multiple enclosure downloads for this
         # item.
-        content_link_stem = content_link_path.stem
-        content_index = 0
-        while os.path.lexists(content_link_path):
-            if (
-                content_link_path.is_symlink()
-                and content_link_path.readlink() == content_link_target
+        enclosure_link_stem = link_path.stem
+        enclosure_index = 0
+        while os.path.lexists(link_path):
+            if link_path.is_symlink() and os.readlink(link_path) == str(
+                enclosure_link_target
             ):
                 logger.debug(
-                    "Duplicate item URL, skip content link: %r -> %r",
-                    str(content_link_path),
-                    str(content_link_target),
+                    "Duplicate item URL, skip enclosure link: %r -> %r",
+                    str(link_path),
+                    str(enclosure_link_target),
                 )
                 break
-            content_index += 1
-            content_link_path = content_link_path.with_stem(
-                content_link_stem[
+            enclosure_index += 1
+            link_path = link_path.with_name(
+                enclosure_link_stem[
                     : self.archive.root_stat.f_namemax
-                    - (len(content_link_path.suffix) + len(str(content_index)))
+                    - (len(link_path.suffix) + len(str(enclosure_index)))
                 ]
-                + str(content_index),
+                + str(enclosure_index)
+                + link_path.suffix,
             )
         else:
             logger.info(
-                "Linking item content: %r -> %r",
-                str(content_link_path),
-                str(content_link_target),
+                "Linking item enclosure: %r -> %r",
+                str(link_path),
+                str(enclosure_link_target),
             )
-            content_link_path.parent.mkdir(parents=True, exist_ok=True)
-            content_link_path.symlink_to(content_link_target)
+            link_path.parent.mkdir(parents=True, exist_ok=True)
+            link_path.symlink_to(enclosure_link_target)
 
         url_result.getparent().attrib[
-            f"{{{self.NAMESPACE}}}content-link-{link_idx}"
-        ] = str(content_link_path)
-        return content_link_path
+            f"{{{self.NAMESPACE}}}enclosure-link-{link_idx}"
+        ] = str(link_path)
+        return link_path
 
 
 def update_download_metadata(download_response, download_path):
     """
     Reflect any metdata that can be extracted from the respons in the download file.
     """
     # Set the filesystem modification datetime if the header is provided
```

### Comparing `feed-archiver-1.0.0/src/feedarchiver/formats.py` & `feed-archiver-1.0.0b11/src/feedarchiver/formats.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Handle different feed XML formats.
 """
 
 import typing
 import logging
 
-from lxml import etree
+from lxml import etree  # nosec: B410
 
 logger = logging.getLogger(__name__)
 
 
 def query_xpath(elem, xpath):
     """
     Return the XPath match raising or logging errors if not one.
@@ -41,28 +41,29 @@
 
     # Constants that define the structural specifics that differ between the formats,
     # mostly tag and attribute names.
     ROOT_TAG = ""
     ITEM_TAG = ""
     ITEM_ID_TAG = ""
     DOWNLOAD_TEXT_TAGS = ["link", "url"]
-    DOWNLOAD_CONTENT_TAGS = ["enclosure", "content"]
-    DOWNLOAD_CONTENT_EXPR = "@rel='enclosure'"
+    DOWNLOAD_ENCLOSURE_TAGS = ["enclosure", "content"]
+    DOWNLOAD_ENCLOSURE_EXPR = "@rel='enclosure'"
     DOWNLOAD_ATTR_NAMES = ["href", "url", "src"]
 
     # XPaths that differ between formats but can't be generalized from the above
     ITEMS_PARENT_XPATH = ""
     SELF_LINK_XPATH = "./*[local-name() = 'link' and @rel = 'self']"
 
     # Map format-specific sub-classes to their corresponding root tag name.
     # Used to match a parsed feed XML tree to the corresponding format.
     FEED_FORMATS: typing.Dict[typing.Type, typing.Type] = {}
 
-    def __init_subclass__(cls, /, **kwargs):
-        """Assemble the XPath components from the format constants.
+    def __init_subclass__(cls, **kwargs):
+        """
+        Assemble the XPath components from the format constants.
 
         Done here so that the resulting XPaths are import-time constants that can be
         overridden by power users, either in their own subclasses or in some future
         configuration option.  The assembled paths can also be printed in logs or CLI
         help so that such power users can use them as a basis for modification.
         """
         super().__init_subclass__(**kwargs)
@@ -75,27 +76,27 @@
         download_feed_prefix = (
             f"{cls.ITEMS_PARENT_XPATH}/*[not(local-name() = '{cls.ITEM_TAG}')"
         )
         cls.DOWNLOAD_FEED_URLS_XPATHS = [
             f"{download_feed_prefix} and {download_text_expr}]/text()",
             f"{download_feed_prefix}]//{download_attr_step}",
         ]
-        download_content_tags_expr = " or ".join(
-            f"local-name()='{download_content_tag}'"
-            for download_content_tag in cls.DOWNLOAD_CONTENT_TAGS
+        download_enclosure_tags_expr = " or ".join(
+            f"local-name()='{download_enclosure_tag}'"
+            for download_enclosure_tag in cls.DOWNLOAD_ENCLOSURE_TAGS
         )
-        download_content_expr = (
-            f"{download_content_tags_expr} or {cls.DOWNLOAD_CONTENT_EXPR}"
+        download_enclosure_expr = (
+            f"{download_enclosure_tags_expr} or {cls.DOWNLOAD_ENCLOSURE_EXPR}"
         )
         cls.DOWNLOAD_ITEM_ASSET_URLS_XPATHS = [
             f".//*[{download_text_expr}]/text()",
-            f".//*[not({download_content_expr})]/{download_attr_step}",
+            f".//*[not({download_enclosure_expr})]/{download_attr_step}",
         ]
-        cls.DOWNLOAD_ITEM_CONTENT_URLS_XPATHS = [
-            f".//*[{download_content_expr}]/{download_attr_step}",
+        cls.DOWNLOAD_ITEM_ENCLOSURE_URLS_XPATHS = [
+            f".//*[{download_enclosure_expr}]/{download_attr_step}",
         ]
 
         # Register this specific feed format by it's root element tag name
         cls.FEED_FORMATS[cls.ROOT_TAG] = cls
 
         logger.debug(
             "%s XPaths:\n%s",
```

### Comparing `feed-archiver-1.0.0/src/feedarchiver/linkpaths/servarr.py` & `feed-archiver-1.0.0b11/src/feedarchiver/enclosures/servarr.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,23 +4,29 @@
 
 import functools
 import pathlib
 import re
 import socket
 import logging
 
+try:
+    from functools import cached_property  # type: ignore
+except ImportError:  # pragma: no cover
+    # BBB: Python <3.8 compatibility
+    from backports.cached_property import cached_property  # type: ignore
+
 import arrapi
 import tenacity
 
-from .. import linkpaths
+from .. import enclosures
 
 logger = logging.getLogger(__name__)
 
 
-class SonarrLinkPathPlugin(linkpaths.LinkPathPlugin):
+class SonarrEnclosurePlugin(enclosures.EnclosurePlugin):  # noqa: V102
     """
     Link enclosures about a TV series episode next to the video file as external audio.
     """
 
     MULTI_EPISODE_RE = re.compile("[Ee& -]")
 
     url = "http://localhost:8989"
@@ -51,37 +57,37 @@
             raise ValueError("Sonarr plugin configuration must specify `api-key`")
         api_key = self.config["api-key"]
         if not isinstance(api_key, str):  # pragma: no cover
             raise ValueError(f"Sonarr `api_key` must be a string: {api_key!r}")
         self.client = arrapi.SonarrAPI(self.url, api_key)
         self.client_get = self.client._raw._get  # pylint: disable=protected-access
 
-    @functools.cached_property
+    @cached_property
     def series_by_title(self):
         """
         Request, collate and cache the full list of series titles to share across calls.
         """
         return {series["title"]: series["id"] for series in self.client_get("series")}
 
     # NOTE: These functions will cache globally, for the life of the process.  This
     # should be fine as `$ feedarchiver update` is expected to be run periodically, such
     # as by `# cron`.
-    @functools.cache  # pylint: disable=method-cache-max-size-none
+    @functools.lru_cache(maxsize=None)  # pylint: disable=method-cache-max-size-none
     def get_episode_files_seasons(self, series_id):
         """
         Request, correlate and cache episode file DB ids to season and episode numbers.
         """
         episode_files_episodes = {}
         for episode in self.client_get("episode", seriesId=series_id):
             episode_files_episodes.setdefault(episode["episodeFileId"], []).append(
                 (episode["seasonNumber"], episode["episodeNumber"])
             )
         return episode_files_episodes
 
-    @functools.cache  # pylint: disable=method-cache-max-size-none
+    @functools.lru_cache(maxsize=None)  # pylint: disable=method-cache-max-size-none
     def get_episode_paths(self, series_id):
         """
         Request, collate and cache series episode file paths by season and episode.
         """
         episode_files_episodes = self.get_episode_files_seasons(series_id)
         episode_paths = {}
         for episode_file in self.client_get("episodeFile", seriesId=series_id):
@@ -89,17 +95,17 @@
                 episode_file["id"]
             ]:
                 episode_paths.setdefault(season_number, {})[
                     episode_number
                 ] = episode_file["path"]
         return episode_paths
 
-    def __call__(self, basename, match, *args, **kwargs):
+    def __call__(self, enclosure_path, match, *args, **kwargs):
         """
-        Lookup the episode and link the enclosure/content next to the video file.
+        Lookup the episode and link the enclosure next to the video file.
         """
         series_id, season_number, episode_numbers, stem_append = self.validate_params(
             match,
         )
 
         # Combine all the parameters to lookup the episode file
         episode_paths = self.get_episode_paths(series_id)
@@ -109,15 +115,15 @@
                 series_id,
                 season_number,
             )
         season_episode_paths = episode_paths.get(season_number, {})
 
         episodes_file_paths = []
         for episode_number in episode_numbers:
-            if episode_number in season_episode_paths:  # pragma: no cover
+            if episode_number in season_episode_paths:
                 # Assemble a path next to the episode file
                 episode_path = pathlib.Path(season_episode_paths[episode_number])
             else:
                 if season_episode_paths:  # pragma: no cover
                     logger.error(
                         "Sonarr `episode_number` not in series %s episodes: S%sE%02d",
                         series_id,
@@ -128,22 +134,23 @@
                 series = self.client_get(f"series/{series_id}")
                 episode_path = pathlib.Path(
                     series["path"],
                     f"Season {season_number:02d}",
                     f"{series['title']} S{season_number}E{episode_number:02d}.mkv",
                 )
             episodes_file_paths.append(
-                episode_path.with_stem(f"{episode_path.stem}{stem_append}").with_suffix(
-                    pathlib.Path(basename).suffix,
+                episode_path.with_name(
+                    f"{episode_path.stem}{stem_append}" + enclosure_path.suffix,
                 ),
             )
 
         return [str(episode_file_path) for episode_file_path in episodes_file_paths]
 
-    def validate_params(self, match):
+    # TODO: Refactor to reduce complexity and improve readability and testibility
+    def validate_params(self, match):  # noqa: MC0001
         """
         Combine plugin config and regex match groups, extract and validate parameters.
         """
         # Get API lookup parameters from the config and override with regex match groups
         params = dict(self.config, **match.groupdict())
 
         # Do any parameter validation that's possible without making API requests
```

### Comparing `feed-archiver-1.0.0/src/feedarchiver/linkpaths/template.py` & `feed-archiver-1.0.0b11/src/feedarchiver/enclosures/template.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 """
-The default link path plugin, expands a template into the target path.
+The default enclosure plugin, expands a template into the target path.
 """
 
 import pathlib
 
 from .. import utils  # noqa, pylint: disable=unused-import
-from .. import linkpaths
+from .. import enclosures
 
 
-class TemplateLinkPathPlugin(linkpaths.LinkPathPlugin):
+class TemplateEnclosurePlugin(enclosures.EnclosurePlugin):  # noqa: V102
     """
-    The default link path plugin, expands a template into the target path.
+    The default enclosure plugin, expands a template into the target path.
     """
 
     # Default a hierarchy under the feed title and item title
     template = str(
         pathlib.Path(
             "Feeds",
-            "{feed_elem.find('title').text.strip()}",
-            "{item_elem.find('title').text.strip()}",
-            "{basename}",
+            "{utils.quote_sep(feed_parsed.feed.title).strip()}",
+            "{utils.quote_sep(item_parsed.title).strip()}{enclosure_path.suffix}",
         )
     )
 
     def load_config(self):
         """
         Pre-process and validate the plugin config prior to linking each enclosure.
         """
@@ -31,26 +30,27 @@
         if not isinstance(self.template, str):  # pragma: no cover
             raise ValueError(
                 f"Format `template` for plugin must be a string: {self.template!r}"
             )
 
     def __call__(
         self,
-        archive_feed,
-        feed_elem,
-        item_elem,
-        url_result,
-        basename,
         *args,
         **kwargs,
     ):  # pylint: disable=too-many-arguments
         """
-        Link the feed item enclosure/content to a target path expanded from a template.
+        Link the feed item enclosure to a target path expanded from a template.
         """
         # Maybe find a better template format/engine, perhaps Jinja2?
         # We need a templating engine that supports a very rich set of operations
         # sufficient, for example, to extract data from `ElementTree` objects.  This
         # means we need to support execution of arbitrary code.  This shouldn't be a
         # problem since anyone that can run `$ feedarchiver` can also run `$ python`.
         # But still, this has a bad code smell.
         # https://python-forum.io/thread-24481.html
-        return [eval(f"f{self.template!r}")]  # pylint: disable=eval-used
+        return [
+            eval(  # nosec: B307, pylint: disable=eval-used
+                f"f{self.template!r}",
+                globals(),
+                dict(locals(), **kwargs),
+            )
+        ]
```

### Comparing `feed-archiver-1.0.0/src/feedarchiver/tests/__init__.py` & `feed-archiver-1.0.0b11/src/feedarchiver/tests/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,31 +6,32 @@
 import datetime
 import pathlib
 import tempfile
 import shutil
 import email.utils
 import unittest
 
-from lxml import etree
+from lxml import etree  # nosec: B410
 
+import respx
 import requests_mock
 
 from .. import utils
 from .. import archive
 from ..utils import mimetypes
 
 
 class FeedarchiverTestCase(
     unittest.TestCase,
-):  # pylint: disable=too-many-instance-attributes
+):
     """
     Constants and set-up used in all feed-archiver tests.
     """
 
-    maxDiff = None
+    maxDiff = None  # noqa: F841
 
     # A date and time in the past all but guaranteed not to exist naturally in the
     # checkout.
     OLD_DATETIME = datetime.datetime(year=1980, month=11, day=25, hour=8, minute=31)
     # The relative path to the example/sample test data this test will use.
     # Default examples are copied from the Wikipedia page of each RSS/Atom syndication
     # XML format to represent the cleanest, simplest form of feeds.
@@ -60,44 +61,45 @@
     def setUp(self):
         """
         Set up used in all feed-archiver tests.
         """
         super().setUp()
 
         # Mock HTTP/S requests:
+        # https://lundberg.github.io/respx/guide/#mock-httpx
+        # TODO: Switch to `assert_all_called=True`
+        self.client_mock = respx.MockRouter(assert_all_called=False)
+        self.addCleanup(self.client_mock.stop)
+        self.client_mock.start()
+        # Mock requests made by external libraries, e.g. API client:
         # https://requests-mock.readthedocs.io/en/latest/fixture.html#fixtures
-        self.requests_mock = requests_mock.Mocker()
-        self.addCleanup(self.requests_mock.stop)
-        self.requests_mock.start()
+        self.request_mocker = requests_mock.Mocker()
+        self.addCleanup(self.request_mocker.stop)
+        self.request_mocker.start()
 
         # Create a temporary directory for mutable test data
-        self.tmp_dir = (
-            tempfile.TemporaryDirectory(  # pylint: disable=consider-using-with
-                suffix=self.EXAMPLE_RELATIVE.suffix,
-                prefix=f"{self.EXAMPLE_RELATIVE.stem}-",
-            )
+        tmp_dir = tempfile.TemporaryDirectory(  # pylint: disable=consider-using-with
+            suffix=self.EXAMPLE_RELATIVE.suffix,
+            prefix=f"{self.EXAMPLE_RELATIVE.stem}-",
         )
-        self.addCleanup(self.tmp_dir.cleanup)
+        self.addCleanup(tmp_dir.cleanup)
 
         # Use the example/sample test data basename to assemble the rest of the
         # filesystem paths used by the tests.
-        self.remotes_path = self.REMOTES_PATH / self.EXAMPLE_RELATIVE
         self.archive_path = self.ARCHIVES_PATH / self.EXAMPLE_RELATIVE
 
         # Copy the testing example feeds archive
-        shutil.copytree(
-            src=self.archive_path,
-            dst=self.tmp_dir.name,
-            dirs_exist_ok=True,
-        )
-        self.archive = archive.Archive(self.tmp_dir.name)
+        if pathlib.Path(tmp_dir.name).exists():  # pragma: no cover
+            shutil.rmtree(tmp_dir.name)
+        shutil.copytree(src=self.archive_path, dst=tmp_dir.name)
+        self.archive = archive.Archive(tmp_dir.name)
         # Mock the Sonarr request that is sent when the config is loaded
-        self.requests_mock.get(
+        self.request_mocker.get(
             f"{self.SONARR_URL}/api/v3/system/status?apikey=secret",
-            json=dict(version="3.0.6.1342"),
+            json={"version": "3.0.6.1342"},
         )
         self.archive.load_config()
         self.archive_feed = self.archive.archive_feeds[0]
         self.feed_url = self.archive_feed.url
         self.feed_path = self.archive.root_path / self.FEED_ARCHIVE_RELATIVE
 
     def mock_remote(self, archive_feed, remote_mock=None):
@@ -124,23 +126,31 @@
             }
             mock_type, _ = mimetypes.guess_type(mock_path.name)
             if mock_type:
                 mock_headers["Content-Type"] = mock_type
             mock_url = archive_feed.archive.path_to_url(
                 archive_feed.archive.root_path / mock_path.relative_to(remote_mock_path)
             )
-            request_mocks[mock_url] = (
-                mock_path,
-                self.requests_mock.get(
+            if mock_url.startswith(self.SONARR_URL):
+                # Mock Servarr requests using the same library as API client
+                mock_response = self.request_mocker.get(
                     mock_url,
                     # Ensure the download response includes `Last-Modified`
                     headers=mock_headers,
                     content=mock_bytes,
-                ),
-            )
+                )
+            else:
+                mock_response = self.client_mock.get(
+                    mock_url,
+                ).respond(
+                    # Ensure the download response includes `Last-Modified`
+                    headers=mock_headers,
+                    content=mock_bytes,
+                )
+            request_mocks[mock_url] = (mock_path, mock_response)
         return request_mocks
 
     def update_feed(self, archive_feed, remote_mock=None):
         """
         Mock the request responses with the mock dir and update the archive.
         """
         request_mocks = self.mock_remote(archive_feed, remote_mock)
@@ -212,15 +222,15 @@
 
 
 def get_feed_items(feed_path):
     """
     Map item ID to item element for all the items in the given feed XML.
     """
     with feed_path.open() as feed_opened:
-        tree = etree.parse(feed_opened)
+        tree = etree.parse(feed_opened, parser=utils.XML_PARSER)  # nosec: B320
     channel = tree.getroot().find("channel")
     return {
         item_elem.find("guid").text: item_elem for item_elem in channel.iter("item")
     }
 
 
 def walk_archive(archive_root_path):
```

### Comparing `feed-archiver-1.0.0/src/feedarchiver/tests/archives/downloads/.feed-archiver.yml` & `feed-archiver-1.0.0b11/src/feedarchiver/tests/archives/end-to-end/.feed-archiver.yml.in`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 defaults:
   base-url: "https://feeds.example.com"
   plugins:
-    link-paths:
+    enclosures:
       sonarr:
-        url: "http://localhost:8989"
-        api-key: "secret"
-  link-paths:
-    - template:
-        "./Music/Podcasts/{feed_elem.find('title').text.strip()}/{item_elem.find('title').text.strip()}/{basename}"
+        url: "http://sonarr:8989"
+        api-key: "${SONARR_API_KEY}"
+  enclosures:
+    - template: "\
+      ./Music/Podcasts/{utils.quote_sep(feed_parsed.feed.title).strip()}\
+      /{utils.quote_sep(item_parsed.title).strip()}{enclosure_path.suffix}"
 feeds:
-  - remote-url:
-      "https://foo.example.com/podcast/feed.rss"
-    link-paths:
+  # A Creative Commons licensed feed
+  - remote-url: "https://www.democracynow.org/podcast.xml"
+    enclosures:
       # This particular feed is a podcast about a TV series/show.  Link enclosures
       # from feed items about an individual episode next to the episode video file as
       # an alternate audio track using a non-default plugin.
       - plugin: "sonarr"
-        match-string: "{item_elem.find('title').text.strip()}"
-        match-pattern: "(?P<item_title>.+) \\((?P<series_title>.+?) (?P<season_number>[0-9])(?P<episode_numbers>[0-9]+[0-9Ee& -]*)\\)"
+        match-string: "{utils.quote_sep(item_parsed.title).strip()}"
+        match-pattern: "\
+        (?P<item_title>.+) \\((?P<series_title>.+) \
+        (?P<season_number>[0-9])(?P<episode_numbers>[0-9]+)\\)"
         stem-append: "-garply"
```

### Comparing `feed-archiver-1.0.0/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/media/common-id.mp3` & `feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/media/common-id.mp3`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/media/el-ni%25C3%25B1o.mp3` & `feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/media/el-ni%25C3%25B1o.mp3`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/common-id.mp3` & `feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/common-id.mp3`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/download` & `feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/bah-episode-title/download.mp3`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/el-ni%25C3%25B1o.png` & `feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/el-ni%25C3%25B1o.png`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/index.html` & `feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/bah-episode-title/index.html`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/fred-episode-title/download` & `feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/download`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/feed.rss` & `feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/feed.rss`

 * *Files 20% similar despite different names*

#### Comparing `feed-archiver-1.0.0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/feed.rss` & `feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/feed.rss`

```diff
@@ -26,14 +26,29 @@
     </itunes:owner>
     <itunes:subtitle>The Foo Podcast subtitle.</itunes:subtitle>
     <itunes:summary><![CDATA[<p class="podcast-description">A description of the <b>whole</b> podcast
 	       feed, regardless of individual episodes.</p>]]></itunes:summary>
     <media:category scheme="http://www.itunes.com/dtds/podcast-1.0.dtd">Qux &amp; Quux/Corge</media:category>
     <!-- Generated by Garply Feed Generator -->
     <item>
+      <guid isPermaLink="false">foo_6be48e7e-e3b8-4f82-bac3-88af73404407</guid>
+      <title>Bah Episode Title (Qux Series Title 108 &amp; 09)</title>
+      <pubDate>Tue, 30 Nov 2021 13:53:22 -0000</pubDate>
+      <link>https://https://foo.example.com/podcast/episodes/bah-episode-title/</link>
+      <description>A description of this specific episode, Bah.</description>
+      <enclosure url="https://foo.example.com/podcast/episodes/bah-episode-title/download.mp3" type="audio/mpeg" length="52079"/>
+      <itunes:episodeType>full</itunes:episodeType>
+      <itunes:duration>00:00:04.24</itunes:duration>
+      <author>plugh@foo.example.com (Plugh Xyzzy)</author>
+      <itunes:author>Plugh Xyzzy</itunes:author>
+      <itunes:summary>A description of this specific episode, Bah.</itunes:summary>
+      <media:content fileSize="52079" type="audio/mpeg" url="https://foo.example.com/podcast/episodes/bah-episode-title/download.mp3"/>
+      <content:encoded>A description of this specific episode, Bah.</content:encoded>
+    </item>
+    <item>
       <guid isPermaLink="false">foo_376d9037-bf85-4e05-913c-be5e7724c4a6</guid>
       <title>El Niño Episode Title (Qux Series Title 106 &amp; 07)</title>
       <pubDate>Tue, 23 Nov 2021 13:53:22 -0000</pubDate>
       <link>https://https://foo.example.com/podcast/episodes/el-ni%C3%B1o-episode-title/</link>
       <description><![CDATA[<p class="episode-description">A description of <b>this specific</b>
 		 episode, El Niño.</p>]]></description>
       <enclosure url="https://foo.example.com/podcast/episodes/el-ni%C3%B1o-episode-title/download" type="audio/mpeg" length="52079"/>
@@ -52,9 +67,18 @@
       <content:encoded><![CDATA[<p class="episode-description">A description of <b>this specific</b>
 		 episode, El Niño.</p>]]></content:encoded>
     </item>
     <item>
       <guid isPermaLink="false">foo_9a8e04a4-9e94-462f-919a-f0419dd6318c</guid>
       <enclosure url="https://foo.example.com/podcast/episodes/fred-episode-title/download" type="application/x-no-extension" length="52079"/>
     </item>
+    <item>
+      <guid isPermaLink="false">foo_f58d2179-d398-4a86-bd60-5b2881aed686</guid>
+      <title>Garply Bonus Episode</title>
+      <enclosure url="https://foo.example.com/podcast/episodes/garply-bonus-episode/download.mp3" type="audio/mpeg" length="52079"/>
+    </item>
+    <item>
+      <guid isPermaLink="false">foo_0bad50c5-83df-47ce-b616-f2b21252ec62</guid>
+      <enclosure url="https://foo.example.com/podcast/episodes/nonexistent-episode/download.mp3" type="audio/mpeg" length="52079"/>
+    </item>
   </channel>
 </rss>
```

### Comparing `feed-archiver-1.0.0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/image.png` & `feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/image.png`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/index.html` & `feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/index.html`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/1` & `feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/index.html`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/2` & `feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/1`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/3` & `feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/2`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/main.html` & `feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/main.html`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/added-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss` & `feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/added-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/added-item/https/waldo.example.com/feeds/waldo` & `feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/added-item/https/waldo.example.com/feeds/waldo`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/1` & `feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/3`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/2` & `feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/1`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/3` & `feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/2`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/main.html` & `feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/main.html`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/empty/https/waldo.example.com/feeds/waldo` & `feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/empty/https/waldo.example.com/feeds/waldo`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/1` & `feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/3`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/2` & `feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/1`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/3` & `feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/2`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/main.html` & `feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/main.html`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/orig/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss` & `feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/orig/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/orig/https/waldo.example.com/feeds/waldo` & `feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/orig/https/waldo.example.com/feeds/waldo`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/1` & `feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/3`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/2` & `feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/1`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/3` & `feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/2`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/main.html` & `feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/main.html`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/removed-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss` & `feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/removed-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/removed-item/https/waldo.example.com/feeds/waldo` & `feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/removed-item/https/waldo.example.com/feeds/waldo`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/1` & `feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/3`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/2` & `feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/1`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/3` & `feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/2`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/main.html` & `feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/main.html`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/reordered-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss` & `feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/reordered-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0/src/feedarchiver/tests/remotes/simple/reordered-item/https/waldo.example.com/feeds/waldo` & `feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/reordered-item/https/waldo.example.com/feeds/waldo`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0/src/feedarchiver/tests/test_archive.py` & `feed-archiver-1.0.0b11/src/feedarchiver/tests/test_archive.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """
 Test the feed-archiver representation of an archive of syndication feeeds.
 """
 
 import typing
-
+import unittest
 from unittest import mock
 
+from .. import archive
 from .. import tests
 
 
 class FeedarchiverArchiveTests(tests.FeedarchiverTestCase):
     """
     Test the feed-archiver representation of an archive of syndication feeeds.
     """
@@ -22,14 +23,16 @@
         """
         Each feed in the archive configuration is updated.
         """
         mock_update_method = mock_feed_class.return_value.update
         mock_update_method.return_value = self.UPDATE_RETURN_VALUE
 
         self.archive.load_config()
+        mock_feed_class.return_value.config = mock_feed_class.mock_calls[0][2]["config"]
+        mock_feed_class.return_value.path = self.feed_path
         mock_feed_class.assert_any_call(
             archive=self.archive,
             config={"remote-url": self.feed_url},
         )
         self.assertEqual(
             mock_feed_class.call_count,
             2,
@@ -57,16 +60,41 @@
 
     @mock.patch("feedarchiver.feed.ArchiveFeed")
     def test_feeds_no_updated_items(self, mock_feed_class):
         """
         Archive handles updates without any updated feed items.
         """
         mock_update_method = mock_feed_class.return_value.update
-        mock_update_method.return_value = ([], {})
+        mock_update_method.return_value = None
+        self.archive.load_config()
+        mock_feed_class.return_value.config = mock_feed_class.mock_calls[0][2]["config"]
 
         updated_feeds = self.archive.update()
 
         self.assertEqual(
             updated_feeds,
-            {},
+            None,
             "Archive updated feed items not empty",
         )
+
+
+class FeedarchiverInvalidArchiveTests(unittest.TestCase):
+    """
+    Test archives with invalid configuration.
+    """
+
+    def test_archive_wo_config(self):
+        """
+        An archive with no configuration raises a helpful error.
+        """
+        with self.assertRaises(ValueError, msg="Wrong empty config error"):
+            archive.Archive(tests.FeedarchiverTestCase.ARCHIVES_PATH / "empty")
+
+    def test_archive_wo_feeds(self):
+        """
+        An archive with no feeds configured raises a helpful error.
+        """
+        feed_archive = archive.Archive(
+            tests.FeedarchiverTestCase.ARCHIVES_PATH / "empty-feeds",
+        )
+        with self.assertRaises(ValueError, msg="Wrong empty feeds error"):
+            feed_archive.load_config()
```

### Comparing `feed-archiver-1.0.0/src/feedarchiver/tests/test_cli.py` & `feed-archiver-1.0.0b11/src/feedarchiver/tests/test_cli.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """
 Test the feed-archiver Command-Line Interface.
 """
 
 import sys
 import os
 import io
-import subprocess
+import runpy
+import subprocess  # nosec B404
 import contextlib
 import pathlib
 
 
 import feedarchiver
 
 from .. import tests
@@ -20,15 +21,15 @@
     Test the feed-archiver Command-Line Interface.
     """
 
     def test_importable(self):
         """
         The Python package is on `sys.path` and thus importable.
         """
-        import_process = subprocess.run(
+        import_process = subprocess.run(  # nosec B603
             [sys.executable, "-c", "import feedarchiver"],
             check=False,
         )
         self.assertEqual(
             import_process.returncode,
             0,
             "The Python package not importable",
@@ -60,15 +61,15 @@
         )
 
     def test_cli_subcommand(self):
         """
         The command line supports sub-commands.
         """
         cwd = pathlib.Path.cwd()
-        os.chdir(self.tmp_dir.name)
+        os.chdir(self.archive.root_path)
         try:
             self.assertIsNone(
                 feedarchiver.main(args=["update"]),
                 "Wrong console script sub-command return value",
             )
         finally:
             os.chdir(cwd)
@@ -80,43 +81,55 @@
         stderr = self.get_cli_error_messages(args=["update", "--non-existent-option"])
         self.assertIn(
             "error: unrecognized arguments: --non-existent-option",
             stderr,
             "Wrong invalid option message",
         )
 
-    def test_cli_module_main(self):
+    def test_cli_dash_m_option(self):
         """
-        The package/module supports execution via Python's `-m` option.
+        The package supports execution via Python's `-m` CLI option.
         """
-        module_main_process = subprocess.run(
+        module_main_process = subprocess.run(  # nosec B603
             [sys.executable, "-m", "feedarchiver", "update"],
             check=False,
-            cwd=self.tmp_dir.name,
+            cwd=self.archive.root_path,
         )
         self.assertEqual(
             module_main_process.returncode,
             0,
             "Running via Python's `-m` option exited with non-zero status code",
         )
 
+    def test_cli_module_main(self):
+        """
+        The package supports execution via Python's `-m` option.
+        """
+        with self.assertRaises(SystemExit, msg="CLI didn't exit") as exc_context:
+            runpy.run_module("feedarchiver")
+        self.assertEqual(
+            exc_context.exception.code,
+            2,
+            "Wrong `runpy` exit status code",
+        )
+
     def test_cli_exit_code(self):
         """
         The command line script exits with status code zero if there are no exceptions.
         """
         # Find the location of the `console_scripts` for this test environment
         prefix_path = pathlib.Path(sys.argv[0]).parent
         while not (prefix_path / "bin").is_dir():
             prefix_path = prefix_path.parent
-            if prefix_path.parent is prefix_path.parents[-1]:  # pragma: no cover
+            if prefix_path.parent is list(prefix_path.parents)[-1]:  # pragma: no cover
                 raise ValueError(f"Could not find script prefix path: {sys.argv[0]}")
 
-        script_process = subprocess.run(
-            [(prefix_path / "bin" / "feed-archiver").resolve(), "update"],
+        script_process = subprocess.run(  # nosec B603
+            [prefix_path / "bin" / "feed-archiver", "update"],
             check=False,
-            cwd=self.tmp_dir.name,
+            cwd=self.archive.root_path,
         )
         self.assertEqual(
             script_process.returncode,
             0,
             "Running the console script exited with non-zero status code",
         )
```

### Comparing `feed-archiver-1.0.0/src/feedarchiver/tests/test_download.py` & `feed-archiver-1.0.0b11/src/feedarchiver/tests/test_download.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,33 +3,34 @@
 """
 
 import os
 import datetime
 import pathlib
 import urllib
 
-from lxml import etree
-import requests_mock
+from lxml import etree  # nosec: B410
+import respx.models
 
+from .. import utils
 from .. import tests
 
 
 class FeedarchiverDownloadTests(tests.FeedarchiverDownloadsTestCase):
     """
     Test the feed-archiver downloading of enclosures, assets, etc..
     """
 
     def test_real_requests_disabled(self):
         """
         Confirm that tests will fail if real/external requests are attempted.
         """
         # Put the mocks in place
         self.update_feed(self.archive_feed)
-        with self.assertRaises(requests_mock.exceptions.NoMockAddress):
-            self.archive.requests.get("http://example.com")
+        with self.assertRaises(respx.models.AllMockedAssertionError):
+            self.archive.client.get("http://example.com")
 
     def test_download_file_metadata(self):
         """
         Download file metadata in the archive reflects remote response headers.
 
         All metadata that can be extracted from the remote response is reflected in the
         file metadata in the archive.
@@ -45,35 +46,29 @@
         os.utime(
             self.ENCLOSURE_MOCK_PATH,
             (enclosure_mock_stat.st_atime, self.OLD_DATETIME.timestamp()),
         )
 
         # Download the enclosure into the archive
         orig_request_mocks = self.mock_remote(self.archive_feed)
-        redirect_request_mock = self.requests_mock.get(
+        redirect_request_mock = self.client_mock.get(
             self.ENCLOSURE_URL,
+        ).respond(
             status_code=302,
-            reason="Found",
             headers={"Location": self.ENCLOSURE_REDIRECT_URL},
         )
         self.archive_feed.update()
         # The archive file's modification time matches.
         self.assertEqual(
             datetime.datetime.fromtimestamp(enclosure_archive_path.stat().st_mtime),
             self.OLD_DATETIME,
             "Archive download modification date doesn't match `Last-Modified` header",
         )
 
         # The most appropriate file basename is symlinked to the download file
-        _, download_request_mock = orig_request_mocks[self.ENCLOSURE_URL]
-        self.assertEqual(
-            download_request_mock.call_count,
-            0,
-            "Mock request without redirect response called",
-        )
         self.assertEqual(
             redirect_request_mock.call_count,
             1,
             "Wrong number of redirect requests",
         )
         _, target_request_mock = orig_request_mocks[self.ENCLOSURE_REDIRECT_URL]
         self.assertEqual(
@@ -81,18 +76,20 @@
             1,
             "Wrong number of redirect redirect target mock request calls",
         )
 
         # Test in the absence of the response headers
         self.archive_feed.path.unlink()
         enclosure_archive_path.unlink()
-        no_header_request_mock = self.requests_mock.get(
+        no_header_request_mock = self.client_mock.get(
             self.ENCLOSURE_URL,
+        ).respond(
             content=self.ENCLOSURE_MOCK_PATH.read_bytes(),
         )
+        no_header_request_mock.reset()
         self.assert_no_header_download_mtime(
             no_header_request_mock,
             self.archive.root_path / self.ENCLOSURE_RELATIVE.with_suffix(".mp3"),
         )
 
     def test_downloads(self):  # pylint: disable=too-many-locals
         """
@@ -167,15 +164,18 @@
             uncalled_request_mocks,
             {},
             # Some request mocks didn't correspond to archive files
             "Archive download missing for request mocks",
         )
 
         # Assert archive URLs updated
-        archive_tree = etree.parse(self.archive_feed.path.open())
+        archive_tree = etree.parse(  # nosec: B320
+            self.archive_feed.path.open(),
+            parser=utils.XML_PARSER,
+        )
         feed_link_split = urllib.parse.urlsplit(
             archive_tree.find("channel").find("link").text,
         )
         feed_link_path = (
             pathlib.PurePosixPath(feed_link_split.path.lstrip("/")) / "index.html"
         )
         self.assertTrue(
@@ -199,48 +199,49 @@
         )
         feed_image_path = pathlib.PurePosixPath(feed_image_split.path.lstrip("/"))
         self.assertTrue(
             (self.archive.root_path / feed_image_path).is_file(),
             "Wrong feed image absolute URL in feed",
         )
         archive_items = archive_tree.find("channel").findall("item")
-        item_link_split = urllib.parse.urlsplit(archive_items[0].find("link").text)
+        archive_item = archive_items[1]
+        item_link_split = urllib.parse.urlsplit(archive_item.find("link").text)
         item_link_path = (
             pathlib.PurePosixPath(
                 urllib.parse.unquote(item_link_split.path).lstrip("/")
             )
             / "index.html"
         )
         self.assertTrue(
             (self.archive.root_path / item_link_path).is_file(),
             "Wrong item link index HTML absolute URL in feed",
         )
         item_enclosure_split = urllib.parse.urlsplit(
-            archive_items[0].find("enclosure").attrib["url"],
+            archive_item.find("enclosure").attrib["url"],
         )
         item_enclosure_path = pathlib.PurePosixPath(
             urllib.parse.unquote(item_enclosure_split.path).lstrip("/"),
         )
         self.assertTrue(
             (self.archive.root_path / item_enclosure_path).is_file(),
             "Wrong item enclosure absolute URL in feed",
         )
         item_media_content_split = urllib.parse.urlsplit(
-            archive_items[0].find("{*}content").attrib["url"],
+            archive_item.find("{*}content").attrib["url"],
         )
         item_media_content_path = pathlib.PurePosixPath(
             urllib.parse.unquote(item_media_content_split.path).lstrip("/"),
         )
         self.assertEqual(
             item_media_content_path,
             item_enclosure_path,
             "Wrong item media content absolute URL in feed",
         )
         item_image_split = urllib.parse.urlsplit(
-            archive_items[0].find("{*}image").attrib["href"],
+            archive_item.find("{*}image").attrib["href"],
         )
         item_image_path = pathlib.PurePosixPath(
             urllib.parse.unquote(item_image_split.path).lstrip("/"),
         )
         self.assertTrue(
             (self.archive.root_path / item_image_path).is_file(),
             "Wrong item image absolute URL in feed",
@@ -251,15 +252,14 @@
         for archive_path, archive_relative in tests.walk_archive(
             self.archive.root_path,
         ):
             with self.subTest(
                 msg="Test one feed download",
                 archive_relative=str(archive_relative),
             ):
-
                 # Assert that the request mock was called correctly
                 download_url, mock_path = self.archive_relative_to_remote_url(
                     archive_relative,
                     remote_mock_path,
                 )
                 self.assertIn(
                     download_url,
```

### Comparing `feed-archiver-1.0.0/src/feedarchiver/tests/test_feed.py` & `feed-archiver-1.0.0b11/src/feedarchiver/tests/test_feed.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,16 +2,17 @@
 Test updating the archive from the feed URLs.
 """
 
 import os
 import datetime
 import logging
 
-from lxml import etree
+from lxml import etree  # nosec: B410
 
+from .. import utils
 from .. import formats
 from .. import feed
 from .. import tests
 
 
 class FeedarchiverFeedTests(tests.FeedarchiverTestCase):
     """
@@ -20,37 +21,37 @@
 
     FEED_MOCK_RELATIVE = (
         tests.FeedarchiverTestCase.EXAMPLE_RELATIVE
         / tests.FeedarchiverTestCase.REMOTE_MOCK
         / tests.FeedarchiverTestCase.FEED_ARCHIVE_RELATIVE
     )
     FEED_FORMAT_PARAMS = [
-        dict(
-            feed_format_class=formats.RssFeedFormat,
-            relative_path=FEED_MOCK_RELATIVE,
-            items_parent_tag="channel",
-            item_tag="item",
-            item_id="7bd204c6-1655-4c27-aeee-53f933c5395f",
-        ),
-        dict(
-            feed_format_class=formats.AtomFeedFormat,
-            relative_path=(
+        {
+            "feed_format_class": formats.RssFeedFormat,
+            "relative_path": FEED_MOCK_RELATIVE,
+            "items_parent_tag": "channel",
+            "item_tag": "item",
+            "item_id": "7bd204c6-1655-4c27-aeee-53f933c5395f",
+        },
+        {
+            "feed_format_class": formats.AtomFeedFormat,
+            "relative_path": (
                 tests.FeedarchiverTestCase.EXAMPLE_RELATIVE
                 / tests.FeedarchiverTestCase.REMOTE_MOCK
                 / "https"
                 / "waldo.example.com"
                 / "feeds"
                 / "waldo"
             ),
-            items_parent_tag=(
+            "items_parent_tag": (
                 f"{{http://www.w3.org/2005/Atom}}{formats.AtomFeedFormat.ROOT_TAG}"
             ),
-            item_tag="entry",
-            item_id="urn:uuid:1225c695-cfb8-4ebb-aaaa-80da344efa6a",
-        ),
+            "item_tag": "entry",
+            "item_id": "urn:uuid:1225c695-cfb8-4ebb-aaaa-80da344efa6a",
+        },
     ]
 
     def test_feed_configs_requested(self):
         """
         Requests are sent for each feed URL in the archive configuration.
         """
         self.assertFalse(
@@ -64,22 +65,28 @@
             1,
             "Wrong number of original feed URL requests",
         )
         self.assertTrue(
             self.feed_path.is_file(),
             "Archive of feed XML does not exist after updating",
         )
-        with feed_path.open() as remote_opened:
-            remote_tree = etree.parse(remote_opened)
+        with feed_path.open(encoding="utf-8") as remote_opened:
+            remote_tree = etree.parse(  # nosec: B320
+                remote_opened,
+                parser=utils.XML_PARSER,
+            )
         remote_items = remote_tree.find("channel").iterchildren("item")
         remote_item_ids = [
             remote_item.find("guid").text for remote_item in remote_items
         ]
-        with self.feed_path.open() as archive_opened:
-            archive_tree = etree.parse(archive_opened)
+        with self.feed_path.open(encoding="utf-8") as archive_opened:
+            archive_tree = etree.parse(  # nosec: B320
+                archive_opened,
+                parser=utils.XML_PARSER,
+            )
         archive_items = archive_tree.find("channel").iterchildren("item")
         archive_item_ids = [
             archive_item.find("guid").text for archive_item in archive_items
         ]
         self.assertEqual(
             archive_item_ids,
             remote_item_ids,
@@ -103,22 +110,28 @@
         # Feed XML hasn't changed
         self.archive_feed.update()
         self.assertEqual(
             get_mock.call_count,
             2,
             "Wrong number of original feed URL requests",
         )
-        with feed_path.open() as remote_opened:
-            remote_tree = etree.parse(remote_opened)
+        with feed_path.open(encoding="utf-8") as remote_opened:
+            remote_tree = etree.parse(  # nosec: B320
+                remote_opened,
+                parser=utils.XML_PARSER,
+            )
         remote_items = remote_tree.find("channel").iterchildren("item")
         remote_item_ids = [
             remote_item.find("guid").text for remote_item in remote_items
         ]
-        with self.feed_path.open() as archive_opened:
-            archive_tree = etree.parse(archive_opened)
+        with self.feed_path.open(encoding="utf-8") as archive_opened:
+            archive_tree = etree.parse(  # nosec: B320
+                archive_opened,
+                parser=utils.XML_PARSER,
+            )
         archive_items = archive_tree.find("channel").iterchildren("item")
         archive_item_ids = [
             archive_item.find("guid").text for archive_item in archive_items
         ]
         self.assertEqual(
             archive_item_ids,
             remote_item_ids,
@@ -136,14 +149,15 @@
         self.assertEqual(
             len(orig_archive_item_elems),
             1,
             "Wrong number of original items in archived feed",
         )
 
         # Update the archive after the remote feed is updated with a new item added
+        get_mock.reset()
         added_item_request_mocks, _ = self.update_feed(
             archive_feed=self.archive_feed,
             remote_mock="added-item",
         )
         _, added_item_get_mock = added_item_request_mocks[self.feed_url]
 
         # Confirm that the correct request mocks have been used
@@ -174,14 +188,15 @@
         # than one item.
         added_item_request_mocks, _ = self.update_feed(
             archive_feed=self.archive_feed,
         )
         _, added_item_get_mock = added_item_request_mocks[self.feed_url]
 
         # Update the archive after the remote feed is updated with an item removed
+        added_item_get_mock.reset()
         removed_item_request_mocks, _ = self.update_feed(
             archive_feed=self.archive_feed,
             remote_mock="removed-item",
         )
         _, removed_item_get_mock = removed_item_request_mocks[self.feed_url]
 
         # Confirm that the correct request mocks have been used
@@ -216,17 +231,24 @@
         # Update the archive after the remote feed is updated with item order changed
         reordered_item_request_mocks, _ = self.update_feed(
             archive_feed=self.archive_feed,
             remote_mock="reordered-item",
         )
         reordered_item_feed_path, _ = reordered_item_request_mocks[self.feed_url]
 
-        remote_tree = etree.parse(reordered_item_feed_path.open())
+        remote_tree = etree.parse(  # nosec: B320
+            reordered_item_feed_path.open(encoding="utf-8"),
+            parser=utils.XML_PARSER,
+        )
         remote_items = remote_tree.find("channel").findall("item")
-        archive_tree = etree.parse(self.feed_path.open())
+        with self.feed_path.open(encoding="utf-8") as feed_opened:
+            archive_tree = etree.parse(  # nosec: B320
+                feed_opened,
+                parser=utils.XML_PARSER,
+            )
         archive_items = archive_tree.find("channel").findall("item")
         self.assertEqual(
             archive_items[0].find("guid").text,
             remote_items[2].find("guid").text,
             "Item added at end of remote feed not at beginning of archive feed",
         )
         self.assertEqual(
@@ -238,22 +260,26 @@
             archive_items[2].find("guid").text,
             remote_items[0].find("guid").text,
             "Item original position in remote feed not preserved",
         )
 
     def test_feed_empty(self):
         """
-        Updating an empty feed works without any errors
+        Updating an empty feed works without any errors.
         """
         # Populate with a feed containing multiple items
         self.update_feed(
             archive_feed=self.archive_feed,
             remote_mock="empty",
         )
-        archive_tree = etree.parse(self.feed_path.open())
+        with self.feed_path.open(encoding="utf-8") as feed_opened:
+            archive_tree = etree.parse(  # nosec: B320
+                feed_opened,
+                parser=utils.XML_PARSER,
+            )
         archive_items = archive_tree.find("channel").findall("item")
         self.assertEqual(
             archive_items,
             [],
             "Archive contains items for an empty feed",
         )
 
@@ -264,16 +290,21 @@
         for feed_format_params in self.FEED_FORMAT_PARAMS:
             feed_format_class = feed_format_params["feed_format_class"]
             relative_path = feed_format_params["relative_path"]
             with self.subTest(
                 msg="Test one XML feed format",
                 feed_format_class=feed_format_class,
             ):
-                with (self.REMOTES_PATH / relative_path).open() as feed_opened:
-                    feed_tree = etree.parse(feed_opened)
+                with (self.REMOTES_PATH / relative_path).open(
+                    encoding="utf-8"
+                ) as feed_opened:
+                    feed_tree = etree.parse(  # nosec: B320
+                        feed_opened,
+                        parser=utils.XML_PARSER,
+                    )
                 feed_root = feed_tree.getroot()
                 feed_format = feed_format_class(self.archive_feed)
 
                 items_parent = feed_format.get_items_parent(feed_root)
                 self.assertEqual(
                     items_parent.tag,
                     feed_format_params["items_parent_tag"],
@@ -328,18 +359,20 @@
         # Test in the absence of the response headers
         no_header_feed_mock_path = (
             self.REMOTES_PATH
             / self.EXAMPLE_RELATIVE
             / "added-item"
             / tests.FeedarchiverTestCase.FEED_ARCHIVE_RELATIVE
         )
-        no_header_request_mock = self.requests_mock.get(
+        no_header_request_mock = self.client_mock.get(
             self.feed_url,
+        ).respond(
             content=no_header_feed_mock_path.read_bytes(),
         )
+        no_header_request_mock.reset()
         self.assert_no_header_download_mtime(
             no_header_request_mock,
             self.feed_path,
         )
 
     def test_feed_empty_archive_feed(self):
         """
@@ -352,28 +385,31 @@
         self.assertEqual(
             len(orig_archive_item_elems),
             1,
             "Wrong number of original archived feed items",
         )
 
         # The archive version of the feed was somehow written as an empty file.
-        self.feed_path.write_text("{'status': 'Got JSON instead of RSS'")
+        self.feed_path.write_text(
+            "{'status': 'Got JSON instead of RSS'",
+            encoding="utf-8",
+        )
         with self.assertLogs(
             feed.logger,
             level=logging.ERROR,
         ) as logged_msgs:
             self.archive_feed.update()
         self.assertEqual(
             get_mock.call_count,
             2,
             "Wrong number of original feed URL requests",
         )
         self.assertEqual(
             len(logged_msgs.records),
             1,
-            "Wrong number of download item logged records",
+            "Wrong number of logged feed records",
         )
         self.assertIn(
             "Unhandled exception parsing archive feed",
             logged_msgs.records[0].message,
             "Wrong logged record message",
         )
```

### Comparing `feed-archiver-1.0.0/src/feedarchiver/tests/test_urls.py` & `feed-archiver-1.0.0b11/src/feedarchiver/tests/test_urls.py`

 * *Files 7% similar despite different names*

```diff
@@ -50,15 +50,15 @@
             ),
             self.feed_path,
             "Different path after un-escaping and re-escaping",
         )
 
     def test_url_dir_index(self):
         """
-        URLs with trailing slashes are escaped to an index file: e.g. `index.html`.
+        Trailing slashes in URLs are escaped to an index file: e.g. `index.html`.
         """
         index_path = self.feed_path.parent / "index.html"
         dir_url = self.feed_url.rsplit("/", 1)[0] + "/"
         self.assertEqual(
             self.archive.path_to_url(index_path),
             dir_url,
             "Wrong directory URL for index path",
```

### Comparing `feed-archiver-1.0.0/src/feedarchiver/utils.py` & `feed-archiver-1.0.0b11/src/feedarchiver/utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,38 @@
 """
-Modifications to the standard library and other helpers.
+Utility functions or other shared constants and values.
+
+Particularly useful to avoid circular imports.
 """
 
 import os
 import functools
+import copy
 import mimetypes
 import urllib.parse
 import email
 import logging
 import tracemalloc
 
+import feedparser
+
+from lxml import etree  # nosec B410
+
 logger = logging.getLogger(__name__)
 
+# Configure the XML parser as securely as possible since we're parsing XML from
+# untrusted sources:
+# https://lxml.de/FAQ.html#how-do-i-use-lxml-safely-as-a-web-service-endpoint
+XML_PARSER = etree.XMLParser(resolve_entities=False)
+
 TRUE_STRS = {"1", "true", "yes", "on"}
-DEBUG = "DEBUG" in os.environ and os.environ["DEBUG"].strip().lower() in TRUE_STRS
-POST_MORTEM = (
+DEBUG = (  # noqa: F841
+    "DEBUG" in os.environ and os.environ["DEBUG"].strip().lower() in TRUE_STRS
+)
+POST_MORTEM = (  # noqa: F841
     "POST_MORTEM" in os.environ
     and os.environ["POST_MORTEM"].strip().lower() in TRUE_STRS
 )
 PYTHONTRACEMALLOC = (
     "PYTHONTRACEMALLOC" in os.environ
     and os.environ["PYTHONTRACEMALLOC"].strip().lower()
 )
@@ -61,15 +75,15 @@
     mimetypes_db = mimetypes._db  # pylint: disable=protected-access
     strict_types_map_inv = mimetypes_db.types_map_inv[True]
     loose_types_map_inv = mimetypes_db.types_map_inv[False]
 
     # Manually promote the priority extensions to the front of the list
     for priority_type, priority_ext in priority_types.items():
         priority_type = priority_type.lower()
-        if priority_type not in strict_types_map_inv:  # pragma: no cover
+        if priority_type not in strict_types_map_inv:
             # Must re-register as a strict type first
             mimetypes.add_type(priority_type, priority_ext)
         for types_map_inv in (strict_types_map_inv, loose_types_map_inv):
             if priority_type not in types_map_inv:
                 continue
             extensions = types_map_inv[priority_type] = list(
                 types_map_inv[priority_type],
@@ -102,21 +116,38 @@
 #         for char_idx, char in enumerate(string.printable)
 #         if urllib.parse.quote(char, safe=" ").startswith("%")
 #     ]
 #
 # Please do report any additional cases that cause issues in any other
 # common filesystems.
 SAFE_CHARS_WIN10_SAMBA = " !#$&'()+,;=@[]^`{}"
+QUOTED_SEP = urllib.parse.quote(os.sep, safe="")
+QUOTED_ALTSEP = None
+if os.altsep is not None:  # pragma: no cover
+    QUOTED_ALTSEP = urllib.parse.quote(os.altsep)
 quote_basename = functools.partial(urllib.parse.quote, safe=SAFE_CHARS_WIN10_SAMBA)
 quote_path = functools.partial(
     urllib.parse.quote,
     safe=f"{SAFE_CHARS_WIN10_SAMBA}{os.sep}{os.altsep}",
 )
 
 
+def quote_sep(string_):  # noqa: V103
+    """
+    Return the string with all occurrences of path separators, slashes, quoted.
+
+    Useful to sanitize input from feed XML when used in enclosure template plugin string
+    formats from adding unintended path parts.
+    """
+    quoted = string_.replace(os.sep, QUOTED_SEP)
+    if os.altsep is not None:  # pragma: no cover
+        quoted = quoted.replace(os.altsep, QUOTED_ALTSEP)
+    return quoted
+
+
 def compare_memory_snapshots(parent):  # pragma: no cover
     """
     Compare two traemalloc snapshots and log the results.
     """
     snapshot = tracemalloc.take_snapshot()
     if getattr(parent, "tracemalloc_snapshot", None) is not None:
         stats = snapshot.compare_to(
@@ -135,7 +166,42 @@
     Parse an RFC822-style `Content-Type` header.
 
     Useful to safely extract the MIME type from the charset.
     """
     message = email.message.Message()
     message["Content-Type"] = content_type
     return message.get_params()[0][0]
+
+
+def copy_empty_items_parent(feed_format, items_parent):
+    """
+    Create an `etree` copy of the feed items parent without any items.
+
+    Useful for richer parsing of single items at a time.
+    """
+    items_parent_copy = etree.Element(items_parent.tag, items_parent.attrib)
+    for child in items_parent:
+        if child.tag == feed_format.ITEM_TAG:
+            # Optimization: This is not strictly correct as feed XML may contain
+            # non-item elements after feed item elements, either interspersed or at the
+            # end.  This is rare, however, in fact I've never seen an instance of it,
+            # items are *most* of a feed's elements and use of the items parent other
+            # elements in enclosure plugin configurations is rare, so avoid unnecessary
+            # iteration until someone reports an issue with this.
+            break
+        items_parent_copy.append(copy.deepcopy(child))
+    return items_parent_copy
+
+
+# We need to parse the archive and remote feed XML using `etree` because we need to be
+# able to modify the XML and write it to the archive, something that `feedparser`
+# doesn't provide.  enclosure plugins, however, frequently need the richer parsing
+# support that `feedparser` *does* provide, such as parsing dates and times.  That rich
+# parsing is only needed in the rare case of new items being added to the archive's
+# version of the feed, so only do the rich parsing on a per-item basis.
+def parse_item_feed(feed_format, feed_elem, item_elem):
+    """
+    Reconstruct a "feed" of just one item and return the richly parsed version.
+    """
+    item_feed_elem = copy_empty_items_parent(feed_format, feed_elem)
+    item_feed_elem.append(copy.deepcopy(item_elem))
+    return feedparser.parse(etree.tostring(item_feed_elem))
```

