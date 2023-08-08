# Comparing `tmp/jax-moseq-0.0.3.tar.gz` & `tmp/jax-moseq-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jax-moseq-0.0.3.tar", last modified: Thu May  4 15:12:12 2023, max compression
+gzip compressed data, was "jax-moseq-0.0.5.tar", last modified: Tue Aug  8 13:51:04 2023, max compression
```

## Comparing `jax-moseq-0.0.3.tar` & `jax-moseq-0.0.5.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-05-04 15:12:12.870587 jax-moseq-0.0.3/
--rw-r--r--   0 calebweinreb   (501) staff       (20)     8384 2023-04-19 14:03:05.000000 jax-moseq-0.0.3/LICENSE.md
--rw-r--r--   0 calebweinreb   (501) staff       (20)      300 2023-05-04 15:12:12.870790 jax-moseq-0.0.3/PKG-INFO
--rw-r--r--   0 calebweinreb   (501) staff       (20)      615 2023-05-04 15:11:20.000000 jax-moseq-0.0.3/README.md
-drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-05-04 15:12:12.872514 jax-moseq-0.0.3/jax_moseq/
--rw-r--r--   0 calebweinreb   (501) staff       (20)      124 2023-05-04 15:11:20.000000 jax-moseq-0.0.3/jax_moseq/__init__.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)      497 2023-05-04 15:12:12.872650 jax-moseq-0.0.3/jax_moseq/_version.py
-drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-05-04 15:12:12.854637 jax-moseq-0.0.3/jax_moseq/models/
--rw-r--r--   0 calebweinreb   (501) staff       (20)       67 2023-04-19 14:03:05.000000 jax-moseq-0.0.3/jax_moseq/models/__init__.py
-drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-05-04 15:12:12.857861 jax-moseq-0.0.3/jax_moseq/models/arhmm/
--rw-r--r--   0 calebweinreb   (501) staff       (20)      182 2023-04-19 14:03:05.000000 jax-moseq-0.0.3/jax_moseq/models/arhmm/__init__.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)     6584 2023-04-19 14:03:05.000000 jax-moseq-0.0.3/jax_moseq/models/arhmm/generate.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)     6789 2023-05-04 15:11:20.000000 jax-moseq-0.0.3/jax_moseq/models/arhmm/gibbs.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)     8064 2023-04-19 14:03:05.000000 jax-moseq-0.0.3/jax_moseq/models/arhmm/initialize.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)     3422 2023-04-19 14:03:05.000000 jax-moseq-0.0.3/jax_moseq/models/arhmm/log_prob.py
-drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-05-04 15:12:12.861379 jax-moseq-0.0.3/jax_moseq/models/keypoint_slds/
--rw-r--r--   0 calebweinreb   (501) staff       (20)      215 2023-04-19 14:03:05.000000 jax-moseq-0.0.3/jax_moseq/models/keypoint_slds/__init__.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    13504 2023-04-19 14:03:05.000000 jax-moseq-0.0.3/jax_moseq/models/keypoint_slds/alignment.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    11141 2023-05-04 15:11:20.000000 jax-moseq-0.0.3/jax_moseq/models/keypoint_slds/gibbs.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    14485 2023-04-30 19:00:54.000000 jax-moseq-0.0.3/jax_moseq/models/keypoint_slds/initialize.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)     4833 2023-04-19 14:03:05.000000 jax-moseq-0.0.3/jax_moseq/models/keypoint_slds/log_prob.py
-drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-05-04 15:12:12.864908 jax-moseq-0.0.3/jax_moseq/models/slds/
--rw-r--r--   0 calebweinreb   (501) staff       (20)      133 2023-04-19 14:03:05.000000 jax-moseq-0.0.3/jax_moseq/models/slds/__init__.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)     9811 2023-05-04 15:11:20.000000 jax-moseq-0.0.3/jax_moseq/models/slds/gibbs.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    10217 2023-04-19 14:03:05.000000 jax-moseq-0.0.3/jax_moseq/models/slds/initialize.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)     4081 2023-04-19 14:03:05.000000 jax-moseq-0.0.3/jax_moseq/models/slds/log_prob.py
-drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-05-04 15:12:12.870060 jax-moseq-0.0.3/jax_moseq/utils/
--rw-r--r--   0 calebweinreb   (501) staff       (20)       45 2023-05-04 15:11:20.000000 jax-moseq-0.0.3/jax_moseq/utils/__init__.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)     1148 2023-04-19 14:03:05.000000 jax-moseq-0.0.3/jax_moseq/utils/autoregression.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)     9385 2023-05-04 15:11:20.000000 jax-moseq-0.0.3/jax_moseq/utils/debugging.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)     2644 2023-05-04 15:11:20.000000 jax-moseq-0.0.3/jax_moseq/utils/distributions.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)     4343 2023-05-04 15:11:20.000000 jax-moseq-0.0.3/jax_moseq/utils/kalman.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    11715 2023-05-04 15:11:20.000000 jax-moseq-0.0.3/jax_moseq/utils/transitions.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)     6471 2023-05-04 15:11:20.000000 jax-moseq-0.0.3/jax_moseq/utils/utils.py
-drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-05-04 15:12:12.854139 jax-moseq-0.0.3/jax_moseq.egg-info/
--rw-r--r--   0 calebweinreb   (501) staff       (20)      300 2023-05-04 15:12:12.000000 jax-moseq-0.0.3/jax_moseq.egg-info/PKG-INFO
--rw-r--r--   0 calebweinreb   (501) staff       (20)     1020 2023-05-04 15:12:12.000000 jax-moseq-0.0.3/jax_moseq.egg-info/SOURCES.txt
--rw-r--r--   0 calebweinreb   (501) staff       (20)        1 2023-05-04 15:12:12.000000 jax-moseq-0.0.3/jax_moseq.egg-info/dependency_links.txt
--rw-r--r--   0 calebweinreb   (501) staff       (20)       38 2023-05-04 15:12:12.000000 jax-moseq-0.0.3/jax_moseq.egg-info/requires.txt
--rw-r--r--   0 calebweinreb   (501) staff       (20)       10 2023-05-04 15:12:12.000000 jax-moseq-0.0.3/jax_moseq.egg-info/top_level.txt
--rw-r--r--   0 calebweinreb   (501) staff       (20)      590 2023-05-04 15:12:12.872005 jax-moseq-0.0.3/setup.cfg
--rw-r--r--   0 calebweinreb   (501) staff       (20)      241 2023-05-04 15:11:20.000000 jax-moseq-0.0.3/setup.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    83607 2023-05-04 15:11:20.000000 jax-moseq-0.0.3/versioneer.py
+drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-08-08 13:51:04.973794 jax-moseq-0.0.5/
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     8384 2023-05-21 00:22:51.000000 jax-moseq-0.0.5/LICENSE.md
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      300 2023-08-08 13:51:04.973983 jax-moseq-0.0.5/PKG-INFO
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      615 2023-05-21 00:22:51.000000 jax-moseq-0.0.5/README.md
+drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-08-08 13:51:04.975365 jax-moseq-0.0.5/jax_moseq/
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      125 2023-08-07 01:51:38.000000 jax-moseq-0.0.5/jax_moseq/__init__.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      497 2023-08-08 13:51:04.975482 jax-moseq-0.0.5/jax_moseq/_version.py
+drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-08-08 13:51:04.895292 jax-moseq-0.0.5/jax_moseq/models/
+-rw-r--r--   0 calebweinreb   (501) staff       (20)       67 2023-05-24 21:31:08.000000 jax-moseq-0.0.5/jax_moseq/models/__init__.py
+drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-08-08 13:51:04.912699 jax-moseq-0.0.5/jax_moseq/models/arhmm/
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      183 2023-08-07 01:51:38.000000 jax-moseq-0.0.5/jax_moseq/models/arhmm/__init__.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     6612 2023-08-07 01:51:38.000000 jax-moseq-0.0.5/jax_moseq/models/arhmm/generate.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     6794 2023-08-07 01:51:38.000000 jax-moseq-0.0.5/jax_moseq/models/arhmm/gibbs.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     7853 2023-08-07 01:51:38.000000 jax-moseq-0.0.5/jax_moseq/models/arhmm/initialize.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     4376 2023-08-07 01:51:38.000000 jax-moseq-0.0.5/jax_moseq/models/arhmm/log_prob.py
+drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-08-08 13:51:04.935993 jax-moseq-0.0.5/jax_moseq/models/keypoint_slds/
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      216 2023-08-07 01:51:38.000000 jax-moseq-0.0.5/jax_moseq/models/keypoint_slds/__init__.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    13738 2023-08-07 01:51:38.000000 jax-moseq-0.0.5/jax_moseq/models/keypoint_slds/alignment.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    13227 2023-08-07 01:51:38.000000 jax-moseq-0.0.5/jax_moseq/models/keypoint_slds/gibbs.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    14363 2023-08-07 01:51:38.000000 jax-moseq-0.0.5/jax_moseq/models/keypoint_slds/initialize.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     4858 2023-08-07 01:51:38.000000 jax-moseq-0.0.5/jax_moseq/models/keypoint_slds/log_prob.py
+drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-08-08 13:51:04.960496 jax-moseq-0.0.5/jax_moseq/models/slds/
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      134 2023-08-07 01:51:38.000000 jax-moseq-0.0.5/jax_moseq/models/slds/__init__.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    12840 2023-08-07 01:51:38.000000 jax-moseq-0.0.5/jax_moseq/models/slds/gibbs.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     9780 2023-08-07 01:51:38.000000 jax-moseq-0.0.5/jax_moseq/models/slds/initialize.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     4066 2023-08-07 01:51:38.000000 jax-moseq-0.0.5/jax_moseq/models/slds/log_prob.py
+drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-08-08 13:51:04.973306 jax-moseq-0.0.5/jax_moseq/utils/
+-rw-r--r--   0 calebweinreb   (501) staff       (20)       46 2023-08-07 01:51:38.000000 jax-moseq-0.0.5/jax_moseq/utils/__init__.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     1133 2023-08-07 01:51:38.000000 jax-moseq-0.0.5/jax_moseq/utils/autoregression.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     9673 2023-08-07 01:51:38.000000 jax-moseq-0.0.5/jax_moseq/utils/debugging.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     2696 2023-08-07 01:51:38.000000 jax-moseq-0.0.5/jax_moseq/utils/distributions.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     6199 2023-08-07 01:51:38.000000 jax-moseq-0.0.5/jax_moseq/utils/kalman.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    13218 2023-08-07 01:51:38.000000 jax-moseq-0.0.5/jax_moseq/utils/transitions.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    15942 2023-08-08 13:50:56.000000 jax-moseq-0.0.5/jax_moseq/utils/utils.py
+drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-08-08 13:51:04.894758 jax-moseq-0.0.5/jax_moseq.egg-info/
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      300 2023-08-08 13:51:04.000000 jax-moseq-0.0.5/jax_moseq.egg-info/PKG-INFO
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     1020 2023-08-08 13:51:04.000000 jax-moseq-0.0.5/jax_moseq.egg-info/SOURCES.txt
+-rw-r--r--   0 calebweinreb   (501) staff       (20)        1 2023-08-08 13:51:04.000000 jax-moseq-0.0.5/jax_moseq.egg-info/dependency_links.txt
+-rw-r--r--   0 calebweinreb   (501) staff       (20)       95 2023-08-08 13:51:04.000000 jax-moseq-0.0.5/jax_moseq.egg-info/requires.txt
+-rw-r--r--   0 calebweinreb   (501) staff       (20)       10 2023-08-08 13:51:04.000000 jax-moseq-0.0.5/jax_moseq.egg-info/top_level.txt
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      649 2023-08-08 13:51:04.974933 jax-moseq-0.0.5/setup.cfg
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      242 2023-08-07 01:51:38.000000 jax-moseq-0.0.5/setup.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    84134 2023-08-07 01:51:38.000000 jax-moseq-0.0.5/versioneer.py
```

### Comparing `jax-moseq-0.0.3/LICENSE.md` & `jax-moseq-0.0.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `jax-moseq-0.0.3/README.md` & `jax-moseq-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `jax-moseq-0.0.3/jax_moseq/models/arhmm/generate.py` & `jax-moseq-0.0.5/jax_moseq/models/arhmm/generate.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import jax
 import jax.numpy as jnp
 import jax.random as jr
 from jax.scipy.linalg import cho_factor
 import numpy as np
+
 na = jnp.newaxis
 
 from jax_moseq.utils import pad_affine
 
+
 def steady_state_distribution(pi, pseudocount=1e-3):
     """
     Compute the steady state distribution of a Markov chain.
 
     Parameters
     ----------
     pi : jax array of shape (num_states, num_states)
@@ -18,23 +20,25 @@
     pseudocount : float, optional
         Pseudocount to add to the transition matrix to make it regular.
 
     Returns
     -------
     steady_state : jax array of shape (num_states,)
         Steady state distribution.
-    """    
+    """
     # make sure the matrix is regular and eigendecompose
-    pi = np.array(pi) # non-symmetric eigendecomposition only works on CPU
-    pi_regular = (pi + pseudocount)/(pi + pseudocount).sum(1)[:,None]
+    pi = np.array(pi)  # non-symmetric eigendecomposition only works on CPU
+    pi_regular = (pi + pseudocount) / (pi + pseudocount).sum(1)[:, None]
     eigenvals, eigenvects = np.linalg.eig(pi_regular.T)
 
     # extract the eigenvector corresponding to the eigenvalue with unit magnitude
     index = np.argmin(np.abs(jnp.abs(eigenvals) - 1))
-    steady_state = np.real(eigenvects[:, index]) / np.sum(np.real(eigenvects[:, index]))
+    steady_state = np.real(eigenvects[:, index]) / np.sum(
+        np.real(eigenvects[:, index])
+    )
     return jnp.array(steady_state)
 
 
 def generate_initial_state(seed, pi, Ab, Q):
     """
     Generate initial states for the ARHMM.
 
@@ -64,15 +68,15 @@
     """
     # sample initial discrete state
     pi0 = steady_state_distribution(pi)
     z = jr.choice(seed, jnp.arange(pi0.shape[0]), p=pi0)
 
     # sample initial latent trajectory
     latent_dim = Ab.shape[1]
-    nlags = (Ab.shape[2]-1) // latent_dim
+    nlags = (Ab.shape[2] - 1) // latent_dim
     xlags = jr.normal(seed, (nlags, latent_dim))
 
     # update the seed
     seed = jr.split(seed)[1]
     return z, xlags, seed
 
 
@@ -111,18 +115,19 @@
     x = jr.multivariate_normal(seed, mu, Q[z])
     xlags = jnp.concatenate([xlags[1:], x[na]], axis=0)
 
     # update the seed
     seed = jr.split(seed)[1]
     return z, xlags, seed
 
+
 def generate_next_state_fast(seed, z, xlags, Ab, L, pi, sigma):
     """
     Generate the next states of an ARHMM, using cholesky
-    factors and precomputed gaussian random variables to 
+    factors and precomputed gaussian random variables to
     speed up sampling.
 
     Parameters
     ----------
     seed : jax.random.PRNGKey
         Random seed.
     z : int
@@ -155,15 +160,14 @@
     xlags = jnp.concatenate([xlags[1:], x[na]], axis=0)
 
     # update the seed
     seed = jr.split(seed)[1]
     return z, xlags, seed
 
 
-
 def generate_states(seed, pi, Ab, Q, n_steps, init_state=None):
     """
     Generate a sequence of states from an ARHMM.
 
     Parameters
     ----------
     seed : jax.random.PRNGKey
@@ -185,23 +189,26 @@
         Discrete states.
     xs : jax array of shape (n_steps,latent_dim)
         Continuous states.
     """
     # initialize the states
     if init_state is None:
         z, xlags, seed = generate_initial_state(seed, pi, Ab, Q)
-    else: 
+    else:
         z, xlags = init_state
-        
+
     # precompute cholesky factors and random samples
     L = cho_factor(Q, lower=True)[0]
     sigmas = jr.normal(seed, (n_steps, Q.shape[-1]))
-    
+
     # generate the states using jax.lax.scan
     def _generate_next_state(carry, sigma):
         z, xlags, seed = carry
-        z, xlags, seed = generate_next_state_fast(seed, z, xlags, Ab, L, pi, sigma)
+        z, xlags, seed = generate_next_state_fast(
+            seed, z, xlags, Ab, L, pi, sigma
+        )
         return (z, xlags, seed), (z, xlags)
+
     carry = (z, xlags, seed)
     _, (zs, xs) = jax.lax.scan(_generate_next_state, carry, sigmas)
 
-    return zs, xs[:,-1]
+    return zs, xs[:, -1]
```

### Comparing `jax-moseq-0.0.3/jax_moseq/models/arhmm/gibbs.py` & `jax-moseq-0.0.5/jax_moseq/models/arhmm/gibbs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 import jax
 import jax.numpy as jnp
 import jax.random as jr
 
 from jax_moseq.utils import (
-    pad_affine, 
-    psd_solve, 
-    psd_inv, 
+    pad_affine,
+    psd_solve,
+    psd_inv,
     nan_check,
-    convert_data_precision
+    mixed_map,
 )
 
-from jax_moseq.utils.distributions import (
-    sample_mniw,
-    sample_hmm_stateseq
-)
+from jax_moseq.utils.distributions import sample_mniw, sample_hmm_stateseq
 from jax_moseq.utils.autoregression import (
     get_lags,
     get_nlags,
-    ar_log_likelihood
+    ar_log_likelihood,
 )
 from jax_moseq.utils.transitions import resample_hdp_transitions
 
 from functools import partial
+
 na = jnp.newaxis
 
 
 @jax.jit
 def resample_discrete_stateseqs(seed, x, mask, Ab, Q, pi, **kwargs):
     """
     Resamples the discrete state sequence ``z``.
@@ -52,25 +50,28 @@
     z : jax_array of shape (N, T - n_lags)
         Discrete state sequences.
     """
     nlags = get_nlags(Ab)
     num_samples = mask.shape[0]
 
     log_likelihoods = jax.lax.map(partial(ar_log_likelihood, x), (Ab, Q))
-    _, z = jax.vmap(sample_hmm_stateseq, in_axes=(0,na,0,0))(
+    _, z = mixed_map(sample_hmm_stateseq, in_axes=(0, na, 0, 0))(
         jr.split(seed, num_samples),
         pi,
-        jnp.moveaxis(log_likelihoods,0,-1),
-        mask.astype(float)[:,nlags:])
-    return convert_data_precision(z)
+        jnp.moveaxis(log_likelihoods, 0, -1),
+        mask.astype(float)[:, nlags:],
+    )
+    return z
+
 
 @nan_check
-@partial(jax.jit, static_argnames=('num_states','nlags'))
-def resample_ar_params(seed, *, nlags, num_states, mask, x, z,
-                       nu_0, S_0, M_0, K_0, **kwargs):
+@partial(jax.jit, static_argnames=("num_states", "nlags"))
+def resample_ar_params(
+    seed, *, nlags, num_states, mask, x, z, nu_0, S_0, M_0, K_0, **kwargs
+):
     """
     Resamples the AR parameters ``Ab`` and ``Q``.
 
     Parameters
     ----------
     seed : jr.PRNGKey
         JAX random seed.
@@ -100,22 +101,28 @@
     Ab : jax array of shape (num_states, latent_dim, ar_dim)
         Autoregressive transforms.
     Q : jax array of shape (num_states, latent_dim, latent_dim)
         Autoregressive noise covariances.
     """
     seeds = jr.split(seed, num_states)
 
-    masks = mask[..., nlags:].reshape(1,-1) * jnp.eye(num_states)[:, z.reshape(-1)]
+    masks = (
+        mask[..., nlags:].reshape(1, -1)
+        * jnp.eye(num_states)[:, z.reshape(-1)]
+    )
     x_in = pad_affine(get_lags(x, nlags)).reshape(-1, nlags * x.shape[-1] + 1)
     x_out = x[..., nlags:, :].reshape(-1, x.shape[-1])
-    
-    map_fun = partial(_resample_regression_params, x_in, x_out, nu_0, S_0, M_0, K_0)
+
+    map_fun = partial(
+        _resample_regression_params, x_in, x_out, nu_0, S_0, M_0, K_0
+    )
     Ab, Q = jax.lax.map(map_fun, (seeds, masks))
     return Ab, Q
 
+
 @nan_check
 @jax.jit
 def _resample_regression_params(x_in, x_out, nu_0, S_0, M_0, K_0, args):
     """
     Resamples regression parameters from a Matrix normal
     inverse-Wishart distribution.
 
@@ -142,31 +149,38 @@
     Ab : jax array of shape (num_states, out_dim, in_dim)
         Regression transforms.
     Q : jax array of shape (num_states, out_dim, out_dim)
         Regression noise covariances.
     """
     seed, mask = args
 
-    S_out_out = jnp.einsum('ti,tj,t->ij', x_out, x_out, mask)
-    S_out_in = jnp.einsum('ti,tj,t->ij', x_out, x_in, mask)
-    S_in_in = jnp.einsum('ti,tj,t->ij', x_in, x_in, mask)
-    
+    S_out_out = jnp.einsum("ti,tj,t->ij", x_out, x_out, mask)
+    S_out_in = jnp.einsum("ti,tj,t->ij", x_out, x_in, mask)
+    S_in_in = jnp.einsum("ti,tj,t->ij", x_in, x_in, mask)
+
     K_0_inv = psd_inv(K_0)
     K_n_inv = K_0_inv + S_in_in
 
     K_n = psd_inv(K_n_inv)
-    M_n = psd_solve(K_n_inv.T, K_0_inv @ M_0.T + S_out_in.T).T  
-     
+    M_n = psd_solve(K_n_inv.T, K_0_inv @ M_0.T + S_out_in.T).T
+
     S_n = S_0 + S_out_out + (M_0 @ K_0_inv @ M_0.T - M_n @ K_n_inv @ M_n.T)
     return sample_mniw(seed, nu_0 + mask.sum(), S_n, M_n, K_n)
 
 
-
-def resample_model(data, seed, states, params, hypparams,
-                   states_only=False, verbose=False, **kwargs):
+def resample_model(
+    data,
+    seed,
+    states,
+    params,
+    hypparams,
+    states_only=False,
+    verbose=False,
+    **kwargs
+):
     """
     Resamples the ARHMM model given the hyperparameters, data,
     current states, and current parameters.
 
     Parameters
     ----------
     data : dict
@@ -192,26 +206,30 @@
         Dictionary containing the hyperparameters and
         updated seed, states, and parameters of the model.
     """
     seed = jr.split(seed)[1]
     params = params.copy()
     states = states.copy()
 
