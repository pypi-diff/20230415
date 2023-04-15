# Comparing `tmp/bovine-0.1.0.tar.gz` & `tmp/bovine-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bovine-0.1.0.tar", max compression
+gzip compressed data, was "bovine-0.1.1.tar", max compression
```

## Comparing `bovine-0.1.0.tar` & `bovine-0.1.1.tar`

### file list

```diff
@@ -1,104 +1,96 @@
--rw-r--r--   0        0        0     9111 2023-04-13 15:55:57.830393 bovine-0.1.0/README.md
--rw-r--r--   0        0        0     8584 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/__init__.py
--rw-r--r--   0        0        0        0 2023-04-13 15:55:57.986394 bovine-0.1.0/bovine/activitypub/__init__.py
--rw-r--r--   0        0        0      172 2023-04-13 15:56:35.630722 bovine-0.1.0/bovine/activitypub/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3091 2023-04-13 15:56:35.630722 bovine-0.1.0/bovine/activitypub/__pycache__/authorization_wrapper.cpython-310.pyc
--rw-r--r--   0        0        0     2476 2023-04-13 15:56:36.070726 bovine-0.1.0/bovine/activitypub/__pycache__/collection_helper.cpython-310.pyc
--rw-r--r--   0        0        0      905 2023-04-13 15:56:36.202727 bovine-0.1.0/bovine/activitypub/__pycache__/collection_iterator.cpython-310.pyc
--rw-r--r--   0        0        0     3664 2023-04-13 15:56:36.210727 bovine-0.1.0/bovine/activitypub/__pycache__/test_actor.cpython-310-pytest-7.3.0.pyc
--rw-r--r--   0        0        0     2736 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/activitypub/authorization_wrapper.py
--rw-r--r--   0        0        0     2219 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/activitypub/collection_helper.py
--rw-r--r--   0        0        0      429 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/activitypub/collection_iterator.py
--rw-r--r--   0        0        0     2909 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/activitypub/test_actor.py
--rw-r--r--   0        0        0     3664 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/activitystreams/__init__.py
--rw-r--r--   0        0        0     3386 2023-04-13 15:56:36.194727 bovine-0.1.0/bovine/activitystreams/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3838 2023-04-13 15:56:36.194727 bovine-0.1.0/bovine/activitystreams/__pycache__/activity_factory.cpython-310.pyc
--rw-r--r--   0        0        0     4085 2023-04-13 15:56:36.198727 bovine-0.1.0/bovine/activitystreams/__pycache__/object_factory.cpython-310.pyc
--rw-r--r--   0        0        0     1493 2023-04-13 15:56:36.198727 bovine-0.1.0/bovine/activitystreams/__pycache__/ordered_collection_builder.cpython-310.pyc
--rw-r--r--   0        0        0     1443 2023-04-13 15:56:36.198727 bovine-0.1.0/bovine/activitystreams/__pycache__/ordered_collection_page_builder.cpython-310.pyc
--rw-r--r--   0        0        0     4559 2023-04-13 15:56:36.242727 bovine-0.1.0/bovine/activitystreams/__pycache__/test_activity_factory.cpython-310-pytest-7.3.0.pyc
--rw-r--r--   0        0        0     3304 2023-04-13 15:56:36.266727 bovine-0.1.0/bovine/activitystreams/__pycache__/test_actor.cpython-310-pytest-7.3.0.pyc
--rw-r--r--   0        0        0     3167 2023-04-13 15:56:36.270727 bovine-0.1.0/bovine/activitystreams/__pycache__/test_object_factory.cpython-310-pytest-7.3.0.pyc
--rw-r--r--   0        0        0     2095 2023-04-13 15:56:36.274727 bovine-0.1.0/bovine/activitystreams/__pycache__/test_ordered_collection_builder.cpython-310-pytest-7.3.0.pyc
--rw-r--r--   0        0        0     1431 2023-04-13 15:56:36.278727 bovine-0.1.0/bovine/activitystreams/__pycache__/test_ordered_collection_page_builder.cpython-310-pytest-7.3.0.pyc
--rw-r--r--   0        0        0     3726 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/activitystreams/activity_factory.py
--rw-r--r--   0        0        0     4240 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/activitystreams/object_factory.py
--rw-r--r--   0        0        0      949 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/activitystreams/ordered_collection_builder.py
--rw-r--r--   0        0        0      899 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/activitystreams/ordered_collection_page_builder.py
--rw-r--r--   0        0        0     2163 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/activitystreams/test_activity_factory.py
--rw-r--r--   0        0        0     1418 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/activitystreams/test_actor.py
--rw-r--r--   0        0        0     1381 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/activitystreams/test_object_factory.py
--rw-r--r--   0        0        0     1165 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/activitystreams/test_ordered_collection_builder.py
--rw-r--r--   0        0        0      907 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/activitystreams/test_ordered_collection_page_builder.py
--rw-r--r--   0        0        0     2354 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/activitystreams/utils/__init__.py
--rw-r--r--   0        0        0     2835 2023-04-13 15:56:36.198727 bovine-0.1.0/bovine/activitystreams/utils/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      907 2023-04-13 15:56:36.202727 bovine-0.1.0/bovine/activitystreams/utils/__pycache__/print.cpython-310.pyc
--rw-r--r--   0        0        0     4762 2023-04-13 15:56:36.290727 bovine-0.1.0/bovine/activitystreams/utils/__pycache__/test_utils.cpython-310-pytest-7.3.0.pyc
--rw-r--r--   0        0        0      787 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/activitystreams/utils/print.py
--rw-r--r--   0        0        0     2266 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/activitystreams/utils/test_utils.py
--rw-r--r--   0        0        0     1326 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/clients/__init__.py
--rw-r--r--   0        0        0     1480 2023-04-13 15:56:35.870724 bovine-0.1.0/bovine/clients/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      267 2023-04-13 15:56:35.874724 bovine-0.1.0/bovine/clients/__pycache__/consts.cpython-310.pyc
--rw-r--r--   0        0        0     1471 2023-04-13 15:56:36.070726 bovine-0.1.0/bovine/clients/__pycache__/event_source.cpython-310.pyc
--rw-r--r--   0        0        0     1013 2023-04-13 15:56:35.874724 bovine-0.1.0/bovine/clients/__pycache__/lookup_account.cpython-310.pyc
--rw-r--r--   0        0        0     2507 2023-04-13 15:56:35.874724 bovine-0.1.0/bovine/clients/__pycache__/moo_auth_client.cpython-310.pyc
--rw-r--r--   0        0        0     1549 2023-04-13 15:56:36.302728 bovine-0.1.0/bovine/clients/__pycache__/nodeinfo.cpython-310.pyc
--rw-r--r--   0        0        0     2470 2023-04-13 15:56:36.070726 bovine-0.1.0/bovine/clients/__pycache__/signed_http.cpython-310.pyc
--rw-r--r--   0        0        0     1470 2023-04-13 15:56:36.070726 bovine-0.1.0/bovine/clients/__pycache__/signed_http_client.cpython-310.pyc
--rw-r--r--   0        0        0     1351 2023-04-13 15:56:36.294728 bovine-0.1.0/bovine/clients/__pycache__/test_event_source.cpython-310-pytest-7.3.0.pyc
--rw-r--r--   0        0        0     1575 2023-04-13 15:56:36.298728 bovine-0.1.0/bovine/clients/__pycache__/test_lookup_account.cpython-310-pytest-7.3.0.pyc
--rw-r--r--   0        0        0     1224 2023-04-13 15:56:36.298728 bovine-0.1.0/bovine/clients/__pycache__/test_nodeinfo.cpython-310-pytest-7.3.0.pyc
--rw-r--r--   0        0        0     2093 2023-04-13 15:56:36.306728 bovine-0.1.0/bovine/clients/__pycache__/test_signed_http.cpython-310-pytest-7.3.0.pyc
--rw-r--r--   0        0        0      820 2023-04-13 15:56:36.306728 bovine-0.1.0/bovine/clients/__pycache__/test_signed_http_client.cpython-310-pytest-7.3.0.pyc
--rw-r--r--   0        0        0       91 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/clients/consts.py
--rw-r--r--   0        0        0     1106 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/clients/event_source.py
--rw-r--r--   0        0        0      787 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/clients/lookup_account.py
--rw-r--r--   0        0        0     3176 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/clients/moo_auth_client.py
--rw-r--r--   0        0        0     1399 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/clients/nodeinfo.py
--rw-r--r--   0        0        0     3278 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/clients/signed_http.py
--rw-r--r--   0        0        0     1074 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/clients/signed_http_client.py
--rw-r--r--   0        0        0      609 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/clients/test_event_source.py
--rw-r--r--   0        0        0      624 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/clients/test_lookup_account.py
--rw-r--r--   0        0        0      327 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/clients/test_nodeinfo.py
--rw-r--r--   0        0        0     1145 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/clients/test_signed_http.py
--rw-r--r--   0        0        0      529 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/clients/test_signed_http_client.py
--rw-r--r--   0        0        0     3999 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/crypto/__init__.py
--rw-r--r--   0        0        0     3633 2023-04-13 15:56:35.874724 bovine-0.1.0/bovine/crypto/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2921 2023-04-13 15:56:36.014725 bovine-0.1.0/bovine/crypto/__pycache__/helper.cpython-310.pyc
--rw-r--r--   0        0        0     2908 2023-04-13 15:56:36.014725 bovine-0.1.0/bovine/crypto/__pycache__/http_signature.cpython-310.pyc
--rw-r--r--   0        0        0     2256 2023-04-13 15:56:36.018725 bovine-0.1.0/bovine/crypto/__pycache__/signature_checker.cpython-310.pyc
--rw-r--r--   0        0        0     1783 2023-04-13 15:56:36.066726 bovine-0.1.0/bovine/crypto/__pycache__/signature_parser.cpython-310.pyc
--rw-r--r--   0        0        0     2362 2023-04-13 15:56:36.230727 bovine-0.1.0/bovine/crypto/__pycache__/test.cpython-310.pyc
--rw-r--r--   0        0        0     5809 2023-04-13 15:56:36.314728 bovine-0.1.0/bovine/crypto/__pycache__/test_crypto.cpython-310-pytest-7.3.0.pyc
--rw-r--r--   0        0        0     2741 2023-04-13 15:56:36.318728 bovine-0.1.0/bovine/crypto/__pycache__/test_helper.cpython-310-pytest-7.3.0.pyc
--rw-r--r--   0        0        0     7453 2023-04-13 15:56:36.334728 bovine-0.1.0/bovine/crypto/__pycache__/test_http_signature.cpython-310-pytest-7.3.0.pyc
--rw-r--r--   0        0        0     2673 2023-04-13 15:56:36.346728 bovine-0.1.0/bovine/crypto/__pycache__/test_signature_parser.cpython-310-pytest-7.3.0.pyc
--rw-r--r--   0        0        0     2764 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/crypto/helper.py
--rw-r--r--   0        0        0     2112 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/crypto/http_signature.py
--rw-r--r--   0        0        0     2942 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/crypto/signature_checker.py
--rw-r--r--   0        0        0     1266 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/crypto/signature_parser.py
--rw-r--r--   0        0        0     2199 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/crypto/test.py
--rw-r--r--   0        0        0     4989 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/crypto/test_crypto.py
--rw-r--r--   0        0        0      896 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/crypto/test_helper.py
--rw-r--r--   0        0        0     5081 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/crypto/test_http_signature.py
--rw-r--r--   0        0        0     1207 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/crypto/test_signature_parser.py
--rw-r--r--   0        0        0      178 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/test_bovine_client.py
--rw-r--r--   0        0        0      282 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/test_types.py
--rw-r--r--   0        0        0     1837 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/types.py
--rw-r--r--   0        0        0        0 2023-04-13 15:55:57.986394 bovine-0.1.0/bovine/utils/__init__.py
--rw-r--r--   0        0        0      166 2023-04-13 15:56:35.870724 bovine-0.1.0/bovine/utils/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      876 2023-04-13 15:56:36.018725 bovine-0.1.0/bovine/utils/__pycache__/date.cpython-310.pyc
--rw-r--r--   0        0        0      365 2023-04-13 15:56:35.870724 bovine-0.1.0/bovine/utils/__pycache__/parse.cpython-310.pyc
--rw-r--r--   0        0        0     3442 2023-04-13 15:56:36.366728 bovine-0.1.0/bovine/utils/__pycache__/test_date.cpython-310-pytest-7.3.0.pyc
--rw-r--r--   0        0        0     1666 2023-04-13 15:56:36.370728 bovine-0.1.0/bovine/utils/__pycache__/test_parse.cpython-310-pytest-7.3.0.pyc
--rw-r--r--   0        0        0      981 2023-04-13 15:56:36.374728 bovine-0.1.0/bovine/utils/__pycache__/test_webfinger.cpython-310-pytest-7.3.0.pyc
--rw-r--r--   0        0        0      456 2023-04-13 15:56:36.374728 bovine-0.1.0/bovine/utils/__pycache__/webfinger.cpython-310.pyc
--rw-r--r--   0        0        0      519 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/utils/date.py
--rw-r--r--   0        0        0      186 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/utils/parse.py
--rw-r--r--   0        0        0      181 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/utils/test.py
--rw-r--r--   0        0        0      737 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/utils/test_date.py
--rw-r--r--   0        0        0      457 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/utils/test_parse.py
--rw-r--r--   0        0        0      200 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/utils/test_webfinger.py
--rw-r--r--   0        0        0      332 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/utils/webfinger.py
--rw-r--r--   0        0        0     1184 2023-04-13 15:55:57.834393 bovine-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    10012 1970-01-01 00:00:00.000000 bovine-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      627 2023-04-15 18:19:16.463381 bovine-0.1.1/README.md
+-rw-r--r--   0        0        0     8584 2023-04-15 18:19:16.463381 bovine-0.1.1/bovine/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-15 18:19:16.587382 bovine-0.1.1/bovine/activitypub/__init__.py
+-rw-r--r--   0        0        0      173 2023-04-15 18:19:52.807613 bovine-0.1.1/bovine/activitypub/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3092 2023-04-15 18:19:52.807613 bovine-0.1.1/bovine/activitypub/__pycache__/authorization_wrapper.cpython-310.pyc
+-rw-r--r--   0        0        0     2477 2023-04-15 18:19:53.195615 bovine-0.1.1/bovine/activitypub/__pycache__/collection_helper.cpython-310.pyc
+-rw-r--r--   0        0        0      906 2023-04-15 18:19:53.303616 bovine-0.1.1/bovine/activitypub/__pycache__/collection_iterator.cpython-310.pyc
+-rw-r--r--   0        0        0     3638 2023-04-15 18:19:53.311616 bovine-0.1.1/bovine/activitypub/__pycache__/test_actor.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0     2736 2023-04-15 18:19:16.463381 bovine-0.1.1/bovine/activitypub/authorization_wrapper.py
+-rw-r--r--   0        0        0     2219 2023-04-15 18:19:16.463381 bovine-0.1.1/bovine/activitypub/collection_helper.py
+-rw-r--r--   0        0        0      429 2023-04-15 18:19:16.463381 bovine-0.1.1/bovine/activitypub/collection_iterator.py
+-rw-r--r--   0        0        0     2757 2023-04-15 18:19:16.463381 bovine-0.1.1/bovine/activitypub/test_actor.py
+-rw-r--r--   0        0        0     4623 2023-04-15 18:19:16.463381 bovine-0.1.1/bovine/activitystreams/__init__.py
+-rw-r--r--   0        0        0     4224 2023-04-15 18:19:53.295616 bovine-0.1.1/bovine/activitystreams/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     4093 2023-04-15 18:19:53.295616 bovine-0.1.1/bovine/activitystreams/__pycache__/activity_factory.cpython-310.pyc
+-rw-r--r--   0        0        0     4086 2023-04-15 18:19:53.299616 bovine-0.1.1/bovine/activitystreams/__pycache__/object_factory.cpython-310.pyc
+-rw-r--r--   0        0        0     4560 2023-04-15 18:19:53.343616 bovine-0.1.1/bovine/activitystreams/__pycache__/test_activity_factory.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0     3305 2023-04-15 18:19:53.351616 bovine-0.1.1/bovine/activitystreams/__pycache__/test_actor.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0     3168 2023-04-15 18:19:53.359616 bovine-0.1.1/bovine/activitystreams/__pycache__/test_object_factory.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0     1929 2023-04-15 18:19:53.363616 bovine-0.1.1/bovine/activitystreams/__pycache__/test_ordered_collection_builder.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0     1368 2023-04-15 18:19:53.367616 bovine-0.1.1/bovine/activitystreams/__pycache__/test_ordered_collection_page.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0     4012 2023-04-15 18:19:16.463381 bovine-0.1.1/bovine/activitystreams/activity_factory.py
+-rw-r--r--   0        0        0     4240 2023-04-15 18:19:16.463381 bovine-0.1.1/bovine/activitystreams/object_factory.py
+-rw-r--r--   0        0        0     2163 2023-04-15 18:19:16.463381 bovine-0.1.1/bovine/activitystreams/test_activity_factory.py
+-rw-r--r--   0        0        0     1418 2023-04-15 18:19:16.463381 bovine-0.1.1/bovine/activitystreams/test_actor.py
+-rw-r--r--   0        0        0     1381 2023-04-15 18:19:16.463381 bovine-0.1.1/bovine/activitystreams/test_object_factory.py
+-rw-r--r--   0        0        0     1010 2023-04-15 18:19:16.463381 bovine-0.1.1/bovine/activitystreams/test_ordered_collection_builder.py
+-rw-r--r--   0        0        0      809 2023-04-15 18:19:16.463381 bovine-0.1.1/bovine/activitystreams/test_ordered_collection_page.py
+-rw-r--r--   0        0        0     2354 2023-04-15 18:19:16.463381 bovine-0.1.1/bovine/activitystreams/utils/__init__.py
+-rw-r--r--   0        0        0     2836 2023-04-15 18:19:53.299616 bovine-0.1.1/bovine/activitystreams/utils/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      908 2023-04-15 18:19:53.303616 bovine-0.1.1/bovine/activitystreams/utils/__pycache__/print.cpython-310.pyc
+-rw-r--r--   0        0        0     4763 2023-04-15 18:19:53.375616 bovine-0.1.1/bovine/activitystreams/utils/__pycache__/test_utils.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0      787 2023-04-15 18:19:16.463381 bovine-0.1.1/bovine/activitystreams/utils/print.py
+-rw-r--r--   0        0        0     2266 2023-04-15 18:19:16.463381 bovine-0.1.1/bovine/activitystreams/utils/test_utils.py
+-rw-r--r--   0        0        0     2081 2023-04-15 18:19:16.463381 bovine-0.1.1/bovine/clients/__init__.py
+-rw-r--r--   0        0        0     2209 2023-04-15 18:19:53.011614 bovine-0.1.1/bovine/clients/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      268 2023-04-15 18:19:53.011614 bovine-0.1.1/bovine/clients/__pycache__/consts.cpython-310.pyc
+-rw-r--r--   0        0        0     1472 2023-04-15 18:19:53.191615 bovine-0.1.1/bovine/clients/__pycache__/event_source.cpython-310.pyc
+-rw-r--r--   0        0        0     1014 2023-04-15 18:19:53.011614 bovine-0.1.1/bovine/clients/__pycache__/lookup_account.cpython-310.pyc
+-rw-r--r--   0        0        0     2508 2023-04-15 18:19:53.015614 bovine-0.1.1/bovine/clients/__pycache__/moo_auth_client.cpython-310.pyc
+-rw-r--r--   0        0        0     1237 2023-04-15 18:19:53.015614 bovine-0.1.1/bovine/clients/__pycache__/nodeinfo.cpython-310.pyc
+-rw-r--r--   0        0        0     2471 2023-04-15 18:19:53.191615 bovine-0.1.1/bovine/clients/__pycache__/signed_http.cpython-310.pyc
+-rw-r--r--   0        0        0     1471 2023-04-15 18:19:53.191615 bovine-0.1.1/bovine/clients/__pycache__/signed_http_client.cpython-310.pyc
+-rw-r--r--   0        0        0     1352 2023-04-15 18:19:53.383616 bovine-0.1.1/bovine/clients/__pycache__/test_event_source.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0     1576 2023-04-15 18:19:53.383616 bovine-0.1.1/bovine/clients/__pycache__/test_lookup_account.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0     1217 2023-04-15 18:19:53.387616 bovine-0.1.1/bovine/clients/__pycache__/test_nodeinfo.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0     2094 2023-04-15 18:19:53.391616 bovine-0.1.1/bovine/clients/__pycache__/test_signed_http.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0      821 2023-04-15 18:19:53.391616 bovine-0.1.1/bovine/clients/__pycache__/test_signed_http_client.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0       91 2023-04-15 18:19:16.463381 bovine-0.1.1/bovine/clients/consts.py
+-rw-r--r--   0        0        0     1106 2023-04-15 18:19:16.463381 bovine-0.1.1/bovine/clients/event_source.py
+-rw-r--r--   0        0        0      787 2023-04-15 18:19:16.463381 bovine-0.1.1/bovine/clients/lookup_account.py
+-rw-r--r--   0        0        0     3176 2023-04-15 18:19:16.463381 bovine-0.1.1/bovine/clients/moo_auth_client.py
+-rw-r--r--   0        0        0      948 2023-04-15 18:19:16.463381 bovine-0.1.1/bovine/clients/nodeinfo.py
+-rw-r--r--   0        0        0     3278 2023-04-15 18:19:16.463381 bovine-0.1.1/bovine/clients/signed_http.py
+-rw-r--r--   0        0        0     1074 2023-04-15 18:19:16.463381 bovine-0.1.1/bovine/clients/signed_http_client.py
+-rw-r--r--   0        0        0      609 2023-04-15 18:19:16.463381 bovine-0.1.1/bovine/clients/test_event_source.py
+-rw-r--r--   0        0        0      624 2023-04-15 18:19:16.463381 bovine-0.1.1/bovine/clients/test_lookup_account.py
+-rw-r--r--   0        0        0      319 2023-04-15 18:19:16.463381 bovine-0.1.1/bovine/clients/test_nodeinfo.py
+-rw-r--r--   0        0        0     1145 2023-04-15 18:19:16.463381 bovine-0.1.1/bovine/clients/test_signed_http.py
+-rw-r--r--   0        0        0      529 2023-04-15 18:19:16.463381 bovine-0.1.1/bovine/clients/test_signed_http_client.py
+-rw-r--r--   0        0        0     3999 2023-04-15 18:19:16.463381 bovine-0.1.1/bovine/crypto/__init__.py
+-rw-r--r--   0        0        0     3634 2023-04-15 18:19:53.015614 bovine-0.1.1/bovine/crypto/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2863 2023-04-15 18:19:53.147615 bovine-0.1.1/bovine/crypto/__pycache__/helper.cpython-310.pyc
+-rw-r--r--   0        0        0     2909 2023-04-15 18:19:53.151615 bovine-0.1.1/bovine/crypto/__pycache__/http_signature.cpython-310.pyc
+-rw-r--r--   0        0        0     2257 2023-04-15 18:19:53.151615 bovine-0.1.1/bovine/crypto/__pycache__/signature_checker.cpython-310.pyc
+-rw-r--r--   0        0        0     1784 2023-04-15 18:19:53.191615 bovine-0.1.1/bovine/crypto/__pycache__/signature_parser.cpython-310.pyc
+-rw-r--r--   0        0        0     2363 2023-04-15 18:19:53.331616 bovine-0.1.1/bovine/crypto/__pycache__/test.cpython-310.pyc
+-rw-r--r--   0        0        0     5810 2023-04-15 18:19:53.399617 bovine-0.1.1/bovine/crypto/__pycache__/test_crypto.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0     2742 2023-04-15 18:19:53.403617 bovine-0.1.1/bovine/crypto/__pycache__/test_helper.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0     7454 2023-04-15 18:19:53.415617 bovine-0.1.1/bovine/crypto/__pycache__/test_http_signature.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0     2674 2023-04-15 18:19:53.423617 bovine-0.1.1/bovine/crypto/__pycache__/test_signature_parser.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0     2664 2023-04-15 18:19:16.463381 bovine-0.1.1/bovine/crypto/helper.py
+-rw-r--r--   0        0        0     2112 2023-04-15 18:19:16.463381 bovine-0.1.1/bovine/crypto/http_signature.py
+-rw-r--r--   0        0        0     2942 2023-04-15 18:19:16.463381 bovine-0.1.1/bovine/crypto/signature_checker.py
+-rw-r--r--   0        0        0     1266 2023-04-15 18:19:16.463381 bovine-0.1.1/bovine/crypto/signature_parser.py
+-rw-r--r--   0        0        0     2199 2023-04-15 18:19:16.463381 bovine-0.1.1/bovine/crypto/test.py
+-rw-r--r--   0        0        0     4989 2023-04-15 18:19:16.463381 bovine-0.1.1/bovine/crypto/test_crypto.py
+-rw-r--r--   0        0        0      896 2023-04-15 18:19:16.463381 bovine-0.1.1/bovine/crypto/test_helper.py
+-rw-r--r--   0        0        0     5081 2023-04-15 18:19:16.467381 bovine-0.1.1/bovine/crypto/test_http_signature.py
+-rw-r--r--   0        0        0     1207 2023-04-15 18:19:16.467381 bovine-0.1.1/bovine/crypto/test_signature_parser.py
+-rw-r--r--   0        0        0      178 2023-04-15 18:19:16.467381 bovine-0.1.1/bovine/test_bovine_client.py
+-rw-r--r--   0        0        0      282 2023-04-15 18:19:16.467381 bovine-0.1.1/bovine/test_types.py
+-rw-r--r--   0        0        0     2397 2023-04-15 18:19:16.467381 bovine-0.1.1/bovine/types.py
+-rw-r--r--   0        0        0      667 2023-04-15 18:19:16.467381 bovine-0.1.1/bovine/utils/__init__.py
+-rw-r--r--   0        0        0      848 2023-04-15 18:19:53.011614 bovine-0.1.1/bovine/utils/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      877 2023-04-15 18:19:53.151615 bovine-0.1.1/bovine/utils/__pycache__/date.cpython-310.pyc
+-rw-r--r--   0        0        0     3443 2023-04-15 18:19:53.431617 bovine-0.1.1/bovine/utils/__pycache__/test_date.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0     1662 2023-04-15 18:19:53.435617 bovine-0.1.1/bovine/utils/__pycache__/test_parse.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0      973 2023-04-15 18:19:53.439617 bovine-0.1.1/bovine/utils/__pycache__/test_webfinger.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0      519 2023-04-15 18:19:16.467381 bovine-0.1.1/bovine/utils/date.py
+-rw-r--r--   0        0        0      181 2023-04-15 18:19:16.467381 bovine-0.1.1/bovine/utils/test.py
+-rw-r--r--   0        0        0      737 2023-04-15 18:19:16.467381 bovine-0.1.1/bovine/utils/test_date.py
+-rw-r--r--   0        0        0      452 2023-04-15 18:19:16.467381 bovine-0.1.1/bovine/utils/test_parse.py
+-rw-r--r--   0        0        0      191 2023-04-15 18:19:16.467381 bovine-0.1.1/bovine/utils/test_webfinger.py
+-rw-r--r--   0        0        0     1178 2023-04-15 18:19:16.467381 bovine-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1523 1970-01-01 00:00:00.000000 bovine-0.1.1/PKG-INFO
```

### Comparing `bovine-0.1.0/bovine/__init__.py` & `bovine-0.1.1/bovine/__init__.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.0/bovine/activitypub/__pycache__/authorization_wrapper.cpython-310.pyc` & `bovine-0.1.1/bovine/activitypub/__pycache__/authorization_wrapper.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 13 15:55:57 2023 UTC, .py size: 2736 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0d26 3864 b00a 0000  o........&8d....
+00000000: 6f0d 0d0a 0000 0000 a4ea 3a64 b00a 0000  o.........:d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 6800 0000 6400  .....@...sh...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6401 6c03 5a03 6400 6403 6c04  ..d.d.l.Z.d.d.l.
 00000050: 6d05 5a05 0100 6400 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6405 6c08 6d09 5a09 0100 6400  ..d.d.l.m.Z...d.
 00000070: 6406 6c0a 6d0b 5a0b 0100 6500 a00c 650d  d.l.m.Z...e...e.
@@ -31,164 +31,164 @@
 000001e0: 6572 6301 0000 0000 0000 0000 0000 0001  erc.............
 000001f0: 0000 0002 0000 0043 0000 0073 1c00 0000  .......C...s....
 00000200: 6400 7c00 5f00 6400 7c00 5f01 6400 7c00  d.|._.d.|._.d.|.
 00000210: 5f02 6400 7c00 5f03 6400 5300 a901 4e29  _.d.|._.d.S...N)
 00000220: 04da 0663 6f6e 6669 67da 0861 6374 6f72  ...config..actor
 00000230: 5f69 64da 0663 6c69 656e 74da 0773 6573  _id..client..ses
 00000240: 7369 6f6e a901 da04 7365 6c66 a900 720f  sion....self..r.
-00000250: 0000 00fa 5c2f 776f 6f64 7065 636b 6572  ....\/woodpecker
+00000250: 0000 00fa 5d2f 776f 6f64 7065 636b 6572  ....]/woodpecker
 00000260: 2f73 7263 2f63 6f64 6562 6572 672e 6f72  /src/codeberg.or
-00000270: 672f 6865 6c67 652f 626f 7669 6e65 2f62  g/helge/bovine/b
-00000280: 6f76 696e 652f 626f 7669 6e65 2f61 6374  ovine/bovine/act
-00000290: 6976 6974 7970 7562 2f61 7574 686f 7269  ivitypub/authori
-000002a0: 7a61 7469 6f6e 5f77 7261 7070 6572 2e70  zation_wrapper.p
-000002b0: 79da 085f 5f69 6e69 745f 5f0f 0000 0073  y..__init__....s
-000002c0: 0800 0000 0601 0601 0601 0a01 7a1d 4175  ............z.Au
-000002d0: 7468 6f72 697a 6174 696f 6e57 7261 7070  thorizationWrapp
-000002e0: 6572 2e5f 5f69 6e69 745f 5f63 0100 0000  er.__init__c....
-000002f0: 0000 0000 0000 0000 0100 0000 0200 0000  ................
-00000300: c300 0000 7314 0000 0081 017c 00a0 00a1  ....s......|....
-00000310: 0049 0064 0048 0001 007c 0053 0072 0800  .I.d.H...|.S.r..
-00000320: 0000 2901 da04 696e 6974 720d 0000 0072  ..)...initr....r
-00000330: 0f00 0000 720f 0000 0072 1000 0000 da0a  ....r....r......
-00000340: 5f5f 6165 6e74 6572 5f5f 1500 0000 7306  __aenter__....s.
-00000350: 0000 0002 800e 0104 017a 1f41 7574 686f  .........z.Autho
-00000360: 7269 7a61 7469 6f6e 5772 6170 7065 722e  rizationWrapper.
-00000370: 5f5f 6165 6e74 6572 5f5f 6301 0000 0000  __aenter__c.....
-00000380: 0000 0000 0000 0002 0000 0002 0000 00c7  ................
-00000390: 0000 0073 1600 0000 8101 7c00 6a00 a001  ...s......|.j...
-000003a0: a100 4900 6400 4800 0100 6400 5300 7208  ..I.d.H...d.S.r.
-000003b0: 0000 0029 0272 0c00 0000 da05 636c 6f73  ...).r......clos
-000003c0: 6529 0272 0e00 0000 da04 6172 6773 720f  e).r......argsr.
-000003d0: 0000 0072 0f00 0000 7210 0000 00da 095f  ...r....r......_
-000003e0: 5f61 6578 6974 5f5f 1900 0000 7304 0000  _aexit__....s...
-000003f0: 0002 8014 017a 1e41 7574 686f 7269 7a61  .....z.Authoriza
-00000400: 7469 6f6e 5772 6170 7065 722e 5f5f 6165  tionWrapper.__ae
-00000410: 7869 745f 5f4e 720c 0000 0063 0200 0000  xit__Nr....c....
-00000420: 0000 0000 0000 0000 0200 0000 0500 0000  ................
-00000430: c300 0000 7392 0000 0081 017c 017c 005f  ....s......|.|._
-00000440: 007c 0164 0075 0072 0d74 01a0 02a1 007c  .|.d.u.r.t.....|
-00000450: 005f 007c 006a 0373 124a 0082 017c 00a0  ._.|.j.s.J...|..
-00000460: 04a1 0072 2a7c 006a 057c 006a 0364 0119  ...r*|.j.|.j.d..
-00000470: 007c 006a 0364 0219 007c 006a 0064 038d  .|.j.d...|.j.d..
-00000480: 0349 0064 0048 0001 0064 0053 007c 00a0  .I.d.H...d.S.|..
-00000490: 06a1 0072 457c 006a 0364 0419 007c 005f  ...rE|.j.d...|._
-000004a0: 077c 006a 087c 006a 0364 0519 007c 006a  .|.j.|.j.d...|.j
-000004b0: 0364 0219 007c 006a 0064 038d 0301 0064  .d...|.j.d.....d
-000004c0: 0053 0074 0964 0683 0182 0129 074e da04  .S.t.d.....).N..
-000004d0: 686f 7374 da0b 7072 6976 6174 655f 6b65  host..private_ke
-000004e0: 7929 0172 0c00 0000 da0b 6163 636f 756e  y).r......accoun
-000004f0: 745f 7572 6cda 0e70 7562 6c69 635f 6b65  t_url..public_ke
-00000500: 795f 7572 6c7a 274e 6f20 6b6e 6f77 6e20  y_urlz'No known 
-00000510: 6175 7468 6f72 697a 6174 696f 6e20 6d65  authorization me
-00000520: 7468 6f64 2061 7661 696c 6162 6c65 290a  thod available).
-00000530: 720c 0000 00da 0761 696f 6874 7470 da0d  r......aiohttp..
-00000540: 436c 6965 6e74 5365 7373 696f 6e72 0900  ClientSessionr..
-00000550: 0000 da0d 5f68 6173 5f6d 6f6f 5f61 7574  ...._has_moo_aut
-00000560: 68da 2177 6974 685f 686f 7374 5f61 6e64  h.!with_host_and
-00000570: 5f65 6432 3535 3139 5f70 7269 7661 7465  _ed25519_private
-00000580: 5f6b 6579 da13 5f68 6173 5f68 7474 705f  _key.._has_http_
-00000590: 7369 676e 6174 7572 6572 0a00 0000 da13  signaturer......
-000005a0: 7769 7468 5f68 7474 705f 7369 676e 6174  with_http_signat
-000005b0: 7572 65da 0945 7863 6570 7469 6f6e 2902  ure..Exception).
-000005c0: 720e 0000 0072 0c00 0000 720f 0000 0072  r....r....r....r
-000005d0: 0f00 0000 7210 0000 0072 1200 0000 1c00  ....r....r......
-000005e0: 0000 7322 0000 0002 8006 0108 010a 010a  ..s"............
-000005f0: 0208 0204 0114 0110 ff08 030c 0104 0108  ................
-00000600: 0108 0104 010a fd08 067a 1941 7574 686f  .........z.Autho
-00000610: 7269 7a61 7469 6f6e 5772 6170 7065 722e  rizationWrapper.
-00000620: 696e 6974 7217 0000 0072 1800 0000 6304  initr....r....c.
-00000630: 0000 0000 0000 0000 0000 0005 0000 0004  ................
-00000640: 0000 00c3 0000 0073 4000 0000 8101 7c03  .......s@.....|.
-00000650: 6400 7500 7209 7400 a001 a100 7d03 7402  d.u.r.t.....}.t.
-00000660: 7c02 8301 7d04 7403 7c03 7c01 7c04 8303  |...}.t.|.|.|...
-00000670: 4900 6400 4800 7c00 5f04 7405 7c03 7c04  I.d.H.|._.t.|.|.
-00000680: 7c02 8303 7c00 5f06 7c00 5300 7208 0000  |...|._.|.S.r...
-00000690: 0029 0772 1b00 0000 721c 0000 0072 0600  .).r....r....r..
-000006a0: 0000 7203 0000 0072 0a00 0000 7204 0000  ..r....r....r...
-000006b0: 0072 0b00 0000 2905 720e 0000 0072 1700  .r....).r....r..
-000006c0: 0000 7218 0000 0072 0c00 0000 5a07 6469  ..r....r....Z.di
-000006d0: 645f 6b65 7972 0f00 0000 720f 0000 0072  d_keyr....r....r
-000006e0: 1000 0000 721e 0000 0031 0000 0073 0e00  ....r....1...s..
-000006f0: 0000 0280 0806 0801 0801 1402 0e02 0402  ................
-00000700: 7a36 4175 7468 6f72 697a 6174 696f 6e57  z6AuthorizationW
-00000710: 7261 7070 6572 2e77 6974 685f 686f 7374  rapper.with_host
-00000720: 5f61 6e64 5f65 6432 3535 3139 5f70 7269  _and_ed25519_pri
-00000730: 7661 7465 5f6b 6579 720a 0000 0063 0200  vate_keyr....c..
-00000740: 0000 0000 0000 0000 0000 0200 0000 0200  ................
-00000750: 0000 4300 0000 730a 0000 007c 017c 005f  ..C...s....|.|._
-00000760: 007c 0053 0072 0800 0000 2901 720a 0000  .|.S.r....).r...
-00000770: 0029 0272 0e00 0000 720a 0000 0072 0f00  .).r....r....r..
-00000780: 0000 720f 0000 0072 1000 0000 da0d 7769  ..r....r......wi
-00000790: 7468 5f61 6374 6f72 5f69 6441 0000 0073  th_actor_idA...s
-000007a0: 0400 0000 0601 0401 7a22 4175 7468 6f72  ........z"Author
-000007b0: 697a 6174 696f 6e57 7261 7070 6572 2e77  izationWrapper.w
-000007c0: 6974 685f 6163 746f 725f 6964 721a 0000  ith_actor_idr...
-000007d0: 0063 0400 0000 0000 0000 0000 0000 0400  .c..............
-000007e0: 0000 0400 0000 4300 0000 7322 0000 007c  ......C...s"...|
-000007f0: 0364 0075 0072 0874 00a0 01a1 007d 0374  .d.u.r.t.....}.t
-00000800: 027c 037c 017c 0283 037c 005f 037c 0053  .|.|.|...|._.|.S
-00000810: 0072 0800 0000 2904 721b 0000 0072 1c00  .r....).r....r..
-00000820: 0000 7205 0000 0072 0b00 0000 2904 720e  ..r....r....).r.
-00000830: 0000 0072 1a00 0000 7218 0000 0072 0c00  ...r....r....r..
-00000840: 0000 720f 0000 0072 0f00 0000 7210 0000  ..r....r....r...
-00000850: 0072 2000 0000 4500 0000 7308 0000 0008  .r ...E...s.....
-00000860: 0608 010e 0204 027a 2841 7574 686f 7269  .......z(Authori
-00000870: 7a61 7469 6f6e 5772 6170 7065 722e 7769  zationWrapper.wi
-00000880: 7468 5f68 7474 705f 7369 676e 6174 7572  th_http_signatur
-00000890: 6563 0100 0000 0000 0000 0000 0000 0100  ec..............
-000008a0: 0000 0400 0000 4300 0000 730e 0000 007c  ......C...s....|
-000008b0: 00a0 0067 0064 01a2 01a1 0153 0029 024e  ...g.d.....S.).N
-000008c0: 2903 7219 0000 0072 1a00 0000 7218 0000  ).r....r....r...
-000008d0: 00a9 01da 095f 6861 735f 6b65 7973 720d  ....._has_keysr.
-000008e0: 0000 0072 0f00 0000 720f 0000 0072 1000  ...r....r....r..
-000008f0: 0000 721f 0000 0052 0000 00f3 0200 0000  ..r....R........
-00000900: 0e01 7a28 4175 7468 6f72 697a 6174 696f  ..z(Authorizatio
-00000910: 6e57 7261 7070 6572 2e5f 6861 735f 6874  nWrapper._has_ht
-00000920: 7470 5f73 6967 6e61 7475 7265 6301 0000  tp_signaturec...
-00000930: 0000 0000 0000 0000 0001 0000 0004 0000  ................
-00000940: 0043 0000 0073 0e00 0000 7c00 a000 6401  .C...s....|...d.
-00000950: 6402 6702 a101 5300 2903 4e72 1700 0000  d.g...S.).Nr....
-00000960: 7218 0000 0072 2300 0000 720d 0000 0072  r....r#...r....r
-00000970: 0f00 0000 720f 0000 0072 1000 0000 721d  ....r....r....r.
-00000980: 0000 0055 0000 0072 2500 0000 7a22 4175  ...U...r%...z"Au
-00000990: 7468 6f72 697a 6174 696f 6e57 7261 7070  thorizationWrapp
-000009a0: 6572 2e5f 6861 735f 6d6f 6f5f 6175 7468  er._has_moo_auth
-000009b0: da08 6b65 795f 6c69 7374 6302 0000 0000  ..key_listc.....
-000009c0: 0000 0000 0000 0003 0000 0003 0000 0043  ...............C
-000009d0: 0000 0073 1e00 0000 7c01 4400 5d0a 7d02  ...s....|.D.].}.
-000009e0: 7c02 7c00 6a00 7601 720c 0100 6401 5300  |.|.j.v.r...d.S.
-000009f0: 7102 6402 5300 2903 4e46 5429 0172 0900  q.d.S.).NFT).r..
-00000a00: 0000 2903 720e 0000 0072 2600 0000 da03  ..).r....r&.....
-00000a10: 6b65 7972 0f00 0000 720f 0000 0072 1000  keyr....r....r..
-00000a20: 0000 7224 0000 0058 0000 0073 0a00 0000  ..r$...X...s....
-00000a30: 0801 0a01 0601 02ff 0403 7a1e 4175 7468  ..........z.Auth
-00000a40: 6f72 697a 6174 696f 6e57 7261 7070 6572  orizationWrapper
-00000a50: 2e5f 6861 735f 6b65 7973 7208 0000 0029  ._has_keysr....)
-00000a60: 12da 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
-00000a70: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
-00000a80: 616d 655f 5f72 1100 0000 7213 0000 0072  ame__r....r....r
-00000a90: 1600 0000 7202 0000 0072 1b00 0000 721c  ....r....r....r.
-00000aa0: 0000 0072 1200 0000 da03 7374 7272 1e00  ...r......strr..
-00000ab0: 0000 7222 0000 0072 2000 0000 721f 0000  ..r"...r ...r...
-00000ac0: 0072 1d00 0000 da04 6c69 7374 7224 0000  .r......listr$..
-00000ad0: 0072 0f00 0000 720f 0000 0072 0f00 0000  .r....r....r....
-00000ae0: 7210 0000 0072 0700 0000 0e00 0000 7332  r....r........s2
-00000af0: 0000 0008 0008 0108 0608 0416 0302 1904  ................
-00000b00: fc02 0202 fe02 0302 fd08 040a fc0e 1002  ................
-00000b10: 0804 fc02 0202 fe02 0302 fd08 040a fc08  ................
-00000b20: 0d08 0312 0372 0700 0000 2910 da07 6c6f  .....r....)...lo
-00000b30: 6767 696e 67da 0674 7970 696e 6772 0200  gging..typingr..
-00000b40: 0000 721b 0000 005a 0e62 6f76 696e 652e  ..r....Z.bovine.
-00000b50: 636c 6965 6e74 7372 0300 0000 5a1e 626f  clientsr....Z.bo
-00000b60: 7669 6e65 2e63 6c69 656e 7473 2e6d 6f6f  vine.clients.moo
-00000b70: 5f61 7574 685f 636c 6965 6e74 7204 0000  _auth_clientr...
-00000b80: 005a 2162 6f76 696e 652e 636c 6965 6e74  .Z!bovine.client
-00000b90: 732e 7369 676e 6564 5f68 7474 705f 636c  s.signed_http_cl
-00000ba0: 6965 6e74 7205 0000 005a 0d62 6f76 696e  ientr....Z.bovin
-00000bb0: 652e 6372 7970 746f 7206 0000 00da 0967  e.cryptor......g
-00000bc0: 6574 4c6f 6767 6572 7228 0000 00da 066c  etLoggerr(.....l
-00000bd0: 6f67 6765 7272 0700 0000 720f 0000 0072  oggerr....r....r
-00000be0: 0f00 0000 720f 0000 0072 1000 0000 da08  ....r....r......
-00000bf0: 3c6d 6f64 756c 653e 0100 0000 7312 0000  <module>....s...
-00000c00: 0008 000c 0108 020c 020c 010c 010c 010a  ................
-00000c10: 0212 03                                  ...
+00000270: 672f 626f 7669 6e65 2f62 6f76 696e 652f  g/bovine/bovine/
+00000280: 626f 7669 6e65 2f62 6f76 696e 652f 6163  bovine/bovine/ac
+00000290: 7469 7669 7479 7075 622f 6175 7468 6f72  tivitypub/author
+000002a0: 697a 6174 696f 6e5f 7772 6170 7065 722e  ization_wrapper.
+000002b0: 7079 da08 5f5f 696e 6974 5f5f 0f00 0000  py..__init__....
+000002c0: 7308 0000 0006 0106 0106 010a 017a 1d41  s............z.A
+000002d0: 7574 686f 7269 7a61 7469 6f6e 5772 6170  uthorizationWrap
+000002e0: 7065 722e 5f5f 696e 6974 5f5f 6301 0000  per.__init__c...
+000002f0: 0000 0000 0000 0000 0001 0000 0002 0000  ................
+00000300: 00c3 0000 0073 1400 0000 8101 7c00 a000  .....s......|...
+00000310: a100 4900 6400 4800 0100 7c00 5300 7208  ..I.d.H...|.S.r.
+00000320: 0000 0029 01da 0469 6e69 7472 0d00 0000  ...)...initr....
+00000330: 720f 0000 0072 0f00 0000 7210 0000 00da  r....r....r.....
+00000340: 0a5f 5f61 656e 7465 725f 5f15 0000 0073  .__aenter__....s
+00000350: 0600 0000 0280 0e01 0401 7a1f 4175 7468  ..........z.Auth
+00000360: 6f72 697a 6174 696f 6e57 7261 7070 6572  orizationWrapper
+00000370: 2e5f 5f61 656e 7465 725f 5f63 0100 0000  .__aenter__c....
+00000380: 0000 0000 0000 0000 0200 0000 0200 0000  ................
+00000390: c700 0000 7316 0000 0081 017c 006a 00a0  ....s......|.j..
+000003a0: 01a1 0049 0064 0048 0001 0064 0053 0072  ...I.d.H...d.S.r
+000003b0: 0800 0000 2902 720c 0000 00da 0563 6c6f  ....).r......clo
+000003c0: 7365 2902 720e 0000 00da 0461 7267 7372  se).r......argsr
+000003d0: 0f00 0000 720f 0000 0072 1000 0000 da09  ....r....r......
+000003e0: 5f5f 6165 7869 745f 5f19 0000 0073 0400  __aexit__....s..
+000003f0: 0000 0280 1401 7a1e 4175 7468 6f72 697a  ......z.Authoriz
+00000400: 6174 696f 6e57 7261 7070 6572 2e5f 5f61  ationWrapper.__a
+00000410: 6578 6974 5f5f 4e72 0c00 0000 6302 0000  exit__Nr....c...
+00000420: 0000 0000 0000 0000 0002 0000 0005 0000  ................
+00000430: 00c3 0000 0073 9200 0000 8101 7c01 7c00  .....s......|.|.
+00000440: 5f00 7c01 6400 7500 720d 7401 a002 a100  _.|.d.u.r.t.....
+00000450: 7c00 5f00 7c00 6a03 7312 4a00 8201 7c00  |._.|.j.s.J...|.
+00000460: a004 a100 722a 7c00 6a05 7c00 6a03 6401  ....r*|.j.|.j.d.
+00000470: 1900 7c00 6a03 6402 1900 7c00 6a00 6403  ..|.j.d...|.j.d.
+00000480: 8d03 4900 6400 4800 0100 6400 5300 7c00  ..I.d.H...d.S.|.
+00000490: a006 a100 7245 7c00 6a03 6404 1900 7c00  ....rE|.j.d...|.
+000004a0: 5f07 7c00 6a08 7c00 6a03 6405 1900 7c00  _.|.j.|.j.d...|.
+000004b0: 6a03 6402 1900 7c00 6a00 6403 8d03 0100  j.d...|.j.d.....
+000004c0: 6400 5300 7409 6406 8301 8201 2907 4eda  d.S.t.d.....).N.
+000004d0: 0468 6f73 74da 0b70 7269 7661 7465 5f6b  .host..private_k
+000004e0: 6579 2901 720c 0000 00da 0b61 6363 6f75  ey).r......accou
+000004f0: 6e74 5f75 726c da0e 7075 626c 6963 5f6b  nt_url..public_k
+00000500: 6579 5f75 726c 7a27 4e6f 206b 6e6f 776e  ey_urlz'No known
+00000510: 2061 7574 686f 7269 7a61 7469 6f6e 206d   authorization m
+00000520: 6574 686f 6420 6176 6169 6c61 626c 6529  ethod available)
+00000530: 0a72 0c00 0000 da07 6169 6f68 7474 70da  .r......aiohttp.
+00000540: 0d43 6c69 656e 7453 6573 7369 6f6e 7209  .ClientSessionr.
+00000550: 0000 00da 0d5f 6861 735f 6d6f 6f5f 6175  ....._has_moo_au
+00000560: 7468 da21 7769 7468 5f68 6f73 745f 616e  th.!with_host_an
+00000570: 645f 6564 3235 3531 395f 7072 6976 6174  d_ed25519_privat
+00000580: 655f 6b65 79da 135f 6861 735f 6874 7470  e_key.._has_http
+00000590: 5f73 6967 6e61 7475 7265 720a 0000 00da  _signaturer.....
+000005a0: 1377 6974 685f 6874 7470 5f73 6967 6e61  .with_http_signa
+000005b0: 7475 7265 da09 4578 6365 7074 696f 6e29  ture..Exception)
+000005c0: 0272 0e00 0000 720c 0000 0072 0f00 0000  .r....r....r....
+000005d0: 720f 0000 0072 1000 0000 7212 0000 001c  r....r....r.....
+000005e0: 0000 0073 2200 0000 0280 0601 0801 0a01  ...s"...........
+000005f0: 0a02 0802 0401 1401 10ff 0803 0c01 0401  ................
+00000600: 0801 0801 0401 0afd 0806 7a19 4175 7468  ..........z.Auth
+00000610: 6f72 697a 6174 696f 6e57 7261 7070 6572  orizationWrapper
+00000620: 2e69 6e69 7472 1700 0000 7218 0000 0063  .initr....r....c
+00000630: 0400 0000 0000 0000 0000 0000 0500 0000  ................
+00000640: 0400 0000 c300 0000 7340 0000 0081 017c  ........s@.....|
+00000650: 0364 0075 0072 0974 00a0 01a1 007d 0374  .d.u.r.t.....}.t
+00000660: 027c 0283 017d 0474 037c 037c 017c 0483  .|...}.t.|.|.|..
+00000670: 0349 0064 0048 007c 005f 0474 057c 037c  .I.d.H.|._.t.|.|
+00000680: 047c 0283 037c 005f 067c 0053 0072 0800  .|...|._.|.S.r..
+00000690: 0000 2907 721b 0000 0072 1c00 0000 7206  ..).r....r....r.
+000006a0: 0000 0072 0300 0000 720a 0000 0072 0400  ...r....r....r..
+000006b0: 0000 720b 0000 0029 0572 0e00 0000 7217  ..r....).r....r.
+000006c0: 0000 0072 1800 0000 720c 0000 005a 0764  ...r....r....Z.d
+000006d0: 6964 5f6b 6579 720f 0000 0072 0f00 0000  id_keyr....r....
+000006e0: 7210 0000 0072 1e00 0000 3100 0000 730e  r....r....1...s.
+000006f0: 0000 0002 8008 0608 0108 0114 020e 0204  ................
+00000700: 027a 3641 7574 686f 7269 7a61 7469 6f6e  .z6Authorization
+00000710: 5772 6170 7065 722e 7769 7468 5f68 6f73  Wrapper.with_hos
+00000720: 745f 616e 645f 6564 3235 3531 395f 7072  t_and_ed25519_pr
+00000730: 6976 6174 655f 6b65 7972 0a00 0000 6302  ivate_keyr....c.
+00000740: 0000 0000 0000 0000 0000 0002 0000 0002  ................
+00000750: 0000 0043 0000 0073 0a00 0000 7c01 7c00  ...C...s....|.|.
+00000760: 5f00 7c00 5300 7208 0000 0029 0172 0a00  _.|.S.r....).r..
+00000770: 0000 2902 720e 0000 0072 0a00 0000 720f  ..).r....r....r.
+00000780: 0000 0072 0f00 0000 7210 0000 00da 0d77  ...r....r......w
+00000790: 6974 685f 6163 746f 725f 6964 4100 0000  ith_actor_idA...
+000007a0: 7304 0000 0006 0104 017a 2241 7574 686f  s........z"Autho
+000007b0: 7269 7a61 7469 6f6e 5772 6170 7065 722e  rizationWrapper.
+000007c0: 7769 7468 5f61 6374 6f72 5f69 6472 1a00  with_actor_idr..
+000007d0: 0000 6304 0000 0000 0000 0000 0000 0004  ..c.............
+000007e0: 0000 0004 0000 0043 0000 0073 2200 0000  .......C...s"...
+000007f0: 7c03 6400 7500 7208 7400 a001 a100 7d03  |.d.u.r.t.....}.
+00000800: 7402 7c03 7c01 7c02 8303 7c00 5f03 7c00  t.|.|.|...|._.|.
+00000810: 5300 7208 0000 0029 0472 1b00 0000 721c  S.r....).r....r.
+00000820: 0000 0072 0500 0000 720b 0000 0029 0472  ...r....r....).r
+00000830: 0e00 0000 721a 0000 0072 1800 0000 720c  ....r....r....r.
+00000840: 0000 0072 0f00 0000 720f 0000 0072 1000  ...r....r....r..
+00000850: 0000 7220 0000 0045 0000 0073 0800 0000  ..r ...E...s....
+00000860: 0806 0801 0e02 0402 7a28 4175 7468 6f72  ........z(Author
+00000870: 697a 6174 696f 6e57 7261 7070 6572 2e77  izationWrapper.w
+00000880: 6974 685f 6874 7470 5f73 6967 6e61 7475  ith_http_signatu
+00000890: 7265 6301 0000 0000 0000 0000 0000 0001  rec.............
+000008a0: 0000 0004 0000 0043 0000 0073 0e00 0000  .......C...s....
+000008b0: 7c00 a000 6700 6401 a201 a101 5300 2902  |...g.d.....S.).
+000008c0: 4e29 0372 1900 0000 721a 0000 0072 1800  N).r....r....r..
+000008d0: 0000 a901 da09 5f68 6173 5f6b 6579 7372  ......_has_keysr
+000008e0: 0d00 0000 720f 0000 0072 0f00 0000 7210  ....r....r....r.
+000008f0: 0000 0072 1f00 0000 5200 0000 f302 0000  ...r....R.......
+00000900: 000e 017a 2841 7574 686f 7269 7a61 7469  ...z(Authorizati
+00000910: 6f6e 5772 6170 7065 722e 5f68 6173 5f68  onWrapper._has_h
+00000920: 7474 705f 7369 676e 6174 7572 6563 0100  ttp_signaturec..
+00000930: 0000 0000 0000 0000 0000 0100 0000 0400  ................
+00000940: 0000 4300 0000 730e 0000 007c 00a0 0064  ..C...s....|...d
+00000950: 0164 0267 02a1 0153 0029 034e 7217 0000  .d.g...S.).Nr...
+00000960: 0072 1800 0000 7223 0000 0072 0d00 0000  .r....r#...r....
+00000970: 720f 0000 0072 0f00 0000 7210 0000 0072  r....r....r....r
+00000980: 1d00 0000 5500 0000 7225 0000 007a 2241  ....U...r%...z"A
+00000990: 7574 686f 7269 7a61 7469 6f6e 5772 6170  uthorizationWrap
+000009a0: 7065 722e 5f68 6173 5f6d 6f6f 5f61 7574  per._has_moo_aut
+000009b0: 68da 086b 6579 5f6c 6973 7463 0200 0000  h..key_listc....
+000009c0: 0000 0000 0000 0000 0300 0000 0300 0000  ................
+000009d0: 4300 0000 731e 0000 007c 0144 005d 0a7d  C...s....|.D.].}
+000009e0: 027c 027c 006a 0076 0172 0c01 0064 0153  .|.|.j.v.r...d.S
+000009f0: 0071 0264 0253 0029 034e 4654 2901 7209  .q.d.S.).NFT).r.
+00000a00: 0000 0029 0372 0e00 0000 7226 0000 00da  ...).r....r&....
+00000a10: 036b 6579 720f 0000 0072 0f00 0000 7210  .keyr....r....r.
+00000a20: 0000 0072 2400 0000 5800 0000 730a 0000  ...r$...X...s...
+00000a30: 0008 010a 0106 0102 ff04 037a 1e41 7574  ...........z.Aut
+00000a40: 686f 7269 7a61 7469 6f6e 5772 6170 7065  horizationWrappe
+00000a50: 722e 5f68 6173 5f6b 6579 7372 0800 0000  r._has_keysr....
+00000a60: 2912 da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
+00000a70: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
+00000a80: 6e61 6d65 5f5f 7211 0000 0072 1300 0000  name__r....r....
+00000a90: 7216 0000 0072 0200 0000 721b 0000 0072  r....r....r....r
+00000aa0: 1c00 0000 7212 0000 00da 0373 7472 721e  ....r......strr.
+00000ab0: 0000 0072 2200 0000 7220 0000 0072 1f00  ...r"...r ...r..
+00000ac0: 0000 721d 0000 00da 046c 6973 7472 2400  ..r......listr$.
+00000ad0: 0000 720f 0000 0072 0f00 0000 720f 0000  ..r....r....r...
+00000ae0: 0072 1000 0000 7207 0000 000e 0000 0073  .r....r........s
+00000af0: 3200 0000 0800 0801 0806 0804 1603 0219  2...............
+00000b00: 04fc 0202 02fe 0203 02fd 0804 0afc 0e10  ................
+00000b10: 0208 04fc 0202 02fe 0203 02fd 0804 0afc  ................
+00000b20: 080d 0803 1203 7207 0000 0029 10da 076c  ......r....)...l
+00000b30: 6f67 6769 6e67 da06 7479 7069 6e67 7202  ogging..typingr.
+00000b40: 0000 0072 1b00 0000 5a0e 626f 7669 6e65  ...r....Z.bovine
+00000b50: 2e63 6c69 656e 7473 7203 0000 005a 1e62  .clientsr....Z.b
+00000b60: 6f76 696e 652e 636c 6965 6e74 732e 6d6f  ovine.clients.mo
+00000b70: 6f5f 6175 7468 5f63 6c69 656e 7472 0400  o_auth_clientr..
+00000b80: 0000 5a21 626f 7669 6e65 2e63 6c69 656e  ..Z!bovine.clien
+00000b90: 7473 2e73 6967 6e65 645f 6874 7470 5f63  ts.signed_http_c
+00000ba0: 6c69 656e 7472 0500 0000 5a0d 626f 7669  lientr....Z.bovi
+00000bb0: 6e65 2e63 7279 7074 6f72 0600 0000 da09  ne.cryptor......
+00000bc0: 6765 744c 6f67 6765 7272 2800 0000 da06  getLoggerr(.....
+00000bd0: 6c6f 6767 6572 7207 0000 0072 0f00 0000  loggerr....r....
+00000be0: 720f 0000 0072 0f00 0000 7210 0000 00da  r....r....r.....
+00000bf0: 083c 6d6f 6475 6c65 3e01 0000 0073 1200  .<module>....s..
+00000c00: 0000 0800 0c01 0802 0c02 0c01 0c01 0c01  ................
+00000c10: 0a02 1203                                ....
```

### Comparing `bovine-0.1.0/bovine/activitypub/__pycache__/collection_helper.cpython-310.pyc` & `bovine-0.1.1/bovine/activitypub/__pycache__/collection_helper.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 13 15:55:57 2023 UTC, .py size: 2219 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0d26 3864 ab08 0000  o........&8d....
+00000000: 6f0d 0d0a 0000 0000 a4ea 3a64 ab08 0000  o.........:d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 3a00 0000 6400  .....@...s:...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6403 6404 6c03 6d04 5a04 0100 6405  ..d.d.l.m.Z...d.
 00000050: 6406 8400 5a05 4700 6407 6408 8400 6408  d...Z.G.d.d...d.
 00000060: 8302 5a06 6401 5300 2909 e900 0000 004e  ..Z.d.S.)......N
 00000070: 2901 da0e 7072 696e 745f 6163 7469 7669  )...print_activi
@@ -17,139 +17,139 @@
 00000100: 0029 064e da06 6f62 6a65 6374 2904 da04  .).N..object)...
 00000110: 6e61 6d65 da07 7375 6d6d 6172 79da 0763  name..summary..c
 00000120: 6f6e 7465 6e74 da02 6964 5429 02da 0474  ontent..idT)...t
 00000130: 6167 73da 0573 7472 6970 7a10 2d2d 2d20  ags..stripz.--- 
 00000140: 756e 6b6e 6f77 6e20 202d 2d2d 2902 da06  unknown  ---)...
 00000150: 626c 6561 6368 da05 636c 6561 6e29 02da  bleach..clean)..
 00000160: 036f 626a da03 6b65 79a9 0072 1100 0000  .obj..key..r....
-00000170: fa58 2f77 6f6f 6470 6563 6b65 722f 7372  .X/woodpecker/sr
-00000180: 632f 636f 6465 6265 7267 2e6f 7267 2f68  c/codeberg.org/h
-00000190: 656c 6765 2f62 6f76 696e 652f 626f 7669  elge/bovine/bovi
-000001a0: 6e65 2f62 6f76 696e 652f 6163 7469 7669  ne/bovine/activi
-000001b0: 7479 7075 622f 636f 6c6c 6563 7469 6f6e  typub/collection
-000001c0: 5f68 656c 7065 722e 7079 da17 7368 6f72  _helper.py..shor
-000001d0: 745f 7665 7273 696f 6e5f 6f66 5f6f 626a  t_version_of_obj
-000001e0: 6563 7408 0000 0073 0e00 0000 0801 0801  ect....s........
-000001f0: 0802 1001 1801 0280 0402 7213 0000 0063  ..........r....c
-00000200: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000210: 0300 0000 4000 0000 7340 0000 0065 005a  ....@...s@...e.Z
-00000220: 0164 005a 0264 0164 0284 005a 0364 0364  .d.Z.d.d...Z.d.d
-00000230: 0484 005a 0464 0564 0684 005a 0564 0764  ...Z.d.d...Z.d.d
-00000240: 0884 005a 0664 1064 0a64 0b84 015a 0764  ...Z.d.d.d...Z.d
-00000250: 1164 0d64 0e84 015a 0864 0f53 0029 12da  .d.d...Z.d.S.)..
-00000260: 1043 6f6c 6c65 6374 696f 6e48 656c 7065  .CollectionHelpe
-00000270: 7263 0300 0000 0000 0000 0000 0000 0300  rc..............
-00000280: 0000 0200 0000 4300 0000 732e 0000 007c  ......C...s....|
-00000290: 017c 005f 007c 027c 005f 0164 007c 005f  .|._.|.|._.d.|._
-000002a0: 0264 007c 005f 0364 007c 005f 0464 007c  .d.|._.d.|._.d.|
-000002b0: 005f 0569 007c 005f 0664 0053 00a9 014e  ._.i.|._.d.S...N
-000002c0: 2907 da0d 636f 6c6c 6563 7469 6f6e 5f69  )...collection_i
-000002d0: 64da 0561 6374 6f72 da11 6261 7369 635f  d..actor..basic_
-000002e0: 696e 666f 726d 6174 696f 6eda 0569 7465  information..ite
-000002f0: 6d73 da0a 6e65 7874 5f69 7465 6d73 da0a  ms..next_items..
-00000300: 6974 656d 5f69 6e64 6578 da0d 656c 656d  item_index..elem
-00000310: 656e 745f 6361 6368 6529 03da 0473 656c  ent_cache)...sel
-00000320: 6672 1600 0000 7217 0000 0072 1100 0000  fr....r....r....
-00000330: 7211 0000 0072 1200 0000 da08 5f5f 696e  r....r......__in
-00000340: 6974 5f5f 1400 0000 730e 0000 0006 0106  it__....s.......
-00000350: 0106 0206 0106 0106 010a 027a 1943 6f6c  ...........z.Col
-00000360: 6c65 6374 696f 6e48 656c 7065 722e 5f5f  lectionHelper.__
-00000370: 696e 6974 5f5f 6301 0000 0000 0000 0000  init__c.........
-00000380: 0000 0002 0000 0004 0000 00c3 0000 0073  ...............s
-00000390: 5800 0000 8101 7c00 6a00 6400 7500 7211  X.....|.j.d.u.r.
-000003a0: 7c00 6a01 a002 7c00 6a03 a101 4900 6400  |.j...|.j...I.d.
-000003b0: 4800 7c00 5f00 7c00 6a01 a002 7c00 6a00  H.|._.|.j...|.j.
-000003c0: 6401 1900 a101 4900 6400 4800 7d01 7c01  d.....I.d.H.}.|.
-000003d0: 6402 1900 7c00 5f04 7c01 6403 1900 7c00  d...|._.|.d...|.
-000003e0: 5f05 6404 7c00 5f06 6400 5300 2905 4eda  _.d.|._.d.S.).N.
-000003f0: 0566 6972 7374 da0c 6f72 6465 7265 6449  .first..orderedI
-00000400: 7465 6d73 da04 6e65 7874 7201 0000 0029  tems..nextr....)
-00000410: 0772 1800 0000 7217 0000 00da 0367 6574  .r....r......get
-00000420: 7216 0000 0072 1900 0000 721a 0000 0072  r....r....r....r
-00000430: 1b00 0000 2902 721d 0000 00da 0872 6573  ....).r......res
-00000440: 706f 6e73 6572 1100 0000 7211 0000 0072  ponser....r....r
-00000450: 1200 0000 da07 7265 6672 6573 681f 0000  ......refresh...
-00000460: 0073 0e00 0000 0280 0a01 1601 1802 0a02  .s..............
-00000470: 0a01 0a01 7a18 436f 6c6c 6563 7469 6f6e  ....z.Collection
-00000480: 4865 6c70 6572 2e72 6566 7265 7368 6301  Helper.refreshc.
-00000490: 0000 0000 0000 0000 0000 0004 0000 0009  ................
-000004a0: 0000 00c3 0000 0073 7800 0000 8101 7400  .......sx.....t.
-000004b0: 8300 0100 7400 6401 7401 7c00 6a02 8301  ....t.d.t.|.j...
-000004c0: 9b00 9d02 8301 0100 7400 8300 0100 7403  ........t.....t.
-000004d0: 7c00 6a02 8301 4400 5d23 5c02 7d01 7d02  |.j...D.]#\.}.}.
-000004e0: 7c00 a004 7c02 a101 4900 6400 4800 7d03  |...|...I.d.H.}.
-000004f0: 7400 7c01 6402 9b04 6403 7c03 a005 6404  t.|.d...d.|...d.
-00000500: a101 6405 9b04 6403 7406 7c03 8301 6400  ..d...d.t.|...d.
-00000510: 6406 8502 1900 9b00 9d05 8301 0100 7116  d.............q.
-00000520: 6400 5300 2907 4e7a 0d49 7465 6d73 206c  d.S.).Nz.Items l
-00000530: 6f61 6465 6420 da01 347a 023a 20da 0474  oaded ..4z.: ..t
-00000540: 7970 65da 0231 30e9 5000 0000 2907 da05  ype..10.P...)...
-00000550: 7072 696e 74da 036c 656e 7219 0000 00da  print..lenr.....
-00000560: 0965 6e75 6d65 7261 7465 da0b 6765 745f  .enumerate..get_
-00000570: 656c 656d 656e 7472 2200 0000 7213 0000  elementr"...r...
-00000580: 0029 0472 1d00 0000 da03 6964 78da 0469  .).r......idx..i
-00000590: 7465 6d72 0f00 0000 7211 0000 0072 1100  temr....r....r..
-000005a0: 0000 7212 0000 0072 0800 0000 2900 0000  ..r....r....)...
-000005b0: 7310 0000 0002 8006 0114 0106 0112 0110  s...............
-000005c0: 0130 0104 fe7a 1843 6f6c 6c65 6374 696f  .0...z.Collectio
-000005d0: 6e48 656c 7065 722e 7375 6d6d 6172 7963  nHelper.summaryc
-000005e0: 0200 0000 0000 0000 0000 0000 0300 0000  ................
-000005f0: 0300 0000 c300 0000 7344 0000 0081 0174  ........sD.....t
-00000600: 007c 0174 0183 0273 087c 0153 007c 017c  .|.t...s.|.S.|.|
-00000610: 006a 0276 0072 127c 006a 027c 0119 0053  .j.v.r.|.j.|...S
-00000620: 007c 006a 03a0 047c 01a1 0149 0064 0048  .|.j...|...I.d.H
-00000630: 007d 027c 027c 006a 027c 013c 007c 0253  .}.|.|.j.|.<.|.S
-00000640: 0072 1500 0000 2905 da0a 6973 696e 7374  .r....)...isinst
-00000650: 616e 6365 da03 7374 7272 1c00 0000 7217  ance..strr....r.
-00000660: 0000 00da 0d70 726f 7879 5f65 6c65 6d65  .....proxy_eleme
-00000670: 6e74 2903 721d 0000 00da 0765 6c65 6d65  nt).r......eleme
-00000680: 6e74 da06 7265 7375 6c74 7211 0000 0072  nt..resultr....r
-00000690: 1100 0000 7212 0000 0072 2c00 0000 3100  ....r....r,...1.
-000006a0: 0000 7310 0000 0002 800a 0104 010a 020a  ..s.............
-000006b0: 0112 020a 0204 027a 1c43 6f6c 6c65 6374  .......z.Collect
-000006c0: 696f 6e48 656c 7065 722e 6765 745f 656c  ionHelper.get_el
-000006d0: 656d 656e 7446 6302 0000 0000 0000 0000  ementFc.........
-000006e0: 0000 0004 0000 0004 0000 00c3 0000 0073  ...............s
-000006f0: 7c00 0000 8101 7c00 6a00 7401 7c00 6a02  |.....|.j.t.|.j.
-00000700: 8301 6b05 7221 7c00 6a03 a004 7c00 6a05  ..k.r!|.j...|.j.
-00000710: a101 4900 6400 4800 7d02 7c00 0400 6a02  ..I.d.H.}.|...j.
-00000720: 7c02 6401 1900 3700 0200 5f02 7c02 6402  |.d...7..._.|.d.
-00000730: 1900 7c00 5f05 7c00 6a02 7c00 6a00 1900  ..|._.|.j.|.j...
-00000740: 7d03 7c00 0400 6a00 6403 3700 0200 5f00  }.|...j.d.7..._.
-00000750: 7c00 a006 7c03 a101 4900 6400 4800 7d03  |...|...I.d.H.}.
-00000760: 7c01 723c 7407 7c03 8301 0100 7c03 5300  |.r<t.|.....|.S.
-00000770: 2904 4e72 2000 0000 7221 0000 0072 0300  ).Nr ...r!...r..
-00000780: 0000 2908 721b 0000 0072 2a00 0000 7219  ..).r....r*...r.
-00000790: 0000 0072 1700 0000 7222 0000 0072 1a00  ...r....r"...r..
-000007a0: 0000 722c 0000 0072 0200 0000 2904 721d  ..r,...r....).r.
-000007b0: 0000 005a 0864 6f5f 7072 696e 7472 2300  ...Z.do_printr#.
-000007c0: 0000 7233 0000 0072 1100 0000 7211 0000  ..r3...r....r...
-000007d0: 0072 1200 0000 da09 6e65 7874 5f69 7465  .r......next_ite
-000007e0: 6d3e 0000 0073 1600 0000 0280 1001 1401  m>...s..........
-000007f0: 1201 0a01 0c02 0e01 1002 0402 0801 0402  ................
-00000800: 7a1a 436f 6c6c 6563 7469 6f6e 4865 6c70  z.CollectionHelp
-00000810: 6572 2e6e 6578 745f 6974 656d e90a 0000  er.next_item....
-00000820: 0063 0200 0000 0000 0000 0000 0000 0200  .c..............
-00000830: 0000 0300 0000 4300 0000 730a 0000 0074  ......C...s....t
-00000840: 007c 007c 0183 0253 0072 1500 0000 7204  .|.|...S.r....r.
-00000850: 0000 0029 0272 1d00 0000 5a0a 6d61 785f  ...).r....Z.max_
-00000860: 6e75 6d62 6572 7211 0000 0072 1100 0000  numberr....r....
-00000870: 7212 0000 00da 0769 7465 7261 7465 4e00  r......iterateN.
-00000880: 0000 7302 0000 000a 017a 1843 6f6c 6c65  ..s......z.Colle
-00000890: 6374 696f 6e48 656c 7065 722e 6974 6572  ctionHelper.iter
-000008a0: 6174 654e 2901 4629 0172 3500 0000 2909  ateN).F).r5...).
-000008b0: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
-000008c0: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
-000008d0: 6d65 5f5f 721e 0000 0072 2400 0000 7208  me__r....r$...r.
-000008e0: 0000 0072 2c00 0000 7234 0000 0072 3600  ...r,...r4...r6.
-000008f0: 0000 7211 0000 0072 1100 0000 7211 0000  ..r....r....r...
-00000900: 0072 1200 0000 7214 0000 0013 0000 0073  .r....r........s
-00000910: 0e00 0000 0800 0801 080b 080a 0808 0a0d  ................
-00000920: 0e10 7214 0000 0029 0772 0d00 0000 5a22  ..r....).r....Z"
-00000930: 626f 7669 6e65 2e61 6374 6976 6974 7973  bovine.activitys
-00000940: 7472 6561 6d73 2e75 7469 6c73 2e70 7269  treams.utils.pri
-00000950: 6e74 7202 0000 005a 1363 6f6c 6c65 6374  ntr....Z.collect
-00000960: 696f 6e5f 6974 6572 6174 6f72 7205 0000  ion_iteratorr...
-00000970: 0072 1300 0000 7214 0000 0072 1100 0000  .r....r....r....
-00000980: 7211 0000 0072 1100 0000 7212 0000 00da  r....r....r.....
-00000990: 083c 6d6f 6475 6c65 3e01 0000 0073 0a00  .<module>....s..
-000009a0: 0000 0800 0c02 0c02 0803 120b            ............
+00000170: fa59 2f77 6f6f 6470 6563 6b65 722f 7372  .Y/woodpecker/sr
+00000180: 632f 636f 6465 6265 7267 2e6f 7267 2f62  c/codeberg.org/b
+00000190: 6f76 696e 652f 626f 7669 6e65 2f62 6f76  ovine/bovine/bov
+000001a0: 696e 652f 626f 7669 6e65 2f61 6374 6976  ine/bovine/activ
+000001b0: 6974 7970 7562 2f63 6f6c 6c65 6374 696f  itypub/collectio
+000001c0: 6e5f 6865 6c70 6572 2e70 79da 1773 686f  n_helper.py..sho
+000001d0: 7274 5f76 6572 7369 6f6e 5f6f 665f 6f62  rt_version_of_ob
+000001e0: 6a65 6374 0800 0000 730e 0000 0008 0108  ject....s.......
+000001f0: 0108 0210 0118 0102 8004 0272 1300 0000  ...........r....
+00000200: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+00000210: 0003 0000 0040 0000 0073 4000 0000 6500  .....@...s@...e.
+00000220: 5a01 6400 5a02 6401 6402 8400 5a03 6403  Z.d.Z.d.d...Z.d.
+00000230: 6404 8400 5a04 6405 6406 8400 5a05 6407  d...Z.d.d...Z.d.
+00000240: 6408 8400 5a06 6410 640a 640b 8401 5a07  d...Z.d.d.d...Z.
+00000250: 6411 640d 640e 8401 5a08 640f 5300 2912  d.d.d...Z.d.S.).
+00000260: da10 436f 6c6c 6563 7469 6f6e 4865 6c70  ..CollectionHelp
+00000270: 6572 6303 0000 0000 0000 0000 0000 0003  erc.............
+00000280: 0000 0002 0000 0043 0000 0073 2e00 0000  .......C...s....
+00000290: 7c01 7c00 5f00 7c02 7c00 5f01 6400 7c00  |.|._.|.|._.d.|.
+000002a0: 5f02 6400 7c00 5f03 6400 7c00 5f04 6400  _.d.|._.d.|._.d.
+000002b0: 7c00 5f05 6900 7c00 5f06 6400 5300 a901  |._.i.|._.d.S...
+000002c0: 4e29 07da 0d63 6f6c 6c65 6374 696f 6e5f  N)...collection_
+000002d0: 6964 da05 6163 746f 72da 1162 6173 6963  id..actor..basic
+000002e0: 5f69 6e66 6f72 6d61 7469 6f6e da05 6974  _information..it
+000002f0: 656d 73da 0a6e 6578 745f 6974 656d 73da  ems..next_items.
+00000300: 0a69 7465 6d5f 696e 6465 78da 0d65 6c65  .item_index..ele
+00000310: 6d65 6e74 5f63 6163 6865 2903 da04 7365  ment_cache)...se
+00000320: 6c66 7216 0000 0072 1700 0000 7211 0000  lfr....r....r...
+00000330: 0072 1100 0000 7212 0000 00da 085f 5f69  .r....r......__i
+00000340: 6e69 745f 5f14 0000 0073 0e00 0000 0601  nit__....s......
+00000350: 0601 0602 0601 0601 0601 0a02 7a19 436f  ............z.Co
+00000360: 6c6c 6563 7469 6f6e 4865 6c70 6572 2e5f  llectionHelper._
+00000370: 5f69 6e69 745f 5f63 0100 0000 0000 0000  _init__c........
+00000380: 0000 0000 0200 0000 0400 0000 c300 0000  ................
+00000390: 7358 0000 0081 017c 006a 0064 0075 0072  sX.....|.j.d.u.r
+000003a0: 117c 006a 01a0 027c 006a 03a1 0149 0064  .|.j...|.j...I.d
+000003b0: 0048 007c 005f 007c 006a 01a0 027c 006a  .H.|._.|.j...|.j
+000003c0: 0064 0119 00a1 0149 0064 0048 007d 017c  .d.....I.d.H.}.|
+000003d0: 0164 0219 007c 005f 047c 0164 0319 007c  .d...|._.|.d...|
+000003e0: 005f 0564 047c 005f 0664 0053 0029 054e  ._.d.|._.d.S.).N
+000003f0: da05 6669 7273 74da 0c6f 7264 6572 6564  ..first..ordered
+00000400: 4974 656d 73da 046e 6578 7472 0100 0000  Items..nextr....
+00000410: 2907 7218 0000 0072 1700 0000 da03 6765  ).r....r......ge
+00000420: 7472 1600 0000 7219 0000 0072 1a00 0000  tr....r....r....
+00000430: 721b 0000 0029 0272 1d00 0000 da08 7265  r....).r......re
+00000440: 7370 6f6e 7365 7211 0000 0072 1100 0000  sponser....r....
+00000450: 7212 0000 00da 0772 6566 7265 7368 1f00  r......refresh..
+00000460: 0000 730e 0000 0002 800a 0116 0118 020a  ..s.............
+00000470: 020a 010a 017a 1843 6f6c 6c65 6374 696f  .....z.Collectio
+00000480: 6e48 656c 7065 722e 7265 6672 6573 6863  nHelper.refreshc
+00000490: 0100 0000 0000 0000 0000 0000 0400 0000  ................
+000004a0: 0900 0000 c300 0000 7378 0000 0081 0174  ........sx.....t
+000004b0: 0083 0001 0074 0064 0174 017c 006a 0283  .....t.d.t.|.j..
+000004c0: 019b 009d 0283 0101 0074 0083 0001 0074  .........t.....t
+000004d0: 037c 006a 0283 0144 005d 235c 027d 017d  .|.j...D.]#\.}.}
+000004e0: 027c 00a0 047c 02a1 0149 0064 0048 007d  .|...|...I.d.H.}
+000004f0: 0374 007c 0164 029b 0464 037c 03a0 0564  .t.|.d...d.|...d
+00000500: 04a1 0164 059b 0464 0374 067c 0383 0164  ...d...d.t.|...d
+00000510: 0064 0685 0219 009b 009d 0583 0101 0071  .d.............q
+00000520: 1664 0053 0029 074e 7a0d 4974 656d 7320  .d.S.).Nz.Items 
+00000530: 6c6f 6164 6564 20da 0134 7a02 3a20 da04  loaded ..4z.: ..
+00000540: 7479 7065 da02 3130 e950 0000 0029 07da  type..10.P...)..
+00000550: 0570 7269 6e74 da03 6c65 6e72 1900 0000  .print..lenr....
+00000560: da09 656e 756d 6572 6174 65da 0b67 6574  ..enumerate..get
+00000570: 5f65 6c65 6d65 6e74 7222 0000 0072 1300  _elementr"...r..
+00000580: 0000 2904 721d 0000 00da 0369 6478 da04  ..).r......idx..
+00000590: 6974 656d 720f 0000 0072 1100 0000 7211  itemr....r....r.
+000005a0: 0000 0072 1200 0000 7208 0000 0029 0000  ...r....r....)..
+000005b0: 0073 1000 0000 0280 0601 1401 0601 1201  .s..............
+000005c0: 1001 3001 04fe 7a18 436f 6c6c 6563 7469  ..0...z.Collecti
+000005d0: 6f6e 4865 6c70 6572 2e73 756d 6d61 7279  onHelper.summary
+000005e0: 6302 0000 0000 0000 0000 0000 0003 0000  c...............
+000005f0: 0003 0000 00c3 0000 0073 4400 0000 8101  .........sD.....
+00000600: 7400 7c01 7401 8302 7308 7c01 5300 7c01  t.|.t...s.|.S.|.
+00000610: 7c00 6a02 7600 7212 7c00 6a02 7c01 1900  |.j.v.r.|.j.|...
+00000620: 5300 7c00 6a03 a004 7c01 a101 4900 6400  S.|.j...|...I.d.
+00000630: 4800 7d02 7c02 7c00 6a02 7c01 3c00 7c02  H.}.|.|.j.|.<.|.
+00000640: 5300 7215 0000 0029 05da 0a69 7369 6e73  S.r....)...isins
+00000650: 7461 6e63 65da 0373 7472 721c 0000 0072  tance..strr....r
+00000660: 1700 0000 da0d 7072 6f78 795f 656c 656d  ......proxy_elem
+00000670: 656e 7429 0372 1d00 0000 da07 656c 656d  ent).r......elem
+00000680: 656e 74da 0672 6573 756c 7472 1100 0000  ent..resultr....
+00000690: 7211 0000 0072 1200 0000 722c 0000 0031  r....r....r,...1
+000006a0: 0000 0073 1000 0000 0280 0a01 0401 0a02  ...s............
+000006b0: 0a01 1202 0a02 0402 7a1c 436f 6c6c 6563  ........z.Collec
+000006c0: 7469 6f6e 4865 6c70 6572 2e67 6574 5f65  tionHelper.get_e
+000006d0: 6c65 6d65 6e74 4663 0200 0000 0000 0000  lementFc........
+000006e0: 0000 0000 0400 0000 0400 0000 c300 0000  ................
+000006f0: 737c 0000 0081 017c 006a 0074 017c 006a  s|.....|.j.t.|.j
+00000700: 0283 016b 0572 217c 006a 03a0 047c 006a  ...k.r!|.j...|.j
+00000710: 05a1 0149 0064 0048 007d 027c 0004 006a  ...I.d.H.}.|...j
+00000720: 027c 0264 0119 0037 0002 005f 027c 0264  .|.d...7..._.|.d
+00000730: 0219 007c 005f 057c 006a 027c 006a 0019  ...|._.|.j.|.j..
+00000740: 007d 037c 0004 006a 0064 0337 0002 005f  .}.|...j.d.7..._
+00000750: 007c 00a0 067c 03a1 0149 0064 0048 007d  .|...|...I.d.H.}
+00000760: 037c 0172 3c74 077c 0383 0101 007c 0353  .|.r<t.|.....|.S
+00000770: 0029 044e 7220 0000 0072 2100 0000 7203  .).Nr ...r!...r.
+00000780: 0000 0029 0872 1b00 0000 722a 0000 0072  ...).r....r*...r
+00000790: 1900 0000 7217 0000 0072 2200 0000 721a  ....r....r"...r.
+000007a0: 0000 0072 2c00 0000 7202 0000 0029 0472  ...r,...r....).r
+000007b0: 1d00 0000 5a08 646f 5f70 7269 6e74 7223  ....Z.do_printr#
+000007c0: 0000 0072 3300 0000 7211 0000 0072 1100  ...r3...r....r..
+000007d0: 0000 7212 0000 00da 096e 6578 745f 6974  ..r......next_it
+000007e0: 656d 3e00 0000 7316 0000 0002 8010 0114  em>...s.........
+000007f0: 0112 010a 010c 020e 0110 0204 0208 0104  ................
+00000800: 027a 1a43 6f6c 6c65 6374 696f 6e48 656c  .z.CollectionHel
+00000810: 7065 722e 6e65 7874 5f69 7465 6de9 0a00  per.next_item...
+00000820: 0000 6302 0000 0000 0000 0000 0000 0002  ..c.............
+00000830: 0000 0003 0000 0043 0000 0073 0a00 0000  .......C...s....
+00000840: 7400 7c00 7c01 8302 5300 7215 0000 0072  t.|.|...S.r....r
+00000850: 0400 0000 2902 721d 0000 005a 0a6d 6178  ....).r....Z.max
+00000860: 5f6e 756d 6265 7272 1100 0000 7211 0000  _numberr....r...
+00000870: 0072 1200 0000 da07 6974 6572 6174 654e  .r......iterateN
+00000880: 0000 0073 0200 0000 0a01 7a18 436f 6c6c  ...s......z.Coll
+00000890: 6563 7469 6f6e 4865 6c70 6572 2e69 7465  ectionHelper.ite
+000008a0: 7261 7465 4e29 0146 2901 7235 0000 0029  rateN).F).r5...)
+000008b0: 09da 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
+000008c0: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
+000008d0: 616d 655f 5f72 1e00 0000 7224 0000 0072  ame__r....r$...r
+000008e0: 0800 0000 722c 0000 0072 3400 0000 7236  ....r,...r4...r6
+000008f0: 0000 0072 1100 0000 7211 0000 0072 1100  ...r....r....r..
+00000900: 0000 7212 0000 0072 1400 0000 1300 0000  ..r....r........
+00000910: 730e 0000 0008 0008 0108 0b08 0a08 080a  s...............
+00000920: 0d0e 1072 1400 0000 2907 720d 0000 005a  ...r....).r....Z
+00000930: 2262 6f76 696e 652e 6163 7469 7669 7479  "bovine.activity
+00000940: 7374 7265 616d 732e 7574 696c 732e 7072  streams.utils.pr
+00000950: 696e 7472 0200 0000 5a13 636f 6c6c 6563  intr....Z.collec
+00000960: 7469 6f6e 5f69 7465 7261 746f 7272 0500  tion_iteratorr..
+00000970: 0000 7213 0000 0072 1400 0000 7211 0000  ..r....r....r...
+00000980: 0072 1100 0000 7211 0000 0072 1200 0000  .r....r....r....
+00000990: da08 3c6d 6f64 756c 653e 0100 0000 730a  ..<module>....s.
+000009a0: 0000 0008 000c 020c 0208 0312 0b         .............
```

### Comparing `bovine-0.1.0/bovine/activitypub/__pycache__/collection_iterator.cpython-310.pyc` & `bovine-0.1.1/bovine/activitypub/__pycache__/collection_iterator.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 13 15:55:57 2023 UTC, .py size: 429 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0d26 3864 ad01 0000  o........&8d....
+00000000: 6f0d 0d0a 0000 0000 a4ea 3a64 ad01 0000  o.........:d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 1200 0000 4700  .....@...s....G.
 00000030: 6400 6401 8400 6401 8302 5a00 6402 5300  d.d...d...Z.d.S.
 00000040: 2903 6300 0000 0000 0000 0000 0000 0000  ).c.............
 00000050: 0000 0002 0000 0040 0000 0073 2400 0000  .......@...s$...
 00000060: 6500 5a01 6400 5a02 6401 6402 8400 5a03  e.Z.d.Z.d.d...Z.
 00000070: 6403 6404 8400 5a04 6405 6406 8400 5a05  d.d...Z.d.d...Z.
@@ -11,47 +11,47 @@
 000000a0: 0000 0000 0000 0003 0000 0002 0000 0043  ...............C
 000000b0: 0000 0073 1600 0000 6401 7c00 5f00 7c01  ...s....d.|._.|.
 000000c0: 7c00 5f01 7c02 7c00 5f02 6400 5300 2902  |._.|.|._.d.S.).
 000000d0: 4ee9 0000 0000 2903 da05 636f 756e 74da  N.....)...count.
 000000e0: 1163 6f6c 6c65 6374 696f 6e5f 6865 6c70  .collection_help
 000000f0: 6572 da0a 6d61 785f 6e75 6d62 6572 2903  er..max_number).
 00000100: da04 7365 6c66 7204 0000 0072 0500 0000  ..selfr....r....
-00000110: a900 7207 0000 00fa 5a2f 776f 6f64 7065  ..r.....Z/woodpe
+00000110: a900 7207 0000 00fa 5b2f 776f 6f64 7065  ..r.....[/woodpe
 00000120: 636b 6572 2f73 7263 2f63 6f64 6562 6572  cker/src/codeber
-00000130: 672e 6f72 672f 6865 6c67 652f 626f 7669  g.org/helge/bovi
-00000140: 6e65 2f62 6f76 696e 652f 626f 7669 6e65  ne/bovine/bovine
-00000150: 2f61 6374 6976 6974 7970 7562 2f63 6f6c  /activitypub/col
-00000160: 6c65 6374 696f 6e5f 6974 6572 6174 6f72  lection_iterator
-00000170: 2e70 79da 085f 5f69 6e69 745f 5f02 0000  .py..__init__...
-00000180: 0073 0600 0000 0601 0601 0a01 7a1b 436f  .s..........z.Co
-00000190: 6c6c 6563 7469 6f6e 4974 6572 6174 6f72  llectionIterator
-000001a0: 2e5f 5f69 6e69 745f 5f63 0100 0000 0000  .__init__c......
-000001b0: 0000 0000 0000 0100 0000 0100 0000 4300  ..............C.
-000001c0: 0000 7304 0000 007c 0053 0029 014e 7207  ..s....|.S.).Nr.
-000001d0: 0000 00a9 0172 0600 0000 7207 0000 0072  .....r....r....r
-000001e0: 0700 0000 7208 0000 00da 095f 5f61 6974  ....r......__ait
-000001f0: 6572 5f5f 0700 0000 7302 0000 0004 017a  er__....s......z
-00000200: 1c43 6f6c 6c65 6374 696f 6e49 7465 7261  .CollectionItera
-00000210: 746f 722e 5f5f 6169 7465 725f 5f63 0100  tor.__aiter__c..
-00000220: 0000 0000 0000 0000 0000 0100 0000 0300  ................
-00000230: 0000 c300 0000 7330 0000 0081 017c 0004  ......s0.....|..
-00000240: 006a 0064 0137 0002 005f 007c 006a 007c  .j.d.7..._.|.j.|
-00000250: 006a 016b 0472 1074 0282 017c 006a 03a0  .j.k.r.t...|.j..
-00000260: 04a1 0049 0064 0048 0053 0029 024e e901  ...I.d.H.S.).N..
-00000270: 0000 0029 0572 0300 0000 7205 0000 00da  ...).r....r.....
-00000280: 1253 746f 7041 7379 6e63 4974 6572 6174  .StopAsyncIterat
-00000290: 696f 6e72 0400 0000 da09 6e65 7874 5f69  ionr......next_i
-000002a0: 7465 6d72 0a00 0000 7207 0000 0072 0700  temr....r....r..
-000002b0: 0000 7208 0000 00da 095f 5f61 6e65 7874  ..r......__anext
-000002c0: 5f5f 0a00 0000 730a 0000 0002 800e 010c  __....s.........
-000002d0: 0104 0110 027a 1c43 6f6c 6c65 6374 696f  .....z.Collectio
-000002e0: 6e49 7465 7261 746f 722e 5f5f 616e 6578  nIterator.__anex
-000002f0: 745f 5f4e 2906 da08 5f5f 6e61 6d65 5f5f  t__N)...__name__
-00000300: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
-00000310: 7175 616c 6e61 6d65 5f5f 7209 0000 0072  qualname__r....r
-00000320: 0b00 0000 720f 0000 0072 0700 0000 7207  ....r....r....r.
-00000330: 0000 0072 0700 0000 7208 0000 0072 0100  ...r....r....r..
-00000340: 0000 0100 0000 7308 0000 0008 0008 0108  ......s.........
-00000350: 050c 0372 0100 0000 4e29 0172 0100 0000  ...r....N).r....
-00000360: 7207 0000 0072 0700 0000 7207 0000 0072  r....r....r....r
-00000370: 0800 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
-00000380: 0000 7302 0000 0012 00                   ..s......
+00000130: 672e 6f72 672f 626f 7669 6e65 2f62 6f76  g.org/bovine/bov
+00000140: 696e 652f 626f 7669 6e65 2f62 6f76 696e  ine/bovine/bovin
+00000150: 652f 6163 7469 7669 7479 7075 622f 636f  e/activitypub/co
+00000160: 6c6c 6563 7469 6f6e 5f69 7465 7261 746f  llection_iterato
+00000170: 722e 7079 da08 5f5f 696e 6974 5f5f 0200  r.py..__init__..
+00000180: 0000 7306 0000 0006 0106 010a 017a 1b43  ..s..........z.C
+00000190: 6f6c 6c65 6374 696f 6e49 7465 7261 746f  ollectionIterato
+000001a0: 722e 5f5f 696e 6974 5f5f 6301 0000 0000  r.__init__c.....
+000001b0: 0000 0000 0000 0001 0000 0001 0000 0043  ...............C
+000001c0: 0000 0073 0400 0000 7c00 5300 2901 4e72  ...s....|.S.).Nr
+000001d0: 0700 0000 a901 7206 0000 0072 0700 0000  ......r....r....
+000001e0: 7207 0000 0072 0800 0000 da09 5f5f 6169  r....r......__ai
+000001f0: 7465 725f 5f07 0000 0073 0200 0000 0401  ter__....s......
+00000200: 7a1c 436f 6c6c 6563 7469 6f6e 4974 6572  z.CollectionIter
+00000210: 6174 6f72 2e5f 5f61 6974 6572 5f5f 6301  ator.__aiter__c.
+00000220: 0000 0000 0000 0000 0000 0001 0000 0003  ................
+00000230: 0000 00c3 0000 0073 3000 0000 8101 7c00  .......s0.....|.
+00000240: 0400 6a00 6401 3700 0200 5f00 7c00 6a00  ..j.d.7..._.|.j.
+00000250: 7c00 6a01 6b04 7210 7402 8201 7c00 6a03  |.j.k.r.t...|.j.
+00000260: a004 a100 4900 6400 4800 5300 2902 4ee9  ....I.d.H.S.).N.
+00000270: 0100 0000 2905 7203 0000 0072 0500 0000  ....).r....r....
+00000280: da12 5374 6f70 4173 796e 6349 7465 7261  ..StopAsyncItera
+00000290: 7469 6f6e 7204 0000 00da 096e 6578 745f  tionr......next_
+000002a0: 6974 656d 720a 0000 0072 0700 0000 7207  itemr....r....r.
+000002b0: 0000 0072 0800 0000 da09 5f5f 616e 6578  ...r......__anex
+000002c0: 745f 5f0a 0000 0073 0a00 0000 0280 0e01  t__....s........
+000002d0: 0c01 0401 1002 7a1c 436f 6c6c 6563 7469  ......z.Collecti
+000002e0: 6f6e 4974 6572 6174 6f72 2e5f 5f61 6e65  onIterator.__ane
+000002f0: 7874 5f5f 4e29 06da 085f 5f6e 616d 655f  xt__N)...__name_
+00000300: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
+00000310: 5f71 7561 6c6e 616d 655f 5f72 0900 0000  _qualname__r....
+00000320: 720b 0000 0072 0f00 0000 7207 0000 0072  r....r....r....r
+00000330: 0700 0000 7207 0000 0072 0800 0000 7201  ....r....r....r.
+00000340: 0000 0001 0000 0073 0800 0000 0800 0801  .......s........
+00000350: 0805 0c03 7201 0000 004e 2901 7201 0000  ....r....N).r...
+00000360: 0072 0700 0000 7207 0000 0072 0700 0000  .r....r....r....
+00000370: 7208 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
+00000380: 0000 0073 0200 0000 1200                 ...s......
```

### Comparing `bovine-0.1.0/bovine/activitypub/__pycache__/test_actor.cpython-310-pytest-7.3.0.pyc` & `bovine-0.1.1/bovine/activitypub/__pycache__/test_actor.cpython-310-pytest-7.3.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 13 15:55:57 2023 UTC, .py size: 2909 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 16% similar despite different names*

```diff
@@ -1,229 +1,228 @@
-00000000: 6f0d 0d0a 0000 0000 0d26 3864 5d0b 0000  o........&8d]...
+00000000: 6f0d 0d0a 0000 0000 a4ea 3a64 c50a 0000  o.........:d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 7600 0000 6400  .....@...sv...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6401 6c06 5a06  ..m.Z...d.d.l.Z.
 00000050: 6400 6402 6c07 6d08 5a08 6d09 5a09 0100  d.d.l.m.Z.m.Z...
 00000060: 6400 6401 6c0a 5a0a 6400 6403 6c0b 6d0c  d.d.l.Z.d.d.l.m.
 00000070: 5a0c 0100 6400 6404 6c0d 6d0e 5a0e 6d0f  Z...d.d.l.m.Z.m.
 00000080: 5a0f 0100 6400 6405 6c10 6d11 5a11 0100  Z...d.d.l.m.Z...
 00000090: 6406 6407 8400 5a12 6408 6409 8400 5a13  d.d...Z.d.d...Z.
 000000a0: 6401 5300 290a e900 0000 004e 2902 da09  d.S.)......N)...
 000000b0: 4173 796e 634d 6f63 6bda 094d 6167 6963  AsyncMock..Magic
 000000c0: 4d6f 636b 2901 da0b 426f 7669 6e65 4163  Mock)...BovineAc
-000000d0: 746f 7229 02da 1862 7569 6c64 5f6f 7264  tor)...build_ord
-000000e0: 6572 6564 5f63 6f6c 6c65 6374 696f 6eda  ered_collection.
-000000f0: 1d62 7569 6c64 5f6f 7264 6572 6564 5f63  .build_ordered_c
-00000100: 6f6c 6c65 6374 696f 6e5f 7061 6765 2901  ollection_page).
-00000110: da0b 7072 6976 6174 655f 6b65 7963 0000  ..private_keyc..
-00000120: 0000 0000 0000 0000 0000 0f00 0000 0700  ................
-00000130: 0000 c300 0000 7398 0100 0081 0174 0074  ......s......t.t
-00000140: 016a 0283 017d 0064 017d 0164 027d 0274  .j...}.d.}.d.}.t
-00000150: 0074 016a 0283 017d 0074 0083 007c 005f  .t.j...}.t...|._
-00000160: 0374 0469 0083 01a0 0564 03a1 016a 067c  .t.i.....d...j.|
-00000170: 0274 077c 0064 048d 037d 0374 0083 007d  .t.|.d...}.t...}
-00000180: 0474 0874 016a 0983 017c 006a 035f 0a7c  .t.t.j...|.j._.|
-00000190: 047c 006a 036a 0a5f 0b64 0564 0684 0074  .|.j.j._.d.d...t
-000001a0: 0c64 0783 0144 0083 017d 0574 0d64 0883  .d...D...}.t.d..
-000001b0: 01a0 0e64 07a1 01a0 0f7c 05a1 017d 0674  ...d.....|...}.t
-000001c0: 10a0 117c 06a0 12a1 00a1 017c 045f 0a7c  ...|.......|._.|
-000001d0: 03a0 137c 01a1 0149 0064 0048 007d 077c  ...|...I.d.H.}.|
-000001e0: 006a 03a0 14a1 0001 007c 0764 0919 007d  .j.......|.d...}
-000001f0: 0864 077d 097c 087c 096b 027d 0a7c 0a73  .d.}.|.|.k.}.|.s
-00000200: 8674 15a0 1664 0a7c 0a66 0164 0b7c 087c  .t...d.|.f.d.|.|
-00000210: 0966 02a1 0474 15a0 177c 08a1 0174 15a0  .f...t...|...t..
-00000220: 177c 09a1 0164 0c9c 0216 007d 0b64 0d64  .|...d.....}.d.d
-00000230: 0e7c 0b69 0116 007d 0c74 1874 15a0 197c  .|.i...}.t.t...|
-00000240: 0ca1 0183 0182 0164 0004 007d 0804 007d  .......d...}...}
-00000250: 0a7d 097c 0764 0f19 007d 087c 087c 056b  .}.|.d...}.|.|.k
-00000260: 027d 0a7c 0a73 c674 15a0 1664 0a7c 0a66  .}.|.s.t...d.|.f
-00000270: 0164 107c 087c 0566 02a1 0474 15a0 177c  .d.|.|.f...t...|
-00000280: 08a1 0164 0f74 1aa0 1ba1 0076 0073 af74  ...d.t.....v.s.t
-00000290: 15a0 1c7c 05a1 0172 b474 15a0 177c 05a1  ...|...r.t...|..
-000002a0: 016e 0164 0f64 119c 0216 007d 0d64 1264  .n.d.d.....}.d.d
-000002b0: 137c 0d69 0116 007d 0e74 1874 15a0 197c  .|.i...}.t.t...|
-000002c0: 0ea1 0183 0182 0164 0004 007d 087d 0a64  .......d...}.}.d
-000002d0: 0053 0029 144e fa1d 6874 7470 733a 2f2f  .S.).N..https://
-000002e0: 7465 7374 5f64 6f6d 6169 6e2f 7465 7374  test_domain/test
-000002f0: 5f70 6174 68da 0e70 7562 6c69 635f 6b65  _path..public_ke
-00000300: 795f 7572 6cda 0861 6374 6f72 5f69 64a9  y_url..actor_id.
-00000310: 01da 0773 6573 7369 6f6e 6301 0000 0000  ...sessionc.....
-00000320: 0000 0000 0000 0002 0000 0004 0000 0053  ...............S
-00000330: 0000 00f3 1400 0000 6700 7c00 5d06 7d01  ........g.|.].}.
-00000340: 6400 7c01 6901 9102 7102 5300 a901 da02  d.|.i...q.S.....
-00000350: 6964 a900 a902 da02 2e30 da01 6a72 1000  id.......0..jr..
-00000360: 0000 7210 0000 00fa 512f 776f 6f64 7065  ..r.....Q/woodpe
-00000370: 636b 6572 2f73 7263 2f63 6f64 6562 6572  cker/src/codeber
-00000380: 672e 6f72 672f 6865 6c67 652f 626f 7669  g.org/helge/bovi
-00000390: 6e65 2f62 6f76 696e 652f 626f 7669 6e65  ne/bovine/bovine
-000003a0: 2f61 6374 6976 6974 7970 7562 2f74 6573  /activitypub/tes
-000003b0: 745f 6163 746f 722e 7079 da0a 3c6c 6973  t_actor.py..<lis
-000003c0: 7463 6f6d 703e 1f00 0000 f302 0000 0014  tcomp>..........
-000003d0: 007a 4474 6573 745f 6163 7469 7669 7479  .zDtest_activity
-000003e0: 5f70 7562 5f63 6c69 656e 745f 6765 745f  _pub_client_get_
-000003f0: 636f 6c6c 6563 7469 6f6e 5f6e 6f5f 7061  collection_no_pa
-00000400: 6765 732e 3c6c 6f63 616c 733e 2e3c 6c69  ges.<locals>.<li
-00000410: 7374 636f 6d70 3ee9 0700 0000 da03 7572  stcomp>.......ur
-00000420: 6cda 0b74 6f74 616c 5f69 7465 6d73 a901  l..total_items..
-00000430: fa02 3d3d a901 7a12 2528 7079 3129 7320  ..==..z.%(py1)s 
-00000440: 3d3d 2025 2870 7934 2973 a902 da03 7079  == %(py4)s....py
-00000450: 31da 0370 7934 fa0e 6173 7365 7274 2025  1..py4..assert %
-00000460: 2870 7936 2973 da03 7079 36da 0569 7465  (py6)s..py6..ite
-00000470: 6d73 a901 7a12 2528 7079 3129 7320 3d3d  ms..z.%(py1)s ==
-00000480: 2025 2870 7933 2973 a902 721e 0000 00da   %(py3)s..r.....
-00000490: 0370 7933 fa0e 6173 7365 7274 2025 2870  .py3..assert %(p
-000004a0: 7935 2973 da03 7079 3529 1d72 0200 0000  y5)s..py5).r....
-000004b0: da07 6169 6f68 7474 70da 0d43 6c69 656e  ..aiohttp..Clien
-000004c0: 7453 6573 7369 6f6e da03 6765 7472 0400  tSession..getr..
-000004d0: 0000 da0d 7769 7468 5f61 6374 6f72 5f69  ....with_actor_i
-000004e0: 64da 1377 6974 685f 6874 7470 5f73 6967  d..with_http_sig
-000004f0: 6e61 7475 7265 7207 0000 0072 0300 0000  naturer....r....
-00000500: da0e 436c 6965 6e74 5265 7370 6f6e 7365  ..ClientResponse
-00000510: da0c 7265 7475 726e 5f76 616c 7565 da04  ..return_value..
-00000520: 7465 7874 da05 7261 6e67 6572 0500 0000  text..ranger....
-00000530: da0a 7769 7468 5f63 6f75 6e74 da0a 7769  ..with_count..wi
-00000540: 7468 5f69 7465 6d73 da04 6a73 6f6e da05  th_items..json..
-00000550: 6475 6d70 73da 0562 7569 6c64 da16 6765  dumps..build..ge
-00000560: 745f 6f72 6465 7265 645f 636f 6c6c 6563  t_ordered_collec
-00000570: 7469 6f6e 5a13 6173 7365 7274 5f61 7761  tionZ.assert_awa
-00000580: 6974 6564 5f6f 6e63 65da 0a40 7079 7465  ited_once..@pyte
-00000590: 7374 5f61 72da 115f 6361 6c6c 5f72 6570  st_ar.._call_rep
-000005a0: 7263 6f6d 7061 7265 da09 5f73 6166 6572  rcompare.._safer
-000005b0: 6570 72da 0e41 7373 6572 7469 6f6e 4572  epr..AssertionEr
-000005c0: 726f 72da 135f 666f 726d 6174 5f65 7870  ror.._format_exp
-000005d0: 6c61 6e61 7469 6f6e da0c 4070 795f 6275  lanation..@py_bu
-000005e0: 696c 7469 6e73 da06 6c6f 6361 6c73 da18  iltins..locals..
-000005f0: 5f73 686f 756c 645f 7265 7072 5f67 6c6f  _should_repr_glo
-00000600: 6261 6c5f 6e61 6d65 290f 720c 0000 0072  bal_name).r....r
-00000610: 1800 0000 7209 0000 00da 0561 6374 6f72  ....r......actor
-00000620: da09 7465 7874 5f6d 6f63 6b72 2200 0000  ..text_mockr"...
-00000630: da07 6275 696c 6465 72da 0672 6573 756c  ..builder..resul
-00000640: 74da 0b40 7079 5f61 7373 6572 7430 da0b  t..@py_assert0..
-00000650: 4070 795f 6173 7365 7274 33da 0b40 7079  @py_assert3..@py
-00000660: 5f61 7373 6572 7432 da0b 4070 795f 666f  _assert2..@py_fo
-00000670: 726d 6174 35da 0b40 7079 5f66 6f72 6d61  rmat5..@py_forma
-00000680: 7437 da0b 4070 795f 666f 726d 6174 34da  t7..@py_format4.
-00000690: 0b40 7079 5f66 6f72 6d61 7436 7210 0000  .@py_format6r...
-000006a0: 0072 1000 0000 7214 0000 00da 3074 6573  .r....r.....0tes
-000006b0: 745f 6163 7469 7669 7479 5f70 7562 5f63  t_activity_pub_c
-000006c0: 6c69 656e 745f 6765 745f 636f 6c6c 6563  lient_get_collec
-000006d0: 7469 6f6e 5f6e 6f5f 7061 6765 730e 0000  tion_no_pages...
-000006e0: 0073 2a00 0000 0280 0a01 0401 0401 0a01  .s*.............
-000006f0: 0801 0603 0601 0801 04fe 02ff 0606 0e01  ................
-00000700: 0a01 1202 1402 1002 1002 0a01 6a02 8001  ............j...
-00000710: 724a 0000 0063 0000 0000 0000 0000 0000  rJ...c..........
-00000720: 0000 1200 0000 0700 0000 c300 0000 7334  ..............s4
-00000730: 0300 0081 0174 0074 016a 0283 017d 0064  .....t.t.j...}.d
-00000740: 017d 0164 027d 0274 0074 016a 0283 017d  .}.d.}.t.t.j...}
-00000750: 0074 0083 007c 005f 0374 0469 0083 01a0  .t...|._.t.i....
-00000760: 0564 03a1 016a 067c 0274 077c 0064 048d  .d...j.|.t.|.d..
-00000770: 037d 0374 0083 007d 0474 0874 016a 0983  .}.t...}.t.t.j..
-00000780: 017c 006a 035f 0a7c 047c 006a 036a 0a5f  .|.j._.|.|.j.j._
-00000790: 0b64 0564 0684 0074 0c64 0783 0144 0083  .d.d...t.d...D..
-000007a0: 017d 0574 0d64 0883 01a0 0e64 07a1 01a0  .}.t.d.....d....
-000007b0: 0f64 0964 0aa1 027d 0674 1064 0b64 0c83  .d.d...}.t.d.d..
-000007c0: 02a0 117c 0564 0064 0d85 0219 00a1 01a0  ...|.d.d........
-000007d0: 1264 0ea1 017d 0774 1064 0b64 0f83 02a0  .d...}.t.d.d....
-000007e0: 117c 0564 0d64 1085 0219 00a1 01a0 1264  .|.d.d.........d
-000007f0: 11a1 017d 0874 1064 0b64 0f83 02a0 117c  ...}.t.d.d.....|
-00000800: 0564 1064 0085 0219 00a1 017d 0974 13a0  .d.d.......}.t..
-00000810: 147c 06a0 15a1 00a1 0174 13a0 147c 07a0  .|.......t...|..
-00000820: 15a1 00a1 0174 13a0 147c 08a0 15a1 00a1  .....t...|......
-00000830: 0174 13a0 147c 09a0 15a1 00a1 0167 047c  .t...|.......g.|
-00000840: 045f 167c 03a0 177c 01a1 0149 0064 0048  ._.|...|...I.d.H
-00000850: 007d 0a7c 0a64 1219 007d 0b64 077d 0c7c  .}.|.d...}.d.}.|
-00000860: 0b7c 0c6b 027d 0d7c 0d73 bf74 18a0 1964  .|.k.}.|.s.t...d
-00000870: 137c 0d66 0164 147c 0b7c 0c66 02a1 0474  .|.f.d.|.|.f...t
-00000880: 18a0 1a7c 0ba1 0174 18a0 1a7c 0ca1 0164  ...|...t...|...d
-00000890: 159c 0216 007d 0e64 1664 177c 0e69 0116  .....}.d.d.|.i..
-000008a0: 007d 0f74 1b74 18a0 1c7c 0fa1 0183 0182  .}.t.t...|......
-000008b0: 0164 0004 007d 0b04 007d 0d7d 0c7c 0a64  .d...}...}.}.|.d
-000008c0: 1819 007d 0b7c 0b7c 056b 027d 0d7c 0d73  ...}.|.|.k.}.|.s
-000008d0: ff74 18a0 1964 137c 0d66 0164 197c 0b7c  .t...d.|.f.d.|.|
-000008e0: 0566 02a1 0474 18a0 1a7c 0ba1 0164 1874  .f...t...|...d.t
-000008f0: 1da0 1ea1 0076 0073 e874 18a0 1f7c 05a1  .....v.s.t...|..
-00000900: 0172 ed74 18a0 1a7c 05a1 016e 0164 1864  .r.t...|...n.d.d
-00000910: 1a9c 0216 007d 1064 1b64 1c7c 1069 0116  .....}.d.d.|.i..
-00000920: 007d 1174 1b74 18a0 1c7c 11a1 0183 0182  .}.t.t...|......
-00000930: 0164 0004 007d 0b7d 0d74 13a0 147c 06a0  .d...}.}.t...|..
-00000940: 15a1 00a1 0174 13a0 147c 07a0 15a1 00a1  .....t...|......
-00000950: 0174 13a0 147c 08a0 15a1 00a1 0174 13a0  .t...|.......t..
-00000960: 147c 09a0 15a1 00a1 0167 047c 045f 167c  .|.......g.|._.|
-00000970: 036a 177c 0164 1d64 1e8d 0249 0064 0048  .j.|.d.d...I.d.H
-00000980: 007d 0a7c 0a64 1219 007d 0b64 077d 0c7c  .}.|.d...}.d.}.|
-00000990: 0b7c 0c6b 027d 0d7c 0d90 0173 5874 18a0  .|.k.}.|...sXt..
-000009a0: 1964 137c 0d66 0164 147c 0b7c 0c66 02a1  .d.|.f.d.|.|.f..
-000009b0: 0474 18a0 1a7c 0ba1 0174 18a0 1a7c 0ca1  .t...|...t...|..
-000009c0: 0164 159c 0216 007d 0e64 1664 177c 0e69  .d.....}.d.d.|.i
-000009d0: 0116 007d 0f74 1b74 18a0 1c7c 0fa1 0183  ...}.t.t...|....
-000009e0: 0182 0164 0004 007d 0b04 007d 0d7d 0c7c  ...d...}...}.}.|
-000009f0: 0a64 1819 007d 0b7c 0564 0064 1085 0219  .d...}.|.d.d....
-00000a00: 007d 0c7c 0b7c 0c6b 027d 0d7c 0d90 0173  .}.|.|.k.}.|...s
-00000a10: 9274 18a0 1964 137c 0d66 0164 147c 0b7c  .t...d.|.f.d.|.|
-00000a20: 0c66 02a1 0474 18a0 1a7c 0ba1 0174 18a0  .f...t...|...t..
-00000a30: 1a7c 0ca1 0164 159c 0216 007d 0e64 1664  .|...d.....}.d.d
-00000a40: 177c 0e69 0116 007d 0f74 1b74 18a0 1c7c  .|.i...}.t.t...|
-00000a50: 0fa1 0183 0182 0164 0004 007d 0b04 007d  .......d...}...}
-00000a60: 0d7d 0c64 0053 0029 1f4e 7208 0000 0072  .}.d.S.).Nr....r
-00000a70: 0900 0000 720a 0000 0072 0b00 0000 6301  ....r....r....c.
-00000a80: 0000 0000 0000 0000 0000 0002 0000 0004  ................
-00000a90: 0000 0053 0000 0072 0d00 0000 720e 0000  ...S...r....r...
-00000aa0: 0072 1000 0000 7211 0000 0072 1000 0000  .r....r....r....
-00000ab0: 7210 0000 0072 1400 0000 7215 0000 003c  r....r....r....<
-00000ac0: 0000 0072 1600 0000 7a41 7465 7374 5f61  ...r....zAtest_a
-00000ad0: 6374 6976 6974 795f 7075 625f 636c 6965  ctivity_pub_clie
-00000ae0: 6e74 5f67 6574 5f63 6f6c 6c65 6374 696f  nt_get_collectio
-00000af0: 6e5f 7061 6765 732e 3c6c 6f63 616c 733e  n_pages.<locals>
-00000b00: 2e3c 6c69 7374 636f 6d70 3ee9 1700 0000  .<listcomp>.....
-00000b10: 7218 0000 00da 0566 6972 7374 da04 6c61  r......first..la
-00000b20: 7374 5a05 7572 6c5f 31da 0670 6167 655f  stZ.url_1..page_
-00000b30: 31e9 0d00 0000 5a06 6e65 7874 5f31 da06  1.....Z.next_1..
-00000b40: 7061 6765 5f32 e914 0000 005a 066e 6578  page_2.....Z.nex
-00000b50: 745f 3272 1900 0000 721a 0000 0072 1c00  t_2r....r....r..
-00000b60: 0000 721d 0000 0072 2000 0000 7221 0000  ..r....r ...r!..
-00000b70: 0072 2200 0000 7223 0000 0072 2400 0000  .r"...r#...r$...
-00000b80: 7226 0000 0072 2700 0000 e911 0000 0029  r&...r'........)
-00000b90: 01da 096d 6178 5f69 7465 6d73 2920 7202  ...max_items) r.
-00000ba0: 0000 0072 2800 0000 7229 0000 0072 2a00  ...r(...r)...r*.
-00000bb0: 0000 7204 0000 0072 2b00 0000 722c 0000  ..r....r+...r,..
-00000bc0: 0072 0700 0000 7203 0000 0072 2d00 0000  .r....r....r-...
-00000bd0: 722e 0000 0072 2f00 0000 7230 0000 0072  r....r/...r0...r
-00000be0: 0500 0000 7231 0000 00da 1377 6974 685f  ....r1.....with_
-00000bf0: 6669 7273 745f 616e 645f 6c61 7374 7206  first_and_lastr.
-00000c00: 0000 0072 3200 0000 da09 7769 7468 5f6e  ...r2.....with_n
-00000c10: 6578 7472 3300 0000 7234 0000 0072 3500  extr3...r4...r5.
-00000c20: 0000 5a0b 7369 6465 5f65 6666 6563 7472  ..Z.side_effectr
-00000c30: 3600 0000 7237 0000 0072 3800 0000 7239  6...r7...r8...r9
-00000c40: 0000 0072 3a00 0000 723b 0000 0072 3c00  ...r:...r;...r<.
-00000c50: 0000 723d 0000 0072 3e00 0000 2912 720c  ..r=...r>...).r.
-00000c60: 0000 0072 1800 0000 7209 0000 0072 3f00  ...r....r....r?.
-00000c70: 0000 7240 0000 0072 2200 0000 7241 0000  ..r@...r"...rA..
-00000c80: 0072 4e00 0000 7250 0000 005a 0670 6167  .rN...rP...Z.pag
-00000c90: 655f 3372 4200 0000 7243 0000 0072 4400  e_3rB...rC...rD.
-00000ca0: 0000 7245 0000 0072 4600 0000 7247 0000  ..rE...rF...rG..
-00000cb0: 0072 4800 0000 7249 0000 0072 1000 0000  .rH...rI...r....
-00000cc0: 7210 0000 0072 1400 0000 da2d 7465 7374  r....r.....-test
-00000cd0: 5f61 6374 6976 6974 795f 7075 625f 636c  _activity_pub_cl
-00000ce0: 6965 6e74 5f67 6574 5f63 6f6c 6c65 6374  ient_get_collect
-00000cf0: 696f 6e5f 7061 6765 732c 0000 0073 5800  ion_pages,...sX.
-00000d00: 0000 0280 0a01 0401 0401 0a01 0801 0603  ................
-00000d10: 0601 0801 04fe 02ff 0605 0e01 0a01 1202  ................
-00000d20: 0603 0601 0801 02fd 0807 0e01 0601 02fd  ................
-00000d30: 0806 0e01 0601 02fd 1805 0c03 0c01 0c01  ................
-00000d40: 0c01 06fc 1007 6a02 7c01 0c03 0c01 0c01  ......j.|.......
-00000d50: 0c01 06fc 1407 6c02 7801 7256 0000 0029  ......l.x.rV...)
-00000d60: 14da 0862 7569 6c74 696e 7372 3c00 0000  ...builtinsr<...
-00000d70: da19 5f70 7974 6573 742e 6173 7365 7274  .._pytest.assert
-00000d80: 696f 6e2e 7265 7772 6974 65da 0961 7373  ion.rewrite..ass
-00000d90: 6572 7469 6f6e da07 7265 7772 6974 6572  ertion..rewriter
-00000da0: 3700 0000 7233 0000 005a 0d75 6e69 7474  7...r3...Z.unitt
-00000db0: 6573 742e 6d6f 636b 7202 0000 0072 0300  est.mockr....r..
-00000dc0: 0000 7228 0000 00da 0662 6f76 696e 6572  ..r(.....boviner
-00000dd0: 0400 0000 5a16 626f 7669 6e65 2e61 6374  ....Z.bovine.act
-00000de0: 6976 6974 7973 7472 6561 6d73 7205 0000  ivitystreamsr...
-00000df0: 0072 0600 0000 5a12 626f 7669 6e65 2e63  .r....Z.bovine.c
-00000e00: 7279 7074 6f2e 7465 7374 7207 0000 0072  rypto.testr....r
-00000e10: 4a00 0000 7256 0000 0072 1000 0000 7210  J...rV...r....r.
-00000e20: 0000 0072 1000 0000 7214 0000 00da 083c  ...r....r......<
-00000e30: 6d6f 6475 6c65 3e01 0000 0073 1000 0000  module>....s....
-00000e40: 2200 1001 0802 0c02 1001 0c04 0803 0c1e  "...............
+000000d0: 746f 7229 02da 114f 7264 6572 6564 436f  tor)...OrderedCo
+000000e0: 6c6c 6563 7469 6f6e da15 4f72 6465 7265  llection..Ordere
+000000f0: 6443 6f6c 6c65 6374 696f 6e50 6167 6529  dCollectionPage)
+00000100: 01da 0b70 7269 7661 7465 5f6b 6579 6300  ...private_keyc.
+00000110: 0000 0000 0000 0000 0000 000f 0000 0007  ................
+00000120: 0000 00c3 0000 0073 9201 0000 8101 7400  .......s......t.
+00000130: 7401 6a02 8301 7d00 6401 7d01 6402 7d02  t.j...}.d.}.d.}.
+00000140: 7400 7401 6a02 8301 7d00 7400 8300 7c00  t.t.j...}.t...|.
+00000150: 5f03 7404 6900 8301 a005 6403 a101 6a06  _.t.i.....d...j.
+00000160: 7c02 7407 7c00 6404 8d03 7d03 7400 8300  |.t.|.d...}.t...
+00000170: 7d04 7408 7401 6a09 8301 7c00 6a03 5f0a  }.t.t.j...|.j._.
+00000180: 7c04 7c00 6a03 6a0a 5f0b 6405 6406 8400  |.|.j.j._.d.d...
+00000190: 740c 6407 8301 4400 8301 7d05 740d 6408  t.d...D...}.t.d.
+000001a0: 6407 7c05 6409 8d03 7d06 740e a00f 7c06  d.|.d...}.t...|.
+000001b0: a010 a100 a101 7c04 5f0a 7c03 a011 7c01  ......|._.|...|.
+000001c0: a101 4900 6400 4800 7d07 7c00 6a03 a012  ..I.d.H.}.|.j...
+000001d0: a100 0100 7c07 640a 1900 7d08 6407 7d09  ....|.d...}.d.}.
+000001e0: 7c08 7c09 6b02 7d0a 7c0a 7383 7413 a014  |.|.k.}.|.s.t...
+000001f0: 640b 7c0a 6601 640c 7c08 7c09 6602 a104  d.|.f.d.|.|.f...
+00000200: 7413 a015 7c08 a101 7413 a015 7c09 a101  t...|...t...|...
+00000210: 640d 9c02 1600 7d0b 640e 640f 7c0b 6901  d.....}.d.d.|.i.
+00000220: 1600 7d0c 7416 7413 a017 7c0c a101 8301  ..}.t.t...|.....
+00000230: 8201 6400 0400 7d08 0400 7d0a 7d09 7c07  ..d...}...}.}.|.
+00000240: 6410 1900 7d08 7c08 7c05 6b02 7d0a 7c0a  d...}.|.|.k.}.|.
+00000250: 73c3 7413 a014 640b 7c0a 6601 6411 7c08  s.t...d.|.f.d.|.
+00000260: 7c05 6602 a104 7413 a015 7c08 a101 6410  |.f...t...|...d.
+00000270: 7418 a019 a100 7600 73ac 7413 a01a 7c05  t.....v.s.t...|.
+00000280: a101 72b1 7413 a015 7c05 a101 6e01 6410  ..r.t...|...n.d.
+00000290: 6412 9c02 1600 7d0d 6413 6414 7c0d 6901  d.....}.d.d.|.i.
+000002a0: 1600 7d0e 7416 7413 a017 7c0e a101 8301  ..}.t.t...|.....
+000002b0: 8201 6400 0400 7d08 7d0a 6400 5300 2915  ..d...}.}.d.S.).
+000002c0: 4efa 1d68 7474 7073 3a2f 2f74 6573 745f  N..https://test_
+000002d0: 646f 6d61 696e 2f74 6573 745f 7061 7468  domain/test_path
+000002e0: da0e 7075 626c 6963 5f6b 6579 5f75 726c  ..public_key_url
+000002f0: da08 6163 746f 725f 6964 a901 da07 7365  ..actor_id....se
+00000300: 7373 696f 6e63 0100 0000 0000 0000 0000  ssionc..........
+00000310: 0000 0200 0000 0400 0000 5300 0000 f314  ..........S.....
+00000320: 0000 0067 007c 005d 067d 0164 007c 0169  ...g.|.].}.d.|.i
+00000330: 0191 0271 0253 00a9 01da 0269 64a9 00a9  ...q.S.....id...
+00000340: 02da 022e 30da 016a 7210 0000 0072 1000  ....0..jr....r..
+00000350: 0000 fa52 2f77 6f6f 6470 6563 6b65 722f  ...R/woodpecker/
+00000360: 7372 632f 636f 6465 6265 7267 2e6f 7267  src/codeberg.org
+00000370: 2f62 6f76 696e 652f 626f 7669 6e65 2f62  /bovine/bovine/b
+00000380: 6f76 696e 652f 626f 7669 6e65 2f61 6374  ovine/bovine/act
+00000390: 6976 6974 7970 7562 2f74 6573 745f 6163  ivitypub/test_ac
+000003a0: 746f 722e 7079 da0a 3c6c 6973 7463 6f6d  tor.py..<listcom
+000003b0: 703e 1c00 0000 f302 0000 0014 007a 4474  p>...........zDt
+000003c0: 6573 745f 6163 7469 7669 7479 5f70 7562  est_activity_pub
+000003d0: 5f63 6c69 656e 745f 6765 745f 636f 6c6c  _client_get_coll
+000003e0: 6563 7469 6f6e 5f6e 6f5f 7061 6765 732e  ection_no_pages.
+000003f0: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
+00000400: 6d70 3ee9 0700 0000 da03 7572 6c29 0372  mp>.......url).r
+00000410: 0f00 0000 da05 636f 756e 74da 0569 7465  ......count..ite
+00000420: 6d73 da0b 746f 7461 6c5f 6974 656d 73a9  ms..total_items.
+00000430: 01fa 023d 3da9 017a 1225 2870 7931 2973  ...==..z.%(py1)s
+00000440: 203d 3d20 2528 7079 3429 73a9 02da 0370   == %(py4)s....p
+00000450: 7931 da03 7079 34fa 0e61 7373 6572 7420  y1..py4..assert 
+00000460: 2528 7079 3629 73da 0370 7936 721a 0000  %(py6)s..py6r...
+00000470: 00a9 017a 1225 2870 7931 2973 203d 3d20  ...z.%(py1)s == 
+00000480: 2528 7079 3329 73a9 0272 2000 0000 da03  %(py3)s..r .....
+00000490: 7079 33fa 0e61 7373 6572 7420 2528 7079  py3..assert %(py
+000004a0: 3529 73da 0370 7935 291b 7202 0000 00da  5)s..py5).r.....
+000004b0: 0761 696f 6874 7470 da0d 436c 6965 6e74  .aiohttp..Client
+000004c0: 5365 7373 696f 6eda 0367 6574 7204 0000  Session..getr...
+000004d0: 00da 0d77 6974 685f 6163 746f 725f 6964  ...with_actor_id
+000004e0: da13 7769 7468 5f68 7474 705f 7369 676e  ..with_http_sign
+000004f0: 6174 7572 6572 0700 0000 7203 0000 00da  aturer....r.....
+00000500: 0e43 6c69 656e 7452 6573 706f 6e73 65da  .ClientResponse.
+00000510: 0c72 6574 7572 6e5f 7661 6c75 65da 0474  .return_value..t
+00000520: 6578 74da 0572 616e 6765 7205 0000 00da  ext..ranger.....
+00000530: 046a 736f 6eda 0564 756d 7073 da05 6275  .json..dumps..bu
+00000540: 696c 64da 1667 6574 5f6f 7264 6572 6564  ild..get_ordered
+00000550: 5f63 6f6c 6c65 6374 696f 6e5a 1361 7373  _collectionZ.ass
+00000560: 6572 745f 6177 6169 7465 645f 6f6e 6365  ert_awaited_once
+00000570: da0a 4070 7974 6573 745f 6172 da11 5f63  ..@pytest_ar.._c
+00000580: 616c 6c5f 7265 7072 636f 6d70 6172 65da  all_reprcompare.
+00000590: 095f 7361 6665 7265 7072 da0e 4173 7365  ._saferepr..Asse
+000005a0: 7274 696f 6e45 7272 6f72 da13 5f66 6f72  rtionError.._for
+000005b0: 6d61 745f 6578 706c 616e 6174 696f 6eda  mat_explanation.
+000005c0: 0c40 7079 5f62 7569 6c74 696e 73da 066c  .@py_builtins..l
+000005d0: 6f63 616c 73da 185f 7368 6f75 6c64 5f72  ocals.._should_r
+000005e0: 6570 725f 676c 6f62 616c 5f6e 616d 6529  epr_global_name)
+000005f0: 0f72 0c00 0000 7218 0000 0072 0900 0000  .r....r....r....
+00000600: da05 6163 746f 72da 0974 6578 745f 6d6f  ..actor..text_mo
+00000610: 636b 721a 0000 00da 0762 7569 6c64 6572  ckr......builder
+00000620: da06 7265 7375 6c74 da0b 4070 795f 6173  ..result..@py_as
+00000630: 7365 7274 30da 0b40 7079 5f61 7373 6572  sert0..@py_asser
+00000640: 7433 da0b 4070 795f 6173 7365 7274 32da  t3..@py_assert2.
+00000650: 0b40 7079 5f66 6f72 6d61 7435 da0b 4070  .@py_format5..@p
+00000660: 795f 666f 726d 6174 37da 0b40 7079 5f66  y_format7..@py_f
+00000670: 6f72 6d61 7434 da0b 4070 795f 666f 726d  ormat4..@py_form
+00000680: 6174 3672 1000 0000 7210 0000 0072 1400  at6r....r....r..
+00000690: 0000 da30 7465 7374 5f61 6374 6976 6974  ...0test_activit
+000006a0: 795f 7075 625f 636c 6965 6e74 5f67 6574  y_pub_client_get
+000006b0: 5f63 6f6c 6c65 6374 696f 6e5f 6e6f 5f70  _collection_no_p
+000006c0: 6167 6573 0b00 0000 732a 0000 0002 800a  ages....s*......
+000006d0: 0104 0104 010a 0108 0106 0306 0108 0104  ................
+000006e0: fe02 ff06 060e 010a 0112 020e 0210 0110  ................
+000006f0: 020a 016a 0280 0172 4900 0000 6300 0000  ...j...rI...c...
+00000700: 0000 0000 0000 0000 0012 0000 0007 0000  ................
+00000710: 00c3 0000 0073 2003 0000 8101 7400 7401  .....s .....t.t.
+00000720: 6a02 8301 7d00 6401 7d01 6402 7d02 7400  j...}.d.}.d.}.t.
+00000730: 7401 6a02 8301 7d00 7400 8300 7c00 5f03  t.j...}.t...|._.
+00000740: 7404 6900 8301 a005 6403 a101 6a06 7c02  t.i.....d...j.|.
+00000750: 7407 7c00 6404 8d03 7d03 7400 8300 7d04  t.|.d...}.t...}.
+00000760: 7408 7401 6a09 8301 7c00 6a03 5f0a 7c04  t.t.j...|.j._.|.
+00000770: 7c00 6a03 6a0a 5f0b 6405 6406 8400 740c  |.j.j._.d.d...t.
+00000780: 6407 8301 4400 8301 7d05 740d 6408 6407  d...D...}.t.d.d.
+00000790: 6409 640a 640b 8d04 7d06 740e 640c 7c05  d.d.d...}.t.d.|.
+000007a0: 6400 640d 8502 1900 640e 640f 6410 8d04  d.d.....d.d.d...
+000007b0: 7d07 740e 6411 7c05 640d 6412 8502 1900  }.t.d.|.d.d.....
+000007c0: 640e 6413 6410 8d04 7d08 740e 6414 7c05  d.d.d...}.t.d.|.
+000007d0: 6412 6400 8502 1900 640e 6415 8d03 7d09  d.d.....d.d...}.
+000007e0: 740f a010 7c06 a011 a100 a101 740f a010  t...|.......t...
+000007f0: 7c07 a011 a100 a101 740f a010 7c08 a011  |.......t...|...
+00000800: a100 a101 740f a010 7c09 a011 a100 a101  ....t...|.......
+00000810: 6704 7c04 5f12 7c03 a013 7c01 a101 4900  g.|._.|...|...I.
+00000820: 6400 4800 7d0a 7c0a 6416 1900 7d0b 6407  d.H.}.|.d...}.d.
+00000830: 7d0c 7c0b 7c0c 6b02 7d0d 7c0d 73b5 7414  }.|.|.k.}.|.s.t.
+00000840: a015 6417 7c0d 6601 6418 7c0b 7c0c 6602  ..d.|.f.d.|.|.f.
+00000850: a104 7414 a016 7c0b a101 7414 a016 7c0c  ..t...|...t...|.
+00000860: a101 6419 9c02 1600 7d0e 641a 641b 7c0e  ..d.....}.d.d.|.
+00000870: 6901 1600 7d0f 7417 7414 a018 7c0f a101  i...}.t.t...|...
+00000880: 8301 8201 6400 0400 7d0b 0400 7d0d 7d0c  ....d...}...}.}.
+00000890: 7c0a 641c 1900 7d0b 7c0b 7c05 6b02 7d0d  |.d...}.|.|.k.}.
+000008a0: 7c0d 73f5 7414 a015 6417 7c0d 6601 641d  |.s.t...d.|.f.d.
+000008b0: 7c0b 7c05 6602 a104 7414 a016 7c0b a101  |.|.f...t...|...
+000008c0: 641c 7419 a01a a100 7600 73de 7414 a01b  d.t.....v.s.t...
+000008d0: 7c05 a101 72e3 7414 a016 7c05 a101 6e01  |...r.t...|...n.
+000008e0: 641c 641e 9c02 1600 7d10 641f 6420 7c10  d.d.....}.d.d |.
+000008f0: 6901 1600 7d11 7417 7414 a018 7c11 a101  i...}.t.t...|...
+00000900: 8301 8201 6400 0400 7d0b 7d0d 740f a010  ....d...}.}.t...
+00000910: 7c06 a011 a100 a101 740f a010 7c07 a011  |.......t...|...
+00000920: a100 a101 740f a010 7c08 a011 a100 a101  ....t...|.......
+00000930: 740f a010 7c09 a011 a100 a101 6704 7c04  t...|.......g.|.
+00000940: 5f12 7c03 6a13 7c01 6421 6422 8d02 4900  _.|.j.|.d!d"..I.
+00000950: 6400 4800 7d0a 7c0a 6416 1900 7d0b 6407  d.H.}.|.d...}.d.
+00000960: 7d0c 7c0b 7c0c 6b02 7d0d 7c0d 9001 734e  }.|.|.k.}.|...sN
+00000970: 7414 a015 6417 7c0d 6601 6418 7c0b 7c0c  t...d.|.f.d.|.|.
+00000980: 6602 a104 7414 a016 7c0b a101 7414 a016  f...t...|...t...
+00000990: 7c0c a101 6419 9c02 1600 7d0e 641a 641b  |...d.....}.d.d.
+000009a0: 7c0e 6901 1600 7d0f 7417 7414 a018 7c0f  |.i...}.t.t...|.
+000009b0: a101 8301 8201 6400 0400 7d0b 0400 7d0d  ......d...}...}.
+000009c0: 7d0c 7c0a 641c 1900 7d0b 7c05 6400 6412  }.|.d...}.|.d.d.
+000009d0: 8502 1900 7d0c 7c0b 7c0c 6b02 7d0d 7c0d  ....}.|.|.k.}.|.
+000009e0: 9001 7388 7414 a015 6417 7c0d 6601 6418  ..s.t...d.|.f.d.
+000009f0: 7c0b 7c0c 6602 a104 7414 a016 7c0b a101  |.|.f...t...|...
+00000a00: 7414 a016 7c0c a101 6419 9c02 1600 7d0e  t...|...d.....}.
+00000a10: 641a 641b 7c0e 6901 1600 7d0f 7417 7414  d.d.|.i...}.t.t.
+00000a20: a018 7c0f a101 8301 8201 6400 0400 7d0b  ..|.......d...}.
+00000a30: 0400 7d0d 7d0c 6400 5300 2923 4e72 0800  ..}.}.d.S.)#Nr..
+00000a40: 0000 7209 0000 0072 0a00 0000 720b 0000  ..r....r....r...
+00000a50: 0063 0100 0000 0000 0000 0000 0000 0200  .c..............
+00000a60: 0000 0400 0000 5300 0000 720d 0000 0072  ......S...r....r
+00000a70: 0e00 0000 7210 0000 0072 1100 0000 7210  ....r....r....r.
+00000a80: 0000 0072 1000 0000 7214 0000 0072 1500  ...r....r....r..
+00000a90: 0000 3800 0000 7216 0000 007a 4174 6573  ..8...r....zAtes
+00000aa0: 745f 6163 7469 7669 7479 5f70 7562 5f63  t_activity_pub_c
+00000ab0: 6c69 656e 745f 6765 745f 636f 6c6c 6563  lient_get_collec
+00000ac0: 7469 6f6e 5f70 6167 6573 2e3c 6c6f 6361  tion_pages.<loca
+00000ad0: 6c73 3e2e 3c6c 6973 7463 6f6d 703e e917  ls>.<listcomp>..
+00000ae0: 0000 0072 1800 0000 da05 6669 7273 74da  ...r......first.
+00000af0: 046c 6173 7429 0472 0f00 0000 7219 0000  .last).r....r...
+00000b00: 0072 4b00 0000 724c 0000 00da 0670 6167  .rK...rL.....pag
+00000b10: 655f 31e9 0d00 0000 5a05 7572 6c5f 315a  e_1.....Z.url_1Z
+00000b20: 066e 6578 745f 3129 0472 0f00 0000 721a  .next_1).r....r.
+00000b30: 0000 00da 0770 6172 745f 6f66 da04 6e65  .....part_of..ne
+00000b40: 7874 da06 7061 6765 5f32 e914 0000 005a  xt..page_2.....Z
+00000b50: 066e 6578 745f 32da 0670 6167 655f 3329  .next_2..page_3)
+00000b60: 0372 0f00 0000 721a 0000 0072 4f00 0000  .r....r....rO...
+00000b70: 721b 0000 0072 1c00 0000 721e 0000 0072  r....r....r....r
+00000b80: 1f00 0000 7222 0000 0072 2300 0000 721a  ....r"...r#...r.
+00000b90: 0000 0072 2400 0000 7225 0000 0072 2700  ...r$...r%...r'.
+00000ba0: 0000 7228 0000 00e9 1100 0000 2901 da09  ..r(........)...
+00000bb0: 6d61 785f 6974 656d 7329 1c72 0200 0000  max_items).r....
+00000bc0: 7229 0000 0072 2a00 0000 722b 0000 0072  r)...r*...r+...r
+00000bd0: 0400 0000 722c 0000 0072 2d00 0000 7207  ....r,...r-...r.
+00000be0: 0000 0072 0300 0000 722e 0000 0072 2f00  ...r....r....r/.
+00000bf0: 0000 7230 0000 0072 3100 0000 7205 0000  ..r0...r1...r...
+00000c00: 0072 0600 0000 7232 0000 0072 3300 0000  .r....r2...r3...
+00000c10: 7234 0000 005a 0b73 6964 655f 6566 6665  r4...Z.side_effe
+00000c20: 6374 7235 0000 0072 3600 0000 7237 0000  ctr5...r6...r7..
+00000c30: 0072 3800 0000 7239 0000 0072 3a00 0000  .r8...r9...r:...
+00000c40: 723b 0000 0072 3c00 0000 723d 0000 0029  r;...r<...r=...)
+00000c50: 1272 0c00 0000 7218 0000 0072 0900 0000  .r....r....r....
+00000c60: 723e 0000 0072 3f00 0000 721a 0000 0072  r>...r?...r....r
+00000c70: 4000 0000 724d 0000 0072 5100 0000 7253  @...rM...rQ...rS
+00000c80: 0000 0072 4100 0000 7242 0000 0072 4300  ...rA...rB...rC.
+00000c90: 0000 7244 0000 0072 4500 0000 7246 0000  ..rD...rE...rF..
+00000ca0: 0072 4700 0000 7248 0000 0072 1000 0000  .rG...rH...r....
+00000cb0: 7210 0000 0072 1400 0000 da2d 7465 7374  r....r.....-test
+00000cc0: 5f61 6374 6976 6974 795f 7075 625f 636c  _activity_pub_cl
+00000cd0: 6965 6e74 5f67 6574 5f63 6f6c 6c65 6374  ient_get_collect
+00000ce0: 696f 6e5f 7061 6765 7328 0000 0073 4e00  ion_pages(...sN.
+00000cf0: 0000 0280 0a01 0401 0401 0a01 0801 0603  ................
+00000d00: 0601 0801 04fe 02ff 0605 0e01 0a01 1202  ................
+00000d10: 1002 0201 1001 06ff 0203 1001 06ff 1603  ................
+00000d20: 0c03 0c01 0c01 0c01 06fc 1007 6a02 7c01  ............j.|.
+00000d30: 0c03 0c01 0c01 0c01 06fc 1407 6c02 7801  ............l.x.
+00000d40: 7256 0000 0029 14da 0862 7569 6c74 696e  rV...)...builtin
+00000d50: 7372 3b00 0000 da19 5f70 7974 6573 742e  sr;....._pytest.
+00000d60: 6173 7365 7274 696f 6e2e 7265 7772 6974  assertion.rewrit
+00000d70: 65da 0961 7373 6572 7469 6f6e da07 7265  e..assertion..re
+00000d80: 7772 6974 6572 3600 0000 7232 0000 005a  writer6...r2...Z
+00000d90: 0d75 6e69 7474 6573 742e 6d6f 636b 7202  .unittest.mockr.
+00000da0: 0000 0072 0300 0000 7229 0000 00da 0662  ...r....r).....b
+00000db0: 6f76 696e 6572 0400 0000 5a16 626f 7669  oviner....Z.bovi
+00000dc0: 6e65 2e61 6374 6976 6974 7973 7472 6561  ne.activitystrea
+00000dd0: 6d73 7205 0000 0072 0600 0000 5a12 626f  msr....r....Z.bo
+00000de0: 7669 6e65 2e63 7279 7074 6f2e 7465 7374  vine.crypto.test
+00000df0: 7207 0000 0072 4900 0000 7256 0000 0072  r....rI...rV...r
+00000e00: 1000 0000 7210 0000 0072 1000 0000 7214  ....r....r....r.
+00000e10: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
+00000e20: 0073 1000 0000 2200 1001 0802 0c02 1001  .s....".........
+00000e30: 0c01 0803 0c1d                           ......
```

### Comparing `bovine-0.1.0/bovine/activitypub/authorization_wrapper.py` & `bovine-0.1.1/bovine/activitypub/authorization_wrapper.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.0/bovine/activitypub/collection_helper.py` & `bovine-0.1.1/bovine/activitypub/collection_helper.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.0/bovine/activitypub/test_actor.py` & `bovine-0.1.1/bovine/activitypub/test_actor.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 import json
 from unittest.mock import AsyncMock, MagicMock
 
 import aiohttp
 
 from bovine import BovineActor
-from bovine.activitystreams import (
-    build_ordered_collection,
-    build_ordered_collection_page,
-)
+from bovine.activitystreams import OrderedCollection, OrderedCollectionPage
 from bovine.crypto.test import private_key
 
 
 async def test_activity_pub_client_get_collection_no_pages():
     session = AsyncMock(aiohttp.ClientSession)
     url = "https://test_domain/test_path"
     public_key_url = "public_key_url"
@@ -26,16 +23,15 @@
 
     text_mock = AsyncMock()
     session.get.return_value = MagicMock(aiohttp.ClientResponse)
     session.get.return_value.text = text_mock
 
     items = [{"id": j} for j in range(7)]
 
-    builder = build_ordered_collection("url").with_count(7).with_items(items)
-
+    builder = OrderedCollection(id="url", count=7, items=items)
     text_mock.return_value = json.dumps(builder.build())
 
     result = await actor.get_ordered_collection(url)
     session.get.assert_awaited_once()
 
     assert result["total_items"] == 7
     assert result["items"] == items
@@ -55,31 +51,22 @@
     )
     text_mock = AsyncMock()
     session.get.return_value = MagicMock(aiohttp.ClientResponse)
     session.get.return_value.text = text_mock
 
     items = [{"id": j} for j in range(23)]
 
-    builder = (
-        build_ordered_collection("url")
-        .with_count(23)
-        .with_first_and_last("first", "last")
-    )
-
-    page_1 = (
-        build_ordered_collection_page("url_1", "page_1")
-        .with_items(items[:13])
-        .with_next("next_1")
+    builder = OrderedCollection(id="url", count=23, first="first", last="last")
+    page_1 = OrderedCollectionPage(
+        id="page_1", items=items[:13], part_of="url_1", next="next_1"
     )
-    page_2 = (
-        build_ordered_collection_page("url_1", "page_2")
-        .with_items(items[13:20])
-        .with_next("next_2")
+    page_2 = OrderedCollectionPage(
+        id="page_2", items=items[13:20], part_of="url_1", next="next_2"
     )
-    page_3 = build_ordered_collection_page("url_1", "page_2").with_items(items[20:])
+    page_3 = OrderedCollectionPage(id="page_3", items=items[20:], part_of="url_1")
 
     text_mock.side_effect = [
         json.dumps(builder.build()),
         json.dumps(page_1.build()),
         json.dumps(page_2.build()),
         json.dumps(page_3.build()),
     ]
```

### Comparing `bovine-0.1.0/bovine/activitystreams/__init__.py` & `bovine-0.1.1/bovine/activitystreams/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,20 @@
 from dataclasses import dataclass
-from typing import Optional
+from typing import Optional, Tuple
 
 from bovine.types import Visibility
 
 from .activity_factory import ActivityFactory
 from .object_factory import ObjectFactory
-from .ordered_collection_builder import OrderedCollectionBuilder
-from .ordered_collection_page_builder import OrderedCollectionPageBuilder
 
 
-def build_ordered_collection(url: str):
-    return OrderedCollectionBuilder(url)
-
-
-def build_ordered_collection_page(url: str, part_of: str):
-    return OrderedCollectionPageBuilder(url, part_of)
-
-
-def factories_for_actor_object(actor_object):
+def factories_for_actor_object(
+    actor_object: dict,
+) -> Tuple[ActivityFactory, ObjectFactory]:
+    """Builds activity and object factories from actor object"""
     return ActivityFactory(actor_object), ObjectFactory(actor_information=actor_object)
 
 
 @dataclass
 class Actor:
     """Actor class represents the basic ActivityStreams actor."""
 
@@ -124,7 +117,61 @@
     def _build_user_endpoints(self):
         endpoints = {}
         if self.event_source:
             endpoints["eventSource"] = self.event_source
         if self.proxy_url:
             endpoints["proxyUrl"] = self.proxy_url
         return endpoints
+
+
+@dataclass
+class OrderedCollection:
+    id: str
+    items: list | None = None
+    count: int = 0
+    first: str | None = None
+    last: str | None = None
+
+    def build(self) -> dict:
+        result = {
+            "@context": "https://www.w3.org/ns/activitystreams",
+            "id": self.id,
+            "totalItems": self.count,
+            "type": "OrderedCollection",
+        }
+
+        if self.items:
+            result["orderedItems"] = self.items
+
+        if self.first:
+            result["first"] = self.first
+
+        if self.last:
+            result["last"] = self.last
+
+        return result
+
+
+@dataclass
+class OrderedCollectionPage:
+    id: str
+    items: list
+    part_of: str
+    next: str | None = None
+    prev: str | None = None
+
+    def build(self) -> dict:
+        result = {
+            "@context": "https://www.w3.org/ns/activitystreams",
+            "id": self.id,
+            "partOf": self.part_of,
+            "orderedItems": self.items,
+            "type": "OrderedCollectionPage",
+        }
+
+        if self.next:
+            result["next"] = self.next
+
+        if self.prev:
+            result["prev"] = self.prev
+
+        return result
```

### Comparing `bovine-0.1.0/bovine/activitystreams/__pycache__/__init__.cpython-310.pyc` & `bovine-0.1.1/bovine/activitystreams/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 13 15:55:57 2023 UTC, .py size: 3664 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 27% similar despite different names*

```diff
@@ -1,212 +1,264 @@
-00000000: 6f0d 0d0a 0000 0000 0d26 3864 500e 0000  o........&8dP...
+00000000: 6f0d 0d0a 0000 0000 a4ea 3a64 0f12 0000  o.........:d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 9200 0000 6400  .....@...s....d.
+00000020: 0006 0000 0040 0000 0073 9400 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
-00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
-00000050: 0100 6404 6405 6c06 6d07 5a07 0100 6404  ..d.d.l.m.Z...d.
-00000060: 6406 6c08 6d09 5a09 0100 6404 6407 6c0a  d.l.m.Z...d.d.l.
-00000070: 6d0b 5a0b 0100 6404 6408 6c0c 6d0d 5a0d  m.Z...d.d.l.m.Z.
-00000080: 0100 6409 650e 6602 640a 640b 8404 5a0f  ..d.e.f.d.d...Z.
-00000090: 6409 650e 640c 650e 6604 640d 640e 8404  d.e.d.e.f.d.d...
-000000a0: 5a10 640f 6410 8400 5a11 6501 4700 6411  Z.d.d...Z.e.G.d.
-000000b0: 6412 8400 6412 8302 8301 5a12 6413 5300  d...d.....Z.d.S.
-000000c0: 2914 e900 0000 0029 01da 0964 6174 6163  )......)...datac
-000000d0: 6c61 7373 2901 da08 4f70 7469 6f6e 616c  lass)...Optional
-000000e0: 2901 da0a 5669 7369 6269 6c69 7479 e901  )...Visibility..
-000000f0: 0000 0029 01da 0f41 6374 6976 6974 7946  ...)...ActivityF
-00000100: 6163 746f 7279 2901 da0d 4f62 6a65 6374  actory)...Object
-00000110: 4661 6374 6f72 79a9 01da 184f 7264 6572  Factory....Order
-00000120: 6564 436f 6c6c 6563 7469 6f6e 4275 696c  edCollectionBuil
-00000130: 6465 72a9 01da 1c4f 7264 6572 6564 436f  der....OrderedCo
-00000140: 6c6c 6563 7469 6f6e 5061 6765 4275 696c  llectionPageBuil
-00000150: 6465 72da 0375 726c 6301 0000 0000 0000  der..urlc.......
-00000160: 0000 0000 0001 0000 0002 0000 0043 0000  .............C..
-00000170: 0073 0800 0000 7400 7c00 8301 5300 a901  .s....t.|...S...
-00000180: 4e72 0800 0000 2901 720c 0000 00a9 0072  Nr....).r......r
-00000190: 0e00 0000 fa53 2f77 6f6f 6470 6563 6b65  .....S/woodpecke
-000001a0: 722f 7372 632f 636f 6465 6265 7267 2e6f  r/src/codeberg.o
-000001b0: 7267 2f68 656c 6765 2f62 6f76 696e 652f  rg/helge/bovine/
-000001c0: 626f 7669 6e65 2f62 6f76 696e 652f 6163  bovine/bovine/ac
-000001d0: 7469 7669 7479 7374 7265 616d 732f 5f5f  tivitystreams/__
-000001e0: 696e 6974 5f5f 2e70 79da 1862 7569 6c64  init__.py..build
-000001f0: 5f6f 7264 6572 6564 5f63 6f6c 6c65 6374  _ordered_collect
-00000200: 696f 6e0c 0000 0073 0200 0000 0801 7210  ion....s......r.
-00000210: 0000 00da 0770 6172 745f 6f66 6302 0000  .....part_ofc...
-00000220: 0000 0000 0000 0000 0002 0000 0003 0000  ................
-00000230: 0043 0000 0073 0a00 0000 7400 7c00 7c01  .C...s....t.|.|.
-00000240: 8302 5300 720d 0000 0072 0a00 0000 2902  ..S.r....r....).
-00000250: 720c 0000 0072 1100 0000 720e 0000 0072  r....r....r....r
-00000260: 0e00 0000 720f 0000 00da 1d62 7569 6c64  ....r......build
-00000270: 5f6f 7264 6572 6564 5f63 6f6c 6c65 6374  _ordered_collect
-00000280: 696f 6e5f 7061 6765 1000 0000 7302 0000  ion_page....s...
-00000290: 000a 0172 1200 0000 6301 0000 0000 0000  ...r....c.......
-000002a0: 0000 0000 0001 0000 0004 0000 0043 0000  .............C..
-000002b0: 0073 1200 0000 7400 7c00 8301 7401 7c00  .s....t.|...t.|.
-000002c0: 6401 8d01 6602 5300 2902 4e29 015a 1161  d...f.S.).N).Z.a
-000002d0: 6374 6f72 5f69 6e66 6f72 6d61 7469 6f6e  ctor_information
-000002e0: 2902 7206 0000 0072 0700 0000 2901 5a0c  ).r....r....).Z.
-000002f0: 6163 746f 725f 6f62 6a65 6374 720e 0000  actor_objectr...
-00000300: 0072 0e00 0000 720f 0000 00da 1a66 6163  .r....r......fac
-00000310: 746f 7269 6573 5f66 6f72 5f61 6374 6f72  tories_for_actor
-00000320: 5f6f 626a 6563 7414 0000 0073 0200 0000  _object....s....
-00000330: 1201 7213 0000 0063 0000 0000 0000 0000  ..r....c........
-00000340: 0000 0000 0000 0000 0300 0000 4000 0000  ............@...
-00000350: 7314 0100 0065 005a 0164 005a 0255 0064  s....e.Z.d.Z.U.d
-00000360: 015a 0365 0465 0564 023c 0064 035a 0665  .Z.e.e.d.<.d.Z.e
-00000370: 0465 0564 043c 0064 055a 0765 0865 0419  .e.d.<.d.Z.e.e..
-00000380: 0065 0564 063c 0064 055a 0965 0865 0419  .e.d.<.d.Z.e.e..
-00000390: 0065 0564 073c 0064 055a 0a65 0865 0419  .e.d.<.d.Z.e.e..
-000003a0: 0065 0564 083c 0064 055a 0b65 0865 0419  .e.d.<.d.Z.e.e..
-000003b0: 0065 0564 093c 0064 055a 0c65 0865 0419  .e.d.<.d.Z.e.e..
-000003c0: 0065 0564 0a3c 0064 055a 0d65 0865 0419  .e.d.<.d.Z.e.e..
-000003d0: 0065 0564 0b3c 0064 055a 0e65 0865 0419  .e.d.<.d.Z.e.e..
-000003e0: 0065 0564 0c3c 0064 055a 0f65 0865 0419  .e.d.<.d.Z.e.e..
-000003f0: 0065 0564 0d3c 0064 055a 1065 0865 0419  .e.d.<.d.Z.e.e..
-00000400: 0065 0564 0e3c 0064 055a 1165 0865 0419  .e.d.<.d.Z.e.e..
-00000410: 0065 0564 0f3c 0064 055a 1265 0865 0419  .e.d.<.d.Z.e.e..
-00000420: 0065 0564 103c 0064 055a 1365 0865 1419  .e.d.<.d.Z.e.e..
-00000430: 0065 0564 113c 0065 156a 1666 0164 1264  .e.d.<.e.j.f.d.d
-00000440: 1384 015a 1764 1464 1584 005a 1864 1664  ...Z.d.d...Z.d.d
-00000450: 1784 005a 1964 1864 1984 005a 1a64 1a64  ...Z.d.d...Z.d.d
-00000460: 1b84 005a 1b64 0553 0029 1cda 0541 6374  ...Z.d.S.)...Act
-00000470: 6f72 7a37 4163 746f 7220 636c 6173 7320  orz7Actor class 
-00000480: 7265 7072 6573 656e 7473 2074 6865 2062  represents the b
-00000490: 6173 6963 2041 6374 6976 6974 7953 7472  asic ActivityStr
-000004a0: 6561 6d73 2061 6374 6f72 2eda 0269 645a  eams actor...idZ
-000004b0: 0650 6572 736f 6eda 0474 7970 654e da04  .Person..typeN..
-000004c0: 6e61 6d65 da12 7072 6566 6572 7265 645f  name..preferred_
-000004d0: 7573 6572 6e61 6d65 da05 696e 626f 78da  username..inbox.
-000004e0: 066f 7574 626f 78da 0966 6f6c 6c6f 7765  .outbox..followe
-000004f0: 7273 da09 666f 6c6c 6f77 696e 67da 0a70  rs..following..p
-00000500: 7562 6c69 635f 6b65 79da 0f70 7562 6c69  ublic_key..publi
-00000510: 635f 6b65 795f 6e61 6d65 da0c 6576 656e  c_key_name..even
-00000520: 745f 736f 7572 6365 da09 7072 6f78 795f  t_source..proxy_
-00000530: 7572 6cda 0773 756d 6d61 7279 da04 6963  url..summary..ic
-00000540: 6f6e 6302 0000 0000 0000 0000 0000 0005  onc.............
-00000550: 0000 0004 0000 0043 0000 0073 9800 0000  .......C...s....
-00000560: 7c00 a000 a100 7c00 6a01 7c00 6a02 6401  |.....|.j.|.j.d.
-00000570: 9c03 7c00 a003 a100 a501 7c00 6a04 7c01  ..|.......|.j.|.
-00000580: 6402 8d01 a501 7d02 7c00 6a05 721c 7c00  d.....}.|.j.r.|.
-00000590: 6a05 7c02 6403 3c00 7c01 7406 6a07 6b02  j.|.d.<.|.t.j.k.
-000005a0: 7223 7c02 5300 7c00 6a08 722c 7c00 6a08  r#|.S.|.j.r,|.j.
-000005b0: 7c02 6404 3c00 6e08 7c00 6a05 7234 7c00  |.d.<.n.|.j.r4|.
-000005c0: 6a05 7c02 6404 3c00 7c00 6a09 7c00 6a0a  j.|.d.<.|.j.|.j.
-000005d0: 6405 9c02 a00b a100 4400 5d0c 5c02 7d03  d.......D.].\.}.
-000005e0: 7d04 7c04 6406 7501 7249 7c04 7c02 7c03  }.|.d.u.rI|.|.|.
-000005f0: 3c00 713d 7c02 5300 2907 7a30 4372 6561  <.q=|.S.).z0Crea
-00000600: 7465 7320 7468 6520 6a73 6f6e 2d6c 6420  tes the json-ld 
-00000610: 7265 7072 6573 656e 7461 7469 6f6e 206f  representation o
-00000620: 6620 7468 6520 6163 746f 722e 2903 7a08  f the actor.).z.
-00000630: 4063 6f6e 7465 7874 7215 0000 0072 1600  @contextr....r..
-00000640: 0000 2901 da0a 7669 7369 6269 6c69 7479  ..)...visibility
-00000650: 5a11 7072 6566 6572 7265 6455 7365 726e  Z.preferredUsern
-00000660: 616d 6572 1700 0000 2902 7221 0000 0072  amer....).r!...r
-00000670: 2200 0000 4e29 0cda 0e5f 6275 696c 645f  "...N)..._build_
-00000680: 636f 6e74 6578 7472 1500 0000 7216 0000  contextr....r...
-00000690: 00da 115f 6275 696c 645f 7075 626c 6963  ..._build_public
-000006a0: 5f6b 6579 da10 5f62 7569 6c64 5f65 6e64  _key.._build_end
-000006b0: 706f 696e 7473 7218 0000 0072 0400 0000  pointsr....r....
-000006c0: da03 5745 4272 1700 0000 7221 0000 0072  ..WEBr....r!...r
-000006d0: 2200 0000 da05 6974 656d 7329 05da 0473  ".....items)...s
-000006e0: 656c 6672 2300 0000 da06 7265 7375 6c74  elfr#.....result
-000006f0: da03 6b65 79da 0576 616c 7565 720e 0000  ..key..valuer...
-00000700: 0072 0e00 0000 720f 0000 00da 0562 7569  .r....r......bui
-00000710: 6c64 2c00 0000 7332 0000 0006 0304 0104  ld,...s2........
-00000720: 0104 fd06 0402 fc0a 0504 fb06 080a 010a  ................
-00000730: 0204 0106 020c 0106 010a 0104 0304 0104  ................
-00000740: fe04 030a fd08 0408 0102 8004 027a 0b41  .............z.A
-00000750: 6374 6f72 2e62 7569 6c64 6301 0000 0000  ctor.buildc.....
-00000760: 0000 0000 0000 0001 0000 0002 0000 0043  ...............C
-00000770: 0000 0073 1200 0000 7c00 6a00 7207 6401  ...s....|.j.r.d.
-00000780: 6402 6702 5300 6401 5300 2903 4e7a 2568  d.g.S.d.S.).Nz%h
-00000790: 7474 7073 3a2f 2f77 7777 2e77 332e 6f72  ttps://www.w3.or
-000007a0: 672f 6e73 2f61 6374 6976 6974 7973 7472  g/ns/activitystr
-000007b0: 6561 6d73 7a1c 6874 7470 733a 2f2f 7733  eamsz.https://w3
-000007c0: 6964 2e6f 7267 2f73 6563 7572 6974 792f  id.org/security/
-000007d0: 7631 2901 721d 0000 00a9 0172 2900 0000  v1).r......r)...
-000007e0: 720e 0000 0072 0e00 0000 720f 0000 0072  r....r....r....r
-000007f0: 2400 0000 4a00 0000 730a 0000 0006 0102  $...J...s.......
-00000800: 0202 0104 fe04 057a 1441 6374 6f72 2e5f  .......z.Actor._
-00000810: 6275 696c 645f 636f 6e74 6578 7463 0100  build_contextc..
-00000820: 0000 0000 0000 0000 0000 0100 0000 0500  ................
-00000830: 0000 4300 0000 732c 0000 007c 006a 0072  ..C...s,...|.j.r
-00000840: 1464 017c 006a 019b 0064 027c 006a 029b  .d.|.j...d.|.j..
-00000850: 009d 037c 006a 017c 006a 0064 039c 0369  ...|.j.|.j.d...i
-00000860: 0153 0069 0053 0029 044e 5a09 7075 626c  .S.i.S.).NZ.publ
-00000870: 6963 4b65 79fa 0123 2903 7215 0000 00da  icKey..#).r.....
-00000880: 056f 776e 6572 5a0c 7075 626c 6963 4b65  .ownerZ.publicKe
-00000890: 7950 656d 2903 721d 0000 0072 1500 0000  yPem).r....r....
-000008a0: 721e 0000 0072 2e00 0000 720e 0000 0072  r....r....r....r
-000008b0: 0e00 0000 720f 0000 0072 2500 0000 5300  ....r....r%...S.
-000008c0: 0000 7310 0000 0006 0102 0210 0104 0104  ..s.............
-000008d0: 0104 fd04 ff04 077a 1741 6374 6f72 2e5f  .......z.Actor._
-000008e0: 6275 696c 645f 7075 626c 6963 5f6b 6579  build_public_key
-000008f0: 6302 0000 0000 0000 0000 0000 0004 0000  c...............
-00000900: 0003 0000 0043 0000 0073 9000 0000 6900  .....C...s....i.
-00000910: 7d02 7c01 7400 6a01 6b02 7209 7c02 5300  }.|.t.j.k.r.|.S.
-00000920: 7c00 6a02 7212 7c00 6a02 7c02 6401 3c00  |.j.r.|.j.|.d.<.
-00000930: 6e05 7c00 6a03 7c02 6401 3c00 7c00 6a04  n.|.j.|.d.<.|.j.
-00000940: 7220 7c00 6a04 7c02 6402 3c00 6e05 7c00  r |.j.|.d.<.n.|.
-00000950: 6a03 7c02 6402 3c00 7c01 7400 6a05 6b03  j.|.d.<.|.t.j.k.
-00000960: 722c 7c02 5300 7c00 a006 a100 7d03 7c03  r,|.S.|.....}.|.
-00000970: 7236 7c03 7c02 6403 3c00 7c00 6a07 723e  r6|.|.d.<.|.j.r>
-00000980: 7c00 6a07 7c02 6404 3c00 7c00 6a08 7246  |.j.|.d.<.|.j.rF
-00000990: 7c00 6a08 7c02 6405 3c00 7c02 5300 2906  |.j.|.d.<.|.S.).
-000009a0: 4e72 1900 0000 721a 0000 00da 0965 6e64  Nr....r......end
-000009b0: 706f 696e 7473 721b 0000 0072 1c00 0000  pointsr....r....
-000009c0: 2909 7204 0000 0072 2700 0000 7219 0000  ).r....r'...r...
-000009d0: 0072 1500 0000 721a 0000 00da 054f 574e  .r....r......OWN
-000009e0: 4552 da15 5f62 7569 6c64 5f75 7365 725f  ER.._build_user_
-000009f0: 656e 6470 6f69 6e74 7372 1b00 0000 721c  endpointsr....r.
-00000a00: 0000 0029 0472 2900 0000 7223 0000 0072  ...).r)...r#...r
-00000a10: 2a00 0000 7231 0000 0072 0e00 0000 720e  *...r1...r....r.
-00000a20: 0000 0072 0f00 0000 7226 0000 005e 0000  ...r....r&...^..
-00000a30: 0073 2600 0000 0401 0a02 0401 0602 0c01  .s&.............
-00000a40: 0a02 0602 0c01 0a02 0a02 0401 0802 0401  ................
-00000a50: 0801 0602 0a01 0601 0a01 0402 7a16 4163  ............z.Ac
-00000a60: 746f 722e 5f62 7569 6c64 5f65 6e64 706f  tor._build_endpo
-00000a70: 696e 7473 6301 0000 0000 0000 0000 0000  intsc...........
-00000a80: 0002 0000 0003 0000 0043 0000 0073 2800  .........C...s(.
-00000a90: 0000 6900 7d01 7c00 6a00 720a 7c00 6a00  ..i.}.|.j.r.|.j.
-00000aa0: 7c01 6401 3c00 7c00 6a01 7212 7c00 6a01  |.d.<.|.j.r.|.j.
-00000ab0: 7c01 6402 3c00 7c01 5300 2903 4eda 0b65  |.d.<.|.S.).N..e
-00000ac0: 7665 6e74 536f 7572 6365 da08 7072 6f78  ventSource..prox
-00000ad0: 7955 726c 2902 721f 0000 0072 2000 0000  yUrl).r....r ...
-00000ae0: 2902 7229 0000 0072 3100 0000 720e 0000  ).r)...r1...r...
-00000af0: 0072 0e00 0000 720f 0000 0072 3300 0000  .r....r....r3...
-00000b00: 7c00 0000 730c 0000 0004 0106 010a 0106  |...s...........
-00000b10: 010a 0104 017a 1b41 6374 6f72 2e5f 6275  .....z.Actor._bu
-00000b20: 696c 645f 7573 6572 5f65 6e64 706f 696e  ild_user_endpoin
-00000b30: 7473 291c da08 5f5f 6e61 6d65 5f5f da0a  ts)...__name__..
-00000b40: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
-00000b50: 616c 6e61 6d65 5f5f da07 5f5f 646f 635f  alname__..__doc_
-00000b60: 5fda 0373 7472 da0f 5f5f 616e 6e6f 7461  _..str..__annota
-00000b70: 7469 6f6e 735f 5f72 1600 0000 7217 0000  tions__r....r...
-00000b80: 0072 0300 0000 7218 0000 0072 1900 0000  .r....r....r....
-00000b90: 721a 0000 0072 1b00 0000 721c 0000 0072  r....r....r....r
-00000ba0: 1d00 0000 721e 0000 0072 1f00 0000 7220  ....r....r....r 
-00000bb0: 0000 0072 2100 0000 7222 0000 00da 0464  ...r!...r".....d
-00000bc0: 6963 7472 0400 0000 da06 5055 424c 4943  ictr......PUBLIC
-00000bd0: 722d 0000 0072 2400 0000 7225 0000 0072  r-...r$...r%...r
-00000be0: 2600 0000 7233 0000 0072 0e00 0000 720e  &...r3...r....r.
-00000bf0: 0000 0072 0e00 0000 720f 0000 0072 1400  ...r....r....r..
-00000c00: 0000 1800 0000 732a 0000 000a 0004 0208  ......s*........
-00000c10: 020c 0110 0110 0110 0110 0110 0110 0110  ................
-00000c20: 0110 0110 0110 0110 0210 010e 0208 1e08  ................
-00000c30: 0908 0b0c 1e72 1400 0000 4e29 13da 0b64  .....r....N)...d
-00000c40: 6174 6163 6c61 7373 6573 7202 0000 00da  ataclassesr.....
-00000c50: 0674 7970 696e 6772 0300 0000 da0c 626f  .typingr......bo
-00000c60: 7669 6e65 2e74 7970 6573 7204 0000 00da  vine.typesr.....
-00000c70: 1061 6374 6976 6974 795f 6661 6374 6f72  .activity_factor
-00000c80: 7972 0600 0000 da0e 6f62 6a65 6374 5f66  yr......object_f
-00000c90: 6163 746f 7279 7207 0000 005a 1a6f 7264  actoryr....Z.ord
-00000ca0: 6572 6564 5f63 6f6c 6c65 6374 696f 6e5f  ered_collection_
-00000cb0: 6275 696c 6465 7272 0900 0000 5a1f 6f72  builderr....Z.or
-00000cc0: 6465 7265 645f 636f 6c6c 6563 7469 6f6e  dered_collection
-00000cd0: 5f70 6167 655f 6275 696c 6465 7272 0b00  _page_builderr..
-00000ce0: 0000 723a 0000 0072 1000 0000 7212 0000  ..r:...r....r...
-00000cf0: 0072 1300 0000 7214 0000 0072 0e00 0000  .r....r....r....
-00000d00: 720e 0000 0072 0e00 0000 720f 0000 00da  r....r....r.....
-00000d10: 083c 6d6f 6475 6c65 3e01 0000 0073 1800  .<module>....s..
-00000d20: 0000 0c00 0c01 0c02 0c02 0c01 0c01 0c01  ................
-00000d30: 0e03 1204 0804 0204 1401                 ..........
+00000040: 6d03 5a03 6d04 5a04 0100 6400 6403 6c05  m.Z.m.Z...d.d.l.
+00000050: 6d06 5a06 0100 6404 6405 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
+00000060: 0100 6404 6406 6c09 6d0a 5a0a 0100 6407  ..d.d.l.m.Z...d.
+00000070: 650b 6408 6504 6508 650a 6602 1900 6604  e.d.e.e.e.f...f.
+00000080: 6409 640a 8404 5a0c 6501 4700 640b 640c  d.d...Z.e.G.d.d.
+00000090: 8400 640c 8302 8301 5a0d 6501 4700 640d  ..d.....Z.e.G.d.
+000000a0: 640e 8400 640e 8302 8301 5a0e 6501 4700  d...d.....Z.e.G.
+000000b0: 640f 6410 8400 6410 8302 8301 5a0f 6411  d.d...d.....Z.d.
+000000c0: 5300 2912 e900 0000 0029 01da 0964 6174  S.)......)...dat
+000000d0: 6163 6c61 7373 2902 da08 4f70 7469 6f6e  aclass)...Option
+000000e0: 616c da05 5475 706c 6529 01da 0a56 6973  al..Tuple)...Vis
+000000f0: 6962 696c 6974 79e9 0100 0000 2901 da0f  ibility.....)...
+00000100: 4163 7469 7669 7479 4661 6374 6f72 7929  ActivityFactory)
+00000110: 01da 0d4f 626a 6563 7446 6163 746f 7279  ...ObjectFactory
+00000120: da0c 6163 746f 725f 6f62 6a65 6374 da06  ..actor_object..
+00000130: 7265 7475 726e 6301 0000 0000 0000 0000  returnc.........
+00000140: 0000 0001 0000 0004 0000 0043 0000 0073  ...........C...s
+00000150: 1200 0000 7400 7c00 8301 7401 7c00 6401  ....t.|...t.|.d.
+00000160: 8d01 6602 5300 2902 7a36 4275 696c 6473  ..f.S.).z6Builds
+00000170: 2061 6374 6976 6974 7920 616e 6420 6f62   activity and ob
+00000180: 6a65 6374 2066 6163 746f 7269 6573 2066  ject factories f
+00000190: 726f 6d20 6163 746f 7220 6f62 6a65 6374  rom actor object
+000001a0: 2901 5a11 6163 746f 725f 696e 666f 726d  ).Z.actor_inform
+000001b0: 6174 696f 6e29 0272 0700 0000 7208 0000  ation).r....r...
+000001c0: 0029 0172 0900 0000 a900 720b 0000 00fa  .).r......r.....
+000001d0: 542f 776f 6f64 7065 636b 6572 2f73 7263  T/woodpecker/src
+000001e0: 2f63 6f64 6562 6572 672e 6f72 672f 626f  /codeberg.org/bo
+000001f0: 7669 6e65 2f62 6f76 696e 652f 626f 7669  vine/bovine/bovi
+00000200: 6e65 2f62 6f76 696e 652f 6163 7469 7669  ne/bovine/activi
+00000210: 7479 7374 7265 616d 732f 5f5f 696e 6974  tystreams/__init
+00000220: 5f5f 2e70 79da 1a66 6163 746f 7269 6573  __.py..factories
+00000230: 5f66 6f72 5f61 6374 6f72 5f6f 626a 6563  _for_actor_objec
+00000240: 740a 0000 0073 0200 0000 1204 720d 0000  t....s......r...
+00000250: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
+00000260: 0000 0300 0000 4000 0000 7314 0100 0065  ......@...s....e
+00000270: 005a 0164 005a 0255 0064 015a 0365 0465  .Z.d.Z.U.d.Z.e.e
+00000280: 0564 023c 0064 035a 0665 0465 0564 043c  .d.<.d.Z.e.e.d.<
+00000290: 0064 055a 0765 0865 0419 0065 0564 063c  .d.Z.e.e...e.d.<
+000002a0: 0064 055a 0965 0865 0419 0065 0564 073c  .d.Z.e.e...e.d.<
+000002b0: 0064 055a 0a65 0865 0419 0065 0564 083c  .d.Z.e.e...e.d.<
+000002c0: 0064 055a 0b65 0865 0419 0065 0564 093c  .d.Z.e.e...e.d.<
+000002d0: 0064 055a 0c65 0865 0419 0065 0564 0a3c  .d.Z.e.e...e.d.<
+000002e0: 0064 055a 0d65 0865 0419 0065 0564 0b3c  .d.Z.e.e...e.d.<
+000002f0: 0064 055a 0e65 0865 0419 0065 0564 0c3c  .d.Z.e.e...e.d.<
+00000300: 0064 055a 0f65 0865 0419 0065 0564 0d3c  .d.Z.e.e...e.d.<
+00000310: 0064 055a 1065 0865 0419 0065 0564 0e3c  .d.Z.e.e...e.d.<
+00000320: 0064 055a 1165 0865 0419 0065 0564 0f3c  .d.Z.e.e...e.d.<
+00000330: 0064 055a 1265 0865 0419 0065 0564 103c  .d.Z.e.e...e.d.<
+00000340: 0064 055a 1365 0865 1419 0065 0564 113c  .d.Z.e.e...e.d.<
+00000350: 0065 156a 1666 0164 1264 1384 015a 1764  .e.j.f.d.d...Z.d
+00000360: 1464 1584 005a 1864 1664 1784 005a 1964  .d...Z.d.d...Z.d
+00000370: 1864 1984 005a 1a64 1a64 1b84 005a 1b64  .d...Z.d.d...Z.d
+00000380: 0553 0029 1cda 0541 6374 6f72 7a37 4163  .S.)...Actorz7Ac
+00000390: 746f 7220 636c 6173 7320 7265 7072 6573  tor class repres
+000003a0: 656e 7473 2074 6865 2062 6173 6963 2041  ents the basic A
+000003b0: 6374 6976 6974 7953 7472 6561 6d73 2061  ctivityStreams a
+000003c0: 6374 6f72 2eda 0269 645a 0650 6572 736f  ctor...idZ.Perso
+000003d0: 6eda 0474 7970 654e da04 6e61 6d65 da12  n..typeN..name..
+000003e0: 7072 6566 6572 7265 645f 7573 6572 6e61  preferred_userna
+000003f0: 6d65 da05 696e 626f 78da 066f 7574 626f  me..inbox..outbo
+00000400: 78da 0966 6f6c 6c6f 7765 7273 da09 666f  x..followers..fo
+00000410: 6c6c 6f77 696e 67da 0a70 7562 6c69 635f  llowing..public_
+00000420: 6b65 79da 0f70 7562 6c69 635f 6b65 795f  key..public_key_
+00000430: 6e61 6d65 da0c 6576 656e 745f 736f 7572  name..event_sour
+00000440: 6365 da09 7072 6f78 795f 7572 6cda 0773  ce..proxy_url..s
+00000450: 756d 6d61 7279 da04 6963 6f6e 6302 0000  ummary..iconc...
+00000460: 0000 0000 0000 0000 0005 0000 0004 0000  ................
+00000470: 0043 0000 0073 9800 0000 7c00 a000 a100  .C...s....|.....
+00000480: 7c00 6a01 7c00 6a02 6401 9c03 7c00 a003  |.j.|.j.d...|...
+00000490: a100 a501 7c00 6a04 7c01 6402 8d01 a501  ....|.j.|.d.....
+000004a0: 7d02 7c00 6a05 721c 7c00 6a05 7c02 6403  }.|.j.r.|.j.|.d.
+000004b0: 3c00 7c01 7406 6a07 6b02 7223 7c02 5300  <.|.t.j.k.r#|.S.
+000004c0: 7c00 6a08 722c 7c00 6a08 7c02 6404 3c00  |.j.r,|.j.|.d.<.
+000004d0: 6e08 7c00 6a05 7234 7c00 6a05 7c02 6404  n.|.j.r4|.j.|.d.
+000004e0: 3c00 7c00 6a09 7c00 6a0a 6405 9c02 a00b  <.|.j.|.j.d.....
+000004f0: a100 4400 5d0c 5c02 7d03 7d04 7c04 6406  ..D.].\.}.}.|.d.
+00000500: 7501 7249 7c04 7c02 7c03 3c00 713d 7c02  u.rI|.|.|.<.q=|.
+00000510: 5300 2907 7a30 4372 6561 7465 7320 7468  S.).z0Creates th
+00000520: 6520 6a73 6f6e 2d6c 6420 7265 7072 6573  e json-ld repres
+00000530: 656e 7461 7469 6f6e 206f 6620 7468 6520  entation of the 
+00000540: 6163 746f 722e 2903 fa08 4063 6f6e 7465  actor.)...@conte
+00000550: 7874 720f 0000 0072 1000 0000 2901 da0a  xtr....r....)...
+00000560: 7669 7369 6269 6c69 7479 5a11 7072 6566  visibilityZ.pref
+00000570: 6572 7265 6455 7365 726e 616d 6572 1100  erredUsernamer..
+00000580: 0000 2902 721b 0000 0072 1c00 0000 4e29  ..).r....r....N)
+00000590: 0cda 0e5f 6275 696c 645f 636f 6e74 6578  ..._build_contex
+000005a0: 7472 0f00 0000 7210 0000 00da 115f 6275  tr....r......_bu
+000005b0: 696c 645f 7075 626c 6963 5f6b 6579 da10  ild_public_key..
+000005c0: 5f62 7569 6c64 5f65 6e64 706f 696e 7473  _build_endpoints
+000005d0: 7212 0000 0072 0500 0000 da03 5745 4272  r....r......WEBr
+000005e0: 1100 0000 721b 0000 0072 1c00 0000 da05  ....r....r......
+000005f0: 6974 656d 7329 05da 0473 656c 6672 1e00  items)...selfr..
+00000600: 0000 da06 7265 7375 6c74 da03 6b65 79da  ....result..key.
+00000610: 0576 616c 7565 720b 0000 0072 0b00 0000  .valuer....r....
+00000620: 720c 0000 00da 0562 7569 6c64 2500 0000  r......build%...
+00000630: 7332 0000 0006 0304 0104 0104 fd06 0402  s2..............
+00000640: fc0a 0504 fb06 080a 010a 0204 0106 020c  ................
+00000650: 0106 010a 0104 0304 0104 fe04 030a fd08  ................
+00000660: 0408 0102 8004 027a 0b41 6374 6f72 2e62  .......z.Actor.b
+00000670: 7569 6c64 6301 0000 0000 0000 0000 0000  uildc...........
+00000680: 0001 0000 0002 0000 0043 0000 0073 1200  .........C...s..
+00000690: 0000 7c00 6a00 7207 6401 6402 6702 5300  ..|.j.r.d.d.g.S.
+000006a0: 6401 5300 2903 4efa 2568 7474 7073 3a2f  d.S.).N.%https:/
+000006b0: 2f77 7777 2e77 332e 6f72 672f 6e73 2f61  /www.w3.org/ns/a
+000006c0: 6374 6976 6974 7973 7472 6561 6d73 7a1c  ctivitystreamsz.
+000006d0: 6874 7470 733a 2f2f 7733 6964 2e6f 7267  https://w3id.org
+000006e0: 2f73 6563 7572 6974 792f 7631 2901 7217  /security/v1).r.
+000006f0: 0000 00a9 0172 2400 0000 720b 0000 0072  .....r$...r....r
+00000700: 0b00 0000 720c 0000 0072 1f00 0000 4300  ....r....r....C.
+00000710: 0000 730a 0000 0006 0102 0202 0104 fe04  ..s.............
+00000720: 057a 1441 6374 6f72 2e5f 6275 696c 645f  .z.Actor._build_
+00000730: 636f 6e74 6578 7463 0100 0000 0000 0000  contextc........
+00000740: 0000 0000 0100 0000 0500 0000 4300 0000  ............C...
+00000750: 732c 0000 007c 006a 0072 1464 017c 006a  s,...|.j.r.d.|.j
+00000760: 019b 0064 027c 006a 029b 009d 037c 006a  ...d.|.j.....|.j
+00000770: 017c 006a 0064 039c 0369 0153 0069 0053  .|.j.d...i.S.i.S
+00000780: 0029 044e 5a09 7075 626c 6963 4b65 79fa  .).NZ.publicKey.
+00000790: 0123 2903 720f 0000 00da 056f 776e 6572  .#).r......owner
+000007a0: 5a0c 7075 626c 6963 4b65 7950 656d 2903  Z.publicKeyPem).
+000007b0: 7217 0000 0072 0f00 0000 7218 0000 0072  r....r....r....r
+000007c0: 2a00 0000 720b 0000 0072 0b00 0000 720c  *...r....r....r.
+000007d0: 0000 0072 2000 0000 4c00 0000 7310 0000  ...r ...L...s...
+000007e0: 0006 0102 0210 0104 0104 0104 fd04 ff04  ................
+000007f0: 077a 1741 6374 6f72 2e5f 6275 696c 645f  .z.Actor._build_
+00000800: 7075 626c 6963 5f6b 6579 6302 0000 0000  public_keyc.....
+00000810: 0000 0000 0000 0004 0000 0003 0000 0043  ...............C
+00000820: 0000 0073 9000 0000 6900 7d02 7c01 7400  ...s....i.}.|.t.
+00000830: 6a01 6b02 7209 7c02 5300 7c00 6a02 7212  j.k.r.|.S.|.j.r.
+00000840: 7c00 6a02 7c02 6401 3c00 6e05 7c00 6a03  |.j.|.d.<.n.|.j.
+00000850: 7c02 6401 3c00 7c00 6a04 7220 7c00 6a04  |.d.<.|.j.r |.j.
+00000860: 7c02 6402 3c00 6e05 7c00 6a03 7c02 6402  |.d.<.n.|.j.|.d.
+00000870: 3c00 7c01 7400 6a05 6b03 722c 7c02 5300  <.|.t.j.k.r,|.S.
+00000880: 7c00 a006 a100 7d03 7c03 7236 7c03 7c02  |.....}.|.r6|.|.
+00000890: 6403 3c00 7c00 6a07 723e 7c00 6a07 7c02  d.<.|.j.r>|.j.|.
+000008a0: 6404 3c00 7c00 6a08 7246 7c00 6a08 7c02  d.<.|.j.rF|.j.|.
+000008b0: 6405 3c00 7c02 5300 2906 4e72 1300 0000  d.<.|.S.).Nr....
+000008c0: 7214 0000 00da 0965 6e64 706f 696e 7473  r......endpoints
+000008d0: 7215 0000 0072 1600 0000 2909 7205 0000  r....r....).r...
+000008e0: 0072 2200 0000 7213 0000 0072 0f00 0000  .r"...r....r....
+000008f0: 7214 0000 00da 054f 574e 4552 da15 5f62  r......OWNER.._b
+00000900: 7569 6c64 5f75 7365 725f 656e 6470 6f69  uild_user_endpoi
+00000910: 6e74 7372 1500 0000 7216 0000 0029 0472  ntsr....r....).r
+00000920: 2400 0000 721e 0000 0072 2500 0000 722d  $...r....r%...r-
+00000930: 0000 0072 0b00 0000 720b 0000 0072 0c00  ...r....r....r..
+00000940: 0000 7221 0000 0057 0000 0073 2600 0000  ..r!...W...s&...
+00000950: 0401 0a02 0401 0602 0c01 0a02 0602 0c01  ................
+00000960: 0a02 0a02 0401 0802 0401 0801 0602 0a01  ................
+00000970: 0601 0a01 0402 7a16 4163 746f 722e 5f62  ......z.Actor._b
+00000980: 7569 6c64 5f65 6e64 706f 696e 7473 6301  uild_endpointsc.
+00000990: 0000 0000 0000 0000 0000 0002 0000 0003  ................
+000009a0: 0000 0043 0000 0073 2800 0000 6900 7d01  ...C...s(...i.}.
+000009b0: 7c00 6a00 720a 7c00 6a00 7c01 6401 3c00  |.j.r.|.j.|.d.<.
+000009c0: 7c00 6a01 7212 7c00 6a01 7c01 6402 3c00  |.j.r.|.j.|.d.<.
+000009d0: 7c01 5300 2903 4eda 0b65 7665 6e74 536f  |.S.).N..eventSo
+000009e0: 7572 6365 da08 7072 6f78 7955 726c 2902  urce..proxyUrl).
+000009f0: 7219 0000 0072 1a00 0000 2902 7224 0000  r....r....).r$..
+00000a00: 0072 2d00 0000 720b 0000 0072 0b00 0000  .r-...r....r....
+00000a10: 720c 0000 0072 2f00 0000 7500 0000 730c  r....r/...u...s.
+00000a20: 0000 0004 0106 010a 0106 010a 0104 017a  ...............z
+00000a30: 1b41 6374 6f72 2e5f 6275 696c 645f 7573  .Actor._build_us
+00000a40: 6572 5f65 6e64 706f 696e 7473 291c da08  er_endpoints)...
+00000a50: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
+00000a60: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
+00000a70: 5f5f da07 5f5f 646f 635f 5fda 0373 7472  __..__doc__..str
+00000a80: da0f 5f5f 616e 6e6f 7461 7469 6f6e 735f  ..__annotations_
+00000a90: 5f72 1000 0000 7211 0000 0072 0300 0000  _r....r....r....
+00000aa0: 7212 0000 0072 1300 0000 7214 0000 0072  r....r....r....r
+00000ab0: 1500 0000 7216 0000 0072 1700 0000 7218  ....r....r....r.
+00000ac0: 0000 0072 1900 0000 721a 0000 0072 1b00  ...r....r....r..
+00000ad0: 0000 721c 0000 00da 0464 6963 7472 0500  ..r......dictr..
+00000ae0: 0000 da06 5055 424c 4943 7228 0000 0072  ....PUBLICr(...r
+00000af0: 1f00 0000 7220 0000 0072 2100 0000 722f  ....r ...r!...r/
+00000b00: 0000 0072 0b00 0000 720b 0000 0072 0b00  ...r....r....r..
+00000b10: 0000 720c 0000 0072 0e00 0000 1100 0000  ..r....r........
+00000b20: 732a 0000 000a 0004 0208 020c 0110 0110  s*..............
+00000b30: 0110 0110 0110 0110 0110 0110 0110 0110  ................
+00000b40: 0110 0210 010e 0208 1e08 0908 0b0c 1e72  ...............r
+00000b50: 0e00 0000 6300 0000 0000 0000 0000 0000  ....c...........
+00000b60: 0000 0000 0003 0000 0040 0000 0073 6000  .........@...s`.
+00000b70: 0000 6500 5a01 6400 5a02 5500 6503 6504  ..e.Z.d.Z.U.e.e.
+00000b80: 6401 3c00 6402 5a05 6506 6402 4200 6504  d.<.d.Z.e.d.B.e.
+00000b90: 6403 3c00 6404 5a07 6508 6504 6405 3c00  d.<.d.Z.e.e.d.<.
+00000ba0: 6402 5a09 6503 6402 4200 6504 6406 3c00  d.Z.e.d.B.e.d.<.
+00000bb0: 6402 5a0a 6503 6402 4200 6504 6407 3c00  d.Z.e.d.B.e.d.<.
+00000bc0: 6408 650b 6602 6409 640a 8404 5a0c 6402  d.e.f.d.d...Z.d.
+00000bd0: 5300 290b da11 4f72 6465 7265 6443 6f6c  S.)...OrderedCol
+00000be0: 6c65 6374 696f 6e72 0f00 0000 4e72 2300  lectionr....Nr#.
+00000bf0: 0000 7201 0000 00da 0563 6f75 6e74 da05  ..r......count..
+00000c00: 6669 7273 74da 046c 6173 7472 0a00 0000  first..lastr....
+00000c10: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+00000c20: 0005 0000 0043 0000 0073 4600 0000 6401  .....C...sF...d.
+00000c30: 7c00 6a00 7c00 6a01 6402 6403 9c04 7d01  |.j.|.j.d.d...}.
+00000c40: 7c00 6a02 7211 7c00 6a02 7c01 6404 3c00  |.j.r.|.j.|.d.<.
+00000c50: 7c00 6a03 7219 7c00 6a03 7c01 6405 3c00  |.j.r.|.j.|.d.<.
+00000c60: 7c00 6a04 7221 7c00 6a04 7c01 6406 3c00  |.j.r!|.j.|.d.<.
+00000c70: 7c01 5300 2907 4e72 2900 0000 723a 0000  |.S.).Nr)...r:..
+00000c80: 0029 0472 1d00 0000 720f 0000 00da 0a74  .).r....r......t
+00000c90: 6f74 616c 4974 656d 7372 1000 0000 da0c  otalItemsr......
+00000ca0: 6f72 6465 7265 6449 7465 6d73 723c 0000  orderedItemsr<..
+00000cb0: 0072 3d00 0000 2905 720f 0000 0072 3b00  .r=...).r....r;.
+00000cc0: 0000 7223 0000 0072 3c00 0000 723d 0000  ..r#...r<...r=..
+00000cd0: 00a9 0272 2400 0000 7225 0000 0072 0b00  ...r$...r%...r..
+00000ce0: 0000 720b 0000 0072 0c00 0000 7228 0000  ..r....r....r(..
+00000cf0: 0086 0000 0073 1800 0000 0202 0401 0401  .....s..........
+00000d00: 0201 06fc 0607 0a01 0602 0a01 0602 0a01  ................
+00000d10: 0402 7a17 4f72 6465 7265 6443 6f6c 6c65  ..z.OrderedColle
+00000d20: 6374 696f 6e2e 6275 696c 6429 0d72 3200  ction.build).r2.
+00000d30: 0000 7233 0000 0072 3400 0000 7236 0000  ..r3...r4...r6..
+00000d40: 0072 3700 0000 7223 0000 00da 046c 6973  .r7...r#.....lis
+00000d50: 7472 3b00 0000 da03 696e 7472 3c00 0000  tr;.....intr<...
+00000d60: 723d 0000 0072 3800 0000 7228 0000 0072  r=...r8...r(...r
+00000d70: 0b00 0000 720b 0000 0072 0b00 0000 720c  ....r....r....r.
+00000d80: 0000 0072 3a00 0000 7e00 0000 730e 0000  ...r:...~...s...
+00000d90: 000a 0008 0210 010c 0110 0110 0112 0272  ...............r
+00000da0: 3a00 0000 6300 0000 0000 0000 0000 0000  :...c...........
+00000db0: 0000 0000 0003 0000 0040 0000 0073 5400  .........@...sT.
+00000dc0: 0000 6500 5a01 6400 5a02 5500 6503 6504  ..e.Z.d.Z.U.e.e.
+00000dd0: 6401 3c00 6505 6504 6402 3c00 6503 6504  d.<.e.e.d.<.e.e.
+00000de0: 6403 3c00 6404 5a06 6503 6404 4200 6504  d.<.d.Z.e.d.B.e.
+00000df0: 6405 3c00 6404 5a07 6503 6404 4200 6504  d.<.d.Z.e.d.B.e.
+00000e00: 6406 3c00 6407 6508 6602 6408 6409 8404  d.<.d.e.f.d.d...
+00000e10: 5a09 6404 5300 290a da15 4f72 6465 7265  Z.d.S.)...Ordere
+00000e20: 6443 6f6c 6c65 6374 696f 6e50 6167 6572  dCollectionPager
+00000e30: 0f00 0000 7223 0000 00da 0770 6172 745f  ....r#.....part_
+00000e40: 6f66 4eda 046e 6578 74da 0470 7265 7672  ofN..next..prevr
+00000e50: 0a00 0000 6301 0000 0000 0000 0000 0000  ....c...........
+00000e60: 0002 0000 0006 0000 0043 0000 0073 3a00  .........C...s:.
+00000e70: 0000 6401 7c00 6a00 7c00 6a01 7c00 6a02  ..d.|.j.|.j.|.j.
+00000e80: 6402 6403 9c05 7d01 7c00 6a03 7213 7c00  d.d...}.|.j.r.|.
+00000e90: 6a03 7c01 6404 3c00 7c00 6a04 721b 7c00  j.|.d.<.|.j.r.|.
+00000ea0: 6a04 7c01 6405 3c00 7c01 5300 2906 4e72  j.|.d.<.|.S.).Nr
+00000eb0: 2900 0000 7243 0000 0029 0572 1d00 0000  )...rC...).r....
+00000ec0: 720f 0000 005a 0670 6172 744f 6672 3f00  r....Z.partOfr?.
+00000ed0: 0000 7210 0000 0072 4500 0000 7246 0000  ..r....rE...rF..
+00000ee0: 0029 0572 0f00 0000 7244 0000 0072 2300  .).r....rD...r#.
+00000ef0: 0000 7245 0000 0072 4600 0000 7240 0000  ..rE...rF...r@..
+00000f00: 0072 0b00 0000 720b 0000 0072 0c00 0000  .r....r....r....
+00000f10: 7228 0000 00a2 0000 0073 1600 0000 0202  r(.......s......
+00000f20: 0401 0401 0401 0201 06fb 0608 0a01 0602  ................
+00000f30: 0a01 0402 7a1b 4f72 6465 7265 6443 6f6c  ....z.OrderedCol
+00000f40: 6c65 6374 696f 6e50 6167 652e 6275 696c  lectionPage.buil
+00000f50: 6429 0a72 3200 0000 7233 0000 0072 3400  d).r2...r3...r4.
+00000f60: 0000 7236 0000 0072 3700 0000 7241 0000  ..r6...r7...rA..
+00000f70: 0072 4500 0000 7246 0000 0072 3800 0000  .rE...rF...r8...
+00000f80: 7228 0000 0072 0b00 0000 720b 0000 0072  r(...r....r....r
+00000f90: 0b00 0000 720c 0000 0072 4300 0000 9a00  ....r....rC.....
+00000fa0: 0000 730e 0000 000a 0008 0208 0108 0110  ..s.............
+00000fb0: 0110 0112 0272 4300 0000 4e29 10da 0b64  .....rC...N)...d
+00000fc0: 6174 6163 6c61 7373 6573 7202 0000 00da  ataclassesr.....
+00000fd0: 0674 7970 696e 6772 0300 0000 7204 0000  .typingr....r...
+00000fe0: 00da 0c62 6f76 696e 652e 7479 7065 7372  ...bovine.typesr
+00000ff0: 0500 0000 da10 6163 7469 7669 7479 5f66  ......activity_f
+00001000: 6163 746f 7279 7207 0000 00da 0e6f 626a  actoryr......obj
+00001010: 6563 745f 6661 6374 6f72 7972 0800 0000  ect_factoryr....
+00001020: 7238 0000 0072 0d00 0000 720e 0000 0072  r8...r....r....r
+00001030: 3a00 0000 7243 0000 0072 0b00 0000 720b  :...rC...r....r.
+00001040: 0000 0072 0b00 0000 720c 0000 00da 083c  ...r....r......<
+00001050: 6d6f 6475 6c65 3e01 0000 0073 2000 0000  module>....s ...
+00001060: 0c00 1001 0c02 0c02 0c01 0203 0201 02ff  ................
+00001070: 0a02 0afe 0207 1001 026c 1001 021b 1401  .........l......
```

### Comparing `bovine-0.1.0/bovine/activitystreams/__pycache__/activity_factory.cpython-310.pyc` & `bovine-0.1.1/bovine/activitystreams/__pycache__/activity_factory.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 13 15:55:57 2023 UTC, .py size: 3726 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0d26 3864 8e0e 0000  o........&8d....
+00000000: 6f0d 0d0a 0000 0000 a4ea 3a64 ac0f 0000  o.........:d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4400 0000 6400  .....@...sD...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 6d04 5a04 6d05 5a05 0100 6501  d.l.m.Z.m.Z...e.
 00000050: 4700 6403 6404 8400 6404 8302 8301 5a06  G.d.d...d.....Z.
 00000060: 4700 6405 6406 8400 6406 8302 5a07 6407  G.d.d...d...Z.d.
 00000070: 5300 2908 e900 0000 0029 02da 0964 6174  S.)......)...dat
@@ -49,192 +49,208 @@
 00000300: 2c20 692e 652e 2070 7562 6c69 6320 696e  , i.e. public in
 00000310: 2074 6f20 616e 6420 666f 6c6c 6f77 6572   to and follower
 00000320: 7320 696e 2063 63fa 2c68 7474 7073 3a2f  s in cc.,https:/
 00000330: 2f77 7777 2e77 332e 6f72 672f 6e73 2f61  /www.w3.org/ns/a
 00000340: 6374 6976 6974 7973 7472 6561 6d73 2350  ctivitystreams#P
 00000350: 7562 6c69 6329 0472 0d00 0000 da03 6164  ublic).r......ad
 00000360: 6472 0900 0000 720e 0000 00a9 01da 0473  dr....r........s
-00000370: 656c 66a9 0072 1800 0000 fa5b 2f77 6f6f  elf..r.....[/woo
+00000370: 656c 66a9 0072 1800 0000 fa5c 2f77 6f6f  elf..r.....\/woo
 00000380: 6470 6563 6b65 722f 7372 632f 636f 6465  dpecker/src/code
-00000390: 6265 7267 2e6f 7267 2f68 656c 6765 2f62  berg.org/helge/b
-000003a0: 6f76 696e 652f 626f 7669 6e65 2f62 6f76  ovine/bovine/bov
-000003b0: 696e 652f 6163 7469 7669 7479 7374 7265  ine/activitystre
-000003c0: 616d 732f 6163 7469 7669 7479 5f66 6163  ams/activity_fac
-000003d0: 746f 7279 2e70 79da 0961 735f 7075 626c  tory.py..as_publ
-000003e0: 6963 1900 0000 7308 0000 000c 0206 010e  ic....s.........
-000003f0: 0104 017a 1241 6374 6976 6974 792e 6173  ...z.Activity.as
-00000400: 5f70 7562 6c69 6363 0100 0000 0000 0000  _publicc........
-00000410: 0000 0000 0100 0000 0300 0000 4300 0000  ............C...
-00000420: 7324 0000 007c 006a 0072 0a7c 006a 01a0  s$...|.j.r.|.j..
-00000430: 027c 006a 00a1 0101 007c 006a 03a0 0264  .|.j.....|.j...d
-00000440: 01a1 0101 007c 0053 0029 027a 426d 616b  .....|.S.).zBmak
-00000450: 6573 2074 6865 2061 6374 6976 6974 7920  es the activity 
-00000460: 756e 6c69 7374 6564 2c20 692e 652e 2070  unlisted, i.e. p
-00000470: 7562 6c69 6320 696e 2063 6320 616e 6420  ublic in cc and 
-00000480: 666f 6c6c 6f77 6572 7320 696e 2074 6f72  followers in tor
-00000490: 1400 0000 2904 7209 0000 0072 0d00 0000  ....).r....r....
-000004a0: 7215 0000 0072 0e00 0000 7216 0000 0072  r....r....r....r
-000004b0: 1800 0000 7218 0000 0072 1900 0000 da0b  ....r....r......
-000004c0: 6173 5f75 6e6c 6973 7465 6420 0000 0073  as_unlisted ...s
-000004d0: 0800 0000 0602 0e01 0c01 0401 7a14 4163  ............z.Ac
-000004e0: 7469 7669 7479 2e61 735f 756e 6c69 7374  tivity.as_unlist
-000004f0: 6564 6301 0000 0000 0000 0000 0000 0005  edc.............
-00000500: 0000 0008 0000 0043 0000 0073 ae00 0000  .......C...s....
-00000510: 6401 7c00 6a00 7c00 6a01 7402 7c00 6a03  d.|.j.|.j.t.|.j.
-00000520: 8301 7402 7c00 6a04 7c00 6a03 1800 8301  ..t.|.j.|.j.....
-00000530: 6402 9c05 7d01 7c00 6a05 7c00 6a06 7c00  d...}.|.j.|.j.|.
-00000540: 6a07 7c00 6a08 7c00 6a09 7c00 6a0a 7c00  j.|.j.|.j.|.j.|.
-00000550: 6a0b 6403 9c07 7d02 7c01 6404 1900 6405  j.d...}.|.d...d.
-00000560: 7501 7235 740c 7c01 6404 1900 8301 6406  u.r5t.|.d.....d.
-00000570: 6b02 7235 7c01 6404 3d00 7c01 6407 1900  k.r5|.d.=.|.d...
-00000580: 6405 7501 7246 740c 7c01 6407 1900 8301  d.u.rFt.|.d.....
-00000590: 6406 6b02 7246 7c01 6407 3d00 7c02 a00d  d.k.rF|.d.=.|...
-000005a0: a100 4400 5d0a 5c02 7d03 7d04 7c04 7254  ..D.].\.}.}.|.rT
-000005b0: 7c04 7c01 7c03 3c00 714a 7c01 5300 2908  |.|.|.<.qJ|.S.).
-000005c0: 7a41 636f 6e76 6572 7473 2074 6865 2061  zAconverts the a
-000005d0: 6374 6976 6974 7920 696e 746f 2061 2064  ctivity into a d
-000005e0: 6963 742c 2074 6861 7420 6361 6e20 6265  ict, that can be
-000005f0: 2073 6572 6961 6c69 7a65 6420 746f 204a   serialized to J
-00000600: 534f 4e7a 2568 7474 7073 3a2f 2f77 7777  SONz%https://www
-00000610: 2e77 332e 6f72 672f 6e73 2f61 6374 6976  .w3.org/ns/activ
-00000620: 6974 7973 7472 6561 6d73 2905 7a08 4063  itystreams).z.@c
-00000630: 6f6e 7465 7874 7207 0000 0072 0800 0000  ontextr....r....
-00000640: 720d 0000 0072 0e00 0000 2907 720a 0000  r....r....).r...
-00000650: 0072 0b00 0000 720f 0000 0072 1000 0000  .r....r....r....
-00000660: 7211 0000 0072 1200 0000 7213 0000 0072  r....r....r....r
-00000670: 0d00 0000 4e72 0100 0000 720e 0000 0029  ....Nr....r....)
-00000680: 0e72 0700 0000 7208 0000 00da 046c 6973  .r....r......lis
-00000690: 7472 0d00 0000 720e 0000 0072 0a00 0000  tr....r....r....
-000006a0: 720b 0000 0072 0f00 0000 7210 0000 0072  r....r....r....r
-000006b0: 1100 0000 7212 0000 0072 1300 0000 da03  ....r....r......
-000006c0: 6c65 6eda 0569 7465 6d73 2905 7217 0000  len..items).r...
-000006d0: 00da 0672 6573 756c 745a 0c65 7874 7261  ...resultZ.extra
-000006e0: 5f66 6965 6c64 73da 036b 6579 da05 7661  _fields..key..va
-000006f0: 6c75 6572 1800 0000 7218 0000 0072 1900  luer....r....r..
-00000700: 0000 da05 6275 696c 6427 0000 0073 2e00  ....build'...s..
-00000710: 0000 0203 0401 0401 0801 0e01 06fb 0409  ................
-00000720: 0401 0401 0401 0401 0401 0401 06f9 1c0a  ................
-00000730: 0601 1c01 0601 1002 0401 0801 0280 0402  ................
-00000740: 7a0e 4163 7469 7669 7479 2e62 7569 6c64  z.Activity.build
-00000750: 2918 da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
-00000760: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
-00000770: 6e61 6d65 5f5f da07 5f5f 646f 635f 5fda  name__..__doc__.
-00000780: 0373 7472 da0f 5f5f 616e 6e6f 7461 7469  .str..__annotati
-00000790: 6f6e 735f 5f72 0800 0000 7204 0000 0072  ons__r....r....r
-000007a0: 0900 0000 720a 0000 0072 0b00 0000 7203  ....r....r....r.
-000007b0: 0000 00da 0373 6574 720d 0000 0072 0500  .....setr....r..
-000007c0: 0000 720e 0000 0072 0f00 0000 7210 0000  ..r....r....r...
-000007d0: 0072 1100 0000 7212 0000 0072 1300 0000  .r....r....r....
-000007e0: 721a 0000 0072 1b00 0000 7222 0000 0072  r....r....r"...r
-000007f0: 1800 0000 7218 0000 0072 1800 0000 7219  ....r....r....r.
-00000800: 0000 0072 0600 0000 0500 0000 7322 0000  ...r........s"..
-00000810: 000a 0004 0208 0310 0110 0110 0110 0116  ................
-00000820: 0116 0110 0210 0110 0110 0210 0108 0208  ................
-00000830: 070c 0772 0600 0000 6300 0000 0000 0000  ...r....c.......
-00000840: 0000 0000 0000 0000 0002 0000 0040 0000  .............@..
-00000850: 0073 4800 0000 6500 5a01 6400 5a02 6401  .sH...e.Z.d.Z.d.
-00000860: 5a03 6402 6403 8400 5a04 6404 6405 8400  Z.d.d...Z.d.d...
-00000870: 5a05 6406 6407 8400 5a06 6408 6409 8400  Z.d.d...Z.d.d...
-00000880: 5a07 640a 640b 8400 5a08 640c 640d 8400  Z.d.d...Z.d.d...
-00000890: 5a09 640e 640f 8400 5a0a 6410 5300 2911  Z.d.d...Z.d.S.).
-000008a0: da0f 4163 7469 7669 7479 4661 6374 6f72  ..ActivityFactor
-000008b0: 797a 4942 6173 6963 2066 6163 746f 7279  yzIBasic factory
-000008c0: 2066 6f72 2041 6374 6976 6974 7920 6f62   for Activity ob
-000008d0: 6a65 6374 732e 0a0a 2020 2020 5573 616c  jects...    Usal
-000008e0: 6c79 2063 7265 6174 6564 2062 7920 6120  ly created by a 
-000008f0: 426f 7669 6e65 436c 6965 6e74 6302 0000  BovineClientc...
-00000900: 0000 0000 0000 0000 0002 0000 0002 0000  ................
-00000910: 0043 0000 0073 0a00 0000 7c01 7c00 5f00  .C...s....|.|._.
-00000920: 6400 5300 2901 4e29 01da 0b69 6e66 6f72  d.S.).N)...infor
-00000930: 6d61 7469 6f6e 2902 7217 0000 00da 1161  mation).r......a
-00000940: 6374 6f72 5f69 6e66 6f72 6d61 7469 6f6e  ctor_information
-00000950: 7218 0000 0072 1800 0000 7219 0000 00da  r....r....r.....
-00000960: 085f 5f69 6e69 745f 5f4c 0000 0073 0200  .__init__L...s..
-00000970: 0000 0a01 7a18 4163 7469 7669 7479 4661  ....z.ActivityFa
-00000980: 6374 6f72 792e 5f5f 696e 6974 5f5f 6302  ctory.__init__c.
-00000990: 0000 0000 0000 0000 0000 0003 0000 000a  ................
-000009a0: 0000 004b 0000 00f3 3600 0000 7400 6407  ...K....6...t.d.
-000009b0: 6401 7c01 6402 1900 7401 7c01 a002 6403  d.|.d...t.|...d.
-000009c0: 6700 a102 8301 7401 7c01 a002 6404 6700  g.....t.|...d.g.
-000009d0: a102 8301 7c01 6405 9c05 7c02 a401 8e01  ....|.d...|.....
-000009e0: 5300 2908 7a23 4163 7469 7669 7479 206f  S.).z#Activity o
-000009f0: 6620 7479 7065 2043 7265 6174 6520 6672  f type Create fr
-00000a00: 6f6d 204f 626a 6563 745a 0643 7265 6174  om ObjectZ.Creat
-00000a10: 65da 0c61 7474 7269 6275 7465 6454 6f72  e..attributedTor
-00000a20: 0e00 0000 720d 0000 00a9 0572 0700 0000  ....r......r....
-00000a30: 7208 0000 0072 0e00 0000 720d 0000 0072  r....r....r....r
-00000a40: 1300 0000 4e72 1800 0000 a903 7206 0000  ....Nr......r...
-00000a50: 0072 2900 0000 da03 6765 74a9 0372 1700  .r).....get..r..
-00000a60: 0000 da03 6f62 6ada 066b 7761 7267 7372  ....obj..kwargsr
-00000a70: 1800 0000 7218 0000 0072 1900 0000 da06  ....r....r......
-00000a80: 6372 6561 7465 4f00 0000 f312 0000 0004  createO.........
-00000a90: 0202 0106 010e 010e 0102 0104 fb02 0606  ................
-00000aa0: fa7a 1641 6374 6976 6974 7946 6163 746f  .z.ActivityFacto
-00000ab0: 7279 2e63 7265 6174 6563 0200 0000 0000  ry.createc......
-00000ac0: 0000 0000 0000 0300 0000 0a00 0000 4b00  ..............K.
-00000ad0: 0000 722e 0000 0029 087a 2341 6374 6976  ..r....).z#Activ
-00000ae0: 6974 7920 6f66 2074 7970 6520 5570 6461  ity of type Upda
-00000af0: 7465 2066 726f 6d20 4f62 6a65 6374 5a06  te from ObjectZ.
-00000b00: 5570 6461 7465 722f 0000 0072 0e00 0000  Updater/...r....
-00000b10: 720d 0000 0072 3000 0000 4e72 1800 0000  r....r0...Nr....
-00000b20: 7231 0000 0072 3300 0000 7218 0000 0072  r1...r3...r....r
-00000b30: 1800 0000 7219 0000 00da 0675 7064 6174  ....r......updat
-00000b40: 655a 0000 0072 3700 0000 7a16 4163 7469  eZ...r7...z.Acti
-00000b50: 7669 7479 4661 6374 6f72 792e 7570 6461  vityFactory.upda
-00000b60: 7465 6302 0000 0000 0000 0000 0000 0003  tec.............
-00000b70: 0000 0006 0000 004b 0000 00f3 1c00 0000  .......K........
-00000b80: 7400 6405 6401 7c00 6a01 6402 1900 7c01  t.d.d.|.j.d...|.
-00000b90: 6403 9c03 7c02 a401 8e01 5300 2906 7a0f  d...|.....S.).z.
-00000ba0: 4c69 6b65 2066 6f72 2074 6172 6765 745a  Like for targetZ
-00000bb0: 044c 696b 6572 0a00 0000 a903 7207 0000  .Liker......r...
-00000bc0: 0072 0800 0000 7213 0000 004e 7218 0000  .r....r....Nr...
-00000bd0: 00a9 0272 0600 0000 722b 0000 00a9 0372  ...r....r+.....r
-00000be0: 1700 0000 7212 0000 0072 3500 0000 7218  ....r....r5...r.
-00000bf0: 0000 0072 1800 0000 7219 0000 00da 046c  ...r....r......l
-00000c00: 696b 6565 0000 00f3 0a00 0000 0402 0c01  ikee............
-00000c10: 04ff 0201 06ff 7a14 4163 7469 7669 7479  ......z.Activity
-00000c20: 4661 6374 6f72 792e 6c69 6b65 6302 0000  Factory.likec...
-00000c30: 0000 0000 0000 0000 0003 0000 0006 0000  ................
-00000c40: 004b 0000 0072 3900 0000 2906 7a11 4465  .K...r9...).z.De
-00000c50: 6c65 7465 2066 6f72 2074 6172 6765 74da  lete for target.
-00000c60: 0644 656c 6574 6572 0a00 0000 723a 0000  .Deleter....r:..
-00000c70: 004e 7218 0000 0072 3b00 0000 723c 0000  .Nr....r;...r<..
-00000c80: 0072 1800 0000 7218 0000 0072 1900 0000  .r....r....r....
-00000c90: da06 6465 6c65 7465 6b00 0000 723e 0000  ..deletek...r>..
-00000ca0: 007a 1641 6374 6976 6974 7946 6163 746f  .z.ActivityFacto
-00000cb0: 7279 2e64 656c 6574 6563 0200 0000 0000  ry.deletec......
-00000cc0: 0000 0000 0000 0300 0000 0600 0000 4b00  ..............K.
-00000cd0: 0000 7239 0000 0029 067a 1141 6363 6570  ..r9...).z.Accep
-00000ce0: 7420 666f 7220 6f62 6a65 6374 da06 4163  t for object..Ac
-00000cf0: 6365 7074 720a 0000 0072 3a00 0000 4e72  ceptr....r:...Nr
-00000d00: 1800 0000 723b 0000 0072 3300 0000 7218  ....r;...r3...r.
-00000d10: 0000 0072 1800 0000 7219 0000 00da 0661  ...r....r......a
-00000d20: 6363 6570 7471 0000 0072 3e00 0000 7a16  cceptq...r>...z.
-00000d30: 4163 7469 7669 7479 4661 6374 6f72 792e  ActivityFactory.
-00000d40: 6163 6365 7074 6302 0000 0000 0000 0000  acceptc.........
-00000d50: 0000 0003 0000 0007 0000 004b 0000 0073  ...........K...s
-00000d60: 2400 0000 7400 6405 6401 7c00 6a01 6402  $...t.d.d.|.j.d.
-00000d70: 1900 7c01 7402 7c01 6701 8301 6403 9c04  ..|.t.|.g...d...
-00000d80: 7c02 a401 8e01 5300 2906 7a11 466f 6c6c  |.....S.).z.Foll
-00000d90: 6f77 2066 6f72 206f 626a 6563 745a 0646  ow for objectZ.F
-00000da0: 6f6c 6c6f 7772 0a00 0000 2904 7207 0000  ollowr....).r...
-00000db0: 0072 0800 0000 7213 0000 0072 0d00 0000  .r....r....r....
-00000dc0: 4e72 1800 0000 2903 7206 0000 0072 2b00  Nr....).r....r+.
-00000dd0: 0000 7229 0000 0072 3300 0000 7218 0000  ..r)...r3...r...
-00000de0: 0072 1800 0000 7219 0000 00da 0666 6f6c  .r....r......fol
-00000df0: 6c6f 7777 0000 0073 1000 0000 0402 0201  loww...s........
-00000e00: 0801 0201 0801 04fc 0205 06fb 7a16 4163  ............z.Ac
-00000e10: 7469 7669 7479 4661 6374 6f72 792e 666f  tivityFactory.fo
-00000e20: 6c6c 6f77 4e29 0b72 2300 0000 7224 0000  llowN).r#...r$..
-00000e30: 0072 2500 0000 7226 0000 0072 2d00 0000  .r%...r&...r-...
-00000e40: 7236 0000 0072 3800 0000 723d 0000 0072  r6...r8...r=...r
-00000e50: 4000 0000 7242 0000 0072 4300 0000 7218  @...rB...rC...r.
-00000e60: 0000 0072 1800 0000 7218 0000 0072 1900  ...r....r....r..
-00000e70: 0000 722a 0000 0047 0000 0073 1200 0000  ..r*...G...s....
-00000e80: 0800 0401 0804 0803 080b 080b 0806 0806  ................
-00000e90: 0c06 722a 0000 004e 2908 da0b 6461 7461  ..r*...N)...data
-00000ea0: 636c 6173 7365 7372 0200 0000 7203 0000  classesr....r...
-00000eb0: 00da 0674 7970 696e 6772 0400 0000 7205  ...typingr....r.
-00000ec0: 0000 0072 0600 0000 722a 0000 0072 1800  ...r....r*...r..
-00000ed0: 0000 7218 0000 0072 1800 0000 7219 0000  ..r....r....r...
-00000ee0: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
-00000ef0: 0a00 0000 1000 1001 0203 1001 1241       .............A
+00000390: 6265 7267 2e6f 7267 2f62 6f76 696e 652f  berg.org/bovine/
+000003a0: 626f 7669 6e65 2f62 6f76 696e 652f 626f  bovine/bovine/bo
+000003b0: 7669 6e65 2f61 6374 6976 6974 7973 7472  vine/activitystr
+000003c0: 6561 6d73 2f61 6374 6976 6974 795f 6661  eams/activity_fa
+000003d0: 6374 6f72 792e 7079 da09 6173 5f70 7562  ctory.py..as_pub
+000003e0: 6c69 6319 0000 0073 0800 0000 0c02 0601  lic....s........
+000003f0: 0e01 0401 7a12 4163 7469 7669 7479 2e61  ....z.Activity.a
+00000400: 735f 7075 626c 6963 6301 0000 0000 0000  s_publicc.......
+00000410: 0000 0000 0001 0000 0003 0000 0043 0000  .............C..
+00000420: 0073 2400 0000 7c00 6a00 720a 7c00 6a01  .s$...|.j.r.|.j.
+00000430: a002 7c00 6a00 a101 0100 7c00 6a03 a002  ..|.j.....|.j...
+00000440: 6401 a101 0100 7c00 5300 2902 7a42 6d61  d.....|.S.).zBma
+00000450: 6b65 7320 7468 6520 6163 7469 7669 7479  kes the activity
+00000460: 2075 6e6c 6973 7465 642c 2069 2e65 2e20   unlisted, i.e. 
+00000470: 7075 626c 6963 2069 6e20 6363 2061 6e64  public in cc and
+00000480: 2066 6f6c 6c6f 7765 7273 2069 6e20 746f   followers in to
+00000490: 7214 0000 0029 0472 0900 0000 720d 0000  r....).r....r...
+000004a0: 0072 1500 0000 720e 0000 0072 1600 0000  .r....r....r....
+000004b0: 7218 0000 0072 1800 0000 7219 0000 00da  r....r....r.....
+000004c0: 0b61 735f 756e 6c69 7374 6564 2000 0000  .as_unlisted ...
+000004d0: 7308 0000 0006 020e 010c 0104 017a 1441  s............z.A
+000004e0: 6374 6976 6974 792e 6173 5f75 6e6c 6973  ctivity.as_unlis
+000004f0: 7465 6463 0100 0000 0000 0000 0000 0000  tedc............
+00000500: 0500 0000 0800 0000 4300 0000 73ae 0000  ........C...s...
+00000510: 0064 017c 006a 007c 006a 0174 027c 006a  .d.|.j.|.j.t.|.j
+00000520: 0383 0174 027c 006a 047c 006a 0318 0083  ...t.|.j.|.j....
+00000530: 0164 029c 057d 017c 006a 057c 006a 067c  .d...}.|.j.|.j.|
+00000540: 006a 077c 006a 087c 006a 097c 006a 0a7c  .j.|.j.|.j.|.j.|
+00000550: 006a 0b64 039c 077d 027c 0164 0419 0064  .j.d...}.|.d...d
+00000560: 0575 0172 3574 0c7c 0164 0419 0083 0164  .u.r5t.|.d.....d
+00000570: 066b 0272 357c 0164 043d 007c 0164 0719  .k.r5|.d.=.|.d..
+00000580: 0064 0575 0172 4674 0c7c 0164 0719 0083  .d.u.rFt.|.d....
+00000590: 0164 066b 0272 467c 0164 073d 007c 02a0  .d.k.rF|.d.=.|..
+000005a0: 0da1 0044 005d 0a5c 027d 037d 047c 0472  ...D.].\.}.}.|.r
+000005b0: 547c 047c 017c 033c 0071 4a7c 0153 0029  T|.|.|.<.qJ|.S.)
+000005c0: 087a 4163 6f6e 7665 7274 7320 7468 6520  .zAconverts the 
+000005d0: 6163 7469 7669 7479 2069 6e74 6f20 6120  activity into a 
+000005e0: 6469 6374 2c20 7468 6174 2063 616e 2062  dict, that can b
+000005f0: 6520 7365 7269 616c 697a 6564 2074 6f20  e serialized to 
+00000600: 4a53 4f4e 7a25 6874 7470 733a 2f2f 7777  JSONz%https://ww
+00000610: 772e 7733 2e6f 7267 2f6e 732f 6163 7469  w.w3.org/ns/acti
+00000620: 7669 7479 7374 7265 616d 7329 057a 0840  vitystreams).z.@
+00000630: 636f 6e74 6578 7472 0700 0000 7208 0000  contextr....r...
+00000640: 0072 0d00 0000 720e 0000 0029 0772 0a00  .r....r....).r..
+00000650: 0000 720b 0000 0072 0f00 0000 7210 0000  ..r....r....r...
+00000660: 0072 1100 0000 7212 0000 0072 1300 0000  .r....r....r....
+00000670: 720d 0000 004e 7201 0000 0072 0e00 0000  r....Nr....r....
+00000680: 290e 7207 0000 0072 0800 0000 da04 6c69  ).r....r......li
+00000690: 7374 720d 0000 0072 0e00 0000 720a 0000  str....r....r...
+000006a0: 0072 0b00 0000 720f 0000 0072 1000 0000  .r....r....r....
+000006b0: 7211 0000 0072 1200 0000 7213 0000 00da  r....r....r.....
+000006c0: 036c 656e da05 6974 656d 7329 0572 1700  .len..items).r..
+000006d0: 0000 da06 7265 7375 6c74 5a0c 6578 7472  ....resultZ.extr
+000006e0: 615f 6669 656c 6473 da03 6b65 79da 0576  a_fields..key..v
+000006f0: 616c 7565 7218 0000 0072 1800 0000 7219  aluer....r....r.
+00000700: 0000 00da 0562 7569 6c64 2700 0000 732e  .....build'...s.
+00000710: 0000 0002 0304 0104 0108 010e 0106 fb04  ................
+00000720: 0904 0104 0104 0104 0104 0104 0106 f91c  ................
+00000730: 0a06 011c 0106 0110 0204 0108 0102 8004  ................
+00000740: 027a 0e41 6374 6976 6974 792e 6275 696c  .z.Activity.buil
+00000750: 6429 18da 085f 5f6e 616d 655f 5fda 0a5f  d)...__name__.._
+00000760: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
+00000770: 6c6e 616d 655f 5fda 075f 5f64 6f63 5f5f  lname__..__doc__
+00000780: da03 7374 72da 0f5f 5f61 6e6e 6f74 6174  ..str..__annotat
+00000790: 696f 6e73 5f5f 7208 0000 0072 0400 0000  ions__r....r....
+000007a0: 7209 0000 0072 0a00 0000 720b 0000 0072  r....r....r....r
+000007b0: 0300 0000 da03 7365 7472 0d00 0000 7205  ......setr....r.
+000007c0: 0000 0072 0e00 0000 720f 0000 0072 1000  ...r....r....r..
+000007d0: 0000 7211 0000 0072 1200 0000 7213 0000  ..r....r....r...
+000007e0: 0072 1a00 0000 721b 0000 0072 2200 0000  .r....r....r"...
+000007f0: 7218 0000 0072 1800 0000 7218 0000 0072  r....r....r....r
+00000800: 1900 0000 7206 0000 0005 0000 0073 2200  ....r........s".
+00000810: 0000 0a00 0402 0803 1001 1001 1001 1001  ................
+00000820: 1601 1601 1002 1001 1001 1002 1001 0802  ................
+00000830: 0807 0c07 7206 0000 0063 0000 0000 0000  ....r....c......
+00000840: 0000 0000 0000 0000 0000 0200 0000 4000  ..............@.
+00000850: 0000 7350 0000 0065 005a 0164 005a 0264  ..sP...e.Z.d.Z.d
+00000860: 015a 0364 0264 0384 005a 0464 0464 0584  .Z.d.d...Z.d.d..
+00000870: 005a 0564 0664 0784 005a 0664 0864 0984  .Z.d.d...Z.d.d..
+00000880: 005a 0764 0a64 0b84 005a 0864 0c64 0d84  .Z.d.d...Z.d.d..
+00000890: 005a 0964 0e64 0f84 005a 0a64 1064 1184  .Z.d.d...Z.d.d..
+000008a0: 005a 0b64 1253 0029 13da 0f41 6374 6976  .Z.d.S.)...Activ
+000008b0: 6974 7946 6163 746f 7279 7a49 4261 7369  ityFactoryzIBasi
+000008c0: 6320 6661 6374 6f72 7920 666f 7220 4163  c factory for Ac
+000008d0: 7469 7669 7479 206f 626a 6563 7473 2e0a  tivity objects..
+000008e0: 0a20 2020 2055 7361 6c6c 7920 6372 6561  .    Usally crea
+000008f0: 7465 6420 6279 2061 2042 6f76 696e 6543  ted by a BovineC
+00000900: 6c69 656e 7463 0200 0000 0000 0000 0000  lientc..........
+00000910: 0000 0200 0000 0200 0000 4300 0000 730a  ..........C...s.
+00000920: 0000 007c 017c 005f 0064 0053 0029 014e  ...|.|._.d.S.).N
+00000930: 2901 da0b 696e 666f 726d 6174 696f 6e29  )...information)
+00000940: 0272 1700 0000 da11 6163 746f 725f 696e  .r......actor_in
+00000950: 666f 726d 6174 696f 6e72 1800 0000 7218  formationr....r.
+00000960: 0000 0072 1900 0000 da08 5f5f 696e 6974  ...r......__init
+00000970: 5f5f 4c00 0000 7302 0000 000a 017a 1841  __L...s......z.A
+00000980: 6374 6976 6974 7946 6163 746f 7279 2e5f  ctivityFactory._
+00000990: 5f69 6e69 745f 5f63 0200 0000 0000 0000  _init__c........
+000009a0: 0000 0000 0300 0000 0a00 0000 4b00 0000  ............K...
+000009b0: f336 0000 0074 0064 0764 017c 0164 0219  .6...t.d.d.|.d..
+000009c0: 0074 017c 01a0 0264 0367 00a1 0283 0174  .t.|...d.g.....t
+000009d0: 017c 01a0 0264 0467 00a1 0283 017c 0164  .|...d.g.....|.d
+000009e0: 059c 057c 02a4 018e 0153 0029 087a 2341  ...|.....S.).z#A
+000009f0: 6374 6976 6974 7920 6f66 2074 7970 6520  ctivity of type 
+00000a00: 4372 6561 7465 2066 726f 6d20 4f62 6a65  Create from Obje
+00000a10: 6374 5a06 4372 6561 7465 da0c 6174 7472  ctZ.Create..attr
+00000a20: 6962 7574 6564 546f 720e 0000 0072 0d00  ibutedTor....r..
+00000a30: 0000 a905 7207 0000 0072 0800 0000 720e  ....r....r....r.
+00000a40: 0000 0072 0d00 0000 7213 0000 004e 7218  ...r....r....Nr.
+00000a50: 0000 00a9 0372 0600 0000 7229 0000 00da  .....r....r)....
+00000a60: 0367 6574 a903 7217 0000 00da 036f 626a  .get..r......obj
+00000a70: da06 6b77 6172 6773 7218 0000 0072 1800  ..kwargsr....r..
+00000a80: 0000 7219 0000 00da 0663 7265 6174 654f  ..r......createO
+00000a90: 0000 00f3 1200 0000 0402 0201 0601 0e01  ................
+00000aa0: 0e01 0201 04fb 0206 06fa 7a16 4163 7469  ..........z.Acti
+00000ab0: 7669 7479 4661 6374 6f72 792e 6372 6561  vityFactory.crea
+00000ac0: 7465 6302 0000 0000 0000 0000 0000 0003  tec.............
+00000ad0: 0000 000a 0000 004b 0000 0072 2e00 0000  .......K...r....
+00000ae0: 2908 7a23 4163 7469 7669 7479 206f 6620  ).z#Activity of 
+00000af0: 7479 7065 2055 7064 6174 6520 6672 6f6d  type Update from
+00000b00: 204f 626a 6563 745a 0655 7064 6174 6572   ObjectZ.Updater
+00000b10: 2f00 0000 720e 0000 0072 0d00 0000 7230  /...r....r....r0
+00000b20: 0000 004e 7218 0000 0072 3100 0000 7233  ...Nr....r1...r3
+00000b30: 0000 0072 1800 0000 7218 0000 0072 1900  ...r....r....r..
+00000b40: 0000 da06 7570 6461 7465 5a00 0000 7237  ....updateZ...r7
+00000b50: 0000 007a 1641 6374 6976 6974 7946 6163  ...z.ActivityFac
+00000b60: 746f 7279 2e75 7064 6174 6563 0200 0000  tory.updatec....
+00000b70: 0000 0000 0000 0000 0300 0000 0600 0000  ................
+00000b80: 4b00 0000 f31c 0000 0074 0064 0564 017c  K........t.d.d.|
+00000b90: 006a 0164 0219 007c 0164 039c 037c 02a4  .j.d...|.d...|..
+00000ba0: 018e 0153 0029 067a 0f4c 696b 6520 666f  ...S.).z.Like fo
+00000bb0: 7220 7461 7267 6574 5a04 4c69 6b65 720a  r targetZ.Liker.
+00000bc0: 0000 00a9 0372 0700 0000 7208 0000 0072  .....r....r....r
+00000bd0: 1300 0000 4e72 1800 0000 a902 7206 0000  ....Nr......r...
+00000be0: 0072 2b00 0000 a903 7217 0000 0072 1200  .r+.....r....r..
+00000bf0: 0000 7235 0000 0072 1800 0000 7218 0000  ..r5...r....r...
+00000c00: 0072 1900 0000 da04 6c69 6b65 6500 0000  .r......likee...
+00000c10: f30a 0000 0004 020c 0104 ff02 0106 ff7a  ...............z
+00000c20: 1441 6374 6976 6974 7946 6163 746f 7279  .ActivityFactory
+00000c30: 2e6c 696b 6563 0200 0000 0000 0000 0000  .likec..........
+00000c40: 0000 0300 0000 0600 0000 4b00 0000 7239  ..........K...r9
+00000c50: 0000 0029 067a 1144 656c 6574 6520 666f  ...).z.Delete fo
+00000c60: 7220 7461 7267 6574 da06 4465 6c65 7465  r target..Delete
+00000c70: 720a 0000 0072 3a00 0000 4e72 1800 0000  r....r:...Nr....
+00000c80: 723b 0000 0072 3c00 0000 7218 0000 0072  r;...r<...r....r
+00000c90: 1800 0000 7219 0000 00da 0664 656c 6574  ....r......delet
+00000ca0: 656b 0000 0072 3e00 0000 7a16 4163 7469  ek...r>...z.Acti
+00000cb0: 7669 7479 4661 6374 6f72 792e 6465 6c65  vityFactory.dele
+00000cc0: 7465 6302 0000 0000 0000 0000 0000 0003  tec.............
+00000cd0: 0000 0006 0000 004b 0000 0072 3900 0000  .......K...r9...
+00000ce0: 2906 7a11 4163 6365 7074 2066 6f72 206f  ).z.Accept for o
+00000cf0: 626a 6563 74da 0641 6363 6570 7472 0a00  bject..Acceptr..
+00000d00: 0000 723a 0000 004e 7218 0000 0072 3b00  ..r:...Nr....r;.
+00000d10: 0000 7233 0000 0072 1800 0000 7218 0000  ..r3...r....r...
+00000d20: 0072 1900 0000 da06 6163 6365 7074 7100  .r......acceptq.
+00000d30: 0000 723e 0000 007a 1641 6374 6976 6974  ..r>...z.Activit
+00000d40: 7946 6163 746f 7279 2e61 6363 6570 7463  yFactory.acceptc
+00000d50: 0200 0000 0000 0000 0000 0000 0300 0000  ................
+00000d60: 0900 0000 4b00 0000 7328 0000 0074 0064  ....K...s(...t.d
+00000d70: 0664 017c 006a 0164 0219 007c 017c 006a  .d.|.j.d...|.|.j
+00000d80: 01a0 0264 0367 00a1 0264 049c 047c 02a4  ...d.g...d...|..
+00000d90: 018e 0153 0029 077a 1341 6e6e 6f75 6e63  ...S.).z.Announc
+00000da0: 6520 666f 7220 6f62 6a65 6374 5a08 416e  e for objectZ.An
+00000db0: 6e6f 756e 6365 720a 0000 0072 0900 0000  nouncer....r....
+00000dc0: 2904 7207 0000 0072 0800 0000 7213 0000  ).r....r....r...
+00000dd0: 0072 0900 0000 4e72 1800 0000 2903 7206  .r....Nr....).r.
+00000de0: 0000 0072 2b00 0000 7232 0000 0072 3300  ...r+...r2...r3.
+00000df0: 0000 7218 0000 0072 1800 0000 7219 0000  ..r....r....r...
+00000e00: 00da 0861 6e6e 6f75 6e63 6577 0000 0073  ...announcew...s
+00000e10: 1000 0000 0402 0201 0801 0201 0c01 04fc  ................
+00000e20: 0205 06fb 7a18 4163 7469 7669 7479 4661  ....z.ActivityFa
+00000e30: 6374 6f72 792e 616e 6e6f 756e 6365 6302  ctory.announcec.
+00000e40: 0000 0000 0000 0000 0000 0003 0000 0007  ................
+00000e50: 0000 004b 0000 0073 2400 0000 7400 6405  ...K...s$...t.d.
+00000e60: 6401 7c00 6a01 6402 1900 7c01 7402 7c01  d.|.j.d...|.t.|.
+00000e70: 6701 8301 6403 9c04 7c02 a401 8e01 5300  g...d...|.....S.
+00000e80: 2906 7a11 466f 6c6c 6f77 2066 6f72 206f  ).z.Follow for o
+00000e90: 626a 6563 745a 0646 6f6c 6c6f 7772 0a00  bjectZ.Followr..
+00000ea0: 0000 2904 7207 0000 0072 0800 0000 7213  ..).r....r....r.
+00000eb0: 0000 0072 0d00 0000 4e72 1800 0000 2903  ...r....Nr....).
+00000ec0: 7206 0000 0072 2b00 0000 7229 0000 0072  r....r+...r)...r
+00000ed0: 3300 0000 7218 0000 0072 1800 0000 7219  3...r....r....r.
+00000ee0: 0000 00da 0666 6f6c 6c6f 7781 0000 0073  .....follow....s
+00000ef0: 1000 0000 0402 0201 0801 0201 0801 04fc  ................
+00000f00: 0205 06fb 7a16 4163 7469 7669 7479 4661  ....z.ActivityFa
+00000f10: 6374 6f72 792e 666f 6c6c 6f77 4e29 0c72  ctory.followN).r
+00000f20: 2300 0000 7224 0000 0072 2500 0000 7226  #...r$...r%...r&
+00000f30: 0000 0072 2d00 0000 7236 0000 0072 3800  ...r-...r6...r8.
+00000f40: 0000 723d 0000 0072 4000 0000 7242 0000  ..r=...r@...rB..
+00000f50: 0072 4300 0000 7244 0000 0072 1800 0000  .rC...rD...r....
+00000f60: 7218 0000 0072 1800 0000 7219 0000 0072  r....r....r....r
+00000f70: 2a00 0000 4700 0000 7314 0000 0008 0004  *...G...s.......
+00000f80: 0108 0408 0308 0b08 0b08 0608 0608 060c  ................
+00000f90: 0a72 2a00 0000 4e29 08da 0b64 6174 6163  .r*...N)...datac
+00000fa0: 6c61 7373 6573 7202 0000 0072 0300 0000  lassesr....r....
+00000fb0: da06 7479 7069 6e67 7204 0000 0072 0500  ..typingr....r..
+00000fc0: 0000 7206 0000 0072 2a00 0000 7218 0000  ..r....r*...r...
+00000fd0: 0072 1800 0000 7218 0000 0072 1900 0000  .r....r....r....
+00000fe0: da08 3c6d 6f64 756c 653e 0100 0000 730a  ..<module>....s.
+00000ff0: 0000 0010 0010 0102 0310 0112 41         ............A
```

### Comparing `bovine-0.1.0/bovine/activitystreams/__pycache__/object_factory.cpython-310.pyc` & `bovine-0.1.1/bovine/activitystreams/__pycache__/object_factory.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 13 15:55:57 2023 UTC, .py size: 4240 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0d26 3864 9010 0000  o........&8d....
+00000000: 6f0d 0d0a 0000 0000 a4ea 3a64 9010 0000  o.........:d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5c00 0000 6400  .....@...s\...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 6d06 5a06 6d07 5a07 0100 6404 6405 6c08  m.Z.m.Z...d.d.l.
 00000060: 6d09 5a09 0100 6502 4700 6406 6407 8400  m.Z...e.G.d.d...
 00000070: 6407 8302 8301 5a0a 4700 6408 6409 8400  d.....Z.G.d.d...
@@ -59,198 +59,198 @@
 000003a0: 7c00 6a00 a001 6401 a101 0100 7c00 6a02  |.j...d.....|.j.
 000003b0: 7210 7c00 6a03 a001 7c00 6a02 a101 0100  r.|.j...|.j.....
 000003c0: 7c00 5300 a902 4e7a 2c68 7474 7073 3a2f  |.S...Nz,https:/
 000003d0: 2f77 7777 2e77 332e 6f72 672f 6e73 2f61  /www.w3.org/ns/a
 000003e0: 6374 6976 6974 7973 7472 6561 6d73 2350  ctivitystreams#P
 000003f0: 7562 6c69 6329 0472 1000 0000 da03 6164  ublic).r......ad
 00000400: 6472 0c00 0000 7211 0000 00a9 01da 0473  dr....r........s
-00000410: 656c 66a9 0072 2100 0000 fa59 2f77 6f6f  elf..r!....Y/woo
+00000410: 656c 66a9 0072 2100 0000 fa5a 2f77 6f6f  elf..r!....Z/woo
 00000420: 6470 6563 6b65 722f 7372 632f 636f 6465  dpecker/src/code
-00000430: 6265 7267 2e6f 7267 2f68 656c 6765 2f62  berg.org/helge/b
-00000440: 6f76 696e 652f 626f 7669 6e65 2f62 6f76  ovine/bovine/bov
-00000450: 696e 652f 6163 7469 7669 7479 7374 7265  ine/activitystre
-00000460: 616d 732f 6f62 6a65 6374 5f66 6163 746f  ams/object_facto
-00000470: 7279 2e70 79da 0961 735f 7075 626c 6963  ry.py..as_public
-00000480: 2300 0000 7308 0000 000c 0106 010e 0104  #...s...........
-00000490: 017a 104f 626a 6563 742e 6173 5f70 7562  .z.Object.as_pub
-000004a0: 6c69 6363 0100 0000 0000 0000 0000 0000  licc............
-000004b0: 0100 0000 0300 0000 4300 0000 7324 0000  ........C...s$..
-000004c0: 007c 006a 0072 0a7c 006a 01a0 027c 006a  .|.j.r.|.j...|.j
-000004d0: 00a1 0101 007c 006a 03a0 0264 01a1 0101  .....|.j...d....
-000004e0: 007c 0053 0072 1d00 0000 2904 720c 0000  .|.S.r....).r...
-000004f0: 0072 1000 0000 721e 0000 0072 1100 0000  .r....r....r....
-00000500: 721f 0000 0072 2100 0000 7221 0000 0072  r....r!...r!...r
-00000510: 2200 0000 da0b 6173 5f75 6e6c 6973 7465  ".....as_unliste
-00000520: 6429 0000 0073 0800 0000 0601 0e01 0c01  d)...s..........
-00000530: 0401 7a12 4f62 6a65 6374 2e61 735f 756e  ..z.Object.as_un
-00000540: 6c69 7374 6564 6301 0000 0000 0000 0000  listedc.........
-00000550: 0000 0005 0000 0005 0000 0043 0000 0073  ...........C...s
-00000560: fc00 0000 6401 7c00 6a00 6402 9c02 7d01  ....d.|.j.d...}.
-00000570: 6900 6403 7c00 6a01 9301 6404 7402 7c00  i.d.|.j...d.t.|.
-00000580: 6a03 8301 9301 6405 7402 7c00 6a04 7c00  j.....d.t.|.j.|.
-00000590: 6a03 1800 8301 9301 6406 7c00 6a05 9301  j.......d.|.j...
-000005a0: 6407 7c00 6a06 9301 6408 7c00 6a07 9301  d.|.j...d.|.j...
-000005b0: 6409 7c00 6a08 9301 640a 7c00 6a09 9301  d.|.j...d.|.j...
-000005c0: 640b 7c00 6a0a 9301 640c 7c00 6a0b 9301  d.|.j...d.|.j...
-000005d0: 640d 7c00 6a0c 9301 640e 7c00 6a0d 9301  d.|.j...d.|.j...
-000005e0: 640f 7c00 6a0e 9301 6410 7c00 6a0f 9301  d.|.j...d.|.j...
-000005f0: 6411 7c00 6a10 9301 6412 7c00 6a11 9301  d.|.j...d.|.j...
-00000600: 7d02 7c02 a012 a100 4400 5d0a 5c02 7d03  }.|.....D.].\.}.
-00000610: 7d04 7c04 725d 7c04 7c01 7c03 3c00 7153  }.|.r]|.|.|.<.qS
-00000620: 6404 7c01 7600 726d 7413 7c01 6404 1900  d.|.v.rmt.|.d...
-00000630: 8301 6413 6b02 726d 7c01 6404 3d00 6405  ..d.k.rm|.d.=.d.
-00000640: 7c01 7600 727c 7413 7c01 6405 1900 8301  |.v.r|t.|.d.....
-00000650: 6413 6b02 727c 7c01 6405 3d00 7c01 5300  d.k.r||.d.=.|.S.
-00000660: 2914 4e7a 2568 7474 7073 3a2f 2f77 7777  ).Nz%https://www
-00000670: 2e77 332e 6f72 672f 6e73 2f61 6374 6976  .w3.org/ns/activ
-00000680: 6974 7973 7472 6561 6d73 2902 7a08 4063  itystreams).z.@c
-00000690: 6f6e 7465 7874 720a 0000 00da 0c61 7474  ontextr......att
-000006a0: 7269 6275 7465 6454 6f72 1000 0000 7211  ributedTor....r.
-000006b0: 0000 0072 0d00 0000 5a09 696e 5265 706c  ...r....Z.inRepl
-000006c0: 7954 6f72 0e00 0000 7215 0000 0072 1200  yTor....r....r..
-000006d0: 0000 7219 0000 0072 1300 0000 7214 0000  ..r....r....r...
-000006e0: 0072 1a00 0000 721b 0000 0072 1c00 0000  .r....r....r....
-000006f0: 7216 0000 0072 1700 0000 7201 0000 0029  r....r....r....)
-00000700: 1472 0a00 0000 720b 0000 00da 046c 6973  .r....r......lis
-00000710: 7472 1000 0000 7211 0000 0072 0d00 0000  tr....r....r....
-00000720: 7218 0000 0072 0e00 0000 7215 0000 0072  r....r....r....r
-00000730: 1200 0000 7219 0000 0072 1300 0000 7214  ....r....r....r.
-00000740: 0000 0072 1a00 0000 721b 0000 0072 1c00  ...r....r....r..
-00000750: 0000 7216 0000 0072 1700 0000 da05 6974  ..r....r......it
-00000760: 656d 73da 036c 656e 2905 7220 0000 00da  ems..len).r ....
-00000770: 0672 6573 756c 74da 0c65 7874 7261 5f66  .result..extra_f
-00000780: 6965 6c64 73da 036b 6579 da05 7661 6c75  ields..key..valu
-00000790: 6572 2100 0000 7221 0000 0072 2200 0000  er!...r!...r"...
-000007a0: da05 6275 696c 642f 0000 0073 5a00 0000  ..build/...sZ...
-000007b0: 0202 0401 06fe 0205 0601 02ff 0a02 02fe  ................
-000007c0: 1003 02fd 0604 02fc 0605 02fb 0606 02fa  ................
-000007d0: 0607 02f9 0608 02f8 0609 02f7 060a 02f6  ................
-000007e0: 060b 02f5 060c 02f4 060d 02f3 060e 02f2  ................
-000007f0: 060f 02f1 0610 04f0 1013 0401 0801 0280  ................
-00000800: 1802 0601 1801 0601 0402 7a0c 4f62 6a65  ..........z.Obje
-00000810: 6374 2e62 7569 6c64 2922 da08 5f5f 6e61  ct.build)"..__na
-00000820: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
-00000830: da0c 5f5f 7175 616c 6e61 6d65 5f5f da07  ..__qualname__..
-00000840: 5f5f 646f 635f 5fda 0373 7472 da0f 5f5f  __doc__..str..__
-00000850: 616e 6e6f 7461 7469 6f6e 735f 5f72 0b00  annotations__r..
-00000860: 0000 7205 0000 0072 0c00 0000 720d 0000  ..r....r....r...
-00000870: 0072 0e00 0000 7203 0000 00da 0373 6574  .r....r......set
-00000880: 7210 0000 0072 0600 0000 7211 0000 0072  r....r....r....r
-00000890: 1200 0000 7213 0000 0072 1400 0000 7215  ....r....r....r.
-000008a0: 0000 00da 0464 6963 7472 1600 0000 da03  .....dictr......
-000008b0: 696e 7472 1700 0000 7218 0000 0072 1900  intr....r....r..
-000008c0: 0000 7226 0000 0072 1a00 0000 7204 0000  ..r&...r....r...
-000008d0: 0072 1b00 0000 721c 0000 0072 2300 0000  .r....r....r#...
-000008e0: 7224 0000 0072 2d00 0000 7221 0000 0072  r$...r-...r!...r
-000008f0: 2100 0000 7221 0000 0072 2200 0000 7209  !...r!...r"...r.
-00000900: 0000 0008 0000 0073 2e00 0000 0a00 0402  .......s........
-00000910: 0803 1001 1001 1001 1001 1601 1601 1002  ................
-00000920: 1001 1001 1001 1002 1001 1002 1001 1601  ................
-00000930: 1601 1001 0802 0806 0c06 7209 0000 0063  ..........r....c
-00000940: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000950: 0300 0000 4000 0000 733a 0000 0065 005a  ....@...s:...e.Z
-00000960: 0164 005a 0264 015a 0364 0d64 0364 0484  .d.Z.d.Z.d.d.d..
-00000970: 015a 0464 0564 0684 005a 0564 0764 0884  .Z.d.d...Z.d.d..
-00000980: 005a 0664 0964 0a84 005a 0764 0b64 0c84  .Z.d.d...Z.d.d..
-00000990: 005a 0864 0253 0029 0eda 0d4f 626a 6563  .Z.d.S.)...Objec
-000009a0: 7446 6163 746f 7279 7a34 4f62 6a65 6374  tFactoryz4Object
-000009b0: 4661 6374 6f72 7920 7573 7561 6c6c 7920  Factory usually 
-000009c0: 6372 6561 7465 6420 7468 726f 7567 6820  created through 
-000009d0: 6120 426f 7669 6e65 436c 6965 6e74 4e63  a BovineClientNc
-000009e0: 0300 0000 0000 0000 0000 0000 0300 0000  ................
-000009f0: 0200 0000 4300 0000 7332 0000 007c 0272  ....C...s2...|.r
-00000a00: 0b7c 027c 005f 007c 026a 017c 005f 0164  .|.|._.|.j.|._.d
-00000a10: 0053 007c 0172 1564 007c 005f 007c 017c  .S.|.r.d.|._.|.|
-00000a20: 005f 0164 0053 0074 0264 0183 0182 0129  ._.d.S.t.d.....)
-00000a30: 024e 7a3e 596f 7520 6e65 6564 2074 6f20  .Nz>You need to 
-00000a40: 6569 7468 6572 2073 7065 6369 6679 2061  either specify a
-00000a50: 6374 6f72 5f69 6e66 6f72 6d61 7469 6f6e  ctor_information
-00000a60: 206f 7220 6120 426f 7669 6e65 436c 6965   or a BovineClie
-00000a70: 6e74 2903 da06 636c 6965 6e74 da0b 696e  nt)...client..in
-00000a80: 666f 726d 6174 696f 6eda 0954 7970 6545  formation..TypeE
-00000a90: 7272 6f72 2903 7220 0000 00da 1161 6374  rror).r .....act
-00000aa0: 6f72 5f69 6e66 6f72 6d61 7469 6f6e 7238  or_informationr8
-00000ab0: 0000 0072 2100 0000 7221 0000 0072 2200  ...r!...r!...r".
-00000ac0: 0000 da08 5f5f 696e 6974 5f5f 5700 0000  ....__init__W...
-00000ad0: 7312 0000 0004 0106 010c 0104 0106 010a  s...............
-00000ae0: 0102 0202 0104 ff7a 164f 626a 6563 7446  .......z.ObjectF
-00000af0: 6163 746f 7279 2e5f 5f69 6e69 745f 5f63  actory.__init__c
-00000b00: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-00000b10: 0700 0000 4b00 0000 f324 0000 0074 0064  ....K....$...t.d
-00000b20: 067c 006a 0164 0119 0064 027c 006a 01a0  .|.j.d...d.|.j..
-00000b30: 0264 03a1 0164 049c 037c 01a4 018e 0153  .d...d...|.....S
-00000b40: 0029 077a 1543 7265 6174 6573 2061 204e  .).z.Creates a N
-00000b50: 6f74 6520 4f62 6a65 6374 720d 0000 005a  ote Objectr....Z
-00000b60: 044e 6f74 6572 0c00 0000 a903 720b 0000  .Noter......r...
-00000b70: 0072 0a00 0000 720c 0000 004e 7221 0000  .r....r....Nr!..
-00000b80: 00a9 0372 0900 0000 7239 0000 00da 0367  ...r....r9.....g
-00000b90: 6574 a902 7220 0000 00da 066b 7761 7267  et..r .....kwarg
-00000ba0: 7372 2100 0000 7221 0000 0072 2200 0000  sr!...r!...r"...
-00000bb0: da04 6e6f 7465 6300 0000 f30e 0000 0004  ..notec.........
-00000bc0: 0208 0102 010a 0104 fd02 0406 fc7a 124f  .............z.O
-00000bd0: 626a 6563 7446 6163 746f 7279 2e6e 6f74  bjectFactory.not
-00000be0: 6563 0100 0000 0000 0000 0000 0000 0200  ec..............
-00000bf0: 0000 0700 0000 4b00 0000 723d 0000 0029  ......K...r=...)
-00000c00: 077a 1943 7265 6174 6573 2061 6e20 4172  .z.Creates an Ar
-00000c10: 7469 636c 6520 4f62 6a65 6374 720d 0000  ticle Objectr...
-00000c20: 005a 0741 7274 6963 6c65 720c 0000 0072  .Z.Articler....r
-00000c30: 3e00 0000 4e72 2100 0000 723f 0000 0072  >...Nr!...r?...r
-00000c40: 4100 0000 7221 0000 0072 2100 0000 7222  A...r!...r!...r"
-00000c50: 0000 00da 0761 7274 6963 6c65 6c00 0000  .....articlel...
-00000c60: 7244 0000 007a 154f 626a 6563 7446 6163  rD...z.ObjectFac
-00000c70: 746f 7279 2e61 7274 6963 6c65 6301 0000  tory.articlec...
-00000c80: 0000 0000 0000 0000 0002 0000 0007 0000  ................
-00000c90: 004b 0000 0072 3d00 0000 2907 7a17 4372  .K...r=...).z.Cr
-00000ca0: 6561 7465 7320 616e 2045 7665 6e74 204f  eates an Event O
-00000cb0: 626a 6563 7472 0d00 0000 da05 4576 656e  bjectr......Even
-00000cc0: 7472 0c00 0000 723e 0000 004e 7221 0000  tr....r>...Nr!..
-00000cd0: 0072 3f00 0000 7241 0000 0072 2100 0000  .r?...rA...r!...
-00000ce0: 7221 0000 0072 2200 0000 da05 6576 656e  r!...r".....even
-00000cf0: 7475 0000 0072 4400 0000 7a13 4f62 6a65  tu...rD...z.Obje
-00000d00: 6374 4661 6374 6f72 792e 6576 656e 7463  ctFactory.eventc
-00000d10: 0200 0000 0000 0000 0000 0000 0400 0000  ................
-00000d20: 0500 0000 c300 0000 734a 0000 0081 017c  ........sJ.....|
-00000d30: 006a 0073 0874 0164 0183 0182 017c 006a  .j.s.t.d.....|.j
-00000d40: 006a 00a0 027c 01a1 0149 0064 0248 007d  .j...|...I.d.H.}
-00000d50: 0274 03a0 047c 02a0 05a1 0049 0064 0248  .t...|.....I.d.H
-00000d60: 00a1 017d 0374 0664 037c 0174 077c 0383  ...}.t.d.|.t.|..
-00000d70: 0164 048d 0353 0029 057a 8843 7265 6174  .d...S.).z.Creat
-00000d80: 6573 2061 206d 656e 7469 6f6e 206f 626a  es a mention obj
-00000d90: 6563 7420 666f 7220 616e 6f74 6865 7220  ect for another 
-00000da0: 6163 746f 722e 2052 6571 7569 7265 7320  actor. Requires 
-00000db0: 636c 6965 6e74 2074 6f20 6265 2073 6574  client to be set
-00000dc0: 2e0a 0a20 2020 2020 2020 203a 7061 7261  ...        :para
-00000dd0: 6d20 6163 746f 725f 746f 5f6d 656e 7469  m actor_to_menti
-00000de0: 6f6e 3a20 5468 6520 5552 4920 6f66 2074  on: The URI of t
-00000df0: 6865 2061 6374 6f72 2074 6f20 6d65 6e74  he actor to ment
-00000e00: 696f 6e7a 2663 6c69 656e 7420 6e65 6564  ionz&client need
-00000e10: 7320 746f 2062 6520 7365 7420 6174 2063  s to be set at c
-00000e20: 6f6e 7374 7275 6374 696f 6e4e 5a07 4d65  onstructionNZ.Me
-00000e30: 6e74 696f 6e29 0372 0a00 0000 721c 0000  ntion).r....r...
-00000e40: 0072 1200 0000 2908 7238 0000 0072 3a00  .r....).r8...r:.
-00000e50: 0000 7240 0000 00da 046a 736f 6eda 056c  ..r@.....json..l
-00000e60: 6f61 6473 da04 7465 7874 7209 0000 0072  oads..textr....r
-00000e70: 0800 0000 2904 7220 0000 005a 1061 6374  ....).r ...Z.act
-00000e80: 6f72 5f74 6f5f 6d65 6e74 696f 6eda 0872  or_to_mention..r
-00000e90: 6573 706f 6e73 655a 0c72 656d 6f74 655f  esponseZ.remote_
-00000ea0: 6163 746f 7272 2100 0000 7221 0000 0072  actorr!...r!...r
-00000eb0: 2200 0000 da15 6d65 6e74 696f 6e5f 666f  ".....mention_fo
-00000ec0: 725f 6163 746f 725f 7572 697e 0000 0073  r_actor_uri~...s
-00000ed0: 1400 0000 0280 0605 0801 1402 1401 0202  ................
-00000ee0: 0201 0201 0601 06fd 7a23 4f62 6a65 6374  ........z#Object
-00000ef0: 4661 6374 6f72 792e 6d65 6e74 696f 6e5f  Factory.mention_
-00000f00: 666f 725f 6163 746f 725f 7572 6929 024e  for_actor_uri).N
-00000f10: 4e29 0972 2e00 0000 722f 0000 0072 3000  N).r....r/...r0.
-00000f20: 0000 7231 0000 0072 3c00 0000 7243 0000  ..r1...r<...rC..
-00000f30: 0072 4500 0000 7247 0000 0072 4c00 0000  .rE...rG...rL...
-00000f40: 7221 0000 0072 2100 0000 7221 0000 0072  r!...r!...r!...r
-00000f50: 2200 0000 7237 0000 0054 0000 0073 0e00  "...r7...T...s..
-00000f60: 0000 0800 0401 0a02 080c 0809 0809 0c09  ................
-00000f70: 7237 0000 0029 0c72 4800 0000 da0b 6461  r7...).rH.....da
-00000f80: 7461 636c 6173 7365 7372 0200 0000 7203  taclassesr....r.
-00000f90: 0000 00da 0674 7970 696e 6772 0400 0000  .....typingr....
-00000fa0: 7205 0000 0072 0600 0000 da05 7574 696c  r....r......util
-00000fb0: 7372 0800 0000 7209 0000 0072 3700 0000  sr....r....r7...
-00000fc0: 7221 0000 0072 2100 0000 7221 0000 0072  r!...r!...r!...r
-00000fd0: 2200 0000 da08 3c6d 6f64 756c 653e 0100  ".....<module>..
-00000fe0: 0000 730e 0000 0008 0010 0114 010c 0202  ..s.............
-00000ff0: 0310 0112 4b                             ....K
+00000430: 6265 7267 2e6f 7267 2f62 6f76 696e 652f  berg.org/bovine/
+00000440: 626f 7669 6e65 2f62 6f76 696e 652f 626f  bovine/bovine/bo
+00000450: 7669 6e65 2f61 6374 6976 6974 7973 7472  vine/activitystr
+00000460: 6561 6d73 2f6f 626a 6563 745f 6661 6374  eams/object_fact
+00000470: 6f72 792e 7079 da09 6173 5f70 7562 6c69  ory.py..as_publi
+00000480: 6323 0000 0073 0800 0000 0c01 0601 0e01  c#...s..........
+00000490: 0401 7a10 4f62 6a65 6374 2e61 735f 7075  ..z.Object.as_pu
+000004a0: 626c 6963 6301 0000 0000 0000 0000 0000  blicc...........
+000004b0: 0001 0000 0003 0000 0043 0000 0073 2400  .........C...s$.
+000004c0: 0000 7c00 6a00 720a 7c00 6a01 a002 7c00  ..|.j.r.|.j...|.
+000004d0: 6a00 a101 0100 7c00 6a03 a002 6401 a101  j.....|.j...d...
+000004e0: 0100 7c00 5300 721d 0000 0029 0472 0c00  ..|.S.r....).r..
+000004f0: 0000 7210 0000 0072 1e00 0000 7211 0000  ..r....r....r...
+00000500: 0072 1f00 0000 7221 0000 0072 2100 0000  .r....r!...r!...
+00000510: 7222 0000 00da 0b61 735f 756e 6c69 7374  r".....as_unlist
+00000520: 6564 2900 0000 7308 0000 0006 010e 010c  ed)...s.........
+00000530: 0104 017a 124f 626a 6563 742e 6173 5f75  ...z.Object.as_u
+00000540: 6e6c 6973 7465 6463 0100 0000 0000 0000  nlistedc........
+00000550: 0000 0000 0500 0000 0500 0000 4300 0000  ............C...
+00000560: 73fc 0000 0064 017c 006a 0064 029c 027d  s....d.|.j.d...}
+00000570: 0169 0064 037c 006a 0193 0164 0474 027c  .i.d.|.j...d.t.|
+00000580: 006a 0383 0193 0164 0574 027c 006a 047c  .j.....d.t.|.j.|
+00000590: 006a 0318 0083 0193 0164 067c 006a 0593  .j.......d.|.j..
+000005a0: 0164 077c 006a 0693 0164 087c 006a 0793  .d.|.j...d.|.j..
+000005b0: 0164 097c 006a 0893 0164 0a7c 006a 0993  .d.|.j...d.|.j..
+000005c0: 0164 0b7c 006a 0a93 0164 0c7c 006a 0b93  .d.|.j...d.|.j..
+000005d0: 0164 0d7c 006a 0c93 0164 0e7c 006a 0d93  .d.|.j...d.|.j..
+000005e0: 0164 0f7c 006a 0e93 0164 107c 006a 0f93  .d.|.j...d.|.j..
+000005f0: 0164 117c 006a 1093 0164 127c 006a 1193  .d.|.j...d.|.j..
+00000600: 017d 027c 02a0 12a1 0044 005d 0a5c 027d  .}.|.....D.].\.}
+00000610: 037d 047c 0472 5d7c 047c 017c 033c 0071  .}.|.r]|.|.|.<.q
+00000620: 5364 047c 0176 0072 6d74 137c 0164 0419  Sd.|.v.rmt.|.d..
+00000630: 0083 0164 136b 0272 6d7c 0164 043d 0064  ...d.k.rm|.d.=.d
+00000640: 057c 0176 0072 7c74 137c 0164 0519 0083  .|.v.r|t.|.d....
+00000650: 0164 136b 0272 7c7c 0164 053d 007c 0153  .d.k.r||.d.=.|.S
+00000660: 0029 144e 7a25 6874 7470 733a 2f2f 7777  .).Nz%https://ww
+00000670: 772e 7733 2e6f 7267 2f6e 732f 6163 7469  w.w3.org/ns/acti
+00000680: 7669 7479 7374 7265 616d 7329 027a 0840  vitystreams).z.@
+00000690: 636f 6e74 6578 7472 0a00 0000 da0c 6174  contextr......at
+000006a0: 7472 6962 7574 6564 546f 7210 0000 0072  tributedTor....r
+000006b0: 1100 0000 720d 0000 005a 0969 6e52 6570  ....r....Z.inRep
+000006c0: 6c79 546f 720e 0000 0072 1500 0000 7212  lyTor....r....r.
+000006d0: 0000 0072 1900 0000 7213 0000 0072 1400  ...r....r....r..
+000006e0: 0000 721a 0000 0072 1b00 0000 721c 0000  ..r....r....r...
+000006f0: 0072 1600 0000 7217 0000 0072 0100 0000  .r....r....r....
+00000700: 2914 720a 0000 0072 0b00 0000 da04 6c69  ).r....r......li
+00000710: 7374 7210 0000 0072 1100 0000 720d 0000  str....r....r...
+00000720: 0072 1800 0000 720e 0000 0072 1500 0000  .r....r....r....
+00000730: 7212 0000 0072 1900 0000 7213 0000 0072  r....r....r....r
+00000740: 1400 0000 721a 0000 0072 1b00 0000 721c  ....r....r....r.
+00000750: 0000 0072 1600 0000 7217 0000 00da 0569  ...r....r......i
+00000760: 7465 6d73 da03 6c65 6e29 0572 2000 0000  tems..len).r ...
+00000770: da06 7265 7375 6c74 da0c 6578 7472 615f  ..result..extra_
+00000780: 6669 656c 6473 da03 6b65 79da 0576 616c  fields..key..val
+00000790: 7565 7221 0000 0072 2100 0000 7222 0000  uer!...r!...r"..
+000007a0: 00da 0562 7569 6c64 2f00 0000 735a 0000  ...build/...sZ..
+000007b0: 0002 0204 0106 fe02 0506 0102 ff0a 0202  ................
+000007c0: fe10 0302 fd06 0402 fc06 0502 fb06 0602  ................
+000007d0: fa06 0702 f906 0802 f806 0902 f706 0a02  ................
+000007e0: f606 0b02 f506 0c02 f406 0d02 f306 0e02  ................
+000007f0: f206 0f02 f106 1004 f010 1304 0108 0102  ................
+00000800: 8018 0206 0118 0106 0104 027a 0c4f 626a  ...........z.Obj
+00000810: 6563 742e 6275 696c 6429 22da 085f 5f6e  ect.build)"..__n
+00000820: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
+00000830: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5fda  _..__qualname__.
+00000840: 075f 5f64 6f63 5f5f da03 7374 72da 0f5f  .__doc__..str.._
+00000850: 5f61 6e6e 6f74 6174 696f 6e73 5f5f 720b  _annotations__r.
+00000860: 0000 0072 0500 0000 720c 0000 0072 0d00  ...r....r....r..
+00000870: 0000 720e 0000 0072 0300 0000 da03 7365  ..r....r......se
+00000880: 7472 1000 0000 7206 0000 0072 1100 0000  tr....r....r....
+00000890: 7212 0000 0072 1300 0000 7214 0000 0072  r....r....r....r
+000008a0: 1500 0000 da04 6469 6374 7216 0000 00da  ......dictr.....
+000008b0: 0369 6e74 7217 0000 0072 1800 0000 7219  .intr....r....r.
+000008c0: 0000 0072 2600 0000 721a 0000 0072 0400  ...r&...r....r..
+000008d0: 0000 721b 0000 0072 1c00 0000 7223 0000  ..r....r....r#..
+000008e0: 0072 2400 0000 722d 0000 0072 2100 0000  .r$...r-...r!...
+000008f0: 7221 0000 0072 2100 0000 7222 0000 0072  r!...r!...r"...r
+00000900: 0900 0000 0800 0000 732e 0000 000a 0004  ........s.......
+00000910: 0208 0310 0110 0110 0110 0116 0116 0110  ................
+00000920: 0210 0110 0110 0110 0210 0110 0210 0116  ................
+00000930: 0116 0110 0108 0208 060c 0672 0900 0000  ...........r....
+00000940: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+00000950: 0003 0000 0040 0000 0073 3a00 0000 6500  .....@...s:...e.
+00000960: 5a01 6400 5a02 6401 5a03 640d 6403 6404  Z.d.Z.d.Z.d.d.d.
+00000970: 8401 5a04 6405 6406 8400 5a05 6407 6408  ..Z.d.d...Z.d.d.
+00000980: 8400 5a06 6409 640a 8400 5a07 640b 640c  ..Z.d.d...Z.d.d.
+00000990: 8400 5a08 6402 5300 290e da0d 4f62 6a65  ..Z.d.S.)...Obje
+000009a0: 6374 4661 6374 6f72 797a 344f 626a 6563  ctFactoryz4Objec
+000009b0: 7446 6163 746f 7279 2075 7375 616c 6c79  tFactory usually
+000009c0: 2063 7265 6174 6564 2074 6872 6f75 6768   created through
+000009d0: 2061 2042 6f76 696e 6543 6c69 656e 744e   a BovineClientN
+000009e0: 6303 0000 0000 0000 0000 0000 0003 0000  c...............
+000009f0: 0002 0000 0043 0000 0073 3200 0000 7c02  .....C...s2...|.
+00000a00: 720b 7c02 7c00 5f00 7c02 6a01 7c00 5f01  r.|.|._.|.j.|._.
+00000a10: 6400 5300 7c01 7215 6400 7c00 5f00 7c01  d.S.|.r.d.|._.|.
+00000a20: 7c00 5f01 6400 5300 7402 6401 8301 8201  |._.d.S.t.d.....
+00000a30: 2902 4e7a 3e59 6f75 206e 6565 6420 746f  ).Nz>You need to
+00000a40: 2065 6974 6865 7220 7370 6563 6966 7920   either specify 
+00000a50: 6163 746f 725f 696e 666f 726d 6174 696f  actor_informatio
+00000a60: 6e20 6f72 2061 2042 6f76 696e 6543 6c69  n or a BovineCli
+00000a70: 656e 7429 03da 0663 6c69 656e 74da 0b69  ent)...client..i
+00000a80: 6e66 6f72 6d61 7469 6f6e da09 5479 7065  nformation..Type
+00000a90: 4572 726f 7229 0372 2000 0000 da11 6163  Error).r .....ac
+00000aa0: 746f 725f 696e 666f 726d 6174 696f 6e72  tor_informationr
+00000ab0: 3800 0000 7221 0000 0072 2100 0000 7222  8...r!...r!...r"
+00000ac0: 0000 00da 085f 5f69 6e69 745f 5f57 0000  .....__init__W..
+00000ad0: 0073 1200 0000 0401 0601 0c01 0401 0601  .s..............
+00000ae0: 0a01 0202 0201 04ff 7a16 4f62 6a65 6374  ........z.Object
+00000af0: 4661 6374 6f72 792e 5f5f 696e 6974 5f5f  Factory.__init__
+00000b00: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+00000b10: 0007 0000 004b 0000 00f3 2400 0000 7400  .....K....$...t.
+00000b20: 6406 7c00 6a01 6401 1900 6402 7c00 6a01  d.|.j.d...d.|.j.
+00000b30: a002 6403 a101 6404 9c03 7c01 a401 8e01  ..d...d...|.....
+00000b40: 5300 2907 7a15 4372 6561 7465 7320 6120  S.).z.Creates a 
+00000b50: 4e6f 7465 204f 626a 6563 7472 0d00 0000  Note Objectr....
+00000b60: 5a04 4e6f 7465 720c 0000 00a9 0372 0b00  Z.Noter......r..
+00000b70: 0000 720a 0000 0072 0c00 0000 4e72 2100  ..r....r....Nr!.
+00000b80: 0000 a903 7209 0000 0072 3900 0000 da03  ....r....r9.....
+00000b90: 6765 74a9 0272 2000 0000 da06 6b77 6172  get..r .....kwar
+00000ba0: 6773 7221 0000 0072 2100 0000 7222 0000  gsr!...r!...r"..
+00000bb0: 00da 046e 6f74 6563 0000 00f3 0e00 0000  ...notec........
+00000bc0: 0402 0801 0201 0a01 04fd 0204 06fc 7a12  ..............z.
+00000bd0: 4f62 6a65 6374 4661 6374 6f72 792e 6e6f  ObjectFactory.no
+00000be0: 7465 6301 0000 0000 0000 0000 0000 0002  tec.............
+00000bf0: 0000 0007 0000 004b 0000 0072 3d00 0000  .......K...r=...
+00000c00: 2907 7a19 4372 6561 7465 7320 616e 2041  ).z.Creates an A
+00000c10: 7274 6963 6c65 204f 626a 6563 7472 0d00  rticle Objectr..
+00000c20: 0000 5a07 4172 7469 636c 6572 0c00 0000  ..Z.Articler....
+00000c30: 723e 0000 004e 7221 0000 0072 3f00 0000  r>...Nr!...r?...
+00000c40: 7241 0000 0072 2100 0000 7221 0000 0072  rA...r!...r!...r
+00000c50: 2200 0000 da07 6172 7469 636c 656c 0000  ".....articlel..
+00000c60: 0072 4400 0000 7a15 4f62 6a65 6374 4661  .rD...z.ObjectFa
+00000c70: 6374 6f72 792e 6172 7469 636c 6563 0100  ctory.articlec..
+00000c80: 0000 0000 0000 0000 0000 0200 0000 0700  ................
+00000c90: 0000 4b00 0000 723d 0000 0029 077a 1743  ..K...r=...).z.C
+00000ca0: 7265 6174 6573 2061 6e20 4576 656e 7420  reates an Event 
+00000cb0: 4f62 6a65 6374 720d 0000 00da 0545 7665  Objectr......Eve
+00000cc0: 6e74 720c 0000 0072 3e00 0000 4e72 2100  ntr....r>...Nr!.
+00000cd0: 0000 723f 0000 0072 4100 0000 7221 0000  ..r?...rA...r!..
+00000ce0: 0072 2100 0000 7222 0000 00da 0565 7665  .r!...r".....eve
+00000cf0: 6e74 7500 0000 7244 0000 007a 134f 626a  ntu...rD...z.Obj
+00000d00: 6563 7446 6163 746f 7279 2e65 7665 6e74  ectFactory.event
+00000d10: 6302 0000 0000 0000 0000 0000 0004 0000  c...............
+00000d20: 0005 0000 00c3 0000 0073 4a00 0000 8101  .........sJ.....
+00000d30: 7c00 6a00 7308 7401 6401 8301 8201 7c00  |.j.s.t.d.....|.
+00000d40: 6a00 6a00 a002 7c01 a101 4900 6402 4800  j.j...|...I.d.H.
+00000d50: 7d02 7403 a004 7c02 a005 a100 4900 6402  }.t...|.....I.d.
+00000d60: 4800 a101 7d03 7406 6403 7c01 7407 7c03  H...}.t.d.|.t.|.
+00000d70: 8301 6404 8d03 5300 2905 7a88 4372 6561  ..d...S.).z.Crea
+00000d80: 7465 7320 6120 6d65 6e74 696f 6e20 6f62  tes a mention ob
+00000d90: 6a65 6374 2066 6f72 2061 6e6f 7468 6572  ject for another
+00000da0: 2061 6374 6f72 2e20 5265 7175 6972 6573   actor. Requires
+00000db0: 2063 6c69 656e 7420 746f 2062 6520 7365   client to be se
+00000dc0: 742e 0a0a 2020 2020 2020 2020 3a70 6172  t...        :par
+00000dd0: 616d 2061 6374 6f72 5f74 6f5f 6d65 6e74  am actor_to_ment
+00000de0: 696f 6e3a 2054 6865 2055 5249 206f 6620  ion: The URI of 
+00000df0: 7468 6520 6163 746f 7220 746f 206d 656e  the actor to men
+00000e00: 7469 6f6e 7a26 636c 6965 6e74 206e 6565  tionz&client nee
+00000e10: 6473 2074 6f20 6265 2073 6574 2061 7420  ds to be set at 
+00000e20: 636f 6e73 7472 7563 7469 6f6e 4e5a 074d  constructionNZ.M
+00000e30: 656e 7469 6f6e 2903 720a 0000 0072 1c00  ention).r....r..
+00000e40: 0000 7212 0000 0029 0872 3800 0000 723a  ..r....).r8...r:
+00000e50: 0000 0072 4000 0000 da04 6a73 6f6e da05  ...r@.....json..
+00000e60: 6c6f 6164 73da 0474 6578 7472 0900 0000  loads..textr....
+00000e70: 7208 0000 0029 0472 2000 0000 5a10 6163  r....).r ...Z.ac
+00000e80: 746f 725f 746f 5f6d 656e 7469 6f6e da08  tor_to_mention..
+00000e90: 7265 7370 6f6e 7365 5a0c 7265 6d6f 7465  responseZ.remote
+00000ea0: 5f61 6374 6f72 7221 0000 0072 2100 0000  _actorr!...r!...
+00000eb0: 7222 0000 00da 156d 656e 7469 6f6e 5f66  r".....mention_f
+00000ec0: 6f72 5f61 6374 6f72 5f75 7269 7e00 0000  or_actor_uri~...
+00000ed0: 7314 0000 0002 8006 0508 0114 0214 0102  s...............
+00000ee0: 0202 0102 0106 0106 fd7a 234f 626a 6563  .........z#Objec
+00000ef0: 7446 6163 746f 7279 2e6d 656e 7469 6f6e  tFactory.mention
+00000f00: 5f66 6f72 5f61 6374 6f72 5f75 7269 2902  _for_actor_uri).
+00000f10: 4e4e 2909 722e 0000 0072 2f00 0000 7230  NN).r....r/...r0
+00000f20: 0000 0072 3100 0000 723c 0000 0072 4300  ...r1...r<...rC.
+00000f30: 0000 7245 0000 0072 4700 0000 724c 0000  ..rE...rG...rL..
+00000f40: 0072 2100 0000 7221 0000 0072 2100 0000  .r!...r!...r!...
+00000f50: 7222 0000 0072 3700 0000 5400 0000 730e  r"...r7...T...s.
+00000f60: 0000 0008 0004 010a 0208 0c08 0908 090c  ................
+00000f70: 0972 3700 0000 290c 7248 0000 00da 0b64  .r7...).rH.....d
+00000f80: 6174 6163 6c61 7373 6573 7202 0000 0072  ataclassesr....r
+00000f90: 0300 0000 da06 7479 7069 6e67 7204 0000  ......typingr...
+00000fa0: 0072 0500 0000 7206 0000 00da 0575 7469  .r....r......uti
+00000fb0: 6c73 7208 0000 0072 0900 0000 7237 0000  lsr....r....r7..
+00000fc0: 0072 2100 0000 7221 0000 0072 2100 0000  .r!...r!...r!...
+00000fd0: 7222 0000 00da 083c 6d6f 6475 6c65 3e01  r".....<module>.
+00000fe0: 0000 0073 0e00 0000 0800 1001 1401 0c02  ...s............
+00000ff0: 0203 1001 124b                           .....K
```

### Comparing `bovine-0.1.0/bovine/activitystreams/__pycache__/test_activity_factory.cpython-310-pytest-7.3.0.pyc` & `bovine-0.1.1/bovine/activitystreams/__pycache__/test_activity_factory.cpython-310-pytest-7.3.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 13 15:55:57 2023 UTC, .py size: 2163 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0d26 3864 7308 0000  o........&8ds...
+00000000: 6f0d 0d0a 0000 0000 a4ea 3a64 7308 0000  o.........:ds...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 5e00 0000 6400  .....@...s^...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6402 6403 6c06 6d07  ..m.Z...d.d.l.m.
 00000050: 5a07 0100 6402 6404 6c08 6d09 5a09 0100  Z...d.d.l.m.Z...
 00000060: 6405 6406 8400 5a0a 6407 6408 8400 5a0b  d.d...Z.d.d...Z.
 00000070: 6409 640a 8400 5a0c 640b 640c 8400 5a0d  d.d...Z.d.d...Z.
@@ -64,222 +64,222 @@
 000003f0: 7870 6c61 6e61 7469 6f6e 2908 da10 6163  xplanation)...ac
 00000400: 7469 7669 7479 5f66 6163 746f 7279 7219  tivity_factoryr.
 00000410: 0000 00da 0672 6573 756c 74da 0b40 7079  .....result..@py
 00000420: 5f61 7373 6572 7430 da0b 4070 795f 6173  _assert0..@py_as
 00000430: 7365 7274 33da 0b40 7079 5f61 7373 6572  sert3..@py_asser
 00000440: 7432 da0b 4070 795f 666f 726d 6174 35da  t2..@py_format5.
 00000450: 0b40 7079 5f66 6f72 6d61 7437 a900 7229  .@py_format7..r)
-00000460: 0000 00fa 602f 776f 6f64 7065 636b 6572  ....`/woodpecker
+00000460: 0000 00fa 612f 776f 6f64 7065 636b 6572  ....a/woodpecker
 00000470: 2f73 7263 2f63 6f64 6562 6572 672e 6f72  /src/codeberg.or
-00000480: 672f 6865 6c67 652f 626f 7669 6e65 2f62  g/helge/bovine/b
-00000490: 6f76 696e 652f 626f 7669 6e65 2f61 6374  ovine/bovine/act
-000004a0: 6976 6974 7973 7472 6561 6d73 2f74 6573  ivitystreams/tes
-000004b0: 745f 6163 7469 7669 7479 5f66 6163 746f  t_activity_facto
-000004c0: 7279 2e70 79da 1a74 6573 745f 6163 7469  ry.py..test_acti
-000004d0: 7669 7479 5f66 6163 746f 7279 5f6c 696b  vity_factory_lik
-000004e0: 6505 0000 0073 1400 0000 0e01 0a02 0c01  e....s..........
-000004f0: 0c01 0601 0802 6a02 6c02 6c01 6e02 722b  ......j.l.l.n.r+
-00000500: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-00000510: 0800 0000 0700 0000 4300 0000 73d4 0100  ........C...s...
-00000520: 0074 0064 0164 0264 039c 0283 017d 007c  .t.d.d.d.....}.|
-00000530: 00a0 0164 0464 0569 01a1 017d 017c 01a0  ...d.d.i...}.|..
-00000540: 02a1 007d 027c 0264 0619 007d 0364 077d  ...}.|.d...}.d.}
-00000550: 047c 037c 046b 027d 057c 0573 4174 03a0  .|.|.k.}.|.sAt..
-00000560: 0464 087c 0566 0164 097c 037c 0466 02a1  .d.|.f.d.|.|.f..
-00000570: 0474 03a0 057c 03a1 0174 03a0 057c 04a1  .t...|...t...|..
-00000580: 0164 0a9c 0216 007d 0664 0b64 0c7c 0669  .d.....}.d.d.|.i
-00000590: 0116 007d 0774 0674 03a0 077c 07a1 0183  ...}.t.t...|....
-000005a0: 0182 0164 0004 007d 0304 007d 057d 047c  ...d...}...}.}.|
-000005b0: 0264 0d19 007d 0364 0e7d 047c 037c 046b  .d...}.d.}.|.|.k
-000005c0: 027d 057c 0573 7674 03a0 0464 087c 0566  .}.|.svt...d.|.f
-000005d0: 0164 097c 037c 0466 02a1 0474 03a0 057c  .d.|.|.f...t...|
-000005e0: 03a1 0174 03a0 057c 04a1 0164 0a9c 0216  ...t...|...d....
-000005f0: 007d 0664 0b64 0c7c 0669 0116 007d 0774  .}.d.d.|.i...}.t
-00000600: 0674 03a0 077c 07a1 0183 0182 0164 0004  .t...|.......d..
-00000610: 007d 0304 007d 057d 047c 0264 0f19 007d  .}...}.}.|.d...}
-00000620: 0364 017d 047c 037c 046b 027d 057c 0573  .d.}.|.|.k.}.|.s
-00000630: ab74 03a0 0464 087c 0566 0164 097c 037c  .t...d.|.f.d.|.|
-00000640: 0466 02a1 0474 03a0 057c 03a1 0174 03a0  .f...t...|...t..
-00000650: 057c 04a1 0164 0a9c 0216 007d 0664 0b64  .|...d.....}.d.d
-00000660: 0c7c 0669 0116 007d 0774 0674 03a0 077c  .|.i...}.t.t...|
-00000670: 07a1 0183 0182 0164 0004 007d 0304 007d  .......d...}...}
-00000680: 057d 047c 0264 1019 0064 0419 007d 0364  .}.|.d...d...}.d
-00000690: 057d 047c 037c 046b 027d 057c 0573 e274  .}.|.|.k.}.|.s.t
-000006a0: 03a0 0464 087c 0566 0164 097c 037c 0466  ...d.|.f.d.|.|.f
-000006b0: 02a1 0474 03a0 057c 03a1 0174 03a0 057c  ...t...|...t...|
-000006c0: 04a1 0164 0a9c 0216 007d 0664 0b64 0c7c  ...d.....}.d.d.|
-000006d0: 0669 0116 007d 0774 0674 03a0 077c 07a1  .i...}.t.t...|..
-000006e0: 0183 0182 0164 0004 007d 0304 007d 057d  .....d...}...}.}
-000006f0: 0464 0053 0029 114e 7205 0000 0072 0600  .d.S.).Nr....r..
-00000700: 0000 7207 0000 0072 0800 0000 da03 6f62  ..r....r......ob
-00000710: 6a72 0b00 0000 720c 0000 0072 0d00 0000  jr....r....r....
-00000720: 720f 0000 0072 1000 0000 7213 0000 0072  r....r....r....r
-00000730: 1400 0000 7217 0000 00da 0641 6363 6570  ....r......Accep
-00000740: 74da 0561 6374 6f72 da06 6f62 6a65 6374  t..actor..object
-00000750: 2908 7203 0000 00da 0661 6363 6570 7472  ).r......acceptr
-00000760: 1c00 0000 721d 0000 0072 1e00 0000 721f  ....r....r....r.
-00000770: 0000 0072 2000 0000 7221 0000 0029 0872  ...r ...r!...).r
-00000780: 2200 0000 7230 0000 0072 2300 0000 7224  "...r0...r#...r$
-00000790: 0000 0072 2500 0000 7226 0000 0072 2700  ...r%...r&...r'.
-000007a0: 0000 7228 0000 0072 2900 0000 7229 0000  ..r(...r)...r)..
-000007b0: 0072 2a00 0000 da1c 7465 7374 5f61 6374  .r*.....test_act
-000007c0: 6976 6974 795f 6661 6374 6f72 795f 6163  ivity_factory_ac
-000007d0: 6365 7074 1700 0000 730e 0000 000e 010e  cept....s.......
-000007e0: 0208 016a 026a 016a 0172 0172 3100 0000  ...j.j.j.r.r1...
-000007f0: 6300 0000 0000 0000 0000 0000 0008 0000  c...............
-00000800: 0007 0000 0043 0000 0073 7801 0000 7400  .....C...sx...t.
-00000810: 6401 6402 6403 9c02 8301 7d00 7401 6404  d.d.d.....}.t.d.
-00000820: 6401 6405 6406 8d03 a002 a100 a003 a100  d.d.d...........
-00000830: 7d01 7c00 a004 7c01 a101 a003 a100 7d02  }.|...|.......}.
-00000840: 7c02 6407 1900 7d03 6405 6701 7d04 7c03  |.d...}.d.g.}.|.
-00000850: 7c04 6b02 7d05 7c05 7349 7405 a006 6408  |.k.}.|.sIt...d.
-00000860: 7c05 6601 6409 7c03 7c04 6602 a104 7405  |.f.d.|.|.f...t.
-00000870: a007 7c03 a101 7405 a007 7c04 a101 640a  ..|...t...|...d.
-00000880: 9c02 1600 7d06 640b 640c 7c06 6901 1600  ....}.d.d.|.i...
-00000890: 7d07 7408 7405 a009 7c07 a101 8301 8201  }.t.t...|.......
-000008a0: 6400 0400 7d03 0400 7d05 7d04 7c02 640d  d...}...}.}.|.d.
-000008b0: 1900 7d03 640e 6701 7d04 7c03 7c04 6b02  ..}.d.g.}.|.|.k.
-000008c0: 7d05 7c05 737f 7405 a006 6408 7c05 6601  }.|.s.t...d.|.f.
-000008d0: 6409 7c03 7c04 6602 a104 7405 a007 7c03  d.|.|.f...t...|.
-000008e0: a101 7405 a007 7c04 a101 640a 9c02 1600  ..t...|...d.....
-000008f0: 7d06 640b 640c 7c06 6901 1600 7d07 7408  }.d.d.|.i...}.t.
-00000900: 7405 a009 7c07 a101 8301 8201 6400 0400  t...|.......d...
-00000910: 7d03 0400 7d05 7d04 7c02 640f 1900 7d03  }...}.}.|.d...}.
-00000920: 6401 7d04 7c03 7c04 6b02 7d05 7c05 73b4  d.}.|.|.k.}.|.s.
-00000930: 7405 a006 6408 7c05 6601 6409 7c03 7c04  t...d.|.f.d.|.|.
-00000940: 6602 a104 7405 a007 7c03 a101 7405 a007  f...t...|...t...
-00000950: 7c04 a101 640a 9c02 1600 7d06 640b 640c  |...d.....}.d.d.
-00000960: 7c06 6901 1600 7d07 7408 7405 a009 7c07  |.i...}.t.t...|.
-00000970: a101 8301 8201 6400 0400 7d03 0400 7d05  ......d...}...}.
-00000980: 7d04 6400 5300 2910 4e72 0500 0000 7206  }.d.S.).Nr....r.
-00000990: 0000 0072 0700 0000 da04 4e6f 7465 fa11  ...r......Note..
-000009a0: 6163 636f 756e 742f 666f 6c6c 6f77 6572  account/follower
-000009b0: 7329 0372 1700 0000 da0d 6174 7472 6962  s).r......attrib
-000009c0: 7574 6564 5f74 6f72 0600 0000 7216 0000  uted_tor....r...
-000009d0: 0072 0d00 0000 720f 0000 0072 1000 0000  .r....r....r....
-000009e0: 7213 0000 0072 1400 0000 7215 0000 007a  r....r....r....z
-000009f0: 2c68 7474 7073 3a2f 2f77 7777 2e77 332e  ,https://www.w3.
-00000a00: 6f72 672f 6e73 2f61 6374 6976 6974 7973  org/ns/activitys
-00000a10: 7472 6561 6d73 2350 7562 6c69 6372 2e00  treams#Publicr..
-00000a20: 0000 290a 7203 0000 0072 0400 0000 da09  ..).r....r......
-00000a30: 6173 5f70 7562 6c69 6372 1c00 0000 da06  as_publicr......
-00000a40: 6372 6561 7465 721d 0000 0072 1e00 0000  creater....r....
-00000a50: 721f 0000 0072 2000 0000 7221 0000 0029  r....r ...r!...)
-00000a60: 0872 2200 0000 da04 6e6f 7465 7223 0000  .r".....noter#..
-00000a70: 0072 2400 0000 7225 0000 0072 2600 0000  .r$...r%...r&...
-00000a80: 7227 0000 0072 2800 0000 7229 0000 0072  r'...r(...r)...r
-00000a90: 2900 0000 722a 0000 00da 1c74 6573 745f  )...r*.....test_
-00000aa0: 6163 7469 7669 7479 5f66 6163 746f 7279  activity_factory
-00000ab0: 5f63 7265 6174 6523 0000 0073 1200 0000  _create#...s....
-00000ac0: 0e01 0c02 0401 0401 02fd 0e06 6c02 6c01  ............l.l.
-00000ad0: 6e01 7238 0000 0063 0000 0000 0000 0000  n.r8...c........
-00000ae0: 0000 0000 0b00 0000 0700 0000 4300 0000  ............C...
-00000af0: 7388 0100 0074 0064 0164 0264 039c 0283  s....t.d.d.d....
-00000b00: 017d 0064 047d 0174 0164 0564 0164 067c  .}.d.}.t.d.d.d.|
-00000b10: 0168 0164 078d 04a0 02a1 007d 027c 00a0  .h.d.......}.|..
-00000b20: 037c 02a1 01a0 02a1 007d 0364 087d 047c  .|.......}.d.}.|
-00000b30: 047c 0376 017d 057c 0573 5374 04a0 0564  .|.v.}.|.sSt...d
-00000b40: 097c 0566 0164 0a7c 047c 0366 02a1 0474  .|.f.d.|.|.f...t
-00000b50: 04a0 067c 04a1 0164 0b74 07a0 08a1 0076  ...|...d.t.....v
-00000b60: 0073 3c74 04a0 097c 03a1 0172 4174 04a0  .s<t...|...rAt..
-00000b70: 067c 03a1 016e 0164 0b64 0c9c 0216 007d  .|...n.d.d.....}
-00000b80: 0664 0d64 0e7c 0669 0116 007d 0774 0a74  .d.d.|.i...}.t.t
-00000b90: 04a0 0b7c 07a1 0183 0182 0164 0004 007d  ...|.......d...}
-00000ba0: 047d 057c 0364 0f19 007d 047c 0167 017d  .}.|.d...}.|.g.}
-00000bb0: 087c 047c 086b 027d 057c 0573 8774 04a0  .|.|.k.}.|.s.t..
-00000bc0: 0564 107c 0566 0164 117c 047c 0866 02a1  .d.|.f.d.|.|.f..
-00000bd0: 0474 04a0 067c 04a1 0174 04a0 067c 08a1  .t...|...t...|..
-00000be0: 0164 129c 0216 007d 0964 1364 147c 0969  .d.....}.d.d.|.i
-00000bf0: 0116 007d 0a74 0a74 04a0 0b7c 0aa1 0183  ...}.t.t...|....
-00000c00: 0182 0164 0004 007d 0404 007d 057d 087c  ...d...}...}.}.|
-00000c10: 0364 1519 007d 0464 017d 087c 047c 086b  .d...}.d.}.|.|.k
-00000c20: 027d 057c 0573 bc74 04a0 0564 107c 0566  .}.|.s.t...d.|.f
-00000c30: 0164 117c 047c 0866 02a1 0474 04a0 067c  .d.|.|.f...t...|
-00000c40: 04a1 0174 04a0 067c 08a1 0164 129c 0216  ...t...|...d....
-00000c50: 007d 0964 1364 147c 0969 0116 007d 0a74  .}.d.d.|.i...}.t
-00000c60: 0a74 04a0 0b7c 0aa1 0183 0182 0164 0004  .t...|.......d..
-00000c70: 007d 0404 007d 057d 0864 0053 0029 164e  .}...}.}.d.S.).N
-00000c80: 7205 0000 0072 0600 0000 7207 0000 007a  r....r....r....z
-00000c90: 1268 7474 7073 3a2f 2f61 6265 6c2f 616c  .https://abel/al
-00000ca0: 6963 6572 3200 0000 7233 0000 0029 0472  icer2...r3...).r
-00000cb0: 1700 0000 7234 0000 0072 0600 0000 7215  ....r4...r....r.
-00000cc0: 0000 0072 1600 0000 2901 fa06 6e6f 7420  ...r....)...not 
-00000cd0: 696e 2901 7a16 2528 7079 3129 7320 6e6f  in).z.%(py1)s no
-00000ce0: 7420 696e 2025 2870 7933 2973 7223 0000  t in %(py3)sr#..
-00000cf0: 0029 0272 1100 0000 da03 7079 337a 0e61  .).r......py3z.a
-00000d00: 7373 6572 7420 2528 7079 3529 73da 0370  ssert %(py5)s..p
-00000d10: 7935 7215 0000 0072 0d00 0000 720f 0000  y5r....r....r...
-00000d20: 0072 1000 0000 7213 0000 0072 1400 0000  .r....r....r....
-00000d30: 722e 0000 0029 0c72 0300 0000 7204 0000  r....).r....r...
-00000d40: 0072 1c00 0000 7236 0000 0072 1d00 0000  .r....r6...r....
-00000d50: 721e 0000 0072 1f00 0000 da0c 4070 795f  r....r......@py_
-00000d60: 6275 696c 7469 6e73 da06 6c6f 6361 6c73  builtins..locals
-00000d70: da18 5f73 686f 756c 645f 7265 7072 5f67  .._should_repr_g
-00000d80: 6c6f 6261 6c5f 6e61 6d65 7220 0000 0072  lobal_namer ...r
-00000d90: 2100 0000 290b 7222 0000 00da 0c72 656d  !...).r".....rem
-00000da0: 6f74 655f 6163 746f 7272 3700 0000 7223  ote_actorr7...r#
-00000db0: 0000 0072 2400 0000 7226 0000 00da 0b40  ...r$...r&.....@
-00000dc0: 7079 5f66 6f72 6d61 7434 da0b 4070 795f  py_format4..@py_
-00000dd0: 666f 726d 6174 3672 2500 0000 7227 0000  format6r%...r'..
-00000de0: 0072 2800 0000 7229 0000 0072 2900 0000  .r(...r)...r)...
-00000df0: 722a 0000 00da 2274 6573 745f 6163 7469  r*...."test_acti
-00000e00: 7669 7479 5f66 6163 746f 7279 5f63 7265  vity_factory_cre
-00000e10: 6174 655f 6e6f 5f63 6332 0000 0073 1c00  ate_no_cc2...s..
-00000e20: 0000 0e01 0401 0201 0201 0201 0201 0401  ................
-00000e30: 04fc 0405 02fb 0e07 7802 6c01 6e01 7242  ........x.l.n.rB
-00000e40: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-00000e50: 0900 0000 0900 0000 4300 0000 73f6 0000  ........C...s...
-00000e60: 0074 0064 0164 0264 039c 0283 017d 007c  .t.d.d.d.....}.|
-00000e70: 00a0 0164 04a1 01a0 02a1 007d 017c 016a  ...d.......}.|.j
-00000e80: 037d 027c 0283 007d 0374 047c 0383 017d  .}.|...}.t.|...}
-00000e90: 0468 0064 05a3 017d 057c 047c 056b 027d  .h.d...}.|.|.k.}
-00000ea0: 067c 0673 6f74 05a0 0664 067c 0666 0164  .|.sot...d.|.f.d
-00000eb0: 077c 047c 0566 02a1 0464 0874 07a0 08a1  .|.|.f...d.t....
-00000ec0: 0076 0073 3774 05a0 0974 04a1 0172 3c74  .v.s7t...t...r<t
-00000ed0: 05a0 0a74 04a1 016e 0164 0864 0974 07a0  ...t...n.d.d.t..
-00000ee0: 08a1 0076 0073 4874 05a0 097c 01a1 0172  ...v.sHt...|...r
-00000ef0: 4d74 05a0 0a7c 01a1 016e 0164 0974 05a0  Mt...|...n.d.t..
-00000f00: 0a7c 02a1 0174 05a0 0a7c 03a1 0174 05a0  .|...t...|...t..
-00000f10: 0a7c 04a1 0174 05a0 0a7c 05a1 0164 0a9c  .|...t...|...d..
-00000f20: 0616 007d 0764 0b64 0c7c 0769 0116 007d  ...}.d.d.|.i...}
-00000f30: 0874 0b74 05a0 0c7c 08a1 0183 0182 0164  .t.t...|.......d
-00000f40: 0004 007d 0204 007d 0304 007d 0404 007d  ...}...}...}...}
-00000f50: 067d 0564 0053 0029 0d4e 7205 0000 0072  .}.d.S.).Nr....r
-00000f60: 0600 0000 7207 0000 0072 0900 0000 3e04  ....r....r....>.
-00000f70: 0000 0072 2e00 0000 722f 0000 0072 1700  ...r....r/...r..
-00000f80: 0000 720b 0000 0072 0d00 0000 2901 7a62  ..r....r....).zb
-00000f90: 2528 7079 3729 730a 7b25 2870 7937 2973  %(py7)s.{%(py7)s
-00000fa0: 203d 2025 2870 7930 2973 2825 2870 7935   = %(py0)s(%(py5
-00000fb0: 2973 0a7b 2528 7079 3529 7320 3d20 2528  )s.{%(py5)s = %(
-00000fc0: 7079 3329 730a 7b25 2870 7933 2973 203d  py3)s.{%(py3)s =
-00000fd0: 2025 2870 7931 2973 2e6b 6579 730a 7d28   %(py1)s.keys.}(
-00000fe0: 290a 7d29 0a7d 203d 3d20 2528 7079 3130  ).}).} == %(py10
-00000ff0: 2973 da03 7365 7472 2300 0000 2906 da03  )s..setr#...)...
-00001000: 7079 3072 1100 0000 723a 0000 0072 3b00  py0r....r:...r;.
-00001010: 0000 da03 7079 375a 0470 7931 307a 0f61  ....py7Z.py10z.a
-00001020: 7373 6572 7420 2528 7079 3132 2973 5a04  ssert %(py12)sZ.
-00001030: 7079 3132 290d 7203 0000 00da 0664 656c  py12).r......del
-00001040: 6574 6572 1c00 0000 da04 6b65 7973 7243  eter......keysrC
-00001050: 0000 0072 1d00 0000 721e 0000 0072 3c00  ...r....r....r<.
-00001060: 0000 723d 0000 0072 3e00 0000 721f 0000  ..r=...r>...r...
-00001070: 0072 2000 0000 7221 0000 0029 0972 2200  .r ...r!...).r".
-00001080: 0000 7223 0000 0072 2600 0000 da0b 4070  ..r#...r&.....@p
-00001090: 795f 6173 7365 7274 345a 0b40 7079 5f61  y_assert4Z.@py_a
-000010a0: 7373 6572 7436 5a0b 4070 795f 6173 7365  ssert6Z.@py_asse
-000010b0: 7274 395a 0b40 7079 5f61 7373 6572 7438  rt9Z.@py_assert8
-000010c0: 5a0c 4070 795f 666f 726d 6174 3131 5a0c  Z.@py_format11Z.
-000010d0: 4070 795f 666f 726d 6174 3133 7229 0000  @py_format13r)..
-000010e0: 0072 2900 0000 722a 0000 00da 1c74 6573  .r)...r*.....tes
-000010f0: 745f 6163 7469 7669 7479 5f6e 6f5f 656d  t_activity_no_em
-00001100: 7074 795f 746f 5f63 6343 0000 0073 0600  pty_to_ccC...s..
-00001110: 0000 0e01 0e02 da02 7249 0000 0029 0fda  ........rI...)..
-00001120: 0862 7569 6c74 696e 7372 3c00 0000 da19  .builtinsr<.....
-00001130: 5f70 7974 6573 742e 6173 7365 7274 696f  _pytest.assertio
-00001140: 6e2e 7265 7772 6974 65da 0961 7373 6572  n.rewrite..asser
-00001150: 7469 6f6e da07 7265 7772 6974 6572 1d00  tion..rewriter..
-00001160: 0000 7222 0000 0072 0300 0000 da0e 6f62  ..r"...r......ob
-00001170: 6a65 6374 5f66 6163 746f 7279 7204 0000  ject_factoryr...
-00001180: 0072 2b00 0000 7231 0000 0072 3800 0000  .r+...r1...r8...
-00001190: 7242 0000 0072 4900 0000 7229 0000 0072  rB...rI...r)...r
-000011a0: 2900 0000 7229 0000 0072 2a00 0000 da08  )...r)...r*.....
-000011b0: 3c6d 6f64 756c 653e 0100 0000 730e 0000  <module>....s...
-000011c0: 0026 000c 0108 0308 1208 0c08 0f0c 11    .&.............
+00000480: 672f 626f 7669 6e65 2f62 6f76 696e 652f  g/bovine/bovine/
+00000490: 626f 7669 6e65 2f62 6f76 696e 652f 6163  bovine/bovine/ac
+000004a0: 7469 7669 7479 7374 7265 616d 732f 7465  tivitystreams/te
+000004b0: 7374 5f61 6374 6976 6974 795f 6661 6374  st_activity_fact
+000004c0: 6f72 792e 7079 da1a 7465 7374 5f61 6374  ory.py..test_act
+000004d0: 6976 6974 795f 6661 6374 6f72 795f 6c69  ivity_factory_li
+000004e0: 6b65 0500 0000 7314 0000 000e 010a 020c  ke....s.........
+000004f0: 010c 0106 0108 026a 026c 026c 016e 0272  .......j.l.l.n.r
+00000500: 2b00 0000 6300 0000 0000 0000 0000 0000  +...c...........
+00000510: 0008 0000 0007 0000 0043 0000 0073 d401  .........C...s..
+00000520: 0000 7400 6401 6402 6403 9c02 8301 7d00  ..t.d.d.d.....}.
+00000530: 7c00 a001 6404 6405 6901 a101 7d01 7c01  |...d.d.i...}.|.
+00000540: a002 a100 7d02 7c02 6406 1900 7d03 6407  ....}.|.d...}.d.
+00000550: 7d04 7c03 7c04 6b02 7d05 7c05 7341 7403  }.|.|.k.}.|.sAt.
+00000560: a004 6408 7c05 6601 6409 7c03 7c04 6602  ..d.|.f.d.|.|.f.
+00000570: a104 7403 a005 7c03 a101 7403 a005 7c04  ..t...|...t...|.
+00000580: a101 640a 9c02 1600 7d06 640b 640c 7c06  ..d.....}.d.d.|.
+00000590: 6901 1600 7d07 7406 7403 a007 7c07 a101  i...}.t.t...|...
+000005a0: 8301 8201 6400 0400 7d03 0400 7d05 7d04  ....d...}...}.}.
+000005b0: 7c02 640d 1900 7d03 640e 7d04 7c03 7c04  |.d...}.d.}.|.|.
+000005c0: 6b02 7d05 7c05 7376 7403 a004 6408 7c05  k.}.|.svt...d.|.
+000005d0: 6601 6409 7c03 7c04 6602 a104 7403 a005  f.d.|.|.f...t...
+000005e0: 7c03 a101 7403 a005 7c04 a101 640a 9c02  |...t...|...d...
+000005f0: 1600 7d06 640b 640c 7c06 6901 1600 7d07  ..}.d.d.|.i...}.
+00000600: 7406 7403 a007 7c07 a101 8301 8201 6400  t.t...|.......d.
+00000610: 0400 7d03 0400 7d05 7d04 7c02 640f 1900  ..}...}.}.|.d...
+00000620: 7d03 6401 7d04 7c03 7c04 6b02 7d05 7c05  }.d.}.|.|.k.}.|.
+00000630: 73ab 7403 a004 6408 7c05 6601 6409 7c03  s.t...d.|.f.d.|.
+00000640: 7c04 6602 a104 7403 a005 7c03 a101 7403  |.f...t...|...t.
+00000650: a005 7c04 a101 640a 9c02 1600 7d06 640b  ..|...d.....}.d.
+00000660: 640c 7c06 6901 1600 7d07 7406 7403 a007  d.|.i...}.t.t...
+00000670: 7c07 a101 8301 8201 6400 0400 7d03 0400  |.......d...}...
+00000680: 7d05 7d04 7c02 6410 1900 6404 1900 7d03  }.}.|.d...d...}.
+00000690: 6405 7d04 7c03 7c04 6b02 7d05 7c05 73e2  d.}.|.|.k.}.|.s.
+000006a0: 7403 a004 6408 7c05 6601 6409 7c03 7c04  t...d.|.f.d.|.|.
+000006b0: 6602 a104 7403 a005 7c03 a101 7403 a005  f...t...|...t...
+000006c0: 7c04 a101 640a 9c02 1600 7d06 640b 640c  |...d.....}.d.d.
+000006d0: 7c06 6901 1600 7d07 7406 7403 a007 7c07  |.i...}.t.t...|.
+000006e0: a101 8301 8201 6400 0400 7d03 0400 7d05  ......d...}...}.
+000006f0: 7d04 6400 5300 2911 4e72 0500 0000 7206  }.d.S.).Nr....r.
+00000700: 0000 0072 0700 0000 7208 0000 00da 036f  ...r....r......o
+00000710: 626a 720b 0000 0072 0c00 0000 720d 0000  bjr....r....r...
+00000720: 0072 0f00 0000 7210 0000 0072 1300 0000  .r....r....r....
+00000730: 7214 0000 0072 1700 0000 da06 4163 6365  r....r......Acce
+00000740: 7074 da05 6163 746f 72da 066f 626a 6563  pt..actor..objec
+00000750: 7429 0872 0300 0000 da06 6163 6365 7074  t).r......accept
+00000760: 721c 0000 0072 1d00 0000 721e 0000 0072  r....r....r....r
+00000770: 1f00 0000 7220 0000 0072 2100 0000 2908  ....r ...r!...).
+00000780: 7222 0000 0072 3000 0000 7223 0000 0072  r"...r0...r#...r
+00000790: 2400 0000 7225 0000 0072 2600 0000 7227  $...r%...r&...r'
+000007a0: 0000 0072 2800 0000 7229 0000 0072 2900  ...r(...r)...r).
+000007b0: 0000 722a 0000 00da 1c74 6573 745f 6163  ..r*.....test_ac
+000007c0: 7469 7669 7479 5f66 6163 746f 7279 5f61  tivity_factory_a
+000007d0: 6363 6570 7417 0000 0073 0e00 0000 0e01  ccept....s......
+000007e0: 0e02 0801 6a02 6a01 6a01 7201 7231 0000  ....j.j.j.r.r1..
+000007f0: 0063 0000 0000 0000 0000 0000 0000 0800  .c..............
+00000800: 0000 0700 0000 4300 0000 7378 0100 0074  ......C...sx...t
+00000810: 0064 0164 0264 039c 0283 017d 0074 0164  .d.d.d.....}.t.d
+00000820: 0464 0164 0564 068d 03a0 02a1 00a0 03a1  .d.d.d..........
+00000830: 007d 017c 00a0 047c 01a1 01a0 03a1 007d  .}.|...|.......}
+00000840: 027c 0264 0719 007d 0364 0567 017d 047c  .|.d...}.d.g.}.|
+00000850: 037c 046b 027d 057c 0573 4974 05a0 0664  .|.k.}.|.sIt...d
+00000860: 087c 0566 0164 097c 037c 0466 02a1 0474  .|.f.d.|.|.f...t
+00000870: 05a0 077c 03a1 0174 05a0 077c 04a1 0164  ...|...t...|...d
+00000880: 0a9c 0216 007d 0664 0b64 0c7c 0669 0116  .....}.d.d.|.i..
+00000890: 007d 0774 0874 05a0 097c 07a1 0183 0182  .}.t.t...|......
+000008a0: 0164 0004 007d 0304 007d 057d 047c 0264  .d...}...}.}.|.d
+000008b0: 0d19 007d 0364 0e67 017d 047c 037c 046b  ...}.d.g.}.|.|.k
+000008c0: 027d 057c 0573 7f74 05a0 0664 087c 0566  .}.|.s.t...d.|.f
+000008d0: 0164 097c 037c 0466 02a1 0474 05a0 077c  .d.|.|.f...t...|
+000008e0: 03a1 0174 05a0 077c 04a1 0164 0a9c 0216  ...t...|...d....
+000008f0: 007d 0664 0b64 0c7c 0669 0116 007d 0774  .}.d.d.|.i...}.t
+00000900: 0874 05a0 097c 07a1 0183 0182 0164 0004  .t...|.......d..
+00000910: 007d 0304 007d 057d 047c 0264 0f19 007d  .}...}.}.|.d...}
+00000920: 0364 017d 047c 037c 046b 027d 057c 0573  .d.}.|.|.k.}.|.s
+00000930: b474 05a0 0664 087c 0566 0164 097c 037c  .t...d.|.f.d.|.|
+00000940: 0466 02a1 0474 05a0 077c 03a1 0174 05a0  .f...t...|...t..
+00000950: 077c 04a1 0164 0a9c 0216 007d 0664 0b64  .|...d.....}.d.d
+00000960: 0c7c 0669 0116 007d 0774 0874 05a0 097c  .|.i...}.t.t...|
+00000970: 07a1 0183 0182 0164 0004 007d 0304 007d  .......d...}...}
+00000980: 057d 0464 0053 0029 104e 7205 0000 0072  .}.d.S.).Nr....r
+00000990: 0600 0000 7207 0000 00da 044e 6f74 65fa  ....r......Note.
+000009a0: 1161 6363 6f75 6e74 2f66 6f6c 6c6f 7765  .account/followe
+000009b0: 7273 2903 7217 0000 00da 0d61 7474 7269  rs).r......attri
+000009c0: 6275 7465 645f 746f 7206 0000 0072 1600  buted_tor....r..
+000009d0: 0000 720d 0000 0072 0f00 0000 7210 0000  ..r....r....r...
+000009e0: 0072 1300 0000 7214 0000 0072 1500 0000  .r....r....r....
+000009f0: 7a2c 6874 7470 733a 2f2f 7777 772e 7733  z,https://www.w3
+00000a00: 2e6f 7267 2f6e 732f 6163 7469 7669 7479  .org/ns/activity
+00000a10: 7374 7265 616d 7323 5075 626c 6963 722e  streams#Publicr.
+00000a20: 0000 0029 0a72 0300 0000 7204 0000 00da  ...).r....r.....
+00000a30: 0961 735f 7075 626c 6963 721c 0000 00da  .as_publicr.....
+00000a40: 0663 7265 6174 6572 1d00 0000 721e 0000  .creater....r...
+00000a50: 0072 1f00 0000 7220 0000 0072 2100 0000  .r....r ...r!...
+00000a60: 2908 7222 0000 00da 046e 6f74 6572 2300  ).r".....noter#.
+00000a70: 0000 7224 0000 0072 2500 0000 7226 0000  ..r$...r%...r&..
+00000a80: 0072 2700 0000 7228 0000 0072 2900 0000  .r'...r(...r)...
+00000a90: 7229 0000 0072 2a00 0000 da1c 7465 7374  r)...r*.....test
+00000aa0: 5f61 6374 6976 6974 795f 6661 6374 6f72  _activity_factor
+00000ab0: 795f 6372 6561 7465 2300 0000 7312 0000  y_create#...s...
+00000ac0: 000e 010c 0204 0104 0102 fd0e 066c 026c  .............l.l
+00000ad0: 016e 0172 3800 0000 6300 0000 0000 0000  .n.r8...c.......
+00000ae0: 0000 0000 000b 0000 0007 0000 0043 0000  .............C..
+00000af0: 0073 8801 0000 7400 6401 6402 6403 9c02  .s....t.d.d.d...
+00000b00: 8301 7d00 6404 7d01 7401 6405 6401 6406  ..}.d.}.t.d.d.d.
+00000b10: 7c01 6801 6407 8d04 a002 a100 7d02 7c00  |.h.d.......}.|.
+00000b20: a003 7c02 a101 a002 a100 7d03 6408 7d04  ..|.......}.d.}.
+00000b30: 7c04 7c03 7601 7d05 7c05 7353 7404 a005  |.|.v.}.|.sSt...
+00000b40: 6409 7c05 6601 640a 7c04 7c03 6602 a104  d.|.f.d.|.|.f...
+00000b50: 7404 a006 7c04 a101 640b 7407 a008 a100  t...|...d.t.....
+00000b60: 7600 733c 7404 a009 7c03 a101 7241 7404  v.s<t...|...rAt.
+00000b70: a006 7c03 a101 6e01 640b 640c 9c02 1600  ..|...n.d.d.....
+00000b80: 7d06 640d 640e 7c06 6901 1600 7d07 740a  }.d.d.|.i...}.t.
+00000b90: 7404 a00b 7c07 a101 8301 8201 6400 0400  t...|.......d...
+00000ba0: 7d04 7d05 7c03 640f 1900 7d04 7c01 6701  }.}.|.d...}.|.g.
+00000bb0: 7d08 7c04 7c08 6b02 7d05 7c05 7387 7404  }.|.|.k.}.|.s.t.
+00000bc0: a005 6410 7c05 6601 6411 7c04 7c08 6602  ..d.|.f.d.|.|.f.
+00000bd0: a104 7404 a006 7c04 a101 7404 a006 7c08  ..t...|...t...|.
+00000be0: a101 6412 9c02 1600 7d09 6413 6414 7c09  ..d.....}.d.d.|.
+00000bf0: 6901 1600 7d0a 740a 7404 a00b 7c0a a101  i...}.t.t...|...
+00000c00: 8301 8201 6400 0400 7d04 0400 7d05 7d08  ....d...}...}.}.
+00000c10: 7c03 6415 1900 7d04 6401 7d08 7c04 7c08  |.d...}.d.}.|.|.
+00000c20: 6b02 7d05 7c05 73bc 7404 a005 6410 7c05  k.}.|.s.t...d.|.
+00000c30: 6601 6411 7c04 7c08 6602 a104 7404 a006  f.d.|.|.f...t...
+00000c40: 7c04 a101 7404 a006 7c08 a101 6412 9c02  |...t...|...d...
+00000c50: 1600 7d09 6413 6414 7c09 6901 1600 7d0a  ..}.d.d.|.i...}.
+00000c60: 740a 7404 a00b 7c0a a101 8301 8201 6400  t.t...|.......d.
+00000c70: 0400 7d04 0400 7d05 7d08 6400 5300 2916  ..}...}.}.d.S.).
+00000c80: 4e72 0500 0000 7206 0000 0072 0700 0000  Nr....r....r....
+00000c90: 7a12 6874 7470 733a 2f2f 6162 656c 2f61  z.https://abel/a
+00000ca0: 6c69 6365 7232 0000 0072 3300 0000 2904  licer2...r3...).
+00000cb0: 7217 0000 0072 3400 0000 7206 0000 0072  r....r4...r....r
+00000cc0: 1500 0000 7216 0000 0029 01fa 066e 6f74  ....r....)...not
+00000cd0: 2069 6e29 017a 1625 2870 7931 2973 206e   in).z.%(py1)s n
+00000ce0: 6f74 2069 6e20 2528 7079 3329 7372 2300  ot in %(py3)sr#.
+00000cf0: 0000 2902 7211 0000 00da 0370 7933 7a0e  ..).r......py3z.
+00000d00: 6173 7365 7274 2025 2870 7935 2973 da03  assert %(py5)s..
+00000d10: 7079 3572 1500 0000 720d 0000 0072 0f00  py5r....r....r..
+00000d20: 0000 7210 0000 0072 1300 0000 7214 0000  ..r....r....r...
+00000d30: 0072 2e00 0000 290c 7203 0000 0072 0400  .r....).r....r..
+00000d40: 0000 721c 0000 0072 3600 0000 721d 0000  ..r....r6...r...
+00000d50: 0072 1e00 0000 721f 0000 00da 0c40 7079  .r....r......@py
+00000d60: 5f62 7569 6c74 696e 73da 066c 6f63 616c  _builtins..local
+00000d70: 73da 185f 7368 6f75 6c64 5f72 6570 725f  s.._should_repr_
+00000d80: 676c 6f62 616c 5f6e 616d 6572 2000 0000  global_namer ...
+00000d90: 7221 0000 0029 0b72 2200 0000 da0c 7265  r!...).r".....re
+00000da0: 6d6f 7465 5f61 6374 6f72 7237 0000 0072  mote_actorr7...r
+00000db0: 2300 0000 7224 0000 0072 2600 0000 da0b  #...r$...r&.....
+00000dc0: 4070 795f 666f 726d 6174 34da 0b40 7079  @py_format4..@py
+00000dd0: 5f66 6f72 6d61 7436 7225 0000 0072 2700  _format6r%...r'.
+00000de0: 0000 7228 0000 0072 2900 0000 7229 0000  ..r(...r)...r)..
+00000df0: 0072 2a00 0000 da22 7465 7374 5f61 6374  .r*...."test_act
+00000e00: 6976 6974 795f 6661 6374 6f72 795f 6372  ivity_factory_cr
+00000e10: 6561 7465 5f6e 6f5f 6363 3200 0000 731c  eate_no_cc2...s.
+00000e20: 0000 000e 0104 0102 0102 0102 0102 0104  ................
+00000e30: 0104 fc04 0502 fb0e 0778 026c 016e 0172  .........x.l.n.r
+00000e40: 4200 0000 6300 0000 0000 0000 0000 0000  B...c...........
+00000e50: 0009 0000 0009 0000 0043 0000 0073 f600  .........C...s..
+00000e60: 0000 7400 6401 6402 6403 9c02 8301 7d00  ..t.d.d.d.....}.
+00000e70: 7c00 a001 6404 a101 a002 a100 7d01 7c01  |...d.......}.|.
+00000e80: 6a03 7d02 7c02 8300 7d03 7404 7c03 8301  j.}.|...}.t.|...
+00000e90: 7d04 6800 6405 a301 7d05 7c04 7c05 6b02  }.h.d...}.|.|.k.
+00000ea0: 7d06 7c06 736f 7405 a006 6406 7c06 6601  }.|.sot...d.|.f.
+00000eb0: 6407 7c04 7c05 6602 a104 6408 7407 a008  d.|.|.f...d.t...
+00000ec0: a100 7600 7337 7405 a009 7404 a101 723c  ..v.s7t...t...r<
+00000ed0: 7405 a00a 7404 a101 6e01 6408 6409 7407  t...t...n.d.d.t.
+00000ee0: a008 a100 7600 7348 7405 a009 7c01 a101  ....v.sHt...|...
+00000ef0: 724d 7405 a00a 7c01 a101 6e01 6409 7405  rMt...|...n.d.t.
+00000f00: a00a 7c02 a101 7405 a00a 7c03 a101 7405  ..|...t...|...t.
+00000f10: a00a 7c04 a101 7405 a00a 7c05 a101 640a  ..|...t...|...d.
+00000f20: 9c06 1600 7d07 640b 640c 7c07 6901 1600  ....}.d.d.|.i...
+00000f30: 7d08 740b 7405 a00c 7c08 a101 8301 8201  }.t.t...|.......
+00000f40: 6400 0400 7d02 0400 7d03 0400 7d04 0400  d...}...}...}...
+00000f50: 7d06 7d05 6400 5300 290d 4e72 0500 0000  }.}.d.S.).Nr....
+00000f60: 7206 0000 0072 0700 0000 7209 0000 003e  r....r....r....>
+00000f70: 0400 0000 722f 0000 0072 0b00 0000 722e  ....r/...r....r.
+00000f80: 0000 0072 1700 0000 720d 0000 0029 017a  ...r....r....).z
+00000f90: 6225 2870 7937 2973 0a7b 2528 7079 3729  b%(py7)s.{%(py7)
+00000fa0: 7320 3d20 2528 7079 3029 7328 2528 7079  s = %(py0)s(%(py
+00000fb0: 3529 730a 7b25 2870 7935 2973 203d 2025  5)s.{%(py5)s = %
+00000fc0: 2870 7933 2973 0a7b 2528 7079 3329 7320  (py3)s.{%(py3)s 
+00000fd0: 3d20 2528 7079 3129 732e 6b65 7973 0a7d  = %(py1)s.keys.}
+00000fe0: 2829 0a7d 290a 7d20 3d3d 2025 2870 7931  ().}).} == %(py1
+00000ff0: 3029 73da 0373 6574 7223 0000 0029 06da  0)s..setr#...)..
+00001000: 0370 7930 7211 0000 0072 3a00 0000 723b  .py0r....r:...r;
+00001010: 0000 00da 0370 7937 5a04 7079 3130 7a0f  .....py7Z.py10z.
+00001020: 6173 7365 7274 2025 2870 7931 3229 735a  assert %(py12)sZ
+00001030: 0470 7931 3229 0d72 0300 0000 da06 6465  .py12).r......de
+00001040: 6c65 7465 721c 0000 00da 046b 6579 7372  leter......keysr
+00001050: 4300 0000 721d 0000 0072 1e00 0000 723c  C...r....r....r<
+00001060: 0000 0072 3d00 0000 723e 0000 0072 1f00  ...r=...r>...r..
+00001070: 0000 7220 0000 0072 2100 0000 2909 7222  ..r ...r!...).r"
+00001080: 0000 0072 2300 0000 7226 0000 00da 0b40  ...r#...r&.....@
+00001090: 7079 5f61 7373 6572 7434 5a0b 4070 795f  py_assert4Z.@py_
+000010a0: 6173 7365 7274 365a 0b40 7079 5f61 7373  assert6Z.@py_ass
+000010b0: 6572 7439 5a0b 4070 795f 6173 7365 7274  ert9Z.@py_assert
+000010c0: 385a 0c40 7079 5f66 6f72 6d61 7431 315a  8Z.@py_format11Z
+000010d0: 0c40 7079 5f66 6f72 6d61 7431 3372 2900  .@py_format13r).
+000010e0: 0000 7229 0000 0072 2a00 0000 da1c 7465  ..r)...r*.....te
+000010f0: 7374 5f61 6374 6976 6974 795f 6e6f 5f65  st_activity_no_e
+00001100: 6d70 7479 5f74 6f5f 6363 4300 0000 7306  mpty_to_ccC...s.
+00001110: 0000 000e 010e 02da 0272 4900 0000 290f  .........rI...).
+00001120: da08 6275 696c 7469 6e73 723c 0000 00da  ..builtinsr<....
+00001130: 195f 7079 7465 7374 2e61 7373 6572 7469  ._pytest.asserti
+00001140: 6f6e 2e72 6577 7269 7465 da09 6173 7365  on.rewrite..asse
+00001150: 7274 696f 6eda 0772 6577 7269 7465 721d  rtion..rewriter.
+00001160: 0000 0072 2200 0000 7203 0000 00da 0e6f  ...r"...r......o
+00001170: 626a 6563 745f 6661 6374 6f72 7972 0400  bject_factoryr..
+00001180: 0000 722b 0000 0072 3100 0000 7238 0000  ..r+...r1...r8..
+00001190: 0072 4200 0000 7249 0000 0072 2900 0000  .rB...rI...r)...
+000011a0: 7229 0000 0072 2900 0000 722a 0000 00da  r)...r)...r*....
+000011b0: 083c 6d6f 6475 6c65 3e01 0000 0073 0e00  .<module>....s..
+000011c0: 0000 2600 0c01 0803 0812 080c 080f 0c11  ..&.............
```

### Comparing `bovine-0.1.0/bovine/activitystreams/__pycache__/test_actor.cpython-310-pytest-7.3.0.pyc` & `bovine-0.1.1/bovine/activitystreams/__pycache__/test_actor.cpython-310-pytest-7.3.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 13 15:55:57 2023 UTC, .py size: 1418 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0d26 3864 8a05 0000  o........&8d....
+00000000: 6f0d 0d0a 0000 0000 a4ea 3a64 8a05 0000  o.........:d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 4e00 0000 6400  .....@...sN...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6402 6c06 6d07  ..m.Z...d.d.l.m.
 00000050: 5a07 0100 6403 6404 6c08 6d09 5a09 0100  Z...d.d.l.m.Z...
 00000060: 6405 6406 8400 5a0a 6407 6408 8400 5a0b  d.d...Z.d.d...Z.
 00000070: 6409 640a 8400 5a0c 6401 5300 290b e900  d.d...Z.d.S.)...
@@ -60,36 +60,36 @@
 000003b0: 7c02 6601 6413 7c09 7c0a 6602 a104 7404  |.f.d.|.|.f...t.
 000003c0: a009 7c09 a101 7404 a009 7c0a a101 6414  ..|...t...|...d.
 000003d0: 9c02 1600 7d0b 6415 6416 7c0b 6901 1600  ....}.d.d.|.i...
 000003e0: 7d0c 740a 7404 a00b 7c0c a101 8301 8201  }.t.t...|.......
 000003f0: 6400 0400 7d09 0400 7d02 7d0a 6400 5300  d...}...}.}.d.S.
 00000400: 2917 4efa 1c68 7474 703a 2f2f 6578 616d  ).N..http://exam
 00000410: 706c 652e 636f 6d2f 6163 746f 722f 3132  ple.com/actor/12
-00000420: 3329 01da 0269 643e 0500 0000 7206 0000  3)...id>....r...
-00000430: 00fa 0840 636f 6e74 6578 74da 0474 7970  ...@context..typ
-00000440: 65da 066f 7574 626f 78da 0569 6e62 6f78  e..outbox..inbox
+00000420: 3329 01da 0269 643e 0500 0000 da05 696e  3)...id>......in
+00000430: 626f 78fa 0840 636f 6e74 6578 7472 0600  box..@contextr..
+00000440: 0000 da04 7479 7065 da06 6f75 7462 6f78  ....type..outbox
 00000450: a901 fa02 3d3d 2901 7a62 2528 7079 3729  ....==).zb%(py7)
 00000460: 730a 7b25 2870 7937 2973 203d 2025 2870  s.{%(py7)s = %(p
 00000470: 7930 2973 2825 2870 7935 2973 0a7b 2528  y0)s(%(py5)s.{%(
 00000480: 7079 3529 7320 3d20 2528 7079 3329 730a  py5)s = %(py3)s.
 00000490: 7b25 2870 7933 2973 203d 2025 2870 7931  {%(py3)s = %(py1
 000004a0: 2973 2e6b 6579 730a 7d28 290a 7d29 0a7d  )s.keys.}().}).}
 000004b0: 203d 3d20 2528 7079 3130 2973 da03 7365   == %(py10)s..se
 000004c0: 74da 0672 6573 756c 7429 06da 0370 7930  t..result)...py0
 000004d0: da03 7079 31da 0370 7933 da03 7079 35da  ..py1..py3..py5.
 000004e0: 0370 7937 da04 7079 3130 7a0f 6173 7365  .py7..py10z.asse
 000004f0: 7274 2025 2870 7931 3229 73da 0470 7931  rt %(py12)s..py1
 00000500: 327a 084a 6f68 6e20 446f 653e 0600 0000  2z.John Doe>....
-00000510: 7206 0000 0072 0700 0000 7208 0000 0072  r....r....r....r
+00000510: 7207 0000 0072 0800 0000 7206 0000 0072  r....r....r....r
 00000520: 0900 0000 720a 0000 00da 046e 616d 655a  ....r......nameZ
 00000530: 1130 3132 3334 3536 3738 3930 3132 3334  .012345678901234
-00000540: 3536 da03 6b65 793e 0700 0000 7206 0000  56..key>....r...
-00000550: 0072 0700 0000 7208 0000 0072 0900 0000  .r....r....r....
-00000560: 720a 0000 0072 1600 0000 da09 7075 626c  r....r......publ
-00000570: 6963 4b65 7972 1800 0000 7a04 236b 6579  icKeyr....z.#key
+00000540: 3536 da03 6b65 793e 0700 0000 7207 0000  56..key>....r...
+00000550: 0072 0800 0000 da09 7075 626c 6963 4b65  .r......publicKe
+00000560: 7972 0600 0000 7209 0000 0072 0a00 0000  yr....r....r....
+00000570: 7216 0000 0072 1800 0000 7a04 236b 6579  r....r....z.#key
 00000580: 2903 7206 0000 00da 056f 776e 6572 da0c  ).r......owner..
 00000590: 7075 626c 6963 4b65 7950 656d a901 7a12  publicKeyPem..z.
 000005a0: 2528 7079 3129 7320 3d3d 2025 2870 7934  %(py1)s == %(py4
 000005b0: 2973 a902 7210 0000 00da 0370 7934 fa0e  )s..r......py4..
 000005c0: 6173 7365 7274 2025 2870 7936 2973 da03  assert %(py6)s..
 000005d0: 7079 3629 1072 0400 0000 da05 6275 696c  py6).r......buil
 000005e0: 64da 046b 6579 7372 0d00 0000 da0a 4070  d..keysr......@p
@@ -109,99 +109,99 @@
 000006c0: 6173 7365 7274 36da 0b40 7079 5f61 7373  assert6..@py_ass
 000006d0: 6572 7439 da0b 4070 795f 6173 7365 7274  ert9..@py_assert
 000006e0: 38da 0c40 7079 5f66 6f72 6d61 7431 31da  8..@py_format11.
 000006f0: 0c40 7079 5f66 6f72 6d61 7431 33da 0b40  .@py_format13..@
 00000700: 7079 5f61 7373 6572 7430 da0b 4070 795f  py_assert0..@py_
 00000710: 6173 7365 7274 33da 0b40 7079 5f66 6f72  assert3..@py_for
 00000720: 6d61 7435 da0b 4070 795f 666f 726d 6174  mat5..@py_format
-00000730: 37a9 0072 3800 0000 fa55 2f77 6f6f 6470  7..r8....U/woodp
+00000730: 37a9 0072 3800 0000 fa56 2f77 6f6f 6470  7..r8....V/woodp
 00000740: 6563 6b65 722f 7372 632f 636f 6465 6265  ecker/src/codebe
-00000750: 7267 2e6f 7267 2f68 656c 6765 2f62 6f76  rg.org/helge/bov
-00000760: 696e 652f 626f 7669 6e65 2f62 6f76 696e  ine/bovine/bovin
-00000770: 652f 6163 7469 7669 7479 7374 7265 616d  e/activitystream
-00000780: 732f 7465 7374 5f61 6374 6f72 2e70 79da  s/test_actor.py.
-00000790: 0a74 6573 745f 6163 746f 7206 0000 0073  .test_actor....s
-000007a0: 9e00 0000 0a01 0802 d602 0602 0801 d601  ................
-000007b0: 0602 0601 0801 0202 0208 28f8 0208 0ef8  ..........(.....
-000007c0: 0208 04f8 0408 08f8 0208 02f8 0208 06f8  ................
-000007d0: 0208 02f8 0408 06f8 0408 08f8 0208 02f8  ................
-000007e0: 0208 06f8 0208 02f8 0408 04f8 0208 02f8  ................
-000007f0: 0208 02f8 0208 02f8 0208 02f8 0208 02f8  ................
-00000800: 0208 02f8 0208 02f8 0208 18f8 0208 02f8  ................
-00000810: 0208 18f8 0a0a 0204 06fc 0204 02fc 0204  ................
-00000820: 16fc 0204 0efc 0204 02fc 0204 02fc 0204  ................
-00000830: 02fc 0204 02fc 0204 18fc 0204 02fc 0204  ................
-00000840: 14fc 723a 0000 0063 0000 0000 0000 0000  ..r:...c........
-00000850: 0000 0000 0700 0000 0700 0000 4300 0000  ............C...
-00000860: 7370 0100 0074 0064 0164 0264 0364 048d  sp...t.d.d.d.d..
-00000870: 037d 007c 00a0 01a1 007d 017c 0164 0219  .}.|.....}.|.d..
-00000880: 007d 0264 027d 037c 027c 036b 027d 047c  .}.d.}.|.|.k.}.|
-00000890: 0473 3a74 02a0 0364 057c 0466 0164 067c  .s:t...d.|.f.d.|
-000008a0: 027c 0366 02a1 0474 02a0 047c 02a1 0174  .|.f...t...|...t
-000008b0: 02a0 047c 03a1 0164 079c 0216 007d 0564  ...|...d.....}.d
-000008c0: 0864 097c 0569 0116 007d 0674 0574 02a0  .d.|.i...}.t.t..
-000008d0: 067c 06a1 0183 0182 0164 0004 007d 0204  .|.......d...}..
-000008e0: 007d 047d 037c 0164 0319 007d 0264 037d  .}.}.|.d...}.d.}
-000008f0: 037c 027c 036b 027d 047c 0473 6f74 02a0  .|.|.k.}.|.sot..
-00000900: 0364 057c 0466 0164 067c 027c 0366 02a1  .d.|.f.d.|.|.f..
-00000910: 0474 02a0 047c 02a1 0174 02a0 047c 03a1  .t...|...t...|..
-00000920: 0164 079c 0216 007d 0564 0864 097c 0569  .d.....}.d.d.|.i
-00000930: 0116 007d 0674 0574 02a0 067c 06a1 0183  ...}.t.t...|....
-00000940: 0182 0164 0004 007d 0204 007d 047d 0364  ...d...}...}.}.d
-00000950: 0a7c 005f 077c 006a 0174 086a 0964 0b8d  .|._.|.j.t.j.d..
-00000960: 017d 017c 0164 0c19 0064 0d19 007d 0264  .}.|.d...d...}.d
-00000970: 0a7d 037c 027c 036b 027d 047c 0473 b074  .}.|.|.k.}.|.s.t
-00000980: 02a0 0364 057c 0466 0164 067c 027c 0366  ...d.|.f.d.|.|.f
-00000990: 02a1 0474 02a0 047c 02a1 0174 02a0 047c  ...t...|...t...|
-000009a0: 03a1 0164 079c 0216 007d 0564 0864 097c  ...d.....}.d.d.|
-000009b0: 0569 0116 007d 0674 0574 02a0 067c 06a1  .i...}.t.t...|..
-000009c0: 0183 0182 0164 0004 007d 0204 007d 047d  .....d...}...}.}
-000009d0: 0364 0053 0029 0e4e 7205 0000 0072 0a00  .d.S.).Nr....r..
-000009e0: 0000 7209 0000 00a9 0372 0600 0000 720a  ..r......r....r.
-000009f0: 0000 0072 0900 0000 720b 0000 0072 1b00  ...r....r....r..
-00000a00: 0000 721c 0000 0072 1e00 0000 721f 0000  ..r....r....r...
-00000a10: 007a 1868 7474 703a 2f2f 6578 616d 706c  .z.http://exampl
-00000a20: 652e 636f 6d2f 7072 6f78 7929 01da 0a76  e.com/proxy)...v
-00000a30: 6973 6962 696c 6974 79da 0965 6e64 706f  isibility..endpo
-00000a40: 696e 7473 da08 7072 6f78 7955 726c 290a  ints..proxyUrl).
-00000a50: 7204 0000 0072 2000 0000 7222 0000 0072  r....r ...r"...r
-00000a60: 2300 0000 7227 0000 0072 2800 0000 7229  #...r'...r(...r)
-00000a70: 0000 00da 0970 726f 7879 5f75 726c 7202  .....proxy_urlr.
-00000a80: 0000 00da 054f 574e 4552 a907 722c 0000  .....OWNER..r,..
-00000a90: 0072 0e00 0000 7234 0000 0072 3500 0000  .r....r4...r5...
-00000aa0: 722d 0000 0072 3600 0000 7237 0000 0072  r-...r6...r7...r
-00000ab0: 3800 0000 7238 0000 0072 3900 0000 da11  8...r8...r9.....
-00000ac0: 7465 7374 5f61 6374 6f72 5f73 6563 6f6e  test_actor_secon
-00000ad0: 6426 0000 0073 0e00 0000 0e01 0802 6a02  d&...s........j.
-00000ae0: 6a01 0602 0e01 7202 7242 0000 0063 0000  j.....r.rB...c..
-00000af0: 0000 0000 0000 0000 0000 0700 0000 0700  ................
-00000b00: 0000 4300 0000 7392 0000 0074 0064 0164  ..C...s....t.d.d
-00000b10: 0264 0364 048d 037d 0064 0564 0669 017c  .d.d...}.d.d.i.|
-00000b20: 005f 017c 00a0 02a1 007d 017c 0164 0719  ._.|.....}.|.d..
-00000b30: 007d 0264 0564 0669 017d 037c 027c 036b  .}.d.d.i.}.|.|.k
-00000b40: 027d 047c 0473 4174 03a0 0464 087c 0466  .}.|.sAt...d.|.f
-00000b50: 0164 097c 027c 0366 02a1 0474 03a0 057c  .d.|.|.f...t...|
-00000b60: 02a1 0174 03a0 057c 03a1 0164 0a9c 0216  ...t...|...d....
-00000b70: 007d 0564 0b64 0c7c 0569 0116 007d 0674  .}.d.d.|.i...}.t
-00000b80: 0674 03a0 077c 06a1 0183 0182 0164 0004  .t...|.......d..
-00000b90: 007d 0204 007d 047d 0364 0053 0029 0d4e  .}...}.}.d.S.).N
-00000ba0: 7205 0000 0072 0a00 0000 7209 0000 0072  r....r....r....r
-00000bb0: 3b00 0000 7208 0000 005a 0549 6d61 6765  ;...r....Z.Image
-00000bc0: da04 6963 6f6e 720b 0000 0072 1b00 0000  ..iconr....r....
-00000bd0: 721c 0000 0072 1e00 0000 721f 0000 0029  r....r....r....)
-00000be0: 0872 0400 0000 7243 0000 0072 2000 0000  .r....rC...r ...
-00000bf0: 7222 0000 0072 2300 0000 7227 0000 0072  r"...r#...r'...r
-00000c00: 2800 0000 7229 0000 0072 4100 0000 7238  (...r)...rA...r8
-00000c10: 0000 0072 3800 0000 7239 0000 00da 1474  ...r8...r9.....t
-00000c20: 6573 745f 6163 746f 725f 7769 7468 5f69  est_actor_with_i
-00000c30: 636f 6e34 0000 0073 0800 0000 0e01 0a01  con4...s........
-00000c40: 0802 7202 7244 0000 0029 0dda 0862 7569  ..r.rD...)...bui
-00000c50: 6c74 696e 7372 2400 0000 da19 5f70 7974  ltinsr$....._pyt
-00000c60: 6573 742e 6173 7365 7274 696f 6e2e 7265  est.assertion.re
-00000c70: 7772 6974 65da 0961 7373 6572 7469 6f6e  write..assertion
-00000c80: da07 7265 7772 6974 6572 2200 0000 da0c  ..rewriter".....
-00000c90: 626f 7669 6e65 2e74 7970 6573 7202 0000  bovine.typesr...
-00000ca0: 00da 0072 0400 0000 723a 0000 0072 4200  ...r....r:...rB.
-00000cb0: 0000 7244 0000 0072 3800 0000 7238 0000  ..rD...r8...r8..
-00000cc0: 0072 3800 0000 7239 0000 00da 083c 6d6f  .r8...r9.....<mo
-00000cd0: 6475 6c65 3e01 0000 0073 0a00 0000 2600  dule>....s....&.
-00000ce0: 0c02 0803 0820 0c0e                      ..... ..
+00000750: 7267 2e6f 7267 2f62 6f76 696e 652f 626f  rg.org/bovine/bo
+00000760: 7669 6e65 2f62 6f76 696e 652f 626f 7669  vine/bovine/bovi
+00000770: 6e65 2f61 6374 6976 6974 7973 7472 6561  ne/activitystrea
+00000780: 6d73 2f74 6573 745f 6163 746f 722e 7079  ms/test_actor.py
+00000790: da0a 7465 7374 5f61 6374 6f72 0600 0000  ..test_actor....
+000007a0: 739e 0000 000a 0108 02d6 0206 0208 01d6  s...............
+000007b0: 0106 0206 0108 0102 0202 0828 f802 080e  ...........(....
+000007c0: f802 0804 f804 0808 f802 0802 f802 0806  ................
+000007d0: f802 0802 f804 0806 f804 0808 f802 0802  ................
+000007e0: f802 0806 f802 0802 f804 0804 f802 0802  ................
+000007f0: f802 0802 f802 0802 f802 0802 f802 0802  ................
+00000800: f802 0802 f802 0802 f802 0818 f802 0802  ................
+00000810: f802 0818 f80a 0a02 0406 fc02 0402 fc02  ................
+00000820: 0416 fc02 040e fc02 0402 fc02 0402 fc02  ................
+00000830: 0402 fc02 0402 fc02 0418 fc02 0402 fc02  ................
+00000840: 0414 fc72 3a00 0000 6300 0000 0000 0000  ...r:...c.......
+00000850: 0000 0000 0007 0000 0007 0000 0043 0000  .............C..
+00000860: 0073 7001 0000 7400 6401 6402 6403 6404  .sp...t.d.d.d.d.
+00000870: 8d03 7d00 7c00 a001 a100 7d01 7c01 6402  ..}.|.....}.|.d.
+00000880: 1900 7d02 6402 7d03 7c02 7c03 6b02 7d04  ..}.d.}.|.|.k.}.
+00000890: 7c04 733a 7402 a003 6405 7c04 6601 6406  |.s:t...d.|.f.d.
+000008a0: 7c02 7c03 6602 a104 7402 a004 7c02 a101  |.|.f...t...|...
+000008b0: 7402 a004 7c03 a101 6407 9c02 1600 7d05  t...|...d.....}.
+000008c0: 6408 6409 7c05 6901 1600 7d06 7405 7402  d.d.|.i...}.t.t.
+000008d0: a006 7c06 a101 8301 8201 6400 0400 7d02  ..|.......d...}.
+000008e0: 0400 7d04 7d03 7c01 6403 1900 7d02 6403  ..}.}.|.d...}.d.
+000008f0: 7d03 7c02 7c03 6b02 7d04 7c04 736f 7402  }.|.|.k.}.|.sot.
+00000900: a003 6405 7c04 6601 6406 7c02 7c03 6602  ..d.|.f.d.|.|.f.
+00000910: a104 7402 a004 7c02 a101 7402 a004 7c03  ..t...|...t...|.
+00000920: a101 6407 9c02 1600 7d05 6408 6409 7c05  ..d.....}.d.d.|.
+00000930: 6901 1600 7d06 7405 7402 a006 7c06 a101  i...}.t.t...|...
+00000940: 8301 8201 6400 0400 7d02 0400 7d04 7d03  ....d...}...}.}.
+00000950: 640a 7c00 5f07 7c00 6a01 7408 6a09 640b  d.|._.|.j.t.j.d.
+00000960: 8d01 7d01 7c01 640c 1900 640d 1900 7d02  ..}.|.d...d...}.
+00000970: 640a 7d03 7c02 7c03 6b02 7d04 7c04 73b0  d.}.|.|.k.}.|.s.
+00000980: 7402 a003 6405 7c04 6601 6406 7c02 7c03  t...d.|.f.d.|.|.
+00000990: 6602 a104 7402 a004 7c02 a101 7402 a004  f...t...|...t...
+000009a0: 7c03 a101 6407 9c02 1600 7d05 6408 6409  |...d.....}.d.d.
+000009b0: 7c05 6901 1600 7d06 7405 7402 a006 7c06  |.i...}.t.t...|.
+000009c0: a101 8301 8201 6400 0400 7d02 0400 7d04  ......d...}...}.
+000009d0: 7d03 6400 5300 290e 4e72 0500 0000 7207  }.d.S.).Nr....r.
+000009e0: 0000 0072 0a00 0000 a903 7206 0000 0072  ...r......r....r
+000009f0: 0700 0000 720a 0000 0072 0b00 0000 721b  ....r....r....r.
+00000a00: 0000 0072 1c00 0000 721e 0000 0072 1f00  ...r....r....r..
+00000a10: 0000 7a18 6874 7470 3a2f 2f65 7861 6d70  ..z.http://examp
+00000a20: 6c65 2e63 6f6d 2f70 726f 7879 2901 da0a  le.com/proxy)...
+00000a30: 7669 7369 6269 6c69 7479 da09 656e 6470  visibility..endp
+00000a40: 6f69 6e74 73da 0870 726f 7879 5572 6c29  oints..proxyUrl)
+00000a50: 0a72 0400 0000 7220 0000 0072 2200 0000  .r....r ...r"...
+00000a60: 7223 0000 0072 2700 0000 7228 0000 0072  r#...r'...r(...r
+00000a70: 2900 0000 da09 7072 6f78 795f 7572 6c72  ).....proxy_urlr
+00000a80: 0200 0000 da05 4f57 4e45 52a9 0772 2c00  ......OWNER..r,.
+00000a90: 0000 720e 0000 0072 3400 0000 7235 0000  ..r....r4...r5..
+00000aa0: 0072 2d00 0000 7236 0000 0072 3700 0000  .r-...r6...r7...
+00000ab0: 7238 0000 0072 3800 0000 7239 0000 00da  r8...r8...r9....
+00000ac0: 1174 6573 745f 6163 746f 725f 7365 636f  .test_actor_seco
+00000ad0: 6e64 2600 0000 730e 0000 000e 0108 026a  nd&...s........j
+00000ae0: 026a 0106 020e 0172 0272 4200 0000 6300  .j.....r.rB...c.
+00000af0: 0000 0000 0000 0000 0000 0007 0000 0007  ................
+00000b00: 0000 0043 0000 0073 9200 0000 7400 6401  ...C...s....t.d.
+00000b10: 6402 6403 6404 8d03 7d00 6405 6406 6901  d.d.d...}.d.d.i.
+00000b20: 7c00 5f01 7c00 a002 a100 7d01 7c01 6407  |._.|.....}.|.d.
+00000b30: 1900 7d02 6405 6406 6901 7d03 7c02 7c03  ..}.d.d.i.}.|.|.
+00000b40: 6b02 7d04 7c04 7341 7403 a004 6408 7c04  k.}.|.sAt...d.|.
+00000b50: 6601 6409 7c02 7c03 6602 a104 7403 a005  f.d.|.|.f...t...
+00000b60: 7c02 a101 7403 a005 7c03 a101 640a 9c02  |...t...|...d...
+00000b70: 1600 7d05 640b 640c 7c05 6901 1600 7d06  ..}.d.d.|.i...}.
+00000b80: 7406 7403 a007 7c06 a101 8301 8201 6400  t.t...|.......d.
+00000b90: 0400 7d02 0400 7d04 7d03 6400 5300 290d  ..}...}.}.d.S.).
+00000ba0: 4e72 0500 0000 7207 0000 0072 0a00 0000  Nr....r....r....
+00000bb0: 723b 0000 0072 0900 0000 5a05 496d 6167  r;...r....Z.Imag
+00000bc0: 65da 0469 636f 6e72 0b00 0000 721b 0000  e..iconr....r...
+00000bd0: 0072 1c00 0000 721e 0000 0072 1f00 0000  .r....r....r....
+00000be0: 2908 7204 0000 0072 4300 0000 7220 0000  ).r....rC...r ..
+00000bf0: 0072 2200 0000 7223 0000 0072 2700 0000  .r"...r#...r'...
+00000c00: 7228 0000 0072 2900 0000 7241 0000 0072  r(...r)...rA...r
+00000c10: 3800 0000 7238 0000 0072 3900 0000 da14  8...r8...r9.....
+00000c20: 7465 7374 5f61 6374 6f72 5f77 6974 685f  test_actor_with_
+00000c30: 6963 6f6e 3400 0000 7308 0000 000e 010a  icon4...s.......
+00000c40: 0108 0272 0272 4400 0000 290d da08 6275  ...r.rD...)...bu
+00000c50: 696c 7469 6e73 7224 0000 00da 195f 7079  iltinsr$....._py
+00000c60: 7465 7374 2e61 7373 6572 7469 6f6e 2e72  test.assertion.r
+00000c70: 6577 7269 7465 da09 6173 7365 7274 696f  ewrite..assertio
+00000c80: 6eda 0772 6577 7269 7465 7222 0000 00da  n..rewriter"....
+00000c90: 0c62 6f76 696e 652e 7479 7065 7372 0200  .bovine.typesr..
+00000ca0: 0000 da00 7204 0000 0072 3a00 0000 7242  ....r....r:...rB
+00000cb0: 0000 0072 4400 0000 7238 0000 0072 3800  ...rD...r8...r8.
+00000cc0: 0000 7238 0000 0072 3900 0000 da08 3c6d  ..r8...r9.....<m
+00000cd0: 6f64 756c 653e 0100 0000 730a 0000 0026  odule>....s....&
+00000ce0: 000c 0208 0308 200c 0e                   ...... ..
```

### Comparing `bovine-0.1.0/bovine/activitystreams/__pycache__/test_object_factory.cpython-310-pytest-7.3.0.pyc` & `bovine-0.1.1/bovine/activitystreams/__pycache__/test_object_factory.cpython-310-pytest-7.3.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 13 15:55:57 2023 UTC, .py size: 1381 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0d26 3864 6505 0000  o........&8de...
+00000000: 6f0d 0d0a 0000 0000 a4ea 3a64 6505 0000  o.........:de...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 4e00 0000 6400  .....@...sN...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6401 6c06 5a06  ..m.Z...d.d.l.Z.
 00000050: 6400 6402 6c07 6d08 5a08 0100 6403 6404  d.d.l.m.Z...d.d.
 00000060: 6c09 6d0a 5a0a 0100 6405 6406 8400 5a0b  l.m.Z...d.d...Z.
 00000070: 6407 6408 8400 5a0c 6401 5300 2909 e900  d.d...Z.d.S.)...
@@ -38,38 +38,38 @@
 00000250: 0366 0164 0f7c 0a7c 0b66 02a1 0474 07a0  .f.d.|.|.f...t..
 00000260: 0c7c 0aa1 0174 07a0 0c7c 0ba1 0164 109c  .|...t...|...d..
 00000270: 0216 007d 0c64 1164 127c 0c69 0116 007d  ...}.d.d.|.i...}
 00000280: 0d74 0d74 07a0 0e7c 0da1 0183 0182 0164  .t.t...|.......d
 00000290: 0004 007d 0a04 007d 037d 0b64 0053 0029  ...}...}.}.d.S.)
 000002a0: 144e da08 6163 746f 725f 6964 da09 666f  .N..actor_id..fo
 000002b0: 6c6c 6f77 6572 7329 02da 0269 6472 0600  llowers)...idr..
-000002c0: 0000 da04 7465 7874 3e06 0000 00da 0274  ....text>......t
-000002d0: 6fda 0263 63da 0763 6f6e 7465 6e74 fa08  o..cc..content..
-000002e0: 4063 6f6e 7465 7874 da04 7479 7065 da0c  @context..type..
-000002f0: 6174 7472 6962 7574 6564 546f a901 fa02  attributedTo....
+000002c0: 0000 da04 7465 7874 3e06 0000 00da 0763  ....text>......c
+000002d0: 6f6e 7465 6e74 da02 6363 fa08 4063 6f6e  ontent..cc..@con
+000002e0: 7465 7874 da04 7479 7065 da0c 6174 7472  text..type..attr
+000002f0: 6962 7574 6564 546f da02 746f a901 fa02  ibutedTo..to....
 00000300: 3d3d a901 7a62 2528 7079 3729 730a 7b25  ==..zb%(py7)s.{%
 00000310: 2870 7937 2973 203d 2025 2870 7930 2973  (py7)s = %(py0)s
 00000320: 2825 2870 7935 2973 0a7b 2528 7079 3529  (%(py5)s.{%(py5)
 00000330: 7320 3d20 2528 7079 3329 730a 7b25 2870  s = %(py3)s.{%(p
 00000340: 7933 2973 203d 2025 2870 7931 2973 2e6b  y3)s = %(py1)s.k
 00000350: 6579 730a 7d28 290a 7d29 0a7d 203d 3d20  eys.}().}).} == 
 00000360: 2528 7079 3130 2973 da03 7365 74da 0672  %(py10)s..set..r
 00000370: 6573 756c 74a9 06da 0370 7930 da03 7079  esult....py0..py
 00000380: 31da 0370 7933 da03 7079 35da 0370 7937  1..py3..py5..py7
 00000390: da04 7079 3130 fa0f 6173 7365 7274 2025  ..py10..assert %
-000003a0: 2870 7931 3229 73da 0470 7931 3272 0900  (py12)s..py12r..
+000003a0: 2870 7931 3229 73da 0470 7931 3272 0e00  (py12)s..py12r..
 000003b0: 0000 7a2c 6874 7470 733a 2f2f 7777 772e  ..z,https://www.
 000003c0: 7733 2e6f 7267 2f6e 732f 6163 7469 7669  w3.org/ns/activi
 000003d0: 7479 7374 7265 616d 7323 5075 626c 6963  tystreams#Public
 000003e0: a901 7a12 2528 7079 3129 7320 3d3d 2025  ..z.%(py1)s == %
 000003f0: 2870 7934 2973 a902 7216 0000 00da 0370  (py4)s..r......p
 00000400: 7934 fa0e 6173 7365 7274 2025 2870 7936  y4..assert %(py6
 00000410: 2973 da03 7079 3672 0a00 0000 290f 7204  )s..py6r....).r.
 00000420: 0000 00da 046e 6f74 65da 0961 735f 7075  .....note..as_pu
-00000430: 626c 6963 720b 0000 00da 0562 7569 6c64  blicr......build
+00000430: 626c 6963 7209 0000 00da 0562 7569 6c64  blicr......build
 00000440: da04 6b65 7973 7212 0000 00da 0a40 7079  ..keysr......@py
 00000450: 7465 7374 5f61 72da 115f 6361 6c6c 5f72  test_ar.._call_r
 00000460: 6570 7263 6f6d 7061 7265 da0c 4070 795f  eprcompare..@py_
 00000470: 6275 696c 7469 6e73 da06 6c6f 6361 6c73  builtins..locals
 00000480: da18 5f73 686f 756c 645f 7265 7072 5f67  .._should_repr_g
 00000490: 6c6f 6261 6c5f 6e61 6d65 da09 5f73 6166  lobal_name.._saf
 000004a0: 6572 6570 72da 0e41 7373 6572 7469 6f6e  erepr..Assertion
@@ -81,118 +81,118 @@
 00000500: da0b 4070 795f 6173 7365 7274 36da 0b40  ..@py_assert6..@
 00000510: 7079 5f61 7373 6572 7439 da0b 4070 795f  py_assert9..@py_
 00000520: 6173 7365 7274 38da 0c40 7079 5f66 6f72  assert8..@py_for
 00000530: 6d61 7431 31da 0c40 7079 5f66 6f72 6d61  mat11..@py_forma
 00000540: 7431 33da 0b40 7079 5f61 7373 6572 7430  t13..@py_assert0
 00000550: da0b 4070 795f 6173 7365 7274 33da 0b40  ..@py_assert3..@
 00000560: 7079 5f66 6f72 6d61 7435 da0b 4070 795f  py_format5..@py_
-00000570: 666f 726d 6174 37a9 0072 3a00 0000 fa5e  format7..r:....^
+00000570: 666f 726d 6174 37a9 0072 3a00 0000 fa5f  format7..r:...._
 00000580: 2f77 6f6f 6470 6563 6b65 722f 7372 632f  /woodpecker/src/
-00000590: 636f 6465 6265 7267 2e6f 7267 2f68 656c  codeberg.org/hel
-000005a0: 6765 2f62 6f76 696e 652f 626f 7669 6e65  ge/bovine/bovine
-000005b0: 2f62 6f76 696e 652f 6163 7469 7669 7479  /bovine/activity
-000005c0: 7374 7265 616d 732f 7465 7374 5f6f 626a  streams/test_obj
-000005d0: 6563 745f 6661 6374 6f72 792e 7079 da13  ect_factory.py..
-000005e0: 7465 7374 5f6f 626a 6563 745f 6661 6374  test_object_fact
-000005f0: 6f72 7907 0000 0073 6a00 0000 0e01 0c02  ory....sj.......
-00000600: 0601 0801 0202 0207 26f9 0207 0ef9 0207  ........&.......
-00000610: 04f9 0407 06f9 0207 02f9 0207 04f9 0207  ................
-00000620: 02f9 0407 06f9 0407 06f9 0207 02f9 0207  ................
-00000630: 04f9 0207 02f9 0407 04f9 0207 02f9 0207  ................
-00000640: 02f9 0207 02f9 0207 02f9 0207 02f9 0207  ................
-00000650: 02f9 0207 02f9 0207 18f9 0207 02f9 0207  ................
-00000660: 18f9 6c09 7001 723c 0000 0063 0000 0000  ..l.p.r<...c....
-00000670: 0000 0000 0000 0000 1300 0000 0900 0000  ................
-00000680: c300 0000 7384 0200 0081 0174 0083 007d  ....s......t...}
-00000690: 0074 0083 007d 0164 017d 027c 017c 006a  .t...}.d.}.|.|.j
-000006a0: 016a 025f 0374 04a0 0564 027c 0264 0364  .j._.t...d.|.d.d
-000006b0: 0464 059c 04a1 017c 016a 065f 0374 077c  .d.....|.j._.t.|
-000006c0: 0064 068d 017d 037c 03a0 087c 02a1 0149  .d...}.|...|...I
-000006d0: 0064 0048 007d 047c 04a0 09a1 007d 057c  .d.H.}.|.....}.|
-000006e0: 056a 0a7d 067c 0683 007d 0774 0b7c 0783  .j.}.|...}.t.|..
-000006f0: 017d 0868 0064 07a3 017d 097c 087c 096b  .}.h.d...}.|.|.k
-00000700: 027d 0a7c 0a73 8c74 0ca0 0d64 087c 0a66  .}.|.s.t...d.|.f
-00000710: 0164 097c 087c 0966 02a1 0464 0a74 0ea0  .d.|.|.f...d.t..
-00000720: 0fa1 0076 0073 5474 0ca0 1074 0ba1 0172  ...v.sTt...t...r
-00000730: 5974 0ca0 1174 0ba1 016e 0164 0a64 0b74  Yt...t...n.d.d.t
-00000740: 0ea0 0fa1 0076 0073 6574 0ca0 107c 05a1  .....v.set...|..
-00000750: 0172 6a74 0ca0 117c 05a1 016e 0164 0b74  .rjt...|...n.d.t
-00000760: 0ca0 117c 06a1 0174 0ca0 117c 07a1 0174  ...|...t...|...t
-00000770: 0ca0 117c 08a1 0174 0ca0 117c 09a1 0164  ...|...t...|...d
-00000780: 0c9c 0616 007d 0b64 0d64 0e7c 0b69 0116  .....}.d.d.|.i..
-00000790: 007d 0c74 1274 0ca0 137c 0ca1 0183 0182  .}.t.t...|......
-000007a0: 0164 0004 007d 0604 007d 0704 007d 0804  .d...}...}...}..
-000007b0: 007d 0a7d 097c 0564 0f19 007d 0d64 107d  .}.}.|.d...}.d.}
-000007c0: 0e7c 0d7c 0e6b 027d 067c 0673 c574 0ca0  .|.|.k.}.|.s.t..
-000007d0: 0d64 087c 0666 0164 117c 0d7c 0e66 02a1  .d.|.f.d.|.|.f..
-000007e0: 0474 0ca0 117c 0da1 0174 0ca0 117c 0ea1  .t...|...t...|..
-000007f0: 0164 129c 0216 007d 0f64 1364 147c 0f69  .d.....}.d.d.|.i
-00000800: 0116 007d 1074 1274 0ca0 137c 10a1 0183  ...}.t.t...|....
-00000810: 0182 0164 0004 007d 0d04 007d 067d 0e7c  ...d...}...}.}.|
-00000820: 0564 1519 007d 0d7c 0d7c 026b 027d 067c  .d...}.|.|.k.}.|
-00000830: 0690 0173 0674 0ca0 0d64 087c 0666 0164  ...s.t...d.|.f.d
-00000840: 167c 0d7c 0266 02a1 0474 0ca0 117c 0da1  .|.|.f...t...|..
-00000850: 0164 1774 0ea0 0fa1 0076 0073 ef74 0ca0  .d.t.....v.s.t..
-00000860: 107c 02a1 0172 f474 0ca0 117c 02a1 016e  .|...r.t...|...n
-00000870: 0164 1764 189c 0216 007d 1164 1964 1a7c  .d.d.....}.d.d.|
-00000880: 1169 0116 007d 1274 1274 0ca0 137c 12a1  .i...}.t.t...|..
-00000890: 0183 0182 0164 0004 007d 0d7d 067c 0564  .....d...}.}.|.d
-000008a0: 1b19 007d 0d64 1c7d 0e7c 0d7c 0e6b 027d  ...}.d.}.|.|.k.}
-000008b0: 067c 0690 0173 3a74 0ca0 0d64 087c 0666  .|...s:t...d.|.f
-000008c0: 0164 117c 0d7c 0e66 02a1 0474 0ca0 117c  .d.|.|.f...t...|
-000008d0: 0da1 0174 0ca0 117c 0ea1 0164 129c 0216  ...t...|...d....
-000008e0: 007d 0f64 1364 147c 0f69 0116 007d 1074  .}.d.d.|.i...}.t
-000008f0: 1274 0ca0 137c 10a1 0183 0182 0164 0004  .t...|.......d..
-00000900: 007d 0d04 007d 067d 0e64 0053 0029 1d4e  .}...}.}.d.S.).N
-00000910: 7a14 6874 7470 733a 2f2f 7265 6d6f 7465  z.https://remote
-00000920: 2f61 6c69 6365 7a25 6874 7470 733a 2f2f  /alicez%https://
-00000930: 7777 772e 7733 2e6f 7267 2f6e 732f 6163  www.w3.org/ns/ac
-00000940: 7469 7669 7479 7374 7265 616d 73da 0650  tivitystreams..P
-00000950: 6572 736f 6e5a 0661 6c79 7373 6129 0472  ersonZ.alyssa).r
-00000960: 0c00 0000 7207 0000 0072 0d00 0000 da11  ....r....r......
-00000970: 7072 6566 6572 7265 6455 7365 726e 616d  preferredUsernam
-00000980: 6529 01da 0663 6c69 656e 743e 0400 0000  e)...client>....
-00000990: da04 6e61 6d65 720d 0000 0072 0c00 0000  ..namer....r....
-000009a0: da04 6872 6566 720f 0000 0072 1100 0000  ..hrefr....r....
-000009b0: 7212 0000 00da 076d 656e 7469 6f6e 7214  r......mentionr.
-000009c0: 0000 0072 1b00 0000 721c 0000 0072 0d00  ...r....r....r..
-000009d0: 0000 da07 4d65 6e74 696f 6e72 1d00 0000  ....Mentionr....
-000009e0: 721e 0000 0072 2000 0000 7221 0000 0072  r....r ...r!...r
-000009f0: 4100 0000 2901 7a12 2528 7079 3129 7320  A...).z.%(py1)s 
-00000a00: 3d3d 2025 2870 7933 2973 da0a 7265 6d6f  == %(py3)s..remo
-00000a10: 7465 5f75 7269 2902 7216 0000 0072 1700  te_uri).r....r..
-00000a20: 0000 7a0e 6173 7365 7274 2025 2870 7935  ..z.assert %(py5
-00000a30: 2973 7218 0000 0072 4000 0000 7a0d 616c  )sr....r@...z.al
-00000a40: 7973 7361 4072 656d 6f74 6529 1472 0200  yssa@remote).r..
-00000a50: 0000 723f 0000 00da 0367 6574 da0c 7265  ..r?.....get..re
-00000a60: 7475 726e 5f76 616c 7565 da04 6a73 6f6e  turn_value..json
-00000a70: da05 6475 6d70 7372 0800 0000 7204 0000  ..dumpsr....r...
-00000a80: 00da 156d 656e 7469 6f6e 5f66 6f72 5f61  ...mention_for_a
-00000a90: 6374 6f72 5f75 7269 7224 0000 0072 2500  ctor_urir$...r%.
-00000aa0: 0000 7212 0000 0072 2600 0000 7227 0000  ..r....r&...r'..
-00000ab0: 0072 2800 0000 7229 0000 0072 2a00 0000  .r(...r)...r*...
-00000ac0: 722b 0000 0072 2c00 0000 722d 0000 0029  r+...r,...r-...)
-00000ad0: 135a 0b6d 6f63 6b5f 636c 6965 6e74 5a0d  .Z.mock_clientZ.
-00000ae0: 6d6f 636b 5f72 6573 706f 6e73 6572 4400  mock_responserD.
-00000af0: 0000 722e 0000 005a 0e6d 656e 7469 6f6e  ..r....Z.mention
-00000b00: 5f6f 626a 6563 7472 4200 0000 722f 0000  _objectrB...r/..
-00000b10: 0072 3000 0000 7231 0000 0072 3200 0000  .r0...r1...r2...
-00000b20: 7233 0000 0072 3400 0000 7235 0000 0072  r3...r4...r5...r
-00000b30: 3600 0000 7237 0000 0072 3800 0000 7239  6...r7...r8...r9
-00000b40: 0000 00da 0b40 7079 5f66 6f72 6d61 7434  .....@py_format4
-00000b50: da0b 4070 795f 666f 726d 6174 3672 3a00  ..@py_format6r:.
-00000b60: 0000 723a 0000 0072 3b00 0000 da1a 7465  ..r:...r;.....te
-00000b70: 7374 5f6d 656e 7469 6f6e 5f66 6f72 5f61  st_mention_for_a
-00000b80: 6374 6f72 5f75 7269 1b00 0000 7326 0000  ctor_uri....s&..
-00000b90: 0002 8006 0106 0104 010a 0204 0202 0202  ................
-00000ba0: 0102 0102 0104 fc08 ff0a 0910 0208 01d6  ................
-00000bb0: 026a 017e 0170 0172 4c00 0000 290d da08  .j.~.p.rL...)...
-00000bc0: 6275 696c 7469 6e73 7228 0000 00da 195f  builtinsr(....._
-00000bd0: 7079 7465 7374 2e61 7373 6572 7469 6f6e  pytest.assertion
-00000be0: 2e72 6577 7269 7465 da09 6173 7365 7274  .rewrite..assert
-00000bf0: 696f 6eda 0772 6577 7269 7465 7226 0000  ion..rewriter&..
-00000c00: 0072 4700 0000 da0d 756e 6974 7465 7374  .rG.....unittest
-00000c10: 2e6d 6f63 6b72 0200 0000 722e 0000 0072  .mockr....r....r
-00000c20: 0400 0000 723c 0000 0072 4c00 0000 723a  ....r<...rL...r:
-00000c30: 0000 0072 3a00 0000 723a 0000 0072 3b00  ...r:...r:...r;.
-00000c40: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
-00000c50: 730a 0000 0022 000c 010c 0208 030c 14    s....".........
+00000590: 636f 6465 6265 7267 2e6f 7267 2f62 6f76  codeberg.org/bov
+000005a0: 696e 652f 626f 7669 6e65 2f62 6f76 696e  ine/bovine/bovin
+000005b0: 652f 626f 7669 6e65 2f61 6374 6976 6974  e/bovine/activit
+000005c0: 7973 7472 6561 6d73 2f74 6573 745f 6f62  ystreams/test_ob
+000005d0: 6a65 6374 5f66 6163 746f 7279 2e70 79da  ject_factory.py.
+000005e0: 1374 6573 745f 6f62 6a65 6374 5f66 6163  .test_object_fac
+000005f0: 746f 7279 0700 0000 736a 0000 000e 010c  tory....sj......
+00000600: 0206 0108 0102 0202 0726 f902 070e f902  .........&......
+00000610: 0704 f904 0706 f902 0702 f902 0704 f902  ................
+00000620: 0702 f904 0706 f904 0706 f902 0702 f902  ................
+00000630: 0704 f902 0702 f904 0704 f902 0702 f902  ................
+00000640: 0702 f902 0702 f902 0702 f902 0702 f902  ................
+00000650: 0702 f902 0702 f902 0718 f902 0702 f902  ................
+00000660: 0718 f96c 0970 0172 3c00 0000 6300 0000  ...l.p.r<...c...
+00000670: 0000 0000 0000 0000 0013 0000 0009 0000  ................
+00000680: 00c3 0000 0073 8402 0000 8101 7400 8300  .....s......t...
+00000690: 7d00 7400 8300 7d01 6401 7d02 7c01 7c00  }.t...}.d.}.|.|.
+000006a0: 6a01 6a02 5f03 7404 a005 6402 7c02 6403  j.j._.t...d.|.d.
+000006b0: 6404 6405 9c04 a101 7c01 6a06 5f03 7407  d.d.....|.j._.t.
+000006c0: 7c00 6406 8d01 7d03 7c03 a008 7c02 a101  |.d...}.|...|...
+000006d0: 4900 6400 4800 7d04 7c04 a009 a100 7d05  I.d.H.}.|.....}.
+000006e0: 7c05 6a0a 7d06 7c06 8300 7d07 740b 7c07  |.j.}.|...}.t.|.
+000006f0: 8301 7d08 6800 6407 a301 7d09 7c08 7c09  ..}.h.d...}.|.|.
+00000700: 6b02 7d0a 7c0a 738c 740c a00d 6408 7c0a  k.}.|.s.t...d.|.
+00000710: 6601 6409 7c08 7c09 6602 a104 640a 740e  f.d.|.|.f...d.t.
+00000720: a00f a100 7600 7354 740c a010 740b a101  ....v.sTt...t...
+00000730: 7259 740c a011 740b a101 6e01 640a 640b  rYt...t...n.d.d.
+00000740: 740e a00f a100 7600 7365 740c a010 7c05  t.....v.set...|.
+00000750: a101 726a 740c a011 7c05 a101 6e01 640b  ..rjt...|...n.d.
+00000760: 740c a011 7c06 a101 740c a011 7c07 a101  t...|...t...|...
+00000770: 740c a011 7c08 a101 740c a011 7c09 a101  t...|...t...|...
+00000780: 640c 9c06 1600 7d0b 640d 640e 7c0b 6901  d.....}.d.d.|.i.
+00000790: 1600 7d0c 7412 740c a013 7c0c a101 8301  ..}.t.t...|.....
+000007a0: 8201 6400 0400 7d06 0400 7d07 0400 7d08  ..d...}...}...}.
+000007b0: 0400 7d0a 7d09 7c05 640f 1900 7d0d 6410  ..}.}.|.d...}.d.
+000007c0: 7d0e 7c0d 7c0e 6b02 7d06 7c06 73c5 740c  }.|.|.k.}.|.s.t.
+000007d0: a00d 6408 7c06 6601 6411 7c0d 7c0e 6602  ..d.|.f.d.|.|.f.
+000007e0: a104 740c a011 7c0d a101 740c a011 7c0e  ..t...|...t...|.
+000007f0: a101 6412 9c02 1600 7d0f 6413 6414 7c0f  ..d.....}.d.d.|.
+00000800: 6901 1600 7d10 7412 740c a013 7c10 a101  i...}.t.t...|...
+00000810: 8301 8201 6400 0400 7d0d 0400 7d06 7d0e  ....d...}...}.}.
+00000820: 7c05 6415 1900 7d0d 7c0d 7c02 6b02 7d06  |.d...}.|.|.k.}.
+00000830: 7c06 9001 7306 740c a00d 6408 7c06 6601  |...s.t...d.|.f.
+00000840: 6416 7c0d 7c02 6602 a104 740c a011 7c0d  d.|.|.f...t...|.
+00000850: a101 6417 740e a00f a100 7600 73ef 740c  ..d.t.....v.s.t.
+00000860: a010 7c02 a101 72f4 740c a011 7c02 a101  ..|...r.t...|...
+00000870: 6e01 6417 6418 9c02 1600 7d11 6419 641a  n.d.d.....}.d.d.
+00000880: 7c11 6901 1600 7d12 7412 740c a013 7c12  |.i...}.t.t...|.
+00000890: a101 8301 8201 6400 0400 7d0d 7d06 7c05  ......d...}.}.|.
+000008a0: 641b 1900 7d0d 641c 7d0e 7c0d 7c0e 6b02  d...}.d.}.|.|.k.
+000008b0: 7d06 7c06 9001 733a 740c a00d 6408 7c06  }.|...s:t...d.|.
+000008c0: 6601 6411 7c0d 7c0e 6602 a104 740c a011  f.d.|.|.f...t...
+000008d0: 7c0d a101 740c a011 7c0e a101 6412 9c02  |...t...|...d...
+000008e0: 1600 7d0f 6413 6414 7c0f 6901 1600 7d10  ..}.d.d.|.i...}.
+000008f0: 7412 740c a013 7c10 a101 8301 8201 6400  t.t...|.......d.
+00000900: 0400 7d0d 0400 7d06 7d0e 6400 5300 291d  ..}...}.}.d.S.).
+00000910: 4e7a 1468 7474 7073 3a2f 2f72 656d 6f74  Nz.https://remot
+00000920: 652f 616c 6963 657a 2568 7474 7073 3a2f  e/alicez%https:/
+00000930: 2f77 7777 2e77 332e 6f72 672f 6e73 2f61  /www.w3.org/ns/a
+00000940: 6374 6976 6974 7973 7472 6561 6d73 da06  ctivitystreams..
+00000950: 5065 7273 6f6e 5a06 616c 7973 7361 2904  PersonZ.alyssa).
+00000960: 720b 0000 0072 0700 0000 720c 0000 00da  r....r....r.....
+00000970: 1170 7265 6665 7272 6564 5573 6572 6e61  .preferredUserna
+00000980: 6d65 2901 da06 636c 6965 6e74 3e04 0000  me)...client>...
+00000990: 0072 0b00 0000 da04 6e61 6d65 720c 0000  .r......namer...
+000009a0: 00da 0468 7265 6672 0f00 0000 7211 0000  ...hrefr....r...
+000009b0: 0072 1200 0000 da07 6d65 6e74 696f 6e72  .r......mentionr
+000009c0: 1400 0000 721b 0000 0072 1c00 0000 720c  ....r....r....r.
+000009d0: 0000 00da 074d 656e 7469 6f6e 721d 0000  .....Mentionr...
+000009e0: 0072 1e00 0000 7220 0000 0072 2100 0000  .r....r ...r!...
+000009f0: 7241 0000 0029 017a 1225 2870 7931 2973  rA...).z.%(py1)s
+00000a00: 203d 3d20 2528 7079 3329 73da 0a72 656d   == %(py3)s..rem
+00000a10: 6f74 655f 7572 6929 0272 1600 0000 7217  ote_uri).r....r.
+00000a20: 0000 007a 0e61 7373 6572 7420 2528 7079  ...z.assert %(py
+00000a30: 3529 7372 1800 0000 7240 0000 007a 0d61  5)sr....r@...z.a
+00000a40: 6c79 7373 6140 7265 6d6f 7465 2914 7202  lyssa@remote).r.
+00000a50: 0000 0072 3f00 0000 da03 6765 74da 0c72  ...r?.....get..r
+00000a60: 6574 7572 6e5f 7661 6c75 65da 046a 736f  eturn_value..jso
+00000a70: 6eda 0564 756d 7073 7208 0000 0072 0400  n..dumpsr....r..
+00000a80: 0000 da15 6d65 6e74 696f 6e5f 666f 725f  ....mention_for_
+00000a90: 6163 746f 725f 7572 6972 2400 0000 7225  actor_urir$...r%
+00000aa0: 0000 0072 1200 0000 7226 0000 0072 2700  ...r....r&...r'.
+00000ab0: 0000 7228 0000 0072 2900 0000 722a 0000  ..r(...r)...r*..
+00000ac0: 0072 2b00 0000 722c 0000 0072 2d00 0000  .r+...r,...r-...
+00000ad0: 2913 5a0b 6d6f 636b 5f63 6c69 656e 745a  ).Z.mock_clientZ
+00000ae0: 0d6d 6f63 6b5f 7265 7370 6f6e 7365 7244  .mock_responserD
+00000af0: 0000 0072 2e00 0000 5a0e 6d65 6e74 696f  ...r....Z.mentio
+00000b00: 6e5f 6f62 6a65 6374 7242 0000 0072 2f00  n_objectrB...r/.
+00000b10: 0000 7230 0000 0072 3100 0000 7232 0000  ..r0...r1...r2..
+00000b20: 0072 3300 0000 7234 0000 0072 3500 0000  .r3...r4...r5...
+00000b30: 7236 0000 0072 3700 0000 7238 0000 0072  r6...r7...r8...r
+00000b40: 3900 0000 da0b 4070 795f 666f 726d 6174  9.....@py_format
+00000b50: 34da 0b40 7079 5f66 6f72 6d61 7436 723a  4..@py_format6r:
+00000b60: 0000 0072 3a00 0000 723b 0000 00da 1a74  ...r:...r;.....t
+00000b70: 6573 745f 6d65 6e74 696f 6e5f 666f 725f  est_mention_for_
+00000b80: 6163 746f 725f 7572 691b 0000 0073 2600  actor_uri....s&.
+00000b90: 0000 0280 0601 0601 0401 0a02 0402 0202  ................
+00000ba0: 0201 0201 0201 04fc 08ff 0a09 1002 0801  ................
+00000bb0: d602 6a01 7e01 7001 724c 0000 0029 0dda  ..j.~.p.rL...)..
+00000bc0: 0862 7569 6c74 696e 7372 2800 0000 da19  .builtinsr(.....
+00000bd0: 5f70 7974 6573 742e 6173 7365 7274 696f  _pytest.assertio
+00000be0: 6e2e 7265 7772 6974 65da 0961 7373 6572  n.rewrite..asser
+00000bf0: 7469 6f6e da07 7265 7772 6974 6572 2600  tion..rewriter&.
+00000c00: 0000 7247 0000 00da 0d75 6e69 7474 6573  ..rG.....unittes
+00000c10: 742e 6d6f 636b 7202 0000 0072 2e00 0000  t.mockr....r....
+00000c20: 7204 0000 0072 3c00 0000 724c 0000 0072  r....r<...rL...r
+00000c30: 3a00 0000 723a 0000 0072 3a00 0000 723b  :...r:...r:...r;
+00000c40: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
+00000c50: 0073 0a00 0000 2200 0c01 0c02 0803 0c14  .s....".........
```

### Comparing `bovine-0.1.0/bovine/activitystreams/__pycache__/test_ordered_collection_builder.cpython-310-pytest-7.3.0.pyc` & `bovine-0.1.1/bovine/activitystreams/__pycache__/test_ordered_collection_builder.cpython-310-pytest-7.3.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 13 15:55:57 2023 UTC, .py size: 1165 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 26% similar despite different names*

```diff
@@ -1,131 +1,121 @@
-00000000: 6f0d 0d0a 0000 0000 0d26 3864 8d04 0000  o........&8d....
+00000000: 6f0d 0d0a 0000 0000 a4ea 3a64 f203 0000  o.........:d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 4200 0000 6400  .....@...sB...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6402 6403 6c06 6d07  ..m.Z...d.d.l.m.
 00000050: 5a07 0100 6404 6405 8400 5a08 6406 6407  Z...d.d...Z.d.d.
 00000060: 8400 5a09 6408 6409 8400 5a0a 6401 5300  ..Z.d.d...Z.d.S.
 00000070: 290a e900 0000 004e e901 0000 0029 01da  )......N.....)..
-00000080: 184f 7264 6572 6564 436f 6c6c 6563 7469  .OrderedCollecti
-00000090: 6f6e 4275 696c 6465 7263 0000 0000 0000  onBuilderc......
-000000a0: 0000 0000 0000 0500 0000 0700 0000 4300  ..............C.
-000000b0: 0000 7392 0000 0074 0064 0183 01a0 01a1  ..s....t.d......
-000000c0: 007d 0064 0264 0164 0364 0464 059c 047d  .}.d.d.d.d.d...}
-000000d0: 017c 007c 016b 027d 027c 0273 4374 02a0  .|.|.k.}.|.sCt..
-000000e0: 0364 067c 0266 0164 077c 007c 0166 02a1  .d.|.f.d.|.|.f..
-000000f0: 0464 0874 04a0 05a1 0076 0073 2874 02a0  .d.t.....v.s(t..
-00000100: 067c 00a1 0172 2d74 02a0 077c 00a1 016e  .|...r-t...|...n
-00000110: 0164 0874 02a0 077c 01a1 0164 099c 0216  .d.t...|...d....
-00000120: 007d 0364 0a64 0b7c 0369 0116 007d 0474  .}.d.d.|.i...}.t
-00000130: 0874 02a0 097c 04a1 0183 0182 0164 0004  .t...|.......d..
-00000140: 007d 027d 0164 0053 0029 0c4e da03 7572  .}.}.d.S.).N..ur
-00000150: 6cfa 2568 7474 7073 3a2f 2f77 7777 2e77  l.%https://www.w
-00000160: 332e 6f72 672f 6e73 2f61 6374 6976 6974  3.org/ns/activit
-00000170: 7973 7472 6561 6d73 7201 0000 00da 114f  ystreamsr......O
-00000180: 7264 6572 6564 436f 6c6c 6563 7469 6f6e  rderedCollection
-00000190: 2904 fa08 4063 6f6e 7465 7874 da02 6964  )...@context..id
-000001a0: da0a 746f 7461 6c49 7465 6d73 da04 7479  ..totalItems..ty
-000001b0: 7065 a901 fa02 3d3d a901 7a12 2528 7079  pe....==..z.%(py
-000001c0: 3029 7320 3d3d 2025 2870 7933 2973 da06  0)s == %(py3)s..
-000001d0: 7265 7375 6c74 a902 da03 7079 30da 0370  result....py0..p
-000001e0: 7933 fa0e 6173 7365 7274 2025 2870 7935  y3..assert %(py5
-000001f0: 2973 da03 7079 3529 0a72 0300 0000 da05  )s..py5).r......
-00000200: 6275 696c 64da 0a40 7079 7465 7374 5f61  build..@pytest_a
-00000210: 72da 115f 6361 6c6c 5f72 6570 7263 6f6d  r.._call_reprcom
-00000220: 7061 7265 da0c 4070 795f 6275 696c 7469  pare..@py_builti
-00000230: 6e73 da06 6c6f 6361 6c73 da18 5f73 686f  ns..locals.._sho
-00000240: 756c 645f 7265 7072 5f67 6c6f 6261 6c5f  uld_repr_global_
-00000250: 6e61 6d65 da09 5f73 6166 6572 6570 72da  name.._saferepr.
-00000260: 0e41 7373 6572 7469 6f6e 4572 726f 72da  .AssertionError.
-00000270: 135f 666f 726d 6174 5f65 7870 6c61 6e61  ._format_explana
-00000280: 7469 6f6e a905 720e 0000 00da 0b40 7079  tion..r......@py
-00000290: 5f61 7373 6572 7432 da0b 4070 795f 6173  _assert2..@py_as
-000002a0: 7365 7274 31da 0b40 7079 5f66 6f72 6d61  sert1..@py_forma
-000002b0: 7434 da0b 4070 795f 666f 726d 6174 36a9  t4..@py_format6.
-000002c0: 0072 2200 0000 fa6a 2f77 6f6f 6470 6563  .r"....j/woodpec
-000002d0: 6b65 722f 7372 632f 636f 6465 6265 7267  ker/src/codeberg
-000002e0: 2e6f 7267 2f68 656c 6765 2f62 6f76 696e  .org/helge/bovin
-000002f0: 652f 626f 7669 6e65 2f62 6f76 696e 652f  e/bovine/bovine/
-00000300: 6163 7469 7669 7479 7374 7265 616d 732f  activitystreams/
-00000310: 7465 7374 5f6f 7264 6572 6564 5f63 6f6c  test_ordered_col
-00000320: 6c65 6374 696f 6e5f 6275 696c 6465 722e  lection_builder.
-00000330: 7079 da1f 7465 7374 5f6f 7264 6572 6564  py..test_ordered
-00000340: 5f63 6f6c 6c65 6374 696f 6e5f 6275 696c  _collection_buil
-00000350: 6465 7204 0000 0073 3000 0000 0c01 1c02  der....s0.......
-00000360: 0205 0efb 0205 04fb 0405 06fb 0205 02fb  ................
-00000370: 0205 04fb 0205 02fb 0405 04fb 0205 02fb  ................
-00000380: 0205 18fb 0205 02fb 0205 10fb 7224 0000  ............r$..
-00000390: 0063 0000 0000 0000 0000 0000 0000 0500  .c..............
-000003a0: 0000 0700 0000 4300 0000 73ac 0000 0074  ......C...s....t
-000003b0: 0064 0183 01a0 0164 02a1 01a0 0264 0364  .d.....d.....d.d
-000003c0: 0469 0167 01a1 01a0 03a1 007d 0064 0564  .i.g.......}.d.d
-000003d0: 0164 0364 0469 0167 0164 0264 0664 079c  .d.d.i.g.d.d.d..
-000003e0: 057d 017c 007c 016b 027d 027c 0273 5074  .}.|.|.k.}.|.sPt
-000003f0: 04a0 0564 087c 0266 0164 097c 007c 0166  ...d.|.f.d.|.|.f
-00000400: 02a1 0464 0a74 06a0 07a1 0076 0073 3574  ...d.t.....v.s5t
-00000410: 04a0 087c 00a1 0172 3a74 04a0 097c 00a1  ...|...r:t...|..
-00000420: 016e 0164 0a74 04a0 097c 01a1 0164 0b9c  .n.d.t...|...d..
-00000430: 0216 007d 0364 0c64 0d7c 0369 0116 007d  ...}.d.d.|.i...}
-00000440: 0474 0a74 04a0 0b7c 04a1 0183 0182 0164  .t.t...|.......d
-00000450: 0004 007d 027d 0164 0053 0029 0e4e 7204  ...}.}.d.S.).Nr.
-00000460: 0000 0072 0200 0000 da04 6974 656d da01  ...r......item..
-00000470: 3172 0500 0000 7206 0000 0029 0572 0700  1r....r....).r..
-00000480: 0000 7208 0000 00da 0c6f 7264 6572 6564  ..r......ordered
-00000490: 4974 656d 7372 0900 0000 720a 0000 0072  Itemsr....r....r
-000004a0: 0b00 0000 720d 0000 0072 0e00 0000 720f  ....r....r....r.
-000004b0: 0000 0072 1200 0000 7213 0000 0029 0c72  ...r....r....).r
-000004c0: 0300 0000 da0a 7769 7468 5f63 6f75 6e74  ......with_count
-000004d0: da0a 7769 7468 5f69 7465 6d73 7214 0000  ..with_itemsr...
-000004e0: 0072 1500 0000 7216 0000 0072 1700 0000  .r....r....r....
-000004f0: 7218 0000 0072 1900 0000 721a 0000 0072  r....r....r....r
-00000500: 1b00 0000 721c 0000 0072 1d00 0000 7222  ....r....r....r"
-00000510: 0000 0072 2200 0000 7223 0000 00da 2a74  ...r"...r#....*t
-00000520: 6573 745f 6f72 6465 7265 645f 636f 6c6c  est_ordered_coll
-00000530: 6563 7469 6f6e 5f62 7569 6c64 6572 5f77  ection_builder_w
-00000540: 6974 685f 6974 656d 730f 0000 0073 3800  ith_items....s8.
-00000550: 0000 0602 0601 0c01 0401 02fc 2407 0206  ............$...
-00000560: 0efa 0206 04fa 0406 06fa 0206 02fa 0206  ................
-00000570: 04fa 0206 02fa 0406 04fa 0206 02fa 0206  ................
-00000580: 18fa 0206 02fa 0206 10fa 722a 0000 0063  ..........r*...c
-00000590: 0000 0000 0000 0000 0000 0000 0500 0000  ................
-000005a0: 0700 0000 4300 0000 73a4 0000 0074 0064  ....C...s....t.d
-000005b0: 0183 01a0 0164 02a1 01a0 0264 0364 04a1  .....d.....d.d..
-000005c0: 02a0 03a1 007d 0064 0564 0164 0364 0464  .....}.d.d.d.d.d
-000005d0: 0264 0664 079c 067d 017c 007c 016b 027d  .d.d...}.|.|.k.}
-000005e0: 027c 0273 4c74 04a0 0564 087c 0266 0164  .|.sLt...d.|.f.d
-000005f0: 097c 007c 0166 02a1 0464 0a74 06a0 07a1  .|.|.f...d.t....
-00000600: 0076 0073 3174 04a0 087c 00a1 0172 3674  .v.s1t...|...r6t
-00000610: 04a0 097c 00a1 016e 0164 0a74 04a0 097c  ...|...n.d.t...|
-00000620: 01a1 0164 0b9c 0216 007d 0364 0c64 0d7c  ...d.....}.d.d.|
-00000630: 0369 0116 007d 0474 0a74 04a0 0b7c 04a1  .i...}.t.t...|..
-00000640: 0183 0182 0164 0004 007d 027d 0164 0053  .....d...}.}.d.S
-00000650: 0029 0e4e 7204 0000 0072 0200 0000 da05  .).Nr....r......
-00000660: 6669 7273 74da 046c 6173 7472 0500 0000  first..lastr....
-00000670: 7206 0000 0029 0672 0700 0000 7208 0000  r....).r....r...
-00000680: 0072 2b00 0000 722c 0000 0072 0900 0000  .r+...r,...r....
-00000690: 720a 0000 0072 0b00 0000 720d 0000 0072  r....r....r....r
-000006a0: 0e00 0000 720f 0000 0072 1200 0000 7213  ....r....r....r.
-000006b0: 0000 0029 0c72 0300 0000 7228 0000 00da  ...).r....r(....
-000006c0: 1377 6974 685f 6669 7273 745f 616e 645f  .with_first_and_
-000006d0: 6c61 7374 7214 0000 0072 1500 0000 7216  lastr....r....r.
-000006e0: 0000 0072 1700 0000 7218 0000 0072 1900  ...r....r....r..
-000006f0: 0000 721a 0000 0072 1b00 0000 721c 0000  ..r....r....r...
-00000700: 0072 1d00 0000 7222 0000 0072 2200 0000  .r....r"...r"...
-00000710: 7223 0000 00da 2e74 6573 745f 6f72 6465  r#.....test_orde
-00000720: 7265 645f 636f 6c6c 6563 7469 6f6e 5f62  red_collection_b
-00000730: 7569 6c64 6572 5f77 6974 685f 6669 7374  uilder_with_fist
-00000740: 5f6c 6173 7420 0000 0073 3800 0000 0602  _last ...s8.....
-00000750: 0601 0801 0401 02fc 2007 0207 0ef9 0207  ........ .......
-00000760: 04f9 0407 06f9 0207 02f9 0207 04f9 0207  ................
-00000770: 02f9 0407 04f9 0207 02f9 0207 18f9 0207  ................
-00000780: 02f9 0207 10f9 722e 0000 0029 0bda 0862  ......r....)...b
-00000790: 7569 6c74 696e 7372 1700 0000 da19 5f70  uiltinsr......_p
-000007a0: 7974 6573 742e 6173 7365 7274 696f 6e2e  ytest.assertion.
-000007b0: 7265 7772 6974 65da 0961 7373 6572 7469  rewrite..asserti
-000007c0: 6f6e da07 7265 7772 6974 6572 1500 0000  on..rewriter....
-000007d0: da1a 6f72 6465 7265 645f 636f 6c6c 6563  ..ordered_collec
-000007e0: 7469 6f6e 5f62 7569 6c64 6572 7203 0000  tion_builderr...
-000007f0: 0072 2400 0000 722a 0000 0072 2e00 0000  .r$...r*...r....
-00000800: 7222 0000 0072 2200 0000 7222 0000 0072  r"...r"...r"...r
-00000810: 2300 0000 da08 3c6d 6f64 756c 653e 0100  #.....<module>..
-00000820: 0000 7308 0000 0026 0008 0308 0b0c 11    ..s....&.......
+00000080: 114f 7264 6572 6564 436f 6c6c 6563 7469  .OrderedCollecti
+00000090: 6f6e 6300 0000 0000 0000 0000 0000 0005  onc.............
+000000a0: 0000 0007 0000 0043 0000 0073 9400 0000  .......C...s....
+000000b0: 7400 6401 6402 8d01 a001 a100 7d00 6403  t.d.d.......}.d.
+000000c0: 6401 6404 6405 6406 9c04 7d01 7c00 7c01  d.d.d.d...}.|.|.
+000000d0: 6b02 7d02 7c02 7344 7402 a003 6407 7c02  k.}.|.sDt...d.|.
+000000e0: 6601 6408 7c00 7c01 6602 a104 6409 7404  f.d.|.|.f...d.t.
+000000f0: a005 a100 7600 7329 7402 a006 7c00 a101  ....v.s)t...|...
+00000100: 722e 7402 a007 7c00 a101 6e01 6409 7402  r.t...|...n.d.t.
+00000110: a007 7c01 a101 640a 9c02 1600 7d03 640b  ..|...d.....}.d.
+00000120: 640c 7c03 6901 1600 7d04 7408 7402 a009  d.|.i...}.t.t...
+00000130: 7c04 a101 8301 8201 6400 0400 7d02 7d01  |.......d...}.}.
+00000140: 6400 5300 290d 4eda 0375 726c 2901 da02  d.S.).N..url)...
+00000150: 6964 fa25 6874 7470 733a 2f2f 7777 772e  id.%https://www.
+00000160: 7733 2e6f 7267 2f6e 732f 6163 7469 7669  w3.org/ns/activi
+00000170: 7479 7374 7265 616d 7372 0100 0000 7203  tystreamsr....r.
+00000180: 0000 0029 04fa 0840 636f 6e74 6578 7472  ...)...@contextr
+00000190: 0500 0000 da0a 746f 7461 6c49 7465 6d73  ......totalItems
+000001a0: da04 7479 7065 a901 fa02 3d3d a901 7a12  ..type....==..z.
+000001b0: 2528 7079 3029 7320 3d3d 2025 2870 7933  %(py0)s == %(py3
+000001c0: 2973 da06 7265 7375 6c74 a902 da03 7079  )s..result....py
+000001d0: 30da 0370 7933 fa0e 6173 7365 7274 2025  0..py3..assert %
+000001e0: 2870 7935 2973 da03 7079 35a9 0a72 0300  (py5)s..py5..r..
+000001f0: 0000 da05 6275 696c 64da 0a40 7079 7465  ....build..@pyte
+00000200: 7374 5f61 72da 115f 6361 6c6c 5f72 6570  st_ar.._call_rep
+00000210: 7263 6f6d 7061 7265 da0c 4070 795f 6275  rcompare..@py_bu
+00000220: 696c 7469 6e73 da06 6c6f 6361 6c73 da18  iltins..locals..
+00000230: 5f73 686f 756c 645f 7265 7072 5f67 6c6f  _should_repr_glo
+00000240: 6261 6c5f 6e61 6d65 da09 5f73 6166 6572  bal_name.._safer
+00000250: 6570 72da 0e41 7373 6572 7469 6f6e 4572  epr..AssertionEr
+00000260: 726f 72da 135f 666f 726d 6174 5f65 7870  ror.._format_exp
+00000270: 6c61 6e61 7469 6f6e a905 720d 0000 00da  lanation..r.....
+00000280: 0b40 7079 5f61 7373 6572 7432 da0b 4070  .@py_assert2..@p
+00000290: 795f 6173 7365 7274 31da 0b40 7079 5f66  y_assert1..@py_f
+000002a0: 6f72 6d61 7434 da0b 4070 795f 666f 726d  ormat4..@py_form
+000002b0: 6174 36a9 0072 2200 0000 fa6b 2f77 6f6f  at6..r"....k/woo
+000002c0: 6470 6563 6b65 722f 7372 632f 636f 6465  dpecker/src/code
+000002d0: 6265 7267 2e6f 7267 2f62 6f76 696e 652f  berg.org/bovine/
+000002e0: 626f 7669 6e65 2f62 6f76 696e 652f 626f  bovine/bovine/bo
+000002f0: 7669 6e65 2f61 6374 6976 6974 7973 7472  vine/activitystr
+00000300: 6561 6d73 2f74 6573 745f 6f72 6465 7265  eams/test_ordere
+00000310: 645f 636f 6c6c 6563 7469 6f6e 5f62 7569  d_collection_bui
+00000320: 6c64 6572 2e70 79da 1f74 6573 745f 6f72  lder.py..test_or
+00000330: 6465 7265 645f 636f 6c6c 6563 7469 6f6e  dered_collection
+00000340: 5f62 7569 6c64 6572 0400 0000 7330 0000  _builder....s0..
+00000350: 000e 011c 0202 050e fb02 0504 fb04 0506  ................
+00000360: fb02 0502 fb02 0504 fb02 0502 fb04 0504  ................
+00000370: fb02 0502 fb02 0518 fb02 0502 fb02 0510  ................
+00000380: fb72 2400 0000 6300 0000 0000 0000 0000  .r$...c.........
+00000390: 0000 0005 0000 0007 0000 0043 0000 0073  ...........C...s
+000003a0: a600 0000 7400 6401 6402 6403 6404 6901  ....t.d.d.d.d.i.
+000003b0: 6701 6405 8d03 a001 a100 7d00 6406 6401  g.d.......}.d.d.
+000003c0: 6403 6404 6901 6701 6402 6407 6408 9c05  d.d.i.g.d.d.d...
+000003d0: 7d01 7c00 7c01 6b02 7d02 7c02 734d 7402  }.|.|.k.}.|.sMt.
+000003e0: a003 6409 7c02 6601 640a 7c00 7c01 6602  ..d.|.f.d.|.|.f.
+000003f0: a104 640b 7404 a005 a100 7600 7332 7402  ..d.t.....v.s2t.
+00000400: a006 7c00 a101 7237 7402 a007 7c00 a101  ..|...r7t...|...
+00000410: 6e01 640b 7402 a007 7c01 a101 640c 9c02  n.d.t...|...d...
+00000420: 1600 7d03 640d 640e 7c03 6901 1600 7d04  ..}.d.d.|.i...}.
+00000430: 7408 7402 a009 7c04 a101 8301 8201 6400  t.t...|.......d.
+00000440: 0400 7d02 7d01 6400 5300 290f 4e72 0400  ..}.}.d.S.).Nr..
+00000450: 0000 7202 0000 00da 0469 7465 6dda 0131  ..r......item..1
+00000460: 2903 7205 0000 00da 0563 6f75 6e74 da05  ).r......count..
+00000470: 6974 656d 7372 0600 0000 7203 0000 0029  itemsr....r....)
+00000480: 0572 0700 0000 7205 0000 00da 0c6f 7264  .r....r......ord
+00000490: 6572 6564 4974 656d 7372 0800 0000 7209  eredItemsr....r.
+000004a0: 0000 0072 0a00 0000 720c 0000 0072 0d00  ...r....r....r..
+000004b0: 0000 720e 0000 0072 1100 0000 7212 0000  ..r....r....r...
+000004c0: 0072 1300 0000 721d 0000 0072 2200 0000  .r....r....r"...
+000004d0: 7222 0000 0072 2300 0000 da2a 7465 7374  r"...r#....*test
+000004e0: 5f6f 7264 6572 6564 5f63 6f6c 6c65 6374  _ordered_collect
+000004f0: 696f 6e5f 6275 696c 6465 725f 7769 7468  ion_builder_with
+00000500: 5f69 7465 6d73 0f00 0000 7330 0000 0018  _items....s0....
+00000510: 0124 0202 060e fa02 0604 fa04 0606 fa02  .$..............
+00000520: 0602 fa02 0604 fa02 0602 fa04 0604 fa02  ................
+00000530: 0602 fa02 0618 fa02 0602 fa02 0610 fa72  ...............r
+00000540: 2a00 0000 6300 0000 0000 0000 0000 0000  *...c...........
+00000550: 0005 0000 0007 0000 0043 0000 0073 9e00  .........C...s..
+00000560: 0000 7400 6401 6402 6403 6404 6405 8d04  ..t.d.d.d.d.d...
+00000570: a001 a100 7d00 6406 6401 6403 6404 6402  ....}.d.d.d.d.d.
+00000580: 6407 6408 9c06 7d01 7c00 7c01 6b02 7d02  d.d...}.|.|.k.}.
+00000590: 7c02 7349 7402 a003 6409 7c02 6601 640a  |.sIt...d.|.f.d.
+000005a0: 7c00 7c01 6602 a104 640b 7404 a005 a100  |.|.f...d.t.....
+000005b0: 7600 732e 7402 a006 7c00 a101 7233 7402  v.s.t...|...r3t.
+000005c0: a007 7c00 a101 6e01 640b 7402 a007 7c01  ..|...n.d.t...|.
+000005d0: a101 640c 9c02 1600 7d03 640d 640e 7c03  ..d.....}.d.d.|.
+000005e0: 6901 1600 7d04 7408 7402 a009 7c04 a101  i...}.t.t...|...
+000005f0: 8301 8201 6400 0400 7d02 7d01 6400 5300  ....d...}.}.d.S.
+00000600: 290f 4e72 0400 0000 7202 0000 00da 0566  ).Nr....r......f
+00000610: 6972 7374 da04 6c61 7374 2904 7205 0000  irst..last).r...
+00000620: 0072 2700 0000 722b 0000 0072 2c00 0000  .r'...r+...r,...
+00000630: 7206 0000 0072 0300 0000 2906 7207 0000  r....r....).r...
+00000640: 0072 0500 0000 722b 0000 0072 2c00 0000  .r....r+...r,...
+00000650: 7208 0000 0072 0900 0000 720a 0000 0072  r....r....r....r
+00000660: 0c00 0000 720d 0000 0072 0e00 0000 7211  ....r....r....r.
+00000670: 0000 0072 1200 0000 7213 0000 0072 1d00  ...r....r....r..
+00000680: 0000 7222 0000 0072 2200 0000 7223 0000  ..r"...r"...r#..
+00000690: 00da 2e74 6573 745f 6f72 6465 7265 645f  ...test_ordered_
+000006a0: 636f 6c6c 6563 7469 6f6e 5f62 7569 6c64  collection_build
+000006b0: 6572 5f77 6974 685f 6669 7374 5f6c 6173  er_with_fist_las
+000006c0: 741b 0000 0073 3000 0000 1401 2002 0207  t....s0..... ...
+000006d0: 0ef9 0207 04f9 0407 06f9 0207 02f9 0207  ................
+000006e0: 04f9 0207 02f9 0407 04f9 0207 02f9 0207  ................
+000006f0: 18f9 0207 02f9 0207 10f9 722d 0000 0029  ..........r-...)
+00000700: 0bda 0862 7569 6c74 696e 7372 1700 0000  ...builtinsr....
+00000710: da19 5f70 7974 6573 742e 6173 7365 7274  .._pytest.assert
+00000720: 696f 6e2e 7265 7772 6974 65da 0961 7373  ion.rewrite..ass
+00000730: 6572 7469 6f6e da07 7265 7772 6974 6572  ertion..rewriter
+00000740: 1500 0000 da00 7203 0000 0072 2400 0000  ......r....r$...
+00000750: 722a 0000 0072 2d00 0000 7222 0000 0072  r*...r-...r"...r
+00000760: 2200 0000 7222 0000 0072 2300 0000 da08  "...r"...r#.....
+00000770: 3c6d 6f64 756c 653e 0100 0000 7308 0000  <module>....s...
+00000780: 0026 0008 0308 0b0c 0c                   .&.......
```

### Comparing `bovine-0.1.0/bovine/activitystreams/activity_factory.py` & `bovine-0.1.1/bovine/activitystreams/activity_factory.py`

 * *Files 8% similar despite different names*

```diff
@@ -112,14 +112,24 @@
 
     def accept(self, obj, **kwargs):
         """Accept for object"""
         return Activity(
             type="Accept", actor=self.information["id"], object=obj, **kwargs
         )
 
+    def announce(self, obj, **kwargs):
+        """Announce for object"""
+        return Activity(
+            type="Announce",
+            actor=self.information["id"],
+            object=obj,
+            followers=self.information.get("followers", []),
+            **kwargs
+        )
+
     def follow(self, obj, **kwargs):
         """Follow for object"""
         return Activity(
             type="Follow",
             actor=self.information["id"],
             object=obj,
             to=set([obj]),
```

### Comparing `bovine-0.1.0/bovine/activitystreams/object_factory.py` & `bovine-0.1.1/bovine/activitystreams/object_factory.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.0/bovine/activitystreams/test_activity_factory.py` & `bovine-0.1.1/bovine/activitystreams/test_activity_factory.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.0/bovine/activitystreams/test_actor.py` & `bovine-0.1.1/bovine/activitystreams/test_actor.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.0/bovine/activitystreams/test_object_factory.py` & `bovine-0.1.1/bovine/activitystreams/test_object_factory.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.0/bovine/activitystreams/test_ordered_collection_builder.py` & `bovine-0.1.1/bovine/activitystreams/test_ordered_collection_builder.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,45 +1,35 @@
-from .ordered_collection_builder import OrderedCollectionBuilder
+from . import OrderedCollection
 
 
 def test_ordered_collection_builder():
-    result = OrderedCollectionBuilder("url").build()
+    result = OrderedCollection(id="url").build()
 
     assert result == {
         "@context": "https://www.w3.org/ns/activitystreams",
         "id": "url",
         "totalItems": 0,
         "type": "OrderedCollection",
     }
 
 
 def test_ordered_collection_builder_with_items():
-    result = (
-        OrderedCollectionBuilder("url")
-        .with_count(1)
-        .with_items([{"item": "1"}])
-        .build()
-    )
+    result = OrderedCollection(id="url", count=1, items=[{"item": "1"}]).build()
 
     assert result == {
         "@context": "https://www.w3.org/ns/activitystreams",
         "id": "url",
         "orderedItems": [{"item": "1"}],
         "totalItems": 1,
         "type": "OrderedCollection",
     }
 
 
 def test_ordered_collection_builder_with_fist_last():
-    result = (
-        OrderedCollectionBuilder("url")
-        .with_count(1)
-        .with_first_and_last("first", "last")
-        .build()
-    )
+    result = OrderedCollection(id="url", count=1, first="first", last="last").build()
 
     assert result == {
         "@context": "https://www.w3.org/ns/activitystreams",
         "id": "url",
         "first": "first",
         "last": "last",
         "totalItems": 1,
```

### Comparing `bovine-0.1.0/bovine/activitystreams/test_ordered_collection_page_builder.py` & `bovine-0.1.1/bovine/activitystreams/test_ordered_collection_page.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,26 @@
-from .ordered_collection_page_builder import OrderedCollectionPageBuilder
+from . import OrderedCollectionPage
 
 
-def test_ordered_collection_page_builder():
-    result = (
-        OrderedCollectionPageBuilder("url?page=1", "url").with_items(["id1"]).build()
-    )
+def test_ordered_collection_page():
+    result = OrderedCollectionPage(
+        id="url?page=1", part_of="url", items=["id1"]
+    ).build()
 
     assert result == {
         "@context": "https://www.w3.org/ns/activitystreams",
         "id": "url?page=1",
         "partOf": "url",
         "orderedItems": ["id1"],
         "type": "OrderedCollectionPage",
     }
 
-    result = (
-        OrderedCollectionPageBuilder("url?page=1", "url")
-        .with_items(["id1"])
-        .with_next("next_url")
-        .with_prev("prev_url")
-        .build()
-    )
+    result = OrderedCollectionPage(
+        id="url?page=1", part_of="url", items=["id1"], next="next_url", prev="prev_url"
+    ).build()
 
     assert result == {
         "@context": "https://www.w3.org/ns/activitystreams",
         "id": "url?page=1",
         "next": "next_url",
         "prev": "prev_url",
         "partOf": "url",
```

### Comparing `bovine-0.1.0/bovine/activitystreams/utils/__init__.py` & `bovine-0.1.1/bovine/activitystreams/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.0/bovine/activitystreams/utils/__pycache__/__init__.cpython-310.pyc` & `bovine-0.1.1/bovine/activitystreams/utils/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 13 15:55:57 2023 UTC, .py size: 2354 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0d26 3864 3209 0000  o........&8d2...
+00000000: 6f0d 0d0a 0000 0000 a4ea 3a64 3209 0000  o.........:d2...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 a800 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6403 6504 6404 6505 6604  m.Z...d.e.d.e.f.
 00000050: 6405 6406 8404 5a06 6403 6501 6504 6505  d.d...Z.d.e.e.e.
 00000060: 4200 1900 6404 6501 6505 1900 6604 6407  B...d.e.e...f.d.
 00000070: 6408 8404 5a07 6409 640a 8400 5a08 6403  d...Z.d.d...Z.d.
@@ -23,156 +23,156 @@
 00000160: 6f72 2074 6865 2061 6374 6f72 2069 6420  or the actor id 
 00000170: 6569 7468 6572 2066 726f 6d20 6174 7472  either from attr
 00000180: 6962 7574 6564 546f 206f 7220 6163 746f  ibutedTo or acto
 00000190: 72da 0c61 7474 7269 6275 7465 6454 6fda  r..attributedTo.
 000001a0: 0561 6374 6f72 5a0d 5f5f 4e4f 5f5f 4143  .actorZ.__NO__AC
 000001b0: 544f 525f 5f29 02da 0367 6574 da0d 6964  TOR__)...get..id
 000001c0: 5f66 6f72 5f6f 626a 6563 7429 0272 0400  _for_object).r..
-000001d0: 0000 7207 0000 00a9 0072 0a00 0000 fa59  ..r......r.....Y
+000001d0: 0000 7207 0000 00a9 0072 0a00 0000 fa5a  ..r......r.....Z
 000001e0: 2f77 6f6f 6470 6563 6b65 722f 7372 632f  /woodpecker/src/
-000001f0: 636f 6465 6265 7267 2e6f 7267 2f68 656c  codeberg.org/hel
-00000200: 6765 2f62 6f76 696e 652f 626f 7669 6e65  ge/bovine/bovine
-00000210: 2f62 6f76 696e 652f 6163 7469 7669 7479  /bovine/activity
-00000220: 7374 7265 616d 732f 7574 696c 732f 5f5f  streams/utils/__
-00000230: 696e 6974 5f5f 2e70 79da 1061 6374 6f72  init__.py..actor
-00000240: 5f66 6f72 5f6f 626a 6563 7405 0000 0073  _for_object....s
-00000250: 0e00 0000 0802 0c01 0a02 0801 0402 0401  ................
-00000260: 0402 720c 0000 0063 0100 0000 0000 0000  ..r....c........
-00000270: 0000 0000 0100 0000 0400 0000 4300 0000  ............C...
-00000280: 7326 0000 007c 0064 0175 0072 0664 0153  s&...|.d.u.r.d.S
-00000290: 0074 007c 0074 0183 0272 0d7c 0053 007c  .t.|.t...r.|.S.|
-000002a0: 00a0 0264 0264 01a1 0253 0029 037a 1e44  ...d.d...S.).z.D
-000002b0: 6574 6572 6d69 6e65 7320 7468 6520 6964  etermines the id
-000002c0: 206f 6620 616e 206f 626a 6563 744e da02   of an objectN..
-000002d0: 6964 2903 da0a 6973 696e 7374 616e 6365  id)...isinstance
-000002e0: da03 7374 7272 0800 0000 a901 7204 0000  ..strr......r...
-000002f0: 0072 0a00 0000 720a 0000 0072 0b00 0000  .r....r....r....
-00000300: 7209 0000 0013 0000 0073 0a00 0000 0803  r........s......
-00000310: 0401 0a01 0401 0c01 7209 0000 0063 0200  ........r....c..
-00000320: 0000 0000 0000 0000 0000 0300 0000 0400  ................
-00000330: 0000 4300 0000 7336 0000 007c 0064 0075  ..C...s6...|.d.u
-00000340: 0072 0774 0083 0053 007c 00a0 017c 0167  .r.t...S.|...|.g
-00000350: 00a1 027d 0274 027c 0274 0383 0272 1774  ...}.t.|.t...r.t
-00000360: 007c 0267 0183 0153 0074 007c 0283 0153  .|.g...S.t.|...S
-00000370: 00a9 014e 2904 da03 7365 7472 0800 0000  ...N)...setr....
-00000380: 720e 0000 0072 0f00 0000 2903 7204 0000  r....r....).r...
-00000390: 00da 036b 6579 da06 7265 7375 6c74 720a  ...key..resultr.
-000003a0: 0000 0072 0a00 0000 720b 0000 00da 1770  ...r....r......p
-000003b0: 726f 7065 7274 795f 666f 725f 6b65 795f  roperty_for_key_
-000003c0: 6173 5f73 6574 1d00 0000 730c 0000 0008  as_set....s.....
-000003d0: 0106 010c 010a 010a 0108 0172 1500 0000  ...........r....
-000003e0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-000003f0: 0004 0000 0003 0000 0073 1800 0000 7400  .........s....t.
-00000400: 6a01 8700 6601 6401 6402 8408 6403 4400  j...f.d.d...d.D.
-00000410: 8301 8e00 5300 2904 7a42 436f 6d62 696e  ....S.).zBCombin
-00000420: 6573 2074 6865 2072 6563 6970 6965 6e74  es the recipient
-00000430: 7320 6672 6f6d 2074 6f2c 2063 632c 2062  s from to, cc, b
-00000440: 746f 2c20 6263 632c 2061 7564 6965 6e63  to, bcc, audienc
-00000450: 6520 696e 746f 2061 2073 6574 6301 0000  e into a setc...
-00000460: 0000 0000 0000 0000 0002 0000 0005 0000  ................
-00000470: 0013 0000 0073 1600 0000 6700 7c00 5d07  .....s....g.|.].
-00000480: 7d01 7400 8800 7c01 8302 9102 7102 5300  }.t...|.....q.S.
-00000490: 720a 0000 0029 0172 1500 0000 2902 da02  r....).r....)...
-000004a0: 2e30 7213 0000 0072 1000 0000 720a 0000  .0r....r....r...
-000004b0: 0072 0b00 0000 da0a 3c6c 6973 7463 6f6d  .r......<listcom
-000004c0: 703e 2900 0000 7308 0000 0006 0002 0208  p>)...s.........
-000004d0: ff06 ff7a 2972 6563 6970 6965 6e74 735f  ...z)recipients_
-000004e0: 666f 725f 6f62 6a65 6374 2e3c 6c6f 6361  for_object.<loca
-000004f0: 6c73 3e2e 3c6c 6973 7463 6f6d 703e a905  ls>.<listcomp>..
-00000500: da02 746f da02 6363 5a03 6274 6f5a 0362  ..to..ccZ.btoZ.b
-00000510: 6363 5a08 6175 6469 656e 6365 2902 7212  ccZ.audience).r.
-00000520: 0000 00da 0575 6e69 6f6e 7210 0000 0072  .....unionr....r
-00000530: 0a00 0000 7210 0000 0072 0b00 0000 da15  ....r....r......
-00000540: 7265 6369 7069 656e 7473 5f66 6f72 5f6f  recipients_for_o
-00000550: 626a 6563 7426 0000 0073 0a00 0000 0402  bject&...s......
-00000560: 0a01 0202 04fe 04ff 721c 0000 0063 0100  ........r....c..
-00000570: 0000 0000 0000 0000 0000 0100 0000 0200  ................
-00000580: 0000 4300 0000 730e 0000 0064 0164 0284  ..C...s....d.d..
-00000590: 007c 0044 0083 0153 0029 034e 6301 0000  .|.D...S.).Nc...
-000005a0: 0000 0000 0000 0000 0002 0000 0004 0000  ................
-000005b0: 0053 0000 0073 1800 0000 6800 7c00 5d08  .S...s....h.|.].
-000005c0: 7d01 7c01 6400 7601 7202 7c01 9202 7102  }.|.d.v.r.|...q.
-000005d0: 5300 2901 a903 5a06 5075 626c 6963 7a09  S.)...Z.Publicz.
-000005e0: 6173 3a50 7562 6c69 637a 2c68 7474 7073  as:Publicz,https
-000005f0: 3a2f 2f77 7777 2e77 332e 6f72 672f 6e73  ://www.w3.org/ns
-00000600: 2f61 6374 6976 6974 7973 7472 6561 6d73  /activitystreams
-00000610: 2350 7562 6c69 6372 0a00 0000 a902 7216  #Publicr......r.
-00000620: 0000 00da 0178 720a 0000 0072 0a00 0000  .....xr....r....
-00000630: 720b 0000 00da 093c 7365 7463 6f6d 703e  r......<setcomp>
-00000640: 3100 0000 730e 0000 0006 0002 0202 0102  1...s...........
-00000650: 0104 ff02 fe06 027a 2072 656d 6f76 655f  .......z remove_
-00000660: 7075 626c 6963 2e3c 6c6f 6361 6c73 3e2e  public.<locals>.
-00000670: 3c73 6574 636f 6d70 3e72 0a00 0000 a901  <setcomp>r......
-00000680: 5a0a 7265 6369 7069 656e 7473 720a 0000  Z.recipientsr...
-00000690: 0072 0a00 0000 720b 0000 00da 0d72 656d  .r....r......rem
-000006a0: 6f76 655f 7075 626c 6963 3000 0000 7306  ove_public0...s.
-000006b0: 0000 0006 0102 0206 fe72 2200 0000 6301  .........r"...c.
-000006c0: 0000 0000 0000 0000 0000 0001 0000 0004  ................
-000006d0: 0000 0003 0000 0073 1e00 0000 7400 7c00  .......s....t.|.
-000006e0: 8301 8900 7401 8700 6601 6401 6402 8408  ....t...f.d.d...
-000006f0: 6403 4400 8301 8301 5300 2904 7a4c 4465  d.D.....S.).zLDe
-00000700: 7465 726d 696e 6573 2069 6620 7468 6520  termines if the 
-00000710: 6f62 6a65 6374 2073 686f 756c 6420 6265  object should be
-00000720: 2063 6f6e 7369 6465 7265 6420 7075 626c   considered publ
-00000730: 6963 2062 6173 6564 206f 6e20 6974 7320  ic based on its 
-00000740: 7265 6369 7069 656e 7473 6301 0000 0000  recipientsc.....
-00000750: 0000 0000 0000 0002 0000 0003 0000 0033  ...............3
-00000760: 0000 0073 1800 0000 8100 7c00 5d07 7d01  ...s......|.].}.
-00000770: 7c01 8800 7600 5600 0100 7102 6400 5300  |...v.V...q.d.S.
-00000780: 7211 0000 0072 0a00 0000 721e 0000 0072  r....r....r....r
-00000790: 2100 0000 720a 0000 0072 0b00 0000 da09  !...r....r......
-000007a0: 3c67 656e 6578 7072 3e3d 0000 0073 0a00  <genexpr>=...s..
-000007b0: 0000 0280 0400 0202 06ff 0aff 7a1c 6973  ............z.is
-000007c0: 5f70 7562 6c69 632e 3c6c 6f63 616c 733e  _public.<locals>
-000007d0: 2e3c 6765 6e65 7870 723e 721d 0000 0029  .<genexpr>r....)
-000007e0: 0272 1c00 0000 da03 616e 7972 1000 0000  .r......anyr....
-000007f0: 720a 0000 0072 2100 0000 720b 0000 00da  r....r!...r.....
-00000800: 0969 735f 7075 626c 6963 3900 0000 7308  .is_public9...s.
-00000810: 0000 0008 020c 0202 0208 fe72 2500 0000  ...........r%...
-00000820: 7207 0000 0063 0100 0000 0000 0000 0000  r....c..........
-00000830: 0000 0300 0000 0300 0000 4300 0000 7344  ..........C...sD
-00000840: 0000 0074 007c 0064 0119 0083 016a 017d  ...t.|.d.....j.}
-00000850: 0174 007c 0064 0119 0083 016a 02a0 0364  .t.|.d.....j...d
-00000860: 02a1 0164 0319 007d 0264 047c 0076 0072  ...d...}.d.|.v.r
-00000870: 1b7c 0064 0419 007d 027c 029b 0064 057c  .|.d...}.|...d.|
-00000880: 019b 009d 0353 0029 067a 4347 6976 656e  .....S.).zCGiven
-00000890: 2061 6e20 6163 746f 7220 6f62 6a65 6374   an actor object
-000008a0: 2c20 692e 652e 2061 2064 6963 742c 2064  , i.e. a dict, d
-000008b0: 6574 6572 6d69 6e65 7320 7468 6520 6665  etermines the fe
-000008c0: 6469 7665 7273 6520 6861 6e64 6c65 720d  diverse handler.
-000008d0: 0000 00fa 012f e9ff ffff ffda 1170 7265  ...../.......pre
-000008e0: 6665 7272 6564 5573 6572 6e61 6d65 fa01  ferredUsername..
-000008f0: 4029 0472 0300 0000 da06 6e65 746c 6f63  @).r......netloc
-00000900: da04 7061 7468 da05 7370 6c69 7429 0372  ..path..split).r
-00000910: 0700 0000 da04 686f 7374 da08 7573 6572  ......host..user
-00000920: 6e61 6d65 720a 0000 0072 0a00 0000 720b  namer....r....r.
-00000930: 0000 00da 1b66 6564 6976 6572 7365 5f68  .....fediverse_h
-00000940: 616e 646c 655f 6672 6f6d 5f61 6374 6f72  andle_from_actor
-00000950: 4300 0000 730a 0000 000e 0218 0108 0208  C...s...........
-00000960: 010e 0272 2f00 0000 da06 6f72 6967 696e  ...r/.....origin
-00000970: da0b 6465 7374 696e 6174 696f 6e63 0200  ..destinationc..
-00000980: 0000 0000 0000 0000 0000 0300 0000 0600  ................
-00000990: 0000 4300 0000 7332 0000 0064 0144 005d  ..C...s2...d.D.]
-000009a0: 147d 027c 027c 0076 0072 1674 0074 017c  .}.|.|.v.r.t.t.|
-000009b0: 007c 0283 0274 017c 017c 0283 0242 0083  .|...t.|.|...B..
-000009c0: 017c 017c 023c 0071 027c 0153 0029 027a  .|.|.<.q.|.S.).z
-000009d0: 4443 6f70 6965 7320 7468 6520 6175 6469  DCopies the audi
-000009e0: 656e 6365 2066 726f 6d20 7468 6520 6f72  ence from the or
-000009f0: 6967 696e 206f 626a 6563 7420 746f 2074  igin object to t
-00000a00: 6865 2064 6573 7469 6e61 7469 6f6e 206f  he destination o
-00000a10: 626a 6563 7472 1800 0000 2902 da04 6c69  bjectr....)...li
-00000a20: 7374 7215 0000 0029 0372 3000 0000 7231  str....).r0...r1
-00000a30: 0000 0072 1300 0000 720a 0000 0072 0a00  ...r....r....r..
-00000a40: 0000 720b 0000 00da 0e63 6f70 795f 746f  ..r......copy_to
-00000a50: 5f61 6e64 5f63 634e 0000 0073 1200 0000  _and_ccN...s....
-00000a60: 0803 0801 0201 0801 0801 02ff 08ff 0280  ................
-00000a70: 0405 7233 0000 004e 2910 da06 7479 7069  ..r3...N)...typi
-00000a80: 6e67 7202 0000 00da 0c75 726c 6c69 622e  ngr......urllib.
-00000a90: 7061 7273 6572 0300 0000 da04 6469 6374  parser......dict
-00000aa0: 720f 0000 0072 0c00 0000 7209 0000 0072  r....r....r....r
-00000ab0: 1500 0000 7212 0000 0072 1c00 0000 7222  ....r....r....r"
-00000ac0: 0000 00da 0462 6f6f 6c72 2500 0000 722f  .....boolr%...r/
-00000ad0: 0000 0072 3300 0000 720a 0000 0072 0a00  ...r3...r....r..
-00000ae0: 0000 720a 0000 0072 0b00 0000 da08 3c6d  ..r....r......<m
-00000af0: 6f64 756c 653e 0100 0000 7314 0000 000c  odule>....s.....
-00000b00: 000c 0112 031e 0e08 0a12 0908 0a12 0912  ................
-00000b10: 0a1a 0b                                  ...
+000001f0: 636f 6465 6265 7267 2e6f 7267 2f62 6f76  codeberg.org/bov
+00000200: 696e 652f 626f 7669 6e65 2f62 6f76 696e  ine/bovine/bovin
+00000210: 652f 626f 7669 6e65 2f61 6374 6976 6974  e/bovine/activit
+00000220: 7973 7472 6561 6d73 2f75 7469 6c73 2f5f  ystreams/utils/_
+00000230: 5f69 6e69 745f 5f2e 7079 da10 6163 746f  _init__.py..acto
+00000240: 725f 666f 725f 6f62 6a65 6374 0500 0000  r_for_object....
+00000250: 730e 0000 0008 020c 010a 0208 0104 0204  s...............
+00000260: 0104 0272 0c00 0000 6301 0000 0000 0000  ...r....c.......
+00000270: 0000 0000 0001 0000 0004 0000 0043 0000  .............C..
+00000280: 0073 2600 0000 7c00 6401 7500 7206 6401  .s&...|.d.u.r.d.
+00000290: 5300 7400 7c00 7401 8302 720d 7c00 5300  S.t.|.t...r.|.S.
+000002a0: 7c00 a002 6402 6401 a102 5300 2903 7a1e  |...d.d...S.).z.
+000002b0: 4465 7465 726d 696e 6573 2074 6865 2069  Determines the i
+000002c0: 6420 6f66 2061 6e20 6f62 6a65 6374 4eda  d of an objectN.
+000002d0: 0269 6429 03da 0a69 7369 6e73 7461 6e63  .id)...isinstanc
+000002e0: 65da 0373 7472 7208 0000 00a9 0172 0400  e..strr......r..
+000002f0: 0000 720a 0000 0072 0a00 0000 720b 0000  ..r....r....r...
+00000300: 0072 0900 0000 1300 0000 730a 0000 0008  .r........s.....
+00000310: 0304 010a 0104 010c 0172 0900 0000 6302  .........r....c.
+00000320: 0000 0000 0000 0000 0000 0003 0000 0004  ................
+00000330: 0000 0043 0000 0073 3600 0000 7c00 6400  ...C...s6...|.d.
+00000340: 7500 7207 7400 8300 5300 7c00 a001 7c01  u.r.t...S.|...|.
+00000350: 6700 a102 7d02 7402 7c02 7403 8302 7217  g...}.t.|.t...r.
+00000360: 7400 7c02 6701 8301 5300 7400 7c02 8301  t.|.g...S.t.|...
+00000370: 5300 a901 4e29 04da 0373 6574 7208 0000  S...N)...setr...
+00000380: 0072 0e00 0000 720f 0000 0029 0372 0400  .r....r....).r..
+00000390: 0000 da03 6b65 79da 0672 6573 756c 7472  ....key..resultr
+000003a0: 0a00 0000 720a 0000 0072 0b00 0000 da17  ....r....r......
+000003b0: 7072 6f70 6572 7479 5f66 6f72 5f6b 6579  property_for_key
+000003c0: 5f61 735f 7365 741d 0000 0073 0c00 0000  _as_set....s....
+000003d0: 0801 0601 0c01 0a01 0a01 0801 7215 0000  ............r...
+000003e0: 0063 0100 0000 0000 0000 0000 0000 0100  .c..............
+000003f0: 0000 0400 0000 0300 0000 7318 0000 0074  ..........s....t
+00000400: 006a 0187 0066 0164 0164 0284 0864 0344  .j...f.d.d...d.D
+00000410: 0083 018e 0053 0029 047a 4243 6f6d 6269  .....S.).zBCombi
+00000420: 6e65 7320 7468 6520 7265 6369 7069 656e  nes the recipien
+00000430: 7473 2066 726f 6d20 746f 2c20 6363 2c20  ts from to, cc, 
+00000440: 6274 6f2c 2062 6363 2c20 6175 6469 656e  bto, bcc, audien
+00000450: 6365 2069 6e74 6f20 6120 7365 7463 0100  ce into a setc..
+00000460: 0000 0000 0000 0000 0000 0200 0000 0500  ................
+00000470: 0000 1300 0000 7316 0000 0067 007c 005d  ......s....g.|.]
+00000480: 077d 0174 0088 007c 0183 0291 0271 0253  .}.t...|.....q.S
+00000490: 0072 0a00 0000 2901 7215 0000 0029 02da  .r....).r....)..
+000004a0: 022e 3072 1300 0000 7210 0000 0072 0a00  ..0r....r....r..
+000004b0: 0000 720b 0000 00da 0a3c 6c69 7374 636f  ..r......<listco
+000004c0: 6d70 3e29 0000 0073 0800 0000 0600 0202  mp>)...s........
+000004d0: 08ff 06ff 7a29 7265 6369 7069 656e 7473  ....z)recipients
+000004e0: 5f66 6f72 5f6f 626a 6563 742e 3c6c 6f63  _for_object.<loc
+000004f0: 616c 733e 2e3c 6c69 7374 636f 6d70 3ea9  als>.<listcomp>.
+00000500: 05da 0274 6fda 0263 635a 0362 746f 5a03  ...to..ccZ.btoZ.
+00000510: 6263 635a 0861 7564 6965 6e63 6529 0272  bccZ.audience).r
+00000520: 1200 0000 da05 756e 696f 6e72 1000 0000  ......unionr....
+00000530: 720a 0000 0072 1000 0000 720b 0000 00da  r....r....r.....
+00000540: 1572 6563 6970 6965 6e74 735f 666f 725f  .recipients_for_
+00000550: 6f62 6a65 6374 2600 0000 730a 0000 0004  object&...s.....
+00000560: 020a 0102 0204 fe04 ff72 1c00 0000 6301  .........r....c.
+00000570: 0000 0000 0000 0000 0000 0001 0000 0002  ................
+00000580: 0000 0043 0000 0073 0e00 0000 6401 6402  ...C...s....d.d.
+00000590: 8400 7c00 4400 8301 5300 2903 4e63 0100  ..|.D...S.).Nc..
+000005a0: 0000 0000 0000 0000 0000 0200 0000 0400  ................
+000005b0: 0000 5300 0000 7318 0000 0068 007c 005d  ..S...s....h.|.]
+000005c0: 087d 017c 0164 0076 0172 027c 0192 0271  .}.|.d.v.r.|...q
+000005d0: 0253 0029 01a9 035a 0650 7562 6c69 637a  .S.)...Z.Publicz
+000005e0: 0961 733a 5075 626c 6963 7a2c 6874 7470  .as:Publicz,http
+000005f0: 733a 2f2f 7777 772e 7733 2e6f 7267 2f6e  s://www.w3.org/n
+00000600: 732f 6163 7469 7669 7479 7374 7265 616d  s/activitystream
+00000610: 7323 5075 626c 6963 720a 0000 00a9 0272  s#Publicr......r
+00000620: 1600 0000 da01 7872 0a00 0000 720a 0000  ......xr....r...
+00000630: 0072 0b00 0000 da09 3c73 6574 636f 6d70  .r......<setcomp
+00000640: 3e31 0000 0073 0e00 0000 0600 0202 0201  >1...s..........
+00000650: 0201 04ff 02fe 0602 7a20 7265 6d6f 7665  ........z remove
+00000660: 5f70 7562 6c69 632e 3c6c 6f63 616c 733e  _public.<locals>
+00000670: 2e3c 7365 7463 6f6d 703e 720a 0000 00a9  .<setcomp>r.....
+00000680: 015a 0a72 6563 6970 6965 6e74 7372 0a00  .Z.recipientsr..
+00000690: 0000 720a 0000 0072 0b00 0000 da0d 7265  ..r....r......re
+000006a0: 6d6f 7665 5f70 7562 6c69 6330 0000 0073  move_public0...s
+000006b0: 0600 0000 0601 0202 06fe 7222 0000 0063  ..........r"...c
+000006c0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+000006d0: 0400 0000 0300 0000 731e 0000 0074 007c  ........s....t.|
+000006e0: 0083 0189 0074 0187 0066 0164 0164 0284  .....t...f.d.d..
+000006f0: 0864 0344 0083 0183 0153 0029 047a 4c44  .d.D.....S.).zLD
+00000700: 6574 6572 6d69 6e65 7320 6966 2074 6865  etermines if the
+00000710: 206f 626a 6563 7420 7368 6f75 6c64 2062   object should b
+00000720: 6520 636f 6e73 6964 6572 6564 2070 7562  e considered pub
+00000730: 6c69 6320 6261 7365 6420 6f6e 2069 7473  lic based on its
+00000740: 2072 6563 6970 6965 6e74 7363 0100 0000   recipientsc....
+00000750: 0000 0000 0000 0000 0200 0000 0300 0000  ................
+00000760: 3300 0000 7318 0000 0081 007c 005d 077d  3...s......|.].}
+00000770: 017c 0188 0076 0056 0001 0071 0264 0053  .|...v.V...q.d.S
+00000780: 0072 1100 0000 720a 0000 0072 1e00 0000  .r....r....r....
+00000790: 7221 0000 0072 0a00 0000 720b 0000 00da  r!...r....r.....
+000007a0: 093c 6765 6e65 7870 723e 3d00 0000 730a  .<genexpr>=...s.
+000007b0: 0000 0002 8004 0002 0206 ff0a ff7a 1c69  .............z.i
+000007c0: 735f 7075 626c 6963 2e3c 6c6f 6361 6c73  s_public.<locals
+000007d0: 3e2e 3c67 656e 6578 7072 3e72 1d00 0000  >.<genexpr>r....
+000007e0: 2902 721c 0000 00da 0361 6e79 7210 0000  ).r......anyr...
+000007f0: 0072 0a00 0000 7221 0000 0072 0b00 0000  .r....r!...r....
+00000800: da09 6973 5f70 7562 6c69 6339 0000 0073  ..is_public9...s
+00000810: 0800 0000 0802 0c02 0202 08fe 7225 0000  ............r%..
+00000820: 0072 0700 0000 6301 0000 0000 0000 0000  .r....c.........
+00000830: 0000 0003 0000 0003 0000 0043 0000 0073  ...........C...s
+00000840: 4400 0000 7400 7c00 6401 1900 8301 6a01  D...t.|.d.....j.
+00000850: 7d01 7400 7c00 6401 1900 8301 6a02 a003  }.t.|.d.....j...
+00000860: 6402 a101 6403 1900 7d02 6404 7c00 7600  d...d...}.d.|.v.
+00000870: 721b 7c00 6404 1900 7d02 7c02 9b00 6405  r.|.d...}.|...d.
+00000880: 7c01 9b00 9d03 5300 2906 7a43 4769 7665  |.....S.).zCGive
+00000890: 6e20 616e 2061 6374 6f72 206f 626a 6563  n an actor objec
+000008a0: 742c 2069 2e65 2e20 6120 6469 6374 2c20  t, i.e. a dict, 
+000008b0: 6465 7465 726d 696e 6573 2074 6865 2066  determines the f
+000008c0: 6564 6976 6572 7365 2068 616e 646c 6572  ediverse handler
+000008d0: 0d00 0000 fa01 2fe9 ffff ffff da11 7072  ....../.......pr
+000008e0: 6566 6572 7265 6455 7365 726e 616d 65fa  eferredUsername.
+000008f0: 0140 2904 7203 0000 00da 066e 6574 6c6f  .@).r......netlo
+00000900: 63da 0470 6174 68da 0573 706c 6974 2903  c..path..split).
+00000910: 7207 0000 00da 0468 6f73 74da 0875 7365  r......host..use
+00000920: 726e 616d 6572 0a00 0000 720a 0000 0072  rnamer....r....r
+00000930: 0b00 0000 da1b 6665 6469 7665 7273 655f  ......fediverse_
+00000940: 6861 6e64 6c65 5f66 726f 6d5f 6163 746f  handle_from_acto
+00000950: 7243 0000 0073 0a00 0000 0e02 1801 0802  rC...s..........
+00000960: 0801 0e02 722f 0000 00da 066f 7269 6769  ....r/.....origi
+00000970: 6eda 0b64 6573 7469 6e61 7469 6f6e 6302  n..destinationc.
+00000980: 0000 0000 0000 0000 0000 0003 0000 0006  ................
+00000990: 0000 0043 0000 0073 3200 0000 6401 4400  ...C...s2...d.D.
+000009a0: 5d14 7d02 7c02 7c00 7600 7216 7400 7401  ].}.|.|.v.r.t.t.
+000009b0: 7c00 7c02 8302 7401 7c01 7c02 8302 4200  |.|...t.|.|...B.
+000009c0: 8301 7c01 7c02 3c00 7102 7c01 5300 2902  ..|.|.<.q.|.S.).
+000009d0: 7a44 436f 7069 6573 2074 6865 2061 7564  zDCopies the aud
+000009e0: 6965 6e63 6520 6672 6f6d 2074 6865 206f  ience from the o
+000009f0: 7269 6769 6e20 6f62 6a65 6374 2074 6f20  rigin object to 
+00000a00: 7468 6520 6465 7374 696e 6174 696f 6e20  the destination 
+00000a10: 6f62 6a65 6374 7218 0000 0029 02da 046c  objectr....)...l
+00000a20: 6973 7472 1500 0000 2903 7230 0000 0072  istr....).r0...r
+00000a30: 3100 0000 7213 0000 0072 0a00 0000 720a  1...r....r....r.
+00000a40: 0000 0072 0b00 0000 da0e 636f 7079 5f74  ...r......copy_t
+00000a50: 6f5f 616e 645f 6363 4e00 0000 7312 0000  o_and_ccN...s...
+00000a60: 0008 0308 0102 0108 0108 0102 ff08 ff02  ................
+00000a70: 8004 0572 3300 0000 4e29 10da 0674 7970  ...r3...N)...typ
+00000a80: 696e 6772 0200 0000 da0c 7572 6c6c 6962  ingr......urllib
+00000a90: 2e70 6172 7365 7203 0000 00da 0464 6963  .parser......dic
+00000aa0: 7472 0f00 0000 720c 0000 0072 0900 0000  tr....r....r....
+00000ab0: 7215 0000 0072 1200 0000 721c 0000 0072  r....r....r....r
+00000ac0: 2200 0000 da04 626f 6f6c 7225 0000 0072  ".....boolr%...r
+00000ad0: 2f00 0000 7233 0000 0072 0a00 0000 720a  /...r3...r....r.
+00000ae0: 0000 0072 0a00 0000 720b 0000 00da 083c  ...r....r......<
+00000af0: 6d6f 6475 6c65 3e01 0000 0073 1400 0000  module>....s....
+00000b00: 0c00 0c01 1203 1e0e 080a 1209 080a 1209  ................
+00000b10: 120a 1a0b                                ....
```

### Comparing `bovine-0.1.0/bovine/activitystreams/utils/__pycache__/print.cpython-310.pyc` & `bovine-0.1.1/bovine/activitystreams/utils/__pycache__/print.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 13 15:55:57 2023 UTC, .py size: 787 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0d26 3864 1303 0000  o........&8d....
+00000000: 6f0d 0d0a 0000 0000 a4ea 3a64 1303 0000  o.........:d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 1c00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6402 6403 8400 5a01 6404  d.l.Z.d.d...Z.d.
 00000040: 6405 8400 5a02 6401 5300 2906 e900 0000  d...Z.d.S.).....
 00000050: 004e 6301 0000 0000 0000 0000 0000 0002  .Nc.............
 00000060: 0000 0007 0000 0043 0000 0073 6000 0000  .......C...s`...
 00000070: 6401 7c00 7600 7217 7400 6402 7c00 6401  d.|.v.r.t.d.|.d.
@@ -14,44 +14,44 @@
 000000d0: 2907 4eda 0474 7970 65fa 0654 7970 653a  ).N..type..Type:
 000000e0: 20da 0231 307a 062c 2049 643a 20da 0269   ..10z., Id: ..i
 000000f0: 64da 066f 626a 6563 7429 05da 0570 7269  d..object)...pri
 00000100: 6e74 da03 6765 74da 0a69 7369 6e73 7461  nt..get..isinsta
 00000110: 6e63 65da 0464 6963 74da 0c70 7269 6e74  nce..dict..print
 00000120: 5f6f 626a 6563 7429 025a 0861 6374 6976  _object).Z.activ
 00000130: 6974 79da 036f 626a a900 720d 0000 00fa  ity..obj..r.....
-00000140: 562f 776f 6f64 7065 636b 6572 2f73 7263  V/woodpecker/src
-00000150: 2f63 6f64 6562 6572 672e 6f72 672f 6865  /codeberg.org/he
-00000160: 6c67 652f 626f 7669 6e65 2f62 6f76 696e  lge/bovine/bovin
-00000170: 652f 626f 7669 6e65 2f61 6374 6976 6974  e/bovine/activit
-00000180: 7973 7472 6561 6d73 2f75 7469 6c73 2f70  ystreams/utils/p
-00000190: 7269 6e74 2e70 79da 0e70 7269 6e74 5f61  rint.py..print_a
-000001a0: 6374 6976 6974 7904 0000 0073 0e00 0000  ctivity....s....
-000001b0: 0801 2001 0601 1602 0801 0c02 08fd 720f  .. ...........r.
-000001c0: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
-000001d0: 0100 0000 0600 0000 4300 0000 73c0 0000  ........C...s...
-000001e0: 0064 017c 0076 0072 1074 0064 027c 0064  .d.|.v.r.t.d.|.d
-000001f0: 0119 009b 009d 0283 0101 0074 0083 0001  ...........t....
-00000200: 0064 037c 0076 0072 247c 0064 0319 0072  .d.|.v.r$|.d...r
-00000210: 2474 0064 047c 0064 0319 009b 009d 0283  $t.d.|.d........
-00000220: 0101 0074 0083 0001 0064 057c 0076 0072  ...t.....d.|.v.r
-00000230: 3f7c 0064 0519 0072 3f74 0064 0683 0101  ?|.d...r?t.d....
-00000240: 0074 0074 016a 027c 0064 0519 0067 0064  .t.t.j.|.d...g.d
-00000250: 0764 088d 0383 0101 0074 0083 0001 0064  .d.......t.....d
-00000260: 097c 0076 0072 5c7c 0064 0919 0072 5e74  .|.v.r\|.d...r^t
-00000270: 0064 0a83 0101 0074 0074 016a 027c 0064  .d.....t.t.j.|.d
-00000280: 0919 0067 0064 0764 088d 0383 0101 0074  ...g.d.d.......t
-00000290: 0083 0001 0064 0053 0064 0053 0064 0053  .....d.S.d.S.d.S
-000002a0: 0029 0b4e 7202 0000 0072 0300 0000 da04  .).Nr....r......
-000002b0: 6e61 6d65 7a06 4e61 6d65 3a20 da07 7375  namez.Name: ..su
-000002c0: 6d6d 6172 795a 0753 756d 6d61 7279 5429  mmaryZ.SummaryT)
-000002d0: 02da 0474 6167 73da 0573 7472 6970 da07  ...tags..strip..
-000002e0: 636f 6e74 656e 745a 0743 6f6e 7465 6e74  contentZ.Content
-000002f0: 2903 7207 0000 00da 0662 6c65 6163 68da  ).r......bleach.
-00000300: 0563 6c65 616e 2901 720c 0000 0072 0d00  .clean).r....r..
-00000310: 0000 720d 0000 0072 0e00 0000 720b 0000  ..r....r....r...
-00000320: 000f 0000 0073 1e00 0000 0801 1201 0601  .....s..........
-00000330: 1002 1201 0601 1001 0801 1801 0601 1002  ................
-00000340: 0801 1801 0a01 08fd 720b 0000 0029 0372  ........r....).r
-00000350: 1500 0000 720f 0000 0072 0b00 0000 720d  ....r....r....r.
-00000360: 0000 0072 0d00 0000 720d 0000 0072 0e00  ...r....r....r..
-00000370: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
-00000380: 7306 0000 0008 0008 030c 0b              s..........
+00000140: 572f 776f 6f64 7065 636b 6572 2f73 7263  W/woodpecker/src
+00000150: 2f63 6f64 6562 6572 672e 6f72 672f 626f  /codeberg.org/bo
+00000160: 7669 6e65 2f62 6f76 696e 652f 626f 7669  vine/bovine/bovi
+00000170: 6e65 2f62 6f76 696e 652f 6163 7469 7669  ne/bovine/activi
+00000180: 7479 7374 7265 616d 732f 7574 696c 732f  tystreams/utils/
+00000190: 7072 696e 742e 7079 da0e 7072 696e 745f  print.py..print_
+000001a0: 6163 7469 7669 7479 0400 0000 730e 0000  activity....s...
+000001b0: 0008 0120 0106 0116 0208 010c 0208 fd72  ... ...........r
+000001c0: 0f00 0000 6301 0000 0000 0000 0000 0000  ....c...........
+000001d0: 0001 0000 0006 0000 0043 0000 0073 c000  .........C...s..
+000001e0: 0000 6401 7c00 7600 7210 7400 6402 7c00  ..d.|.v.r.t.d.|.
+000001f0: 6401 1900 9b00 9d02 8301 0100 7400 8300  d...........t...
+00000200: 0100 6403 7c00 7600 7224 7c00 6403 1900  ..d.|.v.r$|.d...
+00000210: 7224 7400 6404 7c00 6403 1900 9b00 9d02  r$t.d.|.d.......
+00000220: 8301 0100 7400 8300 0100 6405 7c00 7600  ....t.....d.|.v.
+00000230: 723f 7c00 6405 1900 723f 7400 6406 8301  r?|.d...r?t.d...
+00000240: 0100 7400 7401 6a02 7c00 6405 1900 6700  ..t.t.j.|.d...g.
+00000250: 6407 6408 8d03 8301 0100 7400 8300 0100  d.d.......t.....
+00000260: 6409 7c00 7600 725c 7c00 6409 1900 725e  d.|.v.r\|.d...r^
+00000270: 7400 640a 8301 0100 7400 7401 6a02 7c00  t.d.....t.t.j.|.
+00000280: 6409 1900 6700 6407 6408 8d03 8301 0100  d...g.d.d.......
+00000290: 7400 8300 0100 6400 5300 6400 5300 6400  t.....d.S.d.S.d.
+000002a0: 5300 290b 4e72 0200 0000 7203 0000 00da  S.).Nr....r.....
+000002b0: 046e 616d 657a 064e 616d 653a 20da 0773  .namez.Name: ..s
+000002c0: 756d 6d61 7279 5a07 5375 6d6d 6172 7954  ummaryZ.SummaryT
+000002d0: 2902 da04 7461 6773 da05 7374 7269 70da  )...tags..strip.
+000002e0: 0763 6f6e 7465 6e74 5a07 436f 6e74 656e  .contentZ.Conten
+000002f0: 7429 0372 0700 0000 da06 626c 6561 6368  t).r......bleach
+00000300: da05 636c 6561 6e29 0172 0c00 0000 720d  ..clean).r....r.
+00000310: 0000 0072 0d00 0000 720e 0000 0072 0b00  ...r....r....r..
+00000320: 0000 0f00 0000 731e 0000 0008 0112 0106  ......s.........
+00000330: 0110 0212 0106 0110 0108 0118 0106 0110  ................
+00000340: 0208 0118 010a 0108 fd72 0b00 0000 2903  .........r....).
+00000350: 7215 0000 0072 0f00 0000 720b 0000 0072  r....r....r....r
+00000360: 0d00 0000 720d 0000 0072 0d00 0000 720e  ....r....r....r.
+00000370: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
+00000380: 0073 0600 0000 0800 0803 0c0b            .s..........
```

### Comparing `bovine-0.1.0/bovine/activitystreams/utils/__pycache__/test_utils.cpython-310-pytest-7.3.0.pyc` & `bovine-0.1.1/bovine/activitystreams/utils/__pycache__/test_utils.cpython-310-pytest-7.3.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 13 15:55:57 2023 UTC, .py size: 2266 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0d26 3864 da08 0000  o........&8d....
+00000000: 6f0d 0d0a 0000 0000 a4ea 3a64 da08 0000  o.........:d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 6200 0000 6400  .....@...sb...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6402 6c06 6d07  ..m.Z...d.d.l.m.
 00000050: 5a07 0100 6403 6404 6c08 6d09 5a09 6d0a  Z...d.d.l.m.Z.m.
 00000060: 5a0a 6d0b 5a0b 6d0c 5a0c 0100 6405 6406  Z.m.Z.m.Z...d.d.
 00000070: 8400 5a0d 6407 6408 8400 5a0e 6409 640a  ..Z.d.d...Z.d.d.
@@ -30,19 +30,19 @@
 000001d0: 740d 7407 a00e 7c05 a101 8301 8201 6400  t.t...|.......d.
 000001e0: 0400 7d03 7d02 6400 5300 290f 4eda 044e  ..}.}.d.S.).N..N
 000001f0: 6f74 65da 0761 6363 6f75 6e74 fa11 6163  ote..account..ac
 00000200: 636f 756e 742f 666f 6c6c 6f77 6572 73a9  count/followers.
 00000210: 03da 0474 7970 65da 0d61 7474 7269 6275  ...type..attribu
 00000220: 7465 645f 746f da09 666f 6c6c 6f77 6572  ted_to..follower
 00000230: 73da 0263 63da 0274 6fda 0473 616d 653e  s..cc..to..same>
-00000240: 0500 0000 7210 0000 0072 1100 0000 720f  ....r....r....r.
+00000240: 0500 0000 7211 0000 0072 0f00 0000 720a  ....r....r....r.
 00000250: 0000 007a 2c68 7474 7073 3a2f 2f77 7777  ...z,https://www
 00000260: 2e77 332e 6f72 672f 6e73 2f61 6374 6976  .w3.org/ns/activ
 00000270: 6974 7973 7472 6561 6d73 2350 7562 6c69  itystreams#Publi
-00000280: 6372 0a00 0000 a901 fa02 3d3d 2901 7a12  cr........==).z.
+00000280: 6372 1000 0000 a901 fa02 3d3d 2901 7a12  cr........==).z.
 00000290: 2528 7079 3029 7320 3d3d 2025 2870 7933  %(py0)s == %(py3
 000002a0: 2973 da0a 7265 6369 7069 656e 7473 2902  )s..recipients).
 000002b0: da03 7079 30da 0370 7933 7a0e 6173 7365  ..py0..py3z.asse
 000002c0: 7274 2025 2870 7935 2973 da03 7079 3529  rt %(py5)s..py5)
 000002d0: 0f72 0200 0000 da09 6173 5f70 7562 6c69  .r......as_publi
 000002e0: 6372 0f00 0000 da03 6164 6472 1000 0000  cr......addr....
 000002f0: da05 6275 696c 6472 0700 0000 da0a 4070  ..buildr......@p
@@ -54,245 +54,245 @@
 00000350: 6665 7265 7072 da0e 4173 7365 7274 696f  ferepr..Assertio
 00000360: 6e45 7272 6f72 da13 5f66 6f72 6d61 745f  nError.._format_
 00000370: 6578 706c 616e 6174 696f 6e29 06da 046e  explanation)...n
 00000380: 6f74 6572 1400 0000 da0b 4070 795f 6173  oter......@py_as
 00000390: 7365 7274 32da 0b40 7079 5f61 7373 6572  sert2..@py_asser
 000003a0: 7431 da0b 4070 795f 666f 726d 6174 34da  t1..@py_format4.
 000003b0: 0b40 7079 5f66 6f72 6d61 7436 a900 7228  .@py_format6..r(
-000003c0: 0000 00fa 5b2f 776f 6f64 7065 636b 6572  ....[/woodpecker
+000003c0: 0000 00fa 5c2f 776f 6f64 7065 636b 6572  ....\/woodpecker
 000003d0: 2f73 7263 2f63 6f64 6562 6572 672e 6f72  /src/codeberg.or
-000003e0: 672f 6865 6c67 652f 626f 7669 6e65 2f62  g/helge/bovine/b
-000003f0: 6f76 696e 652f 626f 7669 6e65 2f61 6374  ovine/bovine/act
-00000400: 6976 6974 7973 7472 6561 6d73 2f75 7469  ivitystreams/uti
-00000410: 6c73 2f74 6573 745f 7574 696c 732e 7079  ls/test_utils.py
-00000420: da13 7465 7374 5f67 6574 5f72 6563 6970  ..test_get_recip
-00000430: 6965 6e74 730b 0000 0073 4400 0000 0201  ients....sD.....
-00000440: 0601 04ff 0402 02fe 0c03 0c01 0c01 0c01  ................
-00000450: 0801 0802 1602 0206 0efa 0206 04fa 0406  ................
-00000460: 06fa 0206 02fa 0206 04fa 0206 02fa 0406  ................
-00000470: 04fa 0206 02fa 0206 18fa 0206 02fa 0206  ................
-00000480: 10fa 722a 0000 0063 0000 0000 0000 0000  ..r*...c........
-00000490: 0000 0000 0500 0000 0600 0000 4300 0000  ............C...
-000004a0: 73e8 0200 0074 0064 0164 0264 0364 048d  s....t.d.d.d.d..
-000004b0: 03a0 01a1 00a0 02a1 007d 0074 037c 0083  .........}.t.|..
-000004c0: 017d 017c 0173 4364 0564 0674 04a0 05a1  .}.|.sCd.d.t....
-000004d0: 0076 0073 1d74 06a0 0774 03a1 0172 2274  .v.s.t...t...r"t
-000004e0: 06a0 0874 03a1 016e 0164 0664 0774 04a0  ...t...n.d.d.t..
-000004f0: 05a1 0076 0073 2e74 06a0 077c 00a1 0172  ...v.s.t...|...r
-00000500: 3374 06a0 087c 00a1 016e 0164 0774 06a0  3t...|...n.d.t..
-00000510: 087c 01a1 0164 089c 0316 007d 0274 0974  .|...d.....}.t.t
-00000520: 06a0 0a7c 02a1 0183 0182 0164 007d 0174  ...|.......d.}.t
-00000530: 0064 0164 0264 0364 048d 03a0 02a1 007d  .d.d.d.d.......}
-00000540: 0074 037c 0083 017d 017c 010c 007d 037c  .t.|...}.|...}.|
-00000550: 0373 8964 0964 0674 04a0 05a1 0076 0073  .s.d.d.t.....v.s
-00000560: 6374 06a0 0774 03a1 0172 6874 06a0 0874  ct...t...rht...t
-00000570: 03a1 016e 0164 0664 0774 04a0 05a1 0076  ...n.d.d.t.....v
-00000580: 0073 7474 06a0 077c 00a1 0172 7974 06a0  .stt...|...ryt..
-00000590: 087c 00a1 016e 0164 0774 06a0 087c 01a1  .|...n.d.t...|..
-000005a0: 0164 089c 0316 007d 0474 0974 06a0 0a7c  .d.....}.t.t...|
-000005b0: 04a1 0183 0182 0164 0004 007d 017d 0374  .......d...}.}.t
-000005c0: 0064 0164 0264 0364 048d 037d 007c 006a  .d.d.d.d...}.|.j
-000005d0: 0ba0 0c64 0aa1 0101 007c 00a0 02a1 007d  ...d.....|.....}
-000005e0: 0074 037c 0083 017d 017c 010c 007d 037c  .t.|...}.|...}.|
-000005f0: 0373 d964 0964 0674 04a0 05a1 0076 0073  .s.d.d.t.....v.s
-00000600: b374 06a0 0774 03a1 0172 b874 06a0 0874  .t...t...r.t...t
-00000610: 03a1 016e 0164 0664 0774 04a0 05a1 0076  ...n.d.d.t.....v
-00000620: 0073 c474 06a0 077c 00a1 0172 c974 06a0  .s.t...|...r.t..
-00000630: 087c 00a1 016e 0164 0774 06a0 087c 01a1  .|...n.d.t...|..
-00000640: 0164 089c 0316 007d 0474 0974 06a0 0a7c  .d.....}.t.t...|
-00000650: 04a1 0183 0182 0164 0004 007d 017d 0374  .......d...}.}.t
-00000660: 0064 0164 0264 0364 048d 03a0 0da1 00a0  .d.d.d.d........
-00000670: 02a1 007d 0074 037c 0083 017d 017c 0190  ...}.t.|...}.|..
-00000680: 0173 2464 0564 0674 04a0 05a1 0076 0073  .s$d.d.t.....v.s
-00000690: fc74 06a0 0774 03a1 0190 0172 0174 06a0  .t...t.....r.t..
-000006a0: 0874 03a1 016e 0164 0664 0774 04a0 05a1  .t...n.d.d.t....
-000006b0: 0076 0090 0173 0f74 06a0 077c 00a1 0190  .v...s.t...|....
-000006c0: 0172 1474 06a0 087c 00a1 016e 0164 0774  .r.t...|...n.d.t
-000006d0: 06a0 087c 01a1 0164 089c 0316 007d 0274  ...|...d.....}.t
-000006e0: 0974 06a0 0a7c 02a1 0183 0182 0164 007d  .t...|.......d.}
-000006f0: 0174 0064 0164 0264 0364 048d 03a0 02a1  .t.d.d.d.d......
-00000700: 007d 0064 0b7c 0064 0c3c 0074 037c 0083  .}.d.|.d.<.t.|..
-00000710: 017d 017c 0190 0173 7064 0564 0674 04a0  .}.|...spd.d.t..
-00000720: 05a1 0076 0090 0173 4874 06a0 0774 03a1  ...v...sHt...t..
-00000730: 0190 0172 4d74 06a0 0874 03a1 016e 0164  ...rMt...t...n.d
-00000740: 0664 0774 04a0 05a1 0076 0090 0173 5b74  .d.t.....v...s[t
-00000750: 06a0 077c 00a1 0190 0172 6074 06a0 087c  ...|.....r`t...|
-00000760: 00a1 016e 0164 0774 06a0 087c 01a1 0164  ...n.d.t...|...d
-00000770: 089c 0316 007d 0274 0974 06a0 0a7c 02a1  .....}.t.t...|..
-00000780: 0183 0182 0164 007d 0164 0053 0029 0d4e  .....d.}.d.S.).N
-00000790: 7208 0000 0072 0900 0000 720a 0000 0072  r....r....r....r
-000007a0: 0b00 0000 7a2c 6173 7365 7274 2025 2870  ....z,assert %(p
-000007b0: 7933 2973 0a7b 2528 7079 3329 7320 3d20  y3)s.{%(py3)s = 
-000007c0: 2528 7079 3029 7328 2528 7079 3129 7329  %(py0)s(%(py1)s)
-000007d0: 0a7d 7206 0000 0072 2300 0000 2903 7215  .}r....r#...).r.
-000007e0: 0000 00da 0370 7931 7216 0000 007a 3061  .....py1r....z0a
-000007f0: 7373 6572 7420 6e6f 7420 2528 7079 3329  ssert not %(py3)
-00000800: 730a 7b25 2870 7933 2973 203d 2025 2870  s.{%(py3)s = %(p
-00000810: 7930 2973 2825 2870 7931 2973 290a 7d5a  y0)s(%(py1)s).}Z
-00000820: 0773 6f6d 656f 6e65 7a09 6173 3a50 7562  .someonez.as:Pub
-00000830: 6c69 6372 1000 0000 290e 7202 0000 0072  licr....).r....r
-00000840: 1800 0000 721a 0000 0072 0600 0000 721d  ....r....r....r.
-00000850: 0000 0072 1e00 0000 721b 0000 0072 1f00  ...r....r....r..
-00000860: 0000 7220 0000 0072 2100 0000 7222 0000  ..r ...r!...r"..
-00000870: 0072 0f00 0000 7219 0000 00da 0b61 735f  .r....r......as_
-00000880: 756e 6c69 7374 6564 2905 7223 0000 0072  unlisted).r#...r
-00000890: 2400 0000 7226 0000 00da 0b40 7079 5f61  $...r&.....@py_a
-000008a0: 7373 6572 7434 da0b 4070 795f 666f 726d  ssert4..@py_form
-000008b0: 6174 3572 2800 0000 7228 0000 0072 2900  at5r(...r(...r).
-000008c0: 0000 da0e 7465 7374 5f69 735f 7075 626c  ....test_is_publ
-000008d0: 6963 2000 0000 7336 0000 000c 0204 0104  ic ...s6........
-000008e0: 0102 fd74 0502 0206 0104 ff04 0202 fe7e  ...t...........~
-000008f0: 030e 020c 0108 017e 010c 0304 0104 0102  .......~........
-00000900: fd7c 0502 0206 0104 ff04 0202 fe08 0382  .|..............
-00000910: 0172 2f00 0000 6300 0000 0000 0000 0000  .r/...c.........
-00000920: 0000 0006 0000 0007 0000 0043 0000 0073  ...........C...s
-00000930: 8004 0000 6900 7d00 7400 7c00 8301 7d01  ....i.}.t.|...}.
-00000940: 6401 7d02 7c01 7c02 6b02 7d03 7c03 7346  d.}.|.|.k.}.|.sF
-00000950: 7401 a002 6402 7c03 6601 6403 7c01 7c02  t...d.|.f.d.|.|.
-00000960: 6602 a104 6404 7403 a004 a100 7600 7323  f...d.t.....v.s#
-00000970: 7401 a005 7400 a101 7228 7401 a006 7400  t...t...r(t...t.
-00000980: a101 6e01 6404 7401 a006 7c00 a101 7401  ..n.d.t...|...t.
-00000990: a006 7c01 a101 7401 a006 7c02 a101 6405  ..|...t...|...d.
-000009a0: 9c04 1600 7d04 6406 6407 7c04 6901 1600  ....}.d.d.|.i...
-000009b0: 7d05 7407 7401 a008 7c05 a101 8301 8201  }.t.t...|.......
-000009c0: 6400 0400 7d00 0400 7d01 0400 7d03 7d02  d...}...}...}.}.
-000009d0: 6408 6409 6901 7d00 7400 7c00 8301 7d01  d.d.i.}.t.|...}.
-000009e0: 6409 7d02 7c01 7c02 6b02 7d03 7c03 7396  d.}.|.|.k.}.|.s.
-000009f0: 7401 a002 6402 7c03 6601 6403 7c01 7c02  t...d.|.f.d.|.|.
-00000a00: 6602 a104 6404 7403 a004 a100 7600 7373  f...d.t.....v.ss
-00000a10: 7401 a005 7400 a101 7278 7401 a006 7400  t...t...rxt...t.
-00000a20: a101 6e01 6404 7401 a006 7c00 a101 7401  ..n.d.t...|...t.
-00000a30: a006 7c01 a101 7401 a006 7c02 a101 6405  ..|...t...|...d.
-00000a40: 9c04 1600 7d04 6406 6407 7c04 6901 1600  ....}.d.d.|.i...
-00000a50: 7d05 7407 7401 a008 7c05 a101 8301 8201  }.t.t...|.......
-00000a60: 6400 0400 7d00 0400 7d01 0400 7d03 7d02  d...}...}...}.}.
-00000a70: 6408 640a 6409 6901 6901 7d00 7400 7c00  d.d.d.i.i.}.t.|.
-00000a80: 8301 7d01 6409 7d02 7c01 7c02 6b02 7d03  ..}.d.}.|.|.k.}.
-00000a90: 7c03 73e8 7401 a002 6402 7c03 6601 6403  |.s.t...d.|.f.d.
-00000aa0: 7c01 7c02 6602 a104 6404 7403 a004 a100  |.|.f...d.t.....
-00000ab0: 7600 73c5 7401 a005 7400 a101 72ca 7401  v.s.t...t...r.t.
-00000ac0: a006 7400 a101 6e01 6404 7401 a006 7c00  ..t...n.d.t...|.
-00000ad0: a101 7401 a006 7c01 a101 7401 a006 7c02  ..t...|...t...|.
-00000ae0: a101 6405 9c04 1600 7d04 6406 6407 7c04  ..d.....}.d.d.|.
-00000af0: 6901 1600 7d05 7407 7401 a008 7c05 a101  i...}.t.t...|...
-00000b00: 8301 8201 6400 0400 7d00 0400 7d01 0400  ....d...}...}...
-00000b10: 7d03 7d02 6408 6900 6901 7d00 7400 7c00  }.}.d.i.i.}.t.|.
-00000b20: 8301 7d01 6401 7d02 7c01 7c02 6b02 7d03  ..}.d.}.|.|.k.}.
-00000b30: 7c03 9001 733b 7401 a002 6402 7c03 6601  |...s;t...d.|.f.
-00000b40: 6403 7c01 7c02 6602 a104 6404 7403 a004  d.|.|.f...d.t...
-00000b50: a100 7600 9001 7318 7401 a005 7400 a101  ..v...s.t...t...
-00000b60: 9001 721d 7401 a006 7400 a101 6e01 6404  ..r.t...t...n.d.
-00000b70: 7401 a006 7c00 a101 7401 a006 7c01 a101  t...|...t...|...
-00000b80: 7401 a006 7c02 a101 6405 9c04 1600 7d04  t...|...d.....}.
-00000b90: 6406 6407 7c04 6901 1600 7d05 7407 7401  d.d.|.i...}.t.t.
-00000ba0: a008 7c05 a101 8301 8201 6400 0400 7d00  ..|.......d...}.
-00000bb0: 0400 7d01 0400 7d03 7d02 640b 6409 6901  ..}...}.}.d.d.i.
-00000bc0: 7d00 7400 7c00 8301 7d01 6409 7d02 7c01  }.t.|...}.d.}.|.
-00000bd0: 7c02 6b02 7d03 7c03 9001 738e 7401 a002  |.k.}.|...s.t...
-00000be0: 6402 7c03 6601 6403 7c01 7c02 6602 a104  d.|.f.d.|.|.f...
-00000bf0: 6404 7403 a004 a100 7600 9001 736b 7401  d.t.....v...skt.
-00000c00: a005 7400 a101 9001 7270 7401 a006 7400  ..t.....rpt...t.
-00000c10: a101 6e01 6404 7401 a006 7c00 a101 7401  ..n.d.t...|...t.
-00000c20: a006 7c01 a101 7401 a006 7c02 a101 6405  ..|...t...|...d.
-00000c30: 9c04 1600 7d04 6406 6407 7c04 6901 1600  ....}.d.d.|.i...
-00000c40: 7d05 7407 7401 a008 7c05 a101 8301 8201  }.t.t...|.......
-00000c50: 6400 0400 7d00 0400 7d01 0400 7d03 7d02  d...}...}...}.}.
-00000c60: 640b 640a 6409 6901 6901 7d00 7400 7c00  d.d.d.i.i.}.t.|.
-00000c70: 8301 7d01 6409 7d02 7c01 7c02 6b02 7d03  ..}.d.}.|.|.k.}.
-00000c80: 7c03 9001 73e3 7401 a002 6402 7c03 6601  |...s.t...d.|.f.
-00000c90: 6403 7c01 7c02 6602 a104 6404 7403 a004  d.|.|.f...d.t...
-00000ca0: a100 7600 9001 73c0 7401 a005 7400 a101  ..v...s.t...t...
-00000cb0: 9001 72c5 7401 a006 7400 a101 6e01 6404  ..r.t...t...n.d.
-00000cc0: 7401 a006 7c00 a101 7401 a006 7c01 a101  t...|...t...|...
-00000cd0: 7401 a006 7c02 a101 6405 9c04 1600 7d04  t...|...d.....}.
-00000ce0: 6406 6407 7c04 6901 1600 7d05 7407 7401  d.d.|.i...}.t.t.
-00000cf0: a008 7c05 a101 8301 8201 6400 0400 7d00  ..|.......d...}.
-00000d00: 0400 7d01 0400 7d03 7d02 640b 6900 6901  ..}...}.}.d.i.i.
-00000d10: 7d00 7400 7c00 8301 7d01 6401 7d02 7c01  }.t.|...}.d.}.|.
-00000d20: 7c02 6b02 7d03 7c03 9002 7336 7401 a002  |.k.}.|...s6t...
-00000d30: 6402 7c03 6601 6403 7c01 7c02 6602 a104  d.|.f.d.|.|.f...
-00000d40: 6404 7403 a004 a100 7600 9002 7313 7401  d.t.....v...s.t.
-00000d50: a005 7400 a101 9002 7218 7401 a006 7400  ..t.....r.t...t.
-00000d60: a101 6e01 6404 7401 a006 7c00 a101 7401  ..n.d.t...|...t.
-00000d70: a006 7c01 a101 7401 a006 7c02 a101 6405  ..|...t...|...d.
-00000d80: 9c04 1600 7d04 6406 6407 7c04 6901 1600  ....}.d.d.|.i...
-00000d90: 7d05 7407 7401 a008 7c05 a101 8301 8201  }.t.t...|.......
-00000da0: 6400 0400 7d00 0400 7d01 0400 7d03 7d02  d...}...}...}.}.
-00000db0: 6400 5300 290c 4eda 0d5f 5f4e 4f5f 5f41  d.S.).N..__NO__A
-00000dc0: 4354 4f52 5f5f 7212 0000 00a9 017a 3025  CTOR__r......z0%
-00000dd0: 2870 7934 2973 0a7b 2528 7079 3429 7320  (py4)s.{%(py4)s 
-00000de0: 3d20 2528 7079 3029 7328 2528 7079 3229  = %(py0)s(%(py2)
-00000df0: 7329 0a7d 203d 3d20 2528 7079 3729 7372  s).} == %(py7)sr
-00000e00: 0400 0000 a904 7215 0000 00da 0370 7932  ......r......py2
-00000e10: da03 7079 34da 0370 7937 fa0e 6173 7365  ..py4..py7..asse
-00000e20: 7274 2025 2870 7939 2973 da03 7079 39da  rt %(py9)s..py9.
-00000e30: 0561 6374 6f72 5a05 616c 6963 65da 0269  .actorZ.alice..i
-00000e40: 64da 0c61 7474 7269 6275 7465 6454 6f29  d..attributedTo)
-00000e50: 0972 0400 0000 721b 0000 0072 1c00 0000  .r....r....r....
-00000e60: 721d 0000 0072 1e00 0000 721f 0000 0072  r....r....r....r
-00000e70: 2000 0000 7221 0000 0072 2200 0000 a906   ...r!...r".....
-00000e80: 7225 0000 00da 0b40 7079 5f61 7373 6572  r%.....@py_asser
-00000e90: 7433 da0b 4070 795f 6173 7365 7274 365a  t3..@py_assert6Z
-00000ea0: 0b40 7079 5f61 7373 6572 7435 da0b 4070  .@py_assert5..@p
-00000eb0: 795f 666f 726d 6174 385a 0c40 7079 5f66  y_format8Z.@py_f
-00000ec0: 6f72 6d61 7431 3072 2800 0000 7228 0000  ormat10r(...r(..
-00000ed0: 0072 2900 0000 da15 7465 7374 5f61 6374  .r).....test_act
-00000ee0: 6f72 5f66 6f72 5f6f 626a 6563 7440 0000  or_for_object@..
-00000ef0: 0073 0e00 0000 9c01 a001 a401 a601 a601  .s..............
-00000f00: aa01 aa01 723f 0000 0063 0000 0000 0000  ....r?...c......
-00000f10: 0000 0000 0000 0600 0000 0700 0000 4300  ..............C.
-00000f20: 0000 7346 0100 0064 0164 0269 017d 0074  ..sF...d.d.i.}.t
-00000f30: 007c 0083 017d 0164 037d 027c 017c 026b  .|...}.d.}.|.|.k
-00000f40: 027d 037c 0373 4874 01a0 0264 047c 0366  .}.|.sHt...d.|.f
-00000f50: 0164 057c 017c 0266 02a1 0464 0674 03a0  .d.|.|.f...d.t..
-00000f60: 04a1 0076 0073 2574 01a0 0574 00a1 0172  ...v.s%t...t...r
-00000f70: 2a74 01a0 0674 00a1 016e 0164 0674 01a0  *t...t...n.d.t..
-00000f80: 067c 00a1 0174 01a0 067c 01a1 0174 01a0  .|...t...|...t..
-00000f90: 067c 02a1 0164 079c 0416 007d 0464 0864  .|...d.....}.d.d
-00000fa0: 097c 0469 0116 007d 0574 0774 01a0 087c  .|.i...}.t.t...|
-00000fb0: 05a1 0183 0182 0164 0004 007d 0004 007d  .......d...}...}
-00000fc0: 0104 007d 037d 0264 0264 0a64 0b9c 027d  ...}.}.d.d.d...}
-00000fd0: 0074 007c 0083 017d 0164 0c7d 027c 017c  .t.|...}.d.}.|.|
-00000fe0: 026b 027d 037c 0373 9974 01a0 0264 047c  .k.}.|.s.t...d.|
-00000ff0: 0366 0164 057c 017c 0266 02a1 0464 0674  .f.d.|.|.f...d.t
-00001000: 03a0 04a1 0076 0073 7674 01a0 0574 00a1  .....v.svt...t..
-00001010: 0172 7b74 01a0 0674 00a1 016e 0164 0674  .r{t...t...n.d.t
-00001020: 01a0 067c 00a1 0174 01a0 067c 01a1 0174  ...|...t...|...t
-00001030: 01a0 067c 02a1 0164 079c 0416 007d 0464  ...|...d.....}.d
-00001040: 0864 097c 0469 0116 007d 0574 0774 01a0  .d.|.i...}.t.t..
-00001050: 087c 05a1 0183 0182 0164 0004 007d 0004  .|.......d...}..
-00001060: 007d 0104 007d 037d 0264 0053 0029 0d4e  .}...}.}.d.S.).N
-00001070: 7239 0000 007a 1868 7474 7073 3a2f 2f61  r9...z.https://a
-00001080: 6265 6c2f 6163 746f 722f 616c 6963 657a  bel/actor/alicez
-00001090: 0a61 6c69 6365 4061 6265 6c72 1200 0000  .alice@abelr....
-000010a0: 7231 0000 0072 0500 0000 7232 0000 0072  r1...r....r2...r
-000010b0: 3600 0000 7237 0000 00da 0661 6c79 7373  6...r7.....alyss
-000010c0: 6129 0272 3900 0000 da11 7072 6566 6572  a).r9.....prefer
-000010d0: 7265 6455 7365 726e 616d 657a 0b61 6c79  redUsernamez.aly
-000010e0: 7373 6140 6162 656c 2909 7205 0000 0072  ssa@abel).r....r
-000010f0: 1b00 0000 721c 0000 0072 1d00 0000 721e  ....r....r....r.
-00001100: 0000 0072 1f00 0000 7220 0000 0072 2100  ...r....r ...r!.
-00001110: 0000 7222 0000 0072 3b00 0000 7228 0000  ..r"...r;...r(..
-00001120: 0072 2800 0000 7229 0000 00da 1574 6573  .r(...r).....tes
-00001130: 745f 6665 6469 7665 7273 655f 6861 6e64  t_fediverse_hand
-00001140: 6c65 4a00 0000 737c 0000 0022 0102 020e  leJ...s|..."....
-00001150: fe02 0204 fe04 0206 fe02 0202 fe02 0204  ................
-00001160: fe02 0202 fe04 0204 fe02 0202 fe02 0202  ................
-00001170: fe02 0202 fe02 0202 fe02 0202 fe02 0218  ................
-00001180: fe02 0202 fe02 0214 fe24 0302 050e fb02  .........$......
-00001190: 0504 fb04 0506 fb02 0502 fb02 0504 fb02  ................
-000011a0: 0502 fb04 0504 fb02 0502 fb02 0502 fb02  ................
-000011b0: 0502 fb02 0502 fb02 0502 fb02 0518 fb02  ................
-000011c0: 0502 fb02 0518 fb72 4200 0000 2911 da08  .......rB...)...
-000011d0: 6275 696c 7469 6e73 721d 0000 00da 195f  builtinsr......_
-000011e0: 7079 7465 7374 2e61 7373 6572 7469 6f6e  pytest.assertion
-000011f0: 2e72 6577 7269 7465 da09 6173 7365 7274  .rewrite..assert
-00001200: 696f 6eda 0772 6577 7269 7465 721b 0000  ion..rewriter...
-00001210: 005a 2562 6f76 696e 652e 6163 7469 7669  .Z%bovine.activi
-00001220: 7479 7374 7265 616d 732e 6f62 6a65 6374  tystreams.object
-00001230: 5f66 6163 746f 7279 7202 0000 00da 0072  _factoryr......r
-00001240: 0400 0000 7205 0000 0072 0600 0000 7207  ....r....r....r.
-00001250: 0000 0072 2a00 0000 722f 0000 0072 3f00  ...r*...r/...r?.
-00001260: 0000 7242 0000 0072 2800 0000 7228 0000  ..rB...r(...r(..
-00001270: 0072 2800 0000 7229 0000 00da 083c 6d6f  .r(...r).....<mo
-00001280: 6475 6c65 3e01 0000 0073 0c00 0000 2600  dule>....s....&.
-00001290: 1802 0808 0815 0820 0c0a                 ....... ..
+000003e0: 672f 626f 7669 6e65 2f62 6f76 696e 652f  g/bovine/bovine/
+000003f0: 626f 7669 6e65 2f62 6f76 696e 652f 6163  bovine/bovine/ac
+00000400: 7469 7669 7479 7374 7265 616d 732f 7574  tivitystreams/ut
+00000410: 696c 732f 7465 7374 5f75 7469 6c73 2e70  ils/test_utils.p
+00000420: 79da 1374 6573 745f 6765 745f 7265 6369  y..test_get_reci
+00000430: 7069 656e 7473 0b00 0000 7344 0000 0002  pients....sD....
+00000440: 0106 0104 ff04 0202 fe0c 030c 010c 010c  ................
+00000450: 0108 0108 0216 0202 060e fa02 0604 fa04  ................
+00000460: 0606 fa02 0602 fa02 0604 fa02 0602 fa04  ................
+00000470: 0604 fa02 0602 fa02 0618 fa02 0602 fa02  ................
+00000480: 0610 fa72 2a00 0000 6300 0000 0000 0000  ...r*...c.......
+00000490: 0000 0000 0005 0000 0006 0000 0043 0000  .............C..
+000004a0: 0073 e802 0000 7400 6401 6402 6403 6404  .s....t.d.d.d.d.
+000004b0: 8d03 a001 a100 a002 a100 7d00 7403 7c00  ..........}.t.|.
+000004c0: 8301 7d01 7c01 7343 6405 6406 7404 a005  ..}.|.sCd.d.t...
+000004d0: a100 7600 731d 7406 a007 7403 a101 7222  ..v.s.t...t...r"
+000004e0: 7406 a008 7403 a101 6e01 6406 6407 7404  t...t...n.d.d.t.
+000004f0: a005 a100 7600 732e 7406 a007 7c00 a101  ....v.s.t...|...
+00000500: 7233 7406 a008 7c00 a101 6e01 6407 7406  r3t...|...n.d.t.
+00000510: a008 7c01 a101 6408 9c03 1600 7d02 7409  ..|...d.....}.t.
+00000520: 7406 a00a 7c02 a101 8301 8201 6400 7d01  t...|.......d.}.
+00000530: 7400 6401 6402 6403 6404 8d03 a002 a100  t.d.d.d.d.......
+00000540: 7d00 7403 7c00 8301 7d01 7c01 0c00 7d03  }.t.|...}.|...}.
+00000550: 7c03 7389 6409 6406 7404 a005 a100 7600  |.s.d.d.t.....v.
+00000560: 7363 7406 a007 7403 a101 7268 7406 a008  sct...t...rht...
+00000570: 7403 a101 6e01 6406 6407 7404 a005 a100  t...n.d.d.t.....
+00000580: 7600 7374 7406 a007 7c00 a101 7279 7406  v.stt...|...ryt.
+00000590: a008 7c00 a101 6e01 6407 7406 a008 7c01  ..|...n.d.t...|.
+000005a0: a101 6408 9c03 1600 7d04 7409 7406 a00a  ..d.....}.t.t...
+000005b0: 7c04 a101 8301 8201 6400 0400 7d01 7d03  |.......d...}.}.
+000005c0: 7400 6401 6402 6403 6404 8d03 7d00 7c00  t.d.d.d.d...}.|.
+000005d0: 6a0b a00c 640a a101 0100 7c00 a002 a100  j...d.....|.....
+000005e0: 7d00 7403 7c00 8301 7d01 7c01 0c00 7d03  }.t.|...}.|...}.
+000005f0: 7c03 73d9 6409 6406 7404 a005 a100 7600  |.s.d.d.t.....v.
+00000600: 73b3 7406 a007 7403 a101 72b8 7406 a008  s.t...t...r.t...
+00000610: 7403 a101 6e01 6406 6407 7404 a005 a100  t...n.d.d.t.....
+00000620: 7600 73c4 7406 a007 7c00 a101 72c9 7406  v.s.t...|...r.t.
+00000630: a008 7c00 a101 6e01 6407 7406 a008 7c01  ..|...n.d.t...|.
+00000640: a101 6408 9c03 1600 7d04 7409 7406 a00a  ..d.....}.t.t...
+00000650: 7c04 a101 8301 8201 6400 0400 7d01 7d03  |.......d...}.}.
+00000660: 7400 6401 6402 6403 6404 8d03 a00d a100  t.d.d.d.d.......
+00000670: a002 a100 7d00 7403 7c00 8301 7d01 7c01  ....}.t.|...}.|.
+00000680: 9001 7324 6405 6406 7404 a005 a100 7600  ..s$d.d.t.....v.
+00000690: 73fc 7406 a007 7403 a101 9001 7201 7406  s.t...t.....r.t.
+000006a0: a008 7403 a101 6e01 6406 6407 7404 a005  ..t...n.d.d.t...
+000006b0: a100 7600 9001 730f 7406 a007 7c00 a101  ..v...s.t...|...
+000006c0: 9001 7214 7406 a008 7c00 a101 6e01 6407  ..r.t...|...n.d.
+000006d0: 7406 a008 7c01 a101 6408 9c03 1600 7d02  t...|...d.....}.
+000006e0: 7409 7406 a00a 7c02 a101 8301 8201 6400  t.t...|.......d.
+000006f0: 7d01 7400 6401 6402 6403 6404 8d03 a002  }.t.d.d.d.d.....
+00000700: a100 7d00 640b 7c00 640c 3c00 7403 7c00  ..}.d.|.d.<.t.|.
+00000710: 8301 7d01 7c01 9001 7370 6405 6406 7404  ..}.|...spd.d.t.
+00000720: a005 a100 7600 9001 7348 7406 a007 7403  ....v...sHt...t.
+00000730: a101 9001 724d 7406 a008 7403 a101 6e01  ....rMt...t...n.
+00000740: 6406 6407 7404 a005 a100 7600 9001 735b  d.d.t.....v...s[
+00000750: 7406 a007 7c00 a101 9001 7260 7406 a008  t...|.....r`t...
+00000760: 7c00 a101 6e01 6407 7406 a008 7c01 a101  |...n.d.t...|...
+00000770: 6408 9c03 1600 7d02 7409 7406 a00a 7c02  d.....}.t.t...|.
+00000780: a101 8301 8201 6400 7d01 6400 5300 290d  ......d.}.d.S.).
+00000790: 4e72 0800 0000 7209 0000 0072 0a00 0000  Nr....r....r....
+000007a0: 720b 0000 007a 2c61 7373 6572 7420 2528  r....z,assert %(
+000007b0: 7079 3329 730a 7b25 2870 7933 2973 203d  py3)s.{%(py3)s =
+000007c0: 2025 2870 7930 2973 2825 2870 7931 2973   %(py0)s(%(py1)s
+000007d0: 290a 7d72 0600 0000 7223 0000 0029 0372  ).}r....r#...).r
+000007e0: 1500 0000 da03 7079 3172 1600 0000 7a30  ......py1r....z0
+000007f0: 6173 7365 7274 206e 6f74 2025 2870 7933  assert not %(py3
+00000800: 2973 0a7b 2528 7079 3329 7320 3d20 2528  )s.{%(py3)s = %(
+00000810: 7079 3029 7328 2528 7079 3129 7329 0a7d  py0)s(%(py1)s).}
+00000820: 5a07 736f 6d65 6f6e 657a 0961 733a 5075  Z.someonez.as:Pu
+00000830: 626c 6963 7210 0000 0029 0e72 0200 0000  blicr....).r....
+00000840: 7218 0000 0072 1a00 0000 7206 0000 0072  r....r....r....r
+00000850: 1d00 0000 721e 0000 0072 1b00 0000 721f  ....r....r....r.
+00000860: 0000 0072 2000 0000 7221 0000 0072 2200  ...r ...r!...r".
+00000870: 0000 720f 0000 0072 1900 0000 da0b 6173  ..r....r......as
+00000880: 5f75 6e6c 6973 7465 6429 0572 2300 0000  _unlisted).r#...
+00000890: 7224 0000 0072 2600 0000 da0b 4070 795f  r$...r&.....@py_
+000008a0: 6173 7365 7274 34da 0b40 7079 5f66 6f72  assert4..@py_for
+000008b0: 6d61 7435 7228 0000 0072 2800 0000 7229  mat5r(...r(...r)
+000008c0: 0000 00da 0e74 6573 745f 6973 5f70 7562  .....test_is_pub
+000008d0: 6c69 6320 0000 0073 3600 0000 0c02 0401  lic ...s6.......
+000008e0: 0401 02fd 7405 0202 0601 04ff 0402 02fe  ....t...........
+000008f0: 7e03 0e02 0c01 0801 7e01 0c03 0401 0401  ~.......~.......
+00000900: 02fd 7c05 0202 0601 04ff 0402 02fe 0803  ..|.............
+00000910: 8201 722f 0000 0063 0000 0000 0000 0000  ..r/...c........
+00000920: 0000 0000 0600 0000 0700 0000 4300 0000  ............C...
+00000930: 7380 0400 0069 007d 0074 007c 0083 017d  s....i.}.t.|...}
+00000940: 0164 017d 027c 017c 026b 027d 037c 0373  .d.}.|.|.k.}.|.s
+00000950: 4674 01a0 0264 027c 0366 0164 037c 017c  Ft...d.|.f.d.|.|
+00000960: 0266 02a1 0464 0474 03a0 04a1 0076 0073  .f...d.t.....v.s
+00000970: 2374 01a0 0574 00a1 0172 2874 01a0 0674  #t...t...r(t...t
+00000980: 00a1 016e 0164 0474 01a0 067c 00a1 0174  ...n.d.t...|...t
+00000990: 01a0 067c 01a1 0174 01a0 067c 02a1 0164  ...|...t...|...d
+000009a0: 059c 0416 007d 0464 0664 077c 0469 0116  .....}.d.d.|.i..
+000009b0: 007d 0574 0774 01a0 087c 05a1 0183 0182  .}.t.t...|......
+000009c0: 0164 0004 007d 0004 007d 0104 007d 037d  .d...}...}...}.}
+000009d0: 0264 0864 0969 017d 0074 007c 0083 017d  .d.d.i.}.t.|...}
+000009e0: 0164 097d 027c 017c 026b 027d 037c 0373  .d.}.|.|.k.}.|.s
+000009f0: 9674 01a0 0264 027c 0366 0164 037c 017c  .t...d.|.f.d.|.|
+00000a00: 0266 02a1 0464 0474 03a0 04a1 0076 0073  .f...d.t.....v.s
+00000a10: 7374 01a0 0574 00a1 0172 7874 01a0 0674  st...t...rxt...t
+00000a20: 00a1 016e 0164 0474 01a0 067c 00a1 0174  ...n.d.t...|...t
+00000a30: 01a0 067c 01a1 0174 01a0 067c 02a1 0164  ...|...t...|...d
+00000a40: 059c 0416 007d 0464 0664 077c 0469 0116  .....}.d.d.|.i..
+00000a50: 007d 0574 0774 01a0 087c 05a1 0183 0182  .}.t.t...|......
+00000a60: 0164 0004 007d 0004 007d 0104 007d 037d  .d...}...}...}.}
+00000a70: 0264 0864 0a64 0969 0169 017d 0074 007c  .d.d.d.i.i.}.t.|
+00000a80: 0083 017d 0164 097d 027c 017c 026b 027d  ...}.d.}.|.|.k.}
+00000a90: 037c 0373 e874 01a0 0264 027c 0366 0164  .|.s.t...d.|.f.d
+00000aa0: 037c 017c 0266 02a1 0464 0474 03a0 04a1  .|.|.f...d.t....
+00000ab0: 0076 0073 c574 01a0 0574 00a1 0172 ca74  .v.s.t...t...r.t
+00000ac0: 01a0 0674 00a1 016e 0164 0474 01a0 067c  ...t...n.d.t...|
+00000ad0: 00a1 0174 01a0 067c 01a1 0174 01a0 067c  ...t...|...t...|
+00000ae0: 02a1 0164 059c 0416 007d 0464 0664 077c  ...d.....}.d.d.|
+00000af0: 0469 0116 007d 0574 0774 01a0 087c 05a1  .i...}.t.t...|..
+00000b00: 0183 0182 0164 0004 007d 0004 007d 0104  .....d...}...}..
+00000b10: 007d 037d 0264 0869 0069 017d 0074 007c  .}.}.d.i.i.}.t.|
+00000b20: 0083 017d 0164 017d 027c 017c 026b 027d  ...}.d.}.|.|.k.}
+00000b30: 037c 0390 0173 3b74 01a0 0264 027c 0366  .|...s;t...d.|.f
+00000b40: 0164 037c 017c 0266 02a1 0464 0474 03a0  .d.|.|.f...d.t..
+00000b50: 04a1 0076 0090 0173 1874 01a0 0574 00a1  ...v...s.t...t..
+00000b60: 0190 0172 1d74 01a0 0674 00a1 016e 0164  ...r.t...t...n.d
+00000b70: 0474 01a0 067c 00a1 0174 01a0 067c 01a1  .t...|...t...|..
+00000b80: 0174 01a0 067c 02a1 0164 059c 0416 007d  .t...|...d.....}
+00000b90: 0464 0664 077c 0469 0116 007d 0574 0774  .d.d.|.i...}.t.t
+00000ba0: 01a0 087c 05a1 0183 0182 0164 0004 007d  ...|.......d...}
+00000bb0: 0004 007d 0104 007d 037d 0264 0b64 0969  ...}...}.}.d.d.i
+00000bc0: 017d 0074 007c 0083 017d 0164 097d 027c  .}.t.|...}.d.}.|
+00000bd0: 017c 026b 027d 037c 0390 0173 8e74 01a0  .|.k.}.|...s.t..
+00000be0: 0264 027c 0366 0164 037c 017c 0266 02a1  .d.|.f.d.|.|.f..
+00000bf0: 0464 0474 03a0 04a1 0076 0090 0173 6b74  .d.t.....v...skt
+00000c00: 01a0 0574 00a1 0190 0172 7074 01a0 0674  ...t.....rpt...t
+00000c10: 00a1 016e 0164 0474 01a0 067c 00a1 0174  ...n.d.t...|...t
+00000c20: 01a0 067c 01a1 0174 01a0 067c 02a1 0164  ...|...t...|...d
+00000c30: 059c 0416 007d 0464 0664 077c 0469 0116  .....}.d.d.|.i..
+00000c40: 007d 0574 0774 01a0 087c 05a1 0183 0182  .}.t.t...|......
+00000c50: 0164 0004 007d 0004 007d 0104 007d 037d  .d...}...}...}.}
+00000c60: 0264 0b64 0a64 0969 0169 017d 0074 007c  .d.d.d.i.i.}.t.|
+00000c70: 0083 017d 0164 097d 027c 017c 026b 027d  ...}.d.}.|.|.k.}
+00000c80: 037c 0390 0173 e374 01a0 0264 027c 0366  .|...s.t...d.|.f
+00000c90: 0164 037c 017c 0266 02a1 0464 0474 03a0  .d.|.|.f...d.t..
+00000ca0: 04a1 0076 0090 0173 c074 01a0 0574 00a1  ...v...s.t...t..
+00000cb0: 0190 0172 c574 01a0 0674 00a1 016e 0164  ...r.t...t...n.d
+00000cc0: 0474 01a0 067c 00a1 0174 01a0 067c 01a1  .t...|...t...|..
+00000cd0: 0174 01a0 067c 02a1 0164 059c 0416 007d  .t...|...d.....}
+00000ce0: 0464 0664 077c 0469 0116 007d 0574 0774  .d.d.|.i...}.t.t
+00000cf0: 01a0 087c 05a1 0183 0182 0164 0004 007d  ...|.......d...}
+00000d00: 0004 007d 0104 007d 037d 0264 0b69 0069  ...}...}.}.d.i.i
+00000d10: 017d 0074 007c 0083 017d 0164 017d 027c  .}.t.|...}.d.}.|
+00000d20: 017c 026b 027d 037c 0390 0273 3674 01a0  .|.k.}.|...s6t..
+00000d30: 0264 027c 0366 0164 037c 017c 0266 02a1  .d.|.f.d.|.|.f..
+00000d40: 0464 0474 03a0 04a1 0076 0090 0273 1374  .d.t.....v...s.t
+00000d50: 01a0 0574 00a1 0190 0272 1874 01a0 0674  ...t.....r.t...t
+00000d60: 00a1 016e 0164 0474 01a0 067c 00a1 0174  ...n.d.t...|...t
+00000d70: 01a0 067c 01a1 0174 01a0 067c 02a1 0164  ...|...t...|...d
+00000d80: 059c 0416 007d 0464 0664 077c 0469 0116  .....}.d.d.|.i..
+00000d90: 007d 0574 0774 01a0 087c 05a1 0183 0182  .}.t.t...|......
+00000da0: 0164 0004 007d 0004 007d 0104 007d 037d  .d...}...}...}.}
+00000db0: 0264 0053 0029 0c4e da0d 5f5f 4e4f 5f5f  .d.S.).N..__NO__
+00000dc0: 4143 544f 525f 5f72 1200 0000 a901 7a30  ACTOR__r......z0
+00000dd0: 2528 7079 3429 730a 7b25 2870 7934 2973  %(py4)s.{%(py4)s
+00000de0: 203d 2025 2870 7930 2973 2825 2870 7932   = %(py0)s(%(py2
+00000df0: 2973 290a 7d20 3d3d 2025 2870 7937 2973  )s).} == %(py7)s
+00000e00: 7204 0000 00a9 0472 1500 0000 da03 7079  r......r......py
+00000e10: 32da 0370 7934 da03 7079 37fa 0e61 7373  2..py4..py7..ass
+00000e20: 6572 7420 2528 7079 3929 73da 0370 7939  ert %(py9)s..py9
+00000e30: da05 6163 746f 725a 0561 6c69 6365 da02  ..actorZ.alice..
+00000e40: 6964 da0c 6174 7472 6962 7574 6564 546f  id..attributedTo
+00000e50: 2909 7204 0000 0072 1b00 0000 721c 0000  ).r....r....r...
+00000e60: 0072 1d00 0000 721e 0000 0072 1f00 0000  .r....r....r....
+00000e70: 7220 0000 0072 2100 0000 7222 0000 00a9  r ...r!...r"....
+00000e80: 0672 2500 0000 da0b 4070 795f 6173 7365  .r%.....@py_asse
+00000e90: 7274 33da 0b40 7079 5f61 7373 6572 7436  rt3..@py_assert6
+00000ea0: 5a0b 4070 795f 6173 7365 7274 35da 0b40  Z.@py_assert5..@
+00000eb0: 7079 5f66 6f72 6d61 7438 5a0c 4070 795f  py_format8Z.@py_
+00000ec0: 666f 726d 6174 3130 7228 0000 0072 2800  format10r(...r(.
+00000ed0: 0000 7229 0000 00da 1574 6573 745f 6163  ..r).....test_ac
+00000ee0: 746f 725f 666f 725f 6f62 6a65 6374 4000  tor_for_object@.
+00000ef0: 0000 730e 0000 009c 01a0 01a4 01a6 01a6  ..s.............
+00000f00: 01aa 01aa 0172 3f00 0000 6300 0000 0000  .....r?...c.....
+00000f10: 0000 0000 0000 0006 0000 0007 0000 0043  ...............C
+00000f20: 0000 0073 4601 0000 6401 6402 6901 7d00  ...sF...d.d.i.}.
+00000f30: 7400 7c00 8301 7d01 6403 7d02 7c01 7c02  t.|...}.d.}.|.|.
+00000f40: 6b02 7d03 7c03 7348 7401 a002 6404 7c03  k.}.|.sHt...d.|.
+00000f50: 6601 6405 7c01 7c02 6602 a104 6406 7403  f.d.|.|.f...d.t.
+00000f60: a004 a100 7600 7325 7401 a005 7400 a101  ....v.s%t...t...
+00000f70: 722a 7401 a006 7400 a101 6e01 6406 7401  r*t...t...n.d.t.
+00000f80: a006 7c00 a101 7401 a006 7c01 a101 7401  ..|...t...|...t.
+00000f90: a006 7c02 a101 6407 9c04 1600 7d04 6408  ..|...d.....}.d.
+00000fa0: 6409 7c04 6901 1600 7d05 7407 7401 a008  d.|.i...}.t.t...
+00000fb0: 7c05 a101 8301 8201 6400 0400 7d00 0400  |.......d...}...
+00000fc0: 7d01 0400 7d03 7d02 6402 640a 640b 9c02  }...}.}.d.d.d...
+00000fd0: 7d00 7400 7c00 8301 7d01 640c 7d02 7c01  }.t.|...}.d.}.|.
+00000fe0: 7c02 6b02 7d03 7c03 7399 7401 a002 6404  |.k.}.|.s.t...d.
+00000ff0: 7c03 6601 6405 7c01 7c02 6602 a104 6406  |.f.d.|.|.f...d.
+00001000: 7403 a004 a100 7600 7376 7401 a005 7400  t.....v.svt...t.
+00001010: a101 727b 7401 a006 7400 a101 6e01 6406  ..r{t...t...n.d.
+00001020: 7401 a006 7c00 a101 7401 a006 7c01 a101  t...|...t...|...
+00001030: 7401 a006 7c02 a101 6407 9c04 1600 7d04  t...|...d.....}.
+00001040: 6408 6409 7c04 6901 1600 7d05 7407 7401  d.d.|.i...}.t.t.
+00001050: a008 7c05 a101 8301 8201 6400 0400 7d00  ..|.......d...}.
+00001060: 0400 7d01 0400 7d03 7d02 6400 5300 290d  ..}...}.}.d.S.).
+00001070: 4e72 3900 0000 7a18 6874 7470 733a 2f2f  Nr9...z.https://
+00001080: 6162 656c 2f61 6374 6f72 2f61 6c69 6365  abel/actor/alice
+00001090: 7a0a 616c 6963 6540 6162 656c 7212 0000  z.alice@abelr...
+000010a0: 0072 3100 0000 7205 0000 0072 3200 0000  .r1...r....r2...
+000010b0: 7236 0000 0072 3700 0000 da06 616c 7973  r6...r7.....alys
+000010c0: 7361 2902 7239 0000 00da 1170 7265 6665  sa).r9.....prefe
+000010d0: 7272 6564 5573 6572 6e61 6d65 7a0b 616c  rredUsernamez.al
+000010e0: 7973 7361 4061 6265 6c29 0972 0500 0000  yssa@abel).r....
+000010f0: 721b 0000 0072 1c00 0000 721d 0000 0072  r....r....r....r
+00001100: 1e00 0000 721f 0000 0072 2000 0000 7221  ....r....r ...r!
+00001110: 0000 0072 2200 0000 723b 0000 0072 2800  ...r"...r;...r(.
+00001120: 0000 7228 0000 0072 2900 0000 da15 7465  ..r(...r).....te
+00001130: 7374 5f66 6564 6976 6572 7365 5f68 616e  st_fediverse_han
+00001140: 646c 654a 0000 0073 7c00 0000 2201 0202  dleJ...s|..."...
+00001150: 0efe 0202 04fe 0402 06fe 0202 02fe 0202  ................
+00001160: 04fe 0202 02fe 0402 04fe 0202 02fe 0202  ................
+00001170: 02fe 0202 02fe 0202 02fe 0202 02fe 0202  ................
+00001180: 18fe 0202 02fe 0202 14fe 2403 0205 0efb  ..........$.....
+00001190: 0205 04fb 0405 06fb 0205 02fb 0205 04fb  ................
+000011a0: 0205 02fb 0405 04fb 0205 02fb 0205 02fb  ................
+000011b0: 0205 02fb 0205 02fb 0205 02fb 0205 18fb  ................
+000011c0: 0205 02fb 0205 18fb 7242 0000 0029 11da  ........rB...)..
+000011d0: 0862 7569 6c74 696e 7372 1d00 0000 da19  .builtinsr......
+000011e0: 5f70 7974 6573 742e 6173 7365 7274 696f  _pytest.assertio
+000011f0: 6e2e 7265 7772 6974 65da 0961 7373 6572  n.rewrite..asser
+00001200: 7469 6f6e da07 7265 7772 6974 6572 1b00  tion..rewriter..
+00001210: 0000 5a25 626f 7669 6e65 2e61 6374 6976  ..Z%bovine.activ
+00001220: 6974 7973 7472 6561 6d73 2e6f 626a 6563  itystreams.objec
+00001230: 745f 6661 6374 6f72 7972 0200 0000 da00  t_factoryr......
+00001240: 7204 0000 0072 0500 0000 7206 0000 0072  r....r....r....r
+00001250: 0700 0000 722a 0000 0072 2f00 0000 723f  ....r*...r/...r?
+00001260: 0000 0072 4200 0000 7228 0000 0072 2800  ...rB...r(...r(.
+00001270: 0000 7228 0000 0072 2900 0000 da08 3c6d  ..r(...r).....<m
+00001280: 6f64 756c 653e 0100 0000 730c 0000 0026  odule>....s....&
+00001290: 0018 0208 0808 1508 200c 0a              ........ ..
```

### Comparing `bovine-0.1.0/bovine/activitystreams/utils/print.py` & `bovine-0.1.1/bovine/activitystreams/utils/print.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.0/bovine/activitystreams/utils/test_utils.py` & `bovine-0.1.1/bovine/activitystreams/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.0/bovine/clients/__pycache__/__init__.cpython-310.pyc` & `bovine-0.1.1/bovine/clients/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 13 15:55:57 2023 UTC, .py size: 1326 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 27% similar despite different names*

```diff
@@ -1,93 +1,139 @@
-00000000: 6f0d 0d0a 0000 0000 0d26 3864 2e05 0000  o........&8d....
+00000000: 6f0d 0d0a 0000 0000 a4ea 3a64 2108 0000  o.........:d!...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0009 0000 0040 0000 0073 6000 0000 6400  .....@...s`...d.
-00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
-00000040: 0100 6403 6404 6c03 6d04 5a04 0100 6405  ..d.d.l.m.Z...d.
-00000050: 6500 6a05 6406 6506 6407 6506 6401 4200  e.j.d.e.d.e.d.B.
-00000060: 6606 6408 6409 8404 5a07 6405 6500 6a05  f.d.d...Z.d.e.j.
-00000070: 640a 6506 640b 6506 6407 6506 6401 4200  d.e.d.e.d.e.d.B.
-00000080: 6608 640c 640d 8404 5a08 6401 5300 290e  f.d.d...Z.d.S.).
-00000090: e900 0000 004e 2901 da16 7061 7273 655f  .....N)...parse_
-000000a0: 6665 6469 7665 7273 655f 6861 6e64 6c65  fediverse_handle
-000000b0: e901 0000 00a9 01da 156c 6f6f 6b75 705f  .........lookup_
-000000c0: 7769 7468 5f77 6562 6669 6e67 6572 da07  with_webfinger..
-000000d0: 7365 7373 696f 6eda 1066 6564 6976 6572  session..fediver
-000000e0: 7365 5f68 616e 646c 65da 0672 6574 7572  se_handle..retur
-000000f0: 6e63 0200 0000 0000 0000 0000 0000 0600  nc..............
-00000100: 0000 0500 0000 c300 0000 7340 0000 0081  ..........s@....
-00000110: 0174 007c 0183 015c 027d 027d 0364 017c  .t.|...\.}.}.d.|
-00000120: 039b 0064 029d 037d 0464 0364 047c 029b  ...d...}.d.d.|..
-00000130: 0064 057c 039b 009d 0469 017d 0574 017c  .d.|.....i.}.t.|
-00000140: 007c 047c 0583 0349 0064 0648 0053 0029  .|.|...I.d.H.S.)
-00000150: 0761 0801 0000 4c6f 6f6b 7320 7570 2074  .a....Looks up t
-00000160: 6865 2061 6374 6f72 2075 726c 2061 7373  he actor url ass
-00000170: 6f63 6961 7465 6420 7769 7468 2061 2046  ociated with a F
-00000180: 6564 6956 6572 7365 2068 616e 646c 652c  ediVerse handle,
-00000190: 0a20 2020 2069 2e65 2e20 616e 2069 6465  .    i.e. an ide
-000001a0: 6e74 6966 6965 7220 6f66 2074 6865 2066  ntifier of the f
-000001b0: 6f72 6d20 7573 6572 6e61 6d65 4064 6f6d  orm username@dom
-000001c0: 6169 6e2c 2075 7369 6e67 0a20 2020 2074  ain, using.    t
-000001d0: 6865 2077 6562 6669 6e67 6572 2065 6e64  he webfinger end
-000001e0: 706f 696e 740a 0a20 2020 203a 7061 7261  point..    :para
-000001f0: 6d20 7365 7373 696f 6e3a 2074 6865 2061  m session: the a
-00000200: 696f 6874 7470 2e43 6c69 656e 7453 6573  iohttp.ClientSes
-00000210: 7369 6f6e 2074 6f20 7573 650a 2020 2020  sion to use.    
-00000220: 3a70 6172 616d 2066 6564 6976 6572 7365  :param fediverse
-00000230: 5f68 616e 646c 653a 2074 6865 2046 6564  _handle: the Fed
-00000240: 6956 6572 7365 2068 616e 646c 6520 6173  iVerse handle as
-00000250: 2061 2073 7472 696e 670a 2020 2020 fa08   a string.    ..
-00000260: 6874 7470 733a 2f2f fa16 2f2e 7765 6c6c  https://../.well
-00000270: 2d6b 6e6f 776e 2f77 6562 6669 6e67 6572  -known/webfinger
-00000280: da08 7265 736f 7572 6365 7a05 6163 6374  ..resourcez.acct
-00000290: 3afa 0140 4e29 0272 0200 0000 7205 0000  :..@N).r....r...
-000002a0: 0029 0672 0600 0000 7207 0000 00da 0875  .).r....r......u
-000002b0: 7365 726e 616d 65da 0664 6f6d 6169 6eda  sername..domain.
-000002c0: 0d77 6562 6669 6e67 6572 5f75 726c da06  .webfinger_url..
-000002d0: 7061 7261 6d73 a900 7211 0000 00fa 4b2f  params..r.....K/
-000002e0: 776f 6f64 7065 636b 6572 2f73 7263 2f63  woodpecker/src/c
-000002f0: 6f64 6562 6572 672e 6f72 672f 6865 6c67  odeberg.org/helg
-00000300: 652f 626f 7669 6e65 2f62 6f76 696e 652f  e/bovine/bovine/
-00000310: 626f 7669 6e65 2f63 6c69 656e 7473 2f5f  bovine/clients/_
-00000320: 5f69 6e69 745f 5f2e 7079 da1d 6c6f 6f6b  _init__.py..look
-00000330: 7570 5f61 6363 6f75 6e74 5f77 6974 685f  up_account_with_
-00000340: 7765 6266 696e 6765 7208 0000 0073 0a00  webfinger....s..
-00000350: 0000 0280 0c0a 0c02 1401 1202 7213 0000  ............r...
-00000360: 0072 0e00 0000 da03 6469 6463 0300 0000  .r......didc....
-00000370: 0000 0000 0000 0000 0500 0000 0400 0000  ................
-00000380: c300 0000 7328 0000 0081 0164 017c 019b  ....s(.....d.|..
-00000390: 0064 029d 037d 0364 037c 0269 017d 0474  .d...}.d.|.i.}.t
-000003a0: 007c 007c 037c 0483 0349 0064 0448 0053  .|.|.|...I.d.H.S
-000003b0: 0029 057a ff4c 6f6f 6b73 2075 7020 7468  .).z.Looks up th
-000003c0: 6520 6163 746f 7220 7572 6c20 6173 736f  e actor url asso
-000003d0: 6369 6174 6564 2077 6974 6820 6120 6469  ciated with a di
-000003e0: 6420 616e 6420 646f 6d61 696e 0a20 2020  d and domain.   
-000003f0: 2075 7369 6e67 2074 6865 2077 6562 6669   using the webfi
-00000400: 6e67 6572 2065 6e64 706f 696e 740a 0a20  nger endpoint.. 
-00000410: 2020 203a 7061 7261 6d20 7365 7373 696f     :param sessio
-00000420: 6e3a 2074 6865 2061 696f 6874 7470 2e43  n: the aiohttp.C
-00000430: 6c69 656e 7453 6573 7369 6f6e 2074 6f20  lientSession to 
-00000440: 7573 650a 2020 2020 3a70 6172 616d 2064  use.    :param d
-00000450: 6f6d 6169 6e3a 2074 6865 2064 6f6d 6169  omain: the domai
-00000460: 6e20 746f 2070 6572 666f 726d 2074 6865  n to perform the
-00000470: 206c 6f6f 6b75 7020 6672 6f6d 0a20 2020   lookup from.   
-00000480: 203a 7061 7261 6d20 6469 643a 2074 6865   :param did: the
-00000490: 2064 6964 206b 6579 2074 6f20 7065 7266   did key to perf
-000004a0: 6f72 6d20 6c6f 6f6b 7570 2077 6974 680a  orm lookup with.
-000004b0: 2020 2020 7209 0000 0072 0a00 0000 720b      r....r....r.
-000004c0: 0000 004e 7204 0000 0029 0572 0600 0000  ...Nr....).r....
-000004d0: 720e 0000 0072 1400 0000 720f 0000 0072  r....r....r....r
-000004e0: 1000 0000 7211 0000 0072 1100 0000 7212  ....r....r....r.
-000004f0: 0000 00da 196c 6f6f 6b75 705f 6469 645f  .....lookup_did_
-00000500: 7769 7468 5f77 6562 6669 6e67 6572 1a00  with_webfinger..
-00000510: 0000 7308 0000 0002 800c 0a08 0112 0272  ..s............r
-00000520: 1500 0000 2909 da07 6169 6f68 7474 705a  ....)...aiohttpZ
-00000530: 1262 6f76 696e 652e 7574 696c 732e 7061  .bovine.utils.pa
-00000540: 7273 6572 0200 0000 5a0e 6c6f 6f6b 7570  rser....Z.lookup
-00000550: 5f61 6363 6f75 6e74 7205 0000 00da 0d43  _accountr......C
-00000560: 6c69 656e 7453 6573 7369 6f6e da03 7374  lientSession..st
-00000570: 7272 1300 0000 7215 0000 0072 1100 0000  rr....r....r....
-00000580: 7211 0000 0072 1100 0000 7212 0000 00da  r....r....r.....
-00000590: 083c 6d6f 6475 6c65 3e01 0000 0073 2600  .<module>....s&.
-000005a0: 0000 0800 0c02 0c02 0203 0401 02ff 0201  ................
-000005b0: 02ff 0602 0afe 0212 0401 02ff 0201 02ff  ................
-000005c0: 0201 02ff 0602 0efe                      ........
+00000020: 0009 0000 0040 0000 0073 a600 0000 6400  .....@...s....d.
+00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
+00000040: 6401 6c02 5a02 6400 6402 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
+00000050: 0100 6403 6404 6c05 6d06 5a06 0100 6403  ..d.d.l.m.Z...d.
+00000060: 6405 6c07 6d08 5a08 6d09 5a09 0100 6500  d.l.m.Z.m.Z...e.
+00000070: a00a 650b a101 5a0c 6406 6502 6a0d 6407  ..e...Z.d.e.j.d.
+00000080: 650e 6408 650e 6401 4200 6606 6409 640a  e.d.e.d.B.f.d.d.
+00000090: 8404 5a0f 6406 6502 6a0d 640b 650e 640c  ..Z.d.e.j.d.e.d.
+000000a0: 650e 6408 650e 6401 4200 6608 640d 640e  e.d.e.d.B.f.d.d.
+000000b0: 8404 5a10 6406 6502 6a0d 640b 650e 6408  ..Z.d.e.j.d.e.d.
+000000c0: 6511 6401 4200 6606 640f 6410 8404 5a12  e.d.B.f.d.d...Z.
+000000d0: 6401 5300 2911 e900 0000 004e 2901 da16  d.S.)......N)...
+000000e0: 7061 7273 655f 6665 6469 7665 7273 655f  parse_fediverse_
+000000f0: 6861 6e64 6c65 e901 0000 00a9 01da 156c  handle.........l
+00000100: 6f6f 6b75 705f 7769 7468 5f77 6562 6669  ookup_with_webfi
+00000110: 6e67 6572 2902 da10 6665 7463 685f 6e6f  nger)...fetch_no
+00000120: 6465 696e 666f 3230 da17 6665 7463 685f  deinfo20..fetch_
+00000130: 6e6f 6465 696e 666f 5f64 6f63 756d 656e  nodeinfo_documen
+00000140: 74da 0773 6573 7369 6f6e da10 6665 6469  t..session..fedi
+00000150: 7665 7273 655f 6861 6e64 6c65 da06 7265  verse_handle..re
+00000160: 7475 726e 6302 0000 0000 0000 0000 0000  turnc...........
+00000170: 0006 0000 0005 0000 00c3 0000 0073 4000  .............s@.
+00000180: 0000 8101 7400 7c01 8301 5c02 7d02 7d03  ....t.|...\.}.}.
+00000190: 6401 7c03 9b00 6402 9d03 7d04 6403 6404  d.|...d...}.d.d.
+000001a0: 7c02 9b00 6405 7c03 9b00 9d04 6901 7d05  |...d.|.....i.}.
+000001b0: 7401 7c00 7c04 7c05 8303 4900 6406 4800  t.|.|.|...I.d.H.
+000001c0: 5300 2907 6108 0100 004c 6f6f 6b73 2075  S.).a....Looks u
+000001d0: 7020 7468 6520 6163 746f 7220 7572 6c20  p the actor url 
+000001e0: 6173 736f 6369 6174 6564 2077 6974 6820  associated with 
+000001f0: 6120 4665 6469 5665 7273 6520 6861 6e64  a FediVerse hand
+00000200: 6c65 2c0a 2020 2020 692e 652e 2061 6e20  le,.    i.e. an 
+00000210: 6964 656e 7469 6669 6572 206f 6620 7468  identifier of th
+00000220: 6520 666f 726d 2075 7365 726e 616d 6540  e form username@
+00000230: 646f 6d61 696e 2c20 7573 696e 670a 2020  domain, using.  
+00000240: 2020 7468 6520 7765 6266 696e 6765 7220    the webfinger 
+00000250: 656e 6470 6f69 6e74 0a0a 2020 2020 3a70  endpoint..    :p
+00000260: 6172 616d 2073 6573 7369 6f6e 3a20 7468  aram session: th
+00000270: 6520 6169 6f68 7474 702e 436c 6965 6e74  e aiohttp.Client
+00000280: 5365 7373 696f 6e20 746f 2075 7365 0a20  Session to use. 
+00000290: 2020 203a 7061 7261 6d20 6665 6469 7665     :param fedive
+000002a0: 7273 655f 6861 6e64 6c65 3a20 7468 6520  rse_handle: the 
+000002b0: 4665 6469 5665 7273 6520 6861 6e64 6c65  FediVerse handle
+000002c0: 2061 7320 6120 7374 7269 6e67 0a20 2020   as a string.   
+000002d0: 20fa 0868 7474 7073 3a2f 2ffa 162f 2e77   ..https://../.w
+000002e0: 656c 6c2d 6b6e 6f77 6e2f 7765 6266 696e  ell-known/webfin
+000002f0: 6765 72da 0872 6573 6f75 7263 657a 0561  ger..resourcez.a
+00000300: 6363 743a fa01 404e 2902 7202 0000 0072  cct:..@N).r....r
+00000310: 0500 0000 2906 7208 0000 0072 0900 0000  ....).r....r....
+00000320: da08 7573 6572 6e61 6d65 da06 646f 6d61  ..username..doma
+00000330: 696e da0d 7765 6266 696e 6765 725f 7572  in..webfinger_ur
+00000340: 6cda 0670 6172 616d 73a9 0072 1300 0000  l..params..r....
+00000350: fa4c 2f77 6f6f 6470 6563 6b65 722f 7372  .L/woodpecker/sr
+00000360: 632f 636f 6465 6265 7267 2e6f 7267 2f62  c/codeberg.org/b
+00000370: 6f76 696e 652f 626f 7669 6e65 2f62 6f76  ovine/bovine/bov
+00000380: 696e 652f 626f 7669 6e65 2f63 6c69 656e  ine/bovine/clien
+00000390: 7473 2f5f 5f69 6e69 745f 5f2e 7079 da1d  ts/__init__.py..
+000003a0: 6c6f 6f6b 7570 5f61 6363 6f75 6e74 5f77  lookup_account_w
+000003b0: 6974 685f 7765 6266 696e 6765 720e 0000  ith_webfinger...
+000003c0: 0073 0a00 0000 0280 0c0a 0c02 1401 1202  .s..............
+000003d0: 7215 0000 0072 1000 0000 da03 6469 6463  r....r......didc
+000003e0: 0300 0000 0000 0000 0000 0000 0500 0000  ................
+000003f0: 0400 0000 c300 0000 7328 0000 0081 0164  ........s(.....d
+00000400: 017c 019b 0064 029d 037d 0364 037c 0269  .|...d...}.d.|.i
+00000410: 017d 0474 007c 007c 037c 0483 0349 0064  .}.t.|.|.|...I.d
+00000420: 0448 0053 0029 057a ff4c 6f6f 6b73 2075  .H.S.).z.Looks u
+00000430: 7020 7468 6520 6163 746f 7220 7572 6c20  p the actor url 
+00000440: 6173 736f 6369 6174 6564 2077 6974 6820  associated with 
+00000450: 6120 6469 6420 616e 6420 646f 6d61 696e  a did and domain
+00000460: 0a20 2020 2075 7369 6e67 2074 6865 2077  .    using the w
+00000470: 6562 6669 6e67 6572 2065 6e64 706f 696e  ebfinger endpoin
+00000480: 740a 0a20 2020 203a 7061 7261 6d20 7365  t..    :param se
+00000490: 7373 696f 6e3a 2074 6865 2061 696f 6874  ssion: the aioht
+000004a0: 7470 2e43 6c69 656e 7453 6573 7369 6f6e  tp.ClientSession
+000004b0: 2074 6f20 7573 650a 2020 2020 3a70 6172   to use.    :par
+000004c0: 616d 2064 6f6d 6169 6e3a 2074 6865 2064  am domain: the d
+000004d0: 6f6d 6169 6e20 746f 2070 6572 666f 726d  omain to perform
+000004e0: 2074 6865 206c 6f6f 6b75 7020 6672 6f6d   the lookup from
+000004f0: 0a20 2020 203a 7061 7261 6d20 6469 643a  .    :param did:
+00000500: 2074 6865 2064 6964 206b 6579 2074 6f20   the did key to 
+00000510: 7065 7266 6f72 6d20 6c6f 6f6b 7570 2077  perform lookup w
+00000520: 6974 680a 2020 2020 720b 0000 0072 0c00  ith.    r....r..
+00000530: 0000 720d 0000 004e 7204 0000 0029 0572  ..r....Nr....).r
+00000540: 0800 0000 7210 0000 0072 1600 0000 7211  ....r....r....r.
+00000550: 0000 0072 1200 0000 7213 0000 0072 1300  ...r....r....r..
+00000560: 0000 7214 0000 00da 196c 6f6f 6b75 705f  ..r......lookup_
+00000570: 6469 645f 7769 7468 5f77 6562 6669 6e67  did_with_webfing
+00000580: 6572 2000 0000 7308 0000 0002 800c 0a08  er ...s.........
+00000590: 0112 0272 1700 0000 6302 0000 0000 0000  ...r....c.......
+000005a0: 0000 0000 0006 0000 000a 0000 00c3 0000  ................
+000005b0: 0073 9e00 0000 8101 7a25 7400 7c00 7c01  .s......z%t.|.|.
+000005c0: 8302 4900 6401 4800 7d02 7c02 6402 1900  ..I.d.H.}.|.d...
+000005d0: 4400 5d15 7d03 7c03 6403 1900 6404 6b02  D.].}.|.d...d.k.
+000005e0: 7223 7401 7c00 7c03 6405 1900 8302 4900  r#t.|.|.d.....I.
+000005f0: 6401 4800 0200 0100 5700 5300 710e 5700  d.H.....W.S.q.W.
+00000600: 6401 5300 0400 7402 794e 0100 7d04 0100  d.S...t.yN..}...
+00000610: 7a1c 7403 a004 7405 7c04 8301 a101 0100  z.t...t.|.......
+00000620: 7406 a007 a100 a008 a100 4400 5d07 7d05  t.........D.].}.
+00000630: 7403 a004 7c05 a101 0100 713b 5700 5900  t...|.....q;W.Y.
+00000640: 6401 7d04 7e04 6401 5300 6401 7d04 7e04  d.}.~.d.S.d.}.~.
+00000650: 7701 7700 2906 7a58 4665 7463 6865 7320  w.w.).zXFetches 
+00000660: 7468 6520 6e6f 6465 696e 666f 2032 2e30  the nodeinfo 2.0
+00000670: 206f 626a 6563 7420 6672 6f6d 2064 6f6d   object from dom
+00000680: 6169 6e20 7573 696e 6720 7468 6520 2f2e  ain using the /.
+00000690: 7765 6c6c 2d6b 6e6f 776e 2f6e 6f64 6569  well-known/nodei
+000006a0: 6e66 6f0a 2020 2020 656e 6470 6f69 6e74  nfo.    endpoint
+000006b0: 4eda 056c 696e 6b73 da03 7265 6c7a 2f68  N..links..relz/h
+000006c0: 7474 703a 2f2f 6e6f 6465 696e 666f 2e64  ttp://nodeinfo.d
+000006d0: 6961 7370 6f72 612e 736f 6674 7761 7265  iaspora.software
+000006e0: 2f6e 732f 7363 6865 6d61 2f32 2e30 5a04  /ns/schema/2.0Z.
+000006f0: 6872 6566 2909 7207 0000 0072 0600 0000  href).r....r....
+00000700: da09 4578 6365 7074 696f 6eda 066c 6f67  ..Exception..log
+00000710: 6765 72da 0565 7272 6f72 da03 7374 72da  ger..error..str.
+00000720: 0974 7261 6365 6261 636b da0a 666f 726d  .traceback..form
+00000730: 6174 5f65 7863 da0a 7370 6c69 746c 696e  at_exc..splitlin
+00000740: 6573 2906 7208 0000 0072 1000 0000 da04  es).r....r......
+00000750: 6461 7461 da04 6c69 6e6b da01 655a 086c  data..link..eZ.l
+00000760: 6f67 5f6c 696e 6572 1300 0000 7213 0000  og_liner....r...
+00000770: 0072 1400 0000 da0e 6665 7463 685f 6e6f  .r......fetch_no
+00000780: 6465 696e 666f 3000 0000 731e 0000 0002  deinfo0...s.....
+00000790: 8002 0410 010c 020c 011a 0102 ff06 030e  ................
+000007a0: 020e 0110 010c 010e 0108 8002 fc72 2400  .............r$.
+000007b0: 0000 2913 da07 6c6f 6767 696e 6772 1e00  ..)...loggingr..
+000007c0: 0000 da07 6169 6f68 7474 705a 0c62 6f76  ....aiohttpZ.bov
+000007d0: 696e 652e 7574 696c 7372 0200 0000 5a0e  ine.utilsr....Z.
+000007e0: 6c6f 6f6b 7570 5f61 6363 6f75 6e74 7205  lookup_accountr.
+000007f0: 0000 005a 086e 6f64 6569 6e66 6f72 0600  ...Z.nodeinfor..
+00000800: 0000 7207 0000 00da 0967 6574 4c6f 6767  ..r......getLogg
+00000810: 6572 da08 5f5f 6e61 6d65 5f5f 721b 0000  er..__name__r...
+00000820: 00da 0d43 6c69 656e 7453 6573 7369 6f6e  ...ClientSession
+00000830: 721d 0000 0072 1500 0000 7217 0000 00da  r....r....r.....
+00000840: 0464 6963 7472 2400 0000 7213 0000 0072  .dictr$...r....r
+00000850: 1300 0000 7213 0000 0072 1400 0000 da08  ....r....r......
+00000860: 3c6d 6f64 756c 653e 0100 0000 7330 0000  <module>....s0..
+00000870: 0008 0008 0108 020c 020c 0210 010a 0202  ................
+00000880: 0304 0102 ff02 0102 ff06 020a fe02 1204  ................
+00000890: 0102 ff02 0102 ff02 0102 ff06 020a fe20  ............... 
+000008a0: 10                                       .
```

### Comparing `bovine-0.1.0/bovine/clients/__pycache__/event_source.cpython-310.pyc` & `bovine-0.1.1/bovine/clients/__pycache__/event_source.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 13 15:55:57 2023 UTC, .py size: 1106 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0d26 3864 5204 0000  o........&8dR...
+00000000: 6f0d 0d0a 0000 0000 a4ea 3a64 5204 0000  o.........:dR...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 2600 0000 6400  .....@...s&...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 4700 6403 6404 8400 6404 8302 5a03  ..G.d.d...d...Z.
 00000050: 6401 5300 2905 e900 0000 004e 2901 da0f  d.S.)......N)...
 00000060: 5365 7276 6572 5365 6e74 4576 656e 7463  ServerSentEventc
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -16,77 +16,77 @@
 000000f0: 6572 7363 0400 0000 0000 0000 0000 0000  ersc............
 00000100: 0400 0000 0200 0000 4300 0000 731c 0000  ........C...s...
 00000110: 007c 017c 005f 007c 027c 005f 017c 037c  .|.|._.|.|._.|.|
 00000120: 005f 0264 007c 005f 0364 0053 00a9 014e  ._.d.|._.d.S...N
 00000130: 2904 7204 0000 0072 0500 0000 7206 0000  ).r....r....r...
 00000140: 00da 0872 6573 706f 6e73 6529 04da 0473  ...response)...s
 00000150: 656c 6672 0400 0000 7205 0000 0072 0600  elfr....r....r..
-00000160: 0000 a900 720a 0000 00fa 4f2f 776f 6f64  ....r.....O/wood
+00000160: 0000 a900 720a 0000 00fa 502f 776f 6f64  ....r.....P/wood
 00000170: 7065 636b 6572 2f73 7263 2f63 6f64 6562  pecker/src/codeb
-00000180: 6572 672e 6f72 672f 6865 6c67 652f 626f  erg.org/helge/bo
-00000190: 7669 6e65 2f62 6f76 696e 652f 626f 7669  vine/bovine/bovi
-000001a0: 6e65 2f63 6c69 656e 7473 2f65 7665 6e74  ne/clients/event
-000001b0: 5f73 6f75 7263 652e 7079 da08 5f5f 696e  _source.py..__in
-000001c0: 6974 5f5f 0700 0000 7308 0000 0006 0106  it__....s.......
-000001d0: 0106 010a 017a 1445 7665 6e74 536f 7572  .....z.EventSour
-000001e0: 6365 2e5f 5f69 6e69 745f 5f63 0100 0000  ce.__init__c....
-000001f0: 0000 0000 0000 0000 0200 0000 0500 0000  ................
-00000200: c300 0000 7338 0000 0081 0174 006a 0164  ....s8.....t.j.d
-00000210: 0064 018d 017d 017c 006a 026a 037c 006a  .d...}.|.j.j.|.j
-00000220: 0464 0264 0369 017c 006a 05a5 017c 0164  .d.d.i.|.j...|.d
-00000230: 048d 0349 0064 0048 007c 005f 0664 0053  ...I.d.H.|._.d.S
-00000240: 0029 054e 2901 da05 746f 7461 6cda 0641  .).N)...total..A
-00000250: 6363 6570 747a 1174 6578 742f 6576 656e  cceptz.text/even
-00000260: 742d 7374 7265 616d 2902 7206 0000 00da  t-stream).r.....
-00000270: 0774 696d 656f 7574 2907 da07 6169 6f68  .timeout)...aioh
-00000280: 7474 70da 0d43 6c69 656e 7454 696d 656f  ttp..ClientTimeo
-00000290: 7574 7204 0000 00da 0367 6574 7205 0000  utr......getr...
-000002a0: 0072 0600 0000 7208 0000 0029 0272 0900  .r....r....).r..
-000002b0: 0000 720f 0000 0072 0a00 0000 720a 0000  ..r....r....r...
-000002c0: 0072 0b00 0000 da0f 6372 6561 7465 5f72  .r......create_r
-000002d0: 6573 706f 6e73 650d 0000 0073 0e00 0000  esponse....s....
-000002e0: 0280 0c01 0602 0401 0c01 0201 12fd 7a1b  ..............z.
-000002f0: 4576 656e 7453 6f75 7263 652e 6372 6561  EventSource.crea
-00000300: 7465 5f72 6573 706f 6e73 6563 0100 0000  te_responsec....
-00000310: 0000 0000 0000 0000 0100 0000 0100 0000  ................
-00000320: 4300 0000 7304 0000 007c 0053 0072 0700  C...s....|.S.r..
-00000330: 0000 720a 0000 0029 0172 0900 0000 720a  ..r....).r....r.
-00000340: 0000 0072 0a00 0000 720b 0000 00da 095f  ...r....r......_
-00000350: 5f61 6974 6572 5f5f 1600 0000 7302 0000  _aiter__....s...
-00000360: 0004 017a 1545 7665 6e74 536f 7572 6365  ...z.EventSource
-00000370: 2e5f 5f61 6974 6572 5f5f 6301 0000 0000  .__aiter__c.....
-00000380: 0000 0000 0000 0005 0000 0007 0000 00c3  ................
-00000390: 0000 0073 8000 0000 8101 7c00 6a00 6400  ...s......|.j.d.
-000003a0: 7500 720d 7c00 a001 a100 4900 6400 4800  u.r.|.....I.d.H.
-000003b0: 0100 6401 7d01 7c00 6a00 6a02 3200 7a29  ..d.}.|.j.j.2.z)
-000003c0: 3300 6400 4800 5700 7d02 7c02 a003 6402  3.d.H.W.}.|...d.
-000003d0: a101 7d03 7c03 6403 1900 6404 6b02 7225  ..}.|.d...d.k.r%
-000003e0: 7113 7c03 6405 6b02 7236 7404 a005 7c01  q.|.d.k.r6t...|.
-000003f0: a101 7d04 7c04 6a06 7235 7c04 0200 0100  ..}.|.j.r5|.....
-00000400: 5300 7113 7c01 9b00 7c03 9b00 9d02 7d01  S.q.|...|.....}.
-00000410: 7113 3600 6400 5300 2906 4eda 007a 0575  q.6.d.S.).N..z.u
-00000420: 7466 2d38 7201 0000 00fa 013a da01 0a29  tf-8r......:...)
-00000430: 0772 0800 0000 7213 0000 00da 0763 6f6e  .r....r......con
-00000440: 7465 6e74 da06 6465 636f 6465 7202 0000  tent..decoder...
-00000450: 005a 0a70 6172 7365 5f75 7466 38da 0464  .Z.parse_utf8..d
-00000460: 6174 6129 0572 0900 0000 5a08 746f 5f70  ata).r....Z.to_p
-00000470: 6172 7365 5a0d 6c69 6e65 5f69 6e5f 6279  arseZ.line_in_by
-00000480: 7465 73da 046c 696e 65da 0565 7665 6e74  tes..line..event
-00000490: 720a 0000 0072 0a00 0000 720b 0000 00da  r....r....r.....
-000004a0: 095f 5f61 6e65 7874 5f5f 1900 0000 731e  .__anext__....s.
-000004b0: 0000 0002 800a 010e 0104 0214 020a 010c  ................
-000004c0: 0102 0108 010a 0106 0108 0102 ff0e 0306  ................
-000004d0: f77a 1545 7665 6e74 536f 7572 6365 2e5f  .z.EventSource._
-000004e0: 5f61 6e65 7874 5f5f 4e29 0bda 085f 5f6e  _anext__N)...__n
-000004f0: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
-00000500: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5f72  _..__qualname__r
-00000510: 1000 0000 da0d 436c 6965 6e74 5365 7373  ......ClientSess
-00000520: 696f 6eda 0373 7472 da04 6469 6374 720c  ion..str..dictr.
-00000530: 0000 0072 1300 0000 7214 0000 0072 1d00  ...r....r....r..
-00000540: 0000 720a 0000 0072 0a00 0000 720a 0000  ..r....r....r...
-00000550: 0072 0b00 0000 7203 0000 0006 0000 0073  .r....r........s
-00000560: 0a00 0000 0800 1c01 0806 0809 0c03 7203  ..............r.
-00000570: 0000 0029 0472 1000 0000 5a0c 626f 7669  ...).r....Z.bovi
-00000580: 6e65 2e74 7970 6573 7202 0000 0072 0300  ne.typesr....r..
-00000590: 0000 720a 0000 0072 0a00 0000 720a 0000  ..r....r....r...
-000005a0: 0072 0b00 0000 da08 3c6d 6f64 756c 653e  .r......<module>
-000005b0: 0100 0000 7306 0000 0008 000c 0212 03    ....s..........
+00000180: 6572 672e 6f72 672f 626f 7669 6e65 2f62  erg.org/bovine/b
+00000190: 6f76 696e 652f 626f 7669 6e65 2f62 6f76  ovine/bovine/bov
+000001a0: 696e 652f 636c 6965 6e74 732f 6576 656e  ine/clients/even
+000001b0: 745f 736f 7572 6365 2e70 79da 085f 5f69  t_source.py..__i
+000001c0: 6e69 745f 5f07 0000 0073 0800 0000 0601  nit__....s......
+000001d0: 0601 0601 0a01 7a14 4576 656e 7453 6f75  ......z.EventSou
+000001e0: 7263 652e 5f5f 696e 6974 5f5f 6301 0000  rce.__init__c...
+000001f0: 0000 0000 0000 0000 0002 0000 0005 0000  ................
+00000200: 00c3 0000 0073 3800 0000 8101 7400 6a01  .....s8.....t.j.
+00000210: 6400 6401 8d01 7d01 7c00 6a02 6a03 7c00  d.d...}.|.j.j.|.
+00000220: 6a04 6402 6403 6901 7c00 6a05 a501 7c01  j.d.d.i.|.j...|.
+00000230: 6404 8d03 4900 6400 4800 7c00 5f06 6400  d...I.d.H.|._.d.
+00000240: 5300 2905 4e29 01da 0574 6f74 616c da06  S.).N)...total..
+00000250: 4163 6365 7074 7a11 7465 7874 2f65 7665  Acceptz.text/eve
+00000260: 6e74 2d73 7472 6561 6d29 0272 0600 0000  nt-stream).r....
+00000270: da07 7469 6d65 6f75 7429 07da 0761 696f  ..timeout)...aio
+00000280: 6874 7470 da0d 436c 6965 6e74 5469 6d65  http..ClientTime
+00000290: 6f75 7472 0400 0000 da03 6765 7472 0500  outr......getr..
+000002a0: 0000 7206 0000 0072 0800 0000 2902 7209  ..r....r....).r.
+000002b0: 0000 0072 0f00 0000 720a 0000 0072 0a00  ...r....r....r..
+000002c0: 0000 720b 0000 00da 0f63 7265 6174 655f  ..r......create_
+000002d0: 7265 7370 6f6e 7365 0d00 0000 730e 0000  response....s...
+000002e0: 0002 800c 0106 0204 010c 0102 0112 fd7a  ...............z
+000002f0: 1b45 7665 6e74 536f 7572 6365 2e63 7265  .EventSource.cre
+00000300: 6174 655f 7265 7370 6f6e 7365 6301 0000  ate_responsec...
+00000310: 0000 0000 0000 0000 0001 0000 0001 0000  ................
+00000320: 0043 0000 0073 0400 0000 7c00 5300 7207  .C...s....|.S.r.
+00000330: 0000 0072 0a00 0000 2901 7209 0000 0072  ...r....).r....r
+00000340: 0a00 0000 720a 0000 0072 0b00 0000 da09  ....r....r......
+00000350: 5f5f 6169 7465 725f 5f16 0000 0073 0200  __aiter__....s..
+00000360: 0000 0401 7a15 4576 656e 7453 6f75 7263  ....z.EventSourc
+00000370: 652e 5f5f 6169 7465 725f 5f63 0100 0000  e.__aiter__c....
+00000380: 0000 0000 0000 0000 0500 0000 0700 0000  ................
+00000390: c300 0000 7380 0000 0081 017c 006a 0064  ....s......|.j.d
+000003a0: 0075 0072 0d7c 00a0 01a1 0049 0064 0048  .u.r.|.....I.d.H
+000003b0: 0001 0064 017d 017c 006a 006a 0232 007a  ...d.}.|.j.j.2.z
+000003c0: 2933 0064 0048 0057 007d 027c 02a0 0364  )3.d.H.W.}.|...d
+000003d0: 02a1 017d 037c 0364 0319 0064 046b 0272  ...}.|.d...d.k.r
+000003e0: 2571 137c 0364 056b 0272 3674 04a0 057c  %q.|.d.k.r6t...|
+000003f0: 01a1 017d 047c 046a 0672 357c 0402 0001  ...}.|.j.r5|....
+00000400: 0053 0071 137c 019b 007c 039b 009d 027d  .S.q.|...|.....}
+00000410: 0171 1336 0064 0053 0029 064e da00 7a05  .q.6.d.S.).N..z.
+00000420: 7574 662d 3872 0100 0000 fa01 3ada 010a  utf-8r......:...
+00000430: 2907 7208 0000 0072 1300 0000 da07 636f  ).r....r......co
+00000440: 6e74 656e 74da 0664 6563 6f64 6572 0200  ntent..decoder..
+00000450: 0000 5a0a 7061 7273 655f 7574 6638 da04  ..Z.parse_utf8..
+00000460: 6461 7461 2905 7209 0000 005a 0874 6f5f  data).r....Z.to_
+00000470: 7061 7273 655a 0d6c 696e 655f 696e 5f62  parseZ.line_in_b
+00000480: 7974 6573 da04 6c69 6e65 da05 6576 656e  ytes..line..even
+00000490: 7472 0a00 0000 720a 0000 0072 0b00 0000  tr....r....r....
+000004a0: da09 5f5f 616e 6578 745f 5f19 0000 0073  ..__anext__....s
+000004b0: 1e00 0000 0280 0a01 0e01 0402 1402 0a01  ................
+000004c0: 0c01 0201 0801 0a01 0601 0801 02ff 0e03  ................
+000004d0: 06f7 7a15 4576 656e 7453 6f75 7263 652e  ..z.EventSource.
+000004e0: 5f5f 616e 6578 745f 5f4e 290b da08 5f5f  __anext__N)...__
+000004f0: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
+00000500: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
+00000510: 7210 0000 00da 0d43 6c69 656e 7453 6573  r......ClientSes
+00000520: 7369 6f6e da03 7374 72da 0464 6963 7472  sion..str..dictr
+00000530: 0c00 0000 7213 0000 0072 1400 0000 721d  ....r....r....r.
+00000540: 0000 0072 0a00 0000 720a 0000 0072 0a00  ...r....r....r..
+00000550: 0000 720b 0000 0072 0300 0000 0600 0000  ..r....r........
+00000560: 730a 0000 0008 001c 0108 0608 090c 0372  s..............r
+00000570: 0300 0000 2904 7210 0000 005a 0c62 6f76  ....).r....Z.bov
+00000580: 696e 652e 7479 7065 7372 0200 0000 7203  ine.typesr....r.
+00000590: 0000 0072 0a00 0000 720a 0000 0072 0a00  ...r....r....r..
+000005a0: 0000 720b 0000 00da 083c 6d6f 6475 6c65  ..r......<module
+000005b0: 3e01 0000 0073 0600 0000 0800 0c02 1203  >....s..........
```

### Comparing `bovine-0.1.0/bovine/clients/__pycache__/lookup_account.cpython-310.pyc` & `bovine-0.1.1/bovine/clients/__pycache__/lookup_account.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 13 15:55:57 2023 UTC, .py size: 787 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0d26 3864 1303 0000  o........&8d....
+00000000: 6f0d 0d0a 0000 0000 a4ea 3a64 1303 0000  o.........:d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 4a00 0000 6400  .....@...sJ...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6402 6403 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6501 a005 6506 a101 5a07 6404 6502  ..e...e...Z.d.e.
 00000060: 6a08 6405 6509 6406 650a 6606 6407 6408  j.d.e.d.e.f.d.d.
 00000070: 8404 5a0b 6401 5300 2909 e900 0000 004e  ..Z.d.S.)......N
@@ -29,36 +29,36 @@
 000001c0: 0053 0031 0049 0064 0048 0073 7b77 0101  .S.1.I.d.H.s{w..
 000001d0: 0001 0001 0059 0001 0064 0053 0029 0a4e  .....Y...d.S.).N
 000001e0: 7a0a 7573 6572 2d61 6765 6e74 2902 7206  z.user-agent).r.
 000001f0: 0000 00da 0768 6561 6465 7273 e9c8 0000  .....headers....
 00000200: 00da 0872 6573 6f75 7263 657a 1a20 6e6f  ...resourcez. no
 00000210: 7420 666f 756e 6420 7573 696e 6720 7765  t found using we
 00000220: 6266 696e 6765 72da 056c 696e 6b73 da03  bfinger..links..
-00000230: 7265 6cda 0473 656c 665a 0468 7265 6629  rel..selfZ.href)
+00000230: 7265 6cda 0473 656c 66da 0468 7265 6629  rel..self..href)
 00000240: 08da 0367 6574 7203 0000 00da 0673 7461  ...getr......sta
 00000250: 7475 73da 066c 6f67 6765 72da 0477 6172  tus..logger..war
 00000260: 6eda 0474 6578 74da 046a 736f 6eda 056c  n..text..json..l
 00000270: 6f61 6473 2908 7204 0000 0072 0500 0000  oads).r....r....
 00000280: 7206 0000 00da 0872 6573 706f 6e73 6572  r......responser
-00000290: 1100 0000 da04 6461 7461 720a 0000 00da  ......datar.....
-000002a0: 0565 6e74 7279 a900 7217 0000 00fa 512f  .entry..r.....Q/
+00000290: 1200 0000 da04 6461 7461 720a 0000 00da  ......datar.....
+000002a0: 0565 6e74 7279 a900 7218 0000 00fa 522f  .entry..r.....R/
 000002b0: 776f 6f64 7065 636b 6572 2f73 7263 2f63  woodpecker/src/c
-000002c0: 6f64 6562 6572 672e 6f72 672f 6865 6c67  odeberg.org/helg
-000002d0: 652f 626f 7669 6e65 2f62 6f76 696e 652f  e/bovine/bovine/
-000002e0: 626f 7669 6e65 2f63 6c69 656e 7473 2f6c  bovine/clients/l
-000002f0: 6f6f 6b75 705f 6163 636f 756e 742e 7079  ookup_account.py
-00000300: da15 6c6f 6f6b 7570 5f77 6974 685f 7765  ..lookup_with_we
-00000310: 6266 696e 6765 720b 0000 0073 3200 0000  bfinger....s2...
-00000320: 0280 0403 0a01 0eff 0202 0a01 1401 0201  ................
-00000330: 16fb 0e06 0a01 0802 0201 16f6 080c 0801  ................
-00000340: 1401 0a01 16f1 0280 020d 10f3 0411 16ef  ................
-00000350: 0411 7219 0000 0029 0c72 1200 0000 da07  ..r....).r......
-00000360: 6c6f 6767 696e 67da 0761 696f 6874 7470  logging..aiohttp
-00000370: 5a06 636f 6e73 7473 7203 0000 00da 0967  Z.constsr......g
-00000380: 6574 4c6f 6767 6572 da08 5f5f 6e61 6d65  etLogger..__name
-00000390: 5f5f 720f 0000 00da 0d43 6c69 656e 7453  __r......ClientS
-000003a0: 6573 7369 6f6e da03 7374 72da 0464 6963  ession..str..dic
-000003b0: 7472 1900 0000 7217 0000 0072 1700 0000  tr....r....r....
-000003c0: 7217 0000 0072 1800 0000 da08 3c6d 6f64  r....r......<mod
-000003d0: 756c 653e 0100 0000 7318 0000 0008 0008  ule>....s.......
-000003e0: 0108 020c 020a 0202 0304 0102 ff02 0102  ................
-000003f0: ff02 010e ff                             .....
+000002c0: 6f64 6562 6572 672e 6f72 672f 626f 7669  odeberg.org/bovi
+000002d0: 6e65 2f62 6f76 696e 652f 626f 7669 6e65  ne/bovine/bovine
+000002e0: 2f62 6f76 696e 652f 636c 6965 6e74 732f  /bovine/clients/
+000002f0: 6c6f 6f6b 7570 5f61 6363 6f75 6e74 2e70  lookup_account.p
+00000300: 79da 156c 6f6f 6b75 705f 7769 7468 5f77  y..lookup_with_w
+00000310: 6562 6669 6e67 6572 0b00 0000 7332 0000  ebfinger....s2..
+00000320: 0002 8004 030a 010e ff02 020a 0114 0102  ................
+00000330: 0116 fb0e 060a 0108 0202 0116 f608 0c08  ................
+00000340: 0114 010a 0116 f102 8002 0d10 f304 1116  ................
+00000350: ef04 1172 1a00 0000 290c 7213 0000 00da  ...r....).r.....
+00000360: 076c 6f67 6769 6e67 da07 6169 6f68 7474  .logging..aiohtt
+00000370: 705a 0663 6f6e 7374 7372 0300 0000 da09  pZ.constsr......
+00000380: 6765 744c 6f67 6765 72da 085f 5f6e 616d  getLogger..__nam
+00000390: 655f 5f72 1000 0000 da0d 436c 6965 6e74  e__r......Client
+000003a0: 5365 7373 696f 6eda 0373 7472 da04 6469  Session..str..di
+000003b0: 6374 721a 0000 0072 1800 0000 7218 0000  ctr....r....r...
+000003c0: 0072 1800 0000 7219 0000 00da 083c 6d6f  .r....r......<mo
+000003d0: 6475 6c65 3e01 0000 0073 1800 0000 0800  dule>....s......
+000003e0: 0801 0802 0c02 0a02 0203 0401 02ff 0201  ................
+000003f0: 02ff 0201 0eff                           ......
```

### Comparing `bovine-0.1.0/bovine/clients/__pycache__/moo_auth_client.cpython-310.pyc` & `bovine-0.1.1/bovine/clients/__pycache__/moo_auth_client.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 13 15:55:57 2023 UTC, .py size: 3176 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0d26 3864 680c 0000  o........&8dh...
+00000000: 6f0d 0d0a 0000 0000 a4ea 3a64 680c 0000  o.........:dh...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 6200 0000 6400  .....@...sb...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c06 6d07 5a07 0100 6405  ..d.d.l.m.Z...d.
 00000060: 6406 6c08 6d09 5a09 0100 6405 6407 6c0a  d.l.m.Z...d.d.l.
 00000070: 6d0b 5a0b 0100 6408 6409 8400 5a0c 4700  m.Z...d.d...Z.G.
@@ -16,142 +16,142 @@
 000000f0: 4945 4e54 5f4e 414d 4529 01da 0b45 7665  IENT_NAME)...Eve
 00000100: 6e74 536f 7572 6365 6301 0000 0000 0000  ntSourcec.......
 00000110: 0000 0000 0002 0000 0002 0000 0043 0000  .............C..
 00000120: 0073 1400 0000 7400 7c00 8301 7d01 7c01  .s....t.|...}.|.
 00000130: 6a01 7c01 6a02 6602 5300 a901 4e29 0372  j.|.j.f.S...N).r
 00000140: 0200 0000 da06 6e65 746c 6f63 da04 7061  ......netloc..pa
 00000150: 7468 2902 da03 7572 6cda 0a70 6172 7365  th)...url..parse
-00000160: 645f 7572 6ca9 0072 0e00 0000 fa52 2f77  d_url..r.....R/w
+00000160: 645f 7572 6ca9 0072 0e00 0000 fa53 2f77  d_url..r.....S/w
 00000170: 6f6f 6470 6563 6b65 722f 7372 632f 636f  oodpecker/src/co
-00000180: 6465 6265 7267 2e6f 7267 2f68 656c 6765  deberg.org/helge
-00000190: 2f62 6f76 696e 652f 626f 7669 6e65 2f62  /bovine/bovine/b
-000001a0: 6f76 696e 652f 636c 6965 6e74 732f 6d6f  ovine/clients/mo
-000001b0: 6f5f 6175 7468 5f63 6c69 656e 742e 7079  o_auth_client.py
-000001c0: da14 686f 7374 5f74 6172 6765 745f 6672  ..host_target_fr
-000001d0: 6f6d 5f75 726c 0d00 0000 7304 0000 0008  om_url....s.....
-000001e0: 010c 0172 1000 0000 6300 0000 0000 0000  ...r....c.......
-000001f0: 0000 0000 0000 0000 0003 0000 0040 0000  .............@..
-00000200: 0073 3a00 0000 6500 5a01 6400 5a02 6401  .s:...e.Z.d.Z.d.
-00000210: 6402 8400 5a03 6900 6601 6403 6404 8401  d...Z.i.f.d.d...
-00000220: 5a04 6900 6405 6602 6406 6407 8401 5a05  Z.i.d.f.d.d...Z.
-00000230: 6900 6601 6408 6409 8401 5a06 6405 5300  i.f.d.d...Z.d.S.
-00000240: 290a da0d 4d6f 6f41 7574 6843 6c69 656e  )...MooAuthClien
-00000250: 7463 0400 0000 0000 0000 0000 0000 0400  tc..............
-00000260: 0000 0200 0000 4300 0000 7316 0000 007c  ......C...s....|
-00000270: 017c 005f 007c 027c 005f 017c 037c 005f  .|._.|.|._.|.|._
-00000280: 0264 0053 0072 0900 0000 2903 da07 7365  .d.S.r....)...se
-00000290: 7373 696f 6eda 0764 6964 5f6b 6579 da0b  ssion..did_key..
-000002a0: 7072 6976 6174 655f 6b65 7929 04da 0473  private_key)...s
-000002b0: 656c 6672 1200 0000 7213 0000 0072 1400  elfr....r....r..
-000002c0: 0000 720e 0000 0072 0e00 0000 720f 0000  ..r....r....r...
-000002d0: 00da 085f 5f69 6e69 745f 5f13 0000 0073  ...__init__....s
-000002e0: 0600 0000 0601 0601 0a01 7a16 4d6f 6f41  ..........z.MooA
-000002f0: 7574 6843 6c69 656e 742e 5f5f 696e 6974  uthClient.__init
-00000300: 5f5f 6303 0000 0000 0000 0000 0000 0009  __c.............
-00000310: 0000 0004 0000 00c3 0000 0073 8e00 0000  ...........s....
-00000320: 8101 7400 7c01 8301 5c02 7d03 7d04 6401  ..t.|...\.}.}.d.
-00000330: 7d05 6401 7d06 7401 8300 7d07 7402 7c03  }.d.}.t...}.t.|.
-00000340: 6402 7c04 8303 a003 6403 7c07 a102 a004  d.|.....d.|.....
-00000350: 7c00 6a05 a101 7d08 7c05 7c02 6404 3c00  |.j...}.|.|.d.<.
-00000360: 7c07 7c02 6403 3c00 7c03 7c02 6405 3c00  |.|.d.<.|.|.d.<.
-00000370: 7c06 7c02 6406 3c00 6407 7c00 6a06 9b00  |.|.d.<.d.|.j...
-00000380: 9d02 7c02 6408 3c00 7c08 7c02 6409 3c00  ..|.d.<.|.|.d.<.
-00000390: 7407 7c02 640a 3c00 7c00 6a08 6a09 7c01  t.|.d.<.|.j.j.|.
-000003a0: 7c02 640b 8d02 4900 6400 4800 5300 290c  |.d...I.d.H.S.).
-000003b0: 4efa 1961 7070 6c69 6361 7469 6f6e 2f61  N..application/a
-000003c0: 6374 6976 6974 792b 6a73 6f6e da03 6765  ctivity+json..ge
-000003d0: 74da 0464 6174 65da 0661 6363 6570 74da  t..date..accept.
-000003e0: 0468 6f73 74fa 0c63 6f6e 7465 6e74 2d74  .host..content-t
-000003f0: 7970 65fa 0b4d 6f6f 2d41 7574 682d 3120  ype..Moo-Auth-1 
-00000400: da0d 6175 7468 6f72 697a 6174 696f 6efa  ..authorization.
-00000410: 0f78 2d6d 6f6f 2d73 6967 6e61 7475 7265  .x-moo-signature
-00000420: fa0a 7573 6572 2d61 6765 6e74 a901 da07  ..user-agent....
-00000430: 6865 6164 6572 7329 0a72 1000 0000 7205  headers).r....r.
-00000440: 0000 0072 0400 0000 da0a 7769 7468 5f66  ...r......with_f
-00000450: 6965 6c64 da0c 6564 3235 3531 395f 7369  ield..ed25519_si
-00000460: 676e 7214 0000 0072 1300 0000 7207 0000  gnr....r....r...
-00000470: 0072 1200 0000 7218 0000 0029 0972 1500  .r....r....).r..
-00000480: 0000 720c 0000 0072 2200 0000 721b 0000  ..r....r"...r...
-00000490: 00da 0674 6172 6765 7472 1a00 0000 da0c  ...targetr......
-000004a0: 636f 6e74 656e 745f 7479 7065 da0b 6461  content_type..da
-000004b0: 7465 5f68 6561 6465 72da 1073 6967 6e61  te_header..signa
-000004c0: 7475 7265 5f68 6561 6465 7272 0e00 0000  ture_headerr....
-000004d0: 720e 0000 0072 0f00 0000 7218 0000 0019  r....r....r.....
-000004e0: 0000 0073 2200 0000 0280 0c01 0402 0401  ...s"...........
-000004f0: 0601 0a03 0801 0801 02fd 0806 0801 0801  ................
-00000500: 0801 1001 0801 0801 1602 7a11 4d6f 6f41  ..........z.MooA
-00000510: 7574 6843 6c69 656e 742e 6765 744e 6305  uthClient.getNc.
-00000520: 0000 0000 0000 0000 0000 000b 0000 0005  ................
-00000530: 0000 00c3 0000 0073 b000 0000 8101 7400  .......s......t.
-00000540: 7c01 8301 5c02 7d05 7d06 6401 7d07 7c04  |...\.}.}.d.}.|.
-00000550: 6400 7500 720f 6401 7d04 7401 8300 7d08  d.u.r.d.}.t...}.
-00000560: 7402 7c02 8301 7d09 7403 7c05 6402 7c06  t.|...}.t.|.d.|.
-00000570: 8303 a004 6403 7c08 a102 a004 6404 7c09  ....d.|.....d.|.
-00000580: a102 a005 7c00 6a06 a101 7d0a 7c07 7c03  ....|.j...}.|.|.
-00000590: 6405 3c00 7c09 7c03 6404 3c00 7c08 7c03  d.<.|.|.d.<.|.|.
-000005a0: 6403 3c00 7c05 7c03 6406 3c00 7c04 7c03  d.<.|.|.d.<.|.|.
-000005b0: 6407 3c00 6408 7c00 6a07 9b00 9d02 7c03  d.<.d.|.j.....|.
-000005c0: 6409 3c00 7c0a 7c03 640a 3c00 7408 7c03  d.<.|.|.d.<.t.|.
-000005d0: 640b 3c00 7c00 6a09 6a0a 7c01 7c02 7c03  d.<.|.j.j.|.|.|.
-000005e0: 640c 8d03 4900 6400 4800 5300 290d 4e72  d...I.d.H.S.).Nr
-000005f0: 1700 0000 da04 706f 7374 7219 0000 00da  ......postr.....
-00000600: 0664 6967 6573 7472 1a00 0000 721b 0000  .digestr....r...
-00000610: 0072 1c00 0000 721d 0000 0072 1e00 0000  .r....r....r....
-00000620: 721f 0000 0072 2000 0000 2902 da04 6461  r....r ...)...da
-00000630: 7461 7222 0000 0029 0b72 1000 0000 7205  tar"...).r....r.
-00000640: 0000 0072 0300 0000 7204 0000 0072 2300  ...r....r....r#.
-00000650: 0000 7224 0000 0072 1400 0000 7213 0000  ..r$...r....r...
-00000660: 0072 0700 0000 7212 0000 0072 2900 0000  .r....r....r)...
-00000670: 290b 7215 0000 0072 0c00 0000 da04 626f  ).r....r......bo
-00000680: 6479 7222 0000 0072 2600 0000 721b 0000  dyr"...r&...r...
-00000690: 0072 2500 0000 721a 0000 0072 2700 0000  .r%...r....r'...
-000006a0: 722a 0000 0072 2800 0000 720e 0000 0072  r*...r(...r....r
-000006b0: 0e00 0000 720f 0000 0072 2900 0000 3000  ....r....r)...0.
-000006c0: 0000 732a 0000 0002 800c 0104 0108 0204  ..s*............
-000006d0: 0106 0108 020a 0308 0108 0108 0102 fc08  ................
-000006e0: 0708 0108 0208 0108 0110 0108 0108 0118  ................
-000006f0: 027a 124d 6f6f 4175 7468 436c 6965 6e74  .z.MooAuthClient
-00000700: 2e70 6f73 7463 0300 0000 0000 0000 0000  .postc..........
-00000710: 0000 0800 0000 0500 0000 4300 0000 737a  ..........C...sz
-00000720: 0000 0074 007c 0183 015c 027d 037d 0474  ...t.|...\.}.}.t
-00000730: 0183 007d 0564 017d 0674 027c 0364 027c  ...}.d.}.t.|.d.|
-00000740: 0483 03a0 0364 037c 05a1 02a0 047c 006a  .....d.|.....|.j
-00000750: 05a1 017d 077c 067c 0264 043c 007c 057c  ...}.|.|.d.<.|.|
-00000760: 0264 033c 007c 037c 0264 053c 0064 067c  .d.<.|.|.d.<.d.|
-00000770: 006a 069b 009d 027c 0264 073c 007c 077c  .j.....|.d.<.|.|
-00000780: 0264 083c 0074 077c 0264 093c 0074 087c  .d.<.t.|.d.<.t.|
-00000790: 006a 097c 017c 0264 0a8d 0353 0029 0b4e  .j.|.|.d...S.).N
-000007a0: 7a11 7465 7874 2f65 7665 6e74 2d73 7472  z.text/event-str
-000007b0: 6561 6d72 1800 0000 7219 0000 0072 1a00  eamr....r....r..
-000007c0: 0000 721b 0000 0072 1d00 0000 721e 0000  ..r....r....r...
-000007d0: 0072 1f00 0000 7220 0000 0072 2100 0000  .r....r ...r!...
-000007e0: 290a 7210 0000 0072 0500 0000 7204 0000  ).r....r....r...
-000007f0: 0072 2300 0000 7224 0000 0072 1400 0000  .r#...r$...r....
-00000800: 7213 0000 0072 0700 0000 7208 0000 0072  r....r....r....r
-00000810: 1200 0000 2908 7215 0000 0072 0c00 0000  ....).r....r....
-00000820: 7222 0000 0072 1b00 0000 7225 0000 0072  r"...r....r%...r
-00000830: 2700 0000 721a 0000 0072 2800 0000 720e  '...r....r(...r.
-00000840: 0000 0072 0e00 0000 720f 0000 00da 0c65  ...r....r......e
-00000850: 7665 6e74 5f73 6f75 7263 654d 0000 0073  vent_sourceM...s
-00000860: 1c00 0000 0c01 0601 0401 0a02 0801 0801  ................
-00000870: 02fd 0806 0801 0801 1001 0801 0801 1002  ................
-00000880: 7a1a 4d6f 6f41 7574 6843 6c69 656e 742e  z.MooAuthClient.
-00000890: 6576 656e 745f 736f 7572 6365 2907 da08  event_source)...
-000008a0: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
-000008b0: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
-000008c0: 5f5f 7216 0000 0072 1800 0000 7229 0000  __r....r....r)..
-000008d0: 0072 2d00 0000 720e 0000 0072 0e00 0000  .r-...r....r....
-000008e0: 720e 0000 0072 0f00 0000 7211 0000 0012  r....r....r.....
-000008f0: 0000 0073 0a00 0000 0800 0801 0c06 0e17  ...s............
-00000900: 101d 7211 0000 004e 290e da0c 7572 6c6c  ..r....N)...urll
-00000910: 6962 2e70 6172 7365 7202 0000 005a 1462  ib.parser....Z.b
-00000920: 6f76 696e 652e 6372 7970 746f 2e68 656c  ovine.crypto.hel
-00000930: 7065 7272 0300 0000 5a1c 626f 7669 6e65  perr....Z.bovine
-00000940: 2e63 7279 7074 6f2e 6874 7470 5f73 6967  .crypto.http_sig
-00000950: 6e61 7475 7265 7204 0000 005a 1162 6f76  naturer....Z.bov
-00000960: 696e 652e 7574 696c 732e 6461 7465 7205  ine.utils.dater.
-00000970: 0000 00da 0663 6f6e 7374 7372 0700 0000  .....constsr....
-00000980: 722d 0000 0072 0800 0000 7210 0000 0072  r-...r....r....r
-00000990: 1100 0000 720e 0000 0072 0e00 0000 720e  ....r....r....r.
-000009a0: 0000 0072 0f00 0000 da08 3c6d 6f64 756c  ...r......<modul
-000009b0: 653e 0100 0000 7310 0000 000c 000c 020c  e>....s.........
-000009c0: 010c 010c 020c 0108 0512 05              ...........
+00000180: 6465 6265 7267 2e6f 7267 2f62 6f76 696e  deberg.org/bovin
+00000190: 652f 626f 7669 6e65 2f62 6f76 696e 652f  e/bovine/bovine/
+000001a0: 626f 7669 6e65 2f63 6c69 656e 7473 2f6d  bovine/clients/m
+000001b0: 6f6f 5f61 7574 685f 636c 6965 6e74 2e70  oo_auth_client.p
+000001c0: 79da 1468 6f73 745f 7461 7267 6574 5f66  y..host_target_f
+000001d0: 726f 6d5f 7572 6c0d 0000 0073 0400 0000  rom_url....s....
+000001e0: 0801 0c01 7210 0000 0063 0000 0000 0000  ....r....c......
+000001f0: 0000 0000 0000 0000 0000 0300 0000 4000  ..............@.
+00000200: 0000 733a 0000 0065 005a 0164 005a 0264  ..s:...e.Z.d.Z.d
+00000210: 0164 0284 005a 0369 0066 0164 0364 0484  .d...Z.i.f.d.d..
+00000220: 015a 0469 0064 0566 0264 0664 0784 015a  .Z.i.d.f.d.d...Z
+00000230: 0569 0066 0164 0864 0984 015a 0664 0553  .i.f.d.d...Z.d.S
+00000240: 0029 0ada 0d4d 6f6f 4175 7468 436c 6965  .)...MooAuthClie
+00000250: 6e74 6304 0000 0000 0000 0000 0000 0004  ntc.............
+00000260: 0000 0002 0000 0043 0000 0073 1600 0000  .......C...s....
+00000270: 7c01 7c00 5f00 7c02 7c00 5f01 7c03 7c00  |.|._.|.|._.|.|.
+00000280: 5f02 6400 5300 7209 0000 0029 03da 0773  _.d.S.r....)...s
+00000290: 6573 7369 6f6e da07 6469 645f 6b65 79da  ession..did_key.
+000002a0: 0b70 7269 7661 7465 5f6b 6579 2904 da04  .private_key)...
+000002b0: 7365 6c66 7212 0000 0072 1300 0000 7214  selfr....r....r.
+000002c0: 0000 0072 0e00 0000 720e 0000 0072 0f00  ...r....r....r..
+000002d0: 0000 da08 5f5f 696e 6974 5f5f 1300 0000  ....__init__....
+000002e0: 7306 0000 0006 0106 010a 017a 164d 6f6f  s..........z.Moo
+000002f0: 4175 7468 436c 6965 6e74 2e5f 5f69 6e69  AuthClient.__ini
+00000300: 745f 5f63 0300 0000 0000 0000 0000 0000  t__c............
+00000310: 0900 0000 0400 0000 c300 0000 738e 0000  ............s...
+00000320: 0081 0174 007c 0183 015c 027d 037d 0464  ...t.|...\.}.}.d
+00000330: 017d 0564 017d 0674 0183 007d 0774 027c  .}.d.}.t...}.t.|
+00000340: 0364 027c 0483 03a0 0364 037c 07a1 02a0  .d.|.....d.|....
+00000350: 047c 006a 05a1 017d 087c 057c 0264 043c  .|.j...}.|.|.d.<
+00000360: 007c 077c 0264 033c 007c 037c 0264 053c  .|.|.d.<.|.|.d.<
+00000370: 007c 067c 0264 063c 0064 077c 006a 069b  .|.|.d.<.d.|.j..
+00000380: 009d 027c 0264 083c 007c 087c 0264 093c  ...|.d.<.|.|.d.<
+00000390: 0074 077c 0264 0a3c 007c 006a 086a 097c  .t.|.d.<.|.j.j.|
+000003a0: 017c 0264 0b8d 0249 0064 0048 0053 0029  .|.d...I.d.H.S.)
+000003b0: 0c4e fa19 6170 706c 6963 6174 696f 6e2f  .N..application/
+000003c0: 6163 7469 7669 7479 2b6a 736f 6eda 0367  activity+json..g
+000003d0: 6574 da04 6461 7465 da06 6163 6365 7074  et..date..accept
+000003e0: da04 686f 7374 fa0c 636f 6e74 656e 742d  ..host..content-
+000003f0: 7479 7065 fa0b 4d6f 6f2d 4175 7468 2d31  type..Moo-Auth-1
+00000400: 20da 0d61 7574 686f 7269 7a61 7469 6f6e   ..authorization
+00000410: fa0f 782d 6d6f 6f2d 7369 676e 6174 7572  ..x-moo-signatur
+00000420: 65fa 0a75 7365 722d 6167 656e 74a9 01da  e..user-agent...
+00000430: 0768 6561 6465 7273 290a 7210 0000 0072  .headers).r....r
+00000440: 0500 0000 7204 0000 00da 0a77 6974 685f  ....r......with_
+00000450: 6669 656c 64da 0c65 6432 3535 3139 5f73  field..ed25519_s
+00000460: 6967 6e72 1400 0000 7213 0000 0072 0700  ignr....r....r..
+00000470: 0000 7212 0000 0072 1800 0000 2909 7215  ..r....r....).r.
+00000480: 0000 0072 0c00 0000 7222 0000 0072 1b00  ...r....r"...r..
+00000490: 0000 da06 7461 7267 6574 721a 0000 00da  ....targetr.....
+000004a0: 0c63 6f6e 7465 6e74 5f74 7970 65da 0b64  .content_type..d
+000004b0: 6174 655f 6865 6164 6572 da10 7369 676e  ate_header..sign
+000004c0: 6174 7572 655f 6865 6164 6572 720e 0000  ature_headerr...
+000004d0: 0072 0e00 0000 720f 0000 0072 1800 0000  .r....r....r....
+000004e0: 1900 0000 7322 0000 0002 800c 0104 0204  ....s"..........
+000004f0: 0106 010a 0308 0108 0102 fd08 0608 0108  ................
+00000500: 0108 0110 0108 0108 0116 027a 114d 6f6f  ...........z.Moo
+00000510: 4175 7468 436c 6965 6e74 2e67 6574 4e63  AuthClient.getNc
+00000520: 0500 0000 0000 0000 0000 0000 0b00 0000  ................
+00000530: 0500 0000 c300 0000 73b0 0000 0081 0174  ........s......t
+00000540: 007c 0183 015c 027d 057d 0664 017d 077c  .|...\.}.}.d.}.|
+00000550: 0464 0075 0072 0f64 017d 0474 0183 007d  .d.u.r.d.}.t...}
+00000560: 0874 027c 0283 017d 0974 037c 0564 027c  .t.|...}.t.|.d.|
+00000570: 0683 03a0 0464 037c 08a1 02a0 0464 047c  .....d.|.....d.|
+00000580: 09a1 02a0 057c 006a 06a1 017d 0a7c 077c  .....|.j...}.|.|
+00000590: 0364 053c 007c 097c 0364 043c 007c 087c  .d.<.|.|.d.<.|.|
+000005a0: 0364 033c 007c 057c 0364 063c 007c 047c  .d.<.|.|.d.<.|.|
+000005b0: 0364 073c 0064 087c 006a 079b 009d 027c  .d.<.d.|.j.....|
+000005c0: 0364 093c 007c 0a7c 0364 0a3c 0074 087c  .d.<.|.|.d.<.t.|
+000005d0: 0364 0b3c 007c 006a 096a 0a7c 017c 027c  .d.<.|.j.j.|.|.|
+000005e0: 0364 0c8d 0349 0064 0048 0053 0029 0d4e  .d...I.d.H.S.).N
+000005f0: 7217 0000 00da 0470 6f73 7472 1900 0000  r......postr....
+00000600: da06 6469 6765 7374 721a 0000 0072 1b00  ..digestr....r..
+00000610: 0000 721c 0000 0072 1d00 0000 721e 0000  ..r....r....r...
+00000620: 0072 1f00 0000 7220 0000 0029 02da 0464  .r....r ...)...d
+00000630: 6174 6172 2200 0000 290b 7210 0000 0072  atar"...).r....r
+00000640: 0500 0000 7203 0000 0072 0400 0000 7223  ....r....r....r#
+00000650: 0000 0072 2400 0000 7214 0000 0072 1300  ...r$...r....r..
+00000660: 0000 7207 0000 0072 1200 0000 7229 0000  ..r....r....r)..
+00000670: 0029 0b72 1500 0000 720c 0000 00da 0462  .).r....r......b
+00000680: 6f64 7972 2200 0000 7226 0000 0072 1b00  odyr"...r&...r..
+00000690: 0000 7225 0000 0072 1a00 0000 7227 0000  ..r%...r....r'..
+000006a0: 0072 2a00 0000 7228 0000 0072 0e00 0000  .r*...r(...r....
+000006b0: 720e 0000 0072 0f00 0000 7229 0000 0030  r....r....r)...0
+000006c0: 0000 0073 2a00 0000 0280 0c01 0401 0802  ...s*...........
+000006d0: 0401 0601 0802 0a03 0801 0801 0801 02fc  ................
+000006e0: 0807 0801 0802 0801 0801 1001 0801 0801  ................
+000006f0: 1802 7a12 4d6f 6f41 7574 6843 6c69 656e  ..z.MooAuthClien
+00000700: 742e 706f 7374 6303 0000 0000 0000 0000  t.postc.........
+00000710: 0000 0008 0000 0005 0000 0043 0000 0073  ...........C...s
+00000720: 7a00 0000 7400 7c01 8301 5c02 7d03 7d04  z...t.|...\.}.}.
+00000730: 7401 8300 7d05 6401 7d06 7402 7c03 6402  t...}.d.}.t.|.d.
+00000740: 7c04 8303 a003 6403 7c05 a102 a004 7c00  |.....d.|.....|.
+00000750: 6a05 a101 7d07 7c06 7c02 6404 3c00 7c05  j...}.|.|.d.<.|.
+00000760: 7c02 6403 3c00 7c03 7c02 6405 3c00 6406  |.d.<.|.|.d.<.d.
+00000770: 7c00 6a06 9b00 9d02 7c02 6407 3c00 7c07  |.j.....|.d.<.|.
+00000780: 7c02 6408 3c00 7407 7c02 6409 3c00 7408  |.d.<.t.|.d.<.t.
+00000790: 7c00 6a09 7c01 7c02 640a 8d03 5300 290b  |.j.|.|.d...S.).
+000007a0: 4e7a 1174 6578 742f 6576 656e 742d 7374  Nz.text/event-st
+000007b0: 7265 616d 7218 0000 0072 1900 0000 721a  reamr....r....r.
+000007c0: 0000 0072 1b00 0000 721d 0000 0072 1e00  ...r....r....r..
+000007d0: 0000 721f 0000 0072 2000 0000 7221 0000  ..r....r ...r!..
+000007e0: 0029 0a72 1000 0000 7205 0000 0072 0400  .).r....r....r..
+000007f0: 0000 7223 0000 0072 2400 0000 7214 0000  ..r#...r$...r...
+00000800: 0072 1300 0000 7207 0000 0072 0800 0000  .r....r....r....
+00000810: 7212 0000 0029 0872 1500 0000 720c 0000  r....).r....r...
+00000820: 0072 2200 0000 721b 0000 0072 2500 0000  .r"...r....r%...
+00000830: 7227 0000 0072 1a00 0000 7228 0000 0072  r'...r....r(...r
+00000840: 0e00 0000 720e 0000 0072 0f00 0000 da0c  ....r....r......
+00000850: 6576 656e 745f 736f 7572 6365 4d00 0000  event_sourceM...
+00000860: 731c 0000 000c 0106 0104 010a 0208 0108  s...............
+00000870: 0102 fd08 0608 0108 0110 0108 0108 0110  ................
+00000880: 027a 1a4d 6f6f 4175 7468 436c 6965 6e74  .z.MooAuthClient
+00000890: 2e65 7665 6e74 5f73 6f75 7263 6529 07da  .event_source)..
+000008a0: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
+000008b0: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
+000008c0: 655f 5f72 1600 0000 7218 0000 0072 2900  e__r....r....r).
+000008d0: 0000 722d 0000 0072 0e00 0000 720e 0000  ..r-...r....r...
+000008e0: 0072 0e00 0000 720f 0000 0072 1100 0000  .r....r....r....
+000008f0: 1200 0000 730a 0000 0008 0008 010c 060e  ....s...........
+00000900: 1710 1d72 1100 0000 4e29 0eda 0c75 726c  ...r....N)...url
+00000910: 6c69 622e 7061 7273 6572 0200 0000 5a14  lib.parser....Z.
+00000920: 626f 7669 6e65 2e63 7279 7074 6f2e 6865  bovine.crypto.he
+00000930: 6c70 6572 7203 0000 005a 1c62 6f76 696e  lperr....Z.bovin
+00000940: 652e 6372 7970 746f 2e68 7474 705f 7369  e.crypto.http_si
+00000950: 676e 6174 7572 6572 0400 0000 5a11 626f  gnaturer....Z.bo
+00000960: 7669 6e65 2e75 7469 6c73 2e64 6174 6572  vine.utils.dater
+00000970: 0500 0000 da06 636f 6e73 7473 7207 0000  ......constsr...
+00000980: 0072 2d00 0000 7208 0000 0072 1000 0000  .r-...r....r....
+00000990: 7211 0000 0072 0e00 0000 720e 0000 0072  r....r....r....r
+000009a0: 0e00 0000 720f 0000 00da 083c 6d6f 6475  ....r......<modu
+000009b0: 6c65 3e01 0000 0073 1000 0000 0c00 0c02  le>....s........
+000009c0: 0c01 0c01 0c02 0c01 0805 1205            ............
```

### Comparing `bovine-0.1.0/bovine/clients/__pycache__/nodeinfo.cpython-310.pyc` & `bovine-0.1.1/bovine/clients/__pycache__/nodeinfo.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 13 15:55:57 2023 UTC, .py size: 1399 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 15% similar despite different names*

```diff
@@ -1,97 +1,78 @@
-00000000: 6f0d 0d0a 0000 0000 0d26 3864 7705 0000  o........&8dw...
+00000000: 6f0d 0d0a 0000 0000 a4ea 3a64 b403 0000  o.........:d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0007 0000 0040 0000 0073 7200 0000 6400  .....@...sr...d.
+00000020: 0007 0000 0040 0000 0073 6e00 0000 6400  .....@...sn...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6402  d.l.Z.d.d.l.Z.d.
 00000050: 6403 6c04 6d05 5a05 0100 6501 a006 6507  d.l.m.Z...e...e.
 00000060: a101 5a08 6404 6503 6a09 6405 650a 6406  ..Z.d.e.j.d.e.d.
-00000070: 650b 6401 4200 6606 6407 6408 8404 5a0c  e.d.B.f.d.d...Z.
-00000080: 6404 6503 6a09 6409 650a 6406 650b 6401  d.e.j.d.e.d.e.d.
-00000090: 4200 6606 640a 640b 8404 5a0d 6401 5300  B.f.d.d...Z.d.S.
-000000a0: 290c e900 0000 004e e901 0000 0029 01da  )......N.....)..
-000000b0: 1242 4f56 494e 455f 434c 4945 4e54 5f4e  .BOVINE_CLIENT_N
-000000c0: 414d 45da 0773 6573 7369 6f6e da06 646f  AME..session..do
-000000d0: 6d61 696e da06 7265 7475 726e 6302 0000  main..returnc...
-000000e0: 0000 0000 0000 0000 0009 0000 000a 0000  ................
-000000f0: 00c3 0000 0073 fa00 0000 8101 7a53 6401  .....s......zSd.
-00000100: 7c01 9b00 6402 9d03 7d02 7c00 6a00 7c02  |...d...}.|.j.|.
-00000110: 6403 7401 6901 6404 6405 8d03 3400 4900  d.t.i.d.d...4.I.
-00000120: 6400 4800 9a17 7d03 7c03 a002 a100 4900  d.H...}.|.....I.
-00000130: 6400 4800 7d04 7403 a004 7c04 a101 7d05  d.H.}.t...|...}.
-00000140: 5700 6400 0400 0400 8303 4900 6400 4800  W.d.......I.d.H.
-00000150: 0100 6e0b 3100 4900 6400 4800 7333 7701  ..n.1.I.d.H.s3w.
-00000160: 0100 0100 0100 5900 0100 7c05 6406 1900  ......Y...|.d...
-00000170: 4400 5d15 7d06 7c06 6407 1900 6408 6b02  D.].}.|.d...d.k.
-00000180: 7251 7405 7c00 7c06 6409 1900 8302 4900  rQt.|.|.d.....I.
-00000190: 6400 4800 0200 0100 5700 5300 713c 5700  d.H.....W.S.q<W.
-000001a0: 6400 5300 0400 7406 797c 0100 7d07 0100  d.S...t.y|..}...
-000001b0: 7a1c 7407 a008 7409 7c07 8301 a101 0100  z.t...t.|.......
-000001c0: 740a a00b a100 a00c a100 4400 5d07 7d08  t.........D.].}.
-000001d0: 7407 a008 7c08 a101 0100 7169 5700 5900  t...|.....qiW.Y.
-000001e0: 6400 7d07 7e07 6400 5300 6400 7d07 7e07  d.}.~.d.S.d.}.~.
-000001f0: 7701 7700 290a 4e7a 0868 7474 7073 3a2f  w.w.).Nz.https:/
-00000200: 2f7a 152f 2e77 656c 6c2d 6b6e 6f77 6e2f  /z./.well-known/
-00000210: 6e6f 6465 696e 666f fa0a 7573 6572 2d61  nodeinfo..user-a
-00000220: 6765 6e74 e93c 0000 0029 02da 0768 6561  gent.<...)...hea
-00000230: 6465 7273 da07 7469 6d65 6f75 74da 056c  ders..timeout..l
-00000240: 696e 6b73 da03 7265 6c7a 2f68 7474 703a  inks..relz/http:
-00000250: 2f2f 6e6f 6465 696e 666f 2e64 6961 7370  //nodeinfo.diasp
-00000260: 6f72 612e 736f 6674 7761 7265 2f6e 732f  ora.software/ns/
-00000270: 7363 6865 6d61 2f32 2e30 da04 6872 6566  schema/2.0..href
-00000280: 290d da03 6765 7472 0300 0000 da04 7465  )...getr......te
-00000290: 7874 da04 6a73 6f6e da05 6c6f 6164 73da  xt..json..loads.
-000002a0: 1066 6574 6368 5f6e 6f64 6569 6e66 6f32  .fetch_nodeinfo2
-000002b0: 30da 0945 7863 6570 7469 6f6e da06 6c6f  0..Exception..lo
-000002c0: 6767 6572 da05 6572 726f 72da 0373 7472  gger..error..str
-000002d0: da09 7472 6163 6562 6163 6bda 0a66 6f72  ..traceback..for
-000002e0: 6d61 745f 6578 63da 0a73 706c 6974 6c69  mat_exc..splitli
-000002f0: 6e65 7329 0972 0400 0000 7205 0000 005a  nes).r....r....Z
-00000300: 1677 656c 6c6b 6e6f 776e 5f6e 6f64 6569  .wellknown_nodei
-00000310: 6e66 6f5f 7572 6cda 0872 6573 706f 6e73  nfo_url..respons
-00000320: 6572 0f00 0000 da04 6461 7461 da04 6c69  er......data..li
-00000330: 6e6b da01 65da 086c 6f67 5f6c 696e 65a9  nk..e..log_line.
-00000340: 0072 1f00 0000 fa4b 2f77 6f6f 6470 6563  .r.....K/woodpec
-00000350: 6b65 722f 7372 632f 636f 6465 6265 7267  ker/src/codeberg
-00000360: 2e6f 7267 2f68 656c 6765 2f62 6f76 696e  .org/helge/bovin
-00000370: 652f 626f 7669 6e65 2f62 6f76 696e 652f  e/bovine/bovine/
-00000380: 636c 6965 6e74 732f 6e6f 6465 696e 666f  clients/nodeinfo
-00000390: 2e70 79da 0e66 6574 6368 5f6e 6f64 6569  .py..fetch_nodei
-000003a0: 6e66 6f0c 0000 0073 3000 0000 0280 0201  nfo....s0.......
-000003b0: 0c01 0402 0201 0601 0201 0efd 0204 0e01  ................
-000003c0: 0c01 28fa 0c08 0c01 1a01 02ff 0603 0e02  ..(.............
-000003d0: 0e01 1001 0c01 0e01 0880 02fc 7221 0000  ............r!..
-000003e0: 00da 0375 726c 6302 0000 0000 0000 0000  ...urlc.........
-000003f0: 0000 0006 0000 000a 0000 00c3 0000 0073  ...............s
-00000400: ba00 0000 8101 7a33 7c00 6a00 7c01 6401  ......z3|.j.|.d.
-00000410: 7401 6901 6402 8d02 3400 4900 6400 4800  t.i.d...4.I.d.H.
-00000420: 9a18 7d02 7c02 a002 a100 4900 6400 4800  ..}.|.....I.d.H.
-00000430: 7d03 7403 a004 7c03 a101 5700 0200 6400  }.t...|...W...d.
-00000440: 0400 0400 8303 4900 6400 4800 0100 5700  ......I.d.H...W.
-00000450: 5300 3100 4900 6400 4800 732d 7701 0100  S.1.I.d.H.s-w...
-00000460: 0100 0100 5900 0100 5700 6400 5300 0400  ....Y...W.d.S...
-00000470: 7405 795c 0100 7d04 0100 7a1c 7406 a007  t.y\..}...z.t...
-00000480: 7408 7c04 8301 a101 0100 7409 a00a a100  t.|.......t.....
-00000490: a00b a100 4400 5d07 7d05 7406 a007 7c05  ....D.].}.t...|.
-000004a0: a101 0100 7149 5700 5900 6400 7d04 7e04  ....qIW.Y.d.}.~.
-000004b0: 6400 5300 6400 7d04 7e04 7701 7700 2903  d.S.d.}.~.w.w.).
-000004c0: 4e72 0700 0000 2901 7209 0000 0029 0c72  Nr....).r....).r
-000004d0: 0e00 0000 7203 0000 0072 0f00 0000 7210  ....r....r....r.
-000004e0: 0000 0072 1100 0000 7213 0000 0072 1400  ...r....r....r..
-000004f0: 0000 7215 0000 0072 1600 0000 7217 0000  ..r....r....r...
-00000500: 0072 1800 0000 7219 0000 0029 0672 0400  .r....r....).r..
-00000510: 0000 7222 0000 0072 1a00 0000 720f 0000  ..r"...r....r...
-00000520: 0072 1d00 0000 721e 0000 0072 1f00 0000  .r....r....r....
-00000530: 721f 0000 0072 2000 0000 7212 0000 0025  r....r ...r....%
-00000540: 0000 0073 2000 0000 0280 0201 0401 0801  ...s ...........
-00000550: 0eff 0202 0e01 0801 34fc 0e06 0e01 1001  ........4.......
-00000560: 0c01 0e01 0880 02fc 7212 0000 0029 0e72  ........r....).r
-00000570: 1000 0000 da07 6c6f 6767 696e 6772 1700  ......loggingr..
-00000580: 0000 da07 6169 6f68 7474 70da 0663 6f6e  ....aiohttp..con
-00000590: 7374 7372 0300 0000 da09 6765 744c 6f67  stsr......getLog
-000005a0: 6765 72da 085f 5f6e 616d 655f 5f72 1400  ger..__name__r..
-000005b0: 0000 da0d 436c 6965 6e74 5365 7373 696f  ....ClientSessio
-000005c0: 6e72 1600 0000 da04 6469 6374 7221 0000  nr......dictr!..
-000005d0: 0072 1200 0000 721f 0000 0072 1f00 0000  .r....r....r....
-000005e0: 721f 0000 0072 2000 0000 da08 3c6d 6f64  r....r .....<mod
-000005f0: 756c 653e 0100 0000 7310 0000 0008 0008  ule>....s.......
-00000600: 0108 0108 020c 020a 021c 0320 19         ........... .
+00000070: 650b 6606 6407 6408 8404 5a0c 6404 6503  e.f.d.d...Z.d.e.
+00000080: 6a09 6409 650a 6406 650b 6401 4200 6606  j.d.e.d.e.d.B.f.
+00000090: 640a 640b 8404 5a0d 6401 5300 290c e900  d.d...Z.d.S.)...
+000000a0: 0000 004e e901 0000 0029 01da 1242 4f56  ...N.....)...BOV
+000000b0: 494e 455f 434c 4945 4e54 5f4e 414d 45da  INE_CLIENT_NAME.
+000000c0: 0773 6573 7369 6f6e da06 646f 6d61 696e  .session..domain
+000000d0: da06 7265 7475 726e 6302 0000 0000 0000  ..returnc.......
+000000e0: 0000 0000 0004 0000 0009 0000 00c3 0000  ................
+000000f0: 0073 6800 0000 8101 6401 7c01 9b00 6402  .sh.....d.|...d.
+00000100: 9d03 7d02 7c00 6a00 7c02 6403 7401 6901  ..}.|.j.|.d.t.i.
+00000110: 6404 6405 8d03 3400 4900 6400 4800 9a12  d.d...4.I.d.H...
+00000120: 7d03 7c03 a002 a100 4900 6400 4800 5700  }.|.....I.d.H.W.
+00000130: 0200 6400 0400 0400 8303 4900 6400 4800  ..d.......I.d.H.
+00000140: 0100 5300 3100 4900 6400 4800 732d 7701  ..S.1.I.d.H.s-w.
+00000150: 0100 0100 0100 5900 0100 6400 5300 2906  ......Y...d.S.).
+00000160: 4e7a 0868 7474 7073 3a2f 2f7a 152f 2e77  Nz.https://z./.w
+00000170: 656c 6c2d 6b6e 6f77 6e2f 6e6f 6465 696e  ell-known/nodein
+00000180: 666f fa0a 7573 6572 2d61 6765 6e74 e93c  fo..user-agent.<
+00000190: 0000 0029 02da 0768 6561 6465 7273 da07  ...)...headers..
+000001a0: 7469 6d65 6f75 7429 03da 0367 6574 7203  timeout)...getr.
+000001b0: 0000 00da 046a 736f 6e29 0472 0400 0000  .....json).r....
+000001c0: 7205 0000 005a 1677 656c 6c6b 6e6f 776e  r....Z.wellknown
+000001d0: 5f6e 6f64 6569 6e66 6f5f 7572 6cda 0872  _nodeinfo_url..r
+000001e0: 6573 706f 6e73 65a9 0072 0e00 0000 fa4c  esponse..r.....L
+000001f0: 2f77 6f6f 6470 6563 6b65 722f 7372 632f  /woodpecker/src/
+00000200: 636f 6465 6265 7267 2e6f 7267 2f62 6f76  codeberg.org/bov
+00000210: 696e 652f 626f 7669 6e65 2f62 6f76 696e  ine/bovine/bovin
+00000220: 652f 626f 7669 6e65 2f63 6c69 656e 7473  e/bovine/clients
+00000230: 2f6e 6f64 6569 6e66 6f2e 7079 da17 6665  /nodeinfo.py..fe
+00000240: 7463 685f 6e6f 6465 696e 666f 5f64 6f63  tch_nodeinfo_doc
+00000250: 756d 656e 740c 0000 0073 1400 0000 0280  ument....s......
+00000260: 0c01 0402 0201 0601 0201 0efd 0204 0c01  ................
+00000270: 30fb 7210 0000 00da 0375 726c 6302 0000  0.r......urlc...
+00000280: 0000 0000 0000 0000 0006 0000 000a 0000  ................
+00000290: 00c3 0000 0073 ba00 0000 8101 7a33 7c00  .....s......z3|.
+000002a0: 6a00 7c01 6401 7401 6901 6402 8d02 3400  j.|.d.t.i.d...4.
+000002b0: 4900 6400 4800 9a18 7d02 7c02 a002 a100  I.d.H...}.|.....
+000002c0: 4900 6400 4800 7d03 7403 a004 7c03 a101  I.d.H.}.t...|...
+000002d0: 5700 0200 6400 0400 0400 8303 4900 6400  W...d.......I.d.
+000002e0: 4800 0100 5700 5300 3100 4900 6400 4800  H...W.S.1.I.d.H.
+000002f0: 732d 7701 0100 0100 0100 5900 0100 5700  s-w.......Y...W.
+00000300: 6400 5300 0400 7405 795c 0100 7d04 0100  d.S...t.y\..}...
+00000310: 7a1c 7406 a007 7408 7c04 8301 a101 0100  z.t...t.|.......
+00000320: 7409 a00a a100 a00b a100 4400 5d07 7d05  t.........D.].}.
+00000330: 7406 a007 7c05 a101 0100 7149 5700 5900  t...|.....qIW.Y.
+00000340: 6400 7d04 7e04 6400 5300 6400 7d04 7e04  d.}.~.d.S.d.}.~.
+00000350: 7701 7700 2903 4e72 0700 0000 2901 7209  w.w.).Nr....).r.
+00000360: 0000 0029 0c72 0b00 0000 7203 0000 00da  ...).r....r.....
+00000370: 0474 6578 7472 0c00 0000 da05 6c6f 6164  .textr......load
+00000380: 73da 0945 7863 6570 7469 6f6e da06 6c6f  s..Exception..lo
+00000390: 6767 6572 da05 6572 726f 72da 0373 7472  gger..error..str
+000003a0: da09 7472 6163 6562 6163 6bda 0a66 6f72  ..traceback..for
+000003b0: 6d61 745f 6578 63da 0a73 706c 6974 6c69  mat_exc..splitli
+000003c0: 6e65 7329 0672 0400 0000 7211 0000 0072  nes).r....r....r
+000003d0: 0d00 0000 7212 0000 00da 0165 da08 6c6f  ....r......e..lo
+000003e0: 675f 6c69 6e65 720e 0000 0072 0e00 0000  g_liner....r....
+000003f0: 720f 0000 00da 1066 6574 6368 5f6e 6f64  r......fetch_nod
+00000400: 6569 6e66 6f32 3017 0000 0073 2000 0000  einfo20....s ...
+00000410: 0280 0201 0401 0801 0eff 0202 0e01 0801  ................
+00000420: 34fc 0e06 0e01 1001 0c01 0e01 0880 02fc  4...............
+00000430: 721d 0000 0029 0e72 0c00 0000 da07 6c6f  r....).r......lo
+00000440: 6767 696e 6772 1800 0000 da07 6169 6f68  ggingr......aioh
+00000450: 7474 70da 0663 6f6e 7374 7372 0300 0000  ttp..constsr....
+00000460: da09 6765 744c 6f67 6765 72da 085f 5f6e  ..getLogger..__n
+00000470: 616d 655f 5f72 1500 0000 da0d 436c 6965  ame__r......Clie
+00000480: 6e74 5365 7373 696f 6e72 1700 0000 da04  ntSessionr......
+00000490: 6469 6374 7210 0000 0072 1d00 0000 720e  dictr....r....r.
+000004a0: 0000 0072 0e00 0000 720e 0000 0072 0f00  ...r....r....r..
+000004b0: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
+000004c0: 7310 0000 0008 0008 0108 0108 020c 020a  s...............
+000004d0: 0218 0320 0b                             ... .
```

### Comparing `bovine-0.1.0/bovine/clients/__pycache__/signed_http.cpython-310.pyc` & `bovine-0.1.1/bovine/clients/__pycache__/signed_http.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 13 15:55:57 2023 UTC, .py size: 3278 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0d26 3864 ce0c 0000  o........&8d....
+00000000: 6f0d 0d0a 0000 0000 a4ea 3a64 ce0c 0000  o.........:d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000f 0000 0040 0000 0073 e400 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6401 6c03 5a03 6400 6403 6c04  ..d.d.l.Z.d.d.l.
 00000050: 6d05 5a05 0100 6400 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6405 6c08 6d09 5a09 0100 6406  ..d.d.l.m.Z...d.
 00000070: 6407 6c0a 6d0b 5a0b 0100 6406 6408 6c0c  d.l.m.Z...d.d.l.
@@ -53,103 +53,103 @@
 00000340: 0072 1100 0000 290c 7209 0000 0072 0a00  .r....).r....r..
 00000350: 0000 720b 0000 0072 0c00 0000 720d 0000  ..r....r....r...
 00000360: 00da 0a70 6172 7365 645f 7572 6c72 1400  ...parsed_urlr..
 00000370: 0000 da06 7461 7267 6574 7213 0000 00da  ....targetr.....
 00000380: 0c63 6f6e 7465 6e74 5f74 7970 65da 0b64  .content_type..d
 00000390: 6174 655f 6865 6164 6572 da10 7369 676e  ate_header..sign
 000003a0: 6174 7572 655f 6865 6164 6572 a900 7223  ature_header..r#
-000003b0: 0000 00fa 4e2f 776f 6f64 7065 636b 6572  ....N/woodpecker
+000003b0: 0000 00fa 4f2f 776f 6f64 7065 636b 6572  ....O/woodpecker
 000003c0: 2f73 7263 2f63 6f64 6562 6572 672e 6f72  /src/codeberg.or
-000003d0: 672f 6865 6c67 652f 626f 7669 6e65 2f62  g/helge/bovine/b
-000003e0: 6f76 696e 652f 626f 7669 6e65 2f63 6c69  ovine/bovine/cli
-000003f0: 656e 7473 2f73 6967 6e65 645f 6874 7470  ents/signed_http
-00000400: 2e70 79da 0a73 6967 6e65 645f 6765 7410  .py..signed_get.
-00000410: 0000 0073 2800 0000 0280 1607 0802 0601  ...s(...........
-00000420: 0601 0402 0401 0601 0a03 0801 0801 0801  ................
-00000430: 02fc 0807 0801 0801 0801 0801 0801 1401  ................
-00000440: 7225 0000 0063 0500 0000 0000 0000 0000  r%...c..........
-00000450: 0000 0b00 0000 0600 0000 4300 0000 738e  ..........C...s.
-00000460: 0000 0074 00a0 0164 017c 019b 0064 027c  ...t...d.|...d.|
-00000470: 039b 009d 04a1 0101 0074 027c 0383 017d  .........t.|...}
-00000480: 057c 056a 037d 067c 056a 047d 0764 037d  .|.j.}.|.j.}.d.}
-00000490: 0874 0583 007d 0974 067c 0664 047c 0783  .t...}.t.|.d.|..
-000004a0: 03a0 0764 057c 09a1 02a0 0764 067c 08a1  ...d.|.....d.|..
-000004b0: 02a0 067c 017c 02a1 027d 0a7c 087c 0464  ...|.|...}.|.|.d
-000004c0: 063c 007c 097c 0464 053c 007c 067c 0464  .<.|.|.d.<.|.|.d
-000004d0: 073c 007c 0a7c 0464 083c 0074 087c 0464  .<.|.|.d.<.t.|.d
-000004e0: 093c 0074 097c 007c 037c 0464 0a8d 0353  .<.t.|.|.|.d...S
-000004f0: 0029 0b4e 7a19 5369 676e 6564 2065 7665  .).Nz.Signed eve
-00000500: 6e74 2073 6f75 7263 6520 7769 7468 2072  nt source with r
-00000510: 0f00 0000 7a11 7465 7874 2f65 7665 6e74  ....z.text/event
-00000520: 2d73 7472 6561 6d72 1100 0000 7212 0000  -streamr....r...
-00000530: 0072 1300 0000 7214 0000 0072 1600 0000  .r....r....r....
-00000540: 7217 0000 0072 1800 0000 290a 7219 0000  r....r....).r...
-00000550: 0072 1a00 0000 7202 0000 0072 1b00 0000  .r....r....r....
-00000560: 721c 0000 0072 0500 0000 7204 0000 0072  r....r....r....r
-00000570: 1d00 0000 7207 0000 0072 0800 0000 290b  ....r....r....).
-00000580: 7209 0000 0072 0a00 0000 720b 0000 0072  r....r....r....r
-00000590: 0c00 0000 720d 0000 0072 1e00 0000 7214  ....r....r....r.
-000005a0: 0000 0072 1f00 0000 7213 0000 0072 2100  ...r....r....r!.
-000005b0: 0000 7222 0000 0072 2300 0000 7223 0000  ..r"...r#...r#..
-000005c0: 0072 2400 0000 da13 7369 676e 6564 5f65  .r$.....signed_e
-000005d0: 7665 6e74 5f73 6f75 7263 6531 0000 0073  vent_source1...s
-000005e0: 2200 0000 1607 0802 0601 0601 0402 0601  "...............
-000005f0: 0a03 0801 0801 0801 02fc 0807 0801 0801  ................
-00000600: 0801 0801 0e01 7226 0000 00da 0462 6f64  ......r&.....bod
-00000610: 7963 0700 0000 0000 0000 0000 0000 0e00  yc..............
-00000620: 0000 0600 0000 c300 0000 73c4 0000 0081  ..........s.....
-00000630: 0174 00a0 0164 017c 019b 0064 027c 039b  .t...d.|...d.|..
-00000640: 009d 04a1 0101 0074 027c 0383 017d 077c  .......t.|...}.|
-00000650: 076a 037d 087c 076a 047d 0964 037d 0a7c  .j.}.|.j.}.d.}.|
-00000660: 0664 0075 0072 1e64 037d 0674 0583 007d  .d.u.r.d.}.t...}
-00000670: 0b74 067c 0483 017d 0c74 077c 0864 047c  .t.|...}.t.|.d.|
-00000680: 0983 03a0 0864 057c 0ba1 02a0 0864 067c  .....d.|.....d.|
-00000690: 0ca1 02a0 0864 077c 06a1 02a0 077c 017c  .....d.|.....|.|
-000006a0: 02a1 027d 0d7c 0a7c 0564 083c 007c 0c7c  ...}.|.|.d.<.|.|
-000006b0: 0564 063c 007c 0b7c 0564 053c 007c 087c  .d.<.|.|.d.<.|.|
-000006c0: 0564 093c 007c 067c 0564 073c 007c 0d7c  .d.<.|.|.d.<.|.|
-000006d0: 0564 0a3c 0074 097c 0564 0b3c 007c 006a  .d.<.t.|.d.<.|.j
-000006e0: 0a7c 037c 047c 0564 0c8d 0349 0064 0048  .|.|.|.d...I.d.H
-000006f0: 0053 0029 0d4e 7a11 5369 676e 6564 2070  .S.).Nz.Signed p
-00000700: 6f73 7420 7769 7468 2072 0f00 0000 7210  ost with r....r.
-00000710: 0000 00da 0470 6f73 7472 1200 0000 da06  .....postr......
-00000720: 6469 6765 7374 7215 0000 0072 1300 0000  digestr....r....
-00000730: 7214 0000 0072 1600 0000 7217 0000 0029  r....r....r....)
-00000740: 02da 0464 6174 6172 0d00 0000 290b 7219  ...datar....).r.
-00000750: 0000 0072 1a00 0000 7202 0000 0072 1b00  ...r....r....r..
-00000760: 0000 721c 0000 0072 0500 0000 7203 0000  ..r....r....r...
-00000770: 0072 0400 0000 721d 0000 0072 0700 0000  .r....r....r....
-00000780: 7228 0000 0029 0e72 0900 0000 720a 0000  r(...).r....r...
-00000790: 0072 0b00 0000 720c 0000 0072 2700 0000  .r....r....r'...
-000007a0: 720d 0000 0072 2000 0000 721e 0000 0072  r....r ...r....r
-000007b0: 1400 0000 721f 0000 0072 1300 0000 7221  ....r....r....r!
-000007c0: 0000 0072 2900 0000 7222 0000 0072 2300  ...r)...r"...r#.
-000007d0: 0000 7223 0000 0072 2400 0000 da0b 7369  ..r#...r$.....si
-000007e0: 676e 6564 5f70 6f73 7450 0000 0073 3000  gned_postP...s0.
-000007f0: 0000 0280 1609 0802 0601 0601 0402 0802  ................
-00000800: 0401 0601 0802 0a03 0801 0801 0801 0801  ................
-00000810: 02fb 0808 0801 0801 0801 0801 0801 0801  ................
-00000820: 1602 722b 0000 0029 18da 076c 6f67 6769  ..r+...)...loggi
-00000830: 6e67 da0c 7572 6c6c 6962 2e70 6172 7365  ng..urllib.parse
-00000840: 7202 0000 00da 0761 696f 6874 7470 da14  r......aiohttp..
-00000850: 626f 7669 6e65 2e63 7279 7074 6f2e 6865  bovine.crypto.he
-00000860: 6c70 6572 7203 0000 00da 1c62 6f76 696e  lperr......bovin
-00000870: 652e 6372 7970 746f 2e68 7474 705f 7369  e.crypto.http_si
-00000880: 676e 6174 7572 6572 0400 0000 da11 626f  gnaturer......bo
-00000890: 7669 6e65 2e75 7469 6c73 2e64 6174 6572  vine.utils.dater
-000008a0: 0500 0000 da06 636f 6e73 7473 7207 0000  ......constsr...
-000008b0: 00da 0c65 7665 6e74 5f73 6f75 7263 6572  ...event_sourcer
-000008c0: 0800 0000 da09 6765 744c 6f67 6765 72da  ......getLogger.
-000008d0: 085f 5f6e 616d 655f 5f72 1900 0000 da0d  .__name__r......
-000008e0: 436c 6965 6e74 5365 7373 696f 6eda 0373  ClientSession..s
-000008f0: 7472 da04 6469 6374 da0e 436c 6965 6e74  tr..dict..Client
-00000900: 5265 7370 6f6e 7365 7225 0000 0072 2600  Responser%...r&.
-00000910: 0000 722b 0000 0072 2300 0000 7223 0000  ..r+...r#...r#..
-00000920: 0072 2300 0000 7224 0000 00da 083c 6d6f  .r#...r$.....<mo
-00000930: 6475 6c65 3e01 0000 0073 6800 0000 0800  dule>....sh.....
-00000940: 0c01 0802 0c02 0c01 0c01 0c02 0c01 0a02  ................
-00000950: 0208 04fb 0401 02ff 0202 02fe 0203 02fd  ................
-00000960: 0204 02fc 0205 02fb 0406 0afa 0226 04fb  .............&..
-00000970: 0401 02ff 0202 02fe 0203 02fd 0204 02fc  ................
-00000980: 0205 0afb 0225 0201 04f9 0401 02ff 0202  .....%..........
-00000990: 02fe 0203 02fd 0204 02fc 0205 02fb 0206  ................
-000009a0: 02fa 0408 0ef8                           ......
+000003d0: 672f 626f 7669 6e65 2f62 6f76 696e 652f  g/bovine/bovine/
+000003e0: 626f 7669 6e65 2f62 6f76 696e 652f 636c  bovine/bovine/cl
+000003f0: 6965 6e74 732f 7369 676e 6564 5f68 7474  ients/signed_htt
+00000400: 702e 7079 da0a 7369 676e 6564 5f67 6574  p.py..signed_get
+00000410: 1000 0000 7328 0000 0002 8016 0708 0206  ....s(..........
+00000420: 0106 0104 0204 0106 010a 0308 0108 0108  ................
+00000430: 0102 fc08 0708 0108 0108 0108 0108 0114  ................
+00000440: 0172 2500 0000 6305 0000 0000 0000 0000  .r%...c.........
+00000450: 0000 000b 0000 0006 0000 0043 0000 0073  ...........C...s
+00000460: 8e00 0000 7400 a001 6401 7c01 9b00 6402  ....t...d.|...d.
+00000470: 7c03 9b00 9d04 a101 0100 7402 7c03 8301  |.........t.|...
+00000480: 7d05 7c05 6a03 7d06 7c05 6a04 7d07 6403  }.|.j.}.|.j.}.d.
+00000490: 7d08 7405 8300 7d09 7406 7c06 6404 7c07  }.t...}.t.|.d.|.
+000004a0: 8303 a007 6405 7c09 a102 a007 6406 7c08  ....d.|.....d.|.
+000004b0: a102 a006 7c01 7c02 a102 7d0a 7c08 7c04  ....|.|...}.|.|.
+000004c0: 6406 3c00 7c09 7c04 6405 3c00 7c06 7c04  d.<.|.|.d.<.|.|.
+000004d0: 6407 3c00 7c0a 7c04 6408 3c00 7408 7c04  d.<.|.|.d.<.t.|.
+000004e0: 6409 3c00 7409 7c00 7c03 7c04 640a 8d03  d.<.t.|.|.|.d...
+000004f0: 5300 290b 4e7a 1953 6967 6e65 6420 6576  S.).Nz.Signed ev
+00000500: 656e 7420 736f 7572 6365 2077 6974 6820  ent source with 
+00000510: 720f 0000 007a 1174 6578 742f 6576 656e  r....z.text/even
+00000520: 742d 7374 7265 616d 7211 0000 0072 1200  t-streamr....r..
+00000530: 0000 7213 0000 0072 1400 0000 7216 0000  ..r....r....r...
+00000540: 0072 1700 0000 7218 0000 0029 0a72 1900  .r....r....).r..
+00000550: 0000 721a 0000 0072 0200 0000 721b 0000  ..r....r....r...
+00000560: 0072 1c00 0000 7205 0000 0072 0400 0000  .r....r....r....
+00000570: 721d 0000 0072 0700 0000 7208 0000 0029  r....r....r....)
+00000580: 0b72 0900 0000 720a 0000 0072 0b00 0000  .r....r....r....
+00000590: 720c 0000 0072 0d00 0000 721e 0000 0072  r....r....r....r
+000005a0: 1400 0000 721f 0000 0072 1300 0000 7221  ....r....r....r!
+000005b0: 0000 0072 2200 0000 7223 0000 0072 2300  ...r"...r#...r#.
+000005c0: 0000 7224 0000 00da 1373 6967 6e65 645f  ..r$.....signed_
+000005d0: 6576 656e 745f 736f 7572 6365 3100 0000  event_source1...
+000005e0: 7322 0000 0016 0708 0206 0106 0104 0206  s"..............
+000005f0: 010a 0308 0108 0108 0102 fc08 0708 0108  ................
+00000600: 0108 0108 010e 0172 2600 0000 da04 626f  .......r&.....bo
+00000610: 6479 6307 0000 0000 0000 0000 0000 000e  dyc.............
+00000620: 0000 0006 0000 00c3 0000 0073 c400 0000  ...........s....
+00000630: 8101 7400 a001 6401 7c01 9b00 6402 7c03  ..t...d.|...d.|.
+00000640: 9b00 9d04 a101 0100 7402 7c03 8301 7d07  ........t.|...}.
+00000650: 7c07 6a03 7d08 7c07 6a04 7d09 6403 7d0a  |.j.}.|.j.}.d.}.
+00000660: 7c06 6400 7500 721e 6403 7d06 7405 8300  |.d.u.r.d.}.t...
+00000670: 7d0b 7406 7c04 8301 7d0c 7407 7c08 6404  }.t.|...}.t.|.d.
+00000680: 7c09 8303 a008 6405 7c0b a102 a008 6406  |.....d.|.....d.
+00000690: 7c0c a102 a008 6407 7c06 a102 a007 7c01  |.....d.|.....|.
+000006a0: 7c02 a102 7d0d 7c0a 7c05 6408 3c00 7c0c  |...}.|.|.d.<.|.
+000006b0: 7c05 6406 3c00 7c0b 7c05 6405 3c00 7c08  |.d.<.|.|.d.<.|.
+000006c0: 7c05 6409 3c00 7c06 7c05 6407 3c00 7c0d  |.d.<.|.|.d.<.|.
+000006d0: 7c05 640a 3c00 7409 7c05 640b 3c00 7c00  |.d.<.t.|.d.<.|.
+000006e0: 6a0a 7c03 7c04 7c05 640c 8d03 4900 6400  j.|.|.|.d...I.d.
+000006f0: 4800 5300 290d 4e7a 1153 6967 6e65 6420  H.S.).Nz.Signed 
+00000700: 706f 7374 2077 6974 6820 720f 0000 0072  post with r....r
+00000710: 1000 0000 da04 706f 7374 7212 0000 00da  ......postr.....
+00000720: 0664 6967 6573 7472 1500 0000 7213 0000  .digestr....r...
+00000730: 0072 1400 0000 7216 0000 0072 1700 0000  .r....r....r....
+00000740: 2902 da04 6461 7461 720d 0000 0029 0b72  )...datar....).r
+00000750: 1900 0000 721a 0000 0072 0200 0000 721b  ....r....r....r.
+00000760: 0000 0072 1c00 0000 7205 0000 0072 0300  ...r....r....r..
+00000770: 0000 7204 0000 0072 1d00 0000 7207 0000  ..r....r....r...
+00000780: 0072 2800 0000 290e 7209 0000 0072 0a00  .r(...).r....r..
+00000790: 0000 720b 0000 0072 0c00 0000 7227 0000  ..r....r....r'..
+000007a0: 0072 0d00 0000 7220 0000 0072 1e00 0000  .r....r ...r....
+000007b0: 7214 0000 0072 1f00 0000 7213 0000 0072  r....r....r....r
+000007c0: 2100 0000 7229 0000 0072 2200 0000 7223  !...r)...r"...r#
+000007d0: 0000 0072 2300 0000 7224 0000 00da 0b73  ...r#...r$.....s
+000007e0: 6967 6e65 645f 706f 7374 5000 0000 7330  igned_postP...s0
+000007f0: 0000 0002 8016 0908 0206 0106 0104 0208  ................
+00000800: 0204 0106 0108 020a 0308 0108 0108 0108  ................
+00000810: 0102 fb08 0808 0108 0108 0108 0108 0108  ................
+00000820: 0116 0272 2b00 0000 2918 da07 6c6f 6767  ...r+...)...logg
+00000830: 696e 67da 0c75 726c 6c69 622e 7061 7273  ing..urllib.pars
+00000840: 6572 0200 0000 da07 6169 6f68 7474 70da  er......aiohttp.
+00000850: 1462 6f76 696e 652e 6372 7970 746f 2e68  .bovine.crypto.h
+00000860: 656c 7065 7272 0300 0000 da1c 626f 7669  elperr......bovi
+00000870: 6e65 2e63 7279 7074 6f2e 6874 7470 5f73  ne.crypto.http_s
+00000880: 6967 6e61 7475 7265 7204 0000 00da 1162  ignaturer......b
+00000890: 6f76 696e 652e 7574 696c 732e 6461 7465  ovine.utils.date
+000008a0: 7205 0000 00da 0663 6f6e 7374 7372 0700  r......constsr..
+000008b0: 0000 da0c 6576 656e 745f 736f 7572 6365  ....event_source
+000008c0: 7208 0000 00da 0967 6574 4c6f 6767 6572  r......getLogger
+000008d0: da08 5f5f 6e61 6d65 5f5f 7219 0000 00da  ..__name__r.....
+000008e0: 0d43 6c69 656e 7453 6573 7369 6f6e da03  .ClientSession..
+000008f0: 7374 72da 0464 6963 74da 0e43 6c69 656e  str..dict..Clien
+00000900: 7452 6573 706f 6e73 6572 2500 0000 7226  tResponser%...r&
+00000910: 0000 0072 2b00 0000 7223 0000 0072 2300  ...r+...r#...r#.
+00000920: 0000 7223 0000 0072 2400 0000 da08 3c6d  ..r#...r$.....<m
+00000930: 6f64 756c 653e 0100 0000 7368 0000 0008  odule>....sh....
+00000940: 000c 0108 020c 020c 010c 010c 020c 010a  ................
+00000950: 0202 0804 fb04 0102 ff02 0202 fe02 0302  ................
+00000960: fd02 0402 fc02 0502 fb04 060a fa02 2604  ..............&.
+00000970: fb04 0102 ff02 0202 fe02 0302 fd02 0402  ................
+00000980: fc02 050a fb02 2502 0104 f904 0102 ff02  ......%.........
+00000990: 0202 fe02 0302 fd02 0402 fc02 0502 fb02  ................
+000009a0: 0602 fa04 080e f8                        .......
```

### Comparing `bovine-0.1.0/bovine/clients/__pycache__/signed_http_client.cpython-310.pyc` & `bovine-0.1.1/bovine/clients/__pycache__/signed_http_client.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 13 15:55:57 2023 UTC, .py size: 1074 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0d26 3864 3204 0000  o........&8d2...
+00000000: 6f0d 0d0a 0000 0000 a4ea 3a64 3204 0000  o.........:d2...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 1a00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 4700 6402 6403 8400 6403  d.l.Z.G.d.d...d.
 00000040: 8302 5a02 6401 5300 2904 e900 0000 004e  ..Z.d.S.)......N
 00000050: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
 00000060: 0003 0000 0040 0000 0073 4000 0000 6500  .....@...s@...e.
 00000070: 5a01 6400 5a02 640c 6402 6403 8401 5a03  Z.d.Z.d.d.d...Z.
@@ -15,78 +15,78 @@
 000000e0: 007c 017c 005f 007c 027c 005f 017c 037c  .|.|._.|.|._.|.|
 000000f0: 005f 027c 047c 005f 0364 0053 00a9 014e  ._.|.|._.d.S...N
 00000100: 2904 da07 7365 7373 696f 6eda 0e70 7562  )...session..pub
 00000110: 6c69 635f 6b65 795f 7572 6cda 0b70 7269  lic_key_url..pri
 00000120: 7661 7465 5f6b 6579 da0b 6163 636f 756e  vate_key..accoun
 00000130: 745f 7572 6c29 05da 0473 656c 6672 0400  t_url)...selfr..
 00000140: 0000 7205 0000 0072 0600 0000 7207 0000  ..r....r....r...
-00000150: 00a9 0072 0900 0000 fa55 2f77 6f6f 6470  ...r.....U/woodp
+00000150: 00a9 0072 0900 0000 fa56 2f77 6f6f 6470  ...r.....V/woodp
 00000160: 6563 6b65 722f 7372 632f 636f 6465 6265  ecker/src/codebe
-00000170: 7267 2e6f 7267 2f68 656c 6765 2f62 6f76  rg.org/helge/bov
-00000180: 696e 652f 626f 7669 6e65 2f62 6f76 696e  ine/bovine/bovin
-00000190: 652f 636c 6965 6e74 732f 7369 676e 6564  e/clients/signed
-000001a0: 5f68 7474 705f 636c 6965 6e74 2e70 79da  _http_client.py.
-000001b0: 085f 5f69 6e69 745f 5f05 0000 0073 0800  .__init__....s..
-000001c0: 0000 0601 0601 0601 0a01 7a19 5369 676e  ..........z.Sign
-000001d0: 6564 4874 7470 436c 6965 6e74 2e5f 5f69  edHttpClient.__i
-000001e0: 6e69 745f 5f63 0200 0000 0000 0000 0000  nit__c..........
-000001f0: 0000 0200 0000 0200 0000 4300 0000 730a  ..........C...s.
-00000200: 0000 007c 017c 005f 007c 0053 0072 0300  ...|.|._.|.S.r..
-00000210: 0000 2901 7204 0000 0029 0272 0800 0000  ..).r....).r....
-00000220: 7204 0000 0072 0900 0000 7209 0000 0072  r....r....r....r
-00000230: 0a00 0000 da0b 7365 745f 7365 7373 696f  ......set_sessio
-00000240: 6e0b 0000 0073 0400 0000 0601 0402 7a1c  n....s........z.
-00000250: 5369 676e 6564 4874 7470 436c 6965 6e74  SignedHttpClient
-00000260: 2e73 6574 5f73 6573 7369 6f6e 6303 0000  .set_sessionc...
-00000270: 0000 0000 0000 0000 0003 0000 0007 0000  ................
-00000280: 00c3 0000 0073 2400 0000 8101 7400 6a01  .....s$.....t.j.
-00000290: 6a02 a003 7c00 6a04 7c00 6a05 7c00 6a06  j...|.j.|.j.|.j.
-000002a0: 7c01 7c02 a105 4900 6400 4800 5300 7203  |.|...I.d.H.S.r.
-000002b0: 0000 0029 07da 0662 6f76 696e 65da 0763  ...)...bovine..c
-000002c0: 6c69 656e 7473 da0b 7369 676e 6564 5f68  lients..signed_h
-000002d0: 7474 705a 0a73 6967 6e65 645f 6765 7472  ttpZ.signed_getr
-000002e0: 0400 0000 7205 0000 0072 0600 0000 2903  ....r....r....).
-000002f0: 7208 0000 00da 0375 726c da07 6865 6164  r......url..head
-00000300: 6572 7372 0900 0000 7209 0000 0072 0a00  ersr....r....r..
-00000310: 0000 da03 6765 7410 0000 0073 0800 0000  ....get....s....
-00000320: 0280 0801 1001 0aff 7a14 5369 676e 6564  ........z.Signed
-00000330: 4874 7470 436c 6965 6e74 2e67 6574 6305  HttpClient.getc.
-00000340: 0000 0000 0000 0000 0000 0005 0000 0009  ................
-00000350: 0000 00c3 0000 0073 2a00 0000 8101 7400  .......s*.....t.
-00000360: 6a01 6a02 6a03 7c00 6a04 7c00 6a05 7c00  j.j.j.|.j.|.j.|.
-00000370: 6a06 7c01 7c02 7c03 7c04 6401 8d07 4900  j.|.|.|.|.d...I.
-00000380: 6400 4800 5300 2902 4e29 01da 0c63 6f6e  d.H.S.).N)...con
-00000390: 7465 6e74 5f74 7970 6529 0772 0d00 0000  tent_type).r....
-000003a0: 720e 0000 0072 0f00 0000 5a0b 7369 676e  r....r....Z.sign
-000003b0: 6564 5f70 6f73 7472 0400 0000 7205 0000  ed_postr....r...
-000003c0: 0072 0600 0000 2905 7208 0000 0072 1000  .r....).r....r..
-000003d0: 0000 da04 626f 6479 7211 0000 0072 1300  ....bodyr....r..
-000003e0: 0000 7209 0000 0072 0900 0000 720a 0000  ..r....r....r...
-000003f0: 00da 0470 6f73 7415 0000 0073 1400 0000  ...post....s....
-00000400: 0280 0801 0401 0401 0401 0201 0201 0201  ................
-00000410: 0201 0cf9 7a15 5369 676e 6564 4874 7470  ....z.SignedHttp
-00000420: 436c 6965 6e74 2e70 6f73 7463 0200 0000  Client.postc....
-00000430: 0000 0000 0000 0000 0200 0000 0600 0000  ................
-00000440: 4300 0000 731a 0000 0074 006a 016a 02a0  C...s....t.j.j..
-00000450: 037c 006a 047c 006a 057c 006a 067c 01a1  .|.j.|.j.|.j.|..
-00000460: 0453 0072 0300 0000 2907 720d 0000 0072  .S.r....).r....r
-00000470: 0e00 0000 720f 0000 005a 1373 6967 6e65  ....r....Z.signe
-00000480: 645f 6576 656e 745f 736f 7572 6365 7204  d_event_sourcer.
-00000490: 0000 0072 0500 0000 7206 0000 0029 0272  ...r....r....).r
-000004a0: 0800 0000 7210 0000 0072 0900 0000 7209  ....r....r....r.
-000004b0: 0000 0072 0a00 0000 da0c 6576 656e 745f  ...r......event_
-000004c0: 736f 7572 6365 2000 0000 7306 0000 0008  source ...s.....
-000004d0: 010e 0104 ff7a 1d53 6967 6e65 6448 7474  .....z.SignedHtt
-000004e0: 7043 6c69 656e 742e 6576 656e 745f 736f  pClient.event_so
-000004f0: 7572 6365 7203 0000 0029 08da 085f 5f6e  urcer....)...__n
-00000500: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
-00000510: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5f72  _..__qualname__r
-00000520: 0b00 0000 720c 0000 0072 1200 0000 7215  ....r....r....r.
-00000530: 0000 0072 1600 0000 7209 0000 0072 0900  ...r....r....r..
-00000540: 0000 7209 0000 0072 0a00 0000 7202 0000  ..r....r....r...
-00000550: 0004 0000 0073 0c00 0000 0800 0a01 0806  .....s..........
-00000560: 0c05 0e05 0c0b 7202 0000 0029 035a 1a62  ......r....).Z.b
-00000570: 6f76 696e 652e 636c 6965 6e74 732e 7369  ovine.clients.si
-00000580: 676e 6564 5f68 7474 7072 0d00 0000 7202  gned_httpr....r.
-00000590: 0000 0072 0900 0000 7209 0000 0072 0900  ...r....r....r..
-000005a0: 0000 720a 0000 00da 083c 6d6f 6475 6c65  ..r......<module
-000005b0: 3e01 0000 0073 0400 0000 0800 1203       >....s........
+00000170: 7267 2e6f 7267 2f62 6f76 696e 652f 626f  rg.org/bovine/bo
+00000180: 7669 6e65 2f62 6f76 696e 652f 626f 7669  vine/bovine/bovi
+00000190: 6e65 2f63 6c69 656e 7473 2f73 6967 6e65  ne/clients/signe
+000001a0: 645f 6874 7470 5f63 6c69 656e 742e 7079  d_http_client.py
+000001b0: da08 5f5f 696e 6974 5f5f 0500 0000 7308  ..__init__....s.
+000001c0: 0000 0006 0106 0106 010a 017a 1953 6967  ...........z.Sig
+000001d0: 6e65 6448 7474 7043 6c69 656e 742e 5f5f  nedHttpClient.__
+000001e0: 696e 6974 5f5f 6302 0000 0000 0000 0000  init__c.........
+000001f0: 0000 0002 0000 0002 0000 0043 0000 0073  ...........C...s
+00000200: 0a00 0000 7c01 7c00 5f00 7c00 5300 7203  ....|.|._.|.S.r.
+00000210: 0000 0029 0172 0400 0000 2902 7208 0000  ...).r....).r...
+00000220: 0072 0400 0000 7209 0000 0072 0900 0000  .r....r....r....
+00000230: 720a 0000 00da 0b73 6574 5f73 6573 7369  r......set_sessi
+00000240: 6f6e 0b00 0000 7304 0000 0006 0104 027a  on....s........z
+00000250: 1c53 6967 6e65 6448 7474 7043 6c69 656e  .SignedHttpClien
+00000260: 742e 7365 745f 7365 7373 696f 6e63 0300  t.set_sessionc..
+00000270: 0000 0000 0000 0000 0000 0300 0000 0700  ................
+00000280: 0000 c300 0000 7324 0000 0081 0174 006a  ......s$.....t.j
+00000290: 016a 02a0 037c 006a 047c 006a 057c 006a  .j...|.j.|.j.|.j
+000002a0: 067c 017c 02a1 0549 0064 0048 0053 0072  .|.|...I.d.H.S.r
+000002b0: 0300 0000 2907 da06 626f 7669 6e65 da07  ....)...bovine..
+000002c0: 636c 6965 6e74 73da 0b73 6967 6e65 645f  clients..signed_
+000002d0: 6874 7470 5a0a 7369 676e 6564 5f67 6574  httpZ.signed_get
+000002e0: 7204 0000 0072 0500 0000 7206 0000 0029  r....r....r....)
+000002f0: 0372 0800 0000 da03 7572 6cda 0768 6561  .r......url..hea
+00000300: 6465 7273 7209 0000 0072 0900 0000 720a  dersr....r....r.
+00000310: 0000 00da 0367 6574 1000 0000 7308 0000  .....get....s...
+00000320: 0002 8008 0110 010a ff7a 1453 6967 6e65  .........z.Signe
+00000330: 6448 7474 7043 6c69 656e 742e 6765 7463  dHttpClient.getc
+00000340: 0500 0000 0000 0000 0000 0000 0500 0000  ................
+00000350: 0900 0000 c300 0000 732a 0000 0081 0174  ........s*.....t
+00000360: 006a 016a 026a 037c 006a 047c 006a 057c  .j.j.j.|.j.|.j.|
+00000370: 006a 067c 017c 027c 037c 0464 018d 0749  .j.|.|.|.|.d...I
+00000380: 0064 0048 0053 0029 024e 2901 da0c 636f  .d.H.S.).N)...co
+00000390: 6e74 656e 745f 7479 7065 2907 720d 0000  ntent_type).r...
+000003a0: 0072 0e00 0000 720f 0000 005a 0b73 6967  .r....r....Z.sig
+000003b0: 6e65 645f 706f 7374 7204 0000 0072 0500  ned_postr....r..
+000003c0: 0000 7206 0000 0029 0572 0800 0000 7210  ..r....).r....r.
+000003d0: 0000 00da 0462 6f64 7972 1100 0000 7213  .....bodyr....r.
+000003e0: 0000 0072 0900 0000 7209 0000 0072 0a00  ...r....r....r..
+000003f0: 0000 da04 706f 7374 1500 0000 7314 0000  ....post....s...
+00000400: 0002 8008 0104 0104 0104 0102 0102 0102  ................
+00000410: 0102 010c f97a 1553 6967 6e65 6448 7474  .....z.SignedHtt
+00000420: 7043 6c69 656e 742e 706f 7374 6302 0000  pClient.postc...
+00000430: 0000 0000 0000 0000 0002 0000 0006 0000  ................
+00000440: 0043 0000 0073 1a00 0000 7400 6a01 6a02  .C...s....t.j.j.
+00000450: a003 7c00 6a04 7c00 6a05 7c00 6a06 7c01  ..|.j.|.j.|.j.|.
+00000460: a104 5300 7203 0000 0029 0772 0d00 0000  ..S.r....).r....
+00000470: 720e 0000 0072 0f00 0000 5a13 7369 676e  r....r....Z.sign
+00000480: 6564 5f65 7665 6e74 5f73 6f75 7263 6572  ed_event_sourcer
+00000490: 0400 0000 7205 0000 0072 0600 0000 2902  ....r....r....).
+000004a0: 7208 0000 0072 1000 0000 7209 0000 0072  r....r....r....r
+000004b0: 0900 0000 720a 0000 00da 0c65 7665 6e74  ....r......event
+000004c0: 5f73 6f75 7263 6520 0000 0073 0600 0000  _source ...s....
+000004d0: 0801 0e01 04ff 7a1d 5369 676e 6564 4874  ......z.SignedHt
+000004e0: 7470 436c 6965 6e74 2e65 7665 6e74 5f73  tpClient.event_s
+000004f0: 6f75 7263 6572 0300 0000 2908 da08 5f5f  ourcer....)...__
+00000500: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
+00000510: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
+00000520: 720b 0000 0072 0c00 0000 7212 0000 0072  r....r....r....r
+00000530: 1500 0000 7216 0000 0072 0900 0000 7209  ....r....r....r.
+00000540: 0000 0072 0900 0000 720a 0000 0072 0200  ...r....r....r..
+00000550: 0000 0400 0000 730c 0000 0008 000a 0108  ......s.........
+00000560: 060c 050e 050c 0b72 0200 0000 2903 5a1a  .......r....).Z.
+00000570: 626f 7669 6e65 2e63 6c69 656e 7473 2e73  bovine.clients.s
+00000580: 6967 6e65 645f 6874 7470 720d 0000 0072  igned_httpr....r
+00000590: 0200 0000 7209 0000 0072 0900 0000 7209  ....r....r....r.
+000005a0: 0000 0072 0a00 0000 da08 3c6d 6f64 756c  ...r......<modul
+000005b0: 653e 0100 0000 7304 0000 0008 0012 03    e>....s........
```

### Comparing `bovine-0.1.0/bovine/clients/__pycache__/test_event_source.cpython-310-pytest-7.3.0.pyc` & `bovine-0.1.1/bovine/clients/__pycache__/test_event_source.cpython-310-pytest-7.3.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 13 15:55:57 2023 UTC, .py size: 609 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0d26 3864 6102 0000  o........&8da...
+00000000: 6f0d 0d0a 0000 0000 a4ea 3a64 6102 0000  o.........:da...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 4000 0000 6400  .....@...s@...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6402 6c06 6d07  ..m.Z...d.d.l.m.
 00000050: 5a07 0100 6403 6404 6c08 6d09 5a09 0100  Z...d.d.l.m.Z...
 00000060: 6408 6406 6407 8404 5a0a 6401 5300 2909  d.d.d...Z.d.S.).
 00000070: e900 0000 004e 2901 da09 4173 796e 634d  .....N)...AsyncM
@@ -59,27 +59,27 @@
 000003a0: 6e61 7469 6f6e 290a da07 7365 7373 696f  nation)...sessio
 000003b0: 6e72 0600 0000 da08 7265 7370 6f6e 7365  nr......response
 000003c0: da0c 6576 656e 745f 736f 7572 6365 720c  ..event_sourcer.
 000003d0: 0000 00da 0b40 7079 5f61 7373 6572 7431  .....@py_assert1
 000003e0: da0b 4070 795f 6173 7365 7274 34da 0b40  ..@py_assert4..@
 000003f0: 7079 5f61 7373 6572 7433 da0b 4070 795f  py_assert3..@py_
 00000400: 666f 726d 6174 36da 0b40 7079 5f66 6f72  format6..@py_for
-00000410: 6d61 7438 a900 7226 0000 00fa 542f 776f  mat8..r&....T/wo
+00000410: 6d61 7438 a900 7226 0000 00fa 552f 776f  mat8..r&....U/wo
 00000420: 6f64 7065 636b 6572 2f73 7263 2f63 6f64  odpecker/src/cod
-00000430: 6562 6572 672e 6f72 672f 6865 6c67 652f  eberg.org/helge/
-00000440: 626f 7669 6e65 2f62 6f76 696e 652f 626f  bovine/bovine/bo
-00000450: 7669 6e65 2f63 6c69 656e 7473 2f74 6573  vine/clients/tes
-00000460: 745f 6576 656e 745f 736f 7572 6365 2e70  t_event_source.p
-00000470: 79da 1174 6573 745f 6576 656e 745f 736f  y..test_event_so
-00000480: 7572 6365 0600 0000 7318 0000 0002 8006  urce....s.......
-00000490: 0106 010a 0108 010a 020c 020e 018a 010c  ................
-000004a0: 020e 018e 0172 2800 0000 2902 7205 0000  .....r(...).r...
-000004b0: 004e 290b da08 6275 696c 7469 6e73 7218  .N)...builtinsr.
-000004c0: 0000 00da 195f 7079 7465 7374 2e61 7373  ....._pytest.ass
-000004d0: 6572 7469 6f6e 2e72 6577 7269 7465 da09  ertion.rewrite..
-000004e0: 6173 7365 7274 696f 6eda 0772 6577 7269  assertion..rewri
-000004f0: 7465 7216 0000 00da 0d75 6e69 7474 6573  ter......unittes
-00000500: 742e 6d6f 636b 7202 0000 0072 2000 0000  t.mockr....r ...
-00000510: 7204 0000 0072 2800 0000 7226 0000 0072  r....r(...r&...r
-00000520: 2600 0000 7226 0000 0072 2700 0000 da08  &...r&...r'.....
-00000530: 3c6d 6f64 756c 653e 0100 0000 7306 0000  <module>....s...
-00000540: 0026 000c 020e 03                        .&.....
+00000430: 6562 6572 672e 6f72 672f 626f 7669 6e65  eberg.org/bovine
+00000440: 2f62 6f76 696e 652f 626f 7669 6e65 2f62  /bovine/bovine/b
+00000450: 6f76 696e 652f 636c 6965 6e74 732f 7465  ovine/clients/te
+00000460: 7374 5f65 7665 6e74 5f73 6f75 7263 652e  st_event_source.
+00000470: 7079 da11 7465 7374 5f65 7665 6e74 5f73  py..test_event_s
+00000480: 6f75 7263 6506 0000 0073 1800 0000 0280  ource....s......
+00000490: 0601 0601 0a01 0801 0a02 0c02 0e01 8a01  ................
+000004a0: 0c02 0e01 8e01 7228 0000 0029 0272 0500  ......r(...).r..
+000004b0: 0000 4e29 0bda 0862 7569 6c74 696e 7372  ..N)...builtinsr
+000004c0: 1800 0000 da19 5f70 7974 6573 742e 6173  ......_pytest.as
+000004d0: 7365 7274 696f 6e2e 7265 7772 6974 65da  sertion.rewrite.
+000004e0: 0961 7373 6572 7469 6f6e da07 7265 7772  .assertion..rewr
+000004f0: 6974 6572 1600 0000 da0d 756e 6974 7465  iter......unitte
+00000500: 7374 2e6d 6f63 6b72 0200 0000 7220 0000  st.mockr....r ..
+00000510: 0072 0400 0000 7228 0000 0072 2600 0000  .r....r(...r&...
+00000520: 7226 0000 0072 2600 0000 7227 0000 00da  r&...r&...r'....
+00000530: 083c 6d6f 6475 6c65 3e01 0000 0073 0600  .<module>....s..
+00000540: 0000 2600 0c02 0e03                      ..&.....
```

### Comparing `bovine-0.1.0/bovine/clients/__pycache__/test_lookup_account.cpython-310-pytest-7.3.0.pyc` & `bovine-0.1.1/bovine/clients/__pycache__/test_lookup_account.cpython-310-pytest-7.3.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 13 15:55:57 2023 UTC, .py size: 624 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0d26 3864 7002 0000  o........&8dp...
+00000000: 6f0d 0d0a 0000 0000 a4ea 3a64 7002 0000  o.........:dp...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 4600 0000 6400  .....@...sF...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6401 6c06 5a06  ..m.Z...d.d.l.Z.
 00000050: 6402 6403 6c07 6d08 5a08 6d09 5a09 0100  d.d.l.m.Z.m.Z...
 00000060: 6404 6405 8400 5a0a 6406 6407 8400 5a0b  d.d...Z.d.d...Z.
 00000070: 6401 5300 2908 e900 0000 004e e901 0000  d.S.)......N....
@@ -43,57 +43,57 @@
 000002a0: 6d65 da09 5f73 6166 6572 6570 72da 0e41  me.._saferepr..A
 000002b0: 7373 6572 7469 6f6e 4572 726f 72da 135f  ssertionError.._
 000002c0: 666f 726d 6174 5f65 7870 6c61 6e61 7469  format_explanati
 000002d0: 6f6e 2906 da07 7365 7373 696f 6e72 0700  on)...sessionr..
 000002e0: 0000 da0b 4070 795f 6173 7365 7274 31da  ....@py_assert1.
 000002f0: 0b40 7079 5f61 7373 6572 7433 da0b 4070  .@py_assert3..@p
 00000300: 795f 6173 7365 7274 35da 0b40 7079 5f66  y_assert5..@py_f
-00000310: 6f72 6d61 7437 a900 721c 0000 00fa 562f  ormat7..r.....V/
+00000310: 6f72 6d61 7437 a900 721c 0000 00fa 572f  ormat7..r.....W/
 00000320: 776f 6f64 7065 636b 6572 2f73 7263 2f63  woodpecker/src/c
-00000330: 6f64 6562 6572 672e 6f72 672f 6865 6c67  odeberg.org/helg
-00000340: 652f 626f 7669 6e65 2f62 6f76 696e 652f  e/bovine/bovine/
-00000350: 626f 7669 6e65 2f63 6c69 656e 7473 2f74  bovine/clients/t
-00000360: 6573 745f 6c6f 6f6b 7570 5f61 6363 6f75  est_lookup_accou
-00000370: 6e74 2e70 79da 1374 6573 745f 6c6f 6f6b  nt.py..test_look
-00000380: 7570 5f61 6363 6f75 6e74 0600 0000 730a  up_account....s.
-00000390: 0000 0002 8012 0112 0128 ff78 0372 1e00  .........(.x.r..
-000003a0: 0000 6300 0000 0000 0000 0000 0000 0007  ..c.............
-000003b0: 0000 0009 0000 00c3 0000 0073 cc00 0000  ...........s....
-000003c0: 8101 6401 7d00 7400 a001 a100 3400 4900  ..d.}.t.....4.I.
-000003d0: 6400 4800 9a14 7d01 7402 7c01 6402 7c00  d.H...}.t.|.d.|.
-000003e0: 8303 4900 6400 4800 7d02 5700 6400 0400  ..I.d.H.}.W.d...
-000003f0: 0400 8303 4900 6400 4800 0100 6e0b 3100  ....I.d.H...n.1.
-00000400: 4900 6400 4800 7325 7701 0100 0100 0100  I.d.H.s%w.......
-00000410: 5900 0100 7c02 6a03 7d03 6403 7d04 7c03  Y...|.j.}.d.}.|.
-00000420: 7c04 8301 7d05 7c05 735e 6404 6405 7404  |...}.|.s^d.d.t.
-00000430: a005 a100 7600 7341 7406 a007 7c02 a101  ....v.sAt...|...
-00000440: 7246 7406 a008 7c02 a101 6e01 6405 7406  rFt...|...n.d.t.
-00000450: a008 7c03 a101 7406 a008 7c04 a101 7406  ..|...t...|...t.
-00000460: a008 7c05 a101 6406 9c04 1600 7d06 7409  ..|...d.....}.t.
-00000470: 7406 a00a 7c06 a101 8301 8201 6400 0400  t...|.......d...
-00000480: 7d03 0400 7d04 7d05 6400 5300 2907 4e7a  }...}.}.d.S.).Nz
-00000490: 3864 6964 3a6b 6579 3a7a 364d 6b75 6a64  8did:key:z6Mkujd
-000004a0: 5a32 3136 6559 7a35 3576 7a38 5835 4865  Z216eYz55vz8X5He
-000004b0: 7471 654a 586a 3964 646e 355a 485a 5573  tqeJXj9ddn5ZHZUs
-000004c0: 4270 5258 3477 666e 4c7a 0c6d 796d 6174  BpRX4wfnLz.mymat
-000004d0: 682e 726f 636b 7372 0500 0000 7206 0000  h.rocksr....r...
-000004e0: 0072 0700 0000 7208 0000 0029 0b72 0d00  .r....r....).r..
-000004f0: 0000 720e 0000 0072 0400 0000 720f 0000  ..r....r....r...
-00000500: 0072 1000 0000 7211 0000 0072 1200 0000  .r....r....r....
-00000510: 7213 0000 0072 1400 0000 7215 0000 0072  r....r....r....r
-00000520: 1600 0000 2907 5a09 6469 645f 6865 6c67  ....).Z.did_helg
-00000530: 6572 1700 0000 7207 0000 0072 1800 0000  er....r....r....
-00000540: 7219 0000 0072 1a00 0000 721b 0000 0072  r....r....r....r
-00000550: 1c00 0000 721c 0000 0072 1d00 0000 da1e  ....r....r......
-00000560: 7465 7374 5f6c 6f6f 6b75 705f 6469 645f  test_lookup_did_
-00000570: 7769 7468 5f77 6562 6669 6e67 6572 0d00  with_webfinger..
-00000580: 0000 730c 0000 0002 8004 0112 0114 0128  ..s............(
-00000590: ff78 0372 1f00 0000 290c da08 6275 696c  .x.r....)...buil
-000005a0: 7469 6e73 7210 0000 00da 195f 7079 7465  tinsr......_pyte
-000005b0: 7374 2e61 7373 6572 7469 6f6e 2e72 6577  st.assertion.rew
-000005c0: 7269 7465 da09 6173 7365 7274 696f 6eda  rite..assertion.
-000005d0: 0772 6577 7269 7465 7212 0000 0072 0d00  .rewriter....r..
-000005e0: 0000 da00 7203 0000 0072 0400 0000 721e  ....r....r....r.
-000005f0: 0000 0072 1f00 0000 721c 0000 0072 1c00  ...r....r....r..
-00000600: 0000 721c 0000 0072 1d00 0000 da08 3c6d  ..r....r......<m
-00000610: 6f64 756c 653e 0100 0000 7308 0000 0022  odule>....s...."
-00000620: 0010 0208 030c 07                        .......
+00000330: 6f64 6562 6572 672e 6f72 672f 626f 7669  odeberg.org/bovi
+00000340: 6e65 2f62 6f76 696e 652f 626f 7669 6e65  ne/bovine/bovine
+00000350: 2f62 6f76 696e 652f 636c 6965 6e74 732f  /bovine/clients/
+00000360: 7465 7374 5f6c 6f6f 6b75 705f 6163 636f  test_lookup_acco
+00000370: 756e 742e 7079 da13 7465 7374 5f6c 6f6f  unt.py..test_loo
+00000380: 6b75 705f 6163 636f 756e 7406 0000 0073  kup_account....s
+00000390: 0a00 0000 0280 1201 1201 28ff 7803 721e  ..........(.x.r.
+000003a0: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+000003b0: 0700 0000 0900 0000 c300 0000 73cc 0000  ............s...
+000003c0: 0081 0164 017d 0074 00a0 01a1 0034 0049  ...d.}.t.....4.I
+000003d0: 0064 0048 009a 147d 0174 027c 0164 027c  .d.H...}.t.|.d.|
+000003e0: 0083 0349 0064 0048 007d 0257 0064 0004  ...I.d.H.}.W.d..
+000003f0: 0004 0083 0349 0064 0048 0001 006e 0b31  .....I.d.H...n.1
+00000400: 0049 0064 0048 0073 2577 0101 0001 0001  .I.d.H.s%w......
+00000410: 0059 0001 007c 026a 037d 0364 037d 047c  .Y...|.j.}.d.}.|
+00000420: 037c 0483 017d 057c 0573 5e64 0464 0574  .|...}.|.s^d.d.t
+00000430: 04a0 05a1 0076 0073 4174 06a0 077c 02a1  .....v.sAt...|..
+00000440: 0172 4674 06a0 087c 02a1 016e 0164 0574  .rFt...|...n.d.t
+00000450: 06a0 087c 03a1 0174 06a0 087c 04a1 0174  ...|...t...|...t
+00000460: 06a0 087c 05a1 0164 069c 0416 007d 0674  ...|...d.....}.t
+00000470: 0974 06a0 0a7c 06a1 0183 0182 0164 0004  .t...|.......d..
+00000480: 007d 0304 007d 047d 0564 0053 0029 074e  .}...}.}.d.S.).N
+00000490: 7a38 6469 643a 6b65 793a 7a36 4d6b 756a  z8did:key:z6Mkuj
+000004a0: 645a 3231 3665 597a 3535 767a 3858 3548  dZ216eYz55vz8X5H
+000004b0: 6574 7165 4a58 6a39 6464 6e35 5a48 5a55  etqeJXj9ddn5ZHZU
+000004c0: 7342 7052 5834 7766 6e4c 7a0c 6d79 6d61  sBpRX4wfnLz.myma
+000004d0: 7468 2e72 6f63 6b73 7205 0000 0072 0600  th.rocksr....r..
+000004e0: 0000 7207 0000 0072 0800 0000 290b 720d  ..r....r....).r.
+000004f0: 0000 0072 0e00 0000 7204 0000 0072 0f00  ...r....r....r..
+00000500: 0000 7210 0000 0072 1100 0000 7212 0000  ..r....r....r...
+00000510: 0072 1300 0000 7214 0000 0072 1500 0000  .r....r....r....
+00000520: 7216 0000 0029 075a 0964 6964 5f68 656c  r....).Z.did_hel
+00000530: 6765 7217 0000 0072 0700 0000 7218 0000  ger....r....r...
+00000540: 0072 1900 0000 721a 0000 0072 1b00 0000  .r....r....r....
+00000550: 721c 0000 0072 1c00 0000 721d 0000 00da  r....r....r.....
+00000560: 1e74 6573 745f 6c6f 6f6b 7570 5f64 6964  .test_lookup_did
+00000570: 5f77 6974 685f 7765 6266 696e 6765 720d  _with_webfinger.
+00000580: 0000 0073 0c00 0000 0280 0401 1201 1401  ...s............
+00000590: 28ff 7803 721f 0000 0029 0cda 0862 7569  (.x.r....)...bui
+000005a0: 6c74 696e 7372 1000 0000 da19 5f70 7974  ltinsr......_pyt
+000005b0: 6573 742e 6173 7365 7274 696f 6e2e 7265  est.assertion.re
+000005c0: 7772 6974 65da 0961 7373 6572 7469 6f6e  write..assertion
+000005d0: da07 7265 7772 6974 6572 1200 0000 720d  ..rewriter....r.
+000005e0: 0000 00da 0072 0300 0000 7204 0000 0072  .....r....r....r
+000005f0: 1e00 0000 721f 0000 0072 1c00 0000 721c  ....r....r....r.
+00000600: 0000 0072 1c00 0000 721d 0000 00da 083c  ...r....r......<
+00000610: 6d6f 6475 6c65 3e01 0000 0073 0800 0000  module>....s....
+00000620: 2200 1002 0803 0c07                      ".......
```

### Comparing `bovine-0.1.0/bovine/clients/__pycache__/test_nodeinfo.cpython-310-pytest-7.3.0.pyc` & `bovine-0.1.1/bovine/clients/__pycache__/test_nodeinfo.cpython-310-pytest-7.3.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 13 15:55:57 2023 UTC, .py size: 327 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0d26 3864 4701 0000  o........&8dG...
+00000000: 6f0d 0d0a 0000 0000 a4ea 3a64 3f01 0000  o.........:d?...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 3a00 0000 6400  .....@...s:...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6401 6c06 5a06  ..m.Z...d.d.l.Z.
 00000050: 6402 6403 6c07 6d08 5a08 0100 6404 6405  d.d.l.m.Z...d.d.
 00000060: 8400 5a09 6401 5300 2906 e900 0000 004e  ..Z.d.S.)......N
 00000070: e901 0000 0029 01da 0e66 6574 6368 5f6e  .....)...fetch_n
@@ -53,25 +53,25 @@
 00000340: 6f6e da11 5f63 616c 6c5f 7265 7072 636f  on.._call_reprco
 00000350: 6d70 6172 6529 08da 0773 6573 7369 6f6e  mpare)...session
 00000360: 7205 0000 005a 0b40 7079 5f66 6f72 6d61  r....Z.@py_forma
 00000370: 7431 da0b 4070 795f 6173 7365 7274 30da  t1..@py_assert0.
 00000380: 0b40 7079 5f61 7373 6572 7433 da0b 4070  .@py_assert3..@p
 00000390: 795f 6173 7365 7274 32da 0b40 7079 5f66  y_assert2..@py_f
 000003a0: 6f72 6d61 7435 da0b 4070 795f 666f 726d  ormat5..@py_form
-000003b0: 6174 37a9 0072 1e00 0000 fa50 2f77 6f6f  at7..r.....P/woo
+000003b0: 6174 37a9 0072 1e00 0000 fa51 2f77 6f6f  at7..r.....Q/woo
 000003c0: 6470 6563 6b65 722f 7372 632f 636f 6465  dpecker/src/code
-000003d0: 6265 7267 2e6f 7267 2f68 656c 6765 2f62  berg.org/helge/b
-000003e0: 6f76 696e 652f 626f 7669 6e65 2f62 6f76  ovine/bovine/bov
-000003f0: 696e 652f 636c 6965 6e74 732f 7465 7374  ine/clients/test
-00000400: 5f6e 6f64 6569 6e66 6f2e 7079 da13 7465  _nodeinfo.py..te
-00000410: 7374 5f66 6574 6368 5f6e 6f64 6569 6e66  st_fetch_nodeinf
-00000420: 6f06 0000 0073 0e00 0000 0280 1201 1001  o....s..........
-00000430: 3e02 6e02 6c01 2efa 7220 0000 0029 0ada  >.n.l...r ...)..
-00000440: 0862 7569 6c74 696e 7372 1000 0000 da19  .builtinsr......
-00000450: 5f70 7974 6573 742e 6173 7365 7274 696f  _pytest.assertio
-00000460: 6e2e 7265 7772 6974 65da 0961 7373 6572  n.rewrite..asser
-00000470: 7469 6f6e da07 7265 7772 6974 6572 1200  tion..rewriter..
-00000480: 0000 720e 0000 005a 086e 6f64 6569 6e66  ..r....Z.nodeinf
-00000490: 6f72 0300 0000 7220 0000 0072 1e00 0000  or....r ...r....
-000004a0: 721e 0000 0072 1e00 0000 721f 0000 00da  r....r....r.....
-000004b0: 083c 6d6f 6475 6c65 3e01 0000 0073 0600  .<module>....s..
-000004c0: 0000 2200 0c02 0c03                      ..".....
+000003d0: 6265 7267 2e6f 7267 2f62 6f76 696e 652f  berg.org/bovine/
+000003e0: 626f 7669 6e65 2f62 6f76 696e 652f 626f  bovine/bovine/bo
+000003f0: 7669 6e65 2f63 6c69 656e 7473 2f74 6573  vine/clients/tes
+00000400: 745f 6e6f 6465 696e 666f 2e70 79da 1374  t_nodeinfo.py..t
+00000410: 6573 745f 6665 7463 685f 6e6f 6465 696e  est_fetch_nodein
+00000420: 666f 0600 0000 730e 0000 0002 8012 0110  fo....s.........
+00000430: 013e 026e 026c 012e fa72 2000 0000 290a  .>.n.l...r ...).
+00000440: da08 6275 696c 7469 6e73 7210 0000 00da  ..builtinsr.....
+00000450: 195f 7079 7465 7374 2e61 7373 6572 7469  ._pytest.asserti
+00000460: 6f6e 2e72 6577 7269 7465 da09 6173 7365  on.rewrite..asse
+00000470: 7274 696f 6eda 0772 6577 7269 7465 7212  rtion..rewriter.
+00000480: 0000 0072 0e00 0000 da00 7203 0000 0072  ...r......r....r
+00000490: 2000 0000 721e 0000 0072 1e00 0000 721e   ...r....r....r.
+000004a0: 0000 0072 1f00 0000 da08 3c6d 6f64 756c  ...r......<modul
+000004b0: 653e 0100 0000 7306 0000 0022 000c 020c  e>....s...."....
+000004c0: 03                                       .
```

### Comparing `bovine-0.1.0/bovine/clients/__pycache__/test_signed_http.cpython-310-pytest-7.3.0.pyc` & `bovine-0.1.1/bovine/clients/__pycache__/test_signed_http.cpython-310-pytest-7.3.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 13 15:55:57 2023 UTC, .py size: 1145 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0d26 3864 7904 0000  o........&8dy...
+00000000: 6f0d 0d0a 0000 0000 a4ea 3a64 7904 0000  o.........:dy...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 6600 0000 6400  .....@...sf...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6402 6c06 6d07  ..m.Z...d.d.l.m.
 00000050: 5a07 6d08 5a08 0100 6400 6401 6c09 5a09  Z.m.Z...d.d.l.Z.
 00000060: 6400 6403 6c0a 6d0b 5a0b 0100 6400 6404  d.d.l.m.Z...d.d.
 00000070: 6c0c 6d0d 5a0d 6d0e 5a0e 0100 6405 6406  l.m.Z.m.Z...d.d.
@@ -99,33 +99,33 @@
 00000620: 6572 7432 da0b 4070 795f 6173 7365 7274  ert2..@py_assert
 00000630: 31da 0b40 7079 5f66 6f72 6d61 7434 da0b  1..@py_format4..
 00000640: 4070 795f 666f 726d 6174 36da 0461 7267  @py_format6..arg
 00000650: 73da 0b40 7079 5f61 7373 6572 7430 da0b  s..@py_assert0..
 00000660: 4070 795f 6173 7365 7274 33da 0b40 7079  @py_assert3..@py
 00000670: 5f66 6f72 6d61 7435 da0b 4070 795f 666f  _format5..@py_fo
 00000680: 726d 6174 3772 1400 0000 da07 7265 7175  rmat7r......requ
-00000690: 6573 74a9 0072 3400 0000 fa53 2f77 6f6f  est..r4....S/woo
+00000690: 6573 74a9 0072 3400 0000 fa54 2f77 6f6f  est..r4....T/woo
 000006a0: 6470 6563 6b65 722f 7372 632f 636f 6465  dpecker/src/code
-000006b0: 6265 7267 2e6f 7267 2f68 656c 6765 2f62  berg.org/helge/b
-000006c0: 6f76 696e 652f 626f 7669 6e65 2f62 6f76  ovine/bovine/bov
-000006d0: 696e 652f 636c 6965 6e74 732f 7465 7374  ine/clients/test
-000006e0: 5f73 6967 6e65 645f 6874 7470 2e70 79da  _signed_http.py.
-000006f0: 0f74 6573 745f 7369 676e 6564 5f67 6574  .test_signed_get
-00000700: 0b00 0000 732e 0000 0002 8004 0104 010a  ....s...........
-00000710: 0108 0108 0106 020a 0108 0114 020a 0278  ...............x
-00000720: 0208 026c 026a 010c 0106 0206 0106 0106  ...l.j..........
-00000730: 0174 0208 0274 0172 3600 0000 2912 da08  .t...t.r6...)...
-00000740: 6275 696c 7469 6e73 721d 0000 00da 195f  builtinsr......_
-00000750: 7079 7465 7374 2e61 7373 6572 7469 6f6e  pytest.assertion
-00000760: 2e72 6577 7269 7465 da09 6173 7365 7274  .rewrite..assert
-00000770: 696f 6eda 0772 6577 7269 7465 721b 0000  ion..rewriter...
-00000780: 00da 0d75 6e69 7474 6573 742e 6d6f 636b  ...unittest.mock
-00000790: 7202 0000 0072 0300 0000 7217 0000 005a  r....r....r....Z
-000007a0: 1f62 6f76 696e 652e 6372 7970 746f 2e73  .bovine.crypto.s
-000007b0: 6967 6e61 7475 7265 5f63 6865 636b 6572  ignature_checker
-000007c0: 7204 0000 00da 1262 6f76 696e 652e 6372  r......bovine.cr
-000007d0: 7970 746f 2e74 6573 7472 0500 0000 7206  ypto.testr....r.
-000007e0: 0000 00da 0b73 6967 6e65 645f 6874 7470  .....signed_http
-000007f0: 7208 0000 0072 3600 0000 7234 0000 0072  r....r6...r4...r
-00000800: 3400 0000 7234 0000 0072 3500 0000 da08  4...r4...r5.....
-00000810: 3c6d 6f64 756c 653e 0100 0000 730c 0000  <module>....s...
-00000820: 002a 0008 020c 0210 010c 020c 03         .*...........
+000006b0: 6265 7267 2e6f 7267 2f62 6f76 696e 652f  berg.org/bovine/
+000006c0: 626f 7669 6e65 2f62 6f76 696e 652f 626f  bovine/bovine/bo
+000006d0: 7669 6e65 2f63 6c69 656e 7473 2f74 6573  vine/clients/tes
+000006e0: 745f 7369 676e 6564 5f68 7474 702e 7079  t_signed_http.py
+000006f0: da0f 7465 7374 5f73 6967 6e65 645f 6765  ..test_signed_ge
+00000700: 740b 0000 0073 2e00 0000 0280 0401 0401  t....s..........
+00000710: 0a01 0801 0801 0602 0a01 0801 1402 0a02  ................
+00000720: 7802 0802 6c02 6a01 0c01 0602 0601 0601  x...l.j.........
+00000730: 0601 7402 0802 7401 7236 0000 0029 12da  ..t...t.r6...)..
+00000740: 0862 7569 6c74 696e 7372 1d00 0000 da19  .builtinsr......
+00000750: 5f70 7974 6573 742e 6173 7365 7274 696f  _pytest.assertio
+00000760: 6e2e 7265 7772 6974 65da 0961 7373 6572  n.rewrite..asser
+00000770: 7469 6f6e da07 7265 7772 6974 6572 1b00  tion..rewriter..
+00000780: 0000 da0d 756e 6974 7465 7374 2e6d 6f63  ....unittest.moc
+00000790: 6b72 0200 0000 7203 0000 0072 1700 0000  kr....r....r....
+000007a0: 5a1f 626f 7669 6e65 2e63 7279 7074 6f2e  Z.bovine.crypto.
+000007b0: 7369 676e 6174 7572 655f 6368 6563 6b65  signature_checke
+000007c0: 7272 0400 0000 da12 626f 7669 6e65 2e63  rr......bovine.c
+000007d0: 7279 7074 6f2e 7465 7374 7205 0000 0072  rypto.testr....r
+000007e0: 0600 0000 da0b 7369 676e 6564 5f68 7474  ......signed_htt
+000007f0: 7072 0800 0000 7236 0000 0072 3400 0000  pr....r6...r4...
+00000800: 7234 0000 0072 3400 0000 7235 0000 00da  r4...r4...r5....
+00000810: 083c 6d6f 6475 6c65 3e01 0000 0073 0c00  .<module>....s..
+00000820: 0000 2a00 0802 0c02 1001 0c02 0c03       ..*...........
```

### Comparing `bovine-0.1.0/bovine/clients/__pycache__/test_signed_http_client.cpython-310-pytest-7.3.0.pyc` & `bovine-0.1.1/bovine/clients/__pycache__/test_signed_http_client.cpython-310-pytest-7.3.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 13 15:55:57 2023 UTC, .py size: 529 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0d26 3864 1102 0000  o........&8d....
+00000000: 6f0d 0d0a 0000 0000 a4ea 3a64 1102 0000  o.........:d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 5200 0000 6400  .....@...sR...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6402 6c06 6d07  ..m.Z...d.d.l.m.
 00000050: 5a07 0100 6400 6401 6c08 5a08 6400 6403  Z...d.d.l.Z.d.d.
 00000060: 6c09 6d0a 5a0a 0100 6404 6405 6c0b 6d0c  l.m.Z...d.d.l.m.
 00000070: 5a0c 0100 6406 6407 8400 5a0d 6401 5300  Z...d.d...Z.d.S.
@@ -22,31 +22,31 @@
 00000150: 7562 6c69 635f 6b65 795f 7572 6c29 0772  ublic_key_url).r
 00000160: 0200 0000 da07 6169 6f68 7474 70da 0d43  ......aiohttp..C
 00000170: 6c69 656e 7453 6573 7369 6f6e da03 6765  lientSession..ge
 00000180: 7472 0500 0000 7203 0000 00da 1361 7373  tr....r......ass
 00000190: 6572 745f 6177 6169 7465 645f 6f6e 6365  ert_awaited_once
 000001a0: 2904 da07 7365 7373 696f 6eda 0375 726c  )...session..url
 000001b0: 7206 0000 00da 0663 6c69 656e 74a9 0072  r......client..r
-000001c0: 0e00 0000 fa5a 2f77 6f6f 6470 6563 6b65  .....Z/woodpecke
+000001c0: 0e00 0000 fa5b 2f77 6f6f 6470 6563 6b65  .....[/woodpecke
 000001d0: 722f 7372 632f 636f 6465 6265 7267 2e6f  r/src/codeberg.o
-000001e0: 7267 2f68 656c 6765 2f62 6f76 696e 652f  rg/helge/bovine/
-000001f0: 626f 7669 6e65 2f62 6f76 696e 652f 636c  bovine/bovine/cl
-00000200: 6965 6e74 732f 7465 7374 5f73 6967 6e65  ients/test_signe
-00000210: 645f 6874 7470 5f63 6c69 656e 742e 7079  d_http_client.py
-00000220: da1c 7465 7374 5f61 6374 6976 6974 795f  ..test_activity_
-00000230: 7075 625f 636c 6965 6e74 5f67 6574 0a00  pub_client_get..
-00000240: 0000 7312 0000 0002 800a 0104 0104 010a  ..s.............
-00000250: 0108 010c 0210 020e 0272 1000 0000 290e  .........r....).
-00000260: da08 6275 696c 7469 6e73 da0c 4070 795f  ..builtins..@py_
-00000270: 6275 696c 7469 6e73 da19 5f70 7974 6573  builtins.._pytes
-00000280: 742e 6173 7365 7274 696f 6e2e 7265 7772  t.assertion.rewr
-00000290: 6974 65da 0961 7373 6572 7469 6f6e da07  ite..assertion..
-000002a0: 7265 7772 6974 65da 0a40 7079 7465 7374  rewrite..@pytest
-000002b0: 5f61 72da 0d75 6e69 7474 6573 742e 6d6f  _ar..unittest.mo
-000002c0: 636b 7202 0000 0072 0700 0000 da12 626f  ckr....r......bo
-000002d0: 7669 6e65 2e63 7279 7074 6f2e 7465 7374  vine.crypto.test
-000002e0: 7203 0000 00da 1273 6967 6e65 645f 6874  r......signed_ht
-000002f0: 7470 5f63 6c69 656e 7472 0500 0000 7210  tp_clientr....r.
-00000300: 0000 0072 0e00 0000 720e 0000 0072 0e00  ...r....r....r..
-00000310: 0000 720f 0000 00da 083c 6d6f 6475 6c65  ..r......<module
-00000320: 3e01 0000 0073 0a00 0000 2600 0802 0c02  >....s....&.....
-00000330: 0c02 0c03                                ....
+000001e0: 7267 2f62 6f76 696e 652f 626f 7669 6e65  rg/bovine/bovine
+000001f0: 2f62 6f76 696e 652f 626f 7669 6e65 2f63  /bovine/bovine/c
+00000200: 6c69 656e 7473 2f74 6573 745f 7369 676e  lients/test_sign
+00000210: 6564 5f68 7474 705f 636c 6965 6e74 2e70  ed_http_client.p
+00000220: 79da 1c74 6573 745f 6163 7469 7669 7479  y..test_activity
+00000230: 5f70 7562 5f63 6c69 656e 745f 6765 740a  _pub_client_get.
+00000240: 0000 0073 1200 0000 0280 0a01 0401 0401  ...s............
+00000250: 0a01 0801 0c02 1002 0e02 7210 0000 0029  ..........r....)
+00000260: 0eda 0862 7569 6c74 696e 73da 0c40 7079  ...builtins..@py
+00000270: 5f62 7569 6c74 696e 73da 195f 7079 7465  _builtins.._pyte
+00000280: 7374 2e61 7373 6572 7469 6f6e 2e72 6577  st.assertion.rew
+00000290: 7269 7465 da09 6173 7365 7274 696f 6eda  rite..assertion.
+000002a0: 0772 6577 7269 7465 da0a 4070 7974 6573  .rewrite..@pytes
+000002b0: 745f 6172 da0d 756e 6974 7465 7374 2e6d  t_ar..unittest.m
+000002c0: 6f63 6b72 0200 0000 7207 0000 00da 1262  ockr....r......b
+000002d0: 6f76 696e 652e 6372 7970 746f 2e74 6573  ovine.crypto.tes
+000002e0: 7472 0300 0000 da12 7369 676e 6564 5f68  tr......signed_h
+000002f0: 7474 705f 636c 6965 6e74 7205 0000 0072  ttp_clientr....r
+00000300: 1000 0000 720e 0000 0072 0e00 0000 720e  ....r....r....r.
+00000310: 0000 0072 0f00 0000 da08 3c6d 6f64 756c  ...r......<modul
+00000320: 653e 0100 0000 730a 0000 0026 0008 020c  e>....s....&....
+00000330: 020c 020c 03                             .....
```

### Comparing `bovine-0.1.0/bovine/clients/event_source.py` & `bovine-0.1.1/bovine/clients/event_source.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.0/bovine/clients/lookup_account.py` & `bovine-0.1.1/bovine/clients/lookup_account.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.0/bovine/clients/moo_auth_client.py` & `bovine-0.1.1/bovine/clients/moo_auth_client.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.0/bovine/clients/nodeinfo.py` & `bovine-0.1.1/bovine/clients/nodeinfo.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,37 +5,23 @@
 import aiohttp
 
 from .consts import BOVINE_CLIENT_NAME
 
 logger = logging.getLogger(__name__)
 
 
-async def fetch_nodeinfo(session: aiohttp.ClientSession, domain: str) -> dict | None:
-    try:
-        wellknown_nodeinfo_url = f"https://{domain}/.well-known/nodeinfo"
-
-        async with session.get(
-            wellknown_nodeinfo_url,
-            headers={"user-agent": BOVINE_CLIENT_NAME},
-            timeout=60,
-        ) as response:
-            text = await response.text()
-            data = json.loads(text)
+async def fetch_nodeinfo_document(session: aiohttp.ClientSession, domain: str) -> dict:
+    wellknown_nodeinfo_url = f"https://{domain}/.well-known/nodeinfo"
 
-        for link in data["links"]:
-            if link["rel"] == "http://nodeinfo.diaspora.software/ns/schema/2.0":
-                return await fetch_nodeinfo20(session, link["href"])
-
-        return None
-
-    except Exception as e:
-        logger.error(str(e))
-        for log_line in traceback.format_exc().splitlines():
-            logger.error(log_line)
-        return None
+    async with session.get(
+        wellknown_nodeinfo_url,
+        headers={"user-agent": BOVINE_CLIENT_NAME},
+        timeout=60,
+    ) as response:
+        return await response.json()
 
 
 async def fetch_nodeinfo20(session: aiohttp.ClientSession, url: str) -> dict | None:
     try:
         async with session.get(
             url, headers={"user-agent": BOVINE_CLIENT_NAME}
         ) as response:
```

### Comparing `bovine-0.1.0/bovine/clients/signed_http.py` & `bovine-0.1.1/bovine/clients/signed_http.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.0/bovine/clients/signed_http_client.py` & `bovine-0.1.1/bovine/clients/signed_http_client.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.0/bovine/clients/test_event_source.py` & `bovine-0.1.1/bovine/clients/test_event_source.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.0/bovine/clients/test_lookup_account.py` & `bovine-0.1.1/bovine/clients/test_lookup_account.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.0/bovine/clients/test_signed_http.py` & `bovine-0.1.1/bovine/clients/test_signed_http.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.0/bovine/clients/test_signed_http_client.py` & `bovine-0.1.1/bovine/clients/test_signed_http_client.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.0/bovine/crypto/__init__.py` & `bovine-0.1.1/bovine/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.0/bovine/crypto/__pycache__/__init__.cpython-310.pyc` & `bovine-0.1.1/bovine/crypto/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 13 15:55:57 2023 UTC, .py size: 3999 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0d26 3864 9f0f 0000  o........&8d....
+00000000: 6f0d 0d0a 0000 0000 a4ea 3a64 9f0f 0000  o.........:d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 c400 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 6d04 5a04 0100 6400 6403 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 6d07 5a07 0100 6400 6404 6c08  m.Z.m.Z...d.d.l.
 00000060: 6d09 5a09 6d0a 5a0a 0100 6400 6405 6c0b  m.Z.m.Z...d.d.l.
 00000070: 5a0b 6406 6407 6c0c 6d0d 5a0d 6d0e 5a0e  Z.d.d.l.m.Z.m.Z.
@@ -45,184 +45,184 @@
 000002c0: 7465 da0d 7072 6976 6174 655f 6279 7465  te..private_byte
 000002d0: 7372 0400 0000 da08 456e 636f 6469 6e67  sr......Encoding
 000002e0: 5a03 5261 77da 0d50 7269 7661 7465 466f  Z.Raw..PrivateFo
 000002f0: 726d 6174 da0c 4e6f 456e 6372 7970 7469  rmat..NoEncrypti
 00000300: 6f6e 7208 0000 00da 0477 7261 7072 0700  onr......wrapr..
 00000310: 0000 da06 656e 636f 6465 2903 da0b 7072  ....encode)...pr
 00000320: 6976 6174 655f 6b65 7972 1300 0000 da07  ivate_keyr......
-00000330: 7772 6170 7065 64a9 0072 1b00 0000 fa4a  wrapped..r.....J
+00000330: 7772 6170 7065 64a9 0072 1b00 0000 fa4b  wrapped..r.....K
 00000340: 2f77 6f6f 6470 6563 6b65 722f 7372 632f  /woodpecker/src/
-00000350: 636f 6465 6265 7267 2e6f 7267 2f68 656c  codeberg.org/hel
-00000360: 6765 2f62 6f76 696e 652f 626f 7669 6e65  ge/bovine/bovine
-00000370: 2f62 6f76 696e 652f 6372 7970 746f 2f5f  /bovine/crypto/_
-00000380: 5f69 6e69 745f 5f2e 7079 da1c 6765 6e65  _init__.py..gene
-00000390: 7261 7465 5f65 6432 3535 3139 5f70 7269  rate_ed25519_pri
-000003a0: 7661 7465 5f6b 6579 0e00 0000 7310 0000  vate_key....s...
-000003b0: 000a 0204 0206 0106 0106 0106 fd0c 060c  ................
-000003c0: 0272 1d00 0000 da0f 7072 6976 6174 655f  .r......private_
-000003d0: 6b65 795f 7374 7263 0100 0000 0000 0000  key_strc........
-000003e0: 0000 0000 0200 0000 0300 0000 4300 0000  ............C...
-000003f0: 7314 0000 0074 007c 0083 017d 0174 017c  s....t.|...}.t.|
-00000400: 01a0 02a1 0083 0153 0029 017a 9e43 6f6d  .......S.).z.Com
-00000410: 7075 7465 7320 7075 626c 6963 206b 6579  putes public key
-00000420: 2069 6e20 6469 6420 6b65 7920 666f 726d   in did key form
-00000430: 206f 6620 4564 3235 3531 3920 7072 6976   of Ed25519 priv
-00000440: 6174 6520 6b65 790a 0a20 2020 203a 7061  ate key..    :pa
-00000450: 7261 6d20 7072 6976 6174 655f 6b65 795f  ram private_key_
-00000460: 7374 723a 206d 756c 7469 6261 7365 2f6d  str: multibase/m
-00000470: 756c 7469 636f 6465 6320 656e 636f 6465  ulticodec encode
-00000480: 6420 4564 3235 3531 3920 7072 6976 6174  d Ed25519 privat
-00000490: 6520 6b65 790a 0a20 2020 203a 7265 7475  e key..    :retu
-000004a0: 726e 3a20 6469 643a 6b65 7929 0372 0b00  rn: did:key).r..
-000004b0: 0000 720c 0000 00da 0a70 7562 6c69 635f  ..r......public_
-000004c0: 6b65 7929 0272 1e00 0000 7219 0000 0072  key).r....r....r
-000004d0: 1b00 0000 721b 0000 0072 1c00 0000 da16  ....r....r......
-000004e0: 7072 6976 6174 655f 6b65 795f 746f 5f64  private_key_to_d
-000004f0: 6964 5f6b 6579 1d00 0000 7304 0000 0008  id_key....s.....
-00000500: 070c 0272 2000 0000 6300 0000 0000 0000  ...r ...c.......
-00000510: 0000 0000 0004 0000 0005 0000 0043 0000  .............C..
-00000520: 0073 5c00 0000 7400 6a01 6401 6402 6403  .s\...t.j.d.d.d.
-00000530: 8d02 7d00 7c00 6a02 7403 6a04 6a05 7403  ..}.|.j.t.j.j.t.
-00000540: 6a06 6a07 7403 a008 a100 6404 8d03 7d01  j.j.t.....d...}.
-00000550: 7c00 a009 a100 7d02 7c02 6a0a 7403 6a04  |.....}.|.j.t.j.
-00000560: 6a05 7403 6a0b 6a0c 6405 8d02 7d03 7c03  j.t.j.j.d...}.|.
-00000570: a00d 6406 a101 7c01 a00d 6406 a101 6602  ..d...|...d...f.
-00000580: 5300 2907 7a6b 4765 6e65 7261 7465 7320  S.).zkGenerates 
-00000590: 6120 6e65 7720 7061 6972 206f 6620 5253  a new pair of RS
-000005a0: 4120 7075 626c 6963 2061 6e64 2070 7269  A public and pri
-000005b0: 7661 7465 206b 6579 732e 0a0a 2020 2020  vate keys...    
-000005c0: 3a72 6574 7572 6e73 3a20 7065 6d20 656e  :returns: pem en
-000005d0: 636f 6465 6420 7075 626c 6963 2061 6e64  coded public and
-000005e0: 2070 7269 7661 7465 206b 6579 0a20 2020   private key.   
-000005f0: 2069 0100 0100 6900 0800 0029 025a 0f70   i....i....).Z.p
-00000600: 7562 6c69 635f 6578 706f 6e65 6e74 5a08  ublic_exponentZ.
-00000610: 6b65 795f 7369 7a65 7210 0000 0029 0272  key_sizer....).r
-00000620: 1100 0000 7212 0000 007a 0575 7466 2d38  ....r....z.utf-8
-00000630: 290e 7206 0000 005a 1467 656e 6572 6174  ).r....Z.generat
-00000640: 655f 7072 6976 6174 655f 6b65 7972 1300  e_private_keyr..
-00000650: 0000 7204 0000 0072 1400 0000 5a03 5045  ..r....r....Z.PE
-00000660: 4d72 1500 0000 5a05 504b 4353 3872 1600  Mr....Z.PKCS8r..
-00000670: 0000 721f 0000 00da 0c70 7562 6c69 635f  ..r......public_
-00000680: 6279 7465 735a 0c50 7562 6c69 6346 6f72  bytesZ.PublicFor
-00000690: 6d61 745a 1453 7562 6a65 6374 5075 626c  matZ.SubjectPubl
-000006a0: 6963 4b65 7949 6e66 6fda 0664 6563 6f64  icKeyInfo..decod
-000006b0: 6529 0472 1900 0000 5a0f 7072 6976 6174  e).r....Z.privat
-000006c0: 655f 6b65 795f 7065 6d72 1f00 0000 5a0e  e_key_pemr....Z.
-000006d0: 7075 626c 6963 5f6b 6579 5f70 656d 721b  public_key_pemr.
-000006e0: 0000 0072 1b00 0000 721c 0000 00da 1f67  ...r....r......g
-000006f0: 656e 6572 6174 655f 7273 615f 7075 626c  enerate_rsa_publ
-00000700: 6963 5f70 7269 7661 7465 5f6b 6579 2900  ic_private_key).
-00000710: 0000 7318 0000 000e 0604 0106 0106 0106  ..s.............
-00000720: 0106 fd08 0604 0106 0106 0106 fe14 0572  ...............r
-00000730: 2300 0000 6301 0000 0000 0000 0000 0000  #...c...........
-00000740: 0002 0000 0002 0000 0043 0000 0073 0e00  .........C...s..
-00000750: 0000 7400 7c00 8301 7d01 7c01 6a01 5300  ..t.|...}.|.j.S.
-00000760: 2901 7af2 4372 6561 7465 7320 6120 7661  ).z.Creates a va
-00000770: 6c69 6461 7465 5f73 6967 6e61 7475 7265  lidate_signature
-00000780: 2066 756e 6374 696f 6e2e 2076 616c 6964   function. valid
-00000790: 6174 655f 7369 676e 6174 7572 6520 7461  ate_signature ta
-000007a0: 6b65 7320 7468 6520 7265 7175 6573 740a  kes the request.
-000007b0: 2020 2020 6173 2070 6172 616d 6574 6572      as parameter
-000007c0: 2061 6e64 2072 6574 7572 6e73 2074 6865   and returns the
-000007d0: 2070 7562 6c69 6320 6b65 7920 7572 6c20   public key url 
-000007e0: 6966 2074 6865 2068 7474 7020 7369 676e  if the http sign
-000007f0: 6174 7572 6520 6973 2076 616c 6964 2e0a  ature is valid..
-00000800: 0a20 2020 203a 7061 7261 6d20 6b65 795f  .    :param key_
-00000810: 7265 7472 6965 7665 723a 0a20 2020 2020  retriever:.     
-00000820: 2020 2041 2066 756e 6374 696f 6e20 7468     A function th
-00000830: 6174 2072 6574 7572 6e73 2074 6865 2070  at returns the p
-00000840: 7562 6c69 6320 6b65 7920 6f66 2074 6865  ublic key of the
-00000850: 2061 6374 6f72 2902 720e 0000 005a 1276   actor).r....Z.v
-00000860: 616c 6964 6174 655f 7369 676e 6174 7572  alidate_signatur
-00000870: 6529 025a 0d6b 6579 5f72 6574 7269 6576  e).Z.key_retriev
-00000880: 6572 da11 7369 676e 6174 7572 655f 6368  er..signature_ch
-00000890: 6563 6b65 7272 1b00 0000 721b 0000 0072  eckerr....r....r
-000008a0: 1c00 0000 da1d 6275 696c 645f 7661 6c69  ......build_vali
-000008b0: 6461 7465 5f68 7474 705f 7369 676e 6174  date_http_signat
-000008c0: 7572 653f 0000 0073 0400 0000 0807 0601  ure?...s........
-000008d0: 7225 0000 0063 0200 0000 0000 0000 0000  r%...c..........
-000008e0: 0000 0800 0000 0500 0000 c300 0000 7310  ..............s.
-000008f0: 0100 0081 017c 006a 0064 0119 0064 0264  .....|.j.d...d.d
-00000900: 0385 0219 007d 027c 006a 0064 0419 007d  .....}.|.j.d...}
-00000910: 0374 016a 026a 03a0 047c 006a 0064 0519  .t.j.j...|.j.d..
-00000920: 00a1 017d 047c 017c 006a 0064 0619 006b  ...}.|.|.j.d...k
-00000930: 0273 224a 0082 0174 016a 026a 03a0 057c  .s"J...t.j.j...|
-00000940: 04a1 0173 2b4a 0082 017c 006a 06a0 07a1  ...s+J...|.j....
-00000950: 0064 076b 0272 4b74 0883 00a0 0964 0864  .d.k.rKt.....d.d
-00000960: 097c 006a 0a17 00a1 02a0 0964 067c 006a  .|.j.......d.|.j
-00000970: 0064 0619 00a1 02a0 0964 057c 006a 0064  .d.......d.|.j.d
-00000980: 0519 00a1 027d 056e 337c 00a0 0ba1 0049  .....}.n3|.....I
-00000990: 0064 0348 007d 0674 0c7c 0683 017d 077c  .d.H.}.t.|...}.|
-000009a0: 077c 006a 0064 0a19 006b 0372 5f64 0353  .|.j.d...k.r_d.S
-000009b0: 0074 0883 00a0 0964 0864 0b7c 006a 0a17  .t.....d.d.|.j..
-000009c0: 00a1 02a0 0964 067c 006a 0064 0619 00a1  .....d.|.j.d....
-000009d0: 02a0 0964 057c 006a 0064 0519 00a1 02a0  ...d.|.j.d......
-000009e0: 0964 0a7c 006a 0064 0a19 00a1 027d 057c  .d.|.j.d.....}.|
-000009f0: 05a0 0d7c 027c 03a1 0272 867c 0253 0064  ...|.|...r.|.S.d
-00000a00: 0353 0029 0c61 7a01 0000 5661 6c69 6461  .S.).az...Valida
-00000a10: 7465 7320 7468 6520 604d 6f6f 2d41 7574  tes the `Moo-Aut
-00000a20: 682d 3120 3c68 7474 7073 3a2f 2f62 6c6f  h-1 <https://blo
-00000a30: 672e 6d79 6d61 7468 2e72 6f63 6b73 2f32  g.mymath.rocks/2
-00000a40: 3032 332d 3033 2d31 352f 4249 4e31 5f4d  023-03-15/BIN1_M
-00000a50: 6f6f 5f41 7574 6865 6e74 6963 6174 696f  oo_Authenticatio
-00000a60: 6e5f 616e 645f 4175 7468 6f72 6961 7469  n_and_Authoriati
-00000a70: 6f6e 3e60 5f20 7369 676e 6174 7572 6520  on>`_ signature 
-00000a80: 6f66 2074 6865 2072 6571 7565 7374 2e0a  of the request..
-00000a90: 2020 2020 5265 7475 726e 7320 7468 6520      Returns the 
-00000aa0: 6469 642d 6b65 7920 6966 2074 6865 2073  did-key if the s
-00000ab0: 6967 6e61 7475 7265 2069 7320 7661 6c69  ignature is vali
-00000ac0: 642e 0a0a 2020 2020 3a70 6172 616d 2072  d...    :param r
-00000ad0: 6571 7565 7374 3a0a 2020 2020 2020 2020  equest:.        
-00000ae0: 5468 6520 7265 7175 6573 7420 746f 2076  The request to v
-00000af0: 616c 6964 6174 6520 7468 6520 7369 676e  alidate the sign
-00000b00: 6174 7572 6520 666f 722e 0a20 2020 203a  ature for..    :
-00000b10: 7061 7261 6d20 646f 6d61 696e 3a0a 2020  param domain:.  
-00000b20: 2020 2020 2020 5468 6520 646f 6d61 696e        The domain
-00000b30: 2074 6865 2072 6571 7565 7374 2069 7320   the request is 
-00000b40: 6d61 6465 2074 6f2e 0a0a 2020 2020 3a72  made to...    :r
-00000b50: 6574 7572 6e73 3a20 4f6e 2073 7563 6365  eturns: On succe
-00000b60: 7373 2074 6865 2064 6964 206b 6579 2c20  ss the did key, 
-00000b70: 6f6e 2066 6169 6c75 7265 204e 6f6e 650a  on failure None.
-00000b80: 2020 2020 da0d 6175 7468 6f72 697a 6174      ..authorizat
-00000b90: 696f 6ee9 0b00 0000 4e7a 0f78 2d6d 6f6f  ion.....Nz.x-moo
-00000ba0: 2d73 6967 6e61 7475 7265 da04 6461 7465  -signature..date
-00000bb0: da04 686f 7374 da03 6765 747a 1028 7265  ..host..getz.(re
-00000bc0: 7175 6573 742d 7461 7267 6574 297a 0467  quest-target)z.g
-00000bd0: 6574 20da 0664 6967 6573 747a 0570 6f73  et ..digestz.pos
-00000be0: 7420 290e da07 6865 6164 6572 73da 0662  t )...headers..b
-00000bf0: 6f76 696e 65da 0575 7469 6c73 7228 0000  ovine..utilsr(..
-00000c00: 005a 0970 6172 7365 5f67 6d74 5a14 6368  .Z.parse_gmtZ.ch
-00000c10: 6563 6b5f 6d61 785f 6f66 6673 6574 5f6e  eck_max_offset_n
-00000c20: 6f77 da06 6d65 7468 6f64 da05 6c6f 7765  ow..method..lowe
-00000c30: 7272 0d00 0000 da0a 7769 7468 5f66 6965  rr......with_fie
-00000c40: 6c64 da04 7061 7468 da08 6765 745f 6461  ld..path..get_da
-00000c50: 7461 720a 0000 005a 0e65 6432 3535 3139  tar....Z.ed25519
-00000c60: 5f76 6572 6966 7929 08da 0772 6571 7565  _verify)...reque
-00000c70: 7374 da06 646f 6d61 696e 5a06 6469 646b  st..domainZ.didk
-00000c80: 6579 da09 7369 676e 6174 7572 65da 0264  ey..signature..d
-00000c90: 74da 0e68 7474 705f 7369 676e 6174 7572  t..http_signatur
-00000ca0: 65da 0872 6177 5f64 6174 6172 2b00 0000  e..raw_datar+...
-00000cb0: 721b 0000 0072 1b00 0000 721c 0000 00da  r....r....r.....
-00000cc0: 1b76 616c 6964 6174 655f 6d6f 6f5f 6175  .validate_moo_au
-00000cd0: 7468 5f73 6967 6e61 7475 7265 4a00 0000  th_signatureJ...
-00000ce0: 7332 0000 0002 8012 0b0a 0114 0212 0112  s2..............
-00000cf0: 010e 0204 020e 010e 010e 0104 fc0e 0708  ................
-00000d00: 010e 0104 0104 020e 010e 010e 010e 0102  ................
-00000d10: fb0c 0804 0104 0172 3a00 0000 291a da06  .......r:...)...
-00000d20: 7479 7069 6e67 7202 0000 0072 0300 0000  typingr....r....
-00000d30: 5a1e 6372 7970 746f 6772 6170 6879 2e68  Z.cryptography.h
-00000d40: 617a 6d61 742e 7072 696d 6974 6976 6573  azmat.primitives
-00000d50: 7204 0000 005a 2963 7279 7074 6f67 7261  r....Z)cryptogra
-00000d60: 7068 792e 6861 7a6d 6174 2e70 7269 6d69  phy.hazmat.primi
-00000d70: 7469 7665 732e 6173 796d 6d65 7472 6963  tives.asymmetric
-00000d80: 7205 0000 0072 0600 0000 5a0c 6d75 6c74  r....r....Z.mult
-00000d90: 6966 6f72 6d61 7473 7207 0000 0072 0800  iformatsr....r..
-00000da0: 0000 722d 0000 00da 0668 656c 7065 7272  ..r-.....helperr
-00000db0: 0a00 0000 720b 0000 0072 0c00 0000 7238  ....r....r....r8
-00000dc0: 0000 0072 0d00 0000 7224 0000 0072 0e00  ...r....r$...r..
-00000dd0: 0000 da03 7374 7272 1d00 0000 7220 0000  ....strr....r ..
-00000de0: 0072 2300 0000 7225 0000 0072 3a00 0000  .r#...r%...r:...
-00000df0: 721b 0000 0072 1b00 0000 721b 0000 0072  r....r....r....r
-00000e00: 1c00 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
-00000e10: 0000 731a 0000 0010 000c 0210 0110 0108  ..s.............
-00000e20: 0214 020c 010c 010e 0312 0f16 0c08 1616  ................
-00000e30: 0b                                       .
+00000350: 636f 6465 6265 7267 2e6f 7267 2f62 6f76  codeberg.org/bov
+00000360: 696e 652f 626f 7669 6e65 2f62 6f76 696e  ine/bovine/bovin
+00000370: 652f 626f 7669 6e65 2f63 7279 7074 6f2f  e/bovine/crypto/
+00000380: 5f5f 696e 6974 5f5f 2e70 79da 1c67 656e  __init__.py..gen
+00000390: 6572 6174 655f 6564 3235 3531 395f 7072  erate_ed25519_pr
+000003a0: 6976 6174 655f 6b65 790e 0000 0073 1000  ivate_key....s..
+000003b0: 0000 0a02 0402 0601 0601 0601 06fd 0c06  ................
+000003c0: 0c02 721d 0000 00da 0f70 7269 7661 7465  ..r......private
+000003d0: 5f6b 6579 5f73 7472 6301 0000 0000 0000  _key_strc.......
+000003e0: 0000 0000 0002 0000 0003 0000 0043 0000  .............C..
+000003f0: 0073 1400 0000 7400 7c00 8301 7d01 7401  .s....t.|...}.t.
+00000400: 7c01 a002 a100 8301 5300 2901 7a9e 436f  |.......S.).z.Co
+00000410: 6d70 7574 6573 2070 7562 6c69 6320 6b65  mputes public ke
+00000420: 7920 696e 2064 6964 206b 6579 2066 6f72  y in did key for
+00000430: 6d20 6f66 2045 6432 3535 3139 2070 7269  m of Ed25519 pri
+00000440: 7661 7465 206b 6579 0a0a 2020 2020 3a70  vate key..    :p
+00000450: 6172 616d 2070 7269 7661 7465 5f6b 6579  aram private_key
+00000460: 5f73 7472 3a20 6d75 6c74 6962 6173 652f  _str: multibase/
+00000470: 6d75 6c74 6963 6f64 6563 2065 6e63 6f64  multicodec encod
+00000480: 6564 2045 6432 3535 3139 2070 7269 7661  ed Ed25519 priva
+00000490: 7465 206b 6579 0a0a 2020 2020 3a72 6574  te key..    :ret
+000004a0: 7572 6e3a 2064 6964 3a6b 6579 2903 720b  urn: did:key).r.
+000004b0: 0000 0072 0c00 0000 da0a 7075 626c 6963  ...r......public
+000004c0: 5f6b 6579 2902 721e 0000 0072 1900 0000  _key).r....r....
+000004d0: 721b 0000 0072 1b00 0000 721c 0000 00da  r....r....r.....
+000004e0: 1670 7269 7661 7465 5f6b 6579 5f74 6f5f  .private_key_to_
+000004f0: 6469 645f 6b65 791d 0000 0073 0400 0000  did_key....s....
+00000500: 0807 0c02 7220 0000 0063 0000 0000 0000  ....r ...c......
+00000510: 0000 0000 0000 0400 0000 0500 0000 4300  ..............C.
+00000520: 0000 735c 0000 0074 006a 0164 0164 0264  ..s\...t.j.d.d.d
+00000530: 038d 027d 007c 006a 0274 036a 046a 0574  ...}.|.j.t.j.j.t
+00000540: 036a 066a 0774 03a0 08a1 0064 048d 037d  .j.j.t.....d...}
+00000550: 017c 00a0 09a1 007d 027c 026a 0a74 036a  .|.....}.|.j.t.j
+00000560: 046a 0574 036a 0b6a 0c64 058d 027d 037c  .j.t.j.j.d...}.|
+00000570: 03a0 0d64 06a1 017c 01a0 0d64 06a1 0166  ...d...|...d...f
+00000580: 0253 0029 077a 6b47 656e 6572 6174 6573  .S.).zkGenerates
+00000590: 2061 206e 6577 2070 6169 7220 6f66 2052   a new pair of R
+000005a0: 5341 2070 7562 6c69 6320 616e 6420 7072  SA public and pr
+000005b0: 6976 6174 6520 6b65 7973 2e0a 0a20 2020  ivate keys...   
+000005c0: 203a 7265 7475 726e 733a 2070 656d 2065   :returns: pem e
+000005d0: 6e63 6f64 6564 2070 7562 6c69 6320 616e  ncoded public an
+000005e0: 6420 7072 6976 6174 6520 6b65 790a 2020  d private key.  
+000005f0: 2020 6901 0001 0069 0008 0000 2902 5a0f    i....i....).Z.
+00000600: 7075 626c 6963 5f65 7870 6f6e 656e 745a  public_exponentZ
+00000610: 086b 6579 5f73 697a 6572 1000 0000 2902  .key_sizer....).
+00000620: 7211 0000 0072 1200 0000 7a05 7574 662d  r....r....z.utf-
+00000630: 3829 0e72 0600 0000 5a14 6765 6e65 7261  8).r....Z.genera
+00000640: 7465 5f70 7269 7661 7465 5f6b 6579 7213  te_private_keyr.
+00000650: 0000 0072 0400 0000 7214 0000 005a 0350  ...r....r....Z.P
+00000660: 454d 7215 0000 005a 0550 4b43 5338 7216  EMr....Z.PKCS8r.
+00000670: 0000 0072 1f00 0000 da0c 7075 626c 6963  ...r......public
+00000680: 5f62 7974 6573 5a0c 5075 626c 6963 466f  _bytesZ.PublicFo
+00000690: 726d 6174 5a14 5375 626a 6563 7450 7562  rmatZ.SubjectPub
+000006a0: 6c69 634b 6579 496e 666f da06 6465 636f  licKeyInfo..deco
+000006b0: 6465 2904 7219 0000 005a 0f70 7269 7661  de).r....Z.priva
+000006c0: 7465 5f6b 6579 5f70 656d 721f 0000 005a  te_key_pemr....Z
+000006d0: 0e70 7562 6c69 635f 6b65 795f 7065 6d72  .public_key_pemr
+000006e0: 1b00 0000 721b 0000 0072 1c00 0000 da1f  ....r....r......
+000006f0: 6765 6e65 7261 7465 5f72 7361 5f70 7562  generate_rsa_pub
+00000700: 6c69 635f 7072 6976 6174 655f 6b65 7929  lic_private_key)
+00000710: 0000 0073 1800 0000 0e06 0401 0601 0601  ...s............
+00000720: 0601 06fd 0806 0401 0601 0601 06fe 1405  ................
+00000730: 7223 0000 0063 0100 0000 0000 0000 0000  r#...c..........
+00000740: 0000 0200 0000 0200 0000 4300 0000 730e  ..........C...s.
+00000750: 0000 0074 007c 0083 017d 017c 016a 0153  ...t.|...}.|.j.S
+00000760: 0029 017a f243 7265 6174 6573 2061 2076  .).z.Creates a v
+00000770: 616c 6964 6174 655f 7369 676e 6174 7572  alidate_signatur
+00000780: 6520 6675 6e63 7469 6f6e 2e20 7661 6c69  e function. vali
+00000790: 6461 7465 5f73 6967 6e61 7475 7265 2074  date_signature t
+000007a0: 616b 6573 2074 6865 2072 6571 7565 7374  akes the request
+000007b0: 0a20 2020 2061 7320 7061 7261 6d65 7465  .    as paramete
+000007c0: 7220 616e 6420 7265 7475 726e 7320 7468  r and returns th
+000007d0: 6520 7075 626c 6963 206b 6579 2075 726c  e public key url
+000007e0: 2069 6620 7468 6520 6874 7470 2073 6967   if the http sig
+000007f0: 6e61 7475 7265 2069 7320 7661 6c69 642e  nature is valid.
+00000800: 0a0a 2020 2020 3a70 6172 616d 206b 6579  ..    :param key
+00000810: 5f72 6574 7269 6576 6572 3a0a 2020 2020  _retriever:.    
+00000820: 2020 2020 4120 6675 6e63 7469 6f6e 2074      A function t
+00000830: 6861 7420 7265 7475 726e 7320 7468 6520  hat returns the 
+00000840: 7075 626c 6963 206b 6579 206f 6620 7468  public key of th
+00000850: 6520 6163 746f 7229 0272 0e00 0000 5a12  e actor).r....Z.
+00000860: 7661 6c69 6461 7465 5f73 6967 6e61 7475  validate_signatu
+00000870: 7265 2902 5a0d 6b65 795f 7265 7472 6965  re).Z.key_retrie
+00000880: 7665 72da 1173 6967 6e61 7475 7265 5f63  ver..signature_c
+00000890: 6865 636b 6572 721b 0000 0072 1b00 0000  heckerr....r....
+000008a0: 721c 0000 00da 1d62 7569 6c64 5f76 616c  r......build_val
+000008b0: 6964 6174 655f 6874 7470 5f73 6967 6e61  idate_http_signa
+000008c0: 7475 7265 3f00 0000 7304 0000 0008 0706  ture?...s.......
+000008d0: 0172 2500 0000 6302 0000 0000 0000 0000  .r%...c.........
+000008e0: 0000 0008 0000 0005 0000 00c3 0000 0073  ...............s
+000008f0: 1001 0000 8101 7c00 6a00 6401 1900 6402  ......|.j.d...d.
+00000900: 6403 8502 1900 7d02 7c00 6a00 6404 1900  d.....}.|.j.d...
+00000910: 7d03 7401 6a02 6a03 a004 7c00 6a00 6405  }.t.j.j...|.j.d.
+00000920: 1900 a101 7d04 7c01 7c00 6a00 6406 1900  ....}.|.|.j.d...
+00000930: 6b02 7322 4a00 8201 7401 6a02 6a03 a005  k.s"J...t.j.j...
+00000940: 7c04 a101 732b 4a00 8201 7c00 6a06 a007  |...s+J...|.j...
+00000950: a100 6407 6b02 724b 7408 8300 a009 6408  ..d.k.rKt.....d.
+00000960: 6409 7c00 6a0a 1700 a102 a009 6406 7c00  d.|.j.......d.|.
+00000970: 6a00 6406 1900 a102 a009 6405 7c00 6a00  j.d.......d.|.j.
+00000980: 6405 1900 a102 7d05 6e33 7c00 a00b a100  d.....}.n3|.....
+00000990: 4900 6403 4800 7d06 740c 7c06 8301 7d07  I.d.H.}.t.|...}.
+000009a0: 7c07 7c00 6a00 640a 1900 6b03 725f 6403  |.|.j.d...k.r_d.
+000009b0: 5300 7408 8300 a009 6408 640b 7c00 6a0a  S.t.....d.d.|.j.
+000009c0: 1700 a102 a009 6406 7c00 6a00 6406 1900  ......d.|.j.d...
+000009d0: a102 a009 6405 7c00 6a00 6405 1900 a102  ....d.|.j.d.....
+000009e0: a009 640a 7c00 6a00 640a 1900 a102 7d05  ..d.|.j.d.....}.
+000009f0: 7c05 a00d 7c02 7c03 a102 7286 7c02 5300  |...|.|...r.|.S.
+00000a00: 6403 5300 290c 617a 0100 0056 616c 6964  d.S.).az...Valid
+00000a10: 6174 6573 2074 6865 2060 4d6f 6f2d 4175  ates the `Moo-Au
+00000a20: 7468 2d31 203c 6874 7470 733a 2f2f 626c  th-1 <https://bl
+00000a30: 6f67 2e6d 796d 6174 682e 726f 636b 732f  og.mymath.rocks/
+00000a40: 3230 3233 2d30 332d 3135 2f42 494e 315f  2023-03-15/BIN1_
+00000a50: 4d6f 6f5f 4175 7468 656e 7469 6361 7469  Moo_Authenticati
+00000a60: 6f6e 5f61 6e64 5f41 7574 686f 7269 6174  on_and_Authoriat
+00000a70: 696f 6e3e 605f 2073 6967 6e61 7475 7265  ion>`_ signature
+00000a80: 206f 6620 7468 6520 7265 7175 6573 742e   of the request.
+00000a90: 0a20 2020 2052 6574 7572 6e73 2074 6865  .    Returns the
+00000aa0: 2064 6964 2d6b 6579 2069 6620 7468 6520   did-key if the 
+00000ab0: 7369 676e 6174 7572 6520 6973 2076 616c  signature is val
+00000ac0: 6964 2e0a 0a20 2020 203a 7061 7261 6d20  id...    :param 
+00000ad0: 7265 7175 6573 743a 0a20 2020 2020 2020  request:.       
+00000ae0: 2054 6865 2072 6571 7565 7374 2074 6f20   The request to 
+00000af0: 7661 6c69 6461 7465 2074 6865 2073 6967  validate the sig
+00000b00: 6e61 7475 7265 2066 6f72 2e0a 2020 2020  nature for..    
+00000b10: 3a70 6172 616d 2064 6f6d 6169 6e3a 0a20  :param domain:. 
+00000b20: 2020 2020 2020 2054 6865 2064 6f6d 6169         The domai
+00000b30: 6e20 7468 6520 7265 7175 6573 7420 6973  n the request is
+00000b40: 206d 6164 6520 746f 2e0a 0a20 2020 203a   made to...    :
+00000b50: 7265 7475 726e 733a 204f 6e20 7375 6363  returns: On succ
+00000b60: 6573 7320 7468 6520 6469 6420 6b65 792c  ess the did key,
+00000b70: 206f 6e20 6661 696c 7572 6520 4e6f 6e65   on failure None
+00000b80: 0a20 2020 20da 0d61 7574 686f 7269 7a61  .    ..authoriza
+00000b90: 7469 6f6e e90b 0000 004e 7a0f 782d 6d6f  tion.....Nz.x-mo
+00000ba0: 6f2d 7369 676e 6174 7572 65da 0464 6174  o-signature..dat
+00000bb0: 65da 0468 6f73 74da 0367 6574 7a10 2872  e..host..getz.(r
+00000bc0: 6571 7565 7374 2d74 6172 6765 7429 7a04  equest-target)z.
+00000bd0: 6765 7420 da06 6469 6765 7374 7a05 706f  get ..digestz.po
+00000be0: 7374 2029 0eda 0768 6561 6465 7273 da06  st )...headers..
+00000bf0: 626f 7669 6e65 da05 7574 696c 7372 2800  bovine..utilsr(.
+00000c00: 0000 5a09 7061 7273 655f 676d 745a 1463  ..Z.parse_gmtZ.c
+00000c10: 6865 636b 5f6d 6178 5f6f 6666 7365 745f  heck_max_offset_
+00000c20: 6e6f 77da 066d 6574 686f 64da 056c 6f77  now..method..low
+00000c30: 6572 720d 0000 00da 0a77 6974 685f 6669  err......with_fi
+00000c40: 656c 64da 0470 6174 68da 0867 6574 5f64  eld..path..get_d
+00000c50: 6174 6172 0a00 0000 5a0e 6564 3235 3531  atar....Z.ed2551
+00000c60: 395f 7665 7269 6679 2908 da07 7265 7175  9_verify)...requ
+00000c70: 6573 74da 0664 6f6d 6169 6e5a 0664 6964  est..domainZ.did
+00000c80: 6b65 79da 0973 6967 6e61 7475 7265 da02  key..signature..
+00000c90: 6474 da0e 6874 7470 5f73 6967 6e61 7475  dt..http_signatu
+00000ca0: 7265 da08 7261 775f 6461 7461 722b 0000  re..raw_datar+..
+00000cb0: 0072 1b00 0000 721b 0000 0072 1c00 0000  .r....r....r....
+00000cc0: da1b 7661 6c69 6461 7465 5f6d 6f6f 5f61  ..validate_moo_a
+00000cd0: 7574 685f 7369 676e 6174 7572 654a 0000  uth_signatureJ..
+00000ce0: 0073 3200 0000 0280 120b 0a01 1402 1201  .s2.............
+00000cf0: 1201 0e02 0402 0e01 0e01 0e01 04fc 0e07  ................
+00000d00: 0801 0e01 0401 0402 0e01 0e01 0e01 0e01  ................
+00000d10: 02fb 0c08 0401 0401 723a 0000 0029 1ada  ........r:...)..
+00000d20: 0674 7970 696e 6772 0200 0000 7203 0000  .typingr....r...
+00000d30: 005a 1e63 7279 7074 6f67 7261 7068 792e  .Z.cryptography.
+00000d40: 6861 7a6d 6174 2e70 7269 6d69 7469 7665  hazmat.primitive
+00000d50: 7372 0400 0000 5a29 6372 7970 746f 6772  sr....Z)cryptogr
+00000d60: 6170 6879 2e68 617a 6d61 742e 7072 696d  aphy.hazmat.prim
+00000d70: 6974 6976 6573 2e61 7379 6d6d 6574 7269  itives.asymmetri
+00000d80: 6372 0500 0000 7206 0000 005a 0c6d 756c  cr....r....Z.mul
+00000d90: 7469 666f 726d 6174 7372 0700 0000 7208  tiformatsr....r.
+00000da0: 0000 0072 2d00 0000 da06 6865 6c70 6572  ...r-.....helper
+00000db0: 720a 0000 0072 0b00 0000 720c 0000 0072  r....r....r....r
+00000dc0: 3800 0000 720d 0000 0072 2400 0000 720e  8...r....r$...r.
+00000dd0: 0000 00da 0373 7472 721d 0000 0072 2000  .....strr....r .
+00000de0: 0000 7223 0000 0072 2500 0000 723a 0000  ..r#...r%...r:..
+00000df0: 0072 1b00 0000 721b 0000 0072 1b00 0000  .r....r....r....
+00000e00: 721c 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
+00000e10: 0000 0073 1a00 0000 1000 0c02 1001 1001  ...s............
+00000e20: 0802 1402 0c01 0c01 0e03 120f 160c 0816  ................
+00000e30: 160b                                     ..
```

### Comparing `bovine-0.1.0/bovine/crypto/__pycache__/helper.cpython-310.pyc` & `bovine-0.1.1/bovine/crypto/__pycache__/helper.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 13 15:55:57 2023 UTC, .py size: 2764 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0d26 3864 cc0a 0000  o........&8d....
+00000000: 6f0d 0d0a 0000 0000 a4ea 3a64 680a 0000  o.........:dh...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 d800 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6402 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6400 6403 6c05 6d06 5a06 6d07 5a07  ..d.d.l.m.Z.m.Z.
 00000060: 0100 6400 6404 6c08 6d09 5a09 6d0a 5a0a  ..d.d.l.m.Z.m.Z.
 00000070: 6d0b 5a0b 0100 6400 6405 6c0c 6d0d 5a0d  m.Z...d.d.l.m.Z.
@@ -36,148 +36,144 @@
 00000230: 7574 662d 387a 0873 6861 2d32 3536 3d29  utf-8z.sha-256=)
 00000240: 09da 0a69 7369 6e73 7461 6e63 65da 0373  ...isinstance..s
 00000250: 7472 da06 656e 636f 6465 da06 6261 7365  tr..encode..base
 00000260: 3634 da12 7374 616e 6461 7264 5f62 3634  64..standard_b64
 00000270: 656e 636f 6465 da07 6861 7368 6c69 62da  encode..hashlib.
 00000280: 0673 6861 3235 36da 0664 6967 6573 74da  .sha256..digest.
 00000290: 0664 6563 6f64 6529 0272 0c00 0000 7216  .decode).r....r.
-000002a0: 0000 00a9 0072 1800 0000 fa48 2f77 6f6f  .....r.....H/woo
+000002a0: 0000 00a9 0072 1800 0000 fa49 2f77 6f6f  .....r.....I/woo
 000002b0: 6470 6563 6b65 722f 7372 632f 636f 6465  dpecker/src/code
-000002c0: 6265 7267 2e6f 7267 2f68 656c 6765 2f62  berg.org/helge/b
-000002d0: 6f76 696e 652f 626f 7669 6e65 2f62 6f76  ovine/bovine/bov
-000002e0: 696e 652f 6372 7970 746f 2f68 656c 7065  ine/crypto/helpe
-000002f0: 722e 7079 da15 636f 6e74 656e 745f 6469  r.py..content_di
-00000300: 6765 7374 5f73 6861 3235 3611 0000 0073  gest_sha256....s
-00000310: 0800 0000 0a02 0a01 1a02 0801 721a 0000  ............r...
-00000320: 0063 0200 0000 0000 0000 0000 0000 0400  .c..............
-00000330: 0000 0a00 0000 4300 0000 738c 0000 007c  ......C...s....|
-00000340: 00a0 0064 0164 02a1 027d 007a 1374 017c  ...d.d...}.z.t.|
-00000350: 00a0 0264 03a1 0164 0064 048d 027d 0274  ...d...d.d...}.t
-00000360: 037c 0274 046a 0583 0273 184a 0082 0157  .|.t.j...s.J...W
-00000370: 006e 1804 0074 0679 3101 007d 0301 007a  .n...t.y1..}...z
-00000380: 0c74 07a0 087c 03a1 0101 0074 07a0 087c  .t...|.....t...|
-00000390: 00a1 0101 007c 0382 0164 007d 037e 0377  .....|...d.}.~.w
-000003a0: 0177 0074 09a0 0a7c 02a0 0b7c 01a0 0264  .w.t...|...|...d
-000003b0: 03a1 0174 0ca0 0da1 0074 0ea0 0fa1 00a1  ...t.....t......
-000003c0: 03a1 01a0 1064 03a1 0153 0029 054e fa02  .....d...S.).N..
-000003d0: 5c6e da01 0a72 0e00 0000 2901 da08 7061  \n...r....)...pa
-000003e0: 7373 776f 7264 2911 da07 7265 706c 6163  ssword)...replac
-000003f0: 6572 0800 0000 7211 0000 0072 0f00 0000  er....r....r....
-00000400: 7207 0000 00da 0d52 5341 5072 6976 6174  r......RSAPrivat
-00000410: 654b 6579 da09 4578 6365 7074 696f 6eda  eKey..Exception.
-00000420: 066c 6f67 6765 72da 0565 7272 6f72 7212  .logger..errorr.
-00000430: 0000 0072 1300 0000 da04 7369 676e 7206  ...r......signr.
-00000440: 0000 00da 0850 4b43 5331 7631 3572 0300  .....PKCS1v15r..
-00000450: 0000 da06 5348 4132 3536 7217 0000 0029  ....SHA256r....)
-00000460: 04da 0b70 7269 7661 7465 5f6b 6579 da07  ...private_key..
-00000470: 6d65 7373 6167 65da 036b 6579 da01 6572  message..key..er
-00000480: 1800 0000 7218 0000 0072 1900 0000 da0c  ....r....r......
-00000490: 7369 676e 5f6d 6573 7361 6765 1a00 0000  sign_message....
-000004a0: 7326 0000 000c 0102 0112 0114 010e 010a  s&..............
-000004b0: 010a 0104 0108 8002 fd04 0504 0108 0106  ................
-000004c0: 0106 0102 fd02 ff06 0602 fa72 2a00 0000  ...........r*...
-000004d0: 6303 0000 0000 0000 0000 0000 0004 0000  c...............
-000004e0: 0008 0000 0043 0000 0073 7400 0000 7c00  .....C...st...|.
-000004f0: a000 6401 6402 a102 7d00 7401 7c00 a002  ..d.d...}.t.|...
-00000500: 6403 a101 8301 7d03 7403 7c03 7404 6a05  d.....}.t.|.t.j.
-00000510: 8302 7315 4a00 8201 7a15 7c03 a006 7407  ..s.J...z.|...t.
-00000520: a008 7c02 a101 7c01 a002 6403 a101 7409  ..|...|...d...t.
-00000530: a00a a100 740b a00c a100 a104 0100 5700  ....t.........W.
-00000540: 6406 5300 0400 740d 7939 0100 0100 0100  d.S...t.y9......
-00000550: 740e a00f 6404 a101 0100 5900 6405 5300  t...d.....Y.d.S.
-00000560: 7700 2907 4e72 1b00 0000 721c 0000 0072  w.).Nr....r....r
-00000570: 0e00 0000 7a11 696e 7661 6c69 6420 7369  ....z.invalid si
-00000580: 676e 6174 7572 6546 5429 1072 1e00 0000  gnatureFT).r....
-00000590: 7209 0000 0072 1100 0000 720f 0000 0072  r....r....r....r
-000005a0: 0700 0000 da0c 5253 4150 7562 6c69 634b  ......RSAPublicK
-000005b0: 6579 da06 7665 7269 6679 7212 0000 00da  ey..verifyr.....
-000005c0: 1273 7461 6e64 6172 645f 6236 3464 6563  .standard_b64dec
-000005d0: 6f64 6572 0600 0000 7224 0000 0072 0300  oder....r$...r..
-000005e0: 0000 7225 0000 0072 0200 0000 7221 0000  ..r%...r....r!..
-000005f0: 00da 0777 6172 6e69 6e67 2904 da0a 7075  ...warning)...pu
-00000600: 626c 6963 5f6b 6579 7227 0000 00da 0973  blic_keyr'.....s
-00000610: 6967 6e61 7475 7265 5a11 7075 626c 6963  ignatureZ.public
-00000620: 5f6b 6579 5f6c 6f61 6465 6472 1800 0000  _key_loadedr....
-00000630: 7218 0000 0072 1900 0000 da10 7665 7269  r....r......veri
-00000640: 6679 5f73 6967 6e61 7475 7265 2d00 0000  fy_signature-...
-00000650: 731e 0000 000c 010e 0110 0202 0204 0108  s...............
-00000660: 0108 0106 0106 0106 fc04 0a0c fc0a 0106  ................
-00000670: 0102 fe72 3100 0000 722f 0000 0063 0100  ...r1...r/...c..
-00000680: 0000 0000 0000 0000 0000 0400 0000 0400  ................
-00000690: 0000 4300 0000 7336 0000 007c 006a 0074  ..C...s6...|.j.t
-000006a0: 016a 026a 0374 016a 046a 0364 018d 027d  .j.j.t.j.j.d...}
-000006b0: 0174 05a0 0664 027c 01a1 027d 0274 07a0  .t...d.|...}.t..
-000006c0: 087c 0264 03a1 027d 0364 047c 0317 0053  .|.d...}.d.|...S
-000006d0: 0029 054e 2902 da08 656e 636f 6469 6e67  .).N)...encoding
-000006e0: da06 666f 726d 6174 fa0b 6564 3235 3531  ..format..ed2551
-000006f0: 392d 7075 62da 0962 6173 6535 3862 7463  9-pub..base58btc
-00000700: fa08 6469 643a 6b65 793a 2909 da0c 7075  ..did:key:)...pu
-00000710: 626c 6963 5f62 7974 6573 7204 0000 00da  blic_bytesr.....
-00000720: 0845 6e63 6f64 696e 67da 0352 6177 da0c  .Encoding..Raw..
-00000730: 5075 626c 6963 466f 726d 6174 720b 0000  PublicFormatr...
-00000740: 00da 0477 7261 7072 0a00 0000 7211 0000  ...wrapr....r...
-00000750: 0029 0472 2f00 0000 7237 0000 00da 0777  .).r/...r7.....w
-00000760: 7261 7070 6564 da07 656e 636f 6465 6472  rapped..encodedr
-00000770: 1800 0000 7218 0000 0072 1900 0000 da15  ....r....r......
-00000780: 7075 626c 6963 5f6b 6579 5f74 6f5f 6469  public_key_to_di
-00000790: 645f 6b65 7941 0000 0073 0e00 0000 0401  d_keyA...s......
-000007a0: 0601 0601 06fe 0c05 0c01 0802 723e 0000  ............r>..
-000007b0: 00da 0364 6964 6301 0000 0000 0000 0000  ...didc.........
-000007c0: 0000 0004 0000 0005 0000 0043 0000 0073  ...........C...s
-000007d0: 4800 0000 7c00 a000 6401 a101 7307 4a00  H...|...d...s.J.
-000007e0: 8201 7401 a002 7c00 6402 6400 8502 1900  ..t...|.d.d.....
-000007f0: a101 7d01 7403 a004 7c01 a101 5c02 7d02  ..}.t...|...\.}.
-00000800: 7d03 7c02 6a05 6403 6b02 731e 4a00 8201  }.|.j.d.k.s.J...
-00000810: 7406 6a07 a008 7c03 a101 5300 2904 4e72  t.j...|...S.).Nr
-00000820: 3600 0000 e908 0000 0072 3400 0000 2909  6........r4...).
-00000830: da0a 7374 6172 7473 7769 7468 720a 0000  ..startswithr...
-00000840: 0072 1700 0000 720b 0000 00da 0675 6e77  .r....r......unw
-00000850: 7261 70da 046e 616d 6572 0500 0000 da10  rap..namer......
-00000860: 4564 3235 3531 3950 7562 6c69 634b 6579  Ed25519PublicKey
-00000870: da11 6672 6f6d 5f70 7562 6c69 635f 6279  ..from_public_by
-00000880: 7465 7329 0472 3f00 0000 da07 6465 636f  tes).r?.....deco
-00000890: 6465 64da 0563 6f64 6563 da09 6b65 795f  ded..codec..key_
-000008a0: 6279 7465 7372 1800 0000 7218 0000 0072  bytesr....r....r
-000008b0: 1900 0000 da15 6469 645f 6b65 795f 746f  ......did_key_to
-000008c0: 5f70 7562 6c69 635f 6b65 794d 0000 0073  _public_keyM...s
-000008d0: 0a00 0000 0e01 1201 0e01 0e01 0c02 7249  ..............rI
-000008e0: 0000 00da 0f70 7269 7661 7465 5f6b 6579  .....private_key
-000008f0: 5f73 7472 6301 0000 0000 0000 0000 0000  _strc...........
-00000900: 0004 0000 0003 0000 0043 0000 0073 3200  .........C...s2.
-00000910: 0000 7400 a001 7c00 a101 7d01 7402 a003  ..t...|...}.t...
-00000920: 7c01 a101 5c02 7d02 7d03 7c02 6a04 6401  |...\.}.}.|.j.d.
-00000930: 6b02 7313 4a00 8201 7405 6a06 a007 7c03  k.s.J...t.j...|.
-00000940: a101 5300 2902 4e7a 0c65 6432 3535 3139  ..S.).Nz.ed25519
-00000950: 2d70 7269 7629 0872 0a00 0000 7217 0000  -priv).r....r...
-00000960: 0072 0b00 0000 7242 0000 0072 4300 0000  .r....rB...rC...
-00000970: 7205 0000 00da 1145 6432 3535 3139 5072  r......Ed25519Pr
-00000980: 6976 6174 654b 6579 da12 6672 6f6d 5f70  ivateKey..from_p
-00000990: 7269 7661 7465 5f62 7974 6573 2904 724a  rivate_bytes).rJ
-000009a0: 0000 0072 4600 0000 7247 0000 0072 4800  ...rF...rG...rH.
-000009b0: 0000 7218 0000 0072 1800 0000 7219 0000  ..r....r....r...
-000009c0: 00da 1670 7269 7661 7465 5f6b 6579 5f74  ...private_key_t
-000009d0: 6f5f 6564 3235 3531 3956 0000 0073 0800  o_ed25519V...s..
-000009e0: 0000 0a01 0e01 0e01 0c02 724d 0000 0029  ..........rM...)
-000009f0: 1f72 1200 0000 7214 0000 00da 076c 6f67  .r....r......log
-00000a00: 6769 6e67 da17 6372 7970 746f 6772 6170  ging..cryptograp
-00000a10: 6879 2e65 7863 6570 7469 6f6e 7372 0200  hy.exceptionsr..
-00000a20: 0000 da1e 6372 7970 746f 6772 6170 6879  ....cryptography
-00000a30: 2e68 617a 6d61 742e 7072 696d 6974 6976  .hazmat.primitiv
-00000a40: 6573 7203 0000 0072 0400 0000 da29 6372  esr....r.....)cr
+000002c0: 6265 7267 2e6f 7267 2f62 6f76 696e 652f  berg.org/bovine/
+000002d0: 626f 7669 6e65 2f62 6f76 696e 652f 626f  bovine/bovine/bo
+000002e0: 7669 6e65 2f63 7279 7074 6f2f 6865 6c70  vine/crypto/help
+000002f0: 6572 2e70 79da 1563 6f6e 7465 6e74 5f64  er.py..content_d
+00000300: 6967 6573 745f 7368 6132 3536 1100 0000  igest_sha256....
+00000310: 7308 0000 000a 020a 011a 0208 0172 1a00  s............r..
+00000320: 0000 6302 0000 0000 0000 0000 0000 0004  ..c.............
+00000330: 0000 000a 0000 0043 0000 0073 8000 0000  .......C...s....
+00000340: 7a13 7400 7c00 a001 6401 a101 6400 6402  z.t.|...d...d.d.
+00000350: 8d02 7d02 7402 7c02 7403 6a04 8302 7312  ..}.t.|.t.j...s.
+00000360: 4a00 8201 5700 6e18 0400 7405 792b 0100  J...W.n...t.y+..
+00000370: 7d03 0100 7a0c 7406 a007 7c03 a101 0100  }...z.t...|.....
+00000380: 7406 a007 7c00 a101 0100 7c03 8201 6400  t...|.....|...d.
+00000390: 7d03 7e03 7701 7700 7408 a009 7c02 a00a  }.~.w.w.t...|...
+000003a0: 7c01 a001 6401 a101 740b a00c a100 740d  |...d...t.....t.
+000003b0: a00e a100 a103 a101 a00f 6401 a101 5300  ..........d...S.
+000003c0: 2903 4e72 0e00 0000 2901 da08 7061 7373  ).Nr....)...pass
+000003d0: 776f 7264 2910 7208 0000 0072 1100 0000  word).r....r....
+000003e0: 720f 0000 0072 0700 0000 da0d 5253 4150  r....r......RSAP
+000003f0: 7269 7661 7465 4b65 79da 0945 7863 6570  rivateKey..Excep
+00000400: 7469 6f6e da06 6c6f 6767 6572 da05 6572  tion..logger..er
+00000410: 726f 7272 1200 0000 7213 0000 00da 0473  rorr....r......s
+00000420: 6967 6e72 0600 0000 da08 504b 4353 3176  ignr......PKCS1v
+00000430: 3135 7203 0000 00da 0653 4841 3235 3672  15r......SHA256r
+00000440: 1700 0000 2904 da0b 7072 6976 6174 655f  ....)...private_
+00000450: 6b65 79da 076d 6573 7361 6765 da03 6b65  key..message..ke
+00000460: 79da 0165 7218 0000 0072 1800 0000 7219  y..er....r....r.
+00000470: 0000 00da 0c73 6967 6e5f 6d65 7373 6167  .....sign_messag
+00000480: 651a 0000 0073 2400 0000 0201 1201 1401  e....s$.........
+00000490: 0e01 0a01 0a01 0401 0880 02fd 0405 0401  ................
+000004a0: 0801 0601 0601 02fd 02ff 0606 02fa 7227  ..............r'
+000004b0: 0000 0063 0300 0000 0000 0000 0000 0000  ...c............
+000004c0: 0400 0000 0800 0000 4300 0000 7368 0000  ........C...sh..
+000004d0: 0074 007c 00a0 0164 01a1 0183 017d 0374  .t.|...d.....}.t
+000004e0: 027c 0374 036a 0483 0273 0f4a 0082 017a  .|.t.j...s.J...z
+000004f0: 157c 03a0 0574 06a0 077c 02a1 017c 01a0  .|...t...|...|..
+00000500: 0164 01a1 0174 08a0 09a1 0074 0aa0 0ba1  .d...t.....t....
+00000510: 00a1 0401 0057 0064 0453 0004 0074 0c79  .....W.d.S...t.y
+00000520: 3301 0001 0001 0074 0da0 0e64 02a1 0101  3......t...d....
+00000530: 0059 0064 0353 0077 0029 054e 720e 0000  .Y.d.S.w.).Nr...
+00000540: 007a 1169 6e76 616c 6964 2073 6967 6e61  .z.invalid signa
+00000550: 7475 7265 4654 290f 7209 0000 0072 1100  tureFT).r....r..
+00000560: 0000 720f 0000 0072 0700 0000 da0c 5253  ..r....r......RS
+00000570: 4150 7562 6c69 634b 6579 da06 7665 7269  APublicKey..veri
+00000580: 6679 7212 0000 00da 1273 7461 6e64 6172  fyr......standar
+00000590: 645f 6236 3464 6563 6f64 6572 0600 0000  d_b64decoder....
+000005a0: 7221 0000 0072 0300 0000 7222 0000 0072  r!...r....r"...r
+000005b0: 0200 0000 721e 0000 00da 0777 6172 6e69  ....r......warni
+000005c0: 6e67 2904 da0a 7075 626c 6963 5f6b 6579  ng)...public_key
+000005d0: 7224 0000 00da 0973 6967 6e61 7475 7265  r$.....signature
+000005e0: 5a11 7075 626c 6963 5f6b 6579 5f6c 6f61  Z.public_key_loa
+000005f0: 6465 6472 1800 0000 7218 0000 0072 1900  dedr....r....r..
+00000600: 0000 da10 7665 7269 6679 5f73 6967 6e61  ....verify_signa
+00000610: 7475 7265 2c00 0000 731c 0000 000e 0110  ture,...s.......
+00000620: 0202 0204 0108 0108 0106 0106 0106 fc04  ................
+00000630: 0a0c fc0a 0106 0102 fe72 2e00 0000 722c  .........r....r,
+00000640: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
+00000650: 0400 0000 0400 0000 4300 0000 7336 0000  ........C...s6..
+00000660: 007c 006a 0074 016a 026a 0374 016a 046a  .|.j.t.j.j.t.j.j
+00000670: 0364 018d 027d 0174 05a0 0664 027c 01a1  .d...}.t...d.|..
+00000680: 027d 0274 07a0 087c 0264 03a1 027d 0364  .}.t...|.d...}.d
+00000690: 047c 0317 0053 0029 054e 2902 da08 656e  .|...S.).N)...en
+000006a0: 636f 6469 6e67 da06 666f 726d 6174 fa0b  coding..format..
+000006b0: 6564 3235 3531 392d 7075 62da 0962 6173  ed25519-pub..bas
+000006c0: 6535 3862 7463 fa08 6469 643a 6b65 793a  e58btc..did:key:
+000006d0: 2909 da0c 7075 626c 6963 5f62 7974 6573  )...public_bytes
+000006e0: 7204 0000 00da 0845 6e63 6f64 696e 67da  r......Encoding.
+000006f0: 0352 6177 da0c 5075 626c 6963 466f 726d  .Raw..PublicForm
+00000700: 6174 720b 0000 00da 0477 7261 7072 0a00  atr......wrapr..
+00000710: 0000 7211 0000 0029 0472 2c00 0000 7234  ..r....).r,...r4
+00000720: 0000 00da 0777 7261 7070 6564 da07 656e  .....wrapped..en
+00000730: 636f 6465 6472 1800 0000 7218 0000 0072  codedr....r....r
+00000740: 1900 0000 da15 7075 626c 6963 5f6b 6579  ......public_key
+00000750: 5f74 6f5f 6469 645f 6b65 793f 0000 0073  _to_did_key?...s
+00000760: 0e00 0000 0401 0601 0601 06fe 0c05 0c01  ................
+00000770: 0802 723b 0000 00da 0364 6964 6301 0000  ..r;.....didc...
+00000780: 0000 0000 0000 0000 0004 0000 0005 0000  ................
+00000790: 0043 0000 0073 4800 0000 7c00 a000 6401  .C...sH...|...d.
+000007a0: a101 7307 4a00 8201 7401 a002 7c00 6402  ..s.J...t...|.d.
+000007b0: 6400 8502 1900 a101 7d01 7403 a004 7c01  d.......}.t...|.
+000007c0: a101 5c02 7d02 7d03 7c02 6a05 6403 6b02  ..\.}.}.|.j.d.k.
+000007d0: 731e 4a00 8201 7406 6a07 a008 7c03 a101  s.J...t.j...|...
+000007e0: 5300 2904 4e72 3300 0000 e908 0000 0072  S.).Nr3........r
+000007f0: 3100 0000 2909 da0a 7374 6172 7473 7769  1...)...startswi
+00000800: 7468 720a 0000 0072 1700 0000 720b 0000  thr....r....r...
+00000810: 00da 0675 6e77 7261 70da 046e 616d 6572  ...unwrap..namer
+00000820: 0500 0000 da10 4564 3235 3531 3950 7562  ......Ed25519Pub
+00000830: 6c69 634b 6579 da11 6672 6f6d 5f70 7562  licKey..from_pub
+00000840: 6c69 635f 6279 7465 7329 0472 3c00 0000  lic_bytes).r<...
+00000850: da07 6465 636f 6465 64da 0563 6f64 6563  ..decoded..codec
+00000860: da09 6b65 795f 6279 7465 7372 1800 0000  ..key_bytesr....
+00000870: 7218 0000 0072 1900 0000 da15 6469 645f  r....r......did_
+00000880: 6b65 795f 746f 5f70 7562 6c69 635f 6b65  key_to_public_ke
+00000890: 794b 0000 0073 0a00 0000 0e01 1201 0e01  yK...s..........
+000008a0: 0e01 0c02 7246 0000 00da 0f70 7269 7661  ....rF.....priva
+000008b0: 7465 5f6b 6579 5f73 7472 6301 0000 0000  te_key_strc.....
+000008c0: 0000 0000 0000 0004 0000 0003 0000 0043  ...............C
+000008d0: 0000 0073 3200 0000 7400 a001 7c00 a101  ...s2...t...|...
+000008e0: 7d01 7402 a003 7c01 a101 5c02 7d02 7d03  }.t...|...\.}.}.
+000008f0: 7c02 6a04 6401 6b02 7313 4a00 8201 7405  |.j.d.k.s.J...t.
+00000900: 6a06 a007 7c03 a101 5300 2902 4e7a 0c65  j...|...S.).Nz.e
+00000910: 6432 3535 3139 2d70 7269 7629 0872 0a00  d25519-priv).r..
+00000920: 0000 7217 0000 0072 0b00 0000 723f 0000  ..r....r....r?..
+00000930: 0072 4000 0000 7205 0000 00da 1145 6432  .r@...r......Ed2
+00000940: 3535 3139 5072 6976 6174 654b 6579 da12  5519PrivateKey..
+00000950: 6672 6f6d 5f70 7269 7661 7465 5f62 7974  from_private_byt
+00000960: 6573 2904 7247 0000 0072 4300 0000 7244  es).rG...rC...rD
+00000970: 0000 0072 4500 0000 7218 0000 0072 1800  ...rE...r....r..
+00000980: 0000 7219 0000 00da 1670 7269 7661 7465  ..r......private
+00000990: 5f6b 6579 5f74 6f5f 6564 3235 3531 3954  _key_to_ed25519T
+000009a0: 0000 0073 0800 0000 0a01 0e01 0e01 0c02  ...s............
+000009b0: 724a 0000 0029 1f72 1200 0000 7214 0000  rJ...).r....r...
+000009c0: 00da 076c 6f67 6769 6e67 da17 6372 7970  ...logging..cryp
+000009d0: 746f 6772 6170 6879 2e65 7863 6570 7469  tography.excepti
+000009e0: 6f6e 7372 0200 0000 da1e 6372 7970 746f  onsr......crypto
+000009f0: 6772 6170 6879 2e68 617a 6d61 742e 7072  graphy.hazmat.pr
+00000a00: 696d 6974 6976 6573 7203 0000 0072 0400  imitivesr....r..
+00000a10: 0000 da29 6372 7970 746f 6772 6170 6879  ...)cryptography
+00000a20: 2e68 617a 6d61 742e 7072 696d 6974 6976  .hazmat.primitiv
+00000a30: 6573 2e61 7379 6d6d 6574 7269 6372 0500  es.asymmetricr..
+00000a40: 0000 7206 0000 0072 0700 0000 5a2c 6372  ..r....r....Z,cr
 00000a50: 7970 746f 6772 6170 6879 2e68 617a 6d61  yptography.hazma
-00000a60: 742e 7072 696d 6974 6976 6573 2e61 7379  t.primitives.asy
-00000a70: 6d6d 6574 7269 6372 0500 0000 7206 0000  mmetricr....r...
-00000a80: 0072 0700 0000 5a2c 6372 7970 746f 6772  .r....Z,cryptogr
-00000a90: 6170 6879 2e68 617a 6d61 742e 7072 696d  aphy.hazmat.prim
-00000aa0: 6974 6976 6573 2e73 6572 6961 6c69 7a61  itives.serializa
-00000ab0: 7469 6f6e 7208 0000 0072 0900 0000 da0c  tionr....r......
-00000ac0: 6d75 6c74 6966 6f72 6d61 7473 720a 0000  multiformatsr...
-00000ad0: 0072 0b00 0000 da09 6765 744c 6f67 6765  .r......getLogge
-00000ae0: 72da 085f 5f6e 616d 655f 5f72 2100 0000  r..__name__r!...
-00000af0: 7210 0000 00da 0562 7974 6573 721a 0000  r......bytesr...
-00000b00: 0072 2a00 0000 7231 0000 0072 4400 0000  .r*...r1...rD...
-00000b10: 723e 0000 0072 4900 0000 724b 0000 0072  r>...rI...rK...r
-00000b20: 4d00 0000 7218 0000 0072 1800 0000 7218  M...r....r....r.
-00000b30: 0000 0072 1900 0000 da08 3c6d 6f64 756c  ...r......<modul
-00000b40: 653e 0100 0000 731e 0000 0008 0008 0108  e>....s.........
-00000b50: 010c 0210 0114 0110 0110 040a 0216 0308  ................
-00000b60: 0908 1314 1414 0c18 09                   .........
+00000a60: 742e 7072 696d 6974 6976 6573 2e73 6572  t.primitives.ser
+00000a70: 6961 6c69 7a61 7469 6f6e 7208 0000 0072  ializationr....r
+00000a80: 0900 0000 da0c 6d75 6c74 6966 6f72 6d61  ......multiforma
+00000a90: 7473 720a 0000 0072 0b00 0000 da09 6765  tsr....r......ge
+00000aa0: 744c 6f67 6765 72da 085f 5f6e 616d 655f  tLogger..__name_
+00000ab0: 5f72 1e00 0000 7210 0000 00da 0562 7974  _r....r......byt
+00000ac0: 6573 721a 0000 0072 2700 0000 722e 0000  esr....r'...r...
+00000ad0: 0072 4100 0000 723b 0000 0072 4600 0000  .rA...r;...rF...
+00000ae0: 7248 0000 0072 4a00 0000 7218 0000 0072  rH...rJ...r....r
+00000af0: 1800 0000 7218 0000 0072 1900 0000 da08  ....r....r......
+00000b00: 3c6d 6f64 756c 653e 0100 0000 731e 0000  <module>....s...
+00000b10: 0008 0008 0108 010c 0210 0114 0110 0110  ................
+00000b20: 040a 0216 0308 0908 1214 1314 0c18 09    ...............
```

### Comparing `bovine-0.1.0/bovine/crypto/__pycache__/http_signature.cpython-310.pyc` & `bovine-0.1.1/bovine/crypto/__pycache__/http_signature.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 13 15:55:57 2023 UTC, .py size: 2112 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0d26 3864 4008 0000  o........&8d@...
+00000000: 6f0d 0d0a 0000 0000 a4ea 3a64 4008 0000  o.........:d@...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 6800 0000 6400  .....@...sh...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c03 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 6d07 5a07 0100 6405  d.l.m.Z.m.Z...d.
 00000060: 6406 6c08 6d09 5a09 6d0a 5a0a 6d0b 5a0b  d.l.m.Z.m.Z.m.Z.
 00000070: 0100 6500 a00c 650d a101 5a0e 6407 6408  ..e...e...Z.d.d.
@@ -20,163 +20,163 @@
 00000130: 0000 7400 8300 a001 6401 7c01 9b00 6402  ..t.....d.|...d.
 00000140: 7c02 9b00 9d03 a102 a001 6403 7c00 a102  |.........d.|...
 00000150: 5300 2904 4e7a 1028 7265 7175 6573 742d  S.).Nz.(request-
 00000160: 7461 7267 6574 29da 0120 da04 686f 7374  target).. ..host
 00000170: 2902 da0d 4874 7470 5369 676e 6174 7572  )...HttpSignatur
 00000180: 65da 0a77 6974 685f 6669 656c 6429 0372  e..with_field).r
 00000190: 0b00 0000 da06 6d65 7468 6f64 da06 7461  ......method..ta
-000001a0: 7267 6574 a900 7210 0000 00fa 502f 776f  rget..r.....P/wo
+000001a0: 7267 6574 a900 7210 0000 00fa 512f 776f  rget..r.....Q/wo
 000001b0: 6f64 7065 636b 6572 2f73 7263 2f63 6f64  odpecker/src/cod
-000001c0: 6562 6572 672e 6f72 672f 6865 6c67 652f  eberg.org/helge/
-000001d0: 626f 7669 6e65 2f62 6f76 696e 652f 626f  bovine/bovine/bo
-000001e0: 7669 6e65 2f63 7279 7074 6f2f 6874 7470  vine/crypto/http
-000001f0: 5f73 6967 6e61 7475 7265 2e70 79da 0f62  _signature.py..b
-00000200: 7569 6c64 5f73 6967 6e61 7475 7265 0c00  uild_signature..
-00000210: 0000 7308 0000 0004 0212 0108 0102 fd72  ..s............r
-00000220: 1200 0000 6300 0000 0000 0000 0000 0000  ....c...........
-00000230: 0000 0000 0002 0000 0040 0000 0073 4400  .........@...sD.
-00000240: 0000 6500 5a01 6400 5a02 6401 6402 8400  ..e.Z.d.Z.d.d...
-00000250: 5a03 6403 6404 8400 5a04 6405 6406 8400  Z.d.d...Z.d.d...
-00000260: 5a05 6407 6408 8400 5a06 6409 640a 8400  Z.d.d...Z.d.d...
-00000270: 5a07 640b 640c 8400 5a08 640d 640e 8400  Z.d.d...Z.d.d...
-00000280: 5a09 640f 5300 2910 720c 0000 0063 0100  Z.d.S.).r....c..
-00000290: 0000 0000 0000 0000 0000 0100 0000 0200  ................
-000002a0: 0000 4300 0000 730a 0000 0067 007c 005f  ..C...s....g.|._
-000002b0: 0064 0053 00a9 014e 2901 da06 6669 656c  .d.S...N)...fiel
-000002c0: 6473 a901 da04 7365 6c66 7210 0000 0072  ds....selfr....r
-000002d0: 1000 0000 7211 0000 00da 085f 5f69 6e69  ....r......__ini
-000002e0: 745f 5f15 0000 0073 0200 0000 0a01 7a16  t__....s......z.
-000002f0: 4874 7470 5369 676e 6174 7572 652e 5f5f  HttpSignature.__
-00000300: 696e 6974 5f5f 6303 0000 0000 0000 0000  init__c.........
-00000310: 0000 0007 0000 0006 0000 0043 0000 0073  ...........C...s
-00000320: 5600 0000 7c00 a000 a100 7d03 7401 7c02  V...|.....}.t.|.
-00000330: 7c03 8302 7d04 6401 a002 6402 6403 8400  |...}.d...d.d...
-00000340: 7c00 6a03 4400 8301 a101 7d05 6404 7c01  |.j.D.....}.d.|.
-00000350: 9b00 6405 9d03 6406 6407 7c05 9b00 6405  ..d...d.d.|...d.
-00000360: 9d03 6408 7c04 9b00 6405 9d03 6704 7d06  ..d.|...d...g.}.
-00000370: 6409 a002 7c06 a101 5300 290a 4e72 0a00  d...|...S.).Nr..
-00000380: 0000 6301 0000 0000 0000 0000 0000 0003  ..c.............
-00000390: 0000 0003 0000 0073 0000 0073 1800 0000  .......s...s....
-000003a0: 8100 7c00 5d07 5c02 7d01 7d02 7c01 5600  ..|.].\.}.}.|.V.
-000003b0: 0100 7102 6400 5300 7213 0000 0072 1000  ..q.d.S.r....r..
-000003c0: 0000 2903 da02 2e30 da04 6e61 6d65 da01  ..)....0..name..
-000003d0: 5f72 1000 0000 7210 0000 0072 1100 0000  _r....r....r....
-000003e0: da09 3c67 656e 6578 7072 3e1c 0000 0073  ..<genexpr>....s
-000003f0: 0400 0000 0280 1600 7a30 4874 7470 5369  ........z0HttpSi
-00000400: 676e 6174 7572 652e 6275 696c 645f 7369  gnature.build_si
-00000410: 676e 6174 7572 652e 3c6c 6f63 616c 733e  gnature.<locals>
-00000420: 2e3c 6765 6e65 7870 723e 7a07 6b65 7949  .<genexpr>z.keyI
-00000430: 643d 22fa 0122 7a16 616c 676f 7269 7468  d=".."z.algorith
-00000440: 6d3d 2272 7361 2d73 6861 3235 3622 7a09  m="rsa-sha256"z.
-00000450: 6865 6164 6572 733d 227a 0b73 6967 6e61  headers="z.signa
-00000460: 7475 7265 3d22 fa01 2c29 04da 0d62 7569  ture="..,)...bui
-00000470: 6c64 5f6d 6573 7361 6765 7208 0000 00da  ld_messager.....
-00000480: 046a 6f69 6e72 1400 0000 2907 7216 0000  .joinr....).r...
-00000490: 00da 066b 6579 5f69 64da 0b70 7269 7661  ...key_id..priva
-000004a0: 7465 5f6b 6579 da07 6d65 7373 6167 655a  te_key..messageZ
-000004b0: 1073 6967 6e61 7475 7265 5f73 7472 696e  .signature_strin
-000004c0: 67da 0768 6561 6465 7273 5a0f 7369 676e  g..headersZ.sign
-000004d0: 6174 7572 655f 7061 7274 7372 1000 0000  ature_partsr....
-000004e0: 7210 0000 0072 1100 0000 7212 0000 0018  r....r....r.....
-000004f0: 0000 0073 1200 0000 0801 0a02 1601 0a03  ...s............
-00000500: 0201 0a01 0a01 04fc 0a07 7a1d 4874 7470  ..........z.Http
-00000510: 5369 676e 6174 7572 652e 6275 696c 645f  Signature.build_
-00000520: 7369 676e 6174 7572 6563 0200 0000 0000  signaturec......
-00000530: 0000 0000 0000 0500 0000 0700 0000 4300  ..............C.
-00000540: 0000 7340 0000 0074 00a0 0174 02a0 037c  ..s@...t...t...|
-00000550: 01a1 01a1 0164 0119 007d 0274 046a 05a0  .....d...}.t.j..
-00000560: 067c 02a1 017d 037c 00a0 07a1 007d 0474  .|...}.|.....}.t
-00000570: 02a0 087c 03a0 097c 04a0 0864 02a1 01a1  ...|...|...d....
-00000580: 0164 03a1 0253 0029 044e 7206 0000 00fa  .d...S.).Nr.....
-00000590: 0575 7466 2d38 da09 6261 7365 3538 6274  .utf-8..base58bt
-000005a0: 6329 0a72 0500 0000 da06 756e 7772 6170  c).r......unwrap
-000005b0: 7204 0000 00da 0664 6563 6f64 6572 0300  r......decoder..
-000005c0: 0000 da11 4564 3235 3531 3950 7269 7661  ....Ed25519Priva
-000005d0: 7465 4b65 79da 1266 726f 6d5f 7072 6976  teKey..from_priv
-000005e0: 6174 655f 6279 7465 7372 1e00 0000 da06  ate_bytesr......
-000005f0: 656e 636f 6465 da04 7369 676e 2905 7216  encode..sign).r.
-00000600: 0000 005a 0f70 7269 7661 7465 5f65 6e63  ...Z.private_enc
-00000610: 6f64 6564 da0d 7072 6976 6174 655f 6279  oded..private_by
-00000620: 7465 7372 2100 0000 7222 0000 0072 1000  tesr!...r"...r..
-00000630: 0000 7210 0000 0072 1100 0000 da0c 6564  ..r....r......ed
-00000640: 3235 3531 395f 7369 676e 2700 0000 7308  25519_sign'...s.
-00000650: 0000 0014 010c 0108 0218 027a 1a48 7474  ...........z.Htt
-00000660: 7053 6967 6e61 7475 7265 2e65 6432 3535  pSignature.ed255
-00000670: 3139 5f73 6967 6e63 0300 0000 0000 0000  19_signc........
-00000680: 0000 0000 0500 0000 0800 0000 4300 0000  ............C...
-00000690: 7348 0000 0074 007c 0183 017d 0374 01a0  sH...t.|...}.t..
-000006a0: 027c 02a1 017d 027c 00a0 03a1 00a0 0464  .|...}.|.......d
-000006b0: 01a1 017d 047a 097c 03a0 057c 027c 04a1  ...}.z.|...|.|..
-000006c0: 0201 0057 0064 0353 0004 0074 0679 2301  ...W.d.S...t.y#.
-000006d0: 0001 0001 0059 0064 0253 0077 0029 044e  .....Y.d.S.w.).N
-000006e0: 7224 0000 0046 5429 0772 0700 0000 7204  r$...FT).r....r.
-000006f0: 0000 0072 2700 0000 721e 0000 0072 2a00  ...r'...r....r*.
-00000700: 0000 da06 7665 7269 6679 7202 0000 0029  ....verifyr....)
-00000710: 0572 1600 0000 da06 6469 646b 6579 da09  .r......didkey..
-00000720: 7369 676e 6174 7572 65da 0a70 7562 6c69  signature..publi
-00000730: 635f 6b65 7972 2200 0000 7210 0000 0072  c_keyr"...r....r
-00000740: 1000 0000 7211 0000 00da 0e65 6432 3535  ....r......ed255
-00000750: 3139 5f76 6572 6966 792f 0000 0073 1200  19_verify/...s..
-00000760: 0000 0801 0a02 0e02 0202 0e01 0404 0cfd  ................
-00000770: 0601 02ff 7a1c 4874 7470 5369 676e 6174  ....z.HttpSignat
-00000780: 7572 652e 6564 3235 3531 395f 7665 7269  ure.ed25519_veri
-00000790: 6679 6303 0000 0000 0000 0000 0000 0004  fyc.............
-000007a0: 0000 0004 0000 0043 0000 0073 1400 0000  .......C...s....
-000007b0: 7c00 a000 a100 7d03 7401 7c01 7c03 7c02  |.....}.t.|.|.|.
-000007c0: 8303 5300 7213 0000 0029 0272 1e00 0000  ..S.r....).r....
-000007d0: 7209 0000 0029 0472 1600 0000 7231 0000  r....).r....r1..
-000007e0: 0072 3000 0000 7222 0000 0072 1000 0000  .r0...r"...r....
-000007f0: 7210 0000 0072 1100 0000 722e 0000 003d  r....r....r....=
-00000800: 0000 0073 0400 0000 0801 0c01 7a14 4874  ...s........z.Ht
-00000810: 7470 5369 676e 6174 7572 652e 7665 7269  tpSignature.veri
-00000820: 6679 6301 0000 0000 0000 0000 0000 0001  fyc.............
-00000830: 0000 0004 0000 0043 0000 0073 1600 0000  .......C...s....
-00000840: 6401 a000 6402 6403 8400 7c00 6a01 4400  d...d.d...|.j.D.
-00000850: 8301 a101 5300 2904 4eda 010a 6301 0000  ....S.).N...c...
-00000860: 0000 0000 0000 0000 0003 0000 0004 0000  ................
-00000870: 0073 0000 0073 2200 0000 8100 7c00 5d0c  .s...s".....|.].
-00000880: 5c02 7d01 7d02 7c01 9b00 6400 7c02 9b00  \.}.}.|...d.|...
-00000890: 9d03 5600 0100 7102 6401 5300 2902 7a02  ..V...q.d.S.).z.
-000008a0: 3a20 4e72 1000 0000 2903 7218 0000 0072  : Nr....).r....r
-000008b0: 1900 0000 da05 7661 6c75 6572 1000 0000  ......valuer....
-000008c0: 7210 0000 0072 1100 0000 721b 0000 0042  r....r....r....B
-000008d0: 0000 0073 0400 0000 0280 2000 7a2e 4874  ...s...... .z.Ht
-000008e0: 7470 5369 676e 6174 7572 652e 6275 696c  tpSignature.buil
-000008f0: 645f 6d65 7373 6167 652e 3c6c 6f63 616c  d_message.<local
-00000900: 733e 2e3c 6765 6e65 7870 723e 2902 721f  s>.<genexpr>).r.
-00000910: 0000 0072 1400 0000 7215 0000 0072 1000  ...r....r....r..
-00000920: 0000 7210 0000 0072 1100 0000 721e 0000  ..r....r....r...
-00000930: 0041 0000 0073 0200 0000 1601 7a1b 4874  .A...s......z.Ht
-00000940: 7470 5369 676e 6174 7572 652e 6275 696c  tpSignature.buil
-00000950: 645f 6d65 7373 6167 6563 0300 0000 0000  d_messagec......
-00000960: 0000 0000 0000 0300 0000 0400 0000 4300  ..............C.
-00000970: 0000 7314 0000 007c 006a 00a0 017c 017c  ..s....|.j...|.|
-00000980: 0266 02a1 0101 007c 0053 0072 1300 0000  .f.....|.S.r....
-00000990: 2902 7214 0000 00da 0661 7070 656e 6429  ).r......append)
-000009a0: 0372 1600 0000 da0a 6669 656c 645f 6e61  .r......field_na
-000009b0: 6d65 5a0b 6669 656c 645f 7661 6c75 6572  meZ.field_valuer
-000009c0: 1000 0000 7210 0000 0072 1100 0000 720d  ....r....r....r.
-000009d0: 0000 0044 0000 0073 0400 0000 1001 0401  ...D...s........
-000009e0: 7a18 4874 7470 5369 676e 6174 7572 652e  z.HttpSignature.
-000009f0: 7769 7468 5f66 6965 6c64 4e29 0ada 085f  with_fieldN)..._
-00000a00: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
-00000a10: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
-00000a20: 5f72 1700 0000 7212 0000 0072 2d00 0000  _r....r....r-...
-00000a30: 7232 0000 0072 2e00 0000 721e 0000 0072  r2...r....r....r
-00000a40: 0d00 0000 7210 0000 0072 1000 0000 7210  ....r....r....r.
-00000a50: 0000 0072 1100 0000 720c 0000 0014 0000  ...r....r.......
-00000a60: 0073 1000 0000 0800 0801 0803 080f 0808  .s..............
-00000a70: 080e 0804 0c03 720c 0000 0029 11da 076c  ......r....)...l
-00000a80: 6f67 6769 6e67 da17 6372 7970 746f 6772  ogging..cryptogr
-00000a90: 6170 6879 2e65 7863 6570 7469 6f6e 7372  aphy.exceptionsr
-00000aa0: 0200 0000 da29 6372 7970 746f 6772 6170  .....)cryptograp
-00000ab0: 6879 2e68 617a 6d61 742e 7072 696d 6974  hy.hazmat.primit
-00000ac0: 6976 6573 2e61 7379 6d6d 6574 7269 6372  ives.asymmetricr
-00000ad0: 0300 0000 da0c 6d75 6c74 6966 6f72 6d61  ......multiforma
-00000ae0: 7473 7204 0000 0072 0500 0000 da06 6865  tsr....r......he
-00000af0: 6c70 6572 7207 0000 0072 0800 0000 7209  lperr....r....r.
-00000b00: 0000 00da 0967 6574 4c6f 6767 6572 7237  .....getLoggerr7
-00000b10: 0000 00da 066c 6f67 6765 7272 1200 0000  .....loggerr....
-00000b20: 720c 0000 0072 1000 0000 7210 0000 0072  r....r....r....r
-00000b30: 1000 0000 7211 0000 00da 083c 6d6f 6475  ....r......<modu
-00000b40: 6c65 3e01 0000 0073 1000 0000 0800 0c02  le>....s........
-00000b50: 0c01 1001 1402 0a02 0803 1208            ............
+000001c0: 6562 6572 672e 6f72 672f 626f 7669 6e65  eberg.org/bovine
+000001d0: 2f62 6f76 696e 652f 626f 7669 6e65 2f62  /bovine/bovine/b
+000001e0: 6f76 696e 652f 6372 7970 746f 2f68 7474  ovine/crypto/htt
+000001f0: 705f 7369 676e 6174 7572 652e 7079 da0f  p_signature.py..
+00000200: 6275 696c 645f 7369 676e 6174 7572 650c  build_signature.
+00000210: 0000 0073 0800 0000 0402 1201 0801 02fd  ...s............
+00000220: 7212 0000 0063 0000 0000 0000 0000 0000  r....c..........
+00000230: 0000 0000 0000 0200 0000 4000 0000 7344  ..........@...sD
+00000240: 0000 0065 005a 0164 005a 0264 0164 0284  ...e.Z.d.Z.d.d..
+00000250: 005a 0364 0364 0484 005a 0464 0564 0684  .Z.d.d...Z.d.d..
+00000260: 005a 0564 0764 0884 005a 0664 0964 0a84  .Z.d.d...Z.d.d..
+00000270: 005a 0764 0b64 0c84 005a 0864 0d64 0e84  .Z.d.d...Z.d.d..
+00000280: 005a 0964 0f53 0029 1072 0c00 0000 6301  .Z.d.S.).r....c.
+00000290: 0000 0000 0000 0000 0000 0001 0000 0002  ................
+000002a0: 0000 0043 0000 0073 0a00 0000 6700 7c00  ...C...s....g.|.
+000002b0: 5f00 6400 5300 a901 4e29 01da 0666 6965  _.d.S...N)...fie
+000002c0: 6c64 73a9 01da 0473 656c 6672 1000 0000  lds....selfr....
+000002d0: 7210 0000 0072 1100 0000 da08 5f5f 696e  r....r......__in
+000002e0: 6974 5f5f 1500 0000 7302 0000 000a 017a  it__....s......z
+000002f0: 1648 7474 7053 6967 6e61 7475 7265 2e5f  .HttpSignature._
+00000300: 5f69 6e69 745f 5f63 0300 0000 0000 0000  _init__c........
+00000310: 0000 0000 0700 0000 0600 0000 4300 0000  ............C...
+00000320: 7356 0000 007c 00a0 00a1 007d 0374 017c  sV...|.....}.t.|
+00000330: 027c 0383 027d 0464 01a0 0264 0264 0384  .|...}.d...d.d..
+00000340: 007c 006a 0344 0083 01a1 017d 0564 047c  .|.j.D.....}.d.|
+00000350: 019b 0064 059d 0364 0664 077c 059b 0064  ...d...d.d.|...d
+00000360: 059d 0364 087c 049b 0064 059d 0367 047d  ...d.|...d...g.}
+00000370: 0664 09a0 027c 06a1 0153 0029 0a4e 720a  .d...|...S.).Nr.
+00000380: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
+00000390: 0300 0000 0300 0000 7300 0000 7318 0000  ........s...s...
+000003a0: 0081 007c 005d 075c 027d 017d 027c 0156  ...|.].\.}.}.|.V
+000003b0: 0001 0071 0264 0053 0072 1300 0000 7210  ...q.d.S.r....r.
+000003c0: 0000 0029 03da 022e 30da 046e 616d 65da  ...)....0..name.
+000003d0: 015f 7210 0000 0072 1000 0000 7211 0000  ._r....r....r...
+000003e0: 00da 093c 6765 6e65 7870 723e 1c00 0000  ...<genexpr>....
+000003f0: 7304 0000 0002 8016 007a 3048 7474 7053  s........z0HttpS
+00000400: 6967 6e61 7475 7265 2e62 7569 6c64 5f73  ignature.build_s
+00000410: 6967 6e61 7475 7265 2e3c 6c6f 6361 6c73  ignature.<locals
+00000420: 3e2e 3c67 656e 6578 7072 3e7a 076b 6579  >.<genexpr>z.key
+00000430: 4964 3d22 fa01 227a 1661 6c67 6f72 6974  Id=".."z.algorit
+00000440: 686d 3d22 7273 612d 7368 6132 3536 227a  hm="rsa-sha256"z
+00000450: 0968 6561 6465 7273 3d22 7a0b 7369 676e  .headers="z.sign
+00000460: 6174 7572 653d 22fa 012c 2904 da0d 6275  ature="..,)...bu
+00000470: 696c 645f 6d65 7373 6167 6572 0800 0000  ild_messager....
+00000480: da04 6a6f 696e 7214 0000 0029 0772 1600  ..joinr....).r..
+00000490: 0000 da06 6b65 795f 6964 da0b 7072 6976  ....key_id..priv
+000004a0: 6174 655f 6b65 79da 076d 6573 7361 6765  ate_key..message
+000004b0: 5a10 7369 676e 6174 7572 655f 7374 7269  Z.signature_stri
+000004c0: 6e67 da07 6865 6164 6572 735a 0f73 6967  ng..headersZ.sig
+000004d0: 6e61 7475 7265 5f70 6172 7473 7210 0000  nature_partsr...
+000004e0: 0072 1000 0000 7211 0000 0072 1200 0000  .r....r....r....
+000004f0: 1800 0000 7312 0000 0008 010a 0216 010a  ....s...........
+00000500: 0302 010a 010a 0104 fc0a 077a 1d48 7474  ...........z.Htt
+00000510: 7053 6967 6e61 7475 7265 2e62 7569 6c64  pSignature.build
+00000520: 5f73 6967 6e61 7475 7265 6302 0000 0000  _signaturec.....
+00000530: 0000 0000 0000 0005 0000 0007 0000 0043  ...............C
+00000540: 0000 0073 4000 0000 7400 a001 7402 a003  ...s@...t...t...
+00000550: 7c01 a101 a101 6401 1900 7d02 7404 6a05  |.....d...}.t.j.
+00000560: a006 7c02 a101 7d03 7c00 a007 a100 7d04  ..|...}.|.....}.
+00000570: 7402 a008 7c03 a009 7c04 a008 6402 a101  t...|...|...d...
+00000580: a101 6403 a102 5300 2904 4e72 0600 0000  ..d...S.).Nr....
+00000590: fa05 7574 662d 38da 0962 6173 6535 3862  ..utf-8..base58b
+000005a0: 7463 290a 7205 0000 00da 0675 6e77 7261  tc).r......unwra
+000005b0: 7072 0400 0000 da06 6465 636f 6465 7203  pr......decoder.
+000005c0: 0000 00da 1145 6432 3535 3139 5072 6976  .....Ed25519Priv
+000005d0: 6174 654b 6579 da12 6672 6f6d 5f70 7269  ateKey..from_pri
+000005e0: 7661 7465 5f62 7974 6573 721e 0000 00da  vate_bytesr.....
+000005f0: 0665 6e63 6f64 65da 0473 6967 6e29 0572  .encode..sign).r
+00000600: 1600 0000 5a0f 7072 6976 6174 655f 656e  ....Z.private_en
+00000610: 636f 6465 64da 0d70 7269 7661 7465 5f62  coded..private_b
+00000620: 7974 6573 7221 0000 0072 2200 0000 7210  ytesr!...r"...r.
+00000630: 0000 0072 1000 0000 7211 0000 00da 0c65  ...r....r......e
+00000640: 6432 3535 3139 5f73 6967 6e27 0000 0073  d25519_sign'...s
+00000650: 0800 0000 1401 0c01 0802 1802 7a1a 4874  ............z.Ht
+00000660: 7470 5369 676e 6174 7572 652e 6564 3235  tpSignature.ed25
+00000670: 3531 395f 7369 676e 6303 0000 0000 0000  519_signc.......
+00000680: 0000 0000 0005 0000 0008 0000 0043 0000  .............C..
+00000690: 0073 4800 0000 7400 7c01 8301 7d03 7401  .sH...t.|...}.t.
+000006a0: a002 7c02 a101 7d02 7c00 a003 a100 a004  ..|...}.|.......
+000006b0: 6401 a101 7d04 7a09 7c03 a005 7c02 7c04  d...}.z.|...|.|.
+000006c0: a102 0100 5700 6403 5300 0400 7406 7923  ....W.d.S...t.y#
+000006d0: 0100 0100 0100 5900 6402 5300 7700 2904  ......Y.d.S.w.).
+000006e0: 4e72 2400 0000 4654 2907 7207 0000 0072  Nr$...FT).r....r
+000006f0: 0400 0000 7227 0000 0072 1e00 0000 722a  ....r'...r....r*
+00000700: 0000 00da 0676 6572 6966 7972 0200 0000  .....verifyr....
+00000710: 2905 7216 0000 00da 0664 6964 6b65 79da  ).r......didkey.
+00000720: 0973 6967 6e61 7475 7265 da0a 7075 626c  .signature..publ
+00000730: 6963 5f6b 6579 7222 0000 0072 1000 0000  ic_keyr"...r....
+00000740: 7210 0000 0072 1100 0000 da0e 6564 3235  r....r......ed25
+00000750: 3531 395f 7665 7269 6679 2f00 0000 7312  519_verify/...s.
+00000760: 0000 0008 010a 020e 0202 020e 0104 040c  ................
+00000770: fd06 0102 ff7a 1c48 7474 7053 6967 6e61  .....z.HttpSigna
+00000780: 7475 7265 2e65 6432 3535 3139 5f76 6572  ture.ed25519_ver
+00000790: 6966 7963 0300 0000 0000 0000 0000 0000  ifyc............
+000007a0: 0400 0000 0400 0000 4300 0000 7314 0000  ........C...s...
+000007b0: 007c 00a0 00a1 007d 0374 017c 017c 037c  .|.....}.t.|.|.|
+000007c0: 0283 0353 0072 1300 0000 2902 721e 0000  ...S.r....).r...
+000007d0: 0072 0900 0000 2904 7216 0000 0072 3100  .r....).r....r1.
+000007e0: 0000 7230 0000 0072 2200 0000 7210 0000  ..r0...r"...r...
+000007f0: 0072 1000 0000 7211 0000 0072 2e00 0000  .r....r....r....
+00000800: 3d00 0000 7304 0000 0008 010c 017a 1448  =...s........z.H
+00000810: 7474 7053 6967 6e61 7475 7265 2e76 6572  ttpSignature.ver
+00000820: 6966 7963 0100 0000 0000 0000 0000 0000  ifyc............
+00000830: 0100 0000 0400 0000 4300 0000 7316 0000  ........C...s...
+00000840: 0064 01a0 0064 0264 0384 007c 006a 0144  .d...d.d...|.j.D
+00000850: 0083 01a1 0153 0029 044e da01 0a63 0100  .....S.).N...c..
+00000860: 0000 0000 0000 0000 0000 0300 0000 0400  ................
+00000870: 0000 7300 0000 7322 0000 0081 007c 005d  ..s...s".....|.]
+00000880: 0c5c 027d 017d 027c 019b 0064 007c 029b  .\.}.}.|...d.|..
+00000890: 009d 0356 0001 0071 0264 0153 0029 027a  ...V...q.d.S.).z
+000008a0: 023a 204e 7210 0000 0029 0372 1800 0000  .: Nr....).r....
+000008b0: 7219 0000 00da 0576 616c 7565 7210 0000  r......valuer...
+000008c0: 0072 1000 0000 7211 0000 0072 1b00 0000  .r....r....r....
+000008d0: 4200 0000 7304 0000 0002 8020 007a 2e48  B...s...... .z.H
+000008e0: 7474 7053 6967 6e61 7475 7265 2e62 7569  ttpSignature.bui
+000008f0: 6c64 5f6d 6573 7361 6765 2e3c 6c6f 6361  ld_message.<loca
+00000900: 6c73 3e2e 3c67 656e 6578 7072 3e29 0272  ls>.<genexpr>).r
+00000910: 1f00 0000 7214 0000 0072 1500 0000 7210  ....r....r....r.
+00000920: 0000 0072 1000 0000 7211 0000 0072 1e00  ...r....r....r..
+00000930: 0000 4100 0000 7302 0000 0016 017a 1b48  ..A...s......z.H
+00000940: 7474 7053 6967 6e61 7475 7265 2e62 7569  ttpSignature.bui
+00000950: 6c64 5f6d 6573 7361 6765 6303 0000 0000  ld_messagec.....
+00000960: 0000 0000 0000 0003 0000 0004 0000 0043  ...............C
+00000970: 0000 0073 1400 0000 7c00 6a00 a001 7c01  ...s....|.j...|.
+00000980: 7c02 6602 a101 0100 7c00 5300 7213 0000  |.f.....|.S.r...
+00000990: 0029 0272 1400 0000 da06 6170 7065 6e64  .).r......append
+000009a0: 2903 7216 0000 00da 0a66 6965 6c64 5f6e  ).r......field_n
+000009b0: 616d 655a 0b66 6965 6c64 5f76 616c 7565  ameZ.field_value
+000009c0: 7210 0000 0072 1000 0000 7211 0000 0072  r....r....r....r
+000009d0: 0d00 0000 4400 0000 7304 0000 0010 0104  ....D...s.......
+000009e0: 017a 1848 7474 7053 6967 6e61 7475 7265  .z.HttpSignature
+000009f0: 2e77 6974 685f 6669 656c 644e 290a da08  .with_fieldN)...
+00000a00: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
+00000a10: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
+00000a20: 5f5f 7217 0000 0072 1200 0000 722d 0000  __r....r....r-..
+00000a30: 0072 3200 0000 722e 0000 0072 1e00 0000  .r2...r....r....
+00000a40: 720d 0000 0072 1000 0000 7210 0000 0072  r....r....r....r
+00000a50: 1000 0000 7211 0000 0072 0c00 0000 1400  ....r....r......
+00000a60: 0000 7310 0000 0008 0008 0108 0308 0f08  ..s.............
+00000a70: 0808 0e08 040c 0372 0c00 0000 2911 da07  .......r....)...
+00000a80: 6c6f 6767 696e 67da 1763 7279 7074 6f67  logging..cryptog
+00000a90: 7261 7068 792e 6578 6365 7074 696f 6e73  raphy.exceptions
+00000aa0: 7202 0000 00da 2963 7279 7074 6f67 7261  r.....)cryptogra
+00000ab0: 7068 792e 6861 7a6d 6174 2e70 7269 6d69  phy.hazmat.primi
+00000ac0: 7469 7665 732e 6173 796d 6d65 7472 6963  tives.asymmetric
+00000ad0: 7203 0000 00da 0c6d 756c 7469 666f 726d  r......multiform
+00000ae0: 6174 7372 0400 0000 7205 0000 00da 0668  atsr....r......h
+00000af0: 656c 7065 7272 0700 0000 7208 0000 0072  elperr....r....r
+00000b00: 0900 0000 da09 6765 744c 6f67 6765 7272  ......getLoggerr
+00000b10: 3700 0000 da06 6c6f 6767 6572 7212 0000  7.....loggerr...
+00000b20: 0072 0c00 0000 7210 0000 0072 1000 0000  .r....r....r....
+00000b30: 7210 0000 0072 1100 0000 da08 3c6d 6f64  r....r......<mod
+00000b40: 756c 653e 0100 0000 7310 0000 0008 000c  ule>....s.......
+00000b50: 020c 0110 0114 020a 0208 0312 08         .............
```

### Comparing `bovine-0.1.0/bovine/crypto/__pycache__/signature_checker.cpython-310.pyc` & `bovine-0.1.1/bovine/crypto/__pycache__/signature_checker.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 13 15:55:57 2023 UTC, .py size: 2942 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0d26 3864 7e0b 0000  o........&8d~...
+00000000: 6f0d 0d0a 0000 0000 a4ea 3a64 7e0b 0000  o.........:d~...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 7000 0000 6400  .....@...sp...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6400 6401 6c04  d.l.m.Z...d.d.l.
 00000050: 5a05 6400 6403 6c04 6d06 5a06 0100 6404  Z.d.d.l.m.Z...d.
 00000060: 6405 6c07 6d08 5a08 0100 6404 6406 6c09  d.l.m.Z...d.d.l.
 00000070: 6d0a 5a0a 0100 6404 6407 6c0b 6d0c 5a0c  m.Z...d.d.l.m.Z.
@@ -20,122 +20,123 @@
 00000130: 6402 8400 5a03 6403 6404 8400 5a04 6405  d...Z.d.d...Z.d.
 00000140: 5300 2906 da10 5369 676e 6174 7572 6543  S.)...SignatureC
 00000150: 6865 636b 6572 6302 0000 0000 0000 0000  heckerc.........
 00000160: 0000 0002 0000 0002 0000 0043 0000 0073  ...........C...s
 00000170: 0a00 0000 7c01 7c00 5f00 6400 5300 2901  ....|.|._.d.S.).
 00000180: 4e29 01da 0d6b 6579 5f72 6574 7269 6576  N)...key_retriev
 00000190: 6572 2902 da04 7365 6c66 7209 0000 00a9  er)...selfr.....
-000001a0: 0072 0b00 0000 fa53 2f77 6f6f 6470 6563  .r.....S/woodpec
+000001a0: 0072 0b00 0000 fa54 2f77 6f6f 6470 6563  .r.....T/woodpec
 000001b0: 6b65 722f 7372 632f 636f 6465 6265 7267  ker/src/codeberg
-000001c0: 2e6f 7267 2f68 656c 6765 2f62 6f76 696e  .org/helge/bovin
-000001d0: 652f 626f 7669 6e65 2f62 6f76 696e 652f  e/bovine/bovine/
-000001e0: 6372 7970 746f 2f73 6967 6e61 7475 7265  crypto/signature
-000001f0: 5f63 6865 636b 6572 2e70 79da 085f 5f69  _checker.py..__i
-00000200: 6e69 745f 5f10 0000 0073 0200 0000 0a01  nit__....s......
-00000210: 7a19 5369 676e 6174 7572 6543 6865 636b  z.SignatureCheck
-00000220: 6572 2e5f 5f69 6e69 745f 5f63 0200 0000  er.__init__c....
-00000230: 0000 0000 0000 0000 1100 0000 0a00 0000  ................
-00000240: c300 0000 7322 0200 0081 0164 017c 016a  ....s".....d.|.j
-00000250: 0076 0172 0d74 01a0 0264 02a1 0101 0064  .v.r.t...d.....d
-00000260: 0053 007c 016a 03a0 04a1 0064 036b 0272  .S.|.j.....d.k.r
-00000270: 207c 01a0 05a1 0049 0064 0048 007d 0274   |.....I.d.H.}.t
-00000280: 067c 0283 017d 036e 0264 007d 037c 0364  .|...}.n.d.}.|.d
-00000290: 0075 0172 447c 016a 0064 0419 007d 047c  .u.rD|.j.d...}.|
-000002a0: 0464 0064 0585 0219 00a0 04a1 007c 0464  .d.d.........|.d
-000002b0: 0564 0085 0219 0017 007d 047c 047c 036b  .d.......}.|.|.k
-000002c0: 0372 4474 01a0 0764 06a1 0101 0064 0053  .rDt...d.....d.S
-000002d0: 007a 9d74 0883 007d 0574 097c 016a 0064  .z.t...}.t.|.j.d
-000002e0: 0119 0083 017d 067c 06a0 0aa1 007d 0764  .....}.|.....}.d
-000002f0: 077c 0776 0173 5b64 087c 0776 0172 6374  .|.v.s[d.|.v.rct
-00000300: 01a0 0764 09a1 0101 0057 0064 0053 007c  ...d.....W.d.S.|
-00000310: 0364 0075 0172 7364 047c 0776 0172 7374  .d.u.rsd.|.v.rst
-00000320: 01a0 0764 0aa1 0101 0057 0064 0053 0074  ...d.....W.d.S.t
-00000330: 0b7c 016a 0064 0819 0083 017d 0874 0c6a  .|.j.d.....}.t.j
-00000340: 0d6a 0ea0 0f7c 08a1 0173 8f74 01a0 0764  .j...|...s.t...d
-00000350: 0b7c 016a 0064 0819 009b 009d 02a1 0101  .|.j.d..........
-00000360: 0057 0064 0053 007c 0744 005d 287d 097c  .W.d.S.|.D.](}.|
-00000370: 0964 076b 0272 b07c 016a 03a0 04a1 007d  .d.k.r.|.j.....}
-00000380: 0a74 107c 016a 1183 017d 0b7c 0b6a 127d  .t.|.j...}.|.j.}
-00000390: 0c7c 05a0 137c 097c 0a9b 0064 0c7c 0c9b  .|...|.|...d.|..
-000003a0: 009d 03a1 0201 0071 917c 05a0 137c 097c  .......q.|...|.|
-000003b0: 016a 007c 0919 00a1 0201 0071 917c 00a0  .j.|.......q.|..
-000003c0: 147c 066a 15a1 0149 0064 0048 005c 027d  .|.j...I.d.H.\.}
-000003d0: 0d7d 0e7c 0d64 0075 0072 d574 01a0 0264  .}.|.d.u.r.t...d
-000003e0: 0d7c 066a 159b 009d 02a1 0101 0057 0064  .|.j.........W.d
-000003f0: 0053 007c 05a0 167c 0d7c 066a 17a1 0272  .S.|...|.|.j...r
-00000400: df7c 0e57 0053 0057 0064 0053 0004 0074  .|.W.S.W.d.S...t
-00000410: 1890 0179 1001 007d 0f01 007a 2274 01a0  ...y...}...z"t..
-00000420: 1974 1a7c 0f83 01a1 0101 0074 01a0 197c  .t.|.......t...|
-00000430: 016a 00a1 0101 0074 1ba0 1ca1 00a0 1da1  .j.....t........
-00000440: 0044 005d 077d 1074 01a0 197c 10a1 0101  .D.].}.t...|....
-00000450: 0071 fd57 0059 0064 007d 0f7e 0f64 0053  .q.W.Y.d.}.~.d.S
-00000460: 0064 007d 0f7e 0f77 0177 0029 0e4e da09  .d.}.~.w.w.).N..
-00000470: 7369 676e 6174 7572 657a 1553 6967 6e61  signaturez.Signa
-00000480: 7475 7265 206e 6f74 2070 7265 7365 6e74  ture not present
-00000490: da04 706f 7374 da06 6469 6765 7374 e904  ..post..digest..
-000004a0: 0000 007a 1044 6966 6665 7265 6e74 2064  ...z.Different d
-000004b0: 6967 6573 747a 1028 7265 7175 6573 742d  igestz.(request-
-000004c0: 7461 7267 6574 29da 0464 6174 657a 2752  target)..datez'R
-000004d0: 6571 7569 7265 6420 6669 656c 6420 6e6f  equired field no
-000004e0: 7420 7072 6573 656e 7420 696e 2073 6967  t present in sig
-000004f0: 6e61 7475 7265 7a22 4469 6765 7374 206e  naturez"Digest n
-00000500: 6f74 2070 7265 7365 6e74 2c20 6275 7420  ot present, but 
-00000510: 636f 6d70 7574 6162 6c65 7a1e 456e 636f  computablez.Enco
-00000520: 756e 7465 7265 6420 696e 7661 6c69 6420  untered invalid 
-00000530: 6874 7470 2064 6174 6520 da01 207a 1c43  http date .. z.C
-00000540: 6f75 6c64 206e 6f74 2072 6574 7269 6576  ould not retriev
-00000550: 6520 6b65 7920 6672 6f6d 2029 1eda 0768  e key from )...h
-00000560: 6561 6465 7273 da06 6c6f 6767 6572 da05  eaders..logger..
-00000570: 6465 6275 67da 066d 6574 686f 64da 056c  debug..method..l
-00000580: 6f77 6572 da08 6765 745f 6461 7461 7205  ower..get_datar.
-00000590: 0000 00da 0777 6172 6e69 6e67 7206 0000  .....warningr...
-000005a0: 0072 0700 0000 da06 6669 656c 6473 7203  .r......fieldsr.
-000005b0: 0000 00da 0662 6f76 696e 65da 0575 7469  .....bovine..uti
-000005c0: 6c73 7212 0000 00da 1463 6865 636b 5f6d  lsr......check_m
-000005d0: 6178 5f6f 6666 7365 745f 6e6f 7772 0200  ax_offset_nowr..
-000005e0: 0000 da03 7572 6cda 0470 6174 68da 0a77  ....url..path..w
-000005f0: 6974 685f 6669 656c 6472 0900 0000 da06  ith_fieldr......
-00000600: 6b65 795f 6964 da06 7665 7269 6679 720e  key_id..verifyr.
-00000610: 0000 00da 0945 7863 6570 7469 6f6e da05  .....Exception..
-00000620: 6572 726f 72da 0373 7472 da09 7472 6163  error..str..trac
-00000630: 6562 6163 6bda 0a66 6f72 6d61 745f 6578  eback..format_ex
-00000640: 63da 0a73 706c 6974 6c69 6e65 7329 1172  c..splitlines).r
-00000650: 0a00 0000 da07 7265 7175 6573 74da 0464  ......request..d
-00000660: 6174 6172 1000 0000 5a0e 7265 7175 6573  atar....Z.reques
-00000670: 745f 6469 6765 7374 da0e 6874 7470 5f73  t_digest..http_s
-00000680: 6967 6e61 7475 7265 5a10 7061 7273 6564  ignatureZ.parsed
-00000690: 5f73 6967 6e61 7475 7265 5a10 7369 676e  _signatureZ.sign
-000006a0: 6174 7572 655f 6669 656c 6473 5a09 6874  ature_fieldsZ.ht
-000006b0: 7470 5f64 6174 65da 0566 6965 6c64 7217  tp_date..fieldr.
-000006c0: 0000 00da 0a70 6172 7365 645f 7572 6c72  .....parsed_urlr
-000006d0: 2000 0000 da0a 7075 626c 6963 5f6b 6579   .....public_key
-000006e0: da05 6f77 6e65 72da 0165 5a08 6c6f 675f  ..owner..eZ.log_
-000006f0: 6c69 6e65 720b 0000 0072 0b00 0000 720c  liner....r....r.
-00000700: 0000 00da 1276 616c 6964 6174 655f 7369  .....validate_si
-00000710: 676e 6174 7572 6513 0000 0073 6a00 0000  gnature....sj...
-00000720: 0280 0a01 0a01 0401 0e02 0e01 0a01 0402  ................
-00000730: 0802 0a01 1c01 0801 0a01 0401 0202 0601  ................
-00000740: 0e01 0801 0803 0801 0a02 0601 1002 0a01  ................
-00000750: 0601 0e02 0e01 0401 0e01 04ff 0603 0802  ................
-00000760: 0801 0a01 0a01 0601 1801 1402 1602 0802  ................
-00000770: 1201 0601 0e02 0601 06ff 1003 0e01 0c01  ................
-00000780: 1001 0c01 0e01 0880 02fb 7a23 5369 676e  ..........z#Sign
-00000790: 6174 7572 6543 6865 636b 6572 2e76 616c  atureChecker.val
-000007a0: 6964 6174 655f 7369 676e 6174 7572 654e  idate_signatureN
-000007b0: 2905 da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
-000007c0: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
-000007d0: 6e61 6d65 5f5f 720d 0000 0072 3200 0000  name__r....r2...
-000007e0: 720b 0000 0072 0b00 0000 720b 0000 0072  r....r....r....r
-000007f0: 0c00 0000 7208 0000 000f 0000 0073 0600  ....r........s..
-00000800: 0000 0800 0801 0c03 7208 0000 0029 11da  ........r....)..
-00000810: 076c 6f67 6769 6e67 7227 0000 00da 0c75  .loggingr'.....u
-00000820: 726c 6c69 622e 7061 7273 6572 0200 0000  rllib.parser....
-00000830: da11 626f 7669 6e65 2e75 7469 6c73 2e64  ..bovine.utils.d
-00000840: 6174 6572 1c00 0000 7203 0000 00da 0668  ater....r......h
-00000850: 656c 7065 7272 0500 0000 722c 0000 0072  elperr....r,...r
-00000860: 0600 0000 5a10 7369 676e 6174 7572 655f  ....Z.signature_
-00000870: 7061 7273 6572 7207 0000 00da 0967 6574  parserr......get
-00000880: 4c6f 6767 6572 7233 0000 0072 1500 0000  Loggerr3...r....
-00000890: 7208 0000 0072 0b00 0000 720b 0000 0072  r....r....r....r
-000008a0: 0b00 0000 720c 0000 00da 083c 6d6f 6475  ....r......<modu
-000008b0: 6c65 3e01 0000 0073 1400 0000 0800 0801  le>....s........
-000008c0: 0c01 0802 0c01 0c02 0c01 0c01 0a02 1203  ................
+000001c0: 2e6f 7267 2f62 6f76 696e 652f 626f 7669  .org/bovine/bovi
+000001d0: 6e65 2f62 6f76 696e 652f 626f 7669 6e65  ne/bovine/bovine
+000001e0: 2f63 7279 7074 6f2f 7369 676e 6174 7572  /crypto/signatur
+000001f0: 655f 6368 6563 6b65 722e 7079 da08 5f5f  e_checker.py..__
+00000200: 696e 6974 5f5f 1000 0000 7302 0000 000a  init__....s.....
+00000210: 017a 1953 6967 6e61 7475 7265 4368 6563  .z.SignatureChec
+00000220: 6b65 722e 5f5f 696e 6974 5f5f 6302 0000  ker.__init__c...
+00000230: 0000 0000 0000 0000 0011 0000 000a 0000  ................
+00000240: 00c3 0000 0073 2202 0000 8101 6401 7c01  .....s".....d.|.
+00000250: 6a00 7601 720d 7401 a002 6402 a101 0100  j.v.r.t...d.....
+00000260: 6400 5300 7c01 6a03 a004 a100 6403 6b02  d.S.|.j.....d.k.
+00000270: 7220 7c01 a005 a100 4900 6400 4800 7d02  r |.....I.d.H.}.
+00000280: 7406 7c02 8301 7d03 6e02 6400 7d03 7c03  t.|...}.n.d.}.|.
+00000290: 6400 7501 7244 7c01 6a00 6404 1900 7d04  d.u.rD|.j.d...}.
+000002a0: 7c04 6400 6405 8502 1900 a004 a100 7c04  |.d.d.........|.
+000002b0: 6405 6400 8502 1900 1700 7d04 7c04 7c03  d.d.......}.|.|.
+000002c0: 6b03 7244 7401 a007 6406 a101 0100 6400  k.rDt...d.....d.
+000002d0: 5300 7a9d 7408 8300 7d05 7409 7c01 6a00  S.z.t...}.t.|.j.
+000002e0: 6401 1900 8301 7d06 7c06 a00a a100 7d07  d.....}.|.....}.
+000002f0: 6407 7c07 7601 735b 6408 7c07 7601 7263  d.|.v.s[d.|.v.rc
+00000300: 7401 a007 6409 a101 0100 5700 6400 5300  t...d.....W.d.S.
+00000310: 7c03 6400 7501 7273 6404 7c07 7601 7273  |.d.u.rsd.|.v.rs
+00000320: 7401 a007 640a a101 0100 5700 6400 5300  t...d.....W.d.S.
+00000330: 740b 7c01 6a00 6408 1900 8301 7d08 740c  t.|.j.d.....}.t.
+00000340: 6a0d 6a0e a00f 7c08 a101 738f 7401 a007  j.j...|...s.t...
+00000350: 640b 7c01 6a00 6408 1900 9b00 9d02 a101  d.|.j.d.........
+00000360: 0100 5700 6400 5300 7c07 4400 5d28 7d09  ..W.d.S.|.D.](}.
+00000370: 7c09 6407 6b02 72b0 7c01 6a03 a004 a100  |.d.k.r.|.j.....
+00000380: 7d0a 7410 7c01 6a11 8301 7d0b 7c0b 6a12  }.t.|.j...}.|.j.
+00000390: 7d0c 7c05 a013 7c09 7c0a 9b00 640c 7c0c  }.|...|.|...d.|.
+000003a0: 9b00 9d03 a102 0100 7191 7c05 a013 7c09  ........q.|...|.
+000003b0: 7c01 6a00 7c09 1900 a102 0100 7191 7c00  |.j.|.......q.|.
+000003c0: a014 7c06 6a15 a101 4900 6400 4800 5c02  ..|.j...I.d.H.\.
+000003d0: 7d0d 7d0e 7c0d 6400 7500 72d5 7401 a002  }.}.|.d.u.r.t...
+000003e0: 640d 7c06 6a15 9b00 9d02 a101 0100 5700  d.|.j.........W.
+000003f0: 6400 5300 7c05 a016 7c0d 7c06 6a17 a102  d.S.|...|.|.j...
+00000400: 72df 7c0e 5700 5300 5700 6400 5300 0400  r.|.W.S.W.d.S...
+00000410: 7418 9001 7910 0100 7d0f 0100 7a22 7401  t...y...}...z"t.
+00000420: a019 741a 7c0f 8301 a101 0100 7401 a019  ..t.|.......t...
+00000430: 7c01 6a00 a101 0100 741b a01c a100 a01d  |.j.....t.......
+00000440: a100 4400 5d07 7d10 7401 a019 7c10 a101  ..D.].}.t...|...
+00000450: 0100 71fd 5700 5900 6400 7d0f 7e0f 6400  ..q.W.Y.d.}.~.d.
+00000460: 5300 6400 7d0f 7e0f 7701 7700 290e 4eda  S.d.}.~.w.w.).N.
+00000470: 0973 6967 6e61 7475 7265 7a15 5369 676e  .signaturez.Sign
+00000480: 6174 7572 6520 6e6f 7420 7072 6573 656e  ature not presen
+00000490: 74da 0470 6f73 74da 0664 6967 6573 74e9  t..post..digest.
+000004a0: 0400 0000 7a10 4469 6666 6572 656e 7420  ....z.Different 
+000004b0: 6469 6765 7374 7a10 2872 6571 7565 7374  digestz.(request
+000004c0: 2d74 6172 6765 7429 da04 6461 7465 7a27  -target)..datez'
+000004d0: 5265 7175 6972 6564 2066 6965 6c64 206e  Required field n
+000004e0: 6f74 2070 7265 7365 6e74 2069 6e20 7369  ot present in si
+000004f0: 676e 6174 7572 657a 2244 6967 6573 7420  gnaturez"Digest 
+00000500: 6e6f 7420 7072 6573 656e 742c 2062 7574  not present, but
+00000510: 2063 6f6d 7075 7461 626c 657a 1e45 6e63   computablez.Enc
+00000520: 6f75 6e74 6572 6564 2069 6e76 616c 6964  ountered invalid
+00000530: 2068 7474 7020 6461 7465 20da 0120 7a1c   http date .. z.
+00000540: 436f 756c 6420 6e6f 7420 7265 7472 6965  Could not retrie
+00000550: 7665 206b 6579 2066 726f 6d20 291e da07  ve key from )...
+00000560: 6865 6164 6572 73da 066c 6f67 6765 72da  headers..logger.
+00000570: 0564 6562 7567 da06 6d65 7468 6f64 da05  .debug..method..
+00000580: 6c6f 7765 72da 0867 6574 5f64 6174 6172  lower..get_datar
+00000590: 0500 0000 da07 7761 726e 696e 6772 0600  ......warningr..
+000005a0: 0000 7207 0000 00da 0666 6965 6c64 7372  ..r......fieldsr
+000005b0: 0300 0000 da06 626f 7669 6e65 da05 7574  ......bovine..ut
+000005c0: 696c 7372 1200 0000 da14 6368 6563 6b5f  ilsr......check_
+000005d0: 6d61 785f 6f66 6673 6574 5f6e 6f77 7202  max_offset_nowr.
+000005e0: 0000 00da 0375 726c da04 7061 7468 da0a  .....url..path..
+000005f0: 7769 7468 5f66 6965 6c64 7209 0000 00da  with_fieldr.....
+00000600: 066b 6579 5f69 64da 0676 6572 6966 7972  .key_id..verifyr
+00000610: 0e00 0000 da09 4578 6365 7074 696f 6eda  ......Exception.
+00000620: 0565 7272 6f72 da03 7374 72da 0974 7261  .error..str..tra
+00000630: 6365 6261 636b da0a 666f 726d 6174 5f65  ceback..format_e
+00000640: 7863 da0a 7370 6c69 746c 696e 6573 2911  xc..splitlines).
+00000650: 720a 0000 00da 0772 6571 7565 7374 da04  r......request..
+00000660: 6461 7461 7210 0000 005a 0e72 6571 7565  datar....Z.reque
+00000670: 7374 5f64 6967 6573 74da 0e68 7474 705f  st_digest..http_
+00000680: 7369 676e 6174 7572 655a 1070 6172 7365  signatureZ.parse
+00000690: 645f 7369 676e 6174 7572 655a 1073 6967  d_signatureZ.sig
+000006a0: 6e61 7475 7265 5f66 6965 6c64 735a 0968  nature_fieldsZ.h
+000006b0: 7474 705f 6461 7465 da05 6669 656c 6472  ttp_date..fieldr
+000006c0: 1700 0000 da0a 7061 7273 6564 5f75 726c  ......parsed_url
+000006d0: 7220 0000 00da 0a70 7562 6c69 635f 6b65  r .....public_ke
+000006e0: 79da 056f 776e 6572 da01 65da 086c 6f67  y..owner..e..log
+000006f0: 5f6c 696e 6572 0b00 0000 720b 0000 0072  _liner....r....r
+00000700: 0c00 0000 da12 7661 6c69 6461 7465 5f73  ......validate_s
+00000710: 6967 6e61 7475 7265 1300 0000 736a 0000  ignature....sj..
+00000720: 0002 800a 010a 0104 010e 020e 010a 0104  ................
+00000730: 0208 020a 011c 0108 010a 0104 0102 0206  ................
+00000740: 010e 0108 0108 0308 010a 0206 0110 020a  ................
+00000750: 0106 010e 020e 0104 010e 0104 ff06 0308  ................
+00000760: 0208 010a 010a 0106 0118 0114 0216 0208  ................
+00000770: 0212 0106 010e 0206 0106 ff10 030e 010c  ................
+00000780: 0110 010c 010e 0108 8002 fb7a 2353 6967  ...........z#Sig
+00000790: 6e61 7475 7265 4368 6563 6b65 722e 7661  natureChecker.va
+000007a0: 6c69 6461 7465 5f73 6967 6e61 7475 7265  lidate_signature
+000007b0: 4e29 05da 085f 5f6e 616d 655f 5fda 0a5f  N)...__name__.._
+000007c0: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
+000007d0: 6c6e 616d 655f 5f72 0d00 0000 7233 0000  lname__r....r3..
+000007e0: 0072 0b00 0000 720b 0000 0072 0b00 0000  .r....r....r....
+000007f0: 720c 0000 0072 0800 0000 0f00 0000 7306  r....r........s.
+00000800: 0000 0008 0008 010c 0372 0800 0000 2911  .........r....).
+00000810: da07 6c6f 6767 696e 6772 2700 0000 da0c  ..loggingr'.....
+00000820: 7572 6c6c 6962 2e70 6172 7365 7202 0000  urllib.parser...
+00000830: 00da 1162 6f76 696e 652e 7574 696c 732e  ...bovine.utils.
+00000840: 6461 7465 721c 0000 0072 0300 0000 da06  dater....r......
+00000850: 6865 6c70 6572 7205 0000 0072 2c00 0000  helperr....r,...
+00000860: 7206 0000 005a 1073 6967 6e61 7475 7265  r....Z.signature
+00000870: 5f70 6172 7365 7272 0700 0000 da09 6765  _parserr......ge
+00000880: 744c 6f67 6765 7272 3400 0000 7215 0000  tLoggerr4...r...
+00000890: 0072 0800 0000 720b 0000 0072 0b00 0000  .r....r....r....
+000008a0: 720b 0000 0072 0c00 0000 da08 3c6d 6f64  r....r......<mod
+000008b0: 756c 653e 0100 0000 7314 0000 0008 0008  ule>....s.......
+000008c0: 010c 0108 020c 010c 020c 010c 010a 0212  ................
+000008d0: 03                                       .
```

### Comparing `bovine-0.1.0/bovine/crypto/__pycache__/signature_parser.cpython-310.pyc` & `bovine-0.1.1/bovine/crypto/__pycache__/signature_parser.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 13 15:55:57 2023 UTC, .py size: 1266 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0d26 3864 f204 0000  o........&8d....
+00000000: 6f0d 0d0a 0000 0000 a4ea 3a64 f204 0000  o.........:d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 2c00 0000 6400  .....@...s,...d.
 00000030: 6401 6c00 5a00 6500 a001 6502 a101 5a03  d.l.Z.e...e...Z.
 00000040: 4700 6402 6403 8400 6403 8302 5a04 6404  G.d.d...d...Z.d.
 00000050: 6405 8400 5a05 6401 5300 2906 e900 0000  d...Z.d.S.).....
 00000060: 004e 6300 0000 0000 0000 0000 0000 0000  .Nc.............
 00000070: 0000 0003 0000 0040 0000 0073 2800 0000  .......@...s(...
@@ -23,90 +23,90 @@
 00000160: 6f72 7465 6420 616c 676f 7269 7468 6d20  orted algorithm 
 00000170: 2907 da06 6b65 795f 6964 da09 616c 676f  )...key_id..algo
 00000180: 7269 7468 6dda 0768 6561 6465 7273 da09  rithm..headers..
 00000190: 7369 676e 6174 7572 65da 066c 6f67 6765  signature..logge
 000001a0: 72da 0565 7272 6f72 da09 4578 6365 7074  r..error..Except
 000001b0: 696f 6e29 05da 0473 656c 6672 0400 0000  ion)...selfr....
 000001c0: 7205 0000 0072 0600 0000 7207 0000 00a9  r....r....r.....
-000001d0: 0072 0c00 0000 fa52 2f77 6f6f 6470 6563  .r.....R/woodpec
+000001d0: 0072 0c00 0000 fa53 2f77 6f6f 6470 6563  .r.....S/woodpec
 000001e0: 6b65 722f 7372 632f 636f 6465 6265 7267  ker/src/codeberg
-000001f0: 2e6f 7267 2f68 656c 6765 2f62 6f76 696e  .org/helge/bovin
-00000200: 652f 626f 7669 6e65 2f62 6f76 696e 652f  e/bovine/bovine/
-00000210: 6372 7970 746f 2f73 6967 6e61 7475 7265  crypto/signature
-00000220: 5f70 6172 7365 722e 7079 da08 5f5f 696e  _parser.py..__in
-00000230: 6974 5f5f 0700 0000 7316 0000 0006 0106  it__....s.......
-00000240: 0106 0106 010a 0212 010c 010c 010c 0110  ................
-00000250: 0204 fa7a 1253 6967 6e61 7475 7265 2e5f  ...z.Signature._
-00000260: 5f69 6e69 745f 5f63 0100 0000 0000 0000  _init__c........
-00000270: 0000 0000 0100 0000 0300 0000 4300 0000  ............C...
-00000280: 730c 0000 007c 006a 00a0 0164 01a1 0153  s....|.j...d...S
-00000290: 0029 024e da01 2029 0272 0600 0000 da05  .).N.. ).r......
-000002a0: 7370 6c69 7429 0172 0b00 0000 720c 0000  split).r....r...
-000002b0: 0072 0c00 0000 720d 0000 00da 0666 6965  .r....r......fie
-000002c0: 6c64 7315 0000 0073 0200 0000 0c01 7a10  lds....s......z.
-000002d0: 5369 676e 6174 7572 652e 6669 656c 6473  Signature.fields
-000002e0: 6301 0000 0000 0000 0000 0000 0003 0000  c...............
-000002f0: 0008 0000 0043 0000 0073 7000 0000 7a25  .....C...sp...z%
-00000300: 7c00 a000 6401 a101 7d01 6402 6403 8400  |...d...}.d.d...
-00000310: 7c01 4400 8301 7d01 6404 6405 8400 7c01  |.D...}.d.d...|.
-00000320: 4400 8301 7d02 7401 7c02 6406 1900 7c02  D...}.t.|.d...|.
-00000330: a002 6407 6408 a102 7c02 6409 1900 7c02  ..d.d...|.d...|.
-00000340: 640a 1900 8304 5700 5300 0400 7403 7937  d.....W.S...t.y7
-00000350: 0100 0100 0100 7404 a005 640b 7c00 9b00  ......t...d.|...
-00000360: 9d02 a101 0100 5900 6400 5300 7700 290c  ......Y.d.S.w.).
-00000370: 4efa 012c 6301 0000 0000 0000 0000 0000  N..,c...........
-00000380: 0002 0000 0006 0000 0053 0000 0073 1800  .........S...s..
-00000390: 0000 6700 7c00 5d08 7d01 7c01 a000 6400  ..g.|.].}.|...d.
-000003a0: 6401 a102 9102 7102 5300 2902 7a02 3d22  d.....q.S.).z.="
-000003b0: e901 0000 0029 0172 1000 0000 a902 da02  .....).r........
-000003c0: 2e30 da01 7872 0c00 0000 720c 0000 0072  .0..xr....r....r
-000003d0: 0d00 0000 da0a 3c6c 6973 7463 6f6d 703e  ......<listcomp>
-000003e0: 1c00 0000 7302 0000 0018 007a 3353 6967  ....s......z3Sig
-000003f0: 6e61 7475 7265 2e66 726f 6d5f 7369 676e  nature.from_sign
-00000400: 6174 7572 655f 6865 6164 6572 2e3c 6c6f  ature_header.<lo
-00000410: 6361 6c73 3e2e 3c6c 6973 7463 6f6d 703e  cals>.<listcomp>
-00000420: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-00000430: 0007 0000 0053 0000 0073 2200 0000 6900  .....S...s"...i.
-00000440: 7c00 5d0d 7d01 7c01 6400 1900 7c01 6401  |.].}.|.d...|.d.
-00000450: 1900 a000 6402 6403 a102 9302 7102 5300  ....d.d.....q.S.
-00000460: 2904 7201 0000 0072 1300 0000 fa01 22da  ).r....r......".
-00000470: 0029 01da 0772 6570 6c61 6365 7214 0000  .)...replacer...
-00000480: 0072 0c00 0000 720c 0000 0072 0d00 0000  .r....r....r....
-00000490: da0a 3c64 6963 7463 6f6d 703e 1d00 0000  ..<dictcomp>....
-000004a0: 7302 0000 0022 007a 3353 6967 6e61 7475  s....".z3Signatu
-000004b0: 7265 2e66 726f 6d5f 7369 676e 6174 7572  re.from_signatur
-000004c0: 655f 6865 6164 6572 2e3c 6c6f 6361 6c73  e_header.<locals
-000004d0: 3e2e 3c64 6963 7463 6f6d 703e 5a05 6b65  >.<dictcomp>Z.ke
-000004e0: 7949 6472 0500 0000 7203 0000 0072 0600  yIdr....r....r..
-000004f0: 0000 7207 0000 007a 1a66 6169 6c65 6420  ..r....z.failed 
-00000500: 746f 2070 6172 7365 2073 6967 6e61 7475  to parse signatu
-00000510: 7265 2029 0672 1000 0000 7202 0000 00da  re ).r....r.....
-00000520: 0367 6574 720a 0000 0072 0800 0000 7209  .getr....r....r.
-00000530: 0000 0029 03da 0668 6561 6465 7272 0600  ...)...headerr..
-00000540: 0000 da06 7061 7273 6564 720c 0000 0072  ....parsedr....r
-00000550: 0c00 0000 720d 0000 00da 1566 726f 6d5f  ....r......from_
-00000560: 7369 676e 6174 7572 655f 6865 6164 6572  signature_header
-00000570: 1800 0000 731a 0000 0002 020a 010e 010e  ....s...........
-00000580: 0102 0206 010a 0106 0106 0106 fc0c 0616  ................
-00000590: 0102 ff7a 1f53 6967 6e61 7475 7265 2e66  ...z.Signature.f
-000005a0: 726f 6d5f 7369 676e 6174 7572 655f 6865  rom_signature_he
-000005b0: 6164 6572 4e29 07da 085f 5f6e 616d 655f  aderN)...__name_
-000005c0: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
-000005d0: 5f71 7561 6c6e 616d 655f 5f72 0e00 0000  _qualname__r....
-000005e0: 7211 0000 00da 0c73 7461 7469 636d 6574  r......staticmet
-000005f0: 686f 6472 1f00 0000 720c 0000 0072 0c00  hodr....r....r..
-00000600: 0000 720c 0000 0072 0d00 0000 7202 0000  ..r....r....r...
-00000610: 0006 0000 0073 0a00 0000 0800 0801 080e  .....s..........
-00000620: 0203 0e01 7202 0000 0063 0100 0000 0000  ....r....c......
-00000630: 0000 0000 0000 0100 0000 0300 0000 4300  ..............C.
-00000640: 0000 730a 0000 0074 00a0 017c 00a1 0153  ..s....t...|...S
-00000650: 0029 014e 2902 7202 0000 0072 1f00 0000  .).N).r....r....
-00000660: 2901 721d 0000 0072 0c00 0000 720c 0000  ).r....r....r...
-00000670: 0072 0d00 0000 da16 7061 7273 655f 7369  .r......parse_si
-00000680: 676e 6174 7572 655f 6865 6164 6572 2900  gnature_header).
-00000690: 0000 7302 0000 000a 0172 2400 0000 2906  ..s......r$...).
-000006a0: da07 6c6f 6767 696e 67da 0967 6574 4c6f  ..logging..getLo
-000006b0: 6767 6572 7220 0000 0072 0800 0000 7202  ggerr ...r....r.
-000006c0: 0000 0072 2400 0000 720c 0000 0072 0c00  ...r$...r....r..
-000006d0: 0000 720c 0000 0072 0d00 0000 da08 3c6d  ..r....r......<m
-000006e0: 6f64 756c 653e 0100 0000 7308 0000 0008  odule>....s.....
-000006f0: 000a 020e 030c 23                        ......#
+000001f0: 2e6f 7267 2f62 6f76 696e 652f 626f 7669  .org/bovine/bovi
+00000200: 6e65 2f62 6f76 696e 652f 626f 7669 6e65  ne/bovine/bovine
+00000210: 2f63 7279 7074 6f2f 7369 676e 6174 7572  /crypto/signatur
+00000220: 655f 7061 7273 6572 2e70 79da 085f 5f69  e_parser.py..__i
+00000230: 6e69 745f 5f07 0000 0073 1600 0000 0601  nit__....s......
+00000240: 0601 0601 0601 0a02 1201 0c01 0c01 0c01  ................
+00000250: 1002 04fa 7a12 5369 676e 6174 7572 652e  ....z.Signature.
+00000260: 5f5f 696e 6974 5f5f 6301 0000 0000 0000  __init__c.......
+00000270: 0000 0000 0001 0000 0003 0000 0043 0000  .............C..
+00000280: 0073 0c00 0000 7c00 6a00 a001 6401 a101  .s....|.j...d...
+00000290: 5300 2902 4eda 0120 2902 7206 0000 00da  S.).N.. ).r.....
+000002a0: 0573 706c 6974 2901 720b 0000 0072 0c00  .split).r....r..
+000002b0: 0000 720c 0000 0072 0d00 0000 da06 6669  ..r....r......fi
+000002c0: 656c 6473 1500 0000 7302 0000 000c 017a  elds....s......z
+000002d0: 1053 6967 6e61 7475 7265 2e66 6965 6c64  .Signature.field
+000002e0: 7363 0100 0000 0000 0000 0000 0000 0300  sc..............
+000002f0: 0000 0800 0000 4300 0000 7370 0000 007a  ......C...sp...z
+00000300: 257c 00a0 0064 01a1 017d 0164 0264 0384  %|...d...}.d.d..
+00000310: 007c 0144 0083 017d 0164 0464 0584 007c  .|.D...}.d.d...|
+00000320: 0144 0083 017d 0274 017c 0264 0619 007c  .D...}.t.|.d...|
+00000330: 02a0 0264 0764 08a1 027c 0264 0919 007c  ...d.d...|.d...|
+00000340: 0264 0a19 0083 0457 0053 0004 0074 0379  .d.....W.S...t.y
+00000350: 3701 0001 0001 0074 04a0 0564 0b7c 009b  7......t...d.|..
+00000360: 009d 02a1 0101 0059 0064 0053 0077 0029  .......Y.d.S.w.)
+00000370: 0c4e fa01 2c63 0100 0000 0000 0000 0000  .N..,c..........
+00000380: 0000 0200 0000 0600 0000 5300 0000 7318  ..........S...s.
+00000390: 0000 0067 007c 005d 087d 017c 01a0 0064  ...g.|.].}.|...d
+000003a0: 0064 01a1 0291 0271 0253 0029 027a 023d  .d.....q.S.).z.=
+000003b0: 22e9 0100 0000 2901 7210 0000 00a9 02da  ".....).r.......
+000003c0: 022e 30da 0178 720c 0000 0072 0c00 0000  ..0..xr....r....
+000003d0: 720d 0000 00da 0a3c 6c69 7374 636f 6d70  r......<listcomp
+000003e0: 3e1c 0000 0073 0200 0000 1800 7a33 5369  >....s......z3Si
+000003f0: 676e 6174 7572 652e 6672 6f6d 5f73 6967  gnature.from_sig
+00000400: 6e61 7475 7265 5f68 6561 6465 722e 3c6c  nature_header.<l
+00000410: 6f63 616c 733e 2e3c 6c69 7374 636f 6d70  ocals>.<listcomp
+00000420: 3e63 0100 0000 0000 0000 0000 0000 0200  >c..............
+00000430: 0000 0700 0000 5300 0000 7322 0000 0069  ......S...s"...i
+00000440: 007c 005d 0d7d 017c 0164 0019 007c 0164  .|.].}.|.d...|.d
+00000450: 0119 00a0 0064 0264 03a1 0293 0271 0253  .....d.d.....q.S
+00000460: 0029 0472 0100 0000 7213 0000 00fa 0122  .).r....r......"
+00000470: da00 2901 da07 7265 706c 6163 6572 1400  ..)...replacer..
+00000480: 0000 720c 0000 0072 0c00 0000 720d 0000  ..r....r....r...
+00000490: 00da 0a3c 6469 6374 636f 6d70 3e1d 0000  ...<dictcomp>...
+000004a0: 0073 0200 0000 2200 7a33 5369 676e 6174  .s....".z3Signat
+000004b0: 7572 652e 6672 6f6d 5f73 6967 6e61 7475  ure.from_signatu
+000004c0: 7265 5f68 6561 6465 722e 3c6c 6f63 616c  re_header.<local
+000004d0: 733e 2e3c 6469 6374 636f 6d70 3e5a 056b  s>.<dictcomp>Z.k
+000004e0: 6579 4964 7205 0000 0072 0300 0000 7206  eyIdr....r....r.
+000004f0: 0000 0072 0700 0000 7a1a 6661 696c 6564  ...r....z.failed
+00000500: 2074 6f20 7061 7273 6520 7369 676e 6174   to parse signat
+00000510: 7572 6520 2906 7210 0000 0072 0200 0000  ure ).r....r....
+00000520: da03 6765 7472 0a00 0000 7208 0000 0072  ..getr....r....r
+00000530: 0900 0000 2903 da06 6865 6164 6572 7206  ....)...headerr.
+00000540: 0000 00da 0670 6172 7365 6472 0c00 0000  .....parsedr....
+00000550: 720c 0000 0072 0d00 0000 da15 6672 6f6d  r....r......from
+00000560: 5f73 6967 6e61 7475 7265 5f68 6561 6465  _signature_heade
+00000570: 7218 0000 0073 1a00 0000 0202 0a01 0e01  r....s..........
+00000580: 0e01 0202 0601 0a01 0601 0601 06fc 0c06  ................
+00000590: 1601 02ff 7a1f 5369 676e 6174 7572 652e  ....z.Signature.
+000005a0: 6672 6f6d 5f73 6967 6e61 7475 7265 5f68  from_signature_h
+000005b0: 6561 6465 724e 2907 da08 5f5f 6e61 6d65  eaderN)...__name
+000005c0: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
+000005d0: 5f5f 7175 616c 6e61 6d65 5f5f 720e 0000  __qualname__r...
+000005e0: 0072 1100 0000 da0c 7374 6174 6963 6d65  .r......staticme
+000005f0: 7468 6f64 721f 0000 0072 0c00 0000 720c  thodr....r....r.
+00000600: 0000 0072 0c00 0000 720d 0000 0072 0200  ...r....r....r..
+00000610: 0000 0600 0000 730a 0000 0008 0008 0108  ......s.........
+00000620: 0e02 030e 0172 0200 0000 6301 0000 0000  .....r....c.....
+00000630: 0000 0000 0000 0001 0000 0003 0000 0043  ...............C
+00000640: 0000 0073 0a00 0000 7400 a001 7c00 a101  ...s....t...|...
+00000650: 5300 2901 4e29 0272 0200 0000 721f 0000  S.).N).r....r...
+00000660: 0029 0172 1d00 0000 720c 0000 0072 0c00  .).r....r....r..
+00000670: 0000 720d 0000 00da 1670 6172 7365 5f73  ..r......parse_s
+00000680: 6967 6e61 7475 7265 5f68 6561 6465 7229  ignature_header)
+00000690: 0000 0073 0200 0000 0a01 7224 0000 0029  ...s......r$...)
+000006a0: 06da 076c 6f67 6769 6e67 da09 6765 744c  ...logging..getL
+000006b0: 6f67 6765 7272 2000 0000 7208 0000 0072  oggerr ...r....r
+000006c0: 0200 0000 7224 0000 0072 0c00 0000 720c  ....r$...r....r.
+000006d0: 0000 0072 0c00 0000 720d 0000 00da 083c  ...r....r......<
+000006e0: 6d6f 6475 6c65 3e01 0000 0073 0800 0000  module>....s....
+000006f0: 0800 0a02 0e03 0c23                      .......#
```

### Comparing `bovine-0.1.0/bovine/crypto/__pycache__/test.cpython-310.pyc` & `bovine-0.1.1/bovine/crypto/__pycache__/test.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 13 15:55:57 2023 UTC, .py size: 2199 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0d26 3864 9708 0000  o........&8d....
+00000000: 6f0d 0d0a 0000 0000 a4ea 3a64 9708 0000  o.........:d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0001 0000 0040 0000 0073 0c00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 5a01 6402 5300 2903 61c4 0100  Z.d.Z.d.S.).a...
 00000040: 000a 2d2d 2d2d 2d42 4547 494e 2050 5542  ..-----BEGIN PUB
 00000050: 4c49 4320 4b45 592d 2d2d 2d2d 0a4d 4949  LIC KEY-----.MII
 00000060: 4249 6a41 4e42 676b 7168 6b69 4739 7730  BIjANBgkqhkiG9w0
 00000070: 4241 5145 4641 414f 4341 5138 414d 4949  BAQEFAAOCAQ8AMII
@@ -135,14 +135,14 @@
 00000860: 6372 7670 4b59 415a 7a6a 6831 4b43 725a  crvpKYAZzjh1KCrZ
 00000870: 3135 4f59 7237 5a68 6c45 5773 364d 510a  15OYr7ZhlEWs6MQ.
 00000880: 5262 6444 7133 364f 3435 7570 6c4f 6530  RbdDq36O45uplOe0
 00000890: 6865 654f 7350 686a 0a2d 2d2d 2d2d 454e  heeOsPhj.-----EN
 000008a0: 4420 5052 4956 4154 4520 4b45 592d 2d2d  D PRIVATE KEY---
 000008b0: 2d2d 0a4e 2902 da0a 7075 626c 6963 5f6b  --.N)...public_k
 000008c0: 6579 da0b 7072 6976 6174 655f 6b65 79a9  ey..private_key.
-000008d0: 0072 0300 0000 7203 0000 00fa 462f 776f  .r....r.....F/wo
+000008d0: 0072 0300 0000 7203 0000 00fa 472f 776f  .r....r.....G/wo
 000008e0: 6f64 7065 636b 6572 2f73 7263 2f63 6f64  odpecker/src/cod
-000008f0: 6562 6572 672e 6f72 672f 6865 6c67 652f  eberg.org/helge/
-00000900: 626f 7669 6e65 2f62 6f76 696e 652f 626f  bovine/bovine/bo
-00000910: 7669 6e65 2f63 7279 7074 6f2f 7465 7374  vine/crypto/test
-00000920: 2e70 79da 083c 6d6f 6475 6c65 3e01 0000  .py..<module>...
-00000930: 0073 0400 0000 0400 080c                 .s........
+000008f0: 6562 6572 672e 6f72 672f 626f 7669 6e65  eberg.org/bovine
+00000900: 2f62 6f76 696e 652f 626f 7669 6e65 2f62  /bovine/bovine/b
+00000910: 6f76 696e 652f 6372 7970 746f 2f74 6573  ovine/crypto/tes
+00000920: 742e 7079 da08 3c6d 6f64 756c 653e 0100  t.py..<module>..
+00000930: 0000 7304 0000 0004 0008 0c              ..s........
```

### Comparing `bovine-0.1.0/bovine/crypto/__pycache__/test_crypto.cpython-310-pytest-7.3.0.pyc` & `bovine-0.1.1/bovine/crypto/__pycache__/test_crypto.cpython-310-pytest-7.3.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 13 15:55:57 2023 UTC, .py size: 4989 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0d26 3864 7d13 0000  o........&8d}...
+00000000: 6f0d 0d0a 0000 0000 a4ea 3a64 7d13 0000  o.........:d}...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 a600 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6402 6c06 6d07  ..m.Z...d.d.l.m.
 00000050: 5a07 6d08 5a08 6d09 5a09 0100 6403 6404  Z.m.Z.m.Z...d.d.
 00000060: 6c0a 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d 6d0e  l.m.Z.m.Z.m.Z.m.
 00000070: 5a0e 0100 6403 6405 6c0f 6d10 5a10 0100  Z...d.d.l.m.Z...
@@ -82,283 +82,283 @@
 00000510: da0e 4173 7365 7274 696f 6e45 7272 6f72  ..AssertionError
 00000520: da13 5f66 6f72 6d61 745f 6578 706c 616e  .._format_explan
 00000530: 6174 696f 6eda 0865 6e64 7377 6974 6829  ation..endswith)
 00000540: 0672 0b00 0000 7210 0000 00da 0b40 7079  .r....r......@py
 00000550: 5f61 7373 6572 7431 da0b 4070 795f 6173  _assert1..@py_as
 00000560: 7365 7274 33da 0b40 7079 5f61 7373 6572  sert3..@py_asser
 00000570: 7435 da0b 4070 795f 666f 726d 6174 37a9  t5..@py_format7.
-00000580: 0072 1e00 0000 fa4d 2f77 6f6f 6470 6563  .r.....M/woodpec
+00000580: 0072 1e00 0000 fa4e 2f77 6f6f 6470 6563  .r.....N/woodpec
 00000590: 6b65 722f 7372 632f 636f 6465 6265 7267  ker/src/codeberg
-000005a0: 2e6f 7267 2f68 656c 6765 2f62 6f76 696e  .org/helge/bovin
-000005b0: 652f 626f 7669 6e65 2f62 6f76 696e 652f  e/bovine/bovine/
-000005c0: 6372 7970 746f 2f74 6573 745f 6372 7970  crypto/test_cryp
-000005d0: 746f 2e70 79da 2474 6573 745f 6765 6e65  to.py.$test_gene
-000005e0: 7261 7465 5f72 7361 5f70 7562 6c69 635f  rate_rsa_public_
-000005f0: 7072 6976 6174 655f 6b65 790c 0000 0073  private_key....s
-00000600: 0a00 0000 0a01 7402 7401 7402 7801 7220  ......t.t.t.x.r 
-00000610: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-00000620: 0600 0000 0700 0000 4300 0000 7388 0000  ........C...s...
-00000630: 0064 017d 0074 007c 0083 017d 0164 027d  .d.}.t.|...}.d.}
-00000640: 027c 017c 026b 027d 037c 0373 3e74 01a0  .|.|.k.}.|.s>t..
-00000650: 0264 037c 0366 0164 047c 017c 0266 02a1  .d.|.f.d.|.|.f..
-00000660: 0464 0574 03a0 04a1 0076 0073 2374 01a0  .d.t.....v.s#t..
-00000670: 057c 01a1 0172 2874 01a0 067c 01a1 016e  .|...r(t...|...n
-00000680: 0164 0574 01a0 067c 02a1 0164 069c 0216  .d.t...|...d....
-00000690: 007d 0464 0764 087c 0469 0116 007d 0574  .}.d.d.|.i...}.t
-000006a0: 0774 01a0 087c 05a1 0183 0182 0164 0004  .t...|.......d..
-000006b0: 007d 037d 0264 0053 0029 094e 5a30 7a33  .}.}.d.S.).NZ0z3
-000006c0: 7532 5978 636f 7773 6172 6574 6865 6265  u2Yxcowsarethebe
-000006d0: 7374 636f 7773 6172 6574 6865 6265 7374  stcowsarethebest
-000006e0: 636f 7773 6172 6574 6865 6265 7374 fa38  cowsarethebest.8
-000006f0: 6469 643a 6b65 793a 7a36 4d6b 656b 7743  did:key:z6MkekwC
-00000700: 3652 3962 6a39 4572 546f 4237 4169 5a4a  6R9bj9ErToB7AiZJ
-00000710: 6679 4353 4468 615a 6531 5578 6844 6243  fyCSDhaZe1UxhDbC
-00000720: 714a 7268 7170 5335 a901 fa02 3d3d a901  qJrhqpS5....==..
-00000730: 7a12 2528 7079 3029 7320 3d3d 2025 2870  z.%(py0)s == %(p
-00000740: 7933 2973 da07 6469 645f 6b65 79a9 0272  y3)s..did_key..r
-00000750: 0c00 0000 da03 7079 33fa 0e61 7373 6572  ......py3..asser
-00000760: 7420 2528 7079 3529 73da 0370 7935 2909  t %(py5)s..py5).
-00000770: 7208 0000 0072 1400 0000 da11 5f63 616c  r....r......_cal
-00000780: 6c5f 7265 7072 636f 6d70 6172 6572 1200  l_reprcomparer..
-00000790: 0000 7213 0000 0072 1500 0000 7216 0000  ..r....r....r...
-000007a0: 0072 1700 0000 7218 0000 0029 0672 1000  .r....r....).r..
-000007b0: 0000 7225 0000 00da 0b40 7079 5f61 7373  ..r%.....@py_ass
-000007c0: 6572 7432 721a 0000 00da 0b40 7079 5f66  ert2r......@py_f
-000007d0: 6f72 6d61 7434 da0b 4070 795f 666f 726d  ormat4..@py_form
-000007e0: 6174 3672 1e00 0000 721e 0000 0072 1f00  at6r....r....r..
-000007f0: 0000 da1b 7465 7374 5f70 7269 7661 7465  ....test_private
-00000800: 5f6b 6579 5f74 6f5f 6469 645f 6b65 7916  _key_to_did_key.
-00000810: 0000 0073 0600 0000 0401 0802 7c02 722e  ...s........|.r.
-00000820: 0000 007a 2662 6f76 696e 652e 7574 696c  ...z&bovine.util
-00000830: 732e 6461 7465 2e63 6865 636b 5f6d 6178  s.date.check_max
-00000840: 5f6f 6666 7365 745f 6e6f 7763 0100 0000  _offset_nowc....
-00000850: 0000 0000 0000 0000 0700 0000 0800 0000  ................
-00000860: c300 0000 73ac 0000 0081 0164 017c 005f  ....s......d.|._
-00000870: 0074 0164 0264 0364 0464 0564 0664 0764  .t.d.d.d.d.d.d.d
-00000880: 089c 0464 098d 037d 0174 027c 0164 0583  ...d...}.t.|.d..
-00000890: 0249 0064 0048 007d 0264 0a7d 037c 027c  .I.d.H.}.d.}.|.|
-000008a0: 036b 027d 047c 0473 5074 03a0 0464 0b7c  .k.}.|.sPt...d.|
-000008b0: 0466 0164 0c7c 027c 0366 02a1 0464 0d74  .f.d.|.|.f...d.t
-000008c0: 05a0 06a1 0076 0073 3574 03a0 077c 02a1  .....v.s5t...|..
-000008d0: 0172 3a74 03a0 087c 02a1 016e 0164 0d74  .r:t...|...n.d.t
-000008e0: 03a0 087c 03a1 0164 0e9c 0216 007d 0564  ...|...d.....}.d
-000008f0: 0f64 107c 0569 0116 007d 0674 0974 03a0  .d.|.i...}.t.t..
-00000900: 0a7c 06a1 0183 0182 0164 0004 007d 047d  .|.......d...}.}
-00000910: 0364 0053 0029 114e 54da 0367 6574 fa11  .d.S.).NT..get..
-00000920: 2f70 6174 682f 746f 2f72 6573 6f75 7263  /path/to/resourc
-00000930: 65fa 1d57 6564 2c20 3135 204d 6172 2032  e..Wed, 15 Mar 2
-00000940: 3032 3320 3137 3a32 383a 3135 2047 4d54  023 17:28:15 GMT
-00000950: fa0a 6d79 686f 7374 2e74 6c64 fa43 4d6f  ..myhost.tld.CMo
-00000960: 6f2d 4175 7468 2d31 2064 6964 3a6b 6579  o-Auth-1 did:key
-00000970: 3a7a 364d 6b65 6b77 4336 5239 626a 3945  :z6MkekwC6R9bj9E
-00000980: 7254 6f42 3741 695a 4a66 7943 5344 6861  rToB7AiZJfyCSDha
-00000990: 5a65 3155 7868 4462 4371 4a72 6871 7053  Ze1UxhDbCqJrhqpS
-000009a0: 355a 597a 3561 6864 4843 6250 3961 4a45  5ZYz5ahdHCbP9aJE
-000009b0: 7344 7476 4731 4d45 5a70 7850 7a75 7647  sDtvG1MEZpxPzuvG
-000009c0: 4b59 6364 5864 4b76 4d71 3559 4c32 315a  KYcdXdKvMq5YL21Z
-000009d0: 3275 6d78 6a73 3153 6f70 4359 3241 7038  2umxjs1SopCY2Ap8
-000009e0: 765a 7856 6a54 4566 3664 5962 4775 4237  vZxVjTEf6dYbGuB7
-000009f0: 6d74 6763 6755 794e 6442 4c65 2904 da04  mtgcgUyNdBLe)...
-00000a00: 6461 7465 da04 686f 7374 da0d 6175 7468  date..host..auth
-00000a10: 6f72 697a 6174 696f 6efa 0f78 2d6d 6f6f  orization..x-moo
-00000a20: 2d73 6967 6e61 7475 7265 2903 da06 6d65  -signature)...me
-00000a30: 7468 6f64 da04 7061 7468 da07 6865 6164  thod..path..head
-00000a40: 6572 7372 2100 0000 7222 0000 0072 2400  ersr!...r"...r$.
-00000a50: 0000 da06 7265 7375 6c74 7226 0000 0072  ....resultr&...r
-00000a60: 2800 0000 7229 0000 0029 0bda 0c72 6574  (...r)...)...ret
-00000a70: 7572 6e5f 7661 6c75 6572 0300 0000 7209  urn_valuer....r.
-00000a80: 0000 0072 1400 0000 722a 0000 0072 1200  ...r....r*...r..
-00000a90: 0000 7213 0000 0072 1500 0000 7216 0000  ..r....r....r...
-00000aa0: 0072 1700 0000 7218 0000 00a9 07da 0b6d  .r....r........m
-00000ab0: 6f63 6b5f 6f66 6673 6574 da07 7265 7175  ock_offset..requ
-00000ac0: 6573 7472 3b00 0000 722b 0000 0072 1a00  estr;...r+...r..
-00000ad0: 0000 722c 0000 0072 2d00 0000 721e 0000  ..r,...r-...r...
-00000ae0: 0072 1e00 0000 721f 0000 00da 2474 6573  .r....r.....$tes
-00000af0: 745f 7661 6c69 6461 7465 5f6d 6f6f 5f61  t_validate_moo_a
-00000b00: 7574 685f 7369 676e 6174 7572 655f 6765  uth_signature_ge
-00000b10: 741e 0000 0073 1a00 0000 0280 0604 0202  t....s..........
-00000b20: 0201 0201 0202 0201 0201 0201 04fc 06fd  ................
-00000b30: 100b 7c02 7240 0000 0063 0100 0000 0000  ..|.r@...c......
-00000b40: 0000 0000 0000 0700 0000 0900 0000 c300  ................
-00000b50: 0000 73b6 0000 0081 0164 017c 005f 0074  ..s......d.|._.t
-00000b60: 0164 0264 0364 0464 0564 0664 0764 0864  .d.d.d.d.d.d.d.d
-00000b70: 099c 0574 0264 0a64 0b8d 0164 0c8d 047d  ...t.d.d...d...}
-00000b80: 0174 037c 0164 0583 0249 0064 0048 007d  .t.|.d...I.d.H.}
-00000b90: 0264 0d7d 037c 027c 036b 027d 047c 0473  .d.}.|.|.k.}.|.s
-00000ba0: 5574 04a0 0564 0e7c 0466 0164 0f7c 027c  Ut...d.|.f.d.|.|
-00000bb0: 0366 02a1 0464 1074 06a0 07a1 0076 0073  .f...d.t.....v.s
-00000bc0: 3a74 04a0 087c 02a1 0172 3f74 04a0 097c  :t...|...r?t...|
-00000bd0: 02a1 016e 0164 1074 04a0 097c 03a1 0164  ...n.d.t...|...d
-00000be0: 119c 0216 007d 0564 1264 137c 0569 0116  .....}.d.d.|.i..
-00000bf0: 007d 0674 0a74 04a0 0b7c 06a1 0183 0182  .}.t.t...|......
-00000c00: 0164 0004 007d 047d 0364 0053 0029 144e  .d...}.}.d.S.).N
-00000c10: 54da 0470 6f73 7472 3000 0000 7231 0000  T..postr0...r1..
-00000c20: 0072 3200 0000 7233 0000 00fa 3473 6861  .r2...r3....4sha
-00000c30: 2d32 3536 3d4d 494c 6235 6c55 4444 365a  -256=MILb5lUDD6Z
-00000c40: 3070 4453 7868 6778 6a2b 684d 4245 7730  0pDSxhgxj+hMBEw0
-00000c50: 7554 7a50 3367 3271 554a 4748 4d70 396b  uTzP3g2qUJGHMp9k
-00000c60: 3d5a 597a 3476 506b 4a61 6f61 5356 5170  =ZYz4vPkJaoaSVQp
-00000c70: 3544 724d 6238 4576 4361 6a4a 6365 7257  5DrMb8EvCajJcerW
-00000c80: 3336 7273 7957 4445 4c54 5751 3363 596d  36rsyWDELTWQ3cYm
-00000c90: 616f 6e6e 4766 6238 5748 6977 4835 3442  aonnGfb8WHiwH54B
-00000ca0: 5368 6964 4363 6d70 6f79 486a 616e 5652  ShidCcmpoyHjanVR
-00000cb0: 594e 7258 5858 6b61 346a 416e 2905 7234  YNrXXXka4jAn).r4
-00000cc0: 0000 0072 3500 0000 7236 0000 00da 0664  ...r5...r6.....d
-00000cd0: 6967 6573 7472 3700 0000 fa10 7b22 636f  igestr7.....{"co
-00000ce0: 7773 223a 2022 676f 6f64 227d a901 723c  ws": "good"}..r<
-00000cf0: 0000 0029 0472 3800 0000 7239 0000 0072  ...).r8...r9...r
-00000d00: 3a00 0000 da08 6765 745f 6461 7461 7221  :.....get_datar!
-00000d10: 0000 0072 2200 0000 7224 0000 0072 3b00  ...r"...r$...r;.
-00000d20: 0000 7226 0000 0072 2800 0000 7229 0000  ..r&...r(...r)..
-00000d30: 0029 0c72 3c00 0000 7203 0000 0072 0200  .).r<...r....r..
-00000d40: 0000 7209 0000 0072 1400 0000 722a 0000  ..r....r....r*..
-00000d50: 0072 1200 0000 7213 0000 0072 1500 0000  .r....r....r....
-00000d60: 7216 0000 0072 1700 0000 7218 0000 0072  r....r....r....r
-00000d70: 3d00 0000 721e 0000 0072 1e00 0000 721f  =...r....r....r.
-00000d80: 0000 00da 2574 6573 745f 7661 6c69 6461  ....%test_valida
-00000d90: 7465 5f6d 6f6f 5f61 7574 685f 7369 676e  te_moo_auth_sign
-00000da0: 6174 7572 655f 706f 7374 3400 0000 731e  ature_post4...s.
-00000db0: 0000 0002 8006 0402 0202 0102 0102 0202  ................
-00000dc0: 0102 0102 0102 0104 fb08 0706 f610 0d7c  ...............|
-00000dd0: 0272 4700 0000 6301 0000 0000 0000 0000  .rG...c.........
-00000de0: 0000 0006 0000 0008 0000 00c3 0000 0073  ...............s
-00000df0: 6a00 0000 8101 6401 6402 8400 7d01 6403  j.....d.d...}.d.
-00000e00: 7c00 5f00 7401 7c01 8301 7d02 7402 6404  |._.t.|...}.t.d.
-00000e10: 6405 6406 6407 6408 6409 640a 9c03 640b  d.d.d.d.d.d...d.
-00000e20: 8d04 7d03 7c02 7c03 8301 4900 6400 4800  ..}.|.|...I.d.H.
-00000e30: 7d04 7c04 7331 640c 640d 7403 a004 7c04  }.|.s1d.d.t...|.
-00000e40: a101 6901 1600 7d05 7405 7403 a006 7c05  ..i...}.t.t...|.
-00000e50: a101 8301 8201 6400 7d04 6400 5300 290e  ......d.}.d.S.).
-00000e60: 4e63 0100 0000 0000 0000 0000 0000 0100  Nc..............
-00000e70: 0000 0200 0000 d300 0000 f30a 0000 0081  ................
-00000e80: 0174 0064 0166 0253 00a9 024e da05 6f77  .t.d.f.S...N..ow
-00000e90: 6e65 7272 0a00 0000 a901 da03 7572 6c72  nerr........urlr
-00000ea0: 1e00 0000 721e 0000 0072 1f00 0000 da0d  ....r....r......
-00000eb0: 6b65 795f 7265 7472 6965 7665 724e 0000  key_retrieverN..
-00000ec0: 00f3 0400 0000 0280 0801 7a39 7465 7374  ..........z9test
-00000ed0: 5f62 7569 6c64 5f76 616c 6964 6174 655f  _build_validate_
-00000ee0: 6874 7470 5f73 6967 6e61 7475 7265 2e3c  http_signature.<
-00000ef0: 6c6f 6361 6c73 3e2e 6b65 795f 7265 7472  locals>.key_retr
-00000f00: 6965 7665 7254 722f 0000 0072 3000 0000  ieverTr/...r0...
-00000f10: fa23 6874 7470 733a 2f2f 6d79 686f 7374  .#https://myhost
-00000f20: 2e74 6c64 2f70 6174 682f 746f 2f72 6573  .tld/path/to/res
-00000f30: 6f75 7263 6572 3100 0000 7232 0000 0061  ourcer1...r2...a
-00000f40: af01 0000 6b65 7949 643d 226b 6579 5f69  ....keyId="key_i
-00000f50: 6422 2c61 6c67 6f72 6974 686d 3d22 7273  d",algorithm="rs
-00000f60: 612d 7368 6132 3536 222c 6865 6164 6572  a-sha256",header
-00000f70: 733d 2228 7265 7175 6573 742d 7461 7267  s="(request-targ
-00000f80: 6574 2920 686f 7374 2064 6174 6522 2c73  et) host date",s
-00000f90: 6967 6e61 7475 7265 3d22 6277 6741 3355  ignature="bwgA3U
-00000fa0: 616a 7044 7a4d 3037 774d 2b4d 556b 7047  ajpDzM07wM+MUkpG
-00000fb0: 4853 2f6d 4168 6854 752b 5744 6942 4c31  HS/mAhhTu+WDiBL1
-00000fc0: 4832 384a 3736 326a 5555 7567 677a 5038  H28J762jUUuggzP8
-00000fd0: 5765 352b 4930 5748 7970 5342 4357 7438  We5+I0WHypSBCWt8
-00000fe0: 4c61 7032 4162 5971 4736 5066 5473 6446  Lap2AbYqG6PfTsdF
-00000ff0: 4562 6b38 5657 6577 5833 346e 372f 4c55  Ebk8VWewX34n7/LU
-00001000: 534d 2f57 4a65 4138 4146 4345 6e48 5950  SM/WJeA8AFCEnHYP
-00001010: 6438 7252 6962 3464 302b 6b51 562b 5534  d8rRib4d0+kQV+U4
-00001020: 4169 3939 3758 5578 7332 7869 3241 7275  Ai997XUxs2xi2Aru
-00001030: 4e64 6b42 3653 4e4d 6b53 626e 514c 6f42  NdkB6SNMkSbnQLoB
-00001040: 6a59 5434 747a 4761 6632 4931 785a 7571  jYT4tzGaf2I1xZuq
-00001050: 6a44 3148 7676 5730 7861 316f 2f6e 5074  jD1HvvW0xa1o/nPt
-00001060: 3447 356b 6a30 7456 6d67 4472 7267 654b  4G5kj0tVmgDrrgeK
-00001070: 4c32 6855 4a32 3155 6448 6358 444e 4677  L2hUJ21UdHcXDNFw
-00001080: 3951 4a57 662f 4f36 4b79 456d 6275 6d76  9QJWf/O6KyEmbumv
-00001090: 7070 4b47 4655 6664 704b 5368 336e 322f  ppKGFUfdpKSh3n2/
-000010a0: 6650 374f 3442 7871 6164 4362 4d59 6a30  fP7O4BxqadCbMYj0
-000010b0: 6f44 444f 4631 4833 5061 3647 5639 4566  oDDOF1H3Pa6GV9Ef
-000010c0: 4965 5358 584c 5339 5466 7950 706b 5877  IeSXXLS9TfyPpkXw
-000010d0: 6257 724e 707a 5542 5a51 3268 5247 7a58  bWrNpzUBZQ2hRGzX
-000010e0: 326a 532f 4a45 6870 534e 5356 7176 3641  2jS/JEhpSNSVqv6A
-000010f0: 3d3d 2229 0372 3400 0000 7235 0000 00da  ==").r4...r5....
-00001100: 0973 6967 6e61 7475 7265 2904 7238 0000  .signature).r8..
-00001110: 0072 3900 0000 724c 0000 0072 3a00 0000  .r9...rL...r:...
-00001120: fa0e 6173 7365 7274 2025 2870 7931 2973  ..assert %(py1)s
-00001130: da03 7079 3129 0772 3c00 0000 7206 0000  ..py1).r<...r...
-00001140: 0072 0300 0000 7214 0000 0072 1600 0000  .r....r....r....
-00001150: 7217 0000 0072 1800 0000 a906 723e 0000  r....r......r>..
-00001160: 0072 4d00 0000 5a17 7661 6c69 6461 7465  .rM...Z.validate
-00001170: 5f68 7474 705f 7369 676e 6174 7572 6572  _http_signaturer
-00001180: 3f00 0000 da0b 4070 795f 6173 7365 7274  ?.....@py_assert
-00001190: 305a 0b40 7079 5f66 6f72 6d61 7432 721e  0Z.@py_format2r.
-000011a0: 0000 0072 1e00 0000 721f 0000 00da 2274  ...r....r....."t
-000011b0: 6573 745f 6275 696c 645f 7661 6c69 6461  est_build_valida
-000011c0: 7465 5f68 7474 705f 7369 676e 6174 7572  te_http_signatur
-000011d0: 654c 0000 0073 1c00 0000 0280 0802 0603  eL...s..........
-000011e0: 0802 0202 0201 0201 0201 0202 0201 0201  ................
-000011f0: 04fd 06fc 3a0b 7255 0000 0063 0100 0000  ....:.rU...c....
-00001200: 0000 0000 0000 0000 0600 0000 0900 0000  ................
-00001210: c300 0000 7374 0000 0081 0164 0164 0284  ....st.....d.d..
-00001220: 007d 0164 037c 005f 0074 017c 0183 017d  .}.d.|._.t.|...}
-00001230: 0274 0264 0464 0564 0664 0764 0864 0964  .t.d.d.d.d.d.d.d
-00001240: 0a64 0b9c 0474 0364 0c64 0d8d 0164 0e8d  .d...t.d.d...d..
-00001250: 057d 037c 027c 0383 0149 0064 0048 007d  .}.|.|...I.d.H.}
-00001260: 047c 0473 3664 0f64 1074 04a0 057c 04a1  .|.s6d.d.t...|..
-00001270: 0169 0116 007d 0574 0674 04a0 077c 05a1  .i...}.t.t...|..
-00001280: 0183 0182 0164 007d 0464 0053 0029 114e  .....d.}.d.S.).N
-00001290: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-000012a0: 0002 0000 00d3 0000 0072 4800 0000 7249  .........rH...rI
-000012b0: 0000 0072 0a00 0000 724b 0000 0072 1e00  ...r....rK...r..
-000012c0: 0000 721e 0000 0072 1f00 0000 724d 0000  ..r....r....rM..
-000012d0: 0065 0000 0072 4e00 0000 7a3e 7465 7374  .e...rN...z>test
-000012e0: 5f62 7569 6c64 5f76 616c 6964 6174 655f  _build_validate_
-000012f0: 6874 7470 5f73 6967 6e61 7475 7265 5f70  http_signature_p
-00001300: 6f73 742e 3c6c 6f63 616c 733e 2e6b 6579  ost.<locals>.key
-00001310: 5f72 6574 7269 6576 6572 5472 4100 0000  _retrieverTrA...
-00001320: 7230 0000 0072 4f00 0000 7231 0000 0072  r0...rO...r1...r
-00001330: 3200 0000 7242 0000 0061 b601 0000 6b65  2...rB...a....ke
-00001340: 7949 643d 226b 6579 5f69 6422 2c61 6c67  yId="key_id",alg
-00001350: 6f72 6974 686d 3d22 7273 612d 7368 6132  orithm="rsa-sha2
-00001360: 3536 222c 6865 6164 6572 733d 2228 7265  56",headers="(re
-00001370: 7175 6573 742d 7461 7267 6574 2920 686f  quest-target) ho
-00001380: 7374 2064 6174 6520 6469 6765 7374 222c  st date digest",
-00001390: 7369 676e 6174 7572 653d 2251 7065 4c4d  signature="QpeLM
-000013a0: 4568 2f5a 3030 3944 6759 6353 4f6b 7273  Eh/Z009DgYcSOkrs
-000013b0: 4b72 397a 5737 5775 3755 5754 5133 3938  Kr9zW7Wu7UWTQ398
-000013c0: 7176 7565 437a 6145 4c2f 4878 7276 3943  qvueCzaEL/Hxrv9C
-000013d0: 3432 552b 5759 2f4f 3334 782f 3338 356c  42U+WY/O34x/385l
-000013e0: 542b 7a31 4933 426b 3671 4d5a 5444 415a  T+z1I3Bk6qMZTDAZ
-000013f0: 536d 4b47 5942 356c 5a4a 5642 6443 3230  SmKGYB5lZJVBdC20
-00001400: 6134 442b 2b48 7a49 7945 3632 6436 4376  a4D++HzIyE62d6Cv
-00001410: 7155 7351 7749 7634 6f64 2f68 4f6d 6d4f  qUsQwIv4od/hOmmO
-00001420: 5133 484b 4936 394d 554f 734e 724c 796a  Q3HKI69MUOsNrLyj
-00001430: 4951 7855 614c 5342 7a31 6d2f 776b 4c76  IQxUaLSBz1m/wkLv
-00001440: 3869 4d72 6839 5177 554c 6c71 544f 3857  8iMrh9QwULlqTO8W
-00001450: 4856 6a53 4a6c 6756 776c 6c52 744f 4f63  HVjSJlgVwllRtOOc
-00001460: 6d33 777a 6f2f 6372 3258 7946 6a34 6742  m3wzo/cr2XyFj4gB
-00001470: 3843 5564 3361 4733 6471 7a43 664f 4f6f  8CUd3aG3dqzCfOOo
-00001480: 4e51 7655 684d 446c 7850 3755 7142 6e47  NQvUhMDlxP7UqBnG
-00001490: 6f46 3670 6e59 6e54 6e4a 5553 5348 6463  oF6pnYnTnJUSSHdc
-000014a0: 6557 6245 3039 5471 584c 6d41 487a 6175  eWbE09TqXLmAHzau
-000014b0: 5947 5364 6148 5253 3358 522f 536a 6537  YGSdaHRS3XR/Sje7
-000014c0: 4554 3955 614f 6748 4863 504a 4849 4e2b  ET9UaOgHHcPJHIN+
-000014d0: 346a 7242 7044 7032 474d 3639 6a6f 5857  4jrBpDp2GM69joXW
-000014e0: 6b5a 7768 4530 474f 6c39 7133 4b42 534b  kZwhE0GOl9q3KBSK
-000014f0: 413d 3d22 2904 7234 0000 0072 3500 0000  A==").r4...r5...
-00001500: 7243 0000 0072 5000 0000 7244 0000 0072  rC...rP...rD...r
-00001510: 4500 0000 2905 7238 0000 0072 3900 0000  E...).r8...r9...
-00001520: 724c 0000 0072 3a00 0000 7246 0000 0072  rL...r:...rF...r
-00001530: 5100 0000 7252 0000 0029 0872 3c00 0000  Q...rR...).r<...
-00001540: 7206 0000 0072 0300 0000 7202 0000 0072  r....r....r....r
-00001550: 1400 0000 7216 0000 0072 1700 0000 7218  ....r....r....r.
-00001560: 0000 0072 5300 0000 721e 0000 0072 1e00  ...rS...r....r..
-00001570: 0000 721f 0000 00da 2774 6573 745f 6275  ..r.....'test_bu
-00001580: 696c 645f 7661 6c69 6461 7465 5f68 7474  ild_validate_htt
-00001590: 705f 7369 676e 6174 7572 655f 706f 7374  p_signature_post
-000015a0: 6300 0000 7320 0000 0002 8008 0206 0308  c...s ..........
-000015b0: 0202 0202 0102 0102 0102 0202 0102 0102  ................
-000015c0: 0104 fc08 0606 f63a 0d72 5600 0000 2917  .......:.rV...).
-000015d0: da08 6275 696c 7469 6e73 7212 0000 00da  ..builtinsr.....
-000015e0: 195f 7079 7465 7374 2e61 7373 6572 7469  ._pytest.asserti
-000015f0: 6f6e 2e72 6577 7269 7465 da09 6173 7365  on.rewrite..asse
-00001600: 7274 696f 6eda 0772 6577 7269 7465 7214  rtion..rewriter.
-00001610: 0000 00da 0d75 6e69 7474 6573 742e 6d6f  .....unittest.mo
-00001620: 636b 7202 0000 0072 0300 0000 7204 0000  ckr....r....r...
-00001630: 00da 0072 0600 0000 7207 0000 0072 0800  ...r....r....r..
-00001640: 0000 7209 0000 00da 0474 6573 7472 0b00  ..r......testr..
-00001650: 0000 7220 0000 0072 2e00 0000 7240 0000  ..r ...r....r@..
-00001660: 0072 4700 0000 7255 0000 0072 5600 0000  .rG...rU...rV...
-00001670: 721e 0000 0072 1e00 0000 721e 0000 0072  r....r....r....r
-00001680: 1f00 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
-00001690: 0000 731a 0000 002e 0018 020c 0608 0308  ..s.............
-000016a0: 0a06 080a 0106 150a 0106 170a 0106 160e  ................
-000016b0: 01                                       .
+000005a0: 2e6f 7267 2f62 6f76 696e 652f 626f 7669  .org/bovine/bovi
+000005b0: 6e65 2f62 6f76 696e 652f 626f 7669 6e65  ne/bovine/bovine
+000005c0: 2f63 7279 7074 6f2f 7465 7374 5f63 7279  /crypto/test_cry
+000005d0: 7074 6f2e 7079 da24 7465 7374 5f67 656e  pto.py.$test_gen
+000005e0: 6572 6174 655f 7273 615f 7075 626c 6963  erate_rsa_public
+000005f0: 5f70 7269 7661 7465 5f6b 6579 0c00 0000  _private_key....
+00000600: 730a 0000 000a 0174 0274 0174 0278 0172  s......t.t.t.x.r
+00000610: 2000 0000 6300 0000 0000 0000 0000 0000   ...c...........
+00000620: 0006 0000 0007 0000 0043 0000 0073 8800  .........C...s..
+00000630: 0000 6401 7d00 7400 7c00 8301 7d01 6402  ..d.}.t.|...}.d.
+00000640: 7d02 7c01 7c02 6b02 7d03 7c03 733e 7401  }.|.|.k.}.|.s>t.
+00000650: a002 6403 7c03 6601 6404 7c01 7c02 6602  ..d.|.f.d.|.|.f.
+00000660: a104 6405 7403 a004 a100 7600 7323 7401  ..d.t.....v.s#t.
+00000670: a005 7c01 a101 7228 7401 a006 7c01 a101  ..|...r(t...|...
+00000680: 6e01 6405 7401 a006 7c02 a101 6406 9c02  n.d.t...|...d...
+00000690: 1600 7d04 6407 6408 7c04 6901 1600 7d05  ..}.d.d.|.i...}.
+000006a0: 7407 7401 a008 7c05 a101 8301 8201 6400  t.t...|.......d.
+000006b0: 0400 7d03 7d02 6400 5300 2909 4e5a 307a  ..}.}.d.S.).NZ0z
+000006c0: 3375 3259 7863 6f77 7361 7265 7468 6562  3u2Yxcowsaretheb
+000006d0: 6573 7463 6f77 7361 7265 7468 6562 6573  estcowsarethebes
+000006e0: 7463 6f77 7361 7265 7468 6562 6573 74fa  tcowsarethebest.
+000006f0: 3864 6964 3a6b 6579 3a7a 364d 6b65 6b77  8did:key:z6Mkekw
+00000700: 4336 5239 626a 3945 7254 6f42 3741 695a  C6R9bj9ErToB7AiZ
+00000710: 4a66 7943 5344 6861 5a65 3155 7868 4462  JfyCSDhaZe1UxhDb
+00000720: 4371 4a72 6871 7053 35a9 01fa 023d 3da9  CqJrhqpS5....==.
+00000730: 017a 1225 2870 7930 2973 203d 3d20 2528  .z.%(py0)s == %(
+00000740: 7079 3329 73da 0764 6964 5f6b 6579 a902  py3)s..did_key..
+00000750: 720c 0000 00da 0370 7933 fa0e 6173 7365  r......py3..asse
+00000760: 7274 2025 2870 7935 2973 da03 7079 3529  rt %(py5)s..py5)
+00000770: 0972 0800 0000 7214 0000 00da 115f 6361  .r....r......_ca
+00000780: 6c6c 5f72 6570 7263 6f6d 7061 7265 7212  ll_reprcomparer.
+00000790: 0000 0072 1300 0000 7215 0000 0072 1600  ...r....r....r..
+000007a0: 0000 7217 0000 0072 1800 0000 2906 7210  ..r....r....).r.
+000007b0: 0000 0072 2500 0000 da0b 4070 795f 6173  ...r%.....@py_as
+000007c0: 7365 7274 3272 1a00 0000 da0b 4070 795f  sert2r......@py_
+000007d0: 666f 726d 6174 34da 0b40 7079 5f66 6f72  format4..@py_for
+000007e0: 6d61 7436 721e 0000 0072 1e00 0000 721f  mat6r....r....r.
+000007f0: 0000 00da 1b74 6573 745f 7072 6976 6174  .....test_privat
+00000800: 655f 6b65 795f 746f 5f64 6964 5f6b 6579  e_key_to_did_key
+00000810: 1600 0000 7306 0000 0004 0108 027c 0272  ....s........|.r
+00000820: 2e00 0000 7a26 626f 7669 6e65 2e75 7469  ....z&bovine.uti
+00000830: 6c73 2e64 6174 652e 6368 6563 6b5f 6d61  ls.date.check_ma
+00000840: 785f 6f66 6673 6574 5f6e 6f77 6301 0000  x_offset_nowc...
+00000850: 0000 0000 0000 0000 0007 0000 0008 0000  ................
+00000860: 00c3 0000 0073 ac00 0000 8101 6401 7c00  .....s......d.|.
+00000870: 5f00 7401 6402 6403 6404 6405 6406 6407  _.t.d.d.d.d.d.d.
+00000880: 6408 9c04 6409 8d03 7d01 7402 7c01 6405  d...d...}.t.|.d.
+00000890: 8302 4900 6400 4800 7d02 640a 7d03 7c02  ..I.d.H.}.d.}.|.
+000008a0: 7c03 6b02 7d04 7c04 7350 7403 a004 640b  |.k.}.|.sPt...d.
+000008b0: 7c04 6601 640c 7c02 7c03 6602 a104 640d  |.f.d.|.|.f...d.
+000008c0: 7405 a006 a100 7600 7335 7403 a007 7c02  t.....v.s5t...|.
+000008d0: a101 723a 7403 a008 7c02 a101 6e01 640d  ..r:t...|...n.d.
+000008e0: 7403 a008 7c03 a101 640e 9c02 1600 7d05  t...|...d.....}.
+000008f0: 640f 6410 7c05 6901 1600 7d06 7409 7403  d.d.|.i...}.t.t.
+00000900: a00a 7c06 a101 8301 8201 6400 0400 7d04  ..|.......d...}.
+00000910: 7d03 6400 5300 2911 4e54 da03 6765 74fa  }.d.S.).NT..get.
+00000920: 112f 7061 7468 2f74 6f2f 7265 736f 7572  ./path/to/resour
+00000930: 6365 fa1d 5765 642c 2031 3520 4d61 7220  ce..Wed, 15 Mar 
+00000940: 3230 3233 2031 373a 3238 3a31 3520 474d  2023 17:28:15 GM
+00000950: 54fa 0a6d 7968 6f73 742e 746c 64fa 434d  T..myhost.tld.CM
+00000960: 6f6f 2d41 7574 682d 3120 6469 643a 6b65  oo-Auth-1 did:ke
+00000970: 793a 7a36 4d6b 656b 7743 3652 3962 6a39  y:z6MkekwC6R9bj9
+00000980: 4572 546f 4237 4169 5a4a 6679 4353 4468  ErToB7AiZJfyCSDh
+00000990: 615a 6531 5578 6844 6243 714a 7268 7170  aZe1UxhDbCqJrhqp
+000009a0: 5335 5a59 7a35 6168 6448 4362 5039 614a  S5ZYz5ahdHCbP9aJ
+000009b0: 4573 4474 7647 314d 455a 7078 507a 7576  EsDtvG1MEZpxPzuv
+000009c0: 474b 5963 6458 644b 764d 7135 594c 3231  GKYcdXdKvMq5YL21
+000009d0: 5a32 756d 786a 7331 536f 7043 5932 4170  Z2umxjs1SopCY2Ap
+000009e0: 3876 5a78 566a 5445 6636 6459 6247 7542  8vZxVjTEf6dYbGuB
+000009f0: 376d 7467 6367 5579 4e64 424c 6529 04da  7mtgcgUyNdBLe)..
+00000a00: 0464 6174 65da 0468 6f73 74da 0d61 7574  .date..host..aut
+00000a10: 686f 7269 7a61 7469 6f6e fa0f 782d 6d6f  horization..x-mo
+00000a20: 6f2d 7369 676e 6174 7572 6529 03da 066d  o-signature)...m
+00000a30: 6574 686f 64da 0470 6174 68da 0768 6561  ethod..path..hea
+00000a40: 6465 7273 7221 0000 0072 2200 0000 7224  dersr!...r"...r$
+00000a50: 0000 00da 0672 6573 756c 7472 2600 0000  .....resultr&...
+00000a60: 7228 0000 0072 2900 0000 290b da0c 7265  r(...r)...)...re
+00000a70: 7475 726e 5f76 616c 7565 7203 0000 0072  turn_valuer....r
+00000a80: 0900 0000 7214 0000 0072 2a00 0000 7212  ....r....r*...r.
+00000a90: 0000 0072 1300 0000 7215 0000 0072 1600  ...r....r....r..
+00000aa0: 0000 7217 0000 0072 1800 0000 a907 da0b  ..r....r........
+00000ab0: 6d6f 636b 5f6f 6666 7365 74da 0772 6571  mock_offset..req
+00000ac0: 7565 7374 723b 0000 0072 2b00 0000 721a  uestr;...r+...r.
+00000ad0: 0000 0072 2c00 0000 722d 0000 0072 1e00  ...r,...r-...r..
+00000ae0: 0000 721e 0000 0072 1f00 0000 da24 7465  ..r....r.....$te
+00000af0: 7374 5f76 616c 6964 6174 655f 6d6f 6f5f  st_validate_moo_
+00000b00: 6175 7468 5f73 6967 6e61 7475 7265 5f67  auth_signature_g
+00000b10: 6574 1e00 0000 731a 0000 0002 8006 0402  et....s.........
+00000b20: 0202 0102 0102 0202 0102 0102 0104 fc06  ................
+00000b30: fd10 0b7c 0272 4000 0000 6301 0000 0000  ...|.r@...c.....
+00000b40: 0000 0000 0000 0007 0000 0009 0000 00c3  ................
+00000b50: 0000 0073 b600 0000 8101 6401 7c00 5f00  ...s......d.|._.
+00000b60: 7401 6402 6403 6404 6405 6406 6407 6408  t.d.d.d.d.d.d.d.
+00000b70: 6409 9c05 7402 640a 640b 8d01 640c 8d04  d...t.d.d...d...
+00000b80: 7d01 7403 7c01 6405 8302 4900 6400 4800  }.t.|.d...I.d.H.
+00000b90: 7d02 640d 7d03 7c02 7c03 6b02 7d04 7c04  }.d.}.|.|.k.}.|.
+00000ba0: 7355 7404 a005 640e 7c04 6601 640f 7c02  sUt...d.|.f.d.|.
+00000bb0: 7c03 6602 a104 6410 7406 a007 a100 7600  |.f...d.t.....v.
+00000bc0: 733a 7404 a008 7c02 a101 723f 7404 a009  s:t...|...r?t...
+00000bd0: 7c02 a101 6e01 6410 7404 a009 7c03 a101  |...n.d.t...|...
+00000be0: 6411 9c02 1600 7d05 6412 6413 7c05 6901  d.....}.d.d.|.i.
+00000bf0: 1600 7d06 740a 7404 a00b 7c06 a101 8301  ..}.t.t...|.....
+00000c00: 8201 6400 0400 7d04 7d03 6400 5300 2914  ..d...}.}.d.S.).
+00000c10: 4e54 da04 706f 7374 7230 0000 0072 3100  NT..postr0...r1.
+00000c20: 0000 7232 0000 0072 3300 0000 fa34 7368  ..r2...r3....4sh
+00000c30: 612d 3235 363d 4d49 4c62 356c 5544 4436  a-256=MILb5lUDD6
+00000c40: 5a30 7044 5378 6867 786a 2b68 4d42 4577  Z0pDSxhgxj+hMBEw
+00000c50: 3075 547a 5033 6732 7155 4a47 484d 7039  0uTzP3g2qUJGHMp9
+00000c60: 6b3d 5a59 7a34 7650 6b4a 616f 6153 5651  k=ZYz4vPkJaoaSVQ
+00000c70: 7035 4472 4d62 3845 7643 616a 4a63 6572  p5DrMb8EvCajJcer
+00000c80: 5733 3672 7379 5744 454c 5457 5133 6359  W36rsyWDELTWQ3cY
+00000c90: 6d61 6f6e 6e47 6662 3857 4869 7748 3534  maonnGfb8WHiwH54
+00000ca0: 4253 6869 6443 636d 706f 7948 6a61 6e56  BShidCcmpoyHjanV
+00000cb0: 5259 4e72 5858 586b 6134 6a41 6e29 0572  RYNrXXXka4jAn).r
+00000cc0: 3400 0000 7235 0000 0072 3600 0000 da06  4...r5...r6.....
+00000cd0: 6469 6765 7374 7237 0000 00fa 107b 2263  digestr7.....{"c
+00000ce0: 6f77 7322 3a20 2267 6f6f 6422 7da9 0172  ows": "good"}..r
+00000cf0: 3c00 0000 2904 7238 0000 0072 3900 0000  <...).r8...r9...
+00000d00: 723a 0000 00da 0867 6574 5f64 6174 6172  r:.....get_datar
+00000d10: 2100 0000 7222 0000 0072 2400 0000 723b  !...r"...r$...r;
+00000d20: 0000 0072 2600 0000 7228 0000 0072 2900  ...r&...r(...r).
+00000d30: 0000 290c 723c 0000 0072 0300 0000 7202  ..).r<...r....r.
+00000d40: 0000 0072 0900 0000 7214 0000 0072 2a00  ...r....r....r*.
+00000d50: 0000 7212 0000 0072 1300 0000 7215 0000  ..r....r....r...
+00000d60: 0072 1600 0000 7217 0000 0072 1800 0000  .r....r....r....
+00000d70: 723d 0000 0072 1e00 0000 721e 0000 0072  r=...r....r....r
+00000d80: 1f00 0000 da25 7465 7374 5f76 616c 6964  .....%test_valid
+00000d90: 6174 655f 6d6f 6f5f 6175 7468 5f73 6967  ate_moo_auth_sig
+00000da0: 6e61 7475 7265 5f70 6f73 7434 0000 0073  nature_post4...s
+00000db0: 1e00 0000 0280 0604 0202 0201 0201 0202  ................
+00000dc0: 0201 0201 0201 0201 04fb 0807 06f6 100d  ................
+00000dd0: 7c02 7247 0000 0063 0100 0000 0000 0000  |.rG...c........
+00000de0: 0000 0000 0600 0000 0800 0000 c300 0000  ................
+00000df0: 736a 0000 0081 0164 0164 0284 007d 0164  sj.....d.d...}.d
+00000e00: 037c 005f 0074 017c 0183 017d 0274 0264  .|._.t.|...}.t.d
+00000e10: 0464 0564 0664 0764 0864 0964 0a9c 0364  .d.d.d.d.d.d...d
+00000e20: 0b8d 047d 037c 027c 0383 0149 0064 0048  ...}.|.|...I.d.H
+00000e30: 007d 047c 0473 3164 0c64 0d74 03a0 047c  .}.|.s1d.d.t...|
+00000e40: 04a1 0169 0116 007d 0574 0574 03a0 067c  ...i...}.t.t...|
+00000e50: 05a1 0183 0182 0164 007d 0464 0053 0029  .......d.}.d.S.)
+00000e60: 0e4e 6301 0000 0000 0000 0000 0000 0001  .Nc.............
+00000e70: 0000 0002 0000 00d3 0000 00f3 0a00 0000  ................
+00000e80: 8101 7400 6401 6602 5300 a902 4eda 056f  ..t.d.f.S...N..o
+00000e90: 776e 6572 720a 0000 00a9 01da 0375 726c  wnerr........url
+00000ea0: 721e 0000 0072 1e00 0000 721f 0000 00da  r....r....r.....
+00000eb0: 0d6b 6579 5f72 6574 7269 6576 6572 4e00  .key_retrieverN.
+00000ec0: 0000 f304 0000 0002 8008 017a 3974 6573  ...........z9tes
+00000ed0: 745f 6275 696c 645f 7661 6c69 6461 7465  t_build_validate
+00000ee0: 5f68 7474 705f 7369 676e 6174 7572 652e  _http_signature.
+00000ef0: 3c6c 6f63 616c 733e 2e6b 6579 5f72 6574  <locals>.key_ret
+00000f00: 7269 6576 6572 5472 2f00 0000 7230 0000  rieverTr/...r0..
+00000f10: 00fa 2368 7474 7073 3a2f 2f6d 7968 6f73  ..#https://myhos
+00000f20: 742e 746c 642f 7061 7468 2f74 6f2f 7265  t.tld/path/to/re
+00000f30: 736f 7572 6365 7231 0000 0072 3200 0000  sourcer1...r2...
+00000f40: 61af 0100 006b 6579 4964 3d22 6b65 795f  a....keyId="key_
+00000f50: 6964 222c 616c 676f 7269 7468 6d3d 2272  id",algorithm="r
+00000f60: 7361 2d73 6861 3235 3622 2c68 6561 6465  sa-sha256",heade
+00000f70: 7273 3d22 2872 6571 7565 7374 2d74 6172  rs="(request-tar
+00000f80: 6765 7429 2068 6f73 7420 6461 7465 222c  get) host date",
+00000f90: 7369 676e 6174 7572 653d 2262 7767 4133  signature="bwgA3
+00000fa0: 5561 6a70 447a 4d30 3777 4d2b 4d55 6b70  UajpDzM07wM+MUkp
+00000fb0: 4748 532f 6d41 6868 5475 2b57 4469 424c  GHS/mAhhTu+WDiBL
+00000fc0: 3148 3238 4a37 3632 6a55 5575 6767 7a50  1H28J762jUUuggzP
+00000fd0: 3857 6535 2b49 3057 4879 7053 4243 5774  8We5+I0WHypSBCWt
+00000fe0: 384c 6170 3241 6259 7147 3650 6654 7364  8Lap2AbYqG6PfTsd
+00000ff0: 4645 626b 3856 5765 7758 3334 6e37 2f4c  FEbk8VWewX34n7/L
+00001000: 5553 4d2f 574a 6541 3841 4643 456e 4859  USM/WJeA8AFCEnHY
+00001010: 5064 3872 5269 6234 6430 2b6b 5156 2b55  Pd8rRib4d0+kQV+U
+00001020: 3441 6939 3937 5855 7873 3278 6932 4172  4Ai997XUxs2xi2Ar
+00001030: 754e 646b 4236 534e 4d6b 5362 6e51 4c6f  uNdkB6SNMkSbnQLo
+00001040: 426a 5954 3474 7a47 6166 3249 3178 5a75  BjYT4tzGaf2I1xZu
+00001050: 716a 4431 4876 7657 3078 6131 6f2f 6e50  qjD1HvvW0xa1o/nP
+00001060: 7434 4735 6b6a 3074 566d 6744 7272 6765  t4G5kj0tVmgDrrge
+00001070: 4b4c 3268 554a 3231 5564 4863 5844 4e46  KL2hUJ21UdHcXDNF
+00001080: 7739 514a 5766 2f4f 364b 7945 6d62 756d  w9QJWf/O6KyEmbum
+00001090: 7670 704b 4746 5566 6470 4b53 6833 6e32  vppKGFUfdpKSh3n2
+000010a0: 2f66 5037 4f34 4278 7161 6443 624d 596a  /fP7O4BxqadCbMYj
+000010b0: 306f 4444 4f46 3148 3350 6136 4756 3945  0oDDOF1H3Pa6GV9E
+000010c0: 6649 6553 5858 4c53 3954 6679 5070 6b58  fIeSXXLS9TfyPpkX
+000010d0: 7762 5772 4e70 7a55 425a 5132 6852 477a  wbWrNpzUBZQ2hRGz
+000010e0: 5832 6a53 2f4a 4568 7053 4e53 5671 7636  X2jS/JEhpSNSVqv6
+000010f0: 413d 3d22 2903 7234 0000 0072 3500 0000  A==").r4...r5...
+00001100: da09 7369 676e 6174 7572 6529 0472 3800  ..signature).r8.
+00001110: 0000 7239 0000 0072 4c00 0000 723a 0000  ..r9...rL...r:..
+00001120: 00fa 0e61 7373 6572 7420 2528 7079 3129  ...assert %(py1)
+00001130: 73da 0370 7931 2907 723c 0000 0072 0600  s..py1).r<...r..
+00001140: 0000 7203 0000 0072 1400 0000 7216 0000  ..r....r....r...
+00001150: 0072 1700 0000 7218 0000 00a9 0672 3e00  .r....r......r>.
+00001160: 0000 724d 0000 005a 1776 616c 6964 6174  ..rM...Z.validat
+00001170: 655f 6874 7470 5f73 6967 6e61 7475 7265  e_http_signature
+00001180: 723f 0000 00da 0b40 7079 5f61 7373 6572  r?.....@py_asser
+00001190: 7430 5a0b 4070 795f 666f 726d 6174 3272  t0Z.@py_format2r
+000011a0: 1e00 0000 721e 0000 0072 1f00 0000 da22  ....r....r....."
+000011b0: 7465 7374 5f62 7569 6c64 5f76 616c 6964  test_build_valid
+000011c0: 6174 655f 6874 7470 5f73 6967 6e61 7475  ate_http_signatu
+000011d0: 7265 4c00 0000 731c 0000 0002 8008 0206  reL...s.........
+000011e0: 0308 0202 0202 0102 0102 0102 0202 0102  ................
+000011f0: 0104 fd06 fc3a 0b72 5500 0000 6301 0000  .....:.rU...c...
+00001200: 0000 0000 0000 0000 0006 0000 0009 0000  ................
+00001210: 00c3 0000 0073 7400 0000 8101 6401 6402  .....st.....d.d.
+00001220: 8400 7d01 6403 7c00 5f00 7401 7c01 8301  ..}.d.|._.t.|...
+00001230: 7d02 7402 6404 6405 6406 6407 6408 6409  }.t.d.d.d.d.d.d.
+00001240: 640a 640b 9c04 7403 640c 640d 8d01 640e  d.d...t.d.d...d.
+00001250: 8d05 7d03 7c02 7c03 8301 4900 6400 4800  ..}.|.|...I.d.H.
+00001260: 7d04 7c04 7336 640f 6410 7404 a005 7c04  }.|.s6d.d.t...|.
+00001270: a101 6901 1600 7d05 7406 7404 a007 7c05  ..i...}.t.t...|.
+00001280: a101 8301 8201 6400 7d04 6400 5300 2911  ......d.}.d.S.).
+00001290: 4e63 0100 0000 0000 0000 0000 0000 0100  Nc..............
+000012a0: 0000 0200 0000 d300 0000 7248 0000 0072  ..........rH...r
+000012b0: 4900 0000 720a 0000 0072 4b00 0000 721e  I...r....rK...r.
+000012c0: 0000 0072 1e00 0000 721f 0000 0072 4d00  ...r....r....rM.
+000012d0: 0000 6500 0000 724e 0000 007a 3e74 6573  ..e...rN...z>tes
+000012e0: 745f 6275 696c 645f 7661 6c69 6461 7465  t_build_validate
+000012f0: 5f68 7474 705f 7369 676e 6174 7572 655f  _http_signature_
+00001300: 706f 7374 2e3c 6c6f 6361 6c73 3e2e 6b65  post.<locals>.ke
+00001310: 795f 7265 7472 6965 7665 7254 7241 0000  y_retrieverTrA..
+00001320: 0072 3000 0000 724f 0000 0072 3100 0000  .r0...rO...r1...
+00001330: 7232 0000 0072 4200 0000 61b6 0100 006b  r2...rB...a....k
+00001340: 6579 4964 3d22 6b65 795f 6964 222c 616c  eyId="key_id",al
+00001350: 676f 7269 7468 6d3d 2272 7361 2d73 6861  gorithm="rsa-sha
+00001360: 3235 3622 2c68 6561 6465 7273 3d22 2872  256",headers="(r
+00001370: 6571 7565 7374 2d74 6172 6765 7429 2068  equest-target) h
+00001380: 6f73 7420 6461 7465 2064 6967 6573 7422  ost date digest"
+00001390: 2c73 6967 6e61 7475 7265 3d22 5170 654c  ,signature="QpeL
+000013a0: 4d45 682f 5a30 3039 4467 5963 534f 6b72  MEh/Z009DgYcSOkr
+000013b0: 734b 7239 7a57 3757 7537 5557 5451 3339  sKr9zW7Wu7UWTQ39
+000013c0: 3871 7675 6543 7a61 454c 2f48 7872 7639  8qvueCzaEL/Hxrv9
+000013d0: 4334 3255 2b57 592f 4f33 3478 2f33 3835  C42U+WY/O34x/385
+000013e0: 6c54 2b7a 3149 3342 6b36 714d 5a54 4441  lT+z1I3Bk6qMZTDA
+000013f0: 5a53 6d4b 4759 4235 6c5a 4a56 4264 4332  ZSmKGYB5lZJVBdC2
+00001400: 3061 3444 2b2b 487a 4979 4536 3264 3643  0a4D++HzIyE62d6C
+00001410: 7671 5573 5177 4976 346f 642f 684f 6d6d  vqUsQwIv4od/hOmm
+00001420: 4f51 3348 4b49 3639 4d55 4f73 4e72 4c79  OQ3HKI69MUOsNrLy
+00001430: 6a49 5178 5561 4c53 427a 316d 2f77 6b4c  jIQxUaLSBz1m/wkL
+00001440: 7638 694d 7268 3951 7755 4c6c 7154 4f38  v8iMrh9QwULlqTO8
+00001450: 5748 566a 534a 6c67 5677 6c6c 5274 4f4f  WHVjSJlgVwllRtOO
+00001460: 636d 3377 7a6f 2f63 7232 5879 466a 3467  cm3wzo/cr2XyFj4g
+00001470: 4238 4355 6433 6147 3364 717a 4366 4f4f  B8CUd3aG3dqzCfOO
+00001480: 6f4e 5176 5568 4d44 6c78 5037 5571 426e  oNQvUhMDlxP7UqBn
+00001490: 476f 4636 706e 596e 546e 4a55 5353 4864  GoF6pnYnTnJUSSHd
+000014a0: 6365 5762 4530 3954 7158 4c6d 4148 7a61  ceWbE09TqXLmAHza
+000014b0: 7559 4753 6461 4852 5333 5852 2f53 6a65  uYGSdaHRS3XR/Sje
+000014c0: 3745 5439 5561 4f67 4848 6350 4a48 494e  7ET9UaOgHHcPJHIN
+000014d0: 2b34 6a72 4270 4470 3247 4d36 396a 6f58  +4jrBpDp2GM69joX
+000014e0: 576b 5a77 6845 3047 4f6c 3971 334b 4253  WkZwhE0GOl9q3KBS
+000014f0: 4b41 3d3d 2229 0472 3400 0000 7235 0000  KA==").r4...r5..
+00001500: 0072 4300 0000 7250 0000 0072 4400 0000  .rC...rP...rD...
+00001510: 7245 0000 0029 0572 3800 0000 7239 0000  rE...).r8...r9..
+00001520: 0072 4c00 0000 723a 0000 0072 4600 0000  .rL...r:...rF...
+00001530: 7251 0000 0072 5200 0000 2908 723c 0000  rQ...rR...).r<..
+00001540: 0072 0600 0000 7203 0000 0072 0200 0000  .r....r....r....
+00001550: 7214 0000 0072 1600 0000 7217 0000 0072  r....r....r....r
+00001560: 1800 0000 7253 0000 0072 1e00 0000 721e  ....rS...r....r.
+00001570: 0000 0072 1f00 0000 da27 7465 7374 5f62  ...r.....'test_b
+00001580: 7569 6c64 5f76 616c 6964 6174 655f 6874  uild_validate_ht
+00001590: 7470 5f73 6967 6e61 7475 7265 5f70 6f73  tp_signature_pos
+000015a0: 7463 0000 0073 2000 0000 0280 0802 0603  tc...s .........
+000015b0: 0802 0202 0201 0201 0201 0202 0201 0201  ................
+000015c0: 0201 04fc 0806 06f6 3a0d 7256 0000 0029  ........:.rV...)
+000015d0: 17da 0862 7569 6c74 696e 7372 1200 0000  ...builtinsr....
+000015e0: da19 5f70 7974 6573 742e 6173 7365 7274  .._pytest.assert
+000015f0: 696f 6e2e 7265 7772 6974 65da 0961 7373  ion.rewrite..ass
+00001600: 6572 7469 6f6e da07 7265 7772 6974 6572  ertion..rewriter
+00001610: 1400 0000 da0d 756e 6974 7465 7374 2e6d  ......unittest.m
+00001620: 6f63 6b72 0200 0000 7203 0000 0072 0400  ockr....r....r..
+00001630: 0000 da00 7206 0000 0072 0700 0000 7208  ....r....r....r.
+00001640: 0000 0072 0900 0000 da04 7465 7374 720b  ...r......testr.
+00001650: 0000 0072 2000 0000 722e 0000 0072 4000  ...r ...r....r@.
+00001660: 0000 7247 0000 0072 5500 0000 7256 0000  ..rG...rU...rV..
+00001670: 0072 1e00 0000 721e 0000 0072 1e00 0000  .r....r....r....
+00001680: 721f 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
+00001690: 0000 0073 1a00 0000 2e00 1802 0c06 0803  ...s............
+000016a0: 080a 0608 0a01 0615 0a01 0617 0a01 0616  ................
+000016b0: 0e01                                     ..
```

### Comparing `bovine-0.1.0/bovine/crypto/__pycache__/test_helper.cpython-310-pytest-7.3.0.pyc` & `bovine-0.1.1/bovine/crypto/__pycache__/test_helper.cpython-310-pytest-7.3.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 13 15:55:57 2023 UTC, .py size: 896 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0d26 3864 8003 0000  o........&8d....
+00000000: 6f0d 0d0a 0000 0000 a4ea 3a64 8003 0000  o.........:d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 7200 0000 6400  .....@...sr...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6402 6c06 6d07  ..m.Z...d.d.l.m.
 00000050: 5a07 0100 6403 6404 6c08 6d09 5a09 6d0a  Z...d.d.l.m.Z.m.
 00000060: 5a0a 6d0b 5a0b 6d0c 5a0c 0100 6403 6405  Z.m.Z.m.Z...d.d.
 00000070: 6c0d 6d0e 5a0e 6d0f 5a0f 0100 6406 6407  l.m.Z.m.Z...d.d.
@@ -43,130 +43,130 @@
 000002a0: 6d65 da09 5f73 6166 6572 6570 72da 0e41  me.._saferepr..A
 000002b0: 7373 6572 7469 6f6e 4572 726f 72da 135f  ssertionError.._
 000002c0: 666f 726d 6174 5f65 7870 6c61 6e61 7469  format_explanati
 000002d0: 6f6e 2905 720c 0000 00da 0b40 7079 5f61  on).r......@py_a
 000002e0: 7373 6572 7432 da0b 4070 795f 6173 7365  ssert2..@py_asse
 000002f0: 7274 31da 0b40 7079 5f66 6f72 6d61 7434  rt1..@py_format4
 00000300: da0b 4070 795f 666f 726d 6174 36a9 0072  ..@py_format6..r
-00000310: 1c00 0000 fa4d 2f77 6f6f 6470 6563 6b65  .....M/woodpecke
+00000310: 1c00 0000 fa4e 2f77 6f6f 6470 6563 6b65  .....N/woodpecke
 00000320: 722f 7372 632f 636f 6465 6265 7267 2e6f  r/src/codeberg.o
-00000330: 7267 2f68 656c 6765 2f62 6f76 696e 652f  rg/helge/bovine/
-00000340: 626f 7669 6e65 2f62 6f76 696e 652f 6372  bovine/bovine/cr
-00000350: 7970 746f 2f74 6573 745f 6865 6c70 6572  ypto/test_helper
-00000360: 2e70 79da 1a74 6573 745f 636f 6e74 656e  .py..test_conten
-00000370: 745f 6469 6765 7374 5f73 6861 3235 360c  t_digest_sha256.
-00000380: 0000 0073 0400 0000 0801 7c02 721e 0000  ...s......|.r...
-00000390: 0063 0000 0000 0000 0000 0000 0000 0500  .c..............
-000003a0: 0000 0800 0000 4300 0000 73ba 0000 0064  ......C...s....d
-000003b0: 017d 0074 007c 0083 017d 0174 016a 027d  .}.t.|...}.t.j.}
-000003c0: 0274 037c 017c 0283 027d 037c 0373 5764  .t.|.|...}.|.sWd
-000003d0: 0264 0374 04a0 05a1 0076 0073 1c74 06a0  .d.t.....v.s.t..
-000003e0: 0774 03a1 0172 2174 06a0 0874 03a1 016e  .t...r!t...t...n
-000003f0: 0164 0364 0474 04a0 05a1 0076 0073 2d74  .d.d.t.....v.s-t
-00000400: 06a0 077c 01a1 0172 3274 06a0 087c 01a1  ...|...r2t...|..
-00000410: 016e 0164 0464 0574 04a0 05a1 0076 0073  .n.d.d.t.....v.s
-00000420: 3e74 06a0 0774 01a1 0172 4374 06a0 0874  >t...t...rCt...t
-00000430: 01a1 016e 0164 0574 06a0 087c 02a1 0174  ...n.d.t...|...t
-00000440: 06a0 087c 03a1 0164 069c 0516 007d 0474  ...|...d.....}.t
-00000450: 0974 06a0 0a7c 04a1 0183 0182 0164 0004  .t...|.......d..
-00000460: 007d 027d 0364 0053 0029 074e 7a38 6469  .}.}.d.S.).Nz8di
-00000470: 643a 6b65 793a 7a36 4d6b 6954 427a 3179  d:key:z6MkiTBz1y
-00000480: 6d75 6570 4151 3448 4548 5953 4631 4838  muepAQ4HEHYSF1H8
-00000490: 7175 4735 474c 5656 5152 3364 6a64 5833  quG5GLVVQR3djdX3
-000004a0: 6d44 6f6f 5770 7a5b 6173 7365 7274 2025  mDooWpz[assert %
-000004b0: 2870 7936 2973 0a7b 2528 7079 3629 7320  (py6)s.{%(py6)s 
-000004c0: 3d20 2528 7079 3029 7328 2528 7079 3129  = %(py0)s(%(py1)
-000004d0: 732c 2025 2870 7934 2973 0a7b 2528 7079  s, %(py4)s.{%(py
-000004e0: 3429 7320 3d20 2528 7079 3229 732e 4564  4)s = %(py2)s.Ed
-000004f0: 3235 3531 3950 7562 6c69 634b 6579 0a7d  25519PublicKey.}
-00000500: 290a 7dda 0a69 7369 6e73 7461 6e63 6572  ).}..isinstancer
-00000510: 0900 0000 7202 0000 00a9 0572 0d00 0000  ....r......r....
-00000520: da03 7079 31da 0370 7932 da03 7079 34da  ..py1..py2..py4.
-00000530: 0370 7936 290b 7205 0000 0072 0200 0000  .py6).r....r....
-00000540: da10 4564 3235 3531 3950 7562 6c69 634b  ..Ed25519PublicK
-00000550: 6579 721f 0000 0072 1200 0000 7213 0000  eyr....r....r...
-00000560: 0072 1000 0000 7214 0000 0072 1500 0000  .r....r....r....
-00000570: 7216 0000 0072 1700 0000 2905 5a0b 6469  r....r....).Z.di
-00000580: 645f 6578 616d 706c 6572 0900 0000 da0b  d_exampler......
-00000590: 4070 795f 6173 7365 7274 33da 0b40 7079  @py_assert3..@py
-000005a0: 5f61 7373 6572 7435 da0b 4070 795f 666f  _assert5..@py_fo
-000005b0: 726d 6174 3772 1c00 0000 721c 0000 0072  rmat7r....r....r
-000005c0: 1d00 0000 da16 7465 7374 5f64 6964 5f74  ......test_did_t
-000005d0: 6f5f 7075 626c 6963 5f6b 6579 1200 0000  o_public_key....
-000005e0: 7306 0000 0004 0108 02ae 0272 2900 0000  s..........r)...
-000005f0: 6300 0000 0000 0000 0000 0000 0004 0000  c...............
-00000600: 0008 0000 0043 0000 0073 ce00 0000 6401  .....C...s....d.
-00000610: 7d00 7400 7401 7c00 8302 7d01 7402 7403  }.t.t.|...}.t.t.
-00000620: 7c00 7c01 8303 7d02 7c02 7363 6402 6403  |.|...}.|.scd.d.
-00000630: 7404 a005 a100 7600 731b 7406 a007 7402  t.....v.s.t...t.
-00000640: a101 7220 7406 a008 7402 a101 6e01 6403  ..r t...t...n.d.
-00000650: 6404 7404 a005 a100 7600 732c 7406 a007  d.t.....v.s,t...
-00000660: 7403 a101 7231 7406 a008 7403 a101 6e01  t...r1t...t...n.
-00000670: 6404 6405 7404 a005 a100 7600 733d 7406  d.d.t.....v.s=t.
-00000680: a007 7c00 a101 7242 7406 a008 7c00 a101  ..|...rBt...|...
-00000690: 6e01 6405 6406 7404 a005 a100 7600 734e  n.d.d.t.....v.sN
-000006a0: 7406 a007 7c01 a101 7253 7406 a008 7c01  t...|...rSt...|.
-000006b0: a101 6e01 6406 7406 a008 7c02 a101 6407  ..n.d.t...|...d.
-000006c0: 9c05 1600 7d03 7409 7406 a00a 7c03 a101  ....}.t.t...|...
-000006d0: 8301 8201 6400 7d02 6400 5300 2908 4eda  ....d.}.d.S.).N.
-000006e0: 0673 6563 7265 747a 3e61 7373 6572 7420  .secretz>assert 
-000006f0: 2528 7079 3529 730a 7b25 2870 7935 2973  %(py5)s.{%(py5)s
-00000700: 203d 2025 2870 7930 2973 2825 2870 7931   = %(py0)s(%(py1
-00000710: 2973 2c20 2528 7079 3229 732c 2025 2870  )s, %(py2)s, %(p
-00000720: 7933 2973 290a 7d72 0700 0000 7209 0000  y3)s).}r....r...
-00000730: 00da 076d 6573 7361 6765 da09 7369 676e  ...message..sign
-00000740: 6174 7572 6529 0572 0d00 0000 7221 0000  ature).r....r!..
-00000750: 0072 2200 0000 720e 0000 0072 0f00 0000  .r"...r....r....
-00000760: 290b 7206 0000 0072 0800 0000 7207 0000  ).r....r....r...
-00000770: 0072 0900 0000 7212 0000 0072 1300 0000  .r....r....r....
-00000780: 7210 0000 0072 1400 0000 7215 0000 0072  r....r....r....r
-00000790: 1600 0000 7217 0000 0029 0472 2b00 0000  ....r....).r+...
-000007a0: 722c 0000 00da 0b40 7079 5f61 7373 6572  r,.....@py_asser
-000007b0: 7434 721b 0000 0072 1c00 0000 721c 0000  t4r....r....r...
-000007c0: 0072 1d00 0000 da17 7465 7374 5f63 7279  .r......test_cry
-000007d0: 7074 6f5f 7369 676e 5f76 6572 6966 791a  pto_sign_verify.
-000007e0: 0000 0073 0600 0000 0401 0a02 c002 722e  ...s..........r.
-000007f0: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-00000800: 0500 0000 0800 0000 4300 0000 73bc 0000  ........C...s...
-00000810: 0064 017d 0064 027d 0174 0074 017c 007c  .d.}.d.}.t.t.|.|
-00000820: 0183 037d 027c 020c 007d 037c 0373 5664  ...}.|...}.|.sVd
-00000830: 0364 0474 02a0 03a1 0076 0073 1b74 04a0  .d.t.....v.s.t..
-00000840: 0574 00a1 0172 2074 04a0 0674 00a1 016e  .t...r t...t...n
-00000850: 0164 0464 0574 02a0 03a1 0076 0073 2c74  .d.d.t.....v.s,t
-00000860: 04a0 0574 01a1 0172 3174 04a0 0674 01a1  ...t...r1t...t..
-00000870: 016e 0164 0564 0674 02a0 03a1 0076 0073  .n.d.d.t.....v.s
-00000880: 3d74 04a0 057c 00a1 0172 4274 04a0 067c  =t...|...rBt...|
-00000890: 00a1 016e 0164 0674 04a0 067c 01a1 0174  ...n.d.t...|...t
-000008a0: 04a0 067c 02a1 0164 079c 0516 007d 0474  ...|...d.....}.t
-000008b0: 0774 04a0 087c 04a1 0183 0182 0164 0004  .t...|.......d..
-000008c0: 007d 0104 007d 027d 0364 0053 0029 084e  .}...}.}.d.S.).N
-000008d0: 722a 0000 00da 007a 4261 7373 6572 7420  r*.....zBassert 
-000008e0: 6e6f 7420 2528 7079 3629 730a 7b25 2870  not %(py6)s.{%(p
-000008f0: 7936 2973 203d 2025 2870 7930 2973 2825  y6)s = %(py0)s(%
-00000900: 2870 7931 2973 2c20 2528 7079 3229 732c  (py1)s, %(py2)s,
-00000910: 2025 2870 7934 2973 290a 7d72 0700 0000   %(py4)s).}r....
-00000920: 7209 0000 0072 2b00 0000 7220 0000 0029  r....r+...r ...)
-00000930: 0972 0700 0000 7209 0000 0072 1200 0000  .r....r....r....
-00000940: 7213 0000 0072 1000 0000 7214 0000 0072  r....r....r....r
-00000950: 1500 0000 7216 0000 0072 1700 0000 2905  ....r....r....).
-00000960: 722b 0000 0072 2600 0000 7227 0000 005a  r+...r&...r'...Z
-00000970: 0b40 7079 5f61 7373 6572 7437 da0b 4070  .@py_assert7..@p
-00000980: 795f 666f 726d 6174 3872 1c00 0000 721c  y_format8r....r.
-00000990: 0000 0072 1d00 0000 da1f 7465 7374 5f63  ...r......test_c
-000009a0: 7279 7074 6f5f 7369 676e 5f76 6572 6966  rypto_sign_verif
-000009b0: 795f 6661 696c 7572 6522 0000 0073 0400  y_failure"...s..
-000009c0: 0000 0401 b802 7231 0000 0029 14da 0862  ......r1...)...b
-000009d0: 7569 6c74 696e 7372 1200 0000 da19 5f70  uiltinsr......_p
-000009e0: 7974 6573 742e 6173 7365 7274 696f 6e2e  ytest.assertion.
-000009f0: 7265 7772 6974 65da 0961 7373 6572 7469  rewrite..asserti
-00000a00: 6f6e da07 7265 7772 6974 6572 1000 0000  on..rewriter....
-00000a10: da29 6372 7970 746f 6772 6170 6879 2e68  .)cryptography.h
-00000a20: 617a 6d61 742e 7072 696d 6974 6976 6573  azmat.primitives
-00000a30: 2e61 7379 6d6d 6574 7269 6372 0200 0000  .asymmetricr....
-00000a40: da06 6865 6c70 6572 7204 0000 0072 0500  ..helperr....r..
-00000a50: 0000 7206 0000 0072 0700 0000 da04 7465  ..r....r......te
-00000a60: 7374 7208 0000 0072 0900 0000 721e 0000  str....r....r...
-00000a70: 0072 2900 0000 722e 0000 0072 3100 0000  .r)...r....r1...
-00000a80: 721c 0000 0072 1c00 0000 721c 0000 0072  r....r....r....r
-00000a90: 1d00 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
-00000aa0: 0000 730e 0000 0026 0018 0210 0608 0308  ..s....&........
-00000ab0: 0608 080c 08                             .....
+00000330: 7267 2f62 6f76 696e 652f 626f 7669 6e65  rg/bovine/bovine
+00000340: 2f62 6f76 696e 652f 626f 7669 6e65 2f63  /bovine/bovine/c
+00000350: 7279 7074 6f2f 7465 7374 5f68 656c 7065  rypto/test_helpe
+00000360: 722e 7079 da1a 7465 7374 5f63 6f6e 7465  r.py..test_conte
+00000370: 6e74 5f64 6967 6573 745f 7368 6132 3536  nt_digest_sha256
+00000380: 0c00 0000 7304 0000 0008 017c 0272 1e00  ....s......|.r..
+00000390: 0000 6300 0000 0000 0000 0000 0000 0005  ..c.............
+000003a0: 0000 0008 0000 0043 0000 0073 ba00 0000  .......C...s....
+000003b0: 6401 7d00 7400 7c00 8301 7d01 7401 6a02  d.}.t.|...}.t.j.
+000003c0: 7d02 7403 7c01 7c02 8302 7d03 7c03 7357  }.t.|.|...}.|.sW
+000003d0: 6402 6403 7404 a005 a100 7600 731c 7406  d.d.t.....v.s.t.
+000003e0: a007 7403 a101 7221 7406 a008 7403 a101  ..t...r!t...t...
+000003f0: 6e01 6403 6404 7404 a005 a100 7600 732d  n.d.d.t.....v.s-
+00000400: 7406 a007 7c01 a101 7232 7406 a008 7c01  t...|...r2t...|.
+00000410: a101 6e01 6404 6405 7404 a005 a100 7600  ..n.d.d.t.....v.
+00000420: 733e 7406 a007 7401 a101 7243 7406 a008  s>t...t...rCt...
+00000430: 7401 a101 6e01 6405 7406 a008 7c02 a101  t...n.d.t...|...
+00000440: 7406 a008 7c03 a101 6406 9c05 1600 7d04  t...|...d.....}.
+00000450: 7409 7406 a00a 7c04 a101 8301 8201 6400  t.t...|.......d.
+00000460: 0400 7d02 7d03 6400 5300 2907 4e7a 3864  ..}.}.d.S.).Nz8d
+00000470: 6964 3a6b 6579 3a7a 364d 6b69 5442 7a31  id:key:z6MkiTBz1
+00000480: 796d 7565 7041 5134 4845 4859 5346 3148  ymuepAQ4HEHYSF1H
+00000490: 3871 7547 3547 4c56 5651 5233 646a 6458  8quG5GLVVQR3djdX
+000004a0: 336d 446f 6f57 707a 5b61 7373 6572 7420  3mDooWpz[assert 
+000004b0: 2528 7079 3629 730a 7b25 2870 7936 2973  %(py6)s.{%(py6)s
+000004c0: 203d 2025 2870 7930 2973 2825 2870 7931   = %(py0)s(%(py1
+000004d0: 2973 2c20 2528 7079 3429 730a 7b25 2870  )s, %(py4)s.{%(p
+000004e0: 7934 2973 203d 2025 2870 7932 2973 2e45  y4)s = %(py2)s.E
+000004f0: 6432 3535 3139 5075 626c 6963 4b65 790a  d25519PublicKey.
+00000500: 7d29 0a7d da0a 6973 696e 7374 616e 6365  }).}..isinstance
+00000510: 7209 0000 0072 0200 0000 a905 720d 0000  r....r......r...
+00000520: 00da 0370 7931 da03 7079 32da 0370 7934  ...py1..py2..py4
+00000530: da03 7079 3629 0b72 0500 0000 7202 0000  ..py6).r....r...
+00000540: 00da 1045 6432 3535 3139 5075 626c 6963  ...Ed25519Public
+00000550: 4b65 7972 1f00 0000 7212 0000 0072 1300  Keyr....r....r..
+00000560: 0000 7210 0000 0072 1400 0000 7215 0000  ..r....r....r...
+00000570: 0072 1600 0000 7217 0000 0029 055a 0b64  .r....r....).Z.d
+00000580: 6964 5f65 7861 6d70 6c65 7209 0000 00da  id_exampler.....
+00000590: 0b40 7079 5f61 7373 6572 7433 da0b 4070  .@py_assert3..@p
+000005a0: 795f 6173 7365 7274 35da 0b40 7079 5f66  y_assert5..@py_f
+000005b0: 6f72 6d61 7437 721c 0000 0072 1c00 0000  ormat7r....r....
+000005c0: 721d 0000 00da 1674 6573 745f 6469 645f  r......test_did_
+000005d0: 746f 5f70 7562 6c69 635f 6b65 7912 0000  to_public_key...
+000005e0: 0073 0600 0000 0401 0802 ae02 7229 0000  .s..........r)..
+000005f0: 0063 0000 0000 0000 0000 0000 0000 0400  .c..............
+00000600: 0000 0800 0000 4300 0000 73ce 0000 0064  ......C...s....d
+00000610: 017d 0074 0074 017c 0083 027d 0174 0274  .}.t.t.|...}.t.t
+00000620: 037c 007c 0183 037d 027c 0273 6364 0264  .|.|...}.|.scd.d
+00000630: 0374 04a0 05a1 0076 0073 1b74 06a0 0774  .t.....v.s.t...t
+00000640: 02a1 0172 2074 06a0 0874 02a1 016e 0164  ...r t...t...n.d
+00000650: 0364 0474 04a0 05a1 0076 0073 2c74 06a0  .d.t.....v.s,t..
+00000660: 0774 03a1 0172 3174 06a0 0874 03a1 016e  .t...r1t...t...n
+00000670: 0164 0464 0574 04a0 05a1 0076 0073 3d74  .d.d.t.....v.s=t
+00000680: 06a0 077c 00a1 0172 4274 06a0 087c 00a1  ...|...rBt...|..
+00000690: 016e 0164 0564 0674 04a0 05a1 0076 0073  .n.d.d.t.....v.s
+000006a0: 4e74 06a0 077c 01a1 0172 5374 06a0 087c  Nt...|...rSt...|
+000006b0: 01a1 016e 0164 0674 06a0 087c 02a1 0164  ...n.d.t...|...d
+000006c0: 079c 0516 007d 0374 0974 06a0 0a7c 03a1  .....}.t.t...|..
+000006d0: 0183 0182 0164 007d 0264 0053 0029 084e  .....d.}.d.S.).N
+000006e0: da06 7365 6372 6574 7a3e 6173 7365 7274  ..secretz>assert
+000006f0: 2025 2870 7935 2973 0a7b 2528 7079 3529   %(py5)s.{%(py5)
+00000700: 7320 3d20 2528 7079 3029 7328 2528 7079  s = %(py0)s(%(py
+00000710: 3129 732c 2025 2870 7932 2973 2c20 2528  1)s, %(py2)s, %(
+00000720: 7079 3329 7329 0a7d 7207 0000 0072 0900  py3)s).}r....r..
+00000730: 0000 da07 6d65 7373 6167 65da 0973 6967  ....message..sig
+00000740: 6e61 7475 7265 2905 720d 0000 0072 2100  nature).r....r!.
+00000750: 0000 7222 0000 0072 0e00 0000 720f 0000  ..r"...r....r...
+00000760: 0029 0b72 0600 0000 7208 0000 0072 0700  .).r....r....r..
+00000770: 0000 7209 0000 0072 1200 0000 7213 0000  ..r....r....r...
+00000780: 0072 1000 0000 7214 0000 0072 1500 0000  .r....r....r....
+00000790: 7216 0000 0072 1700 0000 2904 722b 0000  r....r....).r+..
+000007a0: 0072 2c00 0000 da0b 4070 795f 6173 7365  .r,.....@py_asse
+000007b0: 7274 3472 1b00 0000 721c 0000 0072 1c00  rt4r....r....r..
+000007c0: 0000 721d 0000 00da 1774 6573 745f 6372  ..r......test_cr
+000007d0: 7970 746f 5f73 6967 6e5f 7665 7269 6679  ypto_sign_verify
+000007e0: 1a00 0000 7306 0000 0004 010a 02c0 0272  ....s..........r
+000007f0: 2e00 0000 6300 0000 0000 0000 0000 0000  ....c...........
+00000800: 0005 0000 0008 0000 0043 0000 0073 bc00  .........C...s..
+00000810: 0000 6401 7d00 6402 7d01 7400 7401 7c00  ..d.}.d.}.t.t.|.
+00000820: 7c01 8303 7d02 7c02 0c00 7d03 7c03 7356  |...}.|...}.|.sV
+00000830: 6403 6404 7402 a003 a100 7600 731b 7404  d.d.t.....v.s.t.
+00000840: a005 7400 a101 7220 7404 a006 7400 a101  ..t...r t...t...
+00000850: 6e01 6404 6405 7402 a003 a100 7600 732c  n.d.d.t.....v.s,
+00000860: 7404 a005 7401 a101 7231 7404 a006 7401  t...t...r1t...t.
+00000870: a101 6e01 6405 6406 7402 a003 a100 7600  ..n.d.d.t.....v.
+00000880: 733d 7404 a005 7c00 a101 7242 7404 a006  s=t...|...rBt...
+00000890: 7c00 a101 6e01 6406 7404 a006 7c01 a101  |...n.d.t...|...
+000008a0: 7404 a006 7c02 a101 6407 9c05 1600 7d04  t...|...d.....}.
+000008b0: 7407 7404 a008 7c04 a101 8301 8201 6400  t.t...|.......d.
+000008c0: 0400 7d01 0400 7d02 7d03 6400 5300 2908  ..}...}.}.d.S.).
+000008d0: 4e72 2a00 0000 da00 7a42 6173 7365 7274  Nr*.....zBassert
+000008e0: 206e 6f74 2025 2870 7936 2973 0a7b 2528   not %(py6)s.{%(
+000008f0: 7079 3629 7320 3d20 2528 7079 3029 7328  py6)s = %(py0)s(
+00000900: 2528 7079 3129 732c 2025 2870 7932 2973  %(py1)s, %(py2)s
+00000910: 2c20 2528 7079 3429 7329 0a7d 7207 0000  , %(py4)s).}r...
+00000920: 0072 0900 0000 722b 0000 0072 2000 0000  .r....r+...r ...
+00000930: 2909 7207 0000 0072 0900 0000 7212 0000  ).r....r....r...
+00000940: 0072 1300 0000 7210 0000 0072 1400 0000  .r....r....r....
+00000950: 7215 0000 0072 1600 0000 7217 0000 0029  r....r....r....)
+00000960: 0572 2b00 0000 7226 0000 0072 2700 0000  .r+...r&...r'...
+00000970: 5a0b 4070 795f 6173 7365 7274 37da 0b40  Z.@py_assert7..@
+00000980: 7079 5f66 6f72 6d61 7438 721c 0000 0072  py_format8r....r
+00000990: 1c00 0000 721d 0000 00da 1f74 6573 745f  ....r......test_
+000009a0: 6372 7970 746f 5f73 6967 6e5f 7665 7269  crypto_sign_veri
+000009b0: 6679 5f66 6169 6c75 7265 2200 0000 7304  fy_failure"...s.
+000009c0: 0000 0004 01b8 0272 3100 0000 2914 da08  .......r1...)...
+000009d0: 6275 696c 7469 6e73 7212 0000 00da 195f  builtinsr......_
+000009e0: 7079 7465 7374 2e61 7373 6572 7469 6f6e  pytest.assertion
+000009f0: 2e72 6577 7269 7465 da09 6173 7365 7274  .rewrite..assert
+00000a00: 696f 6eda 0772 6577 7269 7465 7210 0000  ion..rewriter...
+00000a10: 00da 2963 7279 7074 6f67 7261 7068 792e  ..)cryptography.
+00000a20: 6861 7a6d 6174 2e70 7269 6d69 7469 7665  hazmat.primitive
+00000a30: 732e 6173 796d 6d65 7472 6963 7202 0000  s.asymmetricr...
+00000a40: 00da 0668 656c 7065 7272 0400 0000 7205  ...helperr....r.
+00000a50: 0000 0072 0600 0000 7207 0000 00da 0474  ...r....r......t
+00000a60: 6573 7472 0800 0000 7209 0000 0072 1e00  estr....r....r..
+00000a70: 0000 7229 0000 0072 2e00 0000 7231 0000  ..r)...r....r1..
+00000a80: 0072 1c00 0000 721c 0000 0072 1c00 0000  .r....r....r....
+00000a90: 721d 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
+00000aa0: 0000 0073 0e00 0000 2600 1802 1006 0803  ...s....&.......
+00000ab0: 0806 0808 0c08                           ......
```

### Comparing `bovine-0.1.0/bovine/crypto/__pycache__/test_http_signature.cpython-310-pytest-7.3.0.pyc` & `bovine-0.1.1/bovine/crypto/__pycache__/test_http_signature.cpython-310-pytest-7.3.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 13 15:55:57 2023 UTC, .py size: 5081 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0d26 3864 d913 0000  o........&8d....
+00000000: 6f0d 0d0a 0000 0000 a4ea 3a64 d913 0000  o.........:d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 7600 0000 6400  .....@...sv...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6401 6c06 5a06  ..m.Z...d.d.l.Z.
 00000050: 6402 6403 6c07 6d08 5a08 0100 6402 6404  d.d.l.m.Z...d.d.
 00000060: 6c09 6d0a 5a0a 6d0b 5a0b 0100 6402 6405  l.m.Z.m.Z...d.d.
 00000070: 6c0c 6d0d 5a0d 0100 6406 6407 8400 5a0e  l.m.Z...d.d...Z.
@@ -95,372 +95,372 @@
 000005e0: 6e61 7469 6f6e 290a da0e 6874 7470 5f73  nation)...http_s
 000005f0: 6967 6e61 7475 7265 da10 7369 676e 6174  ignature..signat
 00000600: 7572 655f 7374 7269 6e67 7209 0000 0072  ure_stringr....r
 00000610: 1500 0000 7216 0000 0072 1700 0000 da0b  ....r....r......
 00000620: 4070 795f 6173 7365 7274 32da 0b40 7079  @py_assert2..@py
 00000630: 5f61 7373 6572 7431 da0b 4070 795f 666f  _assert1..@py_fo
 00000640: 726d 6174 34da 0b40 7079 5f66 6f72 6d61  rmat4..@py_forma
-00000650: 7436 a900 7228 0000 00fa 552f 776f 6f64  t6..r(....U/wood
+00000650: 7436 a900 7228 0000 00fa 562f 776f 6f64  t6..r(....V/wood
 00000660: 7065 636b 6572 2f73 7263 2f63 6f64 6562  pecker/src/codeb
-00000670: 6572 672e 6f72 672f 6865 6c67 652f 626f  erg.org/helge/bo
-00000680: 7669 6e65 2f62 6f76 696e 652f 626f 7669  vine/bovine/bovi
-00000690: 6e65 2f63 7279 7074 6f2f 7465 7374 5f68  ne/crypto/test_h
-000006a0: 7474 705f 7369 676e 6174 7572 652e 7079  ttp_signature.py
-000006b0: da13 7465 7374 5f68 7474 705f 7369 676e  ..test_http_sign
-000006c0: 6174 7572 6508 0000 0073 3a00 0000 0e01  ature....s:.....
-000006d0: 0c02 1202 7802 7801 7801 1401 0203 0efd  ....x.x.x.......
-000006e0: 0203 04fd 0403 06fd 0203 02fd 0203 04fd  ................
-000006f0: 0203 02fd 0403 04fd 0203 02fd 0203 18fd  ................
-00000700: 0203 02fd 0203 10fd 722a 0000 0063 0000  ........r*...c..
-00000710: 0000 0000 0000 0000 0000 0a00 0000 0700  ................
-00000720: 0000 4300 0000 739a 0200 0074 0064 0164  ..C...s....t.d.d
-00000730: 0264 0383 03a0 0164 0464 05a1 0204 007d  .d.....d.d.....}
-00000740: 007d 007c 00a0 0064 0674 02a1 027d 0164  .}.|...d.t...}.d
-00000750: 077d 027c 017c 026b 027d 037c 0373 4a74  .}.|.|.k.}.|.sJt
-00000760: 03a0 0464 087c 0366 0164 097c 017c 0266  ...d.|.f.d.|.|.f
-00000770: 02a1 0464 0a74 05a0 06a1 0076 0073 2f74  ...d.t.....v.s/t
-00000780: 03a0 077c 01a1 0172 3474 03a0 087c 01a1  ...|...r4t...|..
-00000790: 016e 0164 0a74 03a0 087c 02a1 0164 0b9c  .n.d.t...|...d..
-000007a0: 0216 007d 0464 0c64 0d7c 0469 0116 007d  ...}.d.d.|.i...}
-000007b0: 0574 0974 03a0 0a7c 05a1 0183 0182 0164  .t.t...|.......d
-000007c0: 0004 007d 037d 027c 01a0 0b64 0ea1 015c  ...}.}.|...d...\
-000007d0: 047d 067d 077d 087d 0964 0f7d 027c 067c  .}.}.}.}.d.}.|.|
-000007e0: 026b 027d 037c 0373 8f74 03a0 0464 087c  .k.}.|.s.t...d.|
-000007f0: 0366 0164 097c 067c 0266 02a1 0464 0674  .f.d.|.|.f...d.t
-00000800: 05a0 06a1 0076 0073 7474 03a0 077c 06a1  .....v.stt...|..
-00000810: 0172 7974 03a0 087c 06a1 016e 0164 0674  .ryt...|...n.d.t
-00000820: 03a0 087c 02a1 0164 0b9c 0216 007d 0464  ...|...d.....}.d
-00000830: 0c64 0d7c 0469 0116 007d 0574 0974 03a0  .d.|.i...}.t.t..
-00000840: 0a7c 05a1 0183 0182 0164 0004 007d 037d  .|.......d...}.}
-00000850: 0264 107d 027c 077c 026b 027d 037c 0373  .d.}.|.|.k.}.|.s
-00000860: cb74 03a0 0464 087c 0366 0164 097c 077c  .t...d.|.f.d.|.|
-00000870: 0266 02a1 0464 1174 05a0 06a1 0076 0073  .f...d.t.....v.s
-00000880: b074 03a0 077c 07a1 0172 b574 03a0 087c  .t...|...r.t...|
-00000890: 07a1 016e 0164 1174 03a0 087c 02a1 0164  ...n.d.t...|...d
-000008a0: 0b9c 0216 007d 0464 0c64 0d7c 0469 0116  .....}.d.d.|.i..
-000008b0: 007d 0574 0974 03a0 0a7c 05a1 0183 0182  .}.t.t...|......
-000008c0: 0164 0004 007d 037d 0264 127d 027c 087c  .d...}.}.d.}.|.|
-000008d0: 026b 027d 037c 0390 0173 0874 03a0 0464  .k.}.|...s.t...d
-000008e0: 087c 0366 0164 097c 087c 0266 02a1 0464  .|.f.d.|.|.f...d
-000008f0: 1374 05a0 06a1 0076 0073 ed74 03a0 077c  .t.....v.s.t...|
-00000900: 08a1 0172 f274 03a0 087c 08a1 016e 0164  ...r.t...|...n.d
-00000910: 1374 03a0 087c 02a1 0164 0b9c 0216 007d  .t...|...d.....}
-00000920: 0464 0c64 0d7c 0469 0116 007d 0574 0974  .d.d.|.i...}.t.t
-00000930: 03a0 0a7c 05a1 0183 0182 0164 0004 007d  ...|.......d...}
-00000940: 037d 0264 147d 027c 097c 026b 027d 037c  .}.d.}.|.|.k.}.|
-00000950: 0390 0173 4774 03a0 0464 087c 0366 0164  ...sGt...d.|.f.d
-00000960: 097c 097c 0266 02a1 0464 1574 05a0 06a1  .|.|.f...d.t....
-00000970: 0076 0090 0173 2c74 03a0 077c 09a1 0190  .v...s,t...|....
-00000980: 0172 3174 03a0 087c 09a1 016e 0164 1574  .r1t...|...n.d.t
-00000990: 03a0 087c 02a1 0164 0b9c 0216 007d 0464  ...|...d.....}.d
-000009a0: 0c64 0d7c 0469 0116 007d 0574 0974 03a0  .d.|.i...}.t.t..
-000009b0: 0a7c 05a1 0183 0182 0164 0004 007d 037d  .|.......d...}.}
-000009c0: 0264 0053 0029 164e fa0a 6d79 686f 7374  .d.S.).N..myhost
-000009d0: 2e74 6c64 da03 6765 74fa 112f 7061 7468  .tld..get../path
-000009e0: 2f74 6f2f 7265 736f 7572 6365 da04 6461  /to/resource..da
-000009f0: 7465 fa1d 5765 642c 2031 3520 4d61 7220  te..Wed, 15 Mar 
-00000a00: 3230 3233 2031 373a 3238 3a31 3520 474d  2023 17:28:15 GM
-00000a10: 5472 0900 0000 61af 0100 006b 6579 4964  Tr....a....keyId
-00000a20: 3d22 6b65 795f 6964 222c 616c 676f 7269  ="key_id",algori
-00000a30: 7468 6d3d 2272 7361 2d73 6861 3235 3622  thm="rsa-sha256"
-00000a40: 2c68 6561 6465 7273 3d22 2872 6571 7565  ,headers="(reque
-00000a50: 7374 2d74 6172 6765 7429 2068 6f73 7420  st-target) host 
-00000a60: 6461 7465 222c 7369 676e 6174 7572 653d  date",signature=
-00000a70: 2262 7767 4133 5561 6a70 447a 4d30 3777  "bwgA3UajpDzM07w
-00000a80: 4d2b 4d55 6b70 4748 532f 6d41 6868 5475  M+MUkpGHS/mAhhTu
-00000a90: 2b57 4469 424c 3148 3238 4a37 3632 6a55  +WDiBL1H28J762jU
-00000aa0: 5575 6767 7a50 3857 6535 2b49 3057 4879  UuggzP8We5+I0WHy
-00000ab0: 7053 4243 5774 384c 6170 3241 6259 7147  pSBCWt8Lap2AbYqG
-00000ac0: 3650 6654 7364 4645 626b 3856 5765 7758  6PfTsdFEbk8VWewX
-00000ad0: 3334 6e37 2f4c 5553 4d2f 574a 6541 3841  34n7/LUSM/WJeA8A
-00000ae0: 4643 456e 4859 5064 3872 5269 6234 6430  FCEnHYPd8rRib4d0
-00000af0: 2b6b 5156 2b55 3441 6939 3937 5855 7873  +kQV+U4Ai997XUxs
-00000b00: 3278 6932 4172 754e 646b 4236 534e 4d6b  2xi2AruNdkB6SNMk
-00000b10: 5362 6e51 4c6f 426a 5954 3474 7a47 6166  SbnQLoBjYT4tzGaf
-00000b20: 3249 3178 5a75 716a 4431 4876 7657 3078  2I1xZuqjD1HvvW0x
-00000b30: 6131 6f2f 6e50 7434 4735 6b6a 3074 566d  a1o/nPt4G5kj0tVm
-00000b40: 6744 7272 6765 4b4c 3268 554a 3231 5564  gDrrgeKL2hUJ21Ud
-00000b50: 4863 5844 4e46 7739 514a 5766 2f4f 364b  HcXDNFw9QJWf/O6K
-00000b60: 7945 6d62 756d 7670 704b 4746 5566 6470  yEmbumvppKGFUfdp
-00000b70: 4b53 6833 6e32 2f66 5037 4f34 4278 7161  KSh3n2/fP7O4Bxqa
-00000b80: 6443 624d 596a 306f 4444 4f46 3148 3350  dCbMYj0oDDOF1H3P
-00000b90: 6136 4756 3945 6649 6553 5858 4c53 3954  a6GV9EfIeSXXLS9T
-00000ba0: 6679 5070 6b58 7762 5772 4e70 7a55 425a  fyPpkXwbWrNpzUBZ
-00000bb0: 5132 6852 477a 5832 6a53 2f4a 4568 7053  Q2hRGzX2jS/JEhpS
-00000bc0: 4e53 5671 7636 413d 3d22 720c 0000 0072  NSVqv6A=="r....r
-00000bd0: 0e00 0000 7223 0000 0072 0f00 0000 7212  ....r#...r....r.
-00000be0: 0000 0072 1300 0000 720a 0000 0072 0b00  ...r....r....r..
-00000bf0: 0000 7214 0000 0072 1500 0000 7a24 6865  ..r....r....z$he
-00000c00: 6164 6572 733d 2228 7265 7175 6573 742d  aders="(request-
-00000c10: 7461 7267 6574 2920 686f 7374 2064 6174  target) host dat
-00000c20: 6522 7216 0000 0061 6401 0000 7369 676e  e"r....ad...sign
-00000c30: 6174 7572 653d 2262 7767 4133 5561 6a70  ature="bwgA3Uajp
-00000c40: 447a 4d30 3777 4d2b 4d55 6b70 4748 532f  DzM07wM+MUkpGHS/
-00000c50: 6d41 6868 5475 2b57 4469 424c 3148 3238  mAhhTu+WDiBL1H28
-00000c60: 4a37 3632 6a55 5575 6767 7a50 3857 6535  J762jUUuggzP8We5
-00000c70: 2b49 3057 4879 7053 4243 5774 384c 6170  +I0WHypSBCWt8Lap
-00000c80: 3241 6259 7147 3650 6654 7364 4645 626b  2AbYqG6PfTsdFEbk
-00000c90: 3856 5765 7758 3334 6e37 2f4c 5553 4d2f  8VWewX34n7/LUSM/
-00000ca0: 574a 6541 3841 4643 456e 4859 5064 3872  WJeA8AFCEnHYPd8r
-00000cb0: 5269 6234 6430 2b6b 5156 2b55 3441 6939  Rib4d0+kQV+U4Ai9
-00000cc0: 3937 5855 7873 3278 6932 4172 754e 646b  97XUxs2xi2AruNdk
-00000cd0: 4236 534e 4d6b 5362 6e51 4c6f 426a 5954  B6SNMkSbnQLoBjYT
-00000ce0: 3474 7a47 6166 3249 3178 5a75 716a 4431  4tzGaf2I1xZuqjD1
-00000cf0: 4876 7657 3078 6131 6f2f 6e50 7434 4735  HvvW0xa1o/nPt4G5
-00000d00: 6b6a 3074 566d 6744 7272 6765 4b4c 3268  kj0tVmgDrrgeKL2h
-00000d10: 554a 3231 5564 4863 5844 4e46 7739 514a  UJ21UdHcXDNFw9QJ
-00000d20: 5766 2f4f 364b 7945 6d62 756d 7670 704b  Wf/O6KyEmbumvppK
-00000d30: 4746 5566 6470 4b53 6833 6e32 2f66 5037  GFUfdpKSh3n2/fP7
-00000d40: 4f34 4278 7161 6443 624d 596a 306f 4444  O4BxqadCbMYj0oDD
-00000d50: 4f46 3148 3350 6136 4756 3945 6649 6553  OF1H3Pa6GV9EfIeS
-00000d60: 5858 4c53 3954 6679 5070 6b58 7762 5772  XXLS9TfyPpkXwbWr
-00000d70: 4e70 7a55 425a 5132 6852 477a 5832 6a53  NpzUBZQ2hRGzX2jS
-00000d80: 2f4a 4568 7053 4e53 5671 7636 413d 3d22  /JEhpSNSVqv6A=="
-00000d90: 7217 0000 0029 0c72 0500 0000 7218 0000  r....).r....r...
-00000da0: 0072 0600 0000 721a 0000 0072 1b00 0000  .r....r....r....
-00000db0: 721c 0000 0072 1d00 0000 721e 0000 0072  r....r....r....r
-00000dc0: 1f00 0000 7220 0000 0072 2100 0000 7219  ....r ...r!...r.
-00000dd0: 0000 0029 0a72 2200 0000 7223 0000 0072  ...).r"...r#...r
-00000de0: 2400 0000 7225 0000 0072 2600 0000 7227  $...r%...r&...r'
-00000df0: 0000 0072 0900 0000 7215 0000 0072 1600  ...r....r....r..
-00000e00: 0000 7217 0000 0072 2800 0000 7228 0000  ..r....r(...r(..
-00000e10: 0072 2900 0000 da14 7465 7374 5f62 7569  .r).....test_bui
-00000e20: 6c64 5f73 6967 6e61 7475 7265 1800 0000  ld_signature....
-00000e30: 7370 0000 0002 0106 0102 ff08 0206 fe0c  sp..............
-00000e40: 0412 0202 030e fd02 0304 fd04 0306 fd02  ................
-00000e50: 0302 fd02 0304 fd02 0302 fd04 0304 fd02  ................
-00000e60: 0302 fd02 0318 fd02 0302 fd02 030c fd12  ................
-00000e70: 0578 0278 017a 0114 0102 030e fd02 0304  .x.x.z..........
-00000e80: fd04 0308 fd02 0302 fd02 0306 fd02 0302  ................
-00000e90: fd04 0304 fd02 0302 fd02 0318 fd02 0302  ................
-00000ea0: fd02 0310 fd72 3000 0000 6300 0000 0000  .....r0...c.....
-00000eb0: 0000 0000 0000 0006 0000 0007 0000 0043  ...............C
-00000ec0: 0000 0073 a800 0000 7400 6401 6402 6403  ...s....t.d.d.d.
-00000ed0: 8303 a001 6404 6405 a102 a001 6406 6407  ....d.d.....d.d.
-00000ee0: a102 0400 7d00 7d00 7c00 a000 6408 7402  ....}.}.|...d.t.
-00000ef0: a102 7d01 6409 7d02 7c01 7c02 6b02 7d03  ..}.d.}.|.|.k.}.
-00000f00: 7c03 734e 7403 a004 640a 7c03 6601 640b  |.sNt...d.|.f.d.
-00000f10: 7c01 7c02 6602 a104 640c 7405 a006 a100  |.|.f...d.t.....
-00000f20: 7600 7333 7403 a007 7c01 a101 7238 7403  v.s3t...|...r8t.
-00000f30: a008 7c01 a101 6e01 640c 7403 a008 7c02  ..|...n.d.t...|.
-00000f40: a101 640d 9c02 1600 7d04 640e 640f 7c04  ..d.....}.d.d.|.
-00000f50: 6901 1600 7d05 7409 7403 a00a 7c05 a101  i...}.t.t...|...
-00000f60: 8301 8201 6400 0400 7d03 7d02 6400 5300  ....d...}.}.d.S.
-00000f70: 2910 4e72 2b00 0000 da04 706f 7374 722d  ).Nr+.....postr-
-00000f80: 0000 0072 2e00 0000 722f 0000 00da 0664  ...r....r/.....d
-00000f90: 6967 6573 74fa 3473 6861 2d32 3536 3d4d  igest.4sha-256=M
-00000fa0: 494c 6235 6c55 4444 365a 3070 4453 7868  ILb5lUDD6Z0pDSxh
-00000fb0: 6778 6a2b 684d 4245 7730 7554 7a50 3367  gxj+hMBEw0uTzP3g
-00000fc0: 3271 554a 4748 4d70 396b 3d72 0900 0000  2qUJGHMp9k=r....
-00000fd0: 61b6 0100 006b 6579 4964 3d22 6b65 795f  a....keyId="key_
-00000fe0: 6964 222c 616c 676f 7269 7468 6d3d 2272  id",algorithm="r
-00000ff0: 7361 2d73 6861 3235 3622 2c68 6561 6465  sa-sha256",heade
-00001000: 7273 3d22 2872 6571 7565 7374 2d74 6172  rs="(request-tar
-00001010: 6765 7429 2068 6f73 7420 6461 7465 2064  get) host date d
-00001020: 6967 6573 7422 2c73 6967 6e61 7475 7265  igest",signature
-00001030: 3d22 5170 654c 4d45 682f 5a30 3039 4467  ="QpeLMEh/Z009Dg
-00001040: 5963 534f 6b72 734b 7239 7a57 3757 7537  YcSOkrsKr9zW7Wu7
-00001050: 5557 5451 3339 3871 7675 6543 7a61 454c  UWTQ398qvueCzaEL
-00001060: 2f48 7872 7639 4334 3255 2b57 592f 4f33  /Hxrv9C42U+WY/O3
-00001070: 3478 2f33 3835 6c54 2b7a 3149 3342 6b36  4x/385lT+z1I3Bk6
-00001080: 714d 5a54 4441 5a53 6d4b 4759 4235 6c5a  qMZTDAZSmKGYB5lZ
-00001090: 4a56 4264 4332 3061 3444 2b2b 487a 4979  JVBdC20a4D++HzIy
-000010a0: 4536 3264 3643 7671 5573 5177 4976 346f  E62d6CvqUsQwIv4o
-000010b0: 642f 684f 6d6d 4f51 3348 4b49 3639 4d55  d/hOmmOQ3HKI69MU
-000010c0: 4f73 4e72 4c79 6a49 5178 5561 4c53 427a  OsNrLyjIQxUaLSBz
-000010d0: 316d 2f77 6b4c 7638 694d 7268 3951 7755  1m/wkLv8iMrh9QwU
-000010e0: 4c6c 7154 4f38 5748 566a 534a 6c67 5677  LlqTO8WHVjSJlgVw
-000010f0: 6c6c 5274 4f4f 636d 3377 7a6f 2f63 7232  llRtOOcm3wzo/cr2
-00001100: 5879 466a 3467 4238 4355 6433 6147 3364  XyFj4gB8CUd3aG3d
-00001110: 717a 4366 4f4f 6f4e 5176 5568 4d44 6c78  qzCfOOoNQvUhMDlx
-00001120: 5037 5571 426e 476f 4636 706e 596e 546e  P7UqBnGoF6pnYnTn
-00001130: 4a55 5353 4864 6365 5762 4530 3954 7158  JUSSHdceWbE09TqX
-00001140: 4c6d 4148 7a61 7559 4753 6461 4852 5333  LmAHzauYGSdaHRS3
-00001150: 5852 2f53 6a65 3745 5439 5561 4f67 4848  XR/Sje7ET9UaOgHH
-00001160: 6350 4a48 494e 2b34 6a72 4270 4470 3247  cPJHIN+4jrBpDp2G
-00001170: 4d36 396a 6f58 576b 5a77 6845 3047 4f6c  M69joXWkZwhE0GOl
-00001180: 3971 334b 4253 4b41 3d3d 2272 0c00 0000  9q3KBSKA=="r....
-00001190: 720e 0000 0072 2300 0000 720f 0000 0072  r....r#...r....r
-000011a0: 1200 0000 7213 0000 0029 0b72 0500 0000  ....r....).r....
-000011b0: 7218 0000 0072 0600 0000 721a 0000 0072  r....r....r....r
-000011c0: 1b00 0000 721c 0000 0072 1d00 0000 721e  ....r....r....r.
-000011d0: 0000 0072 1f00 0000 7220 0000 0072 2100  ...r....r ...r!.
-000011e0: 0000 2906 7222 0000 0072 2300 0000 7224  ..).r"...r#...r$
-000011f0: 0000 0072 2500 0000 7226 0000 0072 2700  ...r%...r&...r'.
-00001200: 0000 7228 0000 0072 2800 0000 7229 0000  ..r(...r(...r)..
-00001210: 00da 1974 6573 745f 6275 696c 645f 7369  ...test_build_si
-00001220: 676e 6174 7572 655f 706f 7374 2f00 0000  gnature_post/...
-00001230: 7338 0000 000a 0208 0108 0106 fd0c 0612  s8..............
-00001240: 0202 030e fd02 0304 fd04 0306 fd02 0302  ................
-00001250: fd02 0304 fd02 0302 fd04 0304 fd02 0302  ................
-00001260: fd02 0318 fd02 0302 fd02 0310 fd72 3400  .............r4.
-00001270: 0000 6300 0000 0000 0000 0000 0000 000c  ..c.............
-00001280: 0000 0007 0000 0043 0000 0073 4601 0000  .......C...sF...
-00001290: 7400 6401 6402 6403 8303 a001 6404 6405  t.d.d.d.....d.d.
-000012a0: a102 7d00 7c00 a002 a100 7d01 6406 7d02  ..}.|.....}.d.}.
-000012b0: 7c01 7c02 6b02 7d03 7c03 7346 7403 a004  |.|.k.}.|.sFt...
-000012c0: 6407 7c03 6601 6408 7c01 7c02 6602 a104  d.|.f.d.|.|.f...
-000012d0: 6409 7405 a006 a100 7600 732b 7403 a007  d.t.....v.s+t...
-000012e0: 7c01 a101 7230 7403 a008 7c01 a101 6e01  |...r0t...|...n.
-000012f0: 6409 7403 a008 7c02 a101 640a 9c02 1600  d.t...|...d.....
-00001300: 7d04 640b 640c 7c04 6901 1600 7d05 7409  }.d.d.|.i...}.t.
-00001310: 7403 a00a 7c05 a101 8301 8201 6400 0400  t...|.......d...
-00001320: 7d03 7d02 7c00 a00b 640d a101 7d06 640e  }.}.|...d...}.d.
-00001330: 7d02 640f 7d07 7c02 7c07 1700 7d08 7c06  }.d.}.|.|...}.|.
-00001340: 7c08 6b02 7d03 7c03 7391 7403 a004 6407  |.k.}.|.s.t...d.
-00001350: 7c03 6601 6410 7c06 7c08 6602 a104 6411  |.f.d.|.|.f...d.
-00001360: 7405 a006 a100 7600 7372 7403 a007 7c06  t.....v.srt...|.
-00001370: a101 7277 7403 a008 7c06 a101 6e01 6411  ..rwt...|...n.d.
-00001380: 7403 a008 7c02 a101 7403 a008 7c07 a101  t...|...t...|...
-00001390: 6412 9c03 1600 7d09 6413 6414 7c09 6901  d.....}.d.d.|.i.
-000013a0: 1600 7d0a 7409 7403 a00a 7c0a a101 8301  ..}.t.t...|.....
-000013b0: 8201 6400 0400 7d03 0400 7d02 0400 7d07  ..d...}...}...}.
-000013c0: 7d08 6415 7d0b 7c00 a00c 7c0b 7c06 a102  }.d.}.|...|.|...
-000013d0: 0100 6400 5300 2916 4e72 2b00 0000 722c  ..d.S.).Nr+...r,
-000013e0: 0000 0072 2d00 0000 722e 0000 0072 2f00  ...r-...r....r/.
-000013f0: 0000 7a5c 2872 6571 7565 7374 2d74 6172  ..z\(request-tar
-00001400: 6765 7429 3a20 6765 7420 2f70 6174 682f  get): get /path/
-00001410: 746f 2f72 6573 6f75 7263 650a 686f 7374  to/resource.host
-00001420: 3a20 6d79 686f 7374 2e74 6c64 0a64 6174  : myhost.tld.dat
-00001430: 653a 2057 6564 2c20 3135 204d 6172 2032  e: Wed, 15 Mar 2
-00001440: 3032 3320 3137 3a32 383a 3135 2047 4d54  023 17:28:15 GMT
-00001450: 720c 0000 0072 0e00 0000 da07 6d65 7373  r....r......mess
-00001460: 6167 6572 0f00 0000 7212 0000 0072 1300  ager....r....r..
-00001470: 0000 da30 7a33 7532 5978 636f 7773 6172  ...0z3u2Yxcowsar
-00001480: 6574 6865 6265 7374 636f 7773 6172 6574  ethebestcowsaret
-00001490: 6865 6265 7374 636f 7773 6172 6574 6865  hebestcowsarethe
-000014a0: 6265 7374 5a2e 7a35 6168 6448 4362 5039  bestZ.z5ahdHCbP9
-000014b0: 614a 4573 4474 7647 314d 455a 7078 507a  aJEsDtvG1MEZpxPz
-000014c0: 7576 474b 5963 6458 644b 764d 7135 594c  uvGKYcdXdKvMq5YL
-000014d0: 3231 5a32 5a2b 756d 786a 7331 536f 7043  21Z2Z+umxjs1SopC
-000014e0: 5932 4170 3876 5a78 566a 5445 6636 6459  Y2Ap8vZxVjTEf6dY
-000014f0: 6247 7542 376d 7467 6367 5579 4e64 424c  bGuB7mtgcgUyNdBL
-00001500: 65a9 017a 1e25 2870 7930 2973 203d 3d20  e..z.%(py0)s == 
-00001510: 2825 2870 7933 2973 202b 2025 2870 7935  (%(py3)s + %(py5
-00001520: 2973 2972 1700 0000 a903 7210 0000 0072  )s)r......r....r
-00001530: 1100 0000 7213 0000 00fa 0e61 7373 6572  ....r......asser
-00001540: 7420 2528 7079 3829 73da 0370 7938 fa38  t %(py8)s..py8.8
-00001550: 6469 643a 6b65 793a 7a36 4d6b 656b 7743  did:key:z6MkekwC
-00001560: 3652 3962 6a39 4572 546f 4237 4169 5a4a  6R9bj9ErToB7AiZJ
-00001570: 6679 4353 4468 615a 6531 5578 6844 6243  fyCSDhaZe1UxhDbC
-00001580: 714a 7268 7170 5335 290d 7205 0000 0072  qJrhqpS5).r....r
-00001590: 1800 0000 da0d 6275 696c 645f 6d65 7373  ......build_mess
-000015a0: 6167 6572 1a00 0000 721b 0000 0072 1c00  ager....r....r..
-000015b0: 0000 721d 0000 0072 1e00 0000 721f 0000  ..r....r....r...
-000015c0: 0072 2000 0000 7221 0000 00da 0c65 6432  .r ...r!.....ed2
-000015d0: 3535 3139 5f73 6967 6eda 0e65 6432 3535  5519_sign..ed255
-000015e0: 3139 5f76 6572 6966 7929 0c72 2200 0000  19_verify).r"...
-000015f0: 7235 0000 0072 2400 0000 7225 0000 0072  r5...r$...r%...r
-00001600: 2600 0000 7227 0000 0072 1700 0000 da0b  &...r'...r......
-00001610: 4070 795f 6173 7365 7274 34da 0b40 7079  @py_assert4..@py
-00001620: 5f61 7373 6572 7436 da0b 4070 795f 666f  _assert6..@py_fo
-00001630: 726d 6174 37da 0b40 7079 5f66 6f72 6d61  rmat7..@py_forma
-00001640: 7439 da06 6469 646b 6579 7228 0000 0072  t9..didkeyr(...r
-00001650: 2800 0000 7229 0000 00da 1274 6573 745f  (...r).....test_
-00001660: 6275 696c 645f 6d65 7373 6167 653e 0000  build_message>..
-00001670: 0073 7a00 0000 0201 0601 02ff 0802 02fe  .sz.............
-00001680: 0804 1202 0205 0efb 0205 04fb 0405 06fb  ................
-00001690: 0205 02fb 0205 04fb 0205 02fb 0405 04fb  ................
-000016a0: 0205 02fb 0205 18fb 0205 02fb 0205 0cfb  ................
-000016b0: 0407 0201 04ff 1e04 0204 0efc 0204 04fc  ................
-000016c0: 0404 06fc 0204 02fc 0204 04fc 0204 02fc  ................
-000016d0: 0404 04fc 0204 02fc 0204 02fc 0204 02fc  ................
-000016e0: 0204 18fc 0204 02fc 0204 14fc 0406 1002  ................
-000016f0: 7244 0000 0063 0000 0000 0000 0000 0000  rD...c..........
-00001700: 0000 0e00 0000 0700 0000 4300 0000 735e  ..........C...s^
-00001710: 0200 0074 00a0 0164 0164 0269 01a1 01a0  ...t...d.d.i....
-00001720: 0264 03a1 017d 0064 047d 017c 007c 016b  .d...}.d.}.|.|.k
-00001730: 027d 027c 0273 4274 03a0 0464 057c 0266  .}.|.sBt...d.|.f
-00001740: 0164 067c 007c 0166 02a1 0464 0774 05a0  .d.|.|.f...d.t..
-00001750: 06a1 0076 0073 2774 03a0 077c 00a1 0172  ...v.s't...|...r
-00001760: 2c74 03a0 087c 00a1 016e 0164 0774 03a0  ,t...|...n.d.t..
-00001770: 087c 01a1 0164 089c 0216 007d 0364 0964  .|...d.....}.d.d
-00001780: 0a7c 0369 0116 007d 0474 0974 03a0 0a7c  .|.i...}.t.t...|
-00001790: 04a1 0183 0182 0164 0004 007d 027d 0174  .......d...}.}.t
-000017a0: 0b7c 0083 017d 0564 0b7d 017c 057c 016b  .|...}.d.}.|.|.k
-000017b0: 027d 027c 0273 8274 03a0 0464 057c 0266  .}.|.s.t...d.|.f
-000017c0: 0164 067c 057c 0166 02a1 0464 0c74 05a0  .d.|.|.f...d.t..
-000017d0: 06a1 0076 0073 6774 03a0 077c 05a1 0172  ...v.sgt...|...r
-000017e0: 6c74 03a0 087c 05a1 016e 0164 0c74 03a0  lt...|...n.d.t..
-000017f0: 087c 01a1 0164 089c 0216 007d 0364 0964  .|...d.....}.d.d
-00001800: 0a7c 0369 0116 007d 0474 0974 03a0 0a7c  .|.i...}.t.t...|
-00001810: 04a1 0183 0182 0164 0004 007d 027d 0174  .......d...}.}.t
-00001820: 0c64 0d64 0e64 0f83 03a0 0d64 1064 11a1  .d.d.d.....d.d..
-00001830: 02a0 0d64 0c7c 05a1 027d 067c 06a0 0ea1  ...d.|...}.|....
-00001840: 007d 0764 127d 017c 077c 016b 027d 027c  .}.d.}.|.|.k.}.|
-00001850: 0273 d074 03a0 0464 057c 0266 0164 067c  .s.t...d.|.f.d.|
-00001860: 077c 0166 02a1 0464 1374 05a0 06a1 0076  .|.f...d.t.....v
-00001870: 0073 b574 03a0 077c 07a1 0172 ba74 03a0  .s.t...|...r.t..
-00001880: 087c 07a1 016e 0164 1374 03a0 087c 01a1  .|...n.d.t...|..
-00001890: 0164 089c 0216 007d 0364 0964 0a7c 0369  .d.....}.d.d.|.i
-000018a0: 0116 007d 0474 0974 03a0 0a7c 04a1 0183  ...}.t.t...|....
-000018b0: 0182 0164 0004 007d 027d 017c 06a0 0f64  ...d...}.}.|...d
-000018c0: 14a1 017d 0864 157d 0164 167d 097c 017c  ...}.d.}.d.}.|.|
-000018d0: 0917 007d 0a7c 087c 0a6b 027d 027c 0290  ...}.|.|.k.}.|..
-000018e0: 0173 1d74 03a0 0464 057c 0266 0164 177c  .s.t...d.|.f.d.|
-000018f0: 087c 0a66 02a1 0464 1874 05a0 06a1 0076  .|.f...d.t.....v
-00001900: 0073 fe74 03a0 077c 08a1 0190 0172 0374  .s.t...|.....r.t
-00001910: 03a0 087c 08a1 016e 0164 1874 03a0 087c  ...|...n.d.t...|
-00001920: 01a1 0174 03a0 087c 09a1 0164 199c 0316  ...t...|...d....
-00001930: 007d 0b64 1a64 1b7c 0b69 0116 007d 0c74  .}.d.d.|.i...}.t
-00001940: 0974 03a0 0a7c 0ca1 0183 0182 0164 0004  .t...|.......d..
-00001950: 007d 0204 007d 0104 007d 097d 0a64 1c7d  .}...}...}.}.d.}
-00001960: 0d7c 06a0 107c 0d7c 08a1 0201 0064 0053  .|...|.|.....d.S
-00001970: 0029 1d4e 5a04 636f 7773 5a04 676f 6f64  .).NZ.cowsZ.good
-00001980: 7a05 7574 662d 3873 1000 0000 7b22 636f  z.utf-8s....{"co
-00001990: 7773 223a 2022 676f 6f64 227d 720c 0000  ws": "good"}r...
-000019a0: 0072 0e00 0000 da04 626f 6479 720f 0000  .r......bodyr...
-000019b0: 0072 1200 0000 7213 0000 0072 3300 0000  .r....r....r3...
-000019c0: 7232 0000 0072 2b00 0000 7231 0000 0072  r2...r+...r1...r
-000019d0: 2d00 0000 722e 0000 0072 2f00 0000 7a9a  -...r....r/...z.
-000019e0: 2872 6571 7565 7374 2d74 6172 6765 7429  (request-target)
-000019f0: 3a20 706f 7374 202f 7061 7468 2f74 6f2f  : post /path/to/
-00001a00: 7265 736f 7572 6365 0a68 6f73 743a 206d  resource.host: m
-00001a10: 7968 6f73 742e 746c 640a 6461 7465 3a20  yhost.tld.date: 
-00001a20: 5765 642c 2031 3520 4d61 7220 3230 3233  Wed, 15 Mar 2023
-00001a30: 2031 373a 3238 3a31 3520 474d 540a 6469   17:28:15 GMT.di
-00001a40: 6765 7374 3a20 7368 612d 3235 363d 4d49  gest: sha-256=MI
-00001a50: 4c62 356c 5544 4436 5a30 7044 5378 6867  Lb5lUDD6Z0pDSxhg
-00001a60: 786a 2b68 4d42 4577 3075 547a 5033 6732  xj+hMBEw0uTzP3g2
-00001a70: 7155 4a47 484d 7039 6b3d 7235 0000 0072  qUJGHMp9k=r5...r
-00001a80: 3600 0000 5a33 7a34 7650 6b4a 616f 6153  6...Z3z4vPkJaoaS
-00001a90: 5651 7035 4472 4d62 3845 7643 616a 4a63  VQp5DrMb8EvCajJc
-00001aa0: 6572 5733 3672 7379 5744 454c 5457 5133  erW36rsyWDELTWQ3
-00001ab0: 6359 6d61 6f6e 6e47 665a 2662 3857 4869  cYmaonnGfZ&b8WHi
-00001ac0: 7748 3534 4253 6869 6443 636d 706f 7948  wH54BShidCcmpoyH
-00001ad0: 6a61 6e56 5259 4e72 5858 586b 6134 6a41  janVRYNrXXXka4jA
-00001ae0: 6e72 3700 0000 7217 0000 0072 3800 0000  nr7...r....r8...
-00001af0: 7239 0000 0072 3a00 0000 723b 0000 0029  r9...r:...r;...)
-00001b00: 11da 046a 736f 6eda 0564 756d 7073 da06  ...json..dumps..
-00001b10: 656e 636f 6465 721a 0000 0072 1b00 0000  encoder....r....
-00001b20: 721c 0000 0072 1d00 0000 721e 0000 0072  r....r....r....r
-00001b30: 1f00 0000 7220 0000 0072 2100 0000 7203  ....r ...r!...r.
-00001b40: 0000 0072 0500 0000 7218 0000 0072 3c00  ...r....r....r<.
-00001b50: 0000 723d 0000 0072 3e00 0000 290e 7245  ..r=...r>...).rE
-00001b60: 0000 0072 2400 0000 7225 0000 0072 2600  ...r$...r%...r&.
-00001b70: 0000 7227 0000 0072 3200 0000 7222 0000  ..r'...r2...r"..
-00001b80: 0072 3500 0000 7217 0000 0072 3f00 0000  .r5...r....r?...
-00001b90: 7240 0000 0072 4100 0000 7242 0000 0072  r@...rA...rB...r
-00001ba0: 4300 0000 7228 0000 0072 2800 0000 7229  C...r(...r(...r)
-00001bb0: 0000 00da 1774 6573 745f 6275 696c 645f  .....test_build_
-00001bc0: 6d65 7373 6167 655f 706f 7374 5b00 0000  message_post[...
-00001bd0: 7380 0000 0014 0178 0208 0278 020a 0308  s......x...x....
-00001be0: 0108 0102 fd08 0612 0202 060e fa02 0604  ................
-00001bf0: fa04 0606 fa02 0602 fa02 0604 fa02 0602  ................
-00001c00: fa04 0604 fa02 0602 fa02 0618 fa02 0602  ................
-00001c10: fa02 060c fa04 0802 0104 ff20 0402 040e  ........... ....
-00001c20: fc02 0404 fc04 0406 fc02 0402 fc02 0406  ................
-00001c30: fc02 0402 fc04 0404 fc02 0402 fc02 0402  ................
-00001c40: fc02 0402 fc02 0418 fc02 0402 fc02 0414  ................
-00001c50: fc04 0610 0272 4900 0000 2913 da08 6275  .....rI...)...bu
-00001c60: 696c 7469 6e73 721c 0000 00da 195f 7079  iltinsr......_py
-00001c70: 7465 7374 2e61 7373 6572 7469 6f6e 2e72  test.assertion.r
-00001c80: 6577 7269 7465 da09 6173 7365 7274 696f  ewrite..assertio
-00001c90: 6eda 0772 6577 7269 7465 721a 0000 0072  n..rewriter....r
-00001ca0: 4600 0000 da06 6865 6c70 6572 7203 0000  F.....helperr...
-00001cb0: 0072 2200 0000 7204 0000 0072 0500 0000  .r"...r....r....
-00001cc0: da04 7465 7374 7206 0000 0072 2a00 0000  ..testr....r*...
-00001cd0: 7230 0000 0072 3400 0000 7244 0000 0072  r0...r4...rD...r
-00001ce0: 4900 0000 7228 0000 0072 2800 0000 7228  I...r(...r(...r(
-00001cf0: 0000 0072 2900 0000 da08 3c6d 6f64 756c  ...r).....<modul
-00001d00: 653e 0100 0000 7312 0000 0022 000c 0210  e>....s...."....
-00001d10: 010c 0108 0308 1008 1708 0f0c 1d         .............
+00000670: 6572 672e 6f72 672f 626f 7669 6e65 2f62  erg.org/bovine/b
+00000680: 6f76 696e 652f 626f 7669 6e65 2f62 6f76  ovine/bovine/bov
+00000690: 696e 652f 6372 7970 746f 2f74 6573 745f  ine/crypto/test_
+000006a0: 6874 7470 5f73 6967 6e61 7475 7265 2e70  http_signature.p
+000006b0: 79da 1374 6573 745f 6874 7470 5f73 6967  y..test_http_sig
+000006c0: 6e61 7475 7265 0800 0000 733a 0000 000e  nature....s:....
+000006d0: 010c 0212 0278 0278 0178 0114 0102 030e  .....x.x.x......
+000006e0: fd02 0304 fd04 0306 fd02 0302 fd02 0304  ................
+000006f0: fd02 0302 fd04 0304 fd02 0302 fd02 0318  ................
+00000700: fd02 0302 fd02 0310 fd72 2a00 0000 6300  .........r*...c.
+00000710: 0000 0000 0000 0000 0000 000a 0000 0007  ................
+00000720: 0000 0043 0000 0073 9a02 0000 7400 6401  ...C...s....t.d.
+00000730: 6402 6403 8303 a001 6404 6405 a102 0400  d.d.....d.d.....
+00000740: 7d00 7d00 7c00 a000 6406 7402 a102 7d01  }.}.|...d.t...}.
+00000750: 6407 7d02 7c01 7c02 6b02 7d03 7c03 734a  d.}.|.|.k.}.|.sJ
+00000760: 7403 a004 6408 7c03 6601 6409 7c01 7c02  t...d.|.f.d.|.|.
+00000770: 6602 a104 640a 7405 a006 a100 7600 732f  f...d.t.....v.s/
+00000780: 7403 a007 7c01 a101 7234 7403 a008 7c01  t...|...r4t...|.
+00000790: a101 6e01 640a 7403 a008 7c02 a101 640b  ..n.d.t...|...d.
+000007a0: 9c02 1600 7d04 640c 640d 7c04 6901 1600  ....}.d.d.|.i...
+000007b0: 7d05 7409 7403 a00a 7c05 a101 8301 8201  }.t.t...|.......
+000007c0: 6400 0400 7d03 7d02 7c01 a00b 640e a101  d...}.}.|...d...
+000007d0: 5c04 7d06 7d07 7d08 7d09 640f 7d02 7c06  \.}.}.}.}.d.}.|.
+000007e0: 7c02 6b02 7d03 7c03 738f 7403 a004 6408  |.k.}.|.s.t...d.
+000007f0: 7c03 6601 6409 7c06 7c02 6602 a104 6406  |.f.d.|.|.f...d.
+00000800: 7405 a006 a100 7600 7374 7403 a007 7c06  t.....v.stt...|.
+00000810: a101 7279 7403 a008 7c06 a101 6e01 6406  ..ryt...|...n.d.
+00000820: 7403 a008 7c02 a101 640b 9c02 1600 7d04  t...|...d.....}.
+00000830: 640c 640d 7c04 6901 1600 7d05 7409 7403  d.d.|.i...}.t.t.
+00000840: a00a 7c05 a101 8301 8201 6400 0400 7d03  ..|.......d...}.
+00000850: 7d02 6410 7d02 7c07 7c02 6b02 7d03 7c03  }.d.}.|.|.k.}.|.
+00000860: 73cb 7403 a004 6408 7c03 6601 6409 7c07  s.t...d.|.f.d.|.
+00000870: 7c02 6602 a104 6411 7405 a006 a100 7600  |.f...d.t.....v.
+00000880: 73b0 7403 a007 7c07 a101 72b5 7403 a008  s.t...|...r.t...
+00000890: 7c07 a101 6e01 6411 7403 a008 7c02 a101  |...n.d.t...|...
+000008a0: 640b 9c02 1600 7d04 640c 640d 7c04 6901  d.....}.d.d.|.i.
+000008b0: 1600 7d05 7409 7403 a00a 7c05 a101 8301  ..}.t.t...|.....
+000008c0: 8201 6400 0400 7d03 7d02 6412 7d02 7c08  ..d...}.}.d.}.|.
+000008d0: 7c02 6b02 7d03 7c03 9001 7308 7403 a004  |.k.}.|...s.t...
+000008e0: 6408 7c03 6601 6409 7c08 7c02 6602 a104  d.|.f.d.|.|.f...
+000008f0: 6413 7405 a006 a100 7600 73ed 7403 a007  d.t.....v.s.t...
+00000900: 7c08 a101 72f2 7403 a008 7c08 a101 6e01  |...r.t...|...n.
+00000910: 6413 7403 a008 7c02 a101 640b 9c02 1600  d.t...|...d.....
+00000920: 7d04 640c 640d 7c04 6901 1600 7d05 7409  }.d.d.|.i...}.t.
+00000930: 7403 a00a 7c05 a101 8301 8201 6400 0400  t...|.......d...
+00000940: 7d03 7d02 6414 7d02 7c09 7c02 6b02 7d03  }.}.d.}.|.|.k.}.
+00000950: 7c03 9001 7347 7403 a004 6408 7c03 6601  |...sGt...d.|.f.
+00000960: 6409 7c09 7c02 6602 a104 6415 7405 a006  d.|.|.f...d.t...
+00000970: a100 7600 9001 732c 7403 a007 7c09 a101  ..v...s,t...|...
+00000980: 9001 7231 7403 a008 7c09 a101 6e01 6415  ..r1t...|...n.d.
+00000990: 7403 a008 7c02 a101 640b 9c02 1600 7d04  t...|...d.....}.
+000009a0: 640c 640d 7c04 6901 1600 7d05 7409 7403  d.d.|.i...}.t.t.
+000009b0: a00a 7c05 a101 8301 8201 6400 0400 7d03  ..|.......d...}.
+000009c0: 7d02 6400 5300 2916 4efa 0a6d 7968 6f73  }.d.S.).N..myhos
+000009d0: 742e 746c 64da 0367 6574 fa11 2f70 6174  t.tld..get../pat
+000009e0: 682f 746f 2f72 6573 6f75 7263 65da 0464  h/to/resource..d
+000009f0: 6174 65fa 1d57 6564 2c20 3135 204d 6172  ate..Wed, 15 Mar
+00000a00: 2032 3032 3320 3137 3a32 383a 3135 2047   2023 17:28:15 G
+00000a10: 4d54 7209 0000 0061 af01 0000 6b65 7949  MTr....a....keyI
+00000a20: 643d 226b 6579 5f69 6422 2c61 6c67 6f72  d="key_id",algor
+00000a30: 6974 686d 3d22 7273 612d 7368 6132 3536  ithm="rsa-sha256
+00000a40: 222c 6865 6164 6572 733d 2228 7265 7175  ",headers="(requ
+00000a50: 6573 742d 7461 7267 6574 2920 686f 7374  est-target) host
+00000a60: 2064 6174 6522 2c73 6967 6e61 7475 7265   date",signature
+00000a70: 3d22 6277 6741 3355 616a 7044 7a4d 3037  ="bwgA3UajpDzM07
+00000a80: 774d 2b4d 556b 7047 4853 2f6d 4168 6854  wM+MUkpGHS/mAhhT
+00000a90: 752b 5744 6942 4c31 4832 384a 3736 326a  u+WDiBL1H28J762j
+00000aa0: 5555 7567 677a 5038 5765 352b 4930 5748  UUuggzP8We5+I0WH
+00000ab0: 7970 5342 4357 7438 4c61 7032 4162 5971  ypSBCWt8Lap2AbYq
+00000ac0: 4736 5066 5473 6446 4562 6b38 5657 6577  G6PfTsdFEbk8VWew
+00000ad0: 5833 346e 372f 4c55 534d 2f57 4a65 4138  X34n7/LUSM/WJeA8
+00000ae0: 4146 4345 6e48 5950 6438 7252 6962 3464  AFCEnHYPd8rRib4d
+00000af0: 302b 6b51 562b 5534 4169 3939 3758 5578  0+kQV+U4Ai997XUx
+00000b00: 7332 7869 3241 7275 4e64 6b42 3653 4e4d  s2xi2AruNdkB6SNM
+00000b10: 6b53 626e 514c 6f42 6a59 5434 747a 4761  kSbnQLoBjYT4tzGa
+00000b20: 6632 4931 785a 7571 6a44 3148 7676 5730  f2I1xZuqjD1HvvW0
+00000b30: 7861 316f 2f6e 5074 3447 356b 6a30 7456  xa1o/nPt4G5kj0tV
+00000b40: 6d67 4472 7267 654b 4c32 6855 4a32 3155  mgDrrgeKL2hUJ21U
+00000b50: 6448 6358 444e 4677 3951 4a57 662f 4f36  dHcXDNFw9QJWf/O6
+00000b60: 4b79 456d 6275 6d76 7070 4b47 4655 6664  KyEmbumvppKGFUfd
+00000b70: 704b 5368 336e 322f 6650 374f 3442 7871  pKSh3n2/fP7O4Bxq
+00000b80: 6164 4362 4d59 6a30 6f44 444f 4631 4833  adCbMYj0oDDOF1H3
+00000b90: 5061 3647 5639 4566 4965 5358 584c 5339  Pa6GV9EfIeSXXLS9
+00000ba0: 5466 7950 706b 5877 6257 724e 707a 5542  TfyPpkXwbWrNpzUB
+00000bb0: 5a51 3268 5247 7a58 326a 532f 4a45 6870  ZQ2hRGzX2jS/JEhp
+00000bc0: 534e 5356 7176 3641 3d3d 2272 0c00 0000  SNSVqv6A=="r....
+00000bd0: 720e 0000 0072 2300 0000 720f 0000 0072  r....r#...r....r
+00000be0: 1200 0000 7213 0000 0072 0a00 0000 720b  ....r....r....r.
+00000bf0: 0000 0072 1400 0000 7215 0000 007a 2468  ...r....r....z$h
+00000c00: 6561 6465 7273 3d22 2872 6571 7565 7374  eaders="(request
+00000c10: 2d74 6172 6765 7429 2068 6f73 7420 6461  -target) host da
+00000c20: 7465 2272 1600 0000 6164 0100 0073 6967  te"r....ad...sig
+00000c30: 6e61 7475 7265 3d22 6277 6741 3355 616a  nature="bwgA3Uaj
+00000c40: 7044 7a4d 3037 774d 2b4d 556b 7047 4853  pDzM07wM+MUkpGHS
+00000c50: 2f6d 4168 6854 752b 5744 6942 4c31 4832  /mAhhTu+WDiBL1H2
+00000c60: 384a 3736 326a 5555 7567 677a 5038 5765  8J762jUUuggzP8We
+00000c70: 352b 4930 5748 7970 5342 4357 7438 4c61  5+I0WHypSBCWt8La
+00000c80: 7032 4162 5971 4736 5066 5473 6446 4562  p2AbYqG6PfTsdFEb
+00000c90: 6b38 5657 6577 5833 346e 372f 4c55 534d  k8VWewX34n7/LUSM
+00000ca0: 2f57 4a65 4138 4146 4345 6e48 5950 6438  /WJeA8AFCEnHYPd8
+00000cb0: 7252 6962 3464 302b 6b51 562b 5534 4169  rRib4d0+kQV+U4Ai
+00000cc0: 3939 3758 5578 7332 7869 3241 7275 4e64  997XUxs2xi2AruNd
+00000cd0: 6b42 3653 4e4d 6b53 626e 514c 6f42 6a59  kB6SNMkSbnQLoBjY
+00000ce0: 5434 747a 4761 6632 4931 785a 7571 6a44  T4tzGaf2I1xZuqjD
+00000cf0: 3148 7676 5730 7861 316f 2f6e 5074 3447  1HvvW0xa1o/nPt4G
+00000d00: 356b 6a30 7456 6d67 4472 7267 654b 4c32  5kj0tVmgDrrgeKL2
+00000d10: 6855 4a32 3155 6448 6358 444e 4677 3951  hUJ21UdHcXDNFw9Q
+00000d20: 4a57 662f 4f36 4b79 456d 6275 6d76 7070  JWf/O6KyEmbumvpp
+00000d30: 4b47 4655 6664 704b 5368 336e 322f 6650  KGFUfdpKSh3n2/fP
+00000d40: 374f 3442 7871 6164 4362 4d59 6a30 6f44  7O4BxqadCbMYj0oD
+00000d50: 444f 4631 4833 5061 3647 5639 4566 4965  DOF1H3Pa6GV9EfIe
+00000d60: 5358 584c 5339 5466 7950 706b 5877 6257  SXXLS9TfyPpkXwbW
+00000d70: 724e 707a 5542 5a51 3268 5247 7a58 326a  rNpzUBZQ2hRGzX2j
+00000d80: 532f 4a45 6870 534e 5356 7176 3641 3d3d  S/JEhpSNSVqv6A==
+00000d90: 2272 1700 0000 290c 7205 0000 0072 1800  "r....).r....r..
+00000da0: 0000 7206 0000 0072 1a00 0000 721b 0000  ..r....r....r...
+00000db0: 0072 1c00 0000 721d 0000 0072 1e00 0000  .r....r....r....
+00000dc0: 721f 0000 0072 2000 0000 7221 0000 0072  r....r ...r!...r
+00000dd0: 1900 0000 290a 7222 0000 0072 2300 0000  ....).r"...r#...
+00000de0: 7224 0000 0072 2500 0000 7226 0000 0072  r$...r%...r&...r
+00000df0: 2700 0000 7209 0000 0072 1500 0000 7216  '...r....r....r.
+00000e00: 0000 0072 1700 0000 7228 0000 0072 2800  ...r....r(...r(.
+00000e10: 0000 7229 0000 00da 1474 6573 745f 6275  ..r).....test_bu
+00000e20: 696c 645f 7369 676e 6174 7572 6518 0000  ild_signature...
+00000e30: 0073 7000 0000 0201 0601 02ff 0802 06fe  .sp.............
+00000e40: 0c04 1202 0203 0efd 0203 04fd 0403 06fd  ................
+00000e50: 0203 02fd 0203 04fd 0203 02fd 0403 04fd  ................
+00000e60: 0203 02fd 0203 18fd 0203 02fd 0203 0cfd  ................
+00000e70: 1205 7802 7801 7a01 1401 0203 0efd 0203  ..x.x.z.........
+00000e80: 04fd 0403 08fd 0203 02fd 0203 06fd 0203  ................
+00000e90: 02fd 0403 04fd 0203 02fd 0203 18fd 0203  ................
+00000ea0: 02fd 0203 10fd 7230 0000 0063 0000 0000  ......r0...c....
+00000eb0: 0000 0000 0000 0000 0600 0000 0700 0000  ................
+00000ec0: 4300 0000 73a8 0000 0074 0064 0164 0264  C...s....t.d.d.d
+00000ed0: 0383 03a0 0164 0464 05a1 02a0 0164 0664  .....d.d.....d.d
+00000ee0: 07a1 0204 007d 007d 007c 00a0 0064 0874  .....}.}.|...d.t
+00000ef0: 02a1 027d 0164 097d 027c 017c 026b 027d  ...}.d.}.|.|.k.}
+00000f00: 037c 0373 4e74 03a0 0464 0a7c 0366 0164  .|.sNt...d.|.f.d
+00000f10: 0b7c 017c 0266 02a1 0464 0c74 05a0 06a1  .|.|.f...d.t....
+00000f20: 0076 0073 3374 03a0 077c 01a1 0172 3874  .v.s3t...|...r8t
+00000f30: 03a0 087c 01a1 016e 0164 0c74 03a0 087c  ...|...n.d.t...|
+00000f40: 02a1 0164 0d9c 0216 007d 0464 0e64 0f7c  ...d.....}.d.d.|
+00000f50: 0469 0116 007d 0574 0974 03a0 0a7c 05a1  .i...}.t.t...|..
+00000f60: 0183 0182 0164 0004 007d 037d 0264 0053  .....d...}.}.d.S
+00000f70: 0029 104e 722b 0000 00da 0470 6f73 7472  .).Nr+.....postr
+00000f80: 2d00 0000 722e 0000 0072 2f00 0000 da06  -...r....r/.....
+00000f90: 6469 6765 7374 fa34 7368 612d 3235 363d  digest.4sha-256=
+00000fa0: 4d49 4c62 356c 5544 4436 5a30 7044 5378  MILb5lUDD6Z0pDSx
+00000fb0: 6867 786a 2b68 4d42 4577 3075 547a 5033  hgxj+hMBEw0uTzP3
+00000fc0: 6732 7155 4a47 484d 7039 6b3d 7209 0000  g2qUJGHMp9k=r...
+00000fd0: 0061 b601 0000 6b65 7949 643d 226b 6579  .a....keyId="key
+00000fe0: 5f69 6422 2c61 6c67 6f72 6974 686d 3d22  _id",algorithm="
+00000ff0: 7273 612d 7368 6132 3536 222c 6865 6164  rsa-sha256",head
+00001000: 6572 733d 2228 7265 7175 6573 742d 7461  ers="(request-ta
+00001010: 7267 6574 2920 686f 7374 2064 6174 6520  rget) host date 
+00001020: 6469 6765 7374 222c 7369 676e 6174 7572  digest",signatur
+00001030: 653d 2251 7065 4c4d 4568 2f5a 3030 3944  e="QpeLMEh/Z009D
+00001040: 6759 6353 4f6b 7273 4b72 397a 5737 5775  gYcSOkrsKr9zW7Wu
+00001050: 3755 5754 5133 3938 7176 7565 437a 6145  7UWTQ398qvueCzaE
+00001060: 4c2f 4878 7276 3943 3432 552b 5759 2f4f  L/Hxrv9C42U+WY/O
+00001070: 3334 782f 3338 356c 542b 7a31 4933 426b  34x/385lT+z1I3Bk
+00001080: 3671 4d5a 5444 415a 536d 4b47 5942 356c  6qMZTDAZSmKGYB5l
+00001090: 5a4a 5642 6443 3230 6134 442b 2b48 7a49  ZJVBdC20a4D++HzI
+000010a0: 7945 3632 6436 4376 7155 7351 7749 7634  yE62d6CvqUsQwIv4
+000010b0: 6f64 2f68 4f6d 6d4f 5133 484b 4936 394d  od/hOmmOQ3HKI69M
+000010c0: 554f 734e 724c 796a 4951 7855 614c 5342  UOsNrLyjIQxUaLSB
+000010d0: 7a31 6d2f 776b 4c76 3869 4d72 6839 5177  z1m/wkLv8iMrh9Qw
+000010e0: 554c 6c71 544f 3857 4856 6a53 4a6c 6756  ULlqTO8WHVjSJlgV
+000010f0: 776c 6c52 744f 4f63 6d33 777a 6f2f 6372  wllRtOOcm3wzo/cr
+00001100: 3258 7946 6a34 6742 3843 5564 3361 4733  2XyFj4gB8CUd3aG3
+00001110: 6471 7a43 664f 4f6f 4e51 7655 684d 446c  dqzCfOOoNQvUhMDl
+00001120: 7850 3755 7142 6e47 6f46 3670 6e59 6e54  xP7UqBnGoF6pnYnT
+00001130: 6e4a 5553 5348 6463 6557 6245 3039 5471  nJUSSHdceWbE09Tq
+00001140: 584c 6d41 487a 6175 5947 5364 6148 5253  XLmAHzauYGSdaHRS
+00001150: 3358 522f 536a 6537 4554 3955 614f 6748  3XR/Sje7ET9UaOgH
+00001160: 4863 504a 4849 4e2b 346a 7242 7044 7032  HcPJHIN+4jrBpDp2
+00001170: 474d 3639 6a6f 5857 6b5a 7768 4530 474f  GM69joXWkZwhE0GO
+00001180: 6c39 7133 4b42 534b 413d 3d22 720c 0000  l9q3KBSKA=="r...
+00001190: 0072 0e00 0000 7223 0000 0072 0f00 0000  .r....r#...r....
+000011a0: 7212 0000 0072 1300 0000 290b 7205 0000  r....r....).r...
+000011b0: 0072 1800 0000 7206 0000 0072 1a00 0000  .r....r....r....
+000011c0: 721b 0000 0072 1c00 0000 721d 0000 0072  r....r....r....r
+000011d0: 1e00 0000 721f 0000 0072 2000 0000 7221  ....r....r ...r!
+000011e0: 0000 0029 0672 2200 0000 7223 0000 0072  ...).r"...r#...r
+000011f0: 2400 0000 7225 0000 0072 2600 0000 7227  $...r%...r&...r'
+00001200: 0000 0072 2800 0000 7228 0000 0072 2900  ...r(...r(...r).
+00001210: 0000 da19 7465 7374 5f62 7569 6c64 5f73  ....test_build_s
+00001220: 6967 6e61 7475 7265 5f70 6f73 742f 0000  ignature_post/..
+00001230: 0073 3800 0000 0a02 0801 0801 06fd 0c06  .s8.............
+00001240: 1202 0203 0efd 0203 04fd 0403 06fd 0203  ................
+00001250: 02fd 0203 04fd 0203 02fd 0403 04fd 0203  ................
+00001260: 02fd 0203 18fd 0203 02fd 0203 10fd 7234  ..............r4
+00001270: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+00001280: 0c00 0000 0700 0000 4300 0000 7346 0100  ........C...sF..
+00001290: 0074 0064 0164 0264 0383 03a0 0164 0464  .t.d.d.d.....d.d
+000012a0: 05a1 027d 007c 00a0 02a1 007d 0164 067d  ...}.|.....}.d.}
+000012b0: 027c 017c 026b 027d 037c 0373 4674 03a0  .|.|.k.}.|.sFt..
+000012c0: 0464 077c 0366 0164 087c 017c 0266 02a1  .d.|.f.d.|.|.f..
+000012d0: 0464 0974 05a0 06a1 0076 0073 2b74 03a0  .d.t.....v.s+t..
+000012e0: 077c 01a1 0172 3074 03a0 087c 01a1 016e  .|...r0t...|...n
+000012f0: 0164 0974 03a0 087c 02a1 0164 0a9c 0216  .d.t...|...d....
+00001300: 007d 0464 0b64 0c7c 0469 0116 007d 0574  .}.d.d.|.i...}.t
+00001310: 0974 03a0 0a7c 05a1 0183 0182 0164 0004  .t...|.......d..
+00001320: 007d 037d 027c 00a0 0b64 0da1 017d 0664  .}.}.|...d...}.d
+00001330: 0e7d 0264 0f7d 077c 027c 0717 007d 087c  .}.d.}.|.|...}.|
+00001340: 067c 086b 027d 037c 0373 9174 03a0 0464  .|.k.}.|.s.t...d
+00001350: 077c 0366 0164 107c 067c 0866 02a1 0464  .|.f.d.|.|.f...d
+00001360: 1174 05a0 06a1 0076 0073 7274 03a0 077c  .t.....v.srt...|
+00001370: 06a1 0172 7774 03a0 087c 06a1 016e 0164  ...rwt...|...n.d
+00001380: 1174 03a0 087c 02a1 0174 03a0 087c 07a1  .t...|...t...|..
+00001390: 0164 129c 0316 007d 0964 1364 147c 0969  .d.....}.d.d.|.i
+000013a0: 0116 007d 0a74 0974 03a0 0a7c 0aa1 0183  ...}.t.t...|....
+000013b0: 0182 0164 0004 007d 0304 007d 0204 007d  ...d...}...}...}
+000013c0: 077d 0864 157d 0b7c 00a0 0c7c 0b7c 06a1  .}.d.}.|...|.|..
+000013d0: 0201 0064 0053 0029 164e 722b 0000 0072  ...d.S.).Nr+...r
+000013e0: 2c00 0000 722d 0000 0072 2e00 0000 722f  ,...r-...r....r/
+000013f0: 0000 007a 5c28 7265 7175 6573 742d 7461  ...z\(request-ta
+00001400: 7267 6574 293a 2067 6574 202f 7061 7468  rget): get /path
+00001410: 2f74 6f2f 7265 736f 7572 6365 0a68 6f73  /to/resource.hos
+00001420: 743a 206d 7968 6f73 742e 746c 640a 6461  t: myhost.tld.da
+00001430: 7465 3a20 5765 642c 2031 3520 4d61 7220  te: Wed, 15 Mar 
+00001440: 3230 3233 2031 373a 3238 3a31 3520 474d  2023 17:28:15 GM
+00001450: 5472 0c00 0000 720e 0000 00da 076d 6573  Tr....r......mes
+00001460: 7361 6765 720f 0000 0072 1200 0000 7213  sager....r....r.
+00001470: 0000 00da 307a 3375 3259 7863 6f77 7361  ....0z3u2Yxcowsa
+00001480: 7265 7468 6562 6573 7463 6f77 7361 7265  rethebestcowsare
+00001490: 7468 6562 6573 7463 6f77 7361 7265 7468  thebestcowsareth
+000014a0: 6562 6573 745a 2e7a 3561 6864 4843 6250  ebestZ.z5ahdHCbP
+000014b0: 3961 4a45 7344 7476 4731 4d45 5a70 7850  9aJEsDtvG1MEZpxP
+000014c0: 7a75 7647 4b59 6364 5864 4b76 4d71 3559  zuvGKYcdXdKvMq5Y
+000014d0: 4c32 315a 325a 2b75 6d78 6a73 3153 6f70  L21Z2Z+umxjs1Sop
+000014e0: 4359 3241 7038 765a 7856 6a54 4566 3664  CY2Ap8vZxVjTEf6d
+000014f0: 5962 4775 4237 6d74 6763 6755 794e 6442  YbGuB7mtgcgUyNdB
+00001500: 4c65 a901 7a1e 2528 7079 3029 7320 3d3d  Le..z.%(py0)s ==
+00001510: 2028 2528 7079 3329 7320 2b20 2528 7079   (%(py3)s + %(py
+00001520: 3529 7329 7217 0000 00a9 0372 1000 0000  5)s)r......r....
+00001530: 7211 0000 0072 1300 0000 fa0e 6173 7365  r....r......asse
+00001540: 7274 2025 2870 7938 2973 da03 7079 38fa  rt %(py8)s..py8.
+00001550: 3864 6964 3a6b 6579 3a7a 364d 6b65 6b77  8did:key:z6Mkekw
+00001560: 4336 5239 626a 3945 7254 6f42 3741 695a  C6R9bj9ErToB7AiZ
+00001570: 4a66 7943 5344 6861 5a65 3155 7868 4462  JfyCSDhaZe1UxhDb
+00001580: 4371 4a72 6871 7053 3529 0d72 0500 0000  CqJrhqpS5).r....
+00001590: 7218 0000 00da 0d62 7569 6c64 5f6d 6573  r......build_mes
+000015a0: 7361 6765 721a 0000 0072 1b00 0000 721c  sager....r....r.
+000015b0: 0000 0072 1d00 0000 721e 0000 0072 1f00  ...r....r....r..
+000015c0: 0000 7220 0000 0072 2100 0000 da0c 6564  ..r ...r!.....ed
+000015d0: 3235 3531 395f 7369 676e da0e 6564 3235  25519_sign..ed25
+000015e0: 3531 395f 7665 7269 6679 290c 7222 0000  519_verify).r"..
+000015f0: 0072 3500 0000 7224 0000 0072 2500 0000  .r5...r$...r%...
+00001600: 7226 0000 0072 2700 0000 7217 0000 00da  r&...r'...r.....
+00001610: 0b40 7079 5f61 7373 6572 7434 da0b 4070  .@py_assert4..@p
+00001620: 795f 6173 7365 7274 36da 0b40 7079 5f66  y_assert6..@py_f
+00001630: 6f72 6d61 7437 da0b 4070 795f 666f 726d  ormat7..@py_form
+00001640: 6174 39da 0664 6964 6b65 7972 2800 0000  at9..didkeyr(...
+00001650: 7228 0000 0072 2900 0000 da12 7465 7374  r(...r).....test
+00001660: 5f62 7569 6c64 5f6d 6573 7361 6765 3e00  _build_message>.
+00001670: 0000 737a 0000 0002 0106 0102 ff08 0202  ..sz............
+00001680: fe08 0412 0202 050e fb02 0504 fb04 0506  ................
+00001690: fb02 0502 fb02 0504 fb02 0502 fb04 0504  ................
+000016a0: fb02 0502 fb02 0518 fb02 0502 fb02 050c  ................
+000016b0: fb04 0702 0104 ff1e 0402 040e fc02 0404  ................
+000016c0: fc04 0406 fc02 0402 fc02 0404 fc02 0402  ................
+000016d0: fc04 0404 fc02 0402 fc02 0402 fc02 0402  ................
+000016e0: fc02 0418 fc02 0402 fc02 0414 fc04 0610  ................
+000016f0: 0272 4400 0000 6300 0000 0000 0000 0000  .rD...c.........
+00001700: 0000 000e 0000 0007 0000 0043 0000 0073  ...........C...s
+00001710: 5e02 0000 7400 a001 6401 6402 6901 a101  ^...t...d.d.i...
+00001720: a002 6403 a101 7d00 6404 7d01 7c00 7c01  ..d...}.d.}.|.|.
+00001730: 6b02 7d02 7c02 7342 7403 a004 6405 7c02  k.}.|.sBt...d.|.
+00001740: 6601 6406 7c00 7c01 6602 a104 6407 7405  f.d.|.|.f...d.t.
+00001750: a006 a100 7600 7327 7403 a007 7c00 a101  ....v.s't...|...
+00001760: 722c 7403 a008 7c00 a101 6e01 6407 7403  r,t...|...n.d.t.
+00001770: a008 7c01 a101 6408 9c02 1600 7d03 6409  ..|...d.....}.d.
+00001780: 640a 7c03 6901 1600 7d04 7409 7403 a00a  d.|.i...}.t.t...
+00001790: 7c04 a101 8301 8201 6400 0400 7d02 7d01  |.......d...}.}.
+000017a0: 740b 7c00 8301 7d05 640b 7d01 7c05 7c01  t.|...}.d.}.|.|.
+000017b0: 6b02 7d02 7c02 7382 7403 a004 6405 7c02  k.}.|.s.t...d.|.
+000017c0: 6601 6406 7c05 7c01 6602 a104 640c 7405  f.d.|.|.f...d.t.
+000017d0: a006 a100 7600 7367 7403 a007 7c05 a101  ....v.sgt...|...
+000017e0: 726c 7403 a008 7c05 a101 6e01 640c 7403  rlt...|...n.d.t.
+000017f0: a008 7c01 a101 6408 9c02 1600 7d03 6409  ..|...d.....}.d.
+00001800: 640a 7c03 6901 1600 7d04 7409 7403 a00a  d.|.i...}.t.t...
+00001810: 7c04 a101 8301 8201 6400 0400 7d02 7d01  |.......d...}.}.
+00001820: 740c 640d 640e 640f 8303 a00d 6410 6411  t.d.d.d.....d.d.
+00001830: a102 a00d 640c 7c05 a102 7d06 7c06 a00e  ....d.|...}.|...
+00001840: a100 7d07 6412 7d01 7c07 7c01 6b02 7d02  ..}.d.}.|.|.k.}.
+00001850: 7c02 73d0 7403 a004 6405 7c02 6601 6406  |.s.t...d.|.f.d.
+00001860: 7c07 7c01 6602 a104 6413 7405 a006 a100  |.|.f...d.t.....
+00001870: 7600 73b5 7403 a007 7c07 a101 72ba 7403  v.s.t...|...r.t.
+00001880: a008 7c07 a101 6e01 6413 7403 a008 7c01  ..|...n.d.t...|.
+00001890: a101 6408 9c02 1600 7d03 6409 640a 7c03  ..d.....}.d.d.|.
+000018a0: 6901 1600 7d04 7409 7403 a00a 7c04 a101  i...}.t.t...|...
+000018b0: 8301 8201 6400 0400 7d02 7d01 7c06 a00f  ....d...}.}.|...
+000018c0: 6414 a101 7d08 6415 7d01 6416 7d09 7c01  d...}.d.}.d.}.|.
+000018d0: 7c09 1700 7d0a 7c08 7c0a 6b02 7d02 7c02  |...}.|.|.k.}.|.
+000018e0: 9001 731d 7403 a004 6405 7c02 6601 6417  ..s.t...d.|.f.d.
+000018f0: 7c08 7c0a 6602 a104 6418 7405 a006 a100  |.|.f...d.t.....
+00001900: 7600 73fe 7403 a007 7c08 a101 9001 7203  v.s.t...|.....r.
+00001910: 7403 a008 7c08 a101 6e01 6418 7403 a008  t...|...n.d.t...
+00001920: 7c01 a101 7403 a008 7c09 a101 6419 9c03  |...t...|...d...
+00001930: 1600 7d0b 641a 641b 7c0b 6901 1600 7d0c  ..}.d.d.|.i...}.
+00001940: 7409 7403 a00a 7c0c a101 8301 8201 6400  t.t...|.......d.
+00001950: 0400 7d02 0400 7d01 0400 7d09 7d0a 641c  ..}...}...}.}.d.
+00001960: 7d0d 7c06 a010 7c0d 7c08 a102 0100 6400  }.|...|.|.....d.
+00001970: 5300 291d 4e5a 0463 6f77 735a 0467 6f6f  S.).NZ.cowsZ.goo
+00001980: 647a 0575 7466 2d38 7310 0000 007b 2263  dz.utf-8s....{"c
+00001990: 6f77 7322 3a20 2267 6f6f 6422 7d72 0c00  ows": "good"}r..
+000019a0: 0000 720e 0000 00da 0462 6f64 7972 0f00  ..r......bodyr..
+000019b0: 0000 7212 0000 0072 1300 0000 7233 0000  ..r....r....r3..
+000019c0: 0072 3200 0000 722b 0000 0072 3100 0000  .r2...r+...r1...
+000019d0: 722d 0000 0072 2e00 0000 722f 0000 007a  r-...r....r/...z
+000019e0: 9a28 7265 7175 6573 742d 7461 7267 6574  .(request-target
+000019f0: 293a 2070 6f73 7420 2f70 6174 682f 746f  ): post /path/to
+00001a00: 2f72 6573 6f75 7263 650a 686f 7374 3a20  /resource.host: 
+00001a10: 6d79 686f 7374 2e74 6c64 0a64 6174 653a  myhost.tld.date:
+00001a20: 2057 6564 2c20 3135 204d 6172 2032 3032   Wed, 15 Mar 202
+00001a30: 3320 3137 3a32 383a 3135 2047 4d54 0a64  3 17:28:15 GMT.d
+00001a40: 6967 6573 743a 2073 6861 2d32 3536 3d4d  igest: sha-256=M
+00001a50: 494c 6235 6c55 4444 365a 3070 4453 7868  ILb5lUDD6Z0pDSxh
+00001a60: 6778 6a2b 684d 4245 7730 7554 7a50 3367  gxj+hMBEw0uTzP3g
+00001a70: 3271 554a 4748 4d70 396b 3d72 3500 0000  2qUJGHMp9k=r5...
+00001a80: 7236 0000 005a 337a 3476 506b 4a61 6f61  r6...Z3z4vPkJaoa
+00001a90: 5356 5170 3544 724d 6238 4576 4361 6a4a  SVQp5DrMb8EvCajJ
+00001aa0: 6365 7257 3336 7273 7957 4445 4c54 5751  cerW36rsyWDELTWQ
+00001ab0: 3363 596d 616f 6e6e 4766 5a26 6238 5748  3cYmaonnGfZ&b8WH
+00001ac0: 6977 4835 3442 5368 6964 4363 6d70 6f79  iwH54BShidCcmpoy
+00001ad0: 486a 616e 5652 594e 7258 5858 6b61 346a  HjanVRYNrXXXka4j
+00001ae0: 416e 7237 0000 0072 1700 0000 7238 0000  Anr7...r....r8..
+00001af0: 0072 3900 0000 723a 0000 0072 3b00 0000  .r9...r:...r;...
+00001b00: 2911 da04 6a73 6f6e da05 6475 6d70 73da  )...json..dumps.
+00001b10: 0665 6e63 6f64 6572 1a00 0000 721b 0000  .encoder....r...
+00001b20: 0072 1c00 0000 721d 0000 0072 1e00 0000  .r....r....r....
+00001b30: 721f 0000 0072 2000 0000 7221 0000 0072  r....r ...r!...r
+00001b40: 0300 0000 7205 0000 0072 1800 0000 723c  ....r....r....r<
+00001b50: 0000 0072 3d00 0000 723e 0000 0029 0e72  ...r=...r>...).r
+00001b60: 4500 0000 7224 0000 0072 2500 0000 7226  E...r$...r%...r&
+00001b70: 0000 0072 2700 0000 7232 0000 0072 2200  ...r'...r2...r".
+00001b80: 0000 7235 0000 0072 1700 0000 723f 0000  ..r5...r....r?..
+00001b90: 0072 4000 0000 7241 0000 0072 4200 0000  .r@...rA...rB...
+00001ba0: 7243 0000 0072 2800 0000 7228 0000 0072  rC...r(...r(...r
+00001bb0: 2900 0000 da17 7465 7374 5f62 7569 6c64  ).....test_build
+00001bc0: 5f6d 6573 7361 6765 5f70 6f73 745b 0000  _message_post[..
+00001bd0: 0073 8000 0000 1401 7802 0802 7802 0a03  .s......x...x...
+00001be0: 0801 0801 02fd 0806 1202 0206 0efa 0206  ................
+00001bf0: 04fa 0406 06fa 0206 02fa 0206 04fa 0206  ................
+00001c00: 02fa 0406 04fa 0206 02fa 0206 18fa 0206  ................
+00001c10: 02fa 0206 0cfa 0408 0201 04ff 2004 0204  ............ ...
+00001c20: 0efc 0204 04fc 0404 06fc 0204 02fc 0204  ................
+00001c30: 06fc 0204 02fc 0404 04fc 0204 02fc 0204  ................
+00001c40: 02fc 0204 02fc 0204 18fc 0204 02fc 0204  ................
+00001c50: 14fc 0406 1002 7249 0000 0029 13da 0862  ......rI...)...b
+00001c60: 7569 6c74 696e 7372 1c00 0000 da19 5f70  uiltinsr......_p
+00001c70: 7974 6573 742e 6173 7365 7274 696f 6e2e  ytest.assertion.
+00001c80: 7265 7772 6974 65da 0961 7373 6572 7469  rewrite..asserti
+00001c90: 6f6e da07 7265 7772 6974 6572 1a00 0000  on..rewriter....
+00001ca0: 7246 0000 00da 0668 656c 7065 7272 0300  rF.....helperr..
+00001cb0: 0000 7222 0000 0072 0400 0000 7205 0000  ..r"...r....r...
+00001cc0: 00da 0474 6573 7472 0600 0000 722a 0000  ...testr....r*..
+00001cd0: 0072 3000 0000 7234 0000 0072 4400 0000  .r0...r4...rD...
+00001ce0: 7249 0000 0072 2800 0000 7228 0000 0072  rI...r(...r(...r
+00001cf0: 2800 0000 7229 0000 00da 083c 6d6f 6475  (...r).....<modu
+00001d00: 6c65 3e01 0000 0073 1200 0000 2200 0c02  le>....s...."...
+00001d10: 1001 0c01 0803 0810 0817 080f 0c1d       ..............
```

### Comparing `bovine-0.1.0/bovine/crypto/__pycache__/test_signature_parser.cpython-310-pytest-7.3.0.pyc` & `bovine-0.1.1/bovine/crypto/__pycache__/test_signature_parser.cpython-310-pytest-7.3.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 13 15:55:57 2023 UTC, .py size: 1207 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0d26 3864 b704 0000  o........&8d....
+00000000: 6f0d 0d0a 0000 0000 a4ea 3a64 b704 0000  o.........:d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 3a00 0000 6400  .....@...s:...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6402 6403 6c06 6d07  ..m.Z...d.d.l.m.
 00000050: 5a07 0100 6404 6405 8400 5a08 6406 6407  Z...d.d...Z.d.d.
 00000060: 8400 5a09 6401 5300 2908 e900 0000 004e  ..Z.d.S.)......N
 00000070: e901 0000 0029 01da 0953 6967 6e61 7475  .....)...Signatu
@@ -113,56 +113,56 @@
 00000700: 0b40 7079 5f61 7373 6572 7431 da0b 4070  .@py_assert1..@p
 00000710: 795f 6173 7365 7274 34da 0b40 7079 5f61  y_assert4..@py_a
 00000720: 7373 6572 7433 da0b 4070 795f 666f 726d  ssert3..@py_form
 00000730: 6174 36da 0b40 7079 5f66 6f72 6d61 7438  at6..@py_format8
 00000740: da0b 4070 795f 6173 7365 7274 36da 0b40  ..@py_assert6..@
 00000750: 7079 5f61 7373 6572 7435 da0c 4070 795f  py_assert5..@py_
 00000760: 666f 726d 6174 3130 a900 7235 0000 00fa  format10..r5....
-00000770: 572f 776f 6f64 7065 636b 6572 2f73 7263  W/woodpecker/src
-00000780: 2f63 6f64 6562 6572 672e 6f72 672f 6865  /codeberg.org/he
-00000790: 6c67 652f 626f 7669 6e65 2f62 6f76 696e  lge/bovine/bovin
-000007a0: 652f 626f 7669 6e65 2f63 7279 7074 6f2f  e/bovine/crypto/
-000007b0: 7465 7374 5f73 6967 6e61 7475 7265 5f70  test_signature_p
-000007c0: 6172 7365 722e 7079 da1d 7465 7374 5f73  arser.py..test_s
-000007d0: 6967 6e61 7475 7265 5f68 6561 6465 725f  ignature_header_
-000007e0: 7061 7273 696e 6704 0000 0073 4e00 0000  parsing....sN...
-000007f0: 0401 0a02 8a02 8a01 8a01 8c01 0201 0206  ................
-00000800: 20fa 0206 0efa 0206 04fa 0406 08fa 0206   ...............
-00000810: 02fa 0206 06fa 0206 02fa 0406 04fa 0206  ................
-00000820: 02fa 0206 02fa 0206 02fa 0206 02fa 0206  ................
-00000830: 02fa 0206 18fa 0206 02fa 0206 18fa 7237  ..............r7
-00000840: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-00000850: 0a00 0000 0700 0000 4300 0000 7204 0000  ........C...r...
-00000860: 0029 144e 7a5a 6b65 7949 643d 2268 7474  .).NzZkeyId="htt
-00000870: 7073 3a2f 2f68 6f73 742e 7573 6572 236d  ps://host.user#m
-00000880: 6169 6e2d 6b65 7922 2c68 6561 6465 7273  ain-key",headers
-00000890: 3d22 2872 6571 7565 7374 2d74 6172 6765  ="(request-targe
-000008a0: 7429 2068 6f73 7420 6461 7465 222c 7369  t) host date",si
-000008b0: 676e 6174 7572 653d 2273 7475 6666 3d22  gnature="stuff="
-000008c0: 7205 0000 0072 0600 0000 7208 0000 0072  r....r....r....r
-000008d0: 0900 0000 720a 0000 0072 0e00 0000 720f  ....r....r....r.
-000008e0: 0000 0072 1000 0000 7211 0000 007a 1a28  ...r....r....z.(
-000008f0: 7265 7175 6573 742d 7461 7267 6574 2920  request-target) 
-00000900: 686f 7374 2064 6174 6572 1200 0000 7a06  host dater....z.
-00000910: 7374 7566 663d 7213 0000 0029 0372 1400  stuff=r....).r..
-00000920: 0000 7215 0000 0072 1600 0000 7218 0000  ..r....r....r...
-00000930: 0072 1900 0000 721b 0000 0072 1c00 0000  .r....r....r....
-00000940: 721d 0000 0072 2c00 0000 7235 0000 0072  r....r,...r5...r
-00000950: 3500 0000 7236 0000 00da 2774 6573 745f  5...r6....'test_
-00000960: 7369 676e 6174 7572 655f 6865 6164 6572  signature_header
-00000970: 5f77 6974 686f 7574 5f61 6c67 6f72 6974  _without_algorit
-00000980: 686d 1600 0000 734e 0000 0004 010a 028a  hm....sN........
-00000990: 028a 018a 018c 0102 0102 0420 fc02 040e  ........... ....
-000009a0: fc02 0404 fc04 0408 fc02 0402 fc02 0406  ................
-000009b0: fc02 0402 fc04 0404 fc02 0402 fc02 0402  ................
-000009c0: fc02 0402 fc02 0402 fc02 0402 fc02 0418  ................
-000009d0: fc02 0402 fc02 0418 fc72 3800 0000 290a  .........r8...).
-000009e0: da08 6275 696c 7469 6e73 7222 0000 00da  ..builtinsr"....
-000009f0: 195f 7079 7465 7374 2e61 7373 6572 7469  ._pytest.asserti
-00000a00: 6f6e 2e72 6577 7269 7465 da09 6173 7365  on.rewrite..asse
-00000a10: 7274 696f 6eda 0772 6577 7269 7465 7220  rtion..rewriter 
-00000a20: 0000 00da 1073 6967 6e61 7475 7265 5f70  .....signature_p
-00000a30: 6172 7365 7272 0300 0000 7237 0000 0072  arserr....r7...r
-00000a40: 3800 0000 7235 0000 0072 3500 0000 7235  8...r5...r5...r5
-00000a50: 0000 0072 3600 0000 da08 3c6d 6f64 756c  ...r6.....<modul
-00000a60: 653e 0100 0000 7306 0000 0026 0008 030c  e>....s....&....
-00000a70: 12                                       .
+00000770: 582f 776f 6f64 7065 636b 6572 2f73 7263  X/woodpecker/src
+00000780: 2f63 6f64 6562 6572 672e 6f72 672f 626f  /codeberg.org/bo
+00000790: 7669 6e65 2f62 6f76 696e 652f 626f 7669  vine/bovine/bovi
+000007a0: 6e65 2f62 6f76 696e 652f 6372 7970 746f  ne/bovine/crypto
+000007b0: 2f74 6573 745f 7369 676e 6174 7572 655f  /test_signature_
+000007c0: 7061 7273 6572 2e70 79da 1d74 6573 745f  parser.py..test_
+000007d0: 7369 676e 6174 7572 655f 6865 6164 6572  signature_header
+000007e0: 5f70 6172 7369 6e67 0400 0000 734e 0000  _parsing....sN..
+000007f0: 0004 010a 028a 028a 018a 018c 0102 0102  ................
+00000800: 0620 fa02 060e fa02 0604 fa04 0608 fa02  . ..............
+00000810: 0602 fa02 0606 fa02 0602 fa04 0604 fa02  ................
+00000820: 0602 fa02 0602 fa02 0602 fa02 0602 fa02  ................
+00000830: 0602 fa02 0618 fa02 0602 fa02 0618 fa72  ...............r
+00000840: 3700 0000 6300 0000 0000 0000 0000 0000  7...c...........
+00000850: 000a 0000 0007 0000 0043 0000 0072 0400  .........C...r..
+00000860: 0000 2914 4e7a 5a6b 6579 4964 3d22 6874  ..).NzZkeyId="ht
+00000870: 7470 733a 2f2f 686f 7374 2e75 7365 7223  tps://host.user#
+00000880: 6d61 696e 2d6b 6579 222c 6865 6164 6572  main-key",header
+00000890: 733d 2228 7265 7175 6573 742d 7461 7267  s="(request-targ
+000008a0: 6574 2920 686f 7374 2064 6174 6522 2c73  et) host date",s
+000008b0: 6967 6e61 7475 7265 3d22 7374 7566 663d  ignature="stuff=
+000008c0: 2272 0500 0000 7206 0000 0072 0800 0000  "r....r....r....
+000008d0: 7209 0000 0072 0a00 0000 720e 0000 0072  r....r....r....r
+000008e0: 0f00 0000 7210 0000 0072 1100 0000 7a1a  ....r....r....z.
+000008f0: 2872 6571 7565 7374 2d74 6172 6765 7429  (request-target)
+00000900: 2068 6f73 7420 6461 7465 7212 0000 007a   host dater....z
+00000910: 0673 7475 6666 3d72 1300 0000 2903 7214  .stuff=r....).r.
+00000920: 0000 0072 1500 0000 7216 0000 0072 1800  ...r....r....r..
+00000930: 0000 7219 0000 0072 1b00 0000 721c 0000  ..r....r....r...
+00000940: 0072 1d00 0000 722c 0000 0072 3500 0000  .r....r,...r5...
+00000950: 7235 0000 0072 3600 0000 da27 7465 7374  r5...r6....'test
+00000960: 5f73 6967 6e61 7475 7265 5f68 6561 6465  _signature_heade
+00000970: 725f 7769 7468 6f75 745f 616c 676f 7269  r_without_algori
+00000980: 7468 6d16 0000 0073 4e00 0000 0401 0a02  thm....sN.......
+00000990: 8a02 8a01 8a01 8c01 0201 0204 20fc 0204  ............ ...
+000009a0: 0efc 0204 04fc 0404 08fc 0204 02fc 0204  ................
+000009b0: 06fc 0204 02fc 0404 04fc 0204 02fc 0204  ................
+000009c0: 02fc 0204 02fc 0204 02fc 0204 02fc 0204  ................
+000009d0: 18fc 0204 02fc 0204 18fc 7238 0000 0029  ..........r8...)
+000009e0: 0ada 0862 7569 6c74 696e 7372 2200 0000  ...builtinsr"...
+000009f0: da19 5f70 7974 6573 742e 6173 7365 7274  .._pytest.assert
+00000a00: 696f 6e2e 7265 7772 6974 65da 0961 7373  ion.rewrite..ass
+00000a10: 6572 7469 6f6e da07 7265 7772 6974 6572  ertion..rewriter
+00000a20: 2000 0000 da10 7369 676e 6174 7572 655f   .....signature_
+00000a30: 7061 7273 6572 7203 0000 0072 3700 0000  parserr....r7...
+00000a40: 7238 0000 0072 3500 0000 7235 0000 0072  r8...r5...r5...r
+00000a50: 3500 0000 7236 0000 00da 083c 6d6f 6475  5...r6.....<modu
+00000a60: 6c65 3e01 0000 0073 0600 0000 2600 0803  le>....s....&...
+00000a70: 0c12                                     ..
```

### Comparing `bovine-0.1.0/bovine/crypto/helper.py` & `bovine-0.1.1/bovine/crypto/helper.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,14 @@
         content = content.encode("utf-8")
 
     digest = base64.standard_b64encode(hashlib.sha256(content).digest()).decode("utf-8")
     return "sha-256=" + digest
 
 
 def sign_message(private_key, message):
-    private_key = private_key.replace("\\n", "\n")
     try:
         key = load_pem_private_key(private_key.encode("utf-8"), password=None)
         assert isinstance(key, rsa.RSAPrivateKey)
     except Exception as e:
         logger.error(e)
         logger.error(private_key)
         raise (e)
@@ -39,15 +38,14 @@
             padding.PKCS1v15(),
             hashes.SHA256(),
         )
     ).decode("utf-8")
 
 
 def verify_signature(public_key, message, signature):
-    public_key = public_key.replace("\\n", "\n")
     public_key_loaded = load_pem_public_key(public_key.encode("utf-8"))
 
     assert isinstance(public_key_loaded, rsa.RSAPublicKey)
 
     try:
         public_key_loaded.verify(
             base64.standard_b64decode(signature),
```

### Comparing `bovine-0.1.0/bovine/crypto/http_signature.py` & `bovine-0.1.1/bovine/crypto/http_signature.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.0/bovine/crypto/signature_checker.py` & `bovine-0.1.1/bovine/crypto/signature_checker.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.0/bovine/crypto/signature_parser.py` & `bovine-0.1.1/bovine/crypto/signature_parser.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.0/bovine/crypto/test.py` & `bovine-0.1.1/bovine/crypto/test.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.0/bovine/crypto/test_crypto.py` & `bovine-0.1.1/bovine/crypto/test_crypto.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.0/bovine/crypto/test_helper.py` & `bovine-0.1.1/bovine/crypto/test_helper.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.0/bovine/crypto/test_http_signature.py` & `bovine-0.1.1/bovine/crypto/test_http_signature.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.0/bovine/crypto/test_signature_parser.py` & `bovine-0.1.1/bovine/crypto/test_signature_parser.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.0/bovine/utils/__pycache__/date.cpython-310.pyc` & `bovine-0.1.1/bovine/utils/__pycache__/date.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 13 15:55:57 2023 UTC, .py size: 519 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0d26 3864 0702 0000  o........&8d....
+00000000: 6f0d 0d0a 0000 0000 a4ea 3a64 0702 0000  o.........:d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0007 0000 0040 0000 0073 5c00 0000 6400  .....@...s\...d.
 00000030: 6401 6c00 6d00 5a00 6d01 5a01 6d02 5a02  d.l.m.Z.m.Z.m.Z.
 00000040: 0100 6400 6402 6c03 6d04 5a04 0100 6403  ..d.d.l.m.Z...d.
 00000050: 6505 6602 6404 6405 8404 5a06 6406 6505  e.f.d.d...Z.d.e.
 00000060: 6403 6500 6604 6407 6408 8404 5a07 640f  d.e.f.d.d...Z.d.
 00000070: 640a 6500 640b 6508 6403 6509 6606 640c  d.e.d.e.d.e.f.d.
@@ -13,43 +13,43 @@
 000000c0: 7572 6e63 0000 0000 0000 0000 0000 0000  urnc............
 000000d0: 0000 0000 0300 0000 4300 0000 730e 0000  ........C...s...
 000000e0: 0074 00a0 01a1 00a0 0264 01a1 0153 0029  .t.......d...S.)
 000000f0: 024e 7a19 2561 2c20 2564 2025 6220 2559  .Nz.%a, %d %b %Y
 00000100: 2025 483a 254d 3a25 5320 474d 5429 0372   %H:%M:%S GMT).r
 00000110: 0200 0000 da06 7574 636e 6f77 da08 7374  ......utcnow..st
 00000120: 7266 7469 6d65 a900 720a 0000 0072 0a00  rftime..r....r..
-00000130: 0000 fa45 2f77 6f6f 6470 6563 6b65 722f  ...E/woodpecker/
+00000130: 0000 fa46 2f77 6f6f 6470 6563 6b65 722f  ...F/woodpecker/
 00000140: 7372 632f 636f 6465 6265 7267 2e6f 7267  src/codeberg.org
-00000150: 2f68 656c 6765 2f62 6f76 696e 652f 626f  /helge/bovine/bo
-00000160: 7669 6e65 2f62 6f76 696e 652f 7574 696c  vine/bovine/util
-00000170: 732f 6461 7465 2e70 79da 0b67 6574 5f67  s/date.py..get_g
-00000180: 6d74 5f6e 6f77 0600 0000 7302 0000 000e  mt_now....s.....
-00000190: 0172 0c00 0000 da0b 6461 7465 5f73 7472  .r......date_str
-000001a0: 696e 6763 0100 0000 0000 0000 0000 0000  ingc............
-000001b0: 0100 0000 0200 0000 4300 0000 7308 0000  ........C...s...
-000001c0: 0074 007c 0083 0153 0029 014e 7205 0000  .t.|...S.).Nr...
-000001d0: 0029 0172 0d00 0000 720a 0000 0072 0a00  .).r....r....r..
-000001e0: 0000 720b 0000 00da 0970 6172 7365 5f67  ..r......parse_g
-000001f0: 6d74 0a00 0000 7302 0000 0008 0172 0e00  mt....s......r..
-00000200: 0000 e905 0000 00da 0264 74da 076d 696e  .........dt..min
-00000210: 7574 6573 6302 0000 0000 0000 0000 0000  utesc...........
-00000220: 0003 0000 0005 0000 0043 0000 0073 3e00  .........C...s>.
-00000230: 0000 7400 6a01 7402 6a03 6401 8d01 7d02  ..t.j.t.j.d...}.
-00000240: 7c00 7c02 7404 7c01 6402 8d01 1700 6b04  |.|.t.|.d.....k.
-00000250: 7212 6403 5300 7c00 7c02 7404 7c01 6402  r.d.S.|.|.t.|.d.
-00000260: 8d01 1800 6b00 721d 6403 5300 6404 5300  ....k.r.d.S.d.S.
-00000270: 2905 4e29 01da 0274 7a29 0172 1100 0000  ).N)...tz).r....
-00000280: 4654 2905 7202 0000 00da 036e 6f77 7204  FT).r......nowr.
-00000290: 0000 00da 0375 7463 7203 0000 0029 0372  .....utcr....).r
-000002a0: 1000 0000 7211 0000 0072 1300 0000 720a  ....r....r....r.
-000002b0: 0000 0072 0a00 0000 720b 0000 00da 1463  ...r....r......c
-000002c0: 6865 636b 5f6d 6178 5f6f 6666 7365 745f  heck_max_offset_
-000002d0: 6e6f 770e 0000 0073 0c00 0000 0e01 1202  now....s........
-000002e0: 0401 1202 0401 0402 7215 0000 004e 2901  ........r....N).
-000002f0: 720f 0000 0029 0b72 0200 0000 7203 0000  r....).r....r...
-00000300: 0072 0400 0000 5a0f 6461 7465 7574 696c  .r....Z.dateutil
-00000310: 2e70 6172 7365 7272 0600 0000 da03 7374  .parserr......st
-00000320: 7272 0c00 0000 720e 0000 00da 0369 6e74  rr....r......int
-00000330: da04 626f 6f6c 7215 0000 0072 0a00 0000  ..boolr....r....
-00000340: 720a 0000 0072 0a00 0000 720b 0000 00da  r....r....r.....
-00000350: 083c 6d6f 6475 6c65 3e01 0000 0073 0a00  .<module>....s..
-00000360: 0000 1400 0c02 0e03 1204 1c04            ............
+00000150: 2f62 6f76 696e 652f 626f 7669 6e65 2f62  /bovine/bovine/b
+00000160: 6f76 696e 652f 626f 7669 6e65 2f75 7469  ovine/bovine/uti
+00000170: 6c73 2f64 6174 652e 7079 da0b 6765 745f  ls/date.py..get_
+00000180: 676d 745f 6e6f 7706 0000 0073 0200 0000  gmt_now....s....
+00000190: 0e01 720c 0000 00da 0b64 6174 655f 7374  ..r......date_st
+000001a0: 7269 6e67 6301 0000 0000 0000 0000 0000  ringc...........
+000001b0: 0001 0000 0002 0000 0043 0000 0073 0800  .........C...s..
+000001c0: 0000 7400 7c00 8301 5300 2901 4e72 0500  ..t.|...S.).Nr..
+000001d0: 0000 2901 720d 0000 0072 0a00 0000 720a  ..).r....r....r.
+000001e0: 0000 0072 0b00 0000 da09 7061 7273 655f  ...r......parse_
+000001f0: 676d 740a 0000 0073 0200 0000 0801 720e  gmt....s......r.
+00000200: 0000 00e9 0500 0000 da02 6474 da07 6d69  ..........dt..mi
+00000210: 6e75 7465 7363 0200 0000 0000 0000 0000  nutesc..........
+00000220: 0000 0300 0000 0500 0000 4300 0000 733e  ..........C...s>
+00000230: 0000 0074 006a 0174 026a 0364 018d 017d  ...t.j.t.j.d...}
+00000240: 027c 007c 0274 047c 0164 028d 0117 006b  .|.|.t.|.d.....k
+00000250: 0472 1264 0353 007c 007c 0274 047c 0164  .r.d.S.|.|.t.|.d
+00000260: 028d 0118 006b 0072 1d64 0353 0064 0453  .....k.r.d.S.d.S
+00000270: 0029 054e 2901 da02 747a 2901 7211 0000  .).N)...tz).r...
+00000280: 0046 5429 0572 0200 0000 da03 6e6f 7772  .FT).r......nowr
+00000290: 0400 0000 da03 7574 6372 0300 0000 2903  ......utcr....).
+000002a0: 7210 0000 0072 1100 0000 7213 0000 0072  r....r....r....r
+000002b0: 0a00 0000 720a 0000 0072 0b00 0000 da14  ....r....r......
+000002c0: 6368 6563 6b5f 6d61 785f 6f66 6673 6574  check_max_offset
+000002d0: 5f6e 6f77 0e00 0000 730c 0000 000e 0112  _now....s.......
+000002e0: 0204 0112 0204 0104 0272 1500 0000 4e29  .........r....N)
+000002f0: 0172 0f00 0000 290b 7202 0000 0072 0300  .r....).r....r..
+00000300: 0000 7204 0000 005a 0f64 6174 6575 7469  ..r....Z.dateuti
+00000310: 6c2e 7061 7273 6572 7206 0000 00da 0373  l.parserr......s
+00000320: 7472 720c 0000 0072 0e00 0000 da03 696e  trr....r......in
+00000330: 74da 0462 6f6f 6c72 1500 0000 720a 0000  t..boolr....r...
+00000340: 0072 0a00 0000 720a 0000 0072 0b00 0000  .r....r....r....
+00000350: da08 3c6d 6f64 756c 653e 0100 0000 730a  ..<module>....s.
+00000360: 0000 0014 000c 020e 0312 041c 04         .............
```

### Comparing `bovine-0.1.0/bovine/utils/__pycache__/test_date.cpython-310-pytest-7.3.0.pyc` & `bovine-0.1.1/bovine/utils/__pycache__/test_date.cpython-310-pytest-7.3.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 13 15:55:57 2023 UTC, .py size: 737 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0d26 3864 e102 0000  o........&8d....
+00000000: 6f0d 0d0a 0000 0000 a4ea 3a64 e102 0000  o.........:d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 5e00 0000 6400  .....@...s^...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6402 6c06 6d06  ..m.Z...d.d.l.m.
 00000050: 5a06 6d07 5a07 6d08 5a08 0100 6403 6404  Z.m.Z.m.Z...d.d.
 00000060: 6c09 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c 0100  l.m.Z.m.Z.m.Z...
 00000070: 6405 6406 8400 5a0d 6407 6408 8400 5a0e  d.d...Z.d.d...Z.
@@ -36,181 +36,181 @@
 00000230: 725f 676c 6f62 616c 5f6e 616d 65da 0e41  r_global_name..A
 00000240: 7373 6572 7469 6f6e 4572 726f 72da 135f  ssertionError.._
 00000250: 666f 726d 6174 5f65 7870 6c61 6e61 7469  format_explanati
 00000260: 6f6e 2905 720b 0000 00da 0b40 7079 5f61  on).r......@py_a
 00000270: 7373 6572 7430 da0b 4070 795f 6173 7365  ssert0..@py_asse
 00000280: 7274 32da 0b40 7079 5f66 6f72 6d61 7434  rt2..@py_format4
 00000290: da0b 4070 795f 666f 726d 6174 36a9 0072  ..@py_format6..r
-000002a0: 1b00 0000 fa4a 2f77 6f6f 6470 6563 6b65  .....J/woodpecke
+000002a0: 1b00 0000 fa4b 2f77 6f6f 6470 6563 6b65  .....K/woodpecke
 000002b0: 722f 7372 632f 636f 6465 6265 7267 2e6f  r/src/codeberg.o
-000002c0: 7267 2f68 656c 6765 2f62 6f76 696e 652f  rg/helge/bovine/
-000002d0: 626f 7669 6e65 2f62 6f76 696e 652f 7574  bovine/bovine/ut
-000002e0: 696c 732f 7465 7374 5f64 6174 652e 7079  ils/test_date.py
-000002f0: da10 7465 7374 5f67 6574 5f67 6d74 5f6e  ..test_get_gmt_n
-00000300: 6f77 0600 0000 7304 0000 0006 017c 0272  ow....s......|.r
-00000310: 1d00 0000 6300 0000 0000 0000 0000 0000  ....c...........
-00000320: 000b 0000 0008 0000 0043 0000 0073 8801  .........C...s..
-00000330: 0000 7400 8300 7d00 7401 7c00 8301 7d01  ..t...}.t.|...}.
-00000340: 7402 6a03 7404 6a05 6401 8d01 7d02 7c01  t.j.t.j.d...}.|.
-00000350: 7c02 6b01 7d03 7c03 7351 7406 a007 6402  |.k.}.|.sQt...d.
-00000360: 7c03 6601 6403 7c01 7c02 6602 a104 6404  |.f.d.|.|.f...d.
-00000370: 7408 a009 a100 7600 7329 7406 a00a 7c01  t.....v.s)t...|.
-00000380: a101 722e 7406 a00b 7c01 a101 6e01 6404  ..r.t...|...n.d.
-00000390: 6405 7408 a009 a100 7600 733a 7406 a00a  d.t.....v.s:t...
-000003a0: 7c02 a101 723f 7406 a00b 7c02 a101 6e01  |...r?t...|...n.
-000003b0: 6405 6406 9c02 1600 7d04 6407 6408 7c04  d.d.....}.d.d.|.
-000003c0: 6901 1600 7d05 740c 7406 a00d 7c05 a101  i...}.t.t...|...
-000003d0: 8301 8201 6400 7d03 6409 7d06 740e 7c06  ....d.}.d.}.t.|.
-000003e0: 640a 8d01 7d07 7c02 7c07 1800 7d08 7c01  d...}.|.|...}.|.
-000003f0: 7c08 6b05 7d03 7c03 73ba 7406 a007 640b  |.k.}.|.s.t...d.
-00000400: 7c03 6601 640c 7c01 7c08 6602 a104 6404  |.f.d.|.|.f...d.
-00000410: 7408 a009 a100 7600 7379 7406 a00a 7c01  t.....v.syt...|.
-00000420: a101 727e 7406 a00b 7c01 a101 6e01 6404  ..r~t...|...n.d.
-00000430: 6405 7408 a009 a100 7600 738a 7406 a00a  d.t.....v.s.t...
-00000440: 7c02 a101 728f 7406 a00b 7c02 a101 6e01  |...r.t...|...n.
-00000450: 6405 640d 7408 a009 a100 7600 739b 7406  d.d.t.....v.s.t.
-00000460: a00a 740e a101 72a0 7406 a00b 740e a101  ..t...r.t...t...
-00000470: 6e01 640d 7406 a00b 7c06 a101 7406 a00b  n.d.t...|...t...
-00000480: 7c07 a101 640e 9c05 1600 7d09 640f 6410  |...d.....}.d.d.
-00000490: 7c09 6901 1600 7d0a 740c 7406 a00d 7c0a  |.i...}.t.t...|.
-000004a0: a101 8301 8201 6400 0400 7d03 0400 7d06  ......d...}...}.
-000004b0: 0400 7d07 7d08 6400 5300 2911 4ea9 01da  ..}.}.d.S.).N...
-000004c0: 0274 7a29 01fa 023c 3d29 017a 1225 2870  .tz)...<=).z.%(p
-000004d0: 7930 2973 203c 3d20 2528 7079 3229 73da  y0)s <= %(py2)s.
-000004e0: 0670 6172 7365 64da 036e 6f77 2902 da03  .parsed..now)...
-000004f0: 7079 30da 0370 7932 7a0e 6173 7365 7274  py0..py2z.assert
-00000500: 2025 2870 7934 2973 da03 7079 34e9 0500   %(py4)s..py4...
-00000510: 0000 2901 da07 7365 636f 6e64 7329 01fa  ..)...seconds)..
-00000520: 023e 3d29 017a 4425 2870 7930 2973 203e  .>=).zD%(py0)s >
-00000530: 3d20 2825 2870 7932 2973 202d 2025 2870  = (%(py2)s - %(p
-00000540: 7937 2973 0a7b 2528 7079 3729 7320 3d20  y7)s.{%(py7)s = 
-00000550: 2528 7079 3329 7328 7365 636f 6e64 733d  %(py3)s(seconds=
-00000560: 2528 7079 3529 7329 0a7d 2972 0300 0000  %(py5)s).})r....
-00000570: 2905 7223 0000 0072 2400 0000 720d 0000  ).r#...r$...r...
-00000580: 0072 0e00 0000 da03 7079 377a 0f61 7373  .r......py7z.ass
-00000590: 6572 7420 2528 7079 3130 2973 da04 7079  ert %(py10)s..py
-000005a0: 3130 290f 7207 0000 0072 0800 0000 7202  10).r....r....r.
-000005b0: 0000 0072 2200 0000 7204 0000 00da 0375  ...r"...r......u
-000005c0: 7463 720f 0000 0072 1000 0000 7212 0000  tcr....r....r...
-000005d0: 0072 1300 0000 7214 0000 0072 1100 0000  .r....r....r....
-000005e0: 7215 0000 0072 1600 0000 7203 0000 0029  r....r....r....)
-000005f0: 0b72 0b00 0000 7221 0000 0072 2200 0000  .r....r!...r"...
-00000600: da0b 4070 795f 6173 7365 7274 31da 0b40  ..@py_assert1..@
-00000610: 7079 5f66 6f72 6d61 7433 da0b 4070 795f  py_format3..@py_
-00000620: 666f 726d 6174 35da 0b40 7079 5f61 7373  format5..@py_ass
-00000630: 6572 7434 da0b 4070 795f 6173 7365 7274  ert4..@py_assert
-00000640: 36da 0b40 7079 5f61 7373 6572 7438 da0b  6..@py_assert8..
-00000650: 4070 795f 666f 726d 6174 39da 0c40 7079  @py_format9..@py
-00000660: 5f66 6f72 6d61 7431 3172 1b00 0000 721b  _format11r....r.
-00000670: 0000 0072 1c00 0000 da0e 7465 7374 5f70  ...r......test_p
-00000680: 6172 7365 5f67 6d74 0c00 0000 730a 0000  arse_gmt....s...
-00000690: 0006 0108 020e 018a 02e2 0172 3400 0000  ...........r4...
-000006a0: 6300 0000 0000 0000 0000 0000 0008 0000  c...............
-000006b0: 0009 0000 0043 0000 0073 5e03 0000 7400  .....C...s^...t.
-000006c0: 6a01 7402 6a03 6401 8d01 7d00 6402 7d01  j.t.j.d...}.d.}.
-000006d0: 7404 7c01 6403 8d01 7d02 7c00 7c02 1800  t.|.d...}.|.|...
-000006e0: 7d03 7405 7c03 8301 7d04 7c04 7363 6404  }.t.|...}.|.scd.
-000006f0: 6405 7406 a007 a100 7600 7324 7408 a009  d.t.....v.s$t...
-00000700: 7405 a101 7229 7408 a00a 7405 a101 6e01  t...r)t...t...n.
-00000710: 6405 6406 7406 a007 a100 7600 7335 7408  d.d.t.....v.s5t.
-00000720: a009 7c00 a101 723a 7408 a00a 7c00 a101  ..|...r:t...|...
-00000730: 6e01 6406 6407 7406 a007 a100 7600 7346  n.d.d.t.....v.sF
-00000740: 7408 a009 7404 a101 724b 7408 a00a 7404  t...t...rKt...t.
-00000750: a101 6e01 6407 7408 a00a 7c01 a101 7408  ..n.d.t...|...t.
-00000760: a00a 7c02 a101 7408 a00a 7c04 a101 6408  ..|...t...|...d.
-00000770: 9c06 1600 7d05 740b 7408 a00c 7c05 a101  ....}.t.t...|...
-00000780: 8301 8201 6400 0400 7d01 0400 7d02 0400  ....d...}...}...
-00000790: 7d03 7d04 6402 7d01 7404 7c01 6403 8d01  }.}.d.}.t.|.d...
-000007a0: 7d02 7c00 7c02 1700 7d03 7405 7c03 8301  }.|.|...}.t.|...
-000007b0: 7d04 7c04 73c7 6409 6405 7406 a007 a100  }.|.s.d.d.t.....
-000007c0: 7600 7388 7408 a009 7405 a101 728d 7408  v.s.t...t...r.t.
-000007d0: a00a 7405 a101 6e01 6405 6406 7406 a007  ..t...n.d.d.t...
-000007e0: a100 7600 7399 7408 a009 7c00 a101 729e  ..v.s.t...|...r.
-000007f0: 7408 a00a 7c00 a101 6e01 6406 6407 7406  t...|...n.d.d.t.
-00000800: a007 a100 7600 73aa 7408 a009 7404 a101  ....v.s.t...t...
-00000810: 72af 7408 a00a 7404 a101 6e01 6407 7408  r.t...t...n.d.t.
-00000820: a00a 7c01 a101 7408 a00a 7c02 a101 7408  ..|...t...|...t.
-00000830: a00a 7c04 a101 6408 9c06 1600 7d05 740b  ..|...d.....}.t.
-00000840: 7408 a00c 7c05 a101 8301 8201 6400 0400  t...|.......d...
-00000850: 7d01 0400 7d02 0400 7d03 7d04 640a 7d01  }...}...}.}.d.}.
-00000860: 7404 7c01 6403 8d01 7d02 7c00 7c02 1800  t.|.d...}.|.|...
-00000870: 7d03 7405 7c03 8301 7d04 7c04 0c00 7d06  }.t.|...}.|...}.
-00000880: 7c06 9001 7333 640b 6405 7406 a007 a100  |...s3d.d.t.....
-00000890: 7600 73f0 7408 a009 7405 a101 72f5 7408  v.s.t...t...r.t.
-000008a0: a00a 7405 a101 6e01 6405 6406 7406 a007  ..t...n.d.d.t...
-000008b0: a100 7600 9001 7303 7408 a009 7c00 a101  ..v...s.t...|...
-000008c0: 9001 7208 7408 a00a 7c00 a101 6e01 6406  ..r.t...|...n.d.
-000008d0: 6407 7406 a007 a100 7600 9001 7316 7408  d.t.....v...s.t.
-000008e0: a009 7404 a101 9001 721b 7408 a00a 7404  ..t.....r.t...t.
-000008f0: a101 6e01 6407 7408 a00a 7c01 a101 7408  ..n.d.t...|...t.
-00000900: a00a 7c02 a101 7408 a00a 7c04 a101 6408  ..|...t...|...d.
-00000910: 9c06 1600 7d07 740b 7408 a00c 7c07 a101  ....}.t.t...|...
-00000920: 8301 8201 6400 0400 7d01 0400 7d02 0400  ....d...}...}...
-00000930: 7d03 0400 7d04 7d06 640a 7d01 7404 7c01  }...}.}.d.}.t.|.
-00000940: 6403 8d01 7d02 7c00 7c02 1700 7d03 7405  d...}.|.|...}.t.
-00000950: 7c03 8301 7d04 7c04 0c00 7d06 7c06 9001  |...}.|...}.|...
-00000960: 73a3 640c 6405 7406 a007 a100 7600 9001  s.d.d.t.....v...
-00000970: 7360 7408 a009 7405 a101 9001 7265 7408  s`t...t.....ret.
-00000980: a00a 7405 a101 6e01 6405 6406 7406 a007  ..t...n.d.d.t...
-00000990: a100 7600 9001 7373 7408 a009 7c00 a101  ..v...sst...|...
-000009a0: 9001 7278 7408 a00a 7c00 a101 6e01 6406  ..rxt...|...n.d.
-000009b0: 6407 7406 a007 a100 7600 9001 7386 7408  d.t.....v...s.t.
-000009c0: a009 7404 a101 9001 728b 7408 a00a 7404  ..t.....r.t...t.
-000009d0: a101 6e01 6407 7408 a00a 7c01 a101 7408  ..n.d.t...|...t.
-000009e0: a00a 7c02 a101 7408 a00a 7c04 a101 6408  ..|...t...|...d.
-000009f0: 9c06 1600 7d07 740b 7408 a00c 7c07 a101  ....}.t.t...|...
-00000a00: 8301 8201 6400 0400 7d01 0400 7d02 0400  ....d...}...}...
-00000a10: 7d03 0400 7d04 7d06 6400 5300 290d 4e72  }...}.}.d.S.).Nr
-00000a20: 1e00 0000 e904 0000 0029 01da 076d 696e  .........)...min
-00000a30: 7574 6573 7a5e 6173 7365 7274 2025 2870  utesz^assert %(p
-00000a40: 7939 2973 0a7b 2528 7079 3929 7320 3d20  y9)s.{%(py9)s = 
-00000a50: 2528 7079 3029 7328 2825 2870 7931 2973  %(py0)s((%(py1)s
-00000a60: 202d 2025 2870 7936 2973 0a7b 2528 7079   - %(py6)s.{%(py
-00000a70: 3629 7320 3d20 2528 7079 3229 7328 6d69  6)s = %(py2)s(mi
-00000a80: 6e75 7465 733d 2528 7079 3429 7329 0a7d  nutes=%(py4)s).}
-00000a90: 2929 0a7d 7206 0000 0072 2200 0000 7203  )).}r....r"...r.
-00000aa0: 0000 0029 0672 2300 0000 720c 0000 0072  ...).r#...r....r
-00000ab0: 2400 0000 7225 0000 00da 0370 7936 da03  $...r%.....py6..
-00000ac0: 7079 397a 5e61 7373 6572 7420 2528 7079  py9z^assert %(py
-00000ad0: 3929 730a 7b25 2870 7939 2973 203d 2025  9)s.{%(py9)s = %
-00000ae0: 2870 7930 2973 2828 2528 7079 3129 7320  (py0)s((%(py1)s 
-00000af0: 2b20 2528 7079 3629 730a 7b25 2870 7936  + %(py6)s.{%(py6
-00000b00: 2973 203d 2025 2870 7932 2973 286d 696e  )s = %(py2)s(min
-00000b10: 7574 6573 3d25 2870 7934 2973 290a 7d29  utes=%(py4)s).})
-00000b20: 290a 7de9 0600 0000 7a62 6173 7365 7274  ).}.....zbassert
-00000b30: 206e 6f74 2025 2870 7939 2973 0a7b 2528   not %(py9)s.{%(
-00000b40: 7079 3929 7320 3d20 2528 7079 3029 7328  py9)s = %(py0)s(
-00000b50: 2825 2870 7931 2973 202d 2025 2870 7936  (%(py1)s - %(py6
-00000b60: 2973 0a7b 2528 7079 3629 7320 3d20 2528  )s.{%(py6)s = %(
-00000b70: 7079 3229 7328 6d69 6e75 7465 733d 2528  py2)s(minutes=%(
-00000b80: 7079 3429 7329 0a7d 2929 0a7d 7a62 6173  py4)s).})).}zbas
-00000b90: 7365 7274 206e 6f74 2025 2870 7939 2973  sert not %(py9)s
-00000ba0: 0a7b 2528 7079 3929 7320 3d20 2528 7079  .{%(py9)s = %(py
-00000bb0: 3029 7328 2825 2870 7931 2973 202b 2025  0)s((%(py1)s + %
-00000bc0: 2870 7936 2973 0a7b 2528 7079 3629 7320  (py6)s.{%(py6)s 
-00000bd0: 3d20 2528 7079 3229 7328 6d69 6e75 7465  = %(py2)s(minute
-00000be0: 733d 2528 7079 3429 7329 0a7d 2929 0a7d  s=%(py4)s).})).}
-00000bf0: 290d 7202 0000 0072 2200 0000 7204 0000  ).r....r"...r...
-00000c00: 0072 2b00 0000 7203 0000 0072 0600 0000  .r+...r....r....
-00000c10: 7212 0000 0072 1300 0000 720f 0000 0072  r....r....r....r
-00000c20: 1400 0000 7211 0000 0072 1500 0000 7216  ....r....r....r.
-00000c30: 0000 0029 0872 2200 0000 da0b 4070 795f  ...).r".....@py_
-00000c40: 6173 7365 7274 33da 0b40 7079 5f61 7373  assert3..@py_ass
-00000c50: 6572 7435 da0b 4070 795f 6173 7365 7274  ert5..@py_assert
-00000c60: 3772 3100 0000 da0c 4070 795f 666f 726d  7r1.....@py_form
-00000c70: 6174 3130 5a0c 4070 795f 6173 7365 7274  at10Z.@py_assert
-00000c80: 3130 7233 0000 0072 1b00 0000 721b 0000  10r3...r....r...
-00000c90: 0072 1c00 0000 da19 7465 7374 5f63 6865  .r......test_che
-00000ca0: 636b 5f6d 6178 5f6f 6666 7365 745f 6e6f  ck_max_offset_no
-00000cb0: 7716 0000 0073 0a00 0000 0e01 c802 c801  w....s..........
-00000cc0: dc01 e401 723e 0000 0029 10da 0862 7569  ....r>...)...bui
-00000cd0: 6c74 696e 7372 1200 0000 da19 5f70 7974  ltinsr......_pyt
-00000ce0: 6573 742e 6173 7365 7274 696f 6e2e 7265  est.assertion.re
-00000cf0: 7772 6974 65da 0961 7373 6572 7469 6f6e  write..assertion
-00000d00: da07 7265 7772 6974 6572 0f00 0000 7202  ..rewriter....r.
-00000d10: 0000 0072 0300 0000 7204 0000 00da 0464  ...r....r......d
-00000d20: 6174 6572 0600 0000 7207 0000 0072 0800  ater....r....r..
-00000d30: 0000 721d 0000 0072 3400 0000 723e 0000  ..r....r4...r>..
-00000d40: 0072 1b00 0000 721b 0000 0072 1b00 0000  .r....r....r....
-00000d50: 721c 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
-00000d60: 0000 0073 0a00 0000 2e00 1402 0803 0806  ...s............
-00000d70: 0c0a                                     ..
+000002c0: 7267 2f62 6f76 696e 652f 626f 7669 6e65  rg/bovine/bovine
+000002d0: 2f62 6f76 696e 652f 626f 7669 6e65 2f75  /bovine/bovine/u
+000002e0: 7469 6c73 2f74 6573 745f 6461 7465 2e70  tils/test_date.p
+000002f0: 79da 1074 6573 745f 6765 745f 676d 745f  y..test_get_gmt_
+00000300: 6e6f 7706 0000 0073 0400 0000 0601 7c02  now....s......|.
+00000310: 721d 0000 0063 0000 0000 0000 0000 0000  r....c..........
+00000320: 0000 0b00 0000 0800 0000 4300 0000 7388  ..........C...s.
+00000330: 0100 0074 0083 007d 0074 017c 0083 017d  ...t...}.t.|...}
+00000340: 0174 026a 0374 046a 0564 018d 017d 027c  .t.j.t.j.d...}.|
+00000350: 017c 026b 017d 037c 0373 5174 06a0 0764  .|.k.}.|.sQt...d
+00000360: 027c 0366 0164 037c 017c 0266 02a1 0464  .|.f.d.|.|.f...d
+00000370: 0474 08a0 09a1 0076 0073 2974 06a0 0a7c  .t.....v.s)t...|
+00000380: 01a1 0172 2e74 06a0 0b7c 01a1 016e 0164  ...r.t...|...n.d
+00000390: 0464 0574 08a0 09a1 0076 0073 3a74 06a0  .d.t.....v.s:t..
+000003a0: 0a7c 02a1 0172 3f74 06a0 0b7c 02a1 016e  .|...r?t...|...n
+000003b0: 0164 0564 069c 0216 007d 0464 0764 087c  .d.d.....}.d.d.|
+000003c0: 0469 0116 007d 0574 0c74 06a0 0d7c 05a1  .i...}.t.t...|..
+000003d0: 0183 0182 0164 007d 0364 097d 0674 0e7c  .....d.}.d.}.t.|
+000003e0: 0664 0a8d 017d 077c 027c 0718 007d 087c  .d...}.|.|...}.|
+000003f0: 017c 086b 057d 037c 0373 ba74 06a0 0764  .|.k.}.|.s.t...d
+00000400: 0b7c 0366 0164 0c7c 017c 0866 02a1 0464  .|.f.d.|.|.f...d
+00000410: 0474 08a0 09a1 0076 0073 7974 06a0 0a7c  .t.....v.syt...|
+00000420: 01a1 0172 7e74 06a0 0b7c 01a1 016e 0164  ...r~t...|...n.d
+00000430: 0464 0574 08a0 09a1 0076 0073 8a74 06a0  .d.t.....v.s.t..
+00000440: 0a7c 02a1 0172 8f74 06a0 0b7c 02a1 016e  .|...r.t...|...n
+00000450: 0164 0564 0d74 08a0 09a1 0076 0073 9b74  .d.d.t.....v.s.t
+00000460: 06a0 0a74 0ea1 0172 a074 06a0 0b74 0ea1  ...t...r.t...t..
+00000470: 016e 0164 0d74 06a0 0b7c 06a1 0174 06a0  .n.d.t...|...t..
+00000480: 0b7c 07a1 0164 0e9c 0516 007d 0964 0f64  .|...d.....}.d.d
+00000490: 107c 0969 0116 007d 0a74 0c74 06a0 0d7c  .|.i...}.t.t...|
+000004a0: 0aa1 0183 0182 0164 0004 007d 0304 007d  .......d...}...}
+000004b0: 0604 007d 077d 0864 0053 0029 114e a901  ...}.}.d.S.).N..
+000004c0: da02 747a 2901 fa02 3c3d 2901 7a12 2528  ..tz)...<=).z.%(
+000004d0: 7079 3029 7320 3c3d 2025 2870 7932 2973  py0)s <= %(py2)s
+000004e0: da06 7061 7273 6564 da03 6e6f 7729 02da  ..parsed..now)..
+000004f0: 0370 7930 da03 7079 327a 0e61 7373 6572  .py0..py2z.asser
+00000500: 7420 2528 7079 3429 73da 0370 7934 e905  t %(py4)s..py4..
+00000510: 0000 0029 01da 0773 6563 6f6e 6473 2901  ...)...seconds).
+00000520: fa02 3e3d 2901 7a44 2528 7079 3029 7320  ..>=).zD%(py0)s 
+00000530: 3e3d 2028 2528 7079 3229 7320 2d20 2528  >= (%(py2)s - %(
+00000540: 7079 3729 730a 7b25 2870 7937 2973 203d  py7)s.{%(py7)s =
+00000550: 2025 2870 7933 2973 2873 6563 6f6e 6473   %(py3)s(seconds
+00000560: 3d25 2870 7935 2973 290a 7d29 7203 0000  =%(py5)s).})r...
+00000570: 0029 0572 2300 0000 7224 0000 0072 0d00  .).r#...r$...r..
+00000580: 0000 720e 0000 00da 0370 7937 7a0f 6173  ..r......py7z.as
+00000590: 7365 7274 2025 2870 7931 3029 73da 0470  sert %(py10)s..p
+000005a0: 7931 3029 0f72 0700 0000 7208 0000 0072  y10).r....r....r
+000005b0: 0200 0000 7222 0000 0072 0400 0000 da03  ....r"...r......
+000005c0: 7574 6372 0f00 0000 7210 0000 0072 1200  utcr....r....r..
+000005d0: 0000 7213 0000 0072 1400 0000 7211 0000  ..r....r....r...
+000005e0: 0072 1500 0000 7216 0000 0072 0300 0000  .r....r....r....
+000005f0: 290b 720b 0000 0072 2100 0000 7222 0000  ).r....r!...r"..
+00000600: 00da 0b40 7079 5f61 7373 6572 7431 da0b  ...@py_assert1..
+00000610: 4070 795f 666f 726d 6174 33da 0b40 7079  @py_format3..@py
+00000620: 5f66 6f72 6d61 7435 da0b 4070 795f 6173  _format5..@py_as
+00000630: 7365 7274 34da 0b40 7079 5f61 7373 6572  sert4..@py_asser
+00000640: 7436 da0b 4070 795f 6173 7365 7274 38da  t6..@py_assert8.
+00000650: 0b40 7079 5f66 6f72 6d61 7439 da0c 4070  .@py_format9..@p
+00000660: 795f 666f 726d 6174 3131 721b 0000 0072  y_format11r....r
+00000670: 1b00 0000 721c 0000 00da 0e74 6573 745f  ....r......test_
+00000680: 7061 7273 655f 676d 740c 0000 0073 0a00  parse_gmt....s..
+00000690: 0000 0601 0802 0e01 8a02 e201 7234 0000  ............r4..
+000006a0: 0063 0000 0000 0000 0000 0000 0000 0800  .c..............
+000006b0: 0000 0900 0000 4300 0000 735e 0300 0074  ......C...s^...t
+000006c0: 006a 0174 026a 0364 018d 017d 0064 027d  .j.t.j.d...}.d.}
+000006d0: 0174 047c 0164 038d 017d 027c 007c 0218  .t.|.d...}.|.|..
+000006e0: 007d 0374 057c 0383 017d 047c 0473 6364  .}.t.|...}.|.scd
+000006f0: 0464 0574 06a0 07a1 0076 0073 2474 08a0  .d.t.....v.s$t..
+00000700: 0974 05a1 0172 2974 08a0 0a74 05a1 016e  .t...r)t...t...n
+00000710: 0164 0564 0674 06a0 07a1 0076 0073 3574  .d.d.t.....v.s5t
+00000720: 08a0 097c 00a1 0172 3a74 08a0 0a7c 00a1  ...|...r:t...|..
+00000730: 016e 0164 0664 0774 06a0 07a1 0076 0073  .n.d.d.t.....v.s
+00000740: 4674 08a0 0974 04a1 0172 4b74 08a0 0a74  Ft...t...rKt...t
+00000750: 04a1 016e 0164 0774 08a0 0a7c 01a1 0174  ...n.d.t...|...t
+00000760: 08a0 0a7c 02a1 0174 08a0 0a7c 04a1 0164  ...|...t...|...d
+00000770: 089c 0616 007d 0574 0b74 08a0 0c7c 05a1  .....}.t.t...|..
+00000780: 0183 0182 0164 0004 007d 0104 007d 0204  .....d...}...}..
+00000790: 007d 037d 0464 027d 0174 047c 0164 038d  .}.}.d.}.t.|.d..
+000007a0: 017d 027c 007c 0217 007d 0374 057c 0383  .}.|.|...}.t.|..
+000007b0: 017d 047c 0473 c764 0964 0574 06a0 07a1  .}.|.s.d.d.t....
+000007c0: 0076 0073 8874 08a0 0974 05a1 0172 8d74  .v.s.t...t...r.t
+000007d0: 08a0 0a74 05a1 016e 0164 0564 0674 06a0  ...t...n.d.d.t..
+000007e0: 07a1 0076 0073 9974 08a0 097c 00a1 0172  ...v.s.t...|...r
+000007f0: 9e74 08a0 0a7c 00a1 016e 0164 0664 0774  .t...|...n.d.d.t
+00000800: 06a0 07a1 0076 0073 aa74 08a0 0974 04a1  .....v.s.t...t..
+00000810: 0172 af74 08a0 0a74 04a1 016e 0164 0774  .r.t...t...n.d.t
+00000820: 08a0 0a7c 01a1 0174 08a0 0a7c 02a1 0174  ...|...t...|...t
+00000830: 08a0 0a7c 04a1 0164 089c 0616 007d 0574  ...|...d.....}.t
+00000840: 0b74 08a0 0c7c 05a1 0183 0182 0164 0004  .t...|.......d..
+00000850: 007d 0104 007d 0204 007d 037d 0464 0a7d  .}...}...}.}.d.}
+00000860: 0174 047c 0164 038d 017d 027c 007c 0218  .t.|.d...}.|.|..
+00000870: 007d 0374 057c 0383 017d 047c 040c 007d  .}.t.|...}.|...}
+00000880: 067c 0690 0173 3364 0b64 0574 06a0 07a1  .|...s3d.d.t....
+00000890: 0076 0073 f074 08a0 0974 05a1 0172 f574  .v.s.t...t...r.t
+000008a0: 08a0 0a74 05a1 016e 0164 0564 0674 06a0  ...t...n.d.d.t..
+000008b0: 07a1 0076 0090 0173 0374 08a0 097c 00a1  ...v...s.t...|..
+000008c0: 0190 0172 0874 08a0 0a7c 00a1 016e 0164  ...r.t...|...n.d
+000008d0: 0664 0774 06a0 07a1 0076 0090 0173 1674  .d.t.....v...s.t
+000008e0: 08a0 0974 04a1 0190 0172 1b74 08a0 0a74  ...t.....r.t...t
+000008f0: 04a1 016e 0164 0774 08a0 0a7c 01a1 0174  ...n.d.t...|...t
+00000900: 08a0 0a7c 02a1 0174 08a0 0a7c 04a1 0164  ...|...t...|...d
+00000910: 089c 0616 007d 0774 0b74 08a0 0c7c 07a1  .....}.t.t...|..
+00000920: 0183 0182 0164 0004 007d 0104 007d 0204  .....d...}...}..
+00000930: 007d 0304 007d 047d 0664 0a7d 0174 047c  .}...}.}.d.}.t.|
+00000940: 0164 038d 017d 027c 007c 0217 007d 0374  .d...}.|.|...}.t
+00000950: 057c 0383 017d 047c 040c 007d 067c 0690  .|...}.|...}.|..
+00000960: 0173 a364 0c64 0574 06a0 07a1 0076 0090  .s.d.d.t.....v..
+00000970: 0173 6074 08a0 0974 05a1 0190 0172 6574  .s`t...t.....ret
+00000980: 08a0 0a74 05a1 016e 0164 0564 0674 06a0  ...t...n.d.d.t..
+00000990: 07a1 0076 0090 0173 7374 08a0 097c 00a1  ...v...sst...|..
+000009a0: 0190 0172 7874 08a0 0a7c 00a1 016e 0164  ...rxt...|...n.d
+000009b0: 0664 0774 06a0 07a1 0076 0090 0173 8674  .d.t.....v...s.t
+000009c0: 08a0 0974 04a1 0190 0172 8b74 08a0 0a74  ...t.....r.t...t
+000009d0: 04a1 016e 0164 0774 08a0 0a7c 01a1 0174  ...n.d.t...|...t
+000009e0: 08a0 0a7c 02a1 0174 08a0 0a7c 04a1 0164  ...|...t...|...d
+000009f0: 089c 0616 007d 0774 0b74 08a0 0c7c 07a1  .....}.t.t...|..
+00000a00: 0183 0182 0164 0004 007d 0104 007d 0204  .....d...}...}..
+00000a10: 007d 0304 007d 047d 0664 0053 0029 0d4e  .}...}.}.d.S.).N
+00000a20: 721e 0000 00e9 0400 0000 2901 da07 6d69  r.........)...mi
+00000a30: 6e75 7465 737a 5e61 7373 6572 7420 2528  nutesz^assert %(
+00000a40: 7079 3929 730a 7b25 2870 7939 2973 203d  py9)s.{%(py9)s =
+00000a50: 2025 2870 7930 2973 2828 2528 7079 3129   %(py0)s((%(py1)
+00000a60: 7320 2d20 2528 7079 3629 730a 7b25 2870  s - %(py6)s.{%(p
+00000a70: 7936 2973 203d 2025 2870 7932 2973 286d  y6)s = %(py2)s(m
+00000a80: 696e 7574 6573 3d25 2870 7934 2973 290a  inutes=%(py4)s).
+00000a90: 7d29 290a 7d72 0600 0000 7222 0000 0072  })).}r....r"...r
+00000aa0: 0300 0000 2906 7223 0000 0072 0c00 0000  ....).r#...r....
+00000ab0: 7224 0000 0072 2500 0000 da03 7079 36da  r$...r%.....py6.
+00000ac0: 0370 7939 7a5e 6173 7365 7274 2025 2870  .py9z^assert %(p
+00000ad0: 7939 2973 0a7b 2528 7079 3929 7320 3d20  y9)s.{%(py9)s = 
+00000ae0: 2528 7079 3029 7328 2825 2870 7931 2973  %(py0)s((%(py1)s
+00000af0: 202b 2025 2870 7936 2973 0a7b 2528 7079   + %(py6)s.{%(py
+00000b00: 3629 7320 3d20 2528 7079 3229 7328 6d69  6)s = %(py2)s(mi
+00000b10: 6e75 7465 733d 2528 7079 3429 7329 0a7d  nutes=%(py4)s).}
+00000b20: 2929 0a7d e906 0000 007a 6261 7373 6572  )).}.....zbasser
+00000b30: 7420 6e6f 7420 2528 7079 3929 730a 7b25  t not %(py9)s.{%
+00000b40: 2870 7939 2973 203d 2025 2870 7930 2973  (py9)s = %(py0)s
+00000b50: 2828 2528 7079 3129 7320 2d20 2528 7079  ((%(py1)s - %(py
+00000b60: 3629 730a 7b25 2870 7936 2973 203d 2025  6)s.{%(py6)s = %
+00000b70: 2870 7932 2973 286d 696e 7574 6573 3d25  (py2)s(minutes=%
+00000b80: 2870 7934 2973 290a 7d29 290a 7d7a 6261  (py4)s).})).}zba
+00000b90: 7373 6572 7420 6e6f 7420 2528 7079 3929  ssert not %(py9)
+00000ba0: 730a 7b25 2870 7939 2973 203d 2025 2870  s.{%(py9)s = %(p
+00000bb0: 7930 2973 2828 2528 7079 3129 7320 2b20  y0)s((%(py1)s + 
+00000bc0: 2528 7079 3629 730a 7b25 2870 7936 2973  %(py6)s.{%(py6)s
+00000bd0: 203d 2025 2870 7932 2973 286d 696e 7574   = %(py2)s(minut
+00000be0: 6573 3d25 2870 7934 2973 290a 7d29 290a  es=%(py4)s).})).
+00000bf0: 7d29 0d72 0200 0000 7222 0000 0072 0400  }).r....r"...r..
+00000c00: 0000 722b 0000 0072 0300 0000 7206 0000  ..r+...r....r...
+00000c10: 0072 1200 0000 7213 0000 0072 0f00 0000  .r....r....r....
+00000c20: 7214 0000 0072 1100 0000 7215 0000 0072  r....r....r....r
+00000c30: 1600 0000 2908 7222 0000 00da 0b40 7079  ....).r".....@py
+00000c40: 5f61 7373 6572 7433 da0b 4070 795f 6173  _assert3..@py_as
+00000c50: 7365 7274 35da 0b40 7079 5f61 7373 6572  sert5..@py_asser
+00000c60: 7437 7231 0000 00da 0c40 7079 5f66 6f72  t7r1.....@py_for
+00000c70: 6d61 7431 305a 0c40 7079 5f61 7373 6572  mat10Z.@py_asser
+00000c80: 7431 3072 3300 0000 721b 0000 0072 1b00  t10r3...r....r..
+00000c90: 0000 721c 0000 00da 1974 6573 745f 6368  ..r......test_ch
+00000ca0: 6563 6b5f 6d61 785f 6f66 6673 6574 5f6e  eck_max_offset_n
+00000cb0: 6f77 1600 0000 730a 0000 000e 01c8 02c8  ow....s.........
+00000cc0: 01dc 01e4 0172 3e00 0000 2910 da08 6275  .....r>...)...bu
+00000cd0: 696c 7469 6e73 7212 0000 00da 195f 7079  iltinsr......_py
+00000ce0: 7465 7374 2e61 7373 6572 7469 6f6e 2e72  test.assertion.r
+00000cf0: 6577 7269 7465 da09 6173 7365 7274 696f  ewrite..assertio
+00000d00: 6eda 0772 6577 7269 7465 720f 0000 0072  n..rewriter....r
+00000d10: 0200 0000 7203 0000 0072 0400 0000 da04  ....r....r......
+00000d20: 6461 7465 7206 0000 0072 0700 0000 7208  dater....r....r.
+00000d30: 0000 0072 1d00 0000 7234 0000 0072 3e00  ...r....r4...r>.
+00000d40: 0000 721b 0000 0072 1b00 0000 721b 0000  ..r....r....r...
+00000d50: 0072 1c00 0000 da08 3c6d 6f64 756c 653e  .r......<module>
+00000d60: 0100 0000 730a 0000 002e 0014 0208 0308  ....s...........
+00000d70: 060c 0a                                  ...
```

### Comparing `bovine-0.1.0/bovine/utils/__pycache__/test_parse.cpython-310-pytest-7.3.0.pyc` & `bovine-0.1.1/bovine/utils/__pycache__/test_parse.cpython-310-pytest-7.3.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 13 15:55:57 2023 UTC, .py size: 457 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0d26 3864 c901 0000  o........&8d....
+00000000: 6f0d 0d0a 0000 0000 a4ea 3a64 c401 0000  o.........:d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 3200 0000 6400  .....@...s2...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6402 6403 6c06 6d07  ..m.Z...d.d.l.m.
 00000050: 5a07 0100 6404 6405 8400 5a08 6401 5300  Z...d.d...Z.d.S.
 00000060: 2906 e900 0000 004e e901 0000 0029 01da  )......N.....)..
 00000070: 1670 6172 7365 5f66 6564 6976 6572 7365  .parse_fediverse
@@ -82,24 +82,23 @@
 00000510: 6f72 da13 5f66 6f72 6d61 745f 6578 706c  or.._format_expl
 00000520: 616e 6174 696f 6e29 06da 0b40 7079 5f61  anation)...@py_a
 00000530: 7373 6572 7431 da0b 4070 795f 6173 7365  ssert1..@py_asse
 00000540: 7274 33da 0b40 7079 5f61 7373 6572 7436  rt3..@py_assert6
 00000550: da0b 4070 795f 6173 7365 7274 35da 0b40  ..@py_assert5..@
 00000560: 7079 5f66 6f72 6d61 7438 da0c 4070 795f  py_format8..@py_
 00000570: 666f 726d 6174 3130 a900 721a 0000 00fa  format10..r.....
-00000580: 4b2f 776f 6f64 7065 636b 6572 2f73 7263  K/woodpecker/src
-00000590: 2f63 6f64 6562 6572 672e 6f72 672f 6865  /codeberg.org/he
-000005a0: 6c67 652f 626f 7669 6e65 2f62 6f76 696e  lge/bovine/bovin
-000005b0: 652f 626f 7669 6e65 2f75 7469 6c73 2f74  e/bovine/utils/t
-000005c0: 6573 745f 7061 7273 652e 7079 da1b 7465  est_parse.py..te
-000005d0: 7374 5f70 6172 7365 5f66 6564 6976 6572  st_parse_fediver
-000005e0: 7365 5f68 616e 646c 6504 0000 0073 0a00  se_handle....s..
-000005f0: 0000 9c01 9c01 9c02 a201 a601 721c 0000  ............r...
-00000600: 0029 09da 0862 7569 6c74 696e 7372 0e00  .)...builtinsr..
-00000610: 0000 da19 5f70 7974 6573 742e 6173 7365  ...._pytest.asse
-00000620: 7274 696f 6e2e 7265 7772 6974 65da 0961  rtion.rewrite..a
-00000630: 7373 6572 7469 6f6e da07 7265 7772 6974  ssertion..rewrit
-00000640: 6572 0c00 0000 da05 7061 7273 6572 0300  er......parser..
-00000650: 0000 721c 0000 0072 1a00 0000 721a 0000  ..r....r....r...
-00000660: 0072 1a00 0000 721b 0000 00da 083c 6d6f  .r....r......<mo
-00000670: 6475 6c65 3e01 0000 0073 0400 0000 2600  dule>....s....&.
-00000680: 0c03                                     ..
+00000580: 4c2f 776f 6f64 7065 636b 6572 2f73 7263  L/woodpecker/src
+00000590: 2f63 6f64 6562 6572 672e 6f72 672f 626f  /codeberg.org/bo
+000005a0: 7669 6e65 2f62 6f76 696e 652f 626f 7669  vine/bovine/bovi
+000005b0: 6e65 2f62 6f76 696e 652f 7574 696c 732f  ne/bovine/utils/
+000005c0: 7465 7374 5f70 6172 7365 2e70 79da 1b74  test_parse.py..t
+000005d0: 6573 745f 7061 7273 655f 6665 6469 7665  est_parse_fedive
+000005e0: 7273 655f 6861 6e64 6c65 0400 0000 730a  rse_handle....s.
+000005f0: 0000 009c 019c 019c 02a2 01a6 0172 1c00  .............r..
+00000600: 0000 2909 da08 6275 696c 7469 6e73 720e  ..)...builtinsr.
+00000610: 0000 00da 195f 7079 7465 7374 2e61 7373  ....._pytest.ass
+00000620: 6572 7469 6f6e 2e72 6577 7269 7465 da09  ertion.rewrite..
+00000630: 6173 7365 7274 696f 6eda 0772 6577 7269  assertion..rewri
+00000640: 7465 720c 0000 00da 0072 0300 0000 721c  ter......r....r.
+00000650: 0000 0072 1a00 0000 721a 0000 0072 1a00  ...r....r....r..
+00000660: 0000 721b 0000 00da 083c 6d6f 6475 6c65  ..r......<module
+00000670: 3e01 0000 0073 0400 0000 2600 0c03       >....s....&...
```

### Comparing `bovine-0.1.0/bovine/utils/__pycache__/test_webfinger.cpython-310-pytest-7.3.0.pyc` & `bovine-0.1.1/bovine/utils/__pycache__/test_webfinger.cpython-310-pytest-7.3.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 13 15:55:57 2023 UTC, .py size: 200 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0d26 3864 c800 0000  o........&8d....
+00000000: 6f0d 0d0a 0000 0000 a4ea 3a64 bf00 0000  o.........:d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 3200 0000 6400  .....@...s2...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6402 6403 6c06 6d07  ..m.Z...d.d.l.m.
 00000050: 5a07 0100 6404 6405 8400 5a08 6401 5300  Z...d.d...Z.d.S.
 00000060: 2906 e900 0000 004e e901 0000 0029 01da  )......N.....)..
 00000070: 1777 6562 6669 6e67 6572 5f72 6573 706f  .webfinger_respo
@@ -39,24 +39,23 @@
 00000260: 756c 645f 7265 7072 5f67 6c6f 6261 6c5f  uld_repr_global_
 00000270: 6e61 6d65 da0e 4173 7365 7274 696f 6e45  name..AssertionE
 00000280: 7272 6f72 da13 5f66 6f72 6d61 745f 6578  rror.._format_ex
 00000290: 706c 616e 6174 696f 6e29 0572 0900 0000  planation).r....
 000002a0: da0b 4070 795f 6173 7365 7274 30da 0b40  ..@py_assert0..@
 000002b0: 7079 5f61 7373 6572 7432 da0b 4070 795f  py_assert2..@py_
 000002c0: 666f 726d 6174 34da 0b40 7079 5f66 6f72  format4..@py_for
-000002d0: 6d61 7436 a900 721a 0000 00fa 4f2f 776f  mat6..r.....O/wo
+000002d0: 6d61 7436 a900 721a 0000 00fa 502f 776f  mat6..r.....P/wo
 000002e0: 6f64 7065 636b 6572 2f73 7263 2f63 6f64  odpecker/src/cod
-000002f0: 6562 6572 672e 6f72 672f 6865 6c67 652f  eberg.org/helge/
-00000300: 626f 7669 6e65 2f62 6f76 696e 652f 626f  bovine/bovine/bo
-00000310: 7669 6e65 2f75 7469 6c73 2f74 6573 745f  vine/utils/test_
-00000320: 7765 6266 696e 6765 722e 7079 da0e 7465  webfinger.py..te
-00000330: 7374 5f77 6562 6669 6e67 6572 0400 0000  st_webfinger....
-00000340: 7306 0000 000c 0178 027c 0172 1c00 0000  s......x.|.r....
-00000350: 2909 da08 6275 696c 7469 6e73 7211 0000  )...builtinsr...
-00000360: 00da 195f 7079 7465 7374 2e61 7373 6572  ..._pytest.asser
-00000370: 7469 6f6e 2e72 6577 7269 7465 da09 6173  tion.rewrite..as
-00000380: 7365 7274 696f 6eda 0772 6577 7269 7465  sertion..rewrite
-00000390: 720e 0000 005a 0977 6562 6669 6e67 6572  r....Z.webfinger
-000003a0: 7203 0000 0072 1c00 0000 721a 0000 0072  r....r....r....r
-000003b0: 1a00 0000 721a 0000 0072 1b00 0000 da08  ....r....r......
-000003c0: 3c6d 6f64 756c 653e 0100 0000 7304 0000  <module>....s...
-000003d0: 0026 000c 03                             .&...
+000002f0: 6562 6572 672e 6f72 672f 626f 7669 6e65  eberg.org/bovine
+00000300: 2f62 6f76 696e 652f 626f 7669 6e65 2f62  /bovine/bovine/b
+00000310: 6f76 696e 652f 7574 696c 732f 7465 7374  ovine/utils/test
+00000320: 5f77 6562 6669 6e67 6572 2e70 79da 0e74  _webfinger.py..t
+00000330: 6573 745f 7765 6266 696e 6765 7204 0000  est_webfinger...
+00000340: 0073 0600 0000 0c01 7802 7c01 721c 0000  .s......x.|.r...
+00000350: 0029 09da 0862 7569 6c74 696e 7372 1100  .)...builtinsr..
+00000360: 0000 da19 5f70 7974 6573 742e 6173 7365  ...._pytest.asse
+00000370: 7274 696f 6e2e 7265 7772 6974 65da 0961  rtion.rewrite..a
+00000380: 7373 6572 7469 6f6e da07 7265 7772 6974  ssertion..rewrit
+00000390: 6572 0e00 0000 da00 7203 0000 0072 1c00  er......r....r..
+000003a0: 0000 721a 0000 0072 1a00 0000 721a 0000  ..r....r....r...
+000003b0: 0072 1b00 0000 da08 3c6d 6f64 756c 653e  .r......<module>
+000003c0: 0100 0000 7304 0000 0026 000c 03         ....s....&...
```

### Comparing `bovine-0.1.0/bovine/utils/date.py` & `bovine-0.1.1/bovine/utils/date.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.0/bovine/utils/test_date.py` & `bovine-0.1.1/bovine/utils/test_date.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.0/pyproject.toml` & `bovine-0.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "bovine"
-version = "0.1.0"
-description = "Core functionality of bovine needed to build client to server applications"
+version = "0.1.1"
+description = "Core functionality of bovine needed to build FediVerse applications"
 authors = ["Helge <helge.krueger@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "bovine" }]
-repository = "https://codeberg.org/helge/bovine"
+repository = "https://codeberg.org/bovine/bovine"
 documentation = "https://bovine.readthedocs.io/en/latest/"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 aiohttp = "^3.8.3"
 cryptography = "^39.0.0"
 python-dateutil = "^2.8.2"
```

