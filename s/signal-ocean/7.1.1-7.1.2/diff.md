# Comparing `tmp/signal-ocean-7.1.1.tar.gz` & `tmp/signal-ocean-7.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "signal-ocean-7.1.1.tar", last modified: Fri Jul 14 10:44:17 2023, max compression
+gzip compressed data, was "signal-ocean-7.1.2.tar", last modified: Thu Jul 27 11:11:39 2023, max compression
```

## Comparing `signal-ocean-7.1.1.tar` & `signal-ocean-7.1.2.tar`

### file list

```diff
@@ -1,150 +1,150 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:44:17.880928 signal-ocean-7.1.1/
--rw-rw-r--   0 root         (0) root         (0)    11357 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2175 2023-07-14 10:44:17.880928 signal-ocean-7.1.1/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     1184 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/README.md
--rw-rw-r--   0 root         (0) root         (0)       30 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/pyproject.toml
--rw-rw-r--   0 root         (0) root         (0)       73 2023-07-14 10:44:17.880928 signal-ocean-7.1.1/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1524 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:44:17.868927 signal-ocean-7.1.1/signal_ocean/
--rw-rw-r--   0 root         (0) root         (0)     1151 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1886 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/_internals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:44:17.868927 signal-ocean-7.1.1/signal_ocean/companies/
--rw-rw-r--   0 root         (0) root         (0)      236 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/companies/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1768 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/companies/companies_api.py
--rw-rw-r--   0 root         (0) root         (0)     3020 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/companies/models.py
--rw-rw-r--   0 root         (0) root         (0)     2511 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/connection.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:44:17.868927 signal-ocean-7.1.1/signal_ocean/distances/
--rw-rw-r--   0 root         (0) root         (0)     1210 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/distances/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2523 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/distances/_distances_json.py
--rw-rw-r--   0 root         (0) root         (0)    11714 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/distances/distances_api.py
--rw-rw-r--   0 root         (0) root         (0)      287 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/distances/loading_condition.py
--rw-rw-r--   0 root         (0) root         (0)     4589 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/distances/models.py
--rw-rw-r--   0 root         (0) root         (0)      266 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/distances/port.py
--rw-rw-r--   0 root         (0) root         (0)      777 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/distances/port_filter.py
--rw-rw-r--   0 root         (0) root         (0)      306 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/distances/vessel_class.py
--rw-rw-r--   0 root         (0) root         (0)      897 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/distances/vessel_class_filter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:44:17.868927 signal-ocean-7.1.1/signal_ocean/freight_pricing/
--rw-rw-r--   0 root         (0) root         (0)     1318 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/freight_pricing/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1113 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/freight_pricing/_freight_pricing_json.py
--rw-rw-r--   0 root         (0) root         (0)     4766 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/freight_pricing/freight_pricing_api.py
--rw-rw-r--   0 root         (0) root         (0)     1274 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/freight_pricing/models.py
--rw-rw-r--   0 root         (0) root         (0)      266 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/freight_pricing/port.py
--rw-rw-r--   0 root         (0) root         (0)      777 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/freight_pricing/port_filter.py
--rw-rw-r--   0 root         (0) root         (0)      306 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/freight_pricing/vessel_class.py
--rw-rw-r--   0 root         (0) root         (0)      897 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/freight_pricing/vessel_class_filter.py
--rw-rw-r--   0 root         (0) root         (0)      167 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/freight_pricing/vessel_subclass.py
--rw-rw-r--   0 root         (0) root         (0)      263 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/freight_pricing/vessel_type.py
--rw-rw-r--   0 root         (0) root         (0)      877 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/freight_pricing/vessel_type_filter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:44:17.872928 signal-ocean-7.1.1/signal_ocean/freight_rates/
--rw-rw-r--   0 root         (0) root         (0)      565 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/freight_rates/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2145 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/freight_rates/_freight_rates_json.py
--rw-rw-r--   0 root         (0) root         (0)      524 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/freight_rates/enums.py
--rw-rw-r--   0 root         (0) root         (0)     3750 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/freight_rates/freight_rates_api.py
--rw-rw-r--   0 root         (0) root         (0)     1820 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/freight_rates/models.py
--rw-rw-r--   0 root         (0) root         (0)      793 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/freight_rates/port_filter.py
--rw-rw-r--   0 root         (0) root         (0)     1278 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/freight_rates/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:44:17.872928 signal-ocean-7.1.1/signal_ocean/geos/
--rw-rw-r--   0 root         (0) root         (0)      132 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/geos/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4338 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/geos/geos_api.py
--rw-rw-r--   0 root         (0) root         (0)     6299 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/geos/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:44:17.872928 signal-ocean-7.1.1/signal_ocean/historical_tonnage_list/
--rw-rw-r--   0 root         (0) root         (0)     2261 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/historical_tonnage_list/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2559 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/historical_tonnage_list/_historical_tonnage_list_json.py
--rw-rw-r--   0 root         (0) root         (0)      331 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/historical_tonnage_list/area.py
--rw-rw-r--   0 root         (0) root         (0)     2537 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/historical_tonnage_list/column.py
--rw-rw-r--   0 root         (0) root         (0)      675 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/historical_tonnage_list/commercial_status.py
--rw-rw-r--   0 root         (0) root         (0)      235 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/historical_tonnage_list/fixture_type.py
--rw-rw-r--   0 root         (0) root         (0)     2105 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/historical_tonnage_list/historical_tonnage_list.py
--rw-rw-r--   0 root         (0) root         (0)     4968 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/historical_tonnage_list/historical_tonnage_list_api.py
--rw-rw-r--   0 root         (0) root         (0)      208 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/historical_tonnage_list/index_level.py
--rw-rw-r--   0 root         (0) root         (0)      493 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/historical_tonnage_list/location_taxonomy.py
--rw-rw-r--   0 root         (0) root         (0)     1004 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/historical_tonnage_list/market_deployment.py
--rw-rw-r--   0 root         (0) root         (0)     1292 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/historical_tonnage_list/operational_status.py
--rw-rw-r--   0 root         (0) root         (0)      510 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/historical_tonnage_list/push_type.py
--rw-rw-r--   0 root         (0) root         (0)      552 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/historical_tonnage_list/tonnage_list.py
--rw-rw-r--   0 root         (0) root         (0)     5517 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/historical_tonnage_list/vessel.py
--rw-rw-r--   0 root         (0) root         (0)     6831 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/historical_tonnage_list/vessel_filter.py
--rw-rw-r--   0 root         (0) root         (0)      632 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/historical_tonnage_list/vessel_subclass.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:44:17.872928 signal-ocean-7.1.1/signal_ocean/market_rates/
--rw-rw-r--   0 root         (0) root         (0)      536 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/market_rates/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1909 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/market_rates/_market_rates_json.py
--rw-rw-r--   0 root         (0) root         (0)      178 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/market_rates/enums.py
--rw-rw-r--   0 root         (0) root         (0)     4006 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/market_rates/market_rates_api.py
--rw-rw-r--   0 root         (0) root         (0)     2548 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/market_rates/models.py
--rw-rw-r--   0 root         (0) root         (0)      773 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/market_rates/utils.py
--rw-rw-r--   0 root         (0) root         (0)     2029 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/market_rates/vessel_classes.py
--rw-rw-r--   0 root         (0) root         (0)     2299 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/plots.py
--rw-rw-r--   0 root         (0) root         (0)      578 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/port.py
--rw-rw-r--   0 root         (0) root         (0)     1489 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/port_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:44:17.876927 signal-ocean-7.1.1/signal_ocean/port_congestion/
--rw-rw-r--   0 root         (0) root         (0)      347 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/port_congestion/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4274 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/port_congestion/models.py
--rw-rw-r--   0 root         (0) root         (0)    19251 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/port_congestion/port_congestion.py
--rw-rw-r--   0 root         (0) root         (0)     4670 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/port_congestion/port_congestion_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:44:17.876927 signal-ocean-7.1.1/signal_ocean/port_expenses/
--rw-rw-r--   0 root         (0) root         (0)     1026 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/port_expenses/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1433 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/port_expenses/_port_expenses_json.py
--rw-rw-r--   0 root         (0) root         (0)      823 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/port_expenses/enums.py
--rw-rw-r--   0 root         (0) root         (0)     1867 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/port_expenses/models.py
--rw-rw-r--   0 root         (0) root         (0)     8527 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/port_expenses/port_expenses_api.py
--rw-rw-r--   0 root         (0) root         (0)      779 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/port_expenses/port_filter.py
--rw-rw-r--   0 root         (0) root         (0)     1147 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/port_filter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:44:17.876927 signal-ocean-7.1.1/signal_ocean/scraped_cargoes/
--rw-rw-r--   0 root         (0) root         (0)      277 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/scraped_cargoes/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    26586 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/scraped_cargoes/models.py
--rw-rw-r--   0 root         (0) root         (0)     5363 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/scraped_cargoes/scraped_cargoes_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:44:17.876927 signal-ocean-7.1.1/signal_ocean/scraped_data/
--rw-rw-r--   0 root         (0) root         (0)       41 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/scraped_data/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4560 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/scraped_data/scraped_data_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:44:17.876927 signal-ocean-7.1.1/signal_ocean/scraped_fixtures/
--rw-rw-r--   0 root         (0) root         (0)      291 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/scraped_fixtures/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    32666 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/scraped_fixtures/models.py
--rw-rw-r--   0 root         (0) root         (0)     6009 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/scraped_fixtures/scraped_fixtures_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:44:17.876927 signal-ocean-7.1.1/signal_ocean/scraped_lineups/
--rw-rw-r--   0 root         (0) root         (0)      281 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/scraped_lineups/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    21114 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/scraped_lineups/models.py
--rw-rw-r--   0 root         (0) root         (0)     5968 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/scraped_lineups/scraped_lineups_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:44:17.876927 signal-ocean-7.1.1/signal_ocean/scraped_positions/
--rw-rw-r--   0 root         (0) root         (0)      301 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/scraped_positions/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    16973 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/scraped_positions/models.py
--rw-rw-r--   0 root         (0) root         (0)     6044 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/scraped_positions/scraped_positions_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:44:17.876927 signal-ocean-7.1.1/signal_ocean/tonnage_list/
--rw-rw-r--   0 root         (0) root         (0)      879 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/tonnage_list/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3345 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/tonnage_list/_json.py
--rw-rw-r--   0 root         (0) root         (0)     6084 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/tonnage_list/api.py
--rw-rw-r--   0 root         (0) root         (0)     7229 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/tonnage_list/data_frame.py
--rw-rw-r--   0 root         (0) root         (0)    26447 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/tonnage_list/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:44:17.876927 signal-ocean-7.1.1/signal_ocean/util/
--rw-rw-r--   0 root         (0) root         (0)       56 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/util/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6505 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/util/parsing_helpers.py
--rw-rw-r--   0 root         (0) root         (0)     6529 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/util/request_helpers.py
--rw-rw-r--   0 root         (0) root         (0)      647 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/vessel_class.py
--rw-rw-r--   0 root         (0) root         (0)     1653 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/vessel_class_api.py
--rw-rw-r--   0 root         (0) root         (0)     1296 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/vessel_class_filter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:44:17.876927 signal-ocean-7.1.1/signal_ocean/vessel_emissions/
--rw-rw-r--   0 root         (0) root         (0)      761 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/vessel_emissions/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    15668 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/vessel_emissions/models.py
--rw-rw-r--   0 root         (0) root         (0)    14610 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/vessel_emissions/vessel_emissions_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:44:17.880928 signal-ocean-7.1.1/signal_ocean/vessel_valuations/
--rw-rw-r--   0 root         (0) root         (0)      298 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/vessel_valuations/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      595 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/vessel_valuations/_valuation_json.py
--rw-rw-r--   0 root         (0) root         (0)      608 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/vessel_valuations/models.py
--rw-rw-r--   0 root         (0) root         (0)     2679 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/vessel_valuations/vessel_valuations_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:44:17.880928 signal-ocean-7.1.1/signal_ocean/vessels/
--rw-rw-r--   0 root         (0) root         (0)      378 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/vessels/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    17416 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/vessels/models.py
--rw-rw-r--   0 root         (0) root         (0)     3539 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/vessels/vessels_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:44:17.880928 signal-ocean-7.1.1/signal_ocean/voyages/
--rw-rw-r--   0 root         (0) root         (0)     1298 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/voyages/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    46003 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/voyages/models.py
--rw-rw-r--   0 root         (0) root         (0)    44702 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/voyages/voyages_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:44:17.880928 signal-ocean-7.1.1/signal_ocean/voyages_market_data/
--rw-rw-r--   0 root         (0) root         (0)      539 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/voyages_market_data/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    15350 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/voyages_market_data/models.py
--rw-rw-r--   0 root         (0) root         (0)    15865 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/voyages_market_data/voyages_market_data_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:44:17.868927 signal-ocean-7.1.1/signal_ocean.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2175 2023-07-14 10:44:17.000000 signal-ocean-7.1.1/signal_ocean.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5081 2023-07-14 10:44:17.000000 signal-ocean-7.1.1/signal_ocean.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 10:44:17.000000 signal-ocean-7.1.1/signal_ocean.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      124 2023-07-14 10:44:17.000000 signal-ocean-7.1.1/signal_ocean.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-14 10:44:17.000000 signal-ocean-7.1.1/signal_ocean.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 11:11:39.763193 signal-ocean-7.1.2/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2175 2023-07-27 11:11:39.763193 signal-ocean-7.1.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1184 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/README.md
+-rw-r--r--   0 root         (0) root         (0)       30 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-27 11:11:39.767193 signal-ocean-7.1.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1524 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 11:11:39.751193 signal-ocean-7.1.2/signal_ocean/
+-rw-r--r--   0 root         (0) root         (0)     1151 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1886 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/_internals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 11:11:39.751193 signal-ocean-7.1.2/signal_ocean/companies/
+-rw-r--r--   0 root         (0) root         (0)      236 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/companies/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1768 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/companies/companies_api.py
+-rw-r--r--   0 root         (0) root         (0)     3020 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/companies/models.py
+-rw-r--r--   0 root         (0) root         (0)     2511 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/connection.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 11:11:39.751193 signal-ocean-7.1.2/signal_ocean/distances/
+-rw-r--r--   0 root         (0) root         (0)     1210 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/distances/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2523 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/distances/_distances_json.py
+-rw-r--r--   0 root         (0) root         (0)    11714 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/distances/distances_api.py
+-rw-r--r--   0 root         (0) root         (0)      287 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/distances/loading_condition.py
+-rw-r--r--   0 root         (0) root         (0)     4589 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/distances/models.py
+-rw-r--r--   0 root         (0) root         (0)      266 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/distances/port.py
+-rw-r--r--   0 root         (0) root         (0)      777 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/distances/port_filter.py
+-rw-r--r--   0 root         (0) root         (0)      306 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/distances/vessel_class.py
+-rw-r--r--   0 root         (0) root         (0)      897 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/distances/vessel_class_filter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 11:11:39.755193 signal-ocean-7.1.2/signal_ocean/freight_pricing/
+-rw-r--r--   0 root         (0) root         (0)     1318 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/freight_pricing/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1113 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/freight_pricing/_freight_pricing_json.py
+-rw-r--r--   0 root         (0) root         (0)     4766 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/freight_pricing/freight_pricing_api.py
+-rw-r--r--   0 root         (0) root         (0)     1274 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/freight_pricing/models.py
+-rw-r--r--   0 root         (0) root         (0)      266 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/freight_pricing/port.py
+-rw-r--r--   0 root         (0) root         (0)      777 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/freight_pricing/port_filter.py
+-rw-r--r--   0 root         (0) root         (0)      306 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/freight_pricing/vessel_class.py
+-rw-r--r--   0 root         (0) root         (0)      897 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/freight_pricing/vessel_class_filter.py
+-rw-r--r--   0 root         (0) root         (0)      167 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/freight_pricing/vessel_subclass.py
+-rw-r--r--   0 root         (0) root         (0)      263 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/freight_pricing/vessel_type.py
+-rw-r--r--   0 root         (0) root         (0)      877 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/freight_pricing/vessel_type_filter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 11:11:39.755193 signal-ocean-7.1.2/signal_ocean/freight_rates/
+-rw-r--r--   0 root         (0) root         (0)      565 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/freight_rates/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2145 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/freight_rates/_freight_rates_json.py
+-rw-r--r--   0 root         (0) root         (0)      524 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/freight_rates/enums.py
+-rw-r--r--   0 root         (0) root         (0)     3750 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/freight_rates/freight_rates_api.py
+-rw-r--r--   0 root         (0) root         (0)     1820 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/freight_rates/models.py
+-rw-r--r--   0 root         (0) root         (0)      793 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/freight_rates/port_filter.py
+-rw-r--r--   0 root         (0) root         (0)     1278 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/freight_rates/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 11:11:39.755193 signal-ocean-7.1.2/signal_ocean/geos/
+-rw-r--r--   0 root         (0) root         (0)      132 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/geos/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4338 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/geos/geos_api.py
+-rw-r--r--   0 root         (0) root         (0)     6299 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/geos/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 11:11:39.755193 signal-ocean-7.1.2/signal_ocean/historical_tonnage_list/
+-rw-r--r--   0 root         (0) root         (0)     2261 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/historical_tonnage_list/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2559 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/historical_tonnage_list/_historical_tonnage_list_json.py
+-rw-r--r--   0 root         (0) root         (0)      331 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/historical_tonnage_list/area.py
+-rw-r--r--   0 root         (0) root         (0)     2537 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/historical_tonnage_list/column.py
+-rw-r--r--   0 root         (0) root         (0)      675 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/historical_tonnage_list/commercial_status.py
+-rw-r--r--   0 root         (0) root         (0)      235 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/historical_tonnage_list/fixture_type.py
+-rw-r--r--   0 root         (0) root         (0)     2105 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/historical_tonnage_list/historical_tonnage_list.py
+-rw-r--r--   0 root         (0) root         (0)     4968 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/historical_tonnage_list/historical_tonnage_list_api.py
+-rw-r--r--   0 root         (0) root         (0)      208 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/historical_tonnage_list/index_level.py
+-rw-r--r--   0 root         (0) root         (0)      493 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/historical_tonnage_list/location_taxonomy.py
+-rw-r--r--   0 root         (0) root         (0)     1004 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/historical_tonnage_list/market_deployment.py
+-rw-r--r--   0 root         (0) root         (0)     1292 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/historical_tonnage_list/operational_status.py
+-rw-r--r--   0 root         (0) root         (0)      510 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/historical_tonnage_list/push_type.py
+-rw-r--r--   0 root         (0) root         (0)      552 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/historical_tonnage_list/tonnage_list.py
+-rw-r--r--   0 root         (0) root         (0)     5517 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/historical_tonnage_list/vessel.py
+-rw-r--r--   0 root         (0) root         (0)     6831 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/historical_tonnage_list/vessel_filter.py
+-rw-r--r--   0 root         (0) root         (0)      632 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/historical_tonnage_list/vessel_subclass.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 11:11:39.755193 signal-ocean-7.1.2/signal_ocean/market_rates/
+-rw-r--r--   0 root         (0) root         (0)      536 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/market_rates/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1909 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/market_rates/_market_rates_json.py
+-rw-r--r--   0 root         (0) root         (0)      178 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/market_rates/enums.py
+-rw-r--r--   0 root         (0) root         (0)     4006 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/market_rates/market_rates_api.py
+-rw-r--r--   0 root         (0) root         (0)     2548 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/market_rates/models.py
+-rw-r--r--   0 root         (0) root         (0)      773 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/market_rates/utils.py
+-rw-r--r--   0 root         (0) root         (0)     2029 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/market_rates/vessel_classes.py
+-rw-r--r--   0 root         (0) root         (0)     2299 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/plots.py
+-rw-r--r--   0 root         (0) root         (0)      578 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/port.py
+-rw-r--r--   0 root         (0) root         (0)     1489 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/port_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 11:11:39.759193 signal-ocean-7.1.2/signal_ocean/port_congestion/
+-rw-r--r--   0 root         (0) root         (0)      347 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/port_congestion/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4274 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/port_congestion/models.py
+-rw-r--r--   0 root         (0) root         (0)    19251 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/port_congestion/port_congestion.py
+-rw-r--r--   0 root         (0) root         (0)     4670 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/port_congestion/port_congestion_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 11:11:39.759193 signal-ocean-7.1.2/signal_ocean/port_expenses/
+-rw-r--r--   0 root         (0) root         (0)     1026 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/port_expenses/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1433 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/port_expenses/_port_expenses_json.py
+-rw-r--r--   0 root         (0) root         (0)      823 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/port_expenses/enums.py
+-rw-r--r--   0 root         (0) root         (0)     1867 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/port_expenses/models.py
+-rw-r--r--   0 root         (0) root         (0)     8527 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/port_expenses/port_expenses_api.py
+-rw-r--r--   0 root         (0) root         (0)      779 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/port_expenses/port_filter.py
+-rw-r--r--   0 root         (0) root         (0)     1147 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/port_filter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 11:11:39.759193 signal-ocean-7.1.2/signal_ocean/scraped_cargoes/
+-rw-r--r--   0 root         (0) root         (0)      277 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/scraped_cargoes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26586 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/scraped_cargoes/models.py
+-rw-r--r--   0 root         (0) root         (0)     5363 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/scraped_cargoes/scraped_cargoes_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 11:11:39.759193 signal-ocean-7.1.2/signal_ocean/scraped_data/
+-rw-r--r--   0 root         (0) root         (0)       41 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/scraped_data/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4560 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/scraped_data/scraped_data_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 11:11:39.759193 signal-ocean-7.1.2/signal_ocean/scraped_fixtures/
+-rw-r--r--   0 root         (0) root         (0)      291 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/scraped_fixtures/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32666 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/scraped_fixtures/models.py
+-rw-r--r--   0 root         (0) root         (0)     6009 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/scraped_fixtures/scraped_fixtures_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 11:11:39.759193 signal-ocean-7.1.2/signal_ocean/scraped_lineups/
+-rw-r--r--   0 root         (0) root         (0)      281 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/scraped_lineups/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21114 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/scraped_lineups/models.py
+-rw-r--r--   0 root         (0) root         (0)     5968 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/scraped_lineups/scraped_lineups_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 11:11:39.759193 signal-ocean-7.1.2/signal_ocean/scraped_positions/
+-rw-r--r--   0 root         (0) root         (0)      301 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/scraped_positions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16973 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/scraped_positions/models.py
+-rw-r--r--   0 root         (0) root         (0)     6044 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/scraped_positions/scraped_positions_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 11:11:39.759193 signal-ocean-7.1.2/signal_ocean/tonnage_list/
+-rw-r--r--   0 root         (0) root         (0)      879 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/tonnage_list/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3345 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/tonnage_list/_json.py
+-rw-r--r--   0 root         (0) root         (0)     6084 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/tonnage_list/api.py
+-rw-r--r--   0 root         (0) root         (0)     7229 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/tonnage_list/data_frame.py
+-rw-r--r--   0 root         (0) root         (0)    26447 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/tonnage_list/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 11:11:39.759193 signal-ocean-7.1.2/signal_ocean/util/
+-rw-r--r--   0 root         (0) root         (0)       56 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6505 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/util/parsing_helpers.py
+-rw-r--r--   0 root         (0) root         (0)     6529 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/util/request_helpers.py
+-rw-r--r--   0 root         (0) root         (0)      647 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/vessel_class.py
+-rw-r--r--   0 root         (0) root         (0)     1653 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/vessel_class_api.py
+-rw-r--r--   0 root         (0) root         (0)     1296 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/vessel_class_filter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 11:11:39.759193 signal-ocean-7.1.2/signal_ocean/vessel_emissions/
+-rw-r--r--   0 root         (0) root         (0)      761 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/vessel_emissions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15668 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/vessel_emissions/models.py
+-rw-r--r--   0 root         (0) root         (0)    14610 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/vessel_emissions/vessel_emissions_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 11:11:39.763193 signal-ocean-7.1.2/signal_ocean/vessel_valuations/
+-rw-r--r--   0 root         (0) root         (0)      298 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/vessel_valuations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      595 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/vessel_valuations/_valuation_json.py
+-rw-r--r--   0 root         (0) root         (0)      608 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/vessel_valuations/models.py
+-rw-r--r--   0 root         (0) root         (0)     2679 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/vessel_valuations/vessel_valuations_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 11:11:39.763193 signal-ocean-7.1.2/signal_ocean/vessels/
+-rw-r--r--   0 root         (0) root         (0)      378 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/vessels/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17416 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/vessels/models.py
+-rw-r--r--   0 root         (0) root         (0)     3539 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/vessels/vessels_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 11:11:39.763193 signal-ocean-7.1.2/signal_ocean/voyages/
+-rw-r--r--   0 root         (0) root         (0)     1298 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/voyages/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    46114 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/voyages/models.py
+-rw-r--r--   0 root         (0) root         (0)    44712 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/voyages/voyages_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 11:11:39.763193 signal-ocean-7.1.2/signal_ocean/voyages_market_data/
+-rw-r--r--   0 root         (0) root         (0)      539 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/voyages_market_data/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15350 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/voyages_market_data/models.py
+-rw-r--r--   0 root         (0) root         (0)    15865 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/voyages_market_data/voyages_market_data_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 11:11:39.751193 signal-ocean-7.1.2/signal_ocean.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2175 2023-07-27 11:11:39.000000 signal-ocean-7.1.2/signal_ocean.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5081 2023-07-27 11:11:39.000000 signal-ocean-7.1.2/signal_ocean.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 11:11:39.000000 signal-ocean-7.1.2/signal_ocean.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      124 2023-07-27 11:11:39.000000 signal-ocean-7.1.2/signal_ocean.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-27 11:11:39.000000 signal-ocean-7.1.2/signal_ocean.egg-info/top_level.txt
```

### Comparing `signal-ocean-7.1.1/LICENSE` & `signal-ocean-7.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/PKG-INFO` & `signal-ocean-7.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: signal-ocean
-Version: 7.1.1
+Version: 7.1.2
 Summary: Access Signal Ocean Platform data using Python.
 Home-page: https://apis.signalocean.com/
 Author: Signal Ocean Developers
 Author-email: signaloceandevelopers@thesignalgroup.com
 License: Apache 2.0
 Project-URL: The Signal Group, https://www.thesignalgroup.com/
 Project-URL: Signal Ocean, https://www.signalocean.com/
