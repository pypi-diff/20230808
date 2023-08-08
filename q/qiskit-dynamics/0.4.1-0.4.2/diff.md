# Comparing `tmp/qiskit-dynamics-0.4.1.tar.gz` & `tmp/qiskit-dynamics-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qiskit-dynamics-0.4.1.tar", last modified: Fri Jun  9 21:53:00 2023, max compression
+gzip compressed data, was "qiskit-dynamics-0.4.2.tar", last modified: Tue Aug  8 14:55:08 2023, max compression
```

## Comparing `qiskit-dynamics-0.4.1.tar` & `qiskit-dynamics-0.4.2.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 21:53:00.037000 qiskit-dynamics-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11416 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5031 2023-06-09 21:53:00.037000 qiskit-dynamics-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 21:53:00.028999 qiskit-dynamics-0.4.1/qiskit_dynamics/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/VERSION.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 21:53:00.032999 qiskit-dynamics-0.4.1/qiskit_dynamics/array/
--rw-r--r--   0 runner    (1001) docker     (123)     6892 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/array/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10887 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/array/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/array/patch_qi.py
--rw-r--r--   0 runner    (1001) docker     (123)     7035 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/array/wrap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 21:53:00.032999 qiskit-dynamics-0.4.1/qiskit_dynamics/backend/
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 21:53:00.032999 qiskit-dynamics-0.4.1/qiskit_dynamics/backend/backend_string_parser/
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/backend/backend_string_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12497 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/backend/backend_string_parser/hamiltonian_string_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/backend/backend_string_parser/operator_from_string.py
--rw-r--r--   0 runner    (1001) docker     (123)    13994 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/backend/backend_string_parser/regex_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     9822 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/backend/backend_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    44918 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/backend/dynamics_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/backend/dynamics_job.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 21:53:00.032999 qiskit-dynamics-0.4.1/qiskit_dynamics/dispatch/
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/dispatch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 21:53:00.032999 qiskit-dynamics-0.4.1/qiskit_dynamics/dispatch/backends/
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/dispatch/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/dispatch/backends/jax.py
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/dispatch/backends/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)    11769 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/dispatch/dispatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/dispatch/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 21:53:00.032999 qiskit-dynamics-0.4.1/qiskit_dynamics/models/
--rw-r--r--   0 runner    (1001) docker     (123)     5678 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21116 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/models/generator_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8531 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/models/hamiltonian_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    29123 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/models/lindblad_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    62696 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/models/operator_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)    26059 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/models/rotating_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)    12484 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/models/rotating_wave_approximation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 21:53:00.032999 qiskit-dynamics-0.4.1/qiskit_dynamics/perturbation/
--rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/perturbation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33060 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/perturbation/array_polynomial.py
--rw-r--r--   0 runner    (1001) docker     (123)    12155 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/perturbation/custom_binary_op.py
--rw-r--r--   0 runner    (1001) docker     (123)    30869 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/perturbation/dyson_magnus.py
--rw-r--r--   0 runner    (1001) docker     (123)     7322 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/perturbation/multiset_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/perturbation/perturbation_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/perturbation/perturbation_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    15298 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/perturbation/solve_lmde_perturbation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 21:53:00.032999 qiskit-dynamics-0.4.1/qiskit_dynamics/pulse/
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/pulse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15322 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/pulse/pulse_to_signals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 21:53:00.032999 qiskit-dynamics-0.4.1/qiskit_dynamics/signals/
--rw-r--r--   0 runner    (1001) docker     (123)     8818 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/signals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40271 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/signals/signals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7425 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/signals/transfer_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 21:53:00.037000 qiskit-dynamics-0.4.1/qiskit_dynamics/solvers/
--rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/solvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/solvers/diffrax_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)    21554 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/solvers/fixed_step_solvers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/solvers/jax_odeint.py
--rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/solvers/lanczos.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 21:53:00.037000 qiskit-dynamics-0.4.1/qiskit_dynamics/solvers/perturbative_solvers/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/solvers/perturbative_solvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9185 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/solvers/perturbative_solvers/dyson_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)    20128 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/solvers/perturbative_solvers/expansion_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/solvers/perturbative_solvers/magnus_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     7094 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/solvers/perturbative_solvers/perturbative_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/solvers/scipy_solve_ivp.py
--rw-r--r--   0 runner    (1001) docker     (123)    38811 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/solvers/solver_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)    18579 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/solvers/solver_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10587 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/solvers/solver_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16654 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/type_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 21:53:00.028999 qiskit-dynamics-0.4.1/qiskit_dynamics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5031 2023-06-09 21:52:59.000000 qiskit-dynamics-0.4.1/qiskit_dynamics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-06-09 21:52:59.000000 qiskit-dynamics-0.4.1/qiskit_dynamics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 21:52:59.000000 qiskit-dynamics-0.4.1/qiskit_dynamics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 21:52:59.000000 qiskit-dynamics-0.4.1/qiskit_dynamics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-09 21:52:59.000000 qiskit-dynamics-0.4.1/qiskit_dynamics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-09 21:52:59.000000 qiskit-dynamics-0.4.1/qiskit_dynamics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 21:53:00.037000 qiskit-dynamics-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:55:08.029363 qiskit-dynamics-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11416 2023-08-08 14:54:57.000000 qiskit-dynamics-0.4.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-08 14:54:57.000000 qiskit-dynamics-0.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5031 2023-08-08 14:55:08.029363 qiskit-dynamics-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-08-08 14:54:57.000000 qiskit-dynamics-0.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-08-08 14:54:57.000000 qiskit-dynamics-0.4.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:55:08.017362 qiskit-dynamics-0.4.2/qiskit_dynamics/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-08 14:54:57.000000 qiskit-dynamics-0.4.2/qiskit_dynamics/VERSION.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-08-08 14:54:57.000000 qiskit-dynamics-0.4.2/qiskit_dynamics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:55:08.025363 qiskit-dynamics-0.4.2/qiskit_dynamics/array/
+-rw-r--r--   0 runner    (1001) docker     (123)     6892 2023-08-08 14:54:57.000000 qiskit-dynamics-0.4.2/qiskit_dynamics/array/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10887 2023-08-08 14:54:57.000000 qiskit-dynamics-0.4.2/qiskit_dynamics/array/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-08-08 14:54:57.000000 qiskit-dynamics-0.4.2/qiskit_dynamics/array/patch_qi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7035 2023-08-08 14:54:57.000000 qiskit-dynamics-0.4.2/qiskit_dynamics/array/wrap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:55:08.025363 qiskit-dynamics-0.4.2/qiskit_dynamics/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-08-08 14:54:57.000000 qiskit-dynamics-0.4.2/qiskit_dynamics/backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:55:08.025363 qiskit-dynamics-0.4.2/qiskit_dynamics/backend/backend_string_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-08-08 14:54:57.000000 qiskit-dynamics-0.4.2/qiskit_dynamics/backend/backend_string_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12558 2023-08-08 14:54:57.000000 qiskit-dynamics-0.4.2/qiskit_dynamics/backend/backend_string_parser/hamiltonian_string_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4891 2023-08-08 14:54:57.000000 qiskit-dynamics-0.4.2/qiskit_dynamics/backend/backend_string_parser/operator_from_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14066 2023-08-08 14:54:57.000000 qiskit-dynamics-0.4.2/qiskit_dynamics/backend/backend_string_parser/regex_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10095 2023-08-08 14:54:57.000000 qiskit-dynamics-0.4.2/qiskit_dynamics/backend/backend_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45208 2023-08-08 14:54:57.000000 qiskit-dynamics-0.4.2/qiskit_dynamics/backend/dynamics_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-08-08 14:54:57.000000 qiskit-dynamics-0.4.2/qiskit_dynamics/backend/dynamics_job.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:55:08.025363 qiskit-dynamics-0.4.2/qiskit_dynamics/dispatch/
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-08-08 14:54:57.000000 qiskit-dynamics-0.4.2/qiskit_dynamics/dispatch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:55:08.025363 qiskit-dynamics-0.4.2/qiskit_dynamics/dispatch/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-08-08 14:54:57.000000 qiskit-dynamics-0.4.2/qiskit_dynamics/dispatch/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-08-08 14:54:57.000000 qiskit-dynamics-0.4.2/qiskit_dynamics/dispatch/backends/jax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-08-08 14:54:57.000000 qiskit-dynamics-0.4.2/qiskit_dynamics/dispatch/backends/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11769 2023-08-08 14:54:57.000000 qiskit-dynamics-0.4.2/qiskit_dynamics/dispatch/dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-08-08 14:54:57.000000 qiskit-dynamics-0.4.2/qiskit_dynamics/dispatch/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:55:08.025363 qiskit-dynamics-0.4.2/qiskit_dynamics/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     5678 2023-08-08 14:54:57.000000 qiskit-dynamics-0.4.2/qiskit_dynamics/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21116 2023-08-08 14:54:57.000000 qiskit-dynamics-0.4.2/qiskit_dynamics/models/generator_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8531 2023-08-08 14:54:57.000000 qiskit-dynamics-0.4.2/qiskit_dynamics/models/hamiltonian_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29123 2023-08-08 14:54:57.000000 qiskit-dynamics-0.4.2/qiskit_dynamics/models/lindblad_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62696 2023-08-08 14:54:57.000000 qiskit-dynamics-0.4.2/qiskit_dynamics/models/operator_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26059 2023-08-08 14:54:57.000000 qiskit-dynamics-0.4.2/qiskit_dynamics/models/rotating_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12484 2023-08-08 14:54:57.000000 qiskit-dynamics-0.4.2/qiskit_dynamics/models/rotating_wave_approximation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:55:08.025363 qiskit-dynamics-0.4.2/qiskit_dynamics/perturbation/
+-rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-08-08 14:54:57.000000 qiskit-dynamics-0.4.2/qiskit_dynamics/perturbation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33060 2023-08-08 14:54:57.000000 qiskit-dynamics-0.4.2/qiskit_dynamics/perturbation/array_polynomial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12155 2023-08-08 14:54:57.000000 qiskit-dynamics-0.4.2/qiskit_dynamics/perturbation/custom_binary_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30869 2023-08-08 14:54:57.000000 qiskit-dynamics-0.4.2/qiskit_dynamics/perturbation/dyson_magnus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7322 2023-08-08 14:54:57.000000 qiskit-dynamics-0.4.2/qiskit_dynamics/perturbation/multiset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-08-08 14:54:57.000000 qiskit-dynamics-0.4.2/qiskit_dynamics/perturbation/perturbation_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-08-08 14:54:57.000000 qiskit-dynamics-0.4.2/qiskit_dynamics/perturbation/perturbation_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15298 2023-08-08 14:54:57.000000 qiskit-dynamics-0.4.2/qiskit_dynamics/perturbation/solve_lmde_perturbation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:55:08.025363 qiskit-dynamics-0.4.2/qiskit_dynamics/pulse/
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-08-08 14:54:57.000000 qiskit-dynamics-0.4.2/qiskit_dynamics/pulse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16414 2023-08-08 14:54:57.000000 qiskit-dynamics-0.4.2/qiskit_dynamics/pulse/pulse_to_signals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:55:08.025363 qiskit-dynamics-0.4.2/qiskit_dynamics/signals/
+-rw-r--r--   0 runner    (1001) docker     (123)     8818 2023-08-08 14:54:57.000000 qiskit-dynamics-0.4.2/qiskit_dynamics/signals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40441 2023-08-08 14:54:57.000000 qiskit-dynamics-0.4.2/qiskit_dynamics/signals/signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7425 2023-08-08 14:54:57.000000 qiskit-dynamics-0.4.2/qiskit_dynamics/signals/transfer_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:55:08.029363 qiskit-dynamics-0.4.2/qiskit_dynamics/solvers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-08-08 14:54:57.000000 qiskit-dynamics-0.4.2/qiskit_dynamics/solvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-08-08 14:54:57.000000 qiskit-dynamics-0.4.2/qiskit_dynamics/solvers/diffrax_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21554 2023-08-08 14:54:57.000000 qiskit-dynamics-0.4.2/qiskit_dynamics/solvers/fixed_step_solvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-08-08 14:54:57.000000 qiskit-dynamics-0.4.2/qiskit_dynamics/solvers/jax_odeint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-08-08 14:54:57.000000 qiskit-dynamics-0.4.2/qiskit_dynamics/solvers/lanczos.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:55:08.029363 qiskit-dynamics-0.4.2/qiskit_dynamics/solvers/perturbative_solvers/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-08-08 14:54:57.000000 qiskit-dynamics-0.4.2/qiskit_dynamics/solvers/perturbative_solvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9185 2023-08-08 14:54:57.000000 qiskit-dynamics-0.4.2/qiskit_dynamics/solvers/perturbative_solvers/dyson_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20128 2023-08-08 14:54:57.000000 qiskit-dynamics-0.4.2/qiskit_dynamics/solvers/perturbative_solvers/expansion_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-08-08 14:54:57.000000 qiskit-dynamics-0.4.2/qiskit_dynamics/solvers/perturbative_solvers/magnus_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7094 2023-08-08 14:54:57.000000 qiskit-dynamics-0.4.2/qiskit_dynamics/solvers/perturbative_solvers/perturbative_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-08-08 14:54:57.000000 qiskit-dynamics-0.4.2/qiskit_dynamics/solvers/scipy_solve_ivp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38811 2023-08-08 14:54:57.000000 qiskit-dynamics-0.4.2/qiskit_dynamics/solvers/solver_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18579 2023-08-08 14:54:57.000000 qiskit-dynamics-0.4.2/qiskit_dynamics/solvers/solver_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10587 2023-08-08 14:54:57.000000 qiskit-dynamics-0.4.2/qiskit_dynamics/solvers/solver_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16654 2023-08-08 14:54:57.000000 qiskit-dynamics-0.4.2/qiskit_dynamics/type_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-08-08 14:54:57.000000 qiskit-dynamics-0.4.2/qiskit_dynamics/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:55:08.025363 qiskit-dynamics-0.4.2/qiskit_dynamics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5031 2023-08-08 14:55:07.000000 qiskit-dynamics-0.4.2/qiskit_dynamics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-08-08 14:55:07.000000 qiskit-dynamics-0.4.2/qiskit_dynamics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 14:55:07.000000 qiskit-dynamics-0.4.2/qiskit_dynamics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 14:55:07.000000 qiskit-dynamics-0.4.2/qiskit_dynamics.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-08-08 14:55:07.000000 qiskit-dynamics-0.4.2/qiskit_dynamics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-08 14:55:07.000000 qiskit-dynamics-0.4.2/qiskit_dynamics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 14:55:08.029363 qiskit-dynamics-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-08-08 14:54:57.000000 qiskit-dynamics-0.4.2/setup.py
```

### Comparing `qiskit-dynamics-0.4.1/LICENSE.txt` & `qiskit-dynamics-0.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.1/PKG-INFO` & `qiskit-dynamics-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit-dynamics
-Version: 0.4.1
+Version: 0.4.2
 Summary: Qiskit ODE solver
 Home-page: https://github.com/Qiskit-Extensions/qiskit-dynamics
 Author: Qiskit Development Team
 Author-email: qiskit@qiskit.org
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/Qiskit-Extensions/qiskit-dynamics/issues
 Project-URL: Source Code, https://github.com/Qiskit-Extensions/qiskit-dynamics
