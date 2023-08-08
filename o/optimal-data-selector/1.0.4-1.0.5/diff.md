# Comparing `tmp/optimal_data_selector-1.0.4.tar.gz` & `tmp/optimal_data_selector-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optimal_data_selector-1.0.4.tar", last modified: Sat Aug  5 16:37:17 2023, max compression
+gzip compressed data, was "optimal_data_selector-1.0.5.tar", last modified: Tue Aug  8 15:32:21 2023, max compression
```

## Comparing `optimal_data_selector-1.0.4.tar` & `optimal_data_selector-1.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-08-05 16:37:17.643789 optimal_data_selector-1.0.4/
--rw-rw-rw-   0        0        0        0 2023-07-13 10:41:27.000000 optimal_data_selector-1.0.4/LICENSE
--rw-rw-rw-   0        0        0      951 2023-08-05 16:37:17.631792 optimal_data_selector-1.0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-05 16:37:17.315384 optimal_data_selector-1.0.4/optimal_data_selector/
--rw-rw-rw-   0        0        0        0 2023-07-13 09:41:50.000000 optimal_data_selector-1.0.4/optimal_data_selector/__init__.py
--rw-rw-rw-   0        0        0     9647 2023-07-13 14:26:26.000000 optimal_data_selector-1.0.4/optimal_data_selector/optimal.py
--rw-rw-rw-   0        0        0        0 2023-07-13 09:28:13.000000 optimal_data_selector-1.0.4/optimal_data_selector/optimal_2.py
--rw-rw-rw-   0        0        0     4732 2023-08-05 16:34:28.000000 optimal_data_selector-1.0.4/optimal_data_selector/word.py
-drwxrwxrwx   0        0        0        0 2023-08-05 16:37:17.556201 optimal_data_selector-1.0.4/optimal_data_selector.egg-info/
--rw-rw-rw-   0        0        0      951 2023-08-05 16:37:15.000000 optimal_data_selector-1.0.4/optimal_data_selector.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      328 2023-08-05 16:37:15.000000 optimal_data_selector-1.0.4/optimal_data_selector.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-05 16:37:15.000000 optimal_data_selector-1.0.4/optimal_data_selector.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-08-05 16:37:15.000000 optimal_data_selector-1.0.4/optimal_data_selector.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-05 16:37:17.644791 optimal_data_selector-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1253 2023-08-05 16:36:27.000000 optimal_data_selector-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-08 15:32:21.230943 optimal_data_selector-1.0.5/
+-rw-rw-rw-   0        0        0        0 2023-07-13 10:41:27.000000 optimal_data_selector-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0      985 2023-08-08 15:32:21.228945 optimal_data_selector-1.0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-08 15:32:21.179975 optimal_data_selector-1.0.5/optimal_data_selector/
+-rw-rw-rw-   0        0        0        0 2023-07-13 09:41:50.000000 optimal_data_selector-1.0.5/optimal_data_selector/__init__.py
+-rw-rw-rw-   0        0        0    11100 2023-08-08 14:54:53.000000 optimal_data_selector-1.0.5/optimal_data_selector/optimal.py
+-rw-rw-rw-   0        0        0        0 2023-07-13 09:28:13.000000 optimal_data_selector-1.0.5/optimal_data_selector/optimal_2.py
+-rw-rw-rw-   0        0        0     5054 2023-08-08 15:19:01.000000 optimal_data_selector-1.0.5/optimal_data_selector/word.py
+drwxrwxrwx   0        0        0        0 2023-08-08 15:32:21.223946 optimal_data_selector-1.0.5/optimal_data_selector.egg-info/
+-rw-rw-rw-   0        0        0      985 2023-08-08 15:32:20.000000 optimal_data_selector-1.0.5/optimal_data_selector.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      328 2023-08-08 15:32:21.000000 optimal_data_selector-1.0.5/optimal_data_selector.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 15:32:20.000000 optimal_data_selector-1.0.5/optimal_data_selector.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-08-08 15:32:20.000000 optimal_data_selector-1.0.5/optimal_data_selector.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-08 15:32:21.230943 optimal_data_selector-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1287 2023-08-08 15:29:06.000000 optimal_data_selector-1.0.5/setup.py
```

### Comparing `optimal_data_selector-1.0.4/PKG-INFO` & `optimal_data_selector-1.0.5/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: optimal_data_selector
-Version: 1.0.4
-Summary: A Package for to optimize models
+Version: 1.0.5
+Summary: A Package for to optimize models, use for nlp short word treatment
 Author: Rohan Majumder
 Author-email: majumderrohan2001@gmail.com
 Keywords: get_best_data_combination,optimise_accuracy,lock_data_combination,gives_best_result,best_data_for_ML_models,works on text data also,short word treatment
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `optimal_data_selector-1.0.4/optimal_data_selector/optimal.py` & `optimal_data_selector-1.0.5/optimal_data_selector/optimal.py`

 * *Files 12% similar despite different names*

