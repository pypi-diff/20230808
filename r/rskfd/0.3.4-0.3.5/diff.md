# Comparing `tmp/rskfd-0.3.4.tar.gz` & `tmp/rskfd-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rskfd-0.3.4.tar", last modified: Wed Oct 12 19:08:00 2022, max compression
+gzip compressed data, was "rskfd-0.3.5.tar", last modified: Tue Aug  8 09:07:48 2023, max compression
```

## Comparing `rskfd-0.3.4.tar` & `rskfd-0.3.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2022-10-12 19:08:00.956622 rskfd-0.3.4/
--rw-rw-rw-   0        0        0     2204 2022-10-12 19:08:00.956622 rskfd-0.3.4/PKG-INFO
--rw-rw-rw-   0        0        0     1386 2020-07-13 06:29:17.000000 rskfd-0.3.4/README.md
-drwxrwxrwx   0        0        0        0 2022-10-12 19:08:00.925379 rskfd-0.3.4/examples/
--rw-rw-rw-   0        0        0     2570 2022-10-12 19:00:26.000000 rskfd-0.3.4/examples/Wv2BinStream.py
--rw-rw-rw-   0        0        0     1275 2022-10-12 18:58:52.000000 rskfd-0.3.4/examples/fileopening.py
--rw-rw-rw-   0        0        0     6637 2020-10-13 07:00:50.000000 rskfd-0.3.4/examples/instrumentexamples.py
--rw-rw-rw-   0        0        0     1082 2020-07-08 13:59:40.000000 rskfd-0.3.4/license.txt
-drwxrwxrwx   0        0        0        0 2022-10-12 19:08:00.925379 rskfd-0.3.4/rskfd/
--rw-rw-rw-   0        0        0     1261 2022-06-15 06:01:52.000000 rskfd-0.3.4/rskfd/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-12 19:08:00.941002 rskfd-0.3.4/rskfd/helper/
--rw-rw-rw-   0        0        0     3902 2020-08-13 18:11:01.000000 rskfd-0.3.4/rskfd/helper/helper.py
-drwxrwxrwx   0        0        0        0 2022-10-12 19:08:00.941002 rskfd-0.3.4/rskfd/iq_data_handling/
--rw-rw-rw-   0        0        0    20867 2022-10-12 18:10:20.000000 rskfd-0.3.4/rskfd/iq_data_handling/iqdata.py
-drwxrwxrwx   0        0        0        0 2022-10-12 19:08:00.956622 rskfd-0.3.4/rskfd/remote_control/
--rw-rw-rw-   0        0        0    14607 2022-10-05 09:04:02.000000 rskfd-0.3.4/rskfd/remote_control/instrument.py
--rw-rw-rw-   0        0        0     1352 2022-06-15 06:04:19.000000 rskfd-0.3.4/rskfd/remote_control/instrumentRS.py
--rw-rw-rw-   0        0        0      675 2019-12-09 13:08:45.000000 rskfd-0.3.4/rskfd/remote_control/instrumentRSExceptions.py
--rw-rw-rw-   0        0        0     8506 2020-10-20 07:35:56.000000 rskfd-0.3.4/rskfd/remote_control/instrumentRS_FSW.py
--rw-rw-rw-   0        0        0     1905 2019-12-09 13:10:19.000000 rskfd-0.3.4/rskfd/remote_control/instrumentRS_VSE.py
-drwxrwxrwx   0        0        0        0 2022-10-12 19:08:00.956622 rskfd-0.3.4/rskfd/signal_generation/
--rw-rw-rw-   0        0        0     2290 2020-12-11 07:28:48.000000 rskfd-0.3.4/rskfd/signal_generation/signal_generation.py
-drwxrwxrwx   0        0        0        0 2022-10-12 19:08:00.956622 rskfd-0.3.4/rskfd/snp_handling/
--rw-rw-rw-   0        0        0     9605 2021-03-16 15:49:04.000000 rskfd-0.3.4/rskfd/snp_handling/snpfiles.py
-drwxrwxrwx   0        0        0        0 2022-10-12 19:08:00.941002 rskfd-0.3.4/rskfd.egg-info/
--rw-rw-rw-   0        0        0     2204 2022-10-12 19:08:00.000000 rskfd-0.3.4/rskfd.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      615 2022-10-12 19:08:00.000000 rskfd-0.3.4/rskfd.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-12 19:08:00.000000 rskfd-0.3.4/rskfd.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2022-10-12 19:08:00.000000 rskfd-0.3.4/rskfd.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2022-10-12 19:08:00.000000 rskfd-0.3.4/rskfd.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2022-10-12 19:08:00.956622 rskfd-0.3.4/setup.cfg
--rw-rw-rw-   0        0        0     1464 2022-10-12 19:07:33.000000 rskfd-0.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-08 09:07:48.696710 rskfd-0.3.5/
+-rw-rw-rw-   0        0        0     2204 2023-08-08 09:07:48.696710 rskfd-0.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1386 2020-07-13 06:29:17.000000 rskfd-0.3.5/README.md
+drwxrwxrwx   0        0        0        0 2023-08-08 09:07:48.665462 rskfd-0.3.5/examples/
+-rw-rw-rw-   0        0        0     3705 2023-02-16 10:45:21.000000 rskfd-0.3.5/examples/Wv2BinStream.py
+-rw-rw-rw-   0        0        0     1275 2022-10-12 18:58:52.000000 rskfd-0.3.5/examples/fileopening.py
+-rw-rw-rw-   0        0        0     6637 2020-10-13 07:00:50.000000 rskfd-0.3.5/examples/instrumentexamples.py
+-rw-rw-rw-   0        0        0     1082 2020-07-08 13:59:40.000000 rskfd-0.3.5/license.txt
+drwxrwxrwx   0        0        0        0 2023-08-08 09:07:48.665462 rskfd-0.3.5/rskfd/
+-rw-rw-rw-   0        0        0     1299 2023-03-15 14:55:14.000000 rskfd-0.3.5/rskfd/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-08 09:07:48.681087 rskfd-0.3.5/rskfd/helper/
+-rw-rw-rw-   0        0        0     4349 2023-03-15 14:58:05.000000 rskfd-0.3.5/rskfd/helper/helper.py
+drwxrwxrwx   0        0        0        0 2023-08-08 09:07:48.681087 rskfd-0.3.5/rskfd/iq_data_handling/
+-rw-rw-rw-   0        0        0    20946 2022-10-26 18:06:47.000000 rskfd-0.3.5/rskfd/iq_data_handling/iqdata.py
+drwxrwxrwx   0        0        0        0 2023-08-08 09:07:48.696710 rskfd-0.3.5/rskfd/remote_control/
+-rw-rw-rw-   0        0        0    14607 2022-10-05 09:04:02.000000 rskfd-0.3.5/rskfd/remote_control/instrument.py
+-rw-rw-rw-   0        0        0     1352 2022-06-15 06:04:19.000000 rskfd-0.3.5/rskfd/remote_control/instrumentRS.py
+-rw-rw-rw-   0        0        0      675 2019-12-09 13:08:45.000000 rskfd-0.3.5/rskfd/remote_control/instrumentRSExceptions.py
+-rw-rw-rw-   0        0        0     8506 2020-10-20 07:35:56.000000 rskfd-0.3.5/rskfd/remote_control/instrumentRS_FSW.py
+-rw-rw-rw-   0        0        0     1905 2019-12-09 13:10:19.000000 rskfd-0.3.5/rskfd/remote_control/instrumentRS_VSE.py
+drwxrwxrwx   0        0        0        0 2023-08-08 09:07:48.696710 rskfd-0.3.5/rskfd/signal_generation/
+-rw-rw-rw-   0        0        0     2290 2020-12-11 07:28:48.000000 rskfd-0.3.5/rskfd/signal_generation/signal_generation.py
+drwxrwxrwx   0        0        0        0 2023-08-08 09:07:48.696710 rskfd-0.3.5/rskfd/snp_handling/
+-rw-rw-rw-   0        0        0     9605 2021-03-16 15:49:04.000000 rskfd-0.3.5/rskfd/snp_handling/snpfiles.py
+drwxrwxrwx   0        0        0        0 2023-08-08 09:07:48.681087 rskfd-0.3.5/rskfd.egg-info/
+-rw-rw-rw-   0        0        0     2204 2023-08-08 09:07:48.000000 rskfd-0.3.5/rskfd.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      615 2023-08-08 09:07:48.000000 rskfd-0.3.5/rskfd.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 09:07:48.000000 rskfd-0.3.5/rskfd.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-08-08 09:07:48.000000 rskfd-0.3.5/rskfd.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       34 2023-08-08 09:07:48.000000 rskfd-0.3.5/rskfd.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-08-08 09:07:48.712335 rskfd-0.3.5/setup.cfg
+-rw-rw-rw-   0        0        0     1464 2023-08-08 07:51:28.000000 rskfd-0.3.5/setup.py
```

### Comparing `rskfd-0.3.4/PKG-INFO` & `rskfd-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rskfd
-Version: 0.3.4
+Version: 0.3.5
 Summary: Python Package for Instrument Control and Data Handling
 Home-page: https://gitlab.com/ramian/rskfd
 Download-URL: https://gitlab.com/ramian/rskfd/
 Author: Florian Ramian
 Author-email: gitlab@ramian.eu
 License: MIT
 Keywords: INSTRUMENT CONTROL,I/Q DATA,WV,IQ.TAR
