# Comparing `tmp/cdktf-cdktf-provider-databricks-5.0.8.tar.gz` & `tmp/cdktf-cdktf-provider-databricks-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdktf-cdktf-provider-databricks-5.0.8.tar", last modified: Fri Apr  7 03:19:31 2023, max compression
+gzip compressed data, was "cdktf-cdktf-provider-databricks-6.0.0.tar", last modified: Sat Apr 15 03:18:53 2023, max compression
```

## Comparing `cdktf-cdktf-provider-databricks-5.0.8.tar` & `cdktf-cdktf-provider-databricks-6.0.0.tar`

### file list

```diff
@@ -1,229 +1,229 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.331717 cdktf-cdktf-provider-databricks-5.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-04-07 03:19:31.331717 cdktf-cdktf-provider-databricks-5.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 03:19:31.331717 cdktf-cdktf-provider-databricks-5.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.275717 cdktf-cdktf-provider-databricks-5.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.291717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/
--rw-r--r--   0 runner    (1001) docker     (123)     9579 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.291717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  6039773 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/_jsii/provider-databricks@5.0.8.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.299717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/aws_s3_mount/
--rw-r--r--   0 runner    (1001) docker     (123)    24254 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/aws_s3_mount/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.299717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/azure_adls_gen1_mount/
--rw-r--r--   0 runner    (1001) docker     (123)    35878 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/azure_adls_gen1_mount/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.299717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/azure_adls_gen2_mount/
--rw-r--r--   0 runner    (1001) docker     (123)    38516 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/azure_adls_gen2_mount/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.299717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/azure_blob_mount/
--rw-r--r--   0 runner    (1001) docker     (123)    33065 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/azure_blob_mount/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.303717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/catalog/
--rw-r--r--   0 runner    (1001) docker     (123)    35891 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/catalog/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.303717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/cluster/
--rw-r--r--   0 runner    (1001) docker     (123)   357225 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/cluster/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.303717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/cluster_policy/
--rw-r--r--   0 runner    (1001) docker     (123)    22833 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/cluster_policy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.303717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_aws_assume_role_policy/
--rw-r--r--   0 runner    (1001) docker     (123)    24085 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_aws_assume_role_policy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.303717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_aws_bucket_policy/
--rw-r--r--   0 runner    (1001) docker     (123)    25724 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_aws_bucket_policy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.303717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_aws_crossaccount_policy/
--rw-r--r--   0 runner    (1001) docker     (123)    18349 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_aws_crossaccount_policy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.303717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_catalogs/
--rw-r--r--   0 runner    (1001) docker     (123)    17542 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_catalogs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.303717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_cluster/
--rw-r--r--   0 runner    (1001) docker     (123)   384767 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_cluster/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.303717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_cluster_policy/
--rw-r--r--   0 runner    (1001) docker     (123)    22586 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_cluster_policy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.303717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_clusters/
--rw-r--r--   0 runner    (1001) docker     (123)    18185 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_clusters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.303717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_current_user/
--rw-r--r--   0 runner    (1001) docker     (123)    16447 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_current_user/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.303717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_dbfs_file/
--rw-r--r--   0 runner    (1001) docker     (123)    20312 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_dbfs_file/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.303717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_dbfs_file_paths/
--rw-r--r--   0 runner    (1001) docker     (123)    29342 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_dbfs_file_paths/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.307717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_directory/
--rw-r--r--   0 runner    (1001) docker     (123)    19448 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_directory/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.307717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_group/
--rw-r--r--   0 runner    (1001) docker     (123)    50331 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_group/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.307717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_instance_pool/
--rw-r--r--   0 runner    (1001) docker     (123)   209139 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_instance_pool/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.307717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_job/
--rw-r--r--   0 runner    (1001) docker     (123)  1532766 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_job/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.307717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_jobs/
--rw-r--r--   0 runner    (1001) docker     (123)    17614 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_jobs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.307717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_mws_credentials/
--rw-r--r--   0 runner    (1001) docker     (123)    17917 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_mws_credentials/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.307717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_mws_workspaces/
--rw-r--r--   0 runner    (1001) docker     (123)    17876 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_mws_workspaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.307717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_node_type/
--rw-r--r--   0 runner    (1001) docker     (123)    50782 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_node_type/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.311717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_notebook/
--rw-r--r--   0 runner    (1001) docker     (123)    26038 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_notebook/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.311717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_notebook_paths/
--rw-r--r--   0 runner    (1001) docker     (123)    29511 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_notebook_paths/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.311717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_schemas/
--rw-r--r--   0 runner    (1001) docker     (123)    19612 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_schemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.311717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_service_principal/
--rw-r--r--   0 runner    (1001) docker     (123)    32042 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_service_principal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.311717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_service_principals/
--rw-r--r--   0 runner    (1001) docker     (123)    20975 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_service_principals/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.311717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_share/
--rw-r--r--   0 runner    (1001) docker     (123)    89715 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_share/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.311717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_shares/
--rw-r--r--   0 runner    (1001) docker     (123)    17592 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_shares/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.311717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_spark_version/
--rw-r--r--   0 runner    (1001) docker     (123)    42307 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_spark_version/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.311717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_sql_warehouse/
--rw-r--r--   0 runner    (1001) docker     (123)    95234 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_sql_warehouse/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.311717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_sql_warehouses/
--rw-r--r--   0 runner    (1001) docker     (123)    20483 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_sql_warehouses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.311717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_tables/
--rw-r--r--   0 runner    (1001) docker     (123)    21628 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_tables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.311717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_user/
--rw-r--r--   0 runner    (1001) docker     (123)    20676 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_user/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.311717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_views/
--rw-r--r--   0 runner    (1001) docker     (123)    21587 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_views/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.311717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_zones/
--rw-r--r--   0 runner    (1001) docker     (123)    15626 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_zones/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.311717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/dbfs_file/
--rw-r--r--   0 runner    (1001) docker     (123)    23806 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/dbfs_file/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.311717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/directory/
--rw-r--r--   0 runner    (1001) docker     (123)    22233 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/directory/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.311717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/entitlements/
--rw-r--r--   0 runner    (1001) docker     (123)    35195 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/entitlements/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.311717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/external_location/
--rw-r--r--   0 runner    (1001) docker     (123)    30967 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/external_location/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.315717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/git_credential/
--rw-r--r--   0 runner    (1001) docker     (123)    25060 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/git_credential/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.315717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/global_init_script/
--rw-r--r--   0 runner    (1001) docker     (123)    34382 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/global_init_script/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.315717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/grants/
--rw-r--r--   0 runner    (1001) docker     (123)    53837 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/grants/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.315717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/group/
--rw-r--r--   0 runner    (1001) docker     (123)    36814 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/group/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.315717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/group_instance_profile/
--rw-r--r--   0 runner    (1001) docker     (123)    19789 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/group_instance_profile/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.315717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/group_member/
--rw-r--r--   0 runner    (1001) docker     (123)    19134 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/group_member/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.315717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/group_role/
--rw-r--r--   0 runner    (1001) docker     (123)    18905 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/group_role/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.315717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/instance_pool/
--rw-r--r--   0 runner    (1001) docker     (123)   167466 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/instance_pool/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.315717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/instance_profile/
--rw-r--r--   0 runner    (1001) docker     (123)    26467 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/instance_profile/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.315717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/ip_access_list/
--rw-r--r--   0 runner    (1001) docker     (123)    24107 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/ip_access_list/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.315717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/job/
--rw-r--r--   0 runner    (1001) docker     (123)  1420468 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/job/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.319717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/library/
--rw-r--r--   0 runner    (1001) docker     (123)    52725 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/library/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.319717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/metastore/
--rw-r--r--   0 runner    (1001) docker     (123)    51945 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/metastore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.319717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/metastore_assignment/
--rw-r--r--   0 runner    (1001) docker     (123)    22302 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/metastore_assignment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.319717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/metastore_data_access/
--rw-r--r--   0 runner    (1001) docker     (123)    77354 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/metastore_data_access/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.319717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/mlflow_experiment/
--rw-r--r--   0 runner    (1001) docker     (123)    37357 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/mlflow_experiment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.319717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/mlflow_model/
--rw-r--r--   0 runner    (1001) docker     (123)    45757 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/mlflow_model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.319717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/mlflow_webhook/
--rw-r--r--   0 runner    (1001) docker     (123)    51339 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/mlflow_webhook/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.319717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/model_serving/
--rw-r--r--   0 runner    (1001) docker     (123)    79930 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/model_serving/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.319717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/mount/
--rw-r--r--   0 runner    (1001) docker     (123)   117718 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/mount/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.323717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/mws_credentials/
--rw-r--r--   0 runner    (1001) docker     (123)    22047 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/mws_credentials/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.323717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/mws_customer_managed_keys/
--rw-r--r--   0 runner    (1001) docker     (123)    45574 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/mws_customer_managed_keys/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.323717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/mws_log_delivery/
--rw-r--r--   0 runner    (1001) docker     (123)    40849 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/mws_log_delivery/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.323717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/mws_networks/
--rw-r--r--   0 runner    (1001) docker     (123)    82705 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/mws_networks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.323717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/mws_permission_assignment/
--rw-r--r--   0 runner    (1001) docker     (123)    22072 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/mws_permission_assignment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.323717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/mws_private_access_settings/
--rw-r--r--   0 runner    (1001) docker     (123)    36729 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/mws_private_access_settings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.323717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/mws_storage_configurations/
--rw-r--r--   0 runner    (1001) docker     (123)    22748 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/mws_storage_configurations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.323717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/mws_vpc_endpoint/
--rw-r--r--   0 runner    (1001) docker     (123)    54558 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/mws_vpc_endpoint/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.323717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/mws_workspaces/
--rw-r--r--   0 runner    (1001) docker     (123)   144297 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/mws_workspaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.323717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/notebook/
--rw-r--r--   0 runner    (1001) docker     (123)    32377 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/notebook/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.323717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/obo_token/
--rw-r--r--   0 runner    (1001) docker     (123)    22054 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/obo_token/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.323717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/permission_assignment/
--rw-r--r--   0 runner    (1001) docker     (123)    19813 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/permission_assignment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.323717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/permissions/
--rw-r--r--   0 runner    (1001) docker     (123)    81680 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/permissions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.323717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)   304424 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/pipeline/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.327717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/provider/
--rw-r--r--   0 runner    (1001) docker     (123)    73500 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/provider/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.327717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/provider_resource/
--rw-r--r--   0 runner    (1001) docker     (123)    23910 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/provider_resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.327717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/recipient/
--rw-r--r--   0 runner    (1001) docker     (123)    62700 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/recipient/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.327717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/repo/
--rw-r--r--   0 runner    (1001) docker     (123)    35181 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/repo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.327717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/schema/
--rw-r--r--   0 runner    (1001) docker     (123)    33276 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/schema/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.327717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/secret/
--rw-r--r--   0 runner    (1001) docker     (123)    21109 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/secret/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.327717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/secret_acl/
--rw-r--r--   0 runner    (1001) docker     (123)    20987 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/secret_acl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.327717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/secret_scope/
--rw-r--r--   0 runner    (1001) docker     (123)    32167 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/secret_scope/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.327717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/service_principal/
--rw-r--r--   0 runner    (1001) docker     (123)    51686 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/service_principal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.327717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/service_principal_role/
--rw-r--r--   0 runner    (1001) docker     (123)    19696 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/service_principal_role/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.327717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/service_principal_secret/
--rw-r--r--   0 runner    (1001) docker     (123)    22284 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/service_principal_secret/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.327717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/share/
--rw-r--r--   0 runner    (1001) docker     (123)    87207 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/share/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.327717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/sql_alert/
--rw-r--r--   0 runner    (1001) docker     (123)    40760 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/sql_alert/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.327717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/sql_dashboard/
--rw-r--r--   0 runner    (1001) docker     (123)    21439 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/sql_dashboard/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.327717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/sql_endpoint/
--rw-r--r--   0 runner    (1001) docker     (123)   102154 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/sql_endpoint/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.327717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/sql_global_config/
--rw-r--r--   0 runner    (1001) docker     (123)    29798 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/sql_global_config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.331717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/sql_permissions/
--rw-r--r--   0 runner    (1001) docker     (123)    50953 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/sql_permissions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.331717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/sql_query/
--rw-r--r--   0 runner    (1001) docker     (123)   217440 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/sql_query/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.331717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/sql_visualization/
--rw-r--r--   0 runner    (1001) docker     (123)    30100 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/sql_visualization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.331717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/sql_widget/
--rw-r--r--   0 runner    (1001) docker     (123)    68587 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/sql_widget/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.331717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/storage_credential/
--rw-r--r--   0 runner    (1001) docker     (123)    75858 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/storage_credential/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.331717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/table/
--rw-r--r--   0 runner    (1001) docker     (123)    73312 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/table/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.331717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/token/
--rw-r--r--   0 runner    (1001) docker     (123)    26539 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/token/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.331717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/user/
--rw-r--r--   0 runner    (1001) docker     (123)    49997 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/user/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.331717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/user_instance_profile/
--rw-r--r--   0 runner    (1001) docker     (123)    19721 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/user_instance_profile/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.331717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/user_role/
--rw-r--r--   0 runner    (1001) docker     (123)    18837 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/user_role/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.331717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/workspace_conf/
--rw-r--r--   0 runner    (1001) docker     (123)    18031 2023-04-07 03:19:13.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/workspace_conf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 03:19:31.291717 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-04-07 03:19:31.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7468 2023-04-07 03:19:31.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 03:19:31.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-07 03:19:31.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-07 03:19:31.000000 cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.164949 cdktf-cdktf-provider-databricks-6.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-04-15 03:18:53.164949 cdktf-cdktf-provider-databricks-6.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 03:18:53.164949 cdktf-cdktf-provider-databricks-6.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.132949 cdktf-cdktf-provider-databricks-6.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.140949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/
+-rw-r--r--   0 runner    (1001) docker     (123)     9579 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.140949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  5965234 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/_jsii/provider-databricks@6.0.0.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.144949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/aws_s3_mount/
+-rw-r--r--   0 runner    (1001) docker     (123)    24254 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/aws_s3_mount/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.148949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/azure_adls_gen1_mount/
+-rw-r--r--   0 runner    (1001) docker     (123)    35878 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/azure_adls_gen1_mount/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.148949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/azure_adls_gen2_mount/
+-rw-r--r--   0 runner    (1001) docker     (123)    38516 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/azure_adls_gen2_mount/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.148949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/azure_blob_mount/
+-rw-r--r--   0 runner    (1001) docker     (123)    33065 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/azure_blob_mount/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.148949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)    35891 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/catalog/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.148949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)   357225 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/cluster/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.148949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/cluster_policy/
+-rw-r--r--   0 runner    (1001) docker     (123)    22833 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/cluster_policy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.148949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_aws_assume_role_policy/
+-rw-r--r--   0 runner    (1001) docker     (123)    24085 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_aws_assume_role_policy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.148949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_aws_bucket_policy/
+-rw-r--r--   0 runner    (1001) docker     (123)    25724 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_aws_bucket_policy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.148949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_aws_crossaccount_policy/
+-rw-r--r--   0 runner    (1001) docker     (123)    18349 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_aws_crossaccount_policy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.148949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_catalogs/
+-rw-r--r--   0 runner    (1001) docker     (123)    17542 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_catalogs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.148949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)   384767 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_cluster/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.148949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_cluster_policy/
+-rw-r--r--   0 runner    (1001) docker     (123)    22586 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_cluster_policy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.148949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_clusters/
+-rw-r--r--   0 runner    (1001) docker     (123)    18185 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_clusters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.148949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_current_user/
+-rw-r--r--   0 runner    (1001) docker     (123)    16447 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_current_user/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.148949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_dbfs_file/
+-rw-r--r--   0 runner    (1001) docker     (123)    20312 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_dbfs_file/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.148949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_dbfs_file_paths/
+-rw-r--r--   0 runner    (1001) docker     (123)    29342 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_dbfs_file_paths/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.148949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_directory/
+-rw-r--r--   0 runner    (1001) docker     (123)    19448 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_directory/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.148949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_group/
+-rw-r--r--   0 runner    (1001) docker     (123)    50331 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_group/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.148949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_instance_pool/
+-rw-r--r--   0 runner    (1001) docker     (123)   209139 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_instance_pool/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.148949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_job/
+-rw-r--r--   0 runner    (1001) docker     (123)  1532766 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_job/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.152949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)    17614 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_jobs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.152949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_mws_credentials/
+-rw-r--r--   0 runner    (1001) docker     (123)    17917 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_mws_credentials/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.152949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_mws_workspaces/
+-rw-r--r--   0 runner    (1001) docker     (123)    17876 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_mws_workspaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.152949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_node_type/
+-rw-r--r--   0 runner    (1001) docker     (123)    50782 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_node_type/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.152949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_notebook/
+-rw-r--r--   0 runner    (1001) docker     (123)    26038 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_notebook/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.152949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_notebook_paths/
+-rw-r--r--   0 runner    (1001) docker     (123)    29511 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_notebook_paths/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.152949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)    19612 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_schemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.152949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_service_principal/
+-rw-r--r--   0 runner    (1001) docker     (123)    32042 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_service_principal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.152949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_service_principals/
+-rw-r--r--   0 runner    (1001) docker     (123)    20975 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_service_principals/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.152949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_share/
+-rw-r--r--   0 runner    (1001) docker     (123)    89715 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_share/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.152949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_shares/
+-rw-r--r--   0 runner    (1001) docker     (123)    17592 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_shares/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.152949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_spark_version/
+-rw-r--r--   0 runner    (1001) docker     (123)    42307 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_spark_version/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.152949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_sql_warehouse/
+-rw-r--r--   0 runner    (1001) docker     (123)    95234 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_sql_warehouse/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.152949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_sql_warehouses/
+-rw-r--r--   0 runner    (1001) docker     (123)    20483 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_sql_warehouses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.152949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_tables/
+-rw-r--r--   0 runner    (1001) docker     (123)    21628 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_tables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.152949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_user/
+-rw-r--r--   0 runner    (1001) docker     (123)    20676 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_user/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.152949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_views/
+-rw-r--r--   0 runner    (1001) docker     (123)    21587 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_views/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.152949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_zones/
+-rw-r--r--   0 runner    (1001) docker     (123)    15626 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_zones/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.152949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/dbfs_file/
+-rw-r--r--   0 runner    (1001) docker     (123)    23806 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/dbfs_file/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.152949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/directory/
+-rw-r--r--   0 runner    (1001) docker     (123)    22233 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/directory/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.152949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/entitlements/
+-rw-r--r--   0 runner    (1001) docker     (123)    35195 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/entitlements/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.156949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/external_location/
+-rw-r--r--   0 runner    (1001) docker     (123)    30967 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/external_location/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.156949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/git_credential/
+-rw-r--r--   0 runner    (1001) docker     (123)    25060 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/git_credential/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.156949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/global_init_script/
+-rw-r--r--   0 runner    (1001) docker     (123)    34382 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/global_init_script/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.156949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/grants/
+-rw-r--r--   0 runner    (1001) docker     (123)    53837 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/grants/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.156949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/group/
+-rw-r--r--   0 runner    (1001) docker     (123)    36814 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/group/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.156949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/group_instance_profile/
+-rw-r--r--   0 runner    (1001) docker     (123)    19789 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/group_instance_profile/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.156949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/group_member/
+-rw-r--r--   0 runner    (1001) docker     (123)    19134 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/group_member/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.156949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/group_role/
+-rw-r--r--   0 runner    (1001) docker     (123)    18905 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/group_role/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.156949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/instance_pool/
+-rw-r--r--   0 runner    (1001) docker     (123)   167466 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/instance_pool/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.156949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/instance_profile/
+-rw-r--r--   0 runner    (1001) docker     (123)    26467 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/instance_profile/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.156949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/ip_access_list/
+-rw-r--r--   0 runner    (1001) docker     (123)    24107 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/ip_access_list/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.156949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/job/
+-rw-r--r--   0 runner    (1001) docker     (123)  1420468 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/job/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.156949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/library/
+-rw-r--r--   0 runner    (1001) docker     (123)    52725 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/library/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.156949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/metastore/
+-rw-r--r--   0 runner    (1001) docker     (123)    51945 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/metastore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.156949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/metastore_assignment/
+-rw-r--r--   0 runner    (1001) docker     (123)    22302 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/metastore_assignment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.156949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/metastore_data_access/
+-rw-r--r--   0 runner    (1001) docker     (123)    77354 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/metastore_data_access/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.156949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/mlflow_experiment/
+-rw-r--r--   0 runner    (1001) docker     (123)    37357 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/mlflow_experiment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.160949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/mlflow_model/
+-rw-r--r--   0 runner    (1001) docker     (123)    45757 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/mlflow_model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.160949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/mlflow_webhook/
+-rw-r--r--   0 runner    (1001) docker     (123)    51339 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/mlflow_webhook/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.160949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/model_serving/
+-rw-r--r--   0 runner    (1001) docker     (123)    79930 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/model_serving/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.160949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/mount/
+-rw-r--r--   0 runner    (1001) docker     (123)   117718 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/mount/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.160949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/mws_credentials/
+-rw-r--r--   0 runner    (1001) docker     (123)    22047 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/mws_credentials/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.160949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/mws_customer_managed_keys/
+-rw-r--r--   0 runner    (1001) docker     (123)    45574 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/mws_customer_managed_keys/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.160949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/mws_log_delivery/
+-rw-r--r--   0 runner    (1001) docker     (123)    40849 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/mws_log_delivery/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.160949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/mws_networks/
+-rw-r--r--   0 runner    (1001) docker     (123)    82705 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/mws_networks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.160949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/mws_permission_assignment/
+-rw-r--r--   0 runner    (1001) docker     (123)    22072 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/mws_permission_assignment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.160949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/mws_private_access_settings/
+-rw-r--r--   0 runner    (1001) docker     (123)    36729 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/mws_private_access_settings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.160949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/mws_storage_configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)    22748 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/mws_storage_configurations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.160949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/mws_vpc_endpoint/
+-rw-r--r--   0 runner    (1001) docker     (123)    54558 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/mws_vpc_endpoint/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.160949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/mws_workspaces/
+-rw-r--r--   0 runner    (1001) docker     (123)   144297 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/mws_workspaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.160949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/notebook/
+-rw-r--r--   0 runner    (1001) docker     (123)    32377 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/notebook/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.160949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/obo_token/
+-rw-r--r--   0 runner    (1001) docker     (123)    22054 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/obo_token/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.160949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/permission_assignment/
+-rw-r--r--   0 runner    (1001) docker     (123)    19813 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/permission_assignment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.160949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/permissions/
+-rw-r--r--   0 runner    (1001) docker     (123)    81680 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/permissions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.160949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)   321951 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/pipeline/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.160949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)    73500 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/provider/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.160949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/provider_resource/
+-rw-r--r--   0 runner    (1001) docker     (123)    23910 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/provider_resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.160949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/recipient/
+-rw-r--r--   0 runner    (1001) docker     (123)    62700 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/recipient/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.160949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/repo/
+-rw-r--r--   0 runner    (1001) docker     (123)    35181 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/repo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.160949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)    33276 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/schema/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.164949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/secret/
+-rw-r--r--   0 runner    (1001) docker     (123)    21109 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/secret/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.164949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/secret_acl/
+-rw-r--r--   0 runner    (1001) docker     (123)    20987 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/secret_acl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.164949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/secret_scope/
+-rw-r--r--   0 runner    (1001) docker     (123)    32167 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/secret_scope/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.164949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/service_principal/
+-rw-r--r--   0 runner    (1001) docker     (123)    51686 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/service_principal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.164949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/service_principal_role/
+-rw-r--r--   0 runner    (1001) docker     (123)    19696 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/service_principal_role/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.164949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/service_principal_secret/
+-rw-r--r--   0 runner    (1001) docker     (123)    22284 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/service_principal_secret/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.164949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/share/
+-rw-r--r--   0 runner    (1001) docker     (123)    87207 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/share/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.164949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/sql_alert/
+-rw-r--r--   0 runner    (1001) docker     (123)    40760 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/sql_alert/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.164949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/sql_dashboard/
+-rw-r--r--   0 runner    (1001) docker     (123)    21439 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/sql_dashboard/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.164949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/sql_endpoint/
+-rw-r--r--   0 runner    (1001) docker     (123)   102154 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/sql_endpoint/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.164949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/sql_global_config/
+-rw-r--r--   0 runner    (1001) docker     (123)    29798 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/sql_global_config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.164949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/sql_permissions/
+-rw-r--r--   0 runner    (1001) docker     (123)    50953 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/sql_permissions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.164949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/sql_query/
+-rw-r--r--   0 runner    (1001) docker     (123)   217440 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/sql_query/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.164949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/sql_visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)    30100 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/sql_visualization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.164949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/sql_widget/
+-rw-r--r--   0 runner    (1001) docker     (123)    68587 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/sql_widget/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.164949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/storage_credential/
+-rw-r--r--   0 runner    (1001) docker     (123)    75858 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/storage_credential/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.164949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/table/
+-rw-r--r--   0 runner    (1001) docker     (123)    73312 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/table/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.164949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/token/
+-rw-r--r--   0 runner    (1001) docker     (123)    26539 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/token/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.164949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/user/
+-rw-r--r--   0 runner    (1001) docker     (123)    49997 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/user/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.164949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/user_instance_profile/
+-rw-r--r--   0 runner    (1001) docker     (123)    19721 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/user_instance_profile/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.164949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/user_role/
+-rw-r--r--   0 runner    (1001) docker     (123)    18837 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/user_role/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.164949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/workspace_conf/
+-rw-r--r--   0 runner    (1001) docker     (123)    18031 2023-04-15 03:18:41.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/workspace_conf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:53.140949 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-04-15 03:18:53.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7468 2023-04-15 03:18:53.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 03:18:53.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-15 03:18:53.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-15 03:18:53.000000 cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks.egg-info/top_level.txt
```

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/LICENSE` & `cdktf-cdktf-provider-databricks-6.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/PKG-INFO` & `cdktf-cdktf-provider-databricks-6.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-databricks
-Version: 5.0.8
+Version: 6.0.0
 Summary: Prebuilt databricks Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-databricks.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-databricks.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/README.md` & `cdktf-cdktf-provider-databricks-6.0.0/README.md`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/setup.py` & `cdktf-cdktf-provider-databricks-6.0.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdktf-cdktf-provider-databricks",
