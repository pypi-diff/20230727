# Comparing `tmp/spice_agent-0.1.7.tar.gz` & `tmp/spice_agent-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spice_agent-0.1.7.tar", max compression
+gzip compressed data, was "spice_agent-0.1.8.tar", max compression
```

## Comparing `spice_agent-0.1.7.tar` & `spice_agent-0.1.8.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1921 2023-07-03 20:15:53.366214 spice_agent-0.1.7/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-03 20:15:53.366214 spice_agent-0.1.7/spice_agent/__init__.py
--rw-r--r--   0        0        0       22 2023-07-03 20:15:53.366214 spice_agent-0.1.7/spice_agent/__version__.py
--rw-r--r--   0        0        0        0 2023-07-03 20:15:53.366214 spice_agent-0.1.7/spice_agent/auth/__init__.py
--rw-r--r--   0        0        0     1024 2023-07-03 20:15:53.366214 spice_agent-0.1.7/spice_agent/auth/actions.py
--rw-r--r--   0        0        0     2761 2023-07-03 20:15:53.366214 spice_agent-0.1.7/spice_agent/auth/commands.py
--rw-r--r--   0        0        0     1869 2023-07-03 20:15:53.366214 spice_agent-0.1.7/spice_agent/cli.py
--rw-r--r--   0        0        0     5039 2023-07-03 20:15:53.366214 spice_agent-0.1.7/spice_agent/client.py
--rw-r--r--   0        0        0        0 2023-07-03 20:15:53.366214 spice_agent-0.1.7/spice_agent/daemons/__init__.py
--rw-r--r--   0        0        0     2500 2023-07-03 20:15:53.366214 spice_agent-0.1.7/spice_agent/daemons/actions.py
--rw-r--r--   0        0        0     1508 2023-07-03 20:15:53.366214 spice_agent-0.1.7/spice_agent/daemons/commands.py
--rw-r--r--   0        0        0     4302 2023-07-03 20:15:53.366214 spice_agent-0.1.7/spice_agent/daemons/launch_agents.py
--rw-r--r--   0        0        0     4982 2023-07-03 20:15:53.366214 spice_agent-0.1.7/spice_agent/daemons/launch_service.py
--rw-r--r--   0        0        0        0 2023-07-03 20:15:53.366214 spice_agent-0.1.7/spice_agent/graphql/__init__.py
--rw-r--r--   0        0        0        0 2023-07-03 20:15:53.366214 spice_agent-0.1.7/spice_agent/graphql/documents/__init__.py
--rw-r--r--   0        0        0     1196 2023-07-03 20:15:53.366214 spice_agent-0.1.7/spice_agent/graphql/documents/authentication.gql
--rw-r--r--   0        0        0     1504 2023-07-03 20:15:53.366214 spice_agent-0.1.7/spice_agent/graphql/sdk.py
--rw-r--r--   0        0        0        0 2023-07-03 20:15:53.366214 spice_agent-0.1.7/spice_agent/hardware/__init__.py
--rw-r--r--   0        0        0     7954 2023-07-03 20:15:53.366214 spice_agent-0.1.7/spice_agent/hardware/actions.py
--rw-r--r--   0        0        0     1070 2023-07-03 20:15:53.366214 spice_agent-0.1.7/spice_agent/hardware/commands.py
--rw-r--r--   0        0        0        0 2023-07-03 20:15:53.366214 spice_agent-0.1.7/spice_agent/inference/__init__.py
--rw-r--r--   0        0        0     6417 2023-07-03 20:15:53.366214 spice_agent-0.1.7/spice_agent/inference/actions.py
--rw-r--r--   0        0        0     1055 2023-07-03 20:15:53.366214 spice_agent-0.1.7/spice_agent/inference/commands.py
--rw-r--r--   0        0        0        0 2023-07-03 20:15:53.366214 spice_agent-0.1.7/spice_agent/tests/__init__.py
--rw-r--r--   0        0        0      555 2023-07-03 20:15:53.366214 spice_agent-0.1.7/spice_agent/tests/test_version.py
--rw-r--r--   0        0        0        0 2023-07-03 20:15:53.366214 spice_agent-0.1.7/spice_agent/training/__init__.py
--rw-r--r--   0        0        0    42091 2023-07-03 20:15:53.366214 spice_agent-0.1.7/spice_agent/training/actions.py
--rw-r--r--   0        0        0       97 2023-07-03 20:15:53.366214 spice_agent-0.1.7/spice_agent/training/commands.py
--rw-r--r--   0        0        0     7269 2023-07-03 20:15:53.366214 spice_agent-0.1.7/spice_agent/uploader/actions.py
--rw-r--r--   0        0        0     1907 2023-07-03 20:15:53.370214 spice_agent-0.1.7/spice_agent/utils/config.py
--rw-r--r--   0        0        0      252 2023-07-03 20:15:53.370214 spice_agent-0.1.7/spice_agent/utils/printer.py
--rw-r--r--   0        0        0        0 2023-07-03 20:15:53.370214 spice_agent-0.1.7/spice_agent/utils/updates.py
--rw-r--r--   0        0        0     1437 2023-07-03 20:15:53.370214 spice_agent-0.1.7/spice_agent/utils/version.py
--rw-r--r--   0        0        0        0 2023-07-03 20:15:53.370214 spice_agent-0.1.7/spice_agent/worker/__init__.py
--rw-r--r--   0        0        0     9500 2023-07-03 20:15:53.370214 spice_agent-0.1.7/spice_agent/worker/actions.py
--rw-r--r--   0        0        0      397 2023-07-03 20:15:53.370214 spice_agent-0.1.7/spice_agent/worker/commands.py
--rw-r--r--   0        0        0      950 1970-01-01 00:00:00.000000 spice_agent-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1921 2023-07-27 00:18:38.620121 spice_agent-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-27 00:18:38.620121 spice_agent-0.1.8/spice_agent/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-27 00:18:38.620121 spice_agent-0.1.8/spice_agent/__version__.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:18:38.620121 spice_agent-0.1.8/spice_agent/auth/__init__.py
+-rw-r--r--   0        0        0     1024 2023-07-27 00:18:38.620121 spice_agent-0.1.8/spice_agent/auth/actions.py
+-rw-r--r--   0        0        0     2976 2023-07-27 00:18:38.620121 spice_agent-0.1.8/spice_agent/auth/commands.py
+-rw-r--r--   0        0        0     1869 2023-07-27 00:18:38.620121 spice_agent-0.1.8/spice_agent/cli.py
+-rw-r--r--   0        0        0     5039 2023-07-27 00:18:38.620121 spice_agent-0.1.8/spice_agent/client.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:18:38.620121 spice_agent-0.1.8/spice_agent/daemons/__init__.py
+-rw-r--r--   0        0        0     2500 2023-07-27 00:18:38.620121 spice_agent-0.1.8/spice_agent/daemons/actions.py
+-rw-r--r--   0        0        0     1508 2023-07-27 00:18:38.620121 spice_agent-0.1.8/spice_agent/daemons/commands.py
+-rw-r--r--   0        0        0     4302 2023-07-27 00:18:38.620121 spice_agent-0.1.8/spice_agent/daemons/launch_agents.py
+-rw-r--r--   0        0        0     4982 2023-07-27 00:18:38.620121 spice_agent-0.1.8/spice_agent/daemons/launch_service.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:18:38.620121 spice_agent-0.1.8/spice_agent/graphql/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:18:38.620121 spice_agent-0.1.8/spice_agent/graphql/documents/__init__.py
+-rw-r--r--   0        0        0     1196 2023-07-27 00:18:38.620121 spice_agent-0.1.8/spice_agent/graphql/documents/authentication.gql
+-rw-r--r--   0        0        0     1504 2023-07-27 00:18:38.620121 spice_agent-0.1.8/spice_agent/graphql/sdk.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:18:38.620121 spice_agent-0.1.8/spice_agent/hardware/__init__.py
+-rw-r--r--   0        0        0     7954 2023-07-27 00:18:38.620121 spice_agent-0.1.8/spice_agent/hardware/actions.py
+-rw-r--r--   0        0        0     1070 2023-07-27 00:18:38.620121 spice_agent-0.1.8/spice_agent/hardware/commands.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:18:38.620121 spice_agent-0.1.8/spice_agent/inference/__init__.py
+-rw-r--r--   0        0        0     6884 2023-07-27 00:18:38.620121 spice_agent-0.1.8/spice_agent/inference/actions.py
+-rw-r--r--   0        0        0     1055 2023-07-27 00:18:38.620121 spice_agent-0.1.8/spice_agent/inference/commands.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:18:38.620121 spice_agent-0.1.8/spice_agent/tests/__init__.py
+-rw-r--r--   0        0        0      555 2023-07-27 00:18:38.620121 spice_agent-0.1.8/spice_agent/tests/test_version.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:18:38.620121 spice_agent-0.1.8/spice_agent/training/__init__.py
+-rw-r--r--   0        0        0    41859 2023-07-27 00:18:38.620121 spice_agent-0.1.8/spice_agent/training/actions.py
+-rw-r--r--   0        0        0       97 2023-07-27 00:18:38.624121 spice_agent-0.1.8/spice_agent/training/commands.py
+-rw-r--r--   0        0        0     7269 2023-07-27 00:18:38.624121 spice_agent-0.1.8/spice_agent/uploader/actions.py
+-rw-r--r--   0        0        0     1907 2023-07-27 00:18:38.624121 spice_agent-0.1.8/spice_agent/utils/config.py
+-rw-r--r--   0        0        0      252 2023-07-27 00:18:38.624121 spice_agent-0.1.8/spice_agent/utils/printer.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:18:38.624121 spice_agent-0.1.8/spice_agent/utils/updates.py
+-rw-r--r--   0        0        0     1788 2023-07-27 00:18:38.624121 spice_agent-0.1.8/spice_agent/utils/version.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:18:38.624121 spice_agent-0.1.8/spice_agent/worker/__init__.py
+-rw-r--r--   0        0        0     9500 2023-07-27 00:18:38.624121 spice_agent-0.1.8/spice_agent/worker/actions.py
+-rw-r--r--   0        0        0      397 2023-07-27 00:18:38.624121 spice_agent-0.1.8/spice_agent/worker/commands.py
+-rw-r--r--   0        0        0      950 1970-01-01 00:00:00.000000 spice_agent-0.1.8/PKG-INFO
```

### Comparing `spice_agent-0.1.7/pyproject.toml` & `spice_agent-0.1.8/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spice_agent"
-version = "0.1.7"
+version = "0.1.8"
 description = "spice agent"
 authors = ["Dylan Stein <dylan@spice.cloud>", "Ankush Patel <ankush@spice.cloud>"]
 license = ""
 
 [tool.poetry.dependencies]
 python = "^3.11.3"
 gql = "^3.4.1"
