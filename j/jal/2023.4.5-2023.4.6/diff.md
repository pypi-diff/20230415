# Comparing `tmp/jal-2023.4.5.tar.gz` & `tmp/jal-2023.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jal-2023.4.5.tar", last modified: Fri Apr 14 18:18:09 2023, max compression
+gzip compressed data, was "jal-2023.4.6.tar", last modified: Sat Apr 15 14:24:53 2023, max compression
```

## Comparing `jal-2023.4.5.tar` & `jal-2023.4.6.tar`

### file list

```diff
@@ -1,218 +1,218 @@
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-14 18:18:09.164846 jal-2023.4.5/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      176 2022-01-13 06:08:45.000000 jal-2023.4.5/MANIFEST.in
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2726 2023-04-14 18:18:09.164846 jal-2023.4.5/PKG-INFO
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-14 18:18:09.121513 jal-2023.4.5/docs/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     7665 2023-04-14 11:26:23.000000 jal-2023.4.5/docs/README.md
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-14 18:18:09.124846 jal-2023.4.5/jal/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)       24 2023-04-14 18:15:15.000000 jal-2023.4.5/jal/__init__.py
--rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)     3832 2023-04-07 14:10:37.000000 jal-2023.4.5/jal/constants.py
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-14 18:18:09.124846 jal-2023.4.5/jal/data_export/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2022-01-13 15:45:51.000000 jal-2023.4.5/jal/data_export/__init__.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    19856 2023-04-14 11:26:23.000000 jal-2023.4.5/jal/data_export/dlsg.py
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-14 18:18:09.128179 jal-2023.4.5/jal/data_export/tax_reports/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2020-12-23 19:03:58.000000 jal-2023.4.5/jal/data_export/tax_reports/__init__.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      990 2023-02-07 18:26:24.000000 jal-2023.4.5/jal/data_export/tax_reports/portugal.json
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     7089 2023-02-08 10:00:47.000000 jal-2023.4.5/jal/data_export/tax_reports/portugal.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1532 2023-02-07 18:26:24.000000 jal-2023.4.5/jal/data_export/tax_reports/russia.json
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    38366 2023-04-14 11:26:23.000000 jal-2023.4.5/jal/data_export/tax_reports/russia.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6433 2023-02-07 18:26:24.000000 jal-2023.4.5/jal/data_export/taxes.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5299 2023-02-07 18:26:24.000000 jal-2023.4.5/jal/data_export/taxes_flow.py
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-14 18:18:09.128179 jal-2023.4.5/jal/data_export/templates/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)        0 2022-01-30 08:37:57.000000 jal-2023.4.5/jal/data_export/templates/__init__.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1286 2023-02-07 18:26:24.000000 jal-2023.4.5/jal/data_export/templates/tax_prt_dividends.json
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2594 2023-02-07 18:26:24.000000 jal-2023.4.5/jal/data_export/templates/tax_prt_shares.json
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6163 2022-01-30 08:37:57.000000 jal-2023.4.5/jal/data_export/templates/tax_rus_bonds.json
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4792 2022-02-13 11:04:18.000000 jal-2023.4.5/jal/data_export/templates/tax_rus_corporate_actions.json
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4938 2022-04-30 20:05:13.000000 jal-2023.4.5/jal/data_export/templates/tax_rus_crypto.json
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4948 2022-04-30 20:05:13.000000 jal-2023.4.5/jal/data_export/templates/tax_rus_derivatives.json
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3249 2022-02-13 11:04:18.000000 jal-2023.4.5/jal/data_export/templates/tax_rus_dividends.json
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1450 2022-01-30 08:37:57.000000 jal-2023.4.5/jal/data_export/templates/tax_rus_fees.json
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1133 2022-06-19 17:39:33.000000 jal-2023.4.5/jal/data_export/templates/tax_rus_flow.json
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1654 2022-07-20 07:00:10.000000 jal-2023.4.5/jal/data_export/templates/tax_rus_interests.json
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5303 2022-01-30 08:37:57.000000 jal-2023.4.5/jal/data_export/templates/tax_rus_trades.json
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    10842 2023-02-08 13:35:53.000000 jal-2023.4.5/jal/data_export/xlsx.py
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-14 18:18:09.131513 jal-2023.4.5/jal/data_import/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2020-12-23 19:03:58.000000 jal-2023.4.5/jal/data_import/__init__.py
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-14 18:18:09.134846 jal-2023.4.5/jal/data_import/broker_statements/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)        0 2022-01-22 16:32:16.000000 jal-2023.4.5/jal/data_import/broker_statements/__init__.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    63265 2023-04-14 11:26:23.000000 jal-2023.4.5/jal/data_import/broker_statements/ibkr.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    19903 2022-08-21 07:15:06.000000 jal-2023.4.5/jal/data_import/broker_statements/just2trade.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     9470 2022-08-21 07:15:06.000000 jal-2023.4.5/jal/data_import/broker_statements/kit.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5857 2023-02-14 12:14:19.000000 jal-2023.4.5/jal/data_import/broker_statements/open_portfolio.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    30709 2023-02-14 12:16:51.000000 jal-2023.4.5/jal/data_import/broker_statements/openbroker.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    15460 2022-12-07 21:59:21.000000 jal-2023.4.5/jal/data_import/broker_statements/psb.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    27469 2022-08-21 07:15:06.000000 jal-2023.4.5/jal/data_import/broker_statements/uralsib.py
--rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)     3893 2023-03-05 19:06:08.000000 jal-2023.4.5/jal/data_import/category_recognizer.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      543 2021-08-05 15:24:10.000000 jal-2023.4.5/jal/data_import/import_schema.json
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    15609 2023-04-14 18:14:21.000000 jal-2023.4.5/jal/data_import/slips.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    13145 2023-04-14 18:14:21.000000 jal-2023.4.5/jal/data_import/slips_tax.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    35649 2023-04-14 11:26:23.000000 jal-2023.4.5/jal/data_import/statement.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    11314 2023-02-02 08:45:14.000000 jal-2023.4.5/jal/data_import/statement_xls.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6950 2023-04-14 11:26:23.000000 jal-2023.4.5/jal/data_import/statement_xml.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3224 2023-04-08 19:50:05.000000 jal-2023.4.5/jal/data_import/statements.py
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-14 18:18:09.138179 jal-2023.4.5/jal/db/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2020-12-23 19:03:58.000000 jal-2023.4.5/jal/db/__init__.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    17607 2023-02-27 16:25:45.000000 jal-2023.4.5/jal/db/account.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    21487 2023-04-14 11:26:23.000000 jal-2023.4.5/jal/db/asset.py
--rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)     6074 2022-12-06 18:30:39.000000 jal-2023.4.5/jal/db/backup_restore.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     7360 2023-02-27 17:48:37.000000 jal-2023.4.5/jal/db/balances_model.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4103 2023-02-27 16:03:46.000000 jal-2023.4.5/jal/db/category.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5218 2023-02-07 18:26:24.000000 jal-2023.4.5/jal/db/closed_trade.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2399 2023-03-08 17:11:23.000000 jal-2023.4.5/jal/db/country.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    18497 2023-04-14 18:14:21.000000 jal-2023.4.5/jal/db/db.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3941 2023-04-12 09:44:25.000000 jal-2023.4.5/jal/db/helpers.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    15989 2023-04-14 11:27:05.000000 jal-2023.4.5/jal/db/holdings_model.py
--rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)    16687 2023-04-14 18:14:21.000000 jal-2023.4.5/jal/db/ledger.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    60565 2023-04-07 14:10:37.000000 jal-2023.4.5/jal/db/operations.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     7486 2023-02-28 14:47:51.000000 jal-2023.4.5/jal/db/operations_model.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3379 2023-02-20 16:05:40.000000 jal-2023.4.5/jal/db/peer.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    15187 2023-04-14 18:14:21.000000 jal-2023.4.5/jal/db/reference_models.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1190 2023-01-06 21:49:49.000000 jal-2023.4.5/jal/db/settings.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      438 2023-02-16 17:12:29.000000 jal-2023.4.5/jal/db/tag.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6777 2023-04-14 18:14:21.000000 jal-2023.4.5/jal/db/tax_estimator.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1458 2023-02-23 19:54:06.000000 jal-2023.4.5/jal/db/view_model.py
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-14 18:18:09.138179 jal-2023.4.5/jal/img/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2922 2021-05-26 12:51:46.000000 jal-2023.4.5/jal/img/accept.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1443 2021-05-26 12:51:46.000000 jal-2023.4.5/jal/img/add.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2049 2021-05-26 12:51:46.000000 jal-2023.4.5/jal/img/add_child.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      435 2022-04-25 10:26:48.000000 jal-2023.4.5/jal/img/broom.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4004 2021-05-26 12:51:46.000000 jal-2023.4.5/jal/img/cancel.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      806 2023-03-08 16:58:09.000000 jal-2023.4.5/jal/img/chart.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      898 2021-05-26 12:51:46.000000 jal-2023.4.5/jal/img/copy.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2812 2021-05-26 12:51:46.000000 jal-2023.4.5/jal/img/delete.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      583 2021-03-20 12:52:05.000000 jal-2023.4.5/jal/img/ibkr.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2340 2022-04-29 07:05:21.000000 jal-2023.4.5/jal/img/j2t.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5563 2022-01-13 06:08:45.000000 jal-2023.4.5/jal/img/jal.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1516 2021-03-22 11:20:31.000000 jal-2023.4.5/jal/img/kit.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1163 2022-12-28 10:47:37.000000 jal-2023.4.5/jal/img/list.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      342 2022-04-25 10:26:48.000000 jal-2023.4.5/jal/img/meatballs.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      611 2021-05-26 12:51:46.000000 jal-2023.4.5/jal/img/new.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1175 2022-07-10 15:39:56.000000 jal-2023.4.5/jal/img/open_portfolio.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    15086 2021-08-05 15:24:10.000000 jal-2023.4.5/jal/img/openbroker.ico
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1150 2021-08-05 15:24:10.000000 jal-2023.4.5/jal/img/psb.ico
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1150 2021-03-20 12:52:05.000000 jal-2023.4.5/jal/img/quik.ico
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2651 2021-05-26 12:51:46.000000 jal-2023.4.5/jal/img/reconcile.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      822 2021-05-26 12:51:46.000000 jal-2023.4.5/jal/img/remove.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1874 2023-03-08 16:53:42.000000 jal-2023.4.5/jal/img/tax.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1406 2021-03-20 12:52:05.000000 jal-2023.4.5/jal/img/uralsib.ico
--rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)     1938 2023-01-19 12:05:21.000000 jal-2023.4.5/jal/jal.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    91499 2023-04-07 14:10:37.000000 jal-2023.4.5/jal/jal_init.sql
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-14 18:18:09.141513 jal-2023.4.5/jal/languages/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      424 2020-12-21 16:23:10.000000 jal-2023.4.5/jal/languages/en.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    32025 2022-01-13 06:08:45.000000 jal-2023.4.5/jal/languages/en.qm
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      287 2022-04-25 10:26:48.000000 jal-2023.4.5/jal/languages/ru.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    86944 2023-04-14 11:26:41.000000 jal-2023.4.5/jal/languages/ru.qm
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-14 18:18:09.141513 jal-2023.4.5/jal/net/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2021-08-17 15:15:47.000000 jal-2023.4.5/jal/net/__init__.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    24656 2023-04-14 18:14:21.000000 jal-2023.4.5/jal/net/downloader.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2912 2023-01-27 21:53:46.000000 jal-2023.4.5/jal/net/helpers.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2040 2023-03-06 11:34:17.000000 jal-2023.4.5/jal/pypi_description.md
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-14 18:18:09.141513 jal-2023.4.5/jal/reports/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2020-12-23 19:03:58.000000 jal-2023.4.5/jal/reports/__init__.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2967 2023-04-14 18:14:21.000000 jal-2023.4.5/jal/reports/category.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    14386 2023-04-14 18:14:21.000000 jal-2023.4.5/jal/reports/deals.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3936 2023-04-14 18:14:21.000000 jal-2023.4.5/jal/reports/holdings.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    14756 2023-04-14 18:14:21.000000 jal-2023.4.5/jal/reports/income_spending.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2855 2023-04-14 18:14:21.000000 jal-2023.4.5/jal/reports/peer.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     8771 2023-04-14 18:14:21.000000 jal-2023.4.5/jal/reports/profit_loss.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3287 2023-02-16 10:22:14.000000 jal-2023.4.5/jal/reports/reports.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2827 2023-04-14 18:14:21.000000 jal-2023.4.5/jal/reports/tag.py
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-14 18:18:09.144846 jal-2023.4.5/jal/ui/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2020-12-23 19:03:58.000000 jal-2023.4.5/jal/ui/__init__.py
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-14 18:18:09.144846 jal-2023.4.5/jal/ui/reports/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)        0 2022-01-13 15:45:51.000000 jal-2023.4.5/jal/ui/reports/__init__.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5179 2023-04-09 17:45:04.000000 jal-2023.4.5/jal/ui/reports/ui_category_report.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4099 2023-04-14 11:27:05.000000 jal-2023.4.5/jal/ui/reports/ui_deals_report.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4159 2023-04-14 11:27:05.000000 jal-2023.4.5/jal/ui/reports/ui_holdings_report.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4156 2023-04-09 17:45:04.000000 jal-2023.4.5/jal/ui/reports/ui_income_spending_report.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5382 2023-04-09 17:45:04.000000 jal-2023.4.5/jal/ui/reports/ui_peer_report.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4687 2023-04-09 17:45:04.000000 jal-2023.4.5/jal/ui/reports/ui_profit_loss_report.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5353 2023-04-09 17:45:04.000000 jal-2023.4.5/jal/ui/reports/ui_tag_report.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4805 2023-04-09 17:45:04.000000 jal-2023.4.5/jal/ui/reports/ui_tax_estimation.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    12742 2023-04-09 17:45:04.000000 jal-2023.4.5/jal/ui/ui_asset_dlg.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4056 2023-04-09 17:45:04.000000 jal-2023.4.5/jal/ui/ui_flow_export_widget.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    14782 2023-04-09 17:45:04.000000 jal-2023.4.5/jal/ui/ui_login_fns_dlg.py
--rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)     9324 2023-04-12 14:15:34.000000 jal-2023.4.5/jal/ui/ui_main_window.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    14510 2023-04-09 17:45:04.000000 jal-2023.4.5/jal/ui/ui_operations_widget.py
--rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)     5707 2023-04-09 17:45:04.000000 jal-2023.4.5/jal/ui/ui_rebuild_window.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     7302 2023-04-09 17:45:04.000000 jal-2023.4.5/jal/ui/ui_reference_data_dlg.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2903 2023-04-09 17:45:04.000000 jal-2023.4.5/jal/ui/ui_select_account_dlg.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3253 2023-04-09 17:45:04.000000 jal-2023.4.5/jal/ui/ui_select_reference_dlg.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    16301 2023-04-09 17:45:04.000000 jal-2023.4.5/jal/ui/ui_slip_import_dlg.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     9674 2023-04-09 17:45:04.000000 jal-2023.4.5/jal/ui/ui_tax_export_widget.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4023 2023-04-09 17:45:04.000000 jal-2023.4.5/jal/ui/ui_update_quotes_window.py
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-14 18:18:09.158180 jal-2023.4.5/jal/updates/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2020-12-23 19:03:58.000000 jal-2023.4.5/jal/updates/__init__.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5122 2020-12-21 16:23:10.000000 jal-2023.4.5/jal/updates/jal_delta_10.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    12870 2021-08-18 12:53:40.000000 jal-2023.4.5/jal/updates/jal_delta_11.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    26116 2021-01-13 17:04:46.000000 jal-2023.4.5/jal/updates/jal_delta_12.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    16516 2021-01-30 16:01:43.000000 jal-2023.4.5/jal/updates/jal_delta_13.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    34961 2021-02-27 17:35:02.000000 jal-2023.4.5/jal/updates/jal_delta_14.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2250 2021-02-27 17:35:02.000000 jal-2023.4.5/jal/updates/jal_delta_15.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3630 2021-02-27 17:35:02.000000 jal-2023.4.5/jal/updates/jal_delta_16.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    20912 2021-02-27 17:35:02.000000 jal-2023.4.5/jal/updates/jal_delta_17.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      656 2021-03-07 11:58:53.000000 jal-2023.4.5/jal/updates/jal_delta_18.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      686 2021-03-08 13:39:11.000000 jal-2023.4.5/jal/updates/jal_delta_19.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    13578 2021-03-12 14:26:01.000000 jal-2023.4.5/jal/updates/jal_delta_20.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1428 2021-03-19 12:24:53.000000 jal-2023.4.5/jal/updates/jal_delta_21.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      949 2021-03-22 11:20:31.000000 jal-2023.4.5/jal/updates/jal_delta_22.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    17602 2021-04-08 12:12:36.000000 jal-2023.4.5/jal/updates/jal_delta_23.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      344 2021-04-11 10:57:46.000000 jal-2023.4.5/jal/updates/jal_delta_24.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     8270 2021-04-22 04:11:28.000000 jal-2023.4.5/jal/updates/jal_delta_25.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2492 2021-08-12 19:15:12.000000 jal-2023.4.5/jal/updates/jal_delta_26.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    26325 2022-01-13 05:57:31.000000 jal-2023.4.5/jal/updates/jal_delta_27.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    13276 2022-01-13 06:08:45.000000 jal-2023.4.5/jal/updates/jal_delta_28.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    35370 2022-01-13 15:45:51.000000 jal-2023.4.5/jal/updates/jal_delta_29.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     8671 2022-02-13 13:11:58.000000 jal-2023.4.5/jal/updates/jal_delta_30.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    11413 2022-02-13 11:04:18.000000 jal-2023.4.5/jal/updates/jal_delta_31.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    12545 2022-03-31 14:26:11.000000 jal-2023.4.5/jal/updates/jal_delta_32.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4229 2022-03-31 14:26:11.000000 jal-2023.4.5/jal/updates/jal_delta_33.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2287 2022-04-06 14:47:21.000000 jal-2023.4.5/jal/updates/jal_delta_34.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2858 2022-04-30 20:05:13.000000 jal-2023.4.5/jal/updates/jal_delta_35.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3427 2022-06-19 17:39:33.000000 jal-2023.4.5/jal/updates/jal_delta_36.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3755 2022-07-20 07:00:10.000000 jal-2023.4.5/jal/updates/jal_delta_37.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    21913 2022-08-21 07:15:06.000000 jal-2023.4.5/jal/updates/jal_delta_38.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      343 2023-01-04 13:14:35.000000 jal-2023.4.5/jal/updates/jal_delta_39.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3055 2023-01-27 21:53:46.000000 jal-2023.4.5/jal/updates/jal_delta_40.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    48157 2023-02-07 18:26:24.000000 jal-2023.4.5/jal/updates/jal_delta_41.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2085 2023-02-20 14:55:36.000000 jal-2023.4.5/jal/updates/jal_delta_42.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2528 2023-03-08 16:23:30.000000 jal-2023.4.5/jal/updates/jal_delta_43.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3020 2023-04-07 14:10:37.000000 jal-2023.4.5/jal/updates/jal_delta_44.sql
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-14 18:18:09.161513 jal-2023.4.5/jal/widgets/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2020-12-23 19:03:58.000000 jal-2023.4.5/jal/widgets/__init__.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3918 2023-01-09 20:51:48.000000 jal-2023.4.5/jal/widgets/abstract_operation_details.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6844 2023-04-14 18:14:21.000000 jal-2023.4.5/jal/widgets/account_select.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    14131 2023-04-14 18:14:21.000000 jal-2023.4.5/jal/widgets/asset_dialog.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    11151 2023-02-23 19:44:39.000000 jal-2023.4.5/jal/widgets/corporate_action_widget.py
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-14 18:18:09.161513 jal-2023.4.5/jal/widgets/custom/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)        0 2022-12-24 19:32:40.000000 jal-2023.4.5/jal/widgets/custom/__init__.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4435 2023-04-14 18:14:21.000000 jal-2023.4.5/jal/widgets/custom/date_range_selector.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2016 2023-01-09 21:29:20.000000 jal-2023.4.5/jal/widgets/custom/db_lookup_combobox.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5331 2023-04-14 18:14:21.000000 jal-2023.4.5/jal/widgets/custom/log_viewer.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    13750 2023-04-14 18:14:21.000000 jal-2023.4.5/jal/widgets/delegates.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     9321 2023-03-08 16:41:32.000000 jal-2023.4.5/jal/widgets/dividend_widget.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     8437 2023-04-14 18:14:21.000000 jal-2023.4.5/jal/widgets/helpers.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    12298 2023-02-25 18:52:44.000000 jal-2023.4.5/jal/widgets/income_spending_widget.py
--rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)    13018 2023-04-14 18:14:21.000000 jal-2023.4.5/jal/widgets/main_window.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3385 2023-04-14 18:14:21.000000 jal-2023.4.5/jal/widgets/mdi.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2854 2022-12-26 13:26:40.000000 jal-2023.4.5/jal/widgets/operations_tabs.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     7159 2023-04-14 18:14:21.000000 jal-2023.4.5/jal/widgets/operations_widget.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6012 2023-04-14 18:14:21.000000 jal-2023.4.5/jal/widgets/price_chart.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5666 2023-04-14 18:09:14.000000 jal-2023.4.5/jal/widgets/qr_scanner.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    11244 2023-04-14 18:14:21.000000 jal-2023.4.5/jal/widgets/reference_data.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    21798 2023-04-14 18:14:21.000000 jal-2023.4.5/jal/widgets/reference_dialogs.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4863 2023-02-19 18:07:24.000000 jal-2023.4.5/jal/widgets/reference_selector.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      632 2022-12-26 08:54:07.000000 jal-2023.4.5/jal/widgets/register_designer_plugins.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3505 2023-04-14 18:14:21.000000 jal-2023.4.5/jal/widgets/selection_dialog.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     7862 2023-04-14 18:14:21.000000 jal-2023.4.5/jal/widgets/tax_widget.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6922 2022-12-26 10:36:44.000000 jal-2023.4.5/jal/widgets/trade_widget.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    10120 2023-04-07 14:10:37.000000 jal-2023.4.5/jal/widgets/transfer_widget.py
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-14 18:18:09.124846 jal-2023.4.5/jal.egg-info/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2726 2023-04-14 18:18:09.000000 jal-2023.4.5/jal.egg-info/PKG-INFO
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5592 2023-04-14 18:18:09.000000 jal-2023.4.5/jal.egg-info/SOURCES.txt
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)        1 2023-04-14 18:18:09.000000 jal-2023.4.5/jal.egg-info/dependency_links.txt
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)       37 2023-04-14 18:18:09.000000 jal-2023.4.5/jal.egg-info/entry_points.txt
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)       67 2023-04-14 18:18:09.000000 jal-2023.4.5/jal.egg-info/requires.txt
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)       10 2023-04-14 18:18:09.000000 jal-2023.4.5/jal.egg-info/top_level.txt
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)       38 2023-04-14 18:18:09.164846 jal-2023.4.5/setup.cfg
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1756 2023-04-14 18:14:21.000000 jal-2023.4.5/setup.py
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-15 14:24:53.986407 jal-2023.4.6/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      176 2022-01-13 06:08:45.000000 jal-2023.4.6/MANIFEST.in
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2726 2023-04-15 14:24:53.986407 jal-2023.4.6/PKG-INFO
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-15 14:24:53.943073 jal-2023.4.6/docs/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     7580 2023-04-15 14:23:01.000000 jal-2023.4.6/docs/README.md
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-15 14:24:53.949740 jal-2023.4.6/jal/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)       24 2023-04-15 14:19:23.000000 jal-2023.4.6/jal/__init__.py
+-rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)     3831 2023-04-15 14:13:28.000000 jal-2023.4.6/jal/constants.py
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-15 14:24:53.949740 jal-2023.4.6/jal/data_export/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2022-01-13 15:45:51.000000 jal-2023.4.6/jal/data_export/__init__.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    19856 2023-04-14 11:26:23.000000 jal-2023.4.6/jal/data_export/dlsg.py
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-15 14:24:53.953073 jal-2023.4.6/jal/data_export/tax_reports/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2020-12-23 19:03:58.000000 jal-2023.4.6/jal/data_export/tax_reports/__init__.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      990 2023-02-07 18:26:24.000000 jal-2023.4.6/jal/data_export/tax_reports/portugal.json
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     7089 2023-02-08 10:00:47.000000 jal-2023.4.6/jal/data_export/tax_reports/portugal.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1532 2023-02-07 18:26:24.000000 jal-2023.4.6/jal/data_export/tax_reports/russia.json
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    38366 2023-04-14 11:26:23.000000 jal-2023.4.6/jal/data_export/tax_reports/russia.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6433 2023-02-07 18:26:24.000000 jal-2023.4.6/jal/data_export/taxes.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5299 2023-02-07 18:26:24.000000 jal-2023.4.6/jal/data_export/taxes_flow.py
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-15 14:24:53.956406 jal-2023.4.6/jal/data_export/templates/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)        0 2022-01-30 08:37:57.000000 jal-2023.4.6/jal/data_export/templates/__init__.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1286 2023-02-07 18:26:24.000000 jal-2023.4.6/jal/data_export/templates/tax_prt_dividends.json
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2594 2023-02-07 18:26:24.000000 jal-2023.4.6/jal/data_export/templates/tax_prt_shares.json
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6163 2022-01-30 08:37:57.000000 jal-2023.4.6/jal/data_export/templates/tax_rus_bonds.json
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4792 2022-02-13 11:04:18.000000 jal-2023.4.6/jal/data_export/templates/tax_rus_corporate_actions.json
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4938 2022-04-30 20:05:13.000000 jal-2023.4.6/jal/data_export/templates/tax_rus_crypto.json
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4948 2022-04-30 20:05:13.000000 jal-2023.4.6/jal/data_export/templates/tax_rus_derivatives.json
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3249 2022-02-13 11:04:18.000000 jal-2023.4.6/jal/data_export/templates/tax_rus_dividends.json
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1450 2022-01-30 08:37:57.000000 jal-2023.4.6/jal/data_export/templates/tax_rus_fees.json
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1133 2022-06-19 17:39:33.000000 jal-2023.4.6/jal/data_export/templates/tax_rus_flow.json
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1654 2022-07-20 07:00:10.000000 jal-2023.4.6/jal/data_export/templates/tax_rus_interests.json
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5303 2022-01-30 08:37:57.000000 jal-2023.4.6/jal/data_export/templates/tax_rus_trades.json
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    10842 2023-02-08 13:35:53.000000 jal-2023.4.6/jal/data_export/xlsx.py
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-15 14:24:53.956406 jal-2023.4.6/jal/data_import/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2020-12-23 19:03:58.000000 jal-2023.4.6/jal/data_import/__init__.py
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-15 14:24:53.959740 jal-2023.4.6/jal/data_import/broker_statements/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)        0 2022-01-22 16:32:16.000000 jal-2023.4.6/jal/data_import/broker_statements/__init__.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    63265 2023-04-14 11:26:23.000000 jal-2023.4.6/jal/data_import/broker_statements/ibkr.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    19903 2022-08-21 07:15:06.000000 jal-2023.4.6/jal/data_import/broker_statements/just2trade.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     9470 2022-08-21 07:15:06.000000 jal-2023.4.6/jal/data_import/broker_statements/kit.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5857 2023-02-14 12:14:19.000000 jal-2023.4.6/jal/data_import/broker_statements/open_portfolio.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    30709 2023-02-14 12:16:51.000000 jal-2023.4.6/jal/data_import/broker_statements/openbroker.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    15460 2022-12-07 21:59:21.000000 jal-2023.4.6/jal/data_import/broker_statements/psb.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    27469 2022-08-21 07:15:06.000000 jal-2023.4.6/jal/data_import/broker_statements/uralsib.py
+-rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)     3893 2023-03-05 19:06:08.000000 jal-2023.4.6/jal/data_import/category_recognizer.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      543 2021-08-05 15:24:10.000000 jal-2023.4.6/jal/data_import/import_schema.json
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    15598 2023-04-15 14:13:28.000000 jal-2023.4.6/jal/data_import/slips.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    13145 2023-04-14 18:14:21.000000 jal-2023.4.6/jal/data_import/slips_tax.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    35649 2023-04-14 11:26:23.000000 jal-2023.4.6/jal/data_import/statement.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    11314 2023-02-02 08:45:14.000000 jal-2023.4.6/jal/data_import/statement_xls.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6950 2023-04-14 11:26:23.000000 jal-2023.4.6/jal/data_import/statement_xml.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3224 2023-04-08 19:50:05.000000 jal-2023.4.6/jal/data_import/statements.py
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-15 14:24:53.959740 jal-2023.4.6/jal/db/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2020-12-23 19:03:58.000000 jal-2023.4.6/jal/db/__init__.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    17607 2023-02-27 16:25:45.000000 jal-2023.4.6/jal/db/account.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    21487 2023-04-14 11:26:23.000000 jal-2023.4.6/jal/db/asset.py
+-rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)     6074 2022-12-06 18:30:39.000000 jal-2023.4.6/jal/db/backup_restore.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     7360 2023-02-27 17:48:37.000000 jal-2023.4.6/jal/db/balances_model.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4103 2023-02-27 16:03:46.000000 jal-2023.4.6/jal/db/category.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5218 2023-02-07 18:26:24.000000 jal-2023.4.6/jal/db/closed_trade.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2399 2023-03-08 17:11:23.000000 jal-2023.4.6/jal/db/country.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    18652 2023-04-15 13:39:15.000000 jal-2023.4.6/jal/db/db.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3941 2023-04-12 09:44:25.000000 jal-2023.4.6/jal/db/helpers.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    15989 2023-04-14 11:27:05.000000 jal-2023.4.6/jal/db/holdings_model.py
+-rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)    16683 2023-04-15 14:13:28.000000 jal-2023.4.6/jal/db/ledger.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    60565 2023-04-07 14:10:37.000000 jal-2023.4.6/jal/db/operations.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     7475 2023-04-15 14:13:28.000000 jal-2023.4.6/jal/db/operations_model.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3379 2023-02-20 16:05:40.000000 jal-2023.4.6/jal/db/peer.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    15204 2023-04-15 13:54:08.000000 jal-2023.4.6/jal/db/reference_models.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1190 2023-01-06 21:49:49.000000 jal-2023.4.6/jal/db/settings.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      438 2023-02-16 17:12:29.000000 jal-2023.4.6/jal/db/tag.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6777 2023-04-14 18:14:21.000000 jal-2023.4.6/jal/db/tax_estimator.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1458 2023-02-23 19:54:06.000000 jal-2023.4.6/jal/db/view_model.py
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-15 14:24:53.963073 jal-2023.4.6/jal/img/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2922 2021-05-26 12:51:46.000000 jal-2023.4.6/jal/img/accept.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1443 2021-05-26 12:51:46.000000 jal-2023.4.6/jal/img/add.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2049 2021-05-26 12:51:46.000000 jal-2023.4.6/jal/img/add_child.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      435 2022-04-25 10:26:48.000000 jal-2023.4.6/jal/img/broom.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4004 2021-05-26 12:51:46.000000 jal-2023.4.6/jal/img/cancel.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      806 2023-03-08 16:58:09.000000 jal-2023.4.6/jal/img/chart.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      898 2021-05-26 12:51:46.000000 jal-2023.4.6/jal/img/copy.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2812 2021-05-26 12:51:46.000000 jal-2023.4.6/jal/img/delete.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      583 2021-03-20 12:52:05.000000 jal-2023.4.6/jal/img/ibkr.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2340 2022-04-29 07:05:21.000000 jal-2023.4.6/jal/img/j2t.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5563 2022-01-13 06:08:45.000000 jal-2023.4.6/jal/img/jal.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1516 2021-03-22 11:20:31.000000 jal-2023.4.6/jal/img/kit.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1163 2022-12-28 10:47:37.000000 jal-2023.4.6/jal/img/list.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      342 2022-04-25 10:26:48.000000 jal-2023.4.6/jal/img/meatballs.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      611 2021-05-26 12:51:46.000000 jal-2023.4.6/jal/img/new.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1175 2022-07-10 15:39:56.000000 jal-2023.4.6/jal/img/open_portfolio.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    15086 2021-08-05 15:24:10.000000 jal-2023.4.6/jal/img/openbroker.ico
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1150 2021-08-05 15:24:10.000000 jal-2023.4.6/jal/img/psb.ico
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1150 2021-03-20 12:52:05.000000 jal-2023.4.6/jal/img/quik.ico
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2651 2021-05-26 12:51:46.000000 jal-2023.4.6/jal/img/reconcile.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      822 2021-05-26 12:51:46.000000 jal-2023.4.6/jal/img/remove.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1874 2023-03-08 16:53:42.000000 jal-2023.4.6/jal/img/tax.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1406 2021-03-20 12:52:05.000000 jal-2023.4.6/jal/img/uralsib.ico
+-rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)     1938 2023-01-19 12:05:21.000000 jal-2023.4.6/jal/jal.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    91499 2023-04-07 14:10:37.000000 jal-2023.4.6/jal/jal_init.sql
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-15 14:24:53.966406 jal-2023.4.6/jal/languages/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      424 2020-12-21 16:23:10.000000 jal-2023.4.6/jal/languages/en.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    32025 2022-01-13 06:08:45.000000 jal-2023.4.6/jal/languages/en.qm
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      287 2022-04-25 10:26:48.000000 jal-2023.4.6/jal/languages/ru.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    87568 2023-04-15 14:17:53.000000 jal-2023.4.6/jal/languages/ru.qm
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-15 14:24:53.966406 jal-2023.4.6/jal/net/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2021-08-17 15:15:47.000000 jal-2023.4.6/jal/net/__init__.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    24656 2023-04-14 18:14:21.000000 jal-2023.4.6/jal/net/downloader.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2912 2023-01-27 21:53:46.000000 jal-2023.4.6/jal/net/helpers.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2040 2023-03-06 11:34:17.000000 jal-2023.4.6/jal/pypi_description.md
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-15 14:24:53.966406 jal-2023.4.6/jal/reports/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2020-12-23 19:03:58.000000 jal-2023.4.6/jal/reports/__init__.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2967 2023-04-14 18:14:21.000000 jal-2023.4.6/jal/reports/category.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    14386 2023-04-14 18:14:21.000000 jal-2023.4.6/jal/reports/deals.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3936 2023-04-14 18:14:21.000000 jal-2023.4.6/jal/reports/holdings.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    14756 2023-04-14 18:14:21.000000 jal-2023.4.6/jal/reports/income_spending.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2855 2023-04-14 18:14:21.000000 jal-2023.4.6/jal/reports/peer.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     8771 2023-04-14 18:14:21.000000 jal-2023.4.6/jal/reports/profit_loss.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3287 2023-02-16 10:22:14.000000 jal-2023.4.6/jal/reports/reports.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2827 2023-04-14 18:14:21.000000 jal-2023.4.6/jal/reports/tag.py
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-15 14:24:53.966406 jal-2023.4.6/jal/ui/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2020-12-23 19:03:58.000000 jal-2023.4.6/jal/ui/__init__.py
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-15 14:24:53.969740 jal-2023.4.6/jal/ui/reports/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)        0 2022-01-13 15:45:51.000000 jal-2023.4.6/jal/ui/reports/__init__.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5179 2023-04-15 14:16:00.000000 jal-2023.4.6/jal/ui/reports/ui_category_report.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4099 2023-04-15 14:16:00.000000 jal-2023.4.6/jal/ui/reports/ui_deals_report.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4159 2023-04-15 14:16:00.000000 jal-2023.4.6/jal/ui/reports/ui_holdings_report.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4156 2023-04-15 14:16:00.000000 jal-2023.4.6/jal/ui/reports/ui_income_spending_report.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5382 2023-04-15 14:16:00.000000 jal-2023.4.6/jal/ui/reports/ui_peer_report.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4687 2023-04-15 14:16:00.000000 jal-2023.4.6/jal/ui/reports/ui_profit_loss_report.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5353 2023-04-15 14:16:00.000000 jal-2023.4.6/jal/ui/reports/ui_tag_report.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4805 2023-04-15 14:16:00.000000 jal-2023.4.6/jal/ui/reports/ui_tax_estimation.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    12742 2023-04-15 14:16:00.000000 jal-2023.4.6/jal/ui/ui_asset_dlg.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4056 2023-04-15 14:16:00.000000 jal-2023.4.6/jal/ui/ui_flow_export_widget.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    14782 2023-04-15 14:16:00.000000 jal-2023.4.6/jal/ui/ui_login_fns_dlg.py
+-rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)     9324 2023-04-15 14:16:00.000000 jal-2023.4.6/jal/ui/ui_main_window.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    14510 2023-04-15 14:16:00.000000 jal-2023.4.6/jal/ui/ui_operations_widget.py
+-rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)     5707 2023-04-15 14:16:00.000000 jal-2023.4.6/jal/ui/ui_rebuild_window.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     7302 2023-04-15 14:16:00.000000 jal-2023.4.6/jal/ui/ui_reference_data_dlg.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2903 2023-04-15 14:16:00.000000 jal-2023.4.6/jal/ui/ui_select_account_dlg.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3253 2023-04-15 14:16:00.000000 jal-2023.4.6/jal/ui/ui_select_reference_dlg.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    16301 2023-04-15 14:16:00.000000 jal-2023.4.6/jal/ui/ui_slip_import_dlg.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     9674 2023-04-15 14:16:00.000000 jal-2023.4.6/jal/ui/ui_tax_export_widget.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4023 2023-04-15 14:16:00.000000 jal-2023.4.6/jal/ui/ui_update_quotes_window.py
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-15 14:24:53.983073 jal-2023.4.6/jal/updates/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2020-12-23 19:03:58.000000 jal-2023.4.6/jal/updates/__init__.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5122 2020-12-21 16:23:10.000000 jal-2023.4.6/jal/updates/jal_delta_10.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    12870 2021-08-18 12:53:40.000000 jal-2023.4.6/jal/updates/jal_delta_11.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    26116 2021-01-13 17:04:46.000000 jal-2023.4.6/jal/updates/jal_delta_12.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    16516 2021-01-30 16:01:43.000000 jal-2023.4.6/jal/updates/jal_delta_13.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    34961 2021-02-27 17:35:02.000000 jal-2023.4.6/jal/updates/jal_delta_14.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2250 2021-02-27 17:35:02.000000 jal-2023.4.6/jal/updates/jal_delta_15.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3630 2021-02-27 17:35:02.000000 jal-2023.4.6/jal/updates/jal_delta_16.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    20912 2021-02-27 17:35:02.000000 jal-2023.4.6/jal/updates/jal_delta_17.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      656 2021-03-07 11:58:53.000000 jal-2023.4.6/jal/updates/jal_delta_18.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      686 2021-03-08 13:39:11.000000 jal-2023.4.6/jal/updates/jal_delta_19.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    13578 2021-03-12 14:26:01.000000 jal-2023.4.6/jal/updates/jal_delta_20.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1428 2021-03-19 12:24:53.000000 jal-2023.4.6/jal/updates/jal_delta_21.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      949 2021-03-22 11:20:31.000000 jal-2023.4.6/jal/updates/jal_delta_22.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    17602 2021-04-08 12:12:36.000000 jal-2023.4.6/jal/updates/jal_delta_23.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      344 2021-04-11 10:57:46.000000 jal-2023.4.6/jal/updates/jal_delta_24.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     8270 2021-04-22 04:11:28.000000 jal-2023.4.6/jal/updates/jal_delta_25.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2492 2021-08-12 19:15:12.000000 jal-2023.4.6/jal/updates/jal_delta_26.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    26325 2022-01-13 05:57:31.000000 jal-2023.4.6/jal/updates/jal_delta_27.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    13276 2022-01-13 06:08:45.000000 jal-2023.4.6/jal/updates/jal_delta_28.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    35370 2022-01-13 15:45:51.000000 jal-2023.4.6/jal/updates/jal_delta_29.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     8671 2022-02-13 13:11:58.000000 jal-2023.4.6/jal/updates/jal_delta_30.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    11413 2022-02-13 11:04:18.000000 jal-2023.4.6/jal/updates/jal_delta_31.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    12545 2022-03-31 14:26:11.000000 jal-2023.4.6/jal/updates/jal_delta_32.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4229 2022-03-31 14:26:11.000000 jal-2023.4.6/jal/updates/jal_delta_33.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2287 2022-04-06 14:47:21.000000 jal-2023.4.6/jal/updates/jal_delta_34.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2858 2022-04-30 20:05:13.000000 jal-2023.4.6/jal/updates/jal_delta_35.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3427 2022-06-19 17:39:33.000000 jal-2023.4.6/jal/updates/jal_delta_36.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3755 2022-07-20 07:00:10.000000 jal-2023.4.6/jal/updates/jal_delta_37.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    21913 2022-08-21 07:15:06.000000 jal-2023.4.6/jal/updates/jal_delta_38.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      343 2023-01-04 13:14:35.000000 jal-2023.4.6/jal/updates/jal_delta_39.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3055 2023-01-27 21:53:46.000000 jal-2023.4.6/jal/updates/jal_delta_40.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    48157 2023-02-07 18:26:24.000000 jal-2023.4.6/jal/updates/jal_delta_41.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2085 2023-02-20 14:55:36.000000 jal-2023.4.6/jal/updates/jal_delta_42.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2528 2023-03-08 16:23:30.000000 jal-2023.4.6/jal/updates/jal_delta_43.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3020 2023-04-07 14:10:37.000000 jal-2023.4.6/jal/updates/jal_delta_44.sql
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-15 14:24:53.986407 jal-2023.4.6/jal/widgets/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2020-12-23 19:03:58.000000 jal-2023.4.6/jal/widgets/__init__.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3912 2023-04-15 09:01:12.000000 jal-2023.4.6/jal/widgets/abstract_operation_details.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6846 2023-04-15 14:13:28.000000 jal-2023.4.6/jal/widgets/account_select.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    14491 2023-04-15 14:13:28.000000 jal-2023.4.6/jal/widgets/asset_dialog.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    11302 2023-04-15 14:13:28.000000 jal-2023.4.6/jal/widgets/corporate_action_widget.py
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-15 14:24:53.986407 jal-2023.4.6/jal/widgets/custom/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)        0 2022-12-24 19:32:40.000000 jal-2023.4.6/jal/widgets/custom/__init__.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4441 2023-04-15 14:13:28.000000 jal-2023.4.6/jal/widgets/custom/date_range_selector.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2015 2023-04-15 14:13:28.000000 jal-2023.4.6/jal/widgets/custom/db_lookup_combobox.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5331 2023-04-14 18:14:21.000000 jal-2023.4.6/jal/widgets/custom/log_viewer.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    13628 2023-04-15 14:13:28.000000 jal-2023.4.6/jal/widgets/delegates.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     9289 2023-04-15 14:13:28.000000 jal-2023.4.6/jal/widgets/dividend_widget.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     8437 2023-04-14 18:14:21.000000 jal-2023.4.6/jal/widgets/helpers.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    12488 2023-04-15 14:13:28.000000 jal-2023.4.6/jal/widgets/income_spending_widget.py
+-rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)    13018 2023-04-14 18:14:21.000000 jal-2023.4.6/jal/widgets/main_window.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3386 2023-04-15 14:13:28.000000 jal-2023.4.6/jal/widgets/mdi.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2854 2022-12-26 13:26:40.000000 jal-2023.4.6/jal/widgets/operations_tabs.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     7159 2023-04-14 18:14:21.000000 jal-2023.4.6/jal/widgets/operations_widget.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6013 2023-04-15 14:13:28.000000 jal-2023.4.6/jal/widgets/price_chart.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5667 2023-04-15 14:13:28.000000 jal-2023.4.6/jal/widgets/qr_scanner.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    11244 2023-04-14 18:14:21.000000 jal-2023.4.6/jal/widgets/reference_data.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    21856 2023-04-15 13:54:08.000000 jal-2023.4.6/jal/widgets/reference_dialogs.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4779 2023-04-15 14:13:28.000000 jal-2023.4.6/jal/widgets/reference_selector.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      632 2022-12-26 08:54:07.000000 jal-2023.4.6/jal/widgets/register_designer_plugins.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3499 2023-04-15 14:14:41.000000 jal-2023.4.6/jal/widgets/selection_dialog.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     7862 2023-04-14 18:14:21.000000 jal-2023.4.6/jal/widgets/tax_widget.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6890 2023-04-15 14:13:28.000000 jal-2023.4.6/jal/widgets/trade_widget.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    10088 2023-04-15 14:13:28.000000 jal-2023.4.6/jal/widgets/transfer_widget.py
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-15 14:24:53.949740 jal-2023.4.6/jal.egg-info/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2726 2023-04-15 14:24:53.000000 jal-2023.4.6/jal.egg-info/PKG-INFO
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5592 2023-04-15 14:24:53.000000 jal-2023.4.6/jal.egg-info/SOURCES.txt
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)        1 2023-04-15 14:24:53.000000 jal-2023.4.6/jal.egg-info/dependency_links.txt
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)       37 2023-04-15 14:24:53.000000 jal-2023.4.6/jal.egg-info/entry_points.txt
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)       67 2023-04-15 14:24:53.000000 jal-2023.4.6/jal.egg-info/requires.txt
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)       10 2023-04-15 14:24:53.000000 jal-2023.4.6/jal.egg-info/top_level.txt
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)       38 2023-04-15 14:24:53.986407 jal-2023.4.6/setup.cfg
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1756 2023-04-14 18:14:21.000000 jal-2023.4.6/setup.py
```

### Comparing `jal-2023.4.5/PKG-INFO` & `jal-2023.4.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jal
-Version: 2023.4.5
+Version: 2023.4.6
 Summary: Just Another Ledger - project to track personal financial records
 Home-page: https://github.com/titov-vv/jal
 Author-email: jal@gmx.ru
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial
 Classifier: Topic :: Office/Business :: Financial :: Accounting
```

### Comparing `jal-2023.4.5/docs/README.md` & `jal-2023.4.6/docs/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 It was designed to keep records of personal incomes/spendings and investments with up-to-date information about account's balances and portfolio value.
 
 ### Support, Feedback
 If you want to ask a question, report a bug, provide help or support an author - you may use email [jal@gmx.ru](mailto:jal@gmx.ru?subject=%5BJAL%5D%20Help) or [Telegram](https://t.me/jal_support) ([Issues](https://github.com/titov-vv/jal/issues) on GitHub are always welcome also).
 
 ### Thanks!
-I would like to a mention people who helped me in 2022 as I got more donations, help and feedback from users this year. 
+I would like to a mention people who helped me in 2022 and 2023 as I got more donations, help and feedback from users this year. 
 And while I can't name every one of them I would like to confirm my appreciation for this help. They did the project better!
 
 ### [FAQ](https://github.com/titov-vv/jal/blob/master/docs/FAQ.md)
 
 ### [Description of error messages](https://github.com/titov-vv/jal/blob/master/docs/error_description.md)
 
 ### Main features
@@ -39,16 +39,14 @@
 Russian tax estimation for open positions.
 - *experimental* Download russian electronic slips from russian tax authority (FNS). This function requires authorization and `pyzbar` package installation for QR recognition.  
 You may authorize via SMS, FNS personal account or ESIA/Gosuslugi. QR code may be scanned from camera, clipboard image or image file on disk.
 - *experimental* Category recognition for goods in electronic slip with help of `tensorflow`
 
 ### Installation
 
-#### *jal* doesn't work with PySide6 6.5.0 yet. Please use 6.4.3 as maximum PySide6 version.
-
 *jal* was created to be portable and cross-platform. Thus, you have several ways to install and run the program:
 - You may get file archive from [the GitHub repository](https://github.com/titov-vv/jal), unpack it into suitable directory on your PC and use `run.py` to start application.
 In order to succeed this way you need to have at least Python 3.8.1 and satisfy all dependencies listed in `requirements.txt`. Let's say some words about installing python on windows-based computers, as this application becomes poplular for non-programming people. The best place to download python distro is official site, sure. Important, in installer dialogues to check boxes for installing `pip` and `Add python to environment variables`. Don't forget to reboot windows to be sure, that changes applies correctly.
 
 - You may use installation package with `pip install jal` command. It will take care about dependencies automatically and will install `jal` entry point<sup>*</sup> to run the program. For windows-users the best and easiest way is to start windows command prompt (cmd) and run command mentioned above in it. If python set up correctly and installation succeeded you may just type `jal` to run application.
 Alternatively you may use `python -m jal.jal` if you can't run application with `jal` entry point.
 - You may mix two methods together - download source files from github and then use `setup.py` for preferred way of installation.
```

### Comparing `jal-2023.4.5/jal/constants.py` & `jal-2023.4.6/jal/constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -148,15 +148,15 @@
     LightGreen = QColor(127, 255, 127)
     LightRed = QColor(255, 127, 127)
     LightYellow = QColor(255, 255, 200)
 
 
 class AssetTypeComboBox(QComboBox):
     def __init__(self, parent=None):
-        QComboBox.__init__(self, parent)
+        super().__init__(parent=parent)
         PredefinedAsset().load2combo(self)
 
     def getKey(self):
         return self.currentData()
 
     def setKey(self, value):
         self.setCurrentIndex(self.findData(value))
```

### Comparing `jal-2023.4.5/jal/data_export/dlsg.py` & `jal-2023.4.6/jal/data_export/dlsg.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/data_export/tax_reports/portugal.json` & `jal-2023.4.6/jal/data_export/tax_reports/portugal.json`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/data_export/tax_reports/portugal.py` & `jal-2023.4.6/jal/data_export/tax_reports/portugal.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/data_export/tax_reports/russia.json` & `jal-2023.4.6/jal/data_export/tax_reports/russia.json`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/data_export/tax_reports/russia.py` & `jal-2023.4.6/jal/data_export/tax_reports/russia.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/data_export/taxes.py` & `jal-2023.4.6/jal/data_export/taxes.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/data_export/taxes_flow.py` & `jal-2023.4.6/jal/data_export/taxes_flow.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/data_export/templates/tax_prt_dividends.json` & `jal-2023.4.6/jal/data_export/templates/tax_prt_dividends.json`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/data_export/templates/tax_prt_shares.json` & `jal-2023.4.6/jal/data_export/templates/tax_prt_shares.json`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/data_export/templates/tax_rus_bonds.json` & `jal-2023.4.6/jal/data_export/templates/tax_rus_bonds.json`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/data_export/templates/tax_rus_corporate_actions.json` & `jal-2023.4.6/jal/data_export/templates/tax_rus_corporate_actions.json`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/data_export/templates/tax_rus_crypto.json` & `jal-2023.4.6/jal/data_export/templates/tax_rus_crypto.json`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/data_export/templates/tax_rus_derivatives.json` & `jal-2023.4.6/jal/data_export/templates/tax_rus_derivatives.json`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/data_export/templates/tax_rus_dividends.json` & `jal-2023.4.6/jal/data_export/templates/tax_rus_dividends.json`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/data_export/templates/tax_rus_fees.json` & `jal-2023.4.6/jal/data_export/templates/tax_rus_fees.json`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/data_export/templates/tax_rus_flow.json` & `jal-2023.4.6/jal/data_export/templates/tax_rus_flow.json`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/data_export/templates/tax_rus_interests.json` & `jal-2023.4.6/jal/data_export/templates/tax_rus_interests.json`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/data_export/templates/tax_rus_trades.json` & `jal-2023.4.6/jal/data_export/templates/tax_rus_trades.json`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/data_export/xlsx.py` & `jal-2023.4.6/jal/data_export/xlsx.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/data_import/broker_statements/ibkr.py` & `jal-2023.4.6/jal/data_import/broker_statements/ibkr.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/data_import/broker_statements/just2trade.py` & `jal-2023.4.6/jal/data_import/broker_statements/just2trade.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/data_import/broker_statements/kit.py` & `jal-2023.4.6/jal/data_import/broker_statements/kit.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/data_import/broker_statements/open_portfolio.py` & `jal-2023.4.6/jal/data_import/broker_statements/open_portfolio.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/data_import/broker_statements/openbroker.py` & `jal-2023.4.6/jal/data_import/broker_statements/openbroker.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/data_import/broker_statements/psb.py` & `jal-2023.4.6/jal/data_import/broker_statements/psb.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/data_import/broker_statements/uralsib.py` & `jal-2023.4.6/jal/data_import/broker_statements/uralsib.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/data_import/category_recognizer.py` & `jal-2023.4.6/jal/data_import/category_recognizer.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/data_import/import_schema.json` & `jal-2023.4.6/jal/data_import/import_schema.json`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/data_import/slips.py` & `jal-2023.4.6/jal/data_import/slips.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
             if col == 4:
                 return self.tr("Amount")
         return None
 
 
 class SlipLinesDelegate(QStyledItemDelegate):
     def __init__(self, parent=None):
-        QStyledItemDelegate.__init__(self, parent)
+        super().__init__(parent=parent)
 
     def paint(self, painter, option, index):
         painter.save()
         pen = painter.pen()
         model = index.model()
         if index.column() == 0:
             text = model.data(index, Qt.DisplayRole)
```

### Comparing `jal-2023.4.5/jal/data_import/slips_tax.py` & `jal-2023.4.6/jal/data_import/slips_tax.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/data_import/statement.py` & `jal-2023.4.6/jal/data_import/statement.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/data_import/statement_xls.py` & `jal-2023.4.6/jal/data_import/statement_xls.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/data_import/statement_xml.py` & `jal-2023.4.6/jal/data_import/statement_xml.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/data_import/statements.py` & `jal-2023.4.6/jal/data_import/statements.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/db/account.py` & `jal-2023.4.6/jal/db/account.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/db/asset.py` & `jal-2023.4.6/jal/db/asset.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/db/backup_restore.py` & `jal-2023.4.6/jal/db/backup_restore.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/db/balances_model.py` & `jal-2023.4.6/jal/db/balances_model.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/db/category.py` & `jal-2023.4.6/jal/db/category.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/db/closed_trade.py` & `jal-2023.4.6/jal/db/closed_trade.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/db/country.py` & `jal-2023.4.6/jal/db/country.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/db/db.py` & `jal-2023.4.6/jal/db/db.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 # ----------------------------------------------------------------------------------------------------------------------
 class JalDB:
     _tables = []
     _instances_with_cache = []
 
     # By default, db objects don't cache data. But if and object may cache db data we need to track it so parameter
     # 'cached' to be set to True. Such objects should implement invalidate_cache(), class_cache() methods also.
-    def __init__(self, cached=None, **kwargs):
+    def __init__(self, cached=False, **kwargs):
         if cached:
             self._instances_with_cache.append(self)
         super().__init__()
 
     def tr(self, text):
         return QApplication.translate("JalDB", text)
 
@@ -129,14 +129,18 @@
         return JalDBError(JalDBError.NoError)
 
     # ------------------------------------------------------------------------------------------------------------------
     # Returns current version of sqlite library
     def get_engine_version(self):
         return self._read("SELECT sqlite_version()")
 
+    # Returns last inserted id
+    def last_insert_id(self):
+        return self._read("SELECT last_insert_rowid()")
+
     # ------------------------------------------------------------------------------------------------------------------
     # This function returns SQLite connection used by JAL or fails with RuntimeError exception
     @staticmethod
     def connection():
         db = QSqlDatabase.database(Setup.DB_CONNECTION)
         if not db.isValid():
             raise RuntimeError(f"DB connection '{Setup.DB_CONNECTION}' is invalid")
@@ -216,20 +220,20 @@
             else:
                 return values
         else:
             return None
 
     # ------------------------------------------------------------------------------------------------------------------
     def invalidate_cache(self):
-        cache_classes = set()   # a list of classes that were already invalidated and don't need extra action
+        processed_cache_classes = set()   # a list of classes that were already invalidated and don't need extra action
         for item in self._instances_with_cache:
-            if item.class_cache() and type(item) in cache_classes:
+            if item.class_cache() and type(item) in processed_cache_classes:
                 continue
             else:
-                cache_classes.add(type(item))
+                processed_cache_classes.add(type(item))
             item.invalidate_cache()
 
     # Method returns true if data are cached on a class level, not in every instance
     @classmethod
     def class_cache(cls) -> True:
         return False
 
@@ -368,17 +372,17 @@
         query_text = query_text[:-2] + ") " + values_text[:-2] + ")"
         query = self._exec(query_text, params, commit=True)
         return query.lastInsertId()
 
 
 # -------------------------------------------------------------------------------------------------------------------
 # Subclassing to hide db connection details
-class JalModel(QSqlTableModel):
+class JalModel(QSqlTableModel, JalDB):
     def __init__(self, parent, table_name):
-        super().__init__(parent=parent, db=JalDB.connection())
+        super().__init__(parent=parent, db=self.connection())
         self.setTable(table_name)
         self._table = table_name
 
     # Returns value of 'field_name' where 'key_field' is equal to 'search_value'
     def get_value(self, field_name: str, key_field: str, search_value: Union[int, str]) -> str:
         if ' ' in field_name or ' ' in key_field:
             return ''
```

### Comparing `jal-2023.4.5/jal/db/helpers.py` & `jal-2023.4.6/jal/db/helpers.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/db/holdings_model.py` & `jal-2023.4.6/jal/db/holdings_model.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/db/ledger.py` & `jal-2023.4.6/jal/db/ledger.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 
 # ===================================================================================================================
 class Ledger(QObject, JalDB):
     updated = Signal()
     SILENT_REBUILD_THRESHOLD = 1000
 
     def __init__(self):
-        QObject.__init__(self)
+        super().__init__()
         self.amounts = LedgerAmounts("amount_acc")    # store last amount for [book, account, asset]
         self.values = LedgerAmounts("value_acc")      # together with corresponding value
         self.main_window = None
         self.progress_bar = None
 
     def setProgressBar(self, main_window, progress_widget):
         self.main_window = main_window
```

### Comparing `jal-2023.4.5/jal/db/operations.py` & `jal-2023.4.6/jal/db/operations.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/db/operations_model.py` & `jal-2023.4.6/jal/db/operations_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,15 +149,15 @@
         self.prepareData()
 
 
 # ----------------------------------------------------------------------------------------------------------------------
 class ColoredAmountsDelegate(QStyledItemDelegate):
     def __init__(self, parent=None):
         self._view = parent
-        QStyledItemDelegate.__init__(self, parent)
+        super().__init__(parent=parent)
 
     def paint(self, painter, option, index):
         painter.save()
         data = index.model().data(index)
         rect = option.rect
         H = rect.height()
         Y = rect.top()
```

### Comparing `jal-2023.4.5/jal/db/peer.py` & `jal-2023.4.6/jal/db/peer.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/db/reference_models.py` & `jal-2023.4.6/jal/db/reference_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 # ----------------------------------------------------------------------------------------------------------------------
 class AbstractReferenceListModel(QSqlRelationalTableModel, JalDB):
     @property
     def completion_model(self):
         return self._completion_model
 
-    def __init__(self, table, parent_view):
+    def __init__(self, table, parent_view, **kwargs):
         self._view = parent_view
         self._table = table
         self._columns = []
         self._deleted_rows = []
         self._default_name = "name"
         self._group_by = None
         self._filter_by = ''
@@ -166,15 +166,15 @@
     ROOT_PID = 0
 
     @property
     def completion_model(self):
         return self._completion_model
 
     def __init__(self, table, parent_view):
-        super().__init__(parent_view)
+        super().__init__(parent=parent_view)
         self._table = table
         self._columns = []
         self._view = parent_view
         self._default_name = "name"
         self._stretch = None
         self._sort_by = None
         self._filter_text = ''
```

### Comparing `jal-2023.4.5/jal/db/settings.py` & `jal-2023.4.6/jal/db/settings.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/db/tax_estimator.py` & `jal-2023.4.6/jal/db/tax_estimator.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/db/view_model.py` & `jal-2023.4.6/jal/db/view_model.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/img/accept.png` & `jal-2023.4.6/jal/img/accept.png`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/img/add.png` & `jal-2023.4.6/jal/img/add.png`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/img/add_child.png` & `jal-2023.4.6/jal/img/add_child.png`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/img/cancel.png` & `jal-2023.4.6/jal/img/cancel.png`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/img/chart.png` & `jal-2023.4.6/jal/img/chart.png`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/img/copy.png` & `jal-2023.4.6/jal/img/copy.png`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/img/delete.png` & `jal-2023.4.6/jal/img/delete.png`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/img/ibkr.png` & `jal-2023.4.6/jal/img/ibkr.png`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/img/j2t.png` & `jal-2023.4.6/jal/img/j2t.png`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/img/jal.png` & `jal-2023.4.6/jal/img/jal.png`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/img/kit.png` & `jal-2023.4.6/jal/img/kit.png`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/img/list.png` & `jal-2023.4.6/jal/img/list.png`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/img/new.png` & `jal-2023.4.6/jal/img/new.png`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/img/open_portfolio.png` & `jal-2023.4.6/jal/img/open_portfolio.png`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/img/openbroker.ico` & `jal-2023.4.6/jal/img/openbroker.ico`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/img/psb.ico` & `jal-2023.4.6/jal/img/psb.ico`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/img/quik.ico` & `jal-2023.4.6/jal/img/quik.ico`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/img/reconcile.png` & `jal-2023.4.6/jal/img/reconcile.png`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/img/remove.png` & `jal-2023.4.6/jal/img/remove.png`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/img/tax.png` & `jal-2023.4.6/jal/img/tax.png`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/img/uralsib.ico` & `jal-2023.4.6/jal/img/uralsib.ico`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/jal.py` & `jal-2023.4.6/jal/jal.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/jal_init.sql` & `jal-2023.4.6/jal/jal_init.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/languages/en.qm` & `jal-2023.4.6/jal/languages/en.qm`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/languages/ru.qm` & `jal-2023.4.6/jal/languages/ru.qm`

 * *Files 1% similar despite different names*

```diff
@@ -1,5434 +1,5473 @@
 00000000: 3cb8 6418 caef 9c95 cd21 1cbf 60a1 bddd  <.d......!..`...
-00000010: a700 0000 0572 755f 5255 4200 0019 d800  .....ru_RUB.....
-00000020: 0000 2300 001b 5100 0000 2300 002f 3f00  ..#...Q...#../?.
-00000030: 0000 2300 012e 9d00 0000 2300 0133 4d00  ..#.......#..3M.
-00000040: 0000 2500 0091 c600 0004 7300 0005 b700  ..%.......s.....
-00000050: 0005 3b00 0008 7800 0005 af00 0134 fe00  ..;...x......4..
-00000060: 0031 0e00 007d 6a00 0031 0e00 0122 7100  .1...}j..1..."q.
-00000070: 0046 3900 0003 7000 0046 3900 00a2 3100  .F9...p..F9...1.
-00000080: 0047 a400 0044 eb00 0048 7200 004d 7e00  .G...D...Hr..M~.
-00000090: 0048 7200 0091 ed00 0048 b700 004d b500  .Hr......H...M..
-000000a0: 0048 b700 0092 4800 004a 7a00 0046 e900  .H....H..Jz..F..
-000000b0: 004a b300 004d ec00 004a b300 0092 f600  .J...M...J......
-000000c0: 004b 1a00 0047 1400 004b 3a00 0047 3f00  .K...G...K:..G?.
-000000d0: 004c b200 004e 2300 004c b200 0093 6200  .L...N#..L....b.
-000000e0: 004c b500 0012 eb00 004c b500 012f a100  .L.......L.../..
-000000f0: 0050 7e00 004e 5a00 0050 7e00 0094 0b00  .P~..NZ..P~.....
-00000100: 0051 3100 001e 0b00 0051 3100 0030 b000  .Q1......Q1..0..
-00000110: 0051 bc00 004e 9100 0051 bc00 0094 3800  .Q...N...Q....8.
-00000120: 0051 be00 004e c800 0051 be00 0094 6500  .Q...N...Q....e.
-00000130: 0052 ac00 0095 7300 0052 ac00 0097 cc00  .R....s..R......
-00000140: 0053 3c00 0014 4f00 0053 3c00 0035 f500  .S<...O..S<..5..
-00000150: 0053 8200 004e ff00 0053 8200 0094 9200  .S...N...S......
-00000160: 0053 8900 004f 3600 0053 8900 0094 bf00  .S...O6..S......
-00000170: 0055 6600 004f 6d00 0055 6600 0095 1900  .Uf..Om..Uf.....
-00000180: 0055 a400 004f a400 0055 a400 0095 4600  .U...O...U....F.
-00000190: 0058 b900 0014 b600 0058 b900 001f 8a00  .X.......X......
-000001a0: 0058 b900 0036 5400 0058 b900 00a9 4300  .X...6T..X....C.
-000001b0: 0058 b900 011e 7900 0058 b900 0130 3500  .X....y..X...05.
-000001c0: 0059 c000 004f db00 0059 c000 0096 6a00  .Y...O...Y....j.
-000001d0: 005a 7700 002a fb00 005a 7700 0089 0900  .Zw..*...Zw.....
-000001e0: 005a 7700 0118 7c00 005a 8800 0032 2500  .Zw...|..Z...2%.
-000001f0: 005b 2a00 0026 9700 0070 7c00 005c f900  .[*..&...p|..\..
-00000200: 047a 6e00 0005 4000 047a 6e00 0117 5e00  .zn...@..zn...^.
-00000210: 0498 9800 008e 5400 04a6 7900 0084 9000  ......T...y.....
-00000220: 04a8 a500 000d 3100 04a8 a500 009f 5200  ......1.......R.
-00000230: 04a8 a500 011d c900 04a8 d300 0090 c500  ................
-00000240: 04cb c300 0093 8f00 04cf 3a00 0034 ea00  ..........:..4..
-00000250: 04d9 5d00 0134 9e00 04e3 1a00 0074 de00  ..]..4.......t..
-00000260: 04e7 de00 000a 3900 04e7 de00 000b a100  ......9.........
-00000270: 0504 cf00 0078 1100 0528 a400 0035 1a00  .....x...(...5..
-00000280: 0548 3500 0006 1b00 0548 3500 000a 6800  .H5......H5...h.
-00000290: 0548 3500 0010 ed00 0548 3500 008d 8a00  .H5......H5.....
-000002a0: 0556 a500 0013 2400 0556 a500 001e 3e00  .V....$..V....>.
-000002b0: 0556 a500 002a c600 0556 a500 0031 2100  .V...*...V...1!.
-000002c0: 0556 a500 0054 6300 0556 a500 012f d400  .V...Tc..V.../..
-000002d0: 0556 a500 0134 c700 0565 c000 0042 f800  .V...4...e...B..
-000002e0: 0566 be00 0035 bb00 0566 be00 011d fb00  .f...5...f......
-000002f0: 056b c200 0056 1200 05a3 0000 004b 0300  .k...V.......K..
-00000300: 05a7 aa00 0119 5f00 05a7 e300 011b 6f00  ......_.......o.
-00000310: 05b3 d800 011c 9800 05c0 6500 0020 cf00  ..........e.. ..
-00000320: 05c0 6500 0032 5500 05db bb00 0026 c600  ..e..2U......&..
-00000330: 05fb 8200 0026 fc00 1530 3000 0011 6600  .....&...00...f.
-00000340: 18d1 5000 00ed dd00 2311 0000 0122 4400  ..P.....#...."D.
-00000350: 26f2 9100 004b 2f00 2aa8 a100 0057 c100  &....K/.*....W..
-00000360: 2acf 0400 0057 f700 2b37 fe00 0058 9d00  *....W..+7...X..
-00000370: 2b76 1e00 0085 5f00 2ba7 e300 005a a100  +v...._.+....Z..
-00000380: 2ec7 e000 0044 8a00 3153 c400 0093 c700  .....D..1S......
-00000390: 3d1a 0e00 005c 5400 4182 8900 00fe dc00  =....\T.A.......
-000003a0: 4796 c400 0077 9200 47af 8000 009b 6100  G....w..G.....a.
-000003b0: 48a9 c400 0006 db00 48a9 c400 0011 b600  H.......H.......
-000003c0: 48a9 c400 001c 0600 48a9 c400 0028 c000  H.......H....(..
-000003d0: 48a9 c400 002f 9700 48a9 c400 009e ed00  H..../..H.......
-000003e0: 48a9 c400 00a9 1300 48a9 c400 012e ef00  H.......H.......
-000003f0: 48a9 c400 0133 a600 4964 b300 008f c100  H....3..Id......
-00000400: 4988 b300 008e 1a00 4a2b 8200 0045 f300  I.......J+...E..
-00000410: 4a36 9500 0029 6f00 4a36 9500 0046 2a00  J6...)o.J6...F*.
-00000420: 4a36 9500 0073 ea00 4a71 ec00 0024 5d00  J6...s..Jq...$].
-00000430: 4ab8 3300 0028 0000 4b6b 9000 0103 7f00  J.3..(..Kk......
-00000440: 4d68 c800 0090 f500 4d96 0a00 0025 0b00  Mh......M....%..
-00000450: 4dc4 b300 0091 2a00 4e7e 1a00 0008 0a00  M.....*.N~......
-00000460: 522b 5a00 0074 2000 52e9 5500 0014 0500  R+Z..t .R.U.....
-00000470: 5308 d400 0095 d600 535d fe00 0075 0d00  S.......S]...u..
-00000480: 5464 c900 0091 5d00 5464 c900 0094 ec00  Td....].Td......
-00000490: 5465 a800 0025 3a00 5483 8a00 0008 3900  Te...%:.T.....9.
-000004a0: 556a c300 0082 ae00 55da be00 0011 2f00  Uj......U...../.
-000004b0: 56bc 5a00 0049 be00 56bc 5a00 008c 7900  V.Z..I..V.Z...y.
-000004c0: 56bc 9300 008a 9900 578f 9500 0031 5800  V.......W....1X.
-000004d0: 578f 9500 0130 0800 57a1 7200 0026 5200  W....0..W.r..&R.
-000004e0: 5839 2400 006a 5900 58c6 a500 009f 8200  X9$..jY.X.......
-000004f0: 5948 5c00 0050 1200 5948 5c00 011c cc00  YH\..P..YH\.....
-00000500: 5a73 0400 0019 7600 5a73 0400 0020 4500  Zs....v.Zs... E.
-00000510: 5a79 2700 011b 3900 5a8a e000 011e e600  Zy'...9.Z.......
-00000520: 5a8b c000 002e 9a00 5a8e c300 0096 9700  Z.......Z.......
-00000530: 5a8e c300 012b 8200 5b6a 7c00 000c 7200  Z....+..[j|...r.
-00000540: 5b6a 7c00 0096 cc00 5c06 8a00 004b b900  [j|.....\....K..
-00000550: 5c83 b500 0034 1800 5c83 b500 0036 bd00  \....4..\....6..
-00000560: 5fb8 5a00 0080 8400 5fb8 5a00 012c e600  _.Z....._.Z..,..
-00000570: 602e 0a00 0055 b000 67f7 0000 00f7 2c00  `....U..g.....,.
-00000580: 70c5 c000 00c7 b300 80a8 e500 0048 fa00  p............H..
-00000590: 81bc 0000 00cd 9c00 918d 3700 003b 6c00  ..........7..;l.
-000005a0: 931f 2000 00d9 0b00 9472 3000 006f 9200  .. ......r0..o..
-000005b0: 9688 5400 00d3 ee00 ab81 4000 0115 7100  ..T.......@...q.
-000005c0: af00 f000 00b5 7200 af26 4500 0122 c800  ......r..&E.."..
-000005d0: b27d 9f00 0078 a700 b4d0 c500 0029 0500  .}...x.......)..
-000005e0: b643 0000 00c2 3800 c9db ba00 0062 5600  .C....8......bV.
-000005f0: cfb0 f400 0030 3d00 e1f3 f000 0016 b900  .....0=.........
-00000600: e25b 3000 002c 2500 ed2c 2500 0027 2c00  .[0..,%..,%..',.
-00000610: fbe4 b100 0047 6a00 ff6b fe00 00b2 b001  .....Gj..k......
-00000620: 11c0 6000 0137 3601 2273 8300 008d c801  ..`..76."s......
-00000630: 24a2 9700 003c 2301 2bca d000 009d d601  $....<#.+.......
-00000640: 3502 c000 00c4 0701 473b 2300 0070 8301  5.......G;#..p..
-00000650: 5567 7000 00cc f501 59b4 9000 001a 3901  Ugp.....Y.....9.
-00000660: 6654 9000 003a 6301 7248 d000 0035 5401  fT...:c.rH...5T.
-00000670: 776d e000 00d5 0e01 78c3 f500 0030 dc01  wm......x....0..
-00000680: 7e51 ea00 0129 3701 873b 2300 0070 b501  ~Q...)7..;#..p..
-00000690: 887c d300 005d 2501 9687 c000 010a 6801  .|...]%.......h.
-000006a0: 98a7 5300 004b e801 a469 f900 0101 7801  ..S..K...i....x.
-000006b0: a885 4000 0132 7101 aff7 3300 0000 0001  ..@..2q...3.....
-000006c0: bef6 7000 00d2 0c01 c26a 9a00 00a2 6601  ..p......j....f.
-000006d0: ce0a 1200 008b 8201 d48e 5000 0042 5401  ..........P..BT.
-000006e0: da69 b000 0114 0001 e128 5000 00bf 3e01  .i.......(P...>.
-000006f0: e26a 9a00 0004 2801 f571 7000 00bc 4d02  .j....(..qp...M.
-00000700: 00dd 0100 0043 9602 01b8 4900 0039 b902  .....C....I..9..
-00000710: 01b8 4900 0087 be02 01b8 4900 00a1 f102  ..I.......I.....
-00000720: 01b8 4900 0136 5e02 24d1 2000 00de c302  ..I..6^.$. .....
-00000730: 2b24 6500 012c 4402 36c0 e700 006c 9f02  +$e..,D.6....l..
-00000740: 38ab b000 00af 4102 488e 8300 0125 8302  8.....A.H....%..
-00000750: 5442 2f00 0021 6902 6b41 b400 012d 1102  TB/..!i.kA...-..
-00000760: 705b 1000 005f a302 75ac 0500 00d7 5b02  p[..._..u.....[.
-00000770: 76e6 2500 0043 2902 80f4 7400 005b 1902  v.%..C)...t..[..
-00000780: 83cb 1900 00ac 4302 84df 6000 000c 3702  ......C...`...7.
-00000790: 86cb d700 00ad d002 960b 0000 0102 a502  ................
-000007a0: 9d24 b400 00be db02 a013 f300 00d3 9302  .$..............
-000007b0: b6bc 9300 0059 1702 b827 6100 00a4 2c02  .....Y...'a...,.
-000007c0: c4de 6000 00c8 4102 d6b9 7000 00df 9e02  ..`...A...p.....
-000007d0: d6b9 7000 00eb 8a02 d6b9 7000 0101 fc02  ..p.......p.....
-000007e0: d6b9 7000 010c c802 da2f f000 00ba 7702  ..p....../....w.
-000007f0: db87 a000 00f2 1d02 ddd8 9000 0017 f302  ................
-00000800: e4ef 0400 001f c302 e60b 0000 0077 1502  .............w..
-00000810: ecb9 d000 006d 9b03 0055 4a00 0128 a003  .....m...UJ..(..
-00000820: 0ae6 8700 0017 5e03 0ae6 8700 001c e603  ......^.........
-00000830: 0b8a 5a00 007a 2203 1108 9c00 012f 1803  ..Z..z"....../..
-00000840: 1638 c400 0096 1e03 1684 be00 001c 3903  .8............9.
-00000850: 2221 4000 00ae b803 232f f000 00f3 6403  "!@.....#/....d.
-00000860: 232f f000 0108 0303 3500 5a00 0087 7203  #/......5.Z...r.
-00000870: 3f3c 8400 0110 7903 55cb 1a00 0075 7903  ?<....y.U....uy.
-00000880: 57fa 2e00 0074 6703 5dae f000 0108 b203  W....tg.].......
-00000890: 5dce f000 00e3 3703 6b8b d900 0124 5e03  ].....7.k....$^.
-000008a0: 7321 8300 010f 5d03 82a1 0000 00df cf03  s!....].........
-000008b0: 8a06 2000 00ff 4c03 8b39 a000 0103 e703  .. ...L..9......
-000008c0: 8b60 e400 003e e403 8c34 6500 0025 f903  .`...>...4e..%..
-000008d0: 8f4e c000 0113 3903 9100 d000 005e ab03  .N....9......^..
-000008e0: 97c9 0000 0120 3b03 b023 a000 00b9 2803  ..... ;..#....(.
-000008f0: cafd 4000 0082 e703 d07e 2400 0068 7b03  ..@......~$..h{.
-00000900: d1c2 7400 0040 be03 d1e5 2200 0005 7103  ..t..@...."...q.
-00000910: da9c f300 005a d303 ec0c f700 003c e903  .....Z.......<..
-00000920: f69b 8000 00c6 6104 0029 e000 0123 a904  ......a..)...#..
-00000930: 09f4 0a00 00bb d904 11d2 4900 000c a304  ..........I.....
-00000940: 11d2 a900 0057 3004 1263 4400 00b5 2404  .....W0..cD...$.
-00000950: 1564 8e00 0028 8604 15b4 7000 0137 af04  .d...(....p..7..
-00000960: 195c b000 0116 c704 2e61 f000 0072 9d04  .\.......a...r..
-00000970: 449a c000 012a 9004 56c0 a000 00b6 fc04  D....*..V.......
-00000980: 62c1 c000 00fe 5104 66ac 6500 0135 6004  b.....Q.f.e..5`.
-00000990: 7914 8000 00d0 a704 7d16 7000 006e 7704  y.......}.p..nw.
-000009a0: 846c 5400 002a 5a04 846c 5400 0082 0b04  .lT..*Z..lT.....
-000009b0: 846c 5400 0088 4204 846c 5400 0133 7304  .lT...B..lT..3s.
-000009c0: 8a9c b300 0009 4004 8a9c b300 0092 1a04  ......@.........
-000009d0: 8c2d c700 0064 c104 8c2d c700 007b a004  .-...d...-...{..
-000009e0: 8e23 4000 0000 c004 8e23 4000 001f 0f04  .#@......#@.....
-000009f0: 8e23 4000 0055 3604 983c 8100 0045 bf04  .#@..U6..<...E..
-00000a00: 9849 bc00 0007 6104 9e16 8200 0101 3904  .I....a.......9.
-00000a10: 9e84 d500 0092 7504 a577 1f00 0066 a804  ......u..w...f..
-00000a20: a5e2 3000 0098 e004 ac2c a500 0085 2604  ..0......,....&.
-00000a30: ac2c a500 00a3 f004 bebd 0000 00a7 6b04  .,............k.
-00000a40: c840 f000 00e9 0804 c840 f000 00ec 4304  .@.......@....C.
-00000a50: c840 f000 010e 0004 cc5c 9400 0027 7a04  .@.......\...'z.
-00000a60: cf4d c200 00f7 b304 d7d5 4000 00ca f604  .M........@.....
-00000a70: dd34 9000 0014 eb04 ee54 4000 010b 6804  .4.......T@...h.
-00000a80: f6d3 c900 00d3 2c05 079c 7300 0120 c905  ......,...s.. ..
-00000a90: 161e a000 00b4 af05 2caa 5000 00b3 0d05  ........,.P.....
-00000aa0: 2cde 2300 00a4 8405 304c 6a00 0048 c405  ,.#.....0Lj..H..
-00000ab0: 33ee 2500 0014 7e05 33ee 2500 0036 2005  3.%...~.3.%..6 .
-00000ac0: 3c8d c200 0017 9d05 3c8d c200 001d b305  <.......<.......
-00000ad0: 3d7b 7000 00e8 a305 3d7b 7000 00eb de05  ={p.....={p.....
-00000ae0: 3d7b 7000 0103 1a05 3d7b 7000 010d 1d05  ={p.....={p.....
-00000af0: 49ee 8900 0067 e105 4e5b d400 0115 bf05  I....g..N[......
-00000b00: 5305 de00 0075 c705 5316 ce00 0074 a605  S....u..S....t..
-00000b10: 633f 7000 00e4 9105 6945 5000 00c5 1505  c?p.....iEP.....
-00000b20: 6bc4 2700 008a 5805 6bcd a500 00b0 d805  k.'...X.k.......
-00000b30: 6c90 5400 0095 a005 6ccc 4300 004a 9e05  l.T.....l.C..J..
-00000b40: 6edf f400 008d 1405 6fe5 c000 00f2 cf05  n.......o.......
-00000b50: 802f 5e00 00b0 0c05 812d 6000 0100 dc05  ./^......-`.....
-00000b60: 88a7 e000 011e ae05 88a8 c000 004c f305  .............L..
-00000b70: 8c6a c300 009e b005 8c6a c300 0118 0805  .j.......j......
-00000b80: 8cbc 8e00 004a 6805 98ab 6e00 008d 5605  .....Jh...n...V.
-00000b90: 9ca9 f100 0038 4505 9dfd c000 00a6 eb05  .....8E.........
-00000ba0: 9e88 c300 0091 9205 a661 8700 004d 2805  .........a...M(.
-00000bb0: a661 8700 0050 9505 a661 8700 0051 3f05  .a...P...a...Q?.
-00000bc0: a7f1 8700 0054 0d05 adfb 2800 009f bd05  .....T....(.....
-00000bd0: b039 5c00 000a a705 b039 5c00 0118 4505  .9\......9\...E.
-00000be0: b093 0000 00c6 ef05 b247 c400 009b 0705  .........G......
-00000bf0: c068 c000 0008 d305 c1f8 2200 008c b905  .h........".....
-00000c00: ced0 2500 00d7 d105 d5fa e400 007f 8e05  ..%.............
-00000c10: d5fa e400 0128 f005 da03 6e00 005c b405  .....(....n..\..
-00000c20: dce3 0000 00d0 2d05 dce3 0000 0100 6305  ......-.......c.
-00000c30: dde3 7900 005f cd05 e1ed 8400 00bd 3a05  ..y.._........:.
-00000c40: ecff 1900 00eb 1905 f264 ba00 0046 5f05  .........d...F_.
-00000c50: f662 ea00 00bb 6405 facb 8300 008f fc06  .b....d.........
-00000c60: 0826 4000 00d5 aa06 08e3 9400 007a b806  .&@..........z..
-00000c70: 0ab9 9000 00e1 9106 129d e000 00de 5206  ..............R.
-00000c80: 148d a400 0021 0306 1867 1e00 0099 2a06  .....!...g....*.
-00000c90: 215f 7400 0062 0306 2b00 1300 0037 2906  !_t..b..+....7).
-00000ca0: 2b00 1300 0037 b906 2b00 1300 0039 3606  +....7..+....96.
-00000cb0: 34af 4a00 0009 0306 3500 0f00 006b 3206  4.J.....5....k2.
-00000cc0: 3c17 4000 00db aa06 3c17 4000 00e7 6606  <.@.....<.@...f.
-00000cd0: 3c17 4000 00f9 9c06 3c17 4000 0112 e906  <.@.....<.@.....
-00000ce0: 3cee 8400 00aa f706 468c a000 00af a206  <.......F.......
-00000cf0: 4e38 c500 00a0 5e06 4f34 c000 010f db06  N8....^.O4......
-00000d00: 53a5 f500 004a 3306 580f ce00 0029 aa06  S....J3.X....)..
-00000d10: 5a60 a900 00f8 0406 6318 9000 00e5 a506  Z`......c.......
-00000d20: 68ee 6400 001b b706 69a9 8400 00a2 af06  h.d.....i.......
-00000d30: 69b7 0200 0127 f106 70e2 d000 006e ce06  i....'..p....n..
-00000d40: 7cd1 c500 0049 4e06 7f33 4700 0031 d906  |....IN..3G..1..
-00000d50: 8786 ea00 00a1 9006 88a1 2400 0134 1206  ..........$..4..
-00000d60: 8f30 5000 011c fc06 9b5a 7700 0118 de06  .0P......Zw.....
-00000d70: 9bb8 0c00 0038 0006 9c50 2000 00c3 5506  .....8...P ...U.
-00000d80: 9fb2 5300 00fd 8a06 a6d5 8300 012b b106  ..S..........+..
-00000d90: a8dd 9c00 0052 3306 aef9 ce00 0059 9606  .....R3......Y..
-00000da0: afe6 3000 0071 c906 b017 2200 00a0 ff06  ..0..q....".....
-00000db0: b8bb 6000 00a7 ec06 c10c 6000 00ce 2806  ..`.......`...(.
-00000dc0: c215 0a00 0007 1a06 c227 5a00 0028 3706  .........'Z..(7.
-00000dd0: c5bd 6a00 0124 2a06 ce8a a100 004b 7006  ..j..$*......Kp.
-00000de0: cf70 9900 0024 2206 d08b 2a00 00c8 f306  .p...$"...*.....
-00000df0: d81c 2e00 00d8 3c06 dbaf 2000 00ef 4406  ......<... ...D.
-00000e00: e231 4000 012b 0706 e6c0 4c00 0052 9807  .1@..+....L..R..
-00000e10: 0120 6600 0020 1307 0140 6600 0019 1007  . f.. ...@f.....
-00000e20: 0923 2000 0061 1007 0ac3 fa00 00a1 5207  .# ..a........R.
-00000e30: 0e35 d000 00db 4a07 126c 4400 0138 3007  .5....J..lD..80.
-00000e40: 1d24 9000 0104 fc07 1db9 0500 0012 a007  .$..............
-00000e50: 3389 e000 00b6 3807 3c71 f700 000e 9207  3.....8.<q......
-00000e60: 449d 1f00 00bd 9f07 47cf 0400 003f e607  D.......G....?..
-00000e70: 4bcf e000 00e7 b607 5cec 7500 00a0 1a07  K.......\.u.....
-00000e80: 62f5 3500 003f 6d07 65e8 b400 007e 3c07  b.5..?m.e....~<.
-00000e90: 65e8 b400 0127 4f07 6c21 5400 000b 2207  e....'O.l!T...".
-00000ea0: 7e9b 0500 00e6 b707 9a56 2000 006f ed07  ~........V ..o..
-00000eb0: 9a6c 1400 000b d107 9a6c 1400 001b 7e07  .l.......l....~.
-00000ec0: 9a6c 1400 002f 6507 9a6c 1400 0051 fb07  .l.../e..l...Q..
-00000ed0: 9a6c 1400 0081 d807 9a6c 1400 012e c007  .l.......l......
-00000ee0: 9aa9 6000 00cb 8e07 9db4 9000 00b8 c107  ..`.............
-00000ef0: 9db4 9000 00fd 1607 9e2e 7300 0135 fd07  ..........s..5..
-00000f00: a121 8000 0022 1607 a674 8700 00a3 0207  .!..."...t......
-00000f10: bdfe de00 002c c607 cf9a 7000 00fb 3607  .....,....p...6.
-00000f20: d231 3400 0003 9f07 daae 0000 0104 8f07  .14.............
-00000f30: dae0 ea00 011b ed07 e0a9 5000 000d cd07  ..........P.....
-00000f40: e0a9 5000 0089 9907 e0a9 5000 0119 f507  ..P.......P.....
-00000f50: ebd7 9e00 00aa 1a07 ebd7 9e00 00ad 0507  ................
-00000f60: ec42 a500 0009 f107 ed5c 8000 0112 0807  .B.......\......
-00000f70: f3d4 e000 00c9 e807 f714 e400 00f8 8508  ................
-00000f80: 0291 0000 0080 b508 08a7 9000 00c4 9008  ................
-00000f90: 1f02 9000 00b5 d808 283b 1400 00fd e108  ........(;......
-00000fa0: 284d 4300 0083 fc08 28e8 e000 00ef fb08  (MC.....(.......
-00000fb0: 2a45 4a00 00a3 4d08 2fe7 9000 009d 5e08  *EJ...M./.....^.
-00000fc0: 3267 1100 0007 cc08 41da 6e00 0085 b408  2g......A.n.....
-00000fd0: 46c5 3a00 0045 2008 4d37 c500 0092 b108  F.:..E .M7......
-00000fe0: 4e6b 2a00 0046 a708 4ef9 1500 005c 1e08  Nk*..F..N....\..
-00000ff0: 6186 7000 0070 e708 6c71 e200 00ac a608  a.p..p..lq......
-00001000: 6f32 c000 00d9 cc08 700d f000 00fa af08  o2......p.......
-00001010: 70b2 8b00 0076 5408 7219 0f00 0089 d008  p....vT.r.......
-00001020: 7a4a 5000 0079 4e08 8284 d500 000c 0208  zJP..yN.........
-00001030: 8284 d500 0082 3f08 8599 7200 0135 2708  ......?...r..5'.
-00001040: 8958 2900 012a 3708 8b87 0000 00d1 6408  .X)..*7.......d.
-00001050: 8fa4 9300 000f c508 8fa4 9300 0086 0208  ................
-00001060: 8fa4 9300 008b fe08 8fa4 9300 0118 a608  ................
-00001070: 9a98 b400 0019 f408 9c61 5e00 011c 4808  .........a^...H.
-00001080: a1a4 9300 0058 d708 a63b 3000 010d 8308  .....X...;0.....
-00001090: aa82 f400 005a 6808 abe2 0900 002a 8b08  .....Zh......*..
-000010a0: abe2 0900 0088 7708 af11 d500 0062 db08  ......w......b..
-000010b0: b89a 9200 0025 be08 bbfe c500 0002 ac08  .....%..........
-000010c0: bbfe c500 0125 3408 bd8a 6000 0116 3d08  .....%4...`...=.
-000010d0: c000 5000 0097 8708 c000 5000 0098 4a08  ..P.......P...J.
-000010e0: c272 0900 0010 0208 c76b 0300 0059 dd08  .r.......k...Y..
-000010f0: cd7c e400 00a9 aa09 00f9 a400 0003 e009  .|..............
-00001100: 162e f000 003a f209 1afc d400 003d a309  .....:.......=..
-00001110: 1fb9 f500 0075 f909 2254 0000 011f dc09  .....u.."T......
-00001120: 2e57 df00 00a5 d209 35e6 6000 0048 8109  .W......5.`..H..
-00001130: 3b85 e000 006c 1109 4459 d000 00e1 0009  ;....l..DY......
-00001140: 4d67 fe00 0117 c809 5962 c900 00e6 f609  Mg......Yb......
-00001150: 5aa4 1000 00b9 c509 5b68 f000 005e 3109  Z.......[h...^1.
-00001160: 5c07 3000 00ee 9509 5ca2 3000 0130 a809  \.0.....\.0..0..
-00001170: 5d03 9000 011e 3909 6302 2500 0135 cd09  ].....9.c.%..5..
-00001180: 667a 9000 00ec cc09 66cc c900 0033 dd09  fz......f....3..
-00001190: 700b c500 0011 fb09 7a29 6900 000f 4509  p.......z)i...E.
-000011a0: 8c00 0a00 0050 4f09 8c81 5e00 0039 7709  .....PO...^..9w.
-000011b0: 8c81 5e00 0050 f109 8c81 5e00 0098 0009  ..^..P....^.....
-000011c0: 8d04 b300 008f 3309 95cb c400 00d6 ee09  ......3.........
-000011d0: a6af c300 0056 b909 a6c1 0a00 0027 c809  .....V.......'..
-000011e0: a6c1 0a00 0044 b709 a6c1 0a00 0083 2809  .....D........(.
-000011f0: a6c1 0a00 0097 4a09 a6c1 0a00 0122 9809  ......J......"..
-00001200: a6c1 c300 0004 6f09 a87a 8000 00f9 f309  ......o..z......
-00001210: b56b a200 008c 3709 b889 ea00 0086 db09  .k....7.........
-00001220: b889 ea00 00a5 3809 cf34 f000 00e0 6b09  ......8..4....k.
-00001230: d82d 3f00 0083 5f09 dbfe c000 00da 8b0a  .-?..._.........
-00001240: 074b 5000 0072 300a 159b 8000 001e 7c0a  .KP..r0.......|.
-00001250: 159b 8000 0054 a40a 17d3 5000 00cc 4c0a  .....T....P...L.
-00001260: 20b0 6000 0078 480a 20fc 9000 00b3 f10a   .`..xH. .......
-00001270: 22d2 d000 00e5 100a 2aef e000 00fb c10a  ".......*.......
-00001280: 2e99 7e00 0056 f10a 30f6 b500 002a 020a  ..~..V..0....*..
-00001290: 338b 1000 00dd d10a 3f0e 9500 0080 3d0a  3.......?.....=.
-000012a0: 3f0e 9500 0129 f60a 4985 3000 0071 550a  ?....)..I.0..qU.
-000012b0: 4cb2 e000 00b7 7c0a 5e50 b000 010a f10a  L.....|.^P......
-000012c0: 62cd 3400 0034 960a 64c8 9500 0086 9f0a  b.4..4..d.......
-000012d0: 65e3 f000 005d 760a 6c11 b300 0005 040a  e....]v.l.......
-000012e0: 6c5b d900 0009 840a 6c5b d900 000b 6a0a  l[......l[....j.
-000012f0: 6c89 9300 0135 900a 70ea 0000 0044 1c0a  l....5..p....D..
-00001300: 8170 8e00 0131 7f0a 84e6 b500 001c 9f0a  .p...1..........
-00001310: 84e6 b500 002f fd0a 84e6 b500 0053 040a  ...../.......S..
-00001320: 84e6 b500 012f 640a 84e6 b500 0133 d20a  ...../d......3..
-00001330: 89ad 3000 00f5 ca0a 89ad 3000 010c 2a0a  ..0.......0...*.
-00001340: 8c5e f000 0065 f90a 954c 2000 00db fb0a  .^...e...L .....
-00001350: 9989 6300 0073 980a ac8c c000 00f9 230a  ..c..s........#.
-00001360: ae3e fa00 0075 3f0a b4bc 2e00 002e ca0a  .>...u?.........
-00001370: b5ff 6400 00b1 700a b6d5 d000 00d2 8c0a  ..d...p.........
-00001380: ba90 7000 00e8 240a be20 4a00 0010 480a  ..p...$.. J...H.
-00001390: c25d 1400 0041 7f0a c945 a000 00b3 640a  .]...A...E....d.
-000013a0: ca80 7300 0053 4a0a cf76 b400 0058 2b0a  ..s..SJ..v...X+.
-000013b0: cfef 4000 0107 6f0a e1b0 da00 00a8 4d0a  ..@...o.......M.
-000013c0: e1b4 8000 0114 6d0a e45f d000 00b8 3a0a  ......m.._....:.
-000013d0: eb63 2000 0022 b30a ee50 6000 0081 6d0a  .c .."...P`...m.
-000013e0: f3de 9e00 0084 cd0a f818 8000 00b7 b50a  ................
-000013f0: f818 8000 00fc 840b 0396 6300 0008 9e0b  ..........c.....
-00001400: 03f9 7300 008e e90b 0476 b400 0058 650b  ..s......v...Xe.
-00001410: 0ac1 5a00 0129 8c0b 139f b500 0087 130b  ..Z..)..........
-00001420: 19b8 d700 008a d70b 1b90 b000 0102 2c0b  ..............,.
-00001430: 1fcd 0500 00a0 bb0b 20ce b000 00c2 c30b  ........ .......
-00001440: 2371 ce00 0001 3e0b 244d 8300 0106 4b0b  #q....>.$M....K.
-00001450: 296c c900 0073 290b 2d80 be00 000e f30b  )l...s).-.......
-00001460: 2d80 be00 008b 340b 2d80 be00 011a 7c0b  -.....4.-.....|.
-00001470: 2fa8 e400 0130 640b 4000 a500 0064 3e0b  /....0d.@....d>.
-00001480: 440d ae00 005a 160b 47ce c400 00ea 040b  D....Z..G.......
-00001490: 4841 e400 00bc d40b 4e26 9900 0010 8e0b  HA......N&......
-000014a0: 543a f400 00e2 340b 5467 9000 002b 290b  T:....4.Tg...+).
-000014b0: 6948 d000 00c5 af0b 6b4e 3000 005f 140b  iH......kN0.._..
-000014c0: 6f1b 4500 0061 790b 76dd 9d00 0134 5d0b  o.E..ay.v....4].
-000014d0: 8a1a 2000 00e3 cb0b 8a1a 2000 0111 b50b  .. ....... .....
-000014e0: 8c6a e300 0059 580b 9253 4000 0002 280b  .j...YX..S@...(.
-000014f0: 94b6 5e00 00cf 750b 967b 5400 0031 880b  ..^...u..{T..1..
-00001500: a0c9 de00 0006 5c0b a3fc 7000 00f1 a30b  ......\...p.....
-00001510: a4a2 2500 0024 950b c474 9000 00dc 970b  ..%..$...t......
-00001520: c4a6 f000 0063 c90b c81a a000 00dd 360b  .....c........6.
-00001530: cbf1 c000 00e4 1e0b cbf1 c000 00e9 910b  ................
-00001540: cbf1 c000 00f4 190b cbf1 c000 0109 f40b  ................
-00001550: db2b b200 0025 6f0b def4 0000 012d ad0b  .+...%o......-..
-00001560: e203 8700 000e 4b0b e217 6300 000e 080b  ......K...c.....
-00001570: e4a0 3000 0015 f10b f39a 4000 0039 fa0b  ..0.......@..9..
-00001580: f39a 4000 0080 fe0b f39a 4000 00c9 760b  ..@.......@...v.
-00001590: fc32 3300 0045 550c 04fe c500 0013 620c  .23..EU.......b.
-000015a0: 0c17 6300 0057 7f0c 0ce3 2300 008e 930c  ..c..W....#.....
-000015b0: 0dec 5a00 007f db0c 1cdb 4200 010e 8a0c  ..Z.......B.....
-000015c0: 1d95 4000 00c0 f00c 3834 1400 000d 670c  ..@.....84....g.
-000015d0: 3834 1400 0089 370c 3834 1400 0119 930c  84....7.84......
-000015e0: 5256 ae00 0033 9f0c 5bd6 a000 0007 930c  RV...3..[.......
-000015f0: 61ce a500 0034 500c 63ce a500 000a dc0c  a....4P.c.......
-00001600: 6dca b800 0037 6a0c 808a a300 00a4 de0c  m....7j.........
-00001610: 83b7 b000 0036 f00c 8910 0000 0006 9a0c  .....6..........
-00001620: 89ed e500 0049 fb0c 98c0 0900 0005 e20c  .....I..........
-00001630: 98c0 0900 0009 ba0c 98c0 0900 000c f30c  ................
-00001640: 98c0 0900 0082 760c 98c0 0900 0088 010c  ......v.........
-00001650: 98c0 0900 009f 1a0c 98c0 0900 0117 8f0c  ................
-00001660: 9fa9 6000 011f 1f0c b106 9a00 011b 9e0c  ..`.............
-00001670: b195 2700 007e e40c b1a8 e500 0030 780c  ..'..~.......0x.
-00001680: ba9f 2400 0111 360c c1c5 c300 0090 820c  ..$...6.........
-00001690: c4e1 d500 0013 ab0c c5f7 d500 007c d90c  .............|..
-000016a0: c7ee 6000 009c 070c c8e8 6400 002f c30c  ..`.......d../..
-000016b0: c9a0 2e00 007d 380c cba2 d500 00ea d90c  .....}8.........
-000016c0: db0c 0400 00b4 610c dda2 6e00 00b1 de0c  ......a...n.....
-000016d0: e3ed a900 0090 370c f3b0 8500 0012 450c  ......7.......E.
-000016e0: fb0f b300 0093 230d 0027 2000 00bf c30d  ......#..' .....
-000016f0: 09a5 6000 011d 540d 0a66 ed00 0126 c30d  ..`...T..f...&..
-00001700: 0ad7 7300 004c 430d 0f91 6000 00f0 850d  ..s..LC...`.....
-00001710: 0f91 6000 0105 b00d 1201 a400 005b a70d  ..`..........[..
-00001720: 1cec 6700 011a ca0d 2d41 7000 00ae 210d  ..g.....-Ap...!.
-00001730: 32db 3000 00ed 270d 35c6 3000 0109 470d  2.0...'.5.0...G.
-00001740: 3b8c 3900 00ab a10d 48cd 6500 0099 f80d  ;.9.....H.e.....
-00001750: 51bd f000 00f4 930d 69f6 0000 009c b40d  Q.......i.......
-00001760: 7298 e700 00ad 5d0d 7c3b 4000 0112 7b0d  r.....].|;@...{.
-00001770: 80f6 3400 0096 ff0d 80f6 3400 0098 8f0d  ..4.......4.....
-00001780: 8344 9300 008f 790d 8c46 7500 0004 a70d  .D....y..Fu.....
-00001790: 8c46 7500 00a5 730d 96e3 5000 00df 4a0d  .Fu...s...P...J.
-000017a0: 9df1 6500 0019 a90d 9df1 6500 0020 7e0d  ..e.......e.. ~.
-000017b0: 9ee3 5e00 006c 5e0d 9ee3 5e00 0077 cc0d  ..^..l^...^..w..
-000017c0: 9ee3 5e00 0084 450d 9ee3 5e00 00a3 a20d  ..^...E...^.....
-000017d0: 9ee3 5e00 00b6 b80d aa4e 9000 00e6 330d  ..^......N....3.
-000017e0: c964 7400 00aa 700d d0e8 e000 00c8 b50d  .dt...p.........
-000017f0: ded8 9000 001d 2b0d ded8 9000 0053 860d  ......+......S..
-00001800: eb49 0000 007f 1c0d ec49 8400 0047 c10d  .I.......I...G..
-00001810: f086 4a00 0038 e10d fcd5 7e00 003e 5c0d  ..J..8....~..>\.
-00001820: fe0b 6000 006f 320e 00f0 b000 00d4 8f0e  ..`..o2.........
-00001830: 03af f000 0076 980e 1bf8 6400 0038 800e  .....v....d..8..
-00001840: 1ddb 6300 0051 9b0e 202b 3a00 007d 970e  ..c..Q.. +:..}..
-00001850: 202b 3a00 0126 2a0e 20d7 0900 010e d80e   +:..&*. .......
-00001860: 2511 7400 0060 170e 38a0 f000 0106 d00e  %.t..`..8.......
-00001870: 5c13 4700 0119 120e 6193 e900 0113 a90e  \.G.....a.......
-00001880: 61d5 0400 00a8 9c0e 68cb dc00 0056 530e  a.......h....VS.
-00001890: 6ac2 e300 0024 cc0e 7617 2000 007b 090e  j....$..v. ..{..
-000018a0: 8347 4400 0069 bf0e 887b b500 0036 850e  .GD..i...{...6..
-000018b0: 887b b500 00a9 730e 9dcc d400 0032 820e  .{....s......2..
-000018c0: a934 c000 0060 960e abf5 1300 0067 6d0e  .4...`.......gm.
-000018d0: ae34 8000 005d d10e b4a5 0a00 0063 640e  .4...].......cd.
-000018e0: b5c2 8000 009a 5a0e b803 9900 006e 220e  ......Z......n".
-000018f0: b82d 1000 00f5 270e c28b b000 0003 0c0e  .-....'.........
-00001900: d945 de00 002d 820e e77d 7000 0121 930e  .E...-...}p..!..
-00001910: f7f8 4000 00f1 260f 09fd b000 00d6 530f  ..@...&.......S.
-00001920: 0cc4 c000 00fc 310f 105e a000 00ba f90f  ......1..^......
-00001930: 11be 6000 00c0 380f 1d28 1000 00ff f30f  ..`...8..(......
-00001940: 201d 8500 0088 b60f 20f1 3000 00d8 930f   ....... .0.....
-00001950: 4321 f500 0132 160f 4a90 4000 00b3 a80f  C!...2..J.@.....
-00001960: 5e00 1000 00ca 710f 8e7b e000 00ce d30f  ^.....q..{......
-00001970: 9222 7c00 00ab 610f 9450 0000 0114 e60f  ."|...a..P......
-00001980: 9ebd c400 0048 190f 9fbc 6000 0136 a00f  .....H....`..6..
-00001990: a262 9000 0139 170f a44f 0300 0000 5f0f  .b...9...O...._.
-000019a0: bd5e e700 011a 2c0f cb15 5200 0069 730f  .^....,...R..is.
-000019b0: cf80 f000 00f6 6e0f d19a 7000 00c1 a90f  ......n...p.....
-000019c0: dfeb 7000 009e 450f e7f7 9000 0138 a50f  ..p...E......8..
-000019d0: ea8a 0900 007d dc0f ea8a 0900 00a6 930f  .....}..........
-000019e0: ea8a 0900 0126 690f f87c e000 0023 990f  .....&i..|...#..
-000019f0: fe37 0300 0086 4169 0001 3992 0300 0000  .7....Ai..9.....
-00001a00: 2404 1e04 4204 3c04 3504 3d04 3804 4204  $...B.<.5.=.8.B.
-00001a10: 4c00 2004 3804 3704 3c04 3504 3d04 3504  L. .8.7.<.5.=.5.
-00001a20: 3d04 3804 4f08 0000 0000 0600 0000 0e43  =.8.O..........C
-00001a30: 616e 6365 6c20 6368 616e 6765 7307 0000  ancel changes...
-00001a40: 0018 4162 7374 7261 6374 4f70 6572 6174  ..AbstractOperat
-00001a50: 696f 6e44 6574 6169 6c73 0103 0000 0026  ionDetails.....&
-00001a60: 0421 043e 0445 0440 0430 043d 0438 0442  .!.>.E.@.0.=.8.B
-00001a70: 044c 0020 0438 0437 043c 0435 043d 0435  .L. .8.7.<.5.=.5
-00001a80: 043d 0438 044f 0800 0000 0006 0000 000e  .=.8.O..........
-00001a90: 436f 6d6d 6974 2063 6861 6e67 6573 0700  Commit changes..
-00001aa0: 0000 1841 6273 7472 6163 744f 7065 7261  ...AbstractOpera
-00001ab0: 7469 6f6e 4465 7461 696c 7301 0300 0000  tionDetails.....
-00001ac0: 3804 1e04 4804 3804 3104 3a04 3000 2004  8...H.8.1.:.0. .
-00001ad0: 3f04 4004 3800 2004 3704 3004 3f04 3804  ?.@.8. .7.0.?.8.
-00001ae0: 4104 3800 2004 3e04 3f04 3504 4004 3004  A.8. .>.?.5.@.0.
-00001af0: 4604 3804 3800 3a00 2008 0000 0000 0600  F.8.8.:. .......
-00001b00: 0000 194f 7065 7261 7469 6f6e 2073 7562  ...Operation sub
-00001b10: 6d69 7420 6661 696c 6564 3a20 0700 0000  mit failed: ....
-00001b20: 1841 6273 7472 6163 744f 7065 7261 7469  .AbstractOperati
-00001b30: 6f6e 4465 7461 696c 7301 0300 0000 8804  onDetails.......
-00001b40: 1d04 3504 4104 3e04 4504 4004 3004 3d04  ..5.A.>.E.@.0.=.
-00001b50: 5104 3d04 3d04 4b04 3500 2004 3804 3704  Q.=.=.K.5. .8.7.
-00001b60: 3c04 3504 3d04 3504 3d04 3804 4f00 2004  <.5.=.5.=.8.O. .
-00001b70: 3104 4b04 3b04 3800 2004 3e04 4204 3c04  1.K.;.8. .>.B.<.
-00001b80: 3504 3d04 3504 3d04 4b00 2004 3f04 3504  5.=.5.=.K. .?.5.
-00001b90: 4004 3504 3400 2004 4104 3e04 3704 3404  @.5.4. .A.>.7.4.
-00001ba0: 3004 3d04 3804 3504 3c00 2004 3d04 3e04  0.=.8.5.<. .=.>.
-00001bb0: 3204 3e04 3900 2004 3e04 3f04 3504 4004  2.>.9. .>.?.5.@.
-00001bc0: 3004 4604 3804 3808 0000 0000 0600 0000  0.F.8.8.........
-00001bd0: 3555 6e73 6176 6564 2063 6861 6e67 6573  5Unsaved changes
-00001be0: 2077 6572 6520 7265 7665 7274 6564 2074   were reverted t
-00001bf0: 6f20 6372 6561 7465 206e 6577 206f 7065  o create new ope
-00001c00: 7261 7469 6f6e 0700 0000 1841 6273 7472  ration.....Abstr
-00001c10: 6163 744f 7065 7261 7469 6f6e 4465 7461  actOperationDeta
-00001c20: 696c 7301 0300 0000 3a04 1d04 3504 3204  ils.....:...5.2.
-00001c30: 3504 4004 3d04 3e04 3500 2004 3704 3d04  5.@.=.>.5. .7.=.
-00001c40: 3004 4704 3504 3d04 3804 3500 2004 3200  0.G.5.=.8.5. .2.
-00001c50: 2004 4104 4204 3e04 3b04 3104 4604 3500   .A.B.>.;.1.F.5.
-00001c60: 3a00 2008 0000 0000 0600 0000 1b43 6f6c  :. ..........Col
-00001c70: 756d 6e20 6861 7320 6e6f 2076 616c 6964  umn has no valid
-00001c80: 2076 616c 7565 3a20 0700 0000 1a41 6273   value: .....Abs
-00001c90: 7472 6163 7452 6566 6572 656e 6365 4c69  tractReferenceLi
-00001ca0: 7374 4d6f 6465 6c01 0300 0000 1e04 1d04  stModel.........
-00001cb0: 3504 3f04 3e04 3b04 3d04 4b04 3500 2004  5.?.>.;.=.K.5. .
-00001cc0: 3404 3004 3d04 3d04 4b04 3508 0000 0000  4.0.=.=.K.5.....
-00001cd0: 0600 0000 1344 6174 6120 6172 6520 696e  .....Data are in
-00001ce0: 636f 6d70 6c65 7465 0700 0000 1a41 6273  complete.....Abs
-00001cf0: 7472 6163 7452 6566 6572 656e 6365 4c69  tractReferenceLi
-00001d00: 7374 4d6f 6465 6c01 0300 0000 2604 1e04  stModel.....&...
-00001d10: 4804 3804 3104 3a04 3000 2004 4104 3e04  H.8.1.:.0. .A.>.
-00001d20: 4504 4004 3004 3d04 3504 3d04 3804 4f00  E.@.0.=.5.=.8.O.
-00001d30: 3a00 2008 0000 0000 0600 0000 0f53 7562  :. ..........Sub
-00001d40: 6d69 7420 6661 696c 6564 3a20 0700 0000  mit failed: ....
-00001d50: 1a41 6273 7472 6163 7452 6566 6572 656e  .AbstractReferen
-00001d60: 6365 4c69 7374 4d6f 6465 6c01 0300 0000  ceListModel.....
-00001d70: 0a04 1b04 4e04 3104 3e04 3908 0000 0000  ....N.1.>.9.....
-00001d80: 0600 0000 0341 4e59 0700 0000 0d41 6363  .....ANY.....Acc
-00001d90: 6f75 6e74 4275 7474 6f6e 0103 0000 0014  ountButton......
-00001da0: 041b 044e 0431 043e 0439 0020 0441 0447  ...N.1.>.9. .A.G
-00001db0: 0435 0442 0800 0000 0006 0000 000b 416e  .5.B..........An
-00001dc0: 7920 6163 636f 756e 7407 0000 000d 4163  y account.....Ac
-00001dd0: 636f 756e 7442 7574 746f 6e01 0300 0000  countButton.....
-00001de0: 1804 1204 4b04 3104 4004 3004 4204 4c00  ....K.1.@.0.B.L.
-00001df0: 2004 4104 4704 3504 4208 0000 0000 0600   .A.G.5.B.......
-00001e00: 0000 0e43 686f 6f73 6520 6163 636f 756e  ...Choose accoun
-00001e10: 7407 0000 000d 4163 636f 756e 7442 7574  t.....AccountBut
-00001e20: 746f 6e01 0300 0000 1404 2204 3804 3f00  ton.......".8.?.
-00001e30: 2004 4104 4704 3504 4204 3000 3a08 0000   .A.G.5.B.0.:...
-00001e40: 0000 0600 0000 0d41 6363 6f75 6e74 2074  .......Account t
-00001e50: 7970 653a 0700 0000 1141 6363 6f75 6e74  ype:.....Account
-00001e60: 4c69 7374 4469 616c 6f67 0103 0000 000a  ListDialog......
-00001e70: 0421 0447 0435 0442 0430 0800 0000 0006  .!.G.5.B.0......
-00001e80: 0000 0008 4163 636f 756e 7473 0700 0000  ....Accounts....
-00001e90: 1141 6363 6f75 6e74 4c69 7374 4469 616c  .AccountListDial
-00001ea0: 6f67 0103 0000 002a 041f 043e 043a 0430  og.....*...>.:.0
-00001eb0: 0437 044b 0432 0430 0442 044c 0020 043d  .7.K.2.0.B.L. .=
-00001ec0: 0435 0430 043a 0442 0438 0432 043d 044b  .5.0.:.B.8.2.=.K
-00001ed0: 0435 0800 0000 0006 0000 000d 5368 6f77  .5..........Show
-00001ee0: 2069 6e61 6374 6976 6507 0000 0011 4163   inactive.....Ac
-00001ef0: 636f 756e 744c 6973 7444 6961 6c6f 6701  countListDialog.
-00001f00: 0300 0000 0e21 1600 2004 4104 4704 3504  .....!.. .A.G.5.
-00001f10: 4204 3008 0000 0000 0600 0000 0941 6363  B.0..........Acc
-00001f20: 6f75 6e74 2023 0700 0000 1041 6363 6f75  ount #.....Accou
-00001f30: 6e74 4c69 7374 4d6f 6465 6c01 0300 0000  ntListModel.....
-00001f40: 0804 1004 3a04 4200 2e08 0000 0000 0600  ....:.B.........
-00001f50: 0000 0441 6374 2e07 0000 0010 4163 636f  ...Act......Acco
-00001f60: 756e 744c 6973 744d 6f64 656c 0103 0000  untListModel....
-00001f70: 0016 0411 0430 043d 043a 002f 0411 0440  .....0.=.:./...@
-00001f80: 043e 043a 0435 0440 0800 0000 0006 0000  .>.:.5.@........
-00001f90: 000b 4261 6e6b 2f42 726f 6b65 7207 0000  ..Bank/Broker...
-00001fa0: 0010 4163 636f 756e 744c 6973 744d 6f64  ..AccountListMod
-00001fb0: 656c 0103 0000 0004 041a 0421 0800 0000  el.........!....
-00001fc0: 0006 0000 0002 4343 0700 0000 1041 6363  ......CC.....Acc
-00001fd0: 6f75 6e74 4c69 7374 4d6f 6465 6c01 0300  ountListModel...
-00001fe0: 0000 0c04 1204 3004 3b04 4e04 4204 3008  ......0.;.N.B.0.
-00001ff0: 0000 0000 0600 0000 0843 7572 7265 6e63  .........Currenc
-00002000: 7907 0000 0010 4163 636f 756e 744c 6973  y.....AccountLis
-00002010: 744d 6f64 656c 0103 0000 0018 041d 0430  tModel.........0
-00002020: 0438 043c 0435 043d 043e 0432 0430 043d  .8.<.5.=.>.2.0.=
-00002030: 0438 0435 0800 0000 0006 0000 0004 4e61  .8.5..........Na
-00002040: 6d65 0700 0000 1041 6363 6f75 6e74 4c69  me.....AccountLi
-00002050: 7374 4d6f 6465 6c01 0300 0000 1004 2204  stModel.......".
-00002060: 3e04 4704 3d04 3e04 4104 4204 4c08 0000  >.G.=.>.A.B.L...
-00002070: 0000 0600 0000 0950 7265 6369 7369 6f6e  .......Precision
-00002080: 0700 0000 1041 6363 6f75 6e74 4c69 7374  .....AccountList
-00002090: 4d6f 6465 6c01 0300 0000 1004 2104 3204  Model.......!.2.
-000020a0: 3504 4004 3504 3d00 2000 4008 0000 0000  5.@.5.=. .@.....
-000020b0: 0600 0000 0c52 6563 6f6e 6369 6c65 6420  .....Reconciled 
-000020c0: 4007 0000 0010 4163 636f 756e 744c 6973  @.....AccountLis
-000020d0: 744d 6f64 656c 0103 0000 001a 0426 0435  tModel.......&.5
-000020e0: 043d 043d 0430 044f 0020 0431 0443 043c  .=.=.0.O. .1.C.<
-000020f0: 0430 0433 0430 0800 0000 0006 0000 0005  .0.3.0..........
-00002100: 4173 7365 7407 0000 000b 4173 7365 7444  Asset.....AssetD
-00002110: 6961 6c6f 6701 0300 0000 1c04 1104 3004  ialog.........0.
-00002120: 3704 3e04 3204 4b04 3900 2004 3004 3a04  7.>.2.K.9. .0.:.
-00002130: 4204 3804 3200 3a08 0000 0000 0600 0000  B.8.2.:.........
-00002140: 0b42 6173 6520 6173 7365 743a 0700 0000  .Base asset:....
-00002150: 0b41 7373 6574 4469 616c 6f67 0103 0000  .AssetDialog....
-00002160: 000c 041e 0442 043c 0435 043d 0430 0800  .....B.<.5.=.0..
-00002170: 0000 0006 0000 0006 4361 6e63 656c 0700  ........Cancel..
-00002180: 0000 0b41 7373 6574 4469 616c 6f67 0103  ...AssetDialog..
-00002190: 0000 0010 0421 0442 0440 0430 043d 0430  .....!.B.@.0.=.0
-000021a0: 003a 0020 0800 0000 0006 0000 0009 436f  .:. ..........Co
-000021b0: 756e 7472 793a 2007 0000 000b 4173 7365  untry: .....Asse
-000021c0: 7444 6961 6c6f 6701 0300 0000 1404 1404  tDialog.........
-000021d0: 3e04 3f00 2e04 3404 3004 3d04 3d04 4b04  >.?...4.0.=.=.K.
-000021e0: 3508 0000 0000 0600 0000 0a45 7874 7261  5..........Extra
-000021f0: 2064 6174 6107 0000 000b 4173 7365 7444   data.....AssetD
-00002200: 6961 6c6f 6701 0300 0000 0a00 4900 5300  ialog.......I.S.
-00002210: 4900 4e00 3a08 0000 0000 0600 0000 0549  I.N.:..........I
-00002220: 5349 4e3a 0700 0000 0b41 7373 6574 4469  SIN:.....AssetDi
-00002230: 616c 6f67 0103 0000 001a 041d 0430 0438  alog.........0.8
-00002240: 043c 0435 043d 043e 0432 0430 043d 0438  .<.5.=.>.2.0.=.8
-00002250: 0435 003a 0800 0000 0006 0000 0005 4e61  .5.:..........Na
-00002260: 6d65 3a07 0000 000b 4173 7365 7444 6961  me:.....AssetDia
-00002270: 6c6f 6701 0300 0000 0404 1e04 1a08 0000  log.............
-00002280: 0000 0600 0000 024f 4b07 0000 000b 4173  .......OK.....As
-00002290: 7365 7444 6961 6c6f 6701 0300 0000 0e04  setDialog.......
-000022a0: 2104 3804 3c04 3204 3e04 3b04 4b08 0000  !.8.<.2.>.;.K...
-000022b0: 0000 0600 0000 0753 796d 626f 6c73 0700  .......Symbols..
-000022c0: 0000 0b41 7373 6574 4469 616c 6f67 0103  ...AssetDialog..
-000022d0: 0000 000a 0422 0438 043f 003a 0020 0800  .....".8.?.:. ..
-000022e0: 0000 0006 0000 0006 5479 7065 3a20 0700  ........Type: ..
-000022f0: 0000 0b41 7373 6574 4469 616c 6f67 0103  ...AssetDialog..
-00002300: 0000 000e 0422 0438 043f 0020 0426 0411  .....".8.?. .&..
-00002310: 003a 0800 0000 0006 0000 000b 4173 7365  .:..........Asse
-00002320: 7420 7479 7065 3a07 0000 000f 4173 7365  t type:.....Asse
-00002330: 744c 6973 7444 6961 6c6f 6701 0300 0000  tListDialog.....
-00002340: 1a04 2604 3504 3d04 3d04 4b04 3500 2004  ..&.5.=.=.K.5. .
-00002350: 3104 4304 3c04 3004 3304 3808 0000 0000  1.C.<.0.3.8.....
-00002360: 0600 0000 0641 7373 6574 7307 0000 000f  .....Assets.....
-00002370: 4173 7365 744c 6973 7444 6961 6c6f 6701  AssetListDialog.
-00002380: 0300 0000 0c04 2104 4204 4004 3004 3d04  ......!.B.@.0.=.
-00002390: 3008 0000 0000 0600 0000 0743 6f75 6e74  0..........Count
-000023a0: 7279 0700 0000 0e41 7373 6574 4c69 7374  ry.....AssetList
-000023b0: 4d6f 6465 6c01 0300 0000 0c04 1204 3004  Model.........0.
-000023c0: 3b04 4e04 4204 3008 0000 0000 0600 0000  ;.N.B.0.........
-000023d0: 0843 7572 7265 6e63 7907 0000 000e 4173  .Currency.....As
-000023e0: 7365 744c 6973 744d 6f64 656c 0103 0000  setListModel....
-000023f0: 001a 0418 0441 0442 002e 043a 043e 0442  .....A.B...:.>.B
-00002400: 0438 0440 043e 0432 043e 043a 0800 0000  .8.@.>.2.>.:....
-00002410: 0006 0000 000b 4461 7461 2073 6f75 7263  ......Data sourc
-00002420: 6507 0000 000e 4173 7365 744c 6973 744d  e.....AssetListM
-00002430: 6f64 656c 0103 0000 0008 0049 0053 0049  odel.......I.S.I
-00002440: 004e 0800 0000 0006 0000 0004 4953 494e  .N..........ISIN
-00002450: 0700 0000 0e41 7373 6574 4c69 7374 4d6f  .....AssetListMo
-00002460: 6465 6c01 0300 0000 1804 1d04 3004 3804  del.........0.8.
-00002470: 3c04 3504 3d04 3e04 3204 3004 3d04 3804  <.5.=.>.2.0.=.8.
-00002480: 3508 0000 0000 0600 0000 044e 616d 6507  5..........Name.
-00002490: 0000 000e 4173 7365 744c 6973 744d 6f64  ....AssetListMod
-000024a0: 656c 0103 0000 000c 0421 0438 043c 0432  el.......!.8.<.2
-000024b0: 043e 043b 0800 0000 0006 0000 0006 5379  .>.;..........Sy
-000024c0: 6d62 6f6c 0700 0000 0e41 7373 6574 4c69  mbol.....AssetLi
-000024d0: 7374 4d6f 6465 6c01 0300 0000 1804 1d04  stModel.........
-000024e0: 3004 3804 3c04 3504 3d04 3e04 3204 3004  0.8.<.5.=.>.2.0.
-000024f0: 3d04 3804 3508 0000 0000 0600 0000 0a41  =.8.5..........A
-00002500: 7373 6574 206e 616d 6507 0000 000f 4173  sset name.....As
-00002510: 7365 7473 4c69 7374 4d6f 6465 6c01 0300  setsListModel...
-00002520: 0000 1a04 1104 3004 3704 3e04 3204 4b04  ......0.7.>.2.K.
-00002530: 3900 2004 3004 3a04 4204 3804 3208 0000  9. .0.:.B.8.2...
-00002540: 0000 0600 0000 0a42 6173 6520 6173 7365  .......Base asse
-00002550: 7407 0000 000f 4173 7365 7473 4c69 7374  t.....AssetsList
-00002560: 4d6f 6465 6c01 0300 0000 0c04 2104 4204  Model.......!.B.
-00002570: 4004 3004 3d04 3008 0000 0000 0600 0000  @.0.=.0.........
-00002580: 0743 6f75 6e74 7279 0700 0000 0f41 7373  .Country.....Ass
-00002590: 6574 734c 6973 744d 6f64 656c 0103 0000  etsListModel....
-000025a0: 0008 0049 0053 0049 004e 0800 0000 0006  ...I.S.I.N......
-000025b0: 0000 0004 4953 494e 0700 0000 0f41 7373  ....ISIN.....Ass
-000025c0: 6574 734c 6973 744d 6f64 656c 0103 0000  etsListModel....
-000025d0: 0008 0421 0447 0435 0442 0800 0000 0006  ...!.G.5.B......
-000025e0: 0000 0007 4163 636f 756e 7407 0000 000d  ....Account.....
-000025f0: 4261 6c61 6e63 6573 4d6f 6465 6c01 0300  BalancesModel...
-00002600: 0000 0c04 1104 3004 3b04 3004 3d04 4108  ......0.;.0.=.A.
-00002610: 0000 0000 0600 0000 0742 616c 616e 6365  .........Balance
-00002620: 0700 0000 0d42 616c 616e 6365 734d 6f64  .....BalancesMod
-00002630: 656c 0103 0000 0010 0411 0430 043b 0430  el.........0.;.0
-00002640: 043d 0441 002c 0020 0800 0000 0006 0000  .=.A.,. ........
-00002650: 0009 4261 6c61 6e63 652c 2007 0000 000d  ..Balance, .....
-00002660: 4261 6c61 6e63 6573 4d6f 6465 6c01 0300  BalancesModel...
-00002670: 0000 0a04 1804 4204 3e04 3304 3e08 0000  ......B.>.3.>...
-00002680: 0000 0600 0000 0554 6f74 616c 0700 0000  .......Total....
-00002690: 0d42 616c 616e 6365 734d 6f64 656c 0103  .BalancesModel..
-000026a0: 0000 001c 0411 0430 0437 043e 0432 0430  .......0.7.>.2.0
-000026b0: 044f 0020 0432 0430 043b 044e 0442 0430  .O. .2.0.;.N.B.0
-000026c0: 0800 0000 0006 0000 000d 4261 7365 2063  ..........Base c
-000026d0: 7572 7265 6e63 7907 0000 0012 4261 7365  urrency.....Base
-000026e0: 4375 7272 656e 6379 4469 616c 6f67 0103  CurrencyDialog..
-000026f0: 0000 000c 0412 0430 043b 044e 0442 0430  .......0.;.N.B.0
-00002700: 0800 0000 0006 0000 0008 4375 7272 656e  ..........Curren
-00002710: 6379 0700 0000 1542 6173 6543 7572 7265  cy.....BaseCurre
-00002720: 6e63 794c 6973 744d 6f64 656c 0103 0000  ncyListModel....
-00002730: 0008 0414 0430 0442 0430 0800 0000 0006  .....0.B.0......
-00002740: 0000 0004 4461 7465 0700 0000 1542 6173  ....Date.....Bas
-00002750: 6543 7572 7265 6e63 794c 6973 744d 6f64  eCurrencyListMod
-00002760: 656c 0103 0000 0024 0027 0020 0437 0430  el.....$.'. .7.0
-00002770: 043c 0435 043d 0435 043d 0430 0020 0443  .<.5.=.5.=.0. .C
-00002780: 0441 043f 0435 0448 043d 043e 0800 0000  .A.?.5.H.=.>....
-00002790: 0006 0000 001b 2720 7761 7320 7375 6363  ......' was succ
-000027a0: 6573 7366 756c 6c79 2072 6570 6c61 6365  essfully replace
-000027b0: 6407 0000 0012 4361 7465 676f 7279 4c69  d.....CategoryLi
-000027c0: 7374 4469 616c 6f67 0103 0000 000c 0027  stDialog.......'
-000027d0: 0020 043d 0430 003a 0020 0800 0000 0006  . .=.0.:. ......
-000027e0: 0000 0008 2720 7769 7468 3a20 0700 0000  ....' with: ....
-000027f0: 1243 6174 6567 6f72 794c 6973 7444 6961  .CategoryListDia
-00002800: 6c6f 6701 0300 0000 1204 1a04 3004 4204  log.........0.B.
-00002810: 3504 3304 3e04 4004 3804 3808 0000 0000  5.3.>.@.8.8.....
-00002820: 0600 0000 0a43 6174 6567 6f72 6965 7307  .....Categories.
-00002830: 0000 0012 4361 7465 676f 7279 4c69 7374  ....CategoryList
-00002840: 4469 616c 6f67 0103 0000 0016 041a 0430  Dialog.........0
-00002850: 0442 0435 0433 043e 0440 0438 044f 0020  .B.5.3.>.@.8.O. 
-00002860: 0027 0800 0000 0006 0000 000a 4361 7465  .'..........Cate
-00002870: 676f 7279 2027 0700 0000 1243 6174 6567  gory '.....Categ
-00002880: 6f72 794c 6973 7444 6961 6c6f 6701 0300  oryListDialog...
-00002890: 0000 2804 1704 3004 3c04 3504 3d04 3804  ..(...0.<.5.=.8.
-000028a0: 4204 4c00 2004 3a04 3004 4204 3504 3304  B.L. .:.0.B.5.3.
-000028b0: 3e04 4004 3804 4e00 2000 2708 0000 0000  >.@.8.N. .'.....
-000028c0: 0600 0000 1252 6570 6c61 6365 2063 6174  .....Replace cat
-000028d0: 6567 6f72 7920 2707 0000 0012 4361 7465  egory '.....Cate
-000028e0: 676f 7279 4c69 7374 4469 616c 6f67 0103  goryListDialog..
-000028f0: 0000 001c 0417 0430 043c 0435 043d 0438  .......0.<.5.=.8
-00002900: 0442 044c 0020 043d 0430 002e 002e 002e  .B.L. .=.0......
-00002910: 0800 0000 0006 0000 000f 5265 706c 6163  ..........Replac
-00002920: 6520 7769 7468 2e2e 2e07 0000 0012 4361  e with........Ca
-00002930: 7465 676f 7279 4c69 7374 4469 616c 6f67  tegoryListDialog
-00002940: 0103 0000 003c 041f 043e 043a 0430 0437  .....<...>.:.0.7
-00002950: 0430 0442 044c 0020 043e 043f 0435 0440  .0.B.L. .>.?.5.@
-00002960: 0430 0446 0438 0438 0020 0441 0020 041a  .0.F.8.8. .A. ..
-00002970: 0430 0442 0435 0433 043e 0440 0438 0435  .0.B.5.3.>.@.8.5
-00002980: 0439 0800 0000 0006 0000 001d 5368 6f77  .9..........Show
-00002990: 206f 7065 7261 7469 6f6e 7320 7769 7468   operations with
-000029a0: 2043 6174 6567 6f72 7907 0000 0012 4361   Category.....Ca
-000029b0: 7465 676f 7279 4c69 7374 4469 616c 6f67  tegoryListDialog
-000029c0: 0103 0000 0010 041e 043f 0435 0440 0430  .........?.5.@.0
-000029d0: 0446 0438 0438 0800 0000 0006 0000 000a  .F.8.8..........
-000029e0: 4f70 6572 6174 696f 6e73 0700 0000 0e43  Operations.....C
-000029f0: 6174 6567 6f72 7952 6570 6f72 7401 0300  ategoryReport...
-00002a00: 0000 1804 3f04 3e00 2004 1a04 3004 4204  ....?.>. ...0.B.
-00002a10: 3504 3304 3e04 4004 3804 3808 0000 0000  5.3.>.@.8.8.....
-00002a20: 0600 0000 0b62 7920 4361 7465 676f 7279  .....by Category
-00002a30: 0700 0000 0e43 6174 6567 6f72 7952 6570  .....CategoryRep
-00002a40: 6f72 7401 0300 0000 1404 1a04 3004 4204  ort.........0.B.
-00002a50: 3504 3304 3e04 4004 3804 4f00 3a08 0000  5.3.>.@.8.O.:...
-00002a60: 0000 0600 0000 0943 6174 6567 6f72 793a  .......Category:
-00002a70: 0700 0000 1443 6174 6567 6f72 7952 6570  .....CategoryRep
-00002a80: 6f72 7457 6964 6765 7401 0300 0000 2404  ortWidget.....$.
-00002a90: 1e04 4204 4704 5104 4200 2004 3f04 3e00  ..B.G.Q.B. .?.>.
-00002aa0: 2004 3a04 3004 4204 3504 3304 3e04 4004   .:.0.B.5.3.>.@.
-00002ab0: 3804 3808 0000 0000 0600 0000 1252 6570  8.8..........Rep
-00002ac0: 6f72 7420 6279 2063 6174 6567 6f72 7907  ort by category.
-00002ad0: 0000 0014 4361 7465 676f 7279 5265 706f  ....CategoryRepo
-00002ae0: 7274 5769 6467 6574 0103 0000 0018 041d  rtWidget........
-00002af0: 0430 0438 043c 0435 043d 043e 0432 0430  .0.8.<.5.=.>.2.0
-00002b00: 043d 0438 0435 0800 0000 0006 0000 0004  .=.8.5..........
-00002b10: 4e61 6d65 0700 0000 1143 6174 6567 6f72  Name.....Categor
-00002b20: 7954 7265 654d 6f64 656c 0103 0000 000c  yTreeModel......
-00002b30: 0427 0430 0441 0442 0430 044f 0800 0000  .'.0.A.B.0.O....
-00002b40: 0006 0000 0005 4f66 7465 6e07 0000 0011  ......Often.....
-00002b50: 4361 7465 676f 7279 5472 6565 4d6f 6465  CategoryTreeMode
-00002b60: 6c01 0300 0000 2004 1304 4004 3004 4404  l..... ...@.0.D.
-00002b70: 3804 3a00 2004 4604 3504 3d04 4b00 2004  8.:. .F.5.=.K. .
-00002b80: 3404 3b04 4f00 2008 0000 0000 0600 0000  4.;.O. .........
-00002b90: 1050 7269 6365 2063 6861 7274 2066 6f72  .Price chart for
-00002ba0: 2007 0000 000b 4368 6172 7457 696e 646f   .....ChartWindo
-00002bb0: 7701 0300 0000 1a04 2604 3504 3d04 3d04  w.......&.5.=.=.
-00002bc0: 3004 4f00 2004 3104 4304 3c04 3004 3304  0.O. .1.C.<.0.3.
-00002bd0: 3008 0000 0000 0600 0000 0541 7373 6574  0..........Asset
-00002be0: 0700 0000 1143 6c6f 7365 6454 7261 6465  .....ClosedTrade
-00002bf0: 734d 6f64 656c 0103 0000 001a 0414 0430  sModel.........0
-00002c00: 0442 0430 0020 0437 0430 043a 0440 044b  .B.0. .7.0.:.@.K
-00002c10: 0442 0438 044f 0800 0000 0006 0000 000a  .B.8.O..........
-00002c20: 436c 6f73 6520 4461 7465 0700 0000 1143  Close Date.....C
-00002c30: 6c6f 7365 6454 7261 6465 734d 6f64 656c  losedTradesModel
-00002c40: 0103 0000 0026 0414 0430 0442 0430 002f  .....&...0.B.0./
-00002c50: 0432 0440 0435 043c 044f 0020 0437 0430  .2.@.5.<.O. .7.0
-00002c60: 043a 0440 044b 0442 0438 044f 0800 0000  .:.@.K.B.8.O....
-00002c70: 0006 0000 000f 436c 6f73 6520 4461 7465  ......Close Date
-00002c80: 2f54 696d 6507 0000 0011 436c 6f73 6564  /Time.....Closed
-00002c90: 5472 6164 6573 4d6f 6465 6c01 0300 0000  TradesModel.....
-00002ca0: 1a04 2604 3504 3d04 3000 2004 3704 3004  ..&.5.=.0. .7.0.
-00002cb0: 3a04 4004 4b04 4204 3804 4f08 0000 0000  :.@.K.B.8.O.....
-00002cc0: 0600 0000 0b43 6c6f 7365 2050 7269 6365  .....Close Price
-00002cd0: 0700 0000 1143 6c6f 7365 6454 7261 6465  .....ClosedTrade
-00002ce0: 734d 6f64 656c 0103 0000 0010 041a 043e  sModel.........>
-00002cf0: 043c 0438 0441 0441 0438 044f 0800 0000  .<.8.A.A.8.O....
-00002d00: 0006 0000 0003 4665 6507 0000 0011 436c  ......Fee.....Cl
-00002d10: 6f73 6564 5472 6164 6573 4d6f 6465 6c01  osedTradesModel.
-00002d20: 0300 0000 1404 1f04 4004 3804 3c04 3504  ........@.8.<.5.
-00002d30: 4704 3004 3d04 3804 3508 0000 0000 0600  G.0.=.8.5.......
-00002d40: 0000 044e 6f74 6507 0000 0011 436c 6f73  ...Note.....Clos
-00002d50: 6564 5472 6164 6573 4d6f 6465 6c01 0300  edTradesModel...
-00002d60: 0000 1a04 1404 3004 4204 3000 2004 3e04  ......0.B.0. .>.
-00002d70: 4204 3a04 4004 4b04 4204 3804 4f08 0000  B.:.@.K.B.8.O...
-00002d80: 0000 0600 0000 094f 7065 6e20 4461 7465  .......Open Date
-00002d90: 0700 0000 1143 6c6f 7365 6454 7261 6465  .....ClosedTrade
-00002da0: 734d 6f64 656c 0103 0000 0026 0414 0430  sModel.....&...0
-00002db0: 0442 0430 002f 0412 0440 0435 043c 044f  .B.0./...@.5.<.O
-00002dc0: 0020 043e 0442 043a 0440 044b 0442 0438  . .>.B.:.@.K.B.8
-00002dd0: 044f 0800 0000 0006 0000 000e 4f70 656e  .O..........Open
-00002de0: 2044 6174 652f 5469 6d65 0700 0000 1143   Date/Time.....C
-00002df0: 6c6f 7365 6454 7261 6465 734d 6f64 656c  losedTradesModel
-00002e00: 0103 0000 001a 0426 0435 043d 0430 0020  .......&.5.=.0. 
-00002e10: 043e 0442 043a 0440 044b 0442 0438 044f  .>.B.:.@.K.B.8.O
-00002e20: 0800 0000 0006 0000 000a 4f70 656e 2050  ..........Open P
-00002e30: 7269 6365 0700 0000 1143 6c6f 7365 6454  rice.....ClosedT
-00002e40: 7261 6465 734d 6f64 656c 0103 0000 0006  radesModel......
-00002e50: 041f 0438 0423 0800 0000 0006 0000 0003  ...8.#..........
-00002e60: 502f 4c07 0000 0011 436c 6f73 6564 5472  P/L.....ClosedTr
-00002e70: 6164 6573 4d6f 6465 6c01 0300 0000 0c04  adesModel.......
-00002e80: 1f04 3804 2300 2c00 2000 2508 0000 0000  ..8.#.,. .%.....
-00002e90: 0600 0000 0650 2f4c 2c20 2507 0000 0011  .....P/L, %.....
-00002ea0: 436c 6f73 6564 5472 6164 6573 4d6f 6465  ClosedTradesMode
-00002eb0: 6c01 0300 0000 0c04 1a04 3e04 3b00 2d04  l.........>.;.-.
-00002ec0: 3204 3e08 0000 0000 0600 0000 0351 7479  2.>..........Qty
-00002ed0: 0700 0000 1143 6c6f 7365 6454 7261 6465  .....ClosedTrade
-00002ee0: 734d 6f64 656c 0103 0000 00a0 041a 043e  sModel.........>
-00002ef0: 043b 0438 0447 0435 0442 0432 043e 0020  .;.8.G.5.B.2.>. 
-00002f00: 0446 0435 043d 043d 044b 0445 0020 0431  .F.5.=.=.K.E. .1
-00002f10: 0443 043c 0430 0433 0020 043d 0435 0434  .C.<.0.3. .=.5.4
-00002f20: 043e 0441 0442 0430 0442 043e 0447 043d  .>.A.B.0.B.>.G.=
-00002f30: 043e 0020 0434 043b 044f 0020 043e 0431  .>. .4.;.O. .>.1
-00002f40: 0440 0430 0431 043e 0442 043a 0438 0020  .@.0.1.>.B.:.8. 
-00002f50: 043a 043e 0440 043f 043e 0440 0430 0442  .:.>.@.?.>.@.0.B
-00002f60: 0438 0432 043d 043e 0433 043e 0020 0441  .8.2.=.>.3.>. .A
-00002f70: 043e 0431 044b 0442 0438 044f 002e 0020  .>.1.K.B.8.O... 
-00002f80: 0414 0430 0442 0430 003a 0020 0800 0000  ...0.B.0.:. ....
-00002f90: 0006 0000 0042 4173 7365 7420 616d 6f75  .....BAsset amou
-00002fa0: 6e74 2069 7320 6e6f 7420 656e 6f75 6768  nt is not enough
-00002fb0: 2066 6f72 2063 6f72 706f 7261 7465 2061   for corporate a
-00002fc0: 6374 696f 6e20 7072 6f63 6573 7369 6e67  ction processing
-00002fd0: 2e20 4461 7465 3a20 0700 0000 0f43 6f72  . Date: .....Cor
-00002fe0: 706f 7261 7465 4163 7469 6f6e 0103 0000  porateAction....
-00002ff0: 0074 0426 0411 0020 043d 0435 0020 044f  .t.&... .=.5. .O
-00003000: 0432 043b 044f 0435 0442 0441 044f 0020  .2.;.O.5.B.A.O. 
-00003010: 0447 0430 0441 0442 044c 044e 0020 0440  .G.0.A.B.L.N. .@
-00003020: 0435 0437 0443 043b 044c 0442 0430 0442  .5.7.C.;.L.B.0.B
-00003030: 043e 0432 0020 043a 043e 0440 043f 043e  .>.2. .:.>.@.?.>
-00003040: 0440 0430 0442 0438 0432 043d 043e 0433  .@.0.B.8.2.=.>.3
-00003050: 043e 0020 0441 043e 0431 044b 0442 0438  .>. .A.>.1.K.B.8
-00003060: 044f 003a 0020 0800 0000 0006 0000 0030  .O.:. .........0
-00003070: 4173 7365 7420 6973 6e27 7420 6120 7061  Asset isn't a pa
-00003080: 7274 206f 6620 636f 7270 6f72 6174 6520  rt of corporate 
-00003090: 6163 7469 6f6e 2072 6573 756c 7473 3a20  action results: 
-000030a0: 0700 0000 0f43 6f72 706f 7261 7465 4163  .....CorporateAc
-000030b0: 7469 6f6e 0103 0000 0056 041d 0435 0020  tion.....V...5. 
-000030c0: 0437 0430 0434 0430 043d 0020 0442 0438  .7.0.4.0.=. .B.8
-000030d0: 043f 0020 043a 043e 0440 043f 043e 0440  .?. .:.>.@.?.>.@
-000030e0: 0430 0442 0438 0432 043d 043e 0433 043e  .0.B.8.2.=.>.3.>
-000030f0: 0020 0441 043e 0431 044b 0442 0438 044f  . .A.>.1.K.B.8.O
-00003100: 002e 0020 0414 0430 0442 0430 003a 0020  ... ...0.B.0.:. 
-00003110: 0800 0000 0006 0000 002b 436f 7270 6f72  .........+Corpor
-00003120: 6174 6520 6163 7469 6f6e 2074 7970 6520  ate action type 
-00003130: 6973 6e27 7420 6465 6669 6e65 642e 2044  isn't defined. D
-00003140: 6174 653a 2007 0000 000f 436f 7270 6f72  ate: .....Corpor
-00003150: 6174 6541 6374 696f 6e01 0300 0000 1204  ateAction.......
-00003160: 1404 3504 3b04 3804 4104 4204 3804 3d04  ..5.;.8.A.B.8.=.
-00003170: 3308 0000 0000 0600 0000 0944 656c 6973  3..........Delis
-00003180: 7469 6e67 0700 0000 0f43 6f72 706f 7261  ting.....Corpora
-00003190: 7465 4163 7469 6f6e 0103 0000 002c 0420  teAction.....,. 
-000031a0: 0435 043e 0440 0433 0430 043d 0438 0437  .5.>.@.3.0.=.8.7
-000031b0: 0430 0446 0438 044f 0020 043a 043e 043c  .0.F.8.O. .:.>.<
-000031c0: 043f 0430 043d 0438 0438 0800 0000 0006  .?.0.=.8.8......
-000031d0: 0000 0006 4d65 7267 6572 0700 0000 0f43  ....Merger.....C
-000031e0: 6f72 706f 7261 7465 4163 7469 6f6e 0103  orporateAction..
-000031f0: 0000 00ac 0420 0435 0437 0443 043b 044c  ..... .5.7.C.;.L
-00003200: 0442 0430 0442 044b 0020 043a 043e 0440  .B.0.B.K. .:.>.@
-00003210: 043f 043e 0440 0430 0442 0438 0432 043d  .?.>.@.0.B.8.2.=
-00003220: 043e 0433 043e 0020 0441 043e 0431 044b  .>.3.>. .A.>.1.K
-00003230: 0442 0438 044f 0020 043d 0435 0020 0440  .B.8.O. .=.5. .@
-00003240: 0430 0441 043f 0440 0435 0434 0435 043b  .0.A.?.@.5.4.5.;
-00003250: 044f 044e 0442 0020 0031 0030 0030 0025  .O.N.B. .1.0.0.%
-00003260: 0020 0441 0442 043e 0438 043c 043e 0441  . .A.B.>.8.<.>.A
-00003270: 0442 0438 0020 0438 0437 043d 0430 0447  .B.8. .8.7.=.0.G
-00003280: 0430 043b 044c 043d 043e 0433 043e 0020  .0.;.L.=.>.3.>. 
-00003290: 0430 043a 0442 0438 0432 0430 002e 0020  .0.:.B.8.2.0... 
-000032a0: 0800 0000 0006 0000 004d 5265 7375 6c74  .........MResult
-000032b0: 7320 7661 6c75 6520 6f66 2063 6f72 706f  s value of corpo
-000032c0: 7261 7465 2061 6374 696f 6e20 646f 6573  rate action does
-000032d0: 6e27 7420 6d61 7463 6820 3130 3025 206f  n't match 100% o
-000032e0: 6620 696e 6974 6961 6c20 6173 7365 7420  f initial asset 
-000032f0: 7661 6c75 652e 2007 0000 000f 436f 7270  value. .....Corp
-00003300: 6f72 6174 6541 6374 696f 6e01 0300 0000  orateAction.....
-00003310: 3a04 1204 4b04 3404 3504 3b04 3504 3d04  :...K.4.5.;.5.=.
-00003320: 3804 3500 2004 3a04 3e04 3c04 3f04 3004  8.5. .:.>.<.?.0.
-00003330: 3d04 3804 3800 2000 2804 4104 3f04 3804  =.8.8. .(.A.?.8.
-00003340: 3d00 2d04 3e04 4404 4400 2908 0000 0000  =.-.>.D.D.).....
-00003350: 0600 0000 0853 7069 6e2d 6f66 6607 0000  .....Spin-off...
-00003360: 000f 436f 7270 6f72 6174 6541 6374 696f  ..CorporateActio
-00003370: 6e01 0300 0000 0a04 2104 3f04 3b04 3804  n.......!.?.;.8.
-00003380: 4208 0000 0000 0600 0000 0553 706c 6974  B..........Split
-00003390: 0700 0000 0f43 6f72 706f 7261 7465 4163  .....CorporateAc
-000033a0: 7469 6f6e 0103 0000 001a 0421 043c 0435  tion.......!.<.5
-000033b0: 043d 0430 0020 0441 0438 043c 0432 043e  .=.0. .A.8.<.2.>
-000033c0: 043b 0430 0800 0000 0006 0000 000d 5379  .;.0..........Sy
-000033d0: 6d62 6f6c 2063 6861 6e67 6507 0000 000f  mbol change.....
-000033e0: 436f 7270 6f72 6174 6541 6374 696f 6e01  CorporateAction.
-000033f0: 0300 0000 1804 1d04 1504 1e04 1f04 2004  .............. .
-00003400: 1504 1404 1504 1b04 1504 1d04 1e08 0000  ................
-00003410: 0000 0600 0000 0955 4e44 4546 494e 4544  .......UNDEFINED
-00003420: 0700 0000 0f43 6f72 706f 7261 7465 4163  .....CorporateAc
-00003430: 7469 6f6e 0103 0000 00ae 041d 0435 043f  tion.........5.?
-00003440: 043e 0434 0435 0440 0436 0438 0432 0430  .>.4.5.@.6.8.2.0
-00003450: 0435 043c 044b 0439 0020 0441 043b 0443  .5.<.K.9. .A.;.C
-00003460: 0447 0430 0439 003a 0020 041a 043e 0440  .G.0.9.:. ...>.@
-00003470: 043f 043e 0440 0430 0442 0438 0432 043d  .?.>.@.0.B.8.2.=
-00003480: 043e 0435 0020 0441 043e 0431 044b 0442  .>.5. .A.>.1.K.B
-00003490: 0438 0435 0020 043f 043e 043a 0440 044b  .8.5. .?.>.:.@.K
-000034a0: 0432 0430 0435 0442 0020 043d 0435 0020  .2.0.5.B. .=.5. 
-000034b0: 0432 0441 044e 0020 043e 0442 043a 0440  .2.A.N. .>.B.:.@
-000034c0: 044b 0442 0443 044e 0020 043f 043e 0437  .K.B.C.N. .?.>.7
-000034d0: 0438 0446 0438 044e 002e 0020 0414 0430  .8.F.8.N... ...0
-000034e0: 0442 0430 003a 0020 0800 0000 0006 0000  .B.0.:. ........
-000034f0: 0046 556e 6861 6e64 6c65 6420 6361 7365  .FUnhandled case
-00003500: 3a20 436f 7270 6f72 6174 6520 6163 7469  : Corporate acti
-00003510: 6f6e 2063 6f76 6572 7320 6e6f 7420 6675  on covers not fu
-00003520: 6c6c 206f 7065 6e20 706f 7369 7469 6f6e  ll open position
-00003530: 2e20 4461 7465 3a20 0700 0000 0f43 6f72  . Date: .....Cor
-00003540: 706f 7261 7465 4163 7469 6f6e 0103 0000  porateAction....
-00003550: 0002 2116 0800 0000 0006 0000 0001 2307  ..!...........#.
-00003560: 0000 0015 436f 7270 6f72 6174 6541 6374  ....CorporateAct
-00003570: 696f 6e57 6964 6765 7401 0300 0000 0804  ionWidget.......
-00003580: 2104 4704 3504 4208 0000 0000 0600 0000  !.G.5.B.........
-00003590: 0741 6363 6f75 6e74 0700 0000 1543 6f72  .Account.....Cor
-000035a0: 706f 7261 7465 4163 7469 6f6e 5769 6467  porateActionWidg
-000035b0: 6574 0103 0000 001c 0414 043e 0431 0430  et.........>.1.0
-000035c0: 0432 0438 0442 044c 0020 0430 043a 0442  .2.8.B.L. .0.:.B
-000035d0: 0438 0432 0800 0000 0006 0000 0009 4164  .8.2..........Ad
-000035e0: 6420 6173 7365 7407 0000 0015 436f 7270  d asset.....Corp
-000035f0: 6f72 6174 6541 6374 696f 6e57 6964 6765  orateActionWidge
-00003600: 7401 0300 0000 0404 2604 1108 0000 0000  t.......&.......
-00003610: 0600 0000 0541 7373 6574 0700 0000 1543  .....Asset.....C
-00003620: 6f72 706f 7261 7465 4163 7469 6f6e 5769  orporateActionWi
-00003630: 6467 6574 0103 0000 002c 041a 043e 0440  dget.....,...>.@
-00003640: 043f 043e 0440 0430 0442 0438 0432 043d  .?.>.@.0.B.8.2.=
-00003650: 043e 0435 0020 0434 0435 0439 0441 0442  .>.5. .4.5.9.A.B
-00003660: 0432 0438 0435 0800 0000 0006 0000 0010  .2.8.5..........
-00003670: 436f 7270 6f72 6174 6520 4163 7469 6f6e  Corporate Action
-00003680: 0700 0000 1543 6f72 706f 7261 7465 4163  .....CorporateAc
-00003690: 7469 6f6e 5769 6467 6574 0103 0000 0014  tionWidget......
-000036a0: 0414 0430 0442 0430 002f 0412 0440 0435  ...0.B.0./...@.5
-000036b0: 043c 044f 0800 0000 0006 0000 0009 4461  .<.O..........Da
-000036c0: 7465 2f54 696d 6507 0000 0015 436f 7270  te/Time.....Corp
-000036d0: 6f72 6174 6541 6374 696f 6e57 6964 6765  orateActionWidge
-000036e0: 7401 0300 0000 1204 1404 3504 3b04 3804  t.........5.;.8.
-000036f0: 4104 4204 3804 3d04 3308 0000 0000 0600  A.B.8.=.3.......
-00003700: 0000 0944 656c 6973 7469 6e67 0700 0000  ...Delisting....
-00003710: 1543 6f72 706f 7261 7465 4163 7469 6f6e  .CorporateAction
-00003720: 5769 6467 6574 0103 0000 0044 041d 0435  Widget.....D...5
-00003730: 0432 043e 0437 043c 043e 0436 043d 043e  .2.>.7.<.>.6.=.>
-00003740: 0020 0434 043e 0431 0430 0432 0438 0442  . .4.>.1.0.2.8.B
-00003750: 044c 0020 043d 043e 0432 0443 044e 0020  .L. .=.>.2.C.N. 
-00003760: 0437 0430 043f 0438 0441 044c 003a 0020  .7.0.?.8.A.L.:. 
-00003770: 0800 0000 0006 0000 001a 4661 696c 6564  ..........Failed
-00003780: 2074 6f20 6164 6420 6e65 7720 7265 636f   to add new reco
-00003790: 7264 3a20 0700 0000 1543 6f72 706f 7261  rd: .....Corpora
-000037a0: 7465 4163 7469 6f6e 5769 6467 6574 0103  teActionWidget..
-000037b0: 0000 0028 041e 0431 044a 0435 0434 0438  ...(...1.J.5.4.8
-000037c0: 043d 0435 043d 0438 0435 0020 043a 043e  .=.5.=.8.5. .:.>
-000037d0: 043c 043f 0430 043d 0438 0438 0800 0000  .<.?.0.=.8.8....
-000037e0: 0006 0000 0006 4d65 7267 6572 0700 0000  ......Merger....
-000037f0: 1543 6f72 706f 7261 7465 4163 7469 6f6e  .CorporateAction
-00003800: 5769 6467 6574 0103 0000 0006 004e 002f  Widget.......N./
-00003810: 0041 0800 0000 0006 0000 0003 4e2f 4107  .A..........N/A.
-00003820: 0000 0015 436f 7270 6f72 6174 6541 6374  ....CorporateAct
-00003830: 696f 6e57 6964 6765 7401 0300 0000 1004  ionWidget.......
-00003840: 1e04 3f04 3804 4104 3004 3d04 3804 3508  ..?.8.A.0.=.8.5.
-00003850: 0000 0000 0600 0000 044e 6f74 6507 0000  .........Note...
-00003860: 0015 436f 7270 6f72 6174 6541 6374 696f  ..CorporateActio
-00003870: 6e57 6964 6765 7401 0300 0000 4804 1e04  nWidget.....H...
-00003880: 4804 3804 3104 3a04 3000 2004 3f04 4004  H.8.1.:.0. .?.@.
-00003890: 3800 2004 3704 3004 3f04 3804 4104 3800  8. .7.0.?.8.A.8.
-000038a0: 2004 3404 3504 4204 3004 3b04 3504 3900   .4.5.B.0.;.5.9.
-000038b0: 2004 3e04 3f04 3504 4004 3004 4604 3804   .>.?.5.@.0.F.8.
-000038c0: 3800 3a00 2008 0000 0000 0600 0000 214f  8.:. .........!O
-000038d0: 7065 7261 7469 6f6e 2064 6574 6169 6c73  peration details
-000038e0: 2073 7562 6d69 7420 6661 696c 6564 3a20   submit failed: 
-000038f0: 0700 0000 1543 6f72 706f 7261 7465 4163  .....CorporateAc
-00003900: 7469 6f6e 5769 6467 6574 0103 0000 0038  tionWidget.....8
-00003910: 041e 0448 0438 0431 043a 0430 0020 043f  ...H.8.1.:.0. .?
-00003920: 0440 0438 0020 0437 0430 043f 0438 0441  .@.8. .7.0.?.8.A
-00003930: 0438 0020 043e 043f 0435 0440 0430 0446  .8. .>.?.5.@.0.F
-00003940: 0438 0438 003a 0020 0800 0000 0006 0000  .8.8.:. ........
-00003950: 0019 4f70 6572 6174 696f 6e20 7375 626d  ..Operation subm
-00003960: 6974 2066 6169 6c65 643a 2007 0000 0015  it failed: .....
-00003970: 436f 7270 6f72 6174 6541 6374 696f 6e57  CorporateActionW
-00003980: 6964 6765 7401 0300 0000 0c04 1a04 3e04  idget.........>.
-00003990: 3b00 2d04 3204 3e08 0000 0000 0600 0000  ;.-.2.>.........
-000039a0: 0351 7479 0700 0000 1543 6f72 706f 7261  .Qty.....Corpora
-000039b0: 7465 4163 7469 6f6e 5769 6467 6574 0103  teActionWidget..
-000039c0: 0000 001a 0423 0434 0430 043b 0438 0442  .....#.4.0.;.8.B
-000039d0: 044c 0020 0430 043a 0442 0438 0432 0800  .L. .0.:.B.8.2..
-000039e0: 0000 0006 0000 000c 5265 6d6f 7665 2061  ........Remove a
-000039f0: 7373 6574 0700 0000 1543 6f72 706f 7261  sset.....Corpora
-00003a00: 7465 4163 7469 6f6e 5769 6467 6574 0103  teActionWidget..
-00003a10: ffff ffff 0800 0000 0006 0000 0008 5370  ..............Sp
-00003a20: 696e 2d4f 6666 0700 0000 1543 6f72 706f  in-Off.....Corpo
-00003a30: 7261 7465 4163 7469 6f6e 5769 6467 6574  rateActionWidget
-00003a40: 0103 0000 000a 0421 043f 043b 0438 0442  .......!.?.;.8.B
-00003a50: 0800 0000 0006 0000 0005 5370 6c69 7407  ..........Split.
-00003a60: 0000 0015 436f 7270 6f72 6174 6541 6374  ....CorporateAct
-00003a70: 696f 6e57 6964 6765 7401 0300 0000 1a04  ionWidget.......
-00003a80: 2104 3c04 3504 3d04 3000 2004 4104 3804  !.<.5.=.0. .A.8.
-00003a90: 3c04 3204 3e04 3b04 3008 0000 0000 0600  <.2.>.;.0.......
-00003aa0: 0000 0d53 796d 626f 6c20 6368 616e 6765  ...Symbol change
-00003ab0: 0700 0000 1543 6f72 706f 7261 7465 4163  .....CorporateAc
-00003ac0: 7469 6f6e 5769 6467 6574 0103 0000 0006  tionWidget......
-00003ad0: 0422 0438 043f 0800 0000 0006 0000 0004  .".8.?..........
-00003ae0: 5479 7065 0700 0000 1543 6f72 706f 7261  Type.....Corpora
-00003af0: 7465 4163 7469 6f6e 5769 6467 6574 0103  teActionWidget..
-00003b00: 0000 0034 0424 043e 0440 043c 0430 0442  ...4.$.>.@.<.0.B
-00003b10: 0020 0431 0430 0437 044b 0020 0434 0430  . .1.0.7.K. .4.0
-00003b20: 043d 043d 044b 0445 0020 0443 0441 0442  .=.=.K.E. .C.A.B
-00003b30: 0430 0440 0435 043b 0800 0000 0006 0000  .0.@.5.;........
-00003b40: 001b 4461 7461 6261 7365 2066 6f72 6d61  ..Database forma
-00003b50: 7420 6973 206f 7574 6461 7465 6407 0000  t is outdated...
-00003b60: 0002 4442 0103 0000 0064 0412 044b 0020  ..DB.....d...K. 
-00003b70: 0441 043e 0433 043b 0430 0441 043d 044b  .A.>.3.;.0.A.=.K
-00003b80: 0020 0441 043a 043e 043d 0432 0435 0440  . .A.:.>.=.2.5.@
-00003b90: 0442 0438 0440 043e 0432 0430 0442 044c  .B.8.@.>.2.0.B.L
-00003ba0: 0020 0434 0430 043d 043d 044b 0435 0020  . .4.0.=.=.K.5. 
-00003bb0: 0432 0020 043d 043e 0432 044b 0439 0020  .2. .=.>.2.K.9. 
-00003bc0: 0444 043e 0440 043c 0430 0442 003f 0800  .D.>.@.<.0.B.?..
-00003bd0: 0000 0006 0000 0032 446f 2079 6f75 2061  .......2Do you a
-00003be0: 6772 6565 2074 6f20 7570 6772 6164 6520  gree to upgrade 
-00003bf0: 796f 7572 2064 6174 6120 746f 206e 6577  your data to new
-00003c00: 6572 2066 6f72 6d61 743f 0700 0000 0244  er format?.....D
-00003c10: 4201 0300 0000 5e04 2404 3e04 4004 3c04  B.....^.$.>.@.<.
-00003c20: 3000 2000 3300 2d04 1d04 1404 2404 1b00  0. .3.-.....$...
-00003c30: 2004 3404 3b04 4f00 2004 4d04 4204 3e04   .4.;.O. .M.B.>.
-00003c40: 3304 3e00 2004 3304 3e04 3404 3000 2004  3.>. .3.>.4.0. .
-00003c50: 3d04 3500 2004 3f04 3e04 3404 3404 3504  =.5. .?.>.4.4.5.
-00003c60: 4004 3604 3804 3204 3004 3504 4204 4104  @.6.8.2.0.5.B.A.
-00003c70: 4f00 3a00 2008 0000 0000 0600 0000 2633  O.:. .........&3
-00003c80: 2d4e 4446 4c20 666f 726d 2069 736e 2774  -NDFL form isn't
-00003c90: 2073 7570 6f6f 7274 6564 2066 6f72 2079   supoorted for y
-00003ca0: 6561 723a 2007 0000 0004 444c 5347 0103  ear: .....DLSG..
-00003cb0: 0000 0086 0421 0442 0440 0430 043d 0430  .....!.B.@.0.=.0
-00003cc0: 0020 0426 0411 0020 043d 0435 0020 0437  . .&... .=.5. .7
-00003cd0: 0430 0434 0430 043d 0430 002c 0020 0434  .0.4.0.=.0.,. .4
-00003ce0: 0438 0432 0438 0434 0435 043d 0434 0020  .8.2.8.4.5.=.4. 
-00003cf0: 043d 0435 0020 0431 0443 0434 0435 0442  .=.5. .1.C.4.5.B
-00003d00: 0020 0432 043a 043b 044e 0447 0451 043d  . .2.:.;.N.G.Q.=
-00003d10: 0020 0432 0020 0434 0435 043a 043b 0430  . .2. .4.5.:.;.0
-00003d20: 0440 0430 0446 0438 044e 0020 0033 002d  .@.0.F.8.N. .3.-
-00003d30: 041d 0424 0414 041b 0020 0800 0000 0006  ...$..... ......
-00003d40: 0000 0047 4163 636f 756e 7420 636f 756e  ...GAccount coun
-00003d50: 7472 7920 6973 206e 6f74 2073 6574 2066  try is not set f
-00003d60: 6f72 2061 7373 6574 2c20 6469 7669 6465  or asset, divide
-00003d70: 6e64 2069 736e 2774 2069 6e63 6c75 6465  nd isn't include
-00003d80: 2069 6e20 332d 4e44 464c 2007 0000 0004   in 3-NDFL .....
-00003d90: 444c 5347 0103 0000 004a 0412 0430 043b  DLSG.....J...0.;
-00003da0: 044e 0442 0430 0020 043d 0435 0020 043f  .N.B.0. .=.5. .?
-00003db0: 043e 0434 0434 0435 0440 0436 0438 0432  .>.4.4.5.@.6.8.2
-00003dc0: 0430 0435 0442 0441 044f 0020 0434 043b  .0.5.B.A.O. .4.;
-00003dd0: 044f 0020 0033 002d 041d 0414 0424 041b  .O. .3.-.....$..
-00003de0: 003a 0020 0800 0000 0006 0000 0026 4375  .:. .........&Cu
-00003df0: 7272 656e 6379 2069 7320 6e6f 7420 7375  rrency is not su
-00003e00: 7070 6f72 7465 6420 666f 7220 332d 4e44  pported for 3-ND
-00003e10: 464c 3a20 0700 0000 0444 4c53 4701 0300  FL: .....DLSG...
-00003e20: 0000 1404 4d04 3a04 4104 3f04 3804 4004  ....M.:.A.?.8.@.
-00003e30: 3004 4604 3804 4f08 0000 0000 0600 0000  0.F.8.O.........
-00003e40: 0665 7870 6972 7907 0000 000c 4461 7461  .expiry.....Data
-00003e50: 4465 6c65 6761 7465 0103 0000 000e 043d  Delegate.......=
-00003e60: 043e 043c 0438 043d 0430 043b 0800 0000  .>.<.8.=.0.;....
-00003e70: 0006 0000 0009 7072 696e 6369 7061 6c07  ......principal.
-00003e80: 0000 000c 4461 7461 4465 6c65 6761 7465  ....DataDelegate
-00003e90: 0103 0000 000e 0440 0435 0433 002e 043a  .......@.5.3...:
-00003ea0: 043e 0434 0800 0000 0006 0000 0008 7265  .>.4..........re
-00003eb0: 672e 636f 6465 0700 0000 0c44 6174 6144  g.code.....DataD
-00003ec0: 656c 6567 6174 6501 0300 0000 1004 1204  elegate.........
-00003ed0: 4104 3500 2004 3404 3004 4204 4b08 0000  A.5. .4.0.B.K...
-00003ee0: 0000 0600 0000 0941 6c6c 2064 6174 6573  .......All dates
-00003ef0: 0700 0000 1144 6174 6552 616e 6765 5365  .....DateRangeSe
-00003f00: 6c65 6374 6f72 0103 0000 0004 0421 003a  lector.......!.:
-00003f10: 0800 0000 0006 0000 0005 4672 6f6d 3a07  ..........From:.
-00003f20: 0000 0011 4461 7465 5261 6e67 6553 656c  ....DateRangeSel
-00003f30: 6563 746f 7201 0300 0000 0a04 1c04 3504  ector.........5.
-00003f40: 4104 4f04 4608 0000 0000 0600 0000 054d  A.O.F..........M
-00003f50: 6f6e 7468 0700 0000 1144 6174 6552 616e  onth.....DateRan
-00003f60: 6765 5365 6c65 6374 6f72 0103 0000 001c  geSelector......
-00003f70: 041f 0440 0435 0434 044b 0434 0443 0449  ...@.5.4.K.4.C.I
-00003f80: 0438 0439 0020 0433 043e 0434 0800 0000  .8.9. .3.>.4....
-00003f90: 0006 0000 000d 5072 6576 696f 7573 2079  ......Previous y
-00003fa0: 6561 7207 0000 0011 4461 7465 5261 6e67  ear.....DateRang
-00003fb0: 6553 656c 6563 746f 7201 0300 0000 0e04  eSelector.......
-00003fc0: 1a04 3204 3004 4004 4204 3004 3b08 0000  ..2.0.@.B.0.;...
-00003fd0: 0000 0600 0000 0751 7561 7274 6572 0700  .......Quarter..
-00003fe0: 0000 1144 6174 6552 616e 6765 5365 6c65  ...DateRangeSele
-00003ff0: 6374 6f72 0103 0000 0024 0422 0435 043a  ctor.....$.".5.:
-00004000: 0443 0449 0438 0439 0020 0434 043e 0020  .C.I.8.9. .4.>. 
-00004010: 0441 0435 0433 043e 0434 043d 044f 0800  .A.5.3.>.4.=.O..
-00004020: 0000 0006 0000 000f 5175 6172 7465 7220  ........Quarter 
-00004030: 746f 2064 6174 6507 0000 0011 4461 7465  to date.....Date
-00004040: 5261 6e67 6553 656c 6563 746f 7201 0300  RangeSelector...
-00004050: 0000 1604 2204 3504 3a04 4304 4904 3804  ....".5.:.C.I.8.
-00004060: 3900 2004 3304 3e04 3408 0000 0000 0600  9. .3.>.4.......
-00004070: 0000 0954 6869 7320 7965 6172 0700 0000  ...This year....
-00004080: 1144 6174 6552 616e 6765 5365 6c65 6374  .DateRangeSelect
-00004090: 6f72 0103 0000 0006 0414 043e 003a 0800  or.........>.:..
-000040a0: 0000 0006 0000 0003 546f 3a07 0000 0011  ........To:.....
-000040b0: 4461 7465 5261 6e67 6553 656c 6563 746f  DateRangeSelecto
-000040c0: 7201 0300 0000 0c04 1d04 3504 3404 3504  r.........5.4.5.
-000040d0: 3b04 4f08 0000 0000 0600 0000 0457 6565  ;.O..........Wee
-000040e0: 6b07 0000 0011 4461 7465 5261 6e67 6553  k.....DateRangeS
-000040f0: 656c 6563 746f 7201 0300 0000 0604 1304  elector.........
-00004100: 3e04 3408 0000 0000 0600 0000 0459 6561  >.4..........Yea
-00004110: 7207 0000 0011 4461 7465 5261 6e67 6553  r.....DateRangeS
-00004120: 656c 6563 746f 7201 0300 0000 1c04 1304  elector.........
-00004130: 3e04 3400 2004 3404 3e00 2004 4104 3504  >.4. .4.>. .A.5.
-00004140: 3304 3e04 3404 3d04 4f08 0000 0000 0600  3.>.4.=.O.......
-00004150: 0000 0c59 6561 7220 746f 2064 6174 6507  ...Year to date.
-00004160: 0000 0011 4461 7465 5261 6e67 6553 656c  ....DateRangeSel
-00004170: 6563 746f 7201 0300 0000 1e04 2104 3404  ector.......!.4.
-00004180: 3504 3b04 3a04 3800 2004 3f04 3e00 2004  5.;.:.8. .?.>. .
-00004190: 4104 4704 3504 4204 4308 0000 0000 0600  A.G.5.B.C.......
-000041a0: 0000 1044 6561 6c73 2062 7920 4163 636f  ...Deals by Acco
-000041b0: 756e 7407 0000 000b 4465 616c 7352 6570  unt.....DealsRep
-000041c0: 6f72 7401 0300 0000 0a04 2104 4704 3504  ort.......!.G.5.
-000041d0: 4200 3a08 0000 0000 0600 0000 0841 6363  B.:..........Acc
-000041e0: 6f75 6e74 3a07 0000 0011 4465 616c 7352  ount:.....DealsR
-000041f0: 6570 6f72 7457 6964 6765 7401 0300 0000  eportWidget.....
-00004200: 0c04 2104 3404 3504 3b04 3a04 3808 0000  ..!.4.5.;.:.8...
-00004210: 0000 0600 0000 0544 6561 6c73 0700 0000  .......Deals....
-00004220: 1144 6561 6c73 5265 706f 7274 5769 6467  .DealsReportWidg
-00004230: 6574 0103 0000 0020 0413 0440 0443 043f  et..... ...@.C.?
-00004240: 043f 0438 0440 043e 0432 0430 0442 044c  .?.8.@.>.2.0.B.L
-00004250: 0020 043f 043e 003a 0800 0000 0006 0000  . .?.>.:........
-00004260: 0009 4772 6f75 7020 6279 3a07 0000 0011  ..Group by:.....
-00004270: 4465 616c 7352 6570 6f72 7457 6964 6765  DealsReportWidge
-00004280: 7401 0300 0000 0e00 3c04 1f04 4304 4104  t.......<...C.A.
-00004290: 4204 3e00 3e08 0000 0000 0600 0000 063c  B.>.>..........<
-000042a0: 4e6f 6e65 3e07 0000 0011 4465 616c 7352  None>.....DealsR
-000042b0: 6570 6f72 7457 696e 646f 7701 0300 0000  eportWindow.....
-000042c0: 1a04 2604 3504 3d04 3d04 3004 4f00 2004  ..&.5.=.=.0.O. .
-000042d0: 3104 4304 3c04 3004 3304 3008 0000 0000  1.C.<.0.3.0.....
-000042e0: 0600 0000 0541 7373 6574 0700 0000 1144  .....Asset.....D
-000042f0: 6561 6c73 5265 706f 7274 5769 6e64 6f77  ealsReportWindow
-00004300: 0103 0000 0030 0426 0411 0020 002d 0020  .....0.&... .-. 
-00004310: 041e 0442 043a 0440 044b 0442 0438 0435  ...B.:.@.K.B.8.5
-00004320: 0020 002d 0020 0417 0430 043a 0440 044b  . .-. ...0.:.@.K
-00004330: 0442 0438 0435 0800 0000 0006 0000 0014  .B.8.5..........
-00004340: 4173 7365 7420 2d20 4f70 656e 202d 2043  Asset - Open - C
-00004350: 6c6f 7365 0700 0000 1144 6561 6c73 5265  lose.....DealsRe
-00004360: 706f 7274 5769 6e64 6f77 0103 0000 0010  portWindow......
-00004370: 0417 0430 043a 0440 044b 0442 0438 0435  ...0.:.@.K.B.8.5
-00004380: 0800 0000 0006 0000 0005 436c 6f73 6507  ..........Close.
-00004390: 0000 0011 4465 616c 7352 6570 6f72 7457  ....DealsReportW
-000043a0: 696e 646f 7701 0300 0000 2604 1704 3004  indow.....&...0.
-000043b0: 3a04 4004 4b04 4204 3804 3500 2000 2d00  :.@.K.B.8.5. .-.
-000043c0: 2004 1e04 4204 3a04 4004 4b04 4204 3804   ...B.:.@.K.B.8.
-000043d0: 3508 0000 0000 0600 0000 0c43 6c6f 7365  5..........Close
-000043e0: 202d 204f 7065 6e07 0000 0011 4465 616c   - Open.....Deal
-000043f0: 7352 6570 6f72 7457 696e 646f 7701 0300  sReportWindow...
-00004400: 0000 2604 1e04 4204 3a04 4004 4b04 4204  ..&...B.:.@.K.B.
-00004410: 3804 3500 2000 2d00 2004 1704 3004 3a04  8.5. .-. ...0.:.
-00004420: 4004 4b04 4204 3804 3508 0000 0000 0600  @.K.B.8.5.......
-00004430: 0000 0c4f 7065 6e20 2d20 436c 6f73 6507  ...Open - Close.
-00004440: 0000 0011 4465 616c 7352 6570 6f72 7457  ....DealsReportW
-00004450: 696e 646f 7701 0300 0000 0a04 2104 4304  indow.......!.C.
-00004460: 3c04 3c04 3008 0000 0000 0600 0000 0641  <.<.0..........A
-00004470: 6d6f 756e 7407 0000 000c 4465 7461 696c  mount.....Detail
-00004480: 734d 6f64 656c 0103 0000 0012 041a 0430  sModel.........0
-00004490: 0442 0435 0433 043e 0440 0438 044f 0800  .B.5.3.>.@.8.O..
-000044a0: 0000 0006 0000 0008 4361 7465 676f 7279  ........Category
-000044b0: 0700 0000 0c44 6574 6169 6c73 4d6f 6465  .....DetailsMode
-000044c0: 6c01 0300 0000 1004 1e04 3f04 3804 4104  l.........?.8.A.
-000044d0: 3004 3d04 3804 3508 0000 0000 0600 0000  0.=.8.5.........
-000044e0: 044e 6f74 6507 0000 000c 4465 7461 696c  .Note.....Detail
-000044f0: 734d 6f64 656c 0103 0000 000a 041c 0435  sModel.........5
-00004500: 0442 043a 0430 0800 0000 0006 0000 0003  .B.:.0..........
-00004510: 5461 6707 0000 000c 4465 7461 696c 734d  Tag.....DetailsM
-00004520: 6f64 656c 0103 0000 009e 041d 0435 0432  odel.........5.2
-00004530: 043e 0437 043c 043e 0436 043d 043e 0020  .>.7.<.>.6.=.>. 
-00004540: 043e 0431 0440 0430 0431 043e 0442 0430  .>.1.@.0.1.>.B.0
-00004550: 0442 044c 0020 0434 0438 0432 0438 0434  .B.L. .4.8.2.8.4
-00004560: 0435 043d 0434 002c 0020 0442 002e 043a  .5.=.4.,. .B...:
-00004570: 002e 0020 043d 0435 0020 0443 043a 0430  ... .=.5. .C.:.0
-00004580: 0437 0430 043d 0020 0431 0430 043d 043a  .7.0.=. .1.0.=.:
-00004590: 0020 0434 043b 044f 0020 0438 043d 0432  . .4.;.O. .8.=.2
-000045a0: 0435 0441 0442 0438 0446 0438 043e 043d  .5.A.B.8.F.8.>.=
-000045b0: 043d 043e 0433 043e 0020 0441 0447 0451  .=.>.3.>. .A.G.Q
-000045c0: 0442 0430 003a 0020 0800 0000 0006 0000  .B.0.:. ........
-000045d0: 0041 4361 6e27 7420 7072 6f63 6573 7320  .ACan't process 
-000045e0: 6469 7669 6465 6e64 2061 7320 6261 6e6b  dividend as bank
-000045f0: 2069 736e 2774 2073 6574 2066 6f72 2069   isn't set for i
-00004600: 6e76 6573 746d 656e 7420 6163 636f 756e  nvestment accoun
-00004610: 743a 2007 0000 0008 4469 7669 6465 6e64  t: .....Dividend
-00004620: 0103 0000 005a 041d 0435 0020 0437 0430  .....Z...5. .7.0
-00004630: 0434 0430 043d 0430 0020 0446 0435 043d  .4.0.=.0. .F.5.=
-00004640: 0430 0020 0434 043b 044f 0020 0432 044b  .0. .4.;.O. .2.K
-00004650: 043f 043b 0430 0442 044b 0020 0446 0435  .?.;.0.B.K. .F.5
-00004660: 043d 043d 044b 043c 0438 0020 0431 0443  .=.=.K.<.8. .1.C
-00004670: 043c 0430 0433 0430 043c 0438 003a 0020  .<.0.3.0.<.8.:. 
-00004680: 0800 0000 0006 0000 002a 4e6f 2070 7269  .........*No pri
-00004690: 6365 2064 6174 6120 666f 7220 7374 6f63  ce data for stoc
-000046a0: 6b20 6469 7669 6465 6e64 2f76 6573 7469  k dividend/vesti
-000046b0: 6e67 3a20 0700 0000 0844 6976 6964 656e  ng: .....Dividen
-000046c0: 6401 0300 0000 7204 1d04 3504 4200 2004  d.....r...5.B. .
-000046d0: 3a04 3e04 4204 3804 4004 3e04 3204 3a04  :.>.B.8.@.>.2.:.
-000046e0: 3800 2004 3404 3b04 4f00 2004 3404 3804  8. .4.;.O. .4.8.
-000046f0: 3204 3804 3404 3504 3d04 3404 3000 2004  2.8.4.5.=.4.0. .
-00004700: 3004 3a04 4604 3804 4f04 3c04 3800 2004  0.:.F.8.O.<.8. .
-00004710: 3804 3b04 3800 2004 3704 3004 4704 3804  8.;.8. .7.0.G.8.
-00004720: 4104 3b04 3504 3d04 3804 4f00 2004 3004  A.;.5.=.8.O. .0.
-00004730: 3a04 4604 3804 3900 2e08 0000 0000 0600  :.F.8.9.........
-00004740: 0000 2d4e 6f20 7374 6f63 6b20 7175 6f74  ..-No stock quot
-00004750: 6520 666f 7220 7374 6f63 6b20 6469 7669  e for stock divi
-00004760: 6465 6e64 206f 7220 7665 7374 696e 672e  dend or vesting.
-00004770: 0700 0000 0844 6976 6964 656e 6401 0300  .....Dividend...
-00004780: 0000 b804 1d04 3504 3f04 3e04 3404 3404  ......5.?.>.4.4.
-00004790: 3504 4004 3604 3804 3204 3004 3504 3c04  5.@.6.8.2.0.5.<.
-000047a0: 3e04 3500 2004 3404 3504 3904 4104 4204  >.5. .4.5.9.A.B.
-000047b0: 3204 3804 3500 3a00 2004 3404 3804 3204  2.8.5.:. .4.8.2.
-000047c0: 3804 3404 3504 3d04 3400 2004 3004 3a04  8.4.5.=.4. .0.:.
-000047d0: 4604 3804 4f04 3c04 3800 2004 3804 3b04  F.8.O.<.8. .8.;.
-000047e0: 3800 2004 3704 3004 4704 3804 4104 3b04  8. .7.0.G.8.A.;.
-000047f0: 3504 3d04 3804 3500 2004 3004 3a04 4604  5.=.8.5. .0.:.F.
-00004800: 3804 3900 2004 3704 3004 3a04 4004 4b04  8.9. .7.0.:.@.K.
-00004810: 3204 3004 3504 4200 2004 3a04 3e04 4004  2.0.5.B. .:.>.@.
-00004820: 3e04 4204 3a04 4304 4e00 2004 3f04 3e04  >.B.:.C.N. .?.>.
-00004830: 3704 3804 4604 3804 4e00 2e08 0000 0000  7.8.F.8.N.......
-00004840: 0600 0000 434e 6f74 2073 7570 706f 7274  ....CNot support
-00004850: 6564 2061 6374 696f 6e3a 2073 746f 636b  ed action: stock
-00004860: 2064 6976 6964 656e 6420 6f72 2076 6573   dividend or ves
-00004870: 7469 6e67 2063 6c6f 7365 7320 7368 6f72  ting closes shor
-00004880: 7420 7472 6164 652e 0700 0000 0844 6976  t trade......Div
-00004890: 6964 656e 6401 0300 0000 0e04 1d04 3004  idend.........0.
-000048a0: 3b04 3e04 3300 3a00 2008 0000 0000 0600  ;.>.3.:. .......
-000048b0: 0000 0554 6178 3a20 0700 0000 0844 6976  ...Tax: .....Div
-000048c0: 6964 656e 6401 0300 0000 3e04 1d04 3504  idend.....>...5.
-000048d0: 3f04 3e04 3404 3404 3504 4004 3604 3804  ?.>.4.4.5.@.6.8.
-000048e0: 3204 3004 3504 3c04 4b04 3900 2004 4204  2.0.5.<.K.9. .B.
-000048f0: 3804 3f00 2004 3404 3804 3204 3804 3404  8.?. .4.8.2.8.4.
-00004900: 3504 3d04 3404 3000 2e08 0000 0000 0600  5.=.4.0.........
-00004910: 0000 1a55 6e73 7570 706f 7274 6564 2064  ...Unsupported d
-00004920: 6976 6964 656e 6420 7479 7065 2e07 0000  ividend type....
-00004930: 0008 4469 7669 6465 6e64 0103 0000 0002  ..Dividend......
-00004940: 2116 0800 0000 0006 0000 0001 2307 0000  !...........#...
-00004950: 000e 4469 7669 6465 6e64 5769 6467 6574  ..DividendWidget
-00004960: 0103 0000 0008 0421 0447 0435 0442 0800  .......!.G.5.B..
-00004970: 0000 0006 0000 0007 4163 636f 756e 7407  ........Account.
-00004980: 0000 000e 4469 7669 6465 6e64 5769 6467  ....DividendWidg
-00004990: 6574 0103 0000 0004 0426 0411 0800 0000  et.......&......
-000049a0: 0006 0000 0005 4173 7365 7407 0000 000e  ......Asset.....
-000049b0: 4469 7669 6465 6e64 5769 6467 6574 0103  DividendWidget..
-000049c0: 0000 000a 041a 0443 043f 043e 043d 0800  .......C.?.>.=..
-000049d0: 0000 0006 0000 000d 426f 6e64 2049 6e74  ........Bond Int
-000049e0: 6572 6573 7407 0000 000e 4469 7669 6465  erest.....Divide
-000049f0: 6e64 5769 6467 6574 0103 0000 0014 0414  ndWidget........
-00004a00: 0430 0442 0430 002f 0412 0440 0435 043c  .0.B.0./...@.5.<
-00004a10: 044f 0800 0000 0006 0000 0009 4461 7465  .O..........Date
-00004a20: 2f54 696d 6507 0000 000e 4469 7669 6465  /Time.....Divide
-00004a30: 6e64 5769 6467 6574 0103 0000 0010 0414  ndWidget........
-00004a40: 0438 0432 0438 0434 0435 043d 0434 0800  .8.2.8.4.5.=.4..
-00004a50: 0000 0006 0000 0008 4469 7669 6465 6e64  ........Dividend
-00004a60: 0700 0000 0e44 6976 6964 656e 6457 6964  .....DividendWid
-00004a70: 6765 7401 0300 0000 0e04 1e04 4204 4104  get.........B.A.
-00004a80: 3504 4704 3a04 3008 0000 0000 0600 0000  5.G.:.0.........
-00004a90: 0745 782d 4461 7465 0700 0000 0e44 6976  .Ex-Date.....Div
-00004aa0: 6964 656e 6457 6964 6765 7401 0300 0000  idendWidget.....
-00004ab0: 0600 4e00 2f00 4108 0000 0000 0600 0000  ..N./.A.........
-00004ac0: 034e 2f41 0700 0000 0e44 6976 6964 656e  .N/A.....Dividen
-00004ad0: 6457 6964 6765 7401 0300 0000 1a04 1d04  dWidget.........
-00004ae0: 3504 4200 2004 3a04 3e04 4204 3804 4004  5.B. .:.>.B.8.@.
-00004af0: 3e04 3204 3a04 3808 0000 0000 0600 0000  >.2.:.8.........
-00004b00: 084e 6f20 7175 6f74 6507 0000 000e 4469  .No quote.....Di
-00004b10: 7669 6465 6e64 5769 6467 6574 0103 0000  videndWidget....
-00004b20: 0010 041e 043f 0438 0441 0430 043d 0438  .....?.8.A.0.=.8
-00004b30: 0435 0800 0000 0006 0000 0004 4e6f 7465  .5..........Note
-00004b40: 0700 0000 0e44 6976 6964 656e 6457 6964  .....DividendWid
-00004b50: 6765 7401 0300 0000 0804 2604 3504 3d04  get.......&.5.=.
-00004b60: 3008 0000 0000 0600 0000 0550 7269 6365  0..........Price
-00004b70: 0700 0000 0e44 6976 6964 656e 6457 6964  .....DividendWid
-00004b80: 6765 7401 0300 0000 2004 1404 3804 3204  get..... ...8.2.
-00004b90: 3804 3404 3504 3d04 3400 2004 3004 3a04  8.4.5.=.4. .0.:.
-00004ba0: 4604 3804 4f04 3c04 3808 0000 0000 0600  F.8.O.<.8.......
-00004bb0: 0000 0e53 746f 636b 2044 6976 6964 656e  ...Stock Dividen
-00004bc0: 6407 0000 000e 4469 7669 6465 6e64 5769  d.....DividendWi
-00004bd0: 6467 6574 0103 0000 001c 041f 0435 0440  dget.........5.@
-00004be0: 0435 0434 0430 0447 0430 0020 0430 043a  .5.4.0.G.0. .0.:
-00004bf0: 0446 0438 0439 0800 0000 0006 0000 000d  .F.8.9..........
-00004c00: 5374 6f63 6b20 5665 7374 696e 6707 0000  Stock Vesting...
-00004c10: 000e 4469 7669 6465 6e64 5769 6467 6574  ..DividendWidget
-00004c20: 0103 0000 000a 041d 0430 043b 043e 0433  .........0.;.>.3
-00004c30: 0800 0000 0006 0000 0003 5461 7807 0000  ..........Tax...
-00004c40: 000e 4469 7669 6465 6e64 5769 6467 6574  ..DividendWidget
-00004c50: 0103 0000 0006 0422 0438 043f 0800 0000  .......".8.?....
-00004c60: 0006 0000 0004 5479 7065 0700 0000 0e44  ......Type.....D
-00004c70: 6976 6964 656e 6457 6964 6765 7401 0300  ividendWidget...
-00004c80: 0000 b204 1d04 4304 3604 3d04 3e00 2004  ......C.6.=.>. .
-00004c90: 4304 4104 4204 3004 3d04 3e04 3204 3804  C.A.B.0.=.>.2.8.
-00004ca0: 4204 4c00 2004 3a04 3e04 4204 3804 4004  B.L. .:.>.B.8.@.
-00004cb0: 3e04 3204 3a04 4300 2004 3104 4304 3c04  >.2.:.C. .1.C.<.
-00004cc0: 3004 3304 3800 2004 3404 3b04 4f00 2004  0.3.8. .4.;.O. .
-00004cd0: 1404 3004 4204 4b00 2f04 1204 4004 3504  ..0.B.K./...@.5.
-00004ce0: 3c04 3504 3d04 3800 2004 3404 3804 3204  <.5.=.8. .4.8.2.
-00004cf0: 3804 3404 3504 3d04 3404 3000 2004 4704  8.4.5.=.4.0. .G.
-00004d00: 3504 4004 3504 3700 2004 3c04 3504 3d04  5.@.5.7. .<.5.=.
-00004d10: 4e00 2004 1404 3004 3d04 3d04 4b04 3500  N. ...0.=.=.K.5.
-00004d20: 2d00 3e04 1a04 3e04 4204 3804 4004 3e04  -.>...>.B.8.@.>.
-00004d30: 3204 3a04 3808 0000 0000 0600 0000 4859  2.:.8.........HY
-00004d40: 6f75 2073 686f 756c 6420 7365 7420 7175  ou should set qu
-00004d50: 6f74 6520 7669 6120 4461 7461 2d3e 5175  ote via Data->Qu
-00004d60: 6f74 6573 206d 656e 7520 666f 7220 4461  otes menu for Da
-00004d70: 7465 2f54 696d 6520 6f66 2074 6865 2064  te/Time of the d
-00004d80: 6976 6964 656e 6407 0000 000e 4469 7669  ividend.....Divi
-00004d90: 6465 6e64 5769 6467 6574 0103 0000 0014  dendWidget......
-00004da0: 043d 0435 0438 0437 0432 0435 0441 0442  .=.5.8.7.2.5.A.B
-00004db0: 043d 043e 0800 0000 0006 0000 0007 756e  .=.>..........un
-00004dc0: 6b6e 6f77 6e07 0000 000e 4469 7669 6465  known.....Divide
-00004dd0: 6e64 5769 6467 6574 0103 0000 0010 0421  ndWidget.......!
-00004de0: 0432 043e 0439 0441 0442 0432 043e 0800  .2.>.9.A.B.2.>..
-00004df0: 0000 0006 0000 0008 5072 6f70 6572 7479  ........Property
-00004e00: 0700 0000 0e45 7874 7261 4461 7461 4d6f  .....ExtraDataMo
-00004e10: 6465 6c01 0300 0000 1004 1704 3d04 3004  del.........=.0.
-00004e20: 4704 3504 3d04 3804 3508 0000 0000 0600  G.5.=.8.5.......
-00004e30: 0000 0556 616c 7565 0700 0000 0e45 7874  ...Value.....Ext
-00004e40: 7261 4461 7461 4d6f 6465 6c01 0300 0000  raDataModel.....
-00004e50: 1a04 2604 3504 3d04 3d04 3004 4f00 2004  ..&.5.=.=.0.O. .
-00004e60: 3104 4304 3c04 3004 3304 3008 0000 0000  1.C.<.0.3.0.....
-00004e70: 0600 0000 0a41 7373 6574 204e 616d 6507  .....Asset Name.
-00004e80: 0000 000d 486f 6c64 696e 6773 4d6f 6465  ....HoldingsMode
-00004e90: 6c01 0300 0000 1c04 1204 3004 3b04 4e04  l.........0.;.N.
-00004ea0: 4204 3000 2f04 2104 4704 5104 4200 2f04  B.0./.!.G.Q.B./.
-00004eb0: 2604 1108 0000 0000 0600 0000 1643 7572  &............Cur
-00004ec0: 7265 6e63 792f 4163 636f 756e 742f 4173  rency/Account/As
-00004ed0: 7365 7407 0000 000d 486f 6c64 696e 6773  set.....Holdings
-00004ee0: 4d6f 6465 6c01 0300 0000 0a04 2d04 3a04  Model.......-.:.
-00004ef0: 4104 3f00 3a08 0000 0000 0600 0000 0445  A.?.:..........E
-00004f00: 7870 3a07 0000 000d 486f 6c64 696e 6773  xp:.....Holdings
-00004f10: 4d6f 6465 6c01 0300 0000 1404 2604 3504  Model.......&.5.
-00004f20: 3d04 3000 2004 3704 3004 3a04 4000 2e08  =.0. .7.0.:.@...
-00004f30: 0000 0000 0600 0000 044c 6173 7407 0000  .........Last...
-00004f40: 000d 486f 6c64 696e 6773 4d6f 6465 6c01  ..HoldingsModel.
-00004f50: 0300 0000 3404 1404 3004 4204 3000 2004  ....4...0.B.0. .
-00004f60: 3f04 3e04 4104 3b04 3504 3404 3d04 3504  ?.>.A.;.5.4.=.5.
-00004f70: 3900 2004 3a04 3e04 4204 3804 4004 3e04  9. .:.>.B.8.@.>.
-00004f80: 3204 3a04 3800 3a00 2008 0000 0000 0600  2.:.8.:. .......
-00004f90: 0000 114c 6173 7420 7175 6f74 6520 6461  ...Last quote da
-00004fa0: 7465 3a20 0700 0000 0d48 6f6c 6469 6e67  te: .....Holding
-00004fb0: 734d 6f64 656c 0103 0000 0014 0426 0435  sModel.......&.5
-00004fc0: 043d 0430 0020 043e 0442 043a 0440 002e  .=.0. .>.B.:.@..
-00004fd0: 0800 0000 0006 0000 0004 4f70 656e 0700  ..........Open..
-00004fe0: 0000 0d48 6f6c 6469 6e67 734d 6f64 656c  ...HoldingsModel
-00004ff0: 0103 0000 0006 041f 0438 0423 0800 0000  .........8.#....
-00005000: 0006 0000 0003 502f 4c07 0000 000d 486f  ......P/L.....Ho
-00005010: 6c64 696e 6773 4d6f 6465 6c01 0300 0000  ldingsModel.....
-00005020: 0c04 1f04 3804 2300 2c00 2000 2508 0000  ....8.#.,. .%...
-00005030: 0000 0600 0000 0650 2f4c 2c20 2507 0000  .......P/L, %...
-00005040: 000d 486f 6c64 696e 6773 4d6f 6465 6c01  ..HoldingsModel.
-00005050: 0300 0000 0c04 1a04 3e04 3b00 2d04 3204  ........>.;.-.2.
-00005060: 3e08 0000 0000 0600 0000 0351 7479 0700  >..........Qty..
-00005070: 0000 0d48 6f6c 6469 6e67 734d 6f64 656c  ...HoldingsModel
-00005080: 0103 0000 000e 0414 043e 043b 044f 002c  .........>.;.O.,
-00005090: 0020 0025 0800 0000 0006 0000 0008 5368  . .%..........Sh
-000050a0: 6172 652c 2025 0700 0000 0d48 6f6c 6469  are, %.....Holdi
-000050b0: 6e67 734d 6f64 656c 0103 0000 000c 041e  ngsModel........
-000050c0: 0446 0435 043d 043a 0430 0800 0000 0006  .F.5.=.:.0......
-000050d0: 0000 0005 5661 6c75 6507 0000 000d 486f  ....Value.....Ho
-000050e0: 6c64 696e 6773 4d6f 6465 6c01 0300 0000  ldingsModel.....
-000050f0: 1004 1e04 4604 3504 3d04 3a04 3000 2c00  ....F.5.=.:.0.,.
-00005100: 2008 0000 0000 0600 0000 0756 616c 7565   ..........Value
-00005110: 2c20 0700 0000 0d48 6f6c 6469 6e67 734d  , .....HoldingsM
-00005120: 6f64 656c 0103 0000 0016 041f 043e 0440  odel.........>.@
-00005130: 0442 0444 0435 043b 044c 0020 0426 0411  .B.D.5.;.L. .&..
-00005140: 0800 0000 0006 0000 0008 486f 6c64 696e  ..........Holdin
-00005150: 6773 0700 0000 0e48 6f6c 6469 6e67 7352  gs.....HoldingsR
-00005160: 6570 6f72 7401 0300 0000 1a04 1e04 4604  eport.........F.
-00005170: 3504 3d04 3804 4204 4c00 2004 3d04 3004  5.=.8.B.L. .=.0.
-00005180: 3b04 3e04 3308 0000 0000 0600 0000 0c45  ;.>.3..........E
-00005190: 7374 696d 6174 6520 7461 7807 0000 0014  stimate tax.....
-000051a0: 486f 6c64 696e 6773 5265 706f 7274 5769  HoldingsReportWi
-000051b0: 6e64 6f77 0103 0000 0016 041f 043e 0440  ndow.........>.@
-000051c0: 0442 0444 0435 043b 044c 0020 0426 0411  .B.D.5.;.L. .&..
-000051d0: 0800 0000 0006 0000 0008 486f 6c64 696e  ..........Holdin
-000051e0: 6773 0700 0000 1448 6f6c 6469 6e67 7352  gs.....HoldingsR
-000051f0: 6570 6f72 7457 696e 646f 7701 0300 0000  eportWindow.....
-00005200: 1404 1f04 3e04 4004 4204 4304 3304 3004  ....>.@.B.C.3.0.
-00005210: 3b04 3804 4f08 0000 0000 0600 0000 0850  ;.8.O..........P
-00005220: 6f72 7475 6761 6c07 0000 0014 486f 6c64  ortugal.....Hold
-00005230: 696e 6773 5265 706f 7274 5769 6e64 6f77  ingsReportWindow
-00005240: 0103 0000 000c 0420 043e 0441 0441 0438  ....... .>.A.A.8
-00005250: 044f 0800 0000 0006 0000 0006 5275 7373  .O..........Russ
-00005260: 6961 0700 0000 1448 6f6c 6469 6e67 7352  ia.....HoldingsR
-00005270: 6570 6f72 7457 696e 646f 7701 0300 0000  eportWindow.....
-00005280: 2804 1f04 3e04 3a04 3004 3704 3004 4204  (...>.:.0.7.0.B.
-00005290: 4c00 2004 3304 4004 3004 4404 3804 3a00  L. .3.@.0.D.8.:.
-000052a0: 2004 4604 3504 3d04 4b08 0000 0000 0600   .F.5.=.K.......
-000052b0: 0000 1053 686f 7720 5072 6963 6520 4368  ...Show Price Ch
-000052c0: 6172 7407 0000 0014 486f 6c64 696e 6773  art.....Holdings
-000052d0: 5265 706f 7274 5769 6e64 6f77 0103 0000  ReportWindow....
-000052e0: 0022 0412 0430 043b 044e 0442 0430 0020  ."...0.;.N.B.0. 
-000052f0: 043f 0435 0440 0435 0441 0447 0451 0442  .?.5.@.5.A.G.Q.B
-00005300: 0430 003a 0800 0000 0006 0000 0010 436f  .0.:..........Co
-00005310: 6d6d 6f6e 2063 7572 7265 6e63 793a 0700  mmon currency:..
-00005320: 0000 0e48 6f6c 6469 6e67 7357 6964 6765  ...HoldingsWidge
-00005330: 7401 0300 0000 1604 1f04 3e04 4004 4204  t.........>.@.B.
-00005340: 4404 3504 3b04 4c00 2004 2604 1108 0000  D.5.;.L. .&.....
-00005350: 0000 0600 0000 0848 6f6c 6469 6e67 7307  .......Holdings.
-00005360: 0000 000e 486f 6c64 696e 6773 5769 6467  ....HoldingsWidg
-00005370: 6574 0103 0000 0018 0421 043e 0445 0440  et.......!.>.E.@
-00005380: 0430 043d 0438 0442 044c 002e 002e 002e  .0.=.8.B.L......
-00005390: 0800 0000 0006 0000 0007 5361 7665 2e2e  ..........Save..
-000053a0: 2e07 0000 000e 486f 6c64 696e 6773 5769  ......HoldingsWi
-000053b0: 6467 6574 0103 0000 0014 0064 0064 002f  dget.......d.d./
-000053c0: 004d 004d 002f 0079 0079 0079 0079 0800  .M.M./.y.y.y.y..
-000053d0: 0000 0006 0000 000a 6464 2f4d 4d2f 7979  ........dd/MM/yy
-000053e0: 7979 0700 0000 0e48 6f6c 6469 6e67 7357  yy.....HoldingsW
-000053f0: 6964 6765 7401 0300 0000 3404 2204 3804  idget.....4.".8.
-00005400: 3f00 2004 2604 1100 2004 3d04 3500 2004  ?. .&... .=.5. .
-00005410: 3f04 3e04 3404 3404 3504 4004 3604 3804  ?.>.4.4.5.@.6.8.
-00005420: 3204 3004 3504 4204 4104 4f00 3a00 2008  2.0.5.B.A.O.:. .
-00005430: 0000 0000 0600 0000 1c41 7373 6574 2074  .........Asset t
-00005440: 7970 6520 6973 6e27 7420 7375 7070 6f72  ype isn't suppor
-00005450: 7465 643a 2007 0000 0004 4942 4b52 0103  ted: .....IBKR..
-00005460: 0000 0054 041a 043e 0440 043f 043e 0440  ...T...>.@.?.>.@
-00005470: 0430 0442 0438 0432 043d 043e 0435 0020  .0.B.8.2.=.>.5. 
-00005480: 0434 0435 0439 0441 0442 0432 0438 0435  .4.5.9.A.B.2.8.5
-00005490: 0020 043d 0435 0020 043f 043e 0434 0434  . .=.5. .?.>.4.4
-000054a0: 0435 0440 0436 0438 0432 0430 0435 0442  .5.@.6.8.2.0.5.B
-000054b0: 0441 044f 003a 0020 0800 0000 0006 0000  .A.O.:. ........
-000054c0: 0022 436f 7270 6f72 6174 6520 6163 7469  ."Corporate acti
-000054d0: 6f6e 2069 736e 2774 2073 7570 706f 7274  on isn't support
-000054e0: 6564 3a20 0700 0000 0449 424b 5201 0300  ed: .....IBKR...
-000054f0: 0000 4604 1d04 3504 3e04 3404 3d04 3e04  ..F...5.>.4.=.>.
-00005500: 3704 3d04 3004 4704 3d04 3e04 3500 2004  7.=.0.G.=.>.5. .
-00005510: 4104 3e04 3204 3f04 3004 3404 3504 3d04  A.>.2.?.0.4.5.=.
-00005520: 3804 3500 2004 4104 4704 5104 4204 3000  8.5. .A.G.Q.B.0.
-00005530: 2004 3404 3b04 4f00 2008 0000 0000 0600   .4.;.O. .......
-00005540: 0000 1b4d 756c 7469 706c 6520 6163 636f  ...Multiple acco
-00005550: 756e 7420 6d61 7463 6820 666f 7220 0700  unt match for ..
-00005560: 0000 0449 424b 5201 0300 0000 6800 4a00  ...IBKR.....h.J.
-00005570: 5300 4f00 4e00 2004 4204 4d04 3300 2000  S.O.N. .B.M.3. .
-00005580: 2700 6400 6f00 6300 7500 6d00 6500 6e00  '.d.o.c.u.m.e.n.
-00005590: 7400 2700 2004 3e04 4204 4104 4304 4204  t.'. .>.B.A.C.B.
-000055a0: 4104 4204 3204 4304 3504 4200 2004 3204  A.B.2.C.5.B. .2.
-000055b0: 3d04 4304 4204 4004 3800 2004 4204 4d04  =.C.B.@.8. .B.M.
-000055c0: 3304 3000 2000 2700 7400 6900 6300 6b00  3.0. .'.t.i.c.k.
-000055d0: 6500 7400 2708 0000 0000 0600 0000 2a43  e.t.'.........*C
-000055e0: 616e 2774 2066 696e 6420 2764 6f63 756d  an't find 'docum
-000055f0: 656e 7427 2074 6167 2069 6e20 6a73 6f6e  ent' tag in json
-00005600: 2027 7469 636b 6574 2707 0000 0010 496d   'ticket'.....Im
-00005610: 706f 7274 536c 6970 4469 616c 6f67 0103  portSlipDialog..
-00005620: 0000 0072 004a 0053 004f 004e 0020 0442  ...r.J.S.O.N. .B
-00005630: 044d 0433 0020 0027 006f 0070 0065 0072  .M.3. .'.o.p.e.r
-00005640: 0061 0074 0069 006f 006e 0054 0079 0070  .a.t.i.o.n.T.y.p
-00005650: 0065 0027 0020 043e 0442 0441 0443 0442  .e.'. .>.B.A.C.B
-00005660: 0441 0442 0432 0443 0435 0442 0020 0432  .A.B.2.C.5.B. .2
-00005670: 043d 0443 0442 0440 0438 0020 0442 044d  .=.C.B.@.8. .B.M
-00005680: 0433 0430 0020 0027 0074 0069 0063 006b  .3.0. .'.t.i.c.k
-00005690: 0065 0074 0027 0800 0000 0006 0000 002f  .e.t.'........./
-000056a0: 4361 6e27 7420 6669 6e64 2027 6f70 6572  Can't find 'oper
-000056b0: 6174 696f 6e54 7970 6527 2074 6167 2069  ationType' tag i
-000056c0: 6e20 6a73 6f6e 2027 7469 636b 6574 2707  n json 'ticket'.
-000056d0: 0000 0010 496d 706f 7274 536c 6970 4469  ....ImportSlipDi
-000056e0: 616c 6f67 0103 0000 006a 004a 0053 004f  alog.....j.J.S.O
-000056f0: 004e 0020 0442 044d 0433 0020 0027 0072  .N. .B.M.3. .'.r
-00005700: 0065 0063 0065 0069 0070 0074 0027 0020  .e.c.e.i.p.t.'. 
-00005710: 043e 0442 0441 0443 0442 0441 0442 0432  .>.B.A.C.B.A.B.2
-00005720: 0443 0435 0442 0020 0432 043d 0443 0442  .C.5.B. .2.=.C.B
-00005730: 0440 0438 0020 0442 044d 0433 0430 0020  .@.8. .B.M.3.0. 
-00005740: 0027 0064 006f 0063 0075 006d 0065 006e  .'.d.o.c.u.m.e.n
-00005750: 0074 0027 0800 0000 0006 0000 002b 4361  .t.'.........+Ca
-00005760: 6e27 7420 6669 6e64 2027 7265 6365 6970  n't find 'receip
-00005770: 7427 2074 6167 2069 6e20 6a73 6f6e 2027  t' tag in json '
-00005780: 646f 6375 6d65 6e74 2707 0000 0010 496d  document'.....Im
-00005790: 706f 7274 536c 6970 4469 616c 6f67 0103  portSlipDialog..
-000057a0: 0000 005e 041a 0430 0442 0435 0433 043e  ...^...0.B.5.3.>
-000057b0: 0440 0438 0438 0020 043d 0435 0020 0440  .@.8.8. .=.5. .@
-000057c0: 0430 0441 043f 043e 0437 043d 0430 043d  .0.A.?.>.7.=.0.=
-000057d0: 044b 003a 0020 0054 0065 006e 0073 006f  .K.:. .T.e.n.s.o
-000057e0: 0072 006c 006f 0077 0020 043d 0435 0020  .r.l.o.w. .=.5. 
-000057f0: 043e 0431 043d 0430 0440 0443 0436 0435  .>.1.=.0.@.C.6.5
-00005800: 043d 0800 0000 0006 0000 0036 4361 7465  .=.........6Cate
-00005810: 676f 7269 6573 2061 7265 206e 6f74 2072  gories are not r
-00005820: 6563 6f67 6e69 7a65 643a 2054 656e 736f  ecognized: Tenso
-00005830: 7266 6c6f 7720 6973 206e 6f74 2066 6f75  rflow is not fou
-00005840: 6e64 0700 0000 1049 6d70 6f72 7453 6c69  nd.....ImportSli
-00005850: 7044 6961 6c6f 6701 0300 0000 4a04 1f04  pDialog.....J...
-00005860: 4004 3504 3204 4b04 4804 3504 3d04 3e00  @.5.2.K.H.5.=.>.
-00005870: 2004 3c04 3004 3a04 4104 3804 3c04 3004   .<.0.:.A.8.<.0.
-00005880: 3b04 4c04 3d04 3e04 3500 2004 4704 3804  ;.L.=.>.5. .G.8.
-00005890: 4104 3b04 3e00 2004 3f04 3e04 3f04 4b04  A.;.>. .?.>.?.K.
-000058a0: 4204 3e04 3a00 2e08 0000 0000 0600 0000  B.>.:...........
-000058b0: 194d 6178 2072 6574 7279 2063 6f75 6e74  .Max retry count
-000058c0: 2065 7863 6565 6465 642e 0700 0000 1049   exceeded......I
-000058d0: 6d70 6f72 7453 6c69 7044 6961 6c6f 6701  mportSlipDialog.
-000058e0: 0300 0000 4600 5100 5200 2004 3a04 3e04  ....F.Q.R. .:.>.
-000058f0: 3400 2004 3d04 3500 2004 3e04 3104 3d04  4. .=.5. .>.1.=.
-00005900: 3004 4004 4304 3604 3504 3d00 2004 3200  0.@.C.6.5.=. .2.
-00005910: 2004 3104 4304 4404 3504 4004 3500 2004   .1.C.D.5.@.5. .
-00005920: 3e04 3104 3c04 3504 3d04 3008 0000 0000  >.1.<.5.=.0.....
-00005930: 0600 0000 1e4e 6f20 5152 2063 6f64 6573  .....No QR codes
-00005940: 2066 6f75 6e64 2069 6e20 636c 6970 626f   found in clipbo
-00005950: 6172 6407 0000 0010 496d 706f 7274 536c  ard.....ImportSl
-00005960: 6970 4469 616c 6f67 0103 0000 0036 0051  ipDialog.....6.Q
-00005970: 0052 002d 043a 043e 0434 0020 0432 0020  .R.-.:.>.4. .2. 
-00005980: 0444 0430 0439 043b 0435 0020 043d 0435  .D.0.9.;.5. .=.5
-00005990: 0020 043e 0431 043d 0430 0440 0443 0436  . .>.1.=.0.@.C.6
-000059a0: 0435 043d 0800 0000 0006 0000 001e 4e6f  .5.=..........No
-000059b0: 2051 5220 636f 6465 7320 7765 7265 2066   QR codes were f
-000059c0: 6f75 6e64 2069 6e20 6669 6c65 0700 0000  ound in file....
-000059d0: 1049 6d70 6f72 7453 6c69 7044 6961 6c6f  .ImportSlipDialo
-000059e0: 6701 0300 0000 7204 1d04 3504 3204 3e04  g.....r...5.2.>.
-000059f0: 3704 3c04 3e04 3604 3d04 3e00 2004 3404  7.<.>.6.=.>. .4.
-00005a00: 3e04 3104 3004 3204 3804 4204 4c00 2004  >.1.0.2.8.B.L. .
-00005a10: 4704 3504 3a00 3a00 2004 3d04 3500 2004  G.5.:.:. .=.5. .
-00005a20: 4304 3a04 3004 3704 3004 3d00 2004 3a04  C.:.0.7.0.=. .:.
-00005a30: 3e04 3d04 4204 4004 3004 3304 3504 3d04  >.=.B.@.0.3.5.=.
-00005a40: 4200 2004 3404 3b04 4f00 2004 3804 3c04  B. .4.;.O. .8.<.
-00005a50: 3f04 3e04 4004 4204 3008 0000 0000 0600  ?.>.@.B.0.......
-00005a60: 0000 414e 6f74 2070 6f73 7369 626c 6520  ..ANot possible 
-00005a70: 746f 2069 6d70 6f72 7420 736c 6970 3a20  to import slip: 
-00005a80: 6361 6e27 7420 696d 706f 7274 3a20 6e6f  can't import: no
-00005a90: 2070 6565 7220 7365 7420 666f 7220 696d   peer set for im
-00005aa0: 706f 7274 0700 0000 1049 6d70 6f72 7453  port.....ImportS
-00005ab0: 6c69 7044 6961 6c6f 6701 0300 0000 6604  lipDialog.....f.
-00005ac0: 1d04 3504 3204 3e04 3704 3c04 3e04 3604  ..5.2.>.7.<.>.6.
-00005ad0: 3d04 3e00 2004 3404 3e04 3104 3004 3204  =.>. .4.>.1.0.2.
-00005ae0: 3804 4204 4c00 2004 4704 3504 3a00 3a00  8.B.L. .G.5.:.:.
-00005af0: 2004 3d04 3500 2004 4304 3a04 3004 3704   .=.5. .C.:.0.7.
-00005b00: 3004 3d00 2004 4104 4704 3504 4200 2004  0.=. .A.G.5.B. .
-00005b10: 3404 3b04 4f00 2004 3804 3c04 3f04 3e04  4.;.O. .8.<.?.>.
-00005b20: 4004 4204 3008 0000 0000 0600 0000 364e  @.B.0.........6N
-00005b30: 6f74 2070 6f73 7369 626c 6520 746f 2069  ot possible to i
-00005b40: 6d70 6f72 7420 736c 6970 3a20 6e6f 2061  mport slip: no a
-00005b50: 6363 6f75 6e74 2073 6574 2066 6f72 2069  ccount set for i
-00005b60: 6d70 6f72 7407 0000 0010 496d 706f 7274  mport.....Import
-00005b70: 536c 6970 4469 616c 6f67 0103 0000 0078  SlipDialog.....x
-00005b80: 041d 0435 0432 043e 0437 043c 043e 0436  ...5.2.>.7.<.>.6
-00005b90: 043d 043e 0020 0434 043e 0431 0430 0432  .=.>. .4.>.1.0.2
-00005ba0: 0438 0442 044c 0020 0447 0435 043a 003a  .8.B.L. .G.5.:.:
-00005bb0: 0020 043a 0430 0442 0435 0433 043e 0440  . .:.0.B.5.3.>.@
-00005bc0: 0438 0438 0020 0443 043a 0430 0437 0430  .8.8. .C.:.0.7.0
-00005bd0: 043d 044b 0020 043d 0435 0020 0434 043b  .=.K. .=.5. .4.;
-00005be0: 044f 0020 0432 0441 0435 0445 0020 0441  .O. .2.A.5.E. .A
-00005bf0: 0442 0440 043e 043a 0800 0000 0006 0000  .B.@.>.:........
-00005c00: 0038 4e6f 7420 706f 7373 6962 6c65 2074  .8Not possible t
-00005c10: 6f20 696d 706f 7274 2073 6c69 703a 2073  o import slip: s
-00005c20: 6f6d 6520 6361 7465 676f 7269 6573 2061  ome categories a
-00005c30: 7265 206e 6f74 2073 6574 0700 0000 1049  re not set.....I
-00005c40: 6d70 6f72 7453 6c69 7044 6961 6c6f 6701  mportSlipDialog.
-00005c50: 0300 0000 5404 1d04 3504 3204 3e04 3704  ....T...5.2.>.7.
-00005c60: 3c04 3e04 3604 3d04 3e00 2004 4004 3004  <.>.6.=.>. .@.0.
-00005c70: 4104 3f04 3e04 3704 3d04 3004 4204 4c00  A.?.>.7.=.0.B.L.
-00005c80: 2004 3f04 4004 3e04 4704 3804 4204 3004   .?.@.>.G.8.B.0.
-00005c90: 3d04 3d04 4b04 3900 2000 5100 5200 2d04  =.=.K.9. .Q.R.-.
-00005ca0: 3a04 3e04 3400 3a00 2008 0000 0000 0600  :.>.4.:. .......
-00005cb0: 0000 2b51 5220 6176 6169 6c61 626c 6520  ..+QR available 
-00005cc0: 6275 7420 7061 7474 6572 6e20 6973 6e27  but pattern isn'
-00005cd0: 7420 7265 636f 676e 697a 6564 3a20 0700  t recognized: ..
-00005ce0: 0000 1049 6d70 6f72 7453 6c69 7044 6961  ...ImportSlipDia
-00005cf0: 6c6f 6701 0300 0000 0800 5100 5200 3a00  log.......Q.R.:.
-00005d00: 2008 0000 0000 0600 0000 0451 523a 2007   ..........QR: .
-00005d10: 0000 0010 496d 706f 7274 536c 6970 4469  ....ImportSlipDi
-00005d20: 616c 6f67 0103 0000 0030 0412 044b 0431  alog.....0...K.1
-00005d30: 0435 0440 0438 0442 0435 0020 0444 0430  .5.@.8.B.5. .D.0
-00005d40: 0439 043b 0020 0441 0020 0051 0052 002d  .9.;. .A. .Q.R.-
-00005d50: 043a 043e 0434 043e 043c 0800 0000 0006  .:.>.4.>.<......
-00005d60: 0000 0018 5365 6c65 6374 2066 696c 6520  ....Select file 
-00005d70: 7769 7468 2051 5220 636f 6465 0700 0000  with QR code....
-00005d80: 1049 6d70 6f72 7453 6c69 7044 6961 6c6f  .ImportSlipDialo
-00005d90: 6701 0300 0000 4204 1204 4b04 3104 3504  g.....B...K.1.5.
-00005da0: 4004 3804 4204 3500 2004 4404 3004 3904  @.8.B.5. .D.0.9.
-00005db0: 3b00 2004 4100 2000 4a00 5300 4f00 4e00  ;. .A. .J.S.O.N.
-00005dc0: 2d04 3404 3004 3d04 3d04 4b04 3c04 3800  -.4.0.=.=.K.<.8.
-00005dd0: 2004 4704 3504 3a04 3008 0000 0000 0600   .G.5.:.0.......
-00005de0: 0000 1f53 656c 6563 7420 6669 6c65 2077  ...Select file w
-00005df0: 6974 6820 736c 6970 204a 534f 4e20 6461  ith slip JSON da
-00005e00: 7461 0700 0000 1049 6d70 6f72 7453 6c69  ta.....ImportSli
-00005e10: 7044 6961 6c6f 6701 0300 0000 3204 1d04  pDialog.....2...
-00005e20: 3504 3804 3704 3204 3504 4104 4204 3d04  5.8.7.2.5.A.B.=.
-00005e30: 4b04 3900 2004 4204 3804 3f00 2004 3e04  K.9. .B.8.?. .>.
-00005e40: 3f04 3504 4004 3004 4604 3804 3800 2008  ?.5.@.0.F.8.8. .
-00005e50: 0000 0000 0600 0000 1755 6e6b 6e6f 776e  .........Unknown
-00005e60: 206f 7065 7261 7469 6f6e 2074 7970 6520   operation type 
-00005e70: 0700 0000 1049 6d70 6f72 7453 6c69 7044  .....ImportSlipD
-00005e80: 6961 6c6f 6701 0300 0000 0600 2027 9c00  ialog....... '..
-00005e90: 2008 0000 0000 0600 0000 0520 e29e 9c20   .......... ... 
-00005ea0: 0700 0000 0d49 6d70 6f72 7453 6c69 7044  .....ImportSlipD
-00005eb0: 6c67 0103 0000 000a 0421 0447 0435 0442  lg.......!.G.5.B
-00005ec0: 003a 0800 0000 0006 0000 0008 4163 636f  .:..........Acco
-00005ed0: 756e 743a 0700 0000 0d49 6d70 6f72 7453  unt:.....ImportS
-00005ee0: 6c69 7044 6c67 0103 0000 0010 0414 043e  lipDlg.........>
-00005ef0: 0431 0430 0432 0438 0442 044c 0800 0000  .1.0.2.8.B.L....
-00005f00: 0006 0000 0003 4164 6407 0000 000d 496d  ......Add.....Im
-00005f10: 706f 7274 536c 6970 446c 6701 0300 0000  portSlipDlg.....
-00005f20: 0c04 2104 4304 3c04 3c04 3000 3a08 0000  ..!.C.<.<.0.:...
-00005f30: 0000 0600 0000 0741 6d6f 756e 743a 0700  .......Amount:..
-00005f40: 0000 0d49 6d70 6f72 7453 6c69 7044 6c67  ...ImportSlipDlg
-00005f50: 0103 0000 0032 0410 0432 0442 043e 002d  .....2...2.B.>.-
-00005f60: 043d 0430 0437 043d 0430 0447 0435 043d  .=.0.7.=.0.G.5.=
-00005f70: 0438 0435 0020 043a 0430 0442 0435 0433  .8.5. .:.0.B.5.3
-00005f80: 043e 0440 0438 0439 0800 0000 0006 0000  .>.@.8.9........
-00005f90: 0016 4175 746f 2d61 7373 6967 6e20 6361  ..Auto-assign ca
-00005fa0: 7465 676f 7269 6573 0700 0000 0d49 6d70  tegories.....Imp
-00005fb0: 6f72 7453 6c69 7044 6c67 0103 0000 000c  ortSlipDlg......
-00005fc0: 041a 0430 043c 0435 0440 0430 0800 0000  ...0.<.5.@.0....
-00005fd0: 0006 0000 0006 4361 6d65 7261 0700 0000  ......Camera....
-00005fe0: 0d49 6d70 6f72 7453 6c69 7044 6c67 0103  .ImportSlipDlg..
-00005ff0: 0000 0010 041e 0447 0438 0441 0442 0438  .......G.8.A.B.8
-00006000: 0442 044c 0800 0000 0006 0000 0005 436c  .B.L..........Cl
-00006010: 6561 7207 0000 000d 496d 706f 7274 536c  ear.....ImportSl
-00006020: 6970 446c 6701 0300 0000 0e04 1704 3004  ipDlg.........0.
-00006030: 3a04 4004 4b04 4204 4c08 0000 0000 0600  :.@.K.B.L.......
-00006040: 0000 0543 6c6f 7365 0700 0000 0d49 6d70  ...Close.....Imp
-00006050: 6f72 7453 6c69 7044 6c67 0103 0000 001a  ortSlipDlg......
-00006060: 0414 0430 0442 0430 0020 002f 0020 0412  ...0.B.0. ./. ..
-00006070: 0440 0435 043c 044f 003a 0800 0000 0006  .@.5.<.O.:......
-00006080: 0000 000c 4461 7465 202f 2054 696d 653a  ....Date / Time:
-00006090: 0700 0000 0d49 6d70 6f72 7453 6c69 7044  .....ImportSlipD
-000060a0: 6c67 0103 0000 0016 0414 0430 0442 0430  lg.........0.B.0
-000060b0: 002f 0412 0440 0435 043c 044f 003a 0800  ./...@.5.<.O.:..
-000060c0: 0000 0006 0000 000a 4461 7465 2f54 696d  ........Date/Tim
-000060d0: 653a 0700 0000 0d49 6d70 6f72 7453 6c69  e:.....ImportSli
-000060e0: 7044 6c67 0103 0000 0006 0424 0414 003a  pDlg.......$...:
-000060f0: 0800 0000 0006 0000 0003 4644 3a07 0000  ..........FD:...
-00006100: 000d 496d 706f 7274 536c 6970 446c 6701  ..ImportSlipDlg.
-00006110: 0300 0000 0604 2404 1d00 3a08 0000 0000  ......$...:.....
-00006120: 0600 0000 0346 4e3a 0700 0000 0d49 6d70  .....FN:.....Imp
-00006130: 6f72 7453 6c69 7044 6c67 0103 0000 0006  ortSlipDlg......
-00006140: 0424 041f 003a 0800 0000 0006 0000 0003  .$...:..........
-00006150: 4650 3a07 0000 000d 496d 706f 7274 536c  FP:.....ImportSl
-00006160: 6970 446c 6701 0300 0000 2604 2104 3a04  ipDlg.....&.!.:.
-00006170: 3004 3d04 3804 4004 3e04 3204 3004 4204  0.=.8.@.>.2.0.B.
-00006180: 4c00 2004 3a04 3004 3c04 3504 4004 3e04  L. .:.0.<.5.@.>.
-00006190: 3908 0000 0000 0600 0000 0f47 6574 2066  9..........Get f
-000061a0: 726f 6d20 6361 6d65 7261 0700 0000 0d49  rom camera.....I
-000061b0: 6d70 6f72 7453 6c69 7044 6c67 0103 0000  mportSlipDlg....
-000061c0: 0024 041f 043e 043b 0443 0447 0438 0442  .$...>.;.C.G.8.B
-000061d0: 044c 0020 0438 0437 0020 0431 0443 0444  .L. .8.7. .1.C.D
-000061e0: 0435 0440 0430 0800 0000 0006 0000 0012  .5.@.0..........
-000061f0: 4765 7420 6672 6f6d 2063 6c69 7062 6f61  Get from clipboa
-00006200: 7264 0700 0000 0d49 6d70 6f72 7453 6c69  rd.....ImportSli
-00006210: 7044 6c67 0103 0000 0030 041f 043e 043b  pDlg.....0...>.;
-00006220: 0443 0447 0438 0442 044c 0020 0447 0435  .C.G.8.B.L. .G.5
-00006230: 043a 0020 0441 0020 0441 0430 0439 0442  .:. .A. .A.0.9.B
-00006240: 0430 0020 0424 041d 0421 0800 0000 0006  .0. .$...!......
-00006250: 0000 0016 4765 7420 736c 6970 2066 726f  ....Get slip fro
-00006260: 6d20 696e 7465 726e 6574 0700 0000 0d49  m internet.....I
-00006270: 6d70 6f72 7453 6c69 7044 6c67 0103 0000  mportSlipDlg....
-00006280: 0016 0418 043c 043f 043e 0440 0442 0020  .....<.?.>.@.B. 
-00006290: 0447 0435 043a 0430 0800 0000 0006 0000  .G.5.:.0........
-000062a0: 000b 496d 706f 7274 2053 6c69 7007 0000  ..Import Slip...
-000062b0: 000d 496d 706f 7274 536c 6970 446c 6701  ..ImportSlipDlg.
-000062c0: 0300 0000 0e04 2104 4204 4004 3e04 3a04  ......!.B.@.>.:.
-000062d0: 3800 3a08 0000 0000 0600 0000 064c 696e  8.:..........Lin
-000062e0: 6573 3a07 0000 000d 496d 706f 7274 536c  es:.....ImportSl
-000062f0: 6970 446c 6701 0300 0000 2404 1704 3004  ipDlg.....$...0.
-00006300: 3304 4004 4304 3704 3804 4204 4c00 2004  3.@.C.7.8.B.L. .
-00006310: 3804 3700 2004 4404 3004 3904 3b04 3008  8.7. .D.0.9.;.0.
-00006320: 0000 0000 0600 0000 0e4c 6f61 6420 6672  .........Load fr
-00006330: 6f6d 2066 696c 6507 0000 000d 496d 706f  om file.....Impo
-00006340: 7274 536c 6970 446c 6701 0300 0000 3604  rtSlipDlg.....6.
-00006350: 1704 3004 3304 4304 3704 3804 4204 4c00  ..0.3.C.7.8.B.L.
-00006360: 2004 4704 3504 3a04 3000 2004 3804 3700   .G.5.:.0. .8.7.
-00006370: 2000 4a00 5300 4f00 4e00 2d04 4404 3004   .J.S.O.N.-.D.0.
-00006380: 3904 3b04 3008 0000 0000 0600 0000 184c  9.;.0..........L
-00006390: 6f61 6420 736c 6970 2066 726f 6d20 4a53  oad slip from JS
-000063a0: 4f4e 2066 696c 6507 0000 000d 496d 706f  ON file.....Impo
-000063b0: 7274 536c 6970 446c 6701 0300 0000 1604  rtSlipDlg.......
-000063c0: 1a04 3e04 3d04 4204 4004 3004 3304 3504  ..>.=.B.@.0.3.5.
-000063d0: 3d04 4200 3a08 0000 0000 0600 0000 0550  =.B.:..........P
-000063e0: 6565 723a 0700 0000 0d49 6d70 6f72 7453  eer:.....ImportS
-000063f0: 6c69 7044 6c67 0103 0000 000e 041f 043e  lipDlg.........>
-00006400: 043a 0443 043f 043a 0430 0800 0000 0006  .:.C.?.:.0......
-00006410: 0000 0008 5075 7263 6861 7365 0700 0000  ....Purchase....
-00006420: 0d49 6d70 6f72 7453 6c69 7044 6c67 0103  .ImportSlipDlg..
-00006430: 0000 000c 0051 0052 002d 043a 043e 0434  .....Q.R.-.:.>.4
-00006440: 0800 0000 0006 0000 0007 5152 2d63 6f64  ..........QR-cod
-00006450: 6507 0000 000d 496d 706f 7274 536c 6970  e.....ImportSlip
-00006460: 446c 6701 0300 0000 0e04 1204 3e04 3704  Dlg.........>.7.
-00006470: 3204 4004 3004 4208 0000 0000 0600 0000  2.@.0.B.........
-00006480: 0652 6574 7572 6e07 0000 000d 496d 706f  .Return.....Impo
-00006490: 7274 536c 6970 446c 6701 0300 0000 2e04  rtSlipDlg.......
-000064a0: 2304 4104 4204 3004 3d04 3e04 3204 3804  #.A.B.0.=.>.2.8.
-000064b0: 4204 4c00 2004 4204 4d04 3300 2004 3404  B.L. .B.M.3. .4.
-000064c0: 3b04 4f00 2004 3204 4104 3504 4508 0000  ;.O. .2.A.5.E...
-000064d0: 0000 0600 0000 1553 6574 2054 6167 2066  .......Set Tag f
-000064e0: 6f72 2061 6c6c 206c 696e 6573 0700 0000  or all lines....
-000064f0: 0d49 6d70 6f72 7453 6c69 7044 6c67 0103  .ImportSlipDlg..
-00006500: 0000 0006 0427 0435 043a 0800 0000 0006  .....'.5.:......
-00006510: 0000 0004 536c 6970 0700 0000 0d49 6d70  ....Slip.....Imp
-00006520: 6f72 7453 6c69 7044 6c67 0103 0000 0016  ortSlipDlg......
-00006530: 0414 0430 043d 043d 044b 0435 0020 0447  ...0.=.=.K.5. .G
-00006540: 0435 043a 0430 0800 0000 0006 0000 0009  .5.:.0..........
-00006550: 536c 6970 2064 6174 6107 0000 000d 496d  Slip data.....Im
-00006560: 706f 7274 536c 6970 446c 6701 0300 0000  portSlipDlg.....
-00006570: 1c04 1704 3004 3a04 4004 4b04 4204 4c00  ....0.:.@.K.B.L.
-00006580: 2004 3a04 3004 3c04 3504 4004 4308 0000   .:.0.<.5.@.C...
-00006590: 0000 0600 0000 0b53 746f 7020 6361 6d65  .......Stop came
-000065a0: 7261 0700 0000 0d49 6d70 6f72 7453 6c69  ra.....ImportSli
-000065b0: 7044 6c67 0103 0000 0008 0422 0438 043f  pDlg.......".8.?
-000065c0: 003a 0800 0000 0006 0000 0005 5479 7065  .:..........Type
-000065d0: 3a07 0000 000d 496d 706f 7274 536c 6970  :.....ImportSlip
-000065e0: 446c 6701 0300 0000 2600 6400 6400 2f00  Dlg.....&.d.d./.
-000065f0: 4d00 4d00 2f00 7900 7900 7900 7900 2000  M.M./.y.y.y.y. .
-00006600: 6800 6800 3a00 6d00 6d00 3a00 7300 7308  h.h.:.m.m.:.s.s.
-00006610: 0000 0000 0600 0000 1364 642f 4d4d 2f79  .........dd/MM/y
-00006620: 7979 7920 6868 3a6d 6d3a 7373 0700 0000  yyy hh:mm:ss....
-00006630: 0d49 6d70 6f72 7453 6c69 7044 6c67 0103  .ImportSlipDlg..
-00006640: 0000 0066 041d 0435 0432 043e 0437 043c  ...f...5.2.>.7.<
-00006650: 043e 0436 043d 043e 0020 043e 0431 0440  .>.6.=.>. .>.1.@
-00006660: 0430 0431 043e 0442 0430 0442 044c 0020  .0.1.>.B.0.B.L. 
-00006670: 043e 043f 0435 0440 0430 0446 0438 044e  .>.?.5.@.0.F.8.N
-00006680: 0020 0431 0435 0437 0020 0434 0435 0442  . .1.5.7. .4.5.B
-00006690: 0430 043b 044c 043d 044b 0445 0020 0434  .0.;.L.=.K.E. .4
-000066a0: 0430 043d 043d 044b 0445 0800 0000 0006  .0.=.=.K.E......
-000066b0: 0000 0027 4361 6e27 7420 7072 6f63 6573  ...'Can't proces
-000066c0: 7320 6f70 6572 6174 696f 6e20 7769 7468  s operation with
-000066d0: 6f75 7420 6465 7461 696c 7307 0000 000e  out details.....
-000066e0: 496e 636f 6d65 5370 656e 6469 6e67 0103  IncomeSpending..
-000066f0: 0000 000c 041a 0443 0440 0441 003a 0020  .......C.@.A.:. 
-00006700: 0800 0000 0006 0000 0006 5261 7465 3a20  ..........Rate: 
-00006710: 0700 0000 0e49 6e63 6f6d 6553 7065 6e64  .....IncomeSpend
-00006720: 696e 6701 0300 0000 1c04 1404 3e04 4504  ing.........>.E.
-00006730: 3e04 3404 4b00 2004 3800 2004 2204 4004  >.4.K. .8. .".@.
-00006740: 3004 4204 4b08 0000 0000 0600 0000 1149  0.B.K..........I
-00006750: 6e63 6f6d 6520 2620 5370 656e 6469 6e67  ncome & Spending
-00006760: 0700 0000 1449 6e63 6f6d 6553 7065 6e64  .....IncomeSpend
-00006770: 696e 6752 6570 6f72 7401 0300 0000 0604  ingReport.......
-00006780: 1004 3f04 4008 0000 0000 0600 0000 0341  ..?.@..........A
-00006790: 7072 0700 0000 1949 6e63 6f6d 6553 7065  pr.....IncomeSpe
-000067a0: 6e64 696e 6752 6570 6f72 744d 6f64 656c  ndingReportModel
-000067b0: 0103 0000 0006 0410 0432 0433 0800 0000  .........2.3....
-000067c0: 0006 0000 0003 4175 6707 0000 0019 496e  ......Aug.....In
-000067d0: 636f 6d65 5370 656e 6469 6e67 5265 706f  comeSpendingRepo
-000067e0: 7274 4d6f 6465 6c01 0300 0000 0604 1404  rtModel.........
-000067f0: 3504 3a08 0000 0000 0600 0000 0344 6563  5.:..........Dec
-00006800: 0700 0000 1949 6e63 6f6d 6553 7065 6e64  .....IncomeSpend
-00006810: 696e 6752 6570 6f72 744d 6f64 656c 0103  ingReportModel..
-00006820: 0000 0006 0424 0435 0432 0800 0000 0006  .....$.5.2......
-00006830: 0000 0003 4665 6207 0000 0019 496e 636f  ....Feb.....Inco
-00006840: 6d65 5370 656e 6469 6e67 5265 706f 7274  meSpendingReport
-00006850: 4d6f 6465 6c01 0300 0000 0604 2f04 3d04  Model......./.=.
-00006860: 3208 0000 0000 0600 0000 034a 616e 0700  2..........Jan..
-00006870: 0000 1949 6e63 6f6d 6553 7065 6e64 696e  ...IncomeSpendin
-00006880: 6752 6570 6f72 744d 6f64 656c 0103 0000  gReportModel....
-00006890: 0006 0418 044e 043b 0800 0000 0006 0000  .....N.;........
-000068a0: 0003 4a75 6c07 0000 0019 496e 636f 6d65  ..Jul.....Income
-000068b0: 5370 656e 6469 6e67 5265 706f 7274 4d6f  SpendingReportMo
-000068c0: 6465 6c01 0300 0000 0604 1804 4e04 3d08  del.........N.=.
-000068d0: 0000 0000 0600 0000 034a 756e 0700 0000  .........Jun....
-000068e0: 1949 6e63 6f6d 6553 7065 6e64 696e 6752  .IncomeSpendingR
-000068f0: 6570 6f72 744d 6f64 656c 0103 0000 0006  eportModel......
-00006900: 041c 0430 0440 0800 0000 0006 0000 0003  ...0.@..........
-00006910: 4d61 7207 0000 0019 496e 636f 6d65 5370  Mar.....IncomeSp
-00006920: 656e 6469 6e67 5265 706f 7274 4d6f 6465  endingReportMode
-00006930: 6c01 0300 0000 0604 1c04 3004 3908 0000  l.........0.9...
-00006940: 0000 0600 0000 034d 6179 0700 0000 1949  .......May.....I
-00006950: 6e63 6f6d 6553 7065 6e64 696e 6752 6570  ncomeSpendingRep
-00006960: 6f72 744d 6f64 656c 0103 0000 0006 041d  ortModel........
-00006970: 043e 044f 0800 0000 0006 0000 0003 4e6f  .>.O..........No
-00006980: 7607 0000 0019 496e 636f 6d65 5370 656e  v.....IncomeSpen
-00006990: 6469 6e67 5265 706f 7274 4d6f 6465 6c01  dingReportModel.
-000069a0: 0300 0000 0604 1e04 3a04 4208 0000 0000  ........:.B.....
-000069b0: 0600 0000 034f 6374 0700 0000 1949 6e63  .....Oct.....Inc
-000069c0: 6f6d 6553 7065 6e64 696e 6752 6570 6f72  omeSpendingRepor
-000069d0: 744d 6f64 656c 0103 0000 0006 0421 0435  tModel.......!.5
-000069e0: 043d 0800 0000 0006 0000 0003 5365 7007  .=..........Sep.
-000069f0: 0000 0019 496e 636f 6d65 5370 656e 6469  ....IncomeSpendi
-00006a00: 6e67 5265 706f 7274 4d6f 6465 6c01 0300  ngReportModel...
-00006a10: 0000 0a04 1804 2204 1e04 1304 1e08 0000  ......".........
-00006a20: 0000 0600 0000 0554 4f54 414c 0700 0000  .......TOTAL....
-00006a30: 1949 6e63 6f6d 6553 7065 6e64 696e 6752  .IncomeSpendingR
-00006a40: 6570 6f72 744d 6f64 656c 0103 0000 000e  eportModel......
-00006a50: 0412 0430 043b 044e 0442 0430 003a 0800  ...0.;.N.B.0.:..
-00006a60: 0000 0006 0000 0009 4375 7272 656e 6379  ........Currency
-00006a70: 3a07 0000 001a 496e 636f 6d65 5370 656e  :.....IncomeSpen
-00006a80: 6469 6e67 5265 706f 7274 5769 6467 6574  dingReportWidget
-00006a90: 0103 0000 001c 0414 043e 0445 043e 0434  .........>.E.>.4
-00006aa0: 044b 0020 0438 0020 0422 0440 0430 0442  .K. .8. .".@.0.B
-00006ab0: 044b 0800 0000 0006 0000 0011 496e 636f  .K..........Inco
-00006ac0: 6d65 2026 2053 7065 6e64 696e 6707 0000  me & Spending...
-00006ad0: 001a 496e 636f 6d65 5370 656e 6469 6e67  ..IncomeSpending
-00006ae0: 5265 706f 7274 5769 6467 6574 0103 0000  ReportWidget....
-00006af0: 0018 0421 043e 0445 0440 0430 043d 0438  ...!.>.E.@.0.=.8
-00006b00: 0442 044c 002e 002e 002e 0800 0000 0006  .B.L............
-00006b10: 0000 0007 5361 7665 2e2e 2e07 0000 001a  ....Save........
-00006b20: 496e 636f 6d65 5370 656e 6469 6e67 5265  IncomeSpendingRe
-00006b30: 706f 7274 5769 6467 6574 0103 0000 001c  portWidget......
-00006b40: 0414 043e 0445 043e 0434 044b 0020 0438  ...>.E.>.4.K. .8
-00006b50: 0020 0422 0440 0430 0442 044b 0800 0000  . .".@.0.B.K....
-00006b60: 0006 0000 0011 496e 636f 6d65 2026 2053  ......Income & S
-00006b70: 7065 6e64 696e 6707 0000 001a 496e 636f  pending.....Inco
-00006b80: 6d65 5370 656e 6469 6e67 5265 706f 7274  meSpendingReport
-00006b90: 5769 6e64 6f77 0103 0000 0022 041f 043e  Window....."...>
-00006ba0: 043a 0430 0437 0430 0442 044c 0020 043e  .:.0.7.0.B.L. .>
-00006bb0: 043f 0435 0440 0430 0446 0438 0438 0800  .?.5.@.0.F.8.8..
-00006bc0: 0000 0006 0000 000f 5368 6f77 206f 7065  ........Show ope
-00006bd0: 7261 7469 6f6e 7307 0000 001a 496e 636f  rations.....Inco
-00006be0: 6d65 5370 656e 6469 6e67 5265 706f 7274  meSpendingReport
-00006bf0: 5769 6e64 6f77 0103 0000 0008 0421 0447  Window.......!.G
-00006c00: 0435 0442 0800 0000 0006 0000 0007 4163  .5.B..........Ac
-00006c10: 636f 756e 7407 0000 0014 496e 636f 6d65  count.....Income
-00006c20: 5370 656e 6469 6e67 5769 6467 6574 0103  SpendingWidget..
-00006c30: 0000 0032 0414 043e 0431 0430 0432 0438  ...2...>.1.0.2.8
-00006c40: 0442 044c 0020 0434 0435 0442 0430 043b  .B.L. .4.5.B.0.;
-00006c50: 044c 043d 0443 044e 0020 0437 0430 043f  .L.=.C.N. .7.0.?
-00006c60: 0438 0441 044c 0800 0000 0006 0000 000a  .8.A.L..........
-00006c70: 4164 6420 6465 7461 696c 0700 0000 1449  Add detail.....I
-00006c80: 6e63 6f6d 6553 7065 6e64 696e 6757 6964  ncomeSpendingWid
-00006c90: 6765 7401 0300 0000 3804 2104 3a04 3e04  get.....8.!.:.>.
-00006ca0: 3f04 3804 4004 3e04 3204 3004 4204 4c00  ?.8.@.>.2.0.B.L.
-00006cb0: 2004 3404 3504 4204 3004 3b04 4c04 3d04   .4.5.B.0.;.L.=.
-00006cc0: 4304 4e00 2004 3704 3004 3f04 3804 4104  C.N. .7.0.?.8.A.
-00006cd0: 4c08 0000 0000 0600 0000 0b43 6f70 7920  L..........Copy 
-00006ce0: 6465 7461 696c 0700 0000 1449 6e63 6f6d  detail.....Incom
-00006cf0: 6553 7065 6e64 696e 6757 6964 6765 7401  eSpendingWidget.
-00006d00: 0300 0000 1404 1404 3004 4204 3000 2f04  ........0.B.0./.
-00006d10: 1204 4004 3504 3c04 4f08 0000 0000 0600  ..@.5.<.O.......
-00006d20: 0000 0944 6174 652f 5469 6d65 0700 0000  ...Date/Time....
-00006d30: 1449 6e63 6f6d 6553 7065 6e64 696e 6757  .IncomeSpendingW
-00006d40: 6964 6765 7401 0300 0000 0c04 1404 3504  idget.........5.
-00006d50: 4204 3004 3b04 3808 0000 0000 0600 0000  B.0.;.8.........
-00006d60: 0744 6574 6169 6c73 0700 0000 1449 6e63  .Details.....Inc
-00006d70: 6f6d 6553 7065 6e64 696e 6757 6964 6765  omeSpendingWidge
-00006d80: 7401 0300 0000 4404 1d04 3504 3204 3e04  t.....D...5.2.>.
-00006d90: 3704 3c04 3e04 3604 3d04 3e00 2004 3404  7.<.>.6.=.>. .4.
-00006da0: 3e04 3104 3004 3204 3804 4204 4c00 2004  >.1.0.2.8.B.L. .
-00006db0: 3d04 3e04 3204 4304 4e00 2004 3704 3004  =.>.2.C.N. .7.0.
-00006dc0: 3f04 3804 4104 4c00 3a00 2008 0000 0000  ?.8.A.L.:. .....
-00006dd0: 0600 0000 1a46 6169 6c65 6420 746f 2061  .....Failed to a
-00006de0: 6464 206e 6577 2072 6563 6f72 643a 2007  dd new record: .
-00006df0: 0000 0014 496e 636f 6d65 5370 656e 6469  ....IncomeSpendi
-00006e00: 6e67 5769 6467 6574 0103 0000 001c 0414  ngWidget........
-00006e10: 043e 0445 043e 0434 0020 002f 0020 0420  .>.E.>.4. ./. . 
-00006e20: 0430 0441 0445 043e 0434 0800 0000 0006  .0.A.E.>.4......
-00006e30: 0000 0011 496e 636f 6d65 202f 2053 7065  ....Income / Spe
-00006e40: 6e64 696e 6707 0000 0014 496e 636f 6d65  nding.....Income
-00006e50: 5370 656e 6469 6e67 5769 6467 6574 0103  SpendingWidget..
-00006e60: 0000 0014 041f 0440 0438 043c 0435 0447  .......@.8.<.5.G
-00006e70: 0430 043d 0438 0435 0800 0000 0006 0000  .0.=.8.5........
-00006e80: 0004 4e6f 7465 0700 0000 1449 6e63 6f6d  ..Note.....Incom
-00006e90: 6553 7065 6e64 696e 6757 6964 6765 7401  eSpendingWidget.
-00006ea0: 0300 0000 4804 1e04 4804 3804 3104 3a04  ....H...H.8.1.:.
-00006eb0: 3000 2004 3f04 4004 3800 2004 3704 3004  0. .?.@.8. .7.0.
-00006ec0: 3f04 3804 4104 3800 2004 3404 3504 4204  ?.8.A.8. .4.5.B.
-00006ed0: 3004 3b04 3504 3900 2004 3e04 3f04 3504  0.;.5.9. .>.?.5.
-00006ee0: 4004 3004 4604 3804 3800 3a00 2008 0000  @.0.F.8.8.:. ...
-00006ef0: 0000 0600 0000 214f 7065 7261 7469 6f6e  ......!Operation
-00006f00: 2064 6574 6169 6c73 2073 7562 6d69 7420   details submit 
-00006f10: 6661 696c 6564 3a20 0700 0000 1449 6e63  failed: .....Inc
-00006f20: 6f6d 6553 7065 6e64 696e 6757 6964 6765  omeSpendingWidge
-00006f30: 7401 0300 0000 3804 1e04 4804 3804 3104  t.....8...H.8.1.
-00006f40: 3a04 3000 2004 3f04 4004 3800 2004 3704  :.0. .?.@.8. .7.
-00006f50: 3004 3f04 3804 4104 3800 2004 3e04 3f04  0.?.8.A.8. .>.?.
-00006f60: 3504 4004 3004 4604 3804 3800 3a00 2008  5.@.0.F.8.8.:. .
-00006f70: 0000 0000 0600 0000 194f 7065 7261 7469  .........Operati
-00006f80: 6f6e 2073 7562 6d69 7420 6661 696c 6564  on submit failed
-00006f90: 3a20 0700 0000 1449 6e63 6f6d 6553 7065  : .....IncomeSpe
-00006fa0: 6e64 696e 6757 6964 6765 7401 0300 0000  ndingWidget.....
-00006fb0: 2004 1e04 3f04 3b04 3004 4204 3000 2004   ...?.;.0.B.0. .
-00006fc0: 3200 2004 3204 3004 3b04 4e04 4204 3500  2. .2.0.;.N.B.5.
-00006fd0: 3a08 0000 0000 0600 0000 1950 6169 6420  :..........Paid 
-00006fe0: 696e 2066 6f72 6569 676e 2063 7572 7265  in foreign curre
-00006ff0: 6e63 793a 0700 0000 1449 6e63 6f6d 6553  ncy:.....IncomeS
-00007000: 7065 6e64 696e 6757 6964 6765 7401 0300  pendingWidget...
-00007010: 0000 1404 1a04 3e04 3d04 4204 4004 3004  ......>.=.B.@.0.
-00007020: 3304 3504 3d04 4208 0000 0000 0600 0000  3.5.=.B.........
-00007030: 0450 6565 7207 0000 0014 496e 636f 6d65  .Peer.....Income
-00007040: 5370 656e 6469 6e67 5769 6467 6574 0103  SpendingWidget..
-00007050: 0000 0030 0423 0434 0430 043b 0438 0442  ...0.#.4.0.;.8.B
-00007060: 044c 0020 0434 0435 0442 0430 043b 044c  .L. .4.5.B.0.;.L
-00007070: 043d 0443 044e 0020 0437 0430 043f 0438  .=.C.N. .7.0.?.8
-00007080: 0441 044c 0800 0000 0006 0000 000d 5265  .A.L..........Re
-00007090: 6d6f 7665 2064 6574 6169 6c07 0000 0014  move detail.....
-000070a0: 496e 636f 6d65 5370 656e 6469 6e67 5769  IncomeSpendingWi
-000070b0: 6467 6574 0103 0000 000c 0026 0421 0447  dget.......&.!.G
-000070c0: 0435 0442 0430 0800 0000 0006 0000 0009  .5.B.0..........
-000070d0: 2641 6363 6f75 6e74 7307 0000 000e 4a41  &Accounts.....JA
-000070e0: 4c5f 4d61 696e 5769 6e64 6f77 0103 0000  L_MainWindow....
-000070f0: 0012 0026 0411 044d 043a 0430 043f 002e  ...&...M.:.0.?..
-00007100: 002e 002e 0800 0000 0006 0000 000a 2642  ..............&B
-00007110: 6163 6b75 702e 2e2e 0700 0000 0e4a 414c  ackup........JAL
-00007120: 5f4d 6169 6e57 696e 646f 7701 0300 0000  _MainWindow.....
-00007130: 1e00 2604 1104 3004 3704 3e04 3204 3004  ..&...0.7.>.2.0.
-00007140: 4f00 2004 3204 3004 3b04 4e04 4204 3008  O. .2.0.;.N.B.0.
-00007150: 0000 0000 0600 0000 0e26 4261 7365 2043  .........&Base C
-00007160: 7572 7265 6e63 7907 0000 000e 4a41 4c5f  urrency.....JAL_
-00007170: 4d61 696e 5769 6e64 6f77 0103 0000 0014  MainWindow......
-00007180: 0026 041a 0430 0442 0435 0433 043e 0440  .&...0.B.5.3.>.@
-00007190: 0438 0438 0800 0000 0006 0000 000b 2643  .8.8..........&C
-000071a0: 6174 6567 6f72 6965 7307 0000 000e 4a41  ategories.....JA
-000071b0: 4c5f 4d61 696e 5769 6e64 6f77 0103 0000  L_MainWindow....
-000071c0: 000e 0026 0414 0430 043d 043d 044b 0435  ...&...0.=.=.K.5
-000071d0: 0800 0000 0006 0000 0005 2644 6174 6107  ..........&Data.
-000071e0: 0000 000e 4a41 4c5f 4d61 696e 5769 6e64  ....JAL_MainWind
-000071f0: 6f77 0103 0000 000c 0026 0412 044b 0445  ow.......&...K.E
-00007200: 043e 0434 0800 0000 0006 0000 0005 2645  .>.4..........&E
-00007210: 7869 7407 0000 000e 4a41 4c5f 4d61 696e  xit.....JAL_Main
-00007220: 5769 6e64 6f77 0103 0000 0010 0026 042d  Window.......&.-
-00007230: 043a 0441 043f 043e 0440 0442 0800 0000  .:.A.?.>.@.B....
-00007240: 0006 0000 0007 2645 7870 6f72 7407 0000  ......&Export...
-00007250: 000e 4a41 4c5f 4d61 696e 5769 6e64 6f77  ..JAL_MainWindow
-00007260: 0103 0000 000e 0026 0418 043c 043f 043e  .......&...<.?.>
-00007270: 0440 0442 0800 0000 0006 0000 0007 2649  .@.B..........&I
-00007280: 6d70 6f72 7407 0000 000e 4a41 4c5f 4d61  mport.....JAL_Ma
-00007290: 696e 5769 6e64 6f77 0103 0000 0012 0026  inWindow.......&
-000072a0: 041e 0441 043d 043e 0432 043d 043e 0435  ...A.=.>.2.=.>.5
-000072b0: 0800 0000 0006 0000 0005 264d 6169 6e07  ..........&Main.
-000072c0: 0000 000e 4a41 4c5f 4d61 696e 5769 6e64  ....JAL_MainWind
-000072d0: 6f77 0103 0000 0012 0026 041e 043f 0435  ow.......&...?.5
-000072e0: 0440 0430 0446 0438 0438 0800 0000 0006  .@.0.F.8.8......
-000072f0: 0000 000b 264f 7065 7261 7469 6f6e 7307  ....&Operations.
-00007300: 0000 000e 4a41 4c5f 4d61 696e 5769 6e64  ....JAL_MainWind
-00007310: 6f77 0103 0000 0018 041a 0026 043e 043d  ow.........&.>.=
-00007320: 0442 0440 0430 0433 0435 043d 0442 044b  .B.@.0.3.5.=.B.K
-00007330: 0800 0000 0006 0000 0006 2650 6565 7273  ..........&Peers
-00007340: 0700 0000 0e4a 414c 5f4d 6169 6e57 696e  .....JAL_MainWin
-00007350: 646f 7701 0300 0000 1400 2604 1a04 3e04  dow.......&...>.
-00007360: 4204 3804 4004 3e04 3204 3a04 3808 0000  B.8.@.>.2.:.8...
-00007370: 0000 0600 0000 0726 5175 6f74 6573 0700  .......&Quotes..
-00007380: 0000 0e4a 414c 5f4d 6169 6e57 696e 646f  ...JAL_MainWindo
-00007390: 7701 0300 0000 1a00 2604 1a04 3e04 4204  w.......&...>.B.
-000073a0: 3804 4004 3e04 3204 3a04 3800 2e00 2e00  8.@.>.2.:.8.....
-000073b0: 2e08 0000 0000 0600 0000 0a26 5175 6f74  ...........&Quot
-000073c0: 6573 2e2e 2e07 0000 000e 4a41 4c5f 4d61  es........JAL_Ma
-000073d0: 696e 5769 6e64 6f77 0103 0000 000e 0026  inWindow.......&
-000073e0: 041e 0442 0447 0435 0442 044b 0800 0000  ...B.G.5.B.K....
-000073f0: 0006 0000 0008 2652 6570 6f72 7473 0700  ......&Reports..
-00007400: 0000 0e4a 414c 5f4d 6169 6e57 696e 646f  ...JAL_MainWindo
-00007410: 7701 0300 0000 2400 2604 1204 3e04 4104  w.....$.&...>.A.
-00007420: 4104 4204 3004 3d04 3e04 3204 3b04 3504  A.B.0.=.>.2.;.5.
-00007430: 3d04 3804 3500 2e00 2e00 2e08 0000 0000  =.8.5...........
-00007440: 0600 0000 0b26 5265 7374 6f72 652e 2e2e  .....&Restore...
-00007450: 0700 0000 0e4a 414c 5f4d 6169 6e57 696e  .....JAL_MainWin
-00007460: 646f 7701 0300 0000 0c00 2604 1e04 4204  dow.......&...B.
-00007470: 4704 5104 4208 0000 0000 0600 0000 0a26  G.Q.B..........&
-00007480: 5374 6174 656d 656e 7407 0000 000e 4a41  Statement.....JA
-00007490: 4c5f 4d61 696e 5769 6e64 6f77 0103 0000  L_MainWindow....
-000074a0: 000a 0026 0422 044d 0433 0438 0800 0000  ...&.".M.3.8....
-000074b0: 0006 0000 0005 2654 6167 7307 0000 000e  ......&Tags.....
-000074c0: 4a41 4c5f 4d61 696e 5769 6e64 6f77 0103  JAL_MainWindow..
-000074d0: 0000 001c 0026 0426 0435 043d 043d 044b  .....&.&.5.=.=.K
-000074e0: 0435 0020 0431 0443 043c 0430 0433 0438  .5. .1.C.<.0.3.8
-000074f0: 0800 0000 0006 0000 0007 4126 7373 6574  ..........A&sset
-00007500: 7307 0000 000e 4a41 4c5f 4d61 696e 5769  s.....JAL_MainWi
-00007510: 6e64 6f77 0103 0000 004e 041e 0442 0447  ndow.....N...B.G
-00007520: 0435 0442 0020 043e 0020 0026 0434 0432  .5.B. .>. .&.4.2
-00007530: 0438 0436 0435 043d 0438 044f 0445 0020  .8.6.5.=.8.O.E. 
-00007540: 043f 043e 0020 0437 0430 0440 0443 0431  .?.>. .7.0.@.C.1
-00007550: 0435 0436 043d 044b 043c 0020 0441 0447  .5.6.=.K.<. .A.G
-00007560: 0435 0442 0430 043c 0800 0000 0006 0000  .5.B.0.<........
-00007570: 001d 466f 7265 6967 6e20 6163 636f 756e  ..Foreign accoun
-00007580: 7473 2026 666c 6f77 2072 6570 6f72 7407  ts &flow report.
-00007590: 0000 000e 4a41 4c5f 4d61 696e 5769 6e64  ....JAL_MainWind
-000075a0: 6f77 0103 0000 003e 0418 043d 0432 0435  ow.....>...=.2.5
-000075b0: 0441 0442 0438 0446 0438 043e 043d 043d  .A.B.8.F.8.>.=.=
-000075c0: 044b 0439 0020 0026 043d 0430 043b 043e  .K.9. .&.=.0.;.>
-000075d0: 0433 043e 0432 044b 0439 0020 043e 0442  .3.>.2.K.9. .>.B
-000075e0: 0447 0435 0442 0800 0000 0006 0000 0016  .G.5.B..........
-000075f0: 496e 7665 7374 6d65 6e74 2026 7461 7820  Investment &tax 
-00007600: 7265 706f 7274 0700 0000 0e4a 414c 5f4d  report.....JAL_M
-00007610: 6169 6e57 696e 646f 7701 0300 0000 0a00  ainWindow.......
-00007620: 2604 2f04 3704 4b04 3a08 0000 0000 0600  &./.7.K.:.......
-00007630: 0000 094c 2661 6e67 7561 6765 0700 0000  ...L&anguage....
-00007640: 0e4a 414c 5f4d 6169 6e57 696e 646f 7701  .JAL_MainWindow.
-00007650: 0300 0000 2a04 1f04 3504 4004 3504 4104  ....*...5.@.5.A.
-00007660: 4704 3804 4204 3004 4204 4c00 2000 2604  G.8.B.0.B.L. .&.
-00007670: 3804 4204 3e04 3304 3800 2e00 2e00 2e08  8.B.>.3.8.......
-00007680: 0000 0000 0600 0000 1352 652d 6275 696c  .........Re-buil
-00007690: 6420 264c 6564 6765 722e 2e2e 0700 0000  d &Ledger.......
-000076a0: 0e4a 414c 5f4d 6169 6e57 696e 646f 7701  .JAL_MainWindow.
-000076b0: 0300 0000 1604 2704 3504 3a00 2000 5b00  ......'.5.:. .[.
-000076c0: 5200 5500 5d00 2e00 2e00 2e08 0000 0000  R.U.]...........
-000076d0: 0600 0000 0c53 6c69 7020 5b52 555d 2e2e  .....Slip [RU]..
-000076e0: 2e07 0000 000e 4a41 4c5f 4d61 696e 5769  ......JAL_MainWi
-000076f0: 6e64 6f77 0103 0000 0006 006a 0061 006c  ndow.......j.a.l
-00007700: 0800 0000 0006 0000 0003 6a61 6c07 0000  ..........jal...
-00007710: 000e 4a41 4c5f 4d61 696e 5769 6e64 6f77  ..JAL_MainWindow
-00007720: 0103 0000 0020 0411 0430 043d 043a 0020  ..... ...0.=.:. 
-00007730: 0434 043b 044f 0020 0441 0447 0435 0442  .4.;.O. .A.G.5.B
-00007740: 0430 0020 2116 0800 0000 0006 0000 0012  .0. !...........
-00007750: 4261 6e6b 2066 6f72 2061 6363 6f75 6e74  Bank for account
-00007760: 2023 0700 0000 0a4a 616c 4163 636f 756e   #.....JalAccoun
-00007770: 7401 0300 0000 2a04 2104 4204 4004 3004  t.....*.!.B.@.0.
-00007780: 3d04 3000 2004 3e04 3104 3d04 3e04 3204  =.0. .>.1.=.>.2.
-00007790: 3b04 5104 3d04 3000 2004 3404 3b04 4f00  ;.Q.=.0. .4.;.O.
-000077a0: 2008 0000 0000 0600 0000 1443 6f75 6e74   ..........Count
-000077b0: 7279 2075 7064 6174 6564 2066 6f72 2007  ry updated for .
-000077c0: 0000 0008 4a61 6c41 7373 6574 0103 0000  ....JalAsset....
-000077d0: 002a 041a 043e 0442 0438 0440 043e 0432  .*...>.B.8.@.>.2
-000077e0: 043a 0438 0020 043e 0431 043d 043e 0432  .:.8. .>.1.=.>.2
-000077f0: 043b 0435 043d 044b 003a 0020 0800 0000  .;.5.=.K.:. ....
-00007800: 0006 0000 0019 5175 6f74 6174 696f 6e73  ......Quotations
-00007810: 2077 6572 6520 7570 6461 7465 643a 2007   were updated: .
-00007820: 0000 0008 4a61 6c41 7373 6574 0103 0000  ....JalAsset....
-00007830: 0046 0420 0435 0433 0438 0441 0442 0440  .F. .5.3.8.A.B.@
-00007840: 0430 0446 0438 043e 043d 043d 044b 0439  .0.F.8.>.=.=.K.9
-00007850: 0020 043d 043e 043c 0435 0440 0020 043e  . .=.>.<.5.@. .>
-00007860: 0431 043d 043e 0432 043b 0451 043d 0020  .1.=.>.2.;.Q.=. 
-00007870: 0434 043b 044f 0020 0800 0000 0006 0000  .4.;.O. ........
-00007880: 0017 5265 672e 6e75 6d62 6572 2075 7064  ..Reg.number upd
-00007890: 6174 6564 2066 6f72 2007 0000 0008 4a61  ated for .....Ja
-000078a0: 6c41 7373 6574 0103 0000 0030 041d 0435  lAsset.....0...5
-000078b0: 0442 0020 043a 043e 0442 0438 0440 043e  .B. .:.>.B.8.@.>
-000078c0: 0432 043a 0438 002f 043a 0443 0440 0441  .2.:.8./.:.C.@.A
-000078d0: 0430 0020 0434 043b 044f 0020 0800 0000  .0. .4.;.O. ....
-000078e0: 0006 0000 001c 5468 6572 6520 6172 6520  ......There are 
-000078f0: 6e6f 2071 756f 7465 2f72 6174 6520 666f  no quote/rate fo
-00007900: 7220 0700 0000 084a 616c 4173 7365 7401  r .....JalAsset.
-00007910: 0300 0000 4c04 1d04 3504 3e04 3604 3804  ....L...5.>.6.8.
-00007920: 3404 3004 3d04 3d04 3004 4f00 2004 3f04  4.0.=.=.0.O. .?.
-00007930: 3e04 3f04 4b04 4204 3a04 3000 2004 3e04  >.?.K.B.:.0. .>.
-00007940: 3104 3d04 3e04 3204 3804 4204 4c00 2000  1.=.>.2.8.B.L. .
-00007950: 4900 5300 4900 4e00 2004 3404 3b04 4f00  I.S.I.N. .4.;.O.
-00007960: 2008 0000 0000 0600 0000 2655 6e65 7870   .........&Unexp
-00007970: 6563 7465 6420 6174 7465 6d70 7420 746f  ected attempt to
-00007980: 2075 7064 6174 6520 4953 494e 2066 6f72   update ISIN for
-00007990: 2007 0000 0008 4a61 6c41 7373 6574 0103   .....JalAsset..
-000079a0: 0000 0006 0020 0432 0020 0800 0000 0006  ..... .2. ......
-000079b0: 0000 0006 2069 6e74 6f20 0700 0000 094a  .... into .....J
-000079c0: 616c 4261 636b 7570 0103 0000 001c 0410  alBackup........
-000079d0: 0440 0445 0438 0432 044b 0020 0028 002a  .@.E.8.2.K. .(.*
-000079e0: 002e 0074 0067 007a 0029 0800 0000 0006  ...t.g.z.)......
-000079f0: 0000 0010 4172 6368 6976 6573 2028 2a2e  ....Archives (*.
-00007a00: 7467 7a29 0700 0000 094a 616c 4261 636b  tgz).....JalBack
-00007a10: 7570 0103 0000 0046 041d 0435 0020 0440  up.....F...5. .@
-00007a20: 0430 0441 043f 043e 0437 043d 0430 043d  .0.A.?.>.7.=.0.=
-00007a30: 0430 0020 043c 0435 0442 043a 0430 0020  .0. .<.5.B.:.0. 
-00007a40: 0440 0435 0437 0435 0440 0432 043d 043e  .@.5.7.5.@.2.=.>
-00007a50: 0439 0020 043a 043e 043f 0438 0438 0800  .9. .:.>.?.8.8..
-00007a60: 0000 0006 0000 001b 4261 636b 7570 206c  ........Backup l
-00007a70: 6162 656c 206e 6f74 2072 6563 6f67 6e69  abel not recogni
-00007a80: 7a65 6407 0000 0009 4a61 6c42 6163 6b75  zed.....JalBacku
-00007a90: 7001 0300 0000 4604 2004 3504 3704 3504  p.....F. .5.7.5.
-00007aa0: 4004 3204 3d04 3004 4f00 2004 3a04 3e04  @.2.=.0.O. .:.>.
-00007ab0: 3f04 3804 4f00 2004 3204 3e04 4104 4104  ?.8.O. .2.>.A.A.
-00007ac0: 4204 3004 3204 3d04 3e04 3204 3b04 3504  B.0.2.=.>.2.;.5.
-00007ad0: 3d04 3000 2004 3804 3700 3a00 2008 0000  =.0. .8.7.:. ...
-00007ae0: 0000 0600 0000 1642 6163 6b75 7020 7265  .......Backup re
-00007af0: 7374 6f72 6564 2066 726f 6d3a 2007 0000  stored from: ...
-00007b00: 0009 4a61 6c42 6163 6b75 7001 0300 0000  ..JalBackup.....
-00007b10: 3a04 2004 3504 3704 3504 4004 3204 3d04  :. .5.7.5.@.2.=.
-00007b20: 3004 4f00 2004 3a04 3e04 3f04 3804 4f00  0.O. .:.>.?.8.O.
-00007b30: 2004 4104 3e04 4504 4004 3004 3d04 5104   .A.>.E.@.0.=.Q.
-00007b40: 3d04 3000 2004 3200 3a00 2008 0000 0000  =.0. .2.:. .....
-00007b50: 0600 0000 1142 6163 6b75 7020 7361 7665  .....Backup save
-00007b60: 6420 696e 3a20 0700 0000 094a 616c 4261  d in: .....JalBa
-00007b70: 636b 7570 0103 0000 0052 041d 0435 0432  ckup.....R...5.2
-00007b80: 043e 0437 043c 043e 0436 043d 043e 0020  .>.7.<.>.6.=.>. 
-00007b90: 043f 0440 043e 0432 0435 0440 0438 0442  .?.@.>.2.5.@.8.B
-00007ba0: 044c 0020 0434 0430 0442 0443 0020 0440  .L. .4.0.B.C. .@
-00007bb0: 0435 0437 0435 0440 0432 043d 043e 0439  .5.7.5.@.2.=.>.9
-00007bc0: 0020 043a 043e 043f 0438 0438 0800 0000  . .:.>.?.8.8....
-00007bd0: 0006 0000 001a 4361 6e27 7420 7661 6c69  ......Can't vali
-00007be0: 6461 7465 2062 6163 6b75 7020 6461 7465  date backup date
-00007bf0: 0700 0000 094a 616c 4261 636b 7570 0103  .....JalBackup..
-00007c00: 0000 0028 0414 0430 043d 043d 044b 0435  ...(...0.=.=.K.5
-00007c10: 0020 0432 043e 0441 0441 0442 0430 043d  . .2.>.A.A.B.0.=
-00007c20: 043e 0432 043b 0435 043d 044b 0800 0000  .>.2.;.5.=.K....
-00007c30: 0006 0000 000d 4461 7461 2072 6573 746f  ......Data resto
-00007c40: 7265 6407 0000 0009 4a61 6c42 6163 6b75  red.....JalBacku
-00007c50: 7001 0300 0000 4204 1404 3004 3d04 3d04  p.....B...0.=.=.
-00007c60: 4b04 3500 2004 3104 4b04 3b04 3800 2004  K.5. .1.K.;.8. .
-00007c70: 3704 3004 3304 4004 4304 3604 3504 3d04  7.0.3.@.C.6.5.=.
-00007c80: 4b00 2004 3804 3700 2004 3104 4d04 3a04  K. .8.7. .1.M.:.
-00007c90: 3004 3f04 3000 2e00 0a08 0000 0000 0600  0.?.0...........
-00007ca0: 0000 2544 6174 6162 6173 6520 7761 7320  ..%Database was 
-00007cb0: 6c6f 6164 6564 2066 726f 6d20 7468 6520  loaded from the 
-00007cc0: 6261 636b 7570 2e0a 0700 0000 094a 616c  backup.......Jal
-00007cd0: 4261 636b 7570 0103 0000 004e 041d 0435  Backup.....N...5
-00007ce0: 0020 0443 0434 0430 043b 043e 0441 044c  . .C.4.0.;.>.A.L
-00007cf0: 0020 0432 043e 0441 0441 0442 0430 043d  . .2.>.A.A.B.0.=
-00007d00: 043e 0432 0438 0442 044c 0020 0440 0435  .>.2.8.B.L. .@.5
-00007d10: 0437 0435 0440 0432 043d 0443 044e 0020  .7.5.@.2.=.C.N. 
-00007d20: 043a 043e 043f 0438 044e 0800 0000 0006  .:.>.?.8.N......
-00007d30: 0000 001d 4661 696c 6564 2074 6f20 7265  ....Failed to re
-00007d40: 7374 6f72 6520 6261 636b 7570 2066 696c  store backup fil
-00007d50: 6507 0000 0009 4a61 6c42 6163 6b75 7001  e.....JalBackup.
-00007d60: 0300 0000 3804 2104 3e04 4504 4004 3004  ....8.!.>.E.@.0.
-00007d70: 3d04 3804 4204 4c00 2004 4004 3504 3704  =.8.B.L. .@.5.7.
-00007d80: 3504 4004 3204 3d04 4304 4e00 2004 3a04  5.@.2.=.C.N. .:.
-00007d90: 3e04 3f04 3804 4e00 2004 3200 3a08 0000  >.?.8.N. .2.:...
-00007da0: 0000 0600 0000 0f53 6176 6520 6261 636b  .......Save back
-00007db0: 7570 2074 6f3a 0700 0000 094a 616c 4261  up to:.....JalBa
-00007dc0: 636b 7570 0103 0000 0040 0412 044b 0431  ckup.....@...K.1
-00007dd0: 0435 0440 0438 0442 0435 0020 0444 0430  .5.@.8.B.5. .D.0
-00007de0: 0439 043b 0020 0441 0020 0440 0435 0437  .9.;. .A. .@.5.7
-00007df0: 0435 0440 0432 043d 043e 0439 0020 043a  .5.@.2.=.>.9. .:
-00007e00: 043e 043f 0438 0435 0439 0800 0000 0006  .>.?.8.5.9......
-00007e10: 0000 0017 5365 6c65 6374 2066 696c 6520  ....Select file 
-00007e20: 7769 7468 2062 6163 6b75 7007 0000 0009  with backup.....
-00007e30: 4a61 6c42 6163 6b75 7001 0300 0000 4a04  JalBackup.....J.
-00007e40: 1d04 3504 3204 3504 4004 3d04 4b04 3900  ..5.2.5.@.=.K.9.
-00007e50: 2004 4404 3e04 4004 3c04 3004 4200 2004   .D.>.@.<.0.B. .
-00007e60: 4404 3004 3904 3b04 3000 2004 4004 3504  D.0.9.;.0. .@.5.
-00007e70: 3704 3504 4004 3204 3d04 3e04 3900 2004  7.5.@.2.=.>.9. .
-00007e80: 3a04 3e04 3f04 3804 3808 0000 0000 0600  :.>.?.8.8.......
-00007e90: 0000 1b57 726f 6e67 2066 6f72 6d61 7420  ...Wrong format 
-00007ea0: 6f66 2062 6163 6b75 7020 6669 6c65 0700  of backup file..
-00007eb0: 0000 094a 616c 4261 636b 7570 0103 0000  ...JalBackup....
-00007ec0: 00c8 0412 044b 0020 0434 043e 043b 0436  .....K. .4.>.;.6
-00007ed0: 043d 044b 0020 043f 0435 0440 0435 0437  .=.K. .?.5.@.5.7
-00007ee0: 0430 043f 0443 0441 0442 0438 0442 044c  .0.?.C.A.B.8.B.L
-00007ef0: 0020 043f 0440 0438 043b 043e 0436 0435  . .?.@.8.;.>.6.5
-00007f00: 043d 0438 0435 002c 0020 0447 0442 043e  .=.8.5.,. .G.B.>
-00007f10: 0431 044b 0020 043f 0440 0438 043c 0435  .1.K. .?.@.8.<.5
-00007f20: 043d 0438 0442 044c 0020 0438 0437 043c  .=.8.B.L. .8.7.<
-00007f30: 0435 043d 0435 043d 0438 044f 000a 041f  .5.=.5.=.8.O....
-00007f40: 0440 0438 043b 043e 0436 0435 043d 0438  .@.8.;.>.6.5.=.8
-00007f50: 0435 0020 0441 0435 0439 0447 0430 0441  .5. .A.5.9.G.0.A
-00007f60: 0020 0437 0430 0432 0435 0440 0448 0438  . .7.0.2.5.@.H.8
-00007f70: 0442 0020 0441 0432 043e 044e 0020 0440  .B. .A.2.>.N. .@
-00007f80: 0430 0431 043e 0442 0443 0800 0000 0006  .0.1.>.B.C......
-00007f90: 0000 0052 596f 7520 7368 6f75 6c64 2072  ...RYou should r
-00007fa0: 6573 7461 7274 2061 7070 6c69 6361 7469  estart applicati
-00007fb0: 6f6e 2074 6f20 6170 706c 7920 6368 616e  on to apply chan
-00007fc0: 6765 730a 4170 706c 6963 6174 696f 6e20  ges.Application 
-00007fd0: 7769 6c6c 2062 6520 7465 726d 696e 6174  will be terminat
-00007fe0: 6564 206e 6f77 0700 0000 094a 616c 4261  ed now.....JalBa
-00007ff0: 636b 7570 0103 0000 0064 041e 043f 0435  ckup.....d...?.5
-00008000: 0440 0430 0446 0438 044f 0020 0443 0436  .@.0.F.8.O. .C.6
-00008010: 0435 0020 0435 0441 0442 044c 0020 0432  .5. .5.A.B.L. .2
-00008020: 0020 0431 0430 0437 0435 0020 0434 0430  . .1.0.7.5. .4.0
-00008030: 043d 043d 044b 0445 0020 0438 0020 0431  .=.=.K.E. .8. .1
-00008040: 044b 043b 0430 0020 043f 0440 043e 043f  .K.;.0. .?.@.>.?
-00008050: 0443 0449 0435 043d 0430 003a 0020 0800  .C.I.5.=.0.:. ..
-00008060: 0000 0006 0000 0031 4f70 6572 6174 696f  .......1Operatio
-00008070: 6e20 616c 7265 6164 7920 7072 6573 656e  n already presen
-00008080: 7420 696e 2064 6220 616e 6420 7761 7320  t in db and was 
-00008090: 736b 6970 7065 643a 2007 0000 0005 4a61  skipped: .....Ja
-000080a0: 6c44 4201 0300 0000 6e00 2004 3804 3c04  lDB.....n. .8.<.
-000080b0: 3504 3504 4200 2004 3d04 3504 4104 3e04  5.5.B. .=.5.A.>.
-000080c0: 4504 4004 3004 3d04 5104 3d04 3d04 4b04  E.@.0.=.Q.=.=.K.
-000080d0: 3500 2004 3804 3704 3c04 3504 3d04 3504  5. .8.7.<.5.=.5.
-000080e0: 3d04 3804 4f00 2c00 0a04 3204 4b00 2004  =.8.O.,...2.K. .
-000080f0: 4504 3e04 4204 3804 4204 3500 2004 3804  E.>.B.8.B.5. .8.
-00008100: 4500 2004 4104 3e04 4504 4004 3004 3d04  E. .A.>.E.@.0.=.
-00008110: 3804 4204 4c00 3f08 0000 0000 0600 0000  8.B.L.?.........
-00008120: 3120 6861 7320 756e 636f 6d6d 6974 7465  1 has uncommitte
-00008130: 6420 6368 616e 6765 732c 0a64 6f20 796f  d changes,.do yo
-00008140: 7520 7761 6e74 2074 6f20 7361 7665 2069  u want to save i
-00008150: 743f 0700 0000 114a 616c 4f70 6572 6174  t?.....JalOperat
-00008160: 696f 6e73 5461 6273 0103 0000 0036 0415  ionsTabs.....6..
-00008170: 0441 0442 044c 0020 043d 0435 0441 043e  .A.B.L. .=.5.A.>
-00008180: 0445 0440 0430 043d 0451 043d 043d 044b  .E.@.0.=.Q.=.=.K
-00008190: 0435 0020 0438 0437 043c 0435 043d 043d  .5. .8.7.<.5.=.=
-000081a0: 0438 044f 0800 0000 0006 0000 0018 596f  .8.O..........Yo
-000081b0: 7520 6861 7665 2075 6e73 6176 6564 2063  u have unsaved c
-000081c0: 6861 6e67 6573 0700 0000 114a 616c 4f70  hanges.....JalOp
-000081d0: 6572 6174 696f 6e73 5461 6273 0103 0000  erationsTabs....
-000081e0: 005a 041d 0435 0432 043e 0437 043c 043e  .Z...5.2.>.7.<.>
-000081f0: 0436 043d 043e 0020 0443 0434 0430 043b  .6.=.>. .C.4.0.;
-00008200: 0438 0442 044c 0020 043f 0440 0435 0434  .8.B.L. .?.@.5.4
-00008210: 043e 043f 0440 0435 0434 0435 043b 0451  .>.?.@.5.4.5.;.Q
-00008220: 043d 043d 0443 044e 0020 043a 0430 0442  .=.=.C.N. .:.0.B
-00008230: 0435 0433 043e 0440 0438 044e 0800 0000  .5.3.>.@.8.N....
-00008240: 0006 0000 0020 4361 6e27 7420 6465 6c65  ..... Can't dele
-00008250: 7465 2070 7265 6465 6669 6e65 6420 6361  te predefined ca
-00008260: 7465 676f 7279 0700 0000 0b4a 616c 5371  tegory.....JalSq
-00008270: 6c45 7272 6f72 0103 0000 009e 042d 0442  lError.......-.B
-00008280: 0438 0020 0434 0430 043d 043d 044b 0435  .8. .4.0.=.=.K.5
-00008290: 0020 043d 0435 0020 043c 043e 0433 0443  . .=.5. .<.>.3.C
-000082a0: 0442 0020 0431 044b 0442 044c 0020 043c  .B. .1.K.B.L. .<
-000082b0: 043e 0434 0438 0444 0438 0446 0438 0440  .>.4.8.D.8.F.8.@
-000082c0: 043e 0432 0430 043d 044b 002c 0020 0442  .>.2.0.=.K.,. .B
-000082d0: 002e 043a 002e 0020 043d 0430 0020 043d  ...:... .=.0. .=
-000082e0: 0438 0445 0020 0435 0441 0442 044c 0020  .8.E. .5.A.B.L. 
-000082f0: 0441 0441 044b 043b 043a 0430 0020 0432  .A.A.K.;.:.0. .2
-00008300: 0020 0434 0440 0443 0433 043e 043c 0020  . .4.@.C.3.>.<. 
-00008310: 043c 0435 0441 0442 0435 0800 0000 0006  .<.5.A.B.5......
-00008320: 0000 003a 4461 7461 2061 7265 2072 6566  ...:Data are ref
-00008330: 6572 656e 6365 6420 696e 2061 6e6f 7468  erenced in anoth
-00008340: 6572 2070 6c61 6365 2061 6e64 2063 616e  er place and can
-00008350: 2774 2062 6520 6d6f 6469 6669 6564 0700  't be modified..
-00008360: 0000 0b4a 616c 5371 6c45 7272 6f72 0103  ...JalSqlError..
-00008370: 0000 001e 041e 0448 0438 0431 043a 0430  .......H.8.1.:.0
-00008380: 0020 0432 0020 0434 0430 043d 043d 044b  . .2. .4.0.=.=.K
-00008390: 0445 0800 0000 0006 0000 000e 4461 7461  .E..........Data
-000083a0: 6261 7365 2065 7272 6f72 0700 0000 0b4a  base error.....J
-000083b0: 616c 5371 6c45 7272 6f72 0103 0000 0050  alSqlError.....P
-000083c0: 041d 0435 0432 0435 0440 043d 043e 0020  ...5.2.5.@.=.>. 
-000083d0: 0432 044b 0431 0440 0430 043d 0430 0020  .2.K.1.@.0.=.0. 
-000083e0: 0432 0430 043b 044e 0442 0430 0020 0434  .2.0.;.N.B.0. .4
-000083f0: 043b 044f 0020 0446 0435 043d 043d 043e  .;.O. .F.5.=.=.>
-00008400: 0439 0020 0431 0443 043c 0430 0433 0438  .9. .1.C.<.0.3.8
-00008410: 0800 0000 0006 0000 002a 496e 636f 7272  .........*Incorr
-00008420: 6563 7420 6375 7272 656e 6379 2061 7373  ect currency ass
-00008430: 6967 6e6d 656e 7420 666f 7220 616e 2061  ignment for an a
-00008440: 7373 6574 0700 0000 0b4a 616c 5371 6c45  sset.....JalSqlE
-00008450: 7272 6f72 0103 0000 0080 041f 043e 043b  rror.........>.;
-00008460: 0435 0020 0411 0430 043d 043a 002f 0411  .5. ...0.=.:./..
-00008470: 0440 043e 043a 0435 0440 0020 0434 043e  .@.>.:.5.@. .4.>
-00008480: 043b 0436 043d 043e 0020 0431 044b 0442  .;.6.=.>. .1.K.B
-00008490: 044c 0020 0437 0430 043f 043e 043b 043d  .L. .7.0.?.>.;.=
-000084a0: 0435 043d 043e 0020 0434 043b 044f 0020  .5.=.>. .4.;.O. 
-000084b0: 0438 043d 0432 0435 0441 0442 0438 0446  .8.=.2.5.A.B.8.F
-000084c0: 0438 043e 043d 043d 043e 0433 043e 0020  .8.>.=.=.>.3.>. 
-000084d0: 0441 0447 0435 0442 0430 0800 0000 0006  .A.G.5.B.0......
-000084e0: 0000 0039 496e 7665 7374 6d65 6e74 2061  ...9Investment a
-000084f0: 6363 6f75 6e74 2073 686f 756c 6420 6861  ccount should ha
-00008500: 7665 2061 7373 6f63 6961 7465 6420 6272  ve associated br
-00008510: 6f6b 6572 2061 7373 6967 6e65 6407 0000  oker assigned...
-00008520: 000b 4a61 6c53 716c 4572 726f 7201 0300  ..JalSqlError...
-00008530: 0000 8800 2004 3e04 3f04 3504 4004 3004  .... .>.?.5.@.0.
-00008540: 4604 3804 3900 2004 4204 4004 3504 3104  F.8.9. .B.@.5.1.
-00008550: 4304 4e04 4200 2004 3f04 3504 4004 3504  C.N.B. .?.5.@.5.
-00008560: 4004 3004 4104 4704 3504 4204 3000 2e00  @.0.A.G.5.B.0...
-00008570: 2004 1204 4b00 2004 4504 3e04 3404 3804   ...K. .E.>.4.8.
-00008580: 4204 3500 2004 3204 4b04 3f04 3e04 3b04  B.5. .2.K.?.>.;.
-00008590: 3d04 3804 4204 4c00 2004 3504 3304 3e00  =.8.B.L. .5.3.>.
-000085a0: 2004 3f04 4004 4f04 3c04 3e00 2004 4104   .?.@.O.<.>. .A.
-000085b0: 3504 3904 4704 3004 4100 3f08 0000 0000  5.9.G.0.A.?.....
-000085c0: 0600 0000 3c20 6f70 6572 6174 696f 6e73  ....< operations
-000085d0: 2072 6571 7569 7265 2072 6562 7569 6c64   require rebuild
-000085e0: 2e20 446f 2079 6f75 2077 616e 7420 746f  . Do you want to
-000085f0: 2064 6f20 6974 2072 6967 6874 206e 6f77   do it right now
-00008600: 3f07 0000 0006 4c65 6467 6572 0103 0000  ?.....Ledger....
-00008610: 0022 002c 0020 043d 043e 0432 0430 044f  .".,. .=.>.2.0.O
-00008620: 0020 0433 0440 0430 043d 0438 0446 0430  . .3.@.0.=.8.F.0
-00008630: 003a 0020 0800 0000 0006 0000 0010 2c20  .:. .........., 
-00008640: 6e65 7720 6672 6f6e 7469 6572 3a20 0700  new frontier: ..
-00008650: 0000 064c 6564 6765 7201 0300 0000 1a04  ...Ledger.......
-00008660: 1f04 3e04 3404 4204 3204 3504 4004 3604  ..>.4.B.2.5.@.6.
-00008670: 3404 3504 3d04 3804 3508 0000 0000 0600  4.5.=.8.5.......
-00008680: 0000 0c43 6f6e 6669 726d 6174 696f 6e07  ...Confirmation.
-00008690: 0000 0006 4c65 6467 6572 0103 0000 0094  ....Ledger......
-000086a0: 041f 0440 043e 0438 0437 043e 0448 043b  ...@.>.8.7.>.H.;
-000086b0: 0430 0020 043e 0448 0438 0431 043a 0430  .0. .>.H.8.1.:.0
-000086c0: 002e 0020 0420 0430 0441 0447 0451 0442  ... . .0.A.G.Q.B
-000086d0: 0020 0438 0442 043e 0433 043e 0432 0020  . .8.B.>.3.>.2. 
-000086e0: 043d 0435 0020 043e 043a 043e 043d 0447  .=.5. .>.:.>.=.G
-000086f0: 0435 043d 002e 0020 041f 0440 043e 0432  .5.=... ...@.>.2
-00008700: 0435 0440 044c 0442 0435 0020 0441 043e  .5.@.L.B.5. .A.>
-00008710: 043e 0431 0449 0435 043d 0438 044f 0020  .>.1.I.5.=.8.O. 
-00008720: 043e 0431 0020 043e 0448 0438 0431 043a  .>.1. .>.H.8.1.:
-00008730: 0430 0445 0800 0000 0006 0000 004d 4578  .0.E.........MEx
-00008740: 6365 7074 696f 6e20 6861 7070 656e 6564  ception happened
-00008750: 2e20 4c65 6467 6572 2069 7320 696e 636f  . Ledger is inco
-00008760: 6d70 6c65 7465 2e20 506c 6561 7365 2063  mplete. Please c
-00008770: 6f72 7265 6374 2065 7272 6f72 7320 6c69  orrect errors li
-00008780: 7374 6564 2069 6e20 6c6f 6707 0000 0006  sted in log.....
-00008790: 4c65 6467 6572 0103 0000 004a 0418 0442  Ledger.....J...B
-000087a0: 043e 0433 0438 0020 0440 0430 0441 0441  .>.3.8. .@.0.A.A
-000087b0: 0447 0438 0442 0430 043d 044b 002e 0020  .G.8.B.0.=.K... 
-000087c0: 0417 0430 0442 0440 0430 0447 0435 043d  ...0.B.@.0.G.5.=
-000087d0: 043d 043e 0435 0020 0432 0440 0435 043c  .=.>.5. .2.@.5.<
-000087e0: 044f 003a 0020 0800 0000 0006 0000 0022  .O.:. ........."
-000087f0: 4c65 6467 6572 2069 7320 636f 6d70 6c65  Ledger is comple
-00008800: 7465 2e20 456c 6170 7365 6420 7469 6d65  te. Elapsed time
-00008810: 3a20 0700 0000 064c 6564 6765 7201 0300  : .....Ledger...
-00008820: 0000 2c04 2204 4004 3004 3d04 3704 3004  ..,.".@.0.=.7.0.
-00008830: 3a04 4604 3804 3800 2004 3e04 4204 4104  :.F.8.8. .>.B.A.
-00008840: 4304 4204 4104 4204 3204 4304 4e04 4208  C.B.A.B.2.C.N.B.
-00008850: 0000 0000 0600 0000 0e4c 6567 6572 2069  .........Leger i
-00008860: 7320 656d 7074 7907 0000 0006 4c65 6467  s empty.....Ledg
-00008870: 6572 0103 0000 0026 041d 0435 0020 0443  er.....&...5. .C
-00008880: 043a 0430 0437 0430 043d 0430 0020 0426  .:.0.7.0.=.0. .&
-00008890: 0411 0020 0434 043b 044f 003a 0020 0800  ... .4.;.O.:. ..
-000088a0: 0000 0006 0000 0016 4e6f 2061 7373 6574  ........No asset
-000088b0: 2064 6566 696e 6564 2066 6f72 3a20 0700   defined for: ..
-000088c0: 0000 064c 6564 6765 7201 0300 0000 3404  ...Ledger.....4.
-000088d0: 1d04 4300 2004 4304 3a04 3004 3704 3004  ..C. .C.:.0.7.0.
-000088e0: 3d04 3000 2004 3a04 3004 4204 3504 3304  =.0. .:.0.B.5.3.
-000088f0: 3e04 4004 3804 4f00 2004 3404 3b04 4f00  >.@.8.O. .4.;.O.
-00008900: 3a00 2008 0000 0000 0600 0000 154e 6f20  :. ..........No 
-00008910: 6361 7465 676f 7279 2073 6574 2066 6f72  category set for
-00008920: 3a20 0700 0000 064c 6564 6765 7201 0300  : .....Ledger...
-00008930: 0000 3404 1d04 3500 2004 4304 3a04 3004  ..4...5. .C.:.0.
-00008940: 3704 3004 3d00 2004 3a04 3e04 3d04 4204  7.0.=. .:.>.=.B.
-00008950: 4004 3004 3304 3504 3d04 4200 2004 3404  @.0.3.5.=.B. .4.
-00008960: 3b04 4f00 3a00 2008 0000 0000 0600 0000  ;.O.:. .........
-00008970: 114e 6f20 7065 6572 2073 6574 2066 6f72  .No peer set for
-00008980: 3a20 0700 0000 064c 6564 6765 7201 0300  : .....Ledger...
-00008990: 0000 2604 1f04 3504 4004 3504 4104 4704  ..&...5.@.5.A.G.
-000089a0: 5104 4200 2004 3804 4204 3e04 3304 3e04  Q.B. .8.B.>.3.>.
-000089b0: 3200 2004 4100 3a00 2008 0000 0000 0600  2. .A.:. .......
-000089c0: 0000 1a52 652d 6275 696c 6469 6e67 206c  ...Re-building l
-000089d0: 6564 6765 7220 7369 6e63 653a 2007 0000  edger since: ...
-000089e0: 0006 4c65 6467 6572 0103 0000 0058 041d  ..Ledger.....X..
-000089f0: 0435 0438 0437 0432 0435 0441 0442 043d  .5.8.7.2.5.A.B.=
-00008a00: 044b 0439 0020 043f 0430 0440 0430 043c  .K.9. .?.0.@.0.<
-00008a10: 0435 0442 0440 0020 043a 0440 0438 0442  .5.B.@. .:.@.8.B
-00008a20: 0438 0447 043d 043e 0441 0442 0438 0020  .8.G.=.>.A.B.8. 
-00008a30: 0441 043e 043e 0431 0449 0435 043d 0438  .A.>.>.1.I.5.=.8
-00008a40: 044f 003a 0020 0800 0000 0006 0000 0020  .O.:. ......... 
-00008a50: 556e 6b6e 6f77 6e20 6c6f 6767 696e 6720  Unknown logging 
-00008a60: 6c65 7665 6c20 7072 6f76 6964 6564 3a20  level provided: 
-00008a70: 0700 0000 094c 6f67 5669 6577 6572 0103  .....LogViewer..
-00008a80: 0000 000c 25b2 0020 006c 006f 0067 0073  ....%.. .l.o.g.s
-00008a90: 0800 0000 0006 0000 0008 e296 b220 6c6f  ............. lo
-00008aa0: 6773 0700 0000 094c 6f67 5669 6577 6572  gs.....LogViewer
-00008ab0: 0103 0000 000c 25b6 0020 006c 006f 0067  ......%.. .l.o.g
-00008ac0: 0073 0800 0000 0006 0000 0008 e296 b620  .s............. 
-00008ad0: 6c6f 6773 0700 0000 094c 6f67 5669 6577  logs.....LogView
-00008ae0: 6572 0103 0000 003e 041e 0448 0438 0431  er.....>...H.8.1
-00008af0: 043a 0430 0020 043b 043e 0433 0438 043d  .:.0. .;.>.3.8.=
-00008b00: 0430 0020 0447 0435 0440 0435 0437 0020  .0. .G.5.@.5.7. 
-00008b10: 0413 043e 0441 0443 0441 043b 0443 0433  ...>.A.C.A.;.C.3
-00008b20: 0438 003a 0020 0800 0000 0006 0000 0013  .8.:. ..........
-00008b30: 4553 4941 206c 6f67 696e 2066 6169 6c65  ESIA login faile
-00008b40: 643a 2007 0000 0008 4c6f 6769 6e46 4e53  d: .....LoginFNS
-00008b50: 0103 0000 0040 0423 0441 043f 0435 0448  .....@.#.A.?.5.H
-00008b60: 043d 044b 0439 0020 043b 043e 0433 0438  .=.K.9. .;.>.3.8
-00008b70: 043d 0020 0447 0435 0440 0435 0437 0020  .=. .G.5.@.5.7. 
-00008b80: 0413 043e 0441 0443 0441 043b 0443 0433  ...>.A.C.A.;.C.3
-00008b90: 0438 003a 0020 0800 0000 0006 0000 0017  .8.:. ..........
-00008ba0: 4553 4941 206c 6f67 696e 2073 7563 6365  ESIA login succe
-00008bb0: 7373 6675 6c3a 2007 0000 0008 4c6f 6769  ssful: .....Logi
-00008bc0: 6e46 4e53 0103 0000 0038 041e 0448 0438  nFNS.....8...H.8
-00008bd0: 0431 043a 0430 0020 043b 043e 0433 0438  .1.:.0. .;.>.3.8
-00008be0: 043d 0430 0020 0447 0435 0440 0435 0437  .=.0. .G.5.@.5.7
-00008bf0: 0020 041b 041a 0020 0424 041d 0421 003a  . ..... .$...!.:
-00008c00: 0020 0800 0000 0006 0000 0012 464e 5320  . ..........FNS 
-00008c10: 6c6f 6769 6e20 6661 696c 6564 3a20 0700  login failed: ..
-00008c20: 0000 084c 6f67 696e 464e 5301 0300 0000  ...LoginFNS.....
-00008c30: 3a04 2304 4104 3f04 3504 4804 3d04 4b04  :.#.A.?.5.H.=.K.
-00008c40: 3900 2004 3b04 3e04 3304 3804 3d00 2004  9. .;.>.3.8.=. .
-00008c50: 4704 3504 4004 3504 3700 2004 1b04 1a00  G.5.@.5.7. .....
-00008c60: 2004 2404 1d04 2100 3a00 2008 0000 0000   .$...!.:. .....
-00008c70: 0600 0000 1646 4e53 206c 6f67 696e 2073  .....FNS login s
-00008c80: 7563 6365 7373 6675 6c3a 2007 0000 0008  uccessful: .....
-00008c90: 4c6f 6769 6e46 4e53 0103 0000 005a 041e  LoginFNS.....Z..
-00008ca0: 0448 0438 0431 043a 0430 0020 043f 043e  .H.8.1.:.0. .?.>
-00008cb0: 043b 0443 0447 0435 043d 0438 044f 0020  .;.C.G.5.=.8.O. 
-00008cc0: 0055 0052 004c 0020 043b 043e 0433 0438  .U.R.L. .;.>.3.8
-00008cd0: 043d 0430 0020 0447 0435 0440 0435 0437  .=.0. .G.5.@.5.7
-00008ce0: 0020 0413 043e 0441 0443 0441 043b 0443  . ...>.A.C.A.;.C
-00008cf0: 0433 0438 003a 0020 0800 0000 0006 0000  .3.8.:. ........
-00008d00: 0015 4765 7420 4553 4941 2055 524c 2066  ..Get ESIA URL f
-00008d10: 6169 6c65 643a 2007 0000 0008 4c6f 6769  ailed: .....Logi
-00008d20: 6e46 4e53 0103 0000 0034 0053 004d 0053  nFNS.....4.S.M.S
-00008d30: 0020 0431 044b 043b 043e 0020 0437 0430  . .1.K.;.>. .7.0
-00008d40: 043f 0440 043e 0448 0435 043d 043e 0020  .?.@.>.H.5.=.>. 
-00008d50: 0443 0441 043f 0435 0448 043d 043e 0800  .C.A.?.5.H.=.>..
-00008d60: 0000 0006 0000 001e 534d 5320 7761 7320  ........SMS was 
-00008d70: 7265 7175 6573 7465 6420 7375 6363 6573  requested succes
-00008d80: 7366 756c 6c79 0700 0000 084c 6f67 696e  sfully.....Login
-00008d90: 464e 5301 0300 0000 1e04 1004 3204 4204  FNS.........2.B.
-00008da0: 3e04 4004 3804 3704 3004 4604 3804 4f00  >.@.8.7.0.F.8.O.
-00008db0: 2004 2404 1d04 2108 0000 0000 0600 0000   .$...!.........
-00008dc0: 1141 7574 686f 7269 7a61 7469 6f6e 2046  .Authorization F
-00008dd0: 4e53 0700 0000 0e4c 6f67 696e 464e 5344  NS.....LoginFNSD
-00008de0: 6961 6c6f 6701 0300 0000 0e04 1704 3004  ialog.........0.
-00008df0: 3a04 4004 4b04 4204 4c08 0000 0000 0600  :.@.K.B.L.......
-00008e00: 0000 0543 6c6f 7365 0700 0000 0e4c 6f67  ...Close.....Log
-00008e10: 696e 464e 5344 6961 6c6f 6701 0300 0000  inFNSDialog.....
-00008e20: 1604 1a04 3e04 3400 2004 3804 3700 2000  ....>.4. .8.7. .
-00008e30: 5300 4d00 5300 3a08 0000 0000 0600 0000  S.M.S.:.........
-00008e40: 0e43 6f64 6520 6672 6f6d 2053 4d53 3a07  .Code from SMS:.
-00008e50: 0000 000e 4c6f 6769 6e46 4e53 4469 616c  ....LoginFNSDial
-00008e60: 6f67 0103 0000 0012 0413 043e 0441 0443  og.........>.A.C
-00008e70: 0441 043b 0443 0433 0438 0800 0000 0006  .A.;.C.3.8......
-00008e80: 0000 000a 4553 4941 204c 6f67 696e 0700  ....ESIA Login..
-00008e90: 0000 0e4c 6f67 696e 464e 5344 6961 6c6f  ...LoginFNSDialo
-00008ea0: 6701 0300 0000 0c04 1b04 1a00 2004 2404  g........... .$.
-00008eb0: 1d04 2108 0000 0000 0600 0000 0946 4e53  ..!..........FNS
-00008ec0: 204c 6f67 696e 0700 0000 0e4c 6f67 696e   Login.....Login
-00008ed0: 464e 5344 6961 6c6f 6701 0300 0000 0804  FNSDialog.......
-00008ee0: 1804 1d04 1d00 3a08 0000 0000 0600 0000  ......:.........
-00008ef0: 0449 4e4e 3a07 0000 000e 4c6f 6769 6e46  .INN:.....LoginF
-00008f00: 4e53 4469 616c 6f67 0103 0000 000a 041b  NSDialog........
-00008f10: 043e 0433 0438 043d 0800 0000 0006 0000  .>.3.8.=........
-00008f20: 0005 4c6f 6769 6e07 0000 000e 4c6f 6769  ..Login.....Logi
-00008f30: 6e46 4e53 4469 616c 6f67 0103 0000 000e  nFNSDialog......
-00008f40: 041f 0430 0440 043e 043b 044c 003a 0800  ...0.@.>.;.L.:..
-00008f50: 0000 0006 0000 0009 5061 7373 776f 7264  ........Password
-00008f60: 3a07 0000 000e 4c6f 6769 6e46 4e53 4469  :.....LoginFNSDi
-00008f70: 616c 6f67 0103 0000 001e 041d 043e 043c  alog.........>.<
-00008f80: 0435 0440 0020 0442 0435 043b 0435 0444  .5.@. .B.5.;.5.D
-00008f90: 043e 043d 0430 003a 0800 0000 0006 0000  .>.=.0.:........
-00008fa0: 000d 5068 6f6e 6520 6e75 6d62 6572 3a07  ..Phone number:.
-00008fb0: 0000 000e 4c6f 6769 6e46 4e53 4469 616c  ....LoginFNSDial
-00008fc0: 6f67 0103 0000 0006 0053 004d 0053 0800  og.......S.M.S..
-00008fd0: 0000 0006 0000 0009 534d 5320 4c6f 6769  ........SMS Logi
-00008fe0: 6e07 0000 000e 4c6f 6769 6e46 4e53 4469  n.....LoginFNSDi
-00008ff0: 616c 6f67 0103 0000 0026 0412 044b 0441  alog.....&...K.A
-00009000: 043b 0430 0442 044c 0020 0053 004d 0053  .;.0.B.L. .S.M.S
-00009010: 0020 0441 0020 043a 043e 0434 043e 043c  . .A. .:.>.4.>.<
-00009020: 0800 0000 0006 0000 0012 5365 6e64 2053  ..........Send S
-00009030: 4d53 2077 6974 6820 636f 6465 0700 0000  MS with code....
-00009040: 0e4c 6f67 696e 464e 5344 6961 6c6f 6701  .LoginFNSDialog.
-00009050: 0300 0000 1600 6100 6200 6f00 7500 7400  ......a.b.o.u.t.
-00009060: 3a00 6200 6c00 6100 6e00 6b08 0000 0000  :.b.l.a.n.k.....
-00009070: 0600 0000 0b61 626f 7574 3a62 6c61 6e6b  .....about:blank
-00009080: 0700 0000 0e4c 6f67 696e 464e 5344 6961  .....LoginFNSDia
-00009090: 6c6f 6701 0300 0000 4404 1d04 3004 3904  log.....D...0.9.
-000090a0: 3404 3504 3d04 3e00 2004 3d04 3504 4104  4.5.=.>. .=.5.A.
-000090b0: 3a04 3e04 3b04 4c04 3a04 3e00 2004 2604  :.>.;.L.:.>. .&.
-000090c0: 1100 2004 3d04 3000 2000 4d00 4f00 4500  .. .=.0. .M.O.E.
-000090d0: 5800 2004 3404 3b04 4f00 3a00 2008 0000  X. .4.;.O.:. ...
-000090e0: 0000 0600 0000 204d 756c 7469 706c 6520  ...... Multiple 
-000090f0: 4d4f 4558 2061 7373 6574 7320 666f 756e  MOEX assets foun
-00009100: 6420 666f 723a 2007 0000 0004 4d4f 4558  d for: .....MOEX
-00009110: 0103 0000 0044 041d 0435 043f 043e 0434  .....D...5.?.>.4
-00009120: 0434 0435 0440 0436 0438 0432 0430 0435  .4.5.@.6.8.2.0.5
-00009130: 043c 044b 0439 0020 0442 0438 043f 0020  .<.K.9. .B.8.?. 
-00009140: 0426 0411 0020 041c 043e 0441 0411 0438  .&... ...>.A...8
-00009150: 0440 0436 0438 003a 0020 0800 0000 0006  .@.6.8.:. ......
-00009160: 0000 0020 556e 7375 7070 6f72 7465 6420  ... Unsupported 
-00009170: 4d4f 4558 2073 6563 7572 6974 7920 7479  MOEX security ty
-00009180: 7065 3a20 0700 0000 044d 4f45 5801 0300  pe: .....MOEX...
-00009190: 0000 1604 1e00 2004 3f04 4004 3e04 3304  ...... .?.@.>.3.
-000091a0: 4004 3004 3c04 3c04 3508 0000 0000 0600  @.0.<.<.5.......
-000091b0: 0000 0541 626f 7574 0700 0000 0a4d 6169  ...About.....Mai
-000091c0: 6e57 696e 646f 7701 0300 0000 1a04 1f04  nWindow.........
-000091d0: 3e04 3404 4204 3204 3504 4004 3604 3404  >.4.B.2.5.@.6.4.
-000091e0: 3504 3d04 3804 3508 0000 0000 0600 0000  5.=.8.5.........
-000091f0: 0c43 6f6e 6669 726d 6174 696f 6e07 0000  .Confirmation...
-00009200: 000a 4d61 696e 5769 6e64 6f77 0103 0000  ..MainWindow....
-00009210: 0014 0418 043d 0444 043e 0440 043c 0430  .....=.D.>.@.<.0
-00009220: 0446 0438 044f 0800 0000 0006 0000 0004  .F.8.O..........
-00009230: 496e 666f 0700 0000 0a4d 6169 6e57 696e  Info.....MainWin
-00009240: 646f 7701 0300 0000 2804 2f04 3704 4b04  dow.....(./.7.K.
-00009250: 3a00 2004 3104 4b04 3b00 2004 3804 3704  :. .1.K.;. .8.7.
-00009260: 3c04 3504 3d04 5104 3d00 2004 3d04 3000  <.5.=.Q.=. .=.0.
-00009270: 2008 0000 0000 0600 0000 184c 616e 6775   ..........Langu
-00009280: 6167 6520 7761 7320 6368 616e 6765 6420  age was changed 
-00009290: 746f 2007 0000 000a 4d61 696e 5769 6e64  to .....MainWind
-000092a0: 6f77 0103 0000 0062 0418 0442 043e 0433  ow.....b...B.>.3
-000092b0: 0438 0020 0442 0440 0430 043d 0437 0430  .8. .B.@.0.=.7.0
-000092c0: 043a 0446 0438 0439 0020 043d 0435 0430  .:.F.8.9. .=.5.0
-000092d0: 043a 0442 0443 0430 043b 044c 043d 044b  .:.B.C.0.;.L.=.K
-000092e0: 002e 0020 041f 0435 0440 0435 0441 0447  ... ...5.@.5.A.G
-000092f0: 0438 0442 0430 0442 044c 0020 0441 0435  .8.B.0.B.L. .A.5
-00009300: 0439 0447 0430 0441 003f 0800 0000 0006  .9.G.0.A.?......
-00009310: 0000 0026 4c65 6467 6572 2069 736e 2774  ...&Ledger isn't
-00009320: 2063 6f6d 706c 6574 652e 2052 6562 7569   complete. Rebui
-00009330: 6c64 2069 7420 6e6f 773f 0700 0000 0a4d  ld it now?.....M
-00009340: 6169 6e57 696e 646f 7701 0300 0000 8004  ainWindow.......
-00009350: 1404 3e04 3f04 3e04 3b04 3d04 3804 4204  ..>.?.>.;.=.8.B.
-00009360: 3504 3b04 4c04 3d04 3004 4f00 2004 3804  5.;.L.=.0.O. .8.
-00009370: 3d04 4404 3e04 4004 3c04 3004 4604 3804  =.D.>.@.<.0.F.8.
-00009380: 4f00 2c00 2004 3804 3d04 4104 4204 4004  O.,. .8.=.A.B.@.
-00009390: 4304 3a04 4604 3804 3800 2c00 2004 4104  C.:.F.8.8.,. .A.
-000093a0: 3e04 3e04 3104 4904 3504 3d04 3804 4f00  >.>.1.I.5.=.8.O.
-000093b0: 2004 3e00 2004 3f04 4004 3e04 3104 3b04   .>. .?.@.>.1.;.
-000093c0: 3504 3c04 3004 4500 2004 3d04 3000 2008  5.<.0.E. .=.0. .
-000093d0: 0000 0000 0600 0000 354d 6f72 6520 696e  ........5More in
-000093e0: 666f 726d 6174 696f 6e2c 206d 616e 7561  formation, manua
-000093f0: 6c73 2061 6e64 2070 726f 626c 656d 2072  ls and problem r
-00009400: 6570 6f72 7473 2061 7265 2061 7420 0700  eports are at ..
-00009410: 0000 0a4d 6169 6e57 696e 646f 7701 0300  ...MainWindow...
-00009420: 0000 5004 1204 3e04 3f04 4004 3e04 4104  ..P...>.?.@.>.A.
-00009430: 4b00 2c00 2004 3a04 3e04 3c04 3c04 3504  K.,. .:.>.<.<.5.
-00009440: 3d04 4204 3004 4004 3804 3800 2c00 2004  =.B.0.@.8.8.,. .
-00009450: 3f04 3e04 3c04 3e04 4904 4c00 2004 3804  ?.>.<.>.I.L. .8.
-00009460: 3b04 3800 2004 3404 3e04 3d04 3004 4204  ;.8. .4.>.=.0.B.
-00009470: 4b00 3a08 0000 0000 0600 0000 2751 7565  K.:.........'Que
-00009480: 7374 696f 6e73 2c20 636f 6d6d 656e 7473  stions, comments
-00009490: 2c20 6865 6c70 206f 7220 646f 6e61 7469  , help or donati
-000094a0: 6f6e 733a 0700 0000 0a4d 6169 6e57 696e  ons:.....MainWin
-000094b0: 646f 7701 0300 0000 2204 2204 4004 3504  dow.....".".@.5.
-000094c0: 3104 4304 3504 4204 4104 4f00 2004 4004  1.C.5.B.A.O. .@.
-000094d0: 3504 4104 4204 3004 4004 4208 0000 0000  5.A.B.0.@.B.....
-000094e0: 0600 0000 1052 6573 7461 7274 2072 6571  .....Restart req
-000094f0: 7569 7265 6407 0000 000a 4d61 696e 5769  uired.....MainWi
-00009500: 6e64 6f77 0103 0000 0050 041a 043e 043d  ndow.....P...>.=
-00009510: 0435 0447 043d 044b 0439 0020 0431 0430  .5.G.=.K.9. .1.0
-00009520: 043b 0430 043d 0441 0020 043f 043e 0020  .;.0.=.A. .?.>. 
-00009530: 043e 0442 0447 0451 0442 0443 0020 043d  .>.B.G.Q.B.C. .=
-00009540: 0435 0020 0441 043e 0432 043f 0430 0434  .5. .A.>.2.?.0.4
-00009550: 0430 0435 0442 003a 0020 0800 0000 0006  .0.5.B.:. ......
-00009560: 0000 0028 5374 6174 656d 656e 7420 656e  ...(Statement en
-00009570: 6469 6e67 2062 616c 616e 6365 2064 6f65  ding balance doe
-00009580: 736e 2774 206d 6174 6368 3a20 0700 0000  sn't match: ....
-00009590: 0a4d 6169 6e57 696e 646f 7701 0300 0000  .MainWindow.....
-000095a0: c804 1204 4b00 2004 3404 3e04 3b04 3604  ....K. .4.>.;.6.
-000095b0: 3d04 4b00 2004 3f04 3504 4004 3504 3704  =.K. .?.5.@.5.7.
-000095c0: 3004 3f04 4304 4104 4204 3804 4204 4c00  0.?.C.A.B.8.B.L.
-000095d0: 2004 3f04 4004 3804 3b04 3e04 3604 3504   .?.@.8.;.>.6.5.
-000095e0: 3d04 3804 3500 2c00 2004 4704 4204 3e04  =.8.5.,. .G.B.>.
-000095f0: 3104 4b00 2004 3f04 4004 3804 3c04 3504  1.K. .?.@.8.<.5.
-00009600: 3d04 3804 4204 4c00 2004 3804 3704 3c04  =.8.B.L. .8.7.<.
-00009610: 3504 3d04 3504 3d04 3804 4f00 0a04 1f04  5.=.5.=.8.O.....
-00009620: 4004 3804 3b04 3e04 3604 3504 3d04 3804  @.8.;.>.6.5.=.8.
-00009630: 3500 2004 4104 3504 3904 4704 3004 4100  5. .A.5.9.G.0.A.
-00009640: 2004 3704 3004 3204 3504 4004 4804 3804   .7.0.2.5.@.H.8.
-00009650: 4200 2004 4104 3204 3e04 4e00 2004 4004  B. .A.2.>.N. .@.
-00009660: 3004 3104 3e04 4204 4308 0000 0000 0600  0.1.>.B.C.......
-00009670: 0000 5259 6f75 2073 686f 756c 6420 7265  ..RYou should re
-00009680: 7374 6172 7420 6170 706c 6963 6174 696f  start applicatio
-00009690: 6e20 746f 2061 7070 6c79 2063 6861 6e67  n to apply chang
-000096a0: 6573 0a41 7070 6c69 6361 7469 6f6e 2077  es.Application w
-000096b0: 696c 6c20 6265 2074 6572 6d69 6e61 7465  ill be terminate
-000096c0: 6420 6e6f 7707 0000 000a 4d61 696e 5769  d now.....MainWi
-000096d0: 6e64 6f77 0103 0000 0030 0434 043e 043c  ndow.....0.4.>.<
-000096e0: 0430 0448 043d 0435 0439 0020 0441 0442  .0.H.=.5.9. .A.B
-000096f0: 0440 0430 043d 0438 0446 0435 0020 0067  .@.0.=.8.F.5. .g
-00009700: 0069 0074 0068 0075 0062 0800 0000 0006  .i.t.h.u.b......
-00009710: 0000 0010 6769 7468 7562 2068 6f6d 6520  ....github home 
-00009720: 7061 6765 0700 0000 0a4d 6169 6e57 696e  page.....MainWin
-00009730: 646f 7701 0300 0000 0c04 3204 3504 4004  dow.......2.5.@.
-00009740: 4104 3804 4f08 0000 0000 0600 0000 0776  A.8.O..........v
-00009750: 6572 7369 6f6e 0700 0000 0a4d 6169 6e57  ersion.....MainW
-00009760: 696e 646f 7701 0300 0000 0600 2e00 2e00  indow...........
-00009770: 2e08 0000 0000 0600 0000 032e 2e2e 0700  ................
-00009780: 0000 0f4d 6f6e 6579 466c 6f77 5769 6467  ...MoneyFlowWidg
-00009790: 6574 0103 0000 0016 0424 0430 0439 043b  et.......$.0.9.;
-000097a0: 0020 0045 0078 0063 0065 006c 003a 0800  . .E.x.c.e.l.:..
-000097b0: 0000 0006 0000 000b 4578 6365 6c20 6669  ........Excel fi
-000097c0: 6c65 3a07 0000 000f 4d6f 6e65 7946 6c6f  le:.....MoneyFlo
-000097d0: 7757 6964 6765 7401 0300 0000 2804 2404  wWidget.....(.$.
-000097e0: 3004 3904 3b04 4b00 2000 4500 7800 6300  0.9.;.K. .E.x.c.
-000097f0: 6500 6c00 2000 2800 2a00 2e00 7800 7300  e.l. .(.*...x.s.
-00009800: 6c00 7800 2908 0000 0000 0600 0000 1445  l.x.)..........E
-00009810: 7863 656c 2066 696c 6573 2028 2a2e 786c  xcel files (*.xl
-00009820: 7378 2907 0000 000f 4d6f 6e65 7946 6c6f  sx).....MoneyFlo
-00009830: 7757 6964 6765 7401 0300 0000 5604 2404  wWidget.....V.$.
-00009840: 3004 3904 3b00 2004 3404 3b04 4f00 2004  0.9.;. .4.;.O. .
-00009850: 4104 3e04 4504 4004 3004 3d04 3504 3d04  A.>.E.@.0.=.5.=.
-00009860: 3804 4f00 2004 4004 3004 4104 4704 5104  8.O. .@.0.A.G.Q.
-00009870: 4204 3000 2004 3200 2004 4404 3e04 4004  B.0. .2. .D.>.@.
-00009880: 3c04 3004 4204 3500 2000 4500 7800 6300  <.0.B.5. .E.x.c.
-00009890: 6500 6c08 0000 0000 0600 0000 2e46 696c  e.l..........Fil
-000098a0: 6520 7768 6572 6520 746f 2073 746f 7265  e where to store
-000098b0: 2074 6178 2072 6570 6f72 7420 696e 2045   tax report in E
-000098c0: 7863 656c 2066 6f72 6d61 7407 0000 000f  xcel format.....
-000098d0: 4d6f 6e65 7946 6c6f 7757 6964 6765 7401  MoneyFlowWidget.
-000098e0: 0300 0000 0a04 1e04 3e04 1404 1404 2108  ........>.....!.
-000098f0: 0000 0000 0600 0000 0a4d 6f6e 6579 2046  .........Money F
-00009900: 6c6f 7707 0000 000f 4d6f 6e65 7946 6c6f  low.....MoneyFlo
-00009910: 7757 6964 6765 7401 0300 0000 2e04 1e04  wWidget.........
-00009920: 3e04 1404 1404 2100 2004 4104 3e04 4504  >.....!. .A.>.E.
-00009930: 4004 3004 3d04 5104 3d00 2004 3200 2004  @.0.=.Q.=. .2. .
-00009940: 4404 3004 3904 3b04 3500 2008 0000 0000  D.0.9.;.5. .....
-00009950: 0600 0000 204d 6f6e 6579 2066 6c6f 7720  .... Money flow 
-00009960: 7265 706f 7274 2073 6176 6564 2074 6f20  report saved to 
-00009970: 6669 6c65 2007 0000 000f 4d6f 6e65 7946  file .....MoneyF
-00009980: 6c6f 7757 6964 6765 7401 0300 0000 1e04  lowWidget.......
-00009990: 2104 3e04 4504 4004 3004 3d04 3804 4204  !.>.E.@.0.=.8.B.
-000099a0: 4c00 2004 1e04 4204 4704 5104 4208 0000  L. ...B.G.Q.B...
-000099b0: 0000 0600 0000 0b53 6176 6520 5265 706f  .......Save Repo
-000099c0: 7274 0700 0000 0f4d 6f6e 6579 466c 6f77  rt.....MoneyFlow
-000099d0: 5769 6467 6574 0103 0000 0024 0421 043e  Widget.....$.!.>
-000099e0: 0445 0440 0430 043d 0438 0442 044c 0020  .E.@.0.=.8.B.L. 
-000099f0: 041e 043e 0414 0414 0421 0020 0432 003a  ...>.....!. .2.:
-00009a00: 0800 0000 0006 0000 001a 5361 7665 206d  ..........Save m
-00009a10: 6f6e 6579 2066 6c6f 7720 7265 706f 7274  oney flow report
-00009a20: 2074 6f3a 0700 0000 0f4d 6f6e 6579 466c   to:.....MoneyFl
-00009a30: 6f77 5769 6467 6574 0103 0000 0018 0412  owWidget........
-00009a40: 044b 0431 0435 0440 0438 0442 0020 0444  .K.1.5.@.8.B. .D
-00009a50: 0430 0439 043b 0800 0000 0006 0000 000b  .0.9.;..........
-00009a60: 5365 6c65 6374 2066 696c 6507 0000 000f  Select file.....
-00009a70: 4d6f 6e65 7946 6c6f 7757 6964 6765 7401  MoneyFlowWidget.
-00009a80: 0300 0000 0804 1304 3e04 3400 3a08 0000  ........>.4.:...
-00009a90: 0000 0600 0000 0559 6561 723a 0700 0000  .......Year:....
-00009aa0: 0f4d 6f6e 6579 466c 6f77 5769 6467 6574  .MoneyFlowWidget
-00009ab0: 0103 0000 0028 0020 043d 0435 0443 0441  .....(. .=.5.C.A
-00009ac0: 043f 0435 0448 043d 044b 0439 0020 0437  .?.5.H.=.K.9. .7
-00009ad0: 0430 043f 0440 043e 0441 003a 0020 0800  .0.?.@.>.A.:. ..
-00009ae0: 0000 0006 0000 0009 2066 6169 6c65 643a  ........ failed:
-00009af0: 2007 0000 0003 4e65 7401 0300 0000 3404   .....Net.....4.
-00009b00: 2204 3804 3f00 2004 2604 1100 2004 3d04  ".8.?. .&... .=.
-00009b10: 3500 2004 3f04 3e04 3404 3404 3504 4004  5. .?.>.4.4.5.@.
-00009b20: 3604 3804 3204 3004 3504 4204 4104 4f00  6.8.2.0.5.B.A.O.
-00009b30: 3a00 2008 0000 0000 0600 0000 1c41 7373  :. ..........Ass
-00009b40: 6574 2074 7970 6520 6973 6e27 7420 7375  et type isn't su
-00009b50: 7070 6f72 7465 643a 2007 0000 000a 4f70  pported: .....Op
-00009b60: 656e 4272 6f6b 6572 0103 0000 0032 0411  enBroker.....2..
-00009b70: 0438 0440 0436 0430 0020 043d 0435 0020  .8.@.6.0. .=.5. 
-00009b80: 043f 043e 0434 0434 0435 0440 0436 0438  .?.>.4.4.5.@.6.8
-00009b90: 0432 0430 0435 0442 0441 044f 003a 0020  .2.0.5.B.A.O.:. 
-00009ba0: 0800 0000 0006 0000 001a 4578 6368 616e  ..........Exchan
-00009bb0: 6765 2069 736e 2774 2073 7570 706f 7274  ge isn't support
-00009bc0: 6564 3a20 0700 0000 0a4f 7065 6e42 726f  ed: .....OpenBro
-00009bd0: 6b65 7201 0300 0000 0804 2104 4704 3504  ker.......!.G.5.
-00009be0: 4208 0000 0000 0600 0000 0741 6363 6f75  B..........Accou
-00009bf0: 6e74 0700 0000 0f4f 7065 7261 7469 6f6e  nt.....Operation
-00009c00: 734d 6f64 656c 0103 0000 000a 0421 0443  sModel.......!.C
-00009c10: 043c 043c 0430 0800 0000 0006 0000 0006  .<.<.0..........
-00009c20: 416d 6f75 6e74 0700 0000 0f4f 7065 7261  Amount.....Opera
-00009c30: 7469 6f6e 734d 6f64 656c 0103 0000 000c  tionsModel......
-00009c40: 0411 0430 043b 0430 043d 0441 0800 0000  ...0.;.0.=.A....
-00009c50: 0006 0000 0007 4261 6c61 6e63 6507 0000  ......Balance...
-00009c60: 000f 4f70 6572 6174 696f 6e73 4d6f 6465  ..OperationsMode
-00009c70: 6c01 0300 0000 0c04 1204 3004 3b04 4e04  l.........0.;.N.
-00009c80: 4204 3008 0000 0000 0600 0000 0843 7572  B.0..........Cur
-00009c90: 7265 6e63 7907 0000 000f 4f70 6572 6174  rency.....Operat
-00009ca0: 696f 6e73 4d6f 6465 6c01 0300 0000 1004  ionsModel.......
-00009cb0: 1e04 3f04 3804 4104 3004 3d04 3804 3508  ..?.8.A.0.=.8.5.
-00009cc0: 0000 0000 0600 0000 054e 6f74 6573 0700  .........Notes..
-00009cd0: 0000 0f4f 7065 7261 7469 6f6e 734d 6f64  ...OperationsMod
-00009ce0: 656c 0103 0000 0014 0414 0430 0442 0430  el.........0.B.0
-00009cf0: 002f 0412 0440 0435 043c 044f 0800 0000  ./...@.5.<.O....
-00009d00: 0006 0000 0009 5469 6d65 7374 616d 7007  ......Timestamp.
-00009d10: 0000 000f 4f70 6572 6174 696f 6e73 4d6f  ....OperationsMo
-00009d20: 6465 6c01 0300 0000 0a04 2104 4704 3504  del.......!.G.5.
-00009d30: 4200 3a08 0000 0000 0600 0000 0841 6363  B.:..........Acc
-00009d40: 6f75 6e74 3a07 0000 0010 4f70 6572 6174  ount:.....Operat
-00009d50: 696f 6e73 5769 6467 6574 0103 0000 004a  ionsWidget.....J
-00009d60: 0412 044b 0020 0445 043e 0442 0438 0442  ...K. .E.>.B.8.B
-00009d70: 0435 0020 0443 0434 0430 043b 0438 0442  .5. .C.4.0.;.8.B
-00009d80: 044c 0020 0432 044b 0431 0440 0430 043d  .L. .2.K.1.@.0.=
-00009d90: 043d 044b 0435 0020 043e 043f 0435 0440  .=.K.5. .>.?.5.@
-00009da0: 0430 0446 0438 0438 003f 0800 0000 0006  .0.F.8.8.?......
-00009db0: 0000 002e 4172 6520 796f 7520 7375 7265  ....Are you sure
-00009dc0: 2074 6f20 6465 6c65 7465 2073 656c 6563   to delete selec
-00009dd0: 7465 6420 7472 616e 7361 6369 6f6e 2873  ted transacion(s
-00009de0: 293f 0700 0000 104f 7065 7261 7469 6f6e  )?.....Operation
-00009df0: 7357 6964 6765 7401 0300 0000 1c04 1104  sWidget.........
-00009e00: 3004 3b04 3004 3d04 4104 4b00 2004 4104  0.;.0.=.A.K. .A.
-00009e10: 4704 3504 4204 3e04 3208 0000 0000 0600  G.5.B.>.2.......
-00009e20: 0000 0842 616c 616e 6365 7307 0000 0010  ...Balances.....
-00009e30: 4f70 6572 6174 696f 6e73 5769 6467 6574  OperationsWidget
-00009e40: 0103 0000 001a 041f 043e 0434 0442 0432  .........>.4.B.2
-00009e50: 0435 0440 0436 0434 0435 043d 0438 0435  .5.@.6.4.5.=.8.5
-00009e60: 0800 0000 0006 0000 000c 436f 6e66 6972  ..........Confir
-00009e70: 6d61 7469 6f6e 0700 0000 104f 7065 7261  mation.....Opera
-00009e80: 7469 6f6e 7357 6964 6765 7401 0300 0000  tionsWidget.....
-00009e90: 1404 1a04 3e04 3f04 3804 4004 3e04 3204  ....>.?.8.@.>.2.
-00009ea0: 3004 4204 4c08 0000 0000 0600 0000 0443  0.B.L..........C
-00009eb0: 6f70 7907 0000 0010 4f70 6572 6174 696f  opy.....Operatio
-00009ec0: 6e73 5769 6467 6574 0103 0000 0026 041a  nsWidget.....&..
-00009ed0: 043e 043f 0438 0440 043e 0432 0430 0442  .>.?.8.@.>.2.0.B
-00009ee0: 044c 0020 043e 043f 0435 0440 0430 0446  .L. .>.?.5.@.0.F
-00009ef0: 0438 044e 0800 0000 0006 0000 000e 436f  .8.N..........Co
-00009f00: 7079 206f 7065 7261 7469 6f6e 0700 0000  py operation....
-00009f10: 104f 7065 7261 7469 6f6e 7357 6964 6765  .OperationsWidge
-00009f20: 7401 0300 0000 0e04 2304 3404 3004 3b04  t.......#.4.0.;.
-00009f30: 3804 4204 4c08 0000 0000 0600 0000 0644  8.B.L..........D
-00009f40: 656c 6574 6507 0000 0010 4f70 6572 6174  elete.....Operat
-00009f50: 696f 6e73 5769 6467 6574 0103 0000 0020  ionsWidget..... 
-00009f60: 0423 0434 0430 043b 0438 0442 044c 0020  .#.4.0.;.8.B.L. 
-00009f70: 043e 043f 0435 0440 0430 0446 0438 044e  .>.?.5.@.0.F.8.N
-00009f80: 0800 0000 0006 0000 0010 4465 6c65 7465  ..........Delete
-00009f90: 206f 7065 7261 7469 6f6e 0700 0000 104f   operation.....O
-00009fa0: 7065 7261 7469 6f6e 7357 6964 6765 7401  perationsWidget.
-00009fb0: 0300 0000 1c04 1d04 3e04 3204 3004 4f00  ........>.2.0.O.
-00009fc0: 2004 3e04 3f04 3504 4004 3004 4604 3804   .>.?.5.@.0.F.8.
-00009fd0: 4f08 0000 0000 0600 0000 0d4e 6577 206f  O..........New o
-00009fe0: 7065 7261 7469 6f6e 0700 0000 104f 7065  peration.....Ope
-00009ff0: 7261 7469 6f6e 7357 6964 6765 7401 0300  rationsWidget...
-0000a000: 0000 1004 1e04 3f04 3504 4004 3004 4604  ......?.5.@.0.F.
-0000a010: 3804 3808 0000 0000 0600 0000 0a4f 7065  8.8..........Ope
-0000a020: 7261 7469 6f6e 7307 0000 0010 4f70 6572  rations.....Oper
-0000a030: 6174 696f 6e73 5769 6467 6574 0103 0000  ationsWidget....
-0000a040: 0024 041e 043f 0435 0440 0430 0446 0438  .$...?.5.@.0.F.8
-0000a050: 0438 0020 0438 0020 0411 0430 043b 0430  .8. .8. ...0.;.0
-0000a060: 043d 0441 044b 0800 0000 0006 0000 0015  .=.A.K..........
-0000a070: 4f70 6572 6174 696f 6e73 2026 2042 616c  Operations & Bal
-0000a080: 616e 6365 7307 0000 0010 4f70 6572 6174  ances.....Operat
-0000a090: 696f 6e73 5769 6467 6574 0103 0000 000e  ionsWidget......
-0000a0a0: 0421 0432 0435 0440 0438 0442 044c 0800  .!.2.5.@.8.B.L..
-0000a0b0: 0000 0006 0000 0009 5265 636f 6e63 696c  ........Reconcil
-0000a0c0: 6507 0000 0010 4f70 6572 6174 696f 6e73  e.....Operations
-0000a0d0: 5769 6467 6574 0103 0000 000c 041f 043e  Widget.........>
-0000a0e0: 0438 0441 043a 003a 0800 0000 0006 0000  .8.A.:.:........
-0000a0f0: 0007 5365 6172 6368 3a07 0000 0010 4f70  ..Search:.....Op
-0000a100: 6572 6174 696f 6e73 5769 6467 6574 0103  erationsWidget..
-0000a110: 0000 002c 041f 043e 043a 0430 0437 044b  ...,...>.:.0.7.K
-0000a120: 0432 0430 0442 044c 0020 0026 043d 0435  .2.0.B.L. .&.=.5
-0000a130: 0430 043a 0442 0438 0432 043d 044b 0435  .0.:.B.8.2.=.K.5
-0000a140: 0800 0000 0006 0000 000e 5368 6f77 2026  ..........Show &
-0000a150: 496e 6163 7469 7665 0700 0000 104f 7065  Inactive.....Ope
-0000a160: 7261 7469 6f6e 7357 6964 6765 7401 0300  rationsWidget...
-0000a170: 0000 1a04 1204 3004 3b04 4e04 4204 3000  ......0.;.N.B.0.
-0000a180: 2004 3804 4204 3e04 3304 3e00 3a08 0000   .8.B.>.3.>.:...
-0000a190: 0000 0600 0000 0d53 756d 2043 7572 7265  .......Sum Curre
-0000a1a0: 6e63 793a 0700 0000 104f 7065 7261 7469  ncy:.....Operati
-0000a1b0: 6f6e 7357 6964 6765 7401 0300 0000 1400  onsWidget.......
-0000a1c0: 6400 6400 2f00 4d00 4d00 2f00 7900 7900  d.d./.M.M./.y.y.
-0000a1d0: 7900 7908 0000 0000 0600 0000 0a64 642f  y.y..........dd/
-0000a1e0: 4d4d 2f79 7979 7907 0000 0010 4f70 6572  MM/yyyy.....Oper
-0000a1f0: 6174 696f 6e73 5769 6467 6574 0103 0000  ationsWidget....
-0000a200: 000c 0412 0430 043b 044e 0442 0430 0800  .....0.;.N.B.0..
-0000a210: 0000 0006 0000 0008 4375 7272 656e 6379  ........Currency
-0000a220: 0700 0000 184f 7074 696f 6e61 6c43 7572  .....OptionalCur
-0000a230: 7265 6e63 7943 6f6d 626f 426f 7801 0300  rencyComboBox...
-0000a240: 0000 0a04 2104 4304 3c04 3c04 3008 0000  ....!.C.<.<.0...
-0000a250: 0000 0600 0000 0641 6d6f 756e 7407 0000  .......Amount...
-0000a260: 0010 5061 6e64 6173 4c69 6e65 734d 6f64  ..PandasLinesMod
-0000a270: 656c 0103 0000 0012 041a 0430 0442 0435  el.........0.B.5
-0000a280: 0433 043e 0440 0438 044f 0800 0000 0006  .3.>.@.8.O......
-0000a290: 0000 0008 4361 7465 676f 7279 0700 0000  ....Category....
-0000a2a0: 1050 616e 6461 734c 696e 6573 4d6f 6465  .PandasLinesMode
-0000a2b0: 6c01 0300 0000 2204 1d04 3004 3704 3204  l....."...0.7.2.
-0000a2c0: 3004 3d04 3804 3500 2004 3f04 4004 3e04  0.=.8.5. .?.@.>.
-0000a2d0: 3404 4304 3a04 4204 3008 0000 0000 0600  4.C.:.B.0.......
-0000a2e0: 0000 0c50 726f 6475 6374 206e 616d 6507  ...Product name.
-0000a2f0: 0000 0010 5061 6e64 6173 4c69 6e65 734d  ....PandasLinesM
-0000a300: 6f64 656c 0103 0000 0006 0422 044d 0433  odel.......".M.3
-0000a310: 0800 0000 0006 0000 0003 5461 6707 0000  ..........Tag...
-0000a320: 0010 5061 6e64 6173 4c69 6e65 734d 6f64  ..PandasLinesMod
-0000a330: 656c 0103 0000 0024 0027 0020 0437 0430  el.....$.'. .7.0
-0000a340: 043c 0435 043d 0435 043d 0430 0020 0443  .<.5.=.5.=.0. .C
-0000a350: 0441 043f 0435 0448 043d 043e 0800 0000  .A.?.5.H.=.>....
-0000a360: 0006 0000 001b 2720 7761 7320 7375 6363  ......' was succ
-0000a370: 6573 7366 756c 6c79 2072 6570 6c61 6365  essfully replace
-0000a380: 6407 0000 000e 5065 6572 4c69 7374 4469  d.....PeerListDi
-0000a390: 616c 6f67 0103 0000 000c 0027 0020 043d  alog.......'. .=
-0000a3a0: 0430 003a 0020 0800 0000 0006 0000 0008  .0.:. ..........
-0000a3b0: 2720 7769 7468 3a20 0700 0000 0e50 6565  ' with: .....Pee
-0000a3c0: 724c 6973 7444 6961 6c6f 6701 0300 0000  rListDialog.....
-0000a3d0: 4e04 2104 3e04 4504 4004 3004 3d04 3804  N.!.>.E.@.0.=.8.
-0000a3e0: 4204 4c00 2004 4104 4204 3004 4004 3e04  B.L. .A.B.0.@.>.
-0000a3f0: 3500 2004 3d04 3004 3704 3204 3004 3d04  5. .=.0.7.2.0.=.
-0000a400: 3804 3500 2004 3200 2004 3f04 4004 3804  8.5. .2. .?.@.8.
-0000a410: 3c04 3504 4704 3004 3d04 3804 3800 3f08  <.5.G.0.=.8.8.?.
-0000a420: 0000 0000 0600 0000 174b 6565 7020 6f6c  .........Keep ol
-0000a430: 6420 6e61 6d65 2069 6e20 6e6f 7465 733f  d name in notes?
-0000a440: 0700 0000 0e50 6565 724c 6973 7444 6961  .....PeerListDia
-0000a450: 6c6f 6701 0300 0000 1804 1a04 3e04 3d04  log.........>.=.
-0000a460: 4204 4004 3004 3304 3504 3d04 4200 2000  B.@.0.3.5.=.B. .
-0000a470: 2708 0000 0000 0600 0000 0650 6565 7220  '..........Peer 
-0000a480: 2707 0000 000e 5065 6572 4c69 7374 4469  '.....PeerListDi
-0000a490: 616c 6f67 0103 0000 0016 041a 043e 043d  alog.........>.=
-0000a4a0: 0442 0440 0430 0433 0435 043d 0442 044b  .B.@.0.3.5.=.B.K
-0000a4b0: 0800 0000 0006 0000 0005 5065 6572 7307  ..........Peers.
-0000a4c0: 0000 000e 5065 6572 4c69 7374 4469 616c  ....PeerListDial
-0000a4d0: 6f67 0103 0000 002c 0417 0430 043c 0435  og.....,...0.<.5
-0000a4e0: 043d 0438 0442 044c 0020 043a 043e 043d  .=.8.B.L. .:.>.=
-0000a4f0: 0442 0440 0430 0433 0435 043d 0442 0430  .B.@.0.3.5.=.B.0
-0000a500: 0020 0027 0800 0000 0006 0000 000e 5265  . .'..........Re
-0000a510: 706c 6163 6520 7065 6572 2027 0700 0000  place peer '....
-0000a520: 0e50 6565 724c 6973 7444 6961 6c6f 6701  .PeerListDialog.
-0000a530: 0300 0000 1c04 1704 3004 3c04 3504 3d04  ........0.<.5.=.
-0000a540: 3804 4204 4c00 2004 3d04 3000 2e00 2e00  8.B.L. .=.0.....
-0000a550: 2e08 0000 0000 0600 0000 0f52 6570 6c61  ...........Repla
-0000a560: 6365 2077 6974 682e 2e2e 0700 0000 0e50  ce with........P
-0000a570: 6565 724c 6973 7444 6961 6c6f 6701 0300  eerListDialog...
-0000a580: 0000 4004 1f04 3e04 3a04 3004 3704 3004  ..@...>.:.0.7.0.
-0000a590: 4204 4c00 2004 3e04 3f04 3504 4004 3004  B.L. .>.?.5.@.0.
-0000a5a0: 4604 3804 3800 2004 4100 2004 1a04 3e04  F.8.8. .A. ...>.
-0000a5b0: 3d04 4204 4004 3004 3304 3504 3d04 4204  =.B.@.0.3.5.=.B.
-0000a5c0: 3e04 3c08 0000 0000 0600 0000 1953 686f  >.<..........Sho
-0000a5d0: 7720 6f70 6572 6174 696f 6e73 2077 6974  w operations wit
-0000a5e0: 6820 5065 6572 0700 0000 0e50 6565 724c  h Peer.....PeerL
-0000a5f0: 6973 7444 6961 6c6f 6701 0300 0000 1004  istDialog.......
-0000a600: 1e04 3f04 3504 4004 3004 4604 3804 3808  ..?.5.@.0.F.8.8.
-0000a610: 0000 0000 0600 0000 0a4f 7065 7261 7469  .........Operati
-0000a620: 6f6e 7307 0000 000a 5065 6572 5265 706f  ons.....PeerRepo
-0000a630: 7274 0103 0000 001c 043f 043e 0020 041a  rt.......?.>. ..
-0000a640: 043e 043d 0442 0440 0430 0433 0435 043d  .>.=.B.@.0.3.5.=
-0000a650: 0442 0443 0800 0000 0006 0000 0007 6279  .B.C..........by
-0000a660: 2050 6565 7207 0000 000a 5065 6572 5265   Peer.....PeerRe
-0000a670: 706f 7274 0103 0000 0016 041a 043e 043d  port.........>.=
-0000a680: 0442 0440 0430 0433 0435 043d 0442 003a  .B.@.0.3.5.=.B.:
-0000a690: 0800 0000 0006 0000 0005 5065 6572 3a07  ..........Peer:.
-0000a6a0: 0000 0010 5065 6572 5265 706f 7274 5769  ....PeerReportWi
-0000a6b0: 6467 6574 0103 0000 0028 041e 0442 0447  dget.....(...B.G
-0000a6c0: 0435 0442 0020 043f 043e 0020 043a 043e  .5.B. .?.>. .:.>
-0000a6d0: 043d 0442 0440 0430 0433 0435 043d 0442  .=.B.@.0.3.5.=.B
-0000a6e0: 0443 0800 0000 0006 0000 000e 5265 706f  .C..........Repo
-0000a6f0: 7274 2062 7920 7065 6572 0700 0000 1050  rt by peer.....P
-0000a700: 6565 7252 6570 6f72 7457 6964 6765 7401  eerReportWidget.
-0000a710: 0300 0000 1604 1a04 3e04 3b00 2d04 3204  ........>.;.-.2.
-0000a720: 3e00 2004 3404 3e04 3a00 2e08 0000 0000  >. .4.>.:.......
-0000a730: 0600 0000 0a44 6f63 7320 636f 756e 7407  .....Docs count.
-0000a740: 0000 000d 5065 6572 5472 6565 4d6f 6465  ....PeerTreeMode
-0000a750: 6c01 0300 0000 0a04 1004 3404 4004 3504  l.........4.@.5.
-0000a760: 4108 0000 0000 0600 0000 084c 6f63 6174  A..........Locat
-0000a770: 696f 6e07 0000 000d 5065 6572 5472 6565  ion.....PeerTree
-0000a780: 4d6f 6465 6c01 0300 0000 1804 1d04 3004  Model.........0.
-0000a790: 3804 3c04 3504 3d04 3e04 3204 3004 3d04  8.<.5.=.>.2.0.=.
-0000a7a0: 3804 3508 0000 0000 0600 0000 044e 616d  8.5..........Nam
-0000a7b0: 6507 0000 000d 5065 6572 5472 6565 4d6f  e.....PeerTreeMo
-0000a7c0: 6465 6c01 0300 0000 1a04 2104 4704 3504  del.......!.G.5.
-0000a7d0: 4204 3000 2004 3200 2004 3104 3004 3d04  B.0. .2. .1.0.=.
-0000a7e0: 3a04 3508 0000 0000 0600 0000 0d42 616e  :.5..........Ban
-0000a7f0: 6b20 6163 636f 756e 7473 0700 0000 1650  k accounts.....P
-0000a800: 7265 6465 6669 6e64 6564 4163 636f 756e  redefindedAccoun
-0000a810: 7454 7970 6501 0300 0000 0a04 1a04 3004  tType.........0.
-0000a820: 4004 4204 4b08 0000 0000 0600 0000 0543  @.B.K..........C
-0000a830: 6172 6473 0700 0000 1650 7265 6465 6669  ards.....Predefi
-0000a840: 6e64 6564 4163 636f 756e 7454 7970 6501  ndedAccountType.
-0000a850: 0300 0000 1004 1d04 3004 3b04 3804 4704  ........0.;.8.G.
-0000a860: 3d04 4b04 3508 0000 0000 0600 0000 0443  =.K.5..........C
-0000a870: 6173 6807 0000 0016 5072 6564 6566 696e  ash.....Predefin
-0000a880: 6465 6441 6363 6f75 6e74 5479 7065 0103  dedAccountType..
-0000a890: 0000 001e 041a 0440 0435 0434 0438 0442  .......@.5.4.8.B
-0000a8a0: 044b 0020 002f 0020 0414 043e 043b 0433  .K. ./. ...>.;.3
-0000a8b0: 0438 0800 0000 0006 0000 000d 4465 6274  .8..........Debt
-0000a8c0: 7320 2f20 4c6f 616e 7307 0000 0016 5072  s / Loans.....Pr
-0000a8d0: 6564 6566 696e 6465 6441 6363 6f75 6e74  edefindedAccount
-0000a8e0: 5479 7065 0103 0000 0014 0418 043d 0432  Type.........=.2
-0000a8f0: 0435 0441 0442 0438 0446 0438 0438 0800  .5.A.B.8.F.8.8..
-0000a900: 0000 0006 0000 000b 496e 7665 7374 6d65  ........Investme
-0000a910: 6e74 7307 0000 0016 5072 6564 6566 696e  nts.....Predefin
-0000a920: 6465 6441 6363 6f75 6e74 5479 7065 0103  dedAccountType..
-0000a930: 0000 0014 0421 0431 0435 0440 0435 0436  .....!.1.5.@.5.6
-0000a940: 0435 043d 0438 044f 0800 0000 0006 0000  .5.=.8.O........
-0000a950: 0007 5361 7669 6e67 7307 0000 0016 5072  ..Savings.....Pr
-0000a960: 6564 6566 696e 6465 6441 6363 6f75 6e74  edefindedAccount
-0000a970: 5479 7065 0103 0000 0014 0065 002d 041a  Type.......e.-..
-0000a980: 043e 0448 0435 043b 044c 043a 0438 0800  .>.H.5.;.L.:.8..
-0000a990: 0000 0006 0000 0009 652d 5761 6c6c 6574  ........e-Wallet
-0000a9a0: 7307 0000 0016 5072 6564 6566 696e 6465  s.....Predefinde
-0000a9b0: 6441 6363 6f75 6e74 5479 7065 0103 0000  dAccountType....
-0000a9c0: 0012 041e 0431 043b 0438 0433 0430 0446  .....1.;.8.3.0.F
-0000a9d0: 0438 0438 0800 0000 0006 0000 0005 426f  .8.8..........Bo
-0000a9e0: 6e64 7307 0000 000f 5072 6564 6566 696e  nds.....Predefin
-0000a9f0: 6564 4173 7365 7401 0300 0000 0c04 2204  edAsset.......".
-0000aa00: 3e04 3204 3004 4004 4b08 0000 0000 0600  >.2.0.@.K.......
-0000aa10: 0000 0b43 6f6d 6d6f 6469 7469 6573 0700  ...Commodities..
-0000aa20: 0000 0f50 7265 6465 6669 6e65 6441 7373  ...PredefinedAss
-0000aa30: 6574 0103 0000 0018 041a 0440 0438 043f  et.........@.8.?
-0000aa40: 0442 043e 0432 0430 043b 044e 0442 044b  .B.>.2.0.;.N.B.K
-0000aa50: 0800 0000 0006 0000 000f 4372 7970 746f  ..........Crypto
-0000aa60: 2d63 7572 7265 6e63 7907 0000 000f 5072  -currency.....Pr
-0000aa70: 6564 6566 696e 6564 4173 7365 7401 0300  edefinedAsset...
-0000aa80: 0000 1404 1404 3504 4004 3804 3204 3004  ......5.@.8.2.0.
-0000aa90: 4204 3804 3204 4b08 0000 0000 0600 0000  B.8.2.K.........
-0000aaa0: 0b44 6572 6976 6174 6976 6573 0700 0000  .Derivatives....
-0000aab0: 0f50 7265 6465 6669 6e65 6441 7373 6574  .PredefinedAsset
-0000aac0: 0103 0000 0008 0411 041f 0418 0424 0800  .............$..
-0000aad0: 0000 0006 0000 0004 4554 4673 0700 0000  ........ETFs....
-0000aae0: 0f50 7265 6465 6669 6e65 6441 7373 6574  .PredefinedAsset
-0000aaf0: 0103 0000 000c 0424 043e 0440 0435 043a  .......$.>.@.5.:
-0000ab00: 0441 0800 0000 0006 0000 0005 466f 7265  .A..........Fore
-0000ab10: 7807 0000 000f 5072 6564 6566 696e 6564  x.....Predefined
-0000ab20: 4173 7365 7401 0300 0000 0a04 2404 3e04  Asset.......$.>.
-0000ab30: 3d04 3404 4b08 0000 0000 0600 0000 0546  =.4.K..........F
-0000ab40: 756e 6473 0700 0000 0f50 7265 6465 6669  unds.....Predefi
-0000ab50: 6e65 6441 7373 6574 0103 0000 000c 0412  nedAsset........
-0000ab60: 0430 043b 044e 0442 044b 0800 0000 0006  .0.;.N.B.K......
-0000ab70: 0000 0005 4d6f 6e65 7907 0000 000f 5072  ....Money.....Pr
-0000ab80: 6564 6566 696e 6564 4173 7365 7401 0300  edefinedAsset...
-0000ab90: 0000 0a04 1004 3a04 4604 3804 3808 0000  ......:.F.8.8...
-0000aba0: 0000 0600 0000 0653 6861 7265 7307 0000  .......Shares...
-0000abb0: 000f 5072 6564 6566 696e 6564 4173 7365  ..PredefinedAsse
-0000abc0: 7401 0300 0000 0200 2508 0000 0000 0600  t.......%.......
-0000abd0: 0000 0125 0700 0000 0f50 726f 6669 744c  ...%.....ProfitL
-0000abe0: 6f73 734d 6f64 656c 0103 0000 0006 0410  ossModel........
-0000abf0: 043f 0440 0800 0000 0006 0000 0003 4170  .?.@..........Ap
-0000ac00: 7207 0000 000f 5072 6f66 6974 4c6f 7373  r.....ProfitLoss
-0000ac10: 4d6f 6465 6c01 0300 0000 0404 2604 1108  Model.......&...
-0000ac20: 0000 0000 0600 0000 0641 7373 6574 7307  .........Assets.
-0000ac30: 0000 000f 5072 6f66 6974 4c6f 7373 4d6f  ....ProfitLossMo
-0000ac40: 6465 6c01 0300 0000 0604 1004 3204 3308  del.........2.3.
-0000ac50: 0000 0000 0600 0000 0341 7567 0700 0000  .........Aug....
-0000ac60: 0f50 726f 6669 744c 6f73 734d 6f64 656c  .ProfitLossModel
-0000ac70: 0103 0000 0012 0418 0437 043c 0435 043d  .........7.<.5.=
-0000ac80: 0435 043d 0438 0435 0800 0000 0006 0000  .5.=.8.5........
-0000ac90: 0006 4368 616e 6765 0700 0000 0f50 726f  ..Change.....Pro
-0000aca0: 6669 744c 6f73 734d 6f64 656c 0103 0000  fitLossModel....
-0000acb0: 0018 0418 0437 043c 0435 043d 0435 043d  .....7.<.5.=.5.=
-0000acc0: 0438 0435 002c 0020 0025 0800 0000 0006  .8.5.,. .%......
-0000acd0: 0000 0009 4368 616e 6765 2c20 2507 0000  ....Change, %...
-0000ace0: 000f 5072 6f66 6974 4c6f 7373 4d6f 6465  ..ProfitLossMode
-0000acf0: 6c01 0300 0000 0604 1404 3504 3a08 0000  l.........5.:...
-0000ad00: 0000 0600 0000 0344 6563 0700 0000 0f50  .......Dec.....P
-0000ad10: 726f 6669 744c 6f73 734d 6f64 656c 0103  rofitLossModel..
-0000ad20: 0000 0012 0414 0438 0432 0438 0434 0435  .......8.2.8.4.5
-0000ad30: 043d 0434 044b 0800 0000 0006 0000 0009  .=.4.K..........
-0000ad40: 4469 7669 6465 6e64 7307 0000 000f 5072  Dividends.....Pr
-0000ad50: 6f66 6974 4c6f 7373 4d6f 6465 6c01 0300  ofitLossModel...
-0000ad60: 0000 0604 2404 3504 3208 0000 0000 0600  ....$.5.2.......
-0000ad70: 0000 0346 6562 0700 0000 0f50 726f 6669  ...Feb.....Profi
-0000ad80: 744c 6f73 734d 6f64 656c 0103 0000 0010  tLossModel......
-0000ad90: 041a 043e 043c 0438 0441 0441 0438 0438  ...>.<.8.A.A.8.8
-0000ada0: 0800 0000 0006 0000 0004 4665 6573 0700  ..........Fees..
-0000adb0: 0000 0f50 726f 6669 744c 6f73 734d 6f64  ...ProfitLossMod
-0000adc0: 656c 0103 0000 0018 0412 0432 043e 0434  el.........2.>.4
-0000add0: 0020 002f 0020 0412 044b 0432 043e 0434  . ./. ...K.2.>.4
-0000ade0: 0800 0000 0006 0000 0008 496e 202f 204f  ..........In / O
-0000adf0: 7574 0700 0000 0f50 726f 6669 744c 6f73  ut.....ProfitLos
-0000ae00: 734d 6f64 656c 0103 0000 0006 042f 043d  sModel......./.=
-0000ae10: 0432 0800 0000 0006 0000 0003 4a61 6e07  .2..........Jan.
-0000ae20: 0000 000f 5072 6f66 6974 4c6f 7373 4d6f  ....ProfitLossMo
-0000ae30: 6465 6c01 0300 0000 0604 1804 4e04 3b08  del.........N.;.
-0000ae40: 0000 0000 0600 0000 034a 756c 0700 0000  .........Jul....
-0000ae50: 0f50 726f 6669 744c 6f73 734d 6f64 656c  .ProfitLossModel
-0000ae60: 0103 0000 0006 0418 044e 043d 0800 0000  .........N.=....
-0000ae70: 0006 0000 0003 4a75 6e07 0000 000f 5072  ......Jun.....Pr
-0000ae80: 6f66 6974 4c6f 7373 4d6f 6465 6c01 0300  ofitLossModel...
-0000ae90: 0000 0604 1c04 3004 4008 0000 0000 0600  ......0.@.......
-0000aea0: 0000 034d 6172 0700 0000 0f50 726f 6669  ...Mar.....Profi
-0000aeb0: 744c 6f73 734d 6f64 656c 0103 0000 0006  tLossModel......
-0000aec0: 041c 0430 0439 0800 0000 0006 0000 0003  ...0.9..........
-0000aed0: 4d61 7907 0000 000f 5072 6f66 6974 4c6f  May.....ProfitLo
-0000aee0: 7373 4d6f 6465 6c01 0300 0000 0404 1404  ssModel.........
-0000aef0: 2108 0000 0000 0600 0000 054d 6f6e 6579  !..........Money
-0000af00: 0700 0000 0f50 726f 6669 744c 6f73 734d  .....ProfitLossM
-0000af10: 6f64 656c 0103 0000 0006 041d 043e 044f  odel.........>.O
-0000af20: 0800 0000 0006 0000 0003 4e6f 7607 0000  ..........Nov...
-0000af30: 000f 5072 6f66 6974 4c6f 7373 4d6f 6465  ..ProfitLossMode
-0000af40: 6c01 0300 0000 0604 1e04 3a04 4208 0000  l.........:.B...
-0000af50: 0000 0600 0000 034f 6374 0700 0000 0f50  .......Oct.....P
-0000af60: 726f 6669 744c 6f73 734d 6f64 656c 0103  rofitLossModel..
-0000af70: 0000 0006 041f 0438 0423 0800 0000 0006  .......8.#......
-0000af80: 0000 0003 5026 4c07 0000 000f 5072 6f66  ....P&L.....Prof
-0000af90: 6974 4c6f 7373 4d6f 6465 6c01 0300 0000  itLossModel.....
-0000afa0: 0c04 1f04 3504 4004 3804 3e04 3408 0000  ....5.@.8.>.4...
-0000afb0: 0000 0600 0000 0650 6572 696f 6407 0000  .......Period...
-0000afc0: 000f 5072 6f66 6974 4c6f 7373 4d6f 6465  ..ProfitLossMode
-0000afd0: 6c01 0300 0000 1a04 1a04 3e04 3d04 3504  l.........>.=.5.
-0000afe0: 4600 2004 3f04 3504 4004 3804 3e04 3404  F. .?.5.@.8.>.4.
-0000aff0: 3008 0000 0000 0600 0000 0a50 6572 696f  0..........Perio
-0000b000: 6420 656e 6407 0000 000f 5072 6f66 6974  d end.....Profit
-0000b010: 4c6f 7373 4d6f 6465 6c01 0300 0000 1c04  LossModel.......
-0000b020: 1d04 3004 4704 3004 3b04 3e00 2004 3f04  ..0.G.0.;.>. .?.
-0000b030: 3504 4004 3804 3e04 3404 3008 0000 0000  5.@.8.>.4.0.....
-0000b040: 0600 0000 0c50 6572 696f 6420 7374 6172  .....Period star
-0000b050: 7407 0000 000f 5072 6f66 6974 4c6f 7373  t.....ProfitLoss
-0000b060: 4d6f 6465 6c01 0300 0000 0604 2104 3504  Model.......!.5.
-0000b070: 3d08 0000 0000 0600 0000 0353 6570 0700  =..........Sep..
-0000b080: 0000 0f50 726f 6669 744c 6f73 734d 6f64  ...ProfitLossMod
-0000b090: 656c 0103 0000 000c 041d 0430 043b 043e  el.........0.;.>
-0000b0a0: 0433 0438 0800 0000 0006 0000 0005 5461  .3.8..........Ta
-0000b0b0: 7865 7307 0000 000f 5072 6f66 6974 4c6f  xes.....ProfitLo
-0000b0c0: 7373 4d6f 6465 6c01 0300 0000 0a04 1804  ssModel.........
-0000b0d0: 4204 3e04 3304 3e08 0000 0000 0600 0000  B.>.3.>.........
-0000b0e0: 0554 6f74 616c 0700 0000 0f50 726f 6669  .Total.....Profi
-0000b0f0: 744c 6f73 734d 6f64 656c 0103 0000 0018  tLossModel......
-0000b100: 041f 0438 0423 0020 043f 043e 0020 0441  ...8.#. .?.>. .A
-0000b110: 0447 0451 0442 0443 0800 0000 0006 0000  .G.Q.B.C........
-0000b120: 000e 5026 4c20 6279 2041 6363 6f75 6e74  ..P&L by Account
-0000b130: 0700 0000 1050 726f 6669 744c 6f73 7352  .....ProfitLossR
-0000b140: 6570 6f72 7401 0300 0000 0a04 2104 4704  eport.......!.G.
-0000b150: 3504 4200 3a08 0000 0000 0600 0000 0841  5.B.:..........A
-0000b160: 6363 6f75 6e74 3a07 0000 0016 5072 6f66  ccount:.....Prof
-0000b170: 6974 4c6f 7373 5265 706f 7274 5769 6467  itLossReportWidg
-0000b180: 6574 0103 0000 0010 0412 0430 043b 044e  et.........0.;.N
-0000b190: 0442 0430 003a 0020 0800 0000 0006 0000  .B.0.:. ........
-0000b1a0: 000a 4375 7272 656e 6379 3a20 0700 0000  ..Currency: ....
-0000b1b0: 1650 726f 6669 744c 6f73 7352 6570 6f72  .ProfitLossRepor
-0000b1c0: 7457 6964 6765 7401 0300 0000 0604 1f04  tWidget.........
-0000b1d0: 3804 2308 0000 0000 0600 0000 0350 264c  8.#..........P&L
-0000b1e0: 0700 0000 1650 726f 6669 744c 6f73 7352  .....ProfitLossR
-0000b1f0: 6570 6f72 7457 6964 6765 7401 0300 0000  eportWidget.....
-0000b200: 1804 2104 3e04 4504 4004 3004 3d04 3804  ..!.>.E.@.0.=.8.
-0000b210: 4204 4c00 2e00 2e00 2e08 0000 0000 0600  B.L.............
-0000b220: 0000 0753 6176 652e 2e2e 0700 0000 1650  ...Save........P
-0000b230: 726f 6669 744c 6f73 7352 6570 6f72 7457  rofitLossReportW
-0000b240: 6964 6765 7401 0300 0000 1004 1204 3004  idget.........0.
-0000b250: 3b04 4e04 4204 3000 3a00 2008 0000 0000  ;.N.B.0.:. .....
-0000b260: 0600 0000 0a43 7572 7265 6e63 793a 2007  .....Currency: .
-0000b270: 0000 0016 5072 6f66 6974 4c6f 7373 5265  ....ProfitLossRe
-0000b280: 706f 7274 5769 6e64 6f77 0103 0000 0018  portWindow......
-0000b290: 041f 0438 0423 0020 043f 043e 0020 0441  ...8.#. .?.>. .A
-0000b2a0: 0447 0451 0442 0443 0800 0000 0006 0000  .G.Q.B.C........
-0000b2b0: 000e 5026 4c20 6279 2041 6363 6f75 6e74  ..P&L by Account
-0000b2c0: 0700 0000 1650 726f 6669 744c 6f73 7352  .....ProfitLossR
-0000b2d0: 6570 6f72 7457 696e 646f 7701 0300 0000  eportWindow.....
-0000b2e0: 1e04 1e04 4804 3804 3104 3a04 3000 2004  ....H.8.1.:.0. .
-0000b2f0: 3a04 3004 3c04 3504 4004 4b00 3a00 2008  :.0.<.5.@.K.:. .
-0000b300: 0000 0000 0600 0000 0e43 616d 6572 6120  .........Camera 
-0000b310: 6572 726f 723a 2007 0000 0009 5152 5363  error: .....QRSc
-0000b320: 616e 6e65 7201 0300 0000 8404 1d04 3500  anner.........5.
-0000b330: 2004 3e04 3104 3d04 3004 4004 4304 3604   .>.1.=.0.@.C.6.
-0000b340: 3504 3d00 2004 3f04 3004 3a04 3504 4200  5.=. .?.0.:.5.B.
-0000b350: 2000 7000 7900 7a00 6200 6100 7200 2c00   .p.y.z.b.a.r.,.
-0000b360: 2004 3d04 3504 3e04 3104 4504 3e04 3404   .=.5.>.1.E.>.4.
-0000b370: 3804 3c04 4b04 3900 2004 3404 3b04 4f00  8.<.K.9. .4.;.O.
-0000b380: 2004 4004 3004 4104 3f04 3e04 3704 3d04   .@.0.A.?.>.7.=.
-0000b390: 3004 3204 3004 3d04 3804 4f00 2000 5100  0.2.0.=.8.O. .Q.
-0000b3a0: 5200 2004 3a04 3e04 3404 3e04 3200 2e08  R. .:.>.4.>.2...
-0000b3b0: 0000 0000 0600 0000 2c50 6163 6b61 6765  ........,Package
-0000b3c0: 2070 797a 6261 7220 6e6f 7420 666f 756e   pyzbar not foun
-0000b3d0: 6420 666f 7220 5152 2072 6563 6f67 6e69  d for QR recogni
-0000b3e0: 7469 6f6e 2e07 0000 0009 5152 5363 616e  tion......QRScan
-0000b3f0: 6e65 7201 0300 0000 2604 1d04 3504 4200  ner.....&...5.B.
-0000b400: 2004 3404 3e04 4104 4204 4304 3f04 3d04   .4.>.A.B.C.?.=.
-0000b410: 4b04 4500 2004 3a04 3004 3c04 3504 4008  K.E. .:.0.<.5.@.
-0000b420: 0000 0000 0600 0000 1e54 6865 7265 2061  .........There a
-0000b430: 7265 206e 6f20 6361 6d65 7261 7320 6176  re no cameras av
-0000b440: 6169 6c61 626c 6507 0000 0009 5152 5363  ailable.....QRSc
-0000b450: 616e 6e65 7201 0300 0000 6804 1d04 3504  anner.....h...5.
-0000b460: 3204 3e04 3704 3c04 3e04 3604 3d04 3e00  2.>.7.<.>.6.=.>.
-0000b470: 2004 3e04 3104 4004 3004 3104 3e04 4204   .>.1.@.0.1.>.B.
-0000b480: 3004 4204 4c00 2004 3404 3004 3d04 3d04  0.B.L. .4.0.=.=.
-0000b490: 4b04 3500 2004 3a04 3e04 4204 3804 4004  K.5. .:.>.B.8.@.
-0000b4a0: 3e04 3204 3e04 3a00 2004 4100 2004 3104  >.2.>.:. .A. .1.
-0000b4b0: 3804 4004 3604 3800 2000 5400 5300 5800  8.@.6.8. .T.S.X.
-0000b4c0: 3a00 2008 0000 0000 0600 0000 2143 616e  :. .........!Can
-0000b4d0: 2774 2070 6172 7365 2064 6174 6120 666f  't parse data fo
-0000b4e0: 7220 5453 5820 7175 6f74 6573 3a20 0700  r TSX quotes: ..
-0000b4f0: 0000 0f51 756f 7465 446f 776e 6c6f 6164  ...QuoteDownload
-0000b500: 6572 0103 0000 0024 0417 0430 0433 0440  er.....$...0.3.@
-0000b510: 0443 0437 043a 0430 0020 0437 0430 0432  .C.7.:.0. .7.0.2
-0000b520: 0435 0440 0448 0435 043d 0430 0800 0000  .5.@.H.5.=.0....
-0000b530: 0006 0000 0012 446f 776e 6c6f 6164 2063  ......Download c
-0000b540: 6f6d 706c 6574 6564 0700 0000 0f51 756f  ompleted.....Quo
-0000b550: 7465 446f 776e 6c6f 6164 6572 0103 0000  teDownloader....
-0000b560: 0060 0049 0053 0049 004e 0020 0432 0020  .`.I.S.I.N. .2. 
-0000b570: 0438 0441 0442 043e 0440 0438 0438 0020  .8.A.B.>.@.8.8. 
-0000b580: 043a 043e 0442 0438 0440 043e 0432 043e  .:.>.B.8.@.>.2.>
-0000b590: 043a 0020 0045 0075 0072 006f 006e 0065  .:. .E.u.r.o.n.e
-0000b5a0: 0078 0074 0020 043d 0435 0020 0441 043e  .x.t. .=.5. .A.>
-0000b5b0: 0432 043f 0430 0434 0430 0435 0442 003a  .2.?.0.4.0.5.B.:
-0000b5c0: 0020 0800 0000 0006 0000 0022 4575 726f  . ........."Euro
-0000b5d0: 6e65 7874 2071 756f 7465 7320 4953 494e  next quotes ISIN
-0000b5e0: 206d 6973 6d61 7463 6820 696e 3a20 0700   mismatch in: ..
-0000b5f0: 0000 0f51 756f 7465 446f 776e 6c6f 6164  ...QuoteDownload
-0000b600: 6572 0103 0000 0064 0417 0430 0433 043e  er.....d...0.3.>
-0000b610: 043b 043e 0432 043e 043a 0020 0438 0441  .;.>.2.>.:. .8.A
-0000b620: 0442 043e 0440 0438 0438 0020 043a 043e  .B.>.@.8.8. .:.>
-0000b630: 0442 0438 0440 043e 0432 043e 043a 0020  .B.8.@.>.2.>.:. 
-0000b640: 0045 0075 0072 006f 006e 0065 0078 0074  .E.u.r.o.n.e.x.t
-0000b650: 0020 043d 0435 0020 043d 0430 0439 0434  . .=.5. .=.0.9.4
-0000b660: 0435 043d 0020 0432 003a 0020 0800 0000  .5.=. .2.:. ....
-0000b670: 0006 0000 0025 4575 726f 6e65 7874 2071  .....%Euronext q
-0000b680: 756f 7465 7320 6865 6164 6572 206e 6f74  uotes header not
-0000b690: 2066 6f75 6e64 2069 6e3a 2007 0000 000f   found in: .....
-0000b6a0: 5175 6f74 6544 6f77 6e6c 6f61 6465 7201  QuoteDownloader.
-0000b6b0: 0300 0000 5a04 1804 4104 4204 3e04 4004  ....Z...A.B.>.@.
-0000b6c0: 3804 4f00 2004 3a04 3e04 4204 3804 4004  8.O. .:.>.B.8.@.
-0000b6d0: 3e04 3204 3e04 3a00 2000 4500 7500 7200  >.2.>.:. .E.u.r.
-0000b6e0: 6f00 6e00 6500 7800 7400 2004 4104 3b04  o.n.e.x.t. .A.;.
-0000b6f0: 3804 4804 3a04 3e04 3c00 2004 3a04 3e04  8.H.:.>.<. .:.>.
-0000b700: 4004 3e04 4204 3a04 3004 4f00 3a00 2008  @.>.B.:.0.O.:. .
-0000b710: 0000 0000 0600 0000 2c45 7572 6f6e 6578  ........,Euronex
-0000b720: 7420 7175 6f74 6573 2068 6973 746f 7279  t quotes history
-0000b730: 2072 6570 6c79 2069 7320 746f 6f20 7368   reply is too sh
-0000b740: 6f72 743a 2007 0000 000f 5175 6f74 6544  ort: .....QuoteD
-0000b750: 6f77 6e6c 6f61 6465 7201 0300 0000 3604  ownloader.....6.
-0000b760: 1d04 3500 2004 3704 3004 3304 4004 4304  ..5. .7.0.3.@.C.
-0000b770: 3604 3504 3d04 4b00 2004 3a04 3e04 4204  6.5.=.K. .:.>.B.
-0000b780: 3804 4004 3e04 3204 3a04 3800 2004 3404  8.@.>.2.:.8. .4.
-0000b790: 3b04 4f00 2008 0000 0000 0600 0000 1e4e  ;.O. ..........N
-0000b7a0: 6f20 7175 6f74 6573 2077 6572 6520 646f  o quotes were do
-0000b7b0: 776e 6c6f 6164 6564 2066 6f72 2007 0000  wnloaded for ...
-0000b7c0: 000f 5175 6f74 6544 6f77 6e6c 6f61 6465  ..QuoteDownloade
-0000b7d0: 7201 0300 0000 2e04 1d04 3500 2004 3704  r.........5. .7.
-0000b7e0: 3004 3304 4004 4304 3604 3504 3d04 4b00  0.3.@.C.6.5.=.K.
-0000b7f0: 2004 3a04 4304 4004 4104 4b00 2004 3404   .:.C.@.A.K. .4.
-0000b800: 3b04 4f00 2008 0000 0000 0600 0000 1d4e  ;.O. ..........N
-0000b810: 6f20 7261 7465 7320 7765 7265 2064 6f77  o rates were dow
-0000b820: 6e6c 6f61 6465 6420 666f 7220 0700 0000  nloaded for ....
-0000b830: 0f51 756f 7465 446f 776e 6c6f 6164 6572  .QuoteDownloader
-0000b840: 0103 0000 002c 041d 0435 0442 0020 0434  .....,...5.B. .4
-0000b850: 0430 043d 043d 044b 0445 0020 0426 0411  .0.=.=.K.E. .&..
-0000b860: 0020 0420 0424 0020 0434 043b 044f 003a  . . .$. .4.;.O.:
-0000b870: 0020 0800 0000 0006 0000 001b 5468 6572  . ..........Ther
-0000b880: 6520 6172 6520 6e6f 2043 4252 2064 6174  e are no CBR dat
-0000b890: 6120 666f 723a 2007 0000 000f 5175 6f74  a for: .....Quot
-0000b8a0: 6544 6f77 6e6c 6f61 6465 7201 0300 0000  eDownloader.....
-0000b8b0: 1204 1a04 3e04 4204 3804 4004 3e04 3204  ....>.B.8.@.>.2.
-0000b8c0: 3a04 3808 0000 0000 0600 0000 0651 756f  :.8..........Quo
-0000b8d0: 7465 7307 0000 0010 5175 6f74 6573 4c69  tes.....QuotesLi
-0000b8e0: 7374 4469 616c 6f67 0103 0000 0004 0426  stDialog.......&
-0000b8f0: 0411 0800 0000 0006 0000 0005 4173 7365  ............Asse
-0000b900: 7407 0000 000f 5175 6f74 6573 4c69 7374  t.....QuotesList
-0000b910: 4d6f 6465 6c01 0300 0000 0c04 1204 3004  Model.........0.
-0000b920: 3b04 4e04 4204 3008 0000 0000 0600 0000  ;.N.B.0.........
-0000b930: 0843 7572 7265 6e63 7907 0000 000f 5175  .Currency.....Qu
-0000b940: 6f74 6573 4c69 7374 4d6f 6465 6c01 0300  otesListModel...
-0000b950: 0000 0804 1404 3004 4204 3008 0000 0000  ......0.B.0.....
-0000b960: 0600 0000 0444 6174 6507 0000 000f 5175  .....Date.....Qu
-0000b970: 6f74 6573 4c69 7374 4d6f 6465 6c01 0300  otesListModel...
-0000b980: 0000 1204 1a04 3e04 4204 3804 4004 3e04  ......>.B.8.@.>.
-0000b990: 3204 3a04 3008 0000 0000 0600 0000 0551  2.:.0..........Q
-0000b9a0: 756f 7465 0700 0000 0f51 756f 7465 734c  uote.....QuotesL
-0000b9b0: 6973 744d 6f64 656c 0103 0000 0028 0026  istModel.....(.&
-0000b9c0: 041f 043e 043b 043d 043e 0441 0442 044c  ...>.;.=.>.A.B.L
-0000b9d0: 044e 002c 0020 0441 0020 043d 0430 0447  .N.,. .A. .=.0.G
-0000b9e0: 0430 043b 0430 0800 0000 0006 0000 0013  .0.;.0..........
-0000b9f0: 2646 756c 6c2c 2066 726f 6d20 7363 7261  &Full, from scra
-0000ba00: 7463 6807 0000 000d 5265 4275 696c 6444  tch.....ReBuildD
-0000ba10: 6961 6c6f 6701 0300 0000 1804 1804 3d04  ialog.........=.
-0000ba20: 4204 3504 4004 3204 3004 3b00 2004 3404  B.5.@.2.0.;. .4.
-0000ba30: 3004 4208 0000 0000 0600 0000 0a44 6174  0.B..........Dat
-0000ba40: 6520 5261 6e67 6507 0000 000d 5265 4275  e Range.....ReBu
-0000ba50: 696c 6444 6961 6c6f 6701 0300 0000 2a00  ildDialog.....*.
-0000ba60: 2604 1104 4b04 4104 4204 4004 3e00 2c00  &...K.A.B.@.>.,.
-0000ba70: 2004 3d04 3e00 2004 3d04 3504 3d04 3004   .=.>. .=.5.=.0.
-0000ba80: 3404 5104 3604 3d04 3e08 0000 0000 0600  4.Q.6.=.>.......
-0000ba90: 0000 1146 6173 742c 2026 756e 7265 6c69  ...Fast, &unreli
-0000baa0: 6162 6c65 0700 0000 0d52 6542 7569 6c64  able.....ReBuild
-0000bab0: 4469 616c 6f67 0103 0000 0016 0414 0430  Dialog.........0
-0000bac0: 0442 0430 0413 0440 0430 043d 0438 0446  .B.0...@.0.=.8.F
-0000bad0: 044b 0800 0000 0006 0000 000c 4672 6f6e  .K..........Fron
-0000bae0: 7469 6572 4461 7465 0700 0000 0d52 6542  tierDate.....ReB
-0000baf0: 7569 6c64 4469 616c 6f67 0103 0000 0022  uildDialog....."
-0000bb00: 041f 0435 0440 0435 0441 0447 0438 0442  ...5.@.5.A.G.8.B
-0000bb10: 0430 0442 044c 0020 0438 0442 043e 0433  .0.B.L. .8.B.>.3
-0000bb20: 0438 0800 0000 0006 0000 000f 5265 2d42  .8..........Re-B
-0000bb30: 7569 6c64 204c 6564 6765 7207 0000 000d  uild Ledger.....
-0000bb40: 5265 4275 696c 6444 6961 6c6f 6701 0300  ReBuildDialog...
-0000bb50: 0000 1004 2100 2000 2604 1404 3004 4204  ....!. .&...0.B.
-0000bb60: 4b00 3a08 0000 0000 0600 0000 0c53 696e  K.:..........Sin
-0000bb70: 6365 2026 4461 7465 3a07 0000 000d 5265  ce &Date:.....Re
-0000bb80: 4275 696c 6444 6961 6c6f 6701 0300 0000  BuildDialog.....
-0000bb90: 2c04 2100 2004 3a04 4004 3004 3904 3d04  ,.!. .:.@.0.9.=.
-0000bba0: 3504 3900 2000 2604 3004 3a04 4204 4304  5.9. .&.0.:.B.C.
-0000bbb0: 3004 3b04 4c04 3d04 3e04 3900 3a08 0000  0.;.L.=.>.9.:...
-0000bbc0: 0000 0600 0000 1353 696e 6365 2026 4c61  .......Since &La
-0000bbd0: 7374 2061 6374 7561 6c3a 0700 0000 0d52  st actual:.....R
-0000bbe0: 6542 7569 6c64 4469 616c 6f67 0103 0000  eBuildDialog....
-0000bbf0: 0014 0064 0064 002f 004d 004d 002f 0079  ...d.d./.M.M./.y
-0000bc00: 0079 0079 0079 0800 0000 0006 0000 000a  .y.y.y..........
-0000bc10: 6464 2f4d 4d2f 7979 7979 0700 0000 0d52  dd/MM/yyyy.....R
-0000bc20: 6542 7569 6c64 4469 616c 6f67 0103 0000  eBuildDialog....
-0000bc30: 000a 041b 044e 0431 043e 0439 0800 0000  .....N.1.>.9....
-0000bc40: 0006 0000 0003 414e 5907 0000 0013 5265  ......ANY.....Re
-0000bc50: 6665 7265 6e63 6544 6174 6144 6961 6c6f  ferenceDataDialo
-0000bc60: 6701 0300 0000 1404 2204 3804 3f00 2004  g.......".8.?. .
-0000bc70: 4104 4704 3504 4204 3000 3a08 0000 0000  A.G.5.B.0.:.....
-0000bc80: 0600 0000 0d41 6363 6f75 6e74 2054 7970  .....Account Typ
-0000bc90: 653a 0700 0000 1352 6566 6572 656e 6365  e:.....Reference
-0000bca0: 4461 7461 4469 616c 6f67 0103 0000 0022  DataDialog....."
-0000bcb0: 0414 043e 0431 0430 0432 0438 0442 044c  ...>.1.0.2.8.B.L
-0000bcc0: 0020 0434 043e 0447 0435 0440 043d 0438  . .4.>.G.5.@.=.8
-0000bcd0: 0439 0800 0000 0006 0000 0009 4164 6420  .9..........Add 
-0000bce0: 6368 696c 6407 0000 0013 5265 6665 7265  child.....Refere
-0000bcf0: 6e63 6544 6174 6144 6961 6c6f 6701 0300  nceDataDialog...
-0000bd00: 0000 1c04 1404 3e04 3104 3004 3204 3804  ......>.1.0.2.8.
-0000bd10: 4204 4c00 2004 3d04 3e04 3204 4b04 3908  B.L. .=.>.2.K.9.
-0000bd20: 0000 0000 0600 0000 0741 6464 206e 6577  .........Add new
-0000bd30: 0700 0000 1352 6566 6572 656e 6365 4461  .....ReferenceDa
-0000bd40: 7461 4469 616c 6f67 0103 0000 001e 0421  taDialog.......!
-0000bd50: 043c 0435 043d 0438 0442 044c 0020 0442  .<.5.=.8.B.L. .B
-0000bd60: 0438 043f 0020 043d 0430 003a 0800 0000  .8.?. .=.0.:....
-0000bd70: 0006 0000 000f 4368 616e 6765 2074 7970  ......Change typ
-0000bd80: 6520 746f 3a07 0000 0013 5265 6665 7265  e to:.....Refere
-0000bd90: 6e63 6544 6174 6144 6961 6c6f 6701 0300  nceDataDialog...
-0000bda0: 0000 1a04 1f04 3e04 3404 4204 3204 3504  ......>.4.B.2.5.
-0000bdb0: 4004 3604 3404 3504 3d04 3804 3508 0000  @.6.4.5.=.8.5...
-0000bdc0: 0000 0600 0000 0c43 6f6e 6669 726d 6174  .......Confirmat
-0000bdd0: 696f 6e07 0000 0013 5265 6665 7265 6e63  ion.....Referenc
-0000bde0: 6544 6174 6144 6961 6c6f 6701 0300 0000  eDataDialog.....
-0000bdf0: 0e04 2304 3404 3004 3b04 3804 4204 4c08  ..#.4.0.;.8.B.L.
-0000be00: 0000 0000 0600 0000 0644 656c 6574 6507  .........Delete.
-0000be10: 0000 0013 5265 6665 7265 6e63 6544 6174  ....ReferenceDat
-0000be20: 6144 6961 6c6f 6701 0300 0000 2204 2104  aDialog.....".!.
-0000be30: 3f04 4004 3004 3204 3e04 4704 3d04 4b04  ?.@.0.2.>.G.=.K.
-0000be40: 3500 2004 3404 3004 3d04 3d04 4b04 3508  5. .4.0.=.=.K.5.
-0000be50: 0000 0000 0600 0000 0e52 6566 6572 656e  .........Referen
-0000be60: 6365 2044 6174 6107 0000 0013 5265 6665  ce Data.....Refe
-0000be70: 7265 6e63 6544 6174 6144 6961 6c6f 6701  renceDataDialog.
-0000be80: 0300 0000 2404 1e04 4204 3c04 3504 3d04  ....$...B.<.5.=.
-0000be90: 3804 4204 4c00 2004 3804 3704 3c04 3504  8.B.L. .8.7.<.5.
-0000bea0: 3d04 3504 3d04 3804 4f08 0000 0000 0600  =.5.=.8.O.......
-0000beb0: 0000 0e52 6576 6572 7420 6368 616e 6765  ...Revert change
-0000bec0: 7307 0000 0013 5265 6665 7265 6e63 6544  s.....ReferenceD
-0000bed0: 6174 6144 6961 6c6f 6701 0300 0000 2604  ataDialog.....&.
-0000bee0: 2104 3e04 4504 4004 3004 3d04 3804 4204  !.>.E.@.0.=.8.B.
-0000bef0: 4c00 2004 3804 3704 3c04 3504 3d04 3504  L. .8.7.<.5.=.5.
-0000bf00: 3d04 3804 4f08 0000 0000 0600 0000 0c53  =.8.O..........S
-0000bf10: 6176 6520 6368 616e 6765 7307 0000 0013  ave changes.....
-0000bf20: 5265 6665 7265 6e63 6544 6174 6144 6961  ReferenceDataDia
-0000bf30: 6c6f 6701 0300 0000 0c04 1f04 3e04 3804  log.........>.8.
-0000bf40: 4104 3a00 3a08 0000 0000 0600 0000 0753  A.:.:..........S
-0000bf50: 6561 7263 683a 0700 0000 1352 6566 6572  earch:.....Refer
-0000bf60: 656e 6365 4461 7461 4469 616c 6f67 0103  enceDataDialog..
-0000bf70: 0000 002a 041f 043e 043a 0430 0437 044b  ...*...>.:.0.7.K
-0000bf80: 0432 0430 0442 044c 0020 043d 0435 0430  .2.0.B.L. .=.5.0
-0000bf90: 043a 0442 0438 0432 043d 044b 0435 0800  .:.B.8.2.=.K.5..
-0000bfa0: 0000 0006 0000 000d 5368 6f77 2069 6e61  ........Show ina
-0000bfb0: 6374 6976 6507 0000 0013 5265 6665 7265  ctive.....Refere
-0000bfc0: 6e63 6544 6174 6144 6961 6c6f 6701 0300  nceDataDialog...
-0000bfd0: 0000 6604 2300 2004 3204 3004 4100 2004  ..f.#. .2.0.A. .
-0000bfe0: 3504 4104 4204 4c00 2004 3d04 3504 4104  5.A.B.L. .=.5.A.
-0000bff0: 3e04 4504 4004 3004 3d04 5104 3d04 3d04  >.E.@.0.=.Q.=.=.
-0000c000: 4b04 3500 2004 3404 3004 3d04 3d04 4b04  K.5. .4.0.=.=.K.
-0000c010: 3500 2e00 2004 1204 4104 5100 2004 4004  5... ...A.Q. .@.
-0000c020: 3004 3204 3d04 3e00 2004 3704 3004 3a04  0.2.=.>. .7.0.:.
-0000c030: 4004 4b04 4204 4c00 3f08 0000 0000 0600  @.K.B.L.?.......
-0000c040: 0000 3359 6f75 2068 6176 6520 756e 636f  ..3You have unco
-0000c050: 6d6d 6974 7465 6420 6368 616e 6765 732e  mmitted changes.
-0000c060: 2044 6f20 796f 7520 7761 6e74 2074 6f20   Do you want to 
-0000c070: 636c 6f73 653f 0700 0000 1352 6566 6572  close?.....Refer
-0000c080: 656e 6365 4461 7461 4469 616c 6f67 0103  enceDataDialog..
-0000c090: 0000 0028 0424 0430 0439 043b 044b 0020  ...(.$.0.9.;.K. 
-0000c0a0: 0045 0078 0063 0065 006c 0020 0028 002a  .E.x.c.e.l. .(.*
-0000c0b0: 002e 0078 0073 006c 0078 0029 0800 0000  ...x.s.l.x.)....
-0000c0c0: 0006 0000 0014 4578 6365 6c20 6669 6c65  ......Excel file
-0000c0d0: 7320 282a 2e78 6c73 7829 0700 0000 0752  s (*.xlsx).....R
-0000c0e0: 6570 6f72 7473 0103 0000 0046 041d 0435  eports.....F...5
-0000c0f0: 0432 043e 0437 043c 043e 0436 043d 043e  .2.>.7.<.>.6.=.>
-0000c100: 0020 0437 0430 0433 0440 0443 0437 0438  . .7.0.3.@.C.7.8
-0000c110: 0442 044c 0020 043a 043b 0430 0441 0441  .B.L. .:.;.0.A.A
-0000c120: 0020 043e 0442 0447 0451 0442 0430 003a  . .>.B.G.Q.B.0.:
-0000c130: 0020 0800 0000 0006 0000 001e 5265 706f  . ..........Repo
-0000c140: 7274 2063 6c61 7373 2063 616e 2774 2062  rt class can't b
-0000c150: 6520 6c6f 6164 6564 3a20 0700 0000 0752  e loaded: .....R
-0000c160: 6570 6f72 7473 0103 0000 0042 041e 0442  eports.....B...B
-0000c170: 0447 0435 0442 0020 043d 0435 0020 043d  .G.5.B. .=.5. .=
-0000c180: 0430 0439 0434 0435 043d 0020 0434 043b  .0.9.4.5.=. .4.;
-0000c190: 044f 0020 043a 043b 0430 0441 0441 0430  .O. .:.;.0.A.A.0
-0000c1a0: 0020 043e 043a 043d 0430 003a 0020 0800  . .>.:.=.0.:. ..
-0000c1b0: 0000 0006 0000 0023 5265 706f 7274 206e  .......#Report n
-0000c1c0: 6f74 2066 6f75 6e64 2066 6f72 2077 696e  ot found for win
-0000c1d0: 646f 7720 636c 6173 733a 2007 0000 0007  dow class: .....
-0000c1e0: 5265 706f 7274 7301 0300 0000 2c04 1e04  Reports.....,...
-0000c1f0: 4204 4704 3504 4200 2004 4104 3e04 4504  B.G.5.B. .A.>.E.
-0000c200: 4004 3004 3d04 5104 3d00 2004 3200 2004  @.0.=.Q.=. .2. .
-0000c210: 4404 3004 3904 3b00 2008 0000 0000 0600  D.0.9.;. .......
-0000c220: 0000 1952 6570 6f72 7420 7761 7320 7361  ...Report was sa
-0000c230: 7665 6420 746f 2066 696c 6520 0700 0000  ved to file ....
-0000c240: 0752 6570 6f72 7473 0103 0000 0024 0421  .Reports.....$.!
-0000c250: 043e 0445 0440 0430 043d 0438 0442 044c  .>.E.@.0.=.8.B.L
-0000c260: 0020 043e 0442 0447 0435 0442 0020 0432  . .>.B.G.5.B. .2
-0000c270: 003a 0800 0000 0006 0000 000f 5361 7665  .:..........Save
-0000c280: 2072 6570 6f72 7420 746f 3a07 0000 0007   report to:.....
-0000c290: 5265 706f 7274 7301 0300 0000 3c04 1b04  Reports.....<...
-0000c2a0: 3e04 3304 3804 3d00 2004 4704 3504 4004  >.3.8.=. .G.5.@.
-0000c2b0: 3504 3700 2004 1304 3e04 4104 4304 4104  5.7. ...>.A.C.A.
-0000c2c0: 3b04 4304 3304 3800 2004 3704 3004 3204  ;.C.3.8. .7.0.2.
-0000c2d0: 3504 4004 4804 5104 3d08 0000 0000 0600  5.@.H.Q.=.......
-0000c2e0: 0000 1445 5349 4120 6c6f 6769 6e20 636f  ...ESIA login co
-0000c2f0: 6d70 6c65 7465 6407 0000 0012 5265 7175  mpleted.....Requ
-0000c300: 6573 7449 6e74 6572 6365 7074 6f72 0103  estInterceptor..
-0000c310: 0000 000a 0410 043a 0442 0438 0432 0800  .......:.B.8.2..
-0000c320: 0000 0006 0000 0005 4173 7365 7407 0000  ........Asset...
-0000c330: 000c 5265 7375 6c74 734d 6f64 656c 0103  ..ResultsModel..
-0000c340: 0000 000c 041a 043e 043b 002d 0432 043e  .......>.;.-.2.>
-0000c350: 0800 0000 0006 0000 0003 5174 7907 0000  ..........Qty...
-0000c360: 000c 5265 7375 6c74 734d 6f64 656c 0103  ..ResultsModel..
-0000c370: 0000 000e 0414 043e 043b 044f 002c 0020  .......>.;.O.,. 
-0000c380: 0025 0800 0000 0006 0000 0008 5368 6172  .%..........Shar
-0000c390: 652c 2025 0700 0000 0c52 6573 756c 7473  e, %.....Results
-0000c3a0: 4d6f 6465 6c01 0300 0000 3004 1204 4b04  Model.....0...K.
-0000c3b0: 3104 4004 3004 3d00 2004 3d04 3504 3a04  1.@.0.=. .=.5.:.
-0000c3c0: 3e04 4004 4004 3504 3a04 4204 3d04 4b04  >.@.@.5.:.B.=.K.
-0000c3d0: 3900 2004 4104 4704 5104 4208 0000 0000  9. .A.G.Q.B.....
-0000c3e0: 0600 0000 1849 6e76 616c 6964 2061 6363  .....Invalid acc
-0000c3f0: 6f75 6e74 2073 656c 6563 7465 6407 0000  ount selected...
-0000c400: 0013 5365 6c65 6374 4163 636f 756e 7444  ..SelectAccountD
-0000c410: 6961 6c6f 6701 0300 0000 2204 1d04 3804  ialog....."...8.
-0000c420: 4704 3504 3304 3e00 2004 3d04 3500 2004  G.5.3.>. .=.5. .
-0000c430: 3204 4b04 3104 4004 3004 3d04 3e08 0000  2.K.1.@.0.=.>...
-0000c440: 0000 0600 0000 0c4e 6f20 7365 6c65 6374  .......No select
-0000c450: 696f 6e07 0000 0013 5365 6c65 6374 4163  ion.....SelectAc
-0000c460: 636f 756e 7444 6961 6c6f 6701 0300 0000  countDialog.....
-0000c470: 4004 1f04 3e04 3604 3004 3b04 4304 3904  @...>.6.0.;.C.9.
-0000c480: 4104 4204 3000 2c00 2004 3204 4b04 3104  A.B.0.,. .2.K.1.
-0000c490: 3504 4004 3804 4204 3500 2004 3404 4004  5.@.8.B.5. .4.@.
-0000c4a0: 4304 3304 3e04 3900 2004 4104 4704 5104  C.3.>.9. .A.G.Q.
-0000c4b0: 4208 0000 0000 0600 0000 1f50 6c65 6173  B..........Pleas
-0000c4c0: 6520 7365 6c65 6374 2064 6966 6665 7265  e select differe
-0000c4d0: 6e74 2061 6363 6f75 6e74 0700 0000 1353  nt account.....S
-0000c4e0: 656c 6563 7441 6363 6f75 6e74 4469 616c  electAccountDial
-0000c4f0: 6f67 0103 0000 0030 041f 043e 0436 0430  og.....0...>.6.0
-0000c500: 043b 0443 0439 0441 0442 0430 0020 0432  .;.C.9.A.B.0. .2
-0000c510: 044b 0431 0435 0440 0438 0442 0435 0020  .K.1.5.@.8.B.5. 
-0000c520: 0441 0447 0451 0442 0800 0000 0006 0000  .A.G.Q.B........
-0000c530: 0015 506c 6561 7365 2073 656c 6563 7420  ..Please select 
-0000c540: 6163 636f 756e 7407 0000 0010 5365 6c65  account.....Sele
-0000c550: 6374 4163 636f 756e 7444 6c67 0103 0000  ctAccountDlg....
-0000c560: 0012 0421 043e 043e 0431 0449 0435 043d  ...!.>.>.1.I.5.=
-0000c570: 0438 0435 0800 0000 0006 0000 0009 5465  .8.5..........Te
-0000c580: 7874 4c61 6265 6c07 0000 0010 5365 6c65  xtLabel.....Sele
-0000c590: 6374 4163 636f 756e 7444 6c67 0103 0000  ctAccountDlg....
-0000c5a0: 0056 0418 0441 043f 043e 043b 044c 0437  .V...A.?.>.;.L.7
-0000c5b0: 043e 0432 0430 0442 044c 0020 044d 0442  .>.2.0.B.L. .M.B
-0000c5c0: 043e 0442 0020 0436 0435 0020 0441 0447  .>.B. .6.5. .A.G
-0000c5d0: 0451 0442 0020 0434 043b 044f 0020 0434  .Q.B. .4.;.O. .4
-0000c5e0: 0430 043d 043d 043e 0439 0020 0432 0430  .0.=.=.>.9. .2.0
-0000c5f0: 043b 044e 0442 044b 0800 0000 0006 0000  .;.N.B.K........
-0000c600: 0027 5573 6520 7468 6520 7361 6d65 2061  .'Use the same a
-0000c610: 6363 6f75 6e74 2066 6f72 2067 6976 656e  ccount for given
-0000c620: 2063 7572 7265 6e63 7907 0000 0010 5365   currency.....Se
-0000c630: 6c65 6374 4163 636f 756e 7444 6c67 0103  lectAccountDlg..
-0000c640: 0000 0024 0412 044b 0431 0435 0440 0438  ...$...K.1.5.@.8
-0000c650: 0442 0435 0020 043a 0430 0442 0435 0433  .B.5. .:.0.B.5.3
-0000c660: 043e 0440 0438 044e 0800 0000 0006 0000  .>.@.8.N........
-0000c670: 0016 506c 6561 7365 2073 656c 6563 7420  ..Please select 
-0000c680: 6361 7465 676f 7279 0700 0000 1453 656c  category.....Sel
-0000c690: 6563 7443 6174 6567 6f72 7944 6961 6c6f  ectCategoryDialo
-0000c6a0: 6701 0300 0000 2804 1204 4b04 3104 3504  g.....(...K.1.5.
-0000c6b0: 4004 3804 4204 3500 2004 3a04 3e04 3d04  @.8.B.5. .:.>.=.
-0000c6c0: 4204 4004 3004 3304 3504 3d04 4204 3008  B.@.0.3.5.=.B.0.
-0000c6d0: 0000 0000 0600 0000 1250 6c65 6173 6520  .........Please 
-0000c6e0: 7365 6c65 6374 2070 6565 7207 0000 0010  select peer.....
-0000c6f0: 5365 6c65 6374 5065 6572 4469 616c 6f67  SelectPeerDialog
-0000c700: 0103 0000 0022 041d 0438 0447 0435 0433  ....."...8.G.5.3
-0000c710: 043e 0020 043d 0435 0020 0432 044b 0431  .>. .=.5. .2.K.1
-0000c720: 0440 0430 043d 043e 0800 0000 0006 0000  .@.0.=.>........
-0000c730: 000c 4e6f 2073 656c 6563 7469 6f6e 0700  ..No selection..
-0000c740: 0000 1553 656c 6563 7452 6566 6572 656e  ...SelectReferen
-0000c750: 6365 4469 616c 6f67 0103 0000 002e 0412  ceDialog........
-0000c760: 044b 0020 0434 043e 043b 0436 043d 044b  .K. .4.>.;.6.=.K
-0000c770: 0020 0441 0434 0435 043b 0430 0442 044c  . .A.4.5.;.0.B.L
-0000c780: 0020 0432 044b 0431 043e 0440 0800 0000  . .2.K.1.>.@....
-0000c790: 0006 0000 001b 596f 7520 7368 6f75 6c64  ......You should
-0000c7a0: 2073 656c 6563 7420 736f 6d65 7468 696e   select somethin
-0000c7b0: 6707 0000 0015 5365 6c65 6374 5265 6665  g.....SelectRefe
-0000c7c0: 7265 6e63 6544 6961 6c6f 6701 0300 0000  renceDialog.....
-0000c7d0: 1c04 1204 4b04 3104 3504 4004 3804 4204  ....K.1.5.@.8.B.
-0000c7e0: 3500 2004 3c04 3504 4204 3a04 4308 0000  5. .<.5.B.:.C...
-0000c7f0: 0000 0600 0000 1150 6c65 6173 6520 7365  .......Please se
-0000c800: 6c65 6374 2074 6167 0700 0000 0f53 656c  lect tag.....Sel
-0000c810: 6563 7454 6167 4469 616c 6f67 0103 0000  ectTagDialog....
-0000c820: 005a 041d 0435 0020 0443 0434 0430 043b  .Z...5. .C.4.0.;
-0000c830: 043e 0441 044c 0020 043f 043e 043b 0443  .>.A.L. .?.>.;.C
-0000c840: 0447 0438 0442 044c 0020 043d 0430 0437  .G.8.B.L. .=.0.7
-0000c850: 0432 0430 043d 0438 0435 0020 043e 0433  .2.0.=.8.5. .>.3
-0000c860: 0440 0430 043d 0438 0437 0430 0446 0438  .@.0.=.8.7.0.F.8
-0000c870: 0438 0020 0438 0437 003a 0020 0800 0000  .8. .8.7.:. ....
-0000c880: 0006 0000 001d 4361 6e27 7420 6765 7420  ......Can't get 
-0000c890: 636f 6d70 616e 7920 6e61 6d65 2066 726f  company name fro
-0000c8a0: 6d3a 2007 0000 000b 536c 6970 7354 6178  m: .....SlipsTax
-0000c8b0: 4150 4901 0300 0000 4804 1d04 3504 3204  API.....H...5.2.
-0000c8c0: 3e04 3704 3c04 3e04 3604 3d04 3e00 2004  >.7.<.>.6.=.>. .
-0000c8d0: 3e04 3104 3204 3d04 3e04 3204 3804 4204  >.1.2.=.>.2.8.B.
-0000c8e0: 4c00 2004 4104 3504 4104 4104 3804 4e00  L. .A.5.A.A.8.N.
-0000c8f0: 2c00 2004 3e04 4204 3204 3504 4200 3a00  ,. .>.B.2.5.B.:.
-0000c900: 2008 0000 0000 0600 0000 2143 616e 2774   .........!Can't
-0000c910: 2072 6566 7265 7368 2073 6573 7369 6f6e   refresh session
-0000c920: 2c20 7265 7370 6f6e 7365 3a20 0700 0000  , response: ....
-0000c930: 0b53 6c69 7073 5461 7841 5049 0103 0000  .SlipsTaxAPI....
-0000c940: 002e 041e 0448 0438 0431 043a 0430 0020  .....H.8.1.:.0. 
-0000c950: 043f 043e 043b 0443 0447 0435 043d 0438  .?.>.;.C.G.5.=.8
-0000c960: 044f 0020 0447 0435 043a 0430 003a 0020  .O. .G.5.:.0.:. 
-0000c970: 0800 0000 0006 0000 0013 4765 7420 7469  ..........Get ti
-0000c980: 636b 6574 2066 6169 6c65 643a 2007 0000  cket failed: ...
-0000c990: 000b 536c 6970 7354 6178 4150 4901 0300  ..SlipsTaxAPI...
-0000c9a0: 0000 3404 1e04 4804 3804 3104 3a04 3000  ..4...H.8.1.:.0.
-0000c9b0: 2004 3f04 3e04 3b04 4304 4704 3504 3d04   .?.>.;.C.G.5.=.
-0000c9c0: 3804 4f00 2000 6900 6400 2004 4704 3504  8.O. .i.d. .G.5.
-0000c9d0: 3a04 3000 3a00 2008 0000 0000 0600 0000  :.0.:. .........
-0000c9e0: 1647 6574 2074 6963 6b65 7420 6964 2066  .Get ticket id f
-0000c9f0: 6169 6c65 643a 2007 0000 000b 536c 6970  ailed: .....Slip
-0000ca00: 7354 6178 4150 4901 0300 0000 7c04 1d04  sTaxAPI.....|...
-0000ca10: 3504 3204 3504 4004 3d04 3004 4f00 2004  5.2.5.@.=.0.O. .
-0000ca20: 3404 3b04 3804 3d04 3000 2004 1804 1d04  4.;.8.=.0. .....
-0000ca30: 1d00 2e00 2004 1d04 3504 3204 3e04 3704  .... ...5.2.>.7.
-0000ca40: 3c04 3e04 3604 3d04 3e00 2004 3f04 3e04  <.>.6.=.>. .?.>.
-0000ca50: 3b04 4304 4704 3804 4204 4c00 2004 3d04  ;.C.G.8.B.L. .=.
-0000ca60: 3004 3804 3c04 3504 3d04 3e04 3204 3004  0.8.<.5.=.>.2.0.
-0000ca70: 3d04 3804 3500 2004 3a04 3e04 3c04 3f04  =.8.5. .:.>.<.?.
-0000ca80: 3004 3d04 3804 3800 2e08 0000 0000 0600  0.=.8.8.........
-0000ca90: 0000 3049 6e63 6f72 7265 6374 206c 656e  ..0Incorrect len
-0000caa0: 6774 6820 6f66 2049 4e4e 2e20 4361 6e27  gth of INN. Can'
-0000cab0: 7420 6765 7420 636f 6d70 616e 7920 6e61  t get company na
-0000cac0: 6d65 2e07 0000 000b 536c 6970 7354 6178  me......SlipsTax
-0000cad0: 4150 4901 0300 0000 5604 1d04 3504 4200  API.....V...5.B.
-0000cae0: 2000 5300 6500 7300 7300 6900 6f00 6e00   .S.e.s.s.i.o.n.
-0000caf0: 4900 6400 2004 3404 3b04 4f00 2004 3704  I.d. .4.;.O. .7.
-0000cb00: 3004 3304 4004 4304 3704 3a04 3800 2004  0.3.@.C.7.:.8. .
-0000cb10: 4704 3504 3a04 3000 2004 4100 2004 4104  G.5.:.0. .A. .A.
-0000cb20: 3004 3904 4204 3000 2004 2404 1d04 2108  0.9.B.0. .$...!.
-0000cb30: 0000 0000 0600 0000 224e 6f20 5275 7373  ........"No Russ
-0000cb40: 6961 6e20 5461 7820 5365 7373 696f 6e49  ian Tax SessionI
-0000cb50: 6420 6176 6169 6c61 626c 6507 0000 000b  d available.....
-0000cb60: 536c 6970 7354 6178 4150 4901 0300 0000  SlipsTaxAPI.....
-0000cb70: 3604 1d04 3504 4200 2004 3004 3a04 4204  6...5.B. .0.:.B.
-0000cb80: 3804 3204 3d04 3e04 3900 2004 4104 3504  8.2.=.>.9. .A.5.
-0000cb90: 4104 4104 3804 3800 2004 3404 3b04 4f00  A.A.8.8. .4.;.O.
-0000cba0: 2004 2404 1d04 2108 0000 0000 0600 0000   .$...!.........
-0000cbb0: 184e 6f20 7661 6c69 6420 7365 7373 696f  .No valid sessio
-0000cbc0: 6e20 7072 6573 656e 7407 0000 000b 536c  n present.....Sl
-0000cbd0: 6970 7354 6178 4150 4901 0300 0000 7a04  ipsTaxAPI.....z.
-0000cbe0: 1e04 3f04 3504 4004 3004 4604 3804 4f00  ..?.5.@.0.F.8.O.
-0000cbf0: 2004 3e04 3104 4004 3004 3104 3004 4204   .>.1.@.0.1.0.B.
-0000cc00: 4b04 3204 3004 3504 4204 4104 4f00 2004  K.2.0.5.B.A.O. .
-0000cc10: 3d04 3000 2004 4104 4204 3e04 4004 3e04  =.0. .A.B.>.@.>.
-0000cc20: 3d04 3500 2004 4104 3504 4004 3204 3504  =.5. .A.5.@.2.5.
-0000cc30: 4004 3000 2e00 2004 1f04 3e04 3204 4204  @.0... ...>.2.B.
-0000cc40: 3e04 4004 4f04 4e00 2004 3504 4904 5100  >.@.O.N. .5.I.Q.
-0000cc50: 2004 4004 3004 3700 2e08 0000 0000 0600   .@.0.7.........
-0000cc60: 0000 384f 7065 7261 7469 6f6e 206d 6967  ..8Operation mig
-0000cc70: 6874 2062 6520 7065 6e64 696e 6720 6f6e  ht be pending on
-0000cc80: 2073 6572 7665 7220 7369 6465 2e20 5472   server side. Tr
-0000cc90: 7969 6e67 2061 6761 696e 2e07 0000 000b  ying again......
-0000cca0: 536c 6970 7354 6178 4150 4901 0300 0000  SlipsTaxAPI.....
-0000ccb0: 2804 1e04 3104 3d04 3e04 3204 3b04 3504  (...1.=.>.2.;.5.
-0000ccc0: 3d04 3804 3500 2004 4104 3504 4104 4104  =.8.5. .A.5.A.A.
-0000ccd0: 3804 3800 2e00 2e00 2e08 0000 0000 0600  8.8.............
-0000cce0: 0000 1552 6566 7265 7368 696e 6720 7365  ...Refreshing se
-0000ccf0: 7373 696f 6e2e 2e2e 0700 0000 0b53 6c69  ssion........Sli
-0000cd00: 7073 5461 7841 5049 0103 0000 0024 0421  psTaxAPI.....$.!
-0000cd10: 0435 0441 0441 0438 044f 0020 043e 0431  .5.A.A.8.O. .>.1
-0000cd20: 043d 043e 0432 043b 0435 043d 0430 003a  .=.>.2.;.5.=.0.:
-0000cd30: 0020 0800 0000 0006 0000 0013 5365 7373  . ..........Sess
-0000cd40: 696f 6e20 7265 6672 6573 6865 643a 2007  ion refreshed: .
-0000cd50: 0000 000b 536c 6970 7354 6178 4150 4901  ....SlipsTaxAPI.
-0000cd60: 0300 0000 1804 2704 3504 3a00 2004 3d04  ......'.5.:. .=.
-0000cd70: 3004 3904 3404 3504 3d00 3a00 2008 0000  0.9.4.5.=.:. ...
-0000cd80: 0000 0600 0000 0c53 6c69 7020 666f 756e  .......Slip foun
-0000cd90: 643a 2007 0000 000b 536c 6970 7354 6178  d: .....SlipsTax
-0000cda0: 4150 4901 0300 0000 1c04 2704 3504 3a00  API.......'.5.:.
-0000cdb0: 2004 3704 3004 3304 4004 4304 3604 3504   .7.0.3.@.C.6.5.
-0000cdc0: 3d00 3a00 2008 0000 0000 0600 0000 0d53  =.:. ..........S
-0000cdd0: 6c69 7020 6c6f 6164 6564 3a20 0700 0000  lip loaded: ....
-0000cde0: 0b53 6c69 7073 5461 7841 5049 0103 0000  .SlipsTaxAPI....
-0000cdf0: 0036 041d 0435 0430 0432 0442 043e 0440  .6...5.0.2.B.>.@
-0000ce00: 0438 0437 043e 0432 0430 043d 043e 0020  .8.7.>.2.0.=.>. 
-0000ce10: 043f 043e 0020 043f 0440 0438 0447 0438  .?.>. .?.@.8.G.8
-0000ce20: 043d 0435 003a 0020 0800 0000 0006 0000  .=.5.:. ........
-0000ce30: 001a 556e 6175 7468 6f72 697a 6564 2077  ..Unauthorized w
-0000ce40: 6974 6820 7265 6173 6f6e 3a20 0700 0000  ith reason: ....
-0000ce50: 0b53 6c69 7073 5461 7841 5049 0103 0000  .SlipsTaxAPI....
-0000ce60: 001c 0421 0447 0451 0442 0020 043d 0435  ...!.G.Q.B. .=.5
-0000ce70: 0020 0432 044b 0431 0440 0430 043d 0800  . .2.K.1.@.0.=..
-0000ce80: 0000 0006 0000 0014 4163 636f 756e 7420  ........Account 
-0000ce90: 6e6f 7420 7365 6c65 6374 6564 0700 0000  not selected....
-0000cea0: 0953 7461 7465 6d65 6e74 0103 0000 0034  .Statement.....4
-0000ceb0: 0414 0430 043d 043d 044b 0435 0020 043d  ...0.=.=.K.5. .=
-0000cec0: 0435 0020 043f 0440 0438 0432 044f 0437  .5. .?.@.8.2.O.7
-0000ced0: 0430 043d 044b 0020 043a 0020 0426 0411  .0.=.K. .:. .&..
-0000cee0: 003a 0020 0800 0000 0006 0000 0023 4173  .:. .........#As
-0000cef0: 7365 7420 6461 7461 2061 7265 6e27 7420  set data aren't 
-0000cf00: 6c69 6e6b 6564 2074 6f20 6173 7365 743a  linked to asset:
-0000cf10: 2007 0000 0009 5374 6174 656d 656e 7401   .....Statement.
-0000cf20: 0300 0000 1e04 2604 1100 2000 6900 6400  ......&... .i.d.
-0000cf30: 2004 3d04 3500 2004 3d04 3004 3904 3404   .=.5. .=.0.9.4.
-0000cf40: 3504 3d08 0000 0000 0600 0000 1241 7373  5.=..........Ass
-0000cf50: 6574 2069 6420 6e6f 7420 666f 756e 6407  et id not found.
-0000cf60: 0000 0009 5374 6174 656d 656e 7401 0300  ....Statement...
-0000cf70: 0000 3204 1d04 3504 3204 3e04 3704 3c04  ..2...5.2.>.7.<.
-0000cf80: 3e04 3604 3d04 3e00 2004 4104 3e04 3704  >.6.=.>. .A.>.7.
-0000cf90: 3404 3004 4204 4c00 2004 4104 4704 5104  4.0.B.L. .A.G.Q.
-0000cfa0: 4200 3a00 2008 0000 0000 0600 0000 1643  B.:. ..........C
-0000cfb0: 616e 2774 2063 7265 6174 6520 6163 636f  an't create acco
-0000cfc0: 756e 743a 2007 0000 0009 5374 6174 656d  unt: .....Statem
-0000cfd0: 656e 7401 0300 0000 2e04 1d04 3504 3204  ent.........5.2.
-0000cfe0: 3e04 3704 3c04 3e04 3604 3d04 3e00 2004  >.7.<.>.6.=.>. .
-0000cff0: 4104 3e04 3704 3404 3004 4204 4c00 2004  A.>.7.4.0.B.L. .
-0000d000: 2604 1100 3a00 2008 0000 0000 0600 0000  &...:. .........
-0000d010: 1443 616e 2774 2063 7265 6174 6520 6173  .Can't create as
-0000d020: 7365 743a 2007 0000 0009 5374 6174 656d  set: .....Statem
-0000d030: 656e 7401 0300 0000 3c04 1d04 3504 3204  ent.....<...5.2.
-0000d040: 3e04 3704 3c04 3e04 3604 3d04 3e00 2004  >.7.<.>.6.=.>. .
-0000d050: 3d04 3004 3904 4204 3500 2004 2604 1100  =.0.9.B.5. .&...
-0000d060: 2004 3200 2004 3e04 4204 4704 5104 4204   .2. .>.B.G.Q.B.
-0000d070: 3500 3a00 2008 0000 0000 0600 0000 2643  5.:. .........&C
-0000d080: 616e 2774 206c 6f63 6174 6520 6173 7365  an't locate asse
-0000d090: 7420 696e 2073 7461 7465 6d65 6e74 2064  t in statement d
-0000d0a0: 6174 613a 2007 0000 0009 5374 6174 656d  ata: .....Statem
-0000d0b0: 656e 7401 0300 0000 1a04 1f04 3e04 3404  ent.........>.4.
-0000d0c0: 4204 3204 3504 4004 3604 3404 3504 3d04  B.2.5.@.6.4.5.=.
-0000d0d0: 3804 3508 0000 0000 0600 0000 0c43 6f6e  8.5..........Con
-0000d0e0: 6669 726d 6174 696f 6e07 0000 0009 5374  firmation.....St
-0000d0f0: 6174 656d 656e 7401 0300 0000 4404 1e04  atement.....D...
-0000d100: 4204 3b04 3004 3404 3e04 4704 3d04 3004  B.;.0.4.>.G.=.0.
-0000d110: 4f00 2004 3804 3d04 4404 3e04 4004 3c04  O. .8.=.D.>.@.<.
-0000d120: 3004 4604 3804 4f00 2004 4104 3e04 4504  0.F.8.O. .A.>.E.
-0000d130: 4004 3004 3d04 3504 3d04 3000 2004 3200  @.0.=.5.=.0. .2.
-0000d140: 2008 0000 0000 0600 0000 1e44 6562 7567   ..........Debug
-0000d150: 2069 6e66 6f72 6d61 7469 6f6e 2069 7320   information is 
-0000d160: 7361 7665 6420 696e 2007 0000 0009 5374  saved in .....St
-0000d170: 6174 656d 656e 7401 0300 0000 1004 1404  atement.........
-0000d180: 3504 3f04 3e04 3704 3804 4200 2008 0000  5.?.>.7.8.B. ...
-0000d190: 0000 0600 0000 0b44 6570 6f73 6974 206f  .......Deposit o
-0000d1a0: 6620 0700 0000 0953 7461 7465 6d65 6e74  f .....Statement
-0000d1b0: 0103 0000 0048 041d 0435 0432 043e 0437  .....H...5.2.>.7
-0000d1c0: 043c 043e 0436 043d 043e 0020 043f 0440  .<.>.6.=.>. .?.@
-0000d1d0: 043e 0447 0438 0442 0430 0442 044c 0020  .>.G.8.B.0.B.L. 
-0000d1e0: 004a 0053 004f 004e 0020 0438 0437 0020  .J.S.O.N. .8.7. 
-0000d1f0: 0444 0430 0439 043b 0430 003a 0020 0800  .D.0.9.;.0.:. ..
-0000d200: 0000 0006 0000 001f 4661 696c 6564 2074  ........Failed t
-0000d210: 6f20 7265 6164 204a 534f 4e20 6672 6f6d  o read JSON from
-0000d220: 2066 696c 653a 2007 0000 0009 5374 6174   file: .....Stat
-0000d230: 656d 656e 7401 0300 0000 4804 1d04 3500  ement.....H...5.
-0000d240: 2004 4304 3404 3004 3b04 3e04 4104 4c00   .C.4.0.;.>.A.L.
-0000d250: 2004 3f04 4004 3e04 4704 3804 4204 3004   .?.@.>.G.8.B.0.
-0000d260: 4204 4c00 2004 4104 4504 3504 3c04 4300  B.L. .A.E.5.<.C.
-0000d270: 2000 4a00 5300 4f00 4e00 2004 3804 3700   .J.S.O.N. .8.7.
-0000d280: 3a00 2008 0000 0000 0600 0000 2146 6169  :. .........!Fai
-0000d290: 6c65 6420 746f 2072 6561 6420 4a53 4f4e  led to read JSON
-0000d2a0: 2073 6368 656d 6120 6672 6f6d 3a20 0700   schema from: ..
-0000d2b0: 0000 0953 7461 7465 6d65 6e74 0103 0000  ...Statement....
-0000d2c0: 0034 041d 0435 0432 043e 0437 043c 043e  .4...5.2.>.7.<.>
-0000d2d0: 0436 043d 043e 0020 043f 0440 043e 0447  .6.=.>. .?.@.>.G
-0000d2e0: 0435 0441 0442 044c 0020 0444 0430 0439  .5.A.B.L. .D.0.9
-0000d2f0: 043b 003a 0020 0800 0000 0006 0000 0015  .;.:. ..........
-0000d300: 4661 696c 6564 2074 6f20 7265 6164 2066  Failed to read f
-0000d310: 696c 653a 2007 0000 0009 5374 6174 656d  ile: .....Statem
-0000d320: 656e 7401 0300 0000 5a04 1e04 4804 3804  ent.....Z...H.8.
-0000d330: 3104 3a04 3000 2004 3f04 4004 3800 2004  1.:.0. .?.@.8. .
-0000d340: 4104 3e04 4504 4004 3004 3d04 3504 3d04  A.>.E.@.0.=.5.=.
-0000d350: 3804 3800 2004 3e04 4204 3b04 3004 3404  8.8. .>.B.;.0.4.
-0000d360: 3e04 4704 3d04 3e04 3900 2004 3804 3d04  >.G.=.>.9. .8.=.
-0000d370: 4404 3e04 4004 3c04 3004 4604 3804 3800  D.>.@.<.0.F.8.8.
-0000d380: 3a00 2008 0000 0000 0600 0000 2546 6169  :. .........%Fai
-0000d390: 6c65 6420 746f 2077 7269 7465 2073 7461  led to write sta
-0000d3a0: 7465 6d65 6e74 2064 756d 7020 696e 746f  tement dump into
-0000d3b0: 3a20 0700 0000 0953 7461 7465 6d65 6e74  : .....Statement
-0000d3c0: 0103 0000 0066 041d 0435 0432 043e 0437  .....f...5.2.>.7
-0000d3d0: 043c 043e 0436 043d 043e 0020 043a 043e  .<.>.6.=.>. .:.>
-0000d3e0: 043d 0442 0432 0435 0440 0442 0438 0440  .=.B.2.5.@.B.8.@
-0000d3f0: 043e 0432 0430 0442 044c 0020 0442 0438  .>.2.0.B.L. .B.8
-0000d400: 043f 0020 0430 043a 0442 0438 0432 0430  .?. .0.:.B.8.2.0
-0000d410: 0020 0432 0020 0442 0440 0430 043d 0441  . .2. .B.@.0.=.A
-0000d420: 0444 0435 0440 0435 003a 0020 0800 0000  .D.5.@.5.:. ....
-0000d430: 0006 0000 002e 496d 706f 7373 6962 6c65  ......Impossible
-0000d440: 2074 6f20 636f 6e76 6572 7420 6173 7365   to convert asse
-0000d450: 7420 7479 7065 2069 6e20 7472 616e 7366  t type in transf
-0000d460: 6572 3a20 0700 0000 0953 7461 7465 6d65  er: .....Stateme
-0000d470: 6e74 0103 0000 0048 041d 0435 043e 0434  nt.....H...5.>.4
-0000d480: 043d 043e 0437 043d 0430 0447 043d 043e  .=.>.7.=.0.G.=.>
-0000d490: 0435 0020 0441 043e 0432 043f 0430 0434  .5. .A.>.2.?.0.4
-0000d4a0: 0435 043d 0438 0435 0020 0432 0430 043b  .5.=.8.5. .2.0.;
-0000d4b0: 044e 0442 044b 0020 0434 043b 044f 0020  .N.B.K. .4.;.O. 
-0000d4c0: 0800 0000 0006 0000 001c 4d75 6c74 6970  ..........Multip
-0000d4d0: 6c65 2063 7572 7265 6e63 7920 6d61 7463  le currency matc
-0000d4e0: 6820 666f 7220 0700 0000 0953 7461 7465  h for .....State
-0000d4f0: 6d65 6e74 0103 0000 003a 041d 0435 043e  ment.....:...5.>
-0000d500: 0434 043d 043e 0437 043d 0430 0447 043d  .4.=.>.7.=.0.G.=
-0000d510: 043e 0435 0020 0441 043e 0432 043f 0430  .>.5. .A.>.2.?.0
-0000d520: 0434 0435 043d 0438 0435 0020 0434 043b  .4.5.=.8.5. .4.;
-0000d530: 044f 0020 0800 0000 0006 0000 0013 4d75  .O. ..........Mu
-0000d540: 6c74 6970 6c65 206d 6174 6368 2066 6f72  ltiple match for
-0000d550: 2007 0000 0009 5374 6174 656d 656e 7401   .....Statement.
-0000d560: 0300 0000 3a04 1204 4b04 3104 3504 4004  ....:...K.1.5.@.
-0000d570: 3804 4204 3500 2004 4104 4704 5104 4200  8.B.5. .A.G.Q.B.
-0000d580: 2004 3404 3b04 4f00 2004 3704 3004 4704   .4.;.O. .7.0.G.
-0000d590: 3804 4104 3b04 3504 3d04 3804 4f00 3a08  8.A.;.5.=.8.O.:.
-0000d5a0: 0000 0000 0600 0000 1d53 656c 6563 7420  .........Select 
-0000d5b0: 6163 636f 756e 7420 746f 2064 6570 6f73  account to depos
-0000d5c0: 6974 2074 6f3a 0700 0000 0953 7461 7465  it to:.....State
-0000d5d0: 6d65 6e74 0103 0000 0036 0412 044b 0431  ment.....6...K.1
-0000d5e0: 0435 0440 0438 0442 0435 0020 0441 0447  .5.@.8.B.5. .A.G
-0000d5f0: 0451 0442 0020 0434 043b 044f 0020 0441  .Q.B. .4.;.O. .A
-0000d600: 043f 0438 0441 0430 043d 0438 044f 003a  .?.8.A.0.=.8.O.:
-0000d610: 0800 0000 0006 0000 0020 5365 6c65 6374  ......... Select
-0000d620: 2061 6363 6f75 6e74 2074 6f20 7769 7468   account to with
-0000d630: 6472 6177 2066 726f 6d3a 0700 0000 0953  draw from:.....S
-0000d640: 7461 7465 6d65 6e74 0103 0000 0048 041d  tatement.....H..
-0000d650: 0435 043a 043e 0442 043e 0440 044b 0435  .5.:.>.B.>.@.K.5
-0000d660: 0020 0441 0435 043a 0446 0438 0438 0020  . .A.5.:.F.8.8. 
-0000d670: 043d 0435 0020 043f 043e 0434 0434 0435  .=.5. .?.>.4.4.5
-0000d680: 0440 0436 0438 0432 0430 044e 0442 0441  .@.6.8.2.0.N.B.A
-0000d690: 044f 003a 0020 0800 0000 0006 0000 0021  .O.:. .........!
-0000d6a0: 536f 6d65 2073 6563 7469 6f6e 7320 6172  Some sections ar
-0000d6b0: 6520 6e6f 7420 7375 7070 6f72 7465 643a  e not supported:
-0000d6c0: 2007 0000 0009 5374 6174 656d 656e 7401   .....Statement.
-0000d6d0: 0300 0000 2a04 1804 3c04 3f04 3e04 4004  ....*...<.?.>.@.
-0000d6e0: 4200 2004 3e04 4204 4704 5104 4204 3000  B. .>.B.G.Q.B.0.
-0000d6f0: 2004 3f04 4004 3504 4004 3204 3004 3d08   .?.@.5.@.2.0.=.
-0000d700: 0000 0000 0600 0000 1e53 7461 7465 6d65  .........Stateme
-0000d710: 6e74 2069 6d70 6f72 7420 7761 7320 6361  nt import was ca
-0000d720: 6e63 656c 6c65 6407 0000 0009 5374 6174  ncelled.....Stat
-0000d730: 656d 656e 7401 0300 0000 2c04 1d04 3504  ement.....,...5.
-0000d740: 3204 3504 4004 3d04 4b04 3900 2004 3f04  2.5.@.=.K.9. .?.
-0000d750: 3504 4004 3804 3e04 3400 2004 3e04 4204  5.@.8.>.4. .>.B.
-0000d760: 4704 5104 4204 3008 0000 0000 0600 0000  G.Q.B.0.........
-0000d770: 1b53 7461 7465 6d65 6e74 2070 6572 696f  .Statement perio
-0000d780: 6420 6973 2069 6e76 616c 6964 0700 0000  d is invalid....
-0000d790: 0953 7461 7465 6d65 6e74 0103 0000 00c6  .Statement......
-0000d7a0: 041f 0435 0440 0438 043e 0434 0020 043e  ...5.@.8.>.4. .>
-0000d7b0: 0442 0447 0451 0442 0430 0020 043d 0430  .B.G.Q.B.0. .=.0
-0000d7c0: 0447 0438 043d 0430 0435 0442 0441 044f  .G.8.=.0.5.B.A.O
-0000d7d0: 0020 0440 0430 043d 0435 0435 0020 043f  . .@.0.=.5.5. .?
-0000d7e0: 043e 0441 043b 0435 0434 043d 0435 0439  .>.A.;.5.4.=.5.9
-0000d7f0: 0020 043e 043f 0435 0440 0430 0446 0438  . .>.?.5.@.0.F.8
-0000d800: 0438 0020 0434 043b 044f 0020 0441 0447  .8. .4.;.O. .A.G
-0000d810: 0451 0442 0430 0020 0028 043f 043e 0432  .Q.B.0. .(.?.>.2
-0000d820: 0442 043e 0440 043d 044b 0439 0020 0438  .B.>.@.=.K.9. .8
-0000d830: 043c 043f 043e 0440 0442 003f 0029 002e  .<.?.>.@.B.?.)..
-0000d840: 0020 041f 0440 043e 0434 043e 043b 0436  . ...@.>.4.>.;.6
-0000d850: 0438 0442 044c 0020 0438 043c 043f 043e  .8.B.L. .8.<.?.>
-0000d860: 0440 0442 003f 0800 0000 0006 0000 0058  .@.B.?.........X
-0000d870: 5374 6174 656d 656e 7420 7065 7269 6f64  Statement period
-0000d880: 2073 7461 7274 7320 6265 666f 7265 206c   starts before l
-0000d890: 6173 7420 7265 636f 7264 6564 206f 7065  ast recorded ope
-0000d8a0: 7261 7469 6f6e 2066 6f72 2074 6865 2061  ration for the a
-0000d8b0: 6363 6f75 6e74 2e20 436f 6e74 696e 7565  ccount. Continue
-0000d8c0: 2069 6d70 6f72 743f 0700 0000 0953 7461   import?.....Sta
-0000d8d0: 7465 6d65 6e74 0103 0000 002a 041e 0442  tement.....*...B
-0000d8e0: 0447 0451 0442 0020 0441 043e 0434 0435  .G.Q.B. .A.>.4.5
-0000d8f0: 0440 0436 0438 0442 0020 043e 0448 0438  .@.6.8.B. .>.H.8
-0000d900: 0431 043a 0438 0800 0000 0006 0000 001b  .1.:.8..........
-0000d910: 5374 6174 656d 656e 7420 7661 6c69 6461  Statement valida
-0000d920: 7469 6f6e 2066 6169 6c65 6407 0000 0009  tion failed.....
-0000d930: 5374 6174 656d 656e 7401 0300 0000 4004  Statement.....@.
-0000d940: 2104 3804 3c04 3204 3e04 3b00 2004 3204  !.8.<.2.>.;. .2.
-0000d950: 3004 3b04 4e04 4204 4b00 2004 3d04 3500  0.;.N.B.K. .=.5.
-0000d960: 2004 3f04 4004 3804 3204 4f04 3704 3004   .?.@.8.2.O.7.0.
-0000d970: 3d00 2004 3a00 2004 2604 1100 3a00 2008  =. .:. .&...:. .
-0000d980: 0000 0000 0600 0000 2753 796d 626f 6c20  ........'Symbol 
-0000d990: 6375 7272 656e 6379 2069 736e 2774 206c  currency isn't l
-0000d9a0: 696e 6b65 6420 746f 2061 7373 6574 3a20  inked to asset: 
-0000d9b0: 0700 0000 0953 7461 7465 6d65 6e74 0103  .....Statement..
-0000d9c0: 0000 0032 0421 0438 043c 0432 043e 043b  ...2.!.8.<.2.>.;
-0000d9d0: 0020 043d 0435 0020 043f 0440 0438 0432  . .=.5. .?.@.8.2
-0000d9e0: 044f 0437 0430 043d 0020 043a 0020 0426  .O.7.0.=. .:. .&
-0000d9f0: 0411 003a 0020 0800 0000 0006 0000 0025  ...:. .........%
-0000da00: 5379 6d62 6f6c 2074 6963 6b65 7220 6973  Symbol ticker is
-0000da10: 6e27 7420 6c69 6e6b 6564 2074 6f20 6173  n't linked to as
-0000da20: 7365 743a 2007 0000 0009 5374 6174 656d  set: .....Statem
-0000da30: 656e 7401 0300 0000 7204 1d04 3504 3204  ent.....r...5.2.
-0000da40: 3e04 3704 3c04 3e04 3604 3d04 3e00 2004  >.7.<.>.6.=.>. .
-0000da50: 4104 3e04 3f04 3e04 4104 4204 3004 3204  A.>.?.>.A.B.0.2.
-0000da60: 3804 4204 4c00 2004 4104 4704 5104 4200  8.B.L. .A.G.Q.B.
-0000da70: 2004 3404 3b04 4f00 2004 3a04 3e04 4004   .4.;.O. .:.>.@.
-0000da80: 3f04 3e04 4004 3004 4204 3804 3204 3d04  ?.>.@.0.B.8.2.=.
-0000da90: 3e04 3304 3e00 2004 3404 3504 3904 4104  >.3.>. .4.5.9.A.
-0000daa0: 4204 3204 3804 4f00 3a00 2008 0000 0000  B.2.8.O.:. .....
-0000dab0: 0600 0000 2855 6e6d 6174 6368 6564 2061  ....(Unmatched a
-0000dac0: 6363 6f75 6e74 2066 6f72 2063 6f72 706f  ccount for corpo
-0000dad0: 7261 7465 2061 6374 696f 6e3a 2007 0000  rate action: ...
-0000dae0: 0009 5374 6174 656d 656e 7401 0300 0000  ..Statement.....
-0000daf0: 7404 1d04 3504 3204 3e04 3704 3c04 3e04  t...5.2.>.7.<.>.
-0000db00: 3604 3d04 3e00 2004 4104 3e04 3f04 3e04  6.=.>. .A.>.?.>.
-0000db10: 4104 4204 3004 3204 3804 4204 4c00 2004  A.B.0.2.8.B.L. .
-0000db20: 4104 4704 5104 4200 2004 3404 3b04 4f00  A.G.Q.B. .4.;.O.
-0000db30: 2004 3e04 3f04 3504 4004 3004 4604 3804   .>.?.5.@.0.F.8.
-0000db40: 3800 2004 3f04 4004 3804 4504 3e04 3404  8. .?.@.8.E.>.4.
-0000db50: 3000 2f04 4004 3004 4104 4504 3e04 3404  0./.@.0.A.E.>.4.
-0000db60: 3000 3a00 2008 0000 0000 0600 0000 2755  0.:. .........'U
-0000db70: 6e6d 6174 6368 6564 2061 6363 6f75 6e74  nmatched account
-0000db80: 2066 6f72 2069 6e63 6f6d 652f 7370 656e   for income/spen
-0000db90: 6469 6e67 3a20 0700 0000 0953 7461 7465  ding: .....State
-0000dba0: 6d65 6e74 0103 0000 0052 041d 0435 0432  ment.....R...5.2
-0000dbb0: 043e 0437 043c 043e 0436 043d 043e 0020  .>.7.<.>.6.=.>. 
-0000dbc0: 0441 043e 043f 043e 0441 0442 0430 0432  .A.>.?.>.A.B.0.2
-0000dbd0: 0438 0442 044c 0020 0441 0447 0451 0442  .8.B.L. .A.G.Q.B
-0000dbe0: 0020 0434 043b 044f 0020 0432 044b 043f  . .4.;.O. .2.K.?
-0000dbf0: 043b 0430 0442 044b 003a 0020 0800 0000  .;.0.B.K.:. ....
-0000dc00: 0006 0000 001f 556e 6d61 7463 6865 6420  ......Unmatched 
-0000dc10: 6163 636f 756e 7420 666f 7220 7061 796d  account for paym
-0000dc20: 656e 743a 2007 0000 0009 5374 6174 656d  ent: .....Statem
-0000dc30: 656e 7401 0300 0000 5004 1d04 3504 3204  ent.....P...5.2.
-0000dc40: 3e04 3704 3c04 3e04 3604 3d04 3e00 2004  >.7.<.>.6.=.>. .
-0000dc50: 4104 3e04 3f04 3e04 4104 4204 3004 3204  A.>.?.>.A.B.0.2.
-0000dc60: 3804 4204 4c00 2004 4104 4704 5104 4200  8.B.L. .A.G.Q.B.
-0000dc70: 2004 3404 3b04 4f00 2004 4104 3404 3504   .4.;.O. .A.4.5.
-0000dc80: 3b04 3a04 3800 3a00 2008 0000 0000 0600  ;.:.8.:. .......
-0000dc90: 0000 1d55 6e6d 6174 6368 6564 2061 6363  ...Unmatched acc
-0000dca0: 6f75 6e74 2066 6f72 2074 7261 6465 3a20  ount for trade: 
-0000dcb0: 0700 0000 0953 7461 7465 6d65 6e74 0103  .....Statement..
-0000dcc0: 0000 0054 041d 0435 0432 0437 043e 043c  ...T...5.2.7.>.<
-0000dcd0: 043e 0436 043d 043e 0020 0441 043e 043f  .>.6.=.>. .A.>.?
-0000dce0: 043e 0441 0442 0430 0432 0438 0442 044c  .>.A.B.0.2.8.B.L
-0000dcf0: 0020 0441 0447 0451 0442 0020 0434 043b  . .A.G.Q.B. .4.;
-0000dd00: 044f 0020 043f 0435 0440 0435 0432 043e  .O. .?.5.@.5.2.>
-0000dd10: 0434 0430 003a 0020 0800 0000 0006 0000  .4.0.:. ........
-0000dd20: 0020 556e 6d61 7463 6865 6420 6163 636f  . Unmatched acco
-0000dd30: 756e 7420 666f 7220 7472 616e 7366 6572  unt for transfer
-0000dd40: 3a20 0700 0000 0953 7461 7465 6d65 6e74  : .....Statement
-0000dd50: 0103 0000 006e 041d 0435 0432 043e 0437  .....n...5.2.>.7
-0000dd60: 043c 043e 0436 043d 043e 0020 0441 043e  .<.>.6.=.>. .A.>
-0000dd70: 043f 043e 0441 0442 0430 0432 0438 0442  .?.>.A.B.0.2.8.B
-0000dd80: 044c 0020 0426 0411 0020 0434 043b 044f  .L. .&... .4.;.O
-0000dd90: 0020 043a 043e 0440 043f 043e 0440 0430  . .:.>.@.?.>.@.0
-0000dda0: 0442 0438 0432 043d 043e 0433 043e 0020  .B.8.2.=.>.3.>. 
-0000ddb0: 0434 0435 0439 0441 0442 0432 0438 044f  .4.5.9.A.B.2.8.O
-0000ddc0: 003a 0020 0800 0000 0006 0000 0026 556e  .:. .........&Un
-0000ddd0: 6d61 7463 6865 6420 6173 7365 7420 666f  matched asset fo
-0000dde0: 7220 636f 7270 6f72 6174 6520 6163 7469  r corporate acti
-0000ddf0: 6f6e 3a20 0700 0000 0953 7461 7465 6d65  on: .....Stateme
-0000de00: 6e74 0103 0000 004e 041d 0435 0432 043e  nt.....N...5.2.>
-0000de10: 0437 043c 043e 0436 043d 043e 0020 0441  .7.<.>.6.=.>. .A
-0000de20: 043e 043f 043e 0441 0442 0430 0432 0438  .>.?.>.A.B.0.2.8
-0000de30: 0442 044c 0020 0426 0411 0020 0434 043b  .B.L. .&... .4.;
-0000de40: 044f 0020 0432 044b 043f 043b 0430 0442  .O. .2.K.?.;.0.B
-0000de50: 044b 003a 0020 0800 0000 0006 0000 001d  .K.:. ..........
-0000de60: 556e 6d61 7463 6865 6420 6173 7365 7420  Unmatched asset 
-0000de70: 666f 7220 7061 796d 656e 743a 2007 0000  for payment: ...
-0000de80: 0009 5374 6174 656d 656e 7401 0300 0000  ..Statement.....
-0000de90: 4c04 1d04 3504 3204 3e04 3704 3c04 3e04  L...5.2.>.7.<.>.
-0000dea0: 3604 3d04 3e00 2004 4104 3e04 3f04 3e04  6.=.>. .A.>.?.>.
-0000deb0: 4104 4204 3004 3204 3804 4204 4c00 2004  A.B.0.2.8.B.L. .
-0000dec0: 2604 1100 2004 3404 3b04 4f00 2004 4104  &... .4.;.O. .A.
-0000ded0: 3404 3504 3b04 3a04 3800 3a00 2008 0000  4.5.;.:.8.:. ...
-0000dee0: 0000 0600 0000 1b55 6e6d 6174 6368 6564  .......Unmatched
-0000def0: 2061 7373 6574 2066 6f72 2074 7261 6465   asset for trade
-0000df00: 3a20 0700 0000 0953 7461 7465 6d65 6e74  : .....Statement
-0000df10: 0103 0000 005e 041d 0435 0432 043e 0437  .....^...5.2.>.7
-0000df20: 043c 043e 0436 043d 043e 0020 0441 043e  .<.>.6.=.>. .A.>
-0000df30: 043f 043e 0441 0442 0430 0432 0438 0442  .?.>.A.B.0.2.8.B
-0000df40: 044c 0020 0426 0411 002f 0432 0430 043b  .L. .&.../.2.0.;
-0000df50: 044e 0442 0443 0020 0434 043b 044f 0020  .N.B.C. .4.;.O. 
-0000df60: 043f 0435 0440 0435 0432 043e 0434 0430  .?.5.@.5.2.>.4.0
-0000df70: 003a 0020 0800 0000 0006 0000 001e 556e  .:. ..........Un
-0000df80: 6d61 7463 6865 6420 6173 7365 7420 666f  matched asset fo
-0000df90: 7220 7472 616e 7366 6572 3a20 0700 0000  r transfer: ....
-0000dfa0: 0953 7461 7465 6d65 6e74 0103 0000 006c  .Statement.....l
-0000dfb0: 041d 0435 0432 043e 0437 043c 043e 0436  ...5.2.>.7.<.>.6
-0000dfc0: 043d 043e 0020 0441 043e 043f 043e 0441  .=.>. .A.>.?.>.A
-0000dfd0: 0442 0430 0432 0438 0442 044c 0020 043a  .B.0.2.8.B.L. .:
-0000dfe0: 0430 0442 0435 0433 043e 0440 0438 044e  .0.B.5.3.>.@.8.N
-0000dff0: 0020 0434 043b 044f 0020 043f 0440 0438  . .4.;.O. .?.@.8
-0000e000: 0445 043e 0434 0430 002f 0440 0430 0441  .E.>.4.0./.@.0.A
-0000e010: 0445 043e 0434 0430 003a 0020 0800 0000  .E.>.4.0.:. ....
-0000e020: 0006 0000 0028 556e 6d61 7463 6865 6420  .....(Unmatched 
-0000e030: 6361 7465 676f 7279 2066 6f72 2069 6e63  category for inc
-0000e040: 6f6d 652f 7370 656e 6469 6e67 3a20 0700  ome/spending: ..
-0000e050: 0000 0953 7461 7465 6d65 6e74 0103 0000  ...Statement....
-0000e060: 0050 041d 0435 0432 043e 0437 043c 043e  .P...5.2.>.7.<.>
-0000e070: 043d 043e 0020 0441 043e 043f 043e 0441  .=.>. .A.>.?.>.A
-0000e080: 0442 0430 0432 0438 0442 044c 0020 0432  .B.0.2.8.B.L. .2
-0000e090: 0430 043b 044e 0442 0443 0020 0434 043b  .0.;.N.B.C. .4.;
-0000e0a0: 044f 0020 0441 0447 0451 0442 0430 003a  .O. .A.G.Q.B.0.:
-0000e0b0: 0020 0800 0000 0006 0000 0020 556e 6d61  . ......... Unma
-0000e0c0: 7463 6865 6420 6375 7272 656e 6379 2066  tched currency f
-0000e0d0: 6f72 2061 6363 6f75 6e74 3a20 0700 0000  or account: ....
-0000e0e0: 0953 7461 7465 6d65 6e74 0103 0000 0082  .Statement......
-0000e0f0: 041d 0435 0432 043e 0437 043c 043e 0436  ...5.2.>.7.<.>.6
-0000e100: 043d 043e 0020 0441 043e 043f 043e 0441  .=.>. .A.>.?.>.A
-0000e110: 0442 0430 0432 0438 0442 044c 0020 043a  .B.0.2.8.B.L. .:
-0000e120: 043e 043d 0442 0440 0430 0433 0435 043d  .>.=.B.@.0.3.5.=
-0000e130: 0442 0430 0020 0434 043b 044f 0020 043e  .B.0. .4.;.O. .>
-0000e140: 043f 0435 0440 0430 0446 0438 0438 0020  .?.5.@.0.F.8.8. 
-0000e150: 043f 0440 0438 0445 043e 0434 0430 002f  .?.@.8.E.>.4.0./
-0000e160: 0440 0430 0441 0445 043e 0434 0430 003a  .@.0.A.E.>.4.0.:
-0000e170: 0020 0800 0000 0006 0000 0024 556e 6d61  . .........$Unma
-0000e180: 7463 6865 6420 7065 6572 2066 6f72 2069  tched peer for i
-0000e190: 6e63 6f6d 652f 7370 656e 6469 6e67 3a20  ncome/spending: 
-0000e1a0: 0700 0000 0953 7461 7465 6d65 6e74 0103  .....Statement..
-0000e1b0: 0000 0052 041d 0435 043f 043e 0434 0434  ...R...5.?.>.4.4
-0000e1c0: 0435 0440 0436 0438 0432 0430 0435 043c  .5.@.6.8.2.0.5.<
-0000e1d0: 043e 0435 0020 043a 043e 0440 043f 043e  .>.5. .:.>.@.?.>
-0000e1e0: 0440 0430 0442 0438 0432 043d 043e 0435  .@.0.B.8.2.=.>.5
-0000e1f0: 0020 0434 0435 0439 0441 0442 0432 0438  . .4.5.9.A.B.2.8
-0000e200: 0435 003a 0020 0800 0000 0006 0000 001e  .5.:. ..........
-0000e210: 556e 7375 7070 6f72 7465 6420 636f 7270  Unsupported corp
-0000e220: 6f72 6174 6520 6163 7469 6f6e 3a20 0700  orate action: ..
-0000e230: 0000 0953 7461 7465 6d65 6e74 0103 0000  ...Statement....
-0000e240: 003c 041d 0435 043f 043e 0434 0434 0435  .<...5.?.>.4.4.5
-0000e250: 0440 0436 0438 0432 0430 0435 043c 044b  .@.6.8.2.0.5.<.K
-0000e260: 0439 0020 0442 0438 043f 0020 0432 044b  .9. .B.8.?. .2.K
-0000e270: 043f 043b 0430 0442 044b 003a 0020 0800  .?.;.0.B.K.:. ..
-0000e280: 0000 0006 0000 001a 556e 7375 7070 6f72  ........Unsuppor
-0000e290: 7465 6420 7061 796d 656e 7420 7479 7065  ted payment type
-0000e2a0: 3a20 0700 0000 0953 7461 7465 6d65 6e74  : .....Statement
-0000e2b0: 0103 0000 0012 0421 043f 0438 0441 0430  .......!.?.8.A.0
-0000e2c0: 043d 0438 0435 0020 0800 0000 0006 0000  .=.8.5. ........
-0000e2d0: 000e 5769 7468 6472 6177 616c 206f 6620  ..Withdrawal of 
-0000e2e0: 0700 0000 0953 7461 7465 6d65 6e74 0103  .....Statement..
-0000e2f0: 0000 0044 002a 002a 002a 0020 041d 0415  ...D.*.*.*. ....
-0000e300: 041e 0411 0425 041e 0414 0418 041c 0410  .....%..........
-0000e310: 0020 0420 0423 0427 041d 0410 042f 0020  . . .#.'...../. 
-0000e320: 041f 0420 041e 0412 0415 0420 041a 0410  ... ....... ....
-0000e330: 0020 002a 002a 002a 0800 0000 0006 0000  . .*.*.*........
-0000e340: 001d 2a2a 2a20 4d41 4e55 414c 2045 4e54  ..*** MANUAL ENT
-0000e350: 5259 2052 4551 5549 5245 4420 2a2a 2a07  RY REQUIRED ***.
-0000e360: 0000 000d 5374 6174 656d 656e 7449 424b  ....StatementIBK
-0000e370: 5201 0300 0000 3404 2204 3804 3f00 2004  R.....4.".8.?. .
-0000e380: 2604 1100 2004 3d04 3500 2004 3f04 3e04  &... .=.5. .?.>.
-0000e390: 3404 3404 3504 4004 3604 3804 3204 3004  4.4.5.@.6.8.2.0.
-0000e3a0: 3504 4204 4104 4f00 3a00 2008 0000 0000  5.B.A.O.:. .....
-0000e3b0: 0600 0000 1c41 7373 6574 2074 7970 6520  .....Asset type 
-0000e3c0: 6973 6e27 7420 7375 7070 6f72 7465 643a  isn't supported:
-0000e3d0: 2007 0000 000d 5374 6174 656d 656e 7449   .....StatementI
-0000e3e0: 424b 5201 0300 0000 4804 1d04 3504 3204  BKR.....H...5.2.
-0000e3f0: 3e04 3704 3c04 3e04 3604 3d04 3e00 2004  >.7.<.>.6.=.>. .
-0000e400: 3d04 3004 3904 4204 3800 2004 3f04 3b04  =.0.9.B.8. .?.;.
-0000e410: 3004 4204 5104 3600 2004 3404 3b04 4f00  0.B.Q.6. .4.;.O.
-0000e420: 2004 3e04 4204 3c04 3504 3d04 4b00 3a00   .>.B.<.5.=.K.:.
-0000e430: 2008 0000 0000 0600 0000 1f43 616e 2774   ..........Can't
-0000e440: 2066 696e 6420 6d61 7463 6820 666f 7220   find match for 
-0000e450: 7265 7665 7273 616c 3a20 0700 0000 0d53  reversal: .....S
-0000e460: 7461 7465 6d65 6e74 4942 4b52 0103 0000  tatementIBKR....
-0000e470: 0046 041d 0435 0432 043e 0437 043c 043e  .F...5.2.>.7.<.>
-0000e480: 0436 043d 043e 0020 043d 0430 0439 0442  .6.=.>. .=.0.9.B
-0000e490: 0438 0020 043f 0430 0440 043d 0443 044e  .8. .?.0.@.=.C.N
-0000e4a0: 0020 0437 0430 043f 0438 0441 044c 0020  . .7.0.?.8.A.L. 
-0000e4b0: 0434 043b 044f 0020 0800 0000 0006 0000  .4.;.O. ........
-0000e4c0: 001d 4361 6e27 7420 6669 6e64 2070 6169  ..Can't find pai
-0000e4d0: 7265 6420 7265 636f 7264 2066 6f72 2007  red record for .
-0000e4e0: 0000 000d 5374 6174 656d 656e 7449 424b  ....StatementIBK
-0000e4f0: 5201 0300 0000 4e04 1d04 3504 3204 3e04  R.....N...5.2.>.
-0000e500: 3c04 3e04 3604 3d04 3e00 2004 3e04 3f04  <.>.6.=.>. .>.?.
-0000e510: 4004 3504 3404 3504 3b04 3804 4204 4c00  @.5.4.5.;.8.B.L.
-0000e520: 2004 3204 3004 3b04 4e04 4204 4300 2004   .2.0.;.N.B.C. .
-0000e530: 3404 3b04 4f00 2004 4104 4704 5104 4204  4.;.O. .A.G.Q.B.
-0000e540: 3000 3a00 2008 0000 0000 0600 0000 2843  0.:. .........(C
-0000e550: 616e 2774 2067 6574 2061 6363 6f75 6e74  an't get account
-0000e560: 2063 7572 7265 6e63 7920 666f 7220 6163   currency for ac
-0000e570: 636f 756e 743a 2007 0000 000d 5374 6174  count: .....Stat
-0000e580: 656d 656e 7449 424b 5201 0300 0000 7004  ementIBKR.....p.
-0000e590: 1d04 3504 3204 3e04 3704 3c04 3e04 3604  ..5.2.>.7.<.>.6.
-0000e5a0: 3d04 3e00 2004 3e04 3f04 4004 3504 3404  =.>. .>.?.@.5.4.
-0000e5b0: 3504 3b04 3804 4204 4c00 2004 3204 3004  5.;.8.B.L. .2.0.
-0000e5c0: 3b04 4e04 4204 4b00 2004 3404 3b04 4f00  ;.N.B.K. .4.;.O.
-0000e5d0: 2004 3e04 3f04 3504 4004 3004 4604 3804   .>.?.5.@.0.F.8.
-0000e5e0: 3800 2004 3e04 3104 3c04 3504 3d04 3000  8. .>.1.<.5.=.0.
-0000e5f0: 2004 3204 3004 3b04 4e04 4200 3a00 2008   .2.0.;.N.B.:. .
-0000e600: 0000 0000 0600 0000 2c43 616e 2774 2067  ........,Can't g
-0000e610: 6574 2063 7572 7265 6e63 6965 7320 666f  et currencies fo
-0000e620: 7220 6375 7272 656e 6379 2065 7863 6861  r currency excha
-0000e630: 6e67 653a 2007 0000 000d 5374 6174 656d  nge: .....Statem
-0000e640: 656e 7449 424b 5201 0300 0000 6804 1d04  entIBKR.....h...
-0000e650: 3504 3204 3e04 3704 3c04 3e04 3604 3d04  5.2.>.7.<.>.6.=.
-0000e660: 3e00 2004 4004 3004 4104 3f04 3e04 3704  >. .@.0.A.?.>.7.
-0000e670: 3d04 3004 4204 4c00 2004 3e04 3f04 3804  =.0.B.L. .>.?.8.
-0000e680: 4104 3004 3d04 3804 3500 2004 1e04 3104  A.0.=.8.5. ...1.
-0000e690: 4a04 3504 3404 3804 3d04 3504 3d04 3804  J.5.4.8.=.5.=.8.
-0000e6a0: 4f00 2004 3a04 3e04 3c04 3f04 3004 3d04  O. .:.>.<.?.0.=.
-0000e6b0: 3804 3900 2008 0000 0000 0600 0000 1f43  8.9. ..........C
-0000e6c0: 616e 2774 2070 6172 7365 204d 6572 6765  an't parse Merge
-0000e6d0: 7220 6465 7363 7269 7074 696f 6e20 0700  r description ..
-0000e6e0: 0000 0d53 7461 7465 6d65 6e74 4942 4b52  ...StatementIBKR
-0000e6f0: 0103 0000 0064 041d 0435 0432 043e 0437  .....d...5.2.>.7
-0000e700: 043c 043e 0436 043d 043e 0020 0440 0430  .<.>.6.=.>. .@.0
-0000e710: 0441 043f 043e 0437 043d 0430 0442 044c  .A.?.>.7.=.0.B.L
-0000e720: 0020 043e 043f 0438 0441 0430 043d 0438  . .>.?.8.A.0.=.8
-0000e730: 0435 0020 0412 044b 0434 0435 043b 0435  .5. ...K.4.5.;.5
-0000e740: 043d 0438 044f 0020 043a 043e 043c 043f  .=.8.O. .:.>.<.?
-0000e750: 0430 043d 0438 0438 0020 0800 0000 0006  .0.=.8.8. ......
-0000e760: 0000 0021 4361 6e27 7420 7061 7273 6520  ...!Can't parse 
-0000e770: 5370 696e 2d6f 6666 2064 6573 6372 6970  Spin-off descrip
-0000e780: 7469 6f6e 2007 0000 000d 5374 6174 656d  tion .....Statem
-0000e790: 656e 7449 424b 5201 0300 0000 4c04 1d04  entIBKR.....L...
-0000e7a0: 3504 3204 3e04 3704 3c04 3e04 3604 3d04  5.2.>.7.<.>.6.=.
-0000e7b0: 3e00 2004 4004 3004 4104 3f04 3e04 3704  >. .@.0.A.?.>.7.
-0000e7c0: 3d04 3004 4204 4c00 2004 3e04 3f04 3804  =.0.B.L. .>.?.8.
-0000e7d0: 4104 3004 3d04 3804 3500 2004 2104 3f04  A.0.=.8.5. .!.?.
-0000e7e0: 3b04 3804 4204 3000 2008 0000 0000 0600  ;.8.B.0. .......
-0000e7f0: 0000 1e43 616e 2774 2070 6172 7365 2053  ...Can't parse S
-0000e800: 706c 6974 2064 6573 6372 6970 7469 6f6e  plit description
-0000e810: 2007 0000 000d 5374 6174 656d 656e 7449   .....StatementI
-0000e820: 424b 5201 0300 0000 6204 1d04 3504 3204  BKR.....b...5.2.
-0000e830: 3e04 3704 3c04 3e04 3604 3d04 3e00 2004  >.7.<.>.6.=.>. .
-0000e840: 4004 3004 4104 3f04 3e04 3704 3d04 3004  @.0.A.?.>.7.=.0.
-0000e850: 4204 4c00 2004 3e04 3f04 3804 4104 3004  B.L. .>.?.8.A.0.
-0000e860: 3d04 3804 3500 2004 1404 3804 3204 3804  =.8.5. ...8.2.8.
-0000e870: 3404 3504 3d04 3404 3000 2004 3004 3a04  4.5.=.4.0. .0.:.
-0000e880: 4604 3804 4f04 3c04 3800 2008 0000 0000  F.8.O.<.8. .....
-0000e890: 0600 0000 2743 616e 2774 2070 6172 7365  ....'Can't parse
-0000e8a0: 2053 746f 636b 2044 6976 6964 656e 6420   Stock Dividend 
-0000e8b0: 6465 7363 7269 7074 696f 6e20 0700 0000  description ....
-0000e8c0: 0d53 7461 7465 6d65 6e74 4942 4b52 0103  .StatementIBKR..
-0000e8d0: 0000 005a 041d 0435 0432 043e 0437 043c  ...Z...5.2.>.7.<
-0000e8e0: 043e 0436 043d 043e 0020 0440 0430 0441  .>.6.=.>. .@.0.A
-0000e8f0: 043f 043e 0437 043d 0430 0442 044c 0020  .?.>.7.=.0.B.L. 
-0000e900: 043e 043f 0438 0441 0430 043d 0438 0435  .>.?.8.A.0.=.8.5
-0000e910: 0020 0421 043c 0435 043d 044b 0020 0441  . .!.<.5.=.K. .A
-0000e920: 0438 043c 0432 043e 043b 0430 0020 0800  .8.<.2.>.;.0. ..
-0000e930: 0000 0006 0000 0026 4361 6e27 7420 7061  .......&Can't pa
-0000e940: 7273 6520 5379 6d62 6f6c 2043 6861 6e67  rse Symbol Chang
-0000e950: 6520 6465 7363 7269 7074 696f 6e20 0700  e description ..
-0000e960: 0000 0d53 7461 7465 6d65 6e74 4942 4b52  ...StatementIBKR
-0000e970: 0103 0000 006e 041d 0435 0432 043e 0437  .....n...5.2.>.7
-0000e980: 043c 043e 0436 043d 043e 0020 043e 0431  .<.>.6.=.>. .>.1
-0000e990: 0440 0430 0431 043e 0442 0430 0442 044c  .@.0.1.>.B.0.B.L
-0000e9a0: 0020 043e 0442 043c 0435 043d 0451 043d  . .>.B.<.5.=.Q.=
-0000e9b0: 043d 043e 0435 0020 043a 043e 0440 043f  .=.>.5. .:.>.@.?
-0000e9c0: 043e 0440 0430 0442 0438 0432 043d 043e  .>.@.0.B.8.2.=.>
-0000e9d0: 0435 0020 0434 0435 0439 0441 0442 0432  .5. .4.5.9.A.B.2
-0000e9e0: 0438 0435 0800 0000 0006 0000 0028 4361  .8.5.........(Ca
-0000e9f0: 6e27 7420 7072 6f63 6573 7320 6361 6e63  n't process canc
-0000ea00: 656c 6c65 6420 636f 7270 6f72 6174 6520  elled corporate 
-0000ea10: 6163 7469 6f6e 0700 0000 0d53 7461 7465  action.....State
-0000ea20: 6d65 6e74 4942 4b52 0103 0000 003e 0414  mentIBKR.....>..
-0000ea30: 0435 043d 0435 0436 043d 044b 0435 0020  .5.=.5.6.=.K.5. 
-0000ea40: 0442 0440 0430 043d 0437 0430 043a 0446  .B.@.0.=.7.0.:.F
-0000ea50: 0438 0438 0020 0437 0430 0433 0440 0443  .8.8. .7.0.3.@.C
-0000ea60: 0436 0435 043d 044b 003a 0020 0800 0000  .6.5.=.K.:. ....
-0000ea70: 0006 0000 001a 4361 7368 2074 7261 6e73  ......Cash trans
-0000ea80: 6163 7469 6f6e 7320 6c6f 6164 6564 3a20  actions loaded: 
-0000ea90: 0700 0000 0d53 7461 7465 6d65 6e74 4942  .....StatementIB
-0000eaa0: 4b52 0103 0000 006a 041a 043e 0440 043f  KR.....j...>.@.?
-0000eab0: 043e 0440 0430 0442 0438 0432 043d 043e  .>.@.0.B.8.2.=.>
-0000eac0: 0435 0020 0441 043e 0431 044b 0442 0438  .5. .A.>.1.K.B.8
-0000ead0: 0435 0020 043d 0435 0020 043f 043e 0434  .5. .=.5. .?.>.4
-0000eae0: 0434 0435 0440 0436 0438 0432 0430 0435  .4.5.@.6.8.2.0.5
-0000eaf0: 0442 0441 044f 0020 0434 043b 044f 0020  .B.A.O. .4.;.O. 
-0000eb00: 0442 0438 043f 0430 0020 0426 0411 003a  .B.8.?.0. .&...:
-0000eb10: 0020 0800 0000 0006 0000 0031 436f 7270  . .........1Corp
-0000eb20: 6f72 6174 6520 6163 7469 6f6e 2069 736e  orate action isn
-0000eb30: 2774 2073 7570 706f 7274 6564 2066 6f72  't supported for
-0000eb40: 2061 7373 6574 2074 7970 653a 2007 0000   asset type: ...
-0000eb50: 000d 5374 6174 656d 656e 7449 424b 5201  ..StatementIBKR.
-0000eb60: 0300 0000 5e04 2204 3804 3f00 2004 3a04  ....^.".8.?. .:.
-0000eb70: 3e04 4004 3f04 3e04 4004 3004 4204 3804  >.@.?.>.@.0.B.8.
-0000eb80: 3204 3d04 3e04 3304 3e00 2004 3404 3504  2.=.>.3.>. .4.5.
-0000eb90: 3904 4104 4204 3204 3804 4f00 2004 3d04  9.A.B.2.8.O. .=.
-0000eba0: 3500 2004 3f04 3e04 3404 3404 3504 4004  5. .?.>.4.4.5.@.
-0000ebb0: 3604 3804 3204 3004 3504 4204 4104 4f00  6.8.2.0.5.B.A.O.
-0000ebc0: 3a00 2008 0000 0000 0600 0000 2843 6f72  :. .........(Cor
-0000ebd0: 706f 7261 7465 2061 6374 696f 6e20 7479  porate action ty
-0000ebe0: 7065 2069 7320 6e6f 7420 7375 7070 6f72  pe is not suppor
-0000ebf0: 7465 643a 2007 0000 000d 5374 6174 656d  ted: .....Statem
-0000ec00: 656e 7449 424b 5201 0300 0000 4404 1a04  entIBKR.....D...
-0000ec10: 3e04 4004 3f04 3e04 4004 3004 4204 3804  >.@.?.>.@.0.B.8.
-0000ec20: 3204 3d04 4b04 3500 2004 3404 3504 3904  2.=.K.5. .4.5.9.
-0000ec30: 4104 4204 3204 3804 4f00 2004 3704 3004  A.B.2.8.O. .7.0.
-0000ec40: 3304 4004 4304 3604 3504 3d04 4b00 3a00  3.@.C.6.5.=.K.:.
-0000ec50: 2008 0000 0000 0600 0000 1a43 6f72 706f   ..........Corpo
-0000ec60: 7261 7465 2061 6374 696f 6e73 206c 6f61  rate actions loa
-0000ec70: 6465 643a 2007 0000 000d 5374 6174 656d  ded: .....Statem
-0000ec80: 656e 7449 424b 5201 0300 0000 5604 1404  entIBKR.....V...
-0000ec90: 3804 3204 3804 3404 3504 3d04 3400 2004  8.2.8.4.5.=.4. .
-0000eca0: 3d04 3500 2004 3d04 3004 3904 3404 3504  =.5. .=.0.9.4.5.
-0000ecb0: 3d00 2004 3404 3b04 4f00 2004 4304 3404  =. .4.;.O. .C.4.
-0000ecc0: 3504 4004 3604 3004 3d04 3d04 3e04 3304  5.@.6.0.=.=.>.3.
-0000ecd0: 3e00 2004 3d04 3004 3b04 3e04 3304 3000  >. .=.0.;.>.3.0.
-0000ece0: 3a00 2008 0000 0000 0600 0000 2844 6976  :. .........(Div
-0000ecf0: 6964 656e 6420 6e6f 7420 666f 756e 6420  idend not found 
-0000ed00: 666f 7220 7769 7468 686f 6c64 696e 6720  for withholding 
-0000ed10: 7461 783a 2007 0000 000d 5374 6174 656d  tax: .....Statem
-0000ed20: 656e 7449 424b 5201 0300 0000 2e00 4900  entIBKR.......I.
-0000ed30: 4200 4b00 5200 2000 6600 6c00 6500 7800  B.K.R. .f.l.e.x.
-0000ed40: 2d04 3e04 4204 4704 5104 4200 2000 2800  -.>.B.G.Q.B. .(.
-0000ed50: 2a00 2e00 7800 6d00 6c00 2908 0000 0000  *...x.m.l.).....
-0000ed60: 0600 0000 1749 424b 5220 666c 6578 2d71  .....IBKR flex-q
-0000ed70: 7565 7279 2028 2a2e 786d 6c29 0700 0000  uery (*.xml)....
-0000ed80: 0d53 7461 7465 6d65 6e74 4942 4b52 0103  .StatementIBKR..
-0000ed90: 0000 0026 0049 006e 0074 0065 0072 0061  ...&.I.n.t.e.r.a
-0000eda0: 0063 0074 0069 0076 0065 0020 0042 0072  .c.t.i.v.e. .B.r
-0000edb0: 006f 006b 0065 0072 0073 0800 0000 0006  .o.k.e.r.s......
-0000edc0: 0000 0013 496e 7465 7261 6374 6976 6520  ....Interactive 
-0000edd0: 4272 6f6b 6572 7307 0000 000d 5374 6174  Brokers.....Stat
-0000ede0: 656d 656e 7449 424b 5201 0300 0000 5604  ementIBKR.....V.
-0000edf0: 2204 3804 3f00 2004 3e04 4204 4704 5104  ".8.?. .>.B.G.Q.
-0000ee00: 4204 3000 2000 4900 6e00 7400 6500 7200  B.0. .I.n.t.e.r.
-0000ee10: 6100 6300 7400 6900 7600 6500 2000 4200  a.c.t.i.v.e. .B.
-0000ee20: 7200 6f00 6b00 6500 7200 7300 2004 3d04  r.o.k.e.r.s. .=.
-0000ee30: 3500 2004 3e04 3f04 4004 3504 3404 3504  5. .>.?.@.5.4.5.
-0000ee40: 3b04 5104 3d08 0000 0000 0600 0000 2949  ;.Q.=.........)I
-0000ee50: 6e74 6572 6163 7469 7665 2042 726f 6b65  nteractive Broke
-0000ee60: 7273 2072 6570 6f72 7420 7479 7065 206e  rs report type n
-0000ee70: 6f74 2066 6f75 6e64 0700 0000 0d53 7461  ot found.....Sta
-0000ee80: 7465 6d65 6e74 4942 4b52 0103 0000 003a  tementIBKR.....:
-0000ee90: 0417 0430 0433 0440 0443 0437 043a 0430  ...0.3.@.C.7.:.0
-0000eea0: 0020 043e 0442 0447 0451 0442 0430 0020  . .>.B.G.Q.B.0. 
-0000eeb0: 0049 0042 0020 0434 043b 044f 0020 0441  .I.B. .4.;.O. .A
-0000eec0: 0447 0451 0442 0430 0020 0800 0000 0006  .G.Q.B.0. ......
-0000eed0: 0000 0023 4c6f 6164 2049 4220 466c 6578  ...#Load IB Flex
-0000eee0: 2d73 7461 7465 6d65 6e74 2066 6f72 2061  -statement for a
-0000eef0: 6363 6f75 6e74 2007 0000 000d 5374 6174  ccount .....Stat
-0000ef00: 656d 656e 7449 424b 5201 0300 0000 5804  ementIBKR.....X.
-0000ef10: 1d04 3504 3404 3e04 4104 4204 3004 4204  ..5.4.>.A.B.0.B.
-0000ef20: 3e04 4704 3d04 3e00 2004 3404 3004 3d04  >.G.=.>. .4.0.=.
-0000ef30: 3d04 4b04 4500 2004 3e04 3100 2004 1e04  =.K.E. .>.1. ...
-0000ef40: 3104 4a04 3504 3404 3804 3d04 3504 3d04  1.J.5.4.8.=.5.=.
-0000ef50: 3804 3800 2004 3a04 3e04 3c04 3f04 3004  8.8. .:.>.<.?.0.
-0000ef60: 3d04 3804 3900 2008 0000 0000 0600 0000  =.8.9. .........
-0000ef70: 224d 6572 6765 7220 6465 7363 7269 7074  "Merger descript
-0000ef80: 696f 6e20 6d69 7373 2073 6f6d 6520 6461  ion miss some da
-0000ef90: 7461 2007 0000 000d 5374 6174 656d 656e  ta .....Statemen
-0000efa0: 7449 424b 5201 0300 0000 5e04 1d04 3504  tIBKR.....^...5.
-0000efb0: 3e04 3404 3d04 3e04 3704 3d04 3004 4704  >.4.=.>.7.=.0.G.
-0000efc0: 3d04 3e04 3500 2004 4104 3e04 3204 3f04  =.>.5. .A.>.2.?.
-0000efd0: 3004 3404 3504 3d04 3804 3500 2004 4104  0.4.5.=.8.5. .A.
-0000efe0: 3e04 3104 4b04 4204 3804 3900 2004 4004  >.1.K.B.8.9. .@.
-0000eff0: 3504 3e04 4004 3304 3004 3d04 3804 3704  5.>.@.3.0.=.8.7.
-0000f000: 3004 4604 3804 3800 2008 0000 0000 0600  0.F.8.8. .......
-0000f010: 0000 294d 756c 7469 706c 6520 6d65 7267  ..)Multiple merg
-0000f020: 6572 2072 6563 6f72 6473 2061 6c72 6561  er records alrea
-0000f030: 6479 2065 7869 7374 2061 7420 0700 0000  dy exist at ....
-0000f040: 0d53 7461 7465 6d65 6e74 4942 4b52 0103  .StatementIBKR..
-0000f050: 0000 0052 0414 0435 0439 0441 0442 0432  ...R...5.9.A.B.2
-0000f060: 0438 0435 0020 043d 0435 0020 043f 043e  .8.5. .=.5. .?.>
-0000f070: 0434 0434 0435 0440 0436 0438 0432 0430  .4.4.5.@.6.8.2.0
-0000f080: 0435 0442 0441 044f 0020 0434 043b 044f  .5.B.A.O. .4.;.O
-0000f090: 0020 043e 043f 0446 0438 043e 043d 043e  . .>.?.F.8.>.=.>
-0000f0a0: 0432 003a 0020 0800 0000 0006 0000 0027  .2.:. .........'
-0000f0b0: 4f70 7469 6f6e 2045 2641 2645 2061 6374  Option E&A&E act
-0000f0c0: 696f 6e20 6973 6e27 7420 696d 706c 656d  ion isn't implem
-0000f0d0: 656e 7465 643a 2007 0000 000d 5374 6174  ented: .....Stat
-0000f0e0: 656d 656e 7449 424b 5201 0300 0000 3a04  ementIBKR.....:.
-0000f0f0: 1804 4104 3f04 3e04 3b04 3d04 3504 3d04  ..A.?.>.;.=.5.=.
-0000f100: 3804 3500 2004 3f04 4004 3e04 3404 3004  8.5. .?.@.>.4.0.
-0000f110: 3d04 3d04 3e04 3304 3e00 2004 3e04 3f04  =.=.>.3.>. .>.?.
-0000f120: 4604 3804 3e04 3d04 3008 0000 0000 0600  F.8.>.=.0.......
-0000f130: 0000 114f 7074 696f 6e20 6173 7369 676e  ...Option assign
-0000f140: 6d65 6e74 0700 0000 0d53 7461 7465 6d65  ment.....Stateme
-0000f150: 6e74 4942 4b52 0103 0000 003a 0418 0441  ntIBKR.....:...A
-0000f160: 043f 043e 043b 043d 0435 043d 0438 0435  .?.>.;.=.5.=.8.5
-0000f170: 002f 044d 043a 0441 043f 0438 0440 0430  ./.M.:.A.?.8.@.0
-0000f180: 0446 0438 044f 0020 043e 043f 0446 0438  .F.8.O. .>.?.F.8
-0000f190: 043e 043d 0430 0800 0000 0006 0000 001a  .>.=.0..........
-0000f1a0: 4f70 7469 6f6e 2061 7373 6967 6e6d 656e  Option assignmen
-0000f1b0: 742f 6578 6572 6369 7365 0700 0000 0d53  t/exercise.....S
-0000f1c0: 7461 7465 6d65 6e74 4942 4b52 0103 0000  tatementIBKR....
-0000f1d0: 003a 0418 0441 043f 043e 043b 043d 0435  .:...A.?.>.;.=.5
-0000f1e0: 043d 0438 0435 0020 043a 0443 043f 043b  .=.8.5. .:.C.?.;
-0000f1f0: 0435 043d 043d 043e 0433 043e 0020 043e  .5.=.=.>.3.>. .>
-0000f200: 043f 0446 0438 043e 043d 0430 0800 0000  .?.F.8.>.=.0....
-0000f210: 0006 0000 000f 4f70 7469 6f6e 2065 7865  ......Option exe
-0000f220: 7263 6973 6507 0000 000d 5374 6174 656d  rcise.....Statem
-0000f230: 656e 7449 424b 5201 0300 0000 2404 2d04  entIBKR.....$.-.
-0000f240: 3a04 4104 3f04 3804 4004 3004 4604 3804  :.A.?.8.@.0.F.8.
-0000f250: 4f00 2004 3e04 3f04 4604 3804 3e04 3d04  O. .>.?.F.8.>.=.
-0000f260: 3008 0000 0000 0600 0000 114f 7074 696f  0..........Optio
-0000f270: 6e20 6578 7069 7261 7469 6f6e 0700 0000  n expiration....
-0000f280: 0d53 7461 7465 6d65 6e74 4942 4b52 0103  .StatementIBKR..
-0000f290: 0000 0040 0414 0435 0439 0441 0442 0432  ...@...5.9.A.B.2
-0000f2a0: 0438 044f 0020 0441 0020 043e 043f 0446  .8.O. .A. .>.?.F
-0000f2b0: 0438 043e 043d 0430 043c 0438 0020 0437  .8.>.=.0.<.8. .7
-0000f2c0: 0430 0433 0440 0443 0436 0435 043d 044b  .0.3.@.C.6.5.=.K
-0000f2d0: 003a 0020 0800 0000 0006 0000 0016 4f70  .:. ..........Op
-0000f2e0: 7469 6f6e 7320 4526 4126 4520 6c6f 6164  tions E&A&E load
-0000f2f0: 6564 3a20 0700 0000 0d53 7461 7465 6d65  ed: .....Stateme
-0000f300: 6e74 4942 4b52 0103 0000 006a 041d 0435  ntIBKR.....j...5
-0000f310: 0020 043d 0430 0439 0434 0435 043d 0430  . .=.0.9.4.5.=.0
-0000f320: 0020 0441 0434 0435 043b 043a 0430 0020  . .A.4.5.;.:.0. 
-0000f330: 0434 043b 044f 0020 0438 0441 043f 043e  .4.;.O. .8.A.?.>
-0000f340: 043b 043d 0435 043d 0438 044f 002f 044d  .;.=.5.=.8.O./.M
-0000f350: 043a 0441 043f 0438 0440 0430 0446 0438  .:.A.?.8.@.0.F.8
-0000f360: 0438 0020 043e 043f 0446 0438 043e 043d  .8. .>.?.F.8.>.=
-0000f370: 0430 003a 0020 0800 0000 0006 0000 0035  .0.:. .........5
-0000f380: 4f72 6967 696e 616c 2074 7261 6465 206e  Original trade n
-0000f390: 6f74 2066 6f75 6e64 2066 6f72 204f 7074  ot found for Opt
-0000f3a0: 696f 6e20 4526 4126 4520 6f70 6572 6174  ion E&A&E operat
-0000f3b0: 696f 6e3a 2007 0000 000d 5374 6174 656d  ion: .....Statem
-0000f3c0: 656e 7449 424b 5201 0300 0000 6c04 1f04  entIBKR.....l...
-0000f3d0: 3b04 3004 4204 5104 3600 2004 3104 4b04  ;.0.B.Q.6. .1.K.
-0000f3e0: 3b00 2004 3e04 4204 3c04 3504 3d04 5104  ;. .>.B.<.5.=.Q.
-0000f3f0: 3d00 2004 3f04 3e00 2004 3f04 4004 3804  =. .?.>. .?.@.8.
-0000f400: 3c04 3504 4004 3d04 3e04 3c04 4300 2004  <.5.@.=.>.<.C. .
-0000f410: 4104 3e04 3204 3f04 3004 3404 3504 3d04  A.>.2.?.0.4.5.=.
-0000f420: 3804 4e00 2004 3e04 3f04 3804 4104 3004  8.N. .>.?.8.A.0.
-0000f430: 3d04 3804 4f00 3a00 2008 0000 0000 0600  =.8.O.:. .......
-0000f440: 0000 3150 6179 6d65 6e74 2077 6173 2072  ..1Payment was r
-0000f450: 6576 6572 7365 6420 6279 2061 7070 726f  eversed by appro
-0000f460: 7869 6d61 7465 2064 6573 6372 6970 7469  ximate descripti
-0000f470: 6f6e 3a20 0700 0000 0d53 7461 7465 6d65  on: .....Stateme
-0000f480: 6e74 4942 4b52 0103 0000 006a 041f 043b  ntIBKR.....j...;
-0000f490: 0430 0442 0451 0436 0020 0431 044b 043b  .0.B.Q.6. .1.K.;
-0000f4a0: 0020 043e 0442 043c 0435 043d 0451 043d  . .>.B.<.5.=.Q.=
-0000f4b0: 002c 0020 043d 043e 0020 0441 0020 043d  .,. .=.>. .A. .=
-0000f4c0: 0435 0441 043e 0432 043f 0430 0434 0430  .5.A.>.2.?.0.4.0
-0000f4d0: 044e 0449 0435 0439 0020 0434 0430 0442  .N.I.5.9. .4.0.B
-0000f4e0: 043e 0439 0020 043e 0442 0447 0451 0442  .>.9. .>.B.G.Q.B
-0000f4f0: 0430 003a 0020 0800 0000 0006 0000 0033  .0.:. .........3
-0000f500: 5061 796d 656e 7420 7761 7320 7265 7665  Payment was reve
-0000f510: 7273 6564 2077 6974 6820 6469 6666 6572  rsed with differ
-0000f520: 656e 7420 7265 706f 7274 6564 2064 6174  ent reported dat
-0000f530: 653a 2007 0000 000d 5374 6174 656d 656e  e: .....Statemen
-0000f540: 7449 424b 5201 0300 0000 2804 1f04 3b04  tIBKR.....(...;.
-0000f550: 3004 4204 5104 3600 2004 3104 4b04 3b00  0.B.Q.6. .1.K.;.
-0000f560: 2004 3e04 4204 3c04 3504 3d04 5104 3d00   .>.B.<.5.=.Q.=.
-0000f570: 3a00 2008 0000 0000 0600 0000 1650 6179  :. ..........Pay
-0000f580: 6d65 6e74 2077 6173 2072 6576 6572 7365  ment was reverse
-0000f590: 643a 2007 0000 000d 5374 6174 656d 656e  d: .....Statemen
-0000f5a0: 7449 424b 5201 0300 0000 1c04 2604 1100  tIBKR.......&...
-0000f5b0: 2004 3704 3004 3304 4004 4304 3604 3504   .7.0.3.@.C.6.5.
-0000f5c0: 3d04 4b00 3a00 2008 0000 0000 0600 0000  =.K.:. .........
-0000f5d0: 1353 6563 7572 6974 6965 7320 6c6f 6164  .Securities load
-0000f5e0: 6564 3a20 0700 0000 0d53 7461 7465 6d65  ed: .....Stateme
-0000f5f0: 6e74 4942 4b52 0103 0000 0056 041d 0435  ntIBKR.....V...5
-0000f600: 0434 043e 0441 0442 0430 0442 043e 0447  .4.>.A.B.0.B.>.G
-0000f610: 043d 043e 0020 0434 0430 043d 043d 044b  .=.>. .4.0.=.=.K
-0000f620: 0445 0020 0434 043b 044f 0020 0412 044b  .E. .4.;.O. ...K
-0000f630: 0434 0435 043b 0435 043d 0438 044f 0020  .4.5.;.5.=.8.O. 
-0000f640: 043a 043e 043c 043f 0430 043d 0438 0438  .:.>.<.?.0.=.8.8
-0000f650: 0020 0800 0000 0006 0000 0024 5370 696e  . .........$Spin
-0000f660: 2d6f 6666 2064 6573 6372 6970 7469 6f6e  -off description
-0000f670: 206d 6973 7320 736f 6d65 2064 6174 6120   miss some data 
-0000f680: 0700 0000 0d53 7461 7465 6d65 6e74 4942  .....StatementIB
-0000f690: 4b52 0103 0000 005c 0418 0441 0445 043e  KR.....\...A.E.>
-0000f6a0: 0434 043d 0430 044f 0020 0426 0411 0020  .4.=.0.O. .&... 
-0000f6b0: 0434 043b 044f 0020 0432 044b 0434 0435  .4.;.O. .2.K.4.5
-0000f6c0: 043b 0435 043d 0438 044f 0020 043a 043e  .;.5.=.8.O. .:.>
-0000f6d0: 043c 043f 0430 043d 0438 0438 0020 043d  .<.?.0.=.8.8. .=
-0000f6e0: 0435 0020 043d 0430 0439 0434 0435 043d  .5. .=.0.9.4.5.=
-0000f6f0: 0430 0020 0800 0000 0006 0000 0021 5370  .0. .........!Sp
-0000f700: 696e 2d6f 6666 2069 6e69 7469 616c 2061  in-off initial a
-0000f710: 7373 6574 206e 6f74 2066 6f75 6e64 2007  sset not found .
-0000f720: 0000 000d 5374 6174 656d 656e 7449 424b  ....StatementIBK
-0000f730: 5201 0300 0000 5604 1e04 4804 3804 3104  R.....V...H.8.1.
-0000f740: 3a04 3000 2004 3e04 3a04 4004 4304 3304  :.0. .>.:.@.C.3.
-0000f750: 3b04 3504 3d04 3804 4f00 2000 5300 7000  ;.5.=.8.O. .S.p.
-0000f760: 6900 6e00 2d00 6f00 6600 6600 2004 4104  i.n.-.o.f.f. .A.
-0000f770: 3b04 3804 4804 3a04 3e04 3c00 2004 3104  ;.8.H.:.>.<. .1.
-0000f780: 3e04 3b04 4c04 4804 3004 4f00 2008 0000  >.;.L.H.0.O. ...
-0000f790: 0000 0600 0000 2353 7069 6e2d 6f66 6620  ......#Spin-off 
-0000f7a0: 726f 756e 6469 6e67 2065 7272 6f72 2069  rounding error i
-0000f7b0: 7320 746f 6f20 6269 6720 0700 0000 0d53  s too big .....S
-0000f7c0: 7461 7465 6d65 6e74 4942 4b52 0103 0000  tatementIBKR....
-0000f7d0: 003e 041d 0435 0434 043e 0441 0442 0430  .>...5.4.>.A.B.0
-0000f7e0: 0442 043e 0447 043d 043e 0020 0434 0430  .B.>.G.=.>. .4.0
-0000f7f0: 043d 043d 044b 0445 0020 0434 043b 044f  .=.=.K.E. .4.;.O
-0000f800: 0020 0421 043f 043b 0438 0442 0430 0020  . .!.?.;.8.B.0. 
-0000f810: 0800 0000 0006 0000 0021 5370 6c69 7420  .........!Split 
-0000f820: 6465 7363 7269 7074 696f 6e20 6d69 7373  description miss
-0000f830: 2073 6f6d 6520 6461 7461 2007 0000 000d   some data .....
-0000f840: 5374 6174 656d 656e 7449 424b 5201 0300  StatementIBKR...
-0000f850: 0000 3804 1704 3004 4704 3804 4104 3b04  ..8...0.G.8.A.;.
-0000f860: 3504 3d04 3804 3500 2004 3004 3a04 4604  5.=.8.5. .0.:.F.
-0000f870: 3804 3900 2004 3704 3004 3304 4004 4304  8.9. .7.0.3.@.C.
-0000f880: 3604 3504 3d04 3e00 3a00 2008 0000 0000  6.5.=.>.:. .....
-0000f890: 0600 0000 1753 746f 636b 2076 6573 7469  .....Stock vesti
-0000f8a0: 6e67 7320 6c6f 6164 6564 3a20 0700 0000  ngs loaded: ....
-0000f8b0: 0d53 7461 7465 6d65 6e74 4942 4b52 0103  .StatementIBKR..
-0000f8c0: 0000 0048 041a 043e 0440 0440 0435 043a  ...H...>.@.@.5.:
-0000f8d0: 0442 0438 0440 043e 0432 043a 0430 0020  .B.8.@.>.2.:.0. 
-0000f8e0: 043d 0430 043b 043e 0433 0430 0020 0434  .=.0.;.>.3.0. .4
-0000f8f0: 043b 044f 0020 0434 0438 0432 0438 0434  .;.O. .4.8.2.8.4
-0000f900: 0435 043d 0434 0430 003a 0020 0800 0000  .5.=.4.0.:. ....
-0000f910: 0006 0000 001d 5461 7820 6164 6a75 7374  ......Tax adjust
-0000f920: 6d65 6e74 2066 6f72 2064 6976 6964 656e  ment for dividen
-0000f930: 643a 2007 0000 000d 5374 6174 656d 656e  d: .....Statemen
-0000f940: 7449 424b 5201 0300 0000 2404 1d04 3004  tIBKR.....$...0.
-0000f950: 3b04 3e04 3304 3800 2004 3704 3004 3304  ;.>.3.8. .7.0.3.
-0000f960: 4004 4304 3604 3504 3d04 4b00 3a00 2008  @.C.6.5.=.K.:. .
-0000f970: 0000 0000 0600 0000 0e54 6178 6573 206c  .........Taxes l
-0000f980: 6f61 6465 643a 2007 0000 000d 5374 6174  oaded: .....Stat
-0000f990: 656d 656e 7449 424b 5201 03ff ffff ff08  ementIBKR.......
-0000f9a0: 0000 0000 0600 0000 0f54 7261 6465 7320  .........Trades 
-0000f9b0: 6c6f 6164 6564 3a20 0700 0000 0d53 7461  loaded: .....Sta
-0000f9c0: 7465 6d65 6e74 4942 4b52 0103 0000 0058  tementIBKR.....X
-0000f9d0: 041d 0435 043f 043e 0434 0434 0435 0440  ...5.?.>.4.4.5.@
-0000f9e0: 0436 0438 0432 0430 0435 043c 044b 0439  .6.8.2.0.5.<.K.9
-0000f9f0: 0020 0444 043e 0440 043c 0430 0442 0020  . .D.>.@.<.0.B. 
-0000fa00: 043e 043f 0438 0441 0430 043d 0438 044f  .>.?.8.A.0.=.8.O
-0000fa10: 0020 0434 0438 0432 0438 0434 0435 043d  . .4.8.2.8.4.5.=
-0000fa20: 0434 0430 003a 0020 0800 0000 0006 0000  .4.0.:. ........
-0000fa30: 0022 556e 6861 6e64 6c65 6420 6469 7669  ."Unhandled divi
-0000fa40: 6465 6e64 2070 6174 7465 726e 2066 6f75  dend pattern fou
-0000fa50: 6e64 3a20 0700 0000 0d53 7461 7465 6d65  nd: .....Stateme
-0000fa60: 6e74 4942 4b52 0103 0000 004e 041d 0435  ntIBKR.....N...5
-0000fa70: 043f 043e 0434 0434 0435 0440 0436 0438  .?.>.4.4.5.@.6.8
-0000fa80: 0432 0430 0435 043c 044b 0439 0020 0444  .2.0.5.<.K.9. .D
-0000fa90: 043e 0440 043c 0430 0442 0020 0441 0442  .>.@.<.0.B. .A.B
-0000faa0: 0440 0430 043d 044b 0020 043d 0430 043b  .@.0.=.K. .=.0.;
-0000fab0: 043e 0433 0430 003a 0020 0800 0000 0006  .>.3.0.:. ......
-0000fac0: 0000 0025 556e 6861 6e64 6c65 6420 7461  ...%Unhandled ta
-0000fad0: 7820 636f 756e 7472 7920 7061 7474 6572  x country patter
-0000fae0: 6e20 666f 756e 643a 2007 0000 000d 5374  n found: .....St
-0000faf0: 6174 656d 656e 7449 424b 5201 0300 0000  atementIBKR.....
-0000fb00: 5204 1d04 3504 3f04 3e04 3404 3404 3504  R...5.?.>.4.4.5.
-0000fb10: 4004 3604 3804 3204 3004 3504 3c04 4b04  @.6.8.2.0.5.<.K.
-0000fb20: 3900 2004 4404 3e04 4004 3c04 3004 4200  9. .D.>.@.<.0.B.
-0000fb30: 2004 3e04 3f04 3804 4104 3004 3d04 3804   .>.?.8.A.0.=.8.
-0000fb40: 4f00 2004 3d04 3004 3b04 3e04 3304 3000  O. .=.0.;.>.3.0.
-0000fb50: 3a00 2008 0000 0000 0600 0000 1d55 6e68  :. ..........Unh
-0000fb60: 616e 646c 6564 2074 6178 2070 6174 7465  andled tax patte
-0000fb70: 726e 2066 6f75 6e64 3a20 0700 0000 0d53  rn found: .....S
-0000fb80: 7461 7465 6d65 6e74 4942 4b52 0103 0000  tatementIBKR....
-0000fb90: 0058 041d 0435 0438 0437 0432 0435 0441  .X...5.8.7.2.5.A
-0000fba0: 0442 043d 044b 0439 0020 0442 0438 043f  .B.=.K.9. .B.8.?
-0000fbb0: 0020 043e 0442 0447 0451 0442 0430 0020  . .>.B.G.Q.B.0. 
-0000fbc0: 0049 006e 0074 0065 0072 0061 0063 0074  .I.n.t.e.r.a.c.t
-0000fbd0: 0069 0076 0065 0020 0042 0072 006f 006b  .i.v.e. .B.r.o.k
-0000fbe0: 0065 0072 0073 003a 0020 0800 0000 0006  .e.r.s.:. ......
-0000fbf0: 0000 0029 556e 6b6e 6f77 6e20 496e 7465  ...)Unknown Inte
-0000fc00: 7261 6374 6976 6520 4272 6f6b 6572 7320  ractive Brokers 
-0000fc10: 7265 706f 7274 2074 7970 653a 2007 0000  report type: ...
-0000fc20: 000d 5374 6174 656d 656e 7449 424b 5201  ..StatementIBKR.
-0000fc30: 0300 0000 a204 1204 4b00 2004 3f04 4b04  ........K. .?.K.
-0000fc40: 4204 3004 3504 4204 3504 4104 4c00 2004  B.0.5.B.5.A.L. .
-0000fc50: 3704 3004 3304 4004 4304 3704 3804 4204  7.0.3.@.C.7.8.B.
-0000fc60: 4c00 2004 3e04 4204 4704 5104 4200 2004  L. .>.B.G.Q.B. .
-0000fc70: 3e00 2004 3f04 3e04 3404 4204 3204 3504  >. .?.>.4.B.2.5.
-0000fc80: 4004 3604 3404 5104 3d04 3d04 4b04 4500  @.6.4.Q.=.=.K.E.
-0000fc90: 2004 4104 3404 3504 3b04 3a04 3004 4500   .A.4.5.;.:.0.E.
-0000fca0: 2004 3204 3c04 3504 4104 4204 3e00 2004   .2.<.5.A.B.>. .
-0000fcb0: 3e04 4204 4704 5104 4204 3000 2004 3f04  >.B.G.Q.B.0. .?.
-0000fcc0: 3e00 2004 1004 3a04 4204 3804 3204 3d04  >. ...:.B.8.2.=.
-0000fcd0: 3e04 4104 4204 3808 0000 0000 0600 0000  >.A.B.8.........
-0000fce0: 3f59 6f75 2074 7279 2074 6f20 696d 706f  ?You try to impo
-0000fcf0: 7274 2054 7261 6465 2063 6f6e 6669 6d61  rt Trade confima
-0000fd00: 7469 6f6e 2072 6570 6f72 742c 206e 6f74  tion report, not
-0000fd10: 2041 6374 6976 6974 7920 7265 706f 7274   Activity report
-0000fd20: 0700 0000 0d53 7461 7465 6d65 6e74 4942  .....StatementIB
-0000fd30: 4b52 0103 0000 0052 041d 0435 0432 043e  KR.....R...5.2.>
-0000fd40: 0437 043c 043e 0436 043d 043e 0020 0440  .7.<.>.6.=.>. .@
-0000fd50: 0430 0441 043f 043e 0437 043d 0430 0442  .0.A.?.>.7.=.0.B
-0000fd60: 044c 0020 043e 043f 0438 0441 0430 043d  .L. .>.?.8.A.0.=
-0000fd70: 0438 0435 0020 0434 0438 0432 0438 0434  .8.5. .4.8.2.8.4
-0000fd80: 0435 043d 0434 0430 0020 0800 0000 0006  .5.=.4.0. ......
-0000fd90: 0000 0021 4361 6e27 7420 7061 7273 6520  ...!Can't parse 
-0000fda0: 4469 7669 6465 6e64 2064 6573 6372 6970  Dividend descrip
-0000fdb0: 7469 6f6e 2007 0000 000c 5374 6174 656d  tion .....Statem
-0000fdc0: 656e 744a 3254 0103 0000 001c 0414 0421  entJ2T.........!
-0000fdd0: 0020 0437 0430 0433 0440 0443 0436 0435  . .7.0.3.@.C.6.5
-0000fde0: 043d 044b 003a 0020 0800 0000 0006 0000  .=.K.:. ........
-0000fdf0: 0016 4361 7368 2062 616c 616e 6365 7320  ..Cash balances 
-0000fe00: 6c6f 6164 6564 3a20 0700 0000 0c53 7461  loaded: .....Sta
-0000fe10: 7465 6d65 6e74 4a32 5401 0300 0000 3a04  tementJ2T.....:.
-0000fe20: 1404 3504 3d04 3504 3604 3d04 4b04 4500  ..5.=.5.6.=.K.E.
-0000fe30: 2004 3e04 3f04 3504 4004 3004 4604 3804   .>.?.5.@.0.F.8.
-0000fe40: 3900 2004 3704 3004 3304 4004 4304 3604  9. .7.0.3.@.C.6.
-0000fe50: 3504 3d04 3e00 3a00 2008 0000 0000 0600  5.=.>.:. .......
-0000fe60: 0000 1843 6173 6820 6f70 6572 6174 696f  ...Cash operatio
-0000fe70: 6e73 206c 6f61 6465 643a 2007 0000 000c  ns loaded: .....
-0000fe80: 5374 6174 656d 656e 744a 3254 0103 0000  StatementJ2T....
-0000fe90: 0048 0421 0434 0435 043b 043a 0438 0020  .H.!.4.5.;.:.8. 
-0000fea0: 0441 0020 043a 0440 0438 043f 0442 043e  .A. .:.@.8.?.B.>
-0000feb0: 002d 0432 0430 043b 044e 0442 0430 043c  .-.2.0.;.N.B.0.<
-0000fec0: 0438 0020 0437 0430 0433 0440 0443 0436  .8. .7.0.3.@.C.6
-0000fed0: 0435 043d 044b 003a 0020 0800 0000 0006  .5.=.K.:. ......
-0000fee0: 0000 0016 4372 7970 746f 2074 7261 6465  ....Crypto trade
-0000fef0: 7320 6c6f 6164 6564 3a20 0700 0000 0c53  s loaded: .....S
-0000ff00: 7461 7465 6d65 6e74 4a32 5401 0300 0000  tatementJ2T.....
-0000ff10: 5004 1200 2004 3e04 3f04 3804 4104 3004  P... .>.?.8.A.0.
-0000ff20: 3d04 3804 3800 2004 3404 3804 3204 3804  =.8.8. .4.8.2.8.
-0000ff30: 3404 3504 3d04 3404 3000 2004 3e04 4204  4.5.=.4.0. .>.B.
-0000ff40: 4104 4304 4204 4104 4204 3204 4304 4e04  A.C.B.A.B.2.C.N.
-0000ff50: 4200 2004 3404 3004 3d04 3d04 4b04 3500  B. .4.0.=.=.K.5.
-0000ff60: 2008 0000 0000 0600 0000 2444 6976 6964   .........$Divid
-0000ff70: 656e 6420 6465 7363 7269 7074 696f 6e20  end description 
-0000ff80: 6d69 7373 2073 6f6d 6520 6461 7461 2007  miss some data .
-0000ff90: 0000 000c 5374 6174 656d 656e 744a 3254  ....StatementJ2T
-0000ffa0: 0103 0000 004e 0414 0438 0432 0438 0434  .....N...8.2.8.4
-0000ffb0: 0435 043d 0434 0020 043d 0435 0020 043d  .5.=.4. .=.5. .=
-0000ffc0: 0430 0439 0434 0435 043d 0020 0434 043b  .0.9.4.5.=. .4.;
-0000ffd0: 044f 0020 0441 043f 0438 0441 0430 043d  .O. .A.?.8.A.0.=
-0000ffe0: 0438 044f 0020 043d 0430 043b 043e 0433  .8.O. .=.0.;.>.3
-0000fff0: 0430 0020 0800 0000 0006 0000 001f 4469  .0. ..........Di
-00010000: 7669 6465 6e64 2066 6f72 2074 6178 2077  vidend for tax w
-00010010: 6173 206e 6f74 2066 6f75 6e64 2007 0000  as not found ...
-00010020: 000c 5374 6174 656d 656e 744a 3254 0103  ..StatementJ2T..
-00010030: 0000 0044 0422 0440 0430 043d 0437 0430  ...D.".@.0.=.7.0
-00010040: 043a 0446 0438 044f 0020 043f 0440 043e  .:.F.8.O. .?.@.>
-00010050: 043f 0443 0449 0435 043d 0430 0020 043f  .?.C.I.5.=.0. .?
-00010060: 0440 0438 0020 0438 043c 043f 043e 0440  .@.8. .8.<.?.>.@
-00010070: 0442 0435 003a 0020 0800 0000 0006 0000  .B.5.:. ........
-00010080: 001f 496d 706f 7274 2073 6b69 7070 6564  ..Import skipped
-00010090: 206f 6620 7472 616e 7361 6374 696f 6e3a   of transaction:
-000100a0: 2007 0000 000c 5374 6174 656d 656e 744a   .....StatementJ
-000100b0: 3254 0103 0000 0014 004a 0075 0073 0074  2T.......J.u.s.t
-000100c0: 0032 0054 0072 0061 0064 0065 0800 0000  .2.T.r.a.d.e....
-000100d0: 0006 0000 000a 4a75 7374 3254 7261 6465  ......Just2Trade
-000100e0: 0700 0000 0c53 7461 7465 6d65 6e74 4a32  .....StatementJ2
-000100f0: 5401 0300 0000 3204 1e04 4204 4704 5104  T.....2...B.G.Q.
-00010100: 4200 2000 4a00 7500 7300 7400 3200 5400  B. .J.u.s.t.2.T.
-00010110: 7200 6100 6400 6500 2000 2800 2a00 2e00  r.a.d.e. .(.*...
-00010120: 7800 6c00 7300 7800 2908 0000 0000 0600  x.l.s.x.).......
-00010130: 0000 1d4a 7573 7432 5472 6164 6520 7374  ...Just2Trade st
-00010140: 6174 656d 656e 7420 282a 2e78 6c73 7829  atement (*.xlsx)
-00010150: 0700 0000 0c53 7461 7465 6d65 6e74 4a32  .....StatementJ2
-00010160: 5401 0300 0000 1c04 2604 1100 2004 3704  T.......&... .7.
-00010170: 3004 3304 4004 4304 3604 3504 3d04 4b00  0.3.@.C.6.5.=.K.
-00010180: 3a00 2008 0000 0000 0600 0000 1353 6563  :. ..........Sec
-00010190: 7572 6974 6965 7320 6c6f 6164 6564 3a20  urities loaded: 
-000101a0: 0700 0000 0c53 7461 7465 6d65 6e74 4a32  .....StatementJ2
-000101b0: 5401 0300 0000 3804 2104 3404 3504 3b04  T.....8.!.4.5.;.
-000101c0: 3a04 3800 2004 4100 2004 3004 3a04 4604  :.8. .A. .0.:.F.
-000101d0: 3804 4f04 3c04 3800 2004 3704 3004 3304  8.O.<.8. .7.0.3.
-000101e0: 4004 4304 3604 3504 3d04 4b00 3a00 2008  @.C.6.5.=.K.:. .
-000101f0: 0000 0000 0600 0000 1553 746f 636b 2074  .........Stock t
-00010200: 7261 6465 7320 6c6f 6164 6564 3a20 0700  rades loaded: ..
-00010210: 0000 0c53 7461 7465 6d65 6e74 4a32 5401  ...StatementJ2T.
-00010220: 0300 0000 4004 1d04 3504 3804 3704 3204  ....@...5.8.7.2.
-00010230: 3504 4104 4204 3d04 3004 4f00 2004 3404  5.A.B.=.0.O. .4.
-00010240: 3504 3d04 3504 3604 3d04 3004 4f00 2004  5.=.5.6.=.0.O. .
-00010250: 4204 4004 3004 3d04 3704 3004 3a04 4604  B.@.0.=.7.0.:.F.
-00010260: 3804 4f00 2008 0000 0000 0600 0000 1e55  8.O. ..........U
-00010270: 6e6b 6e6f 776e 2063 6173 6820 7472 616e  nknown cash tran
-00010280: 7361 6374 696f 6e20 7479 7065 2007 0000  saction type ...
-00010290: 000c 5374 6174 656d 656e 744a 3254 0103  ..StatementJ2T..
-000102a0: 0000 0030 041d 0435 0438 0437 0432 0435  ...0...5.8.7.2.5
-000102b0: 0441 0442 043d 044b 0439 0020 0442 0438  .A.B.=.K.9. .B.8
-000102c0: 043f 0020 0441 0434 0435 043b 043a 0438  .?. .A.4.5.;.:.8
-000102d0: 003a 0020 0800 0000 0006 0000 0014 556e  .:. ..........Un
-000102e0: 6b6e 6f77 6e20 7472 6164 6520 7479 7065  known trade type
-000102f0: 3a20 0700 0000 0c53 7461 7465 6d65 6e74  : .....Statement
-00010300: 4a32 5401 0300 0000 4a04 1d04 3504 3f04  J2T.....J...5.?.
-00010310: 3e04 3404 3404 3504 4004 3604 3804 3204  >.4.4.5.@.6.8.2.
-00010320: 3004 3504 3c04 3004 4f00 2004 3404 3504  0.5.<.0.O. .4.5.
-00010330: 3d04 3504 3604 3d04 3004 4f00 2004 4204  =.5.6.=.0.O. .B.
-00010340: 4004 3004 3d04 3704 3004 3a04 4604 3804  @.0.=.7.0.:.F.8.
-00010350: 4f00 2008 0000 0000 0600 0000 1e55 6e73  O. ..........Uns
-00010360: 7570 7070 6f72 7465 6420 6361 7368 2074  uppported cash t
-00010370: 7261 6e73 6163 7469 6f6e 2007 0000 000c  ransaction .....
-00010380: 5374 6174 656d 656e 744a 3254 0103 0000  StatementJ2T....
-00010390: 003a 0414 0435 043d 0435 0436 043d 044b  .:...5.=.5.6.=.K
-000103a0: 0445 0020 043e 043f 0435 0440 0430 0446  .E. .>.?.5.@.0.F
-000103b0: 0438 0439 0020 0437 0430 0433 0440 0443  .8.9. .7.0.3.@.C
-000103c0: 0436 0435 043d 043e 003a 0020 0800 0000  .6.5.=.>.:. ....
-000103d0: 0006 0000 0018 4361 7368 206f 7065 7261  ......Cash opera
-000103e0: 7469 6f6e 7320 6c6f 6164 6564 3a20 0700  tions loaded: ..
-000103f0: 0000 0c53 7461 7465 6d65 6e74 4b49 5401  ...StatementKIT.
-00010400: 0300 0000 7604 1d04 3004 3b04 3e04 3300  ....v...0.;.>.3.
-00010410: 2004 3d04 3000 2004 3404 3804 3204 3804   .=.0. .4.8.2.8.
-00010420: 3404 3504 3d04 3404 4b00 2004 3d04 3500  4.5.=.4.K. .=.5.
-00010430: 2004 3f04 3e04 3404 3404 3504 4004 3604   .?.>.4.4.5.@.6.
-00010440: 3804 3204 3004 3504 4204 4104 4f00 2004  8.2.0.5.B.A.O. .
-00010450: 3404 3b04 4f00 2004 3104 4004 3e04 3a04  4.;.O. .1.@.>.:.
-00010460: 3504 4004 3000 2004 1a04 1804 2200 2d04  5.@.0. .....".-.
-00010470: 4404 3804 3d04 3004 3d04 4108 0000 0000  D.8.=.0.=.A.....
-00010480: 0600 0000 3e44 6976 6964 656e 6420 7461  ....>Dividend ta
-00010490: 7865 7320 6172 6520 6e6f 7420 7375 7070  xes are not supp
-000104a0: 6f72 7465 6420 666f 7220 4b49 5420 6272  orted for KIT br
-000104b0: 6f6b 6572 2073 7461 7465 6d65 6e74 7320  oker statements 
-000104c0: 7965 7407 0000 000c 5374 6174 656d 656e  yet.....Statemen
-000104d0: 744b 4954 0103 0000 0014 041a 0418 0422  tKIT..........."
-000104e0: 0020 0424 0438 043d 0430 043d 0441 0800  . .$.8.=.0.=.A..
-000104f0: 0000 0006 0000 000b 4b49 5420 4669 6e61  ........KIT Fina
-00010500: 6e63 6507 0000 000c 5374 6174 656d 656e  nce.....Statemen
-00010510: 744b 4954 0103 0000 0032 041e 0442 0447  tKIT.....2...B.G
-00010520: 0451 0442 0020 041a 0418 0422 0020 0424  .Q.B. .....". .$
-00010530: 0438 043d 0430 043d 0441 0020 0028 002a  .8.=.0.=.A. .(.*
-00010540: 002e 0078 006c 0073 0078 0029 0800 0000  ...x.l.s.x.)....
-00010550: 0006 0000 001e 4b49 5420 4669 6e61 6e63  ......KIT Financ
-00010560: 6520 7374 6174 656d 656e 7420 282a 2e78  e statement (*.x
-00010570: 6c73 7829 0700 0000 0c53 7461 7465 6d65  lsx).....Stateme
-00010580: 6e74 4b49 5401 0300 0000 2404 2104 3404  ntKIT.....$.!.4.
-00010590: 3504 3b04 3a04 3800 2004 3704 3004 3304  5.;.:.8. .7.0.3.
-000105a0: 4004 4304 3604 3504 3d04 4b00 3a00 2008  @.C.6.5.=.K.:. .
-000105b0: 0000 0000 0600 0000 0f54 7261 6465 7320  .........Trades 
-000105c0: 6c6f 6164 6564 3a20 0700 0000 0c53 7461  loaded: .....Sta
-000105d0: 7465 6d65 6e74 4b49 5401 0300 0000 3004  tementKIT.....0.
-000105e0: 1d04 3504 3804 3704 3204 3504 4104 4204  ..5.8.7.2.5.A.B.
-000105f0: 3d04 4b04 3900 2004 4204 3804 3f00 2004  =.K.9. .B.8.?. .
-00010600: 4104 3404 3504 3b04 3a04 3800 3a00 2008  A.4.5.;.:.8.:. .
-00010610: 0000 0000 0600 0000 1455 6e6b 6e6f 776e  .........Unknown
-00010620: 2074 7261 6465 2074 7970 653a 2007 0000   trade type: ...
-00010630: 000c 5374 6174 656d 656e 744b 4954 0103  ..StatementKIT..
-00010640: 0000 004a 041d 0435 043f 043e 0434 0434  ...J...5.?.>.4.4
-00010650: 0435 0440 0436 0438 0432 0430 0435 043c  .5.@.6.8.2.0.5.<
-00010660: 0430 044f 0020 0434 0435 043d 0435 0436  .0.O. .4.5.=.5.6
-00010670: 043d 0430 044f 0020 0442 0440 0430 043d  .=.0.O. .B.@.0.=
-00010680: 0437 0430 043a 0446 0438 044f 0020 0800  .7.0.:.F.8.O. ..
-00010690: 0000 0006 0000 001e 556e 7375 7070 706f  ........Unsupppo
-000106a0: 7274 6564 2063 6173 6820 7472 616e 7361  rted cash transa
-000106b0: 6374 696f 6e20 0700 0000 0c53 7461 7465  ction .....State
-000106c0: 6d65 6e74 4b49 5401 0300 0000 2204 2104  mentKIT.....".!.
-000106d0: 4704 3504 4204 3000 2004 3704 3004 3304  G.5.B.0. .7.0.3.
-000106e0: 4004 4304 3604 3504 3d04 4b00 3a00 2008  @.C.6.5.=.K.:. .
-000106f0: 0000 0000 0600 0000 1141 6363 6f75 6e74  .........Account
-00010700: 7320 6c6f 6164 6564 3a20 0700 0000 1353  s loaded: .....S
-00010710: 7461 7465 6d65 6e74 4f70 656e 4272 6f6b  tatementOpenBrok
-00010720: 6572 0103 0000 0064 041e 0442 0441 0443  er.....d...B.A.C
-00010730: 0442 0441 0442 0432 0443 044e 0442 0020  .B.A.B.2.C.N.B. 
-00010740: 0434 0430 043d 043d 044b 0435 0020 0432  .4.0.=.=.K.5. .2
-00010750: 0020 043e 043f 0438 0441 0430 043d 0438  . .>.?.8.A.0.=.8
-00010760: 0438 0020 043f 043e 0433 0430 0448 0435  .8. .?.>.3.0.H.5
-00010770: 043d 0438 044f 0020 043e 0431 043b 0438  .=.8.O. .>.1.;.8
-00010780: 0433 0430 0446 0438 0438 0020 0800 0000  .3.0.F.8.8. ....
-00010790: 0006 0000 002a 426f 6e64 2072 6570 6179  .....*Bond repay
-000107a0: 6d65 6e74 2064 6573 6372 6970 7469 6f6e  ment description
-000107b0: 206d 6973 7320 736f 6d65 2064 6174 6120   miss some data 
-000107c0: 0700 0000 1353 7461 7465 6d65 6e74 4f70  .....StatementOp
-000107d0: 656e 4272 6f6b 6572 0103 0000 0068 041d  enBroker.....h..
-000107e0: 0435 0432 043e 0437 043c 043e 0436 043d  .5.2.>.7.<.>.6.=
-000107f0: 043e 0020 0440 0430 0441 043f 043e 0437  .>. .@.0.A.?.>.7
-00010800: 043d 0430 0442 044c 0020 043d 0430 0437  .=.0.B.L. .=.0.7
-00010810: 0432 0430 043d 0438 0435 0020 043e 0431  .2.0.=.8.5. .>.1
-00010820: 043b 0438 0433 0430 0446 0438 0438 0020  .;.8.3.0.F.8.8. 
-00010830: 0432 0020 043e 043f 0438 0441 0430 043d  .2. .>.?.8.A.0.=
-00010840: 0438 0438 0020 0800 0000 0006 0000 0028  .8.8. .........(
-00010850: 4361 6e27 7420 6465 7465 6374 2062 6f6e  Can't detect bon
-00010860: 6420 6e61 6d65 2066 726f 6d20 6465 7363  d name from desc
-00010870: 7269 7074 696f 6e20 0700 0000 1353 7461  ription .....Sta
-00010880: 7465 6d65 6e74 4f70 656e 4272 6f6b 6572  tementOpenBroker
-00010890: 0103 0000 0062 041d 0435 0432 043e 0437  .....b...5.2.>.7
-000108a0: 043c 043e 0436 043d 043e 0020 043e 043f  .<.>.6.=.>. .>.?
-000108b0: 0440 0435 0434 0435 043b 0438 0442 044c  .@.5.4.5.;.8.B.L
-000108c0: 0020 0442 0438 043f 002f 043a 043e 043b  . .B.8.?./.:.>.;
-000108d0: 0438 0447 0435 0441 0442 0432 043e 0020  .8.G.5.A.B.2.>. 
-000108e0: 0434 043b 044f 0020 0441 0434 0435 043b  .4.;.O. .A.4.5.;
-000108f0: 043a 0438 003a 0020 0800 0000 0006 0000  .:.8.:. ........
-00010900: 0025 4361 6e27 7420 6465 7465 726d 696e  .%Can't determin
-00010910: 6520 7472 6164 6520 7479 7065 2f71 7561  e trade type/qua
-00010920: 6e74 6974 793a 2007 0000 0013 5374 6174  ntity: .....Stat
-00010930: 656d 656e 744f 7065 6e42 726f 6b65 7201  ementOpenBroker.
-00010940: 0300 0000 6804 1d04 3504 3204 3e04 3704  ....h...5.2.>.7.
-00010950: 3c04 3e04 3604 3d04 3e00 2004 3e04 3f04  <.>.6.=.>. .>.?.
-00010960: 4004 3504 3404 3504 3b04 3804 4204 4c00  @.5.4.5.;.8.B.L.
-00010970: 2004 4104 4704 5104 4200 2004 3404 3b04   .A.G.Q.B. .4.;.
-00010980: 4f00 2004 3404 3504 3d04 3504 3604 3d04  O. .4.5.=.5.6.=.
-00010990: 3e04 3900 2004 4204 4004 3004 3d04 3704  >.9. .B.@.0.=.7.
-000109a0: 3004 3a04 4604 3804 3800 3a00 2008 0000  0.:.F.8.8.:. ...
-000109b0: 0000 0600 0000 2743 616e 2774 2066 696e  ......'Can't fin
-000109c0: 6420 6163 636f 756e 7420 666f 7220 6361  d account for ca
-000109d0: 7368 206f 7065 7261 7469 6f6e 3a20 0700  sh operation: ..
-000109e0: 0000 1353 7461 7465 6d65 6e74 4f70 656e  ...StatementOpen
-000109f0: 4272 6f6b 6572 0103 0000 0044 041d 0435  Broker.....D...5
-00010a00: 0432 043e 0437 043c 043e 0436 043d 043e  .2.>.7.<.>.6.=.>
-00010a10: 0020 043d 0430 0439 0442 0438 0020 0441  . .=.0.9.B.8. .A
-00010a20: 0447 0451 0442 0020 0434 043b 044f 0020  .G.Q.B. .4.;.O. 
-00010a30: 0441 0434 0435 043b 043a 0438 003a 0020  .A.4.5.;.:.8.:. 
-00010a40: 0800 0000 0006 0000 001e 4361 6e27 7420  ..........Can't 
-00010a50: 6669 6e64 2061 6363 6f75 6e74 2066 6f72  find account for
-00010a60: 2074 7261 6465 3a20 0700 0000 1353 7461   trade: .....Sta
-00010a70: 7465 6d65 6e74 4f70 656e 4272 6f6b 6572  tementOpenBroker
-00010a80: 0103 0000 0050 041d 0435 0432 043e 0437  .....P...5.2.>.7
-00010a90: 043c 043e 0436 043d 043e 0020 043d 0430  .<.>.6.=.>. .=.0
-00010aa0: 0439 0442 0438 0020 0437 0430 043f 0438  .9.B.8. .7.0.?.8
-00010ab0: 0441 044c 0020 0441 043f 0438 0441 0430  .A.L. .A.?.8.A.0
-00010ac0: 043d 0438 044f 0020 0426 0411 0020 0434  .=.8.O. .&... .4
-00010ad0: 043b 044f 0020 0800 0000 0006 0000 0029  .;.O. .........)
-00010ae0: 4361 6e27 7420 6669 6e64 2061 7373 6574  Can't find asset
-00010af0: 2063 616e 6365 6c6c 6174 696f 6e20 7265   cancellation re
-00010b00: 636f 7264 2066 6f72 2007 0000 0013 5374  cord for .....St
-00010b10: 6174 656d 656e 744f 7065 6e42 726f 6b65  atementOpenBroke
-00010b20: 7201 0300 0000 3204 1d04 3500 2004 3d04  r.....2...5. .=.
-00010b30: 3004 3904 3404 3504 3d04 3000 2004 2604  0.9.4.5.=.0. .&.
-00010b40: 1100 2004 3404 3b04 4f00 2004 3a04 4304  .. .4.;.O. .:.C.
-00010b50: 3f04 3e04 3d04 3000 2008 0000 0000 0600  ?.>.=.0. .......
-00010b60: 0000 2343 616e 2774 2066 696e 6420 6173  ..#Can't find as
-00010b70: 7365 7420 666f 7220 626f 6e64 2069 6e74  set for bond int
-00010b80: 6572 6573 7420 0700 0000 1353 7461 7465  erest .....State
-00010b90: 6d65 6e74 4f70 656e 4272 6f6b 6572 0103  mentOpenBroker..
-00010ba0: 0000 003c 041d 0435 0432 043e 0437 043c  ...<...5.2.>.7.<
-00010bb0: 043e 0436 043d 043e 0020 0441 043e 043f  .>.6.=.>. .A.>.?
-00010bc0: 043e 0441 0442 0430 0432 0438 0442 044c  .>.A.B.0.2.8.B.L
-00010bd0: 0020 0426 0411 0020 0434 043b 044f 0020  . .&... .4.;.O. 
-00010be0: 0800 0000 0006 0000 0016 4361 6e27 7420  ..........Can't 
-00010bf0: 6d61 7463 6820 6173 7365 7420 666f 7220  match asset for 
-00010c00: 0700 0000 1353 7461 7465 6d65 6e74 4f70  .....StatementOp
-00010c10: 656e 4272 6f6b 6572 0103 0000 0066 041d  enBroker.....f..
-00010c20: 0435 0432 043e 0437 043c 043e 0436 043d  .5.2.>.7.<.>.6.=
-00010c30: 043e 0020 0440 0430 0441 043f 043e 0437  .>. .@.0.A.?.>.7
-00010c40: 043d 0430 0442 044c 0020 043e 043f 0438  .=.0.B.L. .>.?.8
-00010c50: 0441 0430 043d 0438 0435 0020 043f 043e  .A.0.=.8.5. .?.>
-00010c60: 0433 0430 0448 0435 043d 0438 044f 0020  .3.0.H.5.=.8.O. 
-00010c70: 043e 0431 043b 0438 0433 0430 0446 0438  .>.1.;.8.3.0.F.8
-00010c80: 0438 0020 0800 0000 0006 0000 0024 4361  .8. .........$Ca
-00010c90: 6e27 7420 7061 7273 6520 426f 6e64 204d  n't parse Bond M
-00010ca0: 6174 7572 6520 6465 7363 7269 7074 696f  ature descriptio
-00010cb0: 6e20 0700 0000 1353 7461 7465 6d65 6e74  n .....Statement
-00010cc0: 4f70 656e 4272 6f6b 6572 0103 0000 004c  OpenBroker.....L
-00010cd0: 041d 0435 0432 043e 0437 043c 043e 0436  ...5.2.>.7.<.>.6
-00010ce0: 043d 043e 0020 0440 0430 0441 043f 043e  .=.>. .@.0.A.?.>
-00010cf0: 0437 043d 0430 0442 044c 0020 043e 043f  .7.=.0.B.L. .>.?
-00010d00: 0438 0441 0430 043d 0438 0435 0020 043a  .8.A.0.=.8.5. .:
-00010d10: 0443 043f 043e 043d 0430 0020 0800 0000  .C.?.>.=.0. ....
-00010d20: 0006 0000 0021 4361 6e27 7420 7061 7273  .....!Can't pars
-00010d30: 6520 496e 7465 7265 7374 2064 6573 6372  e Interest descr
-00010d40: 6970 7469 6f6e 2007 0000 0013 5374 6174  iption .....Stat
-00010d50: 656d 656e 744f 7065 6e42 726f 6b65 7201  ementOpenBroker.
-00010d60: 0300 0000 6604 1d04 3504 3204 3e04 3704  ....f...5.2.>.7.
-00010d70: 3c04 3e04 3604 3d04 3e00 2004 4004 3004  <.>.6.=.>. .@.0.
-00010d80: 4104 3f04 3e04 3704 3d04 3004 4204 4c00  A.?.>.7.=.0.B.L.
-00010d90: 2004 3e04 3f04 3804 4104 3004 3d04 3804   .>.?.8.A.0.=.8.
-00010da0: 3500 2004 3f04 3e04 3304 3004 4804 3504  5. .?.>.3.0.H.5.
-00010db0: 3d04 3804 4f00 2004 3e04 3104 3b04 3804  =.8.O. .>.1.;.8.
-00010dc0: 3304 3004 4604 3804 3800 2008 0000 0000  3.0.F.8.8. .....
-00010dd0: 0600 0000 2743 616e 2774 2070 6172 7365  ....'Can't parse
-00010de0: 2062 6f6e 6420 7265 7061 796d 656e 7420   bond repayment 
-00010df0: 6465 7363 7269 7074 696f 6e20 0700 0000  description ....
-00010e00: 1353 7461 7465 6d65 6e74 4f70 656e 4272  .StatementOpenBr
-00010e10: 6f6b 6572 0103 0000 003a 0414 0435 043d  oker.....:...5.=
-00010e20: 0435 0436 043d 044b 0445 0020 043e 043f  .5.6.=.K.E. .>.?
-00010e30: 0435 0440 0430 0446 0438 0439 0020 0437  .5.@.0.F.8.9. .7
-00010e40: 0430 0433 0440 0443 0436 0435 043d 043e  .0.3.@.C.6.5.=.>
-00010e50: 003a 0020 0800 0000 0006 0000 0018 4361  .:. ..........Ca
-00010e60: 7368 206f 7065 7261 7469 6f6e 7320 6c6f  sh operations lo
-00010e70: 6164 6564 3a20 0700 0000 1353 7461 7465  aded: .....State
-00010e80: 6d65 6e74 4f70 656e 4272 6f6b 6572 0103  mentOpenBroker..
-00010e90: 0000 0048 041e 0442 0441 0443 0442 0441  ...H...B.A.C.B.A
-00010ea0: 0442 0432 0443 044e 0442 0020 0434 0430  .B.2.C.N.B. .4.0
-00010eb0: 043d 043d 044b 0435 0020 0432 0020 043e  .=.=.K.5. .2. .>
-00010ec0: 043f 0438 0441 0430 043d 0438 0020 043a  .?.8.A.0.=.8. .:
-00010ed0: 0443 043f 043e 043d 0430 0020 0800 0000  .C.?.>.=.0. ....
-00010ee0: 0006 0000 0024 496e 7465 7265 7374 2064  .....$Interest d
-00010ef0: 6573 6372 6970 7469 6f6e 206d 6973 7320  escription miss 
-00010f00: 736f 6d65 2064 6174 6120 0700 0000 1353  some data .....S
-00010f10: 7461 7465 6d65 6e74 4f70 656e 4272 6f6b  tatementOpenBrok
-00010f20: 6572 0103 0000 0054 0417 0430 0433 0440  er.....T...0.3.@
-00010f30: 0443 0437 043a 0430 0020 043e 0442 0447  .C.7.:.0. .>.B.G
-00010f40: 0451 0442 0430 0020 041e 0442 043a 0440  .Q.B.0. ...B.:.@
-00010f50: 044b 0442 0438 0435 0020 0431 0440 043e  .K.B.8.5. .1.@.>
-00010f60: 043a 0435 0440 0020 0434 043b 044f 0020  .:.5.@. .4.;.O. 
-00010f70: 0441 0447 0451 0442 0430 0020 0800 0000  .A.G.Q.B.0. ....
-00010f80: 0006 0000 0027 4c6f 6164 204f 7065 6e20  .....'Load Open 
-00010f90: 4272 6f6b 6572 2073 7461 7465 6d65 6e74  Broker statement
-00010fa0: 2066 6f72 2061 6363 6f75 6e74 2007 0000   for account ...
-00010fb0: 0013 5374 6174 656d 656e 744f 7065 6e42  ..StatementOpenB
-00010fc0: 726f 6b65 7201 0300 0000 5604 1d04 3004  roker.....V...0.
-00010fd0: 3904 3404 3504 3d04 4b00 2004 3d04 3504  9.4.5.=.K. .=.5.
-00010fe0: 4104 3a04 3e04 3b04 4c04 3a04 3e00 2004  A.:.>.;.L.:.>. .
-00010ff0: 3704 3004 3f04 3804 4104 3504 3900 2004  7.0.?.8.A.5.9. .
-00011000: 3f04 3e04 3304 3004 4804 3504 3d04 3804  ?.>.3.0.H.5.=.8.
-00011010: 4f00 2004 2604 1100 2004 3404 3b04 4f00  O. .&... .4.;.O.
-00011020: 2008 0000 0000 0600 0000 264d 756c 7469   .........&Multi
-00011030: 706c 6520 6173 7365 7420 6361 6e63 656c  ple asset cancel
-00011040: 6c61 7469 6f6e 206d 6174 6368 2066 6f72  lation match for
-00011050: 2007 0000 0013 5374 6174 656d 656e 744f   .....StatementO
-00011060: 7065 6e42 726f 6b65 7201 0300 0000 7404  penBroker.....t.
-00011070: 1d04 3504 4104 3a04 3e04 3b04 4c04 3a04  ..5.A.:.>.;.L.:.
-00011080: 3e00 2004 4104 3e04 3204 3f04 3004 3404  >. .A.>.2.?.0.4.
-00011090: 3504 3d04 3804 3900 2004 3404 3b04 4f00  5.=.8.9. .4.;.O.
-000110a0: 2004 4104 3804 3c04 3204 3e04 3b04 3000   .A.8.<.2.>.;.0.
-000110b0: 2c00 2004 3804 4104 3f04 3e04 3b04 4c04  ,. .8.A.?.>.;.L.
-000110c0: 3704 4304 3504 3c04 3e04 3304 3e00 2004  7.C.5.<.>.3.>. .
-000110d0: 3104 4004 3e04 3a04 3504 4004 3e04 3c00  1.@.>.:.5.@.>.<.
-000110e0: 3a00 2008 0000 0000 0600 0000 224d 756c  :. ........."Mul
-000110f0: 7469 706c 6520 6d61 7463 6820 666f 7220  tiple match for 
-00011100: 6272 6f6b 6572 2073 796d 626f 6c3a 2007  broker symbol: .
-00011110: 0000 0013 5374 6174 656d 656e 744f 7065  ....StatementOpe
-00011120: 6e42 726f 6b65 7201 0300 0000 4404 1d04  nBroker.....D...
-00011130: 3504 4104 3a04 3e04 3b04 4c04 3a04 3e00  5.A.:.>.;.L.:.>.
-00011140: 2004 4104 3e04 3204 3f04 3004 3404 3504   .A.>.2.?.0.4.5.
-00011150: 3d04 3804 3900 2004 3404 3b04 4f00 2004  =.8.9. .4.;.O. .
-00011160: 4104 3804 3c04 3204 3e04 3b04 3000 3a00  A.8.<.2.>.;.0.:.
-00011170: 2008 0000 0000 0600 0000 1b4d 756c 7469   ..........Multi
-00011180: 706c 6520 6d61 7463 6820 666f 7220 7379  ple match for sy
-00011190: 6d62 6f6c 3a20 0700 0000 1353 7461 7465  mbol: .....State
-000111a0: 6d65 6e74 4f70 656e 4272 6f6b 6572 0103  mentOpenBroker..
-000111b0: 0000 001e 041e 0442 043a 0440 044b 0442  .......B.:.@.K.B
-000111c0: 0438 0435 0020 0431 0440 043e 043a 0435  .8.5. .1.@.>.:.5
-000111d0: 0440 0800 0000 0006 0000 000b 4f70 656e  .@..........Open
-000111e0: 2042 726f 6b65 7207 0000 0013 5374 6174   Broker.....Stat
-000111f0: 656d 656e 744f 7065 6e42 726f 6b65 7201  ementOpenBroker.
-00011200: 0300 0000 3c04 1e04 4204 4704 5104 4200  ....<...B.G.Q.B.
-00011210: 2004 3104 4004 3e04 3a04 3504 4004 3000   .1.@.>.:.5.@.0.
-00011220: 2004 1e04 4204 3a04 4004 4b04 4204 3804   ...B.:.@.K.B.8.
-00011230: 3500 2000 2800 2a00 2e00 7800 6d00 6c00  5. .(.*...x.m.l.
-00011240: 2908 0000 0000 0600 0000 1d4f 7065 6e20  )..........Open 
-00011250: 4272 6f6b 6572 2073 7461 7465 6d65 6e74  Broker statement
-00011260: 2028 2a2e 786d 6c29 0700 0000 1353 7461   (*.xml).....Sta
-00011270: 7465 6d65 6e74 4f70 656e 4272 6f6b 6572  tementOpenBroker
-00011280: 0103 0000 0054 0417 0430 0433 043e 043b  .....T...0.3.>.;
-00011290: 043e 0432 043e 043a 0020 043e 0442 0447  .>.2.>.:. .>.B.G
-000112a0: 0451 0442 0430 0020 041e 0442 043a 0440  .Q.B.0. ...B.:.@
-000112b0: 044b 0442 0438 0435 0020 0431 0440 043e  .K.B.8.5. .1.@.>
-000112c0: 043a 0435 0440 0020 043d 0435 0020 043d  .:.5.@. .=.5. .=
-000112d0: 0430 0439 0434 0435 043d 0800 0000 0006  .0.9.4.5.=......
-000112e0: 0000 0022 4f70 656e 2062 726f 6b65 7220  ..."Open broker 
-000112f0: 7265 706f 7274 2074 6974 6c65 206e 6f74  report title not
-00011300: 2066 6f75 6e64 0700 0000 1353 7461 7465   found.....State
-00011310: 6d65 6e74 4f70 656e 4272 6f6b 6572 0103  mentOpenBroker..
-00011320: 0000 0038 041e 043f 0435 0440 0430 0446  ...8...?.5.@.0.F
-00011330: 0438 044f 0020 043d 0435 0020 043f 043e  .8.O. .=.5. .?.>
-00011340: 0434 0434 0435 0440 0436 0438 0432 0430  .4.4.5.@.6.8.2.0
-00011350: 0435 0442 0441 044f 003a 0020 0800 0000  .5.B.A.O.:. ....
-00011360: 0006 0000 0019 4f70 6572 6174 696f 6e20  ......Operation 
-00011370: 6e6f 7420 7375 7070 6f72 7465 643a 2007  not supported: .
-00011380: 0000 0013 5374 6174 656d 656e 744f 7065  ....StatementOpe
-00011390: 6e42 726f 6b65 7201 0300 0000 1c04 2604  nBroker.......&.
-000113a0: 1100 2004 3704 3004 3304 4004 4304 3604  .. .7.0.3.@.C.6.
-000113b0: 3504 3d04 4b00 3a00 2008 0000 0000 0600  5.=.K.:. .......
-000113c0: 0000 1353 6563 7572 6974 6965 7320 6c6f  ...Securities lo
-000113d0: 6164 6564 3a20 0700 0000 1353 7461 7465  aded: .....State
-000113e0: 6d65 6e74 4f70 656e 4272 6f6b 6572 0103  mentOpenBroker..
-000113f0: 0000 006e 041d 0435 043f 043e 0434 0434  ...n...5.?.>.4.4
-00011400: 0435 0440 0436 0438 0432 0430 0435 043c  .5.@.6.8.2.0.5.<
-00011410: 044b 0439 0020 0437 0430 0433 043e 043b  .K.9. .7.0.3.>.;
-00011420: 043e 0432 043e 043a 0020 043e 0442 0447  .>.2.>.:. .>.B.G
-00011430: 0451 0442 0430 0020 0434 043b 044f 0020  .Q.B.0. .4.;.O. 
-00011440: 041e 0442 043a 0440 044b 0442 0438 0435  ...B.:.@.K.B.8.5
-00011450: 0020 0431 0440 043e 043a 0435 0440 003a  . .1.@.>.:.5.@.:
-00011460: 0020 0800 0000 0006 0000 0026 556e 6578  . .........&Unex
-00011470: 7065 6374 6564 204f 7065 6e20 6272 6f6b  pected Open brok
-00011480: 6572 2072 6570 6f72 7420 6865 6164 6572  er report header
-00011490: 3a20 0700 0000 1353 7461 7465 6d65 6e74  : .....Statement
-000114a0: 4f70 656e 4272 6f6b 6572 0103 0000 0042  OpenBroker.....B
-000114b0: 041d 0435 0438 0437 0432 0435 0441 0442  ...5.8.7.2.5.A.B
-000114c0: 043d 0430 044f 0020 043d 0435 0442 043e  .=.0.O. .=.5.B.>
-000114d0: 0440 0433 043e 0432 0430 044f 0020 043e  .@.3.>.2.0.O. .>
-000114e0: 043f 0435 0440 0430 0446 0438 044f 003a  .?.5.@.0.F.8.O.:
-000114f0: 0020 0800 0000 0006 0000 001d 556e 6b6e  . ..........Unkn
-00011500: 6f77 6e20 6e6f 6e2d 7472 6164 6520 6f70  own non-trade op
-00011510: 6572 6174 696f 6e3a 2007 0000 0013 5374  eration: .....St
-00011520: 6174 656d 656e 744f 7065 6e42 726f 6b65  atementOpenBroke
-00011530: 7201 0300 0000 4604 1d04 3504 3f04 3e04  r.....F...5.?.>.
-00011540: 3404 3404 3504 4004 3604 3804 3204 3004  4.4.5.@.6.8.2.0.
-00011550: 3504 3c04 3e04 3500 2004 3e04 3f04 3804  5.<.>.5. .>.?.8.
-00011560: 4104 3004 3d04 3804 3500 2004 3f04 3b04  A.0.=.8.5. .?.;.
-00011570: 3004 4204 3504 3604 3000 3a00 2008 0000  0.B.5.6.0.:. ...
-00011580: 0000 0600 0000 1d55 6e6b 6e6f 776e 2070  .......Unknown p
-00011590: 6179 6d65 6e74 2064 6573 6372 6970 7469  ayment descripti
-000115a0: 6f6e 3a20 0700 0000 1353 7461 7465 6d65  on: .....Stateme
-000115b0: 6e74 4f70 656e 4272 6f6b 6572 0103 0000  ntOpenBroker....
-000115c0: 0032 041d 0435 0438 0437 0432 0435 0441  .2...5.8.7.2.5.A
-000115d0: 0442 043d 044b 0439 0020 0442 0438 043f  .B.=.K.9. .B.8.?
-000115e0: 0020 043f 043b 0430 0442 0435 0436 0430  . .?.;.0.B.5.6.0
-000115f0: 003a 0020 0800 0000 0006 0000 0016 556e  .:. ..........Un
-00011600: 6b6e 6f77 6e20 7061 796d 656e 7420 7479  known payment ty
-00011610: 7065 3a20 0700 0000 1353 7461 7465 6d65  pe: .....Stateme
-00011620: 6e74 4f70 656e 4272 6f6b 6572 0103 0000  ntOpenBroker....
-00011630: 0016 0426 0411 0020 0431 0435 0437 0020  ...&... .1.5.7. 
-00011640: 0069 0064 003a 0020 0800 0000 0006 0000  .i.d.:. ........
-00011650: 0012 4173 7365 7420 7769 7468 6f75 7420  ..Asset without 
-00011660: 6964 3a20 0700 0000 1653 7461 7465 6d65  id: .....Stateme
-00011670: 6e74 4f70 656e 506f 7274 666f 6c69 6f01  ntOpenPortfolio.
-00011680: 0300 0000 4804 1d04 3504 3204 3e04 3704  ....H...5.2.>.7.
-00011690: 3c04 3e04 3604 3d04 3e00 2004 3f04 4004  <.>.6.=.>. .?.@.
-000116a0: 3e04 4704 3804 4204 3004 4204 4c00 2000  >.G.8.B.0.B.L. .
-000116b0: 4a00 5300 4f00 4e00 2004 3804 3700 2004  J.S.O.N. .8.7. .
-000116c0: 4404 3004 3904 3b04 3000 3a00 2008 0000  D.0.9.;.0.:. ...
-000116d0: 0000 0600 0000 1f46 6169 6c65 6420 746f  .......Failed to
-000116e0: 2072 6561 6420 4a53 4f4e 2066 726f 6d20   read JSON from 
-000116f0: 6669 6c65 3a20 0700 0000 1653 7461 7465  file: .....State
-00011700: 6d65 6e74 4f70 656e 506f 7274 666f 6c69  mentOpenPortfoli
-00011710: 6f01 0300 0000 3404 1d04 3504 3204 3e04  o.....4...5.2.>.
-00011720: 3704 3c04 3e04 3604 3d04 3e00 2004 3f04  7.<.>.6.=.>. .?.
-00011730: 4004 3e04 4704 3504 4104 4204 4c00 2004  @.>.G.5.A.B.L. .
-00011740: 4404 3004 3904 3b00 3a00 2008 0000 0000  D.0.9.;.:. .....
-00011750: 0600 0000 1546 6169 6c65 6420 746f 2072  .....Failed to r
-00011760: 6561 6420 6669 6c65 3a20 0700 0000 1653  ead file: .....S
-00011770: 7461 7465 6d65 6e74 4f70 656e 506f 7274  tatementOpenPort
-00011780: 666f 6c69 6f01 0300 0000 2204 1804 3c04  folio....."...<.
-00011790: 3f04 3e04 4004 4204 3804 4004 3e04 3204  ?.>.@.B.8.@.>.2.
-000117a0: 3004 3d04 3d04 4b04 3900 2021 1608 0000  0.=.=.K.9. !....
-000117b0: 0000 0600 0000 0a49 6d70 6f72 7465 6420  .......Imported 
-000117c0: 2307 0000 0016 5374 6174 656d 656e 744f  #.....StatementO
-000117d0: 7065 6e50 6f72 7466 6f6c 696f 0103 0000  penPortfolio....
-000117e0: 002e 0049 006e 0076 0065 0073 0074 0062  ...I.n.v.e.s.t.b
-000117f0: 006f 006f 006b 0020 002f 0020 0049 005a  .o.o.k. ./. .I.Z
-00011800: 0049 002d 0069 006e 0076 0065 0073 0074  .I.-.i.n.v.e.s.t
-00011810: 0800 0000 0006 0000 0017 496e 7665 7374  ..........Invest
-00011820: 626f 6f6b 202f 2049 5a49 2d49 6e76 6573  book / IZI-Inves
-00011830: 7407 0000 0016 5374 6174 656d 656e 744f  t.....StatementO
-00011840: 7065 6e50 6f72 7466 6f6c 696f 0103 0000  penPortfolio....
-00011850: 0042 041e 0431 044f 0437 0430 0442 0435  .B...1.O.7.0.B.5
-00011860: 043b 044c 043d 0430 044f 0020 0441 0435  .;.L.=.0.O. .A.5
-00011870: 043a 0446 0438 044f 0020 043e 0442 0441  .:.F.8.O. .>.B.A
-00011880: 0443 0442 0441 0442 0432 0443 0435 0442  .C.B.A.B.2.C.5.B
-00011890: 003a 0020 0800 0000 0006 0000 001e 4d61  .:. ..........Ma
-000118a0: 6e64 6174 6f72 7920 7365 6374 696f 6e20  ndatory section 
-000118b0: 6973 206d 6973 7369 6e67 3a20 0700 0000  is missing: ....
-000118c0: 1653 7461 7465 6d65 6e74 4f70 656e 506f  .StatementOpenPo
-000118d0: 7274 666f 6c69 6f01 0300 0000 2e00 4f00  rtfolio.......O.
-000118e0: 7000 6500 6e00 2000 7000 6f00 7200 7400  p.e.n. .p.o.r.t.
-000118f0: 6600 6f00 6c00 6900 6f00 2000 2800 2a00  f.o.l.i.o. .(.*.
-00011900: 2e00 6a00 7300 6f00 6e00 2908 0000 0000  ..j.s.o.n.).....
-00011910: 0600 0000 174f 7065 6e20 706f 7274 666f  .....Open portfo
-00011920: 6c69 6f20 282a 2e6a 736f 6e29 0700 0000  lio (*.json)....
-00011930: 1653 7461 7465 6d65 6e74 4f70 656e 506f  .StatementOpenPo
-00011940: 7274 666f 6c69 6f01 0300 0000 4e04 1d04  rtfolio.....N...
-00011950: 3504 3f04 3e04 3404 3404 3504 4004 3604  5.?.>.4.4.5.@.6.
-00011960: 3804 3204 3004 3504 3c04 3004 4f00 2004  8.2.0.5.<.0.O. .
-00011970: 3204 3504 4004 4104 3804 4f00 2004 4404  2.5.@.A.8.O. .D.
-00011980: 3e04 4004 3c04 3004 4204 3000 2004 4404  >.@.<.0.B.0. .D.
-00011990: 3004 3904 3b04 3000 3a00 2008 0000 0000  0.9.;.0.:. .....
-000119a0: 0600 0000 2e55 6e73 7570 706f 7274 6564  .....Unsupported
-000119b0: 2076 6572 7369 6f6e 206f 6620 6f70 656e   version of open
-000119c0: 2070 6f72 7466 6f6c 696f 2066 6f72 6d61   portfolio forma
-000119d0: 743a 2007 0000 0016 5374 6174 656d 656e  t: .....Statemen
-000119e0: 744f 7065 6e50 6f72 7466 6f6c 696f 0103  tOpenPortfolio..
-000119f0: 0000 0038 041a 0443 043f 043e 043d 044b  ...8...C.?.>.=.K
-00011a00: 0020 043e 0431 043b 0438 0433 0430 0446  . .>.1.;.8.3.0.F
-00011a10: 0438 0439 0020 0437 0430 0433 0440 0443  .8.9. .7.0.3.@.C
-00011a20: 0436 0435 043d 044b 003a 0020 0800 0000  .6.5.=.K.:. ....
-00011a30: 0006 0000 0017 426f 6e64 2069 6e74 6572  ......Bond inter
-00011a40: 6573 7473 206c 6f61 6465 643a 2007 0000  ests loaded: ...
-00011a50: 000c 5374 6174 656d 656e 7450 5342 0103  ..StatementPSB..
-00011a60: 0000 003e 0414 0435 043d 0435 0436 043d  ...>...5.=.5.6.=
-00011a70: 044b 0435 0020 0442 0440 0430 043d 0437  .K.5. .B.@.0.=.7
-00011a80: 0430 043a 0446 0438 0438 0020 0437 0430  .0.:.F.8.8. .7.0
-00011a90: 0433 0440 0443 0436 0435 043d 044b 003a  .3.@.C.6.5.=.K.:
-00011aa0: 0020 0800 0000 0006 0000 001a 4361 7368  . ..........Cash
-00011ab0: 2074 7261 6e73 6163 7469 6f6e 7320 6c6f   transactions lo
-00011ac0: 6164 6564 3a20 0700 0000 0c53 7461 7465  aded: .....State
-00011ad0: 6d65 6e74 5053 4201 0300 0000 2a04 1404  mentPSB.....*...
-00011ae0: 3804 3204 3804 3404 3504 3d04 3404 4b00  8.2.8.4.5.=.4.K.
-00011af0: 2004 3704 3004 3304 4004 4304 3604 3504   .7.0.3.@.C.6.5.
-00011b00: 3d04 4b00 3a00 2008 0000 0000 0600 0000  =.K.:. .........
-00011b10: 1244 6976 6964 656e 6473 206c 6f61 6465  .Dividends loade
-00011b20: 643a 2007 0000 000c 5374 6174 656d 656e  d: .....Statemen
-00011b30: 7450 5342 0103 0000 0014 041f 0421 0411  tPSB.........!..
-00011b40: 002d 0431 0440 043e 043a 0435 0440 0800  .-.1.@.>.:.5.@..
-00011b50: 0000 0006 0000 000a 5053 4220 4272 6f6b  ........PSB Brok
-00011b60: 6572 0700 0000 0c53 7461 7465 6d65 6e74  er.....Statement
-00011b70: 5053 4201 0300 0000 4004 1e04 4204 4704  PSB.....@...B.G.
-00011b80: 5104 4200 2004 3104 4004 3e04 3a04 3504  Q.B. .1.@.>.:.5.
-00011b90: 4004 3000 2004 1f04 2104 1100 2000 2800  @.0. ...!... .(.
-00011ba0: 2a00 2e00 7800 6c00 7300 7800 2000 2a00  *...x.l.s.x. .*.
-00011bb0: 2e00 7800 6c00 7300 2908 0000 0000 0600  ..x.l.s.).......
-00011bc0: 0000 2350 5342 2062 726f 6b65 7220 7374  ..#PSB broker st
-00011bd0: 6174 656d 656e 7420 282a 2e78 6c73 7820  atement (*.xlsx 
-00011be0: 2a2e 786c 7329 0700 0000 0c53 7461 7465  *.xls).....State
-00011bf0: 6d65 6e74 5053 4201 03ff ffff ff08 0000  mentPSB.........
-00011c00: 0000 0600 0000 0f54 7261 6465 7320 6c6f  .......Trades lo
-00011c10: 6164 6564 3a20 0700 0000 0c53 7461 7465  aded: .....State
-00011c20: 6d65 6e74 5053 4201 0300 0000 4004 1d04  mentPSB.....@...
-00011c30: 3504 3f04 3e04 3404 3404 3504 4004 3604  5.?.>.4.4.5.@.6.
-00011c40: 3804 3204 3004 3504 3c04 3004 4f00 2004  8.2.0.5.<.0.O. .
-00011c50: 3e04 3f04 3504 4004 3004 4604 3804 4f00  >.?.5.@.0.F.8.O.
-00011c60: 2004 4100 2004 1404 2100 3a00 2008 0000   .A. ...!.:. ...
-00011c70: 0000 0600 0000 1855 6e6b 6e6f 776e 2063  .......Unknown c
-00011c80: 6173 6820 6f70 6572 6174 696f 6e3a 2007  ash operation: .
-00011c90: 0000 000c 5374 6174 656d 656e 7450 5342  ....StatementPSB
-00011ca0: 0103 0000 003a 041d 0435 0438 0437 0432  .....:...5.8.7.2
-00011cb0: 0435 0441 0442 043d 044b 0439 0020 0442  .5.A.B.=.K.9. .B
-00011cc0: 0438 043f 0020 0434 0432 0438 0436 0435  .8.?. .4.2.8.6.5
-00011cd0: 043d 0438 044f 0020 0414 0421 003a 0020  .=.8.O. ...!.:. 
-00011ce0: 0800 0000 0006 0000 001a 556e 6b6e 6f77  ..........Unknow
-00011cf0: 6e20 6361 7368 2074 7261 6e73 6163 7469  n cash transacti
-00011d00: 6f6e 3a20 0700 0000 0c53 7461 7465 6d65  on: .....Stateme
-00011d10: 6e74 5053 4201 0300 0000 3004 1d04 3504  ntPSB.....0...5.
-00011d20: 3804 3704 3204 3504 4104 4204 3d04 4b04  8.7.2.5.A.B.=.K.
-00011d30: 3900 2004 4204 3804 3f00 2004 4104 3404  9. .B.8.?. .A.4.
-00011d40: 3504 3b04 3a04 3800 3a00 2008 0000 0000  5.;.:.8.:. .....
-00011d50: 0600 0000 1455 6e6b 6e6f 776e 2074 7261  .....Unknown tra
-00011d60: 6465 2074 7970 653a 2007 0000 000c 5374  de type: .....St
-00011d70: 6174 656d 656e 7450 5342 0103 0000 0032  atementPSB.....2
-00011d80: 041d 0435 043f 043e 0434 0434 0435 0440  ...5.?.>.4.4.5.@
-00011d90: 0436 0438 0432 0430 0435 043c 044b 0439  .6.8.2.0.5.<.K.9
-00011da0: 0020 043f 043b 0430 0442 0451 0436 003a  . .?.;.0.B.Q.6.:
-00011db0: 0020 0800 0000 0006 0000 0015 556e 7375  . ..........Unsu
-00011dc0: 7070 6f72 7465 6420 7061 796d 656e 743a  pported payment:
-00011dd0: 2007 0000 000c 5374 6174 656d 656e 7450   .....StatementP
-00011de0: 5342 0103 0000 005a 0421 0434 0435 043b  SB.....Z.!.4.5.;
-00011df0: 043a 0430 0020 0441 0020 0440 0430 0437  .:.0. .A. .@.0.7
-00011e00: 043d 044b 043c 0438 0020 0432 0430 043b  .=.K.<.8. .2.0.;
-00011e10: 044e 0442 0430 043c 0438 0020 043d 0435  .N.B.0.<.8. .=.5
-00011e20: 0020 043f 043e 0434 0434 0435 0440 0436  . .?.>.4.4.5.@.6
-00011e30: 0438 0432 0430 0435 0442 0441 044f 003a  .8.2.0.5.B.A.O.:
-00011e40: 0020 0800 0000 0006 0000 002d 556e 7375  . .........-Unsu
-00011e50: 7070 6f72 7465 6420 7472 6164 6520 7769  pported trade wi
-00011e60: 7468 2064 6966 6665 7265 6e74 2063 7572  th different cur
-00011e70: 7265 6e63 6965 733a 2007 0000 000c 5374  rencies: .....St
-00011e80: 6174 656d 656e 7450 5342 0103 0000 0032  atementPSB.....2
-00011e90: 041e 043f 0435 0440 0430 0446 0438 0438  ...?.5.@.0.F.8.8
-00011ea0: 0020 0441 0020 0426 0411 0020 0437 0430  . .A. .&... .7.0
-00011eb0: 0433 0440 0443 0436 0435 043d 044b 003a  .3.@.C.6.5.=.K.:
-00011ec0: 0020 0800 0000 0006 0000 0019 4173 7365  . ..........Asse
-00011ed0: 7420 6f70 6572 6174 696f 6e73 206c 6f61  t operations loa
-00011ee0: 6465 643a 2007 0000 000d 5374 6174 656d  ded: .....Statem
-00011ef0: 656e 7455 4b46 5501 0300 0000 6804 1e04  entUKFU.....h...
-00011f00: 4204 4104 4304 4204 4104 4204 3204 4304  B.A.C.B.A.B.2.C.
-00011f10: 4e04 4200 2004 3e04 3604 3804 3404 3004  N.B. .>.6.8.4.0.
-00011f20: 3504 3c04 4b04 3500 2004 3404 3004 3d04  5.<.K.5. .4.0.=.
-00011f30: 3d04 4b04 3500 2004 3200 2004 3e04 3f04  =.K.5. .2. .>.?.
-00011f40: 3804 4104 3004 3d04 3804 3800 2004 3f04  8.A.0.=.8.8. .?.
-00011f50: 3504 4004 3504 3204 3e04 3404 3000 2004  5.@.5.2.>.4.0. .
-00011f60: 2604 1100 2008 0000 0000 0600 0000 2a41  &... .........*A
-00011f70: 7373 6574 2074 7261 6e73 6665 7220 6465  sset transfer de
-00011f80: 7363 7269 7074 696f 6e20 6d69 7373 2073  scription miss s
-00011f90: 6f6d 6520 6461 7461 2007 0000 000d 5374  ome data .....St
-00011fa0: 6174 656d 656e 7455 4b46 5501 0300 0000  atementUKFU.....
-00011fb0: 5004 1d04 3504 3204 3e04 3704 3c04 3e04  P...5.2.>.7.<.>.
-00011fc0: 3604 3d04 3e00 2004 3d04 3004 3904 4204  6.=.>. .=.0.9.B.
-00011fd0: 3800 2004 3704 3004 3f04 3804 4104 4c00  8. .7.0.?.8.A.L.
-00011fe0: 2004 4104 3f04 3804 4104 3004 3d04 3804   .A.?.8.A.0.=.8.
-00011ff0: 4f00 2004 2604 1100 2004 3404 3b04 4f00  O. .&... .4.;.O.
-00012000: 2008 0000 0000 0600 0000 2943 616e 2774   .........)Can't
-00012010: 2066 696e 6420 6173 7365 7420 6361 6e63   find asset canc
-00012020: 656c 6c61 7469 6f6e 2072 6563 6f72 6420  ellation record 
-00012030: 666f 7220 0700 0000 0d53 7461 7465 6d65  for .....Stateme
-00012040: 6e74 554b 4655 0103 0000 0046 041d 0435  ntUKFU.....F...5
-00012050: 0432 043e 0437 043c 043e 0436 043d 043e  .2.>.7.<.>.6.=.>
-00012060: 0020 043d 0430 0439 0442 0438 0020 0437  . .=.0.9.B.8. .7
-00012070: 0430 0433 043e 043b 043e 0432 043e 043a  .0.3.>.;.>.2.>.:
-00012080: 0020 043a 043e 043c 0438 0441 0441 0438  . .:.>.<.8.A.A.8
-00012090: 0439 0800 0000 0006 0000 001d 4361 6e27  .9..........Can'
-000120a0: 7420 6765 7420 6865 6164 6572 2074 6f20  t get header to 
-000120b0: 6669 6e64 2066 6565 7307 0000 000d 5374  find fees.....St
-000120c0: 6174 656d 656e 7455 4b46 5501 0300 0000  atementUKFU.....
-000120d0: 5604 1d04 3504 3204 3e04 3704 3c04 3e04  V...5.2.>.7.<.>.
-000120e0: 3604 3d04 3e00 2004 4004 3004 4104 3f04  6.=.>. .@.0.A.?.
-000120f0: 3e04 3704 3d04 3004 4204 4c00 2004 3e04  >.7.=.0.B.L. .>.
-00012100: 3f04 3804 4104 3004 3d04 3804 3500 2004  ?.8.A.0.=.8.5. .
-00012110: 3f04 3504 4004 3504 3204 3e04 3404 3000  ?.5.@.5.2.>.4.0.
-00012120: 2004 2604 1100 2008 0000 0000 0600 0000   .&... .........
-00012130: 2743 616e 2774 2070 6172 7365 2061 7373  'Can't parse ass
-00012140: 6574 2074 7261 6e73 6665 7220 6465 7363  et transfer desc
-00012150: 7269 7074 696f 6e20 0700 0000 0d53 7461  ription .....Sta
-00012160: 7465 6d65 6e74 554b 4655 0103 0000 004c  tementUKFU.....L
-00012170: 041d 0435 0432 043e 0437 043c 043e 0436  ...5.2.>.7.<.>.6
-00012180: 043d 043e 0020 0440 0430 0441 043f 043e  .=.>. .@.0.A.?.>
-00012190: 0437 043d 0430 0442 044c 0020 043e 043f  .7.=.0.B.L. .>.?
-000121a0: 0438 0441 0430 043d 0438 0435 0020 043a  .8.A.0.=.8.5. .:
-000121b0: 0443 043f 043e 043d 0430 0020 0800 0000  .C.?.>.=.0. ....
-000121c0: 0006 0000 0026 4361 6e27 7420 7061 7273  .....&Can't pars
-000121d0: 6520 626f 6e64 2069 6e74 6572 6573 7420  e bond interest 
-000121e0: 6465 7363 7269 7074 696f 6e20 0700 0000  description ....
-000121f0: 0d53 7461 7465 6d65 6e74 554b 4655 0103  .StatementUKFU..
-00012200: 0000 0066 041d 0435 0432 043e 0437 043c  ...f...5.2.>.7.<
-00012210: 043e 0436 043d 043e 0020 0440 0430 0441  .>.6.=.>. .@.0.A
-00012220: 043f 043e 0437 043d 0430 0442 044c 0020  .?.>.7.=.0.B.L. 
-00012230: 043e 043f 0438 0441 0430 043d 0438 0435  .>.?.8.A.0.=.8.5
-00012240: 0020 043f 043e 0433 0430 0448 0435 043d  . .?.>.3.0.H.5.=
-00012250: 0438 044f 0020 043e 0431 043b 0438 0433  .8.O. .>.1.;.8.3
-00012260: 0430 0446 0438 0438 0020 0800 0000 0006  .0.F.8.8. ......
-00012270: 0000 0027 4361 6e27 7420 7061 7273 6520  ...'Can't parse 
-00012280: 626f 6e64 2072 6570 6179 6d65 6e74 2064  bond repayment d
-00012290: 6573 6372 6970 7469 6f6e 2007 0000 000d  escription .....
-000122a0: 5374 6174 656d 656e 7455 4b46 5501 0300  StatementUKFU...
-000122b0: 0000 5204 1d04 3504 3204 3e04 3704 3c04  ..R...5.2.>.7.<.
-000122c0: 3e04 3604 3d04 3e00 2004 4004 3004 4104  >.6.=.>. .@.0.A.
-000122d0: 3f04 3e04 3704 3d04 3004 4204 4c00 2004  ?.>.7.=.0.B.L. .
-000122e0: 3e04 3f04 3804 4104 3004 3d04 3804 3500  >.?.8.A.0.=.8.5.
-000122f0: 2004 3404 3804 3204 3804 3404 3504 3d04   .4.8.2.8.4.5.=.
-00012300: 3404 3000 2008 0000 0000 0600 0000 2143  4.0. .........!C
-00012310: 616e 2774 2070 6172 7365 2064 6976 6964  an't parse divid
-00012320: 656e 6420 6465 7363 7269 7074 696f 6e20  end description 
-00012330: 0700 0000 0d53 7461 7465 6d65 6e74 554b  .....StatementUK
-00012340: 4655 0103 0000 0064 041d 0435 0432 043e  FU.....d...5.2.>
-00012350: 0437 043c 043e 0436 043d 043e 0020 0440  .7.<.>.6.=.>. .@
-00012360: 0430 0441 043f 043e 0437 043d 0430 0442  .0.A.?.>.7.=.0.B
-00012370: 044c 0020 043e 043f 0438 0441 0430 043d  .L. .>.?.8.A.0.=
-00012380: 0438 0435 0020 0434 0435 043d 0435 0436  .8.5. .4.5.=.5.6
-00012390: 043d 043e 0433 043e 0020 043f 0435 0440  .=.>.3.>. .?.5.@
-000123a0: 0435 0432 043e 0434 0430 0020 0800 0000  .5.2.>.4.0. ....
-000123b0: 0006 0000 0027 4361 6e27 7420 7061 7273  .....'Can't pars
-000123c0: 6520 6d6f 6e65 7920 7472 616e 7366 6572  e money transfer
-000123d0: 2064 6573 6372 6970 7469 6f6e 2007 0000   description ...
-000123e0: 000d 5374 6174 656d 656e 7455 4b46 5501  ..StatementUKFU.
-000123f0: 0300 0000 3a04 1404 3504 3d04 3504 3604  ....:...5.=.5.6.
-00012400: 3d04 4b04 4500 2004 3e04 3f04 3504 4004  =.K.E. .>.?.5.@.
-00012410: 3004 4604 3804 3900 2004 3704 3004 3304  0.F.8.9. .7.0.3.
-00012420: 4004 4304 3604 3504 3d04 3e00 3a00 2008  @.C.6.5.=.>.:. .
-00012430: 0000 0000 0600 0000 1843 6173 6820 6f70  .........Cash op
-00012440: 6572 6174 696f 6e73 206c 6f61 6465 643a  erations loaded:
-00012450: 2007 0000 000d 5374 6174 656d 656e 7455   .....StatementU
-00012460: 4b46 5501 0300 0000 4804 1e04 4804 3804  KFU.....H...H.8.
-00012470: 3104 3a04 3000 2004 3f04 4004 3800 2004  1.:.0. .?.@.8. .
-00012480: 3a04 3e04 3d04 3204 3504 4004 4204 3004  :.>.=.2.5.@.B.0.
-00012490: 4604 3804 3800 2004 4104 4304 3c04 3c04  F.8.8. .A.C.<.<.
-000124a0: 4b00 2004 3d04 3004 3b04 3e04 3304 3000  K. .=.0.;.>.3.0.
-000124b0: 2008 0000 0000 0600 0000 1f46 6169 6c65   ..........Faile
-000124c0: 6420 746f 2063 6f6e 7665 7274 2064 6976  d to convert div
-000124d0: 6964 656e 6420 7461 7820 0700 0000 0d53  idend tax .....S
-000124e0: 7461 7465 6d65 6e74 554b 4655 0103 0000  tatementUKFU....
-000124f0: 003e 0421 0434 0435 043b 043e 043a 0020  .>.!.4.5.;.>.:. 
-00012500: 0441 0020 0444 044c 044e 0447 0435 0440  .A. .D.L.N.G.5.@
-00012510: 0441 0430 043c 0438 0020 0437 0430 0433  .A.0.<.8. .7.0.3
-00012520: 0440 0443 0436 0435 043d 043e 003a 0020  .@.C.6.5.=.>.:. 
-00012530: 0800 0000 0006 0000 0017 4675 7475 7265  ..........Future
-00012540: 7320 7472 6164 6573 206c 6f61 6465 643a  s trades loaded:
-00012550: 2007 0000 000d 5374 6174 656d 656e 7455   .....StatementU
-00012560: 4b46 5501 0300 0000 7604 1e04 4204 4104  KFU.....v...B.A.
-00012570: 4304 4204 4104 4204 3204 4304 4e04 4200  C.B.A.B.2.C.N.B.
-00012580: 2004 3e04 3604 3804 3404 3004 3504 3c04   .>.6.8.4.0.5.<.
-00012590: 4b04 3500 2004 3404 3004 3d04 3d04 4b04  K.5. .4.0.=.=.K.
-000125a0: 3500 2004 3200 2004 3e04 3f04 3804 4104  5. .2. .>.?.8.A.
-000125b0: 3004 3d04 3804 3800 2004 3404 3504 3d04  0.=.8.8. .4.5.=.
-000125c0: 3504 3604 3d04 3e04 3304 3e00 2004 3f04  5.6.=.>.3.>. .?.
-000125d0: 3504 4004 3504 3204 3e04 3404 3000 2008  5.@.5.2.>.4.0. .
-000125e0: 0000 0000 0600 0000 2a4d 6f6e 6579 2074  ........*Money t
-000125f0: 7261 6e73 6665 7220 6465 7363 7269 7074  ransfer descript
-00012600: 696f 6e20 6d69 7373 2073 6f6d 6520 6461  ion miss some da
-00012610: 7461 2007 0000 000d 5374 6174 656d 656e  ta .....Statemen
-00012620: 7455 4b46 5501 0300 0000 5604 1d04 3004  tUKFU.....V...0.
-00012630: 3904 3404 3504 3d04 4b00 2004 3d04 3504  9.4.5.=.K. .=.5.
-00012640: 4104 3a04 3e04 3b04 4c04 3a04 3e00 2004  A.:.>.;.L.:.>. .
-00012650: 3704 3004 3f04 3804 4104 3504 3900 2004  7.0.?.8.A.5.9. .
-00012660: 3f04 3e04 3304 3004 4804 3504 3d04 3804  ?.>.3.0.H.5.=.8.
-00012670: 4f00 2004 2604 1100 2004 3404 3b04 4f00  O. .&... .4.;.O.
-00012680: 2008 0000 0000 0600 0000 264d 756c 7469   .........&Multi
-00012690: 706c 6520 6173 7365 7420 6361 6e63 656c  ple asset cancel
-000126a0: 6c61 7469 6f6e 206d 6174 6368 2066 6f72  lation match for
-000126b0: 2007 0000 000d 5374 6174 656d 656e 7455   .....StatementU
-000126c0: 4b46 5501 0300 0000 2404 2104 3404 3504  KFU.....$.!.4.5.
-000126d0: 3b04 3e04 3a00 2004 3704 3004 3304 4004  ;.>.:. .7.0.3.@.
-000126e0: 4304 3604 3504 3d04 3e00 3a00 2008 0000  C.6.5.=.>.:. ...
-000126f0: 0000 0600 0000 0f54 7261 6465 7320 6c6f  .......Trades lo
-00012700: 6164 6564 3a20 0700 0000 0d53 7461 7465  aded: .....State
-00012710: 6d65 6e74 554b 4655 0103 0000 0030 041d  mentUKFU.....0..
-00012720: 0435 0438 0437 0432 0435 0441 0442 043d  .5.8.7.2.5.A.B.=
-00012730: 044b 0439 0020 0442 0438 043f 0020 0441  .K.9. .B.8.?. .A
-00012740: 0434 0435 043b 043a 0438 003a 0020 0800  .4.5.;.:.8.:. ..
-00012750: 0000 0006 0000 0014 556e 6b6e 6f77 6e20  ........Unknown 
-00012760: 7472 6164 6520 7479 7065 3a20 0700 0000  trade type: ....
-00012770: 0d53 7461 7465 6d65 6e74 554b 4655 0103  .StatementUKFU..
-00012780: 0000 003e 041d 0435 043f 043e 0434 0434  ...>...5.?.>.4.4
-00012790: 0435 0440 0436 0438 0432 0430 0435 043c  .5.@.6.8.2.0.5.<
-000127a0: 0430 044f 0020 043e 043f 0435 0440 0430  .0.O. .>.?.5.@.0
-000127b0: 0446 0438 044f 0020 0441 0020 0426 0411  .F.8.O. .A. .&..
-000127c0: 0020 0800 0000 0006 0000 001d 556e 7375  . ..........Unsu
-000127d0: 7070 706f 7274 6564 2061 7373 6574 206f  ppported asset o
-000127e0: 7065 7261 7469 6f6e 2007 0000 000d 5374  peration .....St
-000127f0: 6174 656d 656e 7455 4b46 5501 0300 0000  atementUKFU.....
-00012800: 4a04 1d04 3504 3f04 3e04 3404 3404 3504  J...5.?.>.4.4.5.
-00012810: 4004 3604 3804 3204 3004 3504 3c04 3004  @.6.8.2.0.5.<.0.
-00012820: 4f00 2004 3404 3504 3d04 3504 3604 3d04  O. .4.5.=.5.6.=.
-00012830: 3004 4f00 2004 4204 4004 3004 3d04 3704  0.O. .B.@.0.=.7.
-00012840: 3004 3a04 4604 3804 4f00 2008 0000 0000  0.:.F.8.O. .....
-00012850: 0600 0000 1e55 6e73 7570 7070 6f72 7465  .....Unsuppporte
-00012860: 6420 6361 7368 2074 7261 6e73 6163 7469  d cash transacti
-00012870: 6f6e 2007 0000 000d 5374 6174 656d 656e  on .....Statemen
-00012880: 7455 4b46 5501 0300 0000 1e04 2304 4004  tUKFU.......#.@.
-00012890: 3004 3b04 4104 3804 3100 2004 1a04 4d04  0.;.A.8.1. ...M.
-000128a0: 3f04 3804 4204 3004 3b08 0000 0000 0600  ?.8.B.0.;.......
-000128b0: 0000 0e55 7261 6c73 6962 2042 726f 6b65  ...Uralsib Broke
-000128c0: 7207 0000 000d 5374 6174 656d 656e 7455  r.....StatementU
-000128d0: 4b46 5501 0300 0000 4a04 1e04 4204 4704  KFU.....J...B.G.
-000128e0: 5104 4200 2004 3104 4004 3e04 3a04 3504  Q.B. .1.@.>.:.5.
-000128f0: 4004 3000 2004 2304 4004 3004 3b04 4104  @.0. .#.@.0.;.A.
-00012900: 3804 3100 2004 1a04 4d04 3f04 3804 4204  8.1. ...M.?.8.B.
-00012910: 3004 3b00 2000 2800 2a00 2e00 7a00 6900  0.;. .(.*...z.i.
-00012920: 7000 2908 0000 0000 0600 0000 1955 7261  p.)..........Ura
-00012930: 6c73 6962 2073 7461 7465 6d65 6e74 2028  lsib statement (
-00012940: 2a2e 7a69 7029 0700 0000 0d53 7461 7465  *.zip).....State
-00012950: 6d65 6e74 554b 4655 0103 0000 003e 0410  mentUKFU.....>..
-00012960: 0440 0445 0438 0432 0020 0441 043e 0434  .@.E.8.2. .A.>.4
-00012970: 0435 0440 0436 0438 0442 0020 043d 0435  .5.@.6.8.B. .=.5
-00012980: 0441 043a 043e 043b 044c 043a 043e 0020  .A.:.>.;.L.:.>. 
-00012990: 0444 0430 0439 043b 043e 0432 0800 0000  .D.0.9.;.>.2....
-000129a0: 0006 0000 001f 4172 6368 6976 6520 636f  ......Archive co
-000129b0: 6e74 6169 6e73 206d 756c 7469 706c 6520  ntains multiple 
-000129c0: 6669 6c65 7307 0000 000c 5374 6174 656d  files.....Statem
-000129d0: 656e 7458 4c53 0103 0000 005a 041d 0435  entXLS.....Z...5
-000129e0: 0020 0443 0434 0430 043b 043e 0441 044c  . .C.4.0.;.>.A.L
-000129f0: 0020 043d 0430 0439 0442 0438 0020 043e  . .=.0.9.B.8. .>
-00012a00: 0436 0438 0434 0430 0435 043c 044b 0439  .6.8.4.0.5.<.K.9
-00012a10: 0020 0437 0430 0433 043e 043b 043e 0432  . .7.0.3.>.;.>.2
-00012a20: 043e 043a 0020 043e 0442 0447 0451 0442  .>.:. .>.B.G.Q.B
-00012a30: 0430 003a 0020 0800 0000 0006 0000 0023  .0.:. .........#
-00012a40: 4361 6e27 7420 6669 6e64 2065 7870 6563  Can't find expec
-00012a50: 7465 6420 7265 706f 7274 2068 6561 6465  ted report heade
-00012a60: 723a 2007 0000 000c 5374 6174 656d 656e  r: .....Statemen
-00012a70: 7458 4c53 0103 0000 0066 041d 0435 0020  tXLS.....f...5. 
-00012a80: 0443 0434 0430 043b 043e 0441 044c 0020  .C.4.0.;.>.A.L. 
-00012a90: 043e 043f 0440 0435 0434 0435 043b 0438  .>.?.@.5.4.5.;.8
-00012aa0: 0442 044c 0020 0432 0430 043b 044e 0442  .B.L. .2.0.;.N.B
-00012ab0: 044b 0020 0438 0437 0020 043e 0431 0449  .K. .8.7. .>.1.I
-00012ac0: 0435 0439 0020 0441 0435 043a 0446 0438  .5.9. .A.5.:.F.8
-00012ad0: 0438 0020 043e 0442 0447 0451 0442 0430  .8. .>.B.G.Q.B.0
-00012ae0: 0800 0000 0006 0000 0036 4361 6e27 7420  .........6Can't 
-00012af0: 6765 7420 6375 7272 656e 6369 6573 2066  get currencies f
-00012b00: 726f 6d20 7375 6d6d 6172 7920 7365 6374  rom summary sect
-00012b10: 696f 6e20 6f66 2073 7461 7465 6d65 6e74  ion of statement
-00012b20: 0700 0000 0c53 7461 7465 6d65 6e74 584c  .....StatementXL
-00012b30: 5301 0300 0000 4604 1d04 3504 3204 3e04  S.....F...5.2.>.
-00012b40: 3704 3c04 3e04 3604 3d04 3e00 2004 3e04  7.<.>.6.=.>. .>.
-00012b50: 3f04 4004 3504 3404 3504 3b04 3804 4204  ?.@.5.4.5.;.8.B.
-00012b60: 4c00 2004 3f04 3504 4004 3804 3e04 3400  L. .?.5.@.8.>.4.
-00012b70: 2004 3e04 4204 4704 5104 4204 3008 0000   .>.B.G.Q.B.0...
-00012b80: 0000 0600 0000 1843 616e 2774 2072 6561  .......Can't rea
-00012b90: 6420 7265 706f 7274 2070 6572 696f 6407  d report period.
-00012ba0: 0000 000c 5374 6174 656d 656e 7458 4c53  ....StatementXLS
-00012bb0: 0103 0000 001c 0414 0421 0020 0437 0430  .........!. .7.0
-00012bc0: 0433 0440 0443 0436 0435 043d 044b 003a  .3.@.C.6.5.=.K.:
-00012bd0: 0020 0800 0000 0006 0000 0016 4361 7368  . ..........Cash
-00012be0: 2062 616c 616e 6365 7320 6c6f 6164 6564   balances loaded
-00012bf0: 3a20 0700 0000 0c53 7461 7465 6d65 6e74  : .....Statement
-00012c00: 584c 5301 0300 0000 3604 2104 4204 3e04  XLS.....6.!.B.>.
-00012c10: 3b04 3104 3504 4600 2004 3d04 3500 2004  ;.1.5.F. .=.5. .
-00012c20: 3d04 3004 3904 3404 3504 3d00 2004 3200  =.0.9.4.5.=. .2.
-00012c30: 2004 4104 3504 3a04 4604 3804 3800 2008   .A.5.:.F.8.8. .
-00012c40: 0000 0000 0600 0000 1c43 6f6c 756d 6e20  .........Column 
-00012c50: 6e6f 7420 666f 756e 6420 696e 2073 6563  not found in sec
-00012c60: 7469 6f6e 2007 0000 000c 5374 6174 656d  tion .....Statem
-00012c70: 656e 7458 4c53 0103 0000 0034 041d 0435  entXLS.....4...5
-00012c80: 0441 043a 043e 043b 044c 043a 043e 0020  .A.:.>.;.L.:.>. 
-00012c90: 0441 0447 0435 0442 043e 0432 0020 043d  .A.G.5.B.>.2. .=
-00012ca0: 0430 0439 0434 0435 043d 043e 003a 0020  .0.9.4.5.=.>.:. 
-00012cb0: 0800 0000 0006 0000 0019 4d75 6c74 6970  ..........Multip
-00012cc0: 6c65 2061 6363 6f75 6e74 7320 666f 756e  le accounts foun
-00012cd0: 643a 2007 0000 000c 5374 6174 656d 656e  d: .....Statemen
-00012ce0: 7458 4c53 0103 0000 001c 0426 0411 0020  tXLS.......&... 
-00012cf0: 0437 0430 0433 0440 0443 0436 0435 043d  .7.0.3.@.C.6.5.=
-00012d00: 044b 003a 0020 0800 0000 0006 0000 0013  .K.:. ..........
-00012d10: 5365 6375 7269 7469 6573 206c 6f61 6465  Securities loade
-00012d20: 643a 2007 0000 000c 5374 6174 656d 656e  d: .....Statemen
-00012d30: 7458 4c53 0103 0000 0030 041e 0442 0447  tXLS.....0...B.G
-00012d40: 0451 0442 0020 0437 0430 0433 0440 0443  .Q.B. .7.0.3.@.C
-00012d50: 0436 0435 043d 0020 0443 0441 043f 0435  .6.5.=. .C.A.?.5
-00012d60: 0448 043d 043e 003a 0020 0800 0000 0006  .H.=.>.:. ......
-00012d70: 0000 001f 5374 6174 656d 656e 7420 6c6f  ....Statement lo
-00012d80: 6164 6564 2073 7563 6365 7373 6675 6c6c  aded successfull
-00012d90: 793a 2007 0000 000c 5374 6174 656d 656e  y: .....Statemen
-00012da0: 7458 4c53 0103 0000 0022 0020 0437 0430  tXLS.....". .7.0
-00012db0: 0433 0440 0443 0436 0435 043d 0020 0443  .3.@.C.6.5.=. .C
-00012dc0: 0441 043f 0435 0448 043d 043e 0800 0000  .A.?.5.H.=.>....
-00012dd0: 0006 0000 0014 206c 6f61 6465 6420 7375  ...... loaded su
-00012de0: 6363 6573 7366 756c 6c79 0700 0000 0c53  ccessfully.....S
-00012df0: 7461 7465 6d65 6e74 584d 4c01 0300 0000  tatementXML.....
-00012e00: 3604 1d04 3504 3204 3504 4004 3d04 4b04  6...5.2.5.@.=.K.
-00012e10: 3900 2004 4404 3e04 4004 3c04 3004 4200  9. .D.>.@.<.0.B.
-00012e20: 2000 5800 4d00 4c00 2004 4404 3004 3904   .X.M.L. .D.0.9.
-00012e30: 3b04 3000 3a00 2008 0000 0000 0600 0000  ;.0.:. .........
-00012e40: 1643 616e 2774 2070 6172 7365 2058 4d4c  .Can't parse XML
-00012e50: 2066 696c 653a 2007 0000 000c 5374 6174   file: .....Stat
-00012e60: 656d 656e 7458 4d4c 0103 0000 003e 041d  ementXML.....>..
-00012e70: 0435 0432 043e 0437 043c 043e 0436 043d  .5.2.>.7.<.>.6.=
-00012e80: 043e 0020 0437 0430 0433 0440 0443 0437  .>. .7.0.3.@.C.7
-00012e90: 0438 0442 044c 0020 0430 0442 0442 0440  .8.B.L. .0.B.B.@
-00012ea0: 0438 0431 0443 0442 003a 0020 0800 0000  .8.1.C.B.:. ....
-00012eb0: 0006 0000 001a 4661 696c 6564 2074 6f20  ......Failed to 
-00012ec0: 6c6f 6164 2061 7474 7269 6275 7465 3a20  load attribute: 
-00012ed0: 0700 0000 0c53 7461 7465 6d65 6e74 584d  .....StatementXM
-00012ee0: 4c01 0300 0000 4c04 1d04 3504 3f04 3e04  L.....L...5.?.>.
-00012ef0: 3404 3404 3504 4004 3604 3804 3204 3004  4.4.5.@.6.8.2.0.
-00012f00: 3504 3c04 4b04 3900 2004 4404 3e04 4004  5.<.K.9. .D.>.@.
-00012f10: 3c04 3004 4200 2004 3404 3004 4204 4b00  <.0.B. .4.0.B.K.
-00012f20: 2f04 3204 4004 3504 3c04 3504 3d04 3800  /.2.@.5.<.5.=.8.
-00012f30: 3a00 2008 0000 0000 0600 0000 1e55 6e73  :. ..........Uns
-00012f40: 7570 706f 7274 6564 2064 6174 652f 7469  upported date/ti
-00012f50: 6d65 2066 6f72 6d61 743a 2007 0000 000c  me format: .....
-00012f60: 5374 6174 656d 656e 7458 4d4c 0103 0000  StatementXML....
-00012f70: 0020 041e 0448 0438 0431 043a 0430 0020  . ...H.8.1.:.0. 
-00012f80: 0438 043c 043f 043e 0440 0442 0430 003a  .8.<.?.>.@.B.0.:
-00012f90: 0020 0800 0000 0006 0000 000f 496d 706f  . ..........Impo
-00012fa0: 7274 2066 6169 6c65 643a 2007 0000 000a  rt failed: .....
-00012fb0: 5374 6174 656d 656e 7473 0103 0000 0040  Statements.....@
-00012fc0: 0412 044b 0431 0435 0440 0438 0442 0435  ...K.1.5.@.8.B.5
-00012fd0: 0020 0444 0430 0439 043b 0020 043e 0442  . .D.0.9.;. .>.B
-00012fe0: 0447 0435 0442 0430 0020 0434 043b 044f  .G.5.B.0. .4.;.O
-00012ff0: 0020 0438 043c 043f 043e 0440 0442 0430  . .8.<.?.>.@.B.0
-00013000: 0800 0000 0006 0000 001f 5365 6c65 6374  ..........Select
-00013010: 2073 7461 7465 6d65 6e74 2066 696c 6520   statement file 
-00013020: 746f 2069 6d70 6f72 7407 0000 000a 5374  to import.....St
-00013030: 6174 656d 656e 7473 0103 0000 004a 041a  atements.....J..
-00013040: 043b 0430 0441 0441 0020 043e 0442 0447  .;.0.A.A. .>.B.G
-00013050: 0451 0442 0430 0020 043d 0435 0020 043c  .Q.B.0. .=.5. .<
-00013060: 043e 0436 0435 0442 0020 0431 044b 0442  .>.6.5.B. .1.K.B
-00013070: 044c 0020 0437 0430 0433 0440 0443 0436  .L. .7.0.3.@.C.6
-00013080: 0435 043d 003a 0020 0800 0000 0006 0000  .5.=.:. ........
-00013090: 0021 5374 6174 656d 656e 7420 636c 6173  .!Statement clas
-000130a0: 7320 6361 6e27 7420 6265 206c 6f61 6465  s can't be loade
-000130b0: 643a 2007 0000 000a 5374 6174 656d 656e  d: .....Statemen
-000130c0: 7473 0103 0000 0054 041c 043e 0434 0443  ts.....T...>.4.C
-000130d0: 043b 044c 0020 043e 0442 0447 0451 0442  .;.L. .>.B.G.Q.B
-000130e0: 0430 0020 043d 0435 0020 043c 043e 0436  .0. .=.5. .<.>.6
-000130f0: 0435 0442 0020 0431 044b 0442 044c 0020  .5.B. .1.K.B.L. 
-00013100: 0438 043c 043f 043e 0440 0442 0438 0440  .8.<.?.>.@.B.8.@
-00013110: 043e 0432 0430 043d 003a 0020 0800 0000  .>.2.0.=.:. ....
-00013120: 0006 0000 0024 5374 6174 656d 656e 7420  .....$Statement 
-00013130: 6d6f 6475 6c65 2063 616e 2774 2062 6520  module can't be 
-00013140: 696d 706f 7274 6564 3a20 0700 0000 0a53  imported: .....S
-00013150: 7461 7465 6d65 6e74 7301 0300 0000 0804  tatements.......
-00013160: 1004 3a04 4200 2e08 0000 0000 0600 0000  ..:.B...........
-00013170: 0441 6374 2e07 0000 0010 5379 6d62 6f6c  .Act......Symbol
-00013180: 734c 6973 744d 6f64 656c 0103 0000 000c  sListModel......
-00013190: 0412 0430 043b 044e 0442 0430 0800 0000  ...0.;.N.B.0....
-000131a0: 0006 0000 0008 4375 7272 656e 6379 0700  ......Currency..
-000131b0: 0000 1053 796d 626f 6c73 4c69 7374 4d6f  ...SymbolsListMo
-000131c0: 6465 6c01 0300 0000 1004 1e04 3f04 3804  del.........?.8.
-000131d0: 4104 3004 3d04 3804 3508 0000 0000 0600  A.0.=.8.5.......
-000131e0: 0000 0b44 6573 6372 6970 7469 6f6e 0700  ...Description..
-000131f0: 0000 1053 796d 626f 6c73 4c69 7374 4d6f  ...SymbolsListMo
-00013200: 6465 6c01 0300 0000 1204 1a04 3e04 4204  del.........>.B.
-00013210: 3804 4004 3e04 3204 3a04 3808 0000 0000  8.@.>.2.:.8.....
-00013220: 0600 0000 0651 756f 7465 7307 0000 0010  .....Quotes.....
-00013230: 5379 6d62 6f6c 734c 6973 744d 6f64 656c  SymbolsListModel
-00013240: 0103 0000 000c 0421 0438 043c 0432 043e  .......!.8.<.2.>
-00013250: 043b 0800 0000 0006 0000 0006 5379 6d62  .;..........Symb
-00013260: 6f6c 0700 0000 1053 796d 626f 6c73 4c69  ol.....SymbolsLi
-00013270: 7374 4d6f 6465 6c01 0300 0000 0604 2204  stModel.......".
-00013280: 4d04 3308 0000 0000 0600 0000 0354 6167  M.3..........Tag
-00013290: 0700 0000 0c54 6167 4c69 7374 4d6f 6465  .....TagListMode
-000132a0: 6c01 0300 0000 1004 1e04 3f04 3504 4004  l.........?.5.@.
-000132b0: 3004 4604 3804 3808 0000 0000 0600 0000  0.F.8.8.........
-000132c0: 0a4f 7065 7261 7469 6f6e 7307 0000 0009  .Operations.....
-000132d0: 5461 6752 6570 6f72 7401 0300 0000 1004  TagReport.......
-000132e0: 3f04 3e00 2004 1c04 3504 4204 3a04 3508  ?.>. ...5.B.:.5.
-000132f0: 0000 0000 0600 0000 0662 7920 5461 6707  .........by Tag.
-00013300: 0000 0009 5461 6752 6570 6f72 7401 0300  ....TagReport...
-00013310: 0000 1c04 1e04 4204 4704 3504 4200 2004  ......B.G.5.B. .
-00013320: 3f04 3e00 2004 3c04 3504 4204 3a04 3508  ?.>. .<.5.B.:.5.
-00013330: 0000 0000 0600 0000 0d52 6570 6f72 7420  .........Report 
-00013340: 6279 2074 6167 0700 0000 0f54 6167 5265  by tag.....TagRe
-00013350: 706f 7274 5769 6467 6574 0103 0000 000c  portWidget......
-00013360: 041c 0435 0442 043a 0430 003a 0800 0000  ...5.B.:.0.:....
-00013370: 0006 0000 0004 5461 673a 0700 0000 0f54  ......Tag:.....T
-00013380: 6167 5265 706f 7274 5769 6467 6574 0103  agReportWidget..
-00013390: 0000 0024 0027 0020 0437 0430 043c 0435  ...$.'. .7.0.<.5
-000133a0: 043d 0435 043d 0430 0020 0443 0441 043f  .=.5.=.0. .C.A.?
-000133b0: 0435 0448 043d 043e 0800 0000 0006 0000  .5.H.=.>........
-000133c0: 001b 2720 7761 7320 7375 6363 6573 7366  ..' was successf
-000133d0: 756c 6c79 2072 6570 6c61 6365 6407 0000  ully replaced...
-000133e0: 000e 5461 6773 4c69 7374 4469 616c 6f67  ..TagsListDialog
-000133f0: 0103 0000 000c 0027 0020 043d 0430 003a  .......'. .=.0.:
-00013400: 0020 0800 0000 0006 0000 0008 2720 7769  . ..........' wi
-00013410: 7468 3a20 0700 0000 0e54 6167 734c 6973  th: .....TagsLis
-00013420: 7444 6961 6c6f 6701 0300 0000 2004 1704  tDialog..... ...
-00013430: 3004 3c04 3504 3d04 3804 4204 4c00 2004  0.<.5.=.8.B.L. .
-00013440: 3c04 3504 4204 3a04 4300 2000 2708 0000  <.5.B.:.C. .'...
-00013450: 0000 0600 0000 0d52 6570 6c61 6365 2074  .......Replace t
-00013460: 6167 2027 0700 0000 0e54 6167 734c 6973  ag '.....TagsLis
-00013470: 7444 6961 6c6f 6701 0300 0000 1c04 1704  tDialog.........
-00013480: 3004 3c04 3504 3d04 3804 4204 4c00 2004  0.<.5.=.8.B.L. .
-00013490: 3d04 3000 2e00 2e00 2e08 0000 0000 0600  =.0.............
-000134a0: 0000 0f52 6570 6c61 6365 2077 6974 682e  ...Replace with.
-000134b0: 2e2e 0700 0000 0e54 6167 734c 6973 7444  .......TagsListD
-000134c0: 6961 6c6f 6701 0300 0000 3404 1f04 3e04  ialog.....4...>.
-000134d0: 3a04 3004 3704 3004 4204 4c00 2004 3e04  :.0.7.0.B.L. .>.
-000134e0: 3f04 3504 4004 3004 4604 3804 3800 2004  ?.5.@.0.F.8.8. .
-000134f0: 4100 2004 1c04 3504 4204 3a04 3e04 3908  A. ...5.B.:.>.9.
-00013500: 0000 0000 0600 0000 1853 686f 7720 6f70  .........Show op
-00013510: 6572 6174 696f 6e73 2077 6974 6820 5461  erations with Ta
-00013520: 6707 0000 000e 5461 6773 4c69 7374 4469  g.....TagsListDi
-00013530: 616c 6f67 0103 0000 000e 041c 0435 0442  alog.........5.B
-00013540: 043a 0430 0020 0027 0800 0000 0006 0000  .:.0. .'........
-00013550: 0005 5461 6720 2707 0000 000e 5461 6773  ..Tag '.....Tags
-00013560: 4c69 7374 4469 616c 6f67 0103 0000 0008  ListDialog......
-00013570: 0422 044d 0433 0438 0800 0000 0006 0000  .".M.3.8........
-00013580: 0004 5461 6773 0700 0000 0e54 6167 734c  ..Tags.....TagsL
-00013590: 6973 7444 6961 6c6f 6701 0300 0000 1a04  istDialog.......
-000135a0: 2204 3504 3a04 4304 4904 3804 3900 2004  ".5.:.C.I.8.9. .
-000135b0: 3a04 4304 4004 4100 3a08 0000 0000 0600  :.C.@.A.:.......
-000135c0: 0000 0d43 7572 7265 6e74 2072 6174 653a  ...Current rate:
-000135d0: 0700 0000 1354 6178 4573 7469 6d61 7469  .....TaxEstimati
-000135e0: 6f6e 4469 616c 6f67 0103 0000 0028 041f  onDialog.....(..
-000135f0: 043e 0441 043b 0435 0434 043d 044f 044f  .>.A.;.5.4.=.O.O
-00013600: 0020 043a 043e 0442 0438 0440 043e 0432  . .:.>.B.8.@.>.2
-00013610: 043a 0430 003a 0800 0000 0006 0000 000b  .:.0.:..........
-00013620: 4c61 7374 2071 756f 7465 3a07 0000 0013  Last quote:.....
-00013630: 5461 7845 7374 696d 6174 696f 6e44 6961  TaxEstimationDia
-00013640: 6c6f 6701 0300 0000 1a04 1e04 4604 3504  log.........F.5.
-00013650: 3d04 3a04 3000 2004 3d04 3004 3b04 3e04  =.:.0. .=.0.;.>.
-00013660: 3304 3008 0000 0000 0600 0000 0e54 6178  3.0..........Tax
-00013670: 2045 7374 696d 6174 696f 6e07 0000 0013   Estimation.....
-00013680: 5461 7845 7374 696d 6174 696f 6e44 6961  TaxEstimationDia
-00013690: 6c6f 6701 0300 0000 0800 5800 2e00 5800  log.......X...X.
-000136a0: 5808 0000 0000 0600 0000 0458 2e58 5807  X..........X.XX.
-000136b0: 0000 0013 5461 7845 7374 696d 6174 696f  ....TaxEstimatio
-000136c0: 6e44 6961 6c6f 6701 0300 0000 0a04 1804  nDialog.........
-000136d0: 2204 1e04 1304 1e08 0000 0000 0600 0000  "...............
-000136e0: 0554 4f54 414c 0700 0000 0c54 6178 4573  .TOTAL.....TaxEs
-000136f0: 7469 6d61 746f 7201 0300 0000 2404 1e04  timator.....$...
-00013700: 4604 3504 3d04 3a04 3000 2004 3d04 3004  F.5.=.:.0. .=.0.
-00013710: 3b04 3e04 3304 3000 2004 3404 3b04 4f00  ;.>.3.0. .4.;.O.
-00013720: 2008 0000 0000 0600 0000 1354 6178 2065   ..........Tax e
-00013730: 7374 696d 6174 696f 6e20 666f 7220 0700  stimation for ..
-00013740: 0000 0c54 6178 4573 7469 6d61 746f 7201  ...TaxEstimator.
-00013750: 0300 0000 3c04 2104 4204 3004 3204 3a04  ....<.!.B.0.2.:.
-00013760: 3000 2004 3d04 3004 3b04 3e04 3304 3000  0. .=.0.;.>.3.0.
-00013770: 2004 3d04 3500 2004 3d04 3004 3904 3404   .=.5. .=.0.9.4.
-00013780: 3504 3d04 3000 2004 3404 3b04 4f00 3a00  5.=.0. .4.;.O.:.
-00013790: 2008 0000 0000 0600 0000 1854 6178 2072   ..........Tax r
-000137a0: 6174 6520 6e6f 7420 666f 756e 6420 666f  ate not found fo
-000137b0: 723a 2007 0000 000c 5461 7845 7374 696d  r: .....TaxEstim
-000137c0: 6174 6f72 0103 0000 0008 0414 0430 0442  ator.........0.B
-000137d0: 0430 0800 0000 0006 0000 0004 4461 7465  .0..........Date
-000137e0: 0700 0000 1154 6178 4573 7469 6d61 746f  .....TaxEstimato
-000137f0: 724d 6f64 656c 0103 0000 0014 0426 0435  rModel.......&.5
-00013800: 043d 0430 0020 043e 0442 043a 0440 002e  .=.0. .>.B.:.@..
-00013810: 0800 0000 0006 0000 0004 4f70 656e 0700  ..........Open..
-00013820: 0000 1154 6178 4573 7469 6d61 746f 724d  ...TaxEstimatorM
-00013830: 6f64 656c 0103 0000 0012 041f 0440 0438  odel.........@.8
-00013840: 0431 044b 043b 044c 002c 0020 0800 0000  .1.K.;.L.,. ....
-00013850: 0006 0000 0008 5072 6f66 6974 2c20 0700  ......Profit, ..
-00013860: 0000 1154 6178 4573 7469 6d61 746f 724d  ...TaxEstimatorM
-00013870: 6f64 656c 0103 0000 000c 041a 043e 043b  odel.........>.;
-00013880: 002d 0432 043e 0800 0000 0006 0000 0003  .-.2.>..........
-00013890: 5174 7907 0000 0011 5461 7845 7374 696d  Qty.....TaxEstim
-000138a0: 6174 6f72 4d6f 6465 6c01 0300 0000 0c04  atorModel.......
-000138b0: 1a04 4304 4004 4100 2c00 2008 0000 0000  ..C.@.A.,. .....
-000138c0: 0600 0000 0652 6174 652c 2007 0000 0011  .....Rate, .....
-000138d0: 5461 7845 7374 696d 6174 6f72 4d6f 6465  TaxEstimatorMode
-000138e0: 6c01 0300 0000 0e04 1d04 3004 3b04 3e04  l.........0.;.>.
-000138f0: 3300 2c00 2008 0000 0000 0600 0000 0554  3.,. ..........T
-00013900: 6178 2c20 0700 0000 1154 6178 4573 7469  ax, .....TaxEsti
-00013910: 6d61 746f 724d 6f64 656c 0103 0000 0074  matorModel.....t
-00013920: 041d 0435 0432 043e 0437 043c 043e 0436  ...5.2.>.7.<.>.6
-00013930: 043d 043e 0020 0437 0430 0433 0440 0443  .=.>. .7.0.3.@.C
-00013940: 0437 0438 0442 044c 0020 043f 0430 0440  .7.8.B.L. .?.0.@
-00013950: 0430 043c 0435 0442 0440 044b 0020 043d  .0.<.5.B.@.K. .=
-00013960: 0430 043b 043e 0433 043e 0432 043e 0433  .0.;.>.3.>.2.>.3
-00013970: 043e 0020 043e 0442 0447 0451 0442 0430  .>. .>.B.G.Q.B.0
-00013980: 0020 0438 0437 0020 0444 0430 0439 043b  . .8.7. .D.0.9.;
-00013990: 0430 0020 0800 0000 0006 0000 002b 4361  .0. .........+Ca
-000139a0: 6e27 7420 6c6f 6164 2074 6178 2072 6570  n't load tax rep
-000139b0: 6f72 7420 7061 7261 6d65 7465 7273 2066  ort parameters f
-000139c0: 726f 6d20 6669 6c65 2007 0000 0009 5461  rom file .....Ta
-000139d0: 7852 6570 6f72 7401 0300 0000 2804 1d04  xReport.....(...
-000139e0: 3504 3804 3704 3204 3504 4104 4204 3d04  5.8.7.2.5.A.B.=.
-000139f0: 3004 4f00 2004 3204 3004 3b04 4e04 4204  0.O. .2.0.;.N.B.
-00013a00: 3000 3a00 2008 0000 0000 0600 0000 1943  0.:. ..........C
-00013a10: 7572 7265 6e63 7920 6973 206e 6f74 2064  urrency is not d
-00013a20: 6566 696e 6564 3a20 0700 0000 0954 6178  efined: .....Tax
-00013a30: 5265 706f 7274 0103 0000 004a 041d 0435  Report.....J...5
-00013a40: 0020 0443 043a 0430 0437 0430 043d 0020  . .C.:.0.7.0.=. 
-00013a50: 0448 0430 0431 043b 043e 043d 0020 043e  .H.0.1.;.>.=. .>
-00013a60: 0442 0447 0435 0442 0430 0020 0434 043b  .B.G.5.B.0. .4.;
-00013a70: 044f 0020 0440 0430 0437 0434 0435 043b  .O. .@.0.7.4.5.;
-00013a80: 0430 003a 0020 0800 0000 0006 0000 0026  .0.:. .........&
-00013a90: 4e6f 2072 6570 6f72 7420 7465 6d70 6c61  No report templa
-00013aa0: 7465 2066 6f75 6e64 2066 6f72 2073 6563  te found for sec
-00013ab0: 7469 6f6e 3a20 0700 0000 0954 6178 5265  tion: .....TaxRe
-00013ac0: 706f 7274 0103 0000 006a 041d 0435 0442  port.....j...5.B
-00013ad0: 0020 0438 043d 0444 043e 0440 043c 0430  . .8.=.D.>.@.<.0
-00013ae0: 0446 0438 0438 0020 043e 0020 0421 043e  .F.8.8. .>. .!.>
-00013af0: 0418 0414 041d 0020 0432 0020 043f 0430  ....... .2. .?.0
-00013b00: 0440 0430 043c 0435 0442 0440 0430 0445  .@.0.<.5.B.@.0.E
-00013b10: 0020 043d 0430 043b 043e 0433 043e 0432  . .=.0.;.>.3.>.2
-00013b20: 043e 0433 043e 0020 043e 0442 0447 0451  .>.3.>. .>.B.G.Q
-00013b30: 0442 0430 0800 0000 0006 0000 0042 5468  .B.0.........BTh
-00013b40: 6572 6520 6172 6520 6e6f 2069 6e66 6f72  ere are no infor
-00013b50: 6d61 7469 6f6e 2061 626f 7574 2074 6178  mation about tax
-00013b60: 2074 7265 6174 7920 696e 2074 6178 2072   treaty in tax r
-00013b70: 6570 6f72 7420 7061 7261 6d65 7465 7273  eport parameters
-00013b80: 0700 0000 0954 6178 5265 706f 7274 0103  .....TaxReport..
-00013b90: 0000 0060 041d 0435 0020 0437 0430 0434  ...`...5. .7.0.4
-00013ba0: 0430 043d 044b 0020 043f 0430 0440 0430  .0.=.K. .?.0.@.0
-00013bb0: 043c 0435 0442 0440 044b 0020 043d 0430  .<.5.B.@.K. .=.0
-00013bc0: 043b 043e 0433 043e 0432 043e 0433 043e  .;.>.3.>.2.>.3.>
-00013bd0: 0020 043e 0442 0447 0451 0442 0430 0020  . .>.B.G.Q.B.0. 
-00013be0: 0434 043b 044f 0020 0433 043e 0434 0430  .4.;.O. .3.>.4.0
-00013bf0: 003a 0020 0800 0000 0006 0000 0033 5468  .:. .........3Th
-00013c00: 6572 6520 6172 6520 6e6f 2070 6172 616d  ere are no param
-00013c10: 6574 6572 7320 666f 756e 6420 666f 7220  eters found for 
-00013c20: 7461 7820 7265 706f 7274 2079 6561 723a  tax report year:
-00013c30: 2007 0000 0009 5461 7852 6570 6f72 7401   .....TaxReport.
-00013c40: 0300 0000 0a00 2000 2e00 2e00 2e00 2008  ...... ....... .
-00013c50: 0000 0000 0600 0000 0520 2e2e 2e20 0700  ......... ... ..
-00013c60: 0000 0954 6178 5769 6467 6574 0103 0000  ...TaxWidget....
-00013c70: 0006 002e 002e 002e 0800 0000 0006 0000  ................
-00013c80: 0003 2e2e 2e07 0000 0009 5461 7857 6964  ..........TaxWid
-00013c90: 6765 7401 0300 0000 0a04 2104 4704 3504  get.......!.G.5.
-00013ca0: 4200 3a08 0000 0000 0600 0000 0841 6363  B.:..........Acc
-00013cb0: 6f75 6e74 3a07 0000 0009 5461 7857 6964  ount:.....TaxWid
-00013cc0: 6765 7401 0300 0000 9004 1d04 3804 3604  get.........8.6.
-00013cd0: 3500 2004 4004 3004 4104 3f04 3e04 3b04  5. .@.0.A.?.>.;.
-00013ce0: 3e04 3604 3504 3d04 4b00 2004 4d04 3a04  >.6.5.=.K. .M.:.
-00013cf0: 4104 3f04 3504 4004 3804 3c04 3504 3d04  A.?.5.@.8.<.5.=.
-00013d00: 4204 3004 3b04 4c04 3d04 4b04 3500 2004  B.0.;.L.=.K.5. .
-00013d10: 4404 4304 3d04 3a04 4604 3804 3800 2000  D.C.=.:.F.8.8. .
-00013d20: 2d00 2004 3804 4104 3f04 3e04 3b04 4c04  -. .8.A.?.>.;.L.
-00013d30: 3704 4304 3904 4204 3500 2004 4100 2004  7.C.9.B.5. .A. .
-00013d40: 3e04 4104 4204 3e04 4004 3e04 3604 3d04  >.A.B.>.@.>.6.=.
-00013d50: 3e04 4104 4204 4c04 4e08 0000 0000 0600  >.A.B.L.N.......
-00013d60: 0000 3342 656c 6f77 2066 756e 6374 696f  ..3Below functio
-00013d70: 6e73 2061 7265 2065 7870 6572 696d 656e  ns are experimen
-00013d80: 7461 6c20 2d20 7573 6520 6974 2077 6974  tal - use it wit
-00013d90: 6820 6361 7265 0700 0000 0954 6178 5769  h care.....TaxWi
-00013da0: 6467 6574 0103 0000 0044 041d 0435 0432  dget.....D...5.2
-00013db0: 043e 0437 043c 043e 0436 043d 043e 0020  .>.7.<.>.6.=.>. 
-00013dc0: 0437 0430 043f 0438 0441 0430 0442 044c  .7.0.?.8.A.0.B.L
-00013dd0: 0020 0033 002d 041d 0414 0424 041b 0020  . .3.-.....$... 
-00013de0: 0432 0020 0444 0430 0439 043b 0020 0800  .2. .D.0.9.;. ..
-00013df0: 0000 0006 0000 001f 4361 6e27 7420 7772  ........Can't wr
-00013e00: 6974 6520 7461 7820 666f 726d 2069 6e74  ite tax form int
-00013e10: 6f20 6669 6c65 2007 0000 0009 5461 7857  o file .....TaxW
-00013e20: 6964 6765 7401 0300 0000 0e04 2104 4204  idget.......!.B.
-00013e30: 4004 3004 3d04 3000 3a08 0000 0000 0600  @.0.=.0.:.......
-00013e40: 0000 0843 6f75 6e74 7279 3a07 0000 0009  ...Country:.....
-00013e50: 5461 7857 6964 6765 7401 0300 0000 7804  TaxWidget.....x.
-00013e60: 2104 3e04 3704 3404 3004 4204 4c00 2004  !.>.7.4.0.B.L. .
-00013e70: 4404 3004 3904 3b00 2000 3300 2d04 1d04  D.0.9.;. .3.-...
-00013e80: 2404 1404 1b00 2004 3200 2004 4404 3e04  $..... .2. .D.>.
-00013e90: 4004 3c04 3004 4204 3500 2004 3f04 4004  @.<.0.B.5. .?.@.
-00013ea0: 3e04 3304 4004 3004 3c04 3c04 4b00 2000  >.3.@.0.<.<.K. .
-00013eb0: 2204 1404 3504 3a04 3b04 3004 4004 3004  "...5.:.;.0.@.0.
-00013ec0: 4604 3804 4f00 2200 2000 2800 2a00 2e00  F.8.O.". .(.*...
-00013ed0: 6400 6300 5800 2908 0000 0000 0600 0000  d.c.X.).........
-00013ee0: 4043 7265 6174 6520 7461 7820 666f 726d  @Create tax form
-00013ef0: 2069 6e20 22d0 94d0 b5d0 bad0 bbd0 b0d1   in "...........
-00013f00: 80d0 b0d1 86d0 b8d1 8f22 2070 726f 6772  ........." progr
-00013f10: 616d 2066 6f72 6d61 7420 282a 2e64 6358  am format (*.dcX
-00013f20: 2907 0000 0009 5461 7857 6964 6765 7401  ).....TaxWidget.
-00013f30: 0300 0000 1e04 1404 3004 3d04 3d04 4b04  ........0.=.=.K.
-00013f40: 3500 2004 3d04 3504 3f04 3e04 3b04 3d04  5. .=.5.?.>.;.=.
-00013f50: 4b04 3508 0000 0000 0600 0000 1344 6174  K.5..........Dat
-00013f60: 6120 6172 6520 696e 636f 6d70 6c65 7465  a are incomplete
-00013f70: 0700 0000 0954 6178 5769 6467 6574 0103  .....TaxWidget..
-00013f80: 0000 005c 041d 0435 0020 0438 0441 043f  ...\...5. .8.A.?
-00013f90: 043e 043b 044c 0437 043e 0432 0430 0442  .>.;.L.7.>.2.0.B
-00013fa0: 044c 0020 0434 0430 0442 0443 0020 043f  .L. .4.0.B.C. .?
-00013fb0: 043e 0441 0442 0430 0432 043a 0438 0020  .>.A.B.0.2.:.8. 
-00013fc0: 0434 043b 044f 0020 043a 0443 0440 0441  .4.;.O. .:.C.@.A
-00013fd0: 043e 0432 0020 0432 0430 043b 044e 0442  .>.2. .2.0.;.N.B
-00013fe0: 0800 0000 0006 0000 002d 446f 206e 6f74  .........-Do not
-00013ff0: 2075 7365 2073 6574 746c 656d 656e 7420   use settlement 
-00014000: 6461 7465 2066 6f72 2063 7572 7265 6e63  date for currenc
-00014010: 7920 7261 7465 7307 0000 0009 5461 7857  y rates.....TaxW
-00014020: 6964 6765 7401 0300 0000 1604 2404 3004  idget.......$.0.
-00014030: 3904 3b00 2000 4500 7800 6300 6500 6c00  9.;. .E.x.c.e.l.
-00014040: 3a08 0000 0000 0600 0000 0b45 7863 656c  :..........Excel
-00014050: 2066 696c 653a 0700 0000 0954 6178 5769   file:.....TaxWi
-00014060: 6467 6574 0103 0000 0028 0424 0430 0439  dget.....(.$.0.9
-00014070: 043b 044b 0020 0045 0078 0063 0065 006c  .;.K. .E.x.c.e.l
-00014080: 0020 0028 002a 002e 0078 0073 006c 0078  . .(.*...x.s.l.x
-00014090: 0029 0800 0000 0006 0000 0014 4578 6365  .)..........Exce
-000140a0: 6c20 6669 6c65 7320 282a 2e78 6c73 7829  l files (*.xlsx)
-000140b0: 0700 0000 0954 6178 5769 6467 6574 0103  .....TaxWidget..
-000140c0: 0000 004a 0424 0430 0439 043b 0020 0434  ...J.$.0.9.;. .4
-000140d0: 043b 044f 0020 0441 043e 0445 0440 0430  .;.O. .A.>.E.@.0
-000140e0: 043d 0435 043d 0438 044f 0020 0434 0435  .=.5.=.8.O. .4.5
-000140f0: 043a 043b 0430 0440 0430 0446 0438 0438  .:.;.0.@.0.F.8.8
-00014100: 0020 0033 002d 041d 0414 0424 041b 0800  . .3.-.....$....
-00014110: 0000 0006 0000 0024 4669 6c65 2077 6865  .......$File whe
-00014120: 7265 2074 6f20 7374 6f72 6520 7275 7373  re to store russ
-00014130: 6961 6e20 7461 7820 666f 726d 0700 0000  ian tax form....
-00014140: 0954 6178 5769 6467 6574 0103 0000 0056  .TaxWidget.....V
-00014150: 0424 0430 0439 043b 0020 0434 043b 044f  .$.0.9.;. .4.;.O
-00014160: 0020 0441 043e 0445 0440 0430 043d 0435  . .A.>.E.@.0.=.5
-00014170: 043d 0438 044f 0020 0440 0430 0441 0447  .=.8.O. .@.0.A.G
-00014180: 0451 0442 0430 0020 0432 0020 0444 043e  .Q.B.0. .2. .D.>
-00014190: 0440 043c 0430 0442 0435 0020 0045 0078  .@.<.0.B.5. .E.x
-000141a0: 0063 0065 006c 0800 0000 0006 0000 002e  .c.e.l..........
-000141b0: 4669 6c65 2077 6865 7265 2074 6f20 7374  File where to st
-000141c0: 6f72 6520 7461 7820 7265 706f 7274 2069  ore tax report i
-000141d0: 6e20 4578 6365 6c20 666f 726d 6174 0700  n Excel format..
-000141e0: 0000 0954 6178 5769 6467 6574 0103 0000  ...TaxWidget....
-000141f0: 0068 0417 0430 0440 0443 0431 0435 0436  .h...0.@.C.1.5.6
-00014200: 043d 044b 0439 0020 0441 0447 0451 0442  .=.K.9. .A.G.Q.B
-00014210: 0020 0434 043b 044f 0020 043a 043e 0442  . .4.;.O. .:.>.B
-00014220: 043e 0440 043e 0433 043e 0020 043d 0443  .>.@.>.3.>. .=.C
-00014230: 0436 043d 043e 0020 043f 043e 0434 0433  .6.=.>. .?.>.4.3
-00014240: 043e 0442 043e 0432 0438 0442 044c 0020  .>.B.>.2.8.B.L. 
-00014250: 043e 0442 0447 0451 0442 0800 0000 0006  .>.B.G.Q.B......
-00014260: 0000 0029 466f 7265 6967 6e20 6163 636f  ...)Foreign acco
-00014270: 756e 7420 746f 2070 7265 7061 7265 2074  unt to prepare t
-00014280: 6178 2072 6570 6f72 7420 666f 7207 0000  ax report for...
-00014290: 0009 5461 7857 6964 6765 7401 0300 0000  ..TaxWidget.....
-000142a0: 2604 2404 3004 3904 3b00 2004 4100 2004  &.$.0.9.;. .A. .
-000142b0: 4004 3504 3704 4304 3b04 4c04 4204 3004  @.5.7.C.;.L.B.0.
-000142c0: 4204 3e04 3c00 3a08 0000 0000 0600 0000  B.>.<.:.........
-000142d0: 0c4f 7574 7075 7420 6669 6c65 3a07 0000  .Output file:...
-000142e0: 0009 5461 7857 6964 6765 7401 0300 0000  ..TaxWidget.....
-000142f0: 1e04 2104 3e04 4504 4004 3004 3d04 3804  ..!.>.E.@.0.=.8.
-00014300: 4204 4c00 2004 1e04 4204 4704 5104 4208  B.L. ...B.G.Q.B.
-00014310: 0000 0000 0600 0000 0b53 6176 6520 5265  .........Save Re
-00014320: 706f 7274 0700 0000 0954 6178 5769 6467  port.....TaxWidg
-00014330: 6574 0103 0000 0026 0421 043e 0445 0440  et.....&.!.>.E.@
-00014340: 0430 043d 0438 0442 044c 0020 0033 002d  .0.=.8.B.L. .3.-
-00014350: 041d 0414 0424 041b 0020 0432 003a 0800  .....$... .2.:..
-00014360: 0000 0006 0000 0011 5361 7665 2074 6178  ........Save tax
-00014370: 2066 6f72 6d20 746f 3a07 0000 0009 5461   form to:.....Ta
-00014380: 7857 6964 6765 7401 0300 0000 3804 2104  xWidget.....8.!.
-00014390: 3e04 4504 4004 3004 3d04 3804 4204 4c00  >.E.@.0.=.8.B.L.
-000143a0: 2004 3d04 3004 3b04 3e04 3304 3e04 3204   .=.0.;.>.3.>.2.
-000143b0: 4b04 3900 2004 3e04 4204 4704 5104 4200  K.9. .>.B.G.Q.B.
-000143c0: 2004 3200 3a08 0000 0000 0600 0000 1453   .2.:..........S
-000143d0: 6176 6520 7461 7820 7265 706f 7274 7320  ave tax reports 
-000143e0: 746f 3a07 0000 0009 5461 7857 6964 6765  to:.....TaxWidge
-000143f0: 7401 0300 0000 1804 1204 4b04 3104 3504  t.........K.1.5.
-00014400: 4004 3804 4200 2004 4404 3004 3904 3b08  @.8.B. .D.0.9.;.
-00014410: 0000 0000 0600 0000 0b53 656c 6563 7420  .........Select 
-00014420: 6669 6c65 0700 0000 0954 6178 5769 6467  file.....TaxWidg
-00014430: 6574 0103 0000 0028 041d 0430 043b 043e  et.....(...0.;.>
-00014440: 0433 043e 0432 044b 0439 0020 043e 0442  .3.>.2.K.9. .>.B
-00014450: 0447 0451 0442 0020 043f 0443 0441 0442  .G.Q.B. .?.C.A.B
-00014460: 0800 0000 0006 0000 0013 5461 7820 7265  ..........Tax re
-00014470: 706f 7274 2069 7320 656d 7074 7907 0000  port is empty...
-00014480: 0009 5461 7857 6964 6765 7401 0300 0000  ..TaxWidget.....
-00014490: 4004 1d04 3004 3b04 3e04 3304 3e04 3204  @...0.;.>.3.>.2.
-000144a0: 4b04 3900 2004 3e04 4204 4704 5104 4200  K.9. .>.B.G.Q.B.
-000144b0: 2004 4104 3e04 4504 4004 3004 3d04 5104   .A.>.E.@.0.=.Q.
-000144c0: 3d00 2004 3200 2004 4404 3004 3904 3b00  =. .2. .D.0.9.;.
-000144d0: 2008 0000 0000 0600 0000 1954 6178 2072   ..........Tax r
-000144e0: 6570 6f72 7420 7361 7665 6420 746f 2066  eport saved to f
-000144f0: 696c 6520 0700 0000 0954 6178 5769 6467  ile .....TaxWidg
-00014500: 6574 0103 0000 0040 041d 0430 043b 043e  et.....@...0.;.>
-00014510: 0433 043e 0432 044b 0439 0020 043e 0442  .3.>.2.K.9. .>.B
-00014520: 0447 0451 0442 0020 0441 043e 0445 0440  .G.Q.B. .A.>.E.@
-00014530: 0430 043d 0451 043d 0020 0432 0020 0444  .0.=.Q.=. .2. .D
-00014540: 0430 0439 043b 0020 0800 0000 0006 0000  .0.9.;. ........
-00014550: 001d 5461 7820 7265 706f 7274 2077 6173  ..Tax report was
-00014560: 2073 6176 6564 2074 6f20 6669 6c65 2007   saved to file .
-00014570: 0000 0009 5461 7857 6964 6765 7401 0300  ....TaxWidget...
-00014580: 0000 0c04 1d04 3004 3b04 3e04 3304 3808  ......0.;.>.3.8.
-00014590: 0000 0000 0600 0000 0554 6178 6573 0700  .........Taxes..
-000145a0: 0000 0954 6178 5769 6467 6574 0103 0000  ...TaxWidget....
-000145b0: 004e 041e 0431 043d 043e 0432 0438 0442  .N...1.=.>.2.8.B
-000145c0: 044c 0020 0442 043e 043b 044c 043a 043e  .L. .B.>.;.L.:.>
-000145d0: 0020 0438 043d 0444 043e 0440 043c 0430  . .8.=.D.>.@.<.0
-000145e0: 0446 0438 044e 0020 043e 0020 0434 0438  .F.8.N. .>. .4.8
-000145f0: 0432 0438 0434 0435 043d 0434 0430 0445  .2.8.4.5.=.4.0.E
-00014600: 0800 0000 0006 0000 0027 5570 6461 7465  .........'Update
-00014610: 206f 6e6c 7920 696e 666f 726d 6174 696f   only informatio
-00014620: 6e20 6162 6f75 7420 6469 7669 6465 6e64  n about dividend
-00014630: 7307 0000 0009 5461 7857 6964 6765 7401  s.....TaxWidget.
-00014640: 0300 0000 6404 1804 4104 3f04 3e04 3b04  ....d...A.?.>.;.
-00014650: 4c04 3704 3e04 3204 3004 4204 4c00 2004  L.7.>.2.0.B.L. .
-00014660: 3d04 3004 3704 3204 3004 3d04 3804 3500  =.0.7.2.0.=.8.5.
-00014670: 2004 3104 4004 3e04 3a04 3504 4004 3000   .1.@.>.:.5.@.0.
-00014680: 2004 3a04 3004 3a00 2004 3804 4104 4204   .:.0.:. .8.A.B.
-00014690: 3e04 4704 3d04 3804 3a00 2004 3204 4b04  >.G.=.8.:. .2.K.
-000146a0: 3f04 3b04 3004 4204 4b08 0000 0000 0600  ?.;.0.B.K.......
-000146b0: 0000 2055 7365 2062 726f 6b65 7220 6e61  .. Use broker na
-000146c0: 6d65 2061 7320 696e 636f 6d65 2073 6f75  me as income sou
-000146d0: 7263 6507 0000 0009 5461 7857 6964 6765  rce.....TaxWidge
-000146e0: 7401 0300 0000 0804 1304 3e04 3400 3a08  t.........>.4.:.
-000146f0: 0000 0000 0600 0000 0559 6561 723a 0700  .........Year:..
-00014700: 0000 0954 6178 5769 6467 6574 0103 0000  ...TaxWidget....
-00014710: 0050 0412 044b 0020 043d 0435 0020 0432  .P...K. .=.5. .2
-00014720: 044b 0431 0440 0430 043b 0438 0020 0441  .K.1.@.0.;.8. .A
-00014730: 0447 0451 0442 0020 0434 043b 044f 0020  .G.Q.B. .4.;.O. 
-00014740: 043d 0430 043b 043e 0433 043e 0432 043e  .=.0.;.>.3.>.2.>
-00014750: 0433 043e 0020 043e 0442 0447 0451 0442  .3.>. .>.B.G.Q.B
-00014760: 0430 0800 0000 0006 0000 002e 596f 7520  .0..........You 
-00014770: 6861 7665 6e27 7420 7365 6c65 6374 6564  haven't selected
-00014780: 2061 6e20 6163 636f 756e 7420 666f 7220   an account for 
-00014790: 7461 7820 7265 706f 7274 0700 0000 0954  tax report.....T
-000147a0: 6178 5769 6467 6574 0103 0000 0098 041d  axWidget........
-000147b0: 0435 0432 043e 0437 043c 043e 0436 043d  .5.2.>.7.<.>.6.=
-000147c0: 043e 0020 043e 0431 0440 0430 0431 043e  .>. .>.1.@.0.1.>
-000147d0: 0442 0430 0442 044c 0020 0441 0434 0435  .B.0.B.L. .A.4.5
-000147e0: 043b 043a 0443 002c 0020 0442 002e 043a  .;.:.C.,. .B...:
-000147f0: 002e 0020 043d 0435 0020 0437 0430 0434  ... .=.5. .7.0.4
-00014800: 0430 043d 0020 0431 0430 043d 043a 0020  .0.=. .1.0.=.:. 
-00014810: 0434 043b 044f 0020 0438 043d 0432 0435  .4.;.O. .8.=.2.5
-00014820: 0441 0442 0438 0446 0438 043e 043d 043d  .A.B.8.F.8.>.=.=
-00014830: 043e 0433 043e 0020 0441 0447 0451 0442  .>.3.>. .A.G.Q.B
-00014840: 0430 003a 0020 0800 0000 0006 0000 003e  .0.:. .........>
-00014850: 4361 6e27 7420 7072 6f63 6573 7320 7472  Can't process tr
-00014860: 6164 6520 6173 2062 616e 6b20 6973 6e27  ade as bank isn'
-00014870: 7420 7365 7420 666f 7220 696e 7665 7374  t set for invest
-00014880: 6d65 6e74 2061 6363 6f75 6e74 3a20 0700  ment account: ..
-00014890: 0000 0554 7261 6465 0103 0000 0002 2116  ...Trade......!.
-000148a0: 0800 0000 0006 0000 0001 2307 0000 000b  ..........#.....
-000148b0: 5472 6164 6557 6964 6765 7401 0300 0000  TradeWidget.....
-000148c0: 0804 2104 4704 3504 4208 0000 0000 0600  ..!.G.5.B.......
-000148d0: 0000 0741 6363 6f75 6e74 0700 0000 0b54  ...Account.....T
-000148e0: 7261 6465 5769 6467 6574 0103 0000 0004  radeWidget......
-000148f0: 0426 0411 0800 0000 0006 0000 0005 4173  .&............As
-00014900: 7365 7407 0000 000b 5472 6164 6557 6964  set.....TradeWid
-00014910: 6765 7401 0300 0000 2204 1f04 3e04 3a04  get....."...>.:.
-00014920: 4304 3f04 3a04 3000 2000 2f00 2004 1f04  C.?.:.0. ./. ...
-00014930: 4004 3e04 3404 3004 3604 3008 0000 0000  @.>.4.0.6.0.....
-00014940: 0600 0000 0a42 7579 202f 2053 656c 6c07  .....Buy / Sell.
-00014950: 0000 000b 5472 6164 6557 6964 6765 7401  ....TradeWidget.
-00014960: 0300 0000 1404 1404 3004 4204 3000 2f04  ........0.B.0./.
-00014970: 1204 4004 3504 3c04 4f08 0000 0000 0600  ..@.5.<.O.......
-00014980: 0000 0944 6174 652f 5469 6d65 0700 0000  ...Date/Time....
-00014990: 0b54 7261 6465 5769 6467 6574 0103 0000  .TradeWidget....
-000149a0: 0010 041a 043e 043c 0438 0441 0441 0438  .....>.<.8.A.A.8
-000149b0: 044f 0800 0000 0006 0000 0003 4665 6507  .O..........Fee.
-000149c0: 0000 000b 5472 6164 6557 6964 6765 7401  ....TradeWidget.
-000149d0: 0300 0000 1004 1e04 3f04 3804 4104 3004  ........?.8.A.0.
-000149e0: 3d04 3804 3508 0000 0000 0600 0000 044e  =.8.5..........N
-000149f0: 6f74 6507 0000 000b 5472 6164 6557 6964  ote.....TradeWid
-00014a00: 6765 7401 0300 0000 0804 2604 3504 3d04  get.......&.5.=.
-00014a10: 3008 0000 0000 0600 0000 0550 7269 6365  0..........Price
-00014a20: 0700 0000 0b54 7261 6465 5769 6467 6574  .....TradeWidget
-00014a30: 0103 0000 000c 041a 043e 043b 002d 0432  .........>.;.-.2
-00014a40: 043e 0800 0000 0006 0000 0003 5174 7907  .>..........Qty.
-00014a50: 0000 000b 5472 6164 6557 6964 6765 7401  ....TradeWidget.
-00014a60: 0300 0000 1a04 1404 3004 4204 3000 2004  ........0.B.0. .
-00014a70: 4004 3004 4104 4704 3504 4204 3e04 3208  @.0.A.G.5.B.>.2.
-00014a80: 0000 0000 0600 0000 0a53 6574 746c 656d  .........Settlem
-00014a90: 656e 7407 0000 000b 5472 6164 6557 6964  ent.....TradeWid
-00014aa0: 6765 7401 0300 0000 7a04 1a04 3e04 3b04  get.....z...>.;.
-00014ab0: 3804 4704 3504 4104 4204 3204 3e00 2004  8.G.5.A.B.2.>. .
-00014ac0: 3004 3a04 4204 3804 3204 3000 2004 3d04  0.:.B.8.2.0. .=.
-00014ad0: 3504 3404 3e04 4104 4204 3004 4204 3e04  5.4.>.A.B.0.B.>.
-00014ae0: 4704 3d04 3e00 2004 3404 3b04 4f00 2004  G.=.>. .4.;.O. .
-00014af0: 3e04 3104 4004 3004 3104 3e04 4204 3a04  >.1.@.0.1.>.B.:.
-00014b00: 3800 2004 3f04 3504 4004 3504 3204 3e04  8. .?.5.@.5.2.>.
-00014b10: 3404 3000 2e00 2004 1404 3004 4204 3000  4.0... ...0.B.0.
-00014b20: 3a00 2008 0000 0000 0600 0000 4041 7373  :. .........@Ass
-00014b30: 6574 2061 6d6f 756e 7420 6973 206e 6f74  et amount is not
-00014b40: 2065 6e6f 7567 6820 666f 7220 6173 7365   enough for asse
-00014b50: 7420 7472 616e 7366 6572 2070 726f 6365  t transfer proce
-00014b60: 7373 696e 672e 2044 6174 653a 2007 0000  ssing. Date: ...
-00014b70: 0008 5472 616e 7366 6572 0103 0000 0052  ..Transfer.....R
-00014b80: 0421 043f 0438 0441 0430 043d 0438 0435  .!.?.8.A.0.=.8.5
-00014b90: 0020 0430 043a 0442 0438 0432 0430 0020  . .0.:.B.8.2.0. 
-00014ba0: 043d 0435 0020 043d 0430 0439 0434 0435  .=.5. .=.0.9.4.5
-00014bb0: 043d 043e 0020 0434 043b 044f 0020 0442  .=.>. .4.;.O. .B
-00014bc0: 0440 0430 043d 0441 0444 0435 0440 0430  .@.0.=.A.D.5.@.0
-00014bd0: 002e 0800 0000 0006 0000 0028 4173 7365  ...........(Asse
-00014be0: 7420 7769 7468 6472 6177 616c 206e 6f74  t withdrawal not
-00014bf0: 2066 6f75 6e64 2066 6f72 2074 7261 6e73   found for trans
-00014c00: 6665 722e 0700 0000 0854 7261 6e73 6665  fer......Transfe
-00014c10: 7201 0300 0000 2e04 1e04 4804 3804 3104  r.........H.8.1.
-00014c20: 3a04 3000 2e00 2004 1a04 4304 4004 4100  :.0... ...C.@.A.
-00014c30: 2004 4004 3004 3204 3504 3d00 2004 3d04   .@.0.2.5.=. .=.
-00014c40: 4304 3b04 4e08 0000 0000 0600 0000 1045  C.;.N..........E
-00014c50: 7272 6f72 2e20 5a65 726f 2072 6174 6507  rror. Zero rate.
-00014c60: 0000 0008 5472 616e 7366 6572 0103 0000  ....Transfer....
-00014c70: 0084 041e 0431 0440 0430 0431 043e 0442  .....1.@.0.1.>.B
-00014c80: 0430 043d 043d 043e 0435 0020 043a 043e  .0.=.=.>.5. .:.>
-00014c90: 043b 0438 0447 0435 0441 0442 0432 043e  .;.8.G.5.A.B.2.>
-00014ca0: 0020 043c 0435 043d 044c 0448 0435 002c  . .<.5.=.L.H.5.,
-00014cb0: 0020 0447 0435 043c 0020 043a 043e 043b  . .G.5.<. .:.>.;
-00014cc0: 0438 0447 0435 0441 0442 0432 043e 0020  .8.G.5.A.B.2.>. 
-00014cd0: 0432 0020 0442 0440 0430 043d 0441 0444  .2. .B.@.0.=.A.D
-00014ce0: 0435 0440 0435 002e 0020 0414 0430 0442  .5.@.5... ...0.B
-00014cf0: 0430 003a 0020 0800 0000 0006 0000 003b  .0.:. .........;
-00014d00: 5072 6f63 6573 7365 6420 6173 7365 7420  Processed asset 
-00014d10: 616d 6f75 6e74 2069 7320 6c65 7373 2074  amount is less t
-00014d20: 6861 6e20 7472 616e 7366 6572 2061 6d6f  han transfer amo
-00014d30: 756e 742e 2044 6174 653a 2007 0000 0008  unt. Date: .....
-00014d40: 5472 616e 7366 6572 0103 0000 0002 2116  Transfer......!.
-00014d50: 0800 0000 0006 0000 0001 2307 0000 000e  ..........#.....
-00014d60: 5472 616e 7366 6572 5769 6467 6574 0103  TransferWidget..
-00014d70: 0000 000a 0421 0443 043c 043c 0430 0800  .....!.C.<.<.0..
-00014d80: 0000 0006 0000 0006 416d 6f75 6e74 0700  ........Amount..
-00014d90: 0000 0e54 7261 6e73 6665 7257 6964 6765  ...TransferWidge
-00014da0: 7401 0300 0000 0404 2604 1108 0000 0000  t.......&.......
-00014db0: 0600 0000 0541 7373 6574 0700 0000 0e54  .....Asset.....T
-00014dc0: 7261 6e73 6665 7257 6964 6765 7401 0300  ransferWidget...
-00014dd0: 0000 1404 1404 3004 4204 3000 2f04 1204  ......0.B.0./...
-00014de0: 4004 3504 3c04 4f08 0000 0000 0600 0000  @.5.<.O.........
-00014df0: 0944 6174 652f 5469 6d65 0700 0000 0e54  .Date/Time.....T
-00014e00: 7261 6e73 6665 7257 6964 6765 7401 0300  ransferWidget...
-00014e10: 0000 1e04 2004 3004 3704 3c04 3504 4000  .... .0.7.<.5.@.
-00014e20: 2004 3a04 3e04 3c04 3804 4104 4104 3804   .:.>.<.8.A.A.8.
-00014e30: 3808 0000 0000 0600 0000 0a46 6565 2061  8..........Fee a
-00014e40: 6d6f 756e 7407 0000 000e 5472 616e 7366  mount.....Transf
-00014e50: 6572 5769 6467 6574 0103 0000 0016 041a  erWidget........
-00014e60: 043e 043c 043c 0438 0441 0441 0438 044f  .>.<.<.8.A.A.8.O
-00014e70: 0020 0441 0800 0000 0006 0000 0008 4665  . .A..........Fe
-00014e80: 6520 6672 6f6d 0700 0000 0e54 7261 6e73  e from.....Trans
-00014e90: 6665 7257 6964 6765 7401 0300 0000 0204  ferWidget.......
-00014ea0: 2108 0000 0000 0600 0000 0446 726f 6d07  !..........From.
-00014eb0: 0000 000e 5472 616e 7366 6572 5769 6467  ....TransferWidg
-00014ec0: 6574 0103 0000 0010 041e 043f 0438 0441  et.........?.8.A
-00014ed0: 0430 043d 0438 0435 0800 0000 0006 0000  .0.=.8.5........
-00014ee0: 0004 4e6f 7465 0700 0000 0e54 7261 6e73  ..Note.....Trans
-00014ef0: 6665 7257 6964 6765 7401 0300 0000 0404  ferWidget.......
-00014f00: 1d04 3008 0000 0000 0600 0000 0254 6f07  ..0..........To.
-00014f10: 0000 000e 5472 616e 7366 6572 5769 6467  ....TransferWidg
-00014f20: 6574 0103 0000 000e 041f 0435 0440 0435  et.........5.@.5
-00014f30: 0432 043e 0434 0800 0000 0006 0000 0008  .2.>.4..........
-00014f40: 5472 616e 7366 6572 0700 0000 0e54 7261  Transfer.....Tra
-00014f50: 6e73 6665 7257 6964 6765 7401 0300 0000  nsferWidget.....
-00014f60: 0404 1f04 3e08 0000 0000 0600 0000 0845  ....>..........E
-00014f70: 6e64 2064 6174 6507 0000 000f 5570 6461  nd date.....Upda
-00014f80: 7465 5175 6f74 6573 446c 6701 0300 0000  teQuotesDlg.....
-00014f90: 1204 1804 4104 4204 3e04 4704 3d04 3804  ....A.B.>.G.=.8.
-00014fa0: 3a04 3808 0000 0000 0600 0000 0753 6f75  :.8..........Sou
-00014fb0: 7263 6573 0700 0000 0f55 7064 6174 6551  rces.....UpdateQ
-00014fc0: 756f 7465 7344 6c67 0103 0000 0002 0421  uotesDlg.......!
-00014fd0: 0800 0000 0006 0000 000a 5374 6172 7420  ..........Start 
-00014fe0: 6461 7465 0700 0000 0f55 7064 6174 6551  date.....UpdateQ
-00014ff0: 756f 7465 7344 6c67 0103 0000 0028 041e  uotesDlg.....(..
-00015000: 0431 043d 043e 0432 043b 0435 043d 0438  .1.=.>.2.;.5.=.8
-00015010: 0435 0020 043a 043e 0442 0438 0440 043e  .5. .:.>.B.8.@.>
-00015020: 0432 043e 043a 0800 0000 0006 0000 0015  .2.>.:..........
-00015030: 5570 6461 7465 2061 7373 6574 2773 2071  Update asset's q
-00015040: 756f 7465 7307 0000 000f 5570 6461 7465  uotes.....Update
-00015050: 5175 6f74 6573 446c 6701 0300 0000 1400  QuotesDlg.......
-00015060: 6400 6400 2f00 4d00 4d00 2f00 7900 7900  d.d./.M.M./.y.y.
-00015070: 7900 7908 0000 0000 0600 0000 0a64 642f  y.y..........dd/
-00015080: 4d4d 2f79 7979 7907 0000 000f 5570 6461  MM/yyyy.....Upda
-00015090: 7465 5175 6f74 6573 446c 6701 0300 0000  teQuotesDlg.....
-000150a0: 5804 1d04 3504 3204 3e04 3704 3c04 3e04  X...5.2.>.7.<.>.
-000150b0: 3604 3d04 3e00 2004 3f04 4004 3e04 4704  6.=.>. .?.@.>.G.
-000150c0: 3804 4204 3004 4204 4c00 2004 4804 3004  8.B.0.B.L. .H.0.
-000150d0: 3104 3b04 3e04 3d00 2004 3e04 4204 4704  1.;.>.=. .>.B.G.
-000150e0: 5104 4204 3000 2004 3804 3700 2004 4404  Q.B.0. .8.7. .D.
-000150f0: 3004 3904 3b04 3000 2008 0000 0000 0600  0.9.;.0. .......
-00015100: 0000 2543 616e 2774 206c 6f61 6420 7265  ..%Can't load re
-00015110: 706f 7274 2074 656d 706c 6174 6520 6672  port template fr
-00015120: 6f6d 2066 696c 6520 0700 0000 0458 4c53  om file .....XLS
-00015130: 5801 0300 0000 4404 1d04 3504 3204 3e04  X.....D...5.2.>.
-00015140: 3704 3c04 3e04 3604 3d04 3e00 2004 4104  7.<.>.6.=.>. .A.
-00015150: 3e04 4504 4004 3004 3d04 3804 4204 4c00  >.E.@.0.=.8.B.L.
-00015160: 2004 3e04 4204 4704 5104 4200 2004 3200   .>.B.G.Q.B. .2.
-00015170: 2004 4404 3004 3904 3b00 2008 0000 0000   .D.0.9.;. .....
-00015180: 0600 0000 1c43 616e 2774 2073 6176 6520  .....Can't save 
-00015190: 7265 706f 7274 2069 6e74 6f20 6669 6c65  report into file
-000151a0: 2007 0000 0004 584c 5358 0103 0000 0044   .....XLSX.....D
-000151b0: 041d 0435 0020 0443 043a 0430 0437 0430  ...5. .C.:.0.7.0
-000151c0: 043d 0020 0444 043e 0440 043c 0430 0442  .=. .D.>.@.<.0.B
-000151d0: 0020 0434 043b 044f 0020 043f 043e 043b  . .4.;.O. .?.>.;
-000151e0: 044f 0020 043e 0442 0447 0451 0442 0430  .O. .>.B.G.Q.B.0
-000151f0: 003a 0020 0800 0000 0006 0000 0024 466f  .:. .........$Fo
-00015200: 726d 6174 2069 7320 6d69 7373 696e 6720  rmat is missing 
-00015210: 666f 7220 7265 706f 7274 2066 6965 6c64  for report field
-00015220: 3a20 0700 0000 0458 4c53 5801 0300 0000  : .....XLSX.....
-00015230: 4204 1d04 3500 2004 3704 3004 3404 3004  B...5. .7.0.4.0.
-00015240: 3d00 2004 4804 3004 3104 3b04 3e04 3d00  =. .H.0.1.;.>.=.
-00015250: 2004 3404 3b04 4f00 2004 3404 3004 3d04   .4.;.O. .4.0.=.
-00015260: 3d04 4b04 4500 2004 3e04 4204 4704 5104  =.K.E. .>.B.G.Q.
-00015270: 4204 3008 0000 0000 0600 0000 1a4e 6f20  B.0..........No 
-00015280: 7265 706f 7274 2072 6f77 2074 656d 706c  report row templ
-00015290: 6174 6520 7365 7407 0000 0004 584c 5358  ate set.....XLSX
-000152a0: 0103 0000 003a 0428 0430 0431 043b 043e  .....:.(.0.1.;.>
-000152b0: 043d 0020 0434 043b 044f 0020 0434 0430  .=. .4.;.O. .4.0
-000152c0: 043d 043d 044b 0445 0020 043d 0435 0020  .=.=.K.E. .=.5. 
-000152d0: 043d 0430 0439 0434 0435 043d 003a 0020  .=.0.9.4.5.=.:. 
-000152e0: 0800 0000 0006 0000 001f 5265 706f 7274  ..........Report
-000152f0: 2072 6f77 2074 656d 706c 6174 6520 6e6f   row template no
-00015300: 7420 666f 756e 643a 2007 0000 0004 584c  t found: .....XL
-00015310: 5358 0103 0000 0046 041d 0435 0438 0437  SX.....F...5.8.7
-00015320: 0432 0435 0441 0442 043d 0430 044f 0020  .2.5.A.B.=.0.O. 
-00015330: 0441 0442 0440 043e 043a 0430 0020 0444  .A.B.@.>.:.0. .D
-00015340: 043e 0440 043c 0430 0442 0438 0440 043e  .>.@.<.0.B.8.@.>
-00015350: 0432 0430 043d 0438 044f 003a 0020 0800  .2.0.=.8.O.:. ..
-00015360: 0000 0006 0000 001c 556e 7265 636f 676e  ........Unrecogn
-00015370: 697a 6564 2066 6f72 6d61 7420 7374 7269  ized format stri
-00015380: 6e67 3a20 0700 0000 0458 4c53 5801 8800  ng: .....XLSX...
-00015390: 0000 0d11 01fd 290b ff14 0204 fd2c 0a13  ......)......,..
+00000010: a700 0000 0572 755f 5255 4200 001a 0000  .....ru_RUB.....
+00000020: 0000 2300 001c 2500 0000 2300 0030 1300  ..#...%...#..0..
+00000030: 0000 2300 0130 e500 0000 2300 0135 9500  ..#..0....#..5..
+00000040: 0000 2500 0092 9a00 0004 7300 0005 b700  ..%.......s.....
+00000050: 0005 3b00 0009 4c00 0005 af00 0137 4600  ..;...L......7F.
+00000060: 0031 0e00 007e 3e00 0031 0e00 0124 b900  .1...~>..1...$..
+00000070: 0046 3900 0003 7000 0046 3900 00a3 0500  .F9...p..F9.....
+00000080: 0047 a400 0045 bf00 0048 7200 004e 5200  .G...E...Hr..NR.
+00000090: 0048 7200 0092 c100 0048 b700 004e 8900  .Hr......H...N..
+000000a0: 0048 b700 0093 1c00 004a 7a00 0047 bd00  .H.......Jz..G..
+000000b0: 004a b300 004e c000 004a b300 0093 ca00  .J...N...J......
+000000c0: 004b 1a00 0047 e800 004b 3a00 0048 1300  .K...G...K:..H..
+000000d0: 004c b200 004e f700 004c b200 0094 3600  .L...N...L....6.
+000000e0: 004c b500 0013 bf00 004c b500 0131 e900  .L.......L...1..
+000000f0: 0050 7e00 004f 2e00 0050 7e00 0094 df00  .P~..O...P~.....
+00000100: 0051 3100 001e df00 0051 3100 0031 8400  .Q1......Q1..1..
+00000110: 0051 bc00 004f 6500 0051 bc00 0095 0c00  .Q...Oe..Q......
+00000120: 0051 be00 004f 9c00 0051 be00 0095 3900  .Q...O...Q....9.
+00000130: 0052 ac00 0096 4700 0052 ac00 0098 a000  .R....G..R......
+00000140: 0053 3c00 0015 2300 0053 3c00 0036 c900  .S<...#..S<..6..
+00000150: 0053 8200 004f d300 0053 8200 0095 6600  .S...O...S....f.
+00000160: 0053 8900 0050 0a00 0053 8900 0095 9300  .S...P...S......
+00000170: 0055 6600 0050 4100 0055 6600 0095 ed00  .Uf..PA..Uf.....
+00000180: 0055 a400 0050 7800 0055 a400 0096 1a00  .U...Px..U......
+00000190: 0058 b900 0015 8a00 0058 b900 0020 5e00  .X.......X... ^.
+000001a0: 0058 b900 0037 2800 0058 b900 00aa 1700  .X...7(..X......
+000001b0: 0058 b900 0120 c100 0058 b900 0132 7d00  .X... ...X...2}.
+000001c0: 0059 c000 0050 af00 0059 c000 0097 3e00  .Y...P...Y....>.
+000001d0: 005a 7700 002b cf00 005a 7700 0089 dd00  .Zw..+...Zw.....
+000001e0: 005a 7700 011a c400 005a 8800 0032 f900  .Zw......Z...2..
+000001f0: 005b 2a00 0027 6b00 0070 7c00 005d cd00  .[*..'k..p|..]..
+00000200: 047a 6e00 0005 4000 047a 6e00 0119 a600  .zn...@..zn.....
+00000210: 0498 9800 008f 2800 04a6 7900 0085 6400  ......(...y...d.
+00000220: 04a8 a500 000e 0500 04a8 a500 00a0 2600  ..............&.
+00000230: 04a8 a500 0120 1100 04a8 d300 0091 9900  ..... ..........
+00000240: 04cb c300 0094 6300 04cf 3a00 0035 be00  ......c...:..5..
+00000250: 04d9 5d00 0136 e600 04e3 1a00 0075 b200  ..]..6.......u..
+00000260: 04e7 de00 000b 0d00 04e7 de00 000c 7500  ..............u.
+00000270: 0504 cf00 0078 e500 0528 a400 0035 ee00  .....x...(...5..
+00000280: 0548 3500 0006 1b00 0548 3500 000b 3c00  .H5......H5...<.
+00000290: 0548 3500 0011 c100 0548 3500 008e 5e00  .H5......H5...^.
+000002a0: 0556 a500 0013 f800 0556 a500 001f 1200  .V.......V......
+000002b0: 0556 a500 002b 9a00 0556 a500 0031 f500  .V...+...V...1..
+000002c0: 0556 a500 0055 3700 0556 a500 0132 1c00  .V...U7..V...2..
+000002d0: 0556 a500 0137 0f00 0565 c000 0043 cc00  .V...7...e...C..
+000002e0: 0566 be00 0036 8f00 0566 be00 0120 4300  .f...6...f... C.
+000002f0: 056b c200 0056 e600 05a3 0000 004b d700  .k...V.......K..
+00000300: 05a7 aa00 011b a700 05a7 e300 011d b700  ................
+00000310: 05b3 d800 011e e000 05c0 6500 0021 a300  ..........e..!..
+00000320: 05c0 6500 0033 2900 05db bb00 0027 9a00  ..e..3)......'..
+00000330: 05fb 8200 0027 d000 1530 3000 0012 3a00  .....'...00...:.
+00000340: 18d1 5000 00ee b100 2311 0000 0124 8c00  ..P.....#....$..
+00000350: 26f2 9100 004c 0300 2aa8 a100 0058 9500  &....L..*....X..
+00000360: 2acf 0400 0058 cb00 2b37 fe00 0059 7100  *....X..+7...Yq.
+00000370: 2b76 1e00 0086 3300 2ba7 e300 005b 7500  +v....3.+....[u.
+00000380: 2ec7 e000 0045 5e00 3153 c400 0094 9b00  .....E^.1S......
+00000390: 3d1a 0e00 005d 2800 4182 8900 00ff b000  =....](.A.......
+000003a0: 4796 c400 0078 6600 47af 8000 009c 3500  G....xf.G.....5.
+000003b0: 48a9 c400 0006 db00 48a9 c400 0012 8a00  H.......H.......
+000003c0: 48a9 c400 001c da00 48a9 c400 0029 9400  H.......H....)..
+000003d0: 48a9 c400 0030 6b00 48a9 c400 009f c100  H....0k.H.......
+000003e0: 48a9 c400 00a9 e700 48a9 c400 0131 3700  H.......H....17.
+000003f0: 48a9 c400 0135 ee00 4964 b300 0090 9500  H....5..Id......
+00000400: 4988 b300 008e ee00 4a2b 8200 0046 c700  I.......J+...F..
+00000410: 4a36 9500 002a 4300 4a36 9500 0046 fe00  J6...*C.J6...F..
+00000420: 4a36 9500 0074 be00 4a71 ec00 0025 3100  J6...t..Jq...%1.
+00000430: 4ab8 3300 0028 d400 4b6b 9000 0104 5300  J.3..(..Kk....S.
+00000440: 4d68 c800 0091 c900 4d96 0a00 0025 df00  Mh......M....%..
+00000450: 4dc4 b300 0091 fe00 4e7e 1a00 0008 de00  M.......N~......
+00000460: 522b 5a00 0074 f400 52e9 5500 0014 d900  R+Z..t..R.U.....
+00000470: 5308 d400 0096 aa00 535d fe00 0075 e100  S.......S]...u..
+00000480: 5464 c900 0092 3100 5464 c900 0095 c000  Td....1.Td......
+00000490: 5465 a800 0026 0e00 5483 8a00 0009 0d00  Te...&..T.......
+000004a0: 556a c300 0083 8200 55da be00 0012 0300  Uj......U.......
+000004b0: 56bc 5a00 004a 9200 56bc 5a00 008d 4d00  V.Z..J..V.Z...M.
+000004c0: 56bc 9300 008b 6d00 578f 9500 0032 2c00  V.....m.W....2,.
+000004d0: 578f 9500 0132 5000 57a1 7200 0027 2600  W....2P.W.r..'&.
+000004e0: 5839 2400 006b 2d00 58c6 a500 00a0 5600  X9$..k-.X.....V.
+000004f0: 5948 5c00 0050 e600 5948 5c00 011f 1400  YH\..P..YH\.....
+00000500: 5a73 0400 001a 4a00 5a73 0400 0021 1900  Zs....J.Zs...!..
+00000510: 5a79 2700 011d 8100 5a8a e000 0121 2e00  Zy'.....Z....!..
+00000520: 5a8b c000 002f 6e00 5a8e c300 0097 6b00  Z..../n.Z.....k.
+00000530: 5a8e c300 012d ca00 5b6a 7c00 000d 4600  Z....-..[j|...F.
+00000540: 5b6a 7c00 0097 a000 5c06 8a00 004c 8d00  [j|.....\....L..
+00000550: 5c83 b500 0034 ec00 5c83 b500 0037 9100  \....4..\....7..
+00000560: 5fb8 5a00 0081 5800 5fb8 5a00 012f 2e00  _.Z...X._.Z../..
+00000570: 602e 0a00 0056 8400 67f7 0000 00f8 0000  `....V..g.......
+00000580: 70c5 c000 00c8 8700 80a8 e500 0049 ce00  p............I..
+00000590: 81bc 0000 00ce 7000 918d 3700 003c 4000  ......p...7..<@.
+000005a0: 931f 2000 00d9 df00 9472 3000 0070 6600  .. ......r0..pf.
+000005b0: 9688 5400 00d4 c200 ab81 4000 0117 b900  ..T.......@.....
+000005c0: af00 f000 00b6 4600 af26 4500 0125 1000  ......F..&E..%..
+000005d0: b27d 9f00 0079 7b00 b4d0 c500 0029 d900  .}...y{......)..
+000005e0: b643 0000 00c3 0c00 c9db ba00 0063 2a00  .C...........c*.
+000005f0: cfb0 f400 0031 1100 e1f3 f000 0017 8d00  .....1..........
+00000600: e25b 3000 002c f900 ed2c 2500 0028 0000  .[0..,...,%..(..
+00000610: fbe4 b100 0048 3e00 ff6b fe00 00b3 8401  .....H>..k......
+00000620: 11c0 6000 0139 7e01 1c4b f000 0115 4101  ..`..9~..K....A.
+00000630: 2273 8300 008e 9c01 24a2 9700 003c f701  "s......$....<..
+00000640: 2bca d000 009e aa01 3502 c000 00c4 db01  +.......5.......
+00000650: 473b 2300 0071 5701 5567 7000 00cd c901  G;#..qW.Ugp.....
+00000660: 59b4 9000 001b 0d01 6654 9000 003b 3701  Y.......fT...;7.
+00000670: 7248 d000 0036 2801 776d e000 00d5 e201  rH...6(.wm......
+00000680: 78c3 f500 0031 b001 7e51 ea00 012b 7f01  x....1..~Q...+..
+00000690: 873b 2300 0071 8901 887c d300 005d f901  .;#..q...|...]..
+000006a0: 9687 c000 010b 3c01 98a7 5300 004c bc01  ......<...S..L..
+000006b0: a469 f900 0102 4c01 a885 4000 0134 b901  .i....L...@..4..
+000006c0: aff7 3300 0000 0001 bef6 7000 00d2 e001  ..3.......p.....
+000006d0: c26a 9a00 00a3 3a01 ce0a 1200 008c 5601  .j....:.......V.
+000006e0: d48e 5000 0043 2801 da69 b000 0114 d401  ..P..C(..i......
+000006f0: e128 5000 00c0 1201 e26a 9a00 0004 2801  .(P......j....(.
+00000700: f571 7000 00bd 2102 00dd 0100 0044 6a02  .qp...!......Dj.
+00000710: 01b8 4900 003a 8d02 01b8 4900 0088 9202  ..I..:....I.....
+00000720: 01b8 4900 00a2 c502 01b8 4900 0138 a602  ..I.......I..8..
+00000730: 24d1 2000 00df 9702 2b24 6500 012e 8c02  $. .....+$e.....
+00000740: 36c0 e700 006d 7302 38ab b000 00b0 1502  6....ms.8.......
+00000750: 488e 8300 0127 cb02 5442 2f00 0022 3d02  H....'..TB/.."=.
+00000760: 6b41 b400 012f 5902 705b 1000 0060 7702  kA.../Y.p[...`w.
+00000770: 75ac 0500 00d8 2f02 76e6 2500 0043 fd02  u...../.v.%..C..
+00000780: 80f4 7400 005b ed02 83cb 1900 00ad 1702  ..t..[..........
+00000790: 84df 6000 000d 0b02 86cb d700 00ae a402  ..`.............
+000007a0: 960b 0000 0103 7902 9d24 b400 00bf af02  ......y..$......
+000007b0: a013 f300 00d4 6702 b6bc 9300 0059 eb02  ......g......Y..
+000007c0: b827 6100 00a5 0002 c4de 6000 00c9 1502  .'a.......`.....
+000007d0: d6b9 7000 00e0 7202 d6b9 7000 00ec 5e02  ..p...r...p...^.
+000007e0: d6b9 7000 0102 d002 d6b9 7000 010d 9c02  ..p.......p.....
+000007f0: da2f f000 00bb 4b02 db87 a000 00f2 f102  ./....K.........
+00000800: ddd8 9000 0018 c702 e4ef 0400 0020 9702  ............. ..
+00000810: e60b 0000 0077 e902 ecb9 d000 006e 6f03  .....w.......no.
+00000820: 0055 4a00 012a e803 0ae6 8700 0018 3203  .UJ..*........2.
+00000830: 0ae6 8700 001d ba03 0b8a 5a00 007a f603  ..........Z..z..
+00000840: 1108 9c00 0131 6003 1638 c400 0096 f203  .....1`..8......
+00000850: 1684 be00 001d 0d03 2221 4000 00af 8c03  ........"!@.....
+00000860: 232f f000 00f4 3803 232f f000 0108 d703  #/....8.#/......
+00000870: 3500 5a00 0088 4603 3f3c 8400 0111 4d03  5.Z...F.?<....M.
+00000880: 55cb 1a00 0076 4d03 57fa 2e00 0075 3b03  U....vM.W....u;.
+00000890: 5dae f000 0109 8603 5dce f000 00e4 0b03  ].......].......
+000008a0: 6b8b d900 0126 a603 7321 8300 0110 3103  k....&..s!....1.
+000008b0: 82a1 0000 00e0 a303 8a06 2000 0100 2003  .......... ... .
+000008c0: 8b39 a000 0104 bb03 8b60 e400 003f b803  .9.......`...?..
+000008d0: 8c34 6500 0026 cd03 8f4e c000 0114 0d03  .4e..&...N......
+000008e0: 9100 d000 005f 7f03 97c9 0000 0122 8303  ....._......."..
+000008f0: b023 a000 00b9 fc03 cafd 4000 0083 bb03  .#........@.....
+00000900: d07e 2400 0069 4f03 d1c2 7400 0041 9203  .~$..iO...t..A..
+00000910: d1e5 2200 0005 7103 da9c f300 005b a703  .."...q......[..
+00000920: ec0c f700 003d bd03 f69b 8000 00c7 3504  .....=........5.
+00000930: 0029 e000 0125 f104 09f4 0a00 00bc ad04  .)...%..........
+00000940: 11d2 4900 000d 7704 11d2 a900 0058 0404  ..I...w......X..
+00000950: 1263 4400 00b5 f804 1564 8e00 0029 5a04  .cD......d...)Z.
+00000960: 15b4 7000 0139 f704 195c b000 0119 0f04  ..p..9...\......
+00000970: 2e61 f000 0073 7104 449a c000 012c d804  .a...sq.D....,..
+00000980: 56c0 a000 00b7 d004 62c1 c000 00ff 2504  V.......b.....%.
+00000990: 66ac 6500 0137 a804 7914 8000 00d1 7b04  f.e..7..y.....{.
+000009a0: 7d16 7000 006f 4b04 846c 5400 002b 2e04  }.p..oK..lT..+..
+000009b0: 846c 5400 0082 df04 846c 5400 0089 1604  .lT......lT.....
+000009c0: 846c 5400 0135 bb04 8a9c b300 000a 1404  .lT..5..........
+000009d0: 8a9c b300 0092 ee04 8c2d c700 0065 9504  .........-...e..
+000009e0: 8c2d c700 007c 7404 8e23 4000 0000 c004  .-...|t..#@.....
+000009f0: 8e23 4000 001f e304 8e23 4000 0056 0a04  .#@......#@..V..
+00000a00: 983c 8100 0046 9304 9849 bc00 0008 3504  .<...F...I....5.
+00000a10: 9e16 8200 0102 0d04 9e84 d500 0093 4904  ..............I.
+00000a20: a577 1f00 0067 7c04 a5e2 3000 0099 b404  .w...g|...0.....
+00000a30: ac2c a500 0085 fa04 ac2c a500 00a4 c404  .,.......,......
+00000a40: bebd 0000 00a8 3f04 c840 f000 00e9 dc04  ......?..@......
+00000a50: c840 f000 00ed 1704 c840 f000 010e d404  .@.......@......
+00000a60: cc5c 9400 0028 4e04 cf4d c200 00f8 8704  .\...(N..M......
+00000a70: d5c8 0000 0007 1a04 d7d5 4000 00cb ca04  ..........@.....
+00000a80: dd34 9000 0015 bf04 ee54 4000 010c 3c04  .4.......T@...<.
+00000a90: f6d3 c900 00d4 0005 04e3 1000 0007 9505  ................
+00000aa0: 079c 7300 0123 1105 161e a000 00b5 8305  ..s..#..........
+00000ab0: 2caa 5000 00b3 e105 2cde 2300 00a5 5805  ,.P.....,.#...X.
+00000ac0: 304c 6a00 0049 9805 33ee 2500 0015 5205  0Lj..I..3.%...R.
+00000ad0: 33ee 2500 0036 f405 3c8d c200 0018 7105  3.%..6..<.....q.
+00000ae0: 3c8d c200 001e 8705 3d7b 7000 00e9 7705  <.......={p...w.
+00000af0: 3d7b 7000 00ec b205 3d7b 7000 0103 ee05  ={p.....={p.....
+00000b00: 3d7b 7000 010d f105 49ee 8900 0068 b505  ={p.....I....h..
+00000b10: 4e5b d400 0118 0705 5305 de00 0076 9b05  N[......S....v..
+00000b20: 5316 ce00 0075 7a05 633f 7000 00e5 6505  S....uz.c?p...e.
+00000b30: 6945 5000 00c5 e905 6bc4 2700 008b 2c05  iEP.....k.'...,.
+00000b40: 6bcd a500 00b1 ac05 6c90 5400 0096 7405  k.......l.T...t.
+00000b50: 6ccc 4300 004b 7205 6edf f400 008d e805  l.C..Kr.n.......
+00000b60: 6fe5 c000 00f3 a305 802f 5e00 00b0 e005  o......../^.....
+00000b70: 812d 6000 0101 b005 88a7 e000 0120 f605  .-`.......... ..
+00000b80: 88a8 c000 004d c705 8c6a c300 009f 8405  .....M...j......
+00000b90: 8c6a c300 011a 5005 8cbc 8e00 004b 3c05  .j....P......K<.
+00000ba0: 98ab 6e00 008e 2a05 9ca9 f100 0039 1905  ..n...*......9..
+00000bb0: 9dfd c000 00a7 bf05 9e88 c300 0092 6605  ..............f.
+00000bc0: a661 8700 004d fc05 a661 8700 0051 6905  .a...M...a...Qi.
+00000bd0: a661 8700 0052 1305 a7f1 8700 0054 e105  .a...R.......T..
+00000be0: adfb 2800 00a0 9105 b039 5c00 000b 7b05  ..(......9\...{.
+00000bf0: b039 5c00 011a 8d05 b093 0000 00c7 c305  .9\.............
+00000c00: b247 c400 009b db05 c068 c000 0009 a705  .G.......h......
+00000c10: c1f8 2200 008d 8d05 ced0 2500 00d8 a505  ..".......%.....
+00000c20: d5fa e400 0080 6205 d5fa e400 012b 3805  ......b......+8.
+00000c30: da03 6e00 005d 8805 dce3 0000 00d1 0105  ..n..]..........
+00000c40: dce3 0000 0101 3705 dde3 7900 0060 a105  ......7...y..`..
+00000c50: e1ed 8400 00be 0e05 ecff 1900 00eb ed05  ................
+00000c60: f264 ba00 0047 3305 f662 ea00 00bc 3805  .d...G3..b....8.
+00000c70: facb 8300 0090 d006 0826 4000 00d6 7e06  .........&@...~.
+00000c80: 08e3 9400 007b 8c06 0ab9 9000 00e2 6506  .....{........e.
+00000c90: 129d e000 00df 2606 148d a400 0021 d706  ......&......!..
+00000ca0: 1867 1e00 0099 fe06 215f 7400 0062 d706  .g......!_t..b..
+00000cb0: 2b00 1300 0037 fd06 2b00 1300 0038 8d06  +....7..+....8..
+00000cc0: 2b00 1300 003a 0a06 34af 4a00 0009 d706  +....:..4.J.....
+00000cd0: 3500 0f00 006c 0606 3c17 4000 00dc 7e06  5....l..<.@...~.
+00000ce0: 3c17 4000 00e8 3a06 3c17 4000 00fa 7006  <.@...:.<.@...p.
+00000cf0: 3c17 4000 0113 bd06 3cee 8400 00ab cb06  <.@.....<.......
+00000d00: 468c a000 00b0 7606 4e38 c500 00a1 3206  F.....v.N8....2.
+00000d10: 4f34 c000 0110 af06 53a5 f500 004b 0706  O4......S....K..
+00000d20: 580f ce00 002a 7e06 5a60 a900 00f8 d806  X....*~.Z`......
+00000d30: 6318 9000 00e6 7906 68ee 6400 001c 8b06  c.....y.h.d.....
+00000d40: 69a9 8400 00a3 8306 69b7 0200 012a 3906  i.......i....*9.
+00000d50: 70e2 d000 006f a206 7cd1 c500 004a 2206  p....o..|....J".
+00000d60: 7f33 4700 0032 ad06 8786 ea00 00a2 6406  .3G..2........d.
+00000d70: 88a1 2400 0136 5a06 8f30 5000 011f 4406  ..$..6Z..0P...D.
+00000d80: 9b5a 7700 011b 2606 9bb8 0c00 0038 d406  .Zw...&......8..
+00000d90: 9c50 2000 00c4 2906 9fb2 5300 00fe 5e06  .P ...)...S...^.
+00000da0: a6d5 8300 012d f906 a8dd 9c00 0053 0706  .....-.......S..
+00000db0: aef9 ce00 005a 6a06 afe6 3000 0072 9d06  .....Zj...0..r..
+00000dc0: b017 2200 00a1 d306 b8bb 6000 00a8 c006  ..".......`.....
+00000dd0: c10c 6000 00ce fc06 c215 0a00 0007 ee06  ..`.............
+00000de0: c227 5a00 0029 0b06 c5bd 6a00 0126 7206  .'Z..)....j..&r.
+00000df0: ce8a a100 004c 4406 cf70 9900 0024 f606  .....LD..p...$..
+00000e00: d08b 2a00 00c9 c706 d81c 2e00 00d9 1006  ..*.............
+00000e10: dbaf 2000 00f0 1806 e231 4000 012d 4f06  .. ......1@..-O.
+00000e20: e6c0 4c00 0053 6c07 0120 6600 0020 e707  ..L..Sl.. f.. ..
+00000e30: 0140 6600 0019 e407 0923 2000 0061 e407  .@f......# ..a..
+00000e40: 0ac3 fa00 00a2 2607 0e35 d000 00dc 1e07  ......&..5......
+00000e50: 126c 4400 013a 7807 1d24 9000 0105 d007  .lD..:x..$......
+00000e60: 1db9 0500 0013 7407 3389 e000 00b7 0c07  ......t.3.......
+00000e70: 3c71 f700 000f 6607 449d 1f00 00be 7307  <q....f.D.....s.
+00000e80: 47cf 0400 0040 ba07 4bcf e000 00e8 8a07  G....@..K.......
+00000e90: 5cec 7500 00a0 ee07 62f5 3500 0040 4107  \.u.....b.5..@A.
+00000ea0: 65e8 b400 007f 1007 65e8 b400 0129 9707  e.......e....)..
+00000eb0: 6c21 5400 000b f607 7e9b 0500 00e7 8b07  l!T.....~.......
+00000ec0: 9a56 2000 0070 c107 9a6c 1400 000c a507  .V ..p...l......
+00000ed0: 9a6c 1400 001c 5207 9a6c 1400 0030 3907  .l....R..l...09.
+00000ee0: 9a6c 1400 0052 cf07 9a6c 1400 0082 ac07  .l...R...l......
+00000ef0: 9a6c 1400 0131 0807 9aa9 6000 00cc 6207  .l...1....`...b.
+00000f00: 9db4 9000 00b9 9507 9db4 9000 00fd ea07  ................
+00000f10: 9e2e 7300 0138 4507 a121 8000 0022 ea07  ..s..8E..!..."..
+00000f20: a674 8700 00a3 d607 bdfe de00 002d 9a07  .t...........-..
+00000f30: cf9a 7000 00fc 0a07 d231 3400 0003 9f07  ..p......14.....
+00000f40: daae 0000 0105 6307 dae0 ea00 011e 3507  ......c.......5.
+00000f50: e0a9 5000 000e a107 e0a9 5000 008a 6d07  ..P.......P...m.
+00000f60: e0a9 5000 011c 3d07 ebd7 9e00 00aa ee07  ..P...=.........
+00000f70: ebd7 9e00 00ad d907 ec42 a500 000a c507  .........B......
+00000f80: ed5c 8000 0112 dc07 f3d4 e000 00ca bc07  .\..............
+00000f90: f714 e400 00f9 5908 0291 0000 0081 8908  ......Y.........
+00000fa0: 08a7 9000 00c5 6408 1f02 9000 00b6 ac08  ......d.........
+00000fb0: 283b 1400 00fe b508 284d 4300 0084 d008  (;......(MC.....
+00000fc0: 28e8 e000 00f0 cf08 2a45 4a00 00a4 2108  (.......*EJ...!.
+00000fd0: 2fe7 9000 009e 3208 3267 1100 0008 a008  /.....2.2g......
+00000fe0: 41da 6e00 0086 8808 426e 6000 0116 c208  A.n.....Bn`.....
+00000ff0: 46c5 3a00 0045 f408 4d37 c500 0093 8508  F.:..E..M7......
+00001000: 4e6b 2a00 0047 7b08 4ef9 1500 005c f208  Nk*..G{.N....\..
+00001010: 4fd0 2000 0116 3f08 6186 7000 0071 bb08  O. ...?.a.p..q..
+00001020: 6c71 e200 00ad 7a08 6f32 c000 00da a008  lq....z.o2......
+00001030: 700d f000 00fb 8308 70b2 8b00 0077 2808  p.......p....w(.
+00001040: 7219 0f00 008a a408 7a4a 5000 007a 2208  r.......zJP..z".
+00001050: 8284 d500 000c d608 8284 d500 0083 1308  ................
+00001060: 8599 7200 0137 6f08 8958 2900 012c 7f08  ..r..7o..X)..,..
+00001070: 8b87 0000 00d2 3808 8fa4 9300 0010 9908  ......8.........
+00001080: 8fa4 9300 0086 d608 8fa4 9300 008c d208  ................
+00001090: 8fa4 9300 011a ee08 9a98 b400 001a c808  ................
+000010a0: 9c61 5e00 011e 9008 a1a4 9300 0059 ab08  .a^..........Y..
+000010b0: a63b 3000 010e 5708 aa82 f400 005b 3c08  .;0...W......[<.
+000010c0: abe2 0900 002b 5f08 abe2 0900 0089 4b08  .....+_.......K.
+000010d0: af11 d500 0063 af08 b89a 9200 0026 9208  .....c.......&..
+000010e0: bbfe c500 0002 ac08 bbfe c500 0127 7c08  .............'|.
+000010f0: bd8a 6000 0118 8508 c000 5000 0098 5b08  ..`.......P...[.
+00001100: c000 5000 0099 1e08 c272 0900 0010 d608  ..P......r......
+00001110: c76b 0300 005a b108 cd7c e400 00aa 7e09  .k...Z...|....~.
+00001120: 00f9 a400 0003 e009 162e f000 003b c609  .............;..
+00001130: 1afc d400 003e 7709 1fb9 f500 0076 cd09  .....>w......v..
+00001140: 2254 0000 0122 2409 2e57 df00 00a6 a609  "T..."$..W......
+00001150: 35e6 6000 0049 5509 3b85 e000 006c e509  5.`..IU.;....l..
+00001160: 4459 d000 00e1 d409 4d67 fe00 011a 1009  DY......Mg......
+00001170: 5962 c900 00e7 ca09 5aa4 1000 00ba 9909  Yb......Z.......
+00001180: 5b68 f000 005f 0509 5c07 3000 00ef 6909  [h..._..\.0...i.
+00001190: 5ca2 3000 0132 f009 5d03 9000 0120 8109  \.0..2..].... ..
+000011a0: 6302 2500 0138 1509 667a 9000 00ed a009  c.%..8..fz......
+000011b0: 66cc c900 0034 b109 700b c500 0012 cf09  f....4..p.......
+000011c0: 7a29 6900 0010 1909 8c00 0a00 0051 2309  z)i..........Q#.
+000011d0: 8c81 5e00 003a 4b09 8c81 5e00 0051 c509  ..^..:K...^..Q..
+000011e0: 8c81 5e00 0098 d409 8d04 b300 0090 0709  ..^.............
+000011f0: 95cb c400 00d7 c209 a6af c300 0057 8d09  .............W..
+00001200: a6c1 0a00 0028 9c09 a6c1 0a00 0045 8b09  .....(.......E..
+00001210: a6c1 0a00 0083 fc09 a6c1 0a00 0098 1e09  ................
+00001220: a6c1 0a00 0124 e009 a6c1 c300 0004 6f09  .....$........o.
+00001230: a87a 8000 00fa c709 b56b a200 008d 0b09  .z.......k......
+00001240: b889 ea00 0087 af09 b889 ea00 00a6 0c09  ................
+00001250: cf34 f000 00e1 3f09 d82d 3f00 0084 3309  .4....?..-?...3.
+00001260: dbfe c000 00db 5f0a 074b 5000 0073 040a  ......_..KP..s..
+00001270: 159b 8000 001f 500a 159b 8000 0055 780a  ......P......Ux.
+00001280: 17d3 5000 00cd 200a 20b0 6000 0079 1c0a  ..P... . .`..y..
+00001290: 20fc 9000 00b4 c50a 22d2 d000 00e5 e40a   .......".......
+000012a0: 2aef e000 00fc 950a 2e99 7e00 0057 c50a  *.........~..W..
+000012b0: 30f6 b500 002a d60a 338b 1000 00de a50a  0....*..3.......
+000012c0: 3f0e 9500 0081 110a 3f0e 9500 012c 3e0a  ?.......?....,>.
+000012d0: 4985 3000 0072 290a 4cb2 e000 00b8 500a  I.0..r).L.....P.
+000012e0: 5e50 b000 010b c50a 62cd 3400 0035 6a0a  ^P......b.4..5j.
+000012f0: 64c8 9500 0087 730a 65e3 f000 005e 4a0a  d.....s.e....^J.
+00001300: 6c11 b300 0005 040a 6c5b d900 000a 580a  l.......l[....X.
+00001310: 6c5b d900 000c 3e0a 6c89 9300 0137 d80a  l[....>.l....7..
+00001320: 70ea 0000 0044 f00a 8170 8e00 0133 c70a  p....D...p...3..
+00001330: 84e6 b500 001d 730a 84e6 b500 0030 d10a  ......s......0..
+00001340: 84e6 b500 0053 d80a 84e6 b500 0131 ac0a  .....S.......1..
+00001350: 84e6 b500 0136 1a0a 89ad 3000 00f6 9e0a  .....6....0.....
+00001360: 89ad 3000 010c fe0a 8c5e f000 0066 cd0a  ..0......^...f..
+00001370: 954c 2000 00dc cf0a 9989 6300 0074 6c0a  .L .......c..tl.
+00001380: ac8c c000 00f9 f70a ae3e fa00 0076 130a  .........>...v..
+00001390: b4bc 2e00 002f 9e0a b5ff 6400 00b2 440a  ...../....d...D.
+000013a0: b6d5 d000 00d3 600a ba90 7000 00e8 f80a  ......`...p.....
+000013b0: be20 4a00 0011 1c0a c25d 1400 0042 530a  . J......]...BS.
+000013c0: c945 a000 00b4 380a ca80 7300 0054 1e0a  .E....8...s..T..
+000013d0: cf76 b400 0058 ff0a cfef 4000 0108 430a  .v...X....@...C.
+000013e0: e1b0 da00 00a9 210a e1b4 8000 0115 c60a  ......!.........
+000013f0: e45f d000 00b9 0e0a eb63 2000 0023 870a  ._.......c ..#..
+00001400: ee50 6000 0082 410a f3de 9e00 0085 a10a  .P`...A.........
+00001410: f818 8000 00b8 890a f818 8000 00fd 580b  ..............X.
+00001420: 0396 6300 0009 720b 03f9 7300 008f bd0b  ..c...r...s.....
+00001430: 0476 b400 0059 390b 0ac1 5a00 012b d40b  .v...Y9...Z..+..
+00001440: 139f b500 0087 e70b 19b8 d700 008b ab0b  ................
+00001450: 1b90 b000 0103 000b 1fcd 0500 00a1 8f0b  ................
+00001460: 20ce b000 00c3 970b 2371 ce00 0001 3e0b   .......#q....>.
+00001470: 244d 8300 0107 1f0b 296c c900 0073 fd0b  $M......)l...s..
+00001480: 2d80 be00 000f c70b 2d80 be00 008c 080b  -.......-.......
+00001490: 2d80 be00 011c c40b 2fa8 e400 0132 ac0b  -......./....2..
+000014a0: 4000 a500 0065 120b 440d ae00 005a ea0b  @....e..D....Z..
+000014b0: 47ce c400 00ea d80b 4841 e400 00bd a80b  G.......HA......
+000014c0: 4e26 9900 0011 620b 543a f400 00e3 080b  N&....b.T:......
+000014d0: 5467 9000 002b fd0b 6948 d000 00c6 830b  Tg...+..iH......
+000014e0: 6b4e 3000 005f e80b 6f1b 4500 0062 4d0b  kN0.._..o.E..bM.
+000014f0: 76dd 9d00 0136 a50b 8a1a 2000 00e4 9f0b  v....6.... .....
+00001500: 8a1a 2000 0112 890b 8c6a e300 005a 2c0b  .. ......j...Z,.
+00001510: 9253 4000 0002 280b 94b6 5e00 00d0 490b  .S@...(...^...I.
+00001520: 967b 5400 0032 5c0b a0c9 de00 0006 5c0b  .{T..2\.......\.
+00001530: a3fc 7000 00f2 770b a4a2 2500 0025 690b  ..p...w...%..%i.
+00001540: c474 9000 00dd 6b0b c4a6 f000 0064 9d0b  .t....k......d..
+00001550: c81a a000 00de 0a0b cbf1 c000 00e4 f20b  ................
+00001560: cbf1 c000 00ea 650b cbf1 c000 00f4 ed0b  ......e.........
+00001570: cbf1 c000 010a c80b db2b b200 0026 430b  .........+...&C.
+00001580: def4 0000 012f f50b e203 8700 000f 1f0b  ...../..........
+00001590: e217 6300 000e dc0b e4a0 3000 0016 c50b  ..c.......0.....
+000015a0: f39a 4000 003a ce0b f39a 4000 0081 d20b  ..@..:....@.....
+000015b0: f39a 4000 00ca 4a0b fc32 3300 0046 290c  ..@...J..23..F).
+000015c0: 04fe c500 0014 360c 0c17 6300 0058 530c  ......6...c..XS.
+000015d0: 0ce3 2300 008f 670c 0dec 5a00 0080 af0c  ..#...g...Z.....
+000015e0: 1cdb 4200 010f 5e0c 1d95 4000 00c1 c40c  ..B...^...@.....
+000015f0: 3834 1400 000e 3b0c 3834 1400 008a 0b0c  84....;.84......
+00001600: 3834 1400 011b db0c 5256 ae00 0034 730c  84......RV...4s.
+00001610: 5bd6 a000 0008 670c 61ce a500 0035 240c  [.....g.a....5$.
+00001620: 63ce a500 000b b00c 6dca b800 0038 3e0c  c.......m....8>.
+00001630: 808a a300 00a5 b20c 83b7 b000 0037 c40c  .............7..
+00001640: 8910 0000 0006 9a0c 89ed e500 004a cf0c  .............J..
+00001650: 98c0 0900 0005 e20c 98c0 0900 000a 8e0c  ................
+00001660: 98c0 0900 000d c70c 98c0 0900 0083 4a0c  ..............J.
+00001670: 98c0 0900 0088 d50c 98c0 0900 009f ee0c  ................
+00001680: 98c0 0900 0119 d70c 9fa9 6000 0121 670c  ..........`..!g.
+00001690: b106 9a00 011d e60c b195 2700 007f b80c  ..........'.....
+000016a0: b1a8 e500 0031 4c0c ba9f 2400 0112 0a0c  .....1L...$.....
+000016b0: c1c5 c300 0091 560c c4e1 d500 0014 7f0c  ......V.........
+000016c0: c5f7 d500 007d ad0c c7ee 6000 009c db0c  .....}....`.....
+000016d0: c8e8 6400 0030 970c c9a0 2e00 007e 0c0c  ..d..0.......~..
+000016e0: cba2 d500 00eb ad0c db0c 0400 00b5 350c  ..............5.
+000016f0: dda2 6e00 00b2 b20c e3ed a900 0091 0b0c  ..n.............
+00001700: f3b0 8500 0013 190c fb0f b300 0093 f70d  ................
+00001710: 0027 2000 00c0 970d 09a5 6000 011f 9c0d  .' .......`.....
+00001720: 0a66 ed00 0129 0b0d 0ad7 7300 004d 170d  .f...)....s..M..
+00001730: 0f91 6000 00f1 590d 0f91 6000 0106 840d  ..`...Y...`.....
+00001740: 1201 a400 005c 7b0d 1cec 6700 011d 120d  .....\{...g.....
+00001750: 2d41 7000 00ae f50d 32db 3000 00ed fb0d  -Ap.....2.0.....
+00001760: 35c6 3000 010a 1b0d 3b8c 3900 00ac 750d  5.0.....;.9...u.
+00001770: 48cd 6500 009a cc0d 51bd f000 00f5 670d  H.e.....Q.....g.
+00001780: 69f6 0000 009d 880d 7298 e700 00ae 310d  i.......r.....1.
+00001790: 7c3b 4000 0113 4f0d 80f6 3400 0097 d30d  |;@...O...4.....
+000017a0: 80f6 3400 0099 630d 8344 9300 0090 4d0d  ..4...c..D....M.
+000017b0: 8c46 7500 0004 a70d 8c46 7500 00a6 470d  .Fu......Fu...G.
+000017c0: 96e3 5000 00e0 1e0d 9df1 6500 001a 7d0d  ..P.......e...}.
+000017d0: 9df1 6500 0021 520d 9ee3 5e00 006d 320d  ..e..!R...^..m2.
+000017e0: 9ee3 5e00 0078 a00d 9ee3 5e00 0085 190d  ..^..x....^.....
+000017f0: 9ee3 5e00 00a4 760d 9ee3 5e00 00b7 8c0d  ..^...v...^.....
+00001800: aa4e 9000 00e7 070d c964 7400 00ab 440d  .N.......dt...D.
+00001810: d0e8 e000 00c9 890d ded8 9000 001d ff0d  ................
+00001820: ded8 9000 0054 5a0d eb49 0000 007f f00d  .....TZ..I......
+00001830: ec49 8400 0048 950d f086 4a00 0039 b50d  .I...H....J..9..
+00001840: fcd5 7e00 003f 300d fe0b 6000 0070 060e  ..~..?0...`..p..
+00001850: 00f0 b000 00d5 630e 03af f000 0077 6c0e  ......c......wl.
+00001860: 1bf8 6400 0039 540e 1ddb 6300 0052 6f0e  ..d..9T...c..Ro.
+00001870: 202b 3a00 007e 6b0e 202b 3a00 0128 720e   +:..~k. +:..(r.
+00001880: 20d7 0900 010f ac0e 2511 7400 0060 eb0e   .......%.t..`..
+00001890: 38a0 f000 0107 a40e 5c13 4700 011b 5a0e  8.......\.G...Z.
+000018a0: 6193 e900 0114 7d0e 61d5 0400 00a9 700e  a.....}.a.....p.
+000018b0: 68cb dc00 0057 270e 6ac2 e300 0025 a00e  h....W'.j....%..
+000018c0: 7617 2000 007b dd0e 8347 4400 006a 930e  v. ..{...GD..j..
+000018d0: 887b b500 0037 590e 887b b500 00aa 470e  .{...7Y..{....G.
+000018e0: 9dcc d400 0033 560e a934 c000 0061 6a0e  .....3V..4...aj.
+000018f0: abf5 1300 0068 410e ae34 8000 005e a50e  .....hA..4...^..
+00001900: b4a5 0a00 0064 380e b5c2 8000 009b 2e0e  .....d8.........
+00001910: b803 9900 006e f60e b82d 1000 00f5 fb0e  .....n...-......
+00001920: c28b b000 0003 0c0e d945 de00 002e 560e  .........E....V.
+00001930: e77d 7000 0123 db0e f7f8 4000 00f1 fa0f  .}p..#....@.....
+00001940: 09fd b000 00d7 270f 0cc4 c000 00fd 050f  ......'.........
+00001950: 105e a000 00bb cd0f 11be 6000 00c1 0c0f  .^........`.....
+00001960: 1d28 1000 0100 c70f 201d 8500 0089 8a0f  .(...... .......
+00001970: 20f1 3000 00d9 670f 4321 f500 0134 5e0f   .0...g.C!...4^.
+00001980: 4a90 4000 00b4 7c0f 5e00 1000 00cb 450f  J.@...|.^.....E.
+00001990: 8e7b e000 00cf a70f 9222 7c00 00ac 350f  .{......."|...5.
+000019a0: 9450 0000 0117 2e0f 9ebd c400 0048 ed0f  .P...........H..
+000019b0: 9fbc 6000 0138 e80f a262 9000 013b 5f0f  ..`..8...b...;_.
+000019c0: a44f 0300 0000 5f0f bd5e e700 011c 740f  .O...._..^....t.
+000019d0: cb15 5200 006a 470f cf80 f000 00f7 420f  ..R..jG.......B.
+000019e0: d19a 7000 00c2 7d0f dfeb 7000 009f 190f  ..p...}...p.....
+000019f0: e7f7 9000 013a ed0f ea8a 0900 007e b00f  .....:.......~..
+00001a00: ea8a 0900 00a7 670f ea8a 0900 0128 b10f  ......g......(..
+00001a10: f87c e000 0024 6d0f fe37 0300 0087 1569  .|...$m..7.....i
+00001a20: 0001 3bda 0300 0000 2404 1e04 4204 3c04  ..;.....$...B.<.
+00001a30: 3504 3d04 3804 4204 4c00 2004 3804 3704  5.=.8.B.L. .8.7.
+00001a40: 3c04 3504 3d04 3504 3d04 3804 4f08 0000  <.5.=.5.=.8.O...
+00001a50: 0000 0600 0000 0e43 616e 6365 6c20 6368  .......Cancel ch
+00001a60: 616e 6765 7307 0000 0018 4162 7374 7261  anges.....Abstra
+00001a70: 6374 4f70 6572 6174 696f 6e44 6574 6169  ctOperationDetai
+00001a80: 6c73 0103 0000 0026 0421 043e 0445 0440  ls.....&.!.>.E.@
+00001a90: 0430 043d 0438 0442 044c 0020 0438 0437  .0.=.8.B.L. .8.7
+00001aa0: 043c 0435 043d 0435 043d 0438 044f 0800  .<.5.=.5.=.8.O..
+00001ab0: 0000 0006 0000 000e 436f 6d6d 6974 2063  ........Commit c
+00001ac0: 6861 6e67 6573 0700 0000 1841 6273 7472  hanges.....Abstr
+00001ad0: 6163 744f 7065 7261 7469 6f6e 4465 7461  actOperationDeta
+00001ae0: 696c 7301 0300 0000 3804 1e04 4804 3804  ils.....8...H.8.
+00001af0: 3104 3a04 3000 2004 3f04 4004 3800 2004  1.:.0. .?.@.8. .
+00001b00: 3704 3004 3f04 3804 4104 3800 2004 3e04  7.0.?.8.A.8. .>.
+00001b10: 3f04 3504 4004 3004 4604 3804 3800 3a00  ?.5.@.0.F.8.8.:.
+00001b20: 2008 0000 0000 0600 0000 194f 7065 7261   ..........Opera
+00001b30: 7469 6f6e 2073 7562 6d69 7420 6661 696c  tion submit fail
+00001b40: 6564 3a20 0700 0000 1841 6273 7472 6163  ed: .....Abstrac
+00001b50: 744f 7065 7261 7469 6f6e 4465 7461 696c  tOperationDetail
+00001b60: 7301 0300 0000 8804 1d04 3504 4104 3e04  s.........5.A.>.
+00001b70: 4504 4004 3004 3d04 5104 3d04 3d04 4b04  E.@.0.=.Q.=.=.K.
+00001b80: 3500 2004 3804 3704 3c04 3504 3d04 3504  5. .8.7.<.5.=.5.
+00001b90: 3d04 3804 4f00 2004 3104 4b04 3b04 3800  =.8.O. .1.K.;.8.
+00001ba0: 2004 3e04 4204 3c04 3504 3d04 3504 3d04   .>.B.<.5.=.5.=.
+00001bb0: 4b00 2004 3f04 3504 4004 3504 3400 2004  K. .?.5.@.5.4. .
+00001bc0: 4104 3e04 3704 3404 3004 3d04 3804 3504  A.>.7.4.0.=.8.5.
+00001bd0: 3c00 2004 3d04 3e04 3204 3e04 3900 2004  <. .=.>.2.>.9. .
+00001be0: 3e04 3f04 3504 4004 3004 4604 3804 3808  >.?.5.@.0.F.8.8.
+00001bf0: 0000 0000 0600 0000 3555 6e73 6176 6564  ........5Unsaved
+00001c00: 2063 6861 6e67 6573 2077 6572 6520 7265   changes were re
+00001c10: 7665 7274 6564 2074 6f20 6372 6561 7465  verted to create
+00001c20: 206e 6577 206f 7065 7261 7469 6f6e 0700   new operation..
+00001c30: 0000 1841 6273 7472 6163 744f 7065 7261  ...AbstractOpera
+00001c40: 7469 6f6e 4465 7461 696c 7301 0300 0000  tionDetails.....
+00001c50: 3a04 1d04 3504 3204 3504 4004 3d04 3e04  :...5.2.5.@.=.>.
+00001c60: 3500 2004 3704 3d04 3004 4704 3504 3d04  5. .7.=.0.G.5.=.
+00001c70: 3804 3500 2004 3200 2004 4104 4204 3e04  8.5. .2. .A.B.>.
+00001c80: 3b04 3104 4604 3500 3a00 2008 0000 0000  ;.1.F.5.:. .....
+00001c90: 0600 0000 1b43 6f6c 756d 6e20 6861 7320  .....Column has 
+00001ca0: 6e6f 2076 616c 6964 2076 616c 7565 3a20  no valid value: 
+00001cb0: 0700 0000 1a41 6273 7472 6163 7452 6566  .....AbstractRef
+00001cc0: 6572 656e 6365 4c69 7374 4d6f 6465 6c01  erenceListModel.
+00001cd0: 0300 0000 1e04 1d04 3504 3f04 3e04 3b04  ........5.?.>.;.
+00001ce0: 3d04 4b04 3500 2004 3404 3004 3d04 3d04  =.K.5. .4.0.=.=.
+00001cf0: 4b04 3508 0000 0000 0600 0000 1344 6174  K.5..........Dat
+00001d00: 6120 6172 6520 696e 636f 6d70 6c65 7465  a are incomplete
+00001d10: 0700 0000 1a41 6273 7472 6163 7452 6566  .....AbstractRef
+00001d20: 6572 656e 6365 4c69 7374 4d6f 6465 6c01  erenceListModel.
+00001d30: 0300 0000 2604 1e04 4804 3804 3104 3a04  ....&...H.8.1.:.
+00001d40: 3000 2004 4104 3e04 4504 4004 3004 3d04  0. .A.>.E.@.0.=.
+00001d50: 3504 3d04 3804 4f00 3a00 2008 0000 0000  5.=.8.O.:. .....
+00001d60: 0600 0000 0f53 7562 6d69 7420 6661 696c  .....Submit fail
+00001d70: 6564 3a20 0700 0000 1a41 6273 7472 6163  ed: .....Abstrac
+00001d80: 7452 6566 6572 656e 6365 4c69 7374 4d6f  tReferenceListMo
+00001d90: 6465 6c01 0300 0000 0a04 1b04 4e04 3104  del.........N.1.
+00001da0: 3e04 3908 0000 0000 0600 0000 0341 4e59  >.9..........ANY
+00001db0: 0700 0000 0d41 6363 6f75 6e74 4275 7474  .....AccountButt
+00001dc0: 6f6e 0103 0000 0014 041b 044e 0431 043e  on.........N.1.>
+00001dd0: 0439 0020 0441 0447 0435 0442 0800 0000  .9. .A.G.5.B....
+00001de0: 0006 0000 000b 416e 7920 6163 636f 756e  ......Any accoun
+00001df0: 7407 0000 000d 4163 636f 756e 7442 7574  t.....AccountBut
+00001e00: 746f 6e01 0300 0000 1804 1204 4b04 3104  ton.........K.1.
+00001e10: 4004 3004 4204 4c00 2004 4104 4704 3504  @.0.B.L. .A.G.5.
+00001e20: 4208 0000 0000 0600 0000 0e43 686f 6f73  B..........Choos
+00001e30: 6520 6163 636f 756e 7407 0000 000d 4163  e account.....Ac
+00001e40: 636f 756e 7442 7574 746f 6e01 0300 0000  countButton.....
+00001e50: 1404 2204 3804 3f00 2004 4104 4704 3504  ..".8.?. .A.G.5.
+00001e60: 4204 3000 3a08 0000 0000 0600 0000 0d41  B.0.:..........A
+00001e70: 6363 6f75 6e74 2074 7970 653a 0700 0000  ccount type:....
+00001e80: 1141 6363 6f75 6e74 4c69 7374 4469 616c  .AccountListDial
+00001e90: 6f67 0103 0000 000a 0421 0447 0435 0442  og.......!.G.5.B
+00001ea0: 0430 0800 0000 0006 0000 0008 4163 636f  .0..........Acco
+00001eb0: 756e 7473 0700 0000 1141 6363 6f75 6e74  unts.....Account
+00001ec0: 4c69 7374 4469 616c 6f67 0103 0000 002a  ListDialog.....*
+00001ed0: 041f 043e 043a 0430 0437 044b 0432 0430  ...>.:.0.7.K.2.0
+00001ee0: 0442 044c 0020 043d 0435 0430 043a 0442  .B.L. .=.5.0.:.B
+00001ef0: 0438 0432 043d 044b 0435 0800 0000 0006  .8.2.=.K.5......
+00001f00: 0000 000d 5368 6f77 2069 6e61 6374 6976  ....Show inactiv
+00001f10: 6507 0000 0011 4163 636f 756e 744c 6973  e.....AccountLis
+00001f20: 7444 6961 6c6f 6701 0300 0000 0e21 1600  tDialog......!..
+00001f30: 2004 4104 4704 3504 4204 3008 0000 0000   .A.G.5.B.0.....
+00001f40: 0600 0000 0941 6363 6f75 6e74 2023 0700  .....Account #..
+00001f50: 0000 1041 6363 6f75 6e74 4c69 7374 4d6f  ...AccountListMo
+00001f60: 6465 6c01 0300 0000 0804 1004 3a04 4200  del.........:.B.
+00001f70: 2e08 0000 0000 0600 0000 0441 6374 2e07  ...........Act..
+00001f80: 0000 0010 4163 636f 756e 744c 6973 744d  ....AccountListM
+00001f90: 6f64 656c 0103 0000 0016 0411 0430 043d  odel.........0.=
+00001fa0: 043a 002f 0411 0440 043e 043a 0435 0440  .:./...@.>.:.5.@
+00001fb0: 0800 0000 0006 0000 000b 4261 6e6b 2f42  ..........Bank/B
+00001fc0: 726f 6b65 7207 0000 0010 4163 636f 756e  roker.....Accoun
+00001fd0: 744c 6973 744d 6f64 656c 0103 0000 0004  tListModel......
+00001fe0: 041a 0421 0800 0000 0006 0000 0002 4343  ...!..........CC
+00001ff0: 0700 0000 1041 6363 6f75 6e74 4c69 7374  .....AccountList
+00002000: 4d6f 6465 6c01 0300 0000 0c04 1204 3004  Model.........0.
+00002010: 3b04 4e04 4204 3008 0000 0000 0600 0000  ;.N.B.0.........
+00002020: 0843 7572 7265 6e63 7907 0000 0010 4163  .Currency.....Ac
+00002030: 636f 756e 744c 6973 744d 6f64 656c 0103  countListModel..
+00002040: 0000 0018 041d 0430 0438 043c 0435 043d  .......0.8.<.5.=
+00002050: 043e 0432 0430 043d 0438 0435 0800 0000  .>.2.0.=.8.5....
+00002060: 0006 0000 0004 4e61 6d65 0700 0000 1041  ......Name.....A
+00002070: 6363 6f75 6e74 4c69 7374 4d6f 6465 6c01  ccountListModel.
+00002080: 0300 0000 1004 2204 3e04 4704 3d04 3e04  ......".>.G.=.>.
+00002090: 4104 4204 4c08 0000 0000 0600 0000 0950  A.B.L..........P
+000020a0: 7265 6369 7369 6f6e 0700 0000 1041 6363  recision.....Acc
+000020b0: 6f75 6e74 4c69 7374 4d6f 6465 6c01 0300  ountListModel...
+000020c0: 0000 1004 2104 3204 3504 4004 3504 3d00  ....!.2.5.@.5.=.
+000020d0: 2000 4008 0000 0000 0600 0000 0c52 6563   .@..........Rec
+000020e0: 6f6e 6369 6c65 6420 4007 0000 0010 4163  onciled @.....Ac
+000020f0: 636f 756e 744c 6973 744d 6f64 656c 0103  countListModel..
+00002100: 0000 001a 0426 0435 043d 043d 0430 044f  .....&.5.=.=.0.O
+00002110: 0020 0431 0443 043c 0430 0433 0430 0800  . .1.C.<.0.3.0..
+00002120: 0000 0006 0000 0005 4173 7365 7407 0000  ........Asset...
+00002130: 000b 4173 7365 7444 6961 6c6f 6701 0300  ..AssetDialog...
+00002140: 0000 3e04 1e04 4804 3804 3104 3a04 3000  ..>...H.8.1.:.0.
+00002150: 2004 3704 3004 3f04 3804 4104 3800 2004   .7.0.?.8.A.8. .
+00002160: 3804 3d04 4404 3e04 4004 3c04 3004 4604  8.=.D.>.@.<.0.F.
+00002170: 3804 3800 2004 3e00 2004 2604 1100 3a00  8.8. .>. .&...:.
+00002180: 2008 0000 0000 0600 0000 1d41 7373 6574   ..........Asset
+00002190: 2064 6574 6169 6c73 2073 7562 6d69 7420   details submit 
+000021a0: 6661 696c 6564 3a20 0700 0000 0b41 7373  failed: .....Ass
+000021b0: 6574 4469 616c 6f67 0103 0000 0024 041e  etDialog.....$..
+000021c0: 0448 0438 0431 043a 0430 0020 0437 0430  .H.8.1.:.0. .7.0
+000021d0: 043f 0438 0441 0438 0020 0426 0415 003a  .?.8.A.8. .&...:
+000021e0: 0020 0800 0000 0006 0000 0015 4173 7365  . ..........Asse
+000021f0: 7420 7375 626d 6974 2066 6169 6c65 643a  t submit failed:
+00002200: 2007 0000 000b 4173 7365 7444 6961 6c6f   .....AssetDialo
+00002210: 6701 0300 0000 1c04 1104 3004 3704 3e04  g.........0.7.>.
+00002220: 3204 4b04 3900 2004 3004 3a04 4204 3804  2.K.9. .0.:.B.8.
+00002230: 3200 3a08 0000 0000 0600 0000 0b42 6173  2.:..........Bas
+00002240: 6520 6173 7365 743a 0700 0000 0b41 7373  e asset:.....Ass
+00002250: 6574 4469 616c 6f67 0103 0000 000c 041e  etDialog........
+00002260: 0442 043c 0435 043d 0430 0800 0000 0006  .B.<.5.=.0......
+00002270: 0000 0006 4361 6e63 656c 0700 0000 0b41  ....Cancel.....A
+00002280: 7373 6574 4469 616c 6f67 0103 0000 0010  ssetDialog......
+00002290: 0421 0442 0440 0430 043d 0430 003a 0020  .!.B.@.0.=.0.:. 
+000022a0: 0800 0000 0006 0000 0009 436f 756e 7472  ..........Countr
+000022b0: 793a 2007 0000 000b 4173 7365 7444 6961  y: .....AssetDia
+000022c0: 6c6f 6701 0300 0000 1404 1404 3e04 3f00  log.........>.?.
+000022d0: 2e04 3404 3004 3d04 3d04 4b04 3508 0000  ..4.0.=.=.K.5...
+000022e0: 0000 0600 0000 0a45 7874 7261 2064 6174  .......Extra dat
+000022f0: 6107 0000 000b 4173 7365 7444 6961 6c6f  a.....AssetDialo
+00002300: 6701 0300 0000 0a00 4900 5300 4900 4e00  g.......I.S.I.N.
+00002310: 3a08 0000 0000 0600 0000 0549 5349 4e3a  :..........ISIN:
+00002320: 0700 0000 0b41 7373 6574 4469 616c 6f67  .....AssetDialog
+00002330: 0103 0000 001a 041d 0430 0438 043c 0435  .........0.8.<.5
+00002340: 043d 043e 0432 0430 043d 0438 0435 003a  .=.>.2.0.=.8.5.:
+00002350: 0800 0000 0006 0000 0005 4e61 6d65 3a07  ..........Name:.
+00002360: 0000 000b 4173 7365 7444 6961 6c6f 6701  ....AssetDialog.
+00002370: 0300 0000 0404 1e04 1a08 0000 0000 0600  ................
+00002380: 0000 024f 4b07 0000 000b 4173 7365 7444  ...OK.....AssetD
+00002390: 6961 6c6f 6701 0300 0000 0e04 2104 3804  ialog.......!.8.
+000023a0: 3c04 3204 3e04 3b04 4b08 0000 0000 0600  <.2.>.;.K.......
+000023b0: 0000 0753 796d 626f 6c73 0700 0000 0b41  ...Symbols.....A
+000023c0: 7373 6574 4469 616c 6f67 0103 0000 000a  ssetDialog......
+000023d0: 0422 0438 043f 003a 0020 0800 0000 0006  .".8.?.:. ......
+000023e0: 0000 0006 5479 7065 3a20 0700 0000 0b41  ....Type: .....A
+000023f0: 7373 6574 4469 616c 6f67 0103 0000 000e  ssetDialog......
+00002400: 0422 0438 043f 0020 0426 0411 003a 0800  .".8.?. .&...:..
+00002410: 0000 0006 0000 000b 4173 7365 7420 7479  ........Asset ty
+00002420: 7065 3a07 0000 000f 4173 7365 744c 6973  pe:.....AssetLis
+00002430: 7444 6961 6c6f 6701 0300 0000 1a04 2604  tDialog.......&.
+00002440: 3504 3d04 3d04 4b04 3500 2004 3104 4304  5.=.=.K.5. .1.C.
+00002450: 3c04 3004 3304 3808 0000 0000 0600 0000  <.0.3.8.........
+00002460: 0641 7373 6574 7307 0000 000f 4173 7365  .Assets.....Asse
+00002470: 744c 6973 7444 6961 6c6f 6701 0300 0000  tListDialog.....
+00002480: 0c04 2104 4204 4004 3004 3d04 3008 0000  ..!.B.@.0.=.0...
+00002490: 0000 0600 0000 0743 6f75 6e74 7279 0700  .......Country..
+000024a0: 0000 0e41 7373 6574 4c69 7374 4d6f 6465  ...AssetListMode
+000024b0: 6c01 0300 0000 0c04 1204 3004 3b04 4e04  l.........0.;.N.
+000024c0: 4204 3008 0000 0000 0600 0000 0843 7572  B.0..........Cur
+000024d0: 7265 6e63 7907 0000 000e 4173 7365 744c  rency.....AssetL
+000024e0: 6973 744d 6f64 656c 0103 0000 001a 0418  istModel........
+000024f0: 0441 0442 002e 043a 043e 0442 0438 0440  .A.B...:.>.B.8.@
+00002500: 043e 0432 043e 043a 0800 0000 0006 0000  .>.2.>.:........
+00002510: 000b 4461 7461 2073 6f75 7263 6507 0000  ..Data source...
+00002520: 000e 4173 7365 744c 6973 744d 6f64 656c  ..AssetListModel
+00002530: 0103 0000 0008 0049 0053 0049 004e 0800  .......I.S.I.N..
+00002540: 0000 0006 0000 0004 4953 494e 0700 0000  ........ISIN....
+00002550: 0e41 7373 6574 4c69 7374 4d6f 6465 6c01  .AssetListModel.
+00002560: 0300 0000 1804 1d04 3004 3804 3c04 3504  ........0.8.<.5.
+00002570: 3d04 3e04 3204 3004 3d04 3804 3508 0000  =.>.2.0.=.8.5...
+00002580: 0000 0600 0000 044e 616d 6507 0000 000e  .......Name.....
+00002590: 4173 7365 744c 6973 744d 6f64 656c 0103  AssetListModel..
+000025a0: 0000 000c 0421 0438 043c 0432 043e 043b  .....!.8.<.2.>.;
+000025b0: 0800 0000 0006 0000 0006 5379 6d62 6f6c  ..........Symbol
+000025c0: 0700 0000 0e41 7373 6574 4c69 7374 4d6f  .....AssetListMo
+000025d0: 6465 6c01 0300 0000 1804 1d04 3004 3804  del.........0.8.
+000025e0: 3c04 3504 3d04 3e04 3204 3004 3d04 3804  <.5.=.>.2.0.=.8.
+000025f0: 3508 0000 0000 0600 0000 0a41 7373 6574  5..........Asset
+00002600: 206e 616d 6507 0000 000f 4173 7365 7473   name.....Assets
+00002610: 4c69 7374 4d6f 6465 6c01 0300 0000 1a04  ListModel.......
+00002620: 1104 3004 3704 3e04 3204 4b04 3900 2004  ..0.7.>.2.K.9. .
+00002630: 3004 3a04 4204 3804 3208 0000 0000 0600  0.:.B.8.2.......
+00002640: 0000 0a42 6173 6520 6173 7365 7407 0000  ...Base asset...
+00002650: 000f 4173 7365 7473 4c69 7374 4d6f 6465  ..AssetsListMode
+00002660: 6c01 0300 0000 0c04 2104 4204 4004 3004  l.......!.B.@.0.
+00002670: 3d04 3008 0000 0000 0600 0000 0743 6f75  =.0..........Cou
+00002680: 6e74 7279 0700 0000 0f41 7373 6574 734c  ntry.....AssetsL
+00002690: 6973 744d 6f64 656c 0103 0000 0008 0049  istModel.......I
+000026a0: 0053 0049 004e 0800 0000 0006 0000 0004  .S.I.N..........
+000026b0: 4953 494e 0700 0000 0f41 7373 6574 734c  ISIN.....AssetsL
+000026c0: 6973 744d 6f64 656c 0103 0000 0008 0421  istModel.......!
+000026d0: 0447 0435 0442 0800 0000 0006 0000 0007  .G.5.B..........
+000026e0: 4163 636f 756e 7407 0000 000d 4261 6c61  Account.....Bala
+000026f0: 6e63 6573 4d6f 6465 6c01 0300 0000 0c04  ncesModel.......
+00002700: 1104 3004 3b04 3004 3d04 4108 0000 0000  ..0.;.0.=.A.....
+00002710: 0600 0000 0742 616c 616e 6365 0700 0000  .....Balance....
+00002720: 0d42 616c 616e 6365 734d 6f64 656c 0103  .BalancesModel..
+00002730: 0000 0010 0411 0430 043b 0430 043d 0441  .......0.;.0.=.A
+00002740: 002c 0020 0800 0000 0006 0000 0009 4261  .,. ..........Ba
+00002750: 6c61 6e63 652c 2007 0000 000d 4261 6c61  lance, .....Bala
+00002760: 6e63 6573 4d6f 6465 6c01 0300 0000 0a04  ncesModel.......
+00002770: 1804 4204 3e04 3304 3e08 0000 0000 0600  ..B.>.3.>.......
+00002780: 0000 0554 6f74 616c 0700 0000 0d42 616c  ...Total.....Bal
+00002790: 616e 6365 734d 6f64 656c 0103 0000 001c  ancesModel......
+000027a0: 0411 0430 0437 043e 0432 0430 044f 0020  ...0.7.>.2.0.O. 
+000027b0: 0432 0430 043b 044e 0442 0430 0800 0000  .2.0.;.N.B.0....
+000027c0: 0006 0000 000d 4261 7365 2063 7572 7265  ......Base curre
+000027d0: 6e63 7907 0000 0012 4261 7365 4375 7272  ncy.....BaseCurr
+000027e0: 656e 6379 4469 616c 6f67 0103 0000 000c  encyDialog......
+000027f0: 0412 0430 043b 044e 0442 0430 0800 0000  ...0.;.N.B.0....
+00002800: 0006 0000 0008 4375 7272 656e 6379 0700  ......Currency..
+00002810: 0000 1542 6173 6543 7572 7265 6e63 794c  ...BaseCurrencyL
+00002820: 6973 744d 6f64 656c 0103 0000 0008 0414  istModel........
+00002830: 0430 0442 0430 0800 0000 0006 0000 0004  .0.B.0..........
+00002840: 4461 7465 0700 0000 1542 6173 6543 7572  Date.....BaseCur
+00002850: 7265 6e63 794c 6973 744d 6f64 656c 0103  rencyListModel..
+00002860: 0000 0024 0027 0020 0437 0430 043c 0435  ...$.'. .7.0.<.5
+00002870: 043d 0435 043d 0430 0020 0443 0441 043f  .=.5.=.0. .C.A.?
+00002880: 0435 0448 043d 043e 0800 0000 0006 0000  .5.H.=.>........
+00002890: 001b 2720 7761 7320 7375 6363 6573 7366  ..' was successf
+000028a0: 756c 6c79 2072 6570 6c61 6365 6407 0000  ully replaced...
+000028b0: 0012 4361 7465 676f 7279 4c69 7374 4469  ..CategoryListDi
+000028c0: 616c 6f67 0103 0000 000c 0027 0020 043d  alog.......'. .=
+000028d0: 0430 003a 0020 0800 0000 0006 0000 0008  .0.:. ..........
+000028e0: 2720 7769 7468 3a20 0700 0000 1243 6174  ' with: .....Cat
+000028f0: 6567 6f72 794c 6973 7444 6961 6c6f 6701  egoryListDialog.
+00002900: 0300 0000 1204 1a04 3004 4204 3504 3304  ........0.B.5.3.
+00002910: 3e04 4004 3804 3808 0000 0000 0600 0000  >.@.8.8.........
+00002920: 0a43 6174 6567 6f72 6965 7307 0000 0012  .Categories.....
+00002930: 4361 7465 676f 7279 4c69 7374 4469 616c  CategoryListDial
+00002940: 6f67 0103 0000 0016 041a 0430 0442 0435  og.........0.B.5
+00002950: 0433 043e 0440 0438 044f 0020 0027 0800  .3.>.@.8.O. .'..
+00002960: 0000 0006 0000 000a 4361 7465 676f 7279  ........Category
+00002970: 2027 0700 0000 1243 6174 6567 6f72 794c   '.....CategoryL
+00002980: 6973 7444 6961 6c6f 6701 0300 0000 2804  istDialog.....(.
+00002990: 1704 3004 3c04 3504 3d04 3804 4204 4c00  ..0.<.5.=.8.B.L.
+000029a0: 2004 3a04 3004 4204 3504 3304 3e04 4004   .:.0.B.5.3.>.@.
+000029b0: 3804 4e00 2000 2708 0000 0000 0600 0000  8.N. .'.........
+000029c0: 1252 6570 6c61 6365 2063 6174 6567 6f72  .Replace categor
+000029d0: 7920 2707 0000 0012 4361 7465 676f 7279  y '.....Category
+000029e0: 4c69 7374 4469 616c 6f67 0103 0000 001c  ListDialog......
+000029f0: 0417 0430 043c 0435 043d 0438 0442 044c  ...0.<.5.=.8.B.L
+00002a00: 0020 043d 0430 002e 002e 002e 0800 0000  . .=.0..........
+00002a10: 0006 0000 000f 5265 706c 6163 6520 7769  ......Replace wi
+00002a20: 7468 2e2e 2e07 0000 0012 4361 7465 676f  th........Catego
+00002a30: 7279 4c69 7374 4469 616c 6f67 0103 0000  ryListDialog....
+00002a40: 003c 041f 043e 043a 0430 0437 0430 0442  .<...>.:.0.7.0.B
+00002a50: 044c 0020 043e 043f 0435 0440 0430 0446  .L. .>.?.5.@.0.F
+00002a60: 0438 0438 0020 0441 0020 041a 0430 0442  .8.8. .A. ...0.B
+00002a70: 0435 0433 043e 0440 0438 0435 0439 0800  .5.3.>.@.8.5.9..
+00002a80: 0000 0006 0000 001d 5368 6f77 206f 7065  ........Show ope
+00002a90: 7261 7469 6f6e 7320 7769 7468 2043 6174  rations with Cat
+00002aa0: 6567 6f72 7907 0000 0012 4361 7465 676f  egory.....Catego
+00002ab0: 7279 4c69 7374 4469 616c 6f67 0103 0000  ryListDialog....
+00002ac0: 0010 041e 043f 0435 0440 0430 0446 0438  .....?.5.@.0.F.8
+00002ad0: 0438 0800 0000 0006 0000 000a 4f70 6572  .8..........Oper
+00002ae0: 6174 696f 6e73 0700 0000 0e43 6174 6567  ations.....Categ
+00002af0: 6f72 7952 6570 6f72 7401 0300 0000 1804  oryReport.......
+00002b00: 3f04 3e00 2004 1a04 3004 4204 3504 3304  ?.>. ...0.B.5.3.
+00002b10: 3e04 4004 3804 3808 0000 0000 0600 0000  >.@.8.8.........
+00002b20: 0b62 7920 4361 7465 676f 7279 0700 0000  .by Category....
+00002b30: 0e43 6174 6567 6f72 7952 6570 6f72 7401  .CategoryReport.
+00002b40: 0300 0000 1404 1a04 3004 4204 3504 3304  ........0.B.5.3.
+00002b50: 3e04 4004 3804 4f00 3a08 0000 0000 0600  >.@.8.O.:.......
+00002b60: 0000 0943 6174 6567 6f72 793a 0700 0000  ...Category:....
+00002b70: 1443 6174 6567 6f72 7952 6570 6f72 7457  .CategoryReportW
+00002b80: 6964 6765 7401 0300 0000 2404 1e04 4204  idget.....$...B.
+00002b90: 4704 5104 4200 2004 3f04 3e00 2004 3a04  G.Q.B. .?.>. .:.
+00002ba0: 3004 4204 3504 3304 3e04 4004 3804 3808  0.B.5.3.>.@.8.8.
+00002bb0: 0000 0000 0600 0000 1252 6570 6f72 7420  .........Report 
+00002bc0: 6279 2063 6174 6567 6f72 7907 0000 0014  by category.....
+00002bd0: 4361 7465 676f 7279 5265 706f 7274 5769  CategoryReportWi
+00002be0: 6467 6574 0103 0000 0018 041d 0430 0438  dget.........0.8
+00002bf0: 043c 0435 043d 043e 0432 0430 043d 0438  .<.5.=.>.2.0.=.8
+00002c00: 0435 0800 0000 0006 0000 0004 4e61 6d65  .5..........Name
+00002c10: 0700 0000 1143 6174 6567 6f72 7954 7265  .....CategoryTre
+00002c20: 654d 6f64 656c 0103 0000 000c 0427 0430  eModel.......'.0
+00002c30: 0441 0442 0430 044f 0800 0000 0006 0000  .A.B.0.O........
+00002c40: 0005 4f66 7465 6e07 0000 0011 4361 7465  ..Often.....Cate
+00002c50: 676f 7279 5472 6565 4d6f 6465 6c01 0300  goryTreeModel...
+00002c60: 0000 2004 1304 4004 3004 4404 3804 3a00  .. ...@.0.D.8.:.
+00002c70: 2004 4604 3504 3d04 4b00 2004 3404 3b04   .F.5.=.K. .4.;.
+00002c80: 4f00 2008 0000 0000 0600 0000 1050 7269  O. ..........Pri
+00002c90: 6365 2063 6861 7274 2066 6f72 2007 0000  ce chart for ...
+00002ca0: 000b 4368 6172 7457 696e 646f 7701 0300  ..ChartWindow...
+00002cb0: 0000 1a04 2604 3504 3d04 3d04 3004 4f00  ....&.5.=.=.0.O.
+00002cc0: 2004 3104 4304 3c04 3004 3304 3008 0000   .1.C.<.0.3.0...
+00002cd0: 0000 0600 0000 0541 7373 6574 0700 0000  .......Asset....
+00002ce0: 1143 6c6f 7365 6454 7261 6465 734d 6f64  .ClosedTradesMod
+00002cf0: 656c 0103 0000 001a 0414 0430 0442 0430  el.........0.B.0
+00002d00: 0020 0437 0430 043a 0440 044b 0442 0438  . .7.0.:.@.K.B.8
+00002d10: 044f 0800 0000 0006 0000 000a 436c 6f73  .O..........Clos
+00002d20: 6520 4461 7465 0700 0000 1143 6c6f 7365  e Date.....Close
+00002d30: 6454 7261 6465 734d 6f64 656c 0103 0000  dTradesModel....
+00002d40: 0026 0414 0430 0442 0430 002f 0432 0440  .&...0.B.0./.2.@
+00002d50: 0435 043c 044f 0020 0437 0430 043a 0440  .5.<.O. .7.0.:.@
+00002d60: 044b 0442 0438 044f 0800 0000 0006 0000  .K.B.8.O........
+00002d70: 000f 436c 6f73 6520 4461 7465 2f54 696d  ..Close Date/Tim
+00002d80: 6507 0000 0011 436c 6f73 6564 5472 6164  e.....ClosedTrad
+00002d90: 6573 4d6f 6465 6c01 0300 0000 1a04 2604  esModel.......&.
+00002da0: 3504 3d04 3000 2004 3704 3004 3a04 4004  5.=.0. .7.0.:.@.
+00002db0: 4b04 4204 3804 4f08 0000 0000 0600 0000  K.B.8.O.........
+00002dc0: 0b43 6c6f 7365 2050 7269 6365 0700 0000  .Close Price....
+00002dd0: 1143 6c6f 7365 6454 7261 6465 734d 6f64  .ClosedTradesMod
+00002de0: 656c 0103 0000 0010 041a 043e 043c 0438  el.........>.<.8
+00002df0: 0441 0441 0438 044f 0800 0000 0006 0000  .A.A.8.O........
+00002e00: 0003 4665 6507 0000 0011 436c 6f73 6564  ..Fee.....Closed
+00002e10: 5472 6164 6573 4d6f 6465 6c01 0300 0000  TradesModel.....
+00002e20: 1404 1f04 4004 3804 3c04 3504 4704 3004  ....@.8.<.5.G.0.
+00002e30: 3d04 3804 3508 0000 0000 0600 0000 044e  =.8.5..........N
+00002e40: 6f74 6507 0000 0011 436c 6f73 6564 5472  ote.....ClosedTr
+00002e50: 6164 6573 4d6f 6465 6c01 0300 0000 1a04  adesModel.......
+00002e60: 1404 3004 4204 3000 2004 3e04 4204 3a04  ..0.B.0. .>.B.:.
+00002e70: 4004 4b04 4204 3804 4f08 0000 0000 0600  @.K.B.8.O.......
+00002e80: 0000 094f 7065 6e20 4461 7465 0700 0000  ...Open Date....
+00002e90: 1143 6c6f 7365 6454 7261 6465 734d 6f64  .ClosedTradesMod
+00002ea0: 656c 0103 0000 0026 0414 0430 0442 0430  el.....&...0.B.0
+00002eb0: 002f 0412 0440 0435 043c 044f 0020 043e  ./...@.5.<.O. .>
+00002ec0: 0442 043a 0440 044b 0442 0438 044f 0800  .B.:.@.K.B.8.O..
+00002ed0: 0000 0006 0000 000e 4f70 656e 2044 6174  ........Open Dat
+00002ee0: 652f 5469 6d65 0700 0000 1143 6c6f 7365  e/Time.....Close
+00002ef0: 6454 7261 6465 734d 6f64 656c 0103 0000  dTradesModel....
+00002f00: 001a 0426 0435 043d 0430 0020 043e 0442  ...&.5.=.0. .>.B
+00002f10: 043a 0440 044b 0442 0438 044f 0800 0000  .:.@.K.B.8.O....
+00002f20: 0006 0000 000a 4f70 656e 2050 7269 6365  ......Open Price
+00002f30: 0700 0000 1143 6c6f 7365 6454 7261 6465  .....ClosedTrade
+00002f40: 734d 6f64 656c 0103 0000 0006 041f 0438  sModel.........8
+00002f50: 0423 0800 0000 0006 0000 0003 502f 4c07  .#..........P/L.
+00002f60: 0000 0011 436c 6f73 6564 5472 6164 6573  ....ClosedTrades
+00002f70: 4d6f 6465 6c01 0300 0000 0c04 1f04 3804  Model.........8.
+00002f80: 2300 2c00 2000 2508 0000 0000 0600 0000  #.,. .%.........
+00002f90: 0650 2f4c 2c20 2507 0000 0011 436c 6f73  .P/L, %.....Clos
+00002fa0: 6564 5472 6164 6573 4d6f 6465 6c01 0300  edTradesModel...
+00002fb0: 0000 0c04 1a04 3e04 3b00 2d04 3204 3e08  ......>.;.-.2.>.
+00002fc0: 0000 0000 0600 0000 0351 7479 0700 0000  .........Qty....
+00002fd0: 1143 6c6f 7365 6454 7261 6465 734d 6f64  .ClosedTradesMod
+00002fe0: 656c 0103 0000 00a0 041a 043e 043b 0438  el.........>.;.8
+00002ff0: 0447 0435 0442 0432 043e 0020 0446 0435  .G.5.B.2.>. .F.5
+00003000: 043d 043d 044b 0445 0020 0431 0443 043c  .=.=.K.E. .1.C.<
+00003010: 0430 0433 0020 043d 0435 0434 043e 0441  .0.3. .=.5.4.>.A
+00003020: 0442 0430 0442 043e 0447 043d 043e 0020  .B.0.B.>.G.=.>. 
+00003030: 0434 043b 044f 0020 043e 0431 0440 0430  .4.;.O. .>.1.@.0
+00003040: 0431 043e 0442 043a 0438 0020 043a 043e  .1.>.B.:.8. .:.>
+00003050: 0440 043f 043e 0440 0430 0442 0438 0432  .@.?.>.@.0.B.8.2
+00003060: 043d 043e 0433 043e 0020 0441 043e 0431  .=.>.3.>. .A.>.1
+00003070: 044b 0442 0438 044f 002e 0020 0414 0430  .K.B.8.O... ...0
+00003080: 0442 0430 003a 0020 0800 0000 0006 0000  .B.0.:. ........
+00003090: 0042 4173 7365 7420 616d 6f75 6e74 2069  .BAsset amount i
+000030a0: 7320 6e6f 7420 656e 6f75 6768 2066 6f72  s not enough for
+000030b0: 2063 6f72 706f 7261 7465 2061 6374 696f   corporate actio
+000030c0: 6e20 7072 6f63 6573 7369 6e67 2e20 4461  n processing. Da
+000030d0: 7465 3a20 0700 0000 0f43 6f72 706f 7261  te: .....Corpora
+000030e0: 7465 4163 7469 6f6e 0103 0000 0074 0426  teAction.....t.&
+000030f0: 0411 0020 043d 0435 0020 044f 0432 043b  ... .=.5. .O.2.;
+00003100: 044f 0435 0442 0441 044f 0020 0447 0430  .O.5.B.A.O. .G.0
+00003110: 0441 0442 044c 044e 0020 0440 0435 0437  .A.B.L.N. .@.5.7
+00003120: 0443 043b 044c 0442 0430 0442 043e 0432  .C.;.L.B.0.B.>.2
+00003130: 0020 043a 043e 0440 043f 043e 0440 0430  . .:.>.@.?.>.@.0
+00003140: 0442 0438 0432 043d 043e 0433 043e 0020  .B.8.2.=.>.3.>. 
+00003150: 0441 043e 0431 044b 0442 0438 044f 003a  .A.>.1.K.B.8.O.:
+00003160: 0020 0800 0000 0006 0000 0030 4173 7365  . .........0Asse
+00003170: 7420 6973 6e27 7420 6120 7061 7274 206f  t isn't a part o
+00003180: 6620 636f 7270 6f72 6174 6520 6163 7469  f corporate acti
+00003190: 6f6e 2072 6573 756c 7473 3a20 0700 0000  on results: ....
+000031a0: 0f43 6f72 706f 7261 7465 4163 7469 6f6e  .CorporateAction
+000031b0: 0103 0000 0056 041d 0435 0020 0437 0430  .....V...5. .7.0
+000031c0: 0434 0430 043d 0020 0442 0438 043f 0020  .4.0.=. .B.8.?. 
+000031d0: 043a 043e 0440 043f 043e 0440 0430 0442  .:.>.@.?.>.@.0.B
+000031e0: 0438 0432 043d 043e 0433 043e 0020 0441  .8.2.=.>.3.>. .A
+000031f0: 043e 0431 044b 0442 0438 044f 002e 0020  .>.1.K.B.8.O... 
+00003200: 0414 0430 0442 0430 003a 0020 0800 0000  ...0.B.0.:. ....
+00003210: 0006 0000 002b 436f 7270 6f72 6174 6520  .....+Corporate 
+00003220: 6163 7469 6f6e 2074 7970 6520 6973 6e27  action type isn'
+00003230: 7420 6465 6669 6e65 642e 2044 6174 653a  t defined. Date:
+00003240: 2007 0000 000f 436f 7270 6f72 6174 6541   .....CorporateA
+00003250: 6374 696f 6e01 0300 0000 1204 1404 3504  ction.........5.
+00003260: 3b04 3804 4104 4204 3804 3d04 3308 0000  ;.8.A.B.8.=.3...
+00003270: 0000 0600 0000 0944 656c 6973 7469 6e67  .......Delisting
+00003280: 0700 0000 0f43 6f72 706f 7261 7465 4163  .....CorporateAc
+00003290: 7469 6f6e 0103 0000 002c 0420 0435 043e  tion.....,. .5.>
+000032a0: 0440 0433 0430 043d 0438 0437 0430 0446  .@.3.0.=.8.7.0.F
+000032b0: 0438 044f 0020 043a 043e 043c 043f 0430  .8.O. .:.>.<.?.0
+000032c0: 043d 0438 0438 0800 0000 0006 0000 0006  .=.8.8..........
+000032d0: 4d65 7267 6572 0700 0000 0f43 6f72 706f  Merger.....Corpo
+000032e0: 7261 7465 4163 7469 6f6e 0103 0000 00ac  rateAction......
+000032f0: 0420 0435 0437 0443 043b 044c 0442 0430  . .5.7.C.;.L.B.0
+00003300: 0442 044b 0020 043a 043e 0440 043f 043e  .B.K. .:.>.@.?.>
+00003310: 0440 0430 0442 0438 0432 043d 043e 0433  .@.0.B.8.2.=.>.3
+00003320: 043e 0020 0441 043e 0431 044b 0442 0438  .>. .A.>.1.K.B.8
+00003330: 044f 0020 043d 0435 0020 0440 0430 0441  .O. .=.5. .@.0.A
+00003340: 043f 0440 0435 0434 0435 043b 044f 044e  .?.@.5.4.5.;.O.N
+00003350: 0442 0020 0031 0030 0030 0025 0020 0441  .B. .1.0.0.%. .A
+00003360: 0442 043e 0438 043c 043e 0441 0442 0438  .B.>.8.<.>.A.B.8
+00003370: 0020 0438 0437 043d 0430 0447 0430 043b  . .8.7.=.0.G.0.;
+00003380: 044c 043d 043e 0433 043e 0020 0430 043a  .L.=.>.3.>. .0.:
+00003390: 0442 0438 0432 0430 002e 0020 0800 0000  .B.8.2.0... ....
+000033a0: 0006 0000 004d 5265 7375 6c74 7320 7661  .....MResults va
+000033b0: 6c75 6520 6f66 2063 6f72 706f 7261 7465  lue of corporate
+000033c0: 2061 6374 696f 6e20 646f 6573 6e27 7420   action doesn't 
+000033d0: 6d61 7463 6820 3130 3025 206f 6620 696e  match 100% of in
+000033e0: 6974 6961 6c20 6173 7365 7420 7661 6c75  itial asset valu
+000033f0: 652e 2007 0000 000f 436f 7270 6f72 6174  e. .....Corporat
+00003400: 6541 6374 696f 6e01 0300 0000 3a04 1204  eAction.....:...
+00003410: 4b04 3404 3504 3b04 3504 3d04 3804 3500  K.4.5.;.5.=.8.5.
+00003420: 2004 3a04 3e04 3c04 3f04 3004 3d04 3804   .:.>.<.?.0.=.8.
+00003430: 3800 2000 2804 4104 3f04 3804 3d00 2d04  8. .(.A.?.8.=.-.
+00003440: 3e04 4404 4400 2908 0000 0000 0600 0000  >.D.D.).........
+00003450: 0853 7069 6e2d 6f66 6607 0000 000f 436f  .Spin-off.....Co
+00003460: 7270 6f72 6174 6541 6374 696f 6e01 0300  rporateAction...
+00003470: 0000 0a04 2104 3f04 3b04 3804 4208 0000  ....!.?.;.8.B...
+00003480: 0000 0600 0000 0553 706c 6974 0700 0000  .......Split....
+00003490: 0f43 6f72 706f 7261 7465 4163 7469 6f6e  .CorporateAction
+000034a0: 0103 0000 001a 0421 043c 0435 043d 0430  .......!.<.5.=.0
+000034b0: 0020 0441 0438 043c 0432 043e 043b 0430  . .A.8.<.2.>.;.0
+000034c0: 0800 0000 0006 0000 000d 5379 6d62 6f6c  ..........Symbol
+000034d0: 2063 6861 6e67 6507 0000 000f 436f 7270   change.....Corp
+000034e0: 6f72 6174 6541 6374 696f 6e01 0300 0000  orateAction.....
+000034f0: 1804 1d04 1504 1e04 1f04 2004 1504 1404  .......... .....
+00003500: 1504 1b04 1504 1d04 1e08 0000 0000 0600  ................
+00003510: 0000 0955 4e44 4546 494e 4544 0700 0000  ...UNDEFINED....
+00003520: 0f43 6f72 706f 7261 7465 4163 7469 6f6e  .CorporateAction
+00003530: 0103 0000 00ae 041d 0435 043f 043e 0434  .........5.?.>.4
+00003540: 0435 0440 0436 0438 0432 0430 0435 043c  .5.@.6.8.2.0.5.<
+00003550: 044b 0439 0020 0441 043b 0443 0447 0430  .K.9. .A.;.C.G.0
+00003560: 0439 003a 0020 041a 043e 0440 043f 043e  .9.:. ...>.@.?.>
+00003570: 0440 0430 0442 0438 0432 043d 043e 0435  .@.0.B.8.2.=.>.5
+00003580: 0020 0441 043e 0431 044b 0442 0438 0435  . .A.>.1.K.B.8.5
+00003590: 0020 043f 043e 043a 0440 044b 0432 0430  . .?.>.:.@.K.2.0
+000035a0: 0435 0442 0020 043d 0435 0020 0432 0441  .5.B. .=.5. .2.A
+000035b0: 044e 0020 043e 0442 043a 0440 044b 0442  .N. .>.B.:.@.K.B
+000035c0: 0443 044e 0020 043f 043e 0437 0438 0446  .C.N. .?.>.7.8.F
+000035d0: 0438 044e 002e 0020 0414 0430 0442 0430  .8.N... ...0.B.0
+000035e0: 003a 0020 0800 0000 0006 0000 0046 556e  .:. .........FUn
+000035f0: 6861 6e64 6c65 6420 6361 7365 3a20 436f  handled case: Co
+00003600: 7270 6f72 6174 6520 6163 7469 6f6e 2063  rporate action c
+00003610: 6f76 6572 7320 6e6f 7420 6675 6c6c 206f  overs not full o
+00003620: 7065 6e20 706f 7369 7469 6f6e 2e20 4461  pen position. Da
+00003630: 7465 3a20 0700 0000 0f43 6f72 706f 7261  te: .....Corpora
+00003640: 7465 4163 7469 6f6e 0103 0000 0002 2116  teAction......!.
+00003650: 0800 0000 0006 0000 0001 2307 0000 0015  ..........#.....
+00003660: 436f 7270 6f72 6174 6541 6374 696f 6e57  CorporateActionW
+00003670: 6964 6765 7401 0300 0000 0804 2104 4704  idget.......!.G.
+00003680: 3504 4208 0000 0000 0600 0000 0741 6363  5.B..........Acc
+00003690: 6f75 6e74 0700 0000 1543 6f72 706f 7261  ount.....Corpora
+000036a0: 7465 4163 7469 6f6e 5769 6467 6574 0103  teActionWidget..
+000036b0: 0000 001c 0414 043e 0431 0430 0432 0438  .......>.1.0.2.8
+000036c0: 0442 044c 0020 0430 043a 0442 0438 0432  .B.L. .0.:.B.8.2
+000036d0: 0800 0000 0006 0000 0009 4164 6420 6173  ..........Add as
+000036e0: 7365 7407 0000 0015 436f 7270 6f72 6174  set.....Corporat
+000036f0: 6541 6374 696f 6e57 6964 6765 7401 0300  eActionWidget...
+00003700: 0000 0404 2604 1108 0000 0000 0600 0000  ....&...........
+00003710: 0541 7373 6574 0700 0000 1543 6f72 706f  .Asset.....Corpo
+00003720: 7261 7465 4163 7469 6f6e 5769 6467 6574  rateActionWidget
+00003730: 0103 0000 002c 041a 043e 0440 043f 043e  .....,...>.@.?.>
+00003740: 0440 0430 0442 0438 0432 043d 043e 0435  .@.0.B.8.2.=.>.5
+00003750: 0020 0434 0435 0439 0441 0442 0432 0438  . .4.5.9.A.B.2.8
+00003760: 0435 0800 0000 0006 0000 0010 436f 7270  .5..........Corp
+00003770: 6f72 6174 6520 4163 7469 6f6e 0700 0000  orate Action....
+00003780: 1543 6f72 706f 7261 7465 4163 7469 6f6e  .CorporateAction
+00003790: 5769 6467 6574 0103 0000 0014 0414 0430  Widget.........0
+000037a0: 0442 0430 002f 0412 0440 0435 043c 044f  .B.0./...@.5.<.O
+000037b0: 0800 0000 0006 0000 0009 4461 7465 2f54  ..........Date/T
+000037c0: 696d 6507 0000 0015 436f 7270 6f72 6174  ime.....Corporat
+000037d0: 6541 6374 696f 6e57 6964 6765 7401 0300  eActionWidget...
+000037e0: 0000 1204 1404 3504 3b04 3804 4104 4204  ......5.;.8.A.B.
+000037f0: 3804 3d04 3308 0000 0000 0600 0000 0944  8.=.3..........D
+00003800: 656c 6973 7469 6e67 0700 0000 1543 6f72  elisting.....Cor
+00003810: 706f 7261 7465 4163 7469 6f6e 5769 6467  porateActionWidg
+00003820: 6574 0103 0000 0044 041d 0435 0432 043e  et.....D...5.2.>
+00003830: 0437 043c 043e 0436 043d 043e 0020 0434  .7.<.>.6.=.>. .4
+00003840: 043e 0431 0430 0432 0438 0442 044c 0020  .>.1.0.2.8.B.L. 
+00003850: 043d 043e 0432 0443 044e 0020 0437 0430  .=.>.2.C.N. .7.0
+00003860: 043f 0438 0441 044c 003a 0020 0800 0000  .?.8.A.L.:. ....
+00003870: 0006 0000 001a 4661 696c 6564 2074 6f20  ......Failed to 
+00003880: 6164 6420 6e65 7720 7265 636f 7264 3a20  add new record: 
+00003890: 0700 0000 1543 6f72 706f 7261 7465 4163  .....CorporateAc
+000038a0: 7469 6f6e 5769 6467 6574 0103 0000 0028  tionWidget.....(
+000038b0: 041e 0431 044a 0435 0434 0438 043d 0435  ...1.J.5.4.8.=.5
+000038c0: 043d 0438 0435 0020 043a 043e 043c 043f  .=.8.5. .:.>.<.?
+000038d0: 0430 043d 0438 0438 0800 0000 0006 0000  .0.=.8.8........
+000038e0: 0006 4d65 7267 6572 0700 0000 1543 6f72  ..Merger.....Cor
+000038f0: 706f 7261 7465 4163 7469 6f6e 5769 6467  porateActionWidg
+00003900: 6574 0103 0000 0006 004e 002f 0041 0800  et.......N./.A..
+00003910: 0000 0006 0000 0003 4e2f 4107 0000 0015  ........N/A.....
+00003920: 436f 7270 6f72 6174 6541 6374 696f 6e57  CorporateActionW
+00003930: 6964 6765 7401 0300 0000 1004 1e04 3f04  idget.........?.
+00003940: 3804 4104 3004 3d04 3804 3508 0000 0000  8.A.0.=.8.5.....
+00003950: 0600 0000 044e 6f74 6507 0000 0015 436f  .....Note.....Co
+00003960: 7270 6f72 6174 6541 6374 696f 6e57 6964  rporateActionWid
+00003970: 6765 7401 0300 0000 4804 1e04 4804 3804  get.....H...H.8.
+00003980: 3104 3a04 3000 2004 3f04 4004 3800 2004  1.:.0. .?.@.8. .
+00003990: 3704 3004 3f04 3804 4104 3800 2004 3404  7.0.?.8.A.8. .4.
+000039a0: 3504 4204 3004 3b04 3504 3900 2004 3e04  5.B.0.;.5.9. .>.
+000039b0: 3f04 3504 4004 3004 4604 3804 3800 3a00  ?.5.@.0.F.8.8.:.
+000039c0: 2008 0000 0000 0600 0000 214f 7065 7261   .........!Opera
+000039d0: 7469 6f6e 2064 6574 6169 6c73 2073 7562  tion details sub
+000039e0: 6d69 7420 6661 696c 6564 3a20 0700 0000  mit failed: ....
+000039f0: 1543 6f72 706f 7261 7465 4163 7469 6f6e  .CorporateAction
+00003a00: 5769 6467 6574 0103 0000 0038 041e 0448  Widget.....8...H
+00003a10: 0438 0431 043a 0430 0020 043f 0440 0438  .8.1.:.0. .?.@.8
+00003a20: 0020 0437 0430 043f 0438 0441 0438 0020  . .7.0.?.8.A.8. 
+00003a30: 043e 043f 0435 0440 0430 0446 0438 0438  .>.?.5.@.0.F.8.8
+00003a40: 003a 0020 0800 0000 0006 0000 0019 4f70  .:. ..........Op
+00003a50: 6572 6174 696f 6e20 7375 626d 6974 2066  eration submit f
+00003a60: 6169 6c65 643a 2007 0000 0015 436f 7270  ailed: .....Corp
+00003a70: 6f72 6174 6541 6374 696f 6e57 6964 6765  orateActionWidge
+00003a80: 7401 0300 0000 0c04 1a04 3e04 3b00 2d04  t.........>.;.-.
+00003a90: 3204 3e08 0000 0000 0600 0000 0351 7479  2.>..........Qty
+00003aa0: 0700 0000 1543 6f72 706f 7261 7465 4163  .....CorporateAc
+00003ab0: 7469 6f6e 5769 6467 6574 0103 0000 001a  tionWidget......
+00003ac0: 0423 0434 0430 043b 0438 0442 044c 0020  .#.4.0.;.8.B.L. 
+00003ad0: 0430 043a 0442 0438 0432 0800 0000 0006  .0.:.B.8.2......
+00003ae0: 0000 000c 5265 6d6f 7665 2061 7373 6574  ....Remove asset
+00003af0: 0700 0000 1543 6f72 706f 7261 7465 4163  .....CorporateAc
+00003b00: 7469 6f6e 5769 6467 6574 0103 ffff ffff  tionWidget......
+00003b10: 0800 0000 0006 0000 0008 5370 696e 2d4f  ..........Spin-O
+00003b20: 6666 0700 0000 1543 6f72 706f 7261 7465  ff.....Corporate
+00003b30: 4163 7469 6f6e 5769 6467 6574 0103 0000  ActionWidget....
+00003b40: 000a 0421 043f 043b 0438 0442 0800 0000  ...!.?.;.8.B....
+00003b50: 0006 0000 0005 5370 6c69 7407 0000 0015  ......Split.....
+00003b60: 436f 7270 6f72 6174 6541 6374 696f 6e57  CorporateActionW
+00003b70: 6964 6765 7401 0300 0000 1a04 2104 3c04  idget.......!.<.
+00003b80: 3504 3d04 3000 2004 4104 3804 3c04 3204  5.=.0. .A.8.<.2.
+00003b90: 3e04 3b04 3008 0000 0000 0600 0000 0d53  >.;.0..........S
+00003ba0: 796d 626f 6c20 6368 616e 6765 0700 0000  ymbol change....
+00003bb0: 1543 6f72 706f 7261 7465 4163 7469 6f6e  .CorporateAction
+00003bc0: 5769 6467 6574 0103 0000 0006 0422 0438  Widget.......".8
+00003bd0: 043f 0800 0000 0006 0000 0004 5479 7065  .?..........Type
+00003be0: 0700 0000 1543 6f72 706f 7261 7465 4163  .....CorporateAc
+00003bf0: 7469 6f6e 5769 6467 6574 0103 0000 0034  tionWidget.....4
+00003c00: 0424 043e 0440 043c 0430 0442 0020 0431  .$.>.@.<.0.B. .1
+00003c10: 0430 0437 044b 0020 0434 0430 043d 043d  .0.7.K. .4.0.=.=
+00003c20: 044b 0445 0020 0443 0441 0442 0430 0440  .K.E. .C.A.B.0.@
+00003c30: 0435 043b 0800 0000 0006 0000 001b 4461  .5.;..........Da
+00003c40: 7461 6261 7365 2066 6f72 6d61 7420 6973  tabase format is
+00003c50: 206f 7574 6461 7465 6407 0000 0002 4442   outdated.....DB
+00003c60: 0103 0000 0064 0412 044b 0020 0441 043e  .....d...K. .A.>
+00003c70: 0433 043b 0430 0441 043d 044b 0020 0441  .3.;.0.A.=.K. .A
+00003c80: 043a 043e 043d 0432 0435 0440 0442 0438  .:.>.=.2.5.@.B.8
+00003c90: 0440 043e 0432 0430 0442 044c 0020 0434  .@.>.2.0.B.L. .4
+00003ca0: 0430 043d 043d 044b 0435 0020 0432 0020  .0.=.=.K.5. .2. 
+00003cb0: 043d 043e 0432 044b 0439 0020 0444 043e  .=.>.2.K.9. .D.>
+00003cc0: 0440 043c 0430 0442 003f 0800 0000 0006  .@.<.0.B.?......
+00003cd0: 0000 0032 446f 2079 6f75 2061 6772 6565  ...2Do you agree
+00003ce0: 2074 6f20 7570 6772 6164 6520 796f 7572   to upgrade your
+00003cf0: 2064 6174 6120 746f 206e 6577 6572 2066   data to newer f
+00003d00: 6f72 6d61 743f 0700 0000 0244 4201 0300  ormat?.....DB...
+00003d10: 0000 5e04 2404 3e04 4004 3c04 3000 2000  ..^.$.>.@.<.0. .
+00003d20: 3300 2d04 1d04 1404 2404 1b00 2004 3404  3.-.....$... .4.
+00003d30: 3b04 4f00 2004 4d04 4204 3e04 3304 3e00  ;.O. .M.B.>.3.>.
+00003d40: 2004 3304 3e04 3404 3000 2004 3d04 3500   .3.>.4.0. .=.5.
+00003d50: 2004 3f04 3e04 3404 3404 3504 4004 3604   .?.>.4.4.5.@.6.
+00003d60: 3804 3204 3004 3504 4204 4104 4f00 3a00  8.2.0.5.B.A.O.:.
+00003d70: 2008 0000 0000 0600 0000 2633 2d4e 4446   .........&3-NDF
+00003d80: 4c20 666f 726d 2069 736e 2774 2073 7570  L form isn't sup
+00003d90: 6f6f 7274 6564 2066 6f72 2079 6561 723a  oorted for year:
+00003da0: 2007 0000 0004 444c 5347 0103 0000 0086   .....DLSG......
+00003db0: 0421 0442 0440 0430 043d 0430 0020 0426  .!.B.@.0.=.0. .&
+00003dc0: 0411 0020 043d 0435 0020 0437 0430 0434  ... .=.5. .7.0.4
+00003dd0: 0430 043d 0430 002c 0020 0434 0438 0432  .0.=.0.,. .4.8.2
+00003de0: 0438 0434 0435 043d 0434 0020 043d 0435  .8.4.5.=.4. .=.5
+00003df0: 0020 0431 0443 0434 0435 0442 0020 0432  . .1.C.4.5.B. .2
+00003e00: 043a 043b 044e 0447 0451 043d 0020 0432  .:.;.N.G.Q.=. .2
+00003e10: 0020 0434 0435 043a 043b 0430 0440 0430  . .4.5.:.;.0.@.0
+00003e20: 0446 0438 044e 0020 0033 002d 041d 0424  .F.8.N. .3.-...$
+00003e30: 0414 041b 0020 0800 0000 0006 0000 0047  ..... .........G
+00003e40: 4163 636f 756e 7420 636f 756e 7472 7920  Account country 
+00003e50: 6973 206e 6f74 2073 6574 2066 6f72 2061  is not set for a
+00003e60: 7373 6574 2c20 6469 7669 6465 6e64 2069  sset, dividend i
+00003e70: 736e 2774 2069 6e63 6c75 6465 2069 6e20  sn't include in 
+00003e80: 332d 4e44 464c 2007 0000 0004 444c 5347  3-NDFL .....DLSG
+00003e90: 0103 0000 004a 0412 0430 043b 044e 0442  .....J...0.;.N.B
+00003ea0: 0430 0020 043d 0435 0020 043f 043e 0434  .0. .=.5. .?.>.4
+00003eb0: 0434 0435 0440 0436 0438 0432 0430 0435  .4.5.@.6.8.2.0.5
+00003ec0: 0442 0441 044f 0020 0434 043b 044f 0020  .B.A.O. .4.;.O. 
+00003ed0: 0033 002d 041d 0414 0424 041b 003a 0020  .3.-.....$...:. 
+00003ee0: 0800 0000 0006 0000 0026 4375 7272 656e  .........&Curren
+00003ef0: 6379 2069 7320 6e6f 7420 7375 7070 6f72  cy is not suppor
+00003f00: 7465 6420 666f 7220 332d 4e44 464c 3a20  ted for 3-NDFL: 
+00003f10: 0700 0000 0444 4c53 4701 0300 0000 1404  .....DLSG.......
+00003f20: 4d04 3a04 4104 3f04 3804 4004 3004 4604  M.:.A.?.8.@.0.F.
+00003f30: 3804 4f08 0000 0000 0600 0000 0665 7870  8.O..........exp
+00003f40: 6972 7907 0000 000c 4461 7461 4465 6c65  iry.....DataDele
+00003f50: 6761 7465 0103 0000 000e 043d 043e 043c  gate.......=.>.<
+00003f60: 0438 043d 0430 043b 0800 0000 0006 0000  .8.=.0.;........
+00003f70: 0009 7072 696e 6369 7061 6c07 0000 000c  ..principal.....
+00003f80: 4461 7461 4465 6c65 6761 7465 0103 0000  DataDelegate....
+00003f90: 000e 0440 0435 0433 002e 043a 043e 0434  ...@.5.3...:.>.4
+00003fa0: 0800 0000 0006 0000 0008 7265 672e 636f  ..........reg.co
+00003fb0: 6465 0700 0000 0c44 6174 6144 656c 6567  de.....DataDeleg
+00003fc0: 6174 6501 0300 0000 1004 1204 4104 3500  ate.........A.5.
+00003fd0: 2004 3404 3004 4204 4b08 0000 0000 0600   .4.0.B.K.......
+00003fe0: 0000 0941 6c6c 2064 6174 6573 0700 0000  ...All dates....
+00003ff0: 1144 6174 6552 616e 6765 5365 6c65 6374  .DateRangeSelect
+00004000: 6f72 0103 0000 0004 0421 003a 0800 0000  or.......!.:....
+00004010: 0006 0000 0005 4672 6f6d 3a07 0000 0011  ......From:.....
+00004020: 4461 7465 5261 6e67 6553 656c 6563 746f  DateRangeSelecto
+00004030: 7201 0300 0000 0a04 1c04 3504 4104 4f04  r.........5.A.O.
+00004040: 4608 0000 0000 0600 0000 054d 6f6e 7468  F..........Month
+00004050: 0700 0000 1144 6174 6552 616e 6765 5365  .....DateRangeSe
+00004060: 6c65 6374 6f72 0103 0000 001c 041f 0440  lector.........@
+00004070: 0435 0434 044b 0434 0443 0449 0438 0439  .5.4.K.4.C.I.8.9
+00004080: 0020 0433 043e 0434 0800 0000 0006 0000  . .3.>.4........
+00004090: 000d 5072 6576 696f 7573 2079 6561 7207  ..Previous year.
+000040a0: 0000 0011 4461 7465 5261 6e67 6553 656c  ....DateRangeSel
+000040b0: 6563 746f 7201 0300 0000 0e04 1a04 3204  ector.........2.
+000040c0: 3004 4004 4204 3004 3b08 0000 0000 0600  0.@.B.0.;.......
+000040d0: 0000 0751 7561 7274 6572 0700 0000 1144  ...Quarter.....D
+000040e0: 6174 6552 616e 6765 5365 6c65 6374 6f72  ateRangeSelector
+000040f0: 0103 0000 0024 0422 0435 043a 0443 0449  .....$.".5.:.C.I
+00004100: 0438 0439 0020 0434 043e 0020 0441 0435  .8.9. .4.>. .A.5
+00004110: 0433 043e 0434 043d 044f 0800 0000 0006  .3.>.4.=.O......
+00004120: 0000 000f 5175 6172 7465 7220 746f 2064  ....Quarter to d
+00004130: 6174 6507 0000 0011 4461 7465 5261 6e67  ate.....DateRang
+00004140: 6553 656c 6563 746f 7201 0300 0000 1604  eSelector.......
+00004150: 2204 3504 3a04 4304 4904 3804 3900 2004  ".5.:.C.I.8.9. .
+00004160: 3304 3e04 3408 0000 0000 0600 0000 0954  3.>.4..........T
+00004170: 6869 7320 7965 6172 0700 0000 1144 6174  his year.....Dat
+00004180: 6552 616e 6765 5365 6c65 6374 6f72 0103  eRangeSelector..
+00004190: 0000 0006 0414 043e 003a 0800 0000 0006  .......>.:......
+000041a0: 0000 0003 546f 3a07 0000 0011 4461 7465  ....To:.....Date
+000041b0: 5261 6e67 6553 656c 6563 746f 7201 0300  RangeSelector...
+000041c0: 0000 0c04 1d04 3504 3404 3504 3b04 4f08  ......5.4.5.;.O.
+000041d0: 0000 0000 0600 0000 0457 6565 6b07 0000  .........Week...
+000041e0: 0011 4461 7465 5261 6e67 6553 656c 6563  ..DateRangeSelec
+000041f0: 746f 7201 0300 0000 0604 1304 3e04 3408  tor.........>.4.
+00004200: 0000 0000 0600 0000 0459 6561 7207 0000  .........Year...
+00004210: 0011 4461 7465 5261 6e67 6553 656c 6563  ..DateRangeSelec
+00004220: 746f 7201 0300 0000 1c04 1304 3e04 3400  tor.........>.4.
+00004230: 2004 3404 3e00 2004 4104 3504 3304 3e04   .4.>. .A.5.3.>.
+00004240: 3404 3d04 4f08 0000 0000 0600 0000 0c59  4.=.O..........Y
+00004250: 6561 7220 746f 2064 6174 6507 0000 0011  ear to date.....
+00004260: 4461 7465 5261 6e67 6553 656c 6563 746f  DateRangeSelecto
+00004270: 7201 0300 0000 1e04 2104 3404 3504 3b04  r.......!.4.5.;.
+00004280: 3a04 3800 2004 3f04 3e00 2004 4104 4704  :.8. .?.>. .A.G.
+00004290: 3504 4204 4308 0000 0000 0600 0000 1044  5.B.C..........D
+000042a0: 6561 6c73 2062 7920 4163 636f 756e 7407  eals by Account.
+000042b0: 0000 000b 4465 616c 7352 6570 6f72 7401  ....DealsReport.
+000042c0: 0300 0000 0a04 2104 4704 3504 4200 3a08  ......!.G.5.B.:.
+000042d0: 0000 0000 0600 0000 0841 6363 6f75 6e74  .........Account
+000042e0: 3a07 0000 0011 4465 616c 7352 6570 6f72  :.....DealsRepor
+000042f0: 7457 6964 6765 7401 0300 0000 0c04 2104  tWidget.......!.
+00004300: 3404 3504 3b04 3a04 3808 0000 0000 0600  4.5.;.:.8.......
+00004310: 0000 0544 6561 6c73 0700 0000 1144 6561  ...Deals.....Dea
+00004320: 6c73 5265 706f 7274 5769 6467 6574 0103  lsReportWidget..
+00004330: 0000 0020 0413 0440 0443 043f 043f 0438  ... ...@.C.?.?.8
+00004340: 0440 043e 0432 0430 0442 044c 0020 043f  .@.>.2.0.B.L. .?
+00004350: 043e 003a 0800 0000 0006 0000 0009 4772  .>.:..........Gr
+00004360: 6f75 7020 6279 3a07 0000 0011 4465 616c  oup by:.....Deal
+00004370: 7352 6570 6f72 7457 6964 6765 7401 0300  sReportWidget...
+00004380: 0000 0e00 3c04 1f04 4304 4104 4204 3e00  ....<...C.A.B.>.
+00004390: 3e08 0000 0000 0600 0000 063c 4e6f 6e65  >..........<None
+000043a0: 3e07 0000 0011 4465 616c 7352 6570 6f72  >.....DealsRepor
+000043b0: 7457 696e 646f 7701 0300 0000 1a04 2604  tWindow.......&.
+000043c0: 3504 3d04 3d04 3004 4f00 2004 3104 4304  5.=.=.0.O. .1.C.
+000043d0: 3c04 3004 3304 3008 0000 0000 0600 0000  <.0.3.0.........
+000043e0: 0541 7373 6574 0700 0000 1144 6561 6c73  .Asset.....Deals
+000043f0: 5265 706f 7274 5769 6e64 6f77 0103 0000  ReportWindow....
+00004400: 0030 0426 0411 0020 002d 0020 041e 0442  .0.&... .-. ...B
+00004410: 043a 0440 044b 0442 0438 0435 0020 002d  .:.@.K.B.8.5. .-
+00004420: 0020 0417 0430 043a 0440 044b 0442 0438  . ...0.:.@.K.B.8
+00004430: 0435 0800 0000 0006 0000 0014 4173 7365  .5..........Asse
+00004440: 7420 2d20 4f70 656e 202d 2043 6c6f 7365  t - Open - Close
+00004450: 0700 0000 1144 6561 6c73 5265 706f 7274  .....DealsReport
+00004460: 5769 6e64 6f77 0103 0000 0010 0417 0430  Window.........0
+00004470: 043a 0440 044b 0442 0438 0435 0800 0000  .:.@.K.B.8.5....
+00004480: 0006 0000 0005 436c 6f73 6507 0000 0011  ......Close.....
+00004490: 4465 616c 7352 6570 6f72 7457 696e 646f  DealsReportWindo
+000044a0: 7701 0300 0000 2604 1704 3004 3a04 4004  w.....&...0.:.@.
+000044b0: 4b04 4204 3804 3500 2000 2d00 2004 1e04  K.B.8.5. .-. ...
+000044c0: 4204 3a04 4004 4b04 4204 3804 3508 0000  B.:.@.K.B.8.5...
+000044d0: 0000 0600 0000 0c43 6c6f 7365 202d 204f  .......Close - O
+000044e0: 7065 6e07 0000 0011 4465 616c 7352 6570  pen.....DealsRep
+000044f0: 6f72 7457 696e 646f 7701 0300 0000 2604  ortWindow.....&.
+00004500: 1e04 4204 3a04 4004 4b04 4204 3804 3500  ..B.:.@.K.B.8.5.
+00004510: 2000 2d00 2004 1704 3004 3a04 4004 4b04   .-. ...0.:.@.K.
+00004520: 4204 3804 3508 0000 0000 0600 0000 0c4f  B.8.5..........O
+00004530: 7065 6e20 2d20 436c 6f73 6507 0000 0011  pen - Close.....
+00004540: 4465 616c 7352 6570 6f72 7457 696e 646f  DealsReportWindo
+00004550: 7701 0300 0000 0a04 2104 4304 3c04 3c04  w.......!.C.<.<.
+00004560: 3008 0000 0000 0600 0000 0641 6d6f 756e  0..........Amoun
+00004570: 7407 0000 000c 4465 7461 696c 734d 6f64  t.....DetailsMod
+00004580: 656c 0103 0000 0012 041a 0430 0442 0435  el.........0.B.5
+00004590: 0433 043e 0440 0438 044f 0800 0000 0006  .3.>.@.8.O......
+000045a0: 0000 0008 4361 7465 676f 7279 0700 0000  ....Category....
+000045b0: 0c44 6574 6169 6c73 4d6f 6465 6c01 0300  .DetailsModel...
+000045c0: 0000 1004 1e04 3f04 3804 4104 3004 3d04  ......?.8.A.0.=.
+000045d0: 3804 3508 0000 0000 0600 0000 044e 6f74  8.5..........Not
+000045e0: 6507 0000 000c 4465 7461 696c 734d 6f64  e.....DetailsMod
+000045f0: 656c 0103 0000 000a 041c 0435 0442 043a  el.........5.B.:
+00004600: 0430 0800 0000 0006 0000 0003 5461 6707  .0..........Tag.
+00004610: 0000 000c 4465 7461 696c 734d 6f64 656c  ....DetailsModel
+00004620: 0103 0000 009e 041d 0435 0432 043e 0437  .........5.2.>.7
+00004630: 043c 043e 0436 043d 043e 0020 043e 0431  .<.>.6.=.>. .>.1
+00004640: 0440 0430 0431 043e 0442 0430 0442 044c  .@.0.1.>.B.0.B.L
+00004650: 0020 0434 0438 0432 0438 0434 0435 043d  . .4.8.2.8.4.5.=
+00004660: 0434 002c 0020 0442 002e 043a 002e 0020  .4.,. .B...:... 
+00004670: 043d 0435 0020 0443 043a 0430 0437 0430  .=.5. .C.:.0.7.0
+00004680: 043d 0020 0431 0430 043d 043a 0020 0434  .=. .1.0.=.:. .4
+00004690: 043b 044f 0020 0438 043d 0432 0435 0441  .;.O. .8.=.2.5.A
+000046a0: 0442 0438 0446 0438 043e 043d 043d 043e  .B.8.F.8.>.=.=.>
+000046b0: 0433 043e 0020 0441 0447 0451 0442 0430  .3.>. .A.G.Q.B.0
+000046c0: 003a 0020 0800 0000 0006 0000 0041 4361  .:. .........ACa
+000046d0: 6e27 7420 7072 6f63 6573 7320 6469 7669  n't process divi
+000046e0: 6465 6e64 2061 7320 6261 6e6b 2069 736e  dend as bank isn
+000046f0: 2774 2073 6574 2066 6f72 2069 6e76 6573  't set for inves
+00004700: 746d 656e 7420 6163 636f 756e 743a 2007  tment account: .
+00004710: 0000 0008 4469 7669 6465 6e64 0103 0000  ....Dividend....
+00004720: 005a 041d 0435 0020 0437 0430 0434 0430  .Z...5. .7.0.4.0
+00004730: 043d 0430 0020 0446 0435 043d 0430 0020  .=.0. .F.5.=.0. 
+00004740: 0434 043b 044f 0020 0432 044b 043f 043b  .4.;.O. .2.K.?.;
+00004750: 0430 0442 044b 0020 0446 0435 043d 043d  .0.B.K. .F.5.=.=
+00004760: 044b 043c 0438 0020 0431 0443 043c 0430  .K.<.8. .1.C.<.0
+00004770: 0433 0430 043c 0438 003a 0020 0800 0000  .3.0.<.8.:. ....
+00004780: 0006 0000 002a 4e6f 2070 7269 6365 2064  .....*No price d
+00004790: 6174 6120 666f 7220 7374 6f63 6b20 6469  ata for stock di
+000047a0: 7669 6465 6e64 2f76 6573 7469 6e67 3a20  vidend/vesting: 
+000047b0: 0700 0000 0844 6976 6964 656e 6401 0300  .....Dividend...
+000047c0: 0000 7204 1d04 3504 4200 2004 3a04 3e04  ..r...5.B. .:.>.
+000047d0: 4204 3804 4004 3e04 3204 3a04 3800 2004  B.8.@.>.2.:.8. .
+000047e0: 3404 3b04 4f00 2004 3404 3804 3204 3804  4.;.O. .4.8.2.8.
+000047f0: 3404 3504 3d04 3404 3000 2004 3004 3a04  4.5.=.4.0. .0.:.
+00004800: 4604 3804 4f04 3c04 3800 2004 3804 3b04  F.8.O.<.8. .8.;.
+00004810: 3800 2004 3704 3004 4704 3804 4104 3b04  8. .7.0.G.8.A.;.
+00004820: 3504 3d04 3804 4f00 2004 3004 3a04 4604  5.=.8.O. .0.:.F.
+00004830: 3804 3900 2e08 0000 0000 0600 0000 2d4e  8.9...........-N
+00004840: 6f20 7374 6f63 6b20 7175 6f74 6520 666f  o stock quote fo
+00004850: 7220 7374 6f63 6b20 6469 7669 6465 6e64  r stock dividend
+00004860: 206f 7220 7665 7374 696e 672e 0700 0000   or vesting.....
+00004870: 0844 6976 6964 656e 6401 0300 0000 b804  .Dividend.......
+00004880: 1d04 3504 3f04 3e04 3404 3404 3504 4004  ..5.?.>.4.4.5.@.
+00004890: 3604 3804 3204 3004 3504 3c04 3e04 3500  6.8.2.0.5.<.>.5.
+000048a0: 2004 3404 3504 3904 4104 4204 3204 3804   .4.5.9.A.B.2.8.
+000048b0: 3500 3a00 2004 3404 3804 3204 3804 3404  5.:. .4.8.2.8.4.
+000048c0: 3504 3d04 3400 2004 3004 3a04 4604 3804  5.=.4. .0.:.F.8.
+000048d0: 4f04 3c04 3800 2004 3804 3b04 3800 2004  O.<.8. .8.;.8. .
+000048e0: 3704 3004 4704 3804 4104 3b04 3504 3d04  7.0.G.8.A.;.5.=.
+000048f0: 3804 3500 2004 3004 3a04 4604 3804 3900  8.5. .0.:.F.8.9.
+00004900: 2004 3704 3004 3a04 4004 4b04 3204 3004   .7.0.:.@.K.2.0.
+00004910: 3504 4200 2004 3a04 3e04 4004 3e04 4204  5.B. .:.>.@.>.B.
+00004920: 3a04 4304 4e00 2004 3f04 3e04 3704 3804  :.C.N. .?.>.7.8.
+00004930: 4604 3804 4e00 2e08 0000 0000 0600 0000  F.8.N...........
+00004940: 434e 6f74 2073 7570 706f 7274 6564 2061  CNot supported a
+00004950: 6374 696f 6e3a 2073 746f 636b 2064 6976  ction: stock div
+00004960: 6964 656e 6420 6f72 2076 6573 7469 6e67  idend or vesting
+00004970: 2063 6c6f 7365 7320 7368 6f72 7420 7472   closes short tr
+00004980: 6164 652e 0700 0000 0844 6976 6964 656e  ade......Dividen
+00004990: 6401 0300 0000 0e04 1d04 3004 3b04 3e04  d.........0.;.>.
+000049a0: 3300 3a00 2008 0000 0000 0600 0000 0554  3.:. ..........T
+000049b0: 6178 3a20 0700 0000 0844 6976 6964 656e  ax: .....Dividen
+000049c0: 6401 0300 0000 3e04 1d04 3504 3f04 3e04  d.....>...5.?.>.
+000049d0: 3404 3404 3504 4004 3604 3804 3204 3004  4.4.5.@.6.8.2.0.
+000049e0: 3504 3c04 4b04 3900 2004 4204 3804 3f00  5.<.K.9. .B.8.?.
+000049f0: 2004 3404 3804 3204 3804 3404 3504 3d04   .4.8.2.8.4.5.=.
+00004a00: 3404 3000 2e08 0000 0000 0600 0000 1a55  4.0............U
+00004a10: 6e73 7570 706f 7274 6564 2064 6976 6964  nsupported divid
+00004a20: 656e 6420 7479 7065 2e07 0000 0008 4469  end type......Di
+00004a30: 7669 6465 6e64 0103 0000 0002 2116 0800  vidend......!...
+00004a40: 0000 0006 0000 0001 2307 0000 000e 4469  ........#.....Di
+00004a50: 7669 6465 6e64 5769 6467 6574 0103 0000  videndWidget....
+00004a60: 0008 0421 0447 0435 0442 0800 0000 0006  ...!.G.5.B......
+00004a70: 0000 0007 4163 636f 756e 7407 0000 000e  ....Account.....
+00004a80: 4469 7669 6465 6e64 5769 6467 6574 0103  DividendWidget..
+00004a90: 0000 0004 0426 0411 0800 0000 0006 0000  .....&..........
+00004aa0: 0005 4173 7365 7407 0000 000e 4469 7669  ..Asset.....Divi
+00004ab0: 6465 6e64 5769 6467 6574 0103 0000 000a  dendWidget......
+00004ac0: 041a 0443 043f 043e 043d 0800 0000 0006  ...C.?.>.=......
+00004ad0: 0000 000d 426f 6e64 2049 6e74 6572 6573  ....Bond Interes
+00004ae0: 7407 0000 000e 4469 7669 6465 6e64 5769  t.....DividendWi
+00004af0: 6467 6574 0103 0000 0014 0414 0430 0442  dget.........0.B
+00004b00: 0430 002f 0412 0440 0435 043c 044f 0800  .0./...@.5.<.O..
+00004b10: 0000 0006 0000 0009 4461 7465 2f54 696d  ........Date/Tim
+00004b20: 6507 0000 000e 4469 7669 6465 6e64 5769  e.....DividendWi
+00004b30: 6467 6574 0103 0000 0010 0414 0438 0432  dget.........8.2
+00004b40: 0438 0434 0435 043d 0434 0800 0000 0006  .8.4.5.=.4......
+00004b50: 0000 0008 4469 7669 6465 6e64 0700 0000  ....Dividend....
+00004b60: 0e44 6976 6964 656e 6457 6964 6765 7401  .DividendWidget.
+00004b70: 0300 0000 0e04 1e04 4204 4104 3504 4704  ........B.A.5.G.
+00004b80: 3a04 3008 0000 0000 0600 0000 0745 782d  :.0..........Ex-
+00004b90: 4461 7465 0700 0000 0e44 6976 6964 656e  Date.....Dividen
+00004ba0: 6457 6964 6765 7401 0300 0000 0600 4e00  dWidget.......N.
+00004bb0: 2f00 4108 0000 0000 0600 0000 034e 2f41  /.A..........N/A
+00004bc0: 0700 0000 0e44 6976 6964 656e 6457 6964  .....DividendWid
+00004bd0: 6765 7401 0300 0000 1a04 1d04 3504 4200  get.........5.B.
+00004be0: 2004 3a04 3e04 4204 3804 4004 3e04 3204   .:.>.B.8.@.>.2.
+00004bf0: 3a04 3808 0000 0000 0600 0000 084e 6f20  :.8..........No 
+00004c00: 7175 6f74 6507 0000 000e 4469 7669 6465  quote.....Divide
+00004c10: 6e64 5769 6467 6574 0103 0000 0010 041e  ndWidget........
+00004c20: 043f 0438 0441 0430 043d 0438 0435 0800  .?.8.A.0.=.8.5..
+00004c30: 0000 0006 0000 0004 4e6f 7465 0700 0000  ........Note....
+00004c40: 0e44 6976 6964 656e 6457 6964 6765 7401  .DividendWidget.
+00004c50: 0300 0000 0804 2604 3504 3d04 3008 0000  ......&.5.=.0...
+00004c60: 0000 0600 0000 0550 7269 6365 0700 0000  .......Price....
+00004c70: 0e44 6976 6964 656e 6457 6964 6765 7401  .DividendWidget.
+00004c80: 0300 0000 2004 1404 3804 3204 3804 3404  .... ...8.2.8.4.
+00004c90: 3504 3d04 3400 2004 3004 3a04 4604 3804  5.=.4. .0.:.F.8.
+00004ca0: 4f04 3c04 3808 0000 0000 0600 0000 0e53  O.<.8..........S
+00004cb0: 746f 636b 2044 6976 6964 656e 6407 0000  tock Dividend...
+00004cc0: 000e 4469 7669 6465 6e64 5769 6467 6574  ..DividendWidget
+00004cd0: 0103 0000 001c 041f 0435 0440 0435 0434  .........5.@.5.4
+00004ce0: 0430 0447 0430 0020 0430 043a 0446 0438  .0.G.0. .0.:.F.8
+00004cf0: 0439 0800 0000 0006 0000 000d 5374 6f63  .9..........Stoc
+00004d00: 6b20 5665 7374 696e 6707 0000 000e 4469  k Vesting.....Di
+00004d10: 7669 6465 6e64 5769 6467 6574 0103 0000  videndWidget....
+00004d20: 000a 041d 0430 043b 043e 0433 0800 0000  .....0.;.>.3....
+00004d30: 0006 0000 0003 5461 7807 0000 000e 4469  ......Tax.....Di
+00004d40: 7669 6465 6e64 5769 6467 6574 0103 0000  videndWidget....
+00004d50: 0006 0422 0438 043f 0800 0000 0006 0000  ...".8.?........
+00004d60: 0004 5479 7065 0700 0000 0e44 6976 6964  ..Type.....Divid
+00004d70: 656e 6457 6964 6765 7401 0300 0000 b204  endWidget.......
+00004d80: 1d04 4304 3604 3d04 3e00 2004 4304 4104  ..C.6.=.>. .C.A.
+00004d90: 4204 3004 3d04 3e04 3204 3804 4204 4c00  B.0.=.>.2.8.B.L.
+00004da0: 2004 3a04 3e04 4204 3804 4004 3e04 3204   .:.>.B.8.@.>.2.
+00004db0: 3a04 4300 2004 3104 4304 3c04 3004 3304  :.C. .1.C.<.0.3.
+00004dc0: 3800 2004 3404 3b04 4f00 2004 1404 3004  8. .4.;.O. ...0.
+00004dd0: 4204 4b00 2f04 1204 4004 3504 3c04 3504  B.K./...@.5.<.5.
+00004de0: 3d04 3800 2004 3404 3804 3204 3804 3404  =.8. .4.8.2.8.4.
+00004df0: 3504 3d04 3404 3000 2004 4704 3504 4004  5.=.4.0. .G.5.@.
+00004e00: 3504 3700 2004 3c04 3504 3d04 4e00 2004  5.7. .<.5.=.N. .
+00004e10: 1404 3004 3d04 3d04 4b04 3500 2d00 3e04  ..0.=.=.K.5.-.>.
+00004e20: 1a04 3e04 4204 3804 4004 3e04 3204 3a04  ..>.B.8.@.>.2.:.
+00004e30: 3808 0000 0000 0600 0000 4859 6f75 2073  8.........HYou s
+00004e40: 686f 756c 6420 7365 7420 7175 6f74 6520  hould set quote 
+00004e50: 7669 6120 4461 7461 2d3e 5175 6f74 6573  via Data->Quotes
+00004e60: 206d 656e 7520 666f 7220 4461 7465 2f54   menu for Date/T
+00004e70: 696d 6520 6f66 2074 6865 2064 6976 6964  ime of the divid
+00004e80: 656e 6407 0000 000e 4469 7669 6465 6e64  end.....Dividend
+00004e90: 5769 6467 6574 0103 0000 0014 043d 0435  Widget.......=.5
+00004ea0: 0438 0437 0432 0435 0441 0442 043d 043e  .8.7.2.5.A.B.=.>
+00004eb0: 0800 0000 0006 0000 0007 756e 6b6e 6f77  ..........unknow
+00004ec0: 6e07 0000 000e 4469 7669 6465 6e64 5769  n.....DividendWi
+00004ed0: 6467 6574 0103 0000 0010 0421 0432 043e  dget.......!.2.>
+00004ee0: 0439 0441 0442 0432 043e 0800 0000 0006  .9.A.B.2.>......
+00004ef0: 0000 0008 5072 6f70 6572 7479 0700 0000  ....Property....
+00004f00: 0e45 7874 7261 4461 7461 4d6f 6465 6c01  .ExtraDataModel.
+00004f10: 0300 0000 1004 1704 3d04 3004 4704 3504  ........=.0.G.5.
+00004f20: 3d04 3804 3508 0000 0000 0600 0000 0556  =.8.5..........V
+00004f30: 616c 7565 0700 0000 0e45 7874 7261 4461  alue.....ExtraDa
+00004f40: 7461 4d6f 6465 6c01 0300 0000 1a04 2604  taModel.......&.
+00004f50: 3504 3d04 3d04 3004 4f00 2004 3104 4304  5.=.=.0.O. .1.C.
+00004f60: 3c04 3004 3304 3008 0000 0000 0600 0000  <.0.3.0.........
+00004f70: 0a41 7373 6574 204e 616d 6507 0000 000d  .Asset Name.....
+00004f80: 486f 6c64 696e 6773 4d6f 6465 6c01 0300  HoldingsModel...
+00004f90: 0000 1c04 1204 3004 3b04 4e04 4204 3000  ......0.;.N.B.0.
+00004fa0: 2f04 2104 4704 5104 4200 2f04 2604 1108  /.!.G.Q.B./.&...
+00004fb0: 0000 0000 0600 0000 1643 7572 7265 6e63  .........Currenc
+00004fc0: 792f 4163 636f 756e 742f 4173 7365 7407  y/Account/Asset.
+00004fd0: 0000 000d 486f 6c64 696e 6773 4d6f 6465  ....HoldingsMode
+00004fe0: 6c01 0300 0000 0a04 2d04 3a04 4104 3f00  l.......-.:.A.?.
+00004ff0: 3a08 0000 0000 0600 0000 0445 7870 3a07  :..........Exp:.
+00005000: 0000 000d 486f 6c64 696e 6773 4d6f 6465  ....HoldingsMode
+00005010: 6c01 0300 0000 1404 2604 3504 3d04 3000  l.......&.5.=.0.
+00005020: 2004 3704 3004 3a04 4000 2e08 0000 0000   .7.0.:.@.......
+00005030: 0600 0000 044c 6173 7407 0000 000d 486f  .....Last.....Ho
+00005040: 6c64 696e 6773 4d6f 6465 6c01 0300 0000  ldingsModel.....
+00005050: 3404 1404 3004 4204 3000 2004 3f04 3e04  4...0.B.0. .?.>.
+00005060: 4104 3b04 3504 3404 3d04 3504 3900 2004  A.;.5.4.=.5.9. .
+00005070: 3a04 3e04 4204 3804 4004 3e04 3204 3a04  :.>.B.8.@.>.2.:.
+00005080: 3800 3a00 2008 0000 0000 0600 0000 114c  8.:. ..........L
+00005090: 6173 7420 7175 6f74 6520 6461 7465 3a20  ast quote date: 
+000050a0: 0700 0000 0d48 6f6c 6469 6e67 734d 6f64  .....HoldingsMod
+000050b0: 656c 0103 0000 0014 0426 0435 043d 0430  el.......&.5.=.0
+000050c0: 0020 043e 0442 043a 0440 002e 0800 0000  . .>.B.:.@......
+000050d0: 0006 0000 0004 4f70 656e 0700 0000 0d48  ......Open.....H
+000050e0: 6f6c 6469 6e67 734d 6f64 656c 0103 0000  oldingsModel....
+000050f0: 0006 041f 0438 0423 0800 0000 0006 0000  .....8.#........
+00005100: 0003 502f 4c07 0000 000d 486f 6c64 696e  ..P/L.....Holdin
+00005110: 6773 4d6f 6465 6c01 0300 0000 0c04 1f04  gsModel.........
+00005120: 3804 2300 2c00 2000 2508 0000 0000 0600  8.#.,. .%.......
+00005130: 0000 0650 2f4c 2c20 2507 0000 000d 486f  ...P/L, %.....Ho
+00005140: 6c64 696e 6773 4d6f 6465 6c01 0300 0000  ldingsModel.....
+00005150: 0c04 1a04 3e04 3b00 2d04 3204 3e08 0000  ....>.;.-.2.>...
+00005160: 0000 0600 0000 0351 7479 0700 0000 0d48  .......Qty.....H
+00005170: 6f6c 6469 6e67 734d 6f64 656c 0103 0000  oldingsModel....
+00005180: 000e 0414 043e 043b 044f 002c 0020 0025  .....>.;.O.,. .%
+00005190: 0800 0000 0006 0000 0008 5368 6172 652c  ..........Share,
+000051a0: 2025 0700 0000 0d48 6f6c 6469 6e67 734d   %.....HoldingsM
+000051b0: 6f64 656c 0103 0000 000c 041e 0446 0435  odel.........F.5
+000051c0: 043d 043a 0430 0800 0000 0006 0000 0005  .=.:.0..........
+000051d0: 5661 6c75 6507 0000 000d 486f 6c64 696e  Value.....Holdin
+000051e0: 6773 4d6f 6465 6c01 0300 0000 1004 1e04  gsModel.........
+000051f0: 4604 3504 3d04 3a04 3000 2c00 2008 0000  F.5.=.:.0.,. ...
+00005200: 0000 0600 0000 0756 616c 7565 2c20 0700  .......Value, ..
+00005210: 0000 0d48 6f6c 6469 6e67 734d 6f64 656c  ...HoldingsModel
+00005220: 0103 0000 0016 041f 043e 0440 0442 0444  .........>.@.B.D
+00005230: 0435 043b 044c 0020 0426 0411 0800 0000  .5.;.L. .&......
+00005240: 0006 0000 0008 486f 6c64 696e 6773 0700  ......Holdings..
+00005250: 0000 0e48 6f6c 6469 6e67 7352 6570 6f72  ...HoldingsRepor
+00005260: 7401 0300 0000 1a04 1e04 4604 3504 3d04  t.........F.5.=.
+00005270: 3804 4204 4c00 2004 3d04 3004 3b04 3e04  8.B.L. .=.0.;.>.
+00005280: 3308 0000 0000 0600 0000 0c45 7374 696d  3..........Estim
+00005290: 6174 6520 7461 7807 0000 0014 486f 6c64  ate tax.....Hold
+000052a0: 696e 6773 5265 706f 7274 5769 6e64 6f77  ingsReportWindow
+000052b0: 0103 0000 0016 041f 043e 0440 0442 0444  .........>.@.B.D
+000052c0: 0435 043b 044c 0020 0426 0411 0800 0000  .5.;.L. .&......
+000052d0: 0006 0000 0008 486f 6c64 696e 6773 0700  ......Holdings..
+000052e0: 0000 1448 6f6c 6469 6e67 7352 6570 6f72  ...HoldingsRepor
+000052f0: 7457 696e 646f 7701 0300 0000 1404 1f04  tWindow.........
+00005300: 3e04 4004 4204 4304 3304 3004 3b04 3804  >.@.B.C.3.0.;.8.
+00005310: 4f08 0000 0000 0600 0000 0850 6f72 7475  O..........Portu
+00005320: 6761 6c07 0000 0014 486f 6c64 696e 6773  gal.....Holdings
+00005330: 5265 706f 7274 5769 6e64 6f77 0103 0000  ReportWindow....
+00005340: 000c 0420 043e 0441 0441 0438 044f 0800  ... .>.A.A.8.O..
+00005350: 0000 0006 0000 0006 5275 7373 6961 0700  ........Russia..
+00005360: 0000 1448 6f6c 6469 6e67 7352 6570 6f72  ...HoldingsRepor
+00005370: 7457 696e 646f 7701 0300 0000 2804 1f04  tWindow.....(...
+00005380: 3e04 3a04 3004 3704 3004 4204 4c00 2004  >.:.0.7.0.B.L. .
+00005390: 3304 4004 3004 4404 3804 3a00 2004 4604  3.@.0.D.8.:. .F.
+000053a0: 3504 3d04 4b08 0000 0000 0600 0000 1053  5.=.K..........S
+000053b0: 686f 7720 5072 6963 6520 4368 6172 7407  how Price Chart.
+000053c0: 0000 0014 486f 6c64 696e 6773 5265 706f  ....HoldingsRepo
+000053d0: 7274 5769 6e64 6f77 0103 0000 0022 0412  rtWindow....."..
+000053e0: 0430 043b 044e 0442 0430 0020 043f 0435  .0.;.N.B.0. .?.5
+000053f0: 0440 0435 0441 0447 0451 0442 0430 003a  .@.5.A.G.Q.B.0.:
+00005400: 0800 0000 0006 0000 0010 436f 6d6d 6f6e  ..........Common
+00005410: 2063 7572 7265 6e63 793a 0700 0000 0e48   currency:.....H
+00005420: 6f6c 6469 6e67 7357 6964 6765 7401 0300  oldingsWidget...
+00005430: 0000 1604 1f04 3e04 4004 4204 4404 3504  ......>.@.B.D.5.
+00005440: 3b04 4c00 2004 2604 1108 0000 0000 0600  ;.L. .&.........
+00005450: 0000 0848 6f6c 6469 6e67 7307 0000 000e  ...Holdings.....
+00005460: 486f 6c64 696e 6773 5769 6467 6574 0103  HoldingsWidget..
+00005470: 0000 0018 0421 043e 0445 0440 0430 043d  .....!.>.E.@.0.=
+00005480: 0438 0442 044c 002e 002e 002e 0800 0000  .8.B.L..........
+00005490: 0006 0000 0007 5361 7665 2e2e 2e07 0000  ......Save......
+000054a0: 000e 486f 6c64 696e 6773 5769 6467 6574  ..HoldingsWidget
+000054b0: 0103 0000 0014 0064 0064 002f 004d 004d  .......d.d./.M.M
+000054c0: 002f 0079 0079 0079 0079 0800 0000 0006  ./.y.y.y.y......
+000054d0: 0000 000a 6464 2f4d 4d2f 7979 7979 0700  ....dd/MM/yyyy..
+000054e0: 0000 0e48 6f6c 6469 6e67 7357 6964 6765  ...HoldingsWidge
+000054f0: 7401 0300 0000 3404 2204 3804 3f00 2004  t.....4.".8.?. .
+00005500: 2604 1100 2004 3d04 3500 2004 3f04 3e04  &... .=.5. .?.>.
+00005510: 3404 3404 3504 4004 3604 3804 3204 3004  4.4.5.@.6.8.2.0.
+00005520: 3504 4204 4104 4f00 3a00 2008 0000 0000  5.B.A.O.:. .....
+00005530: 0600 0000 1c41 7373 6574 2074 7970 6520  .....Asset type 
+00005540: 6973 6e27 7420 7375 7070 6f72 7465 643a  isn't supported:
+00005550: 2007 0000 0004 4942 4b52 0103 0000 0054   .....IBKR.....T
+00005560: 041a 043e 0440 043f 043e 0440 0430 0442  ...>.@.?.>.@.0.B
+00005570: 0438 0432 043d 043e 0435 0020 0434 0435  .8.2.=.>.5. .4.5
+00005580: 0439 0441 0442 0432 0438 0435 0020 043d  .9.A.B.2.8.5. .=
+00005590: 0435 0020 043f 043e 0434 0434 0435 0440  .5. .?.>.4.4.5.@
+000055a0: 0436 0438 0432 0430 0435 0442 0441 044f  .6.8.2.0.5.B.A.O
+000055b0: 003a 0020 0800 0000 0006 0000 0022 436f  .:. ........."Co
+000055c0: 7270 6f72 6174 6520 6163 7469 6f6e 2069  rporate action i
+000055d0: 736e 2774 2073 7570 706f 7274 6564 3a20  sn't supported: 
+000055e0: 0700 0000 0449 424b 5201 0300 0000 4604  .....IBKR.....F.
+000055f0: 1d04 3504 3e04 3404 3d04 3e04 3704 3d04  ..5.>.4.=.>.7.=.
+00005600: 3004 4704 3d04 3e04 3500 2004 4104 3e04  0.G.=.>.5. .A.>.
+00005610: 3204 3f04 3004 3404 3504 3d04 3804 3500  2.?.0.4.5.=.8.5.
+00005620: 2004 4104 4704 5104 4204 3000 2004 3404   .A.G.Q.B.0. .4.
+00005630: 3b04 4f00 2008 0000 0000 0600 0000 1b4d  ;.O. ..........M
+00005640: 756c 7469 706c 6520 6163 636f 756e 7420  ultiple account 
+00005650: 6d61 7463 6820 666f 7220 0700 0000 0449  match for .....I
+00005660: 424b 5201 0300 0000 6800 4a00 5300 4f00  BKR.....h.J.S.O.
+00005670: 4e00 2004 4204 4d04 3300 2000 2700 6400  N. .B.M.3. .'.d.
+00005680: 6f00 6300 7500 6d00 6500 6e00 7400 2700  o.c.u.m.e.n.t.'.
+00005690: 2004 3e04 4204 4104 4304 4204 4104 4204   .>.B.A.C.B.A.B.
+000056a0: 3204 4304 3504 4200 2004 3204 3d04 4304  2.C.5.B. .2.=.C.
+000056b0: 4204 4004 3800 2004 4204 4d04 3304 3000  B.@.8. .B.M.3.0.
+000056c0: 2000 2700 7400 6900 6300 6b00 6500 7400   .'.t.i.c.k.e.t.
+000056d0: 2708 0000 0000 0600 0000 2a43 616e 2774  '.........*Can't
+000056e0: 2066 696e 6420 2764 6f63 756d 656e 7427   find 'document'
+000056f0: 2074 6167 2069 6e20 6a73 6f6e 2027 7469   tag in json 'ti
+00005700: 636b 6574 2707 0000 0010 496d 706f 7274  cket'.....Import
+00005710: 536c 6970 4469 616c 6f67 0103 0000 0072  SlipDialog.....r
+00005720: 004a 0053 004f 004e 0020 0442 044d 0433  .J.S.O.N. .B.M.3
+00005730: 0020 0027 006f 0070 0065 0072 0061 0074  . .'.o.p.e.r.a.t
+00005740: 0069 006f 006e 0054 0079 0070 0065 0027  .i.o.n.T.y.p.e.'
+00005750: 0020 043e 0442 0441 0443 0442 0441 0442  . .>.B.A.C.B.A.B
+00005760: 0432 0443 0435 0442 0020 0432 043d 0443  .2.C.5.B. .2.=.C
+00005770: 0442 0440 0438 0020 0442 044d 0433 0430  .B.@.8. .B.M.3.0
+00005780: 0020 0027 0074 0069 0063 006b 0065 0074  . .'.t.i.c.k.e.t
+00005790: 0027 0800 0000 0006 0000 002f 4361 6e27  .'........./Can'
+000057a0: 7420 6669 6e64 2027 6f70 6572 6174 696f  t find 'operatio
+000057b0: 6e54 7970 6527 2074 6167 2069 6e20 6a73  nType' tag in js
+000057c0: 6f6e 2027 7469 636b 6574 2707 0000 0010  on 'ticket'.....
+000057d0: 496d 706f 7274 536c 6970 4469 616c 6f67  ImportSlipDialog
+000057e0: 0103 0000 006a 004a 0053 004f 004e 0020  .....j.J.S.O.N. 
+000057f0: 0442 044d 0433 0020 0027 0072 0065 0063  .B.M.3. .'.r.e.c
+00005800: 0065 0069 0070 0074 0027 0020 043e 0442  .e.i.p.t.'. .>.B
+00005810: 0441 0443 0442 0441 0442 0432 0443 0435  .A.C.B.A.B.2.C.5
+00005820: 0442 0020 0432 043d 0443 0442 0440 0438  .B. .2.=.C.B.@.8
+00005830: 0020 0442 044d 0433 0430 0020 0027 0064  . .B.M.3.0. .'.d
+00005840: 006f 0063 0075 006d 0065 006e 0074 0027  .o.c.u.m.e.n.t.'
+00005850: 0800 0000 0006 0000 002b 4361 6e27 7420  .........+Can't 
+00005860: 6669 6e64 2027 7265 6365 6970 7427 2074  find 'receipt' t
+00005870: 6167 2069 6e20 6a73 6f6e 2027 646f 6375  ag in json 'docu
+00005880: 6d65 6e74 2707 0000 0010 496d 706f 7274  ment'.....Import
+00005890: 536c 6970 4469 616c 6f67 0103 0000 005e  SlipDialog.....^
+000058a0: 041a 0430 0442 0435 0433 043e 0440 0438  ...0.B.5.3.>.@.8
+000058b0: 0438 0020 043d 0435 0020 0440 0430 0441  .8. .=.5. .@.0.A
+000058c0: 043f 043e 0437 043d 0430 043d 044b 003a  .?.>.7.=.0.=.K.:
+000058d0: 0020 0054 0065 006e 0073 006f 0072 006c  . .T.e.n.s.o.r.l
+000058e0: 006f 0077 0020 043d 0435 0020 043e 0431  .o.w. .=.5. .>.1
+000058f0: 043d 0430 0440 0443 0436 0435 043d 0800  .=.0.@.C.6.5.=..
+00005900: 0000 0006 0000 0036 4361 7465 676f 7269  .......6Categori
+00005910: 6573 2061 7265 206e 6f74 2072 6563 6f67  es are not recog
+00005920: 6e69 7a65 643a 2054 656e 736f 7266 6c6f  nized: Tensorflo
+00005930: 7720 6973 206e 6f74 2066 6f75 6e64 0700  w is not found..
+00005940: 0000 1049 6d70 6f72 7453 6c69 7044 6961  ...ImportSlipDia
+00005950: 6c6f 6701 0300 0000 4a04 1f04 4004 3504  log.....J...@.5.
+00005960: 3204 4b04 4804 3504 3d04 3e00 2004 3c04  2.K.H.5.=.>. .<.
+00005970: 3004 3a04 4104 3804 3c04 3004 3b04 4c04  0.:.A.8.<.0.;.L.
+00005980: 3d04 3e04 3500 2004 4704 3804 4104 3b04  =.>.5. .G.8.A.;.
+00005990: 3e00 2004 3f04 3e04 3f04 4b04 4204 3e04  >. .?.>.?.K.B.>.
+000059a0: 3a00 2e08 0000 0000 0600 0000 194d 6178  :............Max
+000059b0: 2072 6574 7279 2063 6f75 6e74 2065 7863   retry count exc
+000059c0: 6565 6465 642e 0700 0000 1049 6d70 6f72  eeded......Impor
+000059d0: 7453 6c69 7044 6961 6c6f 6701 0300 0000  tSlipDialog.....
+000059e0: 4600 5100 5200 2004 3a04 3e04 3400 2004  F.Q.R. .:.>.4. .
+000059f0: 3d04 3500 2004 3e04 3104 3d04 3004 4004  =.5. .>.1.=.0.@.
+00005a00: 4304 3604 3504 3d00 2004 3200 2004 3104  C.6.5.=. .2. .1.
+00005a10: 4304 4404 3504 4004 3500 2004 3e04 3104  C.D.5.@.5. .>.1.
+00005a20: 3c04 3504 3d04 3008 0000 0000 0600 0000  <.5.=.0.........
+00005a30: 1e4e 6f20 5152 2063 6f64 6573 2066 6f75  .No QR codes fou
+00005a40: 6e64 2069 6e20 636c 6970 626f 6172 6407  nd in clipboard.
+00005a50: 0000 0010 496d 706f 7274 536c 6970 4469  ....ImportSlipDi
+00005a60: 616c 6f67 0103 0000 0036 0051 0052 002d  alog.....6.Q.R.-
+00005a70: 043a 043e 0434 0020 0432 0020 0444 0430  .:.>.4. .2. .D.0
+00005a80: 0439 043b 0435 0020 043d 0435 0020 043e  .9.;.5. .=.5. .>
+00005a90: 0431 043d 0430 0440 0443 0436 0435 043d  .1.=.0.@.C.6.5.=
+00005aa0: 0800 0000 0006 0000 001e 4e6f 2051 5220  ..........No QR 
+00005ab0: 636f 6465 7320 7765 7265 2066 6f75 6e64  codes were found
+00005ac0: 2069 6e20 6669 6c65 0700 0000 1049 6d70   in file.....Imp
+00005ad0: 6f72 7453 6c69 7044 6961 6c6f 6701 0300  ortSlipDialog...
+00005ae0: 0000 7204 1d04 3504 3204 3e04 3704 3c04  ..r...5.2.>.7.<.
+00005af0: 3e04 3604 3d04 3e00 2004 3404 3e04 3104  >.6.=.>. .4.>.1.
+00005b00: 3004 3204 3804 4204 4c00 2004 4704 3504  0.2.8.B.L. .G.5.
+00005b10: 3a00 3a00 2004 3d04 3500 2004 4304 3a04  :.:. .=.5. .C.:.
+00005b20: 3004 3704 3004 3d00 2004 3a04 3e04 3d04  0.7.0.=. .:.>.=.
+00005b30: 4204 4004 3004 3304 3504 3d04 4200 2004  B.@.0.3.5.=.B. .
+00005b40: 3404 3b04 4f00 2004 3804 3c04 3f04 3e04  4.;.O. .8.<.?.>.
+00005b50: 4004 4204 3008 0000 0000 0600 0000 414e  @.B.0.........AN
+00005b60: 6f74 2070 6f73 7369 626c 6520 746f 2069  ot possible to i
+00005b70: 6d70 6f72 7420 736c 6970 3a20 6361 6e27  mport slip: can'
+00005b80: 7420 696d 706f 7274 3a20 6e6f 2070 6565  t import: no pee
+00005b90: 7220 7365 7420 666f 7220 696d 706f 7274  r set for import
+00005ba0: 0700 0000 1049 6d70 6f72 7453 6c69 7044  .....ImportSlipD
+00005bb0: 6961 6c6f 6701 0300 0000 6604 1d04 3504  ialog.....f...5.
+00005bc0: 3204 3e04 3704 3c04 3e04 3604 3d04 3e00  2.>.7.<.>.6.=.>.
+00005bd0: 2004 3404 3e04 3104 3004 3204 3804 4204   .4.>.1.0.2.8.B.
+00005be0: 4c00 2004 4704 3504 3a00 3a00 2004 3d04  L. .G.5.:.:. .=.
+00005bf0: 3500 2004 4304 3a04 3004 3704 3004 3d00  5. .C.:.0.7.0.=.
+00005c00: 2004 4104 4704 3504 4200 2004 3404 3b04   .A.G.5.B. .4.;.
+00005c10: 4f00 2004 3804 3c04 3f04 3e04 4004 4204  O. .8.<.?.>.@.B.
+00005c20: 3008 0000 0000 0600 0000 364e 6f74 2070  0.........6Not p
+00005c30: 6f73 7369 626c 6520 746f 2069 6d70 6f72  ossible to impor
+00005c40: 7420 736c 6970 3a20 6e6f 2061 6363 6f75  t slip: no accou
+00005c50: 6e74 2073 6574 2066 6f72 2069 6d70 6f72  nt set for impor
+00005c60: 7407 0000 0010 496d 706f 7274 536c 6970  t.....ImportSlip
+00005c70: 4469 616c 6f67 0103 0000 0078 041d 0435  Dialog.....x...5
+00005c80: 0432 043e 0437 043c 043e 0436 043d 043e  .2.>.7.<.>.6.=.>
+00005c90: 0020 0434 043e 0431 0430 0432 0438 0442  . .4.>.1.0.2.8.B
+00005ca0: 044c 0020 0447 0435 043a 003a 0020 043a  .L. .G.5.:.:. .:
+00005cb0: 0430 0442 0435 0433 043e 0440 0438 0438  .0.B.5.3.>.@.8.8
+00005cc0: 0020 0443 043a 0430 0437 0430 043d 044b  . .C.:.0.7.0.=.K
+00005cd0: 0020 043d 0435 0020 0434 043b 044f 0020  . .=.5. .4.;.O. 
+00005ce0: 0432 0441 0435 0445 0020 0441 0442 0440  .2.A.5.E. .A.B.@
+00005cf0: 043e 043a 0800 0000 0006 0000 0038 4e6f  .>.:.........8No
+00005d00: 7420 706f 7373 6962 6c65 2074 6f20 696d  t possible to im
+00005d10: 706f 7274 2073 6c69 703a 2073 6f6d 6520  port slip: some 
+00005d20: 6361 7465 676f 7269 6573 2061 7265 206e  categories are n
+00005d30: 6f74 2073 6574 0700 0000 1049 6d70 6f72  ot set.....Impor
+00005d40: 7453 6c69 7044 6961 6c6f 6701 0300 0000  tSlipDialog.....
+00005d50: 5404 1d04 3504 3204 3e04 3704 3c04 3e04  T...5.2.>.7.<.>.
+00005d60: 3604 3d04 3e00 2004 4004 3004 4104 3f04  6.=.>. .@.0.A.?.
+00005d70: 3e04 3704 3d04 3004 4204 4c00 2004 3f04  >.7.=.0.B.L. .?.
+00005d80: 4004 3e04 4704 3804 4204 3004 3d04 3d04  @.>.G.8.B.0.=.=.
+00005d90: 4b04 3900 2000 5100 5200 2d04 3a04 3e04  K.9. .Q.R.-.:.>.
+00005da0: 3400 3a00 2008 0000 0000 0600 0000 2b51  4.:. .........+Q
+00005db0: 5220 6176 6169 6c61 626c 6520 6275 7420  R available but 
+00005dc0: 7061 7474 6572 6e20 6973 6e27 7420 7265  pattern isn't re
+00005dd0: 636f 676e 697a 6564 3a20 0700 0000 1049  cognized: .....I
+00005de0: 6d70 6f72 7453 6c69 7044 6961 6c6f 6701  mportSlipDialog.
+00005df0: 0300 0000 0800 5100 5200 3a00 2008 0000  ......Q.R.:. ...
+00005e00: 0000 0600 0000 0451 523a 2007 0000 0010  .......QR: .....
+00005e10: 496d 706f 7274 536c 6970 4469 616c 6f67  ImportSlipDialog
+00005e20: 0103 0000 0030 0412 044b 0431 0435 0440  .....0...K.1.5.@
+00005e30: 0438 0442 0435 0020 0444 0430 0439 043b  .8.B.5. .D.0.9.;
+00005e40: 0020 0441 0020 0051 0052 002d 043a 043e  . .A. .Q.R.-.:.>
+00005e50: 0434 043e 043c 0800 0000 0006 0000 0018  .4.>.<..........
+00005e60: 5365 6c65 6374 2066 696c 6520 7769 7468  Select file with
+00005e70: 2051 5220 636f 6465 0700 0000 1049 6d70   QR code.....Imp
+00005e80: 6f72 7453 6c69 7044 6961 6c6f 6701 0300  ortSlipDialog...
+00005e90: 0000 4204 1204 4b04 3104 3504 4004 3804  ..B...K.1.5.@.8.
+00005ea0: 4204 3500 2004 4404 3004 3904 3b00 2004  B.5. .D.0.9.;. .
+00005eb0: 4100 2000 4a00 5300 4f00 4e00 2d04 3404  A. .J.S.O.N.-.4.
+00005ec0: 3004 3d04 3d04 4b04 3c04 3800 2004 4704  0.=.=.K.<.8. .G.
+00005ed0: 3504 3a04 3008 0000 0000 0600 0000 1f53  5.:.0..........S
+00005ee0: 656c 6563 7420 6669 6c65 2077 6974 6820  elect file with 
+00005ef0: 736c 6970 204a 534f 4e20 6461 7461 0700  slip JSON data..
+00005f00: 0000 1049 6d70 6f72 7453 6c69 7044 6961  ...ImportSlipDia
+00005f10: 6c6f 6701 0300 0000 3204 1d04 3504 3804  log.....2...5.8.
+00005f20: 3704 3204 3504 4104 4204 3d04 4b04 3900  7.2.5.A.B.=.K.9.
+00005f30: 2004 4204 3804 3f00 2004 3e04 3f04 3504   .B.8.?. .>.?.5.
+00005f40: 4004 3004 4604 3804 3800 2008 0000 0000  @.0.F.8.8. .....
+00005f50: 0600 0000 1755 6e6b 6e6f 776e 206f 7065  .....Unknown ope
+00005f60: 7261 7469 6f6e 2074 7970 6520 0700 0000  ration type ....
+00005f70: 1049 6d70 6f72 7453 6c69 7044 6961 6c6f  .ImportSlipDialo
+00005f80: 6701 0300 0000 0600 2027 9c00 2008 0000  g....... '.. ...
+00005f90: 0000 0600 0000 0520 e29e 9c20 0700 0000  ....... ... ....
+00005fa0: 0d49 6d70 6f72 7453 6c69 7044 6c67 0103  .ImportSlipDlg..
+00005fb0: 0000 000a 0421 0447 0435 0442 003a 0800  .....!.G.5.B.:..
+00005fc0: 0000 0006 0000 0008 4163 636f 756e 743a  ........Account:
+00005fd0: 0700 0000 0d49 6d70 6f72 7453 6c69 7044  .....ImportSlipD
+00005fe0: 6c67 0103 0000 0010 0414 043e 0431 0430  lg.........>.1.0
+00005ff0: 0432 0438 0442 044c 0800 0000 0006 0000  .2.8.B.L........
+00006000: 0003 4164 6407 0000 000d 496d 706f 7274  ..Add.....Import
+00006010: 536c 6970 446c 6701 0300 0000 0c04 2104  SlipDlg.......!.
+00006020: 4304 3c04 3c04 3000 3a08 0000 0000 0600  C.<.<.0.:.......
+00006030: 0000 0741 6d6f 756e 743a 0700 0000 0d49  ...Amount:.....I
+00006040: 6d70 6f72 7453 6c69 7044 6c67 0103 0000  mportSlipDlg....
+00006050: 0032 0410 0432 0442 043e 002d 043d 0430  .2...2.B.>.-.=.0
+00006060: 0437 043d 0430 0447 0435 043d 0438 0435  .7.=.0.G.5.=.8.5
+00006070: 0020 043a 0430 0442 0435 0433 043e 0440  . .:.0.B.5.3.>.@
+00006080: 0438 0439 0800 0000 0006 0000 0016 4175  .8.9..........Au
+00006090: 746f 2d61 7373 6967 6e20 6361 7465 676f  to-assign catego
+000060a0: 7269 6573 0700 0000 0d49 6d70 6f72 7453  ries.....ImportS
+000060b0: 6c69 7044 6c67 0103 0000 000c 041a 0430  lipDlg.........0
+000060c0: 043c 0435 0440 0430 0800 0000 0006 0000  .<.5.@.0........
+000060d0: 0006 4361 6d65 7261 0700 0000 0d49 6d70  ..Camera.....Imp
+000060e0: 6f72 7453 6c69 7044 6c67 0103 0000 0010  ortSlipDlg......
+000060f0: 041e 0447 0438 0441 0442 0438 0442 044c  ...G.8.A.B.8.B.L
+00006100: 0800 0000 0006 0000 0005 436c 6561 7207  ..........Clear.
+00006110: 0000 000d 496d 706f 7274 536c 6970 446c  ....ImportSlipDl
+00006120: 6701 0300 0000 0e04 1704 3004 3a04 4004  g.........0.:.@.
+00006130: 4b04 4204 4c08 0000 0000 0600 0000 0543  K.B.L..........C
+00006140: 6c6f 7365 0700 0000 0d49 6d70 6f72 7453  lose.....ImportS
+00006150: 6c69 7044 6c67 0103 0000 001a 0414 0430  lipDlg.........0
+00006160: 0442 0430 0020 002f 0020 0412 0440 0435  .B.0. ./. ...@.5
+00006170: 043c 044f 003a 0800 0000 0006 0000 000c  .<.O.:..........
+00006180: 4461 7465 202f 2054 696d 653a 0700 0000  Date / Time:....
+00006190: 0d49 6d70 6f72 7453 6c69 7044 6c67 0103  .ImportSlipDlg..
+000061a0: 0000 0016 0414 0430 0442 0430 002f 0412  .......0.B.0./..
+000061b0: 0440 0435 043c 044f 003a 0800 0000 0006  .@.5.<.O.:......
+000061c0: 0000 000a 4461 7465 2f54 696d 653a 0700  ....Date/Time:..
+000061d0: 0000 0d49 6d70 6f72 7453 6c69 7044 6c67  ...ImportSlipDlg
+000061e0: 0103 0000 0006 0424 0414 003a 0800 0000  .......$...:....
+000061f0: 0006 0000 0003 4644 3a07 0000 000d 496d  ......FD:.....Im
+00006200: 706f 7274 536c 6970 446c 6701 0300 0000  portSlipDlg.....
+00006210: 0604 2404 1d00 3a08 0000 0000 0600 0000  ..$...:.........
+00006220: 0346 4e3a 0700 0000 0d49 6d70 6f72 7453  .FN:.....ImportS
+00006230: 6c69 7044 6c67 0103 0000 0006 0424 041f  lipDlg.......$..
+00006240: 003a 0800 0000 0006 0000 0003 4650 3a07  .:..........FP:.
+00006250: 0000 000d 496d 706f 7274 536c 6970 446c  ....ImportSlipDl
+00006260: 6701 0300 0000 2604 2104 3a04 3004 3d04  g.....&.!.:.0.=.
+00006270: 3804 4004 3e04 3204 3004 4204 4c00 2004  8.@.>.2.0.B.L. .
+00006280: 3a04 3004 3c04 3504 4004 3e04 3908 0000  :.0.<.5.@.>.9...
+00006290: 0000 0600 0000 0f47 6574 2066 726f 6d20  .......Get from 
+000062a0: 6361 6d65 7261 0700 0000 0d49 6d70 6f72  camera.....Impor
+000062b0: 7453 6c69 7044 6c67 0103 0000 0024 041f  tSlipDlg.....$..
+000062c0: 043e 043b 0443 0447 0438 0442 044c 0020  .>.;.C.G.8.B.L. 
+000062d0: 0438 0437 0020 0431 0443 0444 0435 0440  .8.7. .1.C.D.5.@
+000062e0: 0430 0800 0000 0006 0000 0012 4765 7420  .0..........Get 
+000062f0: 6672 6f6d 2063 6c69 7062 6f61 7264 0700  from clipboard..
+00006300: 0000 0d49 6d70 6f72 7453 6c69 7044 6c67  ...ImportSlipDlg
+00006310: 0103 0000 0030 041f 043e 043b 0443 0447  .....0...>.;.C.G
+00006320: 0438 0442 044c 0020 0447 0435 043a 0020  .8.B.L. .G.5.:. 
+00006330: 0441 0020 0441 0430 0439 0442 0430 0020  .A. .A.0.9.B.0. 
+00006340: 0424 041d 0421 0800 0000 0006 0000 0016  .$...!..........
+00006350: 4765 7420 736c 6970 2066 726f 6d20 696e  Get slip from in
+00006360: 7465 726e 6574 0700 0000 0d49 6d70 6f72  ternet.....Impor
+00006370: 7453 6c69 7044 6c67 0103 0000 0016 0418  tSlipDlg........
+00006380: 043c 043f 043e 0440 0442 0020 0447 0435  .<.?.>.@.B. .G.5
+00006390: 043a 0430 0800 0000 0006 0000 000b 496d  .:.0..........Im
+000063a0: 706f 7274 2053 6c69 7007 0000 000d 496d  port Slip.....Im
+000063b0: 706f 7274 536c 6970 446c 6701 0300 0000  portSlipDlg.....
+000063c0: 0e04 2104 4204 4004 3e04 3a04 3800 3a08  ..!.B.@.>.:.8.:.
+000063d0: 0000 0000 0600 0000 064c 696e 6573 3a07  .........Lines:.
+000063e0: 0000 000d 496d 706f 7274 536c 6970 446c  ....ImportSlipDl
+000063f0: 6701 0300 0000 2404 1704 3004 3304 4004  g.....$...0.3.@.
+00006400: 4304 3704 3804 4204 4c00 2004 3804 3700  C.7.8.B.L. .8.7.
+00006410: 2004 4404 3004 3904 3b04 3008 0000 0000   .D.0.9.;.0.....
+00006420: 0600 0000 0e4c 6f61 6420 6672 6f6d 2066  .....Load from f
+00006430: 696c 6507 0000 000d 496d 706f 7274 536c  ile.....ImportSl
+00006440: 6970 446c 6701 0300 0000 3604 1704 3004  ipDlg.....6...0.
+00006450: 3304 4304 3704 3804 4204 4c00 2004 4704  3.C.7.8.B.L. .G.
+00006460: 3504 3a04 3000 2004 3804 3700 2000 4a00  5.:.0. .8.7. .J.
+00006470: 5300 4f00 4e00 2d04 4404 3004 3904 3b04  S.O.N.-.D.0.9.;.
+00006480: 3008 0000 0000 0600 0000 184c 6f61 6420  0..........Load 
+00006490: 736c 6970 2066 726f 6d20 4a53 4f4e 2066  slip from JSON f
+000064a0: 696c 6507 0000 000d 496d 706f 7274 536c  ile.....ImportSl
+000064b0: 6970 446c 6701 0300 0000 1604 1a04 3e04  ipDlg.........>.
+000064c0: 3d04 4204 4004 3004 3304 3504 3d04 4200  =.B.@.0.3.5.=.B.
+000064d0: 3a08 0000 0000 0600 0000 0550 6565 723a  :..........Peer:
+000064e0: 0700 0000 0d49 6d70 6f72 7453 6c69 7044  .....ImportSlipD
+000064f0: 6c67 0103 0000 000e 041f 043e 043a 0443  lg.........>.:.C
+00006500: 043f 043a 0430 0800 0000 0006 0000 0008  .?.:.0..........
+00006510: 5075 7263 6861 7365 0700 0000 0d49 6d70  Purchase.....Imp
+00006520: 6f72 7453 6c69 7044 6c67 0103 0000 000c  ortSlipDlg......
+00006530: 0051 0052 002d 043a 043e 0434 0800 0000  .Q.R.-.:.>.4....
+00006540: 0006 0000 0007 5152 2d63 6f64 6507 0000  ......QR-code...
+00006550: 000d 496d 706f 7274 536c 6970 446c 6701  ..ImportSlipDlg.
+00006560: 0300 0000 0e04 1204 3e04 3704 3204 4004  ........>.7.2.@.
+00006570: 3004 4208 0000 0000 0600 0000 0652 6574  0.B..........Ret
+00006580: 7572 6e07 0000 000d 496d 706f 7274 536c  urn.....ImportSl
+00006590: 6970 446c 6701 0300 0000 2e04 2304 4104  ipDlg.......#.A.
+000065a0: 4204 3004 3d04 3e04 3204 3804 4204 4c00  B.0.=.>.2.8.B.L.
+000065b0: 2004 4204 4d04 3300 2004 3404 3b04 4f00   .B.M.3. .4.;.O.
+000065c0: 2004 3204 4104 3504 4508 0000 0000 0600   .2.A.5.E.......
+000065d0: 0000 1553 6574 2054 6167 2066 6f72 2061  ...Set Tag for a
+000065e0: 6c6c 206c 696e 6573 0700 0000 0d49 6d70  ll lines.....Imp
+000065f0: 6f72 7453 6c69 7044 6c67 0103 0000 0006  ortSlipDlg......
+00006600: 0427 0435 043a 0800 0000 0006 0000 0004  .'.5.:..........
+00006610: 536c 6970 0700 0000 0d49 6d70 6f72 7453  Slip.....ImportS
+00006620: 6c69 7044 6c67 0103 0000 0016 0414 0430  lipDlg.........0
+00006630: 043d 043d 044b 0435 0020 0447 0435 043a  .=.=.K.5. .G.5.:
+00006640: 0430 0800 0000 0006 0000 0009 536c 6970  .0..........Slip
+00006650: 2064 6174 6107 0000 000d 496d 706f 7274   data.....Import
+00006660: 536c 6970 446c 6701 0300 0000 1c04 1704  SlipDlg.........
+00006670: 3004 3a04 4004 4b04 4204 4c00 2004 3a04  0.:.@.K.B.L. .:.
+00006680: 3004 3c04 3504 4004 4308 0000 0000 0600  0.<.5.@.C.......
+00006690: 0000 0b53 746f 7020 6361 6d65 7261 0700  ...Stop camera..
+000066a0: 0000 0d49 6d70 6f72 7453 6c69 7044 6c67  ...ImportSlipDlg
+000066b0: 0103 0000 0008 0422 0438 043f 003a 0800  .......".8.?.:..
+000066c0: 0000 0006 0000 0005 5479 7065 3a07 0000  ........Type:...
+000066d0: 000d 496d 706f 7274 536c 6970 446c 6701  ..ImportSlipDlg.
+000066e0: 0300 0000 2600 6400 6400 2f00 4d00 4d00  ....&.d.d./.M.M.
+000066f0: 2f00 7900 7900 7900 7900 2000 6800 6800  /.y.y.y.y. .h.h.
+00006700: 3a00 6d00 6d00 3a00 7300 7308 0000 0000  :.m.m.:.s.s.....
+00006710: 0600 0000 1364 642f 4d4d 2f79 7979 7920  .....dd/MM/yyyy 
+00006720: 6868 3a6d 6d3a 7373 0700 0000 0d49 6d70  hh:mm:ss.....Imp
+00006730: 6f72 7453 6c69 7044 6c67 0103 0000 0066  ortSlipDlg.....f
+00006740: 041d 0435 0432 043e 0437 043c 043e 0436  ...5.2.>.7.<.>.6
+00006750: 043d 043e 0020 043e 0431 0440 0430 0431  .=.>. .>.1.@.0.1
+00006760: 043e 0442 0430 0442 044c 0020 043e 043f  .>.B.0.B.L. .>.?
+00006770: 0435 0440 0430 0446 0438 044e 0020 0431  .5.@.0.F.8.N. .1
+00006780: 0435 0437 0020 0434 0435 0442 0430 043b  .5.7. .4.5.B.0.;
+00006790: 044c 043d 044b 0445 0020 0434 0430 043d  .L.=.K.E. .4.0.=
+000067a0: 043d 044b 0445 0800 0000 0006 0000 0027  .=.K.E.........'
+000067b0: 4361 6e27 7420 7072 6f63 6573 7320 6f70  Can't process op
+000067c0: 6572 6174 696f 6e20 7769 7468 6f75 7420  eration without 
+000067d0: 6465 7461 696c 7307 0000 000e 496e 636f  details.....Inco
+000067e0: 6d65 5370 656e 6469 6e67 0103 0000 000c  meSpending......
+000067f0: 041a 0443 0440 0441 003a 0020 0800 0000  ...C.@.A.:. ....
+00006800: 0006 0000 0006 5261 7465 3a20 0700 0000  ......Rate: ....
+00006810: 0e49 6e63 6f6d 6553 7065 6e64 696e 6701  .IncomeSpending.
+00006820: 0300 0000 1c04 1404 3e04 4504 3e04 3404  ........>.E.>.4.
+00006830: 4b00 2004 3800 2004 2204 4004 3004 4204  K. .8. .".@.0.B.
+00006840: 4b08 0000 0000 0600 0000 1149 6e63 6f6d  K..........Incom
+00006850: 6520 2620 5370 656e 6469 6e67 0700 0000  e & Spending....
+00006860: 1449 6e63 6f6d 6553 7065 6e64 696e 6752  .IncomeSpendingR
+00006870: 6570 6f72 7401 0300 0000 0604 1004 3f04  eport.........?.
+00006880: 4008 0000 0000 0600 0000 0341 7072 0700  @..........Apr..
+00006890: 0000 1949 6e63 6f6d 6553 7065 6e64 696e  ...IncomeSpendin
+000068a0: 6752 6570 6f72 744d 6f64 656c 0103 0000  gReportModel....
+000068b0: 0006 0410 0432 0433 0800 0000 0006 0000  .....2.3........
+000068c0: 0003 4175 6707 0000 0019 496e 636f 6d65  ..Aug.....Income
+000068d0: 5370 656e 6469 6e67 5265 706f 7274 4d6f  SpendingReportMo
+000068e0: 6465 6c01 0300 0000 0604 1404 3504 3a08  del.........5.:.
+000068f0: 0000 0000 0600 0000 0344 6563 0700 0000  .........Dec....
+00006900: 1949 6e63 6f6d 6553 7065 6e64 696e 6752  .IncomeSpendingR
+00006910: 6570 6f72 744d 6f64 656c 0103 0000 0006  eportModel......
+00006920: 0424 0435 0432 0800 0000 0006 0000 0003  .$.5.2..........
+00006930: 4665 6207 0000 0019 496e 636f 6d65 5370  Feb.....IncomeSp
+00006940: 656e 6469 6e67 5265 706f 7274 4d6f 6465  endingReportMode
+00006950: 6c01 0300 0000 0604 2f04 3d04 3208 0000  l......./.=.2...
+00006960: 0000 0600 0000 034a 616e 0700 0000 1949  .......Jan.....I
+00006970: 6e63 6f6d 6553 7065 6e64 696e 6752 6570  ncomeSpendingRep
+00006980: 6f72 744d 6f64 656c 0103 0000 0006 0418  ortModel........
+00006990: 044e 043b 0800 0000 0006 0000 0003 4a75  .N.;..........Ju
+000069a0: 6c07 0000 0019 496e 636f 6d65 5370 656e  l.....IncomeSpen
+000069b0: 6469 6e67 5265 706f 7274 4d6f 6465 6c01  dingReportModel.
+000069c0: 0300 0000 0604 1804 4e04 3d08 0000 0000  ........N.=.....
+000069d0: 0600 0000 034a 756e 0700 0000 1949 6e63  .....Jun.....Inc
+000069e0: 6f6d 6553 7065 6e64 696e 6752 6570 6f72  omeSpendingRepor
+000069f0: 744d 6f64 656c 0103 0000 0006 041c 0430  tModel.........0
+00006a00: 0440 0800 0000 0006 0000 0003 4d61 7207  .@..........Mar.
+00006a10: 0000 0019 496e 636f 6d65 5370 656e 6469  ....IncomeSpendi
+00006a20: 6e67 5265 706f 7274 4d6f 6465 6c01 0300  ngReportModel...
+00006a30: 0000 0604 1c04 3004 3908 0000 0000 0600  ......0.9.......
+00006a40: 0000 034d 6179 0700 0000 1949 6e63 6f6d  ...May.....Incom
+00006a50: 6553 7065 6e64 696e 6752 6570 6f72 744d  eSpendingReportM
+00006a60: 6f64 656c 0103 0000 0006 041d 043e 044f  odel.........>.O
+00006a70: 0800 0000 0006 0000 0003 4e6f 7607 0000  ..........Nov...
+00006a80: 0019 496e 636f 6d65 5370 656e 6469 6e67  ..IncomeSpending
+00006a90: 5265 706f 7274 4d6f 6465 6c01 0300 0000  ReportModel.....
+00006aa0: 0604 1e04 3a04 4208 0000 0000 0600 0000  ....:.B.........
+00006ab0: 034f 6374 0700 0000 1949 6e63 6f6d 6553  .Oct.....IncomeS
+00006ac0: 7065 6e64 696e 6752 6570 6f72 744d 6f64  pendingReportMod
+00006ad0: 656c 0103 0000 0006 0421 0435 043d 0800  el.......!.5.=..
+00006ae0: 0000 0006 0000 0003 5365 7007 0000 0019  ........Sep.....
+00006af0: 496e 636f 6d65 5370 656e 6469 6e67 5265  IncomeSpendingRe
+00006b00: 706f 7274 4d6f 6465 6c01 0300 0000 0a04  portModel.......
+00006b10: 1804 2204 1e04 1304 1e08 0000 0000 0600  ..".............
+00006b20: 0000 0554 4f54 414c 0700 0000 1949 6e63  ...TOTAL.....Inc
+00006b30: 6f6d 6553 7065 6e64 696e 6752 6570 6f72  omeSpendingRepor
+00006b40: 744d 6f64 656c 0103 0000 000e 0412 0430  tModel.........0
+00006b50: 043b 044e 0442 0430 003a 0800 0000 0006  .;.N.B.0.:......
+00006b60: 0000 0009 4375 7272 656e 6379 3a07 0000  ....Currency:...
+00006b70: 001a 496e 636f 6d65 5370 656e 6469 6e67  ..IncomeSpending
+00006b80: 5265 706f 7274 5769 6467 6574 0103 0000  ReportWidget....
+00006b90: 001c 0414 043e 0445 043e 0434 044b 0020  .....>.E.>.4.K. 
+00006ba0: 0438 0020 0422 0440 0430 0442 044b 0800  .8. .".@.0.B.K..
+00006bb0: 0000 0006 0000 0011 496e 636f 6d65 2026  ........Income &
+00006bc0: 2053 7065 6e64 696e 6707 0000 001a 496e   Spending.....In
+00006bd0: 636f 6d65 5370 656e 6469 6e67 5265 706f  comeSpendingRepo
+00006be0: 7274 5769 6467 6574 0103 0000 0018 0421  rtWidget.......!
+00006bf0: 043e 0445 0440 0430 043d 0438 0442 044c  .>.E.@.0.=.8.B.L
+00006c00: 002e 002e 002e 0800 0000 0006 0000 0007  ................
+00006c10: 5361 7665 2e2e 2e07 0000 001a 496e 636f  Save........Inco
+00006c20: 6d65 5370 656e 6469 6e67 5265 706f 7274  meSpendingReport
+00006c30: 5769 6467 6574 0103 0000 001c 0414 043e  Widget.........>
+00006c40: 0445 043e 0434 044b 0020 0438 0020 0422  .E.>.4.K. .8. ."
+00006c50: 0440 0430 0442 044b 0800 0000 0006 0000  .@.0.B.K........
+00006c60: 0011 496e 636f 6d65 2026 2053 7065 6e64  ..Income & Spend
+00006c70: 696e 6707 0000 001a 496e 636f 6d65 5370  ing.....IncomeSp
+00006c80: 656e 6469 6e67 5265 706f 7274 5769 6e64  endingReportWind
+00006c90: 6f77 0103 0000 0022 041f 043e 043a 0430  ow....."...>.:.0
+00006ca0: 0437 0430 0442 044c 0020 043e 043f 0435  .7.0.B.L. .>.?.5
+00006cb0: 0440 0430 0446 0438 0438 0800 0000 0006  .@.0.F.8.8......
+00006cc0: 0000 000f 5368 6f77 206f 7065 7261 7469  ....Show operati
+00006cd0: 6f6e 7307 0000 001a 496e 636f 6d65 5370  ons.....IncomeSp
+00006ce0: 656e 6469 6e67 5265 706f 7274 5769 6e64  endingReportWind
+00006cf0: 6f77 0103 0000 0008 0421 0447 0435 0442  ow.......!.G.5.B
+00006d00: 0800 0000 0006 0000 0007 4163 636f 756e  ..........Accoun
+00006d10: 7407 0000 0014 496e 636f 6d65 5370 656e  t.....IncomeSpen
+00006d20: 6469 6e67 5769 6467 6574 0103 0000 0032  dingWidget.....2
+00006d30: 0414 043e 0431 0430 0432 0438 0442 044c  ...>.1.0.2.8.B.L
+00006d40: 0020 0434 0435 0442 0430 043b 044c 043d  . .4.5.B.0.;.L.=
+00006d50: 0443 044e 0020 0437 0430 043f 0438 0441  .C.N. .7.0.?.8.A
+00006d60: 044c 0800 0000 0006 0000 000a 4164 6420  .L..........Add 
+00006d70: 6465 7461 696c 0700 0000 1449 6e63 6f6d  detail.....Incom
+00006d80: 6553 7065 6e64 696e 6757 6964 6765 7401  eSpendingWidget.
+00006d90: 0300 0000 3804 2104 3a04 3e04 3f04 3804  ....8.!.:.>.?.8.
+00006da0: 4004 3e04 3204 3004 4204 4c00 2004 3404  @.>.2.0.B.L. .4.
+00006db0: 3504 4204 3004 3b04 4c04 3d04 4304 4e00  5.B.0.;.L.=.C.N.
+00006dc0: 2004 3704 3004 3f04 3804 4104 4c08 0000   .7.0.?.8.A.L...
+00006dd0: 0000 0600 0000 0b43 6f70 7920 6465 7461  .......Copy deta
+00006de0: 696c 0700 0000 1449 6e63 6f6d 6553 7065  il.....IncomeSpe
+00006df0: 6e64 696e 6757 6964 6765 7401 0300 0000  ndingWidget.....
+00006e00: 1404 1404 3004 4204 3000 2f04 1204 4004  ....0.B.0./...@.
+00006e10: 3504 3c04 4f08 0000 0000 0600 0000 0944  5.<.O..........D
+00006e20: 6174 652f 5469 6d65 0700 0000 1449 6e63  ate/Time.....Inc
+00006e30: 6f6d 6553 7065 6e64 696e 6757 6964 6765  omeSpendingWidge
+00006e40: 7401 0300 0000 0c04 1404 3504 4204 3004  t.........5.B.0.
+00006e50: 3b04 3808 0000 0000 0600 0000 0744 6574  ;.8..........Det
+00006e60: 6169 6c73 0700 0000 1449 6e63 6f6d 6553  ails.....IncomeS
+00006e70: 7065 6e64 696e 6757 6964 6765 7401 0300  pendingWidget...
+00006e80: 0000 4404 1d04 3504 3204 3e04 3704 3c04  ..D...5.2.>.7.<.
+00006e90: 3e04 3604 3d04 3e00 2004 3404 3e04 3104  >.6.=.>. .4.>.1.
+00006ea0: 3004 3204 3804 4204 4c00 2004 3d04 3e04  0.2.8.B.L. .=.>.
+00006eb0: 3204 4304 4e00 2004 3704 3004 3f04 3804  2.C.N. .7.0.?.8.
+00006ec0: 4104 4c00 3a00 2008 0000 0000 0600 0000  A.L.:. .........
+00006ed0: 1a46 6169 6c65 6420 746f 2061 6464 206e  .Failed to add n
+00006ee0: 6577 2072 6563 6f72 643a 2007 0000 0014  ew record: .....
+00006ef0: 496e 636f 6d65 5370 656e 6469 6e67 5769  IncomeSpendingWi
+00006f00: 6467 6574 0103 0000 001c 0414 043e 0445  dget.........>.E
+00006f10: 043e 0434 0020 002f 0020 0420 0430 0441  .>.4. ./. . .0.A
+00006f20: 0445 043e 0434 0800 0000 0006 0000 0011  .E.>.4..........
+00006f30: 496e 636f 6d65 202f 2053 7065 6e64 696e  Income / Spendin
+00006f40: 6707 0000 0014 496e 636f 6d65 5370 656e  g.....IncomeSpen
+00006f50: 6469 6e67 5769 6467 6574 0103 0000 0014  dingWidget......
+00006f60: 041f 0440 0438 043c 0435 0447 0430 043d  ...@.8.<.5.G.0.=
+00006f70: 0438 0435 0800 0000 0006 0000 0004 4e6f  .8.5..........No
+00006f80: 7465 0700 0000 1449 6e63 6f6d 6553 7065  te.....IncomeSpe
+00006f90: 6e64 696e 6757 6964 6765 7401 0300 0000  ndingWidget.....
+00006fa0: 4804 1e04 4804 3804 3104 3a04 3000 2004  H...H.8.1.:.0. .
+00006fb0: 3f04 4004 3800 2004 3704 3004 3f04 3804  ?.@.8. .7.0.?.8.
+00006fc0: 4104 3800 2004 3404 3504 4204 3004 3b04  A.8. .4.5.B.0.;.
+00006fd0: 3504 3900 2004 3e04 3f04 3504 4004 3004  5.9. .>.?.5.@.0.
+00006fe0: 4604 3804 3800 3a00 2008 0000 0000 0600  F.8.8.:. .......
+00006ff0: 0000 214f 7065 7261 7469 6f6e 2064 6574  ..!Operation det
+00007000: 6169 6c73 2073 7562 6d69 7420 6661 696c  ails submit fail
+00007010: 6564 3a20 0700 0000 1449 6e63 6f6d 6553  ed: .....IncomeS
+00007020: 7065 6e64 696e 6757 6964 6765 7401 0300  pendingWidget...
+00007030: 0000 3804 1e04 4804 3804 3104 3a04 3000  ..8...H.8.1.:.0.
+00007040: 2004 3f04 4004 3800 2004 3704 3004 3f04   .?.@.8. .7.0.?.
+00007050: 3804 4104 3800 2004 3e04 3f04 3504 4004  8.A.8. .>.?.5.@.
+00007060: 3004 4604 3804 3800 3a00 2008 0000 0000  0.F.8.8.:. .....
+00007070: 0600 0000 194f 7065 7261 7469 6f6e 2073  .....Operation s
+00007080: 7562 6d69 7420 6661 696c 6564 3a20 0700  ubmit failed: ..
+00007090: 0000 1449 6e63 6f6d 6553 7065 6e64 696e  ...IncomeSpendin
+000070a0: 6757 6964 6765 7401 0300 0000 2004 1e04  gWidget..... ...
+000070b0: 3f04 3b04 3004 4204 3000 2004 3200 2004  ?.;.0.B.0. .2. .
+000070c0: 3204 3004 3b04 4e04 4204 3500 3a08 0000  2.0.;.N.B.5.:...
+000070d0: 0000 0600 0000 1950 6169 6420 696e 2066  .......Paid in f
+000070e0: 6f72 6569 676e 2063 7572 7265 6e63 793a  oreign currency:
+000070f0: 0700 0000 1449 6e63 6f6d 6553 7065 6e64  .....IncomeSpend
+00007100: 696e 6757 6964 6765 7401 0300 0000 1404  ingWidget.......
+00007110: 1a04 3e04 3d04 4204 4004 3004 3304 3504  ..>.=.B.@.0.3.5.
+00007120: 3d04 4208 0000 0000 0600 0000 0450 6565  =.B..........Pee
+00007130: 7207 0000 0014 496e 636f 6d65 5370 656e  r.....IncomeSpen
+00007140: 6469 6e67 5769 6467 6574 0103 0000 0030  dingWidget.....0
+00007150: 0423 0434 0430 043b 0438 0442 044c 0020  .#.4.0.;.8.B.L. 
+00007160: 0434 0435 0442 0430 043b 044c 043d 0443  .4.5.B.0.;.L.=.C
+00007170: 044e 0020 0437 0430 043f 0438 0441 044c  .N. .7.0.?.8.A.L
+00007180: 0800 0000 0006 0000 000d 5265 6d6f 7665  ..........Remove
+00007190: 2064 6574 6169 6c07 0000 0014 496e 636f   detail.....Inco
+000071a0: 6d65 5370 656e 6469 6e67 5769 6467 6574  meSpendingWidget
+000071b0: 0103 0000 000c 0026 0421 0447 0435 0442  .......&.!.G.5.B
+000071c0: 0430 0800 0000 0006 0000 0009 2641 6363  .0..........&Acc
+000071d0: 6f75 6e74 7307 0000 000e 4a41 4c5f 4d61  ounts.....JAL_Ma
+000071e0: 696e 5769 6e64 6f77 0103 0000 0012 0026  inWindow.......&
+000071f0: 0411 044d 043a 0430 043f 002e 002e 002e  ...M.:.0.?......
+00007200: 0800 0000 0006 0000 000a 2642 6163 6b75  ..........&Backu
+00007210: 702e 2e2e 0700 0000 0e4a 414c 5f4d 6169  p........JAL_Mai
+00007220: 6e57 696e 646f 7701 0300 0000 1e00 2604  nWindow.......&.
+00007230: 1104 3004 3704 3e04 3204 3004 4f00 2004  ..0.7.>.2.0.O. .
+00007240: 3204 3004 3b04 4e04 4204 3008 0000 0000  2.0.;.N.B.0.....
+00007250: 0600 0000 0e26 4261 7365 2043 7572 7265  .....&Base Curre
+00007260: 6e63 7907 0000 000e 4a41 4c5f 4d61 696e  ncy.....JAL_Main
+00007270: 5769 6e64 6f77 0103 0000 0014 0026 041a  Window.......&..
+00007280: 0430 0442 0435 0433 043e 0440 0438 0438  .0.B.5.3.>.@.8.8
+00007290: 0800 0000 0006 0000 000b 2643 6174 6567  ..........&Categ
+000072a0: 6f72 6965 7307 0000 000e 4a41 4c5f 4d61  ories.....JAL_Ma
+000072b0: 696e 5769 6e64 6f77 0103 0000 000e 0026  inWindow.......&
+000072c0: 0414 0430 043d 043d 044b 0435 0800 0000  ...0.=.=.K.5....
+000072d0: 0006 0000 0005 2644 6174 6107 0000 000e  ......&Data.....
+000072e0: 4a41 4c5f 4d61 696e 5769 6e64 6f77 0103  JAL_MainWindow..
+000072f0: 0000 000c 0026 0412 044b 0445 043e 0434  .....&...K.E.>.4
+00007300: 0800 0000 0006 0000 0005 2645 7869 7407  ..........&Exit.
+00007310: 0000 000e 4a41 4c5f 4d61 696e 5769 6e64  ....JAL_MainWind
+00007320: 6f77 0103 0000 0010 0026 042d 043a 0441  ow.......&.-.:.A
+00007330: 043f 043e 0440 0442 0800 0000 0006 0000  .?.>.@.B........
+00007340: 0007 2645 7870 6f72 7407 0000 000e 4a41  ..&Export.....JA
+00007350: 4c5f 4d61 696e 5769 6e64 6f77 0103 0000  L_MainWindow....
+00007360: 000e 0026 0418 043c 043f 043e 0440 0442  ...&...<.?.>.@.B
+00007370: 0800 0000 0006 0000 0007 2649 6d70 6f72  ..........&Impor
+00007380: 7407 0000 000e 4a41 4c5f 4d61 696e 5769  t.....JAL_MainWi
+00007390: 6e64 6f77 0103 0000 0012 0026 041e 0441  ndow.......&...A
+000073a0: 043d 043e 0432 043d 043e 0435 0800 0000  .=.>.2.=.>.5....
+000073b0: 0006 0000 0005 264d 6169 6e07 0000 000e  ......&Main.....
+000073c0: 4a41 4c5f 4d61 696e 5769 6e64 6f77 0103  JAL_MainWindow..
+000073d0: 0000 0012 0026 041e 043f 0435 0440 0430  .....&...?.5.@.0
+000073e0: 0446 0438 0438 0800 0000 0006 0000 000b  .F.8.8..........
+000073f0: 264f 7065 7261 7469 6f6e 7307 0000 000e  &Operations.....
+00007400: 4a41 4c5f 4d61 696e 5769 6e64 6f77 0103  JAL_MainWindow..
+00007410: 0000 0018 041a 0026 043e 043d 0442 0440  .......&.>.=.B.@
+00007420: 0430 0433 0435 043d 0442 044b 0800 0000  .0.3.5.=.B.K....
+00007430: 0006 0000 0006 2650 6565 7273 0700 0000  ......&Peers....
+00007440: 0e4a 414c 5f4d 6169 6e57 696e 646f 7701  .JAL_MainWindow.
+00007450: 0300 0000 1400 2604 1a04 3e04 4204 3804  ......&...>.B.8.
+00007460: 4004 3e04 3204 3a04 3808 0000 0000 0600  @.>.2.:.8.......
+00007470: 0000 0726 5175 6f74 6573 0700 0000 0e4a  ...&Quotes.....J
+00007480: 414c 5f4d 6169 6e57 696e 646f 7701 0300  AL_MainWindow...
+00007490: 0000 1a00 2604 1a04 3e04 4204 3804 4004  ....&...>.B.8.@.
+000074a0: 3e04 3204 3a04 3800 2e00 2e00 2e08 0000  >.2.:.8.........
+000074b0: 0000 0600 0000 0a26 5175 6f74 6573 2e2e  .......&Quotes..
+000074c0: 2e07 0000 000e 4a41 4c5f 4d61 696e 5769  ......JAL_MainWi
+000074d0: 6e64 6f77 0103 0000 000e 0026 041e 0442  ndow.......&...B
+000074e0: 0447 0435 0442 044b 0800 0000 0006 0000  .G.5.B.K........
+000074f0: 0008 2652 6570 6f72 7473 0700 0000 0e4a  ..&Reports.....J
+00007500: 414c 5f4d 6169 6e57 696e 646f 7701 0300  AL_MainWindow...
+00007510: 0000 2400 2604 1204 3e04 4104 4104 4204  ..$.&...>.A.A.B.
+00007520: 3004 3d04 3e04 3204 3b04 3504 3d04 3804  0.=.>.2.;.5.=.8.
+00007530: 3500 2e00 2e00 2e08 0000 0000 0600 0000  5...............
+00007540: 0b26 5265 7374 6f72 652e 2e2e 0700 0000  .&Restore.......
+00007550: 0e4a 414c 5f4d 6169 6e57 696e 646f 7701  .JAL_MainWindow.
+00007560: 0300 0000 0c00 2604 1e04 4204 4704 5104  ......&...B.G.Q.
+00007570: 4208 0000 0000 0600 0000 0a26 5374 6174  B..........&Stat
+00007580: 656d 656e 7407 0000 000e 4a41 4c5f 4d61  ement.....JAL_Ma
+00007590: 696e 5769 6e64 6f77 0103 0000 000a 0026  inWindow.......&
+000075a0: 0422 044d 0433 0438 0800 0000 0006 0000  .".M.3.8........
+000075b0: 0005 2654 6167 7307 0000 000e 4a41 4c5f  ..&Tags.....JAL_
+000075c0: 4d61 696e 5769 6e64 6f77 0103 0000 001c  MainWindow......
+000075d0: 0026 0426 0435 043d 043d 044b 0435 0020  .&.&.5.=.=.K.5. 
+000075e0: 0431 0443 043c 0430 0433 0438 0800 0000  .1.C.<.0.3.8....
+000075f0: 0006 0000 0007 4126 7373 6574 7307 0000  ......A&ssets...
+00007600: 000e 4a41 4c5f 4d61 696e 5769 6e64 6f77  ..JAL_MainWindow
+00007610: 0103 0000 004e 041e 0442 0447 0435 0442  .....N...B.G.5.B
+00007620: 0020 043e 0020 0026 0434 0432 0438 0436  . .>. .&.4.2.8.6
+00007630: 0435 043d 0438 044f 0445 0020 043f 043e  .5.=.8.O.E. .?.>
+00007640: 0020 0437 0430 0440 0443 0431 0435 0436  . .7.0.@.C.1.5.6
+00007650: 043d 044b 043c 0020 0441 0447 0435 0442  .=.K.<. .A.G.5.B
+00007660: 0430 043c 0800 0000 0006 0000 001d 466f  .0.<..........Fo
+00007670: 7265 6967 6e20 6163 636f 756e 7473 2026  reign accounts &
+00007680: 666c 6f77 2072 6570 6f72 7407 0000 000e  flow report.....
+00007690: 4a41 4c5f 4d61 696e 5769 6e64 6f77 0103  JAL_MainWindow..
+000076a0: 0000 003e 0418 043d 0432 0435 0441 0442  ...>...=.2.5.A.B
+000076b0: 0438 0446 0438 043e 043d 043d 044b 0439  .8.F.8.>.=.=.K.9
+000076c0: 0020 0026 043d 0430 043b 043e 0433 043e  . .&.=.0.;.>.3.>
+000076d0: 0432 044b 0439 0020 043e 0442 0447 0435  .2.K.9. .>.B.G.5
+000076e0: 0442 0800 0000 0006 0000 0016 496e 7665  .B..........Inve
+000076f0: 7374 6d65 6e74 2026 7461 7820 7265 706f  stment &tax repo
+00007700: 7274 0700 0000 0e4a 414c 5f4d 6169 6e57  rt.....JAL_MainW
+00007710: 696e 646f 7701 0300 0000 0a00 2604 2f04  indow.......&./.
+00007720: 3704 4b04 3a08 0000 0000 0600 0000 094c  7.K.:..........L
+00007730: 2661 6e67 7561 6765 0700 0000 0e4a 414c  &anguage.....JAL
+00007740: 5f4d 6169 6e57 696e 646f 7701 0300 0000  _MainWindow.....
+00007750: 2a04 1f04 3504 4004 3504 4104 4704 3804  *...5.@.5.A.G.8.
+00007760: 4204 3004 4204 4c00 2000 2604 3804 4204  B.0.B.L. .&.8.B.
+00007770: 3e04 3304 3800 2e00 2e00 2e08 0000 0000  >.3.8...........
+00007780: 0600 0000 1352 652d 6275 696c 6420 264c  .....Re-build &L
+00007790: 6564 6765 722e 2e2e 0700 0000 0e4a 414c  edger........JAL
+000077a0: 5f4d 6169 6e57 696e 646f 7701 0300 0000  _MainWindow.....
+000077b0: 1604 2704 3504 3a00 2000 5b00 5200 5500  ..'.5.:. .[.R.U.
+000077c0: 5d00 2e00 2e00 2e08 0000 0000 0600 0000  ]...............
+000077d0: 0c53 6c69 7020 5b52 555d 2e2e 2e07 0000  .Slip [RU]......
+000077e0: 000e 4a41 4c5f 4d61 696e 5769 6e64 6f77  ..JAL_MainWindow
+000077f0: 0103 0000 0006 006a 0061 006c 0800 0000  .......j.a.l....
+00007800: 0006 0000 0003 6a61 6c07 0000 000e 4a41  ......jal.....JA
+00007810: 4c5f 4d61 696e 5769 6e64 6f77 0103 0000  L_MainWindow....
+00007820: 0020 0411 0430 043d 043a 0020 0434 043b  . ...0.=.:. .4.;
+00007830: 044f 0020 0441 0447 0435 0442 0430 0020  .O. .A.G.5.B.0. 
+00007840: 2116 0800 0000 0006 0000 0012 4261 6e6b  !...........Bank
+00007850: 2066 6f72 2061 6363 6f75 6e74 2023 0700   for account #..
+00007860: 0000 0a4a 616c 4163 636f 756e 7401 0300  ...JalAccount...
+00007870: 0000 2a04 2104 4204 4004 3004 3d04 3000  ..*.!.B.@.0.=.0.
+00007880: 2004 3e04 3104 3d04 3e04 3204 3b04 5104   .>.1.=.>.2.;.Q.
+00007890: 3d04 3000 2004 3404 3b04 4f00 2008 0000  =.0. .4.;.O. ...
+000078a0: 0000 0600 0000 1443 6f75 6e74 7279 2075  .......Country u
+000078b0: 7064 6174 6564 2066 6f72 2007 0000 0008  pdated for .....
+000078c0: 4a61 6c41 7373 6574 0103 0000 002a 041a  JalAsset.....*..
+000078d0: 043e 0442 0438 0440 043e 0432 043a 0438  .>.B.8.@.>.2.:.8
+000078e0: 0020 043e 0431 043d 043e 0432 043b 0435  . .>.1.=.>.2.;.5
+000078f0: 043d 044b 003a 0020 0800 0000 0006 0000  .=.K.:. ........
+00007900: 0019 5175 6f74 6174 696f 6e73 2077 6572  ..Quotations wer
+00007910: 6520 7570 6461 7465 643a 2007 0000 0008  e updated: .....
+00007920: 4a61 6c41 7373 6574 0103 0000 0046 0420  JalAsset.....F. 
+00007930: 0435 0433 0438 0441 0442 0440 0430 0446  .5.3.8.A.B.@.0.F
+00007940: 0438 043e 043d 043d 044b 0439 0020 043d  .8.>.=.=.K.9. .=
+00007950: 043e 043c 0435 0440 0020 043e 0431 043d  .>.<.5.@. .>.1.=
+00007960: 043e 0432 043b 0451 043d 0020 0434 043b  .>.2.;.Q.=. .4.;
+00007970: 044f 0020 0800 0000 0006 0000 0017 5265  .O. ..........Re
+00007980: 672e 6e75 6d62 6572 2075 7064 6174 6564  g.number updated
+00007990: 2066 6f72 2007 0000 0008 4a61 6c41 7373   for .....JalAss
+000079a0: 6574 0103 0000 0030 041d 0435 0442 0020  et.....0...5.B. 
+000079b0: 043a 043e 0442 0438 0440 043e 0432 043a  .:.>.B.8.@.>.2.:
+000079c0: 0438 002f 043a 0443 0440 0441 0430 0020  .8./.:.C.@.A.0. 
+000079d0: 0434 043b 044f 0020 0800 0000 0006 0000  .4.;.O. ........
+000079e0: 001c 5468 6572 6520 6172 6520 6e6f 2071  ..There are no q
+000079f0: 756f 7465 2f72 6174 6520 666f 7220 0700  uote/rate for ..
+00007a00: 0000 084a 616c 4173 7365 7401 0300 0000  ...JalAsset.....
+00007a10: 4c04 1d04 3504 3e04 3604 3804 3404 3004  L...5.>.6.8.4.0.
+00007a20: 3d04 3d04 3004 4f00 2004 3f04 3e04 3f04  =.=.0.O. .?.>.?.
+00007a30: 4b04 4204 3a04 3000 2004 3e04 3104 3d04  K.B.:.0. .>.1.=.
+00007a40: 3e04 3204 3804 4204 4c00 2000 4900 5300  >.2.8.B.L. .I.S.
+00007a50: 4900 4e00 2004 3404 3b04 4f00 2008 0000  I.N. .4.;.O. ...
+00007a60: 0000 0600 0000 2655 6e65 7870 6563 7465  ......&Unexpecte
+00007a70: 6420 6174 7465 6d70 7420 746f 2075 7064  d attempt to upd
+00007a80: 6174 6520 4953 494e 2066 6f72 2007 0000  ate ISIN for ...
+00007a90: 0008 4a61 6c41 7373 6574 0103 0000 0006  ..JalAsset......
+00007aa0: 0020 0432 0020 0800 0000 0006 0000 0006  . .2. ..........
+00007ab0: 2069 6e74 6f20 0700 0000 094a 616c 4261   into .....JalBa
+00007ac0: 636b 7570 0103 0000 001c 0410 0440 0445  ckup.........@.E
+00007ad0: 0438 0432 044b 0020 0028 002a 002e 0074  .8.2.K. .(.*...t
+00007ae0: 0067 007a 0029 0800 0000 0006 0000 0010  .g.z.)..........
+00007af0: 4172 6368 6976 6573 2028 2a2e 7467 7a29  Archives (*.tgz)
+00007b00: 0700 0000 094a 616c 4261 636b 7570 0103  .....JalBackup..
+00007b10: 0000 0046 041d 0435 0020 0440 0430 0441  ...F...5. .@.0.A
+00007b20: 043f 043e 0437 043d 0430 043d 0430 0020  .?.>.7.=.0.=.0. 
+00007b30: 043c 0435 0442 043a 0430 0020 0440 0435  .<.5.B.:.0. .@.5
+00007b40: 0437 0435 0440 0432 043d 043e 0439 0020  .7.5.@.2.=.>.9. 
+00007b50: 043a 043e 043f 0438 0438 0800 0000 0006  .:.>.?.8.8......
+00007b60: 0000 001b 4261 636b 7570 206c 6162 656c  ....Backup label
+00007b70: 206e 6f74 2072 6563 6f67 6e69 7a65 6407   not recognized.
+00007b80: 0000 0009 4a61 6c42 6163 6b75 7001 0300  ....JalBackup...
+00007b90: 0000 4604 2004 3504 3704 3504 4004 3204  ..F. .5.7.5.@.2.
+00007ba0: 3d04 3004 4f00 2004 3a04 3e04 3f04 3804  =.0.O. .:.>.?.8.
+00007bb0: 4f00 2004 3204 3e04 4104 4104 4204 3004  O. .2.>.A.A.B.0.
+00007bc0: 3204 3d04 3e04 3204 3b04 3504 3d04 3000  2.=.>.2.;.5.=.0.
+00007bd0: 2004 3804 3700 3a00 2008 0000 0000 0600   .8.7.:. .......
+00007be0: 0000 1642 6163 6b75 7020 7265 7374 6f72  ...Backup restor
+00007bf0: 6564 2066 726f 6d3a 2007 0000 0009 4a61  ed from: .....Ja
+00007c00: 6c42 6163 6b75 7001 0300 0000 3a04 2004  lBackup.....:. .
+00007c10: 3504 3704 3504 4004 3204 3d04 3004 4f00  5.7.5.@.2.=.0.O.
+00007c20: 2004 3a04 3e04 3f04 3804 4f00 2004 4104   .:.>.?.8.O. .A.
+00007c30: 3e04 4504 4004 3004 3d04 5104 3d04 3000  >.E.@.0.=.Q.=.0.
+00007c40: 2004 3200 3a00 2008 0000 0000 0600 0000   .2.:. .........
+00007c50: 1142 6163 6b75 7020 7361 7665 6420 696e  .Backup saved in
+00007c60: 3a20 0700 0000 094a 616c 4261 636b 7570  : .....JalBackup
+00007c70: 0103 0000 0052 041d 0435 0432 043e 0437  .....R...5.2.>.7
+00007c80: 043c 043e 0436 043d 043e 0020 043f 0440  .<.>.6.=.>. .?.@
+00007c90: 043e 0432 0435 0440 0438 0442 044c 0020  .>.2.5.@.8.B.L. 
+00007ca0: 0434 0430 0442 0443 0020 0440 0435 0437  .4.0.B.C. .@.5.7
+00007cb0: 0435 0440 0432 043d 043e 0439 0020 043a  .5.@.2.=.>.9. .:
+00007cc0: 043e 043f 0438 0438 0800 0000 0006 0000  .>.?.8.8........
+00007cd0: 001a 4361 6e27 7420 7661 6c69 6461 7465  ..Can't validate
+00007ce0: 2062 6163 6b75 7020 6461 7465 0700 0000   backup date....
+00007cf0: 094a 616c 4261 636b 7570 0103 0000 0028  .JalBackup.....(
+00007d00: 0414 0430 043d 043d 044b 0435 0020 0432  ...0.=.=.K.5. .2
+00007d10: 043e 0441 0441 0442 0430 043d 043e 0432  .>.A.A.B.0.=.>.2
+00007d20: 043b 0435 043d 044b 0800 0000 0006 0000  .;.5.=.K........
+00007d30: 000d 4461 7461 2072 6573 746f 7265 6407  ..Data restored.
+00007d40: 0000 0009 4a61 6c42 6163 6b75 7001 0300  ....JalBackup...
+00007d50: 0000 4204 1404 3004 3d04 3d04 4b04 3500  ..B...0.=.=.K.5.
+00007d60: 2004 3104 4b04 3b04 3800 2004 3704 3004   .1.K.;.8. .7.0.
+00007d70: 3304 4004 4304 3604 3504 3d04 4b00 2004  3.@.C.6.5.=.K. .
+00007d80: 3804 3700 2004 3104 4d04 3a04 3004 3f04  8.7. .1.M.:.0.?.
+00007d90: 3000 2e00 0a08 0000 0000 0600 0000 2544  0.............%D
+00007da0: 6174 6162 6173 6520 7761 7320 6c6f 6164  atabase was load
+00007db0: 6564 2066 726f 6d20 7468 6520 6261 636b  ed from the back
+00007dc0: 7570 2e0a 0700 0000 094a 616c 4261 636b  up.......JalBack
+00007dd0: 7570 0103 0000 004e 041d 0435 0020 0443  up.....N...5. .C
+00007de0: 0434 0430 043b 043e 0441 044c 0020 0432  .4.0.;.>.A.L. .2
+00007df0: 043e 0441 0441 0442 0430 043d 043e 0432  .>.A.A.B.0.=.>.2
+00007e00: 0438 0442 044c 0020 0440 0435 0437 0435  .8.B.L. .@.5.7.5
+00007e10: 0440 0432 043d 0443 044e 0020 043a 043e  .@.2.=.C.N. .:.>
+00007e20: 043f 0438 044e 0800 0000 0006 0000 001d  .?.8.N..........
+00007e30: 4661 696c 6564 2074 6f20 7265 7374 6f72  Failed to restor
+00007e40: 6520 6261 636b 7570 2066 696c 6507 0000  e backup file...
+00007e50: 0009 4a61 6c42 6163 6b75 7001 0300 0000  ..JalBackup.....
+00007e60: 3804 2104 3e04 4504 4004 3004 3d04 3804  8.!.>.E.@.0.=.8.
+00007e70: 4204 4c00 2004 4004 3504 3704 3504 4004  B.L. .@.5.7.5.@.
+00007e80: 3204 3d04 4304 4e00 2004 3a04 3e04 3f04  2.=.C.N. .:.>.?.
+00007e90: 3804 4e00 2004 3200 3a08 0000 0000 0600  8.N. .2.:.......
+00007ea0: 0000 0f53 6176 6520 6261 636b 7570 2074  ...Save backup t
+00007eb0: 6f3a 0700 0000 094a 616c 4261 636b 7570  o:.....JalBackup
+00007ec0: 0103 0000 0040 0412 044b 0431 0435 0440  .....@...K.1.5.@
+00007ed0: 0438 0442 0435 0020 0444 0430 0439 043b  .8.B.5. .D.0.9.;
+00007ee0: 0020 0441 0020 0440 0435 0437 0435 0440  . .A. .@.5.7.5.@
+00007ef0: 0432 043d 043e 0439 0020 043a 043e 043f  .2.=.>.9. .:.>.?
+00007f00: 0438 0435 0439 0800 0000 0006 0000 0017  .8.5.9..........
+00007f10: 5365 6c65 6374 2066 696c 6520 7769 7468  Select file with
+00007f20: 2062 6163 6b75 7007 0000 0009 4a61 6c42   backup.....JalB
+00007f30: 6163 6b75 7001 0300 0000 4a04 1d04 3504  ackup.....J...5.
+00007f40: 3204 3504 4004 3d04 4b04 3900 2004 4404  2.5.@.=.K.9. .D.
+00007f50: 3e04 4004 3c04 3004 4200 2004 4404 3004  >.@.<.0.B. .D.0.
+00007f60: 3904 3b04 3000 2004 4004 3504 3704 3504  9.;.0. .@.5.7.5.
+00007f70: 4004 3204 3d04 3e04 3900 2004 3a04 3e04  @.2.=.>.9. .:.>.
+00007f80: 3f04 3804 3808 0000 0000 0600 0000 1b57  ?.8.8..........W
+00007f90: 726f 6e67 2066 6f72 6d61 7420 6f66 2062  rong format of b
+00007fa0: 6163 6b75 7020 6669 6c65 0700 0000 094a  ackup file.....J
+00007fb0: 616c 4261 636b 7570 0103 0000 00c8 0412  alBackup........
+00007fc0: 044b 0020 0434 043e 043b 0436 043d 044b  .K. .4.>.;.6.=.K
+00007fd0: 0020 043f 0435 0440 0435 0437 0430 043f  . .?.5.@.5.7.0.?
+00007fe0: 0443 0441 0442 0438 0442 044c 0020 043f  .C.A.B.8.B.L. .?
+00007ff0: 0440 0438 043b 043e 0436 0435 043d 0438  .@.8.;.>.6.5.=.8
+00008000: 0435 002c 0020 0447 0442 043e 0431 044b  .5.,. .G.B.>.1.K
+00008010: 0020 043f 0440 0438 043c 0435 043d 0438  . .?.@.8.<.5.=.8
+00008020: 0442 044c 0020 0438 0437 043c 0435 043d  .B.L. .8.7.<.5.=
+00008030: 0435 043d 0438 044f 000a 041f 0440 0438  .5.=.8.O.....@.8
+00008040: 043b 043e 0436 0435 043d 0438 0435 0020  .;.>.6.5.=.8.5. 
+00008050: 0441 0435 0439 0447 0430 0441 0020 0437  .A.5.9.G.0.A. .7
+00008060: 0430 0432 0435 0440 0448 0438 0442 0020  .0.2.5.@.H.8.B. 
+00008070: 0441 0432 043e 044e 0020 0440 0430 0431  .A.2.>.N. .@.0.1
+00008080: 043e 0442 0443 0800 0000 0006 0000 0052  .>.B.C.........R
+00008090: 596f 7520 7368 6f75 6c64 2072 6573 7461  You should resta
+000080a0: 7274 2061 7070 6c69 6361 7469 6f6e 2074  rt application t
+000080b0: 6f20 6170 706c 7920 6368 616e 6765 730a  o apply changes.
+000080c0: 4170 706c 6963 6174 696f 6e20 7769 6c6c  Application will
+000080d0: 2062 6520 7465 726d 696e 6174 6564 206e   be terminated n
+000080e0: 6f77 0700 0000 094a 616c 4261 636b 7570  ow.....JalBackup
+000080f0: 0103 0000 0064 041e 043f 0435 0440 0430  .....d...?.5.@.0
+00008100: 0446 0438 044f 0020 0443 0436 0435 0020  .F.8.O. .C.6.5. 
+00008110: 0435 0441 0442 044c 0020 0432 0020 0431  .5.A.B.L. .2. .1
+00008120: 0430 0437 0435 0020 0434 0430 043d 043d  .0.7.5. .4.0.=.=
+00008130: 044b 0445 0020 0438 0020 0431 044b 043b  .K.E. .8. .1.K.;
+00008140: 0430 0020 043f 0440 043e 043f 0443 0449  .0. .?.@.>.?.C.I
+00008150: 0435 043d 0430 003a 0020 0800 0000 0006  .5.=.0.:. ......
+00008160: 0000 0031 4f70 6572 6174 696f 6e20 616c  ...1Operation al
+00008170: 7265 6164 7920 7072 6573 656e 7420 696e  ready present in
+00008180: 2064 6220 616e 6420 7761 7320 736b 6970   db and was skip
+00008190: 7065 643a 2007 0000 0005 4a61 6c44 4201  ped: .....JalDB.
+000081a0: 0300 0000 6e00 2004 3804 3c04 3504 3504  ....n. .8.<.5.5.
+000081b0: 4200 2004 3d04 3504 4104 3e04 4504 4004  B. .=.5.A.>.E.@.
+000081c0: 3004 3d04 5104 3d04 3d04 4b04 3500 2004  0.=.Q.=.=.K.5. .
+000081d0: 3804 3704 3c04 3504 3d04 3504 3d04 3804  8.7.<.5.=.5.=.8.
+000081e0: 4f00 2c00 0a04 3204 4b00 2004 4504 3e04  O.,...2.K. .E.>.
+000081f0: 4204 3804 4204 3500 2004 3804 4500 2004  B.8.B.5. .8.E. .
+00008200: 4104 3e04 4504 4004 3004 3d04 3804 4204  A.>.E.@.0.=.8.B.
+00008210: 4c00 3f08 0000 0000 0600 0000 3120 6861  L.?.........1 ha
+00008220: 7320 756e 636f 6d6d 6974 7465 6420 6368  s uncommitted ch
+00008230: 616e 6765 732c 0a64 6f20 796f 7520 7761  anges,.do you wa
+00008240: 6e74 2074 6f20 7361 7665 2069 743f 0700  nt to save it?..
+00008250: 0000 114a 616c 4f70 6572 6174 696f 6e73  ...JalOperations
+00008260: 5461 6273 0103 0000 0036 0415 0441 0442  Tabs.....6...A.B
+00008270: 044c 0020 043d 0435 0441 043e 0445 0440  .L. .=.5.A.>.E.@
+00008280: 0430 043d 0451 043d 043d 044b 0435 0020  .0.=.Q.=.=.K.5. 
+00008290: 0438 0437 043c 0435 043d 043d 0438 044f  .8.7.<.5.=.=.8.O
+000082a0: 0800 0000 0006 0000 0018 596f 7520 6861  ..........You ha
+000082b0: 7665 2075 6e73 6176 6564 2063 6861 6e67  ve unsaved chang
+000082c0: 6573 0700 0000 114a 616c 4f70 6572 6174  es.....JalOperat
+000082d0: 696f 6e73 5461 6273 0103 0000 005a 041d  ionsTabs.....Z..
+000082e0: 0435 0432 043e 0437 043c 043e 0436 043d  .5.2.>.7.<.>.6.=
+000082f0: 043e 0020 0443 0434 0430 043b 0438 0442  .>. .C.4.0.;.8.B
+00008300: 044c 0020 043f 0440 0435 0434 043e 043f  .L. .?.@.5.4.>.?
+00008310: 0440 0435 0434 0435 043b 0451 043d 043d  .@.5.4.5.;.Q.=.=
+00008320: 0443 044e 0020 043a 0430 0442 0435 0433  .C.N. .:.0.B.5.3
+00008330: 043e 0440 0438 044e 0800 0000 0006 0000  .>.@.8.N........
+00008340: 0020 4361 6e27 7420 6465 6c65 7465 2070  . Can't delete p
+00008350: 7265 6465 6669 6e65 6420 6361 7465 676f  redefined catego
+00008360: 7279 0700 0000 0b4a 616c 5371 6c45 7272  ry.....JalSqlErr
+00008370: 6f72 0103 0000 009e 042d 0442 0438 0020  or.......-.B.8. 
+00008380: 0434 0430 043d 043d 044b 0435 0020 043d  .4.0.=.=.K.5. .=
+00008390: 0435 0020 043c 043e 0433 0443 0442 0020  .5. .<.>.3.C.B. 
+000083a0: 0431 044b 0442 044c 0020 043c 043e 0434  .1.K.B.L. .<.>.4
+000083b0: 0438 0444 0438 0446 0438 0440 043e 0432  .8.D.8.F.8.@.>.2
+000083c0: 0430 043d 044b 002c 0020 0442 002e 043a  .0.=.K.,. .B...:
+000083d0: 002e 0020 043d 0430 0020 043d 0438 0445  ... .=.0. .=.8.E
+000083e0: 0020 0435 0441 0442 044c 0020 0441 0441  . .5.A.B.L. .A.A
+000083f0: 044b 043b 043a 0430 0020 0432 0020 0434  .K.;.:.0. .2. .4
+00008400: 0440 0443 0433 043e 043c 0020 043c 0435  .@.C.3.>.<. .<.5
+00008410: 0441 0442 0435 0800 0000 0006 0000 003a  .A.B.5.........:
+00008420: 4461 7461 2061 7265 2072 6566 6572 656e  Data are referen
+00008430: 6365 6420 696e 2061 6e6f 7468 6572 2070  ced in another p
+00008440: 6c61 6365 2061 6e64 2063 616e 2774 2062  lace and can't b
+00008450: 6520 6d6f 6469 6669 6564 0700 0000 0b4a  e modified.....J
+00008460: 616c 5371 6c45 7272 6f72 0103 0000 001e  alSqlError......
+00008470: 041e 0448 0438 0431 043a 0430 0020 0432  ...H.8.1.:.0. .2
+00008480: 0020 0434 0430 043d 043d 044b 0445 0800  . .4.0.=.=.K.E..
+00008490: 0000 0006 0000 000e 4461 7461 6261 7365  ........Database
+000084a0: 2065 7272 6f72 0700 0000 0b4a 616c 5371   error.....JalSq
+000084b0: 6c45 7272 6f72 0103 0000 0050 041d 0435  lError.....P...5
+000084c0: 0432 0435 0440 043d 043e 0020 0432 044b  .2.5.@.=.>. .2.K
+000084d0: 0431 0440 0430 043d 0430 0020 0432 0430  .1.@.0.=.0. .2.0
+000084e0: 043b 044e 0442 0430 0020 0434 043b 044f  .;.N.B.0. .4.;.O
+000084f0: 0020 0446 0435 043d 043d 043e 0439 0020  . .F.5.=.=.>.9. 
+00008500: 0431 0443 043c 0430 0433 0438 0800 0000  .1.C.<.0.3.8....
+00008510: 0006 0000 002a 496e 636f 7272 6563 7420  .....*Incorrect 
+00008520: 6375 7272 656e 6379 2061 7373 6967 6e6d  currency assignm
+00008530: 656e 7420 666f 7220 616e 2061 7373 6574  ent for an asset
+00008540: 0700 0000 0b4a 616c 5371 6c45 7272 6f72  .....JalSqlError
+00008550: 0103 0000 0080 041f 043e 043b 0435 0020  .........>.;.5. 
+00008560: 0411 0430 043d 043a 002f 0411 0440 043e  ...0.=.:./...@.>
+00008570: 043a 0435 0440 0020 0434 043e 043b 0436  .:.5.@. .4.>.;.6
+00008580: 043d 043e 0020 0431 044b 0442 044c 0020  .=.>. .1.K.B.L. 
+00008590: 0437 0430 043f 043e 043b 043d 0435 043d  .7.0.?.>.;.=.5.=
+000085a0: 043e 0020 0434 043b 044f 0020 0438 043d  .>. .4.;.O. .8.=
+000085b0: 0432 0435 0441 0442 0438 0446 0438 043e  .2.5.A.B.8.F.8.>
+000085c0: 043d 043d 043e 0433 043e 0020 0441 0447  .=.=.>.3.>. .A.G
+000085d0: 0435 0442 0430 0800 0000 0006 0000 0039  .5.B.0.........9
+000085e0: 496e 7665 7374 6d65 6e74 2061 6363 6f75  Investment accou
+000085f0: 6e74 2073 686f 756c 6420 6861 7665 2061  nt should have a
+00008600: 7373 6f63 6961 7465 6420 6272 6f6b 6572  ssociated broker
+00008610: 2061 7373 6967 6e65 6407 0000 000b 4a61   assigned.....Ja
+00008620: 6c53 716c 4572 726f 7201 0300 0000 8800  lSqlError.......
+00008630: 2004 3e04 3f04 3504 4004 3004 4604 3804   .>.?.5.@.0.F.8.
+00008640: 3900 2004 4204 4004 3504 3104 4304 4e04  9. .B.@.5.1.C.N.
+00008650: 4200 2004 3f04 3504 4004 3504 4004 3004  B. .?.5.@.5.@.0.
+00008660: 4104 4704 3504 4204 3000 2e00 2004 1204  A.G.5.B.0... ...
+00008670: 4b00 2004 4504 3e04 3404 3804 4204 3500  K. .E.>.4.8.B.5.
+00008680: 2004 3204 4b04 3f04 3e04 3b04 3d04 3804   .2.K.?.>.;.=.8.
+00008690: 4204 4c00 2004 3504 3304 3e00 2004 3f04  B.L. .5.3.>. .?.
+000086a0: 4004 4f04 3c04 3e00 2004 4104 3504 3904  @.O.<.>. .A.5.9.
+000086b0: 4704 3004 4100 3f08 0000 0000 0600 0000  G.0.A.?.........
+000086c0: 3c20 6f70 6572 6174 696f 6e73 2072 6571  < operations req
+000086d0: 7569 7265 2072 6562 7569 6c64 2e20 446f  uire rebuild. Do
+000086e0: 2079 6f75 2077 616e 7420 746f 2064 6f20   you want to do 
+000086f0: 6974 2072 6967 6874 206e 6f77 3f07 0000  it right now?...
+00008700: 0006 4c65 6467 6572 0103 0000 0022 002c  ..Ledger.....".,
+00008710: 0020 043d 043e 0432 0430 044f 0020 0433  . .=.>.2.0.O. .3
+00008720: 0440 0430 043d 0438 0446 0430 003a 0020  .@.0.=.8.F.0.:. 
+00008730: 0800 0000 0006 0000 0010 2c20 6e65 7720  .........., new 
+00008740: 6672 6f6e 7469 6572 3a20 0700 0000 064c  frontier: .....L
+00008750: 6564 6765 7201 0300 0000 1a04 1f04 3e04  edger.........>.
+00008760: 3404 4204 3204 3504 4004 3604 3404 3504  4.B.2.5.@.6.4.5.
+00008770: 3d04 3804 3508 0000 0000 0600 0000 0c43  =.8.5..........C
+00008780: 6f6e 6669 726d 6174 696f 6e07 0000 0006  onfirmation.....
+00008790: 4c65 6467 6572 0103 0000 0094 041f 0440  Ledger.........@
+000087a0: 043e 0438 0437 043e 0448 043b 0430 0020  .>.8.7.>.H.;.0. 
+000087b0: 043e 0448 0438 0431 043a 0430 002e 0020  .>.H.8.1.:.0... 
+000087c0: 0420 0430 0441 0447 0451 0442 0020 0438  . .0.A.G.Q.B. .8
+000087d0: 0442 043e 0433 043e 0432 0020 043d 0435  .B.>.3.>.2. .=.5
+000087e0: 0020 043e 043a 043e 043d 0447 0435 043d  . .>.:.>.=.G.5.=
+000087f0: 002e 0020 041f 0440 043e 0432 0435 0440  ... ...@.>.2.5.@
+00008800: 044c 0442 0435 0020 0441 043e 043e 0431  .L.B.5. .A.>.>.1
+00008810: 0449 0435 043d 0438 044f 0020 043e 0431  .I.5.=.8.O. .>.1
+00008820: 0020 043e 0448 0438 0431 043a 0430 0445  . .>.H.8.1.:.0.E
+00008830: 0800 0000 0006 0000 004d 4578 6365 7074  .........MExcept
+00008840: 696f 6e20 6861 7070 656e 6564 2e20 4c65  ion happened. Le
+00008850: 6467 6572 2069 7320 696e 636f 6d70 6c65  dger is incomple
+00008860: 7465 2e20 506c 6561 7365 2063 6f72 7265  te. Please corre
+00008870: 6374 2065 7272 6f72 7320 6c69 7374 6564  ct errors listed
+00008880: 2069 6e20 6c6f 6707 0000 0006 4c65 6467   in log.....Ledg
+00008890: 6572 0103 0000 004a 0418 0442 043e 0433  er.....J...B.>.3
+000088a0: 0438 0020 0440 0430 0441 0441 0447 0438  .8. .@.0.A.A.G.8
+000088b0: 0442 0430 043d 044b 002e 0020 0417 0430  .B.0.=.K... ...0
+000088c0: 0442 0440 0430 0447 0435 043d 043d 043e  .B.@.0.G.5.=.=.>
+000088d0: 0435 0020 0432 0440 0435 043c 044f 003a  .5. .2.@.5.<.O.:
+000088e0: 0020 0800 0000 0006 0000 0022 4c65 6467  . ........."Ledg
+000088f0: 6572 2069 7320 636f 6d70 6c65 7465 2e20  er is complete. 
+00008900: 456c 6170 7365 6420 7469 6d65 3a20 0700  Elapsed time: ..
+00008910: 0000 064c 6564 6765 7201 0300 0000 2c04  ...Ledger.....,.
+00008920: 2204 4004 3004 3d04 3704 3004 3a04 4604  ".@.0.=.7.0.:.F.
+00008930: 3804 3800 2004 3e04 4204 4104 4304 4204  8.8. .>.B.A.C.B.
+00008940: 4104 4204 3204 4304 4e04 4208 0000 0000  A.B.2.C.N.B.....
+00008950: 0600 0000 0e4c 6567 6572 2069 7320 656d  .....Leger is em
+00008960: 7074 7907 0000 0006 4c65 6467 6572 0103  pty.....Ledger..
+00008970: 0000 0026 041d 0435 0020 0443 043a 0430  ...&...5. .C.:.0
+00008980: 0437 0430 043d 0430 0020 0426 0411 0020  .7.0.=.0. .&... 
+00008990: 0434 043b 044f 003a 0020 0800 0000 0006  .4.;.O.:. ......
+000089a0: 0000 0016 4e6f 2061 7373 6574 2064 6566  ....No asset def
+000089b0: 696e 6564 2066 6f72 3a20 0700 0000 064c  ined for: .....L
+000089c0: 6564 6765 7201 0300 0000 3404 1d04 4300  edger.....4...C.
+000089d0: 2004 4304 3a04 3004 3704 3004 3d04 3000   .C.:.0.7.0.=.0.
+000089e0: 2004 3a04 3004 4204 3504 3304 3e04 4004   .:.0.B.5.3.>.@.
+000089f0: 3804 4f00 2004 3404 3b04 4f00 3a00 2008  8.O. .4.;.O.:. .
+00008a00: 0000 0000 0600 0000 154e 6f20 6361 7465  .........No cate
+00008a10: 676f 7279 2073 6574 2066 6f72 3a20 0700  gory set for: ..
+00008a20: 0000 064c 6564 6765 7201 0300 0000 3404  ...Ledger.....4.
+00008a30: 1d04 3500 2004 4304 3a04 3004 3704 3004  ..5. .C.:.0.7.0.
+00008a40: 3d00 2004 3a04 3e04 3d04 4204 4004 3004  =. .:.>.=.B.@.0.
+00008a50: 3304 3504 3d04 4200 2004 3404 3b04 4f00  3.5.=.B. .4.;.O.
+00008a60: 3a00 2008 0000 0000 0600 0000 114e 6f20  :. ..........No 
+00008a70: 7065 6572 2073 6574 2066 6f72 3a20 0700  peer set for: ..
+00008a80: 0000 064c 6564 6765 7201 0300 0000 2604  ...Ledger.....&.
+00008a90: 1f04 3504 4004 3504 4104 4704 5104 4200  ..5.@.5.A.G.Q.B.
+00008aa0: 2004 3804 4204 3e04 3304 3e04 3200 2004   .8.B.>.3.>.2. .
+00008ab0: 4100 3a00 2008 0000 0000 0600 0000 1a52  A.:. ..........R
+00008ac0: 652d 6275 696c 6469 6e67 206c 6564 6765  e-building ledge
+00008ad0: 7220 7369 6e63 653a 2007 0000 0006 4c65  r since: .....Le
+00008ae0: 6467 6572 0103 0000 0058 041d 0435 0438  dger.....X...5.8
+00008af0: 0437 0432 0435 0441 0442 043d 044b 0439  .7.2.5.A.B.=.K.9
+00008b00: 0020 043f 0430 0440 0430 043c 0435 0442  . .?.0.@.0.<.5.B
+00008b10: 0440 0020 043a 0440 0438 0442 0438 0447  .@. .:.@.8.B.8.G
+00008b20: 043d 043e 0441 0442 0438 0020 0441 043e  .=.>.A.B.8. .A.>
+00008b30: 043e 0431 0449 0435 043d 0438 044f 003a  .>.1.I.5.=.8.O.:
+00008b40: 0020 0800 0000 0006 0000 0020 556e 6b6e  . ......... Unkn
+00008b50: 6f77 6e20 6c6f 6767 696e 6720 6c65 7665  own logging leve
+00008b60: 6c20 7072 6f76 6964 6564 3a20 0700 0000  l provided: ....
+00008b70: 094c 6f67 5669 6577 6572 0103 0000 000c  .LogViewer......
+00008b80: 25b2 0020 006c 006f 0067 0073 0800 0000  %.. .l.o.g.s....
+00008b90: 0006 0000 0008 e296 b220 6c6f 6773 0700  ......... logs..
+00008ba0: 0000 094c 6f67 5669 6577 6572 0103 0000  ...LogViewer....
+00008bb0: 000c 25b6 0020 006c 006f 0067 0073 0800  ..%.. .l.o.g.s..
+00008bc0: 0000 0006 0000 0008 e296 b620 6c6f 6773  ........... logs
+00008bd0: 0700 0000 094c 6f67 5669 6577 6572 0103  .....LogViewer..
+00008be0: 0000 003e 041e 0448 0438 0431 043a 0430  ...>...H.8.1.:.0
+00008bf0: 0020 043b 043e 0433 0438 043d 0430 0020  . .;.>.3.8.=.0. 
+00008c00: 0447 0435 0440 0435 0437 0020 0413 043e  .G.5.@.5.7. ...>
+00008c10: 0441 0443 0441 043b 0443 0433 0438 003a  .A.C.A.;.C.3.8.:
+00008c20: 0020 0800 0000 0006 0000 0013 4553 4941  . ..........ESIA
+00008c30: 206c 6f67 696e 2066 6169 6c65 643a 2007   login failed: .
+00008c40: 0000 0008 4c6f 6769 6e46 4e53 0103 0000  ....LoginFNS....
+00008c50: 0040 0423 0441 043f 0435 0448 043d 044b  .@.#.A.?.5.H.=.K
+00008c60: 0439 0020 043b 043e 0433 0438 043d 0020  .9. .;.>.3.8.=. 
+00008c70: 0447 0435 0440 0435 0437 0020 0413 043e  .G.5.@.5.7. ...>
+00008c80: 0441 0443 0441 043b 0443 0433 0438 003a  .A.C.A.;.C.3.8.:
+00008c90: 0020 0800 0000 0006 0000 0017 4553 4941  . ..........ESIA
+00008ca0: 206c 6f67 696e 2073 7563 6365 7373 6675   login successfu
+00008cb0: 6c3a 2007 0000 0008 4c6f 6769 6e46 4e53  l: .....LoginFNS
+00008cc0: 0103 0000 0038 041e 0448 0438 0431 043a  .....8...H.8.1.:
+00008cd0: 0430 0020 043b 043e 0433 0438 043d 0430  .0. .;.>.3.8.=.0
+00008ce0: 0020 0447 0435 0440 0435 0437 0020 041b  . .G.5.@.5.7. ..
+00008cf0: 041a 0020 0424 041d 0421 003a 0020 0800  ... .$...!.:. ..
+00008d00: 0000 0006 0000 0012 464e 5320 6c6f 6769  ........FNS logi
+00008d10: 6e20 6661 696c 6564 3a20 0700 0000 084c  n failed: .....L
+00008d20: 6f67 696e 464e 5301 0300 0000 3a04 2304  oginFNS.....:.#.
+00008d30: 4104 3f04 3504 4804 3d04 4b04 3900 2004  A.?.5.H.=.K.9. .
+00008d40: 3b04 3e04 3304 3804 3d00 2004 4704 3504  ;.>.3.8.=. .G.5.
+00008d50: 4004 3504 3700 2004 1b04 1a00 2004 2404  @.5.7. ..... .$.
+00008d60: 1d04 2100 3a00 2008 0000 0000 0600 0000  ..!.:. .........
+00008d70: 1646 4e53 206c 6f67 696e 2073 7563 6365  .FNS login succe
+00008d80: 7373 6675 6c3a 2007 0000 0008 4c6f 6769  ssful: .....Logi
+00008d90: 6e46 4e53 0103 0000 005a 041e 0448 0438  nFNS.....Z...H.8
+00008da0: 0431 043a 0430 0020 043f 043e 043b 0443  .1.:.0. .?.>.;.C
+00008db0: 0447 0435 043d 0438 044f 0020 0055 0052  .G.5.=.8.O. .U.R
+00008dc0: 004c 0020 043b 043e 0433 0438 043d 0430  .L. .;.>.3.8.=.0
+00008dd0: 0020 0447 0435 0440 0435 0437 0020 0413  . .G.5.@.5.7. ..
+00008de0: 043e 0441 0443 0441 043b 0443 0433 0438  .>.A.C.A.;.C.3.8
+00008df0: 003a 0020 0800 0000 0006 0000 0015 4765  .:. ..........Ge
+00008e00: 7420 4553 4941 2055 524c 2066 6169 6c65  t ESIA URL faile
+00008e10: 643a 2007 0000 0008 4c6f 6769 6e46 4e53  d: .....LoginFNS
+00008e20: 0103 0000 0034 0053 004d 0053 0020 0431  .....4.S.M.S. .1
+00008e30: 044b 043b 043e 0020 0437 0430 043f 0440  .K.;.>. .7.0.?.@
+00008e40: 043e 0448 0435 043d 043e 0020 0443 0441  .>.H.5.=.>. .C.A
+00008e50: 043f 0435 0448 043d 043e 0800 0000 0006  .?.5.H.=.>......
+00008e60: 0000 001e 534d 5320 7761 7320 7265 7175  ....SMS was requ
+00008e70: 6573 7465 6420 7375 6363 6573 7366 756c  ested successful
+00008e80: 6c79 0700 0000 084c 6f67 696e 464e 5301  ly.....LoginFNS.
+00008e90: 0300 0000 1e04 1004 3204 4204 3e04 4004  ........2.B.>.@.
+00008ea0: 3804 3704 3004 4604 3804 4f00 2004 2404  8.7.0.F.8.O. .$.
+00008eb0: 1d04 2108 0000 0000 0600 0000 1141 7574  ..!..........Aut
+00008ec0: 686f 7269 7a61 7469 6f6e 2046 4e53 0700  horization FNS..
+00008ed0: 0000 0e4c 6f67 696e 464e 5344 6961 6c6f  ...LoginFNSDialo
+00008ee0: 6701 0300 0000 0e04 1704 3004 3a04 4004  g.........0.:.@.
+00008ef0: 4b04 4204 4c08 0000 0000 0600 0000 0543  K.B.L..........C
+00008f00: 6c6f 7365 0700 0000 0e4c 6f67 696e 464e  lose.....LoginFN
+00008f10: 5344 6961 6c6f 6701 0300 0000 1604 1a04  SDialog.........
+00008f20: 3e04 3400 2004 3804 3700 2000 5300 4d00  >.4. .8.7. .S.M.
+00008f30: 5300 3a08 0000 0000 0600 0000 0e43 6f64  S.:..........Cod
+00008f40: 6520 6672 6f6d 2053 4d53 3a07 0000 000e  e from SMS:.....
+00008f50: 4c6f 6769 6e46 4e53 4469 616c 6f67 0103  LoginFNSDialog..
+00008f60: 0000 0012 0413 043e 0441 0443 0441 043b  .......>.A.C.A.;
+00008f70: 0443 0433 0438 0800 0000 0006 0000 000a  .C.3.8..........
+00008f80: 4553 4941 204c 6f67 696e 0700 0000 0e4c  ESIA Login.....L
+00008f90: 6f67 696e 464e 5344 6961 6c6f 6701 0300  oginFNSDialog...
+00008fa0: 0000 0c04 1b04 1a00 2004 2404 1d04 2108  ........ .$...!.
+00008fb0: 0000 0000 0600 0000 0946 4e53 204c 6f67  .........FNS Log
+00008fc0: 696e 0700 0000 0e4c 6f67 696e 464e 5344  in.....LoginFNSD
+00008fd0: 6961 6c6f 6701 0300 0000 0804 1804 1d04  ialog...........
+00008fe0: 1d00 3a08 0000 0000 0600 0000 0449 4e4e  ..:..........INN
+00008ff0: 3a07 0000 000e 4c6f 6769 6e46 4e53 4469  :.....LoginFNSDi
+00009000: 616c 6f67 0103 0000 000a 041b 043e 0433  alog.........>.3
+00009010: 0438 043d 0800 0000 0006 0000 0005 4c6f  .8.=..........Lo
+00009020: 6769 6e07 0000 000e 4c6f 6769 6e46 4e53  gin.....LoginFNS
+00009030: 4469 616c 6f67 0103 0000 000e 041f 0430  Dialog.........0
+00009040: 0440 043e 043b 044c 003a 0800 0000 0006  .@.>.;.L.:......
+00009050: 0000 0009 5061 7373 776f 7264 3a07 0000  ....Password:...
+00009060: 000e 4c6f 6769 6e46 4e53 4469 616c 6f67  ..LoginFNSDialog
+00009070: 0103 0000 001e 041d 043e 043c 0435 0440  .........>.<.5.@
+00009080: 0020 0442 0435 043b 0435 0444 043e 043d  . .B.5.;.5.D.>.=
+00009090: 0430 003a 0800 0000 0006 0000 000d 5068  .0.:..........Ph
+000090a0: 6f6e 6520 6e75 6d62 6572 3a07 0000 000e  one number:.....
+000090b0: 4c6f 6769 6e46 4e53 4469 616c 6f67 0103  LoginFNSDialog..
+000090c0: 0000 0006 0053 004d 0053 0800 0000 0006  .....S.M.S......
+000090d0: 0000 0009 534d 5320 4c6f 6769 6e07 0000  ....SMS Login...
+000090e0: 000e 4c6f 6769 6e46 4e53 4469 616c 6f67  ..LoginFNSDialog
+000090f0: 0103 0000 0026 0412 044b 0441 043b 0430  .....&...K.A.;.0
+00009100: 0442 044c 0020 0053 004d 0053 0020 0441  .B.L. .S.M.S. .A
+00009110: 0020 043a 043e 0434 043e 043c 0800 0000  . .:.>.4.>.<....
+00009120: 0006 0000 0012 5365 6e64 2053 4d53 2077  ......Send SMS w
+00009130: 6974 6820 636f 6465 0700 0000 0e4c 6f67  ith code.....Log
+00009140: 696e 464e 5344 6961 6c6f 6701 0300 0000  inFNSDialog.....
+00009150: 1600 6100 6200 6f00 7500 7400 3a00 6200  ..a.b.o.u.t.:.b.
+00009160: 6c00 6100 6e00 6b08 0000 0000 0600 0000  l.a.n.k.........
+00009170: 0b61 626f 7574 3a62 6c61 6e6b 0700 0000  .about:blank....
+00009180: 0e4c 6f67 696e 464e 5344 6961 6c6f 6701  .LoginFNSDialog.
+00009190: 0300 0000 4404 1d04 3004 3904 3404 3504  ....D...0.9.4.5.
+000091a0: 3d04 3e00 2004 3d04 3504 4104 3a04 3e04  =.>. .=.5.A.:.>.
+000091b0: 3b04 4c04 3a04 3e00 2004 2604 1100 2004  ;.L.:.>. .&... .
+000091c0: 3d04 3000 2000 4d00 4f00 4500 5800 2004  =.0. .M.O.E.X. .
+000091d0: 3404 3b04 4f00 3a00 2008 0000 0000 0600  4.;.O.:. .......
+000091e0: 0000 204d 756c 7469 706c 6520 4d4f 4558  .. Multiple MOEX
+000091f0: 2061 7373 6574 7320 666f 756e 6420 666f   assets found fo
+00009200: 723a 2007 0000 0004 4d4f 4558 0103 0000  r: .....MOEX....
+00009210: 0044 041d 0435 043f 043e 0434 0434 0435  .D...5.?.>.4.4.5
+00009220: 0440 0436 0438 0432 0430 0435 043c 044b  .@.6.8.2.0.5.<.K
+00009230: 0439 0020 0442 0438 043f 0020 0426 0411  .9. .B.8.?. .&..
+00009240: 0020 041c 043e 0441 0411 0438 0440 0436  . ...>.A...8.@.6
+00009250: 0438 003a 0020 0800 0000 0006 0000 0020  .8.:. ......... 
+00009260: 556e 7375 7070 6f72 7465 6420 4d4f 4558  Unsupported MOEX
+00009270: 2073 6563 7572 6974 7920 7479 7065 3a20   security type: 
+00009280: 0700 0000 044d 4f45 5801 0300 0000 1604  .....MOEX.......
+00009290: 1e00 2004 3f04 4004 3e04 3304 4004 3004  .. .?.@.>.3.@.0.
+000092a0: 3c04 3c04 3508 0000 0000 0600 0000 0541  <.<.5..........A
+000092b0: 626f 7574 0700 0000 0a4d 6169 6e57 696e  bout.....MainWin
+000092c0: 646f 7701 0300 0000 1a04 1f04 3e04 3404  dow.........>.4.
+000092d0: 4204 3204 3504 4004 3604 3404 3504 3d04  B.2.5.@.6.4.5.=.
+000092e0: 3804 3508 0000 0000 0600 0000 0c43 6f6e  8.5..........Con
+000092f0: 6669 726d 6174 696f 6e07 0000 000a 4d61  firmation.....Ma
+00009300: 696e 5769 6e64 6f77 0103 0000 0014 0418  inWindow........
+00009310: 043d 0444 043e 0440 043c 0430 0446 0438  .=.D.>.@.<.0.F.8
+00009320: 044f 0800 0000 0006 0000 0004 496e 666f  .O..........Info
+00009330: 0700 0000 0a4d 6169 6e57 696e 646f 7701  .....MainWindow.
+00009340: 0300 0000 2804 2f04 3704 4b04 3a00 2004  ....(./.7.K.:. .
+00009350: 3104 4b04 3b00 2004 3804 3704 3c04 3504  1.K.;. .8.7.<.5.
+00009360: 3d04 5104 3d00 2004 3d04 3000 2008 0000  =.Q.=. .=.0. ...
+00009370: 0000 0600 0000 184c 616e 6775 6167 6520  .......Language 
+00009380: 7761 7320 6368 616e 6765 6420 746f 2007  was changed to .
+00009390: 0000 000a 4d61 696e 5769 6e64 6f77 0103  ....MainWindow..
+000093a0: 0000 0062 0418 0442 043e 0433 0438 0020  ...b...B.>.3.8. 
+000093b0: 0442 0440 0430 043d 0437 0430 043a 0446  .B.@.0.=.7.0.:.F
+000093c0: 0438 0439 0020 043d 0435 0430 043a 0442  .8.9. .=.5.0.:.B
+000093d0: 0443 0430 043b 044c 043d 044b 002e 0020  .C.0.;.L.=.K... 
+000093e0: 041f 0435 0440 0435 0441 0447 0438 0442  ...5.@.5.A.G.8.B
+000093f0: 0430 0442 044c 0020 0441 0435 0439 0447  .0.B.L. .A.5.9.G
+00009400: 0430 0441 003f 0800 0000 0006 0000 0026  .0.A.?.........&
+00009410: 4c65 6467 6572 2069 736e 2774 2063 6f6d  Ledger isn't com
+00009420: 706c 6574 652e 2052 6562 7569 6c64 2069  plete. Rebuild i
+00009430: 7420 6e6f 773f 0700 0000 0a4d 6169 6e57  t now?.....MainW
+00009440: 696e 646f 7701 0300 0000 8004 1404 3e04  indow.........>.
+00009450: 3f04 3e04 3b04 3d04 3804 4204 3504 3b04  ?.>.;.=.8.B.5.;.
+00009460: 4c04 3d04 3004 4f00 2004 3804 3d04 4404  L.=.0.O. .8.=.D.
+00009470: 3e04 4004 3c04 3004 4604 3804 4f00 2c00  >.@.<.0.F.8.O.,.
+00009480: 2004 3804 3d04 4104 4204 4004 4304 3a04   .8.=.A.B.@.C.:.
+00009490: 4604 3804 3800 2c00 2004 4104 3e04 3e04  F.8.8.,. .A.>.>.
+000094a0: 3104 4904 3504 3d04 3804 4f00 2004 3e00  1.I.5.=.8.O. .>.
+000094b0: 2004 3f04 4004 3e04 3104 3b04 3504 3c04   .?.@.>.1.;.5.<.
+000094c0: 3004 4500 2004 3d04 3000 2008 0000 0000  0.E. .=.0. .....
+000094d0: 0600 0000 354d 6f72 6520 696e 666f 726d  ....5More inform
+000094e0: 6174 696f 6e2c 206d 616e 7561 6c73 2061  ation, manuals a
+000094f0: 6e64 2070 726f 626c 656d 2072 6570 6f72  nd problem repor
+00009500: 7473 2061 7265 2061 7420 0700 0000 0a4d  ts are at .....M
+00009510: 6169 6e57 696e 646f 7701 0300 0000 5004  ainWindow.....P.
+00009520: 1204 3e04 3f04 4004 3e04 4104 4b00 2c00  ..>.?.@.>.A.K.,.
+00009530: 2004 3a04 3e04 3c04 3c04 3504 3d04 4204   .:.>.<.<.5.=.B.
+00009540: 3004 4004 3804 3800 2c00 2004 3f04 3e04  0.@.8.8.,. .?.>.
+00009550: 3c04 3e04 4904 4c00 2004 3804 3b04 3800  <.>.I.L. .8.;.8.
+00009560: 2004 3404 3e04 3d04 3004 4204 4b00 3a08   .4.>.=.0.B.K.:.
+00009570: 0000 0000 0600 0000 2751 7565 7374 696f  ........'Questio
+00009580: 6e73 2c20 636f 6d6d 656e 7473 2c20 6865  ns, comments, he
+00009590: 6c70 206f 7220 646f 6e61 7469 6f6e 733a  lp or donations:
+000095a0: 0700 0000 0a4d 6169 6e57 696e 646f 7701  .....MainWindow.
+000095b0: 0300 0000 2204 2204 4004 3504 3104 4304  ....".".@.5.1.C.
+000095c0: 3504 4204 4104 4f00 2004 4004 3504 4104  5.B.A.O. .@.5.A.
+000095d0: 4204 3004 4004 4208 0000 0000 0600 0000  B.0.@.B.........
+000095e0: 1052 6573 7461 7274 2072 6571 7569 7265  .Restart require
+000095f0: 6407 0000 000a 4d61 696e 5769 6e64 6f77  d.....MainWindow
+00009600: 0103 0000 0050 041a 043e 043d 0435 0447  .....P...>.=.5.G
+00009610: 043d 044b 0439 0020 0431 0430 043b 0430  .=.K.9. .1.0.;.0
+00009620: 043d 0441 0020 043f 043e 0020 043e 0442  .=.A. .?.>. .>.B
+00009630: 0447 0451 0442 0443 0020 043d 0435 0020  .G.Q.B.C. .=.5. 
+00009640: 0441 043e 0432 043f 0430 0434 0430 0435  .A.>.2.?.0.4.0.5
+00009650: 0442 003a 0020 0800 0000 0006 0000 0028  .B.:. .........(
+00009660: 5374 6174 656d 656e 7420 656e 6469 6e67  Statement ending
+00009670: 2062 616c 616e 6365 2064 6f65 736e 2774   balance doesn't
+00009680: 206d 6174 6368 3a20 0700 0000 0a4d 6169   match: .....Mai
+00009690: 6e57 696e 646f 7701 0300 0000 c804 1204  nWindow.........
+000096a0: 4b00 2004 3404 3e04 3b04 3604 3d04 4b00  K. .4.>.;.6.=.K.
+000096b0: 2004 3f04 3504 4004 3504 3704 3004 3f04   .?.5.@.5.7.0.?.
+000096c0: 4304 4104 4204 3804 4204 4c00 2004 3f04  C.A.B.8.B.L. .?.
+000096d0: 4004 3804 3b04 3e04 3604 3504 3d04 3804  @.8.;.>.6.5.=.8.
+000096e0: 3500 2c00 2004 4704 4204 3e04 3104 4b00  5.,. .G.B.>.1.K.
+000096f0: 2004 3f04 4004 3804 3c04 3504 3d04 3804   .?.@.8.<.5.=.8.
+00009700: 4204 4c00 2004 3804 3704 3c04 3504 3d04  B.L. .8.7.<.5.=.
+00009710: 3504 3d04 3804 4f00 0a04 1f04 4004 3804  5.=.8.O.....@.8.
+00009720: 3b04 3e04 3604 3504 3d04 3804 3500 2004  ;.>.6.5.=.8.5. .
+00009730: 4104 3504 3904 4704 3004 4100 2004 3704  A.5.9.G.0.A. .7.
+00009740: 3004 3204 3504 4004 4804 3804 4200 2004  0.2.5.@.H.8.B. .
+00009750: 4104 3204 3e04 4e00 2004 4004 3004 3104  A.2.>.N. .@.0.1.
+00009760: 3e04 4204 4308 0000 0000 0600 0000 5259  >.B.C.........RY
+00009770: 6f75 2073 686f 756c 6420 7265 7374 6172  ou should restar
+00009780: 7420 6170 706c 6963 6174 696f 6e20 746f  t application to
+00009790: 2061 7070 6c79 2063 6861 6e67 6573 0a41   apply changes.A
+000097a0: 7070 6c69 6361 7469 6f6e 2077 696c 6c20  pplication will 
+000097b0: 6265 2074 6572 6d69 6e61 7465 6420 6e6f  be terminated no
+000097c0: 7707 0000 000a 4d61 696e 5769 6e64 6f77  w.....MainWindow
+000097d0: 0103 0000 0030 0434 043e 043c 0430 0448  .....0.4.>.<.0.H
+000097e0: 043d 0435 0439 0020 0441 0442 0440 0430  .=.5.9. .A.B.@.0
+000097f0: 043d 0438 0446 0435 0020 0067 0069 0074  .=.8.F.5. .g.i.t
+00009800: 0068 0075 0062 0800 0000 0006 0000 0010  .h.u.b..........
+00009810: 6769 7468 7562 2068 6f6d 6520 7061 6765  github home page
+00009820: 0700 0000 0a4d 6169 6e57 696e 646f 7701  .....MainWindow.
+00009830: 0300 0000 0c04 3204 3504 4004 4104 3804  ......2.5.@.A.8.
+00009840: 4f08 0000 0000 0600 0000 0776 6572 7369  O..........versi
+00009850: 6f6e 0700 0000 0a4d 6169 6e57 696e 646f  on.....MainWindo
+00009860: 7701 0300 0000 0600 2e00 2e00 2e08 0000  w...............
+00009870: 0000 0600 0000 032e 2e2e 0700 0000 0f4d  ...............M
+00009880: 6f6e 6579 466c 6f77 5769 6467 6574 0103  oneyFlowWidget..
+00009890: 0000 0016 0424 0430 0439 043b 0020 0045  .....$.0.9.;. .E
+000098a0: 0078 0063 0065 006c 003a 0800 0000 0006  .x.c.e.l.:......
+000098b0: 0000 000b 4578 6365 6c20 6669 6c65 3a07  ....Excel file:.
+000098c0: 0000 000f 4d6f 6e65 7946 6c6f 7757 6964  ....MoneyFlowWid
+000098d0: 6765 7401 0300 0000 2804 2404 3004 3904  get.....(.$.0.9.
+000098e0: 3b04 4b00 2000 4500 7800 6300 6500 6c00  ;.K. .E.x.c.e.l.
+000098f0: 2000 2800 2a00 2e00 7800 7300 6c00 7800   .(.*...x.s.l.x.
+00009900: 2908 0000 0000 0600 0000 1445 7863 656c  )..........Excel
+00009910: 2066 696c 6573 2028 2a2e 786c 7378 2907   files (*.xlsx).
+00009920: 0000 000f 4d6f 6e65 7946 6c6f 7757 6964  ....MoneyFlowWid
+00009930: 6765 7401 0300 0000 5604 2404 3004 3904  get.....V.$.0.9.
+00009940: 3b00 2004 3404 3b04 4f00 2004 4104 3e04  ;. .4.;.O. .A.>.
+00009950: 4504 4004 3004 3d04 3504 3d04 3804 4f00  E.@.0.=.5.=.8.O.
+00009960: 2004 4004 3004 4104 4704 5104 4204 3000   .@.0.A.G.Q.B.0.
+00009970: 2004 3200 2004 4404 3e04 4004 3c04 3004   .2. .D.>.@.<.0.
+00009980: 4204 3500 2000 4500 7800 6300 6500 6c08  B.5. .E.x.c.e.l.
+00009990: 0000 0000 0600 0000 2e46 696c 6520 7768  .........File wh
+000099a0: 6572 6520 746f 2073 746f 7265 2074 6178  ere to store tax
+000099b0: 2072 6570 6f72 7420 696e 2045 7863 656c   report in Excel
+000099c0: 2066 6f72 6d61 7407 0000 000f 4d6f 6e65   format.....Mone
+000099d0: 7946 6c6f 7757 6964 6765 7401 0300 0000  yFlowWidget.....
+000099e0: 0a04 1e04 3e04 1404 1404 2108 0000 0000  ....>.....!.....
+000099f0: 0600 0000 0a4d 6f6e 6579 2046 6c6f 7707  .....Money Flow.
+00009a00: 0000 000f 4d6f 6e65 7946 6c6f 7757 6964  ....MoneyFlowWid
+00009a10: 6765 7401 0300 0000 2e04 1e04 3e04 1404  get.........>...
+00009a20: 1404 2100 2004 4104 3e04 4504 4004 3004  ..!. .A.>.E.@.0.
+00009a30: 3d04 5104 3d00 2004 3200 2004 4404 3004  =.Q.=. .2. .D.0.
+00009a40: 3904 3b04 3500 2008 0000 0000 0600 0000  9.;.5. .........
+00009a50: 204d 6f6e 6579 2066 6c6f 7720 7265 706f   Money flow repo
+00009a60: 7274 2073 6176 6564 2074 6f20 6669 6c65  rt saved to file
+00009a70: 2007 0000 000f 4d6f 6e65 7946 6c6f 7757   .....MoneyFlowW
+00009a80: 6964 6765 7401 0300 0000 1e04 2104 3e04  idget.......!.>.
+00009a90: 4504 4004 3004 3d04 3804 4204 4c00 2004  E.@.0.=.8.B.L. .
+00009aa0: 1e04 4204 4704 5104 4208 0000 0000 0600  ..B.G.Q.B.......
+00009ab0: 0000 0b53 6176 6520 5265 706f 7274 0700  ...Save Report..
+00009ac0: 0000 0f4d 6f6e 6579 466c 6f77 5769 6467  ...MoneyFlowWidg
+00009ad0: 6574 0103 0000 0024 0421 043e 0445 0440  et.....$.!.>.E.@
+00009ae0: 0430 043d 0438 0442 044c 0020 041e 043e  .0.=.8.B.L. ...>
+00009af0: 0414 0414 0421 0020 0432 003a 0800 0000  .....!. .2.:....
+00009b00: 0006 0000 001a 5361 7665 206d 6f6e 6579  ......Save money
+00009b10: 2066 6c6f 7720 7265 706f 7274 2074 6f3a   flow report to:
+00009b20: 0700 0000 0f4d 6f6e 6579 466c 6f77 5769  .....MoneyFlowWi
+00009b30: 6467 6574 0103 0000 0018 0412 044b 0431  dget.........K.1
+00009b40: 0435 0440 0438 0442 0020 0444 0430 0439  .5.@.8.B. .D.0.9
+00009b50: 043b 0800 0000 0006 0000 000b 5365 6c65  .;..........Sele
+00009b60: 6374 2066 696c 6507 0000 000f 4d6f 6e65  ct file.....Mone
+00009b70: 7946 6c6f 7757 6964 6765 7401 0300 0000  yFlowWidget.....
+00009b80: 0804 1304 3e04 3400 3a08 0000 0000 0600  ....>.4.:.......
+00009b90: 0000 0559 6561 723a 0700 0000 0f4d 6f6e  ...Year:.....Mon
+00009ba0: 6579 466c 6f77 5769 6467 6574 0103 0000  eyFlowWidget....
+00009bb0: 0028 0020 043d 0435 0443 0441 043f 0435  .(. .=.5.C.A.?.5
+00009bc0: 0448 043d 044b 0439 0020 0437 0430 043f  .H.=.K.9. .7.0.?
+00009bd0: 0440 043e 0441 003a 0020 0800 0000 0006  .@.>.A.:. ......
+00009be0: 0000 0009 2066 6169 6c65 643a 2007 0000  .... failed: ...
+00009bf0: 0003 4e65 7401 0300 0000 3404 2204 3804  ..Net.....4.".8.
+00009c00: 3f00 2004 2604 1100 2004 3d04 3500 2004  ?. .&... .=.5. .
+00009c10: 3f04 3e04 3404 3404 3504 4004 3604 3804  ?.>.4.4.5.@.6.8.
+00009c20: 3204 3004 3504 4204 4104 4f00 3a00 2008  2.0.5.B.A.O.:. .
+00009c30: 0000 0000 0600 0000 1c41 7373 6574 2074  .........Asset t
+00009c40: 7970 6520 6973 6e27 7420 7375 7070 6f72  ype isn't suppor
+00009c50: 7465 643a 2007 0000 000a 4f70 656e 4272  ted: .....OpenBr
+00009c60: 6f6b 6572 0103 0000 0032 0411 0438 0440  oker.....2...8.@
+00009c70: 0436 0430 0020 043d 0435 0020 043f 043e  .6.0. .=.5. .?.>
+00009c80: 0434 0434 0435 0440 0436 0438 0432 0430  .4.4.5.@.6.8.2.0
+00009c90: 0435 0442 0441 044f 003a 0020 0800 0000  .5.B.A.O.:. ....
+00009ca0: 0006 0000 001a 4578 6368 616e 6765 2069  ......Exchange i
+00009cb0: 736e 2774 2073 7570 706f 7274 6564 3a20  sn't supported: 
+00009cc0: 0700 0000 0a4f 7065 6e42 726f 6b65 7201  .....OpenBroker.
+00009cd0: 0300 0000 0804 2104 4704 3504 4208 0000  ......!.G.5.B...
+00009ce0: 0000 0600 0000 0741 6363 6f75 6e74 0700  .......Account..
+00009cf0: 0000 0f4f 7065 7261 7469 6f6e 734d 6f64  ...OperationsMod
+00009d00: 656c 0103 0000 000a 0421 0443 043c 043c  el.......!.C.<.<
+00009d10: 0430 0800 0000 0006 0000 0006 416d 6f75  .0..........Amou
+00009d20: 6e74 0700 0000 0f4f 7065 7261 7469 6f6e  nt.....Operation
+00009d30: 734d 6f64 656c 0103 0000 000c 0411 0430  sModel.........0
+00009d40: 043b 0430 043d 0441 0800 0000 0006 0000  .;.0.=.A........
+00009d50: 0007 4261 6c61 6e63 6507 0000 000f 4f70  ..Balance.....Op
+00009d60: 6572 6174 696f 6e73 4d6f 6465 6c01 0300  erationsModel...
+00009d70: 0000 0c04 1204 3004 3b04 4e04 4204 3008  ......0.;.N.B.0.
+00009d80: 0000 0000 0600 0000 0843 7572 7265 6e63  .........Currenc
+00009d90: 7907 0000 000f 4f70 6572 6174 696f 6e73  y.....Operations
+00009da0: 4d6f 6465 6c01 0300 0000 1004 1e04 3f04  Model.........?.
+00009db0: 3804 4104 3004 3d04 3804 3508 0000 0000  8.A.0.=.8.5.....
+00009dc0: 0600 0000 054e 6f74 6573 0700 0000 0f4f  .....Notes.....O
+00009dd0: 7065 7261 7469 6f6e 734d 6f64 656c 0103  perationsModel..
+00009de0: 0000 0014 0414 0430 0442 0430 002f 0412  .......0.B.0./..
+00009df0: 0440 0435 043c 044f 0800 0000 0006 0000  .@.5.<.O........
+00009e00: 0009 5469 6d65 7374 616d 7007 0000 000f  ..Timestamp.....
+00009e10: 4f70 6572 6174 696f 6e73 4d6f 6465 6c01  OperationsModel.
+00009e20: 0300 0000 0a04 2104 4704 3504 4200 3a08  ......!.G.5.B.:.
+00009e30: 0000 0000 0600 0000 0841 6363 6f75 6e74  .........Account
+00009e40: 3a07 0000 0010 4f70 6572 6174 696f 6e73  :.....Operations
+00009e50: 5769 6467 6574 0103 0000 004a 0412 044b  Widget.....J...K
+00009e60: 0020 0445 043e 0442 0438 0442 0435 0020  . .E.>.B.8.B.5. 
+00009e70: 0443 0434 0430 043b 0438 0442 044c 0020  .C.4.0.;.8.B.L. 
+00009e80: 0432 044b 0431 0440 0430 043d 043d 044b  .2.K.1.@.0.=.=.K
+00009e90: 0435 0020 043e 043f 0435 0440 0430 0446  .5. .>.?.5.@.0.F
+00009ea0: 0438 0438 003f 0800 0000 0006 0000 002e  .8.8.?..........
+00009eb0: 4172 6520 796f 7520 7375 7265 2074 6f20  Are you sure to 
+00009ec0: 6465 6c65 7465 2073 656c 6563 7465 6420  delete selected 
+00009ed0: 7472 616e 7361 6369 6f6e 2873 293f 0700  transacion(s)?..
+00009ee0: 0000 104f 7065 7261 7469 6f6e 7357 6964  ...OperationsWid
+00009ef0: 6765 7401 0300 0000 1c04 1104 3004 3b04  get.........0.;.
+00009f00: 3004 3d04 4104 4b00 2004 4104 4704 3504  0.=.A.K. .A.G.5.
+00009f10: 4204 3e04 3208 0000 0000 0600 0000 0842  B.>.2..........B
+00009f20: 616c 616e 6365 7307 0000 0010 4f70 6572  alances.....Oper
+00009f30: 6174 696f 6e73 5769 6467 6574 0103 0000  ationsWidget....
+00009f40: 001a 041f 043e 0434 0442 0432 0435 0440  .....>.4.B.2.5.@
+00009f50: 0436 0434 0435 043d 0438 0435 0800 0000  .6.4.5.=.8.5....
+00009f60: 0006 0000 000c 436f 6e66 6972 6d61 7469  ......Confirmati
+00009f70: 6f6e 0700 0000 104f 7065 7261 7469 6f6e  on.....Operation
+00009f80: 7357 6964 6765 7401 0300 0000 1404 1a04  sWidget.........
+00009f90: 3e04 3f04 3804 4004 3e04 3204 3004 4204  >.?.8.@.>.2.0.B.
+00009fa0: 4c08 0000 0000 0600 0000 0443 6f70 7907  L..........Copy.
+00009fb0: 0000 0010 4f70 6572 6174 696f 6e73 5769  ....OperationsWi
+00009fc0: 6467 6574 0103 0000 0026 041a 043e 043f  dget.....&...>.?
+00009fd0: 0438 0440 043e 0432 0430 0442 044c 0020  .8.@.>.2.0.B.L. 
+00009fe0: 043e 043f 0435 0440 0430 0446 0438 044e  .>.?.5.@.0.F.8.N
+00009ff0: 0800 0000 0006 0000 000e 436f 7079 206f  ..........Copy o
+0000a000: 7065 7261 7469 6f6e 0700 0000 104f 7065  peration.....Ope
+0000a010: 7261 7469 6f6e 7357 6964 6765 7401 0300  rationsWidget...
+0000a020: 0000 0e04 2304 3404 3004 3b04 3804 4204  ....#.4.0.;.8.B.
+0000a030: 4c08 0000 0000 0600 0000 0644 656c 6574  L..........Delet
+0000a040: 6507 0000 0010 4f70 6572 6174 696f 6e73  e.....Operations
+0000a050: 5769 6467 6574 0103 0000 0020 0423 0434  Widget..... .#.4
+0000a060: 0430 043b 0438 0442 044c 0020 043e 043f  .0.;.8.B.L. .>.?
+0000a070: 0435 0440 0430 0446 0438 044e 0800 0000  .5.@.0.F.8.N....
+0000a080: 0006 0000 0010 4465 6c65 7465 206f 7065  ......Delete ope
+0000a090: 7261 7469 6f6e 0700 0000 104f 7065 7261  ration.....Opera
+0000a0a0: 7469 6f6e 7357 6964 6765 7401 0300 0000  tionsWidget.....
+0000a0b0: 1c04 1d04 3e04 3204 3004 4f00 2004 3e04  ....>.2.0.O. .>.
+0000a0c0: 3f04 3504 4004 3004 4604 3804 4f08 0000  ?.5.@.0.F.8.O...
+0000a0d0: 0000 0600 0000 0d4e 6577 206f 7065 7261  .......New opera
+0000a0e0: 7469 6f6e 0700 0000 104f 7065 7261 7469  tion.....Operati
+0000a0f0: 6f6e 7357 6964 6765 7401 0300 0000 1004  onsWidget.......
+0000a100: 1e04 3f04 3504 4004 3004 4604 3804 3808  ..?.5.@.0.F.8.8.
+0000a110: 0000 0000 0600 0000 0a4f 7065 7261 7469  .........Operati
+0000a120: 6f6e 7307 0000 0010 4f70 6572 6174 696f  ons.....Operatio
+0000a130: 6e73 5769 6467 6574 0103 0000 0024 041e  nsWidget.....$..
+0000a140: 043f 0435 0440 0430 0446 0438 0438 0020  .?.5.@.0.F.8.8. 
+0000a150: 0438 0020 0411 0430 043b 0430 043d 0441  .8. ...0.;.0.=.A
+0000a160: 044b 0800 0000 0006 0000 0015 4f70 6572  .K..........Oper
+0000a170: 6174 696f 6e73 2026 2042 616c 616e 6365  ations & Balance
+0000a180: 7307 0000 0010 4f70 6572 6174 696f 6e73  s.....Operations
+0000a190: 5769 6467 6574 0103 0000 000e 0421 0432  Widget.......!.2
+0000a1a0: 0435 0440 0438 0442 044c 0800 0000 0006  .5.@.8.B.L......
+0000a1b0: 0000 0009 5265 636f 6e63 696c 6507 0000  ....Reconcile...
+0000a1c0: 0010 4f70 6572 6174 696f 6e73 5769 6467  ..OperationsWidg
+0000a1d0: 6574 0103 0000 000c 041f 043e 0438 0441  et.........>.8.A
+0000a1e0: 043a 003a 0800 0000 0006 0000 0007 5365  .:.:..........Se
+0000a1f0: 6172 6368 3a07 0000 0010 4f70 6572 6174  arch:.....Operat
+0000a200: 696f 6e73 5769 6467 6574 0103 0000 002c  ionsWidget.....,
+0000a210: 041f 043e 043a 0430 0437 044b 0432 0430  ...>.:.0.7.K.2.0
+0000a220: 0442 044c 0020 0026 043d 0435 0430 043a  .B.L. .&.=.5.0.:
+0000a230: 0442 0438 0432 043d 044b 0435 0800 0000  .B.8.2.=.K.5....
+0000a240: 0006 0000 000e 5368 6f77 2026 496e 6163  ......Show &Inac
+0000a250: 7469 7665 0700 0000 104f 7065 7261 7469  tive.....Operati
+0000a260: 6f6e 7357 6964 6765 7401 0300 0000 1a04  onsWidget.......
+0000a270: 1204 3004 3b04 4e04 4204 3000 2004 3804  ..0.;.N.B.0. .8.
+0000a280: 4204 3e04 3304 3e00 3a08 0000 0000 0600  B.>.3.>.:.......
+0000a290: 0000 0d53 756d 2043 7572 7265 6e63 793a  ...Sum Currency:
+0000a2a0: 0700 0000 104f 7065 7261 7469 6f6e 7357  .....OperationsW
+0000a2b0: 6964 6765 7401 0300 0000 1400 6400 6400  idget.......d.d.
+0000a2c0: 2f00 4d00 4d00 2f00 7900 7900 7900 7908  /.M.M./.y.y.y.y.
+0000a2d0: 0000 0000 0600 0000 0a64 642f 4d4d 2f79  .........dd/MM/y
+0000a2e0: 7979 7907 0000 0010 4f70 6572 6174 696f  yyy.....Operatio
+0000a2f0: 6e73 5769 6467 6574 0103 0000 000c 0412  nsWidget........
+0000a300: 0430 043b 044e 0442 0430 0800 0000 0006  .0.;.N.B.0......
+0000a310: 0000 0008 4375 7272 656e 6379 0700 0000  ....Currency....
+0000a320: 184f 7074 696f 6e61 6c43 7572 7265 6e63  .OptionalCurrenc
+0000a330: 7943 6f6d 626f 426f 7801 0300 0000 0a04  yComboBox.......
+0000a340: 2104 4304 3c04 3c04 3008 0000 0000 0600  !.C.<.<.0.......
+0000a350: 0000 0641 6d6f 756e 7407 0000 0010 5061  ...Amount.....Pa
+0000a360: 6e64 6173 4c69 6e65 734d 6f64 656c 0103  ndasLinesModel..
+0000a370: 0000 0012 041a 0430 0442 0435 0433 043e  .......0.B.5.3.>
+0000a380: 0440 0438 044f 0800 0000 0006 0000 0008  .@.8.O..........
+0000a390: 4361 7465 676f 7279 0700 0000 1050 616e  Category.....Pan
+0000a3a0: 6461 734c 696e 6573 4d6f 6465 6c01 0300  dasLinesModel...
+0000a3b0: 0000 2204 1d04 3004 3704 3204 3004 3d04  .."...0.7.2.0.=.
+0000a3c0: 3804 3500 2004 3f04 4004 3e04 3404 4304  8.5. .?.@.>.4.C.
+0000a3d0: 3a04 4204 3008 0000 0000 0600 0000 0c50  :.B.0..........P
+0000a3e0: 726f 6475 6374 206e 616d 6507 0000 0010  roduct name.....
+0000a3f0: 5061 6e64 6173 4c69 6e65 734d 6f64 656c  PandasLinesModel
+0000a400: 0103 0000 0006 0422 044d 0433 0800 0000  .......".M.3....
+0000a410: 0006 0000 0003 5461 6707 0000 0010 5061  ......Tag.....Pa
+0000a420: 6e64 6173 4c69 6e65 734d 6f64 656c 0103  ndasLinesModel..
+0000a430: 0000 0024 0027 0020 0437 0430 043c 0435  ...$.'. .7.0.<.5
+0000a440: 043d 0435 043d 0430 0020 0443 0441 043f  .=.5.=.0. .C.A.?
+0000a450: 0435 0448 043d 043e 0800 0000 0006 0000  .5.H.=.>........
+0000a460: 001b 2720 7761 7320 7375 6363 6573 7366  ..' was successf
+0000a470: 756c 6c79 2072 6570 6c61 6365 6407 0000  ully replaced...
+0000a480: 000e 5065 6572 4c69 7374 4469 616c 6f67  ..PeerListDialog
+0000a490: 0103 0000 000c 0027 0020 043d 0430 003a  .......'. .=.0.:
+0000a4a0: 0020 0800 0000 0006 0000 0008 2720 7769  . ..........' wi
+0000a4b0: 7468 3a20 0700 0000 0e50 6565 724c 6973  th: .....PeerLis
+0000a4c0: 7444 6961 6c6f 6701 0300 0000 4e04 2104  tDialog.....N.!.
+0000a4d0: 3e04 4504 4004 3004 3d04 3804 4204 4c00  >.E.@.0.=.8.B.L.
+0000a4e0: 2004 4104 4204 3004 4004 3e04 3500 2004   .A.B.0.@.>.5. .
+0000a4f0: 3d04 3004 3704 3204 3004 3d04 3804 3500  =.0.7.2.0.=.8.5.
+0000a500: 2004 3200 2004 3f04 4004 3804 3c04 3504   .2. .?.@.8.<.5.
+0000a510: 4704 3004 3d04 3804 3800 3f08 0000 0000  G.0.=.8.8.?.....
+0000a520: 0600 0000 174b 6565 7020 6f6c 6420 6e61  .....Keep old na
+0000a530: 6d65 2069 6e20 6e6f 7465 733f 0700 0000  me in notes?....
+0000a540: 0e50 6565 724c 6973 7444 6961 6c6f 6701  .PeerListDialog.
+0000a550: 0300 0000 1804 1a04 3e04 3d04 4204 4004  ........>.=.B.@.
+0000a560: 3004 3304 3504 3d04 4200 2000 2708 0000  0.3.5.=.B. .'...
+0000a570: 0000 0600 0000 0650 6565 7220 2707 0000  .......Peer '...
+0000a580: 000e 5065 6572 4c69 7374 4469 616c 6f67  ..PeerListDialog
+0000a590: 0103 0000 0016 041a 043e 043d 0442 0440  .........>.=.B.@
+0000a5a0: 0430 0433 0435 043d 0442 044b 0800 0000  .0.3.5.=.B.K....
+0000a5b0: 0006 0000 0005 5065 6572 7307 0000 000e  ......Peers.....
+0000a5c0: 5065 6572 4c69 7374 4469 616c 6f67 0103  PeerListDialog..
+0000a5d0: 0000 002c 0417 0430 043c 0435 043d 0438  ...,...0.<.5.=.8
+0000a5e0: 0442 044c 0020 043a 043e 043d 0442 0440  .B.L. .:.>.=.B.@
+0000a5f0: 0430 0433 0435 043d 0442 0430 0020 0027  .0.3.5.=.B.0. .'
+0000a600: 0800 0000 0006 0000 000e 5265 706c 6163  ..........Replac
+0000a610: 6520 7065 6572 2027 0700 0000 0e50 6565  e peer '.....Pee
+0000a620: 724c 6973 7444 6961 6c6f 6701 0300 0000  rListDialog.....
+0000a630: 1c04 1704 3004 3c04 3504 3d04 3804 4204  ....0.<.5.=.8.B.
+0000a640: 4c00 2004 3d04 3000 2e00 2e00 2e08 0000  L. .=.0.........
+0000a650: 0000 0600 0000 0f52 6570 6c61 6365 2077  .......Replace w
+0000a660: 6974 682e 2e2e 0700 0000 0e50 6565 724c  ith........PeerL
+0000a670: 6973 7444 6961 6c6f 6701 0300 0000 4004  istDialog.....@.
+0000a680: 1f04 3e04 3a04 3004 3704 3004 4204 4c00  ..>.:.0.7.0.B.L.
+0000a690: 2004 3e04 3f04 3504 4004 3004 4604 3804   .>.?.5.@.0.F.8.
+0000a6a0: 3800 2004 4100 2004 1a04 3e04 3d04 4204  8. .A. ...>.=.B.
+0000a6b0: 4004 3004 3304 3504 3d04 4204 3e04 3c08  @.0.3.5.=.B.>.<.
+0000a6c0: 0000 0000 0600 0000 1953 686f 7720 6f70  .........Show op
+0000a6d0: 6572 6174 696f 6e73 2077 6974 6820 5065  erations with Pe
+0000a6e0: 6572 0700 0000 0e50 6565 724c 6973 7444  er.....PeerListD
+0000a6f0: 6961 6c6f 6701 0300 0000 1004 1e04 3f04  ialog.........?.
+0000a700: 3504 4004 3004 4604 3804 3808 0000 0000  5.@.0.F.8.8.....
+0000a710: 0600 0000 0a4f 7065 7261 7469 6f6e 7307  .....Operations.
+0000a720: 0000 000a 5065 6572 5265 706f 7274 0103  ....PeerReport..
+0000a730: 0000 001c 043f 043e 0020 041a 043e 043d  .....?.>. ...>.=
+0000a740: 0442 0440 0430 0433 0435 043d 0442 0443  .B.@.0.3.5.=.B.C
+0000a750: 0800 0000 0006 0000 0007 6279 2050 6565  ..........by Pee
+0000a760: 7207 0000 000a 5065 6572 5265 706f 7274  r.....PeerReport
+0000a770: 0103 0000 0016 041a 043e 043d 0442 0440  .........>.=.B.@
+0000a780: 0430 0433 0435 043d 0442 003a 0800 0000  .0.3.5.=.B.:....
+0000a790: 0006 0000 0005 5065 6572 3a07 0000 0010  ......Peer:.....
+0000a7a0: 5065 6572 5265 706f 7274 5769 6467 6574  PeerReportWidget
+0000a7b0: 0103 0000 0028 041e 0442 0447 0435 0442  .....(...B.G.5.B
+0000a7c0: 0020 043f 043e 0020 043a 043e 043d 0442  . .?.>. .:.>.=.B
+0000a7d0: 0440 0430 0433 0435 043d 0442 0443 0800  .@.0.3.5.=.B.C..
+0000a7e0: 0000 0006 0000 000e 5265 706f 7274 2062  ........Report b
+0000a7f0: 7920 7065 6572 0700 0000 1050 6565 7252  y peer.....PeerR
+0000a800: 6570 6f72 7457 6964 6765 7401 0300 0000  eportWidget.....
+0000a810: 1604 1a04 3e04 3b00 2d04 3204 3e00 2004  ....>.;.-.2.>. .
+0000a820: 3404 3e04 3a00 2e08 0000 0000 0600 0000  4.>.:...........
+0000a830: 0a44 6f63 7320 636f 756e 7407 0000 000d  .Docs count.....
+0000a840: 5065 6572 5472 6565 4d6f 6465 6c01 0300  PeerTreeModel...
+0000a850: 0000 0a04 1004 3404 4004 3504 4108 0000  ......4.@.5.A...
+0000a860: 0000 0600 0000 084c 6f63 6174 696f 6e07  .......Location.
+0000a870: 0000 000d 5065 6572 5472 6565 4d6f 6465  ....PeerTreeMode
+0000a880: 6c01 0300 0000 1804 1d04 3004 3804 3c04  l.........0.8.<.
+0000a890: 3504 3d04 3e04 3204 3004 3d04 3804 3508  5.=.>.2.0.=.8.5.
+0000a8a0: 0000 0000 0600 0000 044e 616d 6507 0000  .........Name...
+0000a8b0: 000d 5065 6572 5472 6565 4d6f 6465 6c01  ..PeerTreeModel.
+0000a8c0: 0300 0000 1a04 2104 4704 3504 4204 3000  ......!.G.5.B.0.
+0000a8d0: 2004 3200 2004 3104 3004 3d04 3a04 3508   .2. .1.0.=.:.5.
+0000a8e0: 0000 0000 0600 0000 0d42 616e 6b20 6163  .........Bank ac
+0000a8f0: 636f 756e 7473 0700 0000 1650 7265 6465  counts.....Prede
+0000a900: 6669 6e64 6564 4163 636f 756e 7454 7970  findedAccountTyp
+0000a910: 6501 0300 0000 0a04 1a04 3004 4004 4204  e.........0.@.B.
+0000a920: 4b08 0000 0000 0600 0000 0543 6172 6473  K..........Cards
+0000a930: 0700 0000 1650 7265 6465 6669 6e64 6564  .....Predefinded
+0000a940: 4163 636f 756e 7454 7970 6501 0300 0000  AccountType.....
+0000a950: 1004 1d04 3004 3b04 3804 4704 3d04 4b04  ....0.;.8.G.=.K.
+0000a960: 3508 0000 0000 0600 0000 0443 6173 6807  5..........Cash.
+0000a970: 0000 0016 5072 6564 6566 696e 6465 6441  ....PredefindedA
+0000a980: 6363 6f75 6e74 5479 7065 0103 0000 001e  ccountType......
+0000a990: 041a 0440 0435 0434 0438 0442 044b 0020  ...@.5.4.8.B.K. 
+0000a9a0: 002f 0020 0414 043e 043b 0433 0438 0800  ./. ...>.;.3.8..
+0000a9b0: 0000 0006 0000 000d 4465 6274 7320 2f20  ........Debts / 
+0000a9c0: 4c6f 616e 7307 0000 0016 5072 6564 6566  Loans.....Predef
+0000a9d0: 696e 6465 6441 6363 6f75 6e74 5479 7065  indedAccountType
+0000a9e0: 0103 0000 0014 0418 043d 0432 0435 0441  .........=.2.5.A
+0000a9f0: 0442 0438 0446 0438 0438 0800 0000 0006  .B.8.F.8.8......
+0000aa00: 0000 000b 496e 7665 7374 6d65 6e74 7307  ....Investments.
+0000aa10: 0000 0016 5072 6564 6566 696e 6465 6441  ....PredefindedA
+0000aa20: 6363 6f75 6e74 5479 7065 0103 0000 0014  ccountType......
+0000aa30: 0421 0431 0435 0440 0435 0436 0435 043d  .!.1.5.@.5.6.5.=
+0000aa40: 0438 044f 0800 0000 0006 0000 0007 5361  .8.O..........Sa
+0000aa50: 7669 6e67 7307 0000 0016 5072 6564 6566  vings.....Predef
+0000aa60: 696e 6465 6441 6363 6f75 6e74 5479 7065  indedAccountType
+0000aa70: 0103 0000 0014 0065 002d 041a 043e 0448  .......e.-...>.H
+0000aa80: 0435 043b 044c 043a 0438 0800 0000 0006  .5.;.L.:.8......
+0000aa90: 0000 0009 652d 5761 6c6c 6574 7307 0000  ....e-Wallets...
+0000aaa0: 0016 5072 6564 6566 696e 6465 6441 6363  ..PredefindedAcc
+0000aab0: 6f75 6e74 5479 7065 0103 0000 0012 041e  ountType........
+0000aac0: 0431 043b 0438 0433 0430 0446 0438 0438  .1.;.8.3.0.F.8.8
+0000aad0: 0800 0000 0006 0000 0005 426f 6e64 7307  ..........Bonds.
+0000aae0: 0000 000f 5072 6564 6566 696e 6564 4173  ....PredefinedAs
+0000aaf0: 7365 7401 0300 0000 0c04 2204 3e04 3204  set.......".>.2.
+0000ab00: 3004 4004 4b08 0000 0000 0600 0000 0b43  0.@.K..........C
+0000ab10: 6f6d 6d6f 6469 7469 6573 0700 0000 0f50  ommodities.....P
+0000ab20: 7265 6465 6669 6e65 6441 7373 6574 0103  redefinedAsset..
+0000ab30: 0000 0018 041a 0440 0438 043f 0442 043e  .......@.8.?.B.>
+0000ab40: 0432 0430 043b 044e 0442 044b 0800 0000  .2.0.;.N.B.K....
+0000ab50: 0006 0000 000f 4372 7970 746f 2d63 7572  ......Crypto-cur
+0000ab60: 7265 6e63 7907 0000 000f 5072 6564 6566  rency.....Predef
+0000ab70: 696e 6564 4173 7365 7401 0300 0000 1404  inedAsset.......
+0000ab80: 1404 3504 4004 3804 3204 3004 4204 3804  ..5.@.8.2.0.B.8.
+0000ab90: 3204 4b08 0000 0000 0600 0000 0b44 6572  2.K..........Der
+0000aba0: 6976 6174 6976 6573 0700 0000 0f50 7265  ivatives.....Pre
+0000abb0: 6465 6669 6e65 6441 7373 6574 0103 0000  definedAsset....
+0000abc0: 0008 0411 041f 0418 0424 0800 0000 0006  .........$......
+0000abd0: 0000 0004 4554 4673 0700 0000 0f50 7265  ....ETFs.....Pre
+0000abe0: 6465 6669 6e65 6441 7373 6574 0103 0000  definedAsset....
+0000abf0: 000c 0424 043e 0440 0435 043a 0441 0800  ...$.>.@.5.:.A..
+0000ac00: 0000 0006 0000 0005 466f 7265 7807 0000  ........Forex...
+0000ac10: 000f 5072 6564 6566 696e 6564 4173 7365  ..PredefinedAsse
+0000ac20: 7401 0300 0000 0a04 2404 3e04 3d04 3404  t.......$.>.=.4.
+0000ac30: 4b08 0000 0000 0600 0000 0546 756e 6473  K..........Funds
+0000ac40: 0700 0000 0f50 7265 6465 6669 6e65 6441  .....PredefinedA
+0000ac50: 7373 6574 0103 0000 000c 0412 0430 043b  sset.........0.;
+0000ac60: 044e 0442 044b 0800 0000 0006 0000 0005  .N.B.K..........
+0000ac70: 4d6f 6e65 7907 0000 000f 5072 6564 6566  Money.....Predef
+0000ac80: 696e 6564 4173 7365 7401 0300 0000 0a04  inedAsset.......
+0000ac90: 1004 3a04 4604 3804 3808 0000 0000 0600  ..:.F.8.8.......
+0000aca0: 0000 0653 6861 7265 7307 0000 000f 5072  ...Shares.....Pr
+0000acb0: 6564 6566 696e 6564 4173 7365 7401 0300  edefinedAsset...
+0000acc0: 0000 0200 2508 0000 0000 0600 0000 0125  ....%..........%
+0000acd0: 0700 0000 0f50 726f 6669 744c 6f73 734d  .....ProfitLossM
+0000ace0: 6f64 656c 0103 0000 0006 0410 043f 0440  odel.........?.@
+0000acf0: 0800 0000 0006 0000 0003 4170 7207 0000  ..........Apr...
+0000ad00: 000f 5072 6f66 6974 4c6f 7373 4d6f 6465  ..ProfitLossMode
+0000ad10: 6c01 0300 0000 0404 2604 1108 0000 0000  l.......&.......
+0000ad20: 0600 0000 0641 7373 6574 7307 0000 000f  .....Assets.....
+0000ad30: 5072 6f66 6974 4c6f 7373 4d6f 6465 6c01  ProfitLossModel.
+0000ad40: 0300 0000 0604 1004 3204 3308 0000 0000  ........2.3.....
+0000ad50: 0600 0000 0341 7567 0700 0000 0f50 726f  .....Aug.....Pro
+0000ad60: 6669 744c 6f73 734d 6f64 656c 0103 0000  fitLossModel....
+0000ad70: 0012 0418 0437 043c 0435 043d 0435 043d  .....7.<.5.=.5.=
+0000ad80: 0438 0435 0800 0000 0006 0000 0006 4368  .8.5..........Ch
+0000ad90: 616e 6765 0700 0000 0f50 726f 6669 744c  ange.....ProfitL
+0000ada0: 6f73 734d 6f64 656c 0103 0000 0018 0418  ossModel........
+0000adb0: 0437 043c 0435 043d 0435 043d 0438 0435  .7.<.5.=.5.=.8.5
+0000adc0: 002c 0020 0025 0800 0000 0006 0000 0009  .,. .%..........
+0000add0: 4368 616e 6765 2c20 2507 0000 000f 5072  Change, %.....Pr
+0000ade0: 6f66 6974 4c6f 7373 4d6f 6465 6c01 0300  ofitLossModel...
+0000adf0: 0000 0604 1404 3504 3a08 0000 0000 0600  ......5.:.......
+0000ae00: 0000 0344 6563 0700 0000 0f50 726f 6669  ...Dec.....Profi
+0000ae10: 744c 6f73 734d 6f64 656c 0103 0000 0012  tLossModel......
+0000ae20: 0414 0438 0432 0438 0434 0435 043d 0434  ...8.2.8.4.5.=.4
+0000ae30: 044b 0800 0000 0006 0000 0009 4469 7669  .K..........Divi
+0000ae40: 6465 6e64 7307 0000 000f 5072 6f66 6974  dends.....Profit
+0000ae50: 4c6f 7373 4d6f 6465 6c01 0300 0000 0604  LossModel.......
+0000ae60: 2404 3504 3208 0000 0000 0600 0000 0346  $.5.2..........F
+0000ae70: 6562 0700 0000 0f50 726f 6669 744c 6f73  eb.....ProfitLos
+0000ae80: 734d 6f64 656c 0103 0000 0010 041a 043e  sModel.........>
+0000ae90: 043c 0438 0441 0441 0438 0438 0800 0000  .<.8.A.A.8.8....
+0000aea0: 0006 0000 0004 4665 6573 0700 0000 0f50  ......Fees.....P
+0000aeb0: 726f 6669 744c 6f73 734d 6f64 656c 0103  rofitLossModel..
+0000aec0: 0000 0018 0412 0432 043e 0434 0020 002f  .......2.>.4. ./
+0000aed0: 0020 0412 044b 0432 043e 0434 0800 0000  . ...K.2.>.4....
+0000aee0: 0006 0000 0008 496e 202f 204f 7574 0700  ......In / Out..
+0000aef0: 0000 0f50 726f 6669 744c 6f73 734d 6f64  ...ProfitLossMod
+0000af00: 656c 0103 0000 0006 042f 043d 0432 0800  el......./.=.2..
+0000af10: 0000 0006 0000 0003 4a61 6e07 0000 000f  ........Jan.....
+0000af20: 5072 6f66 6974 4c6f 7373 4d6f 6465 6c01  ProfitLossModel.
+0000af30: 0300 0000 0604 1804 4e04 3b08 0000 0000  ........N.;.....
+0000af40: 0600 0000 034a 756c 0700 0000 0f50 726f  .....Jul.....Pro
+0000af50: 6669 744c 6f73 734d 6f64 656c 0103 0000  fitLossModel....
+0000af60: 0006 0418 044e 043d 0800 0000 0006 0000  .....N.=........
+0000af70: 0003 4a75 6e07 0000 000f 5072 6f66 6974  ..Jun.....Profit
+0000af80: 4c6f 7373 4d6f 6465 6c01 0300 0000 0604  LossModel.......
+0000af90: 1c04 3004 4008 0000 0000 0600 0000 034d  ..0.@..........M
+0000afa0: 6172 0700 0000 0f50 726f 6669 744c 6f73  ar.....ProfitLos
+0000afb0: 734d 6f64 656c 0103 0000 0006 041c 0430  sModel.........0
+0000afc0: 0439 0800 0000 0006 0000 0003 4d61 7907  .9..........May.
+0000afd0: 0000 000f 5072 6f66 6974 4c6f 7373 4d6f  ....ProfitLossMo
+0000afe0: 6465 6c01 0300 0000 0404 1404 2108 0000  del.........!...
+0000aff0: 0000 0600 0000 054d 6f6e 6579 0700 0000  .......Money....
+0000b000: 0f50 726f 6669 744c 6f73 734d 6f64 656c  .ProfitLossModel
+0000b010: 0103 0000 0006 041d 043e 044f 0800 0000  .........>.O....
+0000b020: 0006 0000 0003 4e6f 7607 0000 000f 5072  ......Nov.....Pr
+0000b030: 6f66 6974 4c6f 7373 4d6f 6465 6c01 0300  ofitLossModel...
+0000b040: 0000 0604 1e04 3a04 4208 0000 0000 0600  ......:.B.......
+0000b050: 0000 034f 6374 0700 0000 0f50 726f 6669  ...Oct.....Profi
+0000b060: 744c 6f73 734d 6f64 656c 0103 0000 0006  tLossModel......
+0000b070: 041f 0438 0423 0800 0000 0006 0000 0003  ...8.#..........
+0000b080: 5026 4c07 0000 000f 5072 6f66 6974 4c6f  P&L.....ProfitLo
+0000b090: 7373 4d6f 6465 6c01 0300 0000 0c04 1f04  ssModel.........
+0000b0a0: 3504 4004 3804 3e04 3408 0000 0000 0600  5.@.8.>.4.......
+0000b0b0: 0000 0650 6572 696f 6407 0000 000f 5072  ...Period.....Pr
+0000b0c0: 6f66 6974 4c6f 7373 4d6f 6465 6c01 0300  ofitLossModel...
+0000b0d0: 0000 1a04 1a04 3e04 3d04 3504 4600 2004  ......>.=.5.F. .
+0000b0e0: 3f04 3504 4004 3804 3e04 3404 3008 0000  ?.5.@.8.>.4.0...
+0000b0f0: 0000 0600 0000 0a50 6572 696f 6420 656e  .......Period en
+0000b100: 6407 0000 000f 5072 6f66 6974 4c6f 7373  d.....ProfitLoss
+0000b110: 4d6f 6465 6c01 0300 0000 1c04 1d04 3004  Model.........0.
+0000b120: 4704 3004 3b04 3e00 2004 3f04 3504 4004  G.0.;.>. .?.5.@.
+0000b130: 3804 3e04 3404 3008 0000 0000 0600 0000  8.>.4.0.........
+0000b140: 0c50 6572 696f 6420 7374 6172 7407 0000  .Period start...
+0000b150: 000f 5072 6f66 6974 4c6f 7373 4d6f 6465  ..ProfitLossMode
+0000b160: 6c01 0300 0000 0604 2104 3504 3d08 0000  l.......!.5.=...
+0000b170: 0000 0600 0000 0353 6570 0700 0000 0f50  .......Sep.....P
+0000b180: 726f 6669 744c 6f73 734d 6f64 656c 0103  rofitLossModel..
+0000b190: 0000 000c 041d 0430 043b 043e 0433 0438  .......0.;.>.3.8
+0000b1a0: 0800 0000 0006 0000 0005 5461 7865 7307  ..........Taxes.
+0000b1b0: 0000 000f 5072 6f66 6974 4c6f 7373 4d6f  ....ProfitLossMo
+0000b1c0: 6465 6c01 0300 0000 0a04 1804 4204 3e04  del.........B.>.
+0000b1d0: 3304 3e08 0000 0000 0600 0000 0554 6f74  3.>..........Tot
+0000b1e0: 616c 0700 0000 0f50 726f 6669 744c 6f73  al.....ProfitLos
+0000b1f0: 734d 6f64 656c 0103 0000 0018 041f 0438  sModel.........8
+0000b200: 0423 0020 043f 043e 0020 0441 0447 0451  .#. .?.>. .A.G.Q
+0000b210: 0442 0443 0800 0000 0006 0000 000e 5026  .B.C..........P&
+0000b220: 4c20 6279 2041 6363 6f75 6e74 0700 0000  L by Account....
+0000b230: 1050 726f 6669 744c 6f73 7352 6570 6f72  .ProfitLossRepor
+0000b240: 7401 0300 0000 0a04 2104 4704 3504 4200  t.......!.G.5.B.
+0000b250: 3a08 0000 0000 0600 0000 0841 6363 6f75  :..........Accou
+0000b260: 6e74 3a07 0000 0016 5072 6f66 6974 4c6f  nt:.....ProfitLo
+0000b270: 7373 5265 706f 7274 5769 6467 6574 0103  ssReportWidget..
+0000b280: 0000 0010 0412 0430 043b 044e 0442 0430  .......0.;.N.B.0
+0000b290: 003a 0020 0800 0000 0006 0000 000a 4375  .:. ..........Cu
+0000b2a0: 7272 656e 6379 3a20 0700 0000 1650 726f  rrency: .....Pro
+0000b2b0: 6669 744c 6f73 7352 6570 6f72 7457 6964  fitLossReportWid
+0000b2c0: 6765 7401 0300 0000 0604 1f04 3804 2308  get.........8.#.
+0000b2d0: 0000 0000 0600 0000 0350 264c 0700 0000  .........P&L....
+0000b2e0: 1650 726f 6669 744c 6f73 7352 6570 6f72  .ProfitLossRepor
+0000b2f0: 7457 6964 6765 7401 0300 0000 1804 2104  tWidget.......!.
+0000b300: 3e04 4504 4004 3004 3d04 3804 4204 4c00  >.E.@.0.=.8.B.L.
+0000b310: 2e00 2e00 2e08 0000 0000 0600 0000 0753  ...............S
+0000b320: 6176 652e 2e2e 0700 0000 1650 726f 6669  ave........Profi
+0000b330: 744c 6f73 7352 6570 6f72 7457 6964 6765  tLossReportWidge
+0000b340: 7401 0300 0000 1004 1204 3004 3b04 4e04  t.........0.;.N.
+0000b350: 4204 3000 3a00 2008 0000 0000 0600 0000  B.0.:. .........
+0000b360: 0a43 7572 7265 6e63 793a 2007 0000 0016  .Currency: .....
+0000b370: 5072 6f66 6974 4c6f 7373 5265 706f 7274  ProfitLossReport
+0000b380: 5769 6e64 6f77 0103 0000 0018 041f 0438  Window.........8
+0000b390: 0423 0020 043f 043e 0020 0441 0447 0451  .#. .?.>. .A.G.Q
+0000b3a0: 0442 0443 0800 0000 0006 0000 000e 5026  .B.C..........P&
+0000b3b0: 4c20 6279 2041 6363 6f75 6e74 0700 0000  L by Account....
+0000b3c0: 1650 726f 6669 744c 6f73 7352 6570 6f72  .ProfitLossRepor
+0000b3d0: 7457 696e 646f 7701 0300 0000 1e04 1e04  tWindow.........
+0000b3e0: 4804 3804 3104 3a04 3000 2004 3a04 3004  H.8.1.:.0. .:.0.
+0000b3f0: 3c04 3504 4004 4b00 3a00 2008 0000 0000  <.5.@.K.:. .....
+0000b400: 0600 0000 0e43 616d 6572 6120 6572 726f  .....Camera erro
+0000b410: 723a 2007 0000 0009 5152 5363 616e 6e65  r: .....QRScanne
+0000b420: 7201 0300 0000 8404 1d04 3500 2004 3e04  r.........5. .>.
+0000b430: 3104 3d04 3004 4004 4304 3604 3504 3d00  1.=.0.@.C.6.5.=.
+0000b440: 2004 3f04 3004 3a04 3504 4200 2000 7000   .?.0.:.5.B. .p.
+0000b450: 7900 7a00 6200 6100 7200 2c00 2004 3d04  y.z.b.a.r.,. .=.
+0000b460: 3504 3e04 3104 4504 3e04 3404 3804 3c04  5.>.1.E.>.4.8.<.
+0000b470: 4b04 3900 2004 3404 3b04 4f00 2004 4004  K.9. .4.;.O. .@.
+0000b480: 3004 4104 3f04 3e04 3704 3d04 3004 3204  0.A.?.>.7.=.0.2.
+0000b490: 3004 3d04 3804 4f00 2000 5100 5200 2004  0.=.8.O. .Q.R. .
+0000b4a0: 3a04 3e04 3404 3e04 3200 2e08 0000 0000  :.>.4.>.2.......
+0000b4b0: 0600 0000 2c50 6163 6b61 6765 2070 797a  ....,Package pyz
+0000b4c0: 6261 7220 6e6f 7420 666f 756e 6420 666f  bar not found fo
+0000b4d0: 7220 5152 2072 6563 6f67 6e69 7469 6f6e  r QR recognition
+0000b4e0: 2e07 0000 0009 5152 5363 616e 6e65 7201  ......QRScanner.
+0000b4f0: 0300 0000 2604 1d04 3504 4200 2004 3404  ....&...5.B. .4.
+0000b500: 3e04 4104 4204 4304 3f04 3d04 4b04 4500  >.A.B.C.?.=.K.E.
+0000b510: 2004 3a04 3004 3c04 3504 4008 0000 0000   .:.0.<.5.@.....
+0000b520: 0600 0000 1e54 6865 7265 2061 7265 206e  .....There are n
+0000b530: 6f20 6361 6d65 7261 7320 6176 6169 6c61  o cameras availa
+0000b540: 626c 6507 0000 0009 5152 5363 616e 6e65  ble.....QRScanne
+0000b550: 7201 0300 0000 6804 1d04 3504 3204 3e04  r.....h...5.2.>.
+0000b560: 3704 3c04 3e04 3604 3d04 3e00 2004 3e04  7.<.>.6.=.>. .>.
+0000b570: 3104 4004 3004 3104 3e04 4204 3004 4204  1.@.0.1.>.B.0.B.
+0000b580: 4c00 2004 3404 3004 3d04 3d04 4b04 3500  L. .4.0.=.=.K.5.
+0000b590: 2004 3a04 3e04 4204 3804 4004 3e04 3204   .:.>.B.8.@.>.2.
+0000b5a0: 3e04 3a00 2004 4100 2004 3104 3804 4004  >.:. .A. .1.8.@.
+0000b5b0: 3604 3800 2000 5400 5300 5800 3a00 2008  6.8. .T.S.X.:. .
+0000b5c0: 0000 0000 0600 0000 2143 616e 2774 2070  ........!Can't p
+0000b5d0: 6172 7365 2064 6174 6120 666f 7220 5453  arse data for TS
+0000b5e0: 5820 7175 6f74 6573 3a20 0700 0000 0f51  X quotes: .....Q
+0000b5f0: 756f 7465 446f 776e 6c6f 6164 6572 0103  uoteDownloader..
+0000b600: 0000 0024 0417 0430 0433 0440 0443 0437  ...$...0.3.@.C.7
+0000b610: 043a 0430 0020 0437 0430 0432 0435 0440  .:.0. .7.0.2.5.@
+0000b620: 0448 0435 043d 0430 0800 0000 0006 0000  .H.5.=.0........
+0000b630: 0012 446f 776e 6c6f 6164 2063 6f6d 706c  ..Download compl
+0000b640: 6574 6564 0700 0000 0f51 756f 7465 446f  eted.....QuoteDo
+0000b650: 776e 6c6f 6164 6572 0103 0000 0060 0049  wnloader.....`.I
+0000b660: 0053 0049 004e 0020 0432 0020 0438 0441  .S.I.N. .2. .8.A
+0000b670: 0442 043e 0440 0438 0438 0020 043a 043e  .B.>.@.8.8. .:.>
+0000b680: 0442 0438 0440 043e 0432 043e 043a 0020  .B.8.@.>.2.>.:. 
+0000b690: 0045 0075 0072 006f 006e 0065 0078 0074  .E.u.r.o.n.e.x.t
+0000b6a0: 0020 043d 0435 0020 0441 043e 0432 043f  . .=.5. .A.>.2.?
+0000b6b0: 0430 0434 0430 0435 0442 003a 0020 0800  .0.4.0.5.B.:. ..
+0000b6c0: 0000 0006 0000 0022 4575 726f 6e65 7874  ......."Euronext
+0000b6d0: 2071 756f 7465 7320 4953 494e 206d 6973   quotes ISIN mis
+0000b6e0: 6d61 7463 6820 696e 3a20 0700 0000 0f51  match in: .....Q
+0000b6f0: 756f 7465 446f 776e 6c6f 6164 6572 0103  uoteDownloader..
+0000b700: 0000 0064 0417 0430 0433 043e 043b 043e  ...d...0.3.>.;.>
+0000b710: 0432 043e 043a 0020 0438 0441 0442 043e  .2.>.:. .8.A.B.>
+0000b720: 0440 0438 0438 0020 043a 043e 0442 0438  .@.8.8. .:.>.B.8
+0000b730: 0440 043e 0432 043e 043a 0020 0045 0075  .@.>.2.>.:. .E.u
+0000b740: 0072 006f 006e 0065 0078 0074 0020 043d  .r.o.n.e.x.t. .=
+0000b750: 0435 0020 043d 0430 0439 0434 0435 043d  .5. .=.0.9.4.5.=
+0000b760: 0020 0432 003a 0020 0800 0000 0006 0000  . .2.:. ........
+0000b770: 0025 4575 726f 6e65 7874 2071 756f 7465  .%Euronext quote
+0000b780: 7320 6865 6164 6572 206e 6f74 2066 6f75  s header not fou
+0000b790: 6e64 2069 6e3a 2007 0000 000f 5175 6f74  nd in: .....Quot
+0000b7a0: 6544 6f77 6e6c 6f61 6465 7201 0300 0000  eDownloader.....
+0000b7b0: 5a04 1804 4104 4204 3e04 4004 3804 4f00  Z...A.B.>.@.8.O.
+0000b7c0: 2004 3a04 3e04 4204 3804 4004 3e04 3204   .:.>.B.8.@.>.2.
+0000b7d0: 3e04 3a00 2000 4500 7500 7200 6f00 6e00  >.:. .E.u.r.o.n.
+0000b7e0: 6500 7800 7400 2004 4104 3b04 3804 4804  e.x.t. .A.;.8.H.
+0000b7f0: 3a04 3e04 3c00 2004 3a04 3e04 4004 3e04  :.>.<. .:.>.@.>.
+0000b800: 4204 3a04 3004 4f00 3a00 2008 0000 0000  B.:.0.O.:. .....
+0000b810: 0600 0000 2c45 7572 6f6e 6578 7420 7175  ....,Euronext qu
+0000b820: 6f74 6573 2068 6973 746f 7279 2072 6570  otes history rep
+0000b830: 6c79 2069 7320 746f 6f20 7368 6f72 743a  ly is too short:
+0000b840: 2007 0000 000f 5175 6f74 6544 6f77 6e6c   .....QuoteDownl
+0000b850: 6f61 6465 7201 0300 0000 3604 1d04 3500  oader.....6...5.
+0000b860: 2004 3704 3004 3304 4004 4304 3604 3504   .7.0.3.@.C.6.5.
+0000b870: 3d04 4b00 2004 3a04 3e04 4204 3804 4004  =.K. .:.>.B.8.@.
+0000b880: 3e04 3204 3a04 3800 2004 3404 3b04 4f00  >.2.:.8. .4.;.O.
+0000b890: 2008 0000 0000 0600 0000 1e4e 6f20 7175   ..........No qu
+0000b8a0: 6f74 6573 2077 6572 6520 646f 776e 6c6f  otes were downlo
+0000b8b0: 6164 6564 2066 6f72 2007 0000 000f 5175  aded for .....Qu
+0000b8c0: 6f74 6544 6f77 6e6c 6f61 6465 7201 0300  oteDownloader...
+0000b8d0: 0000 2e04 1d04 3500 2004 3704 3004 3304  ......5. .7.0.3.
+0000b8e0: 4004 4304 3604 3504 3d04 4b00 2004 3a04  @.C.6.5.=.K. .:.
+0000b8f0: 4304 4004 4104 4b00 2004 3404 3b04 4f00  C.@.A.K. .4.;.O.
+0000b900: 2008 0000 0000 0600 0000 1d4e 6f20 7261   ..........No ra
+0000b910: 7465 7320 7765 7265 2064 6f77 6e6c 6f61  tes were downloa
+0000b920: 6465 6420 666f 7220 0700 0000 0f51 756f  ded for .....Quo
+0000b930: 7465 446f 776e 6c6f 6164 6572 0103 0000  teDownloader....
+0000b940: 002c 041d 0435 0442 0020 0434 0430 043d  .,...5.B. .4.0.=
+0000b950: 043d 044b 0445 0020 0426 0411 0020 0420  .=.K.E. .&... . 
+0000b960: 0424 0020 0434 043b 044f 003a 0020 0800  .$. .4.;.O.:. ..
+0000b970: 0000 0006 0000 001b 5468 6572 6520 6172  ........There ar
+0000b980: 6520 6e6f 2043 4252 2064 6174 6120 666f  e no CBR data fo
+0000b990: 723a 2007 0000 000f 5175 6f74 6544 6f77  r: .....QuoteDow
+0000b9a0: 6e6c 6f61 6465 7201 0300 0000 1204 1a04  nloader.........
+0000b9b0: 3e04 4204 3804 4004 3e04 3204 3a04 3808  >.B.8.@.>.2.:.8.
+0000b9c0: 0000 0000 0600 0000 0651 756f 7465 7307  .........Quotes.
+0000b9d0: 0000 0010 5175 6f74 6573 4c69 7374 4469  ....QuotesListDi
+0000b9e0: 616c 6f67 0103 0000 0004 0426 0411 0800  alog.......&....
+0000b9f0: 0000 0006 0000 0005 4173 7365 7407 0000  ........Asset...
+0000ba00: 000f 5175 6f74 6573 4c69 7374 4d6f 6465  ..QuotesListMode
+0000ba10: 6c01 0300 0000 0c04 1204 3004 3b04 4e04  l.........0.;.N.
+0000ba20: 4204 3008 0000 0000 0600 0000 0843 7572  B.0..........Cur
+0000ba30: 7265 6e63 7907 0000 000f 5175 6f74 6573  rency.....Quotes
+0000ba40: 4c69 7374 4d6f 6465 6c01 0300 0000 0804  ListModel.......
+0000ba50: 1404 3004 4204 3008 0000 0000 0600 0000  ..0.B.0.........
+0000ba60: 0444 6174 6507 0000 000f 5175 6f74 6573  .Date.....Quotes
+0000ba70: 4c69 7374 4d6f 6465 6c01 0300 0000 1204  ListModel.......
+0000ba80: 1a04 3e04 4204 3804 4004 3e04 3204 3a04  ..>.B.8.@.>.2.:.
+0000ba90: 3008 0000 0000 0600 0000 0551 756f 7465  0..........Quote
+0000baa0: 0700 0000 0f51 756f 7465 734c 6973 744d  .....QuotesListM
+0000bab0: 6f64 656c 0103 0000 0028 0026 041f 043e  odel.....(.&...>
+0000bac0: 043b 043d 043e 0441 0442 044c 044e 002c  .;.=.>.A.B.L.N.,
+0000bad0: 0020 0441 0020 043d 0430 0447 0430 043b  . .A. .=.0.G.0.;
+0000bae0: 0430 0800 0000 0006 0000 0013 2646 756c  .0..........&Ful
+0000baf0: 6c2c 2066 726f 6d20 7363 7261 7463 6807  l, from scratch.
+0000bb00: 0000 000d 5265 4275 696c 6444 6961 6c6f  ....ReBuildDialo
+0000bb10: 6701 0300 0000 1804 1804 3d04 4204 3504  g.........=.B.5.
+0000bb20: 4004 3204 3004 3b00 2004 3404 3004 4208  @.2.0.;. .4.0.B.
+0000bb30: 0000 0000 0600 0000 0a44 6174 6520 5261  .........Date Ra
+0000bb40: 6e67 6507 0000 000d 5265 4275 696c 6444  nge.....ReBuildD
+0000bb50: 6961 6c6f 6701 0300 0000 2a00 2604 1104  ialog.....*.&...
+0000bb60: 4b04 4104 4204 4004 3e00 2c00 2004 3d04  K.A.B.@.>.,. .=.
+0000bb70: 3e00 2004 3d04 3504 3d04 3004 3404 5104  >. .=.5.=.0.4.Q.
+0000bb80: 3604 3d04 3e08 0000 0000 0600 0000 1146  6.=.>..........F
+0000bb90: 6173 742c 2026 756e 7265 6c69 6162 6c65  ast, &unreliable
+0000bba0: 0700 0000 0d52 6542 7569 6c64 4469 616c  .....ReBuildDial
+0000bbb0: 6f67 0103 0000 0016 0414 0430 0442 0430  og.........0.B.0
+0000bbc0: 0413 0440 0430 043d 0438 0446 044b 0800  ...@.0.=.8.F.K..
+0000bbd0: 0000 0006 0000 000c 4672 6f6e 7469 6572  ........Frontier
+0000bbe0: 4461 7465 0700 0000 0d52 6542 7569 6c64  Date.....ReBuild
+0000bbf0: 4469 616c 6f67 0103 0000 0022 041f 0435  Dialog....."...5
+0000bc00: 0440 0435 0441 0447 0438 0442 0430 0442  .@.5.A.G.8.B.0.B
+0000bc10: 044c 0020 0438 0442 043e 0433 0438 0800  .L. .8.B.>.3.8..
+0000bc20: 0000 0006 0000 000f 5265 2d42 7569 6c64  ........Re-Build
+0000bc30: 204c 6564 6765 7207 0000 000d 5265 4275   Ledger.....ReBu
+0000bc40: 696c 6444 6961 6c6f 6701 0300 0000 1004  ildDialog.......
+0000bc50: 2100 2000 2604 1404 3004 4204 4b00 3a08  !. .&...0.B.K.:.
+0000bc60: 0000 0000 0600 0000 0c53 696e 6365 2026  .........Since &
+0000bc70: 4461 7465 3a07 0000 000d 5265 4275 696c  Date:.....ReBuil
+0000bc80: 6444 6961 6c6f 6701 0300 0000 2c04 2100  dDialog.....,.!.
+0000bc90: 2004 3a04 4004 3004 3904 3d04 3504 3900   .:.@.0.9.=.5.9.
+0000bca0: 2000 2604 3004 3a04 4204 4304 3004 3b04   .&.0.:.B.C.0.;.
+0000bcb0: 4c04 3d04 3e04 3900 3a08 0000 0000 0600  L.=.>.9.:.......
+0000bcc0: 0000 1353 696e 6365 2026 4c61 7374 2061  ...Since &Last a
+0000bcd0: 6374 7561 6c3a 0700 0000 0d52 6542 7569  ctual:.....ReBui
+0000bce0: 6c64 4469 616c 6f67 0103 0000 0014 0064  ldDialog.......d
+0000bcf0: 0064 002f 004d 004d 002f 0079 0079 0079  .d./.M.M./.y.y.y
+0000bd00: 0079 0800 0000 0006 0000 000a 6464 2f4d  .y..........dd/M
+0000bd10: 4d2f 7979 7979 0700 0000 0d52 6542 7569  M/yyyy.....ReBui
+0000bd20: 6c64 4469 616c 6f67 0103 0000 000a 041b  ldDialog........
+0000bd30: 044e 0431 043e 0439 0800 0000 0006 0000  .N.1.>.9........
+0000bd40: 0003 414e 5907 0000 0013 5265 6665 7265  ..ANY.....Refere
+0000bd50: 6e63 6544 6174 6144 6961 6c6f 6701 0300  nceDataDialog...
+0000bd60: 0000 1404 2204 3804 3f00 2004 4104 4704  ....".8.?. .A.G.
+0000bd70: 3504 4204 3000 3a08 0000 0000 0600 0000  5.B.0.:.........
+0000bd80: 0d41 6363 6f75 6e74 2054 7970 653a 0700  .Account Type:..
+0000bd90: 0000 1352 6566 6572 656e 6365 4461 7461  ...ReferenceData
+0000bda0: 4469 616c 6f67 0103 0000 0022 0414 043e  Dialog....."...>
+0000bdb0: 0431 0430 0432 0438 0442 044c 0020 0434  .1.0.2.8.B.L. .4
+0000bdc0: 043e 0447 0435 0440 043d 0438 0439 0800  .>.G.5.@.=.8.9..
+0000bdd0: 0000 0006 0000 0009 4164 6420 6368 696c  ........Add chil
+0000bde0: 6407 0000 0013 5265 6665 7265 6e63 6544  d.....ReferenceD
+0000bdf0: 6174 6144 6961 6c6f 6701 0300 0000 1c04  ataDialog.......
+0000be00: 1404 3e04 3104 3004 3204 3804 4204 4c00  ..>.1.0.2.8.B.L.
+0000be10: 2004 3d04 3e04 3204 4b04 3908 0000 0000   .=.>.2.K.9.....
+0000be20: 0600 0000 0741 6464 206e 6577 0700 0000  .....Add new....
+0000be30: 1352 6566 6572 656e 6365 4461 7461 4469  .ReferenceDataDi
+0000be40: 616c 6f67 0103 0000 001e 0421 043c 0435  alog.......!.<.5
+0000be50: 043d 0438 0442 044c 0020 0442 0438 043f  .=.8.B.L. .B.8.?
+0000be60: 0020 043d 0430 003a 0800 0000 0006 0000  . .=.0.:........
+0000be70: 000f 4368 616e 6765 2074 7970 6520 746f  ..Change type to
+0000be80: 3a07 0000 0013 5265 6665 7265 6e63 6544  :.....ReferenceD
+0000be90: 6174 6144 6961 6c6f 6701 0300 0000 1a04  ataDialog.......
+0000bea0: 1f04 3e04 3404 4204 3204 3504 4004 3604  ..>.4.B.2.5.@.6.
+0000beb0: 3404 3504 3d04 3804 3508 0000 0000 0600  4.5.=.8.5.......
+0000bec0: 0000 0c43 6f6e 6669 726d 6174 696f 6e07  ...Confirmation.
+0000bed0: 0000 0013 5265 6665 7265 6e63 6544 6174  ....ReferenceDat
+0000bee0: 6144 6961 6c6f 6701 0300 0000 0e04 2304  aDialog.......#.
+0000bef0: 3404 3004 3b04 3804 4204 4c08 0000 0000  4.0.;.8.B.L.....
+0000bf00: 0600 0000 0644 656c 6574 6507 0000 0013  .....Delete.....
+0000bf10: 5265 6665 7265 6e63 6544 6174 6144 6961  ReferenceDataDia
+0000bf20: 6c6f 6701 0300 0000 2204 2104 3f04 4004  log.....".!.?.@.
+0000bf30: 3004 3204 3e04 4704 3d04 4b04 3500 2004  0.2.>.G.=.K.5. .
+0000bf40: 3404 3004 3d04 3d04 4b04 3508 0000 0000  4.0.=.=.K.5.....
+0000bf50: 0600 0000 0e52 6566 6572 656e 6365 2044  .....Reference D
+0000bf60: 6174 6107 0000 0013 5265 6665 7265 6e63  ata.....Referenc
+0000bf70: 6544 6174 6144 6961 6c6f 6701 0300 0000  eDataDialog.....
+0000bf80: 2404 1e04 4204 3c04 3504 3d04 3804 4204  $...B.<.5.=.8.B.
+0000bf90: 4c00 2004 3804 3704 3c04 3504 3d04 3504  L. .8.7.<.5.=.5.
+0000bfa0: 3d04 3804 4f08 0000 0000 0600 0000 0e52  =.8.O..........R
+0000bfb0: 6576 6572 7420 6368 616e 6765 7307 0000  evert changes...
+0000bfc0: 0013 5265 6665 7265 6e63 6544 6174 6144  ..ReferenceDataD
+0000bfd0: 6961 6c6f 6701 0300 0000 2604 2104 3e04  ialog.....&.!.>.
+0000bfe0: 4504 4004 3004 3d04 3804 4204 4c00 2004  E.@.0.=.8.B.L. .
+0000bff0: 3804 3704 3c04 3504 3d04 3504 3d04 3804  8.7.<.5.=.5.=.8.
+0000c000: 4f08 0000 0000 0600 0000 0c53 6176 6520  O..........Save 
+0000c010: 6368 616e 6765 7307 0000 0013 5265 6665  changes.....Refe
+0000c020: 7265 6e63 6544 6174 6144 6961 6c6f 6701  renceDataDialog.
+0000c030: 0300 0000 0c04 1f04 3e04 3804 4104 3a00  ........>.8.A.:.
+0000c040: 3a08 0000 0000 0600 0000 0753 6561 7263  :..........Searc
+0000c050: 683a 0700 0000 1352 6566 6572 656e 6365  h:.....Reference
+0000c060: 4461 7461 4469 616c 6f67 0103 0000 002a  DataDialog.....*
+0000c070: 041f 043e 043a 0430 0437 044b 0432 0430  ...>.:.0.7.K.2.0
+0000c080: 0442 044c 0020 043d 0435 0430 043a 0442  .B.L. .=.5.0.:.B
+0000c090: 0438 0432 043d 044b 0435 0800 0000 0006  .8.2.=.K.5......
+0000c0a0: 0000 000d 5368 6f77 2069 6e61 6374 6976  ....Show inactiv
+0000c0b0: 6507 0000 0013 5265 6665 7265 6e63 6544  e.....ReferenceD
+0000c0c0: 6174 6144 6961 6c6f 6701 0300 0000 6604  ataDialog.....f.
+0000c0d0: 2300 2004 3204 3004 4100 2004 3504 4104  #. .2.0.A. .5.A.
+0000c0e0: 4204 4c00 2004 3d04 3504 4104 3e04 4504  B.L. .=.5.A.>.E.
+0000c0f0: 4004 3004 3d04 5104 3d04 3d04 4b04 3500  @.0.=.Q.=.=.K.5.
+0000c100: 2004 3404 3004 3d04 3d04 4b04 3500 2e00   .4.0.=.=.K.5...
+0000c110: 2004 1204 4104 5100 2004 4004 3004 3204   ...A.Q. .@.0.2.
+0000c120: 3d04 3e00 2004 3704 3004 3a04 4004 4b04  =.>. .7.0.:.@.K.
+0000c130: 4204 4c00 3f08 0000 0000 0600 0000 3359  B.L.?.........3Y
+0000c140: 6f75 2068 6176 6520 756e 636f 6d6d 6974  ou have uncommit
+0000c150: 7465 6420 6368 616e 6765 732e 2044 6f20  ted changes. Do 
+0000c160: 796f 7520 7761 6e74 2074 6f20 636c 6f73  you want to clos
+0000c170: 653f 0700 0000 1352 6566 6572 656e 6365  e?.....Reference
+0000c180: 4461 7461 4469 616c 6f67 0103 0000 0028  DataDialog.....(
+0000c190: 0424 0430 0439 043b 044b 0020 0045 0078  .$.0.9.;.K. .E.x
+0000c1a0: 0063 0065 006c 0020 0028 002a 002e 0078  .c.e.l. .(.*...x
+0000c1b0: 0073 006c 0078 0029 0800 0000 0006 0000  .s.l.x.)........
+0000c1c0: 0014 4578 6365 6c20 6669 6c65 7320 282a  ..Excel files (*
+0000c1d0: 2e78 6c73 7829 0700 0000 0752 6570 6f72  .xlsx).....Repor
+0000c1e0: 7473 0103 0000 0046 041d 0435 0432 043e  ts.....F...5.2.>
+0000c1f0: 0437 043c 043e 0436 043d 043e 0020 0437  .7.<.>.6.=.>. .7
+0000c200: 0430 0433 0440 0443 0437 0438 0442 044c  .0.3.@.C.7.8.B.L
+0000c210: 0020 043a 043b 0430 0441 0441 0020 043e  . .:.;.0.A.A. .>
+0000c220: 0442 0447 0451 0442 0430 003a 0020 0800  .B.G.Q.B.0.:. ..
+0000c230: 0000 0006 0000 001e 5265 706f 7274 2063  ........Report c
+0000c240: 6c61 7373 2063 616e 2774 2062 6520 6c6f  lass can't be lo
+0000c250: 6164 6564 3a20 0700 0000 0752 6570 6f72  aded: .....Repor
+0000c260: 7473 0103 0000 0042 041e 0442 0447 0435  ts.....B...B.G.5
+0000c270: 0442 0020 043d 0435 0020 043d 0430 0439  .B. .=.5. .=.0.9
+0000c280: 0434 0435 043d 0020 0434 043b 044f 0020  .4.5.=. .4.;.O. 
+0000c290: 043a 043b 0430 0441 0441 0430 0020 043e  .:.;.0.A.A.0. .>
+0000c2a0: 043a 043d 0430 003a 0020 0800 0000 0006  .:.=.0.:. ......
+0000c2b0: 0000 0023 5265 706f 7274 206e 6f74 2066  ...#Report not f
+0000c2c0: 6f75 6e64 2066 6f72 2077 696e 646f 7720  ound for window 
+0000c2d0: 636c 6173 733a 2007 0000 0007 5265 706f  class: .....Repo
+0000c2e0: 7274 7301 0300 0000 2c04 1e04 4204 4704  rts.....,...B.G.
+0000c2f0: 3504 4200 2004 4104 3e04 4504 4004 3004  5.B. .A.>.E.@.0.
+0000c300: 3d04 5104 3d00 2004 3200 2004 4404 3004  =.Q.=. .2. .D.0.
+0000c310: 3904 3b00 2008 0000 0000 0600 0000 1952  9.;. ..........R
+0000c320: 6570 6f72 7420 7761 7320 7361 7665 6420  eport was saved 
+0000c330: 746f 2066 696c 6520 0700 0000 0752 6570  to file .....Rep
+0000c340: 6f72 7473 0103 0000 0024 0421 043e 0445  orts.....$.!.>.E
+0000c350: 0440 0430 043d 0438 0442 044c 0020 043e  .@.0.=.8.B.L. .>
+0000c360: 0442 0447 0435 0442 0020 0432 003a 0800  .B.G.5.B. .2.:..
+0000c370: 0000 0006 0000 000f 5361 7665 2072 6570  ........Save rep
+0000c380: 6f72 7420 746f 3a07 0000 0007 5265 706f  ort to:.....Repo
+0000c390: 7274 7301 0300 0000 3c04 1b04 3e04 3304  rts.....<...>.3.
+0000c3a0: 3804 3d00 2004 4704 3504 4004 3504 3700  8.=. .G.5.@.5.7.
+0000c3b0: 2004 1304 3e04 4104 4304 4104 3b04 4304   ...>.A.C.A.;.C.
+0000c3c0: 3304 3800 2004 3704 3004 3204 3504 4004  3.8. .7.0.2.5.@.
+0000c3d0: 4804 5104 3d08 0000 0000 0600 0000 1445  H.Q.=..........E
+0000c3e0: 5349 4120 6c6f 6769 6e20 636f 6d70 6c65  SIA login comple
+0000c3f0: 7465 6407 0000 0012 5265 7175 6573 7449  ted.....RequestI
+0000c400: 6e74 6572 6365 7074 6f72 0103 0000 000a  nterceptor......
+0000c410: 0410 043a 0442 0438 0432 0800 0000 0006  ...:.B.8.2......
+0000c420: 0000 0005 4173 7365 7407 0000 000c 5265  ....Asset.....Re
+0000c430: 7375 6c74 734d 6f64 656c 0103 0000 000c  sultsModel......
+0000c440: 041a 043e 043b 002d 0432 043e 0800 0000  ...>.;.-.2.>....
+0000c450: 0006 0000 0003 5174 7907 0000 000c 5265  ......Qty.....Re
+0000c460: 7375 6c74 734d 6f64 656c 0103 0000 000e  sultsModel......
+0000c470: 0414 043e 043b 044f 002c 0020 0025 0800  ...>.;.O.,. .%..
+0000c480: 0000 0006 0000 0008 5368 6172 652c 2025  ........Share, %
+0000c490: 0700 0000 0c52 6573 756c 7473 4d6f 6465  .....ResultsMode
+0000c4a0: 6c01 0300 0000 3004 1204 4b04 3104 4004  l.....0...K.1.@.
+0000c4b0: 3004 3d00 2004 3d04 3504 3a04 3e04 4004  0.=. .=.5.:.>.@.
+0000c4c0: 4004 3504 3a04 4204 3d04 4b04 3900 2004  @.5.:.B.=.K.9. .
+0000c4d0: 4104 4704 5104 4208 0000 0000 0600 0000  A.G.Q.B.........
+0000c4e0: 1849 6e76 616c 6964 2061 6363 6f75 6e74  .Invalid account
+0000c4f0: 2073 656c 6563 7465 6407 0000 0013 5365   selected.....Se
+0000c500: 6c65 6374 4163 636f 756e 7444 6961 6c6f  lectAccountDialo
+0000c510: 6701 0300 0000 2204 1d04 3804 4704 3504  g....."...8.G.5.
+0000c520: 3304 3e00 2004 3d04 3500 2004 3204 4b04  3.>. .=.5. .2.K.
+0000c530: 3104 4004 3004 3d04 3e08 0000 0000 0600  1.@.0.=.>.......
+0000c540: 0000 0c4e 6f20 7365 6c65 6374 696f 6e07  ...No selection.
+0000c550: 0000 0013 5365 6c65 6374 4163 636f 756e  ....SelectAccoun
+0000c560: 7444 6961 6c6f 6701 0300 0000 4004 1f04  tDialog.....@...
+0000c570: 3e04 3604 3004 3b04 4304 3904 4104 4204  >.6.0.;.C.9.A.B.
+0000c580: 3000 2c00 2004 3204 4b04 3104 3504 4004  0.,. .2.K.1.5.@.
+0000c590: 3804 4204 3500 2004 3404 4004 4304 3304  8.B.5. .4.@.C.3.
+0000c5a0: 3e04 3900 2004 4104 4704 5104 4208 0000  >.9. .A.G.Q.B...
+0000c5b0: 0000 0600 0000 1f50 6c65 6173 6520 7365  .......Please se
+0000c5c0: 6c65 6374 2064 6966 6665 7265 6e74 2061  lect different a
+0000c5d0: 6363 6f75 6e74 0700 0000 1353 656c 6563  ccount.....Selec
+0000c5e0: 7441 6363 6f75 6e74 4469 616c 6f67 0103  tAccountDialog..
+0000c5f0: 0000 0030 041f 043e 0436 0430 043b 0443  ...0...>.6.0.;.C
+0000c600: 0439 0441 0442 0430 0020 0432 044b 0431  .9.A.B.0. .2.K.1
+0000c610: 0435 0440 0438 0442 0435 0020 0441 0447  .5.@.8.B.5. .A.G
+0000c620: 0451 0442 0800 0000 0006 0000 0015 506c  .Q.B..........Pl
+0000c630: 6561 7365 2073 656c 6563 7420 6163 636f  ease select acco
+0000c640: 756e 7407 0000 0010 5365 6c65 6374 4163  unt.....SelectAc
+0000c650: 636f 756e 7444 6c67 0103 0000 0012 0421  countDlg.......!
+0000c660: 043e 043e 0431 0449 0435 043d 0438 0435  .>.>.1.I.5.=.8.5
+0000c670: 0800 0000 0006 0000 0009 5465 7874 4c61  ..........TextLa
+0000c680: 6265 6c07 0000 0010 5365 6c65 6374 4163  bel.....SelectAc
+0000c690: 636f 756e 7444 6c67 0103 0000 0056 0418  countDlg.....V..
+0000c6a0: 0441 043f 043e 043b 044c 0437 043e 0432  .A.?.>.;.L.7.>.2
+0000c6b0: 0430 0442 044c 0020 044d 0442 043e 0442  .0.B.L. .M.B.>.B
+0000c6c0: 0020 0436 0435 0020 0441 0447 0451 0442  . .6.5. .A.G.Q.B
+0000c6d0: 0020 0434 043b 044f 0020 0434 0430 043d  . .4.;.O. .4.0.=
+0000c6e0: 043d 043e 0439 0020 0432 0430 043b 044e  .=.>.9. .2.0.;.N
+0000c6f0: 0442 044b 0800 0000 0006 0000 0027 5573  .B.K.........'Us
+0000c700: 6520 7468 6520 7361 6d65 2061 6363 6f75  e the same accou
+0000c710: 6e74 2066 6f72 2067 6976 656e 2063 7572  nt for given cur
+0000c720: 7265 6e63 7907 0000 0010 5365 6c65 6374  rency.....Select
+0000c730: 4163 636f 756e 7444 6c67 0103 0000 0024  AccountDlg.....$
+0000c740: 0412 044b 0431 0435 0440 0438 0442 0435  ...K.1.5.@.8.B.5
+0000c750: 0020 043a 0430 0442 0435 0433 043e 0440  . .:.0.B.5.3.>.@
+0000c760: 0438 044e 0800 0000 0006 0000 0016 506c  .8.N..........Pl
+0000c770: 6561 7365 2073 656c 6563 7420 6361 7465  ease select cate
+0000c780: 676f 7279 0700 0000 1453 656c 6563 7443  gory.....SelectC
+0000c790: 6174 6567 6f72 7944 6961 6c6f 6701 0300  ategoryDialog...
+0000c7a0: 0000 2804 1204 4b04 3104 3504 4004 3804  ..(...K.1.5.@.8.
+0000c7b0: 4204 3500 2004 3a04 3e04 3d04 4204 4004  B.5. .:.>.=.B.@.
+0000c7c0: 3004 3304 3504 3d04 4204 3008 0000 0000  0.3.5.=.B.0.....
+0000c7d0: 0600 0000 1250 6c65 6173 6520 7365 6c65  .....Please sele
+0000c7e0: 6374 2070 6565 7207 0000 0010 5365 6c65  ct peer.....Sele
+0000c7f0: 6374 5065 6572 4469 616c 6f67 0103 0000  ctPeerDialog....
+0000c800: 0022 041d 0438 0447 0435 0433 043e 0020  ."...8.G.5.3.>. 
+0000c810: 043d 0435 0020 0432 044b 0431 0440 0430  .=.5. .2.K.1.@.0
+0000c820: 043d 043e 0800 0000 0006 0000 000c 4e6f  .=.>..........No
+0000c830: 2073 656c 6563 7469 6f6e 0700 0000 1553   selection.....S
+0000c840: 656c 6563 7452 6566 6572 656e 6365 4469  electReferenceDi
+0000c850: 616c 6f67 0103 0000 002e 0412 044b 0020  alog.........K. 
+0000c860: 0434 043e 043b 0436 043d 044b 0020 0441  .4.>.;.6.=.K. .A
+0000c870: 0434 0435 043b 0430 0442 044c 0020 0432  .4.5.;.0.B.L. .2
+0000c880: 044b 0431 043e 0440 0800 0000 0006 0000  .K.1.>.@........
+0000c890: 001b 596f 7520 7368 6f75 6c64 2073 656c  ..You should sel
+0000c8a0: 6563 7420 736f 6d65 7468 696e 6707 0000  ect something...
+0000c8b0: 0015 5365 6c65 6374 5265 6665 7265 6e63  ..SelectReferenc
+0000c8c0: 6544 6961 6c6f 6701 0300 0000 1c04 1204  eDialog.........
+0000c8d0: 4b04 3104 3504 4004 3804 4204 3500 2004  K.1.5.@.8.B.5. .
+0000c8e0: 3c04 3504 4204 3a04 4308 0000 0000 0600  <.5.B.:.C.......
+0000c8f0: 0000 1150 6c65 6173 6520 7365 6c65 6374  ...Please select
+0000c900: 2074 6167 0700 0000 0f53 656c 6563 7454   tag.....SelectT
+0000c910: 6167 4469 616c 6f67 0103 0000 005a 041d  agDialog.....Z..
+0000c920: 0435 0020 0443 0434 0430 043b 043e 0441  .5. .C.4.0.;.>.A
+0000c930: 044c 0020 043f 043e 043b 0443 0447 0438  .L. .?.>.;.C.G.8
+0000c940: 0442 044c 0020 043d 0430 0437 0432 0430  .B.L. .=.0.7.2.0
+0000c950: 043d 0438 0435 0020 043e 0433 0440 0430  .=.8.5. .>.3.@.0
+0000c960: 043d 0438 0437 0430 0446 0438 0438 0020  .=.8.7.0.F.8.8. 
+0000c970: 0438 0437 003a 0020 0800 0000 0006 0000  .8.7.:. ........
+0000c980: 001d 4361 6e27 7420 6765 7420 636f 6d70  ..Can't get comp
+0000c990: 616e 7920 6e61 6d65 2066 726f 6d3a 2007  any name from: .
+0000c9a0: 0000 000b 536c 6970 7354 6178 4150 4901  ....SlipsTaxAPI.
+0000c9b0: 0300 0000 4804 1d04 3504 3204 3e04 3704  ....H...5.2.>.7.
+0000c9c0: 3c04 3e04 3604 3d04 3e00 2004 3e04 3104  <.>.6.=.>. .>.1.
+0000c9d0: 3204 3d04 3e04 3204 3804 4204 4c00 2004  2.=.>.2.8.B.L. .
+0000c9e0: 4104 3504 4104 4104 3804 4e00 2c00 2004  A.5.A.A.8.N.,. .
+0000c9f0: 3e04 4204 3204 3504 4200 3a00 2008 0000  >.B.2.5.B.:. ...
+0000ca00: 0000 0600 0000 2143 616e 2774 2072 6566  ......!Can't ref
+0000ca10: 7265 7368 2073 6573 7369 6f6e 2c20 7265  resh session, re
+0000ca20: 7370 6f6e 7365 3a20 0700 0000 0b53 6c69  sponse: .....Sli
+0000ca30: 7073 5461 7841 5049 0103 0000 002e 041e  psTaxAPI........
+0000ca40: 0448 0438 0431 043a 0430 0020 043f 043e  .H.8.1.:.0. .?.>
+0000ca50: 043b 0443 0447 0435 043d 0438 044f 0020  .;.C.G.5.=.8.O. 
+0000ca60: 0447 0435 043a 0430 003a 0020 0800 0000  .G.5.:.0.:. ....
+0000ca70: 0006 0000 0013 4765 7420 7469 636b 6574  ......Get ticket
+0000ca80: 2066 6169 6c65 643a 2007 0000 000b 536c   failed: .....Sl
+0000ca90: 6970 7354 6178 4150 4901 0300 0000 3404  ipsTaxAPI.....4.
+0000caa0: 1e04 4804 3804 3104 3a04 3000 2004 3f04  ..H.8.1.:.0. .?.
+0000cab0: 3e04 3b04 4304 4704 3504 3d04 3804 4f00  >.;.C.G.5.=.8.O.
+0000cac0: 2000 6900 6400 2004 4704 3504 3a04 3000   .i.d. .G.5.:.0.
+0000cad0: 3a00 2008 0000 0000 0600 0000 1647 6574  :. ..........Get
+0000cae0: 2074 6963 6b65 7420 6964 2066 6169 6c65   ticket id faile
+0000caf0: 643a 2007 0000 000b 536c 6970 7354 6178  d: .....SlipsTax
+0000cb00: 4150 4901 0300 0000 7c04 1d04 3504 3204  API.....|...5.2.
+0000cb10: 3504 4004 3d04 3004 4f00 2004 3404 3b04  5.@.=.0.O. .4.;.
+0000cb20: 3804 3d04 3000 2004 1804 1d04 1d00 2e00  8.=.0. .........
+0000cb30: 2004 1d04 3504 3204 3e04 3704 3c04 3e04   ...5.2.>.7.<.>.
+0000cb40: 3604 3d04 3e00 2004 3f04 3e04 3b04 4304  6.=.>. .?.>.;.C.
+0000cb50: 4704 3804 4204 4c00 2004 3d04 3004 3804  G.8.B.L. .=.0.8.
+0000cb60: 3c04 3504 3d04 3e04 3204 3004 3d04 3804  <.5.=.>.2.0.=.8.
+0000cb70: 3500 2004 3a04 3e04 3c04 3f04 3004 3d04  5. .:.>.<.?.0.=.
+0000cb80: 3804 3800 2e08 0000 0000 0600 0000 3049  8.8...........0I
+0000cb90: 6e63 6f72 7265 6374 206c 656e 6774 6820  ncorrect length 
+0000cba0: 6f66 2049 4e4e 2e20 4361 6e27 7420 6765  of INN. Can't ge
+0000cbb0: 7420 636f 6d70 616e 7920 6e61 6d65 2e07  t company name..
+0000cbc0: 0000 000b 536c 6970 7354 6178 4150 4901  ....SlipsTaxAPI.
+0000cbd0: 0300 0000 5604 1d04 3504 4200 2000 5300  ....V...5.B. .S.
+0000cbe0: 6500 7300 7300 6900 6f00 6e00 4900 6400  e.s.s.i.o.n.I.d.
+0000cbf0: 2004 3404 3b04 4f00 2004 3704 3004 3304   .4.;.O. .7.0.3.
+0000cc00: 4004 4304 3704 3a04 3800 2004 4704 3504  @.C.7.:.8. .G.5.
+0000cc10: 3a04 3000 2004 4100 2004 4104 3004 3904  :.0. .A. .A.0.9.
+0000cc20: 4204 3000 2004 2404 1d04 2108 0000 0000  B.0. .$...!.....
+0000cc30: 0600 0000 224e 6f20 5275 7373 6961 6e20  ...."No Russian 
+0000cc40: 5461 7820 5365 7373 696f 6e49 6420 6176  Tax SessionId av
+0000cc50: 6169 6c61 626c 6507 0000 000b 536c 6970  ailable.....Slip
+0000cc60: 7354 6178 4150 4901 0300 0000 3604 1d04  sTaxAPI.....6...
+0000cc70: 3504 4200 2004 3004 3a04 4204 3804 3204  5.B. .0.:.B.8.2.
+0000cc80: 3d04 3e04 3900 2004 4104 3504 4104 4104  =.>.9. .A.5.A.A.
+0000cc90: 3804 3800 2004 3404 3b04 4f00 2004 2404  8.8. .4.;.O. .$.
+0000cca0: 1d04 2108 0000 0000 0600 0000 184e 6f20  ..!..........No 
+0000ccb0: 7661 6c69 6420 7365 7373 696f 6e20 7072  valid session pr
+0000ccc0: 6573 656e 7407 0000 000b 536c 6970 7354  esent.....SlipsT
+0000ccd0: 6178 4150 4901 0300 0000 7a04 1e04 3f04  axAPI.....z...?.
+0000cce0: 3504 4004 3004 4604 3804 4f00 2004 3e04  5.@.0.F.8.O. .>.
+0000ccf0: 3104 4004 3004 3104 3004 4204 4b04 3204  1.@.0.1.0.B.K.2.
+0000cd00: 3004 3504 4204 4104 4f00 2004 3d04 3000  0.5.B.A.O. .=.0.
+0000cd10: 2004 4104 4204 3e04 4004 3e04 3d04 3500   .A.B.>.@.>.=.5.
+0000cd20: 2004 4104 3504 4004 3204 3504 4004 3000   .A.5.@.2.5.@.0.
+0000cd30: 2e00 2004 1f04 3e04 3204 4204 3e04 4004  .. ...>.2.B.>.@.
+0000cd40: 4f04 4e00 2004 3504 4904 5100 2004 4004  O.N. .5.I.Q. .@.
+0000cd50: 3004 3700 2e08 0000 0000 0600 0000 384f  0.7...........8O
+0000cd60: 7065 7261 7469 6f6e 206d 6967 6874 2062  peration might b
+0000cd70: 6520 7065 6e64 696e 6720 6f6e 2073 6572  e pending on ser
+0000cd80: 7665 7220 7369 6465 2e20 5472 7969 6e67  ver side. Trying
+0000cd90: 2061 6761 696e 2e07 0000 000b 536c 6970   again......Slip
+0000cda0: 7354 6178 4150 4901 0300 0000 2804 1e04  sTaxAPI.....(...
+0000cdb0: 3104 3d04 3e04 3204 3b04 3504 3d04 3804  1.=.>.2.;.5.=.8.
+0000cdc0: 3500 2004 4104 3504 4104 4104 3804 3800  5. .A.5.A.A.8.8.
+0000cdd0: 2e00 2e00 2e08 0000 0000 0600 0000 1552  ...............R
+0000cde0: 6566 7265 7368 696e 6720 7365 7373 696f  efreshing sessio
+0000cdf0: 6e2e 2e2e 0700 0000 0b53 6c69 7073 5461  n........SlipsTa
+0000ce00: 7841 5049 0103 0000 0024 0421 0435 0441  xAPI.....$.!.5.A
+0000ce10: 0441 0438 044f 0020 043e 0431 043d 043e  .A.8.O. .>.1.=.>
+0000ce20: 0432 043b 0435 043d 0430 003a 0020 0800  .2.;.5.=.0.:. ..
+0000ce30: 0000 0006 0000 0013 5365 7373 696f 6e20  ........Session 
+0000ce40: 7265 6672 6573 6865 643a 2007 0000 000b  refreshed: .....
+0000ce50: 536c 6970 7354 6178 4150 4901 0300 0000  SlipsTaxAPI.....
+0000ce60: 1804 2704 3504 3a00 2004 3d04 3004 3904  ..'.5.:. .=.0.9.
+0000ce70: 3404 3504 3d00 3a00 2008 0000 0000 0600  4.5.=.:. .......
+0000ce80: 0000 0c53 6c69 7020 666f 756e 643a 2007  ...Slip found: .
+0000ce90: 0000 000b 536c 6970 7354 6178 4150 4901  ....SlipsTaxAPI.
+0000cea0: 0300 0000 1c04 2704 3504 3a00 2004 3704  ......'.5.:. .7.
+0000ceb0: 3004 3304 4004 4304 3604 3504 3d00 3a00  0.3.@.C.6.5.=.:.
+0000cec0: 2008 0000 0000 0600 0000 0d53 6c69 7020   ..........Slip 
+0000ced0: 6c6f 6164 6564 3a20 0700 0000 0b53 6c69  loaded: .....Sli
+0000cee0: 7073 5461 7841 5049 0103 0000 0036 041d  psTaxAPI.....6..
+0000cef0: 0435 0430 0432 0442 043e 0440 0438 0437  .5.0.2.B.>.@.8.7
+0000cf00: 043e 0432 0430 043d 043e 0020 043f 043e  .>.2.0.=.>. .?.>
+0000cf10: 0020 043f 0440 0438 0447 0438 043d 0435  . .?.@.8.G.8.=.5
+0000cf20: 003a 0020 0800 0000 0006 0000 001a 556e  .:. ..........Un
+0000cf30: 6175 7468 6f72 697a 6564 2077 6974 6820  authorized with 
+0000cf40: 7265 6173 6f6e 3a20 0700 0000 0b53 6c69  reason: .....Sli
+0000cf50: 7073 5461 7841 5049 0103 0000 001c 0421  psTaxAPI.......!
+0000cf60: 0447 0451 0442 0020 043d 0435 0020 0432  .G.Q.B. .=.5. .2
+0000cf70: 044b 0431 0440 0430 043d 0800 0000 0006  .K.1.@.0.=......
+0000cf80: 0000 0014 4163 636f 756e 7420 6e6f 7420  ....Account not 
+0000cf90: 7365 6c65 6374 6564 0700 0000 0953 7461  selected.....Sta
+0000cfa0: 7465 6d65 6e74 0103 0000 0034 0414 0430  tement.....4...0
+0000cfb0: 043d 043d 044b 0435 0020 043d 0435 0020  .=.=.K.5. .=.5. 
+0000cfc0: 043f 0440 0438 0432 044f 0437 0430 043d  .?.@.8.2.O.7.0.=
+0000cfd0: 044b 0020 043a 0020 0426 0411 003a 0020  .K. .:. .&...:. 
+0000cfe0: 0800 0000 0006 0000 0023 4173 7365 7420  .........#Asset 
+0000cff0: 6461 7461 2061 7265 6e27 7420 6c69 6e6b  data aren't link
+0000d000: 6564 2074 6f20 6173 7365 743a 2007 0000  ed to asset: ...
+0000d010: 0009 5374 6174 656d 656e 7401 0300 0000  ..Statement.....
+0000d020: 1e04 2604 1100 2000 6900 6400 2004 3d04  ..&... .i.d. .=.
+0000d030: 3500 2004 3d04 3004 3904 3404 3504 3d08  5. .=.0.9.4.5.=.
+0000d040: 0000 0000 0600 0000 1241 7373 6574 2069  .........Asset i
+0000d050: 6420 6e6f 7420 666f 756e 6407 0000 0009  d not found.....
+0000d060: 5374 6174 656d 656e 7401 0300 0000 3204  Statement.....2.
+0000d070: 1d04 3504 3204 3e04 3704 3c04 3e04 3604  ..5.2.>.7.<.>.6.
+0000d080: 3d04 3e00 2004 4104 3e04 3704 3404 3004  =.>. .A.>.7.4.0.
+0000d090: 4204 4c00 2004 4104 4704 5104 4200 3a00  B.L. .A.G.Q.B.:.
+0000d0a0: 2008 0000 0000 0600 0000 1643 616e 2774   ..........Can't
+0000d0b0: 2063 7265 6174 6520 6163 636f 756e 743a   create account:
+0000d0c0: 2007 0000 0009 5374 6174 656d 656e 7401   .....Statement.
+0000d0d0: 0300 0000 2e04 1d04 3504 3204 3e04 3704  ........5.2.>.7.
+0000d0e0: 3c04 3e04 3604 3d04 3e00 2004 4104 3e04  <.>.6.=.>. .A.>.
+0000d0f0: 3704 3404 3004 4204 4c00 2004 2604 1100  7.4.0.B.L. .&...
+0000d100: 3a00 2008 0000 0000 0600 0000 1443 616e  :. ..........Can
+0000d110: 2774 2063 7265 6174 6520 6173 7365 743a  't create asset:
+0000d120: 2007 0000 0009 5374 6174 656d 656e 7401   .....Statement.
+0000d130: 0300 0000 3c04 1d04 3504 3204 3e04 3704  ....<...5.2.>.7.
+0000d140: 3c04 3e04 3604 3d04 3e00 2004 3d04 3004  <.>.6.=.>. .=.0.
+0000d150: 3904 4204 3500 2004 2604 1100 2004 3200  9.B.5. .&... .2.
+0000d160: 2004 3e04 4204 4704 5104 4204 3500 3a00   .>.B.G.Q.B.5.:.
+0000d170: 2008 0000 0000 0600 0000 2643 616e 2774   .........&Can't
+0000d180: 206c 6f63 6174 6520 6173 7365 7420 696e   locate asset in
+0000d190: 2073 7461 7465 6d65 6e74 2064 6174 613a   statement data:
+0000d1a0: 2007 0000 0009 5374 6174 656d 656e 7401   .....Statement.
+0000d1b0: 0300 0000 1a04 1f04 3e04 3404 4204 3204  ........>.4.B.2.
+0000d1c0: 3504 4004 3604 3404 3504 3d04 3804 3508  5.@.6.4.5.=.8.5.
+0000d1d0: 0000 0000 0600 0000 0c43 6f6e 6669 726d  .........Confirm
+0000d1e0: 6174 696f 6e07 0000 0009 5374 6174 656d  ation.....Statem
+0000d1f0: 656e 7401 0300 0000 4404 1e04 4204 3b04  ent.....D...B.;.
+0000d200: 3004 3404 3e04 4704 3d04 3004 4f00 2004  0.4.>.G.=.0.O. .
+0000d210: 3804 3d04 4404 3e04 4004 3c04 3004 4604  8.=.D.>.@.<.0.F.
+0000d220: 3804 4f00 2004 4104 3e04 4504 4004 3004  8.O. .A.>.E.@.0.
+0000d230: 3d04 3504 3d04 3000 2004 3200 2008 0000  =.5.=.0. .2. ...
+0000d240: 0000 0600 0000 1e44 6562 7567 2069 6e66  .......Debug inf
+0000d250: 6f72 6d61 7469 6f6e 2069 7320 7361 7665  ormation is save
+0000d260: 6420 696e 2007 0000 0009 5374 6174 656d  d in .....Statem
+0000d270: 656e 7401 0300 0000 1004 1404 3504 3f04  ent.........5.?.
+0000d280: 3e04 3704 3804 4200 2008 0000 0000 0600  >.7.8.B. .......
+0000d290: 0000 0b44 6570 6f73 6974 206f 6620 0700  ...Deposit of ..
+0000d2a0: 0000 0953 7461 7465 6d65 6e74 0103 0000  ...Statement....
+0000d2b0: 0048 041d 0435 0432 043e 0437 043c 043e  .H...5.2.>.7.<.>
+0000d2c0: 0436 043d 043e 0020 043f 0440 043e 0447  .6.=.>. .?.@.>.G
+0000d2d0: 0438 0442 0430 0442 044c 0020 004a 0053  .8.B.0.B.L. .J.S
+0000d2e0: 004f 004e 0020 0438 0437 0020 0444 0430  .O.N. .8.7. .D.0
+0000d2f0: 0439 043b 0430 003a 0020 0800 0000 0006  .9.;.0.:. ......
+0000d300: 0000 001f 4661 696c 6564 2074 6f20 7265  ....Failed to re
+0000d310: 6164 204a 534f 4e20 6672 6f6d 2066 696c  ad JSON from fil
+0000d320: 653a 2007 0000 0009 5374 6174 656d 656e  e: .....Statemen
+0000d330: 7401 0300 0000 4804 1d04 3500 2004 4304  t.....H...5. .C.
+0000d340: 3404 3004 3b04 3e04 4104 4c00 2004 3f04  4.0.;.>.A.L. .?.
+0000d350: 4004 3e04 4704 3804 4204 3004 4204 4c00  @.>.G.8.B.0.B.L.
+0000d360: 2004 4104 4504 3504 3c04 4300 2000 4a00   .A.E.5.<.C. .J.
+0000d370: 5300 4f00 4e00 2004 3804 3700 3a00 2008  S.O.N. .8.7.:. .
+0000d380: 0000 0000 0600 0000 2146 6169 6c65 6420  ........!Failed 
+0000d390: 746f 2072 6561 6420 4a53 4f4e 2073 6368  to read JSON sch
+0000d3a0: 656d 6120 6672 6f6d 3a20 0700 0000 0953  ema from: .....S
+0000d3b0: 7461 7465 6d65 6e74 0103 0000 0034 041d  tatement.....4..
+0000d3c0: 0435 0432 043e 0437 043c 043e 0436 043d  .5.2.>.7.<.>.6.=
+0000d3d0: 043e 0020 043f 0440 043e 0447 0435 0441  .>. .?.@.>.G.5.A
+0000d3e0: 0442 044c 0020 0444 0430 0439 043b 003a  .B.L. .D.0.9.;.:
+0000d3f0: 0020 0800 0000 0006 0000 0015 4661 696c  . ..........Fail
+0000d400: 6564 2074 6f20 7265 6164 2066 696c 653a  ed to read file:
+0000d410: 2007 0000 0009 5374 6174 656d 656e 7401   .....Statement.
+0000d420: 0300 0000 5a04 1e04 4804 3804 3104 3a04  ....Z...H.8.1.:.
+0000d430: 3000 2004 3f04 4004 3800 2004 4104 3e04  0. .?.@.8. .A.>.
+0000d440: 4504 4004 3004 3d04 3504 3d04 3804 3800  E.@.0.=.5.=.8.8.
+0000d450: 2004 3e04 4204 3b04 3004 3404 3e04 4704   .>.B.;.0.4.>.G.
+0000d460: 3d04 3e04 3900 2004 3804 3d04 4404 3e04  =.>.9. .8.=.D.>.
+0000d470: 4004 3c04 3004 4604 3804 3800 3a00 2008  @.<.0.F.8.8.:. .
+0000d480: 0000 0000 0600 0000 2546 6169 6c65 6420  ........%Failed 
+0000d490: 746f 2077 7269 7465 2073 7461 7465 6d65  to write stateme
+0000d4a0: 6e74 2064 756d 7020 696e 746f 3a20 0700  nt dump into: ..
+0000d4b0: 0000 0953 7461 7465 6d65 6e74 0103 0000  ...Statement....
+0000d4c0: 0066 041d 0435 0432 043e 0437 043c 043e  .f...5.2.>.7.<.>
+0000d4d0: 0436 043d 043e 0020 043a 043e 043d 0442  .6.=.>. .:.>.=.B
+0000d4e0: 0432 0435 0440 0442 0438 0440 043e 0432  .2.5.@.B.8.@.>.2
+0000d4f0: 0430 0442 044c 0020 0442 0438 043f 0020  .0.B.L. .B.8.?. 
+0000d500: 0430 043a 0442 0438 0432 0430 0020 0432  .0.:.B.8.2.0. .2
+0000d510: 0020 0442 0440 0430 043d 0441 0444 0435  . .B.@.0.=.A.D.5
+0000d520: 0440 0435 003a 0020 0800 0000 0006 0000  .@.5.:. ........
+0000d530: 002e 496d 706f 7373 6962 6c65 2074 6f20  ..Impossible to 
+0000d540: 636f 6e76 6572 7420 6173 7365 7420 7479  convert asset ty
+0000d550: 7065 2069 6e20 7472 616e 7366 6572 3a20  pe in transfer: 
+0000d560: 0700 0000 0953 7461 7465 6d65 6e74 0103  .....Statement..
+0000d570: 0000 0048 041d 0435 043e 0434 043d 043e  ...H...5.>.4.=.>
+0000d580: 0437 043d 0430 0447 043d 043e 0435 0020  .7.=.0.G.=.>.5. 
+0000d590: 0441 043e 0432 043f 0430 0434 0435 043d  .A.>.2.?.0.4.5.=
+0000d5a0: 0438 0435 0020 0432 0430 043b 044e 0442  .8.5. .2.0.;.N.B
+0000d5b0: 044b 0020 0434 043b 044f 0020 0800 0000  .K. .4.;.O. ....
+0000d5c0: 0006 0000 001c 4d75 6c74 6970 6c65 2063  ......Multiple c
+0000d5d0: 7572 7265 6e63 7920 6d61 7463 6820 666f  urrency match fo
+0000d5e0: 7220 0700 0000 0953 7461 7465 6d65 6e74  r .....Statement
+0000d5f0: 0103 0000 003a 041d 0435 043e 0434 043d  .....:...5.>.4.=
+0000d600: 043e 0437 043d 0430 0447 043d 043e 0435  .>.7.=.0.G.=.>.5
+0000d610: 0020 0441 043e 0432 043f 0430 0434 0435  . .A.>.2.?.0.4.5
+0000d620: 043d 0438 0435 0020 0434 043b 044f 0020  .=.8.5. .4.;.O. 
+0000d630: 0800 0000 0006 0000 0013 4d75 6c74 6970  ..........Multip
+0000d640: 6c65 206d 6174 6368 2066 6f72 2007 0000  le match for ...
+0000d650: 0009 5374 6174 656d 656e 7401 0300 0000  ..Statement.....
+0000d660: 3a04 1204 4b04 3104 3504 4004 3804 4204  :...K.1.5.@.8.B.
+0000d670: 3500 2004 4104 4704 5104 4200 2004 3404  5. .A.G.Q.B. .4.
+0000d680: 3b04 4f00 2004 3704 3004 4704 3804 4104  ;.O. .7.0.G.8.A.
+0000d690: 3b04 3504 3d04 3804 4f00 3a08 0000 0000  ;.5.=.8.O.:.....
+0000d6a0: 0600 0000 1d53 656c 6563 7420 6163 636f  .....Select acco
+0000d6b0: 756e 7420 746f 2064 6570 6f73 6974 2074  unt to deposit t
+0000d6c0: 6f3a 0700 0000 0953 7461 7465 6d65 6e74  o:.....Statement
+0000d6d0: 0103 0000 0036 0412 044b 0431 0435 0440  .....6...K.1.5.@
+0000d6e0: 0438 0442 0435 0020 0441 0447 0451 0442  .8.B.5. .A.G.Q.B
+0000d6f0: 0020 0434 043b 044f 0020 0441 043f 0438  . .4.;.O. .A.?.8
+0000d700: 0441 0430 043d 0438 044f 003a 0800 0000  .A.0.=.8.O.:....
+0000d710: 0006 0000 0020 5365 6c65 6374 2061 6363  ..... Select acc
+0000d720: 6f75 6e74 2074 6f20 7769 7468 6472 6177  ount to withdraw
+0000d730: 2066 726f 6d3a 0700 0000 0953 7461 7465   from:.....State
+0000d740: 6d65 6e74 0103 0000 0048 041d 0435 043a  ment.....H...5.:
+0000d750: 043e 0442 043e 0440 044b 0435 0020 0441  .>.B.>.@.K.5. .A
+0000d760: 0435 043a 0446 0438 0438 0020 043d 0435  .5.:.F.8.8. .=.5
+0000d770: 0020 043f 043e 0434 0434 0435 0440 0436  . .?.>.4.4.5.@.6
+0000d780: 0438 0432 0430 044e 0442 0441 044f 003a  .8.2.0.N.B.A.O.:
+0000d790: 0020 0800 0000 0006 0000 0021 536f 6d65  . .........!Some
+0000d7a0: 2073 6563 7469 6f6e 7320 6172 6520 6e6f   sections are no
+0000d7b0: 7420 7375 7070 6f72 7465 643a 2007 0000  t supported: ...
+0000d7c0: 0009 5374 6174 656d 656e 7401 0300 0000  ..Statement.....
+0000d7d0: 2a04 1804 3c04 3f04 3e04 4004 4200 2004  *...<.?.>.@.B. .
+0000d7e0: 3e04 4204 4704 5104 4204 3000 2004 3f04  >.B.G.Q.B.0. .?.
+0000d7f0: 4004 3504 4004 3204 3004 3d08 0000 0000  @.5.@.2.0.=.....
+0000d800: 0600 0000 1e53 7461 7465 6d65 6e74 2069  .....Statement i
+0000d810: 6d70 6f72 7420 7761 7320 6361 6e63 656c  mport was cancel
+0000d820: 6c65 6407 0000 0009 5374 6174 656d 656e  led.....Statemen
+0000d830: 7401 0300 0000 2c04 1d04 3504 3204 3504  t.....,...5.2.5.
+0000d840: 4004 3d04 4b04 3900 2004 3f04 3504 4004  @.=.K.9. .?.5.@.
+0000d850: 3804 3e04 3400 2004 3e04 4204 4704 5104  8.>.4. .>.B.G.Q.
+0000d860: 4204 3008 0000 0000 0600 0000 1b53 7461  B.0..........Sta
+0000d870: 7465 6d65 6e74 2070 6572 696f 6420 6973  tement period is
+0000d880: 2069 6e76 616c 6964 0700 0000 0953 7461   invalid.....Sta
+0000d890: 7465 6d65 6e74 0103 0000 00c6 041f 0435  tement.........5
+0000d8a0: 0440 0438 043e 0434 0020 043e 0442 0447  .@.8.>.4. .>.B.G
+0000d8b0: 0451 0442 0430 0020 043d 0430 0447 0438  .Q.B.0. .=.0.G.8
+0000d8c0: 043d 0430 0435 0442 0441 044f 0020 0440  .=.0.5.B.A.O. .@
+0000d8d0: 0430 043d 0435 0435 0020 043f 043e 0441  .0.=.5.5. .?.>.A
+0000d8e0: 043b 0435 0434 043d 0435 0439 0020 043e  .;.5.4.=.5.9. .>
+0000d8f0: 043f 0435 0440 0430 0446 0438 0438 0020  .?.5.@.0.F.8.8. 
+0000d900: 0434 043b 044f 0020 0441 0447 0451 0442  .4.;.O. .A.G.Q.B
+0000d910: 0430 0020 0028 043f 043e 0432 0442 043e  .0. .(.?.>.2.B.>
+0000d920: 0440 043d 044b 0439 0020 0438 043c 043f  .@.=.K.9. .8.<.?
+0000d930: 043e 0440 0442 003f 0029 002e 0020 041f  .>.@.B.?.)... ..
+0000d940: 0440 043e 0434 043e 043b 0436 0438 0442  .@.>.4.>.;.6.8.B
+0000d950: 044c 0020 0438 043c 043f 043e 0440 0442  .L. .8.<.?.>.@.B
+0000d960: 003f 0800 0000 0006 0000 0058 5374 6174  .?.........XStat
+0000d970: 656d 656e 7420 7065 7269 6f64 2073 7461  ement period sta
+0000d980: 7274 7320 6265 666f 7265 206c 6173 7420  rts before last 
+0000d990: 7265 636f 7264 6564 206f 7065 7261 7469  recorded operati
+0000d9a0: 6f6e 2066 6f72 2074 6865 2061 6363 6f75  on for the accou
+0000d9b0: 6e74 2e20 436f 6e74 696e 7565 2069 6d70  nt. Continue imp
+0000d9c0: 6f72 743f 0700 0000 0953 7461 7465 6d65  ort?.....Stateme
+0000d9d0: 6e74 0103 0000 002a 041e 0442 0447 0451  nt.....*...B.G.Q
+0000d9e0: 0442 0020 0441 043e 0434 0435 0440 0436  .B. .A.>.4.5.@.6
+0000d9f0: 0438 0442 0020 043e 0448 0438 0431 043a  .8.B. .>.H.8.1.:
+0000da00: 0438 0800 0000 0006 0000 001b 5374 6174  .8..........Stat
+0000da10: 656d 656e 7420 7661 6c69 6461 7469 6f6e  ement validation
+0000da20: 2066 6169 6c65 6407 0000 0009 5374 6174   failed.....Stat
+0000da30: 656d 656e 7401 0300 0000 4004 2104 3804  ement.....@.!.8.
+0000da40: 3c04 3204 3e04 3b00 2004 3204 3004 3b04  <.2.>.;. .2.0.;.
+0000da50: 4e04 4204 4b00 2004 3d04 3500 2004 3f04  N.B.K. .=.5. .?.
+0000da60: 4004 3804 3204 4f04 3704 3004 3d00 2004  @.8.2.O.7.0.=. .
+0000da70: 3a00 2004 2604 1100 3a00 2008 0000 0000  :. .&...:. .....
+0000da80: 0600 0000 2753 796d 626f 6c20 6375 7272  ....'Symbol curr
+0000da90: 656e 6379 2069 736e 2774 206c 696e 6b65  ency isn't linke
+0000daa0: 6420 746f 2061 7373 6574 3a20 0700 0000  d to asset: ....
+0000dab0: 0953 7461 7465 6d65 6e74 0103 0000 0032  .Statement.....2
+0000dac0: 0421 0438 043c 0432 043e 043b 0020 043d  .!.8.<.2.>.;. .=
+0000dad0: 0435 0020 043f 0440 0438 0432 044f 0437  .5. .?.@.8.2.O.7
+0000dae0: 0430 043d 0020 043a 0020 0426 0411 003a  .0.=. .:. .&...:
+0000daf0: 0020 0800 0000 0006 0000 0025 5379 6d62  . .........%Symb
+0000db00: 6f6c 2074 6963 6b65 7220 6973 6e27 7420  ol ticker isn't 
+0000db10: 6c69 6e6b 6564 2074 6f20 6173 7365 743a  linked to asset:
+0000db20: 2007 0000 0009 5374 6174 656d 656e 7401   .....Statement.
+0000db30: 0300 0000 7204 1d04 3504 3204 3e04 3704  ....r...5.2.>.7.
+0000db40: 3c04 3e04 3604 3d04 3e00 2004 4104 3e04  <.>.6.=.>. .A.>.
+0000db50: 3f04 3e04 4104 4204 3004 3204 3804 4204  ?.>.A.B.0.2.8.B.
+0000db60: 4c00 2004 4104 4704 5104 4200 2004 3404  L. .A.G.Q.B. .4.
+0000db70: 3b04 4f00 2004 3a04 3e04 4004 3f04 3e04  ;.O. .:.>.@.?.>.
+0000db80: 4004 3004 4204 3804 3204 3d04 3e04 3304  @.0.B.8.2.=.>.3.
+0000db90: 3e00 2004 3404 3504 3904 4104 4204 3204  >. .4.5.9.A.B.2.
+0000dba0: 3804 4f00 3a00 2008 0000 0000 0600 0000  8.O.:. .........
+0000dbb0: 2855 6e6d 6174 6368 6564 2061 6363 6f75  (Unmatched accou
+0000dbc0: 6e74 2066 6f72 2063 6f72 706f 7261 7465  nt for corporate
+0000dbd0: 2061 6374 696f 6e3a 2007 0000 0009 5374   action: .....St
+0000dbe0: 6174 656d 656e 7401 0300 0000 7404 1d04  atement.....t...
+0000dbf0: 3504 3204 3e04 3704 3c04 3e04 3604 3d04  5.2.>.7.<.>.6.=.
+0000dc00: 3e00 2004 4104 3e04 3f04 3e04 4104 4204  >. .A.>.?.>.A.B.
+0000dc10: 3004 3204 3804 4204 4c00 2004 4104 4704  0.2.8.B.L. .A.G.
+0000dc20: 5104 4200 2004 3404 3b04 4f00 2004 3e04  Q.B. .4.;.O. .>.
+0000dc30: 3f04 3504 4004 3004 4604 3804 3800 2004  ?.5.@.0.F.8.8. .
+0000dc40: 3f04 4004 3804 4504 3e04 3404 3000 2f04  ?.@.8.E.>.4.0./.
+0000dc50: 4004 3004 4104 4504 3e04 3404 3000 3a00  @.0.A.E.>.4.0.:.
+0000dc60: 2008 0000 0000 0600 0000 2755 6e6d 6174   .........'Unmat
+0000dc70: 6368 6564 2061 6363 6f75 6e74 2066 6f72  ched account for
+0000dc80: 2069 6e63 6f6d 652f 7370 656e 6469 6e67   income/spending
+0000dc90: 3a20 0700 0000 0953 7461 7465 6d65 6e74  : .....Statement
+0000dca0: 0103 0000 0052 041d 0435 0432 043e 0437  .....R...5.2.>.7
+0000dcb0: 043c 043e 0436 043d 043e 0020 0441 043e  .<.>.6.=.>. .A.>
+0000dcc0: 043f 043e 0441 0442 0430 0432 0438 0442  .?.>.A.B.0.2.8.B
+0000dcd0: 044c 0020 0441 0447 0451 0442 0020 0434  .L. .A.G.Q.B. .4
+0000dce0: 043b 044f 0020 0432 044b 043f 043b 0430  .;.O. .2.K.?.;.0
+0000dcf0: 0442 044b 003a 0020 0800 0000 0006 0000  .B.K.:. ........
+0000dd00: 001f 556e 6d61 7463 6865 6420 6163 636f  ..Unmatched acco
+0000dd10: 756e 7420 666f 7220 7061 796d 656e 743a  unt for payment:
+0000dd20: 2007 0000 0009 5374 6174 656d 656e 7401   .....Statement.
+0000dd30: 0300 0000 5004 1d04 3504 3204 3e04 3704  ....P...5.2.>.7.
+0000dd40: 3c04 3e04 3604 3d04 3e00 2004 4104 3e04  <.>.6.=.>. .A.>.
+0000dd50: 3f04 3e04 4104 4204 3004 3204 3804 4204  ?.>.A.B.0.2.8.B.
+0000dd60: 4c00 2004 4104 4704 5104 4200 2004 3404  L. .A.G.Q.B. .4.
+0000dd70: 3b04 4f00 2004 4104 3404 3504 3b04 3a04  ;.O. .A.4.5.;.:.
+0000dd80: 3800 3a00 2008 0000 0000 0600 0000 1d55  8.:. ..........U
+0000dd90: 6e6d 6174 6368 6564 2061 6363 6f75 6e74  nmatched account
+0000dda0: 2066 6f72 2074 7261 6465 3a20 0700 0000   for trade: ....
+0000ddb0: 0953 7461 7465 6d65 6e74 0103 0000 0054  .Statement.....T
+0000ddc0: 041d 0435 0432 0437 043e 043c 043e 0436  ...5.2.7.>.<.>.6
+0000ddd0: 043d 043e 0020 0441 043e 043f 043e 0441  .=.>. .A.>.?.>.A
+0000dde0: 0442 0430 0432 0438 0442 044c 0020 0441  .B.0.2.8.B.L. .A
+0000ddf0: 0447 0451 0442 0020 0434 043b 044f 0020  .G.Q.B. .4.;.O. 
+0000de00: 043f 0435 0440 0435 0432 043e 0434 0430  .?.5.@.5.2.>.4.0
+0000de10: 003a 0020 0800 0000 0006 0000 0020 556e  .:. ......... Un
+0000de20: 6d61 7463 6865 6420 6163 636f 756e 7420  matched account 
+0000de30: 666f 7220 7472 616e 7366 6572 3a20 0700  for transfer: ..
+0000de40: 0000 0953 7461 7465 6d65 6e74 0103 0000  ...Statement....
+0000de50: 006e 041d 0435 0432 043e 0437 043c 043e  .n...5.2.>.7.<.>
+0000de60: 0436 043d 043e 0020 0441 043e 043f 043e  .6.=.>. .A.>.?.>
+0000de70: 0441 0442 0430 0432 0438 0442 044c 0020  .A.B.0.2.8.B.L. 
+0000de80: 0426 0411 0020 0434 043b 044f 0020 043a  .&... .4.;.O. .:
+0000de90: 043e 0440 043f 043e 0440 0430 0442 0438  .>.@.?.>.@.0.B.8
+0000dea0: 0432 043d 043e 0433 043e 0020 0434 0435  .2.=.>.3.>. .4.5
+0000deb0: 0439 0441 0442 0432 0438 044f 003a 0020  .9.A.B.2.8.O.:. 
+0000dec0: 0800 0000 0006 0000 0026 556e 6d61 7463  .........&Unmatc
+0000ded0: 6865 6420 6173 7365 7420 666f 7220 636f  hed asset for co
+0000dee0: 7270 6f72 6174 6520 6163 7469 6f6e 3a20  rporate action: 
+0000def0: 0700 0000 0953 7461 7465 6d65 6e74 0103  .....Statement..
+0000df00: 0000 004e 041d 0435 0432 043e 0437 043c  ...N...5.2.>.7.<
+0000df10: 043e 0436 043d 043e 0020 0441 043e 043f  .>.6.=.>. .A.>.?
+0000df20: 043e 0441 0442 0430 0432 0438 0442 044c  .>.A.B.0.2.8.B.L
+0000df30: 0020 0426 0411 0020 0434 043b 044f 0020  . .&... .4.;.O. 
+0000df40: 0432 044b 043f 043b 0430 0442 044b 003a  .2.K.?.;.0.B.K.:
+0000df50: 0020 0800 0000 0006 0000 001d 556e 6d61  . ..........Unma
+0000df60: 7463 6865 6420 6173 7365 7420 666f 7220  tched asset for 
+0000df70: 7061 796d 656e 743a 2007 0000 0009 5374  payment: .....St
+0000df80: 6174 656d 656e 7401 0300 0000 4c04 1d04  atement.....L...
+0000df90: 3504 3204 3e04 3704 3c04 3e04 3604 3d04  5.2.>.7.<.>.6.=.
+0000dfa0: 3e00 2004 4104 3e04 3f04 3e04 4104 4204  >. .A.>.?.>.A.B.
+0000dfb0: 3004 3204 3804 4204 4c00 2004 2604 1100  0.2.8.B.L. .&...
+0000dfc0: 2004 3404 3b04 4f00 2004 4104 3404 3504   .4.;.O. .A.4.5.
+0000dfd0: 3b04 3a04 3800 3a00 2008 0000 0000 0600  ;.:.8.:. .......
+0000dfe0: 0000 1b55 6e6d 6174 6368 6564 2061 7373  ...Unmatched ass
+0000dff0: 6574 2066 6f72 2074 7261 6465 3a20 0700  et for trade: ..
+0000e000: 0000 0953 7461 7465 6d65 6e74 0103 0000  ...Statement....
+0000e010: 005e 041d 0435 0432 043e 0437 043c 043e  .^...5.2.>.7.<.>
+0000e020: 0436 043d 043e 0020 0441 043e 043f 043e  .6.=.>. .A.>.?.>
+0000e030: 0441 0442 0430 0432 0438 0442 044c 0020  .A.B.0.2.8.B.L. 
+0000e040: 0426 0411 002f 0432 0430 043b 044e 0442  .&.../.2.0.;.N.B
+0000e050: 0443 0020 0434 043b 044f 0020 043f 0435  .C. .4.;.O. .?.5
+0000e060: 0440 0435 0432 043e 0434 0430 003a 0020  .@.5.2.>.4.0.:. 
+0000e070: 0800 0000 0006 0000 001e 556e 6d61 7463  ..........Unmatc
+0000e080: 6865 6420 6173 7365 7420 666f 7220 7472  hed asset for tr
+0000e090: 616e 7366 6572 3a20 0700 0000 0953 7461  ansfer: .....Sta
+0000e0a0: 7465 6d65 6e74 0103 0000 006c 041d 0435  tement.....l...5
+0000e0b0: 0432 043e 0437 043c 043e 0436 043d 043e  .2.>.7.<.>.6.=.>
+0000e0c0: 0020 0441 043e 043f 043e 0441 0442 0430  . .A.>.?.>.A.B.0
+0000e0d0: 0432 0438 0442 044c 0020 043a 0430 0442  .2.8.B.L. .:.0.B
+0000e0e0: 0435 0433 043e 0440 0438 044e 0020 0434  .5.3.>.@.8.N. .4
+0000e0f0: 043b 044f 0020 043f 0440 0438 0445 043e  .;.O. .?.@.8.E.>
+0000e100: 0434 0430 002f 0440 0430 0441 0445 043e  .4.0./.@.0.A.E.>
+0000e110: 0434 0430 003a 0020 0800 0000 0006 0000  .4.0.:. ........
+0000e120: 0028 556e 6d61 7463 6865 6420 6361 7465  .(Unmatched cate
+0000e130: 676f 7279 2066 6f72 2069 6e63 6f6d 652f  gory for income/
+0000e140: 7370 656e 6469 6e67 3a20 0700 0000 0953  spending: .....S
+0000e150: 7461 7465 6d65 6e74 0103 0000 0050 041d  tatement.....P..
+0000e160: 0435 0432 043e 0437 043c 043e 043d 043e  .5.2.>.7.<.>.=.>
+0000e170: 0020 0441 043e 043f 043e 0441 0442 0430  . .A.>.?.>.A.B.0
+0000e180: 0432 0438 0442 044c 0020 0432 0430 043b  .2.8.B.L. .2.0.;
+0000e190: 044e 0442 0443 0020 0434 043b 044f 0020  .N.B.C. .4.;.O. 
+0000e1a0: 0441 0447 0451 0442 0430 003a 0020 0800  .A.G.Q.B.0.:. ..
+0000e1b0: 0000 0006 0000 0020 556e 6d61 7463 6865  ....... Unmatche
+0000e1c0: 6420 6375 7272 656e 6379 2066 6f72 2061  d currency for a
+0000e1d0: 6363 6f75 6e74 3a20 0700 0000 0953 7461  ccount: .....Sta
+0000e1e0: 7465 6d65 6e74 0103 0000 0082 041d 0435  tement.........5
+0000e1f0: 0432 043e 0437 043c 043e 0436 043d 043e  .2.>.7.<.>.6.=.>
+0000e200: 0020 0441 043e 043f 043e 0441 0442 0430  . .A.>.?.>.A.B.0
+0000e210: 0432 0438 0442 044c 0020 043a 043e 043d  .2.8.B.L. .:.>.=
+0000e220: 0442 0440 0430 0433 0435 043d 0442 0430  .B.@.0.3.5.=.B.0
+0000e230: 0020 0434 043b 044f 0020 043e 043f 0435  . .4.;.O. .>.?.5
+0000e240: 0440 0430 0446 0438 0438 0020 043f 0440  .@.0.F.8.8. .?.@
+0000e250: 0438 0445 043e 0434 0430 002f 0440 0430  .8.E.>.4.0./.@.0
+0000e260: 0441 0445 043e 0434 0430 003a 0020 0800  .A.E.>.4.0.:. ..
+0000e270: 0000 0006 0000 0024 556e 6d61 7463 6865  .......$Unmatche
+0000e280: 6420 7065 6572 2066 6f72 2069 6e63 6f6d  d peer for incom
+0000e290: 652f 7370 656e 6469 6e67 3a20 0700 0000  e/spending: ....
+0000e2a0: 0953 7461 7465 6d65 6e74 0103 0000 0052  .Statement.....R
+0000e2b0: 041d 0435 043f 043e 0434 0434 0435 0440  ...5.?.>.4.4.5.@
+0000e2c0: 0436 0438 0432 0430 0435 043c 043e 0435  .6.8.2.0.5.<.>.5
+0000e2d0: 0020 043a 043e 0440 043f 043e 0440 0430  . .:.>.@.?.>.@.0
+0000e2e0: 0442 0438 0432 043d 043e 0435 0020 0434  .B.8.2.=.>.5. .4
+0000e2f0: 0435 0439 0441 0442 0432 0438 0435 003a  .5.9.A.B.2.8.5.:
+0000e300: 0020 0800 0000 0006 0000 001e 556e 7375  . ..........Unsu
+0000e310: 7070 6f72 7465 6420 636f 7270 6f72 6174  pported corporat
+0000e320: 6520 6163 7469 6f6e 3a20 0700 0000 0953  e action: .....S
+0000e330: 7461 7465 6d65 6e74 0103 0000 003c 041d  tatement.....<..
+0000e340: 0435 043f 043e 0434 0434 0435 0440 0436  .5.?.>.4.4.5.@.6
+0000e350: 0438 0432 0430 0435 043c 044b 0439 0020  .8.2.0.5.<.K.9. 
+0000e360: 0442 0438 043f 0020 0432 044b 043f 043b  .B.8.?. .2.K.?.;
+0000e370: 0430 0442 044b 003a 0020 0800 0000 0006  .0.B.K.:. ......
+0000e380: 0000 001a 556e 7375 7070 6f72 7465 6420  ....Unsupported 
+0000e390: 7061 796d 656e 7420 7479 7065 3a20 0700  payment type: ..
+0000e3a0: 0000 0953 7461 7465 6d65 6e74 0103 0000  ...Statement....
+0000e3b0: 0012 0421 043f 0438 0441 0430 043d 0438  ...!.?.8.A.0.=.8
+0000e3c0: 0435 0020 0800 0000 0006 0000 000e 5769  .5. ..........Wi
+0000e3d0: 7468 6472 6177 616c 206f 6620 0700 0000  thdrawal of ....
+0000e3e0: 0953 7461 7465 6d65 6e74 0103 0000 0044  .Statement.....D
+0000e3f0: 002a 002a 002a 0020 041d 0415 041e 0411  .*.*.*. ........
+0000e400: 0425 041e 0414 0418 041c 0410 0020 0420  .%........... . 
+0000e410: 0423 0427 041d 0410 042f 0020 041f 0420  .#.'...../. ... 
+0000e420: 041e 0412 0415 0420 041a 0410 0020 002a  ....... ..... .*
+0000e430: 002a 002a 0800 0000 0006 0000 001d 2a2a  .*.*..........**
+0000e440: 2a20 4d41 4e55 414c 2045 4e54 5259 2052  * MANUAL ENTRY R
+0000e450: 4551 5549 5245 4420 2a2a 2a07 0000 000d  EQUIRED ***.....
+0000e460: 5374 6174 656d 656e 7449 424b 5201 0300  StatementIBKR...
+0000e470: 0000 3404 2204 3804 3f00 2004 2604 1100  ..4.".8.?. .&...
+0000e480: 2004 3d04 3500 2004 3f04 3e04 3404 3404   .=.5. .?.>.4.4.
+0000e490: 3504 4004 3604 3804 3204 3004 3504 4204  5.@.6.8.2.0.5.B.
+0000e4a0: 4104 4f00 3a00 2008 0000 0000 0600 0000  A.O.:. .........
+0000e4b0: 1c41 7373 6574 2074 7970 6520 6973 6e27  .Asset type isn'
+0000e4c0: 7420 7375 7070 6f72 7465 643a 2007 0000  t supported: ...
+0000e4d0: 000d 5374 6174 656d 656e 7449 424b 5201  ..StatementIBKR.
+0000e4e0: 0300 0000 4804 1d04 3504 3204 3e04 3704  ....H...5.2.>.7.
+0000e4f0: 3c04 3e04 3604 3d04 3e00 2004 3d04 3004  <.>.6.=.>. .=.0.
+0000e500: 3904 4204 3800 2004 3f04 3b04 3004 4204  9.B.8. .?.;.0.B.
+0000e510: 5104 3600 2004 3404 3b04 4f00 2004 3e04  Q.6. .4.;.O. .>.
+0000e520: 4204 3c04 3504 3d04 4b00 3a00 2008 0000  B.<.5.=.K.:. ...
+0000e530: 0000 0600 0000 1f43 616e 2774 2066 696e  .......Can't fin
+0000e540: 6420 6d61 7463 6820 666f 7220 7265 7665  d match for reve
+0000e550: 7273 616c 3a20 0700 0000 0d53 7461 7465  rsal: .....State
+0000e560: 6d65 6e74 4942 4b52 0103 0000 0046 041d  mentIBKR.....F..
+0000e570: 0435 0432 043e 0437 043c 043e 0436 043d  .5.2.>.7.<.>.6.=
+0000e580: 043e 0020 043d 0430 0439 0442 0438 0020  .>. .=.0.9.B.8. 
+0000e590: 043f 0430 0440 043d 0443 044e 0020 0437  .?.0.@.=.C.N. .7
+0000e5a0: 0430 043f 0438 0441 044c 0020 0434 043b  .0.?.8.A.L. .4.;
+0000e5b0: 044f 0020 0800 0000 0006 0000 001d 4361  .O. ..........Ca
+0000e5c0: 6e27 7420 6669 6e64 2070 6169 7265 6420  n't find paired 
+0000e5d0: 7265 636f 7264 2066 6f72 2007 0000 000d  record for .....
+0000e5e0: 5374 6174 656d 656e 7449 424b 5201 0300  StatementIBKR...
+0000e5f0: 0000 4e04 1d04 3504 3204 3e04 3c04 3e04  ..N...5.2.>.<.>.
+0000e600: 3604 3d04 3e00 2004 3e04 3f04 4004 3504  6.=.>. .>.?.@.5.
+0000e610: 3404 3504 3b04 3804 4204 4c00 2004 3204  4.5.;.8.B.L. .2.
+0000e620: 3004 3b04 4e04 4204 4300 2004 3404 3b04  0.;.N.B.C. .4.;.
+0000e630: 4f00 2004 4104 4704 5104 4204 3000 3a00  O. .A.G.Q.B.0.:.
+0000e640: 2008 0000 0000 0600 0000 2843 616e 2774   .........(Can't
+0000e650: 2067 6574 2061 6363 6f75 6e74 2063 7572   get account cur
+0000e660: 7265 6e63 7920 666f 7220 6163 636f 756e  rency for accoun
+0000e670: 743a 2007 0000 000d 5374 6174 656d 656e  t: .....Statemen
+0000e680: 7449 424b 5201 0300 0000 7004 1d04 3504  tIBKR.....p...5.
+0000e690: 3204 3e04 3704 3c04 3e04 3604 3d04 3e00  2.>.7.<.>.6.=.>.
+0000e6a0: 2004 3e04 3f04 4004 3504 3404 3504 3b04   .>.?.@.5.4.5.;.
+0000e6b0: 3804 4204 4c00 2004 3204 3004 3b04 4e04  8.B.L. .2.0.;.N.
+0000e6c0: 4204 4b00 2004 3404 3b04 4f00 2004 3e04  B.K. .4.;.O. .>.
+0000e6d0: 3f04 3504 4004 3004 4604 3804 3800 2004  ?.5.@.0.F.8.8. .
+0000e6e0: 3e04 3104 3c04 3504 3d04 3000 2004 3204  >.1.<.5.=.0. .2.
+0000e6f0: 3004 3b04 4e04 4200 3a00 2008 0000 0000  0.;.N.B.:. .....
+0000e700: 0600 0000 2c43 616e 2774 2067 6574 2063  ....,Can't get c
+0000e710: 7572 7265 6e63 6965 7320 666f 7220 6375  urrencies for cu
+0000e720: 7272 656e 6379 2065 7863 6861 6e67 653a  rrency exchange:
+0000e730: 2007 0000 000d 5374 6174 656d 656e 7449   .....StatementI
+0000e740: 424b 5201 0300 0000 6804 1d04 3504 3204  BKR.....h...5.2.
+0000e750: 3e04 3704 3c04 3e04 3604 3d04 3e00 2004  >.7.<.>.6.=.>. .
+0000e760: 4004 3004 4104 3f04 3e04 3704 3d04 3004  @.0.A.?.>.7.=.0.
+0000e770: 4204 4c00 2004 3e04 3f04 3804 4104 3004  B.L. .>.?.8.A.0.
+0000e780: 3d04 3804 3500 2004 1e04 3104 4a04 3504  =.8.5. ...1.J.5.
+0000e790: 3404 3804 3d04 3504 3d04 3804 4f00 2004  4.8.=.5.=.8.O. .
+0000e7a0: 3a04 3e04 3c04 3f04 3004 3d04 3804 3900  :.>.<.?.0.=.8.9.
+0000e7b0: 2008 0000 0000 0600 0000 1f43 616e 2774   ..........Can't
+0000e7c0: 2070 6172 7365 204d 6572 6765 7220 6465   parse Merger de
+0000e7d0: 7363 7269 7074 696f 6e20 0700 0000 0d53  scription .....S
+0000e7e0: 7461 7465 6d65 6e74 4942 4b52 0103 0000  tatementIBKR....
+0000e7f0: 0064 041d 0435 0432 043e 0437 043c 043e  .d...5.2.>.7.<.>
+0000e800: 0436 043d 043e 0020 0440 0430 0441 043f  .6.=.>. .@.0.A.?
+0000e810: 043e 0437 043d 0430 0442 044c 0020 043e  .>.7.=.0.B.L. .>
+0000e820: 043f 0438 0441 0430 043d 0438 0435 0020  .?.8.A.0.=.8.5. 
+0000e830: 0412 044b 0434 0435 043b 0435 043d 0438  ...K.4.5.;.5.=.8
+0000e840: 044f 0020 043a 043e 043c 043f 0430 043d  .O. .:.>.<.?.0.=
+0000e850: 0438 0438 0020 0800 0000 0006 0000 0021  .8.8. .........!
+0000e860: 4361 6e27 7420 7061 7273 6520 5370 696e  Can't parse Spin
+0000e870: 2d6f 6666 2064 6573 6372 6970 7469 6f6e  -off description
+0000e880: 2007 0000 000d 5374 6174 656d 656e 7449   .....StatementI
+0000e890: 424b 5201 0300 0000 4c04 1d04 3504 3204  BKR.....L...5.2.
+0000e8a0: 3e04 3704 3c04 3e04 3604 3d04 3e00 2004  >.7.<.>.6.=.>. .
+0000e8b0: 4004 3004 4104 3f04 3e04 3704 3d04 3004  @.0.A.?.>.7.=.0.
+0000e8c0: 4204 4c00 2004 3e04 3f04 3804 4104 3004  B.L. .>.?.8.A.0.
+0000e8d0: 3d04 3804 3500 2004 2104 3f04 3b04 3804  =.8.5. .!.?.;.8.
+0000e8e0: 4204 3000 2008 0000 0000 0600 0000 1e43  B.0. ..........C
+0000e8f0: 616e 2774 2070 6172 7365 2053 706c 6974  an't parse Split
+0000e900: 2064 6573 6372 6970 7469 6f6e 2007 0000   description ...
+0000e910: 000d 5374 6174 656d 656e 7449 424b 5201  ..StatementIBKR.
+0000e920: 0300 0000 6204 1d04 3504 3204 3e04 3704  ....b...5.2.>.7.
+0000e930: 3c04 3e04 3604 3d04 3e00 2004 4004 3004  <.>.6.=.>. .@.0.
+0000e940: 4104 3f04 3e04 3704 3d04 3004 4204 4c00  A.?.>.7.=.0.B.L.
+0000e950: 2004 3e04 3f04 3804 4104 3004 3d04 3804   .>.?.8.A.0.=.8.
+0000e960: 3500 2004 1404 3804 3204 3804 3404 3504  5. ...8.2.8.4.5.
+0000e970: 3d04 3404 3000 2004 3004 3a04 4604 3804  =.4.0. .0.:.F.8.
+0000e980: 4f04 3c04 3800 2008 0000 0000 0600 0000  O.<.8. .........
+0000e990: 2743 616e 2774 2070 6172 7365 2053 746f  'Can't parse Sto
+0000e9a0: 636b 2044 6976 6964 656e 6420 6465 7363  ck Dividend desc
+0000e9b0: 7269 7074 696f 6e20 0700 0000 0d53 7461  ription .....Sta
+0000e9c0: 7465 6d65 6e74 4942 4b52 0103 0000 005a  tementIBKR.....Z
+0000e9d0: 041d 0435 0432 043e 0437 043c 043e 0436  ...5.2.>.7.<.>.6
+0000e9e0: 043d 043e 0020 0440 0430 0441 043f 043e  .=.>. .@.0.A.?.>
+0000e9f0: 0437 043d 0430 0442 044c 0020 043e 043f  .7.=.0.B.L. .>.?
+0000ea00: 0438 0441 0430 043d 0438 0435 0020 0421  .8.A.0.=.8.5. .!
+0000ea10: 043c 0435 043d 044b 0020 0441 0438 043c  .<.5.=.K. .A.8.<
+0000ea20: 0432 043e 043b 0430 0020 0800 0000 0006  .2.>.;.0. ......
+0000ea30: 0000 0026 4361 6e27 7420 7061 7273 6520  ...&Can't parse 
+0000ea40: 5379 6d62 6f6c 2043 6861 6e67 6520 6465  Symbol Change de
+0000ea50: 7363 7269 7074 696f 6e20 0700 0000 0d53  scription .....S
+0000ea60: 7461 7465 6d65 6e74 4942 4b52 0103 0000  tatementIBKR....
+0000ea70: 006e 041d 0435 0432 043e 0437 043c 043e  .n...5.2.>.7.<.>
+0000ea80: 0436 043d 043e 0020 043e 0431 0440 0430  .6.=.>. .>.1.@.0
+0000ea90: 0431 043e 0442 0430 0442 044c 0020 043e  .1.>.B.0.B.L. .>
+0000eaa0: 0442 043c 0435 043d 0451 043d 043d 043e  .B.<.5.=.Q.=.=.>
+0000eab0: 0435 0020 043a 043e 0440 043f 043e 0440  .5. .:.>.@.?.>.@
+0000eac0: 0430 0442 0438 0432 043d 043e 0435 0020  .0.B.8.2.=.>.5. 
+0000ead0: 0434 0435 0439 0441 0442 0432 0438 0435  .4.5.9.A.B.2.8.5
+0000eae0: 0800 0000 0006 0000 0028 4361 6e27 7420  .........(Can't 
+0000eaf0: 7072 6f63 6573 7320 6361 6e63 656c 6c65  process cancelle
+0000eb00: 6420 636f 7270 6f72 6174 6520 6163 7469  d corporate acti
+0000eb10: 6f6e 0700 0000 0d53 7461 7465 6d65 6e74  on.....Statement
+0000eb20: 4942 4b52 0103 0000 003e 0414 0435 043d  IBKR.....>...5.=
+0000eb30: 0435 0436 043d 044b 0435 0020 0442 0440  .5.6.=.K.5. .B.@
+0000eb40: 0430 043d 0437 0430 043a 0446 0438 0438  .0.=.7.0.:.F.8.8
+0000eb50: 0020 0437 0430 0433 0440 0443 0436 0435  . .7.0.3.@.C.6.5
+0000eb60: 043d 044b 003a 0020 0800 0000 0006 0000  .=.K.:. ........
+0000eb70: 001a 4361 7368 2074 7261 6e73 6163 7469  ..Cash transacti
+0000eb80: 6f6e 7320 6c6f 6164 6564 3a20 0700 0000  ons loaded: ....
+0000eb90: 0d53 7461 7465 6d65 6e74 4942 4b52 0103  .StatementIBKR..
+0000eba0: 0000 006a 041a 043e 0440 043f 043e 0440  ...j...>.@.?.>.@
+0000ebb0: 0430 0442 0438 0432 043d 043e 0435 0020  .0.B.8.2.=.>.5. 
+0000ebc0: 0441 043e 0431 044b 0442 0438 0435 0020  .A.>.1.K.B.8.5. 
+0000ebd0: 043d 0435 0020 043f 043e 0434 0434 0435  .=.5. .?.>.4.4.5
+0000ebe0: 0440 0436 0438 0432 0430 0435 0442 0441  .@.6.8.2.0.5.B.A
+0000ebf0: 044f 0020 0434 043b 044f 0020 0442 0438  .O. .4.;.O. .B.8
+0000ec00: 043f 0430 0020 0426 0411 003a 0020 0800  .?.0. .&...:. ..
+0000ec10: 0000 0006 0000 0031 436f 7270 6f72 6174  .......1Corporat
+0000ec20: 6520 6163 7469 6f6e 2069 736e 2774 2073  e action isn't s
+0000ec30: 7570 706f 7274 6564 2066 6f72 2061 7373  upported for ass
+0000ec40: 6574 2074 7970 653a 2007 0000 000d 5374  et type: .....St
+0000ec50: 6174 656d 656e 7449 424b 5201 0300 0000  atementIBKR.....
+0000ec60: 5e04 2204 3804 3f00 2004 3a04 3e04 4004  ^.".8.?. .:.>.@.
+0000ec70: 3f04 3e04 4004 3004 4204 3804 3204 3d04  ?.>.@.0.B.8.2.=.
+0000ec80: 3e04 3304 3e00 2004 3404 3504 3904 4104  >.3.>. .4.5.9.A.
+0000ec90: 4204 3204 3804 4f00 2004 3d04 3500 2004  B.2.8.O. .=.5. .
+0000eca0: 3f04 3e04 3404 3404 3504 4004 3604 3804  ?.>.4.4.5.@.6.8.
+0000ecb0: 3204 3004 3504 4204 4104 4f00 3a00 2008  2.0.5.B.A.O.:. .
+0000ecc0: 0000 0000 0600 0000 2843 6f72 706f 7261  ........(Corpora
+0000ecd0: 7465 2061 6374 696f 6e20 7479 7065 2069  te action type i
+0000ece0: 7320 6e6f 7420 7375 7070 6f72 7465 643a  s not supported:
+0000ecf0: 2007 0000 000d 5374 6174 656d 656e 7449   .....StatementI
+0000ed00: 424b 5201 0300 0000 4404 1a04 3e04 4004  BKR.....D...>.@.
+0000ed10: 3f04 3e04 4004 3004 4204 3804 3204 3d04  ?.>.@.0.B.8.2.=.
+0000ed20: 4b04 3500 2004 3404 3504 3904 4104 4204  K.5. .4.5.9.A.B.
+0000ed30: 3204 3804 4f00 2004 3704 3004 3304 4004  2.8.O. .7.0.3.@.
+0000ed40: 4304 3604 3504 3d04 4b00 3a00 2008 0000  C.6.5.=.K.:. ...
+0000ed50: 0000 0600 0000 1a43 6f72 706f 7261 7465  .......Corporate
+0000ed60: 2061 6374 696f 6e73 206c 6f61 6465 643a   actions loaded:
+0000ed70: 2007 0000 000d 5374 6174 656d 656e 7449   .....StatementI
+0000ed80: 424b 5201 0300 0000 5604 1404 3804 3204  BKR.....V...8.2.
+0000ed90: 3804 3404 3504 3d04 3400 2004 3d04 3500  8.4.5.=.4. .=.5.
+0000eda0: 2004 3d04 3004 3904 3404 3504 3d00 2004   .=.0.9.4.5.=. .
+0000edb0: 3404 3b04 4f00 2004 4304 3404 3504 4004  4.;.O. .C.4.5.@.
+0000edc0: 3604 3004 3d04 3d04 3e04 3304 3e00 2004  6.0.=.=.>.3.>. .
+0000edd0: 3d04 3004 3b04 3e04 3304 3000 3a00 2008  =.0.;.>.3.0.:. .
+0000ede0: 0000 0000 0600 0000 2844 6976 6964 656e  ........(Dividen
+0000edf0: 6420 6e6f 7420 666f 756e 6420 666f 7220  d not found for 
+0000ee00: 7769 7468 686f 6c64 696e 6720 7461 783a  withholding tax:
+0000ee10: 2007 0000 000d 5374 6174 656d 656e 7449   .....StatementI
+0000ee20: 424b 5201 0300 0000 2e00 4900 4200 4b00  BKR.......I.B.K.
+0000ee30: 5200 2000 6600 6c00 6500 7800 2d04 3e04  R. .f.l.e.x.-.>.
+0000ee40: 4204 4704 5104 4200 2000 2800 2a00 2e00  B.G.Q.B. .(.*...
+0000ee50: 7800 6d00 6c00 2908 0000 0000 0600 0000  x.m.l.).........
+0000ee60: 1749 424b 5220 666c 6578 2d71 7565 7279  .IBKR flex-query
+0000ee70: 2028 2a2e 786d 6c29 0700 0000 0d53 7461   (*.xml).....Sta
+0000ee80: 7465 6d65 6e74 4942 4b52 0103 0000 0026  tementIBKR.....&
+0000ee90: 0049 006e 0074 0065 0072 0061 0063 0074  .I.n.t.e.r.a.c.t
+0000eea0: 0069 0076 0065 0020 0042 0072 006f 006b  .i.v.e. .B.r.o.k
+0000eeb0: 0065 0072 0073 0800 0000 0006 0000 0013  .e.r.s..........
+0000eec0: 496e 7465 7261 6374 6976 6520 4272 6f6b  Interactive Brok
+0000eed0: 6572 7307 0000 000d 5374 6174 656d 656e  ers.....Statemen
+0000eee0: 7449 424b 5201 0300 0000 5604 2204 3804  tIBKR.....V.".8.
+0000eef0: 3f00 2004 3e04 4204 4704 5104 4204 3000  ?. .>.B.G.Q.B.0.
+0000ef00: 2000 4900 6e00 7400 6500 7200 6100 6300   .I.n.t.e.r.a.c.
+0000ef10: 7400 6900 7600 6500 2000 4200 7200 6f00  t.i.v.e. .B.r.o.
+0000ef20: 6b00 6500 7200 7300 2004 3d04 3500 2004  k.e.r.s. .=.5. .
+0000ef30: 3e04 3f04 4004 3504 3404 3504 3b04 5104  >.?.@.5.4.5.;.Q.
+0000ef40: 3d08 0000 0000 0600 0000 2949 6e74 6572  =.........)Inter
+0000ef50: 6163 7469 7665 2042 726f 6b65 7273 2072  active Brokers r
+0000ef60: 6570 6f72 7420 7479 7065 206e 6f74 2066  eport type not f
+0000ef70: 6f75 6e64 0700 0000 0d53 7461 7465 6d65  ound.....Stateme
+0000ef80: 6e74 4942 4b52 0103 0000 003a 0417 0430  ntIBKR.....:...0
+0000ef90: 0433 0440 0443 0437 043a 0430 0020 043e  .3.@.C.7.:.0. .>
+0000efa0: 0442 0447 0451 0442 0430 0020 0049 0042  .B.G.Q.B.0. .I.B
+0000efb0: 0020 0434 043b 044f 0020 0441 0447 0451  . .4.;.O. .A.G.Q
+0000efc0: 0442 0430 0020 0800 0000 0006 0000 0023  .B.0. .........#
+0000efd0: 4c6f 6164 2049 4220 466c 6578 2d73 7461  Load IB Flex-sta
+0000efe0: 7465 6d65 6e74 2066 6f72 2061 6363 6f75  tement for accou
+0000eff0: 6e74 2007 0000 000d 5374 6174 656d 656e  nt .....Statemen
+0000f000: 7449 424b 5201 0300 0000 5804 1d04 3504  tIBKR.....X...5.
+0000f010: 3404 3e04 4104 4204 3004 4204 3e04 4704  4.>.A.B.0.B.>.G.
+0000f020: 3d04 3e00 2004 3404 3004 3d04 3d04 4b04  =.>. .4.0.=.=.K.
+0000f030: 4500 2004 3e04 3100 2004 1e04 3104 4a04  E. .>.1. ...1.J.
+0000f040: 3504 3404 3804 3d04 3504 3d04 3804 3800  5.4.8.=.5.=.8.8.
+0000f050: 2004 3a04 3e04 3c04 3f04 3004 3d04 3804   .:.>.<.?.0.=.8.
+0000f060: 3900 2008 0000 0000 0600 0000 224d 6572  9. ........."Mer
+0000f070: 6765 7220 6465 7363 7269 7074 696f 6e20  ger description 
+0000f080: 6d69 7373 2073 6f6d 6520 6461 7461 2007  miss some data .
+0000f090: 0000 000d 5374 6174 656d 656e 7449 424b  ....StatementIBK
+0000f0a0: 5201 0300 0000 5e04 1d04 3504 3e04 3404  R.....^...5.>.4.
+0000f0b0: 3d04 3e04 3704 3d04 3004 4704 3d04 3e04  =.>.7.=.0.G.=.>.
+0000f0c0: 3500 2004 4104 3e04 3204 3f04 3004 3404  5. .A.>.2.?.0.4.
+0000f0d0: 3504 3d04 3804 3500 2004 4104 3e04 3104  5.=.8.5. .A.>.1.
+0000f0e0: 4b04 4204 3804 3900 2004 4004 3504 3e04  K.B.8.9. .@.5.>.
+0000f0f0: 4004 3304 3004 3d04 3804 3704 3004 4604  @.3.0.=.8.7.0.F.
+0000f100: 3804 3800 2008 0000 0000 0600 0000 294d  8.8. .........)M
+0000f110: 756c 7469 706c 6520 6d65 7267 6572 2072  ultiple merger r
+0000f120: 6563 6f72 6473 2061 6c72 6561 6479 2065  ecords already e
+0000f130: 7869 7374 2061 7420 0700 0000 0d53 7461  xist at .....Sta
+0000f140: 7465 6d65 6e74 4942 4b52 0103 0000 0052  tementIBKR.....R
+0000f150: 0414 0435 0439 0441 0442 0432 0438 0435  ...5.9.A.B.2.8.5
+0000f160: 0020 043d 0435 0020 043f 043e 0434 0434  . .=.5. .?.>.4.4
+0000f170: 0435 0440 0436 0438 0432 0430 0435 0442  .5.@.6.8.2.0.5.B
+0000f180: 0441 044f 0020 0434 043b 044f 0020 043e  .A.O. .4.;.O. .>
+0000f190: 043f 0446 0438 043e 043d 043e 0432 003a  .?.F.8.>.=.>.2.:
+0000f1a0: 0020 0800 0000 0006 0000 0027 4f70 7469  . .........'Opti
+0000f1b0: 6f6e 2045 2641 2645 2061 6374 696f 6e20  on E&A&E action 
+0000f1c0: 6973 6e27 7420 696d 706c 656d 656e 7465  isn't implemente
+0000f1d0: 643a 2007 0000 000d 5374 6174 656d 656e  d: .....Statemen
+0000f1e0: 7449 424b 5201 0300 0000 3a04 1804 4104  tIBKR.....:...A.
+0000f1f0: 3f04 3e04 3b04 3d04 3504 3d04 3804 3500  ?.>.;.=.5.=.8.5.
+0000f200: 2004 3f04 4004 3e04 3404 3004 3d04 3d04   .?.@.>.4.0.=.=.
+0000f210: 3e04 3304 3e00 2004 3e04 3f04 4604 3804  >.3.>. .>.?.F.8.
+0000f220: 3e04 3d04 3008 0000 0000 0600 0000 114f  >.=.0..........O
+0000f230: 7074 696f 6e20 6173 7369 676e 6d65 6e74  ption assignment
+0000f240: 0700 0000 0d53 7461 7465 6d65 6e74 4942  .....StatementIB
+0000f250: 4b52 0103 0000 003a 0418 0441 043f 043e  KR.....:...A.?.>
+0000f260: 043b 043d 0435 043d 0438 0435 002f 044d  .;.=.5.=.8.5./.M
+0000f270: 043a 0441 043f 0438 0440 0430 0446 0438  .:.A.?.8.@.0.F.8
+0000f280: 044f 0020 043e 043f 0446 0438 043e 043d  .O. .>.?.F.8.>.=
+0000f290: 0430 0800 0000 0006 0000 001a 4f70 7469  .0..........Opti
+0000f2a0: 6f6e 2061 7373 6967 6e6d 656e 742f 6578  on assignment/ex
+0000f2b0: 6572 6369 7365 0700 0000 0d53 7461 7465  ercise.....State
+0000f2c0: 6d65 6e74 4942 4b52 0103 0000 003a 0418  mentIBKR.....:..
+0000f2d0: 0441 043f 043e 043b 043d 0435 043d 0438  .A.?.>.;.=.5.=.8
+0000f2e0: 0435 0020 043a 0443 043f 043b 0435 043d  .5. .:.C.?.;.5.=
+0000f2f0: 043d 043e 0433 043e 0020 043e 043f 0446  .=.>.3.>. .>.?.F
+0000f300: 0438 043e 043d 0430 0800 0000 0006 0000  .8.>.=.0........
+0000f310: 000f 4f70 7469 6f6e 2065 7865 7263 6973  ..Option exercis
+0000f320: 6507 0000 000d 5374 6174 656d 656e 7449  e.....StatementI
+0000f330: 424b 5201 0300 0000 2404 2d04 3a04 4104  BKR.....$.-.:.A.
+0000f340: 3f04 3804 4004 3004 4604 3804 4f00 2004  ?.8.@.0.F.8.O. .
+0000f350: 3e04 3f04 4604 3804 3e04 3d04 3008 0000  >.?.F.8.>.=.0...
+0000f360: 0000 0600 0000 114f 7074 696f 6e20 6578  .......Option ex
+0000f370: 7069 7261 7469 6f6e 0700 0000 0d53 7461  piration.....Sta
+0000f380: 7465 6d65 6e74 4942 4b52 0103 0000 0040  tementIBKR.....@
+0000f390: 0414 0435 0439 0441 0442 0432 0438 044f  ...5.9.A.B.2.8.O
+0000f3a0: 0020 0441 0020 043e 043f 0446 0438 043e  . .A. .>.?.F.8.>
+0000f3b0: 043d 0430 043c 0438 0020 0437 0430 0433  .=.0.<.8. .7.0.3
+0000f3c0: 0440 0443 0436 0435 043d 044b 003a 0020  .@.C.6.5.=.K.:. 
+0000f3d0: 0800 0000 0006 0000 0016 4f70 7469 6f6e  ..........Option
+0000f3e0: 7320 4526 4126 4520 6c6f 6164 6564 3a20  s E&A&E loaded: 
+0000f3f0: 0700 0000 0d53 7461 7465 6d65 6e74 4942  .....StatementIB
+0000f400: 4b52 0103 0000 006a 041d 0435 0020 043d  KR.....j...5. .=
+0000f410: 0430 0439 0434 0435 043d 0430 0020 0441  .0.9.4.5.=.0. .A
+0000f420: 0434 0435 043b 043a 0430 0020 0434 043b  .4.5.;.:.0. .4.;
+0000f430: 044f 0020 0438 0441 043f 043e 043b 043d  .O. .8.A.?.>.;.=
+0000f440: 0435 043d 0438 044f 002f 044d 043a 0441  .5.=.8.O./.M.:.A
+0000f450: 043f 0438 0440 0430 0446 0438 0438 0020  .?.8.@.0.F.8.8. 
+0000f460: 043e 043f 0446 0438 043e 043d 0430 003a  .>.?.F.8.>.=.0.:
+0000f470: 0020 0800 0000 0006 0000 0035 4f72 6967  . .........5Orig
+0000f480: 696e 616c 2074 7261 6465 206e 6f74 2066  inal trade not f
+0000f490: 6f75 6e64 2066 6f72 204f 7074 696f 6e20  ound for Option 
+0000f4a0: 4526 4126 4520 6f70 6572 6174 696f 6e3a  E&A&E operation:
+0000f4b0: 2007 0000 000d 5374 6174 656d 656e 7449   .....StatementI
+0000f4c0: 424b 5201 0300 0000 6c04 1f04 3b04 3004  BKR.....l...;.0.
+0000f4d0: 4204 5104 3600 2004 3104 4b04 3b00 2004  B.Q.6. .1.K.;. .
+0000f4e0: 3e04 4204 3c04 3504 3d04 5104 3d00 2004  >.B.<.5.=.Q.=. .
+0000f4f0: 3f04 3e00 2004 3f04 4004 3804 3c04 3504  ?.>. .?.@.8.<.5.
+0000f500: 4004 3d04 3e04 3c04 4300 2004 4104 3e04  @.=.>.<.C. .A.>.
+0000f510: 3204 3f04 3004 3404 3504 3d04 3804 4e00  2.?.0.4.5.=.8.N.
+0000f520: 2004 3e04 3f04 3804 4104 3004 3d04 3804   .>.?.8.A.0.=.8.
+0000f530: 4f00 3a00 2008 0000 0000 0600 0000 3150  O.:. .........1P
+0000f540: 6179 6d65 6e74 2077 6173 2072 6576 6572  ayment was rever
+0000f550: 7365 6420 6279 2061 7070 726f 7869 6d61  sed by approxima
+0000f560: 7465 2064 6573 6372 6970 7469 6f6e 3a20  te description: 
+0000f570: 0700 0000 0d53 7461 7465 6d65 6e74 4942  .....StatementIB
+0000f580: 4b52 0103 0000 006a 041f 043b 0430 0442  KR.....j...;.0.B
+0000f590: 0451 0436 0020 0431 044b 043b 0020 043e  .Q.6. .1.K.;. .>
+0000f5a0: 0442 043c 0435 043d 0451 043d 002c 0020  .B.<.5.=.Q.=.,. 
+0000f5b0: 043d 043e 0020 0441 0020 043d 0435 0441  .=.>. .A. .=.5.A
+0000f5c0: 043e 0432 043f 0430 0434 0430 044e 0449  .>.2.?.0.4.0.N.I
+0000f5d0: 0435 0439 0020 0434 0430 0442 043e 0439  .5.9. .4.0.B.>.9
+0000f5e0: 0020 043e 0442 0447 0451 0442 0430 003a  . .>.B.G.Q.B.0.:
+0000f5f0: 0020 0800 0000 0006 0000 0033 5061 796d  . .........3Paym
+0000f600: 656e 7420 7761 7320 7265 7665 7273 6564  ent was reversed
+0000f610: 2077 6974 6820 6469 6666 6572 656e 7420   with different 
+0000f620: 7265 706f 7274 6564 2064 6174 653a 2007  reported date: .
+0000f630: 0000 000d 5374 6174 656d 656e 7449 424b  ....StatementIBK
+0000f640: 5201 0300 0000 2804 1f04 3b04 3004 4204  R.....(...;.0.B.
+0000f650: 5104 3600 2004 3104 4b04 3b00 2004 3e04  Q.6. .1.K.;. .>.
+0000f660: 4204 3c04 3504 3d04 5104 3d00 3a00 2008  B.<.5.=.Q.=.:. .
+0000f670: 0000 0000 0600 0000 1650 6179 6d65 6e74  .........Payment
+0000f680: 2077 6173 2072 6576 6572 7365 643a 2007   was reversed: .
+0000f690: 0000 000d 5374 6174 656d 656e 7449 424b  ....StatementIBK
+0000f6a0: 5201 0300 0000 1c04 2604 1100 2004 3704  R.......&... .7.
+0000f6b0: 3004 3304 4004 4304 3604 3504 3d04 4b00  0.3.@.C.6.5.=.K.
+0000f6c0: 3a00 2008 0000 0000 0600 0000 1353 6563  :. ..........Sec
+0000f6d0: 7572 6974 6965 7320 6c6f 6164 6564 3a20  urities loaded: 
+0000f6e0: 0700 0000 0d53 7461 7465 6d65 6e74 4942  .....StatementIB
+0000f6f0: 4b52 0103 0000 0056 041d 0435 0434 043e  KR.....V...5.4.>
+0000f700: 0441 0442 0430 0442 043e 0447 043d 043e  .A.B.0.B.>.G.=.>
+0000f710: 0020 0434 0430 043d 043d 044b 0445 0020  . .4.0.=.=.K.E. 
+0000f720: 0434 043b 044f 0020 0412 044b 0434 0435  .4.;.O. ...K.4.5
+0000f730: 043b 0435 043d 0438 044f 0020 043a 043e  .;.5.=.8.O. .:.>
+0000f740: 043c 043f 0430 043d 0438 0438 0020 0800  .<.?.0.=.8.8. ..
+0000f750: 0000 0006 0000 0024 5370 696e 2d6f 6666  .......$Spin-off
+0000f760: 2064 6573 6372 6970 7469 6f6e 206d 6973   description mis
+0000f770: 7320 736f 6d65 2064 6174 6120 0700 0000  s some data ....
+0000f780: 0d53 7461 7465 6d65 6e74 4942 4b52 0103  .StatementIBKR..
+0000f790: 0000 005c 0418 0441 0445 043e 0434 043d  ...\...A.E.>.4.=
+0000f7a0: 0430 044f 0020 0426 0411 0020 0434 043b  .0.O. .&... .4.;
+0000f7b0: 044f 0020 0432 044b 0434 0435 043b 0435  .O. .2.K.4.5.;.5
+0000f7c0: 043d 0438 044f 0020 043a 043e 043c 043f  .=.8.O. .:.>.<.?
+0000f7d0: 0430 043d 0438 0438 0020 043d 0435 0020  .0.=.8.8. .=.5. 
+0000f7e0: 043d 0430 0439 0434 0435 043d 0430 0020  .=.0.9.4.5.=.0. 
+0000f7f0: 0800 0000 0006 0000 0021 5370 696e 2d6f  .........!Spin-o
+0000f800: 6666 2069 6e69 7469 616c 2061 7373 6574  ff initial asset
+0000f810: 206e 6f74 2066 6f75 6e64 2007 0000 000d   not found .....
+0000f820: 5374 6174 656d 656e 7449 424b 5201 0300  StatementIBKR...
+0000f830: 0000 5604 1e04 4804 3804 3104 3a04 3000  ..V...H.8.1.:.0.
+0000f840: 2004 3e04 3a04 4004 4304 3304 3b04 3504   .>.:.@.C.3.;.5.
+0000f850: 3d04 3804 4f00 2000 5300 7000 6900 6e00  =.8.O. .S.p.i.n.
+0000f860: 2d00 6f00 6600 6600 2004 4104 3b04 3804  -.o.f.f. .A.;.8.
+0000f870: 4804 3a04 3e04 3c00 2004 3104 3e04 3b04  H.:.>.<. .1.>.;.
+0000f880: 4c04 4804 3004 4f00 2008 0000 0000 0600  L.H.0.O. .......
+0000f890: 0000 2353 7069 6e2d 6f66 6620 726f 756e  ..#Spin-off roun
+0000f8a0: 6469 6e67 2065 7272 6f72 2069 7320 746f  ding error is to
+0000f8b0: 6f20 6269 6720 0700 0000 0d53 7461 7465  o big .....State
+0000f8c0: 6d65 6e74 4942 4b52 0103 0000 003e 041d  mentIBKR.....>..
+0000f8d0: 0435 0434 043e 0441 0442 0430 0442 043e  .5.4.>.A.B.0.B.>
+0000f8e0: 0447 043d 043e 0020 0434 0430 043d 043d  .G.=.>. .4.0.=.=
+0000f8f0: 044b 0445 0020 0434 043b 044f 0020 0421  .K.E. .4.;.O. .!
+0000f900: 043f 043b 0438 0442 0430 0020 0800 0000  .?.;.8.B.0. ....
+0000f910: 0006 0000 0021 5370 6c69 7420 6465 7363  .....!Split desc
+0000f920: 7269 7074 696f 6e20 6d69 7373 2073 6f6d  ription miss som
+0000f930: 6520 6461 7461 2007 0000 000d 5374 6174  e data .....Stat
+0000f940: 656d 656e 7449 424b 5201 0300 0000 3804  ementIBKR.....8.
+0000f950: 1704 3004 4704 3804 4104 3b04 3504 3d04  ..0.G.8.A.;.5.=.
+0000f960: 3804 3500 2004 3004 3a04 4604 3804 3900  8.5. .0.:.F.8.9.
+0000f970: 2004 3704 3004 3304 4004 4304 3604 3504   .7.0.3.@.C.6.5.
+0000f980: 3d04 3e00 3a00 2008 0000 0000 0600 0000  =.>.:. .........
+0000f990: 1753 746f 636b 2076 6573 7469 6e67 7320  .Stock vestings 
+0000f9a0: 6c6f 6164 6564 3a20 0700 0000 0d53 7461  loaded: .....Sta
+0000f9b0: 7465 6d65 6e74 4942 4b52 0103 0000 0048  tementIBKR.....H
+0000f9c0: 041a 043e 0440 0440 0435 043a 0442 0438  ...>.@.@.5.:.B.8
+0000f9d0: 0440 043e 0432 043a 0430 0020 043d 0430  .@.>.2.:.0. .=.0
+0000f9e0: 043b 043e 0433 0430 0020 0434 043b 044f  .;.>.3.0. .4.;.O
+0000f9f0: 0020 0434 0438 0432 0438 0434 0435 043d  . .4.8.2.8.4.5.=
+0000fa00: 0434 0430 003a 0020 0800 0000 0006 0000  .4.0.:. ........
+0000fa10: 001d 5461 7820 6164 6a75 7374 6d65 6e74  ..Tax adjustment
+0000fa20: 2066 6f72 2064 6976 6964 656e 643a 2007   for dividend: .
+0000fa30: 0000 000d 5374 6174 656d 656e 7449 424b  ....StatementIBK
+0000fa40: 5201 0300 0000 2404 1d04 3004 3b04 3e04  R.....$...0.;.>.
+0000fa50: 3304 3800 2004 3704 3004 3304 4004 4304  3.8. .7.0.3.@.C.
+0000fa60: 3604 3504 3d04 4b00 3a00 2008 0000 0000  6.5.=.K.:. .....
+0000fa70: 0600 0000 0e54 6178 6573 206c 6f61 6465  .....Taxes loade
+0000fa80: 643a 2007 0000 000d 5374 6174 656d 656e  d: .....Statemen
+0000fa90: 7449 424b 5201 03ff ffff ff08 0000 0000  tIBKR...........
+0000faa0: 0600 0000 0f54 7261 6465 7320 6c6f 6164  .....Trades load
+0000fab0: 6564 3a20 0700 0000 0d53 7461 7465 6d65  ed: .....Stateme
+0000fac0: 6e74 4942 4b52 0103 0000 0058 041d 0435  ntIBKR.....X...5
+0000fad0: 043f 043e 0434 0434 0435 0440 0436 0438  .?.>.4.4.5.@.6.8
+0000fae0: 0432 0430 0435 043c 044b 0439 0020 0444  .2.0.5.<.K.9. .D
+0000faf0: 043e 0440 043c 0430 0442 0020 043e 043f  .>.@.<.0.B. .>.?
+0000fb00: 0438 0441 0430 043d 0438 044f 0020 0434  .8.A.0.=.8.O. .4
+0000fb10: 0438 0432 0438 0434 0435 043d 0434 0430  .8.2.8.4.5.=.4.0
+0000fb20: 003a 0020 0800 0000 0006 0000 0022 556e  .:. ........."Un
+0000fb30: 6861 6e64 6c65 6420 6469 7669 6465 6e64  handled dividend
+0000fb40: 2070 6174 7465 726e 2066 6f75 6e64 3a20   pattern found: 
+0000fb50: 0700 0000 0d53 7461 7465 6d65 6e74 4942  .....StatementIB
+0000fb60: 4b52 0103 0000 004e 041d 0435 043f 043e  KR.....N...5.?.>
+0000fb70: 0434 0434 0435 0440 0436 0438 0432 0430  .4.4.5.@.6.8.2.0
+0000fb80: 0435 043c 044b 0439 0020 0444 043e 0440  .5.<.K.9. .D.>.@
+0000fb90: 043c 0430 0442 0020 0441 0442 0440 0430  .<.0.B. .A.B.@.0
+0000fba0: 043d 044b 0020 043d 0430 043b 043e 0433  .=.K. .=.0.;.>.3
+0000fbb0: 0430 003a 0020 0800 0000 0006 0000 0025  .0.:. .........%
+0000fbc0: 556e 6861 6e64 6c65 6420 7461 7820 636f  Unhandled tax co
+0000fbd0: 756e 7472 7920 7061 7474 6572 6e20 666f  untry pattern fo
+0000fbe0: 756e 643a 2007 0000 000d 5374 6174 656d  und: .....Statem
+0000fbf0: 656e 7449 424b 5201 0300 0000 5204 1d04  entIBKR.....R...
+0000fc00: 3504 3f04 3e04 3404 3404 3504 4004 3604  5.?.>.4.4.5.@.6.
+0000fc10: 3804 3204 3004 3504 3c04 4b04 3900 2004  8.2.0.5.<.K.9. .
+0000fc20: 4404 3e04 4004 3c04 3004 4200 2004 3e04  D.>.@.<.0.B. .>.
+0000fc30: 3f04 3804 4104 3004 3d04 3804 4f00 2004  ?.8.A.0.=.8.O. .
+0000fc40: 3d04 3004 3b04 3e04 3304 3000 3a00 2008  =.0.;.>.3.0.:. .
+0000fc50: 0000 0000 0600 0000 1d55 6e68 616e 646c  .........Unhandl
+0000fc60: 6564 2074 6178 2070 6174 7465 726e 2066  ed tax pattern f
+0000fc70: 6f75 6e64 3a20 0700 0000 0d53 7461 7465  ound: .....State
+0000fc80: 6d65 6e74 4942 4b52 0103 0000 0058 041d  mentIBKR.....X..
+0000fc90: 0435 0438 0437 0432 0435 0441 0442 043d  .5.8.7.2.5.A.B.=
+0000fca0: 044b 0439 0020 0442 0438 043f 0020 043e  .K.9. .B.8.?. .>
+0000fcb0: 0442 0447 0451 0442 0430 0020 0049 006e  .B.G.Q.B.0. .I.n
+0000fcc0: 0074 0065 0072 0061 0063 0074 0069 0076  .t.e.r.a.c.t.i.v
+0000fcd0: 0065 0020 0042 0072 006f 006b 0065 0072  .e. .B.r.o.k.e.r
+0000fce0: 0073 003a 0020 0800 0000 0006 0000 0029  .s.:. .........)
+0000fcf0: 556e 6b6e 6f77 6e20 496e 7465 7261 6374  Unknown Interact
+0000fd00: 6976 6520 4272 6f6b 6572 7320 7265 706f  ive Brokers repo
+0000fd10: 7274 2074 7970 653a 2007 0000 000d 5374  rt type: .....St
+0000fd20: 6174 656d 656e 7449 424b 5201 0300 0000  atementIBKR.....
+0000fd30: a204 1204 4b00 2004 3f04 4b04 4204 3004  ....K. .?.K.B.0.
+0000fd40: 3504 4204 3504 4104 4c00 2004 3704 3004  5.B.5.A.L. .7.0.
+0000fd50: 3304 4004 4304 3704 3804 4204 4c00 2004  3.@.C.7.8.B.L. .
+0000fd60: 3e04 4204 4704 5104 4200 2004 3e00 2004  >.B.G.Q.B. .>. .
+0000fd70: 3f04 3e04 3404 4204 3204 3504 4004 3604  ?.>.4.B.2.5.@.6.
+0000fd80: 3404 5104 3d04 3d04 4b04 4500 2004 4104  4.Q.=.=.K.E. .A.
+0000fd90: 3404 3504 3b04 3a04 3004 4500 2004 3204  4.5.;.:.0.E. .2.
+0000fda0: 3c04 3504 4104 4204 3e00 2004 3e04 4204  <.5.A.B.>. .>.B.
+0000fdb0: 4704 5104 4204 3000 2004 3f04 3e00 2004  G.Q.B.0. .?.>. .
+0000fdc0: 1004 3a04 4204 3804 3204 3d04 3e04 4104  ..:.B.8.2.=.>.A.
+0000fdd0: 4204 3808 0000 0000 0600 0000 3f59 6f75  B.8.........?You
+0000fde0: 2074 7279 2074 6f20 696d 706f 7274 2054   try to import T
+0000fdf0: 7261 6465 2063 6f6e 6669 6d61 7469 6f6e  rade confimation
+0000fe00: 2072 6570 6f72 742c 206e 6f74 2041 6374   report, not Act
+0000fe10: 6976 6974 7920 7265 706f 7274 0700 0000  ivity report....
+0000fe20: 0d53 7461 7465 6d65 6e74 4942 4b52 0103  .StatementIBKR..
+0000fe30: 0000 0052 041d 0435 0432 043e 0437 043c  ...R...5.2.>.7.<
+0000fe40: 043e 0436 043d 043e 0020 0440 0430 0441  .>.6.=.>. .@.0.A
+0000fe50: 043f 043e 0437 043d 0430 0442 044c 0020  .?.>.7.=.0.B.L. 
+0000fe60: 043e 043f 0438 0441 0430 043d 0438 0435  .>.?.8.A.0.=.8.5
+0000fe70: 0020 0434 0438 0432 0438 0434 0435 043d  . .4.8.2.8.4.5.=
+0000fe80: 0434 0430 0020 0800 0000 0006 0000 0021  .4.0. .........!
+0000fe90: 4361 6e27 7420 7061 7273 6520 4469 7669  Can't parse Divi
+0000fea0: 6465 6e64 2064 6573 6372 6970 7469 6f6e  dend description
+0000feb0: 2007 0000 000c 5374 6174 656d 656e 744a   .....StatementJ
+0000fec0: 3254 0103 0000 001c 0414 0421 0020 0437  2T.........!. .7
+0000fed0: 0430 0433 0440 0443 0436 0435 043d 044b  .0.3.@.C.6.5.=.K
+0000fee0: 003a 0020 0800 0000 0006 0000 0016 4361  .:. ..........Ca
+0000fef0: 7368 2062 616c 616e 6365 7320 6c6f 6164  sh balances load
+0000ff00: 6564 3a20 0700 0000 0c53 7461 7465 6d65  ed: .....Stateme
+0000ff10: 6e74 4a32 5401 0300 0000 3a04 1404 3504  ntJ2T.....:...5.
+0000ff20: 3d04 3504 3604 3d04 4b04 4500 2004 3e04  =.5.6.=.K.E. .>.
+0000ff30: 3f04 3504 4004 3004 4604 3804 3900 2004  ?.5.@.0.F.8.9. .
+0000ff40: 3704 3004 3304 4004 4304 3604 3504 3d04  7.0.3.@.C.6.5.=.
+0000ff50: 3e00 3a00 2008 0000 0000 0600 0000 1843  >.:. ..........C
+0000ff60: 6173 6820 6f70 6572 6174 696f 6e73 206c  ash operations l
+0000ff70: 6f61 6465 643a 2007 0000 000c 5374 6174  oaded: .....Stat
+0000ff80: 656d 656e 744a 3254 0103 0000 0048 0421  ementJ2T.....H.!
+0000ff90: 0434 0435 043b 043a 0438 0020 0441 0020  .4.5.;.:.8. .A. 
+0000ffa0: 043a 0440 0438 043f 0442 043e 002d 0432  .:.@.8.?.B.>.-.2
+0000ffb0: 0430 043b 044e 0442 0430 043c 0438 0020  .0.;.N.B.0.<.8. 
+0000ffc0: 0437 0430 0433 0440 0443 0436 0435 043d  .7.0.3.@.C.6.5.=
+0000ffd0: 044b 003a 0020 0800 0000 0006 0000 0016  .K.:. ..........
+0000ffe0: 4372 7970 746f 2074 7261 6465 7320 6c6f  Crypto trades lo
+0000fff0: 6164 6564 3a20 0700 0000 0c53 7461 7465  aded: .....State
+00010000: 6d65 6e74 4a32 5401 0300 0000 5004 1200  mentJ2T.....P...
+00010010: 2004 3e04 3f04 3804 4104 3004 3d04 3804   .>.?.8.A.0.=.8.
+00010020: 3800 2004 3404 3804 3204 3804 3404 3504  8. .4.8.2.8.4.5.
+00010030: 3d04 3404 3000 2004 3e04 4204 4104 4304  =.4.0. .>.B.A.C.
+00010040: 4204 4104 4204 3204 4304 4e04 4200 2004  B.A.B.2.C.N.B. .
+00010050: 3404 3004 3d04 3d04 4b04 3500 2008 0000  4.0.=.=.K.5. ...
+00010060: 0000 0600 0000 2444 6976 6964 656e 6420  ......$Dividend 
+00010070: 6465 7363 7269 7074 696f 6e20 6d69 7373  description miss
+00010080: 2073 6f6d 6520 6461 7461 2007 0000 000c   some data .....
+00010090: 5374 6174 656d 656e 744a 3254 0103 0000  StatementJ2T....
+000100a0: 004e 0414 0438 0432 0438 0434 0435 043d  .N...8.2.8.4.5.=
+000100b0: 0434 0020 043d 0435 0020 043d 0430 0439  .4. .=.5. .=.0.9
+000100c0: 0434 0435 043d 0020 0434 043b 044f 0020  .4.5.=. .4.;.O. 
+000100d0: 0441 043f 0438 0441 0430 043d 0438 044f  .A.?.8.A.0.=.8.O
+000100e0: 0020 043d 0430 043b 043e 0433 0430 0020  . .=.0.;.>.3.0. 
+000100f0: 0800 0000 0006 0000 001f 4469 7669 6465  ..........Divide
+00010100: 6e64 2066 6f72 2074 6178 2077 6173 206e  nd for tax was n
+00010110: 6f74 2066 6f75 6e64 2007 0000 000c 5374  ot found .....St
+00010120: 6174 656d 656e 744a 3254 0103 0000 0044  atementJ2T.....D
+00010130: 0422 0440 0430 043d 0437 0430 043a 0446  .".@.0.=.7.0.:.F
+00010140: 0438 044f 0020 043f 0440 043e 043f 0443  .8.O. .?.@.>.?.C
+00010150: 0449 0435 043d 0430 0020 043f 0440 0438  .I.5.=.0. .?.@.8
+00010160: 0020 0438 043c 043f 043e 0440 0442 0435  . .8.<.?.>.@.B.5
+00010170: 003a 0020 0800 0000 0006 0000 001f 496d  .:. ..........Im
+00010180: 706f 7274 2073 6b69 7070 6564 206f 6620  port skipped of 
+00010190: 7472 616e 7361 6374 696f 6e3a 2007 0000  transaction: ...
+000101a0: 000c 5374 6174 656d 656e 744a 3254 0103  ..StatementJ2T..
+000101b0: 0000 0014 004a 0075 0073 0074 0032 0054  .....J.u.s.t.2.T
+000101c0: 0072 0061 0064 0065 0800 0000 0006 0000  .r.a.d.e........
+000101d0: 000a 4a75 7374 3254 7261 6465 0700 0000  ..Just2Trade....
+000101e0: 0c53 7461 7465 6d65 6e74 4a32 5401 0300  .StatementJ2T...
+000101f0: 0000 3204 1e04 4204 4704 5104 4200 2000  ..2...B.G.Q.B. .
+00010200: 4a00 7500 7300 7400 3200 5400 7200 6100  J.u.s.t.2.T.r.a.
+00010210: 6400 6500 2000 2800 2a00 2e00 7800 6c00  d.e. .(.*...x.l.
+00010220: 7300 7800 2908 0000 0000 0600 0000 1d4a  s.x.)..........J
+00010230: 7573 7432 5472 6164 6520 7374 6174 656d  ust2Trade statem
+00010240: 656e 7420 282a 2e78 6c73 7829 0700 0000  ent (*.xlsx)....
+00010250: 0c53 7461 7465 6d65 6e74 4a32 5401 0300  .StatementJ2T...
+00010260: 0000 1c04 2604 1100 2004 3704 3004 3304  ....&... .7.0.3.
+00010270: 4004 4304 3604 3504 3d04 4b00 3a00 2008  @.C.6.5.=.K.:. .
+00010280: 0000 0000 0600 0000 1353 6563 7572 6974  .........Securit
+00010290: 6965 7320 6c6f 6164 6564 3a20 0700 0000  ies loaded: ....
+000102a0: 0c53 7461 7465 6d65 6e74 4a32 5401 0300  .StatementJ2T...
+000102b0: 0000 3804 2104 3404 3504 3b04 3a04 3800  ..8.!.4.5.;.:.8.
+000102c0: 2004 4100 2004 3004 3a04 4604 3804 4f04   .A. .0.:.F.8.O.
+000102d0: 3c04 3800 2004 3704 3004 3304 4004 4304  <.8. .7.0.3.@.C.
+000102e0: 3604 3504 3d04 4b00 3a00 2008 0000 0000  6.5.=.K.:. .....
+000102f0: 0600 0000 1553 746f 636b 2074 7261 6465  .....Stock trade
+00010300: 7320 6c6f 6164 6564 3a20 0700 0000 0c53  s loaded: .....S
+00010310: 7461 7465 6d65 6e74 4a32 5401 0300 0000  tatementJ2T.....
+00010320: 4004 1d04 3504 3804 3704 3204 3504 4104  @...5.8.7.2.5.A.
+00010330: 4204 3d04 3004 4f00 2004 3404 3504 3d04  B.=.0.O. .4.5.=.
+00010340: 3504 3604 3d04 3004 4f00 2004 4204 4004  5.6.=.0.O. .B.@.
+00010350: 3004 3d04 3704 3004 3a04 4604 3804 4f00  0.=.7.0.:.F.8.O.
+00010360: 2008 0000 0000 0600 0000 1e55 6e6b 6e6f   ..........Unkno
+00010370: 776e 2063 6173 6820 7472 616e 7361 6374  wn cash transact
+00010380: 696f 6e20 7479 7065 2007 0000 000c 5374  ion type .....St
+00010390: 6174 656d 656e 744a 3254 0103 0000 0030  atementJ2T.....0
+000103a0: 041d 0435 0438 0437 0432 0435 0441 0442  ...5.8.7.2.5.A.B
+000103b0: 043d 044b 0439 0020 0442 0438 043f 0020  .=.K.9. .B.8.?. 
+000103c0: 0441 0434 0435 043b 043a 0438 003a 0020  .A.4.5.;.:.8.:. 
+000103d0: 0800 0000 0006 0000 0014 556e 6b6e 6f77  ..........Unknow
+000103e0: 6e20 7472 6164 6520 7479 7065 3a20 0700  n trade type: ..
+000103f0: 0000 0c53 7461 7465 6d65 6e74 4a32 5401  ...StatementJ2T.
+00010400: 0300 0000 4a04 1d04 3504 3f04 3e04 3404  ....J...5.?.>.4.
+00010410: 3404 3504 4004 3604 3804 3204 3004 3504  4.5.@.6.8.2.0.5.
+00010420: 3c04 3004 4f00 2004 3404 3504 3d04 3504  <.0.O. .4.5.=.5.
+00010430: 3604 3d04 3004 4f00 2004 4204 4004 3004  6.=.0.O. .B.@.0.
+00010440: 3d04 3704 3004 3a04 4604 3804 4f00 2008  =.7.0.:.F.8.O. .
+00010450: 0000 0000 0600 0000 1e55 6e73 7570 7070  .........Unsuppp
+00010460: 6f72 7465 6420 6361 7368 2074 7261 6e73  orted cash trans
+00010470: 6163 7469 6f6e 2007 0000 000c 5374 6174  action .....Stat
+00010480: 656d 656e 744a 3254 0103 0000 003a 0414  ementJ2T.....:..
+00010490: 0435 043d 0435 0436 043d 044b 0445 0020  .5.=.5.6.=.K.E. 
+000104a0: 043e 043f 0435 0440 0430 0446 0438 0439  .>.?.5.@.0.F.8.9
+000104b0: 0020 0437 0430 0433 0440 0443 0436 0435  . .7.0.3.@.C.6.5
+000104c0: 043d 043e 003a 0020 0800 0000 0006 0000  .=.>.:. ........
+000104d0: 0018 4361 7368 206f 7065 7261 7469 6f6e  ..Cash operation
+000104e0: 7320 6c6f 6164 6564 3a20 0700 0000 0c53  s loaded: .....S
+000104f0: 7461 7465 6d65 6e74 4b49 5401 0300 0000  tatementKIT.....
+00010500: 7604 1d04 3004 3b04 3e04 3300 2004 3d04  v...0.;.>.3. .=.
+00010510: 3000 2004 3404 3804 3204 3804 3404 3504  0. .4.8.2.8.4.5.
+00010520: 3d04 3404 4b00 2004 3d04 3500 2004 3f04  =.4.K. .=.5. .?.
+00010530: 3e04 3404 3404 3504 4004 3604 3804 3204  >.4.4.5.@.6.8.2.
+00010540: 3004 3504 4204 4104 4f00 2004 3404 3b04  0.5.B.A.O. .4.;.
+00010550: 4f00 2004 3104 4004 3e04 3a04 3504 4004  O. .1.@.>.:.5.@.
+00010560: 3000 2004 1a04 1804 2200 2d04 4404 3804  0. .....".-.D.8.
+00010570: 3d04 3004 3d04 4108 0000 0000 0600 0000  =.0.=.A.........
+00010580: 3e44 6976 6964 656e 6420 7461 7865 7320  >Dividend taxes 
+00010590: 6172 6520 6e6f 7420 7375 7070 6f72 7465  are not supporte
+000105a0: 6420 666f 7220 4b49 5420 6272 6f6b 6572  d for KIT broker
+000105b0: 2073 7461 7465 6d65 6e74 7320 7965 7407   statements yet.
+000105c0: 0000 000c 5374 6174 656d 656e 744b 4954  ....StatementKIT
+000105d0: 0103 0000 0014 041a 0418 0422 0020 0424  ...........". .$
+000105e0: 0438 043d 0430 043d 0441 0800 0000 0006  .8.=.0.=.A......
+000105f0: 0000 000b 4b49 5420 4669 6e61 6e63 6507  ....KIT Finance.
+00010600: 0000 000c 5374 6174 656d 656e 744b 4954  ....StatementKIT
+00010610: 0103 0000 0032 041e 0442 0447 0451 0442  .....2...B.G.Q.B
+00010620: 0020 041a 0418 0422 0020 0424 0438 043d  . .....". .$.8.=
+00010630: 0430 043d 0441 0020 0028 002a 002e 0078  .0.=.A. .(.*...x
+00010640: 006c 0073 0078 0029 0800 0000 0006 0000  .l.s.x.)........
+00010650: 001e 4b49 5420 4669 6e61 6e63 6520 7374  ..KIT Finance st
+00010660: 6174 656d 656e 7420 282a 2e78 6c73 7829  atement (*.xlsx)
+00010670: 0700 0000 0c53 7461 7465 6d65 6e74 4b49  .....StatementKI
+00010680: 5401 0300 0000 2404 2104 3404 3504 3b04  T.....$.!.4.5.;.
+00010690: 3a04 3800 2004 3704 3004 3304 4004 4304  :.8. .7.0.3.@.C.
+000106a0: 3604 3504 3d04 4b00 3a00 2008 0000 0000  6.5.=.K.:. .....
+000106b0: 0600 0000 0f54 7261 6465 7320 6c6f 6164  .....Trades load
+000106c0: 6564 3a20 0700 0000 0c53 7461 7465 6d65  ed: .....Stateme
+000106d0: 6e74 4b49 5401 0300 0000 3004 1d04 3504  ntKIT.....0...5.
+000106e0: 3804 3704 3204 3504 4104 4204 3d04 4b04  8.7.2.5.A.B.=.K.
+000106f0: 3900 2004 4204 3804 3f00 2004 4104 3404  9. .B.8.?. .A.4.
+00010700: 3504 3b04 3a04 3800 3a00 2008 0000 0000  5.;.:.8.:. .....
+00010710: 0600 0000 1455 6e6b 6e6f 776e 2074 7261  .....Unknown tra
+00010720: 6465 2074 7970 653a 2007 0000 000c 5374  de type: .....St
+00010730: 6174 656d 656e 744b 4954 0103 0000 004a  atementKIT.....J
+00010740: 041d 0435 043f 043e 0434 0434 0435 0440  ...5.?.>.4.4.5.@
+00010750: 0436 0438 0432 0430 0435 043c 0430 044f  .6.8.2.0.5.<.0.O
+00010760: 0020 0434 0435 043d 0435 0436 043d 0430  . .4.5.=.5.6.=.0
+00010770: 044f 0020 0442 0440 0430 043d 0437 0430  .O. .B.@.0.=.7.0
+00010780: 043a 0446 0438 044f 0020 0800 0000 0006  .:.F.8.O. ......
+00010790: 0000 001e 556e 7375 7070 706f 7274 6564  ....Unsuppported
+000107a0: 2063 6173 6820 7472 616e 7361 6374 696f   cash transactio
+000107b0: 6e20 0700 0000 0c53 7461 7465 6d65 6e74  n .....Statement
+000107c0: 4b49 5401 0300 0000 2204 2104 4704 3504  KIT.....".!.G.5.
+000107d0: 4204 3000 2004 3704 3004 3304 4004 4304  B.0. .7.0.3.@.C.
+000107e0: 3604 3504 3d04 4b00 3a00 2008 0000 0000  6.5.=.K.:. .....
+000107f0: 0600 0000 1141 6363 6f75 6e74 7320 6c6f  .....Accounts lo
+00010800: 6164 6564 3a20 0700 0000 1353 7461 7465  aded: .....State
+00010810: 6d65 6e74 4f70 656e 4272 6f6b 6572 0103  mentOpenBroker..
+00010820: 0000 0064 041e 0442 0441 0443 0442 0441  ...d...B.A.C.B.A
+00010830: 0442 0432 0443 044e 0442 0020 0434 0430  .B.2.C.N.B. .4.0
+00010840: 043d 043d 044b 0435 0020 0432 0020 043e  .=.=.K.5. .2. .>
+00010850: 043f 0438 0441 0430 043d 0438 0438 0020  .?.8.A.0.=.8.8. 
+00010860: 043f 043e 0433 0430 0448 0435 043d 0438  .?.>.3.0.H.5.=.8
+00010870: 044f 0020 043e 0431 043b 0438 0433 0430  .O. .>.1.;.8.3.0
+00010880: 0446 0438 0438 0020 0800 0000 0006 0000  .F.8.8. ........
+00010890: 002a 426f 6e64 2072 6570 6179 6d65 6e74  .*Bond repayment
+000108a0: 2064 6573 6372 6970 7469 6f6e 206d 6973   description mis
+000108b0: 7320 736f 6d65 2064 6174 6120 0700 0000  s some data ....
+000108c0: 1353 7461 7465 6d65 6e74 4f70 656e 4272  .StatementOpenBr
+000108d0: 6f6b 6572 0103 0000 0068 041d 0435 0432  oker.....h...5.2
+000108e0: 043e 0437 043c 043e 0436 043d 043e 0020  .>.7.<.>.6.=.>. 
+000108f0: 0440 0430 0441 043f 043e 0437 043d 0430  .@.0.A.?.>.7.=.0
+00010900: 0442 044c 0020 043d 0430 0437 0432 0430  .B.L. .=.0.7.2.0
+00010910: 043d 0438 0435 0020 043e 0431 043b 0438  .=.8.5. .>.1.;.8
+00010920: 0433 0430 0446 0438 0438 0020 0432 0020  .3.0.F.8.8. .2. 
+00010930: 043e 043f 0438 0441 0430 043d 0438 0438  .>.?.8.A.0.=.8.8
+00010940: 0020 0800 0000 0006 0000 0028 4361 6e27  . .........(Can'
+00010950: 7420 6465 7465 6374 2062 6f6e 6420 6e61  t detect bond na
+00010960: 6d65 2066 726f 6d20 6465 7363 7269 7074  me from descript
+00010970: 696f 6e20 0700 0000 1353 7461 7465 6d65  ion .....Stateme
+00010980: 6e74 4f70 656e 4272 6f6b 6572 0103 0000  ntOpenBroker....
+00010990: 0062 041d 0435 0432 043e 0437 043c 043e  .b...5.2.>.7.<.>
+000109a0: 0436 043d 043e 0020 043e 043f 0440 0435  .6.=.>. .>.?.@.5
+000109b0: 0434 0435 043b 0438 0442 044c 0020 0442  .4.5.;.8.B.L. .B
+000109c0: 0438 043f 002f 043a 043e 043b 0438 0447  .8.?./.:.>.;.8.G
+000109d0: 0435 0441 0442 0432 043e 0020 0434 043b  .5.A.B.2.>. .4.;
+000109e0: 044f 0020 0441 0434 0435 043b 043a 0438  .O. .A.4.5.;.:.8
+000109f0: 003a 0020 0800 0000 0006 0000 0025 4361  .:. .........%Ca
+00010a00: 6e27 7420 6465 7465 726d 696e 6520 7472  n't determine tr
+00010a10: 6164 6520 7479 7065 2f71 7561 6e74 6974  ade type/quantit
+00010a20: 793a 2007 0000 0013 5374 6174 656d 656e  y: .....Statemen
+00010a30: 744f 7065 6e42 726f 6b65 7201 0300 0000  tOpenBroker.....
+00010a40: 6804 1d04 3504 3204 3e04 3704 3c04 3e04  h...5.2.>.7.<.>.
+00010a50: 3604 3d04 3e00 2004 3e04 3f04 4004 3504  6.=.>. .>.?.@.5.
+00010a60: 3404 3504 3b04 3804 4204 4c00 2004 4104  4.5.;.8.B.L. .A.
+00010a70: 4704 5104 4200 2004 3404 3b04 4f00 2004  G.Q.B. .4.;.O. .
+00010a80: 3404 3504 3d04 3504 3604 3d04 3e04 3900  4.5.=.5.6.=.>.9.
+00010a90: 2004 4204 4004 3004 3d04 3704 3004 3a04   .B.@.0.=.7.0.:.
+00010aa0: 4604 3804 3800 3a00 2008 0000 0000 0600  F.8.8.:. .......
+00010ab0: 0000 2743 616e 2774 2066 696e 6420 6163  ..'Can't find ac
+00010ac0: 636f 756e 7420 666f 7220 6361 7368 206f  count for cash o
+00010ad0: 7065 7261 7469 6f6e 3a20 0700 0000 1353  peration: .....S
+00010ae0: 7461 7465 6d65 6e74 4f70 656e 4272 6f6b  tatementOpenBrok
+00010af0: 6572 0103 0000 0044 041d 0435 0432 043e  er.....D...5.2.>
+00010b00: 0437 043c 043e 0436 043d 043e 0020 043d  .7.<.>.6.=.>. .=
+00010b10: 0430 0439 0442 0438 0020 0441 0447 0451  .0.9.B.8. .A.G.Q
+00010b20: 0442 0020 0434 043b 044f 0020 0441 0434  .B. .4.;.O. .A.4
+00010b30: 0435 043b 043a 0438 003a 0020 0800 0000  .5.;.:.8.:. ....
+00010b40: 0006 0000 001e 4361 6e27 7420 6669 6e64  ......Can't find
+00010b50: 2061 6363 6f75 6e74 2066 6f72 2074 7261   account for tra
+00010b60: 6465 3a20 0700 0000 1353 7461 7465 6d65  de: .....Stateme
+00010b70: 6e74 4f70 656e 4272 6f6b 6572 0103 0000  ntOpenBroker....
+00010b80: 0050 041d 0435 0432 043e 0437 043c 043e  .P...5.2.>.7.<.>
+00010b90: 0436 043d 043e 0020 043d 0430 0439 0442  .6.=.>. .=.0.9.B
+00010ba0: 0438 0020 0437 0430 043f 0438 0441 044c  .8. .7.0.?.8.A.L
+00010bb0: 0020 0441 043f 0438 0441 0430 043d 0438  . .A.?.8.A.0.=.8
+00010bc0: 044f 0020 0426 0411 0020 0434 043b 044f  .O. .&... .4.;.O
+00010bd0: 0020 0800 0000 0006 0000 0029 4361 6e27  . .........)Can'
+00010be0: 7420 6669 6e64 2061 7373 6574 2063 616e  t find asset can
+00010bf0: 6365 6c6c 6174 696f 6e20 7265 636f 7264  cellation record
+00010c00: 2066 6f72 2007 0000 0013 5374 6174 656d   for .....Statem
+00010c10: 656e 744f 7065 6e42 726f 6b65 7201 0300  entOpenBroker...
+00010c20: 0000 3204 1d04 3500 2004 3d04 3004 3904  ..2...5. .=.0.9.
+00010c30: 3404 3504 3d04 3000 2004 2604 1100 2004  4.5.=.0. .&... .
+00010c40: 3404 3b04 4f00 2004 3a04 4304 3f04 3e04  4.;.O. .:.C.?.>.
+00010c50: 3d04 3000 2008 0000 0000 0600 0000 2343  =.0. .........#C
+00010c60: 616e 2774 2066 696e 6420 6173 7365 7420  an't find asset 
+00010c70: 666f 7220 626f 6e64 2069 6e74 6572 6573  for bond interes
+00010c80: 7420 0700 0000 1353 7461 7465 6d65 6e74  t .....Statement
+00010c90: 4f70 656e 4272 6f6b 6572 0103 0000 003c  OpenBroker.....<
+00010ca0: 041d 0435 0432 043e 0437 043c 043e 0436  ...5.2.>.7.<.>.6
+00010cb0: 043d 043e 0020 0441 043e 043f 043e 0441  .=.>. .A.>.?.>.A
+00010cc0: 0442 0430 0432 0438 0442 044c 0020 0426  .B.0.2.8.B.L. .&
+00010cd0: 0411 0020 0434 043b 044f 0020 0800 0000  ... .4.;.O. ....
+00010ce0: 0006 0000 0016 4361 6e27 7420 6d61 7463  ......Can't matc
+00010cf0: 6820 6173 7365 7420 666f 7220 0700 0000  h asset for ....
+00010d00: 1353 7461 7465 6d65 6e74 4f70 656e 4272  .StatementOpenBr
+00010d10: 6f6b 6572 0103 0000 0066 041d 0435 0432  oker.....f...5.2
+00010d20: 043e 0437 043c 043e 0436 043d 043e 0020  .>.7.<.>.6.=.>. 
+00010d30: 0440 0430 0441 043f 043e 0437 043d 0430  .@.0.A.?.>.7.=.0
+00010d40: 0442 044c 0020 043e 043f 0438 0441 0430  .B.L. .>.?.8.A.0
+00010d50: 043d 0438 0435 0020 043f 043e 0433 0430  .=.8.5. .?.>.3.0
+00010d60: 0448 0435 043d 0438 044f 0020 043e 0431  .H.5.=.8.O. .>.1
+00010d70: 043b 0438 0433 0430 0446 0438 0438 0020  .;.8.3.0.F.8.8. 
+00010d80: 0800 0000 0006 0000 0024 4361 6e27 7420  .........$Can't 
+00010d90: 7061 7273 6520 426f 6e64 204d 6174 7572  parse Bond Matur
+00010da0: 6520 6465 7363 7269 7074 696f 6e20 0700  e description ..
+00010db0: 0000 1353 7461 7465 6d65 6e74 4f70 656e  ...StatementOpen
+00010dc0: 4272 6f6b 6572 0103 0000 004c 041d 0435  Broker.....L...5
+00010dd0: 0432 043e 0437 043c 043e 0436 043d 043e  .2.>.7.<.>.6.=.>
+00010de0: 0020 0440 0430 0441 043f 043e 0437 043d  . .@.0.A.?.>.7.=
+00010df0: 0430 0442 044c 0020 043e 043f 0438 0441  .0.B.L. .>.?.8.A
+00010e00: 0430 043d 0438 0435 0020 043a 0443 043f  .0.=.8.5. .:.C.?
+00010e10: 043e 043d 0430 0020 0800 0000 0006 0000  .>.=.0. ........
+00010e20: 0021 4361 6e27 7420 7061 7273 6520 496e  .!Can't parse In
+00010e30: 7465 7265 7374 2064 6573 6372 6970 7469  terest descripti
+00010e40: 6f6e 2007 0000 0013 5374 6174 656d 656e  on .....Statemen
+00010e50: 744f 7065 6e42 726f 6b65 7201 0300 0000  tOpenBroker.....
+00010e60: 6604 1d04 3504 3204 3e04 3704 3c04 3e04  f...5.2.>.7.<.>.
+00010e70: 3604 3d04 3e00 2004 4004 3004 4104 3f04  6.=.>. .@.0.A.?.
+00010e80: 3e04 3704 3d04 3004 4204 4c00 2004 3e04  >.7.=.0.B.L. .>.
+00010e90: 3f04 3804 4104 3004 3d04 3804 3500 2004  ?.8.A.0.=.8.5. .
+00010ea0: 3f04 3e04 3304 3004 4804 3504 3d04 3804  ?.>.3.0.H.5.=.8.
+00010eb0: 4f00 2004 3e04 3104 3b04 3804 3304 3004  O. .>.1.;.8.3.0.
+00010ec0: 4604 3804 3800 2008 0000 0000 0600 0000  F.8.8. .........
+00010ed0: 2743 616e 2774 2070 6172 7365 2062 6f6e  'Can't parse bon
+00010ee0: 6420 7265 7061 796d 656e 7420 6465 7363  d repayment desc
+00010ef0: 7269 7074 696f 6e20 0700 0000 1353 7461  ription .....Sta
+00010f00: 7465 6d65 6e74 4f70 656e 4272 6f6b 6572  tementOpenBroker
+00010f10: 0103 0000 003a 0414 0435 043d 0435 0436  .....:...5.=.5.6
+00010f20: 043d 044b 0445 0020 043e 043f 0435 0440  .=.K.E. .>.?.5.@
+00010f30: 0430 0446 0438 0439 0020 0437 0430 0433  .0.F.8.9. .7.0.3
+00010f40: 0440 0443 0436 0435 043d 043e 003a 0020  .@.C.6.5.=.>.:. 
+00010f50: 0800 0000 0006 0000 0018 4361 7368 206f  ..........Cash o
+00010f60: 7065 7261 7469 6f6e 7320 6c6f 6164 6564  perations loaded
+00010f70: 3a20 0700 0000 1353 7461 7465 6d65 6e74  : .....Statement
+00010f80: 4f70 656e 4272 6f6b 6572 0103 0000 0048  OpenBroker.....H
+00010f90: 041e 0442 0441 0443 0442 0441 0442 0432  ...B.A.C.B.A.B.2
+00010fa0: 0443 044e 0442 0020 0434 0430 043d 043d  .C.N.B. .4.0.=.=
+00010fb0: 044b 0435 0020 0432 0020 043e 043f 0438  .K.5. .2. .>.?.8
+00010fc0: 0441 0430 043d 0438 0020 043a 0443 043f  .A.0.=.8. .:.C.?
+00010fd0: 043e 043d 0430 0020 0800 0000 0006 0000  .>.=.0. ........
+00010fe0: 0024 496e 7465 7265 7374 2064 6573 6372  .$Interest descr
+00010ff0: 6970 7469 6f6e 206d 6973 7320 736f 6d65  iption miss some
+00011000: 2064 6174 6120 0700 0000 1353 7461 7465   data .....State
+00011010: 6d65 6e74 4f70 656e 4272 6f6b 6572 0103  mentOpenBroker..
+00011020: 0000 0054 0417 0430 0433 0440 0443 0437  ...T...0.3.@.C.7
+00011030: 043a 0430 0020 043e 0442 0447 0451 0442  .:.0. .>.B.G.Q.B
+00011040: 0430 0020 041e 0442 043a 0440 044b 0442  .0. ...B.:.@.K.B
+00011050: 0438 0435 0020 0431 0440 043e 043a 0435  .8.5. .1.@.>.:.5
+00011060: 0440 0020 0434 043b 044f 0020 0441 0447  .@. .4.;.O. .A.G
+00011070: 0451 0442 0430 0020 0800 0000 0006 0000  .Q.B.0. ........
+00011080: 0027 4c6f 6164 204f 7065 6e20 4272 6f6b  .'Load Open Brok
+00011090: 6572 2073 7461 7465 6d65 6e74 2066 6f72  er statement for
+000110a0: 2061 6363 6f75 6e74 2007 0000 0013 5374   account .....St
+000110b0: 6174 656d 656e 744f 7065 6e42 726f 6b65  atementOpenBroke
+000110c0: 7201 0300 0000 5604 1d04 3004 3904 3404  r.....V...0.9.4.
+000110d0: 3504 3d04 4b00 2004 3d04 3504 4104 3a04  5.=.K. .=.5.A.:.
+000110e0: 3e04 3b04 4c04 3a04 3e00 2004 3704 3004  >.;.L.:.>. .7.0.
+000110f0: 3f04 3804 4104 3504 3900 2004 3f04 3e04  ?.8.A.5.9. .?.>.
+00011100: 3304 3004 4804 3504 3d04 3804 4f00 2004  3.0.H.5.=.8.O. .
+00011110: 2604 1100 2004 3404 3b04 4f00 2008 0000  &... .4.;.O. ...
+00011120: 0000 0600 0000 264d 756c 7469 706c 6520  ......&Multiple 
+00011130: 6173 7365 7420 6361 6e63 656c 6c61 7469  asset cancellati
+00011140: 6f6e 206d 6174 6368 2066 6f72 2007 0000  on match for ...
+00011150: 0013 5374 6174 656d 656e 744f 7065 6e42  ..StatementOpenB
+00011160: 726f 6b65 7201 0300 0000 7404 1d04 3504  roker.....t...5.
+00011170: 4104 3a04 3e04 3b04 4c04 3a04 3e00 2004  A.:.>.;.L.:.>. .
+00011180: 4104 3e04 3204 3f04 3004 3404 3504 3d04  A.>.2.?.0.4.5.=.
+00011190: 3804 3900 2004 3404 3b04 4f00 2004 4104  8.9. .4.;.O. .A.
+000111a0: 3804 3c04 3204 3e04 3b04 3000 2c00 2004  8.<.2.>.;.0.,. .
+000111b0: 3804 4104 3f04 3e04 3b04 4c04 3704 4304  8.A.?.>.;.L.7.C.
+000111c0: 3504 3c04 3e04 3304 3e00 2004 3104 4004  5.<.>.3.>. .1.@.
+000111d0: 3e04 3a04 3504 4004 3e04 3c00 3a00 2008  >.:.5.@.>.<.:. .
+000111e0: 0000 0000 0600 0000 224d 756c 7469 706c  ........"Multipl
+000111f0: 6520 6d61 7463 6820 666f 7220 6272 6f6b  e match for brok
+00011200: 6572 2073 796d 626f 6c3a 2007 0000 0013  er symbol: .....
+00011210: 5374 6174 656d 656e 744f 7065 6e42 726f  StatementOpenBro
+00011220: 6b65 7201 0300 0000 4404 1d04 3504 4104  ker.....D...5.A.
+00011230: 3a04 3e04 3b04 4c04 3a04 3e00 2004 4104  :.>.;.L.:.>. .A.
+00011240: 3e04 3204 3f04 3004 3404 3504 3d04 3804  >.2.?.0.4.5.=.8.
+00011250: 3900 2004 3404 3b04 4f00 2004 4104 3804  9. .4.;.O. .A.8.
+00011260: 3c04 3204 3e04 3b04 3000 3a00 2008 0000  <.2.>.;.0.:. ...
+00011270: 0000 0600 0000 1b4d 756c 7469 706c 6520  .......Multiple 
+00011280: 6d61 7463 6820 666f 7220 7379 6d62 6f6c  match for symbol
+00011290: 3a20 0700 0000 1353 7461 7465 6d65 6e74  : .....Statement
+000112a0: 4f70 656e 4272 6f6b 6572 0103 0000 001e  OpenBroker......
+000112b0: 041e 0442 043a 0440 044b 0442 0438 0435  ...B.:.@.K.B.8.5
+000112c0: 0020 0431 0440 043e 043a 0435 0440 0800  . .1.@.>.:.5.@..
+000112d0: 0000 0006 0000 000b 4f70 656e 2042 726f  ........Open Bro
+000112e0: 6b65 7207 0000 0013 5374 6174 656d 656e  ker.....Statemen
+000112f0: 744f 7065 6e42 726f 6b65 7201 0300 0000  tOpenBroker.....
+00011300: 3c04 1e04 4204 4704 5104 4200 2004 3104  <...B.G.Q.B. .1.
+00011310: 4004 3e04 3a04 3504 4004 3000 2004 1e04  @.>.:.5.@.0. ...
+00011320: 4204 3a04 4004 4b04 4204 3804 3500 2000  B.:.@.K.B.8.5. .
+00011330: 2800 2a00 2e00 7800 6d00 6c00 2908 0000  (.*...x.m.l.)...
+00011340: 0000 0600 0000 1d4f 7065 6e20 4272 6f6b  .......Open Brok
+00011350: 6572 2073 7461 7465 6d65 6e74 2028 2a2e  er statement (*.
+00011360: 786d 6c29 0700 0000 1353 7461 7465 6d65  xml).....Stateme
+00011370: 6e74 4f70 656e 4272 6f6b 6572 0103 0000  ntOpenBroker....
+00011380: 0054 0417 0430 0433 043e 043b 043e 0432  .T...0.3.>.;.>.2
+00011390: 043e 043a 0020 043e 0442 0447 0451 0442  .>.:. .>.B.G.Q.B
+000113a0: 0430 0020 041e 0442 043a 0440 044b 0442  .0. ...B.:.@.K.B
+000113b0: 0438 0435 0020 0431 0440 043e 043a 0435  .8.5. .1.@.>.:.5
+000113c0: 0440 0020 043d 0435 0020 043d 0430 0439  .@. .=.5. .=.0.9
+000113d0: 0434 0435 043d 0800 0000 0006 0000 0022  .4.5.=........."
+000113e0: 4f70 656e 2062 726f 6b65 7220 7265 706f  Open broker repo
+000113f0: 7274 2074 6974 6c65 206e 6f74 2066 6f75  rt title not fou
+00011400: 6e64 0700 0000 1353 7461 7465 6d65 6e74  nd.....Statement
+00011410: 4f70 656e 4272 6f6b 6572 0103 0000 0038  OpenBroker.....8
+00011420: 041e 043f 0435 0440 0430 0446 0438 044f  ...?.5.@.0.F.8.O
+00011430: 0020 043d 0435 0020 043f 043e 0434 0434  . .=.5. .?.>.4.4
+00011440: 0435 0440 0436 0438 0432 0430 0435 0442  .5.@.6.8.2.0.5.B
+00011450: 0441 044f 003a 0020 0800 0000 0006 0000  .A.O.:. ........
+00011460: 0019 4f70 6572 6174 696f 6e20 6e6f 7420  ..Operation not 
+00011470: 7375 7070 6f72 7465 643a 2007 0000 0013  supported: .....
+00011480: 5374 6174 656d 656e 744f 7065 6e42 726f  StatementOpenBro
+00011490: 6b65 7201 0300 0000 1c04 2604 1100 2004  ker.......&... .
+000114a0: 3704 3004 3304 4004 4304 3604 3504 3d04  7.0.3.@.C.6.5.=.
+000114b0: 4b00 3a00 2008 0000 0000 0600 0000 1353  K.:. ..........S
+000114c0: 6563 7572 6974 6965 7320 6c6f 6164 6564  ecurities loaded
+000114d0: 3a20 0700 0000 1353 7461 7465 6d65 6e74  : .....Statement
+000114e0: 4f70 656e 4272 6f6b 6572 0103 0000 006e  OpenBroker.....n
+000114f0: 041d 0435 043f 043e 0434 0434 0435 0440  ...5.?.>.4.4.5.@
+00011500: 0436 0438 0432 0430 0435 043c 044b 0439  .6.8.2.0.5.<.K.9
+00011510: 0020 0437 0430 0433 043e 043b 043e 0432  . .7.0.3.>.;.>.2
+00011520: 043e 043a 0020 043e 0442 0447 0451 0442  .>.:. .>.B.G.Q.B
+00011530: 0430 0020 0434 043b 044f 0020 041e 0442  .0. .4.;.O. ...B
+00011540: 043a 0440 044b 0442 0438 0435 0020 0431  .:.@.K.B.8.5. .1
+00011550: 0440 043e 043a 0435 0440 003a 0020 0800  .@.>.:.5.@.:. ..
+00011560: 0000 0006 0000 0026 556e 6578 7065 6374  .......&Unexpect
+00011570: 6564 204f 7065 6e20 6272 6f6b 6572 2072  ed Open broker r
+00011580: 6570 6f72 7420 6865 6164 6572 3a20 0700  eport header: ..
+00011590: 0000 1353 7461 7465 6d65 6e74 4f70 656e  ...StatementOpen
+000115a0: 4272 6f6b 6572 0103 0000 0042 041d 0435  Broker.....B...5
+000115b0: 0438 0437 0432 0435 0441 0442 043d 0430  .8.7.2.5.A.B.=.0
+000115c0: 044f 0020 043d 0435 0442 043e 0440 0433  .O. .=.5.B.>.@.3
+000115d0: 043e 0432 0430 044f 0020 043e 043f 0435  .>.2.0.O. .>.?.5
+000115e0: 0440 0430 0446 0438 044f 003a 0020 0800  .@.0.F.8.O.:. ..
+000115f0: 0000 0006 0000 001d 556e 6b6e 6f77 6e20  ........Unknown 
+00011600: 6e6f 6e2d 7472 6164 6520 6f70 6572 6174  non-trade operat
+00011610: 696f 6e3a 2007 0000 0013 5374 6174 656d  ion: .....Statem
+00011620: 656e 744f 7065 6e42 726f 6b65 7201 0300  entOpenBroker...
+00011630: 0000 4604 1d04 3504 3f04 3e04 3404 3404  ..F...5.?.>.4.4.
+00011640: 3504 4004 3604 3804 3204 3004 3504 3c04  5.@.6.8.2.0.5.<.
+00011650: 3e04 3500 2004 3e04 3f04 3804 4104 3004  >.5. .>.?.8.A.0.
+00011660: 3d04 3804 3500 2004 3f04 3b04 3004 4204  =.8.5. .?.;.0.B.
+00011670: 3504 3604 3000 3a00 2008 0000 0000 0600  5.6.0.:. .......
+00011680: 0000 1d55 6e6b 6e6f 776e 2070 6179 6d65  ...Unknown payme
+00011690: 6e74 2064 6573 6372 6970 7469 6f6e 3a20  nt description: 
+000116a0: 0700 0000 1353 7461 7465 6d65 6e74 4f70  .....StatementOp
+000116b0: 656e 4272 6f6b 6572 0103 0000 0032 041d  enBroker.....2..
+000116c0: 0435 0438 0437 0432 0435 0441 0442 043d  .5.8.7.2.5.A.B.=
+000116d0: 044b 0439 0020 0442 0438 043f 0020 043f  .K.9. .B.8.?. .?
+000116e0: 043b 0430 0442 0435 0436 0430 003a 0020  .;.0.B.5.6.0.:. 
+000116f0: 0800 0000 0006 0000 0016 556e 6b6e 6f77  ..........Unknow
+00011700: 6e20 7061 796d 656e 7420 7479 7065 3a20  n payment type: 
+00011710: 0700 0000 1353 7461 7465 6d65 6e74 4f70  .....StatementOp
+00011720: 656e 4272 6f6b 6572 0103 0000 0016 0426  enBroker.......&
+00011730: 0411 0020 0431 0435 0437 0020 0069 0064  ... .1.5.7. .i.d
+00011740: 003a 0020 0800 0000 0006 0000 0012 4173  .:. ..........As
+00011750: 7365 7420 7769 7468 6f75 7420 6964 3a20  set without id: 
+00011760: 0700 0000 1653 7461 7465 6d65 6e74 4f70  .....StatementOp
+00011770: 656e 506f 7274 666f 6c69 6f01 0300 0000  enPortfolio.....
+00011780: 4804 1d04 3504 3204 3e04 3704 3c04 3e04  H...5.2.>.7.<.>.
+00011790: 3604 3d04 3e00 2004 3f04 4004 3e04 4704  6.=.>. .?.@.>.G.
+000117a0: 3804 4204 3004 4204 4c00 2000 4a00 5300  8.B.0.B.L. .J.S.
+000117b0: 4f00 4e00 2004 3804 3700 2004 4404 3004  O.N. .8.7. .D.0.
+000117c0: 3904 3b04 3000 3a00 2008 0000 0000 0600  9.;.0.:. .......
+000117d0: 0000 1f46 6169 6c65 6420 746f 2072 6561  ...Failed to rea
+000117e0: 6420 4a53 4f4e 2066 726f 6d20 6669 6c65  d JSON from file
+000117f0: 3a20 0700 0000 1653 7461 7465 6d65 6e74  : .....Statement
+00011800: 4f70 656e 506f 7274 666f 6c69 6f01 0300  OpenPortfolio...
+00011810: 0000 3404 1d04 3504 3204 3e04 3704 3c04  ..4...5.2.>.7.<.
+00011820: 3e04 3604 3d04 3e00 2004 3f04 4004 3e04  >.6.=.>. .?.@.>.
+00011830: 4704 3504 4104 4204 4c00 2004 4404 3004  G.5.A.B.L. .D.0.
+00011840: 3904 3b00 3a00 2008 0000 0000 0600 0000  9.;.:. .........
+00011850: 1546 6169 6c65 6420 746f 2072 6561 6420  .Failed to read 
+00011860: 6669 6c65 3a20 0700 0000 1653 7461 7465  file: .....State
+00011870: 6d65 6e74 4f70 656e 506f 7274 666f 6c69  mentOpenPortfoli
+00011880: 6f01 0300 0000 2204 1804 3c04 3f04 3e04  o....."...<.?.>.
+00011890: 4004 4204 3804 4004 3e04 3204 3004 3d04  @.B.8.@.>.2.0.=.
+000118a0: 3d04 4b04 3900 2021 1608 0000 0000 0600  =.K.9. !........
+000118b0: 0000 0a49 6d70 6f72 7465 6420 2307 0000  ...Imported #...
+000118c0: 0016 5374 6174 656d 656e 744f 7065 6e50  ..StatementOpenP
+000118d0: 6f72 7466 6f6c 696f 0103 0000 002e 0049  ortfolio.......I
+000118e0: 006e 0076 0065 0073 0074 0062 006f 006f  .n.v.e.s.t.b.o.o
+000118f0: 006b 0020 002f 0020 0049 005a 0049 002d  .k. ./. .I.Z.I.-
+00011900: 0069 006e 0076 0065 0073 0074 0800 0000  .i.n.v.e.s.t....
+00011910: 0006 0000 0017 496e 7665 7374 626f 6f6b  ......Investbook
+00011920: 202f 2049 5a49 2d49 6e76 6573 7407 0000   / IZI-Invest...
+00011930: 0016 5374 6174 656d 656e 744f 7065 6e50  ..StatementOpenP
+00011940: 6f72 7466 6f6c 696f 0103 0000 0042 041e  ortfolio.....B..
+00011950: 0431 044f 0437 0430 0442 0435 043b 044c  .1.O.7.0.B.5.;.L
+00011960: 043d 0430 044f 0020 0441 0435 043a 0446  .=.0.O. .A.5.:.F
+00011970: 0438 044f 0020 043e 0442 0441 0443 0442  .8.O. .>.B.A.C.B
+00011980: 0441 0442 0432 0443 0435 0442 003a 0020  .A.B.2.C.5.B.:. 
+00011990: 0800 0000 0006 0000 001e 4d61 6e64 6174  ..........Mandat
+000119a0: 6f72 7920 7365 6374 696f 6e20 6973 206d  ory section is m
+000119b0: 6973 7369 6e67 3a20 0700 0000 1653 7461  issing: .....Sta
+000119c0: 7465 6d65 6e74 4f70 656e 506f 7274 666f  tementOpenPortfo
+000119d0: 6c69 6f01 0300 0000 2e00 4f00 7000 6500  lio.......O.p.e.
+000119e0: 6e00 2000 7000 6f00 7200 7400 6600 6f00  n. .p.o.r.t.f.o.
+000119f0: 6c00 6900 6f00 2000 2800 2a00 2e00 6a00  l.i.o. .(.*...j.
+00011a00: 7300 6f00 6e00 2908 0000 0000 0600 0000  s.o.n.).........
+00011a10: 174f 7065 6e20 706f 7274 666f 6c69 6f20  .Open portfolio 
+00011a20: 282a 2e6a 736f 6e29 0700 0000 1653 7461  (*.json).....Sta
+00011a30: 7465 6d65 6e74 4f70 656e 506f 7274 666f  tementOpenPortfo
+00011a40: 6c69 6f01 0300 0000 4e04 1d04 3504 3f04  lio.....N...5.?.
+00011a50: 3e04 3404 3404 3504 4004 3604 3804 3204  >.4.4.5.@.6.8.2.
+00011a60: 3004 3504 3c04 3004 4f00 2004 3204 3504  0.5.<.0.O. .2.5.
+00011a70: 4004 4104 3804 4f00 2004 4404 3e04 4004  @.A.8.O. .D.>.@.
+00011a80: 3c04 3004 4204 3000 2004 4404 3004 3904  <.0.B.0. .D.0.9.
+00011a90: 3b04 3000 3a00 2008 0000 0000 0600 0000  ;.0.:. .........
+00011aa0: 2e55 6e73 7570 706f 7274 6564 2076 6572  .Unsupported ver
+00011ab0: 7369 6f6e 206f 6620 6f70 656e 2070 6f72  sion of open por
+00011ac0: 7466 6f6c 696f 2066 6f72 6d61 743a 2007  tfolio format: .
+00011ad0: 0000 0016 5374 6174 656d 656e 744f 7065  ....StatementOpe
+00011ae0: 6e50 6f72 7466 6f6c 696f 0103 0000 0038  nPortfolio.....8
+00011af0: 041a 0443 043f 043e 043d 044b 0020 043e  ...C.?.>.=.K. .>
+00011b00: 0431 043b 0438 0433 0430 0446 0438 0439  .1.;.8.3.0.F.8.9
+00011b10: 0020 0437 0430 0433 0440 0443 0436 0435  . .7.0.3.@.C.6.5
+00011b20: 043d 044b 003a 0020 0800 0000 0006 0000  .=.K.:. ........
+00011b30: 0017 426f 6e64 2069 6e74 6572 6573 7473  ..Bond interests
+00011b40: 206c 6f61 6465 643a 2007 0000 000c 5374   loaded: .....St
+00011b50: 6174 656d 656e 7450 5342 0103 0000 003e  atementPSB.....>
+00011b60: 0414 0435 043d 0435 0436 043d 044b 0435  ...5.=.5.6.=.K.5
+00011b70: 0020 0442 0440 0430 043d 0437 0430 043a  . .B.@.0.=.7.0.:
+00011b80: 0446 0438 0438 0020 0437 0430 0433 0440  .F.8.8. .7.0.3.@
+00011b90: 0443 0436 0435 043d 044b 003a 0020 0800  .C.6.5.=.K.:. ..
+00011ba0: 0000 0006 0000 001a 4361 7368 2074 7261  ........Cash tra
+00011bb0: 6e73 6163 7469 6f6e 7320 6c6f 6164 6564  nsactions loaded
+00011bc0: 3a20 0700 0000 0c53 7461 7465 6d65 6e74  : .....Statement
+00011bd0: 5053 4201 0300 0000 2a04 1404 3804 3204  PSB.....*...8.2.
+00011be0: 3804 3404 3504 3d04 3404 4b00 2004 3704  8.4.5.=.4.K. .7.
+00011bf0: 3004 3304 4004 4304 3604 3504 3d04 4b00  0.3.@.C.6.5.=.K.
+00011c00: 3a00 2008 0000 0000 0600 0000 1244 6976  :. ..........Div
+00011c10: 6964 656e 6473 206c 6f61 6465 643a 2007  idends loaded: .
+00011c20: 0000 000c 5374 6174 656d 656e 7450 5342  ....StatementPSB
+00011c30: 0103 0000 0014 041f 0421 0411 002d 0431  .........!...-.1
+00011c40: 0440 043e 043a 0435 0440 0800 0000 0006  .@.>.:.5.@......
+00011c50: 0000 000a 5053 4220 4272 6f6b 6572 0700  ....PSB Broker..
+00011c60: 0000 0c53 7461 7465 6d65 6e74 5053 4201  ...StatementPSB.
+00011c70: 0300 0000 4004 1e04 4204 4704 5104 4200  ....@...B.G.Q.B.
+00011c80: 2004 3104 4004 3e04 3a04 3504 4004 3000   .1.@.>.:.5.@.0.
+00011c90: 2004 1f04 2104 1100 2000 2800 2a00 2e00   ...!... .(.*...
+00011ca0: 7800 6c00 7300 7800 2000 2a00 2e00 7800  x.l.s.x. .*...x.
+00011cb0: 6c00 7300 2908 0000 0000 0600 0000 2350  l.s.).........#P
+00011cc0: 5342 2062 726f 6b65 7220 7374 6174 656d  SB broker statem
+00011cd0: 656e 7420 282a 2e78 6c73 7820 2a2e 786c  ent (*.xlsx *.xl
+00011ce0: 7329 0700 0000 0c53 7461 7465 6d65 6e74  s).....Statement
+00011cf0: 5053 4201 03ff ffff ff08 0000 0000 0600  PSB.............
+00011d00: 0000 0f54 7261 6465 7320 6c6f 6164 6564  ...Trades loaded
+00011d10: 3a20 0700 0000 0c53 7461 7465 6d65 6e74  : .....Statement
+00011d20: 5053 4201 0300 0000 4004 1d04 3504 3f04  PSB.....@...5.?.
+00011d30: 3e04 3404 3404 3504 4004 3604 3804 3204  >.4.4.5.@.6.8.2.
+00011d40: 3004 3504 3c04 3004 4f00 2004 3e04 3f04  0.5.<.0.O. .>.?.
+00011d50: 3504 4004 3004 4604 3804 4f00 2004 4100  5.@.0.F.8.O. .A.
+00011d60: 2004 1404 2100 3a00 2008 0000 0000 0600   ...!.:. .......
+00011d70: 0000 1855 6e6b 6e6f 776e 2063 6173 6820  ...Unknown cash 
+00011d80: 6f70 6572 6174 696f 6e3a 2007 0000 000c  operation: .....
+00011d90: 5374 6174 656d 656e 7450 5342 0103 0000  StatementPSB....
+00011da0: 003a 041d 0435 0438 0437 0432 0435 0441  .:...5.8.7.2.5.A
+00011db0: 0442 043d 044b 0439 0020 0442 0438 043f  .B.=.K.9. .B.8.?
+00011dc0: 0020 0434 0432 0438 0436 0435 043d 0438  . .4.2.8.6.5.=.8
+00011dd0: 044f 0020 0414 0421 003a 0020 0800 0000  .O. ...!.:. ....
+00011de0: 0006 0000 001a 556e 6b6e 6f77 6e20 6361  ......Unknown ca
+00011df0: 7368 2074 7261 6e73 6163 7469 6f6e 3a20  sh transaction: 
+00011e00: 0700 0000 0c53 7461 7465 6d65 6e74 5053  .....StatementPS
+00011e10: 4201 0300 0000 3004 1d04 3504 3804 3704  B.....0...5.8.7.
+00011e20: 3204 3504 4104 4204 3d04 4b04 3900 2004  2.5.A.B.=.K.9. .
+00011e30: 4204 3804 3f00 2004 4104 3404 3504 3b04  B.8.?. .A.4.5.;.
+00011e40: 3a04 3800 3a00 2008 0000 0000 0600 0000  :.8.:. .........
+00011e50: 1455 6e6b 6e6f 776e 2074 7261 6465 2074  .Unknown trade t
+00011e60: 7970 653a 2007 0000 000c 5374 6174 656d  ype: .....Statem
+00011e70: 656e 7450 5342 0103 0000 0032 041d 0435  entPSB.....2...5
+00011e80: 043f 043e 0434 0434 0435 0440 0436 0438  .?.>.4.4.5.@.6.8
+00011e90: 0432 0430 0435 043c 044b 0439 0020 043f  .2.0.5.<.K.9. .?
+00011ea0: 043b 0430 0442 0451 0436 003a 0020 0800  .;.0.B.Q.6.:. ..
+00011eb0: 0000 0006 0000 0015 556e 7375 7070 6f72  ........Unsuppor
+00011ec0: 7465 6420 7061 796d 656e 743a 2007 0000  ted payment: ...
+00011ed0: 000c 5374 6174 656d 656e 7450 5342 0103  ..StatementPSB..
+00011ee0: 0000 005a 0421 0434 0435 043b 043a 0430  ...Z.!.4.5.;.:.0
+00011ef0: 0020 0441 0020 0440 0430 0437 043d 044b  . .A. .@.0.7.=.K
+00011f00: 043c 0438 0020 0432 0430 043b 044e 0442  .<.8. .2.0.;.N.B
+00011f10: 0430 043c 0438 0020 043d 0435 0020 043f  .0.<.8. .=.5. .?
+00011f20: 043e 0434 0434 0435 0440 0436 0438 0432  .>.4.4.5.@.6.8.2
+00011f30: 0430 0435 0442 0441 044f 003a 0020 0800  .0.5.B.A.O.:. ..
+00011f40: 0000 0006 0000 002d 556e 7375 7070 6f72  .......-Unsuppor
+00011f50: 7465 6420 7472 6164 6520 7769 7468 2064  ted trade with d
+00011f60: 6966 6665 7265 6e74 2063 7572 7265 6e63  ifferent currenc
+00011f70: 6965 733a 2007 0000 000c 5374 6174 656d  ies: .....Statem
+00011f80: 656e 7450 5342 0103 0000 0032 041e 043f  entPSB.....2...?
+00011f90: 0435 0440 0430 0446 0438 0438 0020 0441  .5.@.0.F.8.8. .A
+00011fa0: 0020 0426 0411 0020 0437 0430 0433 0440  . .&... .7.0.3.@
+00011fb0: 0443 0436 0435 043d 044b 003a 0020 0800  .C.6.5.=.K.:. ..
+00011fc0: 0000 0006 0000 0019 4173 7365 7420 6f70  ........Asset op
+00011fd0: 6572 6174 696f 6e73 206c 6f61 6465 643a  erations loaded:
+00011fe0: 2007 0000 000d 5374 6174 656d 656e 7455   .....StatementU
+00011ff0: 4b46 5501 0300 0000 6804 1e04 4204 4104  KFU.....h...B.A.
+00012000: 4304 4204 4104 4204 3204 4304 4e04 4200  C.B.A.B.2.C.N.B.
+00012010: 2004 3e04 3604 3804 3404 3004 3504 3c04   .>.6.8.4.0.5.<.
+00012020: 4b04 3500 2004 3404 3004 3d04 3d04 4b04  K.5. .4.0.=.=.K.
+00012030: 3500 2004 3200 2004 3e04 3f04 3804 4104  5. .2. .>.?.8.A.
+00012040: 3004 3d04 3804 3800 2004 3f04 3504 4004  0.=.8.8. .?.5.@.
+00012050: 3504 3204 3e04 3404 3000 2004 2604 1100  5.2.>.4.0. .&...
+00012060: 2008 0000 0000 0600 0000 2a41 7373 6574   .........*Asset
+00012070: 2074 7261 6e73 6665 7220 6465 7363 7269   transfer descri
+00012080: 7074 696f 6e20 6d69 7373 2073 6f6d 6520  ption miss some 
+00012090: 6461 7461 2007 0000 000d 5374 6174 656d  data .....Statem
+000120a0: 656e 7455 4b46 5501 0300 0000 5004 1d04  entUKFU.....P...
+000120b0: 3504 3204 3e04 3704 3c04 3e04 3604 3d04  5.2.>.7.<.>.6.=.
+000120c0: 3e00 2004 3d04 3004 3904 4204 3800 2004  >. .=.0.9.B.8. .
+000120d0: 3704 3004 3f04 3804 4104 4c00 2004 4104  7.0.?.8.A.L. .A.
+000120e0: 3f04 3804 4104 3004 3d04 3804 4f00 2004  ?.8.A.0.=.8.O. .
+000120f0: 2604 1100 2004 3404 3b04 4f00 2008 0000  &... .4.;.O. ...
+00012100: 0000 0600 0000 2943 616e 2774 2066 696e  ......)Can't fin
+00012110: 6420 6173 7365 7420 6361 6e63 656c 6c61  d asset cancella
+00012120: 7469 6f6e 2072 6563 6f72 6420 666f 7220  tion record for 
+00012130: 0700 0000 0d53 7461 7465 6d65 6e74 554b  .....StatementUK
+00012140: 4655 0103 0000 0046 041d 0435 0432 043e  FU.....F...5.2.>
+00012150: 0437 043c 043e 0436 043d 043e 0020 043d  .7.<.>.6.=.>. .=
+00012160: 0430 0439 0442 0438 0020 0437 0430 0433  .0.9.B.8. .7.0.3
+00012170: 043e 043b 043e 0432 043e 043a 0020 043a  .>.;.>.2.>.:. .:
+00012180: 043e 043c 0438 0441 0441 0438 0439 0800  .>.<.8.A.A.8.9..
+00012190: 0000 0006 0000 001d 4361 6e27 7420 6765  ........Can't ge
+000121a0: 7420 6865 6164 6572 2074 6f20 6669 6e64  t header to find
+000121b0: 2066 6565 7307 0000 000d 5374 6174 656d   fees.....Statem
+000121c0: 656e 7455 4b46 5501 0300 0000 5604 1d04  entUKFU.....V...
+000121d0: 3504 3204 3e04 3704 3c04 3e04 3604 3d04  5.2.>.7.<.>.6.=.
+000121e0: 3e00 2004 4004 3004 4104 3f04 3e04 3704  >. .@.0.A.?.>.7.
+000121f0: 3d04 3004 4204 4c00 2004 3e04 3f04 3804  =.0.B.L. .>.?.8.
+00012200: 4104 3004 3d04 3804 3500 2004 3f04 3504  A.0.=.8.5. .?.5.
+00012210: 4004 3504 3204 3e04 3404 3000 2004 2604  @.5.2.>.4.0. .&.
+00012220: 1100 2008 0000 0000 0600 0000 2743 616e  .. .........'Can
+00012230: 2774 2070 6172 7365 2061 7373 6574 2074  't parse asset t
+00012240: 7261 6e73 6665 7220 6465 7363 7269 7074  ransfer descript
+00012250: 696f 6e20 0700 0000 0d53 7461 7465 6d65  ion .....Stateme
+00012260: 6e74 554b 4655 0103 0000 004c 041d 0435  ntUKFU.....L...5
+00012270: 0432 043e 0437 043c 043e 0436 043d 043e  .2.>.7.<.>.6.=.>
+00012280: 0020 0440 0430 0441 043f 043e 0437 043d  . .@.0.A.?.>.7.=
+00012290: 0430 0442 044c 0020 043e 043f 0438 0441  .0.B.L. .>.?.8.A
+000122a0: 0430 043d 0438 0435 0020 043a 0443 043f  .0.=.8.5. .:.C.?
+000122b0: 043e 043d 0430 0020 0800 0000 0006 0000  .>.=.0. ........
+000122c0: 0026 4361 6e27 7420 7061 7273 6520 626f  .&Can't parse bo
+000122d0: 6e64 2069 6e74 6572 6573 7420 6465 7363  nd interest desc
+000122e0: 7269 7074 696f 6e20 0700 0000 0d53 7461  ription .....Sta
+000122f0: 7465 6d65 6e74 554b 4655 0103 0000 0066  tementUKFU.....f
+00012300: 041d 0435 0432 043e 0437 043c 043e 0436  ...5.2.>.7.<.>.6
+00012310: 043d 043e 0020 0440 0430 0441 043f 043e  .=.>. .@.0.A.?.>
+00012320: 0437 043d 0430 0442 044c 0020 043e 043f  .7.=.0.B.L. .>.?
+00012330: 0438 0441 0430 043d 0438 0435 0020 043f  .8.A.0.=.8.5. .?
+00012340: 043e 0433 0430 0448 0435 043d 0438 044f  .>.3.0.H.5.=.8.O
+00012350: 0020 043e 0431 043b 0438 0433 0430 0446  . .>.1.;.8.3.0.F
+00012360: 0438 0438 0020 0800 0000 0006 0000 0027  .8.8. .........'
+00012370: 4361 6e27 7420 7061 7273 6520 626f 6e64  Can't parse bond
+00012380: 2072 6570 6179 6d65 6e74 2064 6573 6372   repayment descr
+00012390: 6970 7469 6f6e 2007 0000 000d 5374 6174  iption .....Stat
+000123a0: 656d 656e 7455 4b46 5501 0300 0000 5204  ementUKFU.....R.
+000123b0: 1d04 3504 3204 3e04 3704 3c04 3e04 3604  ..5.2.>.7.<.>.6.
+000123c0: 3d04 3e00 2004 4004 3004 4104 3f04 3e04  =.>. .@.0.A.?.>.
+000123d0: 3704 3d04 3004 4204 4c00 2004 3e04 3f04  7.=.0.B.L. .>.?.
+000123e0: 3804 4104 3004 3d04 3804 3500 2004 3404  8.A.0.=.8.5. .4.
+000123f0: 3804 3204 3804 3404 3504 3d04 3404 3000  8.2.8.4.5.=.4.0.
+00012400: 2008 0000 0000 0600 0000 2143 616e 2774   .........!Can't
+00012410: 2070 6172 7365 2064 6976 6964 656e 6420   parse dividend 
+00012420: 6465 7363 7269 7074 696f 6e20 0700 0000  description ....
+00012430: 0d53 7461 7465 6d65 6e74 554b 4655 0103  .StatementUKFU..
+00012440: 0000 0064 041d 0435 0432 043e 0437 043c  ...d...5.2.>.7.<
+00012450: 043e 0436 043d 043e 0020 0440 0430 0441  .>.6.=.>. .@.0.A
+00012460: 043f 043e 0437 043d 0430 0442 044c 0020  .?.>.7.=.0.B.L. 
+00012470: 043e 043f 0438 0441 0430 043d 0438 0435  .>.?.8.A.0.=.8.5
+00012480: 0020 0434 0435 043d 0435 0436 043d 043e  . .4.5.=.5.6.=.>
+00012490: 0433 043e 0020 043f 0435 0440 0435 0432  .3.>. .?.5.@.5.2
+000124a0: 043e 0434 0430 0020 0800 0000 0006 0000  .>.4.0. ........
+000124b0: 0027 4361 6e27 7420 7061 7273 6520 6d6f  .'Can't parse mo
+000124c0: 6e65 7920 7472 616e 7366 6572 2064 6573  ney transfer des
+000124d0: 6372 6970 7469 6f6e 2007 0000 000d 5374  cription .....St
+000124e0: 6174 656d 656e 7455 4b46 5501 0300 0000  atementUKFU.....
+000124f0: 3a04 1404 3504 3d04 3504 3604 3d04 4b04  :...5.=.5.6.=.K.
+00012500: 4500 2004 3e04 3f04 3504 4004 3004 4604  E. .>.?.5.@.0.F.
+00012510: 3804 3900 2004 3704 3004 3304 4004 4304  8.9. .7.0.3.@.C.
+00012520: 3604 3504 3d04 3e00 3a00 2008 0000 0000  6.5.=.>.:. .....
+00012530: 0600 0000 1843 6173 6820 6f70 6572 6174  .....Cash operat
+00012540: 696f 6e73 206c 6f61 6465 643a 2007 0000  ions loaded: ...
+00012550: 000d 5374 6174 656d 656e 7455 4b46 5501  ..StatementUKFU.
+00012560: 0300 0000 4804 1e04 4804 3804 3104 3a04  ....H...H.8.1.:.
+00012570: 3000 2004 3f04 4004 3800 2004 3a04 3e04  0. .?.@.8. .:.>.
+00012580: 3d04 3204 3504 4004 4204 3004 4604 3804  =.2.5.@.B.0.F.8.
+00012590: 3800 2004 4104 4304 3c04 3c04 4b00 2004  8. .A.C.<.<.K. .
+000125a0: 3d04 3004 3b04 3e04 3304 3000 2008 0000  =.0.;.>.3.0. ...
+000125b0: 0000 0600 0000 1f46 6169 6c65 6420 746f  .......Failed to
+000125c0: 2063 6f6e 7665 7274 2064 6976 6964 656e   convert dividen
+000125d0: 6420 7461 7820 0700 0000 0d53 7461 7465  d tax .....State
+000125e0: 6d65 6e74 554b 4655 0103 0000 003e 0421  mentUKFU.....>.!
+000125f0: 0434 0435 043b 043e 043a 0020 0441 0020  .4.5.;.>.:. .A. 
+00012600: 0444 044c 044e 0447 0435 0440 0441 0430  .D.L.N.G.5.@.A.0
+00012610: 043c 0438 0020 0437 0430 0433 0440 0443  .<.8. .7.0.3.@.C
+00012620: 0436 0435 043d 043e 003a 0020 0800 0000  .6.5.=.>.:. ....
+00012630: 0006 0000 0017 4675 7475 7265 7320 7472  ......Futures tr
+00012640: 6164 6573 206c 6f61 6465 643a 2007 0000  ades loaded: ...
+00012650: 000d 5374 6174 656d 656e 7455 4b46 5501  ..StatementUKFU.
+00012660: 0300 0000 7604 1e04 4204 4104 4304 4204  ....v...B.A.C.B.
+00012670: 4104 4204 3204 4304 4e04 4200 2004 3e04  A.B.2.C.N.B. .>.
+00012680: 3604 3804 3404 3004 3504 3c04 4b04 3500  6.8.4.0.5.<.K.5.
+00012690: 2004 3404 3004 3d04 3d04 4b04 3500 2004   .4.0.=.=.K.5. .
+000126a0: 3200 2004 3e04 3f04 3804 4104 3004 3d04  2. .>.?.8.A.0.=.
+000126b0: 3804 3800 2004 3404 3504 3d04 3504 3604  8.8. .4.5.=.5.6.
+000126c0: 3d04 3e04 3304 3e00 2004 3f04 3504 4004  =.>.3.>. .?.5.@.
+000126d0: 3504 3204 3e04 3404 3000 2008 0000 0000  5.2.>.4.0. .....
+000126e0: 0600 0000 2a4d 6f6e 6579 2074 7261 6e73  ....*Money trans
+000126f0: 6665 7220 6465 7363 7269 7074 696f 6e20  fer description 
+00012700: 6d69 7373 2073 6f6d 6520 6461 7461 2007  miss some data .
+00012710: 0000 000d 5374 6174 656d 656e 7455 4b46  ....StatementUKF
+00012720: 5501 0300 0000 5604 1d04 3004 3904 3404  U.....V...0.9.4.
+00012730: 3504 3d04 4b00 2004 3d04 3504 4104 3a04  5.=.K. .=.5.A.:.
+00012740: 3e04 3b04 4c04 3a04 3e00 2004 3704 3004  >.;.L.:.>. .7.0.
+00012750: 3f04 3804 4104 3504 3900 2004 3f04 3e04  ?.8.A.5.9. .?.>.
+00012760: 3304 3004 4804 3504 3d04 3804 4f00 2004  3.0.H.5.=.8.O. .
+00012770: 2604 1100 2004 3404 3b04 4f00 2008 0000  &... .4.;.O. ...
+00012780: 0000 0600 0000 264d 756c 7469 706c 6520  ......&Multiple 
+00012790: 6173 7365 7420 6361 6e63 656c 6c61 7469  asset cancellati
+000127a0: 6f6e 206d 6174 6368 2066 6f72 2007 0000  on match for ...
+000127b0: 000d 5374 6174 656d 656e 7455 4b46 5501  ..StatementUKFU.
+000127c0: 0300 0000 2404 2104 3404 3504 3b04 3e04  ....$.!.4.5.;.>.
+000127d0: 3a00 2004 3704 3004 3304 4004 4304 3604  :. .7.0.3.@.C.6.
+000127e0: 3504 3d04 3e00 3a00 2008 0000 0000 0600  5.=.>.:. .......
+000127f0: 0000 0f54 7261 6465 7320 6c6f 6164 6564  ...Trades loaded
+00012800: 3a20 0700 0000 0d53 7461 7465 6d65 6e74  : .....Statement
+00012810: 554b 4655 0103 0000 0030 041d 0435 0438  UKFU.....0...5.8
+00012820: 0437 0432 0435 0441 0442 043d 044b 0439  .7.2.5.A.B.=.K.9
+00012830: 0020 0442 0438 043f 0020 0441 0434 0435  . .B.8.?. .A.4.5
+00012840: 043b 043a 0438 003a 0020 0800 0000 0006  .;.:.8.:. ......
+00012850: 0000 0014 556e 6b6e 6f77 6e20 7472 6164  ....Unknown trad
+00012860: 6520 7479 7065 3a20 0700 0000 0d53 7461  e type: .....Sta
+00012870: 7465 6d65 6e74 554b 4655 0103 0000 003e  tementUKFU.....>
+00012880: 041d 0435 043f 043e 0434 0434 0435 0440  ...5.?.>.4.4.5.@
+00012890: 0436 0438 0432 0430 0435 043c 0430 044f  .6.8.2.0.5.<.0.O
+000128a0: 0020 043e 043f 0435 0440 0430 0446 0438  . .>.?.5.@.0.F.8
+000128b0: 044f 0020 0441 0020 0426 0411 0020 0800  .O. .A. .&... ..
+000128c0: 0000 0006 0000 001d 556e 7375 7070 706f  ........Unsupppo
+000128d0: 7274 6564 2061 7373 6574 206f 7065 7261  rted asset opera
+000128e0: 7469 6f6e 2007 0000 000d 5374 6174 656d  tion .....Statem
+000128f0: 656e 7455 4b46 5501 0300 0000 4a04 1d04  entUKFU.....J...
+00012900: 3504 3f04 3e04 3404 3404 3504 4004 3604  5.?.>.4.4.5.@.6.
+00012910: 3804 3204 3004 3504 3c04 3004 4f00 2004  8.2.0.5.<.0.O. .
+00012920: 3404 3504 3d04 3504 3604 3d04 3004 4f00  4.5.=.5.6.=.0.O.
+00012930: 2004 4204 4004 3004 3d04 3704 3004 3a04   .B.@.0.=.7.0.:.
+00012940: 4604 3804 4f00 2008 0000 0000 0600 0000  F.8.O. .........
+00012950: 1e55 6e73 7570 7070 6f72 7465 6420 6361  .Unsuppported ca
+00012960: 7368 2074 7261 6e73 6163 7469 6f6e 2007  sh transaction .
+00012970: 0000 000d 5374 6174 656d 656e 7455 4b46  ....StatementUKF
+00012980: 5501 0300 0000 1e04 2304 4004 3004 3b04  U.......#.@.0.;.
+00012990: 4104 3804 3100 2004 1a04 4d04 3f04 3804  A.8.1. ...M.?.8.
+000129a0: 4204 3004 3b08 0000 0000 0600 0000 0e55  B.0.;..........U
+000129b0: 7261 6c73 6962 2042 726f 6b65 7207 0000  ralsib Broker...
+000129c0: 000d 5374 6174 656d 656e 7455 4b46 5501  ..StatementUKFU.
+000129d0: 0300 0000 4a04 1e04 4204 4704 5104 4200  ....J...B.G.Q.B.
+000129e0: 2004 3104 4004 3e04 3a04 3504 4004 3000   .1.@.>.:.5.@.0.
+000129f0: 2004 2304 4004 3004 3b04 4104 3804 3100   .#.@.0.;.A.8.1.
+00012a00: 2004 1a04 4d04 3f04 3804 4204 3004 3b00   ...M.?.8.B.0.;.
+00012a10: 2000 2800 2a00 2e00 7a00 6900 7000 2908   .(.*...z.i.p.).
+00012a20: 0000 0000 0600 0000 1955 7261 6c73 6962  .........Uralsib
+00012a30: 2073 7461 7465 6d65 6e74 2028 2a2e 7a69   statement (*.zi
+00012a40: 7029 0700 0000 0d53 7461 7465 6d65 6e74  p).....Statement
+00012a50: 554b 4655 0103 0000 003e 0410 0440 0445  UKFU.....>...@.E
+00012a60: 0438 0432 0020 0441 043e 0434 0435 0440  .8.2. .A.>.4.5.@
+00012a70: 0436 0438 0442 0020 043d 0435 0441 043a  .6.8.B. .=.5.A.:
+00012a80: 043e 043b 044c 043a 043e 0020 0444 0430  .>.;.L.:.>. .D.0
+00012a90: 0439 043b 043e 0432 0800 0000 0006 0000  .9.;.>.2........
+00012aa0: 001f 4172 6368 6976 6520 636f 6e74 6169  ..Archive contai
+00012ab0: 6e73 206d 756c 7469 706c 6520 6669 6c65  ns multiple file
+00012ac0: 7307 0000 000c 5374 6174 656d 656e 7458  s.....StatementX
+00012ad0: 4c53 0103 0000 005a 041d 0435 0020 0443  LS.....Z...5. .C
+00012ae0: 0434 0430 043b 043e 0441 044c 0020 043d  .4.0.;.>.A.L. .=
+00012af0: 0430 0439 0442 0438 0020 043e 0436 0438  .0.9.B.8. .>.6.8
+00012b00: 0434 0430 0435 043c 044b 0439 0020 0437  .4.0.5.<.K.9. .7
+00012b10: 0430 0433 043e 043b 043e 0432 043e 043a  .0.3.>.;.>.2.>.:
+00012b20: 0020 043e 0442 0447 0451 0442 0430 003a  . .>.B.G.Q.B.0.:
+00012b30: 0020 0800 0000 0006 0000 0023 4361 6e27  . .........#Can'
+00012b40: 7420 6669 6e64 2065 7870 6563 7465 6420  t find expected 
+00012b50: 7265 706f 7274 2068 6561 6465 723a 2007  report header: .
+00012b60: 0000 000c 5374 6174 656d 656e 7458 4c53  ....StatementXLS
+00012b70: 0103 0000 0066 041d 0435 0020 0443 0434  .....f...5. .C.4
+00012b80: 0430 043b 043e 0441 044c 0020 043e 043f  .0.;.>.A.L. .>.?
+00012b90: 0440 0435 0434 0435 043b 0438 0442 044c  .@.5.4.5.;.8.B.L
+00012ba0: 0020 0432 0430 043b 044e 0442 044b 0020  . .2.0.;.N.B.K. 
+00012bb0: 0438 0437 0020 043e 0431 0449 0435 0439  .8.7. .>.1.I.5.9
+00012bc0: 0020 0441 0435 043a 0446 0438 0438 0020  . .A.5.:.F.8.8. 
+00012bd0: 043e 0442 0447 0451 0442 0430 0800 0000  .>.B.G.Q.B.0....
+00012be0: 0006 0000 0036 4361 6e27 7420 6765 7420  .....6Can't get 
+00012bf0: 6375 7272 656e 6369 6573 2066 726f 6d20  currencies from 
+00012c00: 7375 6d6d 6172 7920 7365 6374 696f 6e20  summary section 
+00012c10: 6f66 2073 7461 7465 6d65 6e74 0700 0000  of statement....
+00012c20: 0c53 7461 7465 6d65 6e74 584c 5301 0300  .StatementXLS...
+00012c30: 0000 4604 1d04 3504 3204 3e04 3704 3c04  ..F...5.2.>.7.<.
+00012c40: 3e04 3604 3d04 3e00 2004 3e04 3f04 4004  >.6.=.>. .>.?.@.
+00012c50: 3504 3404 3504 3b04 3804 4204 4c00 2004  5.4.5.;.8.B.L. .
+00012c60: 3f04 3504 4004 3804 3e04 3400 2004 3e04  ?.5.@.8.>.4. .>.
+00012c70: 4204 4704 5104 4204 3008 0000 0000 0600  B.G.Q.B.0.......
+00012c80: 0000 1843 616e 2774 2072 6561 6420 7265  ...Can't read re
+00012c90: 706f 7274 2070 6572 696f 6407 0000 000c  port period.....
+00012ca0: 5374 6174 656d 656e 7458 4c53 0103 0000  StatementXLS....
+00012cb0: 001c 0414 0421 0020 0437 0430 0433 0440  .....!. .7.0.3.@
+00012cc0: 0443 0436 0435 043d 044b 003a 0020 0800  .C.6.5.=.K.:. ..
+00012cd0: 0000 0006 0000 0016 4361 7368 2062 616c  ........Cash bal
+00012ce0: 616e 6365 7320 6c6f 6164 6564 3a20 0700  ances loaded: ..
+00012cf0: 0000 0c53 7461 7465 6d65 6e74 584c 5301  ...StatementXLS.
+00012d00: 0300 0000 3604 2104 4204 3e04 3b04 3104  ....6.!.B.>.;.1.
+00012d10: 3504 4600 2004 3d04 3500 2004 3d04 3004  5.F. .=.5. .=.0.
+00012d20: 3904 3404 3504 3d00 2004 3200 2004 4104  9.4.5.=. .2. .A.
+00012d30: 3504 3a04 4604 3804 3800 2008 0000 0000  5.:.F.8.8. .....
+00012d40: 0600 0000 1c43 6f6c 756d 6e20 6e6f 7420  .....Column not 
+00012d50: 666f 756e 6420 696e 2073 6563 7469 6f6e  found in section
+00012d60: 2007 0000 000c 5374 6174 656d 656e 7458   .....StatementX
+00012d70: 4c53 0103 0000 0034 041d 0435 0441 043a  LS.....4...5.A.:
+00012d80: 043e 043b 044c 043a 043e 0020 0441 0447  .>.;.L.:.>. .A.G
+00012d90: 0435 0442 043e 0432 0020 043d 0430 0439  .5.B.>.2. .=.0.9
+00012da0: 0434 0435 043d 043e 003a 0020 0800 0000  .4.5.=.>.:. ....
+00012db0: 0006 0000 0019 4d75 6c74 6970 6c65 2061  ......Multiple a
+00012dc0: 6363 6f75 6e74 7320 666f 756e 643a 2007  ccounts found: .
+00012dd0: 0000 000c 5374 6174 656d 656e 7458 4c53  ....StatementXLS
+00012de0: 0103 0000 001c 0426 0411 0020 0437 0430  .......&... .7.0
+00012df0: 0433 0440 0443 0436 0435 043d 044b 003a  .3.@.C.6.5.=.K.:
+00012e00: 0020 0800 0000 0006 0000 0013 5365 6375  . ..........Secu
+00012e10: 7269 7469 6573 206c 6f61 6465 643a 2007  rities loaded: .
+00012e20: 0000 000c 5374 6174 656d 656e 7458 4c53  ....StatementXLS
+00012e30: 0103 0000 0030 041e 0442 0447 0451 0442  .....0...B.G.Q.B
+00012e40: 0020 0437 0430 0433 0440 0443 0436 0435  . .7.0.3.@.C.6.5
+00012e50: 043d 0020 0443 0441 043f 0435 0448 043d  .=. .C.A.?.5.H.=
+00012e60: 043e 003a 0020 0800 0000 0006 0000 001f  .>.:. ..........
+00012e70: 5374 6174 656d 656e 7420 6c6f 6164 6564  Statement loaded
+00012e80: 2073 7563 6365 7373 6675 6c6c 793a 2007   successfully: .
+00012e90: 0000 000c 5374 6174 656d 656e 7458 4c53  ....StatementXLS
+00012ea0: 0103 0000 0022 0020 0437 0430 0433 0440  .....". .7.0.3.@
+00012eb0: 0443 0436 0435 043d 0020 0443 0441 043f  .C.6.5.=. .C.A.?
+00012ec0: 0435 0448 043d 043e 0800 0000 0006 0000  .5.H.=.>........
+00012ed0: 0014 206c 6f61 6465 6420 7375 6363 6573  .. loaded succes
+00012ee0: 7366 756c 6c79 0700 0000 0c53 7461 7465  sfully.....State
+00012ef0: 6d65 6e74 584d 4c01 0300 0000 3604 1d04  mentXML.....6...
+00012f00: 3504 3204 3504 4004 3d04 4b04 3900 2004  5.2.5.@.=.K.9. .
+00012f10: 4404 3e04 4004 3c04 3004 4200 2000 5800  D.>.@.<.0.B. .X.
+00012f20: 4d00 4c00 2004 4404 3004 3904 3b04 3000  M.L. .D.0.9.;.0.
+00012f30: 3a00 2008 0000 0000 0600 0000 1643 616e  :. ..........Can
+00012f40: 2774 2070 6172 7365 2058 4d4c 2066 696c  't parse XML fil
+00012f50: 653a 2007 0000 000c 5374 6174 656d 656e  e: .....Statemen
+00012f60: 7458 4d4c 0103 0000 0044 041d 0435 0432  tXML.....D...5.2
+00012f70: 043e 0437 043c 043e 0436 043d 043e 0020  .>.7.<.>.6.=.>. 
+00012f80: 0437 0430 0433 0440 0443 0437 0438 0442  .7.0.3.@.C.7.8.B
+00012f90: 044c 0020 043e 0442 0447 0451 0442 0020  .L. .>.B.G.Q.B. 
+00012fa0: 043d 043e 043c 0435 0440 003a 0020 0800  .=.>.<.5.@.:. ..
+00012fb0: 0000 0006 0000 0020 4661 696c 6564 2074  ....... Failed t
+00012fc0: 6f20 6669 6e64 2073 7461 7465 6d65 6e74  o find statement
+00012fd0: 2069 6e64 6578 3a20 0700 0000 0c53 7461   index: .....Sta
+00012fe0: 7465 6d65 6e74 584d 4c01 0300 0000 3e04  tementXML.....>.
+00012ff0: 1d04 3504 3204 3e04 3704 3c04 3e04 3604  ..5.2.>.7.<.>.6.
+00013000: 3d04 3e00 2004 3704 3004 3304 4004 4304  =.>. .7.0.3.@.C.
+00013010: 3704 3804 4204 4c00 2004 3004 4204 4204  7.8.B.L. .0.B.B.
+00013020: 4004 3804 3104 4304 4200 3a00 2008 0000  @.8.1.C.B.:. ...
+00013030: 0000 0600 0000 1a46 6169 6c65 6420 746f  .......Failed to
+00013040: 206c 6f61 6420 6174 7472 6962 7574 653a   load attribute:
+00013050: 2007 0000 000c 5374 6174 656d 656e 7458   .....StatementX
+00013060: 4d4c 0103 0000 0042 041e 0442 0447 0451  ML.....B...B.G.Q
+00013070: 0442 0020 0431 0440 043e 043a 0435 0440  .B. .1.@.>.:.5.@
+00013080: 0430 0020 043d 0435 0020 043d 0430 0439  .0. .=.5. .=.0.9
+00013090: 0434 0435 043d 0020 0432 0020 0444 0430  .4.5.=. .2. .D.0
+000130a0: 0439 043b 0435 003a 0020 0800 0000 0006  .9.;.5.:. ......
+000130b0: 0000 0020 4e6f 2073 7461 7465 6d65 6e74  ... No statement
+000130c0: 2077 6173 2066 6f75 6e64 2069 6e20 6669   was found in fi
+000130d0: 6c65 3a20 0700 0000 0c53 7461 7465 6d65  le: .....Stateme
+000130e0: 6e74 584d 4c01 0300 0000 3404 1d04 3504  ntXML.....4...5.
+000130f0: 3804 3704 3204 3504 4104 4204 3d04 3004  8.7.2.5.A.B.=.0.
+00013100: 4f00 2004 3c04 3504 4204 3a04 3000 2004  O. .<.5.B.:.0. .
+00013110: 3e04 4204 4704 5104 4204 3000 3a00 2008  >.B.G.Q.B.0.:. .
+00013120: 0000 0000 0600 0000 1755 6e6b 6e6f 776e  .........Unknown
+00013130: 2073 7461 7465 6d65 6e74 2074 6167 3a20   statement tag: 
+00013140: 0700 0000 0c53 7461 7465 6d65 6e74 584d  .....StatementXM
+00013150: 4c01 0300 0000 4c04 1d04 3504 3f04 3e04  L.....L...5.?.>.
+00013160: 3404 3404 3504 4004 3604 3804 3204 3004  4.4.5.@.6.8.2.0.
+00013170: 3504 3c04 4b04 3900 2004 4404 3e04 4004  5.<.K.9. .D.>.@.
+00013180: 3c04 3004 4200 2004 3404 3004 4204 4b00  <.0.B. .4.0.B.K.
+00013190: 2f04 3204 4004 3504 3c04 3504 3d04 3800  /.2.@.5.<.5.=.8.
+000131a0: 3a00 2008 0000 0000 0600 0000 1e55 6e73  :. ..........Uns
+000131b0: 7570 706f 7274 6564 2064 6174 652f 7469  upported date/ti
+000131c0: 6d65 2066 6f72 6d61 743a 2007 0000 000c  me format: .....
+000131d0: 5374 6174 656d 656e 7458 4d4c 0103 0000  StatementXML....
+000131e0: 0020 041e 0448 0438 0431 043a 0430 0020  . ...H.8.1.:.0. 
+000131f0: 0438 043c 043f 043e 0440 0442 0430 003a  .8.<.?.>.@.B.0.:
+00013200: 0020 0800 0000 0006 0000 000f 496d 706f  . ..........Impo
+00013210: 7274 2066 6169 6c65 643a 2007 0000 000a  rt failed: .....
+00013220: 5374 6174 656d 656e 7473 0103 0000 0040  Statements.....@
+00013230: 0412 044b 0431 0435 0440 0438 0442 0435  ...K.1.5.@.8.B.5
+00013240: 0020 0444 0430 0439 043b 0020 043e 0442  . .D.0.9.;. .>.B
+00013250: 0447 0435 0442 0430 0020 0434 043b 044f  .G.5.B.0. .4.;.O
+00013260: 0020 0438 043c 043f 043e 0440 0442 0430  . .8.<.?.>.@.B.0
+00013270: 0800 0000 0006 0000 001f 5365 6c65 6374  ..........Select
+00013280: 2073 7461 7465 6d65 6e74 2066 696c 6520   statement file 
+00013290: 746f 2069 6d70 6f72 7407 0000 000a 5374  to import.....St
+000132a0: 6174 656d 656e 7473 0103 0000 004a 041a  atements.....J..
+000132b0: 043b 0430 0441 0441 0020 043e 0442 0447  .;.0.A.A. .>.B.G
+000132c0: 0451 0442 0430 0020 043d 0435 0020 043c  .Q.B.0. .=.5. .<
+000132d0: 043e 0436 0435 0442 0020 0431 044b 0442  .>.6.5.B. .1.K.B
+000132e0: 044c 0020 0437 0430 0433 0440 0443 0436  .L. .7.0.3.@.C.6
+000132f0: 0435 043d 003a 0020 0800 0000 0006 0000  .5.=.:. ........
+00013300: 0021 5374 6174 656d 656e 7420 636c 6173  .!Statement clas
+00013310: 7320 6361 6e27 7420 6265 206c 6f61 6465  s can't be loade
+00013320: 643a 2007 0000 000a 5374 6174 656d 656e  d: .....Statemen
+00013330: 7473 0103 0000 0054 041c 043e 0434 0443  ts.....T...>.4.C
+00013340: 043b 044c 0020 043e 0442 0447 0451 0442  .;.L. .>.B.G.Q.B
+00013350: 0430 0020 043d 0435 0020 043c 043e 0436  .0. .=.5. .<.>.6
+00013360: 0435 0442 0020 0431 044b 0442 044c 0020  .5.B. .1.K.B.L. 
+00013370: 0438 043c 043f 043e 0440 0442 0438 0440  .8.<.?.>.@.B.8.@
+00013380: 043e 0432 0430 043d 003a 0020 0800 0000  .>.2.0.=.:. ....
+00013390: 0006 0000 0024 5374 6174 656d 656e 7420  .....$Statement 
+000133a0: 6d6f 6475 6c65 2063 616e 2774 2062 6520  module can't be 
+000133b0: 696d 706f 7274 6564 3a20 0700 0000 0a53  imported: .....S
+000133c0: 7461 7465 6d65 6e74 7301 0300 0000 0804  tatements.......
+000133d0: 1004 3a04 4200 2e08 0000 0000 0600 0000  ..:.B...........
+000133e0: 0441 6374 2e07 0000 0010 5379 6d62 6f6c  .Act......Symbol
+000133f0: 734c 6973 744d 6f64 656c 0103 0000 000c  sListModel......
+00013400: 0412 0430 043b 044e 0442 0430 0800 0000  ...0.;.N.B.0....
+00013410: 0006 0000 0008 4375 7272 656e 6379 0700  ......Currency..
+00013420: 0000 1053 796d 626f 6c73 4c69 7374 4d6f  ...SymbolsListMo
+00013430: 6465 6c01 0300 0000 1004 1e04 3f04 3804  del.........?.8.
+00013440: 4104 3004 3d04 3804 3508 0000 0000 0600  A.0.=.8.5.......
+00013450: 0000 0b44 6573 6372 6970 7469 6f6e 0700  ...Description..
+00013460: 0000 1053 796d 626f 6c73 4c69 7374 4d6f  ...SymbolsListMo
+00013470: 6465 6c01 0300 0000 1204 1a04 3e04 4204  del.........>.B.
+00013480: 3804 4004 3e04 3204 3a04 3808 0000 0000  8.@.>.2.:.8.....
+00013490: 0600 0000 0651 756f 7465 7307 0000 0010  .....Quotes.....
+000134a0: 5379 6d62 6f6c 734c 6973 744d 6f64 656c  SymbolsListModel
+000134b0: 0103 0000 000c 0421 0438 043c 0432 043e  .......!.8.<.2.>
+000134c0: 043b 0800 0000 0006 0000 0006 5379 6d62  .;..........Symb
+000134d0: 6f6c 0700 0000 1053 796d 626f 6c73 4c69  ol.....SymbolsLi
+000134e0: 7374 4d6f 6465 6c01 0300 0000 0604 2204  stModel.......".
+000134f0: 4d04 3308 0000 0000 0600 0000 0354 6167  M.3..........Tag
+00013500: 0700 0000 0c54 6167 4c69 7374 4d6f 6465  .....TagListMode
+00013510: 6c01 0300 0000 1004 1e04 3f04 3504 4004  l.........?.5.@.
+00013520: 3004 4604 3804 3808 0000 0000 0600 0000  0.F.8.8.........
+00013530: 0a4f 7065 7261 7469 6f6e 7307 0000 0009  .Operations.....
+00013540: 5461 6752 6570 6f72 7401 0300 0000 1004  TagReport.......
+00013550: 3f04 3e00 2004 1c04 3504 4204 3a04 3508  ?.>. ...5.B.:.5.
+00013560: 0000 0000 0600 0000 0662 7920 5461 6707  .........by Tag.
+00013570: 0000 0009 5461 6752 6570 6f72 7401 0300  ....TagReport...
+00013580: 0000 1c04 1e04 4204 4704 3504 4200 2004  ......B.G.5.B. .
+00013590: 3f04 3e00 2004 3c04 3504 4204 3a04 3508  ?.>. .<.5.B.:.5.
+000135a0: 0000 0000 0600 0000 0d52 6570 6f72 7420  .........Report 
+000135b0: 6279 2074 6167 0700 0000 0f54 6167 5265  by tag.....TagRe
+000135c0: 706f 7274 5769 6467 6574 0103 0000 000c  portWidget......
+000135d0: 041c 0435 0442 043a 0430 003a 0800 0000  ...5.B.:.0.:....
+000135e0: 0006 0000 0004 5461 673a 0700 0000 0f54  ......Tag:.....T
+000135f0: 6167 5265 706f 7274 5769 6467 6574 0103  agReportWidget..
+00013600: 0000 0024 0027 0020 0437 0430 043c 0435  ...$.'. .7.0.<.5
+00013610: 043d 0435 043d 0430 0020 0443 0441 043f  .=.5.=.0. .C.A.?
+00013620: 0435 0448 043d 043e 0800 0000 0006 0000  .5.H.=.>........
+00013630: 001b 2720 7761 7320 7375 6363 6573 7366  ..' was successf
+00013640: 756c 6c79 2072 6570 6c61 6365 6407 0000  ully replaced...
+00013650: 000e 5461 6773 4c69 7374 4469 616c 6f67  ..TagsListDialog
+00013660: 0103 0000 000c 0027 0020 043d 0430 003a  .......'. .=.0.:
+00013670: 0020 0800 0000 0006 0000 0008 2720 7769  . ..........' wi
+00013680: 7468 3a20 0700 0000 0e54 6167 734c 6973  th: .....TagsLis
+00013690: 7444 6961 6c6f 6701 0300 0000 2004 1704  tDialog..... ...
+000136a0: 3004 3c04 3504 3d04 3804 4204 4c00 2004  0.<.5.=.8.B.L. .
+000136b0: 3c04 3504 4204 3a04 4300 2000 2708 0000  <.5.B.:.C. .'...
+000136c0: 0000 0600 0000 0d52 6570 6c61 6365 2074  .......Replace t
+000136d0: 6167 2027 0700 0000 0e54 6167 734c 6973  ag '.....TagsLis
+000136e0: 7444 6961 6c6f 6701 0300 0000 1c04 1704  tDialog.........
+000136f0: 3004 3c04 3504 3d04 3804 4204 4c00 2004  0.<.5.=.8.B.L. .
+00013700: 3d04 3000 2e00 2e00 2e08 0000 0000 0600  =.0.............
+00013710: 0000 0f52 6570 6c61 6365 2077 6974 682e  ...Replace with.
+00013720: 2e2e 0700 0000 0e54 6167 734c 6973 7444  .......TagsListD
+00013730: 6961 6c6f 6701 0300 0000 3404 1f04 3e04  ialog.....4...>.
+00013740: 3a04 3004 3704 3004 4204 4c00 2004 3e04  :.0.7.0.B.L. .>.
+00013750: 3f04 3504 4004 3004 4604 3804 3800 2004  ?.5.@.0.F.8.8. .
+00013760: 4100 2004 1c04 3504 4204 3a04 3e04 3908  A. ...5.B.:.>.9.
+00013770: 0000 0000 0600 0000 1853 686f 7720 6f70  .........Show op
+00013780: 6572 6174 696f 6e73 2077 6974 6820 5461  erations with Ta
+00013790: 6707 0000 000e 5461 6773 4c69 7374 4469  g.....TagsListDi
+000137a0: 616c 6f67 0103 0000 000e 041c 0435 0442  alog.........5.B
+000137b0: 043a 0430 0020 0027 0800 0000 0006 0000  .:.0. .'........
+000137c0: 0005 5461 6720 2707 0000 000e 5461 6773  ..Tag '.....Tags
+000137d0: 4c69 7374 4469 616c 6f67 0103 0000 0008  ListDialog......
+000137e0: 0422 044d 0433 0438 0800 0000 0006 0000  .".M.3.8........
+000137f0: 0004 5461 6773 0700 0000 0e54 6167 734c  ..Tags.....TagsL
+00013800: 6973 7444 6961 6c6f 6701 0300 0000 1a04  istDialog.......
+00013810: 2204 3504 3a04 4304 4904 3804 3900 2004  ".5.:.C.I.8.9. .
+00013820: 3a04 4304 4004 4100 3a08 0000 0000 0600  :.C.@.A.:.......
+00013830: 0000 0d43 7572 7265 6e74 2072 6174 653a  ...Current rate:
+00013840: 0700 0000 1354 6178 4573 7469 6d61 7469  .....TaxEstimati
+00013850: 6f6e 4469 616c 6f67 0103 0000 0028 041f  onDialog.....(..
+00013860: 043e 0441 043b 0435 0434 043d 044f 044f  .>.A.;.5.4.=.O.O
+00013870: 0020 043a 043e 0442 0438 0440 043e 0432  . .:.>.B.8.@.>.2
+00013880: 043a 0430 003a 0800 0000 0006 0000 000b  .:.0.:..........
+00013890: 4c61 7374 2071 756f 7465 3a07 0000 0013  Last quote:.....
+000138a0: 5461 7845 7374 696d 6174 696f 6e44 6961  TaxEstimationDia
+000138b0: 6c6f 6701 0300 0000 1a04 1e04 4604 3504  log.........F.5.
+000138c0: 3d04 3a04 3000 2004 3d04 3004 3b04 3e04  =.:.0. .=.0.;.>.
+000138d0: 3304 3008 0000 0000 0600 0000 0e54 6178  3.0..........Tax
+000138e0: 2045 7374 696d 6174 696f 6e07 0000 0013   Estimation.....
+000138f0: 5461 7845 7374 696d 6174 696f 6e44 6961  TaxEstimationDia
+00013900: 6c6f 6701 0300 0000 0800 5800 2e00 5800  log.......X...X.
+00013910: 5808 0000 0000 0600 0000 0458 2e58 5807  X..........X.XX.
+00013920: 0000 0013 5461 7845 7374 696d 6174 696f  ....TaxEstimatio
+00013930: 6e44 6961 6c6f 6701 0300 0000 0a04 1804  nDialog.........
+00013940: 2204 1e04 1304 1e08 0000 0000 0600 0000  "...............
+00013950: 0554 4f54 414c 0700 0000 0c54 6178 4573  .TOTAL.....TaxEs
+00013960: 7469 6d61 746f 7201 0300 0000 2404 1e04  timator.....$...
+00013970: 4604 3504 3d04 3a04 3000 2004 3d04 3004  F.5.=.:.0. .=.0.
+00013980: 3b04 3e04 3304 3000 2004 3404 3b04 4f00  ;.>.3.0. .4.;.O.
+00013990: 2008 0000 0000 0600 0000 1354 6178 2065   ..........Tax e
+000139a0: 7374 696d 6174 696f 6e20 666f 7220 0700  stimation for ..
+000139b0: 0000 0c54 6178 4573 7469 6d61 746f 7201  ...TaxEstimator.
+000139c0: 0300 0000 3c04 2104 4204 3004 3204 3a04  ....<.!.B.0.2.:.
+000139d0: 3000 2004 3d04 3004 3b04 3e04 3304 3000  0. .=.0.;.>.3.0.
+000139e0: 2004 3d04 3500 2004 3d04 3004 3904 3404   .=.5. .=.0.9.4.
+000139f0: 3504 3d04 3000 2004 3404 3b04 4f00 3a00  5.=.0. .4.;.O.:.
+00013a00: 2008 0000 0000 0600 0000 1854 6178 2072   ..........Tax r
+00013a10: 6174 6520 6e6f 7420 666f 756e 6420 666f  ate not found fo
+00013a20: 723a 2007 0000 000c 5461 7845 7374 696d  r: .....TaxEstim
+00013a30: 6174 6f72 0103 0000 0008 0414 0430 0442  ator.........0.B
+00013a40: 0430 0800 0000 0006 0000 0004 4461 7465  .0..........Date
+00013a50: 0700 0000 1154 6178 4573 7469 6d61 746f  .....TaxEstimato
+00013a60: 724d 6f64 656c 0103 0000 0014 0426 0435  rModel.......&.5
+00013a70: 043d 0430 0020 043e 0442 043a 0440 002e  .=.0. .>.B.:.@..
+00013a80: 0800 0000 0006 0000 0004 4f70 656e 0700  ..........Open..
+00013a90: 0000 1154 6178 4573 7469 6d61 746f 724d  ...TaxEstimatorM
+00013aa0: 6f64 656c 0103 0000 0012 041f 0440 0438  odel.........@.8
+00013ab0: 0431 044b 043b 044c 002c 0020 0800 0000  .1.K.;.L.,. ....
+00013ac0: 0006 0000 0008 5072 6f66 6974 2c20 0700  ......Profit, ..
+00013ad0: 0000 1154 6178 4573 7469 6d61 746f 724d  ...TaxEstimatorM
+00013ae0: 6f64 656c 0103 0000 000c 041a 043e 043b  odel.........>.;
+00013af0: 002d 0432 043e 0800 0000 0006 0000 0003  .-.2.>..........
+00013b00: 5174 7907 0000 0011 5461 7845 7374 696d  Qty.....TaxEstim
+00013b10: 6174 6f72 4d6f 6465 6c01 0300 0000 0c04  atorModel.......
+00013b20: 1a04 4304 4004 4100 2c00 2008 0000 0000  ..C.@.A.,. .....
+00013b30: 0600 0000 0652 6174 652c 2007 0000 0011  .....Rate, .....
+00013b40: 5461 7845 7374 696d 6174 6f72 4d6f 6465  TaxEstimatorMode
+00013b50: 6c01 0300 0000 0e04 1d04 3004 3b04 3e04  l.........0.;.>.
+00013b60: 3300 2c00 2008 0000 0000 0600 0000 0554  3.,. ..........T
+00013b70: 6178 2c20 0700 0000 1154 6178 4573 7469  ax, .....TaxEsti
+00013b80: 6d61 746f 724d 6f64 656c 0103 0000 0074  matorModel.....t
+00013b90: 041d 0435 0432 043e 0437 043c 043e 0436  ...5.2.>.7.<.>.6
+00013ba0: 043d 043e 0020 0437 0430 0433 0440 0443  .=.>. .7.0.3.@.C
+00013bb0: 0437 0438 0442 044c 0020 043f 0430 0440  .7.8.B.L. .?.0.@
+00013bc0: 0430 043c 0435 0442 0440 044b 0020 043d  .0.<.5.B.@.K. .=
+00013bd0: 0430 043b 043e 0433 043e 0432 043e 0433  .0.;.>.3.>.2.>.3
+00013be0: 043e 0020 043e 0442 0447 0451 0442 0430  .>. .>.B.G.Q.B.0
+00013bf0: 0020 0438 0437 0020 0444 0430 0439 043b  . .8.7. .D.0.9.;
+00013c00: 0430 0020 0800 0000 0006 0000 002b 4361  .0. .........+Ca
+00013c10: 6e27 7420 6c6f 6164 2074 6178 2072 6570  n't load tax rep
+00013c20: 6f72 7420 7061 7261 6d65 7465 7273 2066  ort parameters f
+00013c30: 726f 6d20 6669 6c65 2007 0000 0009 5461  rom file .....Ta
+00013c40: 7852 6570 6f72 7401 0300 0000 2804 1d04  xReport.....(...
+00013c50: 3504 3804 3704 3204 3504 4104 4204 3d04  5.8.7.2.5.A.B.=.
+00013c60: 3004 4f00 2004 3204 3004 3b04 4e04 4204  0.O. .2.0.;.N.B.
+00013c70: 3000 3a00 2008 0000 0000 0600 0000 1943  0.:. ..........C
+00013c80: 7572 7265 6e63 7920 6973 206e 6f74 2064  urrency is not d
+00013c90: 6566 696e 6564 3a20 0700 0000 0954 6178  efined: .....Tax
+00013ca0: 5265 706f 7274 0103 0000 004a 041d 0435  Report.....J...5
+00013cb0: 0020 0443 043a 0430 0437 0430 043d 0020  . .C.:.0.7.0.=. 
+00013cc0: 0448 0430 0431 043b 043e 043d 0020 043e  .H.0.1.;.>.=. .>
+00013cd0: 0442 0447 0435 0442 0430 0020 0434 043b  .B.G.5.B.0. .4.;
+00013ce0: 044f 0020 0440 0430 0437 0434 0435 043b  .O. .@.0.7.4.5.;
+00013cf0: 0430 003a 0020 0800 0000 0006 0000 0026  .0.:. .........&
+00013d00: 4e6f 2072 6570 6f72 7420 7465 6d70 6c61  No report templa
+00013d10: 7465 2066 6f75 6e64 2066 6f72 2073 6563  te found for sec
+00013d20: 7469 6f6e 3a20 0700 0000 0954 6178 5265  tion: .....TaxRe
+00013d30: 706f 7274 0103 0000 006a 041d 0435 0442  port.....j...5.B
+00013d40: 0020 0438 043d 0444 043e 0440 043c 0430  . .8.=.D.>.@.<.0
+00013d50: 0446 0438 0438 0020 043e 0020 0421 043e  .F.8.8. .>. .!.>
+00013d60: 0418 0414 041d 0020 0432 0020 043f 0430  ....... .2. .?.0
+00013d70: 0440 0430 043c 0435 0442 0440 0430 0445  .@.0.<.5.B.@.0.E
+00013d80: 0020 043d 0430 043b 043e 0433 043e 0432  . .=.0.;.>.3.>.2
+00013d90: 043e 0433 043e 0020 043e 0442 0447 0451  .>.3.>. .>.B.G.Q
+00013da0: 0442 0430 0800 0000 0006 0000 0042 5468  .B.0.........BTh
+00013db0: 6572 6520 6172 6520 6e6f 2069 6e66 6f72  ere are no infor
+00013dc0: 6d61 7469 6f6e 2061 626f 7574 2074 6178  mation about tax
+00013dd0: 2074 7265 6174 7920 696e 2074 6178 2072   treaty in tax r
+00013de0: 6570 6f72 7420 7061 7261 6d65 7465 7273  eport parameters
+00013df0: 0700 0000 0954 6178 5265 706f 7274 0103  .....TaxReport..
+00013e00: 0000 0060 041d 0435 0020 0437 0430 0434  ...`...5. .7.0.4
+00013e10: 0430 043d 044b 0020 043f 0430 0440 0430  .0.=.K. .?.0.@.0
+00013e20: 043c 0435 0442 0440 044b 0020 043d 0430  .<.5.B.@.K. .=.0
+00013e30: 043b 043e 0433 043e 0432 043e 0433 043e  .;.>.3.>.2.>.3.>
+00013e40: 0020 043e 0442 0447 0451 0442 0430 0020  . .>.B.G.Q.B.0. 
+00013e50: 0434 043b 044f 0020 0433 043e 0434 0430  .4.;.O. .3.>.4.0
+00013e60: 003a 0020 0800 0000 0006 0000 0033 5468  .:. .........3Th
+00013e70: 6572 6520 6172 6520 6e6f 2070 6172 616d  ere are no param
+00013e80: 6574 6572 7320 666f 756e 6420 666f 7220  eters found for 
+00013e90: 7461 7820 7265 706f 7274 2079 6561 723a  tax report year:
+00013ea0: 2007 0000 0009 5461 7852 6570 6f72 7401   .....TaxReport.
+00013eb0: 0300 0000 0a00 2000 2e00 2e00 2e00 2008  ...... ....... .
+00013ec0: 0000 0000 0600 0000 0520 2e2e 2e20 0700  ......... ... ..
+00013ed0: 0000 0954 6178 5769 6467 6574 0103 0000  ...TaxWidget....
+00013ee0: 0006 002e 002e 002e 0800 0000 0006 0000  ................
+00013ef0: 0003 2e2e 2e07 0000 0009 5461 7857 6964  ..........TaxWid
+00013f00: 6765 7401 0300 0000 0a04 2104 4704 3504  get.......!.G.5.
+00013f10: 4200 3a08 0000 0000 0600 0000 0841 6363  B.:..........Acc
+00013f20: 6f75 6e74 3a07 0000 0009 5461 7857 6964  ount:.....TaxWid
+00013f30: 6765 7401 0300 0000 9004 1d04 3804 3604  get.........8.6.
+00013f40: 3500 2004 4004 3004 4104 3f04 3e04 3b04  5. .@.0.A.?.>.;.
+00013f50: 3e04 3604 3504 3d04 4b00 2004 4d04 3a04  >.6.5.=.K. .M.:.
+00013f60: 4104 3f04 3504 4004 3804 3c04 3504 3d04  A.?.5.@.8.<.5.=.
+00013f70: 4204 3004 3b04 4c04 3d04 4b04 3500 2004  B.0.;.L.=.K.5. .
+00013f80: 4404 4304 3d04 3a04 4604 3804 3800 2000  D.C.=.:.F.8.8. .
+00013f90: 2d00 2004 3804 4104 3f04 3e04 3b04 4c04  -. .8.A.?.>.;.L.
+00013fa0: 3704 4304 3904 4204 3500 2004 4100 2004  7.C.9.B.5. .A. .
+00013fb0: 3e04 4104 4204 3e04 4004 3e04 3604 3d04  >.A.B.>.@.>.6.=.
+00013fc0: 3e04 4104 4204 4c04 4e08 0000 0000 0600  >.A.B.L.N.......
+00013fd0: 0000 3342 656c 6f77 2066 756e 6374 696f  ..3Below functio
+00013fe0: 6e73 2061 7265 2065 7870 6572 696d 656e  ns are experimen
+00013ff0: 7461 6c20 2d20 7573 6520 6974 2077 6974  tal - use it wit
+00014000: 6820 6361 7265 0700 0000 0954 6178 5769  h care.....TaxWi
+00014010: 6467 6574 0103 0000 0044 041d 0435 0432  dget.....D...5.2
+00014020: 043e 0437 043c 043e 0436 043d 043e 0020  .>.7.<.>.6.=.>. 
+00014030: 0437 0430 043f 0438 0441 0430 0442 044c  .7.0.?.8.A.0.B.L
+00014040: 0020 0033 002d 041d 0414 0424 041b 0020  . .3.-.....$... 
+00014050: 0432 0020 0444 0430 0439 043b 0020 0800  .2. .D.0.9.;. ..
+00014060: 0000 0006 0000 001f 4361 6e27 7420 7772  ........Can't wr
+00014070: 6974 6520 7461 7820 666f 726d 2069 6e74  ite tax form int
+00014080: 6f20 6669 6c65 2007 0000 0009 5461 7857  o file .....TaxW
+00014090: 6964 6765 7401 0300 0000 0e04 2104 4204  idget.......!.B.
+000140a0: 4004 3004 3d04 3000 3a08 0000 0000 0600  @.0.=.0.:.......
+000140b0: 0000 0843 6f75 6e74 7279 3a07 0000 0009  ...Country:.....
+000140c0: 5461 7857 6964 6765 7401 0300 0000 7804  TaxWidget.....x.
+000140d0: 2104 3e04 3704 3404 3004 4204 4c00 2004  !.>.7.4.0.B.L. .
+000140e0: 4404 3004 3904 3b00 2000 3300 2d04 1d04  D.0.9.;. .3.-...
+000140f0: 2404 1404 1b00 2004 3200 2004 4404 3e04  $..... .2. .D.>.
+00014100: 4004 3c04 3004 4204 3500 2004 3f04 4004  @.<.0.B.5. .?.@.
+00014110: 3e04 3304 4004 3004 3c04 3c04 4b00 2000  >.3.@.0.<.<.K. .
+00014120: 2204 1404 3504 3a04 3b04 3004 4004 3004  "...5.:.;.0.@.0.
+00014130: 4604 3804 4f00 2200 2000 2800 2a00 2e00  F.8.O.". .(.*...
+00014140: 6400 6300 5800 2908 0000 0000 0600 0000  d.c.X.).........
+00014150: 4043 7265 6174 6520 7461 7820 666f 726d  @Create tax form
+00014160: 2069 6e20 22d0 94d0 b5d0 bad0 bbd0 b0d1   in "...........
+00014170: 80d0 b0d1 86d0 b8d1 8f22 2070 726f 6772  ........." progr
+00014180: 616d 2066 6f72 6d61 7420 282a 2e64 6358  am format (*.dcX
+00014190: 2907 0000 0009 5461 7857 6964 6765 7401  ).....TaxWidget.
+000141a0: 0300 0000 1e04 1404 3004 3d04 3d04 4b04  ........0.=.=.K.
+000141b0: 3500 2004 3d04 3504 3f04 3e04 3b04 3d04  5. .=.5.?.>.;.=.
+000141c0: 4b04 3508 0000 0000 0600 0000 1344 6174  K.5..........Dat
+000141d0: 6120 6172 6520 696e 636f 6d70 6c65 7465  a are incomplete
+000141e0: 0700 0000 0954 6178 5769 6467 6574 0103  .....TaxWidget..
+000141f0: 0000 005c 041d 0435 0020 0438 0441 043f  ...\...5. .8.A.?
+00014200: 043e 043b 044c 0437 043e 0432 0430 0442  .>.;.L.7.>.2.0.B
+00014210: 044c 0020 0434 0430 0442 0443 0020 043f  .L. .4.0.B.C. .?
+00014220: 043e 0441 0442 0430 0432 043a 0438 0020  .>.A.B.0.2.:.8. 
+00014230: 0434 043b 044f 0020 043a 0443 0440 0441  .4.;.O. .:.C.@.A
+00014240: 043e 0432 0020 0432 0430 043b 044e 0442  .>.2. .2.0.;.N.B
+00014250: 0800 0000 0006 0000 002d 446f 206e 6f74  .........-Do not
+00014260: 2075 7365 2073 6574 746c 656d 656e 7420   use settlement 
+00014270: 6461 7465 2066 6f72 2063 7572 7265 6e63  date for currenc
+00014280: 7920 7261 7465 7307 0000 0009 5461 7857  y rates.....TaxW
+00014290: 6964 6765 7401 0300 0000 1604 2404 3004  idget.......$.0.
+000142a0: 3904 3b00 2000 4500 7800 6300 6500 6c00  9.;. .E.x.c.e.l.
+000142b0: 3a08 0000 0000 0600 0000 0b45 7863 656c  :..........Excel
+000142c0: 2066 696c 653a 0700 0000 0954 6178 5769   file:.....TaxWi
+000142d0: 6467 6574 0103 0000 0028 0424 0430 0439  dget.....(.$.0.9
+000142e0: 043b 044b 0020 0045 0078 0063 0065 006c  .;.K. .E.x.c.e.l
+000142f0: 0020 0028 002a 002e 0078 0073 006c 0078  . .(.*...x.s.l.x
+00014300: 0029 0800 0000 0006 0000 0014 4578 6365  .)..........Exce
+00014310: 6c20 6669 6c65 7320 282a 2e78 6c73 7829  l files (*.xlsx)
+00014320: 0700 0000 0954 6178 5769 6467 6574 0103  .....TaxWidget..
+00014330: 0000 004a 0424 0430 0439 043b 0020 0434  ...J.$.0.9.;. .4
+00014340: 043b 044f 0020 0441 043e 0445 0440 0430  .;.O. .A.>.E.@.0
+00014350: 043d 0435 043d 0438 044f 0020 0434 0435  .=.5.=.8.O. .4.5
+00014360: 043a 043b 0430 0440 0430 0446 0438 0438  .:.;.0.@.0.F.8.8
+00014370: 0020 0033 002d 041d 0414 0424 041b 0800  . .3.-.....$....
+00014380: 0000 0006 0000 0024 4669 6c65 2077 6865  .......$File whe
+00014390: 7265 2074 6f20 7374 6f72 6520 7275 7373  re to store russ
+000143a0: 6961 6e20 7461 7820 666f 726d 0700 0000  ian tax form....
+000143b0: 0954 6178 5769 6467 6574 0103 0000 0056  .TaxWidget.....V
+000143c0: 0424 0430 0439 043b 0020 0434 043b 044f  .$.0.9.;. .4.;.O
+000143d0: 0020 0441 043e 0445 0440 0430 043d 0435  . .A.>.E.@.0.=.5
+000143e0: 043d 0438 044f 0020 0440 0430 0441 0447  .=.8.O. .@.0.A.G
+000143f0: 0451 0442 0430 0020 0432 0020 0444 043e  .Q.B.0. .2. .D.>
+00014400: 0440 043c 0430 0442 0435 0020 0045 0078  .@.<.0.B.5. .E.x
+00014410: 0063 0065 006c 0800 0000 0006 0000 002e  .c.e.l..........
+00014420: 4669 6c65 2077 6865 7265 2074 6f20 7374  File where to st
+00014430: 6f72 6520 7461 7820 7265 706f 7274 2069  ore tax report i
+00014440: 6e20 4578 6365 6c20 666f 726d 6174 0700  n Excel format..
+00014450: 0000 0954 6178 5769 6467 6574 0103 0000  ...TaxWidget....
+00014460: 0068 0417 0430 0440 0443 0431 0435 0436  .h...0.@.C.1.5.6
+00014470: 043d 044b 0439 0020 0441 0447 0451 0442  .=.K.9. .A.G.Q.B
+00014480: 0020 0434 043b 044f 0020 043a 043e 0442  . .4.;.O. .:.>.B
+00014490: 043e 0440 043e 0433 043e 0020 043d 0443  .>.@.>.3.>. .=.C
+000144a0: 0436 043d 043e 0020 043f 043e 0434 0433  .6.=.>. .?.>.4.3
+000144b0: 043e 0442 043e 0432 0438 0442 044c 0020  .>.B.>.2.8.B.L. 
+000144c0: 043e 0442 0447 0451 0442 0800 0000 0006  .>.B.G.Q.B......
+000144d0: 0000 0029 466f 7265 6967 6e20 6163 636f  ...)Foreign acco
+000144e0: 756e 7420 746f 2070 7265 7061 7265 2074  unt to prepare t
+000144f0: 6178 2072 6570 6f72 7420 666f 7207 0000  ax report for...
+00014500: 0009 5461 7857 6964 6765 7401 0300 0000  ..TaxWidget.....
+00014510: 2604 2404 3004 3904 3b00 2004 4100 2004  &.$.0.9.;. .A. .
+00014520: 4004 3504 3704 4304 3b04 4c04 4204 3004  @.5.7.C.;.L.B.0.
+00014530: 4204 3e04 3c00 3a08 0000 0000 0600 0000  B.>.<.:.........
+00014540: 0c4f 7574 7075 7420 6669 6c65 3a07 0000  .Output file:...
+00014550: 0009 5461 7857 6964 6765 7401 0300 0000  ..TaxWidget.....
+00014560: 1e04 2104 3e04 4504 4004 3004 3d04 3804  ..!.>.E.@.0.=.8.
+00014570: 4204 4c00 2004 1e04 4204 4704 5104 4208  B.L. ...B.G.Q.B.
+00014580: 0000 0000 0600 0000 0b53 6176 6520 5265  .........Save Re
+00014590: 706f 7274 0700 0000 0954 6178 5769 6467  port.....TaxWidg
+000145a0: 6574 0103 0000 0026 0421 043e 0445 0440  et.....&.!.>.E.@
+000145b0: 0430 043d 0438 0442 044c 0020 0033 002d  .0.=.8.B.L. .3.-
+000145c0: 041d 0414 0424 041b 0020 0432 003a 0800  .....$... .2.:..
+000145d0: 0000 0006 0000 0011 5361 7665 2074 6178  ........Save tax
+000145e0: 2066 6f72 6d20 746f 3a07 0000 0009 5461   form to:.....Ta
+000145f0: 7857 6964 6765 7401 0300 0000 3804 2104  xWidget.....8.!.
+00014600: 3e04 4504 4004 3004 3d04 3804 4204 4c00  >.E.@.0.=.8.B.L.
+00014610: 2004 3d04 3004 3b04 3e04 3304 3e04 3204   .=.0.;.>.3.>.2.
+00014620: 4b04 3900 2004 3e04 4204 4704 5104 4200  K.9. .>.B.G.Q.B.
+00014630: 2004 3200 3a08 0000 0000 0600 0000 1453   .2.:..........S
+00014640: 6176 6520 7461 7820 7265 706f 7274 7320  ave tax reports 
+00014650: 746f 3a07 0000 0009 5461 7857 6964 6765  to:.....TaxWidge
+00014660: 7401 0300 0000 1804 1204 4b04 3104 3504  t.........K.1.5.
+00014670: 4004 3804 4200 2004 4404 3004 3904 3b08  @.8.B. .D.0.9.;.
+00014680: 0000 0000 0600 0000 0b53 656c 6563 7420  .........Select 
+00014690: 6669 6c65 0700 0000 0954 6178 5769 6467  file.....TaxWidg
+000146a0: 6574 0103 0000 0028 041d 0430 043b 043e  et.....(...0.;.>
+000146b0: 0433 043e 0432 044b 0439 0020 043e 0442  .3.>.2.K.9. .>.B
+000146c0: 0447 0451 0442 0020 043f 0443 0441 0442  .G.Q.B. .?.C.A.B
+000146d0: 0800 0000 0006 0000 0013 5461 7820 7265  ..........Tax re
+000146e0: 706f 7274 2069 7320 656d 7074 7907 0000  port is empty...
+000146f0: 0009 5461 7857 6964 6765 7401 0300 0000  ..TaxWidget.....
+00014700: 4004 1d04 3004 3b04 3e04 3304 3e04 3204  @...0.;.>.3.>.2.
+00014710: 4b04 3900 2004 3e04 4204 4704 5104 4200  K.9. .>.B.G.Q.B.
+00014720: 2004 4104 3e04 4504 4004 3004 3d04 5104   .A.>.E.@.0.=.Q.
+00014730: 3d00 2004 3200 2004 4404 3004 3904 3b00  =. .2. .D.0.9.;.
+00014740: 2008 0000 0000 0600 0000 1954 6178 2072   ..........Tax r
+00014750: 6570 6f72 7420 7361 7665 6420 746f 2066  eport saved to f
+00014760: 696c 6520 0700 0000 0954 6178 5769 6467  ile .....TaxWidg
+00014770: 6574 0103 0000 0040 041d 0430 043b 043e  et.....@...0.;.>
+00014780: 0433 043e 0432 044b 0439 0020 043e 0442  .3.>.2.K.9. .>.B
+00014790: 0447 0451 0442 0020 0441 043e 0445 0440  .G.Q.B. .A.>.E.@
+000147a0: 0430 043d 0451 043d 0020 0432 0020 0444  .0.=.Q.=. .2. .D
+000147b0: 0430 0439 043b 0020 0800 0000 0006 0000  .0.9.;. ........
+000147c0: 001d 5461 7820 7265 706f 7274 2077 6173  ..Tax report was
+000147d0: 2073 6176 6564 2074 6f20 6669 6c65 2007   saved to file .
+000147e0: 0000 0009 5461 7857 6964 6765 7401 0300  ....TaxWidget...
+000147f0: 0000 0c04 1d04 3004 3b04 3e04 3304 3808  ......0.;.>.3.8.
+00014800: 0000 0000 0600 0000 0554 6178 6573 0700  .........Taxes..
+00014810: 0000 0954 6178 5769 6467 6574 0103 0000  ...TaxWidget....
+00014820: 004e 041e 0431 043d 043e 0432 0438 0442  .N...1.=.>.2.8.B
+00014830: 044c 0020 0442 043e 043b 044c 043a 043e  .L. .B.>.;.L.:.>
+00014840: 0020 0438 043d 0444 043e 0440 043c 0430  . .8.=.D.>.@.<.0
+00014850: 0446 0438 044e 0020 043e 0020 0434 0438  .F.8.N. .>. .4.8
+00014860: 0432 0438 0434 0435 043d 0434 0430 0445  .2.8.4.5.=.4.0.E
+00014870: 0800 0000 0006 0000 0027 5570 6461 7465  .........'Update
+00014880: 206f 6e6c 7920 696e 666f 726d 6174 696f   only informatio
+00014890: 6e20 6162 6f75 7420 6469 7669 6465 6e64  n about dividend
+000148a0: 7307 0000 0009 5461 7857 6964 6765 7401  s.....TaxWidget.
+000148b0: 0300 0000 6404 1804 4104 3f04 3e04 3b04  ....d...A.?.>.;.
+000148c0: 4c04 3704 3e04 3204 3004 4204 4c00 2004  L.7.>.2.0.B.L. .
+000148d0: 3d04 3004 3704 3204 3004 3d04 3804 3500  =.0.7.2.0.=.8.5.
+000148e0: 2004 3104 4004 3e04 3a04 3504 4004 3000   .1.@.>.:.5.@.0.
+000148f0: 2004 3a04 3004 3a00 2004 3804 4104 4204   .:.0.:. .8.A.B.
+00014900: 3e04 4704 3d04 3804 3a00 2004 3204 4b04  >.G.=.8.:. .2.K.
+00014910: 3f04 3b04 3004 4204 4b08 0000 0000 0600  ?.;.0.B.K.......
+00014920: 0000 2055 7365 2062 726f 6b65 7220 6e61  .. Use broker na
+00014930: 6d65 2061 7320 696e 636f 6d65 2073 6f75  me as income sou
+00014940: 7263 6507 0000 0009 5461 7857 6964 6765  rce.....TaxWidge
+00014950: 7401 0300 0000 0804 1304 3e04 3400 3a08  t.........>.4.:.
+00014960: 0000 0000 0600 0000 0559 6561 723a 0700  .........Year:..
+00014970: 0000 0954 6178 5769 6467 6574 0103 0000  ...TaxWidget....
+00014980: 0050 0412 044b 0020 043d 0435 0020 0432  .P...K. .=.5. .2
+00014990: 044b 0431 0440 0430 043b 0438 0020 0441  .K.1.@.0.;.8. .A
+000149a0: 0447 0451 0442 0020 0434 043b 044f 0020  .G.Q.B. .4.;.O. 
+000149b0: 043d 0430 043b 043e 0433 043e 0432 043e  .=.0.;.>.3.>.2.>
+000149c0: 0433 043e 0020 043e 0442 0447 0451 0442  .3.>. .>.B.G.Q.B
+000149d0: 0430 0800 0000 0006 0000 002e 596f 7520  .0..........You 
+000149e0: 6861 7665 6e27 7420 7365 6c65 6374 6564  haven't selected
+000149f0: 2061 6e20 6163 636f 756e 7420 666f 7220   an account for 
+00014a00: 7461 7820 7265 706f 7274 0700 0000 0954  tax report.....T
+00014a10: 6178 5769 6467 6574 0103 0000 0098 041d  axWidget........
+00014a20: 0435 0432 043e 0437 043c 043e 0436 043d  .5.2.>.7.<.>.6.=
+00014a30: 043e 0020 043e 0431 0440 0430 0431 043e  .>. .>.1.@.0.1.>
+00014a40: 0442 0430 0442 044c 0020 0441 0434 0435  .B.0.B.L. .A.4.5
+00014a50: 043b 043a 0443 002c 0020 0442 002e 043a  .;.:.C.,. .B...:
+00014a60: 002e 0020 043d 0435 0020 0437 0430 0434  ... .=.5. .7.0.4
+00014a70: 0430 043d 0020 0431 0430 043d 043a 0020  .0.=. .1.0.=.:. 
+00014a80: 0434 043b 044f 0020 0438 043d 0432 0435  .4.;.O. .8.=.2.5
+00014a90: 0441 0442 0438 0446 0438 043e 043d 043d  .A.B.8.F.8.>.=.=
+00014aa0: 043e 0433 043e 0020 0441 0447 0451 0442  .>.3.>. .A.G.Q.B
+00014ab0: 0430 003a 0020 0800 0000 0006 0000 003e  .0.:. .........>
+00014ac0: 4361 6e27 7420 7072 6f63 6573 7320 7472  Can't process tr
+00014ad0: 6164 6520 6173 2062 616e 6b20 6973 6e27  ade as bank isn'
+00014ae0: 7420 7365 7420 666f 7220 696e 7665 7374  t set for invest
+00014af0: 6d65 6e74 2061 6363 6f75 6e74 3a20 0700  ment account: ..
+00014b00: 0000 0554 7261 6465 0103 0000 0002 2116  ...Trade......!.
+00014b10: 0800 0000 0006 0000 0001 2307 0000 000b  ..........#.....
+00014b20: 5472 6164 6557 6964 6765 7401 0300 0000  TradeWidget.....
+00014b30: 0804 2104 4704 3504 4208 0000 0000 0600  ..!.G.5.B.......
+00014b40: 0000 0741 6363 6f75 6e74 0700 0000 0b54  ...Account.....T
+00014b50: 7261 6465 5769 6467 6574 0103 0000 0004  radeWidget......
+00014b60: 0426 0411 0800 0000 0006 0000 0005 4173  .&............As
+00014b70: 7365 7407 0000 000b 5472 6164 6557 6964  set.....TradeWid
+00014b80: 6765 7401 0300 0000 2204 1f04 3e04 3a04  get....."...>.:.
+00014b90: 4304 3f04 3a04 3000 2000 2f00 2004 1f04  C.?.:.0. ./. ...
+00014ba0: 4004 3e04 3404 3004 3604 3008 0000 0000  @.>.4.0.6.0.....
+00014bb0: 0600 0000 0a42 7579 202f 2053 656c 6c07  .....Buy / Sell.
+00014bc0: 0000 000b 5472 6164 6557 6964 6765 7401  ....TradeWidget.
+00014bd0: 0300 0000 1404 1404 3004 4204 3000 2f04  ........0.B.0./.
+00014be0: 1204 4004 3504 3c04 4f08 0000 0000 0600  ..@.5.<.O.......
+00014bf0: 0000 0944 6174 652f 5469 6d65 0700 0000  ...Date/Time....
+00014c00: 0b54 7261 6465 5769 6467 6574 0103 0000  .TradeWidget....
+00014c10: 0010 041a 043e 043c 0438 0441 0441 0438  .....>.<.8.A.A.8
+00014c20: 044f 0800 0000 0006 0000 0003 4665 6507  .O..........Fee.
+00014c30: 0000 000b 5472 6164 6557 6964 6765 7401  ....TradeWidget.
+00014c40: 0300 0000 1004 1e04 3f04 3804 4104 3004  ........?.8.A.0.
+00014c50: 3d04 3804 3508 0000 0000 0600 0000 044e  =.8.5..........N
+00014c60: 6f74 6507 0000 000b 5472 6164 6557 6964  ote.....TradeWid
+00014c70: 6765 7401 0300 0000 0804 2604 3504 3d04  get.......&.5.=.
+00014c80: 3008 0000 0000 0600 0000 0550 7269 6365  0..........Price
+00014c90: 0700 0000 0b54 7261 6465 5769 6467 6574  .....TradeWidget
+00014ca0: 0103 0000 000c 041a 043e 043b 002d 0432  .........>.;.-.2
+00014cb0: 043e 0800 0000 0006 0000 0003 5174 7907  .>..........Qty.
+00014cc0: 0000 000b 5472 6164 6557 6964 6765 7401  ....TradeWidget.
+00014cd0: 0300 0000 1a04 1404 3004 4204 3000 2004  ........0.B.0. .
+00014ce0: 4004 3004 4104 4704 3504 4204 3e04 3208  @.0.A.G.5.B.>.2.
+00014cf0: 0000 0000 0600 0000 0a53 6574 746c 656d  .........Settlem
+00014d00: 656e 7407 0000 000b 5472 6164 6557 6964  ent.....TradeWid
+00014d10: 6765 7401 0300 0000 7a04 1a04 3e04 3b04  get.....z...>.;.
+00014d20: 3804 4704 3504 4104 4204 3204 3e00 2004  8.G.5.A.B.2.>. .
+00014d30: 3004 3a04 4204 3804 3204 3000 2004 3d04  0.:.B.8.2.0. .=.
+00014d40: 3504 3404 3e04 4104 4204 3004 4204 3e04  5.4.>.A.B.0.B.>.
+00014d50: 4704 3d04 3e00 2004 3404 3b04 4f00 2004  G.=.>. .4.;.O. .
+00014d60: 3e04 3104 4004 3004 3104 3e04 4204 3a04  >.1.@.0.1.>.B.:.
+00014d70: 3800 2004 3f04 3504 4004 3504 3204 3e04  8. .?.5.@.5.2.>.
+00014d80: 3404 3000 2e00 2004 1404 3004 4204 3000  4.0... ...0.B.0.
+00014d90: 3a00 2008 0000 0000 0600 0000 4041 7373  :. .........@Ass
+00014da0: 6574 2061 6d6f 756e 7420 6973 206e 6f74  et amount is not
+00014db0: 2065 6e6f 7567 6820 666f 7220 6173 7365   enough for asse
+00014dc0: 7420 7472 616e 7366 6572 2070 726f 6365  t transfer proce
+00014dd0: 7373 696e 672e 2044 6174 653a 2007 0000  ssing. Date: ...
+00014de0: 0008 5472 616e 7366 6572 0103 0000 0052  ..Transfer.....R
+00014df0: 0421 043f 0438 0441 0430 043d 0438 0435  .!.?.8.A.0.=.8.5
+00014e00: 0020 0430 043a 0442 0438 0432 0430 0020  . .0.:.B.8.2.0. 
+00014e10: 043d 0435 0020 043d 0430 0439 0434 0435  .=.5. .=.0.9.4.5
+00014e20: 043d 043e 0020 0434 043b 044f 0020 0442  .=.>. .4.;.O. .B
+00014e30: 0440 0430 043d 0441 0444 0435 0440 0430  .@.0.=.A.D.5.@.0
+00014e40: 002e 0800 0000 0006 0000 0028 4173 7365  ...........(Asse
+00014e50: 7420 7769 7468 6472 6177 616c 206e 6f74  t withdrawal not
+00014e60: 2066 6f75 6e64 2066 6f72 2074 7261 6e73   found for trans
+00014e70: 6665 722e 0700 0000 0854 7261 6e73 6665  fer......Transfe
+00014e80: 7201 0300 0000 2e04 1e04 4804 3804 3104  r.........H.8.1.
+00014e90: 3a04 3000 2e00 2004 1a04 4304 4004 4100  :.0... ...C.@.A.
+00014ea0: 2004 4004 3004 3204 3504 3d00 2004 3d04   .@.0.2.5.=. .=.
+00014eb0: 4304 3b04 4e08 0000 0000 0600 0000 1045  C.;.N..........E
+00014ec0: 7272 6f72 2e20 5a65 726f 2072 6174 6507  rror. Zero rate.
+00014ed0: 0000 0008 5472 616e 7366 6572 0103 0000  ....Transfer....
+00014ee0: 0084 041e 0431 0440 0430 0431 043e 0442  .....1.@.0.1.>.B
+00014ef0: 0430 043d 043d 043e 0435 0020 043a 043e  .0.=.=.>.5. .:.>
+00014f00: 043b 0438 0447 0435 0441 0442 0432 043e  .;.8.G.5.A.B.2.>
+00014f10: 0020 043c 0435 043d 044c 0448 0435 002c  . .<.5.=.L.H.5.,
+00014f20: 0020 0447 0435 043c 0020 043a 043e 043b  . .G.5.<. .:.>.;
+00014f30: 0438 0447 0435 0441 0442 0432 043e 0020  .8.G.5.A.B.2.>. 
+00014f40: 0432 0020 0442 0440 0430 043d 0441 0444  .2. .B.@.0.=.A.D
+00014f50: 0435 0440 0435 002e 0020 0414 0430 0442  .5.@.5... ...0.B
+00014f60: 0430 003a 0020 0800 0000 0006 0000 003b  .0.:. .........;
+00014f70: 5072 6f63 6573 7365 6420 6173 7365 7420  Processed asset 
+00014f80: 616d 6f75 6e74 2069 7320 6c65 7373 2074  amount is less t
+00014f90: 6861 6e20 7472 616e 7366 6572 2061 6d6f  han transfer amo
+00014fa0: 756e 742e 2044 6174 653a 2007 0000 0008  unt. Date: .....
+00014fb0: 5472 616e 7366 6572 0103 0000 0002 2116  Transfer......!.
+00014fc0: 0800 0000 0006 0000 0001 2307 0000 000e  ..........#.....
+00014fd0: 5472 616e 7366 6572 5769 6467 6574 0103  TransferWidget..
+00014fe0: 0000 000a 0421 0443 043c 043c 0430 0800  .....!.C.<.<.0..
+00014ff0: 0000 0006 0000 0006 416d 6f75 6e74 0700  ........Amount..
+00015000: 0000 0e54 7261 6e73 6665 7257 6964 6765  ...TransferWidge
+00015010: 7401 0300 0000 0404 2604 1108 0000 0000  t.......&.......
+00015020: 0600 0000 0541 7373 6574 0700 0000 0e54  .....Asset.....T
+00015030: 7261 6e73 6665 7257 6964 6765 7401 0300  ransferWidget...
+00015040: 0000 1404 1404 3004 4204 3000 2f04 1204  ......0.B.0./...
+00015050: 4004 3504 3c04 4f08 0000 0000 0600 0000  @.5.<.O.........
+00015060: 0944 6174 652f 5469 6d65 0700 0000 0e54  .Date/Time.....T
+00015070: 7261 6e73 6665 7257 6964 6765 7401 0300  ransferWidget...
+00015080: 0000 1e04 2004 3004 3704 3c04 3504 4000  .... .0.7.<.5.@.
+00015090: 2004 3a04 3e04 3c04 3804 4104 4104 3804   .:.>.<.8.A.A.8.
+000150a0: 3808 0000 0000 0600 0000 0a46 6565 2061  8..........Fee a
+000150b0: 6d6f 756e 7407 0000 000e 5472 616e 7366  mount.....Transf
+000150c0: 6572 5769 6467 6574 0103 0000 0016 041a  erWidget........
+000150d0: 043e 043c 043c 0438 0441 0441 0438 044f  .>.<.<.8.A.A.8.O
+000150e0: 0020 0441 0800 0000 0006 0000 0008 4665  . .A..........Fe
+000150f0: 6520 6672 6f6d 0700 0000 0e54 7261 6e73  e from.....Trans
+00015100: 6665 7257 6964 6765 7401 0300 0000 0204  ferWidget.......
+00015110: 2108 0000 0000 0600 0000 0446 726f 6d07  !..........From.
+00015120: 0000 000e 5472 616e 7366 6572 5769 6467  ....TransferWidg
+00015130: 6574 0103 0000 0010 041e 043f 0438 0441  et.........?.8.A
+00015140: 0430 043d 0438 0435 0800 0000 0006 0000  .0.=.8.5........
+00015150: 0004 4e6f 7465 0700 0000 0e54 7261 6e73  ..Note.....Trans
+00015160: 6665 7257 6964 6765 7401 0300 0000 0404  ferWidget.......
+00015170: 1d04 3008 0000 0000 0600 0000 0254 6f07  ..0..........To.
+00015180: 0000 000e 5472 616e 7366 6572 5769 6467  ....TransferWidg
+00015190: 6574 0103 0000 000e 041f 0435 0440 0435  et.........5.@.5
+000151a0: 0432 043e 0434 0800 0000 0006 0000 0008  .2.>.4..........
+000151b0: 5472 616e 7366 6572 0700 0000 0e54 7261  Transfer.....Tra
+000151c0: 6e73 6665 7257 6964 6765 7401 0300 0000  nsferWidget.....
+000151d0: 0404 1f04 3e08 0000 0000 0600 0000 0845  ....>..........E
+000151e0: 6e64 2064 6174 6507 0000 000f 5570 6461  nd date.....Upda
+000151f0: 7465 5175 6f74 6573 446c 6701 0300 0000  teQuotesDlg.....
+00015200: 1204 1804 4104 4204 3e04 4704 3d04 3804  ....A.B.>.G.=.8.
+00015210: 3a04 3808 0000 0000 0600 0000 0753 6f75  :.8..........Sou
+00015220: 7263 6573 0700 0000 0f55 7064 6174 6551  rces.....UpdateQ
+00015230: 756f 7465 7344 6c67 0103 0000 0002 0421  uotesDlg.......!
+00015240: 0800 0000 0006 0000 000a 5374 6172 7420  ..........Start 
+00015250: 6461 7465 0700 0000 0f55 7064 6174 6551  date.....UpdateQ
+00015260: 756f 7465 7344 6c67 0103 0000 0028 041e  uotesDlg.....(..
+00015270: 0431 043d 043e 0432 043b 0435 043d 0438  .1.=.>.2.;.5.=.8
+00015280: 0435 0020 043a 043e 0442 0438 0440 043e  .5. .:.>.B.8.@.>
+00015290: 0432 043e 043a 0800 0000 0006 0000 0015  .2.>.:..........
+000152a0: 5570 6461 7465 2061 7373 6574 2773 2071  Update asset's q
+000152b0: 756f 7465 7307 0000 000f 5570 6461 7465  uotes.....Update
+000152c0: 5175 6f74 6573 446c 6701 0300 0000 1400  QuotesDlg.......
+000152d0: 6400 6400 2f00 4d00 4d00 2f00 7900 7900  d.d./.M.M./.y.y.
+000152e0: 7900 7908 0000 0000 0600 0000 0a64 642f  y.y..........dd/
+000152f0: 4d4d 2f79 7979 7907 0000 000f 5570 6461  MM/yyyy.....Upda
+00015300: 7465 5175 6f74 6573 446c 6701 0300 0000  teQuotesDlg.....
+00015310: 5804 1d04 3504 3204 3e04 3704 3c04 3e04  X...5.2.>.7.<.>.
+00015320: 3604 3d04 3e00 2004 3f04 4004 3e04 4704  6.=.>. .?.@.>.G.
+00015330: 3804 4204 3004 4204 4c00 2004 4804 3004  8.B.0.B.L. .H.0.
+00015340: 3104 3b04 3e04 3d00 2004 3e04 4204 4704  1.;.>.=. .>.B.G.
+00015350: 5104 4204 3000 2004 3804 3700 2004 4404  Q.B.0. .8.7. .D.
+00015360: 3004 3904 3b04 3000 2008 0000 0000 0600  0.9.;.0. .......
+00015370: 0000 2543 616e 2774 206c 6f61 6420 7265  ..%Can't load re
+00015380: 706f 7274 2074 656d 706c 6174 6520 6672  port template fr
+00015390: 6f6d 2066 696c 6520 0700 0000 0458 4c53  om file .....XLS
+000153a0: 5801 0300 0000 4404 1d04 3504 3204 3e04  X.....D...5.2.>.
+000153b0: 3704 3c04 3e04 3604 3d04 3e00 2004 4104  7.<.>.6.=.>. .A.
+000153c0: 3e04 4504 4004 3004 3d04 3804 4204 4c00  >.E.@.0.=.8.B.L.
+000153d0: 2004 3e04 4204 4704 5104 4200 2004 3200   .>.B.G.Q.B. .2.
+000153e0: 2004 4404 3004 3904 3b00 2008 0000 0000   .D.0.9.;. .....
+000153f0: 0600 0000 1c43 616e 2774 2073 6176 6520  .....Can't save 
+00015400: 7265 706f 7274 2069 6e74 6f20 6669 6c65  report into file
+00015410: 2007 0000 0004 584c 5358 0103 0000 0044   .....XLSX.....D
+00015420: 041d 0435 0020 0443 043a 0430 0437 0430  ...5. .C.:.0.7.0
+00015430: 043d 0020 0444 043e 0440 043c 0430 0442  .=. .D.>.@.<.0.B
+00015440: 0020 0434 043b 044f 0020 043f 043e 043b  . .4.;.O. .?.>.;
+00015450: 044f 0020 043e 0442 0447 0451 0442 0430  .O. .>.B.G.Q.B.0
+00015460: 003a 0020 0800 0000 0006 0000 0024 466f  .:. .........$Fo
+00015470: 726d 6174 2069 7320 6d69 7373 696e 6720  rmat is missing 
+00015480: 666f 7220 7265 706f 7274 2066 6965 6c64  for report field
+00015490: 3a20 0700 0000 0458 4c53 5801 0300 0000  : .....XLSX.....
+000154a0: 4204 1d04 3500 2004 3704 3004 3404 3004  B...5. .7.0.4.0.
+000154b0: 3d00 2004 4804 3004 3104 3b04 3e04 3d00  =. .H.0.1.;.>.=.
+000154c0: 2004 3404 3b04 4f00 2004 3404 3004 3d04   .4.;.O. .4.0.=.
+000154d0: 3d04 4b04 4500 2004 3e04 4204 4704 5104  =.K.E. .>.B.G.Q.
+000154e0: 4204 3008 0000 0000 0600 0000 1a4e 6f20  B.0..........No 
+000154f0: 7265 706f 7274 2072 6f77 2074 656d 706c  report row templ
+00015500: 6174 6520 7365 7407 0000 0004 584c 5358  ate set.....XLSX
+00015510: 0103 0000 003a 0428 0430 0431 043b 043e  .....:.(.0.1.;.>
+00015520: 043d 0020 0434 043b 044f 0020 0434 0430  .=. .4.;.O. .4.0
+00015530: 043d 043d 044b 0445 0020 043d 0435 0020  .=.=.K.E. .=.5. 
+00015540: 043d 0430 0439 0434 0435 043d 003a 0020  .=.0.9.4.5.=.:. 
+00015550: 0800 0000 0006 0000 001f 5265 706f 7274  ..........Report
+00015560: 2072 6f77 2074 656d 706c 6174 6520 6e6f   row template no
+00015570: 7420 666f 756e 643a 2007 0000 0004 584c  t found: .....XL
+00015580: 5358 0103 0000 0046 041d 0435 0438 0437  SX.....F...5.8.7
+00015590: 0432 0435 0441 0442 043d 0430 044f 0020  .2.5.A.B.=.0.O. 
+000155a0: 0441 0442 0440 043e 043a 0430 0020 0444  .A.B.@.>.:.0. .D
+000155b0: 043e 0440 043c 0430 0442 0438 0440 043e  .>.@.<.0.B.8.@.>
+000155c0: 0432 0430 043d 0438 044f 003a 0020 0800  .2.0.=.8.O.:. ..
+000155d0: 0000 0006 0000 001c 556e 7265 636f 676e  ........Unrecogn
+000155e0: 697a 6564 2066 6f72 6d61 7420 7374 7269  ized format stri
+000155f0: 6e67 3a20 0700 0000 0458 4c53 5801 8800  ng: .....XLSX...
+00015600: 0000 0d11 01fd 290b ff14 0204 fd2c 0a13  ......)......,..
```

### Comparing `jal-2023.4.5/jal/net/downloader.py` & `jal-2023.4.6/jal/net/downloader.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/net/helpers.py` & `jal-2023.4.6/jal/net/helpers.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/pypi_description.md` & `jal-2023.4.6/jal/pypi_description.md`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/reports/category.py` & `jal-2023.4.6/jal/reports/category.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/reports/deals.py` & `jal-2023.4.6/jal/reports/deals.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/reports/holdings.py` & `jal-2023.4.6/jal/reports/holdings.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/reports/income_spending.py` & `jal-2023.4.6/jal/reports/income_spending.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/reports/peer.py` & `jal-2023.4.6/jal/reports/peer.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/reports/profit_loss.py` & `jal-2023.4.6/jal/reports/profit_loss.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/reports/reports.py` & `jal-2023.4.6/jal/reports/reports.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/reports/tag.py` & `jal-2023.4.6/jal/reports/tag.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/ui/reports/ui_category_report.py` & `jal-2023.4.6/jal/ui/reports/ui_category_report.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 ################################################################################
 ## Form generated from reading UI file 'category_report.ui'
 ##
-## Created by: Qt User Interface Compiler version 6.4.3
+## Created by: Qt User Interface Compiler version 6.5.0
 ##
 ## WARNING! All changes made in this file will be lost when recompiling UI file!
 ################################################################################
 
 from PySide6.QtCore import (QCoreApplication, QDate, QDateTime, QLocale,
     QMetaObject, QObject, QPoint, QRect,
     QSize, QTime, QUrl, Qt)
```

### Comparing `jal-2023.4.5/jal/ui/reports/ui_deals_report.py` & `jal-2023.4.6/jal/ui/reports/ui_deals_report.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 ################################################################################
 ## Form generated from reading UI file 'deals_report.ui'
 ##
-## Created by: Qt User Interface Compiler version 6.4.3
+## Created by: Qt User Interface Compiler version 6.5.0
 ##
 ## WARNING! All changes made in this file will be lost when recompiling UI file!
 ################################################################################
 
 from PySide6.QtCore import (QCoreApplication, QDate, QDateTime, QLocale,
     QMetaObject, QObject, QPoint, QRect,
     QSize, QTime, QUrl, Qt)
```

### Comparing `jal-2023.4.5/jal/ui/reports/ui_holdings_report.py` & `jal-2023.4.6/jal/ui/reports/ui_holdings_report.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 ################################################################################
 ## Form generated from reading UI file 'holdings_report.ui'
 ##
-## Created by: Qt User Interface Compiler version 6.4.3
+## Created by: Qt User Interface Compiler version 6.5.0
 ##
 ## WARNING! All changes made in this file will be lost when recompiling UI file!
 ################################################################################
 
 from PySide6.QtCore import (QCoreApplication, QDate, QDateTime, QLocale,
     QMetaObject, QObject, QPoint, QRect,
     QSize, QTime, QUrl, Qt)
```

### Comparing `jal-2023.4.5/jal/ui/reports/ui_income_spending_report.py` & `jal-2023.4.6/jal/ui/reports/ui_income_spending_report.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 ################################################################################
 ## Form generated from reading UI file 'income_spending_report.ui'
 ##
-## Created by: Qt User Interface Compiler version 6.4.3
+## Created by: Qt User Interface Compiler version 6.5.0
 ##
 ## WARNING! All changes made in this file will be lost when recompiling UI file!
 ################################################################################
 
 from PySide6.QtCore import (QCoreApplication, QDate, QDateTime, QLocale,
     QMetaObject, QObject, QPoint, QRect,
     QSize, QTime, QUrl, Qt)
```

### Comparing `jal-2023.4.5/jal/ui/reports/ui_peer_report.py` & `jal-2023.4.6/jal/ui/reports/ui_peer_report.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 ################################################################################
 ## Form generated from reading UI file 'peer_report.ui'
 ##
-## Created by: Qt User Interface Compiler version 6.4.3
+## Created by: Qt User Interface Compiler version 6.5.0
 ##
 ## WARNING! All changes made in this file will be lost when recompiling UI file!
 ################################################################################
 
 from PySide6.QtCore import (QCoreApplication, QDate, QDateTime, QLocale,
     QMetaObject, QObject, QPoint, QRect,
     QSize, QTime, QUrl, Qt)
```

### Comparing `jal-2023.4.5/jal/ui/reports/ui_profit_loss_report.py` & `jal-2023.4.6/jal/ui/reports/ui_profit_loss_report.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 ################################################################################
 ## Form generated from reading UI file 'profit_loss_report.ui'
 ##
-## Created by: Qt User Interface Compiler version 6.4.3
+## Created by: Qt User Interface Compiler version 6.5.0
 ##
 ## WARNING! All changes made in this file will be lost when recompiling UI file!
 ################################################################################
 
 from PySide6.QtCore import (QCoreApplication, QDate, QDateTime, QLocale,
     QMetaObject, QObject, QPoint, QRect,
     QSize, QTime, QUrl, Qt)
```

### Comparing `jal-2023.4.5/jal/ui/reports/ui_tag_report.py` & `jal-2023.4.6/jal/ui/reports/ui_tag_report.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 ################################################################################
 ## Form generated from reading UI file 'tag_report.ui'
 ##
-## Created by: Qt User Interface Compiler version 6.4.3
+## Created by: Qt User Interface Compiler version 6.5.0
 ##
 ## WARNING! All changes made in this file will be lost when recompiling UI file!
 ################################################################################
 
 from PySide6.QtCore import (QCoreApplication, QDate, QDateTime, QLocale,
     QMetaObject, QObject, QPoint, QRect,
     QSize, QTime, QUrl, Qt)
```

### Comparing `jal-2023.4.5/jal/ui/reports/ui_tax_estimation.py` & `jal-2023.4.6/jal/ui/reports/ui_tax_estimation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 ################################################################################
 ## Form generated from reading UI file 'tax_estimation.ui'
 ##
-## Created by: Qt User Interface Compiler version 6.4.3
+## Created by: Qt User Interface Compiler version 6.5.0
 ##
 ## WARNING! All changes made in this file will be lost when recompiling UI file!
 ################################################################################
 
 from PySide6.QtCore import (QCoreApplication, QDate, QDateTime, QLocale,
     QMetaObject, QObject, QPoint, QRect,
     QSize, QTime, QUrl, Qt)
```

### Comparing `jal-2023.4.5/jal/ui/ui_asset_dlg.py` & `jal-2023.4.6/jal/ui/ui_asset_dlg.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 ################################################################################
 ## Form generated from reading UI file 'asset_dlg.ui'
 ##
-## Created by: Qt User Interface Compiler version 6.4.3
+## Created by: Qt User Interface Compiler version 6.5.0
 ##
 ## WARNING! All changes made in this file will be lost when recompiling UI file!
 ################################################################################
 
 from PySide6.QtCore import (QCoreApplication, QDate, QDateTime, QLocale,
     QMetaObject, QObject, QPoint, QRect,
     QSize, QTime, QUrl, Qt)
```

### Comparing `jal-2023.4.5/jal/ui/ui_flow_export_widget.py` & `jal-2023.4.6/jal/ui/ui_flow_export_widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 ################################################################################
 ## Form generated from reading UI file 'flow_export_widget.ui'
 ##
-## Created by: Qt User Interface Compiler version 6.4.3
+## Created by: Qt User Interface Compiler version 6.5.0
 ##
 ## WARNING! All changes made in this file will be lost when recompiling UI file!
 ################################################################################
 
 from PySide6.QtCore import (QCoreApplication, QDate, QDateTime, QLocale,
     QMetaObject, QObject, QPoint, QRect,
     QSize, QTime, QUrl, Qt)
```

### Comparing `jal-2023.4.5/jal/ui/ui_login_fns_dlg.py` & `jal-2023.4.6/jal/ui/ui_login_fns_dlg.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 ################################################################################
 ## Form generated from reading UI file 'login_fns_dlg.ui'
 ##
-## Created by: Qt User Interface Compiler version 6.4.3
+## Created by: Qt User Interface Compiler version 6.5.0
 ##
 ## WARNING! All changes made in this file will be lost when recompiling UI file!
 ################################################################################
 
 from PySide6.QtCore import (QCoreApplication, QDate, QDateTime, QLocale,
     QMetaObject, QObject, QPoint, QRect,
     QSize, QTime, QUrl, Qt)
```

### Comparing `jal-2023.4.5/jal/ui/ui_main_window.py` & `jal-2023.4.6/jal/ui/ui_main_window.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 ################################################################################
 ## Form generated from reading UI file 'main_window.ui'
 ##
-## Created by: Qt User Interface Compiler version 6.4.3
+## Created by: Qt User Interface Compiler version 6.5.0
 ##
 ## WARNING! All changes made in this file will be lost when recompiling UI file!
 ################################################################################
 
 from PySide6.QtCore import (QCoreApplication, QDate, QDateTime, QLocale,
     QMetaObject, QObject, QPoint, QRect,
     QSize, QTime, QUrl, Qt)
```

### Comparing `jal-2023.4.5/jal/ui/ui_operations_widget.py` & `jal-2023.4.6/jal/ui/ui_operations_widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 ################################################################################
 ## Form generated from reading UI file 'operations_widget.ui'
 ##
-## Created by: Qt User Interface Compiler version 6.4.3
+## Created by: Qt User Interface Compiler version 6.5.0
 ##
 ## WARNING! All changes made in this file will be lost when recompiling UI file!
 ################################################################################
 
 from PySide6.QtCore import (QCoreApplication, QDate, QDateTime, QLocale,
     QMetaObject, QObject, QPoint, QRect,
     QSize, QTime, QUrl, Qt)
```

### Comparing `jal-2023.4.5/jal/ui/ui_rebuild_window.py` & `jal-2023.4.6/jal/ui/ui_rebuild_window.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 ################################################################################
 ## Form generated from reading UI file 'rebuild_window.ui'
 ##
-## Created by: Qt User Interface Compiler version 6.4.3
+## Created by: Qt User Interface Compiler version 6.5.0
 ##
 ## WARNING! All changes made in this file will be lost when recompiling UI file!
 ################################################################################
 
 from PySide6.QtCore import (QCoreApplication, QDate, QDateTime, QLocale,
     QMetaObject, QObject, QPoint, QRect,
     QSize, QTime, QUrl, Qt)
```

### Comparing `jal-2023.4.5/jal/ui/ui_reference_data_dlg.py` & `jal-2023.4.6/jal/ui/ui_reference_data_dlg.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 ################################################################################
 ## Form generated from reading UI file 'reference_data_dlg.ui'
 ##
-## Created by: Qt User Interface Compiler version 6.4.3
+## Created by: Qt User Interface Compiler version 6.5.0
 ##
 ## WARNING! All changes made in this file will be lost when recompiling UI file!
 ################################################################################
 
 from PySide6.QtCore import (QCoreApplication, QDate, QDateTime, QLocale,
     QMetaObject, QObject, QPoint, QRect,
     QSize, QTime, QUrl, Qt)
```

### Comparing `jal-2023.4.5/jal/ui/ui_select_account_dlg.py` & `jal-2023.4.6/jal/ui/ui_select_account_dlg.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 ################################################################################
 ## Form generated from reading UI file 'select_account_dlg.ui'
 ##
-## Created by: Qt User Interface Compiler version 6.4.3
+## Created by: Qt User Interface Compiler version 6.5.0
 ##
 ## WARNING! All changes made in this file will be lost when recompiling UI file!
 ################################################################################
 
 from PySide6.QtCore import (QCoreApplication, QDate, QDateTime, QLocale,
     QMetaObject, QObject, QPoint, QRect,
     QSize, QTime, QUrl, Qt)
```

### Comparing `jal-2023.4.5/jal/ui/ui_select_reference_dlg.py` & `jal-2023.4.6/jal/ui/ui_select_reference_dlg.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 ################################################################################
 ## Form generated from reading UI file 'select_reference_dlg.ui'
 ##
-## Created by: Qt User Interface Compiler version 6.4.3
+## Created by: Qt User Interface Compiler version 6.5.0
 ##
 ## WARNING! All changes made in this file will be lost when recompiling UI file!
 ################################################################################
 
 from PySide6.QtCore import (QCoreApplication, QDate, QDateTime, QLocale,
     QMetaObject, QObject, QPoint, QRect,
     QSize, QTime, QUrl, Qt)
```

### Comparing `jal-2023.4.5/jal/ui/ui_slip_import_dlg.py` & `jal-2023.4.6/jal/ui/ui_slip_import_dlg.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 ################################################################################
 ## Form generated from reading UI file 'slip_import_dlg.ui'
 ##
-## Created by: Qt User Interface Compiler version 6.4.3
+## Created by: Qt User Interface Compiler version 6.5.0
 ##
 ## WARNING! All changes made in this file will be lost when recompiling UI file!
 ################################################################################
 
 from PySide6.QtCore import (QCoreApplication, QDate, QDateTime, QLocale,
     QMetaObject, QObject, QPoint, QRect,
     QSize, QTime, QUrl, Qt)
```

### Comparing `jal-2023.4.5/jal/ui/ui_tax_export_widget.py` & `jal-2023.4.6/jal/ui/ui_tax_export_widget.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 ################################################################################
 ## Form generated from reading UI file 'tax_export_widget.ui'
 ##
-## Created by: Qt User Interface Compiler version 6.4.3
+## Created by: Qt User Interface Compiler version 6.5.0
 ##
 ## WARNING! All changes made in this file will be lost when recompiling UI file!
 ################################################################################
 
 from PySide6.QtCore import (QCoreApplication, QDate, QDateTime, QLocale,
     QMetaObject, QObject, QPoint, QRect,
     QSize, QTime, QUrl, Qt)
```

### Comparing `jal-2023.4.5/jal/ui/ui_update_quotes_window.py` & `jal-2023.4.6/jal/ui/ui_update_quotes_window.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 ################################################################################
 ## Form generated from reading UI file 'quotes_update.ui'
 ##
-## Created by: Qt User Interface Compiler version 6.4.3
+## Created by: Qt User Interface Compiler version 6.5.0
 ##
 ## WARNING! All changes made in this file will be lost when recompiling UI file!
 ################################################################################
 
 from PySide6.QtCore import (QCoreApplication, QDate, QDateTime, QLocale,
     QMetaObject, QObject, QPoint, QRect,
     QSize, QTime, QUrl, Qt)
```

### Comparing `jal-2023.4.5/jal/updates/jal_delta_10.sql` & `jal-2023.4.6/jal/updates/jal_delta_10.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/updates/jal_delta_11.sql` & `jal-2023.4.6/jal/updates/jal_delta_11.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/updates/jal_delta_12.sql` & `jal-2023.4.6/jal/updates/jal_delta_12.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/updates/jal_delta_13.sql` & `jal-2023.4.6/jal/updates/jal_delta_13.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/updates/jal_delta_14.sql` & `jal-2023.4.6/jal/updates/jal_delta_14.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/updates/jal_delta_15.sql` & `jal-2023.4.6/jal/updates/jal_delta_15.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/updates/jal_delta_16.sql` & `jal-2023.4.6/jal/updates/jal_delta_16.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/updates/jal_delta_17.sql` & `jal-2023.4.6/jal/updates/jal_delta_17.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/updates/jal_delta_18.sql` & `jal-2023.4.6/jal/updates/jal_delta_18.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/updates/jal_delta_19.sql` & `jal-2023.4.6/jal/updates/jal_delta_19.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/updates/jal_delta_20.sql` & `jal-2023.4.6/jal/updates/jal_delta_20.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/updates/jal_delta_21.sql` & `jal-2023.4.6/jal/updates/jal_delta_21.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/updates/jal_delta_22.sql` & `jal-2023.4.6/jal/updates/jal_delta_22.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/updates/jal_delta_23.sql` & `jal-2023.4.6/jal/updates/jal_delta_23.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/updates/jal_delta_25.sql` & `jal-2023.4.6/jal/updates/jal_delta_25.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/updates/jal_delta_26.sql` & `jal-2023.4.6/jal/updates/jal_delta_26.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/updates/jal_delta_27.sql` & `jal-2023.4.6/jal/updates/jal_delta_27.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/updates/jal_delta_28.sql` & `jal-2023.4.6/jal/updates/jal_delta_28.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/updates/jal_delta_29.sql` & `jal-2023.4.6/jal/updates/jal_delta_29.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/updates/jal_delta_30.sql` & `jal-2023.4.6/jal/updates/jal_delta_30.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/updates/jal_delta_31.sql` & `jal-2023.4.6/jal/updates/jal_delta_31.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/updates/jal_delta_32.sql` & `jal-2023.4.6/jal/updates/jal_delta_32.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/updates/jal_delta_33.sql` & `jal-2023.4.6/jal/updates/jal_delta_33.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/updates/jal_delta_34.sql` & `jal-2023.4.6/jal/updates/jal_delta_34.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/updates/jal_delta_35.sql` & `jal-2023.4.6/jal/updates/jal_delta_35.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/updates/jal_delta_36.sql` & `jal-2023.4.6/jal/updates/jal_delta_36.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/updates/jal_delta_37.sql` & `jal-2023.4.6/jal/updates/jal_delta_37.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/updates/jal_delta_38.sql` & `jal-2023.4.6/jal/updates/jal_delta_38.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/updates/jal_delta_40.sql` & `jal-2023.4.6/jal/updates/jal_delta_40.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/updates/jal_delta_41.sql` & `jal-2023.4.6/jal/updates/jal_delta_41.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/updates/jal_delta_42.sql` & `jal-2023.4.6/jal/updates/jal_delta_42.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/updates/jal_delta_43.sql` & `jal-2023.4.6/jal/updates/jal_delta_43.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/updates/jal_delta_44.sql` & `jal-2023.4.6/jal/updates/jal_delta_44.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/widgets/abstract_operation_details.py` & `jal-2023.4.6/jal/widgets/abstract_operation_details.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from jal.db.db import JalModel
 
 
 class AbstractOperationDetails(QWidget):
     dbUpdated = Signal()
 
     def __init__(self, parent=None):
-        QWidget.__init__(self, parent)
+        super().__init__(parent)
         self.model = None
         self.table_name = ''
         self.mapper = None
         self.modified = False
         self.name = "N/A"
         self.operation_type = None
```

### Comparing `jal-2023.4.5/jal/widgets/account_select.py` & `jal-2023.4.6/jal/widgets/account_select.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ########################################################################################################################
 #  UI Button to choose accounts
 ########################################################################################################################
 class AccountButton(QPushButton):
     changed = Signal(int)
 
     def __init__(self, parent):
-        QPushButton.__init__(self, parent)
+        super().__init__(parent=parent)
         self.p_account_id = 0
 
         self.Menu = QMenu(self)
         self.Menu.addAction(self.tr("Choose account"), self.ChooseAccount)
         self.Menu.addAction(self.tr("Any account"), self.ClearAccount)
         self.setMenu(self.Menu)
 
@@ -89,15 +89,15 @@
 
 
 # ----------------------------------------------------------------------------------------------------------------------
 class CurrencyComboBox(QComboBox):
     changed = Signal(int)
 
     def __init__(self, parent):
-        QComboBox.__init__(self, parent)
+        super().__init__(parent=parent)
         self.p_selected_id = 0
         self.model = None
         self.activated.connect(self.OnUserSelection)
 
         self.model = JalModel(self, "currencies")
         self.model.select()
         self.setModel(self.model)
@@ -129,16 +129,16 @@
 
 
 # ----------------------------------------------------------------------------------------------------------------------
 class OptionalCurrencyComboBox(QWidget):
     changed = Signal()
     name_updated = Signal(str)
 
-    def __init__(self, parent):
-        QWidget.__init__(self, parent)
+    def __init__(self, parent=None):
+        super().__init__(parent=parent)
         self._id = 0
 
         self.layout = QHBoxLayout()
         self.layout.setContentsMargins(0, 0, 0, 0)
         self.null_flag = QCheckBox(parent)
         self.null_flag.setChecked(False)
         self.null_flag.setText(self.tr("Currency"))
```

### Comparing `jal-2023.4.5/jal/widgets/asset_dialog.py` & `jal-2023.4.6/jal/widgets/asset_dialog.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,23 @@
+import logging
 from datetime import datetime
 from decimal import Decimal
 from PySide6.QtCore import Qt, Property, QDateTime, QTimeZone, QLocale
 from PySide6.QtSql import QSqlRelation, QSqlRelationalDelegate
 from PySide6.QtWidgets import QDialog, QDataWidgetMapper, QStyledItemDelegate, QComboBox, QLineEdit
 from jal.ui.ui_asset_dlg import Ui_AssetDialog
 from jal.constants import PredefinedAsset, AssetData
 from jal.db.helpers import load_icon, localize_decimal
 from jal.widgets.delegates import DateTimeEditWithReset, BoolDelegate
 from jal.db.reference_models import AbstractReferenceListModel
 
 
 class AssetsListModel(AbstractReferenceListModel):
     def __init__(self, table, parent_view):
-        AbstractReferenceListModel.__init__(self, table, parent_view)
+        super().__init__(table=table, parent_view=parent_view)
         self._columns = [("id", ''),
                          ("type_id", 'Asset type'),
                          ("full_name", self.tr("Asset name")),
                          ("isin", self.tr("ISIN")),
                          ("country_id", self.tr("Country")),
                          ("base_asset", self.tr("Base asset"))]
 
@@ -86,24 +87,30 @@
         assert self._model.insertRows(0, 1)
         self._model.setRecord(0, new_record)
         self._mapper.toLast()
         self._symbols_model.filterBy("asset_id", self._asset_id)
         self._data_model.filterBy("asset_id", self._asset_id)
 
     def accept(self) -> None:
-        if not self._model.submitAll():
+        self._model.database().transaction()
+        try:
+            if not self._model.submitAll():
+                raise RuntimeError(self.tr("Asset submit failed: ") + self._model.lastError().text())
+            asset_id = self._model.data(self._model.index(0, self._model.fieldIndex("id")))
+            if asset_id is None:  # we just have saved new asset record and need last inserted id
+                asset_id = self._model.last_insert_id()
+            for model in [self._data_model, self._symbols_model]:
+                for row in range(model.rowCount()):
+                    model.setData(model.index(row, model.fieldIndex("asset_id")), asset_id)
+                if not model.submitAll():
+                    raise RuntimeError(self.tr("Asset details submit failed: ") + model.lastError().text())
+        except Exception as e:
+            self._model.database().rollback()
+            logging.fatal(e)
             return
-        asset_id = self._model.data(self._model.index(0, self._model.fieldIndex("id")))
-        if asset_id is None:  # we just have saved new asset record and need last inserted id
-            asset_id = self._model.query().lastInsertId()
-        for model in [self._data_model, self._symbols_model]:
-            for row in range(model.rowCount()):
-                model.setData(model.index(row, model.fieldIndex("asset_id")), asset_id)
-            if not model.submitAll():
-                return
         self._asset_id = asset_id
         super().accept()
 
     def reject(self) -> None:
         for model in [self._data_model, self._symbols_model, self._model]:
             model.revertAll()
         super().reject()
@@ -137,15 +144,15 @@
         idx = self.ui.DataTable.selectionModel().selection().indexes()
         current_index = idx[0] if idx else self._data_model.index(0, 0)
         self._data_model.removeElement(current_index)
 
 
 class SymbolsListModel(AbstractReferenceListModel):
     def __init__(self, table, parent_view):
-        AbstractReferenceListModel.__init__(self, table, parent_view)
+        super().__init__(table=table, parent_view=parent_view)
         self._columns = [("id", ''),
                          ("asset_id", ''),
                          ("symbol", self.tr("Symbol")),
                          ("currency_id", self.tr("Currency")),
                          ("description", self.tr("Description")),
                          ("quote_source", self.tr("Quotes")),
                          ("active", self.tr("Act."))]
@@ -168,15 +175,15 @@
         self._view.setItemDelegateForColumn(self.fieldIndex("active"), self._bool_delegate)
 
 
 # Delegate class that allows to choose data type in 'key_field' and edit data in 'value_field' (both are integer
 # indices). Editors are created based on data type associated with 'key_field' via self.types dictionary
 class DataDelegate(QStyledItemDelegate):    # Code doubles with pieces from delegates.py
     def __init__(self, key_field, value_field, parent=None):
-        QStyledItemDelegate.__init__(self, parent)
+        super().__init__(parent=parent)
         self._key = key_field
         self._value = value_field
         self.types = {
             AssetData.RegistrationCode: (self.tr("reg.code"), "str"),
             AssetData.ExpiryDate: (self.tr("expiry"), "date"),
             AssetData.PrincipalValue: (self.tr("principal"), "float")
         }
@@ -259,15 +266,15 @@
                 assert False, f"Unknown data type '{self.types[type_idx][1]}' in DataDelegate.setModelData()"
         else:
             assert False, f"Delegate DataDelegate.setModelData() called for not-initialized column {index.column()}"
 
 
 class ExtraDataModel(AbstractReferenceListModel):
     def __init__(self, table, parent_view):
-        AbstractReferenceListModel.__init__(self, table, parent_view)
+        super().__init__(table=table, parent_view=parent_view)
         self._columns = [("id", ''),
                          ("asset_id", ''),
                          ("datatype", self.tr("Property")),
                          ("value", self.tr("Value"))]
         self._default_name = "datatype"
         self._sort_by = "datatype"
         self._hidden = ["id", "asset_id"]
```

### Comparing `jal-2023.4.5/jal/widgets/corporate_action_widget.py` & `jal-2023.4.6/jal/widgets/corporate_action_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,24 +12,24 @@
 from jal.db.helpers import load_icon
 from jal.db.operations import LedgerTransaction
 
 
 # ----------------------------------------------------------------------------------------------------------------------
 class CorporateActionWidgetDelegate(WidgetMapperDelegateBase):
     def __init__(self, parent=None):
-        WidgetMapperDelegateBase.__init__(self, parent)
+        super().__init__(parent=parent)
         self.delegates = {'timestamp': self.timestamp_delegate,
                           'asset_id': self.symbol_delegate,
                           'qty': self.decimal_delegate}
 
 
 # ----------------------------------------------------------------------------------------------------------------------
 class CorporateActionWidget(AbstractOperationDetails):
     def __init__(self, parent=None):
-        AbstractOperationDetails.__init__(self, parent)
+        super().__init__(parent=parent)
         self.name = self.tr("Corporate Action")
         self.operation_type = LedgerTransaction.CorporateAction
         self.combo_model = None
 
         self.asset_delegate = AssetSelectorDelegate()
         self.float_delegate = FloatDelegate(2)
         self.percent_delegate = FloatDelegate(2, percent=True)
@@ -162,24 +162,28 @@
         selection = self.results_table.selectionModel().selection().indexes()
         for idx in selection:
             self.results_model.removeRow(idx.row())
             self.onDataChange(idx, idx, None)
 
     @Slot()
     def saveChanges(self):
-        if not self.model.submitAll():
-            logging.fatal(self.tr("Operation submit failed: ") + self.model.lastError().text())
-            return
-        oid = self.model.data(self.model.index(0, self.model.fieldIndex("id")))
-        if oid is None:  # we just have saved new action record and need last inserted id
-            oid = self.model.query().lastInsertId()
-        for row in range(self.results_model.rowCount()):
-            self.results_model.setData(self.results_model.index(row, self.results_model.fieldIndex("action_id")), oid)
-        if not self.results_model.submitAll():
-            logging.fatal(self.tr("Operation details submit failed: ") + self.results_model.lastError().text())
+        self.model.database().transaction()
+        try:
+            if not self.model.submitAll():
+                raise RuntimeError(self.tr("Operation submit failed: ") + self.model.lastError().text())
+            oid = self.model.data(self.model.index(0, self.model.fieldIndex("id")))
+            if oid is None:  # we just have saved new action record and need last inserted id
+                oid = self.model.last_insert_id()
+            for row in range(self.results_model.rowCount()):
+                self.results_model.setData(self.results_model.index(row, self.results_model.fieldIndex("action_id")), oid)
+            if not self.results_model.submitAll():
+                raise RuntimeError(self.tr("Operation details submit failed: ") + self.results_model.lastError().text())
+        except Exception as e:
+            self.model.database().rollback()
+            logging.fatal(e)
             return
         self.modified = False
         self.commit_button.setEnabled(False)
         self.revert_button.setEnabled(False)
         self.dbUpdated.emit()
 
     @Slot()
```

### Comparing `jal-2023.4.5/jal/widgets/custom/date_range_selector.py` & `jal-2023.4.6/jal/widgets/custom/date_range_selector.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 
 ITEM_NAME = 0
 ITEM_METHOD = 1
 # ----------------------------------------------------------------------------------------------------------------------
 class DateRangeSelector(QWidget):
     changed = Signal(int, int)   # emits signal when one or both dates were changed, "from" and "to" timestamps are sent
 
-    def __init__(self, parent):
-        QWidget.__init__(self, parent)
+    def __init__(self, parent=None):
+        super().__init__(parent=parent)
         self.report_ranges = {
             'week': (self.tr("Week"), ManipulateDate.PreviousWeek),
             'month': (self.tr("Month"), ManipulateDate.PreviousMonth),
             'quarter': (self.tr("Quarter"), ManipulateDate.PreviousQuarter),
             'year': (self.tr("Year"), ManipulateDate.PreviousYear),
             'QTD': (self.tr("Quarter to date"), ManipulateDate.QuarterToDate),
             'YTD': (self.tr("Year to date"), ManipulateDate.YearToDate),
```

### Comparing `jal-2023.4.5/jal/widgets/custom/db_lookup_combobox.py` & `jal-2023.4.6/jal/widgets/custom/db_lookup_combobox.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from jal.db.db import JalModel
 
 
 # Combobox to lookup in db tables:
 # It is mandatory to set up 'table', 'key_field' and 'field' properties at design time
 class DbLookupComboBox(QComboBox):
     def __init__(self, parent=None):
-        QComboBox.__init__(self, parent)
+        super().__init__(parent=parent)
         self._model = None
         self._table = ''
         self._key_field = ''
         self._field = ''
         self._selected_id = -1
 
     def getKey(self):
```

### Comparing `jal-2023.4.5/jal/widgets/custom/log_viewer.py` & `jal-2023.4.6/jal/widgets/custom/log_viewer.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/widgets/delegates.py` & `jal-2023.4.6/jal/widgets/delegates.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 
 # ----------------------------------------------------------------------------------------------------------------------
 # Base class to provide different delegates for WidgetDataMappers in operations widgets
 # Separate delegate class is subclassed for every operation widget with own definition of self.delegates for columns
 class WidgetMapperDelegateBase(QStyledItemDelegate):
     def __init__(self, parent=None):
-        QStyledItemDelegate.__init__(self, parent)
+        super().__init__(parent=parent)
 
         self.timestamp_delegate = TimestampDelegate()
         self.decimal_delegate = FloatDelegate(2)
         self.symbol_delegate = SymbolDelegate()
         self.default = QStyledItemDelegate()
 
         self.delegates = {}
@@ -62,15 +62,15 @@
         super().keyPressEvent(event)
 
 
 # ----------------------------------------------------------------------------------------------------------------------
 # Delegate to convert timestamp from unix-time to QDateTime and display it according to the given format
 class TimestampDelegate(QStyledItemDelegate):
     def __init__(self, display_format='%d/%m/%Y %H:%M:%S', parent=None):
-        QStyledItemDelegate.__init__(self, parent)
+        super().__init__(parent=parent)
         self._parent = parent
         self._format = display_format
 
     def displayText(self, value, locale):
         if isinstance(value, str):  # int value comes here in form of string in case of SQL aggregate function results
             value = int(value)
         text = datetime.utcfromtimestamp(value).strftime(self._format) if value else ''
@@ -118,15 +118,15 @@
 # 'percent' - multiply values by 100 in order to display percents
 # 'empty_zero' - display nothing instead of number 0
 class FloatDelegate(QStyledItemDelegate):
     DEFAULT_TOLERANCE = 6
 
     def __init__(self, tolerance=None, allow_tail=True, colors=False, percent=False, empty_zero=False, parent=None):
         self._parent = parent
-        QStyledItemDelegate.__init__(self, parent)
+        super().__init__(parent=parent)
         try:
             self._tolerance = int(tolerance)
         except (ValueError, TypeError):
             self._tolerance = self.DEFAULT_TOLERANCE
         self._allow_tail = allow_tail
         self._colors = colors
         self._color = None
@@ -207,15 +207,15 @@
 
 # ----------------------------------------------------------------------------------------------------------------------
 # Display '*' if true and empty cell if false
 # Toggle True/False by mouse click
 class BoolDelegate(QStyledItemDelegate):
     def __init__(self, parent=None):
         self._parent = parent
-        QStyledItemDelegate.__init__(self, parent)
+        super().__init__(parent=parent)
 
     def displayText(self, value, locale):
         if value:
             return ' ☒ '
         else:
             return ' ☐ '
 
@@ -245,15 +245,15 @@
 
 
 # ----------------------------------------------------------------------------------------------------------------------
 # QTreeView doesn't draw grid lines and have no normal method to implement it
 # So the purpose of this delegate is solely to draw dotted box around report cell
 class GridLinesDelegate(QStyledItemDelegate):
     def __init__(self, parent=None):
-        QStyledItemDelegate.__init__(self, parent)
+        super().__init__(parent=parent)
 
     def paint(self, painter, option, index):
         painter.save()
         pen = painter.pen()
         pen.setWidth(1)
         pen.setStyle(Qt.DotLine)
         pen.setColor(Qt.GlobalColor.lightGray)
@@ -263,15 +263,15 @@
         super().paint(painter, option, index)
 
 
 # -----------------------------------------------------------------------------------------------------------------------
 # Base class for lookup delegate that allows Asset, Peer, Category and Tag selection
 class LookupSelectorDelegate(QStyledItemDelegate):
     def __init__(self, parent=None):
-        QStyledItemDelegate.__init__(self, parent)
+        super().__init__(parent=parent)
         self._table = ''
         self._field = ''
         self._selector = None
 
     def displayText(self, value, locale):
         item_name = JalModel(self, self._table).get_value(self._field, "id", value)
         if item_name is None:
@@ -292,43 +292,43 @@
 
     def setModelData(self, editor, model, index):
         model.setData(index, editor.selected_id)
 
 
 class CategorySelectorDelegate(LookupSelectorDelegate):
     def __init__(self, parent=None):
-        LookupSelectorDelegate.__init__(self, parent)
+        super().__init__(parent=parent)
         self._table = "categories"
         self._field = "name"
 
     def createSelector(self, parent) -> None:
         self._selector = CategorySelector(parent)
 
 
 class TagSelectorDelegate(LookupSelectorDelegate):
     def __init__(self, parent=None):
-        LookupSelectorDelegate.__init__(self, parent)
+        super().__init__(parent=parent)
         self._table = "tags"
         self._field = "tag"
 
     def createSelector(self, parent) -> None:
         self._selector = TagSelector(parent)
 
 
 class PeerSelectorDelegate(LookupSelectorDelegate):
     def __init__(self, parent=None):
-        LookupSelectorDelegate.__init__(self, parent)
+        super().__init__(parent=parent)
         self._table = "agents"
         self._field = "name"
 
     def createSelector(self, parent) -> None:
         self._selector = PeerSelector(parent)
 
 
 class AssetSelectorDelegate(LookupSelectorDelegate):
     def __init__(self, parent=None):
-        LookupSelectorDelegate.__init__(self, parent)
+        super().__init__(parent=parent)
         self._table = "assets_ext"
         self._field = "symbol"
 
     def createSelector(self, parent) -> None:
         self._selector = AssetSelector(parent)
```

### Comparing `jal-2023.4.5/jal/widgets/dividend_widget.py` & `jal-2023.4.6/jal/widgets/dividend_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,26 +10,26 @@
 from jal.db.asset import JalAsset
 from jal.db.operations import LedgerTransaction, Dividend
 
 
 # ----------------------------------------------------------------------------------------------------------------------
 class DividendWidgetDelegate(WidgetMapperDelegateBase):
     def __init__(self, parent=None):
-        WidgetMapperDelegateBase.__init__(self, parent)
+        super().__init__(parent=parent)
         self.delegates = {'timestamp': self.timestamp_delegate,
                           'ex_date': self.timestamp_delegate,
                           'asset_id': self.symbol_delegate,
                           'amount': self.decimal_delegate,
                           'tax': self.decimal_delegate}
 
 
 # ----------------------------------------------------------------------------------------------------------------------
 class DividendWidget(AbstractOperationDetails):
     def __init__(self, parent=None):
-        AbstractOperationDetails.__init__(self, parent)
+        super().__init__(parent=parent)
         self.name = self.tr("Dividend")
         self.operation_type = LedgerTransaction.Dividend
         self.combo_model = None
 
         self.date_label = QLabel(self)
         self.ex_date_label = QLabel(self)
         self.number_label = QLabel(self)
```

### Comparing `jal-2023.4.5/jal/widgets/helpers.py` & `jal-2023.4.6/jal/widgets/helpers.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/widgets/income_spending_widget.py` & `jal-2023.4.6/jal/widgets/income_spending_widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,22 +14,22 @@
 from jal.db.operations import LedgerTransaction
 from jal.widgets.delegates import WidgetMapperDelegateBase, FloatDelegate, CategorySelectorDelegate, TagSelectorDelegate
 
 
 # ----------------------------------------------------------------------------------------------------------------------
 class IncomeSpendingWidgetDelegate(WidgetMapperDelegateBase):
     def __init__(self, parent=None):
-        WidgetMapperDelegateBase.__init__(self, parent)
+        super().__init__(parent=parent)
         self.delegates = {'timestamp': self.timestamp_delegate}
 
 
 # ----------------------------------------------------------------------------------------------------------------------
 class IncomeSpendingWidget(AbstractOperationDetails):
     def __init__(self, parent=None):
-        AbstractOperationDetails.__init__(self, parent)
+        super().__init__(parent=parent)
         self.name = self.tr("Income / Spending")
         self.operation_type = LedgerTransaction.IncomeSpending
 
         self.category_delegate = CategorySelectorDelegate()
         self.tag_delegate = TagSelectorDelegate()
         self.float_delegate = FloatDelegate(2)
 
@@ -164,25 +164,30 @@
         selection = self.details_table.selectionModel().selection().indexes()
         for idx in selection:
             self.details_model.removeRow(idx.row())
             self.onDataChange(idx, idx, None)
 
     @Slot()
     def saveChanges(self):
-        if not self.model.submitAll():
-            logging.fatal(self.tr("Operation submit failed: ") + self.model.lastError().text())
-            return
-        pid = self.model.data(self.model.index(0, self.model.fieldIndex("id")))
-        if pid is None:  # we just have saved new action record and need last inserted id
-            pid = self.model.query().lastInsertId()
-        for row in range(self.details_model.rowCount()):
-            self.details_model.setData(self.details_model.index(row, self.details_model.fieldIndex("pid")), pid)
-        if not self.details_model.submitAll():
-            logging.fatal(self.tr("Operation details submit failed: ") + self.details_model.lastError().text())
+        self.model.database().transaction()
+        try:
+            if not self.model.submitAll():
+                raise RuntimeError(self.tr("Operation submit failed: ") + self.model.lastError().text())
+            pid = self.model.data(self.model.index(0, self.model.fieldIndex("id")))
+            if pid is None:  # we just have saved new action record and need last inserted id
+                pid = self.model.last_insert_id()
+            for row in range(self.details_model.rowCount()):
+                self.details_model.setData(self.details_model.index(row, self.details_model.fieldIndex("pid")), pid)
+            if not self.details_model.submitAll():
+                raise RuntimeError(self.tr("Operation details submit failed: ") + self.details_model.lastError().text())
+        except Exception as e:
+            self.model.database().rollback()
+            logging.fatal(e)
             return
+        self.model.database().commit()
         self.modified = False
         self.commit_button.setEnabled(False)
         self.revert_button.setEnabled(False)
         self.dbUpdated.emit()
 
     @Slot()
     def revertChanges(self):
```

### Comparing `jal-2023.4.5/jal/widgets/main_window.py` & `jal-2023.4.6/jal/widgets/main_window.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/widgets/mdi.py` & `jal-2023.4.6/jal/widgets/mdi.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 
 # ----------------------------------------------------------------------------------------------------------------------
 # Class that acts as QMdiArea in SubWindowView mode but has Tabs at the same time
 # Child windows should be derived from MdiWidget class for correct operation
 class TabbedMdiArea(QWidget):
     def __init__(self, parent=None):
-        QWidget.__init__(self, parent)
+        super().__init__(parent=parent)
 
         self.layout = QVBoxLayout(self)
         self.layout.setContentsMargins(0, 0, 0, 0)
         self.layout.setSpacing(0)
         self.setLayout(self.layout)
 
         self.mdi = QMdiArea(self)
```

### Comparing `jal-2023.4.5/jal/widgets/operations_tabs.py` & `jal-2023.4.6/jal/widgets/operations_tabs.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/widgets/operations_widget.py` & `jal-2023.4.6/jal/widgets/operations_widget.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/widgets/price_chart.py` & `jal-2023.4.6/jal/widgets/price_chart.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from jal.db.asset import JalAsset
 from jal.constants import CustomColor
 from jal.widgets.mdi import MdiWidget
 
 
 class ChartWidget(QWidget):
     def __init__(self, parent, quotes, trades, data_range, currency_name):
-        QWidget.__init__(self, parent)
+        super().__init__(parent=parent)
         self.setMinimumWidth(600)
         self.setMinimumHeight(400)
 
         self.quotes_series = QLineSeries()
         for point in quotes:            # Conversion to 'float' in order not to get 'int' overflow on some platforms
             self.quotes_series.append(float(point['timestamp']), point['quote'])
```

### Comparing `jal-2023.4.5/jal/widgets/qr_scanner.py` & `jal-2023.4.6/jal/widgets/qr_scanner.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # ----------------------------------------------------------------------------------------------------------------------
 class QRScanner(QWidget):
     QR_SIZE = 0.75      # Size of rectangle for QR capture (used to display only currently)
     QR_SCAN_RATE = 100  # Delay in ms between QR captures
     decodedQR = Signal(str)
 
     def __init__(self, parent=None):
-        QWidget.__init__(self, parent)
+        super().__init__(parent=parent)
         self.processing = False
         self.started = False
         self.rectangle = None
 
         self.setMinimumHeight(405)
         self.layout = QVBoxLayout(self)
         self.layout.setContentsMargins(0, 0, 0, 0)
```

### Comparing `jal-2023.4.5/jal/widgets/reference_data.py` & `jal-2023.4.6/jal/widgets/reference_data.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/widgets/reference_dialogs.py` & `jal-2023.4.6/jal/widgets/reference_dialogs.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 from jal.widgets.asset_dialog import AssetDialog
 from jal.widgets.delegates import GridLinesDelegate
 from jal.widgets.selection_dialog import SelectPeerDialog, SelectCategoryDialog, SelectTagDialog 
 
 
 # ----------------------------------------------------------------------------------------------------------------------
 class AccountListModel(AbstractReferenceListModel):
-    def __init__(self, table, parent_view):
-        AbstractReferenceListModel.__init__(self, table, parent_view)
+    def __init__(self, table, parent_view, **kwargs):
+        super().__init__(table=table, parent_view=parent_view)
         self._columns = [("id", ''),
                          ("type_id", ''),
                          ("name", self.tr("Name")),
                          ("currency_id", self.tr("Currency")),
                          ("active", self.tr("Act.")),
                          ("number", self.tr("Account #")),
                          ("reconciled_on", self.tr("Reconciled @")),
@@ -57,18 +57,18 @@
         self._timestamp_delegate = TimestampDelegate(parent=self._view)
         self._view.setItemDelegateForColumn(self.fieldIndex("reconciled_on"), self._timestamp_delegate)
         self._bool_delegate = BoolDelegate(self._view)
         self._view.setItemDelegateForColumn(self.fieldIndex("active"), self._bool_delegate)
 
 
 class AccountListDialog(ReferenceDataDialog):
-    def __init__(self):
-        ReferenceDataDialog.__init__(self)
+    def __init__(self, parent=None):
+        super().__init__(parent=parent)
         self.table = "accounts"
-        self.model = AccountListModel(self.table, self.ui.DataView)
+        self.model = AccountListModel(table=self.table, parent_view=self.ui.DataView)
         self.ui.DataView.setModel(self.model)
         self.model.configureView()
         self.setup_ui()
         super()._init_completed()
 
     def setup_ui(self):
         self.search_field = "accounts.name"
@@ -92,16 +92,16 @@
         self.ui.GroupCombo.setCurrentIndex(type_id-1)
         item_idx = self.model.locateItem(item_id, use_filter=self._filter_text)
         self.ui.DataView.setCurrentIndex(item_idx)
 
 
 # ----------------------------------------------------------------------------------------------------------------------
 class AssetListModel(AbstractReferenceListModel):
-    def __init__(self, table, parent_view):
-        AbstractReferenceListModel.__init__(self, table, parent_view)
+    def __init__(self, table, parent_view, **kwargs):
+        super().__init__(table=table, parent_view=parent_view)
         pk = QSqlIndex()   # Manual primary key setup is required as we use underlying sql view instead of sql table
         pk.append(self.record().field("id"))
         self.setPrimaryKey(pk)
         self._columns = [("id", ''),
                          ("type_id", ''),
                          ("symbol", self.tr("Symbol")),
                          ("full_name", self.tr("Name")),
@@ -125,16 +125,16 @@
         super().configureView()
         self._lookup_delegate = QSqlRelationalDelegate(self._view)
         self._view.setItemDelegateForColumn(self.fieldIndex("country_id"), self._lookup_delegate)
         self._view.setItemDelegateForColumn(self.fieldIndex("quote_source"), self._lookup_delegate)
 
 
 class AssetListDialog(ReferenceDataDialog):
-    def __init__(self):
-        ReferenceDataDialog.__init__(self)
+    def __init__(self, parent=None):
+        super().__init__(parent=parent)
         self.table = "assets_ext"
         self.model = AssetListModel(self.table, self.ui.DataView)
         self.ui.DataView.setModel(self.model)
         self.model.configureView()
         self.setup_ui()
         super()._init_completed()
 
@@ -164,16 +164,16 @@
 
     def customEditor(self):
         return AssetDialog(self)
 
 
 # ----------------------------------------------------------------------------------------------------------------------
 class PeerTreeModel(SqlTreeModel):
-    def __init__(self, table, parent_view):
-        super().__init__(table, parent_view)
+    def __init__(self, table, parent_view, **kwargs):
+        super().__init__(table=table, parent_view=parent_view)
         self._columns = [("name", self.tr("Name")),
                          ("location", self.tr("Location")),
                          ("actions_count", self.tr("Docs count"))]
         self._sort_by = "name"
         self._stretch = "name"
         self._int_delegate = None
         self._grid_delegate = None
@@ -195,16 +195,16 @@
         self._view.setItemDelegateForColumn(self.fieldIndex("name"), self._grid_delegate)
         self._view.setItemDelegateForColumn(self.fieldIndex("location"), self._grid_delegate)
         self._int_delegate = FloatDelegate(0, parent=self._view)
         self._view.setItemDelegateForColumn(self.fieldIndex("actions_count"), self._int_delegate)
 
 
 class PeerListDialog(ReferenceDataDialog):
-    def __init__(self, parent):
-        ReferenceDataDialog.__init__(self, parent)
+    def __init__(self, parent=None):
+        super().__init__(parent=parent)
         self.table = "agents"
         self.model = PeerTreeModel(self.table, self.ui.TreeView)
         self.ui.TreeView.setModel(self.model)
         self.model.configureView()
         self.setup_ui()
         super()._init_completed()
         self._menu_peer_id = 0
@@ -251,16 +251,16 @@
             JalPeer(self._menu_peer_id).replace_with(dialog.selected_id)
         logging.info(self.tr("Peer '") + self._menu_peer_name + self.tr("' was successfully replaced"))
         self.close()
 
 
 # ----------------------------------------------------------------------------------------------------------------------
 class CategoryTreeModel(SqlTreeModel):
-    def __init__(self, table, parent_view):
-        super().__init__(table, parent_view)
+    def __init__(self, table, parent_view, **kwargs):
+        super().__init__(table=table, parent_view=parent_view)
         self._columns = [("name", self.tr("Name")),
                          ("often", self.tr("Often"))]
         self._sort_by = "name"
         self._stretch = "name"
         self._bool_delegate = None
         self._grid_delegate = None
 
@@ -269,16 +269,16 @@
         self._grid_delegate = GridLinesDelegate(self._view)
         self._view.setItemDelegateForColumn(self.fieldIndex("name"), self._grid_delegate)
         self._bool_delegate = BoolDelegate(self._view)
         self._view.setItemDelegateForColumn(self.fieldIndex("often"), self._bool_delegate)
 
 
 class CategoryListDialog(ReferenceDataDialog):
-    def __init__(self, parent):
-        ReferenceDataDialog.__init__(self, parent)
+    def __init__(self, parent=None):
+        super().__init__(parent=parent)
         self.table = "categories"
         self.model = CategoryTreeModel(self.table, self.ui.TreeView)
         self.ui.TreeView.setModel(self.model)
         self.model.configureView()
         self.setup_ui()
         super()._init_completed()
         self._menu_category_id = 0
@@ -321,26 +321,26 @@
         JalCategory(self._menu_category_id).replace_with(dialog.selected_id)
         logging.info(self.tr("Category '") + self._menu_category_name + self.tr("' was successfully replaced"))
         self.close()
 
 # ----------------------------------------------------------------------------------------------------------------------
 class TagListModel(AbstractReferenceListModel):
     def __init__(self, table, parent_view):
-        AbstractReferenceListModel.__init__(self, table, parent_view)
+        super().__init__(table=table, parent_view=parent_view)
         self._columns = [("id", ''),
                          ("tag", self.tr("Tag"))]
         self._default_name = "tag"
         self._sort_by = "tag"
         self._hidden = ["id"]
         self._stretch = "tag"
 
 
 class TagsListDialog(ReferenceDataDialog):
-    def __init__(self, parent):
-        ReferenceDataDialog.__init__(self, parent)
+    def __init__(self, parent=None):
+        super().__init__(parent)
         self.table = "tags"
         self.model = TagListModel(self.table, self.ui.DataView)
         self.ui.DataView.setModel(self.model)
         self.model.configureView()
         self.setup_ui()
         super()._init_completed()
         self._menu_tag_id = 0
@@ -383,15 +383,15 @@
         logging.info(self.tr("Tag '") + self._menu_tag_name + self.tr("' was successfully replaced"))
         self.close()
 
 
 # ----------------------------------------------------------------------------------------------------------------------
 class QuotesListModel(AbstractReferenceListModel):
     def __init__(self, table, parent_view):
-        AbstractReferenceListModel.__init__(self, table, parent_view)
+        super().__init__(table=table, parent_view=parent_view)
         self._columns = [("id", ''),
                          ("timestamp", self.tr("Date")),
                          ("asset_id", self.tr("Asset")),
                          ("currency_id", self.tr("Currency")),
                          ("quote", self.tr("Quote"))]
         self._hidden = ["id"]
         self._default_name = "quote"
@@ -413,16 +413,16 @@
         self._timestamp_delegate = TimestampDelegate(parent=self._view)
         self._view.setItemDelegateForColumn(self.fieldIndex("timestamp"), self._timestamp_delegate)
         self._lookup_delegate = QSqlRelationalDelegate(self._view)
         self._view.setItemDelegateForColumn(self.fieldIndex("currency_id"), self._lookup_delegate)
 
 
 class QuotesListDialog(ReferenceDataDialog):
-    def __init__(self):
-        ReferenceDataDialog.__init__(self)
+    def __init__(self, parent=None):
+        super().__init__(parent)
         self.table = "quotes"
         self.model = QuotesListModel(self.table, self.ui.DataView)
         self.ui.DataView.setModel(self.model)
         self.model.configureView()
         self.setup_ui()
         super()._init_completed()
 
@@ -432,15 +432,15 @@
         self.setWindowTitle(self.tr("Quotes"))
         self.ui.Toggle.setVisible(False)
 
 
 # ----------------------------------------------------------------------------------------------------------------------
 class BaseCurrencyListModel(AbstractReferenceListModel):
     def __init__(self, table, parent_view):
-        AbstractReferenceListModel.__init__(self, table, parent_view)
+        super().__init__(table=table, parent_view=parent_view)
         self._columns = [("id", ''),
                          ("since_timestamp", self.tr("Date")),
                          ("currency_id", self.tr("Currency"))]
         self._hidden = ["id"]
         self._sort_by = "since_timestamp"
         self._default_name = "currency_id"
         self._timestamp_delegate = None
@@ -456,16 +456,16 @@
         self._timestamp_delegate = TimestampDelegate(display_format='%d/%m/%Y', parent=self._view)
         self._view.setItemDelegateForColumn(self.fieldIndex("since_timestamp"), self._timestamp_delegate)
         self._lookup_delegate = QSqlRelationalDelegate(self._view)
         self._view.setItemDelegateForColumn(self.fieldIndex("currency_id"), self._lookup_delegate)
 
 
 class BaseCurrencyDialog(ReferenceDataDialog):
-    def __init__(self):
-        ReferenceDataDialog.__init__(self)
+    def __init__(self, parent=None):
+        super().__init__(None)
         self.table = "base_currency"
         self.model = BaseCurrencyListModel(self.table, self.ui.DataView)
         self.ui.DataView.setModel(self.model)
         self.model.configureView()
         self.setup_ui()
         super()._init_completed()
```

### Comparing `jal-2023.4.5/jal/widgets/reference_selector.py` & `jal-2023.4.6/jal/widgets/reference_selector.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 
 #-----------------------------------------------------------------------------------------------------------------------
 class AbstractReferenceSelector(QWidget):
     changed = Signal()
 
     def __init__(self, parent=None):
-        QWidget.__init__(self, parent)
+        super().__init__(parent=parent)
         self.completer = None
         self.p_selected_id = 0
 
         self.layout = QHBoxLayout()
         self.layout.setContentsMargins(0, 0, 0, 0)
         self.layout.setSpacing(1)
         self.name = QLineEdit()
@@ -82,44 +82,44 @@
 # ----------------------------------------------------------------------------------------------------------------------
 class AccountSelector(AbstractReferenceSelector):
     def __init__(self, parent=None):
         self.table = "accounts"
         self.selector_field = "name"
         self.details_field = None
         self.dialog = ui_dialogs.AccountListDialog()
-        AbstractReferenceSelector.__init__(self, parent)
+        super().__init__(parent=parent)
 
 
 class AssetSelector(AbstractReferenceSelector):
     def __init__(self, parent=None):
         self.table = "assets_ext"
         self.selector_field = "symbol"
         self.details_field = "full_name"
         self.dialog = ui_dialogs.AssetListDialog()
-        AbstractReferenceSelector.__init__(self, parent)
+        super().__init__(parent=parent)
 
 
 class PeerSelector(AbstractReferenceSelector):
     def __init__(self, parent=None):
         self.table = "agents"
         self.selector_field = "name"
         self.details_field = None
         self.dialog = ui_dialogs.PeerListDialog(parent)
-        AbstractReferenceSelector.__init__(self, parent)
+        super().__init__(parent=parent)
 
 
 class CategorySelector(AbstractReferenceSelector):
     def __init__(self, parent=None):
         self.table = "categories"
         self.selector_field = "name"
         self.details_field = None
         self.dialog = ui_dialogs.CategoryListDialog(parent)
-        AbstractReferenceSelector.__init__(self, parent)
+        super().__init__(parent=parent)
 
 
 class TagSelector(AbstractReferenceSelector):
     def __init__(self, parent=None):
         self.table = "tags"
         self.selector_field = "tag"
         self.details_field = None
         self.dialog = ui_dialogs.TagsListDialog(parent)
-        AbstractReferenceSelector.__init__(self, parent)
+        super().__init__(parent=parent)
```

### Comparing `jal-2023.4.5/jal/widgets/register_designer_plugins.py` & `jal-2023.4.6/jal/widgets/register_designer_plugins.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/widgets/selection_dialog.py` & `jal-2023.4.6/jal/widgets/selection_dialog.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 
 #-----------------------------------------------------------------------------------------------------------------------
 # Dialog for peer selection
 # Constructor takes description to show and default_peer for initial choice
 class SelectPeerDialog(SelectReferenceDialog):
     def __init__(self, description, default_peer=0):
-        SelectReferenceDialog.__init__(self, self.tr("Please select peer"), description)
+        super().__init__(title=self.tr("Please select peer"), description=description)
         self.PeerWidget = PeerSelector(self.ui.SelectorFrame)
         self.ui.FrameLayout.addWidget(self.PeerWidget)
         self.PeerWidget.selected_id = self.selected_id = default_peer
 
     @Slot()
     def closeEvent(self, event):
         self.selected_id = self.PeerWidget.selected_id
@@ -46,15 +46,15 @@
         
         
 #-----------------------------------------------------------------------------------------------------------------------
 # Dialog for category selection
 # Constructor takes description to show and default_category for initial choice
 class SelectCategoryDialog(SelectReferenceDialog):
     def __init__(self, description, default_category=0):
-        SelectReferenceDialog.__init__(self, self.tr("Please select category"), description)
+        super().__init__(title=self.tr("Please select category"), description=description)
         self.CategoryWidget = CategorySelector(self.ui.SelectorFrame)
         self.ui.FrameLayout.addWidget(self.CategoryWidget)
         self.CategoryWidget.selected_id = self.selected_id = default_category
 
     @Slot()
     def closeEvent(self, event):
         self.selected_id = self.CategoryWidget.selected_id
@@ -62,15 +62,15 @@
 
 
 #-----------------------------------------------------------------------------------------------------------------------
 # Dialog for tag selection
 # Constructor takes description to show and default_tag for initial choice
 class SelectTagDialog(SelectReferenceDialog):
     def __init__(self, description, default_tag=0):
-        SelectReferenceDialog.__init__(self, self.tr("Please select tag"), description)
+        super().__init__(title=self.tr("Please select tag"), description=description)
         self.TagWidget = TagSelector(self.ui.SelectorFrame)
         self.ui.FrameLayout.addWidget(self.TagWidget)
         self.TagWidget.selected_id = self.selected_id = default_tag
 
     @Slot()
     def closeEvent(self, event):
         self.selected_id = self.TagWidget.selected_id
```

### Comparing `jal-2023.4.5/jal/widgets/tax_widget.py` & `jal-2023.4.6/jal/widgets/tax_widget.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/jal/widgets/trade_widget.py` & `jal-2023.4.6/jal/widgets/trade_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,27 +8,27 @@
 from jal.widgets.delegates import WidgetMapperDelegateBase
 from jal.db.operations import LedgerTransaction
 
 
 # ----------------------------------------------------------------------------------------------------------------------
 class TradeWidgetDelegate(WidgetMapperDelegateBase):
     def __init__(self, parent=None):
-        WidgetMapperDelegateBase.__init__(self, parent)
+        super().__init__(parent=parent)
         self.delegates = {'timestamp': self.timestamp_delegate,
                           'settlement': self.timestamp_delegate,
                           'asset_id': self.symbol_delegate,
                           'qty': self.decimal_delegate,
                           'price': self.decimal_delegate,
                           'fee': self.decimal_delegate}
 
 
 # ----------------------------------------------------------------------------------------------------------------------
 class TradeWidget(AbstractOperationDetails):
     def __init__(self, parent=None):
-        AbstractOperationDetails.__init__(self, parent)
+        super().__init__(parent=parent)
         self.name = self.tr("Buy / Sell")
         self.operation_type = LedgerTransaction.Trade
 
         self.date_label = QLabel(self)
         self.settlement_label = QLabel()
         self.number_label = QLabel(self)
         self.account_label = QLabel(self)
```

### Comparing `jal-2023.4.5/jal/widgets/transfer_widget.py` & `jal-2023.4.6/jal/widgets/transfer_widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,26 +9,26 @@
 from jal.widgets.delegates import WidgetMapperDelegateBase
 from jal.db.operations import LedgerTransaction
 
 
 # ----------------------------------------------------------------------------------------------------------------------
 class TransferWidgetDelegate(WidgetMapperDelegateBase):
     def __init__(self, parent=None):
-        WidgetMapperDelegateBase.__init__(self, parent)
+        super().__init__(parent=parent)
         self.delegates = {'withdrawal_timestamp': self.timestamp_delegate,
                           'withdrawal': self.decimal_delegate,
                           'deposit_timestamp': self.timestamp_delegate,
                           'deposit': self.decimal_delegate,
                           'fee': self.decimal_delegate}
 
 
 # ----------------------------------------------------------------------------------------------------------------------
 class TransferWidget(AbstractOperationDetails):
     def __init__(self, parent=None):
-        AbstractOperationDetails.__init__(self, parent)
+        super().__init__(parent=parent)
         self.name = self.tr("Transfer")
         self.operation_type = LedgerTransaction.Transfer
 
         self.from_date_label = QLabel(self)
         self.from_account_label = QLabel(self)
         self.from_amount_label = QLabel(self)
         self.to_date_label = QLabel(self)
```

### Comparing `jal-2023.4.5/jal.egg-info/PKG-INFO` & `jal-2023.4.6/jal.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jal
-Version: 2023.4.5
+Version: 2023.4.6
 Summary: Just Another Ledger - project to track personal financial records
 Home-page: https://github.com/titov-vv/jal
 Author-email: jal@gmx.ru
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial
 Classifier: Topic :: Office/Business :: Financial :: Accounting
```

### Comparing `jal-2023.4.5/jal.egg-info/SOURCES.txt` & `jal-2023.4.6/jal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jal-2023.4.5/setup.py` & `jal-2023.4.6/setup.py`

 * *Files identical despite different names*