```

### Comparing `rskfd-0.3.4/README.md` & `rskfd-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `rskfd-0.3.4/examples/Wv2BinStream.py` & `rskfd-0.3.5/examples/Wv2BinStream.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,78 +3,107 @@
 Created on Sun Dec 12 2021
 
 (C) 2021, Rohde&Schwarz, ramian
 """
 
 import struct
 import re
+import math
 
 
-def ConvertWv2BinStream( FileName):
+def ConvertWv2BinStream( FileName, bScale = False):
     '''
     Convert large wv files to bin (KS file format), i.e. do not read full iq vector
+    Note: bin file must not have a higher power than "1", use rescale option to make sure
     '''
     SampleSize = 4 # 2 x 2 bytes
     BlockSize = 50000
 
     try:
         file = open(FileName, "rb")
-        data = file.read( 6000)     # for the header, 62 kB should be sufficient
+        data = file.read( 30000)     # for the header, 30 kB should be sufficient
     except:
         print( "File open error ("+ FileName+")!")
 
     binaryStart = 0
     tags = ""
     Counter = 0
     ConverterSize = 20
     while (binaryStart == 0) & (Counter < len(data)):
         tags += data[Counter:Counter+ConverterSize].decode("ASCII","ignore")
         Counter += ConverterSize
         #{WAVEFORM-20001: #
         res = re.search("WAVEFORM.{0,20}:.{0,3}#",tags)
-        if res != None:
+        if res is not None:
             binaryStart = res.span()[1]
 
+    if binaryStart == 0:
+        print("Binary start not found!\n")
+
     if (Counter > len(data)) & (binaryStart == 0):
         print( "Required tags not found, potentially incompatible file format!")
 
     res = re.search("SAMPLES[ ]*:[ ]*(?P<NumberOfSamples>[0-9]*)[ ]*}",tags)
     if res:
         NumberOfSamples = int( res.group("NumberOfSamples"))
     else:
         NumberOfSamples = -1
     
     outFileName = FileName.lower().replace( '.wv', '.bin')
     outfile = open( outFileName, "wb")
 
-    data = data[binaryStart:]
-    data = data + file.read( SampleSize-(len(data) % SampleSize))
-    NumberOfInt16s = len(data)//2
-    SampleCount = NumberOfInt16s // 2
-    data = list(struct.unpack("h"*NumberOfInt16s, data))
-    for nIdx in range(NumberOfInt16s):
-        outfile.write( struct.pack(">h",data[nIdx]))
-
+    # data = data[binaryStart:]
+    # data = data + file.read( SampleSize-(len(data) % SampleSize))
+    # NumberOfInt16s = len(data)//2
+    # SampleCount = NumberOfInt16s // 2
+    # data = list(struct.unpack("h"*NumberOfInt16s, data))
+    # for nIdx in range(NumberOfInt16s):
+    #     if bScale:
+    #         outfile.write( struct.pack(">h",data[nIdx]))
+    fScaler = 1
+    if bScale:
+        # first loop only to find max
+        SampleCount = 0
+        file.seek(binaryStart)
+        fMaxPower = 0
+        while SampleCount < NumberOfSamples:
+            SamplesToRead = NumberOfSamples-SampleCount
+            if SamplesToRead > BlockSize:
+                SamplesToRead = BlockSize
+            data = file.read( SamplesToRead * SampleSize)
+            NumberOfInt16s = len(data)//2
+            data = list(struct.unpack("h"*NumberOfInt16s, data))
+            fData = list(map( lambda x: x/32767.0, data ))
+            for nIdx in range(0,len(fData)//2):
+                fMaxPower = max( [fMaxPower, fData[nIdx*2]**2 + fData[1+nIdx*2]**2])
+            SampleCount = SampleCount + SamplesToRead
+        fScaler = math.sqrt( fMaxPower)
     
+    SampleCount = 0
+    file.seek(binaryStart)
+    fMaxPower = 0
     while SampleCount < NumberOfSamples:
         SamplesToRead = NumberOfSamples-SampleCount
         if SamplesToRead > BlockSize:
             SamplesToRead = BlockSize
         data = file.read( SamplesToRead * SampleSize)
         NumberOfInt16s = len(data)//2
         data = list(struct.unpack("h"*NumberOfInt16s, data))
         for nIdx in range(NumberOfInt16s):
+            if bScale:
+                data[nIdx] = round( data[nIdx] / fScaler)
             outfile.write( struct.pack(">h",data[nIdx]))
         SampleCount = SampleCount + SamplesToRead
 
     file.close()
     outfile.close()
 
 
 
 if __name__ == "__main__":
-    pass
+    # pass
     # Testcode
-    # ConvertWv2BinStream(r'C:\Users\ramian\Documents\gitlab\demo files\DirectDPD.wv')
+    filename = r'C:\Users\ramian\Downloads\EVM_Eval_11be_320MHz_MCS13'
+    ConvertWv2BinStream( filename+'.wv', bScale=True)
     # import rskfd
-    # iq,fs = rskfd.ReadWv(r'C:\Users\ramian\Documents\gitlab\demo files\DirectDPD.wv')
-    # rskfd.WriteBin( iq,fs, r'C:\Users\ramian\Documents\gitlab\demo files\DirectDPD.bin.test')
+    # iq,fs = rskfd.ReadWv(filename + '.wv')
+    # rskfd.WriteBin( iq,fs, filename +'.bin')
```