```

### Comparing `spice_agent-0.1.7/spice_agent/auth/actions.py` & `spice_agent-0.1.8/spice_agent/auth/actions.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.7/spice_agent/auth/commands.py` & `spice_agent-0.1.8/spice_agent/auth/commands.py`

 * *Files 7% similar despite different names*

```diff
@@ -41,15 +41,22 @@
 @click.option(
     "--transport",
     required=False,
     default="https",
     show_default="https",
     help="Transport protocol for Spice API",
 )
-def config_command(context, username: str, transport: str):
+@click.option(
+    "--register",
+    is_flag=True,
+    show_default=True,
+    default=False,
+    help="Auto Register Hardware with Spice Cloud",
+)
+def config_command(context, username: str, transport: str, register: bool):
     """Configure the CLI"""
     token = os.environ.get("SPICE_TOKEN", "")
     if not token and context.obj.get("YES"):
         raise click.ClickException(
             "SPICE_TOKEN environment variable is required for non-interactive mode"
         )
     host = context.obj.get("HOST", "api.spice.cloud")
@@ -68,24 +75,28 @@
         )
 
     auth = Auth(spice=None)
     auth.setup_config(username=username, token=token, host=host, transport=transport)
     message = f"Config created at '{SPICE_HOSTS_FILEPATH}' for user '{username}' on host '{host}'"  # noqa
     print_result(message=message, context=context, fg="green")
 
