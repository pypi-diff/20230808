# Comparing `tmp/sccircuitbuilder-0.0.2.tar.gz` & `tmp/sccircuitbuilder-0.0.3.tar.gz`

## Comparing `sccircuitbuilder-0.0.2.tar` & `sccircuitbuilder-0.0.3.tar`

### file list

```diff
@@ -1,35 +1,39 @@
--rw-r--r--   0        0        0    10244 2020-02-02 00:00:00.000000 sccircuitbuilder-0.0.2/.DS_Store
--rw-r--r--   0        0        0     2418 2020-02-02 00:00:00.000000 sccircuitbuilder-0.0.2/demo/scqubits_circuit_hamiltonian.ipynb
--rw-r--r--   0        0        0   136985 2020-02-02 00:00:00.000000 sccircuitbuilder-0.0.2/demo/screenshot.png
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 sccircuitbuilder-0.0.2/demo/simple_circuit.circuit
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 sccircuitbuilder-0.0.2/demo/simple_circuit.yml
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 sccircuitbuilder-0.0.2/sccircuitbuilder/__init__.py
--rw-r--r--   0        0        0     7594 2020-02-02 00:00:00.000000 sccircuitbuilder-0.0.2/sccircuitbuilder/branch_element.py
--rw-r--r--   0        0        0    13348 2020-02-02 00:00:00.000000 sccircuitbuilder-0.0.2/sccircuitbuilder/canvas.py
--rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 sccircuitbuilder-0.0.2/sccircuitbuilder/canvas_element.py
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 sccircuitbuilder-0.0.2/sccircuitbuilder/caretaker.py
--rw-r--r--   0        0        0     6411 2020-02-02 00:00:00.000000 sccircuitbuilder-0.0.2/sccircuitbuilder/circuit.py
--rw-r--r--   0        0        0     8778 2020-02-02 00:00:00.000000 sccircuitbuilder-0.0.2/sccircuitbuilder/circuitbuilder.py
--rw-r--r--   0        0        0     6546 2020-02-02 00:00:00.000000 sccircuitbuilder-0.0.2/sccircuitbuilder/connection.py
--rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 sccircuitbuilder-0.0.2/sccircuitbuilder/constants.py
--rw-r--r--   0        0        0     4535 2020-02-02 00:00:00.000000 sccircuitbuilder-0.0.2/sccircuitbuilder/node.py
--rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 sccircuitbuilder-0.0.2/sccircuitbuilder/circuits/Cos2PhiQubit.circuit
--rw-r--r--   0        0        0     2223 2020-02-02 00:00:00.000000 sccircuitbuilder-0.0.2/sccircuitbuilder/circuits/FluxQubit.circuit
--rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 sccircuitbuilder-0.0.2/sccircuitbuilder/circuits/Fluxonium.circuit
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 sccircuitbuilder-0.0.2/sccircuitbuilder/circuits/Transmon.circuit
--rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 sccircuitbuilder-0.0.2/sccircuitbuilder/circuits/TunableTransmon.circuit
--rw-r--r--   0        0        0     2680 2020-02-02 00:00:00.000000 sccircuitbuilder-0.0.2/sccircuitbuilder/circuits/ZeroPi.circuit
--rw-r--r--   0        0        0     2562 2020-02-02 00:00:00.000000 sccircuitbuilder-0.0.2/sccircuitbuilder/elements/Inductor.svg
--rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 sccircuitbuilder-0.0.2/sccircuitbuilder/elements/JJ.svg
--rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 sccircuitbuilder-0.0.2/sccircuitbuilder/elements/capacitor.svg
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 sccircuitbuilder-0.0.2/sccircuitbuilder/elements/ground.svg
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 sccircuitbuilder-0.0.2/sccircuitbuilder/icons/clear.png
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 sccircuitbuilder-0.0.2/sccircuitbuilder/icons/redo.png
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 sccircuitbuilder-0.0.2/sccircuitbuilder/icons/rotate.png
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 sccircuitbuilder-0.0.2/sccircuitbuilder/icons/trash.png
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 sccircuitbuilder-0.0.2/sccircuitbuilder/icons/undo.png
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 sccircuitbuilder-0.0.2/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 sccircuitbuilder-0.0.2/LICENSE
--rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 sccircuitbuilder-0.0.2/README.md
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 sccircuitbuilder-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2263 2020-02-02 00:00:00.000000 sccircuitbuilder-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 sccircuitbuilder-0.0.3/.DS_Store
+-rw-r--r--   0        0        0     2418 2020-02-02 00:00:00.000000 sccircuitbuilder-0.0.3/demo/scqubits_circuit_hamiltonian.ipynb
+-rw-r--r--   0        0        0   136985 2020-02-02 00:00:00.000000 sccircuitbuilder-0.0.3/demo/screenshot.png
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 sccircuitbuilder-0.0.3/demo/simple_circuit.circuit
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 sccircuitbuilder-0.0.3/demo/simple_circuit.yml
+-rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 sccircuitbuilder-0.0.3/sccircuitbuilder/.DS_Store
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 sccircuitbuilder-0.0.3/sccircuitbuilder/__init__.py
+-rw-r--r--   0        0        0     7594 2020-02-02 00:00:00.000000 sccircuitbuilder-0.0.3/sccircuitbuilder/branch_element.py
+-rw-r--r--   0        0        0    13348 2020-02-02 00:00:00.000000 sccircuitbuilder-0.0.3/sccircuitbuilder/canvas.py
+-rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 sccircuitbuilder-0.0.3/sccircuitbuilder/canvas_element.py
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 sccircuitbuilder-0.0.3/sccircuitbuilder/caretaker.py
+-rw-r--r--   0        0        0     6411 2020-02-02 00:00:00.000000 sccircuitbuilder-0.0.3/sccircuitbuilder/circuit.py
+-rw-r--r--   0        0        0     8778 2020-02-02 00:00:00.000000 sccircuitbuilder-0.0.3/sccircuitbuilder/circuitbuilder.py
+-rw-r--r--   0        0        0     6676 2020-02-02 00:00:00.000000 sccircuitbuilder-0.0.3/sccircuitbuilder/connection.py
+-rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 sccircuitbuilder-0.0.3/sccircuitbuilder/constants.py
+-rw-r--r--   0        0        0     4444 2020-02-02 00:00:00.000000 sccircuitbuilder-0.0.3/sccircuitbuilder/node.py
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 sccircuitbuilder-0.0.3/sccircuitbuilder/circuits/.DS_Store
+-rw-r--r--   0        0        0     2612 2020-02-02 00:00:00.000000 sccircuitbuilder-0.0.3/sccircuitbuilder/circuits/Cos2PhiQubit.circuit
+-rw-r--r--   0        0        0     2623 2020-02-02 00:00:00.000000 sccircuitbuilder-0.0.3/sccircuitbuilder/circuits/FluxQubit.circuit
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 sccircuitbuilder-0.0.3/sccircuitbuilder/circuits/Fluxonium.circuit
+-rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 sccircuitbuilder-0.0.3/sccircuitbuilder/circuits/Transmon.circuit
+-rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 sccircuitbuilder-0.0.3/sccircuitbuilder/circuits/TunableTransmon.circuit
+-rw-r--r--   0        0        0     3294 2020-02-02 00:00:00.000000 sccircuitbuilder-0.0.3/sccircuitbuilder/circuits/ZeroPi.circuit
+-rw-r--r--   0        0        0     2562 2020-02-02 00:00:00.000000 sccircuitbuilder-0.0.3/sccircuitbuilder/elements/Inductor.svg
+-rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 sccircuitbuilder-0.0.3/sccircuitbuilder/elements/JJ.svg
+-rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 sccircuitbuilder-0.0.3/sccircuitbuilder/elements/capacitor.svg
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 sccircuitbuilder-0.0.3/sccircuitbuilder/elements/ground.svg
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 sccircuitbuilder-0.0.3/sccircuitbuilder/icons/.DS_Store
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 sccircuitbuilder-0.0.3/sccircuitbuilder/icons/clear.png
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 sccircuitbuilder-0.0.3/sccircuitbuilder/icons/redo.png
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 sccircuitbuilder-0.0.3/sccircuitbuilder/icons/rotate.png
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 sccircuitbuilder-0.0.3/sccircuitbuilder/icons/split.png
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 sccircuitbuilder-0.0.3/sccircuitbuilder/icons/trash.png
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 sccircuitbuilder-0.0.3/sccircuitbuilder/icons/undo.png
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 sccircuitbuilder-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 sccircuitbuilder-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 sccircuitbuilder-0.0.3/README.md
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 sccircuitbuilder-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 sccircuitbuilder-0.0.3/PKG-INFO
```

### Comparing `sccircuitbuilder-0.0.2/demo/scqubits_circuit_hamiltonian.ipynb` & `sccircuitbuilder-0.0.3/demo/scqubits_circuit_hamiltonian.ipynb`

 * *Files identical despite different names*

### Comparing `sccircuitbuilder-0.0.2/demo/screenshot.png` & `sccircuitbuilder-0.0.3/demo/screenshot.png`

 * *Files identical despite different names*

### Comparing `sccircuitbuilder-0.0.2/demo/simple_circuit.circuit` & `sccircuitbuilder-0.0.3/demo/simple_circuit.circuit`

 * *Files identical despite different names*

### Comparing `sccircuitbuilder-0.0.2/sccircuitbuilder/branch_element.py` & `sccircuitbuilder-0.0.3/sccircuitbuilder/branch_element.py`

 * *Files identical despite different names*

### Comparing `sccircuitbuilder-0.0.2/sccircuitbuilder/canvas.py` & `sccircuitbuilder-0.0.3/sccircuitbuilder/canvas.py`

 * *Files identical despite different names*

### Comparing `sccircuitbuilder-0.0.2/sccircuitbuilder/canvas_element.py` & `sccircuitbuilder-0.0.3/sccircuitbuilder/canvas_element.py`

 * *Files identical despite different names*

### Comparing `sccircuitbuilder-0.0.2/sccircuitbuilder/caretaker.py` & `sccircuitbuilder-0.0.3/sccircuitbuilder/caretaker.py`

 * *Files identical despite different names*

### Comparing `sccircuitbuilder-0.0.2/sccircuitbuilder/circuit.py` & `sccircuitbuilder-0.0.3/sccircuitbuilder/circuit.py`

 * *Files identical despite different names*

