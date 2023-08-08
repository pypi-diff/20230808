# Comparing `tmp/ATACFragQC-0.4.6.tar.gz` & `tmp/ATACFragQC-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ATACFragQC-0.4.6.tar", last modified: Mon Apr 24 09:47:15 2023, max compression
+gzip compressed data, was "dist\ATACFragQC-0.4.7.tar", last modified: Tue Aug  8 09:38:51 2023, max compression
```

## Comparing `ATACFragQC-0.4.6.tar` & `ATACFragQC-0.4.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 09:47:15.000000 ATACFragQC-0.4.6/
-drwxrwxrwx   0        0        0        0 2023-04-24 09:47:15.000000 ATACFragQC-0.4.6/ATACFragQC/
--rw-rw-rw-   0        0        0       62 2023-04-24 09:46:00.000000 ATACFragQC-0.4.6/ATACFragQC/__init__.py
--rw-rw-rw-   0        0        0    13684 2023-04-24 09:44:10.000000 ATACFragQC-0.4.6/ATACFragQC/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 09:47:15.000000 ATACFragQC-0.4.6/ATACFragQC.egg-info/
--rw-rw-rw-   0        0        0     1186 2023-04-24 09:47:09.000000 ATACFragQC-0.4.6/ATACFragQC.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      307 2023-04-24 09:47:10.000000 ATACFragQC-0.4.6/ATACFragQC.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 09:47:09.000000 ATACFragQC-0.4.6/ATACFragQC.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-04-24 09:47:10.000000 ATACFragQC-0.4.6/ATACFragQC.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       35 2023-04-24 09:47:10.000000 ATACFragQC-0.4.6/ATACFragQC.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-24 09:47:10.000000 ATACFragQC-0.4.6/ATACFragQC.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1060 2020-12-19 11:09:54.000000 ATACFragQC-0.4.6/LICENSE
--rw-rw-rw-   0        0        0       45 2020-12-19 13:00:27.000000 ATACFragQC-0.4.6/MANIFEST.in
--rw-rw-rw-   0        0        0     1186 2023-04-24 09:47:15.000000 ATACFragQC-0.4.6/PKG-INFO
--rw-rw-rw-   0        0        0      637 2022-06-21 06:16:39.000000 ATACFragQC-0.4.6/README.md
--rw-rw-rw-   0        0        0       91 2020-12-19 12:59:45.000000 ATACFragQC-0.4.6/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-24 09:47:15.000000 ATACFragQC-0.4.6/setup.cfg
--rw-rw-rw-   0        0        0     1175 2020-12-19 11:17:55.000000 ATACFragQC-0.4.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-08 09:38:51.000000 ATACFragQC-0.4.7/
+drwxrwxrwx   0        0        0        0 2023-08-08 09:38:51.000000 ATACFragQC-0.4.7/ATACFragQC/
+-rw-rw-rw-   0        0        0       62 2023-08-08 09:38:19.000000 ATACFragQC-0.4.7/ATACFragQC/__init__.py
+-rw-rw-rw-   0        0        0    13589 2023-08-08 09:37:23.000000 ATACFragQC-0.4.7/ATACFragQC/__main__.py
+drwxrwxrwx   0        0        0        0 2023-08-08 09:38:51.000000 ATACFragQC-0.4.7/ATACFragQC.egg-info/
+-rw-rw-rw-   0        0        0     1186 2023-08-08 09:38:46.000000 ATACFragQC-0.4.7/ATACFragQC.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      307 2023-08-08 09:38:47.000000 ATACFragQC-0.4.7/ATACFragQC.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 09:38:46.000000 ATACFragQC-0.4.7/ATACFragQC.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-08-08 09:38:47.000000 ATACFragQC-0.4.7/ATACFragQC.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       35 2023-08-08 09:38:47.000000 ATACFragQC-0.4.7/ATACFragQC.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-08-08 09:38:47.000000 ATACFragQC-0.4.7/ATACFragQC.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1060 2020-12-19 11:09:54.000000 ATACFragQC-0.4.7/LICENSE
+-rw-rw-rw-   0        0        0       45 2020-12-19 13:00:27.000000 ATACFragQC-0.4.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     1186 2023-08-08 09:38:51.000000 ATACFragQC-0.4.7/PKG-INFO
+-rw-rw-rw-   0        0        0      637 2022-06-21 06:16:39.000000 ATACFragQC-0.4.7/README.md
+-rw-rw-rw-   0        0        0       91 2020-12-19 12:59:45.000000 ATACFragQC-0.4.7/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-08-08 09:38:51.000000 ATACFragQC-0.4.7/setup.cfg
+-rw-rw-rw-   0        0        0     1175 2020-12-19 11:17:55.000000 ATACFragQC-0.4.7/setup.py
```

### Comparing `ATACFragQC-0.4.6/ATACFragQC/__main__.py` & `ATACFragQC-0.4.7/ATACFragQC/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,45 +158,37 @@
         len_count.to_csv(pathname+"_fl.tsv", sep="\t", index=False, header=False)
         if dist_count.size > 0:
             dist_count.to_csv(pathname+"_tss.tsv", sep="\t", index=False, header=False)
             pd.DataFrame({"V1": factors}).to_csv(pathname+"_base.tsv", sep="\t", index=False, header=False)
     pic_list = ["a", "b", "c"]
     pic_list = list(set(pic_list).intersection(set(args.pic_list.split(","))))
     pic_list.sort()
