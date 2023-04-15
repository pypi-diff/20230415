# Comparing `tmp/minitrade-0.1.8.tar.gz` & `tmp/minitrade-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minitrade-0.1.8.tar", max compression
+gzip compressed data, was "minitrade-0.1.9.tar", max compression
```

## Comparing `minitrade-0.1.8.tar` & `minitrade-0.1.9.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0    34523 2023-03-04 12:54:40.123117 minitrade-0.1.8/LICENSE.md
--rw-r--r--   0        0        0    14547 2023-03-14 09:40:29.531676 minitrade-0.1.8/README.md
--rw-r--r--   0        0        0        0 2023-03-04 12:54:40.141358 minitrade-0.1.8/minitrade/admin/Home.py
--rw-r--r--   0        0        0     9760 2023-03-10 05:03:27.818462 minitrade-0.1.8/minitrade/admin/pages/1_Trading.py
--rw-r--r--   0        0        0     1852 2023-03-04 12:54:40.142160 minitrade-0.1.8/minitrade/admin/pages/2_Strategy.py
--rw-r--r--   0        0        0     1162 2023-03-08 07:32:05.574982 minitrade-0.1.8/minitrade/admin/pages/3_Datasource.py
--rw-r--r--   0        0        0     3251 2023-03-10 05:03:27.819230 minitrade-0.1.8/minitrade/admin/pages/4_Broker.py
--rw-r--r--   0        0        0      439 2023-03-04 12:54:40.143228 minitrade-0.1.8/minitrade/admin/pages/5_Logs.py
--rw-r--r--   0        0        0     2063 2023-03-11 08:39:02.497508 minitrade-0.1.8/minitrade/admin/pages/6_Settings.py
--rw-r--r--   0        0        0       58 2023-03-04 12:54:40.143690 minitrade-0.1.8/minitrade/backtest/__init__.py
--rw-r--r--   0        0        0     2188 2023-03-04 12:54:40.143953 minitrade-0.1.8/minitrade/backtest/core/__init__.py
--rw-r--r--   0        0        0    30466 2023-03-10 05:03:27.820267 minitrade-0.1.8/minitrade/backtest/core/_plotting.py
--rw-r--r--   0        0        0     7611 2023-03-10 05:03:27.820928 minitrade-0.1.8/minitrade/backtest/core/_stats.py
--rw-r--r--   0        0        0     8206 2023-03-15 06:45:01.369103 minitrade-0.1.8/minitrade/backtest/core/_util.py
--rw-r--r--   0        0        0     1201 2023-03-04 12:54:40.147083 minitrade-0.1.8/minitrade/backtest/core/autoscale_cb.js
--rw-r--r--   0        0        0    83617 2023-03-15 06:50:10.907708 minitrade-0.1.8/minitrade/backtest/core/backtesting.py
--rw-r--r--   0        0        0    18531 2023-03-10 05:03:27.823770 minitrade-0.1.8/minitrade/backtest/core/lib.py
--rw-r--r--   0        0        0   279689 2023-03-04 12:54:40.149365 minitrade-0.1.8/minitrade/backtest/core/test/EURUSD.csv
--rw-r--r--   0        0        0    97833 2023-03-04 12:54:40.149998 minitrade-0.1.8/minitrade/backtest/core/test/GOOG.csv
--rw-r--r--   0        0        0      660 2023-03-10 05:03:27.824387 minitrade-0.1.8/minitrade/backtest/core/test/__init__.py
--rw-r--r--   0        0        0      325 2023-03-10 05:03:27.824859 minitrade-0.1.8/minitrade/backtest/core/test/__main__.py
--rw-r--r--   0        0        0    35906 2023-03-10 05:03:27.825744 minitrade-0.1.8/minitrade/backtest/core/test/_test.py
--rw-r--r--   0        0        0    12085 2023-03-04 12:54:40.150742 minitrade-0.1.8/minitrade/backtest/utils.py
--rw-r--r--   0        0        0       39 2023-03-04 12:54:40.151027 minitrade-0.1.8/minitrade/broker/__init__.py
--rw-r--r--   0        0        0     9361 2023-03-10 05:03:27.826503 minitrade-0.1.8/minitrade/broker/base.py
--rw-r--r--   0        0        0    10496 2023-03-14 03:40:18.170783 minitrade-0.1.8/minitrade/broker/ib.py
--rw-r--r--   0        0        0    11253 2023-03-17 06:27:09.229882 minitrade-0.1.8/minitrade/broker/ibgateway.py
--rw-r--r--   0        0        0     8760 2023-03-10 07:45:48.654421 minitrade-0.1.8/minitrade/cli.py
--rw-r--r--   0        0        0       20 2023-03-04 12:54:40.152691 minitrade-0.1.8/minitrade/datasource/__init__.py
--rw-r--r--   0        0        0     3954 2023-03-17 06:16:00.053927 minitrade-0.1.8/minitrade/datasource/base.py
--rw-r--r--   0        0        0      980 2023-03-08 07:32:24.478826 minitrade-0.1.8/minitrade/datasource/yahoo.py
--rw-r--r--   0        0        0     4339 2023-03-11 08:39:02.498775 minitrade-0.1.8/minitrade/minitrade.db.sql
--rw-r--r--   0        0        0       22 2023-03-04 12:54:40.153565 minitrade-0.1.8/minitrade/trader/__init__.py
--rw-r--r--   0        0        0     3589 2023-03-16 11:10:44.496816 minitrade-0.1.8/minitrade/trader/scheduler.py
--rw-r--r--   0        0        0    30079 2023-03-16 11:30:35.894143 minitrade-0.1.8/minitrade/trader/trader.py
--rw-r--r--   0        0        0     2328 2023-03-11 08:39:02.500178 minitrade-0.1.8/minitrade/utils/config.py
--rw-r--r--   0        0        0     1139 2023-03-11 08:39:02.500574 minitrade-0.1.8/minitrade/utils/mailjet.py
--rw-r--r--   0        0        0     7719 2023-03-10 05:03:27.830909 minitrade-0.1.8/minitrade/utils/mtdb.py
--rw-r--r--   0        0        0     8086 2023-03-17 05:19:10.028430 minitrade-0.1.8/minitrade/utils/telegram.py
--rw-r--r--   0        0        0     1487 2023-03-17 06:31:52.439977 minitrade-0.1.8/pyproject.toml
--rw-r--r--   0        0        0    16492 1970-01-01 00:00:00.000000 minitrade-0.1.8/setup.py
--rw-r--r--   0        0        0    16264 1970-01-01 00:00:00.000000 minitrade-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-03-04 12:54:40.123117 minitrade-0.1.9/LICENSE.md
+-rw-r--r--   0        0        0    14547 2023-03-14 09:40:29.531676 minitrade-0.1.9/README.md
+-rw-r--r--   0        0        0        0 2023-03-04 12:54:40.141358 minitrade-0.1.9/minitrade/admin/Home.py
+-rw-r--r--   0        0        0     9760 2023-03-10 05:03:27.818462 minitrade-0.1.9/minitrade/admin/pages/1_Trading.py
+-rw-r--r--   0        0        0     1852 2023-03-04 12:54:40.142160 minitrade-0.1.9/minitrade/admin/pages/2_Strategy.py
+-rw-r--r--   0        0        0     1162 2023-03-08 07:32:05.574982 minitrade-0.1.9/minitrade/admin/pages/3_Datasource.py
+-rw-r--r--   0        0        0     3251 2023-03-10 05:03:27.819230 minitrade-0.1.9/minitrade/admin/pages/4_Broker.py
+-rw-r--r--   0        0        0      439 2023-03-04 12:54:40.143228 minitrade-0.1.9/minitrade/admin/pages/5_Logs.py
+-rw-r--r--   0        0        0     2063 2023-03-11 08:39:02.497508 minitrade-0.1.9/minitrade/admin/pages/6_Settings.py
+-rw-r--r--   0        0        0       58 2023-03-04 12:54:40.143690 minitrade-0.1.9/minitrade/backtest/__init__.py
+-rw-r--r--   0        0        0     2188 2023-03-04 12:54:40.143953 minitrade-0.1.9/minitrade/backtest/core/__init__.py
+-rw-r--r--   0        0        0    32867 2023-03-18 03:40:14.105639 minitrade-0.1.9/minitrade/backtest/core/_plotting.py
+-rw-r--r--   0        0        0     7657 2023-03-17 10:13:37.298702 minitrade-0.1.9/minitrade/backtest/core/_stats.py
+-rw-r--r--   0        0        0     8196 2023-03-18 03:30:14.965447 minitrade-0.1.9/minitrade/backtest/core/_util.py
+-rw-r--r--   0        0        0     1201 2023-03-04 12:54:40.147083 minitrade-0.1.9/minitrade/backtest/core/autoscale_cb.js
+-rw-r--r--   0        0        0    84685 2023-03-18 03:23:12.622644 minitrade-0.1.9/minitrade/backtest/core/backtesting.py
+-rw-r--r--   0        0        0    18553 2023-03-17 10:04:53.815122 minitrade-0.1.9/minitrade/backtest/core/lib.py
+-rw-r--r--   0        0        0   279689 2023-03-04 12:54:40.149365 minitrade-0.1.9/minitrade/backtest/core/test/EURUSD.csv
+-rw-r--r--   0        0        0    97833 2023-03-04 12:54:40.149998 minitrade-0.1.9/minitrade/backtest/core/test/GOOG.csv
+-rw-r--r--   0        0        0      660 2023-03-10 05:03:27.824387 minitrade-0.1.9/minitrade/backtest/core/test/__init__.py
+-rw-r--r--   0        0        0      325 2023-03-10 05:03:27.824859 minitrade-0.1.9/minitrade/backtest/core/test/__main__.py
+-rw-r--r--   0        0        0    35906 2023-03-10 05:03:27.825744 minitrade-0.1.9/minitrade/backtest/core/test/_test.py
+-rw-r--r--   0        0        0    12085 2023-03-04 12:54:40.150742 minitrade-0.1.9/minitrade/backtest/utils.py
+-rw-r--r--   0        0        0       39 2023-03-04 12:54:40.151027 minitrade-0.1.9/minitrade/broker/__init__.py
+-rw-r--r--   0        0        0     9361 2023-03-10 05:03:27.826503 minitrade-0.1.9/minitrade/broker/base.py
+-rw-r--r--   0        0        0    10496 2023-03-14 03:40:18.170783 minitrade-0.1.9/minitrade/broker/ib.py
+-rw-r--r--   0        0        0    11253 2023-03-17 06:27:09.229882 minitrade-0.1.9/minitrade/broker/ibgateway.py
+-rw-r--r--   0        0        0     8760 2023-03-10 07:45:48.654421 minitrade-0.1.9/minitrade/cli.py
+-rw-r--r--   0        0        0       20 2023-03-04 12:54:40.152691 minitrade-0.1.9/minitrade/datasource/__init__.py
+-rw-r--r--   0        0        0     3954 2023-03-17 06:16:00.053927 minitrade-0.1.9/minitrade/datasource/base.py
+-rw-r--r--   0        0        0      980 2023-03-08 07:32:24.478826 minitrade-0.1.9/minitrade/datasource/yahoo.py
+-rw-r--r--   0        0        0     4339 2023-03-11 08:39:02.498775 minitrade-0.1.9/minitrade/minitrade.db.sql
+-rw-r--r--   0        0        0       22 2023-03-04 12:54:40.153565 minitrade-0.1.9/minitrade/trader/__init__.py
+-rw-r--r--   0        0        0     3589 2023-03-16 11:10:44.496816 minitrade-0.1.9/minitrade/trader/scheduler.py
+-rw-r--r--   0        0        0    30079 2023-03-16 11:30:35.894143 minitrade-0.1.9/minitrade/trader/trader.py
+-rw-r--r--   0        0        0     2328 2023-03-11 08:39:02.500178 minitrade-0.1.9/minitrade/utils/config.py
+-rw-r--r--   0        0        0     1139 2023-03-11 08:39:02.500574 minitrade-0.1.9/minitrade/utils/mailjet.py
+-rw-r--r--   0        0        0     7719 2023-03-10 05:03:27.830909 minitrade-0.1.9/minitrade/utils/mtdb.py
+-rw-r--r--   0        0        0     8086 2023-03-17 05:19:10.028430 minitrade-0.1.9/minitrade/utils/telegram.py
+-rw-r--r--   0        0        0     1487 2023-03-18 03:40:34.410129 minitrade-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0    16492 1970-01-01 00:00:00.000000 minitrade-0.1.9/setup.py
+-rw-r--r--   0        0        0    16264 1970-01-01 00:00:00.000000 minitrade-0.1.9/PKG-INFO
```

### Comparing `minitrade-0.1.8/LICENSE.md` & `minitrade-0.1.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `minitrade-0.1.8/README.md` & `minitrade-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `minitrade-0.1.8/minitrade/admin/pages/1_Trading.py` & `minitrade-0.1.9/minitrade/admin/pages/1_Trading.py`

 * *Files identical despite different names*

### Comparing `minitrade-0.1.8/minitrade/admin/pages/2_Strategy.py` & `minitrade-0.1.9/minitrade/admin/pages/2_Strategy.py`

 * *Files identical despite different names*

### Comparing `minitrade-0.1.8/minitrade/admin/pages/3_Datasource.py` & `minitrade-0.1.9/minitrade/admin/pages/3_Datasource.py`

 * *Files identical despite different names*

### Comparing `minitrade-0.1.8/minitrade/admin/pages/4_Broker.py` & `minitrade-0.1.9/minitrade/admin/pages/4_Broker.py`

 * *Files identical despite different names*

### Comparing `minitrade-0.1.8/minitrade/admin/pages/6_Settings.py` & `minitrade-0.1.9/minitrade/admin/pages/6_Settings.py`

 * *Files identical despite different names*

### Comparing `minitrade-0.1.8/minitrade/backtest/core/__init__.py` & `minitrade-0.1.9/minitrade/backtest/core/__init__.py`

 * *Files identical despite different names*

### Comparing `minitrade-0.1.8/minitrade/backtest/core/_plotting.py` & `minitrade-0.1.9/minitrade/backtest/core/_plotting.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,16 +9,17 @@
 
 import numpy as np
 import pandas as pd
 from bokeh.colors import RGB
 from bokeh.colors.named import lime as BULL_COLOR
 from bokeh.colors.named import tomato as BEAR_COLOR
 from bokeh.models import (ColumnDataSource, CrosshairTool, CustomJS,
-                          DatetimeTickFormatter, HoverTool, LinearColorMapper,
-                          NumeralTickFormatter, Range1d, Span, WheelZoomTool)
+                          DatetimeTickFormatter, HoverTool, Legend,
+                          LinearColorMapper, NumeralTickFormatter, Range1d,
+                          Span, WheelZoomTool)
 from bokeh.plotting import figure as _figure
 
 try:
     from bokeh.models import CustomJSTickFormatter
 except ImportError:  # Bokeh < 3.0
     from bokeh.models import FuncTickFormatter as CustomJSTickFormatter
 
