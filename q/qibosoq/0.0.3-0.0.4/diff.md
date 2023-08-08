# Comparing `tmp/qibosoq-0.0.3.tar.gz` & `tmp/qibosoq-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qibosoq-0.0.3.tar", max compression
+gzip compressed data, was "qibosoq-0.0.4.tar", max compression
```

## Comparing `qibosoq-0.0.3.tar` & `qibosoq-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    11357 2023-07-08 08:29:21.041516 qibosoq-0.0.3/LICENSE
--rw-r--r--   0        0        0     2577 2023-07-08 08:29:21.041516 qibosoq-0.0.3/README.md
--rw-r--r--   0        0        0     1610 2023-07-08 08:29:21.045516 qibosoq-0.0.3/pyproject.toml
--rw-r--r--   0        0        0       94 2023-07-08 08:29:21.045516 qibosoq-0.0.3/src/qibosoq/__init__.py
--rw-r--r--   0        0        0      428 2023-07-08 08:29:21.045516 qibosoq-0.0.3/src/qibosoq/__main__.py
--rw-r--r--   0        0        0     2086 2023-07-08 08:29:21.045516 qibosoq-0.0.3/src/qibosoq/client.py
--rw-r--r--   0        0        0       22 2023-07-08 08:29:21.045516 qibosoq-0.0.3/src/qibosoq/components/__init__.py
--rw-r--r--   0        0        0     2176 2023-07-08 08:29:21.045516 qibosoq-0.0.3/src/qibosoq/components/base.py
--rw-r--r--   0        0        0     1670 2023-07-08 08:29:21.045516 qibosoq-0.0.3/src/qibosoq/components/pulses.py
--rw-r--r--   0        0        0     1021 2023-07-08 08:29:21.045516 qibosoq-0.0.3/src/qibosoq/configuration.py
--rw-r--r--   0        0        0     1063 2023-07-08 08:29:21.045516 qibosoq-0.0.3/src/qibosoq/log.py
--rw-r--r--   0        0        0       23 2023-07-08 08:29:21.045516 qibosoq-0.0.3/src/qibosoq/programs/__init__.py
--rw-r--r--   0        0        0    13923 2023-07-08 08:29:21.045516 qibosoq-0.0.3/src/qibosoq/programs/base.py
--rw-r--r--   0        0        0     2964 2023-07-08 08:29:21.045516 qibosoq-0.0.3/src/qibosoq/programs/flux.py
--rw-r--r--   0        0        0      917 2023-07-08 08:29:21.045516 qibosoq-0.0.3/src/qibosoq/programs/pulse_sequence.py
--rw-r--r--   0        0        0     4910 2023-07-08 08:29:21.045516 qibosoq-0.0.3/src/qibosoq/programs/sweepers.py
--rw-r--r--   0        0        0     4737 2023-07-08 08:29:21.045516 qibosoq-0.0.3/src/qibosoq/rfsoc_server.py
--rw-r--r--   0        0        0     3395 1970-01-01 00:00:00.000000 qibosoq-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-08-08 06:17:32.882951 qibosoq-0.0.4/LICENSE
+-rw-r--r--   0        0        0     2400 2023-08-08 06:17:32.882951 qibosoq-0.0.4/README.md
+-rw-r--r--   0        0        0     1681 2023-08-08 06:17:32.882951 qibosoq-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0       94 2023-08-08 06:17:32.886951 qibosoq-0.0.4/src/qibosoq/__init__.py
+-rw-r--r--   0        0        0      422 2023-08-08 06:17:32.886951 qibosoq-0.0.4/src/qibosoq/__main__.py
+-rw-r--r--   0        0        0     2020 2023-08-08 06:17:32.886951 qibosoq-0.0.4/src/qibosoq/client.py
+-rw-r--r--   0        0        0       22 2023-08-08 06:17:32.886951 qibosoq-0.0.4/src/qibosoq/components/__init__.py
+-rw-r--r--   0        0        0     3017 2023-08-08 06:17:32.886951 qibosoq-0.0.4/src/qibosoq/components/base.py
+-rw-r--r--   0        0        0     2186 2023-08-08 06:17:32.886951 qibosoq-0.0.4/src/qibosoq/components/pulses.py
+-rw-r--r--   0        0        0      977 2023-08-08 06:17:32.886951 qibosoq-0.0.4/src/qibosoq/configuration.py
+-rw-r--r--   0        0        0     1235 2023-08-08 06:17:32.886951 qibosoq-0.0.4/src/qibosoq/log.py
+-rw-r--r--   0        0        0       23 2023-08-08 06:17:32.886951 qibosoq-0.0.4/src/qibosoq/programs/__init__.py
+-rw-r--r--   0        0        0    12230 2023-08-08 06:17:32.886951 qibosoq-0.0.4/src/qibosoq/programs/base.py
+-rw-r--r--   0        0        0     6536 2023-08-08 06:17:32.886951 qibosoq-0.0.4/src/qibosoq/programs/flux.py
+-rw-r--r--   0        0        0      632 2023-08-08 06:17:32.886951 qibosoq-0.0.4/src/qibosoq/programs/pulse_sequence.py
+-rw-r--r--   0        0        0     5982 2023-08-08 06:17:32.886951 qibosoq-0.0.4/src/qibosoq/programs/sweepers.py
+-rw-r--r--   0        0        0     5332 2023-08-08 06:17:32.886951 qibosoq-0.0.4/src/qibosoq/server.py
+-rw-r--r--   0        0        0     3218 1970-01-01 00:00:00.000000 qibosoq-0.0.4/PKG-INFO
```

### Comparing `qibosoq-0.0.3/LICENSE` & `qibosoq-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `qibosoq-0.0.3/README.md` & `qibosoq-0.0.4/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -4,33 +4,22 @@
 [![codecov](https://codecov.io/gh/qiboteam/qibosoq/branch/main/graph/badge.svg?token=1EKZKVEVX0)](https://codecov.io/gh/qiboteam/qibosoq)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8083285.svg)](https://doi.org/10.5281/zenodo.8083285)
 
 Repository for developing server side of RFSoC fpga boards
 Qibosoq is a server for integrating [Qick](https://github.com/openquantumhardware/qick) in the [Qibolab](https://github.com/qiboteam/qibolab) ecosystem
 for executing arbitrary pulses sequences on QPUs.
 
-The complete documentation for can be found at [qibo.science/qibosoq/stable](https://qibo.science/qibosoq/stable/)
+The complete documentation for can be found at:
+
+* [qibo.science/qibosoq/stable](https://qibo.science/qibosoq/stable/)
+* [qibo.science/qibosoq/latest](https://qibo.science/qibosoq/latest/)
 
-## Installation
-The package can be installed by source:
 
-```sh
-git clone https://github.com/qiboteam/qibosoq.git
-cd qibosoq
-pip install .
-```
-### Developer instructions
-For development make sure to install the package using [`poetry`](https://python-poetry.org/) and to install the pre-commit hooks:
-
-```sh
-git clone https://github.com/qiboteam/qibosoq.git
-cd qibosoq
-poetry install
-pre-commit install
-```
+## Installation
+Please refer to the [documentation](https://qibo.science/qibosoq/stable/getting-started/installation.html) for installation instructions.
 
 ## Configuration parameters
 
 In `configuration.py` some default qibosoq parameters are hardcoded. They can be changed using environment variables ([see documentation](https://qibo.science/qibosoq/stable/getting-started/usage.html)).
 
 * IP of the server
 * Port of the server
```

