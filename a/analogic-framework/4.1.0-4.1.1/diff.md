# Comparing `tmp/analogic-framework-4.1.0.tar.gz` & `tmp/analogic-framework-4.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "analogic-framework-4.1.0.tar", last modified: Wed Apr 12 09:33:36 2023, max compression
+gzip compressed data, was "analogic-framework-4.1.1.tar", last modified: Sat Apr 15 08:59:29 2023, max compression
```

## Comparing `analogic-framework-4.1.0.tar` & `analogic-framework-4.1.1.tar`

### file list

```diff
@@ -1,255 +1,255 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:36.806396 analogic-framework-4.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-12 09:33:36.806396 analogic-framework-4.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10066 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:36.778396 analogic-framework-4.1.0/analogic/
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11724 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/analogic.py
--rw-r--r--   0 runner    (1001) docker     (123)    23429 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/analogic_tm1_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     7363 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/authentication_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/cam.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/camsecure.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/core_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/email.py
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/logging.json
--rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/loginbasic.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/logincam.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/nologin.py
--rw-r--r--   0 runner    (1001) docker     (123)    14105 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/pivot.py
--rw-r--r--   0 runner    (1001) docker     (123)     5281 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/setting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:36.766396 analogic-framework-4.1.0/analogic/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:36.770396 analogic-framework-4.1.0/analogic/static/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:36.778396 analogic-framework-4.1.0/analogic/static/assets/css/
--rw-r--r--   0 runner    (1001) docker     (123)    48488 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/css/bootstrap-grid.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   108539 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/css/bootstrap-grid.min.css.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:36.778396 analogic-framework-4.1.0/analogic/static/assets/css/lib/
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/css/lib/Chart-2.9.3.min.css
--rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/css/lib/nouislider.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    65538 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/css/style.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:36.778396 analogic-framework-4.1.0/analogic/static/assets/css/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/css/widgets/loader.css
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/css/widgets/simulation-panel-slider.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:36.778396 analogic-framework-4.1.0/analogic/static/assets/images/
--rw-r--r--   0 runner    (1001) docker     (123)    10487 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/images/loading.gif
--rw-r--r--   0 runner    (1001) docker     (123)   120349 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/images/loading2.gif
--rw-r--r--   0 runner    (1001) docker     (123)    55508 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/images/loading2_transparent.gif
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/images/triangle.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:36.770396 analogic-framework-4.1.0/analogic/static/assets/js/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:36.782396 analogic-framework-4.1.0/analogic/static/assets/js/framework/
--rw-r--r--   0 runner    (1001) docker     (123)    20536 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/framework/api.js
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/framework/app.js
--rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/framework/authentication.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:36.782396 analogic-framework-4.1.0/analogic/static/assets/js/framework/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/framework/extensions/authentication-provider.js
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/framework/extensions/write-executor.js
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/framework/listener.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:36.782396 analogic-framework-4.1.0/analogic/static/assets/js/framework/load-executor/
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/framework/load-executor/array.js
--rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/framework/load-executor/base.js
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/framework/load-executor/default.js
--rw-r--r--   0 runner    (1001) docker     (123)     3885 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/framework/load-executor/factory.js
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/framework/load-executor/skip.js
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/framework/load-executor/state.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:36.782396 analogic-framework-4.1.0/analogic/static/assets/js/framework/parsing-control/
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/framework/parsing-control/base.js
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/framework/parsing-control/factory.js
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/framework/parsing-control/list.js
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/framework/parsing-control/matrix.js
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/framework/parsing-control/object.js
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/framework/parsing-control/script.js
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/framework/parsing-control/skip.js
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/framework/pivot.js
--rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/framework/query-builder.js
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/framework/redirect.js
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/framework/render.js
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/framework/rest-request.js
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/framework/server.js
--rw-r--r--   0 runner    (1001) docker     (123)    22800 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/framework/utils.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:36.782396 analogic-framework-4.1.0/analogic/static/assets/js/framework/write-executor/
--rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/framework/write-executor/base.js
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/framework/write-executor/download.js
--rw-r--r--   0 runner    (1001) docker     (123)     5735 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/framework/write-executor/factory.js
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/framework/write-executor/function.js
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/framework/write-executor/grid-table.js
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/framework/write-executor/skip.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:36.786396 analogic-framework-4.1.0/analogic/static/assets/js/lib/
--rw-r--r--   0 runner    (1001) docker     (123)   172689 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/lib/Chart-2.9.3.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    44136 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/lib/Sortable.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    12908 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/lib/chartjs-plugin-datalabels.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    21295 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/lib/chartjs-plugin-dragdata.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/lib/debounceAndThrottle.1.8.3.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:36.786396 analogic-framework-4.1.0/analogic/static/assets/js/lib/jquery/
--rw-r--r--   0 runner    (1001) docker     (123)    89411 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/lib/jquery/jquery-3.6.0.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/lib/jquery/jquery.actual.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/lib/jquery/jquery.cookie.js
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/lib/jquery/jquery.doubletap.js
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/lib/jquery/tableSort.js
--rw-r--r--   0 runner    (1001) docker     (123)    26460 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/lib/nouislider.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:36.790396 analogic-framework-4.1.0/analogic/static/assets/js/widgets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:36.790396 analogic-framework-4.1.0/analogic/static/assets/js/widgets/base/
--rw-r--r--   0 runner    (1001) docker     (123)    23255 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/base/widget.js
--rw-r--r--   0 runner    (1001) docker     (123)    12486 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/button.js
--rw-r--r--   0 runner    (1001) docker     (123)    27607 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/combo-chart.js
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/container.js
--rw-r--r--   0 runner    (1001) docker     (123)    15772 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/datepicker.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:36.794396 analogic-framework-4.1.0/analogic/static/assets/js/widgets/default/
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/default/BubbleChartWidget.json
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/default/ButtonWidget.json
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/default/ComboChartWidget.json
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/default/ContainerWidget.json
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/default/DatePickerWidget.json
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/default/DropBoxWidget.json
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/default/GaugeWidget.json
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/default/GridCellWidget.json
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/default/GridRowWidget.json
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/default/GridWidget.json
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/default/HistogramComboChartWidget.json
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/default/HorizontalTableWidget.json
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/default/ImageWidget.json
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/default/LineAreaChartWidget.json
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/default/PanelWidget.json
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/default/PieChartWidget.json
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/default/PopupWidget.json
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/default/ScrollTableWidget.json
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/default/SegmentedBarWidget.json
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/default/SegmentedControlItemWidget.json
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/default/SegmentedControlWidget.json
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/default/SideBarWidget.json
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/default/SimulationPanelSliderWidget.json
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/default/SimulationPanelWidget.json
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/default/SliderWidget.json
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/default/SwipeWidget.json
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/default/TextAreaWidget.json
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/default/TextBoxWidget.json
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/default/TextWidget.json
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/default/ToggleWidget.json
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/default/TornadoChartWidget.json
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/default/VerticalLineBoxWidget.json
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/default/WaterFallWidget.json
--rw-r--r--   0 runner    (1001) docker     (123)    10938 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/dropbox.js
--rw-r--r--   0 runner    (1001) docker     (123)     9323 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/gauge.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:36.794396 analogic-framework-4.1.0/analogic/static/assets/js/widgets/grid/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/grid/grid-cell.js
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/grid/grid-row.js
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/grid/grid.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:36.798396 analogic-framework-4.1.0/analogic/static/assets/js/widgets/grid-table/
--rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/grid-table/grid-table-cell.js
--rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/grid-table/grid-table-header-cell.js
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/grid-table/grid-table-header-row.js
--rw-r--r--   0 runner    (1001) docker     (123)    18935 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/grid-table/grid-table.js
--rw-r--r--   0 runner    (1001) docker     (123)    18115 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/histogram-combo-chart.js
--rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/horizontal-bar-chart.js
--rw-r--r--   0 runner    (1001) docker     (123)    25693 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/horizontal-table.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:36.798396 analogic-framework-4.1.0/analogic/static/assets/js/widgets/horizontaltable/
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/horizontaltable/action-button-row.js
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/horizontaltable/delete-button-row.js
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/horizontaltable/radio-button-row.js
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/image.js
--rw-r--r--   0 runner    (1001) docker     (123)    15899 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/line-area-chart.js
--rw-r--r--   0 runner    (1001) docker     (123)    26611 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/line-scatter-combo.js
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/loader.js
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/page.js
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/panel.js
--rw-r--r--   0 runner    (1001) docker     (123)     6271 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/pie-chart.js
--rw-r--r--   0 runner    (1001) docker     (123)    81004 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/pivot-table.js
--rw-r--r--   0 runner    (1001) docker     (123)     7777 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/popup.js
--rw-r--r--   0 runner    (1001) docker     (123)     8149 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/radar-chart.js
--rw-r--r--   0 runner    (1001) docker     (123)    36449 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/scroll-table.js
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/segmented-bar.js
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/segmented-control-item.js
--rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/segmented-control.js
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/shadow.js
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/simulation-panel-slider.js
--rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/simulation-panel.js
--rw-r--r--   0 runner    (1001) docker     (123)    19961 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/slider.js
--rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/swipe.js
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/system-popup.js
--rw-r--r--   0 runner    (1001) docker     (123)    20395 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/text.js
--rw-r--r--   0 runner    (1001) docker     (123)     4679 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/textarea.js
--rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/textbox.js
--rw-r--r--   0 runner    (1001) docker     (123)     7898 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/toggle.js
--rw-r--r--   0 runner    (1001) docker     (123)     4921 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/tornado-chart.js
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/vertical-line-box.js
--rw-r--r--   0 runner    (1001) docker     (123)    10794 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/water-fall.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:36.770396 analogic-framework-4.1.0/analogic/static/assets/skin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:36.802396 analogic-framework-4.1.0/analogic/static/assets/skin/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-button.css
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-combo-chart.css
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-container.css
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-datepicker.css
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-dropbox.css
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-gauge.css
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-general.css
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-grid-cell.css
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-grid-row.css
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-grid-table-cell.css
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-grid-table.css
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-grid.css
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-horizontal-table.css
--rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-horizontalbarchart.css
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-image.css
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-legend.css
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-line-area-chart.css
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-line-scatter-combo.css
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-page.css
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-panel.css
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-pie-chart.css
--rw-r--r--   0 runner    (1001) docker     (123)    20239 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-pivot-table.css
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-popup.css
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-radar-chart.css
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-scrolltable.css
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-segmented.css
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-segmentedbar.css
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-slider-touch.css
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-slider.css
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-text.css
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-textarea.css
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-textbox.css
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-toggle.css
--rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-tornado.css
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-vertical-line-box.css
--rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-waterfall.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:36.806396 analogic-framework-4.1.0/analogic/static/assets/skin/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)    75822 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/fonts/GothamNarrow-Bold.eot
--rw-r--r--   0 runner    (1001) docker     (123)   253851 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/fonts/GothamNarrow-Bold.svg
--rw-r--r--   0 runner    (1001) docker     (123)    75604 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/fonts/GothamNarrow-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    32032 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/fonts/GothamNarrow-Bold.woff
--rw-r--r--   0 runner    (1001) docker     (123)    23076 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/fonts/GothamNarrow-Bold.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    75582 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/fonts/GothamNarrow-Medium.eot
--rw-r--r--   0 runner    (1001) docker     (123)   256592 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/fonts/GothamNarrow-Medium.svg
--rw-r--r--   0 runner    (1001) docker     (123)    75356 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/fonts/GothamNarrow-Medium.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    32152 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/fonts/GothamNarrow-Medium.woff
--rw-r--r--   0 runner    (1001) docker     (123)    23124 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/fonts/GothamNarrow-Medium.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    26192 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/fonts/pivot.eot
--rw-r--r--   0 runner    (1001) docker     (123)   108091 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/fonts/pivot.svg
--rw-r--r--   0 runner    (1001) docker     (123)    26028 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/fonts/pivot.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    26104 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/fonts/pivot.woff
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:36.806396 analogic-framework-4.1.0/analogic/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/templates/404.html
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/templates/500.html
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/templates/authenticated.html
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/templates/config.html
--rw-r--r--   0 runner    (1001) docker     (123)    10533 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/templates/css.html
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)    11080 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/templates/javascripts.html
--rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/templates/login.html
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/templates/redirect.html
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/templates/sso_error.html
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/templates/unauthorized.html
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/version.config
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:36.806396 analogic-framework-4.1.0/analogic_framework.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-12 09:33:36.000000 analogic-framework-4.1.0/analogic_framework.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11099 2023-04-12 09:33:36.000000 analogic-framework-4.1.0/analogic_framework.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 09:33:36.000000 analogic-framework-4.1.0/analogic_framework.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-12 09:33:36.000000 analogic-framework-4.1.0/analogic_framework.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-12 09:33:36.000000 analogic-framework-4.1.0/analogic_framework.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 09:33:36.806396 analogic-framework-4.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:59:29.435998 analogic-framework-4.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-15 08:59:29.435998 analogic-framework-4.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10066 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:59:29.399997 analogic-framework-4.1.1/analogic/
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11724 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/analogic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23429 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/analogic_tm1_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7363 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/authentication_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/cam.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/camsecure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/core_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/logging.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/loginbasic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/logincam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/nologin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14105 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/pivot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5281 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/setting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:59:29.391997 analogic-framework-4.1.1/analogic/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:59:29.391997 analogic-framework-4.1.1/analogic/static/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:59:29.399997 analogic-framework-4.1.1/analogic/static/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (123)    48488 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/css/bootstrap-grid.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   108539 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/css/bootstrap-grid.min.css.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:59:29.399997 analogic-framework-4.1.1/analogic/static/assets/css/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/css/lib/Chart-2.9.3.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/css/lib/nouislider.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    65538 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/css/style.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:59:29.399997 analogic-framework-4.1.1/analogic/static/assets/css/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/css/widgets/loader.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/css/widgets/simulation-panel-slider.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:59:29.399997 analogic-framework-4.1.1/analogic/static/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    10487 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/images/loading.gif
+-rw-r--r--   0 runner    (1001) docker     (123)   120349 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/images/loading2.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    55508 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/images/loading2_transparent.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/images/triangle.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:59:29.391997 analogic-framework-4.1.1/analogic/static/assets/js/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:59:29.403997 analogic-framework-4.1.1/analogic/static/assets/js/framework/
+-rw-r--r--   0 runner    (1001) docker     (123)    20536 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/framework/api.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/framework/app.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/framework/authentication.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:59:29.403997 analogic-framework-4.1.1/analogic/static/assets/js/framework/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/framework/extensions/authentication-provider.js
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/framework/extensions/write-executor.js
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/framework/listener.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:59:29.403997 analogic-framework-4.1.1/analogic/static/assets/js/framework/load-executor/
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/framework/load-executor/array.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/framework/load-executor/base.js
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/framework/load-executor/default.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3885 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/framework/load-executor/factory.js
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/framework/load-executor/skip.js
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/framework/load-executor/state.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:59:29.407997 analogic-framework-4.1.1/analogic/static/assets/js/framework/parsing-control/
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/framework/parsing-control/base.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/framework/parsing-control/factory.js
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/framework/parsing-control/list.js
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/framework/parsing-control/matrix.js
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/framework/parsing-control/object.js
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/framework/parsing-control/script.js
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/framework/parsing-control/skip.js
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/framework/pivot.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/framework/query-builder.js
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/framework/redirect.js
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/framework/render.js
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/framework/rest-request.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/framework/server.js
+-rw-r--r--   0 runner    (1001) docker     (123)    22800 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/framework/utils.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:59:29.407997 analogic-framework-4.1.1/analogic/static/assets/js/framework/write-executor/
+-rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/framework/write-executor/base.js
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/framework/write-executor/download.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5735 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/framework/write-executor/factory.js
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/framework/write-executor/function.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/framework/write-executor/grid-table.js
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/framework/write-executor/skip.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:59:29.407997 analogic-framework-4.1.1/analogic/static/assets/js/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)   172689 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/lib/Chart-2.9.3.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    44136 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/lib/Sortable.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12908 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/lib/chartjs-plugin-datalabels.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    21295 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/lib/chartjs-plugin-dragdata.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/lib/debounceAndThrottle.1.8.3.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:59:29.407997 analogic-framework-4.1.1/analogic/static/assets/js/lib/jquery/
+-rw-r--r--   0 runner    (1001) docker     (123)    89411 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/lib/jquery/jquery-3.6.0.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/lib/jquery/jquery.actual.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/lib/jquery/jquery.cookie.js
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/lib/jquery/jquery.doubletap.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/lib/jquery/tableSort.js
+-rw-r--r--   0 runner    (1001) docker     (123)    26460 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/lib/nouislider.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:59:29.415997 analogic-framework-4.1.1/analogic/static/assets/js/widgets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:59:29.415997 analogic-framework-4.1.1/analogic/static/assets/js/widgets/base/
+-rw-r--r--   0 runner    (1001) docker     (123)    23255 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/base/widget.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12486 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/button.js
+-rw-r--r--   0 runner    (1001) docker     (123)    27607 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/combo-chart.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/container.js
+-rw-r--r--   0 runner    (1001) docker     (123)    16545 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/datepicker.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:59:29.419997 analogic-framework-4.1.1/analogic/static/assets/js/widgets/default/
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/default/BubbleChartWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/default/ButtonWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/default/ComboChartWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/default/ContainerWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/default/DatePickerWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/default/DropBoxWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/default/GaugeWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/default/GridCellWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/default/GridRowWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/default/GridWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/default/HistogramComboChartWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/default/HorizontalTableWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/default/ImageWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/default/LineAreaChartWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/default/PanelWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/default/PieChartWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/default/PopupWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/default/ScrollTableWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/default/SegmentedBarWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/default/SegmentedControlItemWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/default/SegmentedControlWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/default/SideBarWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/default/SimulationPanelSliderWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/default/SimulationPanelWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/default/SliderWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/default/SwipeWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/default/TextAreaWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/default/TextBoxWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/default/TextWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/default/ToggleWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/default/TornadoChartWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/default/VerticalLineBoxWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/default/WaterFallWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10938 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/dropbox.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9323 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/gauge.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:59:29.423997 analogic-framework-4.1.1/analogic/static/assets/js/widgets/grid/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/grid/grid-cell.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/grid/grid-row.js
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/grid/grid.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:59:29.423997 analogic-framework-4.1.1/analogic/static/assets/js/widgets/grid-table/
+-rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/grid-table/grid-table-cell.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/grid-table/grid-table-header-cell.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/grid-table/grid-table-header-row.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18935 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/grid-table/grid-table.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18115 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/histogram-combo-chart.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/horizontal-bar-chart.js
+-rw-r--r--   0 runner    (1001) docker     (123)    25693 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/horizontal-table.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:59:29.423997 analogic-framework-4.1.1/analogic/static/assets/js/widgets/horizontaltable/
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/horizontaltable/action-button-row.js
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/horizontaltable/delete-button-row.js
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/horizontaltable/radio-button-row.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/image.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15899 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/line-area-chart.js
+-rw-r--r--   0 runner    (1001) docker     (123)    26611 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/line-scatter-combo.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/loader.js
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/page.js
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/panel.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6271 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/pie-chart.js
+-rw-r--r--   0 runner    (1001) docker     (123)    81004 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/pivot-table.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7777 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/popup.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8149 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/radar-chart.js
+-rw-r--r--   0 runner    (1001) docker     (123)    36449 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/scroll-table.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/segmented-bar.js
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/segmented-control-item.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/segmented-control.js
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/shadow.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/simulation-panel-slider.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/simulation-panel.js
+-rw-r--r--   0 runner    (1001) docker     (123)    19961 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/slider.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/swipe.js
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/system-popup.js
+-rw-r--r--   0 runner    (1001) docker     (123)    20395 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/text.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4679 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/textarea.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/textbox.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7898 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/toggle.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4921 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/tornado-chart.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/vertical-line-box.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10794 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/water-fall.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:59:29.395997 analogic-framework-4.1.1/analogic/static/assets/skin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:59:29.427997 analogic-framework-4.1.1/analogic/static/assets/skin/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-button.css
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-combo-chart.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-container.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-datepicker.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-dropbox.css
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-gauge.css
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-general.css
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-grid-cell.css
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-grid-row.css
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-grid-table-cell.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-grid-table.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-grid.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-horizontal-table.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-horizontalbarchart.css
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-image.css
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-legend.css
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-line-area-chart.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-line-scatter-combo.css
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-page.css
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-panel.css
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-pie-chart.css
+-rw-r--r--   0 runner    (1001) docker     (123)    20239 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-pivot-table.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-popup.css
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-radar-chart.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-scrolltable.css
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-segmented.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-segmentedbar.css
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-slider-touch.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-slider.css
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-text.css
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-textarea.css
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-textbox.css
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-toggle.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-tornado.css
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-vertical-line-box.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-waterfall.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:59:29.431998 analogic-framework-4.1.1/analogic/static/assets/skin/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)    75822 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/fonts/GothamNarrow-Bold.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   253851 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/fonts/GothamNarrow-Bold.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    75604 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/fonts/GothamNarrow-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    32032 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/fonts/GothamNarrow-Bold.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    23076 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/fonts/GothamNarrow-Bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    75582 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/fonts/GothamNarrow-Medium.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   256592 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/fonts/GothamNarrow-Medium.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    75356 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/fonts/GothamNarrow-Medium.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    32152 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/fonts/GothamNarrow-Medium.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    23124 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/fonts/GothamNarrow-Medium.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    26192 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/fonts/pivot.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   108091 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/fonts/pivot.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    26028 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/fonts/pivot.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    26104 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/fonts/pivot.woff
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:59:29.435998 analogic-framework-4.1.1/analogic/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/templates/404.html
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/templates/500.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/templates/authenticated.html
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/templates/config.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10533 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/templates/css.html
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11080 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/templates/javascripts.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/templates/login.html
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/templates/redirect.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/templates/sso_error.html
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/templates/unauthorized.html
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/version.config
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:59:29.435998 analogic-framework-4.1.1/analogic_framework.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-15 08:59:29.000000 analogic-framework-4.1.1/analogic_framework.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11099 2023-04-15 08:59:29.000000 analogic-framework-4.1.1/analogic_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 08:59:29.000000 analogic-framework-4.1.1/analogic_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-15 08:59:29.000000 analogic-framework-4.1.1/analogic_framework.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-15 08:59:29.000000 analogic-framework-4.1.1/analogic_framework.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 08:59:29.435998 analogic-framework-4.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/setup.py
```

### Comparing `analogic-framework-4.1.0/LICENSE` & `analogic-framework-4.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/README.md` & `analogic-framework-4.1.1/README.md`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/__init__.py` & `analogic-framework-4.1.1/analogic/__init__.py`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/analogic.py` & `analogic-framework-4.1.1/analogic/analogic.py`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/analogic_tm1_service.py` & `analogic-framework-4.1.1/analogic/analogic_tm1_service.py`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/authentication_provider.py` & `analogic-framework-4.1.1/analogic/authentication_provider.py`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/cam.py` & `analogic-framework-4.1.1/analogic/cam.py`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/camsecure.py` & `analogic-framework-4.1.1/analogic/camsecure.py`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/core_endpoints.py` & `analogic-framework-4.1.1/analogic/core_endpoints.py`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/email.py` & `analogic-framework-4.1.1/analogic/email.py`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/endpoint.py` & `analogic-framework-4.1.1/analogic/endpoint.py`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/loader.py` & `analogic-framework-4.1.1/analogic/loader.py`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/logging.json` & `analogic-framework-4.1.1/analogic/logging.json`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/loginbasic.py` & `analogic-framework-4.1.1/analogic/loginbasic.py`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/nologin.py` & `analogic-framework-4.1.1/analogic/nologin.py`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/pivot.py` & `analogic-framework-4.1.1/analogic/pivot.py`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/setting.py` & `analogic-framework-4.1.1/analogic/setting.py`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/css/bootstrap-grid.min.css` & `analogic-framework-4.1.1/analogic/static/assets/css/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/css/bootstrap-grid.min.css.map` & `analogic-framework-4.1.1/analogic/static/assets/css/bootstrap-grid.min.css.map`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/css/lib/Chart-2.9.3.min.css` & `analogic-framework-4.1.1/analogic/static/assets/css/lib/Chart-2.9.3.min.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/css/lib/nouislider.min.css` & `analogic-framework-4.1.1/analogic/static/assets/css/lib/nouislider.min.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/css/style.css` & `analogic-framework-4.1.1/analogic/static/assets/css/style.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/css/widgets/simulation-panel-slider.css` & `analogic-framework-4.1.1/analogic/static/assets/css/widgets/simulation-panel-slider.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/images/loading.gif` & `analogic-framework-4.1.1/analogic/static/assets/images/loading.gif`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/images/loading2.gif` & `analogic-framework-4.1.1/analogic/static/assets/images/loading2.gif`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/images/loading2_transparent.gif` & `analogic-framework-4.1.1/analogic/static/assets/images/loading2_transparent.gif`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/images/triangle.png` & `analogic-framework-4.1.1/analogic/static/assets/images/triangle.png`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/js/framework/api.js` & `analogic-framework-4.1.1/analogic/static/assets/js/framework/api.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/js/framework/app.js` & `analogic-framework-4.1.1/analogic/static/assets/js/framework/app.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/js/framework/authentication.js` & `analogic-framework-4.1.1/analogic/static/assets/js/framework/authentication.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/js/framework/load-executor/array.js` & `analogic-framework-4.1.1/analogic/static/assets/js/framework/load-executor/array.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/js/framework/load-executor/base.js` & `analogic-framework-4.1.1/analogic/static/assets/js/framework/load-executor/base.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/js/framework/load-executor/factory.js` & `analogic-framework-4.1.1/analogic/static/assets/js/framework/load-executor/factory.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/js/framework/parsing-control/base.js` & `analogic-framework-4.1.1/analogic/static/assets/js/framework/parsing-control/base.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/js/framework/parsing-control/factory.js` & `analogic-framework-4.1.1/analogic/static/assets/js/framework/parsing-control/factory.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/js/framework/parsing-control/matrix.js` & `analogic-framework-4.1.1/analogic/static/assets/js/framework/parsing-control/matrix.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/js/framework/pivot.js` & `analogic-framework-4.1.1/analogic/static/assets/js/framework/pivot.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/js/framework/query-builder.js` & `analogic-framework-4.1.1/analogic/static/assets/js/framework/query-builder.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/js/framework/server.js` & `analogic-framework-4.1.1/analogic/static/assets/js/framework/server.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/js/framework/utils.js` & `analogic-framework-4.1.1/analogic/static/assets/js/framework/utils.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/js/framework/write-executor/base.js` & `analogic-framework-4.1.1/analogic/static/assets/js/framework/write-executor/base.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/js/framework/write-executor/factory.js` & `analogic-framework-4.1.1/analogic/static/assets/js/framework/write-executor/factory.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/js/framework/write-executor/function.js` & `analogic-framework-4.1.1/analogic/static/assets/js/framework/write-executor/function.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/js/framework/write-executor/grid-table.js` & `analogic-framework-4.1.1/analogic/static/assets/js/framework/write-executor/grid-table.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/js/lib/Chart-2.9.3.min.js` & `analogic-framework-4.1.1/analogic/static/assets/js/lib/Chart-2.9.3.min.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/js/lib/Sortable.min.js` & `analogic-framework-4.1.1/analogic/static/assets/js/lib/Sortable.min.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/js/lib/chartjs-plugin-datalabels.min.js` & `analogic-framework-4.1.1/analogic/static/assets/js/lib/chartjs-plugin-datalabels.min.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/js/lib/chartjs-plugin-dragdata.min.js` & `analogic-framework-4.1.1/analogic/static/assets/js/lib/chartjs-plugin-dragdata.min.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/js/lib/debounceAndThrottle.1.8.3.min.js` & `analogic-framework-4.1.1/analogic/static/assets/js/lib/debounceAndThrottle.1.8.3.min.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/js/lib/jquery/jquery-3.6.0.min.js` & `analogic-framework-4.1.1/analogic/static/assets/js/lib/jquery/jquery-3.6.0.min.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/js/lib/jquery/jquery.actual.min.js` & `analogic-framework-4.1.1/analogic/static/assets/js/lib/jquery/jquery.actual.min.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/js/lib/jquery/jquery.cookie.js` & `analogic-framework-4.1.1/analogic/static/assets/js/lib/jquery/jquery.cookie.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/js/lib/jquery/jquery.doubletap.js` & `analogic-framework-4.1.1/analogic/static/assets/js/lib/jquery/jquery.doubletap.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/js/lib/jquery/tableSort.js` & `analogic-framework-4.1.1/analogic/static/assets/js/lib/jquery/tableSort.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/js/lib/nouislider.min.js` & `analogic-framework-4.1.1/analogic/static/assets/js/lib/nouislider.min.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/js/widgets/base/widget.js` & `analogic-framework-4.1.1/analogic/static/assets/js/widgets/base/widget.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/js/widgets/button.js` & `analogic-framework-4.1.1/analogic/static/assets/js/widgets/button.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/js/widgets/combo-chart.js` & `analogic-framework-4.1.1/analogic/static/assets/js/widgets/combo-chart.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/js/widgets/container.js` & `analogic-framework-4.1.1/analogic/static/assets/js/widgets/container.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/js/widgets/datepicker.js` & `analogic-framework-4.1.1/analogic/static/assets/js/widgets/datepicker.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -8,14 +8,16 @@
         let mainDivStyle = this.getGeneralStyles(d),
             titleStyles = this.getHtmlComponentStylesArray('title', d),
             innerStyle = this.getHtmlComponentStylesArray('inner', d),
             dividerStyle = this.getHtmlComponentStylesArray('divider', d),
             monthPicker = this.getRealValue('monthPicker', d, false);
 
         const v = {
+            allowEmptyDate: this.getRealValue('allowEmptyDate', d, false),
+            closeAfterSelectingTheDate: this.getRealValue('closeAfterSelectingTheDate', d, false),
             datePicked: this.getRealValue('datePicked', d, DatePickerWidget.getStandardizedDateString(new Date(), monthPicker)),
             editable: this.getRealValue('editable', d, true),
             local: this.getRealValue('local', d, false),
             skin: this.getRealValue('skin', d, 'standard'),
             maxDate: this.getRealValue('maxDate', d, false),
             minDate: this.getRealValue('minDate', d, false),
             monthPicker: monthPicker,
@@ -26,19 +28,24 @@
         };
 
         let date = DatePickerWidget.getDateFromString(v.datePicked, v.monthPicker),
             dateText = DatePickerWidget.getFormattedDateString(date, v.monthPicker, v.local),
             minDate = v.minDate ? DatePickerWidget.getDateFromString(v.minDate, v.monthPicker) : '',
             maxDate = v.maxDate ? DatePickerWidget.getDateFromString(v.maxDate, v.monthPicker) : '';
 
+        if (v.allowEmptyDate && (!d['datePicked'] || d['datePicked'] === '')) {
+            dateText = '';
+        }
+
         this.value = v.datePicked;
         this.minDate = minDate;
         this.maxDate = maxDate;
         this.panelFixed = v.panelFixed;
         this.local = v.local;
+        this.closeAfterSelectingTheDate = v.closeAfterSelectingTheDate;
 
 
         const months = ['JAN', 'FEB', 'MAR', 'APR', 'MAY', 'JUN', 'JUL', 'AUG', 'SEP', 'OCT', 'NOV', 'DEC'];
 
         let monthsHtml = months.map((month, i) => {
             let ym = new Date(date.getFullYear(), i),
                 disabled = '',
@@ -102,17 +109,18 @@
             return '<div ' + (!d ? '' : 'data-enabled="true"') + (d ? 'data-day="' + d + '"' : '') + ' class="' + disabled + ' ks-datepicker-panel-day-item ' + (d === Number(date.getDate()) ? 'on' : '') + ' ' + (((i % 7) === 6) ? 'ks-weekend ks-weekend-2' : '') + ' ' + (((i % 7) === 5) ? 'ks-weekend ks-weekend-1' : '') + '">' + d + '</div>';
         }).join('');
     }
 
     initEventHandlers() {
         const id = this.id,
             datePicker = $('#' + id + ' .ks-datepicker'),
-            dateInput = $('#' + id + ' .ks-datepicker-input');
+            dateInput = $('#' + id + ' .ks-datepicker-input'),
+            _this = this;
 
-        let date = DatePickerWidget.getDateFromString(Widgets[id].value, datePicker.data('monthpicker')),
+        let date = DatePickerWidget.getDateFromString(_this.value, datePicker.data('monthpicker')),
             yearHolder = $('#' + id + ' .ks-datepicker-panel-year'),
             monthHolders = $('#' + id + ' .ks-datepicker-panel-month-item'),
             dayHolders = $('#' + id + ' .ks-datepicker-panel-day-item'),
             target;
 
         datePicker.on('click touch', e => {
             Doc.find(".dropdown-type .holder").not(datePicker).each((i, el) => {
@@ -120,43 +128,47 @@
                     DatePickerWidget.triggerPickEvent($(el).closest('section').attr('id'), $(el), e);
                 }
             });
 
             if (pickerHolder.is(':visible')) {
                 DatePickerWidget.triggerPickEvent(id, pickerHolder, e);
             } else {
-                pickerHolder.slideDown(50, () => $(e.currentTarget).parent().get(0).scrollIntoView({
-                    behavior: 'smooth',
-                    block: 'start'
-                }));
+                if (window.innerHeight - dateInput.get(0).getBoundingClientRect().y < 300) {
+                    pickerHolder.slideDown(50, () => $(e.currentTarget).parent().get(0).scrollIntoView({
+                        behavior: 'smooth',
+                        block: 'start'
+                    }));
+                } else {
+                    pickerHolder.slideDown(50);
+                }
             }
 
             return false;
         }).on('dateChange.' + id, (_, date) => {
             let m = datePicker.data('monthpicker'),
                 minDateStr = String(datePicker.data('min-date')),
                 maxDateStr = String(datePicker.data('max-date')),
                 minDate = minDateStr ? DatePickerWidget.getDateFromString(minDateStr, m) : '',
                 maxDate = maxDateStr ? DatePickerWidget.getDateFromString(maxDateStr, m) : '';
 
             if (minDateStr && DatePickerWidget.isValidDateString(minDateStr, m)) {
                 if (date < minDate) {
                     date = minDate;
-                    dateInput.val(DatePickerWidget.getFormattedDateString(date, m, Widgets[id].local));
+                    dateInput.val(DatePickerWidget.getFormattedDateString(date, m, _this.local));
                 }
             }
 
             if (maxDateStr && DatePickerWidget.isValidDateString(maxDateStr, m)) {
                 if (date > maxDate) {
                     date = maxDate;
-                    dateInput.val(DatePickerWidget.getFormattedDateString(date, m, Widgets[id].local));
+                    dateInput.val(DatePickerWidget.getFormattedDateString(date, m, _this.local));
                 }
             }
 
-            Widgets[id].value = DatePickerWidget.getStandardizedDateString(date, m);
+            _this.value = DatePickerWidget.getStandardizedDateString(date, m);
 
             $('#' + id + ' .ks-datepicker-panel-days').empty().append(DatePickerWidget.getPickerHolderDaysHtml(date, minDate, maxDate));
             yearHolder.data('year', date.getFullYear()).text(date.getFullYear());
             monthHolders.removeClass('on').filter(`[data-month='${date.getMonth()}']`).addClass('on');
             dayHolders.removeClass('on').filter(`[data-day='${date.getDate()}']`).addClass('on');
 
             monthHolders.each((i, e) => {
@@ -167,30 +179,33 @@
                     target.toggleClass('disabled', ym < min.setMonth(min.getMonth() - 1));
                 }
                 if (maxDate) {
                     target.toggleClass('disabled', ym > maxDate);
                 }
             });
 
-            if (Widgets[id].panelFixed) {
+            if (_this.panelFixed || _this.closeAfterSelectingTheDate) {
                 DatePickerWidget.triggerPickEvent(id, pickerHolder, {});
+                if (_this.closeAfterSelectingTheDate) {
+                    pickerHolder.slideUp(50);
+                }
             }
         });
 
         const pickerHolder = $('#' + id + ' .ks-datepicker-panel').on('click touch', '.ks-datepicker-panel-pager', e => {
             let mod = $(e.currentTarget).hasClass('ks-left') ? -1 : 1;
-            date = DatePickerWidget.getDateFromString(Widgets[id].value, datePicker.data('monthpicker'));
+            date = DatePickerWidget.getDateFromString(_this.value, datePicker.data('monthpicker'));
             date.setYear(Number(date.getFullYear()) + mod);
         }).on('click touch', '.ks-datepicker-panel-month-item', e => {
             target = $(e.currentTarget);
-            date = DatePickerWidget.getDateFromString(Widgets[id].value, datePicker.data('monthpicker'));
+            date = DatePickerWidget.getDateFromString(_this.value, datePicker.data('monthpicker'));
             date.setMonth(target.data('month'));
         }).on('click touch', '.ks-datepicker-panel-day-item[data-enabled="true"]', e => {
             target = $(e.currentTarget);
-            date = DatePickerWidget.getDateFromString(Widgets[id].value, datePicker.data('monthpicker'));
+            date = DatePickerWidget.getDateFromString(_this.value, datePicker.data('monthpicker'));
             date.setDate(target.data('day'));
         }).on('click touch', e => {
             e.stopPropagation();
             $('#' + id + ' .ks-datepicker-input').val(DatePickerWidget.getFormattedDateString(date, datePicker.data('monthpicker'), Widgets[id].local));
             datePicker.trigger('dateChange.' + id, [date]);
         });
 
@@ -199,15 +214,15 @@
             if (!date) {
                 return false;
             }
 
             datePicker.trigger('dateChange.' + id, [date]);
         }).on('focusout', e => {
             let date = DatePickerWidget.getDateFromString($(e.currentTarget).val(), $(e.currentTarget).data('monthpicker'));
-            $('#' + id + ' .ks-datepicker-input').val(DatePickerWidget.getFormattedDateString(date, datePicker.data('monthpicker'), Widgets[id].local));
+            $('#' + id + ' .ks-datepicker-input').val(DatePickerWidget.getFormattedDateString(date, datePicker.data('monthpicker'), _this.local));
         }).on('keypress', e => {
             if (e.which === 13) {
                 $(e.currentTarget).blur();
                 let element = $('<div>');
                 element.data({
                     action: 'pick',
                     id: id,
@@ -215,28 +230,30 @@
                     ordinal: $('#' + id + ' .ks-datepicker').data('ordinal')
                 });
                 Widget.doHandleSystemEvent(element, e, true);
             }
         });
 
         const catcher = Doc.not(datePicker).on('click touch', e => {
-            if (pickerHolder.is(':visible') && !Widgets[id].panelFixed) {
-                let element = $('<div>');
-                element.data({
-                    action: 'pick',
-                    id: id,
-                    value: $('#' + id + ' .ks-datepicker-input').val().slice(0, -1),
-                    ordinal: $('#' + id + ' .ks-datepicker').data('ordinal')
-                });
-                Widget.doHandleSystemEvent(element, e, true);
+            if (pickerHolder.is(':visible') && !_this.panelFixed) {
+                if (!_this.closeAfterSelectingTheDate) {
+                    let element = $('<div>');
+                    element.data({
+                        action: 'pick',
+                        id: id,
+                        value: $('#' + id + ' .ks-datepicker-input').val().slice(0, -1),
+                        ordinal: $('#' + id + ' .ks-datepicker').data('ordinal')
+                    });
+                    Widget.doHandleSystemEvent(element, e, true);
+                }
                 pickerHolder.slideUp(50);
             }
         });
 
-        if (!Widgets[id].panelFixed) {
+        if (!_this.panelFixed) {
             pickerHolder.hide();
         }
     }
 
     reset() {
         delete this.value;
         delete this.minDate;
```