### Comparing `rskfd-0.3.4/examples/fileopening.py` & `rskfd-0.3.5/examples/fileopening.py`

 * *Files identical despite different names*

### Comparing `rskfd-0.3.4/examples/instrumentexamples.py` & `rskfd-0.3.5/examples/instrumentexamples.py`

 * *Files identical despite different names*

### Comparing `rskfd-0.3.4/license.txt` & `rskfd-0.3.5/license.txt`

 * *Files identical despite different names*

### Comparing `rskfd-0.3.4/rskfd/__init__.py` & `rskfd-0.3.5/rskfd/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,8 +23,9 @@
 
 from .signal_generation.signal_generation import CreateWGNSignal
 from .signal_generation.signal_generation import LowPassFilter
 
 from .helper.helper import ShowLogFFT
 from .helper.helper import MeanPower
 from .helper.helper import MaxPower
-from .helper.helper import ConvertUnit
+from .helper.helper import ConvertUnit
+from .helper.helper import Scale2dBm
```

### Comparing `rskfd-0.3.4/rskfd/helper/helper.py` & `rskfd-0.3.5/rskfd/helper/helper.py`

 * *Files 10% similar despite different names*

```diff
@@ -71,14 +71,31 @@
     elif( outUnit == unit.watt):
         data = numpy.power( numpy.abs( data), 2) / impedance
 
     return data
 
 
 
