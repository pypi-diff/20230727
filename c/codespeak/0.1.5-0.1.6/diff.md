# Comparing `tmp/codespeak-0.1.5.tar.gz` & `tmp/codespeak-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codespeak-0.1.5.tar", max compression
+gzip compressed data, was "codespeak-0.1.6.tar", max compression
```

## Comparing `codespeak-0.1.5.tar` & `codespeak-0.1.6.tar`

### file list

```diff
@@ -1,165 +1,170 @@
--rw-r--r--   0        0        0      185 2023-07-26 19:22:12.263946 codespeak-0.1.5/README.md
--rw-r--r--   0        0        0     6148 2023-06-13 18:29:30.684245 codespeak-0.1.5/codespeak/.DS_Store
--rw-r--r--   0        0        0      476 2023-07-26 18:49:48.846960 codespeak-0.1.5/codespeak/__init__.py
--rw-r--r--   0        0        0      401 2023-07-26 18:49:49.938737 codespeak-0.1.5/codespeak/apis/__pycache__/api_keys.cpython-310.pyc
--rw-r--r--   0        0        0      586 2023-07-26 15:21:30.889335 codespeak-0.1.5/codespeak/apis/__pycache__/api_metadata.cpython-310.pyc
--rw-r--r--   0        0        0      648 2023-07-25 20:01:11.732711 codespeak-0.1.5/codespeak/apis/__pycache__/authentication.cpython-310.pyc
--rw-r--r--   0        0        0      179 2023-07-26 18:49:48.847096 codespeak-0.1.5/codespeak/apis/api_keys.py
--rw-r--r--   0        0        0      239 2023-07-26 15:21:30.569084 codespeak-0.1.5/codespeak/apis/api_metadata.py
--rw-r--r--   0        0        0      149 2023-07-26 15:21:30.569541 codespeak-0.1.5/codespeak/constants.py
--rw-r--r--   0        0        0     1699 2023-07-26 16:35:37.600094 codespeak-0.1.5/codespeak/decorate/__pycache__/infer.cpython-310.pyc
--rw-r--r--   0        0        0     3545 2023-07-26 18:49:49.941971 codespeak-0.1.5/codespeak/decorate/__pycache__/writable.cpython-310.pyc
--rw-r--r--   0        0        0     2042 2023-07-26 15:21:30.891707 codespeak-0.1.5/codespeak/decorate/__pycache__/writable_transform.cpython-310.pyc
--rw-r--r--   0        0        0     3472 2023-07-26 18:49:48.847224 codespeak-0.1.5/codespeak/decorate/writable.py
--rw-r--r--   0        0        0     2236 2023-07-26 15:21:30.570234 codespeak-0.1.5/codespeak/decorate/writable_transform.py
--rw-r--r--   0        0        0     4165 2023-07-26 17:15:25.354823 codespeak-0.1.5/codespeak/frame.py
--rw-r--r--   0        0        0      336 2023-06-30 22:33:51.055730 codespeak-0.1.5/codespeak/frame_tests.py
--rw-r--r--   0        0        0       48 2023-07-26 18:49:48.847333 codespeak-0.1.5/codespeak/function/__init__.py
--rw-r--r--   0        0        0      212 2023-07-26 18:49:49.782512 codespeak-0.1.5/codespeak/function/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1848 2023-06-27 18:23:09.761841 codespeak-0.1.5/codespeak/function/__pycache__/_accessors.cpython-310.pyc
--rw-r--r--   0        0        0      419 2023-06-27 00:56:00.232756 codespeak-0.1.5/codespeak/function/__pycache__/_attributes.cpython-310.pyc
--rw-r--r--   0        0        0     1173 2023-06-27 16:25:51.638260 codespeak-0.1.5/codespeak/function/__pycache__/_body_resources.cpython-310.pyc
--rw-r--r--   0        0        0     2963 2023-06-27 16:26:07.363817 codespeak-0.1.5/codespeak/function/__pycache__/_infer.cpython-310.pyc
--rw-r--r--   0        0        0     2190 2023-06-27 14:51:47.078110 codespeak-0.1.5/codespeak/function/__pycache__/_inference.cpython-310.pyc
--rw-r--r--   0        0        0      396 2023-06-27 01:01:53.916633 codespeak-0.1.5/codespeak/function/__pycache__/_inference_attributes.cpython-310.pyc
--rw-r--r--   0        0        0     2787 2023-06-27 18:34:54.562917 codespeak-0.1.5/codespeak/function/__pycache__/_private_function.cpython-310.pyc
--rw-r--r--   0        0        0     1975 2023-06-27 16:25:51.611393 codespeak-0.1.5/codespeak/function/__pycache__/_resources.cpython-310.pyc
--rw-r--r--   0        0        0     1135 2023-06-27 00:56:00.233302 codespeak-0.1.5/codespeak/function/__pycache__/_tests.cpython-310.pyc
--rw-r--r--   0        0        0     1011 2023-06-28 00:30:35.155568 codespeak-0.1.5/codespeak/function/__pycache__/accessors.cpython-310.pyc
--rw-r--r--   0        0        0     7284 2023-07-26 18:49:48.781231 codespeak-0.1.5/codespeak/function/__pycache__/function.cpython-310.pyc
--rw-r--r--   0        0        0      458 2023-07-26 18:49:48.854876 codespeak-0.1.5/codespeak/function/__pycache__/function_attributes.cpython-310.pyc
--rw-r--r--   0        0        0     5839 2023-07-26 15:21:30.635904 codespeak-0.1.5/codespeak/function/__pycache__/function_declaration.cpython-310.pyc
--rw-r--r--   0        0        0     3307 2023-07-26 15:21:30.636336 codespeak-0.1.5/codespeak/function/__pycache__/function_declaration_lite.cpython-310.pyc
--rw-r--r--   0        0        0     1722 2023-07-26 18:49:48.821510 codespeak-0.1.5/codespeak/function/__pycache__/function_digest.cpython-310.pyc
--rw-r--r--   0        0        0     5062 2023-07-26 18:49:48.822412 codespeak-0.1.5/codespeak/function/__pycache__/function_file_service.cpython-310.pyc
--rw-r--r--   0        0        0     1315 2023-07-26 15:21:30.674873 codespeak-0.1.5/codespeak/function/__pycache__/function_lite.cpython-310.pyc
--rw-r--r--   0        0        0     1222 2023-07-26 17:06:04.061905 codespeak-0.1.5/codespeak/function/__pycache__/function_manager.cpython-310.pyc
--rw-r--r--   0        0        0      979 2023-07-26 18:49:48.822704 codespeak-0.1.5/codespeak/function/__pycache__/function_metadata.cpython-310.pyc
--rw-r--r--   0        0        0      615 2023-06-28 16:44:11.395312 codespeak-0.1.5/codespeak/function/__pycache__/function_tests.cpython-310.pyc
--rw-r--r--   0        0        0     6117 2023-06-27 15:12:29.776726 codespeak-0.1.5/codespeak/function/__pycache__/inference.cpython-310.pyc
--rw-r--r--   0        0        0      428 2023-06-27 01:01:53.916402 codespeak-0.1.5/codespeak/function/__pycache__/inference_attributes.cpython-310.pyc
--rw-r--r--   0        0        0      500 2023-06-27 14:51:47.076168 codespeak-0.1.5/codespeak/function/__pycache__/inference_make_response.cpython-310.pyc
--rw-r--r--   0        0        0     1229 2023-06-27 00:56:00.232576 codespeak-0.1.5/codespeak/function/__pycache__/inference_manager.cpython-310.pyc
--rw-r--r--   0        0        0     3334 2023-07-26 18:49:49.783352 codespeak-0.1.5/codespeak/function/__pycache__/writable_function.cpython-310.pyc
--rw-r--r--   0        0        0      159 2023-07-26 18:49:48.847455 codespeak-0.1.5/codespeak/function/function_attributes.py
--rw-r--r--   0        0        0     6796 2023-07-26 15:21:30.571241 codespeak-0.1.5/codespeak/function/function_declaration.py
--rw-r--r--   0        0        0     3264 2023-07-26 15:21:30.571476 codespeak-0.1.5/codespeak/function/function_declaration_lite.py
--rw-r--r--   0        0        0     1005 2023-07-26 15:21:30.571989 codespeak-0.1.5/codespeak/function/function_lite.py
--rw-r--r--   0        0        0      720 2023-07-26 17:05:57.339899 codespeak-0.1.5/codespeak/function/function_manager.py
--rw-r--r--   0        0        0      512 2023-07-04 22:16:19.066082 codespeak-0.1.5/codespeak/function/helper_types/__pycache__/make_inference_response.cpython-310.pyc
--rw-r--r--   0        0        0      150 2023-06-30 22:33:51.058155 codespeak-0.1.5/codespeak/function/helper_types/make_inference_response.py
--rw-r--r--   0        0        0     2491 2023-07-26 18:49:48.847573 codespeak-0.1.5/codespeak/function/writable_function.py
--rw-r--r--   0        0        0        0 2023-06-30 22:33:51.058230 codespeak-0.1.5/codespeak/helpers/__init__.py
--rw-r--r--   0        0        0      153 2023-07-04 22:16:18.811669 codespeak-0.1.5/codespeak/helpers/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      873 2023-06-19 15:37:02.638770 codespeak-0.1.5/codespeak/helpers/__pycache__/abspath_to_project_root.cpython-310.pyc
--rw-r--r--   0        0        0      823 2023-07-04 22:16:18.899018 codespeak-0.1.5/codespeak/helpers/__pycache__/auto_detect_abspath_to_project_root.cpython-310.pyc
--rw-r--r--   0        0        0     1179 2023-07-26 18:49:49.787761 codespeak-0.1.5/codespeak/helpers/__pycache__/derive_module_qualname_for_object.cpython-310.pyc
--rw-r--r--   0        0        0      547 2023-07-26 18:49:49.914049 codespeak-0.1.5/codespeak/helpers/__pycache__/extract_delimited_python_code_from_string.cpython-310.pyc
--rw-r--r--   0        0        0      961 2023-07-04 22:16:18.842565 codespeak-0.1.5/codespeak/helpers/__pycache__/gather_arguments.cpython-310.pyc
--rw-r--r--   0        0        0      574 2023-06-08 17:41:05.179013 codespeak-0.1.5/codespeak/helpers/__pycache__/get_attr_from_qualname.cpython-310.pyc
--rw-r--r--   0        0        0     1572 2023-07-26 15:21:30.882982 codespeak-0.1.5/codespeak/helpers/__pycache__/get_definitions_from_function_object.cpython-310.pyc
--rw-r--r--   0        0        0      904 2023-07-11 14:23:24.339756 codespeak-0.1.5/codespeak/helpers/__pycache__/get_definitions_from_function_signature.cpython-310.pyc
--rw-r--r--   0        0        0      697 2023-07-26 18:49:48.856265 codespeak-0.1.5/codespeak/helpers/__pycache__/guarantee_abspath_to_root_exists.cpython-310.pyc
--rw-r--r--   0        0        0      729 2023-07-04 22:16:18.841814 codespeak-0.1.5/codespeak/helpers/__pycache__/self_type.cpython-310.pyc
--rw-r--r--   0        0        0      606 2023-07-04 22:16:19.060692 codespeak-0.1.5/codespeak/helpers/__pycache__/set_attr_for_qualname.cpython-310.pyc
--rw-r--r--   0        0        0      904 2023-07-11 14:23:24.122135 codespeak-0.1.5/codespeak/helpers/__pycache__/try_get_self_class_object_for_function.cpython-310.pyc
--rw-r--r--   0        0        0     1119 2023-07-26 15:21:30.883396 codespeak-0.1.5/codespeak/helpers/__pycache__/try_get_self_definition_for_for_inferred_function.cpython-310.pyc
--rw-r--r--   0        0        0      747 2023-06-30 22:33:51.058561 codespeak-0.1.5/codespeak/helpers/auto_detect_abspath_to_project_root.py
--rw-r--r--   0        0        0     1422 2023-07-26 18:49:48.847729 codespeak-0.1.5/codespeak/helpers/derive_module_qualname_for_object.py
--rw-r--r--   0        0        0      287 2023-07-26 18:49:48.847833 codespeak-0.1.5/codespeak/helpers/extract_delimited_python_code_from_string.py
--rw-r--r--   0        0        0      503 2023-06-30 22:33:51.059260 codespeak-0.1.5/codespeak/helpers/gather_arguments.py
--rw-r--r--   0        0        0      363 2023-06-30 22:33:51.059370 codespeak-0.1.5/codespeak/helpers/get_attr_from_qualname.py
--rw-r--r--   0        0        0     1648 2023-07-26 15:21:30.572417 codespeak-0.1.5/codespeak/helpers/get_definitions_from_function_object.py
--rw-r--r--   0        0        0      461 2023-07-26 18:49:48.847991 codespeak-0.1.5/codespeak/helpers/guarantee_abspath_to_root_exists.py
--rw-r--r--   0        0        0      531 2023-06-30 22:33:51.060053 codespeak-0.1.5/codespeak/helpers/self_type.py
--rw-r--r--   0        0        0      388 2023-06-30 22:33:51.060156 codespeak-0.1.5/codespeak/helpers/set_attr_for_qualname.py
--rw-r--r--   0        0        0     1056 2023-07-26 15:21:30.572546 codespeak-0.1.5/codespeak/helpers/try_get_self_definition_for_for_inferred_function.py
--rw-r--r--   0        0        0      151 2023-06-22 13:35:46.342743 codespeak-0.1.5/codespeak/inference/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2526 2023-07-26 18:49:48.820937 codespeak-0.1.5/codespeak/inference/__pycache__/api_inference_engine.cpython-310.pyc
--rw-r--r--   0        0        0     5941 2023-06-27 14:49:54.099994 codespeak-0.1.5/codespeak/inference/__pycache__/code_generator.cpython-310.pyc
--rw-r--r--   0        0        0      971 2023-07-26 18:49:49.894428 codespeak-0.1.5/codespeak/inference/__pycache__/codespeak_service.cpython-310.pyc
--rw-r--r--   0        0        0     1275 2023-06-22 13:35:46.639822 codespeak-0.1.5/codespeak/inference/__pycache__/diff.cpython-310.pyc
--rw-r--r--   0        0        0     1969 2023-06-07 22:02:03.282201 codespeak-0.1.5/codespeak/inference/__pycache__/execute.cpython-310.pyc
--rw-r--r--   0        0        0     1513 2023-06-22 13:35:46.640291 codespeak-0.1.5/codespeak/inference/__pycache__/executor.cpython-310.pyc
--rw-r--r--   0        0        0     1191 2023-07-26 18:49:49.894062 codespeak-0.1.5/codespeak/inference/__pycache__/inference_engine.cpython-310.pyc
--rw-r--r--   0        0        0     4441 2023-07-26 15:21:30.709349 codespeak-0.1.5/codespeak/inference/__pycache__/openai_service.cpython-310.pyc
--rw-r--r--   0        0        0     3779 2023-07-26 15:21:30.708690 codespeak-0.1.5/codespeak/inference/__pycache__/prompt.cpython-310.pyc
--rw-r--r--   0        0        0     3384 2023-07-04 22:16:19.059946 codespeak-0.1.5/codespeak/inference/__pycache__/results_collector.cpython-310.pyc
--rw-r--r--   0        0        0     1641 2023-07-26 18:49:48.848149 codespeak-0.1.5/codespeak/inference/codespeak_service.py
--rw-r--r--   0        0        0     1155 2023-07-26 18:49:48.848295 codespeak-0.1.5/codespeak/inference/inference_engine.py
--rw-r--r--   0        0        0     1135 2023-07-26 15:21:30.879660 codespeak-0.1.5/codespeak/interactive_mode/__pycache__/get_approval.cpython-310.pyc
--rw-r--r--   0        0        0     1128 2023-07-26 15:21:30.573790 codespeak-0.1.5/codespeak/interactive_mode/get_approval.py
--rw-r--r--   0        0        0     1491 2023-06-30 22:33:51.061441 codespeak-0.1.5/codespeak/module_frame.py
--rw-r--r--   0        0        0     2401 2023-06-22 13:35:46.325670 codespeak-0.1.5/codespeak/public/__pycache__/codespeak_settings.cpython-310.pyc
--rw-r--r--   0        0        0      497 2023-07-26 15:21:30.884645 codespeak-0.1.5/codespeak/public/__pycache__/dot_get.cpython-310.pyc
--rw-r--r--   0        0        0      438 2023-06-22 13:35:46.643896 codespeak-0.1.5/codespeak/public/__pycache__/example_return.cpython-310.pyc
--rw-r--r--   0        0        0      976 2023-06-22 13:35:46.632956 codespeak-0.1.5/codespeak/public/__pycache__/generated_exception.cpython-310.pyc
--rw-r--r--   0        0        0     1445 2023-07-26 15:21:30.638835 codespeak-0.1.5/codespeak/public/__pycache__/inferred_exception.cpython-310.pyc
--rw-r--r--   0        0        0     3004 2023-07-26 15:21:30.883919 codespeak-0.1.5/codespeak/public/__pycache__/settings.cpython-310.pyc
--rw-r--r--   0        0        0      402 2023-07-26 15:21:30.574023 codespeak-0.1.5/codespeak/public/dot_get.py
--rw-r--r--   0        0        0     1165 2023-07-26 15:21:30.574259 codespeak-0.1.5/codespeak/public/inferred_exception.py
--rw-r--r--   0        0        0      509 2023-07-21 16:32:22.048104 codespeak-0.1.5/codespeak/public/rest_requests/__pycache__/api_keys.cpython-310.pyc
--rw-r--r--   0        0        0     1943 2023-07-26 15:21:30.983132 codespeak-0.1.5/codespeak/public/rest_requests/__pycache__/delete.cpython-310.pyc
--rw-r--r--   0        0        0     1702 2023-07-26 15:21:30.885194 codespeak-0.1.5/codespeak/public/rest_requests/__pycache__/get.cpython-310.pyc
--rw-r--r--   0        0        0     1937 2023-07-26 15:21:30.982216 codespeak-0.1.5/codespeak/public/rest_requests/__pycache__/post.cpython-310.pyc
--rw-r--r--   0        0        0     1934 2023-07-26 15:21:30.982797 codespeak-0.1.5/codespeak/public/rest_requests/__pycache__/put.cpython-310.pyc
--rw-r--r--   0        0        0     2183 2023-07-26 18:49:49.939455 codespeak-0.1.5/codespeak/public/rest_requests/__pycache__/request.cpython-310.pyc
--rw-r--r--   0        0        0     1915 2023-07-26 15:21:30.574379 codespeak-0.1.5/codespeak/public/rest_requests/delete.py
--rw-r--r--   0        0        0     1583 2023-07-26 15:21:30.574562 codespeak-0.1.5/codespeak/public/rest_requests/get.py
--rw-r--r--   0        0        0     1909 2023-07-26 15:21:30.574673 codespeak-0.1.5/codespeak/public/rest_requests/post.py
--rw-r--r--   0        0        0     1906 2023-07-26 15:21:30.574782 codespeak-0.1.5/codespeak/public/rest_requests/put.py
--rw-r--r--   0        0        0     1590 2023-07-26 18:49:48.848456 codespeak-0.1.5/codespeak/public/rest_requests/request.py
--rw-r--r--   0        0        0        0 2023-07-26 15:21:30.575010 codespeak-0.1.5/codespeak/public/rest_requests/rest_request_helpers.py
--rw-r--r--   0        0        0     2768 2023-06-20 14:04:07.183711 codespeak-0.1.5/codespeak/settings/__pycache__/_config.cpython-310.pyc
--rw-r--r--   0        0        0     3633 2023-07-26 18:49:48.789039 codespeak-0.1.5/codespeak/settings/__pycache__/_settings.cpython-310.pyc
--rw-r--r--   0        0        0     2393 2023-06-20 14:04:07.146395 codespeak-0.1.5/codespeak/settings/__pycache__/codespeak_config.cpython-310.pyc
--rw-r--r--   0        0        0      384 2023-07-04 22:16:18.813684 codespeak-0.1.5/codespeak/settings/__pycache__/environment.cpython-310.pyc
--rw-r--r--   0        0        0     3139 2023-07-26 18:49:48.857231 codespeak-0.1.5/codespeak/settings/__pycache__/settings.cpython-310.pyc
--rw-r--r--   0        0        0       83 2023-06-30 22:33:51.062147 codespeak-0.1.5/codespeak/settings/environment.py
--rw-r--r--   0        0        0     2265 2023-07-26 18:49:48.848560 codespeak-0.1.5/codespeak/settings/settings.py
--rw-r--r--   0        0        0      478 2023-06-30 22:33:51.062356 codespeak-0.1.5/codespeak/test_function.py
--rw-r--r--   0        0        0      157 2023-06-28 16:28:25.484531 codespeak-0.1.5/codespeak/type_definitions/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     4469 2023-07-26 15:21:30.639920 codespeak-0.1.5/codespeak/type_definitions/__pycache__/classify.cpython-310.pyc
--rw-r--r--   0        0        0     2199 2023-06-28 19:12:58.004518 codespeak-0.1.5/codespeak/type_definitions/__pycache__/definition.cpython-310.pyc
--rw-r--r--   0        0        0      953 2023-07-04 22:16:18.806739 codespeak-0.1.5/codespeak/type_definitions/__pycache__/free_modules.cpython-310.pyc
--rw-r--r--   0        0        0     1728 2023-07-26 15:21:30.673831 codespeak-0.1.5/codespeak/type_definitions/__pycache__/import_definition.cpython-310.pyc
--rw-r--r--   0        0        0     3194 2023-07-26 15:21:30.640813 codespeak-0.1.5/codespeak/type_definitions/__pycache__/type_definition.cpython-310.pyc
--rw-r--r--   0        0        0     5090 2023-07-26 15:21:30.575781 codespeak-0.1.5/codespeak/type_definitions/classify.py
--rw-r--r--   0        0        0     1046 2023-06-30 22:33:51.062658 codespeak-0.1.5/codespeak/type_definitions/free_modules.py
--rw-r--r--   0        0        0     1153 2023-07-26 15:21:30.576001 codespeak-0.1.5/codespeak/type_definitions/import_definition.py
--rw-r--r--   0        0        0     1869 2023-07-26 15:21:30.576138 codespeak-0.1.5/codespeak/type_definitions/type_definition.py
--rw-r--r--   0        0        0     1011 2023-07-04 22:16:18.815621 codespeak-0.1.5/codespeak/type_definitions/types/__pycache__/builtin.cpython-310.pyc
--rw-r--r--   0        0        0      882 2023-05-24 06:03:30.312106 codespeak-0.1.5/codespeak/type_definitions/types/__pycache__/builtin_type.cpython-310.pyc
--rw-r--r--   0        0        0     1352 2023-05-25 15:06:18.589725 codespeak-0.1.5/codespeak/type_definitions/types/__pycache__/complex_type_reference.cpython-310.pyc
--rw-r--r--   0        0        0     1378 2023-07-04 22:16:18.809085 codespeak-0.1.5/codespeak/type_definitions/types/__pycache__/custom_type_reference.cpython-310.pyc
--rw-r--r--   0        0        0     1010 2023-07-04 22:16:18.817459 codespeak-0.1.5/codespeak/type_definitions/types/__pycache__/generic.cpython-310.pyc
--rw-r--r--   0        0        0      926 2023-05-24 06:03:30.309943 codespeak-0.1.5/codespeak/type_definitions/types/__pycache__/generic_type.cpython-310.pyc
--rw-r--r--   0        0        0     1168 2023-07-04 22:16:18.814948 codespeak-0.1.5/codespeak/type_definitions/types/__pycache__/installed_class.cpython-310.pyc
--rw-r--r--   0        0        0      911 2023-05-24 06:03:30.311581 codespeak-0.1.5/codespeak/type_definitions/types/__pycache__/installed_class_type.cpython-310.pyc
--rw-r--r--   0        0        0     2714 2023-07-26 15:21:30.641713 codespeak-0.1.5/codespeak/type_definitions/types/__pycache__/local_class.cpython-310.pyc
--rw-r--r--   0        0        0     1938 2023-07-04 22:16:18.810536 codespeak-0.1.5/codespeak/type_definitions/types/__pycache__/local_class_as_self.cpython-310.pyc
--rw-r--r--   0        0        0     1330 2023-05-25 03:39:01.380879 codespeak-0.1.5/codespeak/type_definitions/types/__pycache__/local_class_reference.cpython-310.pyc
--rw-r--r--   0        0        0     1972 2023-05-24 06:03:30.310852 codespeak-0.1.5/codespeak/type_definitions/types/__pycache__/local_class_type.cpython-310.pyc
--rw-r--r--   0        0        0     1150 2023-07-04 22:16:18.816292 codespeak-0.1.5/codespeak/type_definitions/types/__pycache__/none.cpython-310.pyc
--rw-r--r--   0        0        0      605 2023-05-24 19:10:20.402432 codespeak-0.1.5/codespeak/type_definitions/types/__pycache__/prompt_annotation.cpython-310.pyc
--rw-r--r--   0        0        0     2373 2023-07-04 22:16:18.817114 codespeak-0.1.5/codespeak/type_definitions/types/__pycache__/typing_type.cpython-310.pyc
--rw-r--r--   0        0        0     1151 2023-07-04 22:16:18.819100 codespeak-0.1.5/codespeak/type_definitions/types/__pycache__/union_type.cpython-310.pyc
--rw-r--r--   0        0        0      509 2023-06-30 22:33:51.062975 codespeak-0.1.5/codespeak/type_definitions/types/builtin.py
--rw-r--r--   0        0        0      689 2023-06-30 22:33:51.063195 codespeak-0.1.5/codespeak/type_definitions/types/custom_type_reference.py
--rw-r--r--   0        0        0      515 2023-06-30 22:33:51.063329 codespeak-0.1.5/codespeak/type_definitions/types/generic.py
--rw-r--r--   0        0        0      666 2023-06-30 22:33:51.063462 codespeak-0.1.5/codespeak/type_definitions/types/installed_class.py
--rw-r--r--   0        0        0     2835 2023-07-26 15:21:30.576289 codespeak-0.1.5/codespeak/type_definitions/types/local_class.py
--rw-r--r--   0        0        0      494 2023-06-30 22:33:51.063899 codespeak-0.1.5/codespeak/type_definitions/types/none.py
--rw-r--r--   0        0        0     1929 2023-06-30 22:33:51.064042 codespeak-0.1.5/codespeak/type_definitions/types/typing_type.py
--rw-r--r--   0        0        0      657 2023-06-30 22:33:51.064165 codespeak-0.1.5/codespeak/type_definitions/types/union_type.py
--rw-r--r--   0        0        0      656 2023-06-28 16:28:25.490460 codespeak-0.1.5/codespeak/type_definitions/utils/__pycache__/dedupe.cpython-310.pyc
--rw-r--r--   0        0        0      800 2023-06-28 16:28:25.490752 codespeak-0.1.5/codespeak/type_definitions/utils/__pycache__/flat_uniques.cpython-310.pyc
--rw-r--r--   0        0        0      492 2023-06-28 16:28:25.491001 codespeak-0.1.5/codespeak/type_definitions/utils/__pycache__/flatten.cpython-310.pyc
--rw-r--r--   0        0        0      585 2023-06-28 16:28:25.542641 codespeak-0.1.5/codespeak/type_definitions/utils/__pycache__/group.cpython-310.pyc
--rw-r--r--   0        0        0      887 2023-05-24 21:59:04.045222 codespeak-0.1.5/codespeak/type_definitions/utils/__pycache__/ref_locals_in_place.cpython-310.pyc
--rw-r--r--   0        0        0      986 2023-05-25 14:58:45.016875 codespeak-0.1.5/codespeak/type_definitions/utils/__pycache__/swap_complex_types.cpython-310.pyc
--rw-r--r--   0        0        0      998 2023-07-04 22:16:18.818245 codespeak-0.1.5/codespeak/type_definitions/utils/__pycache__/swap_custom_types.cpython-310.pyc
--rw-r--r--   0        0        0      907 2023-05-25 14:43:06.205858 codespeak-0.1.5/codespeak/type_definitions/utils/__pycache__/swap_locals.cpython-310.pyc
--rw-r--r--   0        0        0     1162 2023-06-30 22:33:51.064306 codespeak-0.1.5/codespeak/type_definitions/utils/swap_custom_types.py
--rw-r--r--   0        0        0      448 2023-07-26 19:24:52.761418 codespeak-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      895 1970-01-01 00:00:00.000000 codespeak-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      236 2023-07-26 19:27:09.931537 codespeak-0.1.6/README.md
+-rw-r--r--   0        0        0     6148 2023-06-13 18:29:30.684245 codespeak-0.1.6/codespeak/.DS_Store
+-rw-r--r--   0        0        0      430 2023-07-27 20:05:59.706357 codespeak-0.1.6/codespeak/__init__.py
+-rw-r--r--   0        0        0      392 2023-07-27 19:38:03.903263 codespeak-0.1.6/codespeak/apis/__pycache__/api_keys.cpython-310.pyc
+-rw-r--r--   0        0        0      586 2023-07-26 15:21:30.889335 codespeak-0.1.6/codespeak/apis/__pycache__/api_metadata.cpython-310.pyc
+-rw-r--r--   0        0        0      648 2023-07-25 20:01:11.732711 codespeak-0.1.6/codespeak/apis/__pycache__/authentication.cpython-310.pyc
+-rw-r--r--   0        0        0      395 2023-07-27 20:03:53.416659 codespeak-0.1.6/codespeak/apis/__pycache__/get_api_key.cpython-310.pyc
+-rw-r--r--   0        0        0      239 2023-07-26 15:21:30.569084 codespeak-0.1.6/codespeak/apis/api_metadata.py
+-rw-r--r--   0        0        0      170 2023-07-27 20:00:52.893955 codespeak-0.1.6/codespeak/apis/get_api_key.py
+-rw-r--r--   0        0        0      149 2023-07-26 15:21:30.569541 codespeak-0.1.6/codespeak/constants.py
+-rw-r--r--   0        0        0     1699 2023-07-26 16:35:37.600094 codespeak-0.1.6/codespeak/decorate/__pycache__/infer.cpython-310.pyc
+-rw-r--r--   0        0        0     3455 2023-07-27 19:38:08.075659 codespeak-0.1.6/codespeak/decorate/__pycache__/writable.cpython-310.pyc
+-rw-r--r--   0        0        0     2042 2023-07-26 15:21:30.891707 codespeak-0.1.6/codespeak/decorate/__pycache__/writable_transform.cpython-310.pyc
+-rw-r--r--   0        0        0     3384 2023-07-27 19:38:07.383392 codespeak-0.1.6/codespeak/decorate/writable.py
+-rw-r--r--   0        0        0     4167 2023-07-27 18:18:22.973255 codespeak-0.1.6/codespeak/frame.py
+-rw-r--r--   0        0        0      336 2023-06-30 22:33:51.055730 codespeak-0.1.6/codespeak/frame_tests.py
+-rw-r--r--   0        0        0       48 2023-07-26 18:49:48.847333 codespeak-0.1.6/codespeak/function/__init__.py
+-rw-r--r--   0        0        0      212 2023-07-26 18:49:49.782512 codespeak-0.1.6/codespeak/function/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1848 2023-06-27 18:23:09.761841 codespeak-0.1.6/codespeak/function/__pycache__/_accessors.cpython-310.pyc
+-rw-r--r--   0        0        0      419 2023-06-27 00:56:00.232756 codespeak-0.1.6/codespeak/function/__pycache__/_attributes.cpython-310.pyc
+-rw-r--r--   0        0        0     1173 2023-06-27 16:25:51.638260 codespeak-0.1.6/codespeak/function/__pycache__/_body_resources.cpython-310.pyc
+-rw-r--r--   0        0        0     2963 2023-06-27 16:26:07.363817 codespeak-0.1.6/codespeak/function/__pycache__/_infer.cpython-310.pyc
+-rw-r--r--   0        0        0     2190 2023-06-27 14:51:47.078110 codespeak-0.1.6/codespeak/function/__pycache__/_inference.cpython-310.pyc
+-rw-r--r--   0        0        0      396 2023-06-27 01:01:53.916633 codespeak-0.1.6/codespeak/function/__pycache__/_inference_attributes.cpython-310.pyc
+-rw-r--r--   0        0        0     2787 2023-06-27 18:34:54.562917 codespeak-0.1.6/codespeak/function/__pycache__/_private_function.cpython-310.pyc
+-rw-r--r--   0        0        0     1975 2023-06-27 16:25:51.611393 codespeak-0.1.6/codespeak/function/__pycache__/_resources.cpython-310.pyc
+-rw-r--r--   0        0        0     1135 2023-06-27 00:56:00.233302 codespeak-0.1.6/codespeak/function/__pycache__/_tests.cpython-310.pyc
+-rw-r--r--   0        0        0     1011 2023-06-28 00:30:35.155568 codespeak-0.1.6/codespeak/function/__pycache__/accessors.cpython-310.pyc
+-rw-r--r--   0        0        0     7284 2023-07-26 18:49:48.781231 codespeak-0.1.6/codespeak/function/__pycache__/function.cpython-310.pyc
+-rw-r--r--   0        0        0      458 2023-07-26 18:49:48.854876 codespeak-0.1.6/codespeak/function/__pycache__/function_attributes.cpython-310.pyc
+-rw-r--r--   0        0        0     5839 2023-07-26 15:21:30.635904 codespeak-0.1.6/codespeak/function/__pycache__/function_declaration.cpython-310.pyc
+-rw-r--r--   0        0        0     3307 2023-07-26 15:21:30.636336 codespeak-0.1.6/codespeak/function/__pycache__/function_declaration_lite.cpython-310.pyc
+-rw-r--r--   0        0        0     1722 2023-07-26 18:49:48.821510 codespeak-0.1.6/codespeak/function/__pycache__/function_digest.cpython-310.pyc
+-rw-r--r--   0        0        0     5062 2023-07-26 18:49:48.822412 codespeak-0.1.6/codespeak/function/__pycache__/function_file_service.cpython-310.pyc
+-rw-r--r--   0        0        0     1315 2023-07-26 15:21:30.674873 codespeak-0.1.6/codespeak/function/__pycache__/function_lite.cpython-310.pyc
+-rw-r--r--   0        0        0     1222 2023-07-26 17:06:04.061905 codespeak-0.1.6/codespeak/function/__pycache__/function_manager.cpython-310.pyc
+-rw-r--r--   0        0        0      979 2023-07-26 18:49:48.822704 codespeak-0.1.6/codespeak/function/__pycache__/function_metadata.cpython-310.pyc
+-rw-r--r--   0        0        0      615 2023-06-28 16:44:11.395312 codespeak-0.1.6/codespeak/function/__pycache__/function_tests.cpython-310.pyc
+-rw-r--r--   0        0        0     6117 2023-06-27 15:12:29.776726 codespeak-0.1.6/codespeak/function/__pycache__/inference.cpython-310.pyc
+-rw-r--r--   0        0        0      428 2023-06-27 01:01:53.916402 codespeak-0.1.6/codespeak/function/__pycache__/inference_attributes.cpython-310.pyc
+-rw-r--r--   0        0        0      500 2023-06-27 14:51:47.076168 codespeak-0.1.6/codespeak/function/__pycache__/inference_make_response.cpython-310.pyc
+-rw-r--r--   0        0        0     1229 2023-06-27 00:56:00.232576 codespeak-0.1.6/codespeak/function/__pycache__/inference_manager.cpython-310.pyc
+-rw-r--r--   0        0        0     3011 2023-07-27 17:42:17.198341 codespeak-0.1.6/codespeak/function/__pycache__/replace_function.cpython-310.pyc
+-rw-r--r--   0        0        0     3012 2023-07-27 17:39:01.642563 codespeak-0.1.6/codespeak/function/__pycache__/replace_function_.cpython-310.pyc
+-rw-r--r--   0        0        0     3422 2023-07-27 19:38:19.272264 codespeak-0.1.6/codespeak/function/__pycache__/writable_function.cpython-310.pyc
+-rw-r--r--   0        0        0      159 2023-07-26 18:49:48.847455 codespeak-0.1.6/codespeak/function/function_attributes.py
+-rw-r--r--   0        0        0     6796 2023-07-26 15:21:30.571241 codespeak-0.1.6/codespeak/function/function_declaration.py
+-rw-r--r--   0        0        0     3264 2023-07-26 15:21:30.571476 codespeak-0.1.6/codespeak/function/function_declaration_lite.py
+-rw-r--r--   0        0        0     1005 2023-07-26 15:21:30.571989 codespeak-0.1.6/codespeak/function/function_lite.py
+-rw-r--r--   0        0        0      720 2023-07-26 17:05:57.339899 codespeak-0.1.6/codespeak/function/function_manager.py
+-rw-r--r--   0        0        0      512 2023-07-04 22:16:19.066082 codespeak-0.1.6/codespeak/function/helper_types/__pycache__/make_inference_response.cpython-310.pyc
+-rw-r--r--   0        0        0      150 2023-06-30 22:33:51.058155 codespeak-0.1.6/codespeak/function/helper_types/make_inference_response.py
+-rw-r--r--   0        0        0     2630 2023-07-27 19:38:18.746571 codespeak-0.1.6/codespeak/function/writable_function.py
+-rw-r--r--   0        0        0        0 2023-06-30 22:33:51.058230 codespeak-0.1.6/codespeak/helpers/__init__.py
+-rw-r--r--   0        0        0      153 2023-07-04 22:16:18.811669 codespeak-0.1.6/codespeak/helpers/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      873 2023-06-19 15:37:02.638770 codespeak-0.1.6/codespeak/helpers/__pycache__/abspath_to_project_root.cpython-310.pyc
+-rw-r--r--   0        0        0      318 2023-07-26 19:42:12.142010 codespeak-0.1.6/codespeak/helpers/__pycache__/align.cpython-310.pyc
+-rw-r--r--   0        0        0      823 2023-07-04 22:16:18.899018 codespeak-0.1.6/codespeak/helpers/__pycache__/auto_detect_abspath_to_project_root.cpython-310.pyc
+-rw-r--r--   0        0        0     1161 2023-07-27 19:37:30.727852 codespeak-0.1.6/codespeak/helpers/__pycache__/derive_module_qualname_for_object.cpython-310.pyc
+-rw-r--r--   0        0        0      547 2023-07-26 18:49:49.914049 codespeak-0.1.6/codespeak/helpers/__pycache__/extract_delimited_python_code_from_string.cpython-310.pyc
+-rw-r--r--   0        0        0      961 2023-07-04 22:16:18.842565 codespeak-0.1.6/codespeak/helpers/__pycache__/gather_arguments.cpython-310.pyc
+-rw-r--r--   0        0        0      574 2023-06-08 17:41:05.179013 codespeak-0.1.6/codespeak/helpers/__pycache__/get_attr_from_qualname.cpython-310.pyc
+-rw-r--r--   0        0        0     1572 2023-07-26 15:21:30.882982 codespeak-0.1.6/codespeak/helpers/__pycache__/get_definitions_from_function_object.cpython-310.pyc
+-rw-r--r--   0        0        0      904 2023-07-11 14:23:24.339756 codespeak-0.1.6/codespeak/helpers/__pycache__/get_definitions_from_function_signature.cpython-310.pyc
+-rw-r--r--   0        0        0      642 2023-07-27 19:37:52.494037 codespeak-0.1.6/codespeak/helpers/__pycache__/guarantee_abspath_to_root_exists.cpython-310.pyc
+-rw-r--r--   0        0        0      729 2023-07-04 22:16:18.841814 codespeak-0.1.6/codespeak/helpers/__pycache__/self_type.cpython-310.pyc
+-rw-r--r--   0        0        0      606 2023-07-04 22:16:19.060692 codespeak-0.1.6/codespeak/helpers/__pycache__/set_attr_for_qualname.cpython-310.pyc
+-rw-r--r--   0        0        0      904 2023-07-11 14:23:24.122135 codespeak-0.1.6/codespeak/helpers/__pycache__/try_get_self_class_object_for_function.cpython-310.pyc
+-rw-r--r--   0        0        0     1119 2023-07-26 15:21:30.883396 codespeak-0.1.6/codespeak/helpers/__pycache__/try_get_self_definition_for_for_inferred_function.cpython-310.pyc
+-rw-r--r--   0        0        0       79 2023-07-26 19:40:03.372389 codespeak-0.1.6/codespeak/helpers/align.py
+-rw-r--r--   0        0        0      747 2023-06-30 22:33:51.058561 codespeak-0.1.6/codespeak/helpers/auto_detect_abspath_to_project_root.py
+-rw-r--r--   0        0        0     1409 2023-07-27 19:37:30.560128 codespeak-0.1.6/codespeak/helpers/derive_module_qualname_for_object.py
+-rw-r--r--   0        0        0      287 2023-07-26 18:49:48.847833 codespeak-0.1.6/codespeak/helpers/extract_delimited_python_code_from_string.py
+-rw-r--r--   0        0        0      503 2023-06-30 22:33:51.059260 codespeak-0.1.6/codespeak/helpers/gather_arguments.py
+-rw-r--r--   0        0        0      363 2023-06-30 22:33:51.059370 codespeak-0.1.6/codespeak/helpers/get_attr_from_qualname.py
+-rw-r--r--   0        0        0     1648 2023-07-26 15:21:30.572417 codespeak-0.1.6/codespeak/helpers/get_definitions_from_function_object.py
+-rw-r--r--   0        0        0      439 2023-07-27 19:37:51.344629 codespeak-0.1.6/codespeak/helpers/guarantee_abspath_to_root_exists.py
+-rw-r--r--   0        0        0      531 2023-06-30 22:33:51.060053 codespeak-0.1.6/codespeak/helpers/self_type.py
+-rw-r--r--   0        0        0      388 2023-06-30 22:33:51.060156 codespeak-0.1.6/codespeak/helpers/set_attr_for_qualname.py
+-rw-r--r--   0        0        0     1056 2023-07-26 15:21:30.572546 codespeak-0.1.6/codespeak/helpers/try_get_self_definition_for_for_inferred_function.py
+-rw-r--r--   0        0        0      151 2023-06-22 13:35:46.342743 codespeak-0.1.6/codespeak/inference/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2526 2023-07-26 18:49:48.820937 codespeak-0.1.6/codespeak/inference/__pycache__/api_inference_engine.cpython-310.pyc
+-rw-r--r--   0        0        0     5941 2023-06-27 14:49:54.099994 codespeak-0.1.6/codespeak/inference/__pycache__/code_generator.cpython-310.pyc
+-rw-r--r--   0        0        0     1242 2023-07-27 20:07:41.634142 codespeak-0.1.6/codespeak/inference/__pycache__/codespeak_service.cpython-310.pyc
+-rw-r--r--   0        0        0     1275 2023-06-22 13:35:46.639822 codespeak-0.1.6/codespeak/inference/__pycache__/diff.cpython-310.pyc
+-rw-r--r--   0        0        0     1969 2023-06-07 22:02:03.282201 codespeak-0.1.6/codespeak/inference/__pycache__/execute.cpython-310.pyc
+-rw-r--r--   0        0        0     1513 2023-06-22 13:35:46.640291 codespeak-0.1.6/codespeak/inference/__pycache__/executor.cpython-310.pyc
+-rw-r--r--   0        0        0     2223 2023-07-27 18:15:59.477012 codespeak-0.1.6/codespeak/inference/__pycache__/inference_engine.cpython-310.pyc
+-rw-r--r--   0        0        0      480 2023-07-27 18:07:59.723899 codespeak-0.1.6/codespeak/inference/__pycache__/make_inference_response.cpython-310.pyc
+-rw-r--r--   0        0        0     4441 2023-07-26 15:21:30.709349 codespeak-0.1.6/codespeak/inference/__pycache__/openai_service.cpython-310.pyc
+-rw-r--r--   0        0        0     3779 2023-07-26 15:21:30.708690 codespeak-0.1.6/codespeak/inference/__pycache__/prompt.cpython-310.pyc
+-rw-r--r--   0        0        0     3012 2023-07-27 17:54:03.557745 codespeak-0.1.6/codespeak/inference/__pycache__/replace_function.cpython-310.pyc
+-rw-r--r--   0        0        0     3384 2023-07-04 22:16:19.059946 codespeak-0.1.6/codespeak/inference/__pycache__/results_collector.cpython-310.pyc
+-rw-r--r--   0        0        0     6184 2023-07-27 18:12:46.613129 codespeak-0.1.6/codespeak/inference/__pycache__/transform_inference.cpython-310.pyc
+-rw-r--r--   0        0        0      972 2023-07-27 20:07:40.983221 codespeak-0.1.6/codespeak/inference/codespeak_service.py
+-rw-r--r--   0        0        0     2212 2023-07-27 18:15:59.076020 codespeak-0.1.6/codespeak/inference/inference_engine.py
+-rw-r--r--   0        0        0      131 2023-07-27 18:07:52.689625 codespeak-0.1.6/codespeak/inference/make_inference_response.py
+-rw-r--r--   0        0        0     3506 2023-07-27 17:38:58.825842 codespeak-0.1.6/codespeak/inference/replace_function.py
+-rw-r--r--   0        0        0     4823 2023-07-27 17:56:36.040358 codespeak-0.1.6/codespeak/inference/test_transform.py
+-rw-r--r--   0        0        0     7672 2023-07-27 18:08:11.520050 codespeak-0.1.6/codespeak/inference/transform_inference.py
+-rw-r--r--   0        0        0     1135 2023-07-26 15:21:30.879660 codespeak-0.1.6/codespeak/interactive_mode/__pycache__/get_approval.cpython-310.pyc
+-rw-r--r--   0        0        0     1128 2023-07-26 15:21:30.573790 codespeak-0.1.6/codespeak/interactive_mode/get_approval.py
+-rw-r--r--   0        0        0     1491 2023-06-30 22:33:51.061441 codespeak-0.1.6/codespeak/module_frame.py
+-rw-r--r--   0        0        0     2401 2023-06-22 13:35:46.325670 codespeak-0.1.6/codespeak/public/__pycache__/codespeak_settings.cpython-310.pyc
+-rw-r--r--   0        0        0      497 2023-07-26 15:21:30.884645 codespeak-0.1.6/codespeak/public/__pycache__/dot_get.cpython-310.pyc
+-rw-r--r--   0        0        0      438 2023-06-22 13:35:46.643896 codespeak-0.1.6/codespeak/public/__pycache__/example_return.cpython-310.pyc
+-rw-r--r--   0        0        0      976 2023-06-22 13:35:46.632956 codespeak-0.1.6/codespeak/public/__pycache__/generated_exception.cpython-310.pyc
+-rw-r--r--   0        0        0     1445 2023-07-26 15:21:30.638835 codespeak-0.1.6/codespeak/public/__pycache__/inferred_exception.cpython-310.pyc
+-rw-r--r--   0        0        0     3004 2023-07-26 15:21:30.883919 codespeak-0.1.6/codespeak/public/__pycache__/settings.cpython-310.pyc
+-rw-r--r--   0        0        0      402 2023-07-26 15:21:30.574023 codespeak-0.1.6/codespeak/public/dot_get.py
+-rw-r--r--   0        0        0     1165 2023-07-26 15:21:30.574259 codespeak-0.1.6/codespeak/public/inferred_exception.py
+-rw-r--r--   0        0        0      509 2023-07-21 16:32:22.048104 codespeak-0.1.6/codespeak/public/rest_requests/__pycache__/api_keys.cpython-310.pyc
+-rw-r--r--   0        0        0     1943 2023-07-26 15:21:30.983132 codespeak-0.1.6/codespeak/public/rest_requests/__pycache__/delete.cpython-310.pyc
+-rw-r--r--   0        0        0     1705 2023-07-27 20:03:53.399499 codespeak-0.1.6/codespeak/public/rest_requests/__pycache__/get.cpython-310.pyc
+-rw-r--r--   0        0        0     1937 2023-07-26 15:21:30.982216 codespeak-0.1.6/codespeak/public/rest_requests/__pycache__/post.cpython-310.pyc
+-rw-r--r--   0        0        0     1934 2023-07-26 15:21:30.982797 codespeak-0.1.6/codespeak/public/rest_requests/__pycache__/put.cpython-310.pyc
+-rw-r--r--   0        0        0     2174 2023-07-27 19:38:19.409910 codespeak-0.1.6/codespeak/public/rest_requests/__pycache__/request.cpython-310.pyc
+-rw-r--r--   0        0        0     1915 2023-07-26 15:21:30.574379 codespeak-0.1.6/codespeak/public/rest_requests/delete.py
+-rw-r--r--   0        0        0     1586 2023-07-27 20:00:48.545702 codespeak-0.1.6/codespeak/public/rest_requests/get.py
+-rw-r--r--   0        0        0     1909 2023-07-26 15:21:30.574673 codespeak-0.1.6/codespeak/public/rest_requests/post.py
+-rw-r--r--   0        0        0     1906 2023-07-26 15:21:30.574782 codespeak-0.1.6/codespeak/public/rest_requests/put.py
+-rw-r--r--   0        0        0     1581 2023-07-27 19:38:18.738805 codespeak-0.1.6/codespeak/public/rest_requests/request.py
+-rw-r--r--   0        0        0        0 2023-07-26 15:21:30.575010 codespeak-0.1.6/codespeak/public/rest_requests/rest_request_helpers.py
+-rw-r--r--   0        0        0     1850 2023-07-27 20:03:52.974676 codespeak-0.1.6/codespeak/settings.py
+-rw-r--r--   0        0        0      478 2023-06-30 22:33:51.062356 codespeak-0.1.6/codespeak/test_function.py
+-rw-r--r--   0        0        0      157 2023-06-28 16:28:25.484531 codespeak-0.1.6/codespeak/type_definitions/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     4469 2023-07-26 15:21:30.639920 codespeak-0.1.6/codespeak/type_definitions/__pycache__/classify.cpython-310.pyc
+-rw-r--r--   0        0        0     2199 2023-06-28 19:12:58.004518 codespeak-0.1.6/codespeak/type_definitions/__pycache__/definition.cpython-310.pyc
+-rw-r--r--   0        0        0      953 2023-07-04 22:16:18.806739 codespeak-0.1.6/codespeak/type_definitions/__pycache__/free_modules.cpython-310.pyc
+-rw-r--r--   0        0        0     1728 2023-07-26 15:21:30.673831 codespeak-0.1.6/codespeak/type_definitions/__pycache__/import_definition.cpython-310.pyc
+-rw-r--r--   0        0        0     3194 2023-07-26 15:21:30.640813 codespeak-0.1.6/codespeak/type_definitions/__pycache__/type_definition.cpython-310.pyc
+-rw-r--r--   0        0        0     5090 2023-07-26 15:21:30.575781 codespeak-0.1.6/codespeak/type_definitions/classify.py
+-rw-r--r--   0        0        0     1046 2023-06-30 22:33:51.062658 codespeak-0.1.6/codespeak/type_definitions/free_modules.py
+-rw-r--r--   0        0        0     1153 2023-07-26 15:21:30.576001 codespeak-0.1.6/codespeak/type_definitions/import_definition.py
+-rw-r--r--   0        0        0     1869 2023-07-26 15:21:30.576138 codespeak-0.1.6/codespeak/type_definitions/type_definition.py
+-rw-r--r--   0        0        0     1011 2023-07-04 22:16:18.815621 codespeak-0.1.6/codespeak/type_definitions/types/__pycache__/builtin.cpython-310.pyc
+-rw-r--r--   0        0        0      882 2023-05-24 06:03:30.312106 codespeak-0.1.6/codespeak/type_definitions/types/__pycache__/builtin_type.cpython-310.pyc
+-rw-r--r--   0        0        0     1352 2023-05-25 15:06:18.589725 codespeak-0.1.6/codespeak/type_definitions/types/__pycache__/complex_type_reference.cpython-310.pyc
+-rw-r--r--   0        0        0     1378 2023-07-04 22:16:18.809085 codespeak-0.1.6/codespeak/type_definitions/types/__pycache__/custom_type_reference.cpython-310.pyc
+-rw-r--r--   0        0        0     1010 2023-07-04 22:16:18.817459 codespeak-0.1.6/codespeak/type_definitions/types/__pycache__/generic.cpython-310.pyc
+-rw-r--r--   0        0        0      926 2023-05-24 06:03:30.309943 codespeak-0.1.6/codespeak/type_definitions/types/__pycache__/generic_type.cpython-310.pyc
+-rw-r--r--   0        0        0     1168 2023-07-04 22:16:18.814948 codespeak-0.1.6/codespeak/type_definitions/types/__pycache__/installed_class.cpython-310.pyc
+-rw-r--r--   0        0        0      911 2023-05-24 06:03:30.311581 codespeak-0.1.6/codespeak/type_definitions/types/__pycache__/installed_class_type.cpython-310.pyc
+-rw-r--r--   0        0        0     2714 2023-07-26 15:21:30.641713 codespeak-0.1.6/codespeak/type_definitions/types/__pycache__/local_class.cpython-310.pyc
+-rw-r--r--   0        0        0     1938 2023-07-04 22:16:18.810536 codespeak-0.1.6/codespeak/type_definitions/types/__pycache__/local_class_as_self.cpython-310.pyc
+-rw-r--r--   0        0        0     1330 2023-05-25 03:39:01.380879 codespeak-0.1.6/codespeak/type_definitions/types/__pycache__/local_class_reference.cpython-310.pyc
+-rw-r--r--   0        0        0     1972 2023-05-24 06:03:30.310852 codespeak-0.1.6/codespeak/type_definitions/types/__pycache__/local_class_type.cpython-310.pyc
+-rw-r--r--   0        0        0     1150 2023-07-04 22:16:18.816292 codespeak-0.1.6/codespeak/type_definitions/types/__pycache__/none.cpython-310.pyc
+-rw-r--r--   0        0        0      605 2023-05-24 19:10:20.402432 codespeak-0.1.6/codespeak/type_definitions/types/__pycache__/prompt_annotation.cpython-310.pyc
+-rw-r--r--   0        0        0     2373 2023-07-04 22:16:18.817114 codespeak-0.1.6/codespeak/type_definitions/types/__pycache__/typing_type.cpython-310.pyc
+-rw-r--r--   0        0        0     1151 2023-07-04 22:16:18.819100 codespeak-0.1.6/codespeak/type_definitions/types/__pycache__/union_type.cpython-310.pyc
+-rw-r--r--   0        0        0      509 2023-06-30 22:33:51.062975 codespeak-0.1.6/codespeak/type_definitions/types/builtin.py
+-rw-r--r--   0        0        0      689 2023-06-30 22:33:51.063195 codespeak-0.1.6/codespeak/type_definitions/types/custom_type_reference.py
+-rw-r--r--   0        0        0      515 2023-06-30 22:33:51.063329 codespeak-0.1.6/codespeak/type_definitions/types/generic.py
+-rw-r--r--   0        0        0      666 2023-06-30 22:33:51.063462 codespeak-0.1.6/codespeak/type_definitions/types/installed_class.py
+-rw-r--r--   0        0        0     2835 2023-07-26 15:21:30.576289 codespeak-0.1.6/codespeak/type_definitions/types/local_class.py
+-rw-r--r--   0        0        0      494 2023-06-30 22:33:51.063899 codespeak-0.1.6/codespeak/type_definitions/types/none.py
+-rw-r--r--   0        0        0     1929 2023-06-30 22:33:51.064042 codespeak-0.1.6/codespeak/type_definitions/types/typing_type.py
+-rw-r--r--   0        0        0      657 2023-06-30 22:33:51.064165 codespeak-0.1.6/codespeak/type_definitions/types/union_type.py
+-rw-r--r--   0        0        0      656 2023-06-28 16:28:25.490460 codespeak-0.1.6/codespeak/type_definitions/utils/__pycache__/dedupe.cpython-310.pyc
+-rw-r--r--   0        0        0      800 2023-06-28 16:28:25.490752 codespeak-0.1.6/codespeak/type_definitions/utils/__pycache__/flat_uniques.cpython-310.pyc
+-rw-r--r--   0        0        0      492 2023-06-28 16:28:25.491001 codespeak-0.1.6/codespeak/type_definitions/utils/__pycache__/flatten.cpython-310.pyc
+-rw-r--r--   0        0        0      585 2023-06-28 16:28:25.542641 codespeak-0.1.6/codespeak/type_definitions/utils/__pycache__/group.cpython-310.pyc
+-rw-r--r--   0        0        0      887 2023-05-24 21:59:04.045222 codespeak-0.1.6/codespeak/type_definitions/utils/__pycache__/ref_locals_in_place.cpython-310.pyc
+-rw-r--r--   0        0        0      986 2023-05-25 14:58:45.016875 codespeak-0.1.6/codespeak/type_definitions/utils/__pycache__/swap_complex_types.cpython-310.pyc
+-rw-r--r--   0        0        0      998 2023-07-04 22:16:18.818245 codespeak-0.1.6/codespeak/type_definitions/utils/__pycache__/swap_custom_types.cpython-310.pyc
+-rw-r--r--   0        0        0      907 2023-05-25 14:43:06.205858 codespeak-0.1.6/codespeak/type_definitions/utils/__pycache__/swap_locals.cpython-310.pyc
+-rw-r--r--   0        0        0     1162 2023-06-30 22:33:51.064306 codespeak-0.1.6/codespeak/type_definitions/utils/swap_custom_types.py
+-rw-r--r--   0        0        0      448 2023-07-27 20:21:09.014192 codespeak-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      946 1970-01-01 00:00:00.000000 codespeak-0.1.6/PKG-INFO
```

### Comparing `codespeak-0.1.5/codespeak/.DS_Store` & `codespeak-0.1.6/codespeak/.DS_Store`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/apis/__pycache__/api_metadata.cpython-310.pyc` & `codespeak-0.1.6/codespeak/apis/__pycache__/api_metadata.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/apis/__pycache__/authentication.cpython-310.pyc` & `codespeak-0.1.6/codespeak/apis/__pycache__/authentication.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/decorate/__pycache__/infer.cpython-310.pyc` & `codespeak-0.1.6/codespeak/decorate/__pycache__/infer.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/decorate/__pycache__/writable.cpython-310.pyc` & `codespeak-0.1.6/codespeak/decorate/__pycache__/writable.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Jul 26 18:49:48 2023 UTC, .py size: 3472 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,222 +1,216 @@
-00000000: 6f0d 0d0a 0000 0000 cc6a c164 900d 0000  o........j.d....
+00000000: 6f0d 0d0a 0000 0000 9fc7 c264 380d 0000  o..........d8...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 2c01 0000 6400  .....@...s,...d.
+00000020: 0004 0000 0040 0000 0073 2001 0000 6400  .....@...s ...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 6400 6403 6c03 6d04 5a04 6d05 5a05  Z.d.d.l.m.Z.m.Z.
 00000050: 6d06 5a06 6d07 5a07 6d08 5a08 6d09 5a09  m.Z.m.Z.m.Z.m.Z.
 00000060: 0100 6400 6401 6c00 6d01 5a01 0100 6400  ..d.d.l.m.Z...d.
 00000070: 6404 6c0a 6d0b 5a0b 0100 6400 6405 6c0c  d.l.m.Z...d.d.l.
 00000080: 6d0d 5a0d 0100 6400 6406 6c0e 6d0f 5a0f  m.Z...d.d.l.m.Z.
 00000090: 0100 6400 6407 6c10 6d11 5a11 0100 6400  ..d.d.l.m.Z...d.
 000000a0: 6408 6c12 6d13 5a13 0100 6400 6409 6c14  d.l.m.Z...d.d.l.
 000000b0: 6d15 5a15 0100 6400 640a 6c16 6d17 5a17  m.Z...d.d.l.m.Z.
-000000c0: 0100 6400 640b 6c18 6d19 5a19 0100 6400  ..d.d.l.m.Z...d.
-000000d0: 6407 6c1a 6d11 5a11 0100 640c 640d 8400  d.l.m.Z...d.d...
-000000e0: 5a1b 640e 6505 640f 651c 6604 6410 6411  Z.d.e.d.e.f.d.d.
-000000f0: 8404 5a1d 6400 6402 6c1e 5a1f 6400 6412  ..Z.d.d.l.Z.d.d.
-00000100: 6c1e 6d20 5a20 6d21 5a21 0100 6400 6413  l.m Z m!Z!..d.d.
-00000110: 6c22 6d23 5a23 6d24 5a24 6d25 5a25 0100  l"m#Z#m$Z$m%Z%..
-00000120: 4700 6414 6415 8400 6415 651f 6a26 8303  G.d.d...d.e.j&..
-00000130: 5a27 6416 6505 640f 6528 6604 6417 6418  Z'd.e.d.e(f.d.d.
-00000140: 8404 5a29 6419 6505 641a 6505 6604 641b  ..Z)d.e.d.e.f.d.
-00000150: 641c 8404 5a2a 6402 5300 291d e900 0000  d...Z*d.S.).....
-00000160: 0029 01da 0577 7261 7073 4e29 06da 0341  .)...wrapsN)...A
-00000170: 6e79 da08 4361 6c6c 6162 6c65 da04 4469  ny..Callable..Di
-00000180: 6374 da04 4c69 7374 da05 5475 706c 65da  ct..List..Tuple.
-00000190: 0754 7970 6556 6172 2901 da13 4675 6e63  .TypeVar)...Func
-000001a0: 7469 6f6e 4465 636c 6172 6174 696f 6e29  tionDeclaration)
-000001b0: 01da 1057 7269 7461 626c 6546 756e 6374  ...WritableFunct
-000001c0: 696f 6e29 01da 0873 6574 7469 6e67 7329  ion)...settings)
-000001d0: 01da 0b45 6e76 6972 6f6e 6d65 6e74 2901  ...Environment).
-000001e0: da12 4675 6e63 7469 6f6e 4174 7472 6962  ..FunctionAttrib
-000001f0: 7574 6573 2901 da0a 4672 616d 6554 6573  utes)...FrameTes
-00000200: 7473 2901 da05 4672 616d 6529 01da 2467  ts)...Frame)..$g
-00000210: 6574 5f64 6566 696e 6974 696f 6e73 5f66  et_definitions_f
-00000220: 726f 6d5f 6675 6e63 7469 6f6e 5f6f 626a  rom_function_obj
-00000230: 6563 7463 0100 0000 0000 0000 0000 0000  ectc............
-00000240: 0100 0000 0400 0000 0300 0000 7324 0000  ............s$..
-00000250: 0074 0088 0083 0187 0087 0166 0264 0164  .t.........f.d.d
-00000260: 0284 0883 0189 0174 0188 0188 0083 0201  .......t........
-00000270: 0088 0153 0029 034e 6300 0000 0000 0000  ...S.).Nc.......
-00000280: 0000 0000 0003 0000 0004 0000 001f 0000  ................
-00000290: 0073 3200 0000 8801 6a00 7212 7401 8800  .s2.....j.r.t...
-000002a0: 8301 7212 7402 8801 8301 7d02 7c02 a003  ..r.t.....}.|...
-000002b0: 7404 8800 8301 a101 5300 8800 7c00 6900  t.......S...|.i.
-000002c0: 7c01 a401 8e01 5300 a901 4e29 05da 075f  |.....S...N)..._
-000002d0: 6973 5f64 6576 da15 7368 6f75 6c64 5f77  is_dev..should_w
-000002e0: 7269 7465 5f66 756e 6374 696f 6e72 0a00  rite_functionr..
-000002f0: 0000 da06 5f77 7269 7465 da0f 6765 745f  ...._write..get_
-00000300: 736f 7572 6365 5f66 696c 6529 03da 0461  source_file)...a
-00000310: 7267 73da 066b 7761 7267 73da 1177 7269  rgs..kwargs..wri
-00000320: 7461 626c 655f 6675 6e63 7469 6f6e a902  table_function..
-00000330: da04 6675 6e63 da07 7772 6170 7065 72a9  ..func..wrapper.
-00000340: 00fa 3d2f 5573 6572 732f 6e61 7468 616e  ..=/Users/nathan
-00000350: 7368 6972 6c65 792f 636f 6465 7370 6561  shirley/codespea
-00000360: 6b2f 636f 6465 7370 6561 6b2f 6465 636f  k/codespeak/deco
-00000370: 7261 7465 2f77 7269 7461 626c 652e 7079  rate/writable.py
-00000380: 721b 0000 0015 0000 0073 0a00 0000 0602  r........s......
-00000390: 0801 0801 0e01 0e01 7a19 7772 6974 6162  ........z.writab
-000003a0: 6c65 2e3c 6c6f 6361 6c73 3e2e 7772 6170  le.<locals>.wrap
-000003b0: 7065 7229 0272 0200 0000 da23 5f61 7373  per).r.....#_ass
-000003c0: 6967 6e5f 6465 6661 756c 745f 6675 6e63  ign_default_func
-000003d0: 7469 6f6e 5f61 7474 7269 6275 7465 7329  tion_attributes)
-000003e0: 0172 1a00 0000 721c 0000 0072 1900 0000  .r....r....r....
-000003f0: 721d 0000 00da 0877 7269 7461 626c 6514  r......writable.
-00000400: 0000 0073 0800 0000 0601 1001 0a07 0402  ...s............
-00000410: 721f 0000 00da 0866 756e 6374 696f 6eda  r......function.
-00000420: 0672 6574 7572 6e63 0100 0000 0000 0000  .returnc........
-00000430: 0000 0000 0200 0000 0300 0000 4300 0000  ............C...
-00000440: 731e 0000 0074 00a0 017c 00a1 017d 017c  s....t...|...}.|
-00000450: 0164 0075 0072 0d74 0264 0183 0182 017c  .d.u.r.t.d.....|
-00000460: 0153 0029 024e 7a22 4675 6e63 7469 6f6e  .S.).Nz"Function
-00000470: 206d 7573 7420 6265 2064 6566 696e 6564   must be defined
-00000480: 2069 6e20 6120 6669 6c65 2903 da07 696e   in a file)...in
-00000490: 7370 6563 74da 0d67 6574 736f 7572 6365  spect..getsource
-000004a0: 6669 6c65 da0a 5661 6c75 6545 7272 6f72  file..ValueError
-000004b0: 2902 7220 0000 00da 0266 6672 1c00 0000  ).r .....ffr....
-000004c0: 721c 0000 0072 1d00 0000 7215 0000 0022  r....r....r...."
-000004d0: 0000 0073 0800 0000 0a01 0801 0801 0401  ...s............
-000004e0: 7215 0000 0029 02da 0d4d 6179 6265 5365  r....)...MaybeSe
-000004f0: 6e74 696e 656c da0f 5265 6d6f 7661 6c53  ntinel..RemovalS
-00000500: 656e 7469 6e65 6c29 03da 0950 726f 7669  entinel)...Provi
-00000510: 6465 7254 da19 4578 7072 6573 7369 6f6e  derT..Expression
-00000520: 436f 6e74 6578 7450 726f 7669 6465 72da  ContextProvider.
-00000530: 1145 7870 7265 7373 696f 6e43 6f6e 7465  .ExpressionConte
-00000540: 7874 6300 0000 0000 0000 0000 0000 0000  xtc.............
-00000550: 0000 0004 0000 0040 0000 0073 2a00 0000  .......@...s*...
-00000560: 6500 5a01 6400 5a02 6408 6403 6404 8404  e.Z.d.Z.d.d.d...
-00000570: 5a03 6405 6504 6a05 6401 6402 6604 6406  Z.d.e.j.d.d.f.d.
-00000580: 6407 8404 5a06 6402 5300 2909 da12 5368  d...Z.d.S.)...Sh
-00000590: 6f75 6c64 5772 6974 6556 6973 6974 6f72  ouldWriteVisitor
-000005a0: 7221 0000 004e 6301 0000 0000 0000 0000  r!...Nc.........
-000005b0: 0000 0001 0000 0002 0000 0043 0000 0073  ...........C...s
-000005c0: 0a00 0000 6401 7c00 5f00 6400 5300 2902  ....d.|._.d.S.).
-000005d0: 4e46 2901 da0c 7368 6f75 6c64 5f77 7269  NF)...should_wri
-000005e0: 7465 2901 da04 7365 6c66 721c 0000 0072  te)...selfr....r
-000005f0: 1c00 0000 721d 0000 00da 085f 5f69 6e69  ....r......__ini
-00000600: 745f 5f2f 0000 0073 0200 0000 0a01 7a1b  t__/...s......z.
-00000610: 5368 6f75 6c64 5772 6974 6556 6973 6974  ShouldWriteVisit
-00000620: 6f72 2e5f 5f69 6e69 745f 5fda 046e 6f64  or.__init__..nod
-00000630: 6563 0200 0000 0000 0000 0000 0000 0500  ec..............
-00000640: 0000 0300 0000 4300 0000 7386 0000 007c  ......C...s....|
-00000650: 016a 006a 007d 027c 016a 0164 0164 028d  .j.j.}.|.j.d.d..
-00000660: 017d 037c 0364 0075 0172 147c 0264 0364  .}.|.d.u.r.|.d.d
-00000670: 0085 0219 007d 0274 027c 0283 0164 036b  .....}.t.|...d.k
-00000680: 0272 3b74 037c 0264 0419 0074 046a 0583  .r;t.|.d...t.j..
-00000690: 0272 3d7c 0264 0419 007d 0474 027c 046a  .r=|.d...}.t.|.j
-000006a0: 0083 0164 036b 0272 3f74 037c 046a 0064  ...d.k.r?t.|.j.d
-000006b0: 0419 0074 046a 0683 0272 4164 017c 005f  ...t.j...rAd.|._
-000006c0: 0764 0053 0064 0053 0064 0053 0064 0053  .d.S.d.S.d.S.d.S
-000006d0: 0064 0053 0029 054e 5429 01da 0563 6c65  .d.S.).NT)...cle
-000006e0: 616e e901 0000 0072 0100 0000 2908 da04  an.....r....)...
-000006f0: 626f 6479 da0d 6765 745f 646f 6373 7472  body..get_docstr
-00000700: 696e 67da 036c 656e da0a 6973 696e 7374  ing..len..isinst
-00000710: 616e 6365 da03 6373 74da 1353 696d 706c  ance..cst..Simpl
-00000720: 6553 7461 7465 6d65 6e74 4c69 6e65 da04  eStatementLine..
-00000730: 5061 7373 722c 0000 0029 0572 2d00 0000  Passr,...).r-...
-00000740: 722f 0000 0072 3200 0000 da09 646f 6373  r/...r2.....docs
-00000750: 7472 696e 675a 0f66 6972 7374 5f73 7461  tringZ.first_sta
-00000760: 7465 6d65 6e74 721c 0000 0072 1c00 0000  tementr....r....
-00000770: 721d 0000 00da 1176 6973 6974 5f46 756e  r......visit_Fun
-00000780: 6374 696f 6e44 6566 3200 0000 7318 0000  ctionDef2...s...
-00000790: 0008 010c 0108 030c 011c 0308 0110 010c  ................
-000007a0: 0104 ff0a 0308 fb08 027a 2453 686f 756c  .........z$Shoul
-000007b0: 6457 7269 7465 5669 7369 746f 722e 7669  dWriteVisitor.vi
-000007c0: 7369 745f 4675 6e63 7469 6f6e 4465 6629  sit_FunctionDef)
-000007d0: 0272 2100 0000 4e29 07da 085f 5f6e 616d  .r!...N)...__nam
-000007e0: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
-000007f0: 0c5f 5f71 7561 6c6e 616d 655f 5f72 2e00  .__qualname__r..
-00000800: 0000 7236 0000 00da 0b46 756e 6374 696f  ..r6.....Functio
-00000810: 6e44 6566 723a 0000 0072 1c00 0000 721c  nDefr:...r....r.
-00000820: 0000 0072 1c00 0000 721d 0000 0072 2b00  ...r....r....r+.
-00000830: 0000 2e00 0000 7306 0000 0008 000a 0118  ......s.........
-00000840: 0372 2b00 0000 721a 0000 0063 0100 0000  .r+...r....c....
-00000850: 0000 0000 0000 0000 0400 0000 0300 0000  ................
-00000860: 4300 0000 732a 0000 0074 00a0 017c 00a1  C...s*...t...|..
-00000870: 017d 0174 02a0 037c 01a1 017d 0274 0483  .}.t...|...}.t..
-00000880: 007d 037c 02a0 057c 03a1 0101 007c 036a  .}.|...|.....|.j
-00000890: 0653 0072 1100 0000 2907 7222 0000 00da  .S.r....).r"....
-000008a0: 0967 6574 736f 7572 6365 7236 0000 00da  .getsourcer6....
-000008b0: 0c70 6172 7365 5f6d 6f64 756c 6572 2b00  .parse_moduler+.
-000008c0: 0000 da05 7669 7369 7472 2c00 0000 2904  ....visitr,...).
-000008d0: 721a 0000 00da 0673 6f75 7263 65da 066d  r......source..m
-000008e0: 6f64 756c 65da 0776 6973 6974 6f72 721c  odule..visitorr.
-000008f0: 0000 0072 1c00 0000 721d 0000 0072 1300  ...r....r....r..
-00000900: 0000 4300 0000 730a 0000 000a 010a 0106  ..C...s.........
-00000910: 010a 0106 0172 1300 0000 721b 0000 00da  .....r....r.....
-00000920: 0e64 6563 6f72 6174 6564 5f66 756e 6363  .decorated_funcc
-00000930: 0200 0000 0000 0000 0000 0000 0400 0000  ................
-00000940: 0a00 0000 4300 0000 738c 0000 0074 00a0  ....C...s....t..
-00000950: 01a1 007d 0274 027c 0074 036a 047c 0274  ...}.t.|.t.j.|.t
-00000960: 056a 066b 0383 0301 007c 0274 056a 076b  .j.k.....|.t.j.k
-00000970: 0272 4474 087c 0183 017d 0374 027c 0074  .rDt.|...}.t.|.t
-00000980: 036a 0974 0a6a 0b7c 017c 0364 0119 007c  .j.t.j.|.|.d...|
-00000990: 0364 0219 007c 0364 0319 007c 0364 0419  .d...|.d...|.d..
-000009a0: 0064 058d 0583 0301 0074 027c 0074 036a  .d.......t.|.t.j
-000009b0: 0c74 0d7c 0364 0119 0074 0e83 0074 0da0  .t.|.d...t...t..
-000009c0: 0f7c 016a 10a1 0167 0164 068d 0383 0301  .|.j...g.d......
-000009d0: 0064 0053 0064 0053 0029 074e da03 616c  .d.S.d.S.).N..al
-000009e0: 6c72 2d00 0000 da0b 7265 7475 726e 5f74  lr-.....return_t
-000009f0: 7970 65da 0670 6172 616d 7329 05da 0d69  ype..params)...i
-00000a00: 6e66 6572 7265 645f 6675 6e63 da14 616c  nferred_func..al
-00000a10: 6c5f 7479 7065 5f64 6566 696e 6974 696f  l_type_definitio
-00000a20: 6e73 da0f 7365 6c66 5f64 6566 696e 6974  ns..self_definit
-00000a30: 696f 6eda 1672 6574 7572 6e5f 7479 7065  ion..return_type
-00000a40: 5f64 6566 696e 6974 696f 6eda 1170 6172  _definition..par
-00000a50: 616d 5f64 6566 696e 6974 696f 6e73 2903  am_definitions).
-00000a60: da10 7479 7065 5f64 6566 696e 6974 696f  ..type_definitio
-00000a70: 6e73 da05 7465 7374 73da 0770 6172 656e  ns..tests..paren
-00000a80: 7473 2911 720b 0000 00da 0f67 6574 5f65  ts).r......get_e
-00000a90: 6e76 6972 6f6e 6d65 6e74 da07 7365 7461  nvironment..seta
-00000aa0: 7474 7272 0d00 0000 da06 6973 5f64 6576  ttrr......is_dev
-00000ab0: 720c 0000 00da 0450 524f 44da 0344 4556  r......PROD..DEV
-00000ac0: 7210 0000 00da 0b64 6563 6c61 7261 7469  r......declarati
-00000ad0: 6f6e 7209 0000 00da 1e66 726f 6d5f 696e  onr......from_in
-00000ae0: 6665 7272 6564 5f66 756e 635f 6465 636c  ferred_func_decl
-00000af0: 6172 6174 696f 6eda 0566 7261 6d65 720f  aration..framer.
-00000b00: 0000 0072 0e00 0000 da0a 666f 725f 6d6f  ...r......for_mo
-00000b10: 6475 6c65 723c 0000 0029 0472 1b00 0000  duler<...).r....
-00000b20: 7245 0000 00da 0365 6e76 5a14 6675 6e63  rE.....envZ.func
-00000b30: 7469 6f6e 5f64 6566 696e 6974 696f 6e73  tion_definitions
-00000b40: 721c 0000 0072 1c00 0000 721d 0000 0072  r....r....r....r
-00000b50: 1e00 0000 4b00 0000 7332 0000 0008 0114  ....K...s2......
-00000b60: 010a 0108 0102 0102 0104 0104 0102 0106  ................
-00000b70: 0106 0106 0106 0104 fb04 fd02 0b02 0104  ................
-00000b80: 0102 0106 0104 010c 0104 fd08 fd04 f372  ...............r
-00000b90: 1e00 0000 292b da09 6675 6e63 746f 6f6c  ....)+..functool
-00000ba0: 7372 0200 0000 7222 0000 00da 0674 7970  sr....r".....typ
-00000bb0: 696e 6772 0300 0000 7204 0000 0072 0500  ingr....r....r..
-00000bc0: 0000 7206 0000 0072 0700 0000 7208 0000  ..r....r....r...
-00000bd0: 00da 2763 6f64 6573 7065 616b 2e66 756e  ..'codespeak.fun
-00000be0: 6374 696f 6e2e 6675 6e63 7469 6f6e 5f64  ction.function_d
-00000bf0: 6563 6c61 7261 7469 6f6e 7209 0000 005a  eclarationr....Z
-00000c00: 2463 6f64 6573 7065 616b 2e66 756e 6374  $codespeak.funct
-00000c10: 696f 6e2e 7772 6974 6162 6c65 5f66 756e  ion.writable_fun
-00000c20: 6374 696f 6e72 0a00 0000 da12 636f 6465  ctionr......code
-00000c30: 7370 6561 6b2e 7365 7474 696e 6773 720b  speak.settingsr.
-00000c40: 0000 00da 1e63 6f64 6573 7065 616b 2e73  .....codespeak.s
-00000c50: 6574 7469 6e67 732e 656e 7669 726f 6e6d  ettings.environm
-00000c60: 656e 7472 0c00 0000 da26 636f 6465 7370  entr.....&codesp
-00000c70: 6561 6b2e 6675 6e63 7469 6f6e 2e66 756e  eak.function.fun
-00000c80: 6374 696f 6e5f 6174 7472 6962 7574 6573  ction_attributes
-00000c90: 720d 0000 00da 1563 6f64 6573 7065 616b  r......codespeak
-00000ca0: 2e66 7261 6d65 5f74 6573 7473 720e 0000  .frame_testsr...
-00000cb0: 00da 0f63 6f64 6573 7065 616b 2e66 7261  ...codespeak.fra
-00000cc0: 6d65 720f 0000 005a 3663 6f64 6573 7065  mer....Z6codespe
-00000cd0: 616b 2e68 656c 7065 7273 2e67 6574 5f64  ak.helpers.get_d
-00000ce0: 6566 696e 6974 696f 6e73 5f66 726f 6d5f  efinitions_from_
-00000cf0: 6675 6e63 7469 6f6e 5f6f 626a 6563 7472  function_objectr
-00000d00: 1000 0000 5a1b 636f 6465 7370 6561 6b2e  ....Z.codespeak.
-00000d10: 7365 7474 696e 6773 2e73 6574 7469 6e67  settings.setting
-00000d20: 7372 1f00 0000 da03 7374 7272 1500 0000  sr......strr....
-00000d30: da06 6c69 6263 7374 7236 0000 0072 2600  ..libcstr6...r&.
-00000d40: 0000 7227 0000 005a 0f6c 6962 6373 742e  ..r'...Z.libcst.
-00000d50: 6d65 7461 6461 7461 7228 0000 0072 2900  metadatar(...r).
-00000d60: 0000 722a 0000 00da 0a43 5354 5669 7369  ..r*.....CSTVisi
-00000d70: 746f 7272 2b00 0000 da04 626f 6f6c 7213  torr+.....boolr.
-00000d80: 0000 0072 1e00 0000 721c 0000 0072 1c00  ...r....r....r..
-00000d90: 0000 721c 0000 0072 1d00 0000 da08 3c6d  ..r....r......<m
-00000da0: 6f64 756c 653e 0100 0000 732a 0000 000c  odule>....s*....
-00000db0: 0008 0120 010c 010c 010c 030c 010c 010c  ... ............
-00000dc0: 010c 010c 010c 010c 0308 0312 0e08 0710  ................
-00000dd0: 0114 0112 0312 1516 08                   .........
+000000c0: 0100 6400 640b 6c0e 6d18 5a18 0100 640c  ..d.d.l.m.Z...d.
+000000d0: 640d 8400 5a19 640e 6505 640f 651a 6604  d...Z.d.e.d.e.f.
+000000e0: 6410 6411 8404 5a1b 6400 6402 6c1c 5a1d  d.d...Z.d.d.l.Z.
+000000f0: 6400 6412 6c1c 6d1e 5a1e 6d1f 5a1f 0100  d.d.l.m.Z.m.Z...
+00000100: 6400 6413 6c20 6d21 5a21 6d22 5a22 6d23  d.d.l m!Z!m"Z"m#
+00000110: 5a23 0100 4700 6414 6415 8400 6415 651d  Z#..G.d.d...d.e.
+00000120: 6a24 8303 5a25 6416 6505 640f 6526 6604  j$..Z%d.e.d.e&f.
+00000130: 6417 6418 8404 5a27 6419 6505 641a 6505  d.d...Z'd.e.d.e.
+00000140: 6604 641b 641c 8404 5a28 6402 5300 291d  f.d.d...Z(d.S.).
+00000150: e900 0000 0029 01da 0577 7261 7073 4e29  .....)...wrapsN)
+00000160: 06da 0341 6e79 da08 4361 6c6c 6162 6c65  ...Any..Callable
+00000170: da04 4469 6374 da04 4c69 7374 da05 5475  ..Dict..List..Tu
+00000180: 706c 65da 0754 7970 6556 6172 2901 da13  ple..TypeVar)...
+00000190: 4675 6e63 7469 6f6e 4465 636c 6172 6174  FunctionDeclarat
+000001a0: 696f 6e29 01da 1057 7269 7461 626c 6546  ion)...WritableF
+000001b0: 756e 6374 696f 6e29 01da 0873 6574 7469  unction)...setti
+000001c0: 6e67 7329 01da 1246 756e 6374 696f 6e41  ngs)...FunctionA
+000001d0: 7474 7269 6275 7465 7329 01da 0a46 7261  ttributes)...Fra
+000001e0: 6d65 5465 7374 7329 01da 0546 7261 6d65  meTests)...Frame
+000001f0: 2901 da24 6765 745f 6465 6669 6e69 7469  )..$get_definiti
+00000200: 6f6e 735f 6672 6f6d 5f66 756e 6374 696f  ons_from_functio
+00000210: 6e5f 6f62 6a65 6374 2901 da0b 456e 7669  n_object)...Envi
+00000220: 726f 6e6d 656e 7463 0100 0000 0000 0000  ronmentc........
+00000230: 0000 0000 0100 0000 0400 0000 0300 0000  ................
+00000240: 7324 0000 0074 0088 0083 0187 0087 0166  s$...t.........f
+00000250: 0264 0164 0284 0883 0189 0174 0188 0188  .d.d.......t....
+00000260: 0083 0201 0088 0153 0029 034e 6300 0000  .......S.).Nc...
+00000270: 0000 0000 0000 0000 0003 0000 0004 0000  ................
+00000280: 001f 0000 0073 3200 0000 8801 6a00 7212  .....s2.....j.r.
+00000290: 7401 8800 8301 7212 7402 8801 8301 7d02  t.....r.t.....}.
+000002a0: 7c02 a003 7404 8800 8301 a101 5300 8800  |...t.......S...
+000002b0: 7c00 6900 7c01 a401 8e01 5300 a901 4e29  |.i.|.....S...N)
+000002c0: 05da 075f 6973 5f64 6576 da15 7368 6f75  ..._is_dev..shou
+000002d0: 6c64 5f77 7269 7465 5f66 756e 6374 696f  ld_write_functio
+000002e0: 6e72 0a00 0000 da06 5f77 7269 7465 da0f  nr......_write..
+000002f0: 6765 745f 736f 7572 6365 5f66 696c 6529  get_source_file)
+00000300: 03da 0461 7267 73da 066b 7761 7267 73da  ...args..kwargs.
+00000310: 1177 7269 7461 626c 655f 6675 6e63 7469  .writable_functi
+00000320: 6f6e a902 da04 6675 6e63 da07 7772 6170  on....func..wrap
+00000330: 7065 72a9 00fa 3d2f 5573 6572 732f 6e61  per...=/Users/na
+00000340: 7468 616e 7368 6972 6c65 792f 636f 6465  thanshirley/code
+00000350: 7370 6561 6b2f 636f 6465 7370 6561 6b2f  speak/codespeak/
+00000360: 6465 636f 7261 7465 2f77 7269 7461 626c  decorate/writabl
+00000370: 652e 7079 721b 0000 0014 0000 0073 0a00  e.pyr........s..
+00000380: 0000 0602 0801 0801 0e01 0e01 7a19 7772  ............z.wr
+00000390: 6974 6162 6c65 2e3c 6c6f 6361 6c73 3e2e  itable.<locals>.
+000003a0: 7772 6170 7065 7229 0272 0200 0000 da23  wrapper).r.....#
+000003b0: 5f61 7373 6967 6e5f 6465 6661 756c 745f  _assign_default_
+000003c0: 6675 6e63 7469 6f6e 5f61 7474 7269 6275  function_attribu
+000003d0: 7465 7329 0172 1a00 0000 721c 0000 0072  tes).r....r....r
+000003e0: 1900 0000 721d 0000 00da 0877 7269 7461  ....r......writa
+000003f0: 626c 6513 0000 0073 0800 0000 0601 1001  ble....s........
+00000400: 0a07 0402 721f 0000 00da 0866 756e 6374  ....r......funct
+00000410: 696f 6eda 0672 6574 7572 6e63 0100 0000  ion..returnc....
+00000420: 0000 0000 0000 0000 0200 0000 0300 0000  ................
+00000430: 4300 0000 731e 0000 0074 00a0 017c 00a1  C...s....t...|..
+00000440: 017d 017c 0164 0075 0072 0d74 0264 0183  .}.|.d.u.r.t.d..
+00000450: 0182 017c 0153 0029 024e 7a22 4675 6e63  ...|.S.).Nz"Func
+00000460: 7469 6f6e 206d 7573 7420 6265 2064 6566  tion must be def
+00000470: 696e 6564 2069 6e20 6120 6669 6c65 2903  ined in a file).
+00000480: da07 696e 7370 6563 74da 0d67 6574 736f  ..inspect..getso
+00000490: 7572 6365 6669 6c65 da0a 5661 6c75 6545  urcefile..ValueE
+000004a0: 7272 6f72 2902 7220 0000 00da 0266 6672  rror).r .....ffr
+000004b0: 1c00 0000 721c 0000 0072 1d00 0000 7215  ....r....r....r.
+000004c0: 0000 0021 0000 0073 0800 0000 0a01 0801  ...!...s........
+000004d0: 0801 0401 7215 0000 0029 02da 0d4d 6179  ....r....)...May
+000004e0: 6265 5365 6e74 696e 656c da0f 5265 6d6f  beSentinel..Remo
+000004f0: 7661 6c53 656e 7469 6e65 6c29 03da 0950  valSentinel)...P
+00000500: 726f 7669 6465 7254 da19 4578 7072 6573  roviderT..Expres
+00000510: 7369 6f6e 436f 6e74 6578 7450 726f 7669  sionContextProvi
+00000520: 6465 72da 1145 7870 7265 7373 696f 6e43  der..ExpressionC
+00000530: 6f6e 7465 7874 6300 0000 0000 0000 0000  ontextc.........
+00000540: 0000 0000 0000 0004 0000 0040 0000 0073  ...........@...s
+00000550: 2a00 0000 6500 5a01 6400 5a02 6408 6403  *...e.Z.d.Z.d.d.
+00000560: 6404 8404 5a03 6405 6504 6a05 6401 6402  d...Z.d.e.j.d.d.
+00000570: 6604 6406 6407 8404 5a06 6402 5300 2909  f.d.d...Z.d.S.).
+00000580: da12 5368 6f75 6c64 5772 6974 6556 6973  ..ShouldWriteVis
+00000590: 6974 6f72 7221 0000 004e 6301 0000 0000  itorr!...Nc.....
+000005a0: 0000 0000 0000 0001 0000 0002 0000 0043  ...............C
+000005b0: 0000 0073 0a00 0000 6401 7c00 5f00 6400  ...s....d.|._.d.
+000005c0: 5300 2902 4e46 2901 da0c 7368 6f75 6c64  S.).NF)...should
+000005d0: 5f77 7269 7465 2901 da04 7365 6c66 721c  _write)...selfr.
+000005e0: 0000 0072 1c00 0000 721d 0000 00da 085f  ...r....r......_
+000005f0: 5f69 6e69 745f 5f2e 0000 0073 0200 0000  _init__....s....
+00000600: 0a01 7a1b 5368 6f75 6c64 5772 6974 6556  ..z.ShouldWriteV
+00000610: 6973 6974 6f72 2e5f 5f69 6e69 745f 5fda  isitor.__init__.
+00000620: 046e 6f64 6563 0200 0000 0000 0000 0000  .nodec..........
+00000630: 0000 0500 0000 0300 0000 4300 0000 7386  ..........C...s.
+00000640: 0000 007c 016a 006a 007d 027c 016a 0164  ...|.j.j.}.|.j.d
+00000650: 0164 028d 017d 037c 0364 0075 0172 147c  .d...}.|.d.u.r.|
+00000660: 0264 0364 0085 0219 007d 0274 027c 0283  .d.d.....}.t.|..
+00000670: 0164 036b 0272 3b74 037c 0264 0419 0074  .d.k.r;t.|.d...t
+00000680: 046a 0583 0272 3d7c 0264 0419 007d 0474  .j...r=|.d...}.t
+00000690: 027c 046a 0083 0164 036b 0272 3f74 037c  .|.j...d.k.r?t.|
+000006a0: 046a 0064 0419 0074 046a 0683 0272 4164  .j.d...t.j...rAd
+000006b0: 017c 005f 0764 0053 0064 0053 0064 0053  .|._.d.S.d.S.d.S
+000006c0: 0064 0053 0064 0053 0029 054e 5429 01da  .d.S.d.S.).NT)..
+000006d0: 0563 6c65 616e e901 0000 0072 0100 0000  .clean.....r....
+000006e0: 2908 da04 626f 6479 da0d 6765 745f 646f  )...body..get_do
+000006f0: 6373 7472 696e 67da 036c 656e da0a 6973  cstring..len..is
+00000700: 696e 7374 616e 6365 da03 6373 74da 1353  instance..cst..S
+00000710: 696d 706c 6553 7461 7465 6d65 6e74 4c69  impleStatementLi
+00000720: 6e65 da04 5061 7373 722c 0000 0029 0572  ne..Passr,...).r
+00000730: 2d00 0000 722f 0000 0072 3200 0000 da09  -...r/...r2.....
+00000740: 646f 6373 7472 696e 675a 0f66 6972 7374  docstringZ.first
+00000750: 5f73 7461 7465 6d65 6e74 721c 0000 0072  _statementr....r
+00000760: 1c00 0000 721d 0000 00da 1176 6973 6974  ....r......visit
+00000770: 5f46 756e 6374 696f 6e44 6566 3100 0000  _FunctionDef1...
+00000780: 7318 0000 0008 010c 0108 030c 011c 0308  s...............
+00000790: 0110 010c 0104 ff0a 0308 fb08 027a 2453  .............z$S
+000007a0: 686f 756c 6457 7269 7465 5669 7369 746f  houldWriteVisito
+000007b0: 722e 7669 7369 745f 4675 6e63 7469 6f6e  r.visit_Function
+000007c0: 4465 6629 0272 2100 0000 4e29 07da 085f  Def).r!...N)..._
+000007d0: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
+000007e0: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
+000007f0: 5f72 2e00 0000 7236 0000 00da 0b46 756e  _r....r6.....Fun
+00000800: 6374 696f 6e44 6566 723a 0000 0072 1c00  ctionDefr:...r..
+00000810: 0000 721c 0000 0072 1c00 0000 721d 0000  ..r....r....r...
+00000820: 0072 2b00 0000 2d00 0000 7306 0000 0008  .r+...-...s.....
+00000830: 000a 0118 0372 2b00 0000 721a 0000 0063  .....r+...r....c
+00000840: 0100 0000 0000 0000 0000 0000 0400 0000  ................
+00000850: 0300 0000 4300 0000 732a 0000 0074 00a0  ....C...s*...t..
+00000860: 017c 00a1 017d 0174 02a0 037c 01a1 017d  .|...}.t...|...}
+00000870: 0274 0483 007d 037c 02a0 057c 03a1 0101  .t...}.|...|....
+00000880: 007c 036a 0653 0072 1100 0000 2907 7222  .|.j.S.r....).r"
+00000890: 0000 00da 0967 6574 736f 7572 6365 7236  .....getsourcer6
+000008a0: 0000 00da 0c70 6172 7365 5f6d 6f64 756c  .....parse_modul
+000008b0: 6572 2b00 0000 da05 7669 7369 7472 2c00  er+.....visitr,.
+000008c0: 0000 2904 721a 0000 00da 0673 6f75 7263  ..).r......sourc
+000008d0: 65da 066d 6f64 756c 65da 0776 6973 6974  e..module..visit
+000008e0: 6f72 721c 0000 0072 1c00 0000 721d 0000  orr....r....r...
+000008f0: 0072 1300 0000 4200 0000 730a 0000 000a  .r....B...s.....
+00000900: 010a 0106 010a 0106 0172 1300 0000 721b  .........r....r.
+00000910: 0000 00da 0e64 6563 6f72 6174 6564 5f66  .....decorated_f
+00000920: 756e 6363 0200 0000 0000 0000 0000 0000  uncc............
+00000930: 0400 0000 0a00 0000 4300 0000 738a 0000  ........C...s...
+00000940: 0074 006a 017d 0274 027c 0074 036a 047c  .t.j.}.t.|.t.j.|
+00000950: 0274 056a 066b 0383 0301 007c 0274 056a  .t.j.k.....|.t.j
+00000960: 076b 0272 4374 087c 0183 017d 0374 027c  .k.rCt.|...}.t.|
+00000970: 0074 036a 0974 0a6a 0b7c 017c 0364 0119  .t.j.t.j.|.|.d..
+00000980: 007c 0364 0219 007c 0364 0319 007c 0364  .|.d...|.d...|.d
+00000990: 0419 0064 058d 0583 0301 0074 027c 0074  ...d.......t.|.t
+000009a0: 036a 0c74 0d7c 0364 0119 0074 0e83 0074  .j.t.|.d...t...t
+000009b0: 0da0 0f7c 016a 10a1 0167 0164 068d 0383  ...|.j...g.d....
+000009c0: 0301 0064 0053 0064 0053 0029 074e da03  ...d.S.d.S.).N..
+000009d0: 616c 6c72 2d00 0000 da0b 7265 7475 726e  allr-.....return
+000009e0: 5f74 7970 65da 0670 6172 616d 7329 05da  _type..params)..
+000009f0: 0d69 6e66 6572 7265 645f 6675 6e63 da14  .inferred_func..
+00000a00: 616c 6c5f 7479 7065 5f64 6566 696e 6974  all_type_definit
+00000a10: 696f 6e73 da0f 7365 6c66 5f64 6566 696e  ions..self_defin
+00000a20: 6974 696f 6eda 1672 6574 7572 6e5f 7479  ition..return_ty
+00000a30: 7065 5f64 6566 696e 6974 696f 6eda 1170  pe_definition..p
+00000a40: 6172 616d 5f64 6566 696e 6974 696f 6e73  aram_definitions
+00000a50: 2903 da10 7479 7065 5f64 6566 696e 6974  )...type_definit
+00000a60: 696f 6e73 da05 7465 7374 73da 0770 6172  ions..tests..par
+00000a70: 656e 7473 2911 720b 0000 00da 0b65 6e76  ents).r......env
+00000a80: 6972 6f6e 6d65 6e74 da07 7365 7461 7474  ironment..setatt
+00000a90: 7272 0c00 0000 da06 6973 5f64 6576 7210  rr......is_devr.
+00000aa0: 0000 00da 0450 524f 44da 0344 4556 720f  .....PROD..DEVr.
+00000ab0: 0000 00da 0b64 6563 6c61 7261 7469 6f6e  .....declaration
+00000ac0: 7209 0000 00da 1e66 726f 6d5f 696e 6665  r......from_infe
+00000ad0: 7272 6564 5f66 756e 635f 6465 636c 6172  rred_func_declar
+00000ae0: 6174 696f 6eda 0566 7261 6d65 720e 0000  ation..framer...
+00000af0: 0072 0d00 0000 da0a 666f 725f 6d6f 6475  .r......for_modu
+00000b00: 6c65 723c 0000 0029 0472 1b00 0000 7245  ler<...).r....rE
+00000b10: 0000 00da 0365 6e76 5a14 6675 6e63 7469  .....envZ.functi
+00000b20: 6f6e 5f64 6566 696e 6974 696f 6e73 721c  on_definitionsr.
+00000b30: 0000 0072 1c00 0000 721d 0000 0072 1e00  ...r....r....r..
+00000b40: 0000 4a00 0000 7332 0000 0006 0114 010a  ..J...s2........
+00000b50: 0108 0102 0102 0104 0104 0102 0106 0106  ................
+00000b60: 0106 0106 0104 fb04 fd02 0b02 0104 0102  ................
+00000b70: 0106 0104 010c 0104 fd08 fd04 f372 1e00  .............r..
+00000b80: 0000 2929 da09 6675 6e63 746f 6f6c 7372  ..))..functoolsr
+00000b90: 0200 0000 7222 0000 00da 0674 7970 696e  ....r".....typin
+00000ba0: 6772 0300 0000 7204 0000 0072 0500 0000  gr....r....r....
+00000bb0: 7206 0000 0072 0700 0000 7208 0000 00da  r....r....r.....
+00000bc0: 2763 6f64 6573 7065 616b 2e66 756e 6374  'codespeak.funct
+00000bd0: 696f 6e2e 6675 6e63 7469 6f6e 5f64 6563  ion.function_dec
+00000be0: 6c61 7261 7469 6f6e 7209 0000 005a 2463  larationr....Z$c
+00000bf0: 6f64 6573 7065 616b 2e66 756e 6374 696f  odespeak.functio
+00000c00: 6e2e 7772 6974 6162 6c65 5f66 756e 6374  n.writable_funct
+00000c10: 696f 6e72 0a00 0000 da09 636f 6465 7370  ionr......codesp
+00000c20: 6561 6b72 0b00 0000 da26 636f 6465 7370  eakr.....&codesp
+00000c30: 6561 6b2e 6675 6e63 7469 6f6e 2e66 756e  eak.function.fun
+00000c40: 6374 696f 6e5f 6174 7472 6962 7574 6573  ction_attributes
+00000c50: 720c 0000 00da 1563 6f64 6573 7065 616b  r......codespeak
+00000c60: 2e66 7261 6d65 5f74 6573 7473 720d 0000  .frame_testsr...
+00000c70: 00da 0f63 6f64 6573 7065 616b 2e66 7261  ...codespeak.fra
+00000c80: 6d65 720e 0000 005a 3663 6f64 6573 7065  mer....Z6codespe
+00000c90: 616b 2e68 656c 7065 7273 2e67 6574 5f64  ak.helpers.get_d
+00000ca0: 6566 696e 6974 696f 6e73 5f66 726f 6d5f  efinitions_from_
+00000cb0: 6675 6e63 7469 6f6e 5f6f 626a 6563 7472  function_objectr
+00000cc0: 0f00 0000 7210 0000 0072 1f00 0000 da03  ....r....r......
+00000cd0: 7374 7272 1500 0000 da06 6c69 6263 7374  strr......libcst
+00000ce0: 7236 0000 0072 2600 0000 7227 0000 005a  r6...r&...r'...Z
+00000cf0: 0f6c 6962 6373 742e 6d65 7461 6461 7461  .libcst.metadata
+00000d00: 7228 0000 0072 2900 0000 722a 0000 00da  r(...r)...r*....
+00000d10: 0a43 5354 5669 7369 746f 7272 2b00 0000  .CSTVisitorr+...
+00000d20: da04 626f 6f6c 7213 0000 0072 1e00 0000  ..boolr....r....
+00000d30: 721c 0000 0072 1c00 0000 721c 0000 0072  r....r....r....r
+00000d40: 1d00 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
+00000d50: 0000 7328 0000 000c 0008 0120 010c 010c  ..s(....... ....
+00000d60: 010c 030c 010c 010c 010c 010c 010c 0308  ................
+00000d70: 0312 0e08 0710 0114 0112 0312 1516 08    ...............
```