@@ -115,15 +116,16 @@
     from .lib import _EQUITY_AGG, OHLCV_AGG, TRADES_AGG
     df = df.resample(freq, label='right').agg(OHLCV_AGG).dropna()
 
     indicators = [i.resample(freq, label='right').mean().dropna().reindex(df.index)
                   for i in indicators]
     assert not indicators or indicators[0].index.equals(df.index)
 
-    equity_data = equity_data.resample(freq, label='right').agg(_EQUITY_AGG).dropna(how='all')
+    ticker_agg = {ticker: 'last' for ticker in equity_data.columns if ticker not in _EQUITY_AGG}
+    equity_data = equity_data.resample(freq, label='right').agg(_EQUITY_AGG | ticker_agg).dropna(how='all')
     assert equity_data.index.equals(df.index)
 
     def _weighted_returns(s, trades=trades):
         df = trades.loc[s.index]
         return ((df['Size'].abs() * df['ReturnPct']) / df['Size'].abs().sum()).sum()
 
     def _group_trades(column):
@@ -153,15 +155,16 @@
          indicators: List[Union[pd.DataFrame, pd.Series]],
          filename='', plot_width=None,
          plot_equity=True, plot_return=False, plot_pl=True,
          plot_volume=False, plot_drawdown=False, plot_trades=True,
          smooth_equity=False, relative_equity=True,
          superimpose=False, resample=True,
          reverse_indicators=True,