#### html2text {}

```diff
@@ -2,31 +2,29 @@
 badge.svg) [![codecov](https://codecov.io/gh/qiboteam/qibosoq/branch/main/
 graph/badge.svg?token=1EKZKVEVX0)](https://codecov.io/gh/qiboteam/qibosoq) [!
 [DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8083285.svg)](https://
 doi.org/10.5281/zenodo.8083285) Repository for developing server side of RFSoC
 fpga boards Qibosoq is a server for integrating [Qick](https://github.com/
 openquantumhardware/qick) in the [Qibolab](https://github.com/qiboteam/qibolab)
 ecosystem for executing arbitrary pulses sequences on QPUs. The complete
-documentation for can be found at [qibo.science/qibosoq/stable](https://
-qibo.science/qibosoq/stable/) ## Installation The package can be installed by
-source: ```sh git clone https://github.com/qiboteam/qibosoq.git cd qibosoq pip
-install . ``` ### Developer instructions For development make sure to install
-the package using [`poetry`](https://python-poetry.org/) and to install the
-pre-commit hooks: ```sh git clone https://github.com/qiboteam/qibosoq.git cd
-qibosoq poetry install pre-commit install ``` ## Configuration parameters In
-`configuration.py` some default qibosoq parameters are hardcoded. They can be
-changed using environment variables ([see documentation](https://qibo.science/
-qibosoq/stable/getting-started/usage.html)). * IP of the server * Port of the
-server * Paths of log files * Name of python loggers * Path of bitstream * Type
-of readout (multiplexed or not, depending on the loaded bitstream) ## Run the
-server The simplest way of executing the server is: ``` sudo -E python -
-m qibosoq ``` and the server can be closed with `Ctrl-C`.\ Note that with this
-command the script will close as soon as the terminal where it's running it's
-closed. To run the server in detached mode you can use: ``` nohup sudo -
-E python -m qibosoq & ``` And the server can be closed with `sudo kill ` (PID
-will be saved in log). ### TII boards With TII boards the server can also be
-executed using the alias `server-run-bkg`. Also, two additional command are
+documentation for can be found at: * [qibo.science/qibosoq/stable](https://
+qibo.science/qibosoq/stable/) * [qibo.science/qibosoq/latest](https://
+qibo.science/qibosoq/latest/) ## Installation Please refer to the
+[documentation](https://qibo.science/qibosoq/stable/getting-started/
+installation.html) for installation instructions. ## Configuration parameters
+In `configuration.py` some default qibosoq parameters are hardcoded. They can
+be changed using environment variables ([see documentation](https://
+qibo.science/qibosoq/stable/getting-started/usage.html)). * IP of the server *
+Port of the server * Paths of log files * Name of python loggers * Path of
+bitstream * Type of readout (multiplexed or not, depending on the loaded
+bitstream) ## Run the server The simplest way of executing the server is: ```
+sudo -E python -m qibosoq ``` and the server can be closed with `Ctrl-C`.\ Note
+that with this command the script will close as soon as the terminal where it's
+running it's closed. To run the server in detached mode you can use: ``` nohup
+sudo -E python -m qibosoq & ``` And the server can be closed with `sudo kill `
+(PID will be saved in log). ### TII boards With TII boards the server can also
+be executed using the alias `server-run-bkg`. Also, two additional command are
 added in `.bashrc`: `serverinfo` and `serverclose`. `serverinfo` will print the
 PID if the server is running, otherwise will print "No running server".
 `serverclose` will close the server, if it is running. All these commands
 require sudo privileges. ## Contributing Contributions, issues and feature
 requests are welcome! Feel free to check [GitHub_issues]
```

### Comparing `qibosoq-0.0.3/pyproject.toml` & `qibosoq-0.0.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qibosoq"
-version = "0.0.3"
+version = "0.0.4"
 description = "QIBO Server On Qick (qibosoq) is the server component of qibolab to be run on RFSoC boards"
 authors = [
   "Rodolfo Carobene <rodolfo.carobene@gmail.com>",
   "Javier Serrano <javier.serrano@tii.ae>",
 ]
 license = "Apache License 2.0"
 readme = "README.md"