### Comparing `sccircuitbuilder-0.0.2/sccircuitbuilder/circuitbuilder.py` & `sccircuitbuilder-0.0.3/sccircuitbuilder/circuitbuilder.py`

 * *Files identical despite different names*

### Comparing `sccircuitbuilder-0.0.2/sccircuitbuilder/connection.py` & `sccircuitbuilder-0.0.3/sccircuitbuilder/connection.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from sccircuitbuilder.constants import *
 from sccircuitbuilder.canvas_element import CanvasElement
-from PySide6.QtGui import QPen, QColorConstants
+from PySide6.QtGui import QPen, QColorConstants, QAction, QIcon
 import numpy as np
 from PySide6.QtWidgets import QToolBar, QWidget, QSizePolicy, QPushButton
-
+import os
 
 class Connection(CanvasElement):
 
     def __init__(self, origin, dest, displacement, circuit):
         super().__init__(origin)
         self.anchors = []
         self.wires = []
@@ -74,14 +74,20 @@
                 head = wire
             if wire.origin is anchor:
                 tail = wire
         self.anchors.remove(anchor)
         self.circuit.remove_anchor(anchor)
         self.wires.remove(tail)
         head.dest = tail.dest
+
+    def toolbar(self, update):
+        if self.selected_anchor:
+            return self.selected_anchor.toolbar(update)
+        else:
+            return QToolBar()
     
     class ConnectionMomento:
         def __init__(self, connection):
             self.dest = connection.dest.idx
             self.anchors = []
             wire = connection.wires[0]
             while True: #add anchors in path order
@@ -210,17 +216,15 @@
         return None
     
     def delete(self):
         self.connection.remove_anchor(self)
 
     def toolbar(self, update):
         toolbar = QToolBar()
-        split = QPushButton("Delete")
+        delete = QAction("",toolbar)
+        delete.setIcon(QIcon(os.path.join(os.path.dirname(__file__),"icons/trash")))
         def deleteandupdate():
             self.delete()
             update()
-        split.clicked.connect(deleteandupdate)
-        toolbar.addWidget(split)
-        spacer = QWidget()
-        spacer.setSizePolicy(QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Ignored)
-        toolbar.addWidget(spacer)
+        delete.triggered.connect(deleteandupdate)
+        toolbar.addAction(delete)
         return toolbar
```

### Comparing `sccircuitbuilder-0.0.2/sccircuitbuilder/constants.py` & `sccircuitbuilder-0.0.3/sccircuitbuilder/constants.py`

 * *Files identical despite different names*

### Comparing `sccircuitbuilder-0.0.2/sccircuitbuilder/node.py` & `sccircuitbuilder-0.0.3/sccircuitbuilder/node.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from sccircuitbuilder.canvas_element import CanvasElement
 from sccircuitbuilder.constants import *
 from math import sin, cos, pi
 from PySide6.QtGui import QPen, QColorConstants, QPolygon, QIcon, QAction
 from PySide6.QtCore import QPoint
 from PySide6.QtWidgets import QToolBar, QWidget, QSizePolicy, QPushButton
 from numpy.linalg import matrix_power
+import os
 
 GROUND_RAD = .3*SPACING
 
 class Node(CanvasElement):
     def __init__(self, point, circuit):
         super().__init__(point.snaptogrid())
         
@@ -43,23 +44,21 @@
         pen = QPen(QColorConstants.Black, NODE_SIZE)
         painter.setPen(pen)
         painter.drawText(int(self.x+FONTSIZE), int(self.y-FONTSIZE), str(self.idx))
         painter.drawPoint(self.x, self.y)
     
     def toolbar(self, update):
         toolbar = QToolBar()
-        split = QPushButton("Split Node")
+        split = QAction("",toolbar)
+        split.setIcon(QIcon(os.path.join(os.path.dirname(__file__),"icons/split")))
         def splitandupdate():
             self.split()
             update()
-        split.clicked.connect(splitandupdate)
-        toolbar.addWidget(split)
-        spacer = QWidget()
-        spacer.setSizePolicy(QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Ignored)
-        toolbar.addWidget(spacer)
+        split.triggered.connect(splitandupdate)
+        toolbar.addAction(split)
         return toolbar
     
     def split(self):
         if len(self.elements) > 1:
             self.circuit.remove_node(self)
             for element in self.elements:
                 displacement = Point(0,0)
@@ -100,15 +99,14 @@
             update()
         rotate = QAction("",toolbar)
         rotate.setIcon(QIcon(os.path.join(os.path.dirname(__file__), "icons/rotate")))
         rotate.triggered.connect(rotateandupdate)
         toolbar.addAction(rotate)
 
         if not self.elements:
-            toolbar = QToolBar()
             delete = QAction("",toolbar)
             delete.setIcon(QIcon(os.path.join(os.path.dirname(__file__),"icons/trash")))
             def deleteandupdate():
                 self.delete()
                 update()
             delete.triggered.connect(deleteandupdate)
             toolbar.addAction(delete)