```diff
@@ -63,14 +63,15 @@
         from sklearn.preprocessing import MinMaxScaler,StandardScaler
         from sklearn.linear_model import LogisticRegression,LinearRegression,Ridge
         from sklearn.svm import SVC
         from sklearn.tree import DecisionTreeClassifier,DecisionTreeRegressor
         from sklearn.naive_bayes import GaussianNB
         import time
         import warnings
+        import scipy
         warnings.filterwarnings('ignore')
         if scaling == 'normal':
             minmax=MinMaxScaler()
             X=minmax.fit_transform(X)
         elif scaling == 'st_normal':
             std=StandardScaler()
             X=std.fit_transform(X)
@@ -180,11 +181,44 @@
             y_test1=x_train[a][3]
             end1=time.time()
             if acc_forecast == True:
                 print('The accuracy is '+str(max(i4)))
             if time_forecast == True:
                 print('Computation time = '+str((end1-start1)/60),' mints')
             return x_train1,x_test1,y_train1,y_test1
+        
+
+        elif type(predictor) == scipy.sparse._csr.csr_matrix and bs_problem == 'class' and boost == False:
+            start22 = time.time()
+            for i in range(random_state,random_state+combination):
+                x_train1,x_test1,y_train1,y_test1=train_test_split(X,Y,train_size=train_size,random_state=i,shuffle=randomness)
+                x_train.append([x_train1,y_train1,x_test1,y_test1])
+                log=LogisticRegression()
+                svm=SVC()
+                dis=DecisionTreeClassifier(random_state=random_state)
+                clas=[log,svm,dis]
+            for x in x_train:
+                for c in clas:
+                    c.fit(x[0],x[1])
+                    acc.append(c.score(x[2],x[3]))  
+            for i in range(0, len(acc), 3):
+                chunk = acc[i:i+3]
+                i3.append(chunk)
+            for i in i3:
+                i4.append(sum(i)/len(i))
+                a=i4.index(max(i4))
+            x_train1=x_train[a][0]
+            x_test1=x_train[a][2]
+            y_train1=x_train[a][1]
+            y_test1=x_train[a][3]
+            end22=time.time()
+            if acc_forecast == True:
+                print('The accuracy is '+str(max(i4)))
+            if time_forecast == True:
+                print('Computation time = '+str((end22-start22)/60),' mints')
+            return x_train1,x_test1,y_train1,y_test1
+                
+
         elif bs_problem !='class' or bs_problem !='reg':
             print("you have input a wrong value as bs_problem")
     except Exception as ex:
         print('Error : '+str(ex))
```

### Comparing `optimal_data_selector-1.0.4/optimal_data_selector/word.py` & `optimal_data_selector-1.0.5/optimal_data_selector/word.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,48 +1,57 @@
-def short_word_treatment(text,add_words=False,word=None,remove_words=None,mostly_used_shortwords=False):
-    '''This function takes a text input and processes it to expand commonly used short words or acronyms
-    into their full forms. It also provides options to add custom short words and their corresponding full
-    forms, remove existing short words, and display the most frequently used short words.
+def short_word_treatment(text,add_words=False,word=None,remove_words=None,remove_all=False):
+    '''*** Before using it make sure that 'nltk' package is installed
+          *** Before using run these codes***
+
+          --> import nltk
+          --> nltk.download('punkt')
+
+    ABOUT:
+        This function takes a text input and processes it to expand commonly used short words or acronyms
+        into their full forms. It also provides options to add custom short words and their corresponding full
+        forms, remove existing short words, and display the most frequently used short words.
 
     Parameters:
         text (str): The input text to be processed.
 
         add_words (bool): If True, additional custom short words and their corresponding full forms
                           will be added . Default is False.
 
         word (dict): A dictionary containing custom short words as keys and their corresponding full
                      forms as values. This parameter is used when add_words is set to True. Default is None.
 
         remove_words (list): A list of short words to be removed . Default is None.
+        
+        remove_all (bool): If True, the function will remove all the predefine short words, by using this parameter you can
+                           use your own short words only, If False then the function will use all the pre and userdefine 
+                           short words during the treatment 
+
 
