# Comparing `tmp/azapy-1.2.0.tar.gz` & `tmp/azapy-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azapy-1.2.0.tar", last modified: Sat May 13 22:28:30 2023, max compression
+gzip compressed data, was "azapy-1.2.1.tar", last modified: Mon Aug  7 23:27:36 2023, max compression
```

## Comparing `azapy-1.2.0.tar` & `azapy-1.2.1.tar`

### file list

```diff
@@ -1,79 +1,82 @@
-drwxrwxrwx   0        0        0        0 2023-05-13 22:28:30.424109 azapy-1.2.0/
--rw-rw-rw-   0        0        0    35823 2022-12-13 09:07:48.000000 azapy-1.2.0/LICENSE
--rw-rw-rw-   0        0        0     4777 2023-05-13 22:28:30.423111 azapy-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     4066 2023-05-13 22:26:42.000000 azapy-1.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-13 22:28:30.347747 azapy-1.2.0/azapy/
-drwxrwxrwx   0        0        0        0 2023-05-13 22:28:30.362352 azapy-1.2.0/azapy/Analyzers/
--rw-rw-rw-   0        0        0    33510 2023-05-12 06:16:31.000000 azapy-1.2.0/azapy/Analyzers/BTADAnalyzer.py
--rw-rw-rw-   0        0        0    33889 2023-05-12 06:28:16.000000 azapy-1.2.0/azapy/Analyzers/BTSDAnalyzer.py
--rw-rw-rw-   0        0        0    34639 2023-05-12 06:33:17.000000 azapy-1.2.0/azapy/Analyzers/CVaRAnalyzer.py
--rw-rw-rw-   0        0        0   110492 2023-05-12 06:33:17.000000 azapy-1.2.0/azapy/Analyzers/EVaRAnalyzer.py
--rw-rw-rw-   0        0        0    27119 2023-05-12 06:33:17.000000 azapy-1.2.0/azapy/Analyzers/GINIAnalyzer.py
--rw-rw-rw-   0        0        0    34991 2023-05-12 06:45:21.000000 azapy-1.2.0/azapy/Analyzers/LSDAnalyzer.py
--rw-rw-rw-   0        0        0    34185 2023-05-12 06:45:21.000000 azapy-1.2.0/azapy/Analyzers/MADAnalyzer.py
--rw-rw-rw-   0        0        0    22806 2023-05-12 06:45:21.000000 azapy-1.2.0/azapy/Analyzers/MVAnalyzer.py
--rw-rw-rw-   0        0        0    22965 2023-05-12 06:45:21.000000 azapy-1.2.0/azapy/Analyzers/SDAnalyzer.py
--rw-rw-rw-   0        0        0    40136 2023-05-12 06:45:21.000000 azapy-1.2.0/azapy/Analyzers/SMCRAnalyzer.py
--rw-rw-rw-   0        0        0    87044 2023-05-12 07:15:00.000000 azapy-1.2.0/azapy/Analyzers/_RiskAnalyzer.py
--rw-rw-rw-   0        0        0      282 2023-04-02 04:58:03.000000 azapy-1.2.0/azapy/Analyzers/__init__.py
--rw-rw-rw-   0        0        0     6918 2023-05-09 10:52:00.000000 azapy-1.2.0/azapy/Analyzers/_solvers.py
-drwxrwxrwx   0        0        0        0 2023-05-13 22:28:30.368597 azapy-1.2.0/azapy/Engines/
--rw-rw-rw-   0        0        0     3159 2023-05-12 07:07:44.000000 azapy-1.2.0/azapy/Engines/ConstWEngine.py
--rw-rw-rw-   0        0        0      564 2023-05-12 07:07:44.000000 azapy-1.2.0/azapy/Engines/InvDDEngine.py
--rw-rw-rw-   0        0        0      490 2023-05-12 07:07:44.000000 azapy-1.2.0/azapy/Engines/InvVarEngine.py
--rw-rw-rw-   0        0        0     2203 2023-05-12 07:07:44.000000 azapy-1.2.0/azapy/Engines/InvVolEngine.py
--rw-rw-rw-   0        0        0    11177 2023-05-12 07:15:00.000000 azapy-1.2.0/azapy/Engines/KellyEngine.py
--rw-rw-rw-   0        0        0    10169 2023-05-12 07:15:00.000000 azapy-1.2.0/azapy/Engines/_RiskEngine.py
--rw-rw-rw-   0        0        0      143 2023-04-13 21:18:19.000000 azapy-1.2.0/azapy/Engines/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-13 22:28:30.372586 azapy-1.2.0/azapy/Generators/
--rw-rw-rw-   0        0        0     8799 2023-05-12 07:20:44.000000 azapy-1.2.0/azapy/Generators/ModelPipeline.py
--rw-rw-rw-   0        0        0    16203 2023-05-12 07:37:07.000000 azapy-1.2.0/azapy/Generators/Port_Generator.py
--rw-rw-rw-   0        0        0    22241 2023-05-12 09:30:30.000000 azapy-1.2.0/azapy/Generators/Port_Simple.py
--rw-rw-rw-   0        0        0       61 2023-04-16 00:46:11.000000 azapy-1.2.0/azapy/Generators/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-13 22:28:30.378980 azapy-1.2.0/azapy/MkT/
--rw-rw-rw-   0        0        0     1201 2023-05-12 08:40:40.000000 azapy-1.2.0/azapy/MkT/MkTcalendar.py
--rw-rw-rw-   0        0        0    38243 2023-05-12 08:48:44.000000 azapy-1.2.0/azapy/MkT/MkTreader.py
--rw-rw-rw-   0        0        0      141 2023-05-04 05:46:31.000000 azapy-1.2.0/azapy/MkT/__init__.py
--rw-rw-rw-   0        0        0     6552 2023-05-12 08:49:26.000000 azapy-1.2.0/azapy/MkT/readMkT.py
--rw-rw-rw-   0        0        0     2748 2023-05-04 06:46:48.000000 azapy-1.2.0/azapy/MkT/summary_MkTdata.py
--rw-rw-rw-   0        0        0     3176 2023-05-12 08:51:13.000000 azapy-1.2.0/azapy/MkT/update_MkTdata.py
-drwxrwxrwx   0        0        0        0 2023-05-13 22:28:30.397101 azapy-1.2.0/azapy/PortOpt/
--rw-rw-rw-   0        0        0     5710 2023-05-12 08:28:21.000000 azapy-1.2.0/azapy/PortOpt/Port_BTAD.py
--rw-rw-rw-   0        0        0     5629 2023-05-12 08:28:21.000000 azapy-1.2.0/azapy/PortOpt/Port_BTSD.py
--rw-rw-rw-   0        0        0     5492 2023-05-12 08:28:21.000000 azapy-1.2.0/azapy/PortOpt/Port_CVaR.py
--rw-rw-rw-   0        0        0     1530 2023-05-12 08:07:47.000000 azapy-1.2.0/azapy/PortOpt/Port_ConstW.py
--rw-rw-rw-   0        0        0     5623 2023-05-12 08:28:21.000000 azapy-1.2.0/azapy/PortOpt/Port_EVaR.py
--rw-rw-rw-   0        0        0     4931 2023-05-12 08:28:21.000000 azapy-1.2.0/azapy/PortOpt/Port_GINI.py
--rw-rw-rw-   0        0        0     1564 2023-05-12 08:10:37.000000 azapy-1.2.0/azapy/PortOpt/Port_InvDD.py
--rw-rw-rw-   0        0        0     1558 2023-05-12 08:11:57.000000 azapy-1.2.0/azapy/PortOpt/Port_InvVar.py
--rw-rw-rw-   0        0        0     1582 2023-05-12 08:11:57.000000 azapy-1.2.0/azapy/PortOpt/Port_InvVol.py
--rw-rw-rw-   0        0        0     2231 2023-05-12 08:12:50.000000 azapy-1.2.0/azapy/PortOpt/Port_Kelly.py
--rw-rw-rw-   0        0        0     5056 2023-05-12 08:28:21.000000 azapy-1.2.0/azapy/PortOpt/Port_LSD.py
--rw-rw-rw-   0        0        0     5162 2023-05-12 08:28:21.000000 azapy-1.2.0/azapy/PortOpt/Port_MAD.py
--rw-rw-rw-   0        0        0     4860 2023-05-12 08:28:21.000000 azapy-1.2.0/azapy/PortOpt/Port_MV.py
--rw-rw-rw-   0        0        0     6825 2023-05-12 08:22:23.000000 azapy-1.2.0/azapy/PortOpt/Port_Rebalanced.py
--rw-rw-rw-   0        0        0     4868 2023-05-12 08:28:21.000000 azapy-1.2.0/azapy/PortOpt/Port_SD.py
--rw-rw-rw-   0        0        0     5393 2023-05-12 08:28:21.000000 azapy-1.2.0/azapy/PortOpt/Port_SMCR.py
--rw-rw-rw-   0        0        0     5398 2023-05-13 05:13:25.000000 azapy-1.2.0/azapy/PortOpt/_Port_Generator.py
--rw-rw-rw-   0        0        0      422 2023-04-17 21:10:54.000000 azapy-1.2.0/azapy/PortOpt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-13 22:28:30.401088 azapy-1.2.0/azapy/Selectors/
--rw-rw-rw-   0        0        0     6485 2023-05-12 09:06:51.000000 azapy-1.2.0/azapy/Selectors/CorrClusterSelector.py
--rw-rw-rw-   0        0        0     5129 2023-05-12 08:33:03.000000 azapy-1.2.0/azapy/Selectors/DualMomentumSelector.py
--rw-rw-rw-   0        0        0     1496 2023-05-12 08:31:00.000000 azapy-1.2.0/azapy/Selectors/NullSelector.py
--rw-rw-rw-   0        0        0      102 2023-05-07 21:41:02.000000 azapy-1.2.0/azapy/Selectors/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-13 22:28:30.406976 azapy-1.2.0/azapy/Util/
--rw-rw-rw-   0        0        0      135 2023-05-04 05:22:05.000000 azapy-1.2.0/azapy/Util/__init__.py
--rw-rw-rw-   0        0        0     1570 2023-05-12 08:55:05.000000 azapy-1.2.0/azapy/Util/add_cash_security.py
--rw-rw-rw-   0        0        0     3768 2023-05-12 09:04:21.000000 azapy-1.2.0/azapy/Util/drawdown.py
--rw-rw-rw-   0        0        0     2493 2023-05-12 09:00:50.000000 azapy-1.2.0/azapy/Util/gamblingKelly.py
--rw-rw-rw-   0        0        0     7246 2023-05-12 09:04:06.000000 azapy-1.2.0/azapy/Util/schedule.py
--rw-rw-rw-   0        0        0      278 2023-05-13 16:59:44.000000 azapy-1.2.0/azapy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-13 22:28:30.410966 azapy-1.2.0/azapy.egg-info/
--rw-rw-rw-   0        0        0     4777 2023-05-13 22:28:30.000000 azapy-1.2.0/azapy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3639 2023-05-13 22:28:30.000000 azapy-1.2.0/azapy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-13 22:28:30.000000 azapy-1.2.0/azapy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      106 2023-05-13 22:28:30.000000 azapy-1.2.0/azapy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-13 22:28:30.000000 azapy-1.2.0/azapy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      101 2022-12-13 09:07:48.000000 azapy-1.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-13 22:28:30.424109 azapy-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1362 2023-05-13 16:15:11.000000 azapy-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 23:27:36.058677 azapy-1.2.1/
+-rw-rw-rw-   0        0        0    35823 2023-05-25 21:46:30.000000 azapy-1.2.1/LICENSE
+-rw-rw-rw-   0        0        0     4892 2023-08-07 23:27:36.057680 azapy-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4181 2023-08-07 23:10:37.000000 azapy-1.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-08-07 23:27:35.918116 azapy-1.2.1/azapy/
+drwxrwxrwx   0        0        0        0 2023-08-07 23:27:35.947052 azapy-1.2.1/azapy/Analyzers/
+-rw-rw-rw-   0        0        0    33511 2023-07-19 22:46:44.000000 azapy-1.2.1/azapy/Analyzers/BTADAnalyzer.py
+-rw-rw-rw-   0        0        0    33890 2023-07-19 22:46:02.000000 azapy-1.2.1/azapy/Analyzers/BTSDAnalyzer.py
+-rw-rw-rw-   0        0        0    34641 2023-07-19 22:45:27.000000 azapy-1.2.1/azapy/Analyzers/CVaRAnalyzer.py
+-rw-rw-rw-   0        0        0   110494 2023-07-19 22:45:12.000000 azapy-1.2.1/azapy/Analyzers/EVaRAnalyzer.py
+-rw-rw-rw-   0        0        0    27121 2023-07-19 22:44:56.000000 azapy-1.2.1/azapy/Analyzers/GINIAnalyzer.py
+-rw-rw-rw-   0        0        0    34993 2023-07-19 22:42:04.000000 azapy-1.2.1/azapy/Analyzers/LSDAnalyzer.py
+-rw-rw-rw-   0        0        0    34187 2023-07-19 22:43:10.000000 azapy-1.2.1/azapy/Analyzers/MADAnalyzer.py
+-rw-rw-rw-   0        0        0    22809 2023-07-19 22:41:48.000000 azapy-1.2.1/azapy/Analyzers/MVAnalyzer.py
+-rw-rw-rw-   0        0        0    22968 2023-07-19 22:43:13.000000 azapy-1.2.1/azapy/Analyzers/SDAnalyzer.py
+-rw-rw-rw-   0        0        0    40138 2023-07-19 22:42:19.000000 azapy-1.2.1/azapy/Analyzers/SMCRAnalyzer.py
+-rw-rw-rw-   0        0        0    87051 2023-07-19 22:51:32.000000 azapy-1.2.1/azapy/Analyzers/_RiskAnalyzer.py
+-rw-rw-rw-   0        0        0      282 2023-05-25 21:46:30.000000 azapy-1.2.1/azapy/Analyzers/__init__.py
+-rw-rw-rw-   0        0        0     6918 2023-05-25 21:46:30.000000 azapy-1.2.1/azapy/Analyzers/_solvers.py
+drwxrwxrwx   0        0        0        0 2023-08-07 23:27:35.961796 azapy-1.2.1/azapy/Engines/
+-rw-rw-rw-   0        0        0     3159 2023-05-25 21:46:30.000000 azapy-1.2.1/azapy/Engines/ConstWEngine.py
+-rw-rw-rw-   0        0        0      564 2023-05-25 21:46:30.000000 azapy-1.2.1/azapy/Engines/InvDDEngine.py
+-rw-rw-rw-   0        0        0      490 2023-05-25 21:46:30.000000 azapy-1.2.1/azapy/Engines/InvVarEngine.py
+-rw-rw-rw-   0        0        0     2203 2023-05-25 21:46:30.000000 azapy-1.2.1/azapy/Engines/InvVolEngine.py
+-rw-rw-rw-   0        0        0    11181 2023-07-19 22:56:54.000000 azapy-1.2.1/azapy/Engines/KellyEngine.py
+-rw-rw-rw-   0        0        0    13577 2023-07-19 22:55:14.000000 azapy-1.2.1/azapy/Engines/UniversalEngine.py
+-rw-rw-rw-   0        0        0    10171 2023-07-19 22:59:02.000000 azapy-1.2.1/azapy/Engines/_RiskEngine.py
+-rw-rw-rw-   0        0        0      175 2023-05-26 05:13:02.000000 azapy-1.2.1/azapy/Engines/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-07 23:27:35.969798 azapy-1.2.1/azapy/Generators/
+-rw-rw-rw-   0        0        0     8799 2023-05-25 21:46:30.000000 azapy-1.2.1/azapy/Generators/ModelPipeline.py
+-rw-rw-rw-   0        0        0    16208 2023-07-19 23:15:58.000000 azapy-1.2.1/azapy/Generators/Port_Generator.py
+-rw-rw-rw-   0        0        0    22241 2023-05-25 21:46:30.000000 azapy-1.2.1/azapy/Generators/Port_Simple.py
+-rw-rw-rw-   0        0        0       61 2023-05-25 21:46:30.000000 azapy-1.2.1/azapy/Generators/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-07 23:27:35.981543 azapy-1.2.1/azapy/MkT/
+-rw-rw-rw-   0        0        0     1201 2023-05-25 21:46:30.000000 azapy-1.2.1/azapy/MkT/MkTcalendar.py
+-rw-rw-rw-   0        0        0    38319 2023-07-20 05:43:19.000000 azapy-1.2.1/azapy/MkT/MkTreader.py
+-rw-rw-rw-   0        0        0      141 2023-05-25 21:46:30.000000 azapy-1.2.1/azapy/MkT/__init__.py
+-rw-rw-rw-   0        0        0     6552 2023-05-25 21:46:30.000000 azapy-1.2.1/azapy/MkT/readMkT.py
+-rw-rw-rw-   0        0        0     2741 2023-07-19 23:02:46.000000 azapy-1.2.1/azapy/MkT/summary_MkTdata.py
+-rw-rw-rw-   0        0        0     3176 2023-05-25 21:46:30.000000 azapy-1.2.1/azapy/MkT/update_MkTdata.py
+drwxrwxrwx   0        0        0        0 2023-08-07 23:27:36.016318 azapy-1.2.1/azapy/PortOpt/
+-rw-rw-rw-   0        0        0     5710 2023-07-19 23:13:35.000000 azapy-1.2.1/azapy/PortOpt/Port_BTAD.py
+-rw-rw-rw-   0        0        0     5629 2023-07-19 23:13:11.000000 azapy-1.2.1/azapy/PortOpt/Port_BTSD.py
+-rw-rw-rw-   0        0        0     5493 2023-07-19 23:12:34.000000 azapy-1.2.1/azapy/PortOpt/Port_CVaR.py
+-rw-rw-rw-   0        0        0     1530 2023-05-25 21:46:30.000000 azapy-1.2.1/azapy/PortOpt/Port_ConstW.py
+-rw-rw-rw-   0        0        0     5624 2023-07-19 23:12:10.000000 azapy-1.2.1/azapy/PortOpt/Port_EVaR.py
+-rw-rw-rw-   0        0        0     4932 2023-07-19 23:11:58.000000 azapy-1.2.1/azapy/PortOpt/Port_GINI.py
+-rw-rw-rw-   0        0        0     1564 2023-05-25 21:46:30.000000 azapy-1.2.1/azapy/PortOpt/Port_InvDD.py
+-rw-rw-rw-   0        0        0     1558 2023-05-25 21:46:30.000000 azapy-1.2.1/azapy/PortOpt/Port_InvVar.py
+-rw-rw-rw-   0        0        0     1582 2023-05-25 21:46:30.000000 azapy-1.2.1/azapy/PortOpt/Port_InvVol.py
+-rw-rw-rw-   0        0        0     2231 2023-07-19 23:11:26.000000 azapy-1.2.1/azapy/PortOpt/Port_Kelly.py
+-rw-rw-rw-   0        0        0     5057 2023-07-19 23:11:12.000000 azapy-1.2.1/azapy/PortOpt/Port_LSD.py
+-rw-rw-rw-   0        0        0     5163 2023-07-19 23:10:49.000000 azapy-1.2.1/azapy/PortOpt/Port_MAD.py
+-rw-rw-rw-   0        0        0     4861 2023-07-19 23:10:34.000000 azapy-1.2.1/azapy/PortOpt/Port_MV.py
+-rw-rw-rw-   0        0        0     6827 2023-07-19 23:07:48.000000 azapy-1.2.1/azapy/PortOpt/Port_Rebalanced.py
+-rw-rw-rw-   0        0        0     4869 2023-07-19 23:06:16.000000 azapy-1.2.1/azapy/PortOpt/Port_SD.py
+-rw-rw-rw-   0        0        0     5394 2023-07-19 23:06:05.000000 azapy-1.2.1/azapy/PortOpt/Port_SMCR.py
+-rw-rw-rw-   0        0        0     3888 2023-07-19 22:12:11.000000 azapy-1.2.1/azapy/PortOpt/Port_Universal.py
+-rw-rw-rw-   0        0        0     5410 2023-07-19 23:14:58.000000 azapy-1.2.1/azapy/PortOpt/_Port_Generator.py
+-rw-rw-rw-   0        0        0      453 2023-07-09 16:28:54.000000 azapy-1.2.1/azapy/PortOpt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-07 23:27:36.023384 azapy-1.2.1/azapy/Selectors/
+-rw-rw-rw-   0        0        0     6484 2023-07-19 23:18:10.000000 azapy-1.2.1/azapy/Selectors/CorrClusterSelector.py
+-rw-rw-rw-   0        0        0     5130 2023-07-19 23:17:35.000000 azapy-1.2.1/azapy/Selectors/DualMomentumSelector.py
+-rw-rw-rw-   0        0        0     1496 2023-05-25 21:46:30.000000 azapy-1.2.1/azapy/Selectors/NullSelector.py
+-rw-rw-rw-   0        0        0      102 2023-05-25 21:46:30.000000 azapy-1.2.1/azapy/Selectors/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-07 23:27:36.033986 azapy-1.2.1/azapy/Util/
+-rw-rw-rw-   0        0        0      161 2023-07-07 07:27:15.000000 azapy-1.2.1/azapy/Util/__init__.py
+-rw-rw-rw-   0        0        0     1570 2023-05-25 21:46:30.000000 azapy-1.2.1/azapy/Util/add_cash_security.py
+-rw-rw-rw-   0        0        0     3768 2023-05-25 21:46:30.000000 azapy-1.2.1/azapy/Util/drawdown.py
+-rw-rw-rw-   0        0        0     2493 2023-05-25 21:46:30.000000 azapy-1.2.1/azapy/Util/gamblingKelly.py
+-rw-rw-rw-   0        0        0     2729 2023-08-01 22:33:16.000000 azapy-1.2.1/azapy/Util/randomgen.py
+-rw-rw-rw-   0        0        0     7246 2023-05-25 21:46:30.000000 azapy-1.2.1/azapy/Util/schedule.py
+-rw-rw-rw-   0        0        0      278 2023-05-26 05:15:56.000000 azapy-1.2.1/azapy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-07 23:27:36.044108 azapy-1.2.1/azapy.egg-info/
+-rw-rw-rw-   0        0        0     4892 2023-08-07 23:27:35.000000 azapy-1.2.1/azapy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3823 2023-08-07 23:27:35.000000 azapy-1.2.1/azapy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 23:27:35.000000 azapy-1.2.1/azapy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      106 2023-08-07 23:27:35.000000 azapy-1.2.1/azapy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-08-07 23:27:35.000000 azapy-1.2.1/azapy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      101 2023-05-25 21:46:30.000000 azapy-1.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-07 23:27:36.059674 azapy-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1362 2023-07-19 16:03:50.000000 azapy-1.2.1/setup.py
```

### Comparing `azapy-1.2.0/LICENSE` & `azapy-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `azapy-1.2.0/PKG-INFO` & `azapy-1.2.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azapy
-Version: 1.2.0
+Version: 1.2.1
 Summary: Financial Portfolio Optimization Algorithms
 Home-page: https://github.com/Mircea-MMXXI/azapy.git
 Author: Mircea Marinescu
 Author-email: mircea.marinescu@outlook.com
 License: GPLv3
 Project-URL: Documentation, https://azapy.readthedocs.io/en/latest
 Project-URL: Source, https://github.com/Mircea-MMXXI/azapy
@@ -13,45 +13,49 @@
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # azapy project
+
 ## Financial Portfolio Optimization Algorithms
+
 ### An open-source python library for everybody
 
 ![TimeSeries](graphics/Portfolio_1.png)
 
 Author: Mircea Marinescu
 
 email: Mircea.Marinescu@outlook.com
 
 [Package documentation](https://azapy.readthedocs.io/en/latest)
 
 Package installation: `pip install azapy`
 
 [![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/D1D07G22H)
 
-### Contents
-A. Risk-based portfolio optimization algorithms:
+## Contents
+
+### A. Risk-based portfolio optimization algorithms
+
   1. mCVaR - mixture CVaR (Conditional Value at Risk)
   2. mSMCR - mixture SMCR (Second Moment Coherent Risk)
   3. mMAD - m-level MAD (Mean Absolute Deviation)
   4. mLSD - m-level LSD (Lower Semi-Deviation)
   5. mBTAD - mixture BTAD (Below Threshold Absolute Deviation)
   6. mBTSD - mixture BTSD (Below Threshold Semi-Deviation)
   7. GINI - Gini index (as in Corrado Gini statistician 1884-1965)
   8. SD - standard deviation
   9. MV - variance (as in mean-variance model)
   10. mEVaR - mixture EVaR (Entropic Value at Risk)
   <span style="color:red">(alpha version)</span>
 
-For each class of portfolio the following optimization strategies are
-available:
+#### For each class of portfolio the following optimization strategies are available
+
   1. Optimal-risk portfolio for targeted expected rate of return value
   2. Sharpe-optimal portfolio - maximization of generalized Sharpe ratio
   3. Sharpe-optimal portfolio - minimization of inverse generalized Sharpe
   ratio
   4. Minimum risk portfolio
   5. Optimal-risk portfolio for a fixed risk-aversion factor
   6. Optimal-risk portfolio with the same risk value as a benchmark portfolio
@@ -64,55 +68,62 @@
   10. Optimal-diversified portfolio with the same diversification factor as
   a benchmark portfolio (e.g., same as equal weighted portfolio)
   <span style="color:blue">(beta version)</span>
   11. Optimal-diversified portfolio with the same expected rate of return as
   a benchmark portfolio (e.g., same as equal weighted portfolio)
   <span style="color:blue">(beta version)</span>
 
-B. "Naïve" portfolio strategies:
+### B. "Naïve" portfolio strategies
+
   1. Constant weighted portfolio. A particular case is equal
      weighted portfolio.
   2. Inverse volatility portfolio (i.e., portfolio weights are proportional to
      the inverse of asset volatilities)
   3. Inverse variance portfolio (i.e., portfolio weights are proportional to
      the inverse of asset variances)
   4. Inverse drawdown portfolio (i.e., portfolio weights are proportional to
      the asset absolute value of maximum drawdowns over a predefined
      historical period)
 
-C. Greedy portfolio optimization strategies:
+### C. Greedy portfolio optimization strategies
+
   1. Kelly's portfolio (as in John Larry Kelly Jr. scientist 1923-1965) -
      maximization of portfolio log returns
+  2. Universal portfolio (Thomas M. Cover 1996) <span style="color:red">(alpha version)</span>
+
+### D. Market Selectors
 
-D. Market Selectors
   1. Dual Momentum Selector <span style="color:red">(alpha version)</span>
   2. Correlation Clustering Selector <span style="color:red">(alpha version)</span>
 
-Utility functions:
-  * Collect historical market data from various providers.
-    Supported providers:
-
-    - yahoo.com
-    - eodhistoricaldata.com
-    - alphavantage.co
-    - marketstack.com
-
-  * Generate business calendars. At this point only NYSE business calendar
-    is implemented.
-  * Generate rebalancing portfolio schedules.
-  * Append a cash-like security to an existing market data object.
-  * Update market data saved in a directory.
-
-The following third-party packages were used with azapy 1.2.1:
-  * python 3.11.2
-  * pandas 1.5.3
-  * numpy 1.24.3
-  * scipy 1.10.1
-  * statsmodels 0.13.5
-  * matplotlib 3.7.1
-  * plotly 5.9.0
-  * requests 2.29.0
-  * pandas_market_calendars 4.1.4
-  * ecos 2.0.12
-  * cvxopt 1.3.0.1
-  * ta 0.10.2
-  * yfinance 0.2.14
+### Utility functions:
+
+* Collect historical market data from various providers.
+
+  Supported providers:
+  + yahoo.com
+  + eodhistoricaldata.com
+  + alphavantage.co
+  + marketstack.com
+  
+* Generate business calendars. At this point only NYSE business calendar
+  is implemented.
+* Generate rebalancing portfolio schedules.
+* Append a cash-like security to an existing market data object.
+* Update market data saved in a directory.
+* N-simplex random vectors generators.
+
+### Third-party packages used by **azapy** 1.2.1
+
+* python 3.11.2
+* pandas 1.5.3
+* numpy 1.24.3
+* scipy 1.10.1
+* statsmodels 0.13.5
+* matplotlib 3.7.1
+* plotly 5.9.0
+* requests 2.29.0
+* pandas_market_calendars 4.1.4
+* ecos 2.0.12
+* cvxopt 1.3.0.1
+* ta 0.10.2
+* yfinance 0.2.14
```