```

### Comparing `sccircuitbuilder-0.0.2/sccircuitbuilder/circuits/FluxQubit.circuit` & `sccircuitbuilder-0.0.3/sccircuitbuilder/circuits/Transmon.circuit`

 * *Files 27% similar despite different names*

```diff
@@ -1,139 +1,114 @@
-00000000: 8004 95a4 0800 0000 0000 008c 1873 6363  .............scc
+00000000: 8004 950a 0700 0000 0000 008c 1873 6363  .............scc
 00000010: 6972 6375 6974 6275 696c 6465 722e 6369  ircuitbuilder.ci
 00000020: 7263 7569 7494 8c16 4369 7263 7569 742e  rcuit...Circuit.
 00000030: 4369 7263 7569 744d 656d 656e 746f 9493  CircuitMemento..
 00000040: 9429 8194 7d94 288c 0663 7574 6f66 6694  .)..}.(..cutoff.
-00000050: 4b03 8c0f 6772 6f75 6e64 5f6d 656d 656e  K...ground_memen
-00000060: 746f 7394 5d94 288c 1573 6363 6972 6375  tos.].(..sccircu
-00000070: 6974 6275 696c 6465 722e 6e6f 6465 948c  itbuilder.node..
-00000080: 104e 6f64 652e 4e6f 6465 4d65 6d65 6e74  .Node.NodeMement
-00000090: 6f94 9394 2981 947d 9428 8c03 6964 7894  o...)..}.(..idx.
-000000a0: 4b08 8c03 6c6f 6394 8c1a 7363 6369 7263  K...loc...sccirc
-000000b0: 7569 7462 7569 6c64 6572 2e63 6f6e 7374  uitbuilder.const
-000000c0: 616e 7473 948c 0550 6f69 6e74 9493 9429  ants...Point...)
-000000d0: 8194 7d94 288c 0178 944b c88c 0179 944a  ..}.(..x.K...y.J
-000000e0: 38ff ffff 7562 8c03 726f 7494 4b02 7562  8...ub..rot.K.ub
-000000f0: 680a 2981 947d 9428 680d 4b09 680e 6811  h.)..}.(h.K.h.h.
-00000100: 2981 947d 9428 6814 8c15 6e75 6d70 792e  )..}.(h...numpy.
-00000110: 636f 7265 2e6d 756c 7469 6172 7261 7994  core.multiarray.
-00000120: 8c06 7363 616c 6172 9493 948c 056e 756d  ..scalar.....num
-00000130: 7079 948c 0564 7479 7065 9493 948c 0269  py...dtype.....i
-00000140: 3894 8988 8794 5294 284b 038c 013c 944e  8.....R.(K...<.N
-00000150: 4e4e 4aff ffff ff4a ffff ffff 4b00 7494  NNJ....J....K.t.
-00000160: 6243 089c ffff ffff ffff ff94 8694 5294  bC............R.
-00000170: 6815 681d 6823 4308 38ff ffff ffff ffff  h.h.h#C.8.......
-00000180: 9486 9452 9475 6268 164b 0275 6265 8c0d  ...R.ubh.K.ube..
-00000190: 6e6f 6465 5f6d 656d 656e 746f 7394 5d94  node_mementos.].
-000001a0: 2868 0a29 8194 7d94 2868 0d4b 0168 0e68  (h.)..}.(h.K.h.h
-000001b0: 1129 8194 7d94 2868 144b 3268 154b 3275  .)..}.(h.K2h.K2u
-000001c0: 6268 164b 0375 6268 0a29 8194 7d94 2868  bh.K.ubh.)..}.(h
-000001d0: 0d4b 0268 0e68 1129 8194 7d94 2868 144b  .K.h.h.)..}.(h.K
-000001e0: c868 154a 9cff ffff 7562 6816 4b01 7562  .h.J....ubh.K.ub
-000001f0: 680a 2981 947d 9428 680d 4b03 680e 6811  h.)..}.(h.K.h.h.
-00000200: 2981 947d 9428 6814 4a9c ffff ff68 154a  )..}.(h.J....h.J
-00000210: 9cff ffff 7562 6816 4b01 7562 658c 1065  ....ubh.K.ube..e
-00000220: 6c65 6d65 6e74 5f6d 656d 656e 746f 7394  lement_mementos.
-00000230: 5d94 288c 1f73 6363 6972 6375 6974 6275  ].(..sccircuitbu
-00000240: 696c 6465 722e 6272 616e 6368 5f65 6c65  ilder.branch_ele
-00000250: 6d65 6e74 948c 1c42 7261 6e63 6845 6c65  ment...BranchEle
-00000260: 6d65 6e74 2e45 6c65 6d65 6e74 4d6f 6d65  ment.ElementMome
-00000270: 6e74 6f94 9394 2981 947d 9428 8c05 6e6f  nto...)..}.(..no
-00000280: 6465 7394 5d94 284b 014b 0365 8c07 6772  des.].(K.K.e..gr
-00000290: 6f75 6e64 7394 5d94 8c04 6e61 6d65 948c  ounds.]...name..
-000002a0: 024a 4a94 680e 6811 2981 947d 9428 6814  .JJ.h.h.)..}.(h.
-000002b0: 4a9c ffff ff68 154b 0075 628c 0469 636f  J....h.K.ub..ico
-000002c0: 6e94 8c22 2e2f 7363 6369 7263 7569 7462  n.."./sccircuitb
-000002d0: 7569 6c64 6572 2f65 6c65 6d65 6e74 732f  uilder/elements/
-000002e0: 4a4a 2e73 7667 948c 0a70 726f 7065 7274  JJ.svg...propert
-000002f0: 6965 7394 7d94 288c 0245 4394 8c03 4563  ies.}.(..EC...Ec
-00000300: 3194 8c02 454a 948c 0345 6a31 9475 8c0a  1...EJ...Ej1.u..
-00000310: 636f 6e6e 5f6d 656d 6f73 945d 9428 8c1b  conn_memos.].(..
-00000320: 7363 6369 7263 7569 7462 7569 6c64 6572  sccircuitbuilder
-00000330: 2e63 6f6e 6e65 6374 696f 6e94 8c1c 436f  .connection...Co
-00000340: 6e6e 6563 7469 6f6e 2e43 6f6e 6e65 6374  nnection.Connect
-00000350: 696f 6e4d 6f6d 656e 746f 9493 9429 8194  ionMomento...)..
-00000360: 7d94 288c 0464 6573 7494 4b01 8c07 616e  }.(..dest.K...an
-00000370: 6368 6f72 7394 5d94 8c01 6494 6811 2981  chors.]...d.h.).
-00000380: 947d 9428 6814 681d 6823 4308 0000 0000  .}.(h.h.h#C.....
-00000390: 0000 0000 9486 9452 9468 1568 1d68 2343  .......R.h.h.h#C
-000003a0: 0801 0000 0000 0000 0094 8694 5294 7562  ............R.ub
-000003b0: 7562 6855 2981 947d 9428 6858 4b03 6859  ubhU)..}.(hXK.hY
-000003c0: 5d94 685b 6811 2981 947d 9428 6814 681d  ].h[h.)..}.(h.h.
-000003d0: 6823 4308 0000 0000 0000 0000 9486 9452  h#C............R
-000003e0: 9468 1568 1d68 2343 08ff ffff ffff ffff  .h.h.h#C........
-000003f0: ff94 8694 5294 7562 7562 6568 164b 0175  ....R.ububeh.K.u
-00000400: 6268 3e29 8194 7d94 2868 415d 9428 4b02  bh>)..}.(hA].(K.
-00000410: 4b01 6568 435d 9468 4568 4668 0e68 1129  K.ehC].hEhFh.h.)
-00000420: 8194 7d94 2868 144b c868 154b 0075 6268  ..}.(h.K.h.K.ubh
-00000430: 4968 4a68 4b7d 9428 684d 8c03 4563 3294  IhJhK}.(hM..Ec2.
-00000440: 684f 8c03 456a 3294 7568 515d 9428 6855  hO..Ej2.uhQ].(hU
-00000450: 2981 947d 9428 6858 4b02 6859 5d94 685b  )..}.(hXK.hY].h[
-00000460: 6811 2981 947d 9428 6814 681d 6823 4308  h.)..}.(h.h.h#C.
-00000470: 0000 0000 0000 0000 9486 9452 9468 1568  ...........R.h.h
-00000480: 1d68 2343 08ff ffff ffff ffff ff94 8694  .h#C............
-00000490: 5294 7562 7562 6855 2981 947d 9428 6858  R.ububhU)..}.(hX
-000004a0: 4b01 6859 5d94 685b 6811 2981 947d 9428  K.hY].h[h.)..}.(
-000004b0: 6814 681d 6823 4308 0000 0000 0000 0000  h.h.h#C.........
-000004c0: 9486 9452 9468 1568 1d68 2343 0801 0000  ...R.h.h.h#C....
-000004d0: 0000 0000 0094 8694 5294 7562 7562 6568  ........R.ububeh
-000004e0: 164b 0375 6268 3e29 8194 7d94 2868 415d  .K.ubh>)..}.(hA]
-000004f0: 944b 0261 6843 5d94 4b08 6168 458c 0143  .K.ahC].K.ahE..C
-00000500: 9468 0e68 1129 8194 7d94 2868 144b c868  .h.h.)..}.(h.K.h
-00000510: 154a 6aff ffff 7562 6849 8c29 2e2f 7363  .Jj...ubhI.)./sc
-00000520: 6369 7263 7569 7462 7569 6c64 6572 2f65  circuitbuilder/e
-00000530: 6c65 6d65 6e74 732f 6361 7061 6369 746f  lements/capacito
-00000540: 722e 7376 6794 684b 7d94 6893 8c02 4367  r.svg.hK}.h...Cg
-00000550: 9473 6851 5d94 2868 5529 8194 7d94 2868  .shQ].(hU)..}.(h
-00000560: 584b 0268 595d 9468 5b68 1129 8194 7d94  XK.hY].h[h.)..}.
-00000570: 2868 1468 1d68 2343 0800 0000 0000 0000  (h.h.h#C........
-00000580: 0094 8694 5294 6815 681d 6823 4308 0100  ....R.h.h.h#C...
-00000590: 0000 0000 0000 9486 9452 9475 6275 6268  .........R.ububh
-000005a0: 5529 8194 7d94 2868 584b 0868 595d 9468  U)..}.(hXK.hY].h
-000005b0: 5b68 1129 8194 7d94 2868 1468 1d68 2343  [h.)..}.(h.h.h#C
-000005c0: 0800 0000 0000 0000 0094 8694 5294 6815  ............R.h.
-000005d0: 681d 6823 4308 ffff ffff ffff ffff 9486  h.h#C...........
-000005e0: 9452 9475 6275 6265 6816 4b01 7562 683e  .R.ububeh.K.ubh>
-000005f0: 2981 947d 9428 6841 5d94 284b 034b 0265  )..}.(hA].(K.K.e
-00000600: 6843 5d94 6845 6846 680e 6811 2981 947d  hC].hEhFh.h.)..}
-00000610: 9428 6814 4b32 6815 4a9c ffff ff75 6268  .(h.K2h.J....ubh
-00000620: 4968 4a68 4b7d 9428 684d 8c03 434a 3394  IhJhK}.(hM..CJ3.
-00000630: 684f 8c03 454a 3394 7568 515d 9428 6855  hO..EJ3.uhQ].(hU
-00000640: 2981 947d 9428 6858 4b03 6859 5d94 685b  )..}.(hXK.hY].h[
-00000650: 6811 2981 947d 9428 6814 681d 6823 4308  h.)..}.(h.h.h#C.
-00000660: ffff ffff ffff ffff 9486 9452 9468 1568  ...........R.h.h
-00000670: 1d68 2343 0800 0000 0000 0000 0094 8694  .h#C............
-00000680: 5294 7562 7562 6855 2981 947d 9428 6858  R.ububhU)..}.(hX
-00000690: 4b02 6859 5d94 685b 6811 2981 947d 9428  K.hY].h[h.)..}.(
-000006a0: 6814 681d 6823 4308 0100 0000 0000 0000  h.h.h#C.........
-000006b0: 9486 9452 9468 1568 1d68 2343 0800 0000  ...R.h.h.h#C....
-000006c0: 0000 0000 0094 8694 5294 7562 7562 6568  ........R.ububeh
-000006d0: 164b 0075 6268 3e29 8194 7d94 2868 415d  .K.ubh>)..}.(hA]
-000006e0: 944b 0361 6843 5d94 4b09 6168 4568 9368  .K.ahC].K.ahEh.h
-000006f0: 0e68 1129 8194 7d94 2868 144a 9cff ffff  .h.)..}.(h.J....
-00000700: 6815 4a6a ffff ff75 6268 4968 9668 4b7d  h.Jj...ubhIh.hK}
-00000710: 9468 938c 0243 6794 7368 515d 9428 6855  .h...Cg.shQ].(hU
-00000720: 2981 947d 9428 6858 4b03 6859 5d94 685b  )..}.(hXK.hY].h[
-00000730: 6811 2981 947d 9428 6814 681d 6823 4308  h.)..}.(h.h.h#C.
-00000740: 0000 0000 0000 0000 9486 9452 9468 1568  ...........R.h.h
-00000750: 1d68 2343 0801 0000 0000 0000 0094 8694  .h#C............
-00000760: 5294 7562 7562 6855 2981 947d 9428 6858  R.ububhU)..}.(hX
-00000770: 4b09 6859 5d94 685b 6811 2981 947d 9428  K.hY].h[h.)..}.(
-00000780: 6814 681d 6823 4308 0000 0000 0000 0000  h.h.h#C.........
-00000790: 9486 9452 9468 1568 1d68 2343 08ff ffff  ...R.h.h.h#C....
-000007a0: ffff ffff ff94 8694 5294 7562 7562 6568  ........R.ububeh
-000007b0: 164b 0175 6265 8c13 636f 6e6e 6563 7469  .K.ube..connecti
-000007c0: 6f6e 5f6d 656d 656e 746f 7394 5d94 2868  on_mementos.].(h
-000007d0: 5529 8194 7d94 2868 584b 0168 595d 9468  U)..}.(hXK.hY].h
-000007e0: 5b68 5c75 6268 5529 8194 7d94 2868 584b  [h\ubhU)..}.(hXK
-000007f0: 0368 595d 9468 5b68 6775 6268 5529 8194  .hY].h[hgubhU)..
-00000800: 7d94 2868 584b 0268 595d 9468 5b68 7c75  }.(hXK.hY].h[h|u
-00000810: 6268 5529 8194 7d94 2868 584b 0168 595d  bhU)..}.(hXK.hY]
-00000820: 9468 5b68 8775 6268 5529 8194 7d94 2868  .h[h.ubhU)..}.(h
-00000830: 584b 0268 595d 9468 5b68 9d75 6268 5529  XK.hY].h[h.ubhU)
-00000840: 8194 7d94 2868 584b 0868 595d 9468 5b68  ..}.(hXK.hY].h[h
-00000850: a875 6268 5529 8194 7d94 2868 584b 0368  .ubhU)..}.(hXK.h
-00000860: 595d 9468 5b68 bd75 6268 5529 8194 7d94  Y].h[h.ubhU)..}.
-00000870: 2868 584b 0268 595d 9468 5b68 c875 6268  (hXK.hY].h[h.ubh
-00000880: 5529 8194 7d94 2868 584b 0368 595d 9468  U)..}.(hXK.hY].h
-00000890: 5b68 dc75 6268 5529 8194 7d94 2868 584b  [h.ubhU)..}.(hXK
-000008a0: 0968 595d 9468 5b68 e775 6265 7562 2e    .hY].h[h.ubeub.
+00000050: 4b02 8c0f 6772 6f75 6e64 5f6d 656d 656e  K...ground_memen
+00000060: 746f 7394 5d94 8c15 7363 6369 7263 7569  tos.]...sccircui
+00000070: 7462 7569 6c64 6572 2e6e 6f64 6594 8c10  tbuilder.node...
+00000080: 4e6f 6465 2e4e 6f64 654d 656d 656e 746f  Node.NodeMemento
+00000090: 9493 9429 8194 7d94 288c 0369 6478 944b  ...)..}.(..idx.K
+000000a0: 078c 036c 6f63 948c 1a73 6363 6972 6375  ...loc...sccircu
+000000b0: 6974 6275 696c 6465 722e 636f 6e73 7461  itbuilder.consta
+000000c0: 6e74 7394 8c05 506f 696e 7494 9394 2981  nts...Point...).
+000000d0: 947d 9428 8c01 7894 4b64 8c01 7994 4a6a  .}.(..x.Kd..y.Jj
+000000e0: ffff ff75 628c 0372 6f74 944b 0275 6261  ...ub..rot.K.uba
+000000f0: 8c0d 6e6f 6465 5f6d 656d 656e 746f 7394  ..node_mementos.
+00000100: 5d94 2868 0a29 8194 7d94 2868 0d4b 0168  ].(h.)..}.(h.K.h
+00000110: 0e68 1129 8194 7d94 2868 144b 6468 154b  .h.)..}.(h.Kdh.K
+00000120: 9675 6268 164b 0175 6268 0a29 8194 7d94  .ubh.K.ubh.)..}.
+00000130: 2868 0d4b 0268 0e68 1129 8194 7d94 2868  (h.K.h.h.)..}.(h
+00000140: 148c 156e 756d 7079 2e63 6f72 652e 6d75  ...numpy.core.mu
+00000150: 6c74 6961 7272 6179 948c 0673 6361 6c61  ltiarray...scala
+00000160: 7294 9394 8c05 6e75 6d70 7994 8c05 6474  r.....numpy...dt
+00000170: 7970 6594 9394 8c02 6938 9489 8887 9452  ype.....i8.....R
+00000180: 9428 4b03 8c01 3c94 4e4e 4e4a ffff ffff  .(K...<.NNNJ....
+00000190: 4aff ffff ff4b 0074 9462 4308 6400 0000  J....K.t.bC.d...
+000001a0: 0000 0000 9486 9452 9468 1568 2368 2943  .......R.h.h#h)C
+000001b0: 08ce ffff ffff ffff ff94 8694 5294 7562  ............R.ub
+000001c0: 6816 4b01 7562 658c 1065 6c65 6d65 6e74  h.K.ube..element
+000001d0: 5f6d 656d 656e 746f 7394 5d94 288c 1f73  _mementos.].(..s
+000001e0: 6363 6972 6375 6974 6275 696c 6465 722e  ccircuitbuilder.
+000001f0: 6272 616e 6368 5f65 6c65 6d65 6e74 948c  branch_element..
+00000200: 1c42 7261 6e63 6845 6c65 6d65 6e74 2e45  .BranchElement.E
+00000210: 6c65 6d65 6e74 4d6f 6d65 6e74 6f94 9394  lementMomento...
+00000220: 2981 947d 9428 8c05 6e6f 6465 7394 5d94  )..}.(..nodes.].
+00000230: 284b 014b 0265 8c07 6772 6f75 6e64 7394  (K.K.e..grounds.
+00000240: 5d94 8c04 6e61 6d65 948c 024a 4a94 680e  ]...name...JJ.h.
+00000250: 6811 2981 947d 9428 6814 4b00 6815 4b32  h.)..}.(h.K.h.K2
+00000260: 7562 8c04 6963 6f6e 948c 632f 6f70 742f  ub..icon..c/opt/
+00000270: 686f 6d65 6272 6577 2f43 6173 6b72 6f6f  homebrew/Caskroo
+00000280: 6d2f 6d69 6e69 636f 6e64 612f 6261 7365  m/miniconda/base
+00000290: 2f6c 6962 2f70 7974 686f 6e33 2e31 302f  /lib/python3.10/
+000002a0: 7369 7465 2d70 6163 6b61 6765 732f 7363  site-packages/sc
+000002b0: 6369 7263 7569 7462 7569 6c64 6572 2f65  circuitbuilder/e
+000002c0: 6c65 6d65 6e74 732f 4a4a 2e73 7667 948c  lements/JJ.svg..
+000002d0: 0a70 726f 7065 7274 6965 7394 7d94 288c  .properties.}.(.
+000002e0: 0245 4394 8c02 4543 948c 0245 4a94 8c02  .EC...EC...EJ...
+000002f0: 454a 9475 8c0a 636f 6e6e 5f6d 656d 6f73  EJ.u..conn_memos
+00000300: 945d 9428 8c1b 7363 6369 7263 7569 7462  .].(..sccircuitb
+00000310: 7569 6c64 6572 2e63 6f6e 6e65 6374 696f  uilder.connectio
+00000320: 6e94 8c1c 436f 6e6e 6563 7469 6f6e 2e43  n...Connection.C
+00000330: 6f6e 6e65 6374 696f 6e4d 6f6d 656e 746f  onnectionMomento
+00000340: 9493 9429 8194 7d94 288c 0464 6573 7494  ...)..}.(..dest.
+00000350: 4b01 8c07 616e 6368 6f72 7394 5d94 8c01  K...anchors.]...
+00000360: 6494 6811 2981 947d 9428 6814 6823 6829  d.h.)..}.(h.h#h)
+00000370: 4308 0000 0000 0000 0000 9486 9452 9468  C............R.h
+00000380: 1568 2368 2943 0801 0000 0000 0000 0094  .h#h)C..........
+00000390: 8694 5294 7562 7562 684d 2981 947d 9428  ..R.ububhM)..}.(
+000003a0: 6850 4b02 6851 5d94 6853 6811 2981 947d  hPK.hQ].hSh.)..}
+000003b0: 9428 6814 6823 6829 4308 0000 0000 0000  .(h.h#h)C.......
+000003c0: 0000 9486 9452 9468 1568 2368 2943 08ff  .....R.h.h#h)C..
+000003d0: ffff ffff ffff ff94 8694 5294 7562 7562  ..........R.ubub
+000003e0: 6568 164b 0175 6268 3629 8194 7d94 2868  eh.K.ubh6)..}.(h
+000003f0: 395d 9428 4b01 4b02 6568 3b5d 9468 3d8c  9].(K.K.eh;].h=.
+00000400: 0143 9468 0e68 1129 8194 7d94 2868 144b  .C.h.h.)..}.(h.K
+00000410: c868 154b 3275 6268 418c 6a2f 6f70 742f  .h.K2ubhA.j/opt/
+00000420: 686f 6d65 6272 6577 2f43 6173 6b72 6f6f  homebrew/Caskroo
+00000430: 6d2f 6d69 6e69 636f 6e64 612f 6261 7365  m/miniconda/base
+00000440: 2f6c 6962 2f70 7974 686f 6e33 2e31 302f  /lib/python3.10/
+00000450: 7369 7465 2d70 6163 6b61 6765 732f 7363  site-packages/sc
+00000460: 6369 7263 7569 7462 7569 6c64 6572 2f65  circuitbuilder/e
+00000470: 6c65 6d65 6e74 732f 6361 7061 6369 746f  lements/capacito
+00000480: 722e 7376 6794 6843 7d94 686b 686b 7368  r.svg.hC}.hkhksh
+00000490: 495d 9428 684d 2981 947d 9428 6850 4b01  I].(hM)..}.(hPK.
+000004a0: 6851 5d94 6853 6811 2981 947d 9428 6814  hQ].hSh.)..}.(h.
+000004b0: 6823 6829 4308 0000 0000 0000 0000 9486  h#h)C...........
+000004c0: 9452 9468 1568 2368 2943 0801 0000 0000  .R.h.h#h)C......
+000004d0: 0000 0094 8694 5294 7562 7562 684d 2981  ......R.ububhM).
+000004e0: 947d 9428 6850 4b02 6851 5d94 6853 6811  .}.(hPK.hQ].hSh.
+000004f0: 2981 947d 9428 6814 6823 6829 4308 0000  )..}.(h.h#h)C...
+00000500: 0000 0000 0000 9486 9452 9468 1568 2368  .........R.h.h#h
+00000510: 2943 08ff ffff ffff ffff ff94 8694 5294  )C............R.
+00000520: 7562 7562 6568 164b 0175 6268 3629 8194  ububeh.K.ubh6)..
+00000530: 7d94 2868 395d 944b 0261 683b 5d94 4b07  }.(h9].K.ah;].K.
+00000540: 6168 3d68 6b68 0e68 1129 8194 7d94 2868  ah=hkh.h.)..}.(h
+00000550: 144b 6468 154a 9cff ffff 7562 6841 8c6a  .Kdh.J....ubhA.j
+00000560: 2f6f 7074 2f68 6f6d 6562 7265 772f 4361  /opt/homebrew/Ca
+00000570: 736b 726f 6f6d 2f6d 696e 6963 6f6e 6461  skroom/miniconda
+00000580: 2f62 6173 652f 6c69 622f 7079 7468 6f6e  /base/lib/python
+00000590: 332e 3130 2f73 6974 652d 7061 636b 6167  3.10/site-packag
+000005a0: 6573 2f73 6363 6972 6375 6974 6275 696c  es/sccircuitbuil
+000005b0: 6465 722f 656c 656d 656e 7473 2f63 6170  der/elements/cap
+000005c0: 6163 6974 6f72 2e73 7667 9468 437d 9468  acitor.svg.hC}.h
+000005d0: 6b8c 0243 6794 7368 495d 9428 684d 2981  k..Cg.shI].(hM).
+000005e0: 947d 9428 6850 4b02 6851 5d94 6853 6811  .}.(hPK.hQ].hSh.
+000005f0: 2981 947d 9428 6814 6823 6829 4308 0000  )..}.(h.h#h)C...
+00000600: 0000 0000 0000 9486 9452 9468 1568 2368  .........R.h.h#h
+00000610: 2943 0801 0000 0000 0000 0094 8694 5294  )C............R.
+00000620: 7562 7562 684d 2981 947d 9428 6850 4b07  ububhM)..}.(hPK.
+00000630: 6851 5d94 6853 6811 2981 947d 9428 6814  hQ].hSh.)..}.(h.
+00000640: 6823 6829 4308 0000 0000 0000 0000 9486  h#h)C...........
+00000650: 9452 9468 1568 2368 2943 08ff ffff ffff  .R.h.h#h)C......
+00000660: ffff ff94 8694 5294 7562 7562 6568 164b  ......R.ububeh.K
+00000670: 0175 6265 8c13 636f 6e6e 6563 7469 6f6e  .ube..connection
+00000680: 5f6d 656d 656e 746f 7394 5d94 2868 4d29  _mementos.].(hM)
+00000690: 8194 7d94 2868 504b 0168 515d 9468 5368  ..}.(hPK.hQ].hSh
+000006a0: 5475 6268 4d29 8194 7d94 2868 504b 0268  TubhM)..}.(hPK.h
+000006b0: 515d 9468 5368 5f75 6268 4d29 8194 7d94  Q].hSh_ubhM)..}.
+000006c0: 2868 504b 0168 515d 9468 5368 7475 6268  (hPK.hQ].hShtubh
+000006d0: 4d29 8194 7d94 2868 504b 0268 515d 9468  M)..}.(hPK.hQ].h
+000006e0: 5368 7f75 6268 4d29 8194 7d94 2868 504b  Sh.ubhM)..}.(hPK
+000006f0: 0268 515d 9468 5368 9475 6268 4d29 8194  .hQ].hSh.ubhM)..
+00000700: 7d94 2868 504b 0768 515d 9468 5368 9f75  }.(hPK.hQ].hSh.u
+00000710: 6265 7562 2e                             beub.
```

### Comparing `sccircuitbuilder-0.0.2/sccircuitbuilder/circuits/ZeroPi.circuit` & `sccircuitbuilder-0.0.3/sccircuitbuilder/circuits/TunableTransmon.circuit`

 * *Files 22% similar despite different names*

```diff
@@ -1,168 +1,137 @@
-00000000: 8004 956d 0a00 0000 0000 008c 1873 6363  ...m.........scc
+00000000: 8004 9583 0800 0000 0000 008c 1873 6363  .............scc
 00000010: 6972 6375 6974 6275 696c 6465 722e 6369  ircuitbuilder.ci
 00000020: 7263 7569 7494 8c16 4369 7263 7569 742e  rcuit...Circuit.
 00000030: 4369 7263 7569 744d 656d 656e 746f 9493  CircuitMemento..
 00000040: 9429 8194 7d94 288c 0663 7574 6f66 6694  .)..}.(..cutoff.
-00000050: 4b04 8c0f 6772 6f75 6e64 5f6d 656d 656e  K...ground_memen
+00000050: 4b02 8c0f 6772 6f75 6e64 5f6d 656d 656e  K...ground_memen
 00000060: 746f 7394 5d94 8c15 7363 6369 7263 7569  tos.]...sccircui
 00000070: 7462 7569 6c64 6572 2e6e 6f64 6594 8c10  tbuilder.node...
 00000080: 4e6f 6465 2e4e 6f64 654d 656d 656e 746f  Node.NodeMemento
 00000090: 9493 9429 8194 7d94 288c 0369 6478 944b  ...)..}.(..idx.K
-000000a0: 098c 036c 6f63 948c 1a73 6363 6972 6375  ...loc...sccircu
+000000a0: 078c 036c 6f63 948c 1a73 6363 6972 6375  ...loc...sccircu
 000000b0: 6974 6275 696c 6465 722e 636f 6e73 7461  itbuilder.consta
 000000c0: 6e74 7394 8c05 506f 696e 7494 9394 2981  nts...Point...).
