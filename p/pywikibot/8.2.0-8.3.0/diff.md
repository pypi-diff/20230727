# Comparing `tmp/pywikibot-8.2.0.tar.gz` & `tmp/pywikibot-8.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywikibot-8.2.0.tar", last modified: Wed Jul  5 08:35:04 2023, max compression
+gzip compressed data, was "pywikibot-8.3.0.tar", last modified: Thu Jul 27 11:03:46 2023, max compression
```

## Comparing `pywikibot-8.2.0.tar` & `pywikibot-8.3.0.tar`

### file list

```diff
@@ -1,312 +1,312 @@
-drwxrwxrwx   0        0        0        0 2023-07-05 08:35:04.304314 pywikibot-8.2.0/
--rw-rw-rw-   0        0        0     4133 2023-07-02 16:47:05.000000 pywikibot-8.2.0/AUTHORS.rst
--rw-rw-rw-   0        0        0      177 2023-05-16 07:53:09.000000 pywikibot-8.2.0/CODE_OF_CONDUCT.rst
--rw-rw-rw-   0        0        0     1086 2023-05-16 07:53:09.000000 pywikibot-8.2.0/LICENSE
--rw-rw-rw-   0        0        0       88 2023-07-02 16:47:05.000000 pywikibot-8.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0    15888 2023-07-05 08:35:04.303317 pywikibot-8.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     5502 2023-07-02 16:47:05.000000 pywikibot-8.2.0/README.rst
--rw-rw-rw-   0        0        0     6529 2023-07-05 08:22:11.000000 pywikibot-8.2.0/ROADMAP.rst
-drwxrwxrwx   0        0        0        0 2023-07-05 08:35:03.079578 pywikibot-8.2.0/pywikibot/
--rw-rw-rw-   0        0        0    55546 2023-07-05 07:19:34.000000 pywikibot-8.2.0/pywikibot/__init__.py
--rw-rw-rw-   0        0        0      794 2023-07-05 08:22:11.000000 pywikibot-8.2.0/pywikibot/__metadata__.py
--rw-rw-rw-   0        0        0     1886 2023-05-16 07:53:09.000000 pywikibot-8.2.0/pywikibot/_wbtypes.py
--rw-rw-rw-   0        0        0     5655 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/backports.py
--rw-rw-rw-   0        0        0    94724 2023-07-04 09:42:32.000000 pywikibot-8.2.0/pywikibot/bot.py
--rw-rw-rw-   0        0        0    21197 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/bot_choice.py
-drwxrwxrwx   0        0        0        0 2023-07-05 08:35:03.133434 pywikibot-8.2.0/pywikibot/comms/
--rw-rw-rw-   0        0        0      121 2023-05-16 07:53:09.000000 pywikibot-8.2.0/pywikibot/comms/__init__.py
--rw-rw-rw-   0        0        0    15771 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/comms/eventstreams.py
--rw-rw-rw-   0        0        0    20087 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/comms/http.py
--rw-rw-rw-   0        0        0    46549 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/config.py
--rw-rw-rw-   0        0        0    45958 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/cosmetic_changes.py
--rw-rw-rw-   0        0        0     2090 2023-05-16 07:53:09.000000 pywikibot-8.2.0/pywikibot/daemonize.py
-drwxrwxrwx   0        0        0        0 2023-07-05 08:35:03.144404 pywikibot-8.2.0/pywikibot/data/
--rw-rw-rw-   0        0        0      160 2023-05-16 07:53:09.000000 pywikibot-8.2.0/pywikibot/data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-05 08:35:03.153381 pywikibot-8.2.0/pywikibot/data/api/
--rw-rw-rw-   0        0        0     3174 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/data/api/__init__.py
--rw-rw-rw-   0        0        0    41575 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/data/api/_generators.py
--rw-rw-rw-   0        0        0     7368 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/data/api/_optionset.py
--rw-rw-rw-   0        0        0    23238 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/data/api/_paraminfo.py
--rw-rw-rw-   0        0        0    53439 2023-07-04 09:42:32.000000 pywikibot-8.2.0/pywikibot/data/api/_requests.py
--rw-rw-rw-   0        0        0    14120 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/data/memento.py
--rw-rw-rw-   0        0        0     2919 2023-05-16 07:53:09.000000 pywikibot-8.2.0/pywikibot/data/mysql.py
--rw-rw-rw-   0        0        0     8902 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/data/sparql.py
--rw-rw-rw-   0        0        0     3970 2023-05-16 07:53:09.000000 pywikibot-8.2.0/pywikibot/data/wikistats.py
--rw-rw-rw-   0        0        0    96751 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/date.py
--rw-rw-rw-   0        0        0    24902 2023-07-04 16:05:52.000000 pywikibot-8.2.0/pywikibot/diff.py
--rw-rw-rw-   0        0        0     2042 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/echo.py
--rw-rw-rw-   0        0        0     7918 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/editor.py
--rw-rw-rw-   0        0        0    21189 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-07-05 08:35:03.210229 pywikibot-8.2.0/pywikibot/families/
--rw-rw-rw-   0        0        0      118 2023-05-16 07:53:09.000000 pywikibot-8.2.0/pywikibot/families/__init__.py
--rw-rw-rw-   0        0        0     1656 2023-07-04 16:26:13.000000 pywikibot-8.2.0/pywikibot/families/commons_family.py
--rw-rw-rw-   0        0        0      443 2023-05-16 07:53:09.000000 pywikibot-8.2.0/pywikibot/families/foundation_family.py
--rw-rw-rw-   0        0        0      338 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/families/i18n_family.py
--rw-rw-rw-   0        0        0      355 2023-05-15 15:00:32.000000 pywikibot-8.2.0/pywikibot/families/incubator_family.py
--rw-rw-rw-   0        0        0      583 2023-07-04 16:26:13.000000 pywikibot-8.2.0/pywikibot/families/lingualibre_family.py
--rw-rw-rw-   0        0        0      401 2023-05-15 15:00:32.000000 pywikibot-8.2.0/pywikibot/families/mediawiki_family.py
--rw-rw-rw-   0        0        0      593 2023-05-15 15:00:32.000000 pywikibot-8.2.0/pywikibot/families/meta_family.py
--rw-rw-rw-   0        0        0     1205 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/families/osm_family.py
--rw-rw-rw-   0        0        0      369 2023-05-15 15:00:32.000000 pywikibot-8.2.0/pywikibot/families/outreach_family.py
--rw-rw-rw-   0        0        0      361 2023-05-15 15:00:32.000000 pywikibot-8.2.0/pywikibot/families/species_family.py
--rw-rw-rw-   0        0        0      513 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/families/vikidia_family.py
--rw-rw-rw-   0        0        0     2418 2023-07-05 07:54:18.000000 pywikibot-8.2.0/pywikibot/families/wikibooks_family.py
--rw-rw-rw-   0        0        0      958 2023-07-04 16:26:13.000000 pywikibot-8.2.0/pywikibot/families/wikidata_family.py
--rw-rw-rw-   0        0        0     1631 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/families/wikihow_family.py
--rw-rw-rw-   0        0        0     1009 2023-05-15 15:00:32.000000 pywikibot-8.2.0/pywikibot/families/wikimania_family.py
--rw-rw-rw-   0        0        0      777 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/families/wikimediachapter_family.py
--rw-rw-rw-   0        0        0     1832 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/families/wikinews_family.py
--rw-rw-rw-   0        0        0    10732 2023-07-05 07:54:18.000000 pywikibot-8.2.0/pywikibot/families/wikipedia_family.py
--rw-rw-rw-   0        0        0     2886 2023-07-05 07:54:18.000000 pywikibot-8.2.0/pywikibot/families/wikiquote_family.py
--rw-rw-rw-   0        0        0     5335 2023-07-05 07:54:18.000000 pywikibot-8.2.0/pywikibot/families/wikisource_family.py
--rw-rw-rw-   0        0        0      431 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/families/wikispore_family.py
--rw-rw-rw-   0        0        0      425 2023-05-16 07:53:09.000000 pywikibot-8.2.0/pywikibot/families/wikitech_family.py
--rw-rw-rw-   0        0        0     1150 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/families/wikiversity_family.py
--rw-rw-rw-   0        0        0     1027 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/families/wikivoyage_family.py
--rw-rw-rw-   0        0        0     3850 2023-07-05 07:54:18.000000 pywikibot-8.2.0/pywikibot/families/wiktionary_family.py
--rw-rw-rw-   0        0        0     2414 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/families/wowwiki_family.py
--rw-rw-rw-   0        0        0    41181 2023-07-04 16:26:13.000000 pywikibot-8.2.0/pywikibot/family.py
--rw-rw-rw-   0        0        0    33191 2023-05-16 07:53:09.000000 pywikibot-8.2.0/pywikibot/fixes.py
--rw-rw-rw-   0        0        0    20119 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/flow.py
--rw-rw-rw-   0        0        0    29992 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/i18n.py
--rw-rw-rw-   0        0        0     8278 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/interwiki_graph.py
--rw-rw-rw-   0        0        0    13177 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/logentries.py
--rw-rw-rw-   0        0        0    12508 2023-05-16 07:53:09.000000 pywikibot-8.2.0/pywikibot/logging.py
--rw-rw-rw-   0        0        0    22771 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/login.py
-drwxrwxrwx   0        0        0        0 2023-07-05 08:35:03.230176 pywikibot-8.2.0/pywikibot/page/
--rw-rw-rw-   0        0        0     2350 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/page/__init__.py
--rw-rw-rw-   0        0        0    86838 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/page/_basepage.py
--rw-rw-rw-   0        0        0    14599 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/page/_category.py
--rw-rw-rw-   0        0        0    18914 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/page/_collections.py
--rw-rw-rw-   0        0        0     2139 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/page/_decorators.py
--rw-rw-rw-   0        0        0    17407 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/page/_filepage.py
--rw-rw-rw-   0        0        0    29329 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/page/_links.py
--rw-rw-rw-   0        0        0     8515 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/page/_page.py
--rw-rw-rw-   0        0        0     2997 2023-05-16 07:53:09.000000 pywikibot-8.2.0/pywikibot/page/_revision.py
--rw-rw-rw-   0        0        0     4049 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/page/_toolforge.py
--rw-rw-rw-   0        0        0    16266 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/page/_user.py
--rw-rw-rw-   0        0        0    85875 2023-07-05 07:19:34.000000 pywikibot-8.2.0/pywikibot/page/_wikibase.py
-drwxrwxrwx   0        0        0        0 2023-07-05 08:35:03.237158 pywikibot-8.2.0/pywikibot/pagegenerators/
--rw-rw-rw-   0        0        0    29391 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/pagegenerators/__init__.py
--rw-rw-rw-   0        0        0    40292 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/pagegenerators/_factory.py
--rw-rw-rw-   0        0        0    19242 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/pagegenerators/_filters.py
--rw-rw-rw-   0        0        0    45143 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/pagegenerators/_generators.py
--rw-rw-rw-   0        0        0     3938 2023-05-16 07:53:09.000000 pywikibot-8.2.0/pywikibot/plural.py
--rw-rw-rw-   0        0        0    48615 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/proofreadpage.py
-drwxrwxrwx   0        0        0        0 2023-07-05 08:35:03.251120 pywikibot-8.2.0/pywikibot/scripts/
--rw-rw-rw-   0        0        0      882 2023-05-16 07:53:09.000000 pywikibot-8.2.0/pywikibot/scripts/__init__.py
--rw-rw-rw-   0        0        0    11922 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/scripts/generate_family_file.py
--rw-rw-rw-   0        0        0    20021 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/scripts/generate_user_files.py
-drwxrwxrwx   0        0        0        0 2023-07-05 08:35:03.253116 pywikibot-8.2.0/pywikibot/scripts/i18n/
--rw-rw-rw-   0        0        0      309 2023-05-16 07:53:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-05 08:35:04.241483 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/
--rw-rw-rw-   0        0        0      166 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/ab.json
--rw-rw-rw-   0        0        0      511 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/af.json
--rw-rw-rw-   0        0        0      121 2022-04-07 08:52:21.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/an.json
--rw-rw-rw-   0        0        0     1227 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/ar.json
--rw-rw-rw-   0        0        0      131 2022-04-07 08:52:21.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/arc.json
--rw-rw-rw-   0        0        0     1042 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/ast.json
--rw-rw-rw-   0        0        0      163 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/av.json
--rw-rw-rw-   0        0        0      150 2022-04-07 08:52:21.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/awa.json
--rw-rw-rw-   0        0        0      898 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/az.json
--rw-rw-rw-   0        0        0      982 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/azb.json
--rw-rw-rw-   0        0        0     1362 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/ba.json
--rw-rw-rw-   0        0        0      210 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/bar.json
--rw-rw-rw-   0        0        0      989 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/bcc.json
--rw-rw-rw-   0        0        0     1491 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/be-tarask.json
--rw-rw-rw-   0        0        0      894 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/be.json
--rw-rw-rw-   0        0        0      535 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/bg.json
--rw-rw-rw-   0        0        0      203 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/bjn.json
--rw-rw-rw-   0        0        0      642 2023-04-06 12:04:37.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/bn.json
--rw-rw-rw-   0        0        0      179 2022-04-07 08:52:21.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/bo.json
--rw-rw-rw-   0        0        0     1048 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/br.json
--rw-rw-rw-   0        0        0      998 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/bs.json
--rw-rw-rw-   0        0        0     1198 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/ca.json
--rw-rw-rw-   0        0        0      981 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/ce.json
--rw-rw-rw-   0        0        0      768 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/ckb.json
--rw-rw-rw-   0        0        0     1178 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/cs.json
--rw-rw-rw-   0        0        0     1013 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/csb.json
--rw-rw-rw-   0        0        0      995 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/cy.json
--rw-rw-rw-   0        0        0     1022 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/da.json
--rw-rw-rw-   0        0        0     1065 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/de.json
--rw-rw-rw-   0        0        0     1025 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/diq.json
--rw-rw-rw-   0        0        0     1647 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/el.json
--rw-rw-rw-   0        0        0     1027 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/en.json
--rw-rw-rw-   0        0        0     1121 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/eo.json
--rw-rw-rw-   0        0        0     1203 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/es.json
--rw-rw-rw-   0        0        0      333 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/et.json
--rw-rw-rw-   0        0        0     1043 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/eu.json
--rw-rw-rw-   0        0        0     1424 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/fa.json
--rw-rw-rw-   0        0        0      660 2022-04-15 15:42:25.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/fi.json
--rw-rw-rw-   0        0        0      812 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/fo.json
--rw-rw-rw-   0        0        0     1291 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/fr.json
--rw-rw-rw-   0        0        0      227 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/frp.json
--rw-rw-rw-   0        0        0      988 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/frr.json
--rw-rw-rw-   0        0        0       95 2022-04-07 08:52:21.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/fy.json
--rw-rw-rw-   0        0        0      104 2022-04-07 08:52:21.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/ga.json
--rw-rw-rw-   0        0        0     1082 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/gl.json
--rw-rw-rw-   0        0        0      786 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/gsw.json
--rw-rw-rw-   0        0        0      711 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/hak.json
--rw-rw-rw-   0        0        0      858 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/haw.json
--rw-rw-rw-   0        0        0     1192 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/he.json
--rw-rw-rw-   0        0        0     1699 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/hi.json
--rw-rw-rw-   0        0        0      201 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/hr.json
--rw-rw-rw-   0        0        0      593 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/hsb.json
--rw-rw-rw-   0        0        0     1022 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/hu.json
--rw-rw-rw-   0        0        0      259 2022-04-15 15:42:25.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/hy.json
--rw-rw-rw-   0        0        0     1085 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/ia.json
--rw-rw-rw-   0        0        0     1146 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/id.json
--rw-rw-rw-   0        0        0      205 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/ie.json
--rw-rw-rw-   0        0        0      114 2022-04-07 08:52:21.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/ig.json
--rw-rw-rw-   0        0        0      220 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/ilo.json
--rw-rw-rw-   0        0        0     1011 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/io.json
--rw-rw-rw-   0        0        0      735 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/is.json
--rw-rw-rw-   0        0        0     1063 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/it.json
--rw-rw-rw-   0        0        0     1125 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/ja.json
--rw-rw-rw-   0        0        0      196 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/jv.json
--rw-rw-rw-   0        0        0      581 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/kab.json
--rw-rw-rw-   0        0        0     1068 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/kk.json
--rw-rw-rw-   0        0        0     1381 2022-04-07 08:52:21.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/km.json
--rw-rw-rw-   0        0        0      993 2022-04-07 08:52:21.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/kn.json
--rw-rw-rw-   0        0        0     1140 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/ko.json
--rw-rw-rw-   0        0        0     1409 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/krc.json
--rw-rw-rw-   0        0        0     1188 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/ksh.json
--rw-rw-rw-   0        0        0      318 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/ku.json
--rw-rw-rw-   0        0        0      331 2022-04-07 08:52:21.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/ky.json
--rw-rw-rw-   0        0        0      100 2022-04-07 08:52:21.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/la.json
--rw-rw-rw-   0        0        0      988 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/lb.json
--rw-rw-rw-   0        0        0      209 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/li.json
--rw-rw-rw-   0        0        0      174 2022-04-07 08:52:21.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/lki.json
--rw-rw-rw-   0        0        0      963 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/lt.json
--rw-rw-rw-   0        0        0      691 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/lv.json
--rw-rw-rw-   0        0        0      752 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/map-bms.json
--rw-rw-rw-   0        0        0      967 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/mg.json
--rw-rw-rw-   0        0        0      673 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/min.json
--rw-rw-rw-   0        0        0     1353 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/mk.json
--rw-rw-rw-   0        0        0     1943 2022-04-28 20:36:36.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/ml.json
--rw-rw-rw-   0        0        0      168 2022-04-07 08:52:21.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/mni.json
--rw-rw-rw-   0        0        0      267 2022-04-15 15:42:25.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/mr.json
--rw-rw-rw-   0        0        0      968 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/ms.json
--rw-rw-rw-   0        0        0      203 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/mt.json
--rw-rw-rw-   0        0        0     1335 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/my.json
--rw-rw-rw-   0        0        0     1049 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/nan.json
--rw-rw-rw-   0        0        0     1003 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/nb.json
--rw-rw-rw-   0        0        0      983 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/nds-nl.json
--rw-rw-rw-   0        0        0      197 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/nds.json
--rw-rw-rw-   0        0        0     1562 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/ne.json
--rw-rw-rw-   0        0        0      891 2022-04-07 08:52:21.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/new.json
--rw-rw-rw-   0        0        0     1037 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/nl.json
--rw-rw-rw-   0        0        0      232 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/nn.json
--rw-rw-rw-   0        0        0     1344 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/nqo.json
--rw-rw-rw-   0        0        0      148 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/nyn.json
--rw-rw-rw-   0        0        0      226 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/oc.json
--rw-rw-rw-   0        0        0      258 2022-04-07 08:52:21.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/olo.json
--rw-rw-rw-   0        0        0      154 2022-04-07 08:52:21.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/or.json
--rw-rw-rw-   0        0        0      216 2022-04-07 08:52:21.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/pa.json
--rw-rw-rw-   0        0        0      157 2023-04-06 12:04:37.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/pdc.json
--rw-rw-rw-   0        0        0      102 2022-04-07 08:52:21.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/pfl.json
--rw-rw-rw-   0        0        0     1011 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/pl.json
--rw-rw-rw-   0        0        0      870 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/pms.json
--rw-rw-rw-   0        0        0     1070 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/pt-br.json
--rw-rw-rw-   0        0        0     1187 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/pt.json
--rw-rw-rw-   0        0        0     1749 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/qqq.json
--rw-rw-rw-   0        0        0     1149 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/ro.json
--rw-rw-rw-   0        0        0     1582 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/ru.json
--rw-rw-rw-   0        0        0      149 2022-04-07 08:52:21.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/scn.json
--rw-rw-rw-   0        0        0      749 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/sco.json
--rw-rw-rw-   0        0        0      311 2022-04-07 08:52:21.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/sd.json
--rw-rw-rw-   0        0        0      551 2022-04-07 08:52:21.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/sh.json
--rw-rw-rw-   0        0        0      528 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/si.json
--rw-rw-rw-   0        0        0     1046 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/sk.json
--rw-rw-rw-   0        0        0      193 2023-04-06 12:04:37.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/skr-arab.json
--rw-rw-rw-   0        0        0     1078 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/sl.json
--rw-rw-rw-   0        0        0      127 2022-04-07 08:52:21.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/sms.json
--rw-rw-rw-   0        0        0      725 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/so.json
--rw-rw-rw-   0        0        0      452 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/sq.json
--rw-rw-rw-   0        0        0     1439 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/sr.json
--rw-rw-rw-   0        0        0      347 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/su.json
--rw-rw-rw-   0        0        0     1047 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/sv.json
--rw-rw-rw-   0        0        0      650 2022-04-07 08:52:21.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/sw.json
--rw-rw-rw-   0        0        0      124 2022-04-07 08:52:21.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/szl.json
--rw-rw-rw-   0        0        0      683 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/ta.json
--rw-rw-rw-   0        0        0     1390 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/te.json
--rw-rw-rw-   0        0        0      101 2023-04-06 12:04:37.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/tg.json
--rw-rw-rw-   0        0        0     1414 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/th.json
--rw-rw-rw-   0        0        0      155 2023-04-06 12:04:37.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/tk.json
--rw-rw-rw-   0        0        0      219 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/tl.json
--rw-rw-rw-   0        0        0     1115 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/tly.json
--rw-rw-rw-   0        0        0     1159 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/tr.json
--rw-rw-rw-   0        0        0      316 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/tt.json
--rw-rw-rw-   0        0        0     1417 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/uk.json
--rw-rw-rw-   0        0        0      789 2022-04-28 20:36:36.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/ur.json
--rw-rw-rw-   0        0        0      208 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/uz.json
--rw-rw-rw-   0        0        0      253 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/vec.json
--rw-rw-rw-   0        0        0      121 2022-04-07 08:52:22.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/vep.json
--rw-rw-rw-   0        0        0     1105 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/vi.json
--rw-rw-rw-   0        0        0      116 2022-04-07 08:52:22.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/vo.json
--rw-rw-rw-   0        0        0      218 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/war.json
--rw-rw-rw-   0        0        0      461 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/yi.json
--rw-rw-rw-   0        0        0      850 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/yue.json
--rw-rw-rw-   0        0        0     1084 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/zh.json
--rw-rw-rw-   0        0        0     6096 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/scripts/login.py
--rw-rw-rw-   0        0        0     3225 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/scripts/preload_sites.py
--rw-rw-rw-   0        0        0     2033 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/scripts/shell.py
--rw-rw-rw-   0        0        0     3291 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/scripts/version.py
--rw-rw-rw-   0        0        0    18351 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/scripts/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-07-05 08:35:04.263423 pywikibot-8.2.0/pywikibot/site/
--rw-rw-rw-   0        0        0      744 2023-05-16 07:53:09.000000 pywikibot-8.2.0/pywikibot/site/__init__.py
--rw-rw-rw-   0        0        0   112230 2023-07-04 16:26:14.000000 pywikibot-8.2.0/pywikibot/site/_apisite.py
--rw-rw-rw-   0        0        0    15515 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/site/_basesite.py
--rw-rw-rw-   0        0        0    38219 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/site/_datasite.py
--rw-rw-rw-   0        0        0     4254 2023-05-16 07:53:09.000000 pywikibot-8.2.0/pywikibot/site/_decorators.py
--rw-rw-rw-   0        0        0    27970 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/site/_extensions.py
--rw-rw-rw-   0        0        0    93527 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/site/_generators.py
--rw-rw-rw-   0        0        0     3003 2023-05-20 13:58:11.000000 pywikibot-8.2.0/pywikibot/site/_interwikimap.py
--rw-rw-rw-   0        0        0    14558 2023-05-16 07:53:09.000000 pywikibot-8.2.0/pywikibot/site/_namespace.py
--rw-rw-rw-   0        0        0     1595 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/site/_obsoletesites.py
--rw-rw-rw-   0        0        0    14357 2023-07-04 09:42:32.000000 pywikibot-8.2.0/pywikibot/site/_siteinfo.py
--rw-rw-rw-   0        0        0     4868 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/site/_tokenwallet.py
--rw-rw-rw-   0        0        0    25199 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/site/_upload.py
--rw-rw-rw-   0        0        0    11156 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/site_detect.py
-drwxrwxrwx   0        0        0        0 2023-07-05 08:35:04.267413 pywikibot-8.2.0/pywikibot/specialbots/
--rw-rw-rw-   0        0        0      371 2023-05-16 07:53:09.000000 pywikibot-8.2.0/pywikibot/specialbots/__init__.py
--rw-rw-rw-   0        0        0     3109 2023-05-16 07:53:09.000000 pywikibot-8.2.0/pywikibot/specialbots/_unlink.py
--rw-rw-rw-   0        0        0    20160 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/specialbots/_upload.py
--rw-rw-rw-   0        0        0    87550 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/textlib.py
--rw-rw-rw-   0        0        0    12074 2023-05-16 07:53:09.000000 pywikibot-8.2.0/pywikibot/throttle.py
--rw-rw-rw-   0        0        0    14991 2023-07-04 09:42:32.000000 pywikibot-8.2.0/pywikibot/time.py
--rw-rw-rw-   0        0        0     3267 2023-05-16 07:53:09.000000 pywikibot-8.2.0/pywikibot/titletranslate.py
-drwxrwxrwx   0        0        0        0 2023-07-05 08:35:04.285365 pywikibot-8.2.0/pywikibot/tools/
--rw-rw-rw-   0        0        0    28023 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/tools/__init__.py
--rw-rw-rw-   0        0        0    25727 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/tools/_deprecate.py
--rw-rw-rw-   0        0        0     1205 2023-05-16 07:53:09.000000 pywikibot-8.2.0/pywikibot/tools/_logging.py
--rw-rw-rw-   0        0        0    22207 2023-05-16 07:53:09.000000 pywikibot-8.2.0/pywikibot/tools/_unidata.py
--rw-rw-rw-   0        0        0     4076 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/tools/chars.py
--rw-rw-rw-   0        0        0     8765 2023-05-16 07:53:09.000000 pywikibot-8.2.0/pywikibot/tools/collections.py
--rw-rw-rw-   0        0        0    10946 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/tools/djvu.py
--rw-rw-rw-   0        0        0     4018 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/tools/formatter.py
--rw-rw-rw-   0        0        0     9866 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/tools/itertools.py
--rw-rw-rw-   0        0        0     7210 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/tools/threading.py
-drwxrwxrwx   0        0        0        0 2023-07-05 08:35:04.299327 pywikibot-8.2.0/pywikibot/userinterfaces/
--rw-rw-rw-   0        0        0      870 2023-05-16 07:53:09.000000 pywikibot-8.2.0/pywikibot/userinterfaces/__init__.py
--rw-rw-rw-   0        0        0     1906 2023-05-16 07:53:09.000000 pywikibot-8.2.0/pywikibot/userinterfaces/_interface_base.py
--rw-rw-rw-   0        0        0     2687 2023-05-16 07:53:09.000000 pywikibot-8.2.0/pywikibot/userinterfaces/buffer_interface.py
--rw-rw-rw-   0        0        0    22102 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/userinterfaces/gui.py
--rw-rw-rw-   0        0        0      457 2023-05-15 15:00:32.000000 pywikibot-8.2.0/pywikibot/userinterfaces/terminal_interface.py
--rw-rw-rw-   0        0        0    24478 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/userinterfaces/terminal_interface_base.py
--rw-rw-rw-   0        0        0     2114 2023-05-16 07:53:09.000000 pywikibot-8.2.0/pywikibot/userinterfaces/terminal_interface_unix.py
--rw-rw-rw-   0        0        0     2012 2023-05-16 07:53:09.000000 pywikibot-8.2.0/pywikibot/userinterfaces/terminal_interface_win32.py
--rw-rw-rw-   0        0        0    90310 2023-05-16 07:53:09.000000 pywikibot-8.2.0/pywikibot/userinterfaces/transliteration.py
--rw-rw-rw-   0        0        0    16654 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/version.py
--rw-rw-rw-   0        0        0     7366 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/xmlreader.py
-drwxrwxrwx   0        0        0        0 2023-07-05 08:35:03.127450 pywikibot-8.2.0/pywikibot.egg-info/
--rw-rw-rw-   0        0        0    15888 2023-07-05 08:35:02.000000 pywikibot-8.2.0/pywikibot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    10466 2023-07-05 08:35:03.000000 pywikibot-8.2.0/pywikibot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-05 08:35:02.000000 pywikibot-8.2.0/pywikibot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-07-05 08:35:02.000000 pywikibot-8.2.0/pywikibot.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0     1228 2023-07-05 08:35:02.000000 pywikibot-8.2.0/pywikibot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-05 08:35:02.000000 pywikibot-8.2.0/pywikibot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-05 08:35:04.304314 pywikibot-8.2.0/setup.cfg
--rw-rw-rw-   0        0        0    13228 2023-07-02 16:47:05.000000 pywikibot-8.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-05 08:35:04.301324 pywikibot-8.2.0/tests/
--rw-rw-rw-   0        0        0     2814 2023-07-02 16:47:05.000000 pywikibot-8.2.0/tests/tests_tests.py
+drwxrwxrwx   0        0        0        0 2023-07-27 11:03:46.386660 pywikibot-8.3.0/
+-rw-rw-rw-   0        0        0     4133 2023-07-05 09:25:16.000000 pywikibot-8.3.0/AUTHORS.rst
+-rw-rw-rw-   0        0        0      177 2023-05-16 07:53:09.000000 pywikibot-8.3.0/CODE_OF_CONDUCT.rst
+-rw-rw-rw-   0        0        0     1086 2023-05-16 07:53:09.000000 pywikibot-8.3.0/LICENSE
+-rw-rw-rw-   0        0        0       88 2023-07-05 09:25:16.000000 pywikibot-8.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    14648 2023-07-27 11:03:46.386660 pywikibot-8.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5502 2023-07-05 09:25:16.000000 pywikibot-8.3.0/README.rst
+-rw-rw-rw-   0        0        0     4959 2023-07-27 10:00:56.000000 pywikibot-8.3.0/ROADMAP.rst
+drwxrwxrwx   0        0        0        0 2023-07-27 11:03:45.259688 pywikibot-8.3.0/pywikibot/
+-rw-rw-rw-   0        0        0    14220 2023-07-27 10:00:56.000000 pywikibot-8.3.0/pywikibot/__init__.py
+-rw-rw-rw-   0        0        0      794 2023-07-27 11:01:30.000000 pywikibot-8.3.0/pywikibot/__metadata__.py
+-rw-rw-rw-   0        0        0    44088 2023-07-27 10:00:56.000000 pywikibot-8.3.0/pywikibot/_wbtypes.py
+-rw-rw-rw-   0        0        0     5655 2023-07-05 09:25:16.000000 pywikibot-8.3.0/pywikibot/backports.py
+-rw-rw-rw-   0        0        0    94724 2023-07-05 09:25:16.000000 pywikibot-8.3.0/pywikibot/bot.py
+-rw-rw-rw-   0        0        0    21197 2023-07-05 09:25:16.000000 pywikibot-8.3.0/pywikibot/bot_choice.py
+drwxrwxrwx   0        0        0        0 2023-07-27 11:03:45.309556 pywikibot-8.3.0/pywikibot/comms/
+-rw-rw-rw-   0        0        0      121 2023-05-16 07:53:09.000000 pywikibot-8.3.0/pywikibot/comms/__init__.py
+-rw-rw-rw-   0        0        0    15771 2023-07-05 09:25:16.000000 pywikibot-8.3.0/pywikibot/comms/eventstreams.py
+-rw-rw-rw-   0        0        0    20112 2023-07-27 10:00:56.000000 pywikibot-8.3.0/pywikibot/comms/http.py
+-rw-rw-rw-   0        0        0    46549 2023-07-05 09:25:16.000000 pywikibot-8.3.0/pywikibot/config.py
+-rw-rw-rw-   0        0        0    45958 2023-07-05 09:25:16.000000 pywikibot-8.3.0/pywikibot/cosmetic_changes.py
+-rw-rw-rw-   0        0        0     2090 2023-05-16 07:53:09.000000 pywikibot-8.3.0/pywikibot/daemonize.py
+drwxrwxrwx   0        0        0        0 2023-07-27 11:03:45.349449 pywikibot-8.3.0/pywikibot/data/
+-rw-rw-rw-   0        0        0      160 2023-05-16 07:53:09.000000 pywikibot-8.3.0/pywikibot/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-27 11:03:45.353438 pywikibot-8.3.0/pywikibot/data/api/
+-rw-rw-rw-   0        0        0     3174 2023-07-02 16:47:05.000000 pywikibot-8.3.0/pywikibot/data/api/__init__.py
+-rw-rw-rw-   0        0        0    41575 2023-07-05 09:25:16.000000 pywikibot-8.3.0/pywikibot/data/api/_generators.py
+-rw-rw-rw-   0        0        0     7368 2023-07-05 09:25:16.000000 pywikibot-8.3.0/pywikibot/data/api/_optionset.py
+-rw-rw-rw-   0        0        0    23238 2023-07-05 09:25:16.000000 pywikibot-8.3.0/pywikibot/data/api/_paraminfo.py
+-rw-rw-rw-   0        0        0    53439 2023-07-19 09:29:55.000000 pywikibot-8.3.0/pywikibot/data/api/_requests.py
+-rw-rw-rw-   0        0        0    14120 2023-07-05 09:25:16.000000 pywikibot-8.3.0/pywikibot/data/memento.py
+-rw-rw-rw-   0        0        0     2919 2023-05-16 07:53:09.000000 pywikibot-8.3.0/pywikibot/data/mysql.py
+-rw-rw-rw-   0        0        0     8902 2023-07-05 09:25:16.000000 pywikibot-8.3.0/pywikibot/data/sparql.py
+-rw-rw-rw-   0        0        0     3970 2023-05-16 07:53:09.000000 pywikibot-8.3.0/pywikibot/data/wikistats.py
+-rw-rw-rw-   0        0        0    96751 2023-07-16 10:09:15.000000 pywikibot-8.3.0/pywikibot/date.py
+-rw-rw-rw-   0        0        0    24902 2023-07-05 09:25:16.000000 pywikibot-8.3.0/pywikibot/diff.py
+-rw-rw-rw-   0        0        0     2042 2023-07-02 16:47:05.000000 pywikibot-8.3.0/pywikibot/echo.py
+-rw-rw-rw-   0        0        0     7918 2023-07-05 09:25:16.000000 pywikibot-8.3.0/pywikibot/editor.py
+-rw-rw-rw-   0        0        0    21189 2023-07-05 09:25:16.000000 pywikibot-8.3.0/pywikibot/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-07-27 11:03:45.512033 pywikibot-8.3.0/pywikibot/families/
+-rw-rw-rw-   0        0        0      118 2023-05-16 07:53:09.000000 pywikibot-8.3.0/pywikibot/families/__init__.py
+-rw-rw-rw-   0        0        0     1656 2023-07-05 09:25:16.000000 pywikibot-8.3.0/pywikibot/families/commons_family.py
+-rw-rw-rw-   0        0        0      443 2023-05-16 07:53:09.000000 pywikibot-8.3.0/pywikibot/families/foundation_family.py
+-rw-rw-rw-   0        0        0      338 2023-07-05 09:25:16.000000 pywikibot-8.3.0/pywikibot/families/i18n_family.py
+-rw-rw-rw-   0        0        0      355 2023-05-15 15:00:32.000000 pywikibot-8.3.0/pywikibot/families/incubator_family.py
+-rw-rw-rw-   0        0        0      583 2023-07-05 09:25:16.000000 pywikibot-8.3.0/pywikibot/families/lingualibre_family.py
+-rw-rw-rw-   0        0        0      401 2023-05-15 15:00:32.000000 pywikibot-8.3.0/pywikibot/families/mediawiki_family.py
+-rw-rw-rw-   0        0        0      593 2023-05-15 15:00:32.000000 pywikibot-8.3.0/pywikibot/families/meta_family.py
+-rw-rw-rw-   0        0        0     1205 2023-07-05 09:25:16.000000 pywikibot-8.3.0/pywikibot/families/osm_family.py
+-rw-rw-rw-   0        0        0      369 2023-05-15 15:00:32.000000 pywikibot-8.3.0/pywikibot/families/outreach_family.py
+-rw-rw-rw-   0        0        0      361 2023-05-15 15:00:32.000000 pywikibot-8.3.0/pywikibot/families/species_family.py
+-rw-rw-rw-   0        0        0      513 2023-07-05 09:25:16.000000 pywikibot-8.3.0/pywikibot/families/vikidia_family.py
+-rw-rw-rw-   0        0        0     2418 2023-07-05 09:25:16.000000 pywikibot-8.3.0/pywikibot/families/wikibooks_family.py
+-rw-rw-rw-   0        0        0      958 2023-07-05 09:25:16.000000 pywikibot-8.3.0/pywikibot/families/wikidata_family.py
+-rw-rw-rw-   0        0        0     1631 2023-07-05 09:25:16.000000 pywikibot-8.3.0/pywikibot/families/wikihow_family.py
+-rw-rw-rw-   0        0        0     1009 2023-05-15 15:00:32.000000 pywikibot-8.3.0/pywikibot/families/wikimania_family.py
+-rw-rw-rw-   0        0        0      777 2023-07-05 09:25:16.000000 pywikibot-8.3.0/pywikibot/families/wikimediachapter_family.py
+-rw-rw-rw-   0        0        0     1832 2023-07-05 09:25:16.000000 pywikibot-8.3.0/pywikibot/families/wikinews_family.py
+-rw-rw-rw-   0        0        0    10989 2023-07-27 11:01:30.000000 pywikibot-8.3.0/pywikibot/families/wikipedia_family.py
+-rw-rw-rw-   0        0        0     2886 2023-07-27 10:00:56.000000 pywikibot-8.3.0/pywikibot/families/wikiquote_family.py
+-rw-rw-rw-   0        0        0     5335 2023-07-27 10:00:56.000000 pywikibot-8.3.0/pywikibot/families/wikisource_family.py
+-rw-rw-rw-   0        0        0      431 2023-07-05 09:25:16.000000 pywikibot-8.3.0/pywikibot/families/wikispore_family.py
+-rw-rw-rw-   0        0        0      425 2023-05-16 07:53:09.000000 pywikibot-8.3.0/pywikibot/families/wikitech_family.py
+-rw-rw-rw-   0        0        0     1150 2023-07-02 16:47:05.000000 pywikibot-8.3.0/pywikibot/families/wikiversity_family.py
+-rw-rw-rw-   0        0        0     1027 2023-07-05 09:25:16.000000 pywikibot-8.3.0/pywikibot/families/wikivoyage_family.py
+-rw-rw-rw-   0        0        0     4126 2023-07-27 10:00:56.000000 pywikibot-8.3.0/pywikibot/families/wiktionary_family.py
+-rw-rw-rw-   0        0        0     2414 2023-07-05 09:25:16.000000 pywikibot-8.3.0/pywikibot/families/wowwiki_family.py
+-rw-rw-rw-   0        0        0    41747 2023-07-27 10:00:56.000000 pywikibot-8.3.0/pywikibot/family.py
+-rw-rw-rw-   0        0        0    33191 2023-05-16 07:53:09.000000 pywikibot-8.3.0/pywikibot/fixes.py
+-rw-rw-rw-   0        0        0    20119 2023-07-02 16:47:05.000000 pywikibot-8.3.0/pywikibot/flow.py
+-rw-rw-rw-   0        0        0    29992 2023-07-27 10:00:56.000000 pywikibot-8.3.0/pywikibot/i18n.py
+-rw-rw-rw-   0        0        0     8278 2023-07-05 09:25:16.000000 pywikibot-8.3.0/pywikibot/interwiki_graph.py
+-rw-rw-rw-   0        0        0    13177 2023-07-05 09:25:16.000000 pywikibot-8.3.0/pywikibot/logentries.py
+-rw-rw-rw-   0        0        0    12508 2023-05-16 07:53:09.000000 pywikibot-8.3.0/pywikibot/logging.py
+-rw-rw-rw-   0        0        0    22771 2023-07-05 09:25:16.000000 pywikibot-8.3.0/pywikibot/login.py
+drwxrwxrwx   0        0        0        0 2023-07-27 11:03:45.523969 pywikibot-8.3.0/pywikibot/page/
+-rw-rw-rw-   0        0        0     2350 2023-07-02 16:47:05.000000 pywikibot-8.3.0/pywikibot/page/__init__.py
+-rw-rw-rw-   0        0        0    86838 2023-07-05 09:25:16.000000 pywikibot-8.3.0/pywikibot/page/_basepage.py
+-rw-rw-rw-   0        0        0    14599 2023-07-05 09:25:16.000000 pywikibot-8.3.0/pywikibot/page/_category.py
+-rw-rw-rw-   0        0        0    18914 2023-07-05 09:25:16.000000 pywikibot-8.3.0/pywikibot/page/_collections.py
+-rw-rw-rw-   0        0        0     2139 2023-07-05 09:25:16.000000 pywikibot-8.3.0/pywikibot/page/_decorators.py
+-rw-rw-rw-   0        0        0    17407 2023-07-05 09:25:16.000000 pywikibot-8.3.0/pywikibot/page/_filepage.py
+-rw-rw-rw-   0        0        0    29329 2023-07-05 09:25:16.000000 pywikibot-8.3.0/pywikibot/page/_links.py
+-rw-rw-rw-   0        0        0     8515 2023-07-02 16:47:05.000000 pywikibot-8.3.0/pywikibot/page/_page.py
+-rw-rw-rw-   0        0        0     2997 2023-05-16 07:53:09.000000 pywikibot-8.3.0/pywikibot/page/_revision.py
+-rw-rw-rw-   0        0        0     4049 2023-07-02 16:47:05.000000 pywikibot-8.3.0/pywikibot/page/_toolforge.py
+-rw-rw-rw-   0        0        0    16266 2023-07-05 09:25:16.000000 pywikibot-8.3.0/pywikibot/page/_user.py
+-rw-rw-rw-   0        0        0    85875 2023-07-05 09:25:16.000000 pywikibot-8.3.0/pywikibot/page/_wikibase.py
+drwxrwxrwx   0        0        0        0 2023-07-27 11:03:45.565889 pywikibot-8.3.0/pywikibot/pagegenerators/
+-rw-rw-rw-   0        0        0    29391 2023-07-05 09:25:16.000000 pywikibot-8.3.0/pywikibot/pagegenerators/__init__.py
+-rw-rw-rw-   0        0        0    40292 2023-07-05 09:25:16.000000 pywikibot-8.3.0/pywikibot/pagegenerators/_factory.py
+-rw-rw-rw-   0        0        0    19242 2023-07-05 09:25:16.000000 pywikibot-8.3.0/pywikibot/pagegenerators/_filters.py
+-rw-rw-rw-   0        0        0    45143 2023-07-05 09:25:16.000000 pywikibot-8.3.0/pywikibot/pagegenerators/_generators.py
+-rw-rw-rw-   0        0        0     3938 2023-05-16 07:53:09.000000 pywikibot-8.3.0/pywikibot/plural.py
+-rw-rw-rw-   0        0        0    48615 2023-07-05 09:25:16.000000 pywikibot-8.3.0/pywikibot/proofreadpage.py
+drwxrwxrwx   0        0        0        0 2023-07-27 11:03:45.618746 pywikibot-8.3.0/pywikibot/scripts/
+-rw-rw-rw-   0        0        0      882 2023-05-16 07:53:09.000000 pywikibot-8.3.0/pywikibot/scripts/__init__.py
+-rw-rw-rw-   0        0        0    11922 2023-07-05 09:25:16.000000 pywikibot-8.3.0/pywikibot/scripts/generate_family_file.py
+-rw-rw-rw-   0        0        0    20021 2023-07-05 09:25:16.000000 pywikibot-8.3.0/pywikibot/scripts/generate_user_files.py
+drwxrwxrwx   0        0        0        0 2023-07-27 11:03:45.624725 pywikibot-8.3.0/pywikibot/scripts/i18n/
+-rw-rw-rw-   0        0        0      309 2023-05-16 07:53:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-27 11:03:46.259002 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/
+-rw-rw-rw-   0        0        0      166 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/ab.json
+-rw-rw-rw-   0        0        0      511 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/af.json
+-rw-rw-rw-   0        0        0      121 2022-04-07 08:52:21.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/an.json
+-rw-rw-rw-   0        0        0     1227 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/ar.json
+-rw-rw-rw-   0        0        0      131 2022-04-07 08:52:21.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/arc.json
+-rw-rw-rw-   0        0        0     1042 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/ast.json
+-rw-rw-rw-   0        0        0      163 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/av.json
+-rw-rw-rw-   0        0        0      150 2022-04-07 08:52:21.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/awa.json
+-rw-rw-rw-   0        0        0      898 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/az.json
+-rw-rw-rw-   0        0        0      982 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/azb.json
+-rw-rw-rw-   0        0        0     1362 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/ba.json
+-rw-rw-rw-   0        0        0      210 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/bar.json
+-rw-rw-rw-   0        0        0      989 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/bcc.json
+-rw-rw-rw-   0        0        0     1491 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/be-tarask.json
+-rw-rw-rw-   0        0        0      894 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/be.json
+-rw-rw-rw-   0        0        0      535 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/bg.json
+-rw-rw-rw-   0        0        0      203 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/bjn.json
+-rw-rw-rw-   0        0        0      642 2023-04-06 12:04:37.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/bn.json
+-rw-rw-rw-   0        0        0      179 2022-04-07 08:52:21.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/bo.json
+-rw-rw-rw-   0        0        0     1048 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/br.json
+-rw-rw-rw-   0        0        0      998 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/bs.json
+-rw-rw-rw-   0        0        0     1198 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/ca.json
+-rw-rw-rw-   0        0        0      981 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/ce.json
+-rw-rw-rw-   0        0        0      768 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/ckb.json
+-rw-rw-rw-   0        0        0     1178 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/cs.json
+-rw-rw-rw-   0        0        0     1013 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/csb.json
+-rw-rw-rw-   0        0        0      995 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/cy.json
+-rw-rw-rw-   0        0        0     1022 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/da.json
+-rw-rw-rw-   0        0        0     1065 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/de.json
+-rw-rw-rw-   0        0        0     1025 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/diq.json
+-rw-rw-rw-   0        0        0     1647 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/el.json
+-rw-rw-rw-   0        0        0     1027 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/en.json
+-rw-rw-rw-   0        0        0     1121 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/eo.json
+-rw-rw-rw-   0        0        0     1203 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/es.json
+-rw-rw-rw-   0        0        0      333 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/et.json
+-rw-rw-rw-   0        0        0     1043 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/eu.json
+-rw-rw-rw-   0        0        0     1424 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/fa.json
+-rw-rw-rw-   0        0        0      713 2023-07-21 09:20:07.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/fi.json
+-rw-rw-rw-   0        0        0      812 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/fo.json
+-rw-rw-rw-   0        0        0     1291 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/fr.json
+-rw-rw-rw-   0        0        0      227 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/frp.json
+-rw-rw-rw-   0        0        0      988 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/frr.json
+-rw-rw-rw-   0        0        0       95 2022-04-07 08:52:21.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/fy.json
+-rw-rw-rw-   0        0        0      104 2022-04-07 08:52:21.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/ga.json
+-rw-rw-rw-   0        0        0     1083 2023-07-21 09:20:07.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/gl.json
+-rw-rw-rw-   0        0        0      786 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/gsw.json
+-rw-rw-rw-   0        0        0      711 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/hak.json
+-rw-rw-rw-   0        0        0      858 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/haw.json
+-rw-rw-rw-   0        0        0     1192 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/he.json
+-rw-rw-rw-   0        0        0     1699 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/hi.json
+-rw-rw-rw-   0        0        0      201 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/hr.json
+-rw-rw-rw-   0        0        0      593 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/hsb.json
+-rw-rw-rw-   0        0        0     1022 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/hu.json
+-rw-rw-rw-   0        0        0      259 2022-04-15 15:42:25.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/hy.json
+-rw-rw-rw-   0        0        0     1085 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/ia.json
+-rw-rw-rw-   0        0        0     1146 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/id.json
+-rw-rw-rw-   0        0        0      205 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/ie.json
+-rw-rw-rw-   0        0        0      114 2022-04-07 08:52:21.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/ig.json
+-rw-rw-rw-   0        0        0      220 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/ilo.json
+-rw-rw-rw-   0        0        0     1011 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/io.json
+-rw-rw-rw-   0        0        0      735 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/is.json
+-rw-rw-rw-   0        0        0     1063 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/it.json
+-rw-rw-rw-   0        0        0     1125 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/ja.json
+-rw-rw-rw-   0        0        0      196 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/jv.json
+-rw-rw-rw-   0        0        0      581 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/kab.json
+-rw-rw-rw-   0        0        0     1079 2023-07-21 09:20:07.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/kk.json
+-rw-rw-rw-   0        0        0     1381 2022-04-07 08:52:21.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/km.json
+-rw-rw-rw-   0        0        0      993 2022-04-07 08:52:21.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/kn.json
+-rw-rw-rw-   0        0        0     1140 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/ko.json
+-rw-rw-rw-   0        0        0     1409 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/krc.json
+-rw-rw-rw-   0        0        0     1188 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/ksh.json
+-rw-rw-rw-   0        0        0      318 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/ku.json
+-rw-rw-rw-   0        0        0      331 2022-04-07 08:52:21.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/ky.json
+-rw-rw-rw-   0        0        0      100 2022-04-07 08:52:21.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/la.json
+-rw-rw-rw-   0        0        0      988 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/lb.json
+-rw-rw-rw-   0        0        0      209 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/li.json
+-rw-rw-rw-   0        0        0      174 2022-04-07 08:52:21.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/lki.json
+-rw-rw-rw-   0        0        0      963 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/lt.json
+-rw-rw-rw-   0        0        0      691 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/lv.json
+-rw-rw-rw-   0        0        0      752 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/map-bms.json
+-rw-rw-rw-   0        0        0      967 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/mg.json
+-rw-rw-rw-   0        0        0      673 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/min.json
+-rw-rw-rw-   0        0        0     1360 2023-07-21 09:20:07.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/mk.json
+-rw-rw-rw-   0        0        0     1943 2022-04-28 20:36:36.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/ml.json
+-rw-rw-rw-   0        0        0      168 2022-04-07 08:52:21.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/mni.json
+-rw-rw-rw-   0        0        0      267 2022-04-15 15:42:25.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/mr.json
+-rw-rw-rw-   0        0        0      968 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/ms.json
+-rw-rw-rw-   0        0        0      203 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/mt.json
+-rw-rw-rw-   0        0        0     1335 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/my.json
+-rw-rw-rw-   0        0        0     1049 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/nan.json
+-rw-rw-rw-   0        0        0     1003 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/nb.json
+-rw-rw-rw-   0        0        0      983 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/nds-nl.json
+-rw-rw-rw-   0        0        0      197 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/nds.json
+-rw-rw-rw-   0        0        0     1562 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/ne.json
+-rw-rw-rw-   0        0        0      891 2022-04-07 08:52:21.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/new.json
+-rw-rw-rw-   0        0        0     1037 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/nl.json
+-rw-rw-rw-   0        0        0      232 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/nn.json
+-rw-rw-rw-   0        0        0     1443 2023-07-21 09:20:07.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/nqo.json
+-rw-rw-rw-   0        0        0      148 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/nyn.json
+-rw-rw-rw-   0        0        0      226 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/oc.json
+-rw-rw-rw-   0        0        0      258 2022-04-07 08:52:21.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/olo.json
+-rw-rw-rw-   0        0        0      154 2022-04-07 08:52:21.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/or.json
+-rw-rw-rw-   0        0        0      216 2022-04-07 08:52:21.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/pa.json
+-rw-rw-rw-   0        0        0      157 2023-04-06 12:04:37.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/pdc.json
+-rw-rw-rw-   0        0        0      150 2023-07-21 09:20:07.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/pfl.json
+-rw-rw-rw-   0        0        0     1011 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/pl.json
+-rw-rw-rw-   0        0        0      870 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/pms.json
+-rw-rw-rw-   0        0        0     1070 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/pt-br.json
+-rw-rw-rw-   0        0        0     1187 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/pt.json
+-rw-rw-rw-   0        0        0     1749 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/qqq.json
+-rw-rw-rw-   0        0        0     1149 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/ro.json
+-rw-rw-rw-   0        0        0     1582 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/ru.json
+-rw-rw-rw-   0        0        0      149 2022-04-07 08:52:21.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/scn.json
+-rw-rw-rw-   0        0        0      749 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/sco.json
+-rw-rw-rw-   0        0        0      369 2023-07-21 09:20:07.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/sd.json
+-rw-rw-rw-   0        0        0      551 2022-04-07 08:52:21.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/sh.json
+-rw-rw-rw-   0        0        0      528 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/si.json
+-rw-rw-rw-   0        0        0     1046 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/sk.json
+-rw-rw-rw-   0        0        0      193 2023-04-06 12:04:37.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/skr-arab.json
+-rw-rw-rw-   0        0        0     1078 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/sl.json
+-rw-rw-rw-   0        0        0      127 2022-04-07 08:52:21.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/sms.json
+-rw-rw-rw-   0        0        0      725 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/so.json
+-rw-rw-rw-   0        0        0      452 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/sq.json
+-rw-rw-rw-   0        0        0     1439 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/sr.json
+-rw-rw-rw-   0        0        0      347 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/su.json
+-rw-rw-rw-   0        0        0     1047 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/sv.json
+-rw-rw-rw-   0        0        0      650 2022-04-07 08:52:21.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/sw.json
+-rw-rw-rw-   0        0        0      124 2022-04-07 08:52:21.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/szl.json
+-rw-rw-rw-   0        0        0      683 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/ta.json
+-rw-rw-rw-   0        0        0     1390 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/te.json
+-rw-rw-rw-   0        0        0      116 2023-07-21 09:20:07.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/tg.json
+-rw-rw-rw-   0        0        0     1414 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/th.json
+-rw-rw-rw-   0        0        0      170 2023-07-21 09:20:07.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/tk.json
+-rw-rw-rw-   0        0        0      219 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/tl.json
+-rw-rw-rw-   0        0        0     1126 2023-07-21 09:20:07.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/tly.json
+-rw-rw-rw-   0        0        0     1159 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/tr.json
+-rw-rw-rw-   0        0        0      316 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/tt.json
+-rw-rw-rw-   0        0        0     1417 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/uk.json
+-rw-rw-rw-   0        0        0      789 2022-04-28 20:36:36.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/ur.json
+-rw-rw-rw-   0        0        0      208 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/uz.json
+-rw-rw-rw-   0        0        0      253 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/vec.json
+-rw-rw-rw-   0        0        0      121 2022-04-07 08:52:22.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/vep.json
+-rw-rw-rw-   0        0        0     1105 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/vi.json
+-rw-rw-rw-   0        0        0      116 2022-04-07 08:52:22.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/vo.json
+-rw-rw-rw-   0        0        0      218 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/war.json
+-rw-rw-rw-   0        0        0      461 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/yi.json
+-rw-rw-rw-   0        0        0      850 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/yue.json
+-rw-rw-rw-   0        0        0     1084 2023-04-01 15:38:09.000000 pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/zh.json
+-rw-rw-rw-   0        0        0     6096 2023-07-05 09:25:16.000000 pywikibot-8.3.0/pywikibot/scripts/login.py
+-rw-rw-rw-   0        0        0     3225 2023-07-05 09:25:16.000000 pywikibot-8.3.0/pywikibot/scripts/preload_sites.py
+-rw-rw-rw-   0        0        0     2033 2023-07-05 09:25:16.000000 pywikibot-8.3.0/pywikibot/scripts/shell.py
+-rw-rw-rw-   0        0        0     3291 2023-07-05 09:25:16.000000 pywikibot-8.3.0/pywikibot/scripts/version.py
+-rw-rw-rw-   0        0        0    18351 2023-07-05 09:25:16.000000 pywikibot-8.3.0/pywikibot/scripts/wrapper.py
+drwxrwxrwx   0        0        0        0 2023-07-27 11:03:46.276955 pywikibot-8.3.0/pywikibot/site/
+-rw-rw-rw-   0        0        0      744 2023-07-16 09:54:58.000000 pywikibot-8.3.0/pywikibot/site/__init__.py
+-rw-rw-rw-   0        0        0   112230 2023-07-05 09:25:16.000000 pywikibot-8.3.0/pywikibot/site/_apisite.py
+-rw-rw-rw-   0        0        0    15515 2023-07-05 09:25:16.000000 pywikibot-8.3.0/pywikibot/site/_basesite.py
+-rw-rw-rw-   0        0        0    38219 2023-07-05 09:25:16.000000 pywikibot-8.3.0/pywikibot/site/_datasite.py
+-rw-rw-rw-   0        0        0     4254 2023-05-16 07:53:09.000000 pywikibot-8.3.0/pywikibot/site/_decorators.py
+-rw-rw-rw-   0        0        0    27970 2023-07-05 09:25:16.000000 pywikibot-8.3.0/pywikibot/site/_extensions.py
+-rw-rw-rw-   0        0        0    93527 2023-07-05 09:25:16.000000 pywikibot-8.3.0/pywikibot/site/_generators.py
+-rw-rw-rw-   0        0        0     3003 2023-05-20 13:58:11.000000 pywikibot-8.3.0/pywikibot/site/_interwikimap.py
+-rw-rw-rw-   0        0        0    14558 2023-05-16 07:53:09.000000 pywikibot-8.3.0/pywikibot/site/_namespace.py
+-rw-rw-rw-   0        0        0     1595 2023-07-05 09:25:16.000000 pywikibot-8.3.0/pywikibot/site/_obsoletesites.py
+-rw-rw-rw-   0        0        0    14357 2023-07-05 18:58:30.000000 pywikibot-8.3.0/pywikibot/site/_siteinfo.py
+-rw-rw-rw-   0        0        0     4868 2023-07-02 16:47:05.000000 pywikibot-8.3.0/pywikibot/site/_tokenwallet.py
+-rw-rw-rw-   0        0        0    25199 2023-07-05 09:25:16.000000 pywikibot-8.3.0/pywikibot/site/_upload.py
+-rw-rw-rw-   0        0        0    11156 2023-07-02 16:47:05.000000 pywikibot-8.3.0/pywikibot/site_detect.py
+drwxrwxrwx   0        0        0        0 2023-07-27 11:03:46.305876 pywikibot-8.3.0/pywikibot/specialbots/
+-rw-rw-rw-   0        0        0      371 2023-05-16 07:53:09.000000 pywikibot-8.3.0/pywikibot/specialbots/__init__.py
+-rw-rw-rw-   0        0        0     3109 2023-05-16 07:53:09.000000 pywikibot-8.3.0/pywikibot/specialbots/_unlink.py
+-rw-rw-rw-   0        0        0    20160 2023-07-05 09:25:16.000000 pywikibot-8.3.0/pywikibot/specialbots/_upload.py
+-rw-rw-rw-   0        0        0    87526 2023-07-27 10:00:56.000000 pywikibot-8.3.0/pywikibot/textlib.py
+-rw-rw-rw-   0        0        0    12074 2023-05-16 07:53:09.000000 pywikibot-8.3.0/pywikibot/throttle.py
+-rw-rw-rw-   0        0        0    14991 2023-07-05 09:25:16.000000 pywikibot-8.3.0/pywikibot/time.py
+-rw-rw-rw-   0        0        0     3267 2023-05-16 07:53:09.000000 pywikibot-8.3.0/pywikibot/titletranslate.py
+drwxrwxrwx   0        0        0        0 2023-07-27 11:03:46.335796 pywikibot-8.3.0/pywikibot/tools/
+-rw-rw-rw-   0        0        0    28023 2023-07-05 09:25:16.000000 pywikibot-8.3.0/pywikibot/tools/__init__.py
+-rw-rw-rw-   0        0        0    25727 2023-07-05 09:25:16.000000 pywikibot-8.3.0/pywikibot/tools/_deprecate.py
+-rw-rw-rw-   0        0        0     1205 2023-05-16 07:53:09.000000 pywikibot-8.3.0/pywikibot/tools/_logging.py
+-rw-rw-rw-   0        0        0    22207 2023-05-16 07:53:09.000000 pywikibot-8.3.0/pywikibot/tools/_unidata.py
+-rw-rw-rw-   0        0        0     4076 2023-07-05 09:25:16.000000 pywikibot-8.3.0/pywikibot/tools/chars.py
+-rw-rw-rw-   0        0        0     8765 2023-05-16 07:53:09.000000 pywikibot-8.3.0/pywikibot/tools/collections.py
+-rw-rw-rw-   0        0        0    10946 2023-07-05 09:25:16.000000 pywikibot-8.3.0/pywikibot/tools/djvu.py
+-rw-rw-rw-   0        0        0     4018 2023-07-05 09:25:16.000000 pywikibot-8.3.0/pywikibot/tools/formatter.py
+-rw-rw-rw-   0        0        0     9866 2023-07-05 09:25:16.000000 pywikibot-8.3.0/pywikibot/tools/itertools.py
+-rw-rw-rw-   0        0        0     7210 2023-07-08 12:42:13.000000 pywikibot-8.3.0/pywikibot/tools/threading.py
+drwxrwxrwx   0        0        0        0 2023-07-27 11:03:46.374693 pywikibot-8.3.0/pywikibot/userinterfaces/
+-rw-rw-rw-   0        0        0      870 2023-05-16 07:53:09.000000 pywikibot-8.3.0/pywikibot/userinterfaces/__init__.py
+-rw-rw-rw-   0        0        0     1906 2023-05-16 07:53:09.000000 pywikibot-8.3.0/pywikibot/userinterfaces/_interface_base.py
+-rw-rw-rw-   0        0        0     2687 2023-05-16 07:53:09.000000 pywikibot-8.3.0/pywikibot/userinterfaces/buffer_interface.py
+-rw-rw-rw-   0        0        0    22102 2023-07-05 09:25:16.000000 pywikibot-8.3.0/pywikibot/userinterfaces/gui.py
+-rw-rw-rw-   0        0        0      457 2023-05-15 15:00:32.000000 pywikibot-8.3.0/pywikibot/userinterfaces/terminal_interface.py
+-rw-rw-rw-   0        0        0    24478 2023-07-05 09:25:16.000000 pywikibot-8.3.0/pywikibot/userinterfaces/terminal_interface_base.py
+-rw-rw-rw-   0        0        0     2114 2023-05-16 07:53:09.000000 pywikibot-8.3.0/pywikibot/userinterfaces/terminal_interface_unix.py
+-rw-rw-rw-   0        0        0     2012 2023-05-16 07:53:09.000000 pywikibot-8.3.0/pywikibot/userinterfaces/terminal_interface_win32.py
+-rw-rw-rw-   0        0        0    90310 2023-05-16 07:53:09.000000 pywikibot-8.3.0/pywikibot/userinterfaces/transliteration.py
+-rw-rw-rw-   0        0        0    16654 2023-07-05 09:25:16.000000 pywikibot-8.3.0/pywikibot/version.py
+-rw-rw-rw-   0        0        0     7366 2023-07-02 16:47:05.000000 pywikibot-8.3.0/pywikibot/xmlreader.py
+drwxrwxrwx   0        0        0        0 2023-07-27 11:03:45.294596 pywikibot-8.3.0/pywikibot.egg-info/
+-rw-rw-rw-   0        0        0    14648 2023-07-27 11:03:45.000000 pywikibot-8.3.0/pywikibot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    10466 2023-07-27 11:03:45.000000 pywikibot-8.3.0/pywikibot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 11:03:45.000000 pywikibot-8.3.0/pywikibot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-07-27 11:03:45.000000 pywikibot-8.3.0/pywikibot.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0     1228 2023-07-27 11:03:45.000000 pywikibot-8.3.0/pywikibot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-27 11:03:45.000000 pywikibot-8.3.0/pywikibot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-27 11:03:46.386660 pywikibot-8.3.0/setup.cfg
+-rw-rw-rw-   0        0        0    13228 2023-07-09 14:54:24.000000 pywikibot-8.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 11:03:46.384665 pywikibot-8.3.0/tests/
+-rw-rw-rw-   0        0        0     2814 2023-07-02 16:47:05.000000 pywikibot-8.3.0/tests/tests_tests.py
```

### Comparing `pywikibot-8.2.0/AUTHORS.rst` & `pywikibot-8.3.0/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/LICENSE` & `pywikibot-8.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/PKG-INFO` & `pywikibot-8.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywikibot
-Version: 8.2.0
+Version: 8.3.0
 Summary: Python MediaWiki Bot Framework
 Home-page: https://www.mediawiki.org/wiki/Manual:Pywikibot
 Download-URL: https://pywikibot.toolforge.org/
 Maintainer: The Pywikibot team
 Maintainer-email: pywikibot@lists.wikimedia.org
 License: MIT License
 Project-URL: Documentation, https://doc.wikimedia.org/pywikibot/stable/