```

### Comparing `qiskit-dynamics-0.4.1/README.md` & `qiskit-dynamics-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.1/qiskit_dynamics/__init__.py` & `qiskit-dynamics-0.4.2/qiskit_dynamics/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.1/qiskit_dynamics/array/__init__.py` & `qiskit-dynamics-0.4.2/qiskit_dynamics/array/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.1/qiskit_dynamics/array/array.py` & `qiskit-dynamics-0.4.2/qiskit_dynamics/array/array.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.1/qiskit_dynamics/array/patch_qi.py` & `qiskit-dynamics-0.4.2/qiskit_dynamics/array/patch_qi.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.1/qiskit_dynamics/array/wrap.py` & `qiskit-dynamics-0.4.2/qiskit_dynamics/array/wrap.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.1/qiskit_dynamics/backend/__init__.py` & `qiskit-dynamics-0.4.2/qiskit_dynamics/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.1/qiskit_dynamics/backend/backend_string_parser/__init__.py` & `qiskit-dynamics-0.4.2/qiskit_dynamics/backend/backend_string_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.1/qiskit_dynamics/backend/backend_string_parser/hamiltonian_string_parser.py` & `qiskit-dynamics-0.4.2/qiskit_dynamics/backend/backend_string_parser/hamiltonian_string_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,20 +159,20 @@
     else:
         # if user supplied, make a copy and sort it
         subsystem_list = sorted(subsystem_list)
 
     # force keys in hamiltonian['qub'] to be ints
     qub_dict = {int(key): val for key, val in hamiltonian_dict["qub"].items()}
 