-    "version": "5.0.8",
+    "version": "6.0.0",
     "description": "Prebuilt databricks Provider for Terraform CDK (cdktf)",
     "license": "MPL-2.0",
     "url": "https://github.com/cdktf/cdktf-provider-databricks.git",
     "long_description_content_type": "text/markdown",
     "author": "HashiCorp",
     "bdist_wheel": {
         "universal": true
@@ -126,25 +126,25 @@
         "cdktf_cdktf_provider_databricks.user",
         "cdktf_cdktf_provider_databricks.user_instance_profile",
         "cdktf_cdktf_provider_databricks.user_role",
         "cdktf_cdktf_provider_databricks.workspace_conf"
     ],
     "package_data": {
         "cdktf_cdktf_provider_databricks._jsii": [
-            "provider-databricks@5.0.8.jsii.tgz"
+            "provider-databricks@6.0.0.jsii.tgz"
         ],
         "cdktf_cdktf_provider_databricks": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
         "cdktf>=0.15.0, <0.16.0",
         "constructs>=10.0.0, <11.0.0",
-        "jsii>=1.79.0, <2.0.0",
+        "jsii>=1.80.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/aws_s3_mount/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/aws_s3_mount/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/azure_adls_gen1_mount/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/azure_adls_gen1_mount/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/azure_adls_gen2_mount/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/azure_adls_gen2_mount/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/azure_blob_mount/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/azure_blob_mount/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/catalog/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/cluster/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/cluster_policy/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/cluster_policy/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_aws_assume_role_policy/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_aws_assume_role_policy/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_aws_bucket_policy/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_aws_bucket_policy/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_aws_crossaccount_policy/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_aws_crossaccount_policy/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_catalogs/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_catalogs/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_cluster/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_cluster_policy/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_cluster_policy/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_clusters/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_clusters/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_current_user/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_current_user/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_dbfs_file/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_dbfs_file/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_dbfs_file_paths/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_dbfs_file_paths/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_directory/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_directory/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_group/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_group/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_instance_pool/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_instance_pool/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_job/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_job/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_jobs/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_jobs/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_mws_credentials/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_mws_credentials/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_mws_workspaces/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_mws_workspaces/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_node_type/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_node_type/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_notebook/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_notebook/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_notebook_paths/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_notebook_paths/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_schemas/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_service_principal/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_service_principal/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_service_principals/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_service_principals/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_share/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_share/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_shares/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_shares/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_spark_version/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_spark_version/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_sql_warehouse/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_sql_warehouse/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_sql_warehouses/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_sql_warehouses/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_tables/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_tables/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_user/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_user/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_views/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_views/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/data_databricks_zones/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_zones/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/dbfs_file/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/dbfs_file/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/directory/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/directory/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/entitlements/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/entitlements/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/external_location/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/external_location/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/git_credential/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/git_credential/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/global_init_script/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/global_init_script/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/grants/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/grants/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/group/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/group/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/group_instance_profile/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/group_instance_profile/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/group_member/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/group_member/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/group_role/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/group_role/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/instance_pool/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/instance_pool/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/instance_profile/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/instance_profile/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/ip_access_list/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/ip_access_list/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/job/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/job/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/library/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/library/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/metastore/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/metastore/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/metastore_assignment/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/metastore_assignment/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/metastore_data_access/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/metastore_data_access/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/mlflow_experiment/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/mlflow_experiment/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/mlflow_model/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/mlflow_model/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/mlflow_webhook/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/mlflow_webhook/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/model_serving/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/model_serving/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/mount/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/mount/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/mws_credentials/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/mws_credentials/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/mws_customer_managed_keys/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/mws_customer_managed_keys/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/mws_log_delivery/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/mws_log_delivery/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/mws_networks/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/mws_networks/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/mws_permission_assignment/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/mws_permission_assignment/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/mws_private_access_settings/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/mws_private_access_settings/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/mws_storage_configurations/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/mws_storage_configurations/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/mws_vpc_endpoint/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/mws_vpc_endpoint/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/mws_workspaces/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/mws_workspaces/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/notebook/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/notebook/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/obo_token/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/obo_token/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/permission_assignment/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/permission_assignment/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/permissions/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/permissions/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/pipeline/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/pipeline/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,15 @@
         continuous: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         development: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         edition: typing.Optional[builtins.str] = None,
         filters: typing.Optional[typing.Union["PipelineFilters", typing.Dict[builtins.str, typing.Any]]] = None,
         id: typing.Optional[builtins.str] = None,
         library: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union["PipelineLibrary", typing.Dict[builtins.str, typing.Any]]]]] = None,
         name: typing.Optional[builtins.str] = None,
