# Comparing `tmp/sneakpeek_py-0.1.1.tar.gz` & `tmp/sneakpeek_py-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sneakpeek_py-0.1.1.tar", max compression
+gzip compressed data, was "sneakpeek_py-0.1.2.tar", max compression
```

## Comparing `sneakpeek_py-0.1.1.tar` & `sneakpeek_py-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,25 @@
--rw-r--r--   0        0        0       85 2023-04-02 10:58:33.945002 sneakpeek_py-0.1.1/README.md
--rw-r--r--   0        0        0     1675 2023-04-10 15:19:46.404709 sneakpeek_py-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2469 2023-04-10 12:15:19.719088 sneakpeek_py-0.1.1/sneakpeek/api.py
--rw-r--r--   0        0        0      283 2023-04-10 12:48:43.794471 sneakpeek_py-0.1.1/sneakpeek/config.py
--rw-r--r--   0        0        0     3926 2023-04-10 13:01:36.235348 sneakpeek_py-0.1.1/sneakpeek/context.py
--rw-r--r--   0        0        0      726 2023-04-10 11:41:30.863384 sneakpeek_py-0.1.1/sneakpeek/lib/errors.py
--rw-r--r--   0        0        0     1317 2023-04-10 14:50:53.763609 sneakpeek_py-0.1.1/sneakpeek/lib/models.py
--rw-r--r--   0        0        0     3821 2023-04-10 11:28:44.055807 sneakpeek_py-0.1.1/sneakpeek/lib/queue.py
--rw-r--r--   0        0        0     2005 2023-04-10 11:29:01.052309 sneakpeek_py-0.1.1/sneakpeek/lib/storage/base.py
--rw-r--r--   0        0        0     7544 2023-04-10 13:19:00.753044 sneakpeek_py-0.1.1/sneakpeek/lib/storage/in_memory_storage.py
--rw-r--r--   0        0        0     7015 2023-04-10 11:29:46.671675 sneakpeek_py-0.1.1/sneakpeek/lib/storage/redis_storage.py
--rw-r--r--   0        0        0     2349 2023-04-10 15:13:41.871987 sneakpeek_py-0.1.1/sneakpeek/runner.py
--rw-r--r--   0        0        0     6233 2023-04-10 14:52:04.073105 sneakpeek_py-0.1.1/sneakpeek/scheduler.py
--rw-r--r--   0        0        0      262 2023-04-10 12:49:48.973818 sneakpeek_py-0.1.1/sneakpeek/scraper.py
--rw-r--r--   0        0        0     2614 2023-04-10 15:01:10.667971 sneakpeek_py-0.1.1/sneakpeek/server.py
--rw-r--r--   0        0        0     2695 2023-04-10 13:08:17.784798 sneakpeek_py-0.1.1/sneakpeek/worker.py
--rw-r--r--   0        0        0     1663 1970-01-01 00:00:00.000000 sneakpeek_py-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       85 2023-04-02 10:58:33.945002 sneakpeek_py-0.1.2/README.md
+-rw-r--r--   0        0        0     1753 2023-04-15 14:29:59.612255 sneakpeek_py-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2464 2023-04-14 20:55:18.205455 sneakpeek_py-0.1.2/sneakpeek/api.py
+-rw-r--r--   0        0        0      726 2023-04-10 11:41:30.863384 sneakpeek_py-0.1.2/sneakpeek/lib/errors.py
+-rw-r--r--   0        0        0     1325 2023-04-14 20:40:35.860617 sneakpeek_py-0.1.2/sneakpeek/lib/models.py
+-rw-r--r--   0        0        0     4637 2023-04-15 13:21:03.582741 sneakpeek_py-0.1.2/sneakpeek/lib/queue.py
+-rw-r--r--   0        0        0     2066 2023-04-15 13:19:12.546715 sneakpeek_py-0.1.2/sneakpeek/lib/storage/base.py
+-rw-r--r--   0        0        0     9112 2023-04-15 13:20:08.681048 sneakpeek_py-0.1.2/sneakpeek/lib/storage/in_memory_storage.py
+-rw-r--r--   0        0        0     8889 2023-04-15 13:20:22.015469 sneakpeek_py-0.1.2/sneakpeek/lib/storage/redis_storage.py
+-rw-r--r--   0        0        0     1535 2023-04-15 08:35:07.840371 sneakpeek_py-0.1.2/sneakpeek/logging.py
+-rw-r--r--   0        0        0     3291 2023-04-15 13:15:52.422916 sneakpeek_py-0.1.2/sneakpeek/metrics.py
+-rw-r--r--   0        0        0     1338 2023-04-15 14:28:45.826848 sneakpeek_py-0.1.2/sneakpeek/plugins/proxy_plugin.py
+-rw-r--r--   0        0        0     4209 2023-04-15 10:43:26.332501 sneakpeek_py-0.1.2/sneakpeek/plugins/rate_limiter_plugin.py
+-rw-r--r--   0        0        0     2062 2023-04-15 10:43:18.016302 sneakpeek_py-0.1.2/sneakpeek/plugins/requests_logging_plugin.py
+-rw-r--r--   0        0        0     3747 2023-04-15 10:43:12.817939 sneakpeek_py-0.1.2/sneakpeek/plugins/robots_txt_plugin.py
+-rw-r--r--   0        0        0     1391 2023-04-15 14:24:15.543165 sneakpeek_py-0.1.2/sneakpeek/plugins/user_agent_injecter_plugin.py
+-rw-r--r--   0        0        0      659 2023-04-15 07:08:31.686879 sneakpeek_py-0.1.2/sneakpeek/plugins/utils.py
+-rw-r--r--   0        0        0     2910 2023-04-15 12:42:25.391509 sneakpeek_py-0.1.2/sneakpeek/runner.py
+-rw-r--r--   0        0        0    10268 2023-04-15 13:39:19.486115 sneakpeek_py-0.1.2/sneakpeek/scheduler.py
+-rw-r--r--   0        0        0      172 2023-04-14 20:22:32.213615 sneakpeek_py-0.1.2/sneakpeek/scraper_config.py
+-rw-r--r--   0        0        0     5810 2023-04-15 10:36:17.814799 sneakpeek_py-0.1.2/sneakpeek/scraper_context.py
+-rw-r--r--   0        0        0      282 2023-04-14 20:58:00.201559 sneakpeek_py-0.1.2/sneakpeek/scraper_handler.py
+-rw-r--r--   0        0        0     3654 2023-04-15 14:02:33.345443 sneakpeek_py-0.1.2/sneakpeek/server.py
+-rw-r--r--   0        0        0     3309 2023-04-15 13:39:24.072034 sneakpeek_py-0.1.2/sneakpeek/worker.py
+-rw-r--r--   0        0        0     1805 1970-01-01 00:00:00.000000 sneakpeek_py-0.1.2/PKG-INFO
```

### Comparing `sneakpeek_py-0.1.1/pyproject.toml` & `sneakpeek_py-0.1.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "sneakpeek-py"
 packages = [{ include = "sneakpeek" }]
