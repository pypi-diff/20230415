# Comparing `tmp/leeger-2.1.1.tar.gz` & `tmp/leeger-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leeger-2.1.1.tar", last modified: Thu Apr 13 04:29:20 2023, max compression
+gzip compressed data, was "leeger-2.2.0.tar", last modified: Sat Apr 15 00:07:34 2023, max compression
```

## Comparing `leeger-2.1.1.tar` & `leeger-2.2.0.tar`

### file list

```diff
@@ -1,207 +1,207 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 04:29:20.814317 leeger-2.1.1/
--rw-rw-rw-   0        0        0     1088 2022-06-10 22:18:01.000000 leeger-2.1.1/LICENSE
--rw-rw-rw-   0        0        0       24 2022-10-18 21:57:01.000000 leeger-2.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     9660 2023-04-13 04:29:20.813316 leeger-2.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     9249 2023-02-16 17:04:27.000000 leeger-2.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 04:29:19.319189 leeger-2.1.1/leeger/
--rw-rw-rw-   0        0        0       43 2022-08-13 05:53:15.000000 leeger-2.1.1/leeger/__init__.py
--rw-rw-rw-   0        0        0       98 2023-04-13 04:27:09.000000 leeger-2.1.1/leeger/_version.py
-drwxrwxrwx   0        0        0        0 2023-04-13 04:29:19.357192 leeger-2.1.1/leeger/calculator/
--rw-rw-rw-   0        0        0        0 2022-08-13 05:53:37.000000 leeger-2.1.1/leeger/calculator/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 04:29:19.464193 leeger-2.1.1/leeger/calculator/all_time_calculator/
--rw-rw-rw-   0        0        0     5439 2022-12-31 03:44:14.000000 leeger-2.1.1/leeger/calculator/all_time_calculator/AWALAllTimeCalculator.py
--rw-rw-rw-   0        0        0     9389 2022-12-31 03:44:14.000000 leeger-2.1.1/leeger/calculator/all_time_calculator/GameOutcomeAllTimeCalculator.py
--rw-rw-rw-   0        0        0     1318 2022-09-03 21:24:19.000000 leeger-2.1.1/leeger/calculator/all_time_calculator/PlusMinusAllTimeCalculator.py
--rw-rw-rw-   0        0        0     4814 2022-12-31 03:44:14.000000 leeger-2.1.1/leeger/calculator/all_time_calculator/PointsScoredAllTimeCalculator.py
--rw-rw-rw-   0        0        0     9374 2022-12-31 03:44:14.000000 leeger-2.1.1/leeger/calculator/all_time_calculator/SSLAllTimeCalculator.py
--rw-rw-rw-   0        0        0     8845 2022-12-31 03:44:14.000000 leeger-2.1.1/leeger/calculator/all_time_calculator/ScoringShareAllTimeCalculator.py
--rw-rw-rw-   0        0        0     2604 2022-12-31 03:44:14.000000 leeger-2.1.1/leeger/calculator/all_time_calculator/ScoringStandardDeviationAllTimeCalculator.py
--rw-rw-rw-   0        0        0     3351 2022-12-31 03:44:14.000000 leeger-2.1.1/leeger/calculator/all_time_calculator/SingleScoreAllTimeCalculator.py
--rw-rw-rw-   0        0        0     9363 2022-12-31 03:44:14.000000 leeger-2.1.1/leeger/calculator/all_time_calculator/SmartWinsAllTimeCalculator.py
--rw-rw-rw-   0        0        0     1521 2022-10-18 21:57:01.000000 leeger-2.1.1/leeger/calculator/all_time_calculator/TeamSummaryAllTimeCalculator.py
--rw-rw-rw-   0        0        0      712 2022-09-20 22:58:18.000000 leeger-2.1.1/leeger/calculator/all_time_calculator/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 04:29:19.493229 leeger-2.1.1/leeger/calculator/parent/
--rw-rw-rw-   0        0        0    14906 2022-12-31 03:44:14.000000 leeger-2.1.1/leeger/calculator/parent/AllTimeCalculator.py
--rw-rw-rw-   0        0        0     1648 2022-12-31 03:23:44.000000 leeger-2.1.1/leeger/calculator/parent/YearCalculator.py
--rw-rw-rw-   0        0        0       94 2022-08-13 05:45:45.000000 leeger-2.1.1/leeger/calculator/parent/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 04:29:19.603228 leeger-2.1.1/leeger/calculator/year_calculator/
--rw-rw-rw-   0        0        0    10079 2023-02-23 03:42:49.000000 leeger-2.1.1/leeger/calculator/year_calculator/AWALYearCalculator.py
--rw-rw-rw-   0        0        0    18904 2022-12-31 03:44:14.000000 leeger-2.1.1/leeger/calculator/year_calculator/GameOutcomeYearCalculator.py
--rw-rw-rw-   0        0        0     1960 2022-12-31 03:23:44.000000 leeger-2.1.1/leeger/calculator/year_calculator/PlusMinusYearCalculator.py
--rw-rw-rw-   0        0        0     6011 2022-12-31 03:23:44.000000 leeger-2.1.1/leeger/calculator/year_calculator/PointsScoredYearCalculator.py
--rw-rw-rw-   0        0        0     6340 2022-12-31 03:23:44.000000 leeger-2.1.1/leeger/calculator/year_calculator/SSLYearCalculator.py
--rw-rw-rw-   0        0        0     8670 2022-12-31 03:44:14.000000 leeger-2.1.1/leeger/calculator/year_calculator/ScoringShareYearCalculator.py
--rw-rw-rw-   0        0        0     2396 2022-12-31 03:23:44.000000 leeger-2.1.1/leeger/calculator/year_calculator/ScoringStandardDeviationYearCalculator.py
--rw-rw-rw-   0        0        0     2973 2022-12-31 03:23:44.000000 leeger-2.1.1/leeger/calculator/year_calculator/SingleScoreYearCalculator.py
--rw-rw-rw-   0        0        0     8583 2022-12-31 03:23:44.000000 leeger-2.1.1/leeger/calculator/year_calculator/SmartWinsYearCalculator.py
--rw-rw-rw-   0        0        0     1675 2022-12-31 03:23:44.000000 leeger-2.1.1/leeger/calculator/year_calculator/TeamSummaryYearCalculator.py
--rw-rw-rw-   0        0        0      652 2022-09-20 22:58:18.000000 leeger-2.1.1/leeger/calculator/year_calculator/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 04:29:19.626227 leeger-2.1.1/leeger/decorator/
--rw-rw-rw-   0        0        0       85 2022-08-13 05:53:57.000000 leeger-2.1.1/leeger/decorator/__init__.py
--rw-rw-rw-   0        0        0     4853 2023-02-23 03:42:49.000000 leeger-2.1.1/leeger/decorator/validators.py
-drwxrwxrwx   0        0        0        0 2023-04-13 04:29:19.643235 leeger-2.1.1/leeger/enum/
--rw-rw-rw-   0        0        0      782 2023-02-17 18:57:53.000000 leeger-2.1.1/leeger/enum/MatchupType.py
--rw-rw-rw-   0        0        0       38 2022-09-29 19:44:58.000000 leeger-2.1.1/leeger/enum/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 04:29:19.743242 leeger-2.1.1/leeger/exception/
--rw-rw-rw-   0        0        0      157 2022-06-10 22:18:01.000000 leeger-2.1.1/leeger/exception/DoesNotExistException.py
--rw-rw-rw-   0        0        0      117 2022-06-10 22:18:01.000000 leeger-2.1.1/leeger/exception/InvalidFilterException.py
--rw-rw-rw-   0        0        0      138 2022-06-10 22:18:01.000000 leeger-2.1.1/leeger/exception/InvalidLeagueFormatException.py
--rw-rw-rw-   0        0        0      140 2022-06-10 22:18:01.000000 leeger-2.1.1/leeger/exception/InvalidMatchupFormatException.py
--rw-rw-rw-   0        0        0      137 2022-06-10 22:18:01.000000 leeger-2.1.1/leeger/exception/InvalidOwnerFormatException.py
--rw-rw-rw-   0        0        0      134 2022-06-10 22:18:01.000000 leeger-2.1.1/leeger/exception/InvalidTeamFormatException.py
--rw-rw-rw-   0        0        0      134 2022-06-10 22:18:01.000000 leeger-2.1.1/leeger/exception/InvalidWeekFormatException.py
--rw-rw-rw-   0        0        0      134 2022-06-10 22:18:01.000000 leeger-2.1.1/leeger/exception/InvalidYearFormatException.py
--rw-rw-rw-   0        0        0      150 2022-10-16 01:33:13.000000 leeger-2.1.1/leeger/exception/InvalidYearSettingsFormatException.py
--rw-rw-rw-   0        0        0      124 2022-08-08 22:25:46.000000 leeger-2.1.1/leeger/exception/LeagueLoaderException.py
--rw-rw-rw-   0        0        0      134 2022-09-17 17:22:58.000000 leeger-2.1.1/leeger/exception/UnsupportedLeegerFeatureException.py
--rw-rw-rw-   0        0        0      762 2022-10-16 01:33:13.000000 leeger-2.1.1/leeger/exception/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 04:29:19.768396 leeger-2.1.1/leeger/league_loader/
--rw-rw-rw-   0        0        0     8513 2023-02-28 02:34:18.000000 leeger-2.1.1/leeger/league_loader/ESPNLeagueLoader.py
--rw-rw-rw-   0        0        0     7803 2023-02-28 02:34:18.000000 leeger-2.1.1/leeger/league_loader/FleaflickerLeagueLoader.py
--rw-rw-rw-   0        0        0     2549 2023-02-28 02:34:18.000000 leeger-2.1.1/leeger/league_loader/LeagueLoader.py
--rw-rw-rw-   0        0        0    12476 2023-02-28 02:34:18.000000 leeger-2.1.1/leeger/league_loader/MyFantasyLeagueLeagueLoader.py
--rw-rw-rw-   0        0        0    15271 2023-02-28 02:34:18.000000 leeger-2.1.1/leeger/league_loader/SleeperLeagueLoader.py
--rw-rw-rw-   0        0        0    10706 2023-02-28 02:34:18.000000 leeger-2.1.1/leeger/league_loader/YahooLeagueLoader.py
--rw-rw-rw-   0        0        0      222 2022-08-08 20:13:25.000000 leeger-2.1.1/leeger/league_loader/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 04:29:19.772395 leeger-2.1.1/leeger/model/
--rw-rw-rw-   0        0        0        0 2022-08-13 05:54:09.000000 leeger-2.1.1/leeger/model/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 04:29:19.789392 leeger-2.1.1/leeger/model/abstract/
--rw-rw-rw-   0        0        0      550 2023-02-17 18:45:58.000000 leeger-2.1.1/leeger/model/abstract/UniqueId.py
--rw-rw-rw-   0        0        0       32 2022-08-13 05:49:03.000000 leeger-2.1.1/leeger/model/abstract/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 04:29:19.828393 leeger-2.1.1/leeger/model/filter/
--rw-rw-rw-   0        0        0     5502 2023-01-05 20:28:10.000000 leeger-2.1.1/leeger/model/filter/AllTimeFilters.py
--rw-rw-rw-   0        0        0      319 2022-07-13 01:00:45.000000 leeger-2.1.1/leeger/model/filter/WeekFilters.py
--rw-rw-rw-   0        0        0     5110 2023-01-05 20:28:10.000000 leeger-2.1.1/leeger/model/filter/YearFilters.py
--rw-rw-rw-   0        0        0      120 2022-09-17 18:26:39.000000 leeger-2.1.1/leeger/model/filter/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 04:29:19.905394 leeger-2.1.1/leeger/model/league/
--rw-rw-rw-   0        0        0     5600 2023-02-17 18:45:58.000000 leeger-2.1.1/leeger/model/league/League.py
--rw-rw-rw-   0        0        0     4825 2023-02-17 19:22:16.000000 leeger-2.1.1/leeger/model/league/Matchup.py
--rw-rw-rw-   0        0        0      880 2023-02-17 18:45:58.000000 leeger-2.1.1/leeger/model/league/Owner.py
--rw-rw-rw-   0        0        0     1481 2023-02-17 18:54:16.000000 leeger-2.1.1/leeger/model/league/Team.py
--rw-rw-rw-   0        0        0     2780 2023-02-17 18:54:16.000000 leeger-2.1.1/leeger/model/league/Week.py
--rw-rw-rw-   0        0        0     2816 2023-02-17 19:02:21.000000 leeger-2.1.1/leeger/model/league/Year.py
--rw-rw-rw-   0        0        0      999 2023-02-17 19:34:53.000000 leeger-2.1.1/leeger/model/league/YearSettings.py
--rw-rw-rw-   0        0        0      196 2022-10-16 01:33:13.000000 leeger-2.1.1/leeger/model/league/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 04:29:19.917392 leeger-2.1.1/leeger/model/league_helper/
--rw-rw-rw-   0        0        0     3657 2023-01-04 01:53:09.000000 leeger-2.1.1/leeger/model/league_helper/Performance.py
--rw-rw-rw-   0        0        0        0 2023-01-04 01:53:09.000000 leeger-2.1.1/leeger/model/league_helper/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 04:29:19.945395 leeger-2.1.1/leeger/model/stat/
--rw-rw-rw-   0        0        0     3891 2022-11-01 16:02:18.000000 leeger-2.1.1/leeger/model/stat/AllTimeStatSheet.py
--rw-rw-rw-   0        0        0     4125 2023-01-02 01:43:27.000000 leeger-2.1.1/leeger/model/stat/YearStatSheet.py
--rw-rw-rw-   0        0        0       90 2022-08-13 05:49:50.000000 leeger-2.1.1/leeger/model/stat/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 04:29:20.048276 leeger-2.1.1/leeger/util/
--rw-rw-rw-   0        0        0     1113 2022-07-31 17:54:53.000000 leeger-2.1.1/leeger/util/CustomFormatter.py
--rw-rw-rw-   0        0        0      859 2022-07-31 17:55:05.000000 leeger-2.1.1/leeger/util/CustomLogger.py
--rw-rw-rw-   0        0        0      513 2022-06-11 23:09:37.000000 leeger-2.1.1/leeger/util/Deci.py
--rw-rw-rw-   0        0        0     1428 2022-12-26 23:36:20.000000 leeger-2.1.1/leeger/util/GeneralUtil.py
--rw-rw-rw-   0        0        0      237 2022-06-10 22:18:01.000000 leeger-2.1.1/leeger/util/IdGenerator.py
--rw-rw-rw-   0        0        0      312 2023-02-17 18:45:58.000000 leeger-2.1.1/leeger/util/JSONDeserializable.py
--rw-rw-rw-   0        0        0      278 2022-09-03 18:23:27.000000 leeger-2.1.1/leeger/util/JSONSerializable.py
--rw-rw-rw-   0        0        0        0 2022-08-13 05:54:20.000000 leeger-2.1.1/leeger/util/__init__.py
--rw-rw-rw-   0        0        0    15100 2023-02-18 07:06:07.000000 leeger-2.1.1/leeger/util/excel.py
--rw-rw-rw-   0        0        0     9301 2023-01-02 01:43:27.000000 leeger-2.1.1/leeger/util/excel_helper.py
-drwxrwxrwx   0        0        0        0 2023-04-13 04:29:20.098294 leeger-2.1.1/leeger/util/navigator/
--rw-rw-rw-   0        0        0     5669 2023-01-05 20:27:34.000000 leeger-2.1.1/leeger/util/navigator/LeagueNavigator.py
--rw-rw-rw-   0        0        0     2100 2022-12-31 03:44:14.000000 leeger-2.1.1/leeger/util/navigator/MatchupNavigator.py
--rw-rw-rw-   0        0        0     2191 2022-12-31 03:44:14.000000 leeger-2.1.1/leeger/util/navigator/WeekNavigator.py
--rw-rw-rw-   0        0        0     6578 2023-01-05 20:27:15.000000 leeger-2.1.1/leeger/util/navigator/YearNavigator.py
--rw-rw-rw-   0        0        0      178 2022-12-31 03:44:14.000000 leeger-2.1.1/leeger/util/navigator/__init__.py
--rw-rw-rw-   0        0        0    11461 2023-01-02 01:43:27.000000 leeger-2.1.1/leeger/util/stat_sheet.py
-drwxrwxrwx   0        0        0        0 2023-04-13 04:29:20.189294 leeger-2.1.1/leeger/validate/
--rw-rw-rw-   0        0        0      258 2022-08-13 06:01:19.000000 leeger-2.1.1/leeger/validate/__init__.py
--rw-rw-rw-   0        0        0     4254 2022-10-25 22:18:55.000000 leeger-2.1.1/leeger/validate/leagueValidation.py
--rw-rw-rw-   0        0        0     2460 2023-01-04 01:53:09.000000 leeger-2.1.1/leeger/validate/matchupValidation.py
--rw-rw-rw-   0        0        0      493 2022-09-13 21:37:08.000000 leeger-2.1.1/leeger/validate/ownerValidation.py
--rw-rw-rw-   0        0        0      598 2022-09-13 21:37:08.000000 leeger-2.1.1/leeger/validate/teamValidation.py
--rw-rw-rw-   0        0        0     4624 2022-09-17 18:26:39.000000 leeger-2.1.1/leeger/validate/weekValidation.py
--rw-rw-rw-   0        0        0      231 2023-02-17 19:20:27.000000 leeger-2.1.1/leeger/validate/yearSettingsValidation.py
--rw-rw-rw-   0        0        0    13147 2023-01-08 17:42:36.000000 leeger-2.1.1/leeger/validate/yearValidation.py
-drwxrwxrwx   0        0        0        0 2023-04-13 04:29:19.355191 leeger-2.1.1/leeger.egg-info/
--rw-rw-rw-   0        0        0     9660 2023-04-13 04:29:18.000000 leeger-2.1.1/leeger.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7779 2023-04-13 04:29:19.000000 leeger-2.1.1/leeger.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 04:29:18.000000 leeger-2.1.1/leeger.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      139 2023-04-13 04:29:18.000000 leeger-2.1.1/leeger.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-13 04:29:18.000000 leeger-2.1.1/leeger.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      147 2023-04-13 04:26:54.000000 leeger-2.1.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-13 04:29:20.814317 leeger-2.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1048 2022-11-03 07:24:35.000000 leeger-2.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-13 04:29:19.292191 leeger-2.1.1/test/
-drwxrwxrwx   0        0        0        0 2023-04-13 04:29:20.192293 leeger-2.1.1/test/test_calculator/
--rw-rw-rw-   0        0        0        0 2022-06-10 22:18:01.000000 leeger-2.1.1/test/test_calculator/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 04:29:20.321299 leeger-2.1.1/test/test_calculator/test_all_time_calculator/
--rw-rw-rw-   0        0        0        0 2022-06-27 00:56:09.000000 leeger-2.1.1/test/test_calculator/test_all_time_calculator/__init__.py
--rw-rw-rw-   0        0        0    84596 2022-10-18 21:57:01.000000 leeger-2.1.1/test/test_calculator/test_all_time_calculator/test_AWALAllTimeCalculator.py
--rw-rw-rw-   0        0        0   202229 2022-10-18 21:57:01.000000 leeger-2.1.1/test/test_calculator/test_all_time_calculator/test_GameOutcomeAllTimeCalculator.py
--rw-rw-rw-   0        0        0    21521 2022-08-12 21:53:32.000000 leeger-2.1.1/test/test_calculator/test_all_time_calculator/test_PlusMinusAllTimeCalculator.py
--rw-rw-rw-   0        0        0    85906 2022-08-12 21:53:32.000000 leeger-2.1.1/test/test_calculator/test_all_time_calculator/test_PointsScoredAllTimeCalculator.py
--rw-rw-rw-   0        0        0    39781 2022-09-20 22:58:18.000000 leeger-2.1.1/test/test_calculator/test_all_time_calculator/test_SSLAllTimeCalculator.py
--rw-rw-rw-   0        0        0    99301 2022-11-01 16:02:18.000000 leeger-2.1.1/test/test_calculator/test_all_time_calculator/test_ScoringShareAllTimeCalculator.py
--rw-rw-rw-   0        0        0    25110 2022-09-17 18:26:39.000000 leeger-2.1.1/test/test_calculator/test_all_time_calculator/test_ScoringStandardDeviationAllTimeCalculator.py
--rw-rw-rw-   0        0        0    41897 2022-08-12 21:53:32.000000 leeger-2.1.1/test/test_calculator/test_all_time_calculator/test_SingleScoreAllTimeCalculator.py
--rw-rw-rw-   0        0        0    96169 2022-09-17 18:26:39.000000 leeger-2.1.1/test/test_calculator/test_all_time_calculator/test_SmartWinsAllTimeCalculator.py
--rw-rw-rw-   0        0        0    49915 2022-10-18 21:57:01.000000 leeger-2.1.1/test/test_calculator/test_all_time_calculator/test_TeamSummaryAllTimeCalculator.py
-drwxrwxrwx   0        0        0        0 2023-04-13 04:29:20.439295 leeger-2.1.1/test/test_calculator/test_year_calculator/
--rw-rw-rw-   0        0        0        0 2022-06-27 00:54:55.000000 leeger-2.1.1/test/test_calculator/test_year_calculator/__init__.py
--rw-rw-rw-   0        0        0    94805 2022-10-18 21:57:01.000000 leeger-2.1.1/test/test_calculator/test_year_calculator/test_AWALYearCalculator.py
--rw-rw-rw-   0        0        0    80359 2022-10-18 21:57:01.000000 leeger-2.1.1/test/test_calculator/test_year_calculator/test_GameOutcomeYearCalculator.py
--rw-rw-rw-   0        0        0     9174 2022-08-12 21:53:32.000000 leeger-2.1.1/test/test_calculator/test_year_calculator/test_PlusMinusYearCalculator.py
--rw-rw-rw-   0        0        0    36598 2022-08-12 21:53:32.000000 leeger-2.1.1/test/test_calculator/test_year_calculator/test_PointsScoredYearCalculator.py
--rw-rw-rw-   0        0        0    28074 2022-09-20 22:58:18.000000 leeger-2.1.1/test/test_calculator/test_year_calculator/test_SSLYearCalculator.py
--rw-rw-rw-   0        0        0    42133 2022-11-01 16:02:18.000000 leeger-2.1.1/test/test_calculator/test_year_calculator/test_ScoringShareYearCalculator.py
--rw-rw-rw-   0        0        0    11387 2022-09-17 18:26:39.000000 leeger-2.1.1/test/test_calculator/test_year_calculator/test_ScoringStandardDeviationYearCalculator.py
--rw-rw-rw-   0        0        0    32261 2022-08-12 21:53:32.000000 leeger-2.1.1/test/test_calculator/test_year_calculator/test_SingleScoreYearCalculator.py
--rw-rw-rw-   0        0        0    75846 2022-09-17 18:26:39.000000 leeger-2.1.1/test/test_calculator/test_year_calculator/test_SmartWinsYearCalculator.py
--rw-rw-rw-   0        0        0    20425 2022-10-18 21:57:01.000000 leeger-2.1.1/test/test_calculator/test_year_calculator/test_TeamSummaryYearCalculator.py
-drwxrwxrwx   0        0        0        0 2023-04-13 04:29:20.451294 leeger-2.1.1/test/test_decorator/
--rw-rw-rw-   0        0        0        0 2022-06-10 22:18:01.000000 leeger-2.1.1/test/test_decorator/__init__.py
--rw-rw-rw-   0        0        0     4605 2023-01-08 17:42:36.000000 leeger-2.1.1/test/test_decorator/test_validators.py
-drwxrwxrwx   0        0        0        0 2023-04-13 04:29:20.506318 leeger-2.1.1/test/test_league_loader/
--rw-rw-rw-   0        0        0        0 2022-06-25 00:07:47.000000 leeger-2.1.1/test/test_league_loader/__init__.py
--rw-rw-rw-   0        0        0     1240 2022-09-20 22:58:18.000000 leeger-2.1.1/test/test_league_loader/test_ESPNLeagueLoader.py
--rw-rw-rw-   0        0        0      409 2022-10-26 20:01:28.000000 leeger-2.1.1/test/test_league_loader/test_FleaflickerLeagueLoader.py
--rw-rw-rw-   0        0        0      851 2022-09-20 22:58:18.000000 leeger-2.1.1/test/test_league_loader/test_MyFantasyLeagueLeagueLoader.py
--rw-rw-rw-   0        0        0      698 2022-09-20 22:58:18.000000 leeger-2.1.1/test/test_league_loader/test_SleeperLeagueLoader.py
--rw-rw-rw-   0        0        0     1462 2022-10-16 21:38:41.000000 leeger-2.1.1/test/test_league_loader/test_YahooLeagueLoader.py
-drwxrwxrwx   0        0        0        0 2023-04-13 04:29:20.509318 leeger-2.1.1/test/test_model/
--rw-rw-rw-   0        0        0        0 2022-06-10 22:18:01.000000 leeger-2.1.1/test/test_model/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 04:29:20.523317 leeger-2.1.1/test/test_model/test_abstract/
--rw-rw-rw-   0        0        0        0 2022-06-10 22:18:01.000000 leeger-2.1.1/test/test_model/test_abstract/__init__.py
--rw-rw-rw-   0        0        0      932 2022-09-19 23:01:23.000000 leeger-2.1.1/test/test_model/test_abstract/test_UniqueId.py
-drwxrwxrwx   0        0        0        0 2023-04-13 04:29:20.537318 leeger-2.1.1/test/test_model/test_filter/
--rw-rw-rw-   0        0        0        0 2022-07-01 18:59:46.000000 leeger-2.1.1/test/test_model/test_filter/__init__.py
--rw-rw-rw-   0        0        0     1814 2022-07-13 01:00:45.000000 leeger-2.1.1/test/test_model/test_filter/test_AllTimeFilters.py
-drwxrwxrwx   0        0        0        0 2023-04-13 04:29:20.626316 leeger-2.1.1/test/test_model/test_league/
--rw-rw-rw-   0        0        0        0 2022-06-23 01:09:11.000000 leeger-2.1.1/test/test_model/test_league/__init__.py
--rw-rw-rw-   0        0        0    20771 2023-02-17 19:27:57.000000 leeger-2.1.1/test/test_model/test_league/test_League.py
--rw-rw-rw-   0        0        0     8841 2023-02-17 19:28:14.000000 leeger-2.1.1/test/test_model/test_league/test_Matchup.py
--rw-rw-rw-   0        0        0     1136 2023-02-17 19:28:57.000000 leeger-2.1.1/test/test_model/test_league/test_Owner.py
--rw-rw-rw-   0        0        0     1219 2023-02-17 19:29:31.000000 leeger-2.1.1/test/test_model/test_league/test_Team.py
--rw-rw-rw-   0        0        0     8811 2023-02-17 19:30:19.000000 leeger-2.1.1/test/test_model/test_league/test_Week.py
--rw-rw-rw-   0        0        0     8343 2023-02-17 19:31:44.000000 leeger-2.1.1/test/test_model/test_league/test_Year.py
--rw-rw-rw-   0        0        0     1487 2023-02-17 19:34:39.000000 leeger-2.1.1/test/test_model/test_league/test_YearSettings.py
-drwxrwxrwx   0        0        0        0 2023-04-13 04:29:20.638317 leeger-2.1.1/test/test_model/test_league_helper/
--rw-rw-rw-   0        0        0        0 2023-01-04 01:53:09.000000 leeger-2.1.1/test/test_model/test_league_helper/__init__.py
--rw-rw-rw-   0        0        0     6585 2023-01-04 01:53:09.000000 leeger-2.1.1/test/test_model/test_league_helper/test_Performance.py
-drwxrwxrwx   0        0        0        0 2023-04-13 04:29:20.693316 leeger-2.1.1/test/test_util/
--rw-rw-rw-   0        0        0        0 2022-06-10 22:18:01.000000 leeger-2.1.1/test/test_util/__init__.py
--rw-rw-rw-   0        0        0      471 2022-07-13 01:00:46.000000 leeger-2.1.1/test/test_util/test_Deci.py
--rw-rw-rw-   0        0        0     1375 2022-12-26 23:36:20.000000 leeger-2.1.1/test/test_util/test_GeneralUtil.py
--rw-rw-rw-   0        0        0      486 2022-07-13 01:00:45.000000 leeger-2.1.1/test/test_util/test_IdGenerator.py
--rw-rw-rw-   0        0        0    39409 2023-02-18 07:06:07.000000 leeger-2.1.1/test/test_util/test_excel.py
--rw-rw-rw-   0        0        0     7319 2023-01-02 01:43:27.000000 leeger-2.1.1/test/test_util/test_excel_helper.py
-drwxrwxrwx   0        0        0        0 2023-04-13 04:29:20.738315 leeger-2.1.1/test/test_util/test_navigator/
--rw-rw-rw-   0        0        0        0 2022-08-12 22:44:07.000000 leeger-2.1.1/test/test_util/test_navigator/__init__.py
--rw-rw-rw-   0        0        0    47293 2022-12-31 03:44:14.000000 leeger-2.1.1/test/test_util/test_navigator/test_LeagueNavigator.py
--rw-rw-rw-   0        0        0     3722 2022-12-31 03:44:14.000000 leeger-2.1.1/test/test_util/test_navigator/test_MatchupNavigator.py
--rw-rw-rw-   0        0        0     5388 2022-12-31 03:44:14.000000 leeger-2.1.1/test/test_util/test_navigator/test_WeekNavigator.py
--rw-rw-rw-   0        0        0    25968 2022-12-31 03:23:44.000000 leeger-2.1.1/test/test_util/test_navigator/test_YearNavigator.py
--rw-rw-rw-   0        0        0    10636 2023-01-02 01:43:27.000000 leeger-2.1.1/test/test_util/test_stat_sheet.py
-drwxrwxrwx   0        0        0        0 2023-04-13 04:29:20.810315 leeger-2.1.1/test/test_validate/
--rw-rw-rw-   0        0        0        0 2022-08-12 22:13:02.000000 leeger-2.1.1/test/test_validate/__init__.py
--rw-rw-rw-   0        0        0     8307 2022-10-13 23:25:46.000000 leeger-2.1.1/test/test_validate/test_leagueValidation.py
--rw-rw-rw-   0        0        0     4032 2023-02-17 19:19:04.000000 leeger-2.1.1/test/test_validate/test_matchupValidation.py
--rw-rw-rw-   0        0        0      532 2022-08-12 21:37:24.000000 leeger-2.1.1/test/test_validate/test_ownerValidation.py
--rw-rw-rw-   0        0        0      840 2022-08-12 21:37:24.000000 leeger-2.1.1/test/test_validate/test_teamValidation.py
--rw-rw-rw-   0        0        0     5494 2022-09-17 18:26:39.000000 leeger-2.1.1/test/test_validate/test_weekValidation.py
--rw-rw-rw-   0        0        0      612 2023-02-17 19:20:44.000000 leeger-2.1.1/test/test_validate/test_yearSettingsValidation.py
--rw-rw-rw-   0        0        0    22836 2023-01-08 17:42:36.000000 leeger-2.1.1/test/test_validate/test_yearValidation.py
+drwxrwxrwx   0        0        0        0 2023-04-15 00:07:34.117948 leeger-2.2.0/
+-rw-rw-rw-   0        0        0     1088 2022-06-10 22:18:01.000000 leeger-2.2.0/LICENSE
+-rw-rw-rw-   0        0        0       24 2022-10-18 21:57:01.000000 leeger-2.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     9660 2023-04-15 00:07:34.116951 leeger-2.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     9249 2023-02-16 17:04:27.000000 leeger-2.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-15 00:07:33.720948 leeger-2.2.0/leeger/
+-rw-rw-rw-   0        0        0       43 2022-08-13 05:53:15.000000 leeger-2.2.0/leeger/__init__.py
+-rw-rw-rw-   0        0        0       98 2023-04-15 00:06:49.000000 leeger-2.2.0/leeger/_version.py
+drwxrwxrwx   0        0        0        0 2023-04-15 00:07:33.759946 leeger-2.2.0/leeger/calculator/
+-rw-rw-rw-   0        0        0        0 2022-08-13 05:53:37.000000 leeger-2.2.0/leeger/calculator/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-15 00:07:33.783948 leeger-2.2.0/leeger/calculator/all_time_calculator/
+-rw-rw-rw-   0        0        0     5439 2022-12-31 03:44:14.000000 leeger-2.2.0/leeger/calculator/all_time_calculator/AWALAllTimeCalculator.py
+-rw-rw-rw-   0        0        0     9389 2022-12-31 03:44:14.000000 leeger-2.2.0/leeger/calculator/all_time_calculator/GameOutcomeAllTimeCalculator.py
+-rw-rw-rw-   0        0        0     1318 2022-09-03 21:24:19.000000 leeger-2.2.0/leeger/calculator/all_time_calculator/PlusMinusAllTimeCalculator.py
+-rw-rw-rw-   0        0        0     4814 2022-12-31 03:44:14.000000 leeger-2.2.0/leeger/calculator/all_time_calculator/PointsScoredAllTimeCalculator.py
+-rw-rw-rw-   0        0        0     9374 2022-12-31 03:44:14.000000 leeger-2.2.0/leeger/calculator/all_time_calculator/SSLAllTimeCalculator.py
+-rw-rw-rw-   0        0        0     8845 2022-12-31 03:44:14.000000 leeger-2.2.0/leeger/calculator/all_time_calculator/ScoringShareAllTimeCalculator.py
+-rw-rw-rw-   0        0        0     2604 2022-12-31 03:44:14.000000 leeger-2.2.0/leeger/calculator/all_time_calculator/ScoringStandardDeviationAllTimeCalculator.py
+-rw-rw-rw-   0        0        0     3351 2022-12-31 03:44:14.000000 leeger-2.2.0/leeger/calculator/all_time_calculator/SingleScoreAllTimeCalculator.py
+-rw-rw-rw-   0        0        0     9363 2022-12-31 03:44:14.000000 leeger-2.2.0/leeger/calculator/all_time_calculator/SmartWinsAllTimeCalculator.py
+-rw-rw-rw-   0        0        0     1521 2022-10-18 21:57:01.000000 leeger-2.2.0/leeger/calculator/all_time_calculator/TeamSummaryAllTimeCalculator.py
+-rw-rw-rw-   0        0        0      712 2022-09-20 22:58:18.000000 leeger-2.2.0/leeger/calculator/all_time_calculator/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-15 00:07:33.790948 leeger-2.2.0/leeger/calculator/parent/
+-rw-rw-rw-   0        0        0    14906 2022-12-31 03:44:14.000000 leeger-2.2.0/leeger/calculator/parent/AllTimeCalculator.py
+-rw-rw-rw-   0        0        0     1648 2022-12-31 03:23:44.000000 leeger-2.2.0/leeger/calculator/parent/YearCalculator.py
+-rw-rw-rw-   0        0        0       94 2022-08-13 05:45:45.000000 leeger-2.2.0/leeger/calculator/parent/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-15 00:07:33.812946 leeger-2.2.0/leeger/calculator/year_calculator/
+-rw-rw-rw-   0        0        0    10079 2023-02-23 03:42:49.000000 leeger-2.2.0/leeger/calculator/year_calculator/AWALYearCalculator.py
+-rw-rw-rw-   0        0        0    18904 2022-12-31 03:44:14.000000 leeger-2.2.0/leeger/calculator/year_calculator/GameOutcomeYearCalculator.py
+-rw-rw-rw-   0        0        0     1960 2022-12-31 03:23:44.000000 leeger-2.2.0/leeger/calculator/year_calculator/PlusMinusYearCalculator.py
+-rw-rw-rw-   0        0        0     6011 2022-12-31 03:23:44.000000 leeger-2.2.0/leeger/calculator/year_calculator/PointsScoredYearCalculator.py
+-rw-rw-rw-   0        0        0     6340 2022-12-31 03:23:44.000000 leeger-2.2.0/leeger/calculator/year_calculator/SSLYearCalculator.py
+-rw-rw-rw-   0        0        0     8670 2022-12-31 03:44:14.000000 leeger-2.2.0/leeger/calculator/year_calculator/ScoringShareYearCalculator.py
+-rw-rw-rw-   0        0        0     2396 2022-12-31 03:23:44.000000 leeger-2.2.0/leeger/calculator/year_calculator/ScoringStandardDeviationYearCalculator.py
+-rw-rw-rw-   0        0        0     2973 2022-12-31 03:23:44.000000 leeger-2.2.0/leeger/calculator/year_calculator/SingleScoreYearCalculator.py
+-rw-rw-rw-   0        0        0     8583 2022-12-31 03:23:44.000000 leeger-2.2.0/leeger/calculator/year_calculator/SmartWinsYearCalculator.py
+-rw-rw-rw-   0        0        0     1675 2022-12-31 03:23:44.000000 leeger-2.2.0/leeger/calculator/year_calculator/TeamSummaryYearCalculator.py
+-rw-rw-rw-   0        0        0      652 2022-09-20 22:58:18.000000 leeger-2.2.0/leeger/calculator/year_calculator/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-15 00:07:33.816947 leeger-2.2.0/leeger/decorator/
+-rw-rw-rw-   0        0        0       85 2022-08-13 05:53:57.000000 leeger-2.2.0/leeger/decorator/__init__.py
+-rw-rw-rw-   0        0        0     4853 2023-02-23 03:42:49.000000 leeger-2.2.0/leeger/decorator/validators.py
+drwxrwxrwx   0        0        0        0 2023-04-15 00:07:33.820948 leeger-2.2.0/leeger/enum/
+-rw-rw-rw-   0        0        0      782 2023-02-17 18:57:53.000000 leeger-2.2.0/leeger/enum/MatchupType.py
+-rw-rw-rw-   0        0        0       38 2022-09-29 19:44:58.000000 leeger-2.2.0/leeger/enum/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-15 00:07:33.845946 leeger-2.2.0/leeger/exception/
+-rw-rw-rw-   0        0        0      157 2022-06-10 22:18:01.000000 leeger-2.2.0/leeger/exception/DoesNotExistException.py
+-rw-rw-rw-   0        0        0      117 2022-06-10 22:18:01.000000 leeger-2.2.0/leeger/exception/InvalidFilterException.py
+-rw-rw-rw-   0        0        0      138 2022-06-10 22:18:01.000000 leeger-2.2.0/leeger/exception/InvalidLeagueFormatException.py
+-rw-rw-rw-   0        0        0      140 2022-06-10 22:18:01.000000 leeger-2.2.0/leeger/exception/InvalidMatchupFormatException.py
+-rw-rw-rw-   0        0        0      137 2022-06-10 22:18:01.000000 leeger-2.2.0/leeger/exception/InvalidOwnerFormatException.py
+-rw-rw-rw-   0        0        0      134 2022-06-10 22:18:01.000000 leeger-2.2.0/leeger/exception/InvalidTeamFormatException.py
+-rw-rw-rw-   0        0        0      134 2022-06-10 22:18:01.000000 leeger-2.2.0/leeger/exception/InvalidWeekFormatException.py
+-rw-rw-rw-   0        0        0      134 2022-06-10 22:18:01.000000 leeger-2.2.0/leeger/exception/InvalidYearFormatException.py
+-rw-rw-rw-   0        0        0      150 2022-10-16 01:33:13.000000 leeger-2.2.0/leeger/exception/InvalidYearSettingsFormatException.py
+-rw-rw-rw-   0        0        0      124 2022-08-08 22:25:46.000000 leeger-2.2.0/leeger/exception/LeagueLoaderException.py
+-rw-rw-rw-   0        0        0      134 2022-09-17 17:22:58.000000 leeger-2.2.0/leeger/exception/UnsupportedLeegerFeatureException.py
+-rw-rw-rw-   0        0        0      762 2022-10-16 01:33:13.000000 leeger-2.2.0/leeger/exception/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-15 00:07:33.860946 leeger-2.2.0/leeger/league_loader/
+-rw-rw-rw-   0        0        0     8513 2023-02-28 02:34:18.000000 leeger-2.2.0/leeger/league_loader/ESPNLeagueLoader.py
+-rw-rw-rw-   0        0        0     7845 2023-04-15 00:06:05.000000 leeger-2.2.0/leeger/league_loader/FleaflickerLeagueLoader.py
+-rw-rw-rw-   0        0        0     2549 2023-02-28 02:34:18.000000 leeger-2.2.0/leeger/league_loader/LeagueLoader.py
+-rw-rw-rw-   0        0        0    12476 2023-02-28 02:34:18.000000 leeger-2.2.0/leeger/league_loader/MyFantasyLeagueLeagueLoader.py
+-rw-rw-rw-   0        0        0    15271 2023-02-28 02:34:18.000000 leeger-2.2.0/leeger/league_loader/SleeperLeagueLoader.py
+-rw-rw-rw-   0        0        0    10706 2023-02-28 02:34:18.000000 leeger-2.2.0/leeger/league_loader/YahooLeagueLoader.py
+-rw-rw-rw-   0        0        0      222 2022-08-08 20:13:25.000000 leeger-2.2.0/leeger/league_loader/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-15 00:07:33.862947 leeger-2.2.0/leeger/model/
+-rw-rw-rw-   0        0        0        0 2022-08-13 05:54:09.000000 leeger-2.2.0/leeger/model/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-15 00:07:33.866948 leeger-2.2.0/leeger/model/abstract/
+-rw-rw-rw-   0        0        0      550 2023-02-17 18:45:58.000000 leeger-2.2.0/leeger/model/abstract/UniqueId.py
+-rw-rw-rw-   0        0        0       32 2022-08-13 05:49:03.000000 leeger-2.2.0/leeger/model/abstract/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-15 00:07:33.874946 leeger-2.2.0/leeger/model/filter/
+-rw-rw-rw-   0        0        0     5502 2023-01-05 20:28:10.000000 leeger-2.2.0/leeger/model/filter/AllTimeFilters.py
+-rw-rw-rw-   0        0        0      319 2022-07-13 01:00:45.000000 leeger-2.2.0/leeger/model/filter/WeekFilters.py
+-rw-rw-rw-   0        0        0     5110 2023-01-05 20:28:10.000000 leeger-2.2.0/leeger/model/filter/YearFilters.py
+-rw-rw-rw-   0        0        0      120 2022-09-17 18:26:39.000000 leeger-2.2.0/leeger/model/filter/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-15 00:07:33.907949 leeger-2.2.0/leeger/model/league/
+-rw-rw-rw-   0        0        0     5600 2023-02-17 18:45:58.000000 leeger-2.2.0/leeger/model/league/League.py
+-rw-rw-rw-   0        0        0     4825 2023-02-17 19:22:16.000000 leeger-2.2.0/leeger/model/league/Matchup.py
+-rw-rw-rw-   0        0        0      880 2023-02-17 18:45:58.000000 leeger-2.2.0/leeger/model/league/Owner.py
+-rw-rw-rw-   0        0        0     1481 2023-02-17 18:54:16.000000 leeger-2.2.0/leeger/model/league/Team.py
+-rw-rw-rw-   0        0        0     2780 2023-02-17 18:54:16.000000 leeger-2.2.0/leeger/model/league/Week.py
+-rw-rw-rw-   0        0        0     2816 2023-02-17 19:02:21.000000 leeger-2.2.0/leeger/model/league/Year.py
+-rw-rw-rw-   0        0        0      999 2023-02-17 19:34:53.000000 leeger-2.2.0/leeger/model/league/YearSettings.py
+-rw-rw-rw-   0        0        0      196 2022-10-16 01:33:13.000000 leeger-2.2.0/leeger/model/league/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-15 00:07:33.911947 leeger-2.2.0/leeger/model/league_helper/
+-rw-rw-rw-   0        0        0     3657 2023-01-04 01:53:09.000000 leeger-2.2.0/leeger/model/league_helper/Performance.py
+-rw-rw-rw-   0        0        0        0 2023-01-04 01:53:09.000000 leeger-2.2.0/leeger/model/league_helper/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-15 00:07:33.918948 leeger-2.2.0/leeger/model/stat/
+-rw-rw-rw-   0        0        0     3891 2022-11-01 16:02:18.000000 leeger-2.2.0/leeger/model/stat/AllTimeStatSheet.py
+-rw-rw-rw-   0        0        0     4125 2023-01-02 01:43:27.000000 leeger-2.2.0/leeger/model/stat/YearStatSheet.py
+-rw-rw-rw-   0        0        0       90 2022-08-13 05:49:50.000000 leeger-2.2.0/leeger/model/stat/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-15 00:07:33.944948 leeger-2.2.0/leeger/util/
+-rw-rw-rw-   0        0        0     1113 2022-07-31 17:54:53.000000 leeger-2.2.0/leeger/util/CustomFormatter.py
+-rw-rw-rw-   0        0        0      859 2022-07-31 17:55:05.000000 leeger-2.2.0/leeger/util/CustomLogger.py
+-rw-rw-rw-   0        0        0      513 2022-06-11 23:09:37.000000 leeger-2.2.0/leeger/util/Deci.py
+-rw-rw-rw-   0        0        0     1428 2022-12-26 23:36:20.000000 leeger-2.2.0/leeger/util/GeneralUtil.py
+-rw-rw-rw-   0        0        0      237 2022-06-10 22:18:01.000000 leeger-2.2.0/leeger/util/IdGenerator.py
+-rw-rw-rw-   0        0        0      312 2023-02-17 18:45:58.000000 leeger-2.2.0/leeger/util/JSONDeserializable.py
+-rw-rw-rw-   0        0        0      278 2022-09-03 18:23:27.000000 leeger-2.2.0/leeger/util/JSONSerializable.py
+-rw-rw-rw-   0        0        0        0 2022-08-13 05:54:20.000000 leeger-2.2.0/leeger/util/__init__.py
+-rw-rw-rw-   0        0        0    15100 2023-02-18 07:06:07.000000 leeger-2.2.0/leeger/util/excel.py
+-rw-rw-rw-   0        0        0     9301 2023-01-02 01:43:27.000000 leeger-2.2.0/leeger/util/excel_helper.py
+drwxrwxrwx   0        0        0        0 2023-04-15 00:07:33.955951 leeger-2.2.0/leeger/util/navigator/
+-rw-rw-rw-   0        0        0     5669 2023-01-05 20:27:34.000000 leeger-2.2.0/leeger/util/navigator/LeagueNavigator.py
+-rw-rw-rw-   0        0        0     2100 2022-12-31 03:44:14.000000 leeger-2.2.0/leeger/util/navigator/MatchupNavigator.py
+-rw-rw-rw-   0        0        0     2191 2022-12-31 03:44:14.000000 leeger-2.2.0/leeger/util/navigator/WeekNavigator.py
+-rw-rw-rw-   0        0        0     6578 2023-01-05 20:27:15.000000 leeger-2.2.0/leeger/util/navigator/YearNavigator.py
+-rw-rw-rw-   0        0        0      178 2022-12-31 03:44:14.000000 leeger-2.2.0/leeger/util/navigator/__init__.py
+-rw-rw-rw-   0        0        0    11461 2023-01-02 01:43:27.000000 leeger-2.2.0/leeger/util/stat_sheet.py
+drwxrwxrwx   0        0        0        0 2023-04-15 00:07:33.970948 leeger-2.2.0/leeger/validate/
+-rw-rw-rw-   0        0        0      258 2022-08-13 06:01:19.000000 leeger-2.2.0/leeger/validate/__init__.py
+-rw-rw-rw-   0        0        0     4254 2022-10-25 22:18:55.000000 leeger-2.2.0/leeger/validate/leagueValidation.py
+-rw-rw-rw-   0        0        0     2460 2023-01-04 01:53:09.000000 leeger-2.2.0/leeger/validate/matchupValidation.py
+-rw-rw-rw-   0        0        0      493 2022-09-13 21:37:08.000000 leeger-2.2.0/leeger/validate/ownerValidation.py
+-rw-rw-rw-   0        0        0      598 2022-09-13 21:37:08.000000 leeger-2.2.0/leeger/validate/teamValidation.py
+-rw-rw-rw-   0        0        0     4624 2022-09-17 18:26:39.000000 leeger-2.2.0/leeger/validate/weekValidation.py
+-rw-rw-rw-   0        0        0      231 2023-02-17 19:20:27.000000 leeger-2.2.0/leeger/validate/yearSettingsValidation.py
+-rw-rw-rw-   0        0        0    13147 2023-01-08 17:42:36.000000 leeger-2.2.0/leeger/validate/yearValidation.py
+drwxrwxrwx   0        0        0        0 2023-04-15 00:07:33.757944 leeger-2.2.0/leeger.egg-info/
+-rw-rw-rw-   0        0        0     9660 2023-04-15 00:07:33.000000 leeger-2.2.0/leeger.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7779 2023-04-15 00:07:33.000000 leeger-2.2.0/leeger.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 00:07:33.000000 leeger-2.2.0/leeger.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      139 2023-04-15 00:07:33.000000 leeger-2.2.0/leeger.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-15 00:07:33.000000 leeger-2.2.0/leeger.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      147 2023-04-13 04:26:54.000000 leeger-2.2.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-15 00:07:34.117948 leeger-2.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1048 2022-11-03 07:24:35.000000 leeger-2.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 00:07:33.705947 leeger-2.2.0/test/
+drwxrwxrwx   0        0        0        0 2023-04-15 00:07:33.973948 leeger-2.2.0/test/test_calculator/
+-rw-rw-rw-   0        0        0        0 2022-06-10 22:18:01.000000 leeger-2.2.0/test/test_calculator/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-15 00:07:33.999947 leeger-2.2.0/test/test_calculator/test_all_time_calculator/
+-rw-rw-rw-   0        0        0        0 2022-06-27 00:56:09.000000 leeger-2.2.0/test/test_calculator/test_all_time_calculator/__init__.py
+-rw-rw-rw-   0        0        0    84596 2022-10-18 21:57:01.000000 leeger-2.2.0/test/test_calculator/test_all_time_calculator/test_AWALAllTimeCalculator.py
+-rw-rw-rw-   0        0        0   202229 2022-10-18 21:57:01.000000 leeger-2.2.0/test/test_calculator/test_all_time_calculator/test_GameOutcomeAllTimeCalculator.py
+-rw-rw-rw-   0        0        0    21521 2022-08-12 21:53:32.000000 leeger-2.2.0/test/test_calculator/test_all_time_calculator/test_PlusMinusAllTimeCalculator.py
+-rw-rw-rw-   0        0        0    85906 2022-08-12 21:53:32.000000 leeger-2.2.0/test/test_calculator/test_all_time_calculator/test_PointsScoredAllTimeCalculator.py
+-rw-rw-rw-   0        0        0    39781 2022-09-20 22:58:18.000000 leeger-2.2.0/test/test_calculator/test_all_time_calculator/test_SSLAllTimeCalculator.py
+-rw-rw-rw-   0        0        0    99301 2022-11-01 16:02:18.000000 leeger-2.2.0/test/test_calculator/test_all_time_calculator/test_ScoringShareAllTimeCalculator.py
+-rw-rw-rw-   0        0        0    25110 2022-09-17 18:26:39.000000 leeger-2.2.0/test/test_calculator/test_all_time_calculator/test_ScoringStandardDeviationAllTimeCalculator.py
+-rw-rw-rw-   0        0        0    41897 2022-08-12 21:53:32.000000 leeger-2.2.0/test/test_calculator/test_all_time_calculator/test_SingleScoreAllTimeCalculator.py
+-rw-rw-rw-   0        0        0    96169 2022-09-17 18:26:39.000000 leeger-2.2.0/test/test_calculator/test_all_time_calculator/test_SmartWinsAllTimeCalculator.py
+-rw-rw-rw-   0        0        0    49915 2022-10-18 21:57:01.000000 leeger-2.2.0/test/test_calculator/test_all_time_calculator/test_TeamSummaryAllTimeCalculator.py
+drwxrwxrwx   0        0        0        0 2023-04-15 00:07:34.026948 leeger-2.2.0/test/test_calculator/test_year_calculator/
+-rw-rw-rw-   0        0        0        0 2022-06-27 00:54:55.000000 leeger-2.2.0/test/test_calculator/test_year_calculator/__init__.py
+-rw-rw-rw-   0        0        0    94805 2022-10-18 21:57:01.000000 leeger-2.2.0/test/test_calculator/test_year_calculator/test_AWALYearCalculator.py
+-rw-rw-rw-   0        0        0    80359 2022-10-18 21:57:01.000000 leeger-2.2.0/test/test_calculator/test_year_calculator/test_GameOutcomeYearCalculator.py
+-rw-rw-rw-   0        0        0     9174 2022-08-12 21:53:32.000000 leeger-2.2.0/test/test_calculator/test_year_calculator/test_PlusMinusYearCalculator.py
+-rw-rw-rw-   0        0        0    36598 2022-08-12 21:53:32.000000 leeger-2.2.0/test/test_calculator/test_year_calculator/test_PointsScoredYearCalculator.py
+-rw-rw-rw-   0        0        0    28074 2022-09-20 22:58:18.000000 leeger-2.2.0/test/test_calculator/test_year_calculator/test_SSLYearCalculator.py
+-rw-rw-rw-   0        0        0    42133 2022-11-01 16:02:18.000000 leeger-2.2.0/test/test_calculator/test_year_calculator/test_ScoringShareYearCalculator.py
+-rw-rw-rw-   0        0        0    11387 2022-09-17 18:26:39.000000 leeger-2.2.0/test/test_calculator/test_year_calculator/test_ScoringStandardDeviationYearCalculator.py
+-rw-rw-rw-   0        0        0    32261 2022-08-12 21:53:32.000000 leeger-2.2.0/test/test_calculator/test_year_calculator/test_SingleScoreYearCalculator.py
+-rw-rw-rw-   0        0        0    75846 2022-09-17 18:26:39.000000 leeger-2.2.0/test/test_calculator/test_year_calculator/test_SmartWinsYearCalculator.py
+-rw-rw-rw-   0        0        0    20425 2022-10-18 21:57:01.000000 leeger-2.2.0/test/test_calculator/test_year_calculator/test_TeamSummaryYearCalculator.py
+drwxrwxrwx   0        0        0        0 2023-04-15 00:07:34.030950 leeger-2.2.0/test/test_decorator/
+-rw-rw-rw-   0        0        0        0 2022-06-10 22:18:01.000000 leeger-2.2.0/test/test_decorator/__init__.py
+-rw-rw-rw-   0        0        0     4605 2023-01-08 17:42:36.000000 leeger-2.2.0/test/test_decorator/test_validators.py
+drwxrwxrwx   0        0        0        0 2023-04-15 00:07:34.042947 leeger-2.2.0/test/test_league_loader/
+-rw-rw-rw-   0        0        0        0 2022-06-25 00:07:47.000000 leeger-2.2.0/test/test_league_loader/__init__.py
+-rw-rw-rw-   0        0        0     1240 2022-09-20 22:58:18.000000 leeger-2.2.0/test/test_league_loader/test_ESPNLeagueLoader.py
+-rw-rw-rw-   0        0        0      409 2022-10-26 20:01:28.000000 leeger-2.2.0/test/test_league_loader/test_FleaflickerLeagueLoader.py
+-rw-rw-rw-   0        0        0      851 2022-09-20 22:58:18.000000 leeger-2.2.0/test/test_league_loader/test_MyFantasyLeagueLeagueLoader.py
+-rw-rw-rw-   0        0        0      698 2022-09-20 22:58:18.000000 leeger-2.2.0/test/test_league_loader/test_SleeperLeagueLoader.py
+-rw-rw-rw-   0        0        0     1462 2022-10-16 21:38:41.000000 leeger-2.2.0/test/test_league_loader/test_YahooLeagueLoader.py
+drwxrwxrwx   0        0        0        0 2023-04-15 00:07:34.044947 leeger-2.2.0/test/test_model/
+-rw-rw-rw-   0        0        0        0 2022-06-10 22:18:01.000000 leeger-2.2.0/test/test_model/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-15 00:07:34.047948 leeger-2.2.0/test/test_model/test_abstract/
+-rw-rw-rw-   0        0        0        0 2022-06-10 22:18:01.000000 leeger-2.2.0/test/test_model/test_abstract/__init__.py
+-rw-rw-rw-   0        0        0      932 2022-09-19 23:01:23.000000 leeger-2.2.0/test/test_model/test_abstract/test_UniqueId.py
+drwxrwxrwx   0        0        0        0 2023-04-15 00:07:34.051950 leeger-2.2.0/test/test_model/test_filter/
+-rw-rw-rw-   0        0        0        0 2022-07-01 18:59:46.000000 leeger-2.2.0/test/test_model/test_filter/__init__.py
+-rw-rw-rw-   0        0        0     1814 2022-07-13 01:00:45.000000 leeger-2.2.0/test/test_model/test_filter/test_AllTimeFilters.py
+drwxrwxrwx   0        0        0        0 2023-04-15 00:07:34.067944 leeger-2.2.0/test/test_model/test_league/
+-rw-rw-rw-   0        0        0        0 2022-06-23 01:09:11.000000 leeger-2.2.0/test/test_model/test_league/__init__.py
+-rw-rw-rw-   0        0        0    20771 2023-02-17 19:27:57.000000 leeger-2.2.0/test/test_model/test_league/test_League.py
+-rw-rw-rw-   0        0        0     8841 2023-02-17 19:28:14.000000 leeger-2.2.0/test/test_model/test_league/test_Matchup.py
+-rw-rw-rw-   0        0        0     1136 2023-02-17 19:28:57.000000 leeger-2.2.0/test/test_model/test_league/test_Owner.py
+-rw-rw-rw-   0        0        0     1219 2023-02-17 19:29:31.000000 leeger-2.2.0/test/test_model/test_league/test_Team.py
+-rw-rw-rw-   0        0        0     8811 2023-02-17 19:30:19.000000 leeger-2.2.0/test/test_model/test_league/test_Week.py
+-rw-rw-rw-   0        0        0     8343 2023-02-17 19:31:44.000000 leeger-2.2.0/test/test_model/test_league/test_Year.py
+-rw-rw-rw-   0        0        0     1487 2023-02-17 19:34:39.000000 leeger-2.2.0/test/test_model/test_league/test_YearSettings.py
+drwxrwxrwx   0        0        0        0 2023-04-15 00:07:34.070947 leeger-2.2.0/test/test_model/test_league_helper/
+-rw-rw-rw-   0        0        0        0 2023-01-04 01:53:09.000000 leeger-2.2.0/test/test_model/test_league_helper/__init__.py
+-rw-rw-rw-   0        0        0     6585 2023-01-04 01:53:09.000000 leeger-2.2.0/test/test_model/test_league_helper/test_Performance.py
+drwxrwxrwx   0        0        0        0 2023-04-15 00:07:34.084946 leeger-2.2.0/test/test_util/
+-rw-rw-rw-   0        0        0        0 2022-06-10 22:18:01.000000 leeger-2.2.0/test/test_util/__init__.py
+-rw-rw-rw-   0        0        0      471 2022-07-13 01:00:46.000000 leeger-2.2.0/test/test_util/test_Deci.py
+-rw-rw-rw-   0        0        0     1375 2022-12-26 23:36:20.000000 leeger-2.2.0/test/test_util/test_GeneralUtil.py
+-rw-rw-rw-   0        0        0      486 2022-07-13 01:00:45.000000 leeger-2.2.0/test/test_util/test_IdGenerator.py
+-rw-rw-rw-   0        0        0    39409 2023-02-18 07:06:07.000000 leeger-2.2.0/test/test_util/test_excel.py
+-rw-rw-rw-   0        0        0     7319 2023-01-02 01:43:27.000000 leeger-2.2.0/test/test_util/test_excel_helper.py
+drwxrwxrwx   0        0        0        0 2023-04-15 00:07:34.095949 leeger-2.2.0/test/test_util/test_navigator/
+-rw-rw-rw-   0        0        0        0 2022-08-12 22:44:07.000000 leeger-2.2.0/test/test_util/test_navigator/__init__.py
+-rw-rw-rw-   0        0        0    47293 2022-12-31 03:44:14.000000 leeger-2.2.0/test/test_util/test_navigator/test_LeagueNavigator.py
+-rw-rw-rw-   0        0        0     3722 2022-12-31 03:44:14.000000 leeger-2.2.0/test/test_util/test_navigator/test_MatchupNavigator.py
+-rw-rw-rw-   0        0        0     5388 2022-12-31 03:44:14.000000 leeger-2.2.0/test/test_util/test_navigator/test_WeekNavigator.py
+-rw-rw-rw-   0        0        0    25968 2022-12-31 03:23:44.000000 leeger-2.2.0/test/test_util/test_navigator/test_YearNavigator.py
+-rw-rw-rw-   0        0        0    10636 2023-01-02 01:43:27.000000 leeger-2.2.0/test/test_util/test_stat_sheet.py
+drwxrwxrwx   0        0        0        0 2023-04-15 00:07:34.113948 leeger-2.2.0/test/test_validate/
+-rw-rw-rw-   0        0        0        0 2022-08-12 22:13:02.000000 leeger-2.2.0/test/test_validate/__init__.py
+-rw-rw-rw-   0        0        0     8307 2022-10-13 23:25:46.000000 leeger-2.2.0/test/test_validate/test_leagueValidation.py
+-rw-rw-rw-   0        0        0     4032 2023-02-17 19:19:04.000000 leeger-2.2.0/test/test_validate/test_matchupValidation.py
+-rw-rw-rw-   0        0        0      532 2022-08-12 21:37:24.000000 leeger-2.2.0/test/test_validate/test_ownerValidation.py
+-rw-rw-rw-   0        0        0      840 2022-08-12 21:37:24.000000 leeger-2.2.0/test/test_validate/test_teamValidation.py
+-rw-rw-rw-   0        0        0     5494 2022-09-17 18:26:39.000000 leeger-2.2.0/test/test_validate/test_weekValidation.py
+-rw-rw-rw-   0        0        0      612 2023-02-17 19:20:44.000000 leeger-2.2.0/test/test_validate/test_yearSettingsValidation.py
+-rw-rw-rw-   0        0        0    22836 2023-01-08 17:42:36.000000 leeger-2.2.0/test/test_validate/test_yearValidation.py
```

### Comparing `leeger-2.1.1/LICENSE` & `leeger-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/PKG-INFO` & `leeger-2.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leeger
-Version: 2.1.1
+Version: 2.2.0
 Summary: Instant stats for your fantasy football league.
 Home-page: https://github.com/joeyagreco/leeger
 Author: Joey Greco
 Author-email: joeyagreco@gmail.com
 License: MIT
 Keywords: nfl statistics stats football espn yahoo sleeper myfantasyleague,fleaflicker
 Requires-Python: >=3.10