### Comparing `azapy-1.2.0/README.md` & `azapy-1.2.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,43 @@
 # azapy project
+
 ## Financial Portfolio Optimization Algorithms
+
 ### An open-source python library for everybody
 
 ![TimeSeries](graphics/Portfolio_1.png)
 
 Author: Mircea Marinescu
 
 email: Mircea.Marinescu@outlook.com
 
 [Package documentation](https://azapy.readthedocs.io/en/latest)
 
 Package installation: `pip install azapy`
 
 [![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/D1D07G22H)
 
-### Contents
-A. Risk-based portfolio optimization algorithms:
+## Contents
+
+### A. Risk-based portfolio optimization algorithms
+
   1. mCVaR - mixture CVaR (Conditional Value at Risk)
   2. mSMCR - mixture SMCR (Second Moment Coherent Risk)
   3. mMAD - m-level MAD (Mean Absolute Deviation)
   4. mLSD - m-level LSD (Lower Semi-Deviation)
   5. mBTAD - mixture BTAD (Below Threshold Absolute Deviation)
   6. mBTSD - mixture BTSD (Below Threshold Semi-Deviation)
   7. GINI - Gini index (as in Corrado Gini statistician 1884-1965)
   8. SD - standard deviation
   9. MV - variance (as in mean-variance model)
   10. mEVaR - mixture EVaR (Entropic Value at Risk)
   <span style="color:red">(alpha version)</span>
 
-For each class of portfolio the following optimization strategies are
-available:
+#### For each class of portfolio the following optimization strategies are available
+
   1. Optimal-risk portfolio for targeted expected rate of return value
   2. Sharpe-optimal portfolio - maximization of generalized Sharpe ratio
   3. Sharpe-optimal portfolio - minimization of inverse generalized Sharpe
   ratio
   4. Minimum risk portfolio
   5. Optimal-risk portfolio for a fixed risk-aversion factor
   6. Optimal-risk portfolio with the same risk value as a benchmark portfolio
@@ -46,55 +50,62 @@
   10. Optimal-diversified portfolio with the same diversification factor as
   a benchmark portfolio (e.g., same as equal weighted portfolio)
   <span style="color:blue">(beta version)</span>
   11. Optimal-diversified portfolio with the same expected rate of return as
   a benchmark portfolio (e.g., same as equal weighted portfolio)
   <span style="color:blue">(beta version)</span>
 
-B. "Naïve" portfolio strategies:
+### B. "Naïve" portfolio strategies
+
   1. Constant weighted portfolio. A particular case is equal
      weighted portfolio.
   2. Inverse volatility portfolio (i.e., portfolio weights are proportional to
      the inverse of asset volatilities)
   3. Inverse variance portfolio (i.e., portfolio weights are proportional to
      the inverse of asset variances)
   4. Inverse drawdown portfolio (i.e., portfolio weights are proportional to
      the asset absolute value of maximum drawdowns over a predefined
      historical period)
 
-C. Greedy portfolio optimization strategies:
+### C. Greedy portfolio optimization strategies
+
   1. Kelly's portfolio (as in John Larry Kelly Jr. scientist 1923-1965) -
      maximization of portfolio log returns
+  2. Universal portfolio (Thomas M. Cover 1996) <span style="color:red">(alpha version)</span>
+
+### D. Market Selectors
 
-D. Market Selectors
   1. Dual Momentum Selector <span style="color:red">(alpha version)</span>
   2. Correlation Clustering Selector <span style="color:red">(alpha version)</span>
 
-Utility functions:
-  * Collect historical market data from various providers.
-    Supported providers:
-
-    - yahoo.com
-    - eodhistoricaldata.com
-    - alphavantage.co
-    - marketstack.com
-
-  * Generate business calendars. At this point only NYSE business calendar
-    is implemented.
-  * Generate rebalancing portfolio schedules.
-  * Append a cash-like security to an existing market data object.
-  * Update market data saved in a directory.
-
-The following third-party packages were used with azapy 1.2.1:
-  * python 3.11.2
-  * pandas 1.5.3
-  * numpy 1.24.3
-  * scipy 1.10.1
-  * statsmodels 0.13.5
-  * matplotlib 3.7.1
-  * plotly 5.9.0
-  * requests 2.29.0
-  * pandas_market_calendars 4.1.4
-  * ecos 2.0.12
-  * cvxopt 1.3.0.1
-  * ta 0.10.2
-  * yfinance 0.2.14
+### Utility functions:
+
+* Collect historical market data from various providers.
+
+  Supported providers:
+  + yahoo.com
+  + eodhistoricaldata.com
+  + alphavantage.co
+  + marketstack.com
+  
+* Generate business calendars. At this point only NYSE business calendar
+  is implemented.
+* Generate rebalancing portfolio schedules.
+* Append a cash-like security to an existing market data object.
+* Update market data saved in a directory.
+* N-simplex random vectors generators.
+
+### Third-party packages used by **azapy** 1.2.1
+
+* python 3.11.2
+* pandas 1.5.3
+* numpy 1.24.3
+* scipy 1.10.1
+* statsmodels 0.13.5
+* matplotlib 3.7.1
+* plotly 5.9.0
+* requests 2.29.0
+* pandas_market_calendars 4.1.4
+* ecos 2.0.12
+* cvxopt 1.3.0.1
+* ta 0.10.2
+* yfinance 0.2.14
```

### Comparing `azapy-1.2.0/azapy/Analyzers/BTADAnalyzer.py` & `azapy-1.2.1/azapy/Analyzers/BTADAnalyzer.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,32 +98,32 @@
             Frontier type. Active only if `rtype='Risk'`. A value of `1` will
             trigger the evaluation of optimal portfolio along the efficient
             frontier. Otherwise, it will find the portfolio with the lowest
             rate of return along the inefficient portfolio frontier.
             The default is `1`.
         mu0 : `float`, optional
             Risk-free rate accessible to the investor.
-            Relevant only if `rype='Sharpe'` or `rtype='Sharpe2'`.
+            Relevant only if `rtype='Sharpe'` or `rtype='Sharpe2'`.
             The default is `0`.
         aversion : `float`, optional
             The value of the risk-aversion coefficient.
             Must be positive. Relevant only if `rtype='RiskAverse'`.
             The default is `None`.
         ww0 : `list`, `numpy.array` or `pandas.Series`, optional
             Targeted portfolio weights. 
-            Relevant only if `rype='InvNrisk'`.
+            Relevant only if `rtype='InvNrisk'`.
             Its length must be equal to the number of symbols in `rrate` 
             (mktdata). All weights must be >= 0 with thier sum > 0.
             If it is a `list` or a `numpy.array` then the weights are assumed 
             to be in order of `rrate.columns`. If it is a `pandas.Series` then 
             the index should be compatible with the `rrate.columns` or mktdata 
             symbols (same symbols, not necessarily in the same order).
             If it is `None` then it will be set to equal weights.
             The default is `None`.
-        detrendent : Boolean, optional
+        detrended : Boolean, optional
             If it set to `True` then the rates of return are detrended 
             (mean=0). The default value is `True`. 
         method : `str`, optional
             Linear programming numerical method. 
             Could be: `'ecos'`, `'highs-ds'`, `'highs-ipm'`, `'highs'`, 
             `'interior-point'`, `'glpk'` and `'cvxopt'`.
             The default is `'ecos'`.
```

### Comparing `azapy-1.2.0/azapy/Analyzers/BTSDAnalyzer.py` & `azapy-1.2.1/azapy/Analyzers/BTSDAnalyzer.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,32 +98,32 @@
             Frontier type. Active only if `rtype='Risk'`. A value of `1` will
             trigger the evaluation of optimal portfolio along the efficient
             frontier. Otherwise, it will find the portfolio with the lowest
             rate of return along the inefficient portfolio frontier.
             The default is `1`.
         mu0 : `float`, optional
             Risk-free rate accessible to the investor.
-            Relevant only if `rype='Sharpe'` or `rtype='Sharpe2'`.
+            Relevant only if `rtype='Sharpe'` or `rtype='Sharpe2'`.
             The default is `0`.
         aversion : `float`, optional
             The value of the risk-aversion coefficient.
             Must be positive. Relevant only if `rtype='RiskAverse'`.
             The default is `None`.
         ww0 : `list`, `numpy.array` or `pandas.Series`, optional
             Targeted portfolio weights. 
-            Relevant only if `rype='InvNrisk'`.
+            Relevant only if `rtype='InvNrisk'`.
             Its length must be equal to the number of symbols in `rrate` 
             (mktdata). All weights must be >= 0 with thier sum > 0.
             If it is a `list` or a `numpy.array` then the weights are assumed 
             to be in order of `rrate.columns`. If it is a `pandas.Series` then 
             the index should be compatible with the `rrate.columns` or mktdata 
             symbols (same symbols, not necessarily in the same order).
             If it is `None` then it will be set to equal weights.
             The default is `None`.
-        detrendent : Boolean, optional
+        detrended : Boolean, optional
             If it set to `True` then the rates of return are detrended 
             (mean=0). The default value is `True`. 
         method : `str`, optional
             SOCP numerical method. 
             Could be: `'ecos'`, or `'cvxopt'`.
             The defualt is `'ecos'`.
```

### Comparing `azapy-1.2.0/azapy/Analyzers/CVaRAnalyzer.py` & `azapy-1.2.1/azapy/Analyzers/CVaRAnalyzer.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,23 +97,23 @@
             Frontier type. Active only if `rtype='Risk'`. A value of `1` will
             trigger the evaluation of optimal portfolio along the efficient
             frontier. Otherwise, it will find the portfolio with the lowest
             rate of return along the inefficient portfolio frontier.
             The default is `1`.
         mu0 : `float`, optional
             Risk-free rate accessible to the investor.
-            Relevant only if `rype='Sharpe'` or `rtype='Sharpe2'`.
+            Relevant only if `rtype='Sharpe'` or `rtype='Sharpe2'`.
             The default is `0`.
         aversion : `float`, optional
             The value of the risk-aversion coefficient.
             Must be positive. Relevant only if `rtype='RiskAverse'`.
             The default is `None`.
         ww0 : `list`, `numpy.array` or `pandas.Series`, optional
             Targeted portfolio weights. 
-            Relevant only if `rype='InvNrisk'`.
+            Relevant only if `rtype='InvNrisk'`.
             Its length must be equal to the number of symbols in `rrate` 
             (mktdata). All weights must be >= 0 with sum > 0.
             If it is a `list` or a `numpy.array` then the weights are assumed 
             to be in order of `rrate.columns`. If it is a `pandas.Series` then 
             the index should be compatible with the `rrate.columns` or mktdata 
             symbols (same symbols, not necessarily in the same order).
             If it is `None` then it will be set to equal weights.
```

### Comparing `azapy-1.2.0/azapy/Analyzers/EVaRAnalyzer.py` & `azapy-1.2.1/azapy/Analyzers/EVaRAnalyzer.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,23 +104,23 @@
             Frontier type. Active only if `rtype='Risk'`. A value of `1` will
             trigger the evaluation of optimal portfolio along the efficient
             frontier. Otherwise, it will find the portfolio with the lowest
             rate of return along the inefficient portfolio frontier.
             The default is `1`.
         mu0 : `float`, optional
             Risk-free rate accessible to the investor.
-            Relevant only if `rype='Sharpe'` or `rtype='Sharpe2'`.
+            Relevant only if `rtype='Sharpe'` or `rtype='Sharpe2'`.
             The default is `0`.
         aversion : `float`, optional
             The value of the risk-aversion coefficient.
             Must be positive. Relevant only if `rtype='RiskAverse'`.
             The default is `None`.
         ww0 : `list`, `numpy.array` or `pandas.Series`, optional
             Targeted portfolio weights. 
-            Relevant only if `rype='InvNrisk'`.
+            Relevant only if `rtype='InvNrisk'`.
             Its length must be equal to the number of symbols in `rrate` 
             (mktdata). All weights must be >= 0 with sum > 0.
             If it is a `list` or a `numpy.array` then the weights are assumed 
             to be in order of `rrate.columns`. If it is a `pandas.Series` then 
             the index should be compatible with the `rrate.columns` or mktdata 
             symbols (same symbols, not necessarily in the same order).
             If it is `None` then it will be set to equal weights.
```

### Comparing `azapy-1.2.0/azapy/Analyzers/GINIAnalyzer.py` & `azapy-1.2.1/azapy/Analyzers/GINIAnalyzer.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,23 +89,23 @@
             Frontier type. Active only if `rtype='Risk'`. A value of `1` will
             trigger the evaluation of optimal portfolio along the efficient
             frontier. Otherwise, it will find the portfolio with the lowest
             rate of return along the inefficient portfolio frontier.
             The default is `1`.
         mu0 : `float`, optional
             Risk-free rate accessible to the investor.
-            Relevant only if `rype='Sharpe'` or `rtype='Sharpe2'`.
+            Relevant only if `rtype='Sharpe'` or `rtype='Sharpe2'`.
             The default is `0`.
         aversion : `float`, optional
             The value of the risk-aversion coefficient.
             Must be positive. Relevant only if `rtype='RiskAverse'`.
             The default is `None`.
         ww0 : `list`, `numpy.array` or `pandas.Series`, optional
             Targeted portfolio weights. 
-            Relevant only if `rype='InvNrisk'`.
+            Relevant only if `rtype='InvNrisk'`.
             Its length must be equal to the number of symbols in `rrate` 
             (mktdata). All weights must be >= 0 with sum > 0.
             If it is a `list` or a `numpy.array` then the weights are assumed 
             to be in order of `rrate.columns`. If it is a `pandas.Series` then 
             the index should be compatible with the `rrate.columns` or mktdata 
             symbols (same symbols, not necessarily in the same order).
             If it is `None` then it will be set to equal weights.
```

### Comparing `azapy-1.2.0/azapy/Analyzers/LSDAnalyzer.py` & `azapy-1.2.1/azapy/Analyzers/LSDAnalyzer.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,23 +93,23 @@
             Frontier type. Active only if `rtype='Risk'`. A value of `1` will
             trigger the evaluation of optimal portfolio along the efficient
             frontier. Otherwise, it will find the portfolio with the lowest
             rate of return along the inefficient portfolio frontier.
             The default is `1`.
         mu0 : `float`, optional
             Risk-free rate accessible to the investor.
-            Relevant only if `rype='Sharpe'` or `rtype='Sharpe2'`.
+            Relevant only if `rtype='Sharpe'` or `rtype='Sharpe2'`.
             The default is `0`.
         aversion : `float`, optional
             The value of the risk-aversion coefficient.
             Must be positive. Relevant only if `rtype='RiskAverse'`.
             The default is `None`.
         ww0 : `list`, `numpy.array` or `pandas.Series`, optional
             Targeted portfolio weights. 
-            Relevant only if `rype='InvNrisk'`.
+            Relevant only if `rtype='InvNrisk'`.
             Its length must be equal to the number of symbols in `rrate` 
             (mktdata). All weights must be >= 0 with sum > 0.
             If it is a `list` or a `numpy.array` then the weights are assumed 
             to be in order of `rrate.columns`. If it is a `pandas.Series` then 
             the index should be compatible with the `rrate.columns` or mktdata 
             symbols (same symbols, not necessarily in the same order).
             If it is `None` then it will be set to equal weights.
```

### Comparing `azapy-1.2.0/azapy/Analyzers/MADAnalyzer.py` & `azapy-1.2.1/azapy/Analyzers/MADAnalyzer.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,23 +93,23 @@
             Frontier type. Active only if `rtype='Risk'`. A value of `1` will
             trigger the evaluation of optimal portfolio along the efficient
             frontier. Otherwise, it will find the portfolio with the lowest
             rate of return along the inefficient portfolio frontier.
             The default is `1`.
         mu0 : `float`, optional
             Risk-free rate accessible to the investor.
-            Relevant only if `rype='Sharpe'` or `rtype='Sharpe2'`.
+            Relevant only if `rtype='Sharpe'` or `rtype='Sharpe2'`.
             The default is `0`.
         aversion : `float`, optional
             The value of the risk-aversion coefficient.
             Must be positive. Relevant only if `rtype='RiskAverse'`.
             The default is `None`.
         ww0 : `list`, `numpy.array` or `pandas.Series`, optional
             Targeted portfolio weights. 
-            Relevant only if `rype='InvNrisk'`.
+            Relevant only if `rtype='InvNrisk'`.
             Its length must be equal to the number of symbols in `rrate` 
             (mktdata). All weights must be >= 0 with sum > 0.
             If it is a `list` or a `numpy.array` then the weights are assumed 
             to be in order of `rrate.columns`. If it is a `pandas.Series` then 
             the index should be compatible with the `rrate.columns` or mktdata 
             symbols (same symbols, not necessarily in the same order).
             If it is `None` then it will be set to equal weights.
```

### Comparing `azapy-1.2.0/azapy/Analyzers/MVAnalyzer.py` & `azapy-1.2.1/azapy/Analyzers/MVAnalyzer.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     **Attributes**
         * `status` : `int` - the computation status (`0` - success, 
           any other value signifies an error)
         * `ww` : `pandas.Series` -  the portfolio weights 
         * `RR` : `float` - portfolio rate of return
         * `risk` : `float` - portfolio MV risk
         * `primary_risk_comp` : `list` - redundant (single element list 
-          containig MV risk value)
+          containing MV risk value)
         * `secondary_risk_comp` : `list` - redundant 
           (same as `primary_risk_comp`)
         * `sharpe` : `float` - MV-Sharpe ration if `rtype` is set to 
           `'Shapre'` or `'Sharpe2'` otherwise `None`. 
         * `diverse` : `float` - diversification factor if `rtype` is set 
           to `'Divers'` or `'MaxDivers'` otherwise `None`.
         * `name` : `str` - portfolio name
@@ -91,23 +91,23 @@
            Frontier type. Active only if `rtype='Risk'`. A value of `1` will
            trigger the evaluation of optimal portfolio along the efficient
            frontier. Otherwise, it will find the portfolio with the lowest
            rate of return along the inefficient portfolio frontier.
            The default is `1`.
         mu0 : `float`, optional
            Risk-free rate accessible to the investor.
-           Relevant only if `rype='Sharpe'` or `rtype='Sharpe2'`.
+           Relevant only if `rtype='Sharpe'` or `rtype='Sharpe2'`.
            The default is `0`.
         aversion : `float`, optional
            The value of the risk-aversion coefficient.
            Must be positive. Relevant only if `rtype='RiskAverse'`.
            The default is `None`.
         ww0 : `list`, `numpy.array` or `pandas.Series`, optional
            Targeted portfolio weights. 
-           Relevant only if `rype='InvNrisk'`.
+           Relevant only if `rtype='InvNrisk'`.
            Its length must be equal to the number of symbols in `rrate` 
            (mktdata). All weights must be >= 0 with sum > 0.
            If it is a `list` or a `numpy.array` then the weights are assumed 
            to be in order of `rrate.columns`. If it is a `pandas.Series` then 
            the index should be compatible with the `rrate.columns` or mktdata 
            symbols (same symbols, not necessarily in the same order).
            If it is `None` then it will be set to equal weights.
@@ -187,15 +187,15 @@
         # rate of return
         self.RR = np.dot(self.ww, self.muk)
         
         return self.ww
     
     
     def _sharpe_max(self):
-        # Computes the mazimization of Sharpe
+        # Computes the maximization of Sharpe
         # Order of variables
         # w <- [0:nn]
         # t <- nn
         # in total dim = nn + 1
         P = self.rrate.cov().to_numpy()
         nn = P.shape[0]
```

### Comparing `azapy-1.2.0/azapy/Analyzers/SDAnalyzer.py` & `azapy-1.2.1/azapy/Analyzers/SDAnalyzer.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     **Attributes**
         * `status` : `int` - the computation status (`0` - success, 
           any other value signifies an error)
         * `ww` : `pandas.Series` -  the portfolio weights 
         * `RR` : `float` - portfolio rate of return
         * `risk` : `float` - portfolio SD risk
         * `primary_risk_comp` : `list` - redundant (single element list 
-          containig SD risk value)
+          containing SD risk value)
         * `secondary_risk_comp` : `list` - redundant 
           (same as `primary_risk_comp`)
         * `sharpe` : `float` - Sharpe ration if `rtype` is set to 
           `'Shapre'` or `'Sharpe2'` otherwise `None`. 
         * `diverse` : `float` - diversification factor if `rtype` is set 
           to `'Divers'` or `'MaxDivers'` otherwise `None`.
         * `name` : `str` - portfolio name