-         show_legend=True, open_browser=True):
+         show_legend=True, open_browser=True,
+         plot_allocation=False, relative_allocation=True):
     """
     Like much of GUI code everywhere, this is a mess.
     """
     # We need to reset global Bokeh state, otherwise subsequent runs of
     # plot() contain some previous run's cruft data (was noticed when
     # TestPlot.test_file_size() test was failing).
     if not filename and not IS_JUPYTER_NOTEBOOK:
@@ -213,14 +216,15 @@
                                    bounds=(index[0] - pad,
                                            index[-1] + pad))) if index.size > 1 else {}
     fig_ohlc = new_bokeh_figure(**_kwargs)
     figs_above_ohlc, figs_below_ohlc = [], []
 
     source = ColumnDataSource(baseline)
     source.add((baseline.Close >= baseline.Open).values.astype(np.uint8).astype(str), 'inc')
+    source.add(baseline['Close']/baseline['Close'][0], 'bnh_perf')
 
     trade_source = ColumnDataSource(dict(
         index=trades['ExitBar'],
         datetime=trades['ExitTime'],
         exit_price=trades['ExitPrice'],
         ticker=trades['Ticker'],
         size=trades['Size'],
@@ -261,14 +265,18 @@
         kwargs.setdefault('height', 80)
         fig = new_bokeh_figure(x_range=fig_ohlc.x_range,
                                active_scroll='xwheel_zoom',
                                active_drag='xpan',
                                **kwargs)
         fig.xaxis.visible = False
         fig.yaxis.minor_tick_line_color = None
+        fig.add_layout(Legend(), 'center')
+        fig.legend.orientation = "horizontal"
+        fig.legend.background_fill_alpha = 0.8
+        fig.legend.border_line_alpha = 0
         return fig
 
     def set_tooltips(fig, tooltips=(), vline=True, renderers=()):
         tooltips = list(tooltips)
         renderers = list(renderers)
 
         if is_datetime_index:
@@ -281,15 +289,15 @@
             point_policy='follow_mouse',
             renderers=renderers, formatters=formatters,
             tooltips=tooltips, mode='vline' if vline else 'mouse'))
 
     def _plot_equity_section(is_return=False):
         """Equity section"""
         # Max DD Dur. line
-        equity = equity_data['Equity'].copy()
+        equity = equity_data['_Equity'].copy()
         dd_end = equity_data['DrawdownDuration'].idxmax()
         if np.isnan(dd_end):
             dd_start = dd_end = equity.index[0]
         else:
             dd_start = equity[:dd_end].idxmax()
             # If DD not extending into the future, get exact point of intersection with equity
             if dd_end != equity.index[-1]:
@@ -330,26 +338,32 @@
                   source=ColumnDataSource(dict(
                       index=np.r_[index, index[::-1]],
                       equity_dd=np.r_[equity, equity.cummax()[::-1]]
                   )),
                   fill_color='#ffffea', line_color='#ffcb66')
 
         # Equity line
-        r = fig.line('index', source_key, source=source, line_width=1.5, line_alpha=1)
+        r = fig.line('index', source_key, source=source, line_width=1.5, line_alpha=1, legend_label='Strategy')
         if relative_equity:
             tooltip_format = f'@{source_key}{{+0,0.[000]%}}'
             tick_format = '0,0.[00]%'
             legend_format = '{:,.0f}%'
         else:
             tooltip_format = f'@{source_key}{{$ 0,0}}'
             tick_format = '$ 0.0 a'
             legend_format = '${:,.0f}'
         set_tooltips(fig, [(yaxis_label, tooltip_format)], renderers=[r])
         fig.yaxis.formatter = NumeralTickFormatter(format=tick_format)
 