### Comparing `codespeak-0.1.5/codespeak/decorate/__pycache__/writable_transform.cpython-310.pyc` & `codespeak-0.1.6/codespeak/decorate/__pycache__/writable_transform.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/decorate/writable.py` & `codespeak-0.1.6/codespeak/decorate/writable.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,23 +2,22 @@
 import inspect
 from typing import Any, Callable, Dict, List, Tuple, TypeVar
 from functools import wraps
 from codespeak.function.function_declaration import (
     FunctionDeclaration,
 )
 from codespeak.function.writable_function import WritableFunction
-from codespeak.settings import settings
-from codespeak.settings.environment import Environment
+from codespeak import settings
 from codespeak.function.function_attributes import FunctionAttributes
 from codespeak.frame_tests import FrameTests
 from codespeak.frame import Frame
 from codespeak.helpers.get_definitions_from_function_object import (
     get_definitions_from_function_object,
 )
-from codespeak.settings.settings import Environment
+from codespeak import Environment
 
 
 def writable(func):
     @wraps(func)
     def wrapper(*args, **kwargs):
         if wrapper._is_dev:  # type: ignore
             if should_write_function(func):
@@ -69,15 +68,15 @@
     module = cst.parse_module(source)
     visitor = ShouldWriteVisitor()
     module.visit(visitor)
     return visitor.should_write
 
 
 def _assign_default_function_attributes(wrapper: Callable, decorated_func: Callable):