-    subsystem_dims = {int(qubit): qub_dict[int(qubit)] for qubit in subsystem_list}
+    subsystem_dims_dict = {int(qubit): qub_dict[int(qubit)] for qubit in subsystem_list}
 
     # Parse the Hamiltonian
     system = _regex_parser(
         operator_str=hamiltonian_dict["h_str"],
-        subsystem_dims=subsystem_dims,
+        subsystem_dims_dict=subsystem_dims_dict,
         subsystem_list=subsystem_list,
     )
 
     # Extract which channels are associated with which Hamiltonian terms.
     # Assumes one channel appearing in each term appearing at the end.
     channels = []
     for _, ham_str in system:
@@ -223,15 +223,20 @@
 
     # sort channels/operators according to channel ordering
     if len(reduced_channels) > 0:
         reduced_channels, hamiltonian_operators = zip(
             *sorted(zip(reduced_channels, hamiltonian_operators))
         )
 
-    return static_hamiltonian, list(hamiltonian_operators), list(reduced_channels), subsystem_dims
+    return (
+        static_hamiltonian,
+        list(hamiltonian_operators),
+        list(reduced_channels),
+        subsystem_dims_dict,
+    )
 
 
 def _hamiltonian_pre_parse_exceptions(hamiltonian_dict: dict):
     """Raises exceptions for improperly formatted or unsupported elements of
     hamiltonian dict specification.
 
     Parameters:
```

### Comparing `qiskit-dynamics-0.4.1/qiskit_dynamics/backend/backend_string_parser/operator_from_string.py` & `qiskit-dynamics-0.4.2/qiskit_dynamics/backend/backend_string_parser/operator_from_string.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,22 +22,22 @@
 import numpy as np
 
 from qiskit import QiskitError
 import qiskit.quantum_info as qi
 
 
 def _operator_from_string(
-    op_label: str, subsystem_label: int, subsystem_dims: Dict[int, int]
+    op_label: str, subsystem_label: int, subsystem_dims_dict: Dict[int, int]
 ) -> np.ndarray:
     r"""Generates a dense operator acting on a single subsystem, tensoring
     identities for remaining subsystems.
 
     The single system operator is specified via a string in ``op_label``,
     the list of subsystems and their corresponding dimensions are specified in the
-    dictionary ``subsystem_dims``, with system label being the keys specified as ``int``s,
+    dictionary ``subsystem_dims_dict``, with system label being the keys specified as ``int``s,
     and system dimensions the values also specified as ``int``s, and ``subsystem_label``
     indicates which subsystem the operator specified by ``op_label`` acts on.
 
     Accepted ``op_labels`` are:
         - `'X'`: If the target subsystem is two dimensional, the
           Pauli :math:`X` operator, and if greater than two dimensional, returns
           :math:`a + a^\dagger`, where :math:`a` and :math:`a^\dagger` are the
@@ -57,34 +57,34 @@
         - `'I'`: The identity operator.
 
     Note that the ordering of tensor factors is reversed.
 
     Args:
         op_label: The string labelling the single system operator.
         subsystem_label: Index of the subsystem to apply the operator.
-        subsystem_dims: Dictionary of subsystem labels and dimensions.
+        subsystem_dims_dict: Dictionary of subsystem labels and dimensions.
 
     Returns:
         np.ndarray corresponding to the specified operator.
 
     Raises:
         QiskitError: If op_label is invalid.
     """
 
     # construct single system operator
     op_func = __operdict.get(op_label, None)
     if op_func is None:
         raise QiskitError(f"String {op_label} does not correspond to a known operator.")
 
-    dim = subsystem_dims[subsystem_label]
+    dim = subsystem_dims_dict[subsystem_label]
     out = qi.Operator(op_func(dim), input_dims=[dim], output_dims=[dim])
 
     # sort subsystem labels and dimensions according to subsystem label
     sorted_subsystem_keys, sorted_subsystem_dims = zip(
-        *sorted(zip(subsystem_dims.keys(), subsystem_dims.values()))
+        *sorted(zip(subsystem_dims_dict.keys(), subsystem_dims_dict.values()))
     )
 
     # get subsystem location in ordered list
     subsystem_location = sorted_subsystem_keys.index(subsystem_label)
 
     # construct full operator
     return qi.ScalarOp(sorted_subsystem_dims).compose(out, [subsystem_location]).data
```

### Comparing `qiskit-dynamics-0.4.1/qiskit_dynamics/backend/backend_string_parser/regex_parser.py` & `qiskit-dynamics-0.4.2/qiskit_dynamics/backend/backend_string_parser/regex_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,28 +25,28 @@
 
 import numpy as np
 
 from .operator_from_string import _operator_from_string
 
 
 def _regex_parser(
-    operator_str: List[str], subsystem_dims: Dict[int, int], subsystem_list: List[int]
+    operator_str: List[str], subsystem_dims_dict: Dict[int, int], subsystem_list: List[int]
 ) -> List[Tuple[np.array, str]]:
     """Function wrapper for regex parsing object.
 
     Args:
         operator_str: List of strings in accepted format as described in
                       string_model_parser.parse_hamiltonian_dict.