+def Scale2dBm( vfcIqData, fTargetRMSPower):
+    '''
+    Scales an input data vector to a target mean power
+    vfcIqData:          input vector, any unit
+    fTargetRMSPower:    target RMS power
+    
+    Output vector will be in Volts over 50 Ohms
+    '''
+    import numpy
+        
+    fInputPower = MeanPower( vfcIqData)
+    vfcIqData = numpy.multiply( vfcIqData, 10**((fTargetRMSPower-fInputPower)/20))
+
+    return vfcIqData
+
+
+
 def MeanPower( data, inUnit=unit.volt, outUnit=unit.dBm, impedance = 50):
     """
     MeanPower calculates the mean power of an input vector
     data:       input vector
     inUnit:     input unit, default Volts
     outUnit:    output unit, default dBm
     impedance:  impedance for conversion from power to amplitude, default 50 Ohms
```

### Comparing `rskfd-0.3.4/rskfd/iq_data_handling/iqdata.py` & `rskfd-0.3.5/rskfd/iq_data_handling/iqdata.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,15 +121,17 @@
     return data
 
 
 
 def WriteBin( iqData, fSamplingRate, FileName):
     """Writes a bin file, e.g. for use on KS generators
     iqData can be a list of complex or list of floats (iqiqiq format mandatory).
-    writtenSamples = WriteBin("MyFile.bin",complexList, fs)"""
+    writtenSamples = WriteBin("MyFile.bin",complexList, fs)
+    Note: Max power is "1", i.e. I^2+Q^2<=1
+    """
 
     import struct
     from datetime import date
     import math
     import logging
 
     #check if iqData is complex