-    env = settings.get_environment()
+    env = settings.environment
     setattr(wrapper, FunctionAttributes.is_dev, env != Environment.PROD)
     if env == Environment.DEV:
         function_definitions = get_definitions_from_function_object(decorated_func)
         setattr(
             wrapper,
             FunctionAttributes.declaration,
             FunctionDeclaration.from_inferred_func_declaration(
```

### Comparing `codespeak-0.1.5/codespeak/decorate/writable_transform.py` & `codespeak-0.1.6/codespeak/inference/replace_function.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Sequence
+from typing import List, Sequence
 import libcst as cst
 import textwrap
 from libcst import BaseCompoundStatement, FunctionDef, SimpleStatementLine, CSTNode
 
 
 class ReplaceFunctionTransformer(cst.CSTTransformer):
     def __init__(
@@ -17,25 +17,61 @@
         self, original_node: FunctionDef, updated_node: FunctionDef
     ) -> CSTNode:
         if original_node.name.value == self.function_name:
             return self.new_function_def
         return updated_node
 
 
+class AddCodeTransformer(cst.CSTTransformer):
+    def __init__(
+        self,
+        function_name: str,
+        new_function_def: SimpleStatementLine | BaseCompoundStatement,
+        incoming_import_statements: list[str],
+    ) -> None:
+        self.new_function_def = new_function_def
+        self.function_name = function_name
+        self.incoming_import_statements = incoming_import_statements
+
+    def leave_Module(
+        self, original_node: cst.Module, updated_node: cst.Module
+    ) -> cst.Module:
+        body = updated_node.body
+        new_body = []
+        for stmt in body:
+            if (
+                isinstance(stmt, cst.FunctionDef)
+                and stmt.name.value == self.function_name
+            ):
+                for i, import_stmt in enumerate(self.incoming_import_statements):
+                    if i == 0:
+                        import_stmt = "\n\n" + import_stmt
+                    new_body.append(cst.parse_statement(import_stmt))
+                new_body.append(self.new_function_def)
+            else:
+                new_body.append(stmt)
+        return updated_node.with_changes(body=new_body)
+
+
 def get_function_node(
     name: str, body: Sequence[SimpleStatementLine | BaseCompoundStatement]
 ) -> FunctionDef:
     for node in body:
         if isinstance(node, cst.FunctionDef):
             if node.name.value == name:
                 return node
     raise ValueError(f"Function {name} not found in body")
 
 
-def replace_function(filepath: str, function_name: str, new_source_code: str):
+def replace_function(
+    filepath: str,
+    function_name: str,
+    new_source_code: str,
+    incoming_import_statements: List[str],
+):
     replaceable_code = ""
     with open(filepath, "r") as f:
         replaceable_code = f.read()
 
     # Parse the source code into CSTs
     module = cst.parse_module(replaceable_code)
     # new_function_def = cst.parse_statement(new_function)
@@ -52,16 +88,18 @@
 
     # Add leading lines to new function
     new_function_with_comments = new_function_def.with_changes(
         leading_lines=leading_lines
     )
 
     # Create an instance of the transformer and apply it to the CST
-    transformer = ReplaceFunctionTransformer(
-        function_name=function_name, new_function_def=new_function_with_comments
+    transformer = AddCodeTransformer(
+        function_name=function_name,
+        new_function_def=new_function_with_comments,
+        incoming_import_statements=incoming_import_statements,
     )
     new_module = module.visit(transformer)
 
     # Convert the CST back into source code
     new_source_code = new_module.code
 
     with open(filepath, "w") as f:
```

### Comparing `codespeak-0.1.5/codespeak/frame.py` & `codespeak-0.1.6/codespeak/frame.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
     def custom_types(self) -> Dict:
         types_ = {}
         for _class in self.type_definitions:
             types_.update(_class.custom_types())
         for parent in self.parents:
             types_.update(parent.custom_types())
-        types_.update(InferredExceptionHelpers.annotate())
+        # types_.update(InferredExceptionHelpers.annotate())
         return types_
 
     def printable_custom_types(self) -> str:
         return json.dumps(self.custom_types(), indent=4)
 
     def printable_type_definitions_with_inheritance(self) -> str:
         return json.dumps(
```

### Comparing `codespeak-0.1.5/codespeak/function/__pycache__/_accessors.cpython-310.pyc` & `codespeak-0.1.6/codespeak/function/__pycache__/_accessors.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/function/__pycache__/_body_resources.cpython-310.pyc` & `codespeak-0.1.6/codespeak/function/__pycache__/_body_resources.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/function/__pycache__/_infer.cpython-310.pyc` & `codespeak-0.1.6/codespeak/function/__pycache__/_infer.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/function/__pycache__/_inference.cpython-310.pyc` & `codespeak-0.1.6/codespeak/function/__pycache__/_inference.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/function/__pycache__/_private_function.cpython-310.pyc` & `codespeak-0.1.6/codespeak/function/__pycache__/_private_function.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/function/__pycache__/_resources.cpython-310.pyc` & `codespeak-0.1.6/codespeak/function/__pycache__/_resources.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/function/__pycache__/_tests.cpython-310.pyc` & `codespeak-0.1.6/codespeak/function/__pycache__/_tests.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/function/__pycache__/accessors.cpython-310.pyc` & `codespeak-0.1.6/codespeak/function/__pycache__/accessors.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/function/__pycache__/function.cpython-310.pyc` & `codespeak-0.1.6/codespeak/function/__pycache__/function.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/function/__pycache__/function_declaration.cpython-310.pyc` & `codespeak-0.1.6/codespeak/function/__pycache__/function_declaration.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/function/__pycache__/function_declaration_lite.cpython-310.pyc` & `codespeak-0.1.6/codespeak/function/__pycache__/function_declaration_lite.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/function/__pycache__/function_digest.cpython-310.pyc` & `codespeak-0.1.6/codespeak/function/__pycache__/function_digest.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/function/__pycache__/function_file_service.cpython-310.pyc` & `codespeak-0.1.6/codespeak/function/__pycache__/function_file_service.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/function/__pycache__/function_lite.cpython-310.pyc` & `codespeak-0.1.6/codespeak/function/__pycache__/function_lite.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/function/__pycache__/function_manager.cpython-310.pyc` & `codespeak-0.1.6/codespeak/function/__pycache__/function_manager.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/function/__pycache__/function_metadata.cpython-310.pyc` & `codespeak-0.1.6/codespeak/function/__pycache__/function_metadata.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/function/__pycache__/function_tests.cpython-310.pyc` & `codespeak-0.1.6/codespeak/function/__pycache__/function_tests.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/function/__pycache__/inference.cpython-310.pyc` & `codespeak-0.1.6/codespeak/function/__pycache__/inference.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/function/__pycache__/inference_manager.cpython-310.pyc` & `codespeak-0.1.6/codespeak/function/__pycache__/inference_manager.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/function/__pycache__/writable_function.cpython-310.pyc` & `codespeak-0.1.6/codespeak/function/__pycache__/writable_function.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Jul 26 18:49:48 2023 UTC, .py size: 2491 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 18% similar despite different names*

```diff
@@ -1,209 +1,214 @@
-00000000: 6f0d 0d0a 0000 0000 cc6a c164 bb09 0000  o........j.d....
+00000000: 6f0d 0d0a 0000 0000 aac7 c264 460a 0000  o..........dF...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0003 0000 0040 0000 0073 ae00 0000 6400  .....@...s....d.
+00000020: 0003 0000 0040 0000 0073 b200 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 6d04 5a04 6d05 5a05  d.l.m.Z.m.Z.m.Z.
 00000050: 6d06 5a06 6d07 5a07 6d08 5a08 0100 6400  m.Z.m.Z.m.Z...d.
 00000060: 6403 6c09 6d0a 5a0a 0100 6400 6404 6c0b  d.l.m.Z...d.d.l.
 00000070: 6d0c 5a0c 0100 6400 6405 6c0d 6d0e 5a0e  m.Z...d.d.l.m.Z.
 00000080: 0100 6400 6406 6c0f 6d10 5a10 0100 6400  ..d.d.l.m.Z...d.
-00000090: 6407 6c11 6d12 5a12 0100 6400 6408 6c13  d.l.m.Z...d.d.l.
-000000a0: 6d14 5a14 0100 6400 6409 6c15 6d16 5a16  m.Z...d.d.l.m.Z.
-000000b0: 0100 6400 640a 6c17 6d18 5a18 0100 6400  ..d.d.l.m.Z...d.
-000000c0: 640b 6c19 6d1a 5a1a 0100 4700 640c 640d  d.l.m.Z...G.d.d.
-000000d0: 8400 640d 8302 5a1b 6401 5300 290e e900  ..d...Z.d.S.)...
-000000e0: 0000 004e 2906 da03 416e 79da 0843 616c  ...N)...Any..Cal
-000000f0: 6c61 626c 65da 0444 6963 74da 044c 6973  lable..Dict..Lis
-00000100: 74da 0843 6c61 7373 5661 72da 0554 7570  t..ClassVar..Tup
-00000110: 6c65 2901 da13 4675 6e63 7469 6f6e 4465  le)...FunctionDe
-00000120: 636c 6172 6174 696f 6e29 01da 0c46 756e  claration)...Fun
-00000130: 6374 696f 6e4c 6974 6529 01da 1373 656c  ctionLite)...sel
-00000140: 665f 7479 7065 5f69 665f 6578 6973 7473  f_type_if_exists
-00000150: 2901 da10 7265 706c 6163 655f 6675 6e63  )...replace_func
-00000160: 7469 6f6e 2901 da0f 496e 6665 7265 6e63  tion)...Inferenc
-00000170: 6545 6e67 696e 6529 01da 0546 7261 6d65  eEngine)...Frame
-00000180: 2901 da12 4675 6e63 7469 6f6e 4174 7472  )...FunctionAttr
-00000190: 6962 7574 6573 2901 da17 4675 6e63 7469  ibutes)...Functi
-000001a0: 6f6e 4465 636c 6172 6174 696f 6e4c 6974  onDeclarationLit
-000001b0: 6529 01da 0873 6574 7469 6e67 7363 0000  e)...settingsc..
-000001c0: 0000 0000 0000 0000 0000 0000 0000 0500  ................
-000001d0: 0000 4000 0000 73b0 0000 0065 005a 0164  ..@...s....e.Z.d
-000001e0: 005a 0255 0065 0365 0464 013c 0064 0165  .Z.U.e.e.d.<.d.e
-000001f0: 0364 0264 0366 0464 0464 0584 045a 0565  .d.d.f.d.d...Z.e
-00000200: 0664 0265 0766 0264 0664 0784 0483 015a  .d.e.f.d.d.....Z
-00000210: 0865 0664 0265 0966 0264 0864 0984 0483  .e.d.e.f.d.d....
-00000220: 015a 0a64 0265 0b66 0264 0a64 0b84 045a  .Z.d.e.f.d.d...Z
-00000230: 0c64 0265 0b66 0264 0c64 0d84 045a 0d64  .d.e.f.d.d...Z.d
-00000240: 1864 0e64 0f84 045a 0e64 1065 0b64 0264  .d.d...Z.d.e.d.d
-00000250: 0366 0464 1164 1284 045a 0f64 0265 1066  .f.d.d...Z.d.e.f
-00000260: 0264 1364 1484 045a 1165 1264 0165 0364  .d.d...Z.e.d.e.d
-00000270: 1565 1366 0219 0064 0264 0066 0464 1664  .e.f...d.d.f.d.d
-00000280: 1784 0483 015a 1464 0353 0029 19da 1057  .....Z.d.S.)...W
-00000290: 7269 7461 626c 6546 756e 6374 696f 6eda  ritableFunction.
-000002a0: 0466 756e 63da 0672 6574 7572 6e4e 6302  .func..returnNc.
-000002b0: 0000 0000 0000 0000 0000 0002 0000 0003  ................
-000002c0: 0000 0043 0000 0073 1e00 0000 7400 7c01  ...C...s....t.|.
-000002d0: 7401 6a02 8302 730a 7403 6401 8301 8201  t.j...s.t.d.....
-000002e0: 7c01 7c00 5f04 6400 5300 2902 4e75 6300  |.|._.d.S.).Nuc.
-000002f0: 0000 4e6f 2066 7261 6d65 2066 6f75 6e64  ..No frame found
-00000300: 2e20 4d61 6b65 2073 7572 6520 7468 6973  . Make sure this
-00000310: 2069 7320 616e 2069 6e66 6572 7265 6420   is an inferred 
-00000320: 6675 6e63 7469 6f6e e280 9469 7420 7368  function...it sh
-00000330: 6f75 6c64 2075 7365 2063 6f64 6573 7065  ould use codespe
-00000340: 616b 2773 2040 696e 6665 7220 6465 636f  ak's @infer deco
-00000350: 7261 746f 7229 05da 0768 6173 6174 7472  rator)...hasattr
-00000360: 720e 0000 00da 0566 7261 6d65 da09 4578  r......frame..Ex
-00000370: 6365 7074 696f 6e72 1200 0000 2902 da04  ceptionr....)...
-00000380: 7365 6c66 7212 0000 00a9 0072 1800 0000  selfr......r....
-00000390: fa46 2f55 7365 7273 2f6e 6174 6861 6e73  .F/Users/nathans
-000003a0: 6869 726c 6579 2f63 6f64 6573 7065 616b  hirley/codespeak
-000003b0: 2f63 6f64 6573 7065 616b 2f66 756e 6374  /codespeak/funct
-000003c0: 696f 6e2f 7772 6974 6162 6c65 5f66 756e  ion/writable_fun
-000003d0: 6374 696f 6e2e 7079 da08 5f5f 696e 6974  ction.py..__init
-000003e0: 5f5f 1200 0000 730a 0000 000c 0102 0102  __....s.........
-000003f0: 0104 ff0a 037a 1957 7269 7461 626c 6546  .....z.WritableF
-00000400: 756e 6374 696f 6e2e 5f5f 696e 6974 5f5f  unction.__init__
-00000410: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-00000420: 0003 0000 0043 0000 0073 0e00 0000 7400  .....C...s....t.
-00000430: 7c00 6a01 7402 6a03 8302 5300 a901 4e29  |.j.t.j...S...N)
-00000440: 04da 0767 6574 6174 7472 7212 0000 0072  ...getattrr....r
-00000450: 0e00 0000 da0b 6465 636c 6172 6174 696f  ......declaratio
-00000460: 6ea9 0172 1700 0000 7218 0000 0072 1800  n..r....r....r..
-00000470: 0000 7219 0000 0072 1d00 0000 1900 0000  ..r....r........
-00000480: 7302 0000 000e 027a 1c57 7269 7461 626c  s......z.Writabl
-00000490: 6546 756e 6374 696f 6e2e 6465 636c 6172  eFunction.declar
-000004a0: 6174 696f 6e63 0100 0000 0000 0000 0000  ationc..........
-000004b0: 0000 0100 0000 0300 0000 4300 0000 730c  ..........C...s.
-000004c0: 0000 0074 00a0 017c 006a 02a1 0153 0072  ...t...|.j...S.r
-000004d0: 1b00 0000 2903 720d 0000 005a 0c66 6f72  ....).r....Z.for
-000004e0: 5f66 756e 6374 696f 6e72 1200 0000 721e  _functionr....r.
-000004f0: 0000 0072 1800 0000 7218 0000 0072 1900  ...r....r....r..
-00000500: 0000 7215 0000 001d 0000 0073 0200 0000  ..r........s....
-00000510: 0c02 7a16 5772 6974 6162 6c65 4675 6e63  ..z.WritableFunc
-00000520: 7469 6f6e 2e66 7261 6d65 6301 0000 0000  tion.framec.....
-00000530: 0000 0000 0000 0004 0000 0004 0000 0043  ...............C
-00000540: 0000 0073 3400 0000 7c00 a000 a100 7d01  ...s4...|.....}.
-00000550: 7401 a002 a100 7d02 7c02 6400 7500 7210  t.....}.|.d.u.r.
-00000560: 7403 6401 8301 8201 7404 7c01 7c02 6402  t.d.....t.|.|.d.
-00000570: 8d02 7d03 7c03 a005 a100 5300 2903 4e7a  ..}.|.....S.).Nz
-00000580: 2f4e 6f20 6170 6920 7365 742e 2041 6464  /No api set. Add
-00000590: 2061 6e20 6170 6920 7769 7468 2063 6f64   an api with cod
-000005a0: 6573 7065 616b 2e61 6464 5f61 7069 2829  espeak.add_api()
-000005b0: 2902 da0d 6675 6e63 7469 6f6e 5f6c 6974  )...function_lit
-000005c0: 65da 0e61 7069 5f69 6465 6e74 6966 6965  e..api_identifie
-000005d0: 7229 06da 1074 6f5f 6675 6e63 7469 6f6e  r)...to_function
-000005e0: 5f6c 6974 6572 1000 0000 5a1a 6765 745f  _liter....Z.get_
-000005f0: 6375 7272 656e 745f 6170 695f 6964 656e  current_api_iden
-00000600: 7469 6669 6572 da0a 5661 6c75 6545 7272  tifier..ValueErr
-00000610: 6f72 720c 0000 00da 0e6d 616b 655f 696e  orr......make_in
-00000620: 6665 7265 6e63 6529 0472 1700 0000 721f  ference).r....r.
-00000630: 0000 0072 2000 0000 5a14 6170 695f 696e  ...r ...Z.api_in
-00000640: 6665 7265 6e63 655f 656e 6769 6e65 7218  ference_enginer.
-00000650: 0000 0072 1800 0000 7219 0000 00da 0f5f  ...r....r......_
-00000660: 6d61 6b65 5f69 6e66 6572 656e 6365 2100  make_inference!.
-00000670: 0000 7312 0000 0008 0108 0108 0108 0102  ..s.............
-00000680: 0102 0102 0106 fe08 047a 2057 7269 7461  .........z Writa
-00000690: 626c 6546 756e 6374 696f 6e2e 5f6d 616b  bleFunction._mak
-000006a0: 655f 696e 6665 7265 6e63 6563 0100 0000  e_inferencec....
-000006b0: 0000 0000 0000 0000 0200 0000 0300 0000  ................
-000006c0: 4300 0000 7320 0000 0074 00a0 017c 006a  C...s ...t...|.j
-000006d0: 02a1 017d 017c 0164 0075 0072 0e74 0364  ...}.|.d.u.r.t.d
-000006e0: 0183 0182 017c 0153 0029 024e 7a22 4675  .....|.S.).Nz"Fu
-000006f0: 6e63 7469 6f6e 206d 7573 7420 6265 2064  nction must be d
-00000700: 6566 696e 6564 2069 6e20 6120 6669 6c65  efined in a file
-00000710: 2904 da07 696e 7370 6563 74da 0d67 6574  )...inspect..get
-00000720: 736f 7572 6365 6669 6c65 7212 0000 0072  sourcefiler....r
-00000730: 2200 0000 2902 7217 0000 005a 0266 6672  "...).r....Z.ffr
-00000740: 1800 0000 7218 0000 0072 1900 0000 da0b  ....r....r......
-00000750: 736f 7572 6365 5f66 696c 652c 0000 0073  source_file,...s
-00000760: 0800 0000 0c01 0801 0801 0401 7a1c 5772  ............z.Wr
-00000770: 6974 6162 6c65 4675 6e63 7469 6f6e 2e73  itableFunction.s
-00000780: 6f75 7263 655f 6669 6c65 6301 0000 0000  ource_filec.....
-00000790: 0000 0000 0000 0001 0000 0004 0000 0043  ...............C
-000007a0: 0000 0073 1200 0000 7c00 a000 7c00 a001  ...s....|...|...
-000007b0: a100 a101 0100 6400 5300 721b 0000 0029  ......d.S.r....)
-000007c0: 02da 065f 7772 6974 6572 2700 0000 721e  ..._writer'...r.
-000007d0: 0000 0072 1800 0000 7218 0000 0072 1900  ...r....r....r..
-000007e0: 0000 da05 7772 6974 6532 0000 0073 0200  ....write2...s..
-000007f0: 0000 1201 7a16 5772 6974 6162 6c65 4675  ....z.WritableFu
-00000800: 6e63 7469 6f6e 2e77 7269 7465 7227 0000  nction.writer'..
-00000810: 0063 0200 0000 0000 0000 0000 0000 0300  .c..............
-00000820: 0000 0400 0000 4300 0000 731c 0000 007c  ......C...s....|
-00000830: 00a0 00a1 007d 0274 017c 017c 006a 026a  .....}.t.|.|.j.j
-00000840: 037c 0283 0301 0064 0053 0072 1b00 0000  .|.....d.S.r....
-00000850: 2904 7224 0000 0072 0b00 0000 7212 0000  ).r$...r....r...
-00000860: 00da 0c5f 5f71 7561 6c6e 616d 655f 5f29  ...__qualname__)
-00000870: 0372 1700 0000 7227 0000 00da 0969 6e66  .r....r'.....inf
-00000880: 6572 656e 6365 7218 0000 0072 1800 0000  erencer....r....
-00000890: 7219 0000 0072 2800 0000 3500 0000 7304  r....r(...5...s.
-000008a0: 0000 0008 0114 017a 1757 7269 7461 626c  .......z.Writabl
-000008b0: 6546 756e 6374 696f 6e2e 5f77 7269 7465  eFunction._write
-000008c0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-000008d0: 0004 0000 0043 0000 0073 1800 0000 7400  .....C...s....t.
-000008e0: 7c00 6a01 a002 a100 7c00 6a03 a004 a100  |.j.....|.j.....
-000008f0: 6401 8d02 5300 2902 4e29 0272 1d00 0000  d...S.).N).r....
-00000900: da0c 6375 7374 6f6d 5f74 7970 6573 2905  ..custom_types).
-00000910: 7209 0000 0072 1d00 0000 5a13 746f 5f64  r....r....Z.to_d
-00000920: 6563 6c61 7261 7469 6f6e 5f6c 6974 6572  eclaration_liter
-00000930: 1500 0000 722c 0000 0072 1e00 0000 7218  ....r,...r....r.
-00000940: 0000 0072 1800 0000 7219 0000 0072 2100  ...r....r....r!.
-00000950: 0000 3900 0000 7308 0000 0002 0108 0108  ..9...s.........
-00000960: 0106 fe7a 2157 7269 7461 626c 6546 756e  ...z!WritableFun
-00000970: 6374 696f 6e2e 746f 5f66 756e 6374 696f  ction.to_functio
-00000980: 6e5f 6c69 7465 2e63 0100 0000 0000 0000  n_lite.c........
-00000990: 0000 0000 0100 0000 0300 0000 4300 0000  ............C...
-000009a0: 730a 0000 0074 007c 0064 018d 0153 0029  s....t.|.d...S.)
-000009b0: 027a 3767 6574 2063 6c61 7373 6966 6965  .z7get classifie
-000009c0: 6420 4675 6e63 7469 6f6e 206f 626a 6563  d Function objec
-000009d0: 7420 666f 7220 616e 2069 6e66 6572 7265  t for an inferre
-000009e0: 6420 6675 6e63 7469 6f6e a901 7212 0000  d function..r...
-000009f0: 0029 0172 1100 0000 722d 0000 0072 1800  .).r....r-...r..
-00000a00: 0000 7218 0000 0072 1900 0000 da14 6672  ..r....r......fr
-00000a10: 6f6d 5f66 756e 6374 696f 6e5f 6f62 6a65  om_function_obje
-00000a20: 6374 3f00 0000 7302 0000 000a 037a 2557  ct?...s......z%W
-00000a30: 7269 7461 626c 6546 756e 6374 696f 6e2e  ritableFunction.
-00000a40: 6672 6f6d 5f66 756e 6374 696f 6e5f 6f62  from_function_ob
-00000a50: 6a65 6374 2902 7213 0000 004e 2915 da08  ject).r....N)...
-00000a60: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
-00000a70: 6c65 5f5f 722a 0000 0072 0300 0000 da0f  le__r*...r......
-00000a80: 5f5f 616e 6e6f 7461 7469 6f6e 735f 5f72  __annotations__r
-00000a90: 1a00 0000 da08 7072 6f70 6572 7479 7208  ......propertyr.
-00000aa0: 0000 0072 1d00 0000 720d 0000 0072 1500  ...r....r....r..
-00000ab0: 0000 da03 7374 7272 2400 0000 7227 0000  ....strr$...r'..
-00000ac0: 0072 2900 0000 7228 0000 0072 0900 0000  .r)...r(...r....
-00000ad0: 7221 0000 00da 0c73 7461 7469 636d 6574  r!.....staticmet
-00000ae0: 686f 6472 0200 0000 722e 0000 0072 1800  hodr....r....r..
-00000af0: 0000 7218 0000 0072 1800 0000 7219 0000  ..r....r....r...
-00000b00: 0072 1100 0000 0f00 0000 731c 0000 000a  .r........s.....
-00000b10: 0008 0112 0202 0710 0102 0310 010e 030e  ................
-00000b20: 0b0a 0612 030e 0402 0620 0172 1100 0000  ......... .r....
-00000b30: 291c 7225 0000 00da 046a 736f 6eda 0674  ).r%.....json..t
-00000b40: 7970 696e 6772 0200 0000 7203 0000 0072  ypingr....r....r
-00000b50: 0400 0000 7205 0000 0072 0600 0000 7207  ....r....r....r.
-00000b60: 0000 005a 2763 6f64 6573 7065 616b 2e66  ...Z'codespeak.f
-00000b70: 756e 6374 696f 6e2e 6675 6e63 7469 6f6e  unction.function
-00000b80: 5f64 6563 6c61 7261 7469 6f6e 7208 0000  _declarationr...
-00000b90: 00da 2063 6f64 6573 7065 616b 2e66 756e  .. codespeak.fun
-00000ba0: 6374 696f 6e2e 6675 6e63 7469 6f6e 5f6c  ction.function_l
-00000bb0: 6974 6572 0900 0000 5a1b 636f 6465 7370  iter....Z.codesp
-00000bc0: 6561 6b2e 6865 6c70 6572 732e 7365 6c66  eak.helpers.self
-00000bd0: 5f74 7970 6572 0a00 0000 5a25 636f 6465  _typer....Z%code
-00000be0: 7370 6561 6b2e 6465 636f 7261 7465 2e77  speak.decorate.w
-00000bf0: 7269 7461 626c 655f 7472 616e 7366 6f72  ritable_transfor
-00000c00: 6d72 0b00 0000 5a24 636f 6465 7370 6561  mr....Z$codespea
-00000c10: 6b2e 696e 6665 7265 6e63 652e 696e 6665  k.inference.infe
-00000c20: 7265 6e63 655f 656e 6769 6e65 720c 0000  rence_enginer...
-00000c30: 005a 0f63 6f64 6573 7065 616b 2e66 7261  .Z.codespeak.fra
-00000c40: 6d65 720d 0000 005a 2663 6f64 6573 7065  mer....Z&codespe
-00000c50: 616b 2e66 756e 6374 696f 6e2e 6675 6e63  ak.function.func
-00000c60: 7469 6f6e 5f61 7474 7269 6275 7465 7372  tion_attributesr
-00000c70: 0e00 0000 da2c 636f 6465 7370 6561 6b2e  .....,codespeak.
-00000c80: 6675 6e63 7469 6f6e 2e66 756e 6374 696f  function.functio
-00000c90: 6e5f 6465 636c 6172 6174 696f 6e5f 6c69  n_declaration_li
-00000ca0: 7465 720f 0000 005a 1263 6f64 6573 7065  ter....Z.codespe
-00000cb0: 616b 2e73 6574 7469 6e67 7372 1000 0000  ak.settingsr....
-00000cc0: 7211 0000 0072 1800 0000 7218 0000 0072  r....r....r....r
-00000cd0: 1800 0000 7219 0000 00da 083c 6d6f 6475  ....r......<modu
-00000ce0: 6c65 3e01 0000 0073 1a00 0000 0800 0801  le>....s........
-00000cf0: 2001 0c01 0c01 0c01 0c01 0c01 0c01 0c01   ...............
-00000d00: 0c01 0c01 1203                           ......
+00000090: 6407 6c11 6d12 5a12 6d13 5a13 0100 6400  d.l.m.Z.m.Z...d.
+000000a0: 6408 6c14 6d15 5a15 0100 6400 6409 6c16  d.l.m.Z...d.d.l.
+000000b0: 6d17 5a17 0100 6400 640a 6c18 6d19 5a19  m.Z...d.d.l.m.Z.
+000000c0: 0100 6400 640b 6c1a 6d1b 5a1b 0100 4700  ..d.d.l.m.Z...G.
+000000d0: 640c 640d 8400 640d 8302 5a1c 6401 5300  d.d...d...Z.d.S.
+000000e0: 290e e900 0000 004e 2906 da03 416e 79da  )......N)...Any.
+000000f0: 0843 616c 6c61 626c 65da 0444 6963 74da  .Callable..Dict.
+00000100: 044c 6973 74da 0843 6c61 7373 5661 72da  .List..ClassVar.
+00000110: 0554 7570 6c65 2901 da13 4675 6e63 7469  .Tuple)...Functi
+00000120: 6f6e 4465 636c 6172 6174 696f 6e29 01da  onDeclaration)..
+00000130: 0c46 756e 6374 696f 6e4c 6974 6529 01da  .FunctionLite)..
+00000140: 1373 656c 665f 7479 7065 5f69 665f 6578  .self_type_if_ex
+00000150: 6973 7473 2901 da10 7265 706c 6163 655f  ists)...replace_
+00000160: 6675 6e63 7469 6f6e 2902 da0f 496e 6665  function)...Infe
+00000170: 7265 6e63 6545 6e67 696e 65da 154d 616b  renceEngine..Mak
+00000180: 6549 6e66 6572 656e 6365 5265 7370 6f6e  eInferenceRespon
+00000190: 7365 2901 da05 4672 616d 6529 01da 1246  se)...Frame)...F
+000001a0: 756e 6374 696f 6e41 7474 7269 6275 7465  unctionAttribute
+000001b0: 7329 01da 1746 756e 6374 696f 6e44 6563  s)...FunctionDec
+000001c0: 6c61 7261 7469 6f6e 4c69 7465 2901 da08  larationLite)...
+000001d0: 7365 7474 696e 6773 6300 0000 0000 0000  settingsc.......
+000001e0: 0000 0000 0000 0000 0005 0000 0040 0000  .............@..
+000001f0: 0073 b400 0000 6500 5a01 6400 5a02 5500  .s....e.Z.d.Z.U.
+00000200: 6503 6504 6401 3c00 6401 6503 6402 6403  e.e.d.<.d.e.d.d.
+00000210: 6604 6404 6405 8404 5a05 6506 6402 6507  f.d.d...Z.e.d.e.
+00000220: 6602 6406 6407 8404 8301 5a08 6506 6402  f.d.d.....Z.e.d.
+00000230: 6509 6602 6408 6409 8404 8301 5a0a 640a  e.f.d.d.....Z.d.
+00000240: 650b 6402 650c 6604 640b 640c 8404 5a0d  e.d.e.f.d.d...Z.
+00000250: 6402 650b 6602 640d 640e 8404 5a0e 6418  d.e.f.d.d...Z.d.
+00000260: 640f 6410 8404 5a0f 640a 650b 6402 6403  d.d...Z.d.e.d.d.
+00000270: 6604 6411 6412 8404 5a10 6402 6511 6602  f.d.d...Z.d.e.f.
+00000280: 6413 6414 8404 5a12 6513 6401 6503 6415  d.d...Z.e.d.e.d.
+00000290: 6514 6602 1900 6402 6400 6604 6416 6417  e.f...d.d.f.d.d.
+000002a0: 8404 8301 5a15 6403 5300 2919 da10 5772  ....Z.d.S.)...Wr
+000002b0: 6974 6162 6c65 4675 6e63 7469 6f6e da04  itableFunction..
+000002c0: 6675 6e63 da06 7265 7475 726e 4e63 0200  func..returnNc..
+000002d0: 0000 0000 0000 0000 0000 0200 0000 0300  ................
+000002e0: 0000 4300 0000 731e 0000 0074 007c 0174  ..C...s....t.|.t
+000002f0: 016a 0283 0273 0a74 0364 0183 0182 017c  .j...s.t.d.....|
+00000300: 017c 005f 0464 0053 0029 024e 7563 0000  .|._.d.S.).Nuc..
+00000310: 004e 6f20 6672 616d 6520 666f 756e 642e  .No frame found.
+00000320: 204d 616b 6520 7375 7265 2074 6869 7320   Make sure this 
+00000330: 6973 2061 6e20 696e 6665 7272 6564 2066  is an inferred f
+00000340: 756e 6374 696f 6ee2 8094 6974 2073 686f  unction...it sho
+00000350: 756c 6420 7573 6520 636f 6465 7370 6561  uld use codespea
+00000360: 6b27 7320 4069 6e66 6572 2064 6563 6f72  k's @infer decor
+00000370: 6174 6f72 2905 da07 6861 7361 7474 7272  ator)...hasattrr
+00000380: 0f00 0000 da05 6672 616d 65da 0945 7863  ......frame..Exc
+00000390: 6570 7469 6f6e 7213 0000 0029 02da 0473  eptionr....)...s
+000003a0: 656c 6672 1300 0000 a900 7219 0000 00fa  elfr......r.....
+000003b0: 462f 5573 6572 732f 6e61 7468 616e 7368  F/Users/nathansh
+000003c0: 6972 6c65 792f 636f 6465 7370 6561 6b2f  irley/codespeak/
+000003d0: 636f 6465 7370 6561 6b2f 6675 6e63 7469  codespeak/functi
+000003e0: 6f6e 2f77 7269 7461 626c 655f 6675 6e63  on/writable_func
+000003f0: 7469 6f6e 2e70 79da 085f 5f69 6e69 745f  tion.py..__init_
+00000400: 5f12 0000 0073 0a00 0000 0c01 0201 0201  _....s..........
+00000410: 04ff 0a03 7a19 5772 6974 6162 6c65 4675  ....z.WritableFu
+00000420: 6e63 7469 6f6e 2e5f 5f69 6e69 745f 5f63  nction.__init__c
+00000430: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00000440: 0300 0000 4300 0000 730e 0000 0074 007c  ....C...s....t.|
+00000450: 006a 0174 026a 0383 0253 00a9 014e 2904  .j.t.j...S...N).
+00000460: da07 6765 7461 7474 7272 1300 0000 720f  ..getattrr....r.
+00000470: 0000 00da 0b64 6563 6c61 7261 7469 6f6e  .....declaration
+00000480: a901 7218 0000 0072 1900 0000 7219 0000  ..r....r....r...
+00000490: 0072 1a00 0000 721e 0000 0019 0000 0073  .r....r........s
+000004a0: 0200 0000 0e02 7a1c 5772 6974 6162 6c65  ......z.Writable
+000004b0: 4675 6e63 7469 6f6e 2e64 6563 6c61 7261  Function.declara
+000004c0: 7469 6f6e 6301 0000 0000 0000 0000 0000  tionc...........
+000004d0: 0001 0000 0003 0000 0043 0000 0073 0c00  .........C...s..
+000004e0: 0000 7400 a001 7c00 6a02 a101 5300 721c  ..t...|.j...S.r.
+000004f0: 0000 0029 0372 0e00 0000 5a0c 666f 725f  ...).r....Z.for_
+00000500: 6675 6e63 7469 6f6e 7213 0000 0072 1f00  functionr....r..
+00000510: 0000 7219 0000 0072 1900 0000 721a 0000  ..r....r....r...
+00000520: 0072 1600 0000 1d00 0000 7302 0000 000c  .r........s.....
+00000530: 027a 1657 7269 7461 626c 6546 756e 6374  .z.WritableFunct
+00000540: 696f 6e2e 6672 616d 65da 0b73 6f75 7263  ion.frame..sourc
+00000550: 655f 6669 6c65 6302 0000 0000 0000 0000  e_filec.........
+00000560: 0000 0006 0000 0004 0000 0043 0000 0073  ...........C...s
+00000570: 4a00 0000 7c00 a000 a100 7d02 7401 a002  J...|.....}.t...
+00000580: a100 7d03 7c03 6400 7500 7210 7403 6401  ..}.|.d.u.r.t.d.
+00000590: 8301 8201 7404 7c02 7c03 6402 8d02 7d04  ....t.|.|.d...}.
+000005a0: 7c04 6a05 7c01 6403 8d01 7d05 7c04 6a06  |.j.|.d...}.|.j.
+000005b0: 7c05 7c01 6404 8d02 0100 7c05 5300 2905  |.|.d.....|.S.).
+000005c0: 4e7a 2f4e 6f20 6170 6920 7365 742e 2041  Nz/No api set. A
+000005d0: 6464 2061 6e20 6170 6920 7769 7468 2063  dd an api with c
+000005e0: 6f64 6573 7065 616b 2e61 6464 5f61 7069  odespeak.add_api
+000005f0: 2829 2902 da0d 6675 6e63 7469 6f6e 5f6c  ())...function_l
+00000600: 6974 65da 0e61 7069 5f69 6465 6e74 6966  ite..api_identif
+00000610: 6965 72a9 0172 2000 0000 2902 da09 696e  ier..r ...)...in
+00000620: 6665 7265 6e63 6572 2000 0000 2907 da10  ferencer ...)...
+00000630: 746f 5f66 756e 6374 696f 6e5f 6c69 7465  to_function_lite
+00000640: 7211 0000 005a 1a67 6574 5f63 7572 7265  r....Z.get_curre
+00000650: 6e74 5f61 7069 5f69 6465 6e74 6966 6965  nt_api_identifie
+00000660: 72da 0a56 616c 7565 4572 726f 7272 0c00  r..ValueErrorr..
+00000670: 0000 da0e 6d61 6b65 5f69 6e66 6572 656e  ....make_inferen
+00000680: 6365 5a0f 7772 6974 655f 696e 6665 7265  ceZ.write_infere
+00000690: 6e63 6529 0672 1800 0000 7220 0000 0072  nce).r....r ...r
+000006a0: 2100 0000 7222 0000 005a 1069 6e66 6572  !...r"...Z.infer
+000006b0: 656e 6365 5f65 6e67 696e 6572 2400 0000  ence_enginer$...
+000006c0: 7219 0000 0072 1900 0000 721a 0000 00da  r....r....r.....
+000006d0: 195f 6d61 6b65 5f61 6e64 5f77 7269 7465  ._make_and_write
+000006e0: 5f69 6e66 6572 656e 6365 2100 0000 7316  _inference!...s.
+000006f0: 0000 0008 0108 0108 0108 0102 0102 0102  ................
+00000700: 0106 fe0c 040e 0104 017a 2a57 7269 7461  .........z*Writa
+00000710: 626c 6546 756e 6374 696f 6e2e 5f6d 616b  bleFunction._mak
+00000720: 655f 616e 645f 7772 6974 655f 696e 6665  e_and_write_infe
+00000730: 7265 6e63 6563 0100 0000 0000 0000 0000  rencec..........
+00000740: 0000 0200 0000 0300 0000 4300 0000 7320  ..........C...s 
+00000750: 0000 0074 00a0 017c 006a 02a1 017d 017c  ...t...|.j...}.|
+00000760: 0164 0075 0072 0e74 0364 0183 0182 017c  .d.u.r.t.d.....|
+00000770: 0153 0029 024e 7a22 4675 6e63 7469 6f6e  .S.).Nz"Function
+00000780: 206d 7573 7420 6265 2064 6566 696e 6564   must be defined
+00000790: 2069 6e20 6120 6669 6c65 2904 da07 696e   in a file)...in
+000007a0: 7370 6563 74da 0d67 6574 736f 7572 6365  spect..getsource
+000007b0: 6669 6c65 7213 0000 0072 2600 0000 2902  filer....r&...).
+000007c0: 7218 0000 005a 0266 6672 1900 0000 7219  r....Z.ffr....r.
+000007d0: 0000 0072 1a00 0000 7220 0000 002e 0000  ...r....r ......
+000007e0: 0073 0800 0000 0c01 0801 0801 0401 7a1c  .s............z.
+000007f0: 5772 6974 6162 6c65 4675 6e63 7469 6f6e  WritableFunction
+00000800: 2e73 6f75 7263 655f 6669 6c65 6301 0000  .source_filec...
+00000810: 0000 0000 0000 0000 0001 0000 0004 0000  ................
+00000820: 0043 0000 0073 1200 0000 7c00 a000 7c00  .C...s....|...|.
+00000830: a001 a100 a101 0100 6400 5300 721c 0000  ........d.S.r...
+00000840: 0029 02da 065f 7772 6974 6572 2000 0000  .)..._writer ...
+00000850: 721f 0000 0072 1900 0000 7219 0000 0072  r....r....r....r
+00000860: 1a00 0000 da05 7772 6974 6534 0000 0073  ......write4...s
+00000870: 0200 0000 1201 7a16 5772 6974 6162 6c65  ......z.Writable
+00000880: 4675 6e63 7469 6f6e 2e77 7269 7465 6302  Function.writec.
+00000890: 0000 0000 0000 0000 0000 0002 0000 0003  ................
+000008a0: 0000 0043 0000 0073 1000 0000 7c00 6a00  ...C...s....|.j.
+000008b0: 7c01 6401 8d01 0100 6400 5300 2902 4e72  |.d.....d.S.).Nr
+000008c0: 2300 0000 2901 7228 0000 0029 0272 1800  #...).r(...).r..
+000008d0: 0000 7220 0000 0072 1900 0000 7219 0000  ..r ...r....r...
+000008e0: 0072 1a00 0000 722b 0000 0037 0000 0073  .r....r+...7...s
+000008f0: 0200 0000 1001 7a17 5772 6974 6162 6c65  ......z.Writable
+00000900: 4675 6e63 7469 6f6e 2e5f 7772 6974 6563  Function._writec
+00000910: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00000920: 0400 0000 4300 0000 7318 0000 0074 007c  ....C...s....t.|
+00000930: 006a 01a0 02a1 007c 006a 03a0 04a1 0064  .j.....|.j.....d
+00000940: 018d 0253 0029 024e 2902 721e 0000 00da  ...S.).N).r.....
+00000950: 0c63 7573 746f 6d5f 7479 7065 7329 0572  .custom_types).r
+00000960: 0900 0000 721e 0000 005a 1374 6f5f 6465  ....r....Z.to_de
+00000970: 636c 6172 6174 696f 6e5f 6c69 7465 7216  claration_liter.
+00000980: 0000 0072 2d00 0000 721f 0000 0072 1900  ...r-...r....r..
+00000990: 0000 7219 0000 0072 1a00 0000 7225 0000  ..r....r....r%..
+000009a0: 003a 0000 0073 0800 0000 0201 0801 0801  .:...s..........
+000009b0: 06fe 7a21 5772 6974 6162 6c65 4675 6e63  ..z!WritableFunc
+000009c0: 7469 6f6e 2e74 6f5f 6675 6e63 7469 6f6e  tion.to_function
+000009d0: 5f6c 6974 652e 6301 0000 0000 0000 0000  _lite.c.........
+000009e0: 0000 0001 0000 0003 0000 0043 0000 0073  ...........C...s
+000009f0: 0a00 0000 7400 7c00 6401 8d01 5300 2902  ....t.|.d...S.).
+00000a00: 7a37 6765 7420 636c 6173 7369 6669 6564  z7get classified
+00000a10: 2046 756e 6374 696f 6e20 6f62 6a65 6374   Function object
+00000a20: 2066 6f72 2061 6e20 696e 6665 7272 6564   for an inferred
+00000a30: 2066 756e 6374 696f 6ea9 0172 1300 0000   function..r....
+00000a40: 2901 7212 0000 0072 2e00 0000 7219 0000  ).r....r....r...
+00000a50: 0072 1900 0000 721a 0000 00da 1466 726f  .r....r......fro
+00000a60: 6d5f 6675 6e63 7469 6f6e 5f6f 626a 6563  m_function_objec
+00000a70: 7440 0000 0073 0200 0000 0a03 7a25 5772  t@...s......z%Wr
+00000a80: 6974 6162 6c65 4675 6e63 7469 6f6e 2e66  itableFunction.f
+00000a90: 726f 6d5f 6675 6e63 7469 6f6e 5f6f 626a  rom_function_obj
+00000aa0: 6563 7429 0272 1400 0000 4e29 16da 085f  ect).r....N)..._
+00000ab0: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
+00000ac0: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
+00000ad0: 5f72 0300 0000 da0f 5f5f 616e 6e6f 7461  _r......__annota
+00000ae0: 7469 6f6e 735f 5f72 1b00 0000 da08 7072  tions__r......pr
+00000af0: 6f70 6572 7479 7208 0000 0072 1e00 0000  opertyr....r....
+00000b00: 720e 0000 0072 1600 0000 da03 7374 7272  r....r......strr
+00000b10: 0d00 0000 7228 0000 0072 2000 0000 722c  ....r(...r ...r,
+00000b20: 0000 0072 2b00 0000 7209 0000 0072 2500  ...r+...r....r%.
+00000b30: 0000 da0c 7374 6174 6963 6d65 7468 6f64  ....staticmethod
+00000b40: 7202 0000 0072 2f00 0000 7219 0000 0072  r....r/...r....r
+00000b50: 1900 0000 7219 0000 0072 1a00 0000 7212  ....r....r....r.
+00000b60: 0000 000f 0000 0073 1c00 0000 0a00 0801  .......s........
+00000b70: 1202 0207 1001 0203 1001 1203 0e0d 0a06  ................
+00000b80: 1203 0e03 0206 2001 7212 0000 0029 1d72  ...... .r....).r
+00000b90: 2900 0000 da04 6a73 6f6e da06 7479 7069  ).....json..typi
+00000ba0: 6e67 7202 0000 0072 0300 0000 7204 0000  ngr....r....r...
+00000bb0: 0072 0500 0000 7206 0000 0072 0700 0000  .r....r....r....
+00000bc0: 5a27 636f 6465 7370 6561 6b2e 6675 6e63  Z'codespeak.func
+00000bd0: 7469 6f6e 2e66 756e 6374 696f 6e5f 6465  tion.function_de
+00000be0: 636c 6172 6174 696f 6e72 0800 0000 da20  clarationr..... 
+00000bf0: 636f 6465 7370 6561 6b2e 6675 6e63 7469  codespeak.functi
+00000c00: 6f6e 2e66 756e 6374 696f 6e5f 6c69 7465  on.function_lite
+00000c10: 7209 0000 005a 1b63 6f64 6573 7065 616b  r....Z.codespeak
+00000c20: 2e68 656c 7065 7273 2e73 656c 665f 7479  .helpers.self_ty
+00000c30: 7065 720a 0000 005a 2463 6f64 6573 7065  per....Z$codespe
+00000c40: 616b 2e69 6e66 6572 656e 6365 2e72 6570  ak.inference.rep
+00000c50: 6c61 6365 5f66 756e 6374 696f 6e72 0b00  lace_functionr..
+00000c60: 0000 5a24 636f 6465 7370 6561 6b2e 696e  ..Z$codespeak.in
+00000c70: 6665 7265 6e63 652e 696e 6665 7265 6e63  ference.inferenc
+00000c80: 655f 656e 6769 6e65 720c 0000 0072 0d00  e_enginer....r..
+00000c90: 0000 5a0f 636f 6465 7370 6561 6b2e 6672  ..Z.codespeak.fr
+00000ca0: 616d 6572 0e00 0000 5a26 636f 6465 7370  amer....Z&codesp
+00000cb0: 6561 6b2e 6675 6e63 7469 6f6e 2e66 756e  eak.function.fun
+00000cc0: 6374 696f 6e5f 6174 7472 6962 7574 6573  ction_attributes
+00000cd0: 720f 0000 00da 2c63 6f64 6573 7065 616b  r.....,codespeak
+00000ce0: 2e66 756e 6374 696f 6e2e 6675 6e63 7469  .function.functi
+00000cf0: 6f6e 5f64 6563 6c61 7261 7469 6f6e 5f6c  on_declaration_l
+00000d00: 6974 6572 1000 0000 5a09 636f 6465 7370  iter....Z.codesp
+00000d10: 6561 6b72 1100 0000 7212 0000 0072 1900  eakr....r....r..
+00000d20: 0000 7219 0000 0072 1900 0000 721a 0000  ..r....r....r...
+00000d30: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
+00000d40: 1a00 0000 0800 0801 2001 0c01 0c01 0c01  ........ .......
+00000d50: 0c01 1001 0c01 0c01 0c01 0c01 1203       ..............
```

### Comparing `codespeak-0.1.5/codespeak/function/function_declaration.py` & `codespeak-0.1.6/codespeak/function/function_declaration.py`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/function/function_declaration_lite.py` & `codespeak-0.1.6/codespeak/function/function_declaration_lite.py`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/function/function_lite.py` & `codespeak-0.1.6/codespeak/function/function_lite.py`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/function/function_manager.py` & `codespeak-0.1.6/codespeak/function/function_manager.py`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/function/helper_types/__pycache__/make_inference_response.cpython-310.pyc` & `codespeak-0.1.6/codespeak/function/helper_types/__pycache__/make_inference_response.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/function/writable_function.py` & `codespeak-0.1.6/codespeak/function/writable_function.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import inspect
 import json
 from typing import Any, Callable, Dict, List, ClassVar, Tuple
 from codespeak.function.function_declaration import FunctionDeclaration
 from codespeak.function.function_lite import FunctionLite
 from codespeak.helpers.self_type import self_type_if_exists
-from codespeak.decorate.writable_transform import replace_function
-from codespeak.inference.inference_engine import InferenceEngine
+from codespeak.inference.replace_function import replace_function
+from codespeak.inference.inference_engine import InferenceEngine, MakeInferenceResponse
 from codespeak.frame import Frame
 from codespeak.function.function_attributes import FunctionAttributes
 from codespeak.function.function_declaration_lite import FunctionDeclarationLite
-from codespeak.settings import settings
+from codespeak import settings
 
 
 class WritableFunction:
     func: Callable
 
     def __init__(self, func: Callable) -> None:
         if not hasattr(func, FunctionAttributes.frame):
@@ -26,37 +26,38 @@
     def declaration(self) -> FunctionDeclaration:
         return getattr(self.func, FunctionAttributes.declaration)
 
     @property
     def frame(self) -> Frame:
         return Frame.for_function(self.func)
 
-    def _make_inference(self) -> str:
+    def _make_and_write_inference(self, source_file: str) -> MakeInferenceResponse:
         function_lite = self.to_function_lite()
         api_identifier = settings.get_current_api_identifier()
         if api_identifier is None:
             raise ValueError("No api set. Add an api with codespeak.add_api()")
-        api_inference_engine = InferenceEngine(
+        inference_engine = InferenceEngine(
             function_lite=function_lite,
             api_identifier=api_identifier,
         )
-        return api_inference_engine.make_inference()
+        inference = inference_engine.make_inference(source_file=source_file)
+        inference_engine.write_inference(inference=inference, source_file=source_file)
+        return inference
 
     def source_file(self) -> str:
         ff = inspect.getsourcefile(self.func)
         if ff is None:
             raise ValueError("Function must be defined in a file")
         return ff
 
     def write(self) -> None:
         self._write(self.source_file())
 
     def _write(self, source_file: str) -> None:
-        inference = self._make_inference()
-        replace_function(source_file, self.func.__qualname__, inference)
+        self._make_and_write_inference(source_file=source_file)
 
     def to_function_lite(self) -> FunctionLite:
         return FunctionLite(
             declaration=self.declaration.to_declaration_lite(),
             custom_types=self.frame.custom_types(),
         )
```

### Comparing `codespeak-0.1.5/codespeak/helpers/__pycache__/abspath_to_project_root.cpython-310.pyc` & `codespeak-0.1.6/codespeak/helpers/__pycache__/abspath_to_project_root.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/helpers/__pycache__/auto_detect_abspath_to_project_root.cpython-310.pyc` & `codespeak-0.1.6/codespeak/helpers/__pycache__/auto_detect_abspath_to_project_root.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/helpers/__pycache__/derive_module_qualname_for_object.cpython-310.pyc` & `codespeak-0.1.6/codespeak/helpers/__pycache__/derive_module_qualname_for_object.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Jul 26 18:49:48 2023 UTC, .py size: 1422 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 21% similar despite different names*

```diff
@@ -1,74 +1,73 @@
-00000000: 6f0d 0d0a 0000 0000 cc6a c164 8e05 0000  o........j.d....
+00000000: 6f0d 0d0a 0000 0000 7ac7 c264 8105 0000  o.......z..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 4c00 0000 6400  .....@...sL...d.
+00000020: 0004 0000 0040 0000 0073 4800 0000 6400  .....@...sH...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
-00000040: 6402 6c02 6d03 5a03 0100 6400 6403 6c04  d.l.m.Z...d.d.l.
-00000050: 6d05 5a05 0100 6404 6503 6602 6405 6406  m.Z...d.e.f.d.d.
-00000060: 8404 5a06 6407 6507 6408 6507 6604 6409  ..Z.d.e.d.e.f.d.
-00000070: 640a 8404 5a08 6401 5300 290b e900 0000  d...Z.d.S.).....
-00000080: 004e 2901 da03 416e 7929 01da 0873 6574  .N)...Any)...set
-00000090: 7469 6e67 73da 075f 6f62 6a65 6374 6301  tings.._objectc.
-000000a0: 0000 0000 0000 0000 0000 0002 0000 0004  ................
-000000b0: 0000 0043 0000 0073 2800 0000 7400 a001  ...C...s(...t...
-000000c0: 7c00 a101 7d01 7c01 730d 7402 6401 7c00  |...}.|.s.t.d.|.
-000000d0: 6a03 8302 8201 7404 7c01 7405 a006 a100  j.....t.|.t.....
-000000e0: 8302 5300 2902 7a18 5368 6f75 6c64 2062  ..S.).z.Should b
-000000f0: 6520 6120 6c6f 6361 6c20 6f62 6a65 6374  e a local object
-00000100: 7a24 756e 6162 6c65 2074 6f20 6765 7420  z$unable to get 
-00000110: 736f 7572 6365 2066 696c 6520 666f 7220  source file for 
-00000120: 6675 6e63 3a20 2907 da07 696e 7370 6563  func: )...inspec
-00000130: 74da 0d67 6574 736f 7572 6365 6669 6c65  t..getsourcefile
-00000140: da09 4578 6365 7074 696f 6eda 085f 5f6e  ..Exception..__n
-00000150: 616d 655f 5fda 2564 6572 6976 655f 6d6f  ame__.%derive_mo
-00000160: 6475 6c65 5f71 7561 6c6e 616d 655f 6672  dule_qualname_fr
-00000170: 6f6d 5f66 696c 6570 6174 6873 7203 0000  om_filepathsr...
-00000180: 005a 1b67 6574 5f61 6273 7061 7468 5f74  .Z.get_abspath_t
-00000190: 6f5f 7072 6f6a 6563 745f 726f 6f74 2902  o_project_root).
-000001a0: 7204 0000 00da 0b73 6f75 7263 655f 6669  r......source_fi
-000001b0: 6c65 a900 720b 0000 00fa 552f 5573 6572  le..r.....U/User
-000001c0: 732f 6e61 7468 616e 7368 6972 6c65 792f  s/nathanshirley/
-000001d0: 636f 6465 7370 6561 6b2f 636f 6465 7370  codespeak/codesp
-000001e0: 6561 6b2f 6865 6c70 6572 732f 6465 7269  eak/helpers/deri
-000001f0: 7665 5f6d 6f64 756c 655f 7175 616c 6e61  ve_module_qualna
-00000200: 6d65 5f66 6f72 5f6f 626a 6563 742e 7079  me_for_object.py
-00000210: da21 6465 7269 7665 5f6d 6f64 756c 655f  .!derive_module_
-00000220: 7175 616c 6e61 6d65 5f66 6f72 5f6f 626a  qualname_for_obj
-00000230: 6563 7408 0000 0073 0c00 0000 0a02 0401  ect....s........
-00000240: 0c01 0201 0801 04ff 720d 0000 00da 1464  ........r......d
-00000250: 6563 6c61 7261 7469 6f6e 5f66 696c 6570  eclaration_filep
-00000260: 6174 68da 0c70 726f 6a65 6374 5f72 6f6f  ath..project_roo
-00000270: 7463 0200 0000 0000 0000 0000 0000 0500  tc..............
-00000280: 0000 0500 0000 4300 0000 7386 0000 0074  ......C...s....t
-00000290: 006a 01a0 0274 006a 01a0 037c 00a1 01a1  .j...t.j...|....
-000002a0: 017d 0274 006a 01a0 0274 006a 01a0 037c  .}.t.j...t.j...|
-000002b0: 01a1 01a1 017d 017c 02a0 047c 01a1 0173  .....}.|...|...s
-000002c0: 1d74 0564 0183 0182 0174 006a 01a0 067c  .t.d.....t.j...|
-000002d0: 027c 01a1 027d 0374 006a 01a0 077c 03a1  .|...}.t.j...|..
-000002e0: 0164 0219 007d 047c 04a0 0874 006a 0964  .d...}.|...t.j.d
-000002f0: 03a1 027d 047c 04a0 0a64 04a1 0172 417c  ...}.|...d...rA|
-00000300: 0464 0074 0b64 0483 010b 0085 0219 007d  .d.t.d.........}
-00000310: 047c 0453 0029 054e 7a2c 5468 6520 6669  .|.S.).Nz,The fi
-00000320: 6c65 7061 7468 206d 7573 7420 6265 2069  lepath must be i
-00000330: 6e73 6964 6520 7468 6520 7072 6f6a 6563  nside the projec
-00000340: 7420 726f 6f74 7201 0000 00da 012e 7a09  t rootr.......z.
-00000350: 2e5f 5f69 6e69 745f 5f29 0cda 026f 73da  .__init__)...os.
-00000360: 0470 6174 68da 086e 6f72 6d70 6174 68da  .path..normpath.
-00000370: 0761 6273 7061 7468 da0a 7374 6172 7473  .abspath..starts
-00000380: 7769 7468 da0a 5661 6c75 6545 7272 6f72  with..ValueError
-00000390: da07 7265 6c70 6174 68da 0873 706c 6974  ..relpath..split
-000003a0: 6578 74da 0772 6570 6c61 6365 da03 7365  ext..replace..se
-000003b0: 70da 0865 6e64 7377 6974 68da 036c 656e  p..endswith..len
-000003c0: 2905 720e 0000 0072 0f00 0000 da08 6669  ).r....r......fi
-000003d0: 6c65 7061 7468 5a08 7265 6c5f 7061 7468  lepathZ.rel_path
-000003e0: 5a0f 6d6f 6475 6c65 5f71 7561 6c6e 616d  Z.module_qualnam
-000003f0: 6572 0b00 0000 720b 0000 0072 0c00 0000  er....r....r....
-00000400: 7209 0000 0012 0000 0073 1400 0000 1402  r........s......
-00000410: 1401 0a03 0801 0e03 1003 0e03 0a03 1201  ................
-00000420: 0402 7209 0000 0029 0972 0500 0000 7211  ..r....).r....r.
-00000430: 0000 00da 0674 7970 696e 6772 0200 0000  .....typingr....
-00000440: da12 636f 6465 7370 6561 6b2e 7365 7474  ..codespeak.sett
-00000450: 696e 6773 7203 0000 0072 0d00 0000 da03  ingsr....r......
-00000460: 7374 7272 0900 0000 720b 0000 0072 0b00  strr....r....r..
-00000470: 0000 720b 0000 0072 0c00 0000 da08 3c6d  ..r....r......<m
-00000480: 6f64 756c 653e 0100 0000 730c 0000 0008  odule>....s.....
-00000490: 0008 010c 010c 020e 0316 0a              ...........
+00000040: 6402 6c02 6d03 5a03 0100 6400 6401 6c04  d.l.m.Z...d.d.l.
+00000050: 5a04 6403 6503 6602 6404 6405 8404 5a05  Z.d.e.f.d.d...Z.
+00000060: 6406 6506 6407 6506 6604 6408 6409 8404  d.e.d.e.f.d.d...
+00000070: 5a07 6401 5300 290a e900 0000 004e 2901  Z.d.S.)......N).
+00000080: da03 416e 79da 075f 6f62 6a65 6374 6301  ..Any.._objectc.
+00000090: 0000 0000 0000 0000 0000 0002 0000 0004  ................
+000000a0: 0000 0043 0000 0073 2a00 0000 7400 a001  ...C...s*...t...
+000000b0: 7c00 a101 7d01 7c01 730d 7402 6401 7c00  |...}.|.s.t.d.|.
+000000c0: 6a03 8302 8201 7404 7c01 7405 6a06 a007  j.....t.|.t.j...
+000000d0: a100 8302 5300 2902 7a18 5368 6f75 6c64  ....S.).z.Should
+000000e0: 2062 6520 6120 6c6f 6361 6c20 6f62 6a65   be a local obje
+000000f0: 6374 7a24 756e 6162 6c65 2074 6f20 6765  ctz$unable to ge
+00000100: 7420 736f 7572 6365 2066 696c 6520 666f  t source file fo
+00000110: 7220 6675 6e63 3a20 2908 da07 696e 7370  r func: )...insp
+00000120: 6563 74da 0d67 6574 736f 7572 6365 6669  ect..getsourcefi
+00000130: 6c65 da09 4578 6365 7074 696f 6eda 085f  le..Exception.._
+00000140: 5f6e 616d 655f 5fda 2564 6572 6976 655f  _name__.%derive_
+00000150: 6d6f 6475 6c65 5f71 7561 6c6e 616d 655f  module_qualname_
+00000160: 6672 6f6d 5f66 696c 6570 6174 6873 da09  from_filepaths..
+00000170: 636f 6465 7370 6561 6bda 0873 6574 7469  codespeak..setti
+00000180: 6e67 735a 1b67 6574 5f61 6273 7061 7468  ngsZ.get_abspath
+00000190: 5f74 6f5f 7072 6f6a 6563 745f 726f 6f74  _to_project_root
+000001a0: 2902 7203 0000 00da 0b73 6f75 7263 655f  ).r......source_
+000001b0: 6669 6c65 a900 720c 0000 00fa 552f 5573  file..r.....U/Us
+000001c0: 6572 732f 6e61 7468 616e 7368 6972 6c65  ers/nathanshirle
+000001d0: 792f 636f 6465 7370 6561 6b2f 636f 6465  y/codespeak/code
+000001e0: 7370 6561 6b2f 6865 6c70 6572 732f 6465  speak/helpers/de
+000001f0: 7269 7665 5f6d 6f64 756c 655f 7175 616c  rive_module_qual
+00000200: 6e61 6d65 5f66 6f72 5f6f 626a 6563 742e  name_for_object.
+00000210: 7079 da21 6465 7269 7665 5f6d 6f64 756c  py.!derive_modul
+00000220: 655f 7175 616c 6e61 6d65 5f66 6f72 5f6f  e_qualname_for_o
+00000230: 626a 6563 7408 0000 0073 0c00 0000 0a02  bject....s......
+00000240: 0401 0c01 0201 0a01 04ff 720e 0000 00da  ..........r.....
+00000250: 1464 6563 6c61 7261 7469 6f6e 5f66 696c  .declaration_fil
+00000260: 6570 6174 68da 0c70 726f 6a65 6374 5f72  epath..project_r
+00000270: 6f6f 7463 0200 0000 0000 0000 0000 0000  ootc............
+00000280: 0500 0000 0500 0000 4300 0000 7386 0000  ........C...s...
+00000290: 0074 006a 01a0 0274 006a 01a0 037c 00a1  .t.j...t.j...|..
+000002a0: 01a1 017d 0274 006a 01a0 0274 006a 01a0  ...}.t.j...t.j..
+000002b0: 037c 01a1 01a1 017d 017c 02a0 047c 01a1  .|.....}.|...|..
+000002c0: 0173 1d74 0564 0183 0182 0174 006a 01a0  .s.t.d.....t.j..
+000002d0: 067c 027c 01a1 027d 0374 006a 01a0 077c  .|.|...}.t.j...|
+000002e0: 03a1 0164 0219 007d 047c 04a0 0874 006a  ...d...}.|...t.j
+000002f0: 0964 03a1 027d 047c 04a0 0a64 04a1 0172  .d...}.|...d...r
+00000300: 417c 0464 0074 0b64 0483 010b 0085 0219  A|.d.t.d........
+00000310: 007d 047c 0453 0029 054e 7a2c 5468 6520  .}.|.S.).Nz,The 
+00000320: 6669 6c65 7061 7468 206d 7573 7420 6265  filepath must be
+00000330: 2069 6e73 6964 6520 7468 6520 7072 6f6a   inside the proj
+00000340: 6563 7420 726f 6f74 7201 0000 00da 012e  ect rootr.......
+00000350: 7a09 2e5f 5f69 6e69 745f 5f29 0cda 026f  z..__init__)...o
+00000360: 73da 0470 6174 68da 086e 6f72 6d70 6174  s..path..normpat
+00000370: 68da 0761 6273 7061 7468 da0a 7374 6172  h..abspath..star
+00000380: 7473 7769 7468 da0a 5661 6c75 6545 7272  tswith..ValueErr
+00000390: 6f72 da07 7265 6c70 6174 68da 0873 706c  or..relpath..spl
+000003a0: 6974 6578 74da 0772 6570 6c61 6365 da03  itext..replace..
+000003b0: 7365 70da 0865 6e64 7377 6974 68da 036c  sep..endswith..l
+000003c0: 656e 2905 720f 0000 0072 1000 0000 da08  en).r....r......
+000003d0: 6669 6c65 7061 7468 5a08 7265 6c5f 7061  filepathZ.rel_pa
+000003e0: 7468 5a0f 6d6f 6475 6c65 5f71 7561 6c6e  thZ.module_qualn
+000003f0: 616d 6572 0c00 0000 720c 0000 0072 0d00  amer....r....r..
+00000400: 0000 7208 0000 0012 0000 0073 1400 0000  ..r........s....
+00000410: 1402 1401 0a03 0801 0e03 1003 0e03 0a03  ................
+00000420: 1201 0402 7208 0000 0029 0872 0400 0000  ....r....).r....
+00000430: 7212 0000 00da 0674 7970 696e 6772 0200  r......typingr..
+00000440: 0000 7209 0000 0072 0e00 0000 da03 7374  ..r....r......st
+00000450: 7272 0800 0000 720c 0000 0072 0c00 0000  rr....r....r....
+00000460: 720c 0000 0072 0d00 0000 da08 3c6d 6f64  r....r......<mod
+00000470: 756c 653e 0100 0000 730c 0000 0008 0008  ule>....s.......
+00000480: 010c 0108 020e 0316 0a                   .........
```

### Comparing `codespeak-0.1.5/codespeak/helpers/__pycache__/extract_delimited_python_code_from_string.cpython-310.pyc` & `codespeak-0.1.6/codespeak/helpers/__pycache__/extract_delimited_python_code_from_string.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/helpers/__pycache__/gather_arguments.cpython-310.pyc` & `codespeak-0.1.6/codespeak/helpers/__pycache__/gather_arguments.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/helpers/__pycache__/get_attr_from_qualname.cpython-310.pyc` & `codespeak-0.1.6/codespeak/helpers/__pycache__/get_attr_from_qualname.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/helpers/__pycache__/get_definitions_from_function_object.cpython-310.pyc` & `codespeak-0.1.6/codespeak/helpers/__pycache__/get_definitions_from_function_object.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/helpers/__pycache__/get_definitions_from_function_signature.cpython-310.pyc` & `codespeak-0.1.6/codespeak/helpers/__pycache__/get_definitions_from_function_signature.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/helpers/__pycache__/self_type.cpython-310.pyc` & `codespeak-0.1.6/codespeak/helpers/__pycache__/self_type.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/helpers/__pycache__/set_attr_for_qualname.cpython-310.pyc` & `codespeak-0.1.6/codespeak/helpers/__pycache__/set_attr_for_qualname.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/helpers/__pycache__/try_get_self_class_object_for_function.cpython-310.pyc` & `codespeak-0.1.6/codespeak/helpers/__pycache__/try_get_self_class_object_for_function.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/helpers/__pycache__/try_get_self_definition_for_for_inferred_function.cpython-310.pyc` & `codespeak-0.1.6/codespeak/helpers/__pycache__/try_get_self_definition_for_for_inferred_function.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/helpers/auto_detect_abspath_to_project_root.py` & `codespeak-0.1.6/codespeak/helpers/auto_detect_abspath_to_project_root.py`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/helpers/derive_module_qualname_for_object.py` & `codespeak-0.1.6/codespeak/helpers/derive_module_qualname_for_object.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import inspect
 import os
 from typing import Any
 
-from codespeak.settings import settings
+import codespeak
 
 
 def derive_module_qualname_for_object(_object: Any):
     """Should be a local object"""
     source_file = inspect.getsourcefile(_object)
     if not source_file:
         raise Exception("unable to get source file for func: ", _object.__name__)
     return derive_module_qualname_from_filepaths(
-        source_file, settings.get_abspath_to_project_root()
+        source_file, codespeak.settings.get_abspath_to_project_root()
     )
 
 
 def derive_module_qualname_from_filepaths(declaration_filepath: str, project_root: str):
     # Make sure both paths are absolute and normalized
     filepath = os.path.normpath(os.path.abspath(declaration_filepath))
     project_root = os.path.normpath(os.path.abspath(project_root))
```

### Comparing `codespeak-0.1.5/codespeak/helpers/get_definitions_from_function_object.py` & `codespeak-0.1.6/codespeak/helpers/get_definitions_from_function_object.py`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/helpers/self_type.py` & `codespeak-0.1.6/codespeak/helpers/self_type.py`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/helpers/try_get_self_definition_for_for_inferred_function.py` & `codespeak-0.1.6/codespeak/helpers/try_get_self_definition_for_for_inferred_function.py`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/inference/__pycache__/api_inference_engine.cpython-310.pyc` & `codespeak-0.1.6/codespeak/inference/__pycache__/api_inference_engine.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/inference/__pycache__/code_generator.cpython-310.pyc` & `codespeak-0.1.6/codespeak/inference/__pycache__/code_generator.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/inference/__pycache__/diff.cpython-310.pyc` & `codespeak-0.1.6/codespeak/inference/__pycache__/diff.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/inference/__pycache__/execute.cpython-310.pyc` & `codespeak-0.1.6/codespeak/inference/__pycache__/execute.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/inference/__pycache__/executor.cpython-310.pyc` & `codespeak-0.1.6/codespeak/inference/__pycache__/executor.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/inference/__pycache__/openai_service.cpython-310.pyc` & `codespeak-0.1.6/codespeak/inference/__pycache__/openai_service.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/inference/__pycache__/prompt.cpython-310.pyc` & `codespeak-0.1.6/codespeak/inference/__pycache__/prompt.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/inference/__pycache__/results_collector.cpython-310.pyc` & `codespeak-0.1.6/codespeak/inference/__pycache__/results_collector.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/interactive_mode/__pycache__/get_approval.cpython-310.pyc` & `codespeak-0.1.6/codespeak/interactive_mode/__pycache__/get_approval.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/interactive_mode/get_approval.py` & `codespeak-0.1.6/codespeak/interactive_mode/get_approval.py`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/module_frame.py` & `codespeak-0.1.6/codespeak/module_frame.py`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/public/__pycache__/codespeak_settings.cpython-310.pyc` & `codespeak-0.1.6/codespeak/public/__pycache__/codespeak_settings.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/public/__pycache__/generated_exception.cpython-310.pyc` & `codespeak-0.1.6/codespeak/public/__pycache__/generated_exception.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/public/__pycache__/inferred_exception.cpython-310.pyc` & `codespeak-0.1.6/codespeak/public/__pycache__/inferred_exception.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/public/__pycache__/settings.cpython-310.pyc` & `codespeak-0.1.6/codespeak/public/__pycache__/settings.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/public/inferred_exception.py` & `codespeak-0.1.6/codespeak/public/inferred_exception.py`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/public/rest_requests/__pycache__/delete.cpython-310.pyc` & `codespeak-0.1.6/codespeak/public/rest_requests/__pycache__/delete.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/public/rest_requests/__pycache__/get.cpython-310.pyc` & `codespeak-0.1.6/codespeak/public/rest_requests/__pycache__/get.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Jul 26 15:21:30 2023 UTC, .py size: 1583 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,107 +1,107 @@
-00000000: 6f0d 0d0a 0000 0000 fa39 c164 2f06 0000  o........9.d/...
+00000000: 6f0d 0d0a 0000 0000 f0cc c264 3206 0000  o..........d2...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000d 0000 0040 0000 0073 9600 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 0100 6400 6402 6c04 5a04 6400 6403 6c05  ..d.d.l.Z.d.d.l.
 00000050: 6d05 5a05 0100 6400 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6405 6c08 6d09 5a09 0100 6400  ..d.d.l.m.Z...d.
 00000070: 6406 6c0a 6d0b 5a0b 0100 6402 6402 6900  d.l.m.Z...d.d.i.
 00000080: 6603 6407 650c 6408 650c 6409 6501 650c  f.d.e.d.e.d.e.e.
 00000090: 6503 6602 1900 6402 4200 640a 6501 650c  e.f...d.B.d.e.e.
 000000a0: 6503 6602 1900 6402 4200 640b 6501 650c  e.f...d.B.d.e.e.
 000000b0: 6503 6602 1900 660a 640c 640d 8405 5a0d  e.f...f.d.d...Z.
 000000c0: 6402 5300 290e e900 0000 0029 03da 0444  d.S.)......)...D
 000000d0: 6963 74da 044c 6973 74da 0341 6e79 4e29  ict..List..AnyN)
-000000e0: 01da 0466 7572 6c29 01da 0861 7069 5f6b  ...furl)...api_k
-000000f0: 6579 7329 01da 1149 6e66 6572 7265 6445  eys)...InferredE
-00000100: 7863 6570 7469 6f6e 2901 da07 5265 7175  xception)...Requ
-00000110: 6573 74da 0361 7069 da04 7061 7468 da0b  est..api..path..
-00000120: 7061 7468 5f70 6172 616d 73da 0c71 7565  path_params..que
-00000130: 7279 5f70 6172 616d 73da 0768 6561 6465  ry_params..heade
-00000140: 7273 6305 0000 0000 0000 0000 0000 0008  rsc.............
-00000150: 0000 000b 0000 0043 0000 0073 6e00 0000  .......C...sn...
-00000160: 7400 7c00 7c01 6401 7c02 7c03 6401 6401  t.|.|.d.|.|.d.d.
-00000170: 6401 7c04 6402 8d09 7d05 7c05 a001 a100  d.|.d...}.|.....
-00000180: 0100 7402 6a03 7c05 a004 a100 7c05 6a05  ..t.j.|.....|.j.
-00000190: 7c05 6a06 6403 8d03 7d06 7a09 7c06 a007  |.j.d...}.z.|...
-000001a0: a100 0100 5700 7c06 a00a a100 5300 0400  ....W.|.....S...
-000001b0: 7402 6a08 6a09 7936 0100 7d07 0100 7a02  t.j.j.y6..}...z.
-000001c0: 7c07 8201 6401 7d07 7e07 7701 7700 2904  |...d.}.~.w.w.).
-000001d0: 6172 0200 000a 2020 2020 4d61 6b65 7320  ar....    Makes 
-000001e0: 6120 6765 7420 7265 7175 6573 7420 746f  a get request to
-000001f0: 2061 6e20 6170 6920 7769 7468 2061 7574   an api with aut
-00000200: 6f6d 6174 6963 2061 7574 6865 6e74 6963  omatic authentic
-00000210: 6174 696f 6e20 616e 6420 666f 726d 6174  ation and format
-00000220: 7465 6420 7061 7261 6d73 2e20 4e6f 2061  ted params. No a
-00000230: 7069 206b 6579 7320 7265 7175 6972 6564  pi keys required
-00000240: 2e0a 0a20 2020 2041 7267 733a 0a20 2020  ...    Args:.   
-00000250: 2020 2020 2061 7069 2028 7374 7229 3a20       api (str): 
-00000260: 5468 6520 6e61 6d65 206f 6620 7468 6520  The name of the 
-00000270: 6170 6920 746f 2075 7365 2e0a 2020 2020  api to use..    
-00000280: 2020 2020 7061 7468 2028 7374 7229 3a20      path (str): 
-00000290: 5468 6520 6f70 656e 6170 6920 7061 7468  The openapi path
-000002a0: 2066 6f72 2074 6865 206f 7065 7261 7469   for the operati
-000002b0: 6f6e 2e0a 2020 2020 2020 2020 7061 7468  on..        path
-000002c0: 5f70 6172 616d 7320 2844 6963 745b 7374  _params (Dict[st
-000002d0: 722c 2073 7472 5d2c 206f 7074 696f 6e61  r, str], optiona
-000002e0: 6c29 3a20 5468 6520 7061 7468 2070 6172  l): The path par
-000002f0: 616d 6574 6572 7320 746f 2075 7365 2069  ameters to use i
-00000300: 6e20 7468 6520 6f70 6572 6174 696f 6e2e  n the operation.
-00000310: 2044 6566 6175 6c74 7320 746f 204e 6f6e   Defaults to Non
-00000320: 652e 0a20 2020 2020 2020 2071 7565 7279  e..        query
-00000330: 5f70 6172 616d 7320 2844 6963 745b 7374  _params (Dict[st
-00000340: 722c 2073 7472 5d2c 206f 7074 696f 6e61  r, str], optiona
-00000350: 6c29 3a20 5468 6520 7175 6572 7920 7061  l): The query pa
-00000360: 7261 6d65 7465 7273 2074 6f20 7573 6520  rameters to use 
-00000370: 696e 2074 6865 206f 7065 7261 7469 6f6e  in the operation
-00000380: 2e20 4465 6661 756c 7473 2074 6f20 4e6f  . Defaults to No
-00000390: 6e65 2e0a 2020 2020 2020 2020 6865 6164  ne..        head
-000003a0: 6572 7320 2844 6963 745b 7374 722c 2073  ers (Dict[str, s
-000003b0: 7472 5d2c 206f 7074 696f 6e61 6c29 3a20  tr], optional): 
-000003c0: 5468 6520 6865 6164 6572 7320 746f 2075  The headers to u
-000003d0: 7365 2069 6e20 7468 6520 6f70 6572 6174  se in the operat
-000003e0: 696f 6e2e 2044 6566 6175 6c74 7320 746f  ion. Defaults to
-000003f0: 207b 7d2e 0a0a 2020 2020 5265 7475 726e   {}...    Return
-00000400: 733a 0a20 2020 2020 2020 2074 7970 653a  s:.        type:
-00000410: 2074 6865 206a 736f 6e2d 656e 636f 6465   the json-encode
-00000420: 6420 636f 6e74 656e 7420 6f66 2074 6865  d content of the
-00000430: 2072 6573 706f 6e73 652c 2069 6620 616e   response, if an
-00000440: 792e 0a20 2020 204e 2909 7209 0000 0072  y..    N).r....r
-00000450: 0a00 0000 da07 6170 695f 6b65 7972 0b00  ......api_keyr..
-00000460: 0000 720c 0000 00da 0464 6174 615a 056a  ..r......dataZ.j
-00000470: 736f 6e5f da07 636f 6f6b 6965 7372 0d00  son_..cookiesr..
-00000480: 0000 2903 da03 7572 6cda 0670 6172 616d  ..)...url..param
-00000490: 7372 0d00 0000 290b 7208 0000 005a 0c61  sr....).r....Z.a
-000004a0: 7574 6865 6e74 6963 6174 65da 0872 6571  uthenticate..req
-000004b0: 7565 7374 73da 0367 6574 5a08 6d61 6b65  uests..getZ.make
-000004c0: 5f75 726c 720c 0000 0072 0d00 0000 da10  _urlr....r......
-000004d0: 7261 6973 655f 666f 725f 7374 6174 7573  raise_for_status
-000004e0: da0a 6578 6365 7074 696f 6e73 da09 4854  ..exceptions..HT
-000004f0: 5450 4572 726f 72da 046a 736f 6e29 0872  TPError..json).r
-00000500: 0900 0000 720a 0000 0072 0b00 0000 720c  ....r....r....r.
-00000510: 0000 0072 0d00 0000 da07 7265 7175 6573  ...r......reques
-00000520: 74da 0872 6573 706f 6e73 65da 0165 a900  t..response..e..
-00000530: 721c 0000 00fa 442f 5573 6572 732f 6e61  r.....D/Users/na
-00000540: 7468 616e 7368 6972 6c65 792f 636f 6465  thanshirley/code
-00000550: 7370 6561 6b2f 636f 6465 7370 6561 6b2f  speak/codespeak/
-00000560: 7075 626c 6963 2f72 6573 745f 7265 7175  public/rest_requ
-00000570: 6573 7473 2f67 6574 2e70 7972 1400 0000  ests/get.pyr....
-00000580: 0900 0000 7330 0000 0002 1402 0102 0102  ....s0..........
-00000590: 0102 0102 0102 0102 0102 0102 0106 f708  ................
-000005a0: 0b04 0106 0104 0104 0106 fd02 050a 0108  ................
-000005b0: 0312 fe04 0108 8002 ff72 1400 0000 290e  .........r....).
-000005c0: da06 7479 7069 6e67 7202 0000 0072 0300  ..typingr....r..
-000005d0: 0000 7204 0000 0072 1300 0000 7205 0000  ..r....r....r...
-000005e0: 005a 0e63 6f64 6573 7065 616b 2e61 7069  .Z.codespeak.api
-000005f0: 7372 0600 0000 da23 636f 6465 7370 6561  sr.....#codespea
-00000600: 6b2e 7075 626c 6963 2e69 6e66 6572 7265  k.public.inferre
-00000610: 645f 6578 6365 7074 696f 6e72 0700 0000  d_exceptionr....
-00000620: 5a26 636f 6465 7370 6561 6b2e 7075 626c  Z&codespeak.publ
-00000630: 6963 2e72 6573 745f 7265 7175 6573 7473  ic.rest_requests
-00000640: 2e72 6571 7565 7374 7208 0000 00da 0373  .requestr......s
-00000650: 7472 7214 0000 0072 1c00 0000 721c 0000  trr....r....r...
-00000660: 0072 1c00 0000 721d 0000 00da 083c 6d6f  .r....r......<mo
-00000670: 6475 6c65 3e01 0000 0073 2800 0000 1400  dule>....s(.....
-00000680: 0801 0c01 0c01 0c01 0c01 0206 0201 0201  ................
-00000690: 04fb 0201 02ff 0202 02fe 0e03 02fd 0e04  ................
-000006a0: 02fc 0a05 0efb                           ......
+000000e0: 01da 0466 7572 6c29 01da 0b67 6574 5f61  ...furl)...get_a
+000000f0: 7069 5f6b 6579 2901 da11 496e 6665 7272  pi_key)...Inferr
+00000100: 6564 4578 6365 7074 696f 6e29 01da 0752  edException)...R
+00000110: 6571 7565 7374 da03 6170 69da 0470 6174  equest..api..pat
+00000120: 68da 0b70 6174 685f 7061 7261 6d73 da0c  h..path_params..
+00000130: 7175 6572 795f 7061 7261 6d73 da07 6865  query_params..he
+00000140: 6164 6572 7363 0500 0000 0000 0000 0000  adersc..........
+00000150: 0000 0800 0000 0b00 0000 4300 0000 736e  ..........C...sn
+00000160: 0000 0074 007c 007c 0164 017c 027c 0364  ...t.|.|.d.|.|.d
+00000170: 0164 0164 017c 0464 028d 097d 057c 05a0  .d.d.|.d...}.|..
+00000180: 01a1 0001 0074 026a 037c 05a0 04a1 007c  .....t.j.|.....|
+00000190: 056a 057c 056a 0664 038d 037d 067a 097c  .j.|.j.d...}.z.|
+000001a0: 06a0 07a1 0001 0057 007c 06a0 0aa1 0053  .......W.|.....S
+000001b0: 0004 0074 026a 086a 0979 3601 007d 0701  ...t.j.j.y6..}..
+000001c0: 007a 027c 0782 0164 017d 077e 0777 0177  .z.|...d.}.~.w.w
+000001d0: 0029 0461 7202 0000 0a20 2020 204d 616b  .).ar....    Mak
+000001e0: 6573 2061 2067 6574 2072 6571 7565 7374  es a get request
+000001f0: 2074 6f20 616e 2061 7069 2077 6974 6820   to an api with 
+00000200: 6175 746f 6d61 7469 6320 6175 7468 656e  automatic authen
+00000210: 7469 6361 7469 6f6e 2061 6e64 2066 6f72  tication and for
+00000220: 6d61 7474 6564 2070 6172 616d 732e 204e  matted params. N
+00000230: 6f20 6170 6920 6b65 7973 2072 6571 7569  o api keys requi
+00000240: 7265 642e 0a0a 2020 2020 4172 6773 3a0a  red...    Args:.
+00000250: 2020 2020 2020 2020 6170 6920 2873 7472          api (str
+00000260: 293a 2054 6865 206e 616d 6520 6f66 2074  ): The name of t
+00000270: 6865 2061 7069 2074 6f20 7573 652e 0a20  he api to use.. 
+00000280: 2020 2020 2020 2070 6174 6820 2873 7472         path (str
+00000290: 293a 2054 6865 206f 7065 6e61 7069 2070  ): The openapi p
+000002a0: 6174 6820 666f 7220 7468 6520 6f70 6572  ath for the oper
+000002b0: 6174 696f 6e2e 0a20 2020 2020 2020 2070  ation..        p
+000002c0: 6174 685f 7061 7261 6d73 2028 4469 6374  ath_params (Dict
+000002d0: 5b73 7472 2c20 7374 725d 2c20 6f70 7469  [str, str], opti
+000002e0: 6f6e 616c 293a 2054 6865 2070 6174 6820  onal): The path 
+000002f0: 7061 7261 6d65 7465 7273 2074 6f20 7573  parameters to us
+00000300: 6520 696e 2074 6865 206f 7065 7261 7469  e in the operati
+00000310: 6f6e 2e20 4465 6661 756c 7473 2074 6f20  on. Defaults to 
+00000320: 4e6f 6e65 2e0a 2020 2020 2020 2020 7175  None..        qu
+00000330: 6572 795f 7061 7261 6d73 2028 4469 6374  ery_params (Dict
+00000340: 5b73 7472 2c20 7374 725d 2c20 6f70 7469  [str, str], opti
+00000350: 6f6e 616c 293a 2054 6865 2071 7565 7279  onal): The query
+00000360: 2070 6172 616d 6574 6572 7320 746f 2075   parameters to u
+00000370: 7365 2069 6e20 7468 6520 6f70 6572 6174  se in the operat
+00000380: 696f 6e2e 2044 6566 6175 6c74 7320 746f  ion. Defaults to
+00000390: 204e 6f6e 652e 0a20 2020 2020 2020 2068   None..        h
+000003a0: 6561 6465 7273 2028 4469 6374 5b73 7472  eaders (Dict[str
+000003b0: 2c20 7374 725d 2c20 6f70 7469 6f6e 616c  , str], optional
+000003c0: 293a 2054 6865 2068 6561 6465 7273 2074  ): The headers t
+000003d0: 6f20 7573 6520 696e 2074 6865 206f 7065  o use in the ope
+000003e0: 7261 7469 6f6e 2e20 4465 6661 756c 7473  ration. Defaults
+000003f0: 2074 6f20 7b7d 2e0a 0a20 2020 2052 6574   to {}...    Ret
+00000400: 7572 6e73 3a0a 2020 2020 2020 2020 7479  urns:.        ty
+00000410: 7065 3a20 7468 6520 6a73 6f6e 2d65 6e63  pe: the json-enc
+00000420: 6f64 6564 2063 6f6e 7465 6e74 206f 6620  oded content of 
+00000430: 7468 6520 7265 7370 6f6e 7365 2c20 6966  the response, if
+00000440: 2061 6e79 2e0a 2020 2020 4e29 0972 0900   any..    N).r..
+00000450: 0000 720a 0000 00da 0761 7069 5f6b 6579  ..r......api_key
+00000460: 720b 0000 0072 0c00 0000 da04 6461 7461  r....r......data
+00000470: 5a05 6a73 6f6e 5fda 0763 6f6f 6b69 6573  Z.json_..cookies
+00000480: 720d 0000 0029 03da 0375 726c da06 7061  r....)...url..pa
+00000490: 7261 6d73 720d 0000 0029 0b72 0800 0000  ramsr....).r....
+000004a0: 5a0c 6175 7468 656e 7469 6361 7465 da08  Z.authenticate..
+000004b0: 7265 7175 6573 7473 da03 6765 745a 086d  requests..getZ.m
+000004c0: 616b 655f 7572 6c72 0c00 0000 720d 0000  ake_urlr....r...
+000004d0: 00da 1072 6169 7365 5f66 6f72 5f73 7461  ...raise_for_sta
+000004e0: 7475 73da 0a65 7863 6570 7469 6f6e 73da  tus..exceptions.
+000004f0: 0948 5454 5045 7272 6f72 da04 6a73 6f6e  .HTTPError..json
+00000500: 2908 7209 0000 0072 0a00 0000 720b 0000  ).r....r....r...
+00000510: 0072 0c00 0000 720d 0000 00da 0772 6571  .r....r......req
+00000520: 7565 7374 da08 7265 7370 6f6e 7365 da01  uest..response..
+00000530: 65a9 0072 1c00 0000 fa44 2f55 7365 7273  e..r.....D/Users
+00000540: 2f6e 6174 6861 6e73 6869 726c 6579 2f63  /nathanshirley/c
+00000550: 6f64 6573 7065 616b 2f63 6f64 6573 7065  odespeak/codespe
+00000560: 616b 2f70 7562 6c69 632f 7265 7374 5f72  ak/public/rest_r
+00000570: 6571 7565 7374 732f 6765 742e 7079 7214  equests/get.pyr.
+00000580: 0000 0009 0000 0073 3000 0000 0214 0201  .......s0.......
+00000590: 0201 0201 0201 0201 0201 0201 0201 0201  ................
+000005a0: 06f7 080b 0401 0601 0401 0401 06fd 0205  ................
+000005b0: 0a01 0803 12fe 0401 0880 02ff 7214 0000  ............r...
+000005c0: 0029 0eda 0674 7970 696e 6772 0200 0000  .)...typingr....
+000005d0: 7203 0000 0072 0400 0000 7213 0000 0072  r....r....r....r
+000005e0: 0500 0000 5a0e 636f 6465 7370 6561 6b2e  ....Z.codespeak.
+000005f0: 6170 6973 7206 0000 00da 2363 6f64 6573  apisr.....#codes
+00000600: 7065 616b 2e70 7562 6c69 632e 696e 6665  peak.public.infe
+00000610: 7272 6564 5f65 7863 6570 7469 6f6e 7207  rred_exceptionr.
+00000620: 0000 005a 2663 6f64 6573 7065 616b 2e70  ...Z&codespeak.p
+00000630: 7562 6c69 632e 7265 7374 5f72 6571 7565  ublic.rest_reque
+00000640: 7374 732e 7265 7175 6573 7472 0800 0000  sts.requestr....
+00000650: da03 7374 7272 1400 0000 721c 0000 0072  ..strr....r....r
+00000660: 1c00 0000 721c 0000 0072 1d00 0000 da08  ....r....r......
+00000670: 3c6d 6f64 756c 653e 0100 0000 7328 0000  <module>....s(..
+00000680: 0014 0008 010c 010c 010c 010c 0102 0602  ................
+00000690: 0102 0104 fb02 0102 ff02 0202 fe0e 0302  ................
+000006a0: fd0e 0402 fc0a 050e fb                   .........
```

### Comparing `codespeak-0.1.5/codespeak/public/rest_requests/__pycache__/post.cpython-310.pyc` & `codespeak-0.1.6/codespeak/public/rest_requests/__pycache__/post.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/public/rest_requests/__pycache__/put.cpython-310.pyc` & `codespeak-0.1.6/codespeak/public/rest_requests/__pycache__/put.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/public/rest_requests/__pycache__/request.cpython-310.pyc` & `codespeak-0.1.6/codespeak/public/rest_requests/__pycache__/request.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Jul 26 18:49:48 2023 UTC, .py size: 1590 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 cc6a c164 3606 0000  o........j.d6...
+00000000: 6f0d 0d0a 0000 0000 aac7 c264 2d06 0000  o..........d-...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 b200 0000 5500  .....@...s....U.
 00000030: 6400 6401 6c00 6d01 5a01 6d02 5a02 6d03  d.d.l.m.Z.m.Z.m.
 00000040: 5a03 0100 6400 6402 6c04 6d05 5a05 0100  Z...d.d.l.m.Z...
 00000050: 6400 6403 6c06 6d07 5a07 0100 6400 6404  d.d.l.m.Z...d.d.
 00000060: 6c08 6d09 5a09 0100 4700 6405 6406 8400  l.m.Z...G.d.d...
 00000070: 6406 6505 8303 5a0a 6400 6407 6c0b 6d0b  d.e...Z.d.d.l.m.
@@ -122,16 +122,15 @@
 00000790: 0072 1700 0000 7218 0000 00da 0961 7574  .r....r......aut
 000007a0: 685f 7a65 726f 3400 0000 7302 0000 0010  h_zero4...s.....
 000007b0: 0172 3000 0000 721b 0000 004e 2913 da06  .r0...r....N)...
 000007c0: 7479 7069 6e67 7202 0000 0072 0300 0000  typingr....r....
 000007d0: 7204 0000 00da 0870 7964 616e 7469 6372  r......pydanticr
 000007e0: 0500 0000 5a1b 636f 6465 7370 6561 6b2e  ....Z.codespeak.
 000007f0: 6170 6973 2e61 7069 5f6d 6574 6164 6174  apis.api_metadat