-        subsystem_dims: Dictionary mapping subsystem labels to dimensions.
+        subsystem_dims_dict: Dictionary mapping subsystem labels to dimensions.
         subsystem_list: List of subsystems on which the operators are to be constructed.
     Returns:
         List of tuples containing pairs operators and their string coefficients.
     """
 
-    return _HamiltonianParser(h_str=operator_str, subsystem_dims=subsystem_dims).parse(
+    return _HamiltonianParser(h_str=operator_str, subsystem_dims_dict=subsystem_dims_dict).parse(
         subsystem_list
     )
 
 
 class _HamiltonianParser:
     """Legacy object for parsing string specifications of Hamiltonians."""
 
@@ -62,23 +62,25 @@
         Num=re.compile(r"[0-9.]+"),
         MathOrd0=re.compile(r"[*/]"),
         MathOrd1=re.compile(r"[+-]"),
         BrkL=re.compile(r"\("),
         BrkR=re.compile(r"\)"),
     )
 
-    def __init__(self, h_str, subsystem_dims):
+    def __init__(self, h_str, subsystem_dims_dict):
         """Create new quantum operator generator
 
         Parameters:
             h_str (list): list of Hamiltonian string
-            subsystem_dims (dict): dimension of subsystems
+            subsystem_dims_dict (dict): dimension of subsystems
         """
         self.h_str = h_str
-        self.subsystem_dims = {int(label): int(dim) for label, dim in subsystem_dims.items()}
+        self.subsystem_dims_dict = {
+            int(label): int(dim) for label, dim in subsystem_dims_dict.items()
+        }
         self.str2qopr = {}
 
     def parse(self, qubit_list=None):
         """Parse and generate Hamiltonian terms."""
         td_hams = []
         tc_hams = []
 
@@ -190,23 +192,23 @@
                         _key = key
                         _name = p.group()
                         if p.group() not in self.str2qopr:
                             idx = int(p.group("idx"))
                             if qubit_list is not None and idx not in qubit_list:
                                 return 0, None
                             name = p.group("opr")
-                            opr = _operator_from_string(name, idx, self.subsystem_dims)
+                            opr = _operator_from_string(name, idx, self.subsystem_dims_dict)
                             self.str2qopr[p.group()] = opr
                     elif key == "PrjOpr":
                         _key = key
                         _name = p.group()
                         if p.group() not in self.str2qopr:
                             idx = int(p.group("idx"))
                             name = "P"
-                            opr = _operator_from_string(name, idx, self.subsystem_dims)
+                            opr = _operator_from_string(name, idx, self.subsystem_dims_dict)
                             self.str2qopr[p.group()] = opr
                     elif key in ["Func", "Ext"]:
                         _name = p.group("name")
                         _key = key
                     elif key == "MathOrd1":
                         _name = p.group()
                         if prev not in ["QubOpr", "PrjOpr", "CavOpr", "Var", "Num"]:
```

### Comparing `qiskit-dynamics-0.4.1/qiskit_dynamics/backend/backend_utils.py` & `qiskit-dynamics-0.4.2/qiskit_dynamics/backend/backend_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -142,29 +142,39 @@
         else:
             memory_slot_probs[memory_slot_result] = prob
 
     return memory_slot_probs
 
 
 def _sample_probability_dict(
-    probability_dict: Dict, shots: int, seed: Optional[int] = None
+    probability_dict: Dict,
+    shots: int,
+    normalize_probabilities: bool = True,
+    seed: Optional[int] = None,
 ) -> List[str]:
     """Sample outcomes based on probability dictionary.
 
     Args:
         probability_dict: Dictionary representing probability distribution, with keys being
             outcomes, values being probabilities.
         shots: Number of shots.