```

### Comparing `signal-ocean-7.1.1/README.md` & `signal-ocean-7.1.2/README.md`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/setup.py` & `signal-ocean-7.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/signal_ocean/__init__.py` & `signal-ocean-7.1.2/signal_ocean/__init__.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/signal_ocean/_internals.py` & `signal-ocean-7.1.2/signal_ocean/_internals.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/signal_ocean/companies/companies_api.py` & `signal-ocean-7.1.2/signal_ocean/companies/companies_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/signal_ocean/companies/models.py` & `signal-ocean-7.1.2/signal_ocean/companies/models.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/signal_ocean/connection.py` & `signal-ocean-7.1.2/signal_ocean/connection.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/signal_ocean/distances/__init__.py` & `signal-ocean-7.1.2/signal_ocean/distances/__init__.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/signal_ocean/distances/_distances_json.py` & `signal-ocean-7.1.2/signal_ocean/distances/_distances_json.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/signal_ocean/distances/distances_api.py` & `signal-ocean-7.1.2/signal_ocean/distances/distances_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/signal_ocean/distances/models.py` & `signal-ocean-7.1.2/signal_ocean/distances/models.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/signal_ocean/distances/port_filter.py` & `signal-ocean-7.1.2/signal_ocean/distances/port_filter.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/signal_ocean/distances/vessel_class_filter.py` & `signal-ocean-7.1.2/signal_ocean/distances/vessel_class_filter.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/signal_ocean/freight_pricing/__init__.py` & `signal-ocean-7.1.2/signal_ocean/freight_pricing/__init__.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/signal_ocean/freight_pricing/_freight_pricing_json.py` & `signal-ocean-7.1.2/signal_ocean/freight_pricing/_freight_pricing_json.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/signal_ocean/freight_pricing/freight_pricing_api.py` & `signal-ocean-7.1.2/signal_ocean/freight_pricing/freight_pricing_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/signal_ocean/freight_pricing/models.py` & `signal-ocean-7.1.2/signal_ocean/freight_pricing/models.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/signal_ocean/freight_pricing/port_filter.py` & `signal-ocean-7.1.2/signal_ocean/freight_pricing/port_filter.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/signal_ocean/freight_pricing/vessel_class_filter.py` & `signal-ocean-7.1.2/signal_ocean/freight_pricing/vessel_class_filter.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/signal_ocean/freight_pricing/vessel_type_filter.py` & `signal-ocean-7.1.2/signal_ocean/freight_pricing/vessel_type_filter.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/signal_ocean/freight_rates/__init__.py` & `signal-ocean-7.1.2/signal_ocean/freight_rates/__init__.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/signal_ocean/freight_rates/_freight_rates_json.py` & `signal-ocean-7.1.2/signal_ocean/freight_rates/_freight_rates_json.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/signal_ocean/freight_rates/enums.py` & `signal-ocean-7.1.2/signal_ocean/freight_rates/enums.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/signal_ocean/freight_rates/freight_rates_api.py` & `signal-ocean-7.1.2/signal_ocean/freight_rates/freight_rates_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/signal_ocean/freight_rates/models.py` & `signal-ocean-7.1.2/signal_ocean/freight_rates/models.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/signal_ocean/freight_rates/port_filter.py` & `signal-ocean-7.1.2/signal_ocean/freight_rates/port_filter.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/signal_ocean/freight_rates/utils.py` & `signal-ocean-7.1.2/signal_ocean/freight_rates/utils.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/signal_ocean/geos/geos_api.py` & `signal-ocean-7.1.2/signal_ocean/geos/geos_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/signal_ocean/geos/models.py` & `signal-ocean-7.1.2/signal_ocean/geos/models.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/signal_ocean/historical_tonnage_list/__init__.py` & `signal-ocean-7.1.2/signal_ocean/historical_tonnage_list/__init__.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/signal_ocean/historical_tonnage_list/_historical_tonnage_list_json.py` & `signal-ocean-7.1.2/signal_ocean/historical_tonnage_list/_historical_tonnage_list_json.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/signal_ocean/historical_tonnage_list/column.py` & `signal-ocean-7.1.2/signal_ocean/historical_tonnage_list/column.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/signal_ocean/historical_tonnage_list/commercial_status.py` & `signal-ocean-7.1.2/signal_ocean/historical_tonnage_list/commercial_status.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/signal_ocean/historical_tonnage_list/historical_tonnage_list.py` & `signal-ocean-7.1.2/signal_ocean/historical_tonnage_list/historical_tonnage_list.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/signal_ocean/historical_tonnage_list/historical_tonnage_list_api.py` & `signal-ocean-7.1.2/signal_ocean/historical_tonnage_list/historical_tonnage_list_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/signal_ocean/historical_tonnage_list/market_deployment.py` & `signal-ocean-7.1.2/signal_ocean/historical_tonnage_list/market_deployment.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/signal_ocean/historical_tonnage_list/operational_status.py` & `signal-ocean-7.1.2/signal_ocean/historical_tonnage_list/operational_status.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/signal_ocean/historical_tonnage_list/tonnage_list.py` & `signal-ocean-7.1.2/signal_ocean/historical_tonnage_list/tonnage_list.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/signal_ocean/historical_tonnage_list/vessel.py` & `signal-ocean-7.1.2/signal_ocean/historical_tonnage_list/vessel.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/signal_ocean/historical_tonnage_list/vessel_filter.py` & `signal-ocean-7.1.2/signal_ocean/historical_tonnage_list/vessel_filter.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/signal_ocean/historical_tonnage_list/vessel_subclass.py` & `signal-ocean-7.1.2/signal_ocean/historical_tonnage_list/vessel_subclass.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/signal_ocean/market_rates/__init__.py` & `signal-ocean-7.1.2/signal_ocean/market_rates/__init__.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/signal_ocean/market_rates/_market_rates_json.py` & `signal-ocean-7.1.2/signal_ocean/market_rates/_market_rates_json.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/signal_ocean/market_rates/market_rates_api.py` & `signal-ocean-7.1.2/signal_ocean/market_rates/market_rates_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/signal_ocean/market_rates/models.py` & `signal-ocean-7.1.2/signal_ocean/market_rates/models.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/signal_ocean/market_rates/utils.py` & `signal-ocean-7.1.2/signal_ocean/market_rates/utils.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/signal_ocean/market_rates/vessel_classes.py` & `signal-ocean-7.1.2/signal_ocean/market_rates/vessel_classes.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/signal_ocean/plots.py` & `signal-ocean-7.1.2/signal_ocean/plots.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/signal_ocean/port.py` & `signal-ocean-7.1.2/signal_ocean/port.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/signal_ocean/port_api.py` & `signal-ocean-7.1.2/signal_ocean/port_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/signal_ocean/port_congestion/models.py` & `signal-ocean-7.1.2/signal_ocean/port_congestion/models.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/signal_ocean/port_congestion/port_congestion.py` & `signal-ocean-7.1.2/signal_ocean/port_congestion/port_congestion.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/signal_ocean/port_congestion/port_congestion_api.py` & `signal-ocean-7.1.2/signal_ocean/port_congestion/port_congestion_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/signal_ocean/port_expenses/__init__.py` & `signal-ocean-7.1.2/signal_ocean/port_expenses/__init__.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/signal_ocean/port_expenses/_port_expenses_json.py` & `signal-ocean-7.1.2/signal_ocean/port_expenses/_port_expenses_json.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/signal_ocean/port_expenses/enums.py` & `signal-ocean-7.1.2/signal_ocean/port_expenses/enums.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/signal_ocean/port_expenses/models.py` & `signal-ocean-7.1.2/signal_ocean/port_expenses/models.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/signal_ocean/port_expenses/port_expenses_api.py` & `signal-ocean-7.1.2/signal_ocean/port_expenses/port_expenses_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/signal_ocean/port_expenses/port_filter.py` & `signal-ocean-7.1.2/signal_ocean/port_expenses/port_filter.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/signal_ocean/port_filter.py` & `signal-ocean-7.1.2/signal_ocean/port_filter.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/signal_ocean/scraped_cargoes/models.py` & `signal-ocean-7.1.2/signal_ocean/scraped_cargoes/models.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/signal_ocean/scraped_cargoes/scraped_cargoes_api.py` & `signal-ocean-7.1.2/signal_ocean/scraped_cargoes/scraped_cargoes_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/signal_ocean/scraped_data/scraped_data_api.py` & `signal-ocean-7.1.2/signal_ocean/scraped_data/scraped_data_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/signal_ocean/scraped_fixtures/models.py` & `signal-ocean-7.1.2/signal_ocean/scraped_fixtures/models.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/signal_ocean/scraped_fixtures/scraped_fixtures_api.py` & `signal-ocean-7.1.2/signal_ocean/scraped_fixtures/scraped_fixtures_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/signal_ocean/scraped_lineups/models.py` & `signal-ocean-7.1.2/signal_ocean/scraped_lineups/models.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/signal_ocean/scraped_lineups/scraped_lineups_api.py` & `signal-ocean-7.1.2/signal_ocean/scraped_lineups/scraped_lineups_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/signal_ocean/scraped_positions/models.py` & `signal-ocean-7.1.2/signal_ocean/scraped_positions/models.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/signal_ocean/scraped_positions/scraped_positions_api.py` & `signal-ocean-7.1.2/signal_ocean/scraped_positions/scraped_positions_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/signal_ocean/tonnage_list/__init__.py` & `signal-ocean-7.1.2/signal_ocean/tonnage_list/__init__.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/signal_ocean/tonnage_list/_json.py` & `signal-ocean-7.1.2/signal_ocean/tonnage_list/_json.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/signal_ocean/tonnage_list/api.py` & `signal-ocean-7.1.2/signal_ocean/tonnage_list/api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/signal_ocean/tonnage_list/data_frame.py` & `signal-ocean-7.1.2/signal_ocean/tonnage_list/data_frame.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/signal_ocean/tonnage_list/models.py` & `signal-ocean-7.1.2/signal_ocean/tonnage_list/models.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/signal_ocean/util/parsing_helpers.py` & `signal-ocean-7.1.2/signal_ocean/util/parsing_helpers.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/signal_ocean/util/request_helpers.py` & `signal-ocean-7.1.2/signal_ocean/util/request_helpers.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/signal_ocean/vessel_class.py` & `signal-ocean-7.1.2/signal_ocean/vessel_class.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/signal_ocean/vessel_class_api.py` & `signal-ocean-7.1.2/signal_ocean/vessel_class_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/signal_ocean/vessel_class_filter.py` & `signal-ocean-7.1.2/signal_ocean/vessel_class_filter.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/signal_ocean/vessel_emissions/__init__.py` & `signal-ocean-7.1.2/signal_ocean/vessel_emissions/__init__.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/signal_ocean/vessel_emissions/models.py` & `signal-ocean-7.1.2/signal_ocean/vessel_emissions/models.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/signal_ocean/vessel_emissions/vessel_emissions_api.py` & `signal-ocean-7.1.2/signal_ocean/vessel_emissions/vessel_emissions_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/signal_ocean/vessel_valuations/_valuation_json.py` & `signal-ocean-7.1.2/signal_ocean/vessel_valuations/_valuation_json.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/signal_ocean/vessel_valuations/models.py` & `signal-ocean-7.1.2/signal_ocean/vessel_valuations/models.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/signal_ocean/vessel_valuations/vessel_valuations_api.py` & `signal-ocean-7.1.2/signal_ocean/vessel_valuations/vessel_valuations_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/signal_ocean/vessels/models.py` & `signal-ocean-7.1.2/signal_ocean/vessels/models.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/signal_ocean/vessels/vessels_api.py` & `signal-ocean-7.1.2/signal_ocean/vessels/vessels_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/signal_ocean/voyages/__init__.py` & `signal-ocean-7.1.2/signal_ocean/voyages/__init__.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/signal_ocean/voyages/models.py` & `signal-ocean-7.1.2/signal_ocean/voyages/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -192,14 +192,16 @@
     sts_id: Optional[str] = None
     geo_asset_id: Optional[int] = None
     geo_asset_name: Optional[str] = None
     latitude: Optional[float] = None
     longitude: Optional[float] = None
     other_vessel_imo: Optional[int] = None
     other_vessel_name: Optional[str] = None
+    floating_storage_start_date: Optional[datetime] = None
+    floating_storage_duration: Optional[int] = None
 
 
 @dataclass(frozen=True)
 class VoyageEvent:
     """An event associated with a voyage of a vessel.
 
     Voyage events describe the start of the voyage, a stop or a port call that
```

