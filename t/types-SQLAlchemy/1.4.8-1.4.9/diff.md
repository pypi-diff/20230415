# Comparing `tmp/types-SQLAlchemy-1.4.8.tar.gz` & `tmp/types-SQLAlchemy-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-SQLAlchemy-1.4.8.tar", last modified: Sun Jan  9 15:18:06 2022, max compression
+gzip compressed data, was "types-SQLAlchemy-1.4.9.tar", last modified: Mon Jan 10 03:20:03 2022, max compression
```

## Comparing `types-SQLAlchemy-1.4.8.tar` & `types-SQLAlchemy-1.4.9.tar`

### file list

```diff
@@ -1,264 +1,264 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 15:18:06.012390 types-SQLAlchemy-1.4.8/
--rw-r--r--   0 runner    (1001) docker     (121)      618 2022-01-09 15:18:04.000000 types-SQLAlchemy-1.4.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-01-09 15:18:04.000000 types-SQLAlchemy-1.4.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      999 2022-01-09 15:18:06.012390 types-SQLAlchemy-1.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-09 15:18:06.012390 types-SQLAlchemy-1.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     6938 2022-01-09 15:18:04.000000 types-SQLAlchemy-1.4.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 15:18:05.972389 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/
--rw-r--r--   0 runner    (1001) docker     (121)      175 2022-01-09 15:18:04.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (121)     3389 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      693 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/cimmutabledict.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 15:18:05.972389 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/connectors/
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/connectors/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      610 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/connectors/mxodbc.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      771 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/connectors/pyodbc.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      308 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/cresultproxy.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 15:18:05.972389 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/databases/
--rw-r--r--   0 runner    (1001) docker     (121)      627 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/databases/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1619 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dbapi.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 15:18:05.972389 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/
--rw-r--r--   0 runner    (1001) docker     (121)      318 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 15:18:05.972389 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/firebird/
--rw-r--r--   0 runner    (1001) docker     (121)      528 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/firebird/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     4148 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/firebird/base.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      335 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/firebird/fdb.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1260 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/firebird/kinterbasdb.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 15:18:05.976389 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/mssql/
--rw-r--r--   0 runner    (1001) docker     (121)     1389 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/mssql/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    11224 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/mssql/base.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      732 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/mssql/information_schema.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      300 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/mssql/json.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      789 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/mssql/mxodbc.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/mssql/provision.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      689 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/mssql/pymssql.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1505 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/mssql/pyodbc.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 15:18:05.980389 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/mysql/
--rw-r--r--   0 runner    (1001) docker     (121)     1509 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/mysql/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2262 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/mysql/aiomysql.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2251 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/mysql/asyncmy.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     9639 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/mysql/base.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      556 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/mysql/cymysql.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      602 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/mysql/dml.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      697 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/mysql/enumerated.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      399 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/mysql/expression.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      325 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/mysql/json.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      205 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/mysql/mariadb.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1321 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/mysql/mariadbconnector.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1233 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/mysql/mysqlconnector.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1039 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/mysql/mysqldb.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1762 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/mysql/oursql.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/mysql/provision.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      586 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/mysql/pymysql.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      563 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/mysql/pyodbc.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      392 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/mysql/reflection.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       78 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/mysql/reserved_words.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     4752 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/mysql/types.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 15:18:05.980389 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/oracle/
--rw-r--r--   0 runner    (1001) docker     (121)      900 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/oracle/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     8360 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/oracle/base.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     4200 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/oracle/cx_oracle.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/oracle/provision.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 15:18:05.984389 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/postgresql/
--rw-r--r--   0 runner    (1001) docker     (121)     1967 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/postgresql/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1214 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/postgresql/array.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     6384 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/postgresql/asyncpg.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    12128 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/postgresql/base.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1433 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/postgresql/dml.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      725 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/postgresql/ext.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1783 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/postgresql/hstore.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      781 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/postgresql/json.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     4536 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/postgresql/pg8000.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/postgresql/provision.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     3008 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/postgresql/psycopg2.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      309 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/postgresql/psycopg2cffi.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1525 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/postgresql/pygresql.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      905 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/postgresql/pypostgresql.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1104 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/postgresql/ranges.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 15:18:05.984389 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/sqlite/
--rw-r--r--   0 runner    (1001) docker     (121)      737 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/sqlite/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2322 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/sqlite/aiosqlite.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     5816 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/sqlite/base.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1217 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/sqlite/dml.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      300 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/sqlite/json.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/sqlite/provision.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      411 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/sqlite/pysqlcipher.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      836 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/sqlite/pysqlite.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 15:18:05.984389 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/sybase/
--rw-r--r--   0 runner    (1001) docker     (121)      969 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/sybase/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     4643 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/sybase/base.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      333 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/sybase/mxodbc.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      666 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/sybase/pyodbc.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      947 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/sybase/pysybase.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 15:18:05.988390 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/engine/
--rw-r--r--   0 runner    (1001) docker     (121)     1738 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/engine/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     8475 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/engine/base.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      667 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/engine/characteristics.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      866 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/engine/create.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     4835 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/engine/cursor.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     7520 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/engine/default.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1793 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/engine/events.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     7823 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/engine/interfaces.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1207 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/engine/mock.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1665 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/engine/reflection.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     3724 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/engine/result.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1466 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/engine/row.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/engine/strategies.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2449 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/engine/url.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      399 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/engine/util.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 15:18:05.988390 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/event/
--rw-r--r--   0 runner    (1001) docker     (121)      283 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/event/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      257 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/event/api.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2510 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/event/attr.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      724 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/event/base.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/event/legacy.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      776 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/event/registry.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      254 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/events.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     4236 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/exc.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 15:18:05.992390 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/ext/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/ext/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     6425 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/ext/associationproxy.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 15:18:05.992390 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/ext/asyncio/
--rw-r--r--   0 runner    (1001) docker     (121)      691 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/ext/asyncio/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      462 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/ext/asyncio/base.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     3458 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/ext/asyncio/engine.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      204 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/ext/asyncio/events.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      206 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/ext/asyncio/exc.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2038 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/ext/asyncio/result.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2873 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/ext/asyncio/scoping.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     3983 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/ext/asyncio/session.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      960 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/ext/automap.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1203 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/ext/baked.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      218 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/ext/compiler.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 15:18:05.992390 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/ext/declarative/
--rw-r--r--   0 runner    (1001) docker     (121)      735 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/ext/declarative/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      364 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/ext/declarative/extensions.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      907 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/ext/horizontal_shard.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1836 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/ext/hybrid.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      478 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/ext/indexable.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2443 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/ext/instrumentation.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2243 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/ext/mutable.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 15:18:05.996390 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/ext/mypy/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/ext/mypy/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      922 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/ext/mypy/apply.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      274 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/ext/mypy/decl_class.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      914 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/ext/mypy/infer.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1235 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/ext/mypy/names.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1078 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/ext/mypy/plugin.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2394 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/ext/mypy/util.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      818 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/ext/orderinglist.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      316 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/ext/serializer.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 15:18:05.996390 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/future/
--rw-r--r--   0 runner    (1001) docker     (121)      132 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/future/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1333 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/future/engine.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 15:18:05.996390 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/future/orm/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/future/orm/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/inspection.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1324 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/log.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 15:18:06.000390 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/orm/
--rw-r--r--   0 runner    (1001) docker     (121)     3898 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/orm/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     8377 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/orm/attributes.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1591 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/orm/base.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1401 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/orm/clsregistry.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2800 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/orm/collections.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     5849 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/orm/context.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     4658 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/orm/decl_api.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1363 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/orm/decl_base.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     3295 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/orm/dependency.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1930 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/orm/descriptor_props.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2745 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/orm/dynamic.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      792 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/orm/evaluator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     4791 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/orm/events.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/orm/exc.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1094 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/orm/identity.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2806 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/orm/instrumentation.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     4558 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/orm/interfaces.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1474 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/orm/loading.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     4630 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/orm/mapper.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2855 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/orm/path_registry.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1093 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/orm/persistence.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1478 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/orm/properties.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     4994 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/orm/query.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     5462 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/orm/relationships.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     3577 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/orm/scoping.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     6762 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/orm/session.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1932 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/orm/state.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     5454 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/orm/strategies.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2502 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/orm/strategy_options.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      511 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/orm/sync.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     3183 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/orm/unitofwork.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     5477 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/orm/util.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 15:18:06.000390 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/pool/
--rw-r--r--   0 runner    (1001) docker     (121)      795 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/pool/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2506 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/pool/base.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      483 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/pool/dbapi_proxy.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      815 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/pool/events.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1282 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/pool/impl.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      324 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/processors.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1725 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/schema.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 15:18:06.008390 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/sql/
--rw-r--r--   0 runner    (1001) docker     (121)     2489 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/sql/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      483 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/sql/annotation.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     4820 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/sql/base.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2613 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/sql/coercions.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    19391 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/sql/compiler.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      324 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/sql/crud.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     4678 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/sql/ddl.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/sql/default_comparator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     3275 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/sql/dml.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    12855 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/sql/elements.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      515 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/sql/events.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     4617 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/sql/expression.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     5478 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/sql/functions.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     3252 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/sql/lambdas.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      230 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/sql/naming.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     5581 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/sql/operators.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2091 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/sql/roles.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    10924 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/sql/schema.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    13936 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/sql/selectable.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    10468 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/sql/sqltypes.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     9722 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/sql/traversals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     3731 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/sql/type_api.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     3104 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/sql/util.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2660 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/sql/visitors.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 15:18:06.008390 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/testing/
--rw-r--r--   0 runner    (1001) docker     (121)     2353 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/testing/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     3482 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/testing/assertions.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2312 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/testing/assertsql.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/testing/asyncio.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1155 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/testing/config.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2265 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/testing/engines.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      234 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/testing/entities.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2337 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/testing/exclusions.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2338 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/testing/fixtures.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/testing/mock.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1451 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/testing/pickleable.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 15:18:06.008390 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/testing/plugin/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/testing/plugin/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       98 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/testing/plugin/bootstrap.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1700 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/testing/plugin/plugin_base.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1246 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/testing/plugin/pytestplugin.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      300 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/testing/plugin/reinvent_fixtures_py2k.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      584 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/testing/profiling.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1388 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/testing/provision.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    10326 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/testing/requirements.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      384 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/testing/schema.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1377 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/testing/util.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      216 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/testing/warnings.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2049 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/types.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 15:18:06.012390 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/util/
--rw-r--r--   0 runner    (1001) docker     (121)     5956 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/util/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     8548 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/util/_collections.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      275 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/util/_compat_py3k.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      755 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/util/_concurrency_py3k.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      267 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/util/_preloaded.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2569 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/util/compat.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      361 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/util/concurrency.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1023 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/util/deprecations.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     5463 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/util/langhelpers.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1041 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/util/queue.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      163 2022-01-09 15:17:52.000000 types-SQLAlchemy-1.4.8/sqlalchemy-stubs/util/topological.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 15:18:06.012390 types-SQLAlchemy-1.4.8/types_SQLAlchemy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      999 2022-01-09 15:18:05.000000 types-SQLAlchemy-1.4.8/types_SQLAlchemy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     9031 2022-01-09 15:18:05.000000 types-SQLAlchemy-1.4.8/types_SQLAlchemy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-09 15:18:05.000000 types-SQLAlchemy-1.4.8/types_SQLAlchemy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-01-09 15:18:05.000000 types-SQLAlchemy-1.4.8/types_SQLAlchemy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-10 03:20:03.178900 types-SQLAlchemy-1.4.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1767 2022-01-10 03:20:02.000000 types-SQLAlchemy-1.4.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (121)       21 2022-01-10 03:20:02.000000 types-SQLAlchemy-1.4.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)      999 2022-01-10 03:20:03.178900 types-SQLAlchemy-1.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-10 03:20:03.178900 types-SQLAlchemy-1.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     6938 2022-01-10 03:20:02.000000 types-SQLAlchemy-1.4.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-10 03:20:03.146900 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/
+-rw-r--r--   0 runner    (1001) docker     (121)      175 2022-01-10 03:20:02.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (121)     3389 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      693 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/cimmutabledict.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-10 03:20:03.150900 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/connectors/
+-rw-r--r--   0 runner    (1001) docker     (121)       21 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/connectors/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      610 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/connectors/mxodbc.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      771 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/connectors/pyodbc.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      308 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/cresultproxy.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-10 03:20:03.150900 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/databases/
+-rw-r--r--   0 runner    (1001) docker     (121)      627 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/databases/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1619 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dbapi.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-10 03:20:03.150900 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/
+-rw-r--r--   0 runner    (1001) docker     (121)      318 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-10 03:20:03.150900 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/firebird/
+-rw-r--r--   0 runner    (1001) docker     (121)      528 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/firebird/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     4148 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/firebird/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      335 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/firebird/fdb.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1260 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/firebird/kinterbasdb.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-10 03:20:03.150900 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/mssql/
+-rw-r--r--   0 runner    (1001) docker     (121)     1389 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/mssql/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)    11224 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/mssql/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      732 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/mssql/information_schema.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      300 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/mssql/json.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      789 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/mssql/mxodbc.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/mssql/provision.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      689 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/mssql/pymssql.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1505 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/mssql/pyodbc.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-10 03:20:03.154900 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/mysql/
+-rw-r--r--   0 runner    (1001) docker     (121)     1509 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/mysql/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     2262 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/mysql/aiomysql.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     2251 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/mysql/asyncmy.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     9639 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/mysql/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      556 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/mysql/cymysql.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      602 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/mysql/dml.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      697 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/mysql/enumerated.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      399 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/mysql/expression.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      325 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/mysql/json.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      205 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/mysql/mariadb.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1321 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/mysql/mariadbconnector.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1233 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/mysql/mysqlconnector.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1039 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/mysql/mysqldb.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1762 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/mysql/oursql.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/mysql/provision.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      586 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/mysql/pymysql.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      563 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/mysql/pyodbc.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      392 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/mysql/reflection.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       78 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/mysql/reserved_words.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     4752 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/mysql/types.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-10 03:20:03.154900 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/oracle/
+-rw-r--r--   0 runner    (1001) docker     (121)      900 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/oracle/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     8360 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/oracle/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     4200 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/oracle/cx_oracle.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/oracle/provision.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-10 03:20:03.154900 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/postgresql/
+-rw-r--r--   0 runner    (1001) docker     (121)     1967 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/postgresql/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1214 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/postgresql/array.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     6384 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/postgresql/asyncpg.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)    12128 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/postgresql/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1433 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/postgresql/dml.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      725 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/postgresql/ext.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1783 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/postgresql/hstore.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      781 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/postgresql/json.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     4536 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/postgresql/pg8000.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/postgresql/provision.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     3008 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/postgresql/psycopg2.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      309 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/postgresql/psycopg2cffi.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1525 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/postgresql/pygresql.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      905 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/postgresql/pypostgresql.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1104 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/postgresql/ranges.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-10 03:20:03.158900 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/sqlite/
+-rw-r--r--   0 runner    (1001) docker     (121)      737 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/sqlite/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     2322 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/sqlite/aiosqlite.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     5816 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/sqlite/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1217 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/sqlite/dml.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      300 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/sqlite/json.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/sqlite/provision.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      411 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/sqlite/pysqlcipher.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      836 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/sqlite/pysqlite.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-10 03:20:03.158900 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/sybase/
+-rw-r--r--   0 runner    (1001) docker     (121)      969 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/sybase/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     4643 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/sybase/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      333 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/sybase/mxodbc.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      666 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/sybase/pyodbc.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      947 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/sybase/pysybase.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-10 03:20:03.158900 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/engine/
+-rw-r--r--   0 runner    (1001) docker     (121)     1738 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/engine/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     8475 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/engine/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      667 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/engine/characteristics.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      866 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/engine/create.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     4835 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/engine/cursor.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     7520 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/engine/default.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1793 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/engine/events.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     7823 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/engine/interfaces.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1207 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/engine/mock.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1665 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/engine/reflection.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     3724 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/engine/result.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1466 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/engine/row.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       74 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/engine/strategies.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     2449 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/engine/url.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      399 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/engine/util.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-10 03:20:03.158900 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/event/
+-rw-r--r--   0 runner    (1001) docker     (121)      283 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/event/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      257 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/event/api.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     2510 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/event/attr.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      724 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/event/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/event/legacy.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      776 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/event/registry.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      254 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/events.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     4236 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/exc.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-10 03:20:03.162900 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/ext/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/ext/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     6425 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/ext/associationproxy.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-10 03:20:03.162900 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/ext/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (121)      691 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/ext/asyncio/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      462 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/ext/asyncio/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     3458 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/ext/asyncio/engine.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      204 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/ext/asyncio/events.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      206 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/ext/asyncio/exc.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     2038 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/ext/asyncio/result.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     2873 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/ext/asyncio/scoping.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     3983 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/ext/asyncio/session.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      960 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/ext/automap.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1203 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/ext/baked.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      218 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/ext/compiler.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-10 03:20:03.162900 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/ext/declarative/
+-rw-r--r--   0 runner    (1001) docker     (121)      735 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/ext/declarative/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      364 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/ext/declarative/extensions.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      907 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/ext/horizontal_shard.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1836 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/ext/hybrid.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      478 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/ext/indexable.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     2443 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/ext/instrumentation.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     2243 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/ext/mutable.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-10 03:20:03.162900 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/ext/mypy/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/ext/mypy/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      922 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/ext/mypy/apply.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      274 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/ext/mypy/decl_class.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      914 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/ext/mypy/infer.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1235 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/ext/mypy/names.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1078 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/ext/mypy/plugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     2394 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/ext/mypy/util.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      818 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/ext/orderinglist.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      316 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/ext/serializer.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-10 03:20:03.162900 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/future/
+-rw-r--r--   0 runner    (1001) docker     (121)      132 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/future/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1333 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/future/engine.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-10 03:20:03.162900 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/future/orm/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/future/orm/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       48 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/inspection.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1324 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/log.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-10 03:20:03.166900 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/orm/
+-rw-r--r--   0 runner    (1001) docker     (121)     3898 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/orm/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     8377 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/orm/attributes.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1591 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/orm/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1401 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/orm/clsregistry.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     2800 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/orm/collections.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     5849 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/orm/context.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     4658 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/orm/decl_api.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1363 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/orm/decl_base.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     3295 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/orm/dependency.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1930 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/orm/descriptor_props.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     2745 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/orm/dynamic.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      792 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/orm/evaluator.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     4791 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/orm/events.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/orm/exc.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1094 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/orm/identity.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     2806 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/orm/instrumentation.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     4558 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/orm/interfaces.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1474 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/orm/loading.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     4630 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/orm/mapper.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     2855 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/orm/path_registry.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1093 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/orm/persistence.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1478 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/orm/properties.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     4994 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/orm/query.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     5462 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/orm/relationships.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     3577 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/orm/scoping.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     6762 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/orm/session.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1932 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/orm/state.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     5454 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/orm/strategies.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     2502 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/orm/strategy_options.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      511 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/orm/sync.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     3183 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/orm/unitofwork.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     5477 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/orm/util.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-10 03:20:03.170900 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/pool/
+-rw-r--r--   0 runner    (1001) docker     (121)      795 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/pool/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     2506 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/pool/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      483 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/pool/dbapi_proxy.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      815 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/pool/events.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1282 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/pool/impl.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      324 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/processors.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1725 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/schema.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-10 03:20:03.170900 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/sql/
+-rw-r--r--   0 runner    (1001) docker     (121)     2489 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/sql/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      483 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/sql/annotation.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     4820 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/sql/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     2613 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/sql/coercions.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)    19391 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/sql/compiler.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      324 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/sql/crud.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     4678 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/sql/ddl.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       45 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/sql/default_comparator.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     3275 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/sql/dml.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)    12855 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/sql/elements.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      515 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/sql/events.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     4617 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/sql/expression.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     5478 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/sql/functions.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     3252 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/sql/lambdas.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      230 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/sql/naming.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     5581 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/sql/operators.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     2091 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/sql/roles.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)    10924 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/sql/schema.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)    13936 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/sql/selectable.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)    10468 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/sql/sqltypes.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     9722 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/sql/traversals.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     3731 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/sql/type_api.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     3104 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/sql/util.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     2660 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/sql/visitors.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-10 03:20:03.174900 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/testing/
+-rw-r--r--   0 runner    (1001) docker     (121)     2353 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/testing/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     3482 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/testing/assertions.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     2312 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/testing/assertsql.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       21 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/testing/asyncio.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1155 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/testing/config.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     2265 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/testing/engines.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      234 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/testing/entities.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     2337 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/testing/exclusions.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     2338 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/testing/fixtures.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/testing/mock.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1451 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/testing/pickleable.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-10 03:20:03.174900 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/testing/plugin/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/testing/plugin/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       98 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/testing/plugin/bootstrap.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1700 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/testing/plugin/plugin_base.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1246 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/testing/plugin/pytestplugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      300 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/testing/plugin/reinvent_fixtures_py2k.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      584 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/testing/profiling.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1388 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/testing/provision.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)    10326 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/testing/requirements.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      384 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/testing/schema.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1377 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/testing/util.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      216 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/testing/warnings.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     2049 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/types.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-10 03:20:03.178900 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/util/
+-rw-r--r--   0 runner    (1001) docker     (121)     5956 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/util/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     8548 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/util/_collections.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      275 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/util/_compat_py3k.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      755 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/util/_concurrency_py3k.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      267 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/util/_preloaded.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     2569 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/util/compat.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      361 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/util/concurrency.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1023 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/util/deprecations.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     5483 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/util/langhelpers.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1041 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/util/queue.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      163 2022-01-10 03:19:42.000000 types-SQLAlchemy-1.4.9/sqlalchemy-stubs/util/topological.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-10 03:20:03.178900 types-SQLAlchemy-1.4.9/types_SQLAlchemy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      999 2022-01-10 03:20:03.000000 types-SQLAlchemy-1.4.9/types_SQLAlchemy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     9031 2022-01-10 03:20:03.000000 types-SQLAlchemy-1.4.9/types_SQLAlchemy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-10 03:20:03.000000 types-SQLAlchemy-1.4.9/types_SQLAlchemy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2022-01-10 03:20:03.000000 types-SQLAlchemy-1.4.9/types_SQLAlchemy.egg-info/top_level.txt
```

### Comparing `types-SQLAlchemy-1.4.8/PKG-INFO` & `types-SQLAlchemy-1.4.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-SQLAlchemy
-Version: 1.4.8
+Version: 1.4.9
 Summary: Typing stubs for SQLAlchemy
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Typing :: Stubs Only
 Description-Content-Type: text/markdown