@@ -257,36 +257,19 @@
 
 Roadmap
 =======
 
 Current release
 ---------------
 
-* Add support for gpewiki (T335989)
-* family.WikibaseFamilyand family.DefaultWikibaseFamilywere added to familymodule
-* Remove incorrect time normalization in page.Claim(T338748, T325860, T57755)
-* Add support for other types of diffs in Site.compare()
-* Improvements for textlib.extract_sectionsfunction (T338748)
-* Backport ``itertools.batched()`` from Python 3.12 which replaces tools.itertools.itergroup
-* Upcast page types in pagegenerators.RecentChangesPageGenerator(T340450)
-* Enable FilePage.download()to download thumbnails (T247095)
-* Refactor tools.compute_file_hashand use ``hashlib.file_digest`` with Python 3.11
-* Url ends with curly bracket in textlib.compileLinkR(T338029)
-* Allows spaces in environment variables for editor.TextEditor(T102465, T323078)
-* Add textlib.get_regexespublic function (T336144)
-* Return 'https' scheme with family.Family.protocol(T326046)
-* Use ``build`` instead of ``setuptools.setup()`` to build the distribution
-* Raise ``ConnectionError`` on ``requests.ReadTimeout`` in comms.http.error_handling_callback
-* Raise exceptions.ServerErroron ``requests.ReadTimeout`` in comms.http.error_handling_callback
-* Do not evaluate pywikibot.Sitewith dict.pop() as default value (T335720)
-* L10N updates
-* family.Familyclass was rewritten. ``obsolete.setter`` was removed,
-  family.Family.interwiki_replacementsreturns an invariant mapping,
-  family.Family.interwiki_removalsreturns a frozenset. ``closed_wikis``,
-  ``removed_wikis`` and ``code_aliases`` are family.Familyclass attributes.  (T334834)
+* Add support for btmwiktionary (T336117)
+* Add 'yue'/'zh-yue' code_aliases to family files (T341960)
+* All wbtypes are placed in ``pywkibot._wbtypes`` module
+* Use ``site.lang`` instead of ``site.code`` in comms.http.user_agent(T228322)
+* Make header extraction in textlib.extract_sectionsmore robust (T341787)
 
 
 Deprecations
 ------------
 
 * 8.2.0: *normalize* parameter of WbTime.toTimestrand WbTime.toWikibasewill be removed
 * 8.1.0: Dependency of exceptions.NoSiteLinkErrorfrom exceptions.NoPageErrorwill be removed