```

### Comparing `leeger-2.1.1/README.md` & `leeger-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/leeger/calculator/all_time_calculator/AWALAllTimeCalculator.py` & `leeger-2.2.0/leeger/calculator/all_time_calculator/AWALAllTimeCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/leeger/calculator/all_time_calculator/GameOutcomeAllTimeCalculator.py` & `leeger-2.2.0/leeger/calculator/all_time_calculator/GameOutcomeAllTimeCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/leeger/calculator/all_time_calculator/PlusMinusAllTimeCalculator.py` & `leeger-2.2.0/leeger/calculator/all_time_calculator/PlusMinusAllTimeCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/leeger/calculator/all_time_calculator/PointsScoredAllTimeCalculator.py` & `leeger-2.2.0/leeger/calculator/all_time_calculator/PointsScoredAllTimeCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/leeger/calculator/all_time_calculator/SSLAllTimeCalculator.py` & `leeger-2.2.0/leeger/calculator/all_time_calculator/SSLAllTimeCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/leeger/calculator/all_time_calculator/ScoringShareAllTimeCalculator.py` & `leeger-2.2.0/leeger/calculator/all_time_calculator/ScoringShareAllTimeCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/leeger/calculator/all_time_calculator/ScoringStandardDeviationAllTimeCalculator.py` & `leeger-2.2.0/leeger/calculator/all_time_calculator/ScoringStandardDeviationAllTimeCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/leeger/calculator/all_time_calculator/SingleScoreAllTimeCalculator.py` & `leeger-2.2.0/leeger/calculator/all_time_calculator/SingleScoreAllTimeCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/leeger/calculator/all_time_calculator/SmartWinsAllTimeCalculator.py` & `leeger-2.2.0/leeger/calculator/all_time_calculator/SmartWinsAllTimeCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/leeger/calculator/all_time_calculator/TeamSummaryAllTimeCalculator.py` & `leeger-2.2.0/leeger/calculator/all_time_calculator/TeamSummaryAllTimeCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/leeger/calculator/all_time_calculator/__init__.py` & `leeger-2.2.0/leeger/calculator/all_time_calculator/__init__.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/leeger/calculator/parent/AllTimeCalculator.py` & `leeger-2.2.0/leeger/calculator/parent/AllTimeCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/leeger/calculator/parent/YearCalculator.py` & `leeger-2.2.0/leeger/calculator/parent/YearCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/leeger/calculator/year_calculator/AWALYearCalculator.py` & `leeger-2.2.0/leeger/calculator/year_calculator/AWALYearCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/leeger/calculator/year_calculator/GameOutcomeYearCalculator.py` & `leeger-2.2.0/leeger/calculator/year_calculator/GameOutcomeYearCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/leeger/calculator/year_calculator/PlusMinusYearCalculator.py` & `leeger-2.2.0/leeger/calculator/year_calculator/PlusMinusYearCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/leeger/calculator/year_calculator/PointsScoredYearCalculator.py` & `leeger-2.2.0/leeger/calculator/year_calculator/PointsScoredYearCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/leeger/calculator/year_calculator/SSLYearCalculator.py` & `leeger-2.2.0/leeger/calculator/year_calculator/SSLYearCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/leeger/calculator/year_calculator/ScoringShareYearCalculator.py` & `leeger-2.2.0/leeger/calculator/year_calculator/ScoringShareYearCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/leeger/calculator/year_calculator/ScoringStandardDeviationYearCalculator.py` & `leeger-2.2.0/leeger/calculator/year_calculator/ScoringStandardDeviationYearCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/leeger/calculator/year_calculator/SingleScoreYearCalculator.py` & `leeger-2.2.0/leeger/calculator/year_calculator/SingleScoreYearCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/leeger/calculator/year_calculator/SmartWinsYearCalculator.py` & `leeger-2.2.0/leeger/calculator/year_calculator/SmartWinsYearCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/leeger/calculator/year_calculator/TeamSummaryYearCalculator.py` & `leeger-2.2.0/leeger/calculator/year_calculator/TeamSummaryYearCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/leeger/calculator/year_calculator/__init__.py` & `leeger-2.2.0/leeger/calculator/year_calculator/__init__.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/leeger/decorator/validators.py` & `leeger-2.2.0/leeger/decorator/validators.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/leeger/enum/MatchupType.py` & `leeger-2.2.0/leeger/enum/MatchupType.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/leeger/exception/__init__.py` & `leeger-2.2.0/leeger/exception/__init__.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/leeger/league_loader/ESPNLeagueLoader.py` & `leeger-2.2.0/leeger/league_loader/ESPNLeagueLoader.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/leeger/league_loader/FleaflickerLeagueLoader.py` & `leeger-2.2.0/leeger/league_loader/FleaflickerLeagueLoader.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from fleaflicker.api.LeagueInfoAPIClient import LeagueInfoAPIClient
 from fleaflicker.api.ScoringAPIClient import ScoringAPIClient
 from fleaflicker.enum.Sport import Sport
 from sleeper.enum import Sport
 
 from leeger.enum.MatchupType import MatchupType