### Comparing `signal-ocean-7.1.1/signal_ocean/voyages/voyages_api.py` & `signal-ocean-7.1.2/signal_ocean/voyages/voyages_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 VoyagesCondensed = Tuple[VoyageCondensed, ...]
 NextRequestToken = str
 
 
 class VoyagesAPI:
     """Represents Signal's Voyages API."""
 
-    relative_url = "voyages-api/v3/"
+    relative_url = "voyages-api/v3.2/"
 
     def __init__(self, connection: Optional[Connection] = None):
         """Initializes VoyagesAPI.
 
         Args:
             connection: API connection configuration. If not provided, the
                 default connection method is used.
@@ -73,18 +73,18 @@
         hide_event_details: Optional[bool] = None,
         hide_events: Optional[bool] = None,
         hide_market_info: Optional[bool] = None,
         nested: Optional[bool] = True,
         condensed: Optional[bool] = False,
         incremental: Optional[bool] = False,
     ) -> str:
-        """Constructs the VoyagesData V3 endpoint.
+        """Constructs the VoyagesData v3.2 endpoint.
 
         Args:
-            endpoint_params: VoyagesData V3 endpoint parameters dictionary.
+            endpoint_params: VoyagesData v3.2 endpoint parameters dictionary.
             Part of get_voyages method arguments.
             Part of get_voyages_incremental arguments.
 
         Returns:
             The constructed endpoint to call to retrieve the requested \
             voyages for the provided arguments.
         """
