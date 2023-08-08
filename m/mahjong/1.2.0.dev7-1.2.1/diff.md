# Comparing `tmp/mahjong-1.2.0.dev7.tar.gz` & `tmp/mahjong-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mahjong-1.2.0.dev7.tar", last modified: Sat Oct  9 13:18:54 2021, max compression
+gzip compressed data, was "mahjong-1.2.1.tar", last modified: Tue Aug  8 02:15:33 2023, max compression
```

## Comparing `mahjong-1.2.0.dev7.tar` & `mahjong-1.2.1.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxrwxr-x   0 nihisil   (1000) nihisil   (1000)        0 2021-10-09 13:18:54.324035 mahjong-1.2.0.dev7/
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)     1075 2020-10-28 09:47:37.000000 mahjong-1.2.0.dev7/LICENSE.txt
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)     1471 2021-10-09 13:18:54.324035 mahjong-1.2.0.dev7/PKG-INFO
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)     9678 2021-07-22 12:00:42.000000 mahjong-1.2.0.dev7/README.rst
-drwxrwxr-x   0 nihisil   (1000) nihisil   (1000)        0 2021-10-09 13:18:54.320035 mahjong-1.2.0.dev7/mahjong/
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)        0 2021-10-09 12:51:01.000000 mahjong-1.2.0.dev7/mahjong/__init__.py
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)     6015 2021-07-22 12:00:42.000000 mahjong-1.2.0.dev7/mahjong/agari.py
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      418 2020-11-05 12:55:10.000000 mahjong-1.2.0.dev7/mahjong/constants.py
-drwxrwxr-x   0 nihisil   (1000) nihisil   (1000)        0 2021-10-09 13:18:54.324035 mahjong-1.2.0.dev7/mahjong/hand_calculating/
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)       24 2020-10-28 09:47:37.000000 mahjong-1.2.0.dev7/mahjong/hand_calculating/__init__.py
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)     8300 2021-07-22 12:00:42.000000 mahjong-1.2.0.dev7/mahjong/hand_calculating/divider.py
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)     5806 2021-10-09 12:51:01.000000 mahjong-1.2.0.dev7/mahjong/hand_calculating/fu.py
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)    25649 2021-10-09 12:51:01.000000 mahjong-1.2.0.dev7/mahjong/hand_calculating/hand.py
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)     4398 2021-07-22 12:00:42.000000 mahjong-1.2.0.dev7/mahjong/hand_calculating/hand_config.py
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)     1086 2021-10-09 12:51:01.000000 mahjong-1.2.0.dev7/mahjong/hand_calculating/hand_response.py
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)     9514 2021-10-09 12:51:01.000000 mahjong-1.2.0.dev7/mahjong/hand_calculating/scores.py
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)     1153 2020-11-05 12:55:10.000000 mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku.py
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)     4030 2021-07-22 12:00:42.000000 mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_config.py
-drwxrwxr-x   0 nihisil   (1000) nihisil   (1000)        0 2021-10-09 13:18:54.324035 mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)     2599 2021-07-22 12:00:42.000000 mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/__init__.py
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      531 2021-10-09 12:51:01.000000 mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/aka_dora.py
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      519 2021-10-09 12:51:01.000000 mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/chankan.py
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)     1350 2021-10-09 12:51:01.000000 mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/chantai.py
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      491 2021-10-09 12:51:01.000000 mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/chiitoitsu.py
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)     1103 2021-10-09 12:51:01.000000 mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/chinitsu.py
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      599 2021-10-09 12:51:01.000000 mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/chun.py
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      518 2021-07-22 12:00:42.000000 mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/daburu_open_riichi.py
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      539 2021-10-09 12:51:01.000000 mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/daburu_riichi.py
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      487 2021-10-09 12:51:01.000000 mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/dora.py
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      842 2021-10-09 12:51:01.000000 mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/east.py
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      523 2021-10-09 12:51:01.000000 mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/haitei.py
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      601 2021-10-09 12:51:01.000000 mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/haku.py
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      606 2021-10-09 12:51:01.000000 mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/hatsu.py
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)     1107 2021-10-09 12:51:01.000000 mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/honitsu.py
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      703 2021-10-09 12:51:01.000000 mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/honroto.py
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      523 2021-10-09 12:51:01.000000 mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/houtei.py
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      849 2021-10-09 12:51:01.000000 mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/iipeiko.py
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      522 2021-10-09 12:51:01.000000 mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/ippatsu.py
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)     1462 2021-10-09 12:51:01.000000 mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/ittsu.py
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)     1174 2021-10-09 12:51:01.000000 mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/junchan.py
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      510 2021-10-09 12:51:01.000000 mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/nagashi_mangan.py
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      849 2021-10-09 12:51:01.000000 mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/north.py
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      402 2021-07-22 12:00:42.000000 mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/open_riichi.py
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      455 2021-10-09 12:51:01.000000 mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/pinfu.py
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      520 2021-10-09 12:51:01.000000 mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/renhou.py
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      422 2021-10-09 12:51:01.000000 mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/riichi.py
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      526 2021-10-09 12:51:01.000000 mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/rinshan.py
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      859 2021-10-09 12:51:01.000000 mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/ryanpeiko.py
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)     1479 2021-10-09 12:51:01.000000 mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/sanankou.py
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      620 2021-10-09 12:51:01.000000 mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/sankantsu.py
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)     1417 2021-10-09 12:51:01.000000 mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/sanshoku.py
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)     1495 2021-10-09 12:51:01.000000 mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/sanshoku_douko.py
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      868 2021-10-09 12:51:01.000000 mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/shosangen.py
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      849 2021-10-09 12:51:01.000000 mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/south.py
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      703 2021-10-09 12:51:01.000000 mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/tanyao.py
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      631 2021-10-09 12:51:01.000000 mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/toitoi.py
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      522 2021-10-09 12:51:01.000000 mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/tsumo.py
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      842 2021-10-09 12:51:01.000000 mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/west.py
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      453 2021-10-09 12:51:01.000000 mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/yakuhai_place.py
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      453 2021-10-09 12:51:01.000000 mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/yakuhai_round.py
-drwxrwxr-x   0 nihisil   (1000) nihisil   (1000)        0 2021-10-09 13:18:54.324035 mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/yakuman/
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)     1553 2021-07-22 12:00:42.000000 mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/yakuman/__init__.py
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      339 2021-10-09 12:51:01.000000 mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/yakuman/chiihou.py
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      740 2021-10-09 12:51:01.000000 mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/yakuman/chinroto.py
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)     1835 2021-10-09 12:51:01.000000 mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/yakuman/chuuren_poutou.py
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      525 2021-10-09 12:51:01.000000 mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/yakuman/daburu_chuuren_poutou.py
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      532 2021-10-09 12:51:01.000000 mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/yakuman/daburu_kokushi.py
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      614 2021-07-22 12:00:42.000000 mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/yakuman/daichisei.py
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      784 2021-10-09 12:51:01.000000 mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/yakuman/daisangen.py
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)     2018 2021-10-09 12:51:01.000000 mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/yakuman/daisharin.py
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)     1048 2021-10-09 12:51:01.000000 mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/yakuman/daisuushi.py
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      987 2021-10-09 12:51:01.000000 mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/yakuman/kokushi.py
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      765 2021-07-22 12:00:42.000000 mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/yakuman/paarenchan.py
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      515 2021-10-09 12:51:01.000000 mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/yakuman/renhou_yakuman.py
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      755 2021-10-09 12:51:01.000000 mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/yakuman/ryuisou.py
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      495 2021-07-22 12:00:42.000000 mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/yakuman/sashikomi.py
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)     1086 2021-10-09 12:51:01.000000 mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/yakuman/shosuushi.py
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      903 2021-10-09 12:51:01.000000 mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/yakuman/suuankou.py
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      446 2021-10-09 12:51:01.000000 mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/yakuman/suuankou_tanki.py
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      620 2021-10-09 12:51:01.000000 mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/yakuman/suukantsu.py
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      520 2021-10-09 12:51:01.000000 mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/yakuman/tenhou.py
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      790 2021-10-09 12:51:01.000000 mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/yakuman/tsuisou.py
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)     1133 2021-07-22 12:00:42.000000 mahjong-1.2.0.dev7/mahjong/meld.py
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)    11195 2021-07-22 12:00:42.000000 mahjong-1.2.0.dev7/mahjong/shanten.py
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)     3841 2021-07-22 12:01:37.000000 mahjong-1.2.0.dev7/mahjong/tests_mixin.py
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)     6944 2021-07-22 12:00:42.000000 mahjong-1.2.0.dev7/mahjong/tile.py
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)     6110 2021-07-22 12:00:42.000000 mahjong-1.2.0.dev7/mahjong/utils.py
-drwxrwxr-x   0 nihisil   (1000) nihisil   (1000)        0 2021-10-09 13:18:54.320035 mahjong-1.2.0.dev7/mahjong.egg-info/
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)     1471 2021-10-09 13:18:54.000000 mahjong-1.2.0.dev7/mahjong.egg-info/PKG-INFO
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)     3765 2021-10-09 13:18:54.000000 mahjong-1.2.0.dev7/mahjong.egg-info/SOURCES.txt
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)        1 2021-10-09 13:18:54.000000 mahjong-1.2.0.dev7/mahjong.egg-info/dependency_links.txt
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)        8 2021-10-09 13:18:54.000000 mahjong-1.2.0.dev7/mahjong.egg-info/top_level.txt
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      389 2020-11-05 12:55:10.000000 mahjong-1.2.0.dev7/pyproject.toml
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)       79 2021-10-09 13:18:54.324035 mahjong-1.2.0.dev7/setup.cfg
--rw-rw-r--   0 nihisil   (1000) nihisil   (1000)     1183 2021-10-09 13:18:29.000000 mahjong-1.2.0.dev7/setup.py
+drwxrwxr-x   0 nihisil   (1000) nihisil   (1000)        0 2023-08-08 02:15:33.304046 mahjong-1.2.1/
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)     1075 2023-08-08 00:48:36.000000 mahjong-1.2.1/LICENSE.txt
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)     1578 2023-08-08 02:15:33.304046 mahjong-1.2.1/PKG-INFO
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      770 2023-08-08 00:56:56.000000 mahjong-1.2.1/README.md
+drwxrwxr-x   0 nihisil   (1000) nihisil   (1000)        0 2023-08-08 02:15:33.300045 mahjong-1.2.1/mahjong/
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)        0 2023-08-08 00:48:36.000000 mahjong-1.2.1/mahjong/__init__.py
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)     5983 2023-08-08 00:48:36.000000 mahjong-1.2.1/mahjong/agari.py
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      418 2023-08-08 00:48:36.000000 mahjong-1.2.1/mahjong/constants.py
+drwxrwxr-x   0 nihisil   (1000) nihisil   (1000)        0 2023-08-08 02:15:33.300045 mahjong-1.2.1/mahjong/hand_calculating/
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)       24 2023-08-08 00:48:36.000000 mahjong-1.2.1/mahjong/hand_calculating/__init__.py
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)     8276 2023-08-08 00:48:36.000000 mahjong-1.2.1/mahjong/hand_calculating/divider.py
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)     5773 2023-08-08 00:48:36.000000 mahjong-1.2.1/mahjong/hand_calculating/fu.py
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)    25625 2023-08-08 00:48:36.000000 mahjong-1.2.1/mahjong/hand_calculating/hand.py
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)     4358 2023-08-08 00:48:36.000000 mahjong-1.2.1/mahjong/hand_calculating/hand_config.py
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)     1052 2023-08-08 00:48:36.000000 mahjong-1.2.1/mahjong/hand_calculating/hand_response.py
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)     9482 2023-08-08 00:48:36.000000 mahjong-1.2.1/mahjong/hand_calculating/scores.py
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)     1149 2023-08-08 00:48:36.000000 mahjong-1.2.1/mahjong/hand_calculating/yaku.py
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)     3998 2023-08-08 00:48:36.000000 mahjong-1.2.1/mahjong/hand_calculating/yaku_config.py
+drwxrwxr-x   0 nihisil   (1000) nihisil   (1000)        0 2023-08-08 02:15:33.304046 mahjong-1.2.1/mahjong/hand_calculating/yaku_list/
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)     2599 2023-08-08 00:48:36.000000 mahjong-1.2.1/mahjong/hand_calculating/yaku_list/__init__.py
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      507 2023-08-08 00:48:36.000000 mahjong-1.2.1/mahjong/hand_calculating/yaku_list/aka_dora.py
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      495 2023-08-08 00:48:36.000000 mahjong-1.2.1/mahjong/hand_calculating/yaku_list/chankan.py
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)     1326 2023-08-08 00:48:36.000000 mahjong-1.2.1/mahjong/hand_calculating/yaku_list/chantai.py
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      467 2023-08-08 00:48:36.000000 mahjong-1.2.1/mahjong/hand_calculating/yaku_list/chiitoitsu.py
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)     1079 2023-08-08 00:48:36.000000 mahjong-1.2.1/mahjong/hand_calculating/yaku_list/chinitsu.py
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      575 2023-08-08 00:48:36.000000 mahjong-1.2.1/mahjong/hand_calculating/yaku_list/chun.py
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      494 2023-08-08 00:48:36.000000 mahjong-1.2.1/mahjong/hand_calculating/yaku_list/daburu_open_riichi.py
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      515 2023-08-08 00:48:36.000000 mahjong-1.2.1/mahjong/hand_calculating/yaku_list/daburu_riichi.py
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      463 2023-08-08 00:48:36.000000 mahjong-1.2.1/mahjong/hand_calculating/yaku_list/dora.py
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      818 2023-08-08 00:48:36.000000 mahjong-1.2.1/mahjong/hand_calculating/yaku_list/east.py
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      499 2023-08-08 00:48:36.000000 mahjong-1.2.1/mahjong/hand_calculating/yaku_list/haitei.py
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      577 2023-08-08 00:48:36.000000 mahjong-1.2.1/mahjong/hand_calculating/yaku_list/haku.py
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      582 2023-08-08 00:48:36.000000 mahjong-1.2.1/mahjong/hand_calculating/yaku_list/hatsu.py
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)     1083 2023-08-08 00:48:36.000000 mahjong-1.2.1/mahjong/hand_calculating/yaku_list/honitsu.py
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      679 2023-08-08 00:48:36.000000 mahjong-1.2.1/mahjong/hand_calculating/yaku_list/honroto.py
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      499 2023-08-08 00:48:36.000000 mahjong-1.2.1/mahjong/hand_calculating/yaku_list/houtei.py
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      825 2023-08-08 00:48:36.000000 mahjong-1.2.1/mahjong/hand_calculating/yaku_list/iipeiko.py
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      498 2023-08-08 00:48:36.000000 mahjong-1.2.1/mahjong/hand_calculating/yaku_list/ippatsu.py
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)     1438 2023-08-08 00:48:36.000000 mahjong-1.2.1/mahjong/hand_calculating/yaku_list/ittsu.py
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)     1150 2023-08-08 00:48:36.000000 mahjong-1.2.1/mahjong/hand_calculating/yaku_list/junchan.py
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      486 2023-08-08 00:48:36.000000 mahjong-1.2.1/mahjong/hand_calculating/yaku_list/nagashi_mangan.py
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      825 2023-08-08 00:48:36.000000 mahjong-1.2.1/mahjong/hand_calculating/yaku_list/north.py
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      378 2023-08-08 00:48:36.000000 mahjong-1.2.1/mahjong/hand_calculating/yaku_list/open_riichi.py
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      431 2023-08-08 00:48:36.000000 mahjong-1.2.1/mahjong/hand_calculating/yaku_list/pinfu.py
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      496 2023-08-08 00:48:36.000000 mahjong-1.2.1/mahjong/hand_calculating/yaku_list/renhou.py
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      398 2023-08-08 00:48:36.000000 mahjong-1.2.1/mahjong/hand_calculating/yaku_list/riichi.py
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      502 2023-08-08 00:48:36.000000 mahjong-1.2.1/mahjong/hand_calculating/yaku_list/rinshan.py
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      835 2023-08-08 00:48:36.000000 mahjong-1.2.1/mahjong/hand_calculating/yaku_list/ryanpeiko.py
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)     1455 2023-08-08 00:48:36.000000 mahjong-1.2.1/mahjong/hand_calculating/yaku_list/sanankou.py
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      596 2023-08-08 00:48:36.000000 mahjong-1.2.1/mahjong/hand_calculating/yaku_list/sankantsu.py
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)     1393 2023-08-08 00:48:36.000000 mahjong-1.2.1/mahjong/hand_calculating/yaku_list/sanshoku.py
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)     1471 2023-08-08 00:48:36.000000 mahjong-1.2.1/mahjong/hand_calculating/yaku_list/sanshoku_douko.py
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      844 2023-08-08 00:48:36.000000 mahjong-1.2.1/mahjong/hand_calculating/yaku_list/shosangen.py
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      825 2023-08-08 00:48:36.000000 mahjong-1.2.1/mahjong/hand_calculating/yaku_list/south.py
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      679 2023-08-08 00:48:36.000000 mahjong-1.2.1/mahjong/hand_calculating/yaku_list/tanyao.py
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      607 2023-08-08 00:48:36.000000 mahjong-1.2.1/mahjong/hand_calculating/yaku_list/toitoi.py
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      498 2023-08-08 00:48:36.000000 mahjong-1.2.1/mahjong/hand_calculating/yaku_list/tsumo.py
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      818 2023-08-08 00:48:36.000000 mahjong-1.2.1/mahjong/hand_calculating/yaku_list/west.py
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      429 2023-08-08 00:48:36.000000 mahjong-1.2.1/mahjong/hand_calculating/yaku_list/yakuhai_place.py
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      429 2023-08-08 00:48:36.000000 mahjong-1.2.1/mahjong/hand_calculating/yaku_list/yakuhai_round.py
+drwxrwxr-x   0 nihisil   (1000) nihisil   (1000)        0 2023-08-08 02:15:33.304046 mahjong-1.2.1/mahjong/hand_calculating/yaku_list/yakuman/
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)     1553 2023-08-08 00:48:36.000000 mahjong-1.2.1/mahjong/hand_calculating/yaku_list/yakuman/__init__.py
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      315 2023-08-08 00:48:36.000000 mahjong-1.2.1/mahjong/hand_calculating/yaku_list/yakuman/chiihou.py
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      716 2023-08-08 00:48:36.000000 mahjong-1.2.1/mahjong/hand_calculating/yaku_list/yakuman/chinroto.py
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)     1811 2023-08-08 00:48:36.000000 mahjong-1.2.1/mahjong/hand_calculating/yaku_list/yakuman/chuuren_poutou.py
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      501 2023-08-08 00:48:36.000000 mahjong-1.2.1/mahjong/hand_calculating/yaku_list/yakuman/daburu_chuuren_poutou.py
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      508 2023-08-08 00:48:36.000000 mahjong-1.2.1/mahjong/hand_calculating/yaku_list/yakuman/daburu_kokushi.py
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      590 2023-08-08 00:48:36.000000 mahjong-1.2.1/mahjong/hand_calculating/yaku_list/yakuman/daichisei.py
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      760 2023-08-08 00:48:36.000000 mahjong-1.2.1/mahjong/hand_calculating/yaku_list/yakuman/daisangen.py
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)     1994 2023-08-08 00:48:36.000000 mahjong-1.2.1/mahjong/hand_calculating/yaku_list/yakuman/daisharin.py
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)     1024 2023-08-08 00:48:36.000000 mahjong-1.2.1/mahjong/hand_calculating/yaku_list/yakuman/daisuushi.py
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      963 2023-08-08 00:48:36.000000 mahjong-1.2.1/mahjong/hand_calculating/yaku_list/yakuman/kokushi.py
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      741 2023-08-08 00:48:36.000000 mahjong-1.2.1/mahjong/hand_calculating/yaku_list/yakuman/paarenchan.py
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      491 2023-08-08 00:48:36.000000 mahjong-1.2.1/mahjong/hand_calculating/yaku_list/yakuman/renhou_yakuman.py
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      731 2023-08-08 00:48:36.000000 mahjong-1.2.1/mahjong/hand_calculating/yaku_list/yakuman/ryuisou.py
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      471 2023-08-08 00:48:36.000000 mahjong-1.2.1/mahjong/hand_calculating/yaku_list/yakuman/sashikomi.py
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)     1062 2023-08-08 00:48:36.000000 mahjong-1.2.1/mahjong/hand_calculating/yaku_list/yakuman/shosuushi.py
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      879 2023-08-08 00:48:36.000000 mahjong-1.2.1/mahjong/hand_calculating/yaku_list/yakuman/suuankou.py
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      422 2023-08-08 00:48:36.000000 mahjong-1.2.1/mahjong/hand_calculating/yaku_list/yakuman/suuankou_tanki.py
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      596 2023-08-08 00:48:36.000000 mahjong-1.2.1/mahjong/hand_calculating/yaku_list/yakuman/suukantsu.py
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      496 2023-08-08 00:48:36.000000 mahjong-1.2.1/mahjong/hand_calculating/yaku_list/yakuman/tenhou.py
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      766 2023-08-08 00:48:36.000000 mahjong-1.2.1/mahjong/hand_calculating/yaku_list/yakuman/tsuisou.py
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)     1115 2023-08-08 00:48:36.000000 mahjong-1.2.1/mahjong/meld.py
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)    11195 2023-08-08 00:48:36.000000 mahjong-1.2.1/mahjong/shanten.py
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)     3833 2023-08-08 00:48:36.000000 mahjong-1.2.1/mahjong/tests_mixin.py
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)     6904 2023-08-08 00:48:36.000000 mahjong-1.2.1/mahjong/tile.py
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)     6110 2023-08-08 00:48:36.000000 mahjong-1.2.1/mahjong/utils.py
+drwxrwxr-x   0 nihisil   (1000) nihisil   (1000)        0 2023-08-08 02:15:33.300045 mahjong-1.2.1/mahjong.egg-info/
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)     1578 2023-08-08 02:15:33.000000 mahjong-1.2.1/mahjong.egg-info/PKG-INFO
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)     3764 2023-08-08 02:15:33.000000 mahjong-1.2.1/mahjong.egg-info/SOURCES.txt
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)        1 2023-08-08 02:15:33.000000 mahjong-1.2.1/mahjong.egg-info/dependency_links.txt
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)        8 2023-08-08 02:15:33.000000 mahjong-1.2.1/mahjong.egg-info/top_level.txt
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)      389 2023-08-08 00:48:36.000000 mahjong-1.2.1/pyproject.toml
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)       79 2023-08-08 02:15:33.304046 mahjong-1.2.1/setup.cfg
+-rw-rw-r--   0 nihisil   (1000) nihisil   (1000)     1229 2023-08-08 02:09:54.000000 mahjong-1.2.1/setup.py
```

### Comparing `mahjong-1.2.0.dev7/LICENSE.txt` & `mahjong-1.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mahjong-1.2.0.dev7/PKG-INFO` & `mahjong-1.2.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,41 @@
 Metadata-Version: 2.1
 Name: mahjong
