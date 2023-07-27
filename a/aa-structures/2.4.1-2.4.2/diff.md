# Comparing `tmp/aa_structures-2.4.1.tar.gz` & `tmp/aa_structures-2.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aa_structures-2.4.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "aa_structures-2.4.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aa_structures-2.4.1.tar` & `aa_structures-2.4.2.tar`

### file list

```diff
@@ -1,174 +1,172 @@
--rw-r--r--   0        0        0     1070 2023-06-28 11:50:10.152553 aa_structures-2.4.1/LICENSE
--rw-r--r--   0        0        0     4406 2023-06-28 11:50:10.156553 aa_structures-2.4.1/README.md
--rw-r--r--   0        0        0     2069 2023-06-28 11:50:10.156553 aa_structures-2.4.1/pyproject.toml
--rw-r--r--   0        0        0      170 2023-06-29 12:35:51.837332 aa_structures-2.4.1/structures/__init__.py
--rw-r--r--   0        0        0    36110 2023-06-28 11:50:10.160553 aa_structures-2.4.1/structures/admin.py
--rw-r--r--   0        0        0     6228 2023-06-28 11:50:10.160553 aa_structures-2.4.1/structures/app_settings.py
--rw-r--r--   0        0        0      268 2023-06-28 11:50:10.160553 aa_structures-2.4.1/structures/apps.py
--rw-r--r--   0        0        0      915 2023-06-28 11:50:10.160553 aa_structures-2.4.1/structures/auth_hooks.py
--rw-r--r--   0        0        0     1232 2023-06-28 11:50:10.160553 aa_structures-2.4.1/structures/checks.py
--rw-r--r--   0        0        0      741 2023-06-28 11:50:10.160553 aa_structures-2.4.1/structures/constants.py
--rw-r--r--   0        0        0        0 2023-06-29 12:58:08.028016 aa_structures-2.4.1/structures/core/__init__.py
--rw-r--r--   0        0        0    71519 2023-06-28 11:50:10.160553 aa_structures-2.4.1/structures/core/notification_embeds.py
--rw-r--r--   0        0        0    16436 2023-06-28 11:50:10.160553 aa_structures-2.4.1/structures/core/notification_timers.py
--rw-r--r--   0        0        0    19834 2023-06-28 11:50:10.160553 aa_structures-2.4.1/structures/core/serializers.py
--rw-r--r--   0        0        0      623 2023-06-28 11:50:10.160553 aa_structures-2.4.1/structures/core/sovereignty.py
--rw-r--r--   0        0        0     1613 2023-06-28 11:50:10.160553 aa_structures-2.4.1/structures/core/starbases.py
--rw-r--r--   0        0        0      382 2023-06-28 11:50:10.160553 aa_structures-2.4.1/structures/forms.py
--rw-r--r--   0        0        0        0 2023-06-29 12:58:08.028016 aa_structures-2.4.1/structures/helpers/__init__.py
--rw-r--r--   0        0        0      830 2023-06-28 11:50:10.160553 aa_structures-2.4.1/structures/helpers/general.py
--rw-r--r--   0        0        0    13634 2023-06-28 11:50:10.160553 aa_structures-2.4.1/structures/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    61204 2023-06-28 11:50:10.160553 aa_structures-2.4.1/structures/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    47227 2023-06-28 11:50:10.160553 aa_structures-2.4.1/structures/locale/django.pot
--rw-r--r--   0        0        0      380 2023-06-28 11:50:10.160553 aa_structures-2.4.1/structures/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    47274 2023-06-28 11:50:10.160553 aa_structures-2.4.1/structures/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     5784 2023-06-28 11:50:10.160553 aa_structures-2.4.1/structures/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    55691 2023-06-28 11:50:10.160553 aa_structures-2.4.1/structures/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    47227 2023-06-28 11:50:10.160553 aa_structures-2.4.1/structures/locale/fr_FR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    47227 2023-06-28 11:50:10.160553 aa_structures-2.4.1/structures/locale/it_IT/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    47267 2023-06-28 11:50:10.160553 aa_structures-2.4.1/structures/locale/ja/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      391 2023-06-28 11:50:10.164553 aa_structures-2.4.1/structures/locale/ko/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    47024 2023-06-28 11:50:10.164553 aa_structures-2.4.1/structures/locale/ko/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    47227 2023-06-28 11:50:10.164553 aa_structures-2.4.1/structures/locale/ko_KR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      538 2023-06-28 11:50:10.164553 aa_structures-2.4.1/structures/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    47437 2023-06-28 11:50:10.164553 aa_structures-2.4.1/structures/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    47505 2023-06-28 11:50:10.164553 aa_structures-2.4.1/structures/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    11588 2023-06-28 11:50:10.164553 aa_structures-2.4.1/structures/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    58962 2023-06-28 11:50:10.164553 aa_structures-2.4.1/structures/locale/zh_Hans/LC_MESSAGES/django.po
--rw-r--r--   0        0        0        0 2023-06-29 12:58:08.028016 aa_structures-2.4.1/structures/management/commands/__init__.py
--rw-r--r--   0        0        0     1443 2023-06-28 11:50:10.164553 aa_structures-2.4.1/structures/management/commands/structures_load_eve.py
--rw-r--r--   0        0        0     2398 2023-06-28 11:50:10.164553 aa_structures-2.4.1/structures/management/commands/structures_preload_eveuniverse.py
--rw-r--r--   0        0        0    18114 2023-06-29 12:35:51.837332 aa_structures-2.4.1/structures/managers.py
--rw-r--r--   0        0        0    59315 2023-06-28 11:50:10.164553 aa_structures-2.4.1/structures/migrations/0001_initial_new.py
--rw-r--r--   0        0        0     2274 2023-06-28 11:50:10.164553 aa_structures-2.4.1/structures/migrations/0002_remove_eveuniverse_relation_names.py
--rw-r--r--   0        0        0    44042 2023-06-28 11:50:10.164553 aa_structures-2.4.1/structures/migrations/0003_add_localization_and_unique_key.py
--rw-r--r--   0        0        0        0 2023-06-29 12:58:08.028016 aa_structures-2.4.1/structures/migrations/__init__.py
--rw-r--r--   0        0        0      505 2023-06-28 11:50:10.164553 aa_structures-2.4.1/structures/models/__init__.py
--rw-r--r--   0        0        0     2073 2023-06-28 11:50:10.164553 aa_structures-2.4.1/structures/models/eveuniverse.py
--rw-r--r--   0        0        0    42745 2023-06-28 11:50:10.164553 aa_structures-2.4.1/structures/models/notifications.py
--rw-r--r--   0        0        0    53967 2023-06-28 11:50:10.164553 aa_structures-2.4.1/structures/models/owners.py
--rw-r--r--   0        0        0    37256 2023-06-28 11:50:10.164553 aa_structures-2.4.1/structures/models/structures.py
--rw-r--r--   0        0        0      274 2023-06-28 11:50:10.164553 aa_structures-2.4.1/structures/providers.py
--rw-r--r--   0        0        0     1165 2023-06-28 11:50:10.164553 aa_structures-2.4.1/structures/static/structures/css/global.css
--rw-r--r--   0        0        0     1186 2023-06-28 11:50:10.164553 aa_structures-2.4.1/structures/static/structures/css/main.css
--rw-r--r--   0        0        0    43262 2023-06-28 11:50:10.168552 aa_structures-2.4.1/structures/static/structures/img/Spinner-1s-64px-dark.gif
--rw-r--r--   0        0        0    43381 2023-06-28 11:50:10.168552 aa_structures-2.4.1/structures/static/structures/img/Spinner-1s-64px-light.gif
--rw-r--r--   0        0        0      908 2023-06-28 11:50:10.168552 aa_structures-2.4.1/structures/static/structures/img/eve_symbol_128.png
--rw-r--r--   0        0        0      805 2023-06-28 11:50:10.168552 aa_structures-2.4.1/structures/static/structures/img/panel/0h.png
--rw-r--r--   0        0        0      805 2023-06-28 11:50:10.168552 aa_structures-2.4.1/structures/static/structures/img/panel/0l.png
--rw-r--r--   0        0        0      805 2023-06-28 11:50:10.168552 aa_structures-2.4.1/structures/static/structures/img/panel/0m.png
--rw-r--r--   0        0        0      805 2023-06-28 11:50:10.168552 aa_structures-2.4.1/structures/static/structures/img/panel/0r.png
--rw-r--r--   0        0        0      805 2023-06-28 11:50:10.168552 aa_structures-2.4.1/structures/static/structures/img/panel/0s.png
--rw-r--r--   0        0        0     2590 2023-06-28 11:50:10.168552 aa_structures-2.4.1/structures/static/structures/img/panel/1h.png
--rw-r--r--   0        0        0     1976 2023-06-28 11:50:10.168552 aa_structures-2.4.1/structures/static/structures/img/panel/1l.png
--rw-r--r--   0        0        0     2025 2023-06-28 11:50:10.168552 aa_structures-2.4.1/structures/static/structures/img/panel/1m.png
--rw-r--r--   0        0        0     2512 2023-06-28 11:50:10.168552 aa_structures-2.4.1/structures/static/structures/img/panel/1r.png
--rw-r--r--   0        0        0     3541 2023-06-28 11:50:10.168552 aa_structures-2.4.1/structures/static/structures/img/panel/2h.png
--rw-r--r--   0        0        0     2570 2023-06-28 11:50:10.168552 aa_structures-2.4.1/structures/static/structures/img/panel/2l.png
--rw-r--r--   0        0        0     2766 2023-06-28 11:50:10.168552 aa_structures-2.4.1/structures/static/structures/img/panel/2m.png
--rw-r--r--   0        0        0     3497 2023-06-28 11:50:10.168552 aa_structures-2.4.1/structures/static/structures/img/panel/2r.png
--rw-r--r--   0        0        0     4607 2023-06-28 11:50:10.168552 aa_structures-2.4.1/structures/static/structures/img/panel/3h.png
--rw-r--r--   0        0        0     3523 2023-06-28 11:50:10.168552 aa_structures-2.4.1/structures/static/structures/img/panel/3l.png
--rw-r--r--   0        0        0     3720 2023-06-28 11:50:10.168552 aa_structures-2.4.1/structures/static/structures/img/panel/3m.png
--rw-r--r--   0        0        0     4886 2023-06-28 11:50:10.168552 aa_structures-2.4.1/structures/static/structures/img/panel/3r.png
--rw-r--r--   0        0        0     5309 2023-06-28 11:50:10.168552 aa_structures-2.4.1/structures/static/structures/img/panel/4h.png
--rw-r--r--   0        0        0     4628 2023-06-28 11:50:10.168552 aa_structures-2.4.1/structures/static/structures/img/panel/4l.png
--rw-r--r--   0        0        0     4956 2023-06-28 11:50:10.168552 aa_structures-2.4.1/structures/static/structures/img/panel/4m.png
--rw-r--r--   0        0        0     9490 2023-06-28 11:50:10.168552 aa_structures-2.4.1/structures/static/structures/img/panel/4s.png
--rw-r--r--   0        0        0     6109 2023-06-28 11:50:10.168552 aa_structures-2.4.1/structures/static/structures/img/panel/5h.png
--rw-r--r--   0        0        0     5888 2023-06-28 11:50:10.168552 aa_structures-2.4.1/structures/static/structures/img/panel/5l.png
--rw-r--r--   0        0        0     6270 2023-06-28 11:50:10.168552 aa_structures-2.4.1/structures/static/structures/img/panel/5m.png
--rw-r--r--   0        0        0     7399 2023-06-28 11:50:10.168552 aa_structures-2.4.1/structures/static/structures/img/panel/5s.png
--rw-r--r--   0        0        0     7203 2023-06-28 11:50:10.168552 aa_structures-2.4.1/structures/static/structures/img/panel/6h.png
--rw-r--r--   0        0        0     7014 2023-06-28 11:50:10.168552 aa_structures-2.4.1/structures/static/structures/img/panel/6l.png
--rw-r--r--   0        0        0     7439 2023-06-28 11:50:10.168552 aa_structures-2.4.1/structures/static/structures/img/panel/6m.png
--rw-r--r--   0        0        0     8288 2023-06-28 11:50:10.168552 aa_structures-2.4.1/structures/static/structures/img/panel/7h.png
--rw-r--r--   0        0        0     8067 2023-06-28 11:50:10.168552 aa_structures-2.4.1/structures/static/structures/img/panel/7l.png
--rw-r--r--   0        0        0     8580 2023-06-28 11:50:10.168552 aa_structures-2.4.1/structures/static/structures/img/panel/7m.png
--rw-r--r--   0        0        0     9276 2023-06-28 11:50:10.168552 aa_structures-2.4.1/structures/static/structures/img/panel/8h.png
--rw-r--r--   0        0        0     8972 2023-06-28 11:50:10.168552 aa_structures-2.4.1/structures/static/structures/img/panel/8l.png
--rw-r--r--   0        0        0     9541 2023-06-28 11:50:10.168552 aa_structures-2.4.1/structures/static/structures/img/panel/8m.png
--rw-r--r--   0        0        0      195 2023-06-28 11:50:10.168552 aa_structures-2.4.1/structures/static/structures/img/panel/blank.png
--rw-r--r--   0        0        0    16840 2023-06-28 11:50:10.168552 aa_structures-2.4.1/structures/static/structures/img/panel/circle.png
--rw-r--r--   0        0        0    33523 2023-06-28 11:50:10.172552 aa_structures-2.4.1/structures/static/structures/img/panel/dustwheel.png
--rw-r--r--   0        0        0     1480 2023-06-28 11:50:10.172552 aa_structures-2.4.1/structures/static/structures/img/panel/h.png
--rw-r--r--   0        0        0     1480 2023-06-28 11:50:10.172552 aa_structures-2.4.1/structures/static/structures/img/panel/l.png
--rw-r--r--   0        0        0     1480 2023-06-28 11:50:10.172552 aa_structures-2.4.1/structures/static/structures/img/panel/m.png
--rw-r--r--   0        0        0     8879 2023-06-28 11:50:10.172552 aa_structures-2.4.1/structures/static/structures/img/panel/noship.png
--rw-r--r--   0        0        0     1480 2023-06-28 11:50:10.172552 aa_structures-2.4.1/structures/static/structures/img/panel/r.png
--rw-r--r--   0        0        0    43642 2023-06-28 11:50:10.172552 aa_structures-2.4.1/structures/static/structures/img/panel/tyrannis.png
--rw-r--r--   0        0        0    43560 2023-06-28 11:50:10.172552 aa_structures-2.4.1/structures/static/structures/img/panel/tyrannis_blue.png
--rw-r--r--   0        0        0    42833 2023-06-28 11:50:10.172552 aa_structures-2.4.1/structures/static/structures/img/panel/tyrannis_darkred.png
--rw-r--r--   0        0        0    38343 2023-06-28 11:50:10.172552 aa_structures-2.4.1/structures/static/structures/img/panel/tyrannis_default.png
--rw-r--r--   0        0        0    42868 2023-06-28 11:50:10.172552 aa_structures-2.4.1/structures/static/structures/img/panel/tyrannis_revelations.png
--rw-r--r--   0        0        0      496 2023-06-28 11:50:10.172552 aa_structures-2.4.1/structures/static/structures/img/structures_logo.png
--rw-r--r--   0        0        0     8806 2023-06-28 11:50:10.172552 aa_structures-2.4.1/structures/tasks.py
--rw-r--r--   0        0        0      298 2023-06-28 11:50:10.172552 aa_structures-2.4.1/structures/templates/structures/base.html
--rw-r--r--   0        0        0    21200 2023-06-28 11:50:10.172552 aa_structures-2.4.1/structures/templates/structures/main.html
--rw-r--r--   0        0        0      264 2023-06-28 11:50:10.172552 aa_structures-2.4.1/structures/templates/structures/modals/fitting_assets.html
--rw-r--r--   0        0        0     9530 2023-06-28 11:50:10.172552 aa_structures-2.4.1/structures/templates/structures/modals/fitting_gfx.html
--rw-r--r--   0        0        0     2705 2023-06-28 11:50:10.172552 aa_structures-2.4.1/structures/templates/structures/modals/poco_details.html
--rw-r--r--   0        0        0     4133 2023-06-28 11:50:10.172552 aa_structures-2.4.1/structures/templates/structures/modals/starbase_detail.html
--rw-r--r--   0        0        0     4070 2023-06-28 11:50:10.172552 aa_structures-2.4.1/structures/templates/structures/modals/structure_details.html
--rw-r--r--   0        0        0      998 2023-06-28 11:50:10.172552 aa_structures-2.4.1/structures/templates/structures/modals/tab_general_detail.html
--rw-r--r--   0        0        0     1501 2023-06-28 11:50:10.172552 aa_structures-2.4.1/structures/templates/structures/partials/jump_gates_list.html
--rw-r--r--   0        0        0     1034 2023-06-28 11:50:10.172552 aa_structures-2.4.1/structures/templates/structures/partials/poco_list.html
--rw-r--r--   0        0        0     5947 2023-06-28 11:50:10.172552 aa_structures-2.4.1/structures/templates/structures/partials/structure_list.html
--rw-r--r--   0        0        0     1586 2023-06-28 11:50:10.172552 aa_structures-2.4.1/structures/templates/structures/partials/structure_summary.html
--rw-r--r--   0        0        0      117 2023-06-28 11:50:10.172552 aa_structures-2.4.1/structures/templates/structures/templatetags/detail_title.html
--rw-r--r--   0        0        0      375 2023-06-28 11:50:10.172552 aa_structures-2.4.1/structures/templates/structures/templatetags/list_asset.html
--rw-r--r--   0        0        0      706 2023-06-28 11:50:10.172552 aa_structures-2.4.1/structures/templates/structures/templatetags/list_item.html
--rw-r--r--   0        0        0      505 2023-06-28 11:50:10.172552 aa_structures-2.4.1/structures/templates/structures/templatetags/list_tax_item.html
--rw-r--r--   0        0        0       68 2023-06-28 11:50:10.172552 aa_structures-2.4.1/structures/templates/structures/templatetags/list_title.html
--rw-r--r--   0        0        0        0 2023-06-29 12:58:08.036016 aa_structures-2.4.1/structures/templatetags/__init__.py
--rw-r--r--   0        0        0     1601 2023-06-28 11:50:10.172552 aa_structures-2.4.1/structures/templatetags/structures.py
--rw-r--r--   0        0        0       75 2023-06-28 11:50:10.172552 aa_structures-2.4.1/structures/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-06-29 12:58:08.036016 aa_structures-2.4.1/structures/tests/core/__init__.py
--rw-r--r--   0        0        0    13532 2023-06-28 11:50:10.172552 aa_structures-2.4.1/structures/tests/core/test_notification_embeds.py
--rw-r--r--   0        0        0    10435 2023-06-28 11:50:10.172552 aa_structures-2.4.1/structures/tests/core/test_notification_structuretimers.py
--rw-r--r--   0        0        0     5515 2023-06-28 11:50:10.176552 aa_structures-2.4.1/structures/tests/core/test_notifications_timerboard.py
--rw-r--r--   0        0        0     3385 2023-06-28 11:50:10.176552 aa_structures-2.4.1/structures/tests/core/test_serializers.py
--rw-r--r--   0        0        0      825 2023-06-28 11:50:10.176552 aa_structures-2.4.1/structures/tests/core/test_sovereignty.py
--rw-r--r--   0        0        0     3163 2023-06-28 11:50:10.176552 aa_structures-2.4.1/structures/tests/core/test_starbases.py
--rw-r--r--   0        0        0        0 2023-06-29 12:58:08.036016 aa_structures-2.4.1/structures/tests/models/__init__.py
--rw-r--r--   0        0        0     1600 2023-06-28 11:50:10.176552 aa_structures-2.4.1/structures/tests/models/test_eveuniverse.py
--rw-r--r--   0        0        0    39346 2023-06-28 11:50:10.176552 aa_structures-2.4.1/structures/tests/models/test_notifications_1.py
--rw-r--r--   0        0        0    31553 2023-06-28 11:50:10.176552 aa_structures-2.4.1/structures/tests/models/test_notifications_2.py
--rw-r--r--   0        0        0     6004 2023-06-28 11:50:10.176552 aa_structures-2.4.1/structures/tests/models/test_notifications_3.py
--rw-r--r--   0        0        0     5318 2023-06-28 11:50:10.176552 aa_structures-2.4.1/structures/tests/models/test_notifications_discord.py
--rw-r--r--   0        0        0    26807 2023-06-28 11:50:10.176552 aa_structures-2.4.1/structures/tests/models/test_owners_1.py
--rw-r--r--   0        0        0    54158 2023-06-28 11:50:10.176552 aa_structures-2.4.1/structures/tests/models/test_owners_2.py
--rw-r--r--   0        0        0    37407 2023-06-28 11:50:10.176552 aa_structures-2.4.1/structures/tests/models/test_owners_3.py
--rw-r--r--   0        0        0    37744 2023-06-28 11:50:10.176552 aa_structures-2.4.1/structures/tests/models/test_structures.py
--rw-r--r--   0        0        0    21127 2023-06-28 11:50:10.176552 aa_structures-2.4.1/structures/tests/test_admin.py
--rw-r--r--   0        0        0     1242 2023-06-28 11:50:10.176552 aa_structures-2.4.1/structures/tests/test_checks.py
--rw-r--r--   0        0        0     1861 2023-06-28 11:50:10.176552 aa_structures-2.4.1/structures/tests/test_helpers.py
--rw-r--r--   0        0        0    23524 2023-06-28 11:50:10.176552 aa_structures-2.4.1/structures/tests/test_integration.py
--rw-r--r--   0        0        0    27217 2023-06-29 12:35:51.837332 aa_structures-2.4.1/structures/tests/test_managers_1.py
--rw-r--r--   0        0        0     1567 2023-06-28 11:50:10.176552 aa_structures-2.4.1/structures/tests/test_managers_3.py
--rw-r--r--   0        0        0    18409 2023-06-28 11:50:10.176552 aa_structures-2.4.1/structures/tests/test_tasks.py
--rw-r--r--   0        0        0    36695 2023-06-28 11:50:10.176552 aa_structures-2.4.1/structures/tests/test_views.py
--rw-r--r--   0        0        0        0 2023-06-29 12:58:08.036016 aa_structures-2.4.1/structures/tests/testdata/__init__.py
--rw-r--r--   0        0        0     2601 2023-06-28 11:50:10.176552 aa_structures-2.4.1/structures/tests/testdata/create_eveuniverse.py
--rw-r--r--   0        0        0    33188 2023-06-28 11:50:10.176552 aa_structures-2.4.1/structures/tests/testdata/entities.json
--rw-r--r--   0        0        0    13864 2023-06-28 11:50:10.176552 aa_structures-2.4.1/structures/tests/testdata/esi_data.json
--rw-r--r--   0        0        0   979813 2023-06-28 11:50:10.180552 aa_structures-2.4.1/structures/tests/testdata/eveuniverse.json
--rw-r--r--   0        0        0     7827 2023-06-28 11:50:10.180552 aa_structures-2.4.1/structures/tests/testdata/factories.py
--rw-r--r--   0        0        0    10857 2023-06-28 11:50:10.180552 aa_structures-2.4.1/structures/tests/testdata/factories_2.py
--rw-r--r--   0        0        0     5746 2023-06-28 11:50:10.180552 aa_structures-2.4.1/structures/tests/testdata/generate_notifications.py
--rw-r--r--   0        0        0     1415 2023-06-28 11:50:10.180552 aa_structures-2.4.1/structures/tests/testdata/generate_notifications_2.py
--rw-r--r--   0        0        0     6238 2023-06-28 11:50:10.180552 aa_structures-2.4.1/structures/tests/testdata/generate_structures.py
--rw-r--r--   0        0        0    26820 2023-06-28 11:50:10.180552 aa_structures-2.4.1/structures/tests/testdata/helpers.py
--rw-r--r--   0        0        0      395 2023-06-28 11:50:10.180552 aa_structures-2.4.1/structures/tests/testdata/load_eveuniverse.py
--rw-r--r--   0        0        0      963 2023-06-28 11:50:10.180552 aa_structures-2.4.1/structures/tests/testdata/tasks_loadtest.py
--rw-r--r--   0        0        0      414 2023-06-28 11:50:10.180552 aa_structures-2.4.1/structures/tests/testdata/test_generate_structures.py
--rw-r--r--   0        0        0     1057 2023-06-28 11:50:10.180552 aa_structures-2.4.1/structures/urls.py
--rw-r--r--   0        0        0    21820 2023-06-28 11:50:10.180552 aa_structures-2.4.1/structures/views.py
--rw-r--r--   0        0        0        0 2023-06-29 12:58:08.036016 aa_structures-2.4.1/structures/webhooks/__init__.py
--rw-r--r--   0        0        0     6587 2023-06-28 11:50:10.180552 aa_structures-2.4.1/structures/webhooks/core.py
--rw-r--r--   0        0        0     1036 2023-06-28 11:50:10.180552 aa_structures-2.4.1/structures/webhooks/managers.py
--rw-r--r--   0        0        0     1641 2023-06-28 11:50:10.180552 aa_structures-2.4.1/structures/webhooks/models.py
--rw-r--r--   0        0        0        0 2023-06-29 12:58:08.036016 aa_structures-2.4.1/structures/webhooks/tests/__init__.py
--rw-r--r--   0        0        0     6395 2023-06-28 11:50:10.180552 aa_structures-2.4.1/structures/webhooks/tests/test_core.py
--rw-r--r--   0        0        0      459 2023-06-28 11:50:10.180552 aa_structures-2.4.1/structures/webhooks/tests/test_utils.py
--rw-r--r--   0        0        0     5933 1970-01-01 00:00:00.000000 aa_structures-2.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-27 19:21:52.362421 aa_structures-2.4.2/LICENSE
+-rw-r--r--   0        0        0     4406 2023-07-27 19:21:52.362421 aa_structures-2.4.2/README.md
+-rw-r--r--   0        0        0     2113 2023-07-27 19:21:52.366421 aa_structures-2.4.2/pyproject.toml
+-rw-r--r--   0        0        0      170 2023-07-27 19:21:52.366421 aa_structures-2.4.2/structures/__init__.py
+-rw-r--r--   0        0        0    36110 2023-07-27 19:21:52.366421 aa_structures-2.4.2/structures/admin.py
+-rw-r--r--   0        0        0     6228 2023-07-27 19:21:52.366421 aa_structures-2.4.2/structures/app_settings.py
+-rw-r--r--   0        0        0      195 2023-07-27 19:21:52.366421 aa_structures-2.4.2/structures/apps.py
+-rw-r--r--   0        0        0      915 2023-07-27 19:21:52.366421 aa_structures-2.4.2/structures/auth_hooks.py
+-rw-r--r--   0        0        0      741 2023-07-27 19:21:52.366421 aa_structures-2.4.2/structures/constants.py
+-rw-r--r--   0        0        0        0 2023-07-27 19:48:00.999760 aa_structures-2.4.2/structures/core/__init__.py
+-rw-r--r--   0        0        0    71519 2023-07-27 19:21:52.366421 aa_structures-2.4.2/structures/core/notification_embeds.py
+-rw-r--r--   0        0        0    16436 2023-07-27 19:21:52.366421 aa_structures-2.4.2/structures/core/notification_timers.py
+-rw-r--r--   0        0        0    19834 2023-07-27 19:21:52.366421 aa_structures-2.4.2/structures/core/serializers.py
+-rw-r--r--   0        0        0      623 2023-07-27 19:21:52.366421 aa_structures-2.4.2/structures/core/sovereignty.py
+-rw-r--r--   0        0        0     1613 2023-07-27 19:21:52.366421 aa_structures-2.4.2/structures/core/starbases.py
+-rw-r--r--   0        0        0      382 2023-07-27 19:21:52.366421 aa_structures-2.4.2/structures/forms.py
+-rw-r--r--   0        0        0        0 2023-07-27 19:48:01.007759 aa_structures-2.4.2/structures/helpers/__init__.py
+-rw-r--r--   0        0        0      830 2023-07-27 19:21:52.366421 aa_structures-2.4.2/structures/helpers/general.py
+-rw-r--r--   0        0        0    13634 2023-07-27 19:21:52.366421 aa_structures-2.4.2/structures/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    61204 2023-07-27 19:21:52.366421 aa_structures-2.4.2/structures/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    47227 2023-07-27 19:21:52.366421 aa_structures-2.4.2/structures/locale/django.pot
+-rw-r--r--   0        0        0      380 2023-07-27 19:21:52.366421 aa_structures-2.4.2/structures/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    47274 2023-07-27 19:21:52.366421 aa_structures-2.4.2/structures/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     5784 2023-07-27 19:21:52.366421 aa_structures-2.4.2/structures/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    55691 2023-07-27 19:21:52.366421 aa_structures-2.4.2/structures/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    47227 2023-07-27 19:21:52.370421 aa_structures-2.4.2/structures/locale/fr_FR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    47227 2023-07-27 19:21:52.370421 aa_structures-2.4.2/structures/locale/it_IT/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    47267 2023-07-27 19:21:52.370421 aa_structures-2.4.2/structures/locale/ja/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      391 2023-07-27 19:21:52.370421 aa_structures-2.4.2/structures/locale/ko/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    47024 2023-07-27 19:21:52.370421 aa_structures-2.4.2/structures/locale/ko/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    47227 2023-07-27 19:21:52.370421 aa_structures-2.4.2/structures/locale/ko_KR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      538 2023-07-27 19:21:52.370421 aa_structures-2.4.2/structures/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    47437 2023-07-27 19:21:52.370421 aa_structures-2.4.2/structures/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    47505 2023-07-27 19:21:52.370421 aa_structures-2.4.2/structures/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    11588 2023-07-27 19:21:52.370421 aa_structures-2.4.2/structures/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    58962 2023-07-27 19:21:52.370421 aa_structures-2.4.2/structures/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2023-07-27 19:48:01.007759 aa_structures-2.4.2/structures/management/commands/__init__.py
+-rw-r--r--   0        0        0     1443 2023-07-27 19:21:52.370421 aa_structures-2.4.2/structures/management/commands/structures_load_eve.py
+-rw-r--r--   0        0        0     2398 2023-07-27 19:21:52.370421 aa_structures-2.4.2/structures/management/commands/structures_preload_eveuniverse.py
+-rw-r--r--   0        0        0    18114 2023-07-27 19:21:52.370421 aa_structures-2.4.2/structures/managers.py
+-rw-r--r--   0        0        0    59315 2023-07-27 19:21:52.370421 aa_structures-2.4.2/structures/migrations/0001_initial_new.py
+-rw-r--r--   0        0        0     2274 2023-07-27 19:21:52.370421 aa_structures-2.4.2/structures/migrations/0002_remove_eveuniverse_relation_names.py
+-rw-r--r--   0        0        0    44042 2023-07-27 19:21:52.370421 aa_structures-2.4.2/structures/migrations/0003_add_localization_and_unique_key.py
+-rw-r--r--   0        0        0        0 2023-07-27 19:48:01.007759 aa_structures-2.4.2/structures/migrations/__init__.py
+-rw-r--r--   0        0        0      505 2023-07-27 19:21:52.370421 aa_structures-2.4.2/structures/models/__init__.py
+-rw-r--r--   0        0        0     2073 2023-07-27 19:21:52.370421 aa_structures-2.4.2/structures/models/eveuniverse.py
+-rw-r--r--   0        0        0    42745 2023-07-27 19:21:52.370421 aa_structures-2.4.2/structures/models/notifications.py
+-rw-r--r--   0        0        0    53967 2023-07-27 19:21:52.374420 aa_structures-2.4.2/structures/models/owners.py
+-rw-r--r--   0        0        0    37256 2023-07-27 19:21:52.374420 aa_structures-2.4.2/structures/models/structures.py
+-rw-r--r--   0        0        0      274 2023-07-27 19:21:52.374420 aa_structures-2.4.2/structures/providers.py
+-rw-r--r--   0        0        0     1165 2023-07-27 19:21:52.374420 aa_structures-2.4.2/structures/static/structures/css/global.css
+-rw-r--r--   0        0        0     1186 2023-07-27 19:21:52.374420 aa_structures-2.4.2/structures/static/structures/css/main.css
+-rw-r--r--   0        0        0    43262 2023-07-27 19:21:52.374420 aa_structures-2.4.2/structures/static/structures/img/Spinner-1s-64px-dark.gif
+-rw-r--r--   0        0        0    43381 2023-07-27 19:21:52.374420 aa_structures-2.4.2/structures/static/structures/img/Spinner-1s-64px-light.gif
+-rw-r--r--   0        0        0      908 2023-07-27 19:21:52.374420 aa_structures-2.4.2/structures/static/structures/img/eve_symbol_128.png
+-rw-r--r--   0        0        0      805 2023-07-27 19:21:52.374420 aa_structures-2.4.2/structures/static/structures/img/panel/0h.png
+-rw-r--r--   0        0        0      805 2023-07-27 19:21:52.374420 aa_structures-2.4.2/structures/static/structures/img/panel/0l.png
+-rw-r--r--   0        0        0      805 2023-07-27 19:21:52.374420 aa_structures-2.4.2/structures/static/structures/img/panel/0m.png
+-rw-r--r--   0        0        0      805 2023-07-27 19:21:52.374420 aa_structures-2.4.2/structures/static/structures/img/panel/0r.png
+-rw-r--r--   0        0        0      805 2023-07-27 19:21:52.374420 aa_structures-2.4.2/structures/static/structures/img/panel/0s.png
+-rw-r--r--   0        0        0     2590 2023-07-27 19:21:52.374420 aa_structures-2.4.2/structures/static/structures/img/panel/1h.png
+-rw-r--r--   0        0        0     1976 2023-07-27 19:21:52.374420 aa_structures-2.4.2/structures/static/structures/img/panel/1l.png
+-rw-r--r--   0        0        0     2025 2023-07-27 19:21:52.374420 aa_structures-2.4.2/structures/static/structures/img/panel/1m.png
+-rw-r--r--   0        0        0     2512 2023-07-27 19:21:52.374420 aa_structures-2.4.2/structures/static/structures/img/panel/1r.png
+-rw-r--r--   0        0        0     3541 2023-07-27 19:21:52.374420 aa_structures-2.4.2/structures/static/structures/img/panel/2h.png
+-rw-r--r--   0        0        0     2570 2023-07-27 19:21:52.374420 aa_structures-2.4.2/structures/static/structures/img/panel/2l.png
+-rw-r--r--   0        0        0     2766 2023-07-27 19:21:52.374420 aa_structures-2.4.2/structures/static/structures/img/panel/2m.png
+-rw-r--r--   0        0        0     3497 2023-07-27 19:21:52.374420 aa_structures-2.4.2/structures/static/structures/img/panel/2r.png
+-rw-r--r--   0        0        0     4607 2023-07-27 19:21:52.374420 aa_structures-2.4.2/structures/static/structures/img/panel/3h.png
+-rw-r--r--   0        0        0     3523 2023-07-27 19:21:52.374420 aa_structures-2.4.2/structures/static/structures/img/panel/3l.png
+-rw-r--r--   0        0        0     3720 2023-07-27 19:21:52.374420 aa_structures-2.4.2/structures/static/structures/img/panel/3m.png
+-rw-r--r--   0        0        0     4886 2023-07-27 19:21:52.374420 aa_structures-2.4.2/structures/static/structures/img/panel/3r.png
+-rw-r--r--   0        0        0     5309 2023-07-27 19:21:52.374420 aa_structures-2.4.2/structures/static/structures/img/panel/4h.png
+-rw-r--r--   0        0        0     4628 2023-07-27 19:21:52.374420 aa_structures-2.4.2/structures/static/structures/img/panel/4l.png
+-rw-r--r--   0        0        0     4956 2023-07-27 19:21:52.374420 aa_structures-2.4.2/structures/static/structures/img/panel/4m.png
+-rw-r--r--   0        0        0     9490 2023-07-27 19:21:52.374420 aa_structures-2.4.2/structures/static/structures/img/panel/4s.png
+-rw-r--r--   0        0        0     6109 2023-07-27 19:21:52.374420 aa_structures-2.4.2/structures/static/structures/img/panel/5h.png
+-rw-r--r--   0        0        0     5888 2023-07-27 19:21:52.374420 aa_structures-2.4.2/structures/static/structures/img/panel/5l.png
+-rw-r--r--   0        0        0     6270 2023-07-27 19:21:52.374420 aa_structures-2.4.2/structures/static/structures/img/panel/5m.png
+-rw-r--r--   0        0        0     7399 2023-07-27 19:21:52.374420 aa_structures-2.4.2/structures/static/structures/img/panel/5s.png
+-rw-r--r--   0        0        0     7203 2023-07-27 19:21:52.374420 aa_structures-2.4.2/structures/static/structures/img/panel/6h.png
+-rw-r--r--   0        0        0     7014 2023-07-27 19:21:52.374420 aa_structures-2.4.2/structures/static/structures/img/panel/6l.png
+-rw-r--r--   0        0        0     7439 2023-07-27 19:21:52.374420 aa_structures-2.4.2/structures/static/structures/img/panel/6m.png
+-rw-r--r--   0        0        0     8288 2023-07-27 19:21:52.374420 aa_structures-2.4.2/structures/static/structures/img/panel/7h.png
+-rw-r--r--   0        0        0     8067 2023-07-27 19:21:52.374420 aa_structures-2.4.2/structures/static/structures/img/panel/7l.png
+-rw-r--r--   0        0        0     8580 2023-07-27 19:21:52.374420 aa_structures-2.4.2/structures/static/structures/img/panel/7m.png
+-rw-r--r--   0        0        0     9276 2023-07-27 19:21:52.378420 aa_structures-2.4.2/structures/static/structures/img/panel/8h.png
+-rw-r--r--   0        0        0     8972 2023-07-27 19:21:52.378420 aa_structures-2.4.2/structures/static/structures/img/panel/8l.png
+-rw-r--r--   0        0        0     9541 2023-07-27 19:21:52.378420 aa_structures-2.4.2/structures/static/structures/img/panel/8m.png
+-rw-r--r--   0        0        0      195 2023-07-27 19:21:52.378420 aa_structures-2.4.2/structures/static/structures/img/panel/blank.png
+-rw-r--r--   0        0        0    16840 2023-07-27 19:21:52.378420 aa_structures-2.4.2/structures/static/structures/img/panel/circle.png
+-rw-r--r--   0        0        0    33523 2023-07-27 19:21:52.378420 aa_structures-2.4.2/structures/static/structures/img/panel/dustwheel.png
+-rw-r--r--   0        0        0     1480 2023-07-27 19:21:52.378420 aa_structures-2.4.2/structures/static/structures/img/panel/h.png
+-rw-r--r--   0        0        0     1480 2023-07-27 19:21:52.378420 aa_structures-2.4.2/structures/static/structures/img/panel/l.png
+-rw-r--r--   0        0        0     1480 2023-07-27 19:21:52.378420 aa_structures-2.4.2/structures/static/structures/img/panel/m.png
+-rw-r--r--   0        0        0     8879 2023-07-27 19:21:52.378420 aa_structures-2.4.2/structures/static/structures/img/panel/noship.png
+-rw-r--r--   0        0        0     1480 2023-07-27 19:21:52.378420 aa_structures-2.4.2/structures/static/structures/img/panel/r.png
+-rw-r--r--   0        0        0    43642 2023-07-27 19:21:52.378420 aa_structures-2.4.2/structures/static/structures/img/panel/tyrannis.png
+-rw-r--r--   0        0        0    43560 2023-07-27 19:21:52.378420 aa_structures-2.4.2/structures/static/structures/img/panel/tyrannis_blue.png
+-rw-r--r--   0        0        0    42833 2023-07-27 19:21:52.378420 aa_structures-2.4.2/structures/static/structures/img/panel/tyrannis_darkred.png
+-rw-r--r--   0        0        0    38343 2023-07-27 19:21:52.378420 aa_structures-2.4.2/structures/static/structures/img/panel/tyrannis_default.png
+-rw-r--r--   0        0        0    42868 2023-07-27 19:21:52.378420 aa_structures-2.4.2/structures/static/structures/img/panel/tyrannis_revelations.png
+-rw-r--r--   0        0        0      496 2023-07-27 19:21:52.378420 aa_structures-2.4.2/structures/static/structures/img/structures_logo.png
+-rw-r--r--   0        0        0     8806 2023-07-27 19:21:52.378420 aa_structures-2.4.2/structures/tasks.py
+-rw-r--r--   0        0        0      298 2023-07-27 19:21:52.378420 aa_structures-2.4.2/structures/templates/structures/base.html
+-rw-r--r--   0        0        0    21200 2023-07-27 19:21:52.378420 aa_structures-2.4.2/structures/templates/structures/main.html
+-rw-r--r--   0        0        0      264 2023-07-27 19:21:52.378420 aa_structures-2.4.2/structures/templates/structures/modals/fitting_assets.html
+-rw-r--r--   0        0        0     9530 2023-07-27 19:21:52.378420 aa_structures-2.4.2/structures/templates/structures/modals/fitting_gfx.html
+-rw-r--r--   0        0        0     2705 2023-07-27 19:21:52.378420 aa_structures-2.4.2/structures/templates/structures/modals/poco_details.html
+-rw-r--r--   0        0        0     4133 2023-07-27 19:21:52.378420 aa_structures-2.4.2/structures/templates/structures/modals/starbase_detail.html
+-rw-r--r--   0        0        0     4070 2023-07-27 19:21:52.378420 aa_structures-2.4.2/structures/templates/structures/modals/structure_details.html
+-rw-r--r--   0        0        0      998 2023-07-27 19:21:52.378420 aa_structures-2.4.2/structures/templates/structures/modals/tab_general_detail.html
+-rw-r--r--   0        0        0     1501 2023-07-27 19:21:52.378420 aa_structures-2.4.2/structures/templates/structures/partials/jump_gates_list.html
+-rw-r--r--   0        0        0     1034 2023-07-27 19:21:52.378420 aa_structures-2.4.2/structures/templates/structures/partials/poco_list.html
+-rw-r--r--   0        0        0     5947 2023-07-27 19:21:52.378420 aa_structures-2.4.2/structures/templates/structures/partials/structure_list.html
+-rw-r--r--   0        0        0     1586 2023-07-27 19:21:52.378420 aa_structures-2.4.2/structures/templates/structures/partials/structure_summary.html
+-rw-r--r--   0        0        0      117 2023-07-27 19:21:52.378420 aa_structures-2.4.2/structures/templates/structures/templatetags/detail_title.html
+-rw-r--r--   0        0        0      375 2023-07-27 19:21:52.378420 aa_structures-2.4.2/structures/templates/structures/templatetags/list_asset.html
+-rw-r--r--   0        0        0      706 2023-07-27 19:21:52.378420 aa_structures-2.4.2/structures/templates/structures/templatetags/list_item.html
+-rw-r--r--   0        0        0      505 2023-07-27 19:21:52.378420 aa_structures-2.4.2/structures/templates/structures/templatetags/list_tax_item.html
+-rw-r--r--   0        0        0       68 2023-07-27 19:21:52.382420 aa_structures-2.4.2/structures/templates/structures/templatetags/list_title.html
+-rw-r--r--   0        0        0        0 2023-07-27 19:48:01.007759 aa_structures-2.4.2/structures/templatetags/__init__.py
+-rw-r--r--   0        0        0     1601 2023-07-27 19:21:52.382420 aa_structures-2.4.2/structures/templatetags/structures.py
+-rw-r--r--   0        0        0       75 2023-07-27 19:21:52.382420 aa_structures-2.4.2/structures/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-27 19:48:01.007759 aa_structures-2.4.2/structures/tests/core/__init__.py
+-rw-r--r--   0        0        0    13532 2023-07-27 19:21:52.382420 aa_structures-2.4.2/structures/tests/core/test_notification_embeds.py
+-rw-r--r--   0        0        0    10435 2023-07-27 19:21:52.382420 aa_structures-2.4.2/structures/tests/core/test_notification_structuretimers.py
+-rw-r--r--   0        0        0     5515 2023-07-27 19:21:52.382420 aa_structures-2.4.2/structures/tests/core/test_notifications_timerboard.py
+-rw-r--r--   0        0        0     3385 2023-07-27 19:21:52.382420 aa_structures-2.4.2/structures/tests/core/test_serializers.py
+-rw-r--r--   0        0        0      825 2023-07-27 19:21:52.382420 aa_structures-2.4.2/structures/tests/core/test_sovereignty.py
+-rw-r--r--   0        0        0     3163 2023-07-27 19:21:52.382420 aa_structures-2.4.2/structures/tests/core/test_starbases.py
+-rw-r--r--   0        0        0        0 2023-07-27 19:48:01.007759 aa_structures-2.4.2/structures/tests/models/__init__.py
+-rw-r--r--   0        0        0     1600 2023-07-27 19:21:52.382420 aa_structures-2.4.2/structures/tests/models/test_eveuniverse.py
+-rw-r--r--   0        0        0    39346 2023-07-27 19:21:52.382420 aa_structures-2.4.2/structures/tests/models/test_notifications_1.py
+-rw-r--r--   0        0        0    31553 2023-07-27 19:21:52.382420 aa_structures-2.4.2/structures/tests/models/test_notifications_2.py
+-rw-r--r--   0        0        0     6004 2023-07-27 19:21:52.382420 aa_structures-2.4.2/structures/tests/models/test_notifications_3.py
+-rw-r--r--   0        0        0     5318 2023-07-27 19:21:52.382420 aa_structures-2.4.2/structures/tests/models/test_notifications_discord.py
+-rw-r--r--   0        0        0    26807 2023-07-27 19:21:52.382420 aa_structures-2.4.2/structures/tests/models/test_owners_1.py
+-rw-r--r--   0        0        0    54158 2023-07-27 19:21:52.382420 aa_structures-2.4.2/structures/tests/models/test_owners_2.py
+-rw-r--r--   0        0        0    37407 2023-07-27 19:21:52.382420 aa_structures-2.4.2/structures/tests/models/test_owners_3.py
+-rw-r--r--   0        0        0    37744 2023-07-27 19:21:52.382420 aa_structures-2.4.2/structures/tests/models/test_structures.py
+-rw-r--r--   0        0        0    21127 2023-07-27 19:21:52.382420 aa_structures-2.4.2/structures/tests/test_admin.py
+-rw-r--r--   0        0        0     1861 2023-07-27 19:21:52.382420 aa_structures-2.4.2/structures/tests/test_helpers.py
+-rw-r--r--   0        0        0    23524 2023-07-27 19:21:52.382420 aa_structures-2.4.2/structures/tests/test_integration.py
+-rw-r--r--   0        0        0    27217 2023-07-27 19:21:52.382420 aa_structures-2.4.2/structures/tests/test_managers_1.py
+-rw-r--r--   0        0        0     1567 2023-07-27 19:21:52.382420 aa_structures-2.4.2/structures/tests/test_managers_3.py
+-rw-r--r--   0        0        0    18409 2023-07-27 19:21:52.382420 aa_structures-2.4.2/structures/tests/test_tasks.py
+-rw-r--r--   0        0        0    36695 2023-07-27 19:21:52.382420 aa_structures-2.4.2/structures/tests/test_views.py
+-rw-r--r--   0        0        0        0 2023-07-27 19:48:01.007759 aa_structures-2.4.2/structures/tests/testdata/__init__.py
+-rw-r--r--   0        0        0     2601 2023-07-27 19:21:52.382420 aa_structures-2.4.2/structures/tests/testdata/create_eveuniverse.py
+-rw-r--r--   0        0        0    33188 2023-07-27 19:21:52.386420 aa_structures-2.4.2/structures/tests/testdata/entities.json
+-rw-r--r--   0        0        0    13864 2023-07-27 19:21:52.386420 aa_structures-2.4.2/structures/tests/testdata/esi_data.json
+-rw-r--r--   0        0        0   979813 2023-07-27 19:21:52.386420 aa_structures-2.4.2/structures/tests/testdata/eveuniverse.json
+-rw-r--r--   0        0        0     7827 2023-07-27 19:21:52.386420 aa_structures-2.4.2/structures/tests/testdata/factories.py
+-rw-r--r--   0        0        0    10857 2023-07-27 19:21:52.386420 aa_structures-2.4.2/structures/tests/testdata/factories_2.py
+-rw-r--r--   0        0        0     5746 2023-07-27 19:21:52.386420 aa_structures-2.4.2/structures/tests/testdata/generate_notifications.py
+-rw-r--r--   0        0        0     1415 2023-07-27 19:21:52.386420 aa_structures-2.4.2/structures/tests/testdata/generate_notifications_2.py
+-rw-r--r--   0        0        0     6238 2023-07-27 19:21:52.386420 aa_structures-2.4.2/structures/tests/testdata/generate_structures.py
+-rw-r--r--   0        0        0    26820 2023-07-27 19:21:52.386420 aa_structures-2.4.2/structures/tests/testdata/helpers.py
+-rw-r--r--   0        0        0      395 2023-07-27 19:21:52.386420 aa_structures-2.4.2/structures/tests/testdata/load_eveuniverse.py
+-rw-r--r--   0        0        0      963 2023-07-27 19:21:52.386420 aa_structures-2.4.2/structures/tests/testdata/tasks_loadtest.py
+-rw-r--r--   0        0        0      414 2023-07-27 19:21:52.386420 aa_structures-2.4.2/structures/tests/testdata/test_generate_structures.py
+-rw-r--r--   0        0        0     1057 2023-07-27 19:21:52.386420 aa_structures-2.4.2/structures/urls.py
+-rw-r--r--   0        0        0    21820 2023-07-27 19:21:52.386420 aa_structures-2.4.2/structures/views.py
+-rw-r--r--   0        0        0        0 2023-07-27 19:48:01.011759 aa_structures-2.4.2/structures/webhooks/__init__.py
+-rw-r--r--   0        0        0     6587 2023-07-27 19:21:52.386420 aa_structures-2.4.2/structures/webhooks/core.py
+-rw-r--r--   0        0        0     1036 2023-07-27 19:21:52.390420 aa_structures-2.4.2/structures/webhooks/managers.py
+-rw-r--r--   0        0        0     1641 2023-07-27 19:21:52.390420 aa_structures-2.4.2/structures/webhooks/models.py
+-rw-r--r--   0        0        0        0 2023-07-27 19:48:01.011759 aa_structures-2.4.2/structures/webhooks/tests/__init__.py
+-rw-r--r--   0        0        0     6395 2023-07-27 19:21:52.390420 aa_structures-2.4.2/structures/webhooks/tests/test_core.py
+-rw-r--r--   0        0        0      459 2023-07-27 19:21:52.390420 aa_structures-2.4.2/structures/webhooks/tests/test_utils.py
+-rw-r--r--   0        0        0     5929 1970-01-01 00:00:00.000000 aa_structures-2.4.2/PKG-INFO
```