-    if dist_count.size == 0:
+    if "c" in pic_list and dist_count.size == 0:
         pic_list.remove("c")
     if len(pic_list) == 0:
         return
     if "a" in pic_list:
-        ggsave(plot=ggplot(chr_count, aes(x="V1", y="V2"))+geom_bar(stat="identity", width=0.8, fill="#80B1D3")+
-            labs(x="Chromosome", y="Fragments")+scale_y_continuous(expand=(0, 0))+
-            theme(plot_title=element_blank(), panel_background=element_blank(), axis_line=element_line(colour="black"), 
-            axis_text_y=element_text(colour="black"), axis_text_x=element_text(angle=270, hjust=0.3, vjust=1, colour="black")), 
-            width=4, height=6, dpi=200, filename=pathname+".tmpa.png", limitsize=False, verbose=False)
+        plot = ggplot(chr_count, aes(x="V1", y="V2"))+geom_bar(stat="identity", width=0.8, fill="#80B1D3")+labs(x="Chromosome", y="Fragments")+scale_y_continuous(expand=(0, 0))+theme(plot_title=element_blank(), panel_background=element_blank(), axis_line=element_line(colour="black"), axis_text_y=element_text(colour="black"), axis_text_x=element_text(angle=270, hjust=0.3, vjust=1, colour="black"))
+        plot.save(width=4, height=6, dpi=200, filename=pathname+".tmpa.png", limitsize=False, verbose=False)
     if "b" in pic_list:
-        ggsave(plot=ggplot(len_count, aes(x="V1", y="V2"))+geom_bar(stat="identity", colour="#80B1D3", fill="#80B1D3")+
-            labs(x="\nInsert Size", y="Fragments")+scale_y_continuous(expand=(0, 0))+
-            theme(plot_title=element_blank(), panel_background=element_blank(), axis_line=element_line(colour="black"), axis_text=element_text(colour="black")), 
-            width=6, height=6, dpi=200, filename=pathname+".tmpb.png", limitsize=False, verbose=False)
+        plot = ggplot(len_count, aes(x="V1", y="V2"))+geom_bar(stat="identity", colour="#80B1D3", fill="#80B1D3")+labs(x="\nInsert Size", y="Fragments")+scale_y_continuous(expand=(0, 0))+theme(plot_title=element_blank(), panel_background=element_blank(), axis_line=element_line(colour="black"), axis_text=element_text(colour="black"))
+        plot.save(width=6, height=6, dpi=200, filename=pathname+".tmpb.png", limitsize=False, verbose=False)
     if "c" in pic_list:
         break_length = 50
         if args.widthtss > 6000:
             break_length = 2000
         if args.widthtss > 3000:
             break_length = 1000
         elif args.widthtss > 1000:
             break_length = 500
         elif args.widthtss > 400:
             break_length = 200
         break_range = max(1, args.widthtss//break_length)*break_length
-        ggsave(plot=ggplot(dist_count, aes(x="V1", y="V2"))+geom_line(size=1, colour="#80B1D3")+
-            labs(x="\nDistance from TSS (bp)", y="Mean TSS enrichment score")+scale_y_continuous(expand=(0, 0))+
-            scale_x_continuous(breaks=range(-break_range, break_range+1, break_length))+
-            theme(plot_title=element_blank(), panel_background=element_blank(), axis_line=element_line(colour="black"), axis_text=element_text(colour="black")), 
-            width=6, height=6, dpi=200, filename=pathname+".tmpc.png", limitsize=False, verbose=False)
+        plot = ggplot(dist_count, aes(x="V1", y="V2"))+geom_line(size=1, colour="#80B1D3")+labs(x="\nDistance from TSS (bp)", y="Mean TSS enrichment score")+scale_y_continuous(expand=(0, 0))+scale_x_continuous(breaks=range(-break_range, break_range+1, break_length))+theme(plot_title=element_blank(), panel_background=element_blank(), axis_line=element_line(colour="black"), axis_text=element_text(colour="black"))
+        plot.save(width=6, height=6, dpi=200, filename=pathname+".tmpc.png", limitsize=False, verbose=False)
     width = 0
     height = 0
     imgs = [Image.open(pathname+".tmp"+c+".png") for c in pic_list]
     for img in imgs:
         width += img.width
         height = max(height, img.height)
     result = Image.new("RGBA", (width, height), "white")
```

### Comparing `ATACFragQC-0.4.6/ATACFragQC.egg-info/PKG-INFO` & `ATACFragQC-0.4.7/ATACFragQC.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ATACFragQC
-Version: 0.4.6
+Version: 0.4.7
 Summary: Fragment Quality Control for ATAC-seq
 Home-page: https://github.com/0CBH0/ATACFragQC
 Author: 0CBH0
 Author-email: maodatou88@163.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ATACFragQC-0.4.6/LICENSE` & `ATACFragQC-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ATACFragQC-0.4.6/PKG-INFO` & `ATACFragQC-0.4.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ATACFragQC
-Version: 0.4.6
+Version: 0.4.7
 Summary: Fragment Quality Control for ATAC-seq
 Home-page: https://github.com/0CBH0/ATACFragQC
 Author: 0CBH0
 Author-email: maodatou88@163.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ATACFragQC-0.4.6/README.md` & `ATACFragQC-0.4.7/README.md`

 * *Files identical despite different names*

### Comparing `ATACFragQC-0.4.6/setup.py` & `ATACFragQC-0.4.7/setup.py`

 * *Files identical despite different names*