-        mostly_used_shortwords (bool): If True, the function will display the most frequently used
-                                       short words and their occurrence counts. Default is False.
 
     Returns:
         str: The processed text with short words expanded into their full forms.
 
     Example:
         input_text = "OMG, BTW IRL, JK! LOL"
-        expanded_text = short_word_treatment(input_text, mostly_used_shortwords=True)
+        expanded_text = short_word_treatment(input_text)
         print(expanded_text)
     Notes:
-        If the function is not working to the Pc then install nltk package and try again    
+        If the function is not working to the Pc then install nltk package and try again
 
     Output:
         "Oh my God, By the way In real life, Just kidding! Laugh out loud" '''
 
 
     try:
-      import nltk
-      nltk.download('punkt')
       from nltk import word_tokenize
       from collections import Counter
       import pandas as pd
       import warnings
       warnings.filterwarnings('ignore')
+
       d={'LOL': 'Laugh out loud',
       'BRB': 'Be right back',
       'OMG': 'Oh my God',
       'TTYL': 'Talk to you later',
       'BTW': 'By the way',
       'SMH': 'Shaking my head',
       'IMO': 'In my opinion',
@@ -82,41 +91,52 @@
       'COMP':'Competition',
       'R'  : 'Are',
       'TBH': 'To be honest','CAJ':'Casual','OFC':' Of course','TBF':'To be fair','IKR':'I know, right','STFU':'Shut the fuck up','TMB':'Text me back',
       'R8' : 'Right','SRY':'Sorry','GJ':'Good job','W8AM':' Wait a minute','PIC':'Picture','KK':'Okay cool','GM':'Good morning','L8R':'Later',
       'BBL':'Be back later','SEC':'Second','NC':'No comment','B4':'Before','BB':'Bye bye','XOXO':'Hugs and kisses','IMO':'In my opinion','ZZZ':'Sleeping',
       'JJ':'Just joking','F2F':'Face to face','CU':'See you','FAB':'Fabulous','TXT':'Text','M8':'Mate','DND':'Do not disturb','ILY':'I love you',
       'Q4U':'Question for you','TYT':'Take your time','LMA':'Leave me alone','5N':'Fine','Tho':'Though'}
+      con=Counter()
       a=0
+      c='Pre'
       df=0
       data=0
       df_sorted=0
       short=[]
+      w=[]
+      d1=[]
+      dff=pd.DataFrame()
+      if remove_all == True:
+        d.clear()
       if add_words== True:
           #d1={f1:f2 for f1,f2 in zip(word,full_form)}
           for i,j in word.items():
               d[i]=j
       if remove_words != None:
           for k in remove_words:
               d.pop(k)
-        
-        
-    
+
+
+
       text1=text.upper()
       wt=word_tokenize(text1)
-    
+
       for word in wt:
           if word in d:
             short.append(word)
             ind=wt.index(word)
             wt[ind]=d[word]
-      a=Counter(short)
+      #a=Counter(short)
       wt
       text1=' '.join([w for w in wt])
-      if mostly_used_shortwords==True:
-        print('Mostly used word')
-        df=pd.DataFrame(a.items(),columns=['shortword','count'])
-        print(df.sort_values('count',ascending=False)) 
-        
-      return text1.lower() 
+      
+      return text1.lower()
+    except ImportError as ip:
+      print(ip)
+    except ValueError as vs:
+      print(vs)
+    except TypeError as ts:
+      print(ts)
+    except NameError as ns:
+      print(ns)
     except Exception as ex:
-      print('Error : '+str(ex))
+      print(ex)
```

### Comparing `optimal_data_selector-1.0.4/optimal_data_selector.egg-info/PKG-INFO` & `optimal_data_selector-1.0.5/optimal_data_selector.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: optimal-data-selector
-Version: 1.0.4
-Summary: A Package for to optimize models
+Version: 1.0.5
+Summary: A Package for to optimize models, use for nlp short word treatment
 Author: Rohan Majumder
 Author-email: majumderrohan2001@gmail.com
 Keywords: get_best_data_combination,optimise_accuracy,lock_data_combination,gives_best_result,best_data_for_ML_models,works on text data also,short word treatment
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `optimal_data_selector-1.0.4/setup.py` & `optimal_data_selector-1.0.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '1.0.4'
-DESCRIPTION = 'A Package for to optimize models'
+VERSION = '1.0.5'
+DESCRIPTION = 'A Package for to optimize models, use for nlp short word treatment'
 LONG_DESCRIPTION = 'A package to increase the accuracy of ML models, gives you the best data for model training, works on text data also, short word treatment for NLP problems'
 
 # Setting up
 setup(
     name="optimal_data_selector",
     version=VERSION,
     author="Rohan Majumder",
```