-000000d0: 947d 9428 8c01 7894 4a06 ffff ff8c 0179  .}.(..x.J......y
-000000e0: 944a 6aff ffff 7562 8c03 726f 7494 4b03  .Jj...ub..rot.K.
-000000f0: 7562 618c 0d6e 6f64 655f 6d65 6d65 6e74  uba..node_mement
-00000100: 6f73 945d 9428 680a 2981 947d 9428 680d  os.].(h.)..}.(h.
-00000110: 4b01 680e 6811 2981 947d 9428 6814 4bfa  K.h.h.)..}.(h.K.
-00000120: 6815 4a6a ffff ff75 6268 164b 0075 6268  h.Jj...ubh.K.ubh
-00000130: 0a29 8194 7d94 2868 0d4b 0268 0e68 1129  .)..}.(h.K.h.h.)
-00000140: 8194 7d94 2868 144a 6aff ffff 6815 4a6a  ..}.(h.Jj...h.Jj
-00000150: ffff ff75 6268 164b 0175 6268 0a29 8194  ...ubh.K.ubh.)..
-00000160: 7d94 2868 0d4b 0368 0e68 1129 8194 7d94  }.(h.K.h.h.)..}.
-00000170: 2868 144b 9668 154b 9675 6268 164b 0075  (h.K.h.K.ubh.K.u
-00000180: 6268 0a29 8194 7d94 2868 0d4b 0468 0e68  bh.)..}.(h.K.h.h
-00000190: 1129 8194 7d94 2868 144a 6aff ffff 6815  .)..}.(h.Jj...h.
-000001a0: 4b96 7562 6816 4b01 7562 658c 1065 6c65  K.ubh.K.ube..ele
-000001b0: 6d65 6e74 5f6d 656d 656e 746f 7394 5d94  ment_mementos.].
-000001c0: 288c 1f73 6363 6972 6375 6974 6275 696c  (..sccircuitbuil
-000001d0: 6465 722e 6272 616e 6368 5f65 6c65 6d65  der.branch_eleme
-000001e0: 6e74 948c 1c42 7261 6e63 6845 6c65 6d65  nt...BranchEleme
-000001f0: 6e74 2e45 6c65 6d65 6e74 4d6f 6d65 6e74  nt.ElementMoment
-00000200: 6f94 9394 2981 947d 9428 8c05 6e6f 6465  o...)..}.(..node
-00000210: 7394 5d94 284b 024b 0165 8c07 6772 6f75  s.].(K.K.e..grou
-00000220: 6e64 7394 5d94 8c04 6e61 6d65 948c 024a  nds.]...name...J
-00000230: 4a94 680e 6811 2981 947d 9428 6814 4b00  J.h.h.)..}.(h.K.
-00000240: 6815 4a6a ffff ff75 628c 0469 636f 6e94  h.Jj...ub..icon.
-00000250: 8c22 2e2f 7363 6369 7263 7569 7462 7569  ."./sccircuitbui
-00000260: 6c64 6572 2f65 6c65 6d65 6e74 732f 4a4a  lder/elements/JJ
-00000270: 2e73 7667 948c 0a70 726f 7065 7274 6965  .svg...propertie
-00000280: 7394 7d94 288c 0245 4394 8c03 4563 3294  s.}.(..EC...Ec2.
-00000290: 8c02 454a 948c 0345 6a32 9475 8c0a 636f  ..EJ...Ej2.u..co
-000002a0: 6e6e 5f6d 656d 6f73 945d 9428 8c1b 7363  nn_memos.].(..sc
-000002b0: 6369 7263 7569 7462 7569 6c64 6572 2e63  circuitbuilder.c
-000002c0: 6f6e 6e65 6374 696f 6e94 8c1c 436f 6e6e  onnection...Conn
-000002d0: 6563 7469 6f6e 2e43 6f6e 6e65 6374 696f  ection.Connectio
-000002e0: 6e4d 6f6d 656e 746f 9493 9429 8194 7d94  nMomento...)..}.
-000002f0: 288c 0464 6573 7494 4b02 8c07 616e 6368  (..dest.K...anch
-00000300: 6f72 7394 5d94 8c01 6494 6811 2981 947d  ors.]...d.h.)..}
-00000310: 9428 6814 4aff ffff ff68 154b 0075 6275  .(h.J....h.K.ubu
-00000320: 6268 4429 8194 7d94 2868 474b 0168 485d  bhD)..}.(hGK.hH]
-00000330: 9468 4a68 1129 8194 7d94 2868 144b 0168  .hJh.)..}.(h.K.h
-00000340: 154b 0075 6275 6265 6816 4b00 7562 682d  .K.ububeh.K.ubh-
-00000350: 2981 947d 9428 6830 5d94 284b 044b 0265  )..}.(h0].(K.K.e
-00000360: 6832 5d94 6834 8c01 4c94 680e 6811 2981  h2].h4..L.h.h.).
-00000370: 947d 9428 6814 4a6a ffff ff68 154b 0075  .}.(h.Jj...h.K.u
-00000380: 6268 388c 282e 2f73 6363 6972 6375 6974  bh8.(./sccircuit
-00000390: 6275 696c 6465 722f 656c 656d 656e 7473  builder/elements
-000003a0: 2f49 6e64 7563 746f 722e 7376 6794 683a  /Inductor.svg.h:
-000003b0: 7d94 6856 8c01 4c94 7368 405d 9428 6844  }.hV..L.sh@].(hD
-000003c0: 2981 947d 9428 6847 4b04 6848 5d94 684a  )..}.(hGK.hH].hJ
-000003d0: 6811 2981 947d 9428 6814 8c15 6e75 6d70  h.)..}.(h...nump
-000003e0: 792e 636f 7265 2e6d 756c 7469 6172 7261  y.core.multiarra
-000003f0: 7994 8c06 7363 616c 6172 9493 948c 056e  y...scalar.....n
-00000400: 756d 7079 948c 0564 7479 7065 9493 948c  umpy...dtype....
-00000410: 0269 3894 8988 8794 5294 284b 038c 013c  .i8.....R.(K...<
-00000420: 944e 4e4e 4aff ffff ff4a ffff ffff 4b00  .NNNJ....J....K.
-00000430: 7494 6243 0800 0000 0000 0000 0094 8694  t.bC............
-00000440: 5294 6815 6864 686a 4308 0100 0000 0000  R.h.hdhjC.......
-00000450: 0000 9486 9452 9475 6275 6268 4429 8194  .....R.ububhD)..
-00000460: 7d94 2868 474b 0268 485d 9468 4a68 1129  }.(hGK.hH].hJh.)
-00000470: 8194 7d94 2868 1468 6468 6a43 0800 0000  ..}.(h.hdhjC....
-00000480: 0000 0000 0094 8694 5294 6815 6864 686a  ........R.h.hdhj
-00000490: 4308 ffff ffff ffff ffff 9486 9452 9475  C............R.u
-000004a0: 6275 6265 6816 4b01 7562 682d 2981 947d  bubeh.K.ubh-)..}
-000004b0: 9428 6830 5d94 284b 034b 0165 6832 5d94  .(h0].(K.K.eh2].
-000004c0: 6834 6856 680e 6811 2981 947d 9428 6814  h4hVh.h.)..}.(h.
-000004d0: 4b96 6815 4b00 7562 6838 6859 683a 7d94  K.h.K.ubh8hYh:}.
-000004e0: 6856 685b 7368 405d 9428 6844 2981 947d  hVh[sh@].(hD)..}
-000004f0: 9428 6847 4b03 6848 5d94 684a 6811 2981  .(hGK.hH].hJh.).
-00000500: 947d 9428 6814 6864 686a 4308 0000 0000  .}.(h.hdhjC.....
-00000510: 0000 0000 9486 9452 9468 1568 6468 6a43  .......R.h.hdhjC
-00000520: 0801 0000 0000 0000 0094 8694 5294 7562  ............R.ub
-00000530: 7562 6844 2981 947d 9428 6847 4b01 6848  ubhD)..}.(hGK.hH
-00000540: 5d94 684a 6811 2981 947d 9428 6814 6864  ].hJh.)..}.(h.hd
-00000550: 686a 4308 0000 0000 0000 0000 9486 9452  hjC............R
-00000560: 9468 1568 6468 6a43 08ff ffff ffff ffff  .h.hdhjC........
-00000570: ff94 8694 5294 7562 7562 6568 164b 0175  ....R.ububeh.K.u
-00000580: 6268 2d29 8194 7d94 2868 305d 9428 4b04  bh-)..}.(h0].(K.
-00000590: 4b03 6568 325d 9468 3468 3568 0e68 1129  K.eh2].h4h5h.h.)
-000005a0: 8194 7d94 2868 144b 0068 154b 9675 6268  ..}.(h.K.h.K.ubh
-000005b0: 3868 3968 3a7d 9428 683c 8c03 4563 3194  8h9h:}.(h<..Ec1.
-000005c0: 683e 8c03 456a 3194 7568 405d 9428 6844  h>..Ej1.uh@].(hD
-000005d0: 2981 947d 9428 6847 4b04 6848 5d94 684a  )..}.(hGK.hH].hJ
-000005e0: 6811 2981 947d 9428 6814 6864 686a 4308  h.)..}.(h.hdhjC.
-000005f0: ffff ffff ffff ffff 9486 9452 9468 1568  ...........R.h.h
-00000600: 6468 6a43 0800 0000 0000 0000 0094 8694  dhjC............
-00000610: 5294 7562 7562 6844 2981 947d 9428 6847  R.ububhD)..}.(hG
-00000620: 4b03 6848 5d94 684a 6811 2981 947d 9428  K.hH].hJh.)..}.(
-00000630: 6814 6864 686a 4308 0100 0000 0000 0000  h.hdhjC.........
-00000640: 9486 9452 9468 1568 6468 6a43 0800 0000  ...R.h.hdhjC....
-00000650: 0000 0000 0094 8694 5294 7562 7562 6568  ........R.ububeh
-00000660: 164b 0075 6268 2d29 8194 7d94 2868 305d  .K.ubh-)..}.(h0]
-00000670: 944b 0261 6832 5d94 4b09 6168 348c 0143  .K.ah2].K.ah4..C
-00000680: 9468 0e68 1129 8194 7d94 2868 144a 38ff  .h.h.)..}.(h.J8.
-00000690: ffff 6815 4a6a ffff ff75 6268 388c 292e  ..h.Jj...ubh8.).
-000006a0: 2f73 6363 6972 6375 6974 6275 696c 6465  /sccircuitbuilde
-000006b0: 722f 656c 656d 656e 7473 2f63 6170 6163  r/elements/capac
-000006c0: 6974 6f72 2e73 7667 9468 3a7d 9468 c08c  itor.svg.h:}.h..
-000006d0: 0243 6794 7368 405d 9428 6844 2981 947d  .Cg.sh@].(hD)..}
-000006e0: 9428 6847 4b09 6848 5d94 684a 6811 2981  .(hGK.hH].hJh.).
-000006f0: 947d 9428 6814 4aff ffff ff68 154b 0075  .}.(h.J....h.K.u
-00000700: 6275 6268 4429 8194 7d94 2868 474b 0268  bubhD)..}.(hGK.h
-00000710: 485d 9468 4a68 1129 8194 7d94 2868 144b  H].hJh.)..}.(h.K
-00000720: 0168 154b 0075 6275 6265 6816 4b00 7562  .h.K.ububeh.K.ub
-00000730: 682d 2981 947d 9428 6830 5d94 284b 024b  h-)..}.(h0].(K.K
-00000740: 0365 6832 5d94 6834 68c0 680e 6811 2981  .eh2].h4h.h.h.).
-00000750: 947d 9428 6814 4b00 6815 4b00 7562 6838  .}.(h.K.h.K.ubh8
-00000760: 68c3 683a 7d94 68c0 8c01 4394 7368 405d  h.h:}.h...C.sh@]
-00000770: 9428 6844 2981 947d 9428 6847 4b02 6848  .(hD)..}.(hGK.hH
-00000780: 5d94 6811 2981 947d 9428 6814 4ace ffff  ].h.)..}.(h.J...
-00000790: ff68 154a 9cff ffff 7562 6168 4a68 1129  .h.J....ubahJh.)
-000007a0: 8194 7d94 2868 144a ffff ffff 6815 4b00  ..}.(h.J....h.K.
-000007b0: 7562 7562 6844 2981 947d 9428 6847 4b03  ububhD)..}.(hGK.
-000007c0: 6848 5d94 6811 2981 947d 9428 6814 4b64  hH].h.)..}.(h.Kd
-000007d0: 6815 4b64 7562 6168 4a68 1129 8194 7d94  h.KdubahJh.)..}.
-000007e0: 2868 144b 0168 154b 0075 6275 6265 6816  (h.K.h.K.ububeh.
-000007f0: 4b00 7562 682d 2981 947d 9428 6830 5d94  K.ubh-)..}.(h0].
-00000800: 284b 044b 0165 6832 5d94 6834 68c0 680e  (K.K.eh2].h4h.h.
-00000810: 6811 2981 947d 9428 6814 4bfa 6815 4b32  h.)..}.(h.K.h.K2
-00000820: 7562 6838 68c3 683a 7d94 68c0 68d8 7368  ubh8h.h:}.h.h.sh
-00000830: 405d 9428 6844 2981 947d 9428 6847 4b04  @].(hD)..}.(hGK.
-00000840: 6848 5d94 6811 2981 947d 9428 6814 4a6a  hH].h.)..}.(h.Jj
-00000850: ffff ff68 154b c875 6261 684a 6811 2981  ...h.K.ubahJh.).
-00000860: 947d 9428 6814 6864 686a 4308 0000 0000  .}.(h.hdhjC.....
-00000870: 0000 0000 9486 9452 9468 1568 6468 6a43  .......R.h.hdhjC
-00000880: 0801 0000 0000 0000 0094 8694 5294 7562  ............R.ub
-00000890: 7562 6844 2981 947d 9428 6847 4b01 6848  ubhD)..}.(hGK.hH
-000008a0: 5d94 684a 6811 2981 947d 9428 6814 6864  ].hJh.)..}.(h.hd
-000008b0: 686a 4308 0000 0000 0000 0000 9486 9452  hjC............R
-000008c0: 9468 1568 6468 6a43 08ff ffff ffff ffff  .h.hdhjC........
-000008d0: ff94 8694 5294 7562 7562 6568 164b 0175  ....R.ububeh.K.u
-000008e0: 6265 8c13 636f 6e6e 6563 7469 6f6e 5f6d  be..connection_m
-000008f0: 656d 656e 746f 7394 5d94 2868 4429 8194  ementos.].(hD)..
-00000900: 7d94 2868 474b 0268 485d 9468 4a68 4b75  }.(hGK.hH].hJhKu
-00000910: 6268 4429 8194 7d94 2868 474b 0168 485d  bhD)..}.(hGK.hH]
-00000920: 9468 4a68 5075 6268 4429 8194 7d94 2868  .hJhPubhD)..}.(h
-00000930: 474b 0468 485d 9468 4a68 6075 6268 4429  GK.hH].hJh`ubhD)
-00000940: 8194 7d94 2868 474b 0268 485d 9468 4a68  ..}.(hGK.hH].hJh
-00000950: 7675 6268 4429 8194 7d94 2868 474b 0368  vubhD)..}.(hGK.h
-00000960: 485d 9468 4a68 8975 6268 4429 8194 7d94  H].hJh.ubhD)..}.
-00000970: 2868 474b 0168 485d 9468 4a68 9475 6268  (hGK.hH].hJh.ubh
-00000980: 4429 8194 7d94 2868 474b 0468 485d 9468  D)..}.(hGK.hH].h
-00000990: 4a68 a975 6268 4429 8194 7d94 2868 474b  Jh.ubhD)..}.(hGK
-000009a0: 0368 485d 9468 4a68 b475 6268 4429 8194  .hH].hJh.ubhD)..
-000009b0: 7d94 2868 474b 0968 485d 9468 4a68 ca75  }.(hGK.hH].hJh.u
-000009c0: 6268 4429 8194 7d94 2868 474b 0268 485d  bhD)..}.(hGK.hH]
-000009d0: 9468 4a68 cf75 6268 4429 8194 7d94 2868  .hJh.ubhD)..}.(h
-000009e0: 474b 0268 485d 9468 1129 8194 7d94 2868  GK.hH].h.)..}.(h
-000009f0: 144a ceff ffff 6815 4a9c ffff ff75 6261  .J....h.J....uba
-00000a00: 684a 68df 7562 6844 2981 947d 9428 6847  hJh.ubhD)..}.(hG
-00000a10: 4b03 6848 5d94 6811 2981 947d 9428 6814  K.hH].h.)..}.(h.
-00000a20: 4b64 6815 4b64 7562 6168 4a68 e675 6268  Kdh.KdubahJh.ubh
-00000a30: 4429 8194 7d94 2868 474b 0468 485d 9468  D)..}.(hGK.hH].h
-00000a40: 1129 8194 7d94 2868 144a 6aff ffff 6815  .)..}.(h.Jj...h.
-00000a50: 4bc8 7562 6168 4a68 f575 6268 4429 8194  K.ubahJh.ubhD)..
-00000a60: 7d94 2868 474b 0168 485d 9468 4a6a 0001  }.(hGK.hH].hJj..
-00000a70: 0000 7562 6575 622e                      ..ubeub.
+000000d0: 947d 9428 8c01 7894 4b64 8c01 7994 4a6a  .}.(..x.Kd..y.Jj
+000000e0: ffff ff75 628c 0372 6f74 944b 0275 6261  ...ub..rot.K.uba
+000000f0: 8c0d 6e6f 6465 5f6d 656d 656e 746f 7394  ..node_mementos.
+00000100: 5d94 2868 0a29 8194 7d94 2868 0d4b 0168  ].(h.)..}.(h.K.h
+00000110: 0e68 1129 8194 7d94 2868 144b 6468 154b  .h.)..}.(h.Kdh.K
+00000120: 9675 6268 164b 0175 6268 0a29 8194 7d94  .ubh.K.ubh.)..}.
+00000130: 2868 0d4b 0268 0e68 1129 8194 7d94 2868  (h.K.h.h.)..}.(h
+00000140: 148c 156e 756d 7079 2e63 6f72 652e 6d75  ...numpy.core.mu
+00000150: 6c74 6961 7272 6179 948c 0673 6361 6c61  ltiarray...scala
+00000160: 7294 9394 8c05 6e75 6d70 7994 8c05 6474  r.....numpy...dt
+00000170: 7970 6594 9394 8c02 6938 9489 8887 9452  ype.....i8.....R
+00000180: 9428 4b03 8c01 3c94 4e4e 4e4a ffff ffff  .(K...<.NNNJ....
+00000190: 4aff ffff ff4b 0074 9462 4308 6400 0000  J....K.t.bC.d...
+000001a0: 0000 0000 9486 9452 9468 1568 2368 2943  .......R.h.h#h)C
+000001b0: 08ce ffff ffff ffff ff94 8694 5294 7562  ............R.ub
+000001c0: 6816 4b01 7562 658c 1065 6c65 6d65 6e74  h.K.ube..element
+000001d0: 5f6d 656d 656e 746f 7394 5d94 288c 1f73  _mementos.].(..s
+000001e0: 6363 6972 6375 6974 6275 696c 6465 722e  ccircuitbuilder.
+000001f0: 6272 616e 6368 5f65 6c65 6d65 6e74 948c  branch_element..
+00000200: 1c42 7261 6e63 6845 6c65 6d65 6e74 2e45  .BranchElement.E
+00000210: 6c65 6d65 6e74 4d6f 6d65 6e74 6f94 9394  lementMomento...
+00000220: 2981 947d 9428 8c05 6e6f 6465 7394 5d94  )..}.(..nodes.].
+00000230: 284b 014b 0265 8c07 6772 6f75 6e64 7394  (K.K.e..grounds.
+00000240: 5d94 8c04 6e61 6d65 948c 0143 9468 0e68  ]...name...C.h.h
+00000250: 1129 8194 7d94 2868 144b c868 154b 3275  .)..}.(h.K.h.K2u
+00000260: 628c 0469 636f 6e94 8c6a 2f6f 7074 2f68  b..icon..j/opt/h
+00000270: 6f6d 6562 7265 772f 4361 736b 726f 6f6d  omebrew/Caskroom
+00000280: 2f6d 696e 6963 6f6e 6461 2f62 6173 652f  /miniconda/base/
+00000290: 6c69 622f 7079 7468 6f6e 332e 3130 2f73  lib/python3.10/s
+000002a0: 6974 652d 7061 636b 6167 6573 2f73 6363  ite-packages/scc
+000002b0: 6972 6375 6974 6275 696c 6465 722f 656c  ircuitbuilder/el
+000002c0: 656d 656e 7473 2f63 6170 6163 6974 6f72  ements/capacitor
+000002d0: 2e73 7667 948c 0a70 726f 7065 7274 6965  .svg...propertie
+000002e0: 7394 7d94 683e 683e 738c 0a63 6f6e 6e5f  s.}.h>h>s..conn_
+000002f0: 6d65 6d6f 7394 5d94 288c 1b73 6363 6972  memos.].(..sccir
+00000300: 6375 6974 6275 696c 6465 722e 636f 6e6e  cuitbuilder.conn
+00000310: 6563 7469 6f6e 948c 1c43 6f6e 6e65 6374  ection...Connect
+00000320: 696f 6e2e 436f 6e6e 6563 7469 6f6e 4d6f  ion.ConnectionMo
+00000330: 6d65 6e74 6f94 9394 2981 947d 9428 8c04  mento...)..}.(..
+00000340: 6465 7374 944b 018c 0761 6e63 686f 7273  dest.K...anchors
+00000350: 945d 948c 0164 9468 1129 8194 7d94 2868  .]...d.h.)..}.(h
+00000360: 1468 2368 2943 0800 0000 0000 0000 0094  .h#h)C..........
+00000370: 8694 5294 6815 6823 6829 4308 0100 0000  ..R.h.h#h)C.....
+00000380: 0000 0000 9486 9452 9475 6275 6268 4929  .......R.ububhI)
+00000390: 8194 7d94 2868 4c4b 0268 4d5d 9468 4f68  ..}.(hLK.hM].hOh
+000003a0: 1129 8194 7d94 2868 1468 2368 2943 0800  .)..}.(h.h#h)C..
+000003b0: 0000 0000 0000 0094 8694 5294 6815 6823  ..........R.h.h#
+000003c0: 6829 4308 ffff ffff ffff ffff 9486 9452  h)C............R
+000003d0: 9475 6275 6265 6816 4b01 7562 6836 2981  .ububeh.K.ubh6).
+000003e0: 947d 9428 6839 5d94 4b02 6168 3b5d 944b  .}.(h9].K.ah;].K
+000003f0: 0761 683d 683e 680e 6811 2981 947d 9428  .ah=h>h.h.)..}.(
+00000400: 6814 4b64 6815 4a9c ffff ff75 6268 418c  h.Kdh.J....ubhA.
+00000410: 6a2f 6f70 742f 686f 6d65 6272 6577 2f43  j/opt/homebrew/C
+00000420: 6173 6b72 6f6f 6d2f 6d69 6e69 636f 6e64  askroom/minicond
+00000430: 612f 6261 7365 2f6c 6962 2f70 7974 686f  a/base/lib/pytho
+00000440: 6e33 2e31 302f 7369 7465 2d70 6163 6b61  n3.10/site-packa
+00000450: 6765 732f 7363 6369 7263 7569 7462 7569  ges/sccircuitbui
+00000460: 6c64 6572 2f65 6c65 6d65 6e74 732f 6361  lder/elements/ca
+00000470: 7061 6369 746f 722e 7376 6794 6843 7d94  pacitor.svg.hC}.
+00000480: 683e 8c02 4367 9473 6845 5d94 2868 4929  h>..Cg.shE].(hI)
+00000490: 8194 7d94 2868 4c4b 0268 4d5d 9468 4f68  ..}.(hLK.hM].hOh
+000004a0: 1129 8194 7d94 2868 1468 2368 2943 0800  .)..}.(h.h#h)C..
+000004b0: 0000 0000 0000 0094 8694 5294 6815 6823  ..........R.h.h#
+000004c0: 6829 4308 0100 0000 0000 0000 9486 9452  h)C............R
+000004d0: 9475 6275 6268 4929 8194 7d94 2868 4c4b  .ububhI)..}.(hLK
+000004e0: 0768 4d5d 9468 4f68 1129 8194 7d94 2868  .hM].hOh.)..}.(h
+000004f0: 1468 2368 2943 0800 0000 0000 0000 0094  .h#h)C..........
+00000500: 8694 5294 6815 6823 6829 4308 ffff ffff  ..R.h.h#h)C.....
+00000510: ffff ffff 9486 9452 9475 6275 6265 6816  .......R.ububeh.
+00000520: 4b01 7562 6836 2981 947d 9428 6839 5d94  K.ubh6)..}.(h9].
+00000530: 284b 014b 0265 683b 5d94 683d 8c02 4a4a  (K.K.eh;].h=..JJ
+00000540: 9468 0e68 1129 8194 7d94 2868 144a 6aff  .h.h.)..}.(h.Jj.
+00000550: ffff 6815 4b32 7562 6841 8c63 2f6f 7074  ..h.K2ubhA.c/opt
+00000560: 2f68 6f6d 6562 7265 772f 4361 736b 726f  /homebrew/Caskro
+00000570: 6f6d 2f6d 696e 6963 6f6e 6461 2f62 6173  om/miniconda/bas
+00000580: 652f 6c69 622f 7079 7468 6f6e 332e 3130  e/lib/python3.10
+00000590: 2f73 6974 652d 7061 636b 6167 6573 2f73  /site-packages/s
+000005a0: 6363 6972 6375 6974 6275 696c 6465 722f  ccircuitbuilder/
+000005b0: 656c 656d 656e 7473 2f4a 4a2e 7376 6794  elements/JJ.svg.
+000005c0: 6843 7d94 288c 0245 4394 8c03 4543 3194  hC}.(..EC...EC1.
+000005d0: 8c02 454a 948c 0345 4a31 9475 6845 5d94  ..EJ...EJ1.uhE].
+000005e0: 2868 4929 8194 7d94 2868 4c4b 0168 4d5d  (hI)..}.(hLK.hM]
+000005f0: 9468 4f68 1129 8194 7d94 2868 1468 2368  .hOh.)..}.(h.h#h
+00000600: 2943 0800 0000 0000 0000 0094 8694 5294  )C............R.
+00000610: 6815 6823 6829 4308 0100 0000 0000 0000  h.h#h)C.........
+00000620: 9486 9452 9475 6275 6268 4929 8194 7d94  ...R.ububhI)..}.
+00000630: 2868 4c4b 0268 4d5d 9468 4f68 1129 8194  (hLK.hM].hOh.)..
+00000640: 7d94 2868 1468 2368 2943 0800 0000 0000  }.(h.h#h)C......
+00000650: 0000 0094 8694 5294 6815 6823 6829 4308  ......R.h.h#h)C.
+00000660: ffff ffff ffff ffff 9486 9452 9475 6275  ...........R.ubu
+00000670: 6265 6816 4b01 7562 6836 2981 947d 9428  beh.K.ubh6)..}.(
+00000680: 6839 5d94 284b 014b 0265 683b 5d94 683d  h9].(K.K.eh;].h=
+00000690: 6887 680e 6811 2981 947d 9428 6814 4b00  h.h.h.)..}.(h.K.
+000006a0: 6815 4b32 7562 6841 8c63 2f6f 7074 2f68  h.K2ubhA.c/opt/h
+000006b0: 6f6d 6562 7265 772f 4361 736b 726f 6f6d  omebrew/Caskroom
+000006c0: 2f6d 696e 6963 6f6e 6461 2f62 6173 652f  /miniconda/base/
+000006d0: 6c69 622f 7079 7468 6f6e 332e 3130 2f73  lib/python3.10/s
+000006e0: 6974 652d 7061 636b 6167 6573 2f73 6363  ite-packages/scc
+000006f0: 6972 6375 6974 6275 696c 6465 722f 656c  ircuitbuilder/el
+00000700: 656d 656e 7473 2f4a 4a2e 7376 6794 6843  ements/JJ.svg.hC
+00000710: 7d94 2868 8c8c 0345 4332 9468 8e8c 0345  }.(h...EC2.h...E
+00000720: 4a32 9475 6845 5d94 2868 4929 8194 7d94  J2.uhE].(hI)..}.
+00000730: 2868 4c4b 0168 4d5d 9468 4f68 1129 8194  (hLK.hM].hOh.)..
+00000740: 7d94 2868 1468 2368 2943 0800 0000 0000  }.(h.h#h)C......
+00000750: 0000 0094 8694 5294 6815 6823 6829 4308  ......R.h.h#h)C.
+00000760: 0100 0000 0000 0000 9486 9452 9475 6275  ...........R.ubu
+00000770: 6268 4929 8194 7d94 2868 4c4b 0268 4d5d  bhI)..}.(hLK.hM]
+00000780: 9468 4f68 1129 8194 7d94 2868 1468 2368  .hOh.)..}.(h.h#h
+00000790: 2943 0800 0000 0000 0000 0094 8694 5294  )C............R.
+000007a0: 6815 6823 6829 4308 ffff ffff ffff ffff  h.h#h)C.........
+000007b0: 9486 9452 9475 6275 6265 6816 4b01 7562  ...R.ububeh.K.ub
+000007c0: 658c 1363 6f6e 6e65 6374 696f 6e5f 6d65  e..connection_me
+000007d0: 6d65 6e74 6f73 945d 9428 6849 2981 947d  mentos.].(hI)..}
+000007e0: 9428 684c 4b01 684d 5d94 684f 6850 7562  .(hLK.hM].hOhPub
+000007f0: 6849 2981 947d 9428 684c 4b02 684d 5d94  hI)..}.(hLK.hM].
+00000800: 684f 685b 7562 6849 2981 947d 9428 684c  hOh[ubhI)..}.(hL
+00000810: 4b02 684d 5d94 684f 6870 7562 6849 2981  K.hM].hOhpubhI).
+00000820: 947d 9428 684c 4b07 684d 5d94 684f 687b  .}.(hLK.hM].hOh{
+00000830: 7562 6849 2981 947d 9428 684c 4b01 684d  ubhI)..}.(hLK.hM
+00000840: 5d94 684f 6894 7562 6849 2981 947d 9428  ].hOh.ubhI)..}.(
+00000850: 684c 4b02 684d 5d94 684f 689f 7562 6849  hLK.hM].hOh.ubhI
+00000860: 2981 947d 9428 684c 4b01 684d 5d94 684f  )..}.(hLK.hM].hO
+00000870: 68b5 7562 6849 2981 947d 9428 684c 4b02  h.ubhI)..}.(hLK.
+00000880: 684d 5d94 684f 68c0 7562 6575 622e       hM].hOh.ubeub.
```