+        notification: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union["PipelineNotification", typing.Dict[builtins.str, typing.Any]]]]] = None,
         photon: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         storage: typing.Optional[builtins.str] = None,
         target: typing.Optional[builtins.str] = None,
         timeouts: typing.Optional[typing.Union["PipelineTimeouts", typing.Dict[builtins.str, typing.Any]]] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
         count: typing.Optional[jsii.Number] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
@@ -69,14 +70,15 @@
         :param continuous: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/databricks/r/pipeline#continuous Pipeline#continuous}.
         :param development: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/databricks/r/pipeline#development Pipeline#development}.
         :param edition: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/databricks/r/pipeline#edition Pipeline#edition}.
         :param filters: filters block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/databricks/r/pipeline#filters Pipeline#filters}
         :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/databricks/r/pipeline#id Pipeline#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         :param library: library block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/databricks/r/pipeline#library Pipeline#library}
         :param name: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/databricks/r/pipeline#name Pipeline#name}.
+        :param notification: notification block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/databricks/r/pipeline#notification Pipeline#notification}
         :param photon: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/databricks/r/pipeline#photon Pipeline#photon}.
         :param storage: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/databricks/r/pipeline#storage Pipeline#storage}.
         :param target: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/databricks/r/pipeline#target Pipeline#target}.
         :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/databricks/r/pipeline#timeouts Pipeline#timeouts}
         :param connection: 
         :param count: 
         :param depends_on: 