@@ -90,23 +90,23 @@
             Frontier type. Active only if `rtype='Risk'`. A value of `1` will
             trigger the evaluation of optimal portfolio along the efficient
             frontier. Otherwise, it will find the portfolio with the lowest
             rate of return along the inefficient portfolio frontier.
             The default is `1`.
         mu0 : `float`, optional
             Risk-free rate accessible to the investor.
-            Relevant only if `rype='Sharpe'` or `rtype='Sharpe2'`.
+            Relevant only if `rtype='Sharpe'` or `rtype='Sharpe2'`.
             The default is `0`.
         aversion : `float`, optional
             The value of the risk-aversion coefficient.
             Must be positive. Relevant only if `rtype='RiskAverse'`.
             The default is `None`.
         ww0 : `list`, `numpy.array` or `pandas.Series`, optional
             Targeted portfolio weights. 
-            Relevant only if `rype='InvNrisk'`.
+            Relevant only if `rtype='InvNrisk'`.
             Its length must be equal to the number of symbols in `rrate` 
             (mktdata). All weights must be >= 0 with sum > 0.
             If it is a `list` or a `numpy.array` then the weights are assumed 
             to be in order of `rrate.columns`. If it is a `pandas.Series` then 
             the index should be compatible with the `rrate.columns` or mktdata 
             symbols (same symbols, not necessarily in the same order).
             If it is `None` then it will be set to equal weights.