+        normalize_probabilities: Whether or not to normalize the probabilities to sum to 1 before
+            sampling.
         seed: Seed to use in rng construction.
 
     Return:
         List: of entries of probability_dict, sampled according to the probabilities.
     """
     rng = np.random.default_rng(seed=seed)
     alphabet, probs = zip(*probability_dict.items())
+
+    if normalize_probabilities:
+        probs = np.array(probs)
+        probs = probs / probs.sum()
+
     return rng.choice(alphabet, size=shots, replace=True, p=probs)
 
 
 def _get_counts_from_samples(samples: list) -> Dict:
     """Count items in list."""
     return dict(zip(*np.unique(samples, return_counts=True)))
```

### Comparing `qiskit-dynamics-0.4.1/qiskit_dynamics/backend/dynamics_backend.py` & `qiskit-dynamics-0.4.2/qiskit_dynamics/backend/dynamics_backend.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 """
 Pulse-enabled simulator backend.
 """
 
 import datetime
 import uuid
+import warnings
 
 from typing import List, Optional, Union, Dict, Tuple
 import copy
 import numpy as np
 from scipy.integrate._ivp.ivp import OdeResult  # pylint: disable=unused-import
 
 from qiskit import pulse
@@ -105,26 +106,24 @@
 
     * ``shots``: Number of shots per experiment. Defaults to ``1024``.
     * ``solver``: The Qiskit Dynamics :class:`.Solver` instance used for simulation.
     * ``solver_options``: Dictionary containing optional kwargs for passing to :meth:`Solver.solve`,
       indicating solver methods and options. Defaults to the empty dictionary ``{}``.
     * ``subsystem_dims``: Dimensions of subsystems making up the system in ``solver``. Defaults to
       ``[solver.model.dim]``.
-    * ``subsystem_labels``: Integer labels for subsystems. Defaults to ``[0, ...,
-      len(subsystem_dims) - 1]``.
-    * ``meas_map``: Measurement map. Defaults to ``[[idx] for idx in subsystem_labels]``.
+    * ``meas_map``: Measurement map. Defaults to ``[[idx] for idx in range(len(subsystem_dims))]``.
     * ``control_channel_map``: A dictionary mapping control channel labels to indices, to be used
       for control channel index lookup in the :meth:`DynamicsBackend.control_channel` method.
     * ``initial_state``: Initial state for simulation, either the string ``"ground_state"``,
       indicating that the ground state for the system Hamiltonian should be used, or an arbitrary
       ``Statevector`` or ``DensityMatrix``. Defaults to ``"ground_state"``.
     * ``normalize_states``: Boolean indicating whether to normalize states before computing outcome
-      probabilities. Defaults to ``True``. Setting to ``False`` can result in errors if the solution
-      tolerance results in probabilities with significant numerical deviation from a proper
-      probability distribution.
+      probabilities, and normalize probablities before sampling. Defaults to ``True``. Setting to
+      ``False`` can result in errors if the solution tolerance results in probabilities with
+      significant numerical deviation from a proper probability distribution.
     * ``meas_level``: Form of measurement output. Supported values are ``1`` and ``2``. ``1``
       returns IQ points and ``2`` returns counts. Defaults to ``meas_level == 2``.
     * ``meas_return``: Level of measurement data to return. For ``meas_level = 1`` ``"single"``
       returns output from every shot. ``"avg"`` returns average over shots of measurement output.
       Defaults to ``"avg"``.
     * ``iq_centers``: Centers for IQ distribution when using ``meas_level==1`` results. Must have
       type ``List[List[List[float, float]]]`` formatted as ``iq_centers[subsystem][level] = [I,
@@ -183,54 +182,50 @@
         # add subsystem_dims to options so set_options validation works
         if "subsystem_dims" not in options:
             options["subsystem_dims"] = [solver.model.dim]
 
         # Set simulator options
         self.set_options(solver=solver, **options)
 
-        if self.options.subsystem_labels is None:
-            labels = list(range(len(self.options.subsystem_dims)))
-            self.set_options(subsystem_labels=labels)
-
         if self.options.meas_map is None:
-            meas_map = [[idx] for idx in self.options.subsystem_labels]
+            meas_map = [[idx] for idx in range(len(self.options.subsystem_dims))]
             self.set_options(meas_map=meas_map)
 
         # self._target = target or Target() doesn't work as bool(target) can be False
         if target is None:
             target = Target()
         else:
             target = copy.copy(target)
 
         # add default simulator measure instructions
         measure_properties = {}
         instruction_schedule_map = target.instruction_schedule_map()
-        for qubit in self.options.subsystem_labels:
+        for qubit in range(len(self.options.subsystem_dims)):
             if not instruction_schedule_map.has(instruction="measure", qubits=qubit):
                 with pulse.build() as meas_sched:
                     pulse.acquire(
                         duration=1, qubit_or_channel=qubit, register=pulse.MemorySlot(qubit)
                     )
 
                 measure_properties[(qubit,)] = InstructionProperties(calibration=meas_sched)
 
         if bool(measure_properties):
             target.add_instruction(Measure(), measure_properties)
 
         target.dt = solver._dt
+        target.num_qubits = len(self.options.subsystem_dims)
 
         self._target = target
 
     def _default_options(self):
         return Options(
             shots=1024,
             solver=None,
             solver_options={},
             subsystem_dims=None,
-            subsystem_labels=None,
             meas_map=None,
             control_channel_map=None,
             normalize_states=True,
             initial_state="ground_state",
             meas_level=MeasLevel.CLASSIFIED,
             meas_return=MeasReturnType.AVERAGE,
             iq_centers=None,
@@ -379,15 +374,15 @@
 
         # get the acquires sample times and subsystem measurement information
         (
             t_span,
             measurement_subsystems_list,
             memory_slot_indices_list,
         ) = _get_acquire_instruction_timings(
-            schedules, backend.options.subsystem_labels, backend.options.solver._dt
+            schedules, backend.options.subsystem_dims, backend.options.solver._dt
         )
 
         # Build and submit job
         job_id = str(uuid.uuid4())
         dynamics_job = DynamicsJob(
             backend=backend,
             job_id=job_id,
@@ -480,20 +475,18 @@
     def meas_map(self) -> List[List[int]]:
         return self.options.meas_map
 
     def _get_qubit_channel(
         self, qubit: int, ChannelClass: pulse.channels.Channel, method_name: str
     ):
         """Construct a channel instance for a given qubit."""
-        if qubit in self.options.subsystem_labels:
+        if qubit < len(self.options.subsystem_dims):
             return ChannelClass(qubit)
 
-        raise QiskitError(
-            f"{method_name} requested for qubit {qubit} which is not in subsystem_list."
-        )
+        raise QiskitError(f"{method_name} requested for qubit {qubit}, which is out of bounds.")
 
     def drive_channel(self, qubit: int) -> pulse.DriveChannel:
         """Return the drive channel for a given qubit."""
         return self._get_qubit_channel(qubit, pulse.DriveChannel, "drive_channel")
 
     def measure_channel(self, qubit: int) -> pulse.MeasureChannel:
         """Return the measure channel for a given qubit."""
@@ -540,15 +533,15 @@
     def defaults(self) -> PulseDefaults:
         """Get the backend defaults."""
         return self.options.defaults
 
     @classmethod
     def from_backend(
         cls,
-        backend: Union[BackendV1, BackendV2],
+        backend: BackendV1,
         subsystem_list: Optional[List[int]] = None,
         rotating_frame: Optional[Union[Array, RotatingFrame, str]] = "auto",
         evaluation_mode: str = "dense",
         rwa_cutoff_freq: Optional[float] = None,
         **options,
     ) -> "DynamicsBackend":
         """Construct a DynamicsBackend instance from an existing Backend instance.
@@ -612,14 +605,19 @@
           ``static_hamiltonian``.
 
         Otherwise the ``rotating_frame``, ``evaluation_mode``, and ``rwa_cutoff_freq`` are passed
         directly to the :class:`.Solver` initialization.
 
         Args:
             backend: The ``Backend`` instance to build the :class:`.DynamicsBackend` from.
+                Note that while the type hint indicates that `backend` should be a
+                :class:`~qiskit.providers.backend.BackendV1` instance, this method also works for
+                :class:`~qiskit.providers.backend.BackendV2` instances that have been set up with
+                sufficiently populated ``configuration`` and ``defaults`` for backwards
+                compatibility.
             subsystem_list: The list of qubits in the backend to include in the model.
             rotating_frame: Rotating frame argument for the internal :class:`.Solver`. Defaults to
                 ``"auto"``, allowing this method to pick a rotating frame.
             evaluation_mode: Evaluation mode argument for the internal :class:`.Solver`.
             rwa_cutoff_freq: Rotating wave approximation argument for the internal :class:`.Solver`.
             **options: Additional options to be applied in construction of the
                 :class:`.DynamicsBackend`.
@@ -667,17 +665,17 @@
                 "hamiltonian."
             )
 
         (
             static_hamiltonian,
             hamiltonian_operators,
             hamiltonian_channels,
-            subsystem_dims,
+            subsystem_dims_dict,
         ) = parse_backend_hamiltonian_dict(backend_config.hamiltonian, subsystem_list)
-        subsystem_dims = [subsystem_dims[idx] for idx in subsystem_list]
+        subsystem_dims = [subsystem_dims_dict.get(idx, 1) for idx in range(backend_num_qubits)]
 
         # construct model frequencies dictionary from backend
         channel_freqs = _get_backend_channel_freqs(
             backend_target=backend_target,
             backend_config=backend_config,
             backend_defaults=backend_defaults,
             channels=hamiltonian_channels,
@@ -732,15 +730,14 @@
             evaluation_mode=evaluation_mode,
             rwa_cutoff_freq=rwa_cutoff_freq,
         )
 
         return cls(
             solver=solver,
             target=Target(dt=dt),
-            subsystem_labels=subsystem_list,
             subsystem_dims=subsystem_dims,
             **options,
         )
 
 
 def default_experiment_result_function(
     experiment_name: str,
@@ -800,30 +797,28 @@
         )
         yf = backend._dressed_states_adjoint @ yf @ backend._dressed_states
         yf = DensityMatrix(yf, dims=backend.options.subsystem_dims)
 
         if backend.options.normalize_states:
             yf = yf / np.diag(yf.data).sum()
 
