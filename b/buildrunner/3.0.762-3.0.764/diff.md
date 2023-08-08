# Comparing `tmp/buildrunner-3.0.762.tar.gz` & `tmp/buildrunner-3.0.764.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buildrunner-3.0.762.tar", last modified: Thu Jul 27 19:31:11 2023, max compression
+gzip compressed data, was "buildrunner-3.0.764.tar", last modified: Fri Jul 28 16:51:37 2023, max compression
```

## Comparing `buildrunner-3.0.762.tar` & `buildrunner-3.0.764.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:31:11.338060 buildrunner-3.0.762/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-27 19:30:58.000000 buildrunner-3.0.762/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-27 19:30:58.000000 buildrunner-3.0.762/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    57840 2023-07-27 19:31:11.338060 buildrunner-3.0.762/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)    57583 2023-07-27 19:30:58.000000 buildrunner-3.0.762/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:31:11.334060 buildrunner-3.0.762/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)      159 2023-07-27 19:30:58.000000 buildrunner-3.0.762/bin/buildrunner
--rwxr-xr-x   0 runner    (1001) docker     (123)      166 2023-07-27 19:30:58.000000 buildrunner-3.0.762/bin/buildrunner-cleanup
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:31:11.334060 buildrunner-3.0.762/buildrunner/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-27 19:30:58.000000 buildrunner-3.0.762/buildrunner/SourceDockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    27674 2023-07-27 19:30:58.000000 buildrunner-3.0.762/buildrunner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8461 2023-07-27 19:30:58.000000 buildrunner-3.0.762/buildrunner/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    15314 2023-07-27 19:30:58.000000 buildrunner-3.0.762/buildrunner/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:31:11.334060 buildrunner-3.0.762/buildrunner/docker/
--rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-07-27 19:30:58.000000 buildrunner-3.0.762/buildrunner/docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6541 2023-07-27 19:30:58.000000 buildrunner-3.0.762/buildrunner/docker/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-07-27 19:30:58.000000 buildrunner-3.0.762/buildrunner/docker/daemon.py
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-07-27 19:30:58.000000 buildrunner-3.0.762/buildrunner/docker/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)    22485 2023-07-27 19:30:58.000000 buildrunner-3.0.762/buildrunner/docker/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-27 19:30:58.000000 buildrunner-3.0.762/buildrunner/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:31:11.334060 buildrunner-3.0.762/buildrunner/fetch/
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-27 19:30:58.000000 buildrunner-3.0.762/buildrunner/fetch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-27 19:30:58.000000 buildrunner-3.0.762/buildrunner/fetch/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-07-27 19:30:58.000000 buildrunner-3.0.762/buildrunner/fetch/github.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-27 19:30:58.000000 buildrunner-3.0.762/buildrunner/fetch/http.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:31:11.334060 buildrunner-3.0.762/buildrunner/provisioners/
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-27 19:30:58.000000 buildrunner-3.0.762/buildrunner/provisioners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-07-27 19:30:58.000000 buildrunner-3.0.762/buildrunner/provisioners/salt.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-27 19:30:58.000000 buildrunner-3.0.762/buildrunner/provisioners/shell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:31:11.338060 buildrunner-3.0.762/buildrunner/sshagent/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:31:11.338060 buildrunner-3.0.762/buildrunner/sshagent/SSHAgentProxyImage/
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-27 19:30:58.000000 buildrunner-3.0.762/buildrunner/sshagent/SSHAgentProxyImage/Dockerfile
--rwxr-xr-x   0 runner    (1001) docker     (123)      212 2023-07-27 19:30:58.000000 buildrunner-3.0.762/buildrunner/sshagent/SSHAgentProxyImage/login.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      338 2023-07-27 19:30:58.000000 buildrunner-3.0.762/buildrunner/sshagent/SSHAgentProxyImage/run.sh
--rw-r--r--   0 runner    (1001) docker     (123)    14938 2023-07-27 19:30:58.000000 buildrunner-3.0.762/buildrunner/sshagent/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:31:11.338060 buildrunner-3.0.762/buildrunner/steprunner/
--rw-r--r--   0 runner    (1001) docker     (123)     3927 2023-07-27 19:30:58.000000 buildrunner-3.0.762/buildrunner/steprunner/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:31:11.338060 buildrunner-3.0.762/buildrunner/steprunner/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-27 19:30:58.000000 buildrunner-3.0.762/buildrunner/steprunner/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9907 2023-07-27 19:30:58.000000 buildrunner-3.0.762/buildrunner/steprunner/tasks/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     6486 2023-07-27 19:30:58.000000 buildrunner-3.0.762/buildrunner/steprunner/tasks/push.py
--rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-07-27 19:30:58.000000 buildrunner-3.0.762/buildrunner/steprunner/tasks/pypipush.py
--rw-r--r--   0 runner    (1001) docker     (123)     6628 2023-07-27 19:30:58.000000 buildrunner-3.0.762/buildrunner/steprunner/tasks/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)    44014 2023-07-27 19:30:58.000000 buildrunner-3.0.762/buildrunner/steprunner/tasks/run.py
--rw-r--r--   0 runner    (1001) docker     (123)    13278 2023-07-27 19:30:58.000000 buildrunner-3.0.762/buildrunner/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-27 19:31:11.000000 buildrunner-3.0.762/buildrunner/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:31:11.334060 buildrunner-3.0.762/buildrunner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    57840 2023-07-27 19:31:11.000000 buildrunner-3.0.762/buildrunner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-07-27 19:31:11.000000 buildrunner-3.0.762/buildrunner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 19:31:11.000000 buildrunner-3.0.762/buildrunner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-27 19:31:11.000000 buildrunner-3.0.762/buildrunner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-27 19:31:11.000000 buildrunner-3.0.762/buildrunner.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-07-27 19:30:58.000000 buildrunner-3.0.762/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-27 19:31:11.338060 buildrunner-3.0.762/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-07-27 19:30:58.000000 buildrunner-3.0.762/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-27 19:30:58.000000 buildrunner-3.0.762/test_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:31:11.338060 buildrunner-3.0.762/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-07-27 19:30:58.000000 buildrunner-3.0.762/tests/test_buildrunner_files.py
--rw-r--r--   0 runner    (1001) docker     (123)    15123 2023-07-27 19:30:58.000000 buildrunner-3.0.762/tests/test_caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-27 19:30:58.000000 buildrunner-3.0.762/tests/test_console_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-07-27 19:30:58.000000 buildrunner-3.0.762/tests/test_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-07-27 19:30:58.000000 buildrunner-3.0.762/tests/test_push_artifact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-07-27 19:30:58.000000 buildrunner-3.0.762/tests/test_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-27 19:30:58.000000 buildrunner-3.0.762/tests/test_util_checksum.py
--rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-07-27 19:30:58.000000 buildrunner-3.0.762/tests/test_utils_flock.py
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-07-27 19:30:58.000000 buildrunner-3.0.762/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:51:37.797673 buildrunner-3.0.764/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-28 16:51:27.000000 buildrunner-3.0.764/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-28 16:51:27.000000 buildrunner-3.0.764/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    57840 2023-07-28 16:51:37.797673 buildrunner-3.0.764/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)    57583 2023-07-28 16:51:27.000000 buildrunner-3.0.764/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:51:37.789673 buildrunner-3.0.764/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      159 2023-07-28 16:51:27.000000 buildrunner-3.0.764/bin/buildrunner
+-rwxr-xr-x   0 runner    (1001) docker     (123)      166 2023-07-28 16:51:27.000000 buildrunner-3.0.764/bin/buildrunner-cleanup
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:51:37.793673 buildrunner-3.0.764/buildrunner/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-28 16:51:27.000000 buildrunner-3.0.764/buildrunner/SourceDockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    27674 2023-07-28 16:51:27.000000 buildrunner-3.0.764/buildrunner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8461 2023-07-28 16:51:27.000000 buildrunner-3.0.764/buildrunner/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15314 2023-07-28 16:51:27.000000 buildrunner-3.0.764/buildrunner/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:51:37.793673 buildrunner-3.0.764/buildrunner/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-07-28 16:51:27.000000 buildrunner-3.0.764/buildrunner/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6541 2023-07-28 16:51:27.000000 buildrunner-3.0.764/buildrunner/docker/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-07-28 16:51:27.000000 buildrunner-3.0.764/buildrunner/docker/daemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-07-28 16:51:27.000000 buildrunner-3.0.764/buildrunner/docker/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22485 2023-07-28 16:51:27.000000 buildrunner-3.0.764/buildrunner/docker/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-28 16:51:27.000000 buildrunner-3.0.764/buildrunner/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:51:37.793673 buildrunner-3.0.764/buildrunner/fetch/
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-28 16:51:27.000000 buildrunner-3.0.764/buildrunner/fetch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-28 16:51:27.000000 buildrunner-3.0.764/buildrunner/fetch/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-07-28 16:51:27.000000 buildrunner-3.0.764/buildrunner/fetch/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-28 16:51:27.000000 buildrunner-3.0.764/buildrunner/fetch/http.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:51:37.793673 buildrunner-3.0.764/buildrunner/provisioners/
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-28 16:51:27.000000 buildrunner-3.0.764/buildrunner/provisioners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-07-28 16:51:27.000000 buildrunner-3.0.764/buildrunner/provisioners/salt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-28 16:51:27.000000 buildrunner-3.0.764/buildrunner/provisioners/shell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:51:37.793673 buildrunner-3.0.764/buildrunner/sshagent/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:51:37.793673 buildrunner-3.0.764/buildrunner/sshagent/SSHAgentProxyImage/
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-28 16:51:27.000000 buildrunner-3.0.764/buildrunner/sshagent/SSHAgentProxyImage/Dockerfile
+-rwxr-xr-x   0 runner    (1001) docker     (123)      212 2023-07-28 16:51:27.000000 buildrunner-3.0.764/buildrunner/sshagent/SSHAgentProxyImage/login.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      338 2023-07-28 16:51:27.000000 buildrunner-3.0.764/buildrunner/sshagent/SSHAgentProxyImage/run.sh
+-rw-r--r--   0 runner    (1001) docker     (123)    14938 2023-07-28 16:51:27.000000 buildrunner-3.0.764/buildrunner/sshagent/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:51:37.793673 buildrunner-3.0.764/buildrunner/steprunner/
+-rw-r--r--   0 runner    (1001) docker     (123)     3927 2023-07-28 16:51:27.000000 buildrunner-3.0.764/buildrunner/steprunner/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:51:37.797673 buildrunner-3.0.764/buildrunner/steprunner/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-28 16:51:27.000000 buildrunner-3.0.764/buildrunner/steprunner/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9907 2023-07-28 16:51:27.000000 buildrunner-3.0.764/buildrunner/steprunner/tasks/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6486 2023-07-28 16:51:27.000000 buildrunner-3.0.764/buildrunner/steprunner/tasks/push.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-07-28 16:51:27.000000 buildrunner-3.0.764/buildrunner/steprunner/tasks/pypipush.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6628 2023-07-28 16:51:27.000000 buildrunner-3.0.764/buildrunner/steprunner/tasks/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44014 2023-07-28 16:51:27.000000 buildrunner-3.0.764/buildrunner/steprunner/tasks/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13278 2023-07-28 16:51:27.000000 buildrunner-3.0.764/buildrunner/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-28 16:51:37.000000 buildrunner-3.0.764/buildrunner/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:51:37.793673 buildrunner-3.0.764/buildrunner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    57840 2023-07-28 16:51:37.000000 buildrunner-3.0.764/buildrunner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-07-28 16:51:37.000000 buildrunner-3.0.764/buildrunner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 16:51:37.000000 buildrunner-3.0.764/buildrunner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-28 16:51:37.000000 buildrunner-3.0.764/buildrunner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-28 16:51:37.000000 buildrunner-3.0.764/buildrunner.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-07-28 16:51:27.000000 buildrunner-3.0.764/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-28 16:51:37.797673 buildrunner-3.0.764/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-07-28 16:51:27.000000 buildrunner-3.0.764/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-28 16:51:27.000000 buildrunner-3.0.764/test_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:51:37.797673 buildrunner-3.0.764/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-07-28 16:51:27.000000 buildrunner-3.0.764/tests/test_buildrunner_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15123 2023-07-28 16:51:27.000000 buildrunner-3.0.764/tests/test_caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-28 16:51:27.000000 buildrunner-3.0.764/tests/test_console_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-07-28 16:51:27.000000 buildrunner-3.0.764/tests/test_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-07-28 16:51:27.000000 buildrunner-3.0.764/tests/test_push_artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-07-28 16:51:27.000000 buildrunner-3.0.764/tests/test_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-28 16:51:27.000000 buildrunner-3.0.764/tests/test_util_checksum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-07-28 16:51:27.000000 buildrunner-3.0.764/tests/test_utils_flock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-07-28 16:51:27.000000 buildrunner-3.0.764/tests/test_version.py
```

### Comparing `buildrunner-3.0.762/LICENSE` & `buildrunner-3.0.764/LICENSE`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.762/PKG-INFO` & `buildrunner-3.0.764/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildrunner
-Version: 3.0.762
+Version: 3.0.764
 Summary: Docker-based build tool
 Home-page: https://github.com/adobe/buildrunner
 Author: Adobe
 Author-email: noreply@adobe.com
 License: MIT
 Description-Content-Type: text/x-rst
 License-File: LICENSE
```