@@ -212,15 +212,15 @@
         # in total dim = nn + 2
         P = self.rrate.cov().to_numpy()
         nn = P.shape[0]
         
         # build c
         c_data = [0.] * (nn + 1) + [1.]
        
-        # biuld G
+        # build G
         dd = sps.block_diag((sps.diags([-1.] * nn, format='coo'), [0.,-1.]))
         
         if any(np.diag(P) < _tol_cholesky):
             pp = np.concatenate((-la.sqrtm(P), np.zeros((nn,2))), axis=1)
         else:
             pp = np.concatenate((-la.cholesky(P, overwrite_a=True), 
                                  np.zeros((nn,2))), axis=1)
```

### Comparing `azapy-1.2.0/azapy/Analyzers/SMCRAnalyzer.py` & `azapy-1.2.1/azapy/Analyzers/SMCRAnalyzer.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,23 +97,23 @@
             Frontier type. Active only if `rtype='Risk'`. A value of `1` will
             trigger the evaluation of optimal portfolio along the efficient
             frontier. Otherwise, it will find the portfolio with the lowest
             rate of return along the inefficient portfolio frontier.
             The default is `1`.
         mu0 : `float`, optional
             Risk-free rate accessible to the investor.
-            Relevant only if `rype='Sharpe'` or `rtype='Sharpe2'`.
+            Relevant only if `rtype='Sharpe'` or `rtype='Sharpe2'`.
             The default is `0`.
         aversion : `float`, optional
             The value of the risk-aversion coefficient.
             Must be positive. Relevant only if `rtype='RiskAverse'`.
             The default is `None`.
         ww0 : `list`, `numpy.array` or `pandas.Series`, optional
             Targeted portfolio weights. 
