# Comparing `tmp/apache-airflow-providers-cncf-kubernetes-7.4.1.tar.gz` & `tmp/apache-airflow-providers-cncf-kubernetes-7.4.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-cncf-kubernetes-7.4.1.tar", last modified: Fri Aug  4 21:35:15 2023, max compression
+gzip compressed data, was "apache-airflow-providers-cncf-kubernetes-7.4.1rc1.tar", last modified: Fri Aug  4 21:40:55 2023, max compression
```

## Comparing `apache-airflow-providers-cncf-kubernetes-7.4.1.tar` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:15.674228 apache-airflow-providers-cncf-kubernetes-7.4.1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-cncf-kubernetes-7.4.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1156 2023-08-04 21:35:14.000000 apache-airflow-providers-cncf-kubernetes-7.4.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-cncf-kubernetes-7.4.1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     4631 2023-08-04 21:35:15.674838 apache-airflow-providers-cncf-kubernetes-7.4.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2960 2023-08-04 21:35:14.000000 apache-airflow-providers-cncf-kubernetes-7.4.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:15.483250 apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:15.484322 apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:15.485308 apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:15.561395 apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/
--rw-r--r--   0 root         (0) root         (0)     1584 2023-08-04 21:33:34.000000 apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:15.566866 apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/backcompat/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/backcompat/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3914 2023-06-02 11:31:21.000000 apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/backcompat/backwards_compat_converters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:15.572302 apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/decorators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/decorators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6178 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/decorators/kubernetes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:15.587572 apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/executors/
--rw-r--r--   0 root         (0) root         (0)      787 2023-07-26 06:59:50.000000 apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/executors/__init__.py
--rw-r--r--   0 root         (0) root         (0)    30457 2023-08-04 19:44:14.000000 apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/executors/kubernetes_executor.py
--rw-r--r--   0 root         (0) root         (0)     1540 2023-07-26 06:59:50.000000 apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/executors/kubernetes_executor_types.py
--rw-r--r--   0 root         (0) root         (0)    21132 2023-07-26 06:59:50.000000 apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/executors/kubernetes_executor_utils.py
--rw-r--r--   0 root         (0) root         (0)     9983 2023-07-29 06:50:08.000000 apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/executors/local_kubernetes_executor.py
--rw-r--r--   0 root         (0) root         (0)    15886 2023-08-04 21:35:14.000000 apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:15.593450 apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/hooks/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23948 2023-08-04 19:44:14.000000 apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/hooks/kubernetes.py
--rw-r--r--   0 root         (0) root         (0)     2045 2023-07-26 06:59:50.000000 apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/k8s_model.py
--rw-r--r--   0 root         (0) root         (0)     5344 2023-07-26 06:59:50.000000 apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/kube_client.py
--rw-r--r--   0 root         (0) root         (0)     4851 2023-07-26 06:59:50.000000 apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/kube_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:15.596721 apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/kubernetes_executor_templates/
--rw-r--r--   0 root         (0) root         (0)      785 2023-07-26 06:59:50.000000 apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/kubernetes_executor_templates/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4741 2023-07-26 06:59:50.000000 apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/kubernetes_helper_functions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:15.612409 apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1262 2023-07-16 17:25:26.000000 apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/operators/kubernetes_pod.py
--rw-r--r--   0 root         (0) root         (0)    41626 2023-08-04 19:44:14.000000 apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/operators/pod.py
--rw-r--r--   0 root         (0) root         (0)     3827 2023-06-08 05:42:54.000000 apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/operators/resource.py
--rw-r--r--   0 root         (0) root         (0)     7387 2023-07-26 06:59:50.000000 apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/operators/spark_kubernetes.py
--rw-r--r--   0 root         (0) root         (0)    23849 2023-07-26 06:59:50.000000 apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/pod_generator.py
--rw-r--r--   0 root         (0) root         (0)    12129 2023-07-26 06:59:50.000000 apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/pod_generator_deprecated.py
--rw-r--r--   0 root         (0) root         (0)    12039 2023-07-26 06:59:50.000000 apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/pod_launcher_deprecated.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:15.615280 apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/pod_template_file_examples/
--rw-r--r--   0 root         (0) root         (0)      785 2023-07-26 06:59:50.000000 apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/pod_template_file_examples/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1741 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/python_kubernetes_script.jinja2
--rw-r--r--   0 root         (0) root         (0)     3345 2023-06-02 11:31:21.000000 apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/python_kubernetes_script.py
--rw-r--r--   0 root         (0) root         (0)     5213 2023-07-26 06:59:50.000000 apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/secret.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:15.620869 apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/sensors/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5226 2023-06-02 11:31:21.000000 apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/sensors/spark_kubernetes.py
--rw-r--r--   0 root         (0) root         (0)     2900 2023-07-26 06:59:50.000000 apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/template_rendering.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:15.629214 apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/triggers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/triggers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1259 2023-07-16 17:25:26.000000 apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/triggers/kubernetes_pod.py
--rw-r--r--   0 root         (0) root         (0)    11511 2023-07-12 12:42:21.000000 apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/triggers/pod.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:15.647797 apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/utils/
--rw-r--r--   0 root         (0) root         (0)      863 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5176 2023-06-29 05:49:30.000000 apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/utils/delete_from.py
--rw-r--r--   0 root         (0) root         (0)     1553 2023-07-26 06:59:50.000000 apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/utils/k8s_hashlib_wrapper.py
--rw-r--r--   0 root         (0) root         (0)    29231 2023-08-04 19:44:14.000000 apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/utils/pod_manager.py
--rw-r--r--   0 root         (0) root         (0)     2519 2023-06-29 05:49:30.000000 apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/utils/xcom_sidecar.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:15.671454 apache-airflow-providers-cncf-kubernetes-7.4.1/apache_airflow_providers_cncf_kubernetes.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4631 2023-08-04 21:35:15.000000 apache-airflow-providers-cncf-kubernetes-7.4.1/apache_airflow_providers_cncf_kubernetes.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2931 2023-08-04 21:35:15.000000 apache-airflow-providers-cncf-kubernetes-7.4.1/apache_airflow_providers_cncf_kubernetes.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 21:35:15.000000 apache-airflow-providers-cncf-kubernetes-7.4.1/apache_airflow_providers_cncf_kubernetes.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      112 2023-08-04 21:35:15.000000 apache-airflow-providers-cncf-kubernetes-7.4.1/apache_airflow_providers_cncf_kubernetes.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 21:35:15.000000 apache-airflow-providers-cncf-kubernetes-7.4.1/apache_airflow_providers_cncf_kubernetes.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      112 2023-08-04 21:35:15.000000 apache-airflow-providers-cncf-kubernetes-7.4.1/apache_airflow_providers_cncf_kubernetes.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-08-04 21:35:15.000000 apache-airflow-providers-cncf-kubernetes-7.4.1/apache_airflow_providers_cncf_kubernetes.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5031 2023-08-04 10:24:23.000000 apache-airflow-providers-cncf-kubernetes-7.4.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     2074 2023-08-04 21:35:15.676790 apache-airflow-providers-cncf-kubernetes-7.4.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1692 2023-08-04 21:35:14.000000 apache-airflow-providers-cncf-kubernetes-7.4.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:55.958168 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1156 2023-08-04 21:40:54.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     4637 2023-08-04 21:40:55.958772 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2963 2023-08-04 21:40:54.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:55.764664 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:55.765711 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:55.766783 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:55.846230 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/
+-rw-r--r--   0 root         (0) root         (0)     1584 2023-08-04 21:33:34.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:55.853709 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/backcompat/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/backcompat/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3914 2023-06-02 11:31:21.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/backcompat/backwards_compat_converters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:55.860425 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/decorators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/decorators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6178 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/decorators/kubernetes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:55.875097 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/executors/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-07-26 06:59:50.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/executors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    30457 2023-08-04 19:44:14.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/executors/kubernetes_executor.py
+-rw-r--r--   0 root         (0) root         (0)     1540 2023-07-26 06:59:50.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/executors/kubernetes_executor_types.py
+-rw-r--r--   0 root         (0) root         (0)    21132 2023-07-26 06:59:50.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/executors/kubernetes_executor_utils.py
+-rw-r--r--   0 root         (0) root         (0)     9983 2023-07-29 06:50:08.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/executors/local_kubernetes_executor.py
+-rw-r--r--   0 root         (0) root         (0)    15886 2023-08-04 21:40:54.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:55.880849 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/hooks/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23948 2023-08-04 19:44:14.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/hooks/kubernetes.py
+-rw-r--r--   0 root         (0) root         (0)     2045 2023-07-26 06:59:50.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/k8s_model.py
+-rw-r--r--   0 root         (0) root         (0)     5344 2023-07-26 06:59:50.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/kube_client.py
+-rw-r--r--   0 root         (0) root         (0)     4851 2023-07-26 06:59:50.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/kube_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:55.883891 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/kubernetes_executor_templates/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-07-26 06:59:50.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/kubernetes_executor_templates/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4741 2023-07-26 06:59:50.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/kubernetes_helper_functions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:55.898723 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1262 2023-07-16 17:25:26.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/operators/kubernetes_pod.py
+-rw-r--r--   0 root         (0) root         (0)    41626 2023-08-04 19:44:14.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/operators/pod.py
+-rw-r--r--   0 root         (0) root         (0)     3827 2023-06-08 05:42:54.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/operators/resource.py
+-rw-r--r--   0 root         (0) root         (0)     7387 2023-07-26 06:59:50.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/operators/spark_kubernetes.py
+-rw-r--r--   0 root         (0) root         (0)    23849 2023-07-26 06:59:50.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/pod_generator.py
+-rw-r--r--   0 root         (0) root         (0)    12129 2023-07-26 06:59:50.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/pod_generator_deprecated.py
+-rw-r--r--   0 root         (0) root         (0)    12039 2023-07-26 06:59:50.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/pod_launcher_deprecated.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:55.901607 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/pod_template_file_examples/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-07-26 06:59:50.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/pod_template_file_examples/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1741 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.jinja2
+-rw-r--r--   0 root         (0) root         (0)     3345 2023-06-02 11:31:21.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.py
+-rw-r--r--   0 root         (0) root         (0)     5213 2023-07-26 06:59:50.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/secret.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:55.907390 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/sensors/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5226 2023-06-02 11:31:21.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/sensors/spark_kubernetes.py
+-rw-r--r--   0 root         (0) root         (0)     2900 2023-07-26 06:59:50.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/template_rendering.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:55.916333 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/triggers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/triggers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1259 2023-07-16 17:25:26.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/triggers/kubernetes_pod.py
+-rw-r--r--   0 root         (0) root         (0)    11511 2023-07-12 12:42:21.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/triggers/pod.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:55.931113 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/utils/
+-rw-r--r--   0 root         (0) root         (0)      863 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5176 2023-06-29 05:49:30.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/utils/delete_from.py
+-rw-r--r--   0 root         (0) root         (0)     1553 2023-07-26 06:59:50.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/utils/k8s_hashlib_wrapper.py
+-rw-r--r--   0 root         (0) root         (0)    29231 2023-08-04 19:44:14.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/utils/pod_manager.py
+-rw-r--r--   0 root         (0) root         (0)     2519 2023-06-29 05:49:30.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/utils/xcom_sidecar.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:55.955467 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/apache_airflow_providers_cncf_kubernetes.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4637 2023-08-04 21:40:55.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/apache_airflow_providers_cncf_kubernetes.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2931 2023-08-04 21:40:55.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/apache_airflow_providers_cncf_kubernetes.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 21:40:55.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/apache_airflow_providers_cncf_kubernetes.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      112 2023-08-04 21:40:55.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/apache_airflow_providers_cncf_kubernetes.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 21:40:55.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/apache_airflow_providers_cncf_kubernetes.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      117 2023-08-04 21:40:55.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/apache_airflow_providers_cncf_kubernetes.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-08-04 21:40:55.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/apache_airflow_providers_cncf_kubernetes.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5031 2023-08-04 10:24:23.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     2082 2023-08-04 21:40:55.960691 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1692 2023-08-04 21:40:54.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/setup.py
```

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.1/LICENSE` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.1/MANIFEST.in` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.1/PKG-INFO` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-cncf-kubernetes
-Version: 7.4.1
+Version: 7.4.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-cncf-kubernetes package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.4.1/
@@ -66,15 +66,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-cncf-kubernetes``
 
-Release: ``7.4.1``
+Release: ``7.4.1rc1``
 
 
 `Kubernetes <https://kubernetes.io/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.1/README.rst` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-cncf-kubernetes``
 