@@ -98,14 +100,15 @@
             continuous=continuous,
             development=development,
             edition=edition,
             filters=filters,
             id=id,
             library=library,
             name=name,
+            notification=notification,
             photon=photon,
             storage=storage,
             target=target,
             timeouts=timeouts,
             connection=connection,
             count=count,
             depends_on=depends_on,
@@ -154,14 +157,27 @@
         :param value: -
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__718051e6297cf70b4433c1dc18d1514e18bda33aa43b59951fed173deee71445)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         return typing.cast(None, jsii.invoke(self, "putLibrary", [value]))
 
+    @jsii.member(jsii_name="putNotification")
+    def put_notification(
+        self,
+        value: typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union["PipelineNotification", typing.Dict[builtins.str, typing.Any]]]],
+    ) -> None:
+        '''
+        :param value: -
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__aae2ffd87d23f97fff4978ba983ffa8f06b698de24c0d629ea578a2e012f2840)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        return typing.cast(None, jsii.invoke(self, "putNotification", [value]))
+
     @jsii.member(jsii_name="putTimeouts")
     def put_timeouts(self, *, default: typing.Optional[builtins.str] = None) -> None:
         '''
         :param default: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/databricks/r/pipeline#default Pipeline#default}.
         '''
         value = PipelineTimeouts(default=default)
 
@@ -211,14 +227,18 @@
     def reset_library(self) -> None:
         return typing.cast(None, jsii.invoke(self, "resetLibrary", []))
 
     @jsii.member(jsii_name="resetName")
     def reset_name(self) -> None:
         return typing.cast(None, jsii.invoke(self, "resetName", []))
 
+    @jsii.member(jsii_name="resetNotification")
+    def reset_notification(self) -> None:
+        return typing.cast(None, jsii.invoke(self, "resetNotification", []))
+
     @jsii.member(jsii_name="resetPhoton")
     def reset_photon(self) -> None:
         return typing.cast(None, jsii.invoke(self, "resetPhoton", []))
 
     @jsii.member(jsii_name="resetStorage")
     def reset_storage(self) -> None:
         return typing.cast(None, jsii.invoke(self, "resetStorage", []))
@@ -252,14 +272,19 @@
 
     @builtins.property
     @jsii.member(jsii_name="library")
     def library(self) -> "PipelineLibraryList":
         return typing.cast("PipelineLibraryList", jsii.get(self, "library"))
 
     @builtins.property
+    @jsii.member(jsii_name="notification")
+    def notification(self) -> "PipelineNotificationList":
+        return typing.cast("PipelineNotificationList", jsii.get(self, "notification"))
+
+    @builtins.property
     @jsii.member(jsii_name="timeouts")
     def timeouts(self) -> "PipelineTimeoutsOutputReference":
         return typing.cast("PipelineTimeoutsOutputReference", jsii.get(self, "timeouts"))
 
     @builtins.property
     @jsii.member(jsii_name="url")
     def url(self) -> builtins.str:
@@ -334,14 +359,21 @@
 
     @builtins.property
     @jsii.member(jsii_name="nameInput")
     def name_input(self) -> typing.Optional[builtins.str]:
         return typing.cast(typing.Optional[builtins.str], jsii.get(self, "nameInput"))
 
     @builtins.property
+    @jsii.member(jsii_name="notificationInput")
+    def notification_input(
+        self,
+    ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["PipelineNotification"]]]:
+        return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["PipelineNotification"]]], jsii.get(self, "notificationInput"))
+
+    @builtins.property
     @jsii.member(jsii_name="photonInput")
     def photon_input(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], jsii.get(self, "photonInput"))
 
     @builtins.property
@@ -3901,14 +3933,15 @@
         "continuous": "continuous",
         "development": "development",
         "edition": "edition",
         "filters": "filters",
         "id": "id",
         "library": "library",
         "name": "name",
+        "notification": "notification",
         "photon": "photon",
         "storage": "storage",
         "target": "target",
         "timeouts": "timeouts",
     },
 )
 class PipelineConfig(_cdktf_9a9027ec.TerraformMetaArguments):
@@ -3930,14 +3963,15 @@
         continuous: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         development: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         edition: typing.Optional[builtins.str] = None,
         filters: typing.Optional[typing.Union["PipelineFilters", typing.Dict[builtins.str, typing.Any]]] = None,
         id: typing.Optional[builtins.str] = None,
         library: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union["PipelineLibrary", typing.Dict[builtins.str, typing.Any]]]]] = None,
         name: typing.Optional[builtins.str] = None,
+        notification: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union["PipelineNotification", typing.Dict[builtins.str, typing.Any]]]]] = None,
         photon: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         storage: typing.Optional[builtins.str] = None,
         target: typing.Optional[builtins.str] = None,
         timeouts: typing.Optional[typing.Union["PipelineTimeouts", typing.Dict[builtins.str, typing.Any]]] = None,
     ) -> None:
         '''
         :param connection: 