@@ -828,15 +828,15 @@
             event_type=event_type,
             event_horizons=event_horizons,
             event_purpose=event_purposes,
             vessel_class_id=vessel_class_ids,
             port_ids=port_ids,
             vessel_type_id=vessel_type_id,
             voyage_date_from=start_date_from,
-            voyage_date_to=start_date_from,
+            voyage_date_to=start_date_to,
             start_date_from=start_date_from,
             start_date_to=start_date_to,
             first_load_arrival_date_from=first_load_arrival_date_from,
             first_load_arrival_date_to=first_load_arrival_date_to,
             end_date_from=end_date_from,
             end_date_to=end_date_to,
             market_info_rate_from=market_info_rate_from,
@@ -1017,15 +1017,15 @@
             class_filter: A filter used to find specific vessel classes. If
                 not specified, returns all available vessel classes.
 
         Returns:
             A tuple of available vessel classes that match the filter.
         """
         response = self.__connection._make_get_request(
-            "voyages-api/v3/filters/availableVesselClasses"
+            "voyages-api/v3.2/filters/availableVesselClasses"
         )
         response.raise_for_status()
 
         classes = (parse_model(c, VesselClass) for c in response.json())
         class_filter = class_filter or VesselClassFilter()
 
         return tuple(class_filter._apply(classes))
@@ -1039,15 +1039,15 @@
             type_filter: A filter used to find specific vessel types. If not
                 specified, returns all available vessel types.
 
         Returns:
             A tuple of available vessel types that match the filter.
         """
         response = self.__connection._make_get_request(
-            "voyages-api/v3/filters/availableVesselTypes"
+            "voyages-api/v3.2/filters/availableVesselTypes"
         )
         response.raise_for_status()
 
         types = (parse_model(c, VesselType) for c in response.json())
         type_filter = type_filter or VesselTypeFilter()
 
         return tuple(type_filter._apply(types))
