# Comparing `tmp/LN2_Monitor-0.0.1.tar.gz` & `tmp/LN2_Monitor-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LN2_Monitor-0.0.1.tar", last modified: Mon Aug  7 21:23:14 2023, max compression
+gzip compressed data, was "LN2_Monitor-0.0.2.tar", last modified: Tue Aug  8 18:04:19 2023, max compression
```

## Comparing `LN2_Monitor-0.0.1.tar` & `LN2_Monitor-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-08-07 21:23:14.304565 LN2_Monitor-0.0.1/
-drwxrwxrwx   0        0        0        0 2023-08-07 21:23:14.296435 LN2_Monitor-0.0.1/LN2_Monitor.egg-info/
--rw-rw-rw-   0        0        0     2599 2023-08-07 21:23:14.000000 LN2_Monitor-0.0.1/LN2_Monitor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      423 2023-08-07 21:23:14.000000 LN2_Monitor-0.0.1/LN2_Monitor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-07 21:23:14.000000 LN2_Monitor-0.0.1/LN2_Monitor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-08-07 21:23:14.000000 LN2_Monitor-0.0.1/LN2_Monitor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-08-07 21:23:14.000000 LN2_Monitor-0.0.1/LN2_Monitor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2599 2023-08-07 21:23:14.303566 LN2_Monitor-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2051 2023-07-24 21:35:34.000000 LN2_Monitor-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-08-07 21:23:14.299565 LN2_Monitor-0.0.1/ln2_monitor/
--rw-rw-rw-   0        0        0        0 2023-07-18 20:07:57.000000 LN2_Monitor-0.0.1/ln2_monitor/__init__.py
--rw-rw-rw-   0        0        0     3399 2023-07-18 19:22:36.000000 LN2_Monitor-0.0.1/ln2_monitor/d1.py
--rw-rw-rw-   0        0        0      627 2023-08-07 21:22:29.000000 LN2_Monitor-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-07 21:23:14.305567 LN2_Monitor-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      651 2023-07-24 21:21:38.000000 LN2_Monitor-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-08 18:04:19.563276 LN2_Monitor-0.0.2/
+drwxrwxrwx   0        0        0        0 2023-08-08 18:04:19.553276 LN2_Monitor-0.0.2/LN2_Monitor.egg-info/
+-rw-rw-rw-   0        0        0     2718 2023-08-08 18:04:19.000000 LN2_Monitor-0.0.2/LN2_Monitor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2023-08-08 18:04:19.000000 LN2_Monitor-0.0.2/LN2_Monitor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 18:04:19.000000 LN2_Monitor-0.0.2/LN2_Monitor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-08-08 18:04:19.000000 LN2_Monitor-0.0.2/LN2_Monitor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-08-08 18:04:19.000000 LN2_Monitor-0.0.2/LN2_Monitor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2718 2023-08-08 18:04:19.563276 LN2_Monitor-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2227 2023-08-08 18:03:26.000000 LN2_Monitor-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-08-08 18:04:19.563276 LN2_Monitor-0.0.2/ln2_monitor/
+-rw-rw-rw-   0        0        0        0 2023-08-08 18:03:27.000000 LN2_Monitor-0.0.2/ln2_monitor/__init__.py
+-rw-rw-rw-   0        0        0     3593 2023-08-08 18:03:27.000000 LN2_Monitor-0.0.2/ln2_monitor/d1.py
+-rw-rw-rw-   0        0        0      602 2023-08-08 18:03:27.000000 LN2_Monitor-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-08 18:04:19.563276 LN2_Monitor-0.0.2/setup.cfg
```

### Comparing `LN2_Monitor-0.0.1/LN2_Monitor.egg-info/PKG-INFO` & `LN2_Monitor-0.0.2/LN2_Monitor.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,39 +1,37 @@
 Metadata-Version: 2.1
 Name: LN2-Monitor
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Project that helps automate the weighing of LN2
-Home-page: https://github.com/dav17393/LN2_Monitor
-Author: Jordan Wheeler, David Shin
 Author-email: "dav17393, wheeler1711" <wheeler1711@gmail.com>
 Project-URL: Homepage, https://github.com/dav17393/LN2_Monitor
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >3.7
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # LN2_Monitor
 This project will use a USB connection to a dymo scale to help graph and weigh the percentage full of an LN2 trap. The percentage full is based on the maximum weight a LN2 trap can hold(about 28.26kg)
 
 **Required Softwares:**