-    if not states_only: 
-        if verbose: print('Resampling pi (transition matrix)')
-        params['betas'], params['pi'] = resample_hdp_transitions(
-            seed, **data, **states, **params, 
-            **hypparams['trans_hypparams'])
-
-        if verbose: print('Resampling Ab,Q (AR parameters)')
-        params['Ab'], params['Q']= resample_ar_params(
-            seed, **data, **states, **params, 
-            **hypparams['ar_hypparams'])
-
-    if verbose: print('Resampling z (discrete latent states)')
-    states['z'] = resample_discrete_stateseqs(
-        seed, **data, **states, **params)
-
-    return {'seed': seed,
-            'states': states, 
-            'params': params, 
-            'hypparams': hypparams}
+    if not states_only:
+        if verbose:
+            print("Resampling pi (transition matrix)")
+        params["betas"], params["pi"] = resample_hdp_transitions(
+            seed, **data, **states, **params, **hypparams["trans_hypparams"]
+        )
+
+        if verbose:
+            print("Resampling Ab,Q (AR parameters)")
+        params["Ab"], params["Q"] = resample_ar_params(
+            seed, **data, **states, **params, **hypparams["ar_hypparams"]
+        )
+
+    if verbose:
+        print("Resampling z (discrete latent states)")
+    states["z"] = resample_discrete_stateseqs(seed, **data, **states, **params)
+
+    return {
+        "seed": seed,
+        "states": states,
+        "params": params,
+        "hypparams": hypparams,
+    }
```

### Comparing `jax-moseq-0.0.3/jax_moseq/models/arhmm/initialize.py` & `jax-moseq-0.0.5/jax_moseq/models/arhmm/initialize.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 na = jnp.newaxis
 
 
 def init_ar_params(seed, *, num_states, nu_0, S_0, M_0, K_0, **kwargs):
     """
     Initialize the autoregression parameters by sampling from an
     MNIW distribution. Note below that ar_dim = latent_dim * num_lags + 1.
-    
+
     Parameters
     ----------
     seed : jr.PRNGKey
         JAX random seed.
     num_states : int
         Max number of HMM states.
     nu_0 : int
@@ -38,124 +38,124 @@
     Ab : jax array of shape (num_states, latent_dim, ar_dim)
         Autoregressive transforms.
     Q : jax array of shape (num_states, latent_dim, latent_dim)
         Autoregressive noise covariances.
     """
     seeds = jr.split(seed, num_states)
     in_axes = (0, na, na, na, na)
-    Ab, Q = jax.vmap(sample_mniw, in_axes)(
-        seeds, nu_0, S_0, M_0, K_0)
+    Ab, Q = jax.vmap(sample_mniw, in_axes)(seeds, nu_0, S_0, M_0, K_0)
     return Ab, Q
 
 
 def init_states(seed, x, mask, params, **kwargs):
     """
     Initialize the latent states of the ARHMM from the
     data and parameters.
-    
+
     Parameters
     ----------
     seed : jr.PRNGKey
         JAX random seed.
     x : jax array of shape (N, T, latent_dim)
         Latent trajectories.
     mask : jax array of shape (N, T)
         Binary indicator for valid frames.
     params : dict
-        Values for each model parameter. 
+        Values for each model parameter.
     **kwargs : dict
         Overflow, for convenience.
 
     Returns
     -------
     states : dict
         State values for each latent variable.
     """
     z = resample_discrete_stateseqs(seed, x, mask, **params)
-    return {'z': z}
+    return {"z": z}
 
 
 def init_params(seed, trans_hypparams, ar_hypparams, **kwargs):
     """
     Initialize the parameters of the ARHMM from the
     data and hyperparameters.
-    
+
     Parameters
     ----------
     seed : jr.PRNGKey
         JAX random seed.
     trans_hypparams : dict
         HDP transition hyperparameters.
     ar_hypparams : dict
         Autoregression hyperparameters.
     **kwargs : dict
         Overflow, for convenience.
-        
+
     Returns
     -------
     params : dict
         Values for each model parameter.
     """
     params = {}
-    params['betas'], params['pi'] = init_hdp_transitions(seed, **trans_hypparams)
-    params['Ab'], params['Q'] = init_ar_params(seed, **ar_hypparams)
+    params["betas"], params["pi"] = init_hdp_transitions(
+        seed, **trans_hypparams
+    )
+    params["Ab"], params["Q"] = init_ar_params(seed, **ar_hypparams)
     return params
 
 
 def init_hyperparams(trans_hypparams, ar_hypparams, **kwargs):
     """
     Formats the hyperparameter dictionary of the ARHMM.
-    
+
     Parameters
     ----------
     trans_hypparams : dict
         HDP transition hyperparameters.
     ar_hypparams : dict
         Autoregression hyperparameters.
     **kwargs : dict, optional
         Overflow, for convenience.
-        
+
     Returns
     -------
     hypparams : dict
         Values for each group of hyperparameters.
     """
     trans_hypparams = trans_hypparams.copy()
     ar_hypparams = ar_hypparams.copy()
-    
+
     # unpack for brevity
-    d = ar_hypparams['latent_dim']
-    nlags = ar_hypparams['nlags']
-    S_0_scale = ar_hypparams['S_0_scale']
-    K_0_scale = ar_hypparams['K_0_scale']
-
-    ar_hypparams['S_0'] = S_0_scale * jnp.eye(d)
-    ar_hypparams['K_0'] = K_0_scale * jnp.eye(d * nlags + 1)
-    ar_hypparams['M_0'] = jnp.pad(jnp.eye(d), ((0,0),((nlags-1)*d,1)))
-    ar_hypparams['num_states'] = trans_hypparams['num_states']
-    ar_hypparams['nu_0'] = d + 2
-    
-    return {'trans_hypparams': trans_hypparams,
-            'ar_hypparams': ar_hypparams}
-
-
-def init_model(data=None,
-               states=None,
-               params=None,
-               hypparams=None,
-               seed=jr.PRNGKey(0),
-               
-               trans_hypparams=None,
-               ar_hypparams=None,
-               
-               verbose=False,
-               **kwargs):
+    d = ar_hypparams["latent_dim"]
+    nlags = ar_hypparams["nlags"]
+    S_0_scale = ar_hypparams["S_0_scale"]
+    K_0_scale = ar_hypparams["K_0_scale"]
+
+    ar_hypparams["S_0"] = S_0_scale * jnp.eye(d)
+    ar_hypparams["K_0"] = K_0_scale * jnp.eye(d * nlags + 1)
+    ar_hypparams["M_0"] = jnp.pad(jnp.eye(d), ((0, 0), ((nlags - 1) * d, 1)))
+    ar_hypparams["num_states"] = trans_hypparams["num_states"]
+    ar_hypparams["nu_0"] = d + 2
+
+    return {"trans_hypparams": trans_hypparams, "ar_hypparams": ar_hypparams}
+
+
+def init_model(
+    data=None,
+    states=None,
+    params=None,
+    hypparams=None,
+    seed=jr.PRNGKey(0),
+    trans_hypparams=None,
+    ar_hypparams=None,
+    verbose=False,
+    **kwargs
+):
     """
     Initialize an ARHMM model dict containing the hyperparameters
-    and initial seed, states, and parameters. 
+    and initial seed, states, and parameters.
 
     Parameters
     ----------
     data : dict, optional
         Data dictionary containing the observations and mask.
         Must be provided if ``states`` not precomputed.
     states : dict, optional
@@ -179,66 +179,69 @@
         Overflow, for convenience.
 
     Returns
     -------
     model : dict
         Dictionary containing the hyperparameters and
         initial seed, states, and parameters of the model.
-        
+
     Raises
     ------
     ValueError
         If the subset of the parameters provided by the caller
         is insufficient for model initialization.
     """
-    _check_init_args(data, states, params, hypparams,
-                     trans_hypparams, ar_hypparams)
-    
+    _check_init_args(
+        data, states, params, hypparams, trans_hypparams, ar_hypparams
+    )
+
     model = {}
 
     if states is None:
-        x, mask = data['x'], data['mask']
-        
+        x, mask = data["x"], data["mask"]
+
     if isinstance(seed, int):
         seed = jr.PRNGKey(seed)
-    model['seed'] = seed
+    model["seed"] = seed
 
     if hypparams is None:
         if verbose:
-            print('ARHMM: Initializing hyperparameters')
+            print("ARHMM: Initializing hyperparameters")
         hypparams = init_hyperparams(trans_hypparams, ar_hypparams)
     else:
         hypparams = device_put_as_scalar(hypparams)
-    model['hypparams'] = hypparams
-    
+    model["hypparams"] = hypparams
+
     if params is None:
         if verbose:
-            print('ARHMM: Initializing parameters')
+            print("ARHMM: Initializing parameters")
         params = init_params(seed, **hypparams)
     else:
         params = jax.device_put(params)
-    model['params'] = params
+    model["params"] = params
 
     if states is None:
         if verbose:
-            print('ARHMM: Initializing states')
+            print("ARHMM: Initializing states")
         states = init_states(seed, x, mask, params)
     else:
         states = jax.device_put(states)
-    model['states'] = states
+    model["states"] = states
 
     return model
 
+
 @check_precision
-def _check_init_args(data, states, params, hypparams,
-                     trans_hypparams, ar_hypparams):
+def _check_init_args(
+    data, states, params, hypparams, trans_hypparams, ar_hypparams
+):
     """
     Helper method for ``init_model`` that ensures a sufficient subset
     of the initialization arguments have been provided by the caller.
-    
+
     Parameters
     ----------
     data : dict or None
         Data dictionary containing the observations, mask,
         and (optionally) confidences.
     states : dict or None
         State values for each latent variable.
@@ -246,20 +249,22 @@
         Values for each model parameter.
     hypparams : dict or None
         Values for each group of hyperparameters.
     trans_hypparams : dict or None
         HDP transition hyperparameters.
     ar_hypparams : dict or None
         Autoregression hyperparameters.
-        
+
     Raises
     ------
     ValueError
         If the subset of the parameters provided by the caller
         is insufficient for model initialization.
     """
     if not (data or states):
-        raise ValueError('Must provide either `data` or `states`.')
-        
+        raise ValueError("Must provide either `data` or `states`.")
+
     if not (hypparams or (trans_hypparams and ar_hypparams)):
-        raise ValueError('Must provide either `hypparams` or '
-                         'both `trans_hypparams` and `ar_hypparams`.')
+        raise ValueError(
+            "Must provide either `hypparams` or "
+            "both `trans_hypparams` and `ar_hypparams`."
+        )
```

### Comparing `jax-moseq-0.0.3/jax_moseq/models/arhmm/log_prob.py` & `jax-moseq-0.0.5/jax_moseq/models/slds/log_prob.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,118 +1,145 @@
 import jax
 import jax.numpy as jnp
+import tensorflow_probability.substrates.jax.distributions as tfd
 
-from jax_moseq.utils.autoregression import get_nlags, ar_log_likelihood
+from jax_moseq.utils import apply_affine
 
+from jax_moseq.models import arhmm
 
-def discrete_stateseq_log_prob(z, pi, **kwargs):
+na = jnp.newaxis
+
+
+def scale_log_prob(s, s_0, nu_s, **kwargs):
     """
-    Calculate the log probability of a discrete state sequence
-    at each timestep given a matrix of transition probabilities.
+    Calculate the log probability of the noise scale `s` for
+    each datapoint given the noise prior, which is a scaled
+    inverse chi-squared distribution.
 
     Parameters
     ----------
-    z : jax_array of shape (..., T - n_lags)
-        Discrete state sequences.
-    pi : jax_array of shape (num_states, num_states)
-        Transition probabilities.
+    s : jax array
+        Noise scales.
+    s_0 : scalar or jax array, broadcastable to `s`
+        Prior on noise scale.
+    nu_s : int
+        Chi-squared degrees of freedom in noise prior.
     **kwargs : dict
         Overflow, for convenience.
 
     Returns
     -------
-    log_pz : jax array of shape (..., T - 1)
-        Log probability of ``z``.
+    log_ps: jax array
+        Log probability of `s`.
     """
-    return jnp.log(pi[z[...,:-1],z[...,1:]])
+    return -nu_s * s_0 / s / 2 - (1 + nu_s / 2) * jnp.log(s)
 
 
-def continuous_stateseq_log_prob(x, z, Ab, Q, **kwargs):
+def obs_log_prob(Y, x, s, Cd, sigmasq, **kwargs):
     """
-    Calculate the log probability of the trajectory ``x`` at each time 
-    step, given switching autoregressive (AR) parameters
+    Calculate the log probability of the observations at each
+    time-step given the latent trajectories, noise parameters, and
+    observation matrix.
 
     Parameters
-    ----------  
-    x : jax array of shape (..., T, latent_dim)
+    ----------
+    Y : jax array of shape (..., obs_dim)
+        Observations.
+    x : jax array of shape (..., latent_dim)
         Latent trajectories.
-    z : jax_array of shape (..., T - n_lags)
-        Discrete state sequences.
-    Ab : jax array of shape (num_states, latent_dim, ar_dim)
-        Autoregressive transforms.
-    Q : jax array of shape (num_states, latent_dim, latent_dim)
-        Autoregressive noise covariances.
+    s : jax array of shape (..., obs_dim)
+        Noise scales.
+    Cd : jax array of shape (obs_dim, latent_dim + 1)
+        Observation transform.
+    sigmasq : jax_array of shape obs_dim
+        Unscaled noise.
     **kwargs : dict
         Overflow, for convenience.
 
     Returns
     -------
-    log_px : jax array of shape (..., T - n_lags)
-        Log probability of ``x``.
+    log_pY: jax array of shape (..., obs_dim)
+        Log probability of `Y`.
     """
-    return ar_log_likelihood(x, (Ab[z], Q[z]))
+    Y_bar = apply_affine(x, Cd)
+    cov = jnp.sqrt(s * sigmasq)
+    return tfd.MultivariateNormalDiag(Y_bar, cov).log_prob(Y)
 
 
 @jax.jit
-def log_joint_likelihood(x, mask, z, pi, Ab, Q, **kwargs):
+def log_joint_likelihood(
+    Y, mask, x, s, z, pi, Ab, Q, Cd, sigmasq, s_0, nu_s, **kwargs
+):
     """
-    Calculate the total log probability for each latent state
+    Calculate the total log probability for each latent state.
 
     Parameters
     ----------
+    Y : jax array of shape (..., T, obs_dim)
+        Observations.
+    mask : jax array of shape (..., T)
+        Binary indicator for valid frames.
     x : jax array of shape (..., T, latent_dim)
         Latent trajectories.
-    mask : jax array
-        Binary indicator for which data points are valid.
+    s : jax array of shape (..., T, obs_dim)
+        Noise scales.
     z : jax_array of shape (..., T - n_lags)
         Discrete state sequences.
     pi : jax_array of shape (num_states, num_states)
         Transition probabilities.
     Ab : jax array of shape (num_states, latent_dim, ar_dim)
         Autoregressive transforms.
     Q : jax array of shape (num_states, latent_dim, latent_dim)
         Autoregressive noise covariances.
+    Cd : jax array of shape (obs_dim, latent_dim + 1)
+        Observation transform.
+    sigmasq : jax_array of shape obs_dim
+        Unscaled noise.
+    s_0 : scalar or jax array broadcastable to `Y`
+        Prior on noise scale.
+    nu_s : int
+        Chi-squared degrees of freedom in noise prior.
     **kwargs : dict
         Overflow, for convenience.
 
     Returns
     -------
-    ll : dict
-        Dictionary mapping state variable name to its
-        total log probability.
+    ll: dict
+        Dictionary mapping the name of each state variable to
+        its total log probability.
     """
-    ll = {}
-    
-    log_pz = discrete_stateseq_log_prob(z, pi)
-    log_px = continuous_stateseq_log_prob(x, z, Ab, Q)
-    
-    nlags = get_nlags(Ab)
-    ll['z'] = (log_pz * mask[..., nlags + 1:]).sum()
-    ll['x'] = (log_px * mask[..., nlags:]).sum()
+    ll = arhmm.log_joint_likelihood(x, mask, z, pi, Ab, Q)
+
+    log_pY = obs_log_prob(Y, x, s, Cd, sigmasq)
+    log_ps = scale_log_prob(s, s_0, nu_s)
+
+    ll["Y"] = (log_pY * mask).sum()
+    ll["s"] = (log_ps * mask[..., na]).sum()
     return ll
 
 
-def model_likelihood(data, states, params,
-                     hypparams=None, **kwargs):
+def model_likelihood(data, states, params, hypparams, **kwargs):
     """
-    Convenience class that invokes :py:func:`jax_moseq.models.arhmm.log_prob.log_joint_likelihood`.
-    
+    Convenience class that invokes `log_joint_likelihood`.
+
     Parameters
     ----------
     data : dict
         Data dictionary containing the observations and mask.
     states : dict
         State values for each latent variable.
     params : dict
         Values for each model parameter.
-    hypparams : dict, optional
+    hypparams : dict
         Values for each group of hyperparameters.
     **kwargs : dict
         Overflow, for convenience.
 
     Returns
     ------
     ll : dict
         Dictionary mapping state variable name to its
         total log probability.
     """
-    return log_joint_likelihood(**data, **states, **params)
+    return log_joint_likelihood(
+        **data, **states, **params, **hypparams["obs_hypparams"]
+    )
```

### Comparing `jax-moseq-0.0.3/jax_moseq/models/keypoint_slds/alignment.py` & `jax-moseq-0.0.5/jax_moseq/models/keypoint_slds/alignment.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 def to_vanilla_slds(Y, v, h, s, Cd, sigmasq, **kwargs):
     """
     Given the empirical keypoint positions, position/heading
     estimates, isotropic noise estimates, and emission parameters,
     this function returns the (relevant subset of the) observations,
     states, and params for an equivalent SLDS that directly maps the
     latent trajectories to flattened and aligned keypoint observations.
-    
+
     Parameters
     ----------
     Y : jax array of shape (..., k, d)
         Keypoint observations.
     v : jax array of shape (..., d)
         Centroid positions.
     h : jax array of shape (..., T)
@@ -28,15 +28,15 @@
         Noise scales.
     Cd : jax array of shape ((k - 1) * d, latent_dim + 1)
         Observation transform.
     sigmasq : jax_array of shape k
         Unscaled noise.
     **kwargs : dict
         Overflow, for convenience.
-        
+
     Returns
     -------
     Y : jax array of shape (..., k * d)
         Flattened and aligned keypoint observations.
     s : jax array of shape (..., k * d)
         Noise scales repeated along spatial dimension.
     Cd : jax array of shape (k * d, latent_dim + 1)
@@ -61,15 +61,15 @@
     sigmasq = jnp.repeat(sigmasq, d, axis=-1)
 
     return Y, s, Cd, sigmasq
 
 
 def estimate_coordinates(x, v, h, Cd, **kwargs):
     """
-    Estimate keypoint coordinates obtained from projecting the 
+    Estimate keypoint coordinates obtained from projecting the
     latent state ``x`` into keypoint-space (via ``Cd``) and then
     rotating and translating by ``h`` and ``v`` respectively
 
     Parameters
     ----------
     x : jax array of shape (..., latent_dim)
         Latent trajectories.
@@ -117,84 +117,82 @@
     # Apply emissions to obtain flattened,
     # centered, keypoint observation
     y = apply_affine(x, Cd)
 
     # Reshape keypoints
     batch_shape = x.shape[:-1]
     y = y.reshape(*batch_shape, k - 1, -1)
-
-    # Center
-    Gamma = center_embedding(k) 
+    Gamma = center_embedding(k)
     return Gamma @ y
 
 
 @jax.jit
 def rigid_transform(Y, v, h):
     """
     Apply the rigid transform consisting of rotation by h
     and translation by v to a set of keypoint observations.
-    
+
     Parameters
     ----------
     Y : jax array of shape (..., k, d)
         Keypoint observations.
     v : jax array of shape (..., d)
         Centroid positions.
     h : jax array
         Heading angles.
-          
+
     Returns
     -------
     Y_transformed: jax array of shape (..., k, d)
         Rigidly transformed positions.
     """
     return apply_rotation(Y, h) + v[..., na, :]
 
 
 @jax.jit
 def inverse_rigid_transform(Y, v, h):
     """
     Apply the inverse of the rigid transform consisting of
     rotation by h and translation by v to a set of keypoint
     observations.
-    
+
     Parameters
     ----------
     Y : jax array of shape (..., k, d)
         Keypoint observations.
     v : jax array of shape (..., d)
         Centroid positions.
     h : jax array
         Heading angles.
-          
+
     Returns
     -------
     Y_transformed: jax array of shape (..., k, d)
         Rigidly transformed positions.
     """
     return apply_rotation(Y - v[..., na, :], -h)
 
 
 def center_embedding(k):
     """
-    Generates a matrix ``Gamma`` that maps from a (k-1)-dimensional 
+    Generates a matrix ``Gamma`` that maps from a (k-1)-dimensional
     vector space  to the space of k-tuples with zero mean
-    
+
     Parameters
     ----------
     k : int
         Number of keypoints.
 
     Returns
     -------
     Gamma: jax array of shape (k, k - 1)
         Matrix to map to centered embedded space.
-    """  
+    """
     # using numpy.linalg.svd because jax version crashes on windows
-    return jnp.array(np.linalg.svd(np.eye(k) - np.ones((k, k)) / k)[0][:,:-1])
+    return jnp.array(np.linalg.svd(np.eye(k) - np.ones((k, k)) / k)[0][:, :-1])
 
 
 def apply_rotation(Y, h):
     """
     Rotate ``Y`` by ``h`` radians.
 
     Parameters
@@ -207,69 +205,79 @@
     Returns
     ------
     Y_rot : jax array of shape (..., k, d)
         Rotated keypoint observations.
     """
     d = Y.shape[-1]
     rot_matrix = angle_to_rotation_matrix(h, d)
-    return jnp.einsum('...kj,...ij->...ki', Y, rot_matrix)
+    return jnp.einsum("...kj,...ij->...ki", Y, rot_matrix)
 
 
 def angle_to_rotation_matrix(h, d=3):
     """
     Create rotation matrices from an array of angles. If
     ``d > 2`` then rotation is performed in the first two dims.
-    
+
     Parameters
     ----------
     h : jax array of shape (N, T)
         Heading angles.
     d : int, default=3
         Keypoint dimensionality (either 2 or 3).
 
     Returns
     ------
     m: jax array of shape (..., d, d)
         Rotation matrices.
     """
-    m = jnp.tile(jnp.eye(d), (*h.shape,1,1))
-    m = m.at[...,0,0].set(jnp.cos(h))
-    m = m.at[...,1,1].set(jnp.cos(h))
-    m = m.at[...,0,1].set(-jnp.sin(h))
-    m = m.at[...,1,0].set(jnp.sin(h))
+    m = jnp.tile(jnp.eye(d), (*h.shape, 1, 1))
+    m = m.at[..., 0, 0].set(jnp.cos(h))
+    m = m.at[..., 1, 1].set(jnp.cos(h))
+    m = m.at[..., 0, 1].set(-jnp.sin(h))
+    m = m.at[..., 1, 0].set(jnp.sin(h))
     return m
 
 
 def vector_to_angle(V):
     """
     Convert 2D vectors to angles in [-pi, pi]. The vector (1,0)
     corresponds to angle of 0. If V is multidimensional, the first