```

### Comparing `pywikibot-8.2.0/README.rst` & `pywikibot-8.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/ROADMAP.rst` & `pywikibot-8.3.0/ROADMAP.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,15 @@
 Current release
 ---------------
 
-* Add support for gpewiki (:phab:`T335989`)
-* :class:`family.WikibaseFamily` and :class:`family.DefaultWikibaseFamily` were added to :mod:`family` module
-* Remove incorrect time normalization in :class:`page.Claim` (:phab:`T338748`, :phab:`T325860`, :phab:`T57755`)
-* Add support for other types of diffs in :meth:`Site.compare()<pywikibot.site._apisite.APISite.compare>`
-* Improvements for :func:`textlib.extract_sections` function (:phab:`T338748`)
-* Backport ``itertools.batched()`` from Python 3.12 which replaces :func:`tools.itertools.itergroup`
-* Upcast page types in :func:`pagegenerators.RecentChangesPageGenerator` (:phab:`T340450`)
-* Enable :meth:`FilePage.download()<pywikibot.FilePage.download>` to download thumbnails (:phab:`T247095`)
-* Refactor :func:`tools.compute_file_hash` and use ``hashlib.file_digest`` with Python 3.11
-* Url ends with curly bracket in :func:`textlib.compileLinkR` (:phab:`T338029`)
-* Allows spaces in environment variables for :class:`editor.TextEditor` (:phab:`T102465`, :phab:`T323078`)
-* Add :func:`textlib.get_regexes` public function (:phab:`T336144`)
-* Return 'https' scheme with :meth:`family.Family.protocol` (:phab:`T326046`)
-* Use ``build`` instead of ``setuptools.setup()`` to build the distribution
-* Raise ``ConnectionError`` on ``requests.ReadTimeout`` in :func:`comms.http.error_handling_callback`
-* Raise :exc:`exceptions.ServerError` on ``requests.ReadTimeout`` in :func:`comms.http.error_handling_callback`
-* Do not evaluate :func:`pywikibot.Site` with dict.pop() as default value (:phab:`T335720`)
-* L10N updates
-* :class:`family.Family` class was rewritten. ``obsolete.setter`` was removed,
-  :meth:`family.Family.interwiki_replacements` returns an invariant mapping,
-  :meth:`family.Family.interwiki_removals` returns a frozenset. ``closed_wikis``,
-  ``removed_wikis`` and ``code_aliases`` are :class:`family.Family` class attributes.  (:phab:`T334834`)
+* Add support for btmwiktionary (:phab:`T336117`)
+* Add 'yue'/'zh-yue' code_aliases to family files (:phab:`T341960`)
+* All wbtypes are placed in ``pywkibot._wbtypes`` module
+* Use ``site.lang`` instead of ``site.code`` in :func:`comms.http.user_agent` (:phab:`T228322`)
+* Make header extraction in :func:`textlib.extract_sections` more robust (:phab:`T341787`)
 
 
 Deprecations
 ------------
 
 * 8.2.0: *normalize* parameter of :meth:`WbTime.toTimestr` and :meth:`WbTime.toWikibase` will be removed
 * 8.1.0: Dependency of :exc:`exceptions.NoSiteLinkError` from :exc:`exceptions.NoPageError` will be removed