### Comparing `aa_structures-2.4.1/LICENSE` & `aa_structures-2.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/README.md` & `aa_structures-2.4.2/README.md`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/pyproject.toml` & `aa_structures-2.4.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -2,19 +2,17 @@
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "aa-structures"
 dynamic = ["version", "description"]
 readme = "README.md"
-license = {file = "LICENSE"}
+license = { file = "LICENSE" }
 requires-python = ">=3.8"
-authors = [
-    { name = "Erik Kalkoken", email = "kalkoken87@gmail.com" },
-]
+authors = [{ name = "Erik Kalkoken", email = "kalkoken87@gmail.com" }]
 classifiers = [
     "Environment :: Web Environment",
     "Framework :: Django",
     "Framework :: Django :: 4.0",
     "Intended Audience :: End Users/Desktop",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
@@ -24,21 +22,21 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Internet :: WWW/HTTP",
     "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
 ]
 dependencies = [
     "allianceauth-app-utils>=1.18.1",
-    "allianceauth>=3.0.0",
-    "dhooks-lite>=0.6.1",
+    "allianceauth>=3.0",
+    "dhooks-lite>=1.0",
     "django-eveuniverse>=1.0",
     "django-multiselectfield",
     "django-navhelper",
     "pytz!=2022.2",
-    "redis-simple-mq>=0.5",
+    "redis-simple-mq>=1.0",
 ]
 
 [project.urls]
 Homepage = "https://gitlab.com/ErikKalkoken/aa-structures"
 Documentation = "https://aa-structures.readthedocs.io/en/latest/"
 Source = "https://gitlab.com/ErikKalkoken/aa-structures"
 Changelog = "https://gitlab.com/ErikKalkoken/aa-structures/-/blob/master/CHANGELOG.md"
