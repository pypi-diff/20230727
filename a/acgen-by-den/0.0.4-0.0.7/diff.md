# Comparing `tmp/acgen_by_den-0.0.4.tar.gz` & `tmp/acgen_by_den-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acgen_by_den-0.0.4.tar", last modified: Thu Jul 27 05:51:47 2023, max compression
+gzip compressed data, was "acgen_by_den-0.0.7.tar", last modified: Thu Jul 27 06:34:05 2023, max compression
```

## Comparing `acgen_by_den-0.0.4.tar` & `acgen_by_den-0.0.7.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 05:51:47.822356 acgen_by_den-0.0.4/
--rw-rw-rw-   0        0        0      472 2023-07-27 05:51:47.820370 acgen_by_den-0.0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-27 05:51:47.212451 acgen_by_den-0.0.4/acgen_by_den/
--rw-rw-rw-   0        0        0      281 2023-03-22 22:39:32.000000 acgen_by_den-0.0.4/acgen_by_den/__init__.py
--rw-rw-rw-   0        0        0     8327 2023-07-26 23:42:21.000000 acgen_by_den-0.0.4/acgen_by_den/__main__.py
--rw-rw-rw-   0        0        0    10151 2023-03-22 22:39:32.000000 acgen_by_den-0.0.4/acgen_by_den/adb_handler.py
--rw-rw-rw-   0        0        0    13745 2023-03-22 22:39:32.000000 acgen_by_den-0.0.4/acgen_by_den/config_manager.py
--rw-rw-rw-   0        0        0     1501 2023-03-22 22:39:32.000000 acgen_by_den-0.0.4/acgen_by_den/csv_handler.py
-drwxrwxrwx   0        0        0        0 2023-07-27 05:51:47.284964 acgen_by_den-0.0.4/acgen_by_den/edits/
--rw-rw-rw-   0        0        0       67 2023-03-22 22:39:32.000000 acgen_by_den-0.0.4/acgen_by_den/edits/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-27 05:51:47.328671 acgen_by_den-0.0.4/acgen_by_den/edits/basic/
--rw-rw-rw-   0        0        0      122 2023-03-22 22:39:32.000000 acgen_by_den-0.0.4/acgen_by_den/edits/basic/__init__.py
--rw-rw-rw-   0        0        0     8690 2023-03-22 22:39:32.000000 acgen_by_den-0.0.4/acgen_by_den/edits/basic/basic_items.py
--rw-rw-rw-   0        0        0     1490 2023-03-22 22:39:32.000000 acgen_by_den-0.0.4/acgen_by_den/edits/basic/catfruit.py
--rw-rw-rw-   0        0        0     1931 2023-03-22 22:39:32.000000 acgen_by_den-0.0.4/acgen_by_den/edits/basic/catseyes.py
--rw-rw-rw-   0        0        0     1647 2023-03-22 22:39:32.000000 acgen_by_den-0.0.4/acgen_by_den/edits/basic/ototo_base_mats.py
--rw-rw-rw-   0        0        0     3984 2023-03-22 22:39:32.000000 acgen_by_den-0.0.4/acgen_by_den/edits/basic/talent_orbs.py
--rw-rw-rw-   0        0        0    16533 2023-03-22 22:39:32.000000 acgen_by_den-0.0.4/acgen_by_den/edits/basic/talent_orbs_new.py
-drwxrwxrwx   0        0        0        0 2023-07-27 05:51:47.405156 acgen_by_den-0.0.4/acgen_by_den/edits/cats/
--rw-rw-rw-   0        0        0      179 2023-03-22 22:39:32.000000 acgen_by_den-0.0.4/acgen_by_den/edits/cats/__init__.py
--rw-rw-rw-   0        0        0     8978 2023-03-22 22:39:32.000000 acgen_by_den-0.0.4/acgen_by_den/edits/cats/cat_helper.py
--rw-rw-rw-   0        0        0    11121 2023-03-22 22:39:32.000000 acgen_by_den-0.0.4/acgen_by_den/edits/cats/cat_id_selector.py
--rw-rw-rw-   0        0        0     3249 2023-03-22 22:39:32.000000 acgen_by_den-0.0.4/acgen_by_den/edits/cats/chara_drop.py
--rw-rw-rw-   0        0        0     1068 2023-03-22 22:39:32.000000 acgen_by_den-0.0.4/acgen_by_den/edits/cats/clear_cat_guide.py
--rw-rw-rw-   0        0        0     2844 2023-03-22 22:39:32.000000 acgen_by_den-0.0.4/acgen_by_den/edits/cats/evolve_cats.py
--rw-rw-rw-   0        0        0     1260 2023-03-22 22:39:32.000000 acgen_by_den-0.0.4/acgen_by_den/edits/cats/get_remove_cats.py
--rw-rw-rw-   0        0        0     7936 2023-03-22 22:39:32.000000 acgen_by_den-0.0.4/acgen_by_den/edits/cats/talents.py
--rw-rw-rw-   0        0        0     1900 2023-03-22 22:39:32.000000 acgen_by_den-0.0.4/acgen_by_den/edits/cats/upgrade_blue.py
--rw-rw-rw-   0        0        0     4428 2023-03-22 22:39:32.000000 acgen_by_den-0.0.4/acgen_by_den/edits/cats/upgrade_cats.py
-drwxrwxrwx   0        0        0        0 2023-07-27 05:51:47.425022 acgen_by_den-0.0.4/acgen_by_den/edits/gamototo/
--rw-rw-rw-   0        0        0       66 2023-03-22 22:39:32.000000 acgen_by_den-0.0.4/acgen_by_den/edits/gamototo/__init__.py
--rw-rw-rw-   0        0        0      309 2023-03-22 22:39:32.000000 acgen_by_den-0.0.4/acgen_by_den/edits/gamototo/fix_gamatoto.py
--rw-rw-rw-   0        0        0     2794 2023-03-22 22:39:32.000000 acgen_by_den-0.0.4/acgen_by_den/edits/gamototo/gamatoto_xp.py
--rw-rw-rw-   0        0        0     3393 2023-03-22 22:39:32.000000 acgen_by_den-0.0.4/acgen_by_den/edits/gamototo/helpers.py
--rw-rw-rw-   0        0        0     4137 2023-03-22 22:39:32.000000 acgen_by_den-0.0.4/acgen_by_den/edits/gamototo/ototo_cat_cannon.py
-drwxrwxrwx   0        0        0        0 2023-07-27 05:51:47.603824 acgen_by_den-0.0.4/acgen_by_den/edits/levels/
--rw-rw-rw-   0        0        0      313 2023-03-22 22:39:32.000000 acgen_by_den-0.0.4/acgen_by_den/edits/levels/__init__.py
--rw-rw-rw-   0        0        0     1035 2023-03-22 22:39:32.000000 acgen_by_den-0.0.4/acgen_by_den/edits/levels/aku.py
--rw-rw-rw-   0        0        0      491 2023-03-22 22:39:32.000000 acgen_by_den-0.0.4/acgen_by_den/edits/levels/allow_filibuster_clearing.py
--rw-rw-rw-   0        0        0      790 2023-03-22 22:39:32.000000 acgen_by_den-0.0.4/acgen_by_den/edits/levels/behemoth_culling.py
--rw-rw-rw-   0        0        0      646 2023-03-22 22:39:32.000000 acgen_by_den-0.0.4/acgen_by_den/edits/levels/clear_tutorial.py
--rw-rw-rw-   0        0        0     1121 2023-03-22 22:39:32.000000 acgen_by_den-0.0.4/acgen_by_den/edits/levels/enigma_stages.py
--rw-rw-rw-   0        0        0     6307 2023-03-22 22:39:32.000000 acgen_by_den-0.0.4/acgen_by_den/edits/levels/event_stages.py
--rw-rw-rw-   0        0        0     1873 2023-03-22 22:39:32.000000 acgen_by_den-0.0.4/acgen_by_den/edits/levels/gauntlet.py
--rw-rw-rw-   0        0        0     1027 2023-03-22 22:39:32.000000 acgen_by_den-0.0.4/acgen_by_den/edits/levels/itf_timed_scores.py
--rw-rw-rw-   0        0        0     1469 2023-03-22 22:39:32.000000 acgen_by_den-0.0.4/acgen_by_den/edits/levels/legend_quest.py
--rw-rw-rw-   0        0        0     4408 2023-03-22 22:39:32.000000 acgen_by_den-0.0.4/acgen_by_den/edits/levels/main_story.py
--rw-rw-rw-   0        0        0     2323 2023-03-22 22:39:32.000000 acgen_by_den-0.0.4/acgen_by_den/edits/levels/outbreaks.py
--rw-rw-rw-   0        0        0     3031 2023-03-22 22:39:32.000000 acgen_by_den-0.0.4/acgen_by_den/edits/levels/story_level_id_selector.py
--rw-rw-rw-   0        0        0     1175 2023-03-22 22:39:32.000000 acgen_by_den-0.0.4/acgen_by_den/edits/levels/towers.py
--rw-rw-rw-   0        0        0     8458 2023-03-22 22:39:32.000000 acgen_by_den-0.0.4/acgen_by_den/edits/levels/treasures.py
--rw-rw-rw-   0        0        0     1043 2023-03-22 22:39:32.000000 acgen_by_den-0.0.4/acgen_by_den/edits/levels/uncanny.py
--rw-rw-rw-   0        0        0      784 2023-03-22 22:39:32.000000 acgen_by_den-0.0.4/acgen_by_den/edits/levels/unlock_aku_realm.py
-drwxrwxrwx   0        0        0        0 2023-07-27 05:51:47.780636 acgen_by_den-0.0.4/acgen_by_den/edits/other/
--rw-rw-rw-   0        0        0      276 2023-03-22 22:39:32.000000 acgen_by_den-0.0.4/acgen_by_den/edits/other/__init__.py
--rw-rw-rw-   0        0        0     3878 2023-03-22 22:39:32.000000 acgen_by_den-0.0.4/acgen_by_den/edits/other/cat_shrine.py
--rw-rw-rw-   0        0        0     1093 2023-03-22 22:39:32.000000 acgen_by_den-0.0.4/acgen_by_den/edits/other/claim_user_rank_rewards.py
--rw-rw-rw-   0        0        0     1054 2023-03-22 22:39:32.000000 acgen_by_den-0.0.4/acgen_by_den/edits/other/create_new_account.py
--rw-rw-rw-   0        0        0     2187 2023-03-22 22:39:32.000000 acgen_by_den-0.0.4/acgen_by_den/edits/other/fix_elsewhere.py
--rw-rw-rw-   0        0        0      659 2023-03-22 22:39:32.000000 acgen_by_den-0.0.4/acgen_by_den/edits/other/fix_time_issues.py
--rw-rw-rw-   0        0        0     3445 2023-03-22 22:39:32.000000 acgen_by_den-0.0.4/acgen_by_den/edits/other/get_gold_pass.py
--rw-rw-rw-   0        0        0     7067 2023-03-22 22:39:32.000000 acgen_by_den-0.0.4/acgen_by_den/edits/other/meow_medals.py
--rw-rw-rw-   0        0        0     4354 2023-03-22 22:39:32.000000 acgen_by_den-0.0.4/acgen_by_den/edits/other/missions.py
--rw-rw-rw-   0        0        0      975 2023-03-22 22:39:32.000000 acgen_by_den-0.0.4/acgen_by_den/edits/other/play_time.py
--rw-rw-rw-   0        0        0     4568 2023-03-22 22:39:32.000000 acgen_by_den-0.0.4/acgen_by_den/edits/other/scheme_item.py
--rw-rw-rw-   0        0        0     1612 2023-03-22 22:39:32.000000 acgen_by_den-0.0.4/acgen_by_den/edits/other/trade_progress.py
--rw-rw-rw-   0        0        0     1284 2023-03-22 22:39:32.000000 acgen_by_den-0.0.4/acgen_by_den/edits/other/unlock_enemy_guide.py
--rw-rw-rw-   0        0        0      326 2023-03-22 22:39:32.000000 acgen_by_den-0.0.4/acgen_by_den/edits/other/unlock_equip_menu.py
-drwxrwxrwx   0        0        0        0 2023-07-27 05:51:47.816397 acgen_by_den-0.0.4/acgen_by_den/edits/save_management/
--rw-rw-rw-   0        0        0       56 2023-03-22 22:39:32.000000 acgen_by_den-0.0.4/acgen_by_den/edits/save_management/__init__.py
--rw-rw-rw-   0        0        0     1273 2023-03-22 22:39:32.000000 acgen_by_den-0.0.4/acgen_by_den/edits/save_management/convert.py
--rw-rw-rw-   0        0        0     2578 2023-03-22 22:39:32.000000 acgen_by_den-0.0.4/acgen_by_den/edits/save_management/load.py
--rw-rw-rw-   0        0        0      644 2023-03-22 22:39:32.000000 acgen_by_den-0.0.4/acgen_by_den/edits/save_management/other.py
--rw-rw-rw-   0        0        0     2049 2023-03-22 22:39:32.000000 acgen_by_den-0.0.4/acgen_by_den/edits/save_management/save.py
--rw-rw-rw-   0        0        0     1774 2023-07-27 00:48:59.000000 acgen_by_den-0.0.4/acgen_by_den/edits/save_management/server_upload.py
--rw-rw-rw-   0        0        0    12118 2023-04-27 11:52:06.000000 acgen_by_den-0.0.4/acgen_by_den/feature_handler.py
--rw-rw-rw-   0        0        0     4822 2023-04-26 22:37:34.000000 acgen_by_den-0.0.4/acgen_by_den/game_data_getter.py
--rw-rw-rw-   0        0        0    22764 2023-07-27 05:51:29.000000 acgen_by_den-0.0.4/acgen_by_den/helper.py
--rw-rw-rw-   0        0        0     7075 2023-04-27 12:18:12.000000 acgen_by_den-0.0.4/acgen_by_den/item.py
--rw-rw-rw-   0        0        0     3505 2023-03-22 22:39:32.000000 acgen_by_den-0.0.4/acgen_by_den/locale_handler.py
--rw-rw-rw-   0        0        0     1269 2023-03-22 22:39:32.000000 acgen_by_den-0.0.4/acgen_by_den/managed_item.py
--rw-rw-rw-   0        0        0    66964 2023-03-22 22:39:32.000000 acgen_by_den-0.0.4/acgen_by_den/parse_save.py
--rw-rw-rw-   0        0        0     1301 2023-03-22 22:39:32.000000 acgen_by_den-0.0.4/acgen_by_den/patcher.py
--rw-rw-rw-   0        0        0     2415 2023-03-22 22:39:32.000000 acgen_by_den-0.0.4/acgen_by_den/root_handler.py
--rw-rw-rw-   0        0        0    53791 2023-03-22 22:39:32.000000 acgen_by_den-0.0.4/acgen_by_den/serialise_save.py
--rw-rw-rw-   0        0        0    24712 2023-07-27 00:48:25.000000 acgen_by_den-0.0.4/acgen_by_den/server_handler.py
--rw-rw-rw-   0        0        0     3247 2023-07-27 05:19:36.000000 acgen_by_den-0.0.4/acgen_by_den/tracker.py
--rw-rw-rw-   0        0        0     3496 2023-07-27 03:33:58.000000 acgen_by_den-0.0.4/acgen_by_den/updater.py
--rw-rw-rw-   0        0        0     8297 2023-03-22 22:39:32.000000 acgen_by_den-0.0.4/acgen_by_den/user_input_handler.py
-drwxrwxrwx   0        0        0        0 2023-07-27 05:51:47.281983 acgen_by_den-0.0.4/acgen_by_den.egg-info/
--rw-rw-rw-   0        0        0      472 2023-07-27 05:51:46.000000 acgen_by_den-0.0.4/acgen_by_den.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3258 2023-07-27 05:51:46.000000 acgen_by_den-0.0.4/acgen_by_den.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 05:51:46.000000 acgen_by_den-0.0.4/acgen_by_den.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-27 05:51:46.000000 acgen_by_den-0.0.4/acgen_by_den.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       50 2023-07-27 05:51:46.000000 acgen_by_den-0.0.4/acgen_by_den.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-27 05:51:46.000000 acgen_by_den-0.0.4/acgen_by_den.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-27 05:51:47.823353 acgen_by_den-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      804 2023-07-27 05:51:36.000000 acgen_by_den-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 06:34:05.330830 acgen_by_den-0.0.7/
+-rw-rw-rw-   0        0        0      472 2023-07-27 06:34:05.330830 acgen_by_den-0.0.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-27 06:34:04.875461 acgen_by_den-0.0.7/acgen_by_den/
+-rw-rw-rw-   0        0        0      281 2023-03-22 22:39:32.000000 acgen_by_den-0.0.7/acgen_by_den/__init__.py
+-rw-rw-rw-   0        0        0     8327 2023-07-26 23:42:21.000000 acgen_by_den-0.0.7/acgen_by_den/__main__.py
+-rw-rw-rw-   0        0        0    10151 2023-03-22 22:39:32.000000 acgen_by_den-0.0.7/acgen_by_den/adb_handler.py
+-rw-rw-rw-   0        0        0    13745 2023-03-22 22:39:32.000000 acgen_by_den-0.0.7/acgen_by_den/config_manager.py
+-rw-rw-rw-   0        0        0     1501 2023-03-22 22:39:32.000000 acgen_by_den-0.0.7/acgen_by_den/csv_handler.py
+drwxrwxrwx   0        0        0        0 2023-07-27 06:34:04.952943 acgen_by_den-0.0.7/acgen_by_den/edits/
+-rw-rw-rw-   0        0        0       67 2023-03-22 22:39:32.000000 acgen_by_den-0.0.7/acgen_by_den/edits/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-27 06:34:05.017507 acgen_by_den-0.0.7/acgen_by_den/edits/basic/
+-rw-rw-rw-   0        0        0      122 2023-03-22 22:39:32.000000 acgen_by_den-0.0.7/acgen_by_den/edits/basic/__init__.py
+-rw-rw-rw-   0        0        0     8690 2023-03-22 22:39:32.000000 acgen_by_den-0.0.7/acgen_by_den/edits/basic/basic_items.py
+-rw-rw-rw-   0        0        0     1490 2023-03-22 22:39:32.000000 acgen_by_den-0.0.7/acgen_by_den/edits/basic/catfruit.py
+-rw-rw-rw-   0        0        0     1931 2023-03-22 22:39:32.000000 acgen_by_den-0.0.7/acgen_by_den/edits/basic/catseyes.py
+-rw-rw-rw-   0        0        0     1647 2023-03-22 22:39:32.000000 acgen_by_den-0.0.7/acgen_by_den/edits/basic/ototo_base_mats.py
+-rw-rw-rw-   0        0        0     3984 2023-03-22 22:39:32.000000 acgen_by_den-0.0.7/acgen_by_den/edits/basic/talent_orbs.py
+-rw-rw-rw-   0        0        0    16533 2023-03-22 22:39:32.000000 acgen_by_den-0.0.7/acgen_by_den/edits/basic/talent_orbs_new.py
+drwxrwxrwx   0        0        0        0 2023-07-27 06:34:05.094179 acgen_by_den-0.0.7/acgen_by_den/edits/cats/
+-rw-rw-rw-   0        0        0      179 2023-03-22 22:39:32.000000 acgen_by_den-0.0.7/acgen_by_den/edits/cats/__init__.py
+-rw-rw-rw-   0        0        0     8978 2023-03-22 22:39:32.000000 acgen_by_den-0.0.7/acgen_by_den/edits/cats/cat_helper.py
+-rw-rw-rw-   0        0        0    11121 2023-03-22 22:39:32.000000 acgen_by_den-0.0.7/acgen_by_den/edits/cats/cat_id_selector.py
+-rw-rw-rw-   0        0        0     3249 2023-03-22 22:39:32.000000 acgen_by_den-0.0.7/acgen_by_den/edits/cats/chara_drop.py
+-rw-rw-rw-   0        0        0     1068 2023-03-22 22:39:32.000000 acgen_by_den-0.0.7/acgen_by_den/edits/cats/clear_cat_guide.py
+-rw-rw-rw-   0        0        0     2844 2023-03-22 22:39:32.000000 acgen_by_den-0.0.7/acgen_by_den/edits/cats/evolve_cats.py
+-rw-rw-rw-   0        0        0     1260 2023-03-22 22:39:32.000000 acgen_by_den-0.0.7/acgen_by_den/edits/cats/get_remove_cats.py
+-rw-rw-rw-   0        0        0     7936 2023-03-22 22:39:32.000000 acgen_by_den-0.0.7/acgen_by_den/edits/cats/talents.py
+-rw-rw-rw-   0        0        0     1900 2023-03-22 22:39:32.000000 acgen_by_den-0.0.7/acgen_by_den/edits/cats/upgrade_blue.py
+-rw-rw-rw-   0        0        0     4428 2023-03-22 22:39:32.000000 acgen_by_den-0.0.7/acgen_by_den/edits/cats/upgrade_cats.py
+drwxrwxrwx   0        0        0        0 2023-07-27 06:34:05.125422 acgen_by_den-0.0.7/acgen_by_den/edits/gamototo/
+-rw-rw-rw-   0        0        0       66 2023-03-22 22:39:32.000000 acgen_by_den-0.0.7/acgen_by_den/edits/gamototo/__init__.py
+-rw-rw-rw-   0        0        0      309 2023-03-22 22:39:32.000000 acgen_by_den-0.0.7/acgen_by_den/edits/gamototo/fix_gamatoto.py
+-rw-rw-rw-   0        0        0     2794 2023-03-22 22:39:32.000000 acgen_by_den-0.0.7/acgen_by_den/edits/gamototo/gamatoto_xp.py
+-rw-rw-rw-   0        0        0     3393 2023-03-22 22:39:32.000000 acgen_by_den-0.0.7/acgen_by_den/edits/gamototo/helpers.py
+-rw-rw-rw-   0        0        0     4137 2023-03-22 22:39:32.000000 acgen_by_den-0.0.7/acgen_by_den/edits/gamototo/ototo_cat_cannon.py
+drwxrwxrwx   0        0        0        0 2023-07-27 06:34:05.223592 acgen_by_den-0.0.7/acgen_by_den/edits/levels/
+-rw-rw-rw-   0        0        0      313 2023-03-22 22:39:32.000000 acgen_by_den-0.0.7/acgen_by_den/edits/levels/__init__.py
+-rw-rw-rw-   0        0        0     1035 2023-03-22 22:39:32.000000 acgen_by_den-0.0.7/acgen_by_den/edits/levels/aku.py
+-rw-rw-rw-   0        0        0      491 2023-03-22 22:39:32.000000 acgen_by_den-0.0.7/acgen_by_den/edits/levels/allow_filibuster_clearing.py
+-rw-rw-rw-   0        0        0      790 2023-03-22 22:39:32.000000 acgen_by_den-0.0.7/acgen_by_den/edits/levels/behemoth_culling.py
+-rw-rw-rw-   0        0        0      646 2023-03-22 22:39:32.000000 acgen_by_den-0.0.7/acgen_by_den/edits/levels/clear_tutorial.py
+-rw-rw-rw-   0        0        0     1121 2023-03-22 22:39:32.000000 acgen_by_den-0.0.7/acgen_by_den/edits/levels/enigma_stages.py
+-rw-rw-rw-   0        0        0     6307 2023-03-22 22:39:32.000000 acgen_by_den-0.0.7/acgen_by_den/edits/levels/event_stages.py
+-rw-rw-rw-   0        0        0     1873 2023-03-22 22:39:32.000000 acgen_by_den-0.0.7/acgen_by_den/edits/levels/gauntlet.py
+-rw-rw-rw-   0        0        0     1027 2023-03-22 22:39:32.000000 acgen_by_den-0.0.7/acgen_by_den/edits/levels/itf_timed_scores.py
+-rw-rw-rw-   0        0        0     1469 2023-03-22 22:39:32.000000 acgen_by_den-0.0.7/acgen_by_den/edits/levels/legend_quest.py
+-rw-rw-rw-   0        0        0     4408 2023-03-22 22:39:32.000000 acgen_by_den-0.0.7/acgen_by_den/edits/levels/main_story.py
+-rw-rw-rw-   0        0        0     2323 2023-03-22 22:39:32.000000 acgen_by_den-0.0.7/acgen_by_den/edits/levels/outbreaks.py
+-rw-rw-rw-   0        0        0     3031 2023-03-22 22:39:32.000000 acgen_by_den-0.0.7/acgen_by_den/edits/levels/story_level_id_selector.py
+-rw-rw-rw-   0        0        0     1175 2023-03-22 22:39:32.000000 acgen_by_den-0.0.7/acgen_by_den/edits/levels/towers.py
+-rw-rw-rw-   0        0        0     8458 2023-03-22 22:39:32.000000 acgen_by_den-0.0.7/acgen_by_den/edits/levels/treasures.py
+-rw-rw-rw-   0        0        0     1043 2023-03-22 22:39:32.000000 acgen_by_den-0.0.7/acgen_by_den/edits/levels/uncanny.py
+-rw-rw-rw-   0        0        0      784 2023-03-22 22:39:32.000000 acgen_by_den-0.0.7/acgen_by_den/edits/levels/unlock_aku_realm.py
+drwxrwxrwx   0        0        0        0 2023-07-27 06:34:05.297348 acgen_by_den-0.0.7/acgen_by_den/edits/other/
+-rw-rw-rw-   0        0        0      276 2023-03-22 22:39:32.000000 acgen_by_den-0.0.7/acgen_by_den/edits/other/__init__.py
+-rw-rw-rw-   0        0        0     3878 2023-03-22 22:39:32.000000 acgen_by_den-0.0.7/acgen_by_den/edits/other/cat_shrine.py
+-rw-rw-rw-   0        0        0     1093 2023-03-22 22:39:32.000000 acgen_by_den-0.0.7/acgen_by_den/edits/other/claim_user_rank_rewards.py
+-rw-rw-rw-   0        0        0     1054 2023-03-22 22:39:32.000000 acgen_by_den-0.0.7/acgen_by_den/edits/other/create_new_account.py
+-rw-rw-rw-   0        0        0     2187 2023-03-22 22:39:32.000000 acgen_by_den-0.0.7/acgen_by_den/edits/other/fix_elsewhere.py
+-rw-rw-rw-   0        0        0      659 2023-03-22 22:39:32.000000 acgen_by_den-0.0.7/acgen_by_den/edits/other/fix_time_issues.py
+-rw-rw-rw-   0        0        0     3445 2023-03-22 22:39:32.000000 acgen_by_den-0.0.7/acgen_by_den/edits/other/get_gold_pass.py
+-rw-rw-rw-   0        0        0     7067 2023-03-22 22:39:32.000000 acgen_by_den-0.0.7/acgen_by_den/edits/other/meow_medals.py
+-rw-rw-rw-   0        0        0     4354 2023-03-22 22:39:32.000000 acgen_by_den-0.0.7/acgen_by_den/edits/other/missions.py
+-rw-rw-rw-   0        0        0      975 2023-03-22 22:39:32.000000 acgen_by_den-0.0.7/acgen_by_den/edits/other/play_time.py
+-rw-rw-rw-   0        0        0     4568 2023-03-22 22:39:32.000000 acgen_by_den-0.0.7/acgen_by_den/edits/other/scheme_item.py
+-rw-rw-rw-   0        0        0     1612 2023-03-22 22:39:32.000000 acgen_by_den-0.0.7/acgen_by_den/edits/other/trade_progress.py
+-rw-rw-rw-   0        0        0     1284 2023-03-22 22:39:32.000000 acgen_by_den-0.0.7/acgen_by_den/edits/other/unlock_enemy_guide.py
+-rw-rw-rw-   0        0        0      326 2023-03-22 22:39:32.000000 acgen_by_den-0.0.7/acgen_by_den/edits/other/unlock_equip_menu.py
+drwxrwxrwx   0        0        0        0 2023-07-27 06:34:05.325940 acgen_by_den-0.0.7/acgen_by_den/edits/save_management/
+-rw-rw-rw-   0        0        0       56 2023-03-22 22:39:32.000000 acgen_by_den-0.0.7/acgen_by_den/edits/save_management/__init__.py
+-rw-rw-rw-   0        0        0     1273 2023-03-22 22:39:32.000000 acgen_by_den-0.0.7/acgen_by_den/edits/save_management/convert.py
+-rw-rw-rw-   0        0        0     2578 2023-03-22 22:39:32.000000 acgen_by_den-0.0.7/acgen_by_den/edits/save_management/load.py
+-rw-rw-rw-   0        0        0      644 2023-03-22 22:39:32.000000 acgen_by_den-0.0.7/acgen_by_den/edits/save_management/other.py
+-rw-rw-rw-   0        0        0     2049 2023-03-22 22:39:32.000000 acgen_by_den-0.0.7/acgen_by_den/edits/save_management/save.py
+-rw-rw-rw-   0        0        0     1774 2023-07-27 00:48:59.000000 acgen_by_den-0.0.7/acgen_by_den/edits/save_management/server_upload.py
+-rw-rw-rw-   0        0        0    12118 2023-04-27 11:52:06.000000 acgen_by_den-0.0.7/acgen_by_den/feature_handler.py
+-rw-rw-rw-   0        0        0     4822 2023-04-26 22:37:34.000000 acgen_by_den-0.0.7/acgen_by_den/game_data_getter.py
+-rw-rw-rw-   0        0        0    22446 2023-07-27 05:56:11.000000 acgen_by_den-0.0.7/acgen_by_den/helper.py
+-rw-rw-rw-   0        0        0     7075 2023-04-27 12:18:12.000000 acgen_by_den-0.0.7/acgen_by_den/item.py
+-rw-rw-rw-   0        0        0     3505 2023-03-22 22:39:32.000000 acgen_by_den-0.0.7/acgen_by_den/locale_handler.py
+-rw-rw-rw-   0        0        0     1269 2023-03-22 22:39:32.000000 acgen_by_den-0.0.7/acgen_by_den/managed_item.py
+-rw-rw-rw-   0        0        0    66964 2023-03-22 22:39:32.000000 acgen_by_den-0.0.7/acgen_by_den/parse_save.py
+-rw-rw-rw-   0        0        0     1301 2023-03-22 22:39:32.000000 acgen_by_den-0.0.7/acgen_by_den/patcher.py
+-rw-rw-rw-   0        0        0     2415 2023-03-22 22:39:32.000000 acgen_by_den-0.0.7/acgen_by_den/root_handler.py
+-rw-rw-rw-   0        0        0    53791 2023-03-22 22:39:32.000000 acgen_by_den-0.0.7/acgen_by_den/serialise_save.py
+-rw-rw-rw-   0        0        0    24712 2023-07-27 00:48:25.000000 acgen_by_den-0.0.7/acgen_by_den/server_handler.py
+-rw-rw-rw-   0        0        0     3247 2023-07-27 05:19:36.000000 acgen_by_den-0.0.7/acgen_by_den/tracker.py
+-rw-rw-rw-   0        0        0     3496 2023-07-27 03:33:58.000000 acgen_by_den-0.0.7/acgen_by_den/updater.py
+-rw-rw-rw-   0        0        0     8297 2023-03-22 22:39:32.000000 acgen_by_den-0.0.7/acgen_by_den/user_input_handler.py
+drwxrwxrwx   0        0        0        0 2023-07-27 06:34:04.948968 acgen_by_den-0.0.7/acgen_by_den.egg-info/
+-rw-rw-rw-   0        0        0      472 2023-07-27 06:34:04.000000 acgen_by_den-0.0.7/acgen_by_den.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3258 2023-07-27 06:34:04.000000 acgen_by_den-0.0.7/acgen_by_den.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 06:34:04.000000 acgen_by_den-0.0.7/acgen_by_den.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-27 06:34:04.000000 acgen_by_den-0.0.7/acgen_by_den.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       50 2023-07-27 06:34:04.000000 acgen_by_den-0.0.7/acgen_by_den.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-27 06:34:04.000000 acgen_by_den-0.0.7/acgen_by_den.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-27 06:34:05.334550 acgen_by_den-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      804 2023-07-27 06:33:59.000000 acgen_by_den-0.0.7/setup.py
```

### Comparing `acgen_by_den-0.0.4/acgen_by_den/__main__.py` & `acgen_by_den-0.0.7/acgen_by_den/__main__.py`

 * *Files identical despite different names*

### Comparing `acgen_by_den-0.0.4/acgen_by_den/adb_handler.py` & `acgen_by_den-0.0.7/acgen_by_den/adb_handler.py`

 * *Files identical despite different names*

### Comparing `acgen_by_den-0.0.4/acgen_by_den/config_manager.py` & `acgen_by_den-0.0.7/acgen_by_den/config_manager.py`

 * *Files identical despite different names*

### Comparing `acgen_by_den-0.0.4/acgen_by_den/csv_handler.py` & `acgen_by_den-0.0.7/acgen_by_den/csv_handler.py`

 * *Files identical despite different names*

### Comparing `acgen_by_den-0.0.4/acgen_by_den/edits/basic/basic_items.py` & `acgen_by_den-0.0.7/acgen_by_den/edits/basic/basic_items.py`

 * *Files identical despite different names*

### Comparing `acgen_by_den-0.0.4/acgen_by_den/edits/basic/catfruit.py` & `acgen_by_den-0.0.7/acgen_by_den/edits/basic/catfruit.py`

 * *Files identical despite different names*

### Comparing `acgen_by_den-0.0.4/acgen_by_den/edits/basic/catseyes.py` & `acgen_by_den-0.0.7/acgen_by_den/edits/basic/catseyes.py`

 * *Files identical despite different names*

### Comparing `acgen_by_den-0.0.4/acgen_by_den/edits/basic/ototo_base_mats.py` & `acgen_by_den-0.0.7/acgen_by_den/edits/basic/ototo_base_mats.py`

 * *Files identical despite different names*

### Comparing `acgen_by_den-0.0.4/acgen_by_den/edits/basic/talent_orbs.py` & `acgen_by_den-0.0.7/acgen_by_den/edits/basic/talent_orbs.py`

 * *Files identical despite different names*

### Comparing `acgen_by_den-0.0.4/acgen_by_den/edits/basic/talent_orbs_new.py` & `acgen_by_den-0.0.7/acgen_by_den/edits/basic/talent_orbs_new.py`

 * *Files identical despite different names*

### Comparing `acgen_by_den-0.0.4/acgen_by_den/edits/cats/cat_helper.py` & `acgen_by_den-0.0.7/acgen_by_den/edits/cats/cat_helper.py`

 * *Files identical despite different names*

### Comparing `acgen_by_den-0.0.4/acgen_by_den/edits/cats/cat_id_selector.py` & `acgen_by_den-0.0.7/acgen_by_den/edits/cats/cat_id_selector.py`

 * *Files identical despite different names*

### Comparing `acgen_by_den-0.0.4/acgen_by_den/edits/cats/chara_drop.py` & `acgen_by_den-0.0.7/acgen_by_den/edits/cats/chara_drop.py`

 * *Files identical despite different names*

### Comparing `acgen_by_den-0.0.4/acgen_by_den/edits/cats/clear_cat_guide.py` & `acgen_by_den-0.0.7/acgen_by_den/edits/cats/clear_cat_guide.py`

 * *Files identical despite different names*

### Comparing `acgen_by_den-0.0.4/acgen_by_den/edits/cats/evolve_cats.py` & `acgen_by_den-0.0.7/acgen_by_den/edits/cats/evolve_cats.py`

 * *Files identical despite different names*

### Comparing `acgen_by_den-0.0.4/acgen_by_den/edits/cats/get_remove_cats.py` & `acgen_by_den-0.0.7/acgen_by_den/edits/cats/get_remove_cats.py`

 * *Files identical despite different names*

### Comparing `acgen_by_den-0.0.4/acgen_by_den/edits/cats/talents.py` & `acgen_by_den-0.0.7/acgen_by_den/edits/cats/talents.py`

 * *Files identical despite different names*

### Comparing `acgen_by_den-0.0.4/acgen_by_den/edits/cats/upgrade_blue.py` & `acgen_by_den-0.0.7/acgen_by_den/edits/cats/upgrade_blue.py`

 * *Files identical despite different names*

### Comparing `acgen_by_den-0.0.4/acgen_by_den/edits/cats/upgrade_cats.py` & `acgen_by_den-0.0.7/acgen_by_den/edits/cats/upgrade_cats.py`

 * *Files identical despite different names*

### Comparing `acgen_by_den-0.0.4/acgen_by_den/edits/gamototo/gamatoto_xp.py` & `acgen_by_den-0.0.7/acgen_by_den/edits/gamototo/gamatoto_xp.py`

 * *Files identical despite different names*

### Comparing `acgen_by_den-0.0.4/acgen_by_den/edits/gamototo/helpers.py` & `acgen_by_den-0.0.7/acgen_by_den/edits/gamototo/helpers.py`

 * *Files identical despite different names*

### Comparing `acgen_by_den-0.0.4/acgen_by_den/edits/gamototo/ototo_cat_cannon.py` & `acgen_by_den-0.0.7/acgen_by_den/edits/gamototo/ototo_cat_cannon.py`

 * *Files identical despite different names*

### Comparing `acgen_by_den-0.0.4/acgen_by_den/edits/levels/aku.py` & `acgen_by_den-0.0.7/acgen_by_den/edits/levels/aku.py`

 * *Files identical despite different names*

### Comparing `acgen_by_den-0.0.4/acgen_by_den/edits/levels/behemoth_culling.py` & `acgen_by_den-0.0.7/acgen_by_den/edits/levels/behemoth_culling.py`

 * *Files identical despite different names*

### Comparing `acgen_by_den-0.0.4/acgen_by_den/edits/levels/clear_tutorial.py` & `acgen_by_den-0.0.7/acgen_by_den/edits/levels/clear_tutorial.py`

 * *Files identical despite different names*

### Comparing `acgen_by_den-0.0.4/acgen_by_den/edits/levels/enigma_stages.py` & `acgen_by_den-0.0.7/acgen_by_den/edits/levels/enigma_stages.py`

 * *Files identical despite different names*

### Comparing `acgen_by_den-0.0.4/acgen_by_den/edits/levels/event_stages.py` & `acgen_by_den-0.0.7/acgen_by_den/edits/levels/event_stages.py`

 * *Files identical despite different names*

### Comparing `acgen_by_den-0.0.4/acgen_by_den/edits/levels/gauntlet.py` & `acgen_by_den-0.0.7/acgen_by_den/edits/levels/gauntlet.py`

 * *Files identical despite different names*

### Comparing `acgen_by_den-0.0.4/acgen_by_den/edits/levels/itf_timed_scores.py` & `acgen_by_den-0.0.7/acgen_by_den/edits/levels/itf_timed_scores.py`

 * *Files identical despite different names*

### Comparing `acgen_by_den-0.0.4/acgen_by_den/edits/levels/legend_quest.py` & `acgen_by_den-0.0.7/acgen_by_den/edits/levels/legend_quest.py`

 * *Files identical despite different names*

### Comparing `acgen_by_den-0.0.4/acgen_by_den/edits/levels/main_story.py` & `acgen_by_den-0.0.7/acgen_by_den/edits/levels/main_story.py`

 * *Files identical despite different names*

### Comparing `acgen_by_den-0.0.4/acgen_by_den/edits/levels/outbreaks.py` & `acgen_by_den-0.0.7/acgen_by_den/edits/levels/outbreaks.py`

 * *Files identical despite different names*

### Comparing `acgen_by_den-0.0.4/acgen_by_den/edits/levels/story_level_id_selector.py` & `acgen_by_den-0.0.7/acgen_by_den/edits/levels/story_level_id_selector.py`

 * *Files identical despite different names*

### Comparing `acgen_by_den-0.0.4/acgen_by_den/edits/levels/towers.py` & `acgen_by_den-0.0.7/acgen_by_den/edits/levels/towers.py`

 * *Files identical despite different names*

### Comparing `acgen_by_den-0.0.4/acgen_by_den/edits/levels/treasures.py` & `acgen_by_den-0.0.7/acgen_by_den/edits/levels/treasures.py`

 * *Files identical despite different names*

### Comparing `acgen_by_den-0.0.4/acgen_by_den/edits/levels/uncanny.py` & `acgen_by_den-0.0.7/acgen_by_den/edits/levels/uncanny.py`

 * *Files identical despite different names*

### Comparing `acgen_by_den-0.0.4/acgen_by_den/edits/levels/unlock_aku_realm.py` & `acgen_by_den-0.0.7/acgen_by_den/edits/levels/unlock_aku_realm.py`

 * *Files identical despite different names*

### Comparing `acgen_by_den-0.0.4/acgen_by_den/edits/other/cat_shrine.py` & `acgen_by_den-0.0.7/acgen_by_den/edits/other/cat_shrine.py`

 * *Files identical despite different names*

### Comparing `acgen_by_den-0.0.4/acgen_by_den/edits/other/claim_user_rank_rewards.py` & `acgen_by_den-0.0.7/acgen_by_den/edits/other/claim_user_rank_rewards.py`

 * *Files identical despite different names*

### Comparing `acgen_by_den-0.0.4/acgen_by_den/edits/other/create_new_account.py` & `acgen_by_den-0.0.7/acgen_by_den/edits/other/create_new_account.py`

 * *Files identical despite different names*

### Comparing `acgen_by_den-0.0.4/acgen_by_den/edits/other/fix_elsewhere.py` & `acgen_by_den-0.0.7/acgen_by_den/edits/other/fix_elsewhere.py`

 * *Files identical despite different names*

### Comparing `acgen_by_den-0.0.4/acgen_by_den/edits/other/fix_time_issues.py` & `acgen_by_den-0.0.7/acgen_by_den/edits/other/fix_time_issues.py`

 * *Files identical despite different names*

### Comparing `acgen_by_den-0.0.4/acgen_by_den/edits/other/get_gold_pass.py` & `acgen_by_den-0.0.7/acgen_by_den/edits/other/get_gold_pass.py`

 * *Files identical despite different names*

### Comparing `acgen_by_den-0.0.4/acgen_by_den/edits/other/meow_medals.py` & `acgen_by_den-0.0.7/acgen_by_den/edits/other/meow_medals.py`

 * *Files identical despite different names*

### Comparing `acgen_by_den-0.0.4/acgen_by_den/edits/other/missions.py` & `acgen_by_den-0.0.7/acgen_by_den/edits/other/missions.py`

 * *Files identical despite different names*

### Comparing `acgen_by_den-0.0.4/acgen_by_den/edits/other/play_time.py` & `acgen_by_den-0.0.7/acgen_by_den/edits/other/play_time.py`

 * *Files identical despite different names*

### Comparing `acgen_by_den-0.0.4/acgen_by_den/edits/other/scheme_item.py` & `acgen_by_den-0.0.7/acgen_by_den/edits/other/scheme_item.py`

 * *Files identical despite different names*

### Comparing `acgen_by_den-0.0.4/acgen_by_den/edits/other/trade_progress.py` & `acgen_by_den-0.0.7/acgen_by_den/edits/other/trade_progress.py`

 * *Files identical despite different names*

### Comparing `acgen_by_den-0.0.4/acgen_by_den/edits/other/unlock_enemy_guide.py` & `acgen_by_den-0.0.7/acgen_by_den/edits/other/unlock_enemy_guide.py`

 * *Files identical despite different names*

### Comparing `acgen_by_den-0.0.4/acgen_by_den/edits/save_management/convert.py` & `acgen_by_den-0.0.7/acgen_by_den/edits/save_management/convert.py`

 * *Files identical despite different names*

### Comparing `acgen_by_den-0.0.4/acgen_by_den/edits/save_management/load.py` & `acgen_by_den-0.0.7/acgen_by_den/edits/save_management/load.py`

 * *Files identical despite different names*

### Comparing `acgen_by_den-0.0.4/acgen_by_den/edits/save_management/other.py` & `acgen_by_den-0.0.7/acgen_by_den/edits/save_management/other.py`

 * *Files identical despite different names*

### Comparing `acgen_by_den-0.0.4/acgen_by_den/edits/save_management/save.py` & `acgen_by_den-0.0.7/acgen_by_den/edits/save_management/save.py`

 * *Files identical despite different names*

### Comparing `acgen_by_den-0.0.4/acgen_by_den/edits/save_management/server_upload.py` & `acgen_by_den-0.0.7/acgen_by_den/edits/save_management/server_upload.py`

 * *Files identical despite different names*

### Comparing `acgen_by_den-0.0.4/acgen_by_den/feature_handler.py` & `acgen_by_den-0.0.7/acgen_by_den/feature_handler.py`

 * *Files identical despite different names*

### Comparing `acgen_by_den-0.0.4/acgen_by_den/game_data_getter.py` & `acgen_by_den-0.0.7/acgen_by_den/game_data_getter.py`

 * *Files identical despite different names*

### Comparing `acgen_by_den-0.0.4/acgen_by_den/helper.py` & `acgen_by_den-0.0.7/acgen_by_den/helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,23 +126,15 @@
     dir_path = os.path.join(os.path.dirname(os.path.realpath(__file__)), "files")
     return dir_path
 
 
 def read_file_string(file_path: str) -> str:
     """Reads a file and returns its contents as a string"""
 
