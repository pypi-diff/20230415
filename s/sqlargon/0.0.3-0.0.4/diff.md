# Comparing `tmp/sqlargon-0.0.3.tar.gz` & `tmp/sqlargon-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlargon-0.0.3.tar", max compression
+gzip compressed data, was "sqlargon-0.0.4.tar", max compression
```

## Comparing `sqlargon-0.0.3.tar` & `sqlargon-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    11357 2023-04-06 09:54:04.659536 sqlargon-0.0.3/LICENSE
--rw-r--r--   0        0        0     3280 2023-04-06 09:54:04.659536 sqlargon-0.0.3/README.md
--rw-r--r--   0        0        0     1559 2023-04-06 09:54:04.659536 sqlargon-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      454 2023-04-06 09:54:04.659536 sqlargon-0.0.3/sqlargon/__init__.py
--rw-r--r--   0        0        0       22 2023-04-06 09:54:04.659536 sqlargon-0.0.3/sqlargon/_version.py
--rw-r--r--   0        0        0     3585 2023-04-06 09:54:04.659536 sqlargon-0.0.3/sqlargon/db.py
--rw-r--r--   0        0        0        0 2023-04-06 09:54:04.659536 sqlargon-0.0.3/sqlargon/dialects/__init__.py
--rw-r--r--   0        0        0      206 2023-04-06 09:54:04.659536 sqlargon-0.0.3/sqlargon/dialects/postgres.py
--rw-r--r--   0        0        0      243 2023-04-06 09:54:04.659536 sqlargon-0.0.3/sqlargon/dialects/sqlite.py
--rw-r--r--   0        0        0     6243 2023-04-06 09:54:04.659536 sqlargon-0.0.3/sqlargon/function_elements.py
--rw-r--r--   0        0        0        0 2023-04-06 09:54:04.659536 sqlargon-0.0.3/sqlargon/integrations/__init__.py
--rw-r--r--   0        0        0      824 2023-04-06 09:54:04.659536 sqlargon-0.0.3/sqlargon/integrations/fastapi.py
--rw-r--r--   0        0        0     1315 2023-04-06 09:54:04.659536 sqlargon-0.0.3/sqlargon/mixins.py
--rw-r--r--   0        0        0      913 2023-04-06 09:54:04.659536 sqlargon-0.0.3/sqlargon/orm.py
--rw-r--r--   0        0        0        0 2023-04-06 09:54:04.659536 sqlargon-0.0.3/sqlargon/py.typed
--rw-r--r--   0        0        0     7358 2023-04-06 09:54:04.659536 sqlargon-0.0.3/sqlargon/repository.py
--rw-r--r--   0        0        0      803 2023-04-06 09:54:04.659536 sqlargon-0.0.3/sqlargon/settings.py
--rw-r--r--   0        0        0     3033 2023-04-06 09:54:04.659536 sqlargon-0.0.3/sqlargon/types.py
--rw-r--r--   0        0        0      255 2023-04-06 09:54:04.659536 sqlargon-0.0.3/sqlargon/util.py
--rw-r--r--   0        0        0     3978 1970-01-01 00:00:00.000000 sqlargon-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-15 19:35:30.078581 sqlargon-0.0.4/LICENSE
+-rw-r--r--   0        0        0     3277 2023-04-15 19:35:30.078581 sqlargon-0.0.4/README.md
+-rw-r--r--   0        0        0     1559 2023-04-15 19:35:30.082581 sqlargon-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      454 2023-04-15 19:35:30.082581 sqlargon-0.0.4/sqlargon/__init__.py
+-rw-r--r--   0        0        0       22 2023-04-15 19:35:30.082581 sqlargon-0.0.4/sqlargon/_version.py
+-rw-r--r--   0        0        0     3404 2023-04-15 19:35:30.082581 sqlargon-0.0.4/sqlargon/db.py
+-rw-r--r--   0        0        0        0 2023-04-15 19:35:30.082581 sqlargon-0.0.4/sqlargon/dialects/__init__.py
+-rw-r--r--   0        0        0      206 2023-04-15 19:35:30.082581 sqlargon-0.0.4/sqlargon/dialects/postgres.py
+-rw-r--r--   0        0        0      243 2023-04-15 19:35:30.082581 sqlargon-0.0.4/sqlargon/dialects/sqlite.py
+-rw-r--r--   0        0        0     6243 2023-04-15 19:35:30.082581 sqlargon-0.0.4/sqlargon/function_elements.py
+-rw-r--r--   0        0        0        0 2023-04-15 19:35:30.082581 sqlargon-0.0.4/sqlargon/integrations/__init__.py
+-rw-r--r--   0        0        0      858 2023-04-15 19:35:30.082581 sqlargon-0.0.4/sqlargon/integrations/fastapi.py
+-rw-r--r--   0        0        0     1315 2023-04-15 19:35:30.082581 sqlargon-0.0.4/sqlargon/mixins.py
+-rw-r--r--   0        0        0      913 2023-04-15 19:35:30.082581 sqlargon-0.0.4/sqlargon/orm.py
+-rw-r--r--   0        0        0        0 2023-04-15 19:35:30.082581 sqlargon-0.0.4/sqlargon/py.typed
+-rw-r--r--   0        0        0     7358 2023-04-15 19:35:30.082581 sqlargon-0.0.4/sqlargon/repository.py
+-rw-r--r--   0        0        0      803 2023-04-15 19:35:30.082581 sqlargon-0.0.4/sqlargon/settings.py
+-rw-r--r--   0        0        0     3033 2023-04-15 19:35:30.082581 sqlargon-0.0.4/sqlargon/types.py
+-rw-r--r--   0        0        0      255 2023-04-15 19:35:30.082581 sqlargon-0.0.4/sqlargon/util.py
+-rw-r--r--   0        0        0     3975 1970-01-01 00:00:00.000000 sqlargon-0.0.4/PKG-INFO
```

### Comparing `sqlargon-0.0.3/LICENSE` & `sqlargon-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlargon-0.0.3/README.md` & `sqlargon-0.0.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 ![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)
 [![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit)
 
 
 *Wrapper around SQLAlchemy async session, core and Postgres native features*
 
 ---
-Version: 0.0.3
+Version: 0.0.4
 
 Documentation: https://performancemedia.github.io/sqlargon/
 
 Repository: https://github.com/performancemedia/sqlargon
 
 ---
 
@@ -83,26 +83,27 @@
 
 Manager object needs `sqlalchemy.ext.asyncio.AsyncSession`, but it's possible
 to provide the session object by yourself, by subclassing Manager class e.g.
 
 
 ```python
 from fastapi import Depends
-from sqlalchemy.ext.asyncio import AsyncSession
-from sqlargon import Database, SQLAlchemyModelRepository
+from sqlargon import Database
+from sqlargon.integrations.fastapi import FastapiRepositoryProvider
 
-db = Database(url="sqlite+aiosqlite:///:memory:", use_depends=True)
+db = Database(url="sqlite+aiosqlite:///:memory:")
+di = FastapiRepositoryProvider(db)
 
 
 class UserRepository(Repository[User]):
     ...
         
-# then in fastapi
+
 from fastapi import FastAPI
 
 app = FastAPI()
 
 @app.get("/users")
-async def get_users(user_repository: UserRepository = Depends(UserRepository)):
+async def get_users(user_repository: UserRepository = Depends(di[UserRepository])):
     return await user_repository.all()
 
 ```
```

### Comparing `sqlargon-0.0.3/pyproject.toml` & `sqlargon-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sqlargon"
-version = "0.0.3"
+version = "0.0.4"
 description = "SQLAlchemy utils for Postgres and Sqlite"
 readme = "README.md"
 authors = [
     "Radzim Kowalow <radzim.kowalow@performance-media.pl>"
 ]
 
 [tool.poetry.dependencies]
```

### Comparing `sqlargon-0.0.3/sqlargon/db.py` & `sqlargon-0.0.4/sqlargon/db.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,15 +30,14 @@
         pool_size: int = 10,
         max_overflow: int = 0,
         pool_recycle: int = 1200,
         echo: bool = False,
         echo_pool: bool = True,
         json_serializer: Callable[[Any], str] = json_dumps,
         json_deserializer: Callable[[str], Any] = json_loads,
-        use_depends: bool = False,
         **kwargs: Any,
     ) -> None:
         self.engine = create_async_engine(
             url=url,
             poolclass=poolclass,
             pool_size=pool_size,
             max_overflow=max_overflow,
@@ -52,19 +51,14 @@
 
         self.session_maker = async_sessionmaker(
             bind=self.engine, expire_on_commit=False
         )
         self.session = asynccontextmanager(self.session_factory)
         configure_repository_class(self.engine.url.get_dialect().name)
 
-        if use_depends:
-            from .integrations.fastapi import fastapi_integration
-
-            fastapi_integration(self.session_factory)
-
     async def session_factory(self) -> AsyncGenerator[AsyncSession, None]:
         async with self.session_maker() as session:
             try:
                 yield session
                 await session.commit()
             except:  # noqa
                 await session.rollback()
```

### Comparing `sqlargon-0.0.3/sqlargon/function_elements.py` & `sqlargon-0.0.4/sqlargon/function_elements.py`

 * *Files identical despite different names*

### Comparing `sqlargon-0.0.3/sqlargon/mixins.py` & `sqlargon-0.0.4/sqlargon/mixins.py`

 * *Files identical despite different names*

### Comparing `sqlargon-0.0.3/sqlargon/orm.py` & `sqlargon-0.0.4/sqlargon/orm.py`

 * *Files identical despite different names*

### Comparing `sqlargon-0.0.3/sqlargon/repository.py` & `sqlargon-0.0.4/sqlargon/repository.py`

 * *Files identical despite different names*

### Comparing `sqlargon-0.0.3/sqlargon/settings.py` & `sqlargon-0.0.4/sqlargon/settings.py`

 * *Files identical despite different names*

### Comparing `sqlargon-0.0.3/sqlargon/types.py` & `sqlargon-0.0.4/sqlargon/types.py`

 * *Files identical despite different names*

### Comparing `sqlargon-0.0.3/PKG-INFO` & `sqlargon-0.0.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlargon
-Version: 0.0.3
+Version: 0.0.4
 Summary: SQLAlchemy utils for Postgres and Sqlite
 Author: Radzim Kowalow
 Author-email: radzim.kowalow@performance-media.pl
 Requires-Python: >=3.8.1,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -29,15 +29,15 @@
 ![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)
 [![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit)
 
 
 *Wrapper around SQLAlchemy async session, core and Postgres native features*
 
 ---
-Version: 0.0.3
+Version: 0.0.4
 
 Documentation: https://performancemedia.github.io/sqlargon/
 
 Repository: https://github.com/performancemedia/sqlargon
 
 ---
 
@@ -102,27 +102,28 @@
 
 Manager object needs `sqlalchemy.ext.asyncio.AsyncSession`, but it's possible
 to provide the session object by yourself, by subclassing Manager class e.g.
 
 
 ```python
 from fastapi import Depends
-from sqlalchemy.ext.asyncio import AsyncSession
-from sqlargon import Database, SQLAlchemyModelRepository
+from sqlargon import Database
+from sqlargon.integrations.fastapi import FastapiRepositoryProvider
 
-db = Database(url="sqlite+aiosqlite:///:memory:", use_depends=True)
+db = Database(url="sqlite+aiosqlite:///:memory:")
+di = FastapiRepositoryProvider(db)
 
 
 class UserRepository(Repository[User]):
     ...
         
-# then in fastapi
+
 from fastapi import FastAPI
 
 app = FastAPI()
 
 @app.get("/users")
-async def get_users(user_repository: UserRepository = Depends(UserRepository)):
+async def get_users(user_repository: UserRepository = Depends(di[UserRepository])):
     return await user_repository.all()
 
 ```
```