-version = "0.1.1"
+version = "0.1.2"
 description = "Tool box for creating scrapers, so that you only focus on scraping logic"
 authors = ["Dan Yazovsky <daniil.yazovsky@gmail.com>"]
 maintainers = ["Dan Yazovsky <daniil.yazovsky@gmail.com>"]
 repository = "https://github.com/flulemon/sneakpeek"
 documentation = "https://github.com/flulemon/sneakpeek"
 homepage = "https://github.com/flulemon/sneakpeek"
 license = "BSD-3-Clause"
@@ -30,14 +30,17 @@
 pydantic = "^1.10.7"
 fastapi = "^0.95.0"
 fastapi-jsonrpc = "^2.4.1"
 redis = "^4.5.4"
 apscheduler = "^3.10.1"
 aiohttp = "^3.8.4"
 uvicorn = "^0.21.1"
+cachetools = "^5.3.0"
+prometheus-client = "^0.16.0"
+fake-useragent = "^1.1.3"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.2"
 fakeredis = "^2.10.3"
 black = "^23.3.0"
 pytest-lazy-fixture = "^0.6.3"
 pytest-asyncio = "^0.21.0"
```

### Comparing `sneakpeek_py-0.1.1/sneakpeek/api.py` & `sneakpeek_py-0.1.2/sneakpeek/api.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,34 @@
-from typing import List
-
 import fastapi_jsonrpc as jsonrpc
 from fastapi import Body
 
 from sneakpeek.lib.errors import ScraperHasActiveRunError, ScraperNotFoundError
 from sneakpeek.lib.models import Scraper, ScraperRun, ScraperRunPriority
 from sneakpeek.lib.queue import Queue, QueueABC
 from sneakpeek.lib.storage.base import Storage
-from sneakpeek.scraper import ScraperABC
+from sneakpeek.scraper_handler import ScraperHandler
 
 
 def get_public_api_entrypoint(
     storage: Storage,
     queue: Queue,
-    handlers: List[ScraperABC],
+    handlers: list[ScraperHandler],
 ) -> jsonrpc.Entrypoint:
     entrypoint = jsonrpc.Entrypoint("/api/v1/jsonrpc")
 
     @entrypoint.method()
     async def search_scrapers(
         name_filter: str | None = Body(...),
         max_items: int | None = Body(...),
         last_id: int | None = Body(...),
-    ) -> List[Scraper]:
+    ) -> list[Scraper]:
         return await storage.search_scrapers(name_filter, max_items, last_id)
 
     @entrypoint.method()
-    async def get_scrapers() -> List[Scraper]:
+    async def get_scrapers() -> list[Scraper]:
         return await storage.get_scrapers()
 
     @entrypoint.method(errors=[ScraperNotFoundError])
     async def get_scraper(id: int = Body(...)) -> Scraper:
         return await storage.get_scraper(id)
 
     @entrypoint.method()
@@ -49,25 +47,25 @@
         return await storage.update_scraper(scraper)
 
     @entrypoint.method(errors=[ScraperNotFoundError])
     async def delete_scraper(id: int = Body(...)) -> Scraper:
         return await storage.delete_scraper(id)
 
     @entrypoint.method(errors=[ScraperNotFoundError])
-    async def get_scraper_runs(scraper_id: int = Body(...)) -> List[ScraperRun]:
+    async def get_scraper_runs(scraper_id: int = Body(...)) -> list[ScraperRun]:
         return await storage.get_scraper_runs(scraper_id)
 
     @entrypoint.method()
