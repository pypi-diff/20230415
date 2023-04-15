# Comparing `tmp/fastapi_amis_admin_nav-0.0.3.tar.gz` & `tmp/fastapi_amis_admin_nav-0.0.4a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_amis_admin_nav-0.0.3.tar", last modified: Sat Apr 15 08:17:47 2023, max compression
+gzip compressed data, was "fastapi_amis_admin_nav-0.0.4a1.tar", last modified: Sat Apr 15 09:28:24 2023, max compression
```

## Comparing `fastapi_amis_admin_nav-0.0.3.tar` & `fastapi_amis_admin_nav-0.0.4a1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     3037 2023-02-19 04:26:35.599654 fastapi_amis_admin_nav-0.0.3/README.md
--rw-r--r--   0        0        0      380 2023-04-15 08:13:58.179332 fastapi_amis_admin_nav-0.0.3/fastapi_amis_admin_nav/__init__.py
--rw-r--r--   0        0        0     5168 2023-03-23 08:41:54.647360 fastapi_amis_admin_nav-0.0.3/fastapi_amis_admin_nav/admin.py
--rw-r--r--   0        0        0     4791 2023-04-15 08:12:51.041482 fastapi_amis_admin_nav-0.0.3/fastapi_amis_admin_nav/models.py
--rw-r--r--   0        0        0     8437 2023-03-23 11:45:23.744360 fastapi_amis_admin_nav-0.0.3/fastapi_amis_admin_nav/utils.py
--rw-r--r--   0        0        0     1645 2023-03-22 07:48:40.603529 fastapi_amis_admin_nav-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     4108 1970-01-01 00:00:00.000000 fastapi_amis_admin_nav-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     3037 2023-02-19 04:26:35.599654 fastapi_amis_admin_nav-0.0.4a1/README.md
+-rw-r--r--   0        0        0      382 2023-04-15 09:28:19.081403 fastapi_amis_admin_nav-0.0.4a1/fastapi_amis_admin_nav/__init__.py
+-rw-r--r--   0        0        0     5168 2023-03-23 08:41:54.647360 fastapi_amis_admin_nav-0.0.4a1/fastapi_amis_admin_nav/admin.py
+-rw-r--r--   0        0        0     4715 2023-04-15 09:15:19.759421 fastapi_amis_admin_nav-0.0.4a1/fastapi_amis_admin_nav/models.py
+-rw-r--r--   0        0        0     8437 2023-03-23 11:45:23.744360 fastapi_amis_admin_nav-0.0.4a1/fastapi_amis_admin_nav/utils.py
+-rw-r--r--   0        0        0     1645 2023-03-22 07:48:40.603529 fastapi_amis_admin_nav-0.0.4a1/pyproject.toml
+-rw-r--r--   0        0        0     4110 1970-01-01 00:00:00.000000 fastapi_amis_admin_nav-0.0.4a1/PKG-INFO
```

### Comparing `fastapi_amis_admin_nav-0.0.3/README.md` & `fastapi_amis_admin_nav-0.0.4a1/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin_nav-0.0.3/fastapi_amis_admin_nav/admin.py` & `fastapi_amis_admin_nav-0.0.4a1/fastapi_amis_admin_nav/admin.py`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin_nav-0.0.3/fastapi_amis_admin_nav/models.py` & `fastapi_amis_admin_nav-0.0.4a1/fastapi_amis_admin_nav/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,16 +82,14 @@
         page = PageSchema.parse_raw(self.page_schema)
         page.label = self.label or page.label
         page.icon = self.icon or page.icon
         page.url = self.url or page.url or f"/{self.unique_id}"
         page.sort = self.sort
         if self.is_group:  # 如果是分组,则同步tabsMode
             page.tabsMode = self.tabs_mode
-            if page.tabsMode is None:
-                page.schemaApi = None
         page.visible = self.visible
         return page
 
     @classmethod
     def parse_page_schema(cls, obj: PageSchema, **kwargs):
         data = obj.dict(include={"label", "url", "icon", "sort", "visible"})
         data.update(
```

### Comparing `fastapi_amis_admin_nav-0.0.3/fastapi_amis_admin_nav/utils.py` & `fastapi_amis_admin_nav-0.0.4a1/fastapi_amis_admin_nav/utils.py`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin_nav-0.0.3/pyproject.toml` & `fastapi_amis_admin_nav-0.0.4a1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin_nav-0.0.3/PKG-INFO` & `fastapi_amis_admin_nav-0.0.4a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi_amis_admin_nav
-Version: 0.0.3
+Version: 0.0.4a1
 Summary: FastAPI-Amis-Admin-Nav是一个基于FastAPI-Amis-Admin并且为FastAPI-Amis-Admin提供可视化导航页面管理的拓展库.
 Keywords: fastapi,fastapi-user-auth,fastapi-amis-admin,fastapi-amis-admin-nav
 Author-email: Atomi <1456417373@qq.com>
 Maintainer-email: Atomi <1456417373@qq.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Framework :: FastAPI
```

