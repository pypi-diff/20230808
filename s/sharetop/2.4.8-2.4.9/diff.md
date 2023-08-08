# Comparing `tmp/sharetop-2.4.8.tar.gz` & `tmp/sharetop-2.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sharetop-2.4.8.tar", last modified: Fri Aug  4 04:23:47 2023, max compression
+gzip compressed data, was "sharetop-2.4.9.tar", last modified: Tue Aug  8 12:48:08 2023, max compression
```

## Comparing `sharetop-2.4.8.tar` & `sharetop-2.4.9.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxrwxrwx   0        0        0        0 2023-08-04 04:23:47.483309 sharetop-2.4.8/
--rw-rw-rw-   0        0        0     1066 2023-04-26 14:07:21.000000 sharetop-2.4.8/LICENSE
--rw-rw-rw-   0        0        0    51253 2023-08-04 04:23:47.482308 sharetop-2.4.8/PKG-INFO
--rw-rw-rw-   0        0        0    49774 2023-07-15 03:35:16.000000 sharetop-2.4.8/README.md
--rw-rw-rw-   0        0        0       42 2023-08-04 04:23:47.483309 sharetop-2.4.8/setup.cfg
--rw-rw-rw-   0        0        0     1219 2023-04-29 06:50:50.000000 sharetop-2.4.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-04 04:23:47.394938 sharetop-2.4.8/sharetop/
--rw-rw-rw-   0        0        0      297 2023-05-18 12:23:41.000000 sharetop-2.4.8/sharetop/__init__.py
--rw-rw-rw-   0        0        0      386 2023-08-04 04:23:42.000000 sharetop-2.4.8/sharetop/__version__.py
-drwxrwxrwx   0        0        0        0 2023-08-04 04:23:47.426762 sharetop-2.4.8/sharetop/api/
--rw-rw-rw-   0        0        0      306 2023-07-02 13:11:41.000000 sharetop-2.4.8/sharetop/api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-04 04:23:47.429965 sharetop-2.4.8/sharetop/application/
--rw-rw-rw-   0        0        0       33 2023-04-21 11:53:52.000000 sharetop-2.4.8/sharetop/application/__init__.py
--rw-rw-rw-   0        0        0     4461 2023-08-03 04:20:19.000000 sharetop-2.4.8/sharetop/application/base.py
-drwxrwxrwx   0        0        0        0 2023-08-04 04:23:47.434381 sharetop-2.4.8/sharetop/core/
--rw-rw-rw-   0        0        0        0 2023-04-08 05:23:09.000000 sharetop-2.4.8/sharetop/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-04 04:23:47.437397 sharetop-2.4.8/sharetop/core/bond/
--rw-rw-rw-   0        0        0      592 2023-07-15 11:00:24.000000 sharetop-2.4.8/sharetop/core/bond/__init__.py
--rw-rw-rw-   0        0        0     1869 2023-04-24 04:28:03.000000 sharetop-2.4.8/sharetop/core/bond/config.py
--rw-rw-rw-   0        0        0     9767 2023-08-01 15:18:53.000000 sharetop-2.4.8/sharetop/core/bond/get_bond_info.py
--rw-rw-rw-   0        0        0    19614 2023-07-15 10:59:53.000000 sharetop-2.4.8/sharetop/core/bond/get_bond_public_info.py
--rw-rw-rw-   0        0        0      598 2023-04-10 05:06:06.000000 sharetop-2.4.8/sharetop/core/cache.py
-drwxrwxrwx   0        0        0        0 2023-08-04 04:23:47.439378 sharetop-2.4.8/sharetop/core/capital_flow/
--rw-rw-rw-   0        0        0      367 2023-07-15 15:19:38.000000 sharetop-2.4.8/sharetop/core/capital_flow/__init__.py
--rw-rw-rw-   0        0        0     6785 2023-07-25 15:02:39.000000 sharetop-2.4.8/sharetop/core/capital_flow/capital_flow_monitor.py
-drwxrwxrwx   0        0        0        0 2023-08-04 04:23:47.444728 sharetop-2.4.8/sharetop/core/common/
--rw-rw-rw-   0        0        0      188 2023-04-27 15:24:55.000000 sharetop-2.4.8/sharetop/core/common/__init__.py
--rw-rw-rw-   0        0        0     3727 2023-07-19 03:47:04.000000 sharetop-2.4.8/sharetop/core/common/common_base.py
--rw-rw-rw-   0        0        0     8688 2023-05-25 01:16:42.000000 sharetop-2.4.8/sharetop/core/common/config.py
--rw-rw-rw-   0        0        0    22277 2023-08-03 04:22:52.000000 sharetop-2.4.8/sharetop/core/common/explain_change.py
--rw-rw-rw-   0        0        0    12566 2023-08-04 04:02:35.000000 sharetop-2.4.8/sharetop/core/common/getter.py
--rw-rw-rw-   0        0        0      750 2023-04-09 05:42:43.000000 sharetop-2.4.8/sharetop/core/config.py
-drwxrwxrwx   0        0        0        0 2023-08-04 04:23:47.447723 sharetop-2.4.8/sharetop/core/country/
--rw-rw-rw-   0        0        0       91 2023-07-16 02:39:07.000000 sharetop-2.4.8/sharetop/core/country/__init__.py
--rw-rw-rw-   0        0        0      491 2023-05-09 01:30:20.000000 sharetop-2.4.8/sharetop/core/country/config.py
--rw-rw-rw-   0        0        0      807 2023-08-01 23:11:54.000000 sharetop-2.4.8/sharetop/core/country/country_base_info.py
-drwxrwxrwx   0        0        0        0 2023-08-04 04:23:47.454598 sharetop-2.4.8/sharetop/core/fund/
--rw-rw-rw-   0        0        0      996 2023-08-01 14:51:48.000000 sharetop-2.4.8/sharetop/core/fund/__init__.py
--rw-rw-rw-   0        0        0      927 2023-07-28 01:21:27.000000 sharetop-2.4.8/sharetop/core/fund/config.py
--rw-rw-rw-   0        0        0     2727 2023-07-28 00:06:51.000000 sharetop-2.4.8/sharetop/core/fund/fund_list.py
--rw-rw-rw-   0        0        0     1857 2023-07-31 14:52:45.000000 sharetop-2.4.8/sharetop/core/fund/get_fund_base_info.py
--rw-rw-rw-   0        0        0     2624 2023-07-31 15:04:18.000000 sharetop-2.4.8/sharetop/core/fund/get_fund_history_data.py
--rw-rw-rw-   0        0        0     3850 2023-08-01 14:19:07.000000 sharetop-2.4.8/sharetop/core/fund/get_fund_industry_info.py
--rw-rw-rw-   0        0        0     5721 2023-08-01 14:30:58.000000 sharetop-2.4.8/sharetop/core/fund/get_fund_invest_info.py
--rw-rw-rw-   0        0        0    12432 2023-07-31 14:59:03.000000 sharetop-2.4.8/sharetop/core/fund/get_fund_rank.py
--rw-rw-rw-   0        0        0     1466 2023-04-22 03:27:53.000000 sharetop-2.4.8/sharetop/core/fund/get_fund_real_time.py
--rw-rw-rw-   0        0        0     2631 2023-08-01 14:41:19.000000 sharetop-2.4.8/sharetop/core/fund/get_period_change_info.py
--rw-rw-rw-   0        0        0     2561 2023-08-01 14:47:27.000000 sharetop-2.4.8/sharetop/core/fund/get_types_percentage_info.py
-drwxrwxrwx   0        0        0        0 2023-08-04 04:23:47.456234 sharetop-2.4.8/sharetop/core/futures/
--rw-rw-rw-   0        0        0      250 2023-07-16 02:07:46.000000 sharetop-2.4.8/sharetop/core/futures/__init__.py
--rw-rw-rw-   0        0        0    10308 2023-08-01 22:59:24.000000 sharetop-2.4.8/sharetop/core/futures/get_futures_info.py
-drwxrwxrwx   0        0        0        0 2023-08-04 04:23:47.458256 sharetop-2.4.8/sharetop/core/oil/
--rw-rw-rw-   0        0        0      402 2023-05-16 01:17:51.000000 sharetop-2.4.8/sharetop/core/oil/__init__.py
--rw-rw-rw-   0        0        0     1685 2023-05-15 00:28:25.000000 sharetop-2.4.8/sharetop/core/oil/config.py
--rw-rw-rw-   0        0        0     4004 2023-08-02 04:17:10.000000 sharetop-2.4.8/sharetop/core/oil/oil_detail.py
-drwxrwxrwx   0        0        0        0 2023-08-04 04:23:47.460526 sharetop-2.4.8/sharetop/core/pig/
--rw-rw-rw-   0        0        0       84 2023-07-15 10:46:51.000000 sharetop-2.4.8/sharetop/core/pig/__init__.py
--rw-rw-rw-   0        0        0      163 2023-05-16 00:42:46.000000 sharetop-2.4.8/sharetop/core/pig/config.py
--rw-rw-rw-   0        0        0     1538 2023-08-02 13:50:09.000000 sharetop-2.4.8/sharetop/core/pig/pig_detail.py
-drwxrwxrwx   0        0        0        0 2023-08-04 04:23:47.467726 sharetop-2.4.8/sharetop/core/stock/
--rw-rw-rw-   0        0        0      662 2023-07-15 09:27:19.000000 sharetop-2.4.8/sharetop/core/stock/__init__.py
--rw-rw-rw-   0        0        0     4834 2023-07-20 01:18:36.000000 sharetop-2.4.8/sharetop/core/stock/bill_monitor.py
--rw-rw-rw-   0        0        0     1163 2023-07-19 01:27:46.000000 sharetop-2.4.8/sharetop/core/stock/config.py
--rw-rw-rw-   0        0        0    15110 2023-07-20 01:10:32.000000 sharetop-2.4.8/sharetop/core/stock/getter.py
--rw-rw-rw-   0        0        0    10618 2023-08-03 23:05:49.000000 sharetop-2.4.8/sharetop/core/stock/quarterly_report.py
--rw-rw-rw-   0        0        0    10240 2023-07-27 23:27:15.000000 sharetop-2.4.8/sharetop/core/stock/rank_list.py
--rw-rw-rw-   0        0        0      693 2023-07-19 12:30:45.000000 sharetop-2.4.8/sharetop/core/stock/stock_base_info.py
--rw-rw-rw-   0        0        0     7299 2023-07-19 04:12:02.000000 sharetop-2.4.8/sharetop/core/utils.py
-drwxrwxrwx   0        0        0        0 2023-08-04 04:23:47.468736 sharetop-2.4.8/sharetop/crawl/
--rw-rw-rw-   0        0        0       29 2023-04-09 23:19:21.000000 sharetop-2.4.8/sharetop/crawl/__init__.py
--rw-rw-rw-   0        0        0     1088 2023-07-19 05:03:18.000000 sharetop-2.4.8/sharetop/crawl/base.py
--rw-rw-rw-   0        0        0     3271 2023-07-09 23:57:40.000000 sharetop-2.4.8/sharetop/crawl/settings.py
-drwxrwxrwx   0        0        0        0 2023-08-04 04:23:47.470733 sharetop-2.4.8/sharetop/parser/
--rw-rw-rw-   0        0        0       27 2023-04-10 00:54:05.000000 sharetop-2.4.8/sharetop/parser/__init__.py
--rw-rw-rw-   0        0        0     4364 2023-07-19 04:59:24.000000 sharetop-2.4.8/sharetop/parser/base.py
--rw-rw-rw-   0        0        0     2911 2023-07-19 05:36:09.000000 sharetop-2.4.8/sharetop/parser/config.py
-drwxrwxrwx   0        0        0        0 2023-08-04 04:23:47.482308 sharetop-2.4.8/sharetop/test/
--rw-rw-rw-   0        0        0        0 2023-04-29 10:57:35.000000 sharetop-2.4.8/sharetop/test/__init__.py
--rw-rw-rw-   0        0        0      541 2023-08-01 15:19:39.000000 sharetop-2.4.8/sharetop/test/bond_test.py
--rw-rw-rw-   0        0        0      199 2023-05-17 04:49:54.000000 sharetop-2.4.8/sharetop/test/captial.py
--rw-rw-rw-   0        0        0      162 2023-08-01 23:04:30.000000 sharetop-2.4.8/sharetop/test/country_test.py
--rw-rw-rw-   0        0        0      582 2023-07-25 15:03:47.000000 sharetop-2.4.8/sharetop/test/flow_monitor_test.py
--rw-rw-rw-   0        0        0     1691 2023-08-01 14:51:22.000000 sharetop-2.4.8/sharetop/test/fund_test.py
--rw-rw-rw-   0        0        0      418 2023-08-01 23:01:15.000000 sharetop-2.4.8/sharetop/test/futures_test.py
--rw-rw-rw-   0        0        0      692 2023-08-02 04:13:46.000000 sharetop-2.4.8/sharetop/test/oil_test.py
--rw-rw-rw-   0        0        0      217 2023-08-02 04:46:46.000000 sharetop-2.4.8/sharetop/test/pig_test.py
--rw-rw-rw-   0        0        0     1281 2023-08-04 04:15:06.000000 sharetop-2.4.8/sharetop/test/stock_test.py
--rw-rw-rw-   0        0        0      992 2023-07-17 01:23:58.000000 sharetop-2.4.8/sharetop/test/test1.py
--rw-rw-rw-   0        0        0     1997 2023-05-02 03:48:40.000000 sharetop-2.4.8/sharetop/test/test2-akshare.py
--rw-rw-rw-   0        0        0     3709 2023-05-03 07:10:48.000000 sharetop-2.4.8/sharetop/test/test3.py
--rw-rw-rw-   0        0        0      221 2023-07-30 10:45:50.000000 sharetop-2.4.8/sharetop/test/test4.py
--rw-rw-rw-   0        0        0      690 2023-07-15 03:35:15.000000 sharetop-2.4.8/sharetop/test/test5.py
--rw-rw-rw-   0        0        0     1227 2023-07-15 03:35:15.000000 sharetop-2.4.8/sharetop/test/test6.py
--rw-rw-rw-   0        0        0      643 2023-07-05 12:16:23.000000 sharetop-2.4.8/sharetop/test/test7.py
-drwxrwxrwx   0        0        0        0 2023-08-04 04:23:47.424620 sharetop-2.4.8/sharetop.egg-info/
--rw-rw-rw-   0        0        0    51253 2023-08-04 04:23:47.000000 sharetop-2.4.8/sharetop.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2456 2023-08-04 04:23:47.000000 sharetop-2.4.8/sharetop.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-04 04:23:47.000000 sharetop-2.4.8/sharetop.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-08-04 04:23:47.000000 sharetop-2.4.8/sharetop.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-08-04 04:23:47.000000 sharetop-2.4.8/sharetop.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-08 12:48:08.215751 sharetop-2.4.9/
+-rw-rw-rw-   0        0        0     1066 2023-04-26 14:07:21.000000 sharetop-2.4.9/LICENSE
+-rw-rw-rw-   0        0        0    51253 2023-08-08 12:48:08.215751 sharetop-2.4.9/PKG-INFO
+-rw-rw-rw-   0        0        0    49774 2023-07-15 03:35:16.000000 sharetop-2.4.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-08 12:48:08.215751 sharetop-2.4.9/setup.cfg
+-rw-rw-rw-   0        0        0     1219 2023-04-29 06:50:50.000000 sharetop-2.4.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-08 12:48:07.590475 sharetop-2.4.9/sharetop/
+-rw-rw-rw-   0        0        0      297 2023-05-18 12:23:41.000000 sharetop-2.4.9/sharetop/__init__.py
+-rw-rw-rw-   0        0        0      386 2023-08-08 12:48:02.000000 sharetop-2.4.9/sharetop/__version__.py
+drwxrwxrwx   0        0        0        0 2023-08-08 12:48:07.629220 sharetop-2.4.9/sharetop/api/
+-rw-rw-rw-   0        0        0      306 2023-07-02 13:11:41.000000 sharetop-2.4.9/sharetop/api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-08 12:48:07.640716 sharetop-2.4.9/sharetop/application/
+-rw-rw-rw-   0        0        0       33 2023-04-21 11:53:52.000000 sharetop-2.4.9/sharetop/application/__init__.py
+-rw-rw-rw-   0        0        0     4461 2023-08-03 04:20:19.000000 sharetop-2.4.9/sharetop/application/base.py
+drwxrwxrwx   0        0        0        0 2023-08-08 12:48:07.656568 sharetop-2.4.9/sharetop/core/
+-rw-rw-rw-   0        0        0        0 2023-04-08 05:23:09.000000 sharetop-2.4.9/sharetop/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-08 12:48:07.713342 sharetop-2.4.9/sharetop/core/bond/
+-rw-rw-rw-   0        0        0      592 2023-07-15 11:00:24.000000 sharetop-2.4.9/sharetop/core/bond/__init__.py
+-rw-rw-rw-   0        0        0     1869 2023-04-24 04:28:03.000000 sharetop-2.4.9/sharetop/core/bond/config.py
+-rw-rw-rw-   0        0        0     9767 2023-08-01 15:18:53.000000 sharetop-2.4.9/sharetop/core/bond/get_bond_info.py
+-rw-rw-rw-   0        0        0    19614 2023-07-15 10:59:53.000000 sharetop-2.4.9/sharetop/core/bond/get_bond_public_info.py
+-rw-rw-rw-   0        0        0      598 2023-04-10 05:06:06.000000 sharetop-2.4.9/sharetop/core/cache.py
+drwxrwxrwx   0        0        0        0 2023-08-08 12:48:07.728988 sharetop-2.4.9/sharetop/core/capital_flow/
+-rw-rw-rw-   0        0        0      367 2023-07-15 15:19:38.000000 sharetop-2.4.9/sharetop/core/capital_flow/__init__.py
+-rw-rw-rw-   0        0        0     6785 2023-07-25 15:02:39.000000 sharetop-2.4.9/sharetop/core/capital_flow/capital_flow_monitor.py
+drwxrwxrwx   0        0        0        0 2023-08-08 12:48:07.757486 sharetop-2.4.9/sharetop/core/common/
+-rw-rw-rw-   0        0        0      188 2023-04-27 15:24:55.000000 sharetop-2.4.9/sharetop/core/common/__init__.py
+-rw-rw-rw-   0        0        0     3727 2023-07-19 03:47:04.000000 sharetop-2.4.9/sharetop/core/common/common_base.py
+-rw-rw-rw-   0        0        0     8688 2023-05-25 01:16:42.000000 sharetop-2.4.9/sharetop/core/common/config.py
+-rw-rw-rw-   0        0        0    22277 2023-08-03 04:22:52.000000 sharetop-2.4.9/sharetop/core/common/explain_change.py
+-rw-rw-rw-   0        0        0    12505 2023-08-08 01:03:37.000000 sharetop-2.4.9/sharetop/core/common/getter.py
+-rw-rw-rw-   0        0        0      750 2023-04-09 05:42:43.000000 sharetop-2.4.9/sharetop/core/config.py
+drwxrwxrwx   0        0        0        0 2023-08-08 12:48:07.774819 sharetop-2.4.9/sharetop/core/country/
+-rw-rw-rw-   0        0        0       91 2023-07-16 02:39:07.000000 sharetop-2.4.9/sharetop/core/country/__init__.py
+-rw-rw-rw-   0        0        0      491 2023-05-09 01:30:20.000000 sharetop-2.4.9/sharetop/core/country/config.py
+-rw-rw-rw-   0        0        0      806 2023-08-08 01:29:24.000000 sharetop-2.4.9/sharetop/core/country/country_base_info.py
+drwxrwxrwx   0        0        0        0 2023-08-08 12:48:07.878591 sharetop-2.4.9/sharetop/core/fund/
+-rw-rw-rw-   0        0        0      996 2023-08-01 14:51:48.000000 sharetop-2.4.9/sharetop/core/fund/__init__.py
+-rw-rw-rw-   0        0        0      927 2023-07-28 01:21:27.000000 sharetop-2.4.9/sharetop/core/fund/config.py
+-rw-rw-rw-   0        0        0     2752 2023-08-05 00:42:20.000000 sharetop-2.4.9/sharetop/core/fund/fund_list.py
+-rw-rw-rw-   0        0        0     1857 2023-07-31 14:52:45.000000 sharetop-2.4.9/sharetop/core/fund/get_fund_base_info.py
+-rw-rw-rw-   0        0        0     2624 2023-07-31 15:04:18.000000 sharetop-2.4.9/sharetop/core/fund/get_fund_history_data.py
+-rw-rw-rw-   0        0        0     3850 2023-08-01 14:19:07.000000 sharetop-2.4.9/sharetop/core/fund/get_fund_industry_info.py
+-rw-rw-rw-   0        0        0     5767 2023-08-07 04:08:26.000000 sharetop-2.4.9/sharetop/core/fund/get_fund_invest_info.py
+-rw-rw-rw-   0        0        0    12496 2023-08-06 15:01:56.000000 sharetop-2.4.9/sharetop/core/fund/get_fund_rank.py
+-rw-rw-rw-   0        0        0     1466 2023-04-22 03:27:53.000000 sharetop-2.4.9/sharetop/core/fund/get_fund_real_time.py
+-rw-rw-rw-   0        0        0     2631 2023-08-01 14:41:19.000000 sharetop-2.4.9/sharetop/core/fund/get_period_change_info.py
+-rw-rw-rw-   0        0        0     2561 2023-08-07 05:37:01.000000 sharetop-2.4.9/sharetop/core/fund/get_types_percentage_info.py
+drwxrwxrwx   0        0        0        0 2023-08-08 12:48:07.908769 sharetop-2.4.9/sharetop/core/futures/
+-rw-rw-rw-   0        0        0      250 2023-07-16 02:07:46.000000 sharetop-2.4.9/sharetop/core/futures/__init__.py
+-rw-rw-rw-   0        0        0    10308 2023-08-01 22:59:24.000000 sharetop-2.4.9/sharetop/core/futures/get_futures_info.py
+drwxrwxrwx   0        0        0        0 2023-08-08 12:48:07.930362 sharetop-2.4.9/sharetop/core/oil/
+-rw-rw-rw-   0        0        0      402 2023-05-16 01:17:51.000000 sharetop-2.4.9/sharetop/core/oil/__init__.py
+-rw-rw-rw-   0        0        0     1685 2023-05-15 00:28:25.000000 sharetop-2.4.9/sharetop/core/oil/config.py
+-rw-rw-rw-   0        0        0     3993 2023-08-08 10:21:41.000000 sharetop-2.4.9/sharetop/core/oil/oil_detail.py
+drwxrwxrwx   0        0        0        0 2023-08-08 12:48:07.950598 sharetop-2.4.9/sharetop/core/pig/
+-rw-rw-rw-   0        0        0       84 2023-07-15 10:46:51.000000 sharetop-2.4.9/sharetop/core/pig/__init__.py
+-rw-rw-rw-   0        0        0      163 2023-05-16 00:42:46.000000 sharetop-2.4.9/sharetop/core/pig/config.py
+-rw-rw-rw-   0        0        0     1538 2023-08-02 13:50:09.000000 sharetop-2.4.9/sharetop/core/pig/pig_detail.py
+drwxrwxrwx   0        0        0        0 2023-08-08 12:48:08.014895 sharetop-2.4.9/sharetop/core/stock/
+-rw-rw-rw-   0        0        0      662 2023-07-15 09:27:19.000000 sharetop-2.4.9/sharetop/core/stock/__init__.py
+-rw-rw-rw-   0        0        0     4834 2023-07-20 01:18:36.000000 sharetop-2.4.9/sharetop/core/stock/bill_monitor.py
+-rw-rw-rw-   0        0        0     1163 2023-07-19 01:27:46.000000 sharetop-2.4.9/sharetop/core/stock/config.py
+-rw-rw-rw-   0        0        0    15110 2023-07-20 01:10:32.000000 sharetop-2.4.9/sharetop/core/stock/getter.py
+-rw-rw-rw-   0        0        0    10618 2023-08-03 23:05:49.000000 sharetop-2.4.9/sharetop/core/stock/quarterly_report.py
+-rw-rw-rw-   0        0        0    10240 2023-07-27 23:27:15.000000 sharetop-2.4.9/sharetop/core/stock/rank_list.py
+-rw-rw-rw-   0        0        0      693 2023-07-19 12:30:45.000000 sharetop-2.4.9/sharetop/core/stock/stock_base_info.py
+-rw-rw-rw-   0        0        0     7299 2023-07-19 04:12:02.000000 sharetop-2.4.9/sharetop/core/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-08 12:48:08.055406 sharetop-2.4.9/sharetop/crawl/
+-rw-rw-rw-   0        0        0       29 2023-04-09 23:19:21.000000 sharetop-2.4.9/sharetop/crawl/__init__.py
+-rw-rw-rw-   0        0        0     1088 2023-07-19 05:03:18.000000 sharetop-2.4.9/sharetop/crawl/base.py
+-rw-rw-rw-   0        0        0     3271 2023-07-09 23:57:40.000000 sharetop-2.4.9/sharetop/crawl/settings.py
+drwxrwxrwx   0        0        0        0 2023-08-08 12:48:08.087690 sharetop-2.4.9/sharetop/parser/
+-rw-rw-rw-   0        0        0       27 2023-04-10 00:54:05.000000 sharetop-2.4.9/sharetop/parser/__init__.py
+-rw-rw-rw-   0        0        0     4364 2023-07-19 04:59:24.000000 sharetop-2.4.9/sharetop/parser/base.py
+-rw-rw-rw-   0        0        0     2911 2023-07-19 05:36:09.000000 sharetop-2.4.9/sharetop/parser/config.py
+drwxrwxrwx   0        0        0        0 2023-08-08 12:48:08.215751 sharetop-2.4.9/sharetop/test/
+-rw-rw-rw-   0        0        0        0 2023-04-29 10:57:35.000000 sharetop-2.4.9/sharetop/test/__init__.py
+-rw-rw-rw-   0        0        0      541 2023-08-07 14:59:14.000000 sharetop-2.4.9/sharetop/test/bond_test.py
+-rw-rw-rw-   0        0        0      199 2023-05-17 04:49:54.000000 sharetop-2.4.9/sharetop/test/captial.py
+-rw-rw-rw-   0        0        0      189 2023-08-08 01:25:19.000000 sharetop-2.4.9/sharetop/test/country_test.py
+-rw-rw-rw-   0        0        0      578 2023-08-04 23:21:57.000000 sharetop-2.4.9/sharetop/test/flow_monitor_test.py
+-rw-rw-rw-   0        0        0     1762 2023-08-07 05:34:03.000000 sharetop-2.4.9/sharetop/test/fund_test.py
+-rw-rw-rw-   0        0        0      418 2023-08-08 01:11:58.000000 sharetop-2.4.9/sharetop/test/futures_test.py
+-rw-rw-rw-   0        0        0      693 2023-08-08 10:20:17.000000 sharetop-2.4.9/sharetop/test/oil_test.py
+-rw-rw-rw-   0        0        0      234 2023-08-08 10:31:23.000000 sharetop-2.4.9/sharetop/test/pig_test.py
+-rw-rw-rw-   0        0        0     1266 2023-08-04 23:58:06.000000 sharetop-2.4.9/sharetop/test/stock_test.py
+-rw-rw-rw-   0        0        0      992 2023-07-17 01:23:58.000000 sharetop-2.4.9/sharetop/test/test1.py
+-rw-rw-rw-   0        0        0     1997 2023-05-02 03:48:40.000000 sharetop-2.4.9/sharetop/test/test2-akshare.py
+-rw-rw-rw-   0        0        0     3709 2023-05-03 07:10:48.000000 sharetop-2.4.9/sharetop/test/test3.py
+-rw-rw-rw-   0        0        0      221 2023-07-30 10:45:50.000000 sharetop-2.4.9/sharetop/test/test4.py
+-rw-rw-rw-   0        0        0      690 2023-07-15 03:35:15.000000 sharetop-2.4.9/sharetop/test/test5.py
+-rw-rw-rw-   0        0        0     1227 2023-07-15 03:35:15.000000 sharetop-2.4.9/sharetop/test/test6.py
+-rw-rw-rw-   0        0        0      643 2023-07-05 12:16:23.000000 sharetop-2.4.9/sharetop/test/test7.py
+drwxrwxrwx   0        0        0        0 2023-08-08 12:48:07.612824 sharetop-2.4.9/sharetop.egg-info/
+-rw-rw-rw-   0        0        0    51253 2023-08-08 12:48:07.000000 sharetop-2.4.9/sharetop.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2456 2023-08-08 12:48:07.000000 sharetop-2.4.9/sharetop.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 12:48:07.000000 sharetop-2.4.9/sharetop.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-08-08 12:48:07.000000 sharetop-2.4.9/sharetop.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-08-08 12:48:07.000000 sharetop-2.4.9/sharetop.egg-info/top_level.txt
```

### Comparing `sharetop-2.4.8/LICENSE` & `sharetop-2.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.8/PKG-INFO` & `sharetop-2.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sharetop
-Version: 2.4.8
+Version: 2.4.9
 Summary: Provide data related to the economic market
 Home-page: https://github.com/nrliangxy/sharetop
 Author: nrliangxy
 Author-email: nrliangxy@foxmail.com
 License: MIT
 Project-URL: Source, https://github.com/nrliangxy/sharetop
 Keywords: data,finance,quant,stock,fund,futures,share