-from leeger.exception import LeagueLoaderException
 from leeger.league_loader.LeagueLoader import LeagueLoader
 from leeger.model.league.League import League
 from leeger.model.league.Matchup import Matchup
 from leeger.model.league.Owner import Owner
 from leeger.model.league.Team import Team
 from leeger.model.league.Week import Week
 from leeger.model.league.Year import Year
@@ -23,28 +22,27 @@
 
     def __init__(self, leagueId: str, years: list[int], **kwargs):
         # validation
         try:
             int(leagueId)
         except ValueError:
             raise ValueError(f"League ID '{leagueId}' could not be turned into an int.")
-        if len(years) > 1:
-            raise LeagueLoaderException("Fleaflicker League Loader does not yet support multi-year leagues currently.")
         super().__init__(leagueId, years, **kwargs)
 
         self.__fleaflickerTeamIdToOwnerMap: dict[int, Owner] = dict()
         self.__fleaflickerTeamIdToTeamMap: dict[int, Team] = dict()
 
     def __getAllLeagues(self) -> list[dict]:
         # return a list of all leagues
-        # TODO: find a way to pull consecutive leagues with 1 league ID
-        fleaflickerLeague = LeagueInfoAPIClient.get_league_standings(sport=Sport.NFL,
-                                                                     league_id=int(self._leagueId),
-                                                                     season=self._years[0])
-        return [fleaflickerLeague]
+        fleaflickerLeagues = list()
+        for year in self._years:
+            fleaflickerLeagues.append(LeagueInfoAPIClient.get_league_standings(sport=Sport.NFL,
+                                                                               league_id=int(self._leagueId),
+                                                                               season=year))
+        return fleaflickerLeagues
 
     def getOwnerNames(self) -> dict[int, list[str]]:
         yearToOwnerNamesMap: dict[int, list[str]] = dict()
         fleaflickerLeagues = self.__getAllLeagues()
         for fleaflickerLeague in fleaflickerLeagues:
             yearToOwnerNamesMap[int(fleaflickerLeague["season"])] = list()
             for division in fleaflickerLeague["divisions"]:
@@ -80,21 +78,23 @@
         return Year(yearNumber=int(fleaflickerLeague["season"]), teams=teams, weeks=weeks)
 
     def __buildWeeks(self, fleaflickerLeague: dict) -> list[Week]:
         weeks = list()
         # get all weeks
         fleaflicker_league_scoreboard = ScoringAPIClient.get_league_scoreboard(sport=Sport.NFL,
                                                                                league_id=fleaflickerLeague["league"][
-                                                                                   "id"])
+                                                                                   "id"],
+                                                                               season=fleaflickerLeague["season"])
         number_of_scoring_periods = len(fleaflicker_league_scoreboard["eligibleSchedulePeriods"]) + 1
         for scoring_period in range(1, number_of_scoring_periods):
             matchups = list()
             # get all games for this week
             current_scoreboard = ScoringAPIClient.get_league_scoreboard(sport=Sport.NFL,
                                                                         league_id=fleaflickerLeague["league"]["id"],
+                                                                        season=fleaflickerLeague["season"],
                                                                         scoring_period=scoring_period)
             for game in current_scoreboard.get("games", list()):
                 # team A
                 teamAFleaflicker: dict = game["away"]
                 teamA = self.__fleaflickerTeamIdToTeamMap[teamAFleaflicker["id"]]
                 teamAScore = game["awayScore"]["score"].get("value", 0)  # if "value" isn't found, score is 0