```

### Comparing `pywikibot-8.2.0/pywikibot/__metadata__.py` & `pywikibot-8.3.0/pywikibot/__metadata__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #
 # Distributed under the terms of the MIT license.
 #
 from time import strftime
 
 
 __name__ = 'pywikibot'
-__version__ = '8.2.0'
+__version__ = '8.3.0'
 __description__ = 'Python MediaWiki Bot Framework'
 __maintainer__ = 'The Pywikibot team'
 __maintainer_email__ = 'pywikibot@lists.wikimedia.org'
 __license__ = 'MIT License'
 __url__ = 'https://www.mediawiki.org/wiki/Manual:Pywikibot'
 __download_url__ = 'https://pywikibot.toolforge.org/'
 __copyright__ = '(C) Pywikibot team, 2003-' + strftime('%Y')
```

### Comparing `pywikibot-8.2.0/pywikibot/backports.py` & `pywikibot-8.3.0/pywikibot/backports.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/bot.py` & `pywikibot-8.3.0/pywikibot/bot.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/bot_choice.py` & `pywikibot-8.3.0/pywikibot/bot_choice.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/comms/eventstreams.py` & `pywikibot-8.3.0/pywikibot/comms/eventstreams.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/comms/http.py` & `pywikibot-8.3.0/pywikibot/comms/http.py`

 * *Files 5% similar despite different names*

```diff
@@ -184,51 +184,49 @@
         # allow a useragent in the username to allow through a hand-coded
         # percent-encoded value.
         if '%' in username:
             username = quote(username)
     return username
 
 