@@ -16,10 +16,10 @@
 that uses `SQLAlchemy`. The source for this package can be found at
 https://github.com/python/typeshed/tree/master/stubs/SQLAlchemy. All fixes for
 types and metadata should be contributed there.
 
 The `sqlalchemy-stubs` package is an alternative to this package and also includes a mypy plugin for more precise types.
 
 See https://github.com/python/typeshed/blob/master/README.md for more details.
-This package was generated from typeshed commit `8f7dd8c381ed5e2334da1d47ca03b7a5f42c4394`.
+This package was generated from typeshed commit `96c9abb0585bb052bbb36228aa616857b987867b`.
```

### Comparing `types-SQLAlchemy-1.4.8/setup.py` & `types-SQLAlchemy-1.4.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,19 +10,19 @@
 that uses `SQLAlchemy`. The source for this package can be found at
 https://github.com/python/typeshed/tree/master/stubs/SQLAlchemy. All fixes for
 types and metadata should be contributed there.
 
 The `sqlalchemy-stubs` package is an alternative to this package and also includes a mypy plugin for more precise types.
 
 See https://github.com/python/typeshed/blob/master/README.md for more details.
-This package was generated from typeshed commit `8f7dd8c381ed5e2334da1d47ca03b7a5f42c4394`.
+This package was generated from typeshed commit `96c9abb0585bb052bbb36228aa616857b987867b`.
 '''.lstrip()
 
 setup(name=name,
-      version="1.4.8",
+      version="1.4.9",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       install_requires=[],
       packages=['sqlalchemy-stubs'],
       package_data={'sqlalchemy-stubs': ['__init__.pyi', 'cimmutabledict.pyi', 'connectors/__init__.pyi', 'connectors/mxodbc.pyi', 'connectors/pyodbc.pyi', 'cresultproxy.pyi', 'databases/__init__.pyi', 'dbapi.pyi', 'dialects/__init__.pyi', 'dialects/firebird/__init__.pyi', 'dialects/firebird/base.pyi', 'dialects/firebird/fdb.pyi', 'dialects/firebird/kinterbasdb.pyi', 'dialects/mssql/__init__.pyi', 'dialects/mssql/base.pyi', 'dialects/mssql/information_schema.pyi', 'dialects/mssql/json.pyi', 'dialects/mssql/mxodbc.pyi', 'dialects/mssql/provision.pyi', 'dialects/mssql/pymssql.pyi', 'dialects/mssql/pyodbc.pyi', 'dialects/mysql/__init__.pyi', 'dialects/mysql/aiomysql.pyi', 'dialects/mysql/asyncmy.pyi', 'dialects/mysql/base.pyi', 'dialects/mysql/cymysql.pyi', 'dialects/mysql/dml.pyi', 'dialects/mysql/enumerated.pyi', 'dialects/mysql/expression.pyi', 'dialects/mysql/json.pyi', 'dialects/mysql/mariadb.pyi', 'dialects/mysql/mariadbconnector.pyi', 'dialects/mysql/mysqlconnector.pyi', 'dialects/mysql/mysqldb.pyi', 'dialects/mysql/oursql.pyi', 'dialects/mysql/provision.pyi', 'dialects/mysql/pymysql.pyi', 'dialects/mysql/pyodbc.pyi', 'dialects/mysql/reflection.pyi', 'dialects/mysql/reserved_words.pyi', 'dialects/mysql/types.pyi', 'dialects/oracle/__init__.pyi', 'dialects/oracle/base.pyi', 'dialects/oracle/cx_oracle.pyi', 'dialects/oracle/provision.pyi', 'dialects/postgresql/__init__.pyi', 'dialects/postgresql/array.pyi', 'dialects/postgresql/asyncpg.pyi', 'dialects/postgresql/base.pyi', 'dialects/postgresql/dml.pyi', 'dialects/postgresql/ext.pyi', 'dialects/postgresql/hstore.pyi', 'dialects/postgresql/json.pyi', 'dialects/postgresql/pg8000.pyi', 'dialects/postgresql/provision.pyi', 'dialects/postgresql/psycopg2.pyi', 'dialects/postgresql/psycopg2cffi.pyi', 'dialects/postgresql/pygresql.pyi', 'dialects/postgresql/pypostgresql.pyi', 'dialects/postgresql/ranges.pyi', 'dialects/sqlite/__init__.pyi', 'dialects/sqlite/aiosqlite.pyi', 'dialects/sqlite/base.pyi', 'dialects/sqlite/dml.pyi', 'dialects/sqlite/json.pyi', 'dialects/sqlite/provision.pyi', 'dialects/sqlite/pysqlcipher.pyi', 'dialects/sqlite/pysqlite.pyi', 'dialects/sybase/__init__.pyi', 'dialects/sybase/base.pyi', 'dialects/sybase/mxodbc.pyi', 'dialects/sybase/pyodbc.pyi', 'dialects/sybase/pysybase.pyi', 'engine/__init__.pyi', 'engine/base.pyi', 'engine/characteristics.pyi', 'engine/create.pyi', 'engine/cursor.pyi', 'engine/default.pyi', 'engine/events.pyi', 'engine/interfaces.pyi', 'engine/mock.pyi', 'engine/reflection.pyi', 'engine/result.pyi', 'engine/row.pyi', 'engine/strategies.pyi', 'engine/url.pyi', 'engine/util.pyi', 'event/__init__.pyi', 'event/api.pyi', 'event/attr.pyi', 'event/base.pyi', 'event/legacy.pyi', 'event/registry.pyi', 'events.pyi', 'exc.pyi', 'ext/__init__.pyi', 'ext/associationproxy.pyi', 'ext/asyncio/__init__.pyi', 'ext/asyncio/base.pyi', 'ext/asyncio/engine.pyi', 'ext/asyncio/events.pyi', 'ext/asyncio/exc.pyi', 'ext/asyncio/result.pyi', 'ext/asyncio/scoping.pyi', 'ext/asyncio/session.pyi', 'ext/automap.pyi', 'ext/baked.pyi', 'ext/compiler.pyi', 'ext/declarative/__init__.pyi', 'ext/declarative/extensions.pyi', 'ext/horizontal_shard.pyi', 'ext/hybrid.pyi', 'ext/indexable.pyi', 'ext/instrumentation.pyi', 'ext/mutable.pyi', 'ext/mypy/__init__.pyi', 'ext/mypy/apply.pyi', 'ext/mypy/decl_class.pyi', 'ext/mypy/infer.pyi', 'ext/mypy/names.pyi', 'ext/mypy/plugin.pyi', 'ext/mypy/util.pyi', 'ext/orderinglist.pyi', 'ext/serializer.pyi', 'future/__init__.pyi', 'future/engine.pyi', 'future/orm/__init__.pyi', 'inspection.pyi', 'log.pyi', 'orm/__init__.pyi', 'orm/attributes.pyi', 'orm/base.pyi', 'orm/clsregistry.pyi', 'orm/collections.pyi', 'orm/context.pyi', 'orm/decl_api.pyi', 'orm/decl_base.pyi', 'orm/dependency.pyi', 'orm/descriptor_props.pyi', 'orm/dynamic.pyi', 'orm/evaluator.pyi', 'orm/events.pyi', 'orm/exc.pyi', 'orm/identity.pyi', 'orm/instrumentation.pyi', 'orm/interfaces.pyi', 'orm/loading.pyi', 'orm/mapper.pyi', 'orm/path_registry.pyi', 'orm/persistence.pyi', 'orm/properties.pyi', 'orm/query.pyi', 'orm/relationships.pyi', 'orm/scoping.pyi', 'orm/session.pyi', 'orm/state.pyi', 'orm/strategies.pyi', 'orm/strategy_options.pyi', 'orm/sync.pyi', 'orm/unitofwork.pyi', 'orm/util.pyi', 'pool/__init__.pyi', 'pool/base.pyi', 'pool/dbapi_proxy.pyi', 'pool/events.pyi', 'pool/impl.pyi', 'processors.pyi', 'schema.pyi', 'sql/__init__.pyi', 'sql/annotation.pyi', 'sql/base.pyi', 'sql/coercions.pyi', 'sql/compiler.pyi', 'sql/crud.pyi', 'sql/ddl.pyi', 'sql/default_comparator.pyi', 'sql/dml.pyi', 'sql/elements.pyi', 'sql/events.pyi', 'sql/expression.pyi', 'sql/functions.pyi', 'sql/lambdas.pyi', 'sql/naming.pyi', 'sql/operators.pyi', 'sql/roles.pyi', 'sql/schema.pyi', 'sql/selectable.pyi', 'sql/sqltypes.pyi', 'sql/traversals.pyi', 'sql/type_api.pyi', 'sql/util.pyi', 'sql/visitors.pyi', 'testing/__init__.pyi', 'testing/assertions.pyi', 'testing/assertsql.pyi', 'testing/asyncio.pyi', 'testing/config.pyi', 'testing/engines.pyi', 'testing/entities.pyi', 'testing/exclusions.pyi', 'testing/fixtures.pyi', 'testing/mock.pyi', 'testing/pickleable.pyi', 'testing/plugin/__init__.pyi', 'testing/plugin/bootstrap.pyi', 'testing/plugin/plugin_base.pyi', 'testing/plugin/pytestplugin.pyi', 'testing/plugin/reinvent_fixtures_py2k.pyi', 'testing/profiling.pyi', 'testing/provision.pyi', 'testing/requirements.pyi', 'testing/schema.pyi', 'testing/util.pyi', 'testing/warnings.pyi', 'types.pyi', 'util/__init__.pyi', 'util/_collections.pyi', 'util/_compat_py3k.pyi', 'util/_concurrency_py3k.pyi', 'util/_preloaded.pyi', 'util/compat.pyi', 'util/concurrency.pyi', 'util/deprecations.pyi', 'util/langhelpers.pyi', 'util/queue.pyi', 'util/topological.pyi', 'METADATA.toml']},
```

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/__init__.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/cimmutabledict.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/cimmutabledict.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/connectors/mxodbc.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/connectors/mxodbc.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/connectors/pyodbc.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/connectors/pyodbc.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/databases/__init__.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/databases/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dbapi.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dbapi.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/firebird/__init__.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/firebird/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/firebird/base.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/firebird/base.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/firebird/kinterbasdb.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/firebird/kinterbasdb.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/mssql/__init__.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/mssql/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/mssql/base.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/mssql/base.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/mssql/information_schema.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/mssql/information_schema.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/mssql/mxodbc.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/mssql/mxodbc.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/mssql/pymssql.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/mssql/pymssql.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/mssql/pyodbc.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/mssql/pyodbc.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/mysql/__init__.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/mysql/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/mysql/aiomysql.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/mysql/aiomysql.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/mysql/asyncmy.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/mysql/asyncmy.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/mysql/base.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/mysql/base.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/mysql/cymysql.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/mysql/cymysql.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/mysql/dml.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/mysql/dml.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/mysql/enumerated.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/mysql/enumerated.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/mysql/mariadbconnector.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/mysql/mariadbconnector.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/mysql/mysqlconnector.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/mysql/mysqlconnector.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/mysql/mysqldb.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/mysql/mysqldb.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/mysql/oursql.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/mysql/oursql.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/mysql/pymysql.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/mysql/pymysql.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/mysql/pyodbc.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/mysql/pyodbc.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/mysql/types.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/mysql/types.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/oracle/__init__.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/oracle/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/oracle/base.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/oracle/base.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/oracle/cx_oracle.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/oracle/cx_oracle.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/postgresql/__init__.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/postgresql/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/postgresql/array.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/postgresql/array.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/postgresql/asyncpg.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/postgresql/asyncpg.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/postgresql/base.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/postgresql/base.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/postgresql/dml.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/postgresql/dml.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/postgresql/ext.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/postgresql/ext.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/postgresql/hstore.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/postgresql/hstore.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/postgresql/json.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/postgresql/json.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/postgresql/pg8000.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/postgresql/pg8000.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/postgresql/psycopg2.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/postgresql/psycopg2.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/postgresql/pygresql.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/postgresql/pygresql.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/postgresql/pypostgresql.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/postgresql/pypostgresql.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/postgresql/ranges.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/postgresql/ranges.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/sqlite/__init__.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/sqlite/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/sqlite/aiosqlite.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/sqlite/aiosqlite.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/sqlite/base.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/sqlite/base.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/sqlite/dml.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/sqlite/dml.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/sqlite/pysqlite.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/sqlite/pysqlite.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/sybase/__init__.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/sybase/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/sybase/base.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/sybase/base.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/sybase/pyodbc.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/sybase/pyodbc.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/dialects/sybase/pysybase.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/dialects/sybase/pysybase.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/engine/__init__.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/engine/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/engine/base.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/engine/base.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/engine/characteristics.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/engine/characteristics.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/engine/create.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/engine/create.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/engine/cursor.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/engine/cursor.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/engine/default.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/engine/default.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/engine/events.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/engine/events.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/engine/interfaces.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/engine/interfaces.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/engine/mock.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/engine/mock.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/engine/reflection.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/engine/reflection.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/engine/result.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/engine/result.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/engine/row.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/engine/row.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/engine/url.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/engine/url.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/event/attr.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/event/attr.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/event/base.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/event/base.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/event/registry.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/event/registry.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/exc.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/exc.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/ext/associationproxy.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/ext/associationproxy.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/ext/asyncio/__init__.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/ext/asyncio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/ext/asyncio/engine.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/ext/asyncio/engine.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/ext/asyncio/result.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/ext/asyncio/result.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/ext/asyncio/scoping.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/ext/asyncio/scoping.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/ext/asyncio/session.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/ext/asyncio/session.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/ext/automap.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/ext/automap.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/ext/baked.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/ext/baked.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/ext/declarative/__init__.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/ext/declarative/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/ext/horizontal_shard.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/ext/horizontal_shard.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/ext/hybrid.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/ext/hybrid.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/ext/instrumentation.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/ext/instrumentation.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/ext/mutable.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/ext/mutable.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/ext/mypy/apply.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/ext/mypy/apply.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/ext/mypy/infer.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/ext/mypy/infer.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/ext/mypy/names.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/ext/mypy/names.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/ext/mypy/plugin.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/ext/mypy/plugin.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/ext/mypy/util.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/ext/mypy/util.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/ext/orderinglist.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/ext/orderinglist.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/future/engine.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/future/engine.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/log.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/log.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/orm/__init__.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/orm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/orm/attributes.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/orm/attributes.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/orm/base.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/orm/base.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/orm/clsregistry.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/orm/clsregistry.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/orm/collections.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/orm/collections.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/orm/context.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/orm/context.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/orm/decl_api.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/orm/decl_api.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/orm/decl_base.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/orm/decl_base.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/orm/dependency.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/orm/dependency.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/orm/descriptor_props.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/orm/descriptor_props.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/orm/dynamic.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/orm/dynamic.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/orm/evaluator.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/orm/evaluator.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/orm/events.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/orm/events.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/orm/exc.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/orm/exc.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/orm/identity.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/orm/identity.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/orm/instrumentation.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/orm/instrumentation.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/orm/interfaces.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/orm/interfaces.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/orm/loading.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/orm/loading.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/orm/mapper.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/orm/mapper.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/orm/path_registry.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/orm/path_registry.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/orm/persistence.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/orm/persistence.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/orm/properties.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/orm/properties.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/orm/query.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/orm/query.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/orm/relationships.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/orm/relationships.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/orm/scoping.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/orm/scoping.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/orm/session.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/orm/session.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/orm/state.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/orm/state.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/orm/strategies.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/orm/strategies.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/orm/strategy_options.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/orm/strategy_options.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/orm/unitofwork.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/orm/unitofwork.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/orm/util.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/orm/util.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/pool/__init__.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/pool/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/pool/base.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/pool/base.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/pool/events.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/pool/events.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/pool/impl.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/pool/impl.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/schema.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/schema.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/sql/__init__.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/sql/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/sql/base.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/sql/base.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/sql/coercions.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/sql/coercions.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/sql/compiler.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/sql/compiler.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/sql/ddl.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/sql/ddl.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/sql/dml.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/sql/dml.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/sql/elements.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/sql/elements.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/sql/events.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/sql/events.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/sql/expression.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/sql/expression.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/sql/functions.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/sql/functions.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/sql/lambdas.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/sql/lambdas.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/sql/operators.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/sql/operators.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/sql/roles.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/sql/roles.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/sql/schema.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/sql/schema.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/sql/selectable.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/sql/selectable.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/sql/sqltypes.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/sql/sqltypes.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/sql/traversals.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/sql/traversals.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/sql/type_api.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/sql/type_api.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/sql/util.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/sql/util.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/sql/visitors.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/sql/visitors.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/testing/__init__.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/testing/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/testing/assertions.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/testing/assertions.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/testing/assertsql.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/testing/assertsql.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/testing/config.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/testing/config.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/testing/engines.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/testing/engines.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/testing/exclusions.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/testing/exclusions.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/testing/fixtures.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/testing/fixtures.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/testing/pickleable.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/testing/pickleable.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/testing/plugin/plugin_base.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/testing/plugin/plugin_base.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/testing/plugin/pytestplugin.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/testing/plugin/pytestplugin.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/testing/profiling.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/testing/profiling.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/testing/provision.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/testing/provision.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/testing/requirements.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/testing/requirements.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/testing/util.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/testing/util.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/types.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/types.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/util/__init__.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/util/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/util/_collections.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/util/_collections.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/util/_concurrency_py3k.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/util/_concurrency_py3k.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/util/compat.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/util/compat.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/util/deprecations.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/util/deprecations.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/util/langhelpers.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/util/langhelpers.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
+from _typeshed import Self
 from collections.abc import Callable
 from typing import Any, Generic, TypeVar, overload
 
 from . import compat
 
 _R = TypeVar("_R")
-_T = TypeVar("_T")
 
 def md5_hex(x): ...
 
 class safe_reraise:
     warn_only: Any
     def __init__(self, warn_only: bool = ...) -> None: ...
     def __enter__(self) -> None: ...
@@ -61,30 +61,30 @@
 
 class memoized_property(Generic[_R]):
     fget: Callable[..., _R]
     __doc__: str
     __name__: str
     def __init__(self, fget: Callable[..., _R], doc: str | None = ...) -> None: ...
     @overload
-    def __get__(self: _T, obj: None, cls: object) -> _T: ...
+    def __get__(self: Self, obj: None, cls: object) -> Self: ...
     @overload
     def __get__(self, obj: object, cls: object) -> _R: ...
     @classmethod
     def reset(cls, obj: object, name: str) -> None: ...
 
 def memoized_instancemethod(fn): ...
 
 class HasMemoized:
     class memoized_attribute(Generic[_R]):
         fget: Callable[..., _R]
         __doc__: str
         __name__: str
         def __init__(self, fget: Callable[..., _R], doc: str | None = ...) -> None: ...
         @overload
-        def __get__(self: _T, obj: None, cls: object) -> _T: ...
+        def __get__(self: Self, obj: None, cls: object) -> Self: ...
         @overload
         def __get__(self, obj: object, cls: object) -> _R: ...
     @classmethod
     def memoized_instancemethod(cls, fn): ...
 
 class MemoizedSlots:
     def __getattr__(self, key): ...
@@ -109,15 +109,15 @@
     func: Callable[..., _R]
     clslevel: Callable[..., _R]
     def __init__(self, func: Callable[..., _R]) -> None: ...
     @overload
     def __get__(self, instance: None, owner: Any) -> _R: ...
     @overload
     def __get__(self, instance: object, owner: object) -> _R: ...
-    def classlevel(self: _T, func: Callable[..., _R]) -> _T: ...
+    def classlevel(self: Self, func: Callable[..., _R]) -> Self: ...
 
 class hybridmethod:
     func: Any
     clslevel: Any
     def __init__(self, func) -> None: ...
     def __get__(self, instance, owner): ...
     def classlevel(self, func): ...
```

### Comparing `types-SQLAlchemy-1.4.8/sqlalchemy-stubs/util/queue.pyi` & `types-SQLAlchemy-1.4.9/sqlalchemy-stubs/util/queue.pyi`

 * *Files identical despite different names*

### Comparing `types-SQLAlchemy-1.4.8/types_SQLAlchemy.egg-info/PKG-INFO` & `types-SQLAlchemy-1.4.9/types_SQLAlchemy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-SQLAlchemy
-Version: 1.4.8
+Version: 1.4.9
 Summary: Typing stubs for SQLAlchemy
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Typing :: Stubs Only
 Description-Content-Type: text/markdown
@@ -16,10 +16,10 @@
 that uses `SQLAlchemy`. The source for this package can be found at
 https://github.com/python/typeshed/tree/master/stubs/SQLAlchemy. All fixes for
 types and metadata should be contributed there.
 
 The `sqlalchemy-stubs` package is an alternative to this package and also includes a mypy plugin for more precise types.
 
 See https://github.com/python/typeshed/blob/master/README.md for more details.
-This package was generated from typeshed commit `8f7dd8c381ed5e2334da1d47ca03b7a5f42c4394`.
+This package was generated from typeshed commit `96c9abb0585bb052bbb36228aa616857b987867b`.
```

### Comparing `types-SQLAlchemy-1.4.8/types_SQLAlchemy.egg-info/SOURCES.txt` & `types-SQLAlchemy-1.4.9/types_SQLAlchemy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