```

### Comparing `leeger-2.1.1/leeger/league_loader/LeagueLoader.py` & `leeger-2.2.0/leeger/league_loader/LeagueLoader.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/leeger/league_loader/MyFantasyLeagueLeagueLoader.py` & `leeger-2.2.0/leeger/league_loader/MyFantasyLeagueLeagueLoader.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/leeger/league_loader/SleeperLeagueLoader.py` & `leeger-2.2.0/leeger/league_loader/SleeperLeagueLoader.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/leeger/league_loader/YahooLeagueLoader.py` & `leeger-2.2.0/leeger/league_loader/YahooLeagueLoader.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/leeger/model/abstract/UniqueId.py` & `leeger-2.2.0/leeger/model/abstract/UniqueId.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/leeger/model/filter/AllTimeFilters.py` & `leeger-2.2.0/leeger/model/filter/AllTimeFilters.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/leeger/model/filter/YearFilters.py` & `leeger-2.2.0/leeger/model/filter/YearFilters.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/leeger/model/league/League.py` & `leeger-2.2.0/leeger/model/league/League.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/leeger/model/league/Matchup.py` & `leeger-2.2.0/leeger/model/league/Matchup.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/leeger/model/league/Owner.py` & `leeger-2.2.0/leeger/model/league/Owner.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/leeger/model/league/Team.py` & `leeger-2.2.0/leeger/model/league/Team.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/leeger/model/league/Week.py` & `leeger-2.2.0/leeger/model/league/Week.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/leeger/model/league/Year.py` & `leeger-2.2.0/leeger/model/league/Year.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/leeger/model/league/YearSettings.py` & `leeger-2.2.0/leeger/model/league/YearSettings.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/leeger/model/league_helper/Performance.py` & `leeger-2.2.0/leeger/model/league_helper/Performance.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/leeger/model/stat/AllTimeStatSheet.py` & `leeger-2.2.0/leeger/model/stat/AllTimeStatSheet.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/leeger/model/stat/YearStatSheet.py` & `leeger-2.2.0/leeger/model/stat/YearStatSheet.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/leeger/util/CustomFormatter.py` & `leeger-2.2.0/leeger/util/CustomFormatter.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/leeger/util/CustomLogger.py` & `leeger-2.2.0/leeger/util/CustomLogger.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/leeger/util/Deci.py` & `leeger-2.2.0/leeger/util/Deci.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/leeger/util/GeneralUtil.py` & `leeger-2.2.0/leeger/util/GeneralUtil.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/leeger/util/excel.py` & `leeger-2.2.0/leeger/util/excel.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/leeger/util/excel_helper.py` & `leeger-2.2.0/leeger/util/excel_helper.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/leeger/util/navigator/LeagueNavigator.py` & `leeger-2.2.0/leeger/util/navigator/LeagueNavigator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/leeger/util/navigator/MatchupNavigator.py` & `leeger-2.2.0/leeger/util/navigator/MatchupNavigator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/leeger/util/navigator/WeekNavigator.py` & `leeger-2.2.0/leeger/util/navigator/WeekNavigator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/leeger/util/navigator/YearNavigator.py` & `leeger-2.2.0/leeger/util/navigator/YearNavigator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/leeger/util/stat_sheet.py` & `leeger-2.2.0/leeger/util/stat_sheet.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/leeger/validate/leagueValidation.py` & `leeger-2.2.0/leeger/validate/leagueValidation.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/leeger/validate/matchupValidation.py` & `leeger-2.2.0/leeger/validate/matchupValidation.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/leeger/validate/teamValidation.py` & `leeger-2.2.0/leeger/validate/teamValidation.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/leeger/validate/weekValidation.py` & `leeger-2.2.0/leeger/validate/weekValidation.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/leeger/validate/yearValidation.py` & `leeger-2.2.0/leeger/validate/yearValidation.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/leeger.egg-info/PKG-INFO` & `leeger-2.2.0/leeger.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leeger
-Version: 2.1.1
+Version: 2.2.0
 Summary: Instant stats for your fantasy football league.
 Home-page: https://github.com/joeyagreco/leeger
 Author: Joey Greco
 Author-email: joeyagreco@gmail.com
 License: MIT
 Keywords: nfl statistics stats football espn yahoo sleeper myfantasyleague,fleaflicker
 Requires-Python: >=3.10