@@ -3955,14 +3989,15 @@
         :param continuous: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/databricks/r/pipeline#continuous Pipeline#continuous}.
         :param development: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/databricks/r/pipeline#development Pipeline#development}.
         :param edition: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/databricks/r/pipeline#edition Pipeline#edition}.
         :param filters: filters block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/databricks/r/pipeline#filters Pipeline#filters}
         :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/databricks/r/pipeline#id Pipeline#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         :param library: library block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/databricks/r/pipeline#library Pipeline#library}
         :param name: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/databricks/r/pipeline#name Pipeline#name}.
+        :param notification: notification block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/databricks/r/pipeline#notification Pipeline#notification}
         :param photon: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/databricks/r/pipeline#photon Pipeline#photon}.
         :param storage: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/databricks/r/pipeline#storage Pipeline#storage}.
         :param target: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/databricks/r/pipeline#target Pipeline#target}.
         :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/databricks/r/pipeline#timeouts Pipeline#timeouts}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
@@ -3987,14 +4022,15 @@
             check_type(argname="argument continuous", value=continuous, expected_type=type_hints["continuous"])
             check_type(argname="argument development", value=development, expected_type=type_hints["development"])
             check_type(argname="argument edition", value=edition, expected_type=type_hints["edition"])
             check_type(argname="argument filters", value=filters, expected_type=type_hints["filters"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
             check_type(argname="argument library", value=library, expected_type=type_hints["library"])
             check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+            check_type(argname="argument notification", value=notification, expected_type=type_hints["notification"])
             check_type(argname="argument photon", value=photon, expected_type=type_hints["photon"])
             check_type(argname="argument storage", value=storage, expected_type=type_hints["storage"])
             check_type(argname="argument target", value=target, expected_type=type_hints["target"])
             check_type(argname="argument timeouts", value=timeouts, expected_type=type_hints["timeouts"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if connection is not None:
             self._values["connection"] = connection
@@ -4030,14 +4066,16 @@
             self._values["filters"] = filters
         if id is not None:
             self._values["id"] = id
         if library is not None:
             self._values["library"] = library
         if name is not None:
             self._values["name"] = name
+        if notification is not None:
+            self._values["notification"] = notification
         if photon is not None:
             self._values["photon"] = photon
         if storage is not None:
             self._values["storage"] = storage
         if target is not None:
             self._values["target"] = target
         if timeouts is not None:
@@ -4199,14 +4237,25 @@
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
         '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/databricks/r/pipeline#name Pipeline#name}.'''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
+    def notification(
+        self,
+    ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["PipelineNotification"]]]:
+        '''notification block.
+
+        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/databricks/r/pipeline#notification Pipeline#notification}
+        '''
+        result = self._values.get("notification")
+        return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["PipelineNotification"]]], result)
+
+    @builtins.property
     def photon(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/databricks/r/pipeline#photon Pipeline#photon}.'''
         result = self._values.get("photon")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
@@ -5054,14 +5103,233 @@
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__4f0f1330ccdcf68d22a72400fa4519013bc5e812b68193fc914bd4dd07ec9666)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "internalValue", value)
 
 
 @jsii.data_type(
+    jsii_type="@cdktf/provider-databricks.pipeline.PipelineNotification",
+    jsii_struct_bases=[],
+    name_mapping={"alerts": "alerts", "email_recipients": "emailRecipients"},
+)
+class PipelineNotification:
+    def __init__(
+        self,
+        *,
+        alerts: typing.Sequence[builtins.str],
+        email_recipients: typing.Sequence[builtins.str],
+    ) -> None:
+        '''
+        :param alerts: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/databricks/r/pipeline#alerts Pipeline#alerts}.
+        :param email_recipients: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/databricks/r/pipeline#email_recipients Pipeline#email_recipients}.
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__1b8e401d03bcfbc10097c2395af05aff23ca1cdc689241b820c76ab6b8761602)
+            check_type(argname="argument alerts", value=alerts, expected_type=type_hints["alerts"])
+            check_type(argname="argument email_recipients", value=email_recipients, expected_type=type_hints["email_recipients"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {
+            "alerts": alerts,
+            "email_recipients": email_recipients,
+        }
+
+    @builtins.property
+    def alerts(self) -> typing.List[builtins.str]:
+        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/databricks/r/pipeline#alerts Pipeline#alerts}.'''
+        result = self._values.get("alerts")
+        assert result is not None, "Required property 'alerts' is missing"
+        return typing.cast(typing.List[builtins.str], result)
+
+    @builtins.property
+    def email_recipients(self) -> typing.List[builtins.str]:
+        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/databricks/r/pipeline#email_recipients Pipeline#email_recipients}.'''
+        result = self._values.get("email_recipients")
+        assert result is not None, "Required property 'email_recipients' is missing"
+        return typing.cast(typing.List[builtins.str], result)
+
+    def __eq__(self, rhs: typing.Any) -> builtins.bool:
+        return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+    def __ne__(self, rhs: typing.Any) -> builtins.bool:
+        return not (rhs == self)
+
+    def __repr__(self) -> str:
+        return "PipelineNotification(%s)" % ", ".join(
+            k + "=" + repr(v) for k, v in self._values.items()
+        )
+
+
+class PipelineNotificationList(
+    _cdktf_9a9027ec.ComplexList,
+    metaclass=jsii.JSIIMeta,
+    jsii_type="@cdktf/provider-databricks.pipeline.PipelineNotificationList",
+):
+    def __init__(
+        self,
+        terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
+        terraform_attribute: builtins.str,
+        wraps_set: builtins.bool,
+    ) -> None:
+        '''
+        :param terraform_resource: The parent resource.
+        :param terraform_attribute: The attribute on the parent resource this class is referencing.
+        :param wraps_set: whether the list is wrapping a set (will add tolist() to be able to access an item via an index).
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__b6aca95e7ece8bb109cea2c71e613419108b1ca2886cc42d59674f1f36bc21b3)
+            check_type(argname="argument terraform_resource", value=terraform_resource, expected_type=type_hints["terraform_resource"])
+            check_type(argname="argument terraform_attribute", value=terraform_attribute, expected_type=type_hints["terraform_attribute"])
+            check_type(argname="argument wraps_set", value=wraps_set, expected_type=type_hints["wraps_set"])
+        jsii.create(self.__class__, self, [terraform_resource, terraform_attribute, wraps_set])
+
+    @jsii.member(jsii_name="get")
+    def get(self, index: jsii.Number) -> "PipelineNotificationOutputReference":
+        '''
+        :param index: the index of the item to return.
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__0a66e961227762c7b182c9167aa04f72f9bd31331e0546df3097c01a6a9e1a1d)
+            check_type(argname="argument index", value=index, expected_type=type_hints["index"])
+        return typing.cast("PipelineNotificationOutputReference", jsii.invoke(self, "get", [index]))
+
+    @builtins.property
+    @jsii.member(jsii_name="terraformAttribute")
+    def _terraform_attribute(self) -> builtins.str:
+        '''The attribute on the parent resource this class is referencing.'''
+        return typing.cast(builtins.str, jsii.get(self, "terraformAttribute"))
+
+    @_terraform_attribute.setter
+    def _terraform_attribute(self, value: builtins.str) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__8231cd11af95102a530318792ce0d1f23673fe1b9f2c164179a6a7b213f0d414)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "terraformAttribute", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="terraformResource")
+    def _terraform_resource(self) -> _cdktf_9a9027ec.IInterpolatingParent:
+        '''The parent resource.'''
+        return typing.cast(_cdktf_9a9027ec.IInterpolatingParent, jsii.get(self, "terraformResource"))
+
+    @_terraform_resource.setter
+    def _terraform_resource(self, value: _cdktf_9a9027ec.IInterpolatingParent) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__4b85bacc1230974e08767a382bfae3194c400bdba21bbcdfcc7961c2c9e18fbb)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "terraformResource", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="wrapsSet")
+    def _wraps_set(self) -> builtins.bool:
+        '''whether the list is wrapping a set (will add tolist() to be able to access an item via an index).'''
+        return typing.cast(builtins.bool, jsii.get(self, "wrapsSet"))
+
+    @_wraps_set.setter
+    def _wraps_set(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__ea7d09f0bf3cf787a07796959ed668f6733c8814a8d24b420f9a0c74824dcd65)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "wrapsSet", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="internalValue")
+    def internal_value(
+        self,
+    ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List[PipelineNotification]]]:
+        return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List[PipelineNotification]]], jsii.get(self, "internalValue"))
+
+    @internal_value.setter
+    def internal_value(
+        self,
+        value: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List[PipelineNotification]]],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__1af3a27adbe8aabb5143af173954cd2b3ef3b906a41312c354837028a5734b82)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "internalValue", value)
+
+
+class PipelineNotificationOutputReference(
+    _cdktf_9a9027ec.ComplexObject,
+    metaclass=jsii.JSIIMeta,
+    jsii_type="@cdktf/provider-databricks.pipeline.PipelineNotificationOutputReference",
+):
+    def __init__(
+        self,
+        terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
+        terraform_attribute: builtins.str,
+        complex_object_index: jsii.Number,
+        complex_object_is_from_set: builtins.bool,
+    ) -> None:
+        '''
+        :param terraform_resource: The parent resource.
+        :param terraform_attribute: The attribute on the parent resource this class is referencing.
+        :param complex_object_index: the index of this item in the list.
+        :param complex_object_is_from_set: whether the list is wrapping a set (will add tolist() to be able to access an item via an index).
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__61ad8747597828880f5cc8bc2efb25caa1ad683dc883428c18e99c410d461235)
+            check_type(argname="argument terraform_resource", value=terraform_resource, expected_type=type_hints["terraform_resource"])
+            check_type(argname="argument terraform_attribute", value=terraform_attribute, expected_type=type_hints["terraform_attribute"])
+            check_type(argname="argument complex_object_index", value=complex_object_index, expected_type=type_hints["complex_object_index"])
+            check_type(argname="argument complex_object_is_from_set", value=complex_object_is_from_set, expected_type=type_hints["complex_object_is_from_set"])
+        jsii.create(self.__class__, self, [terraform_resource, terraform_attribute, complex_object_index, complex_object_is_from_set])
+
+    @builtins.property
+    @jsii.member(jsii_name="alertsInput")
+    def alerts_input(self) -> typing.Optional[typing.List[builtins.str]]:
+        return typing.cast(typing.Optional[typing.List[builtins.str]], jsii.get(self, "alertsInput"))
+
+    @builtins.property
+    @jsii.member(jsii_name="emailRecipientsInput")
+    def email_recipients_input(self) -> typing.Optional[typing.List[builtins.str]]:
+        return typing.cast(typing.Optional[typing.List[builtins.str]], jsii.get(self, "emailRecipientsInput"))
+
+    @builtins.property
+    @jsii.member(jsii_name="alerts")
+    def alerts(self) -> typing.List[builtins.str]:
+        return typing.cast(typing.List[builtins.str], jsii.get(self, "alerts"))
+
+    @alerts.setter
+    def alerts(self, value: typing.List[builtins.str]) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__9054580b8a926c4b33655825efa87cdc724a30db1aeff0f21bc77a07cd3fc07a)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "alerts", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="emailRecipients")
+    def email_recipients(self) -> typing.List[builtins.str]:
+        return typing.cast(typing.List[builtins.str], jsii.get(self, "emailRecipients"))
+
+    @email_recipients.setter
+    def email_recipients(self, value: typing.List[builtins.str]) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__645b1e294b1de53b2f2eed598bd13922919608f76b48c84659597180c183c479)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "emailRecipients", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="internalValue")
+    def internal_value(
+        self,
+    ) -> typing.Optional[typing.Union[PipelineNotification, _cdktf_9a9027ec.IResolvable]]:
+        return typing.cast(typing.Optional[typing.Union[PipelineNotification, _cdktf_9a9027ec.IResolvable]], jsii.get(self, "internalValue"))
+
+    @internal_value.setter
+    def internal_value(
+        self,
+        value: typing.Optional[typing.Union[PipelineNotification, _cdktf_9a9027ec.IResolvable]],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__86723a1b41e3e00a1f3746f7e6f6c1aa26853ff57701cd2b6c95dc6f94412ffc)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "internalValue", value)
+
+
+@jsii.data_type(
     jsii_type="@cdktf/provider-databricks.pipeline.PipelineTimeouts",
     jsii_struct_bases=[],
     name_mapping={"default": "default"},
 )
 class PipelineTimeouts:
     def __init__(self, *, default: typing.Optional[builtins.str] = None) -> None:
         '''
