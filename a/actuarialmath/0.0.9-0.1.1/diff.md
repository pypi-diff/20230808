# Comparing `tmp/actuarialmath-0.0.9.tar.gz` & `tmp/actuarialmath-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "actuarialmath-0.0.9.tar", last modified: Mon Jun 19 13:00:41 2023, max compression
+gzip compressed data, was "actuarialmath-0.1.1.tar", last modified: Tue Aug  8 19:35:34 2023, max compression
```

## Comparing `actuarialmath-0.0.9.tar` & `actuarialmath-0.1.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxr-x   0 terence   (1000) terence   (1000)        0 2023-06-19 13:00:41.621738 actuarialmath-0.0.9/
--rw-rw-r--   0 terence   (1000) terence   (1000)     1073 2023-05-29 19:44:46.000000 actuarialmath-0.0.9/LICENSE
--rw-rw-r--   0 terence   (1000) terence   (1000)     4241 2023-06-19 13:00:41.621738 actuarialmath-0.0.9/PKG-INFO
--rw-rw-r--   0 terence   (1000) terence   (1000)     4695 2023-06-19 12:18:05.000000 actuarialmath-0.0.9/README.md
--rw-rw-r--   0 terence   (1000) terence   (1000)     3719 2023-06-19 12:21:56.000000 actuarialmath-0.0.9/index.rst
--rw-rw-r--   0 terence   (1000) terence   (1000)      720 2023-06-19 13:00:36.000000 actuarialmath-0.0.9/pyproject.toml
--rw-rw-r--   0 terence   (1000) terence   (1000)       38 2023-06-19 13:00:41.621738 actuarialmath-0.0.9/setup.cfg
-drwxrwxr-x   0 terence   (1000) terence   (1000)        0 2023-06-19 13:00:41.621738 actuarialmath-0.0.9/src/
-drwxrwxr-x   0 terence   (1000) terence   (1000)        0 2023-06-19 13:00:41.621738 actuarialmath-0.0.9/src/actuarialmath/
--rw-rw-r--   0 terence   (1000) terence   (1000)      709 2023-06-18 20:31:22.000000 actuarialmath-0.0.9/src/actuarialmath/__init__.py
--rw-rw-r--   0 terence   (1000) terence   (1000)     4060 2023-06-19 03:40:47.000000 actuarialmath-0.0.9/src/actuarialmath/actuarial.py
--rw-rw-r--   0 terence   (1000) terence   (1000)    14866 2023-06-18 20:28:41.000000 actuarialmath-0.0.9/src/actuarialmath/annuity.py
--rw-rw-r--   0 terence   (1000) terence   (1000)     9386 2023-06-18 20:25:53.000000 actuarialmath-0.0.9/src/actuarialmath/constantforce.py
--rw-rw-r--   0 terence   (1000) terence   (1000)     3619 2023-06-18 20:25:38.000000 actuarialmath-0.0.9/src/actuarialmath/extrarisk.py
--rw-rw-r--   0 terence   (1000) terence   (1000)     9473 2023-06-18 20:28:59.000000 actuarialmath-0.0.9/src/actuarialmath/fractional.py
--rw-rw-r--   0 terence   (1000) terence   (1000)    21102 2023-06-19 02:29:40.000000 actuarialmath-0.0.9/src/actuarialmath/insurance.py
--rw-rw-r--   0 terence   (1000) terence   (1000)     5963 2023-06-18 20:29:37.000000 actuarialmath-0.0.9/src/actuarialmath/interest.py
--rw-rw-r--   0 terence   (1000) terence   (1000)     6862 2023-06-18 20:29:30.000000 actuarialmath-0.0.9/src/actuarialmath/life.py
--rw-rw-r--   0 terence   (1000) terence   (1000)    12178 2023-06-18 20:27:11.000000 actuarialmath-0.0.9/src/actuarialmath/lifetable.py
--rw-rw-r--   0 terence   (1000) terence   (1000)     2697 2023-06-18 20:29:07.000000 actuarialmath-0.0.9/src/actuarialmath/lifetime.py
--rw-rw-r--   0 terence   (1000) terence   (1000)    12027 2023-06-18 22:08:50.000000 actuarialmath-0.0.9/src/actuarialmath/mortalitylaws.py
--rw-rw-r--   0 terence   (1000) terence   (1000)    12437 2023-06-18 20:33:10.000000 actuarialmath-0.0.9/src/actuarialmath/mthly.py
--rw-rw-r--   0 terence   (1000) terence   (1000)    21095 2023-06-18 20:27:49.000000 actuarialmath-0.0.9/src/actuarialmath/policyvalues.py
--rw-rw-r--   0 terence   (1000) terence   (1000)     8824 2023-06-18 20:28:06.000000 actuarialmath-0.0.9/src/actuarialmath/premiums.py
--rw-rw-r--   0 terence   (1000) terence   (1000)    60459 2023-06-19 03:29:25.000000 actuarialmath-0.0.9/src/actuarialmath/recursion.py
--rw-rw-r--   0 terence   (1000) terence   (1000)    11674 2023-06-18 20:31:54.000000 actuarialmath-0.0.9/src/actuarialmath/reserves.py
--rw-rw-r--   0 terence   (1000) terence   (1000)    19564 2023-06-18 20:32:44.000000 actuarialmath-0.0.9/src/actuarialmath/selectlife.py
--rw-rw-r--   0 terence   (1000) terence   (1000)     7286 2023-06-18 20:27:01.000000 actuarialmath-0.0.9/src/actuarialmath/sult.py
--rw-rw-r--   0 terence   (1000) terence   (1000)     8385 2023-06-18 20:29:12.000000 actuarialmath-0.0.9/src/actuarialmath/survival.py
--rw-rw-r--   0 terence   (1000) terence   (1000)     9918 2023-06-18 20:24:33.000000 actuarialmath-0.0.9/src/actuarialmath/udd.py
--rw-rw-r--   0 terence   (1000) terence   (1000)     8098 2023-06-18 20:23:25.000000 actuarialmath-0.0.9/src/actuarialmath/woolhouse.py
-drwxrwxr-x   0 terence   (1000) terence   (1000)        0 2023-06-19 13:00:41.621738 actuarialmath-0.0.9/src/actuarialmath.egg-info/
--rw-rw-r--   0 terence   (1000) terence   (1000)     4241 2023-06-19 13:00:41.000000 actuarialmath-0.0.9/src/actuarialmath.egg-info/PKG-INFO
--rw-rw-r--   0 terence   (1000) terence   (1000)      935 2023-06-19 13:00:41.000000 actuarialmath-0.0.9/src/actuarialmath.egg-info/SOURCES.txt
--rw-rw-r--   0 terence   (1000) terence   (1000)        1 2023-06-19 13:00:41.000000 actuarialmath-0.0.9/src/actuarialmath.egg-info/dependency_links.txt
--rw-rw-r--   0 terence   (1000) terence   (1000)       60 2023-06-19 13:00:41.000000 actuarialmath-0.0.9/src/actuarialmath.egg-info/requires.txt
--rw-rw-r--   0 terence   (1000) terence   (1000)       14 2023-06-19 13:00:41.000000 actuarialmath-0.0.9/src/actuarialmath.egg-info/top_level.txt
-drwxrwxr-x   0 terence   (1000) terence   (1000)        0 2023-06-19 13:00:41.621738 actuarialmath-0.0.9/tests/
--rw-rw-r--   0 terence   (1000) terence   (1000)     2019 2023-06-19 12:37:26.000000 actuarialmath-0.0.9/tests/test_changes.py
+drwxrwxr-x   0 terence   (1000) terence   (1000)        0 2023-08-08 19:35:34.326799 actuarialmath-0.1.1/
+-rw-rw-r--   0 terence   (1000) terence   (1000)     1073 2023-05-29 19:44:46.000000 actuarialmath-0.1.1/LICENSE
+-rw-rw-r--   0 terence   (1000) terence   (1000)     4228 2023-08-08 19:35:34.326799 actuarialmath-0.1.1/PKG-INFO
+-rw-rw-r--   0 terence   (1000) terence   (1000)     4275 2023-08-08 19:07:27.000000 actuarialmath-0.1.1/README.md
+-rw-rw-r--   0 terence   (1000) terence   (1000)     3706 2023-07-21 22:51:38.000000 actuarialmath-0.1.1/index.rst
+-rw-rw-r--   0 terence   (1000) terence   (1000)      825 2023-08-08 19:34:59.000000 actuarialmath-0.1.1/pyproject.toml
+-rw-rw-r--   0 terence   (1000) terence   (1000)       38 2023-08-08 19:35:34.326799 actuarialmath-0.1.1/setup.cfg
+drwxrwxr-x   0 terence   (1000) terence   (1000)        0 2023-08-08 19:35:34.322799 actuarialmath-0.1.1/src/
+drwxrwxr-x   0 terence   (1000) terence   (1000)        0 2023-08-08 19:35:34.326799 actuarialmath-0.1.1/src/actuarialmath/
+-rw-rw-r--   0 terence   (1000) terence   (1000)      709 2023-06-18 20:31:22.000000 actuarialmath-0.1.1/src/actuarialmath/__init__.py
+-rw-rw-r--   0 terence   (1000) terence   (1000)     4628 2023-08-06 10:06:35.000000 actuarialmath-0.1.1/src/actuarialmath/actuarial.py
+-rw-rw-r--   0 terence   (1000) terence   (1000)    18993 2023-08-07 10:11:33.000000 actuarialmath-0.1.1/src/actuarialmath/annuity.py
+-rw-rw-r--   0 terence   (1000) terence   (1000)     9460 2023-08-08 10:17:19.000000 actuarialmath-0.1.1/src/actuarialmath/constantforce.py
+-rw-rw-r--   0 terence   (1000) terence   (1000)     4107 2023-08-08 13:38:44.000000 actuarialmath-0.1.1/src/actuarialmath/extrarisk.py
+-rw-rw-r--   0 terence   (1000) terence   (1000)     9981 2023-08-05 16:06:03.000000 actuarialmath-0.1.1/src/actuarialmath/fractional.py
+-rw-rw-r--   0 terence   (1000) terence   (1000)    26280 2023-08-07 19:22:12.000000 actuarialmath-0.1.1/src/actuarialmath/insurance.py
+-rw-rw-r--   0 terence   (1000) terence   (1000)     6411 2023-08-04 12:27:38.000000 actuarialmath-0.1.1/src/actuarialmath/interest.py
+-rw-rw-r--   0 terence   (1000) terence   (1000)     7383 2023-08-03 22:39:09.000000 actuarialmath-0.1.1/src/actuarialmath/life.py
+-rw-rw-r--   0 terence   (1000) terence   (1000)    12593 2023-08-08 17:42:30.000000 actuarialmath-0.1.1/src/actuarialmath/lifetable.py
+-rw-rw-r--   0 terence   (1000) terence   (1000)     2671 2023-08-04 18:40:16.000000 actuarialmath-0.1.1/src/actuarialmath/lifetime.py
+-rw-rw-r--   0 terence   (1000) terence   (1000)    12448 2023-08-08 10:21:18.000000 actuarialmath-0.1.1/src/actuarialmath/mortalitylaws.py
+-rw-rw-r--   0 terence   (1000) terence   (1000)    13019 2023-08-08 17:52:30.000000 actuarialmath-0.1.1/src/actuarialmath/mthly.py
+-rw-rw-r--   0 terence   (1000) terence   (1000)    24446 2023-08-08 18:39:00.000000 actuarialmath-0.1.1/src/actuarialmath/policyvalues.py
+-rw-rw-r--   0 terence   (1000) terence   (1000)     9792 2023-08-07 20:05:32.000000 actuarialmath-0.1.1/src/actuarialmath/premiums.py
+-rw-rw-r--   0 terence   (1000) terence   (1000)    77262 2023-08-08 16:59:18.000000 actuarialmath-0.1.1/src/actuarialmath/recursion.py
+-rw-rw-r--   0 terence   (1000) terence   (1000)    12162 2023-08-08 08:57:47.000000 actuarialmath-0.1.1/src/actuarialmath/reserves.py
+-rw-rw-r--   0 terence   (1000) terence   (1000)    20866 2023-08-08 18:21:46.000000 actuarialmath-0.1.1/src/actuarialmath/selectlife.py
+-rw-rw-r--   0 terence   (1000) terence   (1000)     7554 2023-06-21 23:27:12.000000 actuarialmath-0.1.1/src/actuarialmath/sult.py
+-rw-rw-r--   0 terence   (1000) terence   (1000)     9169 2023-08-05 15:22:31.000000 actuarialmath-0.1.1/src/actuarialmath/survival.py
+-rw-rw-r--   0 terence   (1000) terence   (1000)    10282 2023-08-08 17:45:34.000000 actuarialmath-0.1.1/src/actuarialmath/udd.py
+-rw-rw-r--   0 terence   (1000) terence   (1000)     8313 2023-08-08 17:49:28.000000 actuarialmath-0.1.1/src/actuarialmath/woolhouse.py
+drwxrwxr-x   0 terence   (1000) terence   (1000)        0 2023-08-08 19:35:34.326799 actuarialmath-0.1.1/src/actuarialmath.egg-info/
+-rw-rw-r--   0 terence   (1000) terence   (1000)     4228 2023-08-08 19:35:34.000000 actuarialmath-0.1.1/src/actuarialmath.egg-info/PKG-INFO
+-rw-rw-r--   0 terence   (1000) terence   (1000)      935 2023-08-08 19:35:34.000000 actuarialmath-0.1.1/src/actuarialmath.egg-info/SOURCES.txt
+-rw-rw-r--   0 terence   (1000) terence   (1000)        1 2023-08-08 19:35:34.000000 actuarialmath-0.1.1/src/actuarialmath.egg-info/dependency_links.txt
+-rw-rw-r--   0 terence   (1000) terence   (1000)       60 2023-08-08 19:35:34.000000 actuarialmath-0.1.1/src/actuarialmath.egg-info/requires.txt
+-rw-rw-r--   0 terence   (1000) terence   (1000)       14 2023-08-08 19:35:34.000000 actuarialmath-0.1.1/src/actuarialmath.egg-info/top_level.txt
+drwxrwxr-x   0 terence   (1000) terence   (1000)        0 2023-08-08 19:35:34.326799 actuarialmath-0.1.1/tests/
+-rw-rw-r--   0 terence   (1000) terence   (1000)     2019 2023-06-19 12:37:26.000000 actuarialmath-0.1.1/tests/test_changes.py
```

### Comparing `actuarialmath-0.0.9/LICENSE` & `actuarialmath-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `actuarialmath-0.0.9/PKG-INFO` & `actuarialmath-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: actuarialmath
-Version: 0.0.9
+Version: 0.1.1
 Summary: A package for actuarial math and life contingent risks
 Author: Terence Lim
 Project-URL: Homepage, https://terence-lim.github.io/actuarialmath-guide
 Project-URL: Bug Tracker, https://github.com/terence-lim/actuarialmath/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -35,19 +35,19 @@
 
    - Extra mortality risks
 
    - 1/mthly payment frequency using UDD or Woolhouse approaches
 
 3. Specify and load a particular form of assumptions
 
+   - Recursion inputs
+
    - Life table, select life table, or standard ultimate life table
 
    - Mortality laws, such as constant force of maturity, beta and uniform distributions, or Makeham's and Gompertz's laws
-
-   - Recursion inputs
     
      
 Quick Start
 -----------
 
 1. ``pip install actuarialmath``
    
@@ -63,29 +63,29 @@
 
 Examples
 --------
 
 ::
 
   # SOA FAM-L sample question 5.7
-  from actuarialmath.recursion import Recursion, Woolhouse
+  from actuarialmath import Recursion, Woolhouse
   # initialize Recursion class with actuarial inputs
   life = Recursion().set_interest(i=0.04)\
                     .set_A(0.188, x=35)\
                     .set_A(0.498, x=65)\
                     .set_p(0.883, x=35, t=30)
   # modfy the standard results with Woolhouse mthly approximation
   mthly = Woolhouse(m=2, life=life, three_term=False)
   # compute the desired temporary annuity value
   print(1000 * mthly.temporary_annuity(35, t=30)) #   solution = 17376.7
 
 ::
 
   # SOA FAM-L sample question 7.20
-  from actuarialmath.sult import SULT, Contract
+  from actuarialmath import SULT, Contract
   life = SULT()
   # compute the required FPT policy value
   S = life.FPT_policy_value(35, t=1, b=1000)  # is always 0 in year 1!
   # input the given policy contract terms
   contract = Contract(benefit=1000,
                       initial_premium=.3,
                       initial_policy=300,
@@ -98,13 +98,13 @@
   print(R-S)   # solution = -277.19
 
 Resources
 ---------
 
 1. `Colab <https://colab.research.google.com/drive/1TcNr1x5HbT2fF3iFMYGXdN_cvRKiSua4?usp=sharing>`_ or `Jupyter notebook <https://terence-lim.github.io/notes/faml.ipynb>`_, to solve all sample SOA FAM-L exam questions
 
-2. `User Guide <https://terence-lim.github.io/actuarialmath-guide/>`_, or `download pdf <https://terence-lim.github.io/notes/actuarialmath-guide.pdf>`_
+2. `Online User Guide <https://terence-lim.github.io/actuarialmath-guide/>`_, or `download pdf <https://terence-lim.github.io/notes/actuarialmath-guide.pdf>`_
 
-3. `Code documentation <https://actuarialmath.readthedocs.io/en/latest/>`_
+3. `API reference <https://actuarialmath.readthedocs.io/en/latest/>`_
 
 4. `Github repo <https://github.com/terence-lim/actuarialmath.git>`_ and `issues <https://github.com/terence-lim/actuarialmath/issues>`_
```

### Comparing `actuarialmath-0.0.9/README.md` & `actuarialmath-0.1.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-# Introduction
+# USER GUIDE
 
 __actuarialmath -- Life Contingent Risks with Python__
 
-This Python package implements fundamental methods for modeling life contingent risks, and closely follows the coverage of traditional topics in actuarial exams and standard texts such as the "Fundamentals of Actuarial Math - Long-term" exam syllabus by the Society of Actuaries, and "Actuarial Mathematics for Life Contingent Risks" by Dickson, Hardy and Waters.
-The resources listed below should be helpful for getting started. The code chunks in this complete [Colab](https://colab.research.google.com/drive/1TcNr1x5HbT2fF3iFMYGXdN_cvRKiSua4?usp=sharing), or [Jupyter notebook](https://terence-lim.github.io/notes/faml.ipynb), demonstrate how to solve each of the sample FAM-L exam questions released by the SOA.
+This Python package implements fundamental methods for modeling life contingent risks, and closely follows the coverage of traditional topics in actuarial exams and standard texts such as the "Fundamentals of Actuarial Math - Long-term" exam syllabus by the Society of Actuaries, and "Actuarial Mathematics for Life Contingent Risks" by Dickson, Hardy and Waters.  The actuarial concepts, and corresponding Python classes, are introduced and modeled hierarchically.
 
-The actuarial concepts, as shown in this graphic, are introduced and modeled hierarchically, and realized by corresponding derivations of Python classes.
 
-![classes](FAM-L.png)
+![classes and concepts](FAM-L.png)
+
 
 ## Quick Start
 
 1. `pip install actuarialmath`
 
    - also requires `numpy`, `scipy`, `matplotlib` and `pandas`.
 
 
 2. Start Python (version >= 3.10) or Jupyter-notebook
 
 
-   - Select and import a suitable subclass to initialize with your actuarial assumptions, such as `MortalityLaws` (or a special law like `ConstantForce`), `LifeTable`, `SULT`, `SelectLife` or `Recursion`.
+   - Select a suitable subclass to initialize with your actuarial assumptions, such as `MortalityLaws` (or a special law like `ConstantForce`), `LifeTable`, `SULT`, `SelectLife` or `Recursion`.
 
    - Call appropriate methods to compute intermediate or final results, or to `solve` parameter values implicitly.
 
-   - Adjust the answers with `ExtraRisk` or `Mthly` (or its `UDD` or `Woolhouse`) classes.
+   - Adjust answers with `ExtraRisk` or `Mthly` (or its `UDD` or `Woolhouse`) classes
+
 
 ## Examples
 
 __SOA FAM-L sample question 5.7__: 
 
 Given $A_{35} = 0.188$, $A_{65} = 0.498$, $S_{35}(30) = 0.883$, calculate the EPV of a temporary annuity $\ddot{a}^{(2)}_{35:\overline{30|}}$ paid half-yearly using the Woolhouse approximation.
 
 ```
-from actuarialmath.recursion import Recursion, Woolhouse
+from actuarialmath import Recursion, Woolhouse
 # initialize Recursion class with actuarial inputs
 life = Recursion().set_interest(i=0.04)\
                   .set_A(0.188, x=35)\
                   .set_A(0.498, x=65)\
                   .set_p(0.883, x=35, t=30)
 # modfy the standard results with Woolhouse mthly approximation
 mthly = Woolhouse(m=2, life=life, three_term=False)
@@ -54,15 +54,15 @@
 - The gross premium policy value at the end of the first policy year is R
 - Using the Full Preliminary Term Method, the modified reserve at the end of the first policy year is S
 - Mortality follows the Standard Ultimate Life Table
 - _i_ = 0.05
 
 Calculate R − S
 ```
-from actuarialmath.sult import SULT, Contract
+from actuarialmath import SULT, Contract
 life = SULT()
 # compute the required FPT policy value
 S = life.FPT_policy_value(35, t=1, b=1000)  # is always 0 in year 1!
 # input the given policy contract terms
 contract = Contract(benefit=1000,
                     initial_premium=.3,
                     initial_policy=300,
@@ -76,17 +76,17 @@
 ```
 
 
 ## Resources
 
 1. [Colab](https://colab.research.google.com/drive/1TcNr1x5HbT2fF3iFMYGXdN_cvRKiSua4?usp=sharing) or [Jupyter notebook](https://terence-lim.github.io/notes/faml.ipynb), to solve all sample SOA FAM-L exam questions
 
-2. [User Guide](https://terence-lim.github.io/actuarialmath-guide/), or [download pdf](https://terence-lim.github.io/notes/actuarialmath-guide.pdf)
+2. [Online User Guide](https://terence-lim.github.io/actuarialmath-guide/), or [download pdf](https://terence-lim.github.io/notes/actuarialmath-guide.pdf)
 
-3. [Code documentation](https://actuarialmath.readthedocs.io/en/latest/)
+3. [API reference](https://actuarialmath.readthedocs.io/en/latest/)
 
 4. [Github repo](https://github.com/terence-lim/actuarialmath.git) and [issues](https://github.com/terence-lim/actuarialmath/issues)
 
 
 
 ## Sources
```

### Comparing `actuarialmath-0.0.9/index.rst` & `actuarialmath-0.1.1/index.rst`

 * *Files 6% similar despite different names*

```diff
@@ -21,19 +21,19 @@
 
    - Extra mortality risks
 
    - 1/mthly payment frequency using UDD or Woolhouse approaches
 
 3. Specify and load a particular form of assumptions
 
+   - Recursion inputs
+
    - Life table, select life table, or standard ultimate life table
 
    - Mortality laws, such as constant force of maturity, beta and uniform distributions, or Makeham's and Gompertz's laws
-
-   - Recursion inputs
     
      
 Quick Start
 -----------
 
 1. ``pip install actuarialmath``
    
@@ -49,29 +49,29 @@
 
 Examples
 --------
 
 ::
 
   # SOA FAM-L sample question 5.7
-  from actuarialmath.recursion import Recursion, Woolhouse
+  from actuarialmath import Recursion, Woolhouse
   # initialize Recursion class with actuarial inputs
   life = Recursion().set_interest(i=0.04)\
                     .set_A(0.188, x=35)\
                     .set_A(0.498, x=65)\
                     .set_p(0.883, x=35, t=30)
   # modfy the standard results with Woolhouse mthly approximation
   mthly = Woolhouse(m=2, life=life, three_term=False)
   # compute the desired temporary annuity value
   print(1000 * mthly.temporary_annuity(35, t=30)) #   solution = 17376.7
 
 ::
 
   # SOA FAM-L sample question 7.20
-  from actuarialmath.sult import SULT, Contract
+  from actuarialmath import SULT, Contract
   life = SULT()
   # compute the required FPT policy value
   S = life.FPT_policy_value(35, t=1, b=1000)  # is always 0 in year 1!
   # input the given policy contract terms
   contract = Contract(benefit=1000,
                       initial_premium=.3,
                       initial_policy=300,
@@ -84,13 +84,13 @@
   print(R-S)   # solution = -277.19
 
 Resources
 ---------
 
 1. `Colab <https://colab.research.google.com/drive/1TcNr1x5HbT2fF3iFMYGXdN_cvRKiSua4?usp=sharing>`_ or `Jupyter notebook <https://terence-lim.github.io/notes/faml.ipynb>`_, to solve all sample SOA FAM-L exam questions
 
-2. `User Guide <https://terence-lim.github.io/actuarialmath-guide/>`_, or `download pdf <https://terence-lim.github.io/notes/actuarialmath-guide.pdf>`_
+2. `Online User Guide <https://terence-lim.github.io/actuarialmath-guide/>`_, or `download pdf <https://terence-lim.github.io/notes/actuarialmath-guide.pdf>`_
 
-3. `Code documentation <https://actuarialmath.readthedocs.io/en/latest/>`_
+3. `API reference <https://actuarialmath.readthedocs.io/en/latest/>`_
 
 4. `Github repo <https://github.com/terence-lim/actuarialmath.git>`_ and `issues <https://github.com/terence-lim/actuarialmath/issues>`_
```

### Comparing `actuarialmath-0.0.9/pyproject.toml` & `actuarialmath-0.1.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,37 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "actuarialmath"
-#version =  "0.0.100"
-version = "0.0.9" 
+version =  "0.1.1"
+#version = "0.0.15" 
 authors = [
   { name="Terence Lim"},
 ]
 description = "A package for actuarial math and life contingent risks"
 readme = "index.rst"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
+#dependencies = [
+#  "matplotlib>=3.7.1",
+#  "numpy>=1.24.3",
+#  "pandas>=2.0.2",
+#  "scipy>=1.10.1",
+#]
+
 dependencies = [
   "matplotlib>=3.7.1",
-  "numpy>=1.24.3",
-  "pandas>=2.0.2",
+  "numpy>=1.22.4",
+  "pandas>=1.5.3",
   "scipy>=1.10.1",
 ]
 
 [project.urls]
 "Homepage" = "https://terence-lim.github.io/actuarialmath-guide"
 "Bug Tracker" = "https://github.com/terence-lim/actuarialmath/issues"
```

### Comparing `actuarialmath-0.0.9/src/actuarialmath/__init__.py` & `actuarialmath-0.1.1/src/actuarialmath/__init__.py`

 * *Files identical despite different names*

### Comparing `actuarialmath-0.0.9/src/actuarialmath/actuarial.py` & `actuarialmath-0.1.1/src/actuarialmath/actuarial.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 """
 import math
 import numpy as np
 import scipy
 import matplotlib.pyplot as plt
 from typing import Callable, Any, Tuple, List
 
-plt.style.use('ggplot')
+plt.style.use('seaborn-dark') # 'ggplot'
 
 class Actuarial(object):
     """Define constants and common utility functions
 
     Constants:
       VARIANCE : select variance as the statistical moment to calculate
 
@@ -21,57 +21,73 @@
     # constants
     VARIANCE = -2
     WHOLE = -999
     _VARIANCE = VARIANCE
     _WHOLE = WHOLE
     _TOL = 1e-6
     _verbose = 0
-    _MAXAGE = 130    # default oldest age
+    _MAXAGE = 100    # default oldest age
     _MINAGE = 0      # default youngest age
 
     #
     # Helpers for numerical computations
     #
     @staticmethod
+    def isclose(r: float, target: float = 0., abs_tol=1e-6) -> bool:
+        """Is close to zero or target value
+        
+        Args:
+          r : value to test if close to zero or target
+          target : target value, default is 0.0
+        """
+        return math.isclose(r, target, abs_tol=abs_tol)
+    
+    @staticmethod
     def integral(fun: Callable[[float], float],
-                 lower: float,
-                 upper: float) -> float:
+                 lower: float, upper: float) -> float:
         """Compute integral of the function between lower and upper limits
         
         Args:
           fun : function to integrate
-          lower : lower limit
           upper : upper limit
+          lower : lower limit
         """
         y = scipy.integrate.quad(fun, lower, upper, full_output=1)
         return y[0]
 
     @staticmethod
     def derivative(fun: Callable[[float], float], x: float) -> float:
         """Compute derivative of the function at a value
         
         Args:
           fun : function to compute derivative
           x : value to compute derivative at
+
+        Examples:
+          >>> print(Actuarial.derivative(fun=lambda x: x/50, x=25))
         """
         return scipy.misc.derivative(fun, x0=x, dx=1)
 
     @staticmethod
     def solve(fun: Callable[[float], float], target: float, 
               grid: float | Tuple | List, mad: bool = False) -> float:
-        """Solve for the root of, or parameter value that minimizes, a function
+        """Solve root, or parameter that minimizes absolute value, of a function
 
         Args:
           fun : function to compute output given input values
           target : target value of function output
           grid : initial range of guesses
-          root : whether solve root (True), or minimize absolute deviation (False)
+          root : whether to solve root (True), or minimize absolute function (False)
 
         Returns:
           value s.t. output of function fun(value) ~ target
+
+        Examples:
+          >>> print(Actuarial.solve(fun=lambda omega: 1/omega, 
+          >>>                       target=0.05, grid=[1, 100]))
         """
         if mad:   # minimize absolute difference
             f = lambda t: abs(fun(t) - target)
             return scipy.optimize.minimize_scalar(f, grid).x    
         else:     # solve root
             f = lambda x: fun(x) - target
             if isinstance(grid, (list, tuple)):
```

### Comparing `actuarialmath-0.0.9/src/actuarialmath/annuity.py` & `actuarialmath-0.1.1/src/actuarialmath/mortalitylaws.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,379 +1,337 @@
-"""Life annuities - Computes present values of annuity benefits
+"""Mortality Laws: Applies shortcut formulas for Beta, Uniform, Makeham and Gompertz
 
-MIT License. Copyright (c) 2022-2023 Terence Lim
+MIT License. Copyright 2022-2023 Terence Lim
 """
-from typing import Callable, Any
 import math
-import matplotlib.pyplot as plt
-import numpy as np
-from actuarialmath import Insurance
+from actuarialmath import Reserves
 
-class Annuity(Insurance):
-    """Compute present values and relationships of life annuities"""
+class MortalityLaws(Reserves):
+    """Apply shortcut formulas for special mortality laws"""
 
-    def a_x(self, x: int, s: int = 0, t: int = Insurance.WHOLE, u: int = 0,
-            benefit: Callable = lambda x,t: 1, discrete: bool = True) -> float:
-        """Numerically compute EPV of annuities from survival functions
-
-        Args:
-          x : age of selection
-          s : years after selection
-          u : year deferred
-          t : term of insurance
-          benefit : benefit as a function of age and year
-          discrete : annuity due (True) or continuous (False)
-        """
-        t = self.max_term(x+s+u, t=t)
-        if discrete:
-            a = sum([benefit(x+s, k) * self.interest.v_t(k) 
-                     * self.p_x(x, s=s, t=k) for k in range(u, t+u)])
-        else:   # use continuous first principles
-            Y = lambda t: (benefit(x+s, t+u) * self.interest.v_t(t+u) 
-                           * self.S(x, 0, t=t+u))
-            a = self.integral(Y, 0, t)
-        return a
-
-
-    def immediate_annuity(self, x: int, s: int = 0, t: int = Insurance.WHOLE, 
-                          b: int = 1, variance=False) -> float:
-        """Compute EPV of immediate life annuity
-
-        Args:
-          x : age of selection
-          s : years after selection
-          t : term of insurance
-          b : benefit amount
-          variance : return EPV (False) or variance (True)
-        """
-        if variance:
-            return self.temporary_annuity(x, s=s, t=self.add_term(t, 1), b=b,
-                                          discrete=True, variance=True)
-        return (self.temporary_annuity(x, s=s, t=t, discrete=True) 
-                - 1 + self.E_x(x, s=s, t=t)) * b
+    def __init__(self, **kwargs):
+        assert 'udd' not in kwargs, "Fractional age must assume same mortality law"
+        super().__init__(**kwargs)
     
-    def annuity_twin(self, A: float, discrete: bool = True) -> float:
-        """Returns annuity from its WL or Endowment Insurance twin"
-
-        Args:
-          A : cost of insurance
-          discrete : discrete/annuity due (True) or continuous (False)
-        """
-        interest = (self.interest.d if discrete else self.interest.delta)
-        return ((1 - A) / interest) if interest else 1 - A
-
-    def insurance_twin(self, a: float, moment: int = 1, 
-                       discrete: bool = True) -> float:
-        """Returns WL or Endowment Insurance twin from annuity
-
-        Args:
-          a : cost of annuity
-          discrete : discrete/annuity due (True) or continuous (False)
-        """
-        assert moment in [1]
-        interest = (self.interest.d if discrete else self.interest.delta)
-        return 1 - a*interest
-  
-    def annuity_variance(self, A2: float, A1: float, b: float = 1.,
-                         discrete: bool = True) -> float:
-        """Compute variance from WL or endowment insurance twin
-
-        Args:
-          A2 : second moment of insurance factor
-          A1 : first moment of insurance factor
-          b : annuity benefit amount
-          discrete : discrete/annuity due (True) or continuous (False)
-        """
-        interest = (self.interest.d if discrete else self.interest.delta)
-        if interest == 0:
-            return b**2 * self.insurance_variance(A2=A2, A1=A1)
-        else:
-            return (b**2 * self.insurance_variance(A2=A2, A1=A1) / interest**2)
-
-    def whole_life_annuity(self, x: int, s: int = 0, b: int = 1, 
-                           variance: bool = False, 
-                           discrete: bool = True) -> float:
-        """Whole life annuity: a_x
+    #
+    # Fractional age actuarial survival functions can use continuous laws
+    #
+    def l_r(self, x: int, s: int = 0, r: float = 0.) -> float:
+        """Fractional lives given special mortality law: l_[x]+s+r
 
         Args:
           x : age of selection
           s : years after selection
-          b : annuity benefit amount
-          variance : return EPV (True) or variance (False)
-          discrete : annuity due (True) or continuous (False)
+          r : fractional year after selection
         """
-        interest = self.interest.d if discrete else self.interest.delta
-        if variance:  # short cut for variance of whole life
-            A1 = self.whole_life_insurance(x, s=s, moment=1, discrete=discrete)
-            A2 = self.whole_life_insurance(x, s=s, moment=2, discrete=discrete)
-            return self.annuity_variance(A2=A2, A1=A1, discrete=discrete, b=b)
-        if interest > 0:
-            A = self.whole_life_insurance(x, s=s, discrete=discrete)
-            return b * (1 - A) / interest if interest > 0 else b * (1 - A)
-        else:  # when interest=1, annuity is expected life time (+1 if discrete)
-            return discrete + self.e_x(x=x, s=s, curtate=discrete)
+        return self.l(x, s+r)
 
-            
-    def temporary_annuity(self, x: int, s: int = 0, t: int = Insurance.WHOLE, 
-                          b: int = 1, variance: bool = False, 
-                          discrete: bool = True) -> float:
-        """Temporary life annuity: a_x:t
+    def p_r(self, x: int, s: int = 0, r: float = 0., t: float = 1.) -> float:
+        """Fractional age survival probability given special mortality law
 
         Args:
           x : age of selection
           s : years after selection
-          t : term of annuity in years
-          b (int) : annuity benefit amount
-          variance : return EPV (True) or variance (False)
-          discrete : annuity due (True) or continuous (False)
+          r : fractional year after selection
+          t : death within next t fractional years
         """
-        if variance:  # short cut for variance of temporary life annuity
-            A1 = self.endowment_insurance(x, s=s, t=t, discrete=discrete)
-            A2 = self.endowment_insurance(x, s=s, t=t, moment=2, 
-                                          discrete=discrete)
-            return self.annuity_variance(A2=A2, A1=A1, discrete=discrete, b=b)
-
-        # difference of whole life on (x) and deferred whole life on (x+t)
-        a = self.whole_life_annuity(x, s=s, b=b, discrete=discrete)
-        if t < 0 or self.max_term(x+s, t) < t:
-            return a
-        a_t = self.whole_life_annuity(x, s=s+t, b=b, discrete=discrete)
-        return a - (a_t * self.E_x(x, s=s, t=t))
+        return self.S(x, s+r, t)
 
-    def deferred_annuity(self, x: int, s: int = 0, u: int = 0, 
-                         t: int = Insurance.WHOLE, b: int = 1, 
-                         discrete: bool = True) -> float:
-        """Deferred life annuity n|t_a_x =  n+t_a_x - n_a_x
+    def q_r(self, x: int, s: int = 0, r: float = 0., t: float = 1., 
+            u: float = 0.) -> float:
+        """Fractional age deferred mortality given special mortality law
 
         Args:
           x : age of selection
           s : years after selection
-          u : years deferred
-          t : term of annuity in years
-          b : annuity benefit amount
-          discrete : annuity due (True) or continuous (False)
-        """
-        a = self.temporary_annuity(x, s=s+u, t=t, b=b, discrete=discrete)
-        return self.E_x(x, s=s, t=u) * a
-
-    def certain_life_annuity(self, x: int, s: int = 0, u: int = 0, 
-                             t: int = Insurance.WHOLE, b: int = 1, 
-                             discrete: bool = True) -> float:
-        """Certain and life annuity = certain + deferred
+          r : fractional year after selection
+          u : survive u fractional years, then...
+          t : death within next t fractional years
+        """
+        return self.p_r(x, s=s, r=r, t=u) - self.p_r(x, s=s, r=r, t=t+u)
+        
+    def mu_r(self, x: int, s: int = 0, r: float = 0.) -> float:
+        """Fractional age force of mortality given special mortality law
 
         Args:
           x : age of selection
           s : years after selection
-          u : years of certain annuity
-          t : term of life annuity in years
-          b : annuity benefit amount
-          discrete : annuity due (True) or continuous (False)
+          r : fractional year after selection
         """
-        u = self.max_term(x+s, u)
-        if u < 0:
-            return 0.
-        a = self.deferred_annuity(x, s=s, u=u, t=t, b=b, discrete=discrete)
-        return self.interest.annuity(u, m=int(discrete)) + a
+        return self.mu(x, s+r)
 
-    def increasing_annuity(self, x: int, s: int = 0, t: int = Insurance.WHOLE, 
-                           b: int = 1, discrete: bool = True) -> float:
-        """Increasing annuity
+    def f_r(self, x: int, s: int = 0, r: float = 0., t: float = 0.0) -> float:
+        """fractional age lifetime density given special mortality law
 
         Args:
           x : age of selection
           s : years after selection
-          t : term of life annuity in years
-          b : benefit amount at end of first year
-          discrete : annuity due (True) or continuous (False)
+          r : fractional year after selection
+          t : mortality at fractional year t
         """
-        t = self.max_term(x+s, t=t)
-        benefit = lambda x, s: b * (s + 1) # increasing benefit
-        return self.a_x(x, s=s, benefit=benefit, t=t, discrete=discrete)
+        return self.f(x, s+r, t)
 
-    def decreasing_annuity(self, x: int, s: int = 0, t: int = 0, 
-                           b: int = 1, discrete: bool = True) -> float:
-        """Identity (Da)_x:n + (Ia)_x:n = (n+1) a_x:n temporary annuity
+    def e_r(self, x: int, s: int = 0, r: float = 0.,
+            t: float = Reserves.WHOLE) -> float:
+        """Fractional age future lifetime given special mortality law
 
         Args:
           x : age of selection
           s : years after selection
-          t : term of life annuity in years
-          b : benefit amount at end of first year
-          discrete : annuity due (True) or continuous (False)
+          r : fractional year after selection
+          t : limited at t years
         """
-        assert t >= 0   # decreasing must be till term
-        t = self.max_term(x+s, t=t)
-        a = self.temporary_annuity(x, s=s, t=t, discrete=discrete)
-        n = t + int(discrete)
-        return b * (a*n - self.increasing_annuity(x, s=s, t=t, discrete=discrete))
+        if t < 0:
+            t = self._MAXAGE - (x + s + r)
+        return self.integrate(lambda t: self.S(x, s+r, t), 0., float(t))
 
-    #
-    # Annuity random variable: Y(t)
-    #
-    def Y_t(self, x: int, prob: float, discrete: bool = True) -> float:
-        """T_x given percentile of the r.v. Y = PV of WL or Temporary Annuity
+class Beta(MortalityLaws):
+    """Shortcuts with beta distribution of deaths (is Uniform when alpha = 1)
 
-        Args:
-          x : age of selection
-          prob : desired probability threshold
-          discrete : annuity due (True) or continuous (False)
-        """
-        assert prob < 1.0
-        t = self.solve(lambda t: self.S(x, 0, t), target=1-prob, grid=25)
-        return math.floor(t) if discrete else t   # opposite of insurance
+    Args:
+      omega : maximum age
+      alpha : alpha paramter of beta distribution
+      radix : assumed starting number of lives for survival function
 
-    def Y_from_t(self, t: float, discrete: bool = True) -> float:
-        """PV of insurance payment Y(t), given T_x (or K_x if discrete)
+    Examples:
+      >>> print(Beta(omega=60, alpha=1/3).mu_x(35) * 1000)
+    """
 
-        Args:
-          t : year of death
-          discrete : annuity due (True) or continuous (False)
-        """
-        if self.interest.delta == 0.:  # return number of payments if interest=0
-            return math.floor(t) + 1 if discrete else t
-        if discrete:
-            return (1 - self.interest.v_t(math.floor(t) + 1)) / self.interest.d
-        else:
-            return (1 - self.interest.v_t(t)) / self.interest.delta
+    def __init__(self, omega: int, alpha: float,
+                 radix: int = MortalityLaws._RADIX, **kwargs): 
+        """Two parameters: alpha and omega, with mu(x) = alpha/(omega-x)"""
 
-    def Y_to_t(self, Y: float) -> float:
-        """T_x  s.t. PV of annuity payments is Y
+        super().__init__(**kwargs)
 
-        Args:
-          Y : Present value of benefits paid
-        """
-        if self.interest.v == 0.:
-            return Y
-        else:
-            return math.log(1 - self.interest.delta*Y) / math.log(self.interest.v)
+        def _mu(x: int, s: float) -> float: 
+            return alpha / (omega - (x+s))
 
+        def _l(x: int, s: float) -> float:
+            return radix * (omega - (x+s))**alpha
 
-    def Y_from_prob(self, x: int, prob: float, discrete: bool = True) -> float:
-        """Percentile of annuity PV r.v. Y, given probability
+        def _S(x: int, s,t : float) -> float:
+            return ((omega-(x+s+t))/(omega-(x+s)))**alpha
 
-        Args:
-          x : age initially insured
-          prob : desired probability threshold
-          discrete : annuity due (True) or continuous (False)
-        """
-        t = self.Y_t(x, prob, discrete=discrete)
-        return self.Y_from_t(t=t, discrete=discrete)
-
-    def Y_to_prob(self, x: int, Y: float) -> float:
-        """Cumulative density of insurance PV r.v. Y, given percentile value
+        def _f(x: int, s,t : float) -> float:
+            return alpha / (omega - (x+s))
 
-        Args:
-          x : age initially insured
-          Y : present value of benefits paid
-        """
-        t = self.Y_to_t(Y)
-        return 1 - self.S(x, 0, t)   # opposite of Insurance
+        self.set_survival(mu=_mu, l=_l, S=_S, f=_f, minage=0, maxage=omega)
+        self.omega_ = omega  # store omega parameter
+        self.alpha_ = alpha  # store alpha parameter
 
-    def Y_x(self, x, s: int = 0, t: int = 1, discrete: bool = True) -> float:
-        """EPV of year t annuity benefit for life aged [x]+s: b_x[s]+s(t)
+    def e_r(self, x: int, s: int = 0, t: float = Reserves.WHOLE) -> float:
+        """Expectation of future lifetime through fractional age: e_[x]+s:t
 
         Args:
-          x : age initially insured
+          x : age of selection
           s : years after selection
-          t : year of benefit
-          discrete : annuity due (True) or continuous (False)
+          t : limited at t years
         """
-        assert t >= 0
-        if discrete:
-            return (self.interest.v_t(math.floor(t)) 
-                    * self.p_x(x, s=s, t=math.floor(t)))
-        else:
-            return (self.interest.v_t(t) * self.p_r(x, s=s, t=t))
+        e = (self.omega_ - (x+s)) / (self.alpha_ + 1)
+        if t > 0 and self.max_term(x+s, t) > t: # temporary expectation
+            return e - self.p_r(x, s=s, t=t) * self.e_r(x, s=s+t)
+        return e   # complete expectation
+
+    def e_x(self, x: int, s: int = 0, n: int = MortalityLaws.WHOLE, 
+          curtate: bool = False, moment: int = 1) -> float:
+        """Shortcut formula for complete expectation
 
-    def Y_plot(self, x: int, s: int = 0, stop : int = 0,
-               benefit: Callable = lambda x,k: 1,
-               T: float | None = None,
-               discrete: bool = True,
-               ax: Any = None,
-               title: str | None = None,               
-               color='r') -> float:
-        """Plot PV of annuity r.v. Y vs T
+        Args:
+          x : age of selection
+          s : years after selection
+          n : death within next n fractional years
+          t : limited at t years
+          curtate : whether curtate (True) or complete (False) lifetime
+          moment : whether to compute first (1) or second (2) moment
+        """
+        if n == 0:
+            return 0
+        if not curtate:
+            if moment == 1:
+                return self.e_r(x, s=s, t=n)
+            if moment == self.VARIANCE and n < 0: # shortcut for complete variance
+                return ((self.omega_ - (x + s))
+                        / ((self.alpha_ + 1)**2 * (self.alpha_ + 1)))
+        return super().e_x(x=x, s=s, n=n, curtate=curtate, moment=moment)
+
+class Uniform(Beta):
+    """Shortcuts with uniform distribution of deaths aka DeMoivre's Law
+
+    Args:
+      omega : maximum age
+
+    Examples:
+      >>> print(Uniform(95).e_x(30, t=40, curtate=False)) # 27.692
+    """
+
+    def __init__(self, omega: int, **kwargs):
+        """One parameter: omega = maxage, with mu(x) = 1/(omega - x)"""
+        super().__init__(omega=omega, alpha=1, **kwargs)
+
+    def e_x(self, x: int, s: int = 0, t: int = Beta.WHOLE, 
+          curtate: bool = False, moment: int = 1) -> float:
+        """Shortcut for expected future lifetime
 
         Args:
           x : age of selection
           s : years after selection
-          stop : time to end plot
-          benefit : benefit as a function of selection age and time
-          discrete : discrete or continuous insurance
-          ax : figure object to plot in
-          color : color to plot
-          title : title of plot
-        """
-        if ax is None:
-            fig, ax = plt.subplots(1, 1)
-        K = 'K' if discrete else 'T'
-        stop = stop or self._MAXAGE - (x + s)
-        step = 1 if discrete else stop / 1000.
-        steps = np.arange(0, stop + step, step)
+          t : limited at t years
+          curtate : whether curtate (True) or complete (False) lifetime
+          moment : whether to compute first (1) or second (2) moment
+        """
+        if moment in [1, self.VARIANCE] and not curtate:
+            if t < 0:
+                if moment == self.VARIANCE:
+                    return (self.omega_ - x)**2 / 12  # complete shortcut
+                else:
+                    return (self.omega_ - x) / 2
+            elif moment == 1:         # temporary expectation shortcut
+                # (Pr[die within n years] * n/2) plus (Pr[survive n years] * n)
+                t = self.max_term(x+s, t)
+                t_p_x = t / (self.omega_ - x)
+                return t_p_x * t  + (1 - t_p_x) * (t / 2)
+        return super().e_x(x=x, s=s, t=t, curtate=curtate, moment=moment)
 
-        # plot benefit values
-        y = [benefit(x, s+t) * self.Y_from_t(t, discrete=discrete) for t in steps]
-        if T is None:
-            ax.bar(steps, y, width=stepsize, alpha=0.5, color=color)
-            Y = None
-        else:
-            ax.step(steps, y, ':', c=color, where='pre' if discrete else 'post')
+    
+    def E_x(self, x: int, s: int = 0, t: int = Beta.WHOLE, 
+            moment: int = 1) -> float:
+        """Shortcut for Pure Endowment
 
-            xmin, xmax = ax.get_xlim()
-            ymin, ymax = ax.get_ylim()
-            yjig = (ymax - ymin) / 50
-            xjig = (xmax - xmin) / 50
-            
-            # indicate PV benefit Y(T*)
-            Y = self.Y_from_t(T, discrete=discrete) * benefit(self._MINAGE, T)
-            ax.plot(T, Y, c=color, marker='o')
-            ax.text(T + xjig, Y + 1*yjig, f"Y*={Y:.2f}", c=color)
+        Args:
+          x : age of selection
+          s : years after selection
+          t : term of pure endowment
+          endowment : amount of pure endowment
+          moment : compute first or second moment
+        """
+        assert moment > 0
+        if t == 0:
+            return 1.
+        if t < 0:
+            return 0.
+        t = self.max_term(x+s, t)
+        t_p_x = (self.omega_ - x - t) / (self.omega_ - x)
+        if moment == self.VARIANCE:  # Bernoulli shortcut for variance
+            return self.interest.v_t(t)**2 * t_p_x * (1 - t_p_x)
+        return (self.interest.v_t(t)**moment * (self.omega_ - x - t) 
+                / (self.omega_ - x))
+
+    def whole_life_insurance(self, x: int, s: int = 0, moment: int = 1, 
+                             b: int = 1, discrete: bool = True) -> float:
+        """Shortcut for whole life insurance
 
-            # indicate given T* time of death
-            ax.vlines(T, ymin, Y, colors='g', linestyles=':')
-            ax.text(T + xjig, ymin, f"{K}={T:.2f}", c='g')
+        Args:
+          x : age of selection
+          s : years after selection
+          b : amount of benefit
+          moment : compute first or second moment
+          discrete : benefit paid year-end (True) or moment of death (False)
+        """
+
+        if not discrete:
+            if moment == Beta.VARIANCE:
+                return (self.whole_life_insurance(x, s=s, b=b, moment=2, 
+                                                  discrete=False) -
+                        self.whole_life_insurance(x, s=s, b=b, moment=1, 
+                                                    discrete=False)**2) * b**2
+            return self.term_insurance(x, s=s, t=self.omega_-(x+s), b=b,
+                                       moment=moment, discrete=False)
+        return super().whole_life_insurance(x, s=s, moment=moment, b=b,
+                                            discrete=discrete)
+
+    def term_insurance(self, x: int, s: int = 0, t: int = 1, b: int = 1, 
+                       moment: int = 1, discrete: bool = False) -> float:
+        """Shortcut for term insurance
 
-            # indicate corresponding probability S(T*)
-            p = 1 - self.S(x, 0, T)     # note this is opposite of insurance
-            ax.hlines(Y, T, xmax, colors='g', linestyles=':')
-            ax.text(xmax, Y - yjig, f"Prob={p:.3f}", c='g', va='top', ha='right')
-        ax.set_title(f"PV annuity r.v. $Y({K}_{{{x if x else 'x'}}})$"
-                     if title is None else title)
-        ax.set_ylabel(f"$Y({K}_x)$", color=color)
-        ax.set_xlabel(f"${K}_x$")
-        plt.tight_layout()
-        return Y
+        Args:
+          x : age of selection
+          s : years after selection
+          t : term of insurance
+          b : amount of benefit
+          moment : compute first or second moment
+          discrete : benefit paid year-end (True) or moment of death (False)
+        """
+        if not discrete and moment in [1, Beta.VARIANCE]:
+            if moment == Beta.VARIANCE:
+                return (self.term_insurance(x, s=s, b=b, t=t, moment=2, 
+                                            discrete=False) -
+                        self.term_insurance(x, s=s, b=b, t=t, 
+                                            discrete=False)**2) * b**2
+            t = self.max_term(x+s, t)                                        
+            return (b * (1 - self.interest.v_t(t)) 
+                    / (self.interest.delta * (self.omega_ - (x+s))))
+        return super().term_insurance(x, s=s, moment=moment, b=b, 
+                                      discrete=discrete)
+
+class Makeham(MortalityLaws):
+    """Includes element in force of mortality that does not depend on age
+
+    Args:
+      A, B, c : parameters of Makeham distribution
+
+    Examples:
+      >>> print(Makeham(A=0.00022, B=2.7e-6, c=1.124).mu_x(60) * 0.9803)  # 0.00316
+    """
+    
+    def __init__(self, A: float, B: float, c: float, **kwargs):
+        assert c > 1, "Makeham requires c > 1"
+        assert B > 0, "Makeham requires B > 0"
+        assert A >= -B, "Makeham requires A >= -B"        
+        super().__init__(**kwargs)
+        self.A_ = A
+        self.B_ = B
+        self.c_ = c
+
+        def _mu(x, s): 
+            return A + B * c**(x+s)
+        
+        def _S(x, s, t):
+            return math.exp(-A*t - B*c**(x+s) * (c**t - 1)/math.log(c))
+
+        self.set_survival(mu=_mu, S=_S)
+
+class Gompertz(Makeham):
+    """Is Makeham's Law with A = 0
+
+    Args:
+      B, c : parameters of Gompertz distribution
+
+    Examples:
+      >>> print(Gompertz(B=0.00027, c=1.1).f_x(50, t=10)) # 0.04839
+    """
+
+    def __init__(self, B: float, c: float, **kwargs):
+        """Gompertz's Law is Makeham's Law with A = 0"""
+        super().__init__(A=0., B=B, c=c, **kwargs)
 
 if __name__ == "__main__":
-    from actuarialmath.policyvalues import Contract
-    from actuarialmath.sult import SULT
-    contract = Contract(premium=0, benefit=10000)  # premiums=0 after t=10
-    L = SULT().gross_policy_value(35, contract=contract)
-    V = SULT().set_interest(i=0).gross_policy_value(35, contract=contract) # 10000
+    print('Beta')
+    life = Beta(omega=100, alpha=0.5)
+    print(life.q_x(25, t=1, u=10))     # 0.0072
+    print(life.e_x(25))                # 50
+    print(Beta(omega=60, alpha=1/3).mu_x(35) * 1000)
+    print()
 
-if False:
-    
-    from actuarialmath.sult import SULT
-    life = SULT()
-    x = 20
-    life.Y_plot(x=x, T=life.Y_t(x=x, prob=0.5))
-
-    life = Annuity().set_interest(delta=0.06)\
-                    .set_survival(mu=lambda *x: 0.04)
-    prob = 0.5
-    x = 0
-    discrete = False
-    t = life.Y_t(0, prob, discrete=discrete)
-    life.Y_plot(x=20, T=t, discrete=discrete)
-    Y = life.Y_from_prob(x, prob=prob, discrete=discrete)
-    print(t, life.Y_to_t(Y))
-    print(Y, life.Y_from_t(t, discrete=discrete))
-    print(prob, life.Y_to_prob(x, Y=Y))
-    
-if False:
-    print("SOA Question 5.6:  (D) 1200")
-    life = Annuity().set_interest(i=0.05)
-    var = life.annuity_variance(A2=0.22, A1=0.45)
-    mean = life.annuity_twin(A=0.45)
-    print(life.portfolio_percentile(mean=mean, variance=var, prob=.95, N=100))
+    print('Uniform')
+    uniform = Uniform(80).set_interest(delta=0.04)
+    print(uniform.whole_life_annuity(20, discrete=False))        # 15.53
+    print(uniform.temporary_annuity(20, t=5, discrete=False))   # 4.35
+    print(Uniform(161).p_x(70, t=1)) # 0.98901
+    print(Uniform(95).e_x(30, t=40, curtate=False)) # 27.692
+    print()
+
+    uniform = Uniform(omega=80).set_interest(delta=0.04)
+    print(uniform.E_x(20, t=5))  # .7505
+    print(uniform.whole_life_insurance(20, discrete=False))  # .3789
+    print(uniform.term_insurance(20, t=5, discrete=False))  # .0755
+    print(uniform.endowment_insurance(20, t=5, discrete=False))  # .8260
+    print(uniform.deferred_insurance(20, u=5, discrete=False))  # .3033
     print()
+
+    print('Gompertz/Makeham')
+    life = Gompertz(B=0.000005, c=1.10)
+    p = life.p_x(80, t=10)  # 869.4
+    print(life.portfolio_percentile(N=1000, mean=p, variance=p*(1-p), prob=0.99)) 
+    print(Gompertz(B=0.00027, c=1.1).f_x(50, t=10)) # 0.04839
     
+    life = Makeham(A=0.00022, B=2.7e-6, c=1.124)
+    print(life.mu_x(60) * 0.9803)  # 0.00316
```

### Comparing `actuarialmath-0.0.9/src/actuarialmath/constantforce.py` & `actuarialmath-0.1.1/src/actuarialmath/constantforce.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,19 +7,22 @@
 from actuarialmath import MortalityLaws
 
 class ConstantForce(MortalityLaws):
     """Constant force of mortality - memoryless exponential distribution of lifetime
 
     Args:
       mu : constant value of force of mortality
-      udd : assume UDD (True) or CFM (False, default) between integer ages
+
+    Examples:
+      >>> life = ConstantForce(mu=0.01).set_interest(delta=0.05)
+      >>> life.term_insurance(35, t=35, discrete=False) + life.E_x(35, t=35)*0.51791
     """
 
-    def __init__(self, mu: float, udd: bool = False, **kwargs):
-        super().__init__(udd=udd, **kwargs)
+    def __init__(self, mu: float, **kwargs):
+        super().__init__(**kwargs)
 
         def _mu(x: int, s: float) -> float:
             """Constant force of mortality"""
             return mu
 
         def _S(x: int, s, t: float) -> float: 
             """Shortcut for survival function with constant force of mortality"""
@@ -156,27 +159,27 @@
         return super().term_insurance(x, s=s, t=t, b=b, moment=moment,
                discrete = discrete)
 
     def Z_t(self, x: int, prob: float, discrete: bool = True) -> float:
         """Shortcut for T_x (or K_x) given survival probability for insurance
 
         Args:
-          x : age selected
+          x : age (does not depend)
           prob : desired probability threshold
           discrete : benefit paid year-end (True) or moment of death (False)
         """
         t = -math.log(prob) / self.mu_
         return math.floor(t) if discrete else t    # opposite of annuity        
 
     def Y_t(self, x: int, prob: float, discrete: bool = True) -> float:
         """Shortcut for T_x (or K_x) given survival probability for annuity
 
         Args:
-          x : age selected
-          prob5~ : desired probability threshold
+          x : age (does not depend)
+          prob: desired probability threshold
           discrete : continuous (False) or annuity due (True)
         """
         t = -math.log(1 - prob) / self.mu_
         return math.ceil(t) if discrete else t    # opposite of insurance
 
 if __name__ == "__main__":
     print("SOA Question 6.36:  (B) 500")
@@ -191,15 +194,15 @@
     print(R)
     print()
 
     print("SOA Question 6.31:  (D) 1330")
     life = ConstantForce(mu=0.01).set_interest(delta=0.05)
     A = life.term_insurance(35, t=35) + life.E_x(35, t=35) * 0.51791 # A_35
     A = (life.term_insurance(35, t=35, discrete=False) 
-            + life.E_x(35, t=35) * 0.51791)    # A_35
+         + life.E_x(35, t=35) * 0.51791)    # A_35
     P = life.premium_equivalence(A=A, b=100000, discrete=False)
     print(P)
     print()
 
     print("SOA Question 6.27:  (D) 10310")
     life = ConstantForce(mu=0.03).set_interest(delta=0.06)
     x = 0
