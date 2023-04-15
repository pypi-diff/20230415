# Comparing `tmp/fastapi_amis_admin_nav-0.0.2.tar.gz` & `tmp/fastapi_amis_admin_nav-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_amis_admin_nav-0.0.2.tar", last modified: Thu Mar 23 12:20:48 2023, max compression
+gzip compressed data, was "fastapi_amis_admin_nav-0.0.3.tar", last modified: Sat Apr 15 08:17:47 2023, max compression
```

## Comparing `fastapi_amis_admin_nav-0.0.2.tar` & `fastapi_amis_admin_nav-0.0.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     3037 2023-02-19 04:26:35.599654 fastapi_amis_admin_nav-0.0.2/README.md
--rw-r--r--   0        0        0      380 2023-03-22 07:48:40.590534 fastapi_amis_admin_nav-0.0.2/fastapi_amis_admin_nav/__init__.py
--rw-r--r--   0        0        0     5168 2023-03-23 08:41:54.647360 fastapi_amis_admin_nav-0.0.2/fastapi_amis_admin_nav/admin.py
--rw-r--r--   0        0        0     4814 2023-03-04 12:55:08.289780 fastapi_amis_admin_nav-0.0.2/fastapi_amis_admin_nav/models.py
--rw-r--r--   0        0        0     8437 2023-03-23 11:45:23.744360 fastapi_amis_admin_nav-0.0.2/fastapi_amis_admin_nav/utils.py
--rw-r--r--   0        0        0     1645 2023-03-22 07:48:40.603529 fastapi_amis_admin_nav-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     4108 1970-01-01 00:00:00.000000 fastapi_amis_admin_nav-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     3037 2023-02-19 04:26:35.599654 fastapi_amis_admin_nav-0.0.3/README.md
+-rw-r--r--   0        0        0      380 2023-04-15 08:13:58.179332 fastapi_amis_admin_nav-0.0.3/fastapi_amis_admin_nav/__init__.py
+-rw-r--r--   0        0        0     5168 2023-03-23 08:41:54.647360 fastapi_amis_admin_nav-0.0.3/fastapi_amis_admin_nav/admin.py
+-rw-r--r--   0        0        0     4791 2023-04-15 08:12:51.041482 fastapi_amis_admin_nav-0.0.3/fastapi_amis_admin_nav/models.py
+-rw-r--r--   0        0        0     8437 2023-03-23 11:45:23.744360 fastapi_amis_admin_nav-0.0.3/fastapi_amis_admin_nav/utils.py
+-rw-r--r--   0        0        0     1645 2023-03-22 07:48:40.603529 fastapi_amis_admin_nav-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     4108 1970-01-01 00:00:00.000000 fastapi_amis_admin_nav-0.0.3/PKG-INFO
```

### Comparing `fastapi_amis_admin_nav-0.0.2/README.md` & `fastapi_amis_admin_nav-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin_nav-0.0.2/fastapi_amis_admin_nav/admin.py` & `fastapi_amis_admin_nav-0.0.3/fastapi_amis_admin_nav/admin.py`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin_nav-0.0.2/fastapi_amis_admin_nav/models.py` & `fastapi_amis_admin_nav-0.0.3/fastapi_amis_admin_nav/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,14 @@
         title="更新时间",
         sa_column_kwargs={"onupdate": func.now(), "server_default": func.now()},
     )
     type: NavPageType = Field(NavPageType.Custom, title="页面类型")
     url: str = Field(
         "",
         title="页面路径",
-        max_length=50,
         amis_form_item={  # 非自定义页面, 都是只读
             "disabledOn": "!this.is_custom",
         },
     )
     label: str = Field(..., title="页面名称", max_length=20)
     icon: str = Field(default="fa fa-flash", title="页面图标", max_length=50)
     sort: int = Field(0, title="排序")
```

### Comparing `fastapi_amis_admin_nav-0.0.2/fastapi_amis_admin_nav/utils.py` & `fastapi_amis_admin_nav-0.0.3/fastapi_amis_admin_nav/utils.py`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin_nav-0.0.2/pyproject.toml` & `fastapi_amis_admin_nav-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin_nav-0.0.2/PKG-INFO` & `fastapi_amis_admin_nav-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi_amis_admin_nav
-Version: 0.0.2
+Version: 0.0.3
 Summary: FastAPI-Amis-Admin-Nav是一个基于FastAPI-Amis-Admin并且为FastAPI-Amis-Admin提供可视化导航页面管理的拓展库.
 Keywords: fastapi,fastapi-user-auth,fastapi-amis-admin,fastapi-amis-admin-nav
 Author-email: Atomi <1456417373@qq.com>
 Maintainer-email: Atomi <1456417373@qq.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Framework :: FastAPI
```