@@ -60,7 +60,11 @@
 docs = "make -C doc html"
 docs-clean = "make -C doc clean"
 test-docs = "make -C doc doctest"
 
 [tool.pytest.ini_options]
 testpaths = ['tests/']
 addopts = ['--cov=qibosoq', '--cov-report=xml', '--cov-report=html']
+
+[[tool.mypy.overrides]]
+module="qick.*"
+ignore_missing_imports = true
```

### Comparing `qibosoq-0.0.3/src/qibosoq/client.py` & `qibosoq-0.0.4/src/qibosoq/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,30 +28,29 @@
         received = bytearray()
         while True:
             tmp = sock.recv(4096)
             if not tmp:
                 break
             received.extend(tmp)
         results = json.loads(received.decode("utf-8"))
-        if isinstance(results, str) and "Error" in results:
+        if isinstance(results, str):
             raise QibosoqError(results)
         return results["i"], results["q"]
 
 
 def convert_commands(obj_dictionary: dict) -> dict:
     """Convert the contents of a commands dictionary from object to dict."""
     dict_dictionary = {
         "operation_code": obj_dictionary["operation_code"],
         "cfg": asdict(obj_dictionary["cfg"]),
         "sequence": [asdict(pulse) for pulse in obj_dictionary["sequence"]],
         "qubits": [asdict(qubit) for qubit in obj_dictionary["qubits"]],
-        "average": obj_dictionary["average"],
     }
     if "sweepers" in obj_dictionary:
-        dict_dictionary["sweepers"] = [asdict(sweep) for sweep in obj_dictionary["sweepers"]]
+        dict_dictionary["sweepers"] = [sweep.serialized for sweep in obj_dictionary["sweepers"]]
     return dict_dictionary
 
 
 def execute(obj_dictionary: dict, host: str, port: int) -> Tuple[list, list]:
     """Convert a dictionary of objects and run experiment."""
     server_commands = convert_commands(obj_dictionary)
     return connect(server_commands, host, port)
```

### Comparing `qibosoq-0.0.3/src/qibosoq/components/base.py` & `qibosoq-0.0.4/src/qibosoq/components/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,48 @@
 """Various helper objects."""
 
 from dataclasses import dataclass
 from enum import Enum, IntEnum, auto
-from typing import Iterable, List, Union, overload
+from typing import Iterable, List, Optional, overload
+
+import numpy as np
+import numpy.typing as npt
 
 
 @dataclass
 class Config:
     """General RFSoC Configuration."""
 
     repetition_duration: int = 100
     """Time to wait between shots (us)."""
     adc_trig_offset: int = 200
     """Time to wait between readout pulse and acquisition (ADC clock ticks)."""
     reps: int = 1000
     """Number of shots."""
     soft_avgs: int = 1
     """Number of software averages."""
+    average: bool = True
+    """Returns integrated results if true."""
 
 
 class OperationCode(IntEnum):
     """Available operations."""
 
     EXECUTE_PULSE_SEQUENCE = auto()
     EXECUTE_PULSE_SEQUENCE_RAW = auto()
     EXECUTE_SWEEPS = auto()
 
 
 @dataclass
 class Qubit:
     """Qubit object, storing flux information."""
 
-    bias: float = 0.0
+    bias: Optional[float] = None
     """Amplitude factor, for sweetspot."""
-    dac: int = None
+    dac: Optional[int] = None
     """DAC responsible for flux control."""
 
 
 class Parameter(str, Enum):
     """Available parameters for sweepers."""
 
     FREQUENCY = "freq"
@@ -45,15 +50,15 @@
     RELATIVE_PHASE = "phase"
     DELAY = "t"
     BIAS = "bias"
     DURATION = "duration"
 
     @overload
     @classmethod
-    def variants(cls, parameters: str) -> "Parameter":
+    def variants(cls, parameters: str) -> "Parameter":  # type: ignore
         """Convert a string to a Parameter."""
 
     @overload
     @classmethod
     def variants(cls, parameters: Iterable[str]) -> Iterable["Parameter"]:
         """Convert a iterable of str to an iterable of Parameters."""
 
@@ -65,17 +70,38 @@
         return type(parameters)(cls[par.upper()] for par in parameters)
 
 
 @dataclass
 class Sweeper:
     """Sweeper object."""
 
-    expts: int = None
+    expts: int
     """Number of points of the sweeper."""
-    parameters: List[Parameter] = None
+    parameters: List[Parameter]
     """List of parameter to update."""
-    starts: List[Union[int, float]] = None
+    indexes: List[int]
+    """Index of the parameter to sweep relative to list of pulses or list of qubits."""
+    starts: npt.NDArray[np.float64]
     """Start value for each parameter to sweep."""
-    stops: List[Union[int, float]] = None
+    stops: npt.NDArray[np.float64]
     """Stop value for each parameter to sweep."""
-    indexes: List[int] = None
-    """Index of the parameter to sweep relative to list of pulses or list of qubits."""
+
+    def __post_init__(self):
+        """Convert starts and stops in np.arrays if needed."""
+        if isinstance(self.starts, list):
+            self.starts = np.array(self.starts, dtype=np.float64)
+        if isinstance(self.stops, list):
+            self.stops = np.array(self.stops, dtype=np.float64)
+
+    @property
+    def serialized(self) -> dict:
+        """Convert a Sweeper object into a dictionary.
+
+        In particular, takes care of the convertion arrays -> lists.
+        """
+        return {
+            "expts": self.expts,
+            "parameters": self.parameters,
+            "indexes": self.indexes,
+            "starts": self.starts.tolist(),
+            "stops": self.stops.tolist(),
+        }
```

### Comparing `qibosoq-0.0.3/src/qibosoq/configuration.py` & `qibosoq-0.0.4/src/qibosoq/configuration.py`

 * *Files 16% similar despite different names*

```diff
@@ -24,9 +24,9 @@
 
 PROGRAM_LOGGER_NAME = from_env("PROGRAM_LOGGER_NAME", "qick_program")
 """Program logger name."""
 
 QICKSOC_LOCATION = from_env("BITSTREAM", "/home/xilinx/jupyter_notebooks/qick_111_rfbv1_mux.bit")
 """Path of the qick bitstream to load."""
 