-    async def get_scraper_handlers() -> List[str]:
+    async def get_scraper_handlers() -> list[str]:
         return [handler.name for handler in handlers]
 
     return entrypoint
 
 
 def create_api(
     storage: Storage,
     queue: QueueABC,
-    handlers: List[ScraperABC],
+    handlers: list[ScraperHandler],
 ) -> jsonrpc.API:
     app = jsonrpc.API()
     app.bind_entrypoint(get_public_api_entrypoint(storage, queue, handlers))
     return app
```

### Comparing `sneakpeek_py-0.1.1/sneakpeek/lib/errors.py` & `sneakpeek_py-0.1.2/sneakpeek/lib/errors.py`

 * *Files identical despite different names*

### Comparing `sneakpeek_py-0.1.1/sneakpeek/lib/models.py` & `sneakpeek_py-0.1.2/sneakpeek/lib/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from datetime import datetime
 from enum import Enum
 
 from pydantic import BaseModel
 
-from sneakpeek.config import ScraperConfig
+from sneakpeek.scraper_config import ScraperConfig
 
 UNSET_ID: int = -1
 
 
 class ScraperSchedule(str, Enum):
     INACTIVE = "inactive"
     EVERY_SECOND = "every_second"
```

### Comparing `sneakpeek_py-0.1.1/sneakpeek/lib/queue.py` & `sneakpeek_py-0.1.2/sneakpeek/lib/queue.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import logging
-from abc import ABC
+from abc import ABC, abstractmethod
 from datetime import datetime, timedelta
 from typing import List
 
 from sneakpeek.lib.errors import (
     ScraperHasActiveRunError,
     ScraperRunPingFinishedError,
     ScraperRunPingNotStartedError,
@@ -11,45 +11,59 @@
 from sneakpeek.lib.models import (
     UNSET_ID,
     ScraperRun,
     ScraperRunPriority,
     ScraperRunStatus,
 )
 from sneakpeek.lib.storage.base import Storage
+from sneakpeek.metrics import count_invocations, measure_latency
 
 DEFAULT_DEAD_TIMEOUT = timedelta(minutes=5)
 
 
 class QueueABC(ABC):
+    @abstractmethod
     async def enqueue(
         self,
         scraper_id: int,
         priority: ScraperRunPriority,
     ) -> ScraperRun:
-        raise NotImplementedError()
+        ...
 
+    @abstractmethod
     async def dequeue(self) -> ScraperRun:
-        raise NotImplementedError()
+        ...
 
+    @abstractmethod
+    async def get_queue_len(self, priority: ScraperRunPriority) -> int:
+        ...
+
+    @abstractmethod
     async def ping_scraper_run(
         self,
         scraper_id: int,
         scraper_run_id: int,
     ) -> ScraperRun:
-        raise NotImplementedError()
+        ...
+
+    @abstractmethod
+    async def kill_dead_scraper_runs(self, scraper_id: int):
+        ...
 
 
 class Queue:
     def __init__(
         self, storage: Storage, dead_timeout: timedelta = DEFAULT_DEAD_TIMEOUT
     ) -> None:
         self._storage = storage
         self._logger = logging.getLogger(__name__)
         self._dead_timeout = dead_timeout
 
+    @count_invocations(subsystem="queue")
+    @measure_latency(subsystem="queue")
     async def enqueue(
         self,
         scraper_id: int,
         priority: ScraperRunPriority,
     ) -> ScraperRun:
         scraper = await self._storage.get_scraper(scraper_id)
         if await self._has_unfinished_runs(scraper_id):
@@ -60,41 +74,52 @@
                 scraper=scraper,
                 status=ScraperRunStatus.PENDING,
                 priority=priority,
                 created_at=datetime.utcnow(),
             )
         )
 
+    @count_invocations(subsystem="queue")
+    @measure_latency(subsystem="queue")
     async def dequeue(self) -> ScraperRun | None:
         for priority in ScraperRunPriority:
             dequeued = await self._storage.dequeue_scraper_run(priority)
             if dequeued:
                 dequeued.started_at = datetime.utcnow()
                 dequeued.status = ScraperRunStatus.STARTED
                 return await self._storage.update_scraper_run(dequeued)
         return None
 
+    @count_invocations(subsystem="queue")
+    @measure_latency(subsystem="queue")
+    async def get_queue_len(self, priority: ScraperRunPriority) -> int:
+        return await self._storage.get_queue_len(priority)
+
+    @count_invocations(subsystem="queue")
+    @measure_latency(subsystem="queue")
     async def ping_scraper_run(
         self,
         scraper_id: int,
         scraper_run_id: int,
     ) -> ScraperRun:
         scraper_run = await self._storage.get_scraper_run(scraper_id, scraper_run_id)
         if scraper_run.status == ScraperRunStatus.PENDING:
             raise ScraperRunPingNotStartedError()
         if scraper_run.status != ScraperRunStatus.STARTED:
             raise ScraperRunPingFinishedError()
         scraper_run.last_active_at = datetime.utcnow()
         return await self._storage.update_scraper_run(scraper_run)
 