-    n-1 dimensions are treated as batch dims. 
+    n-1 dimensions are treated as batch dims.
 
     Parameters
     ----------
     V : jax array of shape (..., 2)
         Batch of 2D vectors.
 
     Returns
     ------
     h : jax array
         Rotation angles in radians.
     """
-    return jnp.arctan2(V[...,1], V[...,0])
+    return jnp.arctan2(V[..., 1], V[..., 0])
 
 
-def fit_pca(Y, mask, anterior_idxs=None, posterior_idxs=None, conf=None, 
-            conf_threshold=0.5, verbose=False, PCA_fitting_num_frames=1000000, 
-            exclude_outliers_for_pca=True, fix_heading=False, **kwargs):
+def fit_pca(
+    Y,
+    mask,
+    anterior_idxs=None,
+    posterior_idxs=None,
+    conf=None,
+    conf_threshold=0.5,
+    verbose=False,
+    PCA_fitting_num_frames=1000000,
+    exclude_outliers_for_pca=False,
+    fix_heading=False,
+    **kwargs,
+):
     """
     Fit a PCA model to transformed keypoint coordinates. If ``conf`` is
     not None, perform linear interpolation over outliers defined by
     ``conf < conf_threshold``.
-    
+
     Parameters
     ----------
     Y : jax array of shape (..., k, d)
         Keypoint observations.
     mask : jax array
         Binary indicator for valid frames.
     anterior_idxs : iterable of ints
@@ -280,160 +288,187 @@
         Confidence for each keypoint observation. Must be >= 0.
     conf_threshold : float, default=0.5
         Confidence threshold for interpolation.
     verbose : bool, default=False
         Whether to print progress updates.
     PCA_fitting_num_frames : int, default=1000000
         Maximum number of frames for PCA fitting.
-    exclude_outliers_for_pca : bool, default=True
+    exclude_outliers_for_pca : bool, default=False
         Whether to exclude frames with low-confidence keypoints.
-        If False, then the low-confidence keypoint coordinates are l
-        inearly interpolated.
+        If False, then the low-confidence keypoint coordinates are
+        linearly interpolated.
     fix_heading : bool, default=False
-        Whether keep the heading angle fixed. If true, the 
+        Whether keep the heading angle fixed. If true, the
         heading ``h`` is set to 0 and keypoints are not rotated.
     **kwargs : dict
         Overflow, for convenience.
 
     Returns
     -------
     pca, sklearn.decomposition._pca.PCA
         PCA object fit to observations.
     """
     Y_flat = preprocess_for_pca(
-        Y, anterior_idxs, posterior_idxs, conf, 
-        conf_threshold, fix_heading, verbose)[0]
-    
-    if not exclude_outliers_for_pca or conf is None: pca_mask = mask
-    else: pca_mask = jnp.logical_and(mask, (conf > conf_threshold).all(-1))
+        Y,
+        anterior_idxs,
+        posterior_idxs,
+        conf,
+        conf_threshold,
+        fix_heading,
+        verbose,
+    )[0]
+
+    if (not exclude_outliers_for_pca) or (conf is None):
+        pca_mask = mask
+    else:
+        pca_mask = jnp.logical_and(mask, (conf > conf_threshold).all(-1))
+
+    assert pca_mask.sum() >= (Y.shape[-1] * Y.shape[-2]), (
+        "Not enough frames for PCA fitting. Make sure "
+        "`exclude_outliers_for_pca=False` 'or decrease `conf_threshold`."
+    )
+
     return utils.fit_pca(Y_flat, pca_mask, PCA_fitting_num_frames, verbose)
 
 
-def preprocess_for_pca(Y, anterior_idxs, posterior_idxs, conf=None, 
-                       conf_threshold=.5, fix_heading=False, 
-                       verbose=False, **kwargs):
+def preprocess_for_pca(
+    Y,
+    anterior_idxs,
+    posterior_idxs,
+    conf=None,
+    conf_threshold=0.5,
+    fix_heading=False,
+    verbose=False,
+    **kwargs,
+):
     """
-    Prepare keypoint coordinates for PCA by performing egocentric 
+    Prepare keypoint coordinates for PCA by performing egocentric
     alignment (optional), changing basis using ``center_embedding(k)``,
     and reshaping to a single flat vector per frame.
-    
+
     Parameters
     ----------
     Y : jax array of shape (..., k, d)
         Keypoint observations.
     anterior_idxs : iterable of ints
         Anterior keypoint indices for heading initialization.
     posterior_idxs : iterable of ints
         Posterior keypoint indices for heading initialization.
     conf : jax array of shape (..., k), optional
         Confidence for each keypoint observation. Must be >= 0.
     conf_threshold : float, default=.5
         Confidence threshold for interpolation.
     fix_heading : bool, default=False
-        Whether keep the heading angle fixed. If true, the 
+        Whether keep the heading angle fixed. If true, the
         heading ``h`` is set to 0 and keypoints are not rotated.
     verbose : bool, default=False
         Whether to print progress updates.
     **kwargs : dict
         Overflow, for convenience.
-          
+
     Returns
     -------
     Y_flat : jax array of shape (..., (k - 1) * d), optional
         Aligned and embedded keypoint observations.
     """
     if conf is not None:
-        outliers = (conf < conf_threshold)
+        outliers = conf < conf_threshold
         if verbose:
             n = outliers.sum()
             pct = outliers.mean() * 100
-            if verbose:
-                print(f'Interpolating {n} ({pct:.1f}%) low-confidence keypoints')
+            print(f"Interpolating {n} ({pct:.1f}%) low-confidence keypoints")
         Y = interpolate(Y, outliers)
-    
+
     if fix_heading:
         v = Y.mean(-2).at[..., 2:].set(0)
         h = jnp.zeros(Y.shape[:-2])
-        Y_aligned = Y - v[...,na,:]
+        Y_aligned = Y - v[..., na, :]
     else:
         Y_aligned, v, h = align_egocentric(Y, anterior_idxs, posterior_idxs)
 
     dims = Y.shape[:-2]
     k, d = Y.shape[-2:]
     Gamma_inv = center_embedding(k).T
     Y_embedded = Gamma_inv @ Y_aligned
     Y_flat = Y_embedded.reshape(*dims, (k - 1) * d)
     return Y_flat, v, h
 
 
 def align_egocentric(Y, anterior_idxs, posterior_idxs, **kwargs):
     """
-    Perform egocentric alignment of keypoints by translating the 
+    Perform egocentric alignment of keypoints by translating the
     centroid to the origin and rotatating so that the vector pointing
-    from the posterior bodyparts toward the anterior bodyparts is 
+    from the posterior bodyparts toward the anterior bodyparts is
     proportional to (1,0).
-    
+
     Parameters
     ----------
     Y : jax array of shape (..., k, d)
         Keypoint observations.
     anterior_idxs : iterable of ints
         Anterior keypoint indices for heading initialization.
     posterior_idxs : iterable of ints
         Posterior keypoint indices for heading initialization.
     **kwargs : dict
         Overflow, for convenience.
-        
+
     Returns
     -------
     Y_aligned : jax array of shape (..., k, d)
         Aligned keypoint coordinates.
     v : jax array of shape (..., d)
         Centroid positions that were used for alignment.
     h : jax array
         Heading angles that were used for alignment.
     """
-    posterior_loc = Y[..., posterior_idxs, :2].mean(-2) 
-    anterior_loc = Y[..., anterior_idxs, :2].mean(-2) 
+    posterior_loc = Y[..., posterior_idxs, :2].mean(-2)
+    anterior_loc = Y[..., anterior_idxs, :2].mean(-2)
     h = vector_to_angle(anterior_loc - posterior_loc)
     v = Y.mean(-2).at[..., 2:].set(0)
-    Y_aligned = inverse_rigid_transform(Y,v,h)
+    Y_aligned = inverse_rigid_transform(Y, v, h)
     return Y_aligned, v, h
 
 
 @jax_io
 def interpolate(Y, outliers, axis=1):
     """
     Use linear interpolation to impute the coordinates of outliers.
-    
+
     Parameters
     ----------
     Y : jax array of shape (N, T, k, d)
         Keypoint observations.
     outliers : jax array of shape (..., T, k)
         Binary indicator whose true entries are outlier points.
     axis : int, default=1
         Axis to interpolate along.
-        
+
     Returns
     -------
     Y_interp : jax array, shape (..., T, k, d)
         Copy of ``Y`` where outliers have been replaced by
         linearly interpolated values.
-    """   
+    """
     Y = np.moveaxis(Y, axis, 0)
     init_shape = Y.shape
-    Y = Y.reshape(init_shape[0],-1)
+    Y = Y.reshape(init_shape[0], -1)
 
     outliers = np.moveaxis(outliers, axis, 0)
-    outliers = np.repeat(outliers[...,None],init_shape[-1],axis=-1)
-    outliers = outliers.reshape(init_shape[0],-1)
+    outliers = np.repeat(outliers[..., None], init_shape[-1], axis=-1)
+    outliers = outliers.reshape(init_shape[0], -1)
 
     interp = lambda x, xp, fp: (
-        np.ones_like(x)*x.mean() if len(xp)==0 else np.interp(x,xp,fp))
-    
-    Y = np.stack([interp(
-        np.arange(init_shape[0]), 
-        np.nonzero(~outliers[:,i])[0],
-        Y[:,i][~outliers[:,i]]
-    ) for i in range(Y.shape[1])], axis=1)     
-    return np.moveaxis(Y.reshape(init_shape),0,axis)
+        np.ones_like(x) * x.mean() if len(xp) == 0 else np.interp(x, xp, fp)
+    )
+
+    Y = np.stack(
+        [
+            interp(
+                np.arange(init_shape[0]),
+                np.nonzero(~outliers[:, i])[0],
+                Y[:, i][~outliers[:, i]],
+            )
+            for i in range(Y.shape[1])
+        ],
+        axis=1,
+    )
+    return np.moveaxis(Y.reshape(init_shape), 0, axis)
```

### Comparing `jax-moseq-0.0.3/jax_moseq/models/keypoint_slds/gibbs.py` & `jax-moseq-0.0.5/jax_moseq/models/keypoint_slds/gibbs.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,44 @@
 import jax
 import jax.numpy as jnp
 import jax.random as jr
+from functools import partial
 
 from jax_moseq.utils.kalman import kalman_sample
-from jax_moseq.utils.distributions import sample_vonmises_fisher, sample_scaled_inv_chi2
+from jax_moseq.utils.distributions import sample_vonmises_fisher
 
 from jax_moseq.models import arhmm, slds
 from jax_moseq.models.keypoint_slds.alignment import (
     to_vanilla_slds,
     estimate_coordinates,
     estimate_aligned,
     apply_rotation,
-    vector_to_angle
+    vector_to_angle,
 )
 
 na = jnp.newaxis
 
 
-@jax.jit
-def resample_continuous_stateseqs(seed, Y, mask, v, h, s, z,
-                                  Cd, sigmasq, Ab, Q, **kwargs):
+@partial(jax.jit, static_argnames=("parallel_message_passing",))
+def resample_continuous_stateseqs(
+    seed,
+    Y,
+    mask,
+    v,
+    h,
+    s,
+    z,
+    Cd,
+    sigmasq,
+    Ab,
+    Q,
+    jitter=1e-3,
+    parallel_message_passing=True,
+    **kwargs
+):
     """
     Resamples the latent trajectories ``x``.
 
     Parameters
     ----------
     seed : jr.PRNGKey
         JAX random seed.
@@ -43,31 +58,49 @@
         Observation transform.
     sigmasq : jax_array of shape k
         Unscaled noise.
     Ab : jax array of shape (num_states, latent_dim, ar_dim)
         Autoregressive transforms.
     Q : jax array of shape (num_states, latent_dim, latent_dim)
         Autoregressive noise covariances.
+    jitter : float, default=1e-3
+        Amount to boost the diagonal of the covariance matrix
+        during backward-sampling of the continuous states.
+    parallel_message_passing : bool, default=True,
+        Use associative scan for Kalman sampling, which is faster on
+        a GPU but has a significantly longer jit time.
     **kwargs : dict
         Overflow, for convenience.
 
     Returns
     ------
     x : jax array of shape (N, T, latent_dim)
         Latent trajectories.
     """
     Y, s, Cd, sigmasq = to_vanilla_slds(Y, v, h, s, Cd, sigmasq)
-    x = slds.resample_continuous_stateseqs(seed, Y, mask, z, s,
-                                           Ab, Q, Cd, sigmasq)
+    x = slds.resample_continuous_stateseqs(
+        seed,
+        Y,
+        mask,
+        z,
+        s,
+        Ab,
+        Q,
+        Cd,
+        sigmasq,
+        jitter=jitter,
+        parallel_message_passing=parallel_message_passing,
+    )
     return x
 
 
 @jax.jit
-def resample_obs_variance(seed, Y, mask, Cd, x, v, h, s,
-                          nu_sigma, sigmasq_0, **kwargs):
+def resample_obs_variance(
+    seed, Y, mask, Cd, x, v, h, s, nu_sigma, sigmasq_0, **kwargs
+):
     """
     Resample the observation variance ``sigmasq``.
 
     Parameters
     ----------
     seed : jr.PRNGKey
         JAX random seed.
@@ -94,21 +127,21 @@
 
     Returns
     ------
     sigmasq : jax_array of shape k
         Unscaled noise.
     """
     sqerr = compute_squared_error(Y, x, v, h, Cd, mask)
-    return slds.resample_obs_variance_from_sqerr(seed, sqerr, mask, s,
-                                                 nu_sigma, sigmasq_0)
+    return slds.resample_obs_variance_from_sqerr(
+        seed, sqerr, mask, s, nu_sigma, sigmasq_0
+    )
 
 
 @jax.jit
-def resample_scales(seed, Y, x, v, h, Cd,
-                    sigmasq, nu_s, s_0, **kwargs):
+def resample_scales(seed, Y, x, v, h, Cd, sigmasq, nu_s, s_0, **kwargs):
     """
     Resample the scale values ``s``.
 
     Parameters
     ----------
     seed : jr.PRNGKey
         JAX random seed.
@@ -133,16 +166,15 @@
 
     Returns
     ------
     s : jax array of shape (N, T, k)
         Noise scales.
     """
     sqerr = compute_squared_error(Y, x, v, h, Cd)
-    return slds.resample_scales_from_sqerr(seed, sqerr,
-                                           sigmasq, nu_s, s_0)
+    return slds.resample_scales_from_sqerr(seed, sqerr, sigmasq, nu_s, s_0)
 
 
 @jax.jit
 def compute_squared_error(Y, x, v, h, Cd, mask=None):
     """
     Computes the squared error between model predicted
     and true observations.
@@ -164,16 +196,16 @@
 
     Returns
     ------
     sqerr : jax array of shape (..., k)
         Squared error between model predicted and
         true observations.
     """
-    Y_bar = estimate_coordinates(x, v, h, Cd)
-    sqerr = ((Y - Y_bar) ** 2).sum(-1)
+    Y_est = estimate_coordinates(x, v, h, Cd)
+    sqerr = ((Y - Y_est) ** 2).sum(-1)
     if mask is not None:
         sqerr = mask[..., na] * sqerr
     return sqerr
 
 
 @jax.jit
 def resample_heading(seed, Y, x, v, s, Cd, sigmasq, **kwargs):
@@ -207,30 +239,43 @@
     k = Y.shape[-2]
 
     Y_bar = estimate_aligned(x, Cd, k)
     Y_cent = Y - v[..., na, :]
     variance = s * sigmasq
 
     # [(..., t, k, d, na) * (..., t, k, na, d) / (..., t, k, na, na)] -> (..., t, d, d)
-    S = (Y_bar[..., :2, na] * Y_cent[..., na, :2] / variance[..., na, na]).sum(-3)
-    del Y_bar, Y_cent, variance    # free up memory
+    S = (Y_bar[..., :2, na] * Y_cent[..., na, :2] / variance[..., na, na]).sum(
+        -3
+    )
+    del Y_bar, Y_cent, variance  # free up memory
 
-    kappa_cos = S[...,0,0] + S[...,1,1]
-    kappa_sin = S[...,0,1] - S[...,1,0]
+    kappa_cos = S[..., 0, 0] + S[..., 1, 1]
+    kappa_sin = S[..., 0, 1] - S[..., 1, 0]
     del S
 
     mean_direction = jnp.stack([kappa_cos, kappa_sin], axis=-1)
     sampled_direction = sample_vonmises_fisher(seed, mean_direction)
     h = vector_to_angle(sampled_direction)
     return h
 
 
-@jax.jit 
-def resample_location(seed, Y, mask, x, h, s, Cd,
-                      sigmasq, sigmasq_loc, **kwargs):
+@jax.jit
+def resample_location(
+    seed,
+    Y,
+    mask,
+    x,
+    h,
+    s,
+    Cd,
+    sigmasq,
+    sigmasq_loc,
+    parallel_message_passing=True,
+    **kwargs
+):
     """
     Resample the centroid positions ``v``.
 
     Parameters
     ----------
     seed : jr.PRNGKey
         JAX random seed.
@@ -246,14 +291,17 @@
         Noise scales.
     Cd : jax array of shape ((k - 1) * d, latent_dim + 1)
         Observation transform.
     sigmasq : jax_array of shape k
         Unscaled noise.
     sigmasq_loc : float
         Assumed variance in centroid displacements.
+    parallel_message_passing : bool, default=True,
+        Use associative scan for Kalman sampling, which is faster on
+        a GPU but has a significantly longer jit time.
     **kwargs : dict
         Overflow, for convenience.
 
     Returns
     ------
     v : jax array of shape (N, T, d)
         Centroid positions.
@@ -261,41 +309,79 @@
     k, d = Y.shape[-2:]
 
     Y_rot = apply_rotation(estimate_aligned(x, Cd, k), h)
 
     variance = s * sigmasq
     gammasq = 1 / (1 / variance).sum(-1, keepdims=True)
 
-    mu = jnp.einsum('...tkd, ...tk->...td',
-                    Y - Y_rot, gammasq / variance)
+    mu = jnp.einsum("...tkd, ...tk->...td", Y - Y_rot, gammasq / variance)
 
     # Apply Kalman filter to get smooth headings
+    # TODO Parameterize these distributional hyperparameter
     seed = jr.split(seed, mask.shape[0])
     m0 = jnp.zeros(d)
-    S0 = jnp.eye(d) * 1e6
+    S0 = jnp.eye(d) * 1e4
     A = jnp.eye(d)[na]
     B = jnp.zeros(d)[na]
     Q = jnp.eye(d)[na] * sigmasq_loc
     C = jnp.eye(d)
     D = jnp.zeros(d)
     R = jnp.repeat(gammasq, d, axis=-1)
-    zz = jnp.zeros_like(mask[:,1:], dtype=int)
+    zz = jnp.zeros_like(mask[:, 1:], dtype=int)
 
-    in_axes = (0,0,0,0,na,na,na,na,na,na,na,0)
-    v = jax.vmap(kalman_sample, in_axes)(
-        seed, mu, mask[:,:-1], zz, m0,
-        S0, A, B, Q, C, D, R)
-    return v
+    masked_dynamics_noise = sigmasq_loc * 10
+    masked_obs_noise = sigmasq.max() * 10
 
+    masked_dynamics_params = {
+        "weights": jnp.eye(d),
+        "bias": jnp.zeros(d),
+        "cov": jnp.eye(d) * masked_dynamics_noise,
+    }
+
+    masked_obs_noise_diag = jnp.ones(d) * masked_obs_noise
+
+    in_axes = (0, 0, 0, 0, na, na, na, na, na, na, na, 0, na, na)
+    v = jax.vmap(
+        partial(kalman_sample, parallel=parallel_message_passing), in_axes
+    )(
+        seed,
+        mu,
+        mask,
+        zz,
+        m0,
+        S0,
+        A,
+        B,
+        Q,
+        C,
+        D,
+        R,
+        masked_dynamics_params,
+        masked_obs_noise_diag,
+    )
+    return v
 
 
-def resample_model(data, seed, states, params, hypparams,
-                   noise_prior, ar_only=False, states_only=False,
-                   skip_noise=False, fix_heading=False, verbose=False,
-                   **kwargs):
+def resample_model(
+    data,
+    seed,
+    states,
+    params,
+    hypparams,
+    noise_prior,
+    ar_only=False,
+    states_only=False,
+    resample_global_noise_scale=False,
+    resample_local_noise_scale=True,
+    fix_heading=False,
+    verbose=False,
+    jitter=1e-3,
+    parallel_message_passing=False,
+    **kwargs
+):
     """
     Resamples the Keypoint SLDS model given the hyperparameters,
     data, noise prior, current states, and current parameters.
 
     Parameters
     ----------
     data : dict
@@ -310,61 +396,92 @@
         Values for each group of hyperparameters.
     noise_prior : scalar or jax array broadcastable to ``s``
         Prior on noise scale.
     ar_only : bool, default=False
         Whether to restrict sampling to ARHMM components.
     states_only : bool, default=False
         Whether to restrict sampling to states.
-    skip_noise : bool, default=False
-        Whether to exclude ``sigmasq`` and ``s`` from resampling.
+    resample_global_noise_scale : bool, default=False
+        Whether to resample the global noise scales (``sigmasq``)
+    resample_local_noise_scale : bool, default=True
+        Whether to resample the local noise scales (``s``)
     fix_heading : bool, default=False
         Whether to exclude ``h`` from resampling.
+    jitter : float, default=1e-3
+        Amount to boost the diagonal of the covariance matrix
+        during backward-sampling of the continuous states.
     verbose : bool, default=False
         Whether to print progress info during resampling.