@@ -1061,15 +1061,15 @@
             vessel_filter: A filter used to find specific vessel . If not
                 specified, returns all available vessels .
 
         Returns:
             A tuple of available vessels that match the filter.
         """
         response = self.__connection._make_get_request(
-            "voyages-api/v3/filters/availableVessels"
+            "voyages-api/v3.2/filters/availableVessels"
         )
         response.raise_for_status()
 
         vessels = (parse_model(c, Vessel) for c in response.json())
         vessel_filter = vessel_filter or VesselFilter()
 
         return tuple(vessel_filter._apply(vessels))
```

### Comparing `signal-ocean-7.1.1/signal_ocean/voyages_market_data/__init__.py` & `signal-ocean-7.1.2/signal_ocean/voyages_market_data/__init__.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/signal_ocean/voyages_market_data/models.py` & `signal-ocean-7.1.2/signal_ocean/voyages_market_data/models.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/signal_ocean/voyages_market_data/voyages_market_data_api.py` & `signal-ocean-7.1.2/signal_ocean/voyages_market_data/voyages_market_data_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.1/signal_ocean.egg-info/PKG-INFO` & `signal-ocean-7.1.2/signal_ocean.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: signal-ocean
-Version: 7.1.1
+Version: 7.1.2
 Summary: Access Signal Ocean Platform data using Python.
 Home-page: https://apis.signalocean.com/
 Author: Signal Ocean Developers
 Author-email: signaloceandevelopers@thesignalgroup.com
 License: Apache 2.0
 Project-URL: The Signal Group, https://www.thesignalgroup.com/
 Project-URL: Signal Ocean, https://www.signalocean.com/
```

### Comparing `signal-ocean-7.1.1/signal_ocean.egg-info/SOURCES.txt` & `signal-ocean-7.1.2/signal_ocean.egg-info/SOURCES.txt`

 * *Files identical despite different names*