+        # Buy-and-hold reference performance
+        if relative_equity and not is_return:
+            fig.line('index', 'bnh_perf', source=source, line_width=1,
+                     line_alpha=1, color='#666666', legend_label='Buy&Hold')
+            set_tooltips(fig, [(yaxis_label, tooltip_format), ('Buy&Hold', f'@bnh_perf{{+0,0.[000]%}}')], renderers=[r])
+
         # Peaks
         argmax = equity.idxmax()
         fig.scatter(argmax, equity[argmax],
                     legend_label='Peak ({})'.format(
                         legend_format.format(equity[argmax] * (100 if relative_equity else 1))),
                     color='cyan', size=8)
         fig.scatter(index[-1], equity.values[-1],
@@ -368,14 +382,44 @@
                  line_color='red', line_width=2,
                  legend_label=f'Max Dd Dur. ({dd_timedelta_label})'
                  .replace(' 00:00:00', '')
                  .replace('(0 days ', '('))
 
         figs_above_ohlc.append(fig)
 
+    def _plot_equity_stack_section(relative=False):
+        """Equity stack area chart section"""
+        equity = equity_data.iloc[:, 1:-2].copy()
+        names = list(equity.columns)
+        if relative:
+            equity = equity.divide(equity.sum(axis=1), axis=0)
+        equity_source = ColumnDataSource(equity)
+        equity_source.add(data.index, 'datetime')
+
+        yaxis_label = 'Allocation'
+        fig = new_indicator_figure(y_axis_label=yaxis_label, height=60 + 10 * len(names))
+
+        if relative:
+            tooltip_format = [f'@{ticker}{{+0,0.[000]%}}' for ticker in names]
+            tick_format = '0,0.[00]%'
+            equity_source.add(pd.Series(1, index=data.index), 'equity')
+        else:
+            tooltip_format = [f'@{ticker}{{$ 0,0}}' for ticker in names]
+            tick_format = '$ 0.0 a'
+            equity_source.add(equity_data['_Equity'], 'equity')
+
+        cg = colorgen()
+        colors = [next(cg) for _ in range(len(names))]
+        r = fig.line('index', 'equity', source=equity_source, line_width=1, line_alpha=0)
+        fig.varea_stack(stackers=names, x='index', color=colors, legend_label=names, source=equity_source)
+        set_tooltips(fig, list(zip(names, tooltip_format)), renderers=[r])
+        fig.yaxis.formatter = NumeralTickFormatter(format=tick_format)
+
+        figs_above_ohlc.append(fig)
+
     def _plot_drawdown_section():
         """Drawdown section"""
         fig = new_indicator_figure(y_axis_label="Drawdown")
         drawdown = equity_data['DrawdownPct']
         argmax = drawdown.idxmax()
         source.add(drawdown, 'drawdown')
         r = fig.line('index', 'drawdown', source=source, line_width=1.3)
@@ -496,14 +540,17 @@
             label_tooltip_pairs.append((source_name, f'@{{{source_name}}}{{0,0.0[0000]}}'))
             ohlc_extreme_values[source_name] = arr.reset_index(drop=True)
             fig.line(
                 'index', source_name, source=source,
                 legend_label=source_name, line_color=color,
                 line_width=2)
         ohlc_tooltips.extend(label_tooltip_pairs)