```

### Comparing `sharetop-2.4.8/README.md` & `sharetop-2.4.9/README.md`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.8/setup.py` & `sharetop-2.4.9/setup.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.8/sharetop/application/base.py` & `sharetop-2.4.9/sharetop/application/base.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.8/sharetop/core/bond/__init__.py` & `sharetop-2.4.9/sharetop/core/bond/__init__.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.8/sharetop/core/bond/config.py` & `sharetop-2.4.9/sharetop/core/bond/config.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.8/sharetop/core/bond/get_bond_info.py` & `sharetop-2.4.9/sharetop/core/bond/get_bond_info.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.8/sharetop/core/bond/get_bond_public_info.py` & `sharetop-2.4.9/sharetop/core/bond/get_bond_public_info.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.8/sharetop/core/cache.py` & `sharetop-2.4.9/sharetop/core/cache.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.8/sharetop/core/capital_flow/capital_flow_monitor.py` & `sharetop-2.4.9/sharetop/core/capital_flow/capital_flow_monitor.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.8/sharetop/core/common/common_base.py` & `sharetop-2.4.9/sharetop/core/common/common_base.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.8/sharetop/core/common/config.py` & `sharetop-2.4.9/sharetop/core/common/config.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.8/sharetop/core/common/explain_change.py` & `sharetop-2.4.9/sharetop/core/common/explain_change.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.8/sharetop/core/common/getter.py` & `sharetop-2.4.9/sharetop/core/common/getter.py`

 * *Files 0% similar despite different names*

