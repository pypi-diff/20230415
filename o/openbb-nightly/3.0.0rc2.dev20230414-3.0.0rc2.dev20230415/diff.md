# Comparing `tmp/openbb_nightly-3.0.0rc2.dev20230414.tar.gz` & `tmp/openbb_nightly-3.0.0rc2.dev20230415.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_nightly-3.0.0rc2.dev20230414.tar", max compression
+gzip compressed data, was "openbb_nightly-3.0.0rc2.dev20230415.tar", max compression
```

## Comparing `openbb_nightly-3.0.0rc2.dev20230414.tar` & `openbb_nightly-3.0.0rc2.dev20230415.tar`

### file list

```diff
@@ -1,970 +1,974 @@
--rw-r--r--   0        0        0     1073 2023-04-14 00:08:52.665576 openbb_nightly-3.0.0rc2.dev20230414/LICENSE
--rw-r--r--   0        0        0    18588 2023-04-14 00:08:52.853589 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/SDK_README.md
--rw-r--r--   0        0        0      243 2023-04-14 00:08:52.853589 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/__init__.py
--rw-r--r--   0        0        0        0 2023-04-14 00:08:52.853589 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/account/__init__.py
--rw-r--r--   0        0        0    21588 2023-04-14 00:08:52.853589 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/account/account_controller.py
--rw-r--r--   0        0        0     1769 2023-04-14 00:08:52.853589 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/account/account_view.py
--rw-r--r--   0        0        0        0 2023-04-14 00:08:52.853589 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/alternative/__init__.py
--rw-r--r--   0        0        0     3131 2023-04-14 00:08:52.853589 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/alternative/alt_controller.py
--rw-r--r--   0        0        0        0 2023-04-14 00:08:52.853589 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/alternative/covid/__init__.py
--rw-r--r--   0        0        0     1881 2023-04-14 00:08:52.853589 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/alternative/covid/countries.txt
--rw-r--r--   0        0        0     9347 2023-04-14 00:08:52.857589 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/alternative/covid/covid_controller.py
--rw-r--r--   0        0        0     5387 2023-04-14 00:08:52.857589 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/alternative/covid/covid_model.py
--rw-r--r--   0        0        0     8586 2023-04-14 00:08:52.857589 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/alternative/covid/covid_view.py
--rw-r--r--   0        0        0     1070 2023-04-14 00:08:52.857589 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/alternative/hackernews_model.py
--rw-r--r--   0        0        0     1087 2023-04-14 00:08:52.857589 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/alternative/hackernews_view.py
--rw-r--r--   0        0        0     6752 2023-04-14 00:08:52.857589 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/alternative/oss/github_model.py
--rw-r--r--   0        0        0     3968 2023-04-14 00:08:52.857589 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/alternative/oss/github_view.py
--rw-r--r--   0        0        0     8656 2023-04-14 00:08:52.857589 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/alternative/oss/oss_controller.py
--rw-r--r--   0        0        0     4437 2023-04-14 00:08:52.857589 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/alternative/oss/runa_model.py
--rw-r--r--   0        0        0     4018 2023-04-14 00:08:52.857589 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/alternative/oss/runa_view.py
--rw-r--r--   0        0        0        0 2023-04-14 00:08:52.857589 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/alternative/realestate/__init__.py
--rw-r--r--   0        0        0     9030 2023-04-14 00:08:52.857589 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/alternative/realestate/landRegistry_model.py
--rw-r--r--   0        0        0     3309 2023-04-14 00:08:52.857589 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/alternative/realestate/landRegistry_view.py
--rw-r--r--   0        0        0     8108 2023-04-14 00:08:52.857589 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/alternative/realestate/realestate_controller.py
--rw-r--r--   0        0        0     2718 2023-04-14 00:08:52.857589 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/base_helpers.py
--rw-r--r--   0        0        0       93 2023-04-14 00:08:52.857589 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/common/__init__.py
--rw-r--r--   0        0        0        0 2023-04-14 00:08:52.857589 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/common/behavioural_analysis/__init__.py
--rw-r--r--   0        0        0     1198 2023-04-14 00:08:52.857589 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/common/behavioural_analysis/finbrain_model.py
--rw-r--r--   0        0        0     4394 2023-04-14 00:08:52.857589 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/common/behavioural_analysis/finbrain_view.py
--rw-r--r--   0        0        0     1335 2023-04-14 00:08:52.857589 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/common/behavioural_analysis/finnhub_model.py
--rw-r--r--   0        0        0     1861 2023-04-14 00:08:52.857589 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/common/behavioural_analysis/finnhub_view.py
--rw-r--r--   0        0        0     4131 2023-04-14 00:08:52.857589 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/common/behavioural_analysis/google_model.py
--rw-r--r--   0        0        0     7118 2023-04-14 00:08:52.857589 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/common/behavioural_analysis/google_view.py
--rw-r--r--   0        0        0     5524 2023-04-14 00:08:52.857589 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/common/behavioural_analysis/reddit_helpers.py
--rw-r--r--   0        0        0    18297 2023-04-14 00:08:52.857589 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/common/behavioural_analysis/reddit_model.py
--rw-r--r--   0        0        0    10206 2023-04-14 00:08:52.857589 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/common/behavioural_analysis/reddit_view.py
--rw-r--r--   0        0        0     3239 2023-04-14 00:08:52.857589 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/common/behavioural_analysis/stocktwits_model.py
--rw-r--r--   0        0        0     2898 2023-04-14 00:08:52.857589 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/common/behavioural_analysis/stocktwits_view.py
--rw-r--r--   0        0        0     6160 2023-04-14 00:08:52.857589 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/common/behavioural_analysis/twitter_model.py
--rw-r--r--   0        0        0     5870 2023-04-14 00:08:52.857589 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/common/behavioural_analysis/twitter_view.py
--rw-r--r--   0        0        0     4142 2023-04-14 00:08:52.857589 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/common/common_model.py
--rw-r--r--   0        0        0     3634 2023-04-14 00:08:52.857589 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/common/feedparser_model.py
--rw-r--r--   0        0        0     1242 2023-04-14 00:08:52.857589 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/common/feedparser_view.py
--rw-r--r--   0        0        0     2639 2023-04-14 00:08:52.857589 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/common/newsapi_model.py
--rw-r--r--   0        0        0     1465 2023-04-14 00:08:52.857589 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/common/newsapi_view.py
--rw-r--r--   0        0        0        0 2023-04-14 00:08:52.857589 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/common/quantitative_analysis/__init__.py
--rw-r--r--   0        0        0    19923 2023-04-14 00:08:52.857589 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/common/quantitative_analysis/qa_model.py
--rw-r--r--   0        0        0    32308 2023-04-14 00:08:52.857589 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/common/quantitative_analysis/qa_view.py
--rw-r--r--   0        0        0     3226 2023-04-14 00:08:52.857589 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/common/quantitative_analysis/rolling_model.py
--rw-r--r--   0        0        0    10790 2023-04-14 00:08:52.857589 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/common/quantitative_analysis/rolling_view.py
--rw-r--r--   0        0        0        0 2023-04-14 00:08:52.857589 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/common/technical_analysis/__init__.py
--rw-r--r--   0        0        0     2977 2023-04-14 00:08:52.857589 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/common/technical_analysis/custom_indicators_model.py
--rw-r--r--   0        0        0     4272 2023-04-14 00:08:52.857589 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/common/technical_analysis/custom_indicators_view.py
--rw-r--r--   0        0        0     6427 2023-04-14 00:08:52.857589 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/common/technical_analysis/momentum_model.py
--rw-r--r--   0        0        0    10556 2023-04-14 00:08:52.861590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/common/technical_analysis/momentum_view.py
--rw-r--r--   0        0        0     4179 2023-04-14 00:08:52.861590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/common/technical_analysis/overlap_model.py
--rw-r--r--   0        0        0     4361 2023-04-14 00:08:52.861590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/common/technical_analysis/overlap_view.py
--rw-r--r--   0        0        0     1453 2023-04-14 00:08:52.861590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/common/technical_analysis/ta_helpers.py
--rw-r--r--   0        0        0     1819 2023-04-14 00:08:52.861590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/common/technical_analysis/trend_indicators_model.py
--rw-r--r--   0        0        0     2621 2023-04-14 00:08:52.861590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/common/technical_analysis/trend_indicators_view.py
--rw-r--r--   0        0        0    19962 2023-04-14 00:08:52.861590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/common/technical_analysis/volatility_model.py
--rw-r--r--   0        0        0    10008 2023-04-14 00:08:52.861590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/common/technical_analysis/volatility_view.py
--rw-r--r--   0        0        0     2614 2023-04-14 00:08:52.861590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/common/technical_analysis/volume_model.py
--rw-r--r--   0        0        0     3806 2023-04-14 00:08:52.861590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/common/technical_analysis/volume_view.py
--rw-r--r--   0        0        0     5813 2023-04-14 00:08:52.861590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/common/ultima_newsmonitor_model.py
--rw-r--r--   0        0        0     3886 2023-04-14 00:08:52.861590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/common/ultima_newsmonitor_view.py
--rw-r--r--   0        0        0     2634 2023-04-14 00:08:52.861590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/config_terminal.py
--rw-r--r--   0        0        0        0 2023-04-14 00:08:52.861590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/__init__.py
--rw-r--r--   0        0        0     9829 2023-04-14 00:08:52.861590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/completer/choices.py
--rw-r--r--   0        0        0        0 2023-04-14 00:08:52.861590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/config/__init__.py
--rw-r--r--   0        0        0     1180 2023-04-14 00:08:52.861590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/config/paths.py
--rw-r--r--   0        0        0     2650 2023-04-14 00:08:52.861590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/config/paths_helper.py
--rw-r--r--   0        0        0     9162 2023-04-14 00:08:52.861590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/integration_tests/README.md
--rw-r--r--   0        0        0    21758 2023-04-14 00:08:52.861590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/integration_tests/integration_controller.py
--rw-r--r--   0        0        0        0 2023-04-14 00:08:52.861590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/log/__init__.py
--rw-r--r--   0        0        0        0 2023-04-14 00:08:52.861590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/log/collection/__init__.py
--rw-r--r--   0        0        0     3848 2023-04-14 00:08:52.861590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/log/collection/log_sender.py
--rw-r--r--   0        0        0     3744 2023-04-14 00:08:52.861590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/log/collection/logging_clock.py
--rw-r--r--   0        0        0     3495 2023-04-14 00:08:52.861590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/log/collection/s3_sender.py
--rw-r--r--   0        0        0      166 2023-04-14 00:08:52.861590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/log/constants.py
--rw-r--r--   0        0        0        0 2023-04-14 00:08:52.861590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/log/generation/__init__.py
--rw-r--r--   0        0        0      524 2023-04-14 00:08:52.861590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/log/generation/common.py
--rw-r--r--   0        0        0      525 2023-04-14 00:08:52.861590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/log/generation/custom_logger.py
--rw-r--r--   0        0        0      979 2023-04-14 00:08:52.861590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/log/generation/directories.py
--rw-r--r--   0        0        0      841 2023-04-14 00:08:52.861590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/log/generation/expired_files.py
--rw-r--r--   0        0        0     4896 2023-04-14 00:08:52.861590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/log/generation/formatter_with_exceptions.py
--rw-r--r--   0        0        0     6058 2023-04-14 00:08:52.861590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/log/generation/path_tracking_file_handler.py
--rw-r--r--   0        0        0     4166 2023-04-14 00:08:52.861590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/log/generation/settings.py
--rw-r--r--   0        0        0     1621 2023-04-14 00:08:52.861590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/log/generation/settings_logger.py
--rw-r--r--   0        0        0      396 2023-04-14 00:08:52.861590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/log/generation/user_logger.py
--rw-r--r--   0        0        0      627 2023-04-14 00:08:52.861590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/models/__init__.py
--rw-r--r--   0        0        0     1221 2023-04-14 00:08:52.861590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/models/base_model.py
--rw-r--r--   0        0        0      818 2023-04-14 00:08:52.861590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/models/credentials_model.py
--rw-r--r--   0        0        0     4154 2023-04-14 00:08:52.861590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/models/preferences_model.py
--rw-r--r--   0        0        0     1817 2023-04-14 00:08:52.861590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/models/profile_model.py
--rw-r--r--   0        0        0     1230 2023-04-14 00:08:52.861590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/models/sources_model.py
--rw-r--r--   0        0        0     1753 2023-04-14 00:08:52.861590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/models/system_model.py
--rw-r--r--   0        0        0      562 2023-04-14 00:08:52.861590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/models/user_model.py
--rw-r--r--   0        0        0      200 2023-04-14 00:08:52.861590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/plots/__init__.py
--rw-r--r--   0        0        0   418780 2023-04-14 00:08:52.861590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/plots/assets/Terminal_icon.png
--rw-r--r--   0        0        0      727 2023-04-14 00:08:52.861590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/plots/assets/icon.png
--rw-r--r--   0        0        0    14311 2023-04-14 00:08:52.861590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/plots/backend.py
--rw-r--r--   0        0        0        0 2023-04-14 00:08:52.861590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/plots/config/__init__.py
--rw-r--r--   0        0        0     7156 2023-04-14 00:08:52.861590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/plots/config/openbb_styles.py
--rw-r--r--   0        0        0     3073 2023-04-14 00:08:52.861590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/plots/no_import.py
--rw-r--r--   0        0        0     1261 2023-04-14 00:08:52.861590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/plots/old_table.html
--rw-r--r--   0        0        0    10522 2023-04-14 00:08:52.861590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/plots/plotly.html
--rw-r--r--   0        0        0    63003 2023-04-14 00:08:52.865590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/plots/plotly_helper.py
--rw-r--r--   0        0        0        0 2023-04-14 00:08:52.865590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/plots/plotly_ta/__init__.py
--rw-r--r--   0        0        0     6724 2023-04-14 00:08:52.865590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/plots/plotly_ta/base.py
--rw-r--r--   0        0        0    11358 2023-04-14 00:08:52.865590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/plots/plotly_ta/data_classes.py
--rw-r--r--   0        0        0     8016 2023-04-14 00:08:52.865590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/plots/plotly_ta/plugins/custom_indicators_plugin.py
--rw-r--r--   0        0        0    15173 2023-04-14 00:08:52.865590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/plots/plotly_ta/plugins/momentum_plugin.py
--rw-r--r--   0        0        0     3361 2023-04-14 00:08:52.865590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/plots/plotly_ta/plugins/overlap_plugin.py
--rw-r--r--   0        0        0     5683 2023-04-14 00:08:52.865590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/plots/plotly_ta/plugins/trend_indicators_plugin.py
--rw-r--r--   0        0        0     6868 2023-04-14 00:08:52.865590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/plots/plotly_ta/plugins/volatility_plugin.py
--rw-r--r--   0        0        0     3429 2023-04-14 00:08:52.865590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/plots/plotly_ta/plugins/volume_plugin.py
--rw-r--r--   0        0        0    20689 2023-04-14 00:08:52.865590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/plots/plotly_ta/ta_class.py
--rw-r--r--   0        0        0   704632 2023-04-14 00:08:52.869590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/plots/table.html
--rw-r--r--   0        0        0    13289 2023-04-14 00:08:52.869590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/plots/web/bar_menus.js
--rw-r--r--   0        0        0   289624 2023-04-14 00:08:52.869590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/plots/web/css/fonts/FiraCode-Regular.ttf
--rw-r--r--   0        0        0   286320 2023-04-14 00:08:52.873590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/plots/web/css/fonts/FiraCode-VF.ttf
--rw-r--r--   0        0        0    25728 2023-04-14 00:08:52.873590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/plots/web/css/style.css
--rw-r--r--   0        0        0      151 2023-04-14 00:08:52.873590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/plots/web/css/table.css
--rw-r--r--   0        0        0    16655 2023-04-14 00:08:52.873590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/plots/web/helpers.js
--rw-r--r--   0        0        0    17072 2023-04-14 00:08:52.873590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/plots/web/main.js
--rw-r--r--   0        0        0     3255 2023-04-14 00:08:52.873590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/plots/web/main_table.js
--rw-r--r--   0        0        0    25359 2023-04-14 00:08:52.873590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/plots/web/popups.js
--rw-r--r--   0        0        0     7775 2023-04-14 00:08:52.873590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/scripts/sdk_audit.py
--rw-r--r--   0        0        0        0 2023-04-14 00:08:52.873590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/sdk/__init__.py
--rw-r--r--   0        0        0      450 2023-04-14 00:08:52.873590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/sdk/controllers/__init__.py
--rw-r--r--   0        0        0     2660 2023-04-14 00:08:52.873590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/sdk/controllers/alt_sdk_controller.py
--rw-r--r--   0        0        0    24088 2023-04-14 00:08:52.873590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/sdk/controllers/crypto_sdk_controller.py
--rw-r--r--   0        0        0     1513 2023-04-14 00:08:52.873590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/sdk/controllers/etf_sdk_controller.py
--rw-r--r--   0        0        0     2365 2023-04-14 00:08:52.873590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/sdk/controllers/forex_sdk_controller.py
--rw-r--r--   0        0        0     5128 2023-04-14 00:08:52.873590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/sdk/controllers/portfolio_sdk_controller.py
--rw-r--r--   0        0        0    18177 2023-04-14 00:08:52.873590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/sdk/controllers/stocks_sdk_controller.py
--rw-r--r--   0        0        0      761 2023-04-14 00:08:52.873590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/sdk/models/__init__.py
--rw-r--r--   0        0        0     4308 2023-04-14 00:08:52.873590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/sdk/models/alt_sdk_model.py
--rw-r--r--   0        0        0    42910 2023-04-14 00:08:52.873590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/sdk/models/crypto_sdk_model.py
--rw-r--r--   0        0        0     4497 2023-04-14 00:08:52.873590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/sdk/models/econometrics_sdk_model.py
--rw-r--r--   0        0        0     7975 2023-04-14 00:08:52.873590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/sdk/models/economy_sdk_model.py
--rw-r--r--   0        0        0     2496 2023-04-14 00:08:52.873590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/sdk/models/etf_sdk_model.py
--rw-r--r--   0        0        0     3515 2023-04-14 00:08:52.873590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/sdk/models/fixedincome_sdk_model.py
--rw-r--r--   0        0        0     8550 2023-04-14 00:08:52.873590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/sdk/models/forecast_sdk_model.py
--rw-r--r--   0        0        0     4386 2023-04-14 00:08:52.873590 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/sdk/models/forex_sdk_model.py
--rw-r--r--   0        0        0     1530 2023-04-14 00:08:52.877591 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/sdk/models/funds_sdk_model.py
--rw-r--r--   0        0        0     1067 2023-04-14 00:08:52.877591 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/sdk/models/futures_sdk_model.py
--rw-r--r--   0        0        0     3638 2023-04-14 00:08:52.877591 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/sdk/models/keys_sdk_model.py
--rw-r--r--   0        0        0    10046 2023-04-14 00:08:52.877591 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/sdk/models/portfolio_sdk_model.py
--rw-r--r--   0        0        0     4603 2023-04-14 00:08:52.877591 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/sdk/models/qa_sdk_model.py
--rw-r--r--   0        0        0    32196 2023-04-14 00:08:52.877591 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/sdk/models/stocks_sdk_model.py
--rw-r--r--   0        0        0     7229 2023-04-14 00:08:52.877591 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/sdk/models/ta_sdk_model.py
--rw-r--r--   0        0        0    11508 2023-04-14 00:08:52.877591 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/sdk/sdk_helpers.py
--rw-r--r--   0        0        0    19757 2023-04-14 00:08:52.877591 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/sdk/sdk_init.py
--rw-r--r--   0        0        0    43820 2023-04-14 00:08:52.877591 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/sdk/trail_map.csv
--rw-r--r--   0        0        0     2801 2023-04-14 00:08:52.877591 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/sdk/trail_map_forecasting.csv
--rw-r--r--   0        0        0     1301 2023-04-14 00:08:52.877591 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/sdk/trail_map_optimization.csv
--rw-r--r--   0        0        0     6912 2023-04-14 00:08:52.877591 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/sdk/trailmap.py
--rw-r--r--   0        0        0        0 2023-04-14 00:08:52.877591 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/session/__init__.py
--rw-r--r--   0        0        0     1017 2023-04-14 00:08:52.877591 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/session/banner.txt
--rw-r--r--   0        0        0      602 2023-04-14 00:08:52.877591 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/session/constants.py
--rw-r--r--   0        0        0     1000 2023-04-14 00:08:52.877591 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/session/current_system.py
--rw-r--r--   0        0        0     4095 2023-04-14 00:08:52.877591 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/session/current_user.py
--rw-r--r--   0        0        0     1400 2023-04-14 00:08:52.877591 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/session/env_handler.py
--rw-r--r--   0        0        0    22307 2023-04-14 00:08:52.877591 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/session/hub_model.py
--rw-r--r--   0        0        0     5518 2023-04-14 00:08:52.877591 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/session/local_model.py
--rw-r--r--   0        0        0     5136 2023-04-14 00:08:52.877591 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/session/routines_handler.py
--rw-r--r--   0        0        0     3097 2023-04-14 00:08:52.877591 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/session/sdk_session.py
--rw-r--r--   0        0        0     3026 2023-04-14 00:08:52.877591 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/session/session_controller.py
--rw-r--r--   0        0        0     5958 2023-04-14 00:08:52.877591 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/session/session_model.py
--rw-r--r--   0        0        0     2834 2023-04-14 00:08:52.877591 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/session/sources_handler.py
--rw-r--r--   0        0        0     1677 2023-04-14 00:08:52.877591 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/session/utils.py
--rw-r--r--   0        0        0     3011 2023-04-14 00:08:52.877591 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/sources/utils.py
--rw-r--r--   0        0        0      199 2023-04-14 00:08:52.877591 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/README.md
--rw-r--r--   0        0        0       84 2023-04-14 00:08:52.877591 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/__init__.py
--rw-r--r--   0        0        0     5303 2023-04-14 00:08:52.877591 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/coinbase_helpers.py
--rw-r--r--   0        0        0     2147 2023-04-14 00:08:52.877591 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/coinpaprika_helpers.py
--rw-r--r--   0        0        0    19295 2023-04-14 00:08:52.877591 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/crypto_controller.py
--rw-r--r--   0        0        0     4481 2023-04-14 00:08:52.877591 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/crypto_models.py
--rw-r--r--   0        0        0     1785 2023-04-14 00:08:52.877591 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/crypto_views.py
--rw-r--r--   0        0        0    30342 2023-04-14 00:08:52.877591 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/cryptocurrency_helpers.py
--rw-r--r--   0        0        0      949 2023-04-14 00:08:52.877591 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/data/README.md
--rw-r--r--   0        0        0     7341 2023-04-14 00:08:52.877591 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/data/binance_gecko_map.json
--rw-r--r--   0        0        0     2436 2023-04-14 00:08:52.877591 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/data/coinbase_gecko_map.json
--rw-r--r--   0        0        0     4813 2023-04-14 00:08:52.877591 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/data/coingecko_categories.json
--rw-r--r--   0        0        0   954385 2023-04-14 00:08:52.881591 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/data/coingecko_coins.json
--rw-r--r--   0        0        0  2245016 2023-04-14 00:08:52.893592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/data/coinpaprika_coins.json
--rw-r--r--   0        0        0    31307 2023-04-14 00:08:52.893592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/data/defillama_dapps.json
--rw-r--r--   0        0        0   107203 2023-04-14 00:08:52.893592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/data/erc20_coins.json
--rw-r--r--   0        0        0     7255 2023-04-14 00:08:52.893592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/data/finbrain_coins.json
--rw-r--r--   0        0        0   222978 2023-04-14 00:08:52.893592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/data/santiment_slugs.json
--rw-r--r--   0        0        0   300253 2023-04-14 00:08:52.897592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/data/yahoofinance_coins.json
--rw-r--r--   0        0        0     4951 2023-04-14 00:08:52.897592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/dataframe_helpers.py
--rw-r--r--   0        0        0        0 2023-04-14 00:08:52.897592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/defi/__init__.py
--rw-r--r--   0        0        0     4537 2023-04-14 00:08:52.897592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/defi/coindix_model.py
--rw-r--r--   0        0        0     2720 2023-04-14 00:08:52.897592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/defi/coindix_view.py
--rw-r--r--   0        0        0     2483 2023-04-14 00:08:52.897592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/defi/cryptosaurio_model.py
--rw-r--r--   0        0        0     1994 2023-04-14 00:08:52.897592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/defi/cryptosaurio_view.py
--rw-r--r--   0        0        0    31284 2023-04-14 00:08:52.897592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/defi/defi_controller.py
--rw-r--r--   0        0        0     8918 2023-04-14 00:08:52.897592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/defi/graph_model.py
--rw-r--r--   0        0        0     7165 2023-04-14 00:08:52.897592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/defi/graph_view.py
--rw-r--r--   0        0        0     5005 2023-04-14 00:08:52.897592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/defi/llama_model.py
--rw-r--r--   0        0        0     5827 2023-04-14 00:08:52.897592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/defi/llama_view.py
--rw-r--r--   0        0        0     1808 2023-04-14 00:08:52.897592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/defi/smartstake_model.py
--rw-r--r--   0        0        0     3110 2023-04-14 00:08:52.897592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/defi/smartstake_view.py
--rw-r--r--   0        0        0     2882 2023-04-14 00:08:52.897592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/defi/substack_model.py
--rw-r--r--   0        0        0     1090 2023-04-14 00:08:52.897592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/defi/substack_view.py
--rw-r--r--   0        0        0     1947 2023-04-14 00:08:52.897592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/defi/terraengineer_model.py
--rw-r--r--   0        0        0     2699 2023-04-14 00:08:52.897592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/defi/terraengineer_view.py
--rw-r--r--   0        0        0     9734 2023-04-14 00:08:52.897592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/defi/terramoney_fcd_model.py
--rw-r--r--   0        0        0     8022 2023-04-14 00:08:52.897592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/defi/terramoney_fcd_view.py
--rw-r--r--   0        0        0        0 2023-04-14 00:08:52.897592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/discovery/__init__.py
--rw-r--r--   0        0        0     2317 2023-04-14 00:08:52.897592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/discovery/coinmarketcap_model.py
--rw-r--r--   0        0        0     1620 2023-04-14 00:08:52.897592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/discovery/coinmarketcap_view.py
--rw-r--r--   0        0        0     2116 2023-04-14 00:08:52.897592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/discovery/coinpaprika_model.py
--rw-r--r--   0        0        0     1936 2023-04-14 00:08:52.897592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/discovery/coinpaprika_view.py
--rw-r--r--   0        0        0     7614 2023-04-14 00:08:52.897592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/discovery/dappradar_model.py
--rw-r--r--   0        0        0     5045 2023-04-14 00:08:52.897592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/discovery/dappradar_view.py
--rw-r--r--   0        0        0    21019 2023-04-14 00:08:52.897592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/discovery/discovery_controller.py
--rw-r--r--   0        0        0    10833 2023-04-14 00:08:52.897592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/discovery/pycoingecko_model.py
--rw-r--r--   0        0        0     6352 2023-04-14 00:08:52.897592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/discovery/pycoingecko_view.py
--rw-r--r--   0        0        0     1095 2023-04-14 00:08:52.897592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/discovery/sdk_helpers.py
--rw-r--r--   0        0        0        0 2023-04-14 00:08:52.897592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/due_diligence/__init__.py
--rw-r--r--   0        0        0     7483 2023-04-14 00:08:52.897592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/due_diligence/binance_model.py
--rw-r--r--   0        0        0     3009 2023-04-14 00:08:52.897592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/due_diligence/binance_view.py
--rw-r--r--   0        0        0     3188 2023-04-14 00:08:52.897592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/due_diligence/ccxt_model.py
--rw-r--r--   0        0        0     2840 2023-04-14 00:08:52.897592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/due_diligence/ccxt_view.py
--rw-r--r--   0        0        0     6439 2023-04-14 00:08:52.897592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/due_diligence/coinbase_model.py
--rw-r--r--   0        0        0     4134 2023-04-14 00:08:52.897592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/due_diligence/coinbase_view.py
--rw-r--r--   0        0        0     6587 2023-04-14 00:08:52.897592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/due_diligence/coinglass_model.py
--rw-r--r--   0        0        0     6638 2023-04-14 00:08:52.897592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/due_diligence/coinglass_view.py
--rw-r--r--   0        0        0    15062 2023-04-14 00:08:52.897592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/due_diligence/coinpaprika_model.py
--rw-r--r--   0        0        0     9133 2023-04-14 00:08:52.897592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/due_diligence/coinpaprika_view.py
--rw-r--r--   0        0        0     2332 2023-04-14 00:08:52.897592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/due_diligence/cryptopanic_view.py
--rw-r--r--   0        0        0    64101 2023-04-14 00:08:52.897592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/due_diligence/dd_controller.py
--rw-r--r--   0        0        0     1850 2023-04-14 00:08:52.897592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/due_diligence/due_diligence_api.py
--rw-r--r--   0        0        0     4333 2023-04-14 00:08:52.897592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/due_diligence/finbrain_crypto_view.py
--rw-r--r--   0        0        0    15044 2023-04-14 00:08:52.897592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/due_diligence/glassnode_model.py
--rw-r--r--   0        0        0    11237 2023-04-14 00:08:52.897592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/due_diligence/glassnode_view.py
--rw-r--r--   0        0        0    24480 2023-04-14 00:08:52.897592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/due_diligence/messari_model.py
--rw-r--r--   0        0        0    22260 2023-04-14 00:08:52.897592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/due_diligence/messari_view.py
--rw-r--r--   0        0        0    25887 2023-04-14 00:08:52.897592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/due_diligence/pycoingecko_model.py
--rw-r--r--   0        0        0     8762 2023-04-14 00:08:52.897592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/due_diligence/pycoingecko_view.py
--rw-r--r--   0        0        0     3076 2023-04-14 00:08:52.901592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/due_diligence/santiment_model.py
--rw-r--r--   0        0        0     2070 2023-04-14 00:08:52.901592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/due_diligence/santiment_view.py
--rw-r--r--   0        0        0     2508 2023-04-14 00:08:52.901592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/due_diligence/sdk_helper.py
--rw-r--r--   0        0        0     6001 2023-04-14 00:08:52.901592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/due_diligence/tokenterminal_model.py
--rw-r--r--   0        0        0     3474 2023-04-14 00:08:52.901592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/due_diligence/tokenterminal_view.py
--rw-r--r--   0        0        0        0 2023-04-14 00:08:52.901592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/nft/__init__.py
--rw-r--r--   0        0        0     5562 2023-04-14 00:08:52.901592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/nft/nft_controller.py
--rw-r--r--   0        0        0     1664 2023-04-14 00:08:52.901592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/nft/nftpricefloor_model.py
--rw-r--r--   0        0        0     4495 2023-04-14 00:08:52.901592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/nft/nftpricefloor_view.py
--rw-r--r--   0        0        0     2895 2023-04-14 00:08:52.901592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/nft/opensea_model.py
--rw-r--r--   0        0        0     1289 2023-04-14 00:08:52.901592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/nft/opensea_view.py
--rw-r--r--   0        0        0        0 2023-04-14 00:08:52.901592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/onchain/__init__.py
--rw-r--r--   0        0        0    21848 2023-04-14 00:08:52.901592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/onchain/bitquery_model.py
--rw-r--r--   0        0        0    11444 2023-04-14 00:08:52.901592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/onchain/bitquery_view.py
--rw-r--r--   0        0        0     3393 2023-04-14 00:08:52.901592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/onchain/blockchain_model.py
--rw-r--r--   0        0        0     4733 2023-04-14 00:08:52.901592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/onchain/blockchain_view.py
--rw-r--r--   0        0        0     1840 2023-04-14 00:08:52.901592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/onchain/ethgasstation_model.py
--rw-r--r--   0        0        0     1266 2023-04-14 00:08:52.901592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/onchain/ethgasstation_view.py
--rw-r--r--   0        0        0    15974 2023-04-14 00:08:52.901592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/onchain/ethplorer_model.py
--rw-r--r--   0        0        0    10572 2023-04-14 00:08:52.901592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/onchain/ethplorer_view.py
--rw-r--r--   0        0        0    53494 2023-04-14 00:08:52.901592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/onchain/onchain_controller.py
--rw-r--r--   0        0        0     5938 2023-04-14 00:08:52.901592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/onchain/shroom_model.py
--rw-r--r--   0        0        0     5144 2023-04-14 00:08:52.901592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/onchain/shroom_view.py
--rw-r--r--   0        0        0     4772 2023-04-14 00:08:52.901592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/onchain/whale_alert_model.py
--rw-r--r--   0        0        0     2088 2023-04-14 00:08:52.901592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/onchain/whale_alert_view.py
--rw-r--r--   0        0        0        0 2023-04-14 00:08:52.901592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/overview/__init__.py
--rw-r--r--   0        0        0     2274 2023-04-14 00:08:52.901592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/overview/blockchaincenter_model.py
--rw-r--r--   0        0        0     2664 2023-04-14 00:08:52.901592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/overview/blockchaincenter_view.py
--rw-r--r--   0        0        0     1464 2023-04-14 00:08:52.901592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/overview/coinbase_model.py
--rw-r--r--   0        0        0     1342 2023-04-14 00:08:52.901592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/overview/coinbase_view.py
--rw-r--r--   0        0        0    11841 2023-04-14 00:08:52.901592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/overview/coinpaprika_model.py
--rw-r--r--   0        0        0     9646 2023-04-14 00:08:52.901592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/overview/coinpaprika_view.py
--rw-r--r--   0        0        0     6776 2023-04-14 00:08:52.901592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/overview/cryptopanic_model.py
--rw-r--r--   0        0        0     2278 2023-04-14 00:08:52.901592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/overview/cryptopanic_view.py
--rw-r--r--   0        0        0     1100 2023-04-14 00:08:52.901592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/overview/glassnode_model.py
--rw-r--r--   0        0        0     4677 2023-04-14 00:08:52.901592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/overview/glassnode_view.py
--rw-r--r--   0        0        0     5936 2023-04-14 00:08:52.901592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/overview/loanscan_model.py
--rw-r--r--   0        0        0     3279 2023-04-14 00:08:52.901592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/overview/loanscan_view.py
--rw-r--r--   0        0        0    55381 2023-04-14 00:08:52.901592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/overview/overview_controller.py
--rw-r--r--   0        0        0    13641 2023-04-14 00:08:52.901592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/overview/pycoingecko_model.py
--rw-r--r--   0        0        0    21320 2023-04-14 00:08:52.901592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/overview/pycoingecko_view.py
--rw-r--r--   0        0        0     5346 2023-04-14 00:08:52.901592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/overview/rekt_model.py
--rw-r--r--   0        0        0     2253 2023-04-14 00:08:52.901592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/overview/rekt_view.py
--rw-r--r--   0        0        0     2042 2023-04-14 00:08:52.901592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/overview/sdk_helpers.py
--rw-r--r--   0        0        0     7167 2023-04-14 00:08:52.901592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/overview/tokenterminal_model.py
--rw-r--r--   0        0        0     3126 2023-04-14 00:08:52.901592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/overview/tokenterminal_view.py
--rw-r--r--   0        0        0     6708 2023-04-14 00:08:52.901592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/overview/withdrawalfees_model.py
--rw-r--r--   0        0        0     3480 2023-04-14 00:08:52.901592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/overview/withdrawalfees_view.py
--rw-r--r--   0        0        0     7635 2023-04-14 00:08:52.901592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/pycoingecko_helpers.py
--rw-r--r--   0        0        0     5693 2023-04-14 00:08:52.901592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/pyth_model.py
--rw-r--r--   0        0        0      973 2023-04-14 00:08:52.901592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/pyth_view.py
--rw-r--r--   0        0        0        0 2023-04-14 00:08:52.901592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/quantitative_analysis/__init__.py
--rw-r--r--   0        0        0    26081 2023-04-14 00:08:52.901592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/quantitative_analysis/qa_controller.py
--rw-r--r--   0        0        0        0 2023-04-14 00:08:52.901592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/technical_analysis/__init__.py
--rw-r--r--   0        0        0    54572 2023-04-14 00:08:52.901592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/technical_analysis/ta_controller.py
--rw-r--r--   0        0        0        0 2023-04-14 00:08:52.901592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/tools/__init__.py
--rw-r--r--   0        0        0     6219 2023-04-14 00:08:52.901592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/tools/tools_controller.py
--rw-r--r--   0        0        0     1357 2023-04-14 00:08:52.901592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/tools/tools_helpers.py
--rw-r--r--   0        0        0     3447 2023-04-14 00:08:52.901592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/tools/tools_model.py
--rw-r--r--   0        0        0     2772 2023-04-14 00:08:52.901592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/tools/tools_view.py
--rw-r--r--   0        0        0    16935 2023-04-14 00:08:52.901592 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/custom_prompt_toolkit.py
--rw-r--r--   0        0        0    55138 2023-04-14 00:08:52.905593 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/custom_reports/lunar_crash/coin_highs.png
--rw-r--r--   0        0        0  2879534 2023-04-14 00:08:52.925594 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/custom_reports/lunar_crash/luna_crash.html
--rw-r--r--   0        0        0   350260 2023-04-14 00:08:52.925594 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/custom_reports/lunar_crash/luna_supply.png
--rw-r--r--   0        0        0   607642 2023-04-14 00:08:52.929594 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/custom_reports/lunar_crash/luna_terra.png
--rw-r--r--   0        0        0    11988 2023-04-14 00:08:52.929594 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/custom_reports/lunar_crash/lunatics.ipynb
--rw-r--r--   0        0        0   667206 2023-04-14 00:08:52.933594 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/custom_reports/lunar_crash/tvl.png
--rw-r--r--   0        0        0   465754 2023-04-14 00:08:52.937595 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/custom_reports/lunar_crash/ust_terra.png
--rw-r--r--   0        0        0        0 2023-04-14 00:08:52.937595 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/dashboards/__init__.py
--rw-r--r--   0        0        0     9027 2023-04-14 00:08:52.937595 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/dashboards/dashboards_controller.py
--rw-r--r--   0        0        0    13422 2023-04-14 00:08:52.937595 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/dashboards/stream/Forecasting.py
--rw-r--r--   0        0        0        0 2023-04-14 00:08:52.937595 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/dashboards/stream/__init__.py
--rw-r--r--   0        0        0     3985 2023-04-14 00:08:52.937595 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/dashboards/stream/common_vars.py
--rw-r--r--   0        0        0     4261 2023-04-14 00:08:52.937595 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/dashboards/stream/pages/Chains.py
--rw-r--r--   0        0        0     3322 2023-04-14 00:08:52.937595 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/dashboards/stream/pages/Correlation.py
--rw-r--r--   0        0        0     8106 2023-04-14 00:08:52.937595 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/dashboards/stream/pages/Futures.py
--rw-r--r--   0        0        0    17126 2023-04-14 00:08:52.937595 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/dashboards/stream/pages/Indicators.py
--rw-r--r--   0        0        0     6964 2023-04-14 00:08:52.937595 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/dashboards/stream/pages/Short_Data.py
--rw-r--r--   0        0        0    13224 2023-04-14 00:08:52.937595 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/dashboards/stream/pages/Stocks.py
--rw-r--r--   0        0        0     4093 2023-04-14 00:08:52.937595 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/dashboards/stream/streamlit_helpers.py
--rw-r--r--   0        0        0     1092 2023-04-14 00:08:52.937595 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/dashboards/streamlit.py
--rw-r--r--   0        0        0     5481 2023-04-14 00:08:52.941595 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/dashboards/voila/chains.ipynb
--rw-r--r--   0        0        0     6789 2023-04-14 00:08:52.941595 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/dashboards/voila/correlation.ipynb
--rw-r--r--   0        0        0    13930 2023-04-14 00:08:52.941595 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/dashboards/voila/forecast.ipynb
--rw-r--r--   0        0        0    10953 2023-04-14 00:08:52.941595 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/dashboards/voila/futures.ipynb
--rw-r--r--   0        0        0     9421 2023-04-14 00:08:52.941595 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/dashboards/voila/shortdata.ipynb
--rw-r--r--   0        0        0    15315 2023-04-14 00:08:52.941595 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/dashboards/voila/stocks.ipynb
--rw-r--r--   0        0        0     5091 2023-04-14 00:08:52.941595 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/decorators.py
--rw-r--r--   0        0        0        0 2023-04-14 00:08:52.941595 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/econometrics/__init__.py
--rw-r--r--   0        0        0    73682 2023-04-14 00:08:52.941595 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/econometrics/econometrics_controller.py
--rw-r--r--   0        0        0     2973 2023-04-14 00:08:52.941595 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/econometrics/econometrics_helpers.py
--rw-r--r--   0        0        0    13544 2023-04-14 00:08:52.941595 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/econometrics/econometrics_model.py
--rw-r--r--   0        0        0    16620 2023-04-14 00:08:52.941595 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/econometrics/econometrics_view.py
--rw-r--r--   0        0        0    20449 2023-04-14 00:08:52.941595 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/econometrics/regression_model.py
--rw-r--r--   0        0        0     6739 2023-04-14 00:08:52.941595 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/econometrics/regression_view.py
--rw-r--r--   0        0        0       77 2023-04-14 00:08:52.941595 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/economy/README.md
--rw-r--r--   0        0        0        0 2023-04-14 00:08:52.941595 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/economy/__init__.py
--rw-r--r--   0        0        0    10230 2023-04-14 00:08:52.941595 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/economy/alphavantage_model.py
--rw-r--r--   0        0        0    12075 2023-04-14 00:08:52.941595 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/economy/alphavantage_view.py
--rw-r--r--   0        0        0     1614 2023-04-14 00:08:52.941595 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/economy/commodity_model.py
--rw-r--r--   0        0        0     1561 2023-04-14 00:08:52.941595 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/economy/commodity_view.py
--rw-r--r--   0        0        0      909 2023-04-14 00:08:52.941595 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/economy/datasets/NASDAQ_CountryCodes.csv
--rw-r--r--   0        0        0    21218 2023-04-14 00:08:52.941595 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/economy/datasets/cpi.csv
--rw-r--r--   0        0        0    10355 2023-04-14 00:08:52.941595 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/economy/datasets/harmonized_cpi.csv
--rw-r--r--   0        0        0    28404 2023-04-14 00:08:52.941595 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/economy/econdb_model.py
--rw-r--r--   0        0        0     8013 2023-04-14 00:08:52.941595 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/economy/econdb_view.py
--rw-r--r--   0        0        0    91589 2023-04-14 00:08:52.941595 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/economy/economy_controller.py
--rw-r--r--   0        0        0     3436 2023-04-14 00:08:52.941595 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/economy/economy_helpers.py
--rw-r--r--   0        0        0     7966 2023-04-14 00:08:52.941595 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/economy/finviz_model.py
--rw-r--r--   0        0        0     4600 2023-04-14 00:08:52.941595 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/economy/finviz_view.py
--rw-r--r--   0        0        0     9940 2023-04-14 00:08:52.941595 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/economy/fred_model.py
--rw-r--r--   0        0        0     9117 2023-04-14 00:08:52.941595 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/economy/fred_view.py
--rw-r--r--   0        0        0     6972 2023-04-14 00:08:52.941595 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/economy/nasdaq_model.py
--rw-r--r--   0        0        0     3286 2023-04-14 00:08:52.941595 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/economy/nasdaq_view.py
--rw-r--r--   0        0        0    38418 2023-04-14 00:08:52.941595 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/economy/oecd_model.py
--rw-r--r--   0        0        0    26364 2023-04-14 00:08:52.941595 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/economy/oecd_view.py
--rw-r--r--   0        0        0     3768 2023-04-14 00:08:52.941595 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/economy/plot_view.py
--rw-r--r--   0        0        0        0 2023-04-14 00:08:52.941595 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/economy/quantitative_analysis/__init__.py
--rw-r--r--   0        0        0    28433 2023-04-14 00:08:52.941595 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/economy/quantitative_analysis/qa_controller.py
--rw-r--r--   0        0        0     1218 2023-04-14 00:08:52.941595 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/economy/sdk_helpers.py
--rw-r--r--   0        0        0    12870 2023-04-14 00:08:52.941595 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/economy/wsj_model.py
--rw-r--r--   0        0        0     4673 2023-04-14 00:08:52.941595 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/economy/wsj_view.py
--rw-r--r--   0        0        0    30415 2023-04-14 00:08:52.941595 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/economy/yfinance_model.py
--rw-r--r--   0        0        0     5055 2023-04-14 00:08:52.941595 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/economy/yfinance_view.py
--rw-r--r--   0        0        0      106 2023-04-14 00:08:52.941595 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/etf/README.md
--rw-r--r--   0        0        0        0 2023-04-14 00:08:52.941595 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/etf/__init__.py
--rw-r--r--   0        0        0     4023 2023-04-14 00:08:52.941595 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/etf/discovery/disc_controller.py
--rw-r--r--   0        0        0     2804 2023-04-14 00:08:52.941595 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/etf/discovery/wsj_model.py
--rw-r--r--   0        0        0     1320 2023-04-14 00:08:52.941595 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/etf/discovery/wsj_view.py
--rw-r--r--   0        0        0    21045 2023-04-14 00:08:52.941595 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/etf/etf_controller.py
--rw-r--r--   0        0        0      450 2023-04-14 00:08:52.945595 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/etf/etf_helper.py
--rw-r--r--   0        0        0   188615 2023-04-14 00:08:52.945595 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/etf/etfs.csv
--rw-r--r--   0        0        0     2608 2023-04-14 00:08:52.945595 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/etf/financedatabase_model.py
--rw-r--r--   0        0        0     3864 2023-04-14 00:08:52.945595 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/etf/financedatabase_view.py
--rw-r--r--   0        0        0     1417 2023-04-14 00:08:52.945595 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/etf/fmp_model.py
--rw-r--r--   0        0        0     3152 2023-04-14 00:08:52.945595 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/etf/fmp_view.py
--rw-r--r--   0        0        0     4172 2023-04-14 00:08:52.945595 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/etf/stockanalysis_model.py
--rw-r--r--   0        0        0     3941 2023-04-14 00:08:52.945595 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/etf/stockanalysis_view.py
--rw-r--r--   0        0        0    51458 2023-04-14 00:08:52.945595 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/etf/technical_analysis/ta_controller.py
--rw-r--r--   0        0        0     8025 2023-04-14 00:08:52.945595 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/featflags_controller.py
--rw-r--r--   0        0        0        0 2023-04-14 00:08:52.945595 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/fixedincome/__init__.py
--rw-r--r--   0        0        0    58622 2023-04-14 00:08:52.945595 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/fixedincome/commercial_paper.csv
--rw-r--r--   0        0        0   125899 2023-04-14 00:08:52.945595 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/fixedincome/corporate_spot_rates.csv
--rw-r--r--   0        0        0     9217 2023-04-14 00:08:52.945595 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/fixedincome/ecb_model.py
--rw-r--r--   0        0        0     7096 2023-04-14 00:08:52.945595 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/fixedincome/ecb_view.py
--rw-r--r--   0        0        0     5811 2023-04-14 00:08:52.945595 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/fixedincome/econdb_model.py
--rw-r--r--   0        0        0     7831 2023-04-14 00:08:52.945595 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/fixedincome/econdb_view.py
--rw-r--r--   0        0        0    56207 2023-04-14 00:08:52.945595 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/fixedincome/fixedincome_controller.py
--rw-r--r--   0        0        0    37985 2023-04-14 00:08:52.945595 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/fixedincome/fred_model.py
--rw-r--r--   0        0        0    51962 2023-04-14 00:08:52.945595 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/fixedincome/fred_view.py
--rw-r--r--   0        0        0   227110 2023-04-14 00:08:52.945595 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/fixedincome/ice_bofa_indices.csv
--rw-r--r--   0        0        0    10963 2023-04-14 00:08:52.945595 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/fixedincome/oecd_model.py
--rw-r--r--   0        0        0     3997 2023-04-14 00:08:52.945595 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/fixedincome/oecd_view.py
--rw-r--r--   0        0        0     2174 2023-04-14 00:08:52.945595 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/fixedincome/yfinance_model.py
--rw-r--r--   0        0        0     1702 2023-04-14 00:08:52.949596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/fixedincome/yfinance_view.py
--rw-r--r--   0        0        0        0 2023-04-14 00:08:52.949596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/__init__.py
--rw-r--r--   0        0        0     1547 2023-04-14 00:08:52.949596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/anom_model.py
--rw-r--r--   0        0        0     2962 2023-04-14 00:08:52.949596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/anom_view.py
--rw-r--r--   0        0        0     4629 2023-04-14 00:08:52.949596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/autoarima_model.py
--rw-r--r--   0        0        0     3933 2023-04-14 00:08:52.949596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/autoarima_view.py
--rw-r--r--   0        0        0     4658 2023-04-14 00:08:52.949596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/autoces_model.py
--rw-r--r--   0        0        0     3970 2023-04-14 00:08:52.949596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/autoces_view.py
--rw-r--r--   0        0        0     4694 2023-04-14 00:08:52.949596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/autoets_model.py
--rw-r--r--   0        0        0     3972 2023-04-14 00:08:52.949596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/autoets_view.py
--rw-r--r--   0        0        0     7272 2023-04-14 00:08:52.949596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/autoselect_model.py
--rw-r--r--   0        0        0     3938 2023-04-14 00:08:52.949596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/autoselect_view.py
--rw-r--r--   0        0        0     5874 2023-04-14 00:08:52.949596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/brnn_model.py
--rw-r--r--   0        0        0     6577 2023-04-14 00:08:52.949596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/brnn_view.py
--rw-r--r--   0        0        0     5562 2023-04-14 00:08:52.949596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/expo_model.py
--rw-r--r--   0        0        0     5038 2023-04-14 00:08:52.949596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/expo_view.py
--rw-r--r--   0        0        0     2053 2023-04-14 00:08:52.949596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/forecast.ipynb
--rw-r--r--   0        0        0   121759 2023-04-14 00:08:52.949596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/forecast_controller.py
--rw-r--r--   0        0        0    15471 2023-04-14 00:08:52.949596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/forecast_model.py
--rw-r--r--   0        0        0     9034 2023-04-14 00:08:52.949596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/forecast_view.py
--rw-r--r--   0        0        0    47334 2023-04-14 00:08:52.949596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/helpers.py
--rw-r--r--   0        0        0     3405 2023-04-14 00:08:52.949596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/linregr_model.py
--rw-r--r--   0        0        0     4760 2023-04-14 00:08:52.949596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/linregr_view.py
--rw-r--r--   0        0        0     5013 2023-04-14 00:08:52.949596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/mstl_model.py
--rw-r--r--   0        0        0     3861 2023-04-14 00:08:52.949596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/mstl_view.py
--rw-r--r--   0        0        0     5896 2023-04-14 00:08:52.949596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/nbeats_model.py
--rw-r--r--   0        0        0     6396 2023-04-14 00:08:52.949596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/nbeats_view.py
--rw-r--r--   0        0        0     7561 2023-04-14 00:08:52.949596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/nhits_model.py
--rw-r--r--   0        0        0     7952 2023-04-14 00:08:52.949596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/nhits_view.py
--rw-r--r--   0        0        0     3007 2023-04-14 00:08:52.949596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/regr_model.py
--rw-r--r--   0        0        0     4521 2023-04-14 00:08:52.949596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/regr_view.py
--rw-r--r--   0        0        0     5030 2023-04-14 00:08:52.949596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/rnn_model.py
--rw-r--r--   0        0        0     5533 2023-04-14 00:08:52.949596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/rnn_view.py
--rw-r--r--   0        0        0     4340 2023-04-14 00:08:52.949596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/rwd_model.py
--rw-r--r--   0        0        0     3643 2023-04-14 00:08:52.949596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/rwd_view.py
--rw-r--r--   0        0        0     4709 2023-04-14 00:08:52.949596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/seasonalnaive_model.py
--rw-r--r--   0        0        0     3879 2023-04-14 00:08:52.949596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/seasonalnaive_view.py
--rw-r--r--   0        0        0     5790 2023-04-14 00:08:52.949596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/tcn_model.py
--rw-r--r--   0        0        0     6289 2023-04-14 00:08:52.949596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/tcn_view.py
--rw-r--r--   0        0        0     7249 2023-04-14 00:08:52.949596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/tft_model.py
--rw-r--r--   0        0        0     6520 2023-04-14 00:08:52.949596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/tft_view.py
--rw-r--r--   0        0        0     4928 2023-04-14 00:08:52.949596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/theta_model.py
--rw-r--r--   0        0        0     4379 2023-04-14 00:08:52.949596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/theta_view.py
--rw-r--r--   0        0        0     6321 2023-04-14 00:08:52.949596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/trans_model.py
--rw-r--r--   0        0        0     6765 2023-04-14 00:08:52.949596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/trans_view.py
--rw-r--r--   0        0        0    12580 2023-04-14 00:08:52.949596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/whisper_model.py
--rw-r--r--   0        0        0     2935 2023-04-14 00:08:52.949596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/whisper_utils.py
--rw-r--r--   0        0        0      122 2023-04-14 00:08:52.949596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forex/README.md
--rw-r--r--   0        0        0        0 2023-04-14 00:08:52.949596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forex/__init__.py
--rw-r--r--   0        0        0     5077 2023-04-14 00:08:52.949596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forex/av_model.py
--rw-r--r--   0        0        0     1458 2023-04-14 00:08:52.949596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forex/av_view.py
--rw-r--r--   0        0        0     3281 2023-04-14 00:08:52.949596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forex/data/av_forex_currencies.csv
--rw-r--r--   0        0        0     7847 2023-04-14 00:08:52.949596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forex/data/polygon_tickers.csv
--rw-r--r--   0        0        0   419838 2023-04-14 00:08:52.953596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forex/data/yahoofinance_forex.json
--rw-r--r--   0        0        0    16492 2023-04-14 00:08:52.953596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forex/forex_controller.py
--rw-r--r--   0        0        0     8211 2023-04-14 00:08:52.953596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forex/forex_helper.py
--rw-r--r--   0        0        0      931 2023-04-14 00:08:52.953596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forex/fxempire_model.py
--rw-r--r--   0        0        0     1471 2023-04-14 00:08:52.953596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forex/fxempire_view.py
--rw-r--r--   0        0        0    17162 2023-04-14 00:08:52.953596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forex/oanda/oanda_controller.py
--rw-r--r--   0        0        0    22592 2023-04-14 00:08:52.953596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forex/oanda/oanda_model.py
--rw-r--r--   0        0        0    12856 2023-04-14 00:08:52.953596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forex/oanda/oanda_view.py
--rw-r--r--   0        0        0     2349 2023-04-14 00:08:52.953596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forex/polygon_model.py
--rw-r--r--   0        0        0        0 2023-04-14 00:08:52.953596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forex/quantitative_analysis/__init__.py
--rw-r--r--   0        0        0    26168 2023-04-14 00:08:52.953596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forex/quantitative_analysis/qa_controller.py
--rw-r--r--   0        0        0     1446 2023-04-14 00:08:52.953596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forex/sdk_helpers.py
--rw-r--r--   0        0        0        0 2023-04-14 00:08:52.953596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forex/technical_analysis/__init__.py
--rw-r--r--   0        0        0    35136 2023-04-14 00:08:52.953596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forex/technical_analysis/ta_controller.py
--rw-r--r--   0        0        0        0 2023-04-14 00:08:52.953596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/futures/__init__.py
--rw-r--r--   0        0        0     2218 2023-04-14 00:08:52.953596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/futures/databento_view.py
--rw-r--r--   0        0        0     8903 2023-04-14 00:08:52.953596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/futures/futures_controller.py
--rw-r--r--   0        0        0      358 2023-04-14 00:08:52.953596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/futures/futures_helper.py
--rw-r--r--   0        0        0      964 2023-04-14 00:08:52.953596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/futures/sdk_helper.py
--rw-r--r--   0        0        0     4989 2023-04-14 00:08:52.953596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/futures/yfinance_model.py
--rw-r--r--   0        0        0     7379 2023-04-14 00:08:52.953596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/futures/yfinance_view.py
--rw-r--r--   0        0        0    13288 2023-04-14 00:08:52.953596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/helper_classes.py
--rw-r--r--   0        0        0    67539 2023-04-14 00:08:52.953596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/helper_funcs.py
--rw-r--r--   0        0        0     3212 2023-04-14 00:08:52.953596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/helpers_denomination.py
--rw-r--r--   0        0        0     9736 2023-04-14 00:08:52.953596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/intro.json
--rw-r--r--   0        0        0    42810 2023-04-14 00:08:52.953596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/keys_controller.py
--rw-r--r--   0        0        0    80049 2023-04-14 00:08:52.953596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/keys_model.py
--rw-r--r--   0        0        0     1148 2023-04-14 00:08:52.953596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/keys_view.py
--rw-r--r--   0        0        0     5984 2023-04-14 00:08:52.953596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/loggers.py
--rw-r--r--   0        0        0     1722 2023-04-14 00:08:52.953596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/menu.py
--rw-r--r--   0        0        0        0 2023-04-14 00:08:52.953596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/exports/alternative/covid/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-14 00:08:52.953596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/exports/common/behavioural_analysis/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-14 00:08:52.953596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/exports/common/prediction_techniques/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-14 00:08:52.953596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/exports/common/quantitative_analysis/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-14 00:08:52.953596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/exports/common/technical_analysis/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-14 00:08:52.953596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/exports/custom/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-14 00:08:52.953596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/exports/econometrics/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-14 00:08:52.953596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/exports/economy/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-14 00:08:52.953596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/exports/etf/movers/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-14 00:08:52.953596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/exports/etf/screeners/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-14 00:08:52.953596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/exports/mutual_funds/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-14 00:08:52.953596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/exports/portfolio/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-14 00:08:52.953596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/exports/portfolio/views/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-14 00:08:52.953596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/exports/stocks/backtesting/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-14 00:08:52.953596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/exports/stocks/behavioural_analysis/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-14 00:08:52.953596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/exports/stocks/comparison_analysis/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-14 00:08:52.953596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/exports/stocks/dark_pool_shorts/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-14 00:08:52.953596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/exports/stocks/discovery/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-14 00:08:52.953596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/exports/stocks/due_diligence/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-14 00:08:52.953596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/exports/stocks/fundamental_analysis/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-14 00:08:52.953596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/exports/stocks/government/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-14 00:08:52.953596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/exports/stocks/insider/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-14 00:08:52.953596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/exports/stocks/options/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-14 00:08:52.953596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/exports/stocks/prediction_techniques/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-14 00:08:52.953596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/exports/stocks/quantitative_analysis/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-14 00:08:52.953596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/exports/stocks/raw_data/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/exports/stocks/sector_industry_analysis/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/exports/stocks/technical_analysis/.gitkeep
--rw-r--r--   0        0        0     8528 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/futures/futures.csv
--rw-r--r--   0        0        0    60770 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/i18n/en.yml
--rw-r--r--   0        0        0     5831 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/i18n/help_translation.ipynb
--rw-r--r--   0        0        0        0 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/.gitkeep
--rw-r--r--   0        0        0     3868 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/README.MD
--rw-r--r--   0        0        0       64 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/account/test_account.openbb
--rw-r--r--   0        0        0       87 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/alternative/test_alt_covid.openbb
--rw-r--r--   0        0        0      153 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/alternative/test_alt_oss.openbb
--rw-r--r--   0        0        0      119 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/alternative/test_alt_realestate.openbb
--rw-r--r--   0        0        0      856 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto.openbb
--rw-r--r--   0        0        0      802 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_dd.openbb
--rw-r--r--   0        0        0     1192 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_defi.openbb
--rw-r--r--   0        0        0      374 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_disc.openbb
--rw-r--r--   0        0        0      168 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_nft.openbb
--rw-r--r--   0        0        0     1229 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_onchain.openbb
--rw-r--r--   0        0        0     1533 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_ov.openbb
--rw-r--r--   0        0        0      561 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_qa.openbb
--rw-r--r--   0        0        0       87 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_shroom.openbb
--rw-r--r--   0        0        0      768 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_ta.openbb
--rw-r--r--   0        0        0      154 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_tools.openbb
--rw-r--r--   0        0        0      120 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/dashboards/test_dashboards_base.openbb
--rw-r--r--   0        0        0     1333 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/econometrics/test_econometrics_base.openbb
--rw-r--r--   0        0        0     2082 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/economy/test_economy.openbb
--rw-r--r--   0        0        0      155 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/etf/test_etf.openbb
--rw-r--r--   0        0        0       33 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/etf/test_etf_ca.openbb
--rw-r--r--   0        0        0       38 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/etf/test_etf_disc.openbb
--rw-r--r--   0        0        0      878 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/etf/test_etf_ta.openbb
--rw-r--r--   0        0        0      749 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/fixedincome/test_fixedincome.openbb
--rw-r--r--   0        0        0      301 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/forecast/test_forecast.openbb
--rw-r--r--   0        0        0      176 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/forecast/test_forecast_advanced.openbb
--rw-r--r--   0        0        0      241 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/forex/test_forex_base.openbb
--rw-r--r--   0        0        0      108 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/forex/test_forex_load.openbb
--rw-r--r--   0        0        0      745 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/forex/test_forex_oanda.openbb
--rw-r--r--   0        0        0       62 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/forex/test_forex_oanda_base.openbb
--rw-r--r--   0        0        0      630 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/forex/test_forex_qa.openbb
--rw-r--r--   0        0        0      611 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/forex/test_forex_ta.openbb
--rw-r--r--   0        0        0      173 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/futures/test_futures.openbb
--rw-r--r--   0        0        0     1275 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/portfolio/test_po_show_plot_rpf.openbb
--rw-r--r--   0        0        0     1826 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/portfolio/test_portfolio.openbb
--rw-r--r--   0        0        0       98 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/portfolio/test_portfolio_boolean_args.openbb
--rw-r--r--   0        0        0      683 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/portfolio/test_portfolio_po.openbb
--rw-r--r--   0        0        0       67 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/reports/test_reports_base.openbb
--rw-r--r--   0        0        0       65 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/reports/test_reports_crypto.openbb
--rw-r--r--   0        0        0      151 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/reports/test_reports_economy.openbb
--rw-r--r--   0        0        0       83 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/reports/test_reports_equity.openbb
--rw-r--r--   0        0        0      113 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/reports/test_reports_etf.openbb
--rw-r--r--   0        0        0      174 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/reports/test_reports_forecast.openbb
--rw-r--r--   0        0        0      158 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/reports/test_reports_forex.openbb
--rw-r--r--   0        0        0      132 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/reports/test_reports_portfolio.openbb
--rw-r--r--   0        0        0      102 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/reports/test_reports_run.openbb
--rw-r--r--   0        0        0      258 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks.openbb
--rw-r--r--   0        0        0      255 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_ba.openbb
--rw-r--r--   0        0        0     1513 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_bt.openbb
--rw-r--r--   0        0        0      422 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_ca.openbb
--rw-r--r--   0        0        0      251 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_disc.openbb
--rw-r--r--   0        0        0      145 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_dps.openbb
--rw-r--r--   0        0        0     1874 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_fa.openbb
--rw-r--r--   0        0        0       44 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_fa_base.openbb
--rw-r--r--   0        0        0       31 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_fa_epsfc.openbb
--rw-r--r--   0        0        0       31 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_fa_revfc.openbb
--rw-r--r--   0        0        0      470 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_gov.openbb
--rw-r--r--   0        0        0      276 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_ins.openbb
--rw-r--r--   0        0        0      340 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_options.openbb
--rw-r--r--   0        0        0       91 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_options_payoff.openbb
--rw-r--r--   0        0        0      121 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_options_pricing.openbb
--rw-r--r--   0        0        0       82 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_options_screen.openbb
--rw-r--r--   0        0        0      644 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_qa.openbb
--rw-r--r--   0        0        0      170 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_scr.openbb
--rw-r--r--   0        0        0      347 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_sia.openbb
--rw-r--r--   0        0        0      717 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_ta.openbb
--rw-r--r--   0        0        0       82 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_th.openbb
--rw-r--r--   0        0        0       65 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/test_jupyter_base.openbb
--rw-r--r--   0        0        0       16 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/test_keys_.openbb
--rw-r--r--   0        0        0       46 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/test_news.openbb
--rw-r--r--   0        0        0     1072 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/models/hub_credentials.json
--rw-r--r--   0        0        0      380 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/models/local_credentials.json
--rw-r--r--   0        0        0    17970 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/portfolio/allocation_example.xlsx
--rw-r--r--   0        0        0    29757 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/portfolio/holdings_example.xlsx
--rw-r--r--   0        0        0      310 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/routines/routine_example.openbb
--rw-r--r--   0        0        0    22198 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/sources/openbb_default.json
--rw-r--r--   0        0        0     2332 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/insider/Agriculture.ini
--rw-r--r--   0        0        0     2354 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/insider/Agro-Chemicals.ini
--rw-r--r--   0        0        0     2341 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/insider/Air-Transportation.ini
--rw-r--r--   0        0        0     2316 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/insider/Apparel.ini
--rw-r--r--   0        0        0     2316 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/insider/Banks.ini
--rw-r--r--   0        0        0     2346 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/insider/Brokers.ini
--rw-r--r--   0        0        0     2336 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/insider/Building-Materials.ini
--rw-r--r--   0        0        0     2346 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/insider/Business-Services.ini
--rw-r--r--   0        0        0     2307 2023-04-14 00:08:52.957596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/insider/Closed-End-Funds.ini
--rw-r--r--   0        0        0     2309 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/insider/Construction.ini
--rw-r--r--   0        0        0     2329 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/insider/Credit-Industry.ini
--rw-r--r--   0        0        0     2353 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/insider/Durable-Goods.ini
--rw-r--r--   0        0        0     2360 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/insider/Electronics.ini
--rw-r--r--   0        0        0     2320 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/insider/Furniture.ini
--rw-r--r--   0        0        0     2344 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/insider/Gold-Silver.ini
--rw-r--r--   0        0        0     2315 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/insider/Grocery.ini
--rw-r--r--   0        0        0     2346 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/insider/Ground-Freight.ini
--rw-r--r--   0        0        0     2376 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/insider/Guided-Missiles.ini
--rw-r--r--   0        0        0     2326 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/insider/Health.ini
--rw-r--r--   0        0        0     2307 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/insider/Hotels.ini
--rw-r--r--   0        0        0     2320 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/insider/Insurance-Agents.ini
--rw-r--r--   0        0        0     2324 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/insider/Insurance-Carriers.ini
--rw-r--r--   0        0        0     2334 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/insider/Investment-Offices.ini
--rw-r--r--   0        0        0     2324 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/insider/Legal.ini
--rw-r--r--   0        0        0     2313 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/insider/Lumber.ini
--rw-r--r--   0        0        0     2341 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/insider/Manufacturing.ini
--rw-r--r--   0        0        0     2296 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/insider/Mining.ini
--rw-r--r--   0        0        0     2367 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/insider/Mortgages.ini
--rw-r--r--   0        0        0     2342 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/insider/Nondurable-Goods.ini
--rw-r--r--   0        0        0     2361 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/insider/Personal-Credit.ini
--rw-r--r--   0        0        0     2351 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/insider/Pharmaceuticals.ini
--rw-r--r--   0        0        0     2336 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/insider/Professional-Services.ini
--rw-r--r--   0        0        0     2322 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/insider/Railroads.ini
--rw-r--r--   0        0        0     2310 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/insider/Real-Estate.ini
--rw-r--r--   0        0        0     2326 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/insider/Restaurants.ini
--rw-r--r--   0        0        0     2341 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/insider/Retail-Stores.ini
--rw-r--r--   0        0        0     2299 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/insider/Retail-Trade.ini
--rw-r--r--   0        0        0     2316 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/insider/Tobacco.ini
--rw-r--r--   0        0        0     2342 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/insider/Utility-Communications.ini
--rw-r--r--   0        0        0     2381 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/insider/Utility-Gas.ini
--rw-r--r--   0        0        0     2314 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/insider/Wholesale-Trade.ini
--rw-r--r--   0        0        0    34473 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/insider/template.ini
--rw-r--r--   0        0        0    34519 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/insider/whales.ini
--rw-r--r--   0        0        0     2688 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/options/README.md
--rw-r--r--   0        0        0     4195 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/options/high_iv.ini
--rw-r--r--   0        0        0     4210 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/options/iv_below_20day.ini
--rw-r--r--   0        0        0     3925 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/options/liquid_otm.ini
--rw-r--r--   0        0        0     4202 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/options/spy_30_delta.ini
--rw-r--r--   0        0        0     4079 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/options/template.ini
--rwxr-xr-x   0        0        0      282 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/screener/5pct_above_low.ini
--rw-r--r--   0        0        0    21940 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/screener/all_parameters.txt
--rwxr-xr-x   0        0        0      315 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/screener/analyst_strong_buy.ini
--rwxr-xr-x   0        0        0      464 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/screener/break_out_stocks.ini
--rw-r--r--   0        0        0      413 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/screener/buffett_like.ini
--rwxr-xr-x   0        0        0      184 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/screener/bull_runs_over_10pct.ini
--rwxr-xr-x   0        0        0      364 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/screener/channel_up_and_low_debt_and_sma_50and200.ini
--rw-r--r--   0        0        0      326 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/screener/cheap_bottom_dividend.ini
--rw-r--r--   0        0        0      193 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/screener/cheap_dividend.ini
--rw-r--r--   0        0        0      241 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/screener/cheap_oversold.ini
--rwxr-xr-x   0        0        0      335 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/screener/continued_momentum_scan.ini
--rw-r--r--   0        0        0      286 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/screener/death_cross.ini
--rwxr-xr-x   0        0        0      167 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/screener/djia_components.ini
--rw-r--r--   0        0        0      221 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/screener/golden_cross.ini
--rwxr-xr-x   0        0        0      255 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/screener/golden_cross_penny.ini
--rwxr-xr-x   0        0        0      518 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/screener/growth_stocks.ini
--rw-r--r--   0        0        0      302 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/screener/heavy_inst_ins.ini
--rwxr-xr-x   0        0        0      279 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/screener/high_vol_and_low_debt.ini
--rw-r--r--   0        0        0      316 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/screener/modified_dreman.ini
--rw-r--r--   0        0        0      349 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/screener/modified_neff.ini
--rwxr-xr-x   0        0        0      295 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/screener/news_scanner.ini
--rwxr-xr-x   0        0        0      274 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/screener/oversold.ini
--rwxr-xr-x   0        0        0      328 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/screener/oversold_under_3dol.ini
--rwxr-xr-x   0        0        0      301 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/screener/oversold_under_5dol.ini
--rwxr-xr-x   0        0        0      212 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/screener/potential_reversals.ini
--rwxr-xr-x   0        0        0      295 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/screener/recent_growth_and_support.ini
--rw-r--r--   0        0        0      337 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/screener/rosenwald.ini
--rw-r--r--   0        0        0      280 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/screener/rosenwald_gtfo.ini
--rw-r--r--   0        0        0      246 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/screener/sdk_guide_preset.ini
--rw-r--r--   0        0        0      360 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/screener/sexy_year.ini
--rwxr-xr-x   0        0        0      222 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/screener/short_squeeze_scan.ini
--rwxr-xr-x   0        0        0      260 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/screener/simplistic_momentum_scanner_under_7dol.ini
--rwxr-xr-x   0        0        0      197 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/screener/sp500_basic_materials_sector.ini
--rwxr-xr-x   0        0        0      211 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/screener/sp500_communication_services_sector.ini
--rwxr-xr-x   0        0        0      201 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/screener/sp500_consumer_cyclical_sector.ini
--rwxr-xr-x   0        0        0      203 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/screener/sp500_consumer_defensive_sector.ini
--rwxr-xr-x   0        0        0      179 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/screener/sp500_energy_sector.ini
--rwxr-xr-x   0        0        0      185 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/screener/sp500_financial_sector.ini
--rwxr-xr-x   0        0        0      187 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/screener/sp500_healthcare_sector.ini
--rwxr-xr-x   0        0        0      189 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/screener/sp500_industrials_sector.ini
--rwxr-xr-x   0        0        0      189 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/screener/sp500_real_estate_sector.ini
--rwxr-xr-x   0        0        0      187 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/screener/sp500_technology_sector.ini
--rwxr-xr-x   0        0        0      185 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/screener/sp500_utilities_sector.ini
--rwxr-xr-x   0        0        0      276 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/screener/stocks_strong_support_levels.ini
--rwxr-xr-x   0        0        0      272 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/screener/top_performers_all.ini
--rwxr-xr-x   0        0        0      299 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/screener/top_performers_healthcare.ini
--rwxr-xr-x   0        0        0      293 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/screener/top_performers_tech.ini
--rwxr-xr-x   0        0        0      286 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/screener/under_15dol_stocks.ini
--rw-r--r--   0        0        0      209 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/screener/undervalue.ini
--rwxr-xr-x   0        0        0      272 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/screener/unusual_volume.ini
--rwxr-xr-x   0        0        0      675 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/screener/value_stocks.ini
--rwxr-xr-x   0        0        0      315 2023-04-14 00:08:52.961596 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/screener/weak_support_and_top_performers.ini
--rw-r--r--   0        0        0   358460 2023-04-14 00:08:52.965597 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/styles/default/Consolas.ttf
--rw-r--r--   0        0        0      972 2023-04-14 00:08:52.965597 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/styles/default/dark.mpfstyle.json
--rw-r--r--   0        0        0      182 2023-04-14 00:08:52.965597 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/styles/default/dark.mplrc.json
--rw-r--r--   0        0        0     2086 2023-04-14 00:08:52.965597 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/styles/default/dark.mplstyle
--rw-r--r--   0        0        0     2750 2023-04-14 00:08:52.965597 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/styles/default/dark.pltstyle.json
--rw-r--r--   0        0        0      203 2023-04-14 00:08:52.965597 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/styles/default/dark.richstyle.json
--rw-r--r--   0        0        0      970 2023-04-14 00:08:52.965597 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/styles/default/light.mpfstyle.json
--rw-r--r--   0        0        0      182 2023-04-14 00:08:52.965597 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/styles/default/light.mplrc.json
--rw-r--r--   0        0        0     2035 2023-04-14 00:08:52.965597 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/styles/default/light.mplstyle
--rw-r--r--   0        0        0    24077 2023-04-14 00:08:52.965597 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/styles/default/light.pltstyle.json
--rw-r--r--   0        0        0      202 2023-04-14 00:08:52.965597 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/styles/default/light.richstyle.json
--rw-r--r--   0        0        0     2607 2023-04-14 00:08:52.965597 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/styles/default/tables.pltstyle.json
--rw-r--r--   0        0        0      186 2023-04-14 00:08:52.965597 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/styles/user/openbb.richstyle.json
--rw-r--r--   0        0        0      144 2023-04-14 00:08:52.965597 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/mutual_funds/README.md
--rw-r--r--   0        0        0        0 2023-04-14 00:08:52.965597 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/mutual_funds/__init__.py
--rw-r--r--   0        0        0    81373 2023-04-14 00:08:52.965597 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/mutual_funds/avanza_fund_ID.csv
--rw-r--r--   0        0        0      834 2023-04-14 00:08:52.965597 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/mutual_funds/avanza_model.py
--rw-r--r--   0        0        0     3941 2023-04-14 00:08:52.965597 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/mutual_funds/avanza_view.py
--rw-r--r--   0        0        0     6535 2023-04-14 00:08:52.965597 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/mutual_funds/mstarpy_model.py
--rw-r--r--   0        0        0     7883 2023-04-14 00:08:52.965597 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/mutual_funds/mstarpy_view.py
--rw-r--r--   0        0        0    15141 2023-04-14 00:08:52.965597 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/mutual_funds/mutual_fund_controller.py
--rw-r--r--   0        0        0     6040 2023-04-14 00:08:52.965597 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/mutual_funds/mutual_funds_utils.py
--rw-r--r--   0        0        0    51056 2023-04-14 00:08:52.965597 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/parent_classes.py
--rw-r--r--   0        0        0       61 2023-04-14 00:08:52.965597 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/portfolio/__init__.py
--rw-r--r--   0        0        0    15080 2023-04-14 00:08:52.969597 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/portfolio/allocation_model.py
--rw-r--r--   0        0        0    12944 2023-04-14 00:08:52.969597 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/portfolio/attribution_model.py
--rw-r--r--   0        0        0      417 2023-04-14 00:08:52.969597 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/portfolio/brokers/README.md
--rw-r--r--   0        0        0        0 2023-04-14 00:08:52.969597 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/portfolio/brokers/__init__.py
--rw-r--r--   0        0        0     3214 2023-04-14 00:08:52.969597 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/portfolio/brokers/bro_controller.py
--rw-r--r--   0        0        0     1121 2023-04-14 00:08:52.969597 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/portfolio/brokers/brokers_helpers.py
--rw-r--r--   0        0        0        0 2023-04-14 00:08:52.969597 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/portfolio/brokers/coinbase/__init__.py
--rw-r--r--   0        0        0     8211 2023-04-14 00:08:52.969597 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/portfolio/brokers/coinbase/coinbase_controller.py
--rw-r--r--   0        0        0     9561 2023-04-14 00:08:52.969597 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/portfolio/brokers/coinbase/coinbase_model.py
--rw-r--r--   0        0        0     4495 2023-04-14 00:08:52.969597 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/portfolio/brokers/coinbase/coinbase_view.py
--rw-r--r--   0        0        0     4666 2023-04-14 00:08:52.969597 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/portfolio/brokers/degiro/README.md
--rw-r--r--   0        0        0        0 2023-04-14 00:08:52.969597 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/portfolio/brokers/degiro/__init__.py
--rw-r--r--   0        0        0    12789 2023-04-14 00:08:52.969597 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/portfolio/brokers/degiro/degiro_controller.py
--rw-r--r--   0        0        0    15571 2023-04-14 00:08:52.969597 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/portfolio/brokers/degiro/degiro_model.py
--rw-r--r--   0        0        0    15670 2023-04-14 00:08:52.969597 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/portfolio/brokers/degiro/degiro_view.py
--rw-r--r--   0        0        0     3894 2023-04-14 00:08:52.969597 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/portfolio/brokers/robinhood/robinhood_controller.py
--rw-r--r--   0        0        0     3002 2023-04-14 00:08:52.969597 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/portfolio/brokers/robinhood/robinhood_model.py
--rw-r--r--   0        0        0     2482 2023-04-14 00:08:52.969597 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/portfolio/brokers/robinhood/robinhood_view.py
--rw-r--r--   0        0        0    30861 2023-04-14 00:08:52.969597 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/portfolio/metrics_model.py
--rw-r--r--   0        0        0    54979 2023-04-14 00:08:52.969597 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/portfolio/portfolio_controller.py
--rw-r--r--   0        0        0    39188 2023-04-14 00:08:52.969597 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/portfolio/portfolio_engine.py
--rw-r--r--   0        0        0     9643 2023-04-14 00:08:52.969597 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/portfolio/portfolio_helper.py
--rw-r--r--   0        0        0    60205 2023-04-14 00:08:52.969597 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/portfolio/portfolio_model.py
--rw-r--r--   0        0        0        0 2023-04-14 00:08:52.969597 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/portfolio/portfolio_optimization/__init__.py
--rw-r--r--   0        0        0     5255 2023-04-14 00:08:52.969597 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/portfolio/portfolio_optimization/excel_model.py
--rw-r--r--   0        0        0     2106 2023-04-14 00:08:52.969597 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/portfolio/portfolio_optimization/optimizer_helper.py
--rw-r--r--   0        0        0   120571 2023-04-14 00:08:52.969597 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/portfolio/portfolio_optimization/optimizer_model.py
--rw-r--r--   0        0        0   155050 2023-04-14 00:08:52.969597 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/portfolio/portfolio_optimization/optimizer_view.py
--rw-r--r--   0        0        0     2773 2023-04-14 00:08:52.969597 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/portfolio/portfolio_optimization/parameters/Parameter.py
--rw-r--r--   0        0        0    13116 2023-04-14 00:08:52.969597 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/portfolio/portfolio_optimization/parameters/params_controller.py
--rw-r--r--   0        0        0     5965 2023-04-14 00:08:52.969597 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/portfolio/portfolio_optimization/parameters/params_helpers.py
--rw-r--r--   0        0        0     5346 2023-04-14 00:08:52.969597 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/portfolio/portfolio_optimization/parameters/params_statics.py
--rw-r--r--   0        0        0     4427 2023-04-14 00:08:52.969597 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/portfolio/portfolio_optimization/parameters/params_view.py
--rw-r--r--   0        0        0   138034 2023-04-14 00:08:52.969597 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/portfolio/portfolio_optimization/po_controller.py
--rw-r--r--   0        0        0     8587 2023-04-14 00:08:52.969597 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/portfolio/portfolio_optimization/po_engine.py
--rw-r--r--   0        0        0   103568 2023-04-14 00:08:52.969597 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/portfolio/portfolio_optimization/po_model.py
--rw-r--r--   0        0        0    24186 2023-04-14 00:08:52.973597 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/portfolio/portfolio_optimization/po_view.py
--rw-r--r--   0        0        0    11390 2023-04-14 00:08:52.973597 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/portfolio/portfolio_optimization/statics.py
--rw-r--r--   0        0        0    12009 2023-04-14 00:08:52.973597 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/portfolio/portfolio_optimization/yahoo_finance_model.py
--rw-r--r--   0        0        0    54944 2023-04-14 00:08:52.973597 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/portfolio/portfolio_view.py
--rw-r--r--   0        0        0     8433 2023-04-14 00:08:52.973597 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/portfolio/statics.py
--rw-r--r--   0        0        0     2877 2023-04-14 00:08:52.973597 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/reporting.md
--rw-r--r--   0        0        0  1028287 2023-04-14 00:08:52.977597 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/reports/.ipynb_checkpoints/test-checkpoint.html
--rw-r--r--   0        0        0     2839 2023-04-14 00:08:52.977597 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/reports/README.md
--rw-r--r--   0        0        0        0 2023-04-14 00:08:52.977597 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/reports/__init__.py
--rw-r--r--   0        0        0      443 2023-04-14 00:08:52.977597 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/reports/data/crypto_tickers.csv
--rw-r--r--   0        0        0      437 2023-04-14 00:08:52.977597 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/reports/data/etf_tickers.csv
--rw-r--r--   0        0        0      222 2023-04-14 00:08:52.977597 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/reports/data/stocks_tickers.csv
--rw-r--r--   0        0        0     9707 2023-04-14 00:08:52.977597 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/reports/reports_controller.py
--rw-r--r--   0        0        0    12310 2023-04-14 00:08:52.977597 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/reports/reports_model.py
--rw-r--r--   0        0        0        0 2023-04-14 00:08:52.977597 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/reports/stored/.gitkeep
--rw-r--r--   0        0        0  1076317 2023-04-14 00:08:52.985598 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/reports/stored/20220512_040312_equity_NVDA.html
--rw-r--r--   0        0        0     5214 2023-04-14 00:08:52.985598 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/reports/templates/OpenBB_reports_logo.png
--rw-r--r--   0        0        0    32656 2023-04-14 00:08:52.985598 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/reports/templates/crypto.ipynb
--rw-r--r--   0        0        0    23095 2023-04-14 00:08:52.985598 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/reports/templates/economy.ipynb
--rw-r--r--   0        0        0    39786 2023-04-14 00:08:52.985598 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/reports/templates/equity.ipynb
--rw-r--r--   0        0        0     9900 2023-04-14 00:08:52.985598 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/reports/templates/etf.ipynb
--rw-r--r--   0        0        0     2782 2023-04-14 00:08:52.985598 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/reports/templates/floppy-disc.png
--rw-r--r--   0        0        0     8567 2023-04-14 00:08:52.985598 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/reports/templates/forecast.ipynb
--rw-r--r--   0        0        0    17778 2023-04-14 00:08:52.985598 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/reports/templates/forex.ipynb
--rw-r--r--   0        0        0    14922 2023-04-14 00:08:52.985598 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/reports/templates/portfolio.ipynb
--rw-r--r--   0        0        0    11247 2023-04-14 00:08:52.985598 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/reports/widget_helpers.py
--rw-r--r--   0        0        0      205 2023-04-14 00:08:52.985598 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/reports/widgets/card.j2
--rw-r--r--   0        0        0     3556 2023-04-14 00:08:52.985598 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/reports/widgets/report.css
--rw-r--r--   0        0        0      474 2023-04-14 00:08:52.985598 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/reports/widgets/report.j2
--rw-r--r--   0        0        0      119 2023-04-14 00:08:52.985598 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/reports/widgets/row.j2
--rw-r--r--   0        0        0      896 2023-04-14 00:08:52.985598 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/reports/widgets/style.css
--rw-r--r--   0        0        0     9967 2023-04-14 00:08:52.985598 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/rich_config.py
--rw-r--r--   0        0        0    30911 2023-04-14 00:08:52.985598 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/sdk.py
--rw-r--r--   0        0        0    22661 2023-04-14 00:08:52.985598 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/settings_controller.py
--rw-r--r--   0        0        0     7105 2023-04-14 00:08:52.985598 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/sources_controller.py
--rw-r--r--   0        0        0      357 2023-04-14 00:08:52.985598 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/README.md
--rw-r--r--   0        0        0        0 2023-04-14 00:08:52.985598 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/__init__.py
--rw-r--r--   0        0        0        0 2023-04-14 00:08:52.985598 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/backtesting/__init__.py
--rw-r--r--   0        0        0    10448 2023-04-14 00:08:52.985598 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/backtesting/bt_controller.py
--rw-r--r--   0        0        0     8126 2023-04-14 00:08:52.985598 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/backtesting/bt_model.py
--rw-r--r--   0        0        0     9046 2023-04-14 00:08:52.989598 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/backtesting/bt_view.py
--rw-r--r--   0        0        0        0 2023-04-14 00:08:52.989598 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/behavioural_analysis/__init__.py
--rw-r--r--   0        0        0    29872 2023-04-14 00:08:52.989598 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/behavioural_analysis/ba_controller.py
--rw-r--r--   0        0        0     3541 2023-04-14 00:08:52.989598 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/behavioural_analysis/finnhub_model.py
--rw-r--r--   0        0        0     3761 2023-04-14 00:08:52.989598 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/behavioural_analysis/finnhub_view.py
--rw-r--r--   0        0        0     1931 2023-04-14 00:08:52.989598 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/cboe_model.py
--rw-r--r--   0        0        0      969 2023-04-14 00:08:52.989598 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/cboe_view.py
--rw-r--r--   0        0        0        0 2023-04-14 00:08:52.989598 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/comparison_analysis/__init__.py
--rw-r--r--   0        0        0    37655 2023-04-14 00:08:52.989598 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/comparison_analysis/ca_controller.py
--rw-r--r--   0        0        0     4871 2023-04-14 00:08:52.989598 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/comparison_analysis/finbrain_model.py
--rw-r--r--   0        0        0     5785 2023-04-14 00:08:52.989598 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/comparison_analysis/finbrain_view.py
--rw-r--r--   0        0        0     1328 2023-04-14 00:08:52.989598 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/comparison_analysis/finnhub_model.py
--rw-r--r--   0        0        0     2679 2023-04-14 00:08:52.989598 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/comparison_analysis/finviz_compare_model.py
--rw-r--r--   0        0        0     1539 2023-04-14 00:08:52.989598 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/comparison_analysis/finviz_compare_view.py
--rw-r--r--   0        0        0    12381 2023-04-14 00:08:52.989598 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/comparison_analysis/marketwatch_model.py
--rw-r--r--   0        0        0     5757 2023-04-14 00:08:52.989598 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/comparison_analysis/marketwatch_view.py
--rw-r--r--   0        0        0     1690 2023-04-14 00:08:52.989598 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/comparison_analysis/polygon_model.py
--rw-r--r--   0        0        0     1379 2023-04-14 00:08:52.989598 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/comparison_analysis/sdk_helpers.py
--rw-r--r--   0        0        0     8073 2023-04-14 00:08:52.989598 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/comparison_analysis/yahoo_finance_model.py
--rw-r--r--   0        0        0    10157 2023-04-14 00:08:52.989598 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/comparison_analysis/yahoo_finance_view.py
--rw-r--r--   0        0        0        0 2023-04-14 00:08:52.989598 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/dark_pool_shorts/__init__.py
--rw-r--r--   0        0        0    20377 2023-04-14 00:08:52.989598 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/dark_pool_shorts/dps_controller.py
--rw-r--r--   0        0        0    10009 2023-04-14 00:08:52.989598 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/dark_pool_shorts/finra_model.py
--rw-r--r--   0        0        0     7203 2023-04-14 00:08:52.989598 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/dark_pool_shorts/finra_view.py
--rw-r--r--   0        0        0     1093 2023-04-14 00:08:52.989598 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/dark_pool_shorts/ibkr_model.py
--rw-r--r--   0        0        0     1200 2023-04-14 00:08:52.989598 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/dark_pool_shorts/ibkr_view.py
--rw-r--r--   0        0        0     1387 2023-04-14 00:08:52.989598 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/dark_pool_shorts/quandl_model.py
--rw-r--r--   0        0        0     4648 2023-04-14 00:08:52.989598 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/dark_pool_shorts/quandl_view.py
--rw-r--r--   0        0        0     6836 2023-04-14 00:08:52.989598 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/dark_pool_shorts/sec_model.py
--rw-r--r--   0        0        0     3470 2023-04-14 00:08:52.989598 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/dark_pool_shorts/sec_view.py
--rw-r--r--   0        0        0     1882 2023-04-14 00:08:52.989598 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/dark_pool_shorts/shortinterest_model.py
--rw-r--r--   0        0        0     1385 2023-04-14 00:08:52.989598 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/dark_pool_shorts/shortinterest_view.py
--rw-r--r--   0        0        0     5053 2023-04-14 00:08:52.989598 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/dark_pool_shorts/stockgrid_model.py
--rw-r--r--   0        0        0     9997 2023-04-14 00:08:52.989598 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/dark_pool_shorts/stockgrid_view.py
--rw-r--r--   0        0        0     1166 2023-04-14 00:08:52.989598 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/dark_pool_shorts/stocksera_model.py
--rw-r--r--   0        0        0     3613 2023-04-14 00:08:52.989598 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/dark_pool_shorts/stocksera_view.py
--rw-r--r--   0        0        0      668 2023-04-14 00:08:52.989598 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/dark_pool_shorts/yahoofinance_model.py
--rw-r--r--   0        0        0     1271 2023-04-14 00:08:52.989598 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/dark_pool_shorts/yahoofinance_view.py
--rw-r--r--   0        0        0     5740 2023-04-14 00:08:52.989598 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/databento_model.py
--rw-r--r--   0        0        0        0 2023-04-14 00:08:52.989598 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/discovery/__init__.py
--rw-r--r--   0        0        0     4169 2023-04-14 00:08:52.989598 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/discovery/ark_model.py
--rw-r--r--   0        0        0     2589 2023-04-14 00:08:52.989598 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/discovery/ark_view.py
--rw-r--r--   0        0        0    30135 2023-04-14 00:08:52.989598 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/discovery/disc_controller.py
--rw-r--r--   0        0        0      483 2023-04-14 00:08:52.989598 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/discovery/disc_helpers.py
--rw-r--r--   0        0        0     2696 2023-04-14 00:08:52.989598 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/discovery/fidelity_model.py
--rw-r--r--   0        0        0     2680 2023-04-14 00:08:52.989598 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/discovery/fidelity_view.py
--rw-r--r--   0        0        0     4164 2023-04-14 00:08:52.989598 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/discovery/finnhub_model.py
--rw-r--r--   0        0        0     2510 2023-04-14 00:08:52.989598 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/discovery/finnhub_view.py
--rw-r--r--   0        0        0     1731 2023-04-14 00:08:52.989598 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/discovery/finviz_model.py
--rw-r--r--   0        0        0     3084 2023-04-14 00:08:52.989598 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/discovery/finviz_view.py
--rw-r--r--   0        0        0     3051 2023-04-14 00:08:52.989598 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/discovery/nasdaq_model.py
--rw-r--r--   0        0        0     3406 2023-04-14 00:08:52.989598 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/discovery/nasdaq_view.py
--rw-r--r--   0        0        0     7080 2023-04-14 00:08:52.989598 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/discovery/seeking_alpha_model.py
--rw-r--r--   0        0        0     4803 2023-04-14 00:08:52.989598 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/discovery/seeking_alpha_view.py
--rw-r--r--   0        0        0     1120 2023-04-14 00:08:52.989598 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/discovery/shortinterest_model.py
--rw-r--r--   0        0        0     2566 2023-04-14 00:08:52.989598 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/discovery/shortinterest_view.py
--rw-r--r--   0        0        0     4113 2023-04-14 00:08:52.989598 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/discovery/yahoofinance_model.py
--rw-r--r--   0        0        0     5871 2023-04-14 00:08:52.989598 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/discovery/yahoofinance_view.py
--rw-r--r--   0        0        0        0 2023-04-14 00:08:52.989598 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/fundamental_analysis/__init__.py
--rw-r--r--   0        0        0    24082 2023-04-14 00:08:52.989598 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/fundamental_analysis/av_model.py
--rw-r--r--   0        0        0    14910 2023-04-14 00:08:52.989598 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/fundamental_analysis/av_view.py
--rw-r--r--   0        0        0    10325 2023-04-14 00:08:52.989598 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/fundamental_analysis/business_insider_model.py
--rw-r--r--   0        0        0     7696 2023-04-14 00:08:52.989598 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/fundamental_analysis/business_insider_view.py
--rw-r--r--   0        0        0     1833 2023-04-14 00:08:52.989598 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/fundamental_analysis/csimarket_model.py
--rw-r--r--   0        0        0     2347 2023-04-14 00:08:52.989598 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/fundamental_analysis/csimarket_view.py
--rw-r--r--   0        0        0    14888 2023-04-14 00:08:52.993599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/fundamental_analysis/dcf_model.py
--rw-r--r--   0        0        0     4279 2023-04-14 00:08:52.993599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/fundamental_analysis/dcf_static.py
--rw-r--r--   0        0        0    44464 2023-04-14 00:08:52.993599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/fundamental_analysis/dcf_view.py
--rw-r--r--   0        0        0     1925 2023-04-14 00:08:52.993599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/fundamental_analysis/eclect_us_model.py
--rw-r--r--   0        0        0     1205 2023-04-14 00:08:52.993599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/fundamental_analysis/eclect_us_view.py
--rw-r--r--   0        0        0     2396 2023-04-14 00:08:52.993599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/fundamental_analysis/eodhd_model.py
--rw-r--r--   0        0        0     4904 2023-04-14 00:08:52.993599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/fundamental_analysis/eodhd_view.py
--rw-r--r--   0        0        0    81664 2023-04-14 00:08:52.993599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/fundamental_analysis/fa_controller.py
--rw-r--r--   0        0        0      266 2023-04-14 00:08:52.993599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/fundamental_analysis/fa_helper.py
--rw-r--r--   0        0        0     1389 2023-04-14 00:08:52.993599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/fundamental_analysis/finnhub_model.py
--rw-r--r--   0        0        0     3518 2023-04-14 00:08:52.993599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/fundamental_analysis/finnhub_view.py
--rw-r--r--   0        0        0     3419 2023-04-14 00:08:52.993599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/fundamental_analysis/finviz_model.py
--rw-r--r--   0        0        0     2484 2023-04-14 00:08:52.993599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/fundamental_analysis/finviz_view.py
--rw-r--r--   0        0        0    20480 2023-04-14 00:08:52.993599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/fundamental_analysis/fmp_model.py
--rw-r--r--   0        0        0    23886 2023-04-14 00:08:52.993599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/fundamental_analysis/fmp_view.py
--rw-r--r--   0        0        0     6417 2023-04-14 00:08:52.993599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/fundamental_analysis/key_metrics_explained.txt
--rw-r--r--   0        0        0    14313 2023-04-14 00:08:52.993599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/fundamental_analysis/marketwatch_model.py
--rw-r--r--   0        0        0     2870 2023-04-14 00:08:52.993599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/fundamental_analysis/marketwatch_view.py
--rw-r--r--   0        0        0     5391 2023-04-14 00:08:52.993599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/fundamental_analysis/polygon_model.py
--rw-r--r--   0        0        0     4361 2023-04-14 00:08:52.993599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/fundamental_analysis/polygon_view.py
--rw-r--r--   0        0        0     7593 2023-04-14 00:08:52.993599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/fundamental_analysis/sdk_helpers.py
--rw-r--r--   0        0        0    11162 2023-04-14 00:08:52.993599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/fundamental_analysis/seeking_alpha_model.py
--rw-r--r--   0        0        0     2059 2023-04-14 00:08:52.993599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/fundamental_analysis/seeking_alpha_view.py
--rw-r--r--   0        0        0    11829 2023-04-14 00:08:52.993599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/fundamental_analysis/yahoo_finance_model.py
--rw-r--r--   0        0        0    14679 2023-04-14 00:08:52.993599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/fundamental_analysis/yahoo_finance_view.py
--rw-r--r--   0        0        0        0 2023-04-14 00:08:52.993599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/government/__init__.py
--rw-r--r--   0        0        0    18461 2023-04-14 00:08:52.993599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/government/gov_controller.py
--rw-r--r--   0        0        0    15719 2023-04-14 00:08:52.993599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/government/quiverquant_model.py
--rw-r--r--   0        0        0    21407 2023-04-14 00:08:52.993599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/government/quiverquant_view.py
--rw-r--r--   0        0        0        0 2023-04-14 00:08:52.993599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/insider/__init__.py
--rw-r--r--   0        0        0     2062 2023-04-14 00:08:52.993599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/insider/businessinsider_model.py
--rw-r--r--   0        0        0     5102 2023-04-14 00:08:52.993599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/insider/businessinsider_view.py
--rw-r--r--   0        0        0     1125 2023-04-14 00:08:52.993599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/insider/finviz_model.py
--rw-r--r--   0        0        0     1171 2023-04-14 00:08:52.993599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/insider/finviz_view.py
--rw-r--r--   0        0        0    32744 2023-04-14 00:08:52.993599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/insider/insider_controller.py
--rw-r--r--   0        0        0    87496 2023-04-14 00:08:52.993599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/insider/openinsider_model.py
--rw-r--r--   0        0        0     7695 2023-04-14 00:08:52.993599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/insider/openinsider_view.py
--rw-r--r--   0        0        0     4909 2023-04-14 00:08:52.993599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/insider/sdk_helper.py
--rw-r--r--   0        0        0    76085 2023-04-14 00:08:52.993599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/mappings/Mic_Codes.csv
--rw-r--r--   0        0        0        0 2023-04-14 00:08:52.993599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/options/__init__.py
--rw-r--r--   0        0        0     1757 2023-04-14 00:08:52.993599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/options/alphaquery_model.py
--rw-r--r--   0        0        0     1713 2023-04-14 00:08:52.993599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/options/alphaquery_view.py
--rw-r--r--   0        0        0     1161 2023-04-14 00:08:52.993599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/options/barchart_model.py
--rw-r--r--   0        0        0     1137 2023-04-14 00:08:52.993599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/options/barchart_view.py
--rw-r--r--   0        0        0     1526 2023-04-14 00:08:52.993599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/options/calculator_model.py
--rw-r--r--   0        0        0     2416 2023-04-14 00:08:52.993599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/options/calculator_view.py
--rw-r--r--   0        0        0     2777 2023-04-14 00:08:52.993599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/options/chartexchange_model.py
--rw-r--r--   0        0        0     3211 2023-04-14 00:08:52.993599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/options/chartexchange_view.py
--rw-r--r--   0        0        0     2433 2023-04-14 00:08:52.997599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/options/fdscanner_model.py
--rw-r--r--   0        0        0     1672 2023-04-14 00:08:52.997599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/options/fdscanner_view.py
--rw-r--r--   0        0        0    21092 2023-04-14 00:08:52.997599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/options/hedge/hedge_controller.py
--rw-r--r--   0        0        0     9884 2023-04-14 00:08:52.997599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/options/hedge/hedge_model.py
--rw-r--r--   0        0        0     3968 2023-04-14 00:08:52.997599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/options/hedge/hedge_view.py
--rw-r--r--   0        0        0    10030 2023-04-14 00:08:52.997599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/options/intrinio_model.py
--rw-r--r--   0        0        0     6101 2023-04-14 00:08:52.997599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/options/intrinio_view.py
--rw-r--r--   0        0        0     7097 2023-04-14 00:08:52.997599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/options/nasdaq_model.py
--rw-r--r--   0        0        0    22486 2023-04-14 00:08:52.997599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/options/op_helpers.py
--rw-r--r--   0        0        0    51845 2023-04-14 00:08:52.997599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/options/options_controller.py
--rw-r--r--   0        0        0    10556 2023-04-14 00:08:52.997599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/options/options_sdk_helper.py
--rw-r--r--   0        0        0    14169 2023-04-14 00:08:52.997599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/options/options_view.py
--rw-r--r--   0        0        0        0 2023-04-14 00:08:52.997599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/options/screen/__init__.py
--rw-r--r--   0        0        0     5686 2023-04-14 00:08:52.997599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/options/screen/screener_controller.py
--rw-r--r--   0        0        0     9556 2023-04-14 00:08:52.997599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/options/screen/syncretism_model.py
--rw-r--r--   0        0        0     5566 2023-04-14 00:08:52.997599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/options/screen/syncretism_view.py
--rw-r--r--   0        0        0     8295 2023-04-14 00:08:52.997599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/options/tradier_model.py
--rw-r--r--   0        0        0     2561 2023-04-14 00:08:52.997599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/options/tradier_view.py
--rw-r--r--   0        0        0     7674 2023-04-14 00:08:52.997599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/options/yfinance_model.py
--rw-r--r--   0        0        0    11615 2023-04-14 00:08:52.997599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/options/yfinance_view.py
--rw-r--r--   0        0        0        0 2023-04-14 00:08:52.997599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/quantitative_analysis/__init__.py
--rw-r--r--   0        0        0     2260 2023-04-14 00:08:52.997599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/quantitative_analysis/beta_model.py
--rw-r--r--   0        0        0     2798 2023-04-14 00:08:52.997599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/quantitative_analysis/beta_view.py
--rw-r--r--   0        0        0     3187 2023-04-14 00:08:52.997599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/quantitative_analysis/factors_model.py
--rw-r--r--   0        0        0      687 2023-04-14 00:08:52.997599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/quantitative_analysis/factors_view.py
--rw-r--r--   0        0        0    38741 2023-04-14 00:08:52.997599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/quantitative_analysis/qa_controller.py
--rw-r--r--   0        0        0      447 2023-04-14 00:08:52.997599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/quantitative_analysis/qa_model.py
--rw-r--r--   0        0        0        0 2023-04-14 00:08:52.997599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/research/__init__.py
--rw-r--r--   0        0        0     6218 2023-04-14 00:08:52.997599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/research/res_controller.py
--rw-r--r--   0        0        0        0 2023-04-14 00:08:52.997599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/screener/__init__.py
--rw-r--r--   0        0        0    46491 2023-04-14 00:08:52.997599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/screener/finviz_model.py
--rw-r--r--   0        0        0     6981 2023-04-14 00:08:52.997599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/screener/finviz_view.py
--rw-r--r--   0        0        0    21493 2023-04-14 00:08:52.997599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/screener/screener_controller.py
--rw-r--r--   0        0        0      944 2023-04-14 00:08:52.997599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/screener/screener_helper.py
--rw-r--r--   0        0        0     2562 2023-04-14 00:08:52.997599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/screener/screener_view.py
--rw-r--r--   0        0        0    27077 2023-04-14 00:08:52.997599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/stock_statics.py
--rw-r--r--   0        0        0    27380 2023-04-14 00:08:52.997599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/stocks_controller.py
--rw-r--r--   0        0        0    33043 2023-04-14 00:08:52.997599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/stocks_helper.py
--rw-r--r--   0        0        0    10576 2023-04-14 00:08:52.997599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/stocks_model.py
--rw-r--r--   0        0        0     1241 2023-04-14 00:08:52.997599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/stocks_view.py
--rw-r--r--   0        0        0        0 2023-04-14 00:08:52.997599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/technical_analysis/__init__.py
--rw-r--r--   0        0        0     1004 2023-04-14 00:08:52.997599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/technical_analysis/finbrain_model.py
--rw-r--r--   0        0        0      644 2023-04-14 00:08:52.997599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/technical_analysis/finbrain_view.py
--rw-r--r--   0        0        0      761 2023-04-14 00:08:52.997599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/technical_analysis/finviz_model.py
--rw-r--r--   0        0        0     1229 2023-04-14 00:08:52.997599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/technical_analysis/finviz_view.py
--rw-r--r--   0        0        0     1532 2023-04-14 00:08:52.997599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/technical_analysis/rsp_model.py
--rw-r--r--   0        0        0     2386 2023-04-14 00:08:52.997599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/technical_analysis/rsp_view.py
--rw-r--r--   0        0        0    63416 2023-04-14 00:08:52.997599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/technical_analysis/ta_controller.py
--rw-r--r--   0        0        0     3260 2023-04-14 00:08:52.997599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/technical_analysis/tradingview_model.py
--rw-r--r--   0        0        0     1985 2023-04-14 00:08:52.997599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/technical_analysis/tradingview_view.py
--rw-r--r--   0        0        0      334 2023-04-14 00:08:52.997599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/tradinghours/README.md
--rw-r--r--   0        0        0        0 2023-04-14 00:08:52.997599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/tradinghours/__init__.py
--rw-r--r--   0        0        0     5328 2023-04-14 00:08:52.997599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/tradinghours/bursa_model.py
--rw-r--r--   0        0        0     2202 2023-04-14 00:08:52.997599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/tradinghours/bursa_view.py
--rw-r--r--   0        0        0        0 2023-04-14 00:08:52.997599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/tradinghours/data/__init__.py
--rw-r--r--   0        0        0    28098 2023-04-14 00:08:52.997599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/tradinghours/data/bursa_open_hours.json
--rw-r--r--   0        0        0     1466 2023-04-14 00:08:52.997599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/tradinghours/pandas_market_cal_model.py
--rw-r--r--   0        0        0     1378 2023-04-14 00:08:52.997599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/tradinghours/pandas_market_cal_view.py
--rw-r--r--   0        0        0    10137 2023-04-14 00:08:53.001599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/tradinghours/tradinghours_controller.py
--rw-r--r--   0        0        0      614 2023-04-14 00:08:53.001599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/tradinghours/tradinghours_helper.py
--rw-r--r--   0        0        0    42263 2023-04-14 00:08:53.001599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/terminal_controller.py
--rw-r--r--   0        0        0    14336 2023-04-14 00:08:53.001599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/terminal_helper.py
--rw-r--r--   0        0        0     3848 2023-04-14 00:08:53.001599 openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/thought_of_the_day.py
--rw-r--r--   0        0        0     5771 2023-04-14 00:08:55.053739 openbb_nightly-3.0.0rc2.dev20230414/pyproject.toml
--rw-r--r--   0        0        0     1137 2023-04-14 00:08:53.005599 openbb_nightly-3.0.0rc2.dev20230414/terminal.py
--rw-r--r--   0        0        0     2293 2023-04-14 00:08:55.061740 openbb_nightly-3.0.0rc2.dev20230414/website/pypi.md
--rw-r--r--   0        0        0     7776 1970-01-01 00:00:00.000000 openbb_nightly-3.0.0rc2.dev20230414/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-04-15 00:10:05.456768 openbb_nightly-3.0.0rc2.dev20230415/LICENSE
+-rw-r--r--   0        0        0    18588 2023-04-15 00:10:05.612771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/SDK_README.md
+-rw-r--r--   0        0        0      243 2023-04-15 00:10:05.612771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-15 00:10:05.612771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/account/__init__.py
+-rw-r--r--   0        0        0    21588 2023-04-15 00:10:05.612771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/account/account_controller.py
+-rw-r--r--   0        0        0     1769 2023-04-15 00:10:05.612771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/account/account_view.py
+-rw-r--r--   0        0        0        0 2023-04-15 00:10:05.612771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/alternative/__init__.py
+-rw-r--r--   0        0        0     3131 2023-04-15 00:10:05.612771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/alternative/alt_controller.py
+-rw-r--r--   0        0        0        0 2023-04-15 00:10:05.612771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/alternative/covid/__init__.py
+-rw-r--r--   0        0        0     1881 2023-04-15 00:10:05.612771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/alternative/covid/countries.txt
+-rw-r--r--   0        0        0     9347 2023-04-15 00:10:05.612771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/alternative/covid/covid_controller.py
+-rw-r--r--   0        0        0     5387 2023-04-15 00:10:05.612771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/alternative/covid/covid_model.py
+-rw-r--r--   0        0        0     8586 2023-04-15 00:10:05.612771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/alternative/covid/covid_view.py
+-rw-r--r--   0        0        0     1070 2023-04-15 00:10:05.612771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/alternative/hackernews_model.py
+-rw-r--r--   0        0        0     1087 2023-04-15 00:10:05.612771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/alternative/hackernews_view.py
+-rw-r--r--   0        0        0     6752 2023-04-15 00:10:05.612771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/alternative/oss/github_model.py
+-rw-r--r--   0        0        0     3968 2023-04-15 00:10:05.612771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/alternative/oss/github_view.py
+-rw-r--r--   0        0        0     8656 2023-04-15 00:10:05.612771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/alternative/oss/oss_controller.py
+-rw-r--r--   0        0        0     4437 2023-04-15 00:10:05.612771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/alternative/oss/runa_model.py
+-rw-r--r--   0        0        0     4018 2023-04-15 00:10:05.612771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/alternative/oss/runa_view.py
+-rw-r--r--   0        0        0        0 2023-04-15 00:10:05.616771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/alternative/realestate/__init__.py
+-rw-r--r--   0        0        0     9030 2023-04-15 00:10:05.616771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/alternative/realestate/landRegistry_model.py
+-rw-r--r--   0        0        0     3309 2023-04-15 00:10:05.616771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/alternative/realestate/landRegistry_view.py
+-rw-r--r--   0        0        0     8108 2023-04-15 00:10:05.616771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/alternative/realestate/realestate_controller.py
+-rw-r--r--   0        0        0     2718 2023-04-15 00:10:05.616771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/base_helpers.py
+-rw-r--r--   0        0        0       93 2023-04-15 00:10:05.616771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/common/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-15 00:10:05.616771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/common/behavioural_analysis/__init__.py
+-rw-r--r--   0        0        0     1198 2023-04-15 00:10:05.616771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/common/behavioural_analysis/finbrain_model.py
+-rw-r--r--   0        0        0     4394 2023-04-15 00:10:05.616771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/common/behavioural_analysis/finbrain_view.py
+-rw-r--r--   0        0        0     1335 2023-04-15 00:10:05.616771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/common/behavioural_analysis/finnhub_model.py
+-rw-r--r--   0        0        0     1861 2023-04-15 00:10:05.616771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/common/behavioural_analysis/finnhub_view.py
+-rw-r--r--   0        0        0     4131 2023-04-15 00:10:05.616771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/common/behavioural_analysis/google_model.py
+-rw-r--r--   0        0        0     7118 2023-04-15 00:10:05.616771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/common/behavioural_analysis/google_view.py
+-rw-r--r--   0        0        0     5524 2023-04-15 00:10:05.616771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/common/behavioural_analysis/reddit_helpers.py
+-rw-r--r--   0        0        0    18297 2023-04-15 00:10:05.616771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/common/behavioural_analysis/reddit_model.py
+-rw-r--r--   0        0        0    10206 2023-04-15 00:10:05.616771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/common/behavioural_analysis/reddit_view.py
+-rw-r--r--   0        0        0     3239 2023-04-15 00:10:05.616771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/common/behavioural_analysis/stocktwits_model.py
+-rw-r--r--   0        0        0     2898 2023-04-15 00:10:05.616771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/common/behavioural_analysis/stocktwits_view.py
+-rw-r--r--   0        0        0     6160 2023-04-15 00:10:05.616771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/common/behavioural_analysis/twitter_model.py
+-rw-r--r--   0        0        0     5870 2023-04-15 00:10:05.616771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/common/behavioural_analysis/twitter_view.py
+-rw-r--r--   0        0        0     4142 2023-04-15 00:10:05.616771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/common/common_model.py
+-rw-r--r--   0        0        0     3634 2023-04-15 00:10:05.616771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/common/feedparser_model.py
+-rw-r--r--   0        0        0     1242 2023-04-15 00:10:05.616771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/common/feedparser_view.py
+-rw-r--r--   0        0        0     2639 2023-04-15 00:10:05.616771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/common/newsapi_model.py
+-rw-r--r--   0        0        0     1465 2023-04-15 00:10:05.616771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/common/newsapi_view.py
+-rw-r--r--   0        0        0        0 2023-04-15 00:10:05.616771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/common/quantitative_analysis/__init__.py
+-rw-r--r--   0        0        0    19923 2023-04-15 00:10:05.616771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/common/quantitative_analysis/qa_model.py
+-rw-r--r--   0        0        0    32308 2023-04-15 00:10:05.616771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/common/quantitative_analysis/qa_view.py
+-rw-r--r--   0        0        0     3226 2023-04-15 00:10:05.616771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/common/quantitative_analysis/rolling_model.py
+-rw-r--r--   0        0        0    10790 2023-04-15 00:10:05.616771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/common/quantitative_analysis/rolling_view.py
+-rw-r--r--   0        0        0        0 2023-04-15 00:10:05.616771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/common/technical_analysis/__init__.py
+-rw-r--r--   0        0        0     2977 2023-04-15 00:10:05.616771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/common/technical_analysis/custom_indicators_model.py
+-rw-r--r--   0        0        0     4272 2023-04-15 00:10:05.616771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/common/technical_analysis/custom_indicators_view.py
+-rw-r--r--   0        0        0     6427 2023-04-15 00:10:05.616771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/common/technical_analysis/momentum_model.py
+-rw-r--r--   0        0        0    10556 2023-04-15 00:10:05.616771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/common/technical_analysis/momentum_view.py
+-rw-r--r--   0        0        0     4179 2023-04-15 00:10:05.616771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/common/technical_analysis/overlap_model.py
+-rw-r--r--   0        0        0     4361 2023-04-15 00:10:05.616771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/common/technical_analysis/overlap_view.py
+-rw-r--r--   0        0        0     1453 2023-04-15 00:10:05.616771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/common/technical_analysis/ta_helpers.py
+-rw-r--r--   0        0        0     1819 2023-04-15 00:10:05.616771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/common/technical_analysis/trend_indicators_model.py
+-rw-r--r--   0        0        0     2621 2023-04-15 00:10:05.616771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/common/technical_analysis/trend_indicators_view.py
+-rw-r--r--   0        0        0    19962 2023-04-15 00:10:05.616771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/common/technical_analysis/volatility_model.py
+-rw-r--r--   0        0        0    10008 2023-04-15 00:10:05.616771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/common/technical_analysis/volatility_view.py
+-rw-r--r--   0        0        0     2614 2023-04-15 00:10:05.616771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/common/technical_analysis/volume_model.py
+-rw-r--r--   0        0        0     3806 2023-04-15 00:10:05.616771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/common/technical_analysis/volume_view.py
+-rw-r--r--   0        0        0     5813 2023-04-15 00:10:05.616771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/common/ultima_newsmonitor_model.py
+-rw-r--r--   0        0        0     3886 2023-04-15 00:10:05.616771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/common/ultima_newsmonitor_view.py
+-rw-r--r--   0        0        0     2634 2023-04-15 00:10:05.616771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/config_terminal.py
+-rw-r--r--   0        0        0        0 2023-04-15 00:10:05.616771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/__init__.py
+-rw-r--r--   0        0        0     9829 2023-04-15 00:10:05.616771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/completer/choices.py
+-rw-r--r--   0        0        0        0 2023-04-15 00:10:05.616771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/config/__init__.py
+-rw-r--r--   0        0        0     1180 2023-04-15 00:10:05.616771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/config/paths.py
+-rw-r--r--   0        0        0     2650 2023-04-15 00:10:05.616771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/config/paths_helper.py
+-rw-r--r--   0        0        0     9704 2023-04-15 00:10:05.616771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/integration_tests/README.md
+-rw-r--r--   0        0        0    23371 2023-04-15 00:10:05.616771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/integration_tests/integration_controller.py
+-rw-r--r--   0        0        0        0 2023-04-15 00:10:05.616771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/log/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-15 00:10:05.616771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/log/collection/__init__.py
+-rw-r--r--   0        0        0     3848 2023-04-15 00:10:05.616771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/log/collection/log_sender.py
+-rw-r--r--   0        0        0     3744 2023-04-15 00:10:05.616771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/log/collection/logging_clock.py
+-rw-r--r--   0        0        0     3495 2023-04-15 00:10:05.616771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/log/collection/s3_sender.py
+-rw-r--r--   0        0        0      166 2023-04-15 00:10:05.616771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/log/constants.py
+-rw-r--r--   0        0        0        0 2023-04-15 00:10:05.616771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/log/generation/__init__.py
+-rw-r--r--   0        0        0      524 2023-04-15 00:10:05.616771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/log/generation/common.py
+-rw-r--r--   0        0        0      525 2023-04-15 00:10:05.616771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/log/generation/custom_logger.py
+-rw-r--r--   0        0        0      979 2023-04-15 00:10:05.616771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/log/generation/directories.py
+-rw-r--r--   0        0        0      841 2023-04-15 00:10:05.616771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/log/generation/expired_files.py
+-rw-r--r--   0        0        0     4896 2023-04-15 00:10:05.616771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/log/generation/formatter_with_exceptions.py
+-rw-r--r--   0        0        0     6058 2023-04-15 00:10:05.616771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/log/generation/path_tracking_file_handler.py
+-rw-r--r--   0        0        0     4166 2023-04-15 00:10:05.616771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/log/generation/settings.py
+-rw-r--r--   0        0        0     1621 2023-04-15 00:10:05.616771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/log/generation/settings_logger.py
+-rw-r--r--   0        0        0      396 2023-04-15 00:10:05.616771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/log/generation/user_logger.py
+-rw-r--r--   0        0        0      627 2023-04-15 00:10:05.620771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/models/__init__.py
+-rw-r--r--   0        0        0     1221 2023-04-15 00:10:05.620771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/models/base_model.py
+-rw-r--r--   0        0        0      818 2023-04-15 00:10:05.620771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/models/credentials_model.py
+-rw-r--r--   0        0        0     4211 2023-04-15 00:10:05.620771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/models/preferences_model.py
+-rw-r--r--   0        0        0     1817 2023-04-15 00:10:05.620771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/models/profile_model.py
+-rw-r--r--   0        0        0     1230 2023-04-15 00:10:05.620771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/models/sources_model.py
+-rw-r--r--   0        0        0     1780 2023-04-15 00:10:05.620771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/models/system_model.py
+-rw-r--r--   0        0        0      634 2023-04-15 00:10:05.620771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/models/user_model.py
+-rw-r--r--   0        0        0      200 2023-04-15 00:10:05.620771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/plots/__init__.py
+-rw-r--r--   0        0        0   418780 2023-04-15 00:10:05.620771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/plots/assets/Terminal_icon.png
+-rw-r--r--   0        0        0      727 2023-04-15 00:10:05.620771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/plots/assets/icon.png
+-rw-r--r--   0        0        0    14311 2023-04-15 00:10:05.620771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/plots/backend.py
+-rw-r--r--   0        0        0        0 2023-04-15 00:10:05.620771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/plots/config/__init__.py
+-rw-r--r--   0        0        0     7156 2023-04-15 00:10:05.620771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/plots/config/openbb_styles.py
+-rw-r--r--   0        0        0     3073 2023-04-15 00:10:05.620771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/plots/no_import.py
+-rw-r--r--   0        0        0     1261 2023-04-15 00:10:05.620771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/plots/old_table.html
+-rw-r--r--   0        0        0    10542 2023-04-15 00:10:05.620771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/plots/plotly.html
+-rw-r--r--   0        0        0    63030 2023-04-15 00:10:05.620771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/plots/plotly_helper.py
+-rw-r--r--   0        0        0        0 2023-04-15 00:10:05.620771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/plots/plotly_ta/__init__.py
+-rw-r--r--   0        0        0     6724 2023-04-15 00:10:05.620771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/plots/plotly_ta/base.py
+-rw-r--r--   0        0        0    11358 2023-04-15 00:10:05.620771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/plots/plotly_ta/data_classes.py
+-rw-r--r--   0        0        0     8016 2023-04-15 00:10:05.620771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/plots/plotly_ta/plugins/custom_indicators_plugin.py
+-rw-r--r--   0        0        0    15173 2023-04-15 00:10:05.620771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/plots/plotly_ta/plugins/momentum_plugin.py
+-rw-r--r--   0        0        0     3361 2023-04-15 00:10:05.620771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/plots/plotly_ta/plugins/overlap_plugin.py
+-rw-r--r--   0        0        0     5683 2023-04-15 00:10:05.620771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/plots/plotly_ta/plugins/trend_indicators_plugin.py
+-rw-r--r--   0        0        0     6868 2023-04-15 00:10:05.620771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/plots/plotly_ta/plugins/volatility_plugin.py
+-rw-r--r--   0        0        0     3429 2023-04-15 00:10:05.620771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/plots/plotly_ta/plugins/volume_plugin.py
+-rw-r--r--   0        0        0    20689 2023-04-15 00:10:05.620771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/plots/plotly_ta/ta_class.py
+-rw-r--r--   0        0        0   704632 2023-04-15 00:10:05.624771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/plots/table.html
+-rw-r--r--   0        0        0    13289 2023-04-15 00:10:05.624771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/plots/web/bar_menus.js
+-rw-r--r--   0        0        0   289624 2023-04-15 00:10:05.628771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/plots/web/css/fonts/FiraCode-Regular.ttf
+-rw-r--r--   0        0        0   286320 2023-04-15 00:10:05.628771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/plots/web/css/fonts/FiraCode-VF.ttf
+-rw-r--r--   0        0        0    25728 2023-04-15 00:10:05.628771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/plots/web/css/style.css
+-rw-r--r--   0        0        0      151 2023-04-15 00:10:05.628771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/plots/web/css/table.css
+-rw-r--r--   0        0        0    16655 2023-04-15 00:10:05.628771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/plots/web/helpers.js
+-rw-r--r--   0        0        0    17072 2023-04-15 00:10:05.628771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/plots/web/main.js
+-rw-r--r--   0        0        0     3255 2023-04-15 00:10:05.628771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/plots/web/main_table.js
+-rw-r--r--   0        0        0    25359 2023-04-15 00:10:05.628771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/plots/web/popups.js
+-rw-r--r--   0        0        0     7775 2023-04-15 00:10:05.628771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/scripts/sdk_audit.py
+-rw-r--r--   0        0        0        0 2023-04-15 00:10:05.628771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/sdk/__init__.py
+-rw-r--r--   0        0        0      450 2023-04-15 00:10:05.628771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/sdk/controllers/__init__.py
+-rw-r--r--   0        0        0     2660 2023-04-15 00:10:05.628771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/sdk/controllers/alt_sdk_controller.py
+-rw-r--r--   0        0        0    24088 2023-04-15 00:10:05.628771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/sdk/controllers/crypto_sdk_controller.py
+-rw-r--r--   0        0        0     1513 2023-04-15 00:10:05.628771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/sdk/controllers/etf_sdk_controller.py
+-rw-r--r--   0        0        0     2365 2023-04-15 00:10:05.628771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/sdk/controllers/forex_sdk_controller.py
+-rw-r--r--   0        0        0     5128 2023-04-15 00:10:05.628771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/sdk/controllers/portfolio_sdk_controller.py
+-rw-r--r--   0        0        0    18208 2023-04-15 00:10:05.628771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/sdk/controllers/stocks_sdk_controller.py
+-rw-r--r--   0        0        0      761 2023-04-15 00:10:05.628771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/sdk/models/__init__.py
+-rw-r--r--   0        0        0     4308 2023-04-15 00:10:05.628771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/sdk/models/alt_sdk_model.py
+-rw-r--r--   0        0        0    42910 2023-04-15 00:10:05.628771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/sdk/models/crypto_sdk_model.py
+-rw-r--r--   0        0        0     4497 2023-04-15 00:10:05.628771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/sdk/models/econometrics_sdk_model.py
+-rw-r--r--   0        0        0     7830 2023-04-15 00:10:05.628771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/sdk/models/economy_sdk_model.py
+-rw-r--r--   0        0        0     2496 2023-04-15 00:10:05.628771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/sdk/models/etf_sdk_model.py
+-rw-r--r--   0        0        0     3515 2023-04-15 00:10:05.628771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/sdk/models/fixedincome_sdk_model.py
+-rw-r--r--   0        0        0     8550 2023-04-15 00:10:05.632771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/sdk/models/forecast_sdk_model.py
+-rw-r--r--   0        0        0     4386 2023-04-15 00:10:05.632771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/sdk/models/forex_sdk_model.py
+-rw-r--r--   0        0        0     1530 2023-04-15 00:10:05.632771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/sdk/models/funds_sdk_model.py
+-rw-r--r--   0        0        0     1067 2023-04-15 00:10:05.632771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/sdk/models/futures_sdk_model.py
+-rw-r--r--   0        0        0     3638 2023-04-15 00:10:05.632771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/sdk/models/keys_sdk_model.py
+-rw-r--r--   0        0        0    10046 2023-04-15 00:10:05.632771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/sdk/models/portfolio_sdk_model.py
+-rw-r--r--   0        0        0     4603 2023-04-15 00:10:05.632771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/sdk/models/qa_sdk_model.py
+-rw-r--r--   0        0        0    32235 2023-04-15 00:10:05.632771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/sdk/models/stocks_sdk_model.py
+-rw-r--r--   0        0        0     7229 2023-04-15 00:10:05.632771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/sdk/models/ta_sdk_model.py
+-rw-r--r--   0        0        0    11508 2023-04-15 00:10:05.632771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/sdk/sdk_helpers.py
+-rw-r--r--   0        0        0    19709 2023-04-15 00:10:05.632771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/sdk/sdk_init.py
+-rw-r--r--   0        0        0    43772 2023-04-15 00:10:05.632771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/sdk/trail_map.csv
+-rw-r--r--   0        0        0     2801 2023-04-15 00:10:05.632771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/sdk/trail_map_forecasting.csv
+-rw-r--r--   0        0        0     1301 2023-04-15 00:10:05.632771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/sdk/trail_map_optimization.csv
+-rw-r--r--   0        0        0     6912 2023-04-15 00:10:05.632771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/sdk/trailmap.py
+-rw-r--r--   0        0        0        0 2023-04-15 00:10:05.632771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/session/__init__.py
+-rw-r--r--   0        0        0     1017 2023-04-15 00:10:05.632771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/session/banner.txt
+-rw-r--r--   0        0        0      602 2023-04-15 00:10:05.632771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/session/constants.py
+-rw-r--r--   0        0        0     1000 2023-04-15 00:10:05.632771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/session/current_system.py
+-rw-r--r--   0        0        0     4095 2023-04-15 00:10:05.632771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/session/current_user.py
+-rw-r--r--   0        0        0     1400 2023-04-15 00:10:05.632771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/session/env_handler.py
+-rw-r--r--   0        0        0    22307 2023-04-15 00:10:05.632771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/session/hub_model.py
+-rw-r--r--   0        0        0     6006 2023-04-15 00:10:05.632771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/session/local_model.py
+-rw-r--r--   0        0        0     5136 2023-04-15 00:10:05.632771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/session/routines_handler.py
+-rw-r--r--   0        0        0     3097 2023-04-15 00:10:05.632771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/session/sdk_session.py
+-rw-r--r--   0        0        0     3026 2023-04-15 00:10:05.632771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/session/session_controller.py
+-rw-r--r--   0        0        0     5958 2023-04-15 00:10:05.632771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/session/session_model.py
+-rw-r--r--   0        0        0     2834 2023-04-15 00:10:05.632771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/session/sources_handler.py
+-rw-r--r--   0        0        0     1677 2023-04-15 00:10:05.632771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/session/utils.py
+-rw-r--r--   0        0        0     3011 2023-04-15 00:10:05.632771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/sources/utils.py
+-rw-r--r--   0        0        0      199 2023-04-15 00:10:05.632771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/README.md
+-rw-r--r--   0        0        0       84 2023-04-15 00:10:05.632771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/__init__.py
+-rw-r--r--   0        0        0     5303 2023-04-15 00:10:05.632771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/coinbase_helpers.py
+-rw-r--r--   0        0        0     2147 2023-04-15 00:10:05.632771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/coinpaprika_helpers.py
+-rw-r--r--   0        0        0    19295 2023-04-15 00:10:05.632771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/crypto_controller.py
+-rw-r--r--   0        0        0     4481 2023-04-15 00:10:05.632771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/crypto_models.py
+-rw-r--r--   0        0        0     1785 2023-04-15 00:10:05.632771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/crypto_views.py
+-rw-r--r--   0        0        0    30342 2023-04-15 00:10:05.632771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/cryptocurrency_helpers.py
+-rw-r--r--   0        0        0      949 2023-04-15 00:10:05.632771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/data/README.md
+-rw-r--r--   0        0        0     7341 2023-04-15 00:10:05.632771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/data/binance_gecko_map.json
+-rw-r--r--   0        0        0     2436 2023-04-15 00:10:05.632771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/data/coinbase_gecko_map.json
+-rw-r--r--   0        0        0     4813 2023-04-15 00:10:05.632771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/data/coingecko_categories.json
+-rw-r--r--   0        0        0   954385 2023-04-15 00:10:05.636771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/data/coingecko_coins.json
+-rw-r--r--   0        0        0  2245016 2023-04-15 00:10:05.644771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/data/coinpaprika_coins.json
+-rw-r--r--   0        0        0    31307 2023-04-15 00:10:05.644771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/data/defillama_dapps.json
+-rw-r--r--   0        0        0   107203 2023-04-15 00:10:05.644771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/data/erc20_coins.json
+-rw-r--r--   0        0        0     7255 2023-04-15 00:10:05.644771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/data/finbrain_coins.json
+-rw-r--r--   0        0        0   222978 2023-04-15 00:10:05.648771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/data/santiment_slugs.json
+-rw-r--r--   0        0        0   300253 2023-04-15 00:10:05.648771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/data/yahoofinance_coins.json
+-rw-r--r--   0        0        0     4951 2023-04-15 00:10:05.648771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/dataframe_helpers.py
+-rw-r--r--   0        0        0        0 2023-04-15 00:10:05.648771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/defi/__init__.py
+-rw-r--r--   0        0        0     4537 2023-04-15 00:10:05.648771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/defi/coindix_model.py
+-rw-r--r--   0        0        0     2720 2023-04-15 00:10:05.648771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/defi/coindix_view.py
+-rw-r--r--   0        0        0     2483 2023-04-15 00:10:05.648771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/defi/cryptosaurio_model.py
+-rw-r--r--   0        0        0     1994 2023-04-15 00:10:05.648771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/defi/cryptosaurio_view.py
+-rw-r--r--   0        0        0    31284 2023-04-15 00:10:05.648771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/defi/defi_controller.py
+-rw-r--r--   0        0        0     8918 2023-04-15 00:10:05.648771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/defi/graph_model.py
+-rw-r--r--   0        0        0     7165 2023-04-15 00:10:05.648771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/defi/graph_view.py
+-rw-r--r--   0        0        0     5005 2023-04-15 00:10:05.648771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/defi/llama_model.py
+-rw-r--r--   0        0        0     5827 2023-04-15 00:10:05.648771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/defi/llama_view.py
+-rw-r--r--   0        0        0     1808 2023-04-15 00:10:05.648771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/defi/smartstake_model.py
+-rw-r--r--   0        0        0     3110 2023-04-15 00:10:05.648771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/defi/smartstake_view.py
+-rw-r--r--   0        0        0     2882 2023-04-15 00:10:05.648771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/defi/substack_model.py
+-rw-r--r--   0        0        0     1090 2023-04-15 00:10:05.648771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/defi/substack_view.py
+-rw-r--r--   0        0        0     1947 2023-04-15 00:10:05.648771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/defi/terraengineer_model.py
+-rw-r--r--   0        0        0     2699 2023-04-15 00:10:05.648771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/defi/terraengineer_view.py
+-rw-r--r--   0        0        0     9734 2023-04-15 00:10:05.648771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/defi/terramoney_fcd_model.py
+-rw-r--r--   0        0        0     8022 2023-04-15 00:10:05.648771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/defi/terramoney_fcd_view.py
+-rw-r--r--   0        0        0        0 2023-04-15 00:10:05.648771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/discovery/__init__.py
+-rw-r--r--   0        0        0     2317 2023-04-15 00:10:05.648771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/discovery/coinmarketcap_model.py
+-rw-r--r--   0        0        0     1620 2023-04-15 00:10:05.648771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/discovery/coinmarketcap_view.py
+-rw-r--r--   0        0        0     2116 2023-04-15 00:10:05.648771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/discovery/coinpaprika_model.py
+-rw-r--r--   0        0        0     1936 2023-04-15 00:10:05.648771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/discovery/coinpaprika_view.py
+-rw-r--r--   0        0        0     7614 2023-04-15 00:10:05.648771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/discovery/dappradar_model.py
+-rw-r--r--   0        0        0     5045 2023-04-15 00:10:05.648771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/discovery/dappradar_view.py
+-rw-r--r--   0        0        0    21019 2023-04-15 00:10:05.648771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/discovery/discovery_controller.py
+-rw-r--r--   0        0        0    10833 2023-04-15 00:10:05.648771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/discovery/pycoingecko_model.py
+-rw-r--r--   0        0        0     6352 2023-04-15 00:10:05.648771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/discovery/pycoingecko_view.py
+-rw-r--r--   0        0        0     1095 2023-04-15 00:10:05.648771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/discovery/sdk_helpers.py
+-rw-r--r--   0        0        0        0 2023-04-15 00:10:05.648771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/due_diligence/__init__.py
+-rw-r--r--   0        0        0     7483 2023-04-15 00:10:05.648771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/due_diligence/binance_model.py
+-rw-r--r--   0        0        0     3009 2023-04-15 00:10:05.648771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/due_diligence/binance_view.py
+-rw-r--r--   0        0        0     3188 2023-04-15 00:10:05.648771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/due_diligence/ccxt_model.py
+-rw-r--r--   0        0        0     2840 2023-04-15 00:10:05.648771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/due_diligence/ccxt_view.py
+-rw-r--r--   0        0        0     6439 2023-04-15 00:10:05.648771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/due_diligence/coinbase_model.py
+-rw-r--r--   0        0        0     4134 2023-04-15 00:10:05.648771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/due_diligence/coinbase_view.py
+-rw-r--r--   0        0        0     6587 2023-04-15 00:10:05.648771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/due_diligence/coinglass_model.py
+-rw-r--r--   0        0        0     6638 2023-04-15 00:10:05.648771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/due_diligence/coinglass_view.py
+-rw-r--r--   0        0        0    15062 2023-04-15 00:10:05.648771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/due_diligence/coinpaprika_model.py
+-rw-r--r--   0        0        0     9133 2023-04-15 00:10:05.648771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/due_diligence/coinpaprika_view.py
+-rw-r--r--   0        0        0     2332 2023-04-15 00:10:05.648771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/due_diligence/cryptopanic_view.py
+-rw-r--r--   0        0        0    64101 2023-04-15 00:10:05.648771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/due_diligence/dd_controller.py
+-rw-r--r--   0        0        0     1850 2023-04-15 00:10:05.648771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/due_diligence/due_diligence_api.py
+-rw-r--r--   0        0        0     4333 2023-04-15 00:10:05.648771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/due_diligence/finbrain_crypto_view.py
+-rw-r--r--   0        0        0    15044 2023-04-15 00:10:05.648771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/due_diligence/glassnode_model.py
+-rw-r--r--   0        0        0    11237 2023-04-15 00:10:05.648771 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/due_diligence/glassnode_view.py
+-rw-r--r--   0        0        0    24480 2023-04-15 00:10:05.652772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/due_diligence/messari_model.py
+-rw-r--r--   0        0        0    22260 2023-04-15 00:10:05.652772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/due_diligence/messari_view.py
+-rw-r--r--   0        0        0    25887 2023-04-15 00:10:05.652772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/due_diligence/pycoingecko_model.py
+-rw-r--r--   0        0        0     8762 2023-04-15 00:10:05.652772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/due_diligence/pycoingecko_view.py
+-rw-r--r--   0        0        0     3076 2023-04-15 00:10:05.652772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/due_diligence/santiment_model.py
+-rw-r--r--   0        0        0     2070 2023-04-15 00:10:05.652772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/due_diligence/santiment_view.py
+-rw-r--r--   0        0        0     2508 2023-04-15 00:10:05.652772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/due_diligence/sdk_helper.py
+-rw-r--r--   0        0        0     6001 2023-04-15 00:10:05.652772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/due_diligence/tokenterminal_model.py
+-rw-r--r--   0        0        0     3474 2023-04-15 00:10:05.652772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/due_diligence/tokenterminal_view.py
+-rw-r--r--   0        0        0        0 2023-04-15 00:10:05.652772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/nft/__init__.py
+-rw-r--r--   0        0        0     5562 2023-04-15 00:10:05.652772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/nft/nft_controller.py
+-rw-r--r--   0        0        0     1664 2023-04-15 00:10:05.652772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/nft/nftpricefloor_model.py
+-rw-r--r--   0        0        0     4495 2023-04-15 00:10:05.652772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/nft/nftpricefloor_view.py
+-rw-r--r--   0        0        0     2895 2023-04-15 00:10:05.652772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/nft/opensea_model.py
+-rw-r--r--   0        0        0     1289 2023-04-15 00:10:05.652772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/nft/opensea_view.py
+-rw-r--r--   0        0        0        0 2023-04-15 00:10:05.652772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/onchain/__init__.py
+-rw-r--r--   0        0        0    21848 2023-04-15 00:10:05.652772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/onchain/bitquery_model.py
+-rw-r--r--   0        0        0    11444 2023-04-15 00:10:05.652772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/onchain/bitquery_view.py
+-rw-r--r--   0        0        0     3393 2023-04-15 00:10:05.652772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/onchain/blockchain_model.py
+-rw-r--r--   0        0        0     4733 2023-04-15 00:10:05.652772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/onchain/blockchain_view.py
+-rw-r--r--   0        0        0     1840 2023-04-15 00:10:05.652772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/onchain/ethgasstation_model.py
+-rw-r--r--   0        0        0     1266 2023-04-15 00:10:05.652772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/onchain/ethgasstation_view.py
+-rw-r--r--   0        0        0    15974 2023-04-15 00:10:05.652772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/onchain/ethplorer_model.py
+-rw-r--r--   0        0        0    10572 2023-04-15 00:10:05.652772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/onchain/ethplorer_view.py
+-rw-r--r--   0        0        0    53494 2023-04-15 00:10:05.652772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/onchain/onchain_controller.py
+-rw-r--r--   0        0        0     5938 2023-04-15 00:10:05.652772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/onchain/shroom_model.py
+-rw-r--r--   0        0        0     5144 2023-04-15 00:10:05.652772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/onchain/shroom_view.py
+-rw-r--r--   0        0        0     4772 2023-04-15 00:10:05.652772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/onchain/whale_alert_model.py
+-rw-r--r--   0        0        0     2088 2023-04-15 00:10:05.652772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/onchain/whale_alert_view.py
+-rw-r--r--   0        0        0        0 2023-04-15 00:10:05.652772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/overview/__init__.py
+-rw-r--r--   0        0        0     2274 2023-04-15 00:10:05.652772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/overview/blockchaincenter_model.py
+-rw-r--r--   0        0        0     2664 2023-04-15 00:10:05.652772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/overview/blockchaincenter_view.py
+-rw-r--r--   0        0        0     1464 2023-04-15 00:10:05.652772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/overview/coinbase_model.py
+-rw-r--r--   0        0        0     1342 2023-04-15 00:10:05.652772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/overview/coinbase_view.py
+-rw-r--r--   0        0        0    11841 2023-04-15 00:10:05.652772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/overview/coinpaprika_model.py
+-rw-r--r--   0        0        0     9646 2023-04-15 00:10:05.652772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/overview/coinpaprika_view.py
+-rw-r--r--   0        0        0     6776 2023-04-15 00:10:05.652772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/overview/cryptopanic_model.py
+-rw-r--r--   0        0        0     2278 2023-04-15 00:10:05.652772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/overview/cryptopanic_view.py
+-rw-r--r--   0        0        0     1100 2023-04-15 00:10:05.652772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/overview/glassnode_model.py
+-rw-r--r--   0        0        0     4677 2023-04-15 00:10:05.652772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/overview/glassnode_view.py
+-rw-r--r--   0        0        0     5936 2023-04-15 00:10:05.652772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/overview/loanscan_model.py
+-rw-r--r--   0        0        0     3279 2023-04-15 00:10:05.652772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/overview/loanscan_view.py
+-rw-r--r--   0        0        0    55381 2023-04-15 00:10:05.652772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/overview/overview_controller.py
+-rw-r--r--   0        0        0    13641 2023-04-15 00:10:05.652772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/overview/pycoingecko_model.py
+-rw-r--r--   0        0        0    21320 2023-04-15 00:10:05.652772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/overview/pycoingecko_view.py
+-rw-r--r--   0        0        0     5346 2023-04-15 00:10:05.652772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/overview/rekt_model.py
+-rw-r--r--   0        0        0     2253 2023-04-15 00:10:05.652772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/overview/rekt_view.py
+-rw-r--r--   0        0        0     2042 2023-04-15 00:10:05.652772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/overview/sdk_helpers.py
+-rw-r--r--   0        0        0     7167 2023-04-15 00:10:05.652772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/overview/tokenterminal_model.py
+-rw-r--r--   0        0        0     3126 2023-04-15 00:10:05.652772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/overview/tokenterminal_view.py
+-rw-r--r--   0        0        0     6708 2023-04-15 00:10:05.652772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/overview/withdrawalfees_model.py
+-rw-r--r--   0        0        0     3480 2023-04-15 00:10:05.652772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/overview/withdrawalfees_view.py
+-rw-r--r--   0        0        0     7635 2023-04-15 00:10:05.652772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/pycoingecko_helpers.py
+-rw-r--r--   0        0        0     5693 2023-04-15 00:10:05.652772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/pyth_model.py
+-rw-r--r--   0        0        0      973 2023-04-15 00:10:05.652772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/pyth_view.py
+-rw-r--r--   0        0        0        0 2023-04-15 00:10:05.652772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/quantitative_analysis/__init__.py
+-rw-r--r--   0        0        0    26081 2023-04-15 00:10:05.652772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/quantitative_analysis/qa_controller.py
+-rw-r--r--   0        0        0        0 2023-04-15 00:10:05.652772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/technical_analysis/__init__.py
+-rw-r--r--   0        0        0    54572 2023-04-15 00:10:05.652772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/technical_analysis/ta_controller.py
+-rw-r--r--   0        0        0        0 2023-04-15 00:10:05.652772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/tools/__init__.py
+-rw-r--r--   0        0        0     6219 2023-04-15 00:10:05.652772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/tools/tools_controller.py
+-rw-r--r--   0        0        0     1357 2023-04-15 00:10:05.652772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/tools/tools_helpers.py
+-rw-r--r--   0        0        0     3447 2023-04-15 00:10:05.652772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/tools/tools_model.py
+-rw-r--r--   0        0        0     2772 2023-04-15 00:10:05.652772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/tools/tools_view.py
+-rw-r--r--   0        0        0    16935 2023-04-15 00:10:05.652772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/custom_prompt_toolkit.py
+-rw-r--r--   0        0        0    55138 2023-04-15 00:10:05.652772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/custom_reports/lunar_crash/coin_highs.png
+-rw-r--r--   0        0        0  2879534 2023-04-15 00:10:05.672772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/custom_reports/lunar_crash/luna_crash.html
+-rw-r--r--   0        0        0   350260 2023-04-15 00:10:05.672772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/custom_reports/lunar_crash/luna_supply.png
+-rw-r--r--   0        0        0   607642 2023-04-15 00:10:05.676772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/custom_reports/lunar_crash/luna_terra.png
+-rw-r--r--   0        0        0    11988 2023-04-15 00:10:05.676772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/custom_reports/lunar_crash/lunatics.ipynb
+-rw-r--r--   0        0        0   667206 2023-04-15 00:10:05.680772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/custom_reports/lunar_crash/tvl.png
+-rw-r--r--   0        0        0   465754 2023-04-15 00:10:05.684772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/custom_reports/lunar_crash/ust_terra.png
+-rw-r--r--   0        0        0        0 2023-04-15 00:10:05.684772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/dashboards/__init__.py
+-rw-r--r--   0        0        0     9027 2023-04-15 00:10:05.684772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/dashboards/dashboards_controller.py
+-rw-r--r--   0        0        0    13422 2023-04-15 00:10:05.684772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/dashboards/stream/Forecasting.py
+-rw-r--r--   0        0        0        0 2023-04-15 00:10:05.684772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/dashboards/stream/__init__.py
+-rw-r--r--   0        0        0     3985 2023-04-15 00:10:05.684772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/dashboards/stream/common_vars.py
+-rw-r--r--   0        0        0     4261 2023-04-15 00:10:05.684772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/dashboards/stream/pages/Chains.py
+-rw-r--r--   0        0        0     3322 2023-04-15 00:10:05.684772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/dashboards/stream/pages/Correlation.py
+-rw-r--r--   0        0        0     8106 2023-04-15 00:10:05.684772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/dashboards/stream/pages/Futures.py
+-rw-r--r--   0        0        0    17126 2023-04-15 00:10:05.684772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/dashboards/stream/pages/Indicators.py
+-rw-r--r--   0        0        0     6964 2023-04-15 00:10:05.684772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/dashboards/stream/pages/Short_Data.py
+-rw-r--r--   0        0        0    13224 2023-04-15 00:10:05.684772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/dashboards/stream/pages/Stocks.py
+-rw-r--r--   0        0        0     4093 2023-04-15 00:10:05.684772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/dashboards/stream/streamlit_helpers.py
+-rw-r--r--   0        0        0     1092 2023-04-15 00:10:05.684772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/dashboards/streamlit.py
+-rw-r--r--   0        0        0     5481 2023-04-15 00:10:05.684772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/dashboards/voila/chains.ipynb
+-rw-r--r--   0        0        0     6789 2023-04-15 00:10:05.684772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/dashboards/voila/correlation.ipynb
+-rw-r--r--   0        0        0    13930 2023-04-15 00:10:05.684772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/dashboards/voila/forecast.ipynb
+-rw-r--r--   0        0        0    10953 2023-04-15 00:10:05.684772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/dashboards/voila/futures.ipynb
+-rw-r--r--   0        0        0     9421 2023-04-15 00:10:05.684772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/dashboards/voila/shortdata.ipynb
+-rw-r--r--   0        0        0    15315 2023-04-15 00:10:05.684772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/dashboards/voila/stocks.ipynb
+-rw-r--r--   0        0        0     5091 2023-04-15 00:10:05.684772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/decorators.py
+-rw-r--r--   0        0        0        0 2023-04-15 00:10:05.684772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/econometrics/__init__.py
+-rw-r--r--   0        0        0    73682 2023-04-15 00:10:05.684772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/econometrics/econometrics_controller.py
+-rw-r--r--   0        0        0     2973 2023-04-15 00:10:05.684772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/econometrics/econometrics_helpers.py
+-rw-r--r--   0        0        0    13544 2023-04-15 00:10:05.684772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/econometrics/econometrics_model.py
+-rw-r--r--   0        0        0    16620 2023-04-15 00:10:05.684772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/econometrics/econometrics_view.py
+-rw-r--r--   0        0        0    20449 2023-04-15 00:10:05.684772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/econometrics/regression_model.py
+-rw-r--r--   0        0        0     6739 2023-04-15 00:10:05.684772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/econometrics/regression_view.py
+-rw-r--r--   0        0        0       77 2023-04-15 00:10:05.684772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/economy/README.md
+-rw-r--r--   0        0        0        0 2023-04-15 00:10:05.684772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/economy/__init__.py
+-rw-r--r--   0        0        0    10230 2023-04-15 00:10:05.684772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/economy/alphavantage_model.py
+-rw-r--r--   0        0        0    12075 2023-04-15 00:10:05.684772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/economy/alphavantage_view.py
+-rw-r--r--   0        0        0     1614 2023-04-15 00:10:05.684772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/economy/commodity_model.py
+-rw-r--r--   0        0        0     1561 2023-04-15 00:10:05.684772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/economy/commodity_view.py
+-rw-r--r--   0        0        0      909 2023-04-15 00:10:05.684772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/economy/datasets/NASDAQ_CountryCodes.csv
+-rw-r--r--   0        0        0    21218 2023-04-15 00:10:05.684772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/economy/datasets/cpi.csv
+-rw-r--r--   0        0        0    10355 2023-04-15 00:10:05.684772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/economy/datasets/harmonized_cpi.csv
+-rw-r--r--   0        0        0    28404 2023-04-15 00:10:05.684772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/economy/econdb_model.py
+-rw-r--r--   0        0        0     8013 2023-04-15 00:10:05.684772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/economy/econdb_view.py
+-rw-r--r--   0        0        0    90104 2023-04-15 00:10:05.684772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/economy/economy_controller.py
+-rw-r--r--   0        0        0     3436 2023-04-15 00:10:05.684772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/economy/economy_helpers.py
+-rw-r--r--   0        0        0     7966 2023-04-15 00:10:05.684772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/economy/finviz_model.py
+-rw-r--r--   0        0        0     3837 2023-04-15 00:10:05.684772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/economy/finviz_view.py
+-rw-r--r--   0        0        0     9940 2023-04-15 00:10:05.684772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/economy/fred_model.py
+-rw-r--r--   0        0        0     9117 2023-04-15 00:10:05.684772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/economy/fred_view.py
+-rw-r--r--   0        0        0     6972 2023-04-15 00:10:05.684772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/economy/nasdaq_model.py
+-rw-r--r--   0        0        0     3286 2023-04-15 00:10:05.684772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/economy/nasdaq_view.py
+-rw-r--r--   0        0        0    38418 2023-04-15 00:10:05.684772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/economy/oecd_model.py
+-rw-r--r--   0        0        0    28242 2023-04-15 00:10:05.684772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/economy/oecd_view.py
+-rw-r--r--   0        0        0     3768 2023-04-15 00:10:05.684772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/economy/plot_view.py
+-rw-r--r--   0        0        0        0 2023-04-15 00:10:05.684772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/economy/quantitative_analysis/__init__.py
+-rw-r--r--   0        0        0    28433 2023-04-15 00:10:05.684772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/economy/quantitative_analysis/qa_controller.py
+-rw-r--r--   0        0        0     1218 2023-04-15 00:10:05.688772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/economy/sdk_helpers.py
+-rw-r--r--   0        0        0    12870 2023-04-15 00:10:05.688772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/economy/wsj_model.py
+-rw-r--r--   0        0        0     4673 2023-04-15 00:10:05.688772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/economy/wsj_view.py
+-rw-r--r--   0        0        0    30415 2023-04-15 00:10:05.688772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/economy/yfinance_model.py
+-rw-r--r--   0        0        0     5055 2023-04-15 00:10:05.688772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/economy/yfinance_view.py
+-rw-r--r--   0        0        0      106 2023-04-15 00:10:05.688772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/etf/README.md
+-rw-r--r--   0        0        0        0 2023-04-15 00:10:05.688772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/etf/__init__.py
+-rw-r--r--   0        0        0     4023 2023-04-15 00:10:05.688772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/etf/discovery/disc_controller.py
+-rw-r--r--   0        0        0     2804 2023-04-15 00:10:05.688772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/etf/discovery/wsj_model.py
+-rw-r--r--   0        0        0     1320 2023-04-15 00:10:05.688772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/etf/discovery/wsj_view.py
+-rw-r--r--   0        0        0    21045 2023-04-15 00:10:05.688772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/etf/etf_controller.py
+-rw-r--r--   0        0        0      450 2023-04-15 00:10:05.688772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/etf/etf_helper.py
+-rw-r--r--   0        0        0   188615 2023-04-15 00:10:05.688772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/etf/etfs.csv
+-rw-r--r--   0        0        0     2608 2023-04-15 00:10:05.688772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/etf/financedatabase_model.py
+-rw-r--r--   0        0        0     3864 2023-04-15 00:10:05.688772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/etf/financedatabase_view.py
+-rw-r--r--   0        0        0     1417 2023-04-15 00:10:05.688772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/etf/fmp_model.py
+-rw-r--r--   0        0        0     3152 2023-04-15 00:10:05.688772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/etf/fmp_view.py
+-rw-r--r--   0        0        0     4172 2023-04-15 00:10:05.688772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/etf/stockanalysis_model.py
+-rw-r--r--   0        0        0     3941 2023-04-15 00:10:05.688772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/etf/stockanalysis_view.py
+-rw-r--r--   0        0        0    51458 2023-04-15 00:10:05.688772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/etf/technical_analysis/ta_controller.py
+-rw-r--r--   0        0        0     8025 2023-04-15 00:10:05.688772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/featflags_controller.py
+-rw-r--r--   0        0        0        0 2023-04-15 00:10:05.688772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/fixedincome/__init__.py
+-rw-r--r--   0        0        0    58622 2023-04-15 00:10:05.688772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/fixedincome/commercial_paper.csv
+-rw-r--r--   0        0        0   125899 2023-04-15 00:10:05.688772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/fixedincome/corporate_spot_rates.csv
+-rw-r--r--   0        0        0     9217 2023-04-15 00:10:05.688772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/fixedincome/ecb_model.py
+-rw-r--r--   0        0        0     7096 2023-04-15 00:10:05.688772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/fixedincome/ecb_view.py
+-rw-r--r--   0        0        0     5811 2023-04-15 00:10:05.688772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/fixedincome/econdb_model.py
+-rw-r--r--   0        0        0     7831 2023-04-15 00:10:05.688772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/fixedincome/econdb_view.py
+-rw-r--r--   0        0        0    56207 2023-04-15 00:10:05.688772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/fixedincome/fixedincome_controller.py
+-rw-r--r--   0        0        0    37985 2023-04-15 00:10:05.688772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/fixedincome/fred_model.py
+-rw-r--r--   0        0        0    51842 2023-04-15 00:10:05.688772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/fixedincome/fred_view.py
+-rw-r--r--   0        0        0   227110 2023-04-15 00:10:05.688772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/fixedincome/ice_bofa_indices.csv
+-rw-r--r--   0        0        0    10963 2023-04-15 00:10:05.688772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/fixedincome/oecd_model.py
+-rw-r--r--   0        0        0     3997 2023-04-15 00:10:05.688772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/fixedincome/oecd_view.py
+-rw-r--r--   0        0        0     2174 2023-04-15 00:10:05.692772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/fixedincome/yfinance_model.py
+-rw-r--r--   0        0        0     1702 2023-04-15 00:10:05.692772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/fixedincome/yfinance_view.py
+-rw-r--r--   0        0        0        0 2023-04-15 00:10:05.692772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/__init__.py
+-rw-r--r--   0        0        0     1547 2023-04-15 00:10:05.692772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/anom_model.py
+-rw-r--r--   0        0        0     2962 2023-04-15 00:10:05.692772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/anom_view.py
+-rw-r--r--   0        0        0     4629 2023-04-15 00:10:05.692772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/autoarima_model.py
+-rw-r--r--   0        0        0     3933 2023-04-15 00:10:05.692772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/autoarima_view.py
+-rw-r--r--   0        0        0     4658 2023-04-15 00:10:05.692772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/autoces_model.py
+-rw-r--r--   0        0        0     3970 2023-04-15 00:10:05.692772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/autoces_view.py
+-rw-r--r--   0        0        0     4694 2023-04-15 00:10:05.692772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/autoets_model.py
+-rw-r--r--   0        0        0     3972 2023-04-15 00:10:05.692772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/autoets_view.py
+-rw-r--r--   0        0        0     7272 2023-04-15 00:10:05.692772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/autoselect_model.py
+-rw-r--r--   0        0        0     3938 2023-04-15 00:10:05.692772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/autoselect_view.py
+-rw-r--r--   0        0        0     5874 2023-04-15 00:10:05.692772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/brnn_model.py
+-rw-r--r--   0        0        0     6577 2023-04-15 00:10:05.692772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/brnn_view.py
+-rw-r--r--   0        0        0     5562 2023-04-15 00:10:05.692772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/expo_model.py
+-rw-r--r--   0        0        0     5038 2023-04-15 00:10:05.692772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/expo_view.py
+-rw-r--r--   0        0        0     2053 2023-04-15 00:10:05.692772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/forecast.ipynb
+-rw-r--r--   0        0        0   121759 2023-04-15 00:10:05.692772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/forecast_controller.py
+-rw-r--r--   0        0        0    15471 2023-04-15 00:10:05.692772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/forecast_model.py
+-rw-r--r--   0        0        0     9034 2023-04-15 00:10:05.692772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/forecast_view.py
+-rw-r--r--   0        0        0    47334 2023-04-15 00:10:05.692772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/helpers.py
+-rw-r--r--   0        0        0     3405 2023-04-15 00:10:05.692772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/linregr_model.py
+-rw-r--r--   0        0        0     4760 2023-04-15 00:10:05.692772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/linregr_view.py
+-rw-r--r--   0        0        0     5013 2023-04-15 00:10:05.692772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/mstl_model.py
+-rw-r--r--   0        0        0     3861 2023-04-15 00:10:05.692772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/mstl_view.py
+-rw-r--r--   0        0        0     5896 2023-04-15 00:10:05.692772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/nbeats_model.py
+-rw-r--r--   0        0        0     6396 2023-04-15 00:10:05.692772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/nbeats_view.py
+-rw-r--r--   0        0        0     7561 2023-04-15 00:10:05.692772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/nhits_model.py
+-rw-r--r--   0        0        0     7952 2023-04-15 00:10:05.692772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/nhits_view.py
+-rw-r--r--   0        0        0     3007 2023-04-15 00:10:05.692772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/regr_model.py
+-rw-r--r--   0        0        0     4521 2023-04-15 00:10:05.692772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/regr_view.py
+-rw-r--r--   0        0        0     5030 2023-04-15 00:10:05.692772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/rnn_model.py
+-rw-r--r--   0        0        0     5533 2023-04-15 00:10:05.692772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/rnn_view.py
+-rw-r--r--   0        0        0     4340 2023-04-15 00:10:05.692772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/rwd_model.py
+-rw-r--r--   0        0        0     3643 2023-04-15 00:10:05.692772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/rwd_view.py
+-rw-r--r--   0        0        0     4709 2023-04-15 00:10:05.692772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/seasonalnaive_model.py
+-rw-r--r--   0        0        0     3879 2023-04-15 00:10:05.692772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/seasonalnaive_view.py
+-rw-r--r--   0        0        0     5790 2023-04-15 00:10:05.692772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/tcn_model.py
+-rw-r--r--   0        0        0     6289 2023-04-15 00:10:05.692772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/tcn_view.py
+-rw-r--r--   0        0        0     7249 2023-04-15 00:10:05.692772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/tft_model.py
+-rw-r--r--   0        0        0     6520 2023-04-15 00:10:05.692772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/tft_view.py
+-rw-r--r--   0        0        0     4928 2023-04-15 00:10:05.692772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/theta_model.py
+-rw-r--r--   0        0        0     4379 2023-04-15 00:10:05.692772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/theta_view.py
+-rw-r--r--   0        0        0     6321 2023-04-15 00:10:05.692772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/trans_model.py
+-rw-r--r--   0        0        0     6765 2023-04-15 00:10:05.692772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/trans_view.py
+-rw-r--r--   0        0        0    12580 2023-04-15 00:10:05.692772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/whisper_model.py
+-rw-r--r--   0        0        0     2935 2023-04-15 00:10:05.692772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/whisper_utils.py
+-rw-r--r--   0        0        0      122 2023-04-15 00:10:05.692772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forex/README.md
+-rw-r--r--   0        0        0        0 2023-04-15 00:10:05.692772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forex/__init__.py
+-rw-r--r--   0        0        0     5077 2023-04-15 00:10:05.692772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forex/av_model.py
+-rw-r--r--   0        0        0     1458 2023-04-15 00:10:05.692772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forex/av_view.py
+-rw-r--r--   0        0        0     3281 2023-04-15 00:10:05.692772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forex/data/av_forex_currencies.csv
+-rw-r--r--   0        0        0     7847 2023-04-15 00:10:05.692772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forex/data/polygon_tickers.csv
+-rw-r--r--   0        0        0   419838 2023-04-15 00:10:05.692772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forex/data/yahoofinance_forex.json
+-rw-r--r--   0        0        0    16492 2023-04-15 00:10:05.692772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forex/forex_controller.py
+-rw-r--r--   0        0        0     8211 2023-04-15 00:10:05.692772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forex/forex_helper.py
+-rw-r--r--   0        0        0      931 2023-04-15 00:10:05.692772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forex/fxempire_model.py
+-rw-r--r--   0        0        0     1471 2023-04-15 00:10:05.692772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forex/fxempire_view.py
+-rw-r--r--   0        0        0    17162 2023-04-15 00:10:05.692772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forex/oanda/oanda_controller.py
+-rw-r--r--   0        0        0    22592 2023-04-15 00:10:05.696772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forex/oanda/oanda_model.py
+-rw-r--r--   0        0        0    12856 2023-04-15 00:10:05.696772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forex/oanda/oanda_view.py
+-rw-r--r--   0        0        0     2349 2023-04-15 00:10:05.696772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forex/polygon_model.py
+-rw-r--r--   0        0        0        0 2023-04-15 00:10:05.696772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forex/quantitative_analysis/__init__.py
+-rw-r--r--   0        0        0    26168 2023-04-15 00:10:05.696772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forex/quantitative_analysis/qa_controller.py
+-rw-r--r--   0        0        0     1446 2023-04-15 00:10:05.696772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forex/sdk_helpers.py
+-rw-r--r--   0        0        0        0 2023-04-15 00:10:05.696772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forex/technical_analysis/__init__.py
+-rw-r--r--   0        0        0    35136 2023-04-15 00:10:05.696772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forex/technical_analysis/ta_controller.py
+-rw-r--r--   0        0        0        0 2023-04-15 00:10:05.696772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/futures/__init__.py
+-rw-r--r--   0        0        0     2218 2023-04-15 00:10:05.696772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/futures/databento_view.py
+-rw-r--r--   0        0        0     8903 2023-04-15 00:10:05.696772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/futures/futures_controller.py
+-rw-r--r--   0        0        0      358 2023-04-15 00:10:05.696772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/futures/futures_helper.py
+-rw-r--r--   0        0        0      964 2023-04-15 00:10:05.696772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/futures/sdk_helper.py
+-rw-r--r--   0        0        0     4989 2023-04-15 00:10:05.696772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/futures/yfinance_model.py
+-rw-r--r--   0        0        0     7379 2023-04-15 00:10:05.696772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/futures/yfinance_view.py
+-rw-r--r--   0        0        0    13288 2023-04-15 00:10:05.696772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/helper_classes.py
+-rw-r--r--   0        0        0    67472 2023-04-15 00:10:05.696772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/helper_funcs.py
+-rw-r--r--   0        0        0     3212 2023-04-15 00:10:05.696772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/helpers_denomination.py
+-rw-r--r--   0        0        0     9736 2023-04-15 00:10:05.696772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/intro.json
+-rw-r--r--   0        0        0    42810 2023-04-15 00:10:05.696772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/keys_controller.py
+-rw-r--r--   0        0        0    80049 2023-04-15 00:10:05.696772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/keys_model.py
+-rw-r--r--   0        0        0     1148 2023-04-15 00:10:05.696772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/keys_view.py
+-rw-r--r--   0        0        0     5984 2023-04-15 00:10:05.696772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/loggers.py
+-rw-r--r--   0        0        0     1722 2023-04-15 00:10:05.696772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/menu.py
+-rw-r--r--   0        0        0    23784 2023-04-15 00:10:05.696772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/documentation_scripts/documentation_commands.csv
+-rw-r--r--   0        0        0    29952 2023-04-15 00:10:05.696772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/documentation_scripts/documentation_commands.json
+-rw-r--r--   0        0        0     6403 2023-04-15 00:10:05.696772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/documentation_scripts/documentation_commands_sdk.csv
+-rw-r--r--   0        0        0     8797 2023-04-15 00:10:05.696772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/documentation_scripts/documentation_commands_sdk.json
+-rw-r--r--   0        0        0    11455 2023-04-15 00:10:05.696772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/documentation_scripts/generate_documentation_commands.py
+-rw-r--r--   0        0        0        0 2023-04-15 00:10:05.696772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/exports/alternative/covid/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-15 00:10:05.696772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/exports/common/behavioural_analysis/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-15 00:10:05.696772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/exports/common/prediction_techniques/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-15 00:10:05.696772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/exports/common/quantitative_analysis/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-15 00:10:05.696772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/exports/common/technical_analysis/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-15 00:10:05.696772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/exports/custom/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-15 00:10:05.696772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/exports/econometrics/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-15 00:10:05.696772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/exports/economy/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-15 00:10:05.696772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/exports/etf/movers/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-15 00:10:05.696772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/exports/etf/screeners/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-15 00:10:05.696772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/exports/mutual_funds/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-15 00:10:05.696772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/exports/portfolio/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-15 00:10:05.696772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/exports/portfolio/views/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-15 00:10:05.696772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/exports/stocks/backtesting/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-15 00:10:05.696772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/exports/stocks/behavioural_analysis/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-15 00:10:05.696772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/exports/stocks/comparison_analysis/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-15 00:10:05.696772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/exports/stocks/dark_pool_shorts/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-15 00:10:05.696772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/exports/stocks/discovery/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-15 00:10:05.696772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/exports/stocks/due_diligence/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-15 00:10:05.696772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/exports/stocks/fundamental_analysis/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-15 00:10:05.696772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/exports/stocks/government/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-15 00:10:05.696772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/exports/stocks/insider/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-15 00:10:05.696772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/exports/stocks/options/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-15 00:10:05.696772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/exports/stocks/prediction_techniques/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-15 00:10:05.696772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/exports/stocks/quantitative_analysis/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-15 00:10:05.696772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/exports/stocks/raw_data/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-15 00:10:05.696772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/exports/stocks/sector_industry_analysis/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-15 00:10:05.696772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/exports/stocks/technical_analysis/.gitkeep
+-rw-r--r--   0        0        0     8528 2023-04-15 00:10:05.696772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/futures/futures.csv
+-rw-r--r--   0        0        0    60721 2023-04-15 00:10:05.696772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/i18n/en.yml
+-rw-r--r--   0        0        0     5831 2023-04-15 00:10:05.696772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/i18n/help_translation.ipynb
+-rw-r--r--   0        0        0        0 2023-04-15 00:10:05.696772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/.gitkeep
+-rw-r--r--   0        0        0     3868 2023-04-15 00:10:05.696772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/README.MD
+-rw-r--r--   0        0        0       85 2023-04-15 00:10:05.696772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/account/test_account.openbb
+-rw-r--r--   0        0        0       87 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/alternative/test_alt_covid.openbb
+-rw-r--r--   0        0        0      153 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/alternative/test_alt_oss.openbb
+-rw-r--r--   0        0        0      119 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/alternative/test_alt_realestate.openbb
+-rw-r--r--   0        0        0      856 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto.openbb
+-rw-r--r--   0        0        0      802 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_dd.openbb
+-rw-r--r--   0        0        0     1192 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_defi.openbb
+-rw-r--r--   0        0        0      374 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_disc.openbb
+-rw-r--r--   0        0        0      168 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_nft.openbb
+-rw-r--r--   0        0        0     1229 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_onchain.openbb
+-rw-r--r--   0        0        0     1533 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_ov.openbb
+-rw-r--r--   0        0        0      561 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_qa.openbb
+-rw-r--r--   0        0        0       87 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_shroom.openbb
+-rw-r--r--   0        0        0      768 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_ta.openbb
+-rw-r--r--   0        0        0      154 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_tools.openbb
+-rw-r--r--   0        0        0      120 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/dashboards/test_dashboards_base.openbb
+-rw-r--r--   0        0        0     1333 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/econometrics/test_econometrics_base.openbb
+-rw-r--r--   0        0        0     2028 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/economy/test_economy.openbb
+-rw-r--r--   0        0        0      155 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/etf/test_etf.openbb
+-rw-r--r--   0        0        0       33 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/etf/test_etf_ca.openbb
+-rw-r--r--   0        0        0       38 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/etf/test_etf_disc.openbb
+-rw-r--r--   0        0        0      878 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/etf/test_etf_ta.openbb
+-rw-r--r--   0        0        0      749 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/fixedincome/test_fixedincome.openbb
+-rw-r--r--   0        0        0      301 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/forecast/test_forecast.openbb
+-rw-r--r--   0        0        0      176 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/forecast/test_forecast_advanced.openbb
+-rw-r--r--   0        0        0      241 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/forex/test_forex_base.openbb
+-rw-r--r--   0        0        0      108 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/forex/test_forex_load.openbb
+-rw-r--r--   0        0        0      745 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/forex/test_forex_oanda.openbb
+-rw-r--r--   0        0        0       62 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/forex/test_forex_oanda_base.openbb
+-rw-r--r--   0        0        0      630 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/forex/test_forex_qa.openbb
+-rw-r--r--   0        0        0      611 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/forex/test_forex_ta.openbb
+-rw-r--r--   0        0        0      173 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/futures/test_futures.openbb
+-rw-r--r--   0        0        0     1275 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/portfolio/test_po_show_plot_rpf.openbb
+-rw-r--r--   0        0        0     1826 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/portfolio/test_portfolio.openbb
+-rw-r--r--   0        0        0       98 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/portfolio/test_portfolio_boolean_args.openbb
+-rw-r--r--   0        0        0      683 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/portfolio/test_portfolio_po.openbb
+-rw-r--r--   0        0        0       67 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/reports/test_reports_base.openbb
+-rw-r--r--   0        0        0       65 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/reports/test_reports_crypto.openbb
+-rw-r--r--   0        0        0      151 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/reports/test_reports_economy.openbb
+-rw-r--r--   0        0        0       83 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/reports/test_reports_equity.openbb
+-rw-r--r--   0        0        0      113 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/reports/test_reports_etf.openbb
+-rw-r--r--   0        0        0      174 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/reports/test_reports_forecast.openbb
+-rw-r--r--   0        0        0      158 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/reports/test_reports_forex.openbb
+-rw-r--r--   0        0        0      132 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/reports/test_reports_portfolio.openbb
+-rw-r--r--   0        0        0      102 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/reports/test_reports_run.openbb
+-rw-r--r--   0        0        0      258 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks.openbb
+-rw-r--r--   0        0        0      255 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_ba.openbb
+-rw-r--r--   0        0        0     1513 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_bt.openbb
+-rw-r--r--   0        0        0      422 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_ca.openbb
+-rw-r--r--   0        0        0      251 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_disc.openbb
+-rw-r--r--   0        0        0      145 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_dps.openbb
+-rw-r--r--   0        0        0     1874 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_fa.openbb
+-rw-r--r--   0        0        0       44 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_fa_base.openbb
+-rw-r--r--   0        0        0       31 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_fa_epsfc.openbb
+-rw-r--r--   0        0        0       31 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_fa_revfc.openbb
+-rw-r--r--   0        0        0      470 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_gov.openbb
+-rw-r--r--   0        0        0      276 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_ins.openbb
+-rw-r--r--   0        0        0      340 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_options.openbb
+-rw-r--r--   0        0        0       91 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_options_payoff.openbb
+-rw-r--r--   0        0        0      121 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_options_pricing.openbb
+-rw-r--r--   0        0        0       82 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_options_screen.openbb
+-rw-r--r--   0        0        0      644 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_qa.openbb
+-rw-r--r--   0        0        0      170 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_scr.openbb
+-rw-r--r--   0        0        0      347 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_sia.openbb
+-rw-r--r--   0        0        0      712 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_ta.openbb
+-rw-r--r--   0        0        0       82 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_th.openbb
+-rw-r--r--   0        0        0       65 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/test_jupyter_base.openbb
+-rw-r--r--   0        0        0       16 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/test_keys_.openbb
+-rw-r--r--   0        0        0       46 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/test_news.openbb
+-rw-r--r--   0        0        0     1072 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/models/hub_credentials.json
+-rw-r--r--   0        0        0      380 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/models/local_credentials.json
+-rw-r--r--   0        0        0    17970 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/portfolio/allocation_example.xlsx
+-rw-r--r--   0        0        0    29757 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/portfolio/holdings_example.xlsx
+-rw-r--r--   0        0        0      310 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/routines/routine_example.openbb
+-rw-r--r--   0        0        0    22116 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/sources/openbb_default.json
+-rw-r--r--   0        0        0     2332 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/insider/Agriculture.ini
+-rw-r--r--   0        0        0     2354 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/insider/Agro-Chemicals.ini
+-rw-r--r--   0        0        0     2341 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/insider/Air-Transportation.ini
+-rw-r--r--   0        0        0     2316 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/insider/Apparel.ini
+-rw-r--r--   0        0        0     2316 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/insider/Banks.ini
+-rw-r--r--   0        0        0     2346 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/insider/Brokers.ini
+-rw-r--r--   0        0        0     2336 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/insider/Building-Materials.ini
+-rw-r--r--   0        0        0     2346 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/insider/Business-Services.ini
+-rw-r--r--   0        0        0     2307 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/insider/Closed-End-Funds.ini
+-rw-r--r--   0        0        0     2309 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/insider/Construction.ini
+-rw-r--r--   0        0        0     2329 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/insider/Credit-Industry.ini
+-rw-r--r--   0        0        0     2353 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/insider/Durable-Goods.ini
+-rw-r--r--   0        0        0     2360 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/insider/Electronics.ini
+-rw-r--r--   0        0        0     2320 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/insider/Furniture.ini
+-rw-r--r--   0        0        0     2344 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/insider/Gold-Silver.ini
+-rw-r--r--   0        0        0     2315 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/insider/Grocery.ini
+-rw-r--r--   0        0        0     2346 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/insider/Ground-Freight.ini
+-rw-r--r--   0        0        0     2376 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/insider/Guided-Missiles.ini
+-rw-r--r--   0        0        0     2326 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/insider/Health.ini
+-rw-r--r--   0        0        0     2307 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/insider/Hotels.ini
+-rw-r--r--   0        0        0     2320 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/insider/Insurance-Agents.ini
+-rw-r--r--   0        0        0     2324 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/insider/Insurance-Carriers.ini
+-rw-r--r--   0        0        0     2334 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/insider/Investment-Offices.ini
+-rw-r--r--   0        0        0     2324 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/insider/Legal.ini
+-rw-r--r--   0        0        0     2313 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/insider/Lumber.ini
+-rw-r--r--   0        0        0     2341 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/insider/Manufacturing.ini
+-rw-r--r--   0        0        0     2296 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/insider/Mining.ini
+-rw-r--r--   0        0        0     2367 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/insider/Mortgages.ini
+-rw-r--r--   0        0        0     2342 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/insider/Nondurable-Goods.ini
+-rw-r--r--   0        0        0     2361 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/insider/Personal-Credit.ini
+-rw-r--r--   0        0        0     2351 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/insider/Pharmaceuticals.ini
+-rw-r--r--   0        0        0     2336 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/insider/Professional-Services.ini
+-rw-r--r--   0        0        0     2322 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/insider/Railroads.ini
+-rw-r--r--   0        0        0     2310 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/insider/Real-Estate.ini
+-rw-r--r--   0        0        0     2326 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/insider/Restaurants.ini
+-rw-r--r--   0        0        0     2341 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/insider/Retail-Stores.ini
+-rw-r--r--   0        0        0     2299 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/insider/Retail-Trade.ini
+-rw-r--r--   0        0        0     2316 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/insider/Tobacco.ini
+-rw-r--r--   0        0        0     2342 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/insider/Utility-Communications.ini
+-rw-r--r--   0        0        0     2381 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/insider/Utility-Gas.ini
+-rw-r--r--   0        0        0     2314 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/insider/Wholesale-Trade.ini
+-rw-r--r--   0        0        0    34473 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/insider/template.ini
+-rw-r--r--   0        0        0    34519 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/insider/whales.ini
+-rw-r--r--   0        0        0     2688 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/options/README.md
+-rw-r--r--   0        0        0     4195 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/options/high_iv.ini
+-rw-r--r--   0        0        0     4210 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/options/iv_below_20day.ini
+-rw-r--r--   0        0        0     3925 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/options/liquid_otm.ini
+-rw-r--r--   0        0        0     4202 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/options/spy_30_delta.ini
+-rw-r--r--   0        0        0     4079 2023-04-15 00:10:05.700772 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/options/template.ini
+-rwxr-xr-x   0        0        0      282 2023-04-15 00:10:05.704773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/screener/5pct_above_low.ini
+-rw-r--r--   0        0        0    21940 2023-04-15 00:10:05.704773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/screener/all_parameters.txt
+-rwxr-xr-x   0        0        0      315 2023-04-15 00:10:05.704773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/screener/analyst_strong_buy.ini
+-rwxr-xr-x   0        0        0      464 2023-04-15 00:10:05.704773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/screener/break_out_stocks.ini
+-rw-r--r--   0        0        0      413 2023-04-15 00:10:05.704773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/screener/buffett_like.ini
+-rwxr-xr-x   0        0        0      184 2023-04-15 00:10:05.704773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/screener/bull_runs_over_10pct.ini
+-rwxr-xr-x   0        0        0      364 2023-04-15 00:10:05.704773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/screener/channel_up_and_low_debt_and_sma_50and200.ini
+-rw-r--r--   0        0        0      326 2023-04-15 00:10:05.704773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/screener/cheap_bottom_dividend.ini
+-rw-r--r--   0        0        0      193 2023-04-15 00:10:05.704773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/screener/cheap_dividend.ini
+-rw-r--r--   0        0        0      241 2023-04-15 00:10:05.704773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/screener/cheap_oversold.ini
+-rwxr-xr-x   0        0        0      335 2023-04-15 00:10:05.704773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/screener/continued_momentum_scan.ini
+-rw-r--r--   0        0        0      286 2023-04-15 00:10:05.704773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/screener/death_cross.ini
+-rwxr-xr-x   0        0        0      167 2023-04-15 00:10:05.704773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/screener/djia_components.ini
+-rw-r--r--   0        0        0      221 2023-04-15 00:10:05.704773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/screener/golden_cross.ini
+-rwxr-xr-x   0        0        0      255 2023-04-15 00:10:05.704773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/screener/golden_cross_penny.ini
+-rwxr-xr-x   0        0        0      518 2023-04-15 00:10:05.704773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/screener/growth_stocks.ini
+-rw-r--r--   0        0        0      302 2023-04-15 00:10:05.704773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/screener/heavy_inst_ins.ini
+-rwxr-xr-x   0        0        0      279 2023-04-15 00:10:05.704773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/screener/high_vol_and_low_debt.ini
+-rw-r--r--   0        0        0      316 2023-04-15 00:10:05.704773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/screener/modified_dreman.ini
+-rw-r--r--   0        0        0      349 2023-04-15 00:10:05.704773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/screener/modified_neff.ini
+-rwxr-xr-x   0        0        0      295 2023-04-15 00:10:05.704773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/screener/news_scanner.ini
+-rwxr-xr-x   0        0        0      274 2023-04-15 00:10:05.704773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/screener/oversold.ini
+-rwxr-xr-x   0        0        0      328 2023-04-15 00:10:05.704773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/screener/oversold_under_3dol.ini
+-rwxr-xr-x   0        0        0      301 2023-04-15 00:10:05.704773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/screener/oversold_under_5dol.ini
+-rwxr-xr-x   0        0        0      212 2023-04-15 00:10:05.704773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/screener/potential_reversals.ini
+-rwxr-xr-x   0        0        0      295 2023-04-15 00:10:05.704773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/screener/recent_growth_and_support.ini
+-rw-r--r--   0        0        0      337 2023-04-15 00:10:05.704773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/screener/rosenwald.ini
+-rw-r--r--   0        0        0      280 2023-04-15 00:10:05.704773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/screener/rosenwald_gtfo.ini
+-rw-r--r--   0        0        0      246 2023-04-15 00:10:05.704773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/screener/sdk_guide_preset.ini
+-rw-r--r--   0        0        0      360 2023-04-15 00:10:05.704773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/screener/sexy_year.ini
+-rwxr-xr-x   0        0        0      222 2023-04-15 00:10:05.704773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/screener/short_squeeze_scan.ini
+-rwxr-xr-x   0        0        0      260 2023-04-15 00:10:05.704773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/screener/simplistic_momentum_scanner_under_7dol.ini
+-rwxr-xr-x   0        0        0      197 2023-04-15 00:10:05.704773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/screener/sp500_basic_materials_sector.ini
+-rwxr-xr-x   0        0        0      211 2023-04-15 00:10:05.704773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/screener/sp500_communication_services_sector.ini
+-rwxr-xr-x   0        0        0      201 2023-04-15 00:10:05.704773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/screener/sp500_consumer_cyclical_sector.ini
+-rwxr-xr-x   0        0        0      203 2023-04-15 00:10:05.704773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/screener/sp500_consumer_defensive_sector.ini
+-rwxr-xr-x   0        0        0      179 2023-04-15 00:10:05.704773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/screener/sp500_energy_sector.ini
+-rwxr-xr-x   0        0        0      185 2023-04-15 00:10:05.704773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/screener/sp500_financial_sector.ini
+-rwxr-xr-x   0        0        0      187 2023-04-15 00:10:05.704773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/screener/sp500_healthcare_sector.ini
+-rwxr-xr-x   0        0        0      189 2023-04-15 00:10:05.704773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/screener/sp500_industrials_sector.ini
+-rwxr-xr-x   0        0        0      189 2023-04-15 00:10:05.704773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/screener/sp500_real_estate_sector.ini
+-rwxr-xr-x   0        0        0      187 2023-04-15 00:10:05.704773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/screener/sp500_technology_sector.ini
+-rwxr-xr-x   0        0        0      185 2023-04-15 00:10:05.704773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/screener/sp500_utilities_sector.ini
+-rwxr-xr-x   0        0        0      276 2023-04-15 00:10:05.704773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/screener/stocks_strong_support_levels.ini
+-rwxr-xr-x   0        0        0      272 2023-04-15 00:10:05.704773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/screener/top_performers_all.ini
+-rwxr-xr-x   0        0        0      299 2023-04-15 00:10:05.704773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/screener/top_performers_healthcare.ini
+-rwxr-xr-x   0        0        0      293 2023-04-15 00:10:05.704773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/screener/top_performers_tech.ini
+-rwxr-xr-x   0        0        0      286 2023-04-15 00:10:05.704773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/screener/under_15dol_stocks.ini
+-rw-r--r--   0        0        0      209 2023-04-15 00:10:05.704773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/screener/undervalue.ini
+-rwxr-xr-x   0        0        0      272 2023-04-15 00:10:05.704773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/screener/unusual_volume.ini
+-rwxr-xr-x   0        0        0      675 2023-04-15 00:10:05.704773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/screener/value_stocks.ini
+-rwxr-xr-x   0        0        0      315 2023-04-15 00:10:05.704773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/screener/weak_support_and_top_performers.ini
+-rw-r--r--   0        0        0   358460 2023-04-15 00:10:05.704773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/styles/default/Consolas.ttf
+-rw-r--r--   0        0        0      972 2023-04-15 00:10:05.704773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/styles/default/dark.mpfstyle.json
+-rw-r--r--   0        0        0      182 2023-04-15 00:10:05.704773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/styles/default/dark.mplrc.json
+-rw-r--r--   0        0        0     2086 2023-04-15 00:10:05.704773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/styles/default/dark.mplstyle
+-rw-r--r--   0        0        0     2750 2023-04-15 00:10:05.708773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/styles/default/dark.pltstyle.json
+-rw-r--r--   0        0        0      203 2023-04-15 00:10:05.708773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/styles/default/dark.richstyle.json
+-rw-r--r--   0        0        0      970 2023-04-15 00:10:05.708773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/styles/default/light.mpfstyle.json
+-rw-r--r--   0        0        0      182 2023-04-15 00:10:05.708773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/styles/default/light.mplrc.json
+-rw-r--r--   0        0        0     2035 2023-04-15 00:10:05.708773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/styles/default/light.mplstyle
+-rw-r--r--   0        0        0    24077 2023-04-15 00:10:05.708773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/styles/default/light.pltstyle.json
+-rw-r--r--   0        0        0      202 2023-04-15 00:10:05.708773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/styles/default/light.richstyle.json
+-rw-r--r--   0        0        0     2607 2023-04-15 00:10:05.708773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/styles/default/tables.pltstyle.json
+-rw-r--r--   0        0        0      186 2023-04-15 00:10:05.708773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/styles/user/openbb.richstyle.json
+-rw-r--r--   0        0        0      144 2023-04-15 00:10:05.708773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/mutual_funds/README.md
+-rw-r--r--   0        0        0        0 2023-04-15 00:10:05.708773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/mutual_funds/__init__.py
+-rw-r--r--   0        0        0    81373 2023-04-15 00:10:05.708773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/mutual_funds/avanza_fund_ID.csv
+-rw-r--r--   0        0        0      834 2023-04-15 00:10:05.708773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/mutual_funds/avanza_model.py
+-rw-r--r--   0        0        0     3941 2023-04-15 00:10:05.708773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/mutual_funds/avanza_view.py
+-rw-r--r--   0        0        0     6535 2023-04-15 00:10:05.708773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/mutual_funds/mstarpy_model.py
+-rw-r--r--   0        0        0     7883 2023-04-15 00:10:05.708773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/mutual_funds/mstarpy_view.py
+-rw-r--r--   0        0        0    15141 2023-04-15 00:10:05.708773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/mutual_funds/mutual_fund_controller.py
+-rw-r--r--   0        0        0     6040 2023-04-15 00:10:05.708773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/mutual_funds/mutual_funds_utils.py
+-rw-r--r--   0        0        0    51056 2023-04-15 00:10:05.708773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/parent_classes.py
+-rw-r--r--   0        0        0       61 2023-04-15 00:10:05.708773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/portfolio/__init__.py
+-rw-r--r--   0        0        0    15080 2023-04-15 00:10:05.708773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/portfolio/allocation_model.py
+-rw-r--r--   0        0        0    12944 2023-04-15 00:10:05.708773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/portfolio/attribution_model.py
+-rw-r--r--   0        0        0      417 2023-04-15 00:10:05.708773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/portfolio/brokers/README.md
+-rw-r--r--   0        0        0        0 2023-04-15 00:10:05.708773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/portfolio/brokers/__init__.py
+-rw-r--r--   0        0        0     3214 2023-04-15 00:10:05.708773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/portfolio/brokers/bro_controller.py
+-rw-r--r--   0        0        0     1121 2023-04-15 00:10:05.708773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/portfolio/brokers/brokers_helpers.py
+-rw-r--r--   0        0        0        0 2023-04-15 00:10:05.708773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/portfolio/brokers/coinbase/__init__.py
+-rw-r--r--   0        0        0     8211 2023-04-15 00:10:05.708773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/portfolio/brokers/coinbase/coinbase_controller.py
+-rw-r--r--   0        0        0     9561 2023-04-15 00:10:05.708773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/portfolio/brokers/coinbase/coinbase_model.py
+-rw-r--r--   0        0        0     4495 2023-04-15 00:10:05.708773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/portfolio/brokers/coinbase/coinbase_view.py
+-rw-r--r--   0        0        0     4666 2023-04-15 00:10:05.708773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/portfolio/brokers/degiro/README.md
+-rw-r--r--   0        0        0        0 2023-04-15 00:10:05.708773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/portfolio/brokers/degiro/__init__.py
+-rw-r--r--   0        0        0    12789 2023-04-15 00:10:05.708773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/portfolio/brokers/degiro/degiro_controller.py
+-rw-r--r--   0        0        0    15571 2023-04-15 00:10:05.708773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/portfolio/brokers/degiro/degiro_model.py
+-rw-r--r--   0        0        0    15670 2023-04-15 00:10:05.708773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/portfolio/brokers/degiro/degiro_view.py
+-rw-r--r--   0        0        0     3894 2023-04-15 00:10:05.708773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/portfolio/brokers/robinhood/robinhood_controller.py
+-rw-r--r--   0        0        0     3002 2023-04-15 00:10:05.708773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/portfolio/brokers/robinhood/robinhood_model.py
+-rw-r--r--   0        0        0     2482 2023-04-15 00:10:05.708773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/portfolio/brokers/robinhood/robinhood_view.py
+-rw-r--r--   0        0        0    30861 2023-04-15 00:10:05.708773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/portfolio/metrics_model.py
+-rw-r--r--   0        0        0    54979 2023-04-15 00:10:05.708773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/portfolio/portfolio_controller.py
+-rw-r--r--   0        0        0    39188 2023-04-15 00:10:05.708773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/portfolio/portfolio_engine.py
+-rw-r--r--   0        0        0     9643 2023-04-15 00:10:05.708773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/portfolio/portfolio_helper.py
+-rw-r--r--   0        0        0    60205 2023-04-15 00:10:05.708773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/portfolio/portfolio_model.py
+-rw-r--r--   0        0        0        0 2023-04-15 00:10:05.708773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/portfolio/portfolio_optimization/__init__.py
+-rw-r--r--   0        0        0     5255 2023-04-15 00:10:05.708773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/portfolio/portfolio_optimization/excel_model.py
+-rw-r--r--   0        0        0     2106 2023-04-15 00:10:05.708773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/portfolio/portfolio_optimization/optimizer_helper.py
+-rw-r--r--   0        0        0   120571 2023-04-15 00:10:05.708773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/portfolio/portfolio_optimization/optimizer_model.py
+-rw-r--r--   0        0        0   155050 2023-04-15 00:10:05.712773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/portfolio/portfolio_optimization/optimizer_view.py
+-rw-r--r--   0        0        0     2773 2023-04-15 00:10:05.712773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/portfolio/portfolio_optimization/parameters/Parameter.py
+-rw-r--r--   0        0        0    13116 2023-04-15 00:10:05.712773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/portfolio/portfolio_optimization/parameters/params_controller.py
+-rw-r--r--   0        0        0     5965 2023-04-15 00:10:05.712773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/portfolio/portfolio_optimization/parameters/params_helpers.py
+-rw-r--r--   0        0        0     5346 2023-04-15 00:10:05.712773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/portfolio/portfolio_optimization/parameters/params_statics.py
+-rw-r--r--   0        0        0     4427 2023-04-15 00:10:05.712773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/portfolio/portfolio_optimization/parameters/params_view.py
+-rw-r--r--   0        0        0   138034 2023-04-15 00:10:05.712773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/portfolio/portfolio_optimization/po_controller.py
+-rw-r--r--   0        0        0     8587 2023-04-15 00:10:05.712773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/portfolio/portfolio_optimization/po_engine.py
+-rw-r--r--   0        0        0   103568 2023-04-15 00:10:05.712773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/portfolio/portfolio_optimization/po_model.py
+-rw-r--r--   0        0        0    24186 2023-04-15 00:10:05.712773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/portfolio/portfolio_optimization/po_view.py
+-rw-r--r--   0        0        0    11390 2023-04-15 00:10:05.712773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/portfolio/portfolio_optimization/statics.py
+-rw-r--r--   0        0        0    12009 2023-04-15 00:10:05.712773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/portfolio/portfolio_optimization/yahoo_finance_model.py
+-rw-r--r--   0        0        0    54944 2023-04-15 00:10:05.712773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/portfolio/portfolio_view.py
+-rw-r--r--   0        0        0     8433 2023-04-15 00:10:05.712773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/portfolio/statics.py
+-rw-r--r--   0        0        0     2877 2023-04-15 00:10:05.712773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/reporting.md
+-rw-r--r--   0        0        0  1028287 2023-04-15 00:10:05.716773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/reports/.ipynb_checkpoints/test-checkpoint.html
+-rw-r--r--   0        0        0     2839 2023-04-15 00:10:05.716773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/reports/README.md
+-rw-r--r--   0        0        0        0 2023-04-15 00:10:05.716773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/reports/__init__.py
+-rw-r--r--   0        0        0      443 2023-04-15 00:10:05.716773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/reports/data/crypto_tickers.csv
+-rw-r--r--   0        0        0      437 2023-04-15 00:10:05.716773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/reports/data/etf_tickers.csv
+-rw-r--r--   0        0        0      222 2023-04-15 00:10:05.716773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/reports/data/stocks_tickers.csv
+-rw-r--r--   0        0        0     9707 2023-04-15 00:10:05.716773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/reports/reports_controller.py
+-rw-r--r--   0        0        0    12310 2023-04-15 00:10:05.716773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/reports/reports_model.py
+-rw-r--r--   0        0        0        0 2023-04-15 00:10:05.716773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/reports/stored/.gitkeep
+-rw-r--r--   0        0        0  1076317 2023-04-15 00:10:05.724773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/reports/stored/20220512_040312_equity_NVDA.html
+-rw-r--r--   0        0        0     5214 2023-04-15 00:10:05.724773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/reports/templates/OpenBB_reports_logo.png
+-rw-r--r--   0        0        0    32656 2023-04-15 00:10:05.724773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/reports/templates/crypto.ipynb
+-rw-r--r--   0        0        0    23095 2023-04-15 00:10:05.724773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/reports/templates/economy.ipynb
+-rw-r--r--   0        0        0    39713 2023-04-15 00:10:05.724773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/reports/templates/equity.ipynb
+-rw-r--r--   0        0        0     9900 2023-04-15 00:10:05.724773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/reports/templates/etf.ipynb
+-rw-r--r--   0        0        0     2782 2023-04-15 00:10:05.724773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/reports/templates/floppy-disc.png
+-rw-r--r--   0        0        0     8567 2023-04-15 00:10:05.724773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/reports/templates/forecast.ipynb
+-rw-r--r--   0        0        0    17778 2023-04-15 00:10:05.724773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/reports/templates/forex.ipynb
+-rw-r--r--   0        0        0    14922 2023-04-15 00:10:05.724773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/reports/templates/portfolio.ipynb
+-rw-r--r--   0        0        0    11247 2023-04-15 00:10:05.724773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/reports/widget_helpers.py
+-rw-r--r--   0        0        0      205 2023-04-15 00:10:05.724773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/reports/widgets/card.j2
+-rw-r--r--   0        0        0     3556 2023-04-15 00:10:05.724773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/reports/widgets/report.css
+-rw-r--r--   0        0        0      474 2023-04-15 00:10:05.724773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/reports/widgets/report.j2
+-rw-r--r--   0        0        0      119 2023-04-15 00:10:05.724773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/reports/widgets/row.j2
+-rw-r--r--   0        0        0      896 2023-04-15 00:10:05.724773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/reports/widgets/style.css
+-rw-r--r--   0        0        0     9967 2023-04-15 00:10:05.724773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/rich_config.py
+-rw-r--r--   0        0        0    30827 2023-04-15 00:10:05.724773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/sdk.py
+-rw-r--r--   0        0        0    24274 2023-04-15 00:10:05.724773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/settings_controller.py
+-rw-r--r--   0        0        0     7105 2023-04-15 00:10:05.724773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/sources_controller.py
+-rw-r--r--   0        0        0      357 2023-04-15 00:10:05.724773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/README.md
+-rw-r--r--   0        0        0        0 2023-04-15 00:10:05.724773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-15 00:10:05.724773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/backtesting/__init__.py
+-rw-r--r--   0        0        0    10448 2023-04-15 00:10:05.724773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/backtesting/bt_controller.py
+-rw-r--r--   0        0        0     8126 2023-04-15 00:10:05.724773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/backtesting/bt_model.py
+-rw-r--r--   0        0        0     9046 2023-04-15 00:10:05.724773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/backtesting/bt_view.py
+-rw-r--r--   0        0        0        0 2023-04-15 00:10:05.724773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/behavioural_analysis/__init__.py
+-rw-r--r--   0        0        0    29872 2023-04-15 00:10:05.724773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/behavioural_analysis/ba_controller.py
+-rw-r--r--   0        0        0     3541 2023-04-15 00:10:05.724773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/behavioural_analysis/finnhub_model.py
+-rw-r--r--   0        0        0     3761 2023-04-15 00:10:05.724773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/behavioural_analysis/finnhub_view.py
+-rw-r--r--   0        0        0     1931 2023-04-15 00:10:05.724773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/cboe_model.py
+-rw-r--r--   0        0        0      969 2023-04-15 00:10:05.724773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/cboe_view.py
+-rw-r--r--   0        0        0        0 2023-04-15 00:10:05.724773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/comparison_analysis/__init__.py
+-rw-r--r--   0        0        0    37655 2023-04-15 00:10:05.724773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/comparison_analysis/ca_controller.py
+-rw-r--r--   0        0        0     4871 2023-04-15 00:10:05.724773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/comparison_analysis/finbrain_model.py
+-rw-r--r--   0        0        0     5785 2023-04-15 00:10:05.724773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/comparison_analysis/finbrain_view.py
+-rw-r--r--   0        0        0     1328 2023-04-15 00:10:05.724773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/comparison_analysis/finnhub_model.py
+-rw-r--r--   0        0        0     2679 2023-04-15 00:10:05.724773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/comparison_analysis/finviz_compare_model.py
+-rw-r--r--   0        0        0     1539 2023-04-15 00:10:05.724773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/comparison_analysis/finviz_compare_view.py
+-rw-r--r--   0        0        0    12381 2023-04-15 00:10:05.724773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/comparison_analysis/marketwatch_model.py
+-rw-r--r--   0        0        0     5757 2023-04-15 00:10:05.724773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/comparison_analysis/marketwatch_view.py
+-rw-r--r--   0        0        0     1690 2023-04-15 00:10:05.724773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/comparison_analysis/polygon_model.py
+-rw-r--r--   0        0        0     1379 2023-04-15 00:10:05.724773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/comparison_analysis/sdk_helpers.py
+-rw-r--r--   0        0        0     8073 2023-04-15 00:10:05.724773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/comparison_analysis/yahoo_finance_model.py
+-rw-r--r--   0        0        0    10157 2023-04-15 00:10:05.724773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/comparison_analysis/yahoo_finance_view.py
+-rw-r--r--   0        0        0        0 2023-04-15 00:10:05.724773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/dark_pool_shorts/__init__.py
+-rw-r--r--   0        0        0    20377 2023-04-15 00:10:05.724773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/dark_pool_shorts/dps_controller.py
+-rw-r--r--   0        0        0    10009 2023-04-15 00:10:05.724773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/dark_pool_shorts/finra_model.py
+-rw-r--r--   0        0        0     7203 2023-04-15 00:10:05.724773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/dark_pool_shorts/finra_view.py
+-rw-r--r--   0        0        0     1093 2023-04-15 00:10:05.724773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/dark_pool_shorts/ibkr_model.py
+-rw-r--r--   0        0        0     1200 2023-04-15 00:10:05.728773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/dark_pool_shorts/ibkr_view.py
+-rw-r--r--   0        0        0     1387 2023-04-15 00:10:05.728773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/dark_pool_shorts/quandl_model.py
+-rw-r--r--   0        0        0     4648 2023-04-15 00:10:05.728773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/dark_pool_shorts/quandl_view.py
+-rw-r--r--   0        0        0     6836 2023-04-15 00:10:05.728773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/dark_pool_shorts/sec_model.py
+-rw-r--r--   0        0        0     3470 2023-04-15 00:10:05.728773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/dark_pool_shorts/sec_view.py
+-rw-r--r--   0        0        0     1882 2023-04-15 00:10:05.728773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/dark_pool_shorts/shortinterest_model.py
+-rw-r--r--   0        0        0     1385 2023-04-15 00:10:05.728773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/dark_pool_shorts/shortinterest_view.py
+-rw-r--r--   0        0        0     5053 2023-04-15 00:10:05.728773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/dark_pool_shorts/stockgrid_model.py
+-rw-r--r--   0        0        0     9997 2023-04-15 00:10:05.728773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/dark_pool_shorts/stockgrid_view.py
+-rw-r--r--   0        0        0     1166 2023-04-15 00:10:05.728773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/dark_pool_shorts/stocksera_model.py
+-rw-r--r--   0        0        0     3613 2023-04-15 00:10:05.728773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/dark_pool_shorts/stocksera_view.py
+-rw-r--r--   0        0        0      668 2023-04-15 00:10:05.728773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/dark_pool_shorts/yahoofinance_model.py
+-rw-r--r--   0        0        0     1271 2023-04-15 00:10:05.728773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/dark_pool_shorts/yahoofinance_view.py
+-rw-r--r--   0        0        0     5740 2023-04-15 00:10:05.728773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/databento_model.py
+-rw-r--r--   0        0        0        0 2023-04-15 00:10:05.728773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/discovery/__init__.py
+-rw-r--r--   0        0        0     4169 2023-04-15 00:10:05.728773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/discovery/ark_model.py
+-rw-r--r--   0        0        0     2589 2023-04-15 00:10:05.728773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/discovery/ark_view.py
+-rw-r--r--   0        0        0    31510 2023-04-15 00:10:05.728773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/discovery/disc_controller.py
+-rw-r--r--   0        0        0      483 2023-04-15 00:10:05.728773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/discovery/disc_helpers.py
+-rw-r--r--   0        0        0     2696 2023-04-15 00:10:05.728773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/discovery/fidelity_model.py
+-rw-r--r--   0        0        0     2680 2023-04-15 00:10:05.728773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/discovery/fidelity_view.py
+-rw-r--r--   0        0        0     4164 2023-04-15 00:10:05.728773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/discovery/finnhub_model.py
+-rw-r--r--   0        0        0     2510 2023-04-15 00:10:05.728773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/discovery/finnhub_view.py
+-rw-r--r--   0        0        0     1731 2023-04-15 00:10:05.728773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/discovery/finviz_model.py
+-rw-r--r--   0        0        0     3084 2023-04-15 00:10:05.728773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/discovery/finviz_view.py
+-rw-r--r--   0        0        0     2562 2023-04-15 00:10:05.728773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/discovery/fmp_view.py
+-rw-r--r--   0        0        0     3051 2023-04-15 00:10:05.728773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/discovery/nasdaq_model.py
+-rw-r--r--   0        0        0     3406 2023-04-15 00:10:05.728773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/discovery/nasdaq_view.py
+-rw-r--r--   0        0        0     7080 2023-04-15 00:10:05.728773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/discovery/seeking_alpha_model.py
+-rw-r--r--   0        0        0     4803 2023-04-15 00:10:05.728773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/discovery/seeking_alpha_view.py
+-rw-r--r--   0        0        0     1120 2023-04-15 00:10:05.728773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/discovery/shortinterest_model.py
+-rw-r--r--   0        0        0     2566 2023-04-15 00:10:05.728773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/discovery/shortinterest_view.py
+-rw-r--r--   0        0        0     4113 2023-04-15 00:10:05.728773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/discovery/yahoofinance_model.py
+-rw-r--r--   0        0        0     5871 2023-04-15 00:10:05.728773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/discovery/yahoofinance_view.py
+-rw-r--r--   0        0        0        0 2023-04-15 00:10:05.728773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/fundamental_analysis/__init__.py
+-rw-r--r--   0        0        0    24082 2023-04-15 00:10:05.728773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/fundamental_analysis/av_model.py
+-rw-r--r--   0        0        0    14910 2023-04-15 00:10:05.728773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/fundamental_analysis/av_view.py
+-rw-r--r--   0        0        0    10325 2023-04-15 00:10:05.728773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/fundamental_analysis/business_insider_model.py
+-rw-r--r--   0        0        0     7696 2023-04-15 00:10:05.728773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/fundamental_analysis/business_insider_view.py
+-rw-r--r--   0        0        0     1833 2023-04-15 00:10:05.728773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/fundamental_analysis/csimarket_model.py
+-rw-r--r--   0        0        0     2347 2023-04-15 00:10:05.728773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/fundamental_analysis/csimarket_view.py
+-rw-r--r--   0        0        0    14888 2023-04-15 00:10:05.728773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/fundamental_analysis/dcf_model.py
+-rw-r--r--   0        0        0     4279 2023-04-15 00:10:05.728773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/fundamental_analysis/dcf_static.py
+-rw-r--r--   0        0        0    44464 2023-04-15 00:10:05.728773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/fundamental_analysis/dcf_view.py
+-rw-r--r--   0        0        0     1925 2023-04-15 00:10:05.728773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/fundamental_analysis/eclect_us_model.py
+-rw-r--r--   0        0        0     1205 2023-04-15 00:10:05.728773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/fundamental_analysis/eclect_us_view.py
+-rw-r--r--   0        0        0     2396 2023-04-15 00:10:05.728773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/fundamental_analysis/eodhd_model.py
+-rw-r--r--   0        0        0     4904 2023-04-15 00:10:05.728773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/fundamental_analysis/eodhd_view.py
+-rw-r--r--   0        0        0    82041 2023-04-15 00:10:05.728773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/fundamental_analysis/fa_controller.py
+-rw-r--r--   0        0        0      266 2023-04-15 00:10:05.728773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/fundamental_analysis/fa_helper.py
+-rw-r--r--   0        0        0     1389 2023-04-15 00:10:05.728773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/fundamental_analysis/finnhub_model.py
+-rw-r--r--   0        0        0     3518 2023-04-15 00:10:05.728773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/fundamental_analysis/finnhub_view.py
+-rw-r--r--   0        0        0     3419 2023-04-15 00:10:05.728773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/fundamental_analysis/finviz_model.py
+-rw-r--r--   0        0        0     2484 2023-04-15 00:10:05.728773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/fundamental_analysis/finviz_view.py
+-rw-r--r--   0        0        0    22206 2023-04-15 00:10:05.728773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/fundamental_analysis/fmp_model.py
+-rw-r--r--   0        0        0    23886 2023-04-15 00:10:05.728773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/fundamental_analysis/fmp_view.py
+-rw-r--r--   0        0        0     6417 2023-04-15 00:10:05.728773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/fundamental_analysis/key_metrics_explained.txt
+-rw-r--r--   0        0        0    14313 2023-04-15 00:10:05.728773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/fundamental_analysis/marketwatch_model.py
+-rw-r--r--   0        0        0     2870 2023-04-15 00:10:05.728773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/fundamental_analysis/marketwatch_view.py
+-rw-r--r--   0        0        0     5391 2023-04-15 00:10:05.728773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/fundamental_analysis/polygon_model.py
+-rw-r--r--   0        0        0     4361 2023-04-15 00:10:05.728773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/fundamental_analysis/polygon_view.py
+-rw-r--r--   0        0        0     7593 2023-04-15 00:10:05.728773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/fundamental_analysis/sdk_helpers.py
+-rw-r--r--   0        0        0    11162 2023-04-15 00:10:05.728773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/fundamental_analysis/seeking_alpha_model.py
+-rw-r--r--   0        0        0     2059 2023-04-15 00:10:05.728773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/fundamental_analysis/seeking_alpha_view.py
+-rw-r--r--   0        0        0    11829 2023-04-15 00:10:05.728773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/fundamental_analysis/yahoo_finance_model.py
+-rw-r--r--   0        0        0    14679 2023-04-15 00:10:05.728773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/fundamental_analysis/yahoo_finance_view.py
+-rw-r--r--   0        0        0        0 2023-04-15 00:10:05.728773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/government/__init__.py
+-rw-r--r--   0        0        0    18461 2023-04-15 00:10:05.728773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/government/gov_controller.py
+-rw-r--r--   0        0        0    15719 2023-04-15 00:10:05.728773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/government/quiverquant_model.py
+-rw-r--r--   0        0        0    21407 2023-04-15 00:10:05.728773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/government/quiverquant_view.py
+-rw-r--r--   0        0        0        0 2023-04-15 00:10:05.728773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/insider/__init__.py
+-rw-r--r--   0        0        0     2062 2023-04-15 00:10:05.728773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/insider/businessinsider_model.py
+-rw-r--r--   0        0        0     5102 2023-04-15 00:10:05.728773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/insider/businessinsider_view.py
+-rw-r--r--   0        0        0     1125 2023-04-15 00:10:05.732773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/insider/finviz_model.py
+-rw-r--r--   0        0        0     1171 2023-04-15 00:10:05.732773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/insider/finviz_view.py
+-rw-r--r--   0        0        0    32744 2023-04-15 00:10:05.732773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/insider/insider_controller.py
+-rw-r--r--   0        0        0    87496 2023-04-15 00:10:05.732773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/insider/openinsider_model.py
+-rw-r--r--   0        0        0     7695 2023-04-15 00:10:05.732773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/insider/openinsider_view.py
+-rw-r--r--   0        0        0     4909 2023-04-15 00:10:05.732773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/insider/sdk_helper.py
+-rw-r--r--   0        0        0    76085 2023-04-15 00:10:05.732773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/mappings/Mic_Codes.csv
+-rw-r--r--   0        0        0        0 2023-04-15 00:10:05.732773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/options/__init__.py
+-rw-r--r--   0        0        0     1757 2023-04-15 00:10:05.732773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/options/alphaquery_model.py
+-rw-r--r--   0        0        0     1713 2023-04-15 00:10:05.732773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/options/alphaquery_view.py
+-rw-r--r--   0        0        0     1161 2023-04-15 00:10:05.732773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/options/barchart_model.py
+-rw-r--r--   0        0        0     1137 2023-04-15 00:10:05.732773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/options/barchart_view.py
+-rw-r--r--   0        0        0     1526 2023-04-15 00:10:05.732773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/options/calculator_model.py
+-rw-r--r--   0        0        0     2416 2023-04-15 00:10:05.732773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/options/calculator_view.py
+-rw-r--r--   0        0        0     2777 2023-04-15 00:10:05.732773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/options/chartexchange_model.py
+-rw-r--r--   0        0        0     3211 2023-04-15 00:10:05.732773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/options/chartexchange_view.py
+-rw-r--r--   0        0        0     2433 2023-04-15 00:10:05.732773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/options/fdscanner_model.py
+-rw-r--r--   0        0        0     1672 2023-04-15 00:10:05.732773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/options/fdscanner_view.py
+-rw-r--r--   0        0        0    21092 2023-04-15 00:10:05.732773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/options/hedge/hedge_controller.py
+-rw-r--r--   0        0        0     9884 2023-04-15 00:10:05.732773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/options/hedge/hedge_model.py
+-rw-r--r--   0        0        0     3968 2023-04-15 00:10:05.732773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/options/hedge/hedge_view.py
+-rw-r--r--   0        0        0    10030 2023-04-15 00:10:05.732773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/options/intrinio_model.py
+-rw-r--r--   0        0        0     6113 2023-04-15 00:10:05.732773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/options/intrinio_view.py
+-rw-r--r--   0        0        0     7097 2023-04-15 00:10:05.732773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/options/nasdaq_model.py
+-rw-r--r--   0        0        0    22486 2023-04-15 00:10:05.732773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/options/op_helpers.py
+-rw-r--r--   0        0        0    51845 2023-04-15 00:10:05.732773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/options/options_controller.py
+-rw-r--r--   0        0        0    10665 2023-04-15 00:10:05.732773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/options/options_sdk_helper.py
+-rw-r--r--   0        0        0    14169 2023-04-15 00:10:05.732773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/options/options_view.py
+-rw-r--r--   0        0        0        0 2023-04-15 00:10:05.732773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/options/screen/__init__.py
+-rw-r--r--   0        0        0     5686 2023-04-15 00:10:05.732773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/options/screen/screener_controller.py
+-rw-r--r--   0        0        0     9556 2023-04-15 00:10:05.732773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/options/screen/syncretism_model.py
+-rw-r--r--   0        0        0     5580 2023-04-15 00:10:05.732773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/options/screen/syncretism_view.py
+-rw-r--r--   0        0        0     8295 2023-04-15 00:10:05.732773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/options/tradier_model.py
+-rw-r--r--   0        0        0     2561 2023-04-15 00:10:05.732773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/options/tradier_view.py
+-rw-r--r--   0        0        0     7674 2023-04-15 00:10:05.732773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/options/yfinance_model.py
+-rw-r--r--   0        0        0    11615 2023-04-15 00:10:05.732773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/options/yfinance_view.py
+-rw-r--r--   0        0        0        0 2023-04-15 00:10:05.732773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/quantitative_analysis/__init__.py
+-rw-r--r--   0        0        0     2260 2023-04-15 00:10:05.732773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/quantitative_analysis/beta_model.py
+-rw-r--r--   0        0        0     2798 2023-04-15 00:10:05.732773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/quantitative_analysis/beta_view.py
+-rw-r--r--   0        0        0     3187 2023-04-15 00:10:05.732773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/quantitative_analysis/factors_model.py
+-rw-r--r--   0        0        0      687 2023-04-15 00:10:05.732773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/quantitative_analysis/factors_view.py
+-rw-r--r--   0        0        0    38741 2023-04-15 00:10:05.732773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/quantitative_analysis/qa_controller.py
+-rw-r--r--   0        0        0      447 2023-04-15 00:10:05.732773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/quantitative_analysis/qa_model.py
+-rw-r--r--   0        0        0        0 2023-04-15 00:10:05.732773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/research/__init__.py
+-rw-r--r--   0        0        0     6218 2023-04-15 00:10:05.732773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/research/res_controller.py
+-rw-r--r--   0        0        0        0 2023-04-15 00:10:05.732773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/screener/__init__.py
+-rw-r--r--   0        0        0    46491 2023-04-15 00:10:05.732773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/screener/finviz_model.py
+-rw-r--r--   0        0        0     6981 2023-04-15 00:10:05.732773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/screener/finviz_view.py
+-rw-r--r--   0        0        0    21493 2023-04-15 00:10:05.732773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/screener/screener_controller.py
+-rw-r--r--   0        0        0      944 2023-04-15 00:10:05.732773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/screener/screener_helper.py
+-rw-r--r--   0        0        0     2562 2023-04-15 00:10:05.732773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/screener/screener_view.py
+-rw-r--r--   0        0        0    27077 2023-04-15 00:10:05.732773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/stock_statics.py
+-rw-r--r--   0        0        0    27380 2023-04-15 00:10:05.732773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/stocks_controller.py
+-rw-r--r--   0        0        0    33043 2023-04-15 00:10:05.732773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/stocks_helper.py
+-rw-r--r--   0        0        0    10576 2023-04-15 00:10:05.732773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/stocks_model.py
+-rw-r--r--   0        0        0     1241 2023-04-15 00:10:05.732773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/stocks_view.py
+-rw-r--r--   0        0        0        0 2023-04-15 00:10:05.732773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/technical_analysis/__init__.py
+-rw-r--r--   0        0        0     1004 2023-04-15 00:10:05.736773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/technical_analysis/finbrain_model.py
+-rw-r--r--   0        0        0      644 2023-04-15 00:10:05.736773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/technical_analysis/finbrain_view.py
+-rw-r--r--   0        0        0     1532 2023-04-15 00:10:05.736773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/technical_analysis/rsp_model.py
+-rw-r--r--   0        0        0     2386 2023-04-15 00:10:05.736773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/technical_analysis/rsp_view.py
+-rw-r--r--   0        0        0    62667 2023-04-15 00:10:05.736773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/technical_analysis/ta_controller.py
+-rw-r--r--   0        0        0     3260 2023-04-15 00:10:05.736773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/technical_analysis/tradingview_model.py
+-rw-r--r--   0        0        0     1985 2023-04-15 00:10:05.736773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/technical_analysis/tradingview_view.py
+-rw-r--r--   0        0        0      334 2023-04-15 00:10:05.736773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/tradinghours/README.md
+-rw-r--r--   0        0        0        0 2023-04-15 00:10:05.736773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/tradinghours/__init__.py
+-rw-r--r--   0        0        0     5328 2023-04-15 00:10:05.736773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/tradinghours/bursa_model.py
+-rw-r--r--   0        0        0     2202 2023-04-15 00:10:05.736773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/tradinghours/bursa_view.py
+-rw-r--r--   0        0        0        0 2023-04-15 00:10:05.736773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/tradinghours/data/__init__.py
+-rw-r--r--   0        0        0    28098 2023-04-15 00:10:05.736773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/tradinghours/data/bursa_open_hours.json
+-rw-r--r--   0        0        0     1466 2023-04-15 00:10:05.736773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/tradinghours/pandas_market_cal_model.py
+-rw-r--r--   0        0        0     1378 2023-04-15 00:10:05.736773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/tradinghours/pandas_market_cal_view.py
+-rw-r--r--   0        0        0    10137 2023-04-15 00:10:05.736773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/tradinghours/tradinghours_controller.py
+-rw-r--r--   0        0        0      614 2023-04-15 00:10:05.736773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/tradinghours/tradinghours_helper.py
+-rw-r--r--   0        0        0    42279 2023-04-15 00:10:05.736773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/terminal_controller.py
+-rw-r--r--   0        0        0    14413 2023-04-15 00:10:05.736773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/terminal_helper.py
+-rw-r--r--   0        0        0     3848 2023-04-15 00:10:05.736773 openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/thought_of_the_day.py
+-rw-r--r--   0        0        0     5771 2023-04-15 00:10:07.460809 openbb_nightly-3.0.0rc2.dev20230415/pyproject.toml
+-rw-r--r--   0        0        0     1137 2023-04-15 00:10:05.740773 openbb_nightly-3.0.0rc2.dev20230415/terminal.py
+-rw-r--r--   0        0        0     2285 2023-04-15 00:10:07.460809 openbb_nightly-3.0.0rc2.dev20230415/website/pypi.md
+-rw-r--r--   0        0        0     7768 1970-01-01 00:00:00.000000 openbb_nightly-3.0.0rc2.dev20230415/PKG-INFO
```

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/LICENSE` & `openbb_nightly-3.0.0rc2.dev20230415/LICENSE`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/SDK_README.md` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/SDK_README.md`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/account/account_controller.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/account/account_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/account/account_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/account/account_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/alternative/alt_controller.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/alternative/alt_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/alternative/covid/countries.txt` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/alternative/covid/countries.txt`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/alternative/covid/covid_controller.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/alternative/covid/covid_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/alternative/covid/covid_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/alternative/covid/covid_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/alternative/covid/covid_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/alternative/covid/covid_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/alternative/hackernews_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/alternative/hackernews_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/alternative/hackernews_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/alternative/hackernews_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/alternative/oss/github_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/alternative/oss/github_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/alternative/oss/github_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/alternative/oss/github_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/alternative/oss/oss_controller.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/alternative/oss/oss_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/alternative/oss/runa_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/alternative/oss/runa_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/alternative/oss/runa_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/alternative/oss/runa_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/alternative/realestate/landRegistry_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/alternative/realestate/landRegistry_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/alternative/realestate/landRegistry_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/alternative/realestate/landRegistry_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/alternative/realestate/realestate_controller.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/alternative/realestate/realestate_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/base_helpers.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/base_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/common/behavioural_analysis/finbrain_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/common/behavioural_analysis/finbrain_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/common/behavioural_analysis/finbrain_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/common/behavioural_analysis/finbrain_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/common/behavioural_analysis/finnhub_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/common/behavioural_analysis/finnhub_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/common/behavioural_analysis/finnhub_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/common/behavioural_analysis/finnhub_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/common/behavioural_analysis/google_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/common/behavioural_analysis/google_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/common/behavioural_analysis/google_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/common/behavioural_analysis/google_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/common/behavioural_analysis/reddit_helpers.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/common/behavioural_analysis/reddit_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/common/behavioural_analysis/reddit_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/common/behavioural_analysis/reddit_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/common/behavioural_analysis/reddit_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/common/behavioural_analysis/reddit_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/common/behavioural_analysis/stocktwits_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/common/behavioural_analysis/stocktwits_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/common/behavioural_analysis/stocktwits_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/common/behavioural_analysis/stocktwits_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/common/behavioural_analysis/twitter_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/common/behavioural_analysis/twitter_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/common/behavioural_analysis/twitter_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/common/behavioural_analysis/twitter_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/common/common_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/common/common_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/common/feedparser_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/common/feedparser_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/common/feedparser_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/common/feedparser_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/common/newsapi_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/common/newsapi_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/common/newsapi_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/common/newsapi_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/common/quantitative_analysis/qa_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/common/quantitative_analysis/qa_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/common/quantitative_analysis/qa_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/common/quantitative_analysis/qa_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/common/quantitative_analysis/rolling_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/common/quantitative_analysis/rolling_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/common/quantitative_analysis/rolling_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/common/quantitative_analysis/rolling_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/common/technical_analysis/custom_indicators_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/common/technical_analysis/custom_indicators_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/common/technical_analysis/custom_indicators_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/common/technical_analysis/custom_indicators_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/common/technical_analysis/momentum_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/common/technical_analysis/momentum_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/common/technical_analysis/momentum_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/common/technical_analysis/momentum_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/common/technical_analysis/overlap_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/common/technical_analysis/overlap_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/common/technical_analysis/overlap_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/common/technical_analysis/overlap_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/common/technical_analysis/ta_helpers.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/common/technical_analysis/ta_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/common/technical_analysis/trend_indicators_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/common/technical_analysis/trend_indicators_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/common/technical_analysis/trend_indicators_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/common/technical_analysis/trend_indicators_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/common/technical_analysis/volatility_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/common/technical_analysis/volatility_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/common/technical_analysis/volatility_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/common/technical_analysis/volatility_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/common/technical_analysis/volume_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/common/technical_analysis/volume_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/common/technical_analysis/volume_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/common/technical_analysis/volume_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/common/ultima_newsmonitor_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/common/ultima_newsmonitor_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/common/ultima_newsmonitor_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/common/ultima_newsmonitor_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/config_terminal.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/config_terminal.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/completer/choices.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/completer/choices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/config/paths.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/config/paths.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/config/paths_helper.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/config/paths_helper.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/integration_tests/README.md` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/integration_tests/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -156,24 +156,43 @@
 
 - To save time, the tests are run in parallel by default. You can choose the number of subprocesses used with `--subproc`. The default number of subprocesses is the minimum between the number of scripts to run and the number of CPUs of your machine.
 
     ```zsh
     python terminal.py -t forex --subproc 4
     ```
 
+- To have a more responsive console output we run the tests in parallel and return the
+  output of each script as soon as it is ready. This means that test results might not
+  be displayed in the same order as they were started. To force displaying tests results
+  in the order they start, use the option `--ordered`:
+
+    ```zsh
+    python terminal.py -t --ordered
+    ```
+
 - To see terminal outputs being printed during the test session, use `--verbose` or `-v`:
 
     ```zsh
     python terminal.py -t -v
     ```
 
-- In verbose mode the tests are run sequentially, by default. This avoids mixing the outputs from several scripts in the console. If you still want to see the outputs during a parallel run, just specify the number of subprocesses you wish to launch with verbose flag, it will force multiprocessing.
+- To run the tests sequentially (it will be way slower for a large number of scripts),
+  use `--subproc 0`:
+
+    ```zsh
+    python terminal.py -t --subproc 0
+    ```
+
+- Enabling verbose mode and running scripts in several processes will mix the output
+  each script in the console. In this case it is advisable to run tests with the option
+  `--subproc 0`, this will run the tests sequentially. It will be slower, but the outputs
+  of each test will not be mixed up.
 
     ```zsh
-    python terminal.py -t forex --subproc 7 -v
+    python terminal.py -t forex --subproc 0 -v
     ```
 
 ### Installer Terminal
 
 Integration tests can also be used on installers, which is a packaged version of the conda terminal.
 More information on how to build an installer can be found [here](/build/README.md).
 To run the tests on installers you can use the same syntax as above, just substitute `python terminal.py` by the full path to OpenBBTerminal executable (not the shortcut!). See the examples below for MacOS.
@@ -259,13 +278,13 @@
     getattr(
   File "/Users/username/OpenBBTerminal/openbb_terminal/decorators.py", line 64, in wrapper
     value = func(*args, **kwargs)
   File "/Users/username/OpenBBTerminal/openbb_terminal/forex/forex_controller.py", line 434, in call_qa
     1 / 0
 Exception type: ZeroDivisionError
 Detail: division by zero
-- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - 
+- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 
 ================================ integration test summary ================================
 FAILED forex/test_forex_qa.openbb -> command: qa
 ============================== 1 failed, 6 passed in 8.88s ===============================
 ```
```

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/integration_tests/integration_controller.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/integration_tests/integration_controller.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,16 +15,29 @@
 from traceback import FrameSummary, extract_tb, format_list
 from typing import Any, Callable, Dict, List, Optional, Tuple
 
 from openbb_terminal.core.config.paths import (
     MISCELLANEOUS_DIRECTORY,
     REPOSITORY_DIRECTORY,
 )
-from openbb_terminal.core.session.current_system import set_system_variable
+from openbb_terminal.core.models import (
+    CredentialsModel,
+    PreferencesModel,
+    ProfileModel,
+    SourcesModel,
+    SystemModel,
+    UserModel,
+)
+from openbb_terminal.core.session.current_system import (
+    get_current_system,
+    set_current_system,
+    set_system_variable,
+)
 from openbb_terminal.core.session.current_user import get_current_user, set_current_user
+from openbb_terminal.core.session.utils import load_dict_to_model
 from openbb_terminal.helper_funcs import check_non_negative
 from openbb_terminal.rich_config import console
 from openbb_terminal.terminal_controller import (
     insert_start_slash,
     replace_dynamic,
     terminal,
 )
@@ -273,14 +286,16 @@
                 terminal(file_cmds, test_mode=True)
 
 
 def run_test(
     file: Path,
     verbose: bool = False,
     special_arguments: Optional[Dict[str, str]] = None,
+    user: Optional[Dict] = None,
+    system: Optional[Dict] = None,
 ) -> Tuple[str, Optional[Dict[str, Any]]]:
     """Run tests in a single process.
 
     Parameters
     ----------
     file: Path
         The path to the file to test
@@ -290,14 +305,31 @@
         Replace `${key=default}` with `value` for every key in the dictionary
 
     Returns
     -------
     Tuple[str, Optional[Dict[str, Any]]]
         The name of the file and the exception
     """
+
+    if user:
+        profile = user.get("profile", {})
+        credentials = user.get("credentials", {})
+        preferences = user.get("preferences", {})
+        sources = user.get("sources", {})
+        user_model = UserModel(
+            profile=load_dict_to_model(profile, ProfileModel),
+            credentials=load_dict_to_model(credentials, CredentialsModel),  # type: ignore
+            preferences=load_dict_to_model(preferences, PreferencesModel),
+            sources=load_dict_to_model(sources, SourcesModel),
+        )
+        set_current_user(user_model)
+
+    if system:
+        set_current_system(load_dict_to_model(system, SystemModel))
+
     file_short_name = str(file).replace(str(SCRIPTS_DIRECTORY), "")[1:]
 
     try:
         run_scripts(
             file,
             verbose=verbose,
             special_arguments=special_arguments,
@@ -417,14 +449,20 @@
 
                 for i, result in enumerate(
                     runner(
                         partial(
                             run_test,
                             verbose=verbose,
                             special_arguments=special_arguments,
+                            # We inject user and system as dict because pickle cannot
+                            # serialize nested classes and the new process has to be
+                            # aware of the current user and system, otherwise it will
+                            # pick the defaults.
+                            user=get_current_user().to_dict(),
+                            system=get_current_system().to_dict(),
                         ),
                         test_files,
                         chunksize=chunksize,
                     )
                 ):
                     file_short_name, exception = result
                     if exception:
@@ -652,15 +690,15 @@
         dest="list_",
         action="store_true",
         default=False,
     )
     parser.add_argument(
         "-o",
         "--ordered",
-        help="Multiprocessing is not ordered by default. Use this flag to run the tests in order.",
+        help="Display results in test starting order.",
         dest="ordered",
         action="store_true",
         default=False,
     )
     for arg in special_arguments_values:
         parser.add_argument(
             f"--{arg}",
@@ -675,19 +713,20 @@
     # Allow the tester to send a path without the -p flag
     if not ns_parser.path and unknown_args:
         ns_parser.path = [u for u in unknown_args if u[0] != "-"]
 
     special_args_dict = {x: getattr(ns_parser, x) for x in special_arguments_values}
 
     if ns_parser.verbose and (
-        ns_parser.subprocesses is None or ns_parser.subprocesses > 0
+        ns_parser.subprocesses is None or ns_parser.subprocesses > 1
     ):
         console.print(
             "WARNING: verbose mode and multiprocessing are not compatible. "
-            "The output of the scripts is mixed up. Consider running with --subproc 0.\n",
+            "Several processes running simultaneously will mix the output of the "
+            "scripts in the screen. Consider running with --subproc 0.\n",
             style="yellow",
         )
 
     if ns_parser.list_:
         return display_available_scripts(ns_parser.path, ns_parser.skip)
 
     run_test_session(
@@ -710,17 +749,20 @@
 
     # user
     current_user = get_current_user()
     current_user.preferences.ENABLE_EXIT_AUTO_HELP = False
     current_user.preferences.USE_ION = True
     current_user.preferences.USE_PROMPT_TOOLKIT = False
     current_user.preferences.REMEMBER_CONTEXTS = False
+    current_user.preferences.PLOT_ENABLE_PYWRY = False
+    current_user.preferences.USE_INTERACTIVE_DF = False
     set_current_user(current_user)
 
     # system
+    set_system_variable("HEADLESS", True)
     set_system_variable("DEBUG_MODE", True)
     set_system_variable("LOG_COLLECT", False)
 
     # run integration tests
     parse_args_and_run()
```

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/log/collection/log_sender.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/log/collection/log_sender.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/log/collection/logging_clock.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/log/collection/logging_clock.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/log/collection/s3_sender.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/log/collection/s3_sender.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/log/generation/common.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/log/generation/common.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/log/generation/custom_logger.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/log/generation/custom_logger.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/log/generation/directories.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/log/generation/directories.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/log/generation/expired_files.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/log/generation/expired_files.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/log/generation/formatter_with_exceptions.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/log/generation/formatter_with_exceptions.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/log/generation/path_tracking_file_handler.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/log/generation/path_tracking_file_handler.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/log/generation/settings.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/log/generation/settings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/log/generation/settings_logger.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/log/generation/settings_logger.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/models/__init__.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/models/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/models/base_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/models/base_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/models/credentials_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/models/credentials_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/models/preferences_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/models/preferences_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,16 @@
     REQUEST_TIMEOUT: PositiveInt = 5
     MONITOR: NonNegativeInt = 0
 
     # STYLE
     MPL_STYLE: str = "dark"
     PMF_STYLE: str = "dark"
     RICH_STYLE: str = "dark"
-    THEME: Literal["dark", "light"] = "dark"
+    CHART_STYLE: Literal["dark", "light"] = "dark"
+    TABLE_STYLE: Literal["dark", "light"] = "dark"
 
     # PATHS
     GUESS_EASTER_EGG_FILE: str = os.getcwd() + os.path.sep + "guess_game.json"
     USER_DATA_DIRECTORY = HOME_DIRECTORY / "OpenBBUserData"
     USER_DATA_SOURCES_FILE: str = str(USER_DATA_DIRECTORY / "sources" / "sources.json")
     USER_EXPORTS_DIRECTORY = USER_DATA_DIRECTORY / "exports"
     USER_CUSTOM_IMPORTS_DIRECTORY = USER_DATA_DIRECTORY / "custom_imports"
```

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/models/profile_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/models/profile_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/models/sources_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/models/sources_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/models/system_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/models/system_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,10 +46,11 @@
     DISABLE_FORECASTING_WARNING: bool = False
     DISABLE_OPTIMIZATION_WARNING: bool = False
 
     # Others
     TEST_MODE: bool = False
     DEBUG_MODE: bool = False
     ENABLE_AUTHENTICATION: bool = True
+    HEADLESS: bool = False
 
     def __repr__(self) -> str:  # pylint: disable=useless-super-delegation
         return super().__repr__()
```

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/models/user_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/models/user_model.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from pydantic.dataclasses import dataclass
 
+from openbb_terminal.core.models.base_model import BaseModel
 from openbb_terminal.core.models.credentials_model import CredentialsModel
 from openbb_terminal.core.models.preferences_model import PreferencesModel
 from openbb_terminal.core.models.profile_model import ProfileModel
 from openbb_terminal.core.models.sources_model import SourcesModel
 
 
 @dataclass(config=dict(validate_assignment=True, frozen=True))
-class UserModel:
+class UserModel(BaseModel):
     """Data model for user."""
 
     profile: ProfileModel
     credentials: CredentialsModel
     preferences: PreferencesModel
     sources: SourcesModel
```

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/plots/assets/Terminal_icon.png` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/plots/assets/Terminal_icon.png`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/plots/assets/icon.png` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/plots/assets/icon.png`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/plots/backend.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/plots/backend.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/plots/config/openbb_styles.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/plots/config/openbb_styles.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/plots/no_import.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/plots/no_import.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/plots/old_table.html` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/plots/old_table.html`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/plots/plotly.html` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/plots/plotly.html`

 * *Files 2% similar despite different names*

```diff
@@ -195,15 +195,15 @@
     <!-- Plotly Chart -->
     <script type="text/javascript">
       window.PlotlyConfig = { MathJaxConfig: "local" };
 
       var interval = setInterval(function () {
         // Waits for OpenBBMain and plotly_figure to be defined before
         // calling OpenBBMain to avoid errors
-        let cmd_src = "";
+        globals.cmd_src = "";
         if (typeof OpenBBMain != "undefined" && window.plotly_figure) {
           clearInterval(interval);
           const date = new Date();
           const formattedDate = new Intl.DateTimeFormat("en-GB", {
             dateStyle: "full",
             timeStyle: "long",
           })
@@ -233,15 +233,15 @@
 
                   let margin = window.plotly_figure.layout.margin;
                   globals.old_margin = { ...margin };
                   if (margin.t != undefined && margin.t > 40) {
                     margin.t = 40;
                   }
                   margin.l = 70;
-                  if (cmd_src == "/stocks/candle") {
+                  if (globals.cmd_src == "/stocks/candle") {
                     margin.r -= 40;
                   }
                 }
               }
             });
           }
 
@@ -259,15 +259,15 @@
 
           if (title.length > 50) {
             document.getElementById("title").style.fontSize = "12px";
           }
 
           let style = "font-size: 12px; font-weight: 400; color: gray;";
           document.getElementById("date").innerHTML =
-            formattedDate + `<br /><span style="${style}">${cmd_src}</span>`;
+            formattedDate + `<br /><span style="${style}">${globals.cmd_src}</span>`;
           document.getElementById("title").innerHTML = title;
 
           CHART_DIV = document.getElementById("openbb_chart");
           CSV_DIV = document.getElementById("popup_csv");
           TEXT_DIV = document.getElementById("popup_text");
           TITLE_DIV = document.getElementById("popup_title");
           DOWNLOAD_DIV = document.getElementById("popup_download");
```

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/plots/plotly_helper.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/plots/plotly_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """Chart and style helpers for Plotly."""
 # pylint: disable=C0302,R0902,W3301
 import json
-import os
 import textwrap
 from datetime import datetime
 from math import floor
 from pathlib import Path
 from typing import Any, Dict, List, Literal, Optional, Tuple, TypeVar, Union
 
 try:
@@ -105,15 +104,15 @@
                 self.console_style = self.load_json_style(json_path)
             else:
                 console.print("Error loading default.")
 
     def apply_style(self, style: Optional[str] = "") -> None:
         """Apply the style to the libraries."""
         if not style:
-            style = get_current_user().preferences.THEME
+            style = get_current_user().preferences.CHART_STYLE
 
         if style != self.plt_style:
             self.load_style(style)
 
         style = style.lower().replace("light", "white")  # type: ignore
 
         if self.plt_style and self.plotly_template:
@@ -240,15 +239,16 @@
         colors = self.plotly_template.get("layout", {}).get("colorway", PLT_COLORWAY)
         if reverse:
             colors.reverse()
         return colors
 
 
 theme = TerminalStyle(
-    get_current_user().preferences.THEME, get_current_user().preferences.RICH_STYLE
+    get_current_user().preferences.CHART_STYLE,
+    get_current_user().preferences.RICH_STYLE,
 )
 theme.apply_style()
 
 
 # pylint: disable=R0913
 class OpenBBFigure(go.Figure):
     """Custom Figure class for OpenBB Terminal.
@@ -1057,15 +1057,15 @@
             ),
         )
 
         if external or self._exported:
             return self  # type: ignore
 
         # We check if in headless mode to return the JSON
-        if strtobool(os.environ.get("HEADLESS", False)):
+        if strtobool(get_current_system().HEADLESS):
             return self.to_json()
 
         kwargs.update(config=dict(scrollZoom=True, displaylogo=False))
         if plots_backend().isatty:
             try:
                 # We check if we need to export the image
                 # This is done to avoid opening after exporting
@@ -1532,16 +1532,16 @@
 
     def _adjust_margins(self) -> None:
         """Adjust the margins of the figure."""
         if self._margin_adjusted:
             return
 
         margin_add = (
-            dict(l=80, r=60, b=105, t=40, pad=0)
-            if not self._has_secondary_y
+            dict(l=80, r=60, b=85, t=40, pad=0)
+            if not self._has_secondary_y or not self.has_subplots
             else dict(l=60, r=50, b=95, t=40, pad=0)
         )
 
         # We adjust margins
         if plots_backend().isatty:
             for key in ["l", "r", "b", "t", "pad"]:
                 if key in self.layout.margin and self.layout.margin[key] is not None:
```

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/plots/plotly_ta/base.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/plots/plotly_ta/base.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/plots/plotly_ta/data_classes.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/plots/plotly_ta/data_classes.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/plots/plotly_ta/plugins/custom_indicators_plugin.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/plots/plotly_ta/plugins/custom_indicators_plugin.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/plots/plotly_ta/plugins/momentum_plugin.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/plots/plotly_ta/plugins/momentum_plugin.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/plots/plotly_ta/plugins/overlap_plugin.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/plots/plotly_ta/plugins/overlap_plugin.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/plots/plotly_ta/plugins/trend_indicators_plugin.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/plots/plotly_ta/plugins/trend_indicators_plugin.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/plots/plotly_ta/plugins/volatility_plugin.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/plots/plotly_ta/plugins/volatility_plugin.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/plots/plotly_ta/plugins/volume_plugin.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/plots/plotly_ta/plugins/volume_plugin.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/plots/plotly_ta/ta_class.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/plots/plotly_ta/ta_class.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/plots/table.html` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/plots/table.html`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/plots/web/bar_menus.js` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/plots/web/bar_menus.js`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/plots/web/css/fonts/FiraCode-Regular.ttf` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/plots/web/css/fonts/FiraCode-Regular.ttf`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/plots/web/css/fonts/FiraCode-VF.ttf` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/plots/web/css/fonts/FiraCode-VF.ttf`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/plots/web/css/style.css` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/plots/web/css/style.css`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/plots/web/helpers.js` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/plots/web/helpers.js`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/plots/web/main.js` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/plots/web/main.js`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/plots/web/main_table.js` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/plots/web/main_table.js`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/plots/web/popups.js` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/plots/web/popups.js`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/scripts/sdk_audit.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/scripts/sdk_audit.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/sdk/controllers/alt_sdk_controller.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/sdk/controllers/alt_sdk_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/sdk/controllers/crypto_sdk_controller.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/sdk/controllers/crypto_sdk_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/sdk/controllers/etf_sdk_controller.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/sdk/controllers/etf_sdk_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/sdk/controllers/forex_sdk_controller.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/sdk/controllers/forex_sdk_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/sdk/controllers/portfolio_sdk_controller.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/sdk/controllers/portfolio_sdk_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/sdk/controllers/stocks_sdk_controller.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/sdk/controllers/stocks_sdk_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,14 +95,16 @@
         """Stocks Discovery Submodule
 
         Attributes:
             `active`: Get stocks ordered in descending order by intraday trade volume. [Source: Yahoo Finance]\n
             `arkord`: Returns ARK orders in a Dataframe\n
             `asc`: Get Yahoo Finance small cap stocks with earnings growth rates better than 25%.\n
             `dividends`: Gets dividend calendar for given date.  Date represents Ex-Dividend Date\n
+            `filings`: Get SEC Filings RSS feed, disseminated by FMP\n
+            `filings_chart`: Display recent forms submitted to the SEC\n
             `fipo`: Future IPOs dates. [Source: Finnhub]\n
             `gainers`: Get top gainers. [Source: Yahoo Finance]\n
             `gtech`: Get technology stocks with revenue and earnings growth in excess of 25%. [Source: Yahoo Finance]\n
             `hotpenny`: Returns today hot penny stocks\n
             `ipo`: Get IPO calendar\n
             `losers`: Get top losers. [Source: Yahoo Finance]\n
             `lowfloat`: Returns low float DataFrame\n
@@ -319,16 +321,14 @@
         Attributes:
             `recom`: Get tradingview recommendation based on technical indicators\n
             `recom_chart`: Print tradingview recommendation based on technical indicators\n
             `rsp`: Relative strength percentile [Source: https://github.com/skyte/relative-strength]\n
             `rsp_chart`: Display Relative Strength Percentile [Source: https://github.com/skyte/relative-strength]\n
             `summary`: Get technical summary report provided by FinBrain's API\n
             `summary_chart`: Print technical summary report provided by FinBrain's API\n
-            `view`: Get finviz image for given ticker\n
-            `view_chart`: View finviz image for ticker\n
         """
 
         return model.StocksTechnicalAnalysis()
 
     @property
     def th(self):
         """Stocks Trading Hours Submodule
```

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/sdk/models/__init__.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/sdk/models/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/sdk/models/alt_sdk_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/sdk/models/alt_sdk_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/sdk/models/crypto_sdk_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/sdk/models/crypto_sdk_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/sdk/models/econometrics_sdk_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/sdk/models/econometrics_sdk_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/sdk/models/economy_sdk_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/sdk/models/economy_sdk_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,15 +47,14 @@
         `revenue`: Governments collect revenues mainly for two purposes: to finance the goods\n
         `revenue_chart`: Governments collect revenues mainly for two purposes: to finance the goods\n
         `rgdp`: Gross domestic product (GDP) is the standard measure of the value added\n
         `rgdp_chart`: Gross domestic product (GDP) is the standard measure of the value added\n
         `rtps`: Get real-time performance sector data\n
         `rtps_chart`: Display Real-Time Performance sector. [Source: AlphaVantage]\n
         `search_index`: Search indices by keyword. [Source: FinanceDatabase]\n
-        `spectrum`: Display finviz spectrum in system viewer [Source: Finviz]\n
         `spending`: General government spending provides an indication of the size\n
         `spending_chart`: General government spending provides an indication of the size\n
         `treasury`: Get U.S. Treasury rates [Source: EconDB]\n
         `treasury_chart`: Display U.S. Treasury rates [Source: EconDB]\n
         `treasury_maturities`: Get treasury maturity options [Source: EconDB]\n
         `trust`: Trust in government refers to the share of people who report having confidence in\n
         `trust_chart`: Trust in government refers to the share of people who report having confidence in\n
@@ -105,15 +104,14 @@
         self.revenue = lib.economy_oecd_model.get_revenue
         self.revenue_chart = lib.economy_oecd_view.plot_revenue
         self.rgdp = lib.economy_oecd_model.get_real_gdp
         self.rgdp_chart = lib.economy_oecd_view.plot_real_gdp
         self.rtps = lib.economy_alphavantage_model.get_sector_data
         self.rtps_chart = lib.economy_alphavantage_view.realtime_performance_sector
         self.search_index = lib.economy_yfinance_model.get_search_indices
-        self.spectrum = lib.economy_finviz_view.display_spectrum
         self.spending = lib.economy_oecd_model.get_spending
         self.spending_chart = lib.economy_oecd_view.plot_spending
         self.treasury = lib.economy_econdb_model.get_treasuries
         self.treasury_chart = lib.economy_econdb_view.show_treasuries
         self.treasury_maturities = lib.economy_econdb_model.get_treasury_maturities
         self.trust = lib.economy_oecd_model.get_trust
         self.trust_chart = lib.economy_oecd_view.plot_trust
```

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/sdk/models/etf_sdk_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/sdk/models/etf_sdk_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/sdk/models/fixedincome_sdk_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/sdk/models/fixedincome_sdk_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/sdk/models/forecast_sdk_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/sdk/models/forecast_sdk_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/sdk/models/forex_sdk_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/sdk/models/forex_sdk_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/sdk/models/funds_sdk_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/sdk/models/funds_sdk_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/sdk/models/futures_sdk_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/sdk/models/futures_sdk_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/sdk/models/keys_sdk_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/sdk/models/keys_sdk_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/sdk/models/portfolio_sdk_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/sdk/models/portfolio_sdk_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/sdk/models/qa_sdk_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/sdk/models/qa_sdk_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/sdk/models/stocks_sdk_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/sdk/models/stocks_sdk_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,14 +143,16 @@
     """Discovery Module.
 
     Attributes:
         `active`: Get stocks ordered in descending order by intraday trade volume. [Source: Yahoo Finance]\n
         `arkord`: Returns ARK orders in a Dataframe\n
         `asc`: Get Yahoo Finance small cap stocks with earnings growth rates better than 25%.\n
         `dividends`: Gets dividend calendar for given date.  Date represents Ex-Dividend Date\n
+        `filings`: Get SEC Filings RSS feed, disseminated by FMP\n
+        `filings_chart`: Display recent forms submitted to the SEC\n
         `fipo`: Future IPOs dates. [Source: Finnhub]\n
         `gainers`: Get top gainers. [Source: Yahoo Finance]\n
         `gtech`: Get technology stocks with revenue and earnings growth in excess of 25%. [Source: Yahoo Finance]\n
         `hotpenny`: Returns today hot penny stocks\n
         `ipo`: Get IPO calendar\n
         `losers`: Get top losers. [Source: Yahoo Finance]\n
         `lowfloat`: Returns low float DataFrame\n
@@ -167,14 +169,16 @@
 
     def __init__(self):
         super().__init__()
         self.active = lib.stocks_disc_yahoofinance_model.get_active
         self.arkord = lib.stocks_disc_ark_model.get_ark_orders
         self.asc = lib.stocks_disc_yahoofinance_model.get_asc
         self.dividends = lib.stocks_disc_nasdaq_model.get_dividend_cal
+        self.filings = lib.stocks_fa_fmp_model.get_filings
+        self.filings_chart = lib.stocks_disc_fmp_view.display_filings
         self.fipo = lib.stocks_disc_finnhub_model.get_future_ipo
         self.gainers = lib.stocks_disc_yahoofinance_model.get_gainers
         self.gtech = lib.stocks_disc_yahoofinance_model.get_gtech
         self.hotpenny = lib.stocks_disc_shortinterest_model.get_today_hot_penny_stocks
         self.ipo = lib.stocks_disc_finnhub_model.get_ipo_calendar
         self.losers = lib.stocks_disc_yahoofinance_model.get_losers
         self.lowfloat = lib.stocks_disc_shortinterest_model.get_low_float
@@ -550,30 +554,26 @@
     Attributes:
         `recom`: Get tradingview recommendation based on technical indicators\n
         `recom_chart`: Print tradingview recommendation based on technical indicators\n
         `rsp`: Relative strength percentile [Source: https://github.com/skyte/relative-strength]\n
         `rsp_chart`: Display Relative Strength Percentile [Source: https://github.com/skyte/relative-strength]\n
         `summary`: Get technical summary report provided by FinBrain's API\n
         `summary_chart`: Print technical summary report provided by FinBrain's API\n
-        `view`: Get finviz image for given ticker\n
-        `view_chart`: View finviz image for ticker\n
     """
 
     _location_path = "stocks.ta"
 
     def __init__(self):
         super().__init__()
         self.recom = lib.stocks_ta_tradingview_model.get_tradingview_recommendation
         self.recom_chart = lib.stocks_ta_tradingview_view.print_recommendation
         self.rsp = lib.stocks_ta_rsp_model.get_rsp
         self.rsp_chart = lib.stocks_ta_rsp_view.display_rsp
         self.summary = lib.stocks_ta_finbrain_model.get_technical_summary_report
         self.summary_chart = lib.stocks_ta_finbrain_view.technical_summary_report
-        self.view = lib.stocks_ta_finviz_model.get_finviz_image
-        self.view_chart = lib.stocks_ta_finviz_view.view
 
 
 class StocksTradingHours(Category):
     """Trading Hours Module.
 
     Attributes:
         `all`: Get all exchanges.\n
```

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/sdk/models/ta_sdk_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/sdk/models/ta_sdk_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/sdk/sdk_helpers.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/sdk/sdk_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/sdk/sdk_init.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/sdk/sdk_init.py`

 * *Files 0% similar despite different names*

```diff
@@ -318,14 +318,15 @@
     yahoofinance_model as stocks_dps_yahoofinance_model,
 )
 
 # Stocks - Fundamental Discovery
 from openbb_terminal.stocks.discovery import (
     ark_model as stocks_disc_ark_model,
     finnhub_model as stocks_disc_finnhub_model,
+    fmp_view as stocks_disc_fmp_view,
     nasdaq_model as stocks_disc_nasdaq_model,
     seeking_alpha_model as stocks_disc_seeking_alpha_model,
     shortinterest_model as stocks_disc_shortinterest_model,
     yahoofinance_model as stocks_disc_yahoofinance_model,
 )
 
 # Stocks - Fundamental Analysis
@@ -402,16 +403,14 @@
     finviz_view as stocks_screener_finviz_view,
 )
 
 # Stocks - Technical Analysis
 from openbb_terminal.stocks.technical_analysis import (
     finbrain_model as stocks_ta_finbrain_model,
     finbrain_view as stocks_ta_finbrain_view,
-    finviz_model as stocks_ta_finviz_model,
-    finviz_view as stocks_ta_finviz_view,
     rsp_model as stocks_ta_rsp_model,
     rsp_view as stocks_ta_rsp_view,
     tradingview_model as stocks_ta_tradingview_model,
     tradingview_view as stocks_ta_tradingview_view,
 )
 
 # Stocks - Trading Hours
```

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/sdk/trail_map.csv` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/sdk/trail_map.csv`

 * *Files 1% similar despite different names*

```diff
@@ -203,15 +203,14 @@
 economy.overview,economy_wsj_model.market_overview,
 economy.perfmap,economy_finviz_model.get_performance_map,
 economy.performance,economy_finviz_model.get_performance_data,
 economy.revenue,economy_oecd_model.get_revenue,economy_oecd_view.plot_revenue
 economy.rgdp,economy_oecd_model.get_real_gdp,economy_oecd_view.plot_real_gdp
 economy.rtps,economy_alphavantage_model.get_sector_data,economy_alphavantage_view.realtime_performance_sector
 economy.search_index,economy_yfinance_model.get_search_indices,
-economy.spectrum,economy_finviz_view.display_spectrum,
 economy.spending,economy_oecd_model.get_spending,economy_oecd_view.plot_spending
 economy.treasury,economy_econdb_model.get_treasuries,economy_econdb_view.show_treasuries
 economy.treasury_maturities,economy_econdb_model.get_treasury_maturities,
 economy.trust,economy_oecd_model.get_trust,economy_oecd_view.plot_trust
 economy.usbonds,economy_wsj_model.us_bonds,
 economy.valuation,economy_finviz_model.get_valuation_data,
 etf.candle,stocks_helper.display_candle,
@@ -407,14 +406,15 @@
 stocks.ca.similar,stocks_ca_sdk_helpers.get_similar,
 stocks.ca.volume,stocks_ca_yahoo_finance_model.get_volume,stocks_ca_yahoo_finance_view.display_volume
 stocks.candle,stocks_helper.display_candle,
 stocks.disc.active,stocks_disc_yahoofinance_model.get_active,
 stocks.disc.arkord,stocks_disc_ark_model.get_ark_orders,
 stocks.disc.asc,stocks_disc_yahoofinance_model.get_asc,
 stocks.disc.dividends,stocks_disc_nasdaq_model.get_dividend_cal,
+stocks.disc.filings,stocks_fa_fmp_model.get_filings,stocks_disc_fmp_view.display_filings
 stocks.disc.fipo,stocks_disc_finnhub_model.get_future_ipo,
 stocks.disc.gainers,stocks_disc_yahoofinance_model.get_gainers,
 stocks.disc.gtech,stocks_disc_yahoofinance_model.get_gtech,
 stocks.disc.hotpenny,stocks_disc_shortinterest_model.get_today_hot_penny_stocks,
 stocks.disc.ipo,stocks_disc_finnhub_model.get_ipo_calendar,
 stocks.disc.losers,stocks_disc_yahoofinance_model.get_losers,
 stocks.disc.lowfloat,stocks_disc_shortinterest_model.get_low_float,
@@ -531,15 +531,14 @@
 stocks.qa.historical_5,stocks_qa_factors_model.get_historical_5,
 stocks.quote,stocks_model.get_quote,
 stocks.screener.screener_data,stocks_screener_finviz_model.get_screener_data,stocks_screener_finviz_view.screener
 stocks.search,stocks_helper.search,
 stocks.ta.recom,stocks_ta_tradingview_model.get_tradingview_recommendation,stocks_ta_tradingview_view.print_recommendation
 stocks.ta.rsp,stocks_ta_rsp_model.get_rsp,stocks_ta_rsp_view.display_rsp
 stocks.ta.summary,stocks_ta_finbrain_model.get_technical_summary_report,stocks_ta_finbrain_view.technical_summary_report
-stocks.ta.view,stocks_ta_finviz_model.get_finviz_image,stocks_ta_finviz_view.view
 stocks.th.all,stocks_th_bursa_model.get_all,stocks_th_bursa_view.display_all
 stocks.th.check_if_open,stocks_th_bursa_model.check_if_open,
 stocks.th.closed,stocks_th_bursa_model.get_closed,stocks_th_bursa_view.display_closed
 stocks.th.exchange,stocks_th_bursa_model.get_bursa,stocks_th_bursa_view.display_exchange
 stocks.th.open,stocks_th_bursa_model.get_open,stocks_th_bursa_view.display_open
 stocks.tob,stocks_cboe_model.get_top_of_book,
 ta.ad,common_ta_volume_model.ad,common_ta_volume_view.display_ad
```

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/sdk/trail_map_forecasting.csv` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/sdk/trail_map_forecasting.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/sdk/trail_map_optimization.csv` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/sdk/trail_map_optimization.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/sdk/trailmap.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/sdk/trailmap.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/session/banner.txt` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/session/banner.txt`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/session/constants.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/session/constants.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/session/current_system.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/session/current_system.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/session/current_user.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/session/current_user.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/session/env_handler.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/session/env_handler.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/session/hub_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/session/hub_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/session/local_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/session/local_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -104,19 +104,21 @@
     """Apply configurations.
 
     Parameters
     ----------
     configs : dict
         The configurations.
     """
-    # Saving the RICH_STYLE state allows user to change from hub rich style to local
+    # Saving the RICH_STYLE state allows user to change the default from 'hub' style to
+    # some custom .richstyle.json file
     set_credentials_from_hub(configs)
     set_preferences_from_hub(configs, fields=["RICH_STYLE"])
     set_rich_style_from_hub(configs)
-    set_chart_table_style_from_hub(configs)
+    set_chart_style_from_hub(configs)
+    set_table_style_from_hub(configs)
     set_sources_from_hub(configs)
 
 
 def set_credentials_from_hub(configs: dict):
     """Set credentials from hub.
 
     Parameters
@@ -178,28 +180,44 @@
                     if "RICH_STYLE" not in preferences:
                         set_preference("RICH_STYLE", "hub")
 
                 except Exception:
                     console.print("[red]Failed to set rich style.[/red]")
 
 
-def set_chart_table_style_from_hub(configs: dict):
-    """Set chart and table style from hub.
+def set_chart_style_from_hub(configs: dict):
+    """Set chart style from hub.
 
     Parameters
     ----------
     configs : dict
         The configurations.
     """
     if configs:
         terminal_style = configs.get("features_terminal_style", {}) or {}
         if terminal_style:
-            chart_table = terminal_style.get("chart_table", None)
-            if chart_table:
-                set_preference("THEME", chart_table)
+            chart_style = terminal_style.get("chart", None)
+            if chart_style:
+                set_preference("CHART_STYLE", chart_style)
+
+
+def set_table_style_from_hub(configs: dict):
+    """Set table style from hub.
+
+    Parameters
+    ----------
+    configs : dict
+        The configurations.
+    """
+    if configs:
+        terminal_style = configs.get("features_terminal_style", {}) or {}
+        if terminal_style:
+            table_style = terminal_style.get("table", None)
+            if table_style:
+                set_preference("TABLE_STYLE", table_style)
 
 
 def set_sources_from_hub(configs: dict):
     """Set sources from hub.
 
     Parameters
     ----------
```

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/session/routines_handler.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/session/routines_handler.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/session/sdk_session.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/session/sdk_session.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/session/session_controller.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/session/session_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/session/session_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/session/session_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/session/sources_handler.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/session/sources_handler.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/session/utils.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/session/utils.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/core/sources/utils.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/core/sources/utils.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/coinbase_helpers.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/coinbase_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/coinpaprika_helpers.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/coinpaprika_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/crypto_controller.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/crypto_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/crypto_models.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/crypto_models.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/crypto_views.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/crypto_views.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/cryptocurrency_helpers.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/cryptocurrency_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/data/README.md` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/data/README.md`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/data/binance_gecko_map.json` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/data/binance_gecko_map.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/data/coinbase_gecko_map.json` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/data/coinbase_gecko_map.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/data/coingecko_categories.json` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/data/coingecko_categories.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/data/coingecko_coins.json` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/data/coingecko_coins.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/data/coinpaprika_coins.json` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/data/coinpaprika_coins.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/data/defillama_dapps.json` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/data/defillama_dapps.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/data/erc20_coins.json` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/data/erc20_coins.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/data/finbrain_coins.json` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/data/finbrain_coins.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/data/santiment_slugs.json` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/data/santiment_slugs.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/data/yahoofinance_coins.json` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/data/yahoofinance_coins.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/dataframe_helpers.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/dataframe_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/defi/coindix_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/defi/coindix_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/defi/coindix_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/defi/coindix_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/defi/cryptosaurio_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/defi/cryptosaurio_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/defi/cryptosaurio_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/defi/cryptosaurio_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/defi/defi_controller.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/defi/defi_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/defi/graph_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/defi/graph_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/defi/graph_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/defi/graph_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/defi/llama_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/defi/llama_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/defi/llama_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/defi/llama_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/defi/smartstake_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/defi/smartstake_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/defi/smartstake_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/defi/smartstake_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/defi/substack_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/defi/substack_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/defi/substack_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/defi/substack_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/defi/terraengineer_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/defi/terraengineer_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/defi/terraengineer_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/defi/terraengineer_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/defi/terramoney_fcd_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/defi/terramoney_fcd_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/defi/terramoney_fcd_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/defi/terramoney_fcd_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/discovery/coinmarketcap_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/discovery/coinmarketcap_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/discovery/coinmarketcap_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/discovery/coinmarketcap_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/discovery/coinpaprika_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/discovery/coinpaprika_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/discovery/coinpaprika_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/discovery/coinpaprika_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/discovery/dappradar_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/discovery/dappradar_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/discovery/dappradar_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/discovery/dappradar_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/discovery/discovery_controller.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/discovery/discovery_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/discovery/pycoingecko_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/discovery/pycoingecko_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/discovery/pycoingecko_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/discovery/pycoingecko_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/discovery/sdk_helpers.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/discovery/sdk_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/due_diligence/binance_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/due_diligence/binance_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/due_diligence/binance_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/due_diligence/binance_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/due_diligence/ccxt_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/due_diligence/ccxt_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/due_diligence/ccxt_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/due_diligence/ccxt_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/due_diligence/coinbase_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/due_diligence/coinbase_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/due_diligence/coinbase_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/due_diligence/coinbase_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/due_diligence/coinglass_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/due_diligence/coinglass_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/due_diligence/coinglass_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/due_diligence/coinglass_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/due_diligence/coinpaprika_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/due_diligence/coinpaprika_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/due_diligence/coinpaprika_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/due_diligence/coinpaprika_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/due_diligence/cryptopanic_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/due_diligence/cryptopanic_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/due_diligence/dd_controller.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/due_diligence/dd_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/due_diligence/due_diligence_api.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/due_diligence/due_diligence_api.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/due_diligence/finbrain_crypto_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/due_diligence/finbrain_crypto_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/due_diligence/glassnode_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/due_diligence/glassnode_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/due_diligence/glassnode_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/due_diligence/glassnode_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/due_diligence/messari_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/due_diligence/messari_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/due_diligence/messari_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/due_diligence/messari_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/due_diligence/pycoingecko_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/due_diligence/pycoingecko_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/due_diligence/pycoingecko_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/due_diligence/pycoingecko_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/due_diligence/santiment_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/due_diligence/santiment_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/due_diligence/santiment_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/due_diligence/santiment_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/due_diligence/sdk_helper.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/due_diligence/sdk_helper.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/due_diligence/tokenterminal_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/due_diligence/tokenterminal_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/due_diligence/tokenterminal_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/due_diligence/tokenterminal_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/nft/nft_controller.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/nft/nft_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/nft/nftpricefloor_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/nft/nftpricefloor_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/nft/nftpricefloor_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/nft/nftpricefloor_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/nft/opensea_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/nft/opensea_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/nft/opensea_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/nft/opensea_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/onchain/bitquery_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/onchain/bitquery_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/onchain/bitquery_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/onchain/bitquery_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/onchain/blockchain_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/onchain/blockchain_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/onchain/blockchain_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/onchain/blockchain_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/onchain/ethgasstation_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/onchain/ethgasstation_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/onchain/ethgasstation_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/onchain/ethgasstation_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/onchain/ethplorer_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/onchain/ethplorer_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/onchain/ethplorer_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/onchain/ethplorer_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/onchain/onchain_controller.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/onchain/onchain_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/onchain/shroom_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/onchain/shroom_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/onchain/shroom_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/onchain/shroom_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/onchain/whale_alert_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/onchain/whale_alert_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/onchain/whale_alert_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/onchain/whale_alert_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/overview/blockchaincenter_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/overview/blockchaincenter_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/overview/blockchaincenter_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/overview/blockchaincenter_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/overview/coinbase_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/overview/coinbase_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/overview/coinbase_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/overview/coinbase_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/overview/coinpaprika_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/overview/coinpaprika_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/overview/coinpaprika_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/overview/coinpaprika_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/overview/cryptopanic_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/overview/cryptopanic_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/overview/cryptopanic_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/overview/cryptopanic_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/overview/glassnode_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/overview/glassnode_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/overview/glassnode_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/overview/glassnode_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/overview/loanscan_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/overview/loanscan_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/overview/loanscan_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/overview/loanscan_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/overview/overview_controller.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/overview/overview_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/overview/pycoingecko_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/overview/pycoingecko_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/overview/pycoingecko_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/overview/pycoingecko_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/overview/rekt_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/overview/rekt_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/overview/rekt_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/overview/rekt_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/overview/sdk_helpers.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/overview/sdk_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/overview/tokenterminal_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/overview/tokenterminal_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/overview/tokenterminal_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/overview/tokenterminal_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/overview/withdrawalfees_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/overview/withdrawalfees_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/overview/withdrawalfees_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/overview/withdrawalfees_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/pycoingecko_helpers.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/pycoingecko_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/pyth_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/pyth_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/pyth_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/pyth_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/quantitative_analysis/qa_controller.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/quantitative_analysis/qa_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/technical_analysis/ta_controller.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/technical_analysis/ta_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/tools/tools_controller.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/tools/tools_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/tools/tools_helpers.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/tools/tools_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/tools/tools_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/tools/tools_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/cryptocurrency/tools/tools_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/cryptocurrency/tools/tools_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/custom_prompt_toolkit.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/custom_prompt_toolkit.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/custom_reports/lunar_crash/coin_highs.png` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/custom_reports/lunar_crash/coin_highs.png`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/custom_reports/lunar_crash/luna_crash.html` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/custom_reports/lunar_crash/luna_crash.html`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/custom_reports/lunar_crash/luna_supply.png` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/custom_reports/lunar_crash/luna_supply.png`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/custom_reports/lunar_crash/luna_terra.png` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/custom_reports/lunar_crash/luna_terra.png`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/custom_reports/lunar_crash/lunatics.ipynb` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/custom_reports/lunar_crash/lunatics.ipynb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/custom_reports/lunar_crash/tvl.png` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/custom_reports/lunar_crash/tvl.png`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/custom_reports/lunar_crash/ust_terra.png` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/custom_reports/lunar_crash/ust_terra.png`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/dashboards/dashboards_controller.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/dashboards/dashboards_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/dashboards/stream/Forecasting.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/dashboards/stream/Forecasting.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/dashboards/stream/common_vars.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/dashboards/stream/common_vars.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/dashboards/stream/pages/Chains.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/dashboards/stream/pages/Chains.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/dashboards/stream/pages/Correlation.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/dashboards/stream/pages/Correlation.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/dashboards/stream/pages/Futures.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/dashboards/stream/pages/Futures.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/dashboards/stream/pages/Indicators.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/dashboards/stream/pages/Indicators.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/dashboards/stream/pages/Short_Data.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/dashboards/stream/pages/Short_Data.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/dashboards/stream/pages/Stocks.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/dashboards/stream/pages/Stocks.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/dashboards/stream/streamlit_helpers.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/dashboards/stream/streamlit_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/dashboards/streamlit.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/dashboards/streamlit.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/dashboards/voila/chains.ipynb` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/dashboards/voila/chains.ipynb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/dashboards/voila/correlation.ipynb` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/dashboards/voila/correlation.ipynb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/dashboards/voila/forecast.ipynb` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/dashboards/voila/forecast.ipynb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/dashboards/voila/futures.ipynb` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/dashboards/voila/futures.ipynb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/dashboards/voila/shortdata.ipynb` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/dashboards/voila/shortdata.ipynb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/dashboards/voila/stocks.ipynb` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/dashboards/voila/stocks.ipynb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/decorators.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/decorators.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/econometrics/econometrics_controller.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/econometrics/econometrics_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/econometrics/econometrics_helpers.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/econometrics/econometrics_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/econometrics/econometrics_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/econometrics/econometrics_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/econometrics/econometrics_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/econometrics/econometrics_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/econometrics/regression_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/econometrics/regression_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/econometrics/regression_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/econometrics/regression_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/economy/alphavantage_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/economy/alphavantage_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/economy/alphavantage_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/economy/alphavantage_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/economy/commodity_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/economy/commodity_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/economy/commodity_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/economy/commodity_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/economy/datasets/NASDAQ_CountryCodes.csv` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/economy/datasets/NASDAQ_CountryCodes.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/economy/datasets/cpi.csv` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/economy/datasets/cpi.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/economy/datasets/harmonized_cpi.csv` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/economy/datasets/harmonized_cpi.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/economy/econdb_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/economy/econdb_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/economy/econdb_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/economy/econdb_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/economy/economy_controller.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/economy/economy_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,14 @@
     plot_view,
     wsj_view,
     yfinance_model,
     yfinance_view,
 )
 from openbb_terminal.helper_funcs import (
     EXPORT_BOTH_RAW_DATA_AND_FIGURES,
-    EXPORT_ONLY_FIGURES_ALLOWED,
     EXPORT_ONLY_RAW_DATA_ALLOWED,
     list_from_str,
     parse_and_split_input,
     print_rich_table,
     valid_date,
 )
 from openbb_terminal.menu import session
@@ -73,15 +72,14 @@
         "macro",
         "fred",
         "index",
         "treasury",
         "plot",
         "valuation",
         "performance",
-        "spectrum",
         "map",
         "rtps",
         "bigmac",
         "events",
         "edebt",
     ]
 
@@ -316,15 +314,14 @@
         mt.add_cmd("bigmac")
         mt.add_cmd("events")
         mt.add_cmd("edebt")
         mt.add_raw("\n")
         mt.add_cmd("rtps")
         mt.add_cmd("valuation")
         mt.add_cmd("performance")
-        mt.add_cmd("spectrum")
         mt.add_raw("\n")
         mt.add_info("_country_")
         mt.add_cmd("gdp")
         mt.add_cmd("rgdp")
         mt.add_cmd("fgdp")
         mt.add_cmd("debt")
         mt.add_cmd("cpi")
@@ -2426,52 +2423,14 @@
                 sheet_name=" ".join(ns_parser.sheet_name)
                 if ns_parser.sheet_name
                 else None,
                 limit=ns_parser.limit,
             )
 
     @log_start_end(log=logger)
-    def call_spectrum(self, other_args: List[str]):
-        """Process spectrum command"""
-        parser = argparse.ArgumentParser(
-            add_help=False,
-            formatter_class=argparse.ArgumentDefaultsHelpFormatter,
-            prog="spectrum",
-            description="""
-                View group (sectors, industry or country) spectrum data. [Source: Finviz]
-            """,
-        )
-        parser.add_argument(
-            "-g",
-            "--group",
-            type=str,
-            choices=list(self.d_GROUPS.keys()),
-            default="sector",
-            dest="group",
-            help="Data group (sector, industry or country)",
-        )
-        if other_args and "-" not in other_args[0][0]:
-            other_args.insert(0, "-g")
-
-        ns_parser = self.parse_known_args_and_warn(
-            parser, other_args, export_allowed=EXPORT_ONLY_FIGURES_ALLOWED
-        )
-        if ns_parser:
-            ns_group = (
-                " ".join(ns_parser.group)
-                if isinstance(ns_parser.group, list)
-                else ns_parser.group
-            )
-            finviz_view.display_spectrum(group=ns_group)
-
-            # # Due to Finviz implementation of Spectrum, we delete the generated spectrum figure
-            # # after saving it and displaying it to the user
-            os.remove(self.d_GROUPS[ns_group] + ".jpg")
-
-    @log_start_end(log=logger)
     def call_eval(self, other_args):
         parser = argparse.ArgumentParser(
             add_help=False,
             formatter_class=argparse.ArgumentDefaultsHelpFormatter,
             prog="eval",
             description="""Create custom data column from loaded datasets.  Can be mathematical expressions supported
             by pandas.eval() function.
```

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/economy/economy_helpers.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/economy/economy_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/economy/finviz_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/economy/finviz_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/economy/finviz_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/economy/finviz_view.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 """ Finviz View """
 __docformat__ = "numpy"
 
 import logging
 import os
 from typing import Optional
 
-from PIL import Image
-
 from openbb_terminal.decorators import log_start_end
 from openbb_terminal.economy import finviz_model
 from openbb_terminal.helper_funcs import export_data, print_rich_table
 
 logger = logging.getLogger(__name__)
 
 
@@ -111,44 +109,14 @@
         "performance",
         df_group,
         sheet_name,
     )
 
 
 @log_start_end(log=logger)
-def display_spectrum(
-    group: str = "sector", export: str = "", sheet_name: Optional[str] = None
-):
-    """Display finviz spectrum in system viewer [Source: Finviz]
-
-    Parameters
-    ----------
-    group: str
-        Group by category. Available groups can be accessed through get_groups().
-    sheet_name: str
-        Optionally specify the name of the sheet the data is exported to.
-    export: str
-        Format to export data
-    """
-    finviz_model.get_spectrum_data(group)
-
-    group = finviz_model.GROUPS[group]
-    img = Image.open(group + ".jpg")
-
-    export_data(
-        export,
-        os.path.dirname(os.path.abspath(__file__)),
-        "spectrum",
-        sheet_name,
-    )
-
-    img.show()
-
-
-@log_start_end(log=logger)
 def display_future(
     future_type: str = "Indices",
     sortby: str = "ticker",
     ascend: bool = False,
     export: str = "",
     sheet_name: Optional[str] = None,
 ):
```

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/economy/fred_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/economy/fred_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/economy/fred_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/economy/fred_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/economy/nasdaq_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/economy/nasdaq_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/economy/nasdaq_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/economy/nasdaq_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/economy/oecd_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/economy/oecd_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/economy/oecd_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/economy/oecd_view.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,50 @@
 """ OECD view """
 __docformat__ = "numpy"
 
 # IMPORTATION STANDARD
 import logging
 import os
 from datetime import datetime
-from typing import List, Optional
-
-import pandas as pd
+from typing import Any, Dict, List, Optional, Union
 
 from openbb_terminal import OpenBBFigure
 from openbb_terminal.decorators import log_start_end
 from openbb_terminal.economy import oecd_model
 from openbb_terminal.helper_funcs import console, export_data, print_rich_table
 
 logger = logging.getLogger(__name__)
 
 # pylint: disable=too-many-arguments, too-many-function-args
 
 
+YAXIS_TITLES = {
+    "AGRWTH": "Annual Growth Rate (%)",
+    "IDX": "Index (Base = 2015)",
+    "IDX2015": "Index (Base = 2015)",
+    "MLN_USD": "Millions of US Dollars",
+    "PC_CHGPY": "Same Quarter of the Previous Year (% Change)",
+    "PC_CHGPP": "Previous Quarter (% Change)",
+    "PC_GDP": "Percentage of GDP (%)",
+    "THND_USD_CAP": "Thousands of USD per Capita",
+    "USD_CAP": "US Dollars per Capita",
+}
+
+
 @log_start_end(log=logger)
 def plot_gdp(
     countries: Optional[List[str]],
     units: str = "USD_CAP",
     start_date: str = "",
     end_date: str = "",
     raw: bool = False,
     export: str = "",
     sheet_name: str = "",
     external_axes: bool = False,
-) -> pd.DataFrame:
+) -> Union[OpenBBFigure, None]:
     """
     Gross domestic product (GDP) is the standard measure of the value added created
     through the production of goods and services in a country during a certain period.
     As such, it also measures the income earned from that production, or the total amount
     spent on final goods and services (less imports). While GDP is the single most important
     indicator to capture economic activity, it falls short of providing a suitable measure of
     people's material well-being for which alternative indicators may be more appropriate.
@@ -50,80 +61,86 @@
     units: str
         Units to get data in. Either 'USD_CAP' or 'MLN_USD'.
         Default is US dollars per capita.
     start_date: str
         Start date of data, in YYYY-MM-DD format
     end_date: str
         End date of data, in YYYY-MM-DD format
+    raw: bool
+        Whether to display raw data in a table
+    export: str
+        Format to export data
+    sheet_name: str
+        Optionally specify the name of the sheet the data is exported to.
+    external_axes: bool, optional
+        Whether to return the figure object or not, by default False
 
     Returns
     -------
-    pd.DataFrame
-        Dataframe with the interest rate data
+    Union[OpenBBFigure, None]
+        OpenBBFigure object if external_axes is True, else None (opens plot in a window)
     """
     if units not in ["USD_CAP", "MLN_USD"]:
         return console.print(
             "Use either USD_CAP (US dollars per capita) "
             "or MLN_USD (millions of US dollars) for units"
         )
 
     df = oecd_model.get_gdp(countries, units, start_date, end_date)
 
-    if not df.empty:
-        if units == "USD_CAP":
-            fig = OpenBBFigure(yaxis_title="US Dollars per Capita")
-        else:
-            fig = OpenBBFigure(yaxis_title="Millions of US Dollars")
-
-        for country in df.columns:
-            fig.add_scatter(
-                x=df.index,
-                y=df[country],
-                name=country.replace("_", " ").title(),
-                mode="lines",
-                line_width=2.5,
-                showlegend=True,
-            )
-
-        title = "Nominal Gross Domestic Product (GDP)"
-        fig.set_title(title)
-
-        if raw:
-            print_rich_table(
-                df,
-                headers=list(df.columns),
-                show_index=True,
-                title=title,
-                export=bool(export),
-            )
-
-        export_data(
-            export,
-            os.path.dirname(os.path.abspath(__file__)),
-            f"nominal_gdp_{units}",
+    if df.empty:
+        return None
+
+    fig = OpenBBFigure(yaxis_title=YAXIS_TITLES[units])
+
+    for country in df.columns:
+        fig.add_scatter(
+            x=df.index,
+            y=df[country],
+            name=country.replace("_", " ").title(),
+            mode="lines",
+            line_width=2.5,
+            showlegend=True,
+        )
+
+    title = "Nominal Gross Domestic Product (GDP)"
+    fig.set_title(title)
+
+    if raw:
+        print_rich_table(
             df,
-            sheet_name,
-            fig,
+            headers=list(df.columns),
+            show_index=True,
+            title=title,
+            export=bool(export),
         )
 
-        return fig.show(external=external_axes)
-    return None
+    export_data(
+        export,
+        os.path.dirname(os.path.abspath(__file__)),
+        f"nominal_gdp_{units}",
+        df,
+        sheet_name,
+        fig,
+    )
+
+    return fig.show(external=external_axes)
 
 
 @log_start_end(log=logger)
 def plot_real_gdp(
     countries: Optional[List[str]],
     units: str = "PC_CHGPY",
     start_date: str = "",
     end_date: str = "",
     raw: bool = False,
     export: str = "",
     sheet_name: str = "",
     external_axes: bool = False,
-) -> pd.DataFrame:
+) -> Union[OpenBBFigure, None]:
     """
     Gross domestic product (GDP) is the standard measure of the value added
     created through the production of goods and services in a country during
     a certain period. As such, it also measures the income earned from that
     production, or the total amount spent on final goods and services (less imports).
     While GDP is the single most important indicator to capture economic activity, it
     falls short of providing a suitable measure of people's material well-being for
@@ -142,88 +159,94 @@
     units: str
         Units to get data in. Either 'PC_CHGPP', 'PC_CHGPY' or 'IDX.
         Default is percentage change from the same quarter of the previous year.
     start_date: str
         Start date of data, in YYYY-MM-DD format
     end_date: str
         End date of data, in YYYY-MM-DD format
+    raw: bool
+        Whether to display raw data in a table
+    export: str
+        Format to export data
+    sheet_name: str
+        Optionally specify the name of the sheet the data is exported to.
+    external_axes: bool, optional
+        Whether to return the figure object or not, by default False
 
     Returns
     -------
-    pd.DataFrame
-        Dataframe with the interest rate data
+    Union[OpenBBFigure, None]
+        OpenBBFigure object if external_axes is True, else None (opens plot in a window)
     """
     if units not in ["PC_CHGPP", "PC_CHGPY", "IDX"]:
         return console.print(
             "Use either PC_CHGPP (percentage change previous quarter), "
             "PC_CHGPY (percentage change from the same quarter of the "
             "previous year) or IDX (index with base at 2015) "
             "for units"
         )
 
     df = oecd_model.get_real_gdp(countries, units, start_date, end_date)
 
-    if not df.empty:
-        if units == "PC_CHGPP":
-            fig = OpenBBFigure(yaxis_title="Previous Quarter (% Change)")
-        elif units == "PC_CHGPY":
-            fig = OpenBBFigure(
-                yaxis_title="Same Quarter of the Previous Year (% Change)",
-                yaxis_title_font_size=13,
-            )
-        else:
-            fig = OpenBBFigure(yaxis_title="Index (Base = 2015)")
-
-        for country in df.columns:
-            fig.add_scatter(
-                x=df.index,
-                y=df[country],
-                name=country.replace("_", " ").title(),
-                mode="lines",
-                line_width=2.5,
-                showlegend=True,
-            )
-
-        title = "Real Gross Domestic Product (GDP)"
-        fig.set_title(title)
-
-        if raw:
-            print_rich_table(
-                df,
-                headers=list(df.columns),
-                show_index=True,
-                title=title,
-                export=bool(export),
-            )
-
-        export_data(
-            export,
-            os.path.dirname(os.path.abspath(__file__)),
-            f"real_gdp_{units}",
-            df if units == "IDX" else df / 100,
-            sheet_name,
-            fig,
+    if df.empty:
+        return None
+
+    kwargs: Dict[str, Any] = {"yaxis_title": YAXIS_TITLES[units]}
+
+    if units == "PC_CHGPY":
+        kwargs["yaxis_title_font_size"] = 14
+
+    fig = OpenBBFigure(**kwargs)
+
+    for country in df.columns:
+        fig.add_scatter(
+            x=df.index,
+            y=df[country],
+            name=country.replace("_", " ").title(),
+            mode="lines",
+            line_width=2.5,
+            showlegend=True,
         )
 
-        return fig.show(external=external_axes)
-    return None
+    title = "Real Gross Domestic Product (GDP)"
+    fig.set_title(title)
+
+    if raw:
+        print_rich_table(
+            df,
+            headers=list(df.columns),
+            show_index=True,
+            title=title,
+            export=bool(export),
+        )
+
+    export_data(
+        export,
+        os.path.dirname(os.path.abspath(__file__)),
+        f"real_gdp_{units}",
+        df if units == "IDX" else df / 100,
+        sheet_name,
+        fig,
+    )
+
+    return fig.show(external=external_axes)
 
 
 @log_start_end(log=logger)
 def plot_gdp_forecast(
     countries: Optional[List[str]],
     types: str = "real",
     quarterly: bool = False,
     start_date: str = "",
     end_date: str = "",
     raw: bool = False,
     export: str = "",
     sheet_name: str = "",
     external_axes: bool = False,
-) -> pd.DataFrame:
+) -> Union[OpenBBFigure, None]:
     """
     Real gross domestic product (GDP) is GDP given in constant prices and
     refers to the volume level of GDP. Constant price estimates of GDP are
     obtained by expressing values of all goods and services produced in a
     given year, expressed in terms of a base period. Forecast is based on an
     assessment of the economic climate in individual countries and the world economy,
     using a combination of model-based analyses and expert judgement. This indicator
@@ -238,95 +261,104 @@
         Default s real GDP (real).
     quarterly: bool
         Whether to get quarterly results.
     start_date: str
         Start date of data, in YYYY-MM-DD format
     end_date: str
         End date of data, in YYYY-MM-DD format
+    raw: bool
+        Whether to display raw data in a table
+    export: str
+        Format to export data
+    sheet_name: str
+        Optionally specify the name of the sheet the data is exported to.
+    external_axes: bool, optional
+        Whether to return the figure object or not, by default False
 
     Returns
     -------
-    pd.DataFrame
-        Dataframe with the interest rate data
+    Union[OpenBBFigure, None]
+        OpenBBFigure object if external_axes is True, else None (opens plot in a window)
     """
     if types not in ["real", "nominal"]:
         return console.print("Use either 'real' or 'nominal' for type")
 
     units = "Q" if quarterly else "A"
     df = oecd_model.get_gdp_forecast(countries, types, units, start_date, end_date)
 
-    if not df.empty:
-        fig = OpenBBFigure(yaxis_title="Growth rates Compared to Previous Year (%)")
+    if df.empty:
+        return None
+
+    fig = OpenBBFigure(yaxis_title="Growth rates Compared to Previous Year (%)")
+
+    future_dates = df[
+        df.index > str(datetime.now())
+        if units == "Q"
+        else df.index >= datetime.now().year
+    ]
+    for country in df.columns:
+        fig.add_scatter(
+            x=df.index,
+            y=df[country],
+            name=country.replace("_", " ").title(),
+            mode="lines",
+            line_width=2.5,
+            showlegend=True,
+        )
+
+    if not future_dates.empty:
+        fig.add_vrect(
+            x0=future_dates.index[0],
+            x1=future_dates.index[-1],
+            annotation_text="Forecast",
+            fillcolor="yellow",
+            opacity=0.20,
+            line_width=0,
+        )
+
+    title = (
+        f"Forecast of {'Quarterly' if units == 'Q' else 'Annual'} "
+        f"{'Real' if types == 'real' else 'Nominal'} Gross Domestic Product (GDP)"
+    )
+    fig.set_title(title, font_size=20)
 
-        future_dates = df[
-            df.index > str(datetime.now())
-            if units == "Q"
-            else df.index >= datetime.now().year
-        ]
-        for country in df.columns:
-            fig.add_scatter(
-                x=df.index,
-                y=df[country],
-                name=country.replace("_", " ").title(),
-                mode="lines",
-                line_width=2.5,
-                showlegend=True,
-            )
-
-        if not future_dates.empty:
-            fig.add_vrect(
-                x0=future_dates.index[0],
-                x1=future_dates.index[-1],
-                annotation_text="Forecast",
-                fillcolor="yellow",
-                opacity=0.20,
-                line_width=0,
-            )
-
-        title = (
-            f"Forecast of {'Quarterly' if units == 'Q' else 'Annual'} "
-            f"{'Real' if types == 'real' else 'Nominal'} Gross Domestic Product (GDP)"
-        )
-        fig.set_title(title, font_size=20)
-
-        if raw:
-            print_rich_table(
-                df,
-                headers=list(df.columns),
-                show_index=True,
-                title=title,
-                export=bool(export),
-            )
-
-        export_data(
-            export,
-            os.path.dirname(os.path.abspath(__file__)),
-            "forecast_gdp",
-            df / 100,
-            sheet_name,
-            fig,
+    if raw:
+        print_rich_table(
+            df,
+            headers=list(df.columns),
+            show_index=True,
+            title=title,
+            export=bool(export),
         )
 
-        return fig.show(external=external_axes)
-    return None
+    export_data(
+        export,
+        os.path.dirname(os.path.abspath(__file__)),
+        "forecast_gdp",
+        df / 100,
+        sheet_name,
+        fig,
+    )
+
+    return fig.show(external=external_axes)
 
 
 @log_start_end(log=logger)
 def plot_cpi(
     countries: Optional[List[str]],
     perspective: str = "TOT",
     frequency: str = "Q",
     units: str = "AGRWTH",
     start_date: str = "",
     end_date: str = "",
     raw: bool = False,
     export: str = "",
     sheet_name: str = "",
     external_axes: bool = False,
-) -> pd.DataFrame:
+) -> Union[OpenBBFigure, None]:
     """
     Inflation measured by consumer price index (CPI) is defined as the change in the prices
     of a basket of goods and services that are typically purchased by specific groups of
     households. Inflation is measured in terms of the annual growth rate and in index,
     2015 base year with a breakdown for food, energy and total excluding food and energy.
     Inflation measures the erosion of living standards. A consumer price index is estimated
     as a series of summary measures of the period-to-period proportional change in the
@@ -351,83 +383,88 @@
     units: str
         Units to get data in. Either 'AGRWTH' (annual growth rate) or IDX2015 (base = 2015).
         Default is Annual Growth Rate (AGRWTH).
     start_date: str
         Start date of data, in YYYY-MM-DD format
     end_date: str
         End date of data, in YYYY-MM-DD format
+    raw: bool
+        Whether to display raw data in a table
+    export: str
+        Format to export data
+    sheet_name: str
+        Optionally specify the name of the sheet the data is exported to.
+    external_axes: bool, optional
+        Whether to return the figure object or not, by default False
 
     Returns
     -------
-    pd.DataFrame
-        Dataframe with the interest rate data
+    Union[OpenBBFigure, None]
+        OpenBBFigure object if external_axes is True, else None (opens plot in a window)
     """
     df = oecd_model.get_cpi(
         countries, perspective, frequency, units, start_date, end_date
     )
 
-    if not df.empty:
-        fig = OpenBBFigure(
-            yaxis_title="Annual Growth Rate (%)"
-            if units == "AGRWTH"
-            else "Index (2015 = 100)"
-        )
-
-        for country in df.columns:
-            fig.add_scatter(
-                x=df.index,
-                y=df[country],
-                name=country.replace("_", " ").title(),
-                mode="lines",
-                line_width=2.5,
-                showlegend=True,
-            )
-
-        perspective_naming = {
-            "FOOD": "Food",
-            "ENRG": "Energy",
-            "TOT": "Total",
-            "TOT_FOODENRG": "Total Excluding Food and Energy",
-        }
-
-        title = f"Consumer Price Index (CPI) ({perspective_naming[perspective]})"
-        fig.set_title(title)
-
-        if raw:
-            print_rich_table(
-                df,
-                headers=list(df.columns),
-                show_index=True,
-                title=title,
-                export=bool(export),
-            )
-
-        export_data(
-            export,
-            os.path.dirname(os.path.abspath(__file__)),
-            "cpi",
-            df / 100 if units == "AGRWTH" else df,
-            sheet_name,
-            fig,
+    if df.empty:
+        return None
+
+    fig = OpenBBFigure(yaxis_title=YAXIS_TITLES[units])
+
+    for country in df.columns:
+        fig.add_scatter(
+            x=df.index,
+            y=df[country],
+            name=country.replace("_", " ").title(),
+            mode="lines",
+            line_width=2.5,
+            showlegend=True,
+        )
+
+    perspective_naming = {
+        "FOOD": "Food",
+        "ENRG": "Energy",
+        "TOT": "Total",
+        "TOT_FOODENRG": "Total Excluding Food and Energy",
+    }
+
+    title = f"Consumer Price Index (CPI) ({perspective_naming[perspective]})"
+    fig.set_title(title)
+
+    if raw:
+        print_rich_table(
+            df,
+            headers=list(df.columns),
+            show_index=True,
+            title=title,
+            export=bool(export),
         )
 
-        return fig.show(external=external_axes)
-    return None
+    export_data(
+        export,
+        os.path.dirname(os.path.abspath(__file__)),
+        "cpi",
+        df / 100 if units == "AGRWTH" else df,
+        sheet_name,
+        fig,
+    )
+
+    return fig.show(external=external_axes)
 
 
 @log_start_end(log=logger)
 def plot_balance(
     countries: Optional[List[str]],
     start_date: str = "",
     end_date: str = "",
     raw: bool = False,
     export: str = "",
     sheet_name: str = "",
     external_axes: bool = False,
-) -> pd.DataFrame:
+) -> Union[OpenBBFigure, None]:
     """
     General government balance is defined as the balance of income and expenditure of government,
     including capital income and capital expenditures. "Net lending" means that governmen
     has a surplus, and is providing financial resources to other sectors, while
     "net borrowing" means that government has a deficit, and requires financial
     esources from other sectors. This indicator is measured as a percentage of GDP.
     All OECD countries compile their data according to the
@@ -437,71 +474,80 @@
     ----------
     countries: list
         List of countries to get data for
     start_date: str
         Start date of data, in YYYY-MM-DD format
     end_date: str
         End date of data, in YYYY-MM-DD format
+    raw: bool
+        Whether to display raw data in a table
+    export: str
+        Format to export data
+    sheet_name: str
+        Optionally specify the name of the sheet the data is exported to.
+    external_axes: bool, optional
+        Whether to return the figure object or not, by default False
 
     Returns
     -------
-    pd.DataFrame
-        Dataframe with the interest rate data
+    Union[OpenBBFigure, None]
+        OpenBBFigure object if external_axes is True, else None (opens plot in a window)
     """
     df = oecd_model.get_balance(countries, start_date, end_date)
 
-    if not df.empty:
-        fig = OpenBBFigure(yaxis_title="Percentage of GDP (%)")
+    if df.empty:
+        return None
 
-        for country in df.columns:
-            fig.add_scatter(
-                x=df.index,
-                y=df[country],
-                name=country.replace("_", " ").title(),
-                mode="lines",
-                line_width=2.5,
-                showlegend=True,
-            )
-
-        title = "Government Defict or Suplus"
-        fig.set_title(title)
-
-        if raw:
-            print_rich_table(
-                df,
-                headers=list(df.columns),
-                show_index=True,
-                title=title,
-                export=bool(export),
-            )
-
-        export_data(
-            export,
-            os.path.dirname(os.path.abspath(__file__)),
-            "balance_percentage_gdp",
-            df / 100,
-            sheet_name,
-            fig,
+    fig = OpenBBFigure(yaxis_title="Percentage of GDP (%)")
+
+    for country in df.columns:
+        fig.add_scatter(
+            x=df.index,
+            y=df[country],
+            name=country.replace("_", " ").title(),
+            mode="lines",
+            line_width=2.5,
+            showlegend=True,
         )
 
-        return fig.show(external=external_axes)
-    return None
+    title = "Government Defict or Suplus"
+    fig.set_title(title)
+
+    if raw:
+        print_rich_table(
+            df,
+            headers=list(df.columns),
+            show_index=True,
+            title=title,
+            export=bool(export),
+        )
+
+    export_data(
+        export,
+        os.path.dirname(os.path.abspath(__file__)),
+        "balance_percentage_gdp",
+        df / 100,
+        sheet_name,
+        fig,
+    )
+
+    return fig.show(external=external_axes)
 
 
 @log_start_end(log=logger)
 def plot_revenue(
     countries: Optional[List[str]],
     units: str = "PC_GDP",
     start_date: str = "",
     end_date: str = "",
     raw: bool = False,
     export: str = "",
     sheet_name: str = "",
     external_axes: bool = False,
-) -> pd.DataFrame:
+) -> Union[OpenBBFigure, None]:
     """
     Governments collect revenues mainly for two purposes: to finance the goods
     and services they provide to citizens and businesses, and to fulfil their
     redistributive role. Comparing levels of government revenues across
     countries provides an indication of the importance of the government
     sector in the economy in terms of available financial resources.
     The total amount of revenues collected by governments is determined
@@ -511,87 +557,93 @@
     National Accounts (SNA 2008). [Source: OECD]
 
     Parameters
     ----------
     countries: list
         List of countries to get data for
     units: str
-        Units to get data in. Either 'PC_GDP' or 'THOUSAND_USD_PER_CAPITA'.
+        Units to get data in. Either 'PC_GDP' or 'THND_USD_CAP'.
         Default is Percentage of GDP.
     start_date: str
         Start date of data, in YYYY-MM-DD format
     end_date: str
         End date of data, in YYYY-MM-DD format
+    raw: bool
+        Whether to display raw data in a table
+    export: str
+        Format to export data
+    sheet_name: str
+        Optionally specify the name of the sheet the data is exported to.
+    external_axes: bool, optional
+        Whether to return the figure object or not, by default False
 
     Returns
     -------
-    pd.DataFrame
-        Dataframe with the interest rate data
+    Union[OpenBBFigure, None]
+        OpenBBFigure object if external_axes is True, else None (opens plot in a window)
     """
     if units not in ["THND_USD_CAP", "PC_GDP"]:
         return console.print(
             "Use either THND_USD_CAP (thousands of USD per capity) "
             "or PC_GDP (percentage of GDP) for units"
         )
 
     df = oecd_model.get_revenue(countries, units, start_date, end_date)
 
-    if not df.empty:
-        if units == "THND_USD_CAP":
-            fig = OpenBBFigure(yaxis_title="Thousands of USD per Capita")
-        else:
-            fig = OpenBBFigure(yaxis_title="Percentage of GDP (%)")
-
-        for country in df.columns:
-            fig.add_scatter(
-                x=df.index,
-                y=df[country],
-                name=country.replace("_", " ").title(),
-                mode="lines",
-                line_width=2.5,
-                showlegend=True,
-            )
-
-        title = "Government Revenue"
-        fig.set_title(title)
-
-        if raw:
-            print_rich_table(
-                df,
-                headers=list(df.columns),
-                show_index=True,
-                title=title,
-                export=bool(export),
-            )
-
-        export_data(
-            export,
-            os.path.dirname(os.path.abspath(__file__)),
-            f"revenue_{units}",
-            df / 100 if units == "PC_GDP" else df,
-            sheet_name,
-            fig,
+    if df.empty:
+        return None
+
+    fig = OpenBBFigure(yaxis_title=YAXIS_TITLES[units])
+
+    for country in df.columns:
+        fig.add_scatter(
+            x=df.index,
+            y=df[country],
+            name=country.replace("_", " ").title(),
+            mode="lines",
+            line_width=2.5,
+            showlegend=True,
         )
 
-        return fig.show(external=external_axes)
-    return None
+    title = "Government Revenue"
+    fig.set_title(title)
+
+    if raw:
+        print_rich_table(
+            df,
+            headers=list(df.columns),
+            show_index=True,
+            title=title,
+            export=bool(export),
+        )
+
+    export_data(
+        export,
+        os.path.dirname(os.path.abspath(__file__)),
+        f"revenue_{units}",
+        df / 100 if units == "PC_GDP" else df,
+        sheet_name,
+        fig,
+    )
+
+    return fig.show(external=external_axes)
 
 
 @log_start_end(log=logger)
 def plot_spending(
     countries: Optional[List[str]],
     perspective: str = "TOT",
     units: str = "PC_GDP",
     start_date: str = "",
     end_date: str = "",
     raw: bool = False,
     export: str = "",
     sheet_name: str = "",
     external_axes: bool = False,
-) -> pd.DataFrame:
+) -> Union[OpenBBFigure, None]:
     """
     General government spending provides an indication of the size
     of government across countries. The large variation in this indicator
     highlights the variety of countries' approaches to delivering public
     goods and services and providing social protection, not necessarily
     differences in resources spent. This indicator is measured in terms of
     thousand USD per capita, and as percentage of GDP. All OECD countries
@@ -599,93 +651,99 @@
     National Accounts (SNA). [Source: OECD]
 
     Parameters
     ----------
     countries: list
         List of countries to get data for
     units: str
-        Units to get data in. Either 'PC_GDP' or 'THOUSAND_USD_PER_CAPITA'.
+        Units to get data in. Either 'PC_GDP' or 'THND_USD_CAP'.
         Default is Percentage of GDP.
     start_date: str
         Start date of data, in YYYY-MM-DD format
     end_date: str
         End date of data, in YYYY-MM-DD format
+    raw: bool
+        Whether to display raw data in a table
+    export: str
+        Format to export data
+    sheet_name: str
+        Optionally specify the name of the sheet the data is exported to.
+    external_axes: bool, optional
+        Whether to return the figure object or not, by default False
 
     Returns
     -------
-    pd.DataFrame
-        Dataframe with the interest rate data
+    Union[OpenBBFigure, None]
+        OpenBBFigure object if external_axes is True, else None (opens plot in a window)
     """
     df = oecd_model.get_spending(countries, perspective, units, start_date, end_date)
 
-    if not df.empty:
-        if units == "THND_USD_CAP":
-            fig = OpenBBFigure(yaxis_title="Thousands of USD per Capita")
-        else:
-            fig = OpenBBFigure(yaxis_title="Percentage of GDP (%)")
-
-        for country in df.columns:
-            fig.add_scatter(
-                x=df.index,
-                y=df[country],
-                name=country.replace("_", " ").title(),
-                mode="lines",
-                line_width=2.5,
-                showlegend=True,
-            )
-
-        perspective_naming = {
-            "TOT": "Total",
-            "RECULTREL": "Recreation, culture and religion)",
-            "HOUCOMM": "Housing and community amenities",
-            "PUBORD": "Public order and safety)",
-            "EDU": "Education",
-            "ENVPROT": "Environmental protection",
-            "GRALPUBSER": "General public services)",
-            "SOCPROT": "Social protection",
-            "ECOAFF": "Economic affairs",
-            "DEF": "Defence",
-            "HEALTH": "Health",
-        }
-
-        title = f"Government Spending ({perspective_naming[perspective]})"
-        fig.set_title(title)
-
-        if raw:
-            print_rich_table(
-                df,
-                headers=list(df.columns),
-                show_index=True,
-                title=title,
-                export=bool(export),
-            )
-
-        export_data(
-            export,
-            os.path.dirname(os.path.abspath(__file__)),
-            f"spending_{units}_{perspective}",
-            df / 100 if units == "PC_GDP" else df,
-            sheet_name,
-            fig,
+    if df.empty:
+        return None
+
+    fig = OpenBBFigure(yaxis_title=YAXIS_TITLES[units])
+
+    for country in df.columns:
+        fig.add_scatter(
+            x=df.index,
+            y=df[country],
+            name=country.replace("_", " ").title(),
+            mode="lines",
+            line_width=2.5,
+            showlegend=True,
+        )
+
+    perspective_naming = {
+        "TOT": "Total",
+        "RECULTREL": "Recreation, culture and religion)",
+        "HOUCOMM": "Housing and community amenities",
+        "PUBORD": "Public order and safety)",
+        "EDU": "Education",
+        "ENVPROT": "Environmental protection",
+        "GRALPUBSER": "General public services)",
+        "SOCPROT": "Social protection",
+        "ECOAFF": "Economic affairs",
+        "DEF": "Defence",
+        "HEALTH": "Health",
+    }
+
+    title = f"Government Spending ({perspective_naming[perspective]})"
+    fig.set_title(title)
+
+    if raw:
+        print_rich_table(
+            df,
+            headers=list(df.columns),
+            show_index=True,
+            title=title,
+            export=bool(export),
         )
 
-        return fig.show(external=external_axes)
-    return None
+    export_data(
+        export,
+        os.path.dirname(os.path.abspath(__file__)),
+        f"spending_{units}_{perspective}",
+        df / 100 if units == "PC_GDP" else df,
+        sheet_name,
+        fig,
+    )
+
+    return fig.show(external=external_axes)
 
 
 @log_start_end(log=logger)
 def plot_debt(
     countries: Optional[List[str]],
     start_date: str = "",
     end_date: str = "",
     raw: bool = False,
     export: str = "",
     sheet_name: str = "",
     external_axes: bool = False,
-) -> pd.DataFrame:
+) -> Union[OpenBBFigure, None]:
     """
     General government debt-to-GDP ratio measures the gross debt of the general
     government as a percentage of GDP. It is a key indicator for the sustainability
     of government finance. Debt is calculated as the sum of the following liability
     categories (as applicable): currency and deposits; debt securities, loans; insurance,
     pensions and standardised guarantee schemes, and other accounts payable. Changes in
     government debt over time primarily reflect the impact of past government deficits. [Source: OECD]
@@ -694,70 +752,79 @@
     ----------
     countries: list
         List of countries to get data for
     start_date: str
         Start date of data, in YYYY-MM-DD format
     end_date: str
         End date of data, in YYYY-MM-DD format
+    raw: bool
+        Whether to display raw data in a table
+    export: str
+        Format to export data
+    sheet_name: str
+        Optionally specify the name of the sheet the data is exported to.
+    external_axes: bool, optional
+        Whether to return the figure object or not, by default False
 
     Returns
     -------
-    pd.DataFrame
-        Dataframe with the interest rate data
+    Union[OpenBBFigure, None]
+        OpenBBFigure object if external_axes is True, else None (opens plot in a window)
     """
     df = oecd_model.get_debt(countries, start_date, end_date)
 
-    if not df.empty:
-        fig = OpenBBFigure(yaxis_title="Percentage of GDP (%)")
+    if df.empty:
+        return None
 
-        for country in df.columns:
-            fig.add_scatter(
-                x=df.index,
-                y=df[country],
-                name=country.replace("_", " ").title(),
-                mode="lines",
-                line_width=2.5,
-                showlegend=True,
-            )
-
-        title = "Government Debt-to-GDP Ratio"
-        fig.set_title(title)
-
-        if raw:
-            print_rich_table(
-                df,
-                headers=list(df.columns),
-                show_index=True,
-                title=title,
-                export=bool(export),
-            )
-
-        export_data(
-            export,
-            os.path.dirname(os.path.abspath(__file__)),
-            "debt_to_gdp",
-            df / 100,
-            sheet_name,
-            fig,
+    fig = OpenBBFigure(yaxis_title="Percentage of GDP (%)")
+
+    for country in df.columns:
+        fig.add_scatter(
+            x=df.index,
+            y=df[country],
+            name=country.replace("_", " ").title(),
+            mode="lines",
+            line_width=2.5,
+            showlegend=True,
         )
 
-        return fig.show(external=external_axes)
-    return None
+    title = "Government Debt-to-GDP Ratio"
+    fig.set_title(title)
+
+    if raw:
+        print_rich_table(
+            df,
+            headers=list(df.columns),
+            show_index=True,
+            title=title,
+            export=bool(export),
+        )
+
+    export_data(
+        export,
+        os.path.dirname(os.path.abspath(__file__)),
+        "debt_to_gdp",
+        df / 100,
+        sheet_name,
+        fig,
+    )
+
+    return fig.show(external=external_axes)
 
 
 @log_start_end(log=logger)
 def plot_trust(
     countries: Optional[List[str]],
     start_date: str = "",
     end_date: str = "",
     raw: bool = False,
     export: str = "",
     sheet_name: str = "",
     external_axes: bool = False,
-) -> pd.DataFrame:
+) -> Union[OpenBBFigure, None]:
     """
     Trust in government refers to the share of people who report having confidence in
     the national government. The data shown reflect the share of respondents answering
     “yes” (the other response categories being “no”, and “don’t know”) to the
     survey question: “In this country, do you have confidence in national
     government? Due to small sample sizes, country averages for horizontal inequalities
     (by age, gender and education) are pooled between 2010-18 to improve the accuracy
@@ -769,51 +836,60 @@
     ----------
     countries: list
         List of countries to get data for
     start_date: str
         Start date of data, in YYYY-MM-DD format
     end_date: str
         End date of data, in YYYY-MM-DD format
+    raw: bool
+        Whether to display raw data in a table
+    export: str
+        Format to export data
+    sheet_name: str
+        Optionally specify the name of the sheet the data is exported to.
+    external_axes: bool, optional
+        Whether to return the figure object or not, by default False
 
     Returns
     -------
-    pd.DataFrame
-        Dataframe with the interest rate data
+    Union[OpenBBFigure, None]
+        OpenBBFigure object if external_axes is True, else None (opens plot in a window)
     """
     df = oecd_model.get_trust(countries, start_date, end_date)
 
-    if not df.empty:
-        fig = OpenBBFigure(yaxis_title="Percentage of all Survey Respondents (%)")
+    if df.empty:
+        return None
+
+    fig = OpenBBFigure(yaxis_title="Percentage of all Survey Respondents (%)")
+
+    for country in df.columns:
+        fig.add_scatter(
+            x=df.index,
+            y=df[country],
+            name=country.replace("_", " ").title(),
+            mode="lines",
+            line_width=2.5,
+            showlegend=True,
+        )
+
+    title = "Trust in the Government"
+    fig.set_title(title)
 
-        for country in df.columns:
-            fig.add_scatter(
-                x=df.index,
-                y=df[country],
-                name=country.replace("_", " ").title(),
-                mode="lines",
-                line_width=2.5,
-                showlegend=True,
-            )
-
-        title = "Trust in the Government"
-        fig.set_title(title)
-
-        if raw:
-            print_rich_table(
-                df,
-                headers=list(df.columns),
-                show_index=True,
-                title=title,
-                export=bool(export),
-            )
-
-        export_data(
-            export,
-            os.path.dirname(os.path.abspath(__file__)),
-            "trust",
-            df / 100,
-            sheet_name,
-            fig,
+    if raw:
+        print_rich_table(
+            df,
+            headers=list(df.columns),
+            show_index=True,
+            title=title,
+            export=bool(export),
         )
 
-        return fig.show(external=external_axes)
-    return None
+    export_data(
+        export,
+        os.path.dirname(os.path.abspath(__file__)),
+        "trust",
+        df / 100,
+        sheet_name,
+        fig,
+    )
+
+    return fig.show(external=external_axes)
```

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/economy/plot_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/economy/plot_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/economy/quantitative_analysis/qa_controller.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/economy/quantitative_analysis/qa_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/economy/sdk_helpers.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/economy/sdk_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/economy/wsj_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/economy/wsj_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/economy/wsj_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/economy/wsj_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/economy/yfinance_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/economy/yfinance_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/economy/yfinance_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/economy/yfinance_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/etf/discovery/disc_controller.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/etf/discovery/disc_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/etf/discovery/wsj_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/etf/discovery/wsj_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/etf/discovery/wsj_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/etf/discovery/wsj_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/etf/etf_controller.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/etf/etf_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/etf/etfs.csv` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/etf/etfs.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/etf/financedatabase_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/etf/financedatabase_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/etf/financedatabase_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/etf/financedatabase_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/etf/fmp_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/etf/fmp_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/etf/fmp_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/etf/fmp_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/etf/stockanalysis_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/etf/stockanalysis_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/etf/stockanalysis_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/etf/stockanalysis_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/etf/technical_analysis/ta_controller.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/etf/technical_analysis/ta_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/featflags_controller.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/featflags_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/fixedincome/commercial_paper.csv` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/fixedincome/commercial_paper.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/fixedincome/corporate_spot_rates.csv` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/fixedincome/corporate_spot_rates.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/fixedincome/ecb_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/fixedincome/ecb_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/fixedincome/ecb_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/fixedincome/ecb_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/fixedincome/econdb_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/fixedincome/econdb_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/fixedincome/econdb_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/fixedincome/econdb_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/fixedincome/fixedincome_controller.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/fixedincome/fixedincome_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/fixedincome/fred_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/fixedincome/fred_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/fixedincome/fred_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/fixedincome/fred_view.py`

 * *Files 2% similar despite different names*

```diff
@@ -217,15 +217,15 @@
     fig.add_scatter(
         x=df.index, y=df[series_id], mode="lines", name=series_id, line_width=2
     )
 
     if export:
         if series_id not in ["ECBESTRTOTVOL", "ECBESTRNUMACTBANKS", "ECBESTRNUMTRANS"]:
             # Check whether it is a percentage, relevant for exporting
-            df_transformed = pd.DataFrame(df, columns=[series_id]) / 100
+            df_transformed = pd.DataFrame(df, columns=[series_id])
         else:
             df_transformed = pd.DataFrame(df, columns=[series_id])
 
         export_data(
             export,
             os.path.dirname(os.path.abspath(__file__)),
             series_id,
@@ -278,15 +278,15 @@
     fig.set_title(ID_TO_NAME_SOFR[series_id])
 
     fig.add_scatter(x=df.index, y=df[series_id], mode="lines", name=series_id)
 
     if export:
         if series_id != "SOFRINDEX":
             # Check whether it is a percentage, relevant for exporting
-            df_transformed = pd.DataFrame(df, columns=[series_id]) / 100
+            df_transformed = pd.DataFrame(df, columns=[series_id])
         else:
             df_transformed = pd.DataFrame(df, columns=[series_id])
 
         export_data(
             export,
             os.path.dirname(os.path.abspath(__file__)),
             series_id,
@@ -339,15 +339,15 @@
     fig.set_title(ID_TO_NAME_SONIA[series_id])
 
     fig.add_scatter(x=df.index, y=df[series_id], mode="lines", name=series_id)
 
     if export:
         if series_id not in ["IUDZOS2", "IUDZLT2"]:
             # Check whether it is a percentage, relevant for exporting
-            df_transformed = pd.DataFrame(df, columns=[series_id]) / 100
+            df_transformed = pd.DataFrame(df, columns=[series_id])
         else:
             df_transformed = pd.DataFrame(df, columns=[series_id])
 
         export_data(
             export,
             os.path.dirname(os.path.abspath(__file__)),
             series_id,
@@ -398,15 +398,15 @@
     fig.set_title(ID_TO_NAME_AMERIBOR[series_id])
 
     fig.add_scatter(x=df.index, y=df[series_id], mode="lines", name=series_id)
 
     if export:
         if series_id not in ["AMBOR30T", "AMBOR90T"]:
             # Check whether it is a percentage, relevant for exporting
-            df_transformed = pd.DataFrame(df, columns=[series_id]) / 100
+            df_transformed = pd.DataFrame(df, columns=[series_id])
         else:
             df_transformed = pd.DataFrame(df, columns=[series_id])
 
         export_data(
             export,
             os.path.dirname(os.path.abspath(__file__)),
             series_id,
@@ -458,15 +458,15 @@
     for series in df.columns:
         fig.add_scatter(x=df.index, y=df[series], name=series)
 
     export_data(
         export,
         os.path.dirname(os.path.abspath(__file__)),
         "fftr",
-        pd.DataFrame(df, columns=["FFTR"]) / 100,
+        pd.DataFrame(df, columns=["FFTR"]),
         sheet_name,
         fig,
     )
 
     return fig.show(external=external_axes)
 
 
@@ -564,19 +564,19 @@
 
         fig.set_title(ID_TO_NAME_FED[series_id])
 
     if export or raw:
         if not quantiles and not target:
             if series_id != "EFFRVOL":
                 # Check whether it is a percentage, relevant for exporting
-                df_transformed = pd.DataFrame(df, columns=[series_id]) / 100
+                df_transformed = pd.DataFrame(df, columns=[series_id])
             else:
                 df_transformed = pd.DataFrame(df, columns=[series_id])
         else:
-            df_transformed = df / 100
+            df_transformed = df
 
     if raw:
         # was a -iloc so we need to flip the index as we use head
         df_transformed = df_transformed.sort_index(ascending=False)
         print_rich_table(
             df_transformed,
             headers=list(df_transformed.columns),
@@ -629,15 +629,15 @@
 
     fig.add_scatter(x=df.index, y=df["IORB"], name="IORB", line_width=2, mode="lines")
 
     export_data(
         export,
         os.path.dirname(os.path.abspath(__file__)),
         "iorb",
-        pd.DataFrame(df, columns=["IORB"]) / 100,
+        pd.DataFrame(df, columns=["IORB"]),
         sheet_name,
         fig,
     )
 
     return fig.show(external=external_axes)
 
 
@@ -746,15 +746,15 @@
 
     fig.add_scatter(x=df.index, y=df[series_id], name=series_id, mode="lines")
 
     export_data(
         export,
         os.path.dirname(os.path.abspath(__file__)),
         series_id,
-        pd.DataFrame(df, columns=[series_id]) / 100,
+        pd.DataFrame(df, columns=[series_id]),
         sheet_name,
         fig,
     )
 
     return fig.show(external=external_axes)
 
 
@@ -824,15 +824,15 @@
             limit=limit,
         )
 
     export_data(
         export,
         os.path.dirname(os.path.abspath(__file__)),
         "ecbdfr",
-        pd.DataFrame(df, columns=["ECBDFR"]) / 100,
+        pd.DataFrame(df, columns=["ECBDFR"]),
         sheet_name,
         fig,
     )
 
     return fig.show(external=external_axes)
 
 
@@ -879,15 +879,15 @@
 
     fig.add_scatter(x=df.index, y=df[series_id], name=series_id, mode="lines")
 
     export_data(
         export,
         os.path.dirname(os.path.abspath(__file__)),
         series_id,
-        pd.DataFrame(df, columns=[series_id]) / 100,
+        pd.DataFrame(df, columns=[series_id]),
         sheet_name,
         fig,
     )
 
     return fig.show(external=external_axes)
 
 
@@ -931,15 +931,15 @@
 
     fig.add_scatter(x=df.index, y=df[series_id], name=series_id, mode="lines")
 
     export_data(
         export,
         os.path.dirname(os.path.abspath(__file__)),
         series_id,
-        pd.DataFrame(df, columns=[series_id]) / 100,
+        pd.DataFrame(df, columns=[series_id]),
         sheet_name,
         fig,
     )
 
     return fig.show(external=external_axes)
 
 
@@ -1003,15 +1003,15 @@
             export=bool(export),
         )
 
     export_data(
         export,
         os.path.dirname(os.path.abspath(__file__)),
         "ycrv",
-        rates.set_index("Maturity") / 100,
+        rates.set_index("Maturity"),
         sheet_name,
         fig,
     )
 
     return fig.show(external=external_axes)
 
 
@@ -1097,15 +1097,15 @@
             limit=limit,
         )
 
     export_data(
         export,
         os.path.dirname(os.path.abspath(__file__)),
         series_id,
-        pd.DataFrame(df, columns=[series_id]) / 100,
+        pd.DataFrame(df, columns=[series_id]),
         sheet_name,
         fig,
     )
 
     return fig.show(external=external_axes)
 
 
@@ -1152,15 +1152,15 @@
 
     fig.add_scatter(x=df.index, y=df[series_id], name="Yield")
 
     export_data(
         export,
         os.path.dirname(os.path.abspath(__file__)),
         series_id,
-        pd.DataFrame(df, columns=["TBFFR"]) / 100,
+        pd.DataFrame(df, columns=["TBFFR"]),
         sheet_name,
         fig,
     )
 
     return fig.show(external=external_axes)
 
 
@@ -1277,15 +1277,15 @@
             console.print(f"\n[bold]{title}[/bold]")
             console.print(description_text)
 
     export_data(
         export,
         os.path.dirname(os.path.abspath(__file__)),
         "ICEBOFA",
-        df / 100,
+        df,
         sheet_name,
         fig,
     )
 
     return fig.show(external=external_axes)
 
 
@@ -1351,15 +1351,15 @@
             limit=limit,
         )
 
     export_data(
         export,
         os.path.dirname(os.path.abspath(__file__)),
         "MOODY",
-        df / 100,
+        df,
         sheet_name,
         fig,
     )
 
     return fig.show(external=external_axes)
 
 
@@ -1456,15 +1456,15 @@
             console.print(f"\n[bold]{title}[/bold]")
             console.print(description_text)
 
     export_data(
         export,
         os.path.dirname(os.path.abspath(__file__)),
         "CP",
-        df / 100,
+        df,
         sheet_name,
         fig,
     )
 
     return fig.show(external=external_axes)
 
 
@@ -1551,15 +1551,15 @@
             console.print(f"\n[bold]{title}[/bold]")
             console.print(description_text)
 
     export_data(
         export,
         os.path.dirname(os.path.abspath(__file__)),
         "SPOT",
-        df / 100,
+        df,
         sheet_name,
         fig,
     )
 
     return fig.show(external=external_axes)
 
 
@@ -1619,13 +1619,13 @@
             export=bool(export),
         )
 
     export_data(
         export,
         os.path.dirname(os.path.abspath(__file__)),
         "cycrv",
-        df / 100,
+        df,
         sheet_name,
         fig,
     )
 
     return fig.show(external=external_axes)
```

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/fixedincome/ice_bofa_indices.csv` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/fixedincome/ice_bofa_indices.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/fixedincome/oecd_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/fixedincome/oecd_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/fixedincome/oecd_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/fixedincome/oecd_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/fixedincome/yfinance_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/fixedincome/yfinance_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/fixedincome/yfinance_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/fixedincome/yfinance_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/anom_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/anom_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/anom_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/anom_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/autoarima_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/autoarima_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/autoarima_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/autoarima_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/autoces_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/autoces_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/autoces_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/autoces_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/autoets_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/autoets_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/autoets_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/autoets_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/autoselect_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/autoselect_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/autoselect_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/autoselect_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/brnn_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/brnn_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/brnn_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/brnn_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/expo_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/expo_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/expo_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/expo_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/forecast.ipynb` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/forecast.ipynb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/forecast_controller.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/forecast_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/forecast_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/forecast_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/forecast_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/forecast_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/helpers.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/linregr_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/linregr_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/linregr_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/linregr_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/mstl_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/mstl_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/mstl_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/mstl_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/nbeats_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/nbeats_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/nbeats_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/nbeats_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/nhits_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/nhits_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/nhits_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/nhits_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/regr_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/regr_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/regr_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/regr_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/rnn_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/rnn_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/rnn_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/rnn_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/rwd_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/rwd_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/rwd_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/rwd_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/seasonalnaive_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/seasonalnaive_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/seasonalnaive_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/seasonalnaive_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/tcn_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/tcn_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/tcn_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/tcn_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/tft_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/tft_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/tft_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/tft_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/theta_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/theta_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/theta_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/theta_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/trans_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/trans_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/trans_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/trans_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/whisper_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/whisper_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forecast/whisper_utils.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forecast/whisper_utils.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forex/av_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forex/av_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forex/av_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forex/av_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forex/data/av_forex_currencies.csv` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forex/data/av_forex_currencies.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forex/data/polygon_tickers.csv` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forex/data/polygon_tickers.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forex/data/yahoofinance_forex.json` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forex/data/yahoofinance_forex.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forex/forex_controller.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forex/forex_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forex/forex_helper.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forex/forex_helper.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forex/fxempire_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forex/fxempire_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forex/fxempire_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forex/fxempire_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forex/oanda/oanda_controller.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forex/oanda/oanda_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forex/oanda/oanda_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forex/oanda/oanda_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forex/oanda/oanda_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forex/oanda/oanda_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forex/polygon_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forex/polygon_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forex/quantitative_analysis/qa_controller.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forex/quantitative_analysis/qa_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forex/sdk_helpers.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forex/sdk_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/forex/technical_analysis/ta_controller.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/forex/technical_analysis/ta_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/futures/databento_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/futures/databento_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/futures/futures_controller.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/futures/futures_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/futures/sdk_helper.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/futures/sdk_helper.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/futures/yfinance_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/futures/yfinance_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/futures/yfinance_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/futures/yfinance_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/helper_classes.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/helper_classes.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/helper_funcs.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/helper_funcs.py`

 * *Files 1% similar despite different names*

```diff
@@ -348,22 +348,19 @@
             df_outgoing.index.name = index_name or "Index"
             df_outgoing = df_outgoing.reset_index()
 
         for col in df_outgoing.columns:
             if col == "":
                 df_outgoing = df_outgoing.rename(columns={col: "  "})
 
-        theme = current_user.preferences.THEME
-        table_theme = "white" if theme == "light" else theme
-
         plots_backend().send_table(
             df_table=df_outgoing,
             title=title,
             source=source,  # type: ignore
-            theme=table_theme,
+            theme=current_user.preferences.TABLE_STYLE,
         )
         return
 
     df = df.copy() if not limit else df.copy().iloc[:limit]
     if current_user.preferences.USE_COLOR and automatic_coloring:
         if columns_to_auto_color:
             for col in columns_to_auto_color:
@@ -1653,15 +1650,15 @@
     for error_code, error_msg in error_code_map.items():
         if requests_obj.status_code == error_code:
             console.print(error_msg)
 
 
 def prefill_form(ticket_type, menu, path, command, message):
     """Pre-fill Google Form and open it in the browser."""
-    form_url = "https://openbb.co/support?"
+    form_url = "https://my.openbb.dev/app/terminal/support?"
 
     params = {
         "type": ticket_type,
         "menu": menu,
         "path": path,
         "command": command,
         "message": message,
```

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/helpers_denomination.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/helpers_denomination.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/intro.json` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/intro.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/keys_controller.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/keys_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/keys_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/keys_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/keys_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/keys_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/loggers.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/loggers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/menu.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/menu.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/futures/futures.csv` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/futures/futures.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/i18n/en.yml` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/i18n/en.yml`

 * *Files 1% similar despite different names*

```diff
@@ -65,16 +65,18 @@
   featflags/overwrite: whether to overwrite Excel files if they already exists
   featflags/version: whether to show the version in the bottom right corner
   featflags/tbhint: displays usage hints in the bottom toolbar
   settings/_info_: Current settings
   settings/_cmds_: Change settings
   settings/colors: set your own terminal colors
   settings/_colors: Colors
-  settings/theme: set plots and tables theme
-  settings/_theme: Theme
+  settings/chart: set charts style
+  settings/_chart: Charts style
+  settings/table: set tables style
+  settings/_table: Tables style
   settings/autoscaling: plot autoscaling
   settings/dt: add or remove datetime from flair
   settings/flair: set the flair emoji to be used
   settings/_flair: Flair
   settings/lang: terminal language
   settings/_language: Language
   settings/userdata: set folder to store user data
@@ -408,15 +410,14 @@
   stocks/bt/whatif: what if you had bought X shares on day Y
   stocks/bt/ema: buy when price exceeds EMA(l)
   stocks/bt/emacross: buy when EMA(short) > EMA(long)
   stocks/bt/rsi: buy when RSI < low and sell when RSI > high
   stocks/bt/load: load a specific stock ticker for analysis
   stocks/ta/_ticker: Ticker
   stocks/ta/load: load a specific stock ticker for analysis
-  stocks/ta/view: view historical data and trendlines
   stocks/ta/summary: technical summary report
   stocks/ta/recom: recommendation based on technical indicators
   stocks/ta/_overlap_: Overlap
   stocks/ta/ema: exponential moving average
   stocks/ta/sma: simple moving average
   stocks/ta/wma: weighted moving average
   stocks/ta/hma: hull moving average
@@ -770,15 +771,14 @@
   economy/spread: show bond spread matrix
   economy/events: show economic calendar
   economy/edebt: show external debt statistics for various countries
   economy/plot: plot data from the above commands together
   economy/rtps: real-time performance sectors
   economy/valuation: valuation of sectors, industry, country
   economy/performance: performance of sectors, industry, country
-  economy/spectrum: spectrum of sectors, industry, country
   economy/eval: create new series by performing operations on loaded data
   economy/forecast: forecast techniques; rnn, nbeats, transformer, block rnn
   economy/qa: Open quantitative analysis menu with stored data
   economy/qa/pick: pick new series from stored economy data
   economy/qa/_series: Selected series
   economy/qa/_statistics_: Statistics
   economy/qa/summary: brief summary statistics of loaded stock
```

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/i18n/help_translation.ipynb` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/i18n/help_translation.ipynb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/README.MD` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/README.MD`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto.openbb` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto.openbb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_dd.openbb` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_dd.openbb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_defi.openbb` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_defi.openbb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_onchain.openbb` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_onchain.openbb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_ov.openbb` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_ov.openbb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_qa.openbb` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_qa.openbb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_ta.openbb` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_ta.openbb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/econometrics/test_econometrics_base.openbb` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/econometrics/test_econometrics_base.openbb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/economy/test_economy.openbb` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/economy/test_economy.openbb`

 * *Files 6% similar despite different names*

```diff
@@ -21,16 +21,14 @@
 events -n
 edebt --limit 10
 rtps
 valuation
 valuation --group sector --sortby MarketCap --reverse
 performance
 performance -g basic_materials -s Month -a
-spectrum
-spectrum --group consumer_defensive
 gdp
 rgdp
 fgdp
 debt
 cpi
 ccpi
 balance
@@ -64,15 +62,14 @@
 macro -p URATE -c Netherlands,Germany -s 2005-01-01
 index -i sp500 -s 2005-01-01
 plot --y1 T10Y2Y --y2 T5YIEM
 plot --y1 T10Y2Y,T20YIEM
 rtps
 valuation
 performance
-spectrum
 fred -p DGS2,DGS5
 eval spread = DGS2 - DGS5
 qa
 summary
 normality
 unitroot --fuller_reg c --kps_reg ct
 line
```

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/etf/test_etf_ta.openbb` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/etf/test_etf_ta.openbb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/fixedincome/test_fixedincome.openbb` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/fixedincome/test_fixedincome.openbb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/forex/test_forex_oanda.openbb` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/forex/test_forex_oanda.openbb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/forex/test_forex_qa.openbb` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/forex/test_forex_qa.openbb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/forex/test_forex_ta.openbb` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/forex/test_forex_ta.openbb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/portfolio/test_po_show_plot_rpf.openbb` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/portfolio/test_po_show_plot_rpf.openbb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/portfolio/test_portfolio.openbb` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/portfolio/test_portfolio.openbb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/portfolio/test_portfolio_po.openbb` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/portfolio/test_portfolio_po.openbb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_bt.openbb` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_bt.openbb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_fa.openbb` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_fa.openbb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_qa.openbb` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_qa.openbb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_ta.openbb` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_ta.openbb`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 stocks
 load ${ticker=aapl}
 ta
-view
 recom
 summary
 ema -l 20,30,50
 sma
 wma
 hma
 zlma
```

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/models/hub_credentials.json` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/models/hub_credentials.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/portfolio/allocation_example.xlsx` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/portfolio/allocation_example.xlsx`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/portfolio/holdings_example.xlsx` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/portfolio/holdings_example.xlsx`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/sources/openbb_default.json` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/sources/openbb_default.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9975879917184265%*

 * *Differences: {"'economy'": "{delete: ['spectrum']}", "'stocks'": "{'ta': {delete: ['view']}}"}*

```diff
@@ -488,17 +488,14 @@
         ],
         "rgdp": [
             "OECD"
         ],
         "rtps": [
             "AlphaVantage"
         ],
-        "spectrum": [
-            "Finviz"
-        ],
         "spending": [
             "OECD"
         ],
         "treasury": [
             "EconDB"
         ],
         "trust": [
@@ -1383,17 +1380,14 @@
                 "TradingView"
             ],
             "summary": [
                 "FinBrain"
             ],
             "tv": [
                 "TradingView"
-            ],
-            "view": [
-                "Finviz"
             ]
         },
         "th": {
             "all": [
                 "Bursa"
             ],
             "closed": [
```

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/insider/Agriculture.ini` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/insider/Agriculture.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/insider/Agro-Chemicals.ini` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/insider/Agro-Chemicals.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/insider/Air-Transportation.ini` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/insider/Air-Transportation.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/insider/Apparel.ini` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/insider/Apparel.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/insider/Banks.ini` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/insider/Banks.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/insider/Brokers.ini` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/insider/Brokers.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/insider/Building-Materials.ini` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/insider/Building-Materials.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/insider/Business-Services.ini` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/insider/Business-Services.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/insider/Closed-End-Funds.ini` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/insider/Closed-End-Funds.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/insider/Construction.ini` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/insider/Construction.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/insider/Credit-Industry.ini` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/insider/Credit-Industry.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/insider/Durable-Goods.ini` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/insider/Durable-Goods.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/insider/Electronics.ini` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/insider/Electronics.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/insider/Furniture.ini` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/insider/Furniture.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/insider/Gold-Silver.ini` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/insider/Gold-Silver.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/insider/Grocery.ini` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/insider/Grocery.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/insider/Ground-Freight.ini` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/insider/Ground-Freight.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/insider/Guided-Missiles.ini` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/insider/Guided-Missiles.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/insider/Health.ini` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/insider/Health.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/insider/Hotels.ini` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/insider/Hotels.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/insider/Insurance-Agents.ini` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/insider/Insurance-Agents.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/insider/Insurance-Carriers.ini` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/insider/Insurance-Carriers.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/insider/Investment-Offices.ini` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/insider/Investment-Offices.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/insider/Legal.ini` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/insider/Legal.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/insider/Lumber.ini` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/insider/Lumber.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/insider/Manufacturing.ini` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/insider/Manufacturing.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/insider/Mining.ini` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/insider/Mining.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/insider/Mortgages.ini` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/insider/Mortgages.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/insider/Nondurable-Goods.ini` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/insider/Nondurable-Goods.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/insider/Personal-Credit.ini` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/insider/Personal-Credit.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/insider/Pharmaceuticals.ini` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/insider/Pharmaceuticals.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/insider/Professional-Services.ini` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/insider/Professional-Services.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/insider/Railroads.ini` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/insider/Railroads.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/insider/Real-Estate.ini` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/insider/Real-Estate.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/insider/Restaurants.ini` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/insider/Restaurants.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/insider/Retail-Stores.ini` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/insider/Retail-Stores.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/insider/Retail-Trade.ini` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/insider/Retail-Trade.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/insider/Tobacco.ini` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/insider/Tobacco.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/insider/Utility-Communications.ini` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/insider/Utility-Communications.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/insider/Utility-Gas.ini` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/insider/Utility-Gas.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/insider/Wholesale-Trade.ini` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/insider/Wholesale-Trade.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/insider/template.ini` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/insider/template.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/insider/whales.ini` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/insider/whales.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/options/README.md` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/options/README.md`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/options/high_iv.ini` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/options/high_iv.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/options/iv_below_20day.ini` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/options/iv_below_20day.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/options/liquid_otm.ini` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/options/liquid_otm.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/options/spy_30_delta.ini` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/options/spy_30_delta.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/options/template.ini` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/options/template.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/screener/all_parameters.txt` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/screener/all_parameters.txt`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/screener/growth_stocks.ini` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/screener/growth_stocks.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/stocks/screener/value_stocks.ini` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/stocks/screener/value_stocks.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/styles/default/Consolas.ttf` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/styles/default/Consolas.ttf`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/styles/default/dark.mpfstyle.json` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/styles/default/dark.mpfstyle.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/styles/default/dark.mplstyle` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/styles/default/dark.mplstyle`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/styles/default/dark.pltstyle.json` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/styles/default/dark.pltstyle.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/styles/default/light.mpfstyle.json` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/styles/default/light.mpfstyle.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/styles/default/light.mplstyle` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/styles/default/light.mplstyle`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/styles/default/light.pltstyle.json` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/styles/default/light.pltstyle.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/miscellaneous/styles/default/tables.pltstyle.json` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/miscellaneous/styles/default/tables.pltstyle.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/mutual_funds/avanza_fund_ID.csv` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/mutual_funds/avanza_fund_ID.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/mutual_funds/avanza_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/mutual_funds/avanza_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/mutual_funds/avanza_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/mutual_funds/avanza_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/mutual_funds/mstarpy_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/mutual_funds/mstarpy_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/mutual_funds/mstarpy_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/mutual_funds/mstarpy_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/mutual_funds/mutual_fund_controller.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/mutual_funds/mutual_fund_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/mutual_funds/mutual_funds_utils.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/mutual_funds/mutual_funds_utils.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/parent_classes.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/parent_classes.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/portfolio/allocation_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/portfolio/allocation_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/portfolio/attribution_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/portfolio/attribution_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/portfolio/brokers/bro_controller.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/portfolio/brokers/bro_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/portfolio/brokers/brokers_helpers.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/portfolio/brokers/brokers_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/portfolio/brokers/coinbase/coinbase_controller.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/portfolio/brokers/coinbase/coinbase_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/portfolio/brokers/coinbase/coinbase_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/portfolio/brokers/coinbase/coinbase_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/portfolio/brokers/coinbase/coinbase_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/portfolio/brokers/coinbase/coinbase_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/portfolio/brokers/degiro/README.md` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/portfolio/brokers/degiro/README.md`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/portfolio/brokers/degiro/degiro_controller.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/portfolio/brokers/degiro/degiro_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/portfolio/brokers/degiro/degiro_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/portfolio/brokers/degiro/degiro_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/portfolio/brokers/degiro/degiro_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/portfolio/brokers/degiro/degiro_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/portfolio/brokers/robinhood/robinhood_controller.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/portfolio/brokers/robinhood/robinhood_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/portfolio/brokers/robinhood/robinhood_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/portfolio/brokers/robinhood/robinhood_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/portfolio/brokers/robinhood/robinhood_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/portfolio/brokers/robinhood/robinhood_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/portfolio/metrics_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/portfolio/metrics_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/portfolio/portfolio_controller.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/portfolio/portfolio_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/portfolio/portfolio_engine.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/portfolio/portfolio_engine.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/portfolio/portfolio_helper.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/portfolio/portfolio_helper.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/portfolio/portfolio_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/portfolio/portfolio_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/portfolio/portfolio_optimization/excel_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/portfolio/portfolio_optimization/excel_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/portfolio/portfolio_optimization/optimizer_helper.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/portfolio/portfolio_optimization/optimizer_helper.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/portfolio/portfolio_optimization/optimizer_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/portfolio/portfolio_optimization/optimizer_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/portfolio/portfolio_optimization/optimizer_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/portfolio/portfolio_optimization/optimizer_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/portfolio/portfolio_optimization/parameters/Parameter.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/portfolio/portfolio_optimization/parameters/Parameter.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/portfolio/portfolio_optimization/parameters/params_controller.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/portfolio/portfolio_optimization/parameters/params_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/portfolio/portfolio_optimization/parameters/params_helpers.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/portfolio/portfolio_optimization/parameters/params_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/portfolio/portfolio_optimization/parameters/params_statics.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/portfolio/portfolio_optimization/parameters/params_statics.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/portfolio/portfolio_optimization/parameters/params_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/portfolio/portfolio_optimization/parameters/params_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/portfolio/portfolio_optimization/po_controller.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/portfolio/portfolio_optimization/po_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/portfolio/portfolio_optimization/po_engine.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/portfolio/portfolio_optimization/po_engine.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/portfolio/portfolio_optimization/po_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/portfolio/portfolio_optimization/po_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/portfolio/portfolio_optimization/po_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/portfolio/portfolio_optimization/po_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/portfolio/portfolio_optimization/statics.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/portfolio/portfolio_optimization/statics.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/portfolio/portfolio_optimization/yahoo_finance_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/portfolio/portfolio_optimization/yahoo_finance_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/portfolio/portfolio_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/portfolio/portfolio_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/portfolio/statics.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/portfolio/statics.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/reporting.md` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/reporting.md`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/reports/.ipynb_checkpoints/test-checkpoint.html` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/reports/.ipynb_checkpoints/test-checkpoint.html`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/reports/README.md` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/reports/README.md`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/reports/reports_controller.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/reports/reports_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/reports/reports_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/reports/reports_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/reports/stored/20220512_040312_equity_NVDA.html` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/reports/stored/20220512_040312_equity_NVDA.html`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/reports/templates/OpenBB_reports_logo.png` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/reports/templates/OpenBB_reports_logo.png`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/reports/templates/crypto.ipynb` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/reports/templates/crypto.ipynb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/reports/templates/economy.ipynb` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/reports/templates/economy.ipynb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/reports/templates/equity.ipynb` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/reports/templates/equity.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998619002525253%*

 * *Differences: {"'cells'": "{18: {'source': {insert: [(0, 'df_sec_filings = openbb.stocks.fa.sec(symbol)[\\n'), "*

 * *            '(1, \'    ["Company Name", "Reporting Owner", "Form Type", "Period"]\\n\'), (2, '*

 * *            "'].head(5)\\n')], delete: [3, 2, 1, 0]}}}"}*

```diff
@@ -255,18 +255,17 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "3022130e",
             "metadata": {},
             "outputs": [],
             "source": [
-                "df_sec_filings = openbb.stocks.fa.sec(symbol)[[\"Type\", \"Category\", \"Link\"]].head(5)\n",
-                "df_sec_filings[\"Link\"] = df_sec_filings[\"Link\"].apply(\n",
-                "    lambda x: f'<a href=\"{x}\">{x}</a>'\n",
-                ")\n",
+                "df_sec_filings = openbb.stocks.fa.sec(symbol)[\n",
+                "    [\"Company Name\", \"Reporting Owner\", \"Form Type\", \"Period\"]\n",
+                "].head(5)\n",
                 "df_sec_filings"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "4662b1ac",
```

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/reports/templates/etf.ipynb` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/reports/templates/etf.ipynb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/reports/templates/floppy-disc.png` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/reports/templates/floppy-disc.png`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/reports/templates/forecast.ipynb` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/reports/templates/forecast.ipynb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/reports/templates/forex.ipynb` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/reports/templates/forex.ipynb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/reports/templates/portfolio.ipynb` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/reports/templates/portfolio.ipynb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/reports/widget_helpers.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/reports/widget_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/reports/widgets/report.css` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/reports/widgets/report.css`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/reports/widgets/style.css` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/reports/widgets/style.css`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/rich_config.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/rich_config.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/sdk.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/sdk.py`

 * *Files 0% similar despite different names*

```diff
@@ -169,15 +169,14 @@
             `revenue`: Governments collect revenues mainly for two purposes: to finance the goods\n
             `revenue_chart`: Governments collect revenues mainly for two purposes: to finance the goods\n
             `rgdp`: Gross domestic product (GDP) is the standard measure of the value added\n
             `rgdp_chart`: Gross domestic product (GDP) is the standard measure of the value added\n
             `rtps`: Get real-time performance sector data\n
             `rtps_chart`: Display Real-Time Performance sector. [Source: AlphaVantage]\n
             `search_index`: Search indices by keyword. [Source: FinanceDatabase]\n
-            `spectrum`: Display finviz spectrum in system viewer [Source: Finviz]\n
             `spending`: General government spending provides an indication of the size\n
             `spending_chart`: General government spending provides an indication of the size\n
             `treasury`: Get U.S. Treasury rates [Source: EconDB]\n
             `treasury_chart`: Display U.S. Treasury rates [Source: EconDB]\n
             `treasury_maturities`: Get treasury maturity options [Source: EconDB]\n
             `trust`: Trust in government refers to the share of people who report having confidence in\n
             `trust_chart`: Trust in government refers to the share of people who report having confidence in\n
```

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/settings_controller.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/settings_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,21 +47,22 @@
 logger = logging.getLogger(__name__)
 
 
 class SettingsController(BaseController):
     """Settings Controller class"""
 
     CHOICES_COMMANDS: List[str] = [
+        "chart",
         "colors",
         "dt",
         "flair",
         "height",
         "lang",
+        "table",
         "tbnews",
-        "theme",
         "tweetnews",
         "tz",
         "userdata",
         "width",
     ]
     if is_local():
         CHOICES_COMMANDS.append("source")
@@ -130,17 +131,21 @@
         current_user = get_current_user()
 
         mt = MenuText("settings/")
         mt.add_info("_info_")
         mt.add_raw("\n")
         mt.add_setting("dt", current_user.preferences.USE_DATETIME)
         mt.add_raw("\n")
-        mt.add_cmd("theme")
+        mt.add_cmd("chart")
         mt.add_raw("\n")
-        mt.add_param("_theme", current_user.preferences.THEME)
+        mt.add_param("_chart", current_user.preferences.CHART_STYLE)
+        mt.add_raw("\n")
+        mt.add_cmd("table")
+        mt.add_raw("\n")
+        mt.add_param("_table", current_user.preferences.TABLE_STYLE)
         mt.add_raw("\n")
         mt.add_cmd("colors")
         mt.add_raw("\n")
         mt.add_param(
             "_colors", f"{current_user.preferences.RICH_STYLE} -> {self.PREVIEW}"
         )
         mt.add_raw("\n")
@@ -262,48 +267,84 @@
                     type_="settings",
                     auth_header=get_current_user().profile.get_auth_header(),
                 )
                 console.print("")
             console.print("Colors updated.")
 
     @log_start_end(log=logger)
-    def call_theme(self, other_args: List[str]):
+    def call_chart(self, other_args: List[str]):
+        """Process chart command"""
+        parser = argparse.ArgumentParser(
+            add_help=False,
+            formatter_class=argparse.ArgumentDefaultsHelpFormatter,
+            prog="theme",
+            description="Choose chart style.",
+        )
+        parser.add_argument(
+            "-s",
+            "--style",
+            type=str,
+            dest="style",
+            choices=["dark", "light"],
+            help="Choose chart style. If you have a hub account you can change theme "
+            f"here {CHARTS_TABLES_URL}.",
+            required="-h" not in other_args and "--help" not in other_args,
+        )
+        if other_args and "-" not in other_args[0][0]:
+            other_args.insert(0, "-s")
+        ns_parser = self.parse_simple_args(parser, other_args)
+        if ns_parser and ns_parser.style:
+            if is_local():
+                self.set_and_save_preference("CHART_STYLE", ns_parser.style)
+            else:
+                set_preference("CHART_STYLE", ns_parser.style)
+                Hub.upload_config(
+                    key="chart",
+                    value=ns_parser.style,
+                    type_="terminal_style",
+                    auth_header=get_current_user().profile.get_auth_header(),
+                )
+                console.print("")
+            console.print("Chart theme updated.\n")
+
+    @log_start_end(log=logger)
+    def call_table(self, other_args: List[str]):
         """Process theme command"""
         parser = argparse.ArgumentParser(
             add_help=False,
             formatter_class=argparse.ArgumentDefaultsHelpFormatter,
             prog="theme",
-            description="Choose theme style.",
+            description="Choose table style.",
         )
         parser.add_argument(
             "-s",
             "--style",
             type=str,
             dest="style",
             choices=["dark", "light"],
-            help="Choose theme style. If you have a hub account you can change theme "
+            help="Choose table style. If you have a hub account you can change theme "
             f"here {CHARTS_TABLES_URL}.",
             required="-h" not in other_args and "--help" not in other_args,
         )
         if other_args and "-" not in other_args[0][0]:
             other_args.insert(0, "-s")
         ns_parser = self.parse_simple_args(parser, other_args)
         if ns_parser and ns_parser.style:
             if is_local():
-                self.set_and_save_preference("THEME", ns_parser.style)
+                self.set_and_save_preference("TABLE_STYLE", ns_parser.style)
             else:
-                set_preference("THEME", ns_parser.style)
+                set_preference("TABLE_STYLE", ns_parser.style)
                 Hub.upload_config(
-                    key="chart_table",
+                    key="table",
                     value=ns_parser.style,
                     type_="terminal_style",
                     auth_header=get_current_user().profile.get_auth_header(),
                 )
                 console.print("")
-            console.print("Theme updated.\n")
+            console.print("Table theme updated.\n")
 
     @log_start_end(log=logger)
     def call_source(self, other_args: List[str]):
         """Process source command"""
         parser = argparse.ArgumentParser(
             add_help=False,
             formatter_class=argparse.ArgumentDefaultsHelpFormatter,
```

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/sources_controller.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/sources_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/backtesting/bt_controller.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/backtesting/bt_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/backtesting/bt_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/backtesting/bt_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/backtesting/bt_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/backtesting/bt_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/behavioural_analysis/ba_controller.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/behavioural_analysis/ba_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/behavioural_analysis/finnhub_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/behavioural_analysis/finnhub_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/behavioural_analysis/finnhub_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/behavioural_analysis/finnhub_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/cboe_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/cboe_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/cboe_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/cboe_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/comparison_analysis/ca_controller.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/comparison_analysis/ca_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/comparison_analysis/finbrain_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/comparison_analysis/finbrain_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/comparison_analysis/finbrain_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/comparison_analysis/finbrain_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/comparison_analysis/finnhub_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/comparison_analysis/finnhub_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/comparison_analysis/finviz_compare_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/comparison_analysis/finviz_compare_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/comparison_analysis/finviz_compare_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/comparison_analysis/finviz_compare_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/comparison_analysis/marketwatch_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/comparison_analysis/marketwatch_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/comparison_analysis/marketwatch_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/comparison_analysis/marketwatch_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/comparison_analysis/polygon_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/comparison_analysis/polygon_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/comparison_analysis/sdk_helpers.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/comparison_analysis/sdk_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/comparison_analysis/yahoo_finance_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/comparison_analysis/yahoo_finance_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/comparison_analysis/yahoo_finance_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/comparison_analysis/yahoo_finance_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/dark_pool_shorts/dps_controller.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/dark_pool_shorts/dps_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/dark_pool_shorts/finra_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/dark_pool_shorts/finra_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/dark_pool_shorts/finra_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/dark_pool_shorts/finra_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/dark_pool_shorts/ibkr_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/dark_pool_shorts/ibkr_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/dark_pool_shorts/ibkr_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/dark_pool_shorts/ibkr_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/dark_pool_shorts/quandl_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/dark_pool_shorts/quandl_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/dark_pool_shorts/quandl_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/dark_pool_shorts/quandl_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/dark_pool_shorts/sec_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/dark_pool_shorts/sec_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/dark_pool_shorts/sec_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/dark_pool_shorts/sec_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/dark_pool_shorts/shortinterest_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/dark_pool_shorts/shortinterest_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/dark_pool_shorts/shortinterest_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/dark_pool_shorts/shortinterest_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/dark_pool_shorts/stockgrid_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/dark_pool_shorts/stockgrid_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/dark_pool_shorts/stockgrid_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/dark_pool_shorts/stockgrid_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/dark_pool_shorts/stocksera_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/dark_pool_shorts/stocksera_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/dark_pool_shorts/stocksera_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/dark_pool_shorts/stocksera_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/dark_pool_shorts/yahoofinance_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/dark_pool_shorts/yahoofinance_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/dark_pool_shorts/yahoofinance_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/dark_pool_shorts/yahoofinance_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/databento_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/databento_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/discovery/ark_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/discovery/ark_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/discovery/ark_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/discovery/ark_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/discovery/disc_controller.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/discovery/disc_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from openbb_terminal.parent_classes import BaseController
 from openbb_terminal.rich_config import MenuText, console
 from openbb_terminal.stocks import stocks_helper
 from openbb_terminal.stocks.discovery import (
     ark_view,
     finnhub_view,
     finviz_view,
+    fmp_view,
     nasdaq_view,
     seeking_alpha_view,
     shortinterest_view,
     yahoofinance_view,
 )
 
 # pylint:disable=C0302
@@ -37,14 +38,15 @@
 logger = logging.getLogger(__name__)
 
 
 class DiscoveryController(BaseController):
     """Discovery Controller class"""
 
     CHOICES_COMMANDS = [
+        "filings",
         "pipo",
         "fipo",
         "gainers",
         "losers",
         "ugs",
         "gtech",
         "active",
@@ -121,14 +123,15 @@
             choices: dict = self.choices_default
 
             self.completer = NestedCompleter.from_nested_dict(choices)
 
     def print_help(self):
         """Print help"""
         mt = MenuText("stocks/disc/")
+        mt.add_cmd("filings", "FinancialModelingPrep")
         mt.add_cmd("pipo", "Finnhub")
         mt.add_cmd("fipo", "Finnhub")
         mt.add_cmd("gainers", "Yahoo Finance")
         mt.add_cmd("losers", "Yahoo Finance")
         mt.add_cmd("ugs", "Yahoo Finance")
         mt.add_cmd("gtech", "Yahoo Finance")
         mt.add_cmd("active", "Yahoo Finance")
@@ -877,14 +880,53 @@
         )
         if ns_parser:
             nasdaq_view.display_top_retail(
                 limit=ns_parser.limit, export=ns_parser.export
             )
 
     @log_start_end(log=logger)
+    def call_filings(self, other_args: List[str]) -> None:
+        """Process Filings command"""
+        parser = argparse.ArgumentParser(
+            add_help=False,
+            formatter_class=argparse.ArgumentDefaultsHelpFormatter,
+            prog="filings",
+            description="The most-recent filings submitted to the SEC",
+        )
+        parser.add_argument(
+            "-p",
+            "--pages",
+            dest="pages",
+            metavar="pages",
+            type=int,
+            default=1,
+            help="The number of pages to get data from (1000 entries/page; maximum 30 pages)",
+        )
+        parser.add_argument(
+            "-t",
+            "--today",
+            dest="today",
+            action="store_true",
+            default=False,
+            help="Show all filings from today",
+        )
+        if other_args and "-" not in other_args[0][0]:
+            other_args.insert(0, "-l")
+        ns_parser = self.parse_known_args_and_warn(
+            parser,
+            other_args,
+            EXPORT_ONLY_RAW_DATA_ALLOWED,
+            limit=5,
+        )
+        if ns_parser:
+            fmp_view.display_filings(
+                ns_parser.pages, ns_parser.limit, ns_parser.today, ns_parser.export
+            )
+
+    @log_start_end(log=logger)
     def call_heatmap(self, other_args: List[str]):
         """Process heatmap command"""
         parser = argparse.ArgumentParser(
             add_help=False,
             formatter_class=argparse.ArgumentDefaultsHelpFormatter,
             prog="heatmap",
             description="""
```

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/discovery/fidelity_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/discovery/fidelity_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/discovery/fidelity_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/discovery/fidelity_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/discovery/finnhub_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/discovery/finnhub_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/discovery/finnhub_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/discovery/finnhub_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/discovery/finviz_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/discovery/finviz_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/discovery/finviz_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/discovery/finviz_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/discovery/nasdaq_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/discovery/nasdaq_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/discovery/nasdaq_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/discovery/nasdaq_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/discovery/seeking_alpha_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/discovery/seeking_alpha_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/discovery/seeking_alpha_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/discovery/seeking_alpha_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/discovery/shortinterest_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/discovery/shortinterest_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/discovery/shortinterest_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/discovery/shortinterest_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/discovery/yahoofinance_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/discovery/yahoofinance_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/discovery/yahoofinance_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/discovery/yahoofinance_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/fundamental_analysis/av_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/fundamental_analysis/av_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/fundamental_analysis/av_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/fundamental_analysis/av_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/fundamental_analysis/business_insider_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/fundamental_analysis/business_insider_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/fundamental_analysis/business_insider_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/fundamental_analysis/business_insider_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/fundamental_analysis/csimarket_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/fundamental_analysis/csimarket_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/fundamental_analysis/csimarket_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/fundamental_analysis/csimarket_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/fundamental_analysis/dcf_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/fundamental_analysis/dcf_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/fundamental_analysis/dcf_static.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/fundamental_analysis/dcf_static.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/fundamental_analysis/dcf_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/fundamental_analysis/dcf_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/fundamental_analysis/eclect_us_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/fundamental_analysis/eclect_us_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/fundamental_analysis/eclect_us_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/fundamental_analysis/eclect_us_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/fundamental_analysis/eodhd_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/fundamental_analysis/eodhd_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/fundamental_analysis/eodhd_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/fundamental_analysis/eodhd_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/fundamental_analysis/fa_controller.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/fundamental_analysis/fa_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -1633,23 +1633,31 @@
                 self.ticker = ns_parser.ticker
                 self.custom_load_wrapper([self.ticker])
             if not self.ticker:
                 console.print(no_ticker_message)
                 return
 
             if self.ticker:
-                dcf = dcf_view.CreateExcelFA(
-                    symbol=self.ticker,
-                    beta=ns_parser.beta,
-                    audit=ns_parser.audit,
-                    ratios=ns_parser.ratios,
-                    len_pred=ns_parser.prediction,
-                    max_similars=ns_parser.similar,
-                    growth=ns_parser.growth,
-                )
+                try:
+                    dcf = dcf_view.CreateExcelFA(
+                        symbol=self.ticker,
+                        beta=ns_parser.beta,
+                        audit=ns_parser.audit,
+                        ratios=ns_parser.ratios,
+                        len_pred=ns_parser.prediction,
+                        max_similars=ns_parser.similar,
+                        growth=ns_parser.growth,
+                    )
+                except Exception as e:
+                    logger.exception(e)
+                    console.print(
+                        "[red]Could not properly create the DCF, please make sure you are"
+                        " using a valid, US listed ticker.[/red]"
+                    )
+                    return
                 if dcf and dcf.data:
                     dcf.create_workbook()
             else:
                 console.print("Please use --ticker or load a ticker first.")
 
     @log_start_end(log=logger)
     def call_dcfc(self, other_args: List[str]):
```

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/fundamental_analysis/finnhub_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/fundamental_analysis/finnhub_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/fundamental_analysis/finnhub_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/fundamental_analysis/finnhub_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/fundamental_analysis/finviz_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/fundamental_analysis/finviz_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/fundamental_analysis/finviz_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/fundamental_analysis/finviz_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/fundamental_analysis/fmp_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/fundamental_analysis/fmp_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -746,7 +746,69 @@
             if "Error Message" not in response.json()
             else message + "\n" + response.json()["Error Message"] + ".\n"
         )
         console.print(message)
         return pd.DataFrame()
 
     return pd.DataFrame(response.json())
+
+
+@log_start_end(log=logger)
+@check_api_key(["API_KEY_FINANCIALMODELINGPREP"])
+def get_filings(
+    pages: int = 1,
+) -> pd.DataFrame:
+    """Get SEC Filings RSS feed, disseminated by FMP
+    Parameters
+    ----------
+    pages: range = 1
+        The range of most-rececnt pages to get entries from (1000 per page; maximum of 30 pages)
+    Returns
+    -------
+    df: pd.DataFrame
+        Dataframe of results
+    Examples
+    --------
+    df = openbb.stocks.filings()
+    df = openbb.stocks.filings(pages=30)
+    """
+    current_user = get_current_user()
+    temp = []
+    try:
+        for i in range(pages):
+            temp.append(
+                pd.read_json(
+                    "https://financialmodelingprep.com/api/v3/rss_feed?&page="
+                    f"{i}"
+                    "&apikey="
+                    f"{current_user.credentials.API_KEY_FINANCIALMODELINGPREP}"
+                )
+            )
+        df = pd.concat(temp)
+        df = df.rename(
+            columns={
+                "title": "Title",
+                "date": "Date",
+                "link": "URL",
+                "cik": "CIK",
+                "form_type": "Form Type",
+                "ticker": "Ticker",
+            },
+        )
+        df_columns = ["Date", "Ticker", "CIK", "Form Type", "Title", "URL"]
+        df = (
+            pd.DataFrame(df, columns=df_columns)
+            .set_index(keys=["Date"])
+            .copy()
+            .sort_index(ascending=False)
+        )
+
+        # Invalid API Keys
+    except ValueError as e:
+        console.print(e)
+        df = pd.DataFrame()
+        # Premium feature, API plan is not authorized
+    except HTTPError as e:
+        console.print(e)
+        df = pd.DataFrame()
+
+    return df
```

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/fundamental_analysis/fmp_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/fundamental_analysis/fmp_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/fundamental_analysis/key_metrics_explained.txt` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/fundamental_analysis/key_metrics_explained.txt`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/fundamental_analysis/marketwatch_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/fundamental_analysis/marketwatch_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/fundamental_analysis/marketwatch_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/fundamental_analysis/marketwatch_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/fundamental_analysis/polygon_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/fundamental_analysis/polygon_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/fundamental_analysis/polygon_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/fundamental_analysis/polygon_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/fundamental_analysis/sdk_helpers.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/fundamental_analysis/sdk_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/fundamental_analysis/seeking_alpha_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/fundamental_analysis/seeking_alpha_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/fundamental_analysis/seeking_alpha_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/fundamental_analysis/seeking_alpha_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/fundamental_analysis/yahoo_finance_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/fundamental_analysis/yahoo_finance_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/fundamental_analysis/yahoo_finance_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/fundamental_analysis/yahoo_finance_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/government/gov_controller.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/government/gov_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/government/quiverquant_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/government/quiverquant_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/government/quiverquant_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/government/quiverquant_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/insider/businessinsider_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/insider/businessinsider_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/insider/businessinsider_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/insider/businessinsider_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/insider/finviz_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/insider/finviz_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/insider/finviz_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/insider/finviz_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/insider/insider_controller.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/insider/insider_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/insider/openinsider_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/insider/openinsider_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/insider/openinsider_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/insider/openinsider_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/insider/sdk_helper.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/insider/sdk_helper.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/mappings/Mic_Codes.csv` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/mappings/Mic_Codes.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/options/alphaquery_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/options/alphaquery_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/options/alphaquery_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/options/alphaquery_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/options/barchart_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/options/barchart_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/options/barchart_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/options/barchart_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/options/calculator_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/options/calculator_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/options/calculator_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/options/calculator_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/options/chartexchange_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/options/chartexchange_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/options/chartexchange_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/options/chartexchange_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/options/fdscanner_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/options/fdscanner_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/options/fdscanner_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/options/fdscanner_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/options/hedge/hedge_controller.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/options/hedge/hedge_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/options/hedge/hedge_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/options/hedge/hedge_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/options/hedge/hedge_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/options/hedge/hedge_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/options/intrinio_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/options/intrinio_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/options/intrinio_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/options/intrinio_view.py`

 * *Files 14% similar despite different names*

```diff
@@ -190,15 +190,15 @@
         horizontal_spacing=0.1,
     )
     fig.set_title(title)
 
     fig.add_scatter(
         x=df.index,
         y=df.price.values,
-        name="Stock Price",
+        name="Option Premium",
         line=dict(color=theme.down_color),
         secondary_y=False,
     )
     fig.add_scatter(
         x=df.index,
         y=df[greek.lower()].values,
         name=greek.title(),
@@ -210,15 +210,15 @@
         yaxis2=dict(
             side="left",
             title=greek,
             anchor="x",
             overlaying="y",
         ),
         yaxis=dict(
-            title=f"{symbol} Price",
+            title=f"{symbol} Option Premium",
             side="right",
         ),
     )
     fig.hide_holidays()
 
     export_data(
         export,
```

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/options/nasdaq_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/options/nasdaq_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/options/op_helpers.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/options/op_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/options/options_controller.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/options/options_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/options/options_sdk_helper.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/options/options_sdk_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,27 +54,28 @@
 
     To get a specific expiration date, use the expiration parameter
 
     >>> aapl_chain_date = openbb.stocks.options.chains("AAPL", expiration="2023-07-21", source="Nasdaq")
     """
 
     source = re.sub(r"\s+", "", source.lower())
+    df = pd.DataFrame()
     if source == "tradier":
         df = tradier_model.get_full_option_chain(symbol)
 
     elif source == "nasdaq":
         df = nasdaq_model.get_full_option_chain(symbol)
 
     elif source == "yahoofinance":
         df = yfinance_model.get_full_option_chain(symbol)
 
     elif source == "intrinio":
         df = intrinio_model.get_full_option_chain(symbol)
 
-    if (df := None) is None:
+    if not isinstance(df, pd.DataFrame) or df.empty:
         logger.info("Invalid Source or Symbol")
         console.print("Invalid Source or Symbol")
         return pd.DataFrame()
 
     if expiration:
         df = df[df.expiration == expiration]
 
@@ -102,22 +103,23 @@
     Examples
     --------
     >>> from openbb_terminal.sdk import openbb
     >>> aapl_price = openbb.stocks.options.price("AAPL", source="Nasdaq")
     """
 
     source = re.sub(r"\s+", "", source.lower())
+    output = None
     if source == "tradier":
         output = tradier_model.get_last_price(symbol)
     if source == "nasdaq":
         output = nasdaq_model.get_last_price(symbol)
     if source == "yahoofinance":
         output = yfinance_model.get_last_price(symbol)
 
-    if (output := None) is None:
+    if not output:
         logger.info("Invalid Source or Symbol")
         console.print("Invalid Source or Symbol")
         return 0.0
 
     return output
 
 
@@ -138,26 +140,26 @@
         Dataframe of full option chain.
 
     Examples
     --------
     >>> from openbb_terminal.sdk import openbb
     >>> SPX_expirations = openbb.stocks.options.expirations("SPX", source = "Tradier")
     """
-
     source = re.sub(r"\s+", "", source.lower())
+    output = []
     if source == "tradier":
         output = tradier_model.option_expirations(symbol)
     if source == "yahoofinance":
         output = yfinance_model.option_expirations(symbol)
     if source == "nasdaq":
         output = nasdaq_model.option_expirations(symbol)
     if source == "intrinio":
         output = intrinio_model.get_expiration_dates(symbol)
 
-    if (output := None) is None:
+    if not output:
         logger.info("Invalid Source or Symbol")
         console.print("Invalid Source or Symbol")
         return []
 
     return output
 
 
@@ -196,23 +198,24 @@
 
     Because this generates a dataframe, we can easily plot the close price for a SPY put:
     (Note that Tradier requires an API key)
     >>> openbb.stocks.options.hist("SPY", "2022-11-18", 400, call=False, source="Tradier").plot(y="close")
     """
 
     source = re.sub(r"\s+", "", source.lower())
+    output = pd.DataFrame()
     if source == "chartexchange":
         output = chartexchange_model.get_option_history(symbol, exp, call, strike)
     if source == "tradier":
         output = tradier_model.get_historical_options(symbol, exp, strike, not call)
     if source == "intrinio":
         occ_symbol = f"{symbol}{''.join(exp[2:].split('-'))}{'C' if call else 'P'}{str(int(1000*strike)).zfill(8)}"
         output = intrinio_model.get_historical_options(occ_symbol)
 
-    if (output := None) is None:
+    if not isinstance(output, pd.DataFrame) or output.empty:
         logger.info("No data found for symbol, check symbol and expiration date")
         console.print("No data found for symbol, check symbol and expiration date")
         return pd.DataFrame()
 
     return output
```

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/options/options_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/options/options_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/options/screen/screener_controller.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/options/screen/screener_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/options/screen/syncretism_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/options/screen/syncretism_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/options/screen/syncretism_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/options/screen/syncretism_view.py`

 * *Files 3% similar despite different names*

```diff
@@ -174,16 +174,16 @@
         vertical_spacing=0.06,
     )
     fig.set_title(
         f"{(greek).capitalize()} historical for {symbol.upper()} {strike} {['Call','Put'][put]}"
     )
     fig.add_scatter(
         x=df.index,
-        y=df.price.values,
-        name="Stock Price",
+        y=df.premium.values,
+        name="Option Premium",
         line=dict(color=theme.down_color),
         connectgaps=True,
         secondary_y=False,
     )
     fig.add_scatter(
         x=df.index,
         y=df[greek.lower()].values,
@@ -197,15 +197,15 @@
         margin=dict(t=30),
         yaxis2=dict(
             side="left",
             title=greek,
             overlaying="y",
         ),
         yaxis=dict(
-            title=f"{symbol} Price",
+            title=f"{symbol} Option Premium",
         ),
     )
 
     export_data(
         export,
         os.path.dirname(os.path.abspath(__file__)),
         "grhist",
```

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/options/tradier_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/options/tradier_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/options/tradier_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/options/tradier_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/options/yfinance_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/options/yfinance_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/options/yfinance_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/options/yfinance_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/quantitative_analysis/beta_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/quantitative_analysis/beta_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/quantitative_analysis/beta_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/quantitative_analysis/beta_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/quantitative_analysis/factors_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/quantitative_analysis/factors_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/quantitative_analysis/factors_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/quantitative_analysis/factors_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/quantitative_analysis/qa_controller.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/quantitative_analysis/qa_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/research/res_controller.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/research/res_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/screener/finviz_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/screener/finviz_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/screener/finviz_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/screener/finviz_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/screener/screener_controller.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/screener/screener_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/screener/screener_helper.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/screener/screener_helper.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/screener/screener_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/screener/screener_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/stock_statics.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/stock_statics.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/stocks_controller.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/stocks_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/stocks_helper.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/stocks_helper.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/stocks_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/stocks_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/stocks_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/stocks_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/technical_analysis/finbrain_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/technical_analysis/finbrain_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/technical_analysis/finbrain_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/technical_analysis/finbrain_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/technical_analysis/rsp_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/technical_analysis/rsp_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/technical_analysis/rsp_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/technical_analysis/rsp_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/technical_analysis/ta_controller.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/technical_analysis/ta_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,14 @@
     valid_date,
 )
 from openbb_terminal.menu import session
 from openbb_terminal.parent_classes import StockBaseController
 from openbb_terminal.rich_config import MenuText, console
 from openbb_terminal.stocks.technical_analysis import (
     finbrain_view,
-    finviz_view,
     rsp_view,
     tradingview_model,
     tradingview_view,
 )
 
 logger = logging.getLogger(__name__)
 
@@ -82,15 +81,14 @@
         "obv",
         "fib",
         "clenow",
         "demark",
         "atr",
         "multi",
         "cones",
-        "view",
     ]
     PATH = "/stocks/ta/"
     CHOICES_GENERATION = True
 
     def __init__(
         self,
         ticker: str,
@@ -135,15 +133,14 @@
         mt.add_raw("\n")
         mt.add_param(
             "_ticker", stock_str if not self.stock.empty else "No ticker loaded"
         )
         mt.add_raw("\n")
         mt.add_cmd("recom", not self.stock.empty)
         mt.add_cmd("summary", not self.stock.empty)
-        mt.add_cmd("view", not self.stock.empty)
         mt.add_raw("\n")
         mt.add_info("_overlap_")
         mt.add_cmd("ema", not self.stock.empty)
         mt.add_cmd("hma", not self.stock.empty)
         mt.add_cmd("sma", not self.stock.empty)
         mt.add_cmd("wma", not self.stock.empty)
         mt.add_cmd("vwap", not self.stock.empty)
@@ -178,33 +175,14 @@
 
     def custom_reset(self):
         """Class specific component of reset command"""
         if self.ticker:
             return ["stocks", f"load {self.ticker}", "ta"]
         return []
 
-    # SPECIFIC
-    @log_start_end(log=logger)
-    def call_view(self, other_args: List[str]):
-        """Process view command"""
-        parser = argparse.ArgumentParser(
-            add_help=False,
-            formatter_class=argparse.ArgumentDefaultsHelpFormatter,
-            prog="view",
-            description="""View historical price with trendlines. [Source: Finviz]""",
-        )
-        ns_parser = self.parse_known_args_and_warn(
-            parser, other_args, EXPORT_ONLY_FIGURES_ALLOWED
-        )
-        if ns_parser:
-            if not self.ticker:
-                no_ticker_message()
-                return
-            finviz_view.view(self.ticker)
-
     @log_start_end(log=logger)
     def call_summary(self, other_args: List[str]):
         """Process summary command"""
         parser = argparse.ArgumentParser(
             add_help=False,
             formatter_class=argparse.ArgumentDefaultsHelpFormatter,
             prog="summary",
```

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/technical_analysis/tradingview_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/technical_analysis/tradingview_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/technical_analysis/tradingview_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/technical_analysis/tradingview_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/tradinghours/bursa_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/tradinghours/bursa_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/tradinghours/bursa_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/tradinghours/bursa_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/tradinghours/data/bursa_open_hours.json` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/tradinghours/data/bursa_open_hours.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/tradinghours/pandas_market_cal_model.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/tradinghours/pandas_market_cal_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/tradinghours/pandas_market_cal_view.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/tradinghours/pandas_market_cal_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/tradinghours/tradinghours_controller.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/tradinghours/tradinghours_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/stocks/tradinghours/tradinghours_helper.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/stocks/tradinghours/tradinghours_helper.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/terminal_controller.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/terminal_controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -500,15 +500,15 @@
 
         self.queue = self.load_class(FundController, self.queue)
 
     def call_intro(self, _):
         """Process intro command."""
         import json
 
-        intro: dict = json.load((Path(__file__).parent / "intro.json").open())
+        intro: dict = json.load((Path(__file__).parent / "intro.json").open())  # type: ignore
 
         for prompt in intro.get("prompts", []):
             console.print(panel.Panel(f"[purple]{prompt['header']}[/purple]"))
             console.print("".join(prompt["content"]))
             if input("") == "q":
                 break
             console.print("\n")
```

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/terminal_helper.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/terminal_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 import matplotlib.pyplot as plt
 
 # IMPORTATION THIRDPARTY
 from packaging import version
 
 from openbb_terminal import thought_of_the_day as thought
+from openbb_terminal.base_helpers import load_env_files
 
 # IMPORTATION INTERNAL
 from openbb_terminal.core.config.paths import SETTINGS_ENV_FILE
 from openbb_terminal.core.plots.backend import plots_backend
 from openbb_terminal.core.session.constants import REGISTER_URL
 from openbb_terminal.core.session.current_system import get_current_system
 from openbb_terminal.core.session.current_user import (
@@ -363,14 +364,15 @@
 def reset(queue: Optional[List[str]] = None):
     """Resets the terminal.  Allows for checking code or keys without quitting"""
     console.print("resetting...")
     logger.info("resetting")
     plt.close("all")
     plots_backend().close(reset=True)
     debug = get_current_system().DEBUG_MODE
+    load_env_files()
 
     # we clear all openbb_terminal modules from sys.modules
     try:
         for module in list(sys.modules.keys()):
             parts = module.split(".")
             if parts[0] == "openbb_terminal":
                 del sys.modules[module]
```

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/openbb_terminal/thought_of_the_day.py` & `openbb_nightly-3.0.0rc2.dev20230415/openbb_terminal/thought_of_the_day.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/pyproject.toml` & `openbb_nightly-3.0.0rc2.dev20230415/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openbb-nightly"
-version = "3.0.0rc2.dev20230414"
+version = "3.0.0rc2.dev20230415"
 description = "Investment Research for Everyone, Anywhere."
 license = "MIT"
 authors = ["Didier Rodrigues Lopes"]
 packages = [
     { include = "openbb_terminal" },
 ]
 include = ["terminal.py", "openbb_terminal/.env"]
```

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/terminal.py` & `openbb_nightly-3.0.0rc2.dev20230415/terminal.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/website/pypi.md` & `openbb_nightly-3.0.0rc2.dev20230415/website/pypi.md`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 If you wish to utilize our **Portfolio Optimization** or **Machine Learning / Artificial Intelligence** toolkits, please see instructions [here](https://docs.openbb.co/sdk/installation).
 
 ## Usage
 
 Access our fully fledged financial SDK with a single line of python code.
 
 ```python
-from openbb_terminal.sdk import openbb-nightly
+from openbb_terminal.sdk import openbb
 ```
 
 Everything you need to use the OpenBB SDK can be found on our [Official Documentation](https://docs.openbb.co/sdk).
 
 Main uses cases can be seen below.
 ___
```

### Comparing `openbb_nightly-3.0.0rc2.dev20230414/PKG-INFO` & `openbb_nightly-3.0.0rc2.dev20230415/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openbb-nightly
-Version: 3.0.0rc2.dev20230414
+Version: 3.0.0rc2.dev20230415
 Summary: Investment Research for Everyone, Anywhere.
 Home-page: https://openbb.co
 License: MIT
 Author: Didier Rodrigues Lopes
 Requires-Python: >=3.8, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.11.*
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -145,15 +145,15 @@
 If you wish to utilize our **Portfolio Optimization** or **Machine Learning / Artificial Intelligence** toolkits, please see instructions [here](https://docs.openbb.co/sdk/installation).
 
 ## Usage
 
 Access our fully fledged financial SDK with a single line of python code.
 
 ```python
-from openbb_terminal.sdk import openbb-nightly
+from openbb_terminal.sdk import openbb
 ```
 
 Everything you need to use the OpenBB SDK can be found on our [Official Documentation](https://docs.openbb.co/sdk).
 
 Main uses cases can be seen below.
 ___
```