+        fig.legend.orientation = "horizontal"
+        fig.legend.background_fill_alpha = 0.8
+        fig.legend.border_line_alpha = 0
 
     def _plot_indicators():
         """Strategy indicators"""
 
         def _too_many_dims(value):
             if value.ndim > 2:
                 warnings.warn(f"Can't plot indicators with >2D ('{value.name}')",
@@ -601,14 +648,17 @@
         return indicator_figs
 
     # Construct figure ...
 
     if plot_equity:
         _plot_equity_section()
 
+    if plot_allocation:
+        _plot_equity_stack_section(relative_allocation)
+
     if plot_return:
         _plot_equity_section(is_return=True)
 
     if plot_drawdown:
         figs_above_ohlc.append(_plot_drawdown_section())
 
     if plot_pl:
```

### Comparing `minitrade-0.1.8/minitrade/backtest/core/_stats.py` & `minitrade-0.1.9/minitrade/backtest/core/_stats.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,41 +32,37 @@
         return 0
     return np.exp(np.log(returns).sum() / (len(returns) or np.nan)) - 1
 
 
 def compute_stats(
         orders: Union[List['Order'], pd.DataFrame],
         trades: Union[List['Trade'], pd.DataFrame],
-        equity: np.ndarray,
+        equity: pd.DataFrame,
         ohlc_data: pd.DataFrame,
         strategy_instance: 'Strategy',
         risk_free_rate: float = 0,
 ) -> pd.Series:
     assert -1 < risk_free_rate < 1
 
     index = ohlc_data.index
-    dd = 1 - equity / np.maximum.accumulate(equity)
+    dd = 1 - equity['_Equity'] / np.maximum.accumulate(equity['_Equity'])
     dd_dur, dd_peaks = compute_drawdown_duration_peaks(pd.Series(dd, index=index))
 
     if isinstance(orders, pd.DataFrame):
         orders_df = orders
     else:
         orders_df = pd.DataFrame({
             'SignalTime': [t.entry_time for t in orders],
             'Ticker': [t.ticker for t in orders],
             'Side': ['Buy' if t.size > 0 else 'Sell' for t in orders],
             'Size': [int(t.size) for t in orders],
             'EntryType': [t.entry_type for t in orders],
         }).set_index('SignalTime')
 
-    equity_df = pd.DataFrame({
-        'Equity': equity,
-        'DrawdownPct': dd,
-        'DrawdownDuration': dd_dur},
-        index=index)
+    equity_df = pd.concat([equity, pd.DataFrame({'DrawdownPct': dd, 'DrawdownDuration': dd_dur}, index=index)], axis=1)
 
     if isinstance(trades, pd.DataFrame):
         trades_df = trades
     else:
         # Came straight from Backtest.run()
         trades_df = pd.DataFrame({
             'EntryBar': [t.entry_bar for t in trades],
@@ -100,29 +96,28 @@
     s.loc['Duration'] = s.End - s.Start
 
     have_position = np.repeat(0, len(index))
     for t in trades_df.itertuples(index=False):
         have_position[t.EntryBar:t.ExitBar + 1] = 1
 
     s.loc['Exposure Time [%]'] = have_position.mean() * 100  # In "n bars" time, not index time
-    s.loc['Equity Final [$]'] = equity[-1]
-    s.loc['Equity Peak [$]'] = equity.max()
-    s.loc['Return [%]'] = (equity[-1] - equity[0]) / equity[0] * 100
+    s.loc['Equity Final [$]'] = equity['_Equity'][-1]
+    s.loc['Equity Peak [$]'] = equity['_Equity'].max()
+    s.loc['Return [%]'] = (equity['_Equity'][-1] - equity['_Equity'][0]) / equity['_Equity'][0] * 100
     c = ohlc_data.Close.values
     s.loc['Buy & Hold Return [%]'] = (c[-1] - c[0]) / c[0] * 100  # long-only return
 
     gmean_day_return: float = 0
     day_returns = np.array(np.nan)
     annual_trading_days = np.nan
     if isinstance(index, pd.DatetimeIndex):
-        day_returns = equity_df['Equity'].resample('D').last().dropna().pct_change()
+        day_returns = equity_df['_Equity'].resample('D').last().dropna().pct_change()
         gmean_day_return = geometric_mean(day_returns)
         annual_trading_days = float(
-            365 if index.dayofweek.to_series().between(5, 6).mean() > 2/7 * .6 else
-            252)
+            365 if index.dayofweek.to_series().between(5, 6).mean() > 2/7 * .6 else 252)
 
     # Annualized return and risk metrics are computed based on the (mostly correct)
     # assumption that the returns are compounded. See: https://dx.doi.org/10.2139/ssrn.3054517
     # Our annualized return matches `empyrical.annual_return(day_returns)` whereas
     # our risk doesn't; they use the simpler approach below.
     annualized_return = (1 + gmean_day_return)**annual_trading_days - 1
     s.loc['Return (Ann.) [%]'] = annualized_return * 100
```

### Comparing `minitrade-0.1.8/minitrade/backtest/core/_util.py` & `minitrade-0.1.9/minitrade/backtest/core/_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,17 +152,17 @@
         return self.__pip
 
     def __get_array(self, key) -> _Array:
         arr = self.__cache.get(key)
         if arr is None:
             array, df = self.__arrays[key]
             if key == '__index':
-                arr = self.__cache[key] = _Indicator(array=array[..., :self.__i], df=lambda: df[:self.__i])
+                arr = self.__cache[key] = _Indicator(array=array[:self.__i], df=lambda: df[:self.__i])
             else:
-                arr = self.__cache[key] = _Indicator(array=array[..., :self.__i], df=lambda: df.iloc[:self.__i])
+                arr = self.__cache[key] = _Indicator(array=array[:self.__i], df=lambda: df.iloc[:self.__i])
         return arr
 
     @property
     def Open(self) -> _Array:
         return self.__get_array('Open')
 
     @property
```

### Comparing `minitrade-0.1.8/minitrade/backtest/core/autoscale_cb.js` & `minitrade-0.1.9/minitrade/backtest/core/autoscale_cb.js`

 * *Files identical despite different names*

### Comparing `minitrade-0.1.8/minitrade/backtest/core/backtesting.py` & `minitrade-0.1.9/minitrade/backtest/core/backtesting.py`

 * *Files 1% similar despite different names*

```diff
@@ -902,15 +902,15 @@
         self._fail_fast = fail_fast
         # percentage of total equity reserved as cash to account for order quantity rounding
         # and sudden price changes
         self._rebalance_cash_reserve = rebalance_cash_reserve
         # minimal percentage value gap to the desired allocation to trigger an order
         self._rebalance_tolerance = rebalance_tolerance
 
-        self._equity = np.tile(np.nan, len(data.index))
+        self._equity = np.tile(np.nan, (len(data.index), len(data.tickers)+2))
         self.orders: List[Order] = []
         self.trades: Dict[str, List[Trade]] = {ticker: [] for ticker in self._data.tickers}
         self.positions: Dict[str, Position] = {ticker: Position(self, ticker) for ticker in self._data.tickers}
         self.closed_trades: List[Trade] = []
 
     def __repr__(self):
         pos = ','.join([f'{k}:{int(p.pl)}' for k, p in self.positions.items()])
@@ -1043,19 +1043,22 @@
         return self._data.now
 
     def next(self, i):
         self._i = i
         self._process_orders()
 
         # Log account equity for the equity curve
-        equity = self.equity()
+        total_equity = self.equity()
+        ticker_equity = [self.equity(ticker) for ticker in self._data.tickers]
+        cash = total_equity - sum(ticker_equity)
+        equity = [total_equity, *ticker_equity, cash]
         self._equity[i] = equity
 
         # If equity is negative, set all to 0 and stop the simulation
-        if equity <= 0:
+        if equity[0] <= 0:
             assert self.margin_available <= 0
             for trade in self.all_trades:
                 self._close_trade(trade, self._data.Close[-1], i)
             self._cash = 0
             self._equity[i:] = 0
             raise _OutOfMoneyError
 
@@ -1489,15 +1492,15 @@
         with np.errstate(invalid='ignore'):
 
             for i in range(start, len(self._data)):
                 # Prepare data and indicators for `next` call
                 data._set_length(i + 1)
                 for attr, indicator in indicator_attrs_np.items():
                     setattr(strategy, attr,
-                            _Indicator(array=indicator[..., : i + 1], df=lambda: indicator_attrs[attr].iloc[: i + 1]))
+                            _Indicator(array=indicator[: i + 1], df=lambda: indicator_attrs[attr].iloc[: i + 1]))
 
                 # Handle orders processing and broker stuff
                 try:
                     broker.next(i)
                 except _OutOfMoneyError:
                     break
 
@@ -1516,18 +1519,24 @@
                 if start < len(self._data):
                     try_(partial(broker.next, i), exception=_OutOfMoneyError)
 
             # Set data back to full length
             # for future `indicator._opts['data'].index` calls to work
             data._set_length(len(self._data))
 
-            equity = pd.Series(broker._equity).bfill().fillna(broker._cash).values
+            equity = pd.DataFrame(broker._equity, index=data.index,
+                                  columns=['_Equity', *data.tickers, '_Cash']).bfill().fillna(broker._cash)
 
-            # TODO change to equal weighed average
-            self._ohlc_ref_data = self._data.groupby(level=1, axis=1).agg(np.mean)
+            # equal weighed average, as if buy and hold an equal weighed portfolio
+            weights = 1 / self._data.xs('Close', axis=1, level=1).iloc[0]
+            weighted_data = self._data.copy()
+            for ticker in weights.index:
+                weighted_data[ticker] = weighted_data[ticker] * weights[ticker]
+            weighted_data = weighted_data.groupby(level=1, axis=1).agg('sum') / weights.sum()
+            self._ohlc_ref_data = weighted_data
 
             self._results = compute_stats(
                 orders=processed_orders,
                 trades=broker.closed_trades,
                 equity=equity,
                 ohlc_data=self._ohlc_ref_data,
                 risk_free_rate=0.0,
@@ -1848,15 +1857,16 @@
 
     def plot(self, *, results: pd.Series = None, filename=None, plot_width=None,
              plot_equity=True, plot_return=False, plot_pl=True,
              plot_volume=False, plot_drawdown=False, plot_trades=True,
              smooth_equity=False, relative_equity=True,
              superimpose: Union[bool, str] = False,
              resample=True, reverse_indicators=False,
-             show_legend=True, open_browser=True):
+             show_legend=True, open_browser=True,
+             plot_allocation=False, relative_allocation=True):
         """
         Plot the progression of the last backtest run.
 
         If `results` is provided, it should be a particular result
         `pd.Series` such as returned by
         `minitrade.backtest.core.backtesting.Backtest.run` or
         `minitrade.backtest.core.backtesting.Backtest.optimize`, otherwise the last
@@ -1927,14 +1937,20 @@
         [TRADES_AGG]: lib.html#backtesting.lib.TRADES_AGG
 
         If `show_legend` is `True`, the resulting plot graphs will contain
         labeled legends.
 
         If `open_browser` is `True`, the resulting `filename` will be
         opened in the default web browser.
+
+        If `plot_allocation` is `True`, the resulting plot will contain
+        an equity allocation graph section. 
+
+        If `relative_allocation` is `True`, scale and label equity allocation graph axis
+        with return percent, not absolute cash-equivalent values.
         """
         if results is None:
             if self._results is None:
                 raise RuntimeError('First issue `backtest.run()` to obtain results.')
             results = self._results
 
         return plot(
@@ -1952,8 +1968,10 @@
             plot_trades=plot_trades,
             smooth_equity=smooth_equity,
             relative_equity=relative_equity,
             superimpose=superimpose,
             resample=resample,
             reverse_indicators=reverse_indicators,
             show_legend=show_legend,
-            open_browser=open_browser)
+            open_browser=open_browser,
+            plot_allocation=plot_allocation,
+            relative_allocation=relative_allocation)
```

### Comparing `minitrade-0.1.8/minitrade/backtest/core/lib.py` & `minitrade-0.1.9/minitrade/backtest/core/lib.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,16 @@
 e.g.
 
     stats['_trades'].resample('1D', on='ExitTime',
                               label='right').agg(TRADES_AGG)
 """
 
 _EQUITY_AGG = {
-    'Equity': 'last',
+    '_Equity': 'last',
+    '_Cash': 'last',
     'DrawdownPct': 'max',
     'DrawdownDuration': 'max',
 }
 
 
 def barssince(condition: Sequence[bool], default=np.inf) -> int:
     """
