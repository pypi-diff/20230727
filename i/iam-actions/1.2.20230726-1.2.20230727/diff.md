# Comparing `tmp/iam_actions-1.2.20230726.tar.gz` & `tmp/iam_actions-1.2.20230727.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20230726.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20230727.tar", max compression
```

## Comparing `iam_actions-1.2.20230726.tar` & `iam_actions-1.2.20230727.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2023-07-26 02:31:33.489491 iam_actions-1.2.20230726/LICENSE
--rw-r--r--   0        0        0     2302 2023-07-26 02:31:33.489491 iam_actions-1.2.20230726/README.md
--rw-r--r--   0        0        0      228 2023-07-26 02:31:33.489491 iam_actions-1.2.20230726/iam_actions/__init__.py
--rw-r--r--   0        0        0  4377792 2023-07-26 02:33:43.655265 iam_actions-1.2.20230726/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2023-07-26 02:31:33.489491 iam_actions-1.2.20230726/iam_actions/data.py
--rw-r--r--   0        0        0       80 2023-07-26 02:31:33.489491 iam_actions-1.2.20230726/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2023-07-26 02:31:33.489491 iam_actions-1.2.20230726/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2023-07-26 02:31:33.489491 iam_actions-1.2.20230726/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2023-07-26 02:31:33.489491 iam_actions-1.2.20230726/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2023-07-26 02:31:33.493491 iam_actions-1.2.20230726/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2023-07-26 02:31:33.493491 iam_actions-1.2.20230726/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2023-07-26 02:31:33.493491 iam_actions-1.2.20230726/iam_actions/generate/services.py
--rw-r--r--   0        0        0   563521 2023-07-26 02:33:43.655265 iam_actions-1.2.20230726/iam_actions/policies.json
--rw-r--r--   0        0        0   197464 2023-07-26 02:33:43.655265 iam_actions-1.2.20230726/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   546555 2023-07-26 02:33:43.655265 iam_actions-1.2.20230726/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2023-07-26 02:33:44.615337 iam_actions-1.2.20230726/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230726/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230726/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-27 02:20:15.740091 iam_actions-1.2.20230727/LICENSE
+-rw-r--r--   0        0        0     2302 2023-07-27 02:20:15.740091 iam_actions-1.2.20230727/README.md
+-rw-r--r--   0        0        0      228 2023-07-27 02:20:15.740091 iam_actions-1.2.20230727/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4380413 2023-07-27 02:22:49.225016 iam_actions-1.2.20230727/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2023-07-27 02:20:15.740091 iam_actions-1.2.20230727/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2023-07-27 02:20:15.740091 iam_actions-1.2.20230727/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2023-07-27 02:20:15.740091 iam_actions-1.2.20230727/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2023-07-27 02:20:15.744091 iam_actions-1.2.20230727/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2023-07-27 02:20:15.744091 iam_actions-1.2.20230727/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2023-07-27 02:20:15.744091 iam_actions-1.2.20230727/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2023-07-27 02:20:15.744091 iam_actions-1.2.20230727/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2023-07-27 02:20:15.744091 iam_actions-1.2.20230727/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   565102 2023-07-27 02:22:49.225016 iam_actions-1.2.20230727/iam_actions/policies.json
+-rw-r--r--   0        0        0   196251 2023-07-27 02:22:49.225016 iam_actions-1.2.20230727/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   548166 2023-07-27 02:22:49.225016 iam_actions-1.2.20230727/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2023-07-27 02:22:50.341023 iam_actions-1.2.20230727/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230727/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230727/PKG-INFO
```

### Comparing `iam_actions-1.2.20230726/LICENSE` & `iam_actions-1.2.20230727/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230726/README.md` & `iam_actions-1.2.20230727/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230726/iam_actions/actions.json` & `iam_actions-1.2.20230727/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9939375601940711%*

 * *Differences: {"'ce'": "{'GetSavingsPlanPurchaseRecommendationDetails': OrderedDict([('access_level', "*

 * *         "'Undocumented'), ('action', 'GetSavingsPlanPurchaseRecommendationDetails'), "*

 * *         "('condition_keys', []), ('description', 'Not Documented by AWS'), ('orphan', False), "*

 * *         "('resources', [])])}",*

 * * "'entityresolution'": "OrderedDict([('ListSchemaMappings', OrderedDict([('access_level', "*

 * *                       "'Undocumented'), ('action', 'ListSchemaMappings'), ('condition_keys', []), "*

 * *            […]*

```diff
@@ -14408,14 +14408,22 @@
             "access_level": "Read",
             "action": "GetRightsizingRecommendation",
             "condition_keys": [],
             "description": "Grants permission to retrieve the rightsizing recommendations for your account",
             "orphan": false,
             "resources": []
         },
+        "GetSavingsPlanPurchaseRecommendationDetails": {
+            "access_level": "Undocumented",
+            "action": "GetSavingsPlanPurchaseRecommendationDetails",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "GetSavingsPlansCoverage": {
             "access_level": "Read",
             "action": "GetSavingsPlansCoverage",
             "condition_keys": [],
             "description": "Grants permission to retrieve the Savings Plans coverage for your account",
             "orphan": false,
             "resources": []
@@ -59196,14 +59204,144 @@
             "description": "Grants permission to Update an application",
             "orphan": false,
             "resources": [
                 "application"
             ]
         }
     },
+    "entityresolution": {
+        "CreateMatchingWorkflow": {
+            "access_level": "Undocumented",
+            "action": "CreateMatchingWorkflow",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "CreateSchemaMapping": {
+            "access_level": "Undocumented",
+            "action": "CreateSchemaMapping",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "DeleteMatchingWorkflow": {
+            "access_level": "Undocumented",
+            "action": "DeleteMatchingWorkflow",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "DeleteSchemaMapping": {
+            "access_level": "Undocumented",
+            "action": "DeleteSchemaMapping",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetMatchId": {
+            "access_level": "Undocumented",
+            "action": "GetMatchId",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetMatchingJob": {
+            "access_level": "Undocumented",
+            "action": "GetMatchingJob",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetMatchingWorkflow": {
+            "access_level": "Undocumented",
+            "action": "GetMatchingWorkflow",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetSchemaMapping": {
+            "access_level": "Undocumented",
+            "action": "GetSchemaMapping",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListMatchingJobs": {
+            "access_level": "Undocumented",
+            "action": "ListMatchingJobs",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListMatchingWorkflows": {
+            "access_level": "Undocumented",
+            "action": "ListMatchingWorkflows",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListSchemaMappings": {
+            "access_level": "Undocumented",
+            "action": "ListSchemaMappings",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListTagsForResource": {
+            "access_level": "Undocumented",
+            "action": "ListTagsForResource",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "StartMatchingJob": {
+            "access_level": "Undocumented",
+            "action": "StartMatchingJob",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "TagResource": {
+            "access_level": "Undocumented",
+            "action": "TagResource",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "UntagResource": {
+            "access_level": "Undocumented",
+            "action": "UntagResource",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "UpdateMatchingWorkflow": {
+            "access_level": "Undocumented",
+            "action": "UpdateMatchingWorkflow",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        }
+    },
     "es": {
         "AcceptInboundConnection": {
             "access_level": "Write",
             "action": "AcceptInboundConnection",
             "condition_keys": [],
             "description": "Grants permission to the destination domain owner to accept an inbound cross-cluster search connection request",
             "orphan": false,
@@ -72150,217 +72288,172 @@
             "description": "Grants permission to enable the Organizational View feature",
             "orphan": false,
             "resources": []
         }
     },
     "healthlake": {
         "CreateFHIRDatastore": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateFHIRDatastore",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:TagKeys"
-            ],
-            "description": "Grants permission to create a datastore that can ingest and export FHIR data",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "CreateResource": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateResource",
             "condition_keys": [],
-            "description": "Grants permission to create resource",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "datastore"
-            ]
+            "resources": []
         },
         "DeleteFHIRDatastore": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteFHIRDatastore",
             "condition_keys": [],
-            "description": "Grants permission to delete a datastore",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "datastore"
-            ]
+            "resources": []
         },
         "DeleteResource": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteResource",
             "condition_keys": [],
-            "description": "Grants permission to delete resource",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "datastore"
-            ]
+            "resources": []
         },
         "DescribeFHIRDatastore": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "DescribeFHIRDatastore",
             "condition_keys": [],
-            "description": "Grants permission to get the properties associated with the FHIR datastore, including the datastore ID, datastore ARN, datastore name, datastore status, created at, datastore type version, and datastore endpoint",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "datastore"
-            ]
+            "resources": []
         },
         "DescribeFHIRExportJob": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "DescribeFHIRExportJob",
             "condition_keys": [],
-            "description": "Grants permission to display the properties of a FHIR export job, including the ID, ARN, name, and the status of the datastore",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "datastore"
-            ]
+            "resources": []
         },
         "DescribeFHIRImportJob": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "DescribeFHIRImportJob",
             "condition_keys": [],
-            "description": "Grants permission to display the properties of a FHIR import job, including the ID, ARN, name, and the status of the datastore",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "datastore"
-            ]
+            "resources": []
         },
         "GetCapabilities": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "GetCapabilities",
             "condition_keys": [],
-            "description": "Grants permission to get the capabilities of a FHIR datastore",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "datastore"
-            ]
+            "resources": []
         },
         "ListFHIRDatastores": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "ListFHIRDatastores",
             "condition_keys": [],
-            "description": "Grants permission to list all FHIR datastores that are in the user\u2019s account, regardless of datastore status",
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListFHIRExportJobs": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "ListFHIRExportJobs",
             "condition_keys": [],
-            "description": "Grants permission to get a list of export jobs for the specified datastore",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "datastore"
-            ]
+            "resources": []
         },
         "ListFHIRImportJobs": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "ListFHIRImportJobs",
             "condition_keys": [],
-            "description": "Grants permission to get a list of import jobs for the specified datastore",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "datastore"
-            ]
+            "resources": []
         },
         "ListTagsForResource": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "ListTagsForResource",
             "condition_keys": [],
-            "description": "Grants permission to get a list of tags for the specified datastore",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "datastore"
-            ]
+            "resources": []
         },
         "ReadResource": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "ReadResource",
             "condition_keys": [],
-            "description": "Grants permission to read resource",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "datastore"
-            ]
+            "resources": []
         },
         "SearchWithGet": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "SearchWithGet",
             "condition_keys": [],
-            "description": "Grants permission to search resources with GET method",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "datastore"
-            ]
+            "resources": []
         },
         "SearchWithPost": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "SearchWithPost",
             "condition_keys": [],
-            "description": "Grants permission to search resources with POST method",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "datastore"
-            ]
+            "resources": []
         },
         "StartFHIRExportJob": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "StartFHIRExportJob",
             "condition_keys": [],
-            "description": "Grants permission to begin a FHIR Export job",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "datastore"
-            ]
+            "resources": []
         },
         "StartFHIRImportJob": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "StartFHIRImportJob",
             "condition_keys": [],
-            "description": "Grants permission to begin a FHIR Import job",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "datastore"
-            ]
+            "resources": []
         },
         "TagResource": {
-            "access_level": "Tagging",
+            "access_level": "Undocumented",
             "action": "TagResource",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:ResourceTag/${TagKey}",
-                "aws:TagKeys"
-            ],
-            "description": "Grants permission to add tags to a datastore",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "datastore"
-            ]
+            "resources": []
         },
         "UntagResource": {
-            "access_level": "Tagging",
+            "access_level": "Undocumented",
             "action": "UntagResource",
-            "condition_keys": [
-                "aws:TagKeys"
-            ],
-            "description": "Grants permission to remove tags associated with a datastore",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "datastore"
-            ]
+            "resources": []
         },
         "UpdateResource": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "UpdateResource",
             "condition_keys": [],
-            "description": "Grants permission to update resource",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "datastore"
-            ]
+            "resources": []
         }
     },
     "honeycode": {
         "ApproveTeamAssociation": {
             "access_level": "Write",
             "action": "ApproveTeamAssociation",
             "condition_keys": [],
@@ -83351,14 +83444,22 @@
             "condition_keys": [],
             "description": "Grants permission to get multiple stream keys simultaneously by stream key ARN",
             "orphan": false,
             "resources": [
                 "Stream-Key"
             ]
         },
+        "BatchStartViewerSessionRevocation": {
+            "access_level": "Undocumented",
+            "action": "BatchStartViewerSessionRevocation",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "CreateChannel": {
             "access_level": "Write",
             "action": "CreateChannel",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
             ],
@@ -83709,14 +83810,22 @@
             "condition_keys": [],
             "description": "Grants permission to insert metadata into an RTMP stream for a specified channel",
             "orphan": false,
             "resources": [
                 "Channel"
             ]
         },
+        "StartViewerSessionRevocation": {
+            "access_level": "Undocumented",
+            "action": "StartViewerSessionRevocation",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "StopStream": {
             "access_level": "Write",
             "action": "StopStream",
             "condition_keys": [],
             "description": "Grants permission to disconnect a streamer on a specified channel",
             "orphan": false,
             "resources": [
@@ -89427,14 +89536,38 @@
             "access_level": "List",
             "action": "ListImports",
             "condition_keys": [],
             "description": "Grants permission to list existing imports",
             "orphan": false,
             "resources": []
         },
+        "ListIntentMetrics": {
+            "access_level": "Undocumented",
+            "action": "ListIntentMetrics",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListIntentPaths": {
+            "access_level": "Undocumented",
+            "action": "ListIntentPaths",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListIntentStageMetrics": {
+            "access_level": "Undocumented",
+            "action": "ListIntentStageMetrics",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "ListIntents": {
             "access_level": "List",
             "action": "ListIntents",
             "condition_keys": [],
             "description": "Grants permission to list intents in a bot",
             "orphan": false,
             "resources": [
@@ -89447,14 +89580,30 @@
             "condition_keys": [],
             "description": "Grants permission to get a list of recommended intents provided by the bot recommendation",
             "orphan": false,
             "resources": [
                 "bot"
             ]
         },
+        "ListSessionAnalyticsData": {
+            "access_level": "Undocumented",
+            "action": "ListSessionAnalyticsData",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListSessionMetrics": {
+            "access_level": "Undocumented",
+            "action": "ListSessionMetrics",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "ListSlotTypes": {
             "access_level": "List",
             "action": "ListSlotTypes",
             "condition_keys": [],
             "description": "Grants permission to list slot types in a bot",
             "orphan": false,
             "resources": [
@@ -94920,14 +95069,30 @@
             "access_level": "Permissions management",
             "action": "Invoke",
             "condition_keys": [],
             "description": "Grants permission to create WebSocket connections to an Ethereum node",
             "orphan": false,
             "resources": []
         },
+        "InvokeRpcBitcoinMainnet": {
+            "access_level": "Undocumented",
+            "action": "InvokeRpcBitcoinMainnet",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "InvokeRpcBitcoinTestnet": {
+            "access_level": "Undocumented",
+            "action": "InvokeRpcBitcoinTestnet",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "ListAccessors": {
             "access_level": "List",
             "action": "ListAccessors",
             "condition_keys": [],
             "description": "Grants permission to list the Amazon Managed Blockchain accessors owned by the current AWS account",
             "orphan": false,
             "resources": []
@@ -95084,14 +95249,64 @@
             "description": "Grants permission to cast a vote for a proposal on behalf of the blockchain network member specified",
             "orphan": false,
             "resources": [
                 "proposal"
             ]
         }
     },
+    "managedblockchain-query": {
+        "BatchGetTokenBalance": {
+            "access_level": "Undocumented",
+            "action": "BatchGetTokenBalance",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetTokenBalance": {
+            "access_level": "Undocumented",
+            "action": "GetTokenBalance",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetTransaction": {
+            "access_level": "Undocumented",
+            "action": "GetTransaction",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListTokenBalances": {
+            "access_level": "Undocumented",
+            "action": "ListTokenBalances",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListTransactionEvents": {
+            "access_level": "Undocumented",
+            "action": "ListTransactionEvents",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListTransactions": {
+            "access_level": "Undocumented",
+            "action": "ListTransactions",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        }
+    },
     "marketplacecommerceanalytics": {
         "GenerateDataSet": {
             "access_level": "Write",
             "action": "GenerateDataSet",
             "condition_keys": [],
             "description": "Request a data set to be published to your Amazon S3 bucket.",
             "orphan": false,
@@ -105045,732 +105260,588 @@
             "resources": [
                 "Link"
             ]
         }
     },
     "omics": {
         "AbortMultipartReadSetUpload": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "AbortMultipartReadSetUpload",
             "condition_keys": [],
-            "description": "Grants permission to abort multipart read set uploads",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "sequenceStore"
-            ]
+            "resources": []
         },
         "BatchDeleteReadSet": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "BatchDeleteReadSet",
             "condition_keys": [],
-            "description": "Grants permission to batch delete Read Sets in the given Sequence Store",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "sequenceStore"
-            ]
+            "resources": []
         },
         "CancelAnnotationImportJob": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CancelAnnotationImportJob",
             "condition_keys": [],
-            "description": "Grants permission to cancel an Annotation Import Job",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "AnnotationImportJob"
-            ]
+            "resources": []
         },
         "CancelRun": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CancelRun",
             "condition_keys": [],
-            "description": "Grants permission to cancel a workflow run and stop all workflow tasks",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "run"
-            ]
+            "resources": []
         },
         "CancelVariantImportJob": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CancelVariantImportJob",
             "condition_keys": [],
-            "description": "Grants permission to cancel a Variant Import Job",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "VariantImportJob"
-            ]
+            "resources": []
         },
         "CompleteMultipartReadSetUpload": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CompleteMultipartReadSetUpload",
             "condition_keys": [],
-            "description": "Grants permission to complete a multipart read set upload",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "sequenceStore"
-            ]
+            "resources": []
         },
         "CreateAnnotationStore": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateAnnotationStore",
             "condition_keys": [],
-            "description": "Grants permission to create an Annotation Store",
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "CreateMultipartReadSetUpload": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateMultipartReadSetUpload",
             "condition_keys": [],
-            "description": "Grants permission to create a multipart read set upload",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "sequenceStore"
-            ]
+            "resources": []
         },
         "CreateReferenceStore": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateReferenceStore",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:TagKeys"
-            ],
-            "description": "Grants permission to create a Reference Store",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "CreateRunGroup": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateRunGroup",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:TagKeys"
-            ],
-            "description": "Grants permission to create a new workflow run group",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "CreateSequenceStore": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateSequenceStore",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:TagKeys"
-            ],
-            "description": "Grants permission to create a Sequence Store",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "CreateVariantStore": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateVariantStore",
             "condition_keys": [],
-            "description": "Grants permission to create a Variant Store",
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "CreateWorkflow": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateWorkflow",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:TagKeys"
-            ],
-            "description": "Grants permission to create a new workflow with a workflow definition and template of workflow parameters",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DeleteAnnotationStore": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteAnnotationStore",
             "condition_keys": [],
-            "description": "Grants permission to delete an Annotation Store",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "AnnotationStore"
-            ]
+            "resources": []
         },
         "DeleteReference": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteReference",
             "condition_keys": [],
-            "description": "Grants permission to delete a Reference in the given Reference Store",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "reference",
-                "referenceStore"
-            ]
+            "resources": []
         },
         "DeleteReferenceStore": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteReferenceStore",
             "condition_keys": [],
-            "description": "Grants permission to delete a Reference Store",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "referenceStore"
-            ]
+            "resources": []
         },
         "DeleteRun": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteRun",
             "condition_keys": [],
-            "description": "Grants permission to delete a workflow run",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "run"
-            ]
+            "resources": []
         },
         "DeleteRunGroup": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteRunGroup",
             "condition_keys": [],
-            "description": "Grants permission to delete a workflow run group",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "runGroup"
-            ]
+            "resources": []
         },
         "DeleteSequenceStore": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteSequenceStore",
             "condition_keys": [],
-            "description": "Grants permission to delete a Sequence Store",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "sequenceStore"
-            ]
+            "resources": []
         },
         "DeleteVariantStore": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteVariantStore",
             "condition_keys": [],
-            "description": "Grants permission to delete a Variant Store",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "VariantStore"
-            ]
+            "resources": []
         },
         "DeleteWorkflow": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteWorkflow",
             "condition_keys": [],
-            "description": "Grants permission to delete a workflow",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "workflow"
-            ]
+            "resources": []
         },
         "GetAnnotationImportJob": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "GetAnnotationImportJob",
             "condition_keys": [],
-            "description": "Grants permission to get the status of an Annotation Import Job",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "AnnotationImportJob"
-            ]
+            "resources": []
         },
         "GetAnnotationStore": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "GetAnnotationStore",
             "condition_keys": [],
-            "description": "Grants permission to get detailed information about an Annotation Store",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "AnnotationStore"
-            ]
+            "resources": []
         },
         "GetReadSet": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "GetReadSet",
             "condition_keys": [],
-            "description": "Grants permission to get a Read Set in the given Sequence Store",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "readSet",
-                "sequenceStore"
-            ]
+            "resources": []
         },
         "GetReadSetActivationJob": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "GetReadSetActivationJob",
             "condition_keys": [],
-            "description": "Grants permission to get details about a Read Set activation job for the given Sequence Store",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "sequenceStore"
-            ]
+            "resources": []
         },
         "GetReadSetExportJob": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "GetReadSetExportJob",
             "condition_keys": [],
-            "description": "Grants permission to get details about a Read Set export job for the given Sequence Store",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "sequenceStore"
-            ]
+            "resources": []
         },
         "GetReadSetImportJob": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "GetReadSetImportJob",
             "condition_keys": [],
-            "description": "Grants permission to get details about a Read Set import job for the given Sequence Store",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "sequenceStore"
-            ]
+            "resources": []
         },
         "GetReadSetMetadata": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "GetReadSetMetadata",
             "condition_keys": [],
-            "description": "Grants permission to get details about a Read Set in the given Sequence Store",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "readSet",
-                "sequenceStore"
-            ]
+            "resources": []
         },
         "GetReference": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "GetReference",
             "condition_keys": [],
-            "description": "Grants permission to get a Reference in the given Reference Store",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "reference",
-                "referenceStore"
-            ]
+            "resources": []
         },
         "GetReferenceImportJob": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "GetReferenceImportJob",
             "condition_keys": [],
-            "description": "Grants permission to get details about a Reference import job for the given Reference Store",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "referenceStore"
-            ]
+            "resources": []
         },
         "GetReferenceMetadata": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "GetReferenceMetadata",
             "condition_keys": [],
-            "description": "Grants permission to get details about a Reference in the given Reference Store",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "reference",
-                "referenceStore"
-            ]
+            "resources": []
         },
         "GetReferenceStore": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "GetReferenceStore",
             "condition_keys": [],
-            "description": "Grants permission to get details about a Reference Store",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "referenceStore"
-            ]
+            "resources": []
         },
         "GetRun": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "GetRun",
             "condition_keys": [],
-            "description": "Grants permission to retrieve workflow run details",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "run"
-            ]
+            "resources": []
         },
         "GetRunGroup": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "GetRunGroup",
             "condition_keys": [],
-            "description": "Grants permission to retrieve workflow run group details",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "runGroup"
-            ]
+            "resources": []
         },
         "GetRunTask": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "GetRunTask",
             "condition_keys": [],
-            "description": "Grants permission to retrieve workflow task details",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "TaskResource",
-                "run"
-            ]
+            "resources": []
         },
         "GetSequenceStore": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "GetSequenceStore",
             "condition_keys": [],
-            "description": "Grants permission to get details about a Sequence Store",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "sequenceStore"
-            ]
+            "resources": []
         },
         "GetVariantImportJob": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "GetVariantImportJob",
             "condition_keys": [],
-            "description": "Grants permission to get the status of a Variant Import Job",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "VariantImportJob"
-            ]
+            "resources": []
         },
         "GetVariantStore": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "GetVariantStore",
             "condition_keys": [],
-            "description": "Grants permission to get detailed information about a Variant Store",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "VariantStore"
-            ]
+            "resources": []
         },
         "GetWorkflow": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "GetWorkflow",
             "condition_keys": [],
-            "description": "Grants permission to retrieve workflow details",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "workflow"
-            ]
+            "resources": []
         },
         "ListAnnotationImportJobs": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "ListAnnotationImportJobs",
             "condition_keys": [],
-            "description": "Grants permission to get a list of Annotation Import Jobs",
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListAnnotationStores": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "ListAnnotationStores",
             "condition_keys": [],
-            "description": "Grants permission to retrieve a list of information about Annotation Stores",
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListMultipartReadSetUploads": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "ListMultipartReadSetUploads",
             "condition_keys": [],
-            "description": "Grants permission to list multipart read set uploads",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "sequenceStore"
-            ]
+            "resources": []
         },
         "ListReadSetActivationJobs": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "ListReadSetActivationJobs",
             "condition_keys": [],
-            "description": "Grants permission to list Read Set activation jobs for the given Sequence Store",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "sequenceStore"
-            ]
+            "resources": []
         },
         "ListReadSetExportJobs": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "ListReadSetExportJobs",
             "condition_keys": [],
-            "description": "Grants permission to list Read Set export jobs for the given Sequence Store",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "sequenceStore"
-            ]
+            "resources": []
         },
         "ListReadSetImportJobs": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "ListReadSetImportJobs",
             "condition_keys": [],
-            "description": "Grants permission to list Read Set import jobs for the given Sequence Store",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "sequenceStore"
-            ]
+            "resources": []
         },
         "ListReadSetUploadParts": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "ListReadSetUploadParts",
             "condition_keys": [],
-            "description": "Grants permission to list read set upload parts",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "sequenceStore"
-            ]
+            "resources": []
         },
         "ListReadSets": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "ListReadSets",
             "condition_keys": [],
-            "description": "Grants permission to list Read Sets in the given Sequence Store",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "sequenceStore"
-            ]
+            "resources": []
         },
         "ListReferenceImportJobs": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "ListReferenceImportJobs",
             "condition_keys": [],
-            "description": "Grants permission to list Reference import jobs for the given Reference Store",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "referenceStore"
-            ]
+            "resources": []
         },
         "ListReferenceStores": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "ListReferenceStores",
             "condition_keys": [],
-            "description": "Grants permission to list Reference Stores",
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListReferences": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "ListReferences",
             "condition_keys": [],
-            "description": "Grants permission to list References in the given Reference Store",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "referenceStore"
-            ]
+            "resources": []
         },
         "ListRunGroups": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "ListRunGroups",
             "condition_keys": [],
-            "description": "Grants permission to retrieve a list of workflow run groups",
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListRunTasks": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "ListRunTasks",
             "condition_keys": [],
-            "description": "Grants permission to retrieve a list of tasks for a workflow run",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "run"
-            ]
+            "resources": []
         },
         "ListRuns": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "ListRuns",
             "condition_keys": [],
-            "description": "Grants permission to retrieve a list of workflow runs",
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListSequenceStores": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "ListSequenceStores",
             "condition_keys": [],
-            "description": "Grants permission to list Sequence Stores",
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListTagsForResource": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "ListTagsForResource",
             "condition_keys": [],
-            "description": "Grants permission to retrieve a list of resource AWS tags",
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListVariantImportJobs": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "ListVariantImportJobs",
             "condition_keys": [],
-            "description": "Grants permission to get a list of Variant Import Jobs",
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListVariantStores": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "ListVariantStores",
             "condition_keys": [],
-            "description": "Grants permission to retrieve a list of metadata for Variant Stores",
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListWorkflows": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "ListWorkflows",
             "condition_keys": [],
-            "description": "Grants permission to retrieve a list of available workflows",
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "StartAnnotationImportJob": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "StartAnnotationImportJob",
             "condition_keys": [],
-            "description": "Grants permission to import a list of Annotation files to an Annotation Store",
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "StartReadSetActivationJob": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "StartReadSetActivationJob",
             "condition_keys": [],
-            "description": "Grants permission to start a Read Set activation job from the given Sequence Store",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "sequenceStore"
-            ]
+            "resources": []
         },
         "StartReadSetExportJob": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "StartReadSetExportJob",
             "condition_keys": [],
-            "description": "Grants permission to start a Read Set export job from the given Sequence Store",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "sequenceStore"
-            ]
+            "resources": []
         },
         "StartReadSetImportJob": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "StartReadSetImportJob",
             "condition_keys": [],
-            "description": "Grants permission to start a Read Set import job into the given Sequence Store",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "sequenceStore"
-            ]
+            "resources": []
         },
         "StartReferenceImportJob": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "StartReferenceImportJob",
             "condition_keys": [],
-            "description": "Grants permission to start a Reference import job into the given Reference Store",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "referenceStore"
-            ]
+            "resources": []
         },
         "StartRun": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "StartRun",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:TagKeys"
-            ],
-            "description": "Grants permission to start a workflow run",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "StartVariantImportJob": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "StartVariantImportJob",
             "condition_keys": [],
-            "description": "Grants permission to import a list of variant files to an Variant Store",
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "TagResource": {
-            "access_level": "Tagging",
+            "access_level": "Undocumented",
             "action": "TagResource",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:TagKeys"
-            ],
-            "description": "Grants permission to add AWS tags to a resource",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "readSet",
-                "reference",
-                "referenceStore",
-                "run",
-                "runGroup",
-                "sequenceStore",
-                "workflow"
-            ]
+            "resources": []
         },
         "UntagResource": {
-            "access_level": "Tagging",
+            "access_level": "Undocumented",
             "action": "UntagResource",
-            "condition_keys": [
-                "aws:TagKeys"
-            ],
-            "description": "Grants permission to remove resource AWS tags",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "readSet",
-                "reference",
-                "referenceStore",
-                "run",
-                "runGroup",
-                "sequenceStore",
-                "workflow"
-            ]
+            "resources": []
         },
         "UpdateAnnotationStore": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "UpdateAnnotationStore",
             "condition_keys": [],
-            "description": "Grants permission to update information about the Annotation Store",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "AnnotationStore"
-            ]
+            "resources": []
         },
         "UpdateRunGroup": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "UpdateRunGroup",
             "condition_keys": [],
-            "description": "Grants permission to update a workflow run group",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "runGroup"
-            ]
+            "resources": []
         },
         "UpdateVariantStore": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "UpdateVariantStore",
             "condition_keys": [],
-            "description": "Grants permission to update metadata about the Variant Store",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "VariantStore"
-            ]
+            "resources": []
         },
         "UpdateWorkflow": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "UpdateWorkflow",
             "condition_keys": [],
-            "description": "Grants permission to update workflow details",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "workflow"
-            ]
+            "resources": []
         },
         "UploadReadSetPart": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "UploadReadSetPart",
             "condition_keys": [],
-            "description": "Grants permission to upload read set parts",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "sequenceStore"
-            ]
+            "resources": []
         }
     },
     "opsworks": {
         "AssignInstance": {
             "access_level": "Write",
             "action": "AssignInstance",
             "condition_keys": [],
@@ -108935,20 +109006,22 @@
             "description": "Grants permission to update a campaign",
             "orphan": false,
             "resources": [
                 "campaign"
             ]
         },
         "UpdateDataset": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "UpdateDataset",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to update a dataset",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "dataset"
+            ]
         },
         "UpdateMetricAttribution": {
             "access_level": "Write",
             "action": "UpdateMetricAttribution",
             "condition_keys": [],
             "description": "Grants permission to update a metric attribution",
             "orphan": false,
@@ -109842,20 +109915,22 @@
             "action": "GetProfileObjectTypeTemplate",
             "condition_keys": [],
             "description": "Grants permission to get a specific object type template",
             "orphan": false,
             "resources": []
         },
         "GetSimilarProfiles": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "GetSimilarProfiles",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to get all the similar profiles in the domain",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "domains"
+            ]
         },
         "GetWorkflow": {
             "access_level": "Read",
             "action": "GetWorkflow",
             "condition_keys": [],
             "description": "Grants permission to get workflow details in a domain",
             "orphan": false,
@@ -109965,20 +110040,22 @@
             "orphan": false,
             "resources": [
                 "domains",
                 "object-types"
             ]
         },
         "ListRuleBasedMatches": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "ListRuleBasedMatches",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to list all the rule-based matching result in the domain",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "domains"
+            ]
         },
         "ListTagsForResource": {
             "access_level": "Read",
             "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Grants permission to list tags for a resource",
             "orphan": false,
@@ -112481,28 +112558,32 @@
             "description": "Grants permission to describe permissions for a QuickSight Dashboard",
             "orphan": false,
             "resources": [
                 "dashboard"
             ]
         },
         "DescribeDashboardSnapshotJob": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "DescribeDashboardSnapshotJob",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to describe a dashboard snapshot job",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "dashboardSnapshotJob"
+            ]
         },
         "DescribeDashboardSnapshotJobResult": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "DescribeDashboardSnapshotJobResult",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to describe result of a dashboard snapshot job",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "dashboardSnapshotJob"
+            ]
         },
         "DescribeDataSet": {
             "access_level": "Read",
             "action": "DescribeDataSet",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
@@ -113335,20 +113416,22 @@
             "description": "Grants permission to search for a sub-set of QuickSight groups",
             "orphan": false,
             "resources": [
                 "group"
             ]
         },
         "SearchUsers": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "SearchUsers",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to search the QuickSight users belonging to this account",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "user"
+            ]
         },
         "SetGroupMapping": {
             "access_level": "Write",
             "action": "SetGroupMapping",
             "condition_keys": [],
             "description": "Grants permission to use Amazon QuickSight, in Enterprise edition, to display your Microsoft Active Directory directory groups so that you can choose which ones to map to roles in Amazon QuickSight",
             "orphan": false,
@@ -113371,20 +113454,22 @@
             "description": "Grants permission to start an asset bundle import job",
             "orphan": false,
             "resources": [
                 "assetBundleImportJob"
             ]
         },
         "StartDashboardSnapshotJob": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "StartDashboardSnapshotJob",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to start a dashboard snapshot job",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "dashboardSnapshotJob"
+            ]
         },
         "Subscribe": {
             "access_level": "Write",
             "action": "Subscribe",
             "condition_keys": [
                 "quicksight:DirectoryType",
                 "quicksight:Edition"
@@ -122376,20 +122461,25 @@
             "description": "Grants permission to create a Firewall rule group",
             "orphan": false,
             "resources": [
                 "firewall-rule-group"
             ]
         },
         "CreateOutpostResolver": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateOutpostResolver",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys"
+            ],
+            "description": "Grants permission to create a Route 53 Resolver on Outposts",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "outpost-resolver"
+            ]
         },
         "CreateResolverEndpoint": {
             "access_level": "Write",
             "action": "CreateResolverEndpoint",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
@@ -122452,20 +122542,22 @@
             "description": "Grants permission to delete a Firewall rule group",
             "orphan": false,
             "resources": [
                 "firewall-rule-group"
             ]
         },
         "DeleteOutpostResolver": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteOutpostResolver",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to delete a Route 53 Resolver on Outposts",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "outpost-resolver"
+            ]
         },
         "DeleteResolverEndpoint": {
             "access_level": "Write",
             "action": "DeleteResolverEndpoint",
             "condition_keys": [],
             "description": "Grants permission to delete a Resolver endpoint. The effect of deleting a Resolver endpoint depends on whether it's an inbound or an outbound endpoint",
             "orphan": false,
@@ -122580,20 +122672,22 @@
             "description": "Grants permission to get information about a specified Firewall rule group policy, which specifies the Firewall rule group operations and resources that you want to allow another AWS account to use",
             "orphan": false,
             "resources": [
                 "firewall-rule-group"
             ]
         },
         "GetOutpostResolver": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "GetOutpostResolver",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to get information about a specified Route 53 Resolver on Outposts",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "outpost-resolver"
+            ]
         },
         "GetResolverConfig": {
             "access_level": "Read",
             "action": "GetResolverConfig",
             "condition_keys": [],
             "description": "Grants permission to get the Resolver Config status within the specified resource",
             "orphan": false,
@@ -122738,18 +122832,18 @@
             "description": "Grants permission to list all the Firewall rule under a speicfied Firewall rule group",
             "orphan": false,
             "resources": [
                 "firewall-rule-group"
             ]
         },
         "ListOutpostResolvers": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "ListOutpostResolvers",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to list all instances of Route 53 Resolver on Outposts that were created using the current AWS account",
             "orphan": false,
             "resources": []
         },
         "ListResolverConfigs": {
             "access_level": "List",
             "action": "ListResolverConfigs",
             "condition_keys": [],
@@ -122825,14 +122919,15 @@
             "condition_keys": [],
             "description": "Grants permission to list the tags that you associated with the specified resource",
             "orphan": false,
             "resources": [
                 "firewall-domain-list",
                 "firewall-rule-group",
                 "firewall-rule-group-association",
+                "outpost-resolver",
                 "resolver-endpoint",
                 "resolver-query-log-config",
                 "resolver-rule"
             ]
         },
         "PutFirewallRuleGroupPolicy": {
             "access_level": "Permissions management",
@@ -122874,14 +122969,15 @@
             "description": "Grants permission to add one or more tags to a specified resource",
             "orphan": false,
             "resources": [
                 "firewall-config",
                 "firewall-domain-list",
                 "firewall-rule-group",
                 "firewall-rule-group-association",
+                "outpost-resolver",
                 "resolver-dnssec-config",
                 "resolver-endpoint",
                 "resolver-query-log-config",
                 "resolver-rule"
             ]
         },
         "UntagResource": {
@@ -122893,14 +122989,15 @@
             "description": "Grants permission to remove one or more tags from a specified resource",
             "orphan": false,
             "resources": [
                 "firewall-config",
                 "firewall-domain-list",
                 "firewall-rule-group",
                 "firewall-rule-group-association",
+                "outpost-resolver",
                 "resolver-dnssec-config",
                 "resolver-endpoint",
                 "resolver-query-log-config",
                 "resolver-rule"
             ]
         },
         "UpdateFirewallConfig": {
@@ -122941,20 +123038,22 @@
             "description": "Grants permission to update selected settings for an Firewall rule group association",
             "orphan": false,
             "resources": [
                 "firewall-rule-group-association"
             ]
         },
         "UpdateOutpostResolver": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "UpdateOutpostResolver",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to update seletected settings for a specified Route 53 Resolver on Outposts",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "outpost-resolver"
+            ]
         },
         "UpdateResolverConfig": {
             "access_level": "Write",
             "action": "UpdateResolverConfig",
             "condition_keys": [],
             "description": "Grants permission to update the Resolver Config status within the specified resource",
             "orphan": false,
@@ -141000,15 +141099,18 @@
             "resources": [
                 "servicesetting"
             ]
         },
         "ResumeSession": {
             "access_level": "Write",
             "action": "ResumeSession",
-            "condition_keys": [],
+            "condition_keys": [
+                "ssm:resourceTag/aws:ssmmessages:session-id",
+                "ssm:resourceTag/aws:ssmmessages:target-id"
+            ],
             "description": "Grants permission to reconnect a Session Manager session to a managed instance",
             "orphan": false,
             "resources": [
                 "session"
             ]
         },
         "SendAutomationSignal": {
@@ -141100,15 +141202,18 @@
             "resources": [
                 "automation-execution"
             ]
         },
         "TerminateSession": {
             "access_level": "Write",
             "action": "TerminateSession",
-            "condition_keys": [],
+            "condition_keys": [
+                "ssm:resourceTag/aws:ssmmessages:session-id",
+                "ssm:resourceTag/aws:ssmmessages:target-id"
+            ],
             "description": "Grants permission to permanently end a Session Manager connection to an instance",
             "orphan": false,
             "resources": [
                 "session"
             ]
         },
         "UnlabelParameterVersion": {
@@ -142061,15 +142166,17 @@
         },
         "DeregisterApplication": {
             "access_level": "Write",
             "action": "DeregisterApplication",
             "condition_keys": [],
             "description": "Grants permission to deregister an SAP application with SSM for SAP",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "application"
+            ]
         },
         "GetApplication": {
             "access_level": "Read",
             "action": "GetApplication",
             "condition_keys": [],
             "description": "Grants permission to access information about an application registered with SSM for SAP by providing the application ID or application ARN",
             "orphan": false,
@@ -142077,15 +142184,17 @@
         },
         "GetComponent": {
             "access_level": "Read",
             "action": "GetComponent",
             "condition_keys": [],
             "description": "Grants permission to access information about a component registered with SSM for SAP by providing the application ID and component ID",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "component"
+            ]
         },
         "GetDatabase": {
             "access_level": "Read",
             "action": "GetDatabase",
             "condition_keys": [],
             "description": "Grants permission to access information about a database registered with SSM for SAP by providing the application ID, component ID, and database ID",
             "orphan": false,
@@ -142117,15 +142226,17 @@
         },
         "ListComponents": {
             "access_level": "List",
             "action": "ListComponents",
             "condition_keys": [],
             "description": "Grants permission to retrieve a list of all components in the account of customer, or a specific application",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "application"
+            ]
         },
         "ListDatabases": {
             "access_level": "List",
             "action": "ListDatabases",
             "condition_keys": [],
             "description": "Grants permission to retrieve a list of all databases in the account of customer, or a specific application",
             "orphan": false,
@@ -142171,55 +142282,61 @@
             "action": "RestoreDatabase",
             "condition_keys": [],
             "description": "Grants permission to restore a database from another database",
             "orphan": false,
             "resources": []
         },
         "StartApplicationRefresh": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "StartApplicationRefresh",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to start an on-demand discovery of a registered SSM for SAP application",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "application"
+            ]
         },
         "TagResource": {
             "access_level": "Tagging",
             "action": "TagResource",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
             ],
             "description": "Grants permission to tag a specified resource ARN",
             "orphan": false,
             "resources": [
                 "application",
+                "component",
                 "database"
             ]
         },
         "UntagResource": {
             "access_level": "Tagging",
             "action": "UntagResource",
             "condition_keys": [
                 "aws:TagKeys"
             ],
             "description": "Grants permission to remove tags from a specified resource ARN",
             "orphan": false,
             "resources": [
                 "application",
+                "component",
                 "database"
             ]
         },
         "UpdateApplicationSettings": {
             "access_level": "Write",
             "action": "UpdateApplicationSettings",
             "condition_keys": [],
             "description": "Grants permission to update settings of a registered SSM for SAP application",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "application"
+            ]
         },
         "UpdateHANABackupSettings": {
             "access_level": "Write",
             "action": "UpdateHANABackupSettings",
             "condition_keys": [],
             "description": "Grants permission to update the HANA backup settings of a specified database",
             "orphan": false,
@@ -144479,23 +144596,23 @@
                 "gateway"
             ]
         },
         "ListAutomaticTapeCreationPolicies": {
             "access_level": "List",
             "action": "ListAutomaticTapeCreationPolicies",
             "condition_keys": [],
-            "description": "Grants permission to list the automatic tape creation policies configured on the specified gateway-VTL or all gateway-VTLs owned by your account",
+            "description": "Grants permission to list the automatic tape creation policies configured on the specified gateway-VTL or all gateway-VTLs owned by your AWS account",
             "orphan": false,
             "resources": []
         },
         "ListFileShares": {
             "access_level": "List",
             "action": "ListFileShares",
             "condition_keys": [],
-            "description": "Grants permission to get a list of the file shares for a specific file gateway, or the list of file shares that belong to the calling user account",
+            "description": "Grants permission to get a list of the file shares for a specific file gateway, or the list of file shares owned by your AWS account",
             "orphan": false,
             "resources": []
         },
         "ListFileSystemAssociations": {
             "access_level": "List",
             "action": "ListFileSystemAssociations",
             "condition_keys": [],
@@ -148040,20 +148157,22 @@
                 "profile",
                 "server",
                 "user",
                 "workflow"
             ]
         },
         "TestConnection": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "TestConnection",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to test a connector's connection to remote server",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "connector"
+            ]
         },
         "TestIdentityProvider": {
             "access_level": "Read",
             "action": "TestIdentityProvider",
             "condition_keys": [],
             "description": "Grants permission to test a server's custom identity provider",
             "orphan": false,
```

### Comparing `iam_actions-1.2.20230726/iam_actions/generate/action_map.py` & `iam_actions-1.2.20230727/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230726/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20230727/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230726/iam_actions/generate/generate.py` & `iam_actions-1.2.20230727/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230726/iam_actions/generate/notifier.py` & `iam_actions-1.2.20230727/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230726/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20230727/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230726/iam_actions/generate/services.py` & `iam_actions-1.2.20230727/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230726/iam_actions/policies.json` & `iam_actions-1.2.20230727/iam_actions/policies.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9994772228878531%*

 * *Differences: {"'serviceMap'": "{'Amazon Lex V2': {'Actions': {insert: [(65, 'ListIntentMetrics'), (66, "*

 * *                 "'ListIntentPaths'), (67, 'ListIntentStageMetrics'), (70, "*

 * *                 "'ListSessionAnalyticsData'), (71, 'ListSessionMetrics')]}}, 'AWS Cost Explorer "*

 * *                 "Service': {'Actions': {insert: [(27, "*

 * *                 "'GetSavingsPlanPurchaseRecommendationDetails')]}}, 'Amazon Managed Blockchain': "*

 * *                 "{'Actions': {insert: [(15, 'InvokeRpcBitcoinMainnet'), (16, "*

 * *        […]*

```diff
@@ -2468,14 +2468,15 @@
                 "GetCostForecast",
                 "GetDimensionValues",
                 "GetPreferences",
                 "GetReservationCoverage",
                 "GetReservationPurchaseRecommendation",
                 "GetReservationUtilization",
                 "GetRightsizingRecommendation",
+                "GetSavingsPlanPurchaseRecommendationDetails",
                 "GetSavingsPlansCoverage",
                 "GetSavingsPlansPurchaseRecommendation",
                 "GetSavingsPlansUtilization",
                 "GetSavingsPlansUtilizationDetails",
                 "GetTags",
                 "GetUsageForecast",
                 "ListCostAllocationTags",
@@ -3930,14 +3931,43 @@
             "ARNRegex": "^arn:${Partition}:elemental-support-content:.+:.+:.+",
             "Actions": [
                 "Query"
             ],
             "HasResource": false,
             "StringPrefix": "elemental-support-content"
         },
+        "AWS Entity Resolution": {
+            "ARNFormat": "arn:aws:entityresolution:${Region}:${Account}:${ResourceType}/${ResourceName}",
+            "ARNRegex": "^arn:aws:entityresolution:.+:.+:.+",
+            "Actions": [
+                "CreateMatchingWorkflow",
+                "CreateSchemaMapping",
+                "DeleteMatchingWorkflow",
+                "DeleteSchemaMapping",
+                "GetMatchId",
+                "GetMatchingJob",
+                "GetMatchingWorkflow",
+                "GetSchemaMapping",
+                "ListMatchingJobs",
+                "ListMatchingWorkflows",
+                "ListSchemaMappings",
+                "ListTagsForResource",
+                "StartMatchingJob",
+                "TagResource",
+                "UntagResource",
+                "UpdateMatchingWorkflow"
+            ],
+            "HasResource": true,
+            "StringPrefix": "entityresolution",
+            "conditionKeys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys"
+            ]
+        },
         "AWS Fault Injection Simulator": {
             "ARNFormat": "arn:aws:fis:${Region}:${Account}:${ResourceType}/${ResourceName}",
             "ARNRegex": "^arn:aws:fis:.+:.+:.+",
             "Actions": [
                 "CreateExperimentTemplate",
                 "DeleteExperimentTemplate",
                 "GetAction",
@@ -14938,14 +14968,15 @@
         },
         "Amazon Interactive Video Service": {
             "ARNFormat": "arn:aws:ivs:${Region}:${Account}:${ArnType}/${ResourceId}",
             "ARNRegex": "^arn:aws:ivs:.+:.+:.+",
             "Actions": [
                 "BatchGetChannel",
                 "BatchGetStreamKey",
+                "BatchStartViewerSessionRevocation",
                 "CreateChannel",
                 "CreateParticipantToken",
                 "CreateRecordingConfiguration",
                 "CreateStage",
                 "CreateStreamKey",
                 "DeleteChannel",
                 "DeletePlaybackKeyPair",
@@ -14971,14 +15002,15 @@
                 "ListStageSessions",
                 "ListStages",
                 "ListStreamKeys",
                 "ListStreamSessions",
                 "ListStreams",
                 "ListTagsForResource",
                 "PutMetadata",
+                "StartViewerSessionRevocation",
                 "StopStream",
                 "TagResource",
                 "UntagResource",
                 "UpdateChannel",
                 "UpdateStage"
             ],
             "HasResource": true,
@@ -15470,16 +15502,21 @@
                 "ListBotVersions",
                 "ListBots",
                 "ListBuiltInIntents",
                 "ListBuiltInSlotTypes",
                 "ListCustomVocabularyItems",
                 "ListExports",
                 "ListImports",
+                "ListIntentMetrics",
+                "ListIntentPaths",
+                "ListIntentStageMetrics",
                 "ListIntents",
                 "ListRecommendedIntents",
+                "ListSessionAnalyticsData",
+                "ListSessionMetrics",
                 "ListSlotTypes",
                 "ListSlots",
                 "ListTagsForResource",
                 "ListTestExecutionResultItems",
                 "ListTestExecutions",
                 "ListTestSetRecords",
                 "ListTestSets",
@@ -16067,14 +16104,16 @@
                 "GET",
                 "GetAccessor",
                 "GetMember",
                 "GetNetwork",
                 "GetNode",
                 "GetProposal",
                 "Invoke",
+                "InvokeRpcBitcoinMainnet",
+                "InvokeRpcBitcoinTestnet",
                 "ListAccessors",
                 "ListInvitations",
                 "ListMembers",
                 "ListNetworks",
                 "ListNodes",
                 "ListProposalVotes",
                 "ListProposals",
@@ -16091,14 +16130,28 @@
             "StringPrefix": "managedblockchain",
             "conditionKeys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:ResourceTag/${TagKey}",
                 "aws:TagKeys"
             ]
         },
+        "Amazon Managed Blockchain Query": {
+            "ARNFormat": "arn:${Partition}:managedblockchain-query:${Region}:${Account}:${ResourceType}/${ResourceName}",
+            "ARNRegex": "^arn:${Partition}:managedblockchain-query:.*:[0-9]*:.+",
+            "Actions": [
+                "BatchGetTokenBalance",
+                "GetTokenBalance",
+                "GetTransaction",
+                "ListTokenBalances",
+                "ListTransactionEvents",
+                "ListTransactions"
+            ],
+            "HasResource": false,
+            "StringPrefix": "managedblockchain-query"
+        },
         "Amazon Managed Grafana": {
             "ARNFormat": "arn:aws:grafana:${Region}:${Account}:/${ResourceType}/${ResourceId}",
             "ARNRegex": "^arn:aws:grafana:.+:.+:.+",
             "Actions": [
                 "AssociateLicense",
                 "CreateWorkspace",
                 "CreateWorkspaceApiKey",
```

### Comparing `iam_actions-1.2.20230726/iam_actions/resourcetypes.json` & `iam_actions-1.2.20230727/iam_actions/resourcetypes.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.991161849617231%*

 * *Differences: {"'entityresolution'": 'OrderedDict()',*

 * * "'healthlake'": '{replace: OrderedDict()}',*

 * * "'managedblockchain-query'": 'OrderedDict()',*

 * * "'omics'": '{replace: OrderedDict()}',*

 * * "'quicksight'": "{'dashboardSnapshotJob': OrderedDict([('arn_pattern', "*

 * *                 "'arn:*:quicksight:*:*:dashboard/*/snapshot-job/*'), ('condition_keys', "*

 * *                 "'aws:ResourceTag/${TagKey}')])}",*

 * * "'route53resolver'": "{'outpost-resolver': OrderedDict([('arn_pattern', "*

 * *                      "'arn:*:route53resolver:*: […]*

```diff
@@ -2506,14 +2506,15 @@
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
         "jobRun": {
             "arn_pattern": "arn:*:emr-serverless:*:*:/applications/*/jobruns/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         }
     },
+    "entityresolution": {},
     "es": {
         "domain": {
             "arn_pattern": "arn:*:es:*:*:domain/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
         "es_role": {
             "arn_pattern": "arn:*:iam::*:role/aws-service-role/es.amazonaws.com/AWSServiceRoleForAmazonOpenSearchService",
@@ -3155,20 +3156,15 @@
     },
     "health": {
         "event": {
             "arn_pattern": "arn:*:health:*::event/*/*/*",
             "condition_keys": null
         }
     },
-    "healthlake": {
-        "datastore": {
-            "arn_pattern": "arn:*:healthlake:*:*:datastore/fhir/*",
-            "condition_keys": "aws:ResourceTag/${TagKey}"
-        }
-    },
+    "healthlake": {},
     "honeycode": {
         "screen": {
             "arn_pattern": "arn:*:honeycode:*:*:screen:workbook/*/app/*/screen/*",
             "condition_keys": null
         },
         "screen-automation": {
             "arn_pattern": "arn:*:honeycode:*:*:screen-automation:workbook/*/app/*/screen/*/automation/*",
@@ -4094,14 +4090,15 @@
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
         "proposal": {
             "arn_pattern": "arn:*:managedblockchain:*::proposals/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         }
     },
+    "managedblockchain-query": {},
     "marketplacecommerceanalytics": {},
     "mechanicalturk": {},
     "mediaconnect": {
         "Bridge": {
             "arn_pattern": "arn:*:mediaconnect:*:*:bridge:*:*",
             "condition_keys": null
         },
@@ -4591,68 +4588,15 @@
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
         "Sink": {
             "arn_pattern": "arn:*:oam:*:*:sink/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         }
     },
-    "omics": {
-        "AnnotationImportJob": {
-            "arn_pattern": "arn:*:omics:*:*:annotationImportJob/*",
-            "condition_keys": "omics:AnnotationImportJobJobId"
-        },
-        "AnnotationStore": {
-            "arn_pattern": "arn:*:omics:*:*:annotationStore/*",
-            "condition_keys": "omics:AnnotationStoreName"
-        },
-        "TaggingResource": {
-            "arn_pattern": "arn:*:omics:*:*:tag/*",
-            "condition_keys": null
-        },
-        "TaskResource": {
-            "arn_pattern": "arn:*:omics:*:*:task/*",
-            "condition_keys": null
-        },
-        "VariantImportJob": {
-            "arn_pattern": "arn:*:omics:*:*:variantImportJob/*",
-            "condition_keys": "omics:VariantImportJobJobId"
-        },
-        "VariantStore": {
-            "arn_pattern": "arn:*:omics:*:*:variantStore/*",
-            "condition_keys": "omics:VariantStoreName"
-        },
-        "readSet": {
-            "arn_pattern": "arn:*:omics:*:*:sequenceStore/*/readSet/*",
-            "condition_keys": "aws:ResourceTag/${TagKey}"
-        },
-        "reference": {
-            "arn_pattern": "arn:*:omics:*:*:referenceStore/*/reference/*",
-            "condition_keys": "aws:ResourceTag/${TagKey}"
-        },
-        "referenceStore": {
-            "arn_pattern": "arn:*:omics:*:*:referenceStore/*",
-            "condition_keys": "aws:ResourceTag/${TagKey}"
-        },
-        "run": {
-            "arn_pattern": "arn:*:omics:*:*:run/*",
-            "condition_keys": "aws:ResourceTag/${TagKey}"
-        },
-        "runGroup": {
-            "arn_pattern": "arn:*:omics:*:*:runGroup/*",
-            "condition_keys": "aws:ResourceTag/${TagKey}"
-        },
-        "sequenceStore": {
-            "arn_pattern": "arn:*:omics:*:*:sequenceStore/*",
-            "condition_keys": "aws:ResourceTag/${TagKey}"
-        },
-        "workflow": {
-            "arn_pattern": "arn:*:omics:*:*:workflow/*",
-            "condition_keys": "aws:ResourceTag/${TagKey}"
-        }
-    },
+    "omics": {},
     "opsworks": {
         "stack": {
             "arn_pattern": "arn:*:opsworks:*:*:stack/*/",
             "condition_keys": null
         }
     },
     "opsworks-cm": {
@@ -4962,14 +4906,18 @@
             "arn_pattern": "arn:*:quicksight:*:*:customization/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
         "dashboard": {
             "arn_pattern": "arn:*:quicksight:*:*:dashboard/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
+        "dashboardSnapshotJob": {
+            "arn_pattern": "arn:*:quicksight:*:*:dashboard/*/snapshot-job/*",
+            "condition_keys": "aws:ResourceTag/${TagKey}"
+        },
         "dataset": {
             "arn_pattern": "arn:*:quicksight:*:*:dataset/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
         "datasource": {
             "arn_pattern": "arn:*:quicksight:*:*:datasource/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
@@ -5456,14 +5404,18 @@
             "arn_pattern": "arn:*:route53resolver:*:*:firewall-rule-group/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
         "firewall-rule-group-association": {
             "arn_pattern": "arn:*:route53resolver:*:*:firewall-rule-group-association/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
+        "outpost-resolver": {
+            "arn_pattern": "arn:*:route53resolver:*:*:outpost-resolver/*",
+            "condition_keys": "aws:ResourceTag/${TagKey}"
+        },
         "resolver-config": {
             "arn_pattern": "arn:*:route53resolver:*:*:resolver-config/*",
             "condition_keys": null
         },
         "resolver-dnssec-config": {
             "arn_pattern": "arn:*:route53resolver:*:*:resolver-dnssec-config/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
@@ -6097,15 +6049,15 @@
         },
         "servicesetting": {
             "arn_pattern": "arn:*:ssm:*:*:servicesetting/*",
             "condition_keys": null
         },
         "session": {
             "arn_pattern": "arn:*:ssm:*:*:session/*",
-            "condition_keys": null
+            "condition_keys": "ssm:resourceTag/aws:ssmmessages:session-id"
         },
         "task": {
             "arn_pattern": "arn:*:ecs:*:*:task/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
         "windowtarget": {
             "arn_pattern": "arn:*:ssm:*:*:windowtarget/*",
@@ -6154,14 +6106,18 @@
         }
     },
     "ssm-sap": {
         "application": {
             "arn_pattern": "arn:*:ssm-sap:*:*:*/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
+        "component": {
+            "arn_pattern": "arn:*:ssm-sap:*:*:*/*/COMPONENT/*",
+            "condition_keys": "aws:ResourceTag/${TagKey}"
+        },
         "database": {
             "arn_pattern": "arn:*:ssm-sap:*:*:*/*/DB/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         }
     },
     "ssmmessages": {},
     "sso": {
```

### Comparing `iam_actions-1.2.20230726/iam_actions/services.json` & `iam_actions-1.2.20230727/iam_actions/services.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9945314309622325%*

 * *Differences: {"'ce'": "{'Actions': {insert: [(27, 'GetSavingsPlanPurchaseRecommendationDetails')]}}",*

 * * "'entityresolution'": "OrderedDict([('Actions', ['CreateMatchingWorkflow', 'CreateSchemaMapping', "*

 * *                       "'DeleteMatchingWorkflow', 'DeleteSchemaMapping', 'GetMatchId', "*

 * *                       "'GetMatchingJob', 'GetMatchingWorkflow', 'GetSchemaMapping', "*

 * *                       "'ListMatchingJobs', 'ListMatchingWorkflows', 'ListSchemaMappings', "*

 * *                       "'ListTagsForResource', 'Start […]*

```diff
@@ -2348,14 +2348,15 @@
             "GetCostForecast",
             "GetDimensionValues",
             "GetPreferences",
             "GetReservationCoverage",
             "GetReservationPurchaseRecommendation",
             "GetReservationUtilization",
             "GetRightsizingRecommendation",
+            "GetSavingsPlanPurchaseRecommendationDetails",
             "GetSavingsPlansCoverage",
             "GetSavingsPlansPurchaseRecommendation",
             "GetSavingsPlansUtilization",
             "GetSavingsPlansUtilizationDetails",
             "GetTags",
             "GetUsageForecast",
             "ListCostAllocationTags",
@@ -8097,14 +8098,49 @@
             "aws:TagKeys"
         ],
         "HasResource": true,
         "ServiceNames": [
             "Amazon EMR Serverless"
         ]
     },
+    "entityresolution": {
+        "ARNFormats": [
+            "arn:aws:entityresolution:${Region}:${Account}:${ResourceType}/${ResourceName}"
+        ],
+        "ARNRegexes": [
+            "^arn:aws:entityresolution:.+:.+:.+"
+        ],
+        "Actions": [
+            "CreateMatchingWorkflow",
+            "CreateSchemaMapping",
+            "DeleteMatchingWorkflow",
+            "DeleteSchemaMapping",
+            "GetMatchId",
+            "GetMatchingJob",
+            "GetMatchingWorkflow",
+            "GetSchemaMapping",
+            "ListMatchingJobs",
+            "ListMatchingWorkflows",
+            "ListSchemaMappings",
+            "ListTagsForResource",
+            "StartMatchingJob",
+            "TagResource",
+            "UntagResource",
+            "UpdateMatchingWorkflow"
+        ],
+        "ConditionKeys": [
+            "aws:RequestTag/${TagKey}",
+            "aws:ResourceTag/${TagKey}",
+            "aws:TagKeys"
+        ],
+        "HasResource": true,
+        "ServiceNames": [
+            "AWS Entity Resolution"
+        ]
+    },
     "es": {
         "ARNFormats": [
             "arn:aws:es:${Region}:${Account}:${Resource}"
         ],
         "ARNRegexes": [
             "^arn:aws:es:.+"
         ],
@@ -11540,14 +11576,15 @@
         ],
         "ARNRegexes": [
             "^arn:aws:ivs:.+:.+:.+"
         ],
         "Actions": [
             "BatchGetChannel",
             "BatchGetStreamKey",
+            "BatchStartViewerSessionRevocation",
             "CreateChannel",
             "CreateParticipantToken",
             "CreateRecordingConfiguration",
             "CreateStage",
             "CreateStreamKey",
             "DeleteChannel",
             "DeletePlaybackKeyPair",
@@ -11573,14 +11610,15 @@
             "ListStageSessions",
             "ListStages",
             "ListStreamKeys",
             "ListStreamSessions",
             "ListStreams",
             "ListTagsForResource",
             "PutMetadata",
+            "StartViewerSessionRevocation",
             "StopStream",
             "TagResource",
             "UntagResource",
             "UpdateChannel",
             "UpdateStage"
         ],
         "ConditionKeys": [
@@ -12418,16 +12456,21 @@
             "ListBotVersions",
             "ListBots",
             "ListBuiltInIntents",
             "ListBuiltInSlotTypes",
             "ListCustomVocabularyItems",
             "ListExports",
             "ListImports",
+            "ListIntentMetrics",
+            "ListIntentPaths",
+            "ListIntentStageMetrics",
             "ListIntents",
             "ListRecommendedIntents",
+            "ListSessionAnalyticsData",
+            "ListSessionMetrics",
             "ListSlotTypes",
             "ListSlots",
             "ListTagsForResource",
             "ListTestExecutionResultItems",
             "ListTestExecutions",
             "ListTestSetRecords",
             "ListTestSets",
@@ -13195,14 +13238,16 @@
             "GET",
             "GetAccessor",
             "GetMember",
             "GetNetwork",
             "GetNode",
             "GetProposal",
             "Invoke",
+            "InvokeRpcBitcoinMainnet",
+            "InvokeRpcBitcoinTestnet",
             "ListAccessors",
             "ListInvitations",
             "ListMembers",
             "ListNetworks",
             "ListNodes",
             "ListProposalVotes",
             "ListProposals",
@@ -13221,14 +13266,35 @@
             "aws:TagKeys"
         ],
         "HasResource": true,
         "ServiceNames": [
             "Amazon Managed Blockchain"
         ]
     },
+    "managedblockchain-query": {
+        "ARNFormats": [
+            "arn:${Partition}:managedblockchain-query:${Region}:${Account}:${ResourceType}/${ResourceName}"
+        ],
+        "ARNRegexes": [
+            "^arn:${Partition}:managedblockchain-query:.*:[0-9]*:.+"
+        ],
+        "Actions": [
+            "BatchGetTokenBalance",
+            "GetTokenBalance",
+            "GetTransaction",
+            "ListTokenBalances",
+            "ListTransactionEvents",
+            "ListTransactions"
+        ],
+        "ConditionKeys": [],
+        "HasResource": false,
+        "ServiceNames": [
+            "Amazon Managed Blockchain Query"
+        ]
+    },
     "marketplacecommerceanalytics": {
         "ARNFormats": [],
         "ARNRegexes": [],
         "Actions": [
             "GenerateDataSet",
             "StartSupportDataExport"
         ],
```

### Comparing `iam_actions-1.2.20230726/pyproject.toml` & `iam_actions-1.2.20230727/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20230726"
+version = "1.2.20230727"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20230726/setup.py` & `iam_actions-1.2.20230727/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20230726',
+    'version': '1.2.20230727',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20230726/PKG-INFO` & `iam_actions-1.2.20230727/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20230726
+Version: 1.2.20230727
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