+    @count_invocations(subsystem="queue")
+    @measure_latency(subsystem="queue")
     async def kill_dead_scraper_runs(self, scraper_id: int) -> List[ScraperRun]:
         runs = await self._storage.get_scraper_runs(scraper_id)
         killed = []
         for run in runs:
-            if self._is_scraper_run_dead(run):
+            if await self._is_scraper_run_dead(run):
                 run.status = ScraperRunStatus.DEAD
                 run.finished_at = datetime.utcnow()
                 killed.append(await self._storage.update_scraper_run(run))
         return killed
 
     async def _is_scraper_run_dead(self, scraper_run: ScraperRun) -> bool:
         if scraper_run.status != ScraperRunStatus.STARTED:
```

### Comparing `sneakpeek_py-0.1.1/sneakpeek/lib/storage/in_memory_storage.py` & `sneakpeek_py-0.1.2/sneakpeek/lib/storage/in_memory_storage.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,35 +2,38 @@
 from asyncio import Lock
 from datetime import datetime, timedelta
 from itertools import count
 from typing import Iterator
 
 from sneakpeek.lib.errors import ScraperNotFoundError, ScraperRunNotFoundError
 from sneakpeek.lib.models import Lease, Scraper, ScraperRun, ScraperRunPriority
+from sneakpeek.metrics import count_invocations, measure_latency
 
 from .base import Storage
 
 
 class InMemoryStorage(Storage):
     def __init__(self, scrapers: list[Scraper] | None = None) -> None:
         self._logger = logging.getLogger(__name__)
         self._scrapers: dict[int, Scraper] = {
             scraper.id: scraper for scraper in scrapers or []
         }
         self._scraper_runs: dict[int, dict[int, ScraperRun]] = {}
         self._queues: dict[ScraperRunPriority, list[ScraperRun]] = {}
-        self._id_generator: Iterator[int] = count()
+        self._id_generator: Iterator[int] = count(1)
         self._lock = Lock()
         self._leases: dict[str, Lease] = {}
 
     def _generate_id(self) -> int:
         for id in self._id_generator:
             if id not in self._scrapers and id not in self._scraper_runs:
                 return id
 
+    @count_invocations(subsystem="storage")
+    @measure_latency(subsystem="storage")
     async def search_scrapers(
         self,
         name_filter: str | None = None,
         max_items: int | None = None,
         offset: int | None = None,
     ) -> list[Scraper]:
         offset = offset or 0
@@ -42,58 +45,74 @@
                 if name_filter in item.name and item.id > offset
             ],
             key=lambda item: item.id,
         )
         max_items = max_items if max_items and max_items > 0 else len(items)
         return items[:max_items]
 
+    @count_invocations(subsystem="storage")
+    @measure_latency(subsystem="storage")
     async def get_scrapers(self) -> list[Scraper]:
         return list(self._scrapers.values())
 
+    @count_invocations(subsystem="storage")
+    @measure_latency(subsystem="storage")
     async def get_scraper(self, id: int) -> Scraper:
         if id not in self._scrapers:
             raise ScraperNotFoundError(id)
         return self._scrapers[id]
 
+    @count_invocations(subsystem="storage")
+    @measure_latency(subsystem="storage")
     async def maybe_get_scraper(self, id: int) -> Scraper | None:
         return self._scrapers.get(id)
 
+    @count_invocations(subsystem="storage")
+    @measure_latency(subsystem="storage")
     async def create_scraper(self, scraper: Scraper) -> Scraper:
         async with self._lock:
             scraper.id = (
                 scraper.id if scraper.id and scraper.id > 0 else self._generate_id()
             )
             if scraper.id and scraper.id in self._scrapers:
                 self._logger.warning(
                     f"Will rewrite existing scraper: {self._scrapers[scraper.id]} with {scraper}"
                 )
             self._scrapers[scraper.id] = scraper
             return scraper
 
+    @count_invocations(subsystem="storage")
+    @measure_latency(subsystem="storage")
     async def update_scraper(self, scraper: Scraper) -> Scraper:
         async with self._lock:
             if scraper.id not in self._scrapers:
                 raise ScraperNotFoundError(scraper.id)
             self._scrapers[scraper.id] = scraper
             return scraper
 
+    @count_invocations(subsystem="storage")
+    @measure_latency(subsystem="storage")
     async def delete_scraper(self, id: int) -> Scraper:
         async with self._lock:
             if id not in self._scrapers:
                 raise ScraperNotFoundError(id)
             scraper_to_delete = self._scrapers[id]
             del self._scrapers[id]
             return scraper_to_delete
 
+    @count_invocations(subsystem="storage")
+    @measure_latency(subsystem="storage")
     async def get_scraper_runs(self, id: int) -> list[ScraperRun]:
         async with self._lock:
             if id not in self._scrapers:
                 raise ScraperNotFoundError(id)
             return list(self._scraper_runs.get(id, {}).values())
 
+    @count_invocations(subsystem="storage")
+    @measure_latency(subsystem="storage")
     async def add_scraper_run(self, scraper_run: ScraperRun) -> ScraperRun:
         async with self._lock:
             scraper_run.id = (
                 scraper_run.id
                 if scraper_run.id and scraper_run.id > 0
                 else self._generate_id()
             )