-    # compute probabilities for measurement slot values
-    measurement_subsystems = [
-        backend.options.subsystem_labels.index(x) for x in measurement_subsystems
-    ]
-
     if backend.options.meas_level == MeasLevel.CLASSIFIED:
         memory_slot_probabilities = _get_memory_slot_probabilities(
             probability_dict=yf.probabilities_dict(qargs=measurement_subsystems),
             memory_slot_indices=memory_slot_indices,
             num_memory_slots=num_memory_slots,
             max_outcome_value=backend.options.max_outcome_level,
         )
 
         # sample
         memory_samples = _sample_probability_dict(
-            memory_slot_probabilities, shots=backend.options.shots, seed=seed
+            memory_slot_probabilities,
+            shots=backend.options.shots,
+            normalize_probabilities=backend.options.normalize_states,
+            seed=seed,
         )
         counts = _get_counts_from_samples(memory_samples)
 
         # construct results object
         exp_data = ExperimentResultData(
             counts=counts, memory=memory_samples if backend.options.memory else None
         )
@@ -885,25 +880,26 @@
         for x in run_input:
             _validate_run_input(x, accept_list=False)
     elif not isinstance(run_input, (QuantumCircuit, Schedule, ScheduleBlock)):
         raise QiskitError(f"Input type {type(run_input)} not supported by DynamicsBackend.run.")
 
 
 def _get_acquire_instruction_timings(
-    schedules: List[Schedule], valid_subsystem_labels: List[int], dt: float
+    schedules: List[Schedule], subsystem_dims: List[int], dt: float
 ) -> Tuple[List[List[float]], List[List[int]], List[List[int]]]:
     """Get the required data from the acquire commands in each schedule.
 
     Additionally validates that each schedule has Acquire instructions occurring at one time, at
-    least one memory slot is being listed, and all measured subsystems exist in
-    ``valid_subsystem_labels``.
+    least one memory slot is being listed, and all measured subsystem indices are less than
+    ``len(subsystem_dims)``. Additionally, a warning is raised if a 'trivial' subsystem is measured,
+    i.e. one with dimension 1.
 
     Args:
         schedules: A list of schedules.
-        valid_subsystem_labels: Valid acquire channel indices.
+        subsystem_dims: List of subsystem dimensions.
         dt: The sample size.
     Returns:
         A tuple of lists containing, for each schedule: the list of integration intervals required
         for each schedule (in absolute time, from 0.0 to the beginning of the acquire instructions),
         a list of the subsystems being measured, and a list of the memory slots indices in which to
         store the results of each subsystem measurement.
     Raises:
@@ -934,22 +930,24 @@
                 raise QiskitError("DynamicsBackend.run only supports measurements at one time.")
 
         # use dt to convert acquire start time from sample index to the integration interval
         t_span_list.append([0.0, dt * schedule_acquire_times[0]])
         measurement_subsystems = []
         memory_slot_indices = []
         for inst in schedule_acquires:
-            if inst.channel.index in valid_subsystem_labels:
-                measurement_subsystems.append(inst.channel.index)
-            else:
+            if not inst.channel.index < len(subsystem_dims):
                 raise QiskitError(
-                    f"Attempted to measure subsystem {inst.channel.index}, but it is not in "
-                    "subsystem_list."
+                    f"Attempted to measure out of bounds subsystem {inst.channel.index}."
                 )
 
+            if subsystem_dims[inst.channel.index] == 1:
+                warnings.warn(f"Measuring trivial subsystem {inst.channel.index} with dimension 1.")
+
+            measurement_subsystems.append(inst.channel.index)
+
             memory_slot_indices.append(inst.mem_slot.index)
 
         measurement_subsystems_list.append(measurement_subsystems)
         memory_slot_indices_list.append(memory_slot_indices)
 
     return t_span_list, measurement_subsystems_list, memory_slot_indices_list
 
@@ -968,15 +966,15 @@
     for sched in run_input:
         num_memslots.append(None)
         if isinstance(sched, ScheduleBlock):
             schedules.append(block_to_schedule(sched))
         elif isinstance(sched, Schedule):
             schedules.append(sched)
         elif isinstance(sched, QuantumCircuit):
-            num_memslots[-1] = sched.cregs[0].size
+            num_memslots[-1] = sum(creg.size for creg in sched.cregs)
             schedules.append(build_schedule(sched, backend, dt=backend.options.solver._dt))
         else:
             raise QiskitError(f"Type {type(sched)} cannot be converted to Schedule.")
     return schedules, num_memslots
 
 
 def _get_backend_channel_freqs(
```

### Comparing `qiskit-dynamics-0.4.1/qiskit_dynamics/backend/dynamics_job.py` & `qiskit-dynamics-0.4.2/qiskit_dynamics/backend/dynamics_job.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.1/qiskit_dynamics/dispatch/__init__.py` & `qiskit-dynamics-0.4.2/qiskit_dynamics/dispatch/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.1/qiskit_dynamics/dispatch/backends/__init__.py` & `qiskit-dynamics-0.4.2/qiskit_dynamics/dispatch/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.1/qiskit_dynamics/dispatch/backends/jax.py` & `qiskit-dynamics-0.4.2/qiskit_dynamics/dispatch/backends/jax.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,51 +13,51 @@
 """Register jax backend for Dispatch"""
 
 # pylint: disable=import-error
 
 
 try:
     import jax
-    from jax.interpreters.xla import DeviceArray
+    from jax import Array
     from jax.core import Tracer
-    from jax.interpreters.ad import JVPTracer
-    from jax.interpreters.partial_eval import JaxprTracer
 
-    JAX_TYPES = (DeviceArray, Tracer, JaxprTracer, JVPTracer)
+    # warning based on JAX version
+    from packaging import version
+    import warnings
 
-    try:
-        # This class was introduced in 0.4.0
-        from jax import Array
-
-        JAX_TYPES += (Array,)
-    except ImportError:
-        pass
-
-    try:
-        # This class is not in older versions of Jax
-        from jax.interpreters.partial_eval import DynamicJaxprTracer
-
-        JAX_TYPES += (DynamicJaxprTracer,)
-    except ImportError:
-        pass
+    if version.parse(jax.__version__) >= version.parse("0.4.4"):
+        import os
+
+        if (
+            version.parse(jax.__version__) > version.parse("0.4.6")
+            or os.environ.get("JAX_JIT_PJIT_API_MERGE", None) != "0"
+        ):
+            warnings.warn(
+                "The functionality in the perturbation module of Qiskit Dynamics requires a JAX "
+                "version <= 0.4.6, due to a bug in JAX versions > 0.4.6. For versions 0.4.4, "
+                "0.4.5, and 0.4.6, using the perturbation module functionality requires setting "
+                "os.environ['JAX_JIT_PJIT_API_MERGE'] = '0' before importing JAX or Dynamics."
+            )
+
+    JAX_TYPES = (Array, Tracer)
 
     from ..dispatch import Dispatch
     import numpy as np
     from .numpy import _numpy_repr
 
     __all__ = []
 
     # Custom handling of functions not in jax.numpy
     HANDLED_FUNCTIONS = {}
 
     @Dispatch.register_asarray("jax", JAX_TYPES)
     def _jax_asarray(array, dtype=None, order=None):
         """Wrapper for jax.numpy.asarray"""
         if (
-            isinstance(array, DeviceArray)
+            isinstance(array, JAX_TYPES)
             and order is None
             and (dtype is None or dtype == array.dtype)
         ):
             return array
         return jax.numpy.asarray(array, dtype=dtype, order=order)
 
     @Dispatch.register_repr("jax")
```

### Comparing `qiskit-dynamics-0.4.1/qiskit_dynamics/dispatch/backends/numpy.py` & `qiskit-dynamics-0.4.2/qiskit_dynamics/dispatch/backends/numpy.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.1/qiskit_dynamics/dispatch/dispatch.py` & `qiskit-dynamics-0.4.2/qiskit_dynamics/dispatch/dispatch.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.1/qiskit_dynamics/dispatch/exceptions.py` & `qiskit-dynamics-0.4.2/qiskit_dynamics/dispatch/exceptions.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.1/qiskit_dynamics/models/__init__.py` & `qiskit-dynamics-0.4.2/qiskit_dynamics/models/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.1/qiskit_dynamics/models/generator_model.py` & `qiskit-dynamics-0.4.2/qiskit_dynamics/models/generator_model.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.1/qiskit_dynamics/models/hamiltonian_model.py` & `qiskit-dynamics-0.4.2/qiskit_dynamics/models/hamiltonian_model.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.1/qiskit_dynamics/models/lindblad_model.py` & `qiskit-dynamics-0.4.2/qiskit_dynamics/models/lindblad_model.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.1/qiskit_dynamics/models/operator_collections.py` & `qiskit-dynamics-0.4.2/qiskit_dynamics/models/operator_collections.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.1/qiskit_dynamics/models/rotating_frame.py` & `qiskit-dynamics-0.4.2/qiskit_dynamics/models/rotating_frame.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.1/qiskit_dynamics/models/rotating_wave_approximation.py` & `qiskit-dynamics-0.4.2/qiskit_dynamics/models/rotating_wave_approximation.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.1/qiskit_dynamics/perturbation/__init__.py` & `qiskit-dynamics-0.4.2/qiskit_dynamics/perturbation/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.1/qiskit_dynamics/perturbation/array_polynomial.py` & `qiskit-dynamics-0.4.2/qiskit_dynamics/perturbation/array_polynomial.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.1/qiskit_dynamics/perturbation/custom_binary_op.py` & `qiskit-dynamics-0.4.2/qiskit_dynamics/perturbation/custom_binary_op.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.1/qiskit_dynamics/perturbation/dyson_magnus.py` & `qiskit-dynamics-0.4.2/qiskit_dynamics/perturbation/dyson_magnus.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.1/qiskit_dynamics/perturbation/multiset_utils.py` & `qiskit-dynamics-0.4.2/qiskit_dynamics/perturbation/multiset_utils.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.1/qiskit_dynamics/perturbation/perturbation_data.py` & `qiskit-dynamics-0.4.2/qiskit_dynamics/perturbation/perturbation_data.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.1/qiskit_dynamics/perturbation/perturbation_utils.py` & `qiskit-dynamics-0.4.2/qiskit_dynamics/perturbation/perturbation_utils.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.1/qiskit_dynamics/perturbation/solve_lmde_perturbation.py` & `qiskit-dynamics-0.4.2/qiskit_dynamics/perturbation/solve_lmde_perturbation.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.1/qiskit_dynamics/pulse/__init__.py` & `qiskit-dynamics-0.4.2/qiskit_dynamics/pulse/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.1/qiskit_dynamics/pulse/pulse_to_signals.py` & `qiskit-dynamics-0.4.2/qiskit_dynamics/pulse/pulse_to_signals.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 """
 Pulse schedule to Signals converter.
 """
 
 from typing import Callable, Dict, List, Optional
 import functools
+from warnings import warn
 
 import numpy as np
 import sympy as sym
 
 from qiskit.pulse import (
     Schedule,
     Play,
@@ -36,14 +37,20 @@
 from qiskit.pulse.exceptions import PulseError
 from qiskit.pulse.library import SymbolicPulse
 from qiskit import QiskitError
 
 from qiskit_dynamics.array import Array
 from qiskit_dynamics.signals import DiscreteSignal
 
+try:
+    import jax
+    import jax.numpy as jnp
+except ImportError:
+    pass
+
 
 class InstructionToSignals:
     """Converts pulse instructions to signals to be used in models.
 
     The :class:`InstructionsToSignals` class converts a pulse schedule to a list of signals that can
     be given to a model. This conversion is done by calling the :meth:`get_signals` method on a
     schedule. The converter applies to instances of :class:`~qiskit.pulse.Schedule`. Instances of