-IS_MULTIPLEXED = from_env("IS_MULTIPLEXED", "True") == "True"  # TODO this should be written in bitstream
+IS_MULTIPLEXED = from_env("IS_MULTIPLEXED", "True") == "True"
 """Whether the readout is multiplexed or not."""
```

### Comparing `qibosoq-0.0.3/src/qibosoq/log.py` & `qibosoq-0.0.4/src/qibosoq/log.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 """Loggers configuration."""
 
 import logging
 import logging.handlers
 import os
+from pathlib import Path
 from typing import Tuple
 
 import qibosoq.configuration as cfg
 
 
 def configure_logger(name: str, filename: str, backup_count: int):
     """Create and configure logger."""
+    # if the log directory does not exsist, create it
+    dir_path = Path(filename).parent
+    if not dir_path.exists():
+        dir_path.mkdir()
+
     if name is not None:
         new_logger = logging.getLogger(name)
     else:
         new_logger = logging
     new_logger.setLevel(logging.DEBUG)
     formatter = logging.Formatter("%(levelname)s :: %(asctime)s ::  %(message)s", "%Y-%m-%d %H:%M:%S")
```

### Comparing `qibosoq-0.0.3/src/qibosoq/programs/base.py` & `qibosoq-0.0.4/src/qibosoq/programs/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,17 +2,15 @@
 
 import logging
 from abc import ABC, abstractmethod
 from dataclasses import asdict
 from typing import Dict, List, Tuple
 
 import numpy as np
-import numpy.typing as npt
 from qick import QickProgram, QickSoc
-from qick.qick_asm import QickRegister
 
 import qibosoq.configuration as qibosoq_cfg
 from qibosoq.components.base import Config, Qubit
 from qibosoq.components.pulses import Arbitrary, Drag, Gaussian, Pulse, Rectangular
 
 logger = logging.getLogger(qibosoq_cfg.MAIN_LOGGER_NAME)
 
@@ -46,15 +44,15 @@
         self.readouts_per_experiment = len([pulse for pulse in self.sequence if pulse.type == "readout"])
 
         self.relax_delay = self.us2cycles(qpcfg.repetition_duration)
         self.syncdelay = self.us2cycles(0)
         self.wait_initialize = self.us2cycles(2.0)
 
         self.pulses_registered = False
-        self.registered_waveforms = {}
+        self.registered_waveforms: Dict[int, list] = {}
         for pulse in sequence:
             if pulse.dac not in self.registered_waveforms:
                 self.registered_waveforms[pulse.dac] = []
 
         if self.is_mux:
             self.multi_ro_pulses = self.group_mux_ro()
             self.readouts_per_experiment = len(self.multi_ro_pulses)
@@ -191,107 +189,68 @@
             pulse_ch=pulse.dac,
             adcs=adcs,
             adc_trig_offset=self.adc_trig_offset,
             wait=False,
             syncdelay=self.syncdelay,
         )
 