### Comparing `sccircuitbuilder-0.0.2/sccircuitbuilder/elements/Inductor.svg` & `sccircuitbuilder-0.0.3/sccircuitbuilder/elements/Inductor.svg`

 * *Files identical despite different names*

### Comparing `sccircuitbuilder-0.0.2/sccircuitbuilder/elements/JJ.svg` & `sccircuitbuilder-0.0.3/sccircuitbuilder/elements/JJ.svg`

 * *Files identical despite different names*

### Comparing `sccircuitbuilder-0.0.2/sccircuitbuilder/elements/capacitor.svg` & `sccircuitbuilder-0.0.3/sccircuitbuilder/elements/capacitor.svg`

 * *Files identical despite different names*

### Comparing `sccircuitbuilder-0.0.2/sccircuitbuilder/elements/ground.svg` & `sccircuitbuilder-0.0.3/sccircuitbuilder/elements/ground.svg`

 * *Files identical despite different names*

### Comparing `sccircuitbuilder-0.0.2/sccircuitbuilder/icons/redo.png` & `sccircuitbuilder-0.0.3/sccircuitbuilder/icons/redo.png`

 * *Files identical despite different names*

### Comparing `sccircuitbuilder-0.0.2/sccircuitbuilder/icons/rotate.png` & `sccircuitbuilder-0.0.3/sccircuitbuilder/icons/rotate.png`

 * *Files identical despite different names*