```

### Comparing `actuarialmath-0.0.9/src/actuarialmath/extrarisk.py` & `actuarialmath-0.1.1/src/actuarialmath/extrarisk.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,21 +7,23 @@
 from actuarialmath import Survival
 from actuarialmath import Actuarial
 
 class ExtraRisk(Actuarial):
     """Adjust mortality by extra risk
 
     Args:
-      life : original survival and mortality rates
+      life : contains original survival and mortality rates
       extra : amount of extra risk to adjust
-      risk : adjust by {"ADD_FORCE" "MULTIPLY_FORCE" "ADD_AGE" "MULTIPLY_RATE"}
+      risk : adjust by {"ADD_FORCE", "MULTIPLY_FORCE", "ADD_AGE", "MULTIPLY_RATE"}
     """
     risks = ["ADD_FORCE", "MULTIPLY_FORCE", "ADD_AGE", "MULTIPLY_RATE"]
 
-    def __init__(self, life: Survival, risk: str = "",
+    def __init__(self,
+                 life: Survival,
+                 risk: str = "",
                  extra: float = 0.) -> "ExtraRisk":
         """Specify type and amount of mortality adjustment to apply"""
         assert not risk or risk in self.risks, "risk must be one of " + str(risks)
         assert extra >= 0, "amount of extra risk must be non-negative"
         self.life = life
         self.extra_ = extra
         self.risk_ = risk
@@ -30,24 +32,35 @@
         """Returns survival function values adjusted by extra risk
 
         Args:
           col : {'p', 'q'} for one-year survival or mortality function values
 
         Returns:
           dict of age and survival function values adjusted by extract risk
+
+        Examples:
+          >>> life = SULT()
+          >>> extra = ExtraRisk(life=life, extra=0.05, risk="ADD_FORCE")
+          >>> select = SelectLife(periods=1).set_select(s=0, age_selected=True, 
+                                                        q=extra['q'])
         """
         f = {'q': self.q_x, 'p': self.p_x}[col[0]]
         return {x: f(x) for x in range(self.life._MINAGE, self.life._MAXAGE+1)}
 
     def p_x(self, x: int, s: int = 0) -> float:
         """Return p_[x]+s after adding or multiplying force of mortality
     
         Args:
           x : age of selection
           s : years after selection
+
+        Examples:
+          >>> life = SULT()
+          >>> extra = ExtraRisk(life=life, extra=2, risk="MULTIPLY_FORCE")
+          >>> print(life.p_x(45), extra.p_x(45))
         """
         if self.risk_ in ["MULTIPLY_RATE"]:
             return 1 - self.q_x(x, s=s)
         if self.risk_ in ["ADD_AGE"]:
             return self.life.p_x(x + self.extra_, s=s)    
         p = self.life.p_x(x, s=s)
         if self.risk_ in ["MULTIPLY_FORCE"]:
```

### Comparing `actuarialmath-0.0.9/src/actuarialmath/fractional.py` & `actuarialmath-0.1.1/src/actuarialmath/fractional.py`

 * *Files 12% similar despite different names*

```diff
@@ -29,17 +29,17 @@
           r : fractional year after selection
         """
         assert x >= 0, "x must be non-negative"
         assert s >= 0, "s must be non-negative"
         assert r >= 0, "r must be non-negative"
         s += math.floor(r)  # interpolate lives between consecutive integer ages
         r -= math.floor(r)
-        if r == 0:
+        if self.isclose(r):
             return self.l_x(x, s=s)
-        if r == 1.0:
+        if self.isclose(r, 1.0):
             return self.l_x(x, s=s+1)
         if self.udd_:
             return self.l_x(x, s=s)*(1-r) + self.l_x(x, s=s+1)*r
         else:
             return self.l_x(x, s=s)**(1-r) * self.l_x(x, s=s+1)**r
 
     def p_r(self, x: int, s: int = 0, r: float = 0., t: float = 1.) -> float:
@@ -48,26 +48,27 @@
         Args:
           x : age of selection
           s : years after selection
           r : fractional year after selection
           t : fractional number of years survived
 
         Examples:
+
         >>> life = Fractional(udd=False).set_survival(l=lambda x,t: 50-x-t)
         >>> print(life.p_r(47, r=0.), life.p_r(47, r=0.5), life.p_r(47, r=1.))
 
         """
         assert x >= 0, "x must be non-negative"
         assert s >= 0, "s must be non-negative"
         assert r >= 0, "r must be non-negative"
         assert t >= 0, "t must be non-negative"
         r_floor = math.floor(r)
         s += r_floor
         r -= r_floor
-        if 0. <= r + t <= 1.:
+        if 0. <= r + t <= 1.:            
             if self.udd_:
                 return 1 - self.q_r(x, s=s, r=r, t=t)
             else:          # Constant force shortcut within int age
                 return self.p_x(x, s=s)**t   # does not depend on r
         return self.l_r(x, s=s, r=r+t) / self.l_r(x, s=s, r=r)
 
     def q_r(self, x: int, s: int = 0, r: float = 0., t: float = 1., 
@@ -114,39 +115,43 @@
         """
         assert x >= 0, "x must be non-negative"
         assert s >= 0, "s must be non-negative"
         assert r >= 0, "r must be non-negative"
         r_floor = math.floor(r)
         s += r_floor
         r -= r_floor
+        if self.isclose(r):
+            return self.mu_x(x, s=s)
         if self.udd_:   # UDD shortcut
             return self.q_x(x, s=s) / (1. - r*self.q_x(x, s=s))
         else:          # Constant force shortcut
-            return -math.log(max(0.0001, self.p_x(x, s=s)))
+            return -math.log(max(0.000001, self.p_x(x, s=s)))
 
     def f_r(self, x: int, s: int = 0, r: float = 0., t: float = 0.0) -> float:
-        """mortality function at fractional age: f_[x]+s+r (t)
+        """Lifetime density function at fractional age: f_[x]+s+r (t)
 
         Args:
           x : age of selection
           s : years after selection
           r : fractional year after selection
           t : death at fractional year t
         """
         assert x >= 0, "x must be non-negative"
         assert s >= 0, "s must be non-negative"
         assert r >= 0, "r must be non-negative"
         assert t >= 0, "t must be non-negative"
         if 0. <= r + t <= 1.:   # shortcuts available within integer ages
-            if self.udd_:           # UDD constant q_x
-                return self.q_x(x, s=s)      # does not depent on fractional age
-            else:                  # Constant force shortcut
+            if self.udd_:       # UDD shortcut: constant q_x
+                return self.q_x(x, s=s)  # does not depend fractional age or duration
+            else:               # Constant force shortcut:
+                if self.isclose(t):
+                    return self.f_x(x=x, s=s)
                 mu = -math.log(max(0.00001, self.p_x(x, s=s)))
-                return math.exp(-mu*t) * mu  # does not depend on fractional age
-        else:      # survive to integer age then extend by fractional mortality
+                return math.exp(-mu*t) * mu    # does not depend on fractional age
+        else: # else survive to integer age, times density at fractional age
             r_floor = math.floor(r)
             r -= r_floor            # s.t. r < 1 
             s += r_floor            # while maintaining x+s+r unchanged
             t_floor = math.floor(r + t)
             u = t_floor - r         # s.t. u + r is integer
             t = t + r - t_floor     # s.t. t < 1
             return self.p_r(x, s=s, r=r, t=u) * self.f_r(x, s=s+u+r, t=t)
@@ -181,56 +186,65 @@
           s : years after selection
           t : fractional year limit of expected future lifetime
         """ 
         assert x >= 0, "x must be non-negative"
         assert s >= 0, "s must be non-negative"
         if t == 0:
             return 0
-        elif t < 0:   # shortcuts for complete expectation 
+
+        # shortcuts for complete expectation
+        elif t < 0:   
             if self.udd_:  # UDD case
-                return self.e_x(x, s=s, t=t, curtate=True) + 0.5
-            else:         # Constant Force Case: compute as maxage temporary
-                return self.e_r(x, s=s, t=self.max_term(x+s, t))
-        elif t <= 1:  # shortcuts within integer age
+                return self.e_x(x=x, s=s, t=t, curtate=True) + 0.5
+            else:         # Constant Force: compute as temporary through maxage
+                return self.e_r(x=x, s=s, t=self.max_term(x+s, t))
+
+        # shortcuts between integer ages
+        elif t <= 1:
             if self.udd_:  # UDD case
-                if t == 1:   # shortcut for UDD 1-year temporary expectation
-                    return 1. - self.q_x(x, s=s)*(1/2)
-                else:        # UDD formula for fractional temporary expectation
-                    return (self.q_r(x, s=s, t=t) * (t/2)
-                            + self.p_r(x, s=s, t=t) * t)
+                if t == 1:     # shortcut for UDD 1-year limited expectation
+                    return 1. - self.q_x(x=x, s=s)*(1/2)
+                else:          # shortcut for fractional limited expectation
+                    return self.q_r(x=x, s=s, t=t)*(t/2) + self.p_r(x, s=s, t=t)*t
             else:         # Constant Force case
-                mu = -math.log(max(0.00001, self.p_x(x, s=s)))  # constant mu
-                return (1. - math.exp(-mu*t)) / mu   # constant force formula
-        else:  # apply one-year recursion formula
-            return (self.e_x(x, s=s, t=1) +
-                    (self.p_x(x, s=s, t=1) * self.e_r(x, s=s+1, t=t-1)))
+                mu = -math.log(max(0.00001, self.p_x(x=x, s=s)))  # constant mu
+                return (1. - math.exp(-mu*t)) / mu                # shortcut
+
+        # t > 1: apply one-year recursion formula            
+        else:
+            return (self.e_r(x=x, s=s, t=1) +
+                    (self.p_x(x=x, s=s) * self.e_r(x=x, s=s+1, t=t-1)))
 
     #
     # Approximation of curtate and complete lifetimes
     #
     @staticmethod 
-    def e_approximate(e_complete: float = None, e_curtate: float = None) -> float:
+    def e_approximate(e_complete: float = None, e_curtate: float = None,
+                      variance: bool = False) -> float:
         """Convert between curtate and complete expectations assuming UDD shortcut
 
         Args:
           e_complete : complete expected lifetime
           e_curtate : or curtate expected lifetime
+          variance : to approximate mean (False) or variance (True)
 
         Returns:
           approximate complete or curtate expectation assuming UDD
         
         Examples:
-          >>> print(Fractional.e_curtate(e_complete=15))
-          >>> print(Fractional.e_curtate(e_curtate=15))
+          >>> print(Fractional.e_approximate(e_complete=15))
+          >>> print(Fractional.e_approximate(e_curtate=15))
         """
         if e_complete is not None:
             assert e_curtate is None, "one of e and e_curtate must be None"
-            return e_complete - 0.5
+            return e_complete - (1/12 if variance else 0.5)
+        elif e_curtate is not None:
+            return e_curtate + (1/12 if variance else 0.5)
         else:
-            return e_curtate + 0.5
+            raise Exception("Provide a value for either e_complete or e_curtate")
 
 if __name__ == "__main__":
     print(Fractional.e_approximate(e_complete=15))  # output e_curtate
     print(Fractional.e_approximate(e_curtate=15))   # output e_complete
 
     x = 45
     life = Fractional(udd=False).set_survival(l=lambda x,t: 50-x-t)
```

### Comparing `actuarialmath-0.0.9/src/actuarialmath/insurance.py` & `actuarialmath-0.1.1/src/actuarialmath/annuity.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,514 +1,494 @@
-"""Life insurance - Computes present values of insurance benefits
+"""Life annuities - Computes present values of annuity benefits
 
 MIT License. Copyright (c) 2022-2023 Terence Lim
 """
-from typing import Callable, Any, Tuple, List
+from typing import Callable, Any
 import math
 import matplotlib.pyplot as plt
 import numpy as np
-from actuarialmath import Fractional
+from actuarialmath import Insurance
 
-class Insurance(Fractional):
-    """Compute expected present values of life insurance"""
+class Annuity(Insurance):
+    """Compute present values and relationships of life annuities"""
 
-    def E_x(self, x: int, s: int = 0, t: int = 1, endowment: int = 1,
-            moment: int = 1) -> float:
-        """Pure endowment: t_E_x
+    def a_x(self, x: int, s: int = 0, t: int = Insurance.WHOLE, u: int = 0,
+            benefit: Callable = lambda x,t: 1, discrete: bool = True) -> float:
+        """Compute EPV of life annuity from survival function
 
         Args:
           x : age of selection
           s : years after selection
-          t : term of pure endowment
-          endowment : amount of pure endowment
-          moment : compute first or second moment
-        """
-        if t < 0:  # t infinite => EPV(t) = 0
-            return 0   
-        if t == 0:    # t = 0 => EPV(0) = 1
-            return 1
-        t = self.max_term(x+s, t)
-        t_p_x = self.p_x(x, s=s, t=t)
-        if moment == self.VARIANCE:  # Bernoulli shortcut for variance
-            return self.interest.v_t(t)**2 * t_p_x * (1 - t_p_x) * endowment**2
-        return (endowment * self.interest.v_t(t))**moment * t_p_x
+          u : year deferred
+          t : term of insurance
+          benefit : benefit as a function of age and year
+          discrete : annuity due (True) or continuous (False)
 
-    def A_x(self, x: int, s: int = 0, t: int = Fractional.WHOLE, u: int = 0,
-            benefit: Callable = lambda x,t: 1., endowment: float = 0.,
-            moment: int = 1, discrete: bool = True) -> float:
-        """Numerically compute EPV of insurance from basic survival functions
+        Examples:
+          >>> life.a_x(x=20)
+        """
+        t = self.max_term(x+s+u, t=t)
+        try:
+            if discrete:
+                a = sum([benefit(x+s, k) * self.interest.v_t(k) 
+                         * self.p_x(x, s=s, t=k) for k in range(int(u), int(t+u))])
+            else:   # use continuous first principles
+                Y = lambda t: (benefit(x+s, t+u) * self.interest.v_t(t+u) 
+                               * self.S(x, 0, t=t+u))
+                a = self.integral(Y, 0, t)
+        except:
+            raise Exception("Failed to numerically integrate EPV of annuity")
+        return a
+
+
+    def immediate_annuity(self, x: int, s: int = 0, t: int = Insurance.WHOLE, 
+                          b: int = 1, variance=False) -> float:
+        """Compute EPV of immediate life annuity
 
         Args:
           x : age of selection
           s : years after selection
-          u : year deferred
           t : term of insurance
-          benefit : benefit as a function of age and year
-          endowment : amount of endowment for endowment insurance
-          moment : compute first or second moment
-          discrete : benefit paid yearend (True) or moment of death (False)
-        """
-        assert moment >= 1
-        if t >=0 and endowment > 0:
-            E = self.E_x(x, s=s, t=t+u, moment=moment) * endowment
-        else:
-            E = 0
-        t = self.max_term(x+s+u, t=t)
-        if discrete:
-            A = sum([(benefit(x+s, k+1)*self.interest.v_t(k+1))**moment 
-                     * self.q_x(x, s=s, u=k) for k in range(u, t+u)])
-        else:   # use continous first principles
-            Z = lambda t: ((benefit(x+s, t+u) * self.interest.v_t(t+u))**moment 
-                           * self.f(x, s, t+u))
-            A = self.integral(Z, 0, t)
-        return A + E
-
-    @staticmethod
-    def insurance_variance(A2: float, A1: float, b: float = 1) -> float:
-        """Compute variance of insurance given moments and benefit
+          b : benefit amount
+          variance : return EPV (False) or variance (True)
+
+        Examples:
+          >>> life.immediate_annuity(x=20, t=30)
+        """
+        if variance:
+            return self.temporary_annuity(x, s=s, t=self.add_term(t, 1), b=b,
+                                          discrete=True, variance=True)
+        return (self.temporary_annuity(x, s=s, t=t, discrete=True) 
+                - 1 + self.E_x(x, s=s, t=t)) * b
+    
+    def annuity_twin(self, A: float, discrete: bool = True) -> float:
+        """Returns annuity from its WL or Endowment Insurance twin"
 
         Args:
-          A2 : second moment of insurance r.v.
-          A1 : first moment of insurance r.v.
-          b : benefit amount
+          A : cost of insurance
+          discrete : discrete/annuity due (True) or continuous (False)
+
+        Examples:
+          >>> life.annuity_twin(A=0.05879)
+        """
+        interest = (self.interest.d if discrete else self.interest.delta)
+        return ((1 - A) / interest) if interest else 1 - A
+
+    def insurance_twin(self, a: float, moment: int = 1, 
+                       discrete: bool = True) -> float:
+        """Returns WL or Endowment Insurance twin from annuity
+
+        Args:
+          a : cost of annuity
+          discrete : discrete/annuity due (True) or continuous (False)
+
+        Examples:
+          >>> life.insurance_twin(a=19.7655)
         """
-        return b**2 * max(0, A2 - A1**2)
+        assert moment in [1]
+        interest = (self.interest.d if discrete else self.interest.delta)
+        return 1 - a*interest
+  
+    def annuity_variance(self, A2: float, A1: float, b: float = 1.,
+                         discrete: bool = True) -> float:
+        """Compute variance from WL or endowment insurance twin
 
-    def whole_life_insurance(self, x: int, s: int = 0, moment: int = 1, 
-                             b: int = 1, discrete: bool = True) -> float:
-        """Whole life insurance: A_x
+        Args:
+          A2 : second moment of insurance factor
+          A1 : first moment of insurance factor
+          b : annuity benefit amount
+          discrete : discrete/annuity due (True) or continuous (False)
+
+        Examples:
+          >>> life.annuity_variance(A2=0.22, A1=0.45)
+        """
+        interest = (self.interest.d if discrete else self.interest.delta)
+        if interest == 0:
+            return b**2 * self.insurance_variance(A2=A2, A1=A1)
+        else:
+            return (b**2 * self.insurance_variance(A2=A2, A1=A1) / interest**2)
+
+    def whole_life_annuity(self, x: int, s: int = 0, b: int = 1, 
+                           variance: bool = False, 
+                           discrete: bool = True) -> float:
+        """Whole life annuity: a_x
 
         Args:
           x : age of selection
           s : years after selection
-          b : amount of benefit
-          moment : compute first or second moment
-          discrete : benefit paid year-end (True) or moment of death (False)
+          b : annuity benefit amount
+          variance : return EPV (True) or variance (False)
+          discrete : annuity due (True) or continuous (False)
+
+        Examples:
+          >>> life.whole_life_annuity(x=24, variance=True, due=False)
         """
-        if moment == self.VARIANCE:
+        interest = self.interest.d if discrete else self.interest.delta
+        if variance:  # short cut for variance of whole life
+            A1 = self.whole_life_insurance(x, s=s, moment=1, discrete=discrete)
             A2 = self.whole_life_insurance(x, s=s, moment=2, discrete=discrete)
-            A1 = self.whole_life_insurance(x, s=s, discrete=discrete)**2
-            return self.insurance_variance(A2=A2, A1=A1, b=b)
-        return self.A_x(x, s=s, t=self.WHOLE, benefit=lambda x,t: b, 
-                        moment=moment, discrete=discrete)
-
-    def term_insurance(self, x: int, s: int = 0, t: int = 1, b: int = 1, 
-                       moment: int = 1, discrete: bool = True) -> float:
-        """Term life insurance: A_x:t^1
+            return self.annuity_variance(A2=A2, A1=A1, discrete=discrete, b=b)
+        if interest > 0:
+            A = self.whole_life_insurance(x, s=s, discrete=discrete)
+            return b * (1 - A) / interest if interest > 0 else b * (1 - A)
+        else:  # when interest=1, annuity is expected life time (+1 if discrete)
+            return discrete + self.e_x(x=x, s=s, curtate=discrete)
+
+            
+    def temporary_annuity(self, x: int, s: int = 0, t: int = Insurance.WHOLE, 
+                          b: int = 1, variance: bool = False, 
+                          discrete: bool = True) -> float:
+        """Temporary life annuity: a_x:t
 
         Args:
           x : age of selection
           s : years after selection
-          t : term of insurance
-          b : amount of benefit
-          moment : compute first or second moment
-          discrete : benefit paid year-end (True) or moment of death (False)
-        """
-        if moment == self.VARIANCE:
-            A2 = self.term_insurance(x, s=s, t=t, moment=2, discrete=discrete)
-            A2 = self.term_insurance(x, s=s, t=t, discrete=discrete)**2
-            return self.insurance_variance(A2=A2, A1=A1, b=b)
-        A = self.whole_life_insurance(x, s=s, b=b, moment=moment, 
-                                      discrete=discrete)
-        if t < 0 or self.max_term(x+s, t=t) < t:
-            return A
-        E = self.E_x(x, s=s, t=t, moment=moment)
-        A -= E * self.whole_life_insurance(x, s=s+t, b=b, moment=moment,
-                                            discrete=discrete)
-        return A
-
-    def deferred_insurance(self, x: int, s: int = 0, u: int = 0, 
-                           t: int = Fractional.WHOLE, b: int = 1, 
-                           moment: int = 1, discrete: bool = True) -> float:
-        """Deferred insurance n|_A_x:t^1 = discounted term or whole life
+          t : term of annuity in years
+          b (int) : annuity benefit amount
+          variance : return EPV (True) or variance (False)
+          discrete : annuity due (True) or continuous (False)
+
+        Examples:
+          >>> life.temporary_annuity(x=24, t=10)
+        """
+        if variance:  # short cut for variance of temporary life annuity
+            A1 = self.endowment_insurance(x, s=s, t=t, discrete=discrete)
+            A2 = self.endowment_insurance(x, s=s, t=t, moment=2, 
+                                          discrete=discrete)
+            return self.annuity_variance(A2=A2, A1=A1, discrete=discrete, b=b)
+
+        # difference of whole life on (x) and deferred whole life on (x+t)
+        a = self.whole_life_annuity(x, s=s, b=b, discrete=discrete)
+        if t < 0 or self.max_term(x+s, t) < t:
+            return a
+        a_t = self.whole_life_annuity(x, s=s+t, b=b, discrete=discrete)
+        return a - (a_t * self.E_x(x, s=s, t=t))
+
+    def deferred_annuity(self, x: int, s: int = 0, u: int = 0, 
+                         t: int = Insurance.WHOLE, b: int = 1, 
+                         discrete: bool = True) -> float:
+        """Deferred life annuity n|t_a_x =  n+t_a_x - n_a_x
 
         Args:
           x : age of selection
           s : years after selection
-          u : year deferred
-          t : term of insurance
-          b : amount of benefit
-          moment : compute first or second moment
-          discrete : benefit paid year-end (True) or moment of death (False)
-        """
-        if self.max_term(x+s, u) < u:
-            return 0.        
-        if moment == self.VARIANCE:
-            A2 = self.deferred_insurance(x, s=s, t=t, u=u, moment=2, 
-                                         discrete=discrete)
-            A1 = self.deferred_insurance(x, s=s, t=t, u=u, discrete=discrete)
-            return self.insurance_variance(A2=A2, A1=A1, b=b)
-        E = self.E_x(x, s=s, t=u, moment=moment)
-        A = self.term_insurance(x, s=s+u, t=t, b=b, moment=moment, 
-                                discrete=discrete)
-        return E * A  # discount insurance by moment*force of interest
-
-    def endowment_insurance(self, x: int, s: int = 0, t: int = 1, b: int = 1, 
-                            endowment: int = -1, moment: int = 1, 
-                            discrete: bool = True) -> float:
-        """Endowment insurance: A_x^1:t = term insurance + pure endowment
+          u : years deferred
+          t : term of annuity in years
+          b : annuity benefit amount
+          discrete : annuity due (True) or continuous (False)
+
+        Examples:
+          >>> life.deferred_annuity(x=24, u=5, t=10, discrete=False)
+        """
+        a = self.temporary_annuity(x, s=s+u, t=t, b=b, discrete=discrete)
+        return self.E_x(x, s=s, t=u) * a
+
+    def certain_life_annuity(self, x: int, s: int = 0, u: int = 0, 
+                             t: int = Insurance.WHOLE, b: int = 1, 
+                             discrete: bool = True) -> float:
+        """Certain and life annuity = certain + deferred
 
         Args:
           x : age of selection
           s : years after selection
-          t : term of insurance
-          b : amount of benefit
-          endowment : amount of endowment paid at end of term if survive
-          moment : compute first or second moment
-          discrete : benefit paid year-end (True) or moment of death (False)
-        """
-        if moment == self.VARIANCE:
-            A2 = self.endowment_insurance(x, s=s, t=t, endowment=endowment, 
-                                          b=b, moment=2, discrete=discrete)
-            A1 = self.endowment_insurance(x, s=s, t=t, endowment=endowment,
-                                          b=b, discrete=discrete)
-            return self.insurance_variance(A2=A2, A1=A1, b=b)
-        E = self.E_x(x, s=s, t=t, moment=moment)
-        A = self.term_insurance(x, s=s, t=t, b=b, moment=moment,
-                                discrete=discrete)
-        return A + E * (b if endowment < 0 else endowment)**moment
-
-    def increasing_insurance(self, x: int, s: int = 0, t: int =
-                             Fractional.WHOLE, 
-                             b: int = 1, discrete: bool = True) -> float:
-        """Increasing life insurance: (IA)_x
+          u : years of certain annuity
+          t : term of life annuity in years
+          b : annuity benefit amount
+          discrete : annuity due (True) or continuous (False)
+
+        Examples:
+          >>> life.certain_life_annuity(x=24, u=5, t=10)
+        """
+        u = self.max_term(x+s, u)
+        if u < 0:
+            return 0.
+        a = self.deferred_annuity(x, s=s, u=u, t=t, b=b, discrete=discrete)
+        return self.interest.annuity(u, m=int(discrete)) + a
+
+    def increasing_annuity(self, x: int, s: int = 0, t: int = Insurance.WHOLE, 
+                           b: int = 1, discrete: bool = True) -> float:
+        """Increasing annuity
 
         Args:
           x : age of selection
           s : years after selection
-          t : term of insurance
-          b : amount of benefit in first year
-          discrete : benefit paid year-end (True) or moment of death (False)
+          t : term of life annuity in years
+          b : benefit amount at end of first year
+          discrete : annuity due (True) or continuous (False)
+
+        Examples:
+          >>> life.increasing_annuity(x=24, t=10)
         """
-        return self.A_x(x, s=s, t=t, benefit=lambda x,t: t * b, 
-                        discrete=discrete)
+        t = self.max_term(x+s, t=t)
+        benefit = lambda x, s: b * (s + 1) # increasing benefit
+        return self.a_x(x, s=s, benefit=benefit, t=t, discrete=discrete)
 
-    def decreasing_insurance(self, x, s: int = 0, t: int = 1, b: int = 1,
-                             discrete: bool = True) -> float:
-        """Decreasing life insurance: (DA)_x
+    def decreasing_annuity(self, x: int, s: int = 0, t: int = 0, 
+                           b: int = 1, discrete: bool = True) -> float:
+        """Identity (Da)_x:n + (Ia)_x:n = (n+1) a_x:n temporary annuity
 
         Args:
           x : age of selection
           s : years after selection
-          t : term of insurance
-          b : amount of benefit in first year
-          discrete : benefit paid year-end (True) or moment of death (False)
+          t : term of life annuity in years
+          b : benefit amount at end of first year
+          discrete : annuity due (True) or continuous (False)
+
+        Examples:
+          >>> life.decreasing_annuity(x=24, t=10)
         """
-        assert t > 0  # decreasing must be term insurance
-        A = self.term_insurance(x, t=t, b=b, discrete=discrete)
-        n = t + int(discrete)   #  (DA)_x:n + (IA)_x:n = (n+1) A^1_x:n
-        return A*n - self.increasing_insurance(x, s=s, t=t, b=b, 
-                                               discrete=discrete)
+        assert t >= 0   # decreasing must be till term
+        t = self.max_term(x+s, t=t)
+        a = self.temporary_annuity(x, s=s, t=t, discrete=discrete)
+        n = t + int(discrete)
+        return b * (a*n - self.increasing_annuity(x, s=s, t=t, discrete=discrete))
 
     #
-    # Insurance random variable: Z(t)
+    # Annuity random variable: Y(t)
     #
-    def Z_t(self, x: int, prob: float, discrete: bool = True) -> float:
-        """T_x given percentile of the PV of WL or Term insurance, i.e. r.v. Z(t)
+    def Y_t(self, x: int, prob: float, discrete: bool = True) -> float:
+        """T_x given percentile of the r.v. Y = PV of WL or Temporary Annuity
 
         Args:
-          x : age initially insured
+          x : age of selection
           prob : desired probability threshold
-          discrete : benefit paid year-end (True) or moment of death (False)
+          discrete : annuity due (True) or continuous (False)
+
+        Returns:
+          T s.t. S(T) == 1-prob; if discrete, return K=ceil(T) s.t. S(K) <= 1-prob
+
         """
         assert prob < 1.0
-        t = self.solve(lambda t: self.S(x, 0, t), target=prob, grid=50)
-        return math.floor(t) if discrete else t    # opposite of annuity
+        t = self.solve(lambda t: self.S(x, 0, t), target=1. - prob,
+                       grid=[self._MINAGE, self._MAXAGE])
+        return math.ceil(t) if discrete else t   # should be opposite of insurance?
 
-    def Z_from_t(self, t: float, discrete: bool = True) -> float:
-        """PV of insurance payment Z(t), given T_x (or K_x if discrete)
+    def Y_x(self, x, s: int = 0, t: float = 1., discrete: bool = True) -> float:
+        """EPV of year t annuity benefit for life aged [x]+s: b_x[s]+s(t)
 
         Args:
-          t : year of death
-          discrete : benefit paid year-end (True) or moment of death (False)
+          x : age initially insured
+          s : years after selection
+          t : year of benefit
+          discrete : annuity due (True) or continuous (False)
         """
-        return self.interest.v_t((math.floor(t) + 1) if discrete else t)
+        assert t >= 0
+        if discrete:
+            u = math.floor(t)
+            return self.interest.v_t(u) * self.p_x(x, s=s, t=u)
+        else:
+            return self.interest.v_t(t) * self.p_r(x, s=s, t=t)
 
-    def Z_to_t(self, Z: float) -> float:
-        """T_x s.t. PV of insurance payment is Z
+    def Y_from_t(self, t: float, discrete: bool = True) -> float:
+        """PV of insurance payment Y(t), given T_x
 
         Args:
-          Z : Present value of benefit paid
+          t : year of death
+          discrete : annuity due (True) or continuous (False)
         """
-        #t = Insurance.solve(lambda t: self.Z_from_t(t), Z, self._MAXAGE/2)
-        t = math.log(Z) / math.log(self.interest.v)
-        return t
+        if self.isclose(self.interest.delta):            # if interest=0:
+            return math.floor(t) + 1 if discrete else t  #   return number of payments
+        if discrete:
+            return (1 - self.interest.v_t(math.floor(t) + 1)) / self.interest.d
+        else:
+            return (1 - self.interest.v_t(t)) / self.interest.delta
 
-    def Z_from_prob(self, x: int, prob: float, discrete: bool = True) -> float:
-        """Percentile of insurance PV r.v. Z, given probability
+    def Y_from_prob(self, x: int, prob: float, discrete: bool = True) -> float:
+        """Percentile of annual or continuous WL annuity PV r.v. Y, given probability
 
         Args:
           x : age initially insured
-          prob : threshold for probability of survival
-          discrete : benefit paid year-end (True) or moment of death (False)
+          prob : desired probability threshold
+          discrete : annuity due (True) or continuous (False)
         """
-        t = self.Z_t(45, prob, discrete=discrete)   # opposite of annuity!
-        return self.Z_from_t(t, discrete=discrete)  # z is WL or Term Insurance
+        t = self.Y_t(x, prob, discrete=discrete)
+        return self.Y_from_t(t=t, discrete=discrete)
 
-    def Z_to_prob(self, x: int, Z: float) -> float:
-        """Cumulative density of insurance PV r.v. Z, given percentile value
+    def Y_to_t(self, Y: float) -> float:
+        """T_x s.t. PV of continuous WL annuity payments is Y
 
         Args:
-          x : age initially insured
-          Z : present value of benefit paid
+          Y : Present value of benefits paid
         """
-        t = self.Z_to_t(Z) 
-        return self.S(x, 0, t)      # z is WL or Term Insurance
+        if self.interest.v == 0.:
+            return Y
+        else:
+            return math.log(1 - self.interest.delta*Y) / math.log(self.interest.v)
 
-    def Z_x(self, x, s: int = 0, t: int = 1, discrete: bool = True):
-        """EPV of year t insurance death benefit for life aged [x]+s: b_x[s]+s(t)
+
+    def Y_to_prob(self, x: int, Y: float) -> float:
+        """Probability that continuous WL annuity PV r.v. is no more than Y
 
         Args:
-          x : age of selection
-          s : years after selection
-          t : year of benefit
-          discrete : benefit paid year-end (True) or moment of death (False)
+          x : age initially insured
+          Y : present value of benefits paid
         """
-        assert t > 0
-        if discrete:
-            u = math.ceil(t) - 1
-            return self.q_x(x, s=s, u=u) * self.interest.v_t(u+1)
-        else:
-            return self.f_r(x, s=s, t=t) * self.interest.v_t(t)
+        t = self.Y_to_t(Y)
+        return 1 - self.S(x, 0, t)   # opposite of Insurance
 
-    def Z_plot(self, x: int, s: int = 0, stop : int = 0,
+    def Y_plot(self,
+               x: int,
+               s: int = 0,
+               stop : int = 0,
                benefit: Callable = lambda x,k: 1,
                T: float | None = None,
                discrete: bool = True,
                ax: Any = None,
-               title: str | None = None,
-               color: str ='r')-> float | None:
-        """Plot of PV of insurance r.v. Z vs t
+               dual: bool = False,
+               title: str | None = None,               
+               color: str ='r',
+               alpha: float = 0.3)-> float | None:
+        """Plot PV of annuity r.v. Y vs T
 
         Args:
           x : age of selection
           s : years after selection
           stop : time to end plot
           benefit : benefit as a function of selection age and time
-          discrete  discrete or continuous insurance
+          discrete : discrete or continuous insurance
           ax : figure object to plot in
-          color : color to plot
+          dual: whether to plot survival function on secondary axis
+          color : color of primary plot 
+          alpha : transparency of plot area
           title : title of plot 
         """
         if ax is None:
             fig, ax = plt.subplots(1, 1)
         K = 'K' if discrete else 'T'
         stop = stop or self._MAXAGE - (x + s)
         step = 1 if discrete else stop / 1000.
         steps = np.arange(0, stop + step, step)
-        
-        # plot PV benefit values
-        z = [benefit(x, s+t) * self.Z_from_t(t, discrete=discrete) for t in steps]
-        if T is None:
-            ax.bar(steps, z, width=step, alpha=0.5, color=color)
-            Z = None
-        else:
-            # plot Z(t)
-            ax.step(steps, z, ':', c=color, where='pre' if discrete else 'post')
-            xmin, xmax = ax.get_xlim()
-            ymin, ymax = ax.get_ylim()
-            yjig = (ymax - ymin) / 50
-            xjig = (xmax - xmin) / 50
+
+        # plot benefit values
+        y = [benefit(x, s+t) * self.Y_from_t(t, discrete=discrete) for t in steps]
+        ax.bar(steps, y, width=step, alpha=alpha, color=color)
+        ax.tick_params(axis='y', colors=color)
+        #ax.step(steps, y, ':', c=color, where='pre' if discrete else 'post')
+        xmin, xmax = ax.get_xlim()
+        xjig = (xmax - xmin) / 50
+        ymin, ymax = ax.get_ylim()
+        yjig = (ymax - ymin) / 50
+
+        # plot survival probabilities in secondary axis
+        if dual:
+            p = [self.p_x(x=x, s=s, t=t) for t in steps]
+            bx = ax.twinx()
+            bx.step(steps, p, '-', c='g', alpha=alpha,
+                    where='pre' if discrete else 'post')
+            #bx.bar(steps, p, color='g', alpha=.2, width=step, align='edge')
+            bx.set_ylabel(f"$S({K})$", color='g')
+            bx.tick_params(axis='y', colors='g')
+    
+        if T is not None:
+            # indicate PV benefit Y(T*)
+            Y = self.Y_from_t(T, discrete=discrete) * benefit(self._MINAGE, T)
             
-            # indicate PV of benefit Z(T*)
-            Z = self.Z_from_t(T, discrete=discrete) * benefit(self._MINAGE, T)
-            ax.plot(T, Z, c=color, marker='o')
-            ax.text(T, Z + yjig, f"Z*={Z:.2f}", c=color)
-
-            # indicate given time of death T*
-            ax.vlines(T, ymin, Z, colors='g', linestyles=':')
-            ax.text(T + xjig, ymin, f"${K}_x$={T:.2f}", c='g')
-
-            # indicate corresponding S(T*)
-            p = self.S(x, 0, T)     # S(t): note that is opposite of annuity
-            ax.hlines(Z, T, xmax, colors='g', linestyles=':')
-            ax.text(xmax, Z - yjig, f"Prob={p:.3f}", c='g', va='top', ha='right')
-        ax.set_title(f"PV insurance r.v. $Z({K}_{{{x if x else 'x'}}})$"
+            label1, = ax.plot(T, Y, c=color, marker='o',
+                              label=f"Y({T:.2f})={Y:.4f}")            
+            #ax.text(T + xjig, Y + 1*yjig, f"Y*={Y:.2f}", c=color)
+            ax.legend(handles=[label1], loc='upper left')
+
+            if dual:
+                prob = self.S(x, 0, T)
+                label2, = bx.plot(T, prob, c='g', marker='o',
+                                  label=f"Pr[{K}>{T:.2f}]={prob:.4f}")
+                bx.legend(handles=[label2], loc='upper right')
+        ax.set_title(f"PV annuity r.v. $Y({K}_{{{x if x else 'x'}}})$"
                      if title is None else title)
-        ax.set_ylabel(f"$Z({K}_x)$", color=color)
+        ax.set_ylabel(f"$Y({K}_x)$", color=color)
         ax.set_xlabel(f"${K}_x$")
-        plt.tight_layout()
-        return Z
+        #plt.tight_layout()
+        return Y if T else None
 
-    def Z_curve(self, x: int, s: int = 0, stop: int = 0,
-                benefit: Callable = lambda x, k: 1,
+    def _Y_plot(self, x: int, s: int = 0, stop : int = 0,
+                benefit: Callable = lambda x,k: 1,
                 T: float | None = None,
                 discrete: bool = True,
-                title: str | None = None,
-                ax: Any = None):
-        """Plot PV of insurance r.v. Z(t) and survival probability vs time t
+                ax: Any = None,
+                title: str | None = None,               
+                color='r') -> float:
+        """Plot PV of annuity r.v. Y vs T
 
         Args:
           x : age of selection
           s : years after selection
-          stop : end at time t, inclusive
+          stop : time to end plot
           benefit : benefit as a function of selection age and time
           discrete : discrete or continuous insurance
-          T : point in time to indicate benefit and survival probability
           ax : figure object to plot in
+          color : color to plot
+          title : title of plot
         """
         if ax is None:
-            fig, ax = plt.subplots(1, 1)        
+            fig, ax = plt.subplots(1, 1)
         K = 'K' if discrete else 'T'
         stop = stop or self._MAXAGE - (x + s)
-        step = 1 # if discrete else stop/1000.
-        steps = range(stop + step)
-        p = [self.p_x(x=x, s=s, t=t) for t in steps]
+        step = 1 if discrete else stop / 1000.
+        steps = np.arange(0, stop + step, step)
 
-        # plot survival probabilities in secondary axis
-        bx = ax.twinx()
-        bx.bar(steps, p, color='g', alpha=.2, width=step, align='edge')
-        bx.set_ylabel(f"$S({K})$", color='g')
-        bx.tick_params(axis='y', colors='g')
-
-        # plot benefit values in primary axis
-        z = [benefit(x, s+t) * self.Z_from_t(t, discrete=discrete) for t in steps]
-        ax.step(steps, z, ':', c='r', where='pre' if discrete else 'post')
-        ax.set_ylabel(f"Z({K})", color='r')
-        ax.tick_params(axis='y', colors='r')
-
-        if T is not None:   # plot PV benefit value and survival prob at given T
-            Z = self.Z_from_t(T, discrete=discrete) * benefit(self._MINAGE, T)
-            label1, = ax.plot(T, Z, c='r', marker='o',
-                              label=f"Z({K}*={T:.2f}): {Z:.2f}")
-            ax.legend(handles=[label1], loc='center left')
+        # plot benefit values
+        y = [benefit(x, s+t) * self.Y_from_t(t, discrete=discrete) for t in steps]
+        if T is None:
+            ax.bar(steps, y, width=stepsize, alpha=0.5, color=color)
+            Y = None
+        else:
+            ax.step(steps, y, ':', c=color, where='pre' if discrete else 'post')
+
+            xmin, xmax = ax.get_xlim()
+            ymin, ymax = ax.get_ylim()
+            yjig = (ymax - ymin) / 50
+            xjig = (xmax - xmin) / 50
             
-            prob = self.S(x, 0, T)      # note: is opposite of annuity
-            label2, = bx.plot(T, prob, c='g', marker='o',
-                               label=f"Pr[{K}>{K}*]<={prob:.3f}")
-            bx.legend(handles=[label2], loc='center right')
-        ax.set_title(title if title is not None else
-                     f"PV benefit $Z({K})$ and survival probability $S({K})$")
-        ax.set_xlabel(f"${K}$")
+            # indicate PV benefit Y(T*)
+            Y = self.Y_from_t(T, discrete=discrete) * benefit(self._MINAGE, T)
+            ax.plot(T, Y, c=color, marker='o')
+            ax.text(T + xjig, Y + 1*yjig, f"Y*={Y:.2f}", c=color)
+
+            # indicate given T* time of death
+            ax.vlines(T, ymin, Y, colors='g', linestyles=':')
+            ax.text(T + xjig, ymin, f"{K}={T:.2f}", c='g')
+
+            # indicate corresponding probability S(T*)
+            p = 1 - self.S(x, 0, T)     # note this is opposite of insurance
+            ax.hlines(Y, T, xmax, colors='g', linestyles=':')
+            ax.text(xmax, Y - yjig, f"Prob={p:.3f}", c='g', va='top', ha='right')
+        ax.set_title(f"PV annuity r.v. $Y({K}_{{{x if x else 'x'}}})$"
+                     if title is None else title)
+        ax.set_ylabel(f"$Y({K}_x)$", color=color)
+        ax.set_xlabel(f"${K}_x$")
         plt.tight_layout()
-
+        return Y
     
 if __name__ == "__main__":
+    from actuarialmath.policyvalues import Contract
+    from actuarialmath.sult import SULT
+    contract = Contract(premium=0, benefit=10000)  # premiums=0 after t=10
+    L = SULT().gross_policy_value(35, contract=contract)
+    V = SULT().set_interest(i=0).gross_policy_value(35, contract=contract) # 10000
 
+if False:
+    
     from actuarialmath.sult import SULT
     life = SULT()
-    life.Z_curve(x=20, stop=80, T=life.Z_t(x=20, prob=0.5),
-                 title="PV insurance benefit if (x) survives median lifetime")
-    
-    print("SOA Question 4.18  (A) 81873 ")
-    def f(x,s,t): return 0.1 if t < 2 else 0.4*t**(-2)
-    life = Insurance().set_interest(delta=0.05)\
-                      .set_survival(f=f, maxage=10)
-    def benefit(x,t): return 0 if t < 2 else 100000
-    prob = 0.9 - life.q_x(x=0, t=2)
-    T = life.Z_t(x=0, prob=prob)
-    life.Z_curve(x=0, T=T, benefit=benefit, discrete=False)
-    Z = life.Z_from_t(T) * benefit(0, T)
-    print(Z)
-    
-    # Example: plot Z vs T
-    life = Insurance().set_interest(delta=0.06)\
-                      .set_survival(mu=lambda *x: 0.04)
-    prob = 0.8
     x = 20
-    discrete = True
-    t = life.Z_t(x, prob, discrete=discrete)
-    Z = life.Z_from_prob(x, prob=prob, discrete=discrete)
-    print(t, life.Z_to_t(Z))
-    print(Z, life.Z_from_t(t, discrete=discrete))
-    print(prob, life.Z_to_prob(x, Z=Z))
-    life.Z_plot(x, T=t, discrete=discrete)
-    plt.show()
-    
+    life.Y_plot(x=x, T=life.Y_t(x=x, prob=0.5))
 
-    print("SOA Question 4.10:  (D)")
+    life = Annuity().set_interest(delta=0.06)\
+                    .set_survival(mu=lambda *x: 0.04)
+    prob = 0.5
     x = 0
-    life = Insurance().set_interest(i=0.0)\
-                      .set_survival(S=lambda x,s,t: 1, maxage=x+40)
-    def expected(x, t):  # true E[Z]
-        if 10 <= t <= 20: return life.interest.v_t(t)
-        elif 20 < t <= 30: return 2 * life.interest.v_t(t)
-        else: return 0
-        
-    def A(x, t):  # Z_x+k (t-k)
-        return life.interest.v_t(t - x) * (t > x)
+    discrete = False
+    t = life.Y_t(0, prob, discrete=discrete)
+    life.Y_plot(x=20, T=t, discrete=discrete)
+    Y = life.Y_from_prob(x, prob=prob, discrete=discrete)
+    print(t, life.Y_to_t(Y))
+    print(Y, life.Y_from_t(t, discrete=discrete))
+    print(prob, life.Y_to_prob(x, Y=Y))
     
-    benefits=[lambda x,t: (life.E_x(x, t=10) * A(x+10, t)
-                             + life.E_x(x, t=20)* A(x+20, t)
-                             - life.E_x(x, t=30) * A(x+30, t)),
-              lambda x,t: (A(x, t)
-                             + life.E_x(x, t=20) * A(x+20, t)
-                             - 2 * life.E_x(x, t=30) * A(x+30, t)),
-              lambda x,t: (life.E_x(x, t=10) * A(x, t)
-                             + life.E_x(x, t=20) * A(x+20, t)
-                             - 2 * life.E_x(x, t=30) * A(x+30, t)),
-              lambda x,t: (life.E_x(x, t=10) * A(x+10, t)
-                             + life.E_x(x, t=20) * A(x+20, t)
-                             - 2 * life.E_x(x, t=30) * A(x+30, t)),
-              lambda x,t: (life.E_x(x, t=10)
-                             * (A(x+10, t)
-                                + life.E_x(x+10, t=10) * A(x+20, t)
-                                - life.E_x(x+20, t=10) * A(x+30, t)))]
-    z = [sum(abs(b(x, t) - expected(x, t)) for t in range(40)) for b in benefits]
-    print("ABCDE"[np.argmin(z)])
+if False:
+    print("SOA Question 5.6:  (D) 1200")
+    life = Annuity().set_interest(i=0.05)
+    var = life.annuity_variance(A2=0.22, A1=0.45)
+    mean = life.annuity_twin(A=0.45)
+    print(life.portfolio_percentile(mean=mean, variance=var, prob=.95, N=100))
+    print()
     
-    fig, ax = plt.subplots(3, 2)
-    ax = ax.ravel()
-    for i, b in enumerate([expected] + benefits):
-        life.Z_plot(x, benefit=b, ax=ax[i], color=f"C{i+1}", title=' ')
-        ax[i].legend(["(" + "abcde"[i-1] + ")" if i else "Z"])        
-
-    print("SOA Question 6.33:  (B) 0.13")
-    life = Insurance().set_survival(mu=lambda x,t: 0.02*t).set_interest(i=0.03)
-    x = 0
-    var = life.E_x(x, t=15, moment=life.VARIANCE, endowment=10000)
-    p = 1- life.portfolio_cdf(mean=0, variance=var, value=50000, N=500)
-    print(p)
-
-
-    print("SOA Question 4.12:  (C) 167")
-    cov = Insurance.covariance(a=1.65, b=10.75, ab=0) # Z1 and Z2 nonoverlapping
-    var = Insurance.variance(a=2, b=1, var_a=46.75, var_b=50.78, cov_ab=cov)
-    print(var)
-
-    print("SOA Question 4.11:  (A) 143385")
-    A1 = 528/1000   # E[Z1]  term insurance
-    C1 = 0.209      # E[pure_endowment]
-    C2 = 0.136      # E[pure_endowment^2]
-    def fun(A2):
-        B1 = A1 + C1   # endowment = term + pure_endowment
-        B2 = A2 + C2   # double force of interest
-        return Insurance.insurance_variance(A2=B2, A1=B1)
-    A2 = Insurance.solve(fun, target=15000/(1000*1000), grid=[143400, 279300])
-    var = Insurance.insurance_variance(A2=A2, A1=A1, b=1000)
-    print(var)
-
-    print("SOA Question 4.15  (E) 0.0833 ")
-    life = Insurance().set_survival(mu=lambda *x: 0.04)\
-                      .set_interest(delta=0.06)
-    benefit = lambda x,t: math.exp(0.02*t)
-    A1 = life.A_x(0, benefit=benefit, discrete=False)
-    A2 = life.A_x(0, moment=2, benefit=benefit, discrete=False)
-    var = A2 - A1**2
-    print(var)
-
-    print("SOA Question 4.4  (A) 0.036")
-    x = 40
-    life = Insurance().set_survival(f=lambda *x: 0.025, maxage=x+40)\
-                      .set_interest(v_t=lambda t: (1 + .2*t)**(-2))
-    benefit = lambda x,t: 1 + .2 * t
-    A1 = life.A_x(x, benefit=benefit, discrete=False)
-    A2 = life.A_x(x, moment=2, benefit=benefit, discrete=False)
-    var = A2 - A1**2
-    print(var)
-
-    print("Other examples of usage")
-    life = Insurance().set_interest(delta=0.06)\
-                      .set_survival(mu=lambda *x: 0.04)
-    benefit = lambda x,t: math.exp(0.02 * t)
-    A1 = life.A_x(0, benefit=benefit)
-    A2 = life.A_x(0, moment=2, benefit=benefit)
-    var = A2 - A1**2 
-    print(var)  # 0.0833
-
-    life = Insurance().set_interest(delta=0.05)\
-                      .set_survival(mu=lambda x,s: 0.03)
-    benefit = lambda x,t: math.exp(0.04 * t)
-    A = life.A_x(0, benefit=benefit)
-    print(A)   # 0.75
-    A2 = life.A_x(0, moment=2, benefit=benefit)
-    print(A2)  #0.60
```

### Comparing `actuarialmath-0.0.9/src/actuarialmath/interest.py` & `actuarialmath-0.1.1/src/actuarialmath/interest.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,83 +5,105 @@
 import math
 import numpy as np
 import pandas as pd
 from typing import Callable
 from actuarialmath import Actuarial
 
 class Interest(Actuarial):
-    """Converts interest rates, and computes value of annuity certain
+    """Store an assumed interest rate, and compute interest rate functions
     
     Args:
       i : assumed annual interest rate
-      d : or assumed discount rate
-      v : or assumed discount factor
-      delta : or assumed continuously compounded interest rate
-      v_t : or assumed discount rate as a function of time
-      i_m : or assumed monthly interest rate
-      d_m : or assumed monthly discount rate
-      m : m'thly frequency, if i_m or d_m are given
-
-    Attributes:
-      i (float) : interest rate
-      d (float) : discount rate
-      delta (float) :  continuously compounded interest rate
-      v (float) : discount factor
-      v_t (Callable) : discount factor as a function of time
+      d : or annual discount rate
+      v : or annual discount factor
+      delta : or continuously compounded interest rate
+      v_t : or discount rate as a function of time
+      i_m : or m-thly interest rate
+      d_m : or m-thly discount rate
+      m : m'thly frequency, if i_m or d_m are specified
     """
 
     def __init__(self, i: float = -1., delta: float = -1., d: float = -1., 
                  v: float = -1., i_m: float = -1., d_m: float = -1., m: int = 0,
                  v_t: Callable[[float], float] | None = None):
         if i_m >= 0:  # given interest rate mthly compounded
             i = self.mthly(m=m, i_m=i_m)
         if d_m >= 0:  # given discount rate mthly compounded
             d = self.mthly(m=m, d_m=d_m)
         if v_t is None:
             if delta >= 0:     # given continously-compounded rate
-                self.i = math.exp(delta) - 1
+                self._i = math.exp(delta) - 1
             elif d >= 0:       # given annual discount rate
-                self.i = d / (1 - d)
+                self._i = d / (1 - d)
             elif v >= 0 :      # given annual discount factor
-                self.i = (1 / v) - 1
+                self._i = (1 / v) - 1
             elif i >= 0:
-                self.i = i
+                self._i = i
             else:              # given annual interest rate
                 raise Exception("non-negative interest rate not given")
-            self.v_t = lambda t: self.v**t 
-            self.v = 1 / (1 + self.i)         # store discount factor
-            self.d = self.i / (1 + self.i)    # store discount rate
-            self.delta = math.log(1 + self.i) # store continuous rate
+            self._v_t = lambda t: self._v**t 
+            self._v = 1 / (1 + self._i)         # store discount factor
+            self._d = self._i / (1 + self._i)    # store discount rate
+            self._delta = math.log(1 + self._i) # store continuous rate
         else:   # given discount function
             assert callable(v_t), "v_t must be a callable discount function"
             assert v_t(0) == 1, "v_t(t=0) must equal 1"
-            self.v_t = v_t
-            #self.i = (1 / v_t(1)) - 1
-            self.v = self.d = self.i = self.delta = None
+            self._v_t = v_t
+            #self._i = (1 / v_t(1)) - 1
+            self._v = self._d = self._i = self._delta = None
+
+    @property
+    def i(self) -> float:
+       """effective annual interest rate"""
+       return self._i
+   
+    @property
+    def d(self) -> float:
+       """annual discount rate of interest"""
+       return self._d
+   
+    @property
+    def delta(self) -> float:
+       """continuously compounded interest rate, or force of interest, per year"""
+       return self._delta
+   
+    @property
+    def v(self) -> float:
+       """annual discount factor"""
+       return self._v
+   
+    @property
+    def v_t(self) -> Callable:
+       """discount factor as a function of time"""
+       return self._v_t
+    
 
     def annuity(self, t: int = -1, m: int = 1, due: bool = True) -> float:
         """Compute value of the annuity certain factor
 
         Args:
           t : number of years of payments
           m : m'thly frequency of payments (0 for continuous payments)
           due : whether annuity due (True) or immediate (False)
+
+        Examples:
+          >>> print(interest.annuity(t=10, due=False), 2.831059)
         """
         v_t = 0 if t < 0 else self.v**t   # is t finite
         assert m >= 0, "mthly frequency must be non-negative"
         if m == 0:  # if continuous
             return (1 - v_t) / self.delta
         elif due:   # if annuity due
             return (1 - v_t) / self.mthly(m=m, d=self.d)
         else:       # if annuity immediate
             return (1 - v_t) / self.mthly(m=m, i=self.i)
 
     @staticmethod
     def mthly(m: int = 0, i: float = -1, d: float = -1,
-            i_m: float = -1, d_m: float = -1) -> float:
+              i_m: float = -1, d_m: float = -1) -> float:
         """Convert to or from m'thly interest rates
 
         Args:
           m : m'thly frequency
           i : an annual-pay interest rate, to convert to m'thly
           d : or annual-pay discount rate, to convert to m'thly
           i_m : or m'thly interest rate, to convert to annual pay
```

### Comparing `actuarialmath-0.0.9/src/actuarialmath/life.py` & `actuarialmath-0.1.1/src/actuarialmath/life.py`

 * *Files 12% similar despite different names*

```diff
@@ -92,35 +92,45 @@
 
         Args:
           p : probability of selecting first r.v.
           p1 : probability of occurrence if first r.v.
           p2 : probability of occurrence if other r.v.
           N : number of trials
           variance : whether to return variance (True) or mean (False)
+
+        Examples:
+          >>> p1 = (1. - 0.02) * (1. - 0.01)  # 2_p_x if vaccine given
+          >>> p2 = (1. - 0.02) * (1. - 0.02)  # 2_p_x if vaccine not given
+          >>> math.sqrt(Life.mixture(p=.2, p1=p1, p2=p2, N=100000, variance=True))
         """
         assert 0 <= p <= 1 and 0 <= p1 <= 1 and 0 <= p2 <= 1 and N >= 1
         mean1 = Life.binomial(p1, N)
         mean2 = Life.binomial(p2, N)
         if variance:
             var1 = Life.binomial(p1, N, variance=True)
             var2 = Life.binomial(p2, N, variance=True)
             return (Life.bernoulli(p, mean1**2 + var1, mean2**2 + var2) -
                     Life.bernoulli(p, mean1, mean2)**2)
         else:
             return Life.bernoulli(p, mean1, mean2)
         
     @staticmethod
     def conditional_variance(p, p1, p2: float, N: int = 1) -> float:
-        """Conditional variance formula
+        """Conditional variance formula for mixture of binomials
 
         Args:
           p : probability of selecting first r.v.
           p1 : probability of occurence for first r.v.
           p2 : probability of occurence for other r.v.
           N : number of trials
+
+        Examples:
+          >>> p1 = (1. - 0.02) * (1. - 0.01)  # 2_p_x if vaccine given
+          >>> p2 = (1. - 0.02) * (1. - 0.02)  # 2_p_x if vaccine not given
+          >>> math.sqrt(Life.mixture(p=.2, p1=p1, p2=p2, N=100000, variance=True))
         """
         assert 0 <= p <= 1 and 0 <= p1 <= 1 and 0 <= p2 <= 1 and N >= 1
         mean1 = Life.binomial(p1, N)
         mean2 = Life.binomial(p2, N)
         var1 = Life.binomial(p1, N, variance=True)
         var2 = Life.binomial(p2, N, variance=True)
         return (Life.bernoulli(p, mean1, mean2, variance=True)  # var of mean
```

### Comparing `actuarialmath-0.0.9/src/actuarialmath/lifetable.py` & `actuarialmath-0.1.1/src/actuarialmath/lifetable.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     """Calculate life table, and iteratively fill in missing values
 
     Args:
       udd : assume UDD or constant force of mortality for fractional ages
       verbose : whether to echo update steps
 
     Notes:
-      4 types of information can be loaded and calculated in the life table:
+      4 types of columns can be loaded and calculated in the life table:
 
       - 'q' : probability (x) dies in one year
       - 'l' : number of lives aged x
       - 'd' : number of deaths of age x
       - 'p' : probability (x) survives at least one year
     """
 
@@ -46,29 +46,41 @@
         def _f(x: int, s, t: float) -> float:
             u = math.floor(t)   # f_x(u+r) = u_p_x * f_u(r)
             return self.p_x(x, s=s, t=u) * self.f_r(x, s=s+u, t=t-u)
 
         self.set_survival(mu=_mu, S=_S, f=_f, l=_l, minage=-1, maxage=-1)
 
 
-    def set_table(self, fill: bool = True, minage: int = -1, maxage: int = -1,
+    def set_table(self,
+                  radix: int = Reserves._RADIX,
+                  minage: int = -1,
+                  maxage: int = -1,
+                  fill: bool = True,
                   l: Dict[int, float] | None = None,
                   d: Dict[int, float] | None = None,
                   p: Dict[int, float] | None = None, 
                   q: Dict[int, float] | None = None) -> "LifeTable":
         """Update life table
 
         Args:
           l : lives at start of year x, or
           d : deaths in year x, or
           p : probabilities that (x) survives one year, or
           q : probabilities that (x) dies in one year
           fill : whether to automatically fill table cells (default is True)
           minage : minimum age in table
           maxage : maximum age in table
+          radix : initial number of lives
+
+        Examples:
+
+        >>> life = LifeTable(udd=True).set_table(l={90: 1000, 93: 825},
+        >>>                                      d={97: 72},
+        >>>                                      p={96: .2},
+        >>>                                      q={95: .4, 97: 1})
         """
 
         inputs = {k:v for k,v in {'l':l, 'd':d, 'q':q, 'p':p}.items() if v}
 
         # infer min and max ages from inputs
         if minage < 0:
             minage = min([min(v) for v in inputs.values()])
@@ -87,18 +99,18 @@
 
         # update table from inputs
         for label, col in inputs.items():
             self._table[label].update(col)
 
         # derive and fill table values
         if fill:
-            self.fill_table()
+            self.fill_table(radix=radix)
         return self
 
-    def fill_table(self, radix: int = Reserves._RADIX) -> "LifeTable":
+    def fill_table(self, radix: int) -> "LifeTable":
         """Iteratively fill in missing table cells (does not check consistency)
 
         Args:
           radix : initial number of lives
         """
 
         def q_x(x: int) -> float | None:
```

### Comparing `actuarialmath-0.0.9/src/actuarialmath/lifetime.py` & `actuarialmath-0.1.1/src/actuarialmath/lifetime.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,25 +33,24 @@
 
         if t == 1 and curtate:      # shortcut for e_x:1
             return self.p_x(x, s=s, t=1)
         
         t = self.max_term(x+s, t)   # length of term must be bounded by max age
         if curtate:
             if moment == 1:
-                return sum([self.p_x(x, s=s, t=k)
-                            for k in range(1, round(t+1))]) 
+                return sum([self.p_x(x, s=s, t=k) for k in range(1, round(t+1))]) 
             e2 = sum([((2 * k) - 1) * self.p_x(x, s=s, t=k)
                       for k in range(1, round(t+1))])
         else:
             if moment == 1:
                 return self.integral(lambda t: self.S(x, s, t), 0., float(t))
             e2 = self.integral(lambda t: 2 * t * self.S(x, s, t), 0., float(t))
 
         if moment == self.VARIANCE:  # variance is E[T_x^2] - E[T_x]^2
-            return e2 - self.e(x, s=s, t=t, curtate=curtate, moment=1)**2
+            return e2 - self.e_x(x, s=s, t=t, curtate=curtate, moment=1)**2
         return e2   # return second moment
 
 
 if __name__ == "__main__":
     print("SOA Question 2.4: (E) 8.2")
     def l(x, s): return 0. if (x+s) >= 100 else 1 - ((x + s)**2) / 10000.
     e = Lifetime().set_survival(l=l).e_x(75, t=10, curtate=False)
```

### Comparing `actuarialmath-0.0.9/src/actuarialmath/mortalitylaws.py` & `actuarialmath-0.1.1/src/actuarialmath/udd.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,322 +1,274 @@
-"""Mortality Laws: Applies shortcut formulas for Beta, Uniform, Makeham and Gompertz
+"""UDD - 1/mthly insurance and annuities with uniform distribution of deaths
 
 MIT License. Copyright 2022-2023 Terence Lim
 """
-import math
-from actuarialmath import Reserves
+import pandas as pd
+from actuarialmath import Interest
+from actuarialmath import Annuity
+from actuarialmath import Mthly
 
-class MortalityLaws(Reserves):
-    """Apply shortcut formulas for special mortality laws"""
+class UDD(Mthly):
+    """1/mthly shortcuts with UDD assumption
 
-    #
-    # Define fractional age actuarial survival functions
-    #
-    def l_r(self, x: int, s: int = 0, r: float = 0.) -> float:
-        """Fractional lives given special mortality law: l_[x]+s+r
+    Args:
+      m : number of payments per year
+      life : original fractional survival and mortality functions
+    """
 
-        Args:
-          x : age of selection
-          s : years after selection
-          r : fractional year after selection
-        """
-        return self.l(x, s+r)
+    def __init__(self, m: int, life: Annuity, **kwargs):
+        super().__init__(m=m, life=life, **kwargs)
+        self.alpha_m = self.alpha(m=m, i=self.life.interest.i)
+        self.beta_m = self.beta(m=m, i=self.life.interest.i)
 
-    def p_r(self, x: int, s: int = 0, r: float = 0., t: float = 1.) -> float:
-        """Fractional age survival probability given special mortality law
+    @staticmethod
+    def alpha(m: int, i: float) -> float:
+        """Compute 1/mthly UDD interest rate beta function value
 
         Args:
-          x : age of selection
-          s : years after selection
-          r : fractional year after selection
-          t : death within next t fractional years
+          m : number of payments per year
+          i : annual interest rate
         """
-        return self.S(x, s+r, t)
+        d = i / (1 + i)
+        i_m = Interest.mthly(m=m, i=i)
+        i_d = Interest.mthly(m=m, d=d)
+        return abs(i*d / ( i_m * i_d))
 
-    def q_r(self, x: int, s: int = 0, r: float = 0., t: float = 1., 
-            u: float = 0.) -> float:
-        """Fractional age deferred mortality given special mortality law
+    @staticmethod
+    def beta(m: int, i: float) -> float:
+        """Compute 1/mthly UDD interest rate alpha function value
 
         Args:
-          x : age of selection
-          s : years after selection
-          r : fractional year after selection
-          u : survive u fractional years, then...
-          t : death within next t fractional years
+          m : number of payments per year
+          i : annual interest rate
         """
-        return self.p_r(x, s=s, r=r, t=u) - self.p_r(x, s=s, r=r, t=t+u)
-        
-    def mu_r(self, x: int, s: int = 0, r: float = 0.) -> float:
-        """Fractional age force of mortality given special mortality law
+        d = i / (1 + i)
+        i_m = Interest.mthly(m=m, i=i)
+        i_d = Interest.mthly(m=m, d=d)
+        return abs((i - i_m) / (i_m * i_d))
 
+    def whole_life_insurance(self, x: int, s: int = 0, moment: int = 1, 
+                             b: int = 1) -> float:
+        """1/mthly UDD Whole life insurance: A_x
+ 
         Args:
           x : age of selection
           s : years after selection
-          r : fractional year after selection
-        """
-        return self.mu(x, s+r)
-
-    def f_r(self, x: int, s: int = 0, r: float = 0., t: float = 0.0) -> float:
-        """fractional age lifetime density given special mortality law
+          b : amount of benefit
+          moment : compute first or second moment
 
-        Args:
-          x : age of selection
-          s : years after selection
-          r : fractional year after selection
-          t : mortality at fractional year t
+        Examples:
+          >>> UDD(m=0, life=SULT(udd=True)).whole_life_insurance(x)
         """
-        return self.f(x, s+r, t)
-
-    def e_r(self, x: int, s: int = 0, r: float = 0.,
-            t: float = Reserves.WHOLE) -> float:
-        """Fractional age future lifetime given special mortality law
+        assert moment in [1, 2, Annuity.VARIANCE]
+        if moment == Annuity.VARIANCE:
+            return ((self.whole_life_insurance(x, s=s, moment=2) -
+                     self.whole_life_insurance(x, s=s)**2) * b**2)
+        A = self.life.whole_life_insurance(x, s=s, moment=moment)
+        i = self.life.interest.i
+        if moment == 2:
+            i = self.interest.double_force(i)
+        i_m = self.life.interest.mthly(m=self.m, i=i)        
+        return A * i / i_m
+
+    def endowment_insurance(self, x: int, s: int = 0, t: int = 1, b: int = 1, 
+                            endowment: int = -1, moment: int = 1) -> float:
+        """1/mthly UDD Endowment insurance = term insurance + pure endowment
 
         Args:
-          x : age of selection
+          x : year of selection
           s : years after selection
-          r : fractional year after selection
-          t : limited at t years
+          t : term of insurance in years
+          b : amount of benefit
+          endowment : amount of endowment
+          moment : return first or second moment
         """
-        if t < 0:
-            t = self._MAXAGE - (x + s + r)
-        return self.integrate(lambda t: self.S(x, s+r, t), 0., float(t))
-
-class Beta(MortalityLaws):
-    """Shortcuts with beta distribution of deaths (is Uniform when alpha = 1)
-
-    Args:
-      omega : maximum age
-      alpha : alpha paramter of beta distribution
-      lives : assumed starting number of lives for survival function
-    """
-    
-    def __init__(self, omega: int, alpha: float,
-                 lives: int = MortalityLaws._RADIX, **kwargs): 
-        """Two parameters: alpha and omega, with mu(x) = alpha/(omega-x)"""
-
-        super().__init__(**kwargs)
-
-        def _mu(x: int, s: float) -> float: 
-            return alpha / (omega - (x+s))
-
-        def _l(x: int, s: float) -> float:
-            return lives * (omega - (x+s))**alpha
+        assert moment in [1, 2, Annuity.VARIANCE]
+        if moment == Annuity.VARIANCE:
+            return (self.endowment_insurance(x, s=s, t=t, endowment=endowment, 
+                                             b=b, moment=2) -
+                    self.endowment_insurance(x, s=s, t=t, endowment=endowment,
+                                             b=b)**2)
+        E = self.E_x(x, s=s, t=t, moment=moment)
+        A = self.term_insurance(x, s=s, t=t, b=b, moment=moment)
+        return A  + E * (b if endowment < 0 else endowment)**moment
 
-        def _S(x: int, s,t : float) -> float:
-            return ((omega-(x+s+t))/(omega-(x+s)))**alpha
 
-        def _f(x: int, s,t : float) -> float:
-            return alpha / (omega - (x+s))
-
-        self.set_survival(mu=_mu, l=_l, S=_S, f=_f, minage=0, maxage=omega)
-        self.omega_ = omega  # store omega parameter
-        self.alpha_ = alpha  # store alpha parameter
-
-    def e_r(self, x: int, s: int = 0, t: float = Reserves.WHOLE) -> float:
-        """Expectation of future lifetime through fractional age: e_[x]+s:t
+    def term_insurance(self, x: int, s: int = 0, t: int = 1, b: int = 1, 
+                       moment: int = 1) -> float:
+        """1/mthly UDD Term insurance: A_x:t
 
         Args:
-          x : age of selection
+          x : year of selection
           s : years after selection
-          t : limited at t years
-        """
-        e = (self.omega_ - (x+s)) / (self.alpha_ + 1)
-        if t > 0 and self.max_term(x+s, t) > t: # temporary expectation
-            return e - self.p_r(x, s=s, t=t) * self.e_r(x, s=s+t)
-        return e   # complete expectation
-
-    def e_x(self, x: int, s: int = 0, n: int = MortalityLaws.WHOLE, 
-          curtate: bool = False, moment: int = 1) -> float:
-        """Shortcut formula for complete expectation
+          t : term of insurance in years
+          b : amount of benefit
+          moment : return first or second moment
 
-        Args:
-          x : age of selection
-          s : years after selection
-          n : death within next n fractional years
-          t : limited at t years
-          curtate : whether curtate (True) or complete (False) lifetime
-          moment : whether to compute first (1) or second (2) moment
+        Examples:
+          >>> UDD(m=12, life=SULT(udd=True)).term_insurance(45)
         """
-        if n == 0:
-            return 0
-        if not curtate:
-            if moment == 1:
-                return self.e_r(x, s=s, t=n)
-            if moment == self.VARIANCE and n < 0: # shortcut for complete variance
-                return ((self.omega_ - (x + s))
-                        / ((self.alpha_ + 1)**2 * (self.alpha_ + 1)))
-        return super().__init__(x=x, s=s, n=n, curtate=curtate, moment=moment)
-
-class Uniform(Beta):
-    """Shortcuts with uniform distribution of deaths aka DeMoivre's Law
-
-    Args:
-      omega : maximum age
-      udd : assume UDD (True, default) or CFM (False) between integer ages
-    """
-
-    def __init__(self, omega: int, udd: bool = True, **kwargs):
-        """One parameter: omega = maxage, with mu(x) = 1/(omega - x)"""
-        super().__init__(omega=omega, alpha=1, udd=udd, **kwargs)
-
-    def e_x(self, x: int, s: int = 0, t: int = Beta.WHOLE, 
-          curtate: bool = False, moment: int = 1) -> float:
-        """Shortcut for expected future lifetime
+        assert moment in [1, 2, Annuity.VARIANCE]
+        if moment == Annuity.VARIANCE:
+            return (self.term_insurance(x, s=s, t=t, b=b, moment=2) -
+                    self.term_insurance(x, s=s, t=t, b=b)**2)
+        A = self.life.term_insurance(x, s=s, t=t, b=b, moment=moment)
+        i = self.life.interest.i
+        if moment == 2:
+            i = self.interest.double_force(i)
+        i_m = self.life.interest.mthly(m=self.m, i=i)        
+        return A * (i / i_m)
+
+    def whole_life_annuity(self, x: int, s: int = 0, b: int = 1, 
+                           variance: bool = False) -> float:
+        """1/mthly UDD Whole life annuity: a_x
 
         Args:
-          x : age of selection
+          x : year of selection
           s : years after selection
-          t : limited at t years
-          curtate : whether curtate (True) or complete (False) lifetime
-          moment : whether to compute first (1) or second (2) moment
-        """
-        if moment in [1, self.VARIANCE] and not curtate:
-            if t < 0:
-                if moment == self.VARIANCE:
-                    return (self.omega_ - x)**2 / 12  # complete shortcut
-                else:
-                    return (self.omega_ - x) / 2
-            elif moment == 1:         # temporary expectation shortcut
-                # (Pr[die within n years] * n/2) plus (Pr[survive n years] * n)
-                t = self.max_term(x+s, t)
-                t_p_x = t / (self.omega_ - x)
-                return t_p_x * t  + (1 - t_p_x) * (t / 2)
-        return super().__init__(x=x, s=s, t=t, curtate=curtate, moment=moment)
-
-    
-    def E_x(self, x: int, s: int = 0, t: int = Beta.WHOLE, 
-            moment: int = 1) -> float:
-        """Shortcut for Pure Endowment
+          b : amount of benefit
+          variance : return first moment (False) or variance (True)
 
-        Args:
-          x : age of selection
-          s : years after selection
-          t : term of pure endowment
-          endowment : amount of pure endowment
-          moment : compute first or second moment
+        Examples:
+          >>> UDD(m=12, life=SULT(udd=True)).whole_life_annuity(x)
         """
-        assert moment > 0
-        if t == 0:
-            return 1.
-        if t < 0:
-            return 0.
-        t = self.max_term(x+s, t)
-        t_p_x = (self.omega_ - x - t) / (self.omega_ - x)
-        if moment == self.VARIANCE:  # Bernoulli shortcut for variance
-            return self.interest.v_t(t)**2 * t_p_x * (1 - t_p_x)
-        return (self.interest.v_t(t)**moment * (self.omega_ - x - t) 
-                / (self.omega_ - x))
-
-    def whole_life_insurance(self, x: int, s: int = 0, moment: int = 1, 
-                             b: int = 1, discrete: bool = True) -> float:
-        """Shortcut for whole life insurance
+        if variance:  # short cut for variance of whole life
+            A1 = self.whole_life_insurance(x, s=s, moment=1)
+            A2 = self.whole_life_insurance(x, s=s, moment=2)
+            return (b**2 * (A2 - A1**2) / self.d**2)
+        a = self.life.whole_life_annuity(x, s=s)
+        return b * (a * self.alpha_m - self.beta_m)
+            
+    def temporary_annuity(self, x: int, s: int = 0, t: int = Annuity.WHOLE, 
+                          b: int = 1, variance: bool = False) -> float:
+        """1/mthly UDD Temporary life annuity: a_x:t
 
         Args:
-          x : age of selection
+          x : year of selection
           s : years after selection
+          t : term of annuity in years
           b : amount of benefit
-          moment : compute first or second moment
-          discrete : benefit paid year-end (True) or moment of death (False)
+          variance : return first moment (False) or variance (True)
+
+        Examples:
+          >>> UDD(m=12, life=SULT(udd=True)).temporary_annuity(45, t=20)
         """
+        if variance:  # short cut for variance of temporary life annuity
+            A1 = self.temporary_insurance(x, s=s, t=t)
+            A2 = self.temporary_insurance(x, s=s, t=t, moment=2)
+            return (b**2 * (A2 - A1**2) / self.d**2)
 
-        if not discrete:
-            if moment == Beta.VARIANCE:
-                return (self.whole_life_insurance(x, s=s, b=b, moment=2, 
-                                                  discrete=False) -
-                        self.whole_life_insurance(x, s=s, b=b, moment=1, 
-                                                    discrete=False)**2) * b**2
-            return self.term_insurance(x, s=s, t=self.omega_-(x+s), b=b,
-                                       moment=moment, discrete=False)
-        return super().whole_life_insurance(x, s=s, moment=moment, b=b,
-                                            discrete=discrete)
+        # difference of whole life on (x) and deferred whole life on (x+t)
+        if t < 0:
+            return self.whole_life_annuity(x, b=b, s=s)  # UDD
+        a = self.life.temporary_annuity(x, s=s, t=t)
+        return b * (a*self.alpha_m - self.beta_m*(1 - self.E_x(x, s=s, t=t)))
 
-    def term_insurance(self, x: int, s: int = 0, t: int = 1, b: int = 1, 
-                       moment: int = 1, discrete: bool = False) -> float:
-        """Shortcut for term insurance
+    def deferred_annuity(self, x: int, s: int = 0, u: int = 0, 
+                         t: int = Annuity.WHOLE, b: int = 1,
+                         variance: bool = False) -> float:
+        """1/mthly UDD Deferred life annuity n|t_a_x =  n+t_a_x - n_a_x
 
         Args:
-          x : age of selection
+          x : year of selection
           s : years after selection
-          t : term of insurance
+          u : years of deferral
+          t : term of annuity in years
           b : amount of benefit
-          moment : compute first or second moment
-          discrete : benefit paid year-end (True) or moment of death (False)
         """
-        if not discrete and moment in [1, Beta.VARIANCE]:
-            if moment == Beta.VARIANCE:
-                return (self.term_insurance(x, s=s, b=b, t=t, moment=2, 
-                                            discrete=False) -
-                        self.term_insurance(x, s=s, b=b, t=t, 
-                                            discrete=False)**2) * b**2
-            t = self.max_term(x+s, t)                                        
-            return (b * (1 - self.interest.v_t(t)) 
-                    / (self.interest.delta * (self.omega_ - (x+s))))
-        return super().term_insurance(x, s=s, moment=moment, b=b, 
-                                      discrete=discrete)
+        if self.max_term(x+s, n) < n:
+            return 0.
+        if variance:  # short cut for variance of temporary life annuity
+            A1 = self.endowment_insurance(x, s=s, t=t)
+            A2 = self.endowment_insurance(x, s=s, t=t, moment=2)
+            return (b**2 * (A2 - A1**2) / self.d**2)
+
+        a = self.life.deferred_annuity(x, s=s, u=u, t=t)
+        return (a * self.alpha_m - self.beta_m * self.E_x(x, s=s, t=u)) * b
+
+    @staticmethod
+    def interest_frame(i: float = 0.05):
+        """Return 1/mthly UDD interest function values in a DataFrame
+
+        Args:
+          i : annual interest rate
+        """
+        interest = Interest(i=i)
+        out = pd.DataFrame(columns=["i(m)", "d(m)", "i/i(m)", "d/d(m)", 
+                                    "alpha(m)", "beta(m)"],
+                           index=[1, 2, 4, 12, 0], 
+                           dtype=float)
+        for m in out.index:
+            i_m = Interest.mthly(m=m, i=interest.i)
+            d_m = Interest.mthly(m=m, d=interest.d)
+            out.loc[m] = [i_m, d_m, interest.i/i_m, interest.d/d_m, 
+                          UDD.alpha(m=m, i=interest.i), 
+                          UDD.beta(m=m, i=interest.i)]
+        return out.round(5)
 
-class Makeham(MortalityLaws):
-    """Includes element in force of mortality that does not depend on age
 
-    Args:
-      A, B, c : parameters of Makeham distribution
-    """
+if __name__ == "__main__":
+    from actuarialmath.sult import SULT
+    from actuarialmath.policyvalues import Contract
     
-    def __init__(self, A: float, B: float, c: float, **kwargs):
-        assert c > 1, "Makeham requires c > 1"
-        assert B > 0, "Makeham requires B > 0"
-        assert A >= -B, "Makeham requires A >= -B"        
-        super().__init__(**kwargs)
-        self.A_ = A
-        self.B_ = B
-        self.c_ = c
-
-        def _mu(x, s): 
-            return A + B * c**(x+s)
-        
-        def _S(x, s, t):
-            return math.exp(-A*t - B*c**(x+s) * (c**t - 1)/math.log(c))
-
-        self.set_survival(mu=_mu, S=_S)
-
-class Gompertz(Makeham):
-    """Is Makeham's Law with A = 0
+    print("SOA Question 7.9:  (A) 38100")
+    sult = SULT(udd=True)
+    x, n, t = 45, 20, 10
+    a = UDD(m=12, life=sult).temporary_annuity(x+10, t=n-10)
+    print(a)
+    A = UDD(m=0, life=sult).endowment_insurance(x+10, t=n-10)
+    print(A)
+    print(A*100000 - a*12*253)
+    contract = Contract(premium=253*12, endowment=100000, benefit=100000)
+    print(sult.gross_future_loss(A=A, a=a, contract=contract))
+    print()
 
-    Args:
-      B, c : parameters of Gompertz distribution
-    """
+    print("SOA Question 6.49:  (C) 86")
+    sult = SULT(udd=True)
+    a = UDD(m=12, life=sult).temporary_annuity(40, t=20)
+    A = sult.whole_life_insurance(40, discrete=False)
+    P = sult.gross_premium(a=a, A=A, benefit=100000, initial_policy=200,
+                           renewal_premium=0.04, initial_premium=0.04)
+    print(P/12)
+    print()
 
-    def __init__(self, B: float, c: float):
-        """Gompertz's Law is Makeham's Law with A = 0"""
-        super().__init__(A=0., B=B, c=c)
+    from actuarialmath.recursion import Recursion    
+    print("SOA Question 6.38:  (B) 11.3")
+    x, n = 0, 10
+    life = Recursion().set_interest(i=0.05)\
+                      .set_A(0.192, x=x, t=n, endowment=1, discrete=False)\
+                      .set_E(0.172, x=x, t=n)
+    a = life.temporary_annuity(x, t=n, discrete=False)
+    print(a)
+
+    def fun(a):      # solve for discrete annuity, given continuous
+        life = Recursion().set_interest(i=0.05)\
+                          .set_a(a, x=x, t=n)\
+                          .set_E(0.172, x=x, t=n)
+        return UDD(m=0, life=life).temporary_annuity(x, t=n)
+    a = life.solve(fun, target=a, grid=a)  # discrete annuity
+    P = life.gross_premium(a=a, A=0.192, benefit=1000)
+    print(P)
+    print()
 
-if __name__ == "__main__":
-    print('Beta')
-    life = Beta(omega=100, alpha=0.5)
-    print(life.q_x(25, t=1, u=10))     # 0.0072
-    print(life.e_x(25))                # 50
-    print(Beta(omega=60, alpha=1/3).mu_x(35) * 1000)
+    print("SOA Question 6.32:  (C) 550")
+    x = 0
+    life = Recursion().set_interest(i=0.05).set_a(9.19, x=x)
+    benefits = UDD(m=0, life=life).whole_life_insurance(x)
+    payments = UDD(m=12, life=life).whole_life_annuity(x)
+    print(benefits, payments)
+    print(life.gross_premium(a=payments, A=benefits, benefit=100000)/12)
     print()
 
-    print('Uniform')
-    uniform = Uniform(80).set_interest(delta=0.04)
-    print(uniform.whole_life_annuity(20, discrete=False))        # 15.53
-    print(uniform.temporary_annuity(20, t=5, discrete=False))   # 4.35
-    print(Uniform(161).p_x(70, t=1)) # 0.98901
-    print(Uniform(95).e_x(30, t=40, curtate=False)) # 27.692
+    print("SOA Question 6.22:  (C) 102")
+    life = SULT(udd=True)
+    a = UDD(m=12, life=life).temporary_annuity(45, t=20)
+    A = UDD(m=0, life=life).whole_life_insurance(45)
+    print(life.gross_premium(A=A, a=a, benefit=100000)/12)
     print()
 
-    uniform = Uniform(omega=80).set_interest(delta=0.04)
-    print(uniform.E_x(20, t=5))  # .7505
-    print(uniform.whole_life_insurance(20, discrete=False))  # .3789
-    print(uniform.term_insurance(20, t=5, discrete=False))  # .0755
-    print(uniform.endowment_insurance(20, t=5, discrete=False))  # .8260
-    print(uniform.deferred_insurance(20, u=5, discrete=False))  # .3033
+    print("Interest Functions at i=0.05")
+    print("----------------------------")
+    print(UDD.interest_frame(i=0.05))
     print()
 
-    print('Gompertz/Makeham')
-    life = Gompertz(B=0.000005, c=1.10)
-    p = life.p_x(80, t=10)  # 869.4
-    print(life.portfolio_percentile(N=1000, mean=p, variance=p*(1-p), prob=0.99)) 
-
-    print(Gompertz(B=0.00027, c=1.1).f_x(50, t=10)) # 0.04839
-    life = Makeham(A=0.00022, B=2.7e-6, c=1.124)
-    print(life.mu_x(60) * 0.9803)  # 0.00316
+
```

### Comparing `actuarialmath-0.0.9/src/actuarialmath/mthly.py` & `actuarialmath-0.1.1/src/actuarialmath/mthly.py`

 * *Files 5% similar despite different names*

```diff
@@ -57,48 +57,54 @@
           t_m : survives number of m'thly periods
         """
         sr = s_m / self.m
         s = math.floor(sr)
         r = sr - s
         return self.life.p_r(x, s=s, r=r, t=t_m/self.m)
 
-    def E_x(self, x: int, s: int = 0, t: int = 1, moment: int = 1,
-            endowment: int = 1) -> float:
-        """Compute pure endowment factor
-
-        Args:
-          x : year of selection
-          s : years after selection
-          t : term length in years
-          moment : return first or second moment
-          endowment : endowment amount
-        """
-        assert moment > 0
-        return self.life.E_x(x, s=s, t=t, moment=moment) * endowment**moment
-
     def Z_m(self, x: int, s: int = 0, t: int = 1, 
             benefit: Callable = lambda x,t: 1, moment: int = 1):
         """Return PV of insurance r.v. Z and probability of death at mthly intervals
 
         Args:
           x : year of selection
           s : years after selection
           t : year of death
           benefit : amount of benefit by year and age selected
           moment : return first or second moment
         
         Returns:
           DataFrame, indexed by mthly period, with column names ['Z', 'p']
+
+        Examples:
+          >>> life = LifeTable(udd=False).set_table(q={0:.16,1:.23})\
+          >>>                            .set_interest(i_m=.18,m=2)
+          >>> mthly = Mthly(m=2, life=life)
+          >>> Z = mthly.Z_m(0, t=2, benefit=lambda x,t: 300000 + t*30000*2)
         """
         Z = [(benefit(x+s, k/self.m) * self.v_m(k+1))**moment 
              for k in range(t * self.m)]
         q = [self.q_m(x, s_m=s*self.m, u_m=k) for k in range (t*self.m)]
         return pd.DataFrame.from_dict(dict(m=range(1, self.m*t + 1), Z=Z, q=q))\
                            .set_index('m')
 
+    def E_x(self, x: int, s: int = 0, t: int = 1, moment: int = 1,
+            endowment: int = 1) -> float:
+        """Compute pure endowment factor
+
+        Args:
+          x : year of selection
+          s : years after selection
+          t : term length in years
+          moment : return first or second moment
+          endowment : endowment amount
+        """
+        assert moment > 0
+        return self.life.E_x(x, s=s, t=t, moment=moment) * endowment**moment
+
     def A_x(self, x: int, s: int = 0, t: int = 1, u: int = 0, 
             benefit: Callable = lambda x,t: 1, moment: int = 1) -> float:
         """Compute insurance factor with m'thly benefits
 
         Args:
           x : year of selection
           s : years after selection
@@ -125,16 +131,16 @@
 
         Args:
           x : age of selection
           s : years after selection
           b : amount of benefit
           moment : compute first or second moment
         """
-        assert moment in [1, 2, Annuity.VARIANCE]
-        if moment == Annuity.VARIANCE:
+        assert moment in [1, 2, Actuarial.VARIANCE]
+        if moment == Actuarial.VARIANCE:
             A2 = self.whole_life_insurance(x, s=s, moment=2)
             A1 = self.whole_life_insurance(x, s=s)
             return self.life.insurance_variance(A2=A2, A1=A1, b=b)
         return sum(self.A_x(x, s=s, b=b, moment=moment))
 
 
     def term_insurance(self, x: int, s: int = 0, t: int = 1, b: int = 1, 
@@ -144,16 +150,16 @@
         Args:
           x : year of selection
           s : years after selection
           t : term of insurance in years
           b : amount of benefit
           moment : return first or second moment
         """
-        assert moment in [1, 2, Annuity.VARIANCE]
-        if moment == Annuity.VARIANCE:
+        assert moment in [1, 2, Actuarial.VARIANCE]
+        if moment == Actuarial.VARIANCE:
             A2 = self.term_insurance(x, s=s, t=t, moment=2)
             A1 = self.term_insurance(x, s=s, t=t)
             return self.life.insurance_variance(A2=A2, A1=A1, b=b)
         A = self.whole_life_insurance(x, s=s, b=b, moment=moment)
         if t < 0 or self.life.max_term(x+s, t) < t:
             return A
         E = self.E_x(x, s=s, t=t, moment=moment)
@@ -215,26 +221,34 @@
         return (1 - d_m * a)
 
     def annuity_twin(self, A: float) -> float:
         """Return value of annuity twin of m'thly insurance
 
         Args:
           A : amount of m'thly insurance
+
+        Examples:
+          >>> mthly = Mthly(m=12, life=Annuity().set_interest(i=0.06))
+          >>> mthly.annuity_twin(A=0.4075)*15*12
         """
         d = self.life.interest.d
         d_m = self.life.interest.mthly(m=self.m, d=d)        
         return (1-A) / d_m
 
     def annuity_variance(self, A2: float, A1: float, b: float = 1) -> float:
         """Variance of m'thly annuity from m'thly insurance moments
 
         Args:
           A2 : double force of interest of m'thly insurance
           A1 : first moment of m'thly insurance
           b : amount of benefit
+
+        Examples:
+          >>> mthly = Mthly(m=12, life=Annuity().set_interest(i=0.06))
+          >>> mthly.annuity_variance(A1=0.4075, A2=0.2105, b=15*12)
         """
         num = self.life.insurance_variance(A2=A2, A1=A1, b=b)
         den = self.life.interest.mthly(m=self.m, d=self.life.interest.d)
         return num / den**2
 
     def whole_life_annuity(self, x: int, s: int = 0, b: int = 1, 
                            variance: bool = False) -> float:
```

### Comparing `actuarialmath-0.0.9/src/actuarialmath/policyvalues.py` & `actuarialmath-0.1.1/src/actuarialmath/policyvalues.py`

 * *Files 14% similar despite different names*

```diff
@@ -57,15 +57,23 @@
         for key, value in terms.items():
             if hasattr(self, key):
                 setattr(self, key, value)
         return self
 
     @property
     def premium_terms(self) -> Dict:    # terms required by gross_premiums 
-        """Getter returns dict of terms required for calculating gross premiums"""
+        """Dict of terms required for calculating gross premiums
+
+        Examples:
+          >>> life = PolicyValues().set_interest(i=0.04)
+          >>> contract = Contract(premium=2.338, benefit=100, initial_premium=.1, 
+          >>>                     renewal_premium=0.05)
+          >>> contract.premium = life.gross_premium(a=12, A=life.insurance_twin(a),
+          >>>                                       **contract.premium_terms)
+        """
         return dict(benefit=self.benefit,
                     initial_policy=self.initial_policy,
                     initial_premium=self.initial_premium,
                     renewal_policy=self.renewal_policy,
                     renewal_premium=self.renewal_premium,
                     settlement_policy=self.settlement_policy)
 
@@ -84,118 +92,118 @@
                         discrete=self.discrete,
                         premium=self.premium,
                         endowment=self.endowment,
                         T=self.T - t)
 
     @property
     def renewal_profit(self) -> float:
-        """Getter returns renewal dollar profit (premium less renewal expenses)"""
+        """Renewal dollar profit (premium less renewal expenses)"""
         # premium less renewal per premium and expense"""
         return ((self.premium * (1 - self.renewal_premium)) - self.renewal_policy)
 
     @property
     def initial_cost(self) -> float:
-        """Getter returns total initial cost (excludes renewal expenses)"""
+        """Total initial cost (net of renewal component of expenses and premiums)"""
         return ((self.initial_policy - self.renewal_policy) +
                 (self.premium * (self.initial_premium - self.renewal_premium)))
 
     @property
     def claims_cost(self) -> float:
-        """Getter returns total claims cost (death benefit + settlement expense)"""
+        """Total claims cost (death benefit + settlement expense)"""
         return self.benefit + self.settlement_policy
 
 class PolicyValues(Premiums):
     """Compute net and gross future losses and policy values"""
     
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
 
     #
     # Net Future Loss shortcuts for WL and Endowment Insurance 
     #
     def net_future_loss(self, A: float, A1: float, b: int = 1) -> float:
-        """Shortcuts for WL or Endowment Insurance net loss
+        """Shortcut for net policy value with WL or Endowment Insurance factors
 
         Args:
           A : insurance factor at age (x)
           A1 : insurance factor at t years after x
           b : benefit amount
         """
         return b * (A1 - A) / (1 - A)
 
     def net_variance_loss(self, A1: float, A2: float, A: float = 0, 
                          b: int = 1) -> float:
-        """Shortcuts for variance of net loss of WL or Endowment Insurance
+        """Variance of net loss with WL or Endowment Insurance factors
 
         Args:
           A : insurance factor at age (x)
           A1 : first moment of insurance factor at t years after x
           A2 : insurance factor at double force of interest t years after x
           b : benefit amount
         """
         if not A:
             A = A1   # assume t = 0 => A = A1
         return b**2 * (A2 - A1**2) / (1 - A)**2
 
     def net_policy_variance(self, x, s: int = 0, t: int = 0, b: int = 1, 
                             n: int = Premiums.WHOLE, endowment: int = 0, 
                             discrete: bool = True) -> float:
-        """Variance of future loss for WL or Endowment Ins assuming equivalence
+        """Variance of net future loss for WL or Endowment Insurance only
 
         Args:
           x : age of selection
           s : years after selection
-          t : term of life annuity in years
-          n : number of years premiums paid
+          n : term of life insurance
+          t : years after issue to compute policy variance
           b : benefit amount
           endowment : endowment amount
           discrete : annuity due (True) or continuous (False)
         """
         if n < 0:             # Whole Life
             A2 = self.whole_life_insurance(x, s=s+t, moment=2,
                                             discrete=discrete)
             A1 = self.whole_life_insurance(x, s=s+t, discrete=discrete)
             A = self.whole_life_insurance(x, s=s, discrete=discrete)
         elif endowment == b:   # Endowment Insurance 
-            n = self.max_term(x+s+t, n)
+            n = self.max_term(x=x+s+t, t=n)
             A2 = self.endowment_insurance(x, s=s+t, t=n-t, moment=2,
                                             discrete=discrete)
             A1 = self.endowment_insurance(x, s=s+t, t=n-t, discrete=discrete)
             A = self.endowment_insurance(x, s=s, t=n, discrete=discrete)
         else:
             raise Exception("Variances for WL and Endowment Ins only")
         return self.net_variance_loss(A=A, A1=A1, A2=A2, b=b)
 
     #
     # Net Policy Value for special and WL/endowment insurance
     #
     def net_policy_value(self, x: int, s: int = 0, t: int = 0, b: int = 1, 
                          n: int = Premiums.WHOLE, endowment: int = 0, 
                          discrete: bool = True) -> float:
-        """Net policy value assuming premiums from equivalence: E[L_t]
+        """Net policy value assuming net premiums from equivalence principle: E[L_t]
 
         Args:
           x : age initially insured
           s : years after selection
-          n : number of years of premiums paid
-          t : year of death
+          n : term of life insurance
+          t : years after issue to compute policy variance
           b : benefit amount
           endowment : endowment amount
           discrete : discrete/annuity due (True) or continuous (False)
         """
         if n < 0:             # Shortcut available for Whole Life
             A1 = self.whole_life_insurance(x, s=s+t, discrete=discrete)
             A = self.whole_life_insurance(x, s=s, discrete=discrete)
         elif endowment == b:  # Shortcut available for (equal) Endowment Insurance
-            n = self.max_term(x+s+t, n)
+            n = self.max_term(x=x+s+t, t=n)
             A1 = self.endowment_insurance(x, s=s+t, t=n-t, 
                                             discrete=discrete)
             A = self.endowment_insurance(x, s=s, t=n, discrete=discrete)
         else:   # Special Term or (unequal) Endowment insurance has no shortcut
-            n = self.max_term(x+s+t, n)
+            n = self.max_term(x=x+s+t, t=n)
             A1 = self.endowment_insurance(x, s=s+t, t=n-t, discrete=discrete,
                                             b=b, endowment=endowment)
             a1 = self.temporary_annuity(x, s=s+t, t=n-t, b=b, 
                                         discrete=discrete)
             A = self.endowment_insurance(x, s=s, t=n, discrete=discrete,
                                             b=b, endowment=endowment)
             a = self.temporary_annuity(x, s=s, t=n, b=b, discrete=discrete)
@@ -204,15 +212,15 @@
 
     #
     # Gross Future Loss shortcuts for WL and Endowment Insurance 
     #
     def gross_future_loss(self, A: float | None = None, 
                           a: float | None = None, 
                           contract: Contract | None = None) -> float:
-        """Shortcut for WL or Endowment Insurance gross future loss
+        """Shortcut for gross policy value with WL or Endowment Insurance factors
 
         Args:
           A : insurance factor at age (x)
           a : annuity factor at age (x)
           contract : policy contract terms and expenses
         """
         contract = contract or Contract()
@@ -221,46 +229,46 @@
         elif A is None:  # assume WL or Endowment Insurance for twin annuity
              A = self.insurance_twin(a, discrete=contract.discrete)
         return ((A * contract.claims_cost + contract.initial_cost) -
                 (a * contract.renewal_profit))
 
     def gross_variance_loss(self, A1: float, A2: float = 0,
                             contract: Contract | None = None) -> float:
-        """Shortcuts for variance of gross loss for WL or endowment insurance
+        """Variance of gross loss with WL or endowment insurance factors
 
         Args:
           A1 : insurance factor
           A2 : insurance factor at double the force of interest
           policy : policy terms and expenses
         """
         contract = contract or Contract()
         interest = self.interest.d if contract.discrete else self.interest.delta
         return (((contract.renewal_profit / interest) + contract.benefit +
                  contract.settlement_policy)**2 * (A2 - A1**2))
 
     def gross_policy_variance(self, x: int, s: int = 0, t: int = 0,
                               n: int = Premiums.WHOLE,
                               contract: Contract | None = None) -> float:
-        """Variance of gross policy value for WL and Endowment Insurance
+        """Variance of gross policy value for WL and Endowment Insurance only
 
         Args:
           x : age initially insured
           s : years after selection
-          n : number of years of premiums paid
-          t : year of death
+          n : term of life insurance
+          t : years after issue to compute policy variance
           contract : policy contract terms and expenses
         """
         contract = contract or Contract()
         if n < 0:  # WL
             A2 = self.whole_life_insurance(x, s=s+t, moment=2,
                                             discrete=contract.discrete)
             A1 = self.whole_life_insurance(x, s=s+t, 
                                             discrete=contract.discrete)
         elif contract.endowment == contract.claims_cost:  # Endowment
-            n = self.max_term(x+s+t, n)
+            n = self.max_term(x=x+s+t, t=n)
             A2 = self.endowment_insurance(x, s=s+t, t=n-t, moment=2, 
                                             discrete=contract.discrete)
             A1 = self.endowment_insurance(x, s=s+t, t=n-t, 
                                             discrete=contract.discrete)
         else:
             raise Exception("Variance for WL or Endowment Ins only")
         return self.gross_variance_loss(A1=A1, A2=A2, contract=contract)
@@ -281,19 +289,19 @@
           contract : policy contract terms
         """
         contract = contract or Contract()
         if n < 0:    # Whole life shortcut
             A = self.whole_life_insurance(x, s=s+t, 
                                           discrete=contract.discrete)
         elif contract.endowment == contract.claims_cost:  # Endowment Ins shortcut
-            n = self.max_term(x+s+t, n)
+            n = self.max_term(x=x+s+t, t=n)
             A = self.endowment_insurance(x, s=s+t, t=n-t, 
                                             discrete=contract.discrete)
         else:  # Special term insurance
-            n = self.max_term(x+s+t, n)
+            n = self.max_term(x=x+s+t, t=n)
             A = self.term_insurance(x, s=s+t, t=n-t, discrete=contract.discrete)
             a = self.temporary_annuity(x, s=s+t, t=n-t,
                                        discrete=contract.discrete)
             endowment = 0
             if contract.endowment:  # endowment not equal to claims cost
                 endowment = self.E_x(x, s=s+t, t=n-t) * contract.endowment
             initial_cost = 0 if t else contract.initial_cost
@@ -302,86 +310,161 @@
         contract = contract.renewals(t) if t else contract # ignore initial if t>0
         return self.gross_future_loss(A=A, contract=contract)
 
     #
     # Future Loss random variable: L(T_x)
     #
     def L_from_t(self, t: float, contract: Contract | None = None) -> float:
-        """PV of Loss L(t) at time of death t = T_x (or K_x if discrete)
+        """PV of Loss L(t) at time of death t = T_x
 
         Args:
           t : year of death
           contract : policy contract
         """
-        contract = contract or Contract()
-        k = math.floor(t) if contract.discrete else t  # if endowment paid
-        if contract.T > 0 and k >= contract.T:
-            t = contract.T
-            endowment = contract.endowment * self.Z_from_t(t)
+        c = contract or Contract()
+        k = math.floor(t) if c.discrete else t
+        if c.T > 0 and k >= c.T:   # if endowment insurance and t is beyond term
+            t = c.T
+            endowment = c.endowment * self.Z_from_t(t)
         else:
             endowment = 0
-        return ((contract.claims_cost
-                 * self.Z_from_t(t, discrete=contract.discrete))
-                + contract.initial_cost
+        return ((c.claims_cost * self.Z_from_t(t, discrete=c.discrete))
                 + endowment
-                - (contract.renewal_profit
-                   * self.Y_from_t(t, discrete=contract.discrete)))
-
-    def L_to_t(self, L: float, contract: Contract | None = None) -> float:
-        """Compute time of death T_x s.t. PV future loss is L
-
-        Args:
-          L : PV of future loss
-          contract : policy contract terms and expenses
-        """
-        contract = contract or Contract()
-        return Contract.solve(lambda t: self.L_from_t(t, contract),
-                              target=L, grid=(0, self._MAXAGE), mad=True)
+                + c.initial_cost
+                - (c.renewal_profit * self.Y_from_t(t, discrete=c.discrete)))
 
     def L_from_prob(self, x: int, prob: float, 
                     contract: Contract | None = None) -> float:
-        """Compute PV of future loss at given percentile prob
+        """Percentile of PV future loss r.v. L given probability
 
         Args:
           x : age
           prob : probability threshold
           contract : policy contract
         """
+        contract = contract or Contract()
         t = self.Z_t(x, prob, discrete=contract.discrete)
         return self.L_from_t(t, contract)
 
+    def L_to_t(self, L: float, contract: Contract | None = None) -> float:
+        """Time of death T_x s.t. PV future loss is no more than L
+
+        Args:
+          L : PV of future loss
+          contract : policy contract terms and expenses
+        """
+        c = contract or Contract()
+        T = Contract.solve(lambda t: self.L_from_t(t, c),
+                           target=L,
+                           grid=(0, self._MAXAGE),
+                           mad=True)
+        if not c.discrete:
+            return T
+        return math.floor(T) if self.L_from_t(t=T, contract=c) <= L else math.ceil(T)
+
     def L_to_prob(self, x: int, L: float,
                   contract: Contract = Contract()) -> float:
-        """Compute percentile of L on the PV of future loss curve"
+        """Probability such that PV of future loss r.v. is no more than L"
 
         Args:
           x : age selected
           L : PV of future loss
           contract : policy contract terms and expenses
         """
         t = self.L_to_t(L, contract)
         return self.S(x, 0, t)
 
-    def L_plot(self, x: int, s: int = 0, stop: int = 0,
+    def L_plot(self,
+               x: int,
+               s: int = 0,
+               stop: int = 0,
                T: float | None = None,
-               contract: Contract = Contract(),
+               contract: Contract | None = None,
                ax: Any = None,
+               dual: bool = False,
                title: str | None = None,
-               color='r') -> float:
+               color: str = 'r',
+               alpha: float = 0.3)-> float | None:
+        """Plot PV of future loss r.v. L vs time of death T_x
+        
+        Args:
+          x : age selected
+          s : years after selection
+          stop : time to end plot
+          contract : policy contract terms and expenses
+          T : point in time to indicate probability and loss values
+          ax : figure object to plot in
+          title : title of plot 
+          dual: whether to plot survival function on secondary axis
+          color : color to plot curve
+          alpha : transparency of plot area
+        """
+        contract = contract or Contract()
+        if ax is None:
+            fig, ax = plt.subplots(1, 1)
+        K = 'K' if contract.discrete else 'T'
+        stop = stop or self._MAXAGE - (x + s)
+        step = 1 if contract.discrete else stop / 1000.
+        steps = np.arange(0, stop + step, step)
+
+        # plot PV loss values
+        y = [self.L_from_t(t, contract=contract) for t in steps]
+        ax.bar(steps, y, width=step, alpha=alpha, color=color)
+        ax.tick_params(axis='y', colors=color)
+        #ax.plot(steps, y, '.', c=color)
+        xmin, xmax = ax.get_xlim()
+        ymin, ymax = ax.get_ylim()
+        yjig = (ymax - ymin) / 50
+        xjig = (xmax - xmin) / 50
+
+        if dual:
+            p = [self.p_x(x=x, s=s, t=t) for t in steps]
+            bx = ax.twinx()
+            bx.step(steps, p, '-', c='g', alpha=alpha,
+                    where='pre' if contract.discrete else 'post')
+            #bx.bar(steps, p, color='g', alpha=.2, width=step, align='edge')
+            bx.set_ylabel(f"$S({K})$", color='g')
+            bx.tick_params(axis='y', colors='g')
+
+        if T is not None:
+            # plot indicate(T*)
+            z = self.L_from_t(T, contract=contract)
+            label1, = ax.plot(T, z, c=color, marker='o', label=f"L({T:.2f})={z:.4f}")
+            ax.legend(handles=[label1], loc='lower left')
+
+            # indicate corresponding S(T*)
+            if dual:
+                prob = self.S(x, s, T)
+                label2, = bx.plot(T, prob, c='g', marker='o',
+                                  label=f"Pr[{K}>{T:.2f}]={prob:.4f}")
+                bx.legend(handles=[label2], loc='upper right')
+        ax.set_title(f"PV future loss at issue r.v. $_0L$")
+        ax.set_ylabel(f"$L({K}_x)$", color=color)
+        ax.set_xlabel(f"${K}_x$")
+        #plt.tight_layout()
+        return z
+
+    def _L_plot(self, x: int, s: int = 0, stop: int = 0,
+                T: float | None = None,
+                contract: Contract | None = None,
+                ax: Any = None,
+                title: str | None = None,
+                color='r') -> float:
         """Plot PV of future loss r.v. L vs time of death T_x
         
         Args:
           x : age selected
           s : years after selection
           stop : time to end plot
           contract : policy contract terms and expenses
           T : point in time to indicate probability and loss values
           title : title of plot 
           color : color to plot curve
-        """        
+        """
+        contract = contract or Contract()
         if ax is None:
             fig, ax = plt.subplots(1, 1)
         K = 'K' if contract.discrete else 'T'
         stop = stop or self._MAXAGE - (x + s)
         step = 1 if contract.discrete else stop / 1000.
         steps = np.arange(0, stop + step, step)
 
@@ -440,16 +523,15 @@
     contract = Contract(premium=0.06, discrete=False)     # Solve second insurance
     variance = life.gross_variance_loss(A1=A1, A2=A2, contract=contract)
     print(variance)
     print()
 
     print("SOA Question 6.30:  (A) 900")
     life = PolicyValues().set_interest(i=0.04)
-    contract = Contract(premium=2.338, benefit=100, initial_premium=.1,
-                        renewal_premium=0.05)
+    contract = Contract(premium=2.338, benefit=100, initial_premium=.1, renewal_premium=0.05)
     var = life.gross_variance_loss(A1=life.insurance_twin(16.50),
                                    A2=0.17, contract=contract)
     print(var)
     print()
 
     print("SOA Question 7.32:  (B) 1.4")
     life = PolicyValues().set_interest(i=0.06)
```

### Comparing `actuarialmath-0.0.9/src/actuarialmath/premiums.py` & `actuarialmath-0.1.1/src/actuarialmath/premiums.py`

 * *Files 11% similar despite different names*

```diff
@@ -23,16 +23,22 @@
           u : years of deferral
           n : number of years of premiums paid
           t : year of death
           b : benefit amount
           endowment : endowment amount
           initial_cost : EPV of any other expenses or benefits, if any
           return_premium : if premiums without interest refunded at death 
-          annuity : whether benefit is insurance (False) or deferred annuity
+          annuity : whether benefit is insurance (False) or annuity
           discrete : whether annuity due (True) or continuous (False)
+
+        Examples:
+          >>> life = Premiums().set_interest(delta=0.06)\
+          >>>                  .set_survival(mu=lambda x,s: 0.04)
+          >>> life.net_premium(x=0)
+
         """
         if annuity:
             A = self.deferred_annuity(x, s=s, b=b, t=t, u=u, 
                                       discrete=discrete or discrete is None)
         else:
             A = self.deferred_insurance(x, s=s, b=b, t=t, u=u, 
                                         discrete=discrete or discrete is None)
@@ -56,14 +62,18 @@
         Args:
           premium : level net premium amount
           b : benefit amount
           discrete : discrete/annuity due (True) or continuous (False)
 
         Returns:
           Insurance factor value, given net premium under equivalence principle
+
+        Examples:
+          >>> life = Premiums().set_interest(d=0.05)
+          >>> life.insurance_equivalence(premium=2143, b=100000)
         """
         d = self.interest.d if discrete else self.interest.delta
         return premium / (d*b + premium)  # from P = b[dA/(1-A)]
 
     def annuity_equivalence(self, premium: float, b: int = 1,
                             discrete: bool = True) -> float:
         """Compute whole life or temporary annuity factor, given net premium
@@ -71,19 +81,24 @@
         Args:
           premium : level net premium amount
           b : benefit amount
           discrete : discrete/annuity due (True) or continuous (False)
 
         Returns:
           Annuity factor value, given net premium under equivalence principle
+
+        Examples:
+          >>> life = Premiums().set_interest(d=0.05)
+          >>> a = life.annuity_equivalence(premium=2143, b=100000)
         """
         d = self.interest.d if discrete else self.interest.delta
         return b / (d*b + premium)  # from P = b * (1/a - d)
 
-    def premium_equivalence(self, A: float | None = None,
+    def premium_equivalence(self,
+                            A: float | None = None,
                             a: float | None = None,
                             b: int = 1, discrete: bool = True) -> float:
         """Compute premium from whole life or endowment insurance and annuity factors
 
         Args:
           A : insurance factor
           a : annuity factor
@@ -100,15 +115,16 @@
             return b * (1/a - interest)
         else:           # Both (special) insurance and annuity factors given
             return b * A / a
 
     #
     # Gross premiums for special insurances
     #
-    def gross_premium(self, a: float | None = None, 
+    def gross_premium(self,
+                      a: float | None = None, 
                       A: float | None = None, IA: float = 0, 
                       discrete: bool = True, benefit: float = 1,
                       E: float = 0, endowment: int = 0, 
                       settlement_policy: float = 0.,
                       initial_policy: float = 0.,
                       initial_premium: float = 0.,
                       renewal_policy: float = 0., 
@@ -124,14 +140,24 @@
           endowment : endowment benefit amount
           settlement_policy : settlement expense per policy
           initial_policy : initial expense per policy
           renewal_policy : renewal expense per policy
           initial_premium : initial premium per $ of gross premium
           renewal_premium : renewal premium per $ of gross premium
           discrete : annuity due (True) or continuous (False)
+
+        Examples:
+          >>> Premiums().gross_premium(a=0.17094,
+          >>>                          A=6.8865,
+          >>>                          IA= 0.96728,
+          >>>                          benefit=100000,
+          >>>                          initial_premium=0.5,
+          >>>                          renewal_premium=.05,
+          >>>                          renewal_policy=200,
+          >>>                          initial_policy=200)
         """
         if a is None:    # assume WL or Endowment Insurance for twin
             a = self.annuity_twin(A, discrete=discrete)
         elif A is None:  # assume WL or Endowment Insurance for twin
              A = self.insurance_twin(a, discrete=discrete)
 
         assert endowment == 0 or E > 0  # missing pure endowment factor if needed
@@ -175,17 +201,17 @@
     A = life.insurance_equivalence(premium=2143, b=100000)
     a = life.annuity_equivalence(premium=2143, b=100000)
     p = life.gross_premium(A=A,
                            a=a,
                            benefit=100000,
                            settlement_policy=0,
                            initial_policy=250,
-                           initial_premium=.04+.35,
+                           initial_premium=0.04 + 0.35,
                            renewal_policy=50,
-                           renewal_premium=.04+.02) 
+                           renewal_premium=0.04 + 0.02) 
     print(A, a, p)
     print()
 
     print("SOA Question 6.20:  (B) 459")
     l = lambda x,s: dict(zip([75, 76, 77, 78],
                              np.cumprod([1, .9, .88, .85]))).get(x+s, 0)
     life = Premiums().set_interest(i=0.04).set_survival(l=l)
```

### Comparing `actuarialmath-0.0.9/src/actuarialmath/recursion.py` & `actuarialmath-0.1.1/src/actuarialmath/recursion.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,667 +1,1112 @@
 """Recursion - Applies recursion, shortcut and actuarial formulas
 
 MIT License. Copyright 2022-2023 Terence Lim
 """
-from typing import Tuple
+from typing import Tuple, Any
+import matplotlib.pyplot as plt
 from actuarialmath import Reserves
+from IPython.display import display_latex, display_pretty
+from IPython import get_ipython
+
+_depth = 3
+
+class _Blog:
+    """Helper to track and display recursion steps"""
+    _notebook: bool = False
+    _latex: bool = False
+
+    def __init__(self, label, *args, levels: int = _depth, verbose: bool = True,
+                 width: int = 80):
+        self.title = f" *{label} {' '.join(args)} :="    # to identify this stack
+        self.levels = levels                             # maximum levels to indent
+        self.width = width                               # line width of display
+        self.verbose = verbose
+        self._history = []
+        self._rules = []
+        self._depths = []
+
+    def __call__(self, *args, depth: int | None = None, rule: str = ''):
+        """Append next message to history"""
+        assert depth is not None and rule, "depth and rule must be specified"
+        msg = " ".join([a for a in args]) 
+        if msg not in self._history:
+        #if True:
+            self._history.insert(0, msg)
+            self._depths.insert(0, depth)
+            self._rules.insert(0, rule)
+
+    def pop(self, depth: int):
+        #"""
+        _last = 0
+        while (_last < len(self._depths) - 1 and
+               depth > self._depths[_last] and
+               self._depths[_last] >= self._depths[_last+1]):
+            _last = _last + 1
+        self._history = self._history[_last:]
+        self._depths = self._depths[_last:]
+        self._rules = self._rules[_last:]
+        #"""
+        #pass
+
+    def __len__(self) -> int:
+        return int(self.verbose and bool(self._history))
+
+    def __str__(self) -> str:
+        """Display message history"""
+        newline = '\n'
+        if not len(self):
+            return ''
+        _str = self.title + newline
+        for msg, depth, rule in zip(self._history, self._depths, self._rules):
+            left = ' '*(3+max(self.levels-abs(depth), 0))
+            right = ' '*max(5, self.width - len(msg) - len(left) - len(rule))
+            _str += left + msg + right + '~' + rule + newline
+        return _str
+
+    def display(self, end='\n'):
+        _str = str(self)
+        if _str:
+            if _Blog._notebook and _Blog._latex:
+                display_latex(_str, raw=True)
+            elif _Blog._notebook:
+                display_pretty(_self, raw=True)
+            else:
+                print(_str, end=end)
+            
+
+    @staticmethod
+    def q(x: int, s: int = 0, t: int = 1, u: int = 0) -> str:
+        """Return string representation of mortality u|t_q_x term"""
+        if t == 0:
+            return "0"
+        if t < 0:
+            return "1"
+        out = []
+        if t != 1:
+            out.append(f"t={t}")
+        if u > 0:
+            out.append(f"defer={u}")
+        return f"q_{x+s}" + "("*bool(out) + ",".join(out) + ")"*bool(out)
+
+    @staticmethod
+    def p(x: int, s: int = 0, t: int = 1) -> str:
+        """Return string representation of survival t_p_x term"""
+        if t == 0:
+            return "1"
+        if t < 0:
+            return "0"
+        out = []
+        if t != 1:
+            out.append(f"t={t}")
+        return f"p_{x+s}" + "("*bool(out) + ",".join(out) + ")"*bool(out)
+
+
+    @staticmethod
+    def e(x: int, s: int = 0, t: int = Reserves.WHOLE, curtate: bool = False,
+          moment: int = 1) -> str:
+        """Return string representation of expected future lifetime t_e_[x+s] term"""
+        out = []
+        if t >= 0:
+            out.append(f"t={t}")
+        if moment != 1:
+            out.append(f"mom={moment}")
+        out.append('curtate' if curtate else 'complete')
+        return f"e_{x+s}" + "("*bool(out) + ",".join(out) + ")"*bool(out)
+
+    @staticmethod
+    def E(x: int, s: int = 0, t: int = 1, endowment: int = 1,
+          moment: int = 1) -> str:
+        """Return string representation of pure endowment t_E_[x+s] term"""
+        out = []
+        out.append(f"t={t if t >= 0 else 'WL'}")  # term or whole life
+        if moment != 1:
+            out.append(f"mom={moment}")
+        if endowment != 1:
+            out.append(f"endow={endowment}")
+        return f"E_{x+s}" + "("*bool(out) + ",".join(out) + ")"*bool(out)
+    
+    @staticmethod
+    def IA(x: int, s: int = 0, t: int = Reserves.WHOLE, b: int = 1,
+           discrete: bool = True) -> str:
+        """Return string representation of increasing insurance IA_[x+s]:t term"""
+        out = []
+        out.append(f"t={t if t >= 0 else 'WL'}")  # term or whole life
+        if b != 1:
+            out.append(f"b={b}")
+        return f"IA_{x+s}" + "("*bool(out) + ",".join(out) + ")"*bool(out)
+
+    @staticmethod
+    def DA(x: int, s: int = 0, t: int = Reserves.WHOLE, b: int = 1,
+           discrete: bool = True) -> str:
+        """Return string representation of decreasing insurance DA_[x+s]:t term"""
+        out = []
+        out.append(f"t={t if t >= 0 else 'WL'}")  # term or whole life
+        if b != 1:
+            out.append(f"b={b}")
+        return f"DA_{x+s}" + "("*bool(out) + ",".join(out) + ")"*bool(out)
+
+    @staticmethod
+    def A(x: int, s: int = 0, t: int = Reserves.WHOLE, u: int = 0, b: int = 1,
+          moment: int = 1, endowment: int = 0, discrete: bool = True) -> str:
+        """Return string representation of insurance u|_A_[x+s]:t term"""
+        out = []
+        out.append(f"t={t if t >= 0 else 'WL'}")  # term or whole life
+        if u != 0:
+            out.append(f"u={u}")
+        if b != 1:
+            out.append(f"b={b}")
+        if endowment != 0:
+            out.append(f"endow={endowment}")
+        if moment != 1:
+            out.append(f"mom={moment}")
+        return f"A_{x+s}" + "("*bool(out) + ",".join(out) + ")"*bool(out)
+
+    @staticmethod
+    def a(x: int, s: int = 0, t: int = Reserves.WHOLE, u: int = 0, b: int = 1,
+          variance: bool = False, discrete: bool = True) -> str:
+        """Return string representation of annuity u|_a_[x+s]:t term"""
+        out = []
+        out.append(f"t={t if t >= 0 else 'WL'}")  # term or whole life
+        if u != 0:
+            out.append(f"u={u}")
+        if b != 1:
+            out.append(f"b={b}")
+        if variance:
+            out.append('var')
+        return f"a_{x+s}" + "("*bool(out) + ",".join(out) + ")"*bool(out)
+
+    @staticmethod
+    def m(moment: int, **kwargs) -> str:
+        """Return string representation of moment exponent"""
+        out = f"^{moment}"*(moment != 1)
+        if not kwargs:
+            return out
+        args = [k for k,v in kwargs.items() if v]
+        if len(args) > 1:
+            return ("(" + "*".join(args) + ")")
+        else:
+            return args[0] + out if len(args) else "0"
+
+class PPrint(_Blog):
+    """Helper to display recursion steps as actuarial notation in latex format"""
+
+    def __init__(self, label: str, *args, **kwargs):
+        super().__init__(label, *args, **kwargs)
+        self.title = f"~\\texttt{{{label}}}{'~'.join(args)}~:=" # identify this stack
+
+    def __str__(self) -> str:
+        if len(self):
+            beg = "\\begin{array}{llll}\n"
+            end = "\\end{array}"
+            lines = [self.title]
+            for msg, depth, rule in zip(self._history, self._depths, self._rules):
+                left = '~~' * (1 + max(self.levels-abs(depth), 0))
+                line = left + msg + '& \\quad \\texttt{' + rule + '}'
+                lines.append(line) #.replace("=", "& ="))
+            s = beg + "\\\\\n".join(lines) + end
+            return s
+        return ""
+
+    @staticmethod
+    def q(x: int, s: int = 0, t: int = 1, u: int = 0) -> str:
+        """Return latex string representation of mortality u|t_q_[x+s] term"""
+        if t == 0:
+            return "~0"
+        if t < 0:
+            return "~1"
+        left = '~'
+        if t != 1 or u > 0:
+            left += "_{{"
+            if u > 0:
+                left += f"{u}|"
+            if t != 1:
+                left += f"{t}"
+            left += "}}"
+        right = f"x+{x+s}" if x + s > 0 else "x"
+        return f"{left}q_{{{right}}}"
+
+    @staticmethod
+    def p(x: int, s: int = 0, t: int = 1) -> str:
+        """Return latex string representation of survival t_p_[x+s] term"""
+        if t == 0:
+            return "~1"
+        if t < 0:
+            return "~0"
+        left = '~'
+        if t != 1:
+            left += f"_{{{t}}}"
+        right = f"x+{x+s}" if x + s > 0 else "x"
+        return f"{left}p_{{{right}}}"
+
+
+    @staticmethod
+    def e(x: int, s: int = 0, t: int = Reserves.WHOLE, curtate: bool = False,
+          moment: int = 1) -> str:
+        """Return string representation of expected future lifetime e_[x+s]:t term"""
+        out = "e" if curtate else "\\overset{{\\circ}}{{e}}"
+        right = f"x+{x+s}" if x + s > 0 else "x"    
+        right += f":\\overline{{{t}|}}" if t >= 0 else ""
+        out += "_{{" + right + "}}"
+        if moment < 0:
+            out = f"Var[{out}]"
+        if moment > 1:
+            out = f"E[{out}^{{{moment}}}]"
+        return "~" + out
+
+    @staticmethod
+    def E(x: int, s: int = 0, t: int = 1, endowment: int = 1,
+          moment: int = 1) -> str:
+        """Return latex string representation of pure endowment t_E_[x+s]:t term"""
+        left = '~'
+        if t != 1:
+            left += f"_{{{t}}}"
+        right = f"x+{x+s}" if x + s > 0 else "x"
+        return f"{left}E_{{{right}}}"
+    
+    @staticmethod
+    def IA(x: int, s: int = 0, t: int = Reserves.WHOLE, b: int = 1,
+           discrete: bool = True) -> str:
+        """Return latex string representation of increasing insurance IA_[x+s]:t term"""
+        out = "(IA)"
+        right = f"x+{x+s}" if x + s > 0 else "x"    
+        right += f":\\overline{{{t}|}}" if t >= 0 else ""
+        out += "_{{" + right + "}}"
+        return "~" + out + f"* {b}"*(b != 1)
+
+    @staticmethod
+    def DA(x: int, s: int = 0, t: int = Reserves.WHOLE, b: int = 1,
+           discrete: bool = True) -> str:
+        """Return latex string representation of decreasing insurance DA_[x+s]:t term"""
+        out = "(DA)"
+        right = f"x+{x+s}" if x + s > 0 else "x"    
+        right += f":\\overline{{{t}|}}" if t >= 0 else ""
+        out += "_{{" + right + "}}"
+        return "~" + out + f"* {b}"*(b != 1)
+
+    @staticmethod
+    def A(x: int, s: int = 0, t: int = Reserves.WHOLE, u: int = 0, b: int = 1,
+          moment: int = 1, endowment: int = 0, discrete: bool = True) -> str:
+        """Return latex string representation of insurance u|_A_[x+s]:t term"""
+        out = "A" if discrete else "\\overline{{A}}"
+        if moment > 1:
+            out = f"^{moment}" + out
+        if u > 0:
+            out = f"_{{{u}|}}" + out
+        if endowment == 0 and t >= 0:
+            out += "^1"
+        right = f"x+{x+s}" if x + s > 0 else "x"    
+        right += f":\\overline{{{t}|}}" if t >= 0 else ""
+        out += "_{{" + right + "}}"
+        return "~" + out + f"* {b}"*(b != 1)
+
+
+    @staticmethod
+    def a(x: int, s: int = 0, t: int = Reserves.WHOLE, u: int = 0, b: int = 1,
+          variance: bool = False, discrete: bool = True) -> str:
+        """Return latex string representation of annuity u|_a_[x+s]:t term"""
+        out = f"\\ddot{{a}}" if discrete else "a"
+        if u > 0:
+            out = f"_{{{u}|}}" + out
+        right = f"x+{x+s}" if x + s > 0 else "x"    
+        right += f":\\overline{{{t}|}}" if t >= 0 else ""
+        out += "_{{" + right + "}}"
+        out += f"* {b}"*(b != 1)
+        if variance:
+            out = f"Var[{out}]"
+        return "~" + out
+    
+    @staticmethod
+    def m(moment: int, **kwargs) -> str:
+        """Return latex string representation of moment exponent"""
+        out = f"^{{{moment}}}"*(moment != 1)
+        if not kwargs:
+            return out
+        args = [k for k,v in kwargs.items() if v]
+        if len(args) > 1:
+            return ("\\left(" + "*".join(args) + "\\right)")
+        else:
+            return args[0] + out if len(args) else "0"
+    
 
 class Recursion(Reserves):
     """Solve by appling recursive, shortcut and actuarial formulas repeatedly
 
     Args:
       depth : maximum depth of recursions (default is 3)
       verbose : whether to echo recursion steps (True, default)
 
     Notes:
-      7 types of information can be loaded and calculated in recursions:
+      7 types of function values can be loaded for recursion computations:
 
       - 'q' : (deferred) probability (x) dies in t years
       - 'p' : probability (x) survives t years
-      - 'e' : (temporary) expected future lifetime, and moments
-      - 'A' : deferred, term, endowment or whole life insurance, and moments
+      - 'e' : (temporary) expected future lifetime, or moments
+      - 'A' : deferred, term, endowment or whole life insurance, or moments
       - 'IA' : decreasing life insurance of t years
       - 'DA' : increasing life insurance of t years
-      - 'a' : deferred, temporary or whole life annuity of t years, and moments
+      - 'a' : deferred, temporary or whole life annuity of t years, or moments
     """
-
-    def __init__(self, depth: int = 5, verbose: bool = True, **kwargs):
+    
+    _Blog = _Blog
+    def __init__(self, depth: int = _depth, verbose: bool = True, **kwargs):
         super().__init__(**kwargs)
         self.db = {}
+        self._t = {'A': {1, 2}, 'a': {1, 2}, 'e': {1, 2}}  # recursion periods to try
         self.maxdepth = depth
-        _Blog._verbose = verbose
+        self._verbose = verbose
+        self.pprint = Recursion._Blog
+
+    def Blog(self, *args, **kwargs):
+        """Returns Blog instance to collect messages and display for this query"""
+        return Recursion._Blog(*args, **kwargs, verbose=self._verbose)
+
+    @staticmethod
+    def blog_options(latex: bool = False, notebook: bool = False):
+        """Static method to change display options for tracing the recursion steps
+
+        Args:
+          latex: display actuarial notation in latex (True) or raw text (False)
+          notebook: display to jupyter or colab notebook (True) or terminal (False)
 
+        Notes:
+          latex and notebook options are set to True if notebook is auto-detected 
+
+        Examples:
+
+        >>> Recursion.blog_options(latex=False)                # display as raw text
+        >>> Recursion.blog_options(latex=True, notebook=True)  # display latex format
+        """
+        _Blog._notebook = notebook
+        _Blog._latex = latex
+        Recursion._Blog = PPrint if latex else _Blog
+        
     #
     # helpers to store given input values
     #
-    def db_key(self, *args, **kwargs) -> Tuple:
+    def _db_key(self, *args, **kwargs) -> Tuple:
         """Generate a unique key representing values of given arguments"""
         assert args and kwargs
         return tuple(list(args) + sorted(kwargs.items()))
 
-    def db_put(self, key: Tuple, value: float | None) -> "Recursion":
+    def _db_put(self, key: Tuple, value: float | None) -> "Recursion":
         """Store the item's key and value; or remove if value is None
+
         Args:
           key : key of the item
           value : value to store for item
         """
         if value is None and key in self.db:
             self.db.pop(key)
         else:
             self.db[key] = value
+            label = key[0]
+            t = [v for k,v in key[1:] if k == 't' and v > 0]
+            if label in self._t:
+                self._t[label] = self._t[label].union(t)
         return self
 
-    def db_print(self):
+    def _db_print(self):
         """Display the stored keys and values"""
         for k in sorted(self.db.keys()):
             print(k, self.db[k])
 
     #
     # Formulas for Mortality: u|t_q_x
     #
-    def get_q(self, x: int, s: int = 0, t: int = 1,
-              u: int = 0) -> float | None:
+    def _get_q(self, x: int, s: int = 0, t: int = 1,
+               u: int = 0) -> float | None:
         """Get mortality rate from key-value store
 
         Args:
           x : age of selection
           s : years after selection
           u : survive u years, then...
           t : death within next t years        
         """
-        key = self.db_key('q', x=x+s, u=u, t=t)
+        key = self._db_key('q', x=x+s, u=u, t=t)
         return self.db.get(key, None)
 
     def set_q(self, val: float, x: int, s: int = 0, t: int = 1, 
               u: int = 0) -> "Recursion":
-        """Set mortality rate u|t_q_[x]+s to given value
+        """Set mortality rate u|t_q_[x+s] to given value
 
         Args:
           val : value to set
           x : age of selection
           s : years after selection
           u : survive u years, then...
           t : death within next t years        
+
+        Examples:
+          >>> Recursion(depth=3).set_q(0.02, x=3)
         """
-        return self.db_put(self.db_key('q', x=x+s, u=u, t=t), val)
+        return self._db_put(self._db_key('q', x=x+s, u=u, t=t), val)
 
     def _q_x(self, x: int, s: int = 0, t: int = 1, u: int = 0, 
              depth: int = 1) -> float:
         """Helper to compute mortality from recursive and alternate formulas"""
-        found = self.get_q(x, s=s, t=t, u=u)
+        found = self._get_q(x, s=s, t=t, u=u)
         if found is not None:
             return found
         if t == 0:
             return 0
         if t < 0:
             return 1
         if u > 0:
             pu = self._p_x(x, s=s, t=u, depth=depth-1) #depth-1)
-            qt = self.get_q(x, s=s+u, t=t)
+            qt = self._get_q(x, s=s+u, t=t)
             if pu is not None and qt is not None:
-                self.blog(_Blog.q(x=x, s=s, t=t, u=u), '=',
-                          _Blog.p(x=x, s=s, t=u), '*', _Blog.q(x=x, s=s+u, t=t),
+                self.blog(self.pprint.q(x=x, s=s, t=t, u=u), '=',
+                          self.pprint.p(x=x, s=s, t=u), '*',
+                          self.pprint.q(x=x, s=s+u, t=t),
                           depth=depth, rule="defer mortality")
                 return pu * qt        # (1) u_p_x * t_q_x+u
-            qu = self.get_q(x, s=s, t=u)
-            qt = self.get_q(x, s=s, t=u+t)
+            else:
+                self.blog.pop(depth=depth)
+            qu = self._get_q(x, s=s, t=u)
+            qt = self._get_q(x, s=s, t=u+t)
             if qu is not None and qt is not None:
-                self.blog(_Blog.q(x=x, s=s, t=t, u=u), '=',
-                          _Blog.q(x=x, s=s, t=t+u), '-', _Blog.q(x=x, s=s, t=u),
+                self.blog(self.pprint.q(x=x, s=s, t=t, u=u), '=',
+                          self.pprint.q(x=x, s=s, t=t+u), '-',
+                          self.pprint.q(x=x, s=s, t=u),
                           depth=depth, rule="limit mortality")
                 return qt - qu        # (2) u+t_q_x - u_q_x
+            else:
+                self.blog.pop(depth=depth)
         if depth <= 0:
             return None
         pu = self._p_x(x, s=s, t=u, depth=depth-1)
         pt = self._p_x(x, s=s, t=u+t, depth=depth-1)
         if pu is not None and pt is not None:
-            self.blog(_Blog.q(x=x, s=s, t=t, u=u), '=',
-                      _Blog.p(x=x, s=s, t=u), '-', _Blog.p(x=x, s=s, t=t+u),
+            self.blog(self.pprint.q(x=x, s=s, t=t, u=u), '=',
+                      self.pprint.p(x=x, s=s, t=u), '-',
+                      self.pprint.p(x=x, s=s, t=t+u),
                       depth=depth, rule="complement survival")
             return pu - pt            # (3) u_p_x - u+t_p_x
+        else:
+            self.blog.pop(depth=depth)
 
 
     def q_x(self, x: int, s: int = 0, t: int = 1, u: int = 0) -> float:
-        self.blog = _Blog("Mortality",
-                         _Blog.q(x=x, s=s, t=t, u=u),
-                         levels=self.maxdepth)
+        self.blog = self.Blog("Mortality",
+                              self.pprint.q(x=x, s=s, t=t, u=u),
+                              levels=self.maxdepth)
         """Compute mortality rate by calling recursion helper"""
         q = self._q_x(x, s=s, t=t, u=u, depth=self.maxdepth)
         if q is not None:
-            print(self.blog, end='')
+            self.blog.display()
         return q
 
     #
     # Formulas for Survival: t_p_x
     #
-    def get_p(self, x: int, s: int = 0, t: int = 1) -> float | None:
+    def _get_p(self, x: int, s: int = 0, t: int = 1) -> float | None:
         """Get survival probability from key-value store
 
         Args:
           x : age of selection
           s : years after selection
           t : survives next t years
         """
         if t == 0:
             return 1
         if t < 0:
             return 0
-        key = self.db_key('p', x=x+s, t=t)
+        key = self._db_key('p', x=x+s, t=t)
         return self.db.get(key, None)
 
     def set_p(self, val: float, x: int, s: int = 0, t: int = 1) -> "Recursion":
-        """Set survival probability t_p_[x]+s to given value
+        """Set survival probability t_p_[x+s] to given value
 
         Args:
           val : value to set
           x : age of selection
           s : years after selection
           t : survives next t years
+
+        Examples:
+          >>> Recursion(depth=3).set_p(0.99, x=0)\
         """
-        return self.db_put(self.db_key('p', x=x+s, t=t), val)
+        return self._db_put(self._db_key('p', x=x+s, t=t), val)
 
     def _p_x(self, x: int, s: int = 0, t: int = 1, depth: int = 1) -> float:
         """Helper to compute survival from recursive and alternate formulas"""
-        found = self.get_p(x, s=s, t=t)
+        found = self._get_p(x, s=s, t=t)
         if found is not None:
             return found
-        found = self.get_q(x, s=s, t=t)  
+        found = self._get_q(x, s=s, t=t)  
         if found is not None:
-            self.blog(_Blog.p(x=x, s=s, t=t), '= 1 -', _Blog.q(x=x, s=s, t=t),
+            self.blog(self.pprint.p(x=x, s=s, t=t), '= 1 -',
+                      self.pprint.q(x=x, s=s, t=t),
                       depth=depth, rule='complement of mortality')
             return 1 - found  # (1) complement of q_x
+        else:
+            self.blog.pop(depth=depth)
         if depth <= 0:
             return None
         
         # (2a) inverse chain rule: p_x(t) = p_x-1(t+1) / p_x-1 
         found = self._p_x(x, s=s-1, t=t+1, depth=depth-1)
         p = self._p_x(x, s=s-1, t=1, depth=depth-1)
         if found is not None and p is not None:
-            self.blog(_Blog.p(x=x, s=s, t=t), '=',
-                      _Blog.p(x=x, s=s-1, t=t+1), '/', _Blog.p(x=x, s=s-1, t=1),
+            self.blog(self.pprint.p(x=x, s=s, t=t), '=',
+                      self.pprint.p(x=x, s=s-1, t=t+1), '/',
+                      self.pprint.p(x=x, s=s-1, t=1),
                       depth=depth, rule="survival chain rule")
             return found / p
+        else:
+            self.blog.pop(depth=depth)
         
         # (2b) inverse chain rule: p_x(t) = p_x(t+1) / p_x+t 
         found = self._p_x(x, s=s, t=t+1, depth=depth-1)
         p = self._p_x(x, s=s+t, t=1, depth=depth-1)
         if found is not None and p is not None:
-            self.blog(_Blog.p(x=x, s=s, t=t), '=',
-                      _Blog.p(x=x, s=s, t=t+1), '/', _Blog.p(x=x, s=s+t, t=1),
+            self.blog(self.pprint.p(x=x, s=s, t=t), '=',
+                      self.pprint.p(x=x, s=s, t=t+1), '/',
+                      self.pprint.p(x=x, s=s+t, t=1),
                       depth=depth, rule="survival chain rule")
             return found / p
+        else:
+            self.blog.pop(depth=depth)
+        
         if t > 1:
             # (3a) chain rule: p_x(t) = p_x * p_x+1(t-1)
             found = self._p_x(x, s=s+1, t=t-1, depth=depth-1)
             p = self._p_x(x, s=s, t=1, depth=depth-1)
             if found is not None and p is not None:
-                self.blog(_Blog.p(x=x, s=s, t=t), '=',
-                          _Blog.p(x=x, s=s+1, t=t-1), '*', _Blog.p(x=x, s=s, t=1),
+                self.blog(self.pprint.p(x=x, s=s, t=t), '=',
+                          self.pprint.p(x=x, s=s+1, t=t-1), '*',
+                          self.pprint.p(x=x, s=s, t=1),
                           depth=depth, rule="survival chain rule")
                 return found * p
+            else:
+                self.blog.pop(depth=depth)
 
             # (3b) chain rule: p_x(t) = p_x+t-1 * p_x(t-1)
             found = self._p_x(x, s=s, t=t-1, depth=depth-1)
             p = self._p_x(x, s=s+t-1, t=1, depth=depth-1)
             if found is not None and p is not None:
-                self.blog(_Blog.p(x=x, s=s, t=t), '=',
-                          _Blog.p(x=x, s=s, t=t-1), '*', _Blog.p(x=x, s=s+t-1, t=1),
+                self.blog(self.pprint.p(x=x, s=s, t=t), '=',
+                          self.pprint.p(x=x, s=s, t=t-1), '*',
+                          self.pprint.p(x=x, s=s+t-1, t=1),
                           depth=depth, rule="survival chain rule")
                 return found * p
+            else:
+                self.blog.pop(depth=depth)
 
         if t == 1:
             E = self._E_x(x, s=s, t=1, depth=depth-1)
             if E is not None:
-                self.blog(_Blog.p(x=x, s=s, t=1), '=',
-                          _Blog.E(x=x, s=s, t=1), "/v",
-                          depth=depth, rule="one-year endowment")
+                self.blog(self.pprint.p(x=x, s=s, t=1), '=',
+                          self.pprint.E(x=x, s=s, t=1), "/v",
+                          depth=depth, rule="one-year pure endowment")
                 return E / self.interest.v
+            else:
+                self.blog.pop(depth=depth)
 
-            # (4a) annuity recursion: p_x = [a_x(t) - 1] / [v a_x+1(t-1)
-            for _t in [self.WHOLE, 2, 3]:  # consider only WL and 2-term
+            for _t in [self.WHOLE, 2, 3, 4]:  # consider only WL, 2-, 3- and 4-term
+                
+                # (4a) annuity recursion: p_x = [a_x(t) - 1] / [v a_x+1(t-1)
                 a = self._a_x(x, s=s, t=_t, depth=depth-1)
                 a1 = self._a_x(x, s=s+1, t=self.add_term(_t, -1), depth=depth-1)
                 if a is not None and a1 is not None:
-                    self.blog(_Blog.p(x=x, s=s, t=1), '= [',
-                              _Blog.a(x=x, s=s, t=_t), '- 1 ] / [ v *',
-                              _Blog.a(x=x, s=s+1, t=_t-1), ']',
+                    self.blog(self.pprint.p(x=x, s=s, t=1), '= [',
+                              self.pprint.a(x=x, s=s, t=_t), '- 1 ] / [ v *',
+                              self.pprint.a(x=x, s=s+1, t=_t-1), ']',
                               depth=depth, rule="annuity recursion")
                     return (a - 1) / (self.interest.v * a1)
+                else:
+                    self.blog.pop(depth=depth)
 
             
-            # (4b) insurance recursion: p_x = [v - A_x(t)] / [v (1 - A_x+1(t-1))]
-            for _t in [self.WHOLE, 2, 3]:  # consider only WL and 2-term
-                A = self._A_x(x, s=s, t=_t, depth=depth-1)
-                A1 = self._A_x(x, s=s+1, t=self.add_term(_t, -1), depth=depth-1)
-                if A is not None and A1 is not None:
-                    self.blog(_Blog.p(x=x, s=s, t=1), '= [ v -',
-                              _Blog.A(x=x, s=s, t=_t), '] / [v * [ 1 -',
-                              _Blog.A(x=x, s=s+1, t=_t-1), ']]',
-                              depth=depth, rule="insurance recursion")
-                    return (self.interest.v - A)/(self.interest.v * (1 - A1))
+                # (4b) insurance recursion: p_x = [v - A_x(t)] / [v (1 - A_x+1(t-1))]
+                for endowment in [0, 1]:
+                    A = self._A_x(x, s=s, t=_t, endowment=endowment, depth=depth-1)
+                    A1 = self._A_x(x, s=s+1, t=self.add_term(_t, -1), endowment=endowment,
+                                   depth=depth-1)
+                    if A is not None and A1 is not None:
+                        self.blog(self.pprint.p(x=x, s=s, t=1), '= [ v -',
+                                  self.pprint.A(x=x, s=s, t=_t, endowment=endowment),
+                                  '] / [v * [ 1 -',
+                                  self.pprint.A(x=x, s=s+1, t=_t-1, endowment=endowment),
+                                  ']]',
+                                  depth=depth, rule="insurance recursion")
+                        return (self.interest.v - A)/(self.interest.v * (1 - A1))
+                    else:
+                        self.blog.pop(depth=depth)
 
     def p_x(self, x: int, s: int = 0, t: int = 1) -> float:
         """Compute survival probability by calling recursion helper
 
         Args:
           x : age of selection
           s : years after selection
           t : survives at least t years
         """
-        self.blog = _Blog("Survival",
-                         _Blog.p(x=x, s=s, t=t),
-                         levels=self.maxdepth)
+        self.blog = self.Blog("Survival",
+                              self.pprint.p(x=x, s=s, t=t),
+                              levels=self.maxdepth)
         p = self._p_x(x, s=s, t=t, depth=self.maxdepth)
         if p is not None:
-            print(self.blog, end='')
+            self.blog.display()
         return p
 
     #
     # Formulas for Expected Future Lifetime: e_x
     #
-    def get_e(self, x: int, s: int = 0, t: int = Reserves.WHOLE, 
-              curtate: bool = False, moment: int = 1) -> float | None:
+    def _get_e(self, x: int, s: int = 0, t: int = Reserves.WHOLE, 
+               curtate: bool = False, moment: int = 1) -> float | None:
         """Get expected future lifetime from key-value store
 
         Args:
           x : age of selection
           s : years after selection
           t : limit of expected future lifetime
           curtate : curtate (True) or complete expectation (False)
           moment : first or second moment of expected future lifetime
         """
-        key = self.db_key('e', x=x+s, t=t, curtate=curtate, moment=moment)
+        key = self._db_key('e', x=x+s, t=t, curtate=curtate, moment=moment)
         return self.db.get(key, None)
 
     def set_e(self, val: float, x: int, s: int = 0, t: int = Reserves.WHOLE, 
               curtate: bool = False, moment: int = 1) -> "Recursion":
-        """Set expected future lifetime e_[x]+s:t to given value
+        """Set expected future lifetime e_[x+s]:t to given value
 
         Args:
           val : value to set
           x : age of selection
           s : years after selection
           t : limit of expected future lifetime
           curtate : curtate (True) or complete expectation (False)
           moment : first or second moment of expected future lifetime
         """
-        return self.db_put(self.db_key('e', x=x+s, t=t, moment=moment,
-                                       curtate=curtate), val)
+        return self._db_put(self._db_key('e', x=x+s, t=t, moment=moment,
+                                         curtate=curtate), val)
 
     def _e_x(self, x: int, s: int = 0, t: int = Reserves.WHOLE, 
             curtate: bool = False, moment: int = 1, 
             depth: int = 1) -> float | None:
         """Helper to compute from recursive and alternate formulas"""
-        found = self.get_e(x, s=s, t=t, curtate=curtate, moment=moment)
+        found = self._get_e(x, s=s, t=t, curtate=curtate, moment=moment)
         if found is not None:
             return found
         if depth <= 0:
             return None
         if moment == 1:
             if t > 0:  
                 p_t = self._p_x(x, s=s, t=t)
                 if t == 1 and curtate:
-                    self.blog(_Blog.e(x=x, s=s, t=1, curtate=curtate), '=',
-                              _Blog.p(x=x, s=s, t=1),
+                    self.blog(self.pprint.e(x=x, s=s, t=1, curtate=curtate), '=',
+                              self.pprint.p(x=x, s=s, t=1),
                               #f"e_{x+s}:1",
                               depth=depth, rule='1-year curtate shortcut')
                     return p_t   # (1) if curtate and t=1: e_x:1 = p_x 
+                else:
+                    self.blog.pop(depth=depth)
                 if t > 1:
                     e = self._e_x(x, s=s, t=Reserves.WHOLE, curtate=curtate, 
                                   moment=1, depth=depth-1)
                     e_t = self._e_x(x, s=s+t, t=Reserves.WHOLE, curtate=curtate,
                                     moment=1, depth=depth-1)
                     if e is not None and e_t is not None and p_t is not None:
-                        self.blog(_Blog.e(x=x, s=s, t=t), '=', _Blog.e(x=x, s=s), '-',
-                                  _Blog.p(x=x, s=s), '*', _Blog.e(x=x, s=s+t),
+                        self.blog(self.pprint.e(x=x, s=s, t=t, curtate=curtate), '=',
+                                  self.pprint.e(x=x, s=s, curtate=curtate), '-',
+                                  self.pprint.p(x=x, s=s), '*',
+                                  self.pprint.e(x=x, s=s+t, curtate=curtate),
                                   #"e_{x+s}:{t}: e_x - p_x e_x+t",
                                   depth=depth, rule="temporary lifetime")
                         return e - p_t*e_t  # (2) temporary = e_x - t_p_x e_x+t
-            e = self._e_x(x, s=s-1, t=self.add_term(t, 1), curtate=curtate,
-                          moment=1, depth=depth-1)
-            e1 = self._e_x(x, s=s-1, t=1, curtate=curtate, moment=1,
-                          depth=depth-1)
-            p = self._p_x(x, s=s-1)
-            if e is not None and e1 is not None and p is not None:
-                #_t = "" if t < 0 else ":" + str(t)
-                #msg = f"forward e_{x+s}{_t} = e_{x+s}:1 + p_{x+s} e_{x+s+1}"
-                self.blog(_Blog.e(x=x, s=s, t=t), '=', _Blog.e(x=x, s=s, t=t), '+',
-                          _Blog.p(x=x, s=s), '*', _Blog.e(x=x, s=s+t),
-                          depth=depth, rule='lifetime forward recursion')
-                return (e - e1) / p # (3) forward: (e_x-1 - e_x-1:1) / p_x-1
-            e = self._e_x(x, s=s, t=1, curtate=curtate,
-                          moment=1, depth=depth-1)
-            e_t = self._e_x(x, s=s+1, t=self.add_term(t, -1), curtate=curtate,
-                            moment=1, depth=depth-1)
-            p = self._p_x(x, s=s)
-            if e is not None and e_t is not None and p is not None:
-                self.blog(_Blog.e(x=x, s=s, t=t), '=', _Blog.e(x=x ,s=s, t=1), '+',
-                          _Blog.p(x=x, s=s), '*', _Blog.e(x=x, s=s+1, t=t-1),
-                          #f"backward: e_x:1 + p_x e_x+1:{t}",
-                          depth=depth, rule='lifetime backward recursion')
-                return e + p * e_t # (4) backward: e_x:1 + p_x e_x+1:t-1
+                    else:
+                        self.blog.pop(depth=depth)
+
+            for u in range(1, 50):
+                e = self._e_x(x, s=s-u, t=self.add_term(t, u), curtate=curtate,
+                              moment=1, depth=depth-1)
+                e1 = self._e_x(x, s=s-u, t=u, curtate=curtate, moment=1,
+                               depth=depth-1)
+                p = self._p_x(x, s=s-u, t=u)
+                if e is not None and e1 is not None and p is not None:
+                    #_t = "" if t < 0 else ":" + str(t)
+                    #msg = f"forward e_{x+s}{_t} = e_{x+s}:1 + p_{x+s} e_{x+s+1}"
+                    self.blog(self.pprint.e(x=x, s=s, t=t, curtate=curtate), '= [',
+                              self.pprint.e(x=x, s=s-1, t=self.add_term(t, 1),
+                                            curtate=curtate), '-',
+                              self.pprint.e(x=x, s=s-1, t=1, curtate=curtate), '] /',
+                              self.pprint.p(x=x, s=s-1, t=1), 
+                              depth=depth, rule='forward recursion')
+                    return (e - e1) / p # (3) forward: (e_x-1 - e_x-1:1) / p_x-1
+                else:
+                    self.blog.pop(depth=depth)
+
+                e = self._e_x(x, s=s, t=u, curtate=curtate, moment=1, depth=depth-1)
+                e_t = self._e_x(x, s=s+u, t=self.add_term(t, -u), curtate=curtate,
+                                moment=1, depth=depth-1)
+                p = self._p_x(x, s=s, t=u)
+                if e is not None and e_t is not None and p is not None:
+                    self.blog(self.pprint.e(x=x, s=s, t=t, curtate=curtate), '=',
+                              self.pprint.e(x=x ,s=s, t=u, curtate=curtate), '+',
+                              self.pprint.p(x=x, s=s, t=u), '*',
+                              self.pprint.e(x=x, s=s+u, t=self.add_term(t, -u),
+                                            curtate=curtate),
+                              #f"backward: e_x:1 + p_x e_x+1:{t}",
+                              depth=depth, rule='backward recursion')
+                    return e + p * e_t # (4) backward: e_x:1 + p_x e_x+1:t-1
+                else:
+                    self.blog.pop(depth=depth)
 
 
     def e_x(self, x: int, s: int = 0, t: int = Reserves.WHOLE, 
             curtate: bool = False, moment: int = 1) -> float:
         """Compute expected future lifetime by calling recursion helper
 
         Args:
           x : age of selection
           s : years after selection
           t : limited at t years
           curtate : whether curtate (True) or complete (False) lifetime
           moment : whether to compute first (1) or second (2) moment
         """
-        self.blog = _Blog("Lifetime",
-                         _Blog.e(x=x, s=s, t=t, moment=moment, curtate=curtate),
-                         levels=self.maxdepth)
+        self.blog = self.Blog("Lifetime",
+                              self.pprint.e(x=x, s=s, t=t, moment=moment,
+                                            curtate=curtate),
+                              levels=self.maxdepth)
         e = self._e_x(x, s=s, t=t, curtate=curtate, moment=moment,
                       depth=self.maxdepth)
         if e is not None:
-            print(self.blog, end='')
+            self.blog.display()
             return e
 
     #
     # Formulas for Pure Endowment: t_E_x
     #
-    def get_E(self, x: int, s: int = 0, t: int = 1, 
-              endowment: int = 1, moment: int = 1) -> float | None:
+    def _get_E(self, x: int, s: int = 0, t: int = 1, 
+               endowment: int = 1, moment: int = 1) -> float | None:
         """Get pure endowment from key-value store
 
         Args:
           x : age of selection
           s : years after selection
           t : death within next t years
           endowment : endowment value
           moment : first or second moment of pure endowment
         """
-        key = self.db_key('E', x=x+s, t=t, moment=moment)
+        key = self._db_key('E', x=x+s, t=t, moment=moment)
         val = self.db.get(key, None)
         if val is not None:
             return val * endowment   # stored with benefit=1
 
     def set_E(self, val: float, x: int, s: int = 0, t: int = 1, 
               endowment: int = 1, moment: int = 1) -> "Recursion":
-        """Set pure endowment t_E_[x]+s to given value
+        """Set pure endowment t_E_[x+s] to given value
 
         Args:
           val : value to set
           x : age of selection
           s : years after selection
           t : death within next t years
           endowment : endowment value
           moment : first or second moment of pure endowment
         """
         val /= endowment   # store with benefit=1
-        return self.db_put(self.db_key('E', x=x+s, t=t, moment=moment), val)
+        return self._db_put(self._db_key('E', x=x+s, t=t, moment=moment), val)
 
     def _E_x(self, x: int, s: int = 0, t: int = 1, endowment: int = 1, 
              moment: int = 1, depth: int = 1) -> float:
-        """Helper to compute from recursive and alternate formulas"""
-        E = self.get_E(x, s=s, t=t, endowment=endowment, moment=moment)
+        """Helper to compute pure endowment from recursive and alternate formulas"""
+        E = self._get_E(x, s=s, t=t, endowment=endowment, moment=moment)
         if E is not None:
             return E
         if t < 0:     # t infinite => EPV(t) = 0
             return 0
         if t == 0:    # t = 0 => EPV(0) = endowment**moment
             return endowment**moment
         if moment > 1:
             E = self._E_x(x, s=s, endowment=endowment, depth=depth)
             if E:  # (1) Shortcut: 2E_x = v E_x
-                self.blog(_Blog.E(x=x, s=s, t=t, moment=moment),
-                          f"= v(t={t})"+_Blog.m(moment), '*', _Blog.E(x=x, s=s, t=t),
+                self.blog(self.pprint.E(x=x, s=s, t=t, moment=moment),
+                          f"= " + self.pprint.m(moment*t, v="v"), '*',
+                          self.pprint.E(x=x, s=s, t=t),
                           depth=depth, rule='moments of pure endowment')
-                return E * self.interest.v**(moment-1) 
+                return E * self.interest.v**(moment-1)
+            else:
+                self.blog.pop(depth=depth)
+
         p = self._p_x(x, s=s, t=t, depth=depth-1)  # depth-1)
+
+        #if t == 1 and x==0:
+        #    print('p', x, s, t, depth)
         if p is not None:   # (2) E_x = p_x * v
             #msg = f"pure endowment {t}_E_{x+s} = {t}_p_{x+s} * v^{t}"
-            self.blog(_Blog.E(x=x, s=s, t=t), '=', _Blog.p(x=x, s=s, t=t),
-                      f"* v(t={t})"+_Blog.m(moment),
+            self.blog(self.pprint.E(x=x, s=s, t=t), '=',
+                      self.pprint.p(x=x, s=s, t=t),
+                      f"*", self.pprint.m(moment*t, v="v"),
                       depth=depth, rule='pure endowment')
             return p * (endowment * self.interest.v_t(t))**moment
+        else:
+            self.blog.pop(depth=depth)
         if depth <= 0:
             return None
 
         At = self._A_x(x, s=s, t=t, moment=moment, b=endowment, endowment=0,
                        depth=depth-1)  #depth-1)
         A = self._A_x(x, s=s, t=t, b=endowment, endowment=endowment, 
                       moment=moment, depth=depth-1)        
         if A is not None and At is not None:
-            self.blog(_Blog.E(x=x, s=s, t=t), '=',
-                      _Blog.A(x=x, s=s, t=t, endowment=endowment), '-',
-                      _Blog.A(x=x, s=s, t=t, endowment=0),
+            self.blog(self.pprint.E(x=x, s=s, t=t), '=',
+                      self.pprint.A(x=x, s=s, t=t, endowment=endowment), '-',
+                      self.pprint.A(x=x, s=s, t=t, endowment=0),
                       #f"endowment - term insurance = {t}_E_{x+s}",
                       depth=depth, rule='endowment insurance minus term')
             return A - At  # (3) endowment insurance - term (helpful SULT)
+        else:
+            self.blog.pop(depth=depth)
 
         E = self._E_x(x, s=s, moment=moment, depth=depth-1)
         Et = self._E_x(x, s=s+1, t=t-1, moment=moment, depth=depth-1)
         if E is not None and Et is not None:
             msg = f"chain Rule: {t}_E_{x+s} = E_{x+s} * {t-1}_E_{x+s+1}"
-            self.blog(_Blog.E(x=x, s=s, t=t, moment=moment), '=',
-                      _Blog.E(x=x, s=s, t=1, moment=moment), '*',
-                      _Blog.E(x=x, s=s+1, t=t-1, moment=moment), '*',
-                      _Blog.m(moment, endow=endowment),
+            self.blog(self.pprint.E(x=x, s=s, t=t, moment=moment), '=',
+                      self.pprint.E(x=x, s=s, t=1, moment=moment), '*',
+                      self.pprint.E(x=x, s=s+1, t=t-1, moment=moment),
+                      # '*', self.pprint.m(moment, endow=endowment),
                       depth=depth, rule='pure endowment chain rule')
             return E * Et * endowment**moment # (4) chain rule
+        else:
+            self.blog.pop(depth=depth)
 
     def E_x(self, x: int, s: int = 0, t: int = 1, 
             endowment: int = 1, moment: int = 1) -> float:
         """Compute pure endowment by calling recursion helper
 
         Args:
           x : age of selection
           s : years after selection
           t : term of pure endowment
           endowment : amount of pure endowment
           moment : compute first or second moment
         """
-        self.blog = _Blog("Pure Endowment",
-                         _Blog.E(x=x, s=s, t=t, moment=moment, endowment=endowment),
-                         levels=self.maxdepth)
+        self.blog = self.Blog("Pure Endowment",
+                              self.pprint.E(x=x, s=s, t=t, moment=moment,
+                                            endowment=endowment),
+                              levels=self.maxdepth)
         if moment == self.VARIANCE:  # Bernoulli shortcut for variance
-            found = self.get_E(x, s=s, t=t, endowment=endowment, moment=moment)
+            found = self._get_E(x, s=s, t=t, endowment=endowment, moment=moment)
             if found is not None:
                 return found
             t_p_x = self.p_x(x, s=s, t=t)
             return (endowment * self.interest.v_t(t))**2 * t_p_x * (1-t_p_x)
         found = self._E_x(x, s=s, t=t, endowment=endowment, moment=moment,
                           depth=self.maxdepth)
         if found is not None:
-            print(self.blog, end='')
+            self.blog.display()
             return found
 
     #
     # Formulas for Increasing Insurance: IA_x:t
     #
-    def get_IA(self, x: int, s: int = 0, t: int = Reserves.WHOLE,
-               b: int = 1, discrete: bool = True) -> float | None:
+    def _get_IA(self, x: int, s: int = 0, t: int = Reserves.WHOLE,
+                b: int = 1, discrete: bool = True) -> float | None:
         """Get increasing insurance from key-value store
 
         Args:
           x : age of selection
           s : years after selection
           t : term of increasing insurance
           b : benefit after year 1
           discrete : discrete or continuous increasing insurance
         """
-        key = self.db_key('IA', x=x+s, t=t, discrete=discrete)
+        key = self._db_key('IA', x=x+s, t=t, discrete=discrete)
         val = self.db.get(key, None)
         if val is not None:
             return val * b   # stored with benefit=1
 
     def set_IA(self, val: float, x: int, s: int = 0, t: int = Reserves.WHOLE,
                b: int = 1, discrete: bool = True) -> "Recursion":
-        """Set increasing insurance IA_[x]+s:t to given value
+        """Set increasing insurance IA_[x+s]:t to given value
 
         Args:
           val : value to set
           x : age of selection
           s : years after selection
           t : term of increasing insurance
           b : benefit after year 1
           discrete : discrete or continuous increasing insurance
         """
         val /= b   # store with benefit=1
-        return self.db_put(self.db_key('IA', x=x+s, t=t, 
-                                       discrete=discrete), val)
+        return self._db_put(self._db_key('IA', x=x+s, t=t, 
+                                         discrete=discrete), val)
 
     def _IA_x(self, x: int, s: int = 0, t: int = Reserves.WHOLE, b: int = 1,
               discrete: bool = True, depth: int = 1) -> float | None:
         """Helper to compute from recursive and alternate formulas"""
         if t == 0:
             return 0
-        found = self.get_IA(x=x, s=s, t=t, b=b, discrete=discrete)
+        found = self._get_IA(x=x, s=s, t=t, b=b, discrete=discrete)
         if found is not None:
             return found
         if depth <= 0:
             return None
 
-        if t > 0:  # decreasing must be term insurance
+        if t > 0:
             A = self._A_x(x=x, s=s, t=t, b=b, discrete=discrete, depth=depth-1)
             n = t + int(discrete)
             DA = self._DA_x(x=x, s=s, t=t, b=b, discrete=discrete, depth=depth-1)
             if A is not None and DA is not None:
-                self.blog(_Blog.IA(x=x, s=s, t=t), f'= {n}',
-                          _Blog.A(x=x, s=s, t=t), '-', _Blog.DA(x=x, s=s, t=t),
+                self.blog(self.pprint.IA(x=x, s=s, t=t), f'= {n}',
+                          self.pprint.A(x=x, s=s, t=t), '-',
+                          self.pprint.DA(x=x, s=s, t=t),
                     #f"identity IA_{x+s}:{t}: ({n})A - DA",
                           depth=depth, rule='varying insurance identity')
                 return A * n - DA  # (1) Identity with term and decreasing
+            else:
+                self.blog.pop(depth=depth)
 
-        A = self._A_x(x=x, s=s, t=1, b=b, discrete=discrete, depth=depth-1)
-        IA = self._IA_x(x=x, s=s+1, t=self.add_term(t, -1), b=b, depth=depth-1)
-        p = self._p_x(x, s=s, t=1, depth=depth-1)   # FIXED t=1
-        if A is not None and IA is not None and p is not None:
-            self.blog(_Blog.IA(x=x, s=s, t=t), '=', _Blog.A(x=x, s=s, t=t), '+',
-                      _Blog.p(x=x, s=s), f"* v(t={t}) *", _Blog.IA(x=x, s=s+1, t=t-1),
-                      #f"backward IA_{x+s}:{t}: A + IA_{x+s+1}:{t-1}",
-                      depth=depth, rule='backward recursion')
-            return A + p * self.interest.v * IA  # (2) backward recursion
+        if discrete:
+            A = self._A_x(x=x, s=s, t=1, b=b, discrete=discrete, depth=depth-1)
+            IA = self._IA_x(x=x, s=s+1, t=self.add_term(t, -1), b=b, depth=depth-1)
+            p = self._p_x(x, s=s, t=1, depth=depth-1)   # FIXED t=1
+            if A is not None and IA is not None and p is not None:
+                self.blog(self.pprint.IA(x=x, s=s, t=t), '=',
+                          self.pprint.A(x=x, s=s, t=t), '+',
+                          self.pprint.p(x=x, s=s), f"*", self.pprint.m(t, v="v"), "*",
+                          self.pprint.IA(x=x, s=s+1, t=t-1),
+                          #f"backward IA_{x+s}:{t}: A + IA_{x+s+1}:{t-1}",
+                          depth=depth, rule='backward recursion')
+                return A + p * self.interest.v * IA  # (2) backward recursion
+            else:
+                self.blog.pop(depth=depth)
 
     def increasing_insurance(self, x: int, s: int = 0, t: int = Reserves.WHOLE,
                              b: int = 1, discrete: bool = True) -> float:
         """Compute increasing insurance with recursive helper
 
         Args:
           x : age of selection
           s : years after selection
           t : term of insurance
           b : amount of benefit in first year
           discrete : benefit paid year-end (True) or moment of death (False)
         """
-        self.blog = _Blog("Increasing Insurance",
-                         _Blog.IA(x=x, s=s, t=t, b=b, discrete=discrete),
-                         levels=self.maxdepth)
+        self.blog = self.Blog("Increasing Insurance",
+                              self.pprint.IA(x=x, s=s, t=t, b=b, discrete=discrete),
+                              levels=self.maxdepth)
         IA = self._IA_x(x, s=s, b=b, t=t, discrete=discrete, depth=self.maxdepth)
         if IA is not None:
-            print(self.blog, end='')
+            self.blog.display()
             return IA
         IA = super().increasing_insurance(x, s=s, b=b, t=t, discrete=discrete)
         if IA is not None:
-            print(self.blog, end='')
+            self.blog.display()
             return IA
 
     #
     # Formulas for Decreasing insurance: DA_x:t
     #
-    def get_DA(self, x: int, s: int = 0, t: int = Reserves.WHOLE,
-               b: int = 1, discrete: bool = True) -> float | None:
+    def _get_DA(self, x: int, s: int = 0, t: int = Reserves.WHOLE,
+                b: int = 1, discrete: bool = True) -> float | None:
         """Get decreasing insurance from key-value store
 
         Args:
           x : age of selection
           s : years after selection
           t : term of decreasing insurance
           b : benefit after year 1
           discrete : discrete or continuous decreasing insurance
         """
-        key = self.db_key('DA', x=x+s, t=t, discrete=discrete)
+        key = self._db_key('DA', x=x+s, t=t, discrete=discrete)
         val = self.db.get(key, None)
         if val is not None:
             return val * b   # stored with benefit=1
 
     def set_DA(self, val: float, x: int, s: int = 0, t: int = Reserves.WHOLE,
                b: int = 1, discrete: bool = True) -> "Recursion":
-        """Set decreasing insurance DA_[x]+s:t to given value
+        """Set decreasing insurance DA_[x+s]:t to given value
 
         Args:
           val : value to set
           x : age of selection
           s : years after selection
           t : term of decreasing insurance
           b : benefit after year 1
           discrete : discrete or continuous decreasing insurance
         """
         val /= b     # store with benefit=1
-        return self.db_put(self.db_key('DA', x=x+s, t=t, 
-                                       discrete=discrete), val)
+        return self._db_put(self._db_key('DA', x=x+s, t=t, 
+                                         discrete=discrete), val)
 
     def _DA_x(self, x: int, s: int = 0, t: int = Reserves.WHOLE, b: int = 1,
               discrete: bool = True, depth: int = 1) -> float | None:
         """Helper to compute from recursive and alternate formulas"""
-        found = self.get_DA(x=x, s=s, t=t, discrete=discrete)
+        found = self._get_DA(x=x, s=s, t=t, discrete=discrete)
         if found is not None:
             return found
         if t == 0:
             return 0
         if depth <= 0:
             return None
-        if t < 0:  # decreasing must be term insurance
-            return None
+        assert t < 0,  "Decreasing insurance must be term insurance"
     
         A = self._A_x(x=x, s=s, t=t, b=b, discrete=discrete, depth=depth-1)
         n = t + int(discrete)
         IA = self._DA_x(x=x, s=s, t=t, b=b, discrete=discrete, depth=depth-1)
         if A is not None and IA is not None:
-            self.blog(_Blog.DA(x=x, s=s, t=t), f'= {n}',
-                      _Blog.A(x=x, s=s, t=t), '-', _Blog.IA(x=x, s=s, t=t),
+            self.blog(self.pprint.DA(x=x, s=s, t=t), f'= {n}',
+                      self.pprint.A(x=x, s=s, t=t), '-',
+                      self.pprint.IA(x=x, s=s, t=t),
                       depth=depth, rule='varying insurance identity')
-            return A * n - IA  # (1) identity with term and decreasing
+            return A * n - IA  # (1) identity with term and increasing
+        else:
+            self.blog.pop(depth=depth)
 
-        DA = self._IA_x(x=x, s=s+1, t=self.add_term(t, -1), b=b, depth=depth-1)
-        p = self._p_x(x, s=s, depth=depth-1)
-        if DA is not None and p is not None:
-            #msg = f"backward DA_{x+s}:{t}: v(t q_{x+s} + p_{x+s} DA_{x+s+1}:{t-1})"
-            self.blog(_Blog.DA(x=x, s=s, t=t), f"= v(t={t}) * t *", _Blog.q(x=x, s=s),
-                      '+', _Blog.p(x=x, s=s), '*', _Blog.DA(x=x, s=s+1, t=t-1),
-                      depth=depth, rule='backward recursion')
-            return self.interest.v * ((1-p)*t + p*DA)  # (2) backward recursion
+        if discrete:
+            DA = self._IA_x(x=x, s=s+1, t=self.add_term(t, -1), b=b, depth=depth-1)
+            p = self._p_x(x, s=s, depth=depth-1)
+            if DA is not None and p is not None:
+                #f"backward DA_{x+s}:{t}: v(t q_{x+s} + p_{x+s} DA_{x+s+1}:{t-1})"
+                self.blog(self.pprint.DA(x=x, s=s, t=t), f"=",
+                          self.pprint.m(t, v="v"), "* t *",
+                          self.pprint.q(x=x, s=s), '+',
+                          self.pprint.p(x=x, s=s), '*', self.pprint.DA(x=x, s=s+1, t=t-1),
+                          depth=depth, rule='backward recursion')
+                return self.interest.v * ((1-p)*t + p*DA)  # (2) backward recursion
+            else:
+                self.blog.pop(depth=depth)
 
     def decreasing_insurance(self, x: int, s: int = 0, t: int = Reserves.WHOLE,
                              b: int = 1, discrete: bool = True) -> float:
-        """Compute decreasing insurance by calling recursive helper first
+        """Compute decreasing insurance by attempting recursive helper first
 
         Args:
           x : age of selection
           s : years after selection
           t : term of insurance
           b : amount of benefit in first year
           discrete : benefit paid year-end (True) or moment of death (False)
         """
-        self.blog = _Blog("Increasing Insurance",
-                         _Blog.DA(x=x, s=s, t=t, b=b, discrete=discrete),
-                         levels=self.maxdepth)
+        self.blog = self.Blog("Increasing Insurance",
+                              self.pprint.DA(x=x, s=s, t=t, b=b, discrete=discrete),
+                              levels=self.maxdepth)
         if t == 0:
             return 0
         A = self._DA_x(x=x, s=s, t=t, b=b, discrete=discrete, depth=self.maxdepth)
         if A is not None:
-            print(self.blog, end='')
+            self.blog.display()
             return A
         A = super().decreasing_insurance(x, s=s, b=b, t=t, discrete=discrete)
         if A is not None:
-            print(self.blog, end='')
+            self.blog.display()
             return A
 
     #
     # Formulas for Insurance: A_x:t
     #
-    def get_A(self, x: int, s: int = 0, u: int = 0, t: int = Reserves.WHOLE,
-              b: int = 1, moment: int = 1, endowment: int = 0, 
-              discrete: bool = True) -> float | None:
+    def _get_A(self, x: int, s: int = 0, u: int = 0, t: int = Reserves.WHOLE,
+               b: int = 1, moment: int = 1, endowment: int = 0, 
+               discrete: bool = True) -> float | None:
         """Get insurance from key-value store
 
         Args:
           x : age of selection
           s : years after selection
           u : defer u years
           t : term of insurance
@@ -675,615 +1120,586 @@
             return endowment
         if b == 0:          # normalize insurance factor by benefit amount
             scale = endowment
             endowment = 1
         else:
             scale = b
             endowment = 1 if b == endowment else endowment / b
-        key = self.db_key('A', x=x+s, u=u, t=t, moment=moment, 
-                          endowment=endowment, discrete=discrete)
+        key = self._db_key('A', x=x+s, u=u, t=t, moment=moment, 
+                           endowment=endowment, discrete=discrete)
         val = self.db.get(key, None)
         if val is not None:
             return val * scale   # stored with benefit=1
 
 
     def set_A(self, val: float, x: int, s: int = 0, t: int = Reserves.WHOLE,
               u: int = 0, b: int = 1, moment: int = 1, endowment: int = 0, 
               discrete: bool = True) -> "Recursion":
-        """Set insurance u|_A_[x]+s:t to given value
+        """Set insurance u|_A_[x+s]:t to given value
 
         Args:
           val : value to set
           x : age of selection
           s : years after selection
           u : defer u years
           t : term of insurance
           endowment : endowment amount
           discrete : discrete (True) or continuous (False) insurance
           moment : first or second moment of insurance
+
+        Examples
+          >>> Recursion().set_interest(i=0.06).set_A(A, x=0)
         """
         if endowment < 0:      # endowment insurance with equal death and endow
             endowment = b
         if endowment == 0:     # normalize insurance factor by benefit amount
             val /= b
         elif b == 0:
             val /= endowment   # store with benefit=1
         else:
             if b != 1:
                 val /= b
                 endowment /= b
-        return self.db_put(self.db_key('A', x=x+s, t=t, u=u,
-                                       moment=moment, endowment=endowment, 
-                                       discrete=discrete), val)
+        return self._db_put(self._db_key('A', x=x+s, t=t, u=u,
+                                         moment=moment, endowment=endowment, 
+                                         discrete=discrete), val)
 
     def _A_x(self, x: int, s: int = 0, t: int = Reserves.WHOLE, u: int = 0,
              b: int = 1, discrete: bool = True, endowment: int = 0,
              moment: int = 1, depth: int = 1) -> float | None:
         """Helper to compute from recursive and alternate formulas"""
-        
+
         if endowment == b and t == 1 and discrete: # 1-year endow ins
+#            self.blog(self.pprint.A(x=x, s=s, t=1, endowment=b, b=b, moment=moment),
+#                      '=', self.pprint.m(moment, v="v"),
+#                      depth=depth, rule='one-year endowment insurance')
             return (self.interest.v_t(1) * endowment)**moment
-        found = self.get_A(x=x, s=s, t=t, b=b, u=u, discrete=discrete, 
-                           moment=moment, endowment=endowment)
+        found = self._get_A(x=x, s=s, t=t, b=b, u=u, discrete=discrete, 
+                            moment=moment, endowment=endowment)
         if found is not None:
             return found
         if depth <= 0:
             return None
 
-        if u > 0:  # (1) deferred insurance  
+        if discrete and u > 0:  # (1) deferred insurance  
             A = self._A_x(x=x, s=s+1, t=t, b=b, u=u-1, discrete=discrete, 
                               moment=moment, endowment=endowment, depth=depth-1)
             E = self._E_x(x, s=s, t=1, moment=moment, depth=depth-1)
             if A is not None and p is not None:  # (1a) backward E_x * A
                 #msg = f"backward deferred {u}_A_{x+s}: {u}_E * A_{x+s+u}"
-                self.blog(_Blog.A(x=x, s=s, t=t, u=u, b=b, moment=moment), '=',
-                          _Blog.E(x=x, s=s, moment=moment), '*',
-                          _Blog.A(x=x, s=s+1, t=t, u=u-1, moment=moment),
+                self.blog(self.pprint.A(x=x, s=s, t=t, u=u, b=b, moment=moment), '=',
+                          self.pprint.E(x=x, s=s, moment=moment), '*',
+                          self.pprint.A(x=x, s=s+1, t=t, u=u-1, moment=moment),
                           depth=depth, rule='backward recursion')
                 return E * A
+            else:
+                self.blog.pop(depth=depth)
 
             A = self._A_x(x, s=s-1, t=t, b=b, u=u+1, discrete=discrete, 
                           moment=moment, endowment=endowment, depth=depth-1)
             E = self._E_x(x, s=s-1, t=1, moment=moment, depth=depth-1)
             if A is not None and E is not None: # (1b) forward recursion
                 msg = f"forward deferred {u}_A_{x+s}: {u+1}A_{x+s-1} / E"
-                self.blog(_Blog.A(x=x, s=s, t=t, u=u, b=b, moment=moment), '=',
-                          _Blog.A(x=x, s=s-1, t=t, u=u+1, moment=moment), '/',
-                          _Blog.E(x=x, s=s-1, moment=moment),
+                self.blog(self.pprint.A(x=x, s=s, t=t, u=u, b=b, moment=moment), '=',
+                          self.pprint.A(x=x, s=s-1, t=t, u=u+1, moment=moment), '/',
+                          self.pprint.E(x=x, s=s-1, moment=moment),
                           depth=depth, rule='forward recursion')
                 return A / E
+            else:
+                self.blog.pop(depth=depth)
             return None
-
+        
         if endowment > 0: # (2a) endowment = term + E_x * endowment
             A = self._A_x(x=x, s=s, t=t, b=b, discrete=discrete, 
                           moment=moment, depth=depth-1)
             E_x = self._E_x(x=x, s=s, t=t, moment=moment, 
                             endowment=endowment, depth=depth-1)
             if A is not None and E_x is not None:
                 # f"term + pure insurance = A_{x+s}:{t}",
-                self.blog(_Blog.A(x=x, s=s, t=t, endowment=endowment, moment=moment),
-                          '=', _Blog.A(x=x, s=s, t=t, moment=moment), '+',
-                          _Blog.E(x=x, s=s, t=t, endowment=endowment, moment=moment),
+                self.blog(self.pprint.A(x=x, s=s, t=t, endowment=endowment,
+                                            moment=moment),
+                          '=', self.pprint.A(x=x, s=s, t=t, moment=moment), '+',
+                          self.pprint.E(x=x, s=s, t=t, endowment=endowment,
+                                            moment=moment),
                           depth=depth, rule='term plus pure endowment')
                 return A + E_x
-        else:             # (2b) term = endowment insurance - E_x * endowment
+            else:
+                self.blog.pop(depth=depth)
+        elif t >= 0:     # (2b) term = endowment insurance - E_x * endowment
             A = self._A_x(x=x, s=s, t=t, b=b, discrete=discrete, 
                           moment=moment, endowment=b, depth=depth-1)
             E_x = self._E_x(x=x, s=s, t=t, moment=moment, endowment=b, 
                             depth=depth-1)
             if A is not None and E_x is not None:
                 #msg = f"endowment insurance - pure endowment = A_{x+s}^1:{t}"
-                self.blog(_Blog.A(x=x, s=s, t=t, moment=moment), '=',
-                          _Blog.A(x=x, s=s, t=t, moment=moment, endowment=b), '-',
-                          _Blog.E(x=x, s=s, t=t, endowment=b, moment=moment),
+                self.blog(self.pprint.A(x=x, s=s, t=t, moment=moment), '=',
+                          self.pprint.A(x=x, s=s, t=t, moment=moment, endowment=b), '-',
+                          self.pprint.E(x=x, s=s, t=t, endowment=b, moment=moment),
                           depth=depth, rule='endowment insurance - pure')
                 return A - E_x
+            else:
+                self.blog.pop(depth=depth)
 
-        if not discrete:  # recursions for discrete insurance
+        if not discrete:  # recursions only for discrete insurance
             return None
         if t == 1:  # special cases for discrete one-year insurance
             if endowment == b:  # (3a) discrete one-year endowment insurance
-                self.blog(_Blog.A(x=x, s=s, t=1, endowment=endowment,
-                                 moment=moment), f"= v"+_Blog.m(moment),
-                          "*", _Blog.m(moment, endow=endowment),
-                          depth=depth, rule='one-year endowment insurance')
-                return (self.interest.v * endowment)**moment
+#                self.blog(self.pprint.A(x=x, s=s, t=1, endowment=endowment,
+#                                 moment=moment), f"= v"+self.pprint.m(moment),
+#                          "*", self.pprint.m(moment, endow=endowment),
+#                          depth=depth, rule='one-year endowment insurance')
+                return (self.interest.v * endowment)**moment   
             p = self._p_x(x, s=s, t=1)
+
+            #print(p, x, s, t, b, endowment)
+            
             if p is not None:  # (3b) one-year discrete insurance
-                self.blog(_Blog.A(x=x, s=s, t=t, moment=moment, endowment=endowment),
-                          f"= v"+_Blog.m(moment), "*",
-                          _Blog.q(x=x, s=s), f"*", "v"*_Blog.m(moment), "+",
-                          _Blog.p(x=x, s=s), f"*".
-                          _Blog.m(moment, endow=endowment),
+                self.blog(self.pprint.A(x=x, s=s, t=t, moment=moment,
+                                            endowment=endowment), "=",
+                          self.pprint.m(moment, v="v"), "*",
+                          self.pprint.q(x=x, s=s), f"*",
+                          self.pprint.m(moment, v="v"), "+",
+                          self.pprint.p(x=x, s=s), f"*".
+                          self.pprint.m(moment, endow=endowment),
                           #f"discrete 1-year insurance: A_{x+s}:1 = qv",
                           depth=depth, rule='one-year discrete insurance')
                 return (self.interest.v**moment 
                         * ((1 - p) * b**moment + p * endowment**moment))
-    
+            else:
+                self.blog.pop(depth=depth)
+                
+        # insurance recursions
+        # TODO: mo re general recursions u in [1, ..., 50]
+
+#        """
         A = self._A_x(x=x, s=s+1, t=self.add_term(t, -1), b=b, 
                       discrete=discrete, moment=moment,
                       endowment=endowment, depth=depth-1)
         p = self._p_x(x, s=s, t=1, depth=depth-1) # (4) backward recursion
         if A is not None and p is not None:
-            self.blog(_Blog.A(x=x, s=s, t=t, b=b, moment=moment),
-                      f"= v"+_Blog.m(moment), "* [",
-                      _Blog.q(x=x,s=s), f"* b"+_Blog.m(moment), "+",
-                      _Blog.p(x=x, s=s), '*',
-                      _Blog.A(x=x, s=s+1, t=t-1, b=b, moment=moment), ']',
+            self.blog(self.pprint.A(x=x, s=s, t=t, b=b, moment=moment),
+                      f"= v"+self.pprint.m(moment), "* [",
+                      self.pprint.q(x=x,s=s), f"*",
+                      self.pprint.m(moment, b="b"), "+",
+                      self.pprint.p(x=x, s=s), '*',
+                      self.pprint.A(x=x, s=s+1, t=t-1, b=b, moment=moment), ']',
                       #f"backward: A_{x+s} = qv + pvA_{x+s+1}",
                       depth=depth, rule='backward recursion')
             return self.interest.v_t(1)**moment * ((1 - p)*b**moment + p*A)
+        else:
+            self.blog.pop(depth=depth)
+        """
+        for y in [1]: #self._t['A']:
+            At = self._A_x(x=x, s=s, t=y, discrete=discrete, b=b,
+                           moment=moment, depth=depth-1)
+            A = self._A_x(x=x, s=s+y, t=self.add_term(t, -y), b=b, discrete=discrete,
+                          moment=moment, endowment=endowment, depth=depth-1)
+            E = self._E_x(x, s=s, t=y, moment=moment, depth=depth-1) 
+
+            #print('*', At, A, E, x, s, t, y, b, endowment)
+            if A is not None and At is not None and E is not None:  # (4a) backward recursion
+                self.blog(self.pprint.A(x=x, s=s, t=t, b=b, moment=moment), "=",
+                          self.pprint.A(x=x, s=s, t=y, moment=moment, b=b), '+',
+                          self.pprint.E(x=x, s=s, t=y, moment=moment), '*',
+                          self.pprint.A(x=x, s=s+y, t=self.add_term(t, -y), b=b,
+                                            moment=moment, endowment=endowment),
+                          #f"backward: A_{x+s} = qv + pvA_{x+s+1}",
+                          depth=depth, rule='backward recursion')
+                return At + E * A
+            else:
+                self.blog.pop(depth=depth)
+
+            At = self._A_x(x=x, s=s-y, t=self.add_term(t, y), b=b, discrete=discrete,
+                           moment=moment, endowment=endowment, depth=depth-1)
+            A = self._A_x(x=x, s=s-y, t=y, b=b, discrete=discrete, moment=moment,
+                          depth=depth-1)
+            E = self._E_x(x, s=s-y, t=y, moment=moment, depth=depth-1) 
 
-        A = self._A_x(x=x, s=s-1, t=self.add_term(t, 1), b=b, u=u, 
+            #print('#', At, A, E, x, s, t, y, b, endowment)
+            if A is not None and At is not None and E is not None:  # (5) forward recursion
+                self.blog(self.pprint.A(x=x, s=s, t=t, b=b,
+                                            moment=moment, endowment=endowment), '= [',
+                          self.pprint.A(x=x, s=s-y, t=self.add_term(t, y),
+                                            b=b, endowment=endowment, moment=moment), '-',
+                          self.pprint.A(x=x, s=s-y, t=y, b=b, moment=moment), '] /',
+                          self.pprint.E(x=x, s=s-y, t=y, moment=moment),
+                          #f"forward: A_{x+s} = (A_{x+s-1}/v - q) / p",
+                          depth=depth, rule='forward recursion')
+                return (At - A) / E
+            else:
+                self.blog.pop(depth=depth)
+        """
+        A = self._A_x(x=x, s=s-1, t=self.add_term(t, 1), b=b, 
                       discrete=discrete, moment=moment, 
                       endowment=endowment, depth=depth-1)
         p = self._p_x(x, s=s-1, t=1, depth=depth-1)
         if A is not None and p is not None:  # (5) forward recursion
-            self.blog(_Blog.A(x=x, s=s, t=t, b=b, moment=moment), '= [',
-                      _Blog.A(x=x, s=s-1, t=t+1, b=b, moment=moment),
-                      f"/v"+_Blog.m(moment), "-", _Blog.q(x=x,s=s),
-                      f"* b"+_Blog.m(moment), "] /", _Blog.p(x=x, s=s),
+            self.blog(self.pprint.A(x=x, s=s, t=t, b=b, moment=moment), '= [',
+                      self.pprint.A(x=x, s=s-1, t=t+1, b=b, moment=moment),
+                      f"/", self.pprint.m(moment, v="v"), "-",
+                      self.pprint.q(x=x, s=s-1), f"*",
+                      self.pprint.m(moment, b="b"), "] /", self.pprint.p(x=x, s=s-1),
                       #f"forward: A_{x+s} = (A_{x+s-1}/v - q) / p",
                       depth=depth, rule='forward recursion')
             return (A/self.interest.v_t(1)**moment - (1-p)*b**moment) / p
+        else:
+            self.blog.pop(depth=depth)
+ #       """
 
     def whole_life_insurance(self, x: int, s: int = 0, b: int = 1, 
                              discrete: bool = True, moment: int = 1) -> float:
-        """Compute whole life insurance A_x by calling recursion helper and twin
+        """Compute whole life insurance A_x by attempting recursion and twin first
 
         Args:
           x : age of selection
           s : years after selection
           b : amount of benefit
           moment : compute first or second moment
           discrete : benefit paid year-end (True) or moment of death (False)
         """
-        self.blog = _Blog("Whole Life Insurance",
-                         _Blog.A(x=x, s=s, t=Reserves.WHOLE, b=b, u=0,
-                                endowment=0, moment=moment, discrete=discrete),
-                         levels=self.maxdepth)
+        self.blog = self.Blog("Whole Life Insurance",
+                              self.pprint.A(x=x, s=s, t=Reserves.WHOLE, b=b, u=0,
+                                            endowment=0, moment=moment,
+                                            discrete=discrete),
+                              levels=self.maxdepth)
         found = self._A_x(x, s=s, b=b, moment=moment, discrete=discrete,
                           depth=self.maxdepth)
         if found is not None:
-            print(self.blog, end='')
+            self.blog.display()
             return found
         if moment == 1 and self.interest.i > 0:  # (1) twin annuity
             a = self._a_x(x, s=s, b=b, discrete=discrete, depth=self.maxdepth)
             if a is not None:
-                self.blog("A_x = 1 - d * a_x",
+                self.blog(self.pprint.a(x=x, s=s), '= [ 1 -',
+                          self.pprint.A(x=x, s=s), f"] / d",
+                          #"Annuity twin: a = (1 - A) / d",
                           depth=self.maxdepth, rule='annuity twin')
-                print(self.blog, end='')
+                self.blog.display()
                 return self.insurance_twin(a=a, discrete=discrete)
         A = super().whole_life_insurance(x, s=s, b=b, discrete=discrete,
                                          moment=moment)
         if A is not None:
-            print(self.blog, end='')
+            self.blog.display()
             return A
 
     def term_insurance(self, x: int, s: int = 0, t: int = 1, b: int = 1, 
                        moment: int = 1, discrete: bool = True) -> float:
-        """Compute term life insurance A_x:t^1 by calling recursion helper: 
+        """Compute term life insurance A_x:t^1 by attempting recursion first 
 
         Args:
           x : age of selection
           s : years after selection
           t : term of insurance
           b : amount of benefit
           moment : compute first or second moment
           discrete : benefit paid year-end (True) or moment of death (False)
         """
-        self.blog = _Blog("Term Insurance",
-                         _Blog.A(x=x, s=s, t=t, b=b, u=0, discrete=discrete,
-                                 endowment=0, moment=moment),
-                         levels=self.maxdepth)
+        self.blog = self.Blog("Term Insurance",
+                              self.pprint.A(x=x, s=s, t=t, b=b, u=0, discrete=discrete,
+                                            endowment=0, moment=moment),
+                              levels=self.maxdepth)
         found = self._A_x(x, s=s, b=b, t=t, moment=moment, discrete=discrete,
                           depth=self.maxdepth)
         if found is not None:
-            print(self.blog, end='')
+            self.blog.display()
             return found
         A = super().term_insurance(x, s=s, b=b, t=t, discrete=discrete,
                                    moment=moment)
         if A is not None:
-            print(self.blog, end='')
+            self.blog.display()
             return A
 
     def deferred_insurance(self, x: int, s: int = 0, b: int = 1, u: int = 0, 
                            t: int = Reserves.WHOLE, moment: int = 1, 
                            discrete: bool = True) -> float:
-        """Compute deferred life insurance u|A_x:t^1 by calling recursion helper: """
-        self.blog = _Blog("Deferred Insurance",
-                         _Blog.A(x=x, s=s, t=t, b=b, u=u, discrete=discrete,
-                                endowment=0, moment=moment),
-                         levels=self.maxdepth)
-        A = self.get_A(x=x, s=s, t=t, b=b, u=u, discrete=discrete, 
-                       moment=moment)
+        """Compute deferred life insurance u|A_x:t^1 by attempting recursion first"""
+        self.blog = self.Blog("Deferred Insurance",
+                              self.pprint.A(x=x, s=s, t=t, b=b, u=u,
+                                            discrete=discrete,
+                                            endowment=0, moment=moment),
+                              levels=self.maxdepth)
+        A = self._get_A(x=x, s=s, t=t, b=b, u=u, discrete=discrete, 
+                        moment=moment)
         if A is not None:
-            print(self.blog, end='')
+            self.blog.display()
             return A
         A = super().deferred_insurance(x, s=s, b=b, t=t, u=u, 
                                        discrete=discrete, moment=moment)
         if A is not None:
-            print(self.blog, end='')
+            self.blog.display()
             return A
     
     def endowment_insurance(self, x: int, s: int = 0, t: int = 1, b: int = 1,
                             endowment: int = -1, moment: int = 1,
                             discrete: bool = True) -> float:
-        """Compute endowment insurance u|A_x:t by calling recursion helper: """
-        self.blog = _Blog("Endowment Insurance",
-                         _Blog.A(x=x, s=s, t=t, b=b, u=0, discrete=discrete,
-                                endowment=endowment, moment=moment),
-                         levels=self.maxdepth)
+        """Compute endowment insurance u|A_x:t by attempting recursion first"""
+        self.blog = self.Blog("Endowment Insurance",
+                              self.pprint.A(x=x, s=s, t=t, b=b, u=0,
+                                            discrete=discrete,
+                                            endowment=endowment, moment=moment),
+                              levels=self.maxdepth)
         assert t >= 0
         if endowment < 0:
             endowment = b
         found = self._A_x(x, s=s, b=b, t=t, moment=moment, discrete=discrete,
                           endowment=endowment, depth=self.maxdepth)
         if found is not None:
-            print(self.blog, end='')
+            self.blog.display()
             return found
         if moment == 1 and endowment == b and self.interest.i > 0:
-            a = self._a_x(x, s=s, b=b, t=t, moment=moment, discrete=discrete,
+            a = self._a_x(x, s=s, b=b, t=t, discrete=discrete,
                           depth=self.maxdepth)
             if a is not None:   # twin insurance
-                print(self.blog, end='')
+                self.blog.display()
                 return self.insurance_twin(a=a, discrete=discrete)
         A = super().endowment_insurance(x, s=s, b=b, t=t, discrete=discrete,
                                         moment=moment, endowment=endowment)
         if A is not None:
-            print(self.blog, end='')
+            self.blog.display()
             return A
 
     #
     # Formulas for Annuties: a_x:t
     #
-    def get_a(self, x: int, s: int = 0, u: int = 0, t: int = Reserves.WHOLE,
-              b: int = 1, variance: bool = False, 
-              discrete: bool = True) -> float | None:
+    def _get_a(self, x: int, s: int = 0, u: int = 0, t: int = Reserves.WHOLE,
+               b: int = 1, variance: bool = False, 
+               discrete: bool = True) -> float | None:
         """Get annuity from key-value store
 
         Args:
           x : age of selection
           s : years after selection
           u : defer u years
           t : term of annuity
           b : benefit amount
           discrete : whether annuity due (True) or continuous (False)
           variance : whether first moment (False) or variance (True)
         """
-        key = self.db_key('a', x=x+s, u=u, t=t, 
-                          variance=variance, discrete=discrete)
+        key = self._db_key('a', x=x+s, u=u, t=t, 
+                           variance=variance, discrete=discrete)
         val = self.db.get(key, None)
         if val is not None:
             return val * b    # stored with benefit=1
 
     def set_a(self, val: float, x: int, s: int = 0, t: int = Reserves.WHOLE,
               u: int = 0, b: int = 1, variance: bool = False, 
               discrete: bool = True) -> "Recursion":
-        """Set annuity u|_a_[x]+s:t to given value
+        """Set annuity u|_a_[x+s]:t to given value
 
         Args:
           val : value to set
           x : age of selection
           s : years after selection
           u : defer u years
           t : term of annuity
           b : benefit amount
           discrete : whether annuity due (True) or continuous (False)
           variance : whether first moment (False) or variance (True)
+ 
+        Examples:
+          >>> Recursion().set_interest(i=0.06).set_a(7, x=1)
         """
         val /= b    # store with benefit=1
-        return self.db_put(self.db_key('a', x=x+s, t=t, u=u, 
-                           variance=variance, discrete=discrete), val)
+        return self._db_put(self._db_key('a', x=x+s, t=t, u=u, 
+                                         variance=variance, discrete=discrete), val)
 
     def _a_x(self, x: int, s: int = 0, t: int = Reserves.WHOLE, 
              u: int = 0, b: int = 1, discrete: bool = True, 
              variance: bool = False, depth: int = 1) -> float | None:
         """Helper to compute from recursive and alternate formulas"""
         if t == 1 and not u and discrete:
-            self.blog(_Blog.a(x=x, s=s, t=1, discrete=discrete), '= 1',
-                      depth=depth, rule='one-year discrete annuity')
+#            self.blog(self.pprint.a(x=x, s=s, t=1, discrete=discrete), '= 1',
+#                      depth=depth, rule='one-year discrete annuity')
             return b 
         if t == 0:
             return 0
-        found = self.get_a(x=x, s=s, t=t, b=b, u=u, discrete=discrete,
-                           variance=variance)
+        found = self._get_a(x=x, s=s, t=t, b=b, u=u, discrete=discrete,
+                            variance=variance)
         if found is not None:
             return found
         if depth <= 0:
             return None
-        if variance:
-            return None
+        assert variance is False, "Annuity recursion requires variance=False"
 
         if u > 0:  # (1) deferred annuity
             found = self._a_x(x=x, s=s+1, t=t, b=b, u=u-1, discrete=discrete, 
                               variance=variance, depth=depth-1)
             E = self._E_x(x, s=s, t=1, depth=depth-1)
             if found is not None and E is not None:
                 #msg = f"backward {u}_a_{x+s} = {u}_E * a_{x+s+u}"
-                self.blog(_Blog.a(x=x, s=s, u=u, t=t), '=',
-                          _Blog.a(x=x, s=s+1, t=t, u=u-1), '/', _Blog.E(x=x, s=s),
+                self.blog(self.pprint.a(x=x, s=s, u=u, t=t), '=',
+                          self.pprint.a(x=x, s=s+1, t=t, u=u-1), '/',
+                          self.pprint.E(x=x, s=s),
                           depth=depth, rule='backward deferred annuity')
                 return E * found  # (1a) backward recusion
+            else:
+                self.blog.pop(depth=depth)
 
             found = self._a_x(x=x, s=s-1, t=t, b=b, u=u+1, discrete=discrete, 
                               depth=depth-1)         # FIXED u=u+1
             E = self._E_x(x, s=s-1, t=1, depth=depth-1)
             if found is not None and E is not None:  # (1b) forward
                 #msg = f"forward: {u}_a_{x+s} = {u+1}_a_{x+s-1}/E_{x+s-1}"
-                self.blog(_Blog.a(x=x, s=s, u=u, t=t), '=',
-                          _Blog.a(x=x, s=s-1, t=t, u=u+1), '/', _Blog.E(x=x, s=s-1),
+                self.blog(self.pprint.a(x=x, s=s, u=u, t=t), '=',
+                          self.pprint.a(x=x, s=s-1, t=t, u=u+1), '/',
+                          self.pprint.E(x=x, s=s-1),
                           depth=depth, rule='forward deferred annuity')
                 return found / E
+            else:
+                self.blog.pop(depth=depth)
+            return None
 
-        else:  # (2) Temporary and whole annuity
+        # TODOS: more general recursions u in [1,...,50]?
+        if discrete:   # recursions only for discrete annuities
             found = self._a_x(x=x, s=s+1, t=self.add_term(t, -1), b=b, u=u, 
                               discrete=discrete, 
                               variance=variance, depth=depth-1)
             E = self._E_x(x, s=s, t=1, depth=depth-1)
             if found is not None and E is not None:  # (2a) backward
                 #msg = (f"backward: a_{x+s}{'' if t < 0 else (':'+str(t))} = 1 + "
                 #       + f"E_{x+s} a_{x+s+1}{'' if t < 0 else (':'+str(t-1))}")
                 #_t = "" if t < 0 else f":{t-1}"
-                self.blog(_Blog.a(x=x, s=s, t=t), '= 1 +',
-                          _Blog.E(x=x, s=s, t=1), '*', _Blog.a(x=x, s=s+1, t=t-1),
+                self.blog(self.pprint.a(x=x, s=s, t=t), '= 1 +',
+                          self.pprint.E(x=x, s=s, t=1), '*',
+                          self.pprint.a(x=x, s=s+1, t=t-1),
                           depth=depth, rule='backward recursion')
                 return b + E * found
+            else:
+                self.blog.pop(depth=depth)
 
             found = self._a_x(x=x, s=s-1, t=self.add_term(t, 1), b=b, u=u, 
                               discrete=discrete, depth=depth-1)
             E = self._E_x(x, s=s-1, t=1, depth=depth-1)
             if found is not None and E is not None:  # (2b) forward
                 _t = "" if t < 0 else f":{t-1}"
-                self.blog(_Blog.a(x=x, s=s, t=t), '= [',
-                          _Blog.a(x=x, s=s-1), '- 1 ] /',
-                          _Blog.E(x=x, s=s-1, t=1),
+                self.blog(self.pprint.a(x=x, s=s, t=t), '= [',
+                          self.pprint.a(x=x, s=s-1, t=self.add_term(t, 1)), '- 1 ] /',
+                          self.pprint.E(x=x, s=s-1, t=1),
                     #f"forward: a_{x+s}{_t} = (a_{x+s-1} - 1)/E",
                           depth=depth, rule='forward recursion')
                 return (found - b) / E
+            else:
+                self.blog.pop(depth=depth)
 
     def whole_life_annuity(self, x: int, s: int = 0, b: int = 1, 
                            variance: bool = False,
                            discrete: bool = True) -> float:
-        """Compute whole life annuity a_x by calling recursion then twin first
+        """Compute whole life annuity a_x by attempting recursion then twin first
 
         Args:
           x : age of selection
           s : years after selection
           b : annuity benefit amount
           variance (bool): return EPV (True) or variance (False)
           discrete : annuity due (True) or continuous (False)
         """
-        self.blog = _Blog("Whole Life Annuity",
-                         _Blog.a(x=x, s=s, t=Reserves.WHOLE, b=b, u=0,
-                                discrete=discrete, variance=False),
-                         levels=self.maxdepth)
+        self.blog = self.Blog("Whole Life Annuity",
+                              self.pprint.a(x=x, s=s, t=Reserves.WHOLE, b=b, u=0,
+                                            discrete=discrete, variance=False),
+                              levels=self.maxdepth)
         found = self._a_x(x, s=s, b=b, variance=variance, 
                           discrete=discrete, depth=self.maxdepth)
         if found is not None:
-            print(self.blog, end='')
+            self.blog.display()
             return found
         if not variance and self.interest.i > 0:  # (1) twin insurance shortcut
             A = self._A_x(x, s=s, b=b, discrete=discrete, depth=self.maxdepth)
             if A is not None:
-                self.blog("a_x = (1-A_x) / d",
+                self.blog(self.pprint.a(x=x, s=s, discrete=discrete, variance=variance),
+                          "= [1 -", self.pprint.A(x=x, s=s, discrete=discrete), "] / d",
                           depth=self.maxdepth, rule='insurance twin')
-                print(self.blog, end='')
+                self.blog.display()
                 return self.annuity_twin(A=A, discrete=discrete)
         a = super().whole_life_annuity(x, s=s, b=b, discrete=discrete,
                                        variance=variance)
         if a is not None:
-            print(self.blog, end='') 
+            self.blog.display() 
             return a
 
     def temporary_annuity(self, x: int, s: int = 0, t: int = Reserves.WHOLE,
                           b: int = 1, variance: bool = False,
                           discrete: bool = True) -> float:
-        """Compute temporary annuity a_x:t by calling recursion then twin first
+        """Compute temporary annuity a_x:t by attempting recursion then twin first
 
         Args:
           x : age of selection
           s : years after selection
           t : term of annuity in years
           b : annuity benefit amount
           variance (bool): return EPV (True) or variance (False)
           discrete : annuity due (True) or continuous (False)
         """
-        self.blog = _Blog("Temporary Annuity",
-                         _Blog.a(x=x, s=s, t=t, b=b, u=0,
-                                discrete=discrete, variance=variance),
-                         levels=self.maxdepth)
+        self.blog = self.Blog("Temporary Annuity",
+                              self.pprint.a(x=x, s=s, t=t, b=b, u=0,
+                                            discrete=discrete, variance=variance),
+                              levels=self.maxdepth)
         found = self._a_x(x, s=s, b=b, t=t, variance=variance, 
                           discrete=discrete, depth=self.maxdepth)
         if found is not None:
-            print(self.blog, end='')
+            self.blog.display()
             return found
         if not variance and self.interest.i > 0: # (1) twin insurance shortcut
             A = self._A_x(x, s=s, b=b, t=t, endowment=b, discrete=discrete, 
                           depth=self.maxdepth)
             if A is not None:
-                self.blog(_Blog.a(x=x, s=s, t=t), '= [ 1 -',
-                          _Blog.A(x=x, s=s, t=t), f"] / d(t={t})",
+                self.blog(self.pprint.a(x=x, s=s, t=t, b=b), '= [ 1 -',
+                          self.pprint.A(x=x, s=s, t=t, b=b, endowment=b), f"] / d",
                           #"Annuity twin: a = (1 - A) / d",
                           depth=self.maxdepth, rule='annuity twin')
-                print(self.blog, end='')
+                self.blog.display()
                 return self.annuity_twin(A=A, discrete=discrete)
         a = super().temporary_annuity(x, s=s, b=b, t=t, discrete=discrete,
                                       variance=variance)
         if a is not None:
-            print(self.blog, end='')
+            self.blog.display()
             return a
 
     def deferred_annuity(self, x: int, s: int = 0, t: int = Reserves.WHOLE,
                          u: int = 0, b: int = 1, discrete: bool = True) -> float:
-        """Compute deferred annuity u|a_x:t by calling recursion first
+        """Compute deferred annuity u|a_x:t by attempting recursion first
 
         Args:
           x : age of selection
           s : years after selection
           u : years deferred
           t : term of annuity in years
           b : annuity benefit amount
           discrete : annuity due (True) or continuous (False)
         """
-        self.blog = _Blog("Deferred Annuity",
-                         _Blog.a(x=x, s=s, t=t, b=b, u=u,
-                                discrete=discrete, variance=False),
-                         levels=self.maxdepth)
+        self.blog = self.Blog("Deferred Annuity",
+                              self.pprint.a(x=x, s=s, t=t, b=b, u=u,
+                                            discrete=discrete, variance=False),
+                              levels=self.maxdepth)
         a = self._a_x(x, s=s, b=b, t=t, u=u, 
-                          discrete=discrete, depth=self.maxdepth)
+                      discrete=discrete, depth=self.maxdepth)
         if a is not None:
-            print(self.blog, end='')
+            self.blog.display()
             return a
         a = self._a_x(x, s=s, b=b, t=self.add_term(u, t),  
                       discrete=discrete, depth=self.maxdepth)
         a_t = self._a_x(x, s=s, b=b, t=u,  
                         discrete=discrete, depth=self.maxdepth)
         if a is not None and a_t is not None:
-            print(self.blog, end='')
+            self.blog.display()
             return a - a_t
         return super().deferred_annuity(x, s=s, b=b, t=t, discrete=discrete)
 
-
-class _Blog:
-    """Helper to track and display recursion progress"""
-    _verbose : bool = True
-    def __init__(self, *args, levels: int = 3, width: int = 80):
-        self.title = ' *' + " ".join(args) + " <--"  # to identify this stack
-        self.levels = levels                         # maximum levels to indent
-        self.width = width - 3                       # display line width
-        self._history = []
-        self._rules = []
-        self._depths = []
-
-    def __call__(self, *args, depth: int | None = None, rule: str = ''):
-        """Append next message to history"""
-        assert depth is not None and rule, "depth and rule must be specified"
-        msg = " ".join([a for a in args]) 
-        if msg not in self._history:
-            self._history.insert(0, msg)
-            self._depths.insert(0, depth)
-            self._rules.insert(0, rule)
-
-    def __len__(self) -> int:
-        return int(_Blog._verbose and bool(self._history))
-
-    def __str__(self):
-        """Display message history"""
-        if not len(self):
-            return ''
-        _str = self.title + '\n'
-        for msg, depth, rule in zip(self._history, self._depths, self._rules):
-            left = ' '*(3+max(self.levels-abs(depth), 0))
-            right = ' '*max(5, self.width - len(msg) - len(left) - len(rule))
-            _str += left + msg + right + '~' + rule + '\n'
-        return _str
-
-    @staticmethod
-    def q(x: int, s: int = 0, t: int = 1, u: int = 0) -> str:
-        """Return string representation of mortality u|t_q_x term"""
-        out = []
-        if t != 1:
-            out.append(f"t={t}")
-        if u > 0:
-            out.append(f"defer={u}")
-        return f"q_{x+s}" + "("*bool(out) + ",".join(out) + ")"*bool(out)
-
-    @staticmethod
-    def p(x: int, s: int = 0, t: int = 1) -> str:
-        """Return string representation of survival t_p_x term"""
-        out = []
-        if t != 1:
-            out.append(f"t={t}")
-        return f"p_{x+s}" + "("*bool(out) + ",".join(out) + ")"*bool(out)
-
-
-    @staticmethod
-    def e(x: int, s: int = 0, t: int = Reserves.WHOLE, curtate: bool = False,
-          moment: int = 1) -> str:
-        """Return string representation of expected future lifetime e_x term"""
-        out = []
-        if t >= 0:
-            out.append(f"t={t}")
-        if moment != 1:
-            out.append(f"mom={moment}")
-        out.append('curtate' if curtate else 'complete')
-        return f"e_{x+s}" + "("*bool(out) + ",".join(out) + ")"*bool(out)
-
-    @staticmethod
-    def E(x: int, s: int = 0, t: int = 1, endowment: int = 1,
-          moment: int = 1) -> str:
-        """Return string representation of pure endowment t_E_x term"""
-        out = []
-        out.append(f"t={t if t >= 0 else 'WL'}")  # term or whole life
-        if moment != 1:
-            out.append(f"mom={moment}")
-        if endowment != 1:
-            out.append(f"endow={endowment}")
-        return f"E_{x+s}" + "("*bool(out) + ",".join(out) + ")"*bool(out)
-    
-    @staticmethod
-    def IA(x: int, s: int = 0, t: int = Reserves.WHOLE, b: int = 1,
-           discrete: bool = True) -> str:
-        """Return string representation of increasing insurance IA_x term"""
-        out = []
-        out.append(f"t={t if t >= 0 else 'WL'}")  # term or whole life
-        if b != 1:
-            out.append(f"b={b}")
-        return f"IA_{x+s}" + "("*bool(out) + ",".join(out) + ")"*bool(out)
-
-    @staticmethod
-    def DA(x: int, s: int = 0, t: int = Reserves.WHOLE, b: int = 1,
-           discrete: bool = True) -> str:
-        """Return string representation of decreasing insurance DA_x term"""
-        out = []
-        out.append(f"t={t if t >= 0 else 'WL'}")  # term or whole life
-        if b != 1:
-            out.append(f"b={b}")
-        return f"DA_{x+s}" + "("*bool(out) + ",".join(out) + ")"*bool(out)
-
-    @staticmethod
-    def A(x: int, s: int = 0, t: int = Reserves.WHOLE, u: int = 0, b: int = 1,
-          moment: int = 1, endowment: int = 0, discrete: bool = True) -> str:
-        """Return string representation of insurance A_x term"""
-        out = []
-        out.append(f"t={t if t >= 0 else 'WL'}")  # term or whole life
-        if u != 0:
-            out.append(f"u={u}")
-        if b != 1:
-            out.append(f"b={b}")
-        if endowment != 0:
-            out.append(f"endow={endowment}")
-        if moment != 1:
-            out.append(f"mom={moment}")
-        return f"A_{x+s}" + "("*bool(out) + ",".join(out) + ")"*bool(out)
-
-    @staticmethod
-    def a(x: int, s: int = 0, t: int = Reserves.WHOLE, u: int = 0, b: int = 1,
-          variance: bool = False, discrete: bool = True) -> str:
-        """Return string representation of annuity a_x term"""
-        out = []
-        out.append(f"t={t if t >= 0 else 'WL'}")  # term or whole life
-        if u != 0:
-            out.append(f"u={u}")
-        if b != 1:
-            out.append(f"b={b}")
-        if variance:
-            out.append('var')
-        return f"a_{x+s}" + "("*bool(out) + ",".join(out) + ")"*bool(out)
-
-    @staticmethod
-    def m(moment: int, **kwargs) -> str:
-        """Return string representation of moment exponent"""
-        out = f"^{moment}"*(moment != 1)
-        if not kwargs:
-            return out
-        args = [k for k,v in kwargs.items() if v]
-        return ("(" + "*".join(args) + ")")+out if args else "0"
-    
+# to auto-detect notebook environment
+try:
+    _shell = str(type(get_ipython())).lower()
+    if "colab" in _shell or "zmq" in _shell:
+        Recursion._Blog = PPrint
+        _Blog._notebook = True
+        _Blog._latex = True
+    else:
+        Recursion._Blog = _Blog
+        _Blog._notebook = False
+        _Blog._latex = False
+except:
+    pass
 
 if __name__ == "__main__":
     from actuarialmath.constantforce import ConstantForce
     from actuarialmath.policyvalues import Contract
 
     print("SOA Question 6.10: (D) 0.91")
     x = 0
```

### Comparing `actuarialmath-0.0.9/src/actuarialmath/reserves.py` & `actuarialmath-0.1.1/src/actuarialmath/reserves.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-"""Reserves - Computes recursive, interim and modified reserves
+"""Reserves - Computes recursive, interim or modified reserves
 
 MIT License. Copyright 2022-2023 Terence Lim
 """
 import math
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
 from typing import Callable, Dict, Any
 from actuarialmath import PolicyValues, Contract
 
 class Reserves(PolicyValues):
-    """Compute recursive, interim and modified reserves"""
-    
+    """Compute recursive, interim or modified reserves"""
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self._reserves = {'V': {}}
         self.T = 0
 
     #
     # Set up reserves table for recursion
@@ -24,14 +23,17 @@
                      V: Dict[int, float] | None = None) -> "Reserves":
         """Set values of the reserves table and the endowment benefit amount
 
         Args:
           T : max term of policy
           V : reserve values, keyed by time t
           endowment : endowment benefit amount
+
+        Examples:
+          >>> life = Reserves().set_reserves(T=3)
         """
         if T:
             self.T = T
         if V:
             self._reserves['V'].update(V)
             self.T = max(len(V) - 1, self.T)
         self._reserves['V'][0] = 0  # initial reserve is 0 by equivalence
@@ -76,24 +78,27 @@
 
     def V_plot(self, ax: Any = None, color: str = 'r', title: str = ''):
         """Plot values from reserves tables
 
         Args:
           title : title to display
           color : color to plot curve
+
+        Examples:
+          >>> life.V_plot(title=f"Reserves for term insurance")
         """
         if ax is None:
             fig, ax = plt.subplots(1, 1)
         y = [self._reserves['V'].get(t, None) for t in range(self.T + 1)]
         ax.plot(list(range(self.T + 1)), y, '.', color=color)
         ax.set_title(title)
         ax.set_ylabel(f"$_tV$", color=color)
         ax.set_xlabel(f"t")
 
-    def V_t(self):
+    def reserves_frame(self):
         """Returns reserves table as a DataFrame"""
         return pd.DataFrame(self._reserves)\
                  .rename_axis('t')\
                  .rename(columns={'V':'V_t'})
 
     #
     # Reserves recursion
@@ -165,14 +170,21 @@
           s : starting s years after selection
           t : year of reserve to solve
           benefit : benefit amount
           premium : amount of premium
           per_premium : expense per $ premium
           per_policy : expense per policy
           reserve_benefit : whether reserve value included in benefit
+
+        Examples:
+          >>> G, x = 368.05, 0
+          >>> def fun(P):  # solve net premium from expense reserve equation
+          >>>     return life.t_V(x=x, t=2, premium=G-P, benefit=lambda t: 0,
+          >>>                     per_policy=5+.08*G)
+          >>> P = life.solve(fun, target=-23.64, grid=[.29, .31]) / 1000
         """
         if t in self._reserves['V']:   # already solved in reserves table
             return self._reserves['V'][t]
         V = self.t_V_forward(x=x, s=s, t=t, premium=premium, 
                              benefit=benefit,
                              reserve_benefit=reserve_benefit, 
                              per_premium=per_premium,
```

### Comparing `actuarialmath-0.0.9/src/actuarialmath/selectlife.py` & `actuarialmath-0.1.1/src/actuarialmath/selectlife.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     """Calculate select life table, and iteratively fill in missing values
 
     Args:
       periods : number of select period years
       verbose : whether to echo update steps
 
     Notes:
-      6 types of information can be loaded and calculated in the select table:
+      6 types of columns can be loaded and calculated in the select table:
 
       - 'q' : probability [x]+s dies in one year
       - 'l' : number of lives aged [x]+s
       - 'd' : number of deaths of age [x]+s
       - 'A' : whole life insurance
       - 'a' : whole life annuity
       - 'e' : expected future curtate lifetime of [x]+s
@@ -38,30 +38,42 @@
         """Returns values from a select and ultimate table
 
         Args:
           table :  may be {'l', 'q', 'e', 'd', 'a', 'A'}
         """
         return self._select[table[0]]
 
-    def set_table(self, fill: bool = True,
+    def set_table(self,
                   l: Dict[int, List[float]] | None = None,
                   d: Dict[int, List[float]] | None = None, 
                   q: Dict[int, List[float]] | None = None,
                   A: Dict[int, List[float]] | None = None,
                   a: Dict[int, List[float]] | None = None, 
-                  e: Dict[int, List[float]] | None = None) -> "SelectLife":
+                  e: Dict[int, List[float]] | None = None,
+                  fill: bool = True,
+                  radix: int = LifeTable._RADIX) -> "SelectLife":
         """Update from table, every age has row for all select durations
 
         Args:
           q : probability [x]+s dies in one year
           l : number of lives aged [x]+s
           d : number of deaths of [x]+s
           A : whole life insurance, or
           a : whole life annuity, or 
           e : expected future lifetime of [x]+s
+          radix : initial number of lives
+          fill : whether to fill missing values using recursion formulas
+        
+        Examples:
+          >>> life = SelectLife().set_table(l={55: [10000, 9493, 8533, 7664],
+          >>>                                  56: [8547, 8028, 6889, 5630],
+          >>>                                  57: [7011, 6443, 5395, 3904],
+          >>>                                  58: [5853, 4846, 3548, 2210]},
+          >>>                               e={57: [None, None, None, 1]})
+          >>> print(life.e_r(58, s=2))
         """
         periods = self.periods_    # infer number of select years, and age range
         minage = self._MINAGE 
         maxage = self._MAXAGE
         
         for lbl, table in [('A',A), ('a',a), ('q',q), ('d',d), ('l',l), ('e',e)]:
             self._select[lbl] = {}
@@ -73,29 +85,35 @@
                     self._select[lbl][age] = {k:v for k,v in enumerate(row)}
 
         self.periods_ = periods    # update number of select years, and age range
         self._MINAGE = minage
         self._MAXAGE = maxage
 
         if fill:         # iteratively fill missing table values
-            self.fill_table()
+            self.fill_table(radix=radix)
         return self
 
-    def set_select(self, s: int, age_selected: bool, fill: bool = False,
+    def set_select(self,
+                   s: int,
+                   age_selected: bool,
+                   radix: int = LifeTable._RADIX,
+                   fill: bool = False,
                    l: Dict[int, float] | None = None,
                    d: Dict[int, float] | None = None,
                    q: Dict[int, float] | None = None,
                    A: Dict[int, float] | None = None,
                    a: Dict[int, float] | None = None,
                    e: Dict[int, float] | None = None) -> "SelectLife":
         """Update a table column, for a particular duration s in the select period
 
         Args:
           s : column to populate - n is ultimate, 0..n-1 is year after select
           age_selected : is indexed by age selected or actual (False, default)
+          radix : initial number of lives
+          fill : whether to fill missing values using recursion formulas
           q : probabilities [x]+s dies in next year, by age
           l : number of lives aged [x]+s, by age
           d : number of deaths of [x]+s, by age
           A : whole life insurance of [x]+s, by age
           a : whole life annuity of [x]+s, by age
           e : expected future lifetime of [x]+s, by age
         """
@@ -121,128 +139,128 @@
                     self._select[table][x][s] = item[age]
 
                     if self._MINAGE < 0 or x < self._MINAGE:  # infer min age
                         self._MINAGE = x
                     if age > self._MAXAGE:                    # infer max age
                         self._MAXAGE = x
         if fill:
-            self.fill_table()
+            self.fill_table(radix=radix)
         return self
 
-    def get_sel(self, x: int, s: int, table: str) -> float | None:
+    def _get_sel(self, x: int, s: int, table: str) -> float | None:
         """Helper to read right across, and down if neccesary (when s > n)"""
         if s > self.periods_:
             x += (s - self.periods_)
             s = self.periods_
         if (x in self._select[table] and s in self._select[table][x] 
             and self._select[table][x][s] is not None):
             return self._select[table][x][s]  # in select
 
-    def isin_sel(self, x: int, s: int, table: str) -> bool:
+    def _isin_sel(self, x: int, s: int, table: str) -> bool:
         """Helper to check if value not missing"""
-        return self.get_sel(x, s, table) is not None
+        return self._get_sel(x, s, table) is not None
 
     def fill_table(self, radix: int = LifeTable._RADIX) -> "SelectLife":
         """Fills in missing table values (does not check for consistency)
 
         Args:
           radix : initial number of lives
         """
         
         def A_x(x: int, s: int) -> float | None:
             """Helper to apply backward and forward recursion for insurance A_x"""
-            if self.isin_sel(x, s, 'A'):
-                return self.get_sel(x, s, 'A')
+            if self._isin_sel(x, s, 'A'):
+                return self._get_sel(x, s, 'A')
 
             _x, _s = (x, s+1) if s < self.periods_ else (x+1, s)  # right or down
-            if self.isin_sel(x, s, 'q') and self.isin_sel(_x, _s, 'A'):
-                q = self.get_sel(x, s, 'q')  # A_x = (v q) + (v p A_x+1)
-                return self.interest.v * (q + (1-q)*self.get_sel(_x, _s, 'A'))
+            if self._isin_sel(x, s, 'q') and self._isin_sel(_x, _s, 'A'):
+                q = self._get_sel(x, s, 'q')  # A_x = (v q) + (v p A_x+1)
+                return self.interest.v * (q + (1-q)*self._get_sel(_x, _s, 'A'))
 
             backwards = [(x, s-1)]   # to move backwards along row
             if s >= self.periods_:      # if in ultimate, can also move up column
                 backwards += [(x-1, s)]
             for _x, _s in backwards:   # A_x+1 = (A_x - qv) / (p v)
-                if self.isin_sel(_x, _s, 'q') and self.isin_sel(_x, _s, 'A'):
-                    q = self.get_sel(_x, _s, 'q')
-                    return ((self.get_sel(_x, _s, 'A') - q * self.interest.v)
+                if self._isin_sel(_x, _s, 'q') and self._isin_sel(_x, _s, 'A'):
+                    q = self._get_sel(_x, _s, 'q')
+                    return ((self._get_sel(_x, _s, 'A') - q * self.interest.v)
                             / (self.interest.v * (1 - q)))
 
         def a_x(x: int, s: int) -> float | None:
             """Helper to apply backward and forward recursion for annuity a_x"""
-            if self.isin_sel(x, s, 'a'):
-                return self.get_sel(x, s, 'a')
+            if self._isin_sel(x, s, 'a'):
+                return self._get_sel(x, s, 'a')
 
             _x, _s = (x, s+1) if s < self.periods_ else (x+1, s)  # right or down
-            if self.isin_sel(x, s, 'q') and self.isin_sel(_x, _s, 'a'):
-                p = 1 - self.get_sel(x, s, 'q')  # a_x = 1 +  (v p a_x+1)
-                return 1 + self.interest.v * p * self.get_sel(_x, _s, 'a')
+            if self._isin_sel(x, s, 'q') and self._isin_sel(_x, _s, 'a'):
+                p = 1 - self._get_sel(x, s, 'q')  # a_x = 1 +  (v p a_x+1)
+                return 1 + self.interest.v * p * self._get_sel(_x, _s, 'a')
 
             backwards = [(x, s-1)]  # to move backwards along row
             if s >= self.periods_:      # if in ultimate, can also move up column
                 backwards += [(x-1, s)]
             for _x, _s in backwards:   # a_x+1 = (a_x - 1) / (p v)
-                if self.isin_sel(_x, _s, 'q') and self.isin_sel(_x, _s, 'a'):
-                    p = 1 - self.get_sel(_x, _s, 'q')
-                    return (self.get_sel(_x, _s, 'a') - 1)/(p*self.interest.v)
+                if self._isin_sel(_x, _s, 'q') and self._isin_sel(_x, _s, 'a'):
+                    p = 1 - self._get_sel(_x, _s, 'q')
+                    return (self._get_sel(_x, _s, 'a') - 1)/(p*self.interest.v)
 
 
         def l_x(x: int, s: int) -> float | None:
             """Helper to solve for number of lives aged [x]+s: l_[x]+s"""
-            if self.isin_sel(x, s, 'l'):
-                return self.get_sel(x, s, 'l')
-            if self.isin_sel(x, s-1, 'l') and self.isin_sel(x, s-1, 'q'):
-                return self.get_sel(x, s-1, 'l')*(1 - self.get_sel(x, s-1, 'q'))
-            if self.isin_sel(x, s+1, 'l') and self.isin_sel(x, s, 'q'):
-                return self.get_sel(x, s+1, 'l') / (1 - self.get_sel(x, s, 'q'))
-            if self.isin_sel(x, s, 'd') and self.isin_sel(x, s, 'q'):
-                return self.get_sel(x, s, 'd') / self.get_sel(x, s, 'q')
+            if self._isin_sel(x, s, 'l'):
+                return self._get_sel(x, s, 'l')
+            if self._isin_sel(x, s-1, 'l') and self._isin_sel(x, s-1, 'q'):
+                return self._get_sel(x, s-1, 'l')*(1 - self._get_sel(x, s-1, 'q'))
+            if self._isin_sel(x, s+1, 'l') and self._isin_sel(x, s, 'q'):
+                return self._get_sel(x, s+1, 'l') / (1 - self._get_sel(x, s, 'q'))
+            if self._isin_sel(x, s, 'd') and self._isin_sel(x, s, 'q'):
+                return self._get_sel(x, s, 'd') / self._get_sel(x, s, 'q')
 
             backwards = [(x, s-1)]  # to move backwards along row
             if s >= self.periods_:     # if in ultimate, can also move up column
                 backwards += [(x-1, s)]
             for _x, _s in backwards:   # l_x+1 = l_x * p_x
-                if self.isin_sel(_x, _s, 'l') and self.isin_sel(_x, _s, 'q'):
-                    p = 1 - self.get_sel(_x, _s, 'q')
-                    return self.get_sel(_x, _s, 'l') * p
+                if self._isin_sel(_x, _s, 'l') and self._isin_sel(_x, _s, 'q'):
+                    p = 1 - self._get_sel(_x, _s, 'q')
+                    return self._get_sel(_x, _s, 'l') * p
 
         def d_x(x: int, s: int) -> float | None:
             """Helper to solve for deaths at [x]+s: l_[x]+s - l_[x]+s+1"""
-            if self.isin_sel(x, s, 'd'):
-                return self.get_sel(x, s, 'd')
-            if self.isin_sel(x, s+1, 'l') and self.isin_sel(x, s, 'l'):
-                return self.get_sel(x, s, 'l') - self.get_sel(x, s+1, 'l')
+            if self._isin_sel(x, s, 'd'):
+                return self._get_sel(x, s, 'd')
+            if self._isin_sel(x, s+1, 'l') and self._isin_sel(x, s, 'l'):
+                return self._get_sel(x, s, 'l') - self._get_sel(x, s+1, 'l')
 
         def q_x(x: int, s: int) -> float | None:
             """Helper to solve for one-year mortality [x]+s: q_[x]+s"""
-            if self.isin_sel(x, s, 'q'):
-                return self.get_sel(x, s, 'q')
-            if self.isin_sel(x, s, 'd') and self.isin_sel(x, s, 'l'):
-                return self.get_sel(x, s, 'd') / self.get_sel(x, s, 'l')
-            if self.isin_sel(x, s, 'e') and self.isin_sel(x, s+1, 'e'):
-                return 1 - (self.get_sel(x, s, 'e') 
-                            / (1 + self.get_sel(x, s+1, 'e')))
+            if self._isin_sel(x, s, 'q'):
+                return self._get_sel(x, s, 'q')
+            if self._isin_sel(x, s, 'd') and self._isin_sel(x, s, 'l'):
+                return self._get_sel(x, s, 'd') / self._get_sel(x, s, 'l')
+            if self._isin_sel(x, s, 'e') and self._isin_sel(x, s+1, 'e'):
+                return 1 - (self._get_sel(x, s, 'e') 
+                            / (1 + self._get_sel(x, s+1, 'e')))
 
         def e_x(x: int, s: int) -> float | None:
             """Helper to solve for expected kurtate lifetime: e_[x]+s"""
-            if self.isin_sel(x, s, 'e'):
-                return self.get_sel(x, s, 'e')
+            if self._isin_sel(x, s, 'e'):
+                return self._get_sel(x, s, 'e')
 
             _x, _s = (x, s+1) if s < self.periods_ else (x+1, s) # right or down
-            if self.isin_sel(x, s, 'q') and self.isin_sel(_x, _s, 'e'):
-                return ((1 - self.get_sel(x, s, 'q'))
-                        * (1 + self.get_sel(_x, _s, 'e')))  # e_x = p(1 + e_x+1)
+            if self._isin_sel(x, s, 'q') and self._isin_sel(_x, _s, 'e'):
+                return ((1 - self._get_sel(x, s, 'q'))
+                        * (1 + self._get_sel(_x, _s, 'e')))  # e_x = p(1 + e_x+1)
 
             backwards = [(x, s-1)]  # to move backwards along row
             if s >= self.periods_:     # if in ultimate, can also move up column
                 backwards += [(x-1, s)]
             for _x, _s in backwards:   # e_x+1 = e_x/p_x - 1
-                if self.isin_sel(_x, _s, 'e') and self.isin_sel(_x, _s, 'q'):
-                    return (self.get_sel(_x, _s, 'e') 
-                            / (1 - self.get_sel(_x, _s, 'q'))) - 1
+                if self._isin_sel(_x, _s, 'e') and self._isin_sel(_x, _s, 'q'):
+                    return (self._get_sel(_x, _s, 'e') 
+                            / (1 - self._get_sel(_x, _s, 'q'))) - 1
 
         # Iterate a few times to impute select table values
         funs = {'l': l_x, 'A': A_x, 'a': a_x, 'q': q_x, 'd': d_x, 'e': e_x}
         curr = 0   # number of updates filled in
         for loop in range(2):   # loop second time if need to assume radix
             prev = curr - 1
             while curr != prev:        # continue while changes made
@@ -250,15 +268,15 @@
                 for tab, fun in funs.items():   # for each table
                     if tab not in self._select:
                         self._select[tab] = {}
                     for x in range(self._MINAGE, self._MAXAGE + 1):  # for each age
                         if x not in self._select[tab]:
                             self._select[tab][x] = {}
                         for s in range(self.periods_+1): # each year after select
-                            if not self.isin_sel(x, s, tab):
+                            if not self._isin_sel(x, s, tab):
                                 val = fun(x, s)
                                 if val is not None:
                                     self._select[tab][x][s] = val
                                     curr += 1
                                     if self._verbose:
                                         print(f"{curr} {tab}(x={x}, s={s}) = {val}")
             if 0 not in self._select['l'][self._MINAGE]: # arbitrary initial lives
@@ -270,51 +288,51 @@
         """Returns insurance value computed from select table
 
         Args:
           x : age of selection
           s : years after selection
         """
         assert moment == 1 and discrete, "Must be discrete insurance"
-        if self.isin_sel(x, s, 'A'):
-            return self.get_sel(x, s, 'A')
+        if self._isin_sel(x, s, 'A'):
+            return self._get_sel(x, s, 'A')
         else:
             return super().A_x(x=x, s=s, moment=1, discrete=True, **kwargs)
 
     def a_x(self, x: int, s: int = 0, moment: int = 1, discrete: bool = True,
             **kwargs) -> float:
         """Returns annuity value computed from select table
 
         Args:
           x : age of selection
           s : years after selection
         """
         assert moment == 1 and discrete, "Must be discrete annuity"
-        if self.isin_sel(x, s, 'a'):
-            return self.get_sel(x, s, 'a')
+        if self._isin_sel(x, s, 'a'):
+            return self._get_sel(x, s, 'a')
         else:
             return super().A_x(x=x, s=s, moment=1, discrete=True, **kwargs)
 
     def l_x(self, x: int, s: int = 0) -> float:
         """Returns number of lives aged [x]+s computed from select table
 
         Args:
           x : age of selection
           s : years after selection
         """
-        return self.get_sel(x, s, 'l')
+        return self._get_sel(x, s, 'l')
 
     def p_x(self, x: int, s: int = 0, t: int = 1) -> float:
         """t_p_[x]+s by chain rule: prod(1_p_[x]+s+y) for y in range(t)
 
         Args:
           x : age of selection
           s : years after selection
           t : survives t years
         """
-        return np.prod([1 - self.get_sel(x, s+y, 'q') for y in range(t)])
+        return np.prod([1 - self._get_sel(x, s+y, 'q') for y in range(t)])
 
     def q_x(self, x: int, s: int = 0, t: int = 1, u: int = 0) -> float:
         """t|u_q_[x]+s = [x]+s survives u years, does not survive next t
 
         Args:
           x : age of selection
           s : years after selection
@@ -329,24 +347,32 @@
 
         Args:
           x : age of selection
           s : years after selection
           t : limit of expected future lifetime
         """
         assert curtate, "Must be curtate lifetimes"
-        if (self.isin_sel(x, s, 'e')):
-            return self.get_sel(x, s, 'e')
+        if (self._isin_sel(x, s, 'e')):
+            return self._get_sel(x, s, 'e')
         e = sum([self.p_x(x, s=s, t=k+1) for k in range(max(1, t))])
         return e
 
     def frame(self, table: str = 'l') -> pd.DataFrame:
         """Returns select and ultimate table values as a DataFrame
 
         Args:
           table : table to return, one of ['A', 'a', 'q', 'd', 'e', 'l']
+
+        Examples:
+          >>> table={21: [.00120, .00150, .00170, .00180],
+          >>>        22: [.00125, .00155, .00175, .00185],
+          >>>        23: [.00130, .00160, .00180, .00195]}
+          >>> life = SelectLife(verbose=True).set_table(q=table)
+          >>> print(life.frame('l').round(1))
+          >>> print(life.frame('q').round(6))
         """
         return pd.DataFrame.from_dict(self._select[table[0]], orient='index')\
                            .sort_index(axis=0)\
                            .sort_index(axis=1)\
                            .rename_axis('Age')\
                            .rename_axis(table[0] + '_[x]+s:', axis=1)
```

### Comparing `actuarialmath-0.0.9/src/actuarialmath/sult.py` & `actuarialmath-0.1.1/src/actuarialmath/sult.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,14 +18,21 @@
 
     Args:
       i : interest rate
       radix : initial number of lives
       minage : minimum age
       maxage : maximum age
       S : survival function, default is Makeham with SOA FAM-L parameters
+
+    Examples:
+      >>> sult = SULT()
+      >>> a = sult.temporary_annuity(70, t=10)
+      >>> A = sult.deferred_annuity(70, u=10)
+      >>> P = sult.gross_premium(a=a, A=A, benefit=100000, initial_premium=0.75,
+      >>>                        renewal_premium=0.05)
     """
 
 
     def __init__(self, i: float = 0.05, radix: int = 100000, 
                  S: Callable[[float, float], float] = _faml_sult,
                  minage: int = 20, maxage: int = 130, **kwargs):
         """Construct SULT"""
```

### Comparing `actuarialmath-0.0.9/src/actuarialmath/survival.py` & `actuarialmath-0.1.1/src/actuarialmath/survival.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,68 +12,78 @@
     _RADIX = 100000   # default initial number of lives in life table
 
     def set_survival(self,
                      S: Callable[[int,float,float], float] | None = None, 
                      f: Callable[[int,float,float], float] | None = None,
                      l: Callable[[int,float], float] | None = None, 
                      mu: Callable[[int,float], float] | None = None,
-                     maxage: int = Life._MAXAGE,
-                     minage: int = Life._MINAGE) -> "Survival":
+                     minage: int = 0, maxage: int = 1000) -> "Survival":
         """Construct the basic survival and mortality functions given any one form
 
         Args:
           S : probability [x]+s survives t years
-          f : or mortality of [x]+s after t years 
+          f : or lifetime density function of [x]+s after t years 
           l : or number of lives aged (x+t)
           mu : or force of mortality at age (x+t)
           maxage : maximum age
           minage : minimum age
+
+        Examples:
+
+        >>> B, c = 0.00027, 1.1
+        >>> def S(x,s,t): return (math.exp(-B * c**(x+s) * (c**t - 1)/math.log(c)))
+        >>> life = Survival().set_survival(S=S)
+
+        >>> def ell(x,s): return (1 - (x+s) / 60)**(1 / 3)
+        >>> life = Survival().set_survival(l=ell)
         """
+        assert(any([S, f, l, mu])), "One form of survival function must be specified"
         self._MAXAGE = maxage
         self._MINAGE = minage
         self.S = None   # survival probability: Prob(T_[x]+s > t)
         self.f = None   # lifetime density: f_[x]+s(t) ~ Prob[([x]+s) dies at t]
         self.l = None   # number of lives aged [x]+s: l_[x]+s
         self.mu = None  # force of mortality: mu_(x+t)
 
         def S_from_l(x: int, s, t: float) -> float:
             """Derive survival probability from number of lives"""
             return (self.l(x, s+t) / self.l(x, s)) if self.l(x, s) else 0.
 
         def mu_from_l(x: int, t: float) -> float:
             """Derive force of mortality from number of lives"""
-            return -self.derivative(lambda s: math.log(self.l(x, s)), t)
+            return -self.derivative(lambda s: self.l(x, s), t) / self.l(x,t)
 
         def f_from_l(x: int, s, t: float) -> float:
             """Derive lifetime density function from number of lives"""
             return -self.derivative(lambda t: self.l(x, s+t), t)
 
         def mu_from_S(x: int, t: float) -> float:
             """Derive force of mortality from survival probability"""
-            return -self.derivative(lambda s: math.log(self.S(x, 0, s)), t)
+            return -self.derivative(lambda s: self.S(x, 0, s), t) / self.S(x,0,t)
 
         def f_from_S(x: int, s, t: float) -> float:
             """Derive lifetime density function from survival probability"""
             return -self.derivative(lambda t: self.S(x, s, t), t)
 
         def S_from_mu(x: int, s, t: float) -> float:
             """Derive survival probability from force of mortality"""
-            return math.exp(-self.integral(lambda t: self.mu(x, s+t), 0, t))
+            return math.exp(-self.integral(lambda t: self.mu(x, s+t),
+                                           lower=0, upper=t))
 
         def S_from_f(x: int, s, t: float) -> float:
             """Derive survival probability from lifetime density function"""
-            return 1 - self.integral(lambda t: self.f(x, s, t), 0, t)
+            return 1 - self.integral(lambda t: self.f(x, s, t), lower=0, upper=t)
 
         def f_from_mu(x: int, s, t: float) -> float:
             """Derive lifetime density function from force of mortality"""
             return self.S(x, s, t) * self.mu(x, s+t)
 
         def mu_from_f(x: int, t: float) -> float:
             """Derive force of mortality from lifetime density function"""
-            self.mu = self.f(x, 0, t) / self.S(x, 0, t)
+            return self.f(x, 0, t) / self.S(x, 0, t)
 
         # derive and set all forms of basic survival and mortality functions
         if l is not None:
             assert callable(l), "l must be callable"
             self.S = S_from_l
             self.mu = mu_from_l
             self.f = f_from_l
@@ -106,15 +116,15 @@
           x : age of selection
           s : years after selection
         """
         assert x >= 0, "x must be non-negative"
         assert s >= 0, "s must be non-negative"
         if self.l is not None:
             return self.l(x, s)
-        return Life.LIFES * self.p_x(x=self._MINAGE, s=0, t=s+x-self._MINAGE)
+        return self._RADIX * self.p_x(x=self._MINAGE, s=0, t=s+x-self._MINAGE)
 
     def d_x(self, x: int, s: int = 0) -> float:
         """Number of deaths at integer age [x]+s: d_[x]+s
 
         Args:
           x : age of selection
           s : years after selection
@@ -141,26 +151,37 @@
         """Probability that [x]+s lives for u, but not t+u years: u|t_q_[x]+s
 
         Args:
           x : age of selection
           s : years after selection
           u : survives u years, then
           t : dies within next t years
+
+        Examples:
+
+        >>> def ell(x,s): return (1-((x+s)/250)) if x+s < 40 else (1-((x+s)/100)**2)
+        >>> q = Survival().set_survival(l=ell).q_x(30, t=20)
         """
         assert x >= 0, "x must be non-negative"
         assert s >= 0, "s must be non-negative"
         return self.p_x(x, s=s, t=u) - self.p_x(x, s=s, t=t+u)
 
     def f_x(self, x: int, s: int = 0, t: int = 0) -> float:
         """Lifetime density function of [x]+s after t years: f_[x]+s(t)
 
         Args:
           x : age of selection
           s : years after selection
           t : dies at year t
+
+        Examples:
+
+        >>> B, c = 0.00027, 1.1
+        >>> def S(x,s,t): return (math.exp(-B * c**(x+s) * (c**t - 1)/math.log(c)))
+        >>> f = Survival().set_survival(S=S).f_x(x=50, t=10)
         """
         assert x >= 0, "x must be non-negative"
         assert s >= 0, "s must be non-negative"
         if self.f is not None:
             return self.f(x, s, t)
         return self.p_x(x, s=s, t=t) * self.mu_x(x, s=s, t=t)
 
@@ -169,17 +190,16 @@
 
         Args:
           x : age of selection
           s : years after selection
           t : force of mortality at year t
 
         Examples:
-          >>> def S(x, s): return (1 - (x+s) / 60)**(1 / 3)
-          >>> print(Survival().set_survival(l=S).mu_x(35))
-
+          >>> def ell(x, s): return (1 - (x+s) / 60)**(1 / 3)
+          >>> print(Survival().set_survival(l=ell).mu_x(35))
         """
         assert x >= 0, "x must be non-negative"
         assert s >= 0, "s must be non-negative"
         if self.mu is not None:
             return self.mu(x, s+t)
         return self.f_x(x, s=s, t=t) / self.p_x(x, s=s, t=t)
 
@@ -202,22 +222,22 @@
     print("SOA Question 2.3: (A) 0.0483")
     B, c = 0.00027, 1.1
     def S(x,s,t): return (math.exp(-B * c**(x+s) * (c**t - 1)/math.log(c)))
     f = Survival().set_survival(S=S).f_x(x=50, t=10)
     print(f)
     
     print("SOA Question 2.6: (C) 13.3")
-    def S(x, s): return (1 - (x+s) / 60)**(1 / 3)
-    mu = Survival().set_survival(l=S).mu_x(35) * 1000
+    def ell(x,s): return (1 - (x+s) / 60)**(1 / 3)
+    mu = Survival().set_survival(l=ell).mu_x(35) * 1000
     print(mu)
 
     print("SOA Question 2.7: (B) 0.1477")
-    def S(x, s): return (1 - ((x+s)/250)) if x+s < 40 else (1 - ((x+s)/100)**2)
-    q = Survival().set_survival(l=S).q_x(30, t=20)
+    def ell(x,s): return (1 - ((x+s)/250)) if x+s < 40 else (1 - ((x+s)/100)**2)
+    q = Survival().set_survival(l=ell).q_x(30, t=20)
     print(q)
 
     print("CAS41-F99:12: k = 41")
-    def mu_from_l(k):
-        def S(x, s): return 100*(k - 0.5*(x+s))**(2/3)
-        return Survival().set_survival(l=S).mu_x(50)
-    k = int(Survival.solve(mu_from_l, target=1/48, grid=50))
-    print(k)
+    def fun(k):
+        return Survival().set_survival(l=lambda x,s: 100*(k - (x+s)/2)**(2/3))\
+                         .mu_x(50)
+    print(Survival.solve(fun, target=1/48, grid=50))
+
```

### Comparing `actuarialmath-0.0.9/src/actuarialmath/woolhouse.py` & `actuarialmath-0.1.1/src/actuarialmath/woolhouse.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,34 +10,34 @@
 class Woolhouse(Mthly):
     """1/m'thly shortcuts with Woolhouse approximation
 
     Args:
       m : number of payments per year
       life : original fractional survival and mortality functions
       three_term : whether to include (True) or ignore (False) third term
-      approximate_mu : function to approximate mu_x for third term
+      approximate_mu : exact (False), approximate (True) or function for third term
     """
     
     def __init__(self, m: int, life: Annuity, three_term: bool = False,
                  approximate_mu: Callable[[int, int], float] | bool = True):
         super().__init__(m=m, life=life)
         self.three_term = three_term          # whether to include third term
-        self.approximate_mu = approximate_mu  # whether to approximate mu
+        self.approximate_mu = approximate_mu  # how to approximate mu
 
     def mu_x(self, x: int, s: int = 0) -> float:
-        """Approximates or computes mu_x for third term
+        """Computes mu_x or calls approximate_mu for third term
 
         Args:
           x : age of selection
           s : years after selection
         """
-        if self.approximate_mu is True:       # approximate mu
+        if self.approximate_mu is True:       # approximate mu from integer ages
             return -.5 * sum([math.log(self.life.p_x(x, s=s+t)) for t in [0,-1]])
         elif self.approximate_mu is False:
-            return self.life.mu_x(x, s=s)     # use exact mu
+            return self.life.mu_x(x, s=s)     # use exact mu from survival model
         else:                                 # apply custom function for mu
             return self.approximate_mu(x, s)
 
     def whole_life_insurance(self, x: int, s: int = 0, b: int = 1,
                              mu: float | None = 0.) -> float:
         """1/m'thly Woolhouse whole life insurance: A_x
  
@@ -112,14 +112,18 @@
         """1/m'thly Woolhouse whole life annuity: a_x
 
         Args:
           x : year of selection
           s : years after selection
           b : amount of benefit
           mu : value of mu at age x+s
+
+        Examples:
+          >>> life = Recursion().set_interest(i=0.05).set_a(3.4611, x=0)
+          >>> Woolhouse(m=4, life=life).whole_life_annuity(x=0)
         """
         a = (self.life.whole_life_annuity(x, s=s, discrete=True) -
              (self.m - 1)/(2 * self.m))
         if self.three_term:
             mu = mu or self.mu_x(x, s)
             a -= (mu + self.life.interest.delta)*(self.m**2 - 1)/(12 * self.m**2)
         return a * b
```

### Comparing `actuarialmath-0.0.9/src/actuarialmath.egg-info/PKG-INFO` & `actuarialmath-0.1.1/src/actuarialmath.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: actuarialmath
-Version: 0.0.9
+Version: 0.1.1
 Summary: A package for actuarial math and life contingent risks
 Author: Terence Lim
 Project-URL: Homepage, https://terence-lim.github.io/actuarialmath-guide
 Project-URL: Bug Tracker, https://github.com/terence-lim/actuarialmath/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -35,19 +35,19 @@
 
    - Extra mortality risks
 
    - 1/mthly payment frequency using UDD or Woolhouse approaches
 
 3. Specify and load a particular form of assumptions
 
+   - Recursion inputs
+
    - Life table, select life table, or standard ultimate life table
 
    - Mortality laws, such as constant force of maturity, beta and uniform distributions, or Makeham's and Gompertz's laws
-
-   - Recursion inputs
     
      
 Quick Start
 -----------
 
 1. ``pip install actuarialmath``
    
@@ -63,29 +63,29 @@
 
 Examples
 --------
 
 ::
 
   # SOA FAM-L sample question 5.7
-  from actuarialmath.recursion import Recursion, Woolhouse
+  from actuarialmath import Recursion, Woolhouse
   # initialize Recursion class with actuarial inputs
   life = Recursion().set_interest(i=0.04)\
                     .set_A(0.188, x=35)\
                     .set_A(0.498, x=65)\
                     .set_p(0.883, x=35, t=30)
   # modfy the standard results with Woolhouse mthly approximation
   mthly = Woolhouse(m=2, life=life, three_term=False)
   # compute the desired temporary annuity value
   print(1000 * mthly.temporary_annuity(35, t=30)) #   solution = 17376.7
 
 ::
 
   # SOA FAM-L sample question 7.20
-  from actuarialmath.sult import SULT, Contract
+  from actuarialmath import SULT, Contract
   life = SULT()
   # compute the required FPT policy value
   S = life.FPT_policy_value(35, t=1, b=1000)  # is always 0 in year 1!
   # input the given policy contract terms
   contract = Contract(benefit=1000,
                       initial_premium=.3,
                       initial_policy=300,
@@ -98,13 +98,13 @@
   print(R-S)   # solution = -277.19
 
 Resources
 ---------
 
 1. `Colab <https://colab.research.google.com/drive/1TcNr1x5HbT2fF3iFMYGXdN_cvRKiSua4?usp=sharing>`_ or `Jupyter notebook <https://terence-lim.github.io/notes/faml.ipynb>`_, to solve all sample SOA FAM-L exam questions
 
-2. `User Guide <https://terence-lim.github.io/actuarialmath-guide/>`_, or `download pdf <https://terence-lim.github.io/notes/actuarialmath-guide.pdf>`_
+2. `Online User Guide <https://terence-lim.github.io/actuarialmath-guide/>`_, or `download pdf <https://terence-lim.github.io/notes/actuarialmath-guide.pdf>`_
 
-3. `Code documentation <https://actuarialmath.readthedocs.io/en/latest/>`_
+3. `API reference <https://actuarialmath.readthedocs.io/en/latest/>`_
 
 4. `Github repo <https://github.com/terence-lim/actuarialmath.git>`_ and `issues <https://github.com/terence-lim/actuarialmath/issues>`_
```

### Comparing `actuarialmath-0.0.9/src/actuarialmath.egg-info/SOURCES.txt` & `actuarialmath-0.1.1/src/actuarialmath.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `actuarialmath-0.0.9/tests/test_changes.py` & `actuarialmath-0.1.1/tests/test_changes.py`

 * *Files identical despite different names*