@@ -5191,14 +5459,17 @@
     "PipelineLibraryFileOutputReference",
     "PipelineLibraryList",
     "PipelineLibraryMaven",
     "PipelineLibraryMavenOutputReference",
     "PipelineLibraryNotebook",
     "PipelineLibraryNotebookOutputReference",
     "PipelineLibraryOutputReference",
+    "PipelineNotification",
+    "PipelineNotificationList",
+    "PipelineNotificationOutputReference",
     "PipelineTimeouts",
     "PipelineTimeoutsOutputReference",
 ]
 
 publication.publish()
 
 def _typecheckingstub__d0bf98735978227a74d3563ac743f858b0ee60db9c653153e602bcf484da355f(
@@ -5213,14 +5484,15 @@
     continuous: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
     development: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
     edition: typing.Optional[builtins.str] = None,
     filters: typing.Optional[typing.Union[PipelineFilters, typing.Dict[builtins.str, typing.Any]]] = None,
     id: typing.Optional[builtins.str] = None,
     library: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union[PipelineLibrary, typing.Dict[builtins.str, typing.Any]]]]] = None,
     name: typing.Optional[builtins.str] = None,
+    notification: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union[PipelineNotification, typing.Dict[builtins.str, typing.Any]]]]] = None,
     photon: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
     storage: typing.Optional[builtins.str] = None,
     target: typing.Optional[builtins.str] = None,
     timeouts: typing.Optional[typing.Union[PipelineTimeouts, typing.Dict[builtins.str, typing.Any]]] = None,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
     count: typing.Optional[jsii.Number] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