### Comparing `buildrunner-3.0.762/README.rst` & `buildrunner-3.0.764/README.rst`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.762/buildrunner/__init__.py` & `buildrunner-3.0.764/buildrunner/__init__.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.762/buildrunner/cli.py` & `buildrunner-3.0.764/buildrunner/cli.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.762/buildrunner/config.py` & `buildrunner-3.0.764/buildrunner/config.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.762/buildrunner/docker/__init__.py` & `buildrunner-3.0.764/buildrunner/docker/__init__.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.762/buildrunner/docker/builder.py` & `buildrunner-3.0.764/buildrunner/docker/builder.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.762/buildrunner/docker/daemon.py` & `buildrunner-3.0.764/buildrunner/docker/daemon.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.762/buildrunner/docker/importer.py` & `buildrunner-3.0.764/buildrunner/docker/importer.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.762/buildrunner/docker/runner.py` & `buildrunner-3.0.764/buildrunner/docker/runner.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.762/buildrunner/errors.py` & `buildrunner-3.0.764/buildrunner/errors.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.762/buildrunner/fetch/__init__.py` & `buildrunner-3.0.764/buildrunner/fetch/__init__.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.762/buildrunner/fetch/github.py` & `buildrunner-3.0.764/buildrunner/fetch/github.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.762/buildrunner/provisioners/__init__.py` & `buildrunner-3.0.764/buildrunner/provisioners/__init__.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.762/buildrunner/provisioners/salt.py` & `buildrunner-3.0.764/buildrunner/provisioners/salt.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.762/buildrunner/provisioners/shell.py` & `buildrunner-3.0.764/buildrunner/provisioners/shell.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.762/buildrunner/sshagent/SSHAgentProxyImage/Dockerfile` & `buildrunner-3.0.764/buildrunner/sshagent/SSHAgentProxyImage/Dockerfile`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.762/buildrunner/sshagent/__init__.py` & `buildrunner-3.0.764/buildrunner/sshagent/__init__.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.762/buildrunner/steprunner/__init__.py` & `buildrunner-3.0.764/buildrunner/steprunner/__init__.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.762/buildrunner/steprunner/tasks/__init__.py` & `buildrunner-3.0.764/buildrunner/steprunner/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.762/buildrunner/steprunner/tasks/build.py` & `buildrunner-3.0.764/buildrunner/steprunner/tasks/build.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.762/buildrunner/steprunner/tasks/push.py` & `buildrunner-3.0.764/buildrunner/steprunner/tasks/push.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.762/buildrunner/steprunner/tasks/pypipush.py` & `buildrunner-3.0.764/buildrunner/steprunner/tasks/pypipush.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.762/buildrunner/steprunner/tasks/remote.py` & `buildrunner-3.0.764/buildrunner/steprunner/tasks/remote.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.762/buildrunner/steprunner/tasks/run.py` & `buildrunner-3.0.764/buildrunner/steprunner/tasks/run.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.762/buildrunner/utils.py` & `buildrunner-3.0.764/buildrunner/utils.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.762/buildrunner.egg-info/PKG-INFO` & `buildrunner-3.0.764/buildrunner.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildrunner
-Version: 3.0.762
+Version: 3.0.764
 Summary: Docker-based build tool
 Home-page: https://github.com/adobe/buildrunner
 Author: Adobe
 Author-email: noreply@adobe.com
 License: MIT
 Description-Content-Type: text/x-rst
 License-File: LICENSE