```diff
@@ -330,15 +330,14 @@
         ('invt', '2'),
         ('fltt', '2'),
         ('fields', fields),
         ('secid', quote_id),
     )
     url = 'http://push2.eastmoney.com/api/qt/stock/get'
     json_response = requests_obj.get(url, params, headers=EASTMONEY_REQUEST_HEADERS).json()
-    print("json_response=================:", json_response)
     items = json_response['data']
     if not items:
         return pd.Series(index=EASTMONEY_BASE_INFO_FIELDS.values(), dtype='object')
     s = pd.Series(items, dtype='object').rename(index=EASTMONEY_BASE_INFO_FIELDS)
     return s
```

### Comparing `sharetop-2.4.8/sharetop/core/config.py` & `sharetop-2.4.9/sharetop/core/config.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.8/sharetop/core/country/country_base_info.py` & `sharetop-2.4.9/sharetop/core/country/country_base_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from .config import country_base_url, country_field_dict
 from ...crawl.settings import *
 from ..utils import to_numeric, requests_obj, parse_obj
 from ..common.explain_change import exchange_explain
 
 
 @to_numeric
-def get_country_list(token: str, limit: int = None, is_explain: bool = False) -> pd.DataFrame:
+def get_country_list(token: str, limit: int = 100, is_explain: bool = False) -> pd.DataFrame:
     """
     国家基本信息列表
     :param token:
     :param limit:
     :return:
     """
     headers = {"token": token}