+    parallel_message_passing : bool, default=True,
+        Use associative scan for Kalman sampling, which is faster on
+        a GPU but has a significantly longer jit time.
 
     Returns
     ------
     model : dict
         Dictionary containing the hyperparameters and
         updated seed, states, and parameters of the model.
     """
-    model = arhmm.resample_model(data, seed, states, params,
-                                 hypparams, states_only, verbose=verbose)
+    model = arhmm.resample_model(
+        data, seed, states, params, hypparams, states_only, verbose=verbose
+    )
     if ar_only:
-        model['noise_prior'] = noise_prior
+        model["noise_prior"] = noise_prior
         return model
-    
-    seed = model['seed']
-    params = model['params'].copy()
-    states = model['states'].copy()
-
-    if not (states_only or skip_noise):
-        if verbose: print('Resampling sigmasq (global noise scales)')
-        params['sigmasq'] = resample_obs_variance(
-            seed, **data, **states, **params, 
-            s_0=noise_prior, **hypparams['obs_hypparams'])
-
-    if verbose: print('Resampling x (continuous latent states)')
-    states['x'] = resample_continuous_stateseqs(
-        seed, **data, **states, **params)
+
+    seed = model["seed"]
+    params = model["params"].copy()
+    states = model["states"].copy()
+
+    if (not states_only) and resample_global_noise_scale:
+        if verbose:
+            print("Resampling sigmasq (global noise scales)")
+        params["sigmasq"] = resample_obs_variance(
+            seed,
+            **data,
+            **states,
+            **params,
+            s_0=noise_prior,
+            **hypparams["obs_hypparams"]
+        )
+
+    if verbose:
+        print("Resampling x (continuous latent states)")
+    states["x"] = resample_continuous_stateseqs(
+        seed,
+        **data,
+        **states,
+        **params,
+        jitter=jitter,
+        parallel_message_passing=parallel_message_passing
+    )
 
     if not fix_heading:
-        if verbose: print('Resampling h (heading)')
-        states['h'] = resample_heading(
-            seed, **data, **states, **params)
-
-    if verbose: print('Resampling v (location)')
-    states['v'] = resample_location(
-        seed, **data, **states, **params, 
-        **hypparams['cen_hypparams'])
-
-    if not skip_noise:
-        if verbose: print('Resampling s (local noise scales)')
-        states['s'] = resample_scales(
-            seed, **data, **states, **params, 
-            s_0=noise_prior, **hypparams['obs_hypparams'])
-
-    return {'seed': seed,
-            'states': states, 
-            'params': params, 
-            'hypparams': hypparams,
-            'noise_prior': noise_prior}
+        if verbose:
+            print("Resampling h (heading)")
+        states["h"] = resample_heading(seed, **data, **states, **params)
+
+    if verbose:
+        print("Resampling v (location)")
+    states["v"] = resample_location(
+        seed, **data, **states, **params, **hypparams["cen_hypparams"]
+    )
+
+    if resample_local_noise_scale:
+        if verbose:
+            print("Resampling s (local noise scales)")
+        states["s"] = resample_scales(
+            seed,
+            **data,
+            **states,
+            **params,
+            s_0=noise_prior,
+            **hypparams["obs_hypparams"]
+        )
+
+    return {
+        "seed": seed,
+        "states": states,
+        "params": params,
+        "hypparams": hypparams,
+        "noise_prior": noise_prior,
+    }
```

### Comparing `jax-moseq-0.0.3/jax_moseq/models/keypoint_slds/initialize.py` & `jax-moseq-0.0.5/jax_moseq/models/keypoint_slds/initialize.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,20 +6,31 @@
 from jax_moseq.utils import jax_io, device_put_as_scalar, check_precision
 
 from jax_moseq.models import arhmm, slds
 from jax_moseq.models.keypoint_slds.gibbs import resample_scales
 from jax_moseq.models.keypoint_slds.alignment import preprocess_for_pca
 
 
-def init_states(seed, Y, mask, params, noise_prior, obs_hypparams,
-                Y_flat=None, v=None, h=None, fix_heading=False, **kwargs):
+def init_states(
+    seed,
+    Y,
+    mask,
+    params,
+    noise_prior,
+    obs_hypparams,
+    Y_flat=None,
+    v=None,
+    h=None,
+    fix_heading=False,
+    **kwargs
+):
     """
     Initialize the latent states of the keypoint SLDS from the data,
     parameters, and hyperparameters.
-    
+
     Parameters
     ----------
     seed : jr.PRNGKey
         JAX random seed.
     Y : jax array of shape (N, T, k, d)
         Keypoint observations.
     mask : jax array of shape (N, T)
@@ -34,44 +45,46 @@
         Aligned and embedded keypoint observations.
     v : jax array of shape (N, T, d), optional
         Initial centroid positions.
     h : jax array of shape (N, T), optional
         Initial heading angles.
     fix_heading : bool, default=False
         Whether keep the heading angle of the pose fixed. If true,
-        the heading variable ``h`` is initialized as 0. 
+        the heading variable ``h`` is initialized as 0.
     **kwargs : dict, optional
         Arguments to :py:func:`jax_moseq.models.keypoint_slds.alignment.preprocess_for_pca`, as a substitute for
         ``Y_flat``, ``v``, or ``h``.
-        
+
     Returns
     -------
     states : dict
         State values for each latent variable.
     """
     if Y_flat is None:
         Y_flat, v, h = preprocess_for_pca(Y, fix_heading, **kwargs)
 
-    x = slds.init_continuous_stateseqs(Y_flat, params['Cd'])
+    x = slds.init_continuous_stateseqs(Y_flat, params["Cd"])
     states = arhmm.init_states(seed, x, mask, params)
-    
-    states['x'] = x
-    states['v'] = v
-    states['h'] = h
-    states['s'] = resample_scales(seed, Y, **states, **params,
-                                  s_0=noise_prior, **obs_hypparams)
-    return states  
+
+    states["x"] = x
+    states["v"] = v
+    states["h"] = h
+    states["s"] = resample_scales(
+        seed, Y, **states, **params, s_0=noise_prior, **obs_hypparams
+    )
+    return states
 
 
-def init_params(seed, pca, Y_flat, mask, trans_hypparams,
-                ar_hypparams, whiten, k, **kwargs):
+def init_params(
+    seed, pca, Y_flat, mask, trans_hypparams, ar_hypparams, whiten, k, **kwargs
+):
     """
     Initialize the parameters of the keypoint SLDS from the
     data and hyperparameters.
-    
+
     Parameters
     ----------
     seed : jr.PRNGKey
         JAX random seed.
     pca : sklearn.decomposition._pca.PCA
         PCA object fit to observations.
     Y_flat : jax array of shape (N, T, (k - 1) * d)
@@ -84,85 +97,86 @@
         Autoregression hyperparameters.
     whiten : bool
         Whether to whiten PC's to initialize continuous latents.
     k : int
         Number of keypoints.
     **kwargs : dict
         Overflow, for convenience.
-        
+
     Returns
     -------
     params : dict
         Values for each model parameter.
     """
     params = arhmm.init_params(seed, trans_hypparams, ar_hypparams)
-    params['Cd'] = slds.init_obs_params(pca, Y_flat, mask, whiten, **ar_hypparams)
-    params['sigmasq'] = jnp.ones(k)
+    params["Cd"] = slds.init_obs_params(
+        pca, Y_flat, mask, whiten, **ar_hypparams
+    )
+    params["sigmasq"] = jnp.ones(k)
     return params
 
 
-def init_hyperparams(trans_hypparams, ar_hypparams,
-                     obs_hypparams, cen_hypparams, **kwargs):
+def init_hyperparams(
+    trans_hypparams, ar_hypparams, obs_hypparams, cen_hypparams, **kwargs
+):
     """
     Formats the hyperparameter dictionary of the keypoint SLDS.
-    
+
     Parameters
     ----------
     trans_hypparams : dict
         HDP transition hyperparameters.
     ar_hypparams : dict
         Autoregression hyperparameters.
     obs_hypparams : dict
         Observation hyperparameters.
     cen_hypparams : dict
         Centroid movement hyperparameters.
     **kwargs : dict
         Overflow, for convenience.
-        
+
     Returns
     -------
     hypparams : dict
         Values for each group of hyperparameters.
     """
-    hyperparams = slds.init_hyperparams(trans_hypparams,
-                                        ar_hypparams,
-                                        obs_hypparams)
-    hyperparams['cen_hypparams'] = cen_hypparams.copy()
+    hyperparams = slds.init_hyperparams(
+        trans_hypparams, ar_hypparams, obs_hypparams
+    )
+    hyperparams["cen_hypparams"] = cen_hypparams.copy()
     return hyperparams
 
 
-def init_model(data=None,
-               states=None,
-               params=None,
-               hypparams=None,
-               noise_prior=None,
-               seed=jr.PRNGKey(0),
-               
-               pca=None,
-               whiten=True,
-               PCA_fitting_num_frames=1000000,
-               anterior_idxs=None,
-               posterior_idxs=None,
-               conf_threshold=.5,
-               
-               error_estimator=None,
-               
-               trans_hypparams=None,
-               ar_hypparams=None,
-               obs_hypparams=None,
-               cen_hypparams=None,
-               
-               verbose=False,
-               exclude_outliers_for_pca=True,
-               fix_heading=False,
-               **kwargs):
+def init_model(
+    data=None,
+    states=None,
+    params=None,
+    hypparams=None,
+    noise_prior=None,
+    seed=jr.PRNGKey(0),
+    pca=None,
+    whiten=True,
+    PCA_fitting_num_frames=1000000,
+    anterior_idxs=None,
+    posterior_idxs=None,
+    conf_threshold=0.5,
+    error_estimator=None,
+    trans_hypparams=None,
+    ar_hypparams=None,
+    obs_hypparams=None,
+    cen_hypparams=None,
+    verbose=False,
+    exclude_outliers_for_pca=True,
+    fix_heading=False,
+    **kwargs
+):
     """
     Initialize a keypoint SLDS model dict containing the
     hyperparameters, noise prior, and initial seed, states,
-    and parameters. 
+    and parameters.
 
     Parameters
     ----------
     data : dict, optional
         Data dictionary containing the observations, mask,
         and (optionally) confidences. Must be provided if ``states``
         or ``params`` not precomputed.
@@ -214,130 +228,182 @@
         Whether to print progress info during initialization.
     exclude_outliers_for_pca : bool, default=True
         Whether to exclude frames with low-confidence keypoints.
         If False, then the low-confidence keypoint coordinates are l
         inearly interpolated.
     fix_heading : bool, default=False
         Whether keep the heading angle of the pose fixed. If true,
-        the heading variable ``h`` is initialized as 0. 
+        the heading variable ``h`` is initialized as 0.
     **kwargs : dict, optional
         Unused. For convenience, enables user to invoke function
         by unpacking dict that contains keys not used by the method.
 
     Returns
     -------
     model : dict
         Dictionary containing the hyperparameters, noise prior,
         and initial seed, states, and parameters of the model.
-        
+
     Raises
     ------
     ValueError
         If the subset of the parameters provided by the caller
         is insufficient for model initialization.
     """
-    has_conf = data and ('conf' in data)
-    _check_init_args(data, states, params, hypparams,
-                     trans_hypparams, ar_hypparams,
-                     obs_hypparams, cen_hypparams,
-                     has_conf, noise_prior, error_estimator,
-                     anterior_idxs, posterior_idxs)
-    
+    has_conf = data and ("conf" in data)
+    _check_init_args(
+        data,
+        states,
+        params,
+        hypparams,
+        trans_hypparams,
+        ar_hypparams,
+        obs_hypparams,
+        cen_hypparams,
+        has_conf,
+        noise_prior,
+        error_estimator,
+        anterior_idxs,
+        posterior_idxs,
+    )
+
     model = {}
-    
-    if has_conf: conf = data['conf']
-    else: conf = None
+
+    if has_conf:
+        conf = data["conf"]
+    else:
+        conf = None
 
     if not (states and params):
-        Y, mask = data['Y'], data['mask']
+        Y, mask = data["Y"], data["mask"]
         Y_flat, v, h = preprocess_for_pca(
-            Y, anterior_idxs, posterior_idxs, conf, 
-            conf_threshold, fix_heading, verbose)
+            Y,
+            anterior_idxs,
+            posterior_idxs,
+            conf,
+            conf_threshold,
+            fix_heading,
+            verbose,
+        )
 
     if isinstance(seed, int):
         seed = jr.PRNGKey(seed)
-    model['seed'] = seed
+    model["seed"] = seed
 
     if hypparams is None:
-        if verbose: print('Keypoint SLDS: Initializing hyperparameters')
+        if verbose:
+            print("Keypoint SLDS: Initializing hyperparameters")
         hypparams = init_hyperparams(
-            trans_hypparams, ar_hypparams, obs_hypparams, cen_hypparams)
+            trans_hypparams, ar_hypparams, obs_hypparams, cen_hypparams
+        )
     else:
         hypparams = device_put_as_scalar(hypparams)
-    model['hypparams'] = hypparams
-    
+    model["hypparams"] = hypparams
+
     if noise_prior is None:
-        if verbose: print('Keypoint SLDS: Initializing noise prior')
-        if has_conf: noise_prior = estimate_error(conf, **error_estimator)
-        else: noise_prior = 1.    # TODO: magic number
-    else: 
+        if verbose:
+            print("Keypoint SLDS: Initializing noise prior")
+        if has_conf:
+            noise_prior = estimate_error(conf, **error_estimator)
+        else:
+            noise_prior = 1.0  # TODO: magic number
+    else:
         noise_prior = jax.device_put(noise_prior)
-    model['noise_prior'] = noise_prior
+    model["noise_prior"] = noise_prior
 
     if params is None:
-        if verbose: print('Keypoint SLDS: Initializing parameters')
+        if verbose:
+            print("Keypoint SLDS: Initializing parameters")
 
         if pca is None:
-            if not exclude_outliers_for_pca or conf is None: pca_mask = mask
-            else: pca_mask = jnp.logical_and(mask, (conf > conf_threshold).all(-1))
-            pca = utils.fit_pca(Y_flat, pca_mask, PCA_fitting_num_frames, verbose)
+            if not exclude_outliers_for_pca or conf is None:
+                pca_mask = mask
+            else:
+                pca_mask = jnp.logical_and(
+                    mask, (conf > conf_threshold).all(-1)
+                )
+            pca = utils.fit_pca(
+                Y_flat, pca_mask, PCA_fitting_num_frames, verbose
+            )
 
         params = init_params(
-            seed, pca, Y_flat, mask, **hypparams, whiten=whiten, k=Y.shape[-2])
-    
-    else: params = jax.device_put(params)
-    model['params'] = params
+            seed, pca, Y_flat, mask, **hypparams, whiten=whiten, k=Y.shape[-2]
+        )
+
+    else:
+        params = jax.device_put(params)
+    model["params"] = params
 
     if states is None:
         if verbose:
-            print('Keypoint SLDS: Initializing states')
-        obs_hypparams = hypparams['obs_hypparams']
-        states = init_states(seed, Y, mask, params, noise_prior,
-                             obs_hypparams, Y_flat, v, h, fix_heading)
+            print("Keypoint SLDS: Initializing states")
+        obs_hypparams = hypparams["obs_hypparams"]
+        states = init_states(
+            seed,
+            Y,
+            mask,
+            params,
+            noise_prior,
+            obs_hypparams,
+            Y_flat,
+            v,
+            h,
+            fix_heading,
+        )
     else:
         states = jax.device_put(states)
-    model['states'] = states
+    model["states"] = states
 
     return model
 
 
 def estimate_error(conf, slope, intercept):
     """
     Using the provided keypoint confidences and parameters
     learned from the noise calibration, returns prior on
     the noise for each datapoint.
-    
+
     Parameters
     ----------
     conf : jax array of shape (..., k)
         Confidence for each keypoint observation. Must be >= 0.
     slope : float
         Slope learned by noise calibration.
     intercept : float
         Intercept learned by noise calibration.
-        
+
     Returns
     -------
     noise_prior : jax array of shape (..., k)
         Prior on the noise for each observation.
     """
     return 10 ** (2 * (jnp.log10(conf + 1e-6) * slope + intercept))
 
 
 @check_precision
-def _check_init_args(data, states, params, hypparams,
-                     trans_hypparams, ar_hypparams,
-                     obs_hypparams, cen_hypparams,
-                     has_conf, noise_prior, error_estimator,
-                     anterior_idxs, posterior_idxs):
+def _check_init_args(
+    data,
+    states,
+    params,
+    hypparams,
+    trans_hypparams,
+    ar_hypparams,
+    obs_hypparams,
+    cen_hypparams,
+    has_conf,
+    noise_prior,
+    error_estimator,
+    anterior_idxs,
+    posterior_idxs,
+):
     """
-    Helper method for :py:func:`jax_moseq.models.initialize.init_model` 
-    that ensures a sufficient subset of the initialization arguments have 
+    Helper method for :py:func:`jax_moseq.models.initialize.init_model`
+    that ensures a sufficient subset of the initialization arguments have
     been provided by the caller.
-    
+
     Parameters
     ----------
     data : dict or None
         Data dictionary containing the observations, mask,
         and (optionally) confidences.
     states : dict or None
         State values for each latent variable.
@@ -359,35 +425,47 @@
         Prior on the noise for each keypoint observation.
     error_estimator : dict or None
         Parameters used to initialize ``noise_prior``.
     anterior_idxs : iterable of ints or None
         Anterior keypoint indices for heading initialization.
     posterior_idxs : iterable of ints or Nonne
         Posterior keypoint indices for heading initialization.
-        
+
     Raises
     ------
     ValueError
         If the subset of the parameters provided by the caller
         is insufficient for model initialization.
     """
     if not (data or (states and params)):
-        raise ValueError('Must provide either `data` or '
-                         'both `states` and `params`.')
-        
-    if not (hypparams or (trans_hypparams and
-                          ar_hypparams and
-                          obs_hypparams and
-                          cen_hypparams)):
-        raise ValueError('Must provide either `hypparams` or '
-                         'all of `trans_hypparams`, `ar_hypparams`, '
-                         '`obs_hypparams`, and `cen_hypparams`.')
-        
-    if has_conf and ((noise_prior is None) and
-                     (error_estimator is None)):
-        raise ValueError('If confidences are provided, must also provide'
-                         'either `error_estimator` or `noise_prior`.')
-        
-    if not (states and params) and (anterior_idxs is None or
-                                    posterior_idxs is None):
-        raise ValueError('If `states` and `params` not provided, must '
-                         'provide `anterior_idxs` and `posterior_idxs`.')
+        raise ValueError(
+            "Must provide either `data` or " "both `states` and `params`."
+        )
+
+    if not (
+        hypparams
+        or (
+            trans_hypparams
+            and ar_hypparams
+            and obs_hypparams
+            and cen_hypparams
+        )
+    ):
+        raise ValueError(
+            "Must provide either `hypparams` or "
+            "all of `trans_hypparams`, `ar_hypparams`, "
+            "`obs_hypparams`, and `cen_hypparams`."
+        )
+
+    if has_conf and ((noise_prior is None) and (error_estimator is None)):
+        raise ValueError(
+            "If confidences are provided, must also provide "
+            "either `error_estimator` or `noise_prior`."
+        )
+
+    if not (states and params) and (
+        anterior_idxs is None or posterior_idxs is None
+    ):
+        raise ValueError(
+            "If `states` and `params` not provided, must "
+            "provide `anterior_idxs` and `posterior_idxs`."
+        )
```

### Comparing `jax-moseq-0.0.3/jax_moseq/models/keypoint_slds/log_prob.py` & `jax-moseq-0.0.5/jax_moseq/models/keypoint_slds/log_prob.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,41 +6,41 @@
 from jax_moseq.models.keypoint_slds.alignment import estimate_coordinates
 
 na = jnp.newaxis
 
 
 def location_log_prob(v, sigmasq_loc):
     """
-    Calculate the log probability of the centroid location at each 
+    Calculate the log probability of the centroid location at each
     time-step, given the prior on centroid movement.
-    
+
     Parameters
     ----------
     v : jax array of shape (..., T, d)
         Centroid positions.
     sigmasq_loc : float
         Assumed variance in centroid displacements.
-   
+
     Returns
     -------
     log_pv: jax array of shape (..., T - 1)
         Log probability of `v`.
     """
     v0 = v[..., :-1, :]
     v1 = v[..., 1:, :]
-    sigma = jnp.sqrt(sigmasq_loc)
-    return tfd.MultivariateNormalDiag(v0, None, sigma).log_prob(v1)
+    sigma = jnp.sqrt(sigmasq_loc) * jnp.ones_like(v0)
+    return tfd.MultivariateNormalDiag(v0, sigma).log_prob(v1)
 
 
 def obs_log_prob(Y, x, v, h, s, Cd, sigmasq, **kwargs):
     """
     Calculate the log probability of keypoint coordinates at each
     time-step, given continuous latent trajectories, centroids, heading
     angles, noise scales, and observation parameters.
-    
+
     Parameters
     ----------
     Y : jax array of shape (..., k, d)
         Keypoint observations.
     x : jax array of shape (..., latent_dim)
         Latent trajectories.
     v : jax array of shape (..., d)
@@ -51,28 +51,44 @@
         Noise scales.
     Cd : jax array of shape ((k - 1) * d, latent_dim + 1)
         Observation transform.
     sigmasq : jax_array of shape k
         Unscaled noise.
     **kwargs : dict
         Overflow, for convenience.
-    
+
     Returns
     -------
     log_pY: jax array of shape (..., k)
         Log probability of `Y`.
     """
     Y_bar = estimate_coordinates(x, v, h, Cd)
-    sigma = jnp.sqrt(s * sigmasq)
-    return tfd.MultivariateNormalDiag(Y_bar, None, sigma).log_prob(Y)
+    sigma = jnp.broadcast_to(jnp.sqrt(s * sigmasq)[..., na], Y.shape)
+    return tfd.MultivariateNormalDiag(Y_bar, sigma).log_prob(Y)
 
 
 @jax.jit
-def log_joint_likelihood(Y, mask, x, v, h, s, z, pi, Ab, Q, Cd,
-                         sigmasq, sigmasq_loc, s_0, nu_s, **kwargs):
+def log_joint_likelihood(
+    Y,
+    mask,
+    x,
+    v,
+    h,
+    s,
+    z,
+    pi,
+    Ab,
+    Q,
+    Cd,
+    sigmasq,
+    sigmasq_loc,
+    s_0,
+    nu_s,
+    **kwargs
+):
     """
     Calculate the total log probability for each latent state.
 
     Parameters
     ----------
     Y : jax array of shape (..., T, k, d)
         Keypoint observations.
@@ -115,24 +131,24 @@
     """
     ll = arhmm.log_joint_likelihood(x, mask, z, pi, Ab, Q)
 
     log_pY = obs_log_prob(Y, x, v, h, s, Cd, sigmasq)
     log_ps = slds.scale_log_prob(s, s_0, nu_s)
     log_pv = location_log_prob(v, sigmasq_loc)
 
-    ll['Y'] = (log_pY * mask[..., na]).sum()
-    ll['s'] = (log_ps * mask[..., na]).sum()
-    ll['v'] = (log_pv * mask[...,1:]).sum()
+    ll["Y"] = (log_pY * mask[..., na]).sum()
+    ll["s"] = (log_ps * mask[..., na]).sum()
+    ll["v"] = (log_pv * mask[..., 1:]).sum()
     return ll
 
 
 def model_likelihood(data, states, params, hypparams, noise_prior, **kwargs):
     """
     Convenience class that invokes `log_joint_likelihood`.