-Version: 1.2.0.dev7
+Version: 1.2.1
 Summary: Mahjong hands calculation
 Home-page: https://github.com/MahjongRepository/mahjong
 Author: Alexey Lisikhin
 Author-email: alexey@nihisil.com
 License: MIT
-Description: This library can calculate hand cost (han, fu with details, yaku, and scores) for riichi mahjong (Japanese version).
-        
-        Also calculating of shanten is supported.
-        
-        The code was validated on tenhou.net phoenix replays in total on **11,120,125 hands**.
-        
-        So, we can say that our hand calculator works the same way that tenhou.net hand calculation.
-        
-        # How to install
-        
-        ```bash
-        pip install mahjong
-        ```
-        
-        # Supported rules and usage examples
-        
-        You can find usage examples and information about all supported rules variations in the [wiki](https://github.com/MahjongRepository/mahjong/wiki)
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+[![Mahjong lib](https://github.com/MahjongRepository/mahjong/actions/workflows/lint_and_test.yml/badge.svg)](https://github.com/MahjongRepository/mahjong/actions/workflows/lint_and_test.yml)
+
+This library can calculate hand cost (han, fu with details, yaku, and scores) for riichi mahjong (Japanese version).
+
+Also calculating of shanten is supported.
+
+The code was validated on tenhou.net phoenix replays in total on **11,120,125 hands**.
+
+So, we can say that our hand calculator works the same way that tenhou.net hand calculation.
+
+# How to install
+
+```bash
+pip install mahjong
+```
+
+# Supported rules and usage examples
+
+You can find usage examples and information about all supported rules variations in the [wiki](https://github.com/MahjongRepository/mahjong/wiki)
```

### Comparing `mahjong-1.2.0.dev7/mahjong/agari.py` & `mahjong-1.2.1/mahjong/agari.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-# -*- coding: utf-8 -*-
 from mahjong.utils import find_isolated_tile_indices
 
 
-class Agari(object):
+class Agari:
     def is_agari(self, tiles_34, open_sets_34=None):
         """
         Determine was it win or not
         :param tiles_34: 34 tiles format array
         :param open_sets_34: array of array of 34 tiles format
         :return: boolean
         """
```

### Comparing `mahjong-1.2.0.dev7/mahjong/hand_calculating/divider.py` & `mahjong-1.2.1/mahjong/hand_calculating/divider.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 import hashlib
 import itertools
 import marshal
 from functools import reduce
 from typing import List
 
 from mahjong.constants import HONOR_INDICES
```

### Comparing `mahjong-1.2.0.dev7/mahjong/hand_calculating/fu.py` & `mahjong-1.2.1/mahjong/hand_calculating/fu.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,13 @@
-# -*- coding: utf-8 -*-
-
 from mahjong.constants import HONOR_INDICES, TERMINAL_INDICES
 from mahjong.meld import Meld
 from mahjong.utils import contains_terminals, is_pair, is_pon_or_kan, simplify
 
 
-class FuCalculator(object):
+class FuCalculator:
     BASE = "base"
     PENCHAN = "penchan"
     KANCHAN = "kanchan"
     VALUED_PAIR = "valued_pair"
     DOUBLE_VALUED_PAIR = "double_valued_pair"
     PAIR_WAIT = "pair_wait"
     TSUMO = "tsumo"
```

### Comparing `mahjong-1.2.0.dev7/mahjong/hand_calculating/hand.py` & `mahjong-1.2.1/mahjong/hand_calculating/hand.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 from mahjong.agari import Agari
 from mahjong.constants import CHUN, EAST, HAKU, HATSU, NORTH, SOUTH, WEST
 from mahjong.hand_calculating.divider import HandDivider
 from mahjong.hand_calculating.fu import FuCalculator
 from mahjong.hand_calculating.hand_config import HandConfig
 from mahjong.hand_calculating.hand_response import HandResponse
 from mahjong.hand_calculating.scores import Aotenjou, ScoresCalculator
```

### Comparing `mahjong-1.2.0.dev7/mahjong/hand_calculating/hand_config.py` & `mahjong-1.2.1/mahjong/hand_calculating/hand_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-# -*- coding: utf-8 -*-
 from mahjong.constants import EAST
 from mahjong.hand_calculating.yaku_config import YakuConfig
 
 
-class HandConstants(object):
+class HandConstants:
     # Hands over 26+ han don't count as double yakuman
     KAZOE_LIMITED = 0
     # Hands over 13+ is a sanbaiman
     KAZOE_SANBAIMAN = 1
     # 26+ han as double yakuman, 39+ han as triple yakuman, etc.
     KAZOE_NO_LIMIT = 2
 
 
-class OptionalRules(object):
+class OptionalRules:
     """
     All the supported optional rules
     """
 
     has_open_tanyao = False
     has_aka_dora = False
     has_double_yakuman = True
```

### Comparing `mahjong-1.2.0.dev7/mahjong/hand_calculating/hand_response.py` & `mahjong-1.2.1/mahjong/hand_calculating/hand_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,8 @@
-# -*- coding: utf-8 -*-
-
-
-class HandResponse(object):
+class HandResponse:
     cost = None
     han = None
     fu = None
     fu_details = None
     yaku = None
     error = None
     is_open_hand = False
```

### Comparing `mahjong-1.2.0.dev7/mahjong/hand_calculating/scores.py` & `mahjong-1.2.1/mahjong/hand_calculating/scores.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-# -*- coding: utf-8 -*-
 from mahjong.hand_calculating.hand_config import HandConfig
 
 
-class ScoresCalculator(object):
+class ScoresCalculator:
     def calculate_scores(self, han, fu, config, is_yakuman=False):
         """
         Calculate how much scores cost a hand with given han and fu
         :param han: int
         :param fu: int
         :param config: HandConfig object
         :param is_yakuman: boolean
```

### Comparing `mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku.py` & `mahjong-1.2.1/mahjong/hand_calculating/yaku.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-# -*- coding: utf-8 -*-
 import warnings
 
 
-class Yaku(object):
+class Yaku:
     yaku_id = None
     tenhou_id = None
     name = None
     han_open = None
     han_closed = None
     is_yakuman = None
 
@@ -36,14 +35,14 @@
         """
         Set id, name, han related to the yaku
         """
         raise NotImplementedError
 
     @property
     def english(self):
-        warnings.warn("Use .name attribute instead of .english attribute", DeprecationWarning)
+        warnings.warn("Use .name attribute instead of .english attribute", DeprecationWarning, stacklevel=2)
         return self.name
 
     @property
     def japanese(self):
-        warnings.warn("Use .name attribute instead of .japanese attribute", DeprecationWarning)
+        warnings.warn("Use .name attribute instead of .japanese attribute", DeprecationWarning, stacklevel=2)
         return self.name
```

### Comparing `mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_config.py` & `mahjong-1.2.1/mahjong/hand_calculating/yaku_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 from itertools import count
 
 from mahjong.hand_calculating.yaku_list import (
     AkaDora,
     Chankan,
     Chantai,
     Chiitoitsu,
@@ -63,15 +62,15 @@
     SuuankouTanki,
     Suukantsu,
     Tenhou,
     Tsuuiisou,
 )
 
 
-class YakuConfig(object):
+class YakuConfig:
     def __init__(self):
         id = count(0)
 
         # Yaku situations
         self.tsumo = Tsumo(next(id))
         self.riichi = Riichi(next(id))
         self.open_riichi = OpenRiichi(next(id))
```

### Comparing `mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/__init__.py` & `mahjong-1.2.1/mahjong/hand_calculating/yaku_list/__init__.py`

 * *Files identical despite different names*

### Comparing `mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/aka_dora.py` & `mahjong-1.2.1/mahjong/hand_calculating/yaku_list/chun.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,25 @@
-# -*- coding: utf-8 -*-
+from mahjong.constants import CHUN
 from mahjong.hand_calculating.yaku import Yaku
+from mahjong.utils import is_pon_or_kan
 
 
-class AkaDora(Yaku):
+class Chun(Yaku):
     """
-    Red five
+    Pon of red dragons
     """
 
     def __init__(self, yaku_id=None):
-        super(AkaDora, self).__init__(yaku_id)
+        super(Chun, self).__init__(yaku_id)
 
     def set_attributes(self):
-        self.tenhou_id = 54
+        self.tenhou_id = 20
 
-        self.name = "Aka Dora"
+        self.name = "Yakuhai (chun)"
 
         self.han_open = 1
         self.han_closed = 1
 
         self.is_yakuman = False
 
     def is_condition_met(self, hand, *args):
-        return True
-
-    def __str__(self):
-        return "Aka Dora {}".format(self.han_closed)
+        return len([x for x in hand if is_pon_or_kan(x) and x[0] == CHUN]) == 1
```

### Comparing `mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/chankan.py` & `mahjong-1.2.1/mahjong/hand_calculating/yaku_list/daburu_riichi.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,24 @@
-# -*- coding: utf-8 -*-
 from mahjong.hand_calculating.yaku import Yaku
 
 
-class Chankan(Yaku):
+class DaburuRiichi(Yaku):
     """
     Yaku situation
     """
 
     def __init__(self, yaku_id=None):
-        super(Chankan, self).__init__(yaku_id)
+        super(DaburuRiichi, self).__init__(yaku_id)
 
     def set_attributes(self):
-        self.tenhou_id = 3
+        self.tenhou_id = 21
 
-        self.name = "Chankan"
+        self.name = "Double Riichi"
 
-        self.han_open = 1
-        self.han_closed = 1
+        self.han_open = None
+        self.han_closed = 2
 
         self.is_yakuman = False
 
     def is_condition_met(self, hand, *args):
         # was it here or not is controlling by superior code
         return True
```

### Comparing `mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/chantai.py` & `mahjong-1.2.1/mahjong/hand_calculating/yaku_list/chantai.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 from mahjong.constants import HONOR_INDICES, TERMINAL_INDICES
 from mahjong.hand_calculating.yaku import Yaku
 from mahjong.utils import is_chi
 
 
 class Chantai(Yaku):
     """
```

### Comparing `mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/chinitsu.py` & `mahjong-1.2.1/mahjong/hand_calculating/yaku_list/chinitsu.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 from mahjong.constants import HONOR_INDICES
 from mahjong.hand_calculating.yaku import Yaku
 from mahjong.utils import is_man, is_pin, is_sou
 
 
 class Chinitsu(Yaku):
     """
```

### Comparing `mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/chun.py` & `mahjong-1.2.1/mahjong/hand_calculating/yaku_list/haku.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,25 @@
-# -*- coding: utf-8 -*-
-from mahjong.constants import CHUN
+from mahjong.constants import HAKU
 from mahjong.hand_calculating.yaku import Yaku
 from mahjong.utils import is_pon_or_kan
 
 
-class Chun(Yaku):
+class Haku(Yaku):
     """
-    Pon of red dragons
+    Pon of white dragons
     """
 
     def __init__(self, yaku_id=None):
-        super(Chun, self).__init__(yaku_id)
+        super(Haku, self).__init__(yaku_id)
 
     def set_attributes(self):
-        self.tenhou_id = 20
+        self.tenhou_id = 18
 
-        self.name = "Yakuhai (chun)"
+        self.name = "Yakuhai (haku)"
 
         self.han_open = 1
         self.han_closed = 1
 
         self.is_yakuman = False
 
     def is_condition_met(self, hand, *args):
-        return len([x for x in hand if is_pon_or_kan(x) and x[0] == CHUN]) == 1
+        return len([x for x in hand if is_pon_or_kan(x) and x[0] == HAKU]) == 1
```

### Comparing `mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/daburu_riichi.py` & `mahjong-1.2.1/mahjong/hand_calculating/yaku_list/hatsu.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-# -*- coding: utf-8 -*-
+from mahjong.constants import HATSU
 from mahjong.hand_calculating.yaku import Yaku
+from mahjong.utils import is_pon_or_kan
 
 
-class DaburuRiichi(Yaku):
+class Hatsu(Yaku):
     """
-    Yaku situation
+    Pon of green dragons
     """
 
     def __init__(self, yaku_id=None):
-        super(DaburuRiichi, self).__init__(yaku_id)
+        super(Hatsu, self).__init__(yaku_id)
 
     def set_attributes(self):
-        self.tenhou_id = 21
+        self.tenhou_id = 19
 
-        self.name = "Double Riichi"
+        self.name = "Yakuhai (hatsu)"
 
-        self.han_open = None
-        self.han_closed = 2
+        self.han_open = 1
+        self.han_closed = 1
 
         self.is_yakuman = False
 
     def is_condition_met(self, hand, *args):
-        # was it here or not is controlling by superior code
-        return True
+        return len([x for x in hand if is_pon_or_kan(x) and x[0] == HATSU]) == 1
```

### Comparing `mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/east.py` & `mahjong-1.2.1/mahjong/hand_calculating/yaku_list/north.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,31 @@
-# -*- coding: utf-8 -*-
-from mahjong.constants import EAST
+from mahjong.constants import NORTH
 from mahjong.hand_calculating.yaku import Yaku
 from mahjong.utils import is_pon_or_kan
 
 
-class YakuhaiEast(Yaku):
+class YakuhaiNorth(Yaku):
     """
-    Pon of east winds
+    Pon of north winds
     """
 
     def __init__(self, yaku_id=None):
-        super(YakuhaiEast, self).__init__(yaku_id)
+        super(YakuhaiNorth, self).__init__(yaku_id)
 
     def set_attributes(self):
         self.tenhou_id = 10
 
-        self.name = "Yakuhai (east)"
+        self.name = "Yakuhai (north)"
 
         self.han_open = 1
         self.han_closed = 1
 
         self.is_yakuman = False
 
     def is_condition_met(self, hand, player_wind, round_wind, *args):
-        if len([x for x in hand if is_pon_or_kan(x) and x[0] == player_wind]) == 1 and player_wind == EAST:
+        if len([x for x in hand if is_pon_or_kan(x) and x[0] == player_wind]) == 1 and player_wind == NORTH:
             return True
 
-        if len([x for x in hand if is_pon_or_kan(x) and x[0] == round_wind]) == 1 and round_wind == EAST:
+        if len([x for x in hand if is_pon_or_kan(x) and x[0] == round_wind]) == 1 and round_wind == NORTH:
             return True
 
         return False
```

### Comparing `mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/haitei.py` & `mahjong-1.2.1/mahjong/hand_calculating/yaku_list/yakuman/paarenchan.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,33 @@
-# -*- coding: utf-8 -*-
 from mahjong.hand_calculating.yaku import Yaku
 
 
-class Haitei(Yaku):
+class Paarenchan(Yaku):
     """
     Yaku situation
     """
 
-    def __init__(self, yaku_id=None):
-        super(Haitei, self).__init__(yaku_id)
+    def __init__(self, yaku_id):
+        super(Paarenchan, self).__init__(yaku_id)
 
     def set_attributes(self):
-        self.tenhou_id = 5
+        self.tenhou_id = 37
 
-        self.name = "Haitei Raoyue"
+        self.name = "Paarenchan"
 
-        self.han_open = 1
-        self.han_closed = 1
+        self.han_open = 13
+        self.han_closed = 13
+        self.count = 0
 
-        self.is_yakuman = False
+        self.is_yakuman = True
+
+    def set_paarenchan_count(self, count):
+        self.han_open = 13 * count
+        self.han_closed = 13 * count
+        self.count = count
 
     def is_condition_met(self, hand, *args):
         # was it here or not is controlling by superior code
         return True
+
+    def __str__(self):
+        return "Paarenchan {}".format(self.count)
```

### Comparing `mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/haku.py` & `mahjong-1.2.1/mahjong/hand_calculating/yaku_list/toitoi.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,24 @@
-# -*- coding: utf-8 -*-
-from mahjong.constants import HAKU
 from mahjong.hand_calculating.yaku import Yaku
 from mahjong.utils import is_pon_or_kan
 
 
-class Haku(Yaku):
+class Toitoi(Yaku):
     """
-    Pon of white dragons
+    The hand consists of all pon sets (and of course a pair), no sequences.
     """
 
     def __init__(self, yaku_id=None):
-        super(Haku, self).__init__(yaku_id)
+        super(Toitoi, self).__init__(yaku_id)
 
     def set_attributes(self):
-        self.tenhou_id = 18
+        self.tenhou_id = 28
+        self.name = "Toitoi"
 
-        self.name = "Yakuhai (haku)"
-
-        self.han_open = 1
-        self.han_closed = 1
+        self.han_open = 2
+        self.han_closed = 2
 
         self.is_yakuman = False
 
     def is_condition_met(self, hand, *args):
-        return len([x for x in hand if is_pon_or_kan(x) and x[0] == HAKU]) == 1
+        count_of_pon = len([i for i in hand if is_pon_or_kan(i)])
+        return count_of_pon == 4
```

### Comparing `mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/hatsu.py` & `mahjong-1.2.1/mahjong/hand_calculating/yaku_list/yakuman/daichisei.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,25 @@
-# -*- coding: utf-8 -*-
-from mahjong.constants import HATSU
+from functools import reduce
+
+from mahjong.constants import HONOR_INDICES
 from mahjong.hand_calculating.yaku import Yaku
-from mahjong.utils import is_pon_or_kan
 
 
-class Hatsu(Yaku):
+class Daichisei(Yaku):
     """
-    Pon of green dragons
+    Yaku situation
     """
 
-    def __init__(self, yaku_id=None):
-        super(Hatsu, self).__init__(yaku_id)
+    def __init__(self, yaku_id):
+        super(Daichisei, self).__init__(yaku_id)
 
     def set_attributes(self):
-        self.tenhou_id = 19
-
-        self.name = "Yakuhai (hatsu)"
+        self.name = "Daichisei"
 
-        self.han_open = 1
-        self.han_closed = 1
+        self.han_open = None
+        self.han_closed = 13
 
-        self.is_yakuman = False
+        self.is_yakuman = True
 
     def is_condition_met(self, hand, *args):
-        return len([x for x in hand if is_pon_or_kan(x) and x[0] == HATSU]) == 1
+        indices = reduce(lambda z, y: z + y, hand)
+        return all(x in HONOR_INDICES for x in indices) and len(hand) == 7
```

### Comparing `mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/honitsu.py` & `mahjong-1.2.1/mahjong/hand_calculating/yaku_list/honitsu.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 from mahjong.constants import HONOR_INDICES
 from mahjong.hand_calculating.yaku import Yaku
 from mahjong.utils import is_man, is_pin, is_sou
 
 
 class Honitsu(Yaku):
     """
```

### Comparing `mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/honroto.py` & `mahjong-1.2.1/mahjong/hand_calculating/yaku_list/yakuman/ryuisou.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,29 +1,28 @@
-# -*- coding: utf-8 -*-
 from functools import reduce
 
-from mahjong.constants import HONOR_INDICES, TERMINAL_INDICES
+from mahjong.constants import HATSU
 from mahjong.hand_calculating.yaku import Yaku
 
 
-class Honroto(Yaku):
+class Ryuuiisou(Yaku):
     """
-    All tiles are terminals or honours
+    Hand composed entirely of green tiles. Green tiles are: green dragons and 2, 3, 4, 6 and 8 of sou.
     """
 
     def __init__(self, yaku_id=None):
-        super(Honroto, self).__init__(yaku_id)
+        super(Ryuuiisou, self).__init__(yaku_id)
 
     def set_attributes(self):
-        self.tenhou_id = 31
+        self.tenhou_id = 43
 
-        self.name = "Honroutou"
+        self.name = "Ryuuiisou"
 
-        self.han_open = 2
-        self.han_closed = 2
+        self.han_open = 13
+        self.han_closed = 13
 
-        self.is_yakuman = False
+        self.is_yakuman = True
 
     def is_condition_met(self, hand, *args):
+        green_indices = [19, 20, 21, 23, 25, HATSU]
         indices = reduce(lambda z, y: z + y, hand)
-        result = HONOR_INDICES + TERMINAL_INDICES
-        return all(x in result for x in indices)
+        return all(x in green_indices for x in indices)
```

### Comparing `mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/houtei.py` & `mahjong-1.2.1/mahjong/hand_calculating/yaku_list/sankantsu.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-# -*- coding: utf-8 -*-
 from mahjong.hand_calculating.yaku import Yaku
+from mahjong.meld import Meld
 
 
-class Houtei(Yaku):
+class SanKantsu(Yaku):
     """
-    Yaku situation
+    The hand with three kan sets
     """
 
     def __init__(self, yaku_id=None):
-        super(Houtei, self).__init__(yaku_id)
+        super(SanKantsu, self).__init__(yaku_id)
 
     def set_attributes(self):
-        self.tenhou_id = 6
+        self.tenhou_id = 27
 
-        self.name = "Houtei Raoyui"
+        self.name = "San Kantsu"
 
-        self.han_open = 1
-        self.han_closed = 1
+        self.han_open = 2
+        self.han_closed = 2
 
         self.is_yakuman = False
 
-    def is_condition_met(self, hand, *args):
-        # was it here or not is controlling by superior code
-        return True
+    def is_condition_met(self, hand, melds, *args):
+        kan_sets = [x for x in melds if x.type == Meld.KAN or x.type == Meld.SHOUMINKAN]
+        return len(kan_sets) == 3
```

### Comparing `mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/iipeiko.py` & `mahjong-1.2.1/mahjong/hand_calculating/yaku_list/iipeiko.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 from mahjong.hand_calculating.yaku import Yaku
 from mahjong.utils import is_chi
 
 
 class Iipeiko(Yaku):
     """
     Hand with two identical chi
```

### Comparing `mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/ippatsu.py` & `mahjong-1.2.1/mahjong/hand_calculating/yaku_list/ryanpeiko.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,33 @@
-# -*- coding: utf-8 -*-
 from mahjong.hand_calculating.yaku import Yaku
+from mahjong.utils import is_chi
 
 
-class Ippatsu(Yaku):
+class Ryanpeikou(Yaku):
     """
-    Yaku situation
+    The hand contains two different Iipeikou’s
     """
 
     def __init__(self, yaku_id=None):
-        super(Ippatsu, self).__init__(yaku_id)
+        super(Ryanpeikou, self).__init__(yaku_id)
 
     def set_attributes(self):
-        self.tenhou_id = 2
+        self.tenhou_id = 32
 
-        self.name = "Ippatsu"
+        self.name = "Ryanpeikou"
 
         self.han_open = None
-        self.han_closed = 1
+        self.han_closed = 3
 
         self.is_yakuman = False
 
     def is_condition_met(self, hand, *args):
-        # was it here or not is controlling by superior code
-        return True
+        chi_sets = [i for i in hand if is_chi(i)]
+        count_of_identical_chi = []
+        for x in chi_sets:
+            count = 0
+            for y in chi_sets:
+                if x == y:
+                    count += 1
+            count_of_identical_chi.append(count)
+
+        return len([x for x in count_of_identical_chi if x >= 2]) == 4
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/ittsu.py` & `mahjong-1.2.1/mahjong/hand_calculating/yaku_list/ittsu.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 from mahjong.hand_calculating.yaku import Yaku
 from mahjong.utils import is_chi, is_man, is_pin, is_sou, simplify
 
 
 class Ittsu(Yaku):
     """
     Three sets of same suit: 1-2-3, 4-5-6, 7-8-9
```

### Comparing `mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/junchan.py` & `mahjong-1.2.1/mahjong/hand_calculating/yaku_list/junchan.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 from mahjong.constants import TERMINAL_INDICES
 from mahjong.hand_calculating.yaku import Yaku
 from mahjong.utils import is_chi
 
 
 class Junchan(Yaku):
     """
```

### Comparing `mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/north.py` & `mahjong-1.2.1/mahjong/hand_calculating/yaku_list/south.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,31 @@
-# -*- coding: utf-8 -*-
-from mahjong.constants import NORTH
+from mahjong.constants import SOUTH
 from mahjong.hand_calculating.yaku import Yaku
 from mahjong.utils import is_pon_or_kan
 
 
-class YakuhaiNorth(Yaku):
+class YakuhaiSouth(Yaku):
     """
-    Pon of north winds
+    Pon of south winds
     """
 
     def __init__(self, yaku_id=None):
-        super(YakuhaiNorth, self).__init__(yaku_id)
+        super(YakuhaiSouth, self).__init__(yaku_id)
 
     def set_attributes(self):
         self.tenhou_id = 10
 
-        self.name = "Yakuhai (north)"
+        self.name = "Yakuhai (south)"
 
         self.han_open = 1
         self.han_closed = 1
 
         self.is_yakuman = False
 
     def is_condition_met(self, hand, player_wind, round_wind, *args):
-        if len([x for x in hand if is_pon_or_kan(x) and x[0] == player_wind]) == 1 and player_wind == NORTH:
+        if len([x for x in hand if is_pon_or_kan(x) and x[0] == player_wind]) == 1 and player_wind == SOUTH:
             return True
 
-        if len([x for x in hand if is_pon_or_kan(x) and x[0] == round_wind]) == 1 and round_wind == NORTH:
+        if len([x for x in hand if is_pon_or_kan(x) and x[0] == round_wind]) == 1 and round_wind == SOUTH:
             return True
 
         return False
```

### Comparing `mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/ryanpeiko.py` & `mahjong-1.2.1/mahjong/hand_calculating/yaku_list/yakuman/suuankou.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-# -*- coding: utf-8 -*-
 from mahjong.hand_calculating.yaku import Yaku
-from mahjong.utils import is_chi
+from mahjong.utils import is_pon_or_kan
 
 
-class Ryanpeikou(Yaku):
+class Suuankou(Yaku):
     """
-    The hand contains two different Iipeikou’s
+    Four closed pon sets
     """
 
     def __init__(self, yaku_id=None):
-        super(Ryanpeikou, self).__init__(yaku_id)
+        super(Suuankou, self).__init__(yaku_id)
 
     def set_attributes(self):
-        self.tenhou_id = 32
+        self.tenhou_id = 41
 
-        self.name = "Ryanpeikou"
+        self.name = "Suu Ankou"
 
         self.han_open = None
-        self.han_closed = 3
+        self.han_closed = 13
 
-        self.is_yakuman = False
+        self.is_yakuman = True
 
-    def is_condition_met(self, hand, *args):
-        chi_sets = [i for i in hand if is_chi(i)]
-        count_of_identical_chi = []
-        for x in chi_sets:
-            count = 0
-            for y in chi_sets:
-                if x == y:
-                    count += 1
-            count_of_identical_chi.append(count)
+    def is_condition_met(self, hand, win_tile, is_tsumo):
+        win_tile //= 4
+        closed_hand = []
+        for item in hand:
+            # if we do the ron on syanpon wait our pon will be consider as open
+            if is_pon_or_kan(item) and win_tile in item and not is_tsumo:
+                continue
 
-        return len([x for x in count_of_identical_chi if x >= 2]) == 4
+            closed_hand.append(item)
+
+        count_of_pon = len([i for i in closed_hand if is_pon_or_kan(i)])
+        return count_of_pon == 4
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/sanankou.py` & `mahjong-1.2.1/mahjong/hand_calculating/yaku_list/sanankou.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 from mahjong.hand_calculating.yaku import Yaku
 from mahjong.utils import is_chi, is_pon_or_kan
 
 
 class Sanankou(Yaku):
     """
     Three closed pon sets, the other sets need not to be closed
```

### Comparing `mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/sankantsu.py` & `mahjong-1.2.1/mahjong/hand_calculating/yaku_list/yakuman/suukantsu.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,25 @@
-# -*- coding: utf-8 -*-
 from mahjong.hand_calculating.yaku import Yaku
 from mahjong.meld import Meld
 
 
-class SanKantsu(Yaku):
+class Suukantsu(Yaku):
     """
-    The hand with three kan sets
+    The hand with four kan sets
     """
 
     def __init__(self, yaku_id=None):
-        super(SanKantsu, self).__init__(yaku_id)
+        super(Suukantsu, self).__init__(yaku_id)
 
     def set_attributes(self):
-        self.tenhou_id = 27
+        self.tenhou_id = 51
 
-        self.name = "San Kantsu"
+        self.name = "Suu Kantsu"
 
-        self.han_open = 2
-        self.han_closed = 2
+        self.han_open = 13
+        self.han_closed = 13
 
-        self.is_yakuman = False
+        self.is_yakuman = True
 
     def is_condition_met(self, hand, melds, *args):
         kan_sets = [x for x in melds if x.type == Meld.KAN or x.type == Meld.SHOUMINKAN]
-        return len(kan_sets) == 3
+        return len(kan_sets) == 4
```

### Comparing `mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/sanshoku.py` & `mahjong-1.2.1/mahjong/hand_calculating/yaku_list/sanshoku.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 from mahjong.hand_calculating.yaku import Yaku
 from mahjong.utils import is_chi, is_man, is_pin, is_sou, simplify
 
 
 class Sanshoku(Yaku):
     """
     The same chi in three suits
```

### Comparing `mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/sanshoku_douko.py` & `mahjong-1.2.1/mahjong/hand_calculating/yaku_list/sanshoku_douko.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 from mahjong.hand_calculating.yaku import Yaku
 from mahjong.utils import is_man, is_pin, is_pon_or_kan, is_sou, simplify
 
 
 class SanshokuDoukou(Yaku):
     """
     Three pon sets consisting of the same numbers in all three suits
```

### Comparing `mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/shosangen.py` & `mahjong-1.2.1/mahjong/hand_calculating/yaku_list/shosangen.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 from mahjong.constants import CHUN, HAKU, HATSU
 from mahjong.hand_calculating.yaku import Yaku
 from mahjong.utils import is_pair, is_pon_or_kan
 
 
 class Shosangen(Yaku):
     """
```

### Comparing `mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/south.py` & `mahjong-1.2.1/mahjong/hand_calculating/yaku_list/west.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,31 @@
-# -*- coding: utf-8 -*-
-from mahjong.constants import SOUTH
+from mahjong.constants import WEST
 from mahjong.hand_calculating.yaku import Yaku
 from mahjong.utils import is_pon_or_kan
 
 
-class YakuhaiSouth(Yaku):
+class YakuhaiWest(Yaku):
     """
-    Pon of south winds
+    Pon of west winds
     """
 
     def __init__(self, yaku_id=None):
-        super(YakuhaiSouth, self).__init__(yaku_id)
+        super(YakuhaiWest, self).__init__(yaku_id)
 
     def set_attributes(self):
         self.tenhou_id = 10
 
-        self.name = "Yakuhai (south)"
+        self.name = "Yakuhai (west)"
 
         self.han_open = 1
         self.han_closed = 1
 
         self.is_yakuman = False
 
     def is_condition_met(self, hand, player_wind, round_wind, *args):
-        if len([x for x in hand if is_pon_or_kan(x) and x[0] == player_wind]) == 1 and player_wind == SOUTH:
+        if len([x for x in hand if is_pon_or_kan(x) and x[0] == player_wind]) == 1 and player_wind == WEST:
             return True
 
-        if len([x for x in hand if is_pon_or_kan(x) and x[0] == round_wind]) == 1 and round_wind == SOUTH:
+        if len([x for x in hand if is_pon_or_kan(x) and x[0] == round_wind]) == 1 and round_wind == WEST:
             return True
 
         return False
```

### Comparing `mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/tanyao.py` & `mahjong-1.2.1/mahjong/hand_calculating/yaku_list/tanyao.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 from functools import reduce
 
 from mahjong.constants import HONOR_INDICES, TERMINAL_INDICES
 from mahjong.hand_calculating.yaku import Yaku
 
 
 class Tanyao(Yaku):
```

### Comparing `mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/west.py` & `mahjong-1.2.1/mahjong/hand_calculating/yaku_list/east.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,31 @@
-# -*- coding: utf-8 -*-
-from mahjong.constants import WEST
+from mahjong.constants import EAST
 from mahjong.hand_calculating.yaku import Yaku
 from mahjong.utils import is_pon_or_kan
 
 
-class YakuhaiWest(Yaku):
+class YakuhaiEast(Yaku):
     """
-    Pon of west winds
+    Pon of east winds
     """
 
     def __init__(self, yaku_id=None):
-        super(YakuhaiWest, self).__init__(yaku_id)
+        super(YakuhaiEast, self).__init__(yaku_id)
 
     def set_attributes(self):
         self.tenhou_id = 10
 
-        self.name = "Yakuhai (west)"
+        self.name = "Yakuhai (east)"
 
         self.han_open = 1
         self.han_closed = 1
 
         self.is_yakuman = False
 
     def is_condition_met(self, hand, player_wind, round_wind, *args):
-        if len([x for x in hand if is_pon_or_kan(x) and x[0] == player_wind]) == 1 and player_wind == WEST:
+        if len([x for x in hand if is_pon_or_kan(x) and x[0] == player_wind]) == 1 and player_wind == EAST:
             return True
 
-        if len([x for x in hand if is_pon_or_kan(x) and x[0] == round_wind]) == 1 and round_wind == WEST:
+        if len([x for x in hand if is_pon_or_kan(x) and x[0] == round_wind]) == 1 and round_wind == EAST:
             return True
 
         return False
```

### Comparing `mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/yakuman/__init__.py` & `mahjong-1.2.1/mahjong/hand_calculating/yaku_list/yakuman/__init__.py`

 * *Files identical despite different names*

### Comparing `mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/yakuman/chinroto.py` & `mahjong-1.2.1/mahjong/hand_calculating/yaku_list/yakuman/chinroto.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 from functools import reduce
 
 from mahjong.constants import TERMINAL_INDICES
 from mahjong.hand_calculating.yaku import Yaku
 
 
 class Chinroutou(Yaku):
```

### Comparing `mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/yakuman/chuuren_poutou.py` & `mahjong-1.2.1/mahjong/hand_calculating/yaku_list/yakuman/chuuren_poutou.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 from functools import reduce
 
 from mahjong.hand_calculating.yaku import Yaku
 from mahjong.utils import is_man, is_pin, is_sou, simplify
 
 
 class ChuurenPoutou(Yaku):
```

### Comparing `mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/yakuman/daisangen.py` & `mahjong-1.2.1/mahjong/hand_calculating/yaku_list/yakuman/daisangen.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 from mahjong.constants import CHUN, HAKU, HATSU
 from mahjong.hand_calculating.yaku import Yaku
 from mahjong.utils import is_pon_or_kan
 
 
 class Daisangen(Yaku):
     """
```

### Comparing `mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/yakuman/daisharin.py` & `mahjong-1.2.1/mahjong/hand_calculating/yaku_list/yakuman/daisharin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 from functools import reduce
 
 from mahjong.hand_calculating.yaku import Yaku
 from mahjong.utils import is_man, is_pin, is_sou, simplify
 
 
 class Daisharin(Yaku):
```

### Comparing `mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/yakuman/daisuushi.py` & `mahjong-1.2.1/mahjong/hand_calculating/yaku_list/yakuman/daisuushi.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 from mahjong.constants import EAST, NORTH, SOUTH, WEST
 from mahjong.hand_calculating.yaku import Yaku
 from mahjong.utils import is_pon_or_kan
 
 
 class DaiSuushii(Yaku):
     """
```

### Comparing `mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/yakuman/kokushi.py` & `mahjong-1.2.1/mahjong/hand_calculating/yaku_list/yakuman/kokushi.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 from mahjong.hand_calculating.yaku import Yaku
 
 
 class KokushiMusou(Yaku):
     """
     A hand composed of one of each of the terminals and honour tiles plus
     any tile that matches anything else in the hand.
```

### Comparing `mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/yakuman/shosuushi.py` & `mahjong-1.2.1/mahjong/hand_calculating/yaku_list/yakuman/shosuushi.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 from mahjong.constants import EAST, NORTH, SOUTH, WEST
 from mahjong.hand_calculating.yaku import Yaku
 from mahjong.utils import is_pair, is_pon_or_kan
 
 
 class Shousuushii(Yaku):
     """
```

### Comparing `mahjong-1.2.0.dev7/mahjong/hand_calculating/yaku_list/yakuman/suukantsu.py` & `mahjong-1.2.1/mahjong/hand_calculating/yaku_list/yakuman/tsuisou.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,32 @@
-# -*- coding: utf-8 -*-
+from functools import reduce
+
+from mahjong.constants import HONOR_INDICES
 from mahjong.hand_calculating.yaku import Yaku
-from mahjong.meld import Meld
 
 
-class Suukantsu(Yaku):
+class Tsuuiisou(Yaku):
     """
-    The hand with four kan sets
+    Hand composed entirely of honour tiles
     """
 
     def __init__(self, yaku_id=None):
-        super(Suukantsu, self).__init__(yaku_id)
+        super(Tsuuiisou, self).__init__(yaku_id)
 
     def set_attributes(self):
-        self.tenhou_id = 51
+        self.tenhou_id = 42
 
-        self.name = "Suu Kantsu"
+        self.name = "Tsuu Iisou"
 
         self.han_open = 13
         self.han_closed = 13
 
         self.is_yakuman = True
 
-    def is_condition_met(self, hand, melds, *args):
-        kan_sets = [x for x in melds if x.type == Meld.KAN or x.type == Meld.SHOUMINKAN]
-        return len(kan_sets) == 4
+    def is_condition_met(self, hand, *args):
+        """
+        Hand composed entirely of honour tiles.
+        :param hand: list of hand's sets
+        :return: boolean
+        """
+        indices = reduce(lambda z, y: z + y, hand)
+        return all(x in HONOR_INDICES for x in indices)
```

### Comparing `mahjong-1.2.0.dev7/mahjong/meld.py` & `mahjong-1.2.1/mahjong/meld.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-# -*- coding: utf-8 -*-
 import warnings
 
 from mahjong.tile import TilesConverter
 
 
-class Meld(object):
+class Meld:
     CHI = "chi"
     PON = "pon"
     KAN = "kan"
     SHOUMINKAN = "shouminkan"
     NUKI = "nuki"
 
     who = None
@@ -36,9 +35,9 @@
 
     @property
     def tiles_34(self):
         return [x // 4 for x in self.tiles]
 
     @property
     def CHANKAN(self):
-        warnings.warn("Use .SHOUMINKAN attribute instead of .CHANKAN attribute", DeprecationWarning)
+        warnings.warn("Use .SHOUMINKAN attribute instead of .CHANKAN attribute", DeprecationWarning, stacklevel=2)
         return self.SHOUMINKAN
```

### Comparing `mahjong-1.2.0.dev7/mahjong/shanten.py` & `mahjong-1.2.1/mahjong/shanten.py`

 * *Files identical despite different names*

### Comparing `mahjong-1.2.0.dev7/mahjong/tests_mixin.py` & `mahjong-1.2.1/mahjong/tests_mixin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from mahjong.hand_calculating.divider import HandDivider
 from mahjong.hand_calculating.hand_config import HandConfig, OptionalRules
 from mahjong.meld import Meld
 from mahjong.tile import TilesConverter
 
 
-class TestMixin(object):
+class TestMixin:
     def _string_to_open_34_set(self, sou="", pin="", man="", honors=""):
         open_set = TilesConverter.string_to_136_array(sou=sou, pin=pin, man=man, honors=honors)
         open_set[0] //= 4
         open_set[1] //= 4
         open_set[2] //= 4
         return open_set
```

### Comparing `mahjong-1.2.0.dev7/mahjong/tile.py` & `mahjong-1.2.1/mahjong/tile.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-# -*- coding: utf-8 -*-
 from mahjong.constants import FIVE_RED_MAN, FIVE_RED_PIN, FIVE_RED_SOU
 
 
-class Tile(object):
+class Tile:
     value = None
     is_tsumogiri = None
 
     def __init__(self, value, is_tsumogiri):
         self.value = value
         self.is_tsumogiri = is_tsumogiri
 
 
-class TilesConverter(object):
+class TilesConverter:
     @staticmethod
     def to_one_line_string(tiles, print_aka_dora=False):
         """
         Convert 136 tiles array to the one line string
         Example of output with print_aka_dora=False: 1244579m3p57z
         Example of output with print_aka_dora=True:  1244079m3p57z
         """
```

### Comparing `mahjong-1.2.0.dev7/mahjong/utils.py` & `mahjong-1.2.1/mahjong/utils.py`

 * *Files identical despite different names*

### Comparing `mahjong-1.2.0.dev7/mahjong.egg-info/PKG-INFO` & `mahjong-1.2.1/mahjong.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,41 @@
 Metadata-Version: 2.1
 Name: mahjong
-Version: 1.2.0.dev7
+Version: 1.2.1
 Summary: Mahjong hands calculation
 Home-page: https://github.com/MahjongRepository/mahjong
 Author: Alexey Lisikhin
 Author-email: alexey@nihisil.com
 License: MIT
-Description: This library can calculate hand cost (han, fu with details, yaku, and scores) for riichi mahjong (Japanese version).
-        
-        Also calculating of shanten is supported.
-        
-        The code was validated on tenhou.net phoenix replays in total on **11,120,125 hands**.
-        
-        So, we can say that our hand calculator works the same way that tenhou.net hand calculation.
-        
-        # How to install
-        
-        ```bash
-        pip install mahjong
-        ```
-        
-        # Supported rules and usage examples
-        
-        You can find usage examples and information about all supported rules variations in the [wiki](https://github.com/MahjongRepository/mahjong/wiki)
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+[![Mahjong lib](https://github.com/MahjongRepository/mahjong/actions/workflows/lint_and_test.yml/badge.svg)](https://github.com/MahjongRepository/mahjong/actions/workflows/lint_and_test.yml)
+
+This library can calculate hand cost (han, fu with details, yaku, and scores) for riichi mahjong (Japanese version).
+
+Also calculating of shanten is supported.
+
+The code was validated on tenhou.net phoenix replays in total on **11,120,125 hands**.
+
+So, we can say that our hand calculator works the same way that tenhou.net hand calculation.
+
+# How to install
+
+```bash
+pip install mahjong
+```
+
+# Supported rules and usage examples
+
+You can find usage examples and information about all supported rules variations in the [wiki](https://github.com/MahjongRepository/mahjong/wiki)
```

### Comparing `mahjong-1.2.0.dev7/mahjong.egg-info/SOURCES.txt` & `mahjong-1.2.1/mahjong.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 LICENSE.txt
-README.rst
+README.md
 pyproject.toml
 setup.cfg
 setup.py
 mahjong/__init__.py
 mahjong/agari.py
 mahjong/constants.py
 mahjong/meld.py
```

### Comparing `mahjong-1.2.0.dev7/setup.py` & `mahjong-1.2.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,28 +10,29 @@
     name="mahjong",
     packages=[
         "mahjong",
         "mahjong.hand_calculating",
         "mahjong.hand_calculating.yaku_list",
         "mahjong.hand_calculating.yaku_list.yakuman",
     ],
-    version="1.2.0.dev7",
+    version="1.2.1",
     description="Mahjong hands calculation",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Alexey Lisikhin",
     author_email="alexey@nihisil.com",
     url="https://github.com/MahjongRepository/mahjong",
     license='MIT',
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Console",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
 )
```

