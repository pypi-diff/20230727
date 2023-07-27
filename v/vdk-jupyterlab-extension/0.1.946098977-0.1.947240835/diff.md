# Comparing `tmp/vdk_jupyterlab_extension-0.1.946098977.tar.gz` & `tmp/vdk_jupyterlab_extension-0.1.947240835.tar.gz`

## Comparing `vdk_jupyterlab_extension-0.1.946098977.tar` & `vdk_jupyterlab_extension-0.1.947240835.tar`

### file list

```diff
@@ -1,90 +1,90 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/.eslintignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/.eslintrc.js
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/.prettierignore
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/.prettierrc
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/.stylelintrc
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/babel.config.js
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/conftest.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/install.json
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/jest.config.js
--rw-r--r--   0        0        0   637378 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/package-lock.json
--rw-r--r--   0        0        0     5716 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/package.json
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/tsconfig.json
--rw-r--r--   0        0        0   425044 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/yarn.lock
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/jupyter-config/nb-config/vdk-jupyterlab-extension.json
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/jupyter-config/server-config/vdk-jupyterlab-extension.json
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/schema/plugin.json
--rw-r--r--   0        0        0     3405 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/src/commandsAndMenu.tsx
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/src/handler.ts
--rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/src/index.ts
--rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/src/initVDKConfigCell.ts
--rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/src/jobData.ts
--rw-r--r--   0        0        0     6593 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/src/serverRequests.ts
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/src/utils.ts
--rw-r--r--   0        0        0     4303 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/src/vdkTags.ts
--rw-r--r--   0        0        0     3490 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/src/__tests__/convert-job-to-notebook-component.spec.ts
--rw-r--r--   0        0        0     3694 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/src/__tests__/create-job-component.spec.ts
--rw-r--r--   0        0        0     3645 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/src/__tests__/deploy-job-component.spec.ts
--rw-r--r--   0        0        0     2667 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/src/__tests__/download-job-component.spec.ts
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/src/__tests__/handler.spec.ts
--rw-r--r--   0        0        0     5475 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/src/__tests__/resquests.spec.ts
--rw-r--r--   0        0        0     6323 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/src/__tests__/run-job-component.spec.tsx
--rw-r--r--   0        0        0     6907 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/src/__tests__/show-dialog.spec.tsx
--rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/src/__tests__/vdk-error-message.spec.ts
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/src/__tests__/vdk-jupyterlab-extension.spec.ts
--rw-r--r--   0        0        0     3910 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/src/__tests__/vdk-tags.spec.ts
--rw-r--r--   0        0        0    12078 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/src/components/ConvertJobToNotebook.tsx
--rw-r--r--   0        0        0     3422 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/src/components/CreateJob.tsx
--rw-r--r--   0        0        0     3771 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/src/components/DeployJob.tsx
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/src/components/DownloadJob.tsx
--rw-r--r--   0        0        0     7861 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/src/components/RunJob.tsx
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/src/components/VdkErrorMessage.ts
--rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/src/components/VdkTextInput.tsx
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/src/components/props.tsx
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/src/vdkOptions/vdk_options.ts
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/style/base.css
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/style/index.css
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/style/index.js
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/style/vdkDialogs.css
--rw-r--r--   0        0        0     7626 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/style/images/versatile-data-kit-logo.svg
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/testutils/jest-file-mock.js
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/testutils/jest-setup-files.js
--rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/ui-tests/README.md
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/ui-tests/jupyter_server_test_config.py
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/ui-tests/package.json
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/ui-tests/playwright.config.js
--rw-r--r--   0        0        0     7410 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/ui-tests/tests/convert-job.spec.ts
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/ui-tests/tests/utils.ts
--rw-r--r--   0        0        0     4512 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/ui-tests/tests/vdk-jupyterlab-extension.spec.ts
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/ui-tests/tests/data/convert-test-job-dirty/10_drop_table.sql
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/ui-tests/tests/data/convert-test-job-dirty/20_create_table.sql
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/ui-tests/tests/data/convert-test-job-dirty/30_ingest_to_table.py
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/vdk_jupyterlab_extension/__init__.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/vdk_jupyterlab_extension/_version.py
--rw-r--r--   0        0        0     3384 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/vdk_jupyterlab_extension/convert_job.py
--rw-r--r--   0        0        0     8109 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/vdk_jupyterlab_extension/handlers.py
--rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/vdk_jupyterlab_extension/job_data.py
--rw-r--r--   0        0        0     9848 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/vdk_jupyterlab_extension/vdk_ui.py
--rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/vdk_jupyterlab_extension/jupyter_sample_job/10_notebook.ipynb
--rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/vdk_jupyterlab_extension/jupyter_sample_job/README.md
--rw-r--r--   0        0        0     2850 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/vdk_jupyterlab_extension/jupyter_sample_job/config.ini
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/vdk_jupyterlab_extension/jupyter_sample_job/requirements.txt
--rw-r--r--   0        0        0     5264 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/vdk_jupyterlab_extension/labextension/package.json
--rw-r--r--   0        0        0     5716 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/vdk_jupyterlab_extension/labextension/schemas/vdk-jupyterlab-extension/package.json.orig
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/vdk_jupyterlab_extension/labextension/schemas/vdk-jupyterlab-extension/plugin.json
--rw-r--r--   0        0        0    21604 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/vdk_jupyterlab_extension/labextension/static/161.58979db168f482d72ccd.js
--rw-r--r--   0        0        0     5454 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/vdk_jupyterlab_extension/labextension/static/747.e678254df7945f8ed34d.js
--rw-r--r--   0        0        0     6841 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/vdk_jupyterlab_extension/labextension/static/remoteEntry.c2eb77da248d9dc524fb.js
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/vdk_jupyterlab_extension/labextension/static/style.js
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/vdk_jupyterlab_extension/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/vdk_jupyterlab_extension/tests/__init__.py
--rw-r--r--   0        0        0     2870 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/vdk_jupyterlab_extension/tests/test_convert_job_directory_processor.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/vdk_jupyterlab_extension/tests/test_directory_archiver.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/vdk_jupyterlab_extension/tests/test_handlers.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/vdk_jupyterlab_extension/vdk_options/__init__.py
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/vdk_jupyterlab_extension/vdk_options/vdk_options.py
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/.gitignore
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/LICENSE
--rw-r--r--   0        0        0     7167 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/README.md
--rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/pyproject.toml
--rw-r--r--   0        0        0     8775 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.946098977/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/.eslintignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/.eslintrc.js
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/.prettierignore
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/.prettierrc
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/.stylelintrc
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/babel.config.js
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/conftest.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/install.json
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/jest.config.js
+-rw-r--r--   0        0        0   637378 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/package-lock.json
+-rw-r--r--   0        0        0     5716 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/package.json
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/tsconfig.json
+-rw-r--r--   0        0        0   425068 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/yarn.lock
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/jupyter-config/nb-config/vdk-jupyterlab-extension.json
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/jupyter-config/server-config/vdk-jupyterlab-extension.json
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/schema/plugin.json
+-rw-r--r--   0        0        0     3405 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/src/commandsAndMenu.tsx
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/src/handler.ts
+-rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/src/index.ts
+-rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/src/initVDKConfigCell.ts
+-rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/src/jobData.ts
+-rw-r--r--   0        0        0     6593 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/src/serverRequests.ts
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/src/utils.ts
+-rw-r--r--   0        0        0     4303 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/src/vdkTags.ts
+-rw-r--r--   0        0        0     3490 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/src/__tests__/convert-job-to-notebook-component.spec.ts
+-rw-r--r--   0        0        0     3694 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/src/__tests__/create-job-component.spec.ts
+-rw-r--r--   0        0        0     3166 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/src/__tests__/deploy-job-component.spec.ts
+-rw-r--r--   0        0        0     2667 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/src/__tests__/download-job-component.spec.ts
+-rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/src/__tests__/handler.spec.ts
+-rw-r--r--   0        0        0     5475 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/src/__tests__/resquests.spec.ts
+-rw-r--r--   0        0        0     6323 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/src/__tests__/run-job-component.spec.tsx
+-rw-r--r--   0        0        0     6907 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/src/__tests__/show-dialog.spec.tsx
+-rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/src/__tests__/vdk-error-message.spec.ts
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/src/__tests__/vdk-jupyterlab-extension.spec.ts
+-rw-r--r--   0        0        0     3910 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/src/__tests__/vdk-tags.spec.ts
+-rw-r--r--   0        0        0    12078 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/src/components/ConvertJobToNotebook.tsx
+-rw-r--r--   0        0        0     3422 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/src/components/CreateJob.tsx
+-rw-r--r--   0        0        0     2982 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/src/components/DeployJob.tsx
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/src/components/DownloadJob.tsx
+-rw-r--r--   0        0        0     7861 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/src/components/RunJob.tsx
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/src/components/VdkErrorMessage.ts
+-rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/src/components/VdkTextInput.tsx
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/src/components/props.tsx
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/src/vdkOptions/vdk_options.ts
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/style/base.css
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/style/index.css
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/style/index.js
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/style/vdkDialogs.css
+-rw-r--r--   0        0        0     7626 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/style/images/versatile-data-kit-logo.svg
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/testutils/jest-file-mock.js
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/testutils/jest-setup-files.js
+-rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/ui-tests/README.md
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/ui-tests/package.json
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0     7410 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/ui-tests/tests/convert-job.spec.ts
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/ui-tests/tests/utils.ts
+-rw-r--r--   0        0        0     4512 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/ui-tests/tests/vdk-jupyterlab-extension.spec.ts
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/ui-tests/tests/data/convert-test-job-dirty/10_drop_table.sql
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/ui-tests/tests/data/convert-test-job-dirty/20_create_table.sql
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/ui-tests/tests/data/convert-test-job-dirty/30_ingest_to_table.py
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/vdk_jupyterlab_extension/__init__.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/vdk_jupyterlab_extension/_version.py
+-rw-r--r--   0        0        0     3384 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/vdk_jupyterlab_extension/convert_job.py
+-rw-r--r--   0        0        0     8050 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/vdk_jupyterlab_extension/handlers.py
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/vdk_jupyterlab_extension/job_data.py
+-rw-r--r--   0        0        0     9641 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/vdk_jupyterlab_extension/vdk_ui.py
+-rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/vdk_jupyterlab_extension/jupyter_sample_job/10_notebook.ipynb
+-rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/vdk_jupyterlab_extension/jupyter_sample_job/README.md
+-rw-r--r--   0        0        0     2850 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/vdk_jupyterlab_extension/jupyter_sample_job/config.ini
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/vdk_jupyterlab_extension/jupyter_sample_job/requirements.txt
+-rw-r--r--   0        0        0     5264 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/vdk_jupyterlab_extension/labextension/package.json
+-rw-r--r--   0        0        0     5716 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/vdk_jupyterlab_extension/labextension/schemas/vdk-jupyterlab-extension/package.json.orig
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/vdk_jupyterlab_extension/labextension/schemas/vdk-jupyterlab-extension/plugin.json
+-rw-r--r--   0        0        0    21056 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/vdk_jupyterlab_extension/labextension/static/161.8695b9e5520bd63d9d87.js
+-rw-r--r--   0        0        0     5454 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/vdk_jupyterlab_extension/labextension/static/747.e678254df7945f8ed34d.js
+-rw-r--r--   0        0        0     6841 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/vdk_jupyterlab_extension/labextension/static/remoteEntry.f0c41c67a1da9120d996.js
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/vdk_jupyterlab_extension/labextension/static/style.js
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/vdk_jupyterlab_extension/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/vdk_jupyterlab_extension/tests/__init__.py
+-rw-r--r--   0        0        0     2870 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/vdk_jupyterlab_extension/tests/test_convert_job_directory_processor.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/vdk_jupyterlab_extension/tests/test_directory_archiver.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/vdk_jupyterlab_extension/tests/test_handlers.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/vdk_jupyterlab_extension/vdk_options/__init__.py
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/vdk_jupyterlab_extension/vdk_options/vdk_options.py
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/.gitignore
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/LICENSE
+-rw-r--r--   0        0        0     7167 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/README.md
+-rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/pyproject.toml
+-rw-r--r--   0        0        0     8775 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/PKG-INFO
```