-    
+
     Parameters
     ----------
     data : dict
         Data dictionary containing the observations and mask.
     states : dict
         State values for each latent variable.
     params : dict
@@ -146,11 +162,15 @@
 
     Returns
     ------
     ll : dict
         Dictionary mapping state variable name to its
         total log probability.
     """
-    return log_joint_likelihood(**data, **states, **params,
-                                **hypparams['obs_hypparams'],
-                                **hypparams['cen_hypparams'],
-                                s_0=noise_prior)
+    return log_joint_likelihood(
+        **data,
+        **states,
+        **params,
+        **hypparams["obs_hypparams"],
+        **hypparams["cen_hypparams"],
+        s_0=noise_prior
+    )
```

### Comparing `jax-moseq-0.0.3/jax_moseq/models/slds/gibbs.py` & `jax-moseq-0.0.5/jax_moseq/models/slds/gibbs.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,88 +1,166 @@
 import jax
 import jax.numpy as jnp
 import jax.random as jr
+from functools import partial
 
-from jax_moseq.utils import apply_affine, nan_check
-from jax_moseq.utils.distributions import sample_scaled_inv_chi2
 from jax_moseq.utils.kalman import kalman_sample, ar_to_lds
-
+from jax_moseq.utils import mixed_map, apply_affine
 from jax_moseq.models import arhmm
 
 na = jnp.newaxis
 
-@nan_check
-@jax.jit
-def resample_continuous_stateseqs(seed, Y, mask, z, s, Ab,
-                                  Q, Cd, sigmasq, **kwargs):
-    """
-    Resamples the latent trajectories `x`.
+
+@partial(jax.jit, static_argnames=("parallel_message_passing",))
+def resample_continuous_stateseqs(
+    seed,
+    y,
+    mask,
+    z,
+    s,
+    Ab,
+    Q,
+    Cd,
+    sigmasq,
+    jitter=1e-3,
+    parallel_message_passing=True,
+    **kwargs
+):
+    """Resample the latent trajectories `x`.
 
     Parameters
     ----------
     seed : jr.PRNGKey
         JAX random seed.
-    Y : jax array of shape (N, T, obs_dim)
+    y : jax.Array of shape (n_recordings, n_timesteps, obs_dim)
         Observations.
-    mask : jax array of shape (N, T)
-        Binary indicator for valid frames.
-    z : jax_array of shape (N, T - n_lags)
-        Discrete state sequences.
-    s : jax array of shape (N, T, obs_dim)
-        Noise scales.
-    Ab : jax array of shape (num_states, latent_dim, ar_dim)
-        Autoregressive transforms.
-    Q : jax array of shape (num_states, latent_dim, latent_dim)
+    mask : jax.Array of shape (n_recordings, n_timesteps)
+        Binary indicator, 1=valid frames, 0=invalid frames.
+    z : jax.Array of shape (n_recordings, n_timesteps-n_lags)
+        Discrete state sequences, taking integer values between [0, n_states),
+        for timesteps [n_lags, n_timesteps),
+    s : jax.Array of shape (n_recordings, n_timesteps, obs_dim)
+        Observation noise scales.
+    Ab : jax.Array of shape (n_states, latent_dim, ar_dim + 1)
+        Autoregressive dynamics and bias, where `ar_dim = latent_dim * n_lags`
+    Q : jax.Array of shape (n_states, latent_dim, latent_dim)
         Autoregressive noise covariances.
-    Cd : jax array of shape (obs_dim, latent_dim + 1)
-        Observation transform.
-    sigmasq : jax_array of shape obs_dim
+    Cd : jax.Array of shape (obs_dim, latent_dim + 1)
+        Affine transform from `latent_dim` to `state_dim`
+    sigmasq : jax.Array of shape (obs_dim,)
         Unscaled noise.
+    jitter : float, default=1e-3
+        Amount to boost the diagonal of the covariance matrix
+        during backward-sampling of the continuous states.
+    parallel_message_passing : bool, default=True,
+        Use associative scan for Kalman sampling, which is faster on
+        a GPU but has a significantly longer jit time.
     **kwargs : dict
         Overflow, for convenience.
 
     Returns
     ------
-    x : jax array of shape (N, T, latent_dim)
-        Latent trajectories.
+    x : jax.Array of shape (n_recordings, n_timesteps, latent_dim)
+        Posterior sample of latent trajectories.
     """
-    n = Y.shape[0]    # num sessions
-    d = Ab.shape[1]   # latent dim
-    nlags = Ab.shape[2] // d
-    
-    # 0. spawn random seed for each session
-    rng = jr.split(seed, n)
-    
-    # 1. Format the time varying parameters
-    y = Y[:, nlags-1:]   # first n_lags frames cannot be assigned syllable
-    mask = mask[:,nlags-1:-1]
-    R = sigmasq * s[:, nlags - 1:]    # scale learned uncertainties
-    
-    # 2. Reformat the dynamics parameters
+    n_recordings, latent_dim, obs_dim = y.shape[0], Ab.shape[1], y.shape[-1]
+    n_lags = Ab.shape[2] // latent_dim
+
+    # TODO Parameterize these distributional hyperparameter
+    init_dynamics_mean = jnp.zeros(latent_dim * n_lags)
+    init_dynamics_cov = 10 * jnp.eye(
+        latent_dim * n_lags
+    )  # TODO: hard coded constant 10
+    masked_dynamics_noise = 10
+    masked_obs_noise = 10
+
+    # =====================================================================
+    # 1. Omit the first L frames of observations and associated sequences
+    # =====================================================================
+    y_ = y[:, n_lags - 1 :]
+    mask_ = mask[:, n_lags - 1 :]
+
+    # Scale unscaled observations by fitted diagonal scales
+    R_ = sigmasq * s[:, n_lags - 1 :]
+
+    # ==========================================================================
+    # 2. Reformat L'th-order AR dynamics in R^D to 1st-order dynamics in R^{DL}
+    # ==========================================================================
     A_, b_, Q_, C_, d_ = ar_to_lds(Ab, Q, Cd)
-    
-    # 3. Initialize the kalman latent estimates
-    mu0 = jnp.zeros(d * nlags)
-    S0 = 10 * jnp.eye(d * nlags) # TODO: hard coded constant 10
-    
-    # 4. Apply vectorized Kalman sample to each session
-    in_axes = (0,0,0,0,na,na,na,na,na,na,na,0)
-    x = jax.vmap(kalman_sample, in_axes)(
-        rng, y, mask, z, mu0, S0,
-        A_, b_, Q_, C_, d_, R
+
+    # =============================================
+    # 3. Formulate parameters for masked timesteps
+    # =============================================
+    ar_dim = latent_dim * n_lags
+
+    # If masked, hold the last state, i.e. set dynamics for "unlagged" states to
+    # identity matrix and all other state dynamics to 0
+    eye_zero_order = jnp.zeros((ar_dim, ar_dim))
+    eye_zero_order = eye_zero_order.at[-latent_dim:, -latent_dim:].set(
+        jnp.eye(latent_dim)
+    )
+
+    masked_dynamics_params = {
+        "weights": eye_zero_order,
+        "bias": jnp.zeros(ar_dim),
+        "cov": jnp.eye(ar_dim) * masked_dynamics_noise,
+    }
+    masked_obs_noise_diag = jnp.ones(obs_dim) * masked_obs_noise
+
+    # ==================================================
+    # 4. Apply vectorized Kalman sample to each recording
+    # Shapes of time-varying parameters going into the Kalman sampler are
+    #   ys:     (n_timesteps-n_lags+1, obs_dim), corresponding to timesteps  [L-1, T)
+    #   mask:   (n_timesteps-n_lags+1,)
+    #   zs:     (n_timesteps-n_lags,), corresponding to timesteps [L, T]
+    #   Rs:     (n_timesteps-n_lags+1, obs_dim)
+    # ==================================================
+    in_axes = (0, 0, 0, 0, na, na, na, na, na, na, na, 0, na, na)
+    x = mixed_map(
+        partial(
+            kalman_sample, jitter=jitter, parallel=parallel_message_passing
+        ),
+        in_axes,
+    )(
+        jr.split(seed, n_recordings),
+        y_,
+        mask_,
+        z,
+        init_dynamics_mean,
+        init_dynamics_cov,
+        A_,
+        b_,
+        Q_,
+        C_,
+        d_,
+        R_,
+        masked_dynamics_params,
+        masked_obs_noise_diag,
+    )
+
+    # =========================================================================
+    # 5. Reformat sampled trajectories back into L'th order AR dynamics in R^D
+    # =========================================================================
+    x = jnp.concatenate(
+        [
+            x[:, 0, : (n_lags - 1) * latent_dim].reshape(
+                -1, n_lags - 1, latent_dim
+            ),
+            x[:, :, -latent_dim:],
+        ],
+        axis=1,
     )
 
-    # 5. Reformat back into AR space 
-    x = jnp.concatenate([x[:, 0, :-d].reshape(-1, nlags-1 ,d), x[:,:,-d:]],axis=1)
     return x
 
 
 @jax.jit
-def resample_obs_variance(seed, Y, mask, x, s, Cd,
-                          nu_sigma, sigmasq_0, **kwargs):
+def resample_obs_variance(
+    seed, Y, mask, x, s, Cd, nu_sigma, sigmasq_0, **kwargs
+):
     """
     Resample the observation variance `sigmasq`.
 
     Parameters
     ----------
     seed : jr.PRNGKey
         JAX random seed.
@@ -104,21 +182,24 @@
         Overflow, for convenience.
 
     Returns
     ------
     sigmasq : jax_array of shape obs_dim
         Unscaled noise.
     """
-    sqerr = compute_squared_error(seed, Y, x, Cd, mask)
-    return resample_obs_variance_from_sqerr(seed, sqerr, mask, s, nu_sigma, sigmasq_0)
+    sqerr = compute_squared_error(Y, x, Cd, mask)
+    return resample_obs_variance_from_sqerr(
+        seed, sqerr, mask, s, nu_sigma, sigmasq_0
+    )
 
 
 @jax.jit
-def resample_obs_variance_from_sqerr(seed, sqerr, mask, s, nu_sigma,
-                                     sigmasq_0, **kwargs):
+def resample_obs_variance_from_sqerr(
+    seed, sqerr, mask, s, nu_sigma, sigmasq_0, **kwargs
+):
     """
     Resample the observation variance `sigmasq` using the
     squared error between predicted and true observations.
 
     Parameters
     ----------
     seed : jr.PRNGKey
@@ -138,24 +219,23 @@
 
     Returns
     ------
     sigmasq : jax_array of shape obs_dim
         Unscaled noise.
     """
     degs = nu_sigma + 3 * mask.sum()
-    
+
     k = sqerr.shape[-1]
-    S_y = (sqerr / s).reshape(-1, k).sum(0)    # (..., k) -> k
+    S_y = (sqerr / s).reshape(-1, k).sum(0)  # (..., k) -> k
     variance = nu_sigma * sigmasq_0 + S_y
     return _resample_spread(seed, degs, variance)
 
 
 @jax.jit
-def resample_scales(seed, Y, x, Cd, sigmasq,
-                    nu_s, s_0, **kwargs):
+def resample_scales(seed, Y, x, Cd, sigmasq, nu_s, s_0, **kwargs):
     """
     Resample the scale values `s`.
 
     Parameters
     ----------
     seed : jr.PRNGKey
         JAX random seed.
@@ -175,21 +255,20 @@
         Overflow, for convenience.
 
     Returns
     ------
     s : jax array of shape (N, T, obs_dim)
         Noise scales.
     """
-    sqerr = compute_squared_error(seed, Y, x, Cd)
+    sqerr = compute_squared_error(Y, x, Cd)
     return resample_scales_from_sqerr(seed, sqerr, sigmasq, nu_s, s_0)
 
 
 @jax.jit
-def resample_scales_from_sqerr(seed, sqerr, sigmasq,
-                               nu_s, s_0, **kwargs):
+def resample_scales_from_sqerr(seed, sqerr, sigmasq, nu_s, s_0, **kwargs):
     """
     Resample the scale values `s` using the squared
     error between predicted and true observations.
 
     Parameters
     ----------
     seed : jr.PRNGKey
@@ -216,15 +295,15 @@
 
 
 @jax.jit
 def _resample_spread(seed, degs, variance):
     """
     Resample the noise values from the computed
     degrees of freedom and variance.
-    
+
     Parameters
     ----------
     seed : jr.PRNGKey
         JAX random seed.
     degs : scalar
         Chi-squared degrees of freedom.
     variance : jax array
@@ -236,23 +315,21 @@
         Resampled noise values.
     """
     # same as sample_scaled_inv_chi2(seed, degs, variance / degs)
     return variance / jr.gamma(seed, degs / 2, shape=variance.shape) / 2
 
 
 @jax.jit
-def compute_squared_error(seed, Y, x, Cd, mask=None):
+def compute_squared_error(Y, x, Cd, mask=None):
     """
     Computes the squared error between model predicted
     and true observations.
 
     Parameters
     ----------
-    seed : jr.PRNGKey
-        JAX random seed.
     Y : jax array of shape (..., obs_dim)
         Observations.
     x : jax array of shape (..., latent_dim)
         Latent trajectories.
     Cd : jax array of shape (obs_dim, latent_dim + 1)
         Observation transform.
     mask : jax array of shape (...), optional
@@ -261,23 +338,32 @@
     Returns
     ------
     sqerr : jax array of shape (..., obs_dim)
         Squared error between model predicted and
         true observations.
     """
     Y_bar = apply_affine(x, Cd)
-    sqerr = ((Y - Y_bar) ** 2)
+    sqerr = (Y - Y_bar) ** 2
     if mask is not None:
         sqerr = mask[..., na] * sqerr
     return sqerr
 
 
-def resample_model(data, seed, states, params, hypparams, 
-                   ar_only=False, states_only=False,
-                   skip_noise=False, **kwargs):
+def resample_model(
+    data,
+    seed,
+    states,
+    params,
+    hypparams,
+    ar_only=False,
+    states_only=False,
+    skip_noise=True,
+    parallel_message_passing=False,
+    **kwargs
+):
     """
     Resamples the SLDS model given the hyperparameters, data,
     current states, and current parameters.
 
     Parameters
     ----------
     data : dict
@@ -290,44 +376,55 @@
         Values for each model parameter.
     hypparams : dict
         Values for each group of hyperparameters.
     ar_only : bool, default=False
         Whether to restrict sampling to ARHMM components.
     states_only : bool, default=False
         Whether to restrict sampling to states.
-    skip_noise : bool, default=False
+    skip_noise : bool, default=True
         Whether to exclude `sigmasq` and `s` from resampling.
+    parallel_message_passing : bool, default=True,
+        Use associative scan for Kalman sampling, which is faster on
+        a GPU but has a significantly longer jit time.
     **kwargs : dict
         Overflow, for convenience.
 
     Returns
     ------
     model : dict
         Dictionary containing the hyperparameters and
         updated seed, states, and parameters of the model.
     """
-    model = arhmm.resample_model(data, seed, states, params,
-                                 hypparams, states_only)
+    model = arhmm.resample_model(
+        data, seed, states, params, hypparams, states_only
+    )
     if ar_only:
         return model
-    
-    seed = model['seed']
-    params = model['params'].copy()
-    states = model['states'].copy()
-    
+
+    seed = model["seed"]
+    params = model["params"].copy()
+    states = model["states"].copy()
+
     if not (states_only or skip_noise):
-        params['sigmasq'] = resample_obs_variance(
-            seed, **data, **states, **params, 
-            **hypparams['obs_hypparams'])
-        
-    states['x'] = resample_continuous_stateseqs(
-        seed, **data, **states, **params)
+        params["sigmasq"] = resample_obs_variance(
+            seed, **data, **states, **params, **hypparams["obs_hypparams"]
+        )
+
+    states["x"] = resample_continuous_stateseqs(
+        seed,
+        **data,
+        **states,
+        **params,
+        parallel_message_passing=parallel_message_passing
+    )
 
     if not skip_noise:
-        states['s'] = resample_scales(
-            seed, **data, **states, **params, 
-            **hypparams['obs_hypparams'])
-        
-    return {'seed': seed,
-            'states': states, 
-            'params': params, 
-            'hypparams': hypparams}
+        states["s"] = resample_scales(
+            seed, **data, **states, **params, **hypparams["obs_hypparams"]
+        )
+
+    return {
+        "seed": seed,
+        "states": states,
+        "params": params,
+        "hypparams": hypparams,
+    }
```

### Comparing `jax-moseq-0.0.3/jax_moseq/models/slds/initialize.py` & `jax-moseq-0.0.5/jax_moseq/models/slds/initialize.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 import jax
 import jax.numpy as jnp
 import jax.random as jr
 import numpy as np
 
-from jax_moseq.utils import jax_io, device_put_as_scalar, fit_pca, check_precision
+from jax_moseq.utils import (
+    jax_io,
+    device_put_as_scalar,
+    fit_pca,
+    check_precision,
+)
 
 from jax_moseq.models import arhmm
 from jax_moseq.models.slds.gibbs import resample_scales
 
 na = jnp.newaxis
 
 
@@ -26,64 +31,63 @@
         Binary indicator for valid frames.
     whiten : bool
         Whether to whiten PC's to initialize continuous latents.
     latent_dim : int
         Dimensionality of continuous latents.
     **kwargs : dict
         Overflow, for convenience.
-        
+
     Returns
     -------
     Cd : jax array of shape (obs_dim, latent_dim + 1)
         Observation transform.
     """
     C = jnp.array(pca.components_[:latent_dim])
     d = jnp.array(pca.mean_)
 
     if whiten:
         Y_flat = Y[mask > 0]
         latents_flat = jax_io(pca.transform)(Y_flat)[:, :latent_dim]
         cov = jnp.cov(latents_flat.T)
         W = jnp.linalg.cholesky(cov)
         C = W.T @ C
-        
+
     Cd = jnp.hstack([C.T, d[:, na]])
     return Cd
 
 
 def init_continuous_stateseqs(Y, Cd, **kwargs):
     """
     Initialize the continuous latents by applying
     the inverse of the emission transform to the data.
-    
+
     Parameters
     ----------
     Y : jax array of shape (N, T, obs_dim)
         Observations.
     Cd : jax array of shape (obs_dim, latent_dim + 1)
         Observation transform.
     **kwargs : dict
         Overflow, for convenience.
-    
+
     Returns
     -------
     x : jax array of shape (N, T, latent_dim)
         Latent trajectories.
     """
     C, d = Cd[:, :-1], Cd[:, -1]
     C_inv = jnp.array(np.linalg.pinv(C))
     return (Y - d) @ C_inv.T
 
 
-def init_states(seed, Y, mask, params,
-                obs_hypparams, **kwargs):
+def init_states(seed, Y, mask, params, obs_hypparams, **kwargs):
     """
     Initialize the latent states of the SLDS from the data,
     parameters, and hyperparameters.
-    
+
     Parameters
     ----------
     seed : jr.PRNGKey
         JAX random seed.
     Y : jax array of shape (N, T, obs_dim)
         Observations.
     mask : jax array of shape (N, T)
@@ -96,30 +100,31 @@
         Overflow, for convenience.
 
     Returns
     -------
     states : dict
         State values for each latent variable.
     """
-    x = init_continuous_stateseqs(Y, params['Cd'])
+    x = init_continuous_stateseqs(Y, params["Cd"])
     s = resample_scales(seed, Y, x, **params, **obs_hypparams)
 
     # initialize arhmm to get discrete latents
     states = arhmm.init_states(seed, x, mask, params)
-    states['x'] = x
-    states['s'] = s
-    return states  
+    states["x"] = x
+    states["s"] = s
+    return states
 
 
-def init_params(seed, pca, Y, mask, trans_hypparams,
-                ar_hypparams, whiten, **kwargs):
+def init_params(
+    seed, pca, Y, mask, trans_hypparams, ar_hypparams, whiten, **kwargs
+):
     """
     Initialize the parameters of the SLDS from the
     data and hyperparameters.
-    
+
     Parameters
     ----------
     seed : jr.PRNGKey
         JAX random seed.
     pca : sklearn.decomposition._pca.PCA
         PCA object fit to observations.
     Y : jax array of shape (N, T, obs_dim)
@@ -138,66 +143,63 @@
     Returns
     -------
     params : dict
         Values for each model parameter.
     """
     params = arhmm.init_params(seed, trans_hypparams, ar_hypparams)
 
-    latent_dim = ar_hypparams['latent_dim']
-    params['Cd'] = init_obs_params(pca, Y, mask, whiten, latent_dim)
-    params['sigmasq'] = jnp.ones(Y.shape[-1])    # TODO
+    latent_dim = ar_hypparams["latent_dim"]
+    params["Cd"] = init_obs_params(pca, Y, mask, whiten, latent_dim)
+    params["sigmasq"] = jnp.ones(Y.shape[-1])  # TODO
     return params
 
 
-def init_hyperparams(trans_hypparams, ar_hypparams,
-                     obs_hypparams, **kwargs):
+def init_hyperparams(trans_hypparams, ar_hypparams, obs_hypparams, **kwargs):
     """
     Formats the hyperparameter dictionary of the SLDS.
 
     Parameters
     ----------
     trans_hypparams : dict
         HDP transition hyperparameters.
     ar_hypparams : dict
         Autoregression hyperparameters.
     obs_hypparams : dict
         Observation hyperparameters.
     **kwargs : dict
         Overflow, for convenience.
-        
+
     Returns
     -------
     hypparams : dict
         Values for each group of hyperparameters.
     """
-    hyperparams = arhmm.init_hyperparams(trans_hypparams,
-                                         ar_hypparams)
-    hyperparams['obs_hypparams'] = obs_hypparams.copy()
+    hyperparams = arhmm.init_hyperparams(trans_hypparams, ar_hypparams)
+    hyperparams["obs_hypparams"] = obs_hypparams.copy()
     return hyperparams
 
 
-def init_model(data=None,
-               states=None,
-               params=None,
-               hypparams=None,
-               seed=jr.PRNGKey(0),
-               
-               pca=None,
-               whiten=True,
-               PCA_fitting_num_frames=1000000,
-               
-               trans_hypparams=None,
-               ar_hypparams=None,
-               obs_hypparams=None,
-               
-               verbose=False,
-               **kwargs):
+def init_model(
+    data=None,
+    states=None,
+    params=None,
+    hypparams=None,
+    seed=jr.PRNGKey(0),
+    pca=None,
+    whiten=True,
+    PCA_fitting_num_frames=1000000,
+    trans_hypparams=None,
+    ar_hypparams=None,
+    obs_hypparams=None,
+    verbose=False,
+    **kwargs
+):
     """
     Initialize a SLDS model dict containing the hyperparameters,
-    noise prior, and initial seed, states, and parameters. 
+    noise prior, and initial seed, states, and parameters.
 
     Parameters
     ----------
     data : dict, optional
         Data dictionary containing the observations, mask,
         and (optionally) confidences. Must be provided if `states`
         or `params` not precomputed.
@@ -233,72 +235,85 @@
         by unpacking dict that contains keys not used by the method.
 
     Returns
     -------
     model : dict
         Dictionary containing the hyperparameters, noise prior,
         and initial seed, states, and parameters of the model.
-        
+
     Raises
     ------
     ValueError
         If the subset of the parameters provided by the caller
         is insufficient for model initialization.
     """
-    _check_init_args(data, states, params,
-                     hypparams, trans_hypparams,
-                     ar_hypparams, obs_hypparams)
-    
+    _check_init_args(
+        data,
+        states,
+        params,
+        hypparams,
+        trans_hypparams,
+        ar_hypparams,
+        obs_hypparams,
+    )
+
     model = {}
-    
+
     if not (states and params):
-        Y, mask = data['Y'], data['mask']
+        Y, mask = data["Y"], data["mask"]
 
     if isinstance(seed, int):
         seed = jr.PRNGKey(seed)
-    model['seed'] = seed
+    model["seed"] = seed
 
     if hypparams is None:
         if verbose:
-            print('SLDS: Initializing hyperparameters')
-        hypparams = init_hyperparams(trans_hypparams,
-                                     ar_hypparams,
-                                     obs_hypparams)
+            print("SLDS: Initializing hyperparameters")
+        hypparams = init_hyperparams(
+            trans_hypparams, ar_hypparams, obs_hypparams
+        )
     else:
         hypparams = device_put_as_scalar(hypparams)
-    model['hypparams'] = hypparams
-        
+    model["hypparams"] = hypparams
+
     if params is None:
         if verbose:
-            print('SLDS: Initializing parameters')
+            print("SLDS: Initializing parameters")
         if pca is None:
             pca = fit_pca(Y, mask, PCA_fitting_num_frames, verbose)
-        params = init_params(seed, pca, Y, mask,
-                             **hypparams, whiten=whiten)
+        params = init_params(seed, pca, Y, mask, **hypparams, whiten=whiten)
     else:
         params = jax.device_put(params)
-    model['params'] = params
+    model["params"] = params
 
     if states is None:
         if verbose:
-            print('SLDS: Initializing states')
+            print("SLDS: Initializing states")
         states = init_states(seed, Y, mask, params, **hypparams)
     else:
         states = jax.device_put(states)
-    model['states'] = states
+    model["states"] = states
 
     return model
 
+
 @check_precision
-def _check_init_args(data, states, params, hypparams,
-                     trans_hypparams, ar_hypparams, obs_hypparams):
+def _check_init_args(
+    data,
+    states,
+    params,
+    hypparams,
+    trans_hypparams,
+    ar_hypparams,
+    obs_hypparams,
+):
     """
     Helper method for `init_model` that ensures a sufficient subset
     of the initialization arguments have been provided by the caller.
-    
+
     Parameters
     ----------
     data : dict or None
         Data dictionary containing the observations, mask,
         and (optionally) confidences.
     states : dict or None
         State values for each latent variable.
@@ -308,24 +323,25 @@
         Values for each group of hyperparameters.
     trans_hypparams : dict or None
         HDP transition hyperparameters.
     ar_hypparams : dict or None
         Autoregression hyperparameters.
     obs_hypparams : dict or None
         Observation hyperparameters.
-        
+
     Raises
     ------
     ValueError
         If the subset of the parameters provided by the caller
         is insufficient for model initialization.
     """
     if not (data or (states and params)):
-        raise ValueError('Must provide either `data` or '
-                         'both `states` and `params`.')
-        
-    if not (hypparams or (trans_hypparams and
-                          ar_hypparams and
-                          obs_hypparams)):
-        raise ValueError('Must provide either `hypparams` or '
-                         'all of `trans_hypparams`, `ar_hypparams`, '
-                         'and `obs_hypparams`.')
+        raise ValueError(
+            "Must provide either `data` or " "both `states` and `params`."
+        )
+
+    if not (hypparams or (trans_hypparams and ar_hypparams and obs_hypparams)):
+        raise ValueError(
+            "Must provide either `hypparams` or "
+            "all of `trans_hypparams`, `ar_hypparams`, "
+            "and `obs_hypparams`."
+        )
```

### Comparing `jax-moseq-0.0.3/jax_moseq/utils/autoregression.py` & `jax-moseq-0.0.5/jax_moseq/utils/autoregression.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,28 +23,28 @@
     x = x[..., nlags:, :]
     return tfd.MultivariateNormalFullCovariance(mu, Q).log_prob(x)
 
 
 def get_lags(x, nlags):
     """
     Get lags of a multivariate time series. Lags are concatenated along
-    the last dim in time-order. 
+    the last dim in time-order.
 
     Parameters
-    ----------  
+    ----------
     nlags: int
         Number of lags
-        
+
     x: jax array, shape (..., t, d)
-        Batch of d-dimensional time series 
-    
+        Batch of d-dimensional time series
+
     Returns
     -------
     x_lagged: jax array, shape (..., t-nlags, d*nlags)
 
     """
     lags = [jnp.roll(x, t, axis=-2) for t in range(1, nlags + 1)]
     return jnp.concatenate(lags[::-1], axis=-1)[..., nlags:, :]
 
 
 def get_nlags(Ab):
-    return Ab.shape[-1] // Ab.shape[-2]
+    return Ab.shape[-1] // Ab.shape[-2]
```

### Comparing `jax-moseq-0.0.3/jax_moseq/utils/debugging.py` & `jax-moseq-0.0.5/jax_moseq/utils/debugging.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,107 +3,114 @@
 import inspect
 import traceback
 import functools
 import contextlib
 import jax.numpy as jnp
 import numpy as np
 
-# JAX has its own implementation of `tree_flatten_with_path` 
-# but it's only in version of 0.4.6 or later, and currently 
+# JAX has its own implementation of `tree_flatten_with_path`
+# but it's only in version of 0.4.6 or later, and currently
 # some platforms (e.g. Windows) require installing < 0.4.6
 from optree import tree_flatten_with_path
 
 
-
 def _check_array_precision(arg, x64):
     """Checks if precision of `arg` matches `x64`"""
     permitted_dtypes = [
         (np.int64 if x64 else np.int32),
         (jnp.int64 if x64 else jnp.int32),
         (np.float64 if x64 else np.float32),
-        (jnp.float64 if x64 else jnp.float32)]
+        (jnp.float64 if x64 else jnp.float32),
+    ]
     if isinstance(arg, jnp.ndarray) or isinstance(arg, np.ndarray):
