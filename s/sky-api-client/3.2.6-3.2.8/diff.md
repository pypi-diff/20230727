# Comparing `tmp/sky_api_client-3.2.6.tar.gz` & `tmp/sky_api_client-3.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sky_api_client-3.2.6.tar", last modified: Fri Apr 28 10:09:34 2023, max compression
+gzip compressed data, was "dist/sky_api_client-3.2.8.tar", last modified: Thu Jul 27 11:10:28 2023, max compression
```

## Comparing `sky_api_client-3.2.6.tar` & `sky_api_client-3.2.8.tar`

### file list

```diff
@@ -1,63 +1,64 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 10:09:34.000000 sky_api_client-3.2.6/
--rw-r--r--   0 root         (0) root         (0)     4142 2023-04-28 10:09:34.000000 sky_api_client-3.2.6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2418 2023-04-28 10:09:17.000000 sky_api_client-3.2.6/README.md
--rw-rw-rw-   0 root         (0) root         (0)      475 2023-04-28 10:09:17.000000 sky_api_client-3.2.6/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-28 10:09:34.000000 sky_api_client-3.2.6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      668 2023-04-28 10:09:17.000000 sky_api_client-3.2.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 10:09:34.000000 sky_api_client-3.2.6/sky_api_client/
--rw-rw-rw-   0 root         (0) root         (0)     2691 2023-04-28 10:09:17.000000 sky_api_client-3.2.6/sky_api_client/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1946 2023-04-28 10:09:17.000000 sky_api_client-3.2.6/sky_api_client/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 10:09:34.000000 sky_api_client-3.2.6/sky_api_client/entity/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-28 10:09:17.000000 sky_api_client-3.2.6/sky_api_client/entity/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      461 2023-04-28 10:09:17.000000 sky_api_client-3.2.6/sky_api_client/entity/address.py
--rw-rw-rw-   0 root         (0) root         (0)     2141 2023-04-28 10:09:17.000000 sky_api_client-3.2.6/sky_api_client/entity/base.py
--rw-rw-rw-   0 root         (0) root         (0)      475 2023-04-28 10:09:17.000000 sky_api_client-3.2.6/sky_api_client/entity/code_table.py
--rw-rw-rw-   0 root         (0) root         (0)      506 2023-04-28 10:09:17.000000 sky_api_client-3.2.6/sky_api_client/entity/constituent.py
--rw-rw-rw-   0 root         (0) root         (0)      272 2023-04-28 10:09:17.000000 sky_api_client-3.2.6/sky_api_client/entity/constituent_address.py
--rw-rw-rw-   0 root         (0) root         (0)      539 2023-04-28 10:09:17.000000 sky_api_client-3.2.6/sky_api_client/entity/constituent_code.py
--rw-rw-rw-   0 root         (0) root         (0)      261 2023-04-28 10:09:17.000000 sky_api_client-3.2.6/sky_api_client/entity/constituent_custom_field.py
--rw-rw-rw-   0 root         (0) root         (0)      254 2023-04-28 10:09:17.000000 sky_api_client-3.2.6/sky_api_client/entity/constituent_education.py
--rw-rw-rw-   0 root         (0) root         (0)      288 2023-04-28 10:09:17.000000 sky_api_client-3.2.6/sky_api_client/entity/constituent_email_address.py
--rw-rw-rw-   0 root         (0) root         (0)      293 2023-04-28 10:09:17.000000 sky_api_client-3.2.6/sky_api_client/entity/constituent_online_presence.py
--rw-rw-rw-   0 root         (0) root         (0)      265 2023-04-28 10:09:17.000000 sky_api_client-3.2.6/sky_api_client/entity/constituent_phone.py
--rw-rw-rw-   0 root         (0) root         (0)      263 2023-04-28 10:09:17.000000 sky_api_client-3.2.6/sky_api_client/entity/constituent_relationship.py
--rw-rw-rw-   0 root         (0) root         (0)      269 2023-04-28 10:09:17.000000 sky_api_client-3.2.6/sky_api_client/entity/constituent_solicit_code.py
--rw-rw-rw-   0 root         (0) root         (0)      430 2023-04-28 10:09:17.000000 sky_api_client-3.2.6/sky_api_client/entity/custom_field.py
--rw-rw-rw-   0 root         (0) root         (0)      270 2023-04-28 10:09:17.000000 sky_api_client-3.2.6/sky_api_client/entity/custom_field_categories.py
--rw-rw-rw-   0 root         (0) root         (0)      977 2023-04-28 10:09:17.000000 sky_api_client-3.2.6/sky_api_client/entity/education.py
--rw-rw-rw-   0 root         (0) root         (0)      439 2023-04-28 10:09:17.000000 sky_api_client-3.2.6/sky_api_client/entity/email_addresses.py
--rw-rw-rw-   0 root         (0) root         (0)      354 2023-04-28 10:09:17.000000 sky_api_client-3.2.6/sky_api_client/entity/event.py
--rw-rw-rw-   0 root         (0) root         (0)      356 2023-04-28 10:09:17.000000 sky_api_client-3.2.6/sky_api_client/entity/event_fee.py
--rw-rw-rw-   0 root         (0) root         (0)      428 2023-04-28 10:09:17.000000 sky_api_client-3.2.6/sky_api_client/entity/event_participant.py
--rw-rw-rw-   0 root         (0) root         (0)      370 2023-04-28 10:09:17.000000 sky_api_client-3.2.6/sky_api_client/entity/event_participant_donation.py
--rw-rw-rw-   0 root         (0) root         (0)      343 2023-04-28 10:09:17.000000 sky_api_client-3.2.6/sky_api_client/entity/event_participant_fee.py
--rw-rw-rw-   0 root         (0) root         (0)      379 2023-04-28 10:09:17.000000 sky_api_client-3.2.6/sky_api_client/entity/event_participant_fee_payment.py
--rw-rw-rw-   0 root         (0) root         (0)      401 2023-04-28 10:09:17.000000 sky_api_client-3.2.6/sky_api_client/entity/event_participant_levels.py
--rw-rw-rw-   0 root         (0) root         (0)      244 2023-04-28 10:09:17.000000 sky_api_client-3.2.6/sky_api_client/entity/event_participation_levels.py
--rw-rw-rw-   0 root         (0) root         (0)      273 2023-04-28 10:09:17.000000 sky_api_client-3.2.6/sky_api_client/entity/fundraising_appeal.py
--rw-rw-rw-   0 root         (0) root         (0)      281 2023-04-28 10:09:17.000000 sky_api_client-3.2.6/sky_api_client/entity/fundraising_campaign.py
--rw-rw-rw-   0 root         (0) root         (0)      265 2023-04-28 10:09:17.000000 sky_api_client-3.2.6/sky_api_client/entity/fundraising_fund.py
--rw-rw-rw-   0 root         (0) root         (0)      277 2023-04-28 10:09:17.000000 sky_api_client-3.2.6/sky_api_client/entity/fundraising_package.py
--rw-rw-rw-   0 root         (0) root         (0)      205 2023-04-28 10:09:17.000000 sky_api_client-3.2.6/sky_api_client/entity/gender.py
--rw-rw-rw-   0 root         (0) root         (0)      341 2023-04-28 10:09:17.000000 sky_api_client-3.2.6/sky_api_client/entity/gift.py
--rw-rw-rw-   0 root         (0) root         (0)      311 2023-04-28 10:09:17.000000 sky_api_client-3.2.6/sky_api_client/entity/gift_batch.py
--rw-rw-rw-   0 root         (0) root         (0)      230 2023-04-28 10:09:17.000000 sky_api_client-3.2.6/sky_api_client/entity/gift_batch_gift.py
--rw-rw-rw-   0 root         (0) root         (0)      213 2023-04-28 10:09:17.000000 sky_api_client-3.2.6/sky_api_client/entity/gift_subtype.py
--rw-rw-rw-   0 root         (0) root         (0)      191 2023-04-28 10:09:17.000000 sky_api_client-3.2.6/sky_api_client/entity/list.py
--rw-rw-rw-   0 root         (0) root         (0)      535 2023-04-28 10:09:17.000000 sky_api_client-3.2.6/sky_api_client/entity/online_presence.py
--rw-rw-rw-   0 root         (0) root         (0)      440 2023-04-28 10:09:17.000000 sky_api_client-3.2.6/sky_api_client/entity/phone.py
--rw-rw-rw-   0 root         (0) root         (0)      494 2023-04-28 10:09:17.000000 sky_api_client-3.2.6/sky_api_client/entity/registry.py
--rw-rw-rw-   0 root         (0) root         (0)      445 2023-04-28 10:09:17.000000 sky_api_client-3.2.6/sky_api_client/entity/relationship.py
--rw-rw-rw-   0 root         (0) root         (0)      765 2023-04-28 10:09:17.000000 sky_api_client-3.2.6/sky_api_client/entity/solicit_code.py
--rw-rw-rw-   0 root         (0) root         (0)      205 2023-04-28 10:09:17.000000 sky_api_client-3.2.6/sky_api_client/entity/suffix.py
--rw-rw-rw-   0 root         (0) root         (0)      587 2023-04-28 10:09:17.000000 sky_api_client-3.2.6/sky_api_client/entity/table_entry.py
--rw-rw-rw-   0 root         (0) root         (0)      201 2023-04-28 10:09:17.000000 sky_api_client-3.2.6/sky_api_client/entity/title.py
--rw-rw-rw-   0 root         (0) root         (0)      379 2023-04-28 10:09:17.000000 sky_api_client-3.2.6/sky_api_client/entity/webhook_subscription.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 10:09:34.000000 sky_api_client-3.2.6/sky_api_client/exceptions/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-28 10:09:17.000000 sky_api_client-3.2.6/sky_api_client/exceptions/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      357 2023-04-28 10:09:17.000000 sky_api_client-3.2.6/sky_api_client/exceptions/exception.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 10:09:34.000000 sky_api_client-3.2.6/sky_api_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4142 2023-04-28 10:09:34.000000 sky_api_client-3.2.6/sky_api_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2155 2023-04-28 10:09:34.000000 sky_api_client-3.2.6/sky_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 10:09:34.000000 sky_api_client-3.2.6/sky_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-04-28 10:09:34.000000 sky_api_client-3.2.6/sky_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 11:10:28.000000 sky_api_client-3.2.8/
+-rw-r--r--   0 root         (0) root         (0)     4142 2023-07-27 11:10:28.000000 sky_api_client-3.2.8/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2418 2023-07-27 11:10:08.000000 sky_api_client-3.2.8/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      475 2023-07-27 11:10:08.000000 sky_api_client-3.2.8/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-27 11:10:28.000000 sky_api_client-3.2.8/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      668 2023-07-27 11:10:08.000000 sky_api_client-3.2.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 11:10:28.000000 sky_api_client-3.2.8/sky_api_client/
+-rw-rw-rw-   0 root         (0) root         (0)     2748 2023-07-27 11:10:08.000000 sky_api_client-3.2.8/sky_api_client/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1946 2023-07-27 11:10:08.000000 sky_api_client-3.2.8/sky_api_client/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 11:10:28.000000 sky_api_client-3.2.8/sky_api_client/entity/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-27 11:10:08.000000 sky_api_client-3.2.8/sky_api_client/entity/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      461 2023-07-27 11:10:08.000000 sky_api_client-3.2.8/sky_api_client/entity/address.py
+-rw-rw-rw-   0 root         (0) root         (0)     2141 2023-07-27 11:10:08.000000 sky_api_client-3.2.8/sky_api_client/entity/base.py
+-rw-rw-rw-   0 root         (0) root         (0)      475 2023-07-27 11:10:08.000000 sky_api_client-3.2.8/sky_api_client/entity/code_table.py
+-rw-rw-rw-   0 root         (0) root         (0)      506 2023-07-27 11:10:08.000000 sky_api_client-3.2.8/sky_api_client/entity/constituent.py
+-rw-rw-rw-   0 root         (0) root         (0)      272 2023-07-27 11:10:08.000000 sky_api_client-3.2.8/sky_api_client/entity/constituent_address.py
+-rw-rw-rw-   0 root         (0) root         (0)      539 2023-07-27 11:10:08.000000 sky_api_client-3.2.8/sky_api_client/entity/constituent_code.py
+-rw-rw-rw-   0 root         (0) root         (0)      261 2023-07-27 11:10:08.000000 sky_api_client-3.2.8/sky_api_client/entity/constituent_custom_field.py
+-rw-rw-rw-   0 root         (0) root         (0)      254 2023-07-27 11:10:08.000000 sky_api_client-3.2.8/sky_api_client/entity/constituent_education.py
+-rw-rw-rw-   0 root         (0) root         (0)      288 2023-07-27 11:10:08.000000 sky_api_client-3.2.8/sky_api_client/entity/constituent_email_address.py
+-rw-rw-rw-   0 root         (0) root         (0)      293 2023-07-27 11:10:08.000000 sky_api_client-3.2.8/sky_api_client/entity/constituent_online_presence.py
+-rw-rw-rw-   0 root         (0) root         (0)      265 2023-07-27 11:10:08.000000 sky_api_client-3.2.8/sky_api_client/entity/constituent_phone.py
+-rw-rw-rw-   0 root         (0) root         (0)      263 2023-07-27 11:10:08.000000 sky_api_client-3.2.8/sky_api_client/entity/constituent_relationship.py
+-rw-rw-rw-   0 root         (0) root         (0)      269 2023-07-27 11:10:08.000000 sky_api_client-3.2.8/sky_api_client/entity/constituent_solicit_code.py
+-rw-rw-rw-   0 root         (0) root         (0)      430 2023-07-27 11:10:08.000000 sky_api_client-3.2.8/sky_api_client/entity/custom_field.py
+-rw-rw-rw-   0 root         (0) root         (0)      270 2023-07-27 11:10:08.000000 sky_api_client-3.2.8/sky_api_client/entity/custom_field_categories.py
+-rw-rw-rw-   0 root         (0) root         (0)      977 2023-07-27 11:10:08.000000 sky_api_client-3.2.8/sky_api_client/entity/education.py
+-rw-rw-rw-   0 root         (0) root         (0)      439 2023-07-27 11:10:08.000000 sky_api_client-3.2.8/sky_api_client/entity/email_addresses.py
+-rw-rw-rw-   0 root         (0) root         (0)      354 2023-07-27 11:10:08.000000 sky_api_client-3.2.8/sky_api_client/entity/event.py
+-rw-rw-rw-   0 root         (0) root         (0)      356 2023-07-27 11:10:08.000000 sky_api_client-3.2.8/sky_api_client/entity/event_fee.py
+-rw-rw-rw-   0 root         (0) root         (0)      428 2023-07-27 11:10:08.000000 sky_api_client-3.2.8/sky_api_client/entity/event_participant.py
+-rw-rw-rw-   0 root         (0) root         (0)      370 2023-07-27 11:10:08.000000 sky_api_client-3.2.8/sky_api_client/entity/event_participant_donation.py
+-rw-rw-rw-   0 root         (0) root         (0)      343 2023-07-27 11:10:08.000000 sky_api_client-3.2.8/sky_api_client/entity/event_participant_fee.py
+-rw-rw-rw-   0 root         (0) root         (0)      379 2023-07-27 11:10:08.000000 sky_api_client-3.2.8/sky_api_client/entity/event_participant_fee_payment.py
+-rw-rw-rw-   0 root         (0) root         (0)      401 2023-07-27 11:10:08.000000 sky_api_client-3.2.8/sky_api_client/entity/event_participant_levels.py
+-rw-rw-rw-   0 root         (0) root         (0)      244 2023-07-27 11:10:08.000000 sky_api_client-3.2.8/sky_api_client/entity/event_participation_levels.py
+-rw-rw-rw-   0 root         (0) root         (0)      273 2023-07-27 11:10:08.000000 sky_api_client-3.2.8/sky_api_client/entity/fundraising_appeal.py
+-rw-rw-rw-   0 root         (0) root         (0)      281 2023-07-27 11:10:08.000000 sky_api_client-3.2.8/sky_api_client/entity/fundraising_campaign.py
+-rw-rw-rw-   0 root         (0) root         (0)      265 2023-07-27 11:10:08.000000 sky_api_client-3.2.8/sky_api_client/entity/fundraising_fund.py
+-rw-rw-rw-   0 root         (0) root         (0)      277 2023-07-27 11:10:08.000000 sky_api_client-3.2.8/sky_api_client/entity/fundraising_package.py
+-rw-rw-rw-   0 root         (0) root         (0)      205 2023-07-27 11:10:08.000000 sky_api_client-3.2.8/sky_api_client/entity/gender.py
+-rw-rw-rw-   0 root         (0) root         (0)      341 2023-07-27 11:10:08.000000 sky_api_client-3.2.8/sky_api_client/entity/gift.py
+-rw-rw-rw-   0 root         (0) root         (0)      397 2023-07-27 11:10:08.000000 sky_api_client-3.2.8/sky_api_client/entity/gift_aid.py
+-rw-rw-rw-   0 root         (0) root         (0)      311 2023-07-27 11:10:08.000000 sky_api_client-3.2.8/sky_api_client/entity/gift_batch.py
+-rw-rw-rw-   0 root         (0) root         (0)      230 2023-07-27 11:10:08.000000 sky_api_client-3.2.8/sky_api_client/entity/gift_batch_gift.py
+-rw-rw-rw-   0 root         (0) root         (0)      213 2023-07-27 11:10:08.000000 sky_api_client-3.2.8/sky_api_client/entity/gift_subtype.py
+-rw-rw-rw-   0 root         (0) root         (0)      191 2023-07-27 11:10:08.000000 sky_api_client-3.2.8/sky_api_client/entity/list.py
+-rw-rw-rw-   0 root         (0) root         (0)      535 2023-07-27 11:10:08.000000 sky_api_client-3.2.8/sky_api_client/entity/online_presence.py
+-rw-rw-rw-   0 root         (0) root         (0)      440 2023-07-27 11:10:08.000000 sky_api_client-3.2.8/sky_api_client/entity/phone.py
+-rw-rw-rw-   0 root         (0) root         (0)      494 2023-07-27 11:10:08.000000 sky_api_client-3.2.8/sky_api_client/entity/registry.py
+-rw-rw-rw-   0 root         (0) root         (0)      445 2023-07-27 11:10:08.000000 sky_api_client-3.2.8/sky_api_client/entity/relationship.py
+-rw-rw-rw-   0 root         (0) root         (0)      765 2023-07-27 11:10:08.000000 sky_api_client-3.2.8/sky_api_client/entity/solicit_code.py
+-rw-rw-rw-   0 root         (0) root         (0)      205 2023-07-27 11:10:08.000000 sky_api_client-3.2.8/sky_api_client/entity/suffix.py
+-rw-rw-rw-   0 root         (0) root         (0)      587 2023-07-27 11:10:08.000000 sky_api_client-3.2.8/sky_api_client/entity/table_entry.py
+-rw-rw-rw-   0 root         (0) root         (0)      201 2023-07-27 11:10:08.000000 sky_api_client-3.2.8/sky_api_client/entity/title.py
+-rw-rw-rw-   0 root         (0) root         (0)      379 2023-07-27 11:10:08.000000 sky_api_client-3.2.8/sky_api_client/entity/webhook_subscription.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 11:10:28.000000 sky_api_client-3.2.8/sky_api_client/exceptions/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-27 11:10:08.000000 sky_api_client-3.2.8/sky_api_client/exceptions/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      357 2023-07-27 11:10:08.000000 sky_api_client-3.2.8/sky_api_client/exceptions/exception.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 11:10:28.000000 sky_api_client-3.2.8/sky_api_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4142 2023-07-27 11:10:28.000000 sky_api_client-3.2.8/sky_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2189 2023-07-27 11:10:28.000000 sky_api_client-3.2.8/sky_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 11:10:28.000000 sky_api_client-3.2.8/sky_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-07-27 11:10:28.000000 sky_api_client-3.2.8/sky_api_client.egg-info/top_level.txt
```

### Comparing `sky_api_client-3.2.6/PKG-INFO` & `sky_api_client-3.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sky_api_client
-Version: 3.2.6
+Version: 3.2.8
 Summary: Python client for RENXT APIs
 Home-page: https://bitbucket.org/kalyanvarma/skyapi
 Author: Uddesh Jain
 Author-email: uddesh@almabase.com
 License: UNKNOWN
 Description: # Sky Api Client