-    if click.confirm("Do you want to register this machine with spice.cloud?"):
+    if register or click.confirm(
+        "Do you want to register this machine with spice.cloud?"
+    ):
         spice = Spice(host=host)
         result = spice.hardware.register()
 
         if result.get("registerHardware"):
             print_result(
                 message="Hardware registered successfully", context=context, fg="green"
             )
 
-    if click.confirm("Do you want to install the agent as a background process?"):
+    if register or click.confirm(
+        "Do you want to install the agent as a background process?"
+    ):
         spice = Spice(host=host)
         spice.daemons.install()
         print_result(
             message="Daemon installed. View its logs with `spice daemon logs`",
             context=context,
             fg="green",
         )
```

### Comparing `spice_agent-0.1.7/spice_agent/cli.py` & `spice_agent-0.1.8/spice_agent/cli.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.7/spice_agent/client.py` & `spice_agent-0.1.8/spice_agent/client.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.7/spice_agent/daemons/actions.py` & `spice_agent-0.1.8/spice_agent/daemons/actions.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.7/spice_agent/daemons/commands.py` & `spice_agent-0.1.8/spice_agent/daemons/commands.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.7/spice_agent/daemons/launch_agents.py` & `spice_agent-0.1.8/spice_agent/daemons/launch_agents.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.7/spice_agent/daemons/launch_service.py` & `spice_agent-0.1.8/spice_agent/daemons/launch_service.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.7/spice_agent/graphql/documents/authentication.gql` & `spice_agent-0.1.8/spice_agent/graphql/documents/authentication.gql`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.7/spice_agent/graphql/sdk.py` & `spice_agent-0.1.8/spice_agent/graphql/sdk.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.7/spice_agent/hardware/actions.py` & `spice_agent-0.1.8/spice_agent/hardware/actions.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.7/spice_agent/hardware/commands.py` & `spice_agent-0.1.8/spice_agent/hardware/commands.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.7/spice_agent/inference/actions.py` & `spice_agent-0.1.8/spice_agent/inference/actions.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,14 +32,15 @@
             logging.getLogger("transformers.modeling_utils").setLevel(logging.ERROR)
             logging.getLogger("pika").setLevel(logging.ERROR)
 
     def _update_inference_job(
         self,
         inference_job_id: str,
         status: str,
+        was_guarded: Optional[bool] = None,
         text_output: Optional[str] = None,
         file_outputs_ids: list[str] = [],
     ):
         mutation = gql(
             """
             mutation updateInferenceJob($input: UpdateInferenceJobInput!) {
                 updateInferenceJob(input: $input) {
@@ -49,32 +50,34 @@
                         createdAt
                         updatedAt
                         completedAt
                         status
                         model {
                             name
                             slug
-                            hfModelRepoId
+                            repoId
                             isTextInput
                             isTextOutput
                             isFileInput
                             isFileOutput
                         }
                         textInput
                         textOutput
-
+                        wasGuarded
                     }
                 }
             }
             """
         )
 
         input: Dict[str, str | float | list[str]] = {"inferenceJobId": inference_job_id}
         if status is not None:
             input["status"] = status
+        if was_guarded is not None:
+            input["wasGuarded"] = was_guarded
         if text_output is not None:
             input["textOutput"] = text_output
         if file_outputs_ids is not None or len(file_outputs_ids) > 0:
             input["fileOutputsIds"] = file_outputs_ids
 
         variables = {"input": input}
 
@@ -107,62 +110,67 @@
             LOGGER.error(
                 f""" [*] Inference Job ID: {inference_job_id} not found.\
                                   Exiting early."""
             )
             return
 
         inference_job_id = result["updateInferenceJob"]["id"]
-        hf_model_repo_id = result["updateInferenceJob"]["model"]["hfModelRepoId"]
+        model_repo_id = result["updateInferenceJob"]["model"]["repoId"]
         text_input = result["updateInferenceJob"]["textInput"]
         is_text_input = result["updateInferenceJob"]["model"]["isTextInput"]
         is_text_output = result["updateInferenceJob"]["model"]["isTextOutput"]
         result["updateInferenceJob"]["model"]["isFileInput"]
         is_file_output = result["updateInferenceJob"]["model"]["isFileOutput"]
 
-        LOGGER.info(f""" [*] Model: {hf_model_repo_id}.""")
+        LOGGER.info(f""" [*] Model: {model_repo_id}.""")
         LOGGER.info(f""" [*] Text Input: '{text_input}'""")
 
         if torch.backends.mps.is_available():
             mps_empty_cache()
         if torch.cuda.is_available():
             torch.cuda.empty_cache()
 
         response = None
         try:
             if is_text_input and is_text_output:
                 result = None
-                pipe = pipeline(model=hf_model_repo_id, device=self.device)
+                pipe = pipeline(model=model_repo_id, device=self.device)
                 result = pipe(text_input)
 
                 response = self._update_inference_job(
                     inference_job_id=inference_job_id,
                     status="COMPLETE",
                     text_output=json.dumps(result),
                 )
             elif is_text_input and is_file_output:
                 SPICE_INFERENCE_DIRECTORY.mkdir(parents=True, exist_ok=True)
                 save_at = Path(SPICE_INFERENCE_DIRECTORY / f"{inference_job_id}.png")
+                was_guarded = False
                 if not save_at.exists():
                     pipe = StableDiffusionPipeline.from_pretrained(
-                        hf_model_repo_id, torch_dtype=torch.float32
+                        model_repo_id, torch_dtype=torch.float32
                     )
                     pipe = pipe.to(self.device)  # type: ignore
-                    result = pipe(text_input).images[0]  # type: ignore
+                    pipe_result = pipe(text_input, return_dict=True)  # type: ignore
+                    result = pipe_result.images[0]  # type: ignore
+                    if pipe_result.nsfw_content_detected:  # type: ignore
+                        was_guarded = pipe_result.nsfw_content_detected[0]  # type: ignore # noqa
                     result.save(save_at)
                 else:
                     LOGGER.info(f""" [*] File already exists at: {save_at}""")
 
                 upload_file_response = self.spice.uploader.upload_file_via_api(
                     path=save_at
                 )
                 file_id = upload_file_response.json()["data"]["uploadFile"]["id"]
                 response = self._update_inference_job(
                     inference_job_id=inference_job_id,
                     status="COMPLETE",
                     file_outputs_ids=file_id,
+                    was_guarded=was_guarded,
                 )
             LOGGER.info(f""" [*] COMPLETE. Result: " {result}""")
             return response
         except PipelineException as exception:
             message = f"""Input: "{input}" threw exception: {exception}"""
             LOGGER.error(message)
             self._update_inference_job(
```