@@ -241,15 +243,15 @@
     from numpy import NaN
 
     try:
         file = open(FileName, "rb")
         if( ReadData):
             data = file.read()
         else:
-            data = file.read( 6000)     # for the header, 62 kB should be sufficient
+            data = file.read( 30000)     # for the header, 30 kB should be sufficient
         file.close()
     except:
         logging.error( "File open error ("+ FileName+")!")
 
     binaryStart = 0
     tags = ""
     Counter = 0
@@ -284,15 +286,15 @@
     res = re.search("Signal generated for SMx RMS level[ ]*:[ ]*(?P<RfRmsLevel>-?[0-9]*.?[0-9]*)[ ]*",tags)
     if res:
         RfRmsLevel = float( res.group("RfRmsLevel"))
     else:
         RfRmsLevel = NaN
 
     if ReadData:
-        data = list(struct.unpack("h"*NumberOfSamples*2, data[binaryStart:-1]))
+        data = list(struct.unpack("h"*NumberOfSamples*2, data[binaryStart:binaryStart+NumberOfSamples*4]))
         data = list(map( lambda x: x/32767.0, data ))
         data = Iqiq2Complex( data)
     
     if ReadData:
         return data,SamplingRate
     else:
         return SamplingRate,NumberOfSamples,RmsLevelOffset,RfRmsLevel
```

### Comparing `rskfd-0.3.4/rskfd/remote_control/instrument.py` & `rskfd-0.3.5/rskfd/remote_control/instrument.py`

 * *Files identical despite different names*

### Comparing `rskfd-0.3.4/rskfd/remote_control/instrumentRS.py` & `rskfd-0.3.5/rskfd/remote_control/instrumentRS.py`

 * *Files identical despite different names*

### Comparing `rskfd-0.3.4/rskfd/remote_control/instrumentRSExceptions.py` & `rskfd-0.3.5/rskfd/remote_control/instrumentRSExceptions.py`

 * *Files identical despite different names*

### Comparing `rskfd-0.3.4/rskfd/remote_control/instrumentRS_FSW.py` & `rskfd-0.3.5/rskfd/remote_control/instrumentRS_FSW.py`

 * *Files identical despite different names*

### Comparing `rskfd-0.3.4/rskfd/remote_control/instrumentRS_VSE.py` & `rskfd-0.3.5/rskfd/remote_control/instrumentRS_VSE.py`

 * *Files identical despite different names*

### Comparing `rskfd-0.3.4/rskfd/signal_generation/signal_generation.py` & `rskfd-0.3.5/rskfd/signal_generation/signal_generation.py`

 * *Files identical despite different names*

### Comparing `rskfd-0.3.4/rskfd/snp_handling/snpfiles.py` & `rskfd-0.3.5/rskfd/snp_handling/snpfiles.py`

 * *Files identical despite different names*

### Comparing `rskfd-0.3.4/rskfd.egg-info/PKG-INFO` & `rskfd-0.3.5/rskfd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rskfd
-Version: 0.3.4
+Version: 0.3.5
 Summary: Python Package for Instrument Control and Data Handling
 Home-page: https://gitlab.com/ramian/rskfd
 Download-URL: https://gitlab.com/ramian/rskfd/
 Author: Florian Ramian
 Author-email: gitlab@ramian.eu
 License: MIT
 Keywords: INSTRUMENT CONTROL,I/Q DATA,WV,IQ.TAR
```

### Comparing `rskfd-0.3.4/rskfd.egg-info/SOURCES.txt` & `rskfd-0.3.5/rskfd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rskfd-0.3.4/setup.py` & `rskfd-0.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
   long_description = filein.read()
 
 setuptools.setup(
   name = 'rskfd',
   #packages = ['rskfd','rskfd.remote_control','rskfd.iq_data_handling','rskfd.signal_generation','rskfd.helper'],
   #packages = setuptools.find_packages(),
   packages = setuptools.find_namespace_packages(),
-  version = '0.3.4',
+  version = '0.3.5',
   license='MIT',
   description = 'Python Package for Instrument Control and Data Handling',
   long_description = long_description,
   long_description_content_type = "text/markdown",
   author = 'Florian Ramian', 
   author_email = 'gitlab@ramian.eu',
   url = 'https://gitlab.com/ramian/rskfd',   # gitlab
```