-Release: ``7.4.1``
+Release: ``7.4.1rc1``
 
 
 `Kubernetes <https://kubernetes.io/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/__init__.py` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/backcompat/__init__.py` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/backcompat/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/backcompat/backwards_compat_converters.py` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/backcompat/backwards_compat_converters.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/decorators/__init__.py` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/decorators/kubernetes.py` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/decorators/kubernetes.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/executors/__init__.py` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/executors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/executors/kubernetes_executor.py` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/executors/kubernetes_executor.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/executors/kubernetes_executor_types.py` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/executors/kubernetes_executor_types.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/executors/kubernetes_executor_utils.py` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/executors/kubernetes_executor_utils.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/executors/local_kubernetes_executor.py` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/executors/local_kubernetes_executor.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/get_provider_info.py` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/hooks/__init__.py` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/hooks/kubernetes.py` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/hooks/kubernetes.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/k8s_model.py` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/k8s_model.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/kube_client.py` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/kube_client.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/kube_config.py` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/kube_config.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/kubernetes_executor_templates/__init__.py` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/kubernetes_executor_templates/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/kubernetes_helper_functions.py` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/kubernetes_helper_functions.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/operators/__init__.py` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/operators/kubernetes_pod.py` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/operators/kubernetes_pod.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/operators/pod.py` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/operators/pod.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/operators/resource.py` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/operators/resource.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/operators/spark_kubernetes.py` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/operators/spark_kubernetes.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/pod_generator.py` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/pod_generator.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/pod_generator_deprecated.py` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/pod_generator_deprecated.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/pod_launcher_deprecated.py` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/pod_launcher_deprecated.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/pod_template_file_examples/__init__.py` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/pod_template_file_examples/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/python_kubernetes_script.jinja2` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.jinja2`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/python_kubernetes_script.py` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/secret.py` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/secret.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/sensors/__init__.py` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/sensors/spark_kubernetes.py` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/sensors/spark_kubernetes.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/template_rendering.py` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/template_rendering.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/triggers/__init__.py` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/triggers/kubernetes_pod.py` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/triggers/kubernetes_pod.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/triggers/pod.py` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/triggers/pod.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/utils/__init__.py` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/utils/delete_from.py` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/utils/delete_from.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/utils/k8s_hashlib_wrapper.py` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/utils/k8s_hashlib_wrapper.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/utils/pod_manager.py` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/utils/pod_manager.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.1/airflow/providers/cncf/kubernetes/utils/xcom_sidecar.py` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/utils/xcom_sidecar.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.1/apache_airflow_providers_cncf_kubernetes.egg-info/PKG-INFO` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/apache_airflow_providers_cncf_kubernetes.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-cncf-kubernetes
-Version: 7.4.1
+Version: 7.4.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-cncf-kubernetes package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.4.1/
@@ -66,15 +66,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-cncf-kubernetes``
 
-Release: ``7.4.1``
+Release: ``7.4.1rc1``
 
 
 `Kubernetes <https://kubernetes.io/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.1/apache_airflow_providers_cncf_kubernetes.egg-info/SOURCES.txt` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/apache_airflow_providers_cncf_kubernetes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.1/pyproject.toml` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.1/setup.cfg` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -43,24 +43,24 @@
 include_package_data = True
 python_requires = ~=3.8
 packages = find:
 setup_requires = 
 	setuptools
 	wheel
 install_requires = 
-	apache-airflow>=2.4.0
+	apache-airflow>=2.4.0.dev0
 	asgiref>=3.5.2
 	cryptography>=2.0.0
 	kubernetes>=21.7.0,<24
 	kubernetes_asyncio>=18.20.1,<25
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.cncf.kubernetes.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.cncf.kubernetes
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.1/setup.py` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/setup.py`

 * *Files identical despite different names*