-    def body(self):
-        """Execute sequence of pulses.
-
-        For each pulses calls the add_pulse_to_register function (if not already registered)
-        before firing it. If the pulse is a readout, it does a measurement and does
-        not wait for the end of it. At the end of the sequence wait for meas and clock.
-        """
-        # in the form of {dac_number_0: last_pulse_of_dac_0, ...}
-        last_pulse_registered = {}
-        muxed_pulses_executed = []
-        muxed_ro_executed_indexes = []
-
-        for pulse in self.sequence:
-            # wait the needed wait time so that the start is timed correctly
-            if isinstance(pulse.start_delay, QickRegister):
-                self.sync(pulse.start_delay.page, pulse.start_delay.addr)
-            else:  # assume is number
-                delay_start = self.soc.us2cycles(pulse.start_delay)
-                if delay_start != 0:
-                    self.synci(delay_start)
-
-            if pulse.type == "drive":
-                self.execute_drive_pulse(pulse, last_pulse_registered)
-            elif pulse.type == "readout":
-                self.execute_readout_pulse(pulse, muxed_pulses_executed, muxed_ro_executed_indexes)
-
-        self.wait_all()
-
-    # pylint: disable=unexpected-keyword-arg, arguments-renamed
-    def acquire(
+    def perform_experiment(
         self,
         soc: QickSoc,
-        load_pulses: bool = True,
-        progress: bool = False,
-        debug: bool = False,
         average: bool = False,
-    ) -> Tuple[npt.NDArray[np.float64], npt.NDArray[np.float64]]:
-        """Call the super() acquire function.
+    ) -> Tuple[list, list]:
+        """Call the acquire function, executing the experiment.
+
+        The acquire function is coded in `qick.AveragerProgram` or `qick.NDAveragerProgram`
 
         Args:
-            load_pulse, progress, debug (bool): internal Qick parameters
-            progress (bool): if true shows a progress bar, slows down things
-            debug (bool): if true prints the program actually executed
             average (bool): if true return averaged res, otherwise single shots
         """
         readouts_per_experiment = self.readouts_per_experiment
         # if there are no readouts, temporaray set 1 so that qick can execute properly
         reads_per_rep = 1 if readouts_per_experiment == 0 else readouts_per_experiment
 
-        res = super().acquire(
+        res = self.acquire(  # pylint: disable=E1123
             soc,
             readouts_per_experiment=reads_per_rep,
-            load_pulses=load_pulses,
-            progress=progress,
-            debug=debug,
         )
         # if there are no actual readouts, return empty lists
         if readouts_per_experiment == 0:
             return [], []
         if average:
             # for sweeps res has 3 parameters, the first is not used
-            return res[-2:]
+            return np.array(res[-2]).tolist(), np.array(res[-1]).tolist()
         # super().acquire function fill buffers used in collect_shots
         return self.collect_shots()[-2:]
 
-    def collect_shots(self) -> Tuple[npt.NDArray[np.float64], npt.NDArray[np.float64]]:
+    def collect_shots(self) -> Tuple[list, list]:
         """Read the internal buffers and returns single shots (i,q)."""
         tot_i = []
         tot_q = []
 
         adcs = []  # list of adcs per readouts (not unique values)
         lengths = []  # length of readouts (only one per adcs)
         for pulse in (pulse for pulse in self.sequence if pulse.type == "readout"):
             adc_ch = pulse.adc
             ro_ch = pulse.dac
             if adc_ch not in adcs:
                 lengths.append(self.soc.us2cycles(pulse.duration, gen_ch=ro_ch))
             adcs.append(adc_ch)
 
-        adcs, adc_count = np.unique(adcs, return_counts=True)
+        unique_adcs, adc_count = np.unique(adcs, return_counts=True)
 
-        for idx, adc_ch in enumerate(adcs):
+        for idx, adc_ch in enumerate(unique_adcs):
             count = adc_count[idx]
-            if self.expts:  # self.expts is None if this is not a sweep
-                shape = (count, self.expts, self.reps)
-            else:
-                shape = (count, self.reps)
+            shape = (count, self.expts, self.reps) if self.expts else (count, self.reps)
             i_val = self.di_buf[idx].reshape(shape) / lengths[idx]
             q_val = self.dq_buf[idx].reshape(shape) / lengths[idx]
 
-            tot_i.append(i_val)
-            tot_q.append(q_val)
-        return np.array(tot_i), np.array(tot_q)
+            tot_i.append(i_val.tolist())
+            tot_q.append(q_val.tolist())
+        return tot_i, tot_q
 
     def declare_gen_mux_ro(self):
         """Declare nqz zone for multiplexed readout."""
         adc_ch_added = []
 
         mux_freqs = []
         mux_gains = []
@@ -314,15 +273,15 @@
             nqz=zone,
             mixer_freq=0,
             mux_freqs=mux_freqs,
             mux_gains=mux_gains,
             ro_ch=adc_ch_added[0],
         )
 
-    def add_muxed_readout_to_register(self, ro_pulses: List[Pulse]):
+    def add_muxed_readout_to_register(self, ro_pulses: List[Rectangular]):
         """Register multiplexed pulse before firing it."""
         # readout amplitude gets divided by len(mask), we are here fixing the values
         mask = [0, 1, 2]
 
         pulse = ro_pulses[0]
         gen_ch = pulse.dac
         length = self.soc.us2cycles(pulse.duration, gen_ch=gen_ch)
@@ -334,16 +293,16 @@
 
     def group_mux_ro(self) -> list:
         """Create a list containing readout pulses grouped by start time.
 
         Example of list:
         [[pulse1, pulse2], [pulse3]]
         """
-        mux_list = []
-        len_last_readout = 0
+        mux_list: List[List[Pulse]] = []
+        len_last_readout = 0.0
         for pulse in (pulse for pulse in self.sequence if pulse.type == "readout"):
             if pulse.start_delay <= len_last_readout and len(mux_list) > 0:
                 # add the pulse to the last multiplexed readout
                 mux_list[-1].append(pulse)
             else:
                 # add a new multiplexed readout
                 mux_list.append([pulse])
```

### Comparing `qibosoq-0.0.3/src/qibosoq/programs/pulse_sequence.py` & `qibosoq-0.0.4/src/qibosoq/programs/pulse_sequence.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,15 +14,9 @@
     """Class to execute arbitrary PulseSequences."""
 
     def initialize(self):
         """Declre nyquist zones for all the DACs and all the readout frequencies.
 
         Function called by AveragerProgram.__init__.
         """
-        self.declare_nqz_zones([pulse for pulse in self.sequence if pulse.type == "drive"])
-        self.declare_nqz_flux()
-        if self.is_mux:
-            self.declare_gen_mux_ro()
-        else:
-            self.declare_nqz_zones([pulse for pulse in self.sequence if pulse.type == "readout"])
-        self.declare_readout_freq()
+        self.declare_zones_and_ro(self.sequence)
         self.sync_all(self.wait_initialize)
```

### Comparing `qibosoq-0.0.3/src/qibosoq/programs/sweepers.py` & `qibosoq-0.0.4/src/qibosoq/programs/sweepers.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """Program used by qibosoq to execute sweeps."""
 
 import logging
-from typing import Iterable, List, Tuple, Union
+from typing import Iterable, List, Union
 
-import numpy as np
 from qick import NDAveragerProgram, QickSoc
 from qick.averager_program import QickSweep, merge_sweeps
 
 import qibosoq.configuration as qibosoq_cfg
 from qibosoq.components.base import Config, Parameter, Qubit, Sweeper
 from qibosoq.components.pulses import Pulse
 from qibosoq.programs.flux import FluxProgram
@@ -18,48 +17,64 @@
 def reversed_sweepers(sweepers: Union[Sweeper, Iterable[Sweeper]]) -> List[Sweeper]:
     """Ensure that sweepers is a list and reverse it.
 
     This is because sweepers are handled by Qick in the opposite order.
     """
     if isinstance(sweepers, Sweeper):
         return [sweepers]
-    return list(reversed(sweepers))
+    return list(reversed(sweepers))  # type: ignore
 
 
 class ExecuteSweeps(FluxProgram, NDAveragerProgram):
     """Class to execute arbitrary PulseSequences with a single sweep."""
 
-    def __init__(
-        self,
-        soc: QickSoc,
-        qpcfg: Config,
-        sequence: List[Pulse],
-        qubits: List[Qubit],
-        sweepers: Tuple[Sweeper, ...],
-    ):
+    def __init__(self, soc: QickSoc, qpcfg: Config, sequence: List[Pulse], qubits: List[Qubit], *sweepers: Sweeper):
         """Init function, sets sweepers parameters before calling super.__init__."""
         self.sweepers = reversed_sweepers(sweepers)
         super().__init__(soc, qpcfg, sequence, qubits)
 
+    def validate(self, sweeper: Sweeper):
+        """Check if a sweeper is valid.
+
+        In particular, it raises an error if:
+            - sweeper is on bias, but not enough information has been given with the qubit
+            - sweeper is on bias wih flux pulses in the sequence
+            - sweeper is on flux pulses
+            - sweeper is on duration
+            - sweeper has pulse paramaters and bias
+        """
+        for idx, par in enumerate(sweeper.parameters):
+            if par is Parameter.BIAS:
+                if any(pulse.type == "flux" for pulse in self.sequence):
+                    raise NotImplementedError("Sweepers on bias are not compatible with flux pulses.")
+                if any(par is not Parameter.BIAS for par in sweeper.parameters):
+                    raise NotImplementedError("Sweepers on bias cannot be swept at the same time with other sweepers.")
+                qubit = self.qubits[sweeper.indexes[idx]]
+                if qubit.dac is None or qubit.bias is None:
+                    raise ValueError(f"Bias swept qubit had incomplete values: {qubit}")
+            elif par is Parameter.DURATION:
+                raise NotImplementedError("Sweepers on duration are not implemented.")
+            else:
+                if self.sequence[sweeper.indexes[idx]].type == "flux":
+                    raise NotImplementedError("Sweepers on flux pulses are not implemented.")
+
     def add_sweep_info(self, sweeper: Sweeper):
         """Register RfsocSweep objects.
 
         Args:
-            sweeper (RfsocSweep): single qibolab sweeper object to register
+            sweeper: single qibolab sweeper object to register
         """
-        starts = sweeper.starts
-        stops = sweeper.stops
-
+        self.validate(sweeper)
         sweep_list = []
-        sweeper.parameters = [Parameter(par) for par in sweeper.parameters]
-        sweeper.starts = np.array(sweeper.starts)
-        sweeper.stops = np.array(sweeper.stops)
+
         if sweeper.parameters[0] is Parameter.BIAS:
             for idx, jdx in enumerate(sweeper.indexes):
                 gen_ch = self.qubits[jdx].dac
+                if gen_ch is None:
+                    raise ValueError("Qubit dac (flux bias) not provided.")
                 sweep_type = "gain"
                 std_register = self.get_gen_reg(gen_ch, sweep_type)
                 swept_register = self.new_gen_reg(gen_ch, name=f"sweep_bias_{gen_ch}")
                 self.bias_sweep_registers[gen_ch] = (swept_register, std_register)
 
                 max_gain = int(self.soccfg["gens"][gen_ch]["maxv"])
                 starts = (sweeper.starts * max_gain).astype(int)
@@ -81,18 +96,21 @@
                 sweep_type = sweeper.parameters[idx].value
                 register = self.get_gen_reg(gen_ch, sweep_type)
 
                 if sweeper.parameters[idx] is Parameter.AMPLITUDE:
                     max_gain = int(self.soccfg["gens"][gen_ch]["maxv"])
                     starts = (sweeper.starts * max_gain).astype(int)
                     stops = (sweeper.stops * max_gain).astype(int)
-                elif sweeper.parameters[idx] is Parameter.DELAY:
-                    # define a new register for the delay
-                    register = self.new_gen_reg(gen_ch, reg_type="time", tproc_reg=True)
-                    pulse.start_delay = register
+                else:
+                    starts = sweeper.starts
+                    stops = sweeper.stops
+                    if sweeper.parameters[idx] is Parameter.DELAY:
+                        # define a new register for the delay
+                        register = self.new_gen_reg(gen_ch, reg_type="time", tproc_reg=True)
+                        pulse.start_delay = register
 
                 new_sweep = QickSweep(
                     self,
                     register,  # sweeper_register
                     starts[idx],  # start
                     stops[idx],  # stop
                     sweeper.expts,  # number of points
@@ -102,21 +120,15 @@
         self.add_sweep(merge_sweeps(sweep_list))
 
     def initialize(self):
         """Declre nyquist zones for all the DACs and all the readout frequencies.
 
         Function called by AveragerProgram.__init__.
         """
-        self.declare_nqz_zones([pulse for pulse in self.sequence if pulse.type == "drive"])
-        self.declare_nqz_flux()
-        if self.is_mux:
-            self.declare_gen_mux_ro()
-        else:
-            self.declare_nqz_zones([pulse for pulse in self.sequence if pulse.type == "readout"])
-        self.declare_readout_freq()
+        self.declare_zones_and_ro(self.sequence)
 
         self.pulses_registered = True
         for pulse in self.sequence:
             if self.is_mux:
                 if pulse.type != "drive":
                     continue
             self.add_pulse_to_register(pulse)
```

### Comparing `qibosoq-0.0.3/src/qibosoq/rfsoc_server.py` & `qibosoq-0.0.4/src/qibosoq/server.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,74 +1,85 @@
-"""Qibosoq server for qibolab-qick integration.
-
-Tested on the following FPGA:
-    * RFSoc4x2
-    * ZCU111
-"""
+"""Qibosoq server for qibolab-qick integration."""
 
 import json
 import logging
 import os
 import socket
 import traceback
 from socketserver import BaseRequestHandler, TCPServer
 from typing import Dict, List
 
+import numpy as np
 from qick import QickSoc
 
 import qibosoq.configuration as cfg
-from qibosoq.components.base import Config, OperationCode, Qubit, Sweeper
+from qibosoq.components.base import Config, OperationCode, Parameter, Qubit, Sweeper
 from qibosoq.components.pulses import Pulse, Shape
 from qibosoq.programs.pulse_sequence import ExecutePulseSequence
 from qibosoq.programs.sweepers import ExecuteSweeps
 
 logger = logging.getLogger(cfg.MAIN_LOGGER_NAME)
 qick_logger = logging.getLogger(cfg.PROGRAM_LOGGER_NAME)
 
 
 def load_pulses(list_sequence: List[Dict]) -> List[Pulse]:
     """Convert a list of pulses (in dict form) to a list of Pulse objects."""
     obj_sequence = []
     for pulse in list_sequence:
-        cls = Shape[pulse["shape"]].value
+        cls = Shape[pulse["shape"].upper()].value
         converted_pulse = cls(**pulse)
         obj_sequence.append(converted_pulse)
     return obj_sequence
 
 
+def load_sweeps(list_sweepers: List[Dict]) -> List[Sweeper]:
+    """Convert a list of sweepers (in dict form) to a list of Sweeper objects."""
+    sweepers = []
+    for sweep in list_sweepers:
+        converted_sweep = Sweeper(
+            expts=sweep["expts"],
+            parameters=[Parameter(par) for par in sweep["parameters"]],
+            starts=np.array(sweep["starts"]),
+            stops=np.array(sweep["stops"]),
+            indexes=sweep["indexes"],
+        )
+        sweepers.append(converted_sweep)
+    return sweepers
+
+
 def execute_program(data: dict, qick_soc: QickSoc) -> dict:
     """Create and execute qick programs.
 
     Returns:
         (dict): dictionary with two keys (i, q) to lists of values
     """
     opcode = OperationCode(data["operation_code"])
-    args = ()
+    args = []
     if opcode is OperationCode.EXECUTE_PULSE_SEQUENCE:
         programcls = ExecutePulseSequence
     elif opcode is OperationCode.EXECUTE_PULSE_SEQUENCE_RAW:
         programcls = ExecutePulseSequence
         data["cfg"]["soft_avgs"] = data["cfg"]["reps"]
         data["cfg"]["reps"] = 1
     elif opcode is OperationCode.EXECUTE_SWEEPS:
         programcls = ExecuteSweeps
-        args = tuple(Sweeper(**sweeper) for sweeper in data["sweepers"])
+        args = load_sweeps(data["sweepers"])
     else:
         raise NotImplementedError(f"Operation code {data['operation_code']} not supported")
 
     program = programcls(
         qick_soc,
         Config(**data["cfg"]),
         load_pulses(data["sequence"]),
         [Qubit(**qubit) for qubit in data["qubits"]],
         *args,
     )
 
     asm_prog = program.asm()
-    qick_logger.handlers[0].doRollover()
+    qick_logger.handlers[0].doRollover()  # type: ignore
     qick_logger.info(asm_prog)
 
     num_instructions = len(program.prog_list)
     max_mem = qick_soc["tprocs"][0]["pmem_size"]
     if num_instructions > max_mem:
         raise MemoryError(
             f"The tproc has a max memory size of {max_mem}, but the program had {num_instructions} instructions"
@@ -80,23 +91,18 @@
             load_pulses=True,
             progress=False,
             debug=False,
         )
         toti = [[results[0][0].tolist()]]
         totq = [[results[0][1].tolist()]]
     else:
-        toti, totq = program.acquire(
+        toti, totq = program.perform_experiment(
             qick_soc,
-            load_pulses=True,
-            progress=False,
-            debug=False,
-            average=data["average"],
+            average=data["cfg"]["average"],
         )
-        toti = toti.tolist()
-        totq = totq.tolist()
 
     return {"i": toti, "q": totq}
 
 
 class ConnectionHandler(BaseRequestHandler):
     """Handle requests to the server."""
 
@@ -123,24 +129,31 @@
         """
         # set the server in non-blocking mode
         self.server.socket.setblocking(False)
 
         try:
             data = self.receive_command()
             results = execute_program(data, self.server.qick_soc)
-        except Exception as exception:  # pylint: disable=bare-except, broad-exception-caught
+        except Exception:  # pylint: disable=W0612,W0718
             logger.exception("")
             logger.error("Faling command: %s", data)
             results = traceback.format_exc()
             self.server.qick_soc.reset_gens()
 
         self.request.sendall(bytes(json.dumps(results), "utf-8"))
 
 
+def log_initial_info():
+    """Log info regarding the loaded configuration."""
+    logger.info("Server listening, PID %d", os.getpid())
+    mux_str = "Multiplexed" if cfg.IS_MULTIPLEXED else "Not multiplexed"
+    logger.info("%s firmware loaded from %s", mux_str, cfg.QICKSOC_LOCATION)
+
+
 def serve(host, port):
     """Open the TCPServer and wait forever for connections."""
     # initialize QickSoc object (firmware and clocks)
     TCPServer.allow_reuse_address = True
     with TCPServer((host, port), ConnectionHandler) as server:
         server.qick_soc = QickSoc(bitfile=cfg.QICKSOC_LOCATION)
-        logger.info("Server listening, PID %d", os.getpid())
+        log_initial_info()
         server.serve_forever()
```

### Comparing `qibosoq-0.0.3/PKG-INFO` & `qibosoq-0.0.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qibosoq
-Version: 0.0.3
+Version: 0.0.4
 Summary: QIBO Server On Qick (qibosoq) is the server component of qibolab to be run on RFSoC boards
 Home-page: https://github.com/qiboteam/qibosoq/
 License: Apache-2.0
 Author: Rodolfo Carobene
 Author-email: rodolfo.carobene@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
@@ -24,33 +24,22 @@
 [![codecov](https://codecov.io/gh/qiboteam/qibosoq/branch/main/graph/badge.svg?token=1EKZKVEVX0)](https://codecov.io/gh/qiboteam/qibosoq)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8083285.svg)](https://doi.org/10.5281/zenodo.8083285)
 
 Repository for developing server side of RFSoC fpga boards
 Qibosoq is a server for integrating [Qick](https://github.com/openquantumhardware/qick) in the [Qibolab](https://github.com/qiboteam/qibolab) ecosystem
 for executing arbitrary pulses sequences on QPUs.
 
-The complete documentation for can be found at [qibo.science/qibosoq/stable](https://qibo.science/qibosoq/stable/)
+The complete documentation for can be found at:
+
+* [qibo.science/qibosoq/stable](https://qibo.science/qibosoq/stable/)
+* [qibo.science/qibosoq/latest](https://qibo.science/qibosoq/latest/)
 
-## Installation
-The package can be installed by source:
 
-```sh
-git clone https://github.com/qiboteam/qibosoq.git
-cd qibosoq
-pip install .
-```
-### Developer instructions
-For development make sure to install the package using [`poetry`](https://python-poetry.org/) and to install the pre-commit hooks:
-
-```sh
-git clone https://github.com/qiboteam/qibosoq.git
-cd qibosoq
-poetry install
-pre-commit install
-```
+## Installation
+Please refer to the [documentation](https://qibo.science/qibosoq/stable/getting-started/installation.html) for installation instructions.
 
 ## Configuration parameters
 
 In `configuration.py` some default qibosoq parameters are hardcoded. They can be changed using environment variables ([see documentation](https://qibo.science/qibosoq/stable/getting-started/usage.html)).
 
 * IP of the server
 * Port of the server
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: qibosoq Version: 0.0.3 Summary: QIBO Server On Qick
+Metadata-Version: 2.1 Name: qibosoq Version: 0.0.4 Summary: QIBO Server On Qick
 (qibosoq) is the server component of qibolab to be run on RFSoC boards Home-
 page: https://github.com/qiboteam/qibosoq/ License: Apache-2.0 Author: Rodolfo
 Carobene Author-email: rodolfo.carobene@gmail.com Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
@@ -13,31 +13,29 @@
 codecov.io/gh/qiboteam/qibosoq/branch/main/graph/badge.svg?token=1EKZKVEVX0)]
 (https://codecov.io/gh/qiboteam/qibosoq) [![DOI](https://zenodo.org/badge/DOI/
 10.5281/zenodo.8083285.svg)](https://doi.org/10.5281/zenodo.8083285) Repository
 for developing server side of RFSoC fpga boards Qibosoq is a server for
 integrating [Qick](https://github.com/openquantumhardware/qick) in the
 [Qibolab](https://github.com/qiboteam/qibolab) ecosystem for executing
 arbitrary pulses sequences on QPUs. The complete documentation for can be found
-at [qibo.science/qibosoq/stable](https://qibo.science/qibosoq/stable/) ##
-Installation The package can be installed by source: ```sh git clone https://
-github.com/qiboteam/qibosoq.git cd qibosoq pip install . ``` ### Developer
-instructions For development make sure to install the package using [`poetry`]
-(https://python-poetry.org/) and to install the pre-commit hooks: ```sh git
-clone https://github.com/qiboteam/qibosoq.git cd qibosoq poetry install pre-
-commit install ``` ## Configuration parameters In `configuration.py` some
-default qibosoq parameters are hardcoded. They can be changed using environment
-variables ([see documentation](https://qibo.science/qibosoq/stable/getting-
-started/usage.html)). * IP of the server * Port of the server * Paths of log
-files * Name of python loggers * Path of bitstream * Type of readout
-(multiplexed or not, depending on the loaded bitstream) ## Run the server The
-simplest way of executing the server is: ``` sudo -E python -m qibosoq ``` and
-the server can be closed with `Ctrl-C`.\ Note that with this command the script
-will close as soon as the terminal where it's running it's closed. To run the
-server in detached mode you can use: ``` nohup sudo -E python -m qibosoq & ```
-And the server can be closed with `sudo kill ` (PID will be saved in log). ###
-TII boards With TII boards the server can also be executed using the alias
-`server-run-bkg`. Also, two additional command are added in `.bashrc`:
-`serverinfo` and `serverclose`. `serverinfo` will print the PID if the server
-is running, otherwise will print "No running server". `serverclose` will close
-the server, if it is running. All these commands require sudo privileges. ##
-Contributing Contributions, issues and feature requests are welcome! Feel free
-to check [GitHub_issues]
+at: * [qibo.science/qibosoq/stable](https://qibo.science/qibosoq/stable/) *
+[qibo.science/qibosoq/latest](https://qibo.science/qibosoq/latest/) ##
+Installation Please refer to the [documentation](https://qibo.science/qibosoq/
+stable/getting-started/installation.html) for installation instructions. ##
+Configuration parameters In `configuration.py` some default qibosoq parameters
+are hardcoded. They can be changed using environment variables ([see
+documentation](https://qibo.science/qibosoq/stable/getting-started/
+usage.html)). * IP of the server * Port of the server * Paths of log files *
+Name of python loggers * Path of bitstream * Type of readout (multiplexed or
+not, depending on the loaded bitstream) ## Run the server The simplest way of
+executing the server is: ``` sudo -E python -m qibosoq ``` and the server can
+be closed with `Ctrl-C`.\ Note that with this command the script will close as
+soon as the terminal where it's running it's closed. To run the server in
+detached mode you can use: ``` nohup sudo -E python -m qibosoq & ``` And the
+server can be closed with `sudo kill ` (PID will be saved in log). ### TII
+boards With TII boards the server can also be executed using the alias `server-
+run-bkg`. Also, two additional command are added in `.bashrc`: `serverinfo` and
+`serverclose`. `serverinfo` will print the PID if the server is running,
+otherwise will print "No running server". `serverclose` will close the server,
+if it is running. All these commands require sudo privileges. ## Contributing
+Contributions, issues and feature requests are welcome! Feel free to check
+[GitHub_issues]
```