-def user_agent(site=None, format_string: str = None) -> str:
-    """
-    Generate the user agent string for a given site and format.
-
-    :param site: The site for which this user agent is intended. May be None.
-    :type site: BaseSite
-    :param format_string: The string to which the values will be added using
-        str.format. Is using config.user_agent_format when it is None.
+def user_agent(site: Optional['pywikibot.site.BaseSite'] = None,
+               format_string: str = '') -> str:
+    """Generate the user agent string for a given site and format.
+
+    :param site: The site for which this user agent is intended. May be
+        None.
+    :param format_string: The string to which the values will be added
+        using str.format. Is using config.user_agent_format when it is
+        empty.
     :return: The formatted user agent
     """
     values = USER_AGENT_PRODUCTS.copy()
     values.update(dict.fromkeys(['script', 'script_product'],
                                 pywikibot.bot.calledModuleName()))
+    values.update(dict.fromkeys(['family', 'code', 'lang', 'site'], ''))
 
     script_comments = []
     if config.user_agent_description:
         script_comments.append(config.user_agent_description)
 
-    values['family'] = ''
-    values['code'] = ''
-    values['lang'] = ''  # TODO: use site.lang, if known
-    values['site'] = ''
-
     username = ''
     if site:
         script_comments.append(str(site))
 
         # TODO: there are several ways of identifying a user, and username
         # is not the best for a HTTP header if the username isn't ASCII.
         if site.username():
             username = user_agent_username(site.username())
             script_comments.append('User:' + username)
 
         values.update({
             'family': site.family.name,
             'code': site.code,
-            'lang': site.code,  # TODO: use site.lang, if known
+            'lang': (site.lang if site.siteinfo.is_cached('lang')
+                     else f'({site.code})'),
             'site': str(site),
         })
 
     values['username'] = username
     values['script_comments'] = '; '.join(script_comments)
 
     format_string = format_string or config.user_agent_format
```

### Comparing `pywikibot-8.2.0/pywikibot/config.py` & `pywikibot-8.3.0/pywikibot/config.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/cosmetic_changes.py` & `pywikibot-8.3.0/pywikibot/cosmetic_changes.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/daemonize.py` & `pywikibot-8.3.0/pywikibot/daemonize.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/data/api/__init__.py` & `pywikibot-8.3.0/pywikibot/data/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/data/api/_generators.py` & `pywikibot-8.3.0/pywikibot/data/api/_generators.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/data/api/_optionset.py` & `pywikibot-8.3.0/pywikibot/data/api/_optionset.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/data/api/_paraminfo.py` & `pywikibot-8.3.0/pywikibot/data/api/_paraminfo.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/data/api/_requests.py` & `pywikibot-8.3.0/pywikibot/data/api/_requests.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/data/memento.py` & `pywikibot-8.3.0/pywikibot/data/memento.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/data/mysql.py` & `pywikibot-8.3.0/pywikibot/data/mysql.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/data/sparql.py` & `pywikibot-8.3.0/pywikibot/data/sparql.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/data/wikistats.py` & `pywikibot-8.3.0/pywikibot/data/wikistats.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/date.py` & `pywikibot-8.3.0/pywikibot/date.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/diff.py` & `pywikibot-8.3.0/pywikibot/diff.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/echo.py` & `pywikibot-8.3.0/pywikibot/echo.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/editor.py` & `pywikibot-8.3.0/pywikibot/editor.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/exceptions.py` & `pywikibot-8.3.0/pywikibot/exceptions.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/families/commons_family.py` & `pywikibot-8.3.0/pywikibot/families/commons_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/families/lingualibre_family.py` & `pywikibot-8.3.0/pywikibot/families/lingualibre_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/families/meta_family.py` & `pywikibot-8.3.0/pywikibot/families/meta_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/families/osm_family.py` & `pywikibot-8.3.0/pywikibot/families/osm_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/families/vikidia_family.py` & `pywikibot-8.3.0/pywikibot/families/vikidia_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/families/wikibooks_family.py` & `pywikibot-8.3.0/pywikibot/families/wikibooks_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/families/wikidata_family.py` & `pywikibot-8.3.0/pywikibot/families/wikidata_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/families/wikihow_family.py` & `pywikibot-8.3.0/pywikibot/families/wikihow_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/families/wikimania_family.py` & `pywikibot-8.3.0/pywikibot/families/wikimania_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/families/wikimediachapter_family.py` & `pywikibot-8.3.0/pywikibot/families/wikimediachapter_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/families/wikinews_family.py` & `pywikibot-8.3.0/pywikibot/families/wikinews_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/families/wikipedia_family.py` & `pywikibot-8.3.0/pywikibot/families/wikipedia_family.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,44 +24,43 @@
         # https://noc.wikimedia.org/conf/highlight.php?file=dblists/deleted.dblist
         'dk', 'mo', 'ru-sib', 'tlh', 'tokipona', 'zh_cn', 'zh_tw',
     ]
 
     languages_by_size = [
         'en', 'ceb', 'de', 'sv', 'fr', 'nl', 'ru', 'es', 'it', 'arz', 'pl',
         'ja', 'zh', 'vi', 'uk', 'war', 'ar', 'pt', 'fa', 'ca', 'sr', 'id',
-        'ko', 'no', 'ce', 'fi', 'cs', 'hu', 'tr', 'tt', 'sh', 'ro',
+        'ko', 'no', 'ce', 'fi', 'cs', 'tr', 'hu', 'tt', 'sh', 'ro',
         'zh-min-nan', 'eu', 'ms', 'eo', 'he', 'hy', 'da', 'bg', 'cy', 'sk',
-        'azb', 'uz', 'et', 'kk', 'simple', 'be', 'min', 'el', 'hr', 'lt', 'gl',
-        'az', 'ur', 'sl', 'ka', 'lld', 'nn', 'hi', 'th', 'ta', 'bn', 'la',
-        'mk', 'zh-yue', 'ast', 'lv', 'tg', 'af', 'my', 'mg', 'mr', 'bs', 'sq',
-        'oc', 'nds', 'te', 'ml', 'be-tarask', 'br', 'ky', 'sw', 'jv', 'new',
+        'azb', 'uz', 'et', 'simple', 'kk', 'be', 'min', 'el', 'hr', 'lt', 'gl',
+        'az', 'ur', 'sl', 'lld', 'ka', 'nn', 'hi', 'th', 'ta', 'bn', 'la',
+        'mk', 'zh-yue', 'ast', 'lv', 'tg', 'af', 'my', 'mg', 'mr', 'sq', 'bs',
+        'oc', 'te', 'nds', 'ml', 'be-tarask', 'br', 'ky', 'sw', 'jv', 'new',
         'lmo', 'pnb', 'vec', 'ht', 'pms', 'ba', 'lb', 'su', 'ku', 'ga', 'szl',
-        'is', 'fy', 'cv', 'pa', 'ckb', 'tl', 'an', 'wuu', 'diq', 'io', 'sco',
-        'vo', 'yo', 'ne', 'ia', 'gu', 'kn', 'als', 'avk', 'ha', 'bar', 'scn',
-        'crh', 'bpy', 'qu', 'nv', 'mn', 'xmf', 'ban', 'si', 'ps', 'frr',
-        'bat-smg', 'os', 'or', 'sah', 'mzn', 'cdo', 'ig', 'gd', 'bug', 'tum',
-        'yi', 'sd', 'ilo', 'am', 'nap', 'li', 'fo', 'gor', 'bcl', 'hsb',
-        'map-bms', 'mai', 'shn', 'eml', 'ace', 'zh-classical', 'sa', 'as',
-        'wa', 'ie', 'lij', 'zu', 'mhr', 'hyw', 'hif', 'sn', 'mrj', 'bjn',
-        'mni', 'km', 'hak', 'so', 'roa-tara', 'pam', 'rue', 'sat', 'nso', 'bh',
-        'se', 'mi', 'myv', 'vls', 'nds-nl', 'sc', 'dag', 'kw', 'vep', 'glk',
-        'bo', 'ary', 'co', 'tk', 'kab', 'gan', 'rw', 'fiu-vro', 'ab', 'gv',
-        'ug', 'nah', 'zea', 'skr', 'frp', 'udm', 'pcd', 'kv', 'mt', 'csb',
-        'gn', 'smn', 'ay', 'nrm', 'ks', 'lez', 'lfn', 'olo', 'mwl', 'stq',
-        'lo', 'ang', 'fur', 'rm', 'mdf', 'lad', 'gom', 'ext', 'kaa', 'tyv',
-        'koi', 'dsb', 'av', 'pap', 'ln', 'dty', 'tw', 'cbk-zam', 'dv', 'ksh',
-        'za', 'gag', 'bxr', 'pfl', 'lg', 'szy', 'pag', 'pi', 'tay', 'blk',
-        'haw', 'awa', 'inh', 'krc', 'xal', 'pdc', 'to', 'atj', 'tcy', 'arc',
-        'mnw', 'jam', 'kbp', 'wo', 'anp', 'kbd', 'nia', 'shi', 'nov', 'ki',
-        'nqo', 'bi', 'tpi', 'tet', 'xh', 'om', 'roa-rup', 'jbo', 'fj', 'lbe',
-        'kg', 'ty', 'guw', 'cu', 'trv', 'ami', 'ff', 'srn', 'sm', 'alt', 'gcr',
-        'chr', 'tn', 'mad', 'ltg', 'ny', 'st', 'pih', 'got', 'rmy', 'ee', 'bm',
-        'ss', 'pcm', 've', 'ts', 'chy', 'kcg', 'rn', 'gur', 'ch', 'ik', 'pnt',
-        'ady', 'fat', 'guc', 'iu', 'pwn', 'sg', 'din', 'ti', 'kl', 'dz', 'cr',
-        'gpe',
+        'is', 'fy', 'cv', 'ckb', 'pa', 'tl', 'an', 'wuu', 'diq', 'io', 'sco',
+        'vo', 'yo', 'ne', 'ia', 'gu', 'kn', 'als', 'ha', 'avk', 'bar', 'scn',
+        'crh', 'bpy', 'qu', 'nv', 'mn', 'xmf', 'ban', 'si', 'tum', 'ps', 'frr',
+        'os', 'bat-smg', 'or', 'sah', 'ig', 'mzn', 'cdo', 'gd', 'bug', 'yi',
+        'sd', 'ilo', 'am', 'nap', 'li', 'bcl', 'fo', 'gor', 'hsb', 'map-bms',
+        'mai', 'shn', 'eml', 'ace', 'zh-classical', 'sa', 'as', 'wa', 'ie',
+        'lij', 'hyw', 'mhr', 'zu', 'sn', 'hif', 'mrj', 'bjn', 'mni', 'km',
+        'hak', 'roa-tara', 'pam', 'rue', 'sat', 'nso', 'bh', 'so', 'se', 'mi',
+        'myv', 'vls', 'nds-nl', 'sc', 'dag', 'kw', 'bo', 'vep', 'co', 'ary',
+        'glk', 'tk', 'kab', 'gan', 'rw', 'fiu-vro', 'ab', 'gv', 'ug', 'nah',
+        'zea', 'skr', 'frp', 'udm', 'pcd', 'kv', 'mt', 'csb', 'gn', 'smn',
+        'ay', 'nrm', 'ks', 'lez', 'lfn', 'olo', 'mwl', 'stq', 'lo', 'ang',
+        'fur', 'rm', 'mdf', 'lad', 'gom', 'ext', 'kaa', 'tyv', 'koi', 'av',
+        'pap', 'dsb', 'ln', 'dty', 'tw', 'cbk-zam', 'dv', 'ksh', 'za', 'gag',
+        'bxr', 'pfl', 'lg', 'szy', 'pag', 'blk', 'pi', 'tay', 'haw', 'awa',
+        'inh', 'krc', 'xal', 'pdc', 'to', 'atj', 'tcy', 'arc', 'mnw', 'jam',
+        'kbp', 'wo', 'kbd', 'anp', 'nia', 'nov', 'shi', 'ki', 'nqo', 'bi',
+        'om', 'tpi', 'xh', 'tet', 'roa-rup', 'jbo', 'fj', 'lbe', 'kg', 'ff',
+        'ty', 'guw', 'cu', 'trv', 'ami', 'srn', 'sm', 'mad', 'alt', 'gcr',
+        'ltg', 'chr', 'tn', 'ny', 'st', 'pih', 'rmy', 'got', 'ee', 'pcm', 'bm',
+        'ss', 'gpe', 've', 'ts', 'chy', 'kcg', 'rn', 'gur', 'ch', 'ik', 'ady',
+        'fat', 'pnt', 'guc', 'iu', 'pwn', 'sg', 'din', 'ti', 'kl', 'dz', 'cr',
     ]
 
     # Sites we want to edit but not count as real languages
     test_codes = ['test', 'test2']
 
     # Templates that indicate a category redirect
     # Redirects to these templates are automatically included
@@ -212,14 +211,24 @@
         'arz': ('صفحة ارشيف',),
         'cs': ('Archiv', 'Archiv Wikipedie', 'Archiv diskuse',
                'Archivace start', 'Posloupnost archivů', 'Rfa-archiv-start',
                'Rfc-archiv-start',),
         'de': ('Archiv',),
     }
 
+    @classmethod
+    def __post_init__(cls):
+        """Add 'yue' code alias due to :phab:`T341960`.
+
+        .. versionadded:: 8.3
+        """
+        aliases = cls.code_aliases.copy()
+        aliases['yue'] = 'zh-yue'
+        cls.code_aliases = aliases
+
     def encodings(self, code):
         """Return a list of historical encodings for a specific site."""
         # Historic compatibility
         if code == 'pl':
             return 'utf-8', 'iso8859-2'
         if code == 'ru':
             return 'utf-8', 'iso8859-5'
```

### Comparing `pywikibot-8.2.0/pywikibot/families/wikiquote_family.py` & `pywikibot-8.3.0/pywikibot/families/wikiquote_family.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,20 +24,20 @@
     removed_wikis = [
         # https://noc.wikimedia.org/conf/highlight.php?file=dblists/deleted.dblist
         'als', 'tokipona',
     ]
 
     languages_by_size = [
         'it', 'en', 'pl', 'ru', 'cs', 'et', 'pt', 'fa', 'uk', 'he', 'fr', 'de',
-        'es', 'tr', 'eo', 'sk', 'bs', 'az', 'ca', 'fi', 'sr', 'lt', 'zh', 'sl',
+        'es', 'tr', 'eo', 'sk', 'bs', 'az', 'ca', 'fi', 'sr', 'zh', 'lt', 'sl',
         'ar', 'su', 'id', 'bg', 'hy', 'hr', 'el', 'nn', 'sv', 'li', 'hu', 'ko',
-        'nl', 'ja', 'sah', 'la', 'ta', 'hi', 'ig', 'gl', 'gu', 'ur', 'guw',
-        'as', 'be', 'te', 'vi', 'tl', 'cy', 'bn', 'no', 'sq', 'ml', 'kn', 'ro',
-        'eu', 'ku', 'uz', 'ka', 'da', 'sa', 'is', 'bcl', 'th', 'br', 'mr',
-        'af', 'ky',
+        'nl', 'sah', 'ja', 'la', 'ta', 'hi', 'ig', 'gl', 'gu', 'ur', 'as',
+        'guw', 'be', 'te', 'vi', 'tl', 'bn', 'cy', 'no', 'sq', 'ml', 'kn',
+        'ro', 'eu', 'ku', 'uz', 'ka', 'da', 'sa', 'is', 'bcl', 'th', 'br',
+        'mr', 'af', 'ky',
     ]
 
     category_redirect_templates = {
         '_default': (),
         'ar': ('تحويل تصنيف',),
         'en': ('Category redirect',),
         'ro': ('Redirect categorie',),
```

### Comparing `pywikibot-8.2.0/pywikibot/families/wikisource_family.py` & `pywikibot-8.3.0/pywikibot/families/wikisource_family.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,18 +23,18 @@
         # https://noc.wikimedia.org/conf/highlight.php?file=dblists/deleted.dblist
         'tokipona',
     ]
 
     languages_by_size = [
         'pl', 'en', 'ru', 'de', 'fr', 'zh', 'he', 'it', 'uk', 'ar', 'es',
         'mul', 'gu', 'cs', 'sr', 'pt', 'bn', 'fa', 'sv', 'ko', 'hu', 'ta',
-        'ml', 'sa', 'te', 'sl', 'tr', 'vi', 'la', 'hy', 'el', 'be', 'ja', 'ro',
-        'nl', 'fi', 'nap', 'az', 'ca', 'hr', 'br', 'kn', 'no', 'id', 'th',
-        'hi', 'eo', 'is', 'cy', 'vec', 'ban', 'pms', 'mr', 'lij', 'da', 'et',
-        'as', 'mk', 'yi', 'bg', 'jv', 'wa', 'li', 'pa', 'lt', 'or', 'eu', 'gl',
+        'ml', 'sa', 'te', 'sl', 'tr', 'vi', 'la', 'hy', 'be', 'el', 'ja', 'nl',
+        'ro', 'fi', 'nap', 'az', 'ca', 'hr', 'br', 'kn', 'no', 'id', 'th',
+        'hi', 'eo', 'is', 'cy', 'vec', 'mr', 'ban', 'pms', 'lij', 'da', 'et',
+        'as', 'mk', 'yi', 'bg', 'jv', 'wa', 'li', 'lt', 'pa', 'or', 'eu', 'gl',
         'bs', 'sah', 'sk', 'zh-min-nan', 'fo',
     ]
 
     # Sites we want to edit but not count as real languages
     test_codes = ['beta']
 
     category_redirect_templates = {
```

### Comparing `pywikibot-8.2.0/pywikibot/families/wikiversity_family.py` & `pywikibot-8.3.0/pywikibot/families/wikiversity_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/families/wikivoyage_family.py` & `pywikibot-8.3.0/pywikibot/families/wikivoyage_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/families/wiktionary_family.py` & `pywikibot-8.3.0/pywikibot/families/wiktionary_family.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,24 +34,24 @@
     languages_by_size = [
         'en', 'fr', 'mg', 'zh', 'ru', 'de', 'es', 'sh', 'sv', 'nl', 'el', 'pl',
         'ku', 'lt', 'ca', 'it', 'hu', 'fi', 'ta', 'pt', 'tr', 'ja', 'io', 'hy',
         'ko', 'kn', 'vi', 'sr', 'th', 'hi', 'ro', 'id', 'no', 'et', 'skr',
         'cs', 'ml', 'my', 'uz', 'li', 'eo', 'or', 'te', 'fa', 'gl', 'ar', 'oc',
         'sg', 'jv', 'is', 'az', 'uk', 'eu', 'ast', 'br', 'mnw', 'da', 'bn',
         'simple', 'lo', 'la', 'hr', 'shn', 'sk', 'fj', 'ky', 'wa', 'bg', 'ur',
-        'cy', 'ps', 'tg', 'lmo', 'he', 'vo', 'om', 'sl', 'af', 'kbd',
-        'zh-min-nan', 'scn', 'ms', 'tl', 'pa', 'fy', 'sw', 'ka', 'nn', 'min',
-        'lv', 'kk', 'gor', 'nds', 'sq', 'lb', 'co', 'mn', 'bs', 'pnb', 'nah',
+        'lmo', 'cy', 'ps', 'tg', 'he', 'kbd', 'vo', 'om', 'sl', 'af',
+        'zh-min-nan', 'scn', 'ms', 'tl', 'pa', 'fy', 'sw', 'ka', 'nn', 'kk',
+        'min', 'lv', 'gor', 'nds', 'sq', 'lb', 'co', 'bs', 'mn', 'pnb', 'nah',
         'yue', 'ckb', 'sa', 'km', 'be', 'vec', 'diq', 'tk', 'nia', 'mk', 'sm',
-        'hsb', 'ks', 'shy', 'su', 'ga', 'bcl', 'gd', 'an', 'gom', 'mr', 'wo',
-        'mni', 'bjn', 'ia', 'ang', 'mt', 'sd', 'fo', 'tt', 'ha', 'gn', 'so',
+        'hsb', 'ks', 'shy', 'su', 'bcl', 'ga', 'gd', 'an', 'gom', 'mr', 'wo',
+        'mni', 'ia', 'bjn', 'ang', 'mt', 'sd', 'fo', 'tt', 'ha', 'so', 'gn',
         'si', 'ie', 'mi', 'csb', 'ug', 'guw', 'st', 'hif', 'roa-rup', 'jbo',
         'kl', 'zu', 'ay', 'ln', 'yi', 'gu', 'na', 'gv', 'kw', 'tpi', 'kcg',
         'am', 'ne', 'rw', 'ts', 'ig', 'qu', 'ss', 'iu', 'chr', 'dv', 'ti',
-        'tn',
+        'tn', 'btm',
     ]
 
     category_redirect_templates = {
         '_default': (),
         'ar': ('تحويل تصنيف',),
         'zh': ('分类重定向',),
     }
@@ -83,7 +83,17 @@
     doc_subpages = {
         '_default': (('/doc', ),
                      ['en']
                      ),
         'ar': ('/شرح', '/doc'),
         'sr': ('/док', ),
     }
+
+    @classmethod
+    def __post_init__(cls):
+        """Add 'zh-yue' code alias due to :phab:`T341960`.
+
+        .. versionadded:: 8.3
+        """
+        aliases = cls.code_aliases.copy()
+        aliases['zh-yue'] = 'yue'
+        cls.code_aliases = aliases
```

### Comparing `pywikibot-8.2.0/pywikibot/families/wowwiki_family.py` & `pywikibot-8.3.0/pywikibot/families/wowwiki_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/family.py` & `pywikibot-8.3.0/pywikibot/family.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 """Objects representing MediaWiki families."""
 #
 # (C) Pywikibot team, 2004-2023
 #
 # Distributed under the terms of the MIT license.
 #
 import collections
+import inspect
 import logging
 import string
 import sys
 import types
 import urllib.parse as urlparse
 import warnings
 from importlib import import_module
 from itertools import chain
+from textwrap import fill
 from os.path import basename, dirname, splitext
 from typing import Optional
 
 import pywikibot
 from pywikibot import config
 from pywikibot.backports import (
     Dict,
@@ -51,33 +53,42 @@
        :attr:`obsolete` setter was removed.
     """
 
     def __new__(cls):
         """Allocator."""
         # any Family class defined in this file are abstract
         if cls in globals().values():
