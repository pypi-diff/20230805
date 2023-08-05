# Comparing `tmp/aramgg-poro-0.0.7.tar.gz` & `tmp/aramgg-poro-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aramgg-poro-0.0.7.tar", last modified: Sun Jul  2 08:04:31 2023, max compression
+gzip compressed data, was "aramgg-poro-0.0.8.tar", last modified: Sat Aug  5 06:17:38 2023, max compression
```

## Comparing `aramgg-poro-0.0.7.tar` & `aramgg-poro-0.0.8.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxrwxrwx   0        0        0        0 2023-07-02 08:04:31.501217 aramgg-poro-0.0.7/
--rw-rw-rw-   0        0        0        6 2023-07-01 08:54:15.000000 aramgg-poro-0.0.7/LICENSE.txt
--rw-rw-rw-   0        0        0      503 2023-07-02 08:04:31.500216 aramgg-poro-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0       24 2023-07-01 08:53:39.000000 aramgg-poro-0.0.7/README.md
--rw-rw-rw-   0        0        0      126 2023-07-02 08:04:15.000000 aramgg-poro-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-02 08:04:31.501217 aramgg-poro-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      782 2023-07-02 08:02:24.000000 aramgg-poro-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-02 08:04:31.402215 aramgg-poro-0.0.7/src/
-drwxrwxrwx   0        0        0        0 2023-07-02 08:04:31.430215 aramgg-poro-0.0.7/src/aramgg_poro.egg-info/
--rw-rw-rw-   0        0        0      503 2023-07-02 08:04:31.000000 aramgg-poro-0.0.7/src/aramgg_poro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2045 2023-07-02 08:04:31.000000 aramgg-poro-0.0.7/src/aramgg_poro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-02 08:04:31.000000 aramgg-poro-0.0.7/src/aramgg_poro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-07-02 08:04:31.000000 aramgg-poro-0.0.7/src/aramgg_poro.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-02 08:04:31.435216 aramgg-poro-0.0.7/src/poro/
--rw-rw-rw-   0        0        0      517 2023-07-02 07:51:25.000000 aramgg-poro-0.0.7/src/poro/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-02 08:04:31.438215 aramgg-poro-0.0.7/src/poro/_configuration/
--rw-rw-rw-   0        0        0      130 2023-06-02 08:31:36.000000 aramgg-poro-0.0.7/src/poro/_configuration/__init__.py
--rw-rw-rw-   0        0        0     1385 2023-07-02 08:02:31.000000 aramgg-poro-0.0.7/src/poro/_configuration/pipeline.py
-drwxrwxrwx   0        0        0        0 2023-07-02 08:04:31.440216 aramgg-poro-0.0.7/src/poro/apis/
--rw-rw-rw-   0        0        0      506 2023-07-02 07:49:16.000000 aramgg-poro-0.0.7/src/poro/apis/__init__.py
--rw-rw-rw-   0        0        0     2243 2023-07-02 08:02:45.000000 aramgg-poro-0.0.7/src/poro/apis/common.py
-drwxrwxrwx   0        0        0        0 2023-07-02 08:04:31.450216 aramgg-poro-0.0.7/src/poro/apis/ddragon/
--rw-rw-rw-   0        0        0      221 2023-06-11 08:38:54.000000 aramgg-poro-0.0.7/src/poro/apis/ddragon/__init__.py
--rw-rw-rw-   0        0        0      416 2023-06-06 12:00:55.000000 aramgg-poro-0.0.7/src/poro/apis/ddragon/champion.py
--rw-rw-rw-   0        0        0      380 2023-06-09 09:45:43.000000 aramgg-poro-0.0.7/src/poro/apis/ddragon/item.py
--rw-rw-rw-   0        0        0     1665 2023-06-22 05:42:40.000000 aramgg-poro-0.0.7/src/poro/apis/ddragon/perk.py
--rw-rw-rw-   0        0        0      438 2023-06-11 07:56:52.000000 aramgg-poro-0.0.7/src/poro/apis/ddragon/profileicon.py
--rw-rw-rw-   0        0        0      391 2023-06-11 07:46:08.000000 aramgg-poro-0.0.7/src/poro/apis/ddragon/spell.py
--rw-rw-rw-   0        0        0     1899 2023-06-23 03:29:48.000000 aramgg-poro-0.0.7/src/poro/apis/ddragon/sprite.py
--rw-rw-rw-   0        0        0      334 2023-06-06 07:47:25.000000 aramgg-poro-0.0.7/src/poro/apis/ddragon/version.py
-drwxrwxrwx   0        0        0        0 2023-07-02 08:04:31.454215 aramgg-poro-0.0.7/src/poro/apis/riotapi/
--rw-rw-rw-   0        0        0       62 2023-06-03 06:24:09.000000 aramgg-poro-0.0.7/src/poro/apis/riotapi/__init__.py
--rw-rw-rw-   0        0        0     1945 2023-06-21 07:43:30.000000 aramgg-poro-0.0.7/src/poro/apis/riotapi/match.py
--rw-rw-rw-   0        0        0      711 2023-06-03 07:20:05.000000 aramgg-poro-0.0.7/src/poro/apis/riotapi/summoner.py
-drwxrwxrwx   0        0        0        0 2023-07-02 08:04:31.456216 aramgg-poro-0.0.7/src/poro/core/
--rw-rw-rw-   0        0        0      364 2023-06-22 04:53:16.000000 aramgg-poro-0.0.7/src/poro/core/__init__.py
--rw-rw-rw-   0        0        0     3032 2023-06-26 09:42:10.000000 aramgg-poro-0.0.7/src/poro/core/common.py
-drwxrwxrwx   0        0        0        0 2023-07-02 08:04:31.466215 aramgg-poro-0.0.7/src/poro/core/ddragon/
--rw-rw-rw-   0        0        0        0 2023-07-01 09:01:00.000000 aramgg-poro-0.0.7/src/poro/core/ddragon/__init__.py
--rw-rw-rw-   0        0        0      738 2023-06-28 06:05:41.000000 aramgg-poro-0.0.7/src/poro/core/ddragon/champion.py
--rw-rw-rw-   0        0        0      698 2023-06-28 06:14:01.000000 aramgg-poro-0.0.7/src/poro/core/ddragon/item.py
--rw-rw-rw-   0        0        0     1396 2023-06-28 06:22:32.000000 aramgg-poro-0.0.7/src/poro/core/ddragon/perk.py
--rw-rw-rw-   0        0        0      770 2023-06-28 07:42:55.000000 aramgg-poro-0.0.7/src/poro/core/ddragon/profileicon.py
--rw-rw-rw-   0        0        0      708 2023-06-28 06:33:20.000000 aramgg-poro-0.0.7/src/poro/core/ddragon/spell.py
--rw-rw-rw-   0        0        0     1140 2023-06-28 06:13:14.000000 aramgg-poro-0.0.7/src/poro/core/ddragon/sprite.py
--rw-rw-rw-   0        0        0      405 2023-06-07 09:25:57.000000 aramgg-poro-0.0.7/src/poro/core/ddragon/version.py
-drwxrwxrwx   0        0        0        0 2023-07-02 08:04:31.469215 aramgg-poro-0.0.7/src/poro/core/riotapi/
--rw-rw-rw-   0        0        0        0 2023-07-01 09:01:07.000000 aramgg-poro-0.0.7/src/poro/core/riotapi/__init__.py
--rw-rw-rw-   0        0        0    11058 2023-07-01 07:28:51.000000 aramgg-poro-0.0.7/src/poro/core/riotapi/match.py
--rw-rw-rw-   0        0        0     1846 2023-06-07 08:37:25.000000 aramgg-poro-0.0.7/src/poro/core/riotapi/summoner.py
--rw-rw-rw-   0        0        0     1318 2023-06-03 07:10:29.000000 aramgg-poro-0.0.7/src/poro/data.py
-drwxrwxrwx   0        0        0        0 2023-07-02 08:04:31.471217 aramgg-poro-0.0.7/src/poro/dto/
--rw-rw-rw-   0        0        0        0 2023-06-01 12:38:41.000000 aramgg-poro-0.0.7/src/poro/dto/__init__.py
--rw-rw-rw-   0        0        0      194 2023-06-01 08:03:02.000000 aramgg-poro-0.0.7/src/poro/dto/common.py
-drwxrwxrwx   0        0        0        0 2023-07-02 08:04:31.481216 aramgg-poro-0.0.7/src/poro/dto/ddragon/
--rw-rw-rw-   0        0        0        0 2023-07-01 09:04:36.000000 aramgg-poro-0.0.7/src/poro/dto/ddragon/__init__.py
--rw-rw-rw-   0        0        0      120 2023-06-06 07:02:47.000000 aramgg-poro-0.0.7/src/poro/dto/ddragon/champion.py
--rw-rw-rw-   0        0        0       73 2023-06-09 09:42:30.000000 aramgg-poro-0.0.7/src/poro/dto/ddragon/item.py
--rw-rw-rw-   0        0        0      120 2023-06-22 05:00:47.000000 aramgg-poro-0.0.7/src/poro/dto/ddragon/perk.py
--rw-rw-rw-   0        0        0       80 2023-06-11 07:53:34.000000 aramgg-poro-0.0.7/src/poro/dto/ddragon/profileicon.py
--rw-rw-rw-   0        0        0       74 2023-06-11 07:44:17.000000 aramgg-poro-0.0.7/src/poro/dto/ddragon/spell.py
--rw-rw-rw-   0        0        0       75 2023-06-11 08:01:00.000000 aramgg-poro-0.0.7/src/poro/dto/ddragon/sprite.py
--rw-rw-rw-   0        0        0       76 2023-06-06 06:49:37.000000 aramgg-poro-0.0.7/src/poro/dto/ddragon/version.py
-drwxrwxrwx   0        0        0        0 2023-07-02 08:04:31.485216 aramgg-poro-0.0.7/src/poro/dto/riotapi/
--rw-rw-rw-   0        0        0        0 2023-07-01 09:04:30.000000 aramgg-poro-0.0.7/src/poro/dto/riotapi/__init__.py
--rw-rw-rw-   0        0        0      114 2023-06-03 06:41:57.000000 aramgg-poro-0.0.7/src/poro/dto/riotapi/match.py
--rw-rw-rw-   0        0        0       73 2023-06-02 04:47:17.000000 aramgg-poro-0.0.7/src/poro/dto/riotapi/summoner.py
--rw-rw-rw-   0        0        0       94 2023-07-02 07:51:04.000000 aramgg-poro-0.0.7/src/poro/poro.py
-drwxrwxrwx   0        0        0        0 2023-07-02 08:04:31.486217 aramgg-poro-0.0.7/src/poro/transformers/
--rw-rw-rw-   0        0        0      533 2023-06-11 08:41:07.000000 aramgg-poro-0.0.7/src/poro/transformers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-02 08:04:31.496215 aramgg-poro-0.0.7/src/poro/transformers/ddragon/
--rw-rw-rw-   0        0        0      277 2023-06-11 08:43:26.000000 aramgg-poro-0.0.7/src/poro/transformers/ddragon/__init__.py
--rw-rw-rw-   0        0        0      269 2023-06-06 11:59:32.000000 aramgg-poro-0.0.7/src/poro/transformers/ddragon/champion.py
--rw-rw-rw-   0        0        0      233 2023-06-09 09:47:31.000000 aramgg-poro-0.0.7/src/poro/transformers/ddragon/item.py
--rw-rw-rw-   0        0        0      402 2023-06-22 04:52:50.000000 aramgg-poro-0.0.7/src/poro/transformers/ddragon/perk.py
--rw-rw-rw-   0        0        0      297 2023-06-11 07:57:49.000000 aramgg-poro-0.0.7/src/poro/transformers/ddragon/profileicon.py
--rw-rw-rw-   0        0        0      242 2023-06-11 07:49:08.000000 aramgg-poro-0.0.7/src/poro/transformers/ddragon/spell.py
--rw-rw-rw-   0        0        0      251 2023-06-11 08:40:48.000000 aramgg-poro-0.0.7/src/poro/transformers/ddragon/sprite.py
--rw-rw-rw-   0        0        0      256 2023-06-06 07:30:27.000000 aramgg-poro-0.0.7/src/poro/transformers/ddragon/version.py
-drwxrwxrwx   0        0        0        0 2023-07-02 08:04:31.499216 aramgg-poro-0.0.7/src/poro/transformers/riotapi/
--rw-rw-rw-   0        0        0       78 2023-06-11 07:36:21.000000 aramgg-poro-0.0.7/src/poro/transformers/riotapi/__init__.py
--rw-rw-rw-   0        0        0      362 2023-06-03 07:25:53.000000 aramgg-poro-0.0.7/src/poro/transformers/riotapi/match.py
--rw-rw-rw-   0        0        0      333 2023-06-02 07:12:46.000000 aramgg-poro-0.0.7/src/poro/transformers/riotapi/summoner.py
--rw-rw-rw-   0        0        0     1039 2023-06-28 05:57:58.000000 aramgg-poro-0.0.7/src/poro/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-05 06:17:38.317005 aramgg-poro-0.0.8/
+-rw-rw-rw-   0        0        0        6 2023-07-01 08:54:15.000000 aramgg-poro-0.0.8/LICENSE.txt
+-rw-rw-rw-   0        0        0      503 2023-08-05 06:17:38.316006 aramgg-poro-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0       24 2023-07-01 08:53:39.000000 aramgg-poro-0.0.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-05 06:17:38.317005 aramgg-poro-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      901 2023-08-05 06:16:38.000000 aramgg-poro-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-05 06:17:38.224005 aramgg-poro-0.0.8/src/
+drwxrwxrwx   0        0        0        0 2023-08-05 06:17:38.249005 aramgg-poro-0.0.8/src/aramgg_poro.egg-info/
+-rw-rw-rw-   0        0        0      503 2023-08-05 06:17:38.000000 aramgg-poro-0.0.8/src/aramgg_poro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2068 2023-08-05 06:17:38.000000 aramgg-poro-0.0.8/src/aramgg_poro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 06:17:38.000000 aramgg-poro-0.0.8/src/aramgg_poro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2023-08-05 06:17:38.000000 aramgg-poro-0.0.8/src/aramgg_poro.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-08-05 06:17:38.000000 aramgg-poro-0.0.8/src/aramgg_poro.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-05 06:17:38.254005 aramgg-poro-0.0.8/src/poro/
+-rw-rw-rw-   0        0        0      517 2023-07-02 07:51:25.000000 aramgg-poro-0.0.8/src/poro/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-05 06:17:38.257005 aramgg-poro-0.0.8/src/poro/_configuration/
+-rw-rw-rw-   0        0        0      130 2023-06-02 08:31:36.000000 aramgg-poro-0.0.8/src/poro/_configuration/__init__.py
+-rw-rw-rw-   0        0        0     1385 2023-07-02 08:02:31.000000 aramgg-poro-0.0.8/src/poro/_configuration/pipeline.py
+drwxrwxrwx   0        0        0        0 2023-08-05 06:17:38.259004 aramgg-poro-0.0.8/src/poro/apis/
+-rw-rw-rw-   0        0        0      506 2023-07-02 07:49:16.000000 aramgg-poro-0.0.8/src/poro/apis/__init__.py
+-rw-rw-rw-   0        0        0     2243 2023-07-02 08:02:45.000000 aramgg-poro-0.0.8/src/poro/apis/common.py
+drwxrwxrwx   0        0        0        0 2023-08-05 06:17:38.269005 aramgg-poro-0.0.8/src/poro/apis/ddragon/
+-rw-rw-rw-   0        0        0      221 2023-06-11 08:38:54.000000 aramgg-poro-0.0.8/src/poro/apis/ddragon/__init__.py
+-rw-rw-rw-   0        0        0      416 2023-06-06 12:00:55.000000 aramgg-poro-0.0.8/src/poro/apis/ddragon/champion.py
+-rw-rw-rw-   0        0        0      380 2023-06-09 09:45:43.000000 aramgg-poro-0.0.8/src/poro/apis/ddragon/item.py
+-rw-rw-rw-   0        0        0     1665 2023-06-22 05:42:40.000000 aramgg-poro-0.0.8/src/poro/apis/ddragon/perk.py
+-rw-rw-rw-   0        0        0      438 2023-06-11 07:56:52.000000 aramgg-poro-0.0.8/src/poro/apis/ddragon/profileicon.py
+-rw-rw-rw-   0        0        0      391 2023-06-11 07:46:08.000000 aramgg-poro-0.0.8/src/poro/apis/ddragon/spell.py
+-rw-rw-rw-   0        0        0     1899 2023-06-23 03:29:48.000000 aramgg-poro-0.0.8/src/poro/apis/ddragon/sprite.py
+-rw-rw-rw-   0        0        0      334 2023-06-06 07:47:25.000000 aramgg-poro-0.0.8/src/poro/apis/ddragon/version.py
+drwxrwxrwx   0        0        0        0 2023-08-05 06:17:38.272005 aramgg-poro-0.0.8/src/poro/apis/riotapi/
+-rw-rw-rw-   0        0        0       62 2023-06-03 06:24:09.000000 aramgg-poro-0.0.8/src/poro/apis/riotapi/__init__.py
+-rw-rw-rw-   0        0        0     1945 2023-06-21 07:43:30.000000 aramgg-poro-0.0.8/src/poro/apis/riotapi/match.py
+-rw-rw-rw-   0        0        0      711 2023-06-03 07:20:05.000000 aramgg-poro-0.0.8/src/poro/apis/riotapi/summoner.py
+drwxrwxrwx   0        0        0        0 2023-08-05 06:17:38.275006 aramgg-poro-0.0.8/src/poro/core/
+-rw-rw-rw-   0        0        0      364 2023-06-22 04:53:16.000000 aramgg-poro-0.0.8/src/poro/core/__init__.py
+-rw-rw-rw-   0        0        0     3032 2023-06-26 09:42:10.000000 aramgg-poro-0.0.8/src/poro/core/common.py
+drwxrwxrwx   0        0        0        0 2023-08-05 06:17:38.284005 aramgg-poro-0.0.8/src/poro/core/ddragon/
+-rw-rw-rw-   0        0        0        0 2023-07-01 09:01:00.000000 aramgg-poro-0.0.8/src/poro/core/ddragon/__init__.py
+-rw-rw-rw-   0        0        0      738 2023-06-28 06:05:41.000000 aramgg-poro-0.0.8/src/poro/core/ddragon/champion.py
+-rw-rw-rw-   0        0        0      698 2023-06-28 06:14:01.000000 aramgg-poro-0.0.8/src/poro/core/ddragon/item.py
+-rw-rw-rw-   0        0        0     1396 2023-06-28 06:22:32.000000 aramgg-poro-0.0.8/src/poro/core/ddragon/perk.py
+-rw-rw-rw-   0        0        0      770 2023-06-28 07:42:55.000000 aramgg-poro-0.0.8/src/poro/core/ddragon/profileicon.py
+-rw-rw-rw-   0        0        0      708 2023-06-28 06:33:20.000000 aramgg-poro-0.0.8/src/poro/core/ddragon/spell.py
+-rw-rw-rw-   0        0        0     1140 2023-06-28 06:13:14.000000 aramgg-poro-0.0.8/src/poro/core/ddragon/sprite.py
+-rw-rw-rw-   0        0        0      405 2023-06-07 09:25:57.000000 aramgg-poro-0.0.8/src/poro/core/ddragon/version.py
+drwxrwxrwx   0        0        0        0 2023-08-05 06:17:38.287004 aramgg-poro-0.0.8/src/poro/core/riotapi/
+-rw-rw-rw-   0        0        0        0 2023-07-01 09:01:07.000000 aramgg-poro-0.0.8/src/poro/core/riotapi/__init__.py
+-rw-rw-rw-   0        0        0    11058 2023-07-01 07:28:51.000000 aramgg-poro-0.0.8/src/poro/core/riotapi/match.py
+-rw-rw-rw-   0        0        0     1846 2023-06-07 08:37:25.000000 aramgg-poro-0.0.8/src/poro/core/riotapi/summoner.py
+-rw-rw-rw-   0        0        0     1318 2023-06-03 07:10:29.000000 aramgg-poro-0.0.8/src/poro/data.py
+drwxrwxrwx   0        0        0        0 2023-08-05 06:17:38.289004 aramgg-poro-0.0.8/src/poro/dto/
+-rw-rw-rw-   0        0        0        0 2023-06-01 12:38:41.000000 aramgg-poro-0.0.8/src/poro/dto/__init__.py
+-rw-rw-rw-   0        0        0      194 2023-06-01 08:03:02.000000 aramgg-poro-0.0.8/src/poro/dto/common.py
+drwxrwxrwx   0        0        0        0 2023-08-05 06:17:38.298006 aramgg-poro-0.0.8/src/poro/dto/ddragon/
+-rw-rw-rw-   0        0        0        0 2023-07-01 09:04:36.000000 aramgg-poro-0.0.8/src/poro/dto/ddragon/__init__.py
+-rw-rw-rw-   0        0        0      120 2023-06-06 07:02:47.000000 aramgg-poro-0.0.8/src/poro/dto/ddragon/champion.py
+-rw-rw-rw-   0        0        0       73 2023-06-09 09:42:30.000000 aramgg-poro-0.0.8/src/poro/dto/ddragon/item.py
+-rw-rw-rw-   0        0        0      120 2023-06-22 05:00:47.000000 aramgg-poro-0.0.8/src/poro/dto/ddragon/perk.py
+-rw-rw-rw-   0        0        0       80 2023-06-11 07:53:34.000000 aramgg-poro-0.0.8/src/poro/dto/ddragon/profileicon.py
+-rw-rw-rw-   0        0        0       74 2023-06-11 07:44:17.000000 aramgg-poro-0.0.8/src/poro/dto/ddragon/spell.py
+-rw-rw-rw-   0        0        0       75 2023-06-11 08:01:00.000000 aramgg-poro-0.0.8/src/poro/dto/ddragon/sprite.py
+-rw-rw-rw-   0        0        0       76 2023-06-06 06:49:37.000000 aramgg-poro-0.0.8/src/poro/dto/ddragon/version.py
+drwxrwxrwx   0        0        0        0 2023-08-05 06:17:38.301005 aramgg-poro-0.0.8/src/poro/dto/riotapi/
+-rw-rw-rw-   0        0        0        0 2023-07-01 09:04:30.000000 aramgg-poro-0.0.8/src/poro/dto/riotapi/__init__.py
+-rw-rw-rw-   0        0        0      114 2023-06-03 06:41:57.000000 aramgg-poro-0.0.8/src/poro/dto/riotapi/match.py
+-rw-rw-rw-   0        0        0       73 2023-06-02 04:47:17.000000 aramgg-poro-0.0.8/src/poro/dto/riotapi/summoner.py
+-rw-rw-rw-   0        0        0       94 2023-07-02 07:51:04.000000 aramgg-poro-0.0.8/src/poro/poro.py
+drwxrwxrwx   0        0        0        0 2023-08-05 06:17:38.302007 aramgg-poro-0.0.8/src/poro/transformers/
+-rw-rw-rw-   0        0        0      533 2023-06-11 08:41:07.000000 aramgg-poro-0.0.8/src/poro/transformers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-05 06:17:38.312007 aramgg-poro-0.0.8/src/poro/transformers/ddragon/
+-rw-rw-rw-   0        0        0      277 2023-06-11 08:43:26.000000 aramgg-poro-0.0.8/src/poro/transformers/ddragon/__init__.py
+-rw-rw-rw-   0        0        0      269 2023-06-06 11:59:32.000000 aramgg-poro-0.0.8/src/poro/transformers/ddragon/champion.py
+-rw-rw-rw-   0        0        0      233 2023-06-09 09:47:31.000000 aramgg-poro-0.0.8/src/poro/transformers/ddragon/item.py
+-rw-rw-rw-   0        0        0      402 2023-06-22 04:52:50.000000 aramgg-poro-0.0.8/src/poro/transformers/ddragon/perk.py
+-rw-rw-rw-   0        0        0      297 2023-06-11 07:57:49.000000 aramgg-poro-0.0.8/src/poro/transformers/ddragon/profileicon.py
+-rw-rw-rw-   0        0        0      242 2023-06-11 07:49:08.000000 aramgg-poro-0.0.8/src/poro/transformers/ddragon/spell.py
+-rw-rw-rw-   0        0        0      251 2023-06-11 08:40:48.000000 aramgg-poro-0.0.8/src/poro/transformers/ddragon/sprite.py
+-rw-rw-rw-   0        0        0      256 2023-06-06 07:30:27.000000 aramgg-poro-0.0.8/src/poro/transformers/ddragon/version.py
+drwxrwxrwx   0        0        0        0 2023-08-05 06:17:38.315006 aramgg-poro-0.0.8/src/poro/transformers/riotapi/
+-rw-rw-rw-   0        0        0       78 2023-06-11 07:36:21.000000 aramgg-poro-0.0.8/src/poro/transformers/riotapi/__init__.py
+-rw-rw-rw-   0        0        0      362 2023-06-03 07:25:53.000000 aramgg-poro-0.0.8/src/poro/transformers/riotapi/match.py
+-rw-rw-rw-   0        0        0      333 2023-06-02 07:12:46.000000 aramgg-poro-0.0.8/src/poro/transformers/riotapi/summoner.py
+-rw-rw-rw-   0        0        0     1039 2023-06-28 05:57:58.000000 aramgg-poro-0.0.8/src/poro/utils.py
```

### Comparing `aramgg-poro-0.0.7/setup.py` & `aramgg-poro-0.0.8/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
+install_requires= [
+    "setuptools>=42",
+    "Pillow",
+    "requests"
+]
+
 setuptools.setup(
     name="aramgg-poro",
-    version="0.0.7",
+    version="0.0.8",
     author="peep12ng",
     author_email="peep12ng@gmail.com",
     description="aramgg riotapi lib",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/poro/",
     project_urls={
@@ -19,8 +25,9 @@
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
     python_requires=">=3.6",
+    install_requires=install_requires
 )
```

### Comparing `aramgg-poro-0.0.7/src/aramgg_poro.egg-info/SOURCES.txt` & `aramgg-poro-0.0.8/src/aramgg_poro.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 LICENSE.txt
 README.md
-pyproject.toml
 setup.py
 src/aramgg_poro.egg-info/PKG-INFO
 src/aramgg_poro.egg-info/SOURCES.txt
 src/aramgg_poro.egg-info/dependency_links.txt
+src/aramgg_poro.egg-info/requires.txt
 src/aramgg_poro.egg-info/top_level.txt
 src/poro/__init__.py
 src/poro/data.py
 src/poro/poro.py
 src/poro/utils.py
 src/poro/_configuration/__init__.py
 src/poro/_configuration/pipeline.py
```

### Comparing `aramgg-poro-0.0.7/src/poro/__init__.py` & `aramgg-poro-0.0.8/src/poro/__init__.py`

 * *Files identical despite different names*

### Comparing `aramgg-poro-0.0.7/src/poro/_configuration/pipeline.py` & `aramgg-poro-0.0.8/src/poro/_configuration/pipeline.py`

 * *Files identical despite different names*

### Comparing `aramgg-poro-0.0.7/src/poro/apis/common.py` & `aramgg-poro-0.0.8/src/poro/apis/common.py`

 * *Files identical despite different names*

### Comparing `aramgg-poro-0.0.7/src/poro/apis/ddragon/perk.py` & `aramgg-poro-0.0.8/src/poro/apis/ddragon/perk.py`

 * *Files identical despite different names*

### Comparing `aramgg-poro-0.0.7/src/poro/apis/ddragon/sprite.py` & `aramgg-poro-0.0.8/src/poro/apis/ddragon/sprite.py`

 * *Files identical despite different names*

### Comparing `aramgg-poro-0.0.7/src/poro/apis/riotapi/match.py` & `aramgg-poro-0.0.8/src/poro/apis/riotapi/match.py`

 * *Files identical despite different names*

### Comparing `aramgg-poro-0.0.7/src/poro/apis/riotapi/summoner.py` & `aramgg-poro-0.0.8/src/poro/apis/riotapi/summoner.py`

 * *Files identical despite different names*

### Comparing `aramgg-poro-0.0.7/src/poro/core/common.py` & `aramgg-poro-0.0.8/src/poro/core/common.py`

 * *Files identical despite different names*

### Comparing `aramgg-poro-0.0.7/src/poro/core/ddragon/champion.py` & `aramgg-poro-0.0.8/src/poro/core/ddragon/champion.py`

 * *Files identical despite different names*

### Comparing `aramgg-poro-0.0.7/src/poro/core/ddragon/item.py` & `aramgg-poro-0.0.8/src/poro/core/ddragon/item.py`

 * *Files identical despite different names*

### Comparing `aramgg-poro-0.0.7/src/poro/core/ddragon/perk.py` & `aramgg-poro-0.0.8/src/poro/core/ddragon/perk.py`

 * *Files identical despite different names*

### Comparing `aramgg-poro-0.0.7/src/poro/core/ddragon/profileicon.py` & `aramgg-poro-0.0.8/src/poro/core/ddragon/profileicon.py`

 * *Files identical despite different names*

### Comparing `aramgg-poro-0.0.7/src/poro/core/ddragon/spell.py` & `aramgg-poro-0.0.8/src/poro/core/ddragon/spell.py`

 * *Files identical despite different names*

### Comparing `aramgg-poro-0.0.7/src/poro/core/ddragon/sprite.py` & `aramgg-poro-0.0.8/src/poro/core/ddragon/sprite.py`

 * *Files identical despite different names*

### Comparing `aramgg-poro-0.0.7/src/poro/core/riotapi/match.py` & `aramgg-poro-0.0.8/src/poro/core/riotapi/match.py`

 * *Files identical despite different names*

### Comparing `aramgg-poro-0.0.7/src/poro/core/riotapi/summoner.py` & `aramgg-poro-0.0.8/src/poro/core/riotapi/summoner.py`

 * *Files identical despite different names*

### Comparing `aramgg-poro-0.0.7/src/poro/data.py` & `aramgg-poro-0.0.8/src/poro/data.py`

 * *Files identical despite different names*

### Comparing `aramgg-poro-0.0.7/src/poro/transformers/__init__.py` & `aramgg-poro-0.0.8/src/poro/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `aramgg-poro-0.0.7/src/poro/utils.py` & `aramgg-poro-0.0.8/src/poro/utils.py`

 * *Files identical despite different names*