-
-PyUSB 1.0 (https://sourceforge.net/projects/pyusb/files/PyUSB%201.0/)
+download the softwares below first:
 
 libusb-win32 (https://sourceforge.net/projects/libusb-win32/)
+After installing libusg-win32, click through the install screens until you get to "device selection". In device selection, select the USB input device with product ID 8009(pid:8009). 
 
-pip install ln2-monitor
+to install the code: python3 -m pip install LN2_Monitor
 then go into python and input "from ln2_monitor import d1". 
 input "scale = d1.SCL()"
 
-**How to run the Software:**
+**How to run the Software:** (not needed if pip installed)
 
-After opening up the program, download both softwares and run the libusb-win32 software. In device selection, select the USB input device with product ID 8009(pid:8009). Then pipinstall pyusb, numpy, and matplot. Then run the code by changing the directory whichever folder the d1 file was downloaded to. Then switch powershell to python and import the d1 file. Set scale = d1.SCL() and run scale.main() or scale.plot() to start plotting and transferring the data to a txt file. You can also run scale.getkg() or scale.getdata() to get the kg or the array respectively. The basic minimum and maximum weights(kg) are set to default as the blucifer cryostat. Scale.setweight() can be run to change the minumum and maximum weight of the cryostat.
+After opening up the program, download the software above and run the software. In device selection, select the USB input device with product ID 8009(pid:8009). Then pipinstall pyusb, numpy, and matplot. Then run the code by changing the directory whichever folder the d1 file was downloaded to. Then switch powershell to python and import the d1 file. Set scale = d1.SCL() and run scale.main() or scale.plot() to start plotting and transferring the data to a txt file. You can also run scale.getkg() or scale.getdata() to get the kg or the array respectively. The basic minimum and maximum weights(kg) are set to default as the blucifer cryostat. Scale.setweight() can be run to change the minumum and maximum weight of the cryostat.
 
-To turn off "auto-sleep" mode on the scale, hold the kg/lb button and turn the scale on. 
+**To turn off "auto-sleep" mode on the scale, hold the kg/lb button and turn the scale on. **
 
 **The array that is returned when calling the scale.main(), scale.plot(), or scale.getdata() functions can be translated as shown below:**
 array('B'[3, 2, 11, 255, 0, 0])
 
 The first element is always 3 and negatable.
 The second element is also negatable.
 The third element will only return either 2 or 11, with 2 meaning the scale is in kg mode and 11 meaning the scale is in lbs/oz mode.
```

### Comparing `LN2_Monitor-0.0.1/PKG-INFO` & `LN2_Monitor-0.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,39 +1,37 @@
 Metadata-Version: 2.1
 Name: LN2_Monitor
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Project that helps automate the weighing of LN2
-Home-page: https://github.com/dav17393/LN2_Monitor
-Author: Jordan Wheeler, David Shin
 Author-email: "dav17393, wheeler1711" <wheeler1711@gmail.com>
 Project-URL: Homepage, https://github.com/dav17393/LN2_Monitor
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >3.7
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # LN2_Monitor
 This project will use a USB connection to a dymo scale to help graph and weigh the percentage full of an LN2 trap. The percentage full is based on the maximum weight a LN2 trap can hold(about 28.26kg)
 
 **Required Softwares:**
-
-PyUSB 1.0 (https://sourceforge.net/projects/pyusb/files/PyUSB%201.0/)
+download the softwares below first:
 
 libusb-win32 (https://sourceforge.net/projects/libusb-win32/)
+After installing libusg-win32, click through the install screens until you get to "device selection". In device selection, select the USB input device with product ID 8009(pid:8009). 
 
-pip install ln2-monitor
+to install the code: python3 -m pip install LN2_Monitor
 then go into python and input "from ln2_monitor import d1". 
 input "scale = d1.SCL()"
 
-**How to run the Software:**
+**How to run the Software:** (not needed if pip installed)
 
-After opening up the program, download both softwares and run the libusb-win32 software. In device selection, select the USB input device with product ID 8009(pid:8009). Then pipinstall pyusb, numpy, and matplot. Then run the code by changing the directory whichever folder the d1 file was downloaded to. Then switch powershell to python and import the d1 file. Set scale = d1.SCL() and run scale.main() or scale.plot() to start plotting and transferring the data to a txt file. You can also run scale.getkg() or scale.getdata() to get the kg or the array respectively. The basic minimum and maximum weights(kg) are set to default as the blucifer cryostat. Scale.setweight() can be run to change the minumum and maximum weight of the cryostat.
+After opening up the program, download the software above and run the software. In device selection, select the USB input device with product ID 8009(pid:8009). Then pipinstall pyusb, numpy, and matplot. Then run the code by changing the directory whichever folder the d1 file was downloaded to. Then switch powershell to python and import the d1 file. Set scale = d1.SCL() and run scale.main() or scale.plot() to start plotting and transferring the data to a txt file. You can also run scale.getkg() or scale.getdata() to get the kg or the array respectively. The basic minimum and maximum weights(kg) are set to default as the blucifer cryostat. Scale.setweight() can be run to change the minumum and maximum weight of the cryostat.
 
-To turn off "auto-sleep" mode on the scale, hold the kg/lb button and turn the scale on. 
+**To turn off "auto-sleep" mode on the scale, hold the kg/lb button and turn the scale on. **
 
 **The array that is returned when calling the scale.main(), scale.plot(), or scale.getdata() functions can be translated as shown below:**
 array('B'[3, 2, 11, 255, 0, 0])
 
 The first element is always 3 and negatable.
 The second element is also negatable.
 The third element will only return either 2 or 11, with 2 meaning the scale is in kg mode and 11 meaning the scale is in lbs/oz mode.
```

### Comparing `LN2_Monitor-0.0.1/README.md` & `LN2_Monitor-0.0.2/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-# LN2_Monitor
-This project will use a USB connection to a dymo scale to help graph and weigh the percentage full of an LN2 trap. The percentage full is based on the maximum weight a LN2 trap can hold(about 28.26kg)
-
-**Required Softwares:**
-
-PyUSB 1.0 (https://sourceforge.net/projects/pyusb/files/PyUSB%201.0/)
-
-libusb-win32 (https://sourceforge.net/projects/libusb-win32/)
-
-pip install ln2-monitor
-then go into python and input "from ln2_monitor import d1". 
-input "scale = d1.SCL()"
-
-**How to run the Software:**
-
-After opening up the program, download both softwares and run the libusb-win32 software. In device selection, select the USB input device with product ID 8009(pid:8009). Then pipinstall pyusb, numpy, and matplot. Then run the code by changing the directory whichever folder the d1 file was downloaded to. Then switch powershell to python and import the d1 file. Set scale = d1.SCL() and run scale.main() or scale.plot() to start plotting and transferring the data to a txt file. You can also run scale.getkg() or scale.getdata() to get the kg or the array respectively. The basic minimum and maximum weights(kg) are set to default as the blucifer cryostat. Scale.setweight() can be run to change the minumum and maximum weight of the cryostat.
-
-To turn off "auto-sleep" mode on the scale, hold the kg/lb button and turn the scale on. 
-
-**The array that is returned when calling the scale.main(), scale.plot(), or scale.getdata() functions can be translated as shown below:**
-array('B'[3, 2, 11, 255, 0, 0])
-
-The first element is always 3 and negatable.
-The second element is also negatable.
-The third element will only return either 2 or 11, with 2 meaning the scale is in kg mode and 11 meaning the scale is in lbs/oz mode.
-The fourth element is the scale factor. A value of 255 means the scaling factor is 10^-1(0.1), a value of 254 means a scaling factor of 10^-2(0.01), and so on. 
-The fourth and fifth elements together are used to determine the weight.
-The sixth element is also negatable. 
-
-Enjoy!
+# LN2_Monitor
+This project will use a USB connection to a dymo scale to help graph and weigh the percentage full of an LN2 trap. The percentage full is based on the maximum weight a LN2 trap can hold(about 28.26kg)
+
+**Required Softwares:**
+download the softwares below first:
+
+libusb-win32 (https://sourceforge.net/projects/libusb-win32/)
+After installing libusg-win32, click through the install screens until you get to "device selection". In device selection, select the USB input device with product ID 8009(pid:8009). 
+
+to install the code: python3 -m pip install LN2_Monitor
+then go into python and input "from ln2_monitor import d1". 
+input "scale = d1.SCL()"
+
+**How to run the Software:** (not needed if pip installed)
+
+After opening up the program, download the software above and run the software. In device selection, select the USB input device with product ID 8009(pid:8009). Then pipinstall pyusb, numpy, and matplot. Then run the code by changing the directory whichever folder the d1 file was downloaded to. Then switch powershell to python and import the d1 file. Set scale = d1.SCL() and run scale.main() or scale.plot() to start plotting and transferring the data to a txt file. You can also run scale.getkg() or scale.getdata() to get the kg or the array respectively. The basic minimum and maximum weights(kg) are set to default as the blucifer cryostat. Scale.setweight() can be run to change the minumum and maximum weight of the cryostat.
+
+**To turn off "auto-sleep" mode on the scale, hold the kg/lb button and turn the scale on. **
+
+**The array that is returned when calling the scale.main(), scale.plot(), or scale.getdata() functions can be translated as shown below:**
+array('B'[3, 2, 11, 255, 0, 0])
+
+The first element is always 3 and negatable.
+The second element is also negatable.
+The third element will only return either 2 or 11, with 2 meaning the scale is in kg mode and 11 meaning the scale is in lbs/oz mode.
+The fourth element is the scale factor. A value of 255 means the scaling factor is 10^-1(0.1), a value of 254 means a scaling factor of 10^-2(0.01), and so on. 
+The fourth and fifth elements together are used to determine the weight.
+The sixth element is also negatable. 
+
+Enjoy!
```

### Comparing `LN2_Monitor-0.0.1/ln2_monitor/d1.py` & `LN2_Monitor-0.0.2/ln2_monitor/d1.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,116 +1,128 @@
-import usb.core
-import usb.util
-import time
-import numpy as np
-import math
-
-from datetime import datetime
-from matplotlib import pyplot
-from matplotlib.animation import FuncAnimation
-from random import randrange
-
-
-class SCL():
-
-    def __init__(self):
-        self.VENDOR_ID = 0x0922
-        self.PRODUCT_ID = 0x8009
-        self.device = usb.core.find(idVendor=self.VENDOR_ID,idProduct=self.PRODUCT_ID)
-        self.device.set_configuration()
-        self.endpoint = self.device[0][(0,0)][0]
-        self.data = None
-        self.weighmax = 28.2588
-        self.weighmin = 10.97694
-    
-    def main(self):
-        self.plot()
-    
-    if __name__ == "__main":
-        main()
-
-    def getdata(self):
-        try:
-           self.data = self.device.read(self.endpoint.bEndpointAddress,self.endpoint.wMaxPacketSize)
-        except:
-            usb.util.dispose_resources(self.device)
-            time.sleep(0.1)
-            self.device = usb.core.find(idVendor=self.VENDOR_ID,idProduct=self.PRODUCT_ID)
-            self.device.set_configuration()
-            self.endpoint = self.device[0][(0,0)][0]
-            self.data = self.device.read(self.endpoint.bEndpointAddress,self.endpoint.wMaxPacketSize)
-        print (self.data)
-        
-     
-    def setweight(self):
-        self.weighmax = float(input("What is the Maximum Weight(kg) of the Cryostat?:"))
-        self.weighmin = float(input("What is the Minumum Weight(kg) of the Cryostat?:"))
-    def getpercentfull(self):
-        self.per= None
-        while self.per == None:
-            self.getdata()
-            try:
-                self.per =  ((((self.data[4] + (256*self.data[5]))/10)-self.weighmin)/(self.weighmax-self.weighmin))*100
-            except:
-                time.sleep(0.1)
-                continue
-            print(self.per)
-        return self.per
-    
-    def getkg(self):
-        self.kg = None
-        
-        while self.kg == None:
-            self.getdata()
-            try:
-                self.kg = ((self.data[4] + (256*self.data[5]))/10)
-
-            except:
-                time.sleep(0.1)
-                continue
-        print(self.kg)       
-    
-    def plot(self, interval=1000):
-        x_data, y_data = [], []
-        now = datetime.now()
-        date_time = now.strftime("%Y_%m_%d, Dymo")
-        date_timesec = now.strftime("%Y/%m/%d, %H:%M:%S")
-        self.tfile = open(date_time+'.txt', 'a')
-    
-        figure = pyplot.figure()
-        line, = pyplot.plot_date(x_data, y_data, '-')
-        self.interval = interval
-        pyplot.title('Cryostat fullness')
-        pyplot.ylabel('Percent full')
-       
-        
-        def update(frame):
-            self.getpercentfull()
-            x_data.append(datetime.now())
-            y_data.append(self.per)
-            items = str(date_timesec)+","+" "+str(round(self.per,2))+"%"+"\n"
-            self.tfile.write(items)
-            line.set_data(x_data, y_data)
-            figure.gca().relim()
-            figure.gca().autoscale_view()
-            return line,
-  
-        animation = FuncAnimation(figure, update, interval=self.interval)
-      
-        pyplot.show()
-        self.tfile.close()
-      
-  
-    def __str__(self):
-        return f"{self.data}"
-        
-    def close(self):
-        self.scl.close()
-        
-   
-  
-
-  
-
-
-
-
+import usb.core
+import usb.util
+import time
+import numpy as np
+import math
+
+from datetime import datetime
+from matplotlib import pyplot
+from matplotlib.animation import FuncAnimation
+from random import randrange
+
+
+class SCL():
+
+    def __init__(self):
+        self.VENDOR_ID = 0x0922
+        self.PRODUCT_ID = 0x8009
+        self.device = usb.core.find(idVendor=self.VENDOR_ID,idProduct=self.PRODUCT_ID)
+        self.device.set_configuration()
+        self.endpoint = self.device[0][(0,0)][0]
+        self.data = None
+        self.weighmax = 28.2588
+        self.weighmin = 10.97694
+    
+    def main(self):
+        self.plot()
+    
+    if __name__ == "__main":
+        main()
+    
+   
+     
+       
+
+    def getdata(self):
+        try:
+           self.data = self.device.read(self.endpoint.bEndpointAddress,self.endpoint.wMaxPacketSize)
+        except:
+            usb.util.dispose_resources(self.device)
+            time.sleep(0.1)
+            self.device = usb.core.find(idVendor=self.VENDOR_ID,idProduct=self.PRODUCT_ID)
+            self.device.set_configuration()
+            self.endpoint = self.device[0][(0,0)][0]
+            self.data = self.device.read(self.endpoint.bEndpointAddress,self.endpoint.wMaxPacketSize)
+        print (self.data)
+        
+     
+    def setweight(self):
+        self.weighmax = float(input("What is the Maximum Weight(kg) of the LN2 Trap?:"))
+        self.weighmin = float(input("What is the Minumum Weight(kg) of the LN2 Trap?:"))
+    def getpercentfull(self):
+        self.per= None
+        while self.per == None:
+            self.getdata()
+            try:
+                self.per =  ((((self.data[4] + (256*self.data[5]))/10)-self.weighmin)/(self.weighmax-self.weighmin))*100
+            except:
+                time.sleep(0.1)
+                continue
+            print(self.per)
+        return self.per
+    
+    def getkg(self):
+        self.kg = None
+        
+        while self.kg == None:
+            self.getdata()
+            try:
+                self.kg = ((self.data[4] + (256*self.data[5]))/10)
+
+            except:
+                time.sleep(0.1)
+                continue
+        print(self.kg)       
+    
+    def plot(self, interval=1000000):
+        x_data, y_data = [], []
+        date_time = datetime.now().strftime("%Y_%m_%d Dymo")
+        self.tfile = open(date_time+ '.txt', 'a')
+    
+        figure = pyplot.figure()
+        line, = pyplot.plot_date(x_data, y_data, '-')
+        self.interval = interval
+        pyplot.title('LN2 Trap Fullness')
+        pyplot.ylabel('Percent Full')
+        pyplot.xlabel('Time')
+       
+        
+        def update(frame):
+            self.getpercentfull()
+            ax = pyplot.gca()
+            x_data.append(datetime.now())
+            y_data.append(self.per)
+            items = str(datetime.now().strftime("%H:%M:%S")) +","+" "+str(round(self.per,2))+"%"+"\n"
+            self.tfile.write(items)
+            line.set_data(x_data, y_data)
+            figure.gca().relim()
+            figure.gca().autoscale_view()
+            pyplot.plot(x_data, y_data, '-', color='blue')
+            if self.per > 10:
+                ax.set_facecolor('white')
+            if self.per < 20:
+                ax.set_facecolor('red')
+            return line,
+
+ 
+        animation = FuncAnimation(figure, update, interval=self.interval/1000)
+        #pyplot.figure(figsize=(12,8))
+        pyplot.xticks(rotation = 30)
+        pyplot.show()
+
+        self.tfile.close()
+      
+  
+    def __str__(self):
+        return f"{self.data}"
+        
+    def close(self):
+        self.scl.close()
+        
+   
+  
+
+  
+
+
+
+
```