@@ -129,14 +136,17 @@
           ``ShiftFrequency`` instructions (up to the sampling rate :math:`dt`).
         * ``SetFrequency``, with a frequency value :math:`\mu` at time-step :math:`k`, updates
           :math:`\phi_a \mapsto \phi_a - (\mu - (\Delta\nu + \nu)) k dt` and
           :math:`\Delta\nu \mapsto \mu - \nu`, where :math:`\nu` is the analog carrier frequency.
           Similarly to ``ShiftFrequency``, the shift rule for :math:`\phi_a` is defined to maintain
           carrier wave continuity.
 
+        If, at any sample point :math:`k`, :math:`\Delta\nu(k)` is larger than the Nyquist sampling
+        rate given by ``dt``, a warning will be raised.
+
         Args:
             schedule: The schedule to represent in terms of signals. Instances of
                 :class:`~qiskit.pulse.ScheduleBlock` must first be converted to
                 :class:`~qiskit.pulse.Schedule` using the
                 :func:`~qiskit.pulse.transforms.block_to_schedule` function in Qiskit Pulse.
 
         Returns:
@@ -184,30 +194,32 @@
                     )
                 )
                 signals[chan].add_samples(start_sample, samples)
 
             if isinstance(inst, ShiftPhase):
                 phases[chan] += inst.phase
 
+            if isinstance(inst, SetPhase):
+                phases[chan] = inst.phase
+
             if isinstance(inst, ShiftFrequency):
                 frequency_shifts[chan] = frequency_shifts[chan] + Array(inst.frequency)
                 phase_accumulations[chan] = (
                     phase_accumulations[chan] - inst.frequency * start_sample * self._dt
                 )
