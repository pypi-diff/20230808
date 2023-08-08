# Comparing `tmp/vdk_jupyterlab_extension-0.1.951673056.tar.gz` & `tmp/vdk_jupyterlab_extension-0.1.959565555.tar.gz`

## Comparing `vdk_jupyterlab_extension-0.1.951673056.tar` & `vdk_jupyterlab_extension-0.1.959565555.tar`

### file list

```diff
@@ -1,90 +1,91 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/.eslintignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/.eslintrc.js
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/.prettierignore
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/.prettierrc
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/.stylelintrc
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/babel.config.js
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/conftest.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/install.json
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/jest.config.js
--rw-r--r--   0        0        0   637378 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/package-lock.json
--rw-r--r--   0        0        0     5716 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/package.json
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/tsconfig.json
--rw-r--r--   0        0        0   425098 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/yarn.lock
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/jupyter-config/nb-config/vdk-jupyterlab-extension.json
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/jupyter-config/server-config/vdk-jupyterlab-extension.json
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/schema/plugin.json
--rw-r--r--   0        0        0     3405 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/src/commandsAndMenu.tsx
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/src/handler.ts
--rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/src/index.ts
--rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/src/initVDKConfigCell.ts
--rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/src/jobData.ts
--rw-r--r--   0        0        0     6593 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/src/serverRequests.ts
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/src/utils.ts
--rw-r--r--   0        0        0     4303 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/src/vdkTags.ts
--rw-r--r--   0        0        0     3490 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/src/__tests__/convert-job-to-notebook-component.spec.ts
--rw-r--r--   0        0        0     3694 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/src/__tests__/create-job-component.spec.ts
--rw-r--r--   0        0        0     3166 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/src/__tests__/deploy-job-component.spec.ts
--rw-r--r--   0        0        0     2667 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/src/__tests__/download-job-component.spec.ts
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/src/__tests__/handler.spec.ts
--rw-r--r--   0        0        0     5475 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/src/__tests__/resquests.spec.ts
--rw-r--r--   0        0        0     6323 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/src/__tests__/run-job-component.spec.tsx
--rw-r--r--   0        0        0     6907 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/src/__tests__/show-dialog.spec.tsx
--rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/src/__tests__/vdk-error-message.spec.ts
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/src/__tests__/vdk-jupyterlab-extension.spec.ts
--rw-r--r--   0        0        0     3910 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/src/__tests__/vdk-tags.spec.ts
--rw-r--r--   0        0        0    12092 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/src/components/ConvertJobToNotebook.tsx
--rw-r--r--   0        0        0     3422 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/src/components/CreateJob.tsx
--rw-r--r--   0        0        0     2982 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/src/components/DeployJob.tsx
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/src/components/DownloadJob.tsx
--rw-r--r--   0        0        0     7861 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/src/components/RunJob.tsx
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/src/components/VdkErrorMessage.ts
--rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/src/components/VdkTextInput.tsx
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/src/components/props.tsx
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/src/vdkOptions/vdk_options.ts
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/style/base.css
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/style/index.css
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/style/index.js
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/style/vdkDialogs.css
--rw-r--r--   0        0        0     7626 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/style/images/versatile-data-kit-logo.svg
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/testutils/jest-file-mock.js
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/testutils/jest-setup-files.js
--rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/ui-tests/README.md
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/ui-tests/jupyter_server_test_config.py
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/ui-tests/package.json
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/ui-tests/playwright.config.js
--rw-r--r--   0        0        0     7417 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/ui-tests/tests/convert-job.spec.ts
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/ui-tests/tests/utils.ts
--rw-r--r--   0        0        0     4478 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/ui-tests/tests/vdk-jupyterlab-extension.spec.ts
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/ui-tests/tests/data/convert-test-job-dirty/10_drop_table.sql
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/ui-tests/tests/data/convert-test-job-dirty/20_create_table.sql
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/ui-tests/tests/data/convert-test-job-dirty/30_ingest_to_table.py
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/vdk_jupyterlab_extension/__init__.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/vdk_jupyterlab_extension/_version.py
--rw-r--r--   0        0        0     3384 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/vdk_jupyterlab_extension/convert_job.py
--rw-r--r--   0        0        0     8050 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/vdk_jupyterlab_extension/handlers.py
--rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/vdk_jupyterlab_extension/job_data.py
--rw-r--r--   0        0        0     9641 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/vdk_jupyterlab_extension/vdk_ui.py
--rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/vdk_jupyterlab_extension/jupyter_sample_job/10_notebook.ipynb
--rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/vdk_jupyterlab_extension/jupyter_sample_job/README.md
--rw-r--r--   0        0        0     2850 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/vdk_jupyterlab_extension/jupyter_sample_job/config.ini
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/vdk_jupyterlab_extension/jupyter_sample_job/requirements.txt
--rw-r--r--   0        0        0     5264 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/vdk_jupyterlab_extension/labextension/package.json
--rw-r--r--   0        0        0     5716 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/vdk_jupyterlab_extension/labextension/schemas/vdk-jupyterlab-extension/package.json.orig
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/vdk_jupyterlab_extension/labextension/schemas/vdk-jupyterlab-extension/plugin.json
--rw-r--r--   0        0        0    21084 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/vdk_jupyterlab_extension/labextension/static/161.687b3e6d54b7501a02f7.js
--rw-r--r--   0        0        0     5454 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/vdk_jupyterlab_extension/labextension/static/747.e678254df7945f8ed34d.js
--rw-r--r--   0        0        0     6841 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/vdk_jupyterlab_extension/labextension/static/remoteEntry.c52cf3d95e66ca429f2e.js
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/vdk_jupyterlab_extension/labextension/static/style.js
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/vdk_jupyterlab_extension/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/vdk_jupyterlab_extension/tests/__init__.py
--rw-r--r--   0        0        0     2870 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/vdk_jupyterlab_extension/tests/test_convert_job_directory_processor.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/vdk_jupyterlab_extension/tests/test_directory_archiver.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/vdk_jupyterlab_extension/tests/test_handlers.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/vdk_jupyterlab_extension/vdk_options/__init__.py
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/vdk_jupyterlab_extension/vdk_options/vdk_options.py
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/.gitignore
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/LICENSE
--rw-r--r--   0        0        0     6577 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/README.md
--rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/pyproject.toml
--rw-r--r--   0        0        0     8185 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.951673056/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/.eslintignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/.eslintrc.js
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/.prettierignore
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/.prettierrc
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/.stylelintrc
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/babel.config.js
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/conftest.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/install.json
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/jest.config.js
+-rw-r--r--   0        0        0   638841 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/package-lock.json
+-rw-r--r--   0        0        0     5757 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/package.json
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/tsconfig.json
+-rw-r--r--   0        0        0   425484 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/yarn.lock
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/jupyter-config/nb-config/vdk-jupyterlab-extension.json
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/jupyter-config/server-config/vdk-jupyterlab-extension.json
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/schema/plugin.json
+-rw-r--r--   0        0        0     3950 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/src/commandsAndMenu.tsx
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/src/handler.ts
+-rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/src/index.ts
+-rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/src/initVDKConfigCell.ts
+-rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/src/jobData.ts
+-rw-r--r--   0        0        0     6593 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/src/serverRequests.ts
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/src/utils.ts
+-rw-r--r--   0        0        0     4303 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/src/vdkTags.ts
+-rw-r--r--   0        0        0     3490 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/src/__tests__/convert-job-to-notebook-component.spec.ts
+-rw-r--r--   0        0        0     3694 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/src/__tests__/create-job-component.spec.ts
+-rw-r--r--   0        0        0     3166 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/src/__tests__/deploy-job-component.spec.ts
+-rw-r--r--   0        0        0     2667 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/src/__tests__/download-job-component.spec.ts
+-rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/src/__tests__/handler.spec.ts
+-rw-r--r--   0        0        0     5475 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/src/__tests__/resquests.spec.ts
+-rw-r--r--   0        0        0     6333 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/src/__tests__/run-job-component.spec.tsx
+-rw-r--r--   0        0        0     6907 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/src/__tests__/show-dialog.spec.tsx
+-rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/src/__tests__/vdk-error-message.spec.ts
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/src/__tests__/vdk-jupyterlab-extension.spec.ts
+-rw-r--r--   0        0        0     3910 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/src/__tests__/vdk-tags.spec.ts
+-rw-r--r--   0        0        0    12260 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/src/components/ConvertJobToNotebook.tsx
+-rw-r--r--   0        0        0     3560 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/src/components/CreateJob.tsx
+-rw-r--r--   0        0        0     3130 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/src/components/DeployJob.tsx
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/src/components/DownloadJob.tsx
+-rw-r--r--   0        0        0     8017 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/src/components/RunJob.tsx
+-rw-r--r--   0        0        0     3313 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/src/components/StatusButton.tsx
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/src/components/VdkErrorMessage.ts
+-rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/src/components/VdkTextInput.tsx
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/src/components/props.tsx
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/src/vdkOptions/vdk_options.ts
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/style/base.css
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/style/index.css
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/style/index.js
+-rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/style/vdkDialogs.css
+-rw-r--r--   0        0        0     7626 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/style/images/versatile-data-kit-logo.svg
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/testutils/jest-file-mock.js
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/testutils/jest-setup-files.js
+-rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/ui-tests/README.md
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/ui-tests/package.json
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0     7417 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/ui-tests/tests/convert-job.spec.ts
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/ui-tests/tests/utils.ts
+-rw-r--r--   0        0        0     4478 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/ui-tests/tests/vdk-jupyterlab-extension.spec.ts
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/ui-tests/tests/data/convert-test-job-dirty/10_drop_table.sql
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/ui-tests/tests/data/convert-test-job-dirty/20_create_table.sql
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/ui-tests/tests/data/convert-test-job-dirty/30_ingest_to_table.py
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/vdk_jupyterlab_extension/__init__.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/vdk_jupyterlab_extension/_version.py
+-rw-r--r--   0        0        0     3384 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/vdk_jupyterlab_extension/convert_job.py
+-rw-r--r--   0        0        0     8050 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/vdk_jupyterlab_extension/handlers.py
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/vdk_jupyterlab_extension/job_data.py
+-rw-r--r--   0        0        0     9641 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/vdk_jupyterlab_extension/vdk_ui.py
+-rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/vdk_jupyterlab_extension/jupyter_sample_job/10_notebook.ipynb
+-rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/vdk_jupyterlab_extension/jupyter_sample_job/README.md
+-rw-r--r--   0        0        0     2850 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/vdk_jupyterlab_extension/jupyter_sample_job/config.ini
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/vdk_jupyterlab_extension/jupyter_sample_job/requirements.txt
+-rw-r--r--   0        0        0     5301 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/vdk_jupyterlab_extension/labextension/package.json
+-rw-r--r--   0        0        0     5757 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/vdk_jupyterlab_extension/labextension/schemas/vdk-jupyterlab-extension/package.json.orig
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/vdk_jupyterlab_extension/labextension/schemas/vdk-jupyterlab-extension/plugin.json
+-rw-r--r--   0        0        0    23173 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/vdk_jupyterlab_extension/labextension/static/242.9f4f2d980858aa93e6aa.js
+-rw-r--r--   0        0        0     5955 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/vdk_jupyterlab_extension/labextension/static/747.d96a6a524ff42595fecc.js
+-rw-r--r--   0        0        0     6904 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/vdk_jupyterlab_extension/labextension/static/remoteEntry.4fde18a81e31cc9c2aa5.js
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/vdk_jupyterlab_extension/labextension/static/style.js
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/vdk_jupyterlab_extension/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/vdk_jupyterlab_extension/tests/__init__.py
+-rw-r--r--   0        0        0     2870 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/vdk_jupyterlab_extension/tests/test_convert_job_directory_processor.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/vdk_jupyterlab_extension/tests/test_directory_archiver.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/vdk_jupyterlab_extension/tests/test_handlers.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/vdk_jupyterlab_extension/vdk_options/__init__.py
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/vdk_jupyterlab_extension/vdk_options/vdk_options.py
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/.gitignore
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/LICENSE
+-rw-r--r--   0        0        0     6577 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/README.md
+-rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/pyproject.toml
+-rw-r--r--   0        0        0     8185 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.959565555/PKG-INFO
```