```

### Comparing `sharetop-2.4.8/sharetop/core/fund/__init__.py` & `sharetop-2.4.9/sharetop/core/fund/__init__.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.8/sharetop/core/fund/config.py` & `sharetop-2.4.9/sharetop/core/fund/config.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.8/sharetop/core/fund/fund_list.py` & `sharetop-2.4.9/sharetop/core/fund/fund_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import re
 import pandas as pd
 from retry import retry
-from ..utils import requests_obj, validate_request
+from ..utils import requests_obj, validate_request, to_numeric
 from ..common.getter import BaseApplication
 from ..common.explain_change import exchange_explain
 
 
 @validate_request
+@to_numeric
 @retry(tries=3)
 def get_fund_codes(token: str, ft: str = None, is_explain: bool = False) -> pd.DataFrame:
     """
     获取天天基金网公开的全部公墓基金名单
     Parameters
     ----------
     ft : str, optional
```

### Comparing `sharetop-2.4.8/sharetop/core/fund/get_fund_base_info.py` & `sharetop-2.4.9/sharetop/core/fund/get_fund_base_info.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.8/sharetop/core/fund/get_fund_history_data.py` & `sharetop-2.4.9/sharetop/core/fund/get_fund_history_data.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.8/sharetop/core/fund/get_fund_industry_info.py` & `sharetop-2.4.9/sharetop/core/fund/get_fund_industry_info.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.8/sharetop/core/fund/get_fund_invest_info.py` & `sharetop-2.4.9/sharetop/core/fund/get_fund_invest_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import uuid
 import pandas as pd
-from typing import List, Union
+from typing import List, Union, Dict, Any
 from retry import retry
 from ..utils import to_numeric, requests_obj, validate_request
 from jsonpath import jsonpath
 from .config import EastmoneyFundHeaders
 from ..common.explain_change import exchange_explain
 
 
@@ -111,15 +111,15 @@
     if not dfs:
         return pd.DataFrame(columns=fields)
     df = pd.concat(dfs, axis=0, ignore_index=True).rename(columns=columns)[fields]
     return exchange_explain(df, is_explain)
 
 
 @validate_request
-def get_fund_public_dates(token: str, fund_code: str) -> List[str]:
+def get_fund_public_dates(token: str, fund_code: str) -> Dict[str, Any]:
     """
     获取历史上更新持仓情况的日期列表
     Parameters
     ----------
     fund_code : str
         6 位基金代码
     Returns