@@ -110,47 +129,60 @@
 
             self._scraper_runs[scraper_run.scraper.id][scraper_run.id] = scraper_run
             if scraper_run.priority not in self._queues:
                 self._queues[scraper_run.priority] = []
             self._queues[scraper_run.priority].append(scraper_run)
             return scraper_run
 
+    @count_invocations(subsystem="storage")
+    @measure_latency(subsystem="storage")
     async def update_scraper_run(self, scraper_run: ScraperRun) -> ScraperRun:
         async with self._lock:
             if scraper_run.scraper.id not in self._scrapers:
                 raise ScraperNotFoundError(scraper_run.scraper.id)
             if (
                 not self._scraper_runs.get(scraper_run.scraper.id)
                 or scraper_run.id not in self._scraper_runs[scraper_run.scraper.id]
             ):
                 raise ScraperRunNotFoundError(scraper_run.id)
 
             self._scraper_runs[scraper_run.scraper.id][scraper_run.id] = scraper_run
             return scraper_run
 
+    @count_invocations(subsystem="storage")
+    @measure_latency(subsystem="storage")
     async def get_scraper_run(self, scraper_id: int, scraper_run_id: int) -> ScraperRun:
         async with self._lock:
             if scraper_id not in self._scrapers:
                 raise ScraperNotFoundError(scraper_id)
             if (
                 not self._scraper_runs.get(scraper_id)
                 or scraper_run_id not in self._scraper_runs[scraper_id]
             ):
                 raise ScraperRunNotFoundError(scraper_run_id)
             return self._scraper_runs[scraper_id][scraper_run_id]
 
+    @count_invocations(subsystem="storage")
+    @measure_latency(subsystem="storage")
     async def dequeue_scraper_run(
         self,
         priority: ScraperRunPriority,
     ) -> ScraperRun | None:
         async with self._lock:
             if not self._queues.get(priority):
                 return None
             return self._queues[priority].pop(0)
 