@@ -5240,14 +5512,20 @@
 
 def _typecheckingstub__718051e6297cf70b4433c1dc18d1514e18bda33aa43b59951fed173deee71445(
     value: typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union[PipelineLibrary, typing.Dict[builtins.str, typing.Any]]]],
 ) -> None:
     """Type checking stubs"""
     pass
 
+def _typecheckingstub__aae2ffd87d23f97fff4978ba983ffa8f06b698de24c0d629ea578a2e012f2840(
+    value: typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union[PipelineNotification, typing.Dict[builtins.str, typing.Any]]]],
+) -> None:
+    """Type checking stubs"""
+    pass
+
 def _typecheckingstub__cc9504f8da036eea33cd9d2fa16e93a946738866c0f20f792eafc46b930f7623(
     value: typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable],
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__62ac2805211275e46dbbeeb48262da2e18af8958f90c77a563416d57d2f8e66f(
@@ -6041,14 +6319,15 @@
     continuous: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
     development: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
     edition: typing.Optional[builtins.str] = None,
     filters: typing.Optional[typing.Union[PipelineFilters, typing.Dict[builtins.str, typing.Any]]] = None,
     id: typing.Optional[builtins.str] = None,
     library: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union[PipelineLibrary, typing.Dict[builtins.str, typing.Any]]]]] = None,
     name: typing.Optional[builtins.str] = None,