-        if not arg.dtype in permitted_dtypes:  return False   
+        if not arg.dtype in permitted_dtypes:
+            return False
     return True
 
+
 def check_precision(fn):
     """
     Decorator to check that the precision of the arguments matches the
     precision of the jax configuration.
     """
     arg_names = inspect.getfullargspec(fn).args
-   
+
     @functools.wraps(fn)
     def wrapper(*args, **kwargs):
         x64 = jax.config.x64_enabled
         args_with_wrong_precision = []
-        for name,arg in list(zip(arg_names,args)) + list(kwargs.items()):
+        for name, arg in list(zip(arg_names, args)) + list(kwargs.items()):
             check_fn = functools.partial(_check_array_precision, x64=x64)
             if not jax.tree_util.tree_all(jax.tree_map(check_fn, arg)):
                 args_with_wrong_precision.append(name)
-                
+
         if len(args_with_wrong_precision) > 0:
             msg = f'JAX is configured to use {"64" if x64 else "32"}-bit precision, '
             msg += f'but following arguments contain {"32" if x64 else "64"}-bit arrays: '
-            msg += ', '.join([f'"{name}"' for name in args_with_wrong_precision])
+            msg += ", ".join(
+                [f'"{name}"' for name in args_with_wrong_precision]
+            )
             msg += '. Either change the JAX config using `jax.config.update("jax_enable_x64", True/False)` '
-            msg += 'or convert the arguments to the correct precision using `jax_moseq.utils.utils.convert_data_precision`.'
+            msg += "or convert the arguments to the correct precision using `jax_moseq.utils.utils.convert_data_precision`."
             raise ValueError(msg)
 
         return fn(*args, **kwargs)
+
     return wrapper
 
 
 def convert_data_precision(data, x64=None):
     """
     Convert all numerical data in a pytree to the specified precision.
-    
-    Note that converting to 64-bit precision is only possible if 
+
+    Note that converting to 64-bit precision is only possible if
     ``jax.config.x64_enabled`` is ``True``. To update this setting, use
     ``jax.config.update('jax_enable_x64', True)``.
 
     Parameters
     ----------
     data: pytree (dict, list, tuple, array, or any nested combination thereof)
         The data to convert.
     x64: bool, default=None
         If ``x64=True``, convert to 64-bit precision. If ``x64=False``,
         convert to 32-bit precision. If ``x64=None``, infer the desired
-        precision from ``jax.config.x64_enabled``. 
+        precision from ``jax.config.x64_enabled``.
 
     Returns
     -------
     data: pytree
         The converted data.
     """
-    if x64 is None: x64 = jax.config.x64_enabled
-    elif x64==True and not jax.config.x64_enabled:
+    if x64 is None:
+        x64 = jax.config.x64_enabled
+    elif x64 == True and not jax.config.x64_enabled:
         raise ValueError(
-            'Cannot convert to 64-bit precision because jax.config.x64_enabled==False '
-            'Use jax.config.update("jax_enable_x64", True) to enable 64-bit precision.')
-    
+            "Cannot convert to 64-bit precision because jax.config.x64_enabled==False "
+            'Use jax.config.update("jax_enable_x64", True) to enable 64-bit precision.'
+        )
+
     def convert(x):
         x = jnp.asarray(x)
         if jnp.issubdtype(x.dtype, jnp.integer):
             return x.astype(jnp.int64 if x64 else jnp.int32)
         elif jnp.issubdtype(x.dtype, jnp.floating):
             return x.astype(jnp.float64 if x64 else jnp.float32)
-    
+
     return jax.tree_map(convert, data)
 
 
 def check_for_nans(data):
     """
     Check for NaNs in all arrays of a pytree.
 
     Parameters
     ----------
     data: pytree (dict, list, tuple, array, or any nested combination thereof)
         The data to check for NaNs in.
-    
+
     Returns
     -------
     any_nans: bool
         Whether any of the arrays in ``data`` contain a NaN.
 
     nan_info: list of tuples
         List of arrays containing a NaN, in the form of pairs
@@ -111,45 +118,45 @@
         keys that define the location of the array in the pytree.
 
     messages: list of str
         List of messages; one for each elements of ``nan_info``.
     """
 
     def _format(path, num_nan):
-        path = '/'.join(map(str,path))
-        msg  = f"{num_nan} NaNs found in {path}"
+        path = "/".join(map(str, path))
+        msg = f"{num_nan} NaNs found in {path}"
         return msg
-        
+
     nan_info = []
     messages = []
-    for path,value in zip(*tree_flatten_with_path(data)[:2]):
+    for path, value in zip(*tree_flatten_with_path(data)[:2]):
         if isinstance(value, jnp.ndarray):
             if jnp.isnan(value).any():
                 num_nans = jnp.isnan(value).sum().item()
                 nan_info.append((path, num_nans))
                 messages.append(_format(path, num_nans))
-    
-    any_nans = len(nan_info)>0
+
+    any_nans = len(nan_info) > 0
     return any_nans, nan_info, messages
 
 
 class CheckOutputsError(Exception):
     pass
 
 
 class checked_function_args:
     """
     Context manager that activates the :py:func`check_output` decorator
-    and captures the inputs of the decorated function. 
+    and captures the inputs of the decorated function.
 
     The `checked_function_args` context manager is a debugging tool
     that identifies when one or more functions in a call stack are
-    producing outputs with an undesired property (e.g. NaNs), and 
+    producing outputs with an undesired property (e.g. NaNs), and
     what the inputs to those functions were.
-    
+
     Examples
     --------
     Define a decorator called `nan_check` and use it to check for NaNs
     in the outputs of `func`. The inputs that caused `func` to produce
     NaNs are captured by the `checked_function_args` context manager.::
 
         >>> from jax_moseq.utils import check_for_nans
@@ -182,14 +189,15 @@
         File "<module>", line 92, in <module>
             caller_of_func(0, 2)
         File "<module>", line 89, in caller_of_func
             func(a, b)
         >>> print(args)
         {'func': ((0, 2), {}), 'caller_of_func': ((0, 2), {})}
     """
+
     def __init__(self):
         self.inputs_dict = {}
         self.active = False
         self.exit_stack = contextlib.ExitStack()
 
     def __enter__(self):
         self.active = True
@@ -199,67 +207,85 @@
 
     def __exit__(self, exc_type, exc_value, exc_traceback):
         self.active = False
         del sys._checked_function_args
         self.exit_stack.close()
 
         if isinstance(exc_value, CheckOutputsError):
-            print(exc_value, end='\n')  # Print the exception message
+            print(exc_value, end="\n")  # Print the exception message
 
             # Extract the traceback and filter out frames from the 'wrapper'
             tb_frames = traceback.extract_tb(exc_traceback)
-            filtered_frames = [frame for frame in tb_frames if frame.name != 'wrapper']
+            filtered_frames = [
+                frame for frame in tb_frames if frame.name != "wrapper"
+            ]
 
             # Format the filtered frames in a pretty way
             formatted_frames = traceback.format_list(filtered_frames)
 
             # Print the formatted frames
             for frame in formatted_frames:
                 print(frame)
 
             return True  # Suppress the exception from propagating further
-        
+
 
 def check_output(checker, error_message):
     """
     Creates a decorator that applies `checker` to the outputs of a function.
 
     This decorator is intended to be used in conjunction with the
     :py:class:`checked_function_args` context manager, and is only
-    active when the context manager is active. See 
+    active when the context manager is active. See
     :py:class:`checked_function_args` for example usage.
 
     Parameters
     ----------
     checker : callable
-        A function that takes the outputs of the decorated function and 
+        A function that takes the outputs of the decorated function and
         returns a boolean value.
 
     error_message : str
         The error message to be displayed when raising a CheckOutputsError.
 
     Returns
     -------
     decorator : callable
         The generated decorator that checks the function output.
     """
+
     def decorator(func):
         @functools.wraps(func)
         def wrapper(*args, **kwargs):
             try:
                 result = func(*args, **kwargs)
-                if not hasattr(sys, '_checked_function_args') or not sys._checked_function_args.active:
+                if (
+                    not hasattr(sys, "_checked_function_args")
+                    or not sys._checked_function_args.active
+                ):
                     return result
 
                 if checker(result):
-                    sys._checked_function_args.inputs_dict[func.__name__] = (args, kwargs)
+                    sys._checked_function_args.inputs_dict[func.__name__] = (
+                        args,
+                        kwargs,
+                    )
                     raise CheckOutputsError(error_message)
                 return result
-            
+
             except CheckOutputsError as e:
-                if hasattr(sys, '_checked_function_args') and sys._checked_function_args.active:
-                    sys._checked_function_args.inputs_dict[func.__name__] = (args, kwargs)
+                if (
+                    hasattr(sys, "_checked_function_args")
+                    and sys._checked_function_args.active
+                ):
+                    sys._checked_function_args.inputs_dict[func.__name__] = (
+                        args,
+                        kwargs,
+                    )
                 raise e
+
         return wrapper
+
     return decorator
 
-nan_check = check_output(check_for_nans, 'NaNs detected')
+
+nan_check = check_output(check_for_nans, "NaNs detected")
```

### Comparing `jax-moseq-0.0.3/jax_moseq/utils/distributions.py` & `jax-moseq-0.0.5/jax_moseq/utils/distributions.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,79 +1,94 @@
 import jax, jax.numpy as jnp, jax.random as jr
 import tensorflow_probability.substrates.jax.distributions as tfd
 from dynamax.hidden_markov_model.inference import hmm_posterior_sample
-from jax_moseq.utils import nan_check
+from jax_moseq.utils import convert_data_precision
+
 na = jnp.newaxis
 
+
 def sample_vonmises(seed, theta, kappa):
     return tfd.VonMises(theta, kappa).sample(seed=seed)
 
+
 def sample_vonmises_fisher(seed, direction):
     kappa = jnp.sqrt((direction**2).sum(-1))
-    direction = direction / kappa[...,na]
+    direction = direction / kappa[..., na]
     return tfd.VonMisesFisher(direction, kappa).sample(seed=seed)
 
+
 def sample_gamma(seed, a, b):
     return jr.gamma(seed, a) / b
 
+
 def sample_inv_gamma(seed, a, b):
-    return 1/sample_gamma(seed, a, b)
+    return 1 / sample_gamma(seed, a, b)
+
 
 def sample_scaled_inv_chi2(seed, degs, variance):
-    return sample_inv_gamma(seed, degs/2, degs*variance/2)
+    return sample_inv_gamma(seed, degs / 2, degs * variance / 2)
+
 
 def sample_chi2(seed, degs):
-    return jr.gamma(seed, degs/2)*2
+    return jr.gamma(seed, degs / 2) * 2
+
 
 def sample_mn(seed, M, U, V):
-    G = jr.normal(seed,M.shape)
-    G = jnp.dot(jnp.linalg.cholesky(U),G)
-    G = jnp.dot(G,jnp.linalg.cholesky(V).T)
+    G = jr.normal(seed, M.shape)
+    G = jnp.dot(jnp.linalg.cholesky(U), G)
+    G = jnp.dot(G, jnp.linalg.cholesky(V).T)
     return M + G
 
-@nan_check
-def sample_invwishart(seed,S,nu):
+
+def sample_invwishart(seed, S, nu):
     n = S.shape[0]
-    
+
     chi2_seed, norm_seed = jr.split(seed)
     x = jnp.diag(jnp.sqrt(sample_chi2(chi2_seed, nu - jnp.arange(n))))
