# Comparing `tmp/shikithon-2.4.1.tar.gz` & `tmp/shikithon-2.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shikithon-2.4.1.tar", max compression
+gzip compressed data, was "shikithon-2.4.2.tar", max compression
```

## Comparing `shikithon-2.4.1.tar` & `shikithon-2.4.2.tar`

### file list

```diff
@@ -1,131 +1,131 @@
--rw-r--r--   0        0        0     1070 2023-03-27 22:04:22.002118 shikithon-2.4.1/LICENSE
--rw-r--r--   0        0        0    12386 2023-03-27 22:04:22.002118 shikithon-2.4.1/README.md
--rw-r--r--   0        0        0     1189 2023-03-27 22:04:22.002118 shikithon-2.4.1/pyproject.toml
--rw-r--r--   0        0        0      262 2023-03-27 22:04:22.002118 shikithon-2.4.1/shikithon/__init__.py
--rw-r--r--   0        0        0     3903 2023-03-27 22:04:22.002118 shikithon-2.4.1/shikithon/api.py
--rw-r--r--   0        0        0    22004 2023-03-27 22:04:22.002118 shikithon-2.4.1/shikithon/base_client.py
--rw-r--r--   0        0        0      189 2023-03-27 22:04:22.002118 shikithon-2.4.1/shikithon/decorators/__init__.py
--rw-r--r--   0        0        0     2074 2023-03-27 22:04:22.002118 shikithon-2.4.1/shikithon/decorators/exceptions_handler.py
--rw-r--r--   0        0        0     1616 2023-03-27 22:04:22.002118 shikithon-2.4.1/shikithon/decorators/method_endpoint.py
--rw-r--r--   0        0        0    34606 2023-03-27 22:04:22.002118 shikithon-2.4.1/shikithon/endpoints.py
--rw-r--r--   0        0        0     1648 2023-03-27 22:04:22.002118 shikithon-2.4.1/shikithon/enums/__init__.py
--rw-r--r--   0        0        0     2705 2023-03-27 22:04:22.002118 shikithon-2.4.1/shikithon/enums/anime.py
--rw-r--r--   0        0        0      895 2023-03-27 22:04:22.002118 shikithon-2.4.1/shikithon/enums/club.py
--rw-r--r--   0        0        0      632 2023-03-27 22:04:22.002118 shikithon-2.4.1/shikithon/enums/comment.py
--rw-r--r--   0        0        0      310 2023-03-27 22:04:22.002118 shikithon-2.4.1/shikithon/enums/enhanced_enum.py
--rw-r--r--   0        0        0      289 2023-03-27 22:04:22.002118 shikithon-2.4.1/shikithon/enums/favorite.py
--rw-r--r--   0        0        0      222 2023-03-27 22:04:22.002118 shikithon-2.4.1/shikithon/enums/history.py
--rw-r--r--   0        0        0     1961 2023-03-27 22:04:22.002118 shikithon-2.4.1/shikithon/enums/manga.py
--rw-r--r--   0        0        0      286 2023-03-27 22:04:22.002118 shikithon-2.4.1/shikithon/enums/message.py
--rw-r--r--   0        0        0      466 2023-03-27 22:04:22.002118 shikithon-2.4.1/shikithon/enums/person.py
--rw-r--r--   0        0        0     1522 2023-03-27 22:04:22.002118 shikithon-2.4.1/shikithon/enums/ranobe.py
--rw-r--r--   0        0        0      240 2023-03-27 22:04:22.002118 shikithon-2.4.1/shikithon/enums/request.py
--rw-r--r--   0        0        0      218 2023-03-27 22:04:22.002118 shikithon-2.4.1/shikithon/enums/response.py
--rw-r--r--   0        0        0      198 2023-03-27 22:04:22.002118 shikithon-2.4.1/shikithon/enums/style.py
--rw-r--r--   0        0        0     1999 2023-03-27 22:04:22.002118 shikithon-2.4.1/shikithon/enums/topic.py
--rw-r--r--   0        0        0      685 2023-03-27 22:04:22.002118 shikithon-2.4.1/shikithon/enums/user_rate.py
--rw-r--r--   0        0        0      380 2023-03-27 22:04:22.002118 shikithon-2.4.1/shikithon/enums/video.py
--rw-r--r--   0        0        0      657 2023-03-27 22:04:22.002118 shikithon-2.4.1/shikithon/exceptions/__init__.py
--rw-r--r--   0        0        0      276 2023-03-27 22:04:22.002118 shikithon-2.4.1/shikithon/exceptions/already_running_client.py
--rw-r--r--   0        0        0      329 2023-03-27 22:04:22.002118 shikithon-2.4.1/shikithon/exceptions/invalid_content_type.py
--rw-r--r--   0        0        0      732 2023-03-27 22:04:22.002118 shikithon-2.4.1/shikithon/exceptions/missing_app_variable.py
--rw-r--r--   0        0        0      231 2023-03-27 22:04:22.002118 shikithon-2.4.1/shikithon/exceptions/retry_later.py
--rw-r--r--   0        0        0      358 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/exceptions/shikimori_api_response_error.py
--rw-r--r--   0        0        0      240 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/exceptions/shikithon_exception.py
--rw-r--r--   0        0        0      234 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/exceptions/store_exception.py
--rw-r--r--   0        0        0     1689 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/models/__init__.py
--rw-r--r--   0        0        0      230 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/models/abuse_response.py
--rw-r--r--   0        0        0      303 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/models/achievement.py
--rw-r--r--   0        0        0      190 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/models/activity.py
--rw-r--r--   0        0        0     1735 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/models/anime.py
--rw-r--r--   0        0        0      410 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/models/ban.py
--rw-r--r--   0        0        0      270 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/models/birthday.py
--rw-r--r--   0        0        0      331 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/models/calendar_event.py
--rw-r--r--   0        0        0      796 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/models/character.py
--rw-r--r--   0        0        0      789 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/models/club.py
--rw-r--r--   0        0        0      290 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/models/club_image.py
--rw-r--r--   0        0        0      488 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/models/comment.py
--rw-r--r--   0        0        0      688 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/models/constants.py
--rw-r--r--   0        0        0      207 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/models/created_user_image.py
--rw-r--r--   0        0        0      218 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/models/dialog.py
--rw-r--r--   0        0        0      243 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/models/favourite.py
--rw-r--r--   0        0        0      452 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/models/favourites.py
--rw-r--r--   0        0        0      195 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/models/forum.py
--rw-r--r--   0        0        0      327 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/models/franchise_tree.py
--rw-r--r--   0        0        0      186 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/models/genre.py
--rw-r--r--   0        0        0      401 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/models/history.py
--rw-r--r--   0        0        0      196 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/models/image.py
--rw-r--r--   0        0        0      414 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/models/link.py
--rw-r--r--   0        0        0      492 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/models/linked_topic.py
--rw-r--r--   0        0        0      199 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/models/logo.py
--rw-r--r--   0        0        0     1645 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/models/manga.py
--rw-r--r--   0        0        0      564 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/models/message.py
--rw-r--r--   0        0        0      956 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/models/person.py
--rw-r--r--   0        0        0      158 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/models/publisher.py
--rw-r--r--   0        0        0     1572 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/models/ranobe.py
--rw-r--r--   0        0        0      161 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/models/rating.py
--rw-r--r--   0        0        0      277 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/models/rating_list.py
--rw-r--r--   0        0        0      379 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/models/relation.py
--rw-r--r--   0        0        0      356 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/models/role.py
--rw-r--r--   0        0        0      271 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/models/roles.py
--rw-r--r--   0        0        0      158 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/models/score.py
--rw-r--r--   0        0        0      241 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/models/score_list.py
--rw-r--r--   0        0        0      171 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/models/screenshot.py
--rw-r--r--   0        0        0      234 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/models/seyu.py
--rw-r--r--   0        0        0      857 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/models/stats.py
--rw-r--r--   0        0        0      206 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/models/status.py
--rw-r--r--   0        0        0      246 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/models/status_list.py
--rw-r--r--   0        0        0      249 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/models/studio.py
--rw-r--r--   0        0        0      388 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/models/style.py
--rw-r--r--   0        0        0      808 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/models/topic.py
--rw-r--r--   0        0        0      252 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/models/tree_link.py
--rw-r--r--   0        0        0      301 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/models/tree_node.py
--rw-r--r--   0        0        0      155 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/models/type.py
--rw-r--r--   0        0        0      235 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/models/type_list.py
--rw-r--r--   0        0        0      243 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/models/unread_messages.py
--rw-r--r--   0        0        0      853 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/models/user.py
--rw-r--r--   0        0        0      229 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/models/user_image.py
--rw-r--r--   0        0        0      703 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/models/user_list.py
--rw-r--r--   0        0        0      538 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/models/user_rate.py
--rw-r--r--   0        0        0      167 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/models/user_rate_score.py
--rw-r--r--   0        0        0      169 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/models/user_rate_status.py
--rw-r--r--   0        0        0      287 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/models/video.py
--rw-r--r--   0        0        0      328 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/models/works.py
--rw-r--r--   0        0        0        0 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/py.typed
--rw-r--r--   0        0        0     1294 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/resources/__init__.py
--rw-r--r--   0        0        0     4703 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/resources/abuse_requests.py
--rw-r--r--   0        0        0     1173 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/resources/achievements.py
--rw-r--r--   0        0        0    14250 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/resources/animes.py
--rw-r--r--   0        0        0     1157 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/resources/appears.py
--rw-r--r--   0        0        0     1316 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/resources/bans.py
--rw-r--r--   0        0        0      162 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/resources/base_resource.py
--rw-r--r--   0        0        0     1291 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/resources/calendars.py
--rw-r--r--   0        0        0     1813 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/resources/characters.py
--rw-r--r--   0        0        0    12292 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/resources/clubs.py
--rw-r--r--   0        0        0     6300 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/resources/comments.py
--rw-r--r--   0        0        0     3222 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/resources/constants.py
--rw-r--r--   0        0        0     2437 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/resources/dialogs.py
--rw-r--r--   0        0        0     3682 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/resources/favorites.py
--rw-r--r--   0        0        0      909 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/resources/forums.py
--rw-r--r--   0        0        0     1480 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/resources/friends.py
--rw-r--r--   0        0        0      908 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/resources/genres.py
--rw-r--r--   0        0        0     9698 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/resources/mangas.py
--rw-r--r--   0        0        0     6548 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/resources/messages.py
--rw-r--r--   0        0        0     2005 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/resources/people.py
--rw-r--r--   0        0        0      952 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/resources/publishers.py
--rw-r--r--   0        0        0     9513 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/resources/ranobes.py
--rw-r--r--   0        0        0      748 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/resources/stats.py
--rw-r--r--   0        0        0      919 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/resources/studios.py
--rw-r--r--   0        0        0     4178 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/resources/styles.py
--rw-r--r--   0        0        0     9881 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/resources/topics.py
--rw-r--r--   0        0        0     1533 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/resources/user_images.py
--rw-r--r--   0        0        0    10984 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/resources/user_rates.py
--rw-r--r--   0        0        0    15779 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/resources/users.py
--rw-r--r--   0        0        0      217 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/store/__init__.py
--rw-r--r--   0        0        0     4117 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/store/base.py
--rw-r--r--   0        0        0     3143 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/store/json.py
--rw-r--r--   0        0        0     4428 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/store/memory.py
--rw-r--r--   0        0        0     1190 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/store/null.py
--rw-r--r--   0        0        0       82 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/utils/__init__.py
--rw-r--r--   0        0        0    12419 2023-03-27 22:04:22.006119 shikithon-2.4.1/shikithon/utils/utils.py
--rw-r--r--   0        0        0    13526 1970-01-01 00:00:00.000000 shikithon-2.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-04-15 16:01:18.885165 shikithon-2.4.2/LICENSE
+-rw-r--r--   0        0        0    12407 2023-04-15 16:01:18.885165 shikithon-2.4.2/README.md
+-rw-r--r--   0        0        0     1188 2023-04-15 16:01:18.885165 shikithon-2.4.2/pyproject.toml
+-rw-r--r--   0        0        0      262 2023-04-15 16:01:18.885165 shikithon-2.4.2/shikithon/__init__.py
+-rw-r--r--   0        0        0     3903 2023-04-15 16:01:18.885165 shikithon-2.4.2/shikithon/api.py
+-rw-r--r--   0        0        0    22001 2023-04-15 16:01:18.885165 shikithon-2.4.2/shikithon/base_client.py
+-rw-r--r--   0        0        0      189 2023-04-15 16:01:18.885165 shikithon-2.4.2/shikithon/decorators/__init__.py
+-rw-r--r--   0        0        0     2074 2023-04-15 16:01:18.885165 shikithon-2.4.2/shikithon/decorators/exceptions_handler.py
+-rw-r--r--   0        0        0     1616 2023-04-15 16:01:18.885165 shikithon-2.4.2/shikithon/decorators/method_endpoint.py
+-rw-r--r--   0        0        0    34606 2023-04-15 16:01:18.885165 shikithon-2.4.2/shikithon/endpoints.py
+-rw-r--r--   0        0        0     1648 2023-04-15 16:01:18.885165 shikithon-2.4.2/shikithon/enums/__init__.py
+-rw-r--r--   0        0        0     2705 2023-04-15 16:01:18.885165 shikithon-2.4.2/shikithon/enums/anime.py
+-rw-r--r--   0        0        0      895 2023-04-15 16:01:18.885165 shikithon-2.4.2/shikithon/enums/club.py
+-rw-r--r--   0        0        0      632 2023-04-15 16:01:18.885165 shikithon-2.4.2/shikithon/enums/comment.py
+-rw-r--r--   0        0        0      310 2023-04-15 16:01:18.885165 shikithon-2.4.2/shikithon/enums/enhanced_enum.py
+-rw-r--r--   0        0        0      289 2023-04-15 16:01:18.885165 shikithon-2.4.2/shikithon/enums/favorite.py
+-rw-r--r--   0        0        0      222 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/enums/history.py
+-rw-r--r--   0        0        0     1961 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/enums/manga.py
+-rw-r--r--   0        0        0      286 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/enums/message.py
+-rw-r--r--   0        0        0      466 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/enums/person.py
+-rw-r--r--   0        0        0     1522 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/enums/ranobe.py
+-rw-r--r--   0        0        0      240 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/enums/request.py
+-rw-r--r--   0        0        0      218 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/enums/response.py
+-rw-r--r--   0        0        0      198 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/enums/style.py
+-rw-r--r--   0        0        0     1999 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/enums/topic.py
+-rw-r--r--   0        0        0      685 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/enums/user_rate.py
+-rw-r--r--   0        0        0      380 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/enums/video.py
+-rw-r--r--   0        0        0      657 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/exceptions/__init__.py
+-rw-r--r--   0        0        0      276 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/exceptions/already_running_client.py
+-rw-r--r--   0        0        0      329 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/exceptions/invalid_content_type.py
+-rw-r--r--   0        0        0      732 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/exceptions/missing_app_variable.py
+-rw-r--r--   0        0        0      231 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/exceptions/retry_later.py
+-rw-r--r--   0        0        0      358 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/exceptions/shikimori_api_response_error.py
+-rw-r--r--   0        0        0      240 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/exceptions/shikithon_exception.py
+-rw-r--r--   0        0        0      234 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/exceptions/store_exception.py
+-rw-r--r--   0        0        0     1689 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/__init__.py
+-rw-r--r--   0        0        0      230 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/abuse_response.py
+-rw-r--r--   0        0        0      303 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/achievement.py
+-rw-r--r--   0        0        0      190 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/activity.py
+-rw-r--r--   0        0        0     1735 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/anime.py
+-rw-r--r--   0        0        0      410 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/ban.py
+-rw-r--r--   0        0        0      270 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/birthday.py
+-rw-r--r--   0        0        0      331 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/calendar_event.py
+-rw-r--r--   0        0        0      796 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/character.py
+-rw-r--r--   0        0        0      789 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/club.py
+-rw-r--r--   0        0        0      290 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/club_image.py
+-rw-r--r--   0        0        0      488 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/comment.py
+-rw-r--r--   0        0        0      688 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/constants.py
+-rw-r--r--   0        0        0      207 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/created_user_image.py
+-rw-r--r--   0        0        0      218 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/dialog.py
+-rw-r--r--   0        0        0      243 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/favourite.py
+-rw-r--r--   0        0        0      452 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/favourites.py
+-rw-r--r--   0        0        0      195 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/forum.py
+-rw-r--r--   0        0        0      327 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/franchise_tree.py
+-rw-r--r--   0        0        0      186 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/genre.py
+-rw-r--r--   0        0        0      401 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/history.py
+-rw-r--r--   0        0        0      196 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/image.py
+-rw-r--r--   0        0        0      414 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/link.py
+-rw-r--r--   0        0        0      492 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/linked_topic.py
+-rw-r--r--   0        0        0      199 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/logo.py
+-rw-r--r--   0        0        0     1645 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/manga.py
+-rw-r--r--   0        0        0      564 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/message.py
+-rw-r--r--   0        0        0      956 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/person.py
+-rw-r--r--   0        0        0      158 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/publisher.py
+-rw-r--r--   0        0        0     1572 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/ranobe.py
+-rw-r--r--   0        0        0      161 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/rating.py
+-rw-r--r--   0        0        0      277 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/rating_list.py
+-rw-r--r--   0        0        0      379 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/relation.py
+-rw-r--r--   0        0        0      356 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/role.py
+-rw-r--r--   0        0        0      271 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/roles.py
+-rw-r--r--   0        0        0      158 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/score.py
+-rw-r--r--   0        0        0      241 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/score_list.py
+-rw-r--r--   0        0        0      171 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/screenshot.py
+-rw-r--r--   0        0        0      234 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/seyu.py
+-rw-r--r--   0        0        0      857 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/stats.py
+-rw-r--r--   0        0        0      206 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/status.py
+-rw-r--r--   0        0        0      246 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/status_list.py
+-rw-r--r--   0        0        0      249 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/studio.py
+-rw-r--r--   0        0        0      388 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/style.py
+-rw-r--r--   0        0        0      808 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/topic.py
+-rw-r--r--   0        0        0      252 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/tree_link.py
+-rw-r--r--   0        0        0      301 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/tree_node.py
+-rw-r--r--   0        0        0      155 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/type.py
+-rw-r--r--   0        0        0      235 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/type_list.py
+-rw-r--r--   0        0        0      243 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/unread_messages.py
+-rw-r--r--   0        0        0      853 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/user.py
+-rw-r--r--   0        0        0      229 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/user_image.py
+-rw-r--r--   0        0        0      703 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/user_list.py
+-rw-r--r--   0        0        0      538 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/user_rate.py
+-rw-r--r--   0        0        0      167 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/user_rate_score.py
+-rw-r--r--   0        0        0      169 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/user_rate_status.py
+-rw-r--r--   0        0        0      287 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/video.py
+-rw-r--r--   0        0        0      328 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/works.py
+-rw-r--r--   0        0        0        0 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/py.typed
+-rw-r--r--   0        0        0     1294 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/resources/__init__.py
+-rw-r--r--   0        0        0     4703 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/resources/abuse_requests.py
+-rw-r--r--   0        0        0     1173 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/resources/achievements.py
+-rw-r--r--   0        0        0    14250 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/resources/animes.py
+-rw-r--r--   0        0        0     1157 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/resources/appears.py
+-rw-r--r--   0        0        0     1316 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/resources/bans.py
+-rw-r--r--   0        0        0      162 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/resources/base_resource.py
+-rw-r--r--   0        0        0     1291 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/resources/calendars.py
+-rw-r--r--   0        0        0     1813 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/resources/characters.py
+-rw-r--r--   0        0        0    12292 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/resources/clubs.py
+-rw-r--r--   0        0        0     6300 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/resources/comments.py
+-rw-r--r--   0        0        0     3222 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/resources/constants.py
+-rw-r--r--   0        0        0     2437 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/resources/dialogs.py
+-rw-r--r--   0        0        0     3682 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/resources/favorites.py
+-rw-r--r--   0        0        0      909 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/resources/forums.py
+-rw-r--r--   0        0        0     1480 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/resources/friends.py
+-rw-r--r--   0        0        0      908 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/resources/genres.py
+-rw-r--r--   0        0        0     9698 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/resources/mangas.py
+-rw-r--r--   0        0        0     6548 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/resources/messages.py
+-rw-r--r--   0        0        0     2005 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/resources/people.py
+-rw-r--r--   0        0        0      952 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/resources/publishers.py
+-rw-r--r--   0        0        0     9513 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/resources/ranobes.py
+-rw-r--r--   0        0        0      748 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/resources/stats.py
+-rw-r--r--   0        0        0      919 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/resources/studios.py
+-rw-r--r--   0        0        0     4178 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/resources/styles.py
+-rw-r--r--   0        0        0     9881 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/resources/topics.py
+-rw-r--r--   0        0        0     1533 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/resources/user_images.py
+-rw-r--r--   0        0        0    10984 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/resources/user_rates.py
+-rw-r--r--   0        0        0    15779 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/resources/users.py
+-rw-r--r--   0        0        0      217 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/store/__init__.py
+-rw-r--r--   0        0        0     4117 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/store/base.py
+-rw-r--r--   0        0        0     3143 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/store/json.py
+-rw-r--r--   0        0        0     4428 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/store/memory.py
+-rw-r--r--   0        0        0     1190 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/store/null.py
+-rw-r--r--   0        0        0       82 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/utils/__init__.py
+-rw-r--r--   0        0        0    12419 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/utils/utils.py
+-rw-r--r--   0        0        0    13547 1970-01-01 00:00:00.000000 shikithon-2.4.2/PKG-INFO
```

### Comparing `shikithon-2.4.1/LICENSE` & `shikithon-2.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `shikithon-2.4.1/README.md` & `shikithon-2.4.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -108,14 +108,15 @@
     async with api_auth_maker:
         ...
 
 asyncio.run(main())
 ```
 
 Выполнение нескольких запросов одновременно с помощью метода `multiple_requests`:
+
 ```py
 # В этом примере используется распаковка, но можно также получать весь массив с данными ответов
 # в одной переменнной (chainsaw, lycoris_anime, ... -> data = await ...)
 from shikithon import ShikimoriAPI, JSONStore
 
 config = ...
 
@@ -136,28 +137,28 @@
 # [Character(id=204621, name='Chisato Nishikigi', russian='Тисато Нисикиги', ...]
 # [Ranobe(id=151431, name='Lycoris Recoil: Ordinary Days', russian='Ликорис Рикоил: Повседневность', ...]
 ```
 
 Также, если хочется узнать как использовать встроенные хранилища конфигов или хочется создать свой,
 посмотрите [этот гайд](https://github.com/SecondThundeR/shikithon/wiki/%D0%93%D0%B0%D0%B9%D0%B4-%D0%BF%D0%BE-%D1%85%D1%80%D0%B0%D0%BD%D0%B8%D0%BB%D0%B8%D1%89%D0%B0%D0%BC-%D0%BA%D0%BE%D0%BD%D1%84%D0%B8%D0%B3%D1%83%D1%80%D0%B0%D1%86%D0%B8%D0%B8)
 
-#### Пара уточнений по использованию:
+### Пара уточнений по использованию
 
 - Возможно вам придется импортировать модели для ручной аннотации возвращаемых моделей в PyCharm
 _(в нем немного некорретно работает наследование типа от функции)_
 - При отсутствии каких-либо полей в данных конфигурации, библиотека выдает исключение
 - Если вы хотите использовать логгирование библиотеки, передайте флаг `logging=True` в объект API:
 `api = ShikimoriAPI(app_name="...", logging=True)`
 
-### Получение данных для конфигурации
+## Получение данных для конфигурации
 
-Для начала вам необходимо создать новое OAuth-приложение [здесь](https://shikimori.one/oauth/applications).
+Для начала вам необходимо создать новое OAuth-приложение [здесь](https://shikimori.me/oauth/applications).
 После этого, сохраните `app_name`, `client_id`, `client_secret`, а так же `redirect_uri`, если вы его меняли
 
-Позже, [на данной странице](https://shikimori.one/oauth) выберите свое приложение, необходимые разрешения
+Позже, [на данной странице](https://shikimori.me/oauth) выберите свое приложение, необходимые разрешения
 и получите код авторизации и сохраните его.
 _(Если необходимо, то можно также получить токены авторизации, пройдя следующий этап после получения кода авторизации)_
 
 ## Список изменений
 
 Все изменения перечислены на [странице релизов](https://github.com/SecondThundeR/shikithon/releases)
 
@@ -182,15 +183,16 @@
 - [loguru](https://github.com/Delgan/loguru) для удобного логгирования
 [(Лицензия)](https://github.com/Delgan/loguru/blob/master/LICENSE)
 - [validators](https://github.com/kvesteri/validators) для проверки строк на наличие ссылки в ней
 [(Лицензия)](https://github.com/kvesteri/validators/blob/master/LICENSE)
 - [typing-extensions](https://github.com/python/typing_extensions) для корректной типизации декораторов
 [(Лицензия)](https://github.com/python/typing_extensions/blob/main/LICENSE)
 
-В качестве зависимости для разработки, проект использует две зависимости:
+Также, данный проект использует две библиотеки в качестве зависимостей для разработки:
+
 - [pre-commit](https://github.com/pre-commit/pre-commit) для автоматизации форматирования и проверки кода
 [(Лицензия)](https://github.com/pre-commit/pre-commit/blob/main/LICENSE)
 - [mypy](https://github.com/python/mypy) для проверки типов [(Лицензия)](https://github.com/python/mypy/blob/master/LICENSE)
 
 ## Лицензия проекта
 
 Данный проект имеет MIT лицензию.
```

### Comparing `shikithon-2.4.1/pyproject.toml` & `shikithon-2.4.2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shikithon"
-version = "2.4.1"
+version = "2.4.2"
 description = "Yet another Python wrapper for Shikimori API"
 authors = [
     "SecondThundeR <awayfromgalaxy@gmail.com>"
 ]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/SecondThundeR/shikithon"
@@ -30,21 +30,21 @@
 ignore_missing_imports = true
 check_untyped_defs = true
 warn_redundant_casts = true
 
 [tool.poetry.dependencies]
 python = "^3.8.10"
 pydantic = "^1.10.7"
-loguru = "^0.6.0"
-validators = "^0.20.0"
+loguru = "^0.7.0"
+validators ="^0.20.0"
 aiohttp = "^3.8.4"
 pyrate-limiter = "^2.10.0"
 backoff = "^2.2.1"
 typing-extensions = "^4.5.0"
 
 [tool.poetry.group.dev.dependencies]
-pre-commit = "^3.2.1"
-mypy = "^1.1.1"
+pre-commit = "^3.2.2"
+mypy = "^1.2.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `shikithon-2.4.1/shikithon/api.py` & `shikithon-2.4.2/shikithon/api.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.4.1/shikithon/base_client.py` & `shikithon-2.4.2/shikithon/base_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,17 +19,17 @@
                          ShikimoriAPIResponseError, ShikithonException)
 from .store import NullStore, Store
 from .utils import Utils
 
 MAX_CALLS_PER_SECOND = 5
 MAX_CALLS_PER_MINUTE = 90
 
-SHIKIMORI_API_URL = 'https://shikimori.one/api'
-SHIKIMORI_API_URL_V2 = 'https://shikimori.one/api/v2'
-SHIKIMORI_OAUTH_URL = 'https://shikimori.one/oauth'
+SHIKIMORI_API_URL = 'https://shikimori.me/api'
+SHIKIMORI_API_URL_V2 = 'https://shikimori.me/api/v2'
+SHIKIMORI_OAUTH_URL = 'https://shikimori.me/oauth'
 DEFAULT_REDIRECT_URI = 'urn:ietf:wg:oauth:2.0:oob'
 
 RT = TypeVar('RT')
 
 
 class ClientConfig(TypedDict, total=False):
     app_name: str
```

### Comparing `shikithon-2.4.1/shikithon/decorators/exceptions_handler.py` & `shikithon-2.4.2/shikithon/decorators/exceptions_handler.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.4.1/shikithon/decorators/method_endpoint.py` & `shikithon-2.4.2/shikithon/decorators/method_endpoint.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.4.1/shikithon/endpoints.py` & `shikithon-2.4.2/shikithon/endpoints.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.4.1/shikithon/enums/__init__.py` & `shikithon-2.4.2/shikithon/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.4.1/shikithon/enums/anime.py` & `shikithon-2.4.2/shikithon/enums/anime.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.4.1/shikithon/enums/club.py` & `shikithon-2.4.2/shikithon/enums/club.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.4.1/shikithon/enums/comment.py` & `shikithon-2.4.2/shikithon/enums/comment.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.4.1/shikithon/enums/manga.py` & `shikithon-2.4.2/shikithon/enums/manga.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.4.1/shikithon/enums/ranobe.py` & `shikithon-2.4.2/shikithon/enums/ranobe.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.4.1/shikithon/enums/topic.py` & `shikithon-2.4.2/shikithon/enums/topic.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.4.1/shikithon/enums/user_rate.py` & `shikithon-2.4.2/shikithon/enums/user_rate.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.4.1/shikithon/exceptions/__init__.py` & `shikithon-2.4.2/shikithon/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.4.1/shikithon/exceptions/missing_app_variable.py` & `shikithon-2.4.2/shikithon/exceptions/missing_app_variable.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.4.1/shikithon/models/__init__.py` & `shikithon-2.4.2/shikithon/models/__init__.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.4.1/shikithon/models/anime.py` & `shikithon-2.4.2/shikithon/models/anime.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.4.1/shikithon/models/character.py` & `shikithon-2.4.2/shikithon/models/character.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.4.1/shikithon/models/club.py` & `shikithon-2.4.2/shikithon/models/club.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.4.1/shikithon/models/constants.py` & `shikithon-2.4.2/shikithon/models/constants.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.4.1/shikithon/models/manga.py` & `shikithon-2.4.2/shikithon/models/manga.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.4.1/shikithon/models/message.py` & `shikithon-2.4.2/shikithon/models/message.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.4.1/shikithon/models/person.py` & `shikithon-2.4.2/shikithon/models/person.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.4.1/shikithon/models/ranobe.py` & `shikithon-2.4.2/shikithon/models/ranobe.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.4.1/shikithon/models/stats.py` & `shikithon-2.4.2/shikithon/models/stats.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.4.1/shikithon/models/topic.py` & `shikithon-2.4.2/shikithon/models/topic.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.4.1/shikithon/models/user.py` & `shikithon-2.4.2/shikithon/models/user.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.4.1/shikithon/models/user_list.py` & `shikithon-2.4.2/shikithon/models/user_list.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.4.1/shikithon/models/user_rate.py` & `shikithon-2.4.2/shikithon/models/user_rate.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.4.1/shikithon/resources/__init__.py` & `shikithon-2.4.2/shikithon/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.4.1/shikithon/resources/abuse_requests.py` & `shikithon-2.4.2/shikithon/resources/abuse_requests.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.4.1/shikithon/resources/achievements.py` & `shikithon-2.4.2/shikithon/resources/achievements.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.4.1/shikithon/resources/animes.py` & `shikithon-2.4.2/shikithon/resources/animes.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.4.1/shikithon/resources/appears.py` & `shikithon-2.4.2/shikithon/resources/appears.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.4.1/shikithon/resources/bans.py` & `shikithon-2.4.2/shikithon/resources/bans.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.4.1/shikithon/resources/calendars.py` & `shikithon-2.4.2/shikithon/resources/calendars.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.4.1/shikithon/resources/characters.py` & `shikithon-2.4.2/shikithon/resources/characters.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.4.1/shikithon/resources/clubs.py` & `shikithon-2.4.2/shikithon/resources/clubs.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.4.1/shikithon/resources/comments.py` & `shikithon-2.4.2/shikithon/resources/comments.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.4.1/shikithon/resources/constants.py` & `shikithon-2.4.2/shikithon/resources/constants.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.4.1/shikithon/resources/dialogs.py` & `shikithon-2.4.2/shikithon/resources/dialogs.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.4.1/shikithon/resources/favorites.py` & `shikithon-2.4.2/shikithon/resources/favorites.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.4.1/shikithon/resources/forums.py` & `shikithon-2.4.2/shikithon/resources/forums.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.4.1/shikithon/resources/friends.py` & `shikithon-2.4.2/shikithon/resources/friends.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.4.1/shikithon/resources/genres.py` & `shikithon-2.4.2/shikithon/resources/genres.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.4.1/shikithon/resources/mangas.py` & `shikithon-2.4.2/shikithon/resources/mangas.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.4.1/shikithon/resources/messages.py` & `shikithon-2.4.2/shikithon/resources/messages.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.4.1/shikithon/resources/people.py` & `shikithon-2.4.2/shikithon/resources/people.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.4.1/shikithon/resources/publishers.py` & `shikithon-2.4.2/shikithon/resources/publishers.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.4.1/shikithon/resources/ranobes.py` & `shikithon-2.4.2/shikithon/resources/ranobes.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.4.1/shikithon/resources/stats.py` & `shikithon-2.4.2/shikithon/resources/stats.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.4.1/shikithon/resources/studios.py` & `shikithon-2.4.2/shikithon/resources/studios.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.4.1/shikithon/resources/styles.py` & `shikithon-2.4.2/shikithon/resources/styles.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.4.1/shikithon/resources/topics.py` & `shikithon-2.4.2/shikithon/resources/topics.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.4.1/shikithon/resources/user_images.py` & `shikithon-2.4.2/shikithon/resources/user_images.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.4.1/shikithon/resources/user_rates.py` & `shikithon-2.4.2/shikithon/resources/user_rates.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.4.1/shikithon/resources/users.py` & `shikithon-2.4.2/shikithon/resources/users.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.4.1/shikithon/store/base.py` & `shikithon-2.4.2/shikithon/store/base.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.4.1/shikithon/store/json.py` & `shikithon-2.4.2/shikithon/store/json.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.4.1/shikithon/store/memory.py` & `shikithon-2.4.2/shikithon/store/memory.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.4.1/shikithon/store/null.py` & `shikithon-2.4.2/shikithon/store/null.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.4.1/shikithon/utils/utils.py` & `shikithon-2.4.2/shikithon/utils/utils.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.4.1/PKG-INFO` & `shikithon-2.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shikithon
-Version: 2.4.1
+Version: 2.4.2
 Summary: Yet another Python wrapper for Shikimori API
 Home-page: https://github.com/SecondThundeR/shikithon
 License: MIT
 Keywords: Python,Shikimori,API
 Author: SecondThundeR
 Author-email: awayfromgalaxy@gmail.com
 Requires-Python: >=3.8.10,<4.0.0
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Requires-Dist: backoff (>=2.2.1,<3.0.0)
-Requires-Dist: loguru (>=0.6.0,<0.7.0)
+Requires-Dist: loguru (>=0.7.0,<0.8.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: pyrate-limiter (>=2.10.0,<3.0.0)
 Requires-Dist: typing-extensions (>=4.5.0,<5.0.0)
 Requires-Dist: validators (>=0.20.0,<0.21.0)
 Project-URL: Documentation, https://github.com/SecondThundeR/shikithon/README.md
 Project-URL: Repository, https://github.com/SecondThundeR/shikithon
 Description-Content-Type: text/markdown
@@ -136,14 +136,15 @@
     async with api_auth_maker:
         ...
 
 asyncio.run(main())
 ```
 
 Выполнение нескольких запросов одновременно с помощью метода `multiple_requests`:
+
 ```py
 # В этом примере используется распаковка, но можно также получать весь массив с данными ответов
 # в одной переменнной (chainsaw, lycoris_anime, ... -> data = await ...)
 from shikithon import ShikimoriAPI, JSONStore
 
 config = ...
 
@@ -164,28 +165,28 @@
 # [Character(id=204621, name='Chisato Nishikigi', russian='Тисато Нисикиги', ...]
 # [Ranobe(id=151431, name='Lycoris Recoil: Ordinary Days', russian='Ликорис Рикоил: Повседневность', ...]
 ```
 
 Также, если хочется узнать как использовать встроенные хранилища конфигов или хочется создать свой,
 посмотрите [этот гайд](https://github.com/SecondThundeR/shikithon/wiki/%D0%93%D0%B0%D0%B9%D0%B4-%D0%BF%D0%BE-%D1%85%D1%80%D0%B0%D0%BD%D0%B8%D0%BB%D0%B8%D1%89%D0%B0%D0%BC-%D0%BA%D0%BE%D0%BD%D1%84%D0%B8%D0%B3%D1%83%D1%80%D0%B0%D1%86%D0%B8%D0%B8)
 
-#### Пара уточнений по использованию:
+### Пара уточнений по использованию
 
 - Возможно вам придется импортировать модели для ручной аннотации возвращаемых моделей в PyCharm
 _(в нем немного некорретно работает наследование типа от функции)_
 - При отсутствии каких-либо полей в данных конфигурации, библиотека выдает исключение
 - Если вы хотите использовать логгирование библиотеки, передайте флаг `logging=True` в объект API:
 `api = ShikimoriAPI(app_name="...", logging=True)`
 
-### Получение данных для конфигурации
+## Получение данных для конфигурации
 
-Для начала вам необходимо создать новое OAuth-приложение [здесь](https://shikimori.one/oauth/applications).
+Для начала вам необходимо создать новое OAuth-приложение [здесь](https://shikimori.me/oauth/applications).
 После этого, сохраните `app_name`, `client_id`, `client_secret`, а так же `redirect_uri`, если вы его меняли
 
-Позже, [на данной странице](https://shikimori.one/oauth) выберите свое приложение, необходимые разрешения
+Позже, [на данной странице](https://shikimori.me/oauth) выберите свое приложение, необходимые разрешения
 и получите код авторизации и сохраните его.
 _(Если необходимо, то можно также получить токены авторизации, пройдя следующий этап после получения кода авторизации)_
 
 ## Список изменений
 
 Все изменения перечислены на [странице релизов](https://github.com/SecondThundeR/shikithon/releases)
 
@@ -210,15 +211,16 @@
 - [loguru](https://github.com/Delgan/loguru) для удобного логгирования
 [(Лицензия)](https://github.com/Delgan/loguru/blob/master/LICENSE)
 - [validators](https://github.com/kvesteri/validators) для проверки строк на наличие ссылки в ней
 [(Лицензия)](https://github.com/kvesteri/validators/blob/master/LICENSE)
 - [typing-extensions](https://github.com/python/typing_extensions) для корректной типизации декораторов
 [(Лицензия)](https://github.com/python/typing_extensions/blob/main/LICENSE)
 
-В качестве зависимости для разработки, проект использует две зависимости:
+Также, данный проект использует две библиотеки в качестве зависимостей для разработки:
+
 - [pre-commit](https://github.com/pre-commit/pre-commit) для автоматизации форматирования и проверки кода
 [(Лицензия)](https://github.com/pre-commit/pre-commit/blob/main/LICENSE)
 - [mypy](https://github.com/python/mypy) для проверки типов [(Лицензия)](https://github.com/python/mypy/blob/master/LICENSE)
 
 ## Лицензия проекта
 
 Данный проект имеет MIT лицензию.
```

