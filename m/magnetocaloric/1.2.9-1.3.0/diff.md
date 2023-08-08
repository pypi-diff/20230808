# Comparing `tmp/magnetocaloric-1.2.9.tar.gz` & `tmp/magnetocaloric-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magnetocaloric-1.2.9.tar", last modified: Thu Aug  3 11:51:41 2023, max compression
+gzip compressed data, was "magnetocaloric-1.3.0.tar", last modified: Tue Aug  8 15:58:07 2023, max compression
```

## Comparing `magnetocaloric-1.2.9.tar` & `magnetocaloric-1.3.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 11:51:41.329053 magnetocaloric-1.2.9/
--rw-rw-rw-   0        0        0       84 2022-04-14 07:58:46.000000 magnetocaloric-1.2.9/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1057 2023-07-27 08:24:00.000000 magnetocaloric-1.2.9/Licence.txt
--rw-rw-rw-   0        0        0       81 2022-04-14 07:58:45.000000 magnetocaloric-1.2.9/MANIFEST.in
--rw-rw-rw-   0        0        0     3969 2023-08-03 11:51:41.329053 magnetocaloric-1.2.9/PKG-INFO
--rw-rw-rw-   0        0        0     3222 2023-08-03 11:49:15.000000 magnetocaloric-1.2.9/README.md
-drwxrwxrwx   0        0        0        0 2023-08-03 11:51:41.285041 magnetocaloric-1.2.9/magnetocaloric/
--rw-rw-rw-   0        0        0      560 2023-07-31 06:14:28.000000 magnetocaloric-1.2.9/magnetocaloric/Color_marker.py
--rw-rw-rw-   0        0        0     1397 2023-07-30 11:40:32.000000 magnetocaloric-1.2.9/magnetocaloric/M_H_reshaping.py
--rw-rw-rw-   0        0        0     2059 2023-07-30 11:43:59.000000 magnetocaloric-1.2.9/magnetocaloric/RCP_plot.py
--rw-rw-rw-   0        0        0     3548 2023-07-30 11:43:19.000000 magnetocaloric-1.2.9/magnetocaloric/T_FWHM_RCP.py
--rw-rw-rw-   0        0        0      843 2023-08-03 11:49:45.000000 magnetocaloric-1.2.9/magnetocaloric/__init__.py
--rw-rw-rw-   0        0        0     1487 2023-07-30 11:41:26.000000 magnetocaloric-1.2.9/magnetocaloric/arrott_plot.py
--rw-rw-rw-   0        0        0     1424 2023-07-30 11:37:12.000000 magnetocaloric-1.2.9/magnetocaloric/collect_from_database.py
--rw-rw-rw-   0        0        0     5566 2023-08-03 03:03:55.000000 magnetocaloric-1.2.9/magnetocaloric/data_visualization01.py
--rw-rw-rw-   0        0        0     2433 2023-07-31 06:15:05.000000 magnetocaloric-1.2.9/magnetocaloric/entropy_change01.py
--rw-rw-rw-   0        0        0     1229 2023-07-30 11:38:43.000000 magnetocaloric-1.2.9/magnetocaloric/entropy_change02.py
--rw-rw-rw-   0        0        0    15238 2023-08-03 11:49:11.000000 magnetocaloric-1.2.9/magnetocaloric/mcepy.py
--rw-rw-rw-   0        0        0     2434 2023-07-30 11:42:47.000000 magnetocaloric-1.2.9/magnetocaloric/modified_arrott_plot.py
--rw-rw-rw-   0        0        0     2166 2023-08-03 03:09:46.000000 magnetocaloric-1.2.9/magnetocaloric/store_to_database01.py
--rw-rw-rw-   0        0        0      930 2023-07-30 11:36:24.000000 magnetocaloric-1.2.9/magnetocaloric/take_temp.py
-drwxrwxrwx   0        0        0        0 2023-08-03 11:51:41.325051 magnetocaloric-1.2.9/magnetocaloric.egg-info/
--rw-rw-rw-   0        0        0     3969 2023-08-03 11:51:40.000000 magnetocaloric-1.2.9/magnetocaloric.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      699 2023-08-03 11:51:40.000000 magnetocaloric-1.2.9/magnetocaloric.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 11:51:40.000000 magnetocaloric-1.2.9/magnetocaloric.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       77 2023-08-03 11:51:40.000000 magnetocaloric-1.2.9/magnetocaloric.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-08-03 11:51:40.000000 magnetocaloric-1.2.9/magnetocaloric.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-03 11:51:41.329053 magnetocaloric-1.2.9/setup.cfg
--rw-rw-rw-   0        0        0     1190 2023-08-03 11:49:17.000000 magnetocaloric-1.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-08 15:58:07.959611 magnetocaloric-1.3.0/
+-rw-rw-rw-   0        0        0       84 2022-04-14 07:58:46.000000 magnetocaloric-1.3.0/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1057 2023-07-27 08:24:00.000000 magnetocaloric-1.3.0/Licence.txt
+-rw-rw-rw-   0        0        0       81 2022-04-14 07:58:45.000000 magnetocaloric-1.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     3969 2023-08-08 15:58:07.959611 magnetocaloric-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3222 2023-08-08 15:50:56.000000 magnetocaloric-1.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-08-08 15:58:07.912718 magnetocaloric-1.3.0/magnetocaloric/
+-rw-rw-rw-   0        0        0      560 2023-07-31 06:14:28.000000 magnetocaloric-1.3.0/magnetocaloric/Color_marker.py
+-rw-rw-rw-   0        0        0     1397 2023-07-30 11:40:32.000000 magnetocaloric-1.3.0/magnetocaloric/M_H_reshaping.py
+-rw-rw-rw-   0        0        0     2059 2023-07-30 11:43:59.000000 magnetocaloric-1.3.0/magnetocaloric/RCP_plot.py
+-rw-rw-rw-   0        0        0     3548 2023-07-30 11:43:19.000000 magnetocaloric-1.3.0/magnetocaloric/T_FWHM_RCP.py
+-rw-rw-rw-   0        0        0      843 2023-08-03 11:49:45.000000 magnetocaloric-1.3.0/magnetocaloric/__init__.py
+-rw-rw-rw-   0        0        0     1487 2023-07-30 11:41:26.000000 magnetocaloric-1.3.0/magnetocaloric/arrott_plot.py
+-rw-rw-rw-   0        0        0     1424 2023-07-30 11:37:12.000000 magnetocaloric-1.3.0/magnetocaloric/collect_from_database.py
+-rw-rw-rw-   0        0        0     5566 2023-08-03 03:03:55.000000 magnetocaloric-1.3.0/magnetocaloric/data_visualization01.py
+-rw-rw-rw-   0        0        0     2433 2023-07-31 06:15:05.000000 magnetocaloric-1.3.0/magnetocaloric/entropy_change01.py
+-rw-rw-rw-   0        0        0     1229 2023-07-30 11:38:43.000000 magnetocaloric-1.3.0/magnetocaloric/entropy_change02.py
+-rw-rw-rw-   0        0        0    13910 2023-08-08 15:56:38.000000 magnetocaloric-1.3.0/magnetocaloric/mcepy.py
+-rw-rw-rw-   0        0        0     2434 2023-07-30 11:42:47.000000 magnetocaloric-1.3.0/magnetocaloric/modified_arrott_plot.py
+-rw-rw-rw-   0        0        0     2166 2023-08-03 03:09:46.000000 magnetocaloric-1.3.0/magnetocaloric/store_to_database01.py
+-rw-rw-rw-   0        0        0      930 2023-07-30 11:36:24.000000 magnetocaloric-1.3.0/magnetocaloric/take_temp.py
+drwxrwxrwx   0        0        0        0 2023-08-08 15:58:07.959611 magnetocaloric-1.3.0/magnetocaloric.egg-info/
+-rw-rw-rw-   0        0        0     3969 2023-08-08 15:58:06.000000 magnetocaloric-1.3.0/magnetocaloric.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      699 2023-08-08 15:58:06.000000 magnetocaloric-1.3.0/magnetocaloric.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 15:58:06.000000 magnetocaloric-1.3.0/magnetocaloric.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       77 2023-08-08 15:58:06.000000 magnetocaloric-1.3.0/magnetocaloric.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-08-08 15:58:06.000000 magnetocaloric-1.3.0/magnetocaloric.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-08 15:58:07.959611 magnetocaloric-1.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1190 2023-08-08 15:55:56.000000 magnetocaloric-1.3.0/setup.py
```

### Comparing `magnetocaloric-1.2.9/Licence.txt` & `magnetocaloric-1.3.0/Licence.txt`

 * *Files identical despite different names*

### Comparing `magnetocaloric-1.2.9/PKG-INFO` & `magnetocaloric-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magnetocaloric
-Version: 1.2.9
+Version: 1.3.0
 Summary: Effective Approach To Calculate Magnetocaloric Effect Of Any Magnetic Material Using Python
 Home-page: https://github.com/supratimdasinfo/Magnetocaloric-Effect
 Author: Supratim Das
 Author-email: supratim0707@gmail.com
 License: MIT
 Keywords: magnetocaloric,mcepy,magnetic,programming,code,python,supratim,das,bhaskar,biswas,physics
 Classifier: Development Status :: 5 - Production/Stable