### Comparing `vdk_jupyterlab_extension-0.1.951673056/.eslintrc.js` & `vdk_jupyterlab_extension-0.1.959565555/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.951673056/jest.config.js` & `vdk_jupyterlab_extension-0.1.959565555/jest.config.js`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.951673056/package-lock.json` & `vdk_jupyterlab_extension-0.1.959565555/package-lock.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998551616015436%*

 * *Differences: {"'packages'": "{'': {'dependencies': {'@jupyterlab/mainmenu': '3.6.3'}}, "*

 * *               "'node_modules/@jupyterlab/mainmenu': OrderedDict([('version', '3.6.3'), "*

 * *               "('resolved', "*

 * *               "'https://registry.npmjs.org/@jupyterlab/mainmenu/-/mainmenu-3.6.3.tgz'), "*

 * *               "('integrity', "*

 * *               "'sha512-ohZzHDeReKX3zbLz2bUsYRSdkX6bVhNoCer3Rat8gjfb8vr/bqK9ReAvvoA4rRqm0mrfqwotpZSzbE4+y5KqZA=='), "*

 * *               "('dependencies', OrderedDict([('@jupyterlab/apputils', '^3 […]*

```diff
@@ -12,14 +12,15 @@
                 "@jupyterlab/codeeditor": "3.6.3",
                 "@jupyterlab/codemirror": "3.6.3",
                 "@jupyterlab/coreutils": "5.6.0",
                 "@jupyterlab/docmanager": "3.6.3",
                 "@jupyterlab/docprovider": "3.6.3",
                 "@jupyterlab/docregistry": "3.6.3",
                 "@jupyterlab/filebrowser": "3.6.3",
+                "@jupyterlab/mainmenu": "3.6.3",
                 "@jupyterlab/nbformat": "3.6.3",
                 "@jupyterlab/notebook": "3.6.3",
                 "@jupyterlab/outputarea": "3.6.3",
                 "@jupyterlab/rendermime": "3.6.3",
                 "@jupyterlab/rendermime-interfaces": "3.6.3",
                 "@jupyterlab/services": "6.6.3",
                 "@jupyterlab/settingregistry": "3.6.3",
@@ -2568,14 +2569,47 @@
             "dependencies": {
                 "@lumino/algorithm": "^1.9.2",
                 "@lumino/commands": "^1.21.1",
                 "@lumino/coreutils": "^1.12.1",
                 "@lumino/disposable": "^1.10.4",
                 "@lumino/domutils": "^1.8.2",
                 "@lumino/dragdrop": "^1.14.5",
+                "@lumino/keyboard": "^1.8.2",
+                "@lumino/messaging": "^1.10.3",
+                "@lumino/properties": "^1.8.2",
+                "@lumino/signaling": "^1.11.1",
+                "@lumino/virtualdom": "^1.14.3"
+            },
+            "integrity": "sha512-NHKu1NBDo6ETBDoNrqSkornfUCwc8EFFzw6+LWBfYVxn2PIwciq2SdiJGEyNqL+0h/A9eVKb5ui5z4cwpRekmQ==",
+            "resolved": "https://registry.npmjs.org/@lumino/widgets/-/widgets-1.37.2.tgz",
+            "version": "1.37.2"
+        },
+        "node_modules/@jupyterlab/mainmenu": {
+            "dependencies": {
+                "@jupyterlab/apputils": "^3.6.3",
+                "@jupyterlab/services": "^6.6.3",
+                "@jupyterlab/translation": "^3.6.3",
+                "@jupyterlab/ui-components": "^3.6.3",
+                "@lumino/algorithm": "^1.9.0",
+                "@lumino/commands": "^1.19.0",
+                "@lumino/coreutils": "^1.11.0",
+                "@lumino/widgets": "^1.37.2"
+            },
+            "integrity": "sha512-ohZzHDeReKX3zbLz2bUsYRSdkX6bVhNoCer3Rat8gjfb8vr/bqK9ReAvvoA4rRqm0mrfqwotpZSzbE4+y5KqZA==",
+            "resolved": "https://registry.npmjs.org/@jupyterlab/mainmenu/-/mainmenu-3.6.3.tgz",
+            "version": "3.6.3"
+        },
+        "node_modules/@jupyterlab/mainmenu/node_modules/@lumino/widgets": {
+            "dependencies": {
+                "@lumino/algorithm": "^1.9.2",
+                "@lumino/commands": "^1.21.1",
+                "@lumino/coreutils": "^1.12.1",
+                "@lumino/disposable": "^1.10.4",
+                "@lumino/domutils": "^1.8.2",
+                "@lumino/dragdrop": "^1.14.5",
                 "@lumino/keyboard": "^1.8.2",
                 "@lumino/messaging": "^1.10.3",
                 "@lumino/properties": "^1.8.2",
                 "@lumino/signaling": "^1.11.1",
                 "@lumino/virtualdom": "^1.14.3"
             },
             "integrity": "sha512-NHKu1NBDo6ETBDoNrqSkornfUCwc8EFFzw6+LWBfYVxn2PIwciq2SdiJGEyNqL+0h/A9eVKb5ui5z4cwpRekmQ==",
```

### Comparing `vdk_jupyterlab_extension-0.1.951673056/package.json` & `vdk_jupyterlab_extension-0.1.959565555/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9765151515151516%*

 * *Differences: {"'dependencies'": "{'@jupyterlab/mainmenu': '3.6.3'}", "'version'": "'0.1.959565555'"}*

```diff
@@ -15,14 +15,15 @@
         "@jupyterlab/codeeditor": "3.6.3",
         "@jupyterlab/codemirror": "3.6.3",
         "@jupyterlab/coreutils": "5.6.0",
         "@jupyterlab/docmanager": "3.6.3",
         "@jupyterlab/docprovider": "3.6.3",
         "@jupyterlab/docregistry": "3.6.3",
         "@jupyterlab/filebrowser": "3.6.3",
+        "@jupyterlab/mainmenu": "3.6.3",
         "@jupyterlab/nbformat": "3.6.3",
         "@jupyterlab/notebook": "3.6.3",
         "@jupyterlab/outputarea": "3.6.3",
         "@jupyterlab/rendermime": "3.6.3",
         "@jupyterlab/rendermime-interfaces": "3.6.3",
         "@jupyterlab/services": "6.6.3",
         "@jupyterlab/settingregistry": "3.6.3",
@@ -147,9 +148,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.951673056"
+    "version": "0.1.959565555"
 }
```

### Comparing `vdk_jupyterlab_extension-0.1.951673056/tsconfig.json` & `vdk_jupyterlab_extension-0.1.959565555/tsconfig.json`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.951673056/yarn.lock` & `vdk_jupyterlab_extension-0.1.959565555/yarn.lock`

 * *Files 1% similar despite different names*

```diff
@@ -11,20 +11,21 @@
   version "2.2.1"
   resolved "https://registry.yarnpkg.com/@ampproject/remapping/-/remapping-2.2.1.tgz#99e8e11851128b8702cd57c33684f1d0f260b630"
   integrity sha512-lFMjJTrFL3j7L9yBxwYfCq2k6qqwHyzuUl/XBnif78PWTJYyL/dfowQHWE3sp6U6ZzqWiiIZnpTMO96zhkjwtg==
   dependencies:
     "@jridgewell/gen-mapping" "^0.3.0"
     "@jridgewell/trace-mapping" "^0.3.9"
 
-"@babel/code-frame@^7.0.0", "@babel/code-frame@^7.10.4", "@babel/code-frame@^7.12.13", "@babel/code-frame@^7.22.5", "@babel/code-frame@^7.8.0":
-  version "7.22.5"
-  resolved "https://registry.yarnpkg.com/@babel/code-frame/-/code-frame-7.22.5.tgz#234d98e1551960604f1246e6475891a570ad5658"
-  integrity sha512-Xmwn266vad+6DAqEB2A6V/CcZVp62BbwVmcOJc2RPuwih1kw02TjQvWVWlcKGbBPd+8/0V5DEkOcizRGYsspYQ==
+"@babel/code-frame@^7.0.0", "@babel/code-frame@^7.10.4", "@babel/code-frame@^7.12.13", "@babel/code-frame@^7.22.10", "@babel/code-frame@^7.22.5", "@babel/code-frame@^7.8.0":
+  version "7.22.10"
+  resolved "https://registry.yarnpkg.com/@babel/code-frame/-/code-frame-7.22.10.tgz#1c20e612b768fefa75f6e90d6ecb86329247f0a3"
+  integrity sha512-/KKIMG4UEL35WmI9OlvMhurwtytjvXoFcGNrOvyG9zIzA8YmPjVtIZUf7b05+TPO7G7/GEmLHDaoCgACHl9hhA==
   dependencies:
-    "@babel/highlight" "^7.22.5"
+    "@babel/highlight" "^7.22.10"
+    chalk "^2.4.2"
 
 "@babel/compat-data@^7.20.5", "@babel/compat-data@^7.22.9":
   version "7.22.9"
   resolved "https://registry.yarnpkg.com/@babel/compat-data/-/compat-data-7.22.9.tgz#71cdb00a1ce3a329ce4cbec3a44f9fef35669730"
   integrity sha512-5UamI7xkUcJ3i9qVDS+KFDEK8/7oJ55/sJMB1Ge7IEapr7KfdfV/HErR+koZwOfd+SgtFKOKRhRakdg++DcJpQ==
 
 "@babel/core@7.8.0":
@@ -45,62 +46,62 @@
     json5 "^2.1.0"
     lodash "^4.17.13"
     resolve "^1.3.2"
     semver "^5.4.1"
     source-map "^0.5.0"
 
 "@babel/core@^7.1.0", "@babel/core@^7.12.3", "@babel/core@^7.7.2", "@babel/core@^7.7.5", "@babel/core@^7.8.0":
-  version "7.22.9"
-  resolved "https://registry.yarnpkg.com/@babel/core/-/core-7.22.9.tgz#bd96492c68822198f33e8a256061da3cf391f58f"
-  integrity sha512-G2EgeufBcYw27U4hhoIwFcgc1XU7TlXJ3mv04oOv1WCuo900U/anZSPzEqNjwdjgffkk2Gs0AN0dW1CKVLcG7w==
+  version "7.22.10"
+  resolved "https://registry.yarnpkg.com/@babel/core/-/core-7.22.10.tgz#aad442c7bcd1582252cb4576747ace35bc122f35"
+  integrity sha512-fTmqbbUBAwCcre6zPzNngvsI0aNrPZe77AeqvDxWM9Nm+04RrJ3CAmGHA9f7lJQY6ZMhRztNemy4uslDxTX4Qw==
   dependencies:
     "@ampproject/remapping" "^2.2.0"
-    "@babel/code-frame" "^7.22.5"
-    "@babel/generator" "^7.22.9"
-    "@babel/helper-compilation-targets" "^7.22.9"
+    "@babel/code-frame" "^7.22.10"
+    "@babel/generator" "^7.22.10"
+    "@babel/helper-compilation-targets" "^7.22.10"
     "@babel/helper-module-transforms" "^7.22.9"
-    "@babel/helpers" "^7.22.6"
-    "@babel/parser" "^7.22.7"
+    "@babel/helpers" "^7.22.10"
+    "@babel/parser" "^7.22.10"
     "@babel/template" "^7.22.5"
-    "@babel/traverse" "^7.22.8"
-    "@babel/types" "^7.22.5"
+    "@babel/traverse" "^7.22.10"
+    "@babel/types" "^7.22.10"
     convert-source-map "^1.7.0"
     debug "^4.1.0"
     gensync "^1.0.0-beta.2"
     json5 "^2.2.2"
     semver "^6.3.1"
 
-"@babel/generator@^7.22.7", "@babel/generator@^7.22.9", "@babel/generator@^7.7.2", "@babel/generator@^7.8.0":
-  version "7.22.9"
-  resolved "https://registry.yarnpkg.com/@babel/generator/-/generator-7.22.9.tgz#572ecfa7a31002fa1de2a9d91621fd895da8493d"
-  integrity sha512-KtLMbmicyuK2Ak/FTCJVbDnkN1SlT8/kceFTiuDiiRUUSMnHMidxSCdG4ndkTOHHpoomWe/4xkvHkEOncwjYIw==
+"@babel/generator@^7.22.10", "@babel/generator@^7.7.2", "@babel/generator@^7.8.0":
+  version "7.22.10"
+  resolved "https://registry.yarnpkg.com/@babel/generator/-/generator-7.22.10.tgz#c92254361f398e160645ac58831069707382b722"
+  integrity sha512-79KIf7YiWjjdZ81JnLujDRApWtl7BxTqWD88+FFdQEIOG8LJ0etDOM7CXuIgGJa55sGOwZVwuEsaLEm0PJ5/+A==
   dependencies:
-    "@babel/types" "^7.22.5"
+    "@babel/types" "^7.22.10"
     "@jridgewell/gen-mapping" "^0.3.2"
     "@jridgewell/trace-mapping" "^0.3.17"
     jsesc "^2.5.1"
 
 "@babel/helper-annotate-as-pure@^7.22.5":
   version "7.22.5"
   resolved "https://registry.yarnpkg.com/@babel/helper-annotate-as-pure/-/helper-annotate-as-pure-7.22.5.tgz#e7f06737b197d580a01edf75d97e2c8be99d3882"
   integrity sha512-LvBTxu8bQSQkcyKOU+a1btnNFQ1dMAd0R6PyW3arXes06F6QLWLIrd681bxRPIXlrMGR3XYnW9JyML7dP3qgxg==
   dependencies:
     "@babel/types" "^7.22.5"
 
 "@babel/helper-builder-binary-assignment-operator-visitor@^7.22.5":
-  version "7.22.5"
-  resolved "https://registry.yarnpkg.com/@babel/helper-builder-binary-assignment-operator-visitor/-/helper-builder-binary-assignment-operator-visitor-7.22.5.tgz#a3f4758efdd0190d8927fcffd261755937c71878"
-  integrity sha512-m1EP3lVOPptR+2DwD125gziZNcmoNSHGmJROKoy87loWUQyJaVXDgpmruWqDARZSmtYQ+Dl25okU8+qhVzuykw==
-  dependencies:
-    "@babel/types" "^7.22.5"
-
-"@babel/helper-compilation-targets@^7.20.7", "@babel/helper-compilation-targets@^7.22.5", "@babel/helper-compilation-targets@^7.22.6", "@babel/helper-compilation-targets@^7.22.9":
-  version "7.22.9"
-  resolved "https://registry.yarnpkg.com/@babel/helper-compilation-targets/-/helper-compilation-targets-7.22.9.tgz#f9d0a7aaaa7cd32a3f31c9316a69f5a9bcacb892"
-  integrity sha512-7qYrNM6HjpnPHJbopxmb8hSPoZ0gsX8IvUS32JGVoy+pU9e5N0nLr1VjJoR6kA4d9dmGLxNYOjeB8sUDal2WMw==
+  version "7.22.10"
+  resolved "https://registry.yarnpkg.com/@babel/helper-builder-binary-assignment-operator-visitor/-/helper-builder-binary-assignment-operator-visitor-7.22.10.tgz#573e735937e99ea75ea30788b57eb52fab7468c9"
+  integrity sha512-Av0qubwDQxC56DoUReVDeLfMEjYYSN1nZrTUrWkXd7hpU73ymRANkbuDm3yni9npkn+RXy9nNbEJZEzXr7xrfQ==
+  dependencies:
+    "@babel/types" "^7.22.10"
+
+"@babel/helper-compilation-targets@^7.20.7", "@babel/helper-compilation-targets@^7.22.10", "@babel/helper-compilation-targets@^7.22.5", "@babel/helper-compilation-targets@^7.22.6":
+  version "7.22.10"
+  resolved "https://registry.yarnpkg.com/@babel/helper-compilation-targets/-/helper-compilation-targets-7.22.10.tgz#01d648bbc25dd88f513d862ee0df27b7d4e67024"
+  integrity sha512-JMSwHD4J7SLod0idLq5PKgI+6g/hLD/iuWBq08ZX49xE14VpVEojJ5rHWptpirV2j020MvypRLAXAO50igCJ5Q==
   dependencies:
     "@babel/compat-data" "^7.22.9"
     "@babel/helper-validator-option" "^7.22.5"
     browserslist "^4.21.9"
     lru-cache "^5.1.1"
     semver "^6.3.1"
 
@@ -221,44 +222,44 @@
 
 "@babel/helper-validator-option@^7.22.5":
   version "7.22.5"
   resolved "https://registry.yarnpkg.com/@babel/helper-validator-option/-/helper-validator-option-7.22.5.tgz#de52000a15a177413c8234fa3a8af4ee8102d0ac"
   integrity sha512-R3oB6xlIVKUnxNUxbmgq7pKjxpru24zlimpE8WK47fACIlM0II/Hm1RS8IaOI7NgCr6LNS+jl5l75m20npAziw==
 
 "@babel/helper-wrap-function@^7.22.9":
-  version "7.22.9"
-  resolved "https://registry.yarnpkg.com/@babel/helper-wrap-function/-/helper-wrap-function-7.22.9.tgz#189937248c45b0182c1dcf32f3444ca153944cb9"
-  integrity sha512-sZ+QzfauuUEfxSEjKFmi3qDSHgLsTPK/pEpoD/qonZKOtTPTLbf59oabPQ4rKekt9lFcj/hTZaOhWwFYrgjk+Q==
+  version "7.22.10"
+  resolved "https://registry.yarnpkg.com/@babel/helper-wrap-function/-/helper-wrap-function-7.22.10.tgz#d845e043880ed0b8c18bd194a12005cb16d2f614"
+  integrity sha512-OnMhjWjuGYtdoO3FmsEFWvBStBAe2QOgwOLsLNDjN+aaiMD8InJk1/O3HSD8lkqTjCgg5YI34Tz15KNNA3p+nQ==
   dependencies:
     "@babel/helper-function-name" "^7.22.5"
     "@babel/template" "^7.22.5"
-    "@babel/types" "^7.22.5"
+    "@babel/types" "^7.22.10"
 
-"@babel/helpers@^7.22.6", "@babel/helpers@^7.8.0":
-  version "7.22.6"
-  resolved "https://registry.yarnpkg.com/@babel/helpers/-/helpers-7.22.6.tgz#8e61d3395a4f0c5a8060f309fb008200969b5ecd"
-  integrity sha512-YjDs6y/fVOYFV8hAf1rxd1QvR9wJe1pDBZ2AREKq/SDayfPzgk0PBnVuTCE5X1acEpMMNOVUqoe+OwiZGJ+OaA==
+"@babel/helpers@^7.22.10", "@babel/helpers@^7.8.0":
+  version "7.22.10"
+  resolved "https://registry.yarnpkg.com/@babel/helpers/-/helpers-7.22.10.tgz#ae6005c539dfbcb5cd71fb51bfc8a52ba63bc37a"
+  integrity sha512-a41J4NW8HyZa1I1vAndrraTlPZ/eZoga2ZgS7fEr0tZJGVU4xqdE80CEm0CcNjha5EZ8fTBYLKHF0kqDUuAwQw==
   dependencies:
     "@babel/template" "^7.22.5"
-    "@babel/traverse" "^7.22.6"
-    "@babel/types" "^7.22.5"
+    "@babel/traverse" "^7.22.10"
+    "@babel/types" "^7.22.10"
 
-"@babel/highlight@^7.22.5":
-  version "7.22.5"
-  resolved "https://registry.yarnpkg.com/@babel/highlight/-/highlight-7.22.5.tgz#aa6c05c5407a67ebce408162b7ede789b4d22031"
-  integrity sha512-BSKlD1hgnedS5XRnGOljZawtag7H1yPfQp0tdNJCHoH6AZ+Pcm9VvkrK59/Yy593Ypg0zMxH2BxD1VPYUQ7UIw==
+"@babel/highlight@^7.22.10":
+  version "7.22.10"
+  resolved "https://registry.yarnpkg.com/@babel/highlight/-/highlight-7.22.10.tgz#02a3f6d8c1cb4521b2fd0ab0da8f4739936137d7"
+  integrity sha512-78aUtVcT7MUscr0K5mIEnkwxPE0MaxkR5RxRwuHaQ+JuU5AmTPhY+do2mdzVTnIJJpyBglql2pehuBIWHug+WQ==
   dependencies:
     "@babel/helper-validator-identifier" "^7.22.5"
-    chalk "^2.0.0"
+    chalk "^2.4.2"
     js-tokens "^4.0.0"
 
-"@babel/parser@^7.1.0", "@babel/parser@^7.14.7", "@babel/parser@^7.20.7", "@babel/parser@^7.22.5", "@babel/parser@^7.22.7", "@babel/parser@^7.8.0":
-  version "7.22.7"
-  resolved "https://registry.yarnpkg.com/@babel/parser/-/parser-7.22.7.tgz#df8cf085ce92ddbdbf668a7f186ce848c9036cae"
-  integrity sha512-7NF8pOkHP5o2vpmGgNGcfAeCvOYhGLyA3Z4eBQkT1RJlWu47n63bCs93QfJ2hIAFCil7L5P2IWhs1oToVgrL0Q==
+"@babel/parser@^7.1.0", "@babel/parser@^7.14.7", "@babel/parser@^7.20.7", "@babel/parser@^7.22.10", "@babel/parser@^7.22.5", "@babel/parser@^7.8.0":
+  version "7.22.10"
+  resolved "https://registry.yarnpkg.com/@babel/parser/-/parser-7.22.10.tgz#e37634f9a12a1716136c44624ef54283cabd3f55"
+  integrity sha512-lNbdGsQb9ekfsnjFGhEiF4hfFqGgfOP3H3d27re3n+CGhNuTSUEQdfWk556sTLNTloczcdM5TYF2LhzmDQKyvQ==
 
 "@babel/plugin-proposal-async-generator-functions@^7.0.0":
   version "7.20.7"
   resolved "https://registry.yarnpkg.com/@babel/plugin-proposal-async-generator-functions/-/plugin-proposal-async-generator-functions-7.20.7.tgz#bfb7276d2d573cb67ba379984a2334e262ba5326"
   integrity sha512-xMbiLsn/8RK7Wq7VeVytytS2L6qE69bXPB10YCmMdDZbKF4okCqY74pI/jJQ/8U0b/F6NrT2+14b8/P9/3AMGA==
   dependencies:
     "@babel/helper-environment-visitor" "^7.18.9"
@@ -412,17 +413,17 @@
   version "7.22.5"
   resolved "https://registry.yarnpkg.com/@babel/plugin-transform-block-scoped-functions/-/plugin-transform-block-scoped-functions-7.22.5.tgz#27978075bfaeb9fa586d3cb63a3d30c1de580024"
   integrity sha512-tdXZ2UdknEKQWKJP1KMNmuF5Lx3MymtMN/pvA+p/VEkhK8jVcQ1fzSy8KM9qRYhAf2/lV33hoMPKI/xaI9sADA==
   dependencies:
     "@babel/helper-plugin-utils" "^7.22.5"
 
 "@babel/plugin-transform-block-scoping@^7.0.0":
-  version "7.22.5"
-  resolved "https://registry.yarnpkg.com/@babel/plugin-transform-block-scoping/-/plugin-transform-block-scoping-7.22.5.tgz#8bfc793b3a4b2742c0983fadc1480d843ecea31b"
-  integrity sha512-EcACl1i5fSQ6bt+YGuU/XGCeZKStLmyVGytWkpyhCLeQVA0eu6Wtiw92V+I1T/hnezUv7j74dA/Ro69gWcU+hg==
+  version "7.22.10"
+  resolved "https://registry.yarnpkg.com/@babel/plugin-transform-block-scoping/-/plugin-transform-block-scoping-7.22.10.tgz#88a1dccc3383899eb5e660534a76a22ecee64faa"
+  integrity sha512-1+kVpGAOOI1Albt6Vse7c8pHzcZQdQKW+wJH+g8mCaszOdDVwRXa/slHPqIw+oJAJANTKDMuM2cBdV0Dg618Vg==
   dependencies:
     "@babel/helper-plugin-utils" "^7.22.5"
 
 "@babel/plugin-transform-classes@^7.0.0":
   version "7.22.6"
   resolved "https://registry.yarnpkg.com/@babel/plugin-transform-classes/-/plugin-transform-classes-7.22.6.tgz#e04d7d804ed5b8501311293d1a0e6d43e94c3363"
   integrity sha512-58EgM6nuPNG6Py4Z3zSuu0xWu2VfodiMi72Jt5Kj2FECmaYk1RrTXA45z6KBFsu9tRgwQDwIiY4FXTt+YsSFAQ==
@@ -442,17 +443,17 @@
   resolved "https://registry.yarnpkg.com/@babel/plugin-transform-computed-properties/-/plugin-transform-computed-properties-7.22.5.tgz#cd1e994bf9f316bd1c2dafcd02063ec261bb3869"
   integrity sha512-4GHWBgRf0krxPX+AaPtgBAlTgTeZmqDynokHOX7aqqAB4tHs3U2Y02zH6ETFdLZGcg9UQSD1WCmkVrE9ErHeOg==
   dependencies:
     "@babel/helper-plugin-utils" "^7.22.5"
     "@babel/template" "^7.22.5"
 
 "@babel/plugin-transform-destructuring@^7.0.0":
-  version "7.22.5"
-  resolved "https://registry.yarnpkg.com/@babel/plugin-transform-destructuring/-/plugin-transform-destructuring-7.22.5.tgz#d3aca7438f6c26c78cdd0b0ba920a336001b27cc"
-  integrity sha512-GfqcFuGW8vnEqTUBM7UtPd5A4q797LTvvwKxXTgRsFjoqaJiEg9deBG6kWeQYkVEL569NpnmpC0Pkr/8BLKGnQ==
+  version "7.22.10"
+  resolved "https://registry.yarnpkg.com/@babel/plugin-transform-destructuring/-/plugin-transform-destructuring-7.22.10.tgz#38e2273814a58c810b6c34ea293be4973c4eb5e2"
+  integrity sha512-dPJrL0VOyxqLM9sritNbMSGx/teueHF/htMKrPT7DNxccXxRDPYqlgPFFdr8u+F+qUZOkZoXue/6rL5O5GduEw==
   dependencies:
     "@babel/helper-plugin-utils" "^7.22.5"
 
 "@babel/plugin-transform-dotall-regex@^7.0.0":
   version "7.22.5"
   resolved "https://registry.yarnpkg.com/@babel/plugin-transform-dotall-regex/-/plugin-transform-dotall-regex-7.22.5.tgz#dbb4f0e45766eb544e193fb00e65a1dd3b2a4165"
   integrity sha512-5/Yk9QxCQCl+sOIB1WelKnVRxTJDSAIxtJLL2/pqL14ZVlbH0fUQUZa/T5/UnQtBNgghR7mfB8ERBKyKPCi7Vw==
@@ -552,20 +553,20 @@
   version "7.22.5"
   resolved "https://registry.yarnpkg.com/@babel/plugin-transform-parameters/-/plugin-transform-parameters-7.22.5.tgz#c3542dd3c39b42c8069936e48717a8d179d63a18"
   integrity sha512-AVkFUBurORBREOmHRKo06FjHYgjrabpdqRSwq6+C7R5iTCZOsM4QbcB27St0a4U6fffyAOqh3s/qEfybAhfivg==
   dependencies:
     "@babel/helper-plugin-utils" "^7.22.5"
 
 "@babel/plugin-transform-regenerator@^7.0.0":
-  version "7.22.5"
-  resolved "https://registry.yarnpkg.com/@babel/plugin-transform-regenerator/-/plugin-transform-regenerator-7.22.5.tgz#cd8a68b228a5f75fa01420e8cc2fc400f0fc32aa"
-  integrity sha512-rR7KePOE7gfEtNTh9Qw+iO3Q/e4DEsoQ+hdvM6QUDH7JRJ5qxq5AA52ZzBWbI5i9lfNuvySgOGP8ZN7LAmaiPw==
+  version "7.22.10"
+  resolved "https://registry.yarnpkg.com/@babel/plugin-transform-regenerator/-/plugin-transform-regenerator-7.22.10.tgz#8ceef3bd7375c4db7652878b0241b2be5d0c3cca"
+  integrity sha512-F28b1mDt8KcT5bUyJc/U9nwzw6cV+UmTeRlXYIl2TNqMMJif0Jeey9/RQ3C4NOd2zp0/TRsDns9ttj2L523rsw==
   dependencies:
     "@babel/helper-plugin-utils" "^7.22.5"
-    regenerator-transform "^0.15.1"
+    regenerator-transform "^0.15.2"
 
 "@babel/plugin-transform-shorthand-properties@^7.0.0":
   version "7.22.5"
   resolved "https://registry.yarnpkg.com/@babel/plugin-transform-shorthand-properties/-/plugin-transform-shorthand-properties-7.22.5.tgz#6e277654be82b5559fc4b9f58088507c24f0c624"
   integrity sha512-vM4fq9IXHscXVKzDv5itkO1X52SmdFBFcMIBZ2FRn2nqVYqw6dBexUgMvAjHW+KXpPPViD/Yo3GrDEBaRC0QYA==
   dependencies:
     "@babel/helper-plugin-utils" "^7.22.5"
@@ -656,49 +657,49 @@
 
 "@babel/regjsgen@^0.8.0":
   version "0.8.0"
   resolved "https://registry.yarnpkg.com/@babel/regjsgen/-/regjsgen-0.8.0.tgz#f0ba69b075e1f05fb2825b7fad991e7adbb18310"
   integrity sha512-x/rqGMdzj+fWZvCOYForTghzbtqPDZ5gPwaoNGHdgDfF2QA/XZbCBp4Moo5scrkAMPhB7z26XM/AaHuIJdgauA==
 
 "@babel/runtime@^7.1.2", "@babel/runtime@^7.12.5", "@babel/runtime@^7.8.4":
-  version "7.22.6"
-  resolved "https://registry.yarnpkg.com/@babel/runtime/-/runtime-7.22.6.tgz#57d64b9ae3cff1d67eb067ae117dac087f5bd438"
-  integrity sha512-wDb5pWm4WDdF6LFUde3Jl8WzPA+3ZbxYqkC6xAXuD3irdEHN1k0NfTRrJD8ZD378SJ61miMLCqIOXYhd8x+AJQ==
+  version "7.22.10"
+  resolved "https://registry.yarnpkg.com/@babel/runtime/-/runtime-7.22.10.tgz#ae3e9631fd947cb7e3610d3e9d8fef5f76696682"
+  integrity sha512-21t/fkKLMZI4pqP2wlmsQAWnYW1PDyKyyUV4vCi+B25ydmdaYTKXPwCj0BzSUnZf4seIiYvSA3jcZ3gdsMFkLQ==
   dependencies:
-    regenerator-runtime "^0.13.11"
+    regenerator-runtime "^0.14.0"
 
 "@babel/template@^7.22.5", "@babel/template@^7.3.3", "@babel/template@^7.8.0":
   version "7.22.5"
   resolved "https://registry.yarnpkg.com/@babel/template/-/template-7.22.5.tgz#0c8c4d944509875849bd0344ff0050756eefc6ec"
   integrity sha512-X7yV7eiwAxdj9k94NEylvbVHLiVG1nvzCV2EAowhxLTwODV1jl9UzZ48leOC0sH7OnuHrIkllaBgneUykIcZaw==
   dependencies:
     "@babel/code-frame" "^7.22.5"
     "@babel/parser" "^7.22.5"
     "@babel/types" "^7.22.5"
 
-"@babel/traverse@^7.1.0", "@babel/traverse@^7.22.6", "@babel/traverse@^7.22.8", "@babel/traverse@^7.7.2", "@babel/traverse@^7.8.0":
-  version "7.22.8"
-  resolved "https://registry.yarnpkg.com/@babel/traverse/-/traverse-7.22.8.tgz#4d4451d31bc34efeae01eac222b514a77aa4000e"
-  integrity sha512-y6LPR+wpM2I3qJrsheCTwhIinzkETbplIgPBbwvqPKc+uljeA5gP+3nP8irdYt1mjQaDnlIcG+dw8OjAco4GXw==
+"@babel/traverse@^7.1.0", "@babel/traverse@^7.22.10", "@babel/traverse@^7.7.2", "@babel/traverse@^7.8.0":
+  version "7.22.10"
+  resolved "https://registry.yarnpkg.com/@babel/traverse/-/traverse-7.22.10.tgz#20252acb240e746d27c2e82b4484f199cf8141aa"
+  integrity sha512-Q/urqV4pRByiNNpb/f5OSv28ZlGJiFiiTh+GAHktbIrkPhPbl90+uW6SmpoLyZqutrg9AEaEf3Q/ZBRHBXgxig==
   dependencies:
-    "@babel/code-frame" "^7.22.5"
-    "@babel/generator" "^7.22.7"
+    "@babel/code-frame" "^7.22.10"
+    "@babel/generator" "^7.22.10"
     "@babel/helper-environment-visitor" "^7.22.5"
     "@babel/helper-function-name" "^7.22.5"
     "@babel/helper-hoist-variables" "^7.22.5"
     "@babel/helper-split-export-declaration" "^7.22.6"
-    "@babel/parser" "^7.22.7"
-    "@babel/types" "^7.22.5"
+    "@babel/parser" "^7.22.10"
+    "@babel/types" "^7.22.10"
     debug "^4.1.0"
     globals "^11.1.0"
 
-"@babel/types@^7.0.0", "@babel/types@^7.20.7", "@babel/types@^7.22.5", "@babel/types@^7.3.3", "@babel/types@^7.8.0":
-  version "7.22.5"
-  resolved "https://registry.yarnpkg.com/@babel/types/-/types-7.22.5.tgz#cd93eeaab025880a3a47ec881f4b096a5b786fbe"
-  integrity sha512-zo3MIHGOkPOfoRXitsgHLjEXmlDaD/5KU1Uzuc9GNiZPhSqVxVRtxuPaSBZDsYZ9qV88AjtMtWW7ww98loJ9KA==
+"@babel/types@^7.0.0", "@babel/types@^7.20.7", "@babel/types@^7.22.10", "@babel/types@^7.22.5", "@babel/types@^7.3.3", "@babel/types@^7.8.0":
+  version "7.22.10"
+  resolved "https://registry.yarnpkg.com/@babel/types/-/types-7.22.10.tgz#4a9e76446048f2c66982d1a989dd12b8a2d2dc03"
+  integrity sha512-obaoigiLrlDZ7TUQln/8m4mSqIW2QFeOrCQc9r+xsaHGNoplVNYlRVpsfE8Vj35GEm2ZH4ZhrNYogs/3fj85kg==
   dependencies:
     "@babel/helper-string-parser" "^7.22.5"
     "@babel/helper-validator-identifier" "^7.22.5"
     to-fast-properties "^2.0.0"
 
 "@bcoe/v8-coverage@^0.2.3":
   version "0.2.3"
@@ -1155,49 +1156,44 @@
   resolved "https://registry.yarnpkg.com/@jridgewell/gen-mapping/-/gen-mapping-0.3.3.tgz#7e02e6eb5df901aaedb08514203b096614024098"
   integrity sha512-HLhSWOLRi875zjjMG/r+Nv0oCW8umGb0BgEhyX3dDX3egwZtB8PqLnjz3yedt8R5StBrzcg4aBpnh8UA9D1BoQ==
   dependencies:
     "@jridgewell/set-array" "^1.0.1"
     "@jridgewell/sourcemap-codec" "^1.4.10"
     "@jridgewell/trace-mapping" "^0.3.9"
 
-"@jridgewell/resolve-uri@3.1.0":
-  version "3.1.0"
-  resolved "https://registry.yarnpkg.com/@jridgewell/resolve-uri/-/resolve-uri-3.1.0.tgz#2203b118c157721addfe69d47b70465463066d78"
-  integrity sha512-F2msla3tad+Mfht5cJq7LSXcdudKTWCVYUgw6pLFOOHSTtZlj6SWNYAp+AhuqLmWdBO2X5hPrLcu8cVP8fy28w==
+"@jridgewell/resolve-uri@^3.1.0":
+  version "3.1.1"
+  resolved "https://registry.yarnpkg.com/@jridgewell/resolve-uri/-/resolve-uri-3.1.1.tgz#c08679063f279615a3326583ba3a90d1d82cc721"
+  integrity sha512-dSYZh7HhCDtCKm4QakX0xFpsRDqjjtZf/kjI/v3T3Nwt5r8/qz/M19F9ySyOqU94SXBmeG9ttTul+YnR4LOxFA==
 
 "@jridgewell/set-array@^1.0.1":
   version "1.1.2"
   resolved "https://registry.yarnpkg.com/@jridgewell/set-array/-/set-array-1.1.2.tgz#7c6cf998d6d20b914c0a55a91ae928ff25965e72"
   integrity sha512-xnkseuNADM0gt2bs+BvhO0p78Mk762YnZdsuzFV018NoG1Sj1SCQvpSqa7XUaTam5vAGasABV9qXASMKnFMwMw==
 
 "@jridgewell/source-map@^0.3.3":
   version "0.3.5"
   resolved "https://registry.yarnpkg.com/@jridgewell/source-map/-/source-map-0.3.5.tgz#a3bb4d5c6825aab0d281268f47f6ad5853431e91"
   integrity sha512-UTYAUj/wviwdsMfzoSJspJxbkH5o1snzwX0//0ENX1u/55kkZZkcTZP6u9bwKGkv+dkk9at4m1Cpt0uY80kcpQ==
   dependencies:
     "@jridgewell/gen-mapping" "^0.3.0"
     "@jridgewell/trace-mapping" "^0.3.9"
 
-"@jridgewell/sourcemap-codec@1.4.14":
-  version "1.4.14"
-  resolved "https://registry.yarnpkg.com/@jridgewell/sourcemap-codec/-/sourcemap-codec-1.4.14.tgz#add4c98d341472a289190b424efbdb096991bb24"
-  integrity sha512-XPSJHWmi394fuUuzDnGz1wiKqWfo1yXecHQMRf2l6hztTO+nPru658AyDngaBe7isIxEkRsPR3FZh+s7iVa4Uw==
-
-"@jridgewell/sourcemap-codec@^1.4.10":
+"@jridgewell/sourcemap-codec@^1.4.10", "@jridgewell/sourcemap-codec@^1.4.14":
   version "1.4.15"
   resolved "https://registry.yarnpkg.com/@jridgewell/sourcemap-codec/-/sourcemap-codec-1.4.15.tgz#d7c6e6755c78567a951e04ab52ef0fd26de59f32"
   integrity sha512-eF2rxCRulEKXHTRiDrDy6erMYWqNw4LPdQ8UQA4huuxaQsVeRPFl2oM8oDGxMFhJUWZf9McpLtJasDDZb/Bpeg==
 
 "@jridgewell/trace-mapping@^0.3.17", "@jridgewell/trace-mapping@^0.3.9":
-  version "0.3.18"
-  resolved "https://registry.yarnpkg.com/@jridgewell/trace-mapping/-/trace-mapping-0.3.18.tgz#25783b2086daf6ff1dcb53c9249ae480e4dd4cd6"
-  integrity sha512-w+niJYzMHdd7USdiH2U6869nqhD2nbfZXND5Yp93qIbEmnDNk7PD48o+YchRVpzMU7M6jVCbenTR7PA1FLQ9pA==
+  version "0.3.19"
+  resolved "https://registry.yarnpkg.com/@jridgewell/trace-mapping/-/trace-mapping-0.3.19.tgz#f8a3249862f91be48d3127c3cfe992f79b4b8811"
+  integrity sha512-kf37QtfW+Hwx/buWGMPcR60iF9ziHa6r/CZJIHbmcm4+0qrXiVdxegAH0F6yddEVQ7zdkjcGCgCzUu+BcbhQxw==
   dependencies:
-    "@jridgewell/resolve-uri" "3.1.0"
-    "@jridgewell/sourcemap-codec" "1.4.14"
+    "@jridgewell/resolve-uri" "^3.1.0"
+    "@jridgewell/sourcemap-codec" "^1.4.14"
 
 "@juggle/resize-observer@^3.3.1":
   version "3.4.0"
   resolved "https://registry.yarnpkg.com/@juggle/resize-observer/-/resize-observer-3.4.0.tgz#08d6c5e20cf7e4cc02fd181c4b0c225cd31dbb60"
   integrity sha512-dfLbk+PwWvFzSxwk3n5ySL0hfBog779o8h68wK/7/APo/7cgyWp5jcXockbxdk5kFRkbeXWm4Fbi9FrdN381sA==
 
 "@jupyter/ydoc@~0.2.3", "@jupyter/ydoc@~0.2.4":
@@ -1701,25 +1697,39 @@
     "@lumino/messaging" "^1.10.0"
     "@lumino/polling" "^1.9.0"
     "@lumino/signaling" "^1.10.0"
     "@lumino/virtualdom" "^1.14.0"
     "@lumino/widgets" "^1.37.2"
     react "^17.0.1"
 
+"@jupyterlab/mainmenu@3.6.3":
+  version "3.6.3"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/mainmenu/-/mainmenu-3.6.3.tgz#5d322db9b8d742b7042109ab7e8c733696ae38fc"
+  integrity sha512-ohZzHDeReKX3zbLz2bUsYRSdkX6bVhNoCer3Rat8gjfb8vr/bqK9ReAvvoA4rRqm0mrfqwotpZSzbE4+y5KqZA==
+  dependencies:
+    "@jupyterlab/apputils" "^3.6.3"
+    "@jupyterlab/services" "^6.6.3"
+    "@jupyterlab/translation" "^3.6.3"
+    "@jupyterlab/ui-components" "^3.6.3"
+    "@lumino/algorithm" "^1.9.0"
+    "@lumino/commands" "^1.19.0"
+    "@lumino/coreutils" "^1.11.0"
+    "@lumino/widgets" "^1.37.2"
+
 "@jupyterlab/nbformat@3.6.3":
   version "3.6.3"
   resolved "https://registry.yarnpkg.com/@jupyterlab/nbformat/-/nbformat-3.6.3.tgz#8520338e3679cbe8ce2ea8eb5a9b816f8b774ad3"
   integrity sha512-0qJLa4dtOmu9EmHFeM7gaZi4qheovIPc9ZrgGGRuG0obajs4YYlvh4MQvCSgpVhme4AuBfGlcfzhlx+Gbzr5Xw==
   dependencies:
     "@lumino/coreutils" "^1.11.0"
 
 "@jupyterlab/nbformat@^3.0.0 || ^4.0.0-alpha.15":
-  version "4.0.3"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/nbformat/-/nbformat-4.0.3.tgz#02f005a7dccf34d70c99d935d92459927ec9c489"
-  integrity sha512-wpOktEi5XLPrAvTH+xkimeDghOz+oj1lPUHLeRTzcYBZfMybHQxV9XKfroXllcypkyqSBI5Ppfv6/GYeQQzmHQ==
+  version "4.0.4"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/nbformat/-/nbformat-4.0.4.tgz#fc712fea6011f9ff4d13ff156d5fa78d52751c92"
+  integrity sha512-ZAgLgnJbl0M3C3x0kHbwaxOXj6ydHj5V3PhFsAcKFZ1Jzqy15zn7wfVeLk9XimSisaijePCpKTY8uNku/IpVAw==
   dependencies:
     "@lumino/coreutils" "^2.1.1"
 
 "@jupyterlab/nbformat@^3.6.3", "@jupyterlab/nbformat@^3.6.5":
   version "3.6.5"
   resolved "https://registry.yarnpkg.com/@jupyterlab/nbformat/-/nbformat-3.6.5.tgz#dfb957d1297b2f319690df326e2ecc1eee99edfa"
   integrity sha512-yyyNniuzxycsF+kHvjpAIjZ+qrt3G/HEViZN+FJA3vFpg6e2n/nqa7BgzlxINS5SH4FnBG6rM/u45bwih38VkA==
@@ -2401,17 +2411,17 @@
   resolved "https://registry.yarnpkg.com/@types/eslint-scope/-/eslint-scope-3.7.4.tgz#37fc1223f0786c39627068a12e94d6e6fc61de16"
   integrity sha512-9K4zoImiZc3HlIp6AVUDE4CWYx22a+lhSZMYNpbjW04+YF0KWj4pJXnEMjdnFTiQibFFmElcsasJXDbdI/EPhA==
   dependencies:
     "@types/eslint" "*"
     "@types/estree" "*"
 
 "@types/eslint@*":
-  version "8.44.1"
-  resolved "https://registry.yarnpkg.com/@types/eslint/-/eslint-8.44.1.tgz#d1811559bb6bcd1a76009e3f7883034b78a0415e"
-  integrity sha512-XpNDc4Z5Tb4x+SW1MriMVeIsMoONHCkWFMkR/aPJbzEsxqHy+4Glu/BqTdPrApfDeMaXbtNh6bseNgl5KaWrSg==
+  version "8.44.2"
+  resolved "https://registry.yarnpkg.com/@types/eslint/-/eslint-8.44.2.tgz#0d21c505f98a89b8dd4d37fa162b09da6089199a"
+  integrity sha512-sdPRb9K6iL5XZOmBubg8yiFp5yS/JdUDQsq5e6h95km91MCYMuvp7mh1fjPEYUhvHepKpZOjnEaMBR4PxjWDzg==
   dependencies:
     "@types/estree" "*"
     "@types/json-schema" "*"
 
 "@types/estree@*", "@types/estree@^1.0.0":
   version "1.0.1"
   resolved "https://registry.yarnpkg.com/@types/estree/-/estree-1.0.1.tgz#aa22750962f3bf0e79d753d3cc067f010c95f194"
@@ -2458,17 +2468,17 @@
 
 "@types/minimist@^1.2.0":
   version "1.2.2"
   resolved "https://registry.yarnpkg.com/@types/minimist/-/minimist-1.2.2.tgz#ee771e2ba4b3dc5b372935d549fd9617bf345b8c"
   integrity sha512-jhuKLIRrhvCPLqwPcx6INqmKeiA5EWrsCOPhrlFSrbrmU4ZMPjj5Ul/oLCMDO98XRUIwVm78xICz4EPCektzeQ==
 
 "@types/node@*":
-  version "20.4.5"
-  resolved "https://registry.yarnpkg.com/@types/node/-/node-20.4.5.tgz#9dc0a5cb1ccce4f7a731660935ab70b9c00a5d69"
-  integrity sha512-rt40Nk13II9JwQBdeYqmbn2Q6IVTA5uPhvSO+JVqdXw/6/4glI6oR9ezty/A9Hg5u7JH4OmYmuQ+XvjKm0Datg==
+  version "20.4.8"
+  resolved "https://registry.yarnpkg.com/@types/node/-/node-20.4.8.tgz#b5dda19adaa473a9bf0ab5cbd8f30ec7d43f5c85"
+  integrity sha512-0mHckf6D2DiIAzh8fM8f3HQCvMKDpK94YQ0DSVkfWTG9BZleYIWudw9cJxX8oCk9bM+vAkDyujDV6dmKHbvQpg==
 
 "@types/normalize-package-data@^2.4.0":
   version "2.4.1"
   resolved "https://registry.yarnpkg.com/@types/normalize-package-data/-/normalize-package-data-2.4.1.tgz#d3357479a0fdfdd5907fe67e17e0a85c906e1301"
   integrity sha512-Gj7cI7z+98M282Tqmp2K5EIsoouUEzbBJhQQzDE3jSIRk6r9gsz0oUokqIUR4u1R3dMHo0pDHM7sNOHyhulypw==
 
 "@types/parse-json@^4.0.0":
@@ -3304,26 +3314,26 @@
 
 camelcase@^6.0.0, camelcase@^6.2.0:
   version "6.3.0"
   resolved "https://registry.yarnpkg.com/camelcase/-/camelcase-6.3.0.tgz#5685b95eb209ac9c0c177467778c9c84df58ba9a"
   integrity sha512-Gmy6FhYlCY7uOElZUSbxo2UCDH8owEk996gkbrpsgGtrJLM3J7jGxl9Ic7Qwwj4ivOE5AWZWRMecDdF7hqGjFA==
 
 caniuse-lite@^1.0.30001517:
-  version "1.0.30001518"
-  resolved "https://registry.yarnpkg.com/caniuse-lite/-/caniuse-lite-1.0.30001518.tgz#b3ca93904cb4699c01218246c4d77a71dbe97150"
-  integrity sha512-rup09/e3I0BKjncL+FesTayKtPrdwKhUufQFd3riFw1hHg8JmIFoInYfB102cFcY/pPgGmdyl/iy+jgiDi2vdA==
+  version "1.0.30001519"
+  resolved "https://registry.yarnpkg.com/caniuse-lite/-/caniuse-lite-1.0.30001519.tgz#3e7b8b8a7077e78b0eb054d69e6edf5c7df35601"
+  integrity sha512-0QHgqR+Jv4bxHMp8kZ1Kn8CH55OikjKJ6JmKkZYP1F3D7w+lnFXF70nG5eNfsZS89jadi5Ywy5UCSKLAglIRkg==
 
 capture-exit@^2.0.0:
   version "2.0.0"
   resolved "https://registry.yarnpkg.com/capture-exit/-/capture-exit-2.0.0.tgz#fb953bfaebeb781f62898239dabb426d08a509a4"
   integrity sha512-PiT/hQmTonHhl/HFGN+Lx3JJUznrVYJ3+AQsnthneZbvW7x+f08Tk7yLJTLEOUvBTbduLeeBkxEaYXUOUrRq6g==
   dependencies:
     rsvp "^4.8.4"
 
-chalk@^2.0.0, chalk@^2.3.0, chalk@^2.4.1:
+chalk@^2.3.0, chalk@^2.4.1, chalk@^2.4.2:
   version "2.4.2"
   resolved "https://registry.yarnpkg.com/chalk/-/chalk-2.4.2.tgz#cd42541677a54333cf541a49108c1432b44c9424"
   integrity sha512-Mti+f9lpJNcwF4tWV8/OrTTtF1gZi+f8FqlyAdouralcFWFQWF2+NgCHShjkCb+IFBLq9buZwE1xckQU4peSuQ==
   dependencies:
     ansi-styles "^3.2.1"
     escape-string-regexp "^1.0.5"
     supports-color "^5.3.0"
@@ -3896,17 +3906,17 @@
   dependencies:
     chalk "^2.3.0"
     find-root "^1.0.0"
     lodash "^4.17.4"
     semver "^5.4.1"
 
 electron-to-chromium@^1.4.477:
-  version "1.4.479"
-  resolved "https://registry.yarnpkg.com/electron-to-chromium/-/electron-to-chromium-1.4.479.tgz#ec9f676f23d3a0b0e429bc454d25e0b3253d2118"
-  integrity sha512-ABv1nHMIR8I5n3O3Een0gr6i0mfM+YcTZqjHy3pAYaOjgFG+BMquuKrSyfYf5CbEkLr9uM05RA3pOk4udNB/aQ==
+  version "1.4.487"
+  resolved "https://registry.yarnpkg.com/electron-to-chromium/-/electron-to-chromium-1.4.487.tgz#e2ef8b15f2791bf68fa6f38f2656f1a551d360ae"
+  integrity sha512-XbCRs/34l31np/p33m+5tdBrdXu9jJkZxSbNxj5I0H1KtV2ZMSB+i/HYqDiRzHaFx2T5EdytjoBRe8QRJE2vQg==
 
 emittery@^0.7.1:
   version "0.7.2"
   resolved "https://registry.yarnpkg.com/emittery/-/emittery-0.7.2.tgz#25595908e13af0f5674ab419396e2fb394cdfa82"
   integrity sha512-A8OG5SR/ij3SsJdWDJdkkSYUjQdCUx6APQXem0SaEePBSRg4eymGYwBkKo1Y6DU+af/Jn2dBQqDBvjnr9Vi8nQ==
 
 emittery@^0.8.1:
@@ -5139,18 +5149,18 @@
 is-ci@^2.0.0:
   version "2.0.0"
   resolved "https://registry.yarnpkg.com/is-ci/-/is-ci-2.0.0.tgz#6bc6334181810e04b5c22b3d589fdca55026404c"
   integrity sha512-YfJT7rkpQB0updsdHLGWrvhBJfcfzNNawYDNIyQXJz0IViGf75O8EBPKSdvw2rF+LGCsX4FZ8tcr3b19LcZq4w==
   dependencies:
     ci-info "^2.0.0"
 
-is-core-module@^2.11.0, is-core-module@^2.5.0:
-  version "2.12.1"
-  resolved "https://registry.yarnpkg.com/is-core-module/-/is-core-module-2.12.1.tgz#0c0b6885b6f80011c71541ce15c8d66cf5a4f9fd"
-  integrity sha512-Q4ZuBAe2FUsKtyQJoQHlvP8OvBERxO3jEmy1I7hcRXcJBGGHFh/aJBswbXuS9sgrDH2QUO8ilkwNPHvHMd8clg==
+is-core-module@^2.13.0, is-core-module@^2.5.0:
+  version "2.13.0"
+  resolved "https://registry.yarnpkg.com/is-core-module/-/is-core-module-2.13.0.tgz#bb52aa6e2cbd49a30c2ba68c42bf3435ba6072db"
+  integrity sha512-Z7dk6Qo8pOCp3l4tsX2C5ZVas4V+UxwQodwZhLopL91TX8UyyHEXafPcyoeeWuLrwzHcr3igO78wNLwHJHsMCQ==
   dependencies:
     has "^1.0.3"
 
 is-data-descriptor@^0.1.4:
   version "0.1.4"
   resolved "https://registry.yarnpkg.com/is-data-descriptor/-/is-data-descriptor-0.1.4.tgz#0b5ee648388e2c860282e793f1856fec3f301b56"
   integrity sha512-+w9D5ulSoBNlmw9OHn3U2v51SyoCd0he+bB3xMl62oijhrspxowjU+AIcDY0N3iEJbUEkB15IlMASQsxYigvXg==
@@ -7667,23 +7677,23 @@
     regenerate "^1.4.2"
 
 regenerate@^1.4.2:
   version "1.4.2"
   resolved "https://registry.yarnpkg.com/regenerate/-/regenerate-1.4.2.tgz#b9346d8827e8f5a32f7ba29637d398b69014848a"
   integrity sha512-zrceR/XhGYU/d/opr2EKO7aRHUeiBI8qjtfHqADTwZd6Szfy16la6kqD0MIUs5z5hx6AaKa+PixpPrR289+I0A==
 
-regenerator-runtime@^0.13.11:
-  version "0.13.11"
-  resolved "https://registry.yarnpkg.com/regenerator-runtime/-/regenerator-runtime-0.13.11.tgz#f6dca3e7ceec20590d07ada785636a90cdca17f9"
-  integrity sha512-kY1AZVr2Ra+t+piVaJ4gxaFaReZVH40AKNo7UCX6W+dEwBo/2oZJzqfuN1qLq1oL45o56cPaTXELwrTh8Fpggg==
-
-regenerator-transform@^0.15.1:
-  version "0.15.1"
-  resolved "https://registry.yarnpkg.com/regenerator-transform/-/regenerator-transform-0.15.1.tgz#f6c4e99fc1b4591f780db2586328e4d9a9d8dc56"
-  integrity sha512-knzmNAcuyxV+gQCufkYcvOqX/qIIfHLv0u5x79kRxuGojfYVky1f15TzZEu2Avte8QGepvUNTnLskf8E6X6Vyg==
+regenerator-runtime@^0.14.0:
+  version "0.14.0"
+  resolved "https://registry.yarnpkg.com/regenerator-runtime/-/regenerator-runtime-0.14.0.tgz#5e19d68eb12d486f797e15a3c6a918f7cec5eb45"
+  integrity sha512-srw17NI0TUWHuGa5CFGGmhfNIeja30WMBfbslPNhf6JrqQlLN5gcrvig1oqPxiVaXb0oW0XRKtH6Nngs5lKCIA==
+
+regenerator-transform@^0.15.2:
+  version "0.15.2"
+  resolved "https://registry.yarnpkg.com/regenerator-transform/-/regenerator-transform-0.15.2.tgz#5bbae58b522098ebdf09bca2f83838929001c7a4"
+  integrity sha512-hfMp2BoF0qOk3uc5V20ALGDS2ddjQaLrdl7xrGXvAIow7qeWRM2VA2HuCHkUKk9slq3VwEwLNK3DFBqDfPGYtg==
   dependencies:
     "@babel/runtime" "^7.8.4"
 
 regex-not@^1.0.0, regex-not@^1.0.2:
   version "1.0.2"
   resolved "https://registry.yarnpkg.com/regex-not/-/regex-not-1.0.2.tgz#1f4ece27e00b0b65e0247a6810e6a85d83a5752c"
   integrity sha512-J6SDjUgDxQj5NusnOtdFxDwN/+HWykR8GELwctJ7mdqhcyy1xEc4SRFHUXvxTp661YaVKAjfRLZ9cCqS6tn32A==
@@ -7793,19 +7803,19 @@
 
 resolve.exports@^1.1.0:
   version "1.1.1"
   resolved "https://registry.yarnpkg.com/resolve.exports/-/resolve.exports-1.1.1.tgz#05cfd5b3edf641571fd46fa608b610dda9ead999"
   integrity sha512-/NtpHNDN7jWhAaQ9BvBUYZ6YTXsRBgfqWFWP7BZBaoMJO/I3G5OFzvTuWNlZC3aPjins1F+TNrLKsGbH4rfsRQ==
 
 resolve@^1.10.0, resolve@^1.18.1, resolve@^1.20.0, resolve@^1.3.2, resolve@^1.9.0:
-  version "1.22.2"
-  resolved "https://registry.yarnpkg.com/resolve/-/resolve-1.22.2.tgz#0ed0943d4e301867955766c9f3e1ae6d01c6845f"
-  integrity sha512-Sb+mjNHOULsBv818T40qSPeRiuWLyaGMa5ewydRLFimneixmVy2zdivRl+AF6jaYPC8ERxGDmFSiqui6SfPd+g==
+  version "1.22.4"
+  resolved "https://registry.yarnpkg.com/resolve/-/resolve-1.22.4.tgz#1dc40df46554cdaf8948a486a10f6ba1e2026c34"
+  integrity sha512-PXNdCiPqDqeUou+w1C2eTQbNfxKSuMxqTCuvlmmMsk1NWHL5fRrhY6Pl0qEYYc6+QqGClco1Qj8XnjPego4wfg==
   dependencies:
-    is-core-module "^2.11.0"
+    is-core-module "^2.13.0"
     path-parse "^1.0.7"
     supports-preserve-symlinks-flag "^1.0.0"
 
 ret@~0.1.10:
   version "0.1.15"
   resolved "https://registry.yarnpkg.com/ret/-/ret-0.1.15.tgz#b8a4825d5bdb1fc3f6f53c2bc33f81388681c7bc"
   integrity sha512-TTlYpa+OL+vMMNG24xSlQGEJ3B/RzEfUlLct7b5G/ytav+wPrplCpVMFuwzXbkecJrb6IYo1iFb0S9v37754mg==
```

### Comparing `vdk_jupyterlab_extension-0.1.951673056/schema/plugin.json` & `vdk_jupyterlab_extension-0.1.959565555/schema/plugin.json`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.951673056/src/handler.ts` & `vdk_jupyterlab_extension-0.1.959565555/src/handler.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.951673056/src/index.ts` & `vdk_jupyterlab_extension-0.1.959565555/src/index.ts`

 * *Files 8% similar despite different names*

```diff
@@ -15,14 +15,18 @@
 import { IChangedArgs } from '@jupyterlab/coreutils';
 import { INotebookTracker } from '@jupyterlab/notebook';
 import { trackVdkTags } from './vdkTags';
 import { IThemeManager } from '@jupyterlab/apputils';
 import { IDocumentManager } from '@jupyterlab/docmanager';
 import { initVDKConfigCell } from './initVDKConfigCell';
 import { populateNotebook } from './components/ConvertJobToNotebook';
+import {
+  createStatusButton,
+  createStatusMenu
+} from './components/StatusButton';
 
 /**
  * Current working directory in Jupyter
  * The variable can be accessed anywhere in the JupyterFrontEndPlugin
  */
 export let workingDirectory: string = '';
 
@@ -55,17 +59,33 @@
       } else {
         //  * Populates notebook with provided content for convert job operation
         //  * Check src/components/ConvertJobToNotebook.tsx for more
         populateNotebook(notebookTracker);
       }
     });
 
+    createStatusMenu(commands);
+    const statusButton = createStatusButton(commands);
+
     const fileBrowser = factory.defaultBrowser;
 
-    updateVDKMenu(commands, docManager, fileBrowser, notebookTracker);
+    app.restored.then(() => {
+      const topPanel = document.querySelector('#jp-top-panel');
+      if (topPanel) {
+        topPanel.appendChild(statusButton.element);
+      }
+    });
+
+    updateVDKMenu(
+      commands,
+      docManager,
+      fileBrowser,
+      notebookTracker,
+      statusButton
+    );
 
     fileBrowser.model.pathChanged.connect(onPathChanged);
     trackVdkTags(notebookTracker, themeManager);
   }
 };
 
 export default plugin;
```

### Comparing `vdk_jupyterlab_extension-0.1.951673056/src/initVDKConfigCell.ts` & `vdk_jupyterlab_extension-0.1.959565555/src/initVDKConfigCell.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.951673056/src/jobData.ts` & `vdk_jupyterlab_extension-0.1.959565555/src/jobData.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.951673056/src/serverRequests.ts` & `vdk_jupyterlab_extension-0.1.959565555/src/serverRequests.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.951673056/src/vdkTags.ts` & `vdk_jupyterlab_extension-0.1.959565555/src/vdkTags.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.951673056/src/__tests__/convert-job-to-notebook-component.spec.ts` & `vdk_jupyterlab_extension-0.1.959565555/src/__tests__/convert-job-to-notebook-component.spec.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.951673056/src/__tests__/create-job-component.spec.ts` & `vdk_jupyterlab_extension-0.1.959565555/src/__tests__/create-job-component.spec.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.951673056/src/__tests__/deploy-job-component.spec.ts` & `vdk_jupyterlab_extension-0.1.959565555/src/__tests__/deploy-job-component.spec.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.951673056/src/__tests__/download-job-component.spec.ts` & `vdk_jupyterlab_extension-0.1.959565555/src/__tests__/download-job-component.spec.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.951673056/src/__tests__/handler.spec.ts` & `vdk_jupyterlab_extension-0.1.959565555/src/__tests__/handler.spec.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.951673056/src/__tests__/resquests.spec.ts` & `vdk_jupyterlab_extension-0.1.959565555/src/__tests__/resquests.spec.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.951673056/src/__tests__/run-job-component.spec.tsx` & `vdk_jupyterlab_extension-0.1.959565555/src/__tests__/run-job-component.spec.tsx`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 /*
  * Copyright 2023-2023 VMware, Inc.
  * SPDX-License-Identifier: Apache-2.0
  */
-import RunJobDialog, { findFailingCellId, getCellInputAreaPromp, handleErrorsProducedByNotebookCell } from '../components/RunJob';
+import RunJobDialog, { findFailingCellId, getCellInputAreaPrompt, handleErrorsProducedByNotebookCell } from '../components/RunJob';
 import { render, fireEvent } from '@testing-library/react';
 import { jobData } from '../jobData';
 import { VdkOption } from '../vdkOptions/vdk_options';
 import { IJobPathProp } from '../components/props';
 import { VdkErrorMessage } from '../components/VdkErrorMessage';
 import { IDocumentManager } from '@jupyterlab/docmanager';
 
@@ -135,44 +135,44 @@
 
     expect(docManager.openOrReveal).toHaveBeenCalledWith('/path/to/notebook.ipynb');
     expect(result).toBe(true);
   });
 
 });
 