### Comparing `analogic-framework-4.1.0/analogic/static/assets/js/widgets/default/ScrollTableWidget.json` & `analogic-framework-4.1.1/analogic/static/assets/js/widgets/default/ScrollTableWidget.json`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/js/widgets/dropbox.js` & `analogic-framework-4.1.1/analogic/static/assets/js/widgets/dropbox.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/js/widgets/gauge.js` & `analogic-framework-4.1.1/analogic/static/assets/js/widgets/gauge.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/js/widgets/grid/grid-cell.js` & `analogic-framework-4.1.1/analogic/static/assets/js/widgets/grid/grid-cell.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/js/widgets/grid/grid-row.js` & `analogic-framework-4.1.1/analogic/static/assets/js/widgets/grid/grid-row.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/js/widgets/grid/grid.js` & `analogic-framework-4.1.1/analogic/static/assets/js/widgets/grid/grid.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/js/widgets/grid-table/grid-table-cell.js` & `analogic-framework-4.1.1/analogic/static/assets/js/widgets/grid-table/grid-table-cell.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/js/widgets/grid-table/grid-table-header-cell.js` & `analogic-framework-4.1.1/analogic/static/assets/js/widgets/grid-table/grid-table-header-cell.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/js/widgets/grid-table/grid-table-header-row.js` & `analogic-framework-4.1.1/analogic/static/assets/js/widgets/grid-table/grid-table-header-row.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/js/widgets/grid-table/grid-table.js` & `analogic-framework-4.1.1/analogic/static/assets/js/widgets/grid-table/grid-table.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/js/widgets/histogram-combo-chart.js` & `analogic-framework-4.1.1/analogic/static/assets/js/widgets/histogram-combo-chart.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/js/widgets/horizontal-bar-chart.js` & `analogic-framework-4.1.1/analogic/static/assets/js/widgets/horizontal-bar-chart.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/js/widgets/horizontal-table.js` & `analogic-framework-4.1.1/analogic/static/assets/js/widgets/horizontal-table.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/js/widgets/horizontaltable/action-button-row.js` & `analogic-framework-4.1.1/analogic/static/assets/js/widgets/horizontaltable/action-button-row.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/js/widgets/horizontaltable/delete-button-row.js` & `analogic-framework-4.1.1/analogic/static/assets/js/widgets/horizontaltable/delete-button-row.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/js/widgets/horizontaltable/radio-button-row.js` & `analogic-framework-4.1.1/analogic/static/assets/js/widgets/horizontaltable/radio-button-row.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/js/widgets/image.js` & `analogic-framework-4.1.1/analogic/static/assets/js/widgets/image.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/js/widgets/line-area-chart.js` & `analogic-framework-4.1.1/analogic/static/assets/js/widgets/line-area-chart.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/js/widgets/line-scatter-combo.js` & `analogic-framework-4.1.1/analogic/static/assets/js/widgets/line-scatter-combo.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/js/widgets/loader.js` & `analogic-framework-4.1.1/analogic/static/assets/js/widgets/loader.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/js/widgets/page.js` & `analogic-framework-4.1.1/analogic/static/assets/js/widgets/page.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/js/widgets/pie-chart.js` & `analogic-framework-4.1.1/analogic/static/assets/js/widgets/pie-chart.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/js/widgets/pivot-table.js` & `analogic-framework-4.1.1/analogic/static/assets/js/widgets/pivot-table.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/js/widgets/popup.js` & `analogic-framework-4.1.1/analogic/static/assets/js/widgets/popup.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/js/widgets/radar-chart.js` & `analogic-framework-4.1.1/analogic/static/assets/js/widgets/radar-chart.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/js/widgets/scroll-table.js` & `analogic-framework-4.1.1/analogic/static/assets/js/widgets/scroll-table.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/js/widgets/segmented-bar.js` & `analogic-framework-4.1.1/analogic/static/assets/js/widgets/segmented-bar.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/js/widgets/segmented-control-item.js` & `analogic-framework-4.1.1/analogic/static/assets/js/widgets/segmented-control-item.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/js/widgets/segmented-control.js` & `analogic-framework-4.1.1/analogic/static/assets/js/widgets/segmented-control.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/js/widgets/simulation-panel-slider.js` & `analogic-framework-4.1.1/analogic/static/assets/js/widgets/simulation-panel-slider.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/js/widgets/simulation-panel.js` & `analogic-framework-4.1.1/analogic/static/assets/js/widgets/simulation-panel.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/js/widgets/slider.js` & `analogic-framework-4.1.1/analogic/static/assets/js/widgets/slider.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/js/widgets/swipe.js` & `analogic-framework-4.1.1/analogic/static/assets/js/widgets/swipe.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/js/widgets/system-popup.js` & `analogic-framework-4.1.1/analogic/static/assets/js/widgets/system-popup.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/js/widgets/text.js` & `analogic-framework-4.1.1/analogic/static/assets/js/widgets/text.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/js/widgets/textarea.js` & `analogic-framework-4.1.1/analogic/static/assets/js/widgets/textarea.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/js/widgets/textbox.js` & `analogic-framework-4.1.1/analogic/static/assets/js/widgets/textbox.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/js/widgets/toggle.js` & `analogic-framework-4.1.1/analogic/static/assets/js/widgets/toggle.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/js/widgets/tornado-chart.js` & `analogic-framework-4.1.1/analogic/static/assets/js/widgets/tornado-chart.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/js/widgets/vertical-line-box.js` & `analogic-framework-4.1.1/analogic/static/assets/js/widgets/vertical-line-box.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/js/widgets/water-fall.js` & `analogic-framework-4.1.1/analogic/static/assets/js/widgets/water-fall.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-button.css` & `analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-button.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-container.css` & `analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-container.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-datepicker.css` & `analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-datepicker.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-dropbox.css` & `analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-dropbox.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-grid-table.css` & `analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-grid-table.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-grid.css` & `analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-grid.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-horizontal-table.css` & `analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-horizontal-table.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-horizontalbarchart.css` & `analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-horizontalbarchart.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-line-scatter-combo.css` & `analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-line-scatter-combo.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-pivot-table.css` & `analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-pivot-table.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-popup.css` & `analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-popup.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-scrolltable.css` & `analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-scrolltable.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-segmentedbar.css` & `analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-segmentedbar.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-slider-touch.css` & `analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-slider-touch.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-slider.css` & `analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-slider.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-text.css` & `analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-text.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-textarea.css` & `analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-textarea.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-textbox.css` & `analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-textbox.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-toggle.css` & `analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-toggle.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-tornado.css` & `analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-tornado.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-vertical-line-box.css` & `analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-vertical-line-box.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-waterfall.css` & `analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-waterfall.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/skin/fonts/GothamNarrow-Bold.eot` & `analogic-framework-4.1.1/analogic/static/assets/skin/fonts/GothamNarrow-Bold.eot`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/skin/fonts/GothamNarrow-Bold.svg` & `analogic-framework-4.1.1/analogic/static/assets/skin/fonts/GothamNarrow-Bold.svg`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/skin/fonts/GothamNarrow-Bold.ttf` & `analogic-framework-4.1.1/analogic/static/assets/skin/fonts/GothamNarrow-Bold.ttf`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/skin/fonts/GothamNarrow-Bold.woff` & `analogic-framework-4.1.1/analogic/static/assets/skin/fonts/GothamNarrow-Bold.woff`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/skin/fonts/GothamNarrow-Bold.woff2` & `analogic-framework-4.1.1/analogic/static/assets/skin/fonts/GothamNarrow-Bold.woff2`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/skin/fonts/GothamNarrow-Medium.eot` & `analogic-framework-4.1.1/analogic/static/assets/skin/fonts/GothamNarrow-Medium.eot`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/skin/fonts/GothamNarrow-Medium.svg` & `analogic-framework-4.1.1/analogic/static/assets/skin/fonts/GothamNarrow-Medium.svg`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/skin/fonts/GothamNarrow-Medium.ttf` & `analogic-framework-4.1.1/analogic/static/assets/skin/fonts/GothamNarrow-Medium.ttf`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/skin/fonts/GothamNarrow-Medium.woff` & `analogic-framework-4.1.1/analogic/static/assets/skin/fonts/GothamNarrow-Medium.woff`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/skin/fonts/GothamNarrow-Medium.woff2` & `analogic-framework-4.1.1/analogic/static/assets/skin/fonts/GothamNarrow-Medium.woff2`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/skin/fonts/pivot.eot` & `analogic-framework-4.1.1/analogic/static/assets/skin/fonts/pivot.eot`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/skin/fonts/pivot.svg` & `analogic-framework-4.1.1/analogic/static/assets/skin/fonts/pivot.svg`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/skin/fonts/pivot.ttf` & `analogic-framework-4.1.1/analogic/static/assets/skin/fonts/pivot.ttf`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/static/assets/skin/fonts/pivot.woff` & `analogic-framework-4.1.1/analogic/static/assets/skin/fonts/pivot.woff`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/templates/authenticated.html` & `analogic-framework-4.1.1/analogic/templates/authenticated.html`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/templates/config.html` & `analogic-framework-4.1.1/analogic/templates/config.html`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/templates/css.html` & `analogic-framework-4.1.1/analogic/templates/css.html`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/templates/javascripts.html` & `analogic-framework-4.1.1/analogic/templates/javascripts.html`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/templates/login.html` & `analogic-framework-4.1.1/analogic/templates/login.html`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/templates/redirect.html` & `analogic-framework-4.1.1/analogic/templates/redirect.html`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic/templates/sso_error.html` & `analogic-framework-4.1.1/analogic/templates/sso_error.html`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/analogic_framework.egg-info/SOURCES.txt` & `analogic-framework-4.1.1/analogic_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.0/setup.py` & `analogic-framework-4.1.1/setup.py`

 * *Files identical despite different names*