```

### Comparing `minitrade-0.1.8/minitrade/backtest/core/test/EURUSD.csv` & `minitrade-0.1.9/minitrade/backtest/core/test/EURUSD.csv`

 * *Files identical despite different names*

### Comparing `minitrade-0.1.8/minitrade/backtest/core/test/GOOG.csv` & `minitrade-0.1.9/minitrade/backtest/core/test/GOOG.csv`

 * *Files identical despite different names*

### Comparing `minitrade-0.1.8/minitrade/backtest/core/test/__init__.py` & `minitrade-0.1.9/minitrade/backtest/core/test/__init__.py`

 * *Files identical despite different names*

### Comparing `minitrade-0.1.8/minitrade/backtest/core/test/_test.py` & `minitrade-0.1.9/minitrade/backtest/core/test/_test.py`

 * *Files identical despite different names*

### Comparing `minitrade-0.1.8/minitrade/backtest/utils.py` & `minitrade-0.1.9/minitrade/backtest/utils.py`

 * *Files identical despite different names*

### Comparing `minitrade-0.1.8/minitrade/broker/base.py` & `minitrade-0.1.9/minitrade/broker/base.py`

 * *Files identical despite different names*

### Comparing `minitrade-0.1.8/minitrade/broker/ib.py` & `minitrade-0.1.9/minitrade/broker/ib.py`

 * *Files identical despite different names*

### Comparing `minitrade-0.1.8/minitrade/broker/ibgateway.py` & `minitrade-0.1.9/minitrade/broker/ibgateway.py`

 * *Files identical despite different names*

### Comparing `minitrade-0.1.8/minitrade/cli.py` & `minitrade-0.1.9/minitrade/cli.py`

 * *Files identical despite different names*

### Comparing `minitrade-0.1.8/minitrade/datasource/base.py` & `minitrade-0.1.9/minitrade/datasource/base.py`

 * *Files identical despite different names*

### Comparing `minitrade-0.1.8/minitrade/datasource/yahoo.py` & `minitrade-0.1.9/minitrade/datasource/yahoo.py`

 * *Files identical despite different names*

### Comparing `minitrade-0.1.8/minitrade/minitrade.db.sql` & `minitrade-0.1.9/minitrade/minitrade.db.sql`

 * *Files identical despite different names*

### Comparing `minitrade-0.1.8/minitrade/trader/scheduler.py` & `minitrade-0.1.9/minitrade/trader/scheduler.py`

 * *Files identical despite different names*

### Comparing `minitrade-0.1.8/minitrade/trader/trader.py` & `minitrade-0.1.9/minitrade/trader/trader.py`

 * *Files identical despite different names*

### Comparing `minitrade-0.1.8/minitrade/utils/config.py` & `minitrade-0.1.9/minitrade/utils/config.py`

 * *Files identical despite different names*

### Comparing `minitrade-0.1.8/minitrade/utils/mailjet.py` & `minitrade-0.1.9/minitrade/utils/mailjet.py`

 * *Files identical despite different names*

### Comparing `minitrade-0.1.8/minitrade/utils/mtdb.py` & `minitrade-0.1.9/minitrade/utils/mtdb.py`

 * *Files identical despite different names*

### Comparing `minitrade-0.1.8/minitrade/utils/telegram.py` & `minitrade-0.1.9/minitrade/utils/telegram.py`

 * *Files identical despite different names*

### Comparing `minitrade-0.1.8/pyproject.toml` & `minitrade-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "minitrade"
-version = "0.1.8"
+version = "0.1.9"
 description = "A personal automated trading system"
 authors = ["Wei Wu <dodid@outlook.com>"]
 readme = "README.md"
 license = "AGPL-3.0-or-later"
 repository = "https://github.com/dodid/minitrade"
 homepage = "https://dodid.github.io/minitrade/"
 keywords = ["finance", "investing", "trading", "algorithmic-trading", "backtesting", "backtesting-frameworks", "interactive-brokers"]