-            Relevant only if `rype='InvNrisk'`.
+            Relevant only if `rtype='InvNrisk'`.
             Its length must be equal to the number of symbols in `rrate` 
             (mktdata). All weights must be >= 0 with sum > 0.
             If it is a `list` or a `numpy.array` then the weights are assumed 
             to be in order of `rrate.columns`. If it is a `pandas.Series` then 
             the index should be compatible with the `rrate.columns` or mktdata 
             symbols (same symbols, not necessarily in the same order).
             If it is `None` then it will be set to equal weights.
@@ -138,15 +138,15 @@
         # Order of variables:
         # u <- 0, 
         # eta <- 1
         # s <- [2 : nn + 2] 
         # in total dim = nn + 2
         nn = self.nn
         
-        # buold c
+        # build c
         c_data = [1., 1. / (1. - alpha) / np.sqrt(nn)] + [0.] * nn
         
         # build G
         # linear
         G_icol = [0] * nn + list(range(2, nn + 2)) \
                + list(range(2, nn + 2)) + [1]
         G_irow = list(range(nn)) * 2 + list(range(nn, 2 * nn)) + [2 * nn]
```

### Comparing `azapy-1.2.0/azapy/Analyzers/_RiskAnalyzer.py` & `azapy-1.2.1/azapy/Analyzers/_RiskAnalyzer.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     
     **Methods**
         * getWeights
         * getRisk
         * getPositions
         * getRiskComp
         * getDiversification
-        * viewForntiers
+        * viewFrontiers
         * set_rrate
         * set_method
         * set_mktdata
         * set_rtype
         * set_random_seed
     **Attributes**
         * status
@@ -106,23 +106,23 @@
             Frontier type. Active only if `rtype='Risk'`. A value of `1` will
             trigger the evaluation of optimal portfolio along the efficient
             frontier. Otherwise, it will find the portfolio with the lowest
             rate of return along the inefficient portfolio frontier.
             The default is `1`.
         mu0 : `float`, optional
             Risk-free rate accessible to the investor.
-            Relevant only if `rype='Sharpe'` or `rtype='Sharpe2'`.
+            Relevant only if `rtype='Sharpe'` or `rtype='Sharpe2'`.
             The default is `0`.
         aversion : `float`, optional
             The value of the risk-aversion coefficient.
             Must be positive. Relevant only if `rtype='RiskAverse'`.
             The default is `None`.
         ww0 : `list`, `numpy.array` or `pandas.Series`, optional
             Targeted portfolio weights. 
-            Relevant only if `rype='InvNrisk'`.
+            Relevant only if `rtype='InvNrisk'`.
             Its length must be equal to the number of symbols in `rrate` 
             (mktdata). All weights must be >= 0 with sum > 0.
             If it is a `list` or a `numpy.array` then the weights are assumed 
             to be in order of `rrate.columns`. If it is a `pandas.Series` then 
             the index should be compatible with the `rrate.columns` or mktdata 
             symbols (same symbols, not necessarily in the same order).
             If it is `None` then it will be set to equal weights.
@@ -242,38 +242,38 @@
             Frontier type. Active only if `rtype='Risk'`. A value of `1` will
             trigger the evaluation of optimal portfolio along the efficient
             frontier. Otherwise, it will find the portfolio with the lowest
             rate of return along the inefficient portfolio frontier.
             The default is `1`.
         mu0 : `float`, optional
             Risk-free rate accessible to the investor.
-            Relevant only if `rype='Sharpe'` or `rtype='Sharpe2'`.
+            Relevant only if `rtype='Sharpe'` or `rtype='Sharpe2'`.
             The default is `0`.
         aversion : `float`, optional
             The value of the risk-aversion coefficient.
             Must be positive. Relevant only if `rtype='RiskAverse'`.
             The default is `None`.
         ww0 : `list`, `numpy.array` or `pandas.Series`, optional
             Targeted portfolio weights. 
-            Relevant only if `rype='InvNrisk'`.
+            Relevant only if `rtype='InvNrisk'`.
             Its length must be equal to the number of symbols in `rrate` 
             (mktdata). All weights must be >= 0 with sum > 0.
             If it is a `list` or a `numpy.array` then the weights are assumed 
             to be in order of `rrate.columns`. If it is a `pandas.Series` then 
             the index should be compatible with the `rrate.columns` or mktdata 
             symbols (same symbols, not necessarily in the same order).
             If it is `None` then it will be set to equal weights.
             The default is `None`.
         mktdata : `pandas.DataFrame`, optional
             The portfolio components historical, prices or rates of return, see
             `'pclose'` definition below.
             If it is not `None`, it will overwrite the set of historical rates
             of return computed in the constructor from `'mktdata'`. 
             The default is `None`. 
-        **params : other optional paramters
+        **params : other optional parameters
             Most common: \n
             `verbose` : Boolean, optional
                 If it set to `True`, then it will print a message when 
                 the optimal portfolio degenerates to a single asset.
                 The default is `False`.
             `pclose` : Boolean, optional
                 If it is absent then the `mktdata` is considered to contain 
@@ -742,15 +742,15 @@
         freq : `str`, optional
             Rate of return horizon. It could be 
             `'Q'` for a quarter or `'M'` for a month. The default is `'Q'`.
         hlength : `float`, optional
             History length in number of years used for calibration. A
             fractional number will be rounded to an integer number of months.
             The default is `3.25`.
-        pclose : Boolena, optiona; \n
+        pclose : Boolean, optional \n
             `True` : assumes `mktdata` contains closing prices only, 
             with columns the asset symbols and indexed by the 
             observation dates, \n
             `False` : assumes `mktdata` is in the usual format
             returned by `azapy.mktData` function.
             
 
@@ -849,23 +849,23 @@
             Frontier type. Active only if `rtype='Risk'`. A value of `1` will
             trigger the evaluation of optimal portfolio along the efficient
             frontier. Otherwise, it will find the portfolio with the lowest
             rate of return along the inefficient portfolio frontier.
             The default is `1`.
         mu0 : `float`, optional
             Risk-free rate accessible to the investor.
-            Relevant only if `rype='Sharpe'` or `rtype='Sharpe2'`.
+            Relevant only if `rtype='Sharpe'` or `rtype='Sharpe2'`.
             The default is `0`.
         aversion : `float`, optional
             The value of the risk-aversion coefficient.
             Must be positive. Relevant only if `rtype='RiskAverse'`.
             The default is `None`.
         ww0 : `list`, `numpy.array` or `pandas.Series`, optional
             Targeted portfolio weights. 
-            Relevant only if `rype='InvNrisk'`.
+            Relevant only if `rtype='InvNrisk'`.
             Its length must be equal to the number of symbols in `rrate` 
             (mktdata). All weights must be >= 0 with sum > 0.
             If it is a `list` or a `numpy.array` then the weights are assumed 
             to be in order of `rrate.columns`. If it is a `pandas.Series` then 
             the index should be compatible with the `rrate.columns` or mktdata 
             symbols (same symbols, not necessarily in the same order).
             If it is `None` then it will be set to equal weights.
@@ -932,23 +932,23 @@
             Number of points along the inefficient diversification frontier
             (equally spaced along the rate of return axis).
             The default is `20`.
         invN : Boolean, optional
             If it is `True`, then the equal weighted portfolio and the optimal 
             portfolio with the same risk value are added to
             the plot. The default is `True`.
-        invNrisk : Boolena, optional
+        invNrisk : Boolean, optional
             If it is `True`, then the efficient risk portfolio with same risk 
-            as equal weighth portfolio is added to the plot.
-            The defualt is `False`.
+            as equal weighted portfolio is added to the plot.
+            The default is `False`.
         invNdiverse : Boolean, optional
             If it is `True`, then the efficient diversified portfolio with the 
             same diversification factor as the equal weighted portfolio is
             added to the plot. The default is `False`.
-        invNdrr : Boolena, optional
+        invNdrr : Boolean, optional
             If it is `True`, then the efficient diversified portfolio with the 
             same expected rate of return as the equal weighted portfolio is
             added to the plot. The default value is `False`.
         component : Boolean, optional
             If it is `True`, then the single component portfolios are added to 
             the plot. The default is `True`.
         randomport : `int`, optional
@@ -965,15 +965,15 @@
             Graphical representation format. \n
                 * `'RR_risk'` : expected rate of return vs risk
                 * `'Sharpe_RR'` : sharpe vs expected rate of return
                 * `'Diverse_RR'` : diversification vs expected rate of return
                 
             The default is `'RR_risk'`.
         **opt : optional
-            Additonal parameters:\n
+            Additional parameters:\n
                 * `'title'` : `str` 
                     The default is 'Portfolio frontiers'.
                 * `'xlabel'` : `str` 
                     The default is \n
                     - `'risk'` if `fig_type='RR_risk'`,
                     - `'rate of returns'` otherwise.
                 * `'ylabel'` : `str` 
@@ -1793,15 +1793,15 @@
         -------
         `None`
         """
         self.rng = np.random.RandomState(seed)
 
 
     def _ww_gen(self):
-        return self.rng.dirichlet([0.5] * self.mm)
+        return self.rng.dirichlet([1] * self.mm)
     
     
     def _set_lp_method(self, method):
         self.methods = ['ecos', 'highs-ds', 'highs-ipm', 'highs',
                        'interior-point', 'glpk', 'cvxopt']
         if not method in self.methods:
             raise ValueError(f"unknown method {method} - "
```

### Comparing `azapy-1.2.0/azapy/Analyzers/_solvers.py` & `azapy-1.2.1/azapy/Analyzers/_solvers.py`

 * *Files identical despite different names*

### Comparing `azapy-1.2.0/azapy/Engines/ConstWEngine.py` & `azapy-1.2.1/azapy/Engines/ConstWEngine.py`

 * *Files identical despite different names*

### Comparing `azapy-1.2.0/azapy/Engines/InvDDEngine.py` & `azapy-1.2.1/azapy/Engines/InvDDEngine.py`

 * *Files identical despite different names*

### Comparing `azapy-1.2.0/azapy/Engines/InvVolEngine.py` & `azapy-1.2.1/azapy/Engines/InvVolEngine.py`

 * *Files identical despite different names*

### Comparing `azapy-1.2.0/azapy/Engines/KellyEngine.py` & `azapy-1.2.1/azapy/Engines/KellyEngine.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
             Rate of return horizon. It could be 
             'Q' for a quarter or 'M' for a month. The default is `'Q'`.
         hlength : `float`, optional
             History length in number of years used for calibration. A 
             fractional number will be rounded to an integer number of months.
             The default is `3.25` years.
         name : `str`, optional
-            Portfolio name. Deafult value is `'Kelly'`.
+            Portfolio name. Default value is `'Kelly'`.
         rtype : `str`, optional
             Optimization approximation. It can be:\n
                 'ExpCone' - exponential cone constraint programming solver 
                 for original Kelly problem. \n
                 'Full' - non-linear solver for original Kelly problem. \n
                 'Order2' - second order Taylor approximation of original Kelly 
                 problem. It is a QP problem. \n
@@ -81,15 +81,15 @@
                 'Order2' - second order Taylor approximation of original Kelly 
                 problem. It is a QP problem.\n  
             A value different than `None` will
             overwrite the value for `rtype` set in the constructor. \n
             The default is `None`.
         method : `str`, optional
             The QP solver class. It is relevant only if `rtype='Order2'`.
-            It takes 2 values: 'ecos' or 'cvxopt'.
+            It takes 2 values: `'ecos'` or `'cvxopt'`.
             A value different than `None` will overwrite the
             value set in the constructor.
             The default is `None`.
         mktdata : `pandas.DataFrame`, optional
             The portfolio components historical, prices or rates of return, see
             `'pclose'` definition below.
             If it is not `None`, it will overwrite the set of historical rates
```

### Comparing `azapy-1.2.0/azapy/Engines/_RiskEngine.py` & `azapy-1.2.1/azapy/Engines/_RiskEngine.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
             Rate of return horizon. It could be 
             `'Q'` for a quarter or `'M'` for a month. The default is `'Q'`.
         hlength : `float`, optional
             History length in number of years used for calibration. A
             fractional number will be rounded to an integer number of months.
             The default is `3.25` years.
         name : `str`, optional
-            Portfolio name. Deafult value is `None`
+            Portfolio name. Default value is `None`
 
         Returns
         -------
         The object.
         """
         self._ptype_ = 'Optimizer'
         self.ww = None