```

### Comparing `buildrunner-3.0.762/buildrunner.egg-info/SOURCES.txt` & `buildrunner-3.0.764/buildrunner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.762/buildrunner.egg-info/requires.txt` & `buildrunner-3.0.764/buildrunner.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.762/requirements.txt` & `buildrunner-3.0.764/requirements.txt`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.762/setup.py` & `buildrunner-3.0.764/setup.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.762/test_requirements.txt` & `buildrunner-3.0.764/test_requirements.txt`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.762/tests/test_buildrunner_files.py` & `buildrunner-3.0.764/tests/test_buildrunner_files.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.762/tests/test_caching.py` & `buildrunner-3.0.764/tests/test_caching.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.762/tests/test_console_logger.py` & `buildrunner-3.0.764/tests/test_console_logger.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.762/tests/test_dependencies.py` & `buildrunner-3.0.764/tests/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.762/tests/test_push_artifact.py` & `buildrunner-3.0.764/tests/test_push_artifact.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.762/tests/test_runner.py` & `buildrunner-3.0.764/tests/test_runner.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.762/tests/test_util_checksum.py` & `buildrunner-3.0.764/tests/test_util_checksum.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.762/tests/test_utils_flock.py` & `buildrunner-3.0.764/tests/test_utils_flock.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.762/tests/test_version.py` & `buildrunner-3.0.764/tests/test_version.py`

 * *Files identical despite different names*