+    @count_invocations(subsystem="storage")
+    @measure_latency(subsystem="storage")
+    async def get_queue_len(self, priority: ScraperRunPriority) -> int:
+        return len(self._queues.get(priority) or [])
+
+    @count_invocations(subsystem="storage")
+    @measure_latency(subsystem="storage")
     async def delete_old_scraper_runs(self, keep_last: int = 50) -> None:
         async with self._lock:
             self._scraper_runs = {
                 scraper_id: {
                     scraper_run.id: scraper_run
                     for scraper_run in sorted(
                         scraper_runs.values(),
@@ -165,14 +197,16 @@
         existing_lease = self._leases.get(lease_name)
         return (
             not existing_lease
             or existing_lease.acquired_until < datetime.utcnow()
             or existing_lease.owner_id == owner_id
         )
 
+    @count_invocations(subsystem="storage")
+    @measure_latency(subsystem="storage")
     async def maybe_acquire_lease(
         self,
         lease_name: str,
         owner_id: str,
         acquire_for: timedelta,
     ) -> Lease | None:
         async with self._lock:
@@ -182,13 +216,15 @@
                     owner_id=owner_id,
                     acquired=datetime.utcnow(),
                     acquired_until=datetime.utcnow() + acquire_for,
                 )
                 return self._leases[lease_name]
         return None
 
+    @count_invocations(subsystem="storage")
+    @measure_latency(subsystem="storage")
     async def release_lease(self, lease_name: str, owner_id: str) -> None:
         async with self._lock:
             if lease_name not in self._leases:
                 return
             if self._can_acquire_lease(lease_name, owner_id):
                 del self._leases[lease_name]
```

### Comparing `sneakpeek_py-0.1.1/sneakpeek/lib/storage/redis_storage.py` & `sneakpeek_py-0.1.2/sneakpeek/lib/storage/redis_storage.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,15 @@
 from datetime import datetime, timedelta
 from typing import List
 
 from redis.asyncio import Redis
 
 from sneakpeek.lib.errors import ScraperNotFoundError, ScraperRunNotFoundError
-from sneakpeek.lib.models import (
-    Lease,
-    Scraper,
-    ScraperRun,
-    ScraperRunPriority,
-    ScraperRunStatus,
-)
+from sneakpeek.lib.models import Lease, Scraper, ScraperRun, ScraperRunPriority
+from sneakpeek.metrics import count_invocations, measure_latency
 
 from .base import Storage
 
 
 class RedisStorage(Storage):
     def __init__(self, redis: Redis) -> None:
         self._redis = redis
@@ -33,72 +28,92 @@
 
     def _get_scraper_key(self, id: int) -> str:
         return f"scraper:{id}"
 
     def _get_scraper_run_key(self, scraper_id: int, run_id: int) -> str:
         return f"scraper_run:{scraper_id}:{run_id}"
 
+    @count_invocations(subsystem="storage")
+    @measure_latency(subsystem="storage")
     async def search_scrapers(
         self,
         name_filter: str | None = None,
         max_items: int | None = None,
         offset: int | None = None,
     ) -> List[Scraper]:
         start = offset or 0
         end = start + (max_items or 10)
         return [
             scraper
             for scraper in await self.get_scrapers()
             if name_filter in scraper.name
         ][start:end]
 
+    @count_invocations(subsystem="storage")
+    @measure_latency(subsystem="storage")
     async def get_scrapers(self) -> List[Scraper]:
         keys = [key.decode() async for key in self._redis.scan_iter("scraper:*")]
         return sorted(
             (Scraper.parse_raw(scraper) for scraper in await self._redis.mget(keys)),
             key=lambda x: x.id,
         )
 
+    @count_invocations(subsystem="storage")
+    @measure_latency(subsystem="storage")
     async def get_scraper(self, id: int) -> Scraper:
         scraper = await self.maybe_get_scraper(id)
         if not scraper:
             raise ScraperNotFoundError()
         return scraper
 
+    @count_invocations(subsystem="storage")
+    @measure_latency(subsystem="storage")
     async def maybe_get_scraper(self, id: int) -> Scraper | None:
         scraper = await self._redis.get(f"scraper:{id}")
         return Scraper.parse_raw(scraper) if scraper else None
 
+    @count_invocations(subsystem="storage")
+    @measure_latency(subsystem="storage")
     async def create_scraper(self, scraper: Scraper) -> Scraper:
-        scraper.id = await self._generate_id()
+        scraper.id = (
+            scraper.id if scraper.id and scraper.id > 0 else await self._generate_id()
+        )
         await self._redis.set(self._get_scraper_key(scraper.id), scraper.json())
         return scraper
 
+    @count_invocations(subsystem="storage")
+    @measure_latency(subsystem="storage")
     async def update_scraper(self, scraper: Scraper) -> Scraper:
         if not await self._redis.exists(self._get_scraper_key(scraper.id)):
             raise ScraperNotFoundError()
         await self._redis.set(self._get_scraper_key(scraper.id), scraper.json())
         return scraper
 
+    @count_invocations(subsystem="storage")
+    @measure_latency(subsystem="storage")
     async def delete_scraper(self, id: int) -> Scraper:
         scraper = await self._redis.getdel(self._get_scraper_key(id))
         if not scraper:
             raise ScraperNotFoundError()
         return Scraper.parse_raw(scraper)
 
+    @count_invocations(subsystem="storage")
+    @measure_latency(subsystem="storage")
     async def get_scraper_runs(self, scraper_id: int) -> List[ScraperRun]:
         keys = [
             key.decode()
             async for key in self._redis.scan_iter(f"scraper_run:{scraper_id}:*")
         ]
         return sorted(
             [ScraperRun.parse_raw(run) for run in await self._redis.mget(keys)],
             key=lambda x: x.id,
         )
 
+    @count_invocations(subsystem="storage")
+    @measure_latency(subsystem="storage")
     async def add_scraper_run(self, scraper_run: ScraperRun) -> ScraperRun:
         if not await self._redis.exists(f"scraper:{scraper_run.scraper.id}"):
             raise ScraperNotFoundError()
         scraper_run.id = (
             scraper_run.id
             if scraper_run.id and scraper_run.id > 0
             else await self._generate_id()
@@ -114,58 +129,78 @@
             f"queue:{scraper_run.priority}:{job_id}",
             scraper_run.json(),
         )
         await pipeline.execute()
 
         return scraper_run
 
+    @count_invocations(subsystem="storage")
+    @measure_latency(subsystem="storage")
     async def update_scraper_run(self, scraper_run: ScraperRun) -> ScraperRun:
         if not await self._redis.exists(self._get_scraper_key(scraper_run.scraper.id)):
             raise ScraperNotFoundError()
         if not await self._redis.exists(
             self._get_scraper_run_key(scraper_run.scraper.id, scraper_run.id)
         ):
             raise ScraperRunNotFoundError()
         await self._redis.set(
             self._get_scraper_run_key(scraper_run.scraper.id, scraper_run.id),
             scraper_run.json(),
         )
         return scraper_run
 
+    @count_invocations(subsystem="storage")
+    @measure_latency(subsystem="storage")
     async def dequeue_scraper_run(
         self, priority: ScraperRunPriority
     ) -> ScraperRun | None:
         offset = await self._get_queue_offset(priority)
         last_id = await self._get_queue_last_id(priority)
         if offset < last_id:
             pipeline = self._redis.pipeline()
             pipeline.getdel(f"queue:{priority}:{offset+1}")
             pipeline.incr(f"internal:queue:{priority}:offset")
             run, _ = await pipeline.execute()
             return ScraperRun.parse_raw(run)
         return None
 
+    @count_invocations(subsystem="storage")
+    @measure_latency(subsystem="storage")
+    async def get_queue_len(self, priority: ScraperRunPriority) -> int:
+        offset = await self._get_queue_offset(priority)
+        last_id = await self._get_queue_last_id(priority)
+        return last_id - offset
+
+    @count_invocations(subsystem="storage")
+    @measure_latency(subsystem="storage")
     async def delete_old_scraper_runs(self, keep_last: int = 50) -> None:
         to_delete = []
         for scraper in await self.get_scrapers():
             runs = await self.get_scraper_runs(scraper.id)
             if len(runs) > keep_last:
                 to_delete += [
                     self._get_scraper_run_key(scraper.id, run.id)
                     for run in runs[:-keep_last]
                 ]
         await self._redis.delete(*to_delete)
 
-    async def has_unfinished_scraper_runs(self, scraper_id: int) -> bool:
-        return any(
-            run
-            for run in await self.get_scraper_runs(scraper_id)
-            if run.status in (ScraperRunStatus.PENDING, ScraperRunStatus.STARTED)
+    @count_invocations(subsystem="storage")
+    @measure_latency(subsystem="storage")
+    async def get_scraper_run(self, scraper_id: int, scraper_run_id: int) -> ScraperRun:
+        if not await self._redis.exists(self._get_scraper_key(scraper_id)):
+            raise ScraperNotFoundError()
+        scraper_run = await self._redis.get(
+            self._get_scraper_run_key(scraper_id, scraper_run_id),
         )
+        if not scraper_run:
+            raise ScraperRunNotFoundError()
+        return ScraperRun.parse_raw(scraper_run)
 
+    @count_invocations(subsystem="storage")
+    @measure_latency(subsystem="storage")
     async def maybe_acquire_lease(
         self,
         lease_name: str,
         owner_id: str,
         acquire_for: timedelta,
     ) -> Lease | None:
         lease_key = f"lease:{lease_name}"
@@ -184,11 +219,13 @@
                 acquired=datetime.utcnow(),
                 acquired_until=datetime.utcnow() + acquire_for,
             )
             if result
             else None
         )
 
+    @count_invocations(subsystem="storage")
+    @measure_latency(subsystem="storage")
     async def release_lease(self, lease_name: str, owner_id: str) -> None:
         lease_owner = await self._redis.get(f"lease:{lease_name}")
         if lease_owner == owner_id:
             await self._redis.delete(f"lease:{lease_name}")
```

### Comparing `sneakpeek_py-0.1.1/sneakpeek/runner.py` & `sneakpeek_py-0.1.2/sneakpeek/runner.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,65 +1,78 @@
 import logging
-from abc import ABC
+from abc import ABC, abstractmethod
 from datetime import datetime
 from traceback import format_exc
 from typing import List
 
-from sneakpeek.context import ScraperContext
+from prometheus_client import Counter
+
 from sneakpeek.lib.errors import UnknownScraperHandlerError
 from sneakpeek.lib.models import Scraper, ScraperRun, ScraperRunStatus
 from sneakpeek.lib.queue import QueueABC
 from sneakpeek.lib.storage.base import Storage
-from sneakpeek.scraper import ScraperABC
+from sneakpeek.logging import scraper_run_context
+from sneakpeek.metrics import count_invocations, delay_histogram
+from sneakpeek.scraper_context import Plugin, ScraperContext
+from sneakpeek.scraper_handler import ScraperHandler
+
+scraper_runs = Counter(
+    name="scraper_runs",
+    documentation="Scraper runs executed",
+    namespace="sneakpeek",
+    labelnames=["type"],
+)
 
 
 class RunnerABC(ABC):
+    @abstractmethod
     async def run(self, run: ScraperRun) -> None:
-        raise NotImplementedError()
+        ...
 
 
 class Runner(RunnerABC):
     def __init__(
         self,
         handlers: List[Scraper],
         queue: QueueABC,
         storage: Storage,
+        plugins: list[Plugin] | None = None,
     ) -> None:
         self._logger = logging.getLogger(__name__)
         self._handlers = {handler.name: handler for handler in handlers}
         self._queue = queue
         self._storage = storage
+        self._plugins = plugins
 
-    def _get_handler(self, run: ScraperRun) -> ScraperABC:
+    def _get_handler(self, run: ScraperRun) -> ScraperHandler:
         if run.scraper.handler not in self._handlers:
             raise UnknownScraperHandlerError(
                 f"Unknown scraper handler '{run.scraper.handler}'"
             )
         return self._handlers[run.scraper.handler]
 
-    def _build_context(self, run: ScraperRun) -> ScraperContext:
-        return ScraperContext(
-            run.scraper.id,
-            run.id,
-            run.scraper.config,
-        )
-
+    @count_invocations(subsystem="scraper_runner")
     async def run(self, run: ScraperRun) -> None:
-        human_run_id = f"'{run.scraper.id}::{run.scraper.name}::{run.id}'"
-        self._logger.info(f"Running scraper {human_run_id}")
-        try:
-            await self._queue.ping_scraper_run(run.scraper.id, run.id)
-            run.scraper.config
-            handler = self._get_handler(run)
-            async with self._build_context(run) as context:
+        delay_histogram.labels(type="time_spent_in_queue").observe(
+            (datetime.utcnow() - run.created_at).total_seconds()
+        )
+        with scraper_run_context(run):
+            self._logger.info("Starting scraper")
+            context = ScraperContext(run.scraper.config, self._plugins)
+            try:
+                await context.start_session()
+                await self._queue.ping_scraper_run(run.scraper.id, run.id)
+                handler = self._get_handler(run)
                 run.result = await handler.run(context)
-            run.status = ScraperRunStatus.SUCCEEDED
-        except Exception as e:
-            self._logger.error(f"Failed to execute: {human_run_id}: {e}")
-            self._logger.debug(
-                f"Failed to execute: {human_run_id}. Traceback: {format_exc()}"
-            )
-            run.status = ScraperRunStatus.FAILED
-            run.result = str(e)
-        run.finished_at = datetime.utcnow()
-        await self._storage.update_scraper_run(run)
-        self._logger.info(f"Successfully executed {human_run_id}")
+                run.status = ScraperRunStatus.SUCCEEDED
+                scraper_runs.labels(type="success").inc()
+            except Exception as e:
+                self._logger.error(f"Failed to execute scraper with error: {e}")
+                self._logger.debug(f"Traceback: {format_exc()}")
+                run.status = ScraperRunStatus.FAILED
+                run.result = str(e)
+                scraper_runs.labels(type="failed").inc()
+            finally:
+                await context.close()
+            run.finished_at = datetime.utcnow()
+            await self._storage.update_scraper_run(run)
+            self._logger.info("Successfully executed scraper")
```

### Comparing `sneakpeek_py-0.1.1/sneakpeek/worker.py` & `sneakpeek_py-0.1.2/sneakpeek/worker.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 import logging
-from abc import ABC
+from abc import ABC, abstractmethod
 from asyncio import AbstractEventLoop, Lock, get_running_loop, sleep
 from datetime import timedelta
 from traceback import format_exc
 from typing import Dict
 
 from sneakpeek.lib.models import ScraperRun
 from sneakpeek.lib.queue import QueueABC
+from sneakpeek.metrics import count_invocations, measure_latency, replicas_gauge
 from sneakpeek.runner import RunnerABC
 
 
 class WorkerABC(ABC):
+    @abstractmethod
     async def start(self) -> None:
-        raise NotImplementedError()
+        ...
 
+    @abstractmethod
     async def stop(self) -> None:
-        raise NotImplementedError()
+        ...
 
 
 class Worker(WorkerABC):
     def __init__(
         self,
         runner: RunnerABC,
         queue: QueueABC,
@@ -31,25 +34,29 @@
         self._logger = logging.getLogger(__name__)
         self._lock = Lock()
         self._runner = runner
         self._queue = queue
         self._active: Dict[int, ScraperRun] = {}
         self._max_concurrency = max_concurrency
 
+    @count_invocations(subsystem="worker")
     async def _execute_scraper(self, scraper_run: ScraperRun) -> None:
         self._logger.info(f"Executing scraper run id={scraper_run.id}")
         try:
             await self._runner.run(scraper_run)
         except Exception as e:
             self._logger.error(f"Failed to execute {scraper_run.id}: {e}")
             self._logger.debug(f"Failed to execute {scraper_run.id}: {format_exc()}")
         del self._active[scraper_run.id]
 
+    @measure_latency(subsystem="worker")
+    @count_invocations(subsystem="worker")
     async def _on_tick(self) -> None:
         async with self._lock:
+            replicas_gauge.labels(type="active_scrapers").set(len(self._active))
             if len(self._active) >= self._max_concurrency:
                 self._logger.debug(
                     f"Not dequeuing any tasks because worker has reached max concurrency,"
                     f" there are {len(self._active)} of active tasks"
                 )
                 return
 
@@ -60,20 +67,28 @@
 
             self._logger.info(f"Dequeued a job with id={dequeued.id}")
             self._active[dequeued.id] = dequeued
             self._loop.create_task(self._execute_scraper(dequeued))
 
     async def _worker_loop(self) -> None:
         while self._running:
-            await self._on_tick()
+            replicas_gauge.labels(type="worker").set(1)
+            try:
+                await self._on_tick()
+            except Exception as e:
+                self._logger.error(f"Worker on tick function failed: {e}")
+                self._logger.debug(
+                    f"Worker on tick function failed. Traceback: {format_exc()}"
+                )
+
             await sleep(timedelta(seconds=1).total_seconds())
 
     async def start(self) -> None:
         self._logger.info("Starting worker")
         self._running = True
         if not self._loop:
             self._loop = get_running_loop()
         self._loop.create_task(self._worker_loop())
 
-    async def stop(self) -> None:
+    def stop(self) -> None:
         self._logger.info(f"Stopping worker. There are {len(self._active)} jobs")
         self._running = False
```

### Comparing `sneakpeek_py-0.1.1/PKG-INFO` & `sneakpeek_py-0.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sneakpeek-py
-Version: 0.1.1
+Version: 0.1.2
 Summary: Tool box for creating scrapers, so that you only focus on scraping logic
 Home-page: https://github.com/flulemon/sneakpeek
 License: BSD-3-Clause
 Author: Dan Yazovsky
 Author-email: daniil.yazovsky@gmail.com
 Maintainer: Dan Yazovsky
 Maintainer-email: daniil.yazovsky@gmail.com
@@ -22,16 +22,19 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Requires-Dist: apscheduler (>=3.10.1,<4.0.0)
+Requires-Dist: cachetools (>=5.3.0,<6.0.0)
+Requires-Dist: fake-useragent (>=1.1.3,<2.0.0)
 Requires-Dist: fastapi (>=0.95.0,<0.96.0)
 Requires-Dist: fastapi-jsonrpc (>=2.4.1,<3.0.0)
+Requires-Dist: prometheus-client (>=0.16.0,<0.17.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: redis (>=4.5.4,<5.0.0)
 Requires-Dist: uvicorn (>=0.21.1,<0.22.0)
 Project-URL: Documentation, https://github.com/flulemon/sneakpeek
 Project-URL: Repository, https://github.com/flulemon/sneakpeek
 Description-Content-Type: text/markdown
```