@@ -105,15 +105,15 @@
         freq : `str`, optional
             Rate of return horizon. It could be 
             `'Q'` for a quarter or `'M'` for a month. The default is `'Q'`.
         hlength : `float`, optional
             History length in number of years used for calibration. A
             fractional number will be rounded to an integer number of months.
             The default is `3.25`.
-        pclose : Boolena, optiona \n
+        pclose : Boolean, optional \n
             `True` : assumes `mktdata` contains closing prices only, 
             with columns the asset symbols and indexed by the 
             observation dates, \n
             `False` : assumes `mktdata` is in the usual format
             returned by `azapy.mktData` function.
             
         Returns
@@ -128,21 +128,21 @@
         
         if freq is None:
             if self.freq is None:
                 raise ValueError("freq not set - it must be 'Q' or 'M'.")
         elif freq in ['Q', 'M']:
             self.freq = freq
         else:
-            raise ValueError(f"wrrong value for freq: {freq}" 
+            raise ValueError(f"wrong value for freq: {freq}" 
                               " - it must be 'Q' or 'M'.")
             
         if hlength is None:
             if self.hlength is None:
                 raise ValueError("hlength must be set to a positive "
-                                 "value eq 1")
+                                 "value e.g. 1")
         else:
             self.hlength = hlength
 
         if mktdata is None:
             # nothing else to do
             return
```

### Comparing `azapy-1.2.0/azapy/Generators/ModelPipeline.py` & `azapy-1.2.1/azapy/Generators/ModelPipeline.py`

 * *Files identical despite different names*

### Comparing `azapy-1.2.0/azapy/Generators/Port_Generator.py` & `azapy-1.2.1/azapy/Generators/Port_Generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         * port : 'pandas.Series' - portfolio time series
         * schedule : 'pandas.DataFrame' - rebalancing schedule
     """
     def __init__(self, mktdata, symb=None, sdate=None, edate=None, 
                  col_price='close', col_divd='divd', col_ref='adjusted',
                  pname='Port', pcolname=None, capital=100000, schedule=None,
                  freq='Q', noffset=-3, fixoffset=-1, histoffset=3.25, 
-                 calendar=None, multitreading=True):
+                 calendar=None, multithreading=True):
         """
         Constructor
     
         Parameters
         ----------
         mktdata : `pandas.DataFrame`
             MkT data in the format "symbol", "date", "open", "high", "low",
@@ -41,15 +41,15 @@
             set to include all the symbols from `mktdata`. The default
             is `None`.
         sdate : date like, optional
             Start date for historical data. If set to `None` the `sdate` will
             be set to the earliest date in `mktdata`. The default is `None`.
         edate : date like, optional
             End date for historical dates and so the simulation. Must be
-            greater than  `sdate`. If it is `None` then `edat`e will be set
+            greater than  `sdate`. If it is `None` then `edate` will be set
             to the latest date in `mktdata`. The default is `None`.
         col_price : `str`, optional
             Column name in the mktdata DataFrame that will be considered
             for portfolio aggregation. The default is `'close'`.
         col_divd :  `str`, optional
             Column name in the mktdata DataFrame that holds the dividend
             information. The default is `'dvid'`.
@@ -82,15 +82,15 @@
             Number of business day offset of fixing date `'Dfix'` relative to
             the rebalancing date `'Droll'`. It can be 0 or negative. It is
             relevant only if the schedule is `None`. The default is `-1`.
         calendar : `numpy.busdaycalendar`, optional
             Business calendar. If it is `None` then it will be set to NYSE
             business calendar. The default
             value is `None`.
-        multitreading : Boolean, optional
+        multithreading : Boolean, optional
             If it is `True` then the rebalancing weights will 
             be computed concurrent. The default is `True`.
     
         Returns
         -------
         The object.
         """
@@ -109,15 +109,15 @@
         self.noffset = noffset
         self.fixoffset = fixoffset
         self.histoffset = histoffset
         self.calendar = calendar
         self.verbose = False
         if self.calendar is None: 
             self._default_calendar()
-        self.multitreading = multitreading
+        self.multithreading = multithreading
         
         
     def set_model(self, wwModel, verbose=False):
         """
         Sets model parameters and evaluates the portfolio time-series.
         
         Parameters
@@ -146,15 +146,15 @@
         if self.schedule is None:
             self.schedule = schedule_offset(self.sdate, self.edate, self.freq,
                                             self.noffset, self.fixoffset,
                                             self.calendar, self.histoffset)
     
     
     def _set_weights(self):
-        if self.multitreading:
+        if self.multithreading:
             return self._set_weights_mt()
         return self._set_weights_sr()
     
     
     def _set_weights_sr(self):
         # local function
         def _fww(Dfix):
```

### Comparing `azapy-1.2.0/azapy/Generators/Port_Simple.py` & `azapy-1.2.1/azapy/Generators/Port_Simple.py`

 * *Files identical despite different names*

### Comparing `azapy-1.2.0/azapy/MkT/MkTcalendar.py` & `azapy-1.2.1/azapy/MkT/MkTcalendar.py`

 * *Files identical despite different names*

### Comparing `azapy-1.2.0/azapy/MkT/MkTreader.py` & `azapy-1.2.1/azapy/MkT/MkTreader.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     """ 
     Collects historical market prices from market data providers such as
     'yahoo', 'eodhistoricaldata', 'alphavantage' and 'marketstack'.
     
     **Attributs**
         - `dsource` : dict of request instructions per symbol
         - `delta_time` : execution time of the request in seconds
-        - `rout` : pandas.DataFrame contenig historical prices for all
+        - `rout` : pandas.DataFrame containing historical prices for all
           symbols. It is created during the call of `get` function.
         - `rout_status` : request status information. It is created during 
           the call of `get_request_status` function or during the 
           call of function `get` with option `verbose=True`.
         - `error_log` : contains lists of missing historical observation 
           dates. It is created together with `rout_status`.
     """
@@ -73,15 +73,15 @@
             Exchange business day calendar. If set to `None` it will default to 
             the NY stock exchange business calendar (provided by the azapy 
             function NYSEgen).
             The default is `None`.
         output_format : `str`, optional
             The function output format. It can be:
                 - `'frame'` - `pandas.DataFrame`
-                - `'dict'` - `dict` of `pandaws.DataFrame`. 
+                - `'dict'` - `dict` of `pandas.DataFrame`. 
                   The symbols are the keys.
                   
             The default is `'frame'`
         source : `str` or `dict`, optional
             If it is a `str`, then it represents the market data provider for 
             all historical prices request. Possible values are: `'yahoo'`, 
             `'alphavantage'`, `'alphavantage_yahoo'`, `'eodhistoricaldata'`,
@@ -816,14 +816,15 @@
             aprice['divd'].fillna(0., inplace=True)
             
         esprice = pd.DataFrame({'split': ysymb.splits})
         if esprice.empty:
             aprice['split'] = 1.
         else:
             esprice.index.name = 'date'
+            esprice.index = pd.to_datetime(esprice.index.date, utc=False)
             aprice = pd.merge(aprice, esprice, how='left', 
                               left_index=True, right_index=True)
             aprice['split'].fillna(1., inplace=True)
         
         aprice['adjusted'] = aprice['close']
         self._adjustSplit(aprice, inplace=True)
```

### Comparing `azapy-1.2.0/azapy/MkT/readMkT.py` & `azapy-1.2.1/azapy/MkT/readMkT.py`

 * *Files identical despite different names*

### Comparing `azapy-1.2.0/azapy/MkT/summary_MkTdata.py` & `azapy-1.2.1/azapy/MkT/summary_MkTdata.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 import pandas as pd
 import numpy as np
 from collections import defaultdict 
 
 from .MkTcalendar import NYSEgen
 
+
 def summary_MkTdata(mktdata, calendar=None, sdate=None, edate=None):
     """
     Summary of MkT data time-series length and quality (checks for missing
     records).
+    
+    Notes
+    -----
+    Its main application is to assess the missing data in the 
+    time-series extracted with `azapy.readMkT` function.
 
     Parameters
     ----------
-    mktdata : `pandas.DataFrame` or a dict of `pndas.DataFrame`
+    mktdata : `pandas.DataFrame` or a dict of `pandas.DataFrame`
         Market Data in the format returned by `azapy.readMkT` function.
     calendar : `numpy.busdaycalendar`, optional
         Business days calendar. If is set to None it will 
         default to NYSE business calendar.
     sdate : `pandas.Timestamp`, optional
         Time-series start date. If it is `None` then `sdate` will be set to the 
         earliest date in mktdata.
@@ -32,19 +38,14 @@
         - `begin` : start date
         - `end` : end date
         - `length` : number of records
         - `na_total` : total number of `nan`
         - `na_b` : number of missing records at the beginning
         - `na_e` : number of missing records at the end
         - `cont` : total number of missing records
-        
-    Comments
-    --------
-    The main application is to assess the missing data in the 
-    time-series extracted with `azapy.readMkT` function.
     """
     if isinstance(mktdata, dict):
         gite = mktdata.items()
     else:
         gite = mktdata.groupby('symbol')
     
     sds = []
```

### Comparing `azapy-1.2.0/azapy/MkT/update_MkTdata.py` & `azapy-1.2.1/azapy/MkT/update_MkTdata.py`

 * *Files identical despite different names*

### Comparing `azapy-1.2.0/azapy/PortOpt/Port_BTAD.py` & `azapy-1.2.1/azapy/PortOpt/Port_BTAD.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,25 +67,25 @@
             The default is `0`.
         aversion : `float`, optional
             The value of the risk-aversion factor.
             Must be positive. Relevant only if `rtype='RiskAvers'`.
             The default is `None`.
         ww0 : `list` (also `numpy.array` or `pandas.Series`), optional
             Targeted portfolio weights. 
-            Relevant only if `rype='InvNrisk'`.
+            Relevant only if `rtype='InvNrisk'`.
             Its length must be equal to the number of
             symbols in `rrate` (`mktdata`). 
             All weights must be >= 0 with their sum > 0.
             If it is a list or a `numpy.array` then the weights are assumed to
             by in order of `rrate.columns`. If it is a `pandas.Series` then 
             the index should be compatible with the `rrate.columns` or `mktdata` 
             symbols (same symbols, not necessarily in the same order).
             If it is `None` then it will be set to equal weights.
             The default is `None`.
-        detrendent : Boolean, optional
+        detrended : Boolean, optional
             If it set to `True` then the rates of return are detrended 
             (`mean=0`). The default value is `True`. 
         hlength : `float`, optional
             The length in year of the historical calibration period relative
             to `'Dfix'`. A fractional number will be rounded to an integer 
             number of months. The default is `3.25` years.
         method : `str`, optional
```

### Comparing `azapy-1.2.0/azapy/PortOpt/Port_BTSD.py` & `azapy-1.2.1/azapy/PortOpt/Port_BTSD.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,25 +67,25 @@
             The default is `0`.
         aversion : `float`, optional
             The value of the risk-aversion factor.
             Must be positive. Relevant only if `rtype='RiskAvers'`.
             The default is `None`.
         ww0 : `list` (also `numpy.array` or `pandas.Series`), optional
             Targeted portfolio weights. 
-            Relevant only if `rype='InvNrisk'`.
+            Relevant only if `rtype='InvNrisk'`.
             Its length must be equal to the number of
             symbols in `rrate` (`mktdata`). 
             All weights must be >= 0 with their sum > 0.
             If it is a list or a `numpy.array` then the weights are assumed to
             by in order of `rrate.columns`. If it is a `pandas.Series` then 
             the index should be compatible with the `rrate.columns` or `mktdata` 
             symbols (same symbols, not necessarily in the same order).
             If it is `None` then it will be set to equal weights.
             The default is `None`.
-        detrendent : Boolean, optional
+        detrended : Boolean, optional
             If it set to `True` then the rates of return are detrended 
             (`mean=0`). The default value is `True`. 
         hlength : `float`, optional
             The length in year of the historical calibration period relative
             to `'Dfix'`. A fractional number will be rounded to an integer 
             number of months. The default is `3.25` years.
         method : `str`, optional
```

### Comparing `azapy-1.2.0/azapy/PortOpt/Port_CVaR.py` & `azapy-1.2.1/azapy/PortOpt/Port_CVaR.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
             The default is `0`.
         aversion : `float`, optional
             The value of the risk-aversion factor.
             Must be positive. Relevant only if `rtype='RiskAvers'`.
             The default is `None`.
         ww0 : `list` (also `numpy.array` or `pandas.Series`), optional
             Targeted portfolio weights. 