+    notification: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union[PipelineNotification, typing.Dict[builtins.str, typing.Any]]]]] = None,
     photon: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
     storage: typing.Optional[builtins.str] = None,
     target: typing.Optional[builtins.str] = None,
     timeouts: typing.Optional[typing.Union[PipelineTimeouts, typing.Dict[builtins.str, typing.Any]]] = None,
 ) -> None:
     """Type checking stubs"""
     pass
@@ -6250,14 +6529,87 @@
 
 def _typecheckingstub__4f0f1330ccdcf68d22a72400fa4519013bc5e812b68193fc914bd4dd07ec9666(
     value: typing.Optional[typing.Union[PipelineLibrary, _cdktf_9a9027ec.IResolvable]],
 ) -> None:
     """Type checking stubs"""
     pass
 
+def _typecheckingstub__1b8e401d03bcfbc10097c2395af05aff23ca1cdc689241b820c76ab6b8761602(
+    *,
+    alerts: typing.Sequence[builtins.str],
+    email_recipients: typing.Sequence[builtins.str],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__b6aca95e7ece8bb109cea2c71e613419108b1ca2886cc42d59674f1f36bc21b3(
+    terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
+    terraform_attribute: builtins.str,
+    wraps_set: builtins.bool,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__0a66e961227762c7b182c9167aa04f72f9bd31331e0546df3097c01a6a9e1a1d(
+    index: jsii.Number,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__8231cd11af95102a530318792ce0d1f23673fe1b9f2c164179a6a7b213f0d414(
+    value: builtins.str,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__4b85bacc1230974e08767a382bfae3194c400bdba21bbcdfcc7961c2c9e18fbb(
+    value: _cdktf_9a9027ec.IInterpolatingParent,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__ea7d09f0bf3cf787a07796959ed668f6733c8814a8d24b420f9a0c74824dcd65(
+    value: builtins.bool,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__1af3a27adbe8aabb5143af173954cd2b3ef3b906a41312c354837028a5734b82(
+    value: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List[PipelineNotification]]],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__61ad8747597828880f5cc8bc2efb25caa1ad683dc883428c18e99c410d461235(
+    terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
+    terraform_attribute: builtins.str,
+    complex_object_index: jsii.Number,
+    complex_object_is_from_set: builtins.bool,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__9054580b8a926c4b33655825efa87cdc724a30db1aeff0f21bc77a07cd3fc07a(
+    value: typing.List[builtins.str],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__645b1e294b1de53b2f2eed598bd13922919608f76b48c84659597180c183c479(
+    value: typing.List[builtins.str],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__86723a1b41e3e00a1f3746f7e6f6c1aa26853ff57701cd2b6c95dc6f94412ffc(
+    value: typing.Optional[typing.Union[PipelineNotification, _cdktf_9a9027ec.IResolvable]],
+) -> None:
+    """Type checking stubs"""
+    pass
+
 def _typecheckingstub__1d29c3e7df634a524db84f9a53d81f360f05c83c2ec781945dacda30bf99870f(
     *,
     default: typing.Optional[builtins.str] = None,
 ) -> None:
     """Type checking stubs"""
     pass
```

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/provider/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/provider_resource/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/provider_resource/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/recipient/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/recipient/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/repo/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/repo/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/schema/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/secret/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/secret/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/secret_acl/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/secret_acl/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/secret_scope/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/secret_scope/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/service_principal/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/service_principal/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/service_principal_role/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/service_principal_role/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/service_principal_secret/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/service_principal_secret/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/share/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/share/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/sql_alert/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/sql_alert/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/sql_dashboard/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/sql_dashboard/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/sql_endpoint/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/sql_endpoint/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/sql_global_config/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/sql_global_config/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/sql_permissions/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/sql_permissions/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/sql_query/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/sql_query/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/sql_visualization/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/sql_visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/sql_widget/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/sql_widget/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/storage_credential/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/storage_credential/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/table/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/table/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/token/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/token/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/user/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/user/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/user_instance_profile/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/user_instance_profile/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/user_role/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/user_role/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks/workspace_conf/__init__.py` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks/workspace_conf/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks.egg-info/PKG-INFO` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-databricks
-Version: 5.0.8
+Version: 6.0.0
 Summary: Prebuilt databricks Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-databricks.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-databricks.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdktf-cdktf-provider-databricks-5.0.8/src/cdktf_cdktf_provider_databricks.egg-info/SOURCES.txt` & `cdktf-cdktf-provider-databricks-6.0.0/src/cdktf_cdktf_provider_databricks.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 src/cdktf_cdktf_provider_databricks/py.typed
 src/cdktf_cdktf_provider_databricks.egg-info/PKG-INFO
 src/cdktf_cdktf_provider_databricks.egg-info/SOURCES.txt
 src/cdktf_cdktf_provider_databricks.egg-info/dependency_links.txt
 src/cdktf_cdktf_provider_databricks.egg-info/requires.txt
 src/cdktf_cdktf_provider_databricks.egg-info/top_level.txt
 src/cdktf_cdktf_provider_databricks/_jsii/__init__.py
-src/cdktf_cdktf_provider_databricks/_jsii/provider-databricks@5.0.8.jsii.tgz
+src/cdktf_cdktf_provider_databricks/_jsii/provider-databricks@6.0.0.jsii.tgz
 src/cdktf_cdktf_provider_databricks/aws_s3_mount/__init__.py
 src/cdktf_cdktf_provider_databricks/azure_adls_gen1_mount/__init__.py
 src/cdktf_cdktf_provider_databricks/azure_adls_gen2_mount/__init__.py
 src/cdktf_cdktf_provider_databricks/azure_blob_mount/__init__.py
 src/cdktf_cdktf_provider_databricks/catalog/__init__.py
 src/cdktf_cdktf_provider_databricks/cluster/__init__.py
 src/cdktf_cdktf_provider_databricks/cluster_policy/__init__.py
```