@@ -138,9 +138,9 @@
         ('product', 'EFund'),
         ('serverVersion', '6.3.6'),
         ('version', '6.3.8'),
     )
     url = 'https://fundmobapi.eastmoney.com/FundMNewApi/FundMNIVInfoMultiple'
     json_response = requests_obj.get(url, params, headers=EastmoneyFundHeaders).json()
     if json_response['Datas'] is None:
-        return []
-    return json_response['Datas']
+        return {"date_list": []}
+    return {"date_list": json_response['Datas']}
```

### Comparing `sharetop-2.4.8/sharetop/core/fund/get_fund_rank.py` & `sharetop-2.4.9/sharetop/core/fund/get_fund_rank.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import requests
 import datetime
 import re
 import pandas as pd
-from ..utils import requests_obj, parse_obj, validate_request
+from ..utils import requests_obj, parse_obj, validate_request, to_numeric
 from .config import fund_money_cloumns
 from ..common.explain_change import exchange_explain
 
 
 def fund_export_df(text_data):
     json_data = parse_obj.parse_fund_json(text_data)
     temp_df = pd.DataFrame(json_data)
     temp_df = temp_df.iloc[:, 0].str.split(",", expand=True)
     temp_df.reset_index(inplace=True)
     temp_df["index"] = list(range(1, len(temp_df) + 1))
     return temp_df
 
 