### Comparing `sccircuitbuilder-0.0.2/sccircuitbuilder/icons/undo.png` & `sccircuitbuilder-0.0.3/sccircuitbuilder/icons/undo.png`

 * *Files identical despite different names*

### Comparing `sccircuitbuilder-0.0.2/LICENSE` & `sccircuitbuilder-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sccircuitbuilder-0.0.2/README.md` & `sccircuitbuilder-0.0.3/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 # Superconducting Circuit Builder
-This is a GUI for designing superconducting circuits intended to accompany the Python package scQubits.
+This is a GUI for designing superconducting circuits in the lumped-element limit intended to accompany the Python package scQubits.
 
 ## Installation
-* git clone https://github.com/benmcdonough20/CircuitBuilder.git
-* pip install pyside2
+`pip install sccircuitbuilder`
 
 ## Usage
 Run `import sccircuitbuilder as sc`, then `sc.GUI()`. The elements used to build a circuit are
 1) Capacitor
 2) Inductor
 3) Josephson Junction
 
 Drag the icons from the toolbox onto the canvas to place down an element. Drag nodes together to connect them. Left-click on wires to add anchor points and drag 
-the anchor points to guide the wires.
+the anchor points to guide the wires. Export the circuit to scqubits to diagonalize and simulate the circuit!
 
 ### Keyboard
 * `Shift + Right Click` - add to selection
 * `Shift + Right Drag` - add box to selection
 * `Enter` on property entry box - change property
 
 ### Mouse