-
-            if isinstance(inst, SetPhase):
-                phases[chan] = inst.phase
+                _nyquist_warn(frequency_shifts[chan], self._dt, chan)
 
             if isinstance(inst, SetFrequency):
                 phase_accumulations[chan] = phase_accumulations[chan] - (
                     (inst.frequency - (frequency_shifts[chan] + signals[chan].carrier_freq))
                     * start_sample
                     * self._dt
                 )
                 frequency_shifts[chan] = inst.frequency - signals[chan].carrier_freq
+                _nyquist_warn(frequency_shifts[chan], self._dt, chan)
 
         # ensure all signals have the same number of samples
         max_duration = 0
         for sig in signals.values():
             max_duration = max(max_duration, sig.duration)
 
         for sig in signals.values():
@@ -363,7 +375,21 @@
     params = []
     for param in sorted(expr.free_symbols, key=lambda s: s.name):
         if param.name == "t":
             params.insert(0, param)
             continue
         params.append(param)
     return sym.lambdify(params, expr, modules=backend)
+
+
+def _nyquist_warn(frequency_shift: Array, dt: float, channel: str):
+    """Raise a warning if the frequency shift is above the Nyquist frequency given by ``dt``."""
+
+    if (
+        Array(frequency_shift).backend != "jax" or not isinstance(jnp.array(0), jax.core.Tracer)
+    ) and np.abs(frequency_shift) > 0.5 / dt:
+        warn(
+            "Due to SetFrequency and ShiftFrequency instructions, the digital carrier frequency "
+            f"of channel {channel} is larger than the Nyquist frequency of the envelope sample "
+            "size dt. As shifts of the frequency from the analog frequency are handled digitally, "
+            "this will result in aliasing effects."
+        )
```

### Comparing `qiskit-dynamics-0.4.1/qiskit_dynamics/signals/__init__.py` & `qiskit-dynamics-0.4.2/qiskit_dynamics/signals/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.1/qiskit_dynamics/signals/signals.py` & `qiskit-dynamics-0.4.2/qiskit_dynamics/signals/signals.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,16 +92,20 @@
         self._is_constant = False
 
         if isinstance(envelope, (complex, float, int)):
             envelope = Array(complex(envelope))
 
         if isinstance(envelope, Array):
             # if envelope is constant and the carrier is zero, this is a constant signal
-            if carrier_freq == 0.0:
-                self._is_constant = True
+            try:
+                # try block is for catching JAX tracer errors
+                if carrier_freq == 0.0:
+                    self._is_constant = True
+            except Exception:  # pylint: disable=broad-except
+                pass
 
             if envelope.backend == "jax":
                 self._envelope = lambda t: envelope * jnp.ones_like(Array(t).data)
             else:
                 self._envelope = lambda t: envelope * np.ones_like(t)
         elif callable(envelope):
             if Array.default_backend() == "jax":
```

### Comparing `qiskit-dynamics-0.4.1/qiskit_dynamics/signals/transfer_functions.py` & `qiskit-dynamics-0.4.2/qiskit_dynamics/signals/transfer_functions.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.1/qiskit_dynamics/solvers/__init__.py` & `qiskit-dynamics-0.4.2/qiskit_dynamics/solvers/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.1/qiskit_dynamics/solvers/diffrax_solver.py` & `qiskit-dynamics-0.4.2/qiskit_dynamics/solvers/diffrax_solver.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.1/qiskit_dynamics/solvers/fixed_step_solvers.py` & `qiskit-dynamics-0.4.2/qiskit_dynamics/solvers/fixed_step_solvers.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.1/qiskit_dynamics/solvers/jax_odeint.py` & `qiskit-dynamics-0.4.2/qiskit_dynamics/solvers/jax_odeint.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.1/qiskit_dynamics/solvers/lanczos.py` & `qiskit-dynamics-0.4.2/qiskit_dynamics/solvers/lanczos.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.1/qiskit_dynamics/solvers/perturbative_solvers/__init__.py` & `qiskit-dynamics-0.4.2/qiskit_dynamics/solvers/perturbative_solvers/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.1/qiskit_dynamics/solvers/perturbative_solvers/dyson_solver.py` & `qiskit-dynamics-0.4.2/qiskit_dynamics/solvers/perturbative_solvers/dyson_solver.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.1/qiskit_dynamics/solvers/perturbative_solvers/expansion_model.py` & `qiskit-dynamics-0.4.2/qiskit_dynamics/solvers/perturbative_solvers/expansion_model.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.1/qiskit_dynamics/solvers/perturbative_solvers/magnus_solver.py` & `qiskit-dynamics-0.4.2/qiskit_dynamics/solvers/perturbative_solvers/magnus_solver.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.1/qiskit_dynamics/solvers/perturbative_solvers/perturbative_solver.py` & `qiskit-dynamics-0.4.2/qiskit_dynamics/solvers/perturbative_solvers/perturbative_solver.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.1/qiskit_dynamics/solvers/scipy_solve_ivp.py` & `qiskit-dynamics-0.4.2/qiskit_dynamics/solvers/scipy_solve_ivp.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.1/qiskit_dynamics/solvers/solver_classes.py` & `qiskit-dynamics-0.4.2/qiskit_dynamics/solvers/solver_classes.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.1/qiskit_dynamics/solvers/solver_functions.py` & `qiskit-dynamics-0.4.2/qiskit_dynamics/solvers/solver_functions.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.1/qiskit_dynamics/solvers/solver_utils.py` & `qiskit-dynamics-0.4.2/qiskit_dynamics/solvers/solver_utils.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.1/qiskit_dynamics/type_utils.py` & `qiskit-dynamics-0.4.2/qiskit_dynamics/type_utils.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.1/qiskit_dynamics/version.py` & `qiskit-dynamics-0.4.2/qiskit_dynamics/version.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.1/qiskit_dynamics.egg-info/PKG-INFO` & `qiskit-dynamics-0.4.2/qiskit_dynamics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit-dynamics
-Version: 0.4.1
+Version: 0.4.2
 Summary: Qiskit ODE solver
 Home-page: https://github.com/Qiskit-Extensions/qiskit-dynamics
 Author: Qiskit Development Team
 Author-email: qiskit@qiskit.org
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/Qiskit-Extensions/qiskit-dynamics/issues
 Project-URL: Source Code, https://github.com/Qiskit-Extensions/qiskit-dynamics
```

### Comparing `qiskit-dynamics-0.4.1/qiskit_dynamics.egg-info/SOURCES.txt` & `qiskit-dynamics-0.4.2/qiskit_dynamics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.1/setup.py` & `qiskit-dynamics-0.4.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,18 +17,19 @@
 
 requirements = [
     "numpy>=1.17",
     "scipy>=1.4",
     "matplotlib>=3.0",
     "qiskit-terra>=0.23.0",
     "multiset>=3.0.1",
+    "sympy>=1.12"
 ]
 
-jax_extras = ['jax>=0.2.26, <= 0.4.6',
-              'jaxlib>=0.1.75, <= 0.4.6']
+jax_extras = ['jax>=0.4.0, <= 0.4.6',
+              'jaxlib>=0.4.0, <= 0.4.6']
 
 PACKAGES = setuptools.find_packages(exclude=['test*'])
 
 version_path = os.path.abspath(
     os.path.join(os.path.dirname(__file__), 'qiskit_dynamics',
                  'VERSION.txt'))
```