-    try:
-        with open(file_path, "r", encoding="utf-8") as file:
-            return file.read()
-    except FileNotFoundError as err:
-        raise Exception("File not found: " + file_path) from err
-    except UnicodeDecodeError as err:
-        raise Exception("Error reading file: " + file_path + ": " + str(err)) from err
-
-
+    print()
 def chunks(lst: list[Any], chunk_len: int) -> Generator[Any, Any, Any]:
     """Split list into chunks of n"""
 
     for i in range(0, len(lst), chunk_len):
         yield lst[i : i + chunk_len]
```

### Comparing `acgen_by_den-0.0.4/acgen_by_den/item.py` & `acgen_by_den-0.0.7/acgen_by_den/item.py`

 * *Files identical despite different names*

### Comparing `acgen_by_den-0.0.4/acgen_by_den/locale_handler.py` & `acgen_by_den-0.0.7/acgen_by_den/locale_handler.py`

 * *Files identical despite different names*

### Comparing `acgen_by_den-0.0.4/acgen_by_den/managed_item.py` & `acgen_by_den-0.0.7/acgen_by_den/managed_item.py`

 * *Files identical despite different names*

### Comparing `acgen_by_den-0.0.4/acgen_by_den/parse_save.py` & `acgen_by_den-0.0.7/acgen_by_den/parse_save.py`

 * *Files identical despite different names*

### Comparing `acgen_by_den-0.0.4/acgen_by_den/patcher.py` & `acgen_by_den-0.0.7/acgen_by_den/patcher.py`

 * *Files identical despite different names*

### Comparing `acgen_by_den-0.0.4/acgen_by_den/root_handler.py` & `acgen_by_den-0.0.7/acgen_by_den/root_handler.py`

 * *Files identical despite different names*

### Comparing `acgen_by_den-0.0.4/acgen_by_den/serialise_save.py` & `acgen_by_den-0.0.7/acgen_by_den/serialise_save.py`

 * *Files identical despite different names*

### Comparing `acgen_by_den-0.0.4/acgen_by_den/server_handler.py` & `acgen_by_den-0.0.7/acgen_by_den/server_handler.py`

 * *Files identical despite different names*

### Comparing `acgen_by_den-0.0.4/acgen_by_den/tracker.py` & `acgen_by_den-0.0.7/acgen_by_den/tracker.py`

 * *Files identical despite different names*

### Comparing `acgen_by_den-0.0.4/acgen_by_den/updater.py` & `acgen_by_den-0.0.7/acgen_by_den/updater.py`

 * *Files identical despite different names*

### Comparing `acgen_by_den-0.0.4/acgen_by_den/user_input_handler.py` & `acgen_by_den-0.0.7/acgen_by_den/user_input_handler.py`

 * *Files identical despite different names*

### Comparing `acgen_by_den-0.0.4/acgen_by_den.egg-info/SOURCES.txt` & `acgen_by_den-0.0.7/acgen_by_den.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `acgen_by_den-0.0.4/setup.py` & `acgen_by_den-0.0.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='acgen_by_den',
-    version='0.0.4',
+    version='0.0.7',
     description='This is a project developed by Serem for development purposes',
     author='serem',
     author_email='gangh9230@gmail.com',
     url='https://github.com/hayul0629/wdex',
     install_requires=[
         "colored==1.4.4",
         "tk",
```