### Comparing `vdk_jupyterlab_extension-0.1.946098977/.eslintrc.js` & `vdk_jupyterlab_extension-0.1.947240835/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.946098977/jest.config.js` & `vdk_jupyterlab_extension-0.1.947240835/jest.config.js`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.946098977/package-lock.json` & `vdk_jupyterlab_extension-0.1.947240835/package-lock.json`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.946098977/package.json` & `vdk_jupyterlab_extension-0.1.947240835/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9772727272727273%*

 * *Differences: {"'version'": "'0.1.947240835'"}*

```diff
@@ -147,9 +147,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.946098977"
+    "version": "0.1.947240835"
 }
```

### Comparing `vdk_jupyterlab_extension-0.1.946098977/tsconfig.json` & `vdk_jupyterlab_extension-0.1.947240835/tsconfig.json`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.946098977/yarn.lock` & `vdk_jupyterlab_extension-0.1.947240835/yarn.lock`

 * *Files 0% similar despite different names*

```diff
@@ -3896,17 +3896,17 @@
   dependencies:
     chalk "^2.3.0"
     find-root "^1.0.0"
     lodash "^4.17.4"
     semver "^5.4.1"
 
 electron-to-chromium@^1.4.431:
-  version "1.4.471"
-  resolved "https://registry.yarnpkg.com/electron-to-chromium/-/electron-to-chromium-1.4.471.tgz#14cb056d0ce4bfa99df57946d57fe46c2330dac3"
-  integrity sha512-GpmGRC1vTl60w/k6YpQ18pSiqnmr0j3un//5TV1idPi6aheNfkT1Ye71tMEabWyNDO6sBMgAR+95Eb0eUUr1tA==
+  version "1.4.473"
+  resolved "https://registry.yarnpkg.com/electron-to-chromium/-/electron-to-chromium-1.4.473.tgz#4853de13a335c70fe1f9df8d4029be54068767d1"
+  integrity sha512-aVfC8+440vGfl06l8HKKn8/PD5jRfSnLkTTD65EFvU46igbpQRri1gxSzW9/+TeUlwYzrXk1sw867T96zlyECA==
 
 emittery@^0.7.1:
   version "0.7.2"
   resolved "https://registry.yarnpkg.com/emittery/-/emittery-0.7.2.tgz#25595908e13af0f5674ab419396e2fb394cdfa82"
   integrity sha512-A8OG5SR/ij3SsJdWDJdkkSYUjQdCUx6APQXem0SaEePBSRg4eymGYwBkKo1Y6DU+af/Jn2dBQqDBvjnr9Vi8nQ==
 
 emittery@^0.8.1:
@@ -3951,19 +3951,20 @@
   resolved "https://registry.yarnpkg.com/enhanced-resolve/-/enhanced-resolve-5.15.0.tgz#1af946c7d93603eb88e9896cee4904dc012e9c35"
   integrity sha512-LXYT42KJ7lpIKECr2mAXIaMldcNCh/7E0KBKOu4KSfkHmP+mZmSs+8V5gBAqisWBy0OO4W5Oyys0GO1Y8KtdKg==
   dependencies:
     graceful-fs "^4.2.4"
     tapable "^2.2.0"
 
 enquirer@^2.3.5:
-  version "2.3.6"
-  resolved "https://registry.yarnpkg.com/enquirer/-/enquirer-2.3.6.tgz#2a7fe5dd634a1e4125a975ec994ff5456dc3734d"
-  integrity sha512-yjNnPr315/FjS4zIsUxYguYUPP2e1NK4d7E7ZOLiyYCcbFBiTMyID+2wvm2w6+pZ/odMA7cRkjhsPbltwBOrLg==
+  version "2.4.0"
+  resolved "https://registry.yarnpkg.com/enquirer/-/enquirer-2.4.0.tgz#4f36f6c644137cc4fd2891da407ede2b1fea904a"
+  integrity sha512-ehu97t6FTYK2I3ZYtnp0BZ9vt0mvEL/cnHBds7Ct6jo9VX1VIkiFhOvVRWh6eblQqd7KOoICIQV+syZ3neXO/Q==
   dependencies:
     ansi-colors "^4.1.1"
+    strip-ansi "^6.0.1"
 
 entities@^2.0.0:
   version "2.2.0"
   resolved "https://registry.yarnpkg.com/entities/-/entities-2.2.0.tgz#098dc90ebb83d8dffa089d55256b351d34c4da55"
   integrity sha512-p92if5Nz619I0w+akJrLZH0MX0Pb5DX39XOwQTtXSdQQOaYH03S1uIQp4mhOZtAXrxq4ViO67YTiLBo2638o9A==
 
 envinfo@^7.7.3:
```

### Comparing `vdk_jupyterlab_extension-0.1.946098977/schema/plugin.json` & `vdk_jupyterlab_extension-0.1.947240835/schema/plugin.json`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.946098977/src/commandsAndMenu.tsx` & `vdk_jupyterlab_extension-0.1.947240835/src/commandsAndMenu.tsx`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.946098977/src/handler.ts` & `vdk_jupyterlab_extension-0.1.947240835/src/handler.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.946098977/src/index.ts` & `vdk_jupyterlab_extension-0.1.947240835/src/index.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.946098977/src/initVDKConfigCell.ts` & `vdk_jupyterlab_extension-0.1.947240835/src/initVDKConfigCell.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.946098977/src/jobData.ts` & `vdk_jupyterlab_extension-0.1.947240835/src/jobData.ts`

 * *Files 11% similar despite different names*

```diff
@@ -41,16 +41,15 @@
   const jsObj = {
     jobName: jobData.get(VdkOption.NAME),
     jobTeam: jobData.get(VdkOption.TEAM),
     jobPath: jobData.get(VdkOption.PATH),
     cloud: jobData.get(VdkOption.CLOUD),
     local: jobData.get(VdkOption.LOCAL),
     jobArguments: jobData.get(VdkOption.ARGUMENTS),
-    deploymentReason: jobData.get(VdkOption.DEPLOYMENT_REASON),
-    enableDeploy: jobData.get(VdkOption.DEPLOY_ENABLE)
+    deploymentReason: jobData.get(VdkOption.DEPLOYMENT_REASON)
   };
   return jsObj;
 }
 
 /*
  * Function that checks whether a value is defined in jobData
  * Shows dialog that operation cannot be performed because of undefined value
```

### Comparing `vdk_jupyterlab_extension-0.1.946098977/src/serverRequests.ts` & `vdk_jupyterlab_extension-0.1.947240835/src/serverRequests.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.946098977/src/vdkTags.ts` & `vdk_jupyterlab_extension-0.1.947240835/src/vdkTags.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.946098977/src/__tests__/convert-job-to-notebook-component.spec.ts` & `vdk_jupyterlab_extension-0.1.947240835/src/__tests__/convert-job-to-notebook-component.spec.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.946098977/src/__tests__/create-job-component.spec.ts` & `vdk_jupyterlab_extension-0.1.947240835/src/__tests__/create-job-component.spec.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.946098977/src/__tests__/deploy-job-component.spec.ts` & `vdk_jupyterlab_extension-0.1.947240835/src/__tests__/deploy-job-component.spec.ts`

 * *Files 10% similar despite different names*

```diff
@@ -34,27 +34,14 @@
     const input = component.getByPlaceholderText(defaultProps.jobPath);
     expect(input).toBe(
       component.getAllByLabelText('Path to job directory:')[0]
     );
   });
 });
 
-describe('#onEnableClick', () => {
-  it('should put a flag for enabled in jobData', () => {
-    const component = render(new DeployJobDialog(defaultProps).render());
-    const enableCheckbox = component.getAllByLabelText(
-      'Enable'
-    )[0] as HTMLInputElement;
-    expect(enableCheckbox.checked).toEqual(false);
-    fireEvent.click(enableCheckbox);
-    expect(enableCheckbox.checked).toEqual(true);
-    expect(jobData.get(VdkOption.DEPLOY_ENABLE)).toEqual('1');
-  });
-});
-
 describe('#onNameChange', () => {
   it('should change the job name in jobData', () => {
     const component = render(new DeployJobDialog(defaultProps).render());
     const input = component.getByPlaceholderText(defaultProps.jobName);
     fireEvent.change(input, { target: { value: 'second-name' } });
     expect(jobData.get(VdkOption.NAME)).toEqual('second-name');
   });
```