```

### Comparing `minitrade-0.1.8/setup.py` & `minitrade-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
  'yfinance>=0.1.93,<0.2.0']
 
 entry_points = \
 {'console_scripts': ['minitrade = minitrade.cli:mtcli']}
 
 setup_kwargs = {
     'name': 'minitrade',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'A personal automated trading system',
     'long_description': "## Minitrade\n\n**[Documentation](https://dodid.github.io/minitrade/)**\n\n- [Minitrade](#minitrade)\n- [Installation](#installation)\n- [Backtesting](#backtesting)\n  - [Single asset strattegy](#single-asset-strattegy)\n  - [Multi-asset strategy](#multi-asset-strategy)\n- [Trading](#trading)\n  - [Launch](#launch)\n  - [Configure](#configure)\n  - [IB gateway](#ib-gateway)\n\n\n**Minitrade** is a personal trading system that supports both strategy backtesting and automated order execution.\n\nIt integrates with [Backtesting.py](https://github.com/kernc/backtesting.py) under the hood, and:\n- Is fully compatible with Backtesting.py strategies with minor adaptions.\n- Supports multi-asset portfolio and rebalancing strategies.\n\nOr it can be used as a full trading system that:\n- Automatically executes trading strategies and submits orders.\n- Manages strategy execution via web console.\n- Runs on very low cost machines. \n\nLimitations as a backtesting framework:\n- Multi-asset strategy only supports long positions and market order. \n\nLimitations (for now) as a trading system:\n- Tested only on Linux\n- Support only daily bar and market-on-open order\n- Support only long positions\n- Support only Interactive Brokers\n\nOn the other hand, Minitrade is intended to be easily hackable to fit individual's needs.\n\n## Installation\n\nMinitrade requires `python=3.10.*`\n\n\nIf only used as a backtesting framework:\n\n    $ pip install minitrade\n\nIf used as a trading system, continue with the following:\n\n    $ minitrade init\n\nFor a detailed setup guide on Ubuntu, check out [Installation](INSTALL.md).\n\n## Backtesting\n\nMinitrade uses [Backtesting.py](https://github.com/kernc/backtesting.py) as the core library for backtesting and adds the capability to implement multi-asset strategies. \n\n### Single asset strattegy\n\nFor single asset strategies, those written for Backtesting.py can be easily adapted to work with Minitrade. The following illustrates what changes are necessary:\n\n```python\nfrom minitrade.backtest import Backtest, Strategy\nfrom minitrade.backtest.core.lib import crossover\n\nfrom minitrade.backtest.core.test import SMA, GOOG\n\n\nclass SmaCross(Strategy):\n    def init(self):\n        price = self.data.Close.df\n        self.ma1 = self.I(SMA, price, 10, overlay=True)\n        self.ma2 = self.I(SMA, price, 20, overlay=True)\n\n    def next(self):\n        if crossover(self.ma1, self.ma2):\n            self.position().close()\n            self.buy()\n        elif crossover(self.ma2, self.ma1):\n            self.position().close()\n            self.sell()\n\n\nbt = Backtest(GOOG, SmaCross, commission=.002)\nstats = bt.run()\nbt.plot()\n```\n\n1. Change to import from minitrade modules. Generally `backtesting` becomes `minitrade.backtest.core`.\n2. Minitrade expects `Volume` data to be always avaiable. `Strategy.data` should be consisted of OHLCV.\n3. Minitrade doesn't try to guess where to plot the indicators. So if you want to overlay the indicators on the main chart, set `overlay=True` explicitly.\n4. `Strategy.position` is no longer a property but a function. Any occurrence of `self.position` should be changed to `self.position()`. \n\nThat's it. Check out [compatibility](docs/compatibility.md) for more details.\n\n![plot of single-asset strategy](https://imgur.com/N3E2d6m.jpg)\n\nAlso note that some original utility functions and strategy classes only make sense for single asset strategy. Don't use those in multi-asset strategies.\n\n### Multi-asset strategy\n\nMinitrade extends `Backtesting.py` to support backtesting of multi-asset strategies. \n\nMulti-asset strategies take a 2-level DataFrame as data input. For example, for a strategy class that intends to invest in AAPL and GOOG as a portfolio, the `self.data` should look like:\n\n```\n$ print(self.data)\n\n                          AAPL                              GOOG \n                          Open  High  Low   Close Volume    Open  High  Low   Close Volume\nDate          \n2018-01-02 00:00:00-05:00 40.39 40.90 40.18 40.89 102223600 52.42 53.35 52.26 53.25 24752000\n2018-01-03 00:00:00-05:00 40.95 41.43 40.82 40.88 118071600 53.22 54.31 53.16 54.12 28604000\n2018-01-04 00:00:00-05:00 40.95 41.18 40.85 41.07 89738400 54.40 54.68 54.20 54.32 20092000\n2018-01-05 00:00:00-05:00 41.17 41.63 41.08 41.54 94640000 54.70 55.21 54.60 55.11 25582000\n2018-01-08 00:00:00-05:00 41.38 41.68 41.28 41.38 82271200 55.11 55.56 55.08 55.35 20952000\n```\n\nLike in `Backtesting.py`, `self.data` is `_Data` type that supports progressively revealing of data, and the raw DataFrame can be accessed by `self.data.df`. \n\nTo facilitate indicator calculation, Minitrade has built-in integration with [pandas_ta](https://github.com/twopirllc/pandas-ta) a TA library. `pandas_ta` is accessible using `.ta` property of any DataFrame. Check out [here](https://github.com/twopirllc/pandas-ta#pandas-ta-dataframe-extension) for usage. `.ta` is also enhanced to support 2-level DataFrames. \n\nFor example,\n\n```\n$ print(self.data.df.ta.sma(3))\n\n                                 AAPL       GOOG\nDate                                            \n2018-01-02 00:00:00-05:00         NaN        NaN\n2018-01-03 00:00:00-05:00         NaN        NaN\n2018-01-04 00:00:00-05:00   40.946616  53.898000\n2018-01-05 00:00:00-05:00   41.163408  54.518500\n2018-01-08 00:00:00-05:00   41.331144  54.926167\n```\n\nEven simpler, `self.data.ta.sma(3)` works the same on `self.data`.\n\n\n`self.I()` can take both DataFrame/Series and functions as arguments to define an indicator. If DataFrame/Series is given as input, it's expected to have exactly the same index as `self.data`. For example,\n\n```\nself.sma = self.I(self.data.df.ta.sma(3), name='SMA_3')\n```\n\nWithin `Strategy.next()`, indicators are returned as type `_Array`, essentially `numpy.ndarray`, same as in `Backtesting.py`. The `.df` accessor returns either `DataFrame` or `Series` of the corresponding value. It's the caller's responsibility to know which exact type should be returned. `.s` accessor is also available but only as a syntax suger to return a `Series`. If the actual data is a DataFrame, `.s` throws a `ValueError`. \n\nA key addition to support multi-asset strategy is a `Strategy.alloc` attribute, which combined with `Strategy.rebalance()` API, allows to specify how cash value should be allocate among the different assets. \n\nHere is an example:\n\n```python\n# This strategy evenly allocates cash into the assets\n# that have the top 2 highest rate-of-change every day, \n# on condition that the ROC is possitive.\n\nclass TopPositiveRoc(Strategy):\n    n = 10\n\n    def init(self):\n        roc = self.data.ta.roc(self.n)\n        self.roc = self.I(roc, name='ROC')\n\n    def next(self):\n        roc = self.roc.df.iloc[-1]\n        self.alloc.add(\n            roc.nlargest(2).index, \n            roc > 0\n        ).equal_weight()\n        self.rebalance()\n```\n\n`self.alloc` keeps track of what assets you want to buy and how much weight you want to assign to each. \n\nAt the beginning of each `Strategy.next()` call, `self.alloc` starts empty. \n\nUse `alloc.add()` to add assets to a candidate pool. `alloc.add()` takes either an index or a boolean Series as input. If it's an index, all asset in the index are added to the pool. If it's a boolean Series, index items having a `True` value are added to the pool. When multiple conditions are specified in the same call, the conditions are joined by logical `AND` and the resulted assets are added the the pool. `alloc.add()` can be called multiple times which means a logical `OR` relation and add all assets involved to the pool. \n\nOnce candidate assets are determined, Call `alloc.equal_weight()` to assign equal weight in term of value to each selected asset.\n\nAnd finally, call `Strategy.rebalance()`, which will look at the current equity value, calculate the target value for each asset, calculate how many shares to buy or sell based on the current long/short positions, and generate orders that will bring the portfolio to the target allocation.\n\nRun the above strategy on some DJIA components: \n\n![plot of multi-asset strategy](https://imgur.com/ecy6yTm.jpg)\n\n## Trading\n\nTrading a strategy manually is demanding. Running backtest, submitting orders, sticking to the plan despite ups and downs, and tracking performance takes not only effort, but also discipline. Minitrade makes it easy by automating the entire process.\n\nMinitrade's trading system consists of 3 modules:\n1. A scheduler, that runs strategies periodically and triggers order submission.\n2. A broker gateway, that interfaces with the broker system (IB in this case) and handles the communication.\n3. A web UI, that allows managing trading plans and monitoring the executions.\n\n### Launch\n\nTo start trading, run the following:\n\n```\n# start scheduler\nminitrade scheduler start\n\n# start ibgateway\nminitrade ib start \n\n# start web UI\nminitrade web\n```\n\nUse `nohup` or other tools to keep the processes running after quiting the shell.\n\nThe web UI can be accessed at: ```http://127.0.0.1:8501```\n\n![Minitrade web UI - trading](https://imgur.com/1oOPcU7.jpg)\n\n![Minitrade web UI - performance ](https://imgur.com/ofc9k4i.jpg)\n\n### Configure \n\nConfiguring the system takes a few steps:\n\n1. Data source\n\n    Test the data source and make sure it works. Currently only Yahoo is supported. If a proxy is needed to visit Yahoo, configure it in the UI.\n\n2. Broker\n\n    Put in the username and password, and give the account an alias. Note the **Account type** selected is only a hint to help remember. Whether it's paper or live depends on the account itself, rather than on what's chosen here. \n\n    A test connection to the broker is made before the account is saved. It verifies if the credentials are correct and a connection can be established successfully. For IB, if two-factor authentication is enabled, a notification will be sent to the mobile phone. Confirming on the mobile to finish login.\n\n    The credentials are saved in a local database. Be sure to secure the access to the server. \n\n    ![Minitrade web UI - performance ](https://imgur.com/Y0lPTQx.jpg)\n\n3. Telegram bot (required)\n\n    Configure a Telegram bot to receive notifications and to control trader execution. Follow [the instructions](https://medium.com/geekculture/generate-telegram-token-for-bot-api-d26faf9bf064) to create a bot, and take note of the token and chat ID. Configure those in web UI. On saving the configuration, a test message will be sent. Setup is successful if the message can be received.\n\n    After changing telegram settings, restart all minitrade processes to make the change effective.\n    \n4. Email provider (optional)\n\n    Configure a **[Mailjet](https://mailjet.com)** account to receive email notifcations about backtesting and trading results. A free-tier account should be enough. Configure authorized senders in Mailjet, otherwise sending will fail. Try use different domains for senders and receivers if free email services like Hotmail, Gmail are used, otherwise, e.g., an email sending from a Hotmail address, through 3rd part servers, to the same or another Hotmail address is likely to be treated as spam and not delivered. Sending from Hotmail address to Gmail address or vice versa increases the chance of going through. On saving the configuration, a test email will be sent. Setup is successful if the email can be received.\n\n5. Strategy\n\n    Strategies are just Python files containing a strategy class implementation inherited from the `Strategy` class. The files can be uploaded via the UI and be made available for defining a trade plan. If a strategy class can't be found, it will show an error. If multiple strategy classes exist in a file, the one to be run should be decorated with `@entry_strategy`. To update a strategy, upload a differnt file with the same filename.\n\n6. Trade plan\n\n    A trade plan provides all necessary information to trade a strategy, including:\n    - which strategy to run\n    - the universe of assets as a list of tickers\n    - which data source to get price data from\n    - which timezone are the assets traded\n    - which date should a backtest starts\n    - which date should a trade order be generated from\n    - at what time of day should a backtest run \n    - which broker account should orders be submitted through\n    - how much initial cash should be invested\n\n    The generic tickers need to be resolved to broker specific instrument IDs. Therefore a connection to broker will be made, which may trigger 2FA authentication. Pay attention to 2FA push on mobile phone if necessary.\n\n    Once everything is defined, a test backtest dryrun will start. It should finish without error, though it will not generate any actual orders. \n\n    If the test run is successful, the trade plan is scheduled to run every Mon-Fri at the specified time. The time should be between market close and next market open and after when EOD market data becomes available from the selected data source. \n\n    Backtests can be triggered at any time without duplicate orders or any other side effects. \n\n    Backtesting and trading can be enabled or disabled via the UI.\n\n    ![Minitrade web UI - trade plan ](https://imgur.com/Zhrakz5.jpg)\n\n\n### IB gateway\n\nMinitrade uses [IB's client portal API](https://www.interactivebrokers.com/en/trading/ib-api.php#client-portal-api) to submit orders. The gateway client will be automatically downloaded and configured when `minitrade init` is run. It handles automatically login via Chrome and Selenium webdriver. \n\nIB automatically disconnects a session after 24 hours or so. Minitrade checks connection status when it needs to interact with IB, i.e. when an order should be submitted or account info is retrieved via web UI. Therefore, Should Minitrade initiates a connection, if dead, automatically, a silent 2FA push notification would be sent to mobile phone at random times, which would be quite easy to miss and result in a login failure. After a few consecutive failed attempts, IB may lock out the account and one has to contact customer service to unlock. \n\nTo avoid this, Minitrade only submits orders where there is already a working connection to a broker. If there is not, Minitrade sends messages via Telegram bot to notify that there are pending orders to be submitted. User should issue `/ib login` command manually to the bot to trigger a login to IB account. The 2FA push notification should be received in a few seconds and user can complete the login process on mobile phone. Once login is successful, Minitrade will be able to submit orders when trader runs again every 20 minutes.\n",
     'author': 'Wei Wu',
     'author_email': 'dodid@outlook.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://dodid.github.io/minitrade/',
```

### Comparing `minitrade-0.1.8/PKG-INFO` & `minitrade-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minitrade
-Version: 0.1.8
+Version: 0.1.9
 Summary: A personal automated trading system
 Home-page: https://dodid.github.io/minitrade/
 License: AGPL-3.0-or-later
 Keywords: finance,investing,trading,algorithmic-trading,backtesting,backtesting-frameworks,interactive-brokers
 Author: Wei Wu
 Author-email: dodid@outlook.com
 Requires-Python: >=3.10,<3.11
```