@@ -12,15 +12,15 @@
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: Licence.txt
 
 
-# magnetocaloric 1.2.9
+# magnetocaloric 1.3.0
 #### Developed by Supratim Das
 
 ![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?)
 
 Effective approach to determine magnetocaloric performance of any magnetic material using python programming. From isotherm M(H) curves, using the Maxwell Relation the magnetocaloric performance of a material can be calculated with the help of this module.
 
 ## What's New
@@ -38,15 +38,15 @@
 
 ### 1. Installation 
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install magnetocaloric package.
 
 ```bash
 
- pip install magnetocaloric==1.2.9
+ pip install magnetocaloric==1.3.0
 
 ```
 ### 2. Manage Excel Spreadsheet
 -  Check the main excel spreadsheet from where the M-H data will be fetched by the program, data must be arranged in this format given below. 
 
 ![](https://raw.githubusercontent.com/supratimdasinfo/magnetocaloric.mcepy/main/Screenshot%20(229).png?raw=True)
```

### Comparing `magnetocaloric-1.2.9/README.md` & `magnetocaloric-1.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-# magnetocaloric 1.2.9
+# magnetocaloric 1.3.0
 #### Developed by Supratim Das
 
 ![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?)
 
 Effective approach to determine magnetocaloric performance of any magnetic material using python programming. From isotherm M(H) curves, using the Maxwell Relation the magnetocaloric performance of a material can be calculated with the help of this module.
 
 ## What's New
@@ -21,15 +21,15 @@
 
 ### 1. Installation 
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install magnetocaloric package.
 
 ```bash
 
- pip install magnetocaloric==1.2.9
+ pip install magnetocaloric==1.3.0
 
 ```
 ### 2. Manage Excel Spreadsheet
 -  Check the main excel spreadsheet from where the M-H data will be fetched by the program, data must be arranged in this format given below. 
 
 ![](https://raw.githubusercontent.com/supratimdasinfo/magnetocaloric.mcepy/main/Screenshot%20(229).png?raw=True)
```

### Comparing `magnetocaloric-1.2.9/magnetocaloric/Color_marker.py` & `magnetocaloric-1.3.0/magnetocaloric/Color_marker.py`

 * *Files identical despite different names*

### Comparing `magnetocaloric-1.2.9/magnetocaloric/M_H_reshaping.py` & `magnetocaloric-1.3.0/magnetocaloric/M_H_reshaping.py`

 * *Files identical despite different names*

### Comparing `magnetocaloric-1.2.9/magnetocaloric/RCP_plot.py` & `magnetocaloric-1.3.0/magnetocaloric/RCP_plot.py`

 * *Files identical despite different names*

### Comparing `magnetocaloric-1.2.9/magnetocaloric/T_FWHM_RCP.py` & `magnetocaloric-1.3.0/magnetocaloric/T_FWHM_RCP.py`

 * *Files identical despite different names*

### Comparing `magnetocaloric-1.2.9/magnetocaloric/__init__.py` & `magnetocaloric-1.3.0/magnetocaloric/__init__.py`

 * *Files identical despite different names*

### Comparing `magnetocaloric-1.2.9/magnetocaloric/arrott_plot.py` & `magnetocaloric-1.3.0/magnetocaloric/arrott_plot.py`

 * *Files identical despite different names*

### Comparing `magnetocaloric-1.2.9/magnetocaloric/collect_from_database.py` & `magnetocaloric-1.3.0/magnetocaloric/collect_from_database.py`

 * *Files identical despite different names*

### Comparing `magnetocaloric-1.2.9/magnetocaloric/data_visualization01.py` & `magnetocaloric-1.3.0/magnetocaloric/data_visualization01.py`

 * *Files identical despite different names*

### Comparing `magnetocaloric-1.2.9/magnetocaloric/entropy_change01.py` & `magnetocaloric-1.3.0/magnetocaloric/entropy_change01.py`

 * *Files identical despite different names*

### Comparing `magnetocaloric-1.2.9/magnetocaloric/entropy_change02.py` & `magnetocaloric-1.3.0/magnetocaloric/entropy_change02.py`

 * *Files identical despite different names*

### Comparing `magnetocaloric-1.2.9/magnetocaloric/mcepy.py` & `magnetocaloric-1.3.0/magnetocaloric/mcepy.py`

 * *Files 12% similar despite different names*

```diff
@@ -106,81 +106,54 @@
 
     # Store Data to Excel Files
     store_to_database01(n, T, one_H_by_M_con, M_sqr, path_two, path_three, six_entropy_change_con)
 
     return
 
 
-def sysdtpas():
-    if ((int(mu/3))%2 == 0) :
-        psasrwdo = dd*mm*yy
-        if psasrwdo < 10**5 :
-            for d in range (0, 1000):
-                psasrwdo += psasrwdo
-                if psasrwdo > 10**5 :
-                    break
-        psasrwdo3 = 0
-        for m in range (0, 6):
-            psasrwdo2 = float(psasrwdo/10**(m+1))                
-            psasrwdo1 = int(round((float(psasrwdo2)- int(psasrwdo2)),1)*10)*10**(5-m)               
-            psasrwdo3 += psasrwdo1
-        if psasrwdo3 < 10**5 :
-            for d in range (0, 1000):
-                psasrwdo3 += psasrwdo3
-                if psasrwdo3 > 10**5 :
-                    break
-        cpt = bcrypt.hashpw((str(psasrwdo3)).encode(), bcrypt.gensalt()) 
-        
-    else:
-        cekch_ady = [2, 5, 8, 11, 14, 17, 20, 23, 26, 29]
-        for i in range(0, len(cekch_ady), 1):
-             if (abs(dd - cekch_ady[i]))<= 1 :
-                psasrwdo = (cekch_ady[i])*mm*yy
-                if psasrwdo < 10**5 :
-                    for d in range (0, 1000):
-                        psasrwdo += psasrwdo
-                        if psasrwdo > 10**5 :
-                            break
-                psasrwdo3 = 0
-                for m in range (0, 6):
-                    psasrwdo2 = float(psasrwdo/10**(m+1))                
-                    psasrwdo1 = int(round((float(psasrwdo2)- int(psasrwdo2)),1)*10)*10**(5-m)               
-                    psasrwdo3 += psasrwdo1
-                if psasrwdo3 < 10**5 :
-                    for d in range (0, 1000):
-                        psasrwdo3 += psasrwdo3
-                        if psasrwdo3 > 10**5 :
-                            break            
-                
-                cpt = bcrypt.hashpw((str(psasrwdo3)).encode(), bcrypt.gensalt())           
-                break
-             elif ((dd - 30) == 1):
-                psasrwdo = 31*mm*yy           
-                if psasrwdo < 10**5 :
-                    for d in range (0, 1000):
-                        psasrwdo += psasrwdo
-                        if psasrwdo > 10**5 :
-                            break
-                psasrwdo3 = 0
-                for m in range (0, 6):
-                    psasrwdo2 = float(psasrwdo/10**(m+1))               
-                    psasrwdo1 = int(round((float(psasrwdo2)- int(psasrwdo2)),1)*10)*10**(5-m)                
-                    psasrwdo3 += psasrwdo1
-                    if psasrwdo3 < 10**5 :
-                        for d in range (0, 1000):
-                            psasrwdo3 += psasrwdo3
-                            if psasrwdo3 > 10**5 :
-                                break            
-                    
-                cpt = bcrypt.hashpw((str(psasrwdo3)).encode(), bcrypt.gensalt())
-                break
-    return cpt, psasrwdo3
-
+def sysdtpas(code):
+    tnuere = [7, 28, 56, 84]
+    acescs = False
+    psasrwdo3_total = []
+    for j in range (0, len(tnuere)):
+        psasrwdo3_con = []
+        for i in range (0, tnuere[j]):        
+            previous_day = today - timedelta(days=i)
+            dp = previous_day.day
+            mp = previous_day.month
+            yp = previous_day.year
+            psasrwdo = dp*mp*yp
+            if psasrwdo < 10**5 :
+                while psasrwdo < 10**5 :
+                    psasrwdo += dp * 3.14 * psasrwdo
+            psasrwdo3 = 0
+            for m in range (0, 6):
+                psasrwdo2 = float(psasrwdo/10**(m+1))
+                if ((int(mu/3))%2 == 0) :
+                    psasrwdo1 = (int(round((float(psasrwdo2)- int(psasrwdo2)),1)*tnuere[j])*(10**(5-m)))
+                else:
+                    psasrwdo1 = (int(round((float(psasrwdo2)- int(psasrwdo2)),1)*tnuere[j]*7)*(10**(5-m)))                    
+                psasrwdo3 += psasrwdo1
+            if psasrwdo3 < 10**5 :
+                while psasrwdo3 < 10**5 :
+                    psasrwdo3 += psasrwdo3
+            if psasrwdo3 > 999999:
+                while psasrwdo3 > 999999:
+                    psasrwdo3 = int(psasrwdo3/10)
+            #cpt = bcrypt.hashpw((str(psasrwdo3)).encode(), bcrypt.gensalt())
+            psasrwdo3_con.append(psasrwdo3)
+        psasrwdo3_total.append(psasrwdo3_con)
+    for x in range(0, len(psasrwdo3_total)):
+        for y in range(0, len(psasrwdo3_total[x])):
+            if code == psasrwdo3_total[x][y]:
+                acescs = True
+    return acescs
+"""
 def chkdtpas(stored_password, entered_password):
-    return bcrypt.checkpw(entered_password.encode(), stored_password)
+    return bcrypt.checkpw(entered_password.encode(), stored_password)"""
 
 def datavisualizationtwo(code, one_n, n, T, H, colour, marker, Label_one, plot_legend, one_M_plot_final, two_M_plot_final, H_plot_final, temperatures, five_entropy_change_con, M_sqr, one_H_by_M_con):
     """
     Visualize the data using Matplotlib.
 
     Args:
         one_n (int): Number of data points along one direction.
@@ -198,16 +171,15 @@
         five_entropy_change_con (list): List of lists containing entropy change data.
         M_sqr (list): List of squared magnetization values (M^2).
         one_H_by_M_con (list): List of lists containing H/M (applied field / magnetization) data.
 
     Returns:
         None: The function displays plots based on the data.
     """
-    funcval, actu = sysdtpas()
-    if chkdtpas(funcval, code):
+    if sysdtpas(code):
         
         if (plot_legend == 1):
 
             # Plotting magnetization vs. applied field for each temperature.
             for k in range(n):
                 plt.plot(H_plot_final, one_M_plot_final[k], linestyle='solid', label=T[n - (k + 1)], marker=next(marker), markersize=6, linewidth=2)
             plt.legend(loc='upper left', frameon=False, ncol=3)
@@ -300,16 +272,16 @@
         path_three (str): Filepath for the second Excel spreadsheet.
         six_entropy_change_con (list): List of lists containing entropy change values for each temperature.
 
     Note:
         The function will insert appropriate headers and blank spaces in the data before saving to Excel.
     """
     # Save entropy change data to the first Excel spreadsheet (path_two).
-    funcval, actu = sysdtpas()
-    if chkdtpas(funcval, code):
+
+    if sysdtpas(code):
         workbook = xlsxwriter.Workbook(path_two)
         worksheet = workbook.add_worksheet()
         row = 0
         for col, data in enumerate(six_entropy_change_con):
             worksheet.write_column(row, col, data)
         workbook.close()
```

### Comparing `magnetocaloric-1.2.9/magnetocaloric/modified_arrott_plot.py` & `magnetocaloric-1.3.0/magnetocaloric/modified_arrott_plot.py`

 * *Files identical despite different names*

### Comparing `magnetocaloric-1.2.9/magnetocaloric/store_to_database01.py` & `magnetocaloric-1.3.0/magnetocaloric/store_to_database01.py`

 * *Files identical despite different names*

### Comparing `magnetocaloric-1.2.9/magnetocaloric/take_temp.py` & `magnetocaloric-1.3.0/magnetocaloric/take_temp.py`

 * *Files identical despite different names*

### Comparing `magnetocaloric-1.2.9/magnetocaloric.egg-info/PKG-INFO` & `magnetocaloric-1.3.0/magnetocaloric.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magnetocaloric
-Version: 1.2.9
+Version: 1.3.0
 Summary: Effective Approach To Calculate Magnetocaloric Effect Of Any Magnetic Material Using Python
 Home-page: https://github.com/supratimdasinfo/Magnetocaloric-Effect
 Author: Supratim Das
 Author-email: supratim0707@gmail.com
 License: MIT
 Keywords: magnetocaloric,mcepy,magnetic,programming,code,python,supratim,das,bhaskar,biswas,physics
 Classifier: Development Status :: 5 - Production/Stable
@@ -12,15 +12,15 @@
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: Licence.txt
 
 
-# magnetocaloric 1.2.9
+# magnetocaloric 1.3.0
 #### Developed by Supratim Das
 
 ![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?)
 
 Effective approach to determine magnetocaloric performance of any magnetic material using python programming. From isotherm M(H) curves, using the Maxwell Relation the magnetocaloric performance of a material can be calculated with the help of this module.
 
 ## What's New
@@ -38,15 +38,15 @@
 
 ### 1. Installation 
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install magnetocaloric package.
 
 ```bash
 
- pip install magnetocaloric==1.2.9
+ pip install magnetocaloric==1.3.0
 
 ```
 ### 2. Manage Excel Spreadsheet
 -  Check the main excel spreadsheet from where the M-H data will be fetched by the program, data must be arranged in this format given below. 
 
 ![](https://raw.githubusercontent.com/supratimdasinfo/magnetocaloric.mcepy/main/Screenshot%20(229).png?raw=True)
```

### Comparing `magnetocaloric-1.2.9/magnetocaloric.egg-info/SOURCES.txt` & `magnetocaloric-1.3.0/magnetocaloric.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `magnetocaloric-1.2.9/setup.py` & `magnetocaloric-1.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='magnetocaloric',
-  version='1.2.9',
+  version='1.3.0',
   description='Effective Approach To Calculate Magnetocaloric Effect Of Any Magnetic Material Using Python',
   long_description=long_description,
   long_description_content_type="text/markdown",
   url='https://github.com/supratimdasinfo/Magnetocaloric-Effect',  
   author='Supratim Das',
   author_email='supratim0707@gmail.com',
   license='MIT',
```