+@to_numeric
 @validate_request
 def get_fund_open_rank(token: str, symbol: str = "全部", is_explain: bool = False) -> pd.DataFrame:
     """
     东方财富网-数据中心-开放基金排行
     https://fund.eastmoney.com/data/fundranking.html
     :param token:
     :param is_explain:
@@ -113,14 +114,15 @@
             "成立来",
             "手续费",
         ]
     ]
     return exchange_explain(temp_df, is_explain)
 
 
+@to_numeric
 @validate_request
 def get_fund_exchange_rank(token: str, is_explain: bool = False) -> pd.DataFrame:
     """
     东方财富网-数据中心-场内交易基金排行
     https://fund.eastmoney.com/data/fbsfundranking.html
     :return: 场内交易基金数据
     :rtype: pandas.DataFrame
@@ -204,14 +206,15 @@
     # temp_df['近2年'] = pd.to_numeric(temp_df['近2年'], errors="coerce")
     # temp_df['近3年'] = pd.to_numeric(temp_df['近3年'], errors="coerce")
     # temp_df['今年来'] = pd.to_numeric(temp_df['今年来'], errors="coerce")
     # temp_df['成立来'] = pd.to_numeric(temp_df['成立来'], errors="coerce")
     return exchange_explain(temp_df, is_explain)
 
 
+@to_numeric
 @validate_request
 def get_fund_money_rank(token: str, is_explain: bool = False) -> pd.DataFrame:
     """
     东方财富网-数据中心-货币型基金排行
     https://fund.eastmoney.com/data/hbxfundranking.html
     :return: 货币型基金排行
     :rtype: pandas.DataFrame
@@ -257,14 +260,15 @@
     # temp_df['近3年'] = pd.to_numeric(temp_df['近3年'], errors="coerce")
     # temp_df['近5年'] = pd.to_numeric(temp_df['近5年'], errors="coerce")
     # temp_df['今年来'] = pd.to_numeric(temp_df['今年来'], errors="coerce")
     # temp_df['成立来'] = pd.to_numeric(temp_df['成立来'], errors="coerce")
     return exchange_explain(temp_df, is_explain)
 
 
+@to_numeric
 @validate_request
 def get_fund_hk_rank(token: str, is_explain: bool = False) -> pd.DataFrame:
     """
     东方财富网-数据中心-香港基金排行
     https://overseas.1234567.com.cn/FundList
     :return: 香港基金排行
     :rtype: pandas.DataFrame