```

### Comparing `leeger-2.1.1/leeger.egg-info/SOURCES.txt` & `leeger-2.2.0/leeger.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/setup.py` & `leeger-2.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/test/test_calculator/test_all_time_calculator/test_AWALAllTimeCalculator.py` & `leeger-2.2.0/test/test_calculator/test_all_time_calculator/test_AWALAllTimeCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/test/test_calculator/test_all_time_calculator/test_GameOutcomeAllTimeCalculator.py` & `leeger-2.2.0/test/test_calculator/test_all_time_calculator/test_GameOutcomeAllTimeCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/test/test_calculator/test_all_time_calculator/test_PlusMinusAllTimeCalculator.py` & `leeger-2.2.0/test/test_calculator/test_all_time_calculator/test_PlusMinusAllTimeCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/test/test_calculator/test_all_time_calculator/test_PointsScoredAllTimeCalculator.py` & `leeger-2.2.0/test/test_calculator/test_all_time_calculator/test_PointsScoredAllTimeCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/test/test_calculator/test_all_time_calculator/test_SSLAllTimeCalculator.py` & `leeger-2.2.0/test/test_calculator/test_all_time_calculator/test_SSLAllTimeCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/test/test_calculator/test_all_time_calculator/test_ScoringShareAllTimeCalculator.py` & `leeger-2.2.0/test/test_calculator/test_all_time_calculator/test_ScoringShareAllTimeCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/test/test_calculator/test_all_time_calculator/test_ScoringStandardDeviationAllTimeCalculator.py` & `leeger-2.2.0/test/test_calculator/test_all_time_calculator/test_ScoringStandardDeviationAllTimeCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/test/test_calculator/test_all_time_calculator/test_SingleScoreAllTimeCalculator.py` & `leeger-2.2.0/test/test_calculator/test_all_time_calculator/test_SingleScoreAllTimeCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/test/test_calculator/test_all_time_calculator/test_SmartWinsAllTimeCalculator.py` & `leeger-2.2.0/test/test_calculator/test_all_time_calculator/test_SmartWinsAllTimeCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/test/test_calculator/test_all_time_calculator/test_TeamSummaryAllTimeCalculator.py` & `leeger-2.2.0/test/test_calculator/test_all_time_calculator/test_TeamSummaryAllTimeCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/test/test_calculator/test_year_calculator/test_AWALYearCalculator.py` & `leeger-2.2.0/test/test_calculator/test_year_calculator/test_AWALYearCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/test/test_calculator/test_year_calculator/test_GameOutcomeYearCalculator.py` & `leeger-2.2.0/test/test_calculator/test_year_calculator/test_GameOutcomeYearCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/test/test_calculator/test_year_calculator/test_PlusMinusYearCalculator.py` & `leeger-2.2.0/test/test_calculator/test_year_calculator/test_PlusMinusYearCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/test/test_calculator/test_year_calculator/test_PointsScoredYearCalculator.py` & `leeger-2.2.0/test/test_calculator/test_year_calculator/test_PointsScoredYearCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/test/test_calculator/test_year_calculator/test_SSLYearCalculator.py` & `leeger-2.2.0/test/test_calculator/test_year_calculator/test_SSLYearCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/test/test_calculator/test_year_calculator/test_ScoringShareYearCalculator.py` & `leeger-2.2.0/test/test_calculator/test_year_calculator/test_ScoringShareYearCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/test/test_calculator/test_year_calculator/test_ScoringStandardDeviationYearCalculator.py` & `leeger-2.2.0/test/test_calculator/test_year_calculator/test_ScoringStandardDeviationYearCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/test/test_calculator/test_year_calculator/test_SingleScoreYearCalculator.py` & `leeger-2.2.0/test/test_calculator/test_year_calculator/test_SingleScoreYearCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/test/test_calculator/test_year_calculator/test_SmartWinsYearCalculator.py` & `leeger-2.2.0/test/test_calculator/test_year_calculator/test_SmartWinsYearCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/test/test_calculator/test_year_calculator/test_TeamSummaryYearCalculator.py` & `leeger-2.2.0/test/test_calculator/test_year_calculator/test_TeamSummaryYearCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/test/test_decorator/test_validators.py` & `leeger-2.2.0/test/test_decorator/test_validators.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/test/test_league_loader/test_ESPNLeagueLoader.py` & `leeger-2.2.0/test/test_league_loader/test_ESPNLeagueLoader.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/test/test_league_loader/test_MyFantasyLeagueLeagueLoader.py` & `leeger-2.2.0/test/test_league_loader/test_MyFantasyLeagueLeagueLoader.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/test/test_league_loader/test_SleeperLeagueLoader.py` & `leeger-2.2.0/test/test_league_loader/test_SleeperLeagueLoader.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/test/test_league_loader/test_YahooLeagueLoader.py` & `leeger-2.2.0/test/test_league_loader/test_YahooLeagueLoader.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/test/test_model/test_abstract/test_UniqueId.py` & `leeger-2.2.0/test/test_model/test_abstract/test_UniqueId.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/test/test_model/test_filter/test_AllTimeFilters.py` & `leeger-2.2.0/test/test_model/test_filter/test_AllTimeFilters.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/test/test_model/test_league/test_League.py` & `leeger-2.2.0/test/test_model/test_league/test_League.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/test/test_model/test_league/test_Matchup.py` & `leeger-2.2.0/test/test_model/test_league/test_Matchup.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/test/test_model/test_league/test_Owner.py` & `leeger-2.2.0/test/test_model/test_league/test_Owner.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/test/test_model/test_league/test_Team.py` & `leeger-2.2.0/test/test_model/test_league/test_Team.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/test/test_model/test_league/test_Week.py` & `leeger-2.2.0/test/test_model/test_league/test_Week.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/test/test_model/test_league/test_Year.py` & `leeger-2.2.0/test/test_model/test_league/test_Year.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/test/test_model/test_league/test_YearSettings.py` & `leeger-2.2.0/test/test_model/test_league/test_YearSettings.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/test/test_model/test_league_helper/test_Performance.py` & `leeger-2.2.0/test/test_model/test_league_helper/test_Performance.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/test/test_util/test_GeneralUtil.py` & `leeger-2.2.0/test/test_util/test_GeneralUtil.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/test/test_util/test_excel.py` & `leeger-2.2.0/test/test_util/test_excel.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/test/test_util/test_excel_helper.py` & `leeger-2.2.0/test/test_util/test_excel_helper.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/test/test_util/test_navigator/test_LeagueNavigator.py` & `leeger-2.2.0/test/test_util/test_navigator/test_LeagueNavigator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/test/test_util/test_navigator/test_MatchupNavigator.py` & `leeger-2.2.0/test/test_util/test_navigator/test_MatchupNavigator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/test/test_util/test_navigator/test_WeekNavigator.py` & `leeger-2.2.0/test/test_util/test_navigator/test_WeekNavigator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/test/test_util/test_navigator/test_YearNavigator.py` & `leeger-2.2.0/test/test_util/test_navigator/test_YearNavigator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/test/test_util/test_stat_sheet.py` & `leeger-2.2.0/test/test_util/test_stat_sheet.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/test/test_validate/test_leagueValidation.py` & `leeger-2.2.0/test/test_validate/test_leagueValidation.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/test/test_validate/test_matchupValidation.py` & `leeger-2.2.0/test/test_validate/test_matchupValidation.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/test/test_validate/test_ownerValidation.py` & `leeger-2.2.0/test/test_validate/test_ownerValidation.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/test/test_validate/test_teamValidation.py` & `leeger-2.2.0/test/test_validate/test_teamValidation.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/test/test_validate/test_weekValidation.py` & `leeger-2.2.0/test/test_validate/test_weekValidation.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/test/test_validate/test_yearSettingsValidation.py` & `leeger-2.2.0/test/test_validate/test_yearSettingsValidation.py`

 * *Files identical despite different names*

### Comparing `leeger-2.1.1/test/test_validate/test_yearValidation.py` & `leeger-2.2.0/test/test_validate/test_yearValidation.py`

 * *Files identical despite different names*