-            raise TypeError(
-                'Abstract Family class {} cannot be instantiated; '
-                'subclass it instead'.format(cls.__name__))
+            raise TypeError(f'Abstract Family class {cls.__name__} cannot be'
+                            ' instantiated;  subclass it instead')
 
         # Override classproperty
         cls.instance = super().__new__(cls)
         cls.__new__ = lambda cls: cls.instance  # shortcut
 
         # don't use hasattr() here. consider only the class itself
         if '__init__' in cls.__dict__:
             # Initializer deprecated. Families should be immutable and any
             # instance / class modification should go to allocator (__new__).
-            cls.__init__ = deprecated(cls.__init__)
+            cls.__init__ = deprecated(instead='__post_init__() classmethod',
+                                      since='3.0.20180710')(cls.__init__)
 
             # Invoke initializer immediately and make initializer no-op.
             # This is to avoid repeated initializer invocation on repeated
             # invocations of the metaclass's __call__.
             cls.instance.__init__()
             cls.__init__ = lambda self: None  # no-op
+        elif '__post_init__' not in cls.__dict__:
+            pass
+        elif inspect.ismethod(cls.__post_init__):  # classmethod check
+            cls.__post_init__()
+        else:
+            raise RuntimeError(fill(
+                f'__post_init__() method of {cls.__module__}.{cls.__name__}'
+                ' class or its superclass must be a classmethod. Please  check'
+                ' your family file.', width=66))
 
         return cls.instance
 
     @classproperty
     def instance(cls):
         """Get the singleton instance."""
         # This is a placeholder to invoke allocator before it's allocated.
```

### Comparing `pywikibot-8.2.0/pywikibot/fixes.py` & `pywikibot-8.3.0/pywikibot/fixes.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/flow.py` & `pywikibot-8.3.0/pywikibot/flow.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/i18n.py` & `pywikibot-8.3.0/pywikibot/i18n.py`

 * *Files 0% similar despite different names*

```diff
@@ -907,15 +907,15 @@
 
     >>> from pywikibot import i18n
     >>> i18n.known_languages()[:10]
     ['ab', 'aeb', 'af', 'am', 'an', 'ang', 'anp', 'ar', 'arc', 'ary']
     >>> i18n.known_languages()[-10:]
     ['vo', 'vro', 'wa', 'war', 'xal', 'xmf', 'yi', 'yo', 'yue', 'zh']
     >>> len(i18n.known_languages())
-    252
+    253
 
     The implementation is roughly equivalent to:
 
     .. code-block:: Python
 
        langs = set()
        for dirpath in bundles():