-    x = x.at[jnp.triu_indices_from(x,1)].set(jr.normal(norm_seed, (n*(n-1)//2,)))
-    R = jnp.linalg.qr(x,'r')
-    
+    x = x.at[jnp.triu_indices_from(x, 1)].set(
+        jr.normal(norm_seed, (n * (n - 1) // 2,))
+    )
+    R = jnp.linalg.qr(x, "r")
+
     chol = jnp.linalg.cholesky(S)
-    
-    T = jax.scipy.linalg.solve_triangular(R.T,chol.T,lower=True).T
-    return jnp.dot(T,T.T)
 
-@nan_check
+    T = jax.scipy.linalg.solve_triangular(R.T, chol.T, lower=True).T
+    return jnp.dot(T, T.T)
+
+
 def sample_mniw(seed, nu, S, M, K):
     sigma = sample_invwishart(seed, S, nu)
     A = sample_mn(seed, M, sigma, K)
     return A, sigma
 
+
 def sample_hmm_stateseq(seed, transition_matrix, log_likelihoods, mask):
     """Sample state sequences in a Markov chain.
 
     Parameters
     ----------
-        seed: jax.random.PRNGKey
-            Random seed
-        transition_matrix: jax array, shape (num_states, num_states)
-            Transition matrix
-        log_likelihoods: jax array, shape (num_timesteps, num_states)
-            Sequence of log likelihoods of emissions given hidden state and parameters
-        mask: jax array, shape (num_timesteps,)
-            Sequence indicating whether to use an emission (1) or not (0)
+    seed: jax.random.PRNGKey
+        Random seed
+    transition_matrix: jax array, shape (num_states, num_states)
+        Transition matrix
+    log_likelihoods: jax array, shape (num_timesteps, num_states)
+        Sequence of log likelihoods of emissions given hidden state and parameters
+    mask: jax array, shape (num_timesteps,)
+        Sequence indicating whether to use an emission (1) or not (0)
 
     Returns
     -------
-        log_norm: float: 
-            Posterior marginal log likelihood
-        states: jax array, shape (num_timesteps,)
-            Sequence of sampled states
+    log_norm: float:
+        Posterior marginal log likelihood
+    states: jax array, shape (num_timesteps,)
+        Sequence of sampled states
     """
 
     num_states = transition_matrix.shape[0]
-    initial_distribution = jnp.ones(num_states)/num_states
+    initial_distribution = jnp.ones(num_states) / num_states
 
-    masked_log_likelihoods = log_likelihoods * mask[:,None]
-    return hmm_posterior_sample(seed, initial_distribution, transition_matrix, masked_log_likelihoods)
+    masked_log_likelihoods = log_likelihoods * mask[:, None]
+    L, z = hmm_posterior_sample(
+        seed, initial_distribution, transition_matrix, masked_log_likelihoods
+    )
+    z = convert_data_precision(z)
+    return L, z
```

### Comparing `jax-moseq-0.0.3/jax_moseq/utils/transitions.py` & `jax-moseq-0.0.5/jax_moseq/utils/transitions.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,56 +1,61 @@
 import numpy as np
 from numba import njit, prange
 
 import jax
 import jax.numpy as jnp
 import jax.random as jr
+
 eps = jnp.finfo(jnp.float32).tiny
 from functools import partial
 
 
-@partial(jax.jit, static_argnames=('num_states'))
+@partial(jax.jit, static_argnames=("num_states"))
 def count_transitions(num_states, stateseqs, mask):
     """
     Count the number of transitions between each pair of
     states ``i`` and ``j`` in the unmasked entries of ``stateseqs``,
     including self transitions (i.e. i == j).
 
     Parameters
     ----------
     num_states: int
         Total number of states (must exceed ``max(stateseqs)``).
 
     stateseqs: jax int array of shape (..., T)
         Batch of state sequences where the last dim indexes time.
-        All entries 
+        All entries
 
     mask: jax array of shape (..., T + num_lags)
         Binary indicator for which elements of ``stateseqs`` are valid.
         If ``num_lags > 0``, the first ``num_lags`` time points of the mask
         are ignored (ensures time alignment with the AR process).
 
     Returns
     -------
     transition_counts: jax array of shape (num_states, num_states)
         The number of transitions between every pair of states.
-    """    
+    """
     T = stateseqs.shape[-1]
-    
-    mask = mask[..., -T + 1:]
+
+    mask = mask[..., -T + 1 :]
     start_states = stateseqs[..., :-1]
     end_states = stateseqs[..., 1:]
-    
+
     transition_counts = jnp.zeros((num_states, num_states))
-    transition_counts = transition_counts.at[start_states, end_states].add(mask)
+    transition_counts = transition_counts.at[start_states, end_states].add(
+        mask
+    )
     return transition_counts
 
 
 @njit
-def _sample_loyal_crf_table_counts(rng, customer_counts, dish_ratings, loyalty):
+def _sample_loyal_crf_table_counts(
+    rng, customer_counts, dish_ratings, loyalty
+):
     """
     In a Chinese restaurant franchise (CRF) process with loyal customers,
     ``table_counts[i, j]`` represents the number of tables in restaurant ``i``
     that were served dish ``j``, which is a random variable that depends on:
 
         (1) the observed number of patrons in the restaurant eating
             the dish (``customer_counts[i, j]``),
@@ -77,27 +82,27 @@
     customer_counts : numpy array of shape (N, N)
         Number of customers for each restaurant/dish pair.
     dish_ratings : numpy array of shape N
         Parameter representing franchise-wide popularity of each dish.
     loyalty : scalar
         Non-negative scalar representing customers' bias for their
         restaurant's specialty dish.
-        
+
     Returns
     -------
     table_counts : numpy array of shape (N, N)
         Number of tables in each restaurant served each dish.
 
     References
     ----------
     See the supplement to Fox et al. 2011 at
     <http://dx.doi.org/10.1214/10-AOAS395SUPP>.
     """
 
-    N = len(dish_ratings)    # num restaurants/dishes
+    N = len(dish_ratings)  # num restaurants/dishes
 
     # Sample counts without considering loyalty factor
     table_counts = np.zeros_like(customer_counts)
     for i in prange(N):
         for j in range(N):
             # Sample counts by simulating table dish
             # assignment process.
@@ -108,93 +113,95 @@
                     dish_rating += loyalty
                 p = dish_rating / (k + dish_rating)
                 bernoulli_sample = rng.random() < p
                 table_counts[i, j] += bernoulli_sample
     return table_counts
 
 
-def _sample_beta_suffient_stats(seed, transition_counts,
-                                betas, alpha, kappa, gamma):
+def _sample_beta_suffient_stats(
+    seed, transition_counts, betas, alpha, kappa, gamma
+):
     """
     Compute the sufficient statistics for the Gibbs resampling
     of ``betas`` using the auxillary parameter scheme devised
     by Fox et al. for the Sticky HDP-HMM.
 
     Parameters
     ----------
     seed : jr.PRNGKey
         JAX random seed.
     transition_counts : jax array of shape (num_states, num_states)
         The number of transitions between every pair of states.
     betas : jax array of shape num_states
         State usages.
     alpha : scalar
-        State usage influence hyperparameter. 
+        State usage influence hyperparameter.
     kappa : scalar
         State persistence (i.e. "stickiness") hyperparameter.
     gamma : scalar
         Usage uniformity hyperparameter.
 
     Returns
     -------
     sufficient_stats : jax array of shape num_states
         Sufficient statistics for resampling `betas`.
     """
     num_states = len(betas)
-    
+
     # Sample table counts (uses numpy/numba)
     rng = np.random.default_rng(seed[0].item())
     concentrations = np.array(alpha * betas)
     transition_counts = np.array(transition_counts, dtype=np.int32)
     # m in Fox et al.
-    table_counts = _sample_loyal_crf_table_counts(rng, transition_counts,
-                                                  concentrations, kappa)
-    
+    table_counts = _sample_loyal_crf_table_counts(
+        rng, transition_counts, concentrations, kappa
+    )
+
     # Downweight the influence of self transitions,
     # which are less informative about state usages
-    auxillary_param = table_counts    # corresponds to mbar in Fox et al.
+    auxillary_param = table_counts  # corresponds to mbar in Fox et al.
     diagonal_counts = np.diag(auxillary_param)
     p = concentrations / (concentrations + kappa)
     binomial_samples = rng.binomial(diagonal_counts, p)
     np.fill_diagonal(auxillary_param, binomial_samples)
-    
+
     # Compute sufficient statistics
     sufficient_stats = auxillary_param.sum(0) + (gamma / num_states)
     sufficient_stats = jax.device_put(sufficient_stats)
     return sufficient_stats
 
 
-def sample_betas(seed, transition_counts,
-                 betas, alpha, kappa, gamma):
+def sample_betas(seed, transition_counts, betas, alpha, kappa, gamma):
     """
     Sample the state usages ``betas`` given the observed transition
     counts and the model hyperparameters.
 
     Parameters
     ----------
     seed : jr.PRNGKey
         JAX random seed.
     transition_counts : jax array of shape (num_states, num_states)
         The number of transitions between every pair of states.
     betas : jax array of shape num_states
         State usages.
     alpha : scalar
-        State usage influence hyperparameter. 
+        State usage influence hyperparameter.
     kappa : scalar
         State persistence (i.e. "stickiness") hyperparameter.
     gamma : scalar
         Usage uniformity hyperparameter.
 
     Returns
     -------
     betas : jax array of shape num_states
         Resampled state usages.
     """
     sufficient_stats = _sample_beta_suffient_stats(
-                seed, transition_counts, betas, alpha, kappa, gamma)
+        seed, transition_counts, betas, alpha, kappa, gamma
+    )
     betas = jr.dirichlet(seed, sufficient_stats)
     return betas
 
 
 def sample_pi(seed, transition_counts, betas, alpha, kappa):
     """
     Sample the transition matrix ``pi`` given the observed transition
@@ -205,84 +212,87 @@
     seed : jr.PRNGKey
         JAX random seed.
     transition_counts : jax array of shape (num_states, num_states)
         The number of transitions between every pair of states.
     betas : jax array of shape num_states
         State usages.
     alpha : scalar
-        State usage influence hyperparameter. 
+        State usage influence hyperparameter.
     kappa : scalar
         State persistence (i.e. "stickiness") hyperparameter.
 
     Returns
     -------
     pi : jax_array of shape (num_states, num_states)
         Resampled transition probabilities.
     """
     num_states = len(betas)
-    sufficient_stats = transition_counts + \
-            alpha * betas + kappa * jnp.eye(num_states)
+    sufficient_stats = (
+        transition_counts + alpha * betas + kappa * jnp.eye(num_states)
+    )
     pi = jr.dirichlet(seed, sufficient_stats)
     return pi
 
 
-def sample_hdp_transitions(seed, transition_counts,
-                           betas, alpha, kappa, gamma):
+def sample_hdp_transitions(
+    seed, transition_counts, betas, alpha, kappa, gamma
+):
     """
     Sample the transition parameters of the HDP-HMM given
     the observed transition counts, the current usage estimates,
     and the model hyperparameters.
 
     Parameters
     ----------
     seed : jr.PRNGKey
         JAX random seed.
     transition_counts : jax array of shape (num_states, num_states)
         The number of transitions between every pair of states.
     betas : jax array of shape num_states
         State usages.
     alpha : scalar
-        State usage influence hyperparameter. 
+        State usage influence hyperparameter.
     kappa : scalar
         State persistence (i.e. "stickiness") hyperparameter.
     gamma : scalar
         Usage uniformity hyperparameter.
 
     Returns
     -------
     betas : jax array of shape num_states
         Resampled state usages.
     pi : jax_array of shape (num_states, num_states)
         Resampled transition probabilities.
     """
     seeds = jr.split(seed)
-    betas = sample_betas(seeds[0], transition_counts,
-                         betas, alpha, kappa, gamma)
-    pi = sample_pi(seeds[1], transition_counts,
-                   betas, alpha, kappa)
+    betas = sample_betas(
+        seeds[0], transition_counts, betas, alpha, kappa, gamma
+    )
+    pi = sample_pi(seeds[1], transition_counts, betas, alpha, kappa)
     return betas, pi
 
 
-def resample_hdp_transitions(seed, z, mask, betas,
-                             alpha, kappa, gamma, **kwargs):
+def resample_hdp_transitions(
+    seed, z, mask, betas, alpha, kappa, gamma, **kwargs
+):
     """
     Resample the transition parameters of the HDP-HMM.
 
     Parameters
     ----------
     seed : jr.PRNGKey
         JAX random seed.
     z : jax_array of shape (..., T - n_lags)
         Discrete state sequences.
     mask : jax array of shape (..., T)
         Binary indicator for which data points are valid.
     betas : jax array of shape (num_states,)
         State usages.
     alpha : scalar
-        State usage influence hyperparameter. 
+        State usage influence hyperparameter.
     kappa : scalar
         State persistence (i.e. "stickiness") hyperparameter.
     gamma : scalar
         Usage uniformity hyperparameter.
     kwargs : dict
         Overflow, for convenience.
 
@@ -291,16 +301,17 @@
     betas : jax array of shape (num_states,)
         Resampled state usages.
     pi : jax_array of shape (num_states, num_states)
         Resampled transition probabilities.
     """
     num_states = len(betas)
     transition_counts = count_transitions(num_states, z, mask)
-    betas, pi = sample_hdp_transitions(seed, transition_counts,
-                                       betas, alpha, kappa, gamma)
+    betas, pi = sample_hdp_transitions(
+        seed, transition_counts, betas, alpha, kappa, gamma
+    )
     return betas, pi
 
 
 def init_hdp_transitions(seed, num_states, alpha, kappa, gamma, **kwargs):
     """
     Initialize the transition parameters of the HDP-HMM.
 
@@ -309,15 +320,15 @@
     seed : jr.PRNGKey
         JAX random seed.
     num_states : int
         Max number of HMM states.
     betas : jax array of shape (num_states,)
         State usages.
     alpha : scalar
-        State usage influence hyperparameter. 
+        State usage influence hyperparameter.
     kappa : scalar
         State persistence (i.e. "stickiness") hyperparameter.
     gamma : scalar
         Usage uniformity hyperparameter.
     kwargs : dict
         Overflow, for convenience.
 
@@ -325,15 +336,73 @@
     -------
     betas : jax array of shape (num_states,)
         Initial state usages.
     pi : jax_array of shape (num_states, num_states)
         Initial transition probabilities.
     """
     seeds = jr.split(seed)
-    betas_init = jr.dirichlet(seeds[0], jnp.full(num_states, gamma / num_states))
+    betas_init = jr.dirichlet(
+        seeds[0], jnp.full(num_states, gamma / num_states)
+    )
     pseudo_counts = jnp.zeros((num_states, num_states))
-    betas, pi = sample_hdp_transitions(seeds[1], pseudo_counts, betas_init,
-                                       alpha, kappa, gamma)
-    
+    betas, pi = sample_hdp_transitions(
+        seeds[1], pseudo_counts, betas_init, alpha, kappa, gamma
+    )
+
     # pseudocount for numerical stability
-    pi = (pi+eps)/(pi+eps).sum(1)[:,None]
-    return betas, pi
+    pi = (pi + eps) / (pi + eps).sum(1)[:, None]
+    return betas, pi
+
+
+def sample_dir_transitions(seed, transition_counts, beta, kappa):
+    """
+    Sample a transition matrix using a sticky Dirichlet prior.
+
+    Parameters
+    ----------
+    seed : jr.PRNGKey
+        JAX random seed.
+    transition_counts : jax array of shape (num_states, num_states)
+        The number of transitions between every pair of states.
+    beta : scalar
+        Dirichlet prior concentration parameter.
+    kappa : scalar
+        State persistence (i.e. "stickiness") hyperparameter.
+
+    Returns
+    -------
+    pi : jax_array of shape (num_states, num_states)
+        Transition probabilities.
+    """
+    num_states = transition_counts.shape[0]
+    conc = (beta + transition_counts) + kappa * jnp.eye(num_states)
+    pi = jax.vmap(jr.dirichlet)(jr.split(seed, num_states), conc)
+    return pi
+
+
+def resample_dir_transitions(seed, num_states, z, mask, beta, kappa, **kwargs):
+    """
+    Resample Markov transition probabilities using a sticky Dirichlet prior.
+
+    Parameters
+    ----------
+    seed : jr.PRNGKey
+        JAX random seed.
+    num_states : int
+        Max number of HMM states.
+    z : jax_array of shape (..., T - n_lags)
+        Discrete state sequences.
+    mask : jax array of shape (..., T)
+        Binary indicator for which data points are valid.
+    beta : scalar
+        Dirichlet prior concentration parameter.
+    kappa : scalar
+        State persistence (i.e. "stickiness") hyperparameter.
+
+    Returns
+    -------
+    pi : jax_array of shape (num_states, num_states)
+        Resampled transition probabilities.
+    """
+    transition_counts = count_transitions(num_states, z, mask)
+    pi = sample_dir_transitions(seed, transition_counts, beta, kappa)
+    return pi
```

### Comparing `jax-moseq-0.0.3/jax_moseq.egg-info/SOURCES.txt` & `jax-moseq-0.0.5/jax_moseq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jax-moseq-0.0.3/setup.cfg` & `jax-moseq-0.0.5/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -8,17 +8,19 @@
 	Operating System :: OS Independent
 
 [options]
 packages = find:
 include_package_data = True
 python_requires = >=3.8
 install_requires = 
-	numba
+	numba>=0.56.4
 	dynamax
 	chex==0.1.6
+	jaxtyping==0.2.14
+	tensorflow_probability==0.19.0
 	tqdm
 	optree
 
 [options.package_data]
 * = *.md
 
 [versioneer]
```

### Comparing `jax-moseq-0.0.3/versioneer.py` & `jax-moseq-0.0.5/versioneer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 # Version: 0.28
 
 """The Versioneer - like a rocketeer, but for versions.
 
 The Versioneer
 ==============
 
@@ -344,33 +343,37 @@
     versioneer_py = os.path.join(root, "versioneer.py")
     if not (os.path.exists(setup_py) or os.path.exists(versioneer_py)):
         # allow 'python path/to/setup.py COMMAND'
         root = os.path.dirname(os.path.realpath(os.path.abspath(sys.argv[0])))
         setup_py = os.path.join(root, "setup.py")
         versioneer_py = os.path.join(root, "versioneer.py")
     if not (os.path.exists(setup_py) or os.path.exists(versioneer_py)):
-        err = ("Versioneer was unable to run the project root directory. "
-               "Versioneer requires setup.py to be executed from "
-               "its immediate directory (like 'python setup.py COMMAND'), "
-               "or in a way that lets it use sys.argv[0] to find the root "
-               "(like 'python path/to/setup.py COMMAND').")
+        err = (
+            "Versioneer was unable to run the project root directory. "
+            "Versioneer requires setup.py to be executed from "
+            "its immediate directory (like 'python setup.py COMMAND'), "
+            "or in a way that lets it use sys.argv[0] to find the root "
+            "(like 'python path/to/setup.py COMMAND')."
+        )
         raise VersioneerBadRootError(err)
     try:
         # Certain runtime workflows (setup.py install/develop in a setuptools
         # tree) execute all dependencies in a single python process, so
         # "versioneer" may be imported multiple times, and python's shared
         # module-import table will cache the first one. So we can't use
         # os.path.dirname(__file__), as that will find whichever
         # versioneer.py was first imported, even in later projects.
         my_path = os.path.realpath(os.path.abspath(__file__))
         me_dir = os.path.normcase(os.path.splitext(my_path)[0])
         vsr_dir = os.path.normcase(os.path.splitext(versioneer_py)[0])
         if me_dir != vsr_dir and "VERSIONEER_PEP518" not in globals():
-            print("Warning: build in %s is using versioneer.py from %s"
-                  % (os.path.dirname(my_path), versioneer_py))
+            print(
+                "Warning: build in %s is using versioneer.py from %s"
+                % (os.path.dirname(my_path), versioneer_py)
+            )
     except NameError:
         pass
     return root
 
 
 def get_config_from_root(root):
     """Read the project setup.cfg file to determine Versioneer config."""
@@ -380,29 +383,29 @@
     # the top of versioneer.py for instructions on writing your setup.cfg .
     root = Path(root)
     pyproject_toml = root / "pyproject.toml"
     setup_cfg = root / "setup.cfg"
     section = None
     if pyproject_toml.exists() and have_tomllib:
         try:
-            with open(pyproject_toml, 'rb') as fobj:
+            with open(pyproject_toml, "rb") as fobj:
                 pp = tomllib.load(fobj)
-            section = pp['tool']['versioneer']
+            section = pp["tool"]["versioneer"]
         except (tomllib.TOMLDecodeError, KeyError):
             pass
     if not section:
         parser = configparser.ConfigParser()
         with open(setup_cfg) as cfg_file:
             parser.read_file(cfg_file)
         parser.get("versioneer", "VCS")  # raise error if missing
 
         section = parser["versioneer"]
 
     cfg = VersioneerConfig()
-    cfg.VCS = section['VCS']
+    cfg.VCS = section["VCS"]
     cfg.style = section.get("style", "")
     cfg.versionfile_source = section.get("versionfile_source")
     cfg.versionfile_build = section.get("versionfile_build")
     cfg.tag_prefix = section.get("tag_prefix")
     if cfg.tag_prefix in ("''", '""', None):
         cfg.tag_prefix = ""
     cfg.parentdir_prefix = section.get("parentdir_prefix")
@@ -417,23 +420,26 @@
 # these dictionaries contain VCS-specific tools
 LONG_VERSION_PY: Dict[str, str] = {}
 HANDLERS: Dict[str, Dict[str, Callable]] = {}
 
 
 def register_vcs_handler(vcs, method):  # decorator
     """Create decorator to mark a method as the handler of a VCS."""
+
     def decorate(f):
         """Store f in HANDLERS[vcs][method]."""
         HANDLERS.setdefault(vcs, {})[method] = f
         return f
+
     return decorate
 
 
-def run_command(commands, args, cwd=None, verbose=False, hide_stderr=False,
-                env=None):
+def run_command(
+    commands, args, cwd=None, verbose=False, hide_stderr=False, env=None
+):
     """Call the given command(s)."""
     assert isinstance(commands, list)
     process = None
 
     popen_kwargs = {}
     if sys.platform == "win32":
         # This hides the console window if pythonw.exe is used
@@ -441,18 +447,22 @@
         startupinfo.dwFlags |= subprocess.STARTF_USESHOWWINDOW
         popen_kwargs["startupinfo"] = startupinfo
 
     for command in commands:
         try:
             dispcmd = str([command] + args)
             # remember shell=False, so use git.cmd on windows, not just git
-            process = subprocess.Popen([command] + args, cwd=cwd, env=env,
-                                       stdout=subprocess.PIPE,
-                                       stderr=(subprocess.PIPE if hide_stderr
-                                               else None), **popen_kwargs)
+            process = subprocess.Popen(
+                [command] + args,
+                cwd=cwd,
+                env=env,
+                stdout=subprocess.PIPE,
+                stderr=(subprocess.PIPE if hide_stderr else None),
+                **popen_kwargs,
+            )
             break
         except OSError:
             e = sys.exc_info()[1]
             if e.errno == errno.ENOENT:
                 continue
             if verbose:
                 print("unable to run %s" % dispcmd)
@@ -467,15 +477,17 @@
         if verbose:
             print("unable to run %s (error)" % dispcmd)
             print("stdout was %s" % stdout)
         return None, process.returncode
     return stdout, process.returncode
 
 
-LONG_VERSION_PY['git'] = r'''
+LONG_VERSION_PY[
+    "git"
+] = r'''
 # This file helps to compute a version number in source trees obtained from
 # git-archive tarball (such as those provided by githubs download-from-tag
 # feature). Distribution tarballs (built by setup.py sdist) and build
 # directories (produced by setup.py build) will contain a much shorter file
 # that just contains the computed version number.
 
 # This file is released into the public domain.
@@ -1183,49 +1195,56 @@
         if verbose:
             print("keywords are unexpanded, not using")
         raise NotThisMethod("unexpanded keywords, not a git-archive tarball")
     refs = {r.strip() for r in refnames.strip("()").split(",")}
     # starting in git-1.8.3, tags are listed as "tag: foo-1.0" instead of
     # just "foo-1.0". If we see a "tag: " prefix, prefer those.
     TAG = "tag: "
-    tags = {r[len(TAG):] for r in refs if r.startswith(TAG)}
+    tags = {r[len(TAG) :] for r in refs if r.startswith(TAG)}
     if not tags:
         # Either we're using git < 1.8.3, or there really are no tags. We use
         # a heuristic: assume all version tags have a digit. The old git %d
         # expansion behaves like git log --decorate=short and strips out the
         # refs/heads/ and refs/tags/ prefixes that would let us distinguish
         # between branches and tags. By ignoring refnames without digits, we
         # filter out many common branch names like "release" and
         # "stabilization", as well as "HEAD" and "master".
-        tags = {r for r in refs if re.search(r'\d', r)}
+        tags = {r for r in refs if re.search(r"\d", r)}
         if verbose:
             print("discarding '%s', no digits" % ",".join(refs - tags))
     if verbose:
         print("likely tags: %s" % ",".join(sorted(tags)))
     for ref in sorted(tags):
         # sorting will prefer e.g. "2.0" over "2.0rc1"
         if ref.startswith(tag_prefix):
-            r = ref[len(tag_prefix):]
+            r = ref[len(tag_prefix) :]
             # Filter out refs that exactly match prefix or that don't start
             # with a number once the prefix is stripped (mostly a concern
             # when prefix is '')
-            if not re.match(r'\d', r):
+            if not re.match(r"\d", r):
                 continue
             if verbose:
                 print("picking %s" % r)
-            return {"version": r,
-                    "full-revisionid": keywords["full"].strip(),
-                    "dirty": False, "error": None,
-                    "date": date}
+            return {
+                "version": r,
+                "full-revisionid": keywords["full"].strip(),
+                "dirty": False,
+                "error": None,
+                "date": date,
+            }
     # no suitable tags, so version is "0+unknown", but full hex is still there
     if verbose:
         print("no suitable tags, using unknown + full revision id")
-    return {"version": "0+unknown",
-            "full-revisionid": keywords["full"].strip(),
-            "dirty": False, "error": "no suitable tags", "date": None}
+    return {
+        "version": "0+unknown",
+        "full-revisionid": keywords["full"].strip(),
+        "dirty": False,
+        "error": "no suitable tags",
+        "date": None,
+    }
 
 
 @register_vcs_handler("git", "pieces_from_vcs")
 def git_pieces_from_vcs(tag_prefix, root, verbose, runner=run_command):
     """Get version from 'git describe' in the root of the source tree.
 
     This only gets called if the git-archive 'subst' keywords were *not*
@@ -1239,43 +1258,54 @@
     # GIT_DIR can interfere with correct operation of Versioneer.
     # It may be intended to be passed to the Versioneer-versioned project,
     # but that should not change where we get our version from.
     env = os.environ.copy()
     env.pop("GIT_DIR", None)
     runner = functools.partial(runner, env=env)
 
-    _, rc = runner(GITS, ["rev-parse", "--git-dir"], cwd=root,
-                   hide_stderr=not verbose)
+    _, rc = runner(
+        GITS, ["rev-parse", "--git-dir"], cwd=root, hide_stderr=not verbose
+    )
     if rc != 0:
         if verbose:
             print("Directory %s not under git control" % root)
         raise NotThisMethod("'git rev-parse --git-dir' returned error")
 
     # if there is a tag matching tag_prefix, this yields TAG-NUM-gHEX[-dirty]
     # if there isn't one, this yields HEX[-dirty] (no NUM)
-    describe_out, rc = runner(GITS, [
-        "describe", "--tags", "--dirty", "--always", "--long",
-        "--match", f"{tag_prefix}[[:digit:]]*"
-    ], cwd=root)
+    describe_out, rc = runner(
+        GITS,
+        [
+            "describe",
+            "--tags",
+            "--dirty",
+            "--always",
+            "--long",
+            "--match",
+            f"{tag_prefix}[[:digit:]]*",
+        ],
+        cwd=root,
+    )
     # --long was added in git-1.5.5
     if describe_out is None:
         raise NotThisMethod("'git describe' failed")
     describe_out = describe_out.strip()
     full_out, rc = runner(GITS, ["rev-parse", "HEAD"], cwd=root)
     if full_out is None:
         raise NotThisMethod("'git rev-parse' failed")
     full_out = full_out.strip()
 
     pieces = {}
     pieces["long"] = full_out
     pieces["short"] = full_out[:7]  # maybe improved later
     pieces["error"] = None
 
-    branch_name, rc = runner(GITS, ["rev-parse", "--abbrev-ref", "HEAD"],
-                             cwd=root)
+    branch_name, rc = runner(
+        GITS, ["rev-parse", "--abbrev-ref", "HEAD"], cwd=root
+    )
     # --abbrev-ref was added in git-1.6.3
     if rc != 0 or branch_name is None:
         raise NotThisMethod("'git rev-parse --abbrev-ref' returned error")
     branch_name = branch_name.strip()
 
     if branch_name == "HEAD":
         # If we aren't exactly on a branch, pick a branch which represents
@@ -1307,52 +1337,57 @@
     # TAG might have hyphens.
     git_describe = describe_out
 
     # look for -dirty suffix
     dirty = git_describe.endswith("-dirty")
     pieces["dirty"] = dirty
     if dirty:
-        git_describe = git_describe[:git_describe.rindex("-dirty")]
+        git_describe = git_describe[: git_describe.rindex("-dirty")]
 
     # now we have TAG-NUM-gHEX or HEX
 
     if "-" in git_describe:
         # TAG-NUM-gHEX
-        mo = re.search(r'^(.+)-(\d+)-g([0-9a-f]+)$', git_describe)
+        mo = re.search(r"^(.+)-(\d+)-g([0-9a-f]+)$", git_describe)
         if not mo:
             # unparsable. Maybe git-describe is misbehaving?
-            pieces["error"] = ("unable to parse git-describe output: '%s'"
-                               % describe_out)
+            pieces["error"] = (
+                "unable to parse git-describe output: '%s'" % describe_out
+            )
             return pieces
 
         # tag
         full_tag = mo.group(1)
         if not full_tag.startswith(tag_prefix):
             if verbose:
                 fmt = "tag '%s' doesn't start with prefix '%s'"
                 print(fmt % (full_tag, tag_prefix))
-            pieces["error"] = ("tag '%s' doesn't start with prefix '%s'"
-                               % (full_tag, tag_prefix))
+            pieces["error"] = "tag '%s' doesn't start with prefix '%s'" % (
+                full_tag,
+                tag_prefix,
+            )
             return pieces
-        pieces["closest-tag"] = full_tag[len(tag_prefix):]
+        pieces["closest-tag"] = full_tag[len(tag_prefix) :]
 
         # distance: number of commits since tag
         pieces["distance"] = int(mo.group(2))
 
         # commit: short hex revision ID
         pieces["short"] = mo.group(3)
 
     else:
         # HEX: no tags
         pieces["closest-tag"] = None
         out, rc = runner(GITS, ["rev-list", "HEAD", "--left-right"], cwd=root)
         pieces["distance"] = len(out.split())  # total number of commits
 
     # commit date: see ISO-8601 comment in git_versions_from_keywords()
-    date = runner(GITS, ["show", "-s", "--format=%ci", "HEAD"], cwd=root)[0].strip()
+    date = runner(GITS, ["show", "-s", "--format=%ci", "HEAD"], cwd=root)[
+        0
+    ].strip()
     # Use only the last line.  Previous lines may contain GPG signature
     # information.
     date = date.splitlines()[-1]
     pieces["date"] = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
 
     return pieces
 
@@ -1403,23 +1438,29 @@
     two directory levels for an appropriately named parent directory
     """
     rootdirs = []
 
     for _ in range(3):
         dirname = os.path.basename(root)
         if dirname.startswith(parentdir_prefix):
-            return {"version": dirname[len(parentdir_prefix):],
-                    "full-revisionid": None,
-                    "dirty": False, "error": None, "date": None}
+            return {
+                "version": dirname[len(parentdir_prefix) :],
+                "full-revisionid": None,
+                "dirty": False,
+                "error": None,
+                "date": None,
+            }
         rootdirs.append(root)
         root = os.path.dirname(root)  # up a level
 
     if verbose:
-        print("Tried directories %s but none started with prefix %s" %
-              (str(rootdirs), parentdir_prefix))
+        print(
+            "Tried directories %s but none started with prefix %s"
+            % (str(rootdirs), parentdir_prefix)
+        )
     raise NotThisMethod("rootdir doesn't start with parentdir_prefix")
 
 
 SHORT_VERSION_PY = """
 # This file was generated by 'versioneer.py' (0.28) from
 # revision-control system data, or from the parent directory name of an
 # unpacked source archive. Distribution tarballs contain a pre-generated copy
@@ -1440,29 +1481,36 @@
 def versions_from_file(filename):
     """Try to determine the version from _version.py if present."""
     try:
         with open(filename) as f:
             contents = f.read()
     except OSError:
         raise NotThisMethod("unable to read _version.py")
-    mo = re.search(r"version_json = '''\n(.*)'''  # END VERSION_JSON",
-                   contents, re.M | re.S)
+    mo = re.search(
+        r"version_json = '''\n(.*)'''  # END VERSION_JSON",
+        contents,
+        re.M | re.S,
+    )
     if not mo:
-        mo = re.search(r"version_json = '''\r\n(.*)'''  # END VERSION_JSON",
-                       contents, re.M | re.S)
+        mo = re.search(
+            r"version_json = '''\r\n(.*)'''  # END VERSION_JSON",
+            contents,
+            re.M | re.S,
+        )
     if not mo:
         raise NotThisMethod("no version_json in _version.py")
     return json.loads(mo.group(1))
 
 
 def write_to_version_file(filename, versions):
     """Write the given version number to the given _version.py file."""
     os.unlink(filename)
-    contents = json.dumps(versions, sort_keys=True,
-                          indent=1, separators=(",", ": "))
+    contents = json.dumps(
+        versions, sort_keys=True, indent=1, separators=(",", ": ")
+    )
     with open(filename, "w") as f:
         f.write(SHORT_VERSION_PY % contents)
 
     print("set %s to '%s'" % (filename, versions["version"]))
 
 
 def plus_or_dot(pieces):
@@ -1486,16 +1534,15 @@
         if pieces["distance"] or pieces["dirty"]:
             rendered += plus_or_dot(pieces)
             rendered += "%d.g%s" % (pieces["distance"], pieces["short"])
             if pieces["dirty"]:
                 rendered += ".dirty"
     else:
         # exception #1
-        rendered = "0+untagged.%d.g%s" % (pieces["distance"],
-                                          pieces["short"])
+        rendered = "0+untagged.%d.g%s" % (pieces["distance"], pieces["short"])
         if pieces["dirty"]:
             rendered += ".dirty"
     return rendered
 
 
 def render_pep440_branch(pieces):
     """TAG[[.dev0]+DISTANCE.gHEX[.dirty]] .
@@ -1516,16 +1563,15 @@
             if pieces["dirty"]:
                 rendered += ".dirty"
     else:
         # exception #1
         rendered = "0"
         if pieces["branch"] != "master":
             rendered += ".dev0"
-        rendered += "+untagged.%d.g%s" % (pieces["distance"],
-                                          pieces["short"])
+        rendered += "+untagged.%d.g%s" % (pieces["distance"], pieces["short"])
         if pieces["dirty"]:
             rendered += ".dirty"
     return rendered
 
 
 def pep440_split_post(ver):
     """Split pep440 version string at the post-release segment.
@@ -1542,18 +1588,23 @@
 
     Exceptions:
     1: no tags. 0.post0.devDISTANCE
     """
     if pieces["closest-tag"]:
         if pieces["distance"]:
             # update the post release segment
-            tag_version, post_version = pep440_split_post(pieces["closest-tag"])
+            tag_version, post_version = pep440_split_post(
+                pieces["closest-tag"]
+            )
             rendered = tag_version
             if post_version is not None:
-                rendered += ".post%d.dev%d" % (post_version + 1, pieces["distance"])
+                rendered += ".post%d.dev%d" % (
+                    post_version + 1,
+                    pieces["distance"],
+                )
             else:
                 rendered += ".post0.dev%d" % (pieces["distance"])
         else:
             # no commits, use the tag as the version
             rendered = pieces["closest-tag"]
     else:
         # exception #1
@@ -1678,19 +1729,21 @@
         rendered += "-dirty"
     return rendered
 
 
 def render(pieces, style):
     """Render the given version pieces into the requested style."""
     if pieces["error"]:
-        return {"version": "unknown",
-                "full-revisionid": pieces.get("long"),
-                "dirty": None,
-                "error": pieces["error"],
-                "date": None}
+        return {
+            "version": "unknown",
+            "full-revisionid": pieces.get("long"),
+            "dirty": None,
+            "error": pieces["error"],
+            "date": None,
+        }
 
     if not style or style == "default":
         style = "pep440"  # the default
 
     if style == "pep440":
         rendered = render_pep440(pieces)
     elif style == "pep440-branch":
@@ -1706,17 +1759,21 @@
     elif style == "git-describe":
         rendered = render_git_describe(pieces)
     elif style == "git-describe-long":
         rendered = render_git_describe_long(pieces)
     else:
         raise ValueError("unknown style '%s'" % style)
 
-    return {"version": rendered, "full-revisionid": pieces["long"],
-            "dirty": pieces["dirty"], "error": None,
-            "date": pieces.get("date")}
+    return {
+        "version": rendered,
+        "full-revisionid": pieces["long"],
+        "dirty": pieces["dirty"],
+        "error": None,
+        "date": pieces.get("date"),
+    }
 
 
 class VersioneerBadRootError(Exception):
     """The project root directory is unknown or missing key files."""
 
 
 def get_versions(verbose=False):
@@ -1731,16 +1788,17 @@
     root = get_root()
     cfg = get_config_from_root(root)
 
     assert cfg.VCS is not None, "please set [versioneer]VCS= in setup.cfg"
     handlers = HANDLERS.get(cfg.VCS)
     assert handlers, "unrecognized VCS '%s'" % cfg.VCS
     verbose = verbose or cfg.verbose
-    assert cfg.versionfile_source is not None, \
-        "please set versioneer.versionfile_source"
+    assert (
+        cfg.versionfile_source is not None
+    ), "please set versioneer.versionfile_source"
     assert cfg.tag_prefix is not None, "please set versioneer.tag_prefix"
 
     versionfile_abs = os.path.join(root, cfg.versionfile_source)
 
     # extract version from first of: _version.py, VCS command (e.g. 'git
     # describe'), parentdir. This is meant to work for developers using a
     # source checkout, for users of a tarball created by 'setup.py sdist',
@@ -1786,17 +1844,21 @@
             return ver
     except NotThisMethod:
         pass
 
     if verbose:
         print("unable to compute version")
 
-    return {"version": "0+unknown", "full-revisionid": None,
-            "dirty": None, "error": "unable to compute version",
-            "date": None}
+    return {
+        "version": "0+unknown",
+        "full-revisionid": None,
+        "dirty": None,
+        "error": "unable to compute version",
+        "date": None,
+    }
 
 
 def get_version():
     """Get the short version string for this project."""
     return get_versions()["version"]
 
 
@@ -1841,14 +1903,15 @@
             vers = get_versions(verbose=True)
             print("Version: %s" % vers["version"])
             print(" full-revisionid: %s" % vers.get("full-revisionid"))
             print(" dirty: %s" % vers.get("dirty"))
             print(" date: %s" % vers.get("date"))
             if vers["error"]:
                 print(" error: %s" % vers["error"])
+
     cmds["version"] = cmd_version
 
     # we override "build_py" in setuptools
     #
     # most invocation pathways end up running build_py:
     #  distutils/build -> build_py
     #  distutils/install -> distutils/build ->..
@@ -1862,16 +1925,16 @@
     #   then does setup.py bdist_wheel, or sometimes setup.py install
     #  setup.py egg_info -> ?
 
     # pip install -e . and setuptool/editable_wheel will invoke build_py
     # but the build_py command is not expected to copy any files.
 
     # we override different "build_py" commands for both environments
-    if 'build_py' in cmds:
-        _build_py = cmds['build_py']
+    if "build_py" in cmds:
+        _build_py = cmds["build_py"]
     else:
         from setuptools.command.build_py import build_py as _build_py
 
     class cmd_build_py(_build_py):
         def run(self):
             root = get_root()
             cfg = get_config_from_root(root)
@@ -1880,22 +1943,24 @@
             if getattr(self, "editable_mode", False):
                 # During editable installs `.py` and data files are
                 # not copied to build_lib
                 return
             # now locate _version.py in the new build/ directory and replace
             # it with an updated value
             if cfg.versionfile_build:
-                target_versionfile = os.path.join(self.build_lib,
-                                                  cfg.versionfile_build)
+                target_versionfile = os.path.join(
+                    self.build_lib, cfg.versionfile_build
+                )
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
+
     cmds["build_py"] = cmd_build_py
 
-    if 'build_ext' in cmds:
-        _build_ext = cmds['build_ext']
+    if "build_ext" in cmds:
+        _build_ext = cmds["build_ext"]
     else:
         from setuptools.command.build_ext import build_ext as _build_ext
 
     class cmd_build_ext(_build_ext):
         def run(self):
             root = get_root()
             cfg = get_config_from_root(root)
@@ -1907,27 +1972,32 @@
                 # As in place builds will already have a _version.py
                 # in the module dir, we do not need to write one.
                 return
             # now locate _version.py in the new build/ directory and replace
             # it with an updated value
             if not cfg.versionfile_build:
                 return
-            target_versionfile = os.path.join(self.build_lib,
-                                              cfg.versionfile_build)
+            target_versionfile = os.path.join(
+                self.build_lib, cfg.versionfile_build
+            )
             if not os.path.exists(target_versionfile):
-                print(f"Warning: {target_versionfile} does not exist, skipping "
-                      "version update. This can happen if you are running build_ext "
-                      "without first running build_py.")
+                print(
+                    f"Warning: {target_versionfile} does not exist, skipping "
+                    "version update. This can happen if you are running build_ext "
+                    "without first running build_py."
+                )
                 return
             print("UPDATING %s" % target_versionfile)
             write_to_version_file(target_versionfile, versions)
+
     cmds["build_ext"] = cmd_build_ext
 
     if "cx_Freeze" in sys.modules:  # cx_freeze enabled?
         from cx_Freeze.dist import build_exe as _build_exe
+
         # nczeczulin reports that py2exe won't like the pep440-style string
         # as FILEVERSION, but it can be used for PRODUCTVERSION, e.g.
         # setup(console=[{
         #   "version": versioneer.get_version().split("+", 1)[0], # FILEVERSION
         #   "product_version": versioneer.get_version(),
         #   ...
 
@@ -1940,25 +2010,29 @@
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
 
                 _build_exe.run(self)
                 os.unlink(target_versionfile)
                 with open(cfg.versionfile_source, "w") as f:
                     LONG = LONG_VERSION_PY[cfg.VCS]
-                    f.write(LONG %
-                            {"DOLLAR": "$",
-                             "STYLE": cfg.style,
-                             "TAG_PREFIX": cfg.tag_prefix,
-                             "PARENTDIR_PREFIX": cfg.parentdir_prefix,
-                             "VERSIONFILE_SOURCE": cfg.versionfile_source,
-                             })
+                    f.write(
+                        LONG
+                        % {
+                            "DOLLAR": "$",
+                            "STYLE": cfg.style,
+                            "TAG_PREFIX": cfg.tag_prefix,
+                            "PARENTDIR_PREFIX": cfg.parentdir_prefix,
+                            "VERSIONFILE_SOURCE": cfg.versionfile_source,
+                        }
+                    )
+
         cmds["build_exe"] = cmd_build_exe
         del cmds["build_py"]
 
-    if 'py2exe' in sys.modules:  # py2exe enabled?
+    if "py2exe" in sys.modules:  # py2exe enabled?
         try:
             from py2exe.setuptools_buildexe import py2exe as _py2exe
         except ImportError:
             from py2exe.distutils_buildexe import py2exe as _py2exe
 
         class cmd_py2exe(_py2exe):
             def run(self):
@@ -1969,63 +2043,70 @@
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
 
                 _py2exe.run(self)
                 os.unlink(target_versionfile)
                 with open(cfg.versionfile_source, "w") as f:
                     LONG = LONG_VERSION_PY[cfg.VCS]
-                    f.write(LONG %
-                            {"DOLLAR": "$",
-                             "STYLE": cfg.style,
-                             "TAG_PREFIX": cfg.tag_prefix,
-                             "PARENTDIR_PREFIX": cfg.parentdir_prefix,
-                             "VERSIONFILE_SOURCE": cfg.versionfile_source,
-                             })
+                    f.write(
+                        LONG
+                        % {
+                            "DOLLAR": "$",
+                            "STYLE": cfg.style,
+                            "TAG_PREFIX": cfg.tag_prefix,
+                            "PARENTDIR_PREFIX": cfg.parentdir_prefix,
+                            "VERSIONFILE_SOURCE": cfg.versionfile_source,
+                        }
+                    )
+
         cmds["py2exe"] = cmd_py2exe
 
     # sdist farms its file list building out to egg_info
-    if 'egg_info' in cmds:
-        _egg_info = cmds['egg_info']
+    if "egg_info" in cmds:
+        _egg_info = cmds["egg_info"]
     else:
         from setuptools.command.egg_info import egg_info as _egg_info
 
     class cmd_egg_info(_egg_info):
         def find_sources(self):
             # egg_info.find_sources builds the manifest list and writes it
             # in one shot
             super().find_sources()
 
             # Modify the filelist and normalize it
             root = get_root()
             cfg = get_config_from_root(root)
-            self.filelist.append('versioneer.py')
+            self.filelist.append("versioneer.py")
             if cfg.versionfile_source:
                 # There are rare cases where versionfile_source might not be
                 # included by default, so we must be explicit
                 self.filelist.append(cfg.versionfile_source)
             self.filelist.sort()
             self.filelist.remove_duplicates()
 
             # The write method is hidden in the manifest_maker instance that
             # generated the filelist and was thrown away
             # We will instead replicate their final normalization (to unicode,
             # and POSIX-style paths)
             from setuptools import unicode_utils
-            normalized = [unicode_utils.filesys_decode(f).replace(os.sep, '/')
-                          for f in self.filelist.files]
 
-            manifest_filename = os.path.join(self.egg_info, 'SOURCES.txt')
-            with open(manifest_filename, 'w') as fobj:
-                fobj.write('\n'.join(normalized))
+            normalized = [
+                unicode_utils.filesys_decode(f).replace(os.sep, "/")
+                for f in self.filelist.files
+            ]
+
+            manifest_filename = os.path.join(self.egg_info, "SOURCES.txt")
+            with open(manifest_filename, "w") as fobj:
+                fobj.write("\n".join(normalized))
 
-    cmds['egg_info'] = cmd_egg_info
+    cmds["egg_info"] = cmd_egg_info
 
     # we override different "sdist" commands for both environments
-    if 'sdist' in cmds:
-        _sdist = cmds['sdist']
+    if "sdist" in cmds:
+        _sdist = cmds["sdist"]
     else:
         from setuptools.command.sdist import sdist as _sdist
 
     class cmd_sdist(_sdist):
         def run(self):
             versions = get_versions()
             self._versioneer_generated_versions = versions
@@ -2039,16 +2120,18 @@
             cfg = get_config_from_root(root)
             _sdist.make_release_tree(self, base_dir, files)
             # now locate _version.py in the new base_dir directory
             # (remembering that it may be a hardlink) and replace it with an
             # updated value
             target_versionfile = os.path.join(base_dir, cfg.versionfile_source)
             print("UPDATING %s" % target_versionfile)
-            write_to_version_file(target_versionfile,
-                                  self._versioneer_generated_versions)
+            write_to_version_file(
+                target_versionfile, self._versioneer_generated_versions
+            )
+
     cmds["sdist"] = cmd_sdist
 
     return cmds
 
 
 CONFIG_ERROR = """
 setup.cfg is missing the necessary Versioneer configuration. You need
@@ -2100,36 +2183,43 @@
 
 
 def do_setup():
     """Do main VCS-independent setup function for installing Versioneer."""
     root = get_root()
     try:
         cfg = get_config_from_root(root)
-    except (OSError, configparser.NoSectionError,
-            configparser.NoOptionError) as e:
+    except (
+        OSError,
+        configparser.NoSectionError,
+        configparser.NoOptionError,
+    ) as e:
         if isinstance(e, (OSError, configparser.NoSectionError)):
-            print("Adding sample versioneer config to setup.cfg",
-                  file=sys.stderr)
+            print(
+                "Adding sample versioneer config to setup.cfg", file=sys.stderr
+            )
             with open(os.path.join(root, "setup.cfg"), "a") as f:
                 f.write(SAMPLE_CONFIG)
         print(CONFIG_ERROR, file=sys.stderr)
         return 1
 
     print(" creating %s" % cfg.versionfile_source)
     with open(cfg.versionfile_source, "w") as f:
         LONG = LONG_VERSION_PY[cfg.VCS]
-        f.write(LONG % {"DOLLAR": "$",
-                        "STYLE": cfg.style,
-                        "TAG_PREFIX": cfg.tag_prefix,
-                        "PARENTDIR_PREFIX": cfg.parentdir_prefix,
-                        "VERSIONFILE_SOURCE": cfg.versionfile_source,
-                        })
+        f.write(
+            LONG
+            % {
+                "DOLLAR": "$",
+                "STYLE": cfg.style,
+                "TAG_PREFIX": cfg.tag_prefix,
+                "PARENTDIR_PREFIX": cfg.parentdir_prefix,
+                "VERSIONFILE_SOURCE": cfg.versionfile_source,
+            }
+        )
 
-    ipy = os.path.join(os.path.dirname(cfg.versionfile_source),
-                       "__init__.py")
+    ipy = os.path.join(os.path.dirname(cfg.versionfile_source), "__init__.py")
     if os.path.exists(ipy):
         try:
             with open(ipy, "r") as f:
                 old = f.read()
         except OSError:
             old = ""
         module = os.path.splitext(os.path.basename(cfg.versionfile_source))[0]
```