### Comparing `vdk_jupyterlab_extension-0.1.946098977/src/__tests__/download-job-component.spec.ts` & `vdk_jupyterlab_extension-0.1.947240835/src/__tests__/download-job-component.spec.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.946098977/src/__tests__/handler.spec.ts` & `vdk_jupyterlab_extension-0.1.947240835/src/__tests__/handler.spec.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.946098977/src/__tests__/resquests.spec.ts` & `vdk_jupyterlab_extension-0.1.947240835/src/__tests__/resquests.spec.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.946098977/src/__tests__/run-job-component.spec.tsx` & `vdk_jupyterlab_extension-0.1.947240835/src/__tests__/run-job-component.spec.tsx`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.946098977/src/__tests__/show-dialog.spec.tsx` & `vdk_jupyterlab_extension-0.1.947240835/src/__tests__/show-dialog.spec.tsx`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.946098977/src/__tests__/vdk-error-message.spec.ts` & `vdk_jupyterlab_extension-0.1.947240835/src/__tests__/vdk-error-message.spec.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.946098977/src/__tests__/vdk-tags.spec.ts` & `vdk_jupyterlab_extension-0.1.947240835/src/__tests__/vdk-tags.spec.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.946098977/src/components/ConvertJobToNotebook.tsx` & `vdk_jupyterlab_extension-0.1.947240835/src/components/ConvertJobToNotebook.tsx`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.946098977/src/components/CreateJob.tsx` & `vdk_jupyterlab_extension-0.1.947240835/src/components/CreateJob.tsx`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.946098977/src/components/DeployJob.tsx` & `vdk_jupyterlab_extension-0.1.947240835/src/components/DeployJob.tsx`

 * *Files 16% similar despite different names*

```diff
@@ -41,44 +41,17 @@
           label="Path to job directory:"
         ></VDKTextInput>
         <VDKTextInput
           option={VdkOption.DEPLOYMENT_REASON}
           value="reason"
           label="Deployment reason:"
         ></VDKTextInput>
-        <div>
-          <input
-            type="checkbox"
-            name="enable"
-            id="enable"
-            className="jp-vdk-checkbox"
-            onClick={this.onEnableClick()}
-          />
-          <label className="checkboxLabel" htmlFor="enable">
-            Enable
-          </label>
-        </div>
       </>
     );
   }
-  /**
-   * Callback invoked upon choosing Enable checkbox
-   */
-  private onEnableClick() {
-    return (event: React.MouseEvent) => {
-      const checkbox = document.getElementById('enable');
-      if (checkbox?.classList.contains('checked')) {
-        checkbox.classList.remove('checked');
-        jobData.set(VdkOption.DEPLOY_ENABLE, '');
-      } else {
-        checkbox?.classList.add('checked');
-        jobData.set(VdkOption.DEPLOY_ENABLE, '1');
-      }
-    };
-  }
 }
 
 export async function showCreateDeploymentDialog() {
   const result = await showDialog({
     title: CREATE_DEP_BUTTON_LABEL,
     body: (
       <DeployJobDialog
```

### Comparing `vdk_jupyterlab_extension-0.1.946098977/src/components/DownloadJob.tsx` & `vdk_jupyterlab_extension-0.1.947240835/src/components/DownloadJob.tsx`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.946098977/src/components/RunJob.tsx` & `vdk_jupyterlab_extension-0.1.947240835/src/components/RunJob.tsx`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.946098977/src/components/VdkErrorMessage.ts` & `vdk_jupyterlab_extension-0.1.947240835/src/components/VdkErrorMessage.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.946098977/src/components/VdkTextInput.tsx` & `vdk_jupyterlab_extension-0.1.947240835/src/components/VdkTextInput.tsx`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.946098977/style/base.css` & `vdk_jupyterlab_extension-0.1.947240835/style/base.css`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.946098977/style/vdkDialogs.css` & `vdk_jupyterlab_extension-0.1.947240835/style/vdkDialogs.css`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.946098977/style/images/versatile-data-kit-logo.svg` & `vdk_jupyterlab_extension-0.1.947240835/style/images/versatile-data-kit-logo.svg`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.946098977/ui-tests/README.md` & `vdk_jupyterlab_extension-0.1.947240835/ui-tests/README.md`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.946098977/ui-tests/jupyter_server_test_config.py` & `vdk_jupyterlab_extension-0.1.947240835/ui-tests/jupyter_server_test_config.py`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.946098977/ui-tests/tests/convert-job.spec.ts` & `vdk_jupyterlab_extension-0.1.947240835/ui-tests/tests/convert-job.spec.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.946098977/ui-tests/tests/vdk-jupyterlab-extension.spec.ts` & `vdk_jupyterlab_extension-0.1.947240835/ui-tests/tests/vdk-jupyterlab-extension.spec.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.946098977/ui-tests/tests/data/convert-test-job-dirty/30_ingest_to_table.py` & `vdk_jupyterlab_extension-0.1.947240835/ui-tests/tests/data/convert-test-job-dirty/30_ingest_to_table.py`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.946098977/vdk_jupyterlab_extension/__init__.py` & `vdk_jupyterlab_extension-0.1.947240835/vdk_jupyterlab_extension/__init__.py`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.946098977/vdk_jupyterlab_extension/convert_job.py` & `vdk_jupyterlab_extension-0.1.947240835/vdk_jupyterlab_extension/convert_job.py`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.946098977/vdk_jupyterlab_extension/handlers.py` & `vdk_jupyterlab_extension-0.1.947240835/vdk_jupyterlab_extension/handlers.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,15 +168,14 @@
         input_data = self.get_json_body()
         try:
             status = VdkUI.create_deployment(
                 input_data[VdkOption.NAME.value],
                 input_data[VdkOption.TEAM.value],
                 input_data[VdkOption.PATH.value],
                 input_data[VdkOption.DEPLOYMENT_REASON.value],
-                input_data[VdkOption.DEPLOY_ENABLE.value],
             )
             self.finish(json.dumps({"message": f"{status}", "error": ""}))
         except Exception as e:
             self.finish(json.dumps({"message": f"{e}", "error": "true"}))
 
 
 class GetNotebookInfoHandler(APIHandler):
```

### Comparing `vdk_jupyterlab_extension-0.1.946098977/vdk_jupyterlab_extension/job_data.py` & `vdk_jupyterlab_extension-0.1.947240835/vdk_jupyterlab_extension/job_data.py`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.946098977/vdk_jupyterlab_extension/vdk_ui.py` & `vdk_jupyterlab_extension-0.1.947240835/vdk_jupyterlab_extension/vdk_ui.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from pathlib import Path
 
 from vdk.internal.control.command_groups.job.create import JobCreate
 from vdk.internal.control.command_groups.job.delete import JobDelete
 from vdk.internal.control.command_groups.job.deploy_cli_impl import JobDeploy
 from vdk.internal.control.command_groups.job.download_job import JobDownloadSource
 from vdk.internal.control.utils import cli_utils
+from vdk.internal.control.utils.output_printer import InMemoryTextPrinter
 from vdk_jupyterlab_extension.convert_job import ConvertJobDirectoryProcessor
 from vdk_jupyterlab_extension.convert_job import DirectoryArchiver
 
 
 class RestApiUrlConfiguration:
     @staticmethod
     def get_rest_api_url():
@@ -139,45 +140,37 @@
         )
 
         cmd.create_job(name, team, path, cloud, local, jupyter_job_dir)
 
         return f"Job with name {name} was created."
 
     @staticmethod
-    def create_deployment(name: str, team: str, path: str, reason: str, enabled: bool):
+    def create_deployment(name: str, team: str, path: str, reason: str):
         """
         Execute `Deploy job`.
         :param name: the name of the data job that will be deployed
         :param team: the team of the data job that will be deployed
         :param path: the path to the job's directory
         :param reason: the reason of deployment
-        :param enabled: flag whether the job is enabled (that will basically un-pause the job)
         :return: output string of the operation
         """
-        output = "text"
-        cmd = JobDeploy(RestApiUrlConfiguration.get_rest_api_url(), output)
-        if enabled:
-            cmd.create(
-                name=name,
-                team=team,
-                job_path=path,
-                reason=reason,
-                vdk_version=None,
-                enabled=True,
-            )
-        else:
-            cmd.create(
-                name=name,
-                team=team,
-                job_path=path,
-                reason=reason,
-                vdk_version=None,
-                enabled=False,
-            )
-        return f"Job with name {name} and team {team} is deployed successfully!"
+        printer = InMemoryTextPrinter()
+        cmd = JobDeploy(RestApiUrlConfiguration.get_rest_api_url(), printer)
+        cmd.create(
+            name=name,
+            team=team,
+            job_path=path,
+            reason=reason,
+            vdk_version=None,
+            enabled=True,
+        )
+        return (
+            f"Job with name {name} and team {team} is deployed successfully! "
+            f"Deployment information:\n {printer.get_memory().strip()}"
+        )
 
     @staticmethod
     def get_notebook_info(cell_id: str, pr_path: str):
         """
         Return information about the notebook that includes a cell with a given id
         :param cell_id: the id of the cell
         :param pr_path: the path to the parent directory of the notebook
```

### Comparing `vdk_jupyterlab_extension-0.1.946098977/vdk_jupyterlab_extension/jupyter_sample_job/10_notebook.ipynb` & `vdk_jupyterlab_extension-0.1.947240835/vdk_jupyterlab_extension/jupyter_sample_job/10_notebook.ipynb`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.946098977/vdk_jupyterlab_extension/jupyter_sample_job/README.md` & `vdk_jupyterlab_extension-0.1.947240835/vdk_jupyterlab_extension/jupyter_sample_job/README.md`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.946098977/vdk_jupyterlab_extension/jupyter_sample_job/config.ini` & `vdk_jupyterlab_extension-0.1.947240835/vdk_jupyterlab_extension/jupyter_sample_job/config.ini`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.946098977/vdk_jupyterlab_extension/labextension/package.json` & `vdk_jupyterlab_extension-0.1.947240835/vdk_jupyterlab_extension/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9768939393939394%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.f0c41c67a1da9120d996.js'}}",*

 * * "'version'": "'0.1.947240835'"}*

```diff
@@ -79,15 +79,15 @@
                 "jlpm clean:all"
             ]
         }
     },
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.c2eb77da248d9dc524fb.js",
+            "load": "static/remoteEntry.f0c41c67a1da9120d996.js",
             "style": "./style"
         },
         "discovery": {
             "server": {
                 "base": {
                     "name": "vdk_jupyterlab_extension"
                 },
@@ -152,9 +152,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.946098977"
+    "version": "0.1.947240835"
 }
```

### Comparing `vdk_jupyterlab_extension-0.1.946098977/vdk_jupyterlab_extension/labextension/schemas/vdk-jupyterlab-extension/package.json.orig` & `vdk_jupyterlab_extension-0.1.947240835/vdk_jupyterlab_extension/labextension/schemas/vdk-jupyterlab-extension/package.json.orig`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9772727272727273%*

 * *Differences: {"'version'": "'0.1.947240835'"}*

```diff
@@ -147,9 +147,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.946098977"
+    "version": "0.1.947240835"
 }
```