-00000800: 6172 0600 0000 da12 636f 6465 7370 6561  ar......codespea
-00000810: 6b2e 7365 7474 696e 6773 7207 0000 0072  k.settingsr....r
-00000820: 0800 0000 722a 0000 0072 2b00 0000 7227  ....r*...r+...r'
-00000830: 0000 0072 2200 0000 7230 0000 0072 1b00  ...r"...r0...r..
-00000840: 0000 da03 696e 7472 2800 0000 7217 0000  ....intr(...r...
-00000850: 0072 1700 0000 7217 0000 0072 1800 0000  .r....r....r....
-00000860: da08 3c6d 6f64 756c 653e 0100 0000 7314  ..<module>....s.
-00000870: 0000 0016 000c 010c 010c 0110 030c 2314  ..............#.
-00000880: 011e 030e 061c 04                        .......
+00000800: 6172 0600 0000 da09 636f 6465 7370 6561  ar......codespea
+00000810: 6b72 0700 0000 7208 0000 0072 2a00 0000  kr....r....r*...
+00000820: 722b 0000 0072 2700 0000 7222 0000 0072  r+...r'...r"...r
+00000830: 3000 0000 721b 0000 00da 0369 6e74 7228  0...r......intr(
+00000840: 0000 0072 1700 0000 7217 0000 0072 1700  ...r....r....r..
+00000850: 0000 7218 0000 00da 083c 6d6f 6475 6c65  ..r......<module
+00000860: 3e01 0000 0073 1400 0000 1600 0c01 0c01  >....s..........
+00000870: 0c01 1003 0c23 1401 1e03 0e06 1c04       .....#........
```

### Comparing `codespeak-0.1.5/codespeak/public/rest_requests/delete.py` & `codespeak-0.1.6/codespeak/public/rest_requests/delete.py`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/public/rest_requests/get.py` & `codespeak-0.1.6/codespeak/public/rest_requests/get.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Dict, List, Any
 import requests
 from furl import furl
-from codespeak.apis import api_keys
+from codespeak.apis import get_api_key
 from codespeak.public.inferred_exception import InferredException
 from codespeak.public.rest_requests.request import Request
 
 
 def get(
     api: str,
     path: str,
```

### Comparing `codespeak-0.1.5/codespeak/public/rest_requests/post.py` & `codespeak-0.1.6/codespeak/public/rest_requests/post.py`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/public/rest_requests/put.py` & `codespeak-0.1.6/codespeak/public/rest_requests/put.py`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/public/rest_requests/request.py` & `codespeak-0.1.6/codespeak/public/rest_requests/request.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Any, Callable, Dict
 from pydantic import BaseModel
 from codespeak.apis.api_metadata import api_metadatas
-from codespeak.settings import settings
+from codespeak import settings
 
 
 class Request(BaseModel):
     api: str
     path: str
     api_key: str | None
     path_params: Dict[str, Any] | None
```

### Comparing `codespeak-0.1.5/codespeak/type_definitions/__pycache__/classify.cpython-310.pyc` & `codespeak-0.1.6/codespeak/type_definitions/__pycache__/classify.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/type_definitions/__pycache__/definition.cpython-310.pyc` & `codespeak-0.1.6/codespeak/type_definitions/__pycache__/definition.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/type_definitions/__pycache__/free_modules.cpython-310.pyc` & `codespeak-0.1.6/codespeak/type_definitions/__pycache__/free_modules.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/type_definitions/__pycache__/import_definition.cpython-310.pyc` & `codespeak-0.1.6/codespeak/type_definitions/__pycache__/import_definition.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/type_definitions/__pycache__/type_definition.cpython-310.pyc` & `codespeak-0.1.6/codespeak/type_definitions/__pycache__/type_definition.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/type_definitions/classify.py` & `codespeak-0.1.6/codespeak/type_definitions/classify.py`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/type_definitions/free_modules.py` & `codespeak-0.1.6/codespeak/type_definitions/free_modules.py`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/type_definitions/import_definition.py` & `codespeak-0.1.6/codespeak/type_definitions/import_definition.py`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/type_definitions/type_definition.py` & `codespeak-0.1.6/codespeak/type_definitions/type_definition.py`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/type_definitions/types/__pycache__/builtin.cpython-310.pyc` & `codespeak-0.1.6/codespeak/type_definitions/types/__pycache__/builtin.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/type_definitions/types/__pycache__/builtin_type.cpython-310.pyc` & `codespeak-0.1.6/codespeak/type_definitions/types/__pycache__/builtin_type.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/type_definitions/types/__pycache__/complex_type_reference.cpython-310.pyc` & `codespeak-0.1.6/codespeak/type_definitions/types/__pycache__/complex_type_reference.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/type_definitions/types/__pycache__/custom_type_reference.cpython-310.pyc` & `codespeak-0.1.6/codespeak/type_definitions/types/__pycache__/custom_type_reference.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/type_definitions/types/__pycache__/generic.cpython-310.pyc` & `codespeak-0.1.6/codespeak/type_definitions/types/__pycache__/generic.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/type_definitions/types/__pycache__/generic_type.cpython-310.pyc` & `codespeak-0.1.6/codespeak/type_definitions/types/__pycache__/generic_type.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/type_definitions/types/__pycache__/installed_class.cpython-310.pyc` & `codespeak-0.1.6/codespeak/type_definitions/types/__pycache__/installed_class.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/type_definitions/types/__pycache__/installed_class_type.cpython-310.pyc` & `codespeak-0.1.6/codespeak/type_definitions/types/__pycache__/installed_class_type.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/type_definitions/types/__pycache__/local_class.cpython-310.pyc` & `codespeak-0.1.6/codespeak/type_definitions/types/__pycache__/local_class.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/type_definitions/types/__pycache__/local_class_as_self.cpython-310.pyc` & `codespeak-0.1.6/codespeak/type_definitions/types/__pycache__/local_class_as_self.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/type_definitions/types/__pycache__/local_class_reference.cpython-310.pyc` & `codespeak-0.1.6/codespeak/type_definitions/types/__pycache__/local_class_reference.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/type_definitions/types/__pycache__/local_class_type.cpython-310.pyc` & `codespeak-0.1.6/codespeak/type_definitions/types/__pycache__/local_class_type.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/type_definitions/types/__pycache__/none.cpython-310.pyc` & `codespeak-0.1.6/codespeak/type_definitions/types/__pycache__/none.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/type_definitions/types/__pycache__/prompt_annotation.cpython-310.pyc` & `codespeak-0.1.6/codespeak/type_definitions/types/__pycache__/prompt_annotation.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/type_definitions/types/__pycache__/typing_type.cpython-310.pyc` & `codespeak-0.1.6/codespeak/type_definitions/types/__pycache__/typing_type.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/type_definitions/types/__pycache__/union_type.cpython-310.pyc` & `codespeak-0.1.6/codespeak/type_definitions/types/__pycache__/union_type.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/type_definitions/types/custom_type_reference.py` & `codespeak-0.1.6/codespeak/type_definitions/types/custom_type_reference.py`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/type_definitions/types/generic.py` & `codespeak-0.1.6/codespeak/type_definitions/types/generic.py`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/type_definitions/types/installed_class.py` & `codespeak-0.1.6/codespeak/type_definitions/types/installed_class.py`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/type_definitions/types/local_class.py` & `codespeak-0.1.6/codespeak/type_definitions/types/local_class.py`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/type_definitions/types/typing_type.py` & `codespeak-0.1.6/codespeak/type_definitions/types/typing_type.py`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/type_definitions/types/union_type.py` & `codespeak-0.1.6/codespeak/type_definitions/types/union_type.py`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/type_definitions/utils/__pycache__/dedupe.cpython-310.pyc` & `codespeak-0.1.6/codespeak/type_definitions/utils/__pycache__/dedupe.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/type_definitions/utils/__pycache__/flat_uniques.cpython-310.pyc` & `codespeak-0.1.6/codespeak/type_definitions/utils/__pycache__/flat_uniques.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/type_definitions/utils/__pycache__/group.cpython-310.pyc` & `codespeak-0.1.6/codespeak/type_definitions/utils/__pycache__/group.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/type_definitions/utils/__pycache__/ref_locals_in_place.cpython-310.pyc` & `codespeak-0.1.6/codespeak/type_definitions/utils/__pycache__/ref_locals_in_place.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/type_definitions/utils/__pycache__/swap_complex_types.cpython-310.pyc` & `codespeak-0.1.6/codespeak/type_definitions/utils/__pycache__/swap_complex_types.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/type_definitions/utils/__pycache__/swap_custom_types.cpython-310.pyc` & `codespeak-0.1.6/codespeak/type_definitions/utils/__pycache__/swap_custom_types.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/type_definitions/utils/__pycache__/swap_locals.cpython-310.pyc` & `codespeak-0.1.6/codespeak/type_definitions/utils/__pycache__/swap_locals.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/codespeak/type_definitions/utils/swap_custom_types.py` & `codespeak-0.1.6/codespeak/type_definitions/utils/swap_custom_types.py`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.5/PKG-INFO` & `codespeak-0.1.6/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codespeak
-Version: 0.1.5
+Version: 0.1.6
 Summary: 
 Author: nateshirley
 Author-email: nate.00.shirley@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -19,7 +19,9 @@
 Requires-Dist: sqlalchemy (>=2.0.13,<3.0.0)
 Description-Content-Type: text/markdown
 
 # <img src="https://raw.githubusercontent.com/nateshirley/codespeak-assets/main/speaker.png" style="zoom:17%;" /> Codespeak
 
 Fast, no-frills code completion for users of your REST API.
 
+`pip install codespeak` or `poetry add codespeak`
+
```