```

### Comparing `pywikibot-8.2.0/pywikibot/interwiki_graph.py` & `pywikibot-8.3.0/pywikibot/interwiki_graph.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/logentries.py` & `pywikibot-8.3.0/pywikibot/logentries.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/logging.py` & `pywikibot-8.3.0/pywikibot/logging.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/login.py` & `pywikibot-8.3.0/pywikibot/login.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/page/__init__.py` & `pywikibot-8.3.0/pywikibot/page/__init__.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/page/_basepage.py` & `pywikibot-8.3.0/pywikibot/page/_basepage.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/page/_category.py` & `pywikibot-8.3.0/pywikibot/page/_category.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/page/_collections.py` & `pywikibot-8.3.0/pywikibot/page/_collections.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/page/_decorators.py` & `pywikibot-8.3.0/pywikibot/page/_decorators.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/page/_filepage.py` & `pywikibot-8.3.0/pywikibot/page/_filepage.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/page/_links.py` & `pywikibot-8.3.0/pywikibot/page/_links.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/page/_page.py` & `pywikibot-8.3.0/pywikibot/page/_page.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/page/_revision.py` & `pywikibot-8.3.0/pywikibot/page/_revision.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/page/_toolforge.py` & `pywikibot-8.3.0/pywikibot/page/_toolforge.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/page/_user.py` & `pywikibot-8.3.0/pywikibot/page/_user.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/page/_wikibase.py` & `pywikibot-8.3.0/pywikibot/page/_wikibase.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/pagegenerators/__init__.py` & `pywikibot-8.3.0/pywikibot/pagegenerators/__init__.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/pagegenerators/_factory.py` & `pywikibot-8.3.0/pywikibot/pagegenerators/_factory.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/pagegenerators/_filters.py` & `pywikibot-8.3.0/pywikibot/pagegenerators/_filters.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/pagegenerators/_generators.py` & `pywikibot-8.3.0/pywikibot/pagegenerators/_generators.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/plural.py` & `pywikibot-8.3.0/pywikibot/plural.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/proofreadpage.py` & `pywikibot-8.3.0/pywikibot/proofreadpage.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/__init__.py` & `pywikibot-8.3.0/pywikibot/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/generate_family_file.py` & `pywikibot-8.3.0/pywikibot/scripts/generate_family_file.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/generate_user_files.py` & `pywikibot-8.3.0/pywikibot/scripts/generate_user_files.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/ar.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/ar.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/ast.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/ast.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/az.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/az.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/azb.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/azb.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/ba.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/ba.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/bcc.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/bcc.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/be-tarask.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/be-tarask.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/be.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/be.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/bg.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/bg.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/bn.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/bn.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/br.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/br.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/bs.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/bs.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/ca.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/ca.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/ce.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/ce.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/ckb.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/ckb.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/cs.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/cs.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/csb.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/csb.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/cy.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/cy.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/da.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/da.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/de.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/de.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/diq.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/diq.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/el.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/el.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/en.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/en.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/eo.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/eo.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/es.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/es.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/eu.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/eu.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/fa.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/fa.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/fi.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/fo.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.4318181818181818%*

 * *Differences: {"'@metadata'": "{'authors': ['EileenSanda']}",*

 * * "'pywikibot-bot-prefix'": "'Bottur:'",*

 * * "'pywikibot-cosmetic-changes'": "'; broytingar av útsjónd'",*

 * * "'pywikibot-enter-category-name'": "'Vinarliga skriva bólkanavnið:'",*

 * * "'pywikibot-enter-file-links-processing'": "'Slóðir til hvørja fílusíðu skulu viðgerast?'",*

 * * "'pywikibot-enter-finished-browser'": "'Trýst á Enter tá tú ert liðug/ur at rætta í brovsaranum.'",*

 * * "'pywikibot-enter-namespace-number'": "'Vinarliga skriva eitt navnarúm við tilhoyrandi nummari:' […]*

```diff
@@ -1,17 +1,17 @@
 {
     "@metadata": {
         "authors": [
-            "Crt",
-            "Nedergard",
-            "VezonThunder"
+            "EileenSanda"
         ]
     },
-    "pywikibot-cosmetic-changes": "; kosmeettisia muutoksia",
-    "pywikibot-enter-category-name": "Kirjoita luokan nimi",
-    "pywikibot-enter-file-links-processing": "Mille tiedostosivulle viev\u00e4t linkit tulee k\u00e4sitell\u00e4?",
-    "pywikibot-enter-finished-browser": "Paina enter, kun olet valmis selaimessa.",
-    "pywikibot-enter-namespace-number": "Kirjoita nimiavaruuden numero",
-    "pywikibot-enter-new-text": "Kirjoita uusi teksti",
-    "pywikibot-enter-page-processing": "Mik\u00e4 sivu otetaan k\u00e4sitelt\u00e4v\u00e4ksi?",
-    "pywikibot-fixes-isbn": "Botti muotoili ISBN-tunnuksen"
+    "pywikibot-bot-prefix": "Bottur:",
+    "pywikibot-cosmetic-changes": "; broytingar av \u00fatsj\u00f3nd",
+    "pywikibot-enter-category-name": "Vinarliga skriva b\u00f3lkanavni\u00f0:",
+    "pywikibot-enter-file-links-processing": "Sl\u00f3\u00f0ir til hv\u00f8rja f\u00edlus\u00ed\u00f0u skulu vi\u00f0gerast?",
+    "pywikibot-enter-finished-browser": "Tr\u00fdst \u00e1 Enter t\u00e1 t\u00fa ert li\u00f0ug/ur at r\u00e6tta \u00ed brovsaranum.",
+    "pywikibot-enter-namespace-number": "Vinarliga skriva eitt navnar\u00fam vi\u00f0 tilhoyrandi nummari:",
+    "pywikibot-enter-new-text": "Vinarliga skriva n\u00fdggja tekstin:",
+    "pywikibot-enter-page-processing": "Hv\u00f8r s\u00ed\u00f0a skal vi\u00f0gerast?",
+    "pywikibot-enter-xml-filename": "Vinarliga skriva XML f\u00edlunavni\u00f0 hj\u00e1 dump'inum:",
+    "pywikibot-fixes-isbn": "Bottur: Formaterar ISBN"
 }
```

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/fo.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/pms.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5227272727272727%*

 * *Differences: {"'@metadata'": "{'authors': ['Borichèt', 'Dragonòt']}",*

 * * "'pywikibot-bot-prefix'": "'Trigomiro:'",*

 * * "'pywikibot-cosmetic-changes'": "'; cangiament cosmétich'",*

 * * "'pywikibot-enter-category-name'": '"Për piasì, ch\'a anserissa ël nòm ëd la categorìa:"',*

 * * "'pywikibot-enter-file-links-processing'": '"Liure a la pàgina d\'archivi ch\'a ventrìa traté?"',*

 * * "'pywikibot-enter-finished-browser'": '"Ch\'a sgnaca A cap quand a l\'ha finì ant ël navigador."',*

 * * "'pywikibot-enter-namespace-number'": "'Për piasì anseriss  […]*

```diff
@@ -1,17 +1,18 @@
 {
     "@metadata": {
         "authors": [
-            "EileenSanda"
+            "Borich\u00e8t",
+            "Dragon\u00f2t"
         ]
     },
-    "pywikibot-bot-prefix": "Bottur:",
-    "pywikibot-cosmetic-changes": "; broytingar av \u00fatsj\u00f3nd",
-    "pywikibot-enter-category-name": "Vinarliga skriva b\u00f3lkanavni\u00f0:",
-    "pywikibot-enter-file-links-processing": "Sl\u00f3\u00f0ir til hv\u00f8rja f\u00edlus\u00ed\u00f0u skulu vi\u00f0gerast?",
-    "pywikibot-enter-finished-browser": "Tr\u00fdst \u00e1 Enter t\u00e1 t\u00fa ert li\u00f0ug/ur at r\u00e6tta \u00ed brovsaranum.",
-    "pywikibot-enter-namespace-number": "Vinarliga skriva eitt navnar\u00fam vi\u00f0 tilhoyrandi nummari:",
-    "pywikibot-enter-new-text": "Vinarliga skriva n\u00fdggja tekstin:",
-    "pywikibot-enter-page-processing": "Hv\u00f8r s\u00ed\u00f0a skal vi\u00f0gerast?",
-    "pywikibot-enter-xml-filename": "Vinarliga skriva XML f\u00edlunavni\u00f0 hj\u00e1 dump'inum:",
-    "pywikibot-fixes-isbn": "Bottur: Formaterar ISBN"
+    "pywikibot-bot-prefix": "Trigomiro:",
+    "pywikibot-cosmetic-changes": "; cangiament cosm\u00e9tich",
+    "pywikibot-enter-category-name": "P\u00ebr pias\u00ec, ch'a anserissa \u00ebl n\u00f2m \u00ebd la categor\u00eca:",
+    "pywikibot-enter-file-links-processing": "Liure a la p\u00e0gina d'archivi ch'a ventr\u00eca trat\u00e9?",
+    "pywikibot-enter-finished-browser": "Ch'a sgnaca A cap quand a l'ha fin\u00ec ant \u00ebl navigador.",
+    "pywikibot-enter-namespace-number": "P\u00ebr pias\u00ec anseriss n\u00eb spassi nominal con s\u00f2 n\u00f9mer:",
+    "pywikibot-enter-new-text": "P\u00ebr pias\u00ec, ch'a anserissa \u00ebl test neuv:",
+    "pywikibot-enter-page-processing": "Che p\u00e0gina a ventr\u00eca trat\u00e9?",
+    "pywikibot-enter-xml-filename": "P\u00ebr pias\u00ec anseriss \u00ebl n\u00f2m \u00ebd l'archivi XML d\u00ebl dump:",
+    "pywikibot-fixes-isbn": "Trigomiro: Formassion \u00ebd l'ISBN"
 }
```

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/fr.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/fr.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/frr.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/frr.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/gl.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/gl.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'pywikibot-cosmetic-changes'": "'; cambios estéticos'"}*

```diff
@@ -3,15 +3,15 @@
         "authors": [
             "Banjo",
             "Gallaecio",
             "Toli\u00f1o"
         ]
     },
     "pywikibot-bot-prefix": "Robot:",
-    "pywikibot-cosmetic-changes": "; cambios est\u00e9tica",
+    "pywikibot-cosmetic-changes": "; cambios est\u00e9ticos",
     "pywikibot-enter-category-name": "Insira o nome da categor\u00eda:",
     "pywikibot-enter-file-links-processing": "As ligaz\u00f3ns a que p\u00e1xina de ficheiro se deben procesar?",
     "pywikibot-enter-finished-browser": "Prema na tecla \"Intro\" cando remate no navegador.",
     "pywikibot-enter-namespace-number": "Insira un espazo de nomes segundo o seu n\u00famero:",
     "pywikibot-enter-new-text": "Insira o novo texto:",
     "pywikibot-enter-page-processing": "Que p\u00e1xina se debe procesar?",
     "pywikibot-enter-xml-filename": "Insira o nome do ficheiro de descarga XML:",
```

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/gsw.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/gsw.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/hak.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/hak.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/haw.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/haw.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/he.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/he.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/hi.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/hi.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/hsb.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/hsb.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/hu.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/hu.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/ia.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/ia.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/id.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/id.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/io.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/io.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/is.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/is.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/it.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/it.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/ja.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/ja.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/kab.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/kab.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/kk.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/kk.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9479166666666666%*

 * *Differences: {"'@metadata'": "{'authors': {insert: [(1, 'Lifeway')]}}", "'pywikibot-bot-prefix'": "'Бот:'"}*

```diff
@@ -1,14 +1,15 @@
 {
     "@metadata": {
         "authors": [
-            "Arystanbek"
+            "Arystanbek",
+            "Lifeway"
         ]
     },
-    "pywikibot-bot-prefix": "\u0420\u043e\u0431\u043e\u0442:",
+    "pywikibot-bot-prefix": "\u0411\u043e\u0442:",
     "pywikibot-cosmetic-changes": "; \u0431\u0435\u0437\u0435\u043d\u0434\u0456\u0440\u0443 \u04e9\u0437\u0433\u0435\u0440\u0456\u0441\u0442\u0435\u0440\u0456",
     "pywikibot-enter-category-name": "\u0421\u0430\u043d\u0430\u0442 \u0430\u0442\u0430\u0443\u044b\u043d \u0435\u043d\u0433\u0456\u0437\u0456\u04a3\u0456\u0437:",
     "pywikibot-enter-file-links-processing": "\u0424\u0430\u0439\u043b \u0431\u0435\u0442\u0456 \u0441\u0456\u043b\u0442\u0435\u043c\u0435\u043b\u0435\u0440\u0456\u043d \u04e9\u04a3\u0434\u0435\u0443 \u043a\u0435\u0440\u0435\u043a \u043f\u0435?",
     "pywikibot-enter-finished-browser": "\u0411\u0440\u0430\u0443\u0437\u0435\u0440\u0434\u0435 \u0430\u044f\u049b\u0442\u0430\u0493\u0430\u043d \u043a\u0435\u0437\u0434\u0435 Enter \u043f\u0435\u0440\u043d\u0435\u0441\u0456\u043d \u0431\u0430\u0441\u044b\u04a3\u044b\u0437.",
     "pywikibot-enter-namespace-number": "\u0415\u0441\u0456\u043c \u043a\u0435\u04a3\u0456\u0441\u0442\u0456\u0433\u0456\u043d \u043e\u043d\u044b\u04a3 \u043d\u04e9\u043c\u0435\u0440\u0456 \u0431\u043e\u0439\u044b\u043d\u0448\u0430 \u0435\u043d\u0433\u0456\u0437\u0456\u04a3\u0456\u0437:",
     "pywikibot-enter-new-text": "\u0416\u0430\u04a3\u0430 \u043c\u04d9\u0442\u0456\u043d \u0435\u043d\u0433\u0456\u0437\u0456\u04a3\u0456\u0437:",
     "pywikibot-enter-page-processing": "\u049a\u0430\u043d\u0434\u0430\u0439 \u0431\u0435\u0442 \u04e9\u04a3\u0434\u0435\u0443 \u043a\u0435\u0440\u0435\u043a?",
```

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/km.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/km.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/kn.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/kn.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/ko.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/ko.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/krc.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/krc.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/ksh.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/ksh.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/lb.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/lb.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/lt.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/lt.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/lv.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/lv.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/map-bms.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/map-bms.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/mg.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/mg.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/min.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/min.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/mk.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/mk.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'pywikibot-fixes-isbn'": "'Робот: Форматирање на ISBN'"}*

```diff
@@ -11,11 +11,11 @@
     "pywikibot-enter-finished-browser": "\u0421\u0442\u0438\u0441\u043d\u0435\u0442\u0435 \u043d\u0430 \u201eEnter\u201c \u043a\u043e\u0433\u0430 \u045c\u0435 \u0437\u0430\u0432\u0440\u0448\u0438\u0442\u0435 \u0432\u043e \u043f\u0440\u0435\u043b\u0438\u0441\u0442\u0443\u0432\u0430\u0447\u043e\u0442.",
     "pywikibot-enter-namespace-number": "\u0412\u043d\u0435\u0441\u0435\u0442\u0435 \u0433\u043e \u0438\u043c\u0435\u043d\u0441\u043a\u0438\u043e\u0442 \u043f\u0440\u043e\u0441\u0442\u043e\u0440 \u0441\u043f\u043e\u0440\u0435\u0434 \u043d\u0435\u0433\u043e\u0432\u0438\u043e\u0442 \u0431\u0440\u043e\u0458:",
     "pywikibot-enter-new-text": "\u0412\u043d\u0435\u0441\u0435\u0442\u0435 \u0433\u043e \u043d\u043e\u0432\u0438\u043e\u0442 \u0442\u0435\u043a\u0441\u0442:",
     "pywikibot-enter-page-processing": "\u041a\u043e\u0458\u0430 \u0441\u0442\u0440\u0430\u043d\u0438\u0446\u0430 \u0442\u0440\u0435\u0431\u0430 \u0434\u0430 \u0441\u0435 \u043e\u0431\u0440\u0430\u0431\u043e\u0442\u0438?",
     "pywikibot-enter-xml-filename": "\u0412\u043d\u0435\u0441\u0435\u0442\u0435 \u0433\u043e \u0438\u043c\u0435\u0442\u043e \u043d\u0430 XML-\u0441\u043a\u043b\u0430\u0434\u043e\u0442:",
     "pywikibot-fixes-fckeditor": "\u0411\u043e\u0442: \u0418\u0441\u043f\u0440\u0430\u0432\u043a\u0430 \u043d\u0430 \u0437\u0431\u043e\u0433\u0430\u0442\u0435\u043d HMTL",
     "pywikibot-fixes-html": "\u0411\u043e\u0442: \u041f\u0440\u0435\u0442\u0432\u043e\u0440\u0430\u045a\u0435/\u0438\u0441\u043f\u0440\u0430\u0432\u043a\u0430 \u043d\u0430 HTML",
-    "pywikibot-fixes-isbn": "\u0420\u043e\u0431\u043e\u0442: \u0424\u043e\u0440\u043c\u0430\u0442\u0438\u0440\u0430\u043c ISBN",
+    "pywikibot-fixes-isbn": "\u0420\u043e\u0431\u043e\u0442: \u0424\u043e\u0440\u043c\u0430\u0442\u0438\u0440\u0430\u045a\u0435 \u043d\u0430 ISBN",
     "pywikibot-fixes-syntax": "\u0411\u043e\u0442: \u0418\u0441\u043f\u0440\u0430\u0432\u043a\u0430 \u043d\u0430 \u0432\u0438\u043a\u0438\u0441\u0438\u043d\u0442\u0430\u043a\u0441\u0430",
     "pywikibot-touch": "\u041d\u0438\u0448\u0442\u043e\u0432\u043d\u043e \u0443\u0440\u0435\u0434\u0443\u0432\u0430\u045a\u0435 \u0441\u043e Pywikibot"
 }
```

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/ml.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/ml.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/ms.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/ms.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/my.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/my.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/nan.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/nan.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/nb.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/nb.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/nds-nl.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/nds-nl.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/ne.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/ne.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/new.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/new.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/nl.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/nl.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/nqo.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/nqo.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9333333333333333%*

 * *Differences: {"'pywikibot-enter-xml-filename'": "'XML ߢߊ߬ߡߊ ߞߐߕߐ߮ ߕߐ߮ ߟߊߘߏ߲߬ ߖߊ߰ߣߌ߲߫:'"}*

```diff
@@ -8,13 +8,14 @@
     "pywikibot-cosmetic-changes": "; \u07e1\u07ca\u07ec\u07de\u07cb\u07f2\u07f0\u07e7\u07ca\u07ec\u07df\u07cc \u07e1\u07dd\u07ca\u07ec\u07df\u07cb\u07f2\u07ec\u07e0\u07cc\u07f2 \u07e0\u07ce\u07ec",
     "pywikibot-enter-category-name": "\u07e6\u07cc\u07df\u07e1\u07ca \u07d5\u07d0\u07ee \u07df\u07ca\u07d8\u07cf\u07f2\u07ec \u07d6\u07ca\u07f0\u07e3\u07cc\u07f2\u07eb:",
     "pywikibot-enter-file-links-processing": "\u07de\u07d0\u07d5\u07d0\u07ee \u07de\u07d0\u07dc\u07cd \u07e2\u07ca\u07d3\u07d0\u07eb \u07d5\u07d0\u07eb \u07e6\u07cb\u07eb \u07db\u07d8\u07cc\u07ec\u07dc\u07cb\u07f2 \u07e1\u07cd\u07f2 \u07e0\u07ca\u07eb",
     "pywikibot-enter-finished-browser": "\u07d8\u07cf\u07f2\u07ec (enter) \u07d8\u07cc\u07ef \u07e3\u07f4\u07cc \u07d3\u07ca\u07f2\u07eb \u07d8\u07ca\u07eb \u07db\u07cf\u07f2\u07ef\u07d3\u07ca\u07df\u07ca\u07f2 \u07e0\u07ca\u07eb.",
     "pywikibot-enter-namespace-number": "\u07d5\u07d0\u07ef \u07de\u07e3\u07cd \u07df\u07ca\u07d8\u07cf\u07f2\u07ec \u07ca\u07ec \u07dd\u07d9\u07cd\u07d5\u07cd \u07df\u07ca\u07eb \u07d6\u07ca\u07f0\u07e3\u07cc\u07f2\u07eb:",
     "pywikibot-enter-new-text": "\u07de\u07df\u07cf\u07dc\u07cd\u07eb \u07de\u07ce\u07d8\u07ca\u07eb \u07df\u07ca\u07d8\u07cf\u07f2\u07ec \u07d6\u07ca\u07f0\u07e3\u07cc\u07f2\u07eb:",
     "pywikibot-enter-page-processing": "\u07de\u07d0\u07dc\u07cd \u07e2\u07ce\u07ec\u07e1\u07ca\u07f2\u07eb \u07e0\u07cb\u07ec \u07e2\u07ca\u07d3\u07d0\u07eb \u07d5\u07d0\u07eb \u07e6\u07cb\u07eb\u061f",
+    "pywikibot-enter-xml-filename": "XML \u07e2\u07ca\u07ec\u07e1\u07ca \u07de\u07d0\u07d5\u07d0\u07ee \u07d5\u07d0\u07ee \u07df\u07ca\u07d8\u07cf\u07f2\u07ec \u07d6\u07ca\u07f0\u07e3\u07cc\u07f2\u07eb:",
     "pywikibot-fixes-fckeditor": "\u07e1\u07d0\u07f0\u07e1\u07d0\u07ee: \u07e6\u07cb\u07eb \u07e1\u07ca\u07ec\u07e6\u07df\u07cd\u07ec\u07e1\u07ca\u07f2\u07ec\u07e0\u07ca\u07eb-\u07db\u07d3\u07ca\u07ec\u07d5\u07cc\u07ec\u07e3\u07cd\u07f2 HTML \u07d8\u07d0\u07d3\u07cd\u07f2\u07ed \u07de\u07ca\u07f2\u07ec",
     "pywikibot-fixes-html": "\u07e1\u07d0\u07f0\u07e1\u07d0\u07ee: \u07e6\u07cb\u07eb HTML \u07e6\u07df\u07cd\u07ec\u07e1\u07ca\\\u07d8\u07d0\u07d3\u07cd\u07f2\u07ed \u07de\u07ca\u07f2\u07ec",
     "pywikibot-fixes-isbn": "\u07e1\u07d0\u07f0\u07e1\u07d0\u07ee: \u07e6\u07cb\u07eb ISBN \u07dd\u07d9\u07cd\u07d5\u07cd \u07db\u07cf\u07ef\u07d9\u07cf \u07de\u07ca\u07f2\u07ec",
     "pywikibot-fixes-syntax": "\u07e1\u07d0\u07f0\u07e1\u07d0\u07ee: \u07e6\u07cb\u07eb \u07e5\u07de\u07cc \u07de\u07ce\u07e1\u07e6\u07ca \u07e2\u07ca\u07d3\u07d0\u07df\u07cc \u07d8\u07d0\u07d3\u07cd\u07f2\u07ed \u07de\u07ca\u07f2\u07ec",
     "pywikibot-touch": "\u07d4\u07ca\u07cc\u07e5\u07de\u07cc\u07d3\u07cf\u07d5 \u07e1\u07ca\u07f0\u07d2\u07ec\u07e0\u07ca\u07eb \u07dc\u07ca\u07f2\u07ef\u07db\u07ca\u07f2 \u07e1\u07ca\u07ec\u07e6\u07df\u07cd\u07ec\u07e1\u07ca\u07f2\u07ec\u07e0\u07cc\u07f2"
 }
```

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/pl.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/pl.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/pms.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/pt.json`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.38333333333333336%*

 * *Differences: {"'@metadata'": "{'authors': ['Alchimista', 'Hamilton Abreu', 'Leonardo Gregianin', 'Malafaya', "*

 * *                "'Vitorvicentevalente']}",*

 * * "'pywikibot-bot-prefix'": "'Robô:'",*

 * * "'pywikibot-cosmetic-changes'": "'; mudanças triviais'",*

 * * "'pywikibot-enter-category-name'": "'Por favor, introduza o nome da categoria:'",*

 * * "'pywikibot-enter-file-links-processing'": "'Devem ser processadas as hiperligações para qual "*

 * *                                            "página de ficheiro?'",*

 * * "'pywikibot-enter-finished […]*

```diff
@@ -1,18 +1,25 @@
 {
     "@metadata": {
         "authors": [
-            "Borich\u00e8t",
-            "Dragon\u00f2t"
+            "Alchimista",
+            "Hamilton Abreu",
+            "Leonardo Gregianin",
+            "Malafaya",
+            "Vitorvicentevalente"
         ]
     },
-    "pywikibot-bot-prefix": "Trigomiro:",
-    "pywikibot-cosmetic-changes": "; cangiament cosm\u00e9tich",
-    "pywikibot-enter-category-name": "P\u00ebr pias\u00ec, ch'a anserissa \u00ebl n\u00f2m \u00ebd la categor\u00eca:",
-    "pywikibot-enter-file-links-processing": "Liure a la p\u00e0gina d'archivi ch'a ventr\u00eca trat\u00e9?",
-    "pywikibot-enter-finished-browser": "Ch'a sgnaca A cap quand a l'ha fin\u00ec ant \u00ebl navigador.",
-    "pywikibot-enter-namespace-number": "P\u00ebr pias\u00ec anseriss n\u00eb spassi nominal con s\u00f2 n\u00f9mer:",
-    "pywikibot-enter-new-text": "P\u00ebr pias\u00ec, ch'a anserissa \u00ebl test neuv:",
-    "pywikibot-enter-page-processing": "Che p\u00e0gina a ventr\u00eca trat\u00e9?",
-    "pywikibot-enter-xml-filename": "P\u00ebr pias\u00ec anseriss \u00ebl n\u00f2m \u00ebd l'archivi XML d\u00ebl dump:",
-    "pywikibot-fixes-isbn": "Trigomiro: Formassion \u00ebd l'ISBN"
+    "pywikibot-bot-prefix": "Rob\u00f4:",
+    "pywikibot-cosmetic-changes": "; mudan\u00e7as triviais",
+    "pywikibot-enter-category-name": "Por favor, introduza o nome da categoria:",
+    "pywikibot-enter-file-links-processing": "Devem ser processadas as hiperliga\u00e7\u00f5es para qual p\u00e1gina de ficheiro?",
+    "pywikibot-enter-finished-browser": "Pressione Enter quando terminar no navegador",
+    "pywikibot-enter-namespace-number": "Por favor, introduza um espa\u00e7o nominal usando o seu n\u00famero:",
+    "pywikibot-enter-new-text": "Por favor, introduza o novo texto:",
+    "pywikibot-enter-page-processing": "Que p\u00e1gina deve ser processada?",
+    "pywikibot-enter-xml-filename": "Por favor introduza o nome do ficheiro XML:",
+    "pywikibot-fixes-fckeditor": "Rob\u00f4: A corrigir o HTML gerado pelo editor visual.",
+    "pywikibot-fixes-html": "Rob\u00f4: Convers\u00e3o ou corre\u00e7\u00e3o de HTML",
+    "pywikibot-fixes-isbn": "Rob\u00f4: A formatar o ISBN",
+    "pywikibot-fixes-syntax": "Rob\u00f4: Corre\u00e7\u00e3o da sintaxe wiki",
+    "pywikibot-touch": "Edi\u00e7\u00e3o por toque de Pywikibot"
 }
```

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/pt-br.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/pt-br.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/qqq.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/qqq.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/ro.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/ro.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/ru.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/ru.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/sco.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/sco.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/sh.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/sh.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/si.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/si.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/sk.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/sk.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/sl.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/sl.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/so.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/so.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/sr.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/sr.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/sv.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/sv.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/sw.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/sw.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/ta.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/ta.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/te.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/te.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/th.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/th.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/tly.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/tly.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9431818181818182%*

 * *Differences: {"'@metadata'": "{'authors': {insert: [(0, 'Lifeway')]}}", "'pywikibot-bot-prefix'": "'Бот:'"}*

```diff
@@ -1,14 +1,15 @@
 {
     "@metadata": {
         "authors": [
+            "Lifeway",
             "\u0413\u0443\u0441\u0435\u0439\u043d"
         ]
     },
-    "pywikibot-bot-prefix": "\u0420\u043e\u0431\u043e\u0442:",
+    "pywikibot-bot-prefix": "\u0411\u043e\u0442:",
     "pywikibot-cosmetic-changes": "; \u043a\u043e\u0441\u043c\u0435\u0442\u0438\u043a\u04d9 \u0434\u04d9\u0433\u0438\u0448\u043e\u043d",
     "pywikibot-enter-category-name": "\u0417\u04d9\u04bb\u043c\u04d9\u0442 \u043d\u044b\u0431\u043e, \u0442\u0438\u0441\u043f\u0438\u0440\u0438 \u043d\u043e\u043c \u0434\u04d9\u0493\u0430\u043d\u0434\u04d9\u043d:",
     "pywikibot-enter-file-links-processing": "\u0421\u04d9\u0431\u043e\u043d\u043e\u043d \u0431\u04d9 \u043a\u043e\u043d \u0433\u044b\u043b\u04d9 \u0448\u0438\u043a\u0438\u043b\u043e\u043d \u0441\u04d9\u04bb\u0438\u0444\u04d9 \u0431\u04d9\u043f\u0435 \u0435\u043c\u043e\u043b \u043a\u0430\u0440\u0434\u04d9 \u0431\u044b\u0431\u0443\u043d?",
     "pywikibot-enter-finished-browser": "Enter \u0435\u0433\u04d9\u0442\u04d9\u0434\u044b\u0433\u043c\u04d9 \u0435\u0433\u04d9\u0442\u04d9\u0458\u043e\u043d, \u043a\u0435\u0458\u043d\u04d9 \u043e\u0431\u04d9\u0440\u04d9\u0445\u043d\u0435\u0458\u043e\u043d \u0431\u04d9 \u0431\u0440\u0430\u0443\u0437\u0435\u0440 \u0434\u04d9\u0433\u0438\u0448\u0438\u0458\u043e\u043d \u0434\u04d9\u0493\u0430\u043d\u0434\u0435\u0458.",
     "pywikibot-enter-namespace-number": "\u0417\u04d9\u04bb\u043c\u04d9\u0442 \u043d\u044b\u0431\u043e, \u043d\u043e\u043c\u043e\u043d \u043c\u04d9\u043a\u043e\u043d \u043d\u0443\u043c\u0440\u04d9 \u0434\u04d9\u0493\u0430\u043d\u0434\u04d9\u043d:",
     "pywikibot-enter-new-text": "\u0417\u04d9\u04bb\u043c\u04d9\u0442 \u043d\u044b\u0431\u043e, \u043d\u0443\u0458\u04d9 \u043c\u04d9\u0442\u043d \u0434\u04d9\u0493\u0430\u043d\u0434\u04d9\u043d:",
     "pywikibot-enter-page-processing": "\u041a\u043e\u043d \u0433\u044b\u043b\u04d9 \u0441\u04d9\u04bb\u0438\u0444\u04d9 \u0431\u04d9\u043f\u0435 \u0435\u043c\u043e\u043b \u043a\u0430\u0440\u0434\u04d9 \u0431\u044b\u0431\u0443?",
```

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/tr.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/tr.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/uk.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/uk.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/ur.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/ur.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/vi.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/vi.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/yue.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/yue.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/zh.json` & `pywikibot-8.3.0/pywikibot/scripts/i18n/pywikibot/zh.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/login.py` & `pywikibot-8.3.0/pywikibot/scripts/login.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/preload_sites.py` & `pywikibot-8.3.0/pywikibot/scripts/preload_sites.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/shell.py` & `pywikibot-8.3.0/pywikibot/scripts/shell.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/version.py` & `pywikibot-8.3.0/pywikibot/scripts/version.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/scripts/wrapper.py` & `pywikibot-8.3.0/pywikibot/scripts/wrapper.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/site/__init__.py` & `pywikibot-8.3.0/pywikibot/site/__init__.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/site/_apisite.py` & `pywikibot-8.3.0/pywikibot/site/_apisite.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/site/_basesite.py` & `pywikibot-8.3.0/pywikibot/site/_basesite.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/site/_datasite.py` & `pywikibot-8.3.0/pywikibot/site/_datasite.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/site/_decorators.py` & `pywikibot-8.3.0/pywikibot/site/_decorators.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/site/_extensions.py` & `pywikibot-8.3.0/pywikibot/site/_extensions.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/site/_generators.py` & `pywikibot-8.3.0/pywikibot/site/_generators.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/site/_interwikimap.py` & `pywikibot-8.3.0/pywikibot/site/_interwikimap.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/site/_namespace.py` & `pywikibot-8.3.0/pywikibot/site/_namespace.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/site/_obsoletesites.py` & `pywikibot-8.3.0/pywikibot/site/_obsoletesites.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/site/_siteinfo.py` & `pywikibot-8.3.0/pywikibot/site/_siteinfo.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/site/_tokenwallet.py` & `pywikibot-8.3.0/pywikibot/site/_tokenwallet.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/site/_upload.py` & `pywikibot-8.3.0/pywikibot/site/_upload.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/site_detect.py` & `pywikibot-8.3.0/pywikibot/site_detect.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/specialbots/_unlink.py` & `pywikibot-8.3.0/pywikibot/specialbots/_unlink.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/specialbots/_upload.py` & `pywikibot-8.3.0/pywikibot/specialbots/_upload.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/textlib.py` & `pywikibot-8.3.0/pywikibot/textlib.py`

 * *Files 0% similar despite different names*

```diff
@@ -266,15 +266,15 @@
                      lambda site: '|'.join(site.namespaces[14])),
         'comment': re.compile(r'<!--[\s\S]*?-->'),
         # files
         'file': (FILE_LINK_REGEX, lambda site: '|'.join(site.namespaces[6])),
         # section headers
         'header': re.compile(
             r'(?:(?<=\n)|\A)(?:<!--[\s\S]*?-->)*'
-            r'=(?:[^\n]|<!--[\s\S]*?-->)+='
+            r'(=(?:[^\n]|<!--[\s\S]*?-->)+=)'
             r' *(?:<!--[\s\S]*?--> *)*(?=\n|\Z)'),
         # external links
         'hyperlink': compileLinkR(),
         # also finds links to foreign sites with preleading ":"
         'interwiki': (
             r'\[\[:?(%s)\s?:[^\]]*\]\]\s*',
             lambda site: '|'.join(
@@ -929,15 +929,15 @@
 
 
 # -------------------------------
 # Functions dealing with sections
 # -------------------------------
 
 #: Head pattern
-HEAD_PATTERN = re.compile('{0}[^=]+{0}'.format('(={1,6})'))
+HEAD_PATTERN = re.compile(r'(={1,6}).+\1', re.DOTALL)
 TITLE_PATTERN = re.compile("'{3}([^']+)'{3}")
 
 _Heading = namedtuple('_Heading', ('text', 'start', 'end'))
 
 
 class Section(NamedTuple):
 
@@ -953,15 +953,15 @@
     @property
     def level(self) -> int:
         """Return the section level.
 
         .. versionadded:: 8.2
         """
         m = HEAD_PATTERN.match(self.title)
-        return min(map(len, m.groups()))
+        return len(m[1])
 
     @property
     def heading(self) -> str:
         """Return the section title without equal signs.
 
         .. versionadded:: 8.2
         """
@@ -994,17 +994,17 @@
 
 
 def _extract_headings(text: str) -> List[_Heading]:
     """Return _Heading objects."""
     headings = []
     heading_regex = get_regexes('header')[0]
     for match in heading_regex.finditer(text):
-        start, end = match.span()
+        start, end = match.span(1)
         if not isDisabled(text, start) and not isDisabled(text, end):
-            headings.append(_Heading(match.group(), start, end))
+            headings.append(_Heading(match[1], start, end))
     return headings
 
 
 def _extract_sections(text: str, headings) -> List[Section]:
     """Return a list of :class:`Section` objects."""
     sections = []
     if headings:
```

### Comparing `pywikibot-8.2.0/pywikibot/throttle.py` & `pywikibot-8.3.0/pywikibot/throttle.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/time.py` & `pywikibot-8.3.0/pywikibot/time.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/titletranslate.py` & `pywikibot-8.3.0/pywikibot/titletranslate.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/tools/__init__.py` & `pywikibot-8.3.0/pywikibot/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/tools/_deprecate.py` & `pywikibot-8.3.0/pywikibot/tools/_deprecate.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/tools/_logging.py` & `pywikibot-8.3.0/pywikibot/tools/_logging.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/tools/_unidata.py` & `pywikibot-8.3.0/pywikibot/tools/_unidata.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/tools/chars.py` & `pywikibot-8.3.0/pywikibot/tools/chars.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/tools/collections.py` & `pywikibot-8.3.0/pywikibot/tools/collections.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/tools/djvu.py` & `pywikibot-8.3.0/pywikibot/tools/djvu.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/tools/formatter.py` & `pywikibot-8.3.0/pywikibot/tools/formatter.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/tools/itertools.py` & `pywikibot-8.3.0/pywikibot/tools/itertools.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/tools/threading.py` & `pywikibot-8.3.0/pywikibot/tools/threading.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/userinterfaces/__init__.py` & `pywikibot-8.3.0/pywikibot/userinterfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/userinterfaces/_interface_base.py` & `pywikibot-8.3.0/pywikibot/userinterfaces/_interface_base.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/userinterfaces/buffer_interface.py` & `pywikibot-8.3.0/pywikibot/userinterfaces/buffer_interface.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/userinterfaces/gui.py` & `pywikibot-8.3.0/pywikibot/userinterfaces/gui.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/userinterfaces/terminal_interface_base.py` & `pywikibot-8.3.0/pywikibot/userinterfaces/terminal_interface_base.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/userinterfaces/terminal_interface_unix.py` & `pywikibot-8.3.0/pywikibot/userinterfaces/terminal_interface_unix.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/userinterfaces/terminal_interface_win32.py` & `pywikibot-8.3.0/pywikibot/userinterfaces/terminal_interface_win32.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/userinterfaces/transliteration.py` & `pywikibot-8.3.0/pywikibot/userinterfaces/transliteration.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/version.py` & `pywikibot-8.3.0/pywikibot/version.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot/xmlreader.py` & `pywikibot-8.3.0/pywikibot/xmlreader.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot.egg-info/PKG-INFO` & `pywikibot-8.3.0/pywikibot.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywikibot
-Version: 8.2.0
+Version: 8.3.0
 Summary: Python MediaWiki Bot Framework
 Home-page: https://www.mediawiki.org/wiki/Manual:Pywikibot
 Download-URL: https://pywikibot.toolforge.org/
 Maintainer: The Pywikibot team
 Maintainer-email: pywikibot@lists.wikimedia.org
 License: MIT License
 Project-URL: Documentation, https://doc.wikimedia.org/pywikibot/stable/
@@ -257,36 +257,19 @@
 
 Roadmap
 =======
 
 Current release
 ---------------
 
-* Add support for gpewiki (T335989)
-* family.WikibaseFamilyand family.DefaultWikibaseFamilywere added to familymodule
-* Remove incorrect time normalization in page.Claim(T338748, T325860, T57755)
-* Add support for other types of diffs in Site.compare()
-* Improvements for textlib.extract_sectionsfunction (T338748)
-* Backport ``itertools.batched()`` from Python 3.12 which replaces tools.itertools.itergroup
-* Upcast page types in pagegenerators.RecentChangesPageGenerator(T340450)
-* Enable FilePage.download()to download thumbnails (T247095)
-* Refactor tools.compute_file_hashand use ``hashlib.file_digest`` with Python 3.11
-* Url ends with curly bracket in textlib.compileLinkR(T338029)
-* Allows spaces in environment variables for editor.TextEditor(T102465, T323078)
-* Add textlib.get_regexespublic function (T336144)
-* Return 'https' scheme with family.Family.protocol(T326046)
-* Use ``build`` instead of ``setuptools.setup()`` to build the distribution
-* Raise ``ConnectionError`` on ``requests.ReadTimeout`` in comms.http.error_handling_callback
-* Raise exceptions.ServerErroron ``requests.ReadTimeout`` in comms.http.error_handling_callback
-* Do not evaluate pywikibot.Sitewith dict.pop() as default value (T335720)
-* L10N updates
-* family.Familyclass was rewritten. ``obsolete.setter`` was removed,
-  family.Family.interwiki_replacementsreturns an invariant mapping,
-  family.Family.interwiki_removalsreturns a frozenset. ``closed_wikis``,
-  ``removed_wikis`` and ``code_aliases`` are family.Familyclass attributes.  (T334834)
+* Add support for btmwiktionary (T336117)
+* Add 'yue'/'zh-yue' code_aliases to family files (T341960)
+* All wbtypes are placed in ``pywkibot._wbtypes`` module
+* Use ``site.lang`` instead of ``site.code`` in comms.http.user_agent(T228322)
+* Make header extraction in textlib.extract_sectionsmore robust (T341787)
 
 
 Deprecations
 ------------
 
 * 8.2.0: *normalize* parameter of WbTime.toTimestrand WbTime.toWikibasewill be removed
 * 8.1.0: Dependency of exceptions.NoSiteLinkErrorfrom exceptions.NoPageErrorwill be removed
```

### Comparing `pywikibot-8.2.0/pywikibot.egg-info/SOURCES.txt` & `pywikibot-8.3.0/pywikibot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/pywikibot.egg-info/requires.txt` & `pywikibot-8.3.0/pywikibot.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/setup.py` & `pywikibot-8.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.2.0/tests/tests_tests.py` & `pywikibot-8.3.0/tests/tests_tests.py`

 * *Files identical despite different names*