### Comparing `vdk_jupyterlab_extension-0.1.946098977/vdk_jupyterlab_extension/labextension/schemas/vdk-jupyterlab-extension/plugin.json` & `vdk_jupyterlab_extension-0.1.947240835/vdk_jupyterlab_extension/labextension/schemas/vdk-jupyterlab-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.946098977/vdk_jupyterlab_extension/labextension/static/161.58979db168f482d72ccd.js` & `vdk_jupyterlab_extension-0.1.947240835/vdk_jupyterlab_extension/labextension/static/161.8695b9e5520bd63d9d87.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -1,53 +1,52 @@
 "use strict";
 (self.webpackChunkvdk_jupyterlab_extension = self.webpackChunkvdk_jupyterlab_extension || []).push([
     [161], {
-        161: (e, t, n) => {
-            n.r(t), n.d(t, {
+        161: (e, t, o) => {
+            o.r(t), o.d(t, {
                 default: () => z,
                 workingDirectory: () => G
             });
-            var o, a = n(38),
-                l = n(33),
-                r = n(271),
-                s = n.n(r);
+            var n, a = o(38),
+                l = o(33),
+                r = o(271),
+                s = o.n(r);
             ! function(e) {
-                e.NAME = "jobName", e.TEAM = "jobTeam", e.PATH = "jobPath", e.CLOUD = "cloud", e.LOCAL = "local", e.ARGUMENTS = "jobArguments", e.DEPLOYMENT_REASON = "deploymentReason", e.DEPLOY_ENABLE = "enableDeploy"
-            }(o || (o = {}));
-            var c = new Map([]);
+                e.NAME = "jobName", e.TEAM = "jobTeam", e.PATH = "jobPath", e.CLOUD = "cloud", e.LOCAL = "local", e.ARGUMENTS = "jobArguments", e.DEPLOYMENT_REASON = "deploymentReason"
+            }(n || (n = {}));
+            var i = new Map([]);
 
-            function i() {
-                for (const e of Object.values(o)) c.set(e, "")
+            function c() {
+                for (const e of Object.values(n)) i.set(e, "")
             }
 
-            function d() {
+            function u() {
                 return {
-                    jobName: c.get(o.NAME),
-                    jobTeam: c.get(o.TEAM),
-                    jobPath: c.get(o.PATH),
-                    cloud: c.get(o.CLOUD),
-                    local: c.get(o.LOCAL),
-                    jobArguments: c.get(o.ARGUMENTS),
-                    deploymentReason: c.get(o.DEPLOYMENT_REASON),
-                    enableDeploy: c.get(o.DEPLOY_ENABLE)
+                    jobName: i.get(n.NAME),
+                    jobTeam: i.get(n.TEAM),
+                    jobPath: i.get(n.PATH),
+                    cloud: i.get(n.CLOUD),
+                    local: i.get(n.LOCAL),
+                    jobArguments: i.get(n.ARGUMENTS),
+                    deploymentReason: i.get(n.DEPLOYMENT_REASON)
                 }
             }
-            async function u(e) {
-                return !!c.get(e) || (await (0, l.showErrorMessage)("Encountered an error while trying to execute operation. Error:", "The " + e + " should be defined!", [l.Dialog.okButton()]), !1)
+            async function d(e) {
+                return !!i.get(e) || (await (0, l.showErrorMessage)("Encountered an error while trying to execute operation. Error:", "The " + e + " should be defined!", [l.Dialog.okButton()]), !1)
             }
-            i();
+            c();
             const m = e => {
                 const t = e.split(/(?=[/\\])/);
                 return t[t.length - 1]
             };
             class h extends r.Component {
                 constructor(e) {
                     super(e), this.onInputChange = e => {
                         let t = e.currentTarget.value;
-                        t || (t = this.props.value), c.set(this.props.option, t)
+                        t || (t = this.props.value), i.set(this.props.option, t)
                     }
                 }
                 render() {
                     return s().createElement(s().Fragment, null, s().createElement("div", {
                         className: "jp-vdk-input-wrapper"
                     }, s().createElement("label", {
                         className: "jp-vdk-label",
@@ -57,22 +56,22 @@
                         id: this.props.option,
                         className: "jp-vdk-input",
                         placeholder: m(this.props.value),
                         onChange: this.onInputChange
                     })))
                 }
             }
-            var p = n(142),
-                g = n(820);
+            var p = o(142),
+                g = o(820);
             async function b(e = "", t = {}) {
-                const n = g.ServerConnection.makeSettings(),
-                    o = p.URLExt.join(n.baseUrl, "vdk-jupyterlab-extension", e);
+                const o = g.ServerConnection.makeSettings(),
+                    n = p.URLExt.join(o.baseUrl, "vdk-jupyterlab-extension", e);
                 let a;
                 try {
-                    a = await g.ServerConnection.makeRequest(o, t, n)
+                    a = await g.ServerConnection.makeRequest(n, t, o)
                 } catch (e) {
                     throw e
                 }
                 let l = await a.text();
                 if (l.length > 0) try {
                     l = JSON.parse(l)
                 } catch (e) {
@@ -80,82 +79,82 @@
                 }
                 if (!a.ok) throw new Error(a.statusText);
                 return l
             }
             const v = async e => {
                 await (0, l.showErrorMessage)("Encountered an error while trying to connect the server. Error:", e, [l.Dialog.okButton()])
             };
-            async function E() {
-                if (!await u(o.PATH)) return {
+            async function y() {
+                if (!await d(n.PATH)) return {
                     message: "",
                     status: !1
                 };
                 try {
                     const e = await b("run", {
-                        body: JSON.stringify(d()),
+                        body: JSON.stringify(u()),
                         method: "POST"
                     });
                     return {
                         message: e.message,
                         status: "0" == e.message
                     }
                 } catch (e) {
                     return v(e), {
                         message: "",
                         status: !1
                     }
                 }
             }
-            async function y(e) {
-                if (await u(o.NAME) && await u(o.TEAM)) try {
+            async function E(e) {
+                if (await d(n.NAME) && await d(n.TEAM)) try {
                     const t = await b(e, {
-                        body: JSON.stringify(d()),
+                        body: JSON.stringify(u()),
                         method: "POST"
                     });
                     t.error ? await (0, l.showErrorMessage)("Encountered an error while trying the " + e + " operation. Error:", t.message, [l.Dialog.okButton()]) : alert(t.message)
                 } catch (e) {
                     v(e)
                 }
             }
-            class k {
+            class f {
                 constructor(e) {
                     this.exception_message = "", this.what_happened = "", this.why_it_happened = "", this.consequences = "", this.countermeasures = "", this.__parse_message(e)
                 }
                 __parse_message(e) {
                     const t = ["exception_message", "what_happened", "why_it_happened", "consequences", "countermeasures"],
-                        n = ["ERROR : ", "WHAT HAPPENED :", "WHY IT HAPPENED :", "CONSEQUENCES :", "COUNTERMEASURES :"],
-                        o = e.split("\n");
+                        o = ["ERROR : ", "WHAT HAPPENED :", "WHY IT HAPPENED :", "CONSEQUENCES :", "COUNTERMEASURES :"],
+                        n = e.split("\n");
                     let a = 0;
-                    for (let l = 0; l < o.length; l++) {
-                        const r = o[l].indexOf(n[a]);
+                    for (let l = 0; l < n.length; l++) {
+                        const r = n[l].indexOf(o[a]);
                         if (-1 !== r) {
-                            if (this[t[a]] = n[a] + o[l].substring(r + n[a].length), a++, a === t.length) break
+                            if (this[t[a]] = o[a] + n[l].substring(r + o[a].length), a++, a === t.length) break
                         } else this.exception_message = e
                     }
                 }
             }
-            const f = "Convert Job To Notebook",
-                w = "Run Job",
+            const w = "Convert Job To Notebook",
+                k = "Run Job",
                 j = "Create Deployment";
-            class N extends r.Component {
+            class C extends r.Component {
                 constructor(e) {
                     super(e), this._onArgsChange = e => {
                         let t = e.currentTarget.value;
-                        t && this._isJSON(t) && c.set(o.ARGUMENTS, t)
+                        t && this._isJSON(t) && i.set(n.ARGUMENTS, t)
                     }, this._isJSON = e => {
                         try {
                             return JSON.parse(e), !0
                         } catch (e) {
                             return !1
                         }
                     }
                 }
                 render() {
                     return s().createElement(s().Fragment, null, s().createElement(h, {
-                        option: o.PATH,
+                        option: n.PATH,
                         value: this.props.jobPath,
                         label: "Path to job directory:"
                     }), s().createElement("div", {
                         className: "jp-vdk-input-wrapper"
                     }, s().createElement("label", {
                         className: "jp-vdk-label",
                         htmlFor: "arguments"
@@ -167,84 +166,84 @@
                         onChange: this._onArgsChange
                     })), s().createElement("ul", {
                         id: "argumentsUl",
                         className: "hidden"
                     }))
                 }
             }
-            async function C(e) {
+            async function T(e) {
                 if ((await (0, l.showDialog)({
-                        title: w,
-                        body: s().createElement(N, {
-                            jobPath: c.get(o.PATH)
+                        title: k,
+                        body: s().createElement(C, {
+                            jobPath: i.get(n.PATH)
                         }),
                         buttons: [l.Dialog.okButton(), l.Dialog.cancelButton()]
                     })).button.accept) {
                     let {
                         message: t,
-                        status: n
-                    } = await E();
-                    if (n)(0, l.showDialog)({
-                        title: w,
+                        status: o
+                    } = await y();
+                    if (o)(0, l.showDialog)({
+                        title: k,
                         body: s().createElement("div", {
                             className: "vdk-run-dialog-message-container"
                         }, s().createElement("p", {
                             className: "vdk-run-dialog-message"
                         }, "The job was executed successfully!")),
                         buttons: [l.Dialog.okButton()]
                     });
                     else {
                         t = "ERROR : " + t;
-                        const n = new k(t);
-                        e && await _(n, e) || (0, l.showDialog)({
-                            title: w,
+                        const o = new f(t);
+                        e && await _(o, e) || (0, l.showDialog)({
+                            title: k,
                             body: s().createElement("div", {
                                 className: "vdk-run-error-message "
-                            }, s().createElement("p", null, n.exception_message), s().createElement("p", null, n.what_happened), s().createElement("p", null, n.why_it_happened), s().createElement("p", null, n.consequences), s().createElement("p", null, n.countermeasures)),
+                            }, s().createElement("p", null, o.exception_message), s().createElement("p", null, o.what_happened), s().createElement("p", null, o.why_it_happened), s().createElement("p", null, o.consequences), s().createElement("p", null, o.countermeasures)),
                             buttons: [l.Dialog.okButton()]
                         })
                     }
                 }
             }
-            const D = e => {
+            const A = e => {
                     const t = e.getElementsByClassName("jp-Cell-inputWrapper");
                     for (let e = 0; e < t.length; e++) {
-                        const n = t[e].getElementsByClassName("jp-Cell-inputArea");
-                        if (n.length > 0) {
-                            const e = n[0].getElementsByClassName("jp-InputArea-prompt");
+                        const o = t[e].getElementsByClassName("jp-Cell-inputArea");
+                        if (o.length > 0) {
+                            const e = o[0].getElementsByClassName("jp-InputArea-prompt");
                             if (e.length > 0) return e[0]
                         }
                     }
                 },
-                A = e => {
-                    const t = D(e);
+                N = e => {
+                    const t = A(e);
                     null == t || t.classList.add("jp-vdk-failing-cell-prompt"), e.scrollIntoView(), e.classList.add("jp-vdk-failing-cell"), Array.from(document.getElementsByClassName("jp-vdk-failing-cell-num")).forEach((e => {
                         e.classList.remove("jp-vdk-failing-cell-num"), e.classList.add("jp-vdk-cell-num")
                     }))
                 },
-                T = e => {
+                D = e => {
                     e.classList.remove("jp-vdk-failing-cell");
-                    const t = D(e);
+                    const t = A(e);
                     null == t || t.classList.remove("jp-vdk-failing-cell-prompt")
                 },
                 _ = async (e, t) => {
-                    const n = (e => {
+                    const o = (e => {
                         const t = e.match(/cell_id:([0-9a-fA-F-]+)/);
                         return t ? t[1] : ""
                     })(e.what_happened);
-                    if (n) {
+                    if (o) {
                         const {
                             path: a,
                             cellIndex: r
                         } = await async function(e) {
                             const t = {
                                 cellId: e,
-                                jobPath: c.get(o.PATH)
+                                jobPath: i.get(n.PATH)
                             };
-                            if (!await u(o.PATH)) return {
+                            if (!await d(n.PATH)) return {
                                 path: "",
                                 cellIndex: ""
                             };
                             try {
                                 const e = await b("notebook", {
                                     body: JSON.stringify(t),
                                     method: "POST"
@@ -255,94 +254,79 @@
                                 }
                             } catch (e) {
                                 return {
                                     path: "",
                                     cellIndex: ""
                                 }
                             }
-                        }(n);
+                        }(o);
                         if (a) {
-                            const n = async () => {
+                            const o = async () => {
                                 const e = t.openOrReveal(a);
                                 if (e) {
                                     await e.revealed;
                                     const t = Array.from(e.node.children);
                                     t && t.forEach((async e => {
-                                        e.classList.contains("jp-Notebook") && (async (e, t, n) => {
-                                            const o = e.children;
-                                            if (t > o.length)(0, l.showDialog)({
+                                        e.classList.contains("jp-Notebook") && (async (e, t, o) => {
+                                            const n = e.children;
+                                            if (t > n.length)(0, l.showDialog)({
                                                 title: "Run Failed",
-                                                body: s().createElement("div", null, s().createElement("p", null, "Sorry, something went wrong while trying to find the failing cell!"), s().createElement("p", null, "Please, check the ", n, " once more and try to run the job while the notebook is active!")),
+                                                body: s().createElement("div", null, s().createElement("p", null, "Sorry, something went wrong while trying to find the failing cell!"), s().createElement("p", null, "Please, check the ", o, " once more and try to run the job while the notebook is active!")),
                                                 buttons: [l.Dialog.cancelButton()]
                                             });
                                             else
-                                                for (let e = 0; e < o.length; e++) e === t ? A(o[e]) : T(o[e])
+                                                for (let e = 0; e < n.length; e++) e === t ? N(n[e]) : D(n[e])
                                         })(e, Number(r), a)
                                     }))
                                 }
                             };
                             return (await (0, l.showDialog)({
-                                title: w,
+                                title: k,
                                 body: s().createElement("div", {
                                     className: "vdk-run-error-message "
                                 }, s().createElement("p", null, e.exception_message), s().createElement("p", null, e.what_happened), s().createElement("p", null, e.why_it_happened), s().createElement("p", null, e.consequences), s().createElement("p", null, e.countermeasures)),
                                 buttons: [l.Dialog.okButton({
                                     label: "See failing cell"
                                 }), l.Dialog.cancelButton()]
-                            })).button.accept && n(), !0
+                            })).button.accept && o(), !0
                         }
                     }
                     return !1
                 };
             class P extends r.Component {
                 constructor(e) {
                     super(e)
                 }
                 render() {
                     return s().createElement(s().Fragment, null, s().createElement(h, {
-                        option: o.NAME,
+                        option: n.NAME,
                         value: this.props.jobName,
                         label: "Job Name:"
                     }), s().createElement(h, {
-                        option: o.TEAM,
+                        option: n.TEAM,
                         value: this.props.jobTeam,
                         label: "Job Team:"
                     }), s().createElement(h, {
-                        option: o.PATH,
+                        option: n.PATH,
                         value: this.props.jobPath,
                         label: "Path to job directory:"
                     }), s().createElement(h, {
-                        option: o.DEPLOYMENT_REASON,
+                        option: n.DEPLOYMENT_REASON,
                         value: "reason",
                         label: "Deployment reason:"
-                    }), s().createElement("div", null, s().createElement("input", {
-                        type: "checkbox",
-                        name: "enable",
-                        id: "enable",
-                        className: "jp-vdk-checkbox",
-                        onClick: this.onEnableClick()
-                    }), s().createElement("label", {
-                        className: "checkboxLabel",
-                        htmlFor: "enable"
-                    }, "Enable")))
-                }
-                onEnableClick() {
-                    return e => {
-                        const t = document.getElementById("enable");
-                        (null == t ? void 0 : t.classList.contains("checked")) ? (t.classList.remove("checked"), c.set(o.DEPLOY_ENABLE, "")) : (null == t || t.classList.add("checked"), c.set(o.DEPLOY_ENABLE, "1"))
-                    }
+                    }))
                 }
             }
             async function x() {
                 const e = await (0, l.showDialog)({
                     title: j,
                     body: s().createElement(P, {
-                        jobName: c.get(o.NAME),
-                        jobPath: c.get(o.PATH),
-                        jobTeam: c.get(o.TEAM)
+                        jobName: i.get(n.NAME),
+                        jobPath: i.get(n.PATH),
+                        jobTeam: i.get(n.TEAM)
                     }),
                     buttons: [l.Dialog.okButton(), l.Dialog.cancelButton()]
                 });
                 if (!e.value && e.button.accept) try {
                     if ((await (0, l.showDialog)({
                             title: j,
                             body: "The job will be executed once before deployment.",
@@ -351,22 +335,22 @@
                             }), l.Dialog.okButton({
                                 label: "Continue"
                             })]
                         })).button.accept) {
                         const {
                             message: e,
                             status: t
-                        } = await E();
-                        t ? await u(o.DEPLOYMENT_REASON) && await y("deploy") : (0, l.showErrorMessage)("Encоuntered an error while running the job!", e, [l.Dialog.okButton()])
+                        } = await y();
+                        t ? await d(n.DEPLOYMENT_REASON) && await E("deploy") : (0, l.showErrorMessage)("Encоuntered an error while running the job!", e, [l.Dialog.okButton()])
                     }
                 } catch (e) {
                     await (0, l.showErrorMessage)("Encountered an error when deploying the job. Error:", e, [l.Dialog.okButton()])
                 }
             }
-            class L extends r.Component {
+            class O extends r.Component {
                 constructor(e) {
                     super(e)
                 }
                 render() {
                     return s().createElement(s().Fragment, null, s().createElement("div", {
                         className: "jp-vdk-checkbox-wrappers"
                     }, s().createElement("div", null, s().createElement("input", {
@@ -384,23 +368,23 @@
                         id: "Cloud",
                         className: "jp-vdk-checkbox",
                         onClick: this._onCloudClick()
                     }), s().createElement("label", {
                         className: "checkboxLabel",
                         htmlFor: "Cloud"
                     }, "Cloud"))), s().createElement(h, {
-                        option: o.NAME,
+                        option: n.NAME,
                         value: this.props.jobName,
                         label: "Job Name:"
                     }), s().createElement(h, {
-                        option: o.TEAM,
+                        option: n.TEAM,
                         value: this.props.jobTeam,
                         label: "Job Team:"
                     }), s().createElement(h, {
-                        option: o.PATH,
+                        option: n.PATH,
                         value: this.props.jobPath,
                         label: "Path to job directory:"
                     }))
                 }
                 _onLocalClick() {
                     return e => {
                         this.setJobFlags("Local")
@@ -409,93 +393,93 @@
                 _onCloudClick() {
                     return e => {
                         this.setJobFlags("Cloud")
                     }
                 }
                 setJobFlags(e) {
                     let t = document.getElementById(e);
-                    (null == t ? void 0 : t.classList.contains("checked")) ? (t.classList.remove("checked"), "Cloud" === e ? c.set(o.CLOUD, "") : c.set(o.LOCAL, "")) : (null == t || t.classList.add("checked"), "Cloud" === e ? c.set(o.CLOUD, "1") : c.set(o.LOCAL, "1"))
+                    (null == t ? void 0 : t.classList.contains("checked")) ? (t.classList.remove("checked"), "Cloud" === e ? i.set(n.CLOUD, "") : i.set(n.LOCAL, "")) : (null == t || t.classList.add("checked"), "Cloud" === e ? i.set(n.CLOUD, "1") : i.set(n.LOCAL, "1"))
                 }
             }
-            async function O() {
+            async function L() {
                 (await (0, l.showDialog)({
                     title: "Create Job",
-                    body: s().createElement(L, {
-                        jobPath: c.get(o.PATH),
-                        jobName: c.get(o.NAME),
-                        jobTeam: c.get(o.TEAM)
+                    body: s().createElement(O, {
+                        jobPath: i.get(n.PATH),
+                        jobName: i.get(n.NAME),
+                        jobTeam: i.get(n.TEAM)
                     }),
                     buttons: [l.Dialog.okButton(), l.Dialog.cancelButton()]
-                })).button.accept && await y("create")
+                })).button.accept && await E("create")
             }
-            class B extends r.Component {
+            class S extends r.Component {
                 constructor(e) {
                     super(e)
                 }
                 render() {
                     return s().createElement(s().Fragment, null, s().createElement(h, {
-                        option: o.NAME,
+                        option: n.NAME,
                         value: "default-name",
                         label: "Job Name:"
                     }), s().createElement(h, {
-                        option: o.TEAM,
+                        option: n.TEAM,
                         value: "default-team",
                         label: "Job Team:"
                     }), s().createElement(h, {
-                        option: o.PATH,
+                        option: n.PATH,
                         value: this.props.jobPath,
                         label: "Path to job directory:"
                     }))
                 }
             }
-            async function S() {
+            async function M() {
                 (await (0, l.showDialog)({
                     title: "Download Job",
-                    body: s().createElement(B, {
-                        jobPath: c.get(o.PATH)
+                    body: s().createElement(S, {
+                        jobPath: i.get(n.PATH)
                     }),
                     buttons: [l.Dialog.okButton(), l.Dialog.cancelButton()]
-                })).button.accept && await y("download")
+                })).button.accept && await E("download")
             }
-            var M;
+            var B;
             class J extends r.Component {
                 constructor(e) {
                     super(e)
                 }
                 render() {
                     return s().createElement(s().Fragment, null, s().createElement(h, {
-                        option: o.PATH,
+                        option: n.PATH,
                         value: this.props.jobPath,
                         label: "Path to job directory:"
                     }))
                 }
             }
-            async function H(e, t, n) {
+            async function H(e, t, o) {
                 if ((await (0, l.showDialog)({
-                        title: f,
+                        title: w,
                         body: s().createElement(J, {
-                            jobPath: c.get(o.PATH)
+                            jobPath: i.get(n.PATH)
                         }),
                         buttons: [l.Dialog.okButton(), l.Dialog.cancelButton()]
                     })).button.accept && (await (0, l.showDialog)({
-                        title: f,
-                        body: s().createElement("p", null, "Are you sure you want to convert the Data Job with path:", " ", s().createElement("i", null, c.get(o.PATH)), " to notebook?"),
+                        title: w,
+                        body: s().createElement("p", null, "Are you sure you want to convert the Data Job with path:", " ", s().createElement("i", null, i.get(n.PATH)), " to notebook?"),
                         buttons: [l.Dialog.okButton(), l.Dialog.cancelButton()]
                     })).button.accept) {
                     let {
                         message: a,
                         status: r
                     } = await async function() {
-                        if (!await u(o.PATH)) return {
+                        if (!await d(n.PATH)) return {
                             message: "The job path is not defined. Please define it before attempting to convert the job to a notebook.",
                             status: !1
                         };
                         try {
                             const e = await b("convertJobToNotebook", {
-                                body: JSON.stringify(d()),
+                                body: JSON.stringify(u()),
                                 method: "POST"
                             });
                             return {
                                 message: e.message,
                                 status: "" == e.error
                             }
                         } catch (e) {
@@ -503,200 +487,200 @@
                                 message: "",
                                 status: !1
                             }
                         }
                     }();
                     if (r) {
                         const r = JSON.parse(a);
-                        M = R(r.code_structure, r.removed_files), await I(e, t, n), await (0, l.showDialog)({
-                            title: f,
+                        B = R(r.code_structure, r.removed_files), await I(e, t, o), await (0, l.showDialog)({
+                            title: w,
                             body: s().createElement("div", {
                                 className: "vdk-convert-to-notebook-dialog-message-container"
                             }, s().createElement("p", {
                                 className: "vdk-convert-to-notebook-dialog-message"
-                            }, "The Data Job with path ", s().createElement("i", null, c.get(o.PATH)), " was converted to notebook successfully!")),
+                            }, "The Data Job with path ", s().createElement("i", null, i.get(n.PATH)), " was converted to notebook successfully!")),
                             buttons: [l.Dialog.okButton()]
                         })
                     } else if (a) {
                         a = "ERROR : " + a;
-                        const e = new k(a);
+                        const e = new f(a);
                         await (0, l.showDialog)({
-                            title: f,
+                            title: w,
                             body: s().createElement("div", {
                                 className: "vdk-convert-to-notebook-error-message "
                             }, s().createElement("p", null, e.exception_message), s().createElement("p", null, e.what_happened), s().createElement("p", null, e.why_it_happened), s().createElement("p", null, e.consequences), s().createElement("p", null, e.countermeasures)),
                             buttons: [l.Dialog.okButton()]
                         })
                     }
                 }
             }
-            const I = async (e, t, n) => {
+            const I = async (e, t, o) => {
                 try {
-                    const n = await async function() {
+                    const o = await async function() {
                         return await b("serverPath", {
                             method: "GET"
                         }) || (await (0, l.showErrorMessage)("Encountered an error while trying to connect the server. Error:       the server's location cannot be identified!", [l.Dialog.okButton()]), "")
                     }();
-                    c.set(o.NAME, c.get(o.PATH).split(/[\\/]/).pop() || ""), await t.model.cd(c.get(o.PATH).substring(n.length)), e.execute("notebook:create-new")
+                    i.set(n.NAME, i.get(n.PATH).split(/[\\/]/).pop() || ""), await t.model.cd(i.get(n.PATH).substring(o.length)), e.execute("notebook:create-new")
                 } catch (e) {
                     await (0, l.showErrorMessage)("Something went wrong while trying to create the new transformed notebook. Error:", e, [l.Dialog.okButton()])
                 }
             }, R = (e, t) => {
-                const n = [];
-                for (let o = 0; o < e.length; o++) n.push({
-                    source: "#### " + t[o],
+                const o = [];
+                for (let n = 0; n < e.length; n++) o.push({
+                    source: "#### " + t[n],
                     type: "markdown"
-                }), n.push({
-                    source: e[o],
+                }), o.push({
+                    source: e[n],
                     type: "code"
-                }), e[o].includes("def run(job_input: IJobInput)") && n.push({
+                }), e[n].includes("def run(job_input: IJobInput)") && o.push({
                     source: "run(job_input)",
                     type: "code"
                 });
-                return n
+                return o
             };
-            var F = "";
+            var V = "";
 
-            function V(e, t, n, a, r, s, u, m) {
+            function F(e, t, o, a, r, s, d, m) {
                 e.addCommand(t, {
-                    label: n,
+                    label: o,
                     caption: a,
                     execute: async () => {
                         try {
-                            F ? (0, l.showErrorMessage)("Another VDK operation is currently running!", "Please wait until the operation ends!", [l.Dialog.okButton()]) : (F = t, c.set(o.PATH, G), await async function() {
+                            V ? (0, l.showErrorMessage)("Another VDK operation is currently running!", "Please wait until the operation ends!", [l.Dialog.okButton()]) : (V = t, i.set(n.PATH, G), await async function() {
                                 try {
                                     const e = await b("job", {
-                                        body: JSON.stringify(JSON.stringify(d())),
+                                        body: JSON.stringify(JSON.stringify(u())),
                                         method: "POST"
                                     });
-                                    e && (c.set(o.NAME, e[o.NAME]), c.set(o.TEAM, e[o.TEAM]), c.set(o.PATH, e[o.PATH]))
+                                    e && (i.set(n.NAME, e[n.NAME]), i.set(n.TEAM, e[n.TEAM]), i.set(n.PATH, e[n.PATH]))
                                 } catch (e) {
                                     v(e)
                                 }
-                            }(), "Convert Job To Notebook" == n ? await r(e, u, m) : s ? await r(s) : await r(), i(), F = "")
+                            }(), "Convert Job To Notebook" == o ? await r(e, d, m) : s ? await r(s) : await r(), c(), V = "")
                         } catch (e) {
                             await (0, l.showErrorMessage)("Encountered an error when trying to open the dialog. Error:", e, [l.Dialog.okButton()])
                         }
                     }
                 })
             }
-            var K = n(280),
-                W = n(123);
+            var K = o(280),
+                W = o(123);
             const U = (e, t) => {
-                    const n = document.createElement("div");
-                    n.innerText = String(e), t.classList.contains("jp-vdk-failing-cell") ? n.classList.add("jp-vdk-failing-cell-num") : n.classList.add("jp-vdk-cell-num"), t.appendChild(n)
+                    const o = document.createElement("div");
+                    o.innerText = String(e), t.classList.contains("jp-vdk-failing-cell") ? o.classList.add("jp-vdk-failing-cell-num") : o.classList.add("jp-vdk-cell-num"), t.appendChild(o)
                 },
                 q = e => {
                     const t = document.createElement("img");
                     t.setAttribute("src", "https://raw.githubusercontent.com/vmware/versatile-data-kit/dc15f7489f763a0e0e29370b2e06a714448fc234/support/images/versatile-data-kit-logo.svg"), t.setAttribute("width", "20"), t.setAttribute("height", "20"), t.classList.add("jp-vdk-logo"), e.appendChild(t)
                 };
-            var Y = n(986);
+            var Y = o(986);
             let G = "";
             const z = {
                     id: "vdk-jupyterlab-extension:plugin",
                     autoStart: !0,
                     optional: [a.ISettingRegistry, K.IFileBrowserFactory, W.INotebookTracker, l.IThemeManager, Y.IDocumentManager],
-                    activate: async (e, t, n, a, l, r) => {
+                    activate: async (e, t, o, a, l, r) => {
                         const {
                             commands: s
                         } = e;
                         a.activeCellChanged.connect(((e, t) => {
-                            "jp-vdk:menu-convert-job-to-notebook" !== F ? function(e) {
-                                var t, n, o, a;
+                            "jp-vdk:menu-convert-job-to-notebook" !== V ? function(e) {
+                                var t, o, n, a;
                                 const l = e.currentWidget;
                                 if (l) {
-                                    const r = null === (n = null === (t = l.content.model) || void 0 === t ? void 0 : t.contentFactory) || void 0 === n ? void 0 : n.createCodeCell({
+                                    const r = null === (o = null === (t = l.content.model) || void 0 === t ? void 0 : t.contentFactory) || void 0 === o ? void 0 : o.createCodeCell({
                                             cell: {
                                                 cell_type: "code",
                                                 source: ['"""\n', "vdk_ipython extension introduces a magic command for Jupyter.\n", "The command enables the user to load VDK for the current notebook.\n", "VDK provides the job_input API, which has methods for:\n", "    * executing queries to an OLAP database;\n", "    * ingesting data into a database;\n", "    * processing data into a database.\n", "See the IJobInput documentation for more details.\n", "https://github.com/vmware/versatile-data-kit/blob/main/projects/vdk-core/src/vdk/api/job_input.py\n", "Please refrain from tagging this cell with VDK as it is not an actual part of the data job\n", "and is only used for development purposes.\n", '"""\n', "%reload_ext vdk_ipython\n", "%reload_VDK\n", "job_input = VDK.get_initialized_job_input()"],
                                                 metadata: {}
                                             }
                                         }),
-                                        s = null === (a = null === (o = e.currentWidget) || void 0 === o ? void 0 : o.content.model) || void 0 === a ? void 0 : a.cells,
-                                        c = null == s ? void 0 : s.get(0).value.text;
-                                    s && r && s.length <= 1 && "" == c && (s.insert(0, r), s.remove(1))
+                                        s = null === (a = null === (n = e.currentWidget) || void 0 === n ? void 0 : n.content.model) || void 0 === a ? void 0 : a.cells,
+                                        i = null == s ? void 0 : s.get(0).value.text;
+                                    s && r && s.length <= 1 && "" == i && (s.insert(0, r), s.remove(1))
                                 }
                             }(a) : (async e => {
-                                var t, n;
+                                var t, o;
                                 const a = e.currentWidget;
                                 if (a) {
-                                    const l = null === (n = null === (t = e.currentWidget) || void 0 === t ? void 0 : t.content.model) || void 0 === n ? void 0 : n.cells,
+                                    const l = null === (o = null === (t = e.currentWidget) || void 0 === t ? void 0 : t.content.model) || void 0 === o ? void 0 : o.cells,
                                         r = null == l ? void 0 : l.get(0).value.text;
                                     if (l && l.length <= 1 && "" == r) {
                                         l.remove(1);
                                         const e = e => {
-                                                var t, n;
-                                                const o = null === (n = null === (t = a.content.model) || void 0 === t ? void 0 : t.contentFactory) || void 0 === n ? void 0 : n.createMarkdownCell({
+                                                var t, o;
+                                                const n = null === (o = null === (t = a.content.model) || void 0 === t ? void 0 : t.contentFactory) || void 0 === o ? void 0 : o.createMarkdownCell({
                                                     cell: {
                                                         cell_type: "markdown",
                                                         source: e,
                                                         metadata: {}
                                                     }
                                                 });
-                                                o && l.push(o)
+                                                n && l.push(n)
                                             },
                                             t = (e, t) => {
-                                                var n, o;
-                                                const r = null === (o = null === (n = a.content.model) || void 0 === n ? void 0 : n.contentFactory) || void 0 === o ? void 0 : o.createCodeCell({
+                                                var o, n;
+                                                const r = null === (n = null === (o = a.content.model) || void 0 === o ? void 0 : o.contentFactory) || void 0 === n ? void 0 : n.createCodeCell({
                                                     cell: {
                                                         cell_type: "code",
                                                         source: e,
                                                         metadata: t
                                                     }
                                                 });
                                                 r && l.push(r)
                                             };
-                                        e(["# " + c.get(o.NAME)]), e(["### Please go through this guide before continuing with the data job run and development."]), e(["#### Introduction and Preparations\n", "*  *This is a notebook transformed from a directory style data job located in " + c.get(o.PATH) + ".*\n", "*  *If you are not familiar with notebook data jobs make sure to check the **Getting Started**(TODO: add link) page.*\n", "*  *You can find the **original job** at " + c.get(o.PATH).split(/[/\\]/).slice(0, -1).join("/") + ".*"]), e(["#### Execution Order and Identifying Cells\n", "*  *The below cells are automatically generated corresponding to a step(.sql or .py file with VDK run function) \n", "    in your original job.* \n", "*  *You will notice that some cells are coloured and include the VDK logo and a numbering. \n", '    These are the "vdk" tagged cells.\n', "    Only these cells are executed during VDK run and all the others are ignored(for example the current cell).*\n", "*  *Code cells in the notebook will be executed according to the numbering when running the notebook data job with VDK.\n", "    This means that the steps in the job are organized from the top to the bottom, starting with the first step.*\n", '*  *When you see a title saying **"Step generated from: sample.py"** before some blocks of code, \n', '    it means that the code below that title was created from the "sample.py" file.*\n', '*  *Similarly, if you come across code cells that have the format **"job_input.execute_query(query_string)"** ,\n', '    it means that those cells contain code generated from ".sql" files.*\n', '*  *On the other hand, code cells originating from ".py" files remain unchanged.\n', '    However, an additional cell is included that calls the "run" function using the command **"run(job_input)"** . \n', '    This cell executes the "run" function from the code generated from the ".py" file.*\n', '*  *You can delete the cells that are not tagged with "vdk" \n', "    as they are not essential to the data job's execution.\n", "    However, removing tagged cells will result in a different data job run.* "]), e(["#### Tips: \n", "* *Before running the job, it is recommended to review the cells\n", "    to ensure a clear understanding of the data job run.  \n", "    This will help to ensure the desired outcome.* "]), t(['"""\n', "vdk_ipython extension introduces a magic command for Jupyter.\n", "The command enables the user to load VDK for the current notebook.\n", "VDK provides the job_input API, which has methods for:\n", "    * executing queries to an OLAP database;\n", "    * ingesting data into a database;\n", "    * processing data into a database.\n", "See the IJobInput documentation for more details.\n", "https://github.com/vmware/versatile-data-kit/blob/main/projects/vdk-core/src/vdk/api/job_input.py\n", "Please refrain from tagging this cell with VDK as it is not an actual part of the data job\n", "and is only used for development purposes.\n", '"""\n', "%reload_ext vdk_ipython\n", "%reload_VDK\n", "job_input = VDK.get_initialized_job_input()"], {});
-                                        for (const n of M) "markdown" === n.type ? e([n.source]) : "code" === n.type && t([n.source], {
+                                        e(["# " + i.get(n.NAME)]), e(["### Please go through this guide before continuing with the data job run and development."]), e(["#### Introduction and Preparations\n", "*  *This is a notebook transformed from a directory style data job located in " + i.get(n.PATH) + ".*\n", "*  *If you are not familiar with notebook data jobs make sure to check the **Getting Started**(TODO: add link) page.*\n", "*  *You can find the **original job** at " + i.get(n.PATH).split(/[/\\]/).slice(0, -1).join("/") + ".*"]), e(["#### Execution Order and Identifying Cells\n", "*  *The below cells are automatically generated corresponding to a step(.sql or .py file with VDK run function) \n", "    in your original job.* \n", "*  *You will notice that some cells are coloured and include the VDK logo and a numbering. \n", '    These are the "vdk" tagged cells.\n', "    Only these cells are executed during VDK run and all the others are ignored(for example the current cell).*\n", "*  *Code cells in the notebook will be executed according to the numbering when running the notebook data job with VDK.\n", "    This means that the steps in the job are organized from the top to the bottom, starting with the first step.*\n", '*  *When you see a title saying **"Step generated from: sample.py"** before some blocks of code, \n', '    it means that the code below that title was created from the "sample.py" file.*\n', '*  *Similarly, if you come across code cells that have the format **"job_input.execute_query(query_string)"** ,\n', '    it means that those cells contain code generated from ".sql" files.*\n', '*  *On the other hand, code cells originating from ".py" files remain unchanged.\n', '    However, an additional cell is included that calls the "run" function using the command **"run(job_input)"** . \n', '    This cell executes the "run" function from the code generated from the ".py" file.*\n', '*  *You can delete the cells that are not tagged with "vdk" \n', "    as they are not essential to the data job's execution.\n", "    However, removing tagged cells will result in a different data job run.* "]), e(["#### Tips: \n", "* *Before running the job, it is recommended to review the cells\n", "    to ensure a clear understanding of the data job run.  \n", "    This will help to ensure the desired outcome.* "]), t(['"""\n', "vdk_ipython extension introduces a magic command for Jupyter.\n", "The command enables the user to load VDK for the current notebook.\n", "VDK provides the job_input API, which has methods for:\n", "    * executing queries to an OLAP database;\n", "    * ingesting data into a database;\n", "    * processing data into a database.\n", "See the IJobInput documentation for more details.\n", "https://github.com/vmware/versatile-data-kit/blob/main/projects/vdk-core/src/vdk/api/job_input.py\n", "Please refrain from tagging this cell with VDK as it is not an actual part of the data job\n", "and is only used for development purposes.\n", '"""\n', "%reload_ext vdk_ipython\n", "%reload_VDK\n", "job_input = VDK.get_initialized_job_input()"], {});
+                                        for (const o of B) "markdown" === o.type ? e([o.source]) : "code" === o.type && t([o.source], {
                                             tags: ["vdk"]
                                         });
-                                        M = []
+                                        B = []
                                     }
                                 }
                             })(a)
                         }));
-                        const i = n.defaultBrowser;
-                        ! function(e, t, n, o) {
-                            V(e, "jp-vdk:menu-run", "Run", "Execute VDK Run Command", C, t), V(e, "jp-vdk:menu-create", "Create", "Execute VDK Create Command", O), V(e, "jp-vdk:menu-download", "Download", "Execute VDK Download Command", S), V(e, "jp-vdk:menu-convert-job-to-notebook", "Convert Job To Notebook", "Convert Data Job To Jupyter Notebook", H, void 0, n, o), V(e, "jp-vdk:menu-create-deployment", "Deploy", "Create deployment of a VDK job", x)
-                        }(s, r, i, a), i.model.pathChanged.connect(Q), ((e, t) => {
-                            const n = async () => {
+                        const c = o.defaultBrowser;
+                        ! function(e, t, o, n) {
+                            F(e, "jp-vdk:menu-run", "Run", "Execute VDK Run Command", T, t), F(e, "jp-vdk:menu-create", "Create", "Execute VDK Create Command", L), F(e, "jp-vdk:menu-download", "Download", "Execute VDK Download Command", M), F(e, "jp-vdk:menu-convert-job-to-notebook", "Convert Job To Notebook", "Convert Data Job To Jupyter Notebook", H, void 0, o, n), F(e, "jp-vdk:menu-create-deployment", "Deploy", "Create deployment of a VDK job", x)
+                        }(s, r, c, a), c.model.pathChanged.connect(Q), ((e, t) => {
+                            const o = async () => {
                                 if (e.currentWidget && e.currentWidget.model && 0 !== e.currentWidget.model.cells.length) {
-                                    let n = [],
-                                        o = 0;
-                                    for (; e.currentWidget && e.currentWidget.model && e.currentWidget.model.cells.get(o);) {
-                                        const t = e.currentWidget.model.cells.get(o).metadata.get("tags");
-                                        t && t.includes("vdk") && n.push(o), o++
+                                    let o = [],
+                                        n = 0;
+                                    for (; e.currentWidget && e.currentWidget.model && e.currentWidget.model.cells.get(n);) {
+                                        const t = e.currentWidget.model.cells.get(n).metadata.get("tags");
+                                        t && t.includes("vdk") && o.push(n), n++
                                     }
-                                    n.length || (n = await async function(e) {
+                                    o.length || (o = await async function(e) {
                                         try {
                                             const t = {
                                                 nbPath: e
                                             };
                                             return await b("vdkCellIndices", {
                                                 body: JSON.stringify(t),
                                                 method: "POST"
                                             })
                                         } catch (e) {
                                             v(e)
                                         }
                                         return []
-                                    }(e.currentWidget.context.path)), n.length > 0 && e.activeCell && e.activeCell.parent && e.activeCell.parent.node.children && ((e, t, n, o) => {
+                                    }(e.currentWidget.context.path)), o.length > 0 && e.activeCell && e.activeCell.parent && e.activeCell.parent.node.children && ((e, t, o, n) => {
                                         Array.from(document.getElementsByClassName("jp-vdk-cell-num")).forEach((e => {
                                             e.remove()
                                         })), Array.from(document.getElementsByClassName("jp-vdk-failing-cell-num")).forEach((e => {
                                             e.remove()
                                         })), Array.from(document.getElementsByClassName("jp-vdk-logo")).forEach((e => {
                                             e.remove()
                                         }));
                                         let a = 0;
-                                        for (let l = 0; l < e.length; l++) t.includes(l) ? (n.theme && n.isLight(n.theme.toString()) ? (e[l].classList.remove("jp-vdk-cell-dark"), e[l].classList.add("jp-vdk-cell")) : (e[l].classList.add("jp-vdk-cell"), e[l].classList.add("jp-vdk-cell-dark")), o && e[l] != o && q(e[l]), U(++a, e[l])) : (e[l].classList.remove("jp-vdk-cell"), e[l].classList.remove("jp-vdk-cell-dark"))
-                                    })(Array.from(e.activeCell.parent.node.children), n, t, e.activeCell.node)
+                                        for (let l = 0; l < e.length; l++) t.includes(l) ? (o.theme && o.isLight(o.theme.toString()) ? (e[l].classList.remove("jp-vdk-cell-dark"), e[l].classList.add("jp-vdk-cell")) : (e[l].classList.add("jp-vdk-cell"), e[l].classList.add("jp-vdk-cell-dark")), n && e[l] != n && q(e[l]), U(++a, e[l])) : (e[l].classList.remove("jp-vdk-cell"), e[l].classList.remove("jp-vdk-cell-dark"))
+                                    })(Array.from(e.activeCell.parent.node.children), o, t, e.activeCell.node)
                                 }
                             };
-                            e.activeCellChanged.connect(n), t.themeChanged.connect(n)
+                            e.activeCellChanged.connect(o), t.themeChanged.connect(o)
                         })(a, l)
                     }
                 },
                 Q = async (e, t) => {
                     G = t.newValue
                 }
         }
```

### Comparing `vdk_jupyterlab_extension-0.1.946098977/vdk_jupyterlab_extension/labextension/static/747.e678254df7945f8ed34d.js` & `vdk_jupyterlab_extension-0.1.947240835/vdk_jupyterlab_extension/labextension/static/747.e678254df7945f8ed34d.js`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.946098977/vdk_jupyterlab_extension/labextension/static/remoteEntry.c2eb77da248d9dc524fb.js` & `vdk_jupyterlab_extension-0.1.947240835/vdk_jupyterlab_extension/labextension/static/remoteEntry.f0c41c67a1da9120d996.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, a, i, u, l, f, s, d, p, c, h, v, b = {
+    var e, r, t, n, o, a, i, u, l, f, d, s, p, c, h, v, b = {
             913: (e, r, t) => {
                 var n = {
                         "./index": () => t.e(161).then((() => () => t(161))),
                         "./extension": () => t.e(161).then((() => () => t(161))),
                         "./style": () => t.e(747).then((() => () => t(747)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
@@ -43,49 +43,49 @@
         }), r
     }, y.d = (e, r) => {
         for (var t in r) y.o(r, t) && !y.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, y.f = {}, y.e = e => Promise.all(Object.keys(y.f).reduce(((r, t) => (y.f[t](e, r), r)), [])), y.u = e => e + "." + {
-        161: "58979db168f482d72ccd",
+        161: "8695b9e5520bd63d9d87",
         747: "e678254df7945f8ed34d"
     } [e] + ".js?v=" + {
-        161: "58979db168f482d72ccd",
+        161: "8695b9e5520bd63d9d87",
         747: "e678254df7945f8ed34d"
     } [e], y.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
     }(), y.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "vdk-jupyterlab-extension:", y.l = (t, n, o, a) => {
         if (e[t]) e[t].push(n);
         else {
             var i, u;
             if (void 0 !== o)
                 for (var l = document.getElementsByTagName("script"), f = 0; f < l.length; f++) {
-                    var s = l[f];
-                    if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + o) {
-                        i = s;
+                    var d = l[f];
+                    if (d.getAttribute("src") == t || d.getAttribute("data-webpack") == r + o) {
+                        i = d;
                         break
                     }
                 }
             i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, y.nc && i.setAttribute("nonce", y.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [n];
-            var d = (r, n) => {
+            var s = (r, n) => {
                     i.onerror = i.onload = null, clearTimeout(p);
                     var o = e[t];
                     if (delete e[t], i.parentNode && i.parentNode.removeChild(i), o && o.forEach((e => e(n))), r) return r(n)
                 },
-                p = setTimeout(d.bind(null, void 0, {
+                p = setTimeout(s.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
-            i.onerror = d.bind(null, i.onerror), i.onload = d.bind(null, i.onload), u && document.head.appendChild(i)
+            i.onerror = s.bind(null, i.onerror), i.onload = s.bind(null, i.onload), u && document.head.appendChild(i)
         }
     }, y.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
@@ -106,15 +106,15 @@
                     var o = a[e] = a[e] || {},
                         u = o[r];
                     (!u || !u.loaded && (1 != !u.eager ? n : i > u.from)) && (o[r] = {
                         get: () => y.e(161).then((() => () => y(161))),
                         from: i,
                         eager: !1
                     })
-                })("vdk-jupyterlab-extension", "0.1.946098977"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                })("vdk-jupyterlab-extension", "0.1.947240835"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         y.g.importScripts && (e = y.g.location + "");
         var r = y.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -164,33 +164,33 @@
     }, a = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
                 o = n < 0;
             o && (n = -n - 1);
             for (var i = 0, u = 1, l = !0;; u++, i++) {
-                var f, s, d = u < e.length ? (typeof e[u])[0] : "";
-                if (i >= r.length || "o" == (s = (typeof(f = r[i]))[0])) return !l || ("u" == d ? u > n && !o : "" == d != o);
-                if ("u" == s) {
-                    if (!l || "u" != d) return !1
+                var f, d, s = u < e.length ? (typeof e[u])[0] : "";
+                if (i >= r.length || "o" == (d = (typeof(f = r[i]))[0])) return !l || ("u" == s ? u > n && !o : "" == s != o);
+                if ("u" == d) {
+                    if (!l || "u" != s) return !1
                 } else if (l)
-                    if (d == s)
+                    if (s == d)
                         if (u <= n) {
                             if (f != e[u]) return !1
                         } else {
                             if (o ? f > e[u] : f < e[u]) return !1;
                             f != e[u] && (l = !1)
                         }
-                else if ("s" != d && "n" != d) {
+                else if ("s" != s && "n" != s) {
                     if (o || u <= n) return !1;
                     l = !1, u--
                 } else {
-                    if (u <= n || s < d != o) return !1;
+                    if (u <= n || d < s != o) return !1;
                     l = !1
-                } else "s" != d && "n" != d && (l = !1, u--)
+                } else "s" != s && "n" != s && (l = !1, u--)
             }
         }
         var p = [],
             c = p.pop.bind(p);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
             p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? a(h, r) : !c())
@@ -201,18 +201,18 @@
         if (!t || !y.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, u = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
     }, l = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", f = (e, r, t, n) => {
         var o = u(e, t);
-        return a(n, o) || s(l(e, t, o, n)), d(e[t][o])
-    }, s = e => {
+        return a(n, o) || d(l(e, t, o, n)), s(e[t][o])
+    }, d = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
-    }, d = e => (e.loaded = 1, e.get()), p = (e => function(r, t, n, o) {
+    }, s = e => (e.loaded = 1, e.get()), p = (e => function(r, t, n, o) {
         var a = y.I(r);
         return a && a.then ? a.then(e.bind(e, r, y.S[r], t, n, o)) : e(r, y.S[r], t, n)
     })(((e, r, t, n) => (i(e, t), f(r, 0, t, n)))), c = {}, h = {
         33: () => p("default", "@jupyterlab/apputils", [1, 3, 6, 3]),
         38: () => p("default", "@jupyterlab/settingregistry", [1, 3, 6, 3]),
         123: () => p("default", "@jupyterlab/notebook", [1, 3, 6, 3]),
         142: () => p("default", "@jupyterlab/coreutils", [1, 5, 6, 3]),
```

### Comparing `vdk_jupyterlab_extension-0.1.946098977/vdk_jupyterlab_extension/labextension/static/third-party-licenses.json` & `vdk_jupyterlab_extension-0.1.947240835/vdk_jupyterlab_extension/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.946098977/vdk_jupyterlab_extension/tests/test_convert_job_directory_processor.py` & `vdk_jupyterlab_extension-0.1.947240835/vdk_jupyterlab_extension/tests/test_convert_job_directory_processor.py`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.946098977/vdk_jupyterlab_extension/tests/test_directory_archiver.py` & `vdk_jupyterlab_extension-0.1.947240835/vdk_jupyterlab_extension/tests/test_directory_archiver.py`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.946098977/.gitignore` & `vdk_jupyterlab_extension-0.1.947240835/.gitignore`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.946098977/README.md` & `vdk_jupyterlab_extension-0.1.947240835/README.md`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.946098977/pyproject.toml` & `vdk_jupyterlab_extension-0.1.947240835/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.946098977/PKG-INFO` & `vdk_jupyterlab_extension-0.1.947240835/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-jupyterlab-extension
-Version: 0.1.946098977
+Version: 0.1.947240835
 Summary: A Jupyterlab extension for using VDK
 Project-URL: Homepage, https://github.com/vmware/versatile-data-kit
 Project-URL: Bug Tracker, https://github.com/vmware/versatile-data-kit/issues
 Project-URL: Repository, https://github.com/vmware/versatile-data-kit
 Author-email: Versatile Data Kit Development Team <versatile-data-kit@vmware.com>
 License: See https://github.com/vmware/versatile-data-kit/blob/main/LICENSE
 License-File: LICENSE
```