```

### Comparing `sky_api_client-3.2.6/README.md` & `sky_api_client-3.2.8/README.md`

 * *Files identical despite different names*

### Comparing `sky_api_client-3.2.6/setup.py` & `sky_api_client-3.2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='sky_api_client',
-    version='3.2.6',
+    version='3.2.8',
     author='Uddesh Jain',
     author_email='uddesh@almabase.com',
     description='Python client for RENXT APIs',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://bitbucket.org/kalyanvarma/skyapi',
     classifiers=[
```

### Comparing `sky_api_client-3.2.6/sky_api_client/__init__.py` & `sky_api_client-3.2.8/sky_api_client/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,7 +36,8 @@
 from sky_api_client.entity import fundraising_appeal  # noqa: F401
 from sky_api_client.entity import fundraising_fund  # noqa: F401
 from sky_api_client.entity import fundraising_campaign  # noqa: F401
 from sky_api_client.entity import fundraising_package  # noqa: F401
 from sky_api_client.entity import constituent_solicit_code  # noqa: F401
 from sky_api_client.entity import solicit_code  # noqa: F401
 from sky_api_client.entity import list  # noqa: F401
+from sky_api_client.entity import gift_aid  # noqa: F401
```

### Comparing `sky_api_client-3.2.6/sky_api_client/client.py` & `sky_api_client-3.2.8/sky_api_client/client.py`

 * *Files identical despite different names*

### Comparing `sky_api_client-3.2.6/sky_api_client/entity/base.py` & `sky_api_client-3.2.8/sky_api_client/entity/base.py`

 * *Files identical despite different names*

### Comparing `sky_api_client-3.2.6/sky_api_client/entity/constituent_code.py` & `sky_api_client-3.2.8/sky_api_client/entity/constituent_code.py`

 * *Files identical despite different names*

### Comparing `sky_api_client-3.2.6/sky_api_client/entity/education.py` & `sky_api_client-3.2.8/sky_api_client/entity/education.py`

 * *Files identical despite different names*

### Comparing `sky_api_client-3.2.6/sky_api_client/entity/online_presence.py` & `sky_api_client-3.2.8/sky_api_client/entity/online_presence.py`

 * *Files identical despite different names*

### Comparing `sky_api_client-3.2.6/sky_api_client/entity/solicit_code.py` & `sky_api_client-3.2.8/sky_api_client/entity/solicit_code.py`

 * *Files identical despite different names*

### Comparing `sky_api_client-3.2.6/sky_api_client/entity/table_entry.py` & `sky_api_client-3.2.8/sky_api_client/entity/table_entry.py`

 * *Files identical despite different names*

### Comparing `sky_api_client-3.2.6/sky_api_client.egg-info/PKG-INFO` & `sky_api_client-3.2.8/sky_api_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sky-api-client
-Version: 3.2.6
+Version: 3.2.8
 Summary: Python client for RENXT APIs
 Home-page: https://bitbucket.org/kalyanvarma/skyapi
 Author: Uddesh Jain
 Author-email: uddesh@almabase.com
 License: UNKNOWN
 Description: # Sky Api Client
```

### Comparing `sky_api_client-3.2.6/sky_api_client.egg-info/SOURCES.txt` & `sky_api_client-3.2.8/sky_api_client.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 sky_api_client/entity/event_participation_levels.py
 sky_api_client/entity/fundraising_appeal.py
 sky_api_client/entity/fundraising_campaign.py
 sky_api_client/entity/fundraising_fund.py
 sky_api_client/entity/fundraising_package.py
 sky_api_client/entity/gender.py
 sky_api_client/entity/gift.py
+sky_api_client/entity/gift_aid.py
 sky_api_client/entity/gift_batch.py
 sky_api_client/entity/gift_batch_gift.py
 sky_api_client/entity/gift_subtype.py
 sky_api_client/entity/list.py
 sky_api_client/entity/online_presence.py
 sky_api_client/entity/phone.py
 sky_api_client/entity/registry.py
```