@@ -53,23 +51,24 @@
 sections = [
     "FUTURE",
     "STDLIB",
     "THIRDPARTY",
     "DJANGO",
     "ALLIANCEAUTH",
     "FIRSTPARTY",
-    "LOCALFOLDER"
+    "LOCALFOLDER",
 ]
 known_allianceauth = ["allianceauth", "app_utils"]
 known_django = ["django", "django_webtest", "esi", "eveuniverse"]
 
 [tool.pylint.'MASTER']
-ignore-patterns = ["test_.*.py,__init__.py", "generate_.*.py"]
+ignore-patterns = ["__init__.py", "auth_hooks.py", "apps.py"]
+ignore-paths = ["^.*/tests/.*$", "^.*/migrations/.*$"]
 
 [tool.pylint.'BASIC']
-good-names = ["i", "j", "k", "x", "f", "ex"]
+good-names = ["i", "j", "k", "ex"]
 
 [tool.pylint.'FORMAT']
-max-line-length = 100
+max-line-length = 120
 
 [tool.pylint.'MESSAGES CONTROL']
-disable = ["R", "C"]
+disable = ["R0902", "R0903"]
```

### Comparing `aa_structures-2.4.1/structures/admin.py` & `aa_structures-2.4.2/structures/admin.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/app_settings.py` & `aa_structures-2.4.2/structures/app_settings.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/auth_hooks.py` & `aa_structures-2.4.2/structures/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/constants.py` & `aa_structures-2.4.2/structures/constants.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/core/notification_embeds.py` & `aa_structures-2.4.2/structures/core/notification_embeds.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/core/notification_timers.py` & `aa_structures-2.4.2/structures/core/notification_timers.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/core/serializers.py` & `aa_structures-2.4.2/structures/core/serializers.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/core/sovereignty.py` & `aa_structures-2.4.2/structures/core/sovereignty.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/core/starbases.py` & `aa_structures-2.4.2/structures/core/starbases.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/helpers/general.py` & `aa_structures-2.4.2/structures/helpers/general.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/locale/de/LC_MESSAGES/django.mo` & `aa_structures-2.4.2/structures/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/locale/de/LC_MESSAGES/django.po` & `aa_structures-2.4.2/structures/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/locale/django.pot` & `aa_structures-2.4.2/structures/locale/django.pot`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/locale/en/LC_MESSAGES/django.po` & `aa_structures-2.4.2/structures/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/locale/es/LC_MESSAGES/django.mo` & `aa_structures-2.4.2/structures/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/locale/es/LC_MESSAGES/django.po` & `aa_structures-2.4.2/structures/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/locale/fr_FR/LC_MESSAGES/django.po` & `aa_structures-2.4.2/structures/locale/fr_FR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/locale/it_IT/LC_MESSAGES/django.po` & `aa_structures-2.4.2/structures/locale/it_IT/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/locale/ja/LC_MESSAGES/django.po` & `aa_structures-2.4.2/structures/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/locale/ko/LC_MESSAGES/django.po` & `aa_structures-2.4.2/structures/locale/ko/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/locale/ko_KR/LC_MESSAGES/django.po` & `aa_structures-2.4.2/structures/locale/ko_KR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/locale/ru/LC_MESSAGES/django.mo` & `aa_structures-2.4.2/structures/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/locale/ru/LC_MESSAGES/django.po` & `aa_structures-2.4.2/structures/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/locale/uk/LC_MESSAGES/django.po` & `aa_structures-2.4.2/structures/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/locale/zh_Hans/LC_MESSAGES/django.mo` & `aa_structures-2.4.2/structures/locale/zh_Hans/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/locale/zh_Hans/LC_MESSAGES/django.po` & `aa_structures-2.4.2/structures/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/management/commands/structures_load_eve.py` & `aa_structures-2.4.2/structures/management/commands/structures_load_eve.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/management/commands/structures_preload_eveuniverse.py` & `aa_structures-2.4.2/structures/management/commands/structures_preload_eveuniverse.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/managers.py` & `aa_structures-2.4.2/structures/managers.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/migrations/0001_initial_new.py` & `aa_structures-2.4.2/structures/migrations/0001_initial_new.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/migrations/0002_remove_eveuniverse_relation_names.py` & `aa_structures-2.4.2/structures/migrations/0002_remove_eveuniverse_relation_names.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/migrations/0003_add_localization_and_unique_key.py` & `aa_structures-2.4.2/structures/migrations/0003_add_localization_and_unique_key.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/models/eveuniverse.py` & `aa_structures-2.4.2/structures/models/eveuniverse.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/models/notifications.py` & `aa_structures-2.4.2/structures/models/notifications.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/models/owners.py` & `aa_structures-2.4.2/structures/models/owners.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/models/structures.py` & `aa_structures-2.4.2/structures/models/structures.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/static/structures/css/global.css` & `aa_structures-2.4.2/structures/static/structures/css/global.css`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/static/structures/css/main.css` & `aa_structures-2.4.2/structures/static/structures/css/main.css`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/static/structures/img/Spinner-1s-64px-dark.gif` & `aa_structures-2.4.2/structures/static/structures/img/Spinner-1s-64px-dark.gif`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/static/structures/img/Spinner-1s-64px-light.gif` & `aa_structures-2.4.2/structures/static/structures/img/Spinner-1s-64px-light.gif`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/static/structures/img/eve_symbol_128.png` & `aa_structures-2.4.2/structures/static/structures/img/eve_symbol_128.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/static/structures/img/panel/0h.png` & `aa_structures-2.4.2/structures/static/structures/img/panel/0h.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/static/structures/img/panel/0l.png` & `aa_structures-2.4.2/structures/static/structures/img/panel/0l.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/static/structures/img/panel/0m.png` & `aa_structures-2.4.2/structures/static/structures/img/panel/0m.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/static/structures/img/panel/0r.png` & `aa_structures-2.4.2/structures/static/structures/img/panel/0r.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/static/structures/img/panel/0s.png` & `aa_structures-2.4.2/structures/static/structures/img/panel/0s.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/static/structures/img/panel/1h.png` & `aa_structures-2.4.2/structures/static/structures/img/panel/1h.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/static/structures/img/panel/1l.png` & `aa_structures-2.4.2/structures/static/structures/img/panel/1l.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/static/structures/img/panel/1m.png` & `aa_structures-2.4.2/structures/static/structures/img/panel/1m.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/static/structures/img/panel/1r.png` & `aa_structures-2.4.2/structures/static/structures/img/panel/1r.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/static/structures/img/panel/2h.png` & `aa_structures-2.4.2/structures/static/structures/img/panel/2h.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/static/structures/img/panel/2l.png` & `aa_structures-2.4.2/structures/static/structures/img/panel/2l.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/static/structures/img/panel/2m.png` & `aa_structures-2.4.2/structures/static/structures/img/panel/2m.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/static/structures/img/panel/2r.png` & `aa_structures-2.4.2/structures/static/structures/img/panel/2r.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/static/structures/img/panel/3h.png` & `aa_structures-2.4.2/structures/static/structures/img/panel/3h.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/static/structures/img/panel/3l.png` & `aa_structures-2.4.2/structures/static/structures/img/panel/3l.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/static/structures/img/panel/3m.png` & `aa_structures-2.4.2/structures/static/structures/img/panel/3m.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/static/structures/img/panel/3r.png` & `aa_structures-2.4.2/structures/static/structures/img/panel/3r.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/static/structures/img/panel/4h.png` & `aa_structures-2.4.2/structures/static/structures/img/panel/4h.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/static/structures/img/panel/4l.png` & `aa_structures-2.4.2/structures/static/structures/img/panel/4l.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/static/structures/img/panel/4m.png` & `aa_structures-2.4.2/structures/static/structures/img/panel/4m.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/static/structures/img/panel/4s.png` & `aa_structures-2.4.2/structures/static/structures/img/panel/4s.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/static/structures/img/panel/5h.png` & `aa_structures-2.4.2/structures/static/structures/img/panel/5h.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/static/structures/img/panel/5l.png` & `aa_structures-2.4.2/structures/static/structures/img/panel/5l.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/static/structures/img/panel/5m.png` & `aa_structures-2.4.2/structures/static/structures/img/panel/5m.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/static/structures/img/panel/5s.png` & `aa_structures-2.4.2/structures/static/structures/img/panel/5s.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/static/structures/img/panel/6h.png` & `aa_structures-2.4.2/structures/static/structures/img/panel/6h.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/static/structures/img/panel/6l.png` & `aa_structures-2.4.2/structures/static/structures/img/panel/6l.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/static/structures/img/panel/6m.png` & `aa_structures-2.4.2/structures/static/structures/img/panel/6m.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/static/structures/img/panel/7h.png` & `aa_structures-2.4.2/structures/static/structures/img/panel/7h.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/static/structures/img/panel/7l.png` & `aa_structures-2.4.2/structures/static/structures/img/panel/7l.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/static/structures/img/panel/7m.png` & `aa_structures-2.4.2/structures/static/structures/img/panel/7m.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/static/structures/img/panel/8h.png` & `aa_structures-2.4.2/structures/static/structures/img/panel/8h.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/static/structures/img/panel/8l.png` & `aa_structures-2.4.2/structures/static/structures/img/panel/8l.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/static/structures/img/panel/8m.png` & `aa_structures-2.4.2/structures/static/structures/img/panel/8m.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/static/structures/img/panel/circle.png` & `aa_structures-2.4.2/structures/static/structures/img/panel/circle.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/static/structures/img/panel/dustwheel.png` & `aa_structures-2.4.2/structures/static/structures/img/panel/dustwheel.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/static/structures/img/panel/h.png` & `aa_structures-2.4.2/structures/static/structures/img/panel/h.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/static/structures/img/panel/l.png` & `aa_structures-2.4.2/structures/static/structures/img/panel/l.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/static/structures/img/panel/m.png` & `aa_structures-2.4.2/structures/static/structures/img/panel/m.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/static/structures/img/panel/noship.png` & `aa_structures-2.4.2/structures/static/structures/img/panel/noship.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/static/structures/img/panel/r.png` & `aa_structures-2.4.2/structures/static/structures/img/panel/r.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/static/structures/img/panel/tyrannis.png` & `aa_structures-2.4.2/structures/static/structures/img/panel/tyrannis.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/static/structures/img/panel/tyrannis_blue.png` & `aa_structures-2.4.2/structures/static/structures/img/panel/tyrannis_blue.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/static/structures/img/panel/tyrannis_darkred.png` & `aa_structures-2.4.2/structures/static/structures/img/panel/tyrannis_darkred.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/static/structures/img/panel/tyrannis_default.png` & `aa_structures-2.4.2/structures/static/structures/img/panel/tyrannis_default.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/static/structures/img/panel/tyrannis_revelations.png` & `aa_structures-2.4.2/structures/static/structures/img/panel/tyrannis_revelations.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/tasks.py` & `aa_structures-2.4.2/structures/tasks.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/templates/structures/main.html` & `aa_structures-2.4.2/structures/templates/structures/main.html`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/templates/structures/modals/fitting_gfx.html` & `aa_structures-2.4.2/structures/templates/structures/modals/fitting_gfx.html`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/templates/structures/modals/poco_details.html` & `aa_structures-2.4.2/structures/templates/structures/modals/poco_details.html`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/templates/structures/modals/starbase_detail.html` & `aa_structures-2.4.2/structures/templates/structures/modals/starbase_detail.html`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/templates/structures/modals/structure_details.html` & `aa_structures-2.4.2/structures/templates/structures/modals/structure_details.html`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/templates/structures/modals/tab_general_detail.html` & `aa_structures-2.4.2/structures/templates/structures/modals/tab_general_detail.html`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/templates/structures/partials/jump_gates_list.html` & `aa_structures-2.4.2/structures/templates/structures/partials/jump_gates_list.html`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/templates/structures/partials/poco_list.html` & `aa_structures-2.4.2/structures/templates/structures/partials/poco_list.html`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/templates/structures/partials/structure_list.html` & `aa_structures-2.4.2/structures/templates/structures/partials/structure_list.html`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/templates/structures/partials/structure_summary.html` & `aa_structures-2.4.2/structures/templates/structures/partials/structure_summary.html`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/templates/structures/templatetags/list_item.html` & `aa_structures-2.4.2/structures/templates/structures/templatetags/list_item.html`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/templatetags/structures.py` & `aa_structures-2.4.2/structures/templatetags/structures.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/tests/core/test_notification_embeds.py` & `aa_structures-2.4.2/structures/tests/core/test_notification_embeds.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/tests/core/test_notification_structuretimers.py` & `aa_structures-2.4.2/structures/tests/core/test_notification_structuretimers.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/tests/core/test_notifications_timerboard.py` & `aa_structures-2.4.2/structures/tests/core/test_notifications_timerboard.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/tests/core/test_serializers.py` & `aa_structures-2.4.2/structures/tests/core/test_serializers.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/tests/core/test_sovereignty.py` & `aa_structures-2.4.2/structures/tests/core/test_sovereignty.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/tests/core/test_starbases.py` & `aa_structures-2.4.2/structures/tests/core/test_starbases.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/tests/models/test_eveuniverse.py` & `aa_structures-2.4.2/structures/tests/models/test_eveuniverse.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/tests/models/test_notifications_1.py` & `aa_structures-2.4.2/structures/tests/models/test_notifications_1.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/tests/models/test_notifications_2.py` & `aa_structures-2.4.2/structures/tests/models/test_notifications_2.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/tests/models/test_notifications_3.py` & `aa_structures-2.4.2/structures/tests/models/test_notifications_3.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/tests/models/test_notifications_discord.py` & `aa_structures-2.4.2/structures/tests/models/test_notifications_discord.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/tests/models/test_owners_1.py` & `aa_structures-2.4.2/structures/tests/models/test_owners_1.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/tests/models/test_owners_2.py` & `aa_structures-2.4.2/structures/tests/models/test_owners_2.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/tests/models/test_owners_3.py` & `aa_structures-2.4.2/structures/tests/models/test_owners_3.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/tests/models/test_structures.py` & `aa_structures-2.4.2/structures/tests/models/test_structures.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/tests/test_admin.py` & `aa_structures-2.4.2/structures/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/tests/test_helpers.py` & `aa_structures-2.4.2/structures/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/tests/test_integration.py` & `aa_structures-2.4.2/structures/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/tests/test_managers_1.py` & `aa_structures-2.4.2/structures/tests/test_managers_1.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/tests/test_managers_3.py` & `aa_structures-2.4.2/structures/tests/test_managers_3.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/tests/test_tasks.py` & `aa_structures-2.4.2/structures/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/tests/test_views.py` & `aa_structures-2.4.2/structures/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/tests/testdata/create_eveuniverse.py` & `aa_structures-2.4.2/structures/tests/testdata/create_eveuniverse.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/tests/testdata/entities.json` & `aa_structures-2.4.2/structures/tests/testdata/entities.json`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/tests/testdata/esi_data.json` & `aa_structures-2.4.2/structures/tests/testdata/esi_data.json`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/tests/testdata/eveuniverse.json` & `aa_structures-2.4.2/structures/tests/testdata/eveuniverse.json`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/tests/testdata/factories.py` & `aa_structures-2.4.2/structures/tests/testdata/factories.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/tests/testdata/factories_2.py` & `aa_structures-2.4.2/structures/tests/testdata/factories_2.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/tests/testdata/generate_notifications.py` & `aa_structures-2.4.2/structures/tests/testdata/generate_notifications.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/tests/testdata/generate_notifications_2.py` & `aa_structures-2.4.2/structures/tests/testdata/generate_notifications_2.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/tests/testdata/generate_structures.py` & `aa_structures-2.4.2/structures/tests/testdata/generate_structures.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/tests/testdata/helpers.py` & `aa_structures-2.4.2/structures/tests/testdata/helpers.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/tests/testdata/tasks_loadtest.py` & `aa_structures-2.4.2/structures/tests/testdata/tasks_loadtest.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/urls.py` & `aa_structures-2.4.2/structures/urls.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/views.py` & `aa_structures-2.4.2/structures/views.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/webhooks/core.py` & `aa_structures-2.4.2/structures/webhooks/core.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/webhooks/managers.py` & `aa_structures-2.4.2/structures/webhooks/managers.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/webhooks/models.py` & `aa_structures-2.4.2/structures/webhooks/models.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/structures/webhooks/tests/test_core.py` & `aa_structures-2.4.2/structures/webhooks/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.1/PKG-INFO` & `aa_structures-2.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa-structures
-Version: 2.4.1
+Version: 2.4.2
 Summary: App for managing Eve Online structures with Alliance Auth.
 Author-email: Erik Kalkoken <kalkoken87@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.0
@@ -15,21 +15,21 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Dist: allianceauth-app-utils>=1.18.1
-Requires-Dist: allianceauth>=3.0.0
-Requires-Dist: dhooks-lite>=0.6.1
+Requires-Dist: allianceauth>=3.0
+Requires-Dist: dhooks-lite>=1.0
 Requires-Dist: django-eveuniverse>=1.0
 Requires-Dist: django-multiselectfield
 Requires-Dist: django-navhelper
 Requires-Dist: pytz!=2022.2
-Requires-Dist: redis-simple-mq>=0.5
+Requires-Dist: redis-simple-mq>=1.0
 Project-URL: Changelog, https://gitlab.com/ErikKalkoken/aa-structures/-/blob/master/CHANGELOG.md
 Project-URL: Documentation, https://aa-structures.readthedocs.io/en/latest/
 Project-URL: Homepage, https://gitlab.com/ErikKalkoken/aa-structures
 Project-URL: Source, https://gitlab.com/ErikKalkoken/aa-structures
 Project-URL: Tracker, https://gitlab.com/ErikKalkoken/aa-structures/-/issues
 
 # Structures
```