```

### Comparing `sharetop-2.4.8/sharetop/core/fund/get_fund_real_time.py` & `sharetop-2.4.9/sharetop/core/fund/get_fund_real_time.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.8/sharetop/core/fund/get_period_change_info.py` & `sharetop-2.4.9/sharetop/core/fund/get_period_change_info.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.8/sharetop/core/fund/get_types_percentage_info.py` & `sharetop-2.4.9/sharetop/core/fund/get_types_percentage_info.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.8/sharetop/core/futures/get_futures_info.py` & `sharetop-2.4.9/sharetop/core/futures/get_futures_info.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.8/sharetop/core/oil/config.py` & `sharetop-2.4.9/sharetop/core/oil/config.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.8/sharetop/core/oil/oil_detail.py` & `sharetop-2.4.9/sharetop/core/oil/oil_detail.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,70 +32,70 @@
     if isinstance(r, dict):
         return r
     data_json = r.json()
     df = parse_obj.parse_god_cup_json(data_json, field_dict)
     return df
 
 
-def get_oil_reserves(token: str, data_type: str = None, limit: int = None, is_explain: bool = False) -> pd.DataFrame:
+def get_oil_reserves(token: str, data_type: str = '1', limit: int = 100, is_explain: bool = False) -> pd.DataFrame:
     """
     获取机构的石油储量
     :param token:
     :param data_type: 1为国家数据 2为机构数据 4为大洲数据
     :param limit:
     :return:
     """
     return exchange_explain(get_oil_data_common(token, oil_reserves_url, oil_reserves_field_dict, data_type, limit), is_explain)
 
 
-def get_oil_products(token: str, data_type: str = None, limit: int = None, is_explain: bool = False) -> pd.DataFrame:
+def get_oil_products(token: str, data_type: str = '1', limit: int = 100, is_explain: bool = False) -> pd.DataFrame:
     """
     获取机构的石油产量
     :param token:
     :param data_type: 1为国家数据 2为机构数据 4为大洲数据
     :param limit:
     :return:
     """
     return exchange_explain(get_oil_data_common(token, oil_products_url, oil_products_field_dict, data_type, limit), is_explain)
 
 
-def get_oil_consumption(token: str, data_type: str = None, limit: int = None, is_explain: bool = False) -> pd.DataFrame:
+def get_oil_consumption(token: str, data_type: str = '1', limit: int = 100, is_explain: bool = False) -> pd.DataFrame:
     """
     获取机构的消费量
     :param token:
     :param data_type: 1为国家数据 2为机构数据 4为大洲数据
     :param limit:
     :return:
     """
     return exchange_explain(get_oil_data_common(token, oil_consumption_url, oil_consumption_field_dict, data_type, limit), is_explain)
 
 
-def get_oil_refinerythroughput(token: str, data_type: str = None, limit: int = None, is_explain: bool = False) -> pd.DataFrame:
+def get_oil_refinerythroughput(token: str, data_type: str = '1', limit: int = 100, is_explain: bool = False) -> pd.DataFrame:
     """
     获取石油的加工量
     :param token:
     :param data_type: 1为国家数据 2为机构数据 4为大洲数据
     :param limit:
     :return:
     """
     return exchange_explain(get_oil_data_common(token, oil_refinerythroughput_url, oil_refinerythroughput_field_dict, data_type, limit), is_explain)
 
 
-def get_oil_refinerycapacity(token: str, data_type: str = None, limit: int = None, is_explain: bool = False) -> pd.DataFrame:
+def get_oil_refinerycapacity(token: str, data_type: str = '1', limit: int = 100, is_explain: bool = False) -> pd.DataFrame:
     """
     获取石油的产能
     :param token:
     :param data_type: 1为国家数据 2为机构数据 4为大洲数据
     :param limit:
     :return:
     """
     return exchange_explain(get_oil_data_common(token, oil_refinerycapacity_url, oil_refinerycapacity_field_dict, data_type, limit), is_explain)
 
 
-def get_oil_crudeoilpricehistory(token: str, limit: int = None, is_explain: bool = False) -> pd.DataFrame:
+def get_oil_crudeoilpricehistory(token: str, limit: int = 100, is_explain: bool = False) -> pd.DataFrame:
     """
     获取石油的历史价格
     :param token:
     :param limit: 数据限制
     :return:
     """
     return exchange_explain(get_oil_data_common(token, oil_crudeoilpricehistory_url, oil_crudeoilpricehistory_field_dict, limit=limit), is_explain)
```

### Comparing `sharetop-2.4.8/sharetop/core/pig/pig_detail.py` & `sharetop-2.4.9/sharetop/core/pig/pig_detail.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.8/sharetop/core/stock/__init__.py` & `sharetop-2.4.9/sharetop/core/stock/__init__.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.8/sharetop/core/stock/bill_monitor.py` & `sharetop-2.4.9/sharetop/core/stock/bill_monitor.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.8/sharetop/core/stock/config.py` & `sharetop-2.4.9/sharetop/core/stock/config.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.8/sharetop/core/stock/getter.py` & `sharetop-2.4.9/sharetop/core/stock/getter.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.8/sharetop/core/stock/quarterly_report.py` & `sharetop-2.4.9/sharetop/core/stock/quarterly_report.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.8/sharetop/core/stock/rank_list.py` & `sharetop-2.4.9/sharetop/core/stock/rank_list.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.8/sharetop/core/stock/stock_base_info.py` & `sharetop-2.4.9/sharetop/core/stock/stock_base_info.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.8/sharetop/core/utils.py` & `sharetop-2.4.9/sharetop/core/utils.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.8/sharetop/crawl/base.py` & `sharetop-2.4.9/sharetop/crawl/base.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.8/sharetop/crawl/settings.py` & `sharetop-2.4.9/sharetop/crawl/settings.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.8/sharetop/parser/base.py` & `sharetop-2.4.9/sharetop/parser/base.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.8/sharetop/parser/config.py` & `sharetop-2.4.9/sharetop/parser/config.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.8/sharetop/test/bond_test.py` & `sharetop-2.4.9/sharetop/test/bond_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,14 @@
 token = "f109298d079b5f60"
 
 
 # d = bond_treasure_issue_cninfo()
 
 # d = bond_local_government_issue_cninfo()
 
-# d = get_bond_base_info(token, "113672")
-d = get_bond_public(token)
+d = get_bond_base_info(token, "113672")
+# d = get_bond_public(token)
 # d = get_bond_base_info_list(token)
 
 # d = get_bond_realtime_quotes()
 
 print(d.to_dict("records"))