-            Relevant only if `rype='InvNrisk'`.
+            Relevant only if `rtype='InvNrisk'`.
             Its length must be equal to the number of
             symbols in `rrate` (`mktdata`). 
             All weights must be >= 0 with their sum > 0.
             If it is a list or a `numpy.array` then the weights are assumed to
             by in order of `rrate.columns`. If it is a `pandas.Series` then 
             the index should be compatible with the `rrate.columns` or `mktdata` 
             symbols (same symbols, not necessarily in the same order).
```

### Comparing `azapy-1.2.0/azapy/PortOpt/Port_ConstW.py` & `azapy-1.2.1/azapy/PortOpt/Port_ConstW.py`

 * *Files identical despite different names*

### Comparing `azapy-1.2.0/azapy/PortOpt/Port_EVaR.py` & `azapy-1.2.1/azapy/PortOpt/Port_EVaR.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
             The default is `0`.
         aversion : `float`, optional
             The value of the risk-aversion factor.
             Must be positive. Relevant only if `rtype='RiskAvers'`.
             The default is `None`.
         ww0 : `list` (also `numpy.array` or `pandas.Series`), optional
             Targeted portfolio weights. 
-            Relevant only if `rype='InvNrisk'`.
+            Relevant only if `rtype='InvNrisk'`.
             Its length must be equal to the number of
             symbols in `rrate` (`mktdata`). 
             All weights must be >= 0 with their sum > 0.
             If it is a list or a `numpy.array` then the weights are assumed to
             by in order of `rrate.columns`. If it is a `pandas.Series` then 
             the index should be compatible with the `rrate.columns` or `mktdata` 
             symbols (same symbols, not necessarily in the same order).
```

### Comparing `azapy-1.2.0/azapy/PortOpt/Port_GINI.py` & `azapy-1.2.1/azapy/PortOpt/Port_GINI.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
             The default is `0`.
         aversion : `float`, optional
             The value of the risk-aversion factor.
             Must be positive. Relevant only if `rtype='RiskAvers'`.
             The default is `None`.
         ww0 : `list` (also `numpy.array` or `pandas.Series`), optional
             Targeted portfolio weights. 
-            Relevant only if `rype='InvNrisk'`.
+            Relevant only if `rtype='InvNrisk'`.
             Its length must be equal to the number of
             symbols in `rrate` (`mktdata`). 
             All weights must be >= 0 with their sum > 0.
             If it is a list or a `numpy.array` then the weights are assumed to
             by in order of `rrate.columns`. If it is a `pandas.Series` then 
             the index should be compatible with the `rrate.columns` or `mktdata` 
             symbols (same symbols, not necessarily in the same order).
```

### Comparing `azapy-1.2.0/azapy/PortOpt/Port_InvDD.py` & `azapy-1.2.1/azapy/PortOpt/Port_InvDD.py`

 * *Files identical despite different names*

### Comparing `azapy-1.2.0/azapy/PortOpt/Port_InvVar.py` & `azapy-1.2.1/azapy/PortOpt/Port_InvVar.py`

 * *Files identical despite different names*

### Comparing `azapy-1.2.0/azapy/PortOpt/Port_InvVol.py` & `azapy-1.2.1/azapy/PortOpt/Port_InvVol.py`

 * *Files identical despite different names*

### Comparing `azapy-1.2.0/azapy/PortOpt/Port_Kelly.py` & `azapy-1.2.1/azapy/PortOpt/Port_Kelly.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         Parameters
         ----------
         rtype : `str`, optional
             Type of optimization. It could take the values:\n
                 `'ExpCone'` - Exponential cone constraint programming solution
                 for full Kelly problem. \n
                 `'Full'` - Non-linear solver for full Kelly problem. \n
-                `'Order2'` - Second order Tayler approximation of Kelly problem. \n
+                `'Order2'` - Second order Taylor approximation of Kelly problem. \n
             The default is `'ExpCone'`.
         hlength : `float`, optional
             The length in year of the historical calibration period relative 
             to `'Dfix'`. A fractional number will be rounded to an integer number 
             of months. The default is `1.25` years. 
         method : `str`, optional
             The QP solver class. It is relevant only if `rtype='Order2'`.
```

### Comparing `azapy-1.2.0/azapy/PortOpt/Port_LSD.py` & `azapy-1.2.1/azapy/PortOpt/Port_LSD.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
             The default is `0`.
         aversion : `float`, optional
             The value of the risk-aversion factor.
             Must be positive. Relevant only if `rtype='RiskAvers'`.
             The default is `None`.
         ww0 : `list` (also `numpy.array` or `pandas.Series`), optional
             Targeted portfolio weights. 
-            Relevant only if `rype='InvNrisk'`.
+            Relevant only if `rtype='InvNrisk'`.
             Its length must be equal to the number of
             symbols in `rrate` (`mktdata`). 
             All weights must be >= 0 with their sum > 0.
             If it is a list or a `numpy.array` then the weights are assumed to
             by in order of `rrate.columns`. If it is a `pandas.Series` then 
             the index should be compatible with the `rrate.columns` or `mktdata` 
             symbols (same symbols, not necessarily in the same order).
```

### Comparing `azapy-1.2.0/azapy/PortOpt/Port_MAD.py` & `azapy-1.2.1/azapy/PortOpt/Port_MAD.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
             The default is `0`.
         aversion : `float`, optional
             The value of the risk-aversion factor.
             Must be positive. Relevant only if `rtype='RiskAvers'`.
             The default is `None`.
         ww0 : `list` (also `numpy.array` or `pandas.Series`), optional
             Targeted portfolio weights. 
-            Relevant only if `rype='InvNrisk'`.
+            Relevant only if `rtype='InvNrisk'`.
             Its length must be equal to the number of
             symbols in `rrate` (`mktdata`). 
             All weights must be >= 0 with their sum > 0.
             If it is a list or a `numpy.array` then the weights are assumed to
             by in order of `rrate.columns`. If it is a `pandas.Series` then 
             the index should be compatible with the `rrate.columns` or `mktdata` 
             symbols (same symbols, not necessarily in the same order).
```

### Comparing `azapy-1.2.0/azapy/PortOpt/Port_MV.py` & `azapy-1.2.1/azapy/PortOpt/Port_MV.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
             The default is `0`.
         aversion : `float`, optional
             The value of the risk-aversion factor.
             Must be positive. Relevant only if `rtype='RiskAvers'`.
             The default is `None`.
         ww0 : `list` (also `numpy.array` or `pandas.Series`), optional
             Targeted portfolio weights. 
-            Relevant only if `rype='InvNrisk'`.
+            Relevant only if `rtype='InvNrisk'`.
             Its length must be equal to the number of
             symbols in `rrate` (`mktdata`). 
             All weights must be >= 0 with their sum > 0.
             If it is a list or a `numpy.array` then the weights are assumed to
             by in order of `rrate.columns`. If it is a `pandas.Series` then 
             the index should be compatible with the `rrate.columns` or `mktdata` 
             symbols (same symbols, not necessarily in the same order).
```

### Comparing `azapy-1.2.0/azapy/PortOpt/Port_Rebalanced.py` & `azapy-1.2.1/azapy/PortOpt/Port_Rebalanced.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
        
     The most important method is `set_model`. It must be called before any
     other method.
     """                  
     def __init__(self, mktdata, symb=None, sdate=None, edate=None, 
                  col_price='close', col_divd='divd', col_ref='adjusted',
                  pname='Port', pcolname=None, capital=100000, schedule=None,
-                 multitreading=True):
+                 multithreading=True):
         """
         Constructor
     
         Parameters
         ----------
         mktdata : `pandas.DataFrame`
             MkT data in the format "symbol", "date", "open", "high", "low",
@@ -36,15 +36,15 @@
             set to include all the symbols from `mktdata`. The default
             is `None`.
         sdate : date like, optional
             Start date for historical data. If set to `None` the `sdate` will
             be set to the earliest date in mktdata. The default is `None`.
         edate : date like, optional
             End date for historical dates and so the simulation. Must be
-            greater than  `sdate`. If it is `None` then `edat`e will be set
+            greater than  `sdate`. If it is `None` then `edate` will be set
             to the latest date in mktdata. The default is `None`.
         col_price : `str`, optional
             Column name in the mktdata DataFrame that will be considered
             for portfolio aggregation. The default is `'close'`.
         col_divd :  `str`, optional
             Column name in the mktdata DataFrame that holds the dividend
             information. The default is `'dvid'`.
@@ -59,15 +59,15 @@
         capital : `float`, optional
             Initial portfolio Capital in dollars. The default is `100000`.
         schedule : `pandas.DataFrame`, optional
             Rebalancing schedule, with columns for `'Droll'` rolling date and
             `'Dfix'` fixing date. If it is `None` than the schedule will be set
             using the `freq`, `noffset`, `fixoffset` and `calendar`
             information. The default is `None`.
-        multitreading : Boolean, optional
+        multithreading : Boolean, optional
             If it is `True` then the weights at the rebalancing dates will 
             be computed concurrent. The default is `True`.
     
         Returns
         -------
         The object.
         """
```

### Comparing `azapy-1.2.0/azapy/PortOpt/Port_SD.py` & `azapy-1.2.1/azapy/PortOpt/Port_SD.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
             The default is `0`.
         aversion : `float`, optional
             The value of the risk-aversion factor.
             Must be positive. Relevant only if `rtype='RiskAvers'`.
             The default is `None`.
         ww0 : `list` (also `numpy.array` or `pandas.Series`), optional
             Targeted portfolio weights. 
-            Relevant only if `rype='InvNrisk'`.
+            Relevant only if `rtype='InvNrisk'`.
             Its length must be equal to the number of
             symbols in `rrate` (`mktdata`). 
             All weights must be >= 0 with their sum > 0.
             If it is a list or a `numpy.array` then the weights are assumed to
             by in order of `rrate.columns`. If it is a `pandas.Series` then 
             the index should be compatible with the `rrate.columns` or `mktdata` 
             symbols (same symbols, not necessarily in the same order).
```

### Comparing `azapy-1.2.0/azapy/PortOpt/Port_SMCR.py` & `azapy-1.2.1/azapy/PortOpt/Port_SMCR.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
             The default is `0`.
         aversion : `float`, optional
             The value of the risk-aversion factor.
             Must be positive. Relevant only if `rtype='RiskAvers'`.
             The default is `None`.
         ww0 : `list` (also `numpy.array` or `pandas.Series`), optional
             Targeted portfolio weights. 
-            Relevant only if `rype='InvNrisk'`.
+            Relevant only if `rtype='InvNrisk'`.
             Its length must be equal to the number of
             symbols in `rrate` (`mktdata`). 
             All weights must be >= 0 with their sum > 0.
             If it is a list or a `numpy.array` then the weights are assumed to
             by in order of `rrate.columns`. If it is a `pandas.Series` then 
             the index should be compatible with the `rrate.columns` or `mktdata` 
             symbols (same symbols, not necessarily in the same order).
@@ -83,15 +83,15 @@
             The default is `None`.
         hlength : `float`, optional
             The length in year of the historical calibration period relative
             to `'Dfix'`. A fractional number will be rounded to an integer 
             number of months. The default is `3.25` years.
         method : `str`, optional
             SOCP numerical method. Could be: `'ecos'` or `'cvxopt'`.
-            The defualt is `'ecos'`.
+            The default is `'ecos'`.
         verbose : Boolean, optional
             If it set to `True` then it will print messages when the optimal
             portfolio degenerates to a single asset portfolio as a limited 
             case. 
             The default is `False`.
 
         Returns
```

### Comparing `azapy-1.2.0/azapy/PortOpt/_Port_Generator.py` & `azapy-1.2.1/azapy/PortOpt/_Port_Generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     
     def __init__(self, mktdata, symb=None, sdate=None, edate=None, 
                  col_price='close', col_divd='divd', col_ref='adjusted',
                  col_calib='adjusted',
                  pname='Port', pcolname=None, capital=100000, 
                  schedule=None,
                  freq='Q', noffset=-3, fixoffset=-1, histoffset=3.25, 
-                 calendar=None, multitreading=True):
+                 calendar=None, multithreading=True):
         """
         Constructor
     
         Parameters
         ----------
         mktdata : `pandas.DataFrame`
             MkT data in the format "symbol", "date", "open", "high", "low",