@@ -34,11 +33,16 @@
 * Delete elements
 * Wire anchor points
 * Undo / Redo
 * Save / Open
 * Export to scQubits circuit format
 * Pre-made circuit library
 
+## Future plans
+* Offset charge / external flux
+* Further integration with scqubits
+* Accompanying tutorials
+
 ## Known issues
-There are still many bugs!
 * Right click has no activation distance, so using a mouse will result in some dropped right clicks
 * Sometime import/undo/redo (the memento-based functionalities) crash, but usually they seem to work 
+* File save is not very inteligent and adds `.circuit` to the end of the filename regardless of whether it is already there
```

### Comparing `sccircuitbuilder-0.0.2/pyproject.toml` & `sccircuitbuilder-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "sccircuitbuilder"
-version = "0.0.2"
+version = "0.0.3"
 dependencies = ["numpy", "pyside6"]
 keywords = [
   "quantum",
   "quantum computing",
   "superconducting circuits",
   "circuit QED",
   "cQED",
```

### Comparing `sccircuitbuilder-0.0.2/PKG-INFO` & `sccircuitbuilder-0.0.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sccircuitbuilder
-Version: 0.0.2
+Version: 0.0.3
 Summary: A graphical user interface to create superconducting circuits intended to accompany scQubits
 Project-URL: Homepage, https://github.com/benmcdonough20/SuperconductingCircuitBuilder
 Project-URL: Tracker, https://github.com/benmcdonough20/SuperconductingCircuitBuilder/issues
 Author-email: Ben McDonough <ben.mcdonough@yale.edu>
 License-File: LICENSE
 Keywords: cQED,circuit QED,quantum,quantum computing,superconducting circuits
 Classifier: License :: OSI Approved :: MIT License
@@ -12,28 +12,27 @@
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: numpy
 Requires-Dist: pyside6
 Description-Content-Type: text/markdown
 
 # Superconducting Circuit Builder
-This is a GUI for designing superconducting circuits intended to accompany the Python package scQubits.
+This is a GUI for designing superconducting circuits in the lumped-element limit intended to accompany the Python package scQubits.
 
 ## Installation
-* git clone https://github.com/benmcdonough20/CircuitBuilder.git
-* pip install pyside2
+`pip install sccircuitbuilder`
 
 ## Usage
 Run `import sccircuitbuilder as sc`, then `sc.GUI()`. The elements used to build a circuit are
 1) Capacitor
 2) Inductor
 3) Josephson Junction
 
 Drag the icons from the toolbox onto the canvas to place down an element. Drag nodes together to connect them. Left-click on wires to add anchor points and drag 
-the anchor points to guide the wires.
+the anchor points to guide the wires. Export the circuit to scqubits to diagonalize and simulate the circuit!
 
 ### Keyboard
 * `Shift + Right Click` - add to selection
 * `Shift + Right Drag` - add box to selection
 * `Enter` on property entry box - change property
 
 ### Mouse
@@ -51,11 +50,16 @@
 * Delete elements
 * Wire anchor points
 * Undo / Redo
 * Save / Open
 * Export to scQubits circuit format
 * Pre-made circuit library
 
+## Future plans
+* Offset charge / external flux
+* Further integration with scqubits
+* Accompanying tutorials
+
 ## Known issues
-There are still many bugs!
 * Right click has no activation distance, so using a mouse will result in some dropped right clicks
 * Sometime import/undo/redo (the memento-based functionalities) crash, but usually they seem to work 
+* File save is not very inteligent and adds `.circuit` to the end of the filename regardless of whether it is already there
```