```

### Comparing `sharetop-2.4.8/sharetop/test/flow_monitor_test.py` & `sharetop-2.4.9/sharetop/test/flow_monitor_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,10 +7,10 @@
 
 # d = get_stock_real_time_daily_capital(stock_code, is_explain=True)
 
 # d = get_stock_history_capital(token, stock_code, is_explain=False)
 
 # d = get_stock_real_time_sum_capital(stock_code, is_explain=True)
 
-d = get_stock_real_time_sector_capital("industry", "1", is_explain=True)
+d = get_stock_real_time_sector_capital("area", "1", is_explain=True)
 
 print("d====:", d.to_dict("records"))
```

### Comparing `sharetop-2.4.8/sharetop/test/fund_test.py` & `sharetop-2.4.9/sharetop/test/fund_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,39 +7,39 @@
 from sharetop.core.fund.get_period_change_info import get_fund_period_change
 from sharetop.core.fund.get_types_percentage_info import get_fund_types_percentage
 from sharetop.core.fund.get_fund_real_time import get_fund_real_time_god
 
 
 token = "f109298d079b5f60"
 
-# d = get_fund_base_info(token, "001299")
+# d = get_fund_base_info(token, "001299", is_explain=False)
 
 # d = get_fund_history_price(token, "001299", is_explain=True)
 
 # d = get_public_dates(token, "001299")
 
-# d = get_fund_industry_distribution(token, "161725", "2023-03-31")
+# d = get_fund_industry_distribution(token, "161725", "2023-03-31", is_explain=False)
 
 # d = get_fund_invest_position(token, "161725", "2023-03-31")
 
 # d = get_fund_public_dates(token, "161725")
 
 # d = fund_open_fund_rank(token, "债券型")
 
-# d = get_fund_open_rank(token, is_explain=True)
+# d = get_fund_open_rank(token, is_explain=False)
 
-# d = get_fund_exchange_rank(token)
+# d = get_fund_exchange_rank(token, is_explain=True)
 
 # d = get_fund_money_rank(token)
 
-# d = get_fund_period_change(token, "161725")
+# d = get_fund_period_change(token, "161725", is_explain=True)
 
-# d = get_fund_types_percentage(token, "161725")
+d = get_fund_types_percentage(token, "161725")
 
-d = get_fund_real_time_god("161725")
+# d = get_fund_real_time_god("161725")
 # d = fund_money_rank(token)
 
 # d = get_period_change(token, "001299")
 
 # d = get_types_percentage(token, "001299")
 
 # d = get_fund_codes(token, is_explain=True)
```

### Comparing `sharetop-2.4.8/sharetop/test/oil_test.py` & `sharetop-2.4.9/sharetop/test/oil_test.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import time
 
 from sharetop.core.oil.oil_detail import get_oil_reserves, get_oil_products, get_oil_consumption,\
     get_oil_refinerythroughput, get_oil_refinerycapacity, get_oil_crudeoilpricehistory
 
 token = "f109298d079b5f60"
 
-# d1 = get_oil_reserves(token, "1")
+# d2 = get_oil_reserves(token, "1")
 # print(d1)
 #
 # d2 = get_oil_products(token, "1")
 # print(d2)
 
 # d2 = get_oil_consumption(token, "1")
-# d2 = get_oil_refinerythroughput(token, "1", is_explain=True)
+# d2 = get_oil_refinerythroughput(token, "1", is_explain=False)
 d2 = get_oil_crudeoilpricehistory(token)
 
 # d2 = get_oil_refinerycapacity(token, "1", is_explain=False)
 print(d2.to_dict("records"))
 
 # for i in range(10):
 #     # time.sleep(3)
```

### Comparing `sharetop-2.4.8/sharetop/test/stock_test.py` & `sharetop-2.4.9/sharetop/test/stock_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,33 +4,33 @@
 from sharetop.core.stock.rank_list import get_stock_dragon_tiger_list
 
 from sharetop.core.stock.stock_base_info import get_stock_base_info
 
 token = "f109298d079b5f60"
 
 
-# d = get_stock_kline_data(token, ["002714", "516110"], is_explain=True)
+# d = get_stock_kline_data(token, "516110", is_explain=False)
 
 # d = get_real_time_bill("002714")
 
 # d = get_history_data(token, "002714", klt=102)
 
 # d = get_real_time_data(["002714", "516110"])
 
 # d = get_stock_market_real_time_data(token, is_explain=False)
 
-d = get_stock_company_report_data(token, '002714', None, False)
+# d = get_stock_company_report_data(token, '002714', None, False)
 
 # d = get_stock_all_company_quarterly_report(token, '2013-12-31', is_explain=True)
 
-# d = get_stock_dragon_tiger_list(token, is_explain=True)
+d = get_stock_dragon_tiger_list(token, '2023-07-21', '2023-08-03')
 
-# d = get_stock_base_info(["002714", "562510"])
+# d = get_stock_base_info("002714")
 # d = get_stock_base_info(["002714", "600809"], is_explain=True)
 
 # d = get_stock_all_report_dates(token, is_explain=False)
 
 # d = get_stock_real_time_data("002714", is_explain=False)
 
-print(d.to_dict("records")[1])
+print(d.to_dict("records"))
 
 # print(type(d.to_dict("records")[0]['free_float_market_cap']))
```

### Comparing `sharetop-2.4.8/sharetop/test/test1.py` & `sharetop-2.4.9/sharetop/test/test1.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.8/sharetop/test/test2-akshare.py` & `sharetop-2.4.9/sharetop/test/test2-akshare.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.8/sharetop/test/test3.py` & `sharetop-2.4.9/sharetop/test/test3.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.8/sharetop/test/test5.py` & `sharetop-2.4.9/sharetop/test/test5.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.8/sharetop/test/test6.py` & `sharetop-2.4.9/sharetop/test/test6.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.8/sharetop/test/test7.py` & `sharetop-2.4.9/sharetop/test/test7.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.8/sharetop.egg-info/PKG-INFO` & `sharetop-2.4.9/sharetop.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sharetop
-Version: 2.4.8
+Version: 2.4.9
 Summary: Provide data related to the economic market
 Home-page: https://github.com/nrliangxy/sharetop
 Author: nrliangxy
 Author-email: nrliangxy@foxmail.com
 License: MIT
 Project-URL: Source, https://github.com/nrliangxy/sharetop
 Keywords: data,finance,quant,stock,fund,futures,share
```

### Comparing `sharetop-2.4.8/sharetop.egg-info/SOURCES.txt` & `sharetop-2.4.9/sharetop.egg-info/SOURCES.txt`

 * *Files identical despite different names*