### Comparing `spice_agent-0.1.7/spice_agent/inference/commands.py` & `spice_agent-0.1.8/spice_agent/inference/commands.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.7/spice_agent/tests/test_version.py` & `spice_agent-0.1.8/spice_agent/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.7/spice_agent/training/actions.py` & `spice_agent-0.1.8/spice_agent/training/actions.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,16 @@
     AutoModelForImageClassification,
     AutoModelForSequenceClassification,
     AutoTokenizer,
     Trainer,
     TrainingArguments,
 )
 
+from transformers.data import DefaultDataCollator
+
 from spice_agent.utils.config import (
     HF_HUB_DIRECTORY,
     SPICE_MODEL_CACHE_FILEPATH,
     SPICE_ROUND_VERIFICATION_FILEPATH,
     SPICE_TRAINING_FILEPATH,
     copy_directory,
     create_directory,
@@ -267,16 +269,15 @@
         return self.spice.session.execute(query, variable_values=variables)
 
     def _update_training_round(
         self,
         training_round_id: str,
         status: str,
         status_details: Optional[dict] = None,
-        round_accuracy: Optional[float] = None,
-        round_loss: Optional[float] = None,
+        metrics: Optional[dict] = None,
     ):
         mutation = gql(
             """
             mutation updateTrainingRound($input: UpdateTrainingRoundInput!) {
                 updateTrainingRound(input: $input) {
                     ... on TrainingRound {
                         id
@@ -297,18 +298,16 @@
             """  # noqa
         )
         input: Dict[str, str | float] = {"trainingRoundId": training_round_id}
         if status is not None:
             input["status"] = status
         if status_details:
             input["statusDetails"] = json.dumps(status_details)
-        if round_accuracy is not None:
-            input["roundAccuracy"] = round_accuracy
-        if round_loss is not None:
-            input["roundLoss"] = round_loss
+        if metrics:
+            input["metrics"] = json.dumps(metrics)
 
         variables = {"input": input}
         try:
             result = self.spice.session.execute(mutation, variable_values=variables)
         except TransportQueryError as exception:
             if exception.errors:
                 for error in exception.errors:
@@ -326,16 +325,15 @@
 
     def _update_training_round_step(
         self,
         training_round_step_id: str,
         status: str,
         status_details: Optional[dict] = None,
         file_id: Optional[str] = None,
-        step_accuracy: Optional[float] = None,
-        step_loss: Optional[float] = None,
+        metrics: Optional[dict] = None,
     ):
         mutation = gql(
             """
             mutation updateTrainingRoundStep($input: UpdateTrainingRoundStepInput!) {
                 updateTrainingRoundStep(input: $input) {
                     ... on TrainingRoundStep {
                         id
@@ -366,18 +364,16 @@
         input: Dict[str, str | float] = {"trainingRoundStepId": training_round_step_id}
         if status is not None:
             input["status"] = status
         if status_details:
             input["statusDetails"] = json.dumps(status_details)
         if file_id is not None:
             input["fileId"] = file_id
-        if step_accuracy is not None:
-            input["stepAccuracy"] = step_accuracy
-        if step_loss is not None:
-            input["stepLoss"] = step_loss
+        if metrics:
+            input["metrics"] = json.dumps(metrics)
 
         variables = {"input": input}
 
         try:
             result = self.spice.session.execute(mutation, variable_values=variables)
         except TransportQueryError as exception:
             if exception.errors:
@@ -771,14 +767,15 @@
         trainer = Trainer(
             model=model,
             args=training_args,
             train_dataset=tokenized_dataset,
             tokenizer=tokenizer,
             compute_metrics=compute_metrics,
             callbacks=[status_details_callback],
+            data_collator=DefaultDataCollator(),
         )
 
         self._update_training_round_step(
             training_round_step_id=training_round_step_id, status="TRAINING"
         )
 
         trainer.train()
@@ -859,14 +856,15 @@
         trainer = Trainer(
             model=model,
             args=eval_args,
             eval_dataset=tokenized_dataset,
             tokenizer=tokenizer,
             compute_metrics=compute_metrics,
             callbacks=[status_details_callback],
+            data_collator=DefaultDataCollator(),
         )
 
         self._update_training_round_step(
             training_round_step_id=training_round_step_id,
             status="TESTING",
         )
 
@@ -874,16 +872,15 @@
 
         trainer.log_metrics("eval", metrics)
         trainer.save_metrics("eval", metrics, combined=False)
 
         self._update_training_round_step(
             training_round_step_id=training_round_step_id,
             status="TESTING_COMPLETE",
-            step_accuracy=metrics["eval_accuracy"],
-            step_loss=metrics["eval_loss"],
+            metrics=metrics,
         )
 
         # clear the cache
         test_dataset.cleanup_cache_files()
 
     def _download_verify_model_file(self, url, destination_url, is_json=False):
         response = requests.get(url)
@@ -1060,14 +1057,15 @@
         trainer = Trainer(
             model=model,
             args=eval_args,
             eval_dataset=tokenized_dataset,
             tokenizer=tokenizer,
             compute_metrics=compute_metrics,
             callbacks=[status_details_callback],
+            data_collator=DefaultDataCollator(),
         )
 
         self._update_training_round(
             training_round_id=training_round_id,
             status="VERIFYING",
         )
         metrics = trainer.evaluate()
@@ -1098,13 +1096,12 @@
                 )
 
         print("Complete!")
 
         self._update_training_round(
             training_round_id=training_round_id,
             status="VERIFYING_COMPLETE",
-            round_accuracy=metrics["eval_accuracy"],
-            round_loss=metrics["eval_loss"],
+            metrics=metrics,
         )
 
         # clear the cache
         test_dataset.cleanup_cache_files()
```

### Comparing `spice_agent-0.1.7/spice_agent/uploader/actions.py` & `spice_agent-0.1.8/spice_agent/uploader/actions.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.7/spice_agent/utils/config.py` & `spice_agent-0.1.8/spice_agent/utils/config.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.7/spice_agent/utils/version.py` & `spice_agent-0.1.8/spice_agent/utils/version.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,19 +27,26 @@
     current_version = get_current_version()
     is_outdated, latest_version = get_is_outdated_and_get_latest_version(
         current_version=current_version
     )
     os_family = platform.system()
     if is_outdated:
         LOGGER.warn(
-            f"spice_agent version is at: {get_current_version()} latest is {latest_version}."  # noqa
+            f"spice_agent version is at: {get_current_version()}. Version {latest_version} is available."  # noqa
         )
-        # currently only supporting macOS
+        # currently only supporting macOS and WSL2
         if os_family == "Darwin":
-            LOGGER.warn("Attempting to update and restarting the spice daemon.")
+            LOGGER.warn("Attempting to update and restart the spice daemon.")
+            os.system("pip install --upgrade spice-agent")
+            daemons = Daemons(spice=None)
+            daemons.uninstall()
+            daemons.install()
+            sys.exit()
+        elif os_family == "Linux" and "WSL2" in platform.platform():
+            LOGGER.warn("Attempting to update and restart the spice daemon.")
             os.system("pip install --upgrade spice-agent")
             daemons = Daemons(spice=None)
             daemons.uninstall()
             daemons.install()
             sys.exit()
         else:
             LOGGER.warn(
```

### Comparing `spice_agent-0.1.7/spice_agent/worker/actions.py` & `spice_agent-0.1.8/spice_agent/worker/actions.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.7/PKG-INFO` & `spice_agent-0.1.8/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spice-agent
-Version: 0.1.7
+Version: 0.1.8
 Summary: spice agent
 Author: Dylan Stein
 Author-email: dylan@spice.cloud
 Requires-Python: >=3.11.3,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: accelerate (>=0.20.3,<0.21.0)
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
```