-describe('getCellInputAreaPromp', () => {
+describe('getCellInputAreaPrompt', () => {
   test('returns the prompt element when it exists', () => {
     const mockPromptElement = document.createElement('div');
     mockPromptElement.classList.add('jp-InputArea-prompt');
 
     const mockCellInputArea = document.createElement('div');
     mockCellInputArea.classList.add('jp-Cell-inputArea');
     mockCellInputArea.appendChild(mockPromptElement);
 
     const mockCellInputWrapper = document.createElement('div');
     mockCellInputWrapper.classList.add('jp-Cell-inputWrapper');
     mockCellInputWrapper.appendChild(mockCellInputArea);
 
-    const mockFailinCell = document.createElement('div');
-    mockFailinCell.appendChild(mockCellInputWrapper);
+    const mockFailingCell = document.createElement('div');
+    mockFailingCell.appendChild(mockCellInputWrapper);
 
-    const result = getCellInputAreaPromp(mockFailinCell);
+    const result = getCellInputAreaPrompt(mockFailingCell);
 
     expect(result).toBe(mockPromptElement);
   });
 
   test('returns undefined when prompt element does not exist', () => {
     const mockCellInputArea = document.createElement('div');
     mockCellInputArea.classList.add('jp-Cell-inputArea');
 
     const mockCellInputWrapper = document.createElement('div');
     mockCellInputWrapper.classList.add('jp-Cell-inputWrapper');
     mockCellInputWrapper.appendChild(mockCellInputArea);
 
-    const mockFailinCell = document.createElement('div');
-    mockFailinCell.appendChild(mockCellInputWrapper);
+    const mockFailingCell = document.createElement('div');
+    mockFailingCell.appendChild(mockCellInputWrapper);
 
-    const result = getCellInputAreaPromp(mockFailinCell);
+    const result = getCellInputAreaPrompt(mockFailingCell);
 
     expect(result).toBeUndefined();
   });
 });
```

### Comparing `vdk_jupyterlab_extension-0.1.951673056/src/__tests__/show-dialog.spec.tsx` & `vdk_jupyterlab_extension-0.1.959565555/src/__tests__/show-dialog.spec.tsx`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.951673056/src/__tests__/vdk-error-message.spec.ts` & `vdk_jupyterlab_extension-0.1.959565555/src/__tests__/vdk-error-message.spec.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.951673056/src/__tests__/vdk-tags.spec.ts` & `vdk_jupyterlab_extension-0.1.959565555/src/__tests__/vdk-tags.spec.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.951673056/src/components/ConvertJobToNotebook.tsx` & `vdk_jupyterlab_extension-0.1.959565555/src/components/ConvertJobToNotebook.tsx`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 import React, { Component } from 'react';
 import { jobData } from '../jobData';
 import { VdkOption } from '../vdkOptions/vdk_options';
 import VDKTextInput from './VdkTextInput';
 import { Dialog, showDialog, showErrorMessage } from '@jupyterlab/apputils';
-import { getServerDirRequest, jobConvertToNotebookRequest } from '../serverRequests';
+import {
+  getServerDirRequest,
+  jobConvertToNotebookRequest
+} from '../serverRequests';
 import { VdkErrorMessage } from './VdkErrorMessage';
 import { CONVERT_JOB_TO_NOTEBOOK_BUTTON_LABEL } from '../utils';
 import { CommandRegistry } from '@lumino/commands';
 import { FileBrowser } from '@jupyterlab/filebrowser';
 import { INotebookTracker } from '@jupyterlab/notebook';
-import {  IJobPathProp, JupyterCellProps } from './props';
-
+import { IJobPathProp, JupyterCellProps } from './props';
+import { StatusButton } from './StatusButton';
 
 export var notebookContent: JupyterCellProps[];
 
 /**
  * A class responsible for the Transform Job operation
  * for more information check:
  * https://github.com/vmware/versatile-data-kit/wiki/VDK-Jupyter-Integration-Convert-Job-Operation
  */
-export default class ConvertJobToNotebookDialog extends Component<IJobPathProp> {
+export default class ConvertJobToNotebookDialog extends Component<
+  IJobPathProp
+> {
   /**
    * Returns a React component for rendering a convert menu.
    *
    * @param props - component properties
    * @returns React component
    */
   constructor(props: IJobPathProp) {
@@ -43,16 +48,20 @@
           label="Path to job directory:"
         ></VDKTextInput>
       </>
     );
   }
 }
 
-export async function showConvertJobToNotebookDialog(commands: CommandRegistry,
-  fileBrowser: FileBrowser, notebookTracker: INotebookTracker): Promise<void> {
+export async function showConvertJobToNotebookDialog(
+  commands: CommandRegistry,
+  fileBrowser: FileBrowser,
+  notebookTracker: INotebookTracker,
+  statusButton?: StatusButton
+): Promise<void> {
   const result = await showDialog({
     title: CONVERT_JOB_TO_NOTEBOOK_BUTTON_LABEL,
     body: (
       <ConvertJobToNotebookDialog
         jobPath={jobData.get(VdkOption.PATH)!}
       ></ConvertJobToNotebookDialog>
     ),
@@ -66,18 +75,22 @@
           Are you sure you want to convert the Data Job with path:{' '}
           <i>{jobData.get(VdkOption.PATH)}</i> to notebook?
         </p>
       ),
       buttons: [Dialog.okButton(), Dialog.cancelButton()]
     });
     if (confirmation.button.accept) {
+      statusButton?.show('Convert', jobData.get(VdkOption.PATH)!);
       let { message, status } = await jobConvertToNotebookRequest();
       if (status) {
         const transformjobResult = JSON.parse(message);
-        notebookContent  = initializeNotebookContent(transformjobResult["code_structure"], transformjobResult["removed_files"])
+        notebookContent = initializeNotebookContent(
+          transformjobResult['code_structure'],
+          transformjobResult['removed_files']
+        );
         await createTranformedNotebook(commands, fileBrowser, notebookTracker);
         await showDialog({
           title: CONVERT_JOB_TO_NOTEBOOK_BUTTON_LABEL,
           body: (
             <div className="vdk-convert-to-notebook-dialog-message-container">
               <p className="vdk-convert-to-notebook-dialog-message">
                 The Data Job with path <i>{jobData.get(VdkOption.PATH)}</i> was
@@ -118,172 +131,191 @@
  *
  * @param {JupyterCellProps[]} notebookContent - The content to populate the notebook with.
  * @param {CommandRegistry} commands - The command registry to execute Jupyter commands.
  * @param {FileBrowser} fileBrowser - The file browser to navigate the file system.
  * @param {INotebookTracker} notebookTracker - The notebook tracker to track changes to the notebook.
  */
 export const createTranformedNotebook = async (
-  commands: CommandRegistry, fileBrowser: FileBrowser, notebookTracker: INotebookTracker) => {
+  commands: CommandRegistry,
+  fileBrowser: FileBrowser,
+  notebookTracker: INotebookTracker
+) => {
   try {
     const baseDir = await getServerDirRequest();
-    jobData.set(VdkOption.NAME,
-      jobData.get(VdkOption.PATH)!.split(/[\\/]/).pop() || ""); //get the name of the job using the directory
-    await fileBrowser.model.cd(jobData.get(VdkOption.PATH)!.substring(baseDir.length));  // relative path for Jupyter
+    jobData.set(
+      VdkOption.NAME,
+      jobData.get(VdkOption.PATH)!.split(/[\\/]/).pop() || ''
+    ); //get the name of the job using the directory
+    await fileBrowser.model.cd(
+      jobData.get(VdkOption.PATH)!.substring(baseDir.length)
+    ); // relative path for Jupyter
     commands.execute('notebook:create-new');
-  }
-  catch (error) {
+  } catch (error) {
     await showErrorMessage(
       'Something went wrong while trying to create the new transformed notebook. Error:',
       error,
       [Dialog.okButton()]
     );
   }
-}
-
+};
 
 /**
  * Initializes notebook content.
  *
  * The function takes code and filenames as parameters and generates a structured notebook content.
  * The code blocks are turned into notebook cells.
  *
  * @param {string[]} codeStructure - The code blocks to turn into notebook cells.
  * @param {string[]} fileNames - The names of the files to turn into titles.
  * @return {JupyterCellProps[]} - The structured content ready to be used to populate a notebook.
  */
-export const initializeNotebookContent = (codeStructure: string[], fileNames: string[]): JupyterCellProps[] => {
+export const initializeNotebookContent = (
+  codeStructure: string[],
+  fileNames: string[]
+): JupyterCellProps[] => {
   const notebookContent: JupyterCellProps[] = [];
 
   for (let i = 0; i < codeStructure.length; i++) {
     notebookContent.push({
-      source: "#### " + fileNames[i], // make names bolder
+      source: '#### ' + fileNames[i], // make names bolder
       type: 'markdown'
     });
     notebookContent.push({
       source: codeStructure[i],
       type: 'code'
     });
     if (codeStructure[i].includes('def run(job_input: IJobInput)')) {
       notebookContent.push({
         source: 'run(job_input)',
         type: 'code'
       });
     }
   }
   return notebookContent;
-}
+};
 
 /**
  * Populates notebook with provided content.
  *
  * The function takes notebook content and a notebook tracker as parameters.
  * When a new notebook becomes active, it is populated with the provided content.
  * @param {INotebookTracker} notebookTracker - The notebook tracker to track changes to the notebook.
  */
 export const populateNotebook = async (notebookTracker: INotebookTracker) => {
-    const notebookPanel = notebookTracker.currentWidget;
-    if (notebookPanel) {
-      const cells = notebookTracker.currentWidget?.content.model?.cells;
-      const cellContent = cells?.get(0).value.text;
-      // check if the notebook has only 1 empty cell, which is how we judge if it is a new notebook or not
-      if (cells && cells.length <= 1 && cellContent == '') {
-        cells.remove(1);
-
-        const addMarkdownCell = (source: string[]) => {
-          const markdownCell = notebookPanel.content.model?.contentFactory?.createMarkdownCell({
+  const notebookPanel = notebookTracker.currentWidget;
+  if (notebookPanel) {
+    const cells = notebookTracker.currentWidget?.content.model?.cells;
+    const cellContent = cells?.get(0).value.text;
+    // check if the notebook has only 1 empty cell, which is how we judge if it is a new notebook or not
+    if (cells && cells.length <= 1 && cellContent == '') {
+      cells.remove(1);
+
+      const addMarkdownCell = (source: string[]) => {
+        const markdownCell = notebookPanel.content.model?.contentFactory?.createMarkdownCell(
+          {
             cell: {
               cell_type: 'markdown',
               source: source,
               metadata: {}
             }
-          });
-          if (markdownCell) cells.push(markdownCell);
+          }
+        );
+        if (markdownCell) {
+          cells.push(markdownCell);
         }
+      };
 
-        const addCodeCell = (source: string[], metadata: {}) => {
-          const codeCell = notebookPanel.content.model?.contentFactory?.createCodeCell({
+      const addCodeCell = (source: string[], metadata: {}) => {
+        const codeCell = notebookPanel.content.model?.contentFactory?.createCodeCell(
+          {
             cell: {
               cell_type: 'code',
               source: source,
               metadata: metadata
             }
-          });
-          if (codeCell) cells.push(codeCell);
-        }
-        addMarkdownCell([
-          "# " + jobData.get(VdkOption.NAME)
-        ]);
-
-        addMarkdownCell([
-          "### Please go through this guide before continuing with the data job run and development."
-        ]);
-
-        addMarkdownCell([
-          "#### Introduction and Preparations\n",
-          "*  *This is a notebook transformed from a directory style data job located in " + jobData.get(VdkOption.PATH) + ".*\n",
-          "*  *If you are not familiar with notebook data jobs make sure to check the **Getting Started**(TODO: add link) page.*\n",
-          "*  *You can find the **original job** at " + jobData.get(VdkOption.PATH)!.split(/[/\\]/).slice(0, -1).join('/') + ".*"
-        ]);
-
-        addMarkdownCell([
-          "#### Execution Order and Identifying Cells\n",
-          "*  *The below cells are automatically generated corresponding to a step(.sql or .py file with VDK run function) \n",
-          "    in your original job.* \n",
-          "*  *You will notice that some cells are coloured and include the VDK logo and a numbering. \n",
-          "    These are the \"vdk\" tagged cells.\n",
-          "    Only these cells are executed during VDK run and all the others are ignored(for example the current cell).*\n",
-          "*  *Code cells in the notebook will be executed according to the numbering when running the notebook data job with VDK.\n",
-          "    This means that the steps in the job are organized from the top to the bottom, starting with the first step.*\n",
-          "*  *When you see a title saying **\"Step generated from: sample.py\"** before some blocks of code, \n",
-          "    it means that the code below that title was created from the \"sample.py\" file.*\n",
-          "*  *Similarly, if you come across code cells that have the format **\"job_input.execute_query(query_string)\"** ,\n",
-          "    it means that those cells contain code generated from \".sql\" files.*\n",
-          "*  *On the other hand, code cells originating from \".py\" files remain unchanged.\n",
-          "    However, an additional cell is included that calls the \"run\" function using the command **\"run(job_input)\"** . \n",
-          "    This cell executes the \"run\" function from the code generated from the \".py\" file.*\n",
-          "*  *You can delete the cells that are not tagged with \"vdk\" \n",
-          "    as they are not essential to the data job's execution.\n",
-          "    However, removing tagged cells will result in a different data job run.* "
-        ]);
-
-        addMarkdownCell([
-          "#### Tips: \n",
-          "* *Before running the job, it is recommended to review the cells\n",
-          "    to ensure a clear understanding of the data job run.  \n",
-          "    This will help to ensure the desired outcome.* "
-        ]);
-
-        addCodeCell([
-          `"""\n`,
-          `vdk.plugin.ipython extension introduces a magic command for Jupyter.\n`,
-          `The command enables the user to load VDK for the current notebook.\n`,
-          `VDK provides the job_input API, which has methods for:\n`,
-          `    * executing queries to an OLAP database;\n`,
-          `    * ingesting data into a database;\n`,
-          `    * processing data into a database.\n`,
-          `See the IJobInput documentation for more details.\n`,
-          `https://github.com/vmware/versatile-data-kit/blob/main/projects/vdk-core/src/vdk/api/job_input.py\n`,
-          `Please refrain from tagging this cell with VDK as it is not an actual part of the data job\n`,
-          `and is only used for development purposes.\n`,
-          `"""\n`,
-          `%reload_ext vdk.plugin.ipython\n`,
-          `%reload_VDK\n`,
-          `job_input = VDK.get_initialized_job_input()`
-        ], {})
-
-        // add code that came from the previous version of the job and the names of the files where they came from
-        for (const cellProps of notebookContent) {
-          if (cellProps.type === 'markdown') {
-            addMarkdownCell([cellProps.source])
-          } else if (cellProps.type === 'code') {
-            addCodeCell([cellProps.source], {
-              "tags": [
-                "vdk"
-              ]
-            })
           }
+        );
+        if (codeCell) {
+          cells.push(codeCell);
         }
+      };
+      addMarkdownCell(['# ' + jobData.get(VdkOption.NAME)]);
 
-        notebookContent = [];
+      addMarkdownCell([
+        '### Please go through this guide before continuing with the data job run and development.'
+      ]);
+
+      addMarkdownCell([
+        '#### Introduction and Preparations\n',
+        '*  *This is a notebook transformed from a directory style data job located in ' +
+          jobData.get(VdkOption.PATH) +
+          '.*\n',
+        '*  *If you are not familiar with notebook data jobs make sure to check the **Getting Started**(TODO: add link) page.*\n',
+        '*  *You can find the **original job** at ' +
+          jobData.get(VdkOption.PATH)!.split(/[/\\]/).slice(0, -1).join('/') +
+          '.*'
+      ]);
+
+      addMarkdownCell([
+        '#### Execution Order and Identifying Cells\n',
+        '*  *The below cells are automatically generated corresponding to a step(.sql or .py file with VDK run function) \n',
+        '    in your original job.* \n',
+        '*  *You will notice that some cells are coloured and include the VDK logo and a numbering. \n',
+        '    These are the "vdk" tagged cells.\n',
+        '    Only these cells are executed during VDK run and all the others are ignored(for example the current cell).*\n',
+        '*  *Code cells in the notebook will be executed according to the numbering when running the notebook data job with VDK.\n',
+        '    This means that the steps in the job are organized from the top to the bottom, starting with the first step.*\n',
+        '*  *When you see a title saying **"Step generated from: sample.py"** before some blocks of code, \n',
+        '    it means that the code below that title was created from the "sample.py" file.*\n',
+        '*  *Similarly, if you come across code cells that have the format **"job_input.execute_query(query_string)"** ,\n',
+        '    it means that those cells contain code generated from ".sql" files.*\n',
+        '*  *On the other hand, code cells originating from ".py" files remain unchanged.\n',
+        '    However, an additional cell is included that calls the "run" function using the command **"run(job_input)"** . \n',
+        '    This cell executes the "run" function from the code generated from the ".py" file.*\n',
+        '*  *You can delete the cells that are not tagged with "vdk" \n',
+        "    as they are not essential to the data job's execution.\n",
+        '    However, removing tagged cells will result in a different data job run.* '
+      ]);
+
+      addMarkdownCell([
+        '#### Tips: \n',
+        '* *Before running the job, it is recommended to review the cells\n',
+        '    to ensure a clear understanding of the data job run.  \n',
+        '    This will help to ensure the desired outcome.* '
+      ]);
+
+      addCodeCell(
+        [
+          '"""\n',
+          'vdk.plugin.ipython extension introduces a magic command for Jupyter.\n',
+          'The command enables the user to load VDK for the current notebook.\n',
+          'VDK provides the job_input API, which has methods for:\n',
+          '    * executing queries to an OLAP database;\n',
+          '    * ingesting data into a database;\n',
+          '    * processing data into a database.\n',
+          'See the IJobInput documentation for more details.\n',
+          'https://github.com/vmware/versatile-data-kit/blob/main/projects/vdk-core/src/vdk/api/job_input.py\n',
+          'Please refrain from tagging this cell with VDK as it is not an actual part of the data job\n',
+          'and is only used for development purposes.\n',
+          '"""\n',
+          '%reload_ext vdk.plugin.ipython\n',
+          '%reload_VDK\n',
+          'job_input = VDK.get_initialized_job_input()'
+        ],
+        {}
+      );
+
+      // add code that came from the previous version of the job and the names of the files where they came from
+      for (const cellProps of notebookContent) {
+        if (cellProps.type === 'markdown') {
+          addMarkdownCell([cellProps.source]);
+        } else if (cellProps.type === 'code') {
+          addCodeCell([cellProps.source], {
+            tags: ['vdk']
+          });
+        }
       }
+
+      notebookContent = [];
     }
-}
+  }
+};
```

### Comparing `vdk_jupyterlab_extension-0.1.951673056/src/components/CreateJob.tsx` & `vdk_jupyterlab_extension-0.1.959565555/src/components/CreateJob.tsx`

 * *Files 12% similar despite different names*

```diff
@@ -2,16 +2,17 @@
 import { jobData } from '../jobData';
 import { VdkOption } from '../vdkOptions/vdk_options';
 import VDKTextInput from './VdkTextInput';
 import { Dialog, showDialog } from '@jupyterlab/apputils';
 import { jobRequest } from '../serverRequests';
 import { IJobFullProps } from './props';
 import { CREATE_JOB_BUTTON_LABEL } from '../utils';
+import { StatusButton } from './StatusButton';
 
-export default class CreateJobDialog extends Component<(IJobFullProps)> {
+export default class CreateJobDialog extends Component<IJobFullProps> {
   /**
    * Returns a React component for rendering a create menu.
    *
    * @param props - component properties
    * @returns React component
    */
   constructor(props: IJobFullProps) {
@@ -85,15 +86,15 @@
       this.setJobFlags('Cloud');
     };
   }
   /**
    * Function that sets job's cloud/local flags
    */
   private setJobFlags(flag: string) {
-    let checkbox = document.getElementById(flag);
+    const checkbox = document.getElementById(flag);
     if (checkbox?.classList.contains('checked')) {
       checkbox.classList.remove('checked');
       if (flag === 'Cloud') {
         jobData.set(VdkOption.CLOUD, '');
       } else {
         jobData.set(VdkOption.LOCAL, '');
       }
@@ -104,23 +105,24 @@
       } else {
         jobData.set(VdkOption.LOCAL, '1');
       }
     }
   }
 }
 
-export async function showCreateJobDialog() {
+export async function showCreateJobDialog(statusButton?: StatusButton) {
   const result = await showDialog({
     title: CREATE_JOB_BUTTON_LABEL,
     body: (
       <CreateJobDialog
         jobPath={jobData.get(VdkOption.PATH)!}
         jobName={jobData.get(VdkOption.NAME)!}
         jobTeam={jobData.get(VdkOption.TEAM)!}
       ></CreateJobDialog>
     ),
     buttons: [Dialog.okButton(), Dialog.cancelButton()]
   });
   if (result.button.accept) {
+    statusButton?.show('Create', jobData.get(VdkOption.PATH)!);
     await jobRequest('create');
   }
 }
```

### Comparing `vdk_jupyterlab_extension-0.1.951673056/src/components/DeployJob.tsx` & `vdk_jupyterlab_extension-0.1.959565555/src/components/DeployJob.tsx`

 * *Files 16% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import { checkIfVdkOptionDataIsDefined, jobData } from '../jobData';
 import { VdkOption } from '../vdkOptions/vdk_options';
 import VDKTextInput from './VdkTextInput';
 import { Dialog, showDialog, showErrorMessage } from '@jupyterlab/apputils';
 import { jobRequest, jobRunRequest } from '../serverRequests';
 import { IJobFullProps } from './props';
 import { CREATE_DEP_BUTTON_LABEL } from '../utils';
+import { StatusButton } from './StatusButton';
 
 export default class DeployJobDialog extends Component<IJobFullProps> {
   /**
    * Returns a React component for rendering a Deploy menu.
    *
    * @param props - component properties
    * @returns React component
@@ -46,15 +47,15 @@
           label="Deployment reason:"
         ></VDKTextInput>
       </>
     );
   }
 }
 
-export async function showCreateDeploymentDialog() {
+export async function showCreateDeploymentDialog(statusButton?: StatusButton) {
   const result = await showDialog({
     title: CREATE_DEP_BUTTON_LABEL,
     body: (
       <DeployJobDialog
         jobName={jobData.get(VdkOption.NAME)!}
         jobPath={jobData.get(VdkOption.PATH)!}
         jobTeam={jobData.get(VdkOption.TEAM)!}
@@ -70,23 +71,24 @@
         body: 'The job will be executed once before deployment.',
         buttons: [
           Dialog.cancelButton({ label: 'Cancel' }),
           Dialog.okButton({ label: 'Continue' })
         ]
       });
       if (runConfirmationResult.button.accept) {
+        statusButton?.show('Deploy', jobData.get(VdkOption.PATH)!);
         const { message, status } = await jobRunRequest();
         if (status) {
           if (
             await checkIfVdkOptionDataIsDefined(VdkOption.DEPLOYMENT_REASON)
           ) {
             await jobRequest('deploy');
           }
         } else {
-          showErrorMessage(
+          await showErrorMessage(
             'Encоuntered an error while running the job!',
             message,
             [Dialog.okButton()]
           );
         }
       }
     } catch (error) {
```

### Comparing `vdk_jupyterlab_extension-0.1.951673056/src/components/DownloadJob.tsx` & `vdk_jupyterlab_extension-0.1.959565555/src/components/DownloadJob.tsx`

 * *Files 13% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import { VdkOption } from '../vdkOptions/vdk_options';
 import VDKTextInput from './VdkTextInput';
 import { Dialog, showDialog } from '@jupyterlab/apputils';
 import { jobRequest } from '../serverRequests';
 import { IJobPathProp } from './props';
 import { jobData } from '../jobData';
 import { DOWNLOAD_JOB_BUTTON_LABEL } from '../utils';
+import { StatusButton } from './StatusButton';
 
 export default class DownloadJobDialog extends Component<IJobPathProp> {
   /**
    * Returns a React component for rendering a download menu.
    *
    * @param props - component properties
    * @returns React component
@@ -41,21 +42,22 @@
           label="Path to job directory:"
         ></VDKTextInput>
       </>
     );
   }
 }
 
-export async function showDownloadJobDialog() {
+export async function showDownloadJobDialog(statusButton?: StatusButton) {
   const result = await showDialog({
     title: DOWNLOAD_JOB_BUTTON_LABEL,
     body: (
       <DownloadJobDialog
         jobPath={jobData.get(VdkOption.PATH)!}
       ></DownloadJobDialog>
     ),
     buttons: [Dialog.okButton(), Dialog.cancelButton()]
   });
   if (result.button.accept) {
+    statusButton?.show('Download', jobData.get(VdkOption.PATH)!);
     await jobRequest('download');
   }
 }
```

### Comparing `vdk_jupyterlab_extension-0.1.951673056/src/components/RunJob.tsx` & `vdk_jupyterlab_extension-0.1.959565555/src/components/RunJob.tsx`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import VDKTextInput from './VdkTextInput';
 import { Dialog, showDialog } from '@jupyterlab/apputils';
 import { getNotebookInfo, jobRunRequest } from '../serverRequests';
 import { IJobPathProp } from './props';
 import { VdkErrorMessage } from './VdkErrorMessage';
 import { IDocumentManager } from '@jupyterlab/docmanager';
 import { RUN_FAILED_BUTTON_LABEL, RUN_JOB_BUTTON_LABEL } from '../utils';
+import { StatusButton } from './StatusButton';
 
 export default class RunJobDialog extends Component<IJobPathProp> {
   /**
    * Returns a React component for rendering a run menu.
    *
    * @param props - component properties
    * @returns React component
@@ -68,21 +69,25 @@
       return true;
     } catch (e) {
       return false;
     }
   };
 }
 
-export async function showRunJobDialog(docManager?: IDocumentManager) {
+export async function showRunJobDialog(
+  docManager?: IDocumentManager,
+  statusButton?: StatusButton
+) {
   const result = await showDialog({
     title: RUN_JOB_BUTTON_LABEL,
     body: <RunJobDialog jobPath={jobData.get(VdkOption.PATH)!}></RunJobDialog>,
     buttons: [Dialog.okButton(), Dialog.cancelButton()]
   });
   if (result.button.accept) {
+    statusButton?.show('Run', jobData.get(VdkOption.PATH)!);
     let { message, status } = await jobRunRequest();
     if (status) {
       showDialog({
         title: RUN_JOB_BUTTON_LABEL,
         body: (
           <div className="vdk-run-dialog-message-container">
             <p className="vdk-run-dialog-message">
@@ -121,22 +126,22 @@
   const regex = /cell_id:([0-9a-fA-F-]+)/;
   const match = message.match(regex);
   if (match) return match[1];
   return '';
 };
 
 /**
- * Returns a Element that is used for numarating cell executions on Jupyter (text with [] if not executed and  with [1], [2] if executed)
+ * Returns a Element that is used for numerating cell executions on Jupyter (text with [] if not executed and  with [1], [2] if executed)
  * @param failingCell - parent cell of that element
  * @returns Element or undefined if the element could not be found
  */
-export const getCellInputAreaPromp = (
-  failinCell: Element
+export const getCellInputAreaPrompt = (
+  failingCell: Element
 ): Element | undefined => {
-  const cellInputWrappers = failinCell.getElementsByClassName(
+  const cellInputWrappers = failingCell.getElementsByClassName(
     'jp-Cell-inputWrapper'
   );
   for (let i = 0; i < cellInputWrappers.length; i++) {
     const cellAreas =
       cellInputWrappers[i].getElementsByClassName('jp-Cell-inputArea');
     if (cellAreas.length > 0) {
       const cellInputArea = cellAreas[0];
@@ -147,15 +152,15 @@
         return promptElements[0];
       }
     }
   }
 };
 
 const switchToFailingCell = (failingCell: Element) => {
-  const prompt = getCellInputAreaPromp(failingCell);
+  const prompt = getCellInputAreaPrompt(failingCell);
   prompt?.classList.add('jp-vdk-failing-cell-prompt');
   failingCell.scrollIntoView();
   failingCell.classList.add('jp-vdk-failing-cell');
   // Delete previous fail numbering
   const vdkFailingCellNums = Array.from(
     document.getElementsByClassName('jp-vdk-failing-cell-num')
   );
@@ -163,16 +168,16 @@
     element.classList.remove('jp-vdk-failing-cell-num');
     element.classList.add('jp-vdk-cell-num');
   });
 };
 
 const unmarkOldFailingCells = (cell: Element) => {
   cell.classList.remove('jp-vdk-failing-cell');
-  const cellPropt = getCellInputAreaPromp(cell);
-  cellPropt?.classList.remove('jp-vdk-failing-cell-prompt');
+  const cellPrompt = getCellInputAreaPrompt(cell);
+  cellPrompt?.classList.remove('jp-vdk-failing-cell-prompt');
 };
 
 export const findFailingCellInNotebookCells = async (
   element: Element,
   failingCellIndex: Number,
   nbPath: string
 ) => {
@@ -248,15 +253,15 @@
         buttons: [
           Dialog.okButton({ label: 'See failing cell' }),
           Dialog.cancelButton()
         ]
       });
 
       if (result.button.accept) {
-        navigateToFailingCell();
+        await navigateToFailingCell();
       }
 
       return true;
     }
   }
 
   return false;
```

### Comparing `vdk_jupyterlab_extension-0.1.951673056/src/components/VdkErrorMessage.ts` & `vdk_jupyterlab_extension-0.1.959565555/src/components/VdkErrorMessage.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.951673056/src/components/VdkTextInput.tsx` & `vdk_jupyterlab_extension-0.1.959565555/src/components/VdkTextInput.tsx`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.951673056/style/base.css` & `vdk_jupyterlab_extension-0.1.959565555/style/base.css`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.951673056/style/vdkDialogs.css` & `vdk_jupyterlab_extension-0.1.959565555/style/vdkDialogs.css`

 * *Files 14% similar despite different names*

```diff
@@ -52,7 +52,36 @@
   font-size: 20px;
   color: #33b53a;
   padding: 20px;
 }
 .vdk-run-dialog-message-container {
   position: relative;
 }
+
+.vdk-status-dialog-message {
+  font-size: 20px;
+  padding: 20px;
+}
+.vdk-status-dialog-message-container {
+  position: relative;
+}
+
+.jp-vdk-check-status-button {
+  position: absolute;
+  right: 1px;
+  border-radius: 5px;
+}
+
+.jp-vdk-status-button-content {
+  display: flex;
+  align-items: center;
+}
+
+.jp-vdk-check-status-button .jp-vdk-logo {
+  position: static;
+  padding-right: 5px;
+}
+
+.jp-vdk-check-status-button:hover {
+  background-color: #e0e0e0;
+  cursor: pointer;
+}
```

### Comparing `vdk_jupyterlab_extension-0.1.951673056/style/images/versatile-data-kit-logo.svg` & `vdk_jupyterlab_extension-0.1.959565555/style/images/versatile-data-kit-logo.svg`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.951673056/ui-tests/README.md` & `vdk_jupyterlab_extension-0.1.959565555/ui-tests/README.md`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.951673056/ui-tests/jupyter_server_test_config.py` & `vdk_jupyterlab_extension-0.1.959565555/ui-tests/jupyter_server_test_config.py`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.951673056/ui-tests/tests/convert-job.spec.ts` & `vdk_jupyterlab_extension-0.1.959565555/ui-tests/tests/convert-job.spec.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.951673056/ui-tests/tests/vdk-jupyterlab-extension.spec.ts` & `vdk_jupyterlab_extension-0.1.959565555/ui-tests/tests/vdk-jupyterlab-extension.spec.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.951673056/ui-tests/tests/data/convert-test-job-dirty/30_ingest_to_table.py` & `vdk_jupyterlab_extension-0.1.959565555/ui-tests/tests/data/convert-test-job-dirty/30_ingest_to_table.py`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.951673056/vdk_jupyterlab_extension/__init__.py` & `vdk_jupyterlab_extension-0.1.959565555/vdk_jupyterlab_extension/__init__.py`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.951673056/vdk_jupyterlab_extension/convert_job.py` & `vdk_jupyterlab_extension-0.1.959565555/vdk_jupyterlab_extension/convert_job.py`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.951673056/vdk_jupyterlab_extension/handlers.py` & `vdk_jupyterlab_extension-0.1.959565555/vdk_jupyterlab_extension/handlers.py`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.951673056/vdk_jupyterlab_extension/job_data.py` & `vdk_jupyterlab_extension-0.1.959565555/vdk_jupyterlab_extension/job_data.py`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.951673056/vdk_jupyterlab_extension/vdk_ui.py` & `vdk_jupyterlab_extension-0.1.959565555/vdk_jupyterlab_extension/vdk_ui.py`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.951673056/vdk_jupyterlab_extension/jupyter_sample_job/10_notebook.ipynb` & `vdk_jupyterlab_extension-0.1.959565555/vdk_jupyterlab_extension/jupyter_sample_job/10_notebook.ipynb`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.951673056/vdk_jupyterlab_extension/jupyter_sample_job/README.md` & `vdk_jupyterlab_extension-0.1.959565555/vdk_jupyterlab_extension/jupyter_sample_job/README.md`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.951673056/vdk_jupyterlab_extension/jupyter_sample_job/config.ini` & `vdk_jupyterlab_extension-0.1.959565555/vdk_jupyterlab_extension/jupyter_sample_job/config.ini`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.951673056/vdk_jupyterlab_extension/labextension/package.json` & `vdk_jupyterlab_extension-0.1.959565555/vdk_jupyterlab_extension/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9761363636363637%*

 * *Differences: {"'dependencies'": "{'@jupyterlab/mainmenu': '3.6.3'}",*

 * * "'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.4fde18a81e31cc9c2aa5.js'}}",*

 * * "'version'": "'0.1.959565555'"}*

```diff
@@ -15,14 +15,15 @@
         "@jupyterlab/codeeditor": "3.6.3",
         "@jupyterlab/codemirror": "3.6.3",
         "@jupyterlab/coreutils": "5.6.0",
         "@jupyterlab/docmanager": "3.6.3",
         "@jupyterlab/docprovider": "3.6.3",
         "@jupyterlab/docregistry": "3.6.3",
         "@jupyterlab/filebrowser": "3.6.3",
+        "@jupyterlab/mainmenu": "3.6.3",
         "@jupyterlab/nbformat": "3.6.3",
         "@jupyterlab/notebook": "3.6.3",
         "@jupyterlab/outputarea": "3.6.3",
         "@jupyterlab/rendermime": "3.6.3",
         "@jupyterlab/rendermime-interfaces": "3.6.3",
         "@jupyterlab/services": "6.6.3",
         "@jupyterlab/settingregistry": "3.6.3",
@@ -79,15 +80,15 @@
                 "jlpm clean:all"
             ]
         }
     },
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.c52cf3d95e66ca429f2e.js",
+            "load": "static/remoteEntry.4fde18a81e31cc9c2aa5.js",
             "style": "./style"
         },
         "discovery": {
             "server": {
                 "base": {
                     "name": "vdk_jupyterlab_extension"
                 },
@@ -152,9 +153,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.951673056"
+    "version": "0.1.959565555"
 }
```

### Comparing `vdk_jupyterlab_extension-0.1.951673056/vdk_jupyterlab_extension/labextension/schemas/vdk-jupyterlab-extension/package.json.orig` & `vdk_jupyterlab_extension-0.1.959565555/vdk_jupyterlab_extension/labextension/schemas/vdk-jupyterlab-extension/package.json.orig`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9765151515151516%*

 * *Differences: {"'dependencies'": "{'@jupyterlab/mainmenu': '3.6.3'}", "'version'": "'0.1.959565555'"}*

```diff
@@ -15,14 +15,15 @@
         "@jupyterlab/codeeditor": "3.6.3",
         "@jupyterlab/codemirror": "3.6.3",
         "@jupyterlab/coreutils": "5.6.0",
         "@jupyterlab/docmanager": "3.6.3",
         "@jupyterlab/docprovider": "3.6.3",
         "@jupyterlab/docregistry": "3.6.3",
         "@jupyterlab/filebrowser": "3.6.3",
+        "@jupyterlab/mainmenu": "3.6.3",
         "@jupyterlab/nbformat": "3.6.3",
         "@jupyterlab/notebook": "3.6.3",
         "@jupyterlab/outputarea": "3.6.3",
         "@jupyterlab/rendermime": "3.6.3",
         "@jupyterlab/rendermime-interfaces": "3.6.3",
         "@jupyterlab/services": "6.6.3",
         "@jupyterlab/settingregistry": "3.6.3",
@@ -147,9 +148,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.951673056"
+    "version": "0.1.959565555"
 }
```

### Comparing `vdk_jupyterlab_extension-0.1.951673056/vdk_jupyterlab_extension/labextension/schemas/vdk-jupyterlab-extension/plugin.json` & `vdk_jupyterlab_extension-0.1.959565555/vdk_jupyterlab_extension/labextension/schemas/vdk-jupyterlab-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.951673056/vdk_jupyterlab_extension/labextension/static/161.687b3e6d54b7501a02f7.js` & `vdk_jupyterlab_extension-0.1.959565555/vdk_jupyterlab_extension/labextension/static/242.9f4f2d980858aa93e6aa.js`

 * *Files 22% similar despite different names*

#### js-beautify {}

```diff
@@ -1,48 +1,48 @@
 "use strict";
 (self.webpackChunkvdk_jupyterlab_extension = self.webpackChunkvdk_jupyterlab_extension || []).push([
-    [161], {
-        161: (e, t, o) => {
-            o.r(t), o.d(t, {
-                default: () => z,
-                workingDirectory: () => G
+    [242], {
+        242: (e, t, n) => {
+            n.r(t), n.d(t, {
+                default: () => Z,
+                workingDirectory: () => X
             });
-            var n, a = o(38),
-                l = o(33),
-                r = o(271),
-                s = o.n(r);
+            var o, a = n(38),
+                l = n(33),
+                r = n(271),
+                s = n.n(r);
             ! function(e) {
                 e.NAME = "jobName", e.TEAM = "jobTeam", e.PATH = "jobPath", e.CLOUD = "cloud", e.LOCAL = "local", e.ARGUMENTS = "jobArguments", e.DEPLOYMENT_REASON = "deploymentReason"
-            }(n || (n = {}));
+            }(o || (o = {}));
             var i = new Map([]);
 
             function c() {
-                for (const e of Object.values(n)) i.set(e, "")
+                for (const e of Object.values(o)) i.set(e, "")
             }
 
             function u() {
                 return {
-                    jobName: i.get(n.NAME),
-                    jobTeam: i.get(n.TEAM),
-                    jobPath: i.get(n.PATH),
-                    cloud: i.get(n.CLOUD),
-                    local: i.get(n.LOCAL),
-                    jobArguments: i.get(n.ARGUMENTS),
-                    deploymentReason: i.get(n.DEPLOYMENT_REASON)
+                    jobName: i.get(o.NAME),
+                    jobTeam: i.get(o.TEAM),
+                    jobPath: i.get(o.PATH),
+                    cloud: i.get(o.CLOUD),
+                    local: i.get(o.LOCAL),
+                    jobArguments: i.get(o.ARGUMENTS),
+                    deploymentReason: i.get(o.DEPLOYMENT_REASON)
                 }
             }
             async function d(e) {
                 return !!i.get(e) || (await (0, l.showErrorMessage)("Encountered an error while trying to execute operation. Error:", "The " + e + " should be defined!", [l.Dialog.okButton()]), !1)
             }
             c();
-            const m = e => {
+            const h = e => {
                 const t = e.split(/(?=[/\\])/);
                 return t[t.length - 1]
             };
-            class h extends r.Component {
+            class m extends r.Component {
                 constructor(e) {
                     super(e), this.onInputChange = e => {
                         let t = e.currentTarget.value;
                         t || (t = this.props.value), i.set(this.props.option, t)
                     }
                 }
                 render() {
@@ -51,27 +51,27 @@
                     }, s().createElement("label", {
                         className: "jp-vdk-label",
                         htmlFor: this.props.option
                     }, this.props.label), s().createElement("input", {
                         type: "text",
                         id: this.props.option,
                         className: "jp-vdk-input",
-                        placeholder: m(this.props.value),
+                        placeholder: h(this.props.value),
                         onChange: this.onInputChange
                     })))
                 }
             }
-            var p = o(142),
-                g = o(820);
+            var p = n(142),
+                g = n(820);
             async function b(e = "", t = {}) {
-                const o = g.ServerConnection.makeSettings(),
-                    n = p.URLExt.join(o.baseUrl, "vdk-jupyterlab-extension", e);
+                const n = g.ServerConnection.makeSettings(),
+                    o = p.URLExt.join(n.baseUrl, "vdk-jupyterlab-extension", e);
                 let a;
                 try {
-                    a = await g.ServerConnection.makeRequest(n, t, o)
+                    a = await g.ServerConnection.makeRequest(o, t, n)
                 } catch (e) {
                     throw e
                 }
                 let l = await a.text();
                 if (l.length > 0) try {
                     l = JSON.parse(l)
                 } catch (e) {
@@ -79,16 +79,16 @@
                 }
                 if (!a.ok) throw new Error(a.statusText);
                 return l
             }
             const v = async e => {
                 await (0, l.showErrorMessage)("Encountered an error while trying to connect the server. Error:", e, [l.Dialog.okButton()])
             };
-            async function y() {
-                if (!await d(n.PATH)) return {
+            async function E() {
+                if (!await d(o.PATH)) return {
                     message: "",
                     status: !1
                 };
                 try {
                     const e = await b("run", {
                         body: JSON.stringify(u()),
                         method: "POST"
@@ -100,61 +100,63 @@
                 } catch (e) {
                     return v(e), {
                         message: "",
                         status: !1
                     }
                 }
             }
-            async function E(e) {
-                if (await d(n.NAME) && await d(n.TEAM)) try {
+            async function y(e) {
+                if (await d(o.NAME) && await d(o.TEAM)) try {
                     const t = await b(e, {
                         body: JSON.stringify(u()),
                         method: "POST"
                     });
                     t.error ? await (0, l.showErrorMessage)("Encountered an error while trying the " + e + " operation. Error:", t.message, [l.Dialog.okButton()]) : alert(t.message)
                 } catch (e) {
                     v(e)
                 }
             }
-            class f {
+            class w {
                 constructor(e) {
                     this.exception_message = "", this.what_happened = "", this.why_it_happened = "", this.consequences = "", this.countermeasures = "", this.__parse_message(e)
                 }
                 __parse_message(e) {
                     const t = ["exception_message", "what_happened", "why_it_happened", "consequences", "countermeasures"],
-                        o = ["ERROR : ", "WHAT HAPPENED :", "WHY IT HAPPENED :", "CONSEQUENCES :", "COUNTERMEASURES :"],
-                        n = e.split("\n");
+                        n = ["ERROR : ", "WHAT HAPPENED :", "WHY IT HAPPENED :", "CONSEQUENCES :", "COUNTERMEASURES :"],
+                        o = e.split("\n");
                     let a = 0;
-                    for (let l = 0; l < n.length; l++) {
-                        const r = n[l].indexOf(o[a]);
+                    for (let l = 0; l < o.length; l++) {
+                        const r = o[l].indexOf(n[a]);
                         if (-1 !== r) {
-                            if (this[t[a]] = o[a] + n[l].substring(r + o[a].length), a++, a === t.length) break
+                            if (this[t[a]] = n[a] + o[l].substring(r + n[a].length), a++, a === t.length) break
                         } else this.exception_message = e
                     }
                 }
             }
-            const w = "Convert Job To Notebook",
+            const f = "Convert Job To Notebook",
                 k = "Run Job",
-                j = "Create Deployment";
+                j = "Create Deployment",
+                T = "Status",
+                N = "jp-vdk:check-status-button";
             class C extends r.Component {
                 constructor(e) {
                     super(e), this._onArgsChange = e => {
                         let t = e.currentTarget.value;
-                        t && this._isJSON(t) && i.set(n.ARGUMENTS, t)
+                        t && this._isJSON(t) && i.set(o.ARGUMENTS, t)
                     }, this._isJSON = e => {
                         try {
                             return JSON.parse(e), !0
                         } catch (e) {
                             return !1
                         }
                     }
                 }
                 render() {
-                    return s().createElement(s().Fragment, null, s().createElement(h, {
-                        option: n.PATH,
+                    return s().createElement(s().Fragment, null, s().createElement(m, {
+                        option: o.PATH,
                         value: this.props.jobPath,
                         label: "Path to job directory:"
                     }), s().createElement("div", {
                         className: "jp-vdk-input-wrapper"
                     }, s().createElement("label", {
                         className: "jp-vdk-label",
                         htmlFor: "arguments"
@@ -166,84 +168,85 @@
                         onChange: this._onArgsChange
                     })), s().createElement("ul", {
                         id: "argumentsUl",
                         className: "hidden"
                     }))
                 }
             }
-            async function T(e) {
+            async function A(e, t) {
                 if ((await (0, l.showDialog)({
                         title: k,
                         body: s().createElement(C, {
-                            jobPath: i.get(n.PATH)
+                            jobPath: i.get(o.PATH)
                         }),
                         buttons: [l.Dialog.okButton(), l.Dialog.cancelButton()]
                     })).button.accept) {
+                    null == t || t.show("Run", i.get(o.PATH));
                     let {
-                        message: t,
-                        status: o
-                    } = await y();
-                    if (o)(0, l.showDialog)({
+                        message: n,
+                        status: a
+                    } = await E();
+                    if (a)(0, l.showDialog)({
                         title: k,
                         body: s().createElement("div", {
                             className: "vdk-run-dialog-message-container"
                         }, s().createElement("p", {
                             className: "vdk-run-dialog-message"
                         }, "The job was executed successfully!")),
                         buttons: [l.Dialog.okButton()]
                     });
                     else {
-                        t = "ERROR : " + t;
-                        const o = new f(t);
-                        e && await _(o, e) || (0, l.showDialog)({
+                        n = "ERROR : " + n;
+                        const t = new w(n);
+                        e && await x(t, e) || (0, l.showDialog)({
                             title: k,
                             body: s().createElement("div", {
                                 className: "vdk-run-error-message "
-                            }, s().createElement("p", null, o.exception_message), s().createElement("p", null, o.what_happened), s().createElement("p", null, o.why_it_happened), s().createElement("p", null, o.consequences), s().createElement("p", null, o.countermeasures)),
+                            }, s().createElement("p", null, t.exception_message), s().createElement("p", null, t.what_happened), s().createElement("p", null, t.why_it_happened), s().createElement("p", null, t.consequences), s().createElement("p", null, t.countermeasures)),
                             buttons: [l.Dialog.okButton()]
                         })
                     }
                 }
             }
-            const A = e => {
+            const D = e => {
                     const t = e.getElementsByClassName("jp-Cell-inputWrapper");
                     for (let e = 0; e < t.length; e++) {
-                        const o = t[e].getElementsByClassName("jp-Cell-inputArea");
-                        if (o.length > 0) {
-                            const e = o[0].getElementsByClassName("jp-InputArea-prompt");
+                        const n = t[e].getElementsByClassName("jp-Cell-inputArea");
+                        if (n.length > 0) {
+                            const e = n[0].getElementsByClassName("jp-InputArea-prompt");
                             if (e.length > 0) return e[0]
                         }
                     }
                 },
-                N = e => {
-                    const t = A(e);
+                P = e => {
+                    const t = D(e);
                     null == t || t.classList.add("jp-vdk-failing-cell-prompt"), e.scrollIntoView(), e.classList.add("jp-vdk-failing-cell"), Array.from(document.getElementsByClassName("jp-vdk-failing-cell-num")).forEach((e => {
                         e.classList.remove("jp-vdk-failing-cell-num"), e.classList.add("jp-vdk-cell-num")
                     }))
                 },
-                D = e => {
+                _ = e => {
                     e.classList.remove("jp-vdk-failing-cell");
-                    const t = A(e);
+                    const t = D(e);
                     null == t || t.classList.remove("jp-vdk-failing-cell-prompt")
                 },
-                _ = async (e, t) => {
-                    const o = (e => {
+                x = async (e, t) => {
+                    const n = (e => {
                         const t = e.match(/cell_id:([0-9a-fA-F-]+)/);
                         return t ? t[1] : ""
                     })(e.what_happened);
-                    if (o) {
+                    if (n) {
                         const {
                             path: a,
                             cellIndex: r
                         } = await async function(e) {
                             const t = {
                                 cellId: e,
-                                jobPath: i.get(n.PATH)
+                                jobPath: i.get(o.PATH)
                             };
-                            if (!await d(n.PATH)) return {
+                            if (!await d(o.PATH)) return {
                                 path: "",
                                 cellIndex: ""
                             };
                             try {
                                 const e = await b("notebook", {
                                     body: JSON.stringify(t),
                                     method: "POST"
@@ -254,103 +257,104 @@
                                 }
                             } catch (e) {
                                 return {
                                     path: "",
                                     cellIndex: ""
                                 }
                             }
-                        }(o);
+                        }(n);
                         if (a) {
-                            const o = async () => {
+                            const n = async () => {
                                 const e = t.openOrReveal(a);
                                 if (e) {
                                     await e.revealed;
                                     const t = Array.from(e.node.children);
                                     t && t.forEach((async e => {
-                                        e.classList.contains("jp-Notebook") && (async (e, t, o) => {
-                                            const n = e.children;
-                                            if (t > n.length)(0, l.showDialog)({
+                                        e.classList.contains("jp-Notebook") && (async (e, t, n) => {
+                                            const o = e.children;
+                                            if (t > o.length)(0, l.showDialog)({
                                                 title: "Run Failed",
-                                                body: s().createElement("div", null, s().createElement("p", null, "Sorry, something went wrong while trying to find the failing cell!"), s().createElement("p", null, "Please, check the ", o, " once more and try to run the job while the notebook is active!")),
+                                                body: s().createElement("div", null, s().createElement("p", null, "Sorry, something went wrong while trying to find the failing cell!"), s().createElement("p", null, "Please, check the ", n, " once more and try to run the job while the notebook is active!")),
                                                 buttons: [l.Dialog.cancelButton()]
                                             });
                                             else
-                                                for (let e = 0; e < n.length; e++) e === t ? N(n[e]) : D(n[e])
+                                                for (let e = 0; e < o.length; e++) e === t ? P(o[e]) : _(o[e])
                                         })(e, Number(r), a)
                                     }))
                                 }
                             };
                             return (await (0, l.showDialog)({
                                 title: k,
                                 body: s().createElement("div", {
                                     className: "vdk-run-error-message "
                                 }, s().createElement("p", null, e.exception_message), s().createElement("p", null, e.what_happened), s().createElement("p", null, e.why_it_happened), s().createElement("p", null, e.consequences), s().createElement("p", null, e.countermeasures)),
                                 buttons: [l.Dialog.okButton({
                                     label: "See failing cell"
                                 }), l.Dialog.cancelButton()]
-                            })).button.accept && o(), !0
+                            })).button.accept && await n(), !0
                         }
                     }
                     return !1
                 };
-            class P extends r.Component {
+            class O extends r.Component {
                 constructor(e) {
                     super(e)
                 }
                 render() {
-                    return s().createElement(s().Fragment, null, s().createElement(h, {
-                        option: n.NAME,
+                    return s().createElement(s().Fragment, null, s().createElement(m, {
+                        option: o.NAME,
                         value: this.props.jobName,
                         label: "Job Name:"
-                    }), s().createElement(h, {
-                        option: n.TEAM,
+                    }), s().createElement(m, {
+                        option: o.TEAM,
                         value: this.props.jobTeam,
                         label: "Job Team:"
-                    }), s().createElement(h, {
-                        option: n.PATH,
+                    }), s().createElement(m, {
+                        option: o.PATH,
                         value: this.props.jobPath,
                         label: "Path to job directory:"
-                    }), s().createElement(h, {
-                        option: n.DEPLOYMENT_REASON,
+                    }), s().createElement(m, {
+                        option: o.DEPLOYMENT_REASON,
                         value: "reason",
                         label: "Deployment reason:"
                     }))
                 }
             }
-            async function x() {
-                const e = await (0, l.showDialog)({
+            async function L(e) {
+                const t = await (0, l.showDialog)({
                     title: j,
-                    body: s().createElement(P, {
-                        jobName: i.get(n.NAME),
-                        jobPath: i.get(n.PATH),
-                        jobTeam: i.get(n.TEAM)
+                    body: s().createElement(O, {
+                        jobName: i.get(o.NAME),
+                        jobPath: i.get(o.PATH),
+                        jobTeam: i.get(o.TEAM)
                     }),
                     buttons: [l.Dialog.okButton(), l.Dialog.cancelButton()]
                 });
-                if (!e.value && e.button.accept) try {
+                if (!t.value && t.button.accept) try {
                     if ((await (0, l.showDialog)({
                             title: j,
                             body: "The job will be executed once before deployment.",
                             buttons: [l.Dialog.cancelButton({
                                 label: "Cancel"
                             }), l.Dialog.okButton({
                                 label: "Continue"
                             })]
                         })).button.accept) {
+                        null == e || e.show("Deploy", i.get(o.PATH));
                         const {
-                            message: e,
-                            status: t
-                        } = await y();
-                        t ? await d(n.DEPLOYMENT_REASON) && await E("deploy") : (0, l.showErrorMessage)("Encоuntered an error while running the job!", e, [l.Dialog.okButton()])
+                            message: t,
+                            status: n
+                        } = await E();
+                        n ? await d(o.DEPLOYMENT_REASON) && await y("deploy") : await (0, l.showErrorMessage)("Encоuntered an error while running the job!", t, [l.Dialog.okButton()])
                     }
                 } catch (e) {
                     await (0, l.showErrorMessage)("Encountered an error when deploying the job. Error:", e, [l.Dialog.okButton()])
                 }
             }
-            class O extends r.Component {
+            class S extends r.Component {
                 constructor(e) {
                     super(e)
                 }
                 render() {
                     return s().createElement(s().Fragment, null, s().createElement("div", {
                         className: "jp-vdk-checkbox-wrappers"
                     }, s().createElement("div", null, s().createElement("input", {
@@ -367,24 +371,24 @@
                         name: "Cloud",
                         id: "Cloud",
                         className: "jp-vdk-checkbox",
                         onClick: this._onCloudClick()
                     }), s().createElement("label", {
                         className: "checkboxLabel",
                         htmlFor: "Cloud"
-                    }, "Cloud"))), s().createElement(h, {
-                        option: n.NAME,
+                    }, "Cloud"))), s().createElement(m, {
+                        option: o.NAME,
                         value: this.props.jobName,
                         label: "Job Name:"
-                    }), s().createElement(h, {
-                        option: n.TEAM,
+                    }), s().createElement(m, {
+                        option: o.TEAM,
                         value: this.props.jobTeam,
                         label: "Job Team:"
-                    }), s().createElement(h, {
-                        option: n.PATH,
+                    }), s().createElement(m, {
+                        option: o.PATH,
                         value: this.props.jobPath,
                         label: "Path to job directory:"
                     }))
                 }
                 _onLocalClick() {
                     return e => {
                         this.setJobFlags("Local")
@@ -392,88 +396,89 @@
                 }
                 _onCloudClick() {
                     return e => {
                         this.setJobFlags("Cloud")
                     }
                 }
                 setJobFlags(e) {
-                    let t = document.getElementById(e);
-                    (null == t ? void 0 : t.classList.contains("checked")) ? (t.classList.remove("checked"), "Cloud" === e ? i.set(n.CLOUD, "") : i.set(n.LOCAL, "")) : (null == t || t.classList.add("checked"), "Cloud" === e ? i.set(n.CLOUD, "1") : i.set(n.LOCAL, "1"))
+                    const t = document.getElementById(e);
+                    (null == t ? void 0 : t.classList.contains("checked")) ? (t.classList.remove("checked"), "Cloud" === e ? i.set(o.CLOUD, "") : i.set(o.LOCAL, "")) : (null == t || t.classList.add("checked"), "Cloud" === e ? i.set(o.CLOUD, "1") : i.set(o.LOCAL, "1"))
                 }
             }
-            async function L() {
+            async function M(e) {
                 (await (0, l.showDialog)({
                     title: "Create Job",
-                    body: s().createElement(O, {
-                        jobPath: i.get(n.PATH),
-                        jobName: i.get(n.NAME),
-                        jobTeam: i.get(n.TEAM)
+                    body: s().createElement(S, {
+                        jobPath: i.get(o.PATH),
+                        jobName: i.get(o.NAME),
+                        jobTeam: i.get(o.TEAM)
                     }),
                     buttons: [l.Dialog.okButton(), l.Dialog.cancelButton()]
-                })).button.accept && await E("create")
+                })).button.accept && (null == e || e.show("Create", i.get(o.PATH)), await y("create"))
             }
-            class S extends r.Component {
+            class B extends r.Component {
                 constructor(e) {
                     super(e)
                 }
                 render() {
-                    return s().createElement(s().Fragment, null, s().createElement(h, {
-                        option: n.NAME,
+                    return s().createElement(s().Fragment, null, s().createElement(m, {
+                        option: o.NAME,
                         value: "default-name",
                         label: "Job Name:"
-                    }), s().createElement(h, {
-                        option: n.TEAM,
+                    }), s().createElement(m, {
+                        option: o.TEAM,
                         value: "default-team",
                         label: "Job Team:"
-                    }), s().createElement(h, {
-                        option: n.PATH,
+                    }), s().createElement(m, {
+                        option: o.PATH,
                         value: this.props.jobPath,
                         label: "Path to job directory:"
                     }))
                 }
             }
-            async function M() {
+            async function H(e) {
                 (await (0, l.showDialog)({
                     title: "Download Job",
-                    body: s().createElement(S, {
-                        jobPath: i.get(n.PATH)
+                    body: s().createElement(B, {
+                        jobPath: i.get(o.PATH)
                     }),
                     buttons: [l.Dialog.okButton(), l.Dialog.cancelButton()]
-                })).button.accept && await E("download")
+                })).button.accept && (null == e || e.show("Download", i.get(o.PATH)), await y("download"))
             }
-            var B;
-            class J extends r.Component {
+            var J;
+            class I extends r.Component {
                 constructor(e) {
                     super(e)
                 }
                 render() {
-                    return s().createElement(s().Fragment, null, s().createElement(h, {
-                        option: n.PATH,
+                    return s().createElement(s().Fragment, null, s().createElement(m, {
+                        option: o.PATH,
                         value: this.props.jobPath,
                         label: "Path to job directory:"
                     }))
                 }
             }
-            async function H(e, t, o) {
+            async function R(e, t, n, a) {
                 if ((await (0, l.showDialog)({
-                        title: w,
-                        body: s().createElement(J, {
-                            jobPath: i.get(n.PATH)
+                        title: f,
+                        body: s().createElement(I, {
+                            jobPath: i.get(o.PATH)
                         }),
                         buttons: [l.Dialog.okButton(), l.Dialog.cancelButton()]
                     })).button.accept && (await (0, l.showDialog)({
-                        title: w,
-                        body: s().createElement("p", null, "Are you sure you want to convert the Data Job with path:", " ", s().createElement("i", null, i.get(n.PATH)), " to notebook?"),
+                        title: f,
+                        body: s().createElement("p", null, "Are you sure you want to convert the Data Job with path:", " ", s().createElement("i", null, i.get(o.PATH)), " to notebook?"),
                         buttons: [l.Dialog.okButton(), l.Dialog.cancelButton()]
                     })).button.accept) {
+                    null == a || a.show("Convert", i.get(o.PATH));
                     let {
-                        message: a,
-                        status: r
+                        message: r,
+                        status: c
                     } = await async function() {
-                        if (!await d(n.PATH)) return {
+                        if (!await d(o.PATH)) return {
                             message: "The job path is not defined. Please define it before attempting to convert the job to a notebook.",
                             status: !1
                         };
                         try {
                             const e = await b("convertJobToNotebook", {
                                 body: JSON.stringify(u()),
                                 method: "POST"
@@ -485,204 +490,267 @@
                         } catch (e) {
                             return v(e), {
                                 message: "",
                                 status: !1
                             }
                         }
                     }();
-                    if (r) {
-                        const r = JSON.parse(a);
-                        B = R(r.code_structure, r.removed_files), await I(e, t, o), await (0, l.showDialog)({
-                            title: w,
+                    if (c) {
+                        const a = JSON.parse(r);
+                        J = V(a.code_structure, a.removed_files), await K(e, t, n), await (0, l.showDialog)({
+                            title: f,
                             body: s().createElement("div", {
                                 className: "vdk-convert-to-notebook-dialog-message-container"
                             }, s().createElement("p", {
                                 className: "vdk-convert-to-notebook-dialog-message"
-                            }, "The Data Job with path ", s().createElement("i", null, i.get(n.PATH)), " was converted to notebook successfully!")),
+                            }, "The Data Job with path ", s().createElement("i", null, i.get(o.PATH)), " was converted to notebook successfully!")),
                             buttons: [l.Dialog.okButton()]
                         })
-                    } else if (a) {
-                        a = "ERROR : " + a;
-                        const e = new f(a);
+                    } else if (r) {
+                        r = "ERROR : " + r;
+                        const e = new w(r);
                         await (0, l.showDialog)({
-                            title: w,
+                            title: f,
                             body: s().createElement("div", {
                                 className: "vdk-convert-to-notebook-error-message "
                             }, s().createElement("p", null, e.exception_message), s().createElement("p", null, e.what_happened), s().createElement("p", null, e.why_it_happened), s().createElement("p", null, e.consequences), s().createElement("p", null, e.countermeasures)),
                             buttons: [l.Dialog.okButton()]
                         })
                     }
                 }
             }
-            const I = async (e, t, o) => {
+            const K = async (e, t, n) => {
                 try {
-                    const o = await async function() {
+                    const n = await async function() {
                         return await b("serverPath", {
                             method: "GET"
                         }) || (await (0, l.showErrorMessage)("Encountered an error while trying to connect the server. Error:       the server's location cannot be identified!", [l.Dialog.okButton()]), "")
                     }();
-                    i.set(n.NAME, i.get(n.PATH).split(/[\\/]/).pop() || ""), await t.model.cd(i.get(n.PATH).substring(o.length)), e.execute("notebook:create-new")
+                    i.set(o.NAME, i.get(o.PATH).split(/[\\/]/).pop() || ""), await t.model.cd(i.get(o.PATH).substring(n.length)), e.execute("notebook:create-new")
                 } catch (e) {
                     await (0, l.showErrorMessage)("Something went wrong while trying to create the new transformed notebook. Error:", e, [l.Dialog.okButton()])
                 }
-            }, R = (e, t) => {
-                const o = [];
-                for (let n = 0; n < e.length; n++) o.push({
-                    source: "#### " + t[n],
+            }, V = (e, t) => {
+                const n = [];
+                for (let o = 0; o < e.length; o++) n.push({
+                    source: "#### " + t[o],
                     type: "markdown"
-                }), o.push({
-                    source: e[n],
+                }), n.push({
+                    source: e[o],
                     type: "code"
-                }), e[n].includes("def run(job_input: IJobInput)") && o.push({
+                }), e[o].includes("def run(job_input: IJobInput)") && n.push({
                     source: "run(job_input)",
                     type: "code"
                 });
-                return o
+                return n
             };
-            var V = "";
+            var F = "";
 
-            function F(e, t, o, a, r, s, d, m) {
+            function W(e, t, n, a, r, s, d, h, m) {
                 e.addCommand(t, {
-                    label: o,
+                    label: n,
                     caption: a,
                     execute: async () => {
                         try {
-                            V ? (0, l.showErrorMessage)("Another VDK operation is currently running!", "Please wait until the operation ends!", [l.Dialog.okButton()]) : (V = t, i.set(n.PATH, G), await async function() {
+                            F ? await (0, l.showErrorMessage)("Another VDK operation is currently running!", "Please wait until the operation ends!", [l.Dialog.okButton()]) : (F = t, i.set(o.PATH, X), await async function() {
                                 try {
                                     const e = await b("job", {
                                         body: JSON.stringify(JSON.stringify(u())),
                                         method: "POST"
                                     });
-                                    e && (i.set(n.NAME, e[n.NAME]), i.set(n.TEAM, e[n.TEAM]), i.set(n.PATH, e[n.PATH]))
+                                    e && (i.set(o.NAME, e[o.NAME]), i.set(o.TEAM, e[o.TEAM]), i.set(o.PATH, e[o.PATH]))
                                 } catch (e) {
                                     v(e)
                                 }
-                            }(), "Convert Job To Notebook" == o ? await r(e, d, m) : s ? await r(s) : await r(), c(), V = "")
+                            }(), "Convert Job To Notebook" === n ? await r(e, h, m, s) : d ? await r(d, s) : await r(s), s.hide(), c(), F = "")
                         } catch (e) {
                             await (0, l.showErrorMessage)("Encountered an error when trying to open the dialog. Error:", e, [l.Dialog.okButton()])
                         }
                     }
                 })
             }
-            var K = o(280),
-                W = o(123);
-            const U = (e, t) => {
-                    const o = document.createElement("div");
-                    o.innerText = String(e), t.classList.contains("jp-vdk-failing-cell") ? o.classList.add("jp-vdk-failing-cell-num") : o.classList.add("jp-vdk-cell-num"), t.appendChild(o)
+            var q = n(280),
+                U = n(123);
+            const Y = (e, t) => {
+                    const n = document.createElement("div");
+                    n.innerText = String(e), t.classList.contains("jp-vdk-failing-cell") ? n.classList.add("jp-vdk-failing-cell-num") : n.classList.add("jp-vdk-cell-num"), t.appendChild(n)
                 },
-                q = e => {
+                G = e => {
                     const t = document.createElement("img");
                     t.setAttribute("src", "https://raw.githubusercontent.com/vmware/versatile-data-kit/dc15f7489f763a0e0e29370b2e06a714448fc234/support/images/versatile-data-kit-logo.svg"), t.setAttribute("width", "20"), t.setAttribute("height", "20"), t.classList.add("jp-vdk-logo"), e.appendChild(t)
                 };
-            var Y = o(986);
-            let G = "";
-            const z = {
+            var z = n(986),
+                Q = n(502);
+            class $ {
+                constructor(e) {
+                    this.buttonElement = document.createElement("button"), this.buttonElement.id = "jp-vdk-check-status-button", this.buttonElement.className = "jp-vdk-check-status-button";
+                    const t = document.createElement("div");
+                    t.className = "jp-vdk-status-button-content", G(t);
+                    const n = document.createElement("span");
+                    n.innerHTML = "00:00:00", t.appendChild(n), this.buttonElement.appendChild(t), this.buttonElement.onclick = () => {
+                        e.execute(N, {
+                            operation: this.operation,
+                            path: this.jobPath
+                        })
+                    }, this.buttonElement.title = "VDK operation is in progress. Click here for more info.", this.buttonElement.style.display = "none", this.counter = 0
+                }
+                get element() {
+                    return this.buttonElement
+                }
+                show(e, t) {
+                    this.operation = e, this.jobPath = t, this.buttonElement.style.display = "", this.startTimer()
+                }
+                hide() {
+                    this.buttonElement.style.display = "none", this.stopTimer()
+                }
+                startTimer() {
+                    this.counter = 0, this.timerId = window.setInterval((() => {
+                        this.counter++;
+                        const e = this.buttonElement.querySelector("span");
+                        var t;
+                        e && (e.innerHTML = `${t=this.counter,new Date(1e3*t).toISOString().substr(11,8)}`)
+                    }), 1e3)
+                }
+                stopTimer() {
+                    this.timerId && (clearInterval(this.timerId), this.timerId = void 0);
+                    const e = this.buttonElement.querySelector("span");
+                    e && (e.innerHTML = "00:00:00")
+                }
+            }
+            let X = "";
+            const Z = {
                     id: "vdk-jupyterlab-extension:plugin",
                     autoStart: !0,
-                    optional: [a.ISettingRegistry, K.IFileBrowserFactory, W.INotebookTracker, l.IThemeManager, Y.IDocumentManager],
-                    activate: async (e, t, o, a, l, r) => {
+                    optional: [a.ISettingRegistry, q.IFileBrowserFactory, U.INotebookTracker, l.IThemeManager, z.IDocumentManager],
+                    activate: async (e, t, n, a, r, c) => {
                         const {
-                            commands: s
+                            commands: u
                         } = e;
                         a.activeCellChanged.connect(((e, t) => {
-                            "jp-vdk:menu-convert-job-to-notebook" !== V ? function(e) {
-                                var t, o, n, a;
-                                const l = e.currentWidget;
-                                if (l) {
-                                    const r = null === (o = null === (t = l.content.model) || void 0 === t ? void 0 : t.contentFactory) || void 0 === o ? void 0 : o.createCodeCell({
-                                            cell: {
-                                                cell_type: "code",
-                                                source: ['"""\n', "vdk.plugin.ipython extension introduces a magic command for Jupyter.\n", "The command enables the user to load VDK for the current notebook.\n", "VDK provides the job_input API, which has methods for:\n", "    * executing queries to an OLAP database;\n", "    * ingesting data into a database;\n", "    * processing data into a database.\n", "See the IJobInput documentation for more details.\n", "https://github.com/vmware/versatile-data-kit/blob/main/projects/vdk-core/src/vdk/api/job_input.py\n", "Please refrain from tagging this cell with VDK as it is not an actual part of the data job\n", "and is only used for development purposes.\n", '"""\n', "%reload_ext vdk.plugin.ipython\n", "%reload_VDK\n", "job_input = VDK.get_initialized_job_input()"],
-                                                metadata: {}
-                                            }
-                                        }),
-                                        s = null === (a = null === (n = e.currentWidget) || void 0 === n ? void 0 : n.content.model) || void 0 === a ? void 0 : a.cells,
-                                        i = null == s ? void 0 : s.get(0).value.text;
-                                    s && r && s.length <= 1 && "" == i && (s.insert(0, r), s.remove(1))
-                                }
-                            }(a) : (async e => {
-                                var t, o;
-                                const a = e.currentWidget;
-                                if (a) {
-                                    const l = null === (o = null === (t = e.currentWidget) || void 0 === t ? void 0 : t.content.model) || void 0 === o ? void 0 : o.cells,
-                                        r = null == l ? void 0 : l.get(0).value.text;
-                                    if (l && l.length <= 1 && "" == r) {
-                                        l.remove(1);
-                                        const e = e => {
-                                                var t, o;
-                                                const n = null === (o = null === (t = a.content.model) || void 0 === t ? void 0 : t.contentFactory) || void 0 === o ? void 0 : o.createMarkdownCell({
-                                                    cell: {
-                                                        cell_type: "markdown",
-                                                        source: e,
-                                                        metadata: {}
-                                                    }
-                                                });
-                                                n && l.push(n)
-                                            },
-                                            t = (e, t) => {
-                                                var o, n;
-                                                const r = null === (n = null === (o = a.content.model) || void 0 === o ? void 0 : o.contentFactory) || void 0 === n ? void 0 : n.createCodeCell({
-                                                    cell: {
-                                                        cell_type: "code",
-                                                        source: e,
-                                                        metadata: t
-                                                    }
-                                                });
-                                                r && l.push(r)
-                                            };
-                                        e(["# " + i.get(n.NAME)]), e(["### Please go through this guide before continuing with the data job run and development."]), e(["#### Introduction and Preparations\n", "*  *This is a notebook transformed from a directory style data job located in " + i.get(n.PATH) + ".*\n", "*  *If you are not familiar with notebook data jobs make sure to check the **Getting Started**(TODO: add link) page.*\n", "*  *You can find the **original job** at " + i.get(n.PATH).split(/[/\\]/).slice(0, -1).join("/") + ".*"]), e(["#### Execution Order and Identifying Cells\n", "*  *The below cells are automatically generated corresponding to a step(.sql or .py file with VDK run function) \n", "    in your original job.* \n", "*  *You will notice that some cells are coloured and include the VDK logo and a numbering. \n", '    These are the "vdk" tagged cells.\n', "    Only these cells are executed during VDK run and all the others are ignored(for example the current cell).*\n", "*  *Code cells in the notebook will be executed according to the numbering when running the notebook data job with VDK.\n", "    This means that the steps in the job are organized from the top to the bottom, starting with the first step.*\n", '*  *When you see a title saying **"Step generated from: sample.py"** before some blocks of code, \n', '    it means that the code below that title was created from the "sample.py" file.*\n', '*  *Similarly, if you come across code cells that have the format **"job_input.execute_query(query_string)"** ,\n', '    it means that those cells contain code generated from ".sql" files.*\n', '*  *On the other hand, code cells originating from ".py" files remain unchanged.\n', '    However, an additional cell is included that calls the "run" function using the command **"run(job_input)"** . \n', '    This cell executes the "run" function from the code generated from the ".py" file.*\n', '*  *You can delete the cells that are not tagged with "vdk" \n', "    as they are not essential to the data job's execution.\n", "    However, removing tagged cells will result in a different data job run.* "]), e(["#### Tips: \n", "* *Before running the job, it is recommended to review the cells\n", "    to ensure a clear understanding of the data job run.  \n", "    This will help to ensure the desired outcome.* "]), t(['"""\n', "vdk.plugin.ipython extension introduces a magic command for Jupyter.\n", "The command enables the user to load VDK for the current notebook.\n", "VDK provides the job_input API, which has methods for:\n", "    * executing queries to an OLAP database;\n", "    * ingesting data into a database;\n", "    * processing data into a database.\n", "See the IJobInput documentation for more details.\n", "https://github.com/vmware/versatile-data-kit/blob/main/projects/vdk-core/src/vdk/api/job_input.py\n", "Please refrain from tagging this cell with VDK as it is not an actual part of the data job\n", "and is only used for development purposes.\n", '"""\n', "%reload_ext vdk.plugin.ipython\n", "%reload_VDK\n", "job_input = VDK.get_initialized_job_input()"], {});
-                                        for (const o of B) "markdown" === o.type ? e([o.source]) : "code" === o.type && t([o.source], {
-                                            tags: ["vdk"]
-                                        });
-                                        B = []
+                                "jp-vdk:menu-convert-job-to-notebook" !== F ? function(e) {
+                                    var t, n, o, a;
+                                    const l = e.currentWidget;
+                                    if (l) {
+                                        const r = null === (n = null === (t = l.content.model) || void 0 === t ? void 0 : t.contentFactory) || void 0 === n ? void 0 : n.createCodeCell({
+                                                cell: {
+                                                    cell_type: "code",
+                                                    source: ['"""\n', "vdk.plugin.ipython extension introduces a magic command for Jupyter.\n", "The command enables the user to load VDK for the current notebook.\n", "VDK provides the job_input API, which has methods for:\n", "    * executing queries to an OLAP database;\n", "    * ingesting data into a database;\n", "    * processing data into a database.\n", "See the IJobInput documentation for more details.\n", "https://github.com/vmware/versatile-data-kit/blob/main/projects/vdk-core/src/vdk/api/job_input.py\n", "Please refrain from tagging this cell with VDK as it is not an actual part of the data job\n", "and is only used for development purposes.\n", '"""\n', "%reload_ext vdk.plugin.ipython\n", "%reload_VDK\n", "job_input = VDK.get_initialized_job_input()"],
+                                                    metadata: {}
+                                                }
+                                            }),
+                                            s = null === (a = null === (o = e.currentWidget) || void 0 === o ? void 0 : o.content.model) || void 0 === a ? void 0 : a.cells,
+                                            i = null == s ? void 0 : s.get(0).value.text;
+                                        s && r && s.length <= 1 && "" == i && (s.insert(0, r), s.remove(1))
                                     }
-                                }
-                            })(a)
-                        }));
-                        const c = o.defaultBrowser;
-                        ! function(e, t, o, n) {
-                            F(e, "jp-vdk:menu-run", "Run", "Execute VDK Run Command", T, t), F(e, "jp-vdk:menu-create", "Create", "Execute VDK Create Command", L), F(e, "jp-vdk:menu-download", "Download", "Execute VDK Download Command", M), F(e, "jp-vdk:menu-convert-job-to-notebook", "Convert Job To Notebook", "Convert Data Job To Jupyter Notebook", H, void 0, o, n), F(e, "jp-vdk:menu-create-deployment", "Deploy", "Create deployment of a VDK job", x)
-                        }(s, r, c, a), c.model.pathChanged.connect(Q), ((e, t) => {
-                            const o = async () => {
-                                if (e.currentWidget && e.currentWidget.model && 0 !== e.currentWidget.model.cells.length) {
-                                    let o = [],
-                                        n = 0;
-                                    for (; e.currentWidget && e.currentWidget.model && e.currentWidget.model.cells.get(n);) {
-                                        const t = e.currentWidget.model.cells.get(n).metadata.get("tags");
-                                        t && t.includes("vdk") && o.push(n), n++
+                                }(a) : (async e => {
+                                    var t, n;
+                                    const a = e.currentWidget;
+                                    if (a) {
+                                        const l = null === (n = null === (t = e.currentWidget) || void 0 === t ? void 0 : t.content.model) || void 0 === n ? void 0 : n.cells,
+                                            r = null == l ? void 0 : l.get(0).value.text;
+                                        if (l && l.length <= 1 && "" == r) {
+                                            l.remove(1);
+                                            const e = e => {
+                                                    var t, n;
+                                                    const o = null === (n = null === (t = a.content.model) || void 0 === t ? void 0 : t.contentFactory) || void 0 === n ? void 0 : n.createMarkdownCell({
+                                                        cell: {
+                                                            cell_type: "markdown",
+                                                            source: e,
+                                                            metadata: {}
+                                                        }
+                                                    });
+                                                    o && l.push(o)
+                                                },
+                                                t = (e, t) => {
+                                                    var n, o;
+                                                    const r = null === (o = null === (n = a.content.model) || void 0 === n ? void 0 : n.contentFactory) || void 0 === o ? void 0 : o.createCodeCell({
+                                                        cell: {
+                                                            cell_type: "code",
+                                                            source: e,
+                                                            metadata: t
+                                                        }
+                                                    });
+                                                    r && l.push(r)
+                                                };
+                                            e(["# " + i.get(o.NAME)]), e(["### Please go through this guide before continuing with the data job run and development."]), e(["#### Introduction and Preparations\n", "*  *This is a notebook transformed from a directory style data job located in " + i.get(o.PATH) + ".*\n", "*  *If you are not familiar with notebook data jobs make sure to check the **Getting Started**(TODO: add link) page.*\n", "*  *You can find the **original job** at " + i.get(o.PATH).split(/[/\\]/).slice(0, -1).join("/") + ".*"]), e(["#### Execution Order and Identifying Cells\n", "*  *The below cells are automatically generated corresponding to a step(.sql or .py file with VDK run function) \n", "    in your original job.* \n", "*  *You will notice that some cells are coloured and include the VDK logo and a numbering. \n", '    These are the "vdk" tagged cells.\n', "    Only these cells are executed during VDK run and all the others are ignored(for example the current cell).*\n", "*  *Code cells in the notebook will be executed according to the numbering when running the notebook data job with VDK.\n", "    This means that the steps in the job are organized from the top to the bottom, starting with the first step.*\n", '*  *When you see a title saying **"Step generated from: sample.py"** before some blocks of code, \n', '    it means that the code below that title was created from the "sample.py" file.*\n', '*  *Similarly, if you come across code cells that have the format **"job_input.execute_query(query_string)"** ,\n', '    it means that those cells contain code generated from ".sql" files.*\n', '*  *On the other hand, code cells originating from ".py" files remain unchanged.\n', '    However, an additional cell is included that calls the "run" function using the command **"run(job_input)"** . \n', '    This cell executes the "run" function from the code generated from the ".py" file.*\n', '*  *You can delete the cells that are not tagged with "vdk" \n', "    as they are not essential to the data job's execution.\n", "    However, removing tagged cells will result in a different data job run.* "]), e(["#### Tips: \n", "* *Before running the job, it is recommended to review the cells\n", "    to ensure a clear understanding of the data job run.  \n", "    This will help to ensure the desired outcome.* "]), t(['"""\n', "vdk.plugin.ipython extension introduces a magic command for Jupyter.\n", "The command enables the user to load VDK for the current notebook.\n", "VDK provides the job_input API, which has methods for:\n", "    * executing queries to an OLAP database;\n", "    * ingesting data into a database;\n", "    * processing data into a database.\n", "See the IJobInput documentation for more details.\n", "https://github.com/vmware/versatile-data-kit/blob/main/projects/vdk-core/src/vdk/api/job_input.py\n", "Please refrain from tagging this cell with VDK as it is not an actual part of the data job\n", "and is only used for development purposes.\n", '"""\n', "%reload_ext vdk.plugin.ipython\n", "%reload_VDK\n", "job_input = VDK.get_initialized_job_input()"], {});
+                                            for (const n of J) "markdown" === n.type ? e([n.source]) : "code" === n.type && t([n.source], {
+                                                tags: ["vdk"]
+                                            });
+                                            J = []
+                                        }
+                                    }
+                                })(a)
+                            })),
+                            function(e) {
+                                e.addCommand(N, {
+                                    label: T,
+                                    icon: Q.checkIcon,
+                                    execute: async e => {
+                                        const t = e.operation || "UNKNOWN",
+                                            n = e.path || "UNKNOWN";
+                                        await (0, l.showDialog)({
+                                            title: T,
+                                            body: s().createElement("div", {
+                                                className: "vdk-status-dialog-message-container"
+                                            }, s().createElement("p", {
+                                                className: "vdk-status-dialog-message"
+                                            }, s().createElement("b", null, t), " operation is currently running for job with path: ", s().createElement("i", null, n), "!")),
+                                            buttons: [l.Dialog.okButton()]
+                                        })
                                     }
-                                    o.length || (o = await async function(e) {
-                                        try {
-                                            const t = {
-                                                nbPath: e
-                                            };
-                                            return await b("vdkCellIndices", {
-                                                body: JSON.stringify(t),
-                                                method: "POST"
-                                            })
-                                        } catch (e) {
-                                            v(e)
+                                })
+                            }(u);
+                        const d = function(e) {
+                                return new $(e)
+                            }(u),
+                            h = n.defaultBrowser;
+                        e.restored.then((() => {
+                                const e = document.querySelector("#jp-top-panel");
+                                e && e.appendChild(d.element)
+                            })),
+                            function(e, t, n, o, a) {
+                                W(e, "jp-vdk:menu-run", "Run", "Execute VDK Run Command", A, a, t), W(e, "jp-vdk:menu-create", "Create", "Execute VDK Create Command", M, a), W(e, "jp-vdk:menu-download", "Download", "Execute VDK Download Command", H, a), W(e, "jp-vdk:menu-convert-job-to-notebook", "Convert Job To Notebook", "Convert Data Job To Jupyter Notebook", R, a, void 0, n, o), W(e, "jp-vdk:menu-create-deployment", "Deploy", "Create deployment of a VDK job", L, a)
+                            }(u, c, h, a, d), h.model.pathChanged.connect(ee), ((e, t) => {
+                                const n = async () => {
+                                    if (e.currentWidget && e.currentWidget.model && 0 !== e.currentWidget.model.cells.length) {
+                                        let n = [],
+                                            o = 0;
+                                        for (; e.currentWidget && e.currentWidget.model && e.currentWidget.model.cells.get(o);) {
+                                            const t = e.currentWidget.model.cells.get(o).metadata.get("tags");
+                                            t && t.includes("vdk") && n.push(o), o++
                                         }
-                                        return []
-                                    }(e.currentWidget.context.path)), o.length > 0 && e.activeCell && e.activeCell.parent && e.activeCell.parent.node.children && ((e, t, o, n) => {
-                                        Array.from(document.getElementsByClassName("jp-vdk-cell-num")).forEach((e => {
-                                            e.remove()
-                                        })), Array.from(document.getElementsByClassName("jp-vdk-failing-cell-num")).forEach((e => {
-                                            e.remove()
-                                        })), Array.from(document.getElementsByClassName("jp-vdk-logo")).forEach((e => {
-                                            e.remove()
-                                        }));
-                                        let a = 0;
-                                        for (let l = 0; l < e.length; l++) t.includes(l) ? (o.theme && o.isLight(o.theme.toString()) ? (e[l].classList.remove("jp-vdk-cell-dark"), e[l].classList.add("jp-vdk-cell")) : (e[l].classList.add("jp-vdk-cell"), e[l].classList.add("jp-vdk-cell-dark")), n && e[l] != n && q(e[l]), U(++a, e[l])) : (e[l].classList.remove("jp-vdk-cell"), e[l].classList.remove("jp-vdk-cell-dark"))
-                                    })(Array.from(e.activeCell.parent.node.children), o, t, e.activeCell.node)
-                                }
-                            };
-                            e.activeCellChanged.connect(o), t.themeChanged.connect(o)
-                        })(a, l)
+                                        n.length || (n = await async function(e) {
+                                            try {
+                                                const t = {
+                                                    nbPath: e
+                                                };
+                                                return await b("vdkCellIndices", {
+                                                    body: JSON.stringify(t),
+                                                    method: "POST"
+                                                })
+                                            } catch (e) {
+                                                v(e)
+                                            }
+                                            return []
+                                        }(e.currentWidget.context.path)), n.length > 0 && e.activeCell && e.activeCell.parent && e.activeCell.parent.node.children && ((e, t, n, o) => {
+                                            Array.from(document.getElementsByClassName("jp-vdk-cell-num")).forEach((e => {
+                                                e.remove()
+                                            })), Array.from(document.getElementsByClassName("jp-vdk-failing-cell-num")).forEach((e => {
+                                                e.remove()
+                                            })), Array.from(document.getElementsByClassName("jp-vdk-logo")).forEach((e => {
+                                                e.remove()
+                                            }));
+                                            let a = 0;
+                                            for (let l = 0; l < e.length; l++) t.includes(l) ? (n.theme && n.isLight(n.theme.toString()) ? (e[l].classList.remove("jp-vdk-cell-dark"), e[l].classList.add("jp-vdk-cell")) : (e[l].classList.add("jp-vdk-cell"), e[l].classList.add("jp-vdk-cell-dark")), o && e[l] != o && G(e[l]), Y(++a, e[l])) : (e[l].classList.remove("jp-vdk-cell"), e[l].classList.remove("jp-vdk-cell-dark"))
+                                        })(Array.from(e.activeCell.parent.node.children), n, t, e.activeCell.node)
+                                    }
+                                };
+                                e.activeCellChanged.connect(n), t.themeChanged.connect(n)
+                            })(a, r)
                     }
                 },
-                Q = async (e, t) => {
-                    G = t.newValue
+                ee = async (e, t) => {
+                    X = t.newValue
                 }
         }
     }
 ]);
```

### Comparing `vdk_jupyterlab_extension-0.1.951673056/vdk_jupyterlab_extension/labextension/static/747.e678254df7945f8ed34d.js` & `vdk_jupyterlab_extension-0.1.959565555/vdk_jupyterlab_extension/labextension/static/747.d96a6a524ff42595fecc.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -18,15 +18,15 @@
             t.d(e, {
                 Z: () => i
             });
             var r = t(645),
                 o = t.n(r)()((function(n) {
                     return n[1]
                 }));
-            o.push([n.id, "/*\n * Copyright 2021-2023 VMware, Inc.\n * SPDX-License-Identifier: Apache-2.0\n */\n\n.jp-vdk-input-wrapper {\n  display: flex;\n  flex-direction: column;\n  margin-top: 15px;\n}\n\n.hidden {\n  display: none;\n}\n\n.jp-vdk-checkbox-wrappers {\n  display: flex;\n  justify-content: flex-start;\n  align-items: center;\n  margin-left: 0;\n  padding-left: 0;\n}\n\n.jp-vdk-checkbox {\n  margin-right: 10px;\n}\n\n#enable {\n  margin-top: 10px;\n  margin-left: 0;\n}\n\n.vdk-run-error-message {\n  color: #c0392b;\n  padding: 20px;\n  font-weight: bold;\n  display: flex;\n  flex-direction: column;\n  align-items: flex-start;\n}\n\n.vdk-run-error-message p {\n  padding-bottom: 10px;\n}\n\n.vdk-run-error-message a {\n  color: #11239a;\n  text-decoration: underline;\n}\n\n.vdk-run-dialog-message {\n  font-size: 20px;\n  color: #33b53a;\n  padding: 20px;\n}\n.vdk-run-dialog-message-container {\n  position: relative;\n}\n", ""]);
+            o.push([n.id, "/*\n * Copyright 2021-2023 VMware, Inc.\n * SPDX-License-Identifier: Apache-2.0\n */\n\n.jp-vdk-input-wrapper {\n  display: flex;\n  flex-direction: column;\n  margin-top: 15px;\n}\n\n.hidden {\n  display: none;\n}\n\n.jp-vdk-checkbox-wrappers {\n  display: flex;\n  justify-content: flex-start;\n  align-items: center;\n  margin-left: 0;\n  padding-left: 0;\n}\n\n.jp-vdk-checkbox {\n  margin-right: 10px;\n}\n\n#enable {\n  margin-top: 10px;\n  margin-left: 0;\n}\n\n.vdk-run-error-message {\n  color: #c0392b;\n  padding: 20px;\n  font-weight: bold;\n  display: flex;\n  flex-direction: column;\n  align-items: flex-start;\n}\n\n.vdk-run-error-message p {\n  padding-bottom: 10px;\n}\n\n.vdk-run-error-message a {\n  color: #11239a;\n  text-decoration: underline;\n}\n\n.vdk-run-dialog-message {\n  font-size: 20px;\n  color: #33b53a;\n  padding: 20px;\n}\n.vdk-run-dialog-message-container {\n  position: relative;\n}\n\n.vdk-status-dialog-message {\n  font-size: 20px;\n  padding: 20px;\n}\n.vdk-status-dialog-message-container {\n  position: relative;\n}\n\n.jp-vdk-check-status-button {\n  position: absolute;\n  right: 1px;\n  border-radius: 5px;\n}\n\n.jp-vdk-status-button-content {\n  display: flex;\n  align-items: center;\n}\n\n.jp-vdk-check-status-button .jp-vdk-logo {\n  position: static;\n  padding-right: 5px;\n}\n\n.jp-vdk-check-status-button:hover {\n  background-color: #e0e0e0;\n  cursor: pointer;\n}\n", ""]);
             const i = o
         },
         645: n => {
             n.exports = function(n) {
                 var e = [];
                 return e.toString = function() {
                     return this.map((function(e) {
@@ -86,15 +86,15 @@
                     var p = a(d),
                         u = {
                             css: c[1],
                             media: c[2],
                             sourceMap: c[3]
                         }; - 1 !== p ? (i[p].references++, i[p].updater(u)) : i.push({
                         identifier: d,
-                        updater: h(u, e),
+                        updater: g(u, e),
                         references: 1
                     }), r.push(d)
                 }
                 return r
             }
 
             function l(n) {
@@ -137,15 +137,15 @@
                     for (; n.firstChild;) n.removeChild(n.firstChild);
                     n.appendChild(document.createTextNode(r))
                 }
             }
             var f = null,
                 v = 0;
 
-            function h(n, e) {
+            function g(n, e) {
                 var t, r, o;
                 if (e.singleton) {
                     var i = v++;
                     t = f || (f = l(e)), r = p.bind(null, t, i, !1), o = p.bind(null, t, i, !0)
                 } else t = l(e), r = u.bind(null, t, e), o = function() {
                     ! function(n) {
                         if (null === n.parentNode) return !1;
```

### Comparing `vdk_jupyterlab_extension-0.1.951673056/vdk_jupyterlab_extension/labextension/static/remoteEntry.c52cf3d95e66ca429f2e.js` & `vdk_jupyterlab_extension-0.1.959565555/vdk_jupyterlab_extension/labextension/static/remoteEntry.4fde18a81e31cc9c2aa5.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, a, i, u, l, f, d, s, p, c, h, v, b = {
+    var e, r, t, n, o, a, i, u, l, s, d, f, p, c, h, v, b = {
             913: (e, r, t) => {
                 var n = {
-                        "./index": () => t.e(161).then((() => () => t(161))),
-                        "./extension": () => t.e(161).then((() => () => t(161))),
+                        "./index": () => t.e(242).then((() => () => t(242))),
+                        "./extension": () => t.e(242).then((() => () => t(242))),
                         "./style": () => t.e(747).then((() => () => t(747)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
                     a = (e, r) => {
                         if (t.S) {
@@ -43,49 +43,49 @@
         }), r
     }, y.d = (e, r) => {
         for (var t in r) y.o(r, t) && !y.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, y.f = {}, y.e = e => Promise.all(Object.keys(y.f).reduce(((r, t) => (y.f[t](e, r), r)), [])), y.u = e => e + "." + {
-        161: "687b3e6d54b7501a02f7",
-        747: "e678254df7945f8ed34d"
+        242: "9f4f2d980858aa93e6aa",
+        747: "d96a6a524ff42595fecc"
     } [e] + ".js?v=" + {
-        161: "687b3e6d54b7501a02f7",
-        747: "e678254df7945f8ed34d"
+        242: "9f4f2d980858aa93e6aa",
+        747: "d96a6a524ff42595fecc"
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
-                for (var l = document.getElementsByTagName("script"), f = 0; f < l.length; f++) {
-                    var d = l[f];
+                for (var l = document.getElementsByTagName("script"), s = 0; s < l.length; s++) {
+                    var d = l[s];
                     if (d.getAttribute("src") == t || d.getAttribute("data-webpack") == r + o) {
                         i = d;
                         break
                     }
                 }
             i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, y.nc && i.setAttribute("nonce", y.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [n];
-            var s = (r, n) => {
+            var f = (r, n) => {
                     i.onerror = i.onload = null, clearTimeout(p);
                     var o = e[t];
                     if (delete e[t], i.parentNode && i.parentNode.removeChild(i), o && o.forEach((e => e(n))), r) return r(n)
                 },
-                p = setTimeout(s.bind(null, void 0, {
+                p = setTimeout(f.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
-            i.onerror = s.bind(null, i.onerror), i.onload = s.bind(null, i.onload), u && document.head.appendChild(i)
+            i.onerror = f.bind(null, i.onerror), i.onload = f.bind(null, i.onload), u && document.head.appendChild(i)
         }
     }, y.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
@@ -102,19 +102,19 @@
                 var a = y.S[t],
                     i = "vdk-jupyterlab-extension",
                     u = [];
                 return "default" === t && ((e, r, t, n) => {
                     var o = a[e] = a[e] || {},
                         u = o[r];
                     (!u || !u.loaded && (1 != !u.eager ? n : i > u.from)) && (o[r] = {
-                        get: () => y.e(161).then((() => () => y(161))),
+                        get: () => y.e(242).then((() => () => y(242))),
                         from: i,
                         eager: !1
                     })
-                })("vdk-jupyterlab-extension", "0.1.951673056"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                })("vdk-jupyterlab-extension", "0.1.959565555"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
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
-                var f, d, s = u < e.length ? (typeof e[u])[0] : "";
-                if (i >= r.length || "o" == (d = (typeof(f = r[i]))[0])) return !l || ("u" == s ? u > n && !o : "" == s != o);
+                var s, d, f = u < e.length ? (typeof e[u])[0] : "";
+                if (i >= r.length || "o" == (d = (typeof(s = r[i]))[0])) return !l || ("u" == f ? u > n && !o : "" == f != o);
                 if ("u" == d) {
-                    if (!l || "u" != s) return !1
+                    if (!l || "u" != f) return !1
                 } else if (l)
-                    if (s == d)
+                    if (f == d)
                         if (u <= n) {
-                            if (f != e[u]) return !1
+                            if (s != e[u]) return !1
                         } else {
-                            if (o ? f > e[u] : f < e[u]) return !1;
-                            f != e[u] && (l = !1)
+                            if (o ? s > e[u] : s < e[u]) return !1;
+                            s != e[u] && (l = !1)
                         }
-                else if ("s" != s && "n" != s) {
+                else if ("s" != f && "n" != f) {
                     if (o || u <= n) return !1;
                     l = !1, u--
                 } else {
-                    if (u <= n || d < s != o) return !1;
+                    if (u <= n || d < f != o) return !1;
                     l = !1
-                } else "s" != s && "n" != s && (l = !1, u--)
+                } else "s" != f && "n" != f && (l = !1, u--)
             }
         }
         var p = [],
             c = p.pop.bind(p);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
             p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? a(h, r) : !c())
@@ -199,33 +199,34 @@
     }, i = (e, r) => {
         var t = y.S[e];
         if (!t || !y.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, u = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
-    }, l = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", f = (e, r, t, n) => {
+    }, l = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", s = (e, r, t, n) => {
         var o = u(e, t);
-        return a(n, o) || d(l(e, t, o, n)), s(e[t][o])
+        return a(n, o) || d(l(e, t, o, n)), f(e[t][o])
     }, d = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
-    }, s = e => (e.loaded = 1, e.get()), p = (e => function(r, t, n, o) {
+    }, f = e => (e.loaded = 1, e.get()), p = (e => function(r, t, n, o) {
         var a = y.I(r);
         return a && a.then ? a.then(e.bind(e, r, y.S[r], t, n, o)) : e(r, y.S[r], t, n)
-    })(((e, r, t, n) => (i(e, t), f(r, 0, t, n)))), c = {}, h = {
+    })(((e, r, t, n) => (i(e, t), s(r, 0, t, n)))), c = {}, h = {
         33: () => p("default", "@jupyterlab/apputils", [1, 3, 6, 3]),
         38: () => p("default", "@jupyterlab/settingregistry", [1, 3, 6, 3]),
         123: () => p("default", "@jupyterlab/notebook", [1, 3, 6, 3]),
         142: () => p("default", "@jupyterlab/coreutils", [1, 5, 6, 3]),
         271: () => p("default", "react", [1, 17, 0, 1]),
         280: () => p("default", "@jupyterlab/filebrowser", [1, 3, 6, 3]),
+        502: () => p("default", "@jupyterlab/ui-components", [1, 3, 6, 3]),
         820: () => p("default", "@jupyterlab/services", [1, 6, 6, 3]),
         986: () => p("default", "@jupyterlab/docmanager", [1, 3, 6, 3])
     }, v = {
-        161: [33, 38, 123, 142, 271, 280, 820, 986]
+        242: [33, 38, 123, 142, 271, 280, 502, 820, 986]
     }, y.f.consumes = (e, r) => {
         y.o(v, e) && v[e].forEach((e => {
             if (y.o(c, e)) return r.push(c[e]);
             var t = r => {
                     c[e] = 0, y.m[e] = t => {
                         delete y.c[e], t.exports = r()
                     }
```

### Comparing `vdk_jupyterlab_extension-0.1.951673056/vdk_jupyterlab_extension/labextension/static/third-party-licenses.json` & `vdk_jupyterlab_extension-0.1.959565555/vdk_jupyterlab_extension/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.951673056/vdk_jupyterlab_extension/tests/test_convert_job_directory_processor.py` & `vdk_jupyterlab_extension-0.1.959565555/vdk_jupyterlab_extension/tests/test_convert_job_directory_processor.py`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.951673056/vdk_jupyterlab_extension/tests/test_directory_archiver.py` & `vdk_jupyterlab_extension-0.1.959565555/vdk_jupyterlab_extension/tests/test_directory_archiver.py`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.951673056/.gitignore` & `vdk_jupyterlab_extension-0.1.959565555/.gitignore`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.951673056/README.md` & `vdk_jupyterlab_extension-0.1.959565555/README.md`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.951673056/pyproject.toml` & `vdk_jupyterlab_extension-0.1.959565555/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.951673056/PKG-INFO` & `vdk_jupyterlab_extension-0.1.959565555/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-jupyterlab-extension
-Version: 0.1.951673056
+Version: 0.1.959565555
 Summary: A Jupyterlab extension for using VDK
 Project-URL: Homepage, https://github.com/vmware/versatile-data-kit
 Project-URL: Bug Tracker, https://github.com/vmware/versatile-data-kit/issues
 Project-URL: Repository, https://github.com/vmware/versatile-data-kit
 Author-email: Versatile Data Kit Development Team <versatile-data-kit@vmware.com>
 License: See https://github.com/vmware/versatile-data-kit/blob/main/LICENSE
 License-File: LICENSE
```