@@ -84,15 +84,15 @@
         
         super().__init__(mktdata, symb=symb, sdate=sdate, edate=edate, 
                      col_price=col_price, col_divd=col_divd, col_ref=col_ref,
                      pname=pname, pcolname=pcolname, capital=capital, 
                      schedule=schedule,
                      freq=freq, noffset=noffset, fixoffset=fixoffset, 
                      histoffset=histoffset, calendar=calendar,
-                     multitreading=True)
+                     multithreading=multithreading)
         self.col_calib = col_calib
         
         
     def get_weights(self, fancy=False):
         """
         Returns the portfolio weights at each rebalancing period.
```

### Comparing `azapy-1.2.0/azapy/Selectors/CorrClusterSelector.py` & `azapy-1.2.1/azapy/Selectors/CorrClusterSelector.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         corr_thresold : `float`, optional
             Cluster correlation threshold (i.e., a cluster contains only symbols 
             with inter-correlation higher than `corr_threshold`. 
             The default is 0.95.
         freq : `str`, optional
             The horizon of rates subject to correlation estimations. 
             It can be either `'M'` for monthly or `'Q'` for quarterly rates. 
-            The defualt is `'Q'`.
+            The default is `'Q'`.
         ftype : `str`, optional
             Inner-cluster filter (i.e., criteria to designate the representative
             of a cluster with more than one symbol). At this point only 
             `'f13612w'` is implemented.
             The default is 'f13612w'.
         fw : `list`, optional
             List of filter wights. 
@@ -87,15 +87,15 @@
                     If set to `True`, then the dendrogram of hierarchical 
                     classification is printed out. The default is `False`.
                     Note: the tree cutoff is at `1 - corr_threshold` level.
 
         Returns
         -------
         (capital, mkt) : tuple
-            caplital : `float`
+            capital : `float`
                 Fraction of capital allocated to the selection. For this 
                 selector it is always 1.
             mkt  : `pandas.DataFrame`
                Selection MkT data in the format produced by the `azapy` 
                function `readMkT`.
         """
         mkt = mktdata.pivot(columns='symbol', values=self.col_price)
```

### Comparing `azapy-1.2.0/azapy/Selectors/DualMomentumSelector.py` & `azapy-1.2.1/azapy/Selectors/DualMomentumSelector.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
                  nw=3, threshold=6, col_price='adjusted'):
         """
         Constructor
 
         Parameters
         ----------
         pname : `str`, optional
-            Selctor name. The default is 'DualMomentum'.
+            Selector name. The default is 'DualMomentum'.
         ftype : `str`, optional
             The filter name (at this point only `'f13612w'` filter is supported). 
             The default is `'f13612w'` are equal weights.
         fw : `list`, optional
             List of filter wights. 
             For `'f13612w'` it must be a list of 4 positive (not all zero)
             numbers. A value of `None` indicates equal weights.
```

### Comparing `azapy-1.2.0/azapy/Selectors/NullSelector.py` & `azapy-1.2.1/azapy/Selectors/NullSelector.py`

 * *Files identical despite different names*

### Comparing `azapy-1.2.0/azapy/Util/add_cash_security.py` & `azapy-1.2.1/azapy/Util/add_cash_security.py`

 * *Files identical despite different names*

### Comparing `azapy-1.2.0/azapy/Util/drawdown.py` & `azapy-1.2.1/azapy/Util/drawdown.py`

 * *Files identical despite different names*

### Comparing `azapy-1.2.0/azapy/Util/gamblingKelly.py` & `azapy-1.2.1/azapy/Util/gamblingKelly.py`

 * *Files identical despite different names*

### Comparing `azapy-1.2.0/azapy/Util/schedule.py` & `azapy-1.2.1/azapy/Util/schedule.py`

 * *Files identical despite different names*

### Comparing `azapy-1.2.0/azapy.egg-info/PKG-INFO` & `azapy-1.2.1/azapy.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azapy
-Version: 1.2.0
+Version: 1.2.1
 Summary: Financial Portfolio Optimization Algorithms
 Home-page: https://github.com/Mircea-MMXXI/azapy.git
 Author: Mircea Marinescu
 Author-email: mircea.marinescu@outlook.com
 License: GPLv3
 Project-URL: Documentation, https://azapy.readthedocs.io/en/latest
 Project-URL: Source, https://github.com/Mircea-MMXXI/azapy
@@ -13,45 +13,49 @@
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # azapy project
+
 ## Financial Portfolio Optimization Algorithms
+
 ### An open-source python library for everybody
 
 ![TimeSeries](graphics/Portfolio_1.png)
 
 Author: Mircea Marinescu
 
 email: Mircea.Marinescu@outlook.com
 
 [Package documentation](https://azapy.readthedocs.io/en/latest)
 
 Package installation: `pip install azapy`
 
 [![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/D1D07G22H)
 
-### Contents
-A. Risk-based portfolio optimization algorithms:
+## Contents
+
+### A. Risk-based portfolio optimization algorithms
+
   1. mCVaR - mixture CVaR (Conditional Value at Risk)
   2. mSMCR - mixture SMCR (Second Moment Coherent Risk)
   3. mMAD - m-level MAD (Mean Absolute Deviation)
   4. mLSD - m-level LSD (Lower Semi-Deviation)
   5. mBTAD - mixture BTAD (Below Threshold Absolute Deviation)
   6. mBTSD - mixture BTSD (Below Threshold Semi-Deviation)
   7. GINI - Gini index (as in Corrado Gini statistician 1884-1965)
   8. SD - standard deviation
   9. MV - variance (as in mean-variance model)
   10. mEVaR - mixture EVaR (Entropic Value at Risk)
   <span style="color:red">(alpha version)</span>
 
-For each class of portfolio the following optimization strategies are
-available:
+#### For each class of portfolio the following optimization strategies are available
+
   1. Optimal-risk portfolio for targeted expected rate of return value
   2. Sharpe-optimal portfolio - maximization of generalized Sharpe ratio
   3. Sharpe-optimal portfolio - minimization of inverse generalized Sharpe
   ratio
   4. Minimum risk portfolio
   5. Optimal-risk portfolio for a fixed risk-aversion factor
   6. Optimal-risk portfolio with the same risk value as a benchmark portfolio
@@ -64,55 +68,62 @@
   10. Optimal-diversified portfolio with the same diversification factor as
   a benchmark portfolio (e.g., same as equal weighted portfolio)
   <span style="color:blue">(beta version)</span>
   11. Optimal-diversified portfolio with the same expected rate of return as
   a benchmark portfolio (e.g., same as equal weighted portfolio)
   <span style="color:blue">(beta version)</span>
 
-B. "Naïve" portfolio strategies:
+### B. "Naïve" portfolio strategies
+
   1. Constant weighted portfolio. A particular case is equal
      weighted portfolio.
   2. Inverse volatility portfolio (i.e., portfolio weights are proportional to
      the inverse of asset volatilities)
   3. Inverse variance portfolio (i.e., portfolio weights are proportional to
      the inverse of asset variances)
   4. Inverse drawdown portfolio (i.e., portfolio weights are proportional to
      the asset absolute value of maximum drawdowns over a predefined
      historical period)
 
-C. Greedy portfolio optimization strategies:
+### C. Greedy portfolio optimization strategies
+
   1. Kelly's portfolio (as in John Larry Kelly Jr. scientist 1923-1965) -
      maximization of portfolio log returns
+  2. Universal portfolio (Thomas M. Cover 1996) <span style="color:red">(alpha version)</span>
+
+### D. Market Selectors
 
-D. Market Selectors
   1. Dual Momentum Selector <span style="color:red">(alpha version)</span>
   2. Correlation Clustering Selector <span style="color:red">(alpha version)</span>
 
-Utility functions:
-  * Collect historical market data from various providers.
-    Supported providers:
-
-    - yahoo.com
-    - eodhistoricaldata.com
-    - alphavantage.co
-    - marketstack.com
-
-  * Generate business calendars. At this point only NYSE business calendar
-    is implemented.
-  * Generate rebalancing portfolio schedules.
-  * Append a cash-like security to an existing market data object.
-  * Update market data saved in a directory.
-
-The following third-party packages were used with azapy 1.2.1:
-  * python 3.11.2
-  * pandas 1.5.3
-  * numpy 1.24.3
-  * scipy 1.10.1
-  * statsmodels 0.13.5
-  * matplotlib 3.7.1
-  * plotly 5.9.0
-  * requests 2.29.0
-  * pandas_market_calendars 4.1.4
-  * ecos 2.0.12
-  * cvxopt 1.3.0.1
-  * ta 0.10.2
-  * yfinance 0.2.14
+### Utility functions:
+
+* Collect historical market data from various providers.
+
+  Supported providers:
+  + yahoo.com
+  + eodhistoricaldata.com
+  + alphavantage.co
+  + marketstack.com
+  
+* Generate business calendars. At this point only NYSE business calendar
+  is implemented.
+* Generate rebalancing portfolio schedules.
+* Append a cash-like security to an existing market data object.
+* Update market data saved in a directory.
+* N-simplex random vectors generators.
+
+### Third-party packages used by **azapy** 1.2.1
+
+* python 3.11.2
+* pandas 1.5.3
+* numpy 1.24.3
+* scipy 1.10.1
+* statsmodels 0.13.5
+* matplotlib 3.7.1
+* plotly 5.9.0
+* requests 2.29.0
+* pandas_market_calendars 4.1.4
+* ecos 2.0.12
+* cvxopt 1.3.0.1
+* ta 0.10.2
+* yfinance 0.2.14
```

### Comparing `azapy-1.2.0/azapy.egg-info/SOURCES.txt` & `azapy-1.2.1/azapy.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 ./azapy/Analyzers/__init__.py
 ./azapy/Analyzers/_solvers.py
 ./azapy/Engines/ConstWEngine.py
 ./azapy/Engines/InvDDEngine.py
 ./azapy/Engines/InvVarEngine.py
 ./azapy/Engines/InvVolEngine.py
 ./azapy/Engines/KellyEngine.py
+./azapy/Engines/UniversalEngine.py
 ./azapy/Engines/_RiskEngine.py
 ./azapy/Engines/__init__.py
 ./azapy/Generators/ModelPipeline.py
 ./azapy/Generators/Port_Generator.py
 ./azapy/Generators/Port_Simple.py
 ./azapy/Generators/__init__.py
 ./azapy/MkT/MkTcalendar.py
@@ -45,24 +46,26 @@
 ./azapy/PortOpt/Port_Kelly.py
 ./azapy/PortOpt/Port_LSD.py
 ./azapy/PortOpt/Port_MAD.py
 ./azapy/PortOpt/Port_MV.py
 ./azapy/PortOpt/Port_Rebalanced.py
 ./azapy/PortOpt/Port_SD.py
 ./azapy/PortOpt/Port_SMCR.py
+./azapy/PortOpt/Port_Universal.py
 ./azapy/PortOpt/_Port_Generator.py
 ./azapy/PortOpt/__init__.py
 ./azapy/Selectors/CorrClusterSelector.py
 ./azapy/Selectors/DualMomentumSelector.py
 ./azapy/Selectors/NullSelector.py
 ./azapy/Selectors/__init__.py
 ./azapy/Util/__init__.py
 ./azapy/Util/add_cash_security.py
 ./azapy/Util/drawdown.py
 ./azapy/Util/gamblingKelly.py
+./azapy/Util/randomgen.py
 ./azapy/Util/schedule.py
 azapy/__init__.py
 azapy.egg-info/PKG-INFO
 azapy.egg-info/SOURCES.txt
 azapy.egg-info/dependency_links.txt
 azapy.egg-info/requires.txt
 azapy.egg-info/top_level.txt
@@ -80,14 +83,15 @@
 azapy/Analyzers/__init__.py
 azapy/Analyzers/_solvers.py
 azapy/Engines/ConstWEngine.py
 azapy/Engines/InvDDEngine.py
 azapy/Engines/InvVarEngine.py
 azapy/Engines/InvVolEngine.py
 azapy/Engines/KellyEngine.py
+azapy/Engines/UniversalEngine.py
 azapy/Engines/_RiskEngine.py
 azapy/Engines/__init__.py
 azapy/Generators/ModelPipeline.py
 azapy/Generators/Port_Generator.py
 azapy/Generators/Port_Simple.py
 azapy/Generators/__init__.py
 azapy/MkT/MkTcalendar.py
@@ -108,18 +112,20 @@
 azapy/PortOpt/Port_Kelly.py
 azapy/PortOpt/Port_LSD.py
 azapy/PortOpt/Port_MAD.py
 azapy/PortOpt/Port_MV.py
 azapy/PortOpt/Port_Rebalanced.py
 azapy/PortOpt/Port_SD.py
 azapy/PortOpt/Port_SMCR.py
+azapy/PortOpt/Port_Universal.py
 azapy/PortOpt/_Port_Generator.py
 azapy/PortOpt/__init__.py
 azapy/Selectors/CorrClusterSelector.py
 azapy/Selectors/DualMomentumSelector.py
 azapy/Selectors/NullSelector.py
 azapy/Selectors/__init__.py
 azapy/Util/__init__.py
 azapy/Util/add_cash_security.py
 azapy/Util/drawdown.py
 azapy/Util/gamblingKelly.py
+azapy/Util/randomgen.py
 azapy/Util/schedule.py
```

### Comparing `azapy-1.2.0/setup.py` & `azapy-1.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #from azapy import __version__
 
 with open("README.md", "r", encoding="utf-8") as readme:
     long_description = readme.read()
 
 setuptools.setup(
     name="azapy",
-    version="1.2.0",
+    version="1.2.1",
     author="Mircea Marinescu",
     author_email="mircea.marinescu@outlook.com",
     description="Financial Portfolio Optimization Algorithms",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Mircea-MMXXI/azapy.git",
     project_urls={
```

