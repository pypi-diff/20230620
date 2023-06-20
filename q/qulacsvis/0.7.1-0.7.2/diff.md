# Comparing `tmp/qulacsvis-0.7.1.tar.gz` & `tmp/qulacsvis-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qulacsvis-0.7.1.tar", max compression
+gzip compressed data, was "qulacsvis-0.7.2.tar", max compression
```

## Comparing `qulacsvis-0.7.1.tar` & `qulacsvis-0.7.2.tar`

### file list

```diff
@@ -1,14 +1,18 @@
--rw-r--r--   0        0        0     1069 2023-06-15 09:04:22.075056 qulacsvis-0.7.1/LICENSE
--rw-r--r--   0        0        0     4131 2023-06-15 09:04:22.075056 qulacsvis-0.7.1/README.md
--rw-r--r--   0        0        0     1063 2023-06-15 09:04:22.075056 qulacsvis-0.7.1/pyproject.toml
--rw-r--r--   0        0        0       50 2023-06-15 09:04:22.075056 qulacsvis-0.7.1/qulacsvis/__init__.py
--rw-r--r--   0        0        0        0 2023-06-15 09:04:22.079056 qulacsvis-0.7.1/qulacsvis/utils/__init__.py
--rw-r--r--   0        0        0     2720 2023-06-15 09:04:22.079056 qulacsvis-0.7.1/qulacsvis/utils/gate.py
--rw-r--r--   0        0        0     3894 2023-06-15 09:04:22.079056 qulacsvis-0.7.1/qulacsvis/utils/latex.py
--rw-r--r--   0        0        0      243 2023-06-15 09:04:22.079056 qulacsvis-0.7.1/qulacsvis/visualization/__init__.py
--rw-r--r--   0        0        0     4503 2023-06-15 09:04:22.079056 qulacsvis-0.7.1/qulacsvis/visualization/circuit_drawer.py
--rw-r--r--   0        0        0     3877 2023-06-15 09:04:22.079056 qulacsvis-0.7.1/qulacsvis/visualization/circuit_parser.py
--rw-r--r--   0        0        0     9492 2023-06-15 09:04:22.079056 qulacsvis-0.7.1/qulacsvis/visualization/latex.py
--rw-r--r--   0        0        0    16480 2023-06-15 09:04:22.079056 qulacsvis-0.7.1/qulacsvis/visualization/matplotlib.py
--rw-r--r--   0        0        0    34179 2023-06-15 09:04:22.079056 qulacsvis-0.7.1/qulacsvis/visualization/text.py
--rw-r--r--   0        0        0     5150 1970-01-01 00:00:00.000000 qulacsvis-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-20 08:09:02.842449 qulacsvis-0.7.2/LICENSE
+-rw-r--r--   0        0        0     4131 2023-06-20 08:09:02.842449 qulacsvis-0.7.2/README.md
+-rw-r--r--   0        0        0     1063 2023-06-20 08:09:02.842449 qulacsvis-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0       50 2023-06-20 08:09:02.842449 qulacsvis-0.7.2/qulacsvis/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-20 08:09:02.842449 qulacsvis-0.7.2/qulacsvis/models/__init__.py
+-rw-r--r--   0        0        0     3297 2023-06-20 08:09:02.842449 qulacsvis-0.7.2/qulacsvis/models/circuit.py
+-rw-r--r--   0        0        0        0 2023-06-20 08:09:02.842449 qulacsvis-0.7.2/qulacsvis/qulacs/__init__.py
+-rw-r--r--   0        0        0      732 2023-06-20 08:09:02.842449 qulacsvis-0.7.2/qulacsvis/qulacs/circuit.py
+-rw-r--r--   0        0        0        0 2023-06-20 08:09:02.842449 qulacsvis-0.7.2/qulacsvis/utils/__init__.py
+-rw-r--r--   0        0        0     2720 2023-06-20 08:09:02.842449 qulacsvis-0.7.2/qulacsvis/utils/gate.py
+-rw-r--r--   0        0        0     3894 2023-06-20 08:09:02.842449 qulacsvis-0.7.2/qulacsvis/utils/latex.py
+-rw-r--r--   0        0        0      243 2023-06-20 08:09:02.842449 qulacsvis-0.7.2/qulacsvis/visualization/__init__.py
+-rw-r--r--   0        0        0     4571 2023-06-20 08:09:02.842449 qulacsvis-0.7.2/qulacsvis/visualization/circuit_drawer.py
+-rw-r--r--   0        0        0      603 2023-06-20 08:09:02.842449 qulacsvis-0.7.2/qulacsvis/visualization/circuit_parser.py
+-rw-r--r--   0        0        0     9211 2023-06-20 08:09:02.842449 qulacsvis-0.7.2/qulacsvis/visualization/latex.py
+-rw-r--r--   0        0        0    16211 2023-06-20 08:09:02.842449 qulacsvis-0.7.2/qulacsvis/visualization/matplotlib.py
+-rw-r--r--   0        0        0    34165 2023-06-20 08:09:02.842449 qulacsvis-0.7.2/qulacsvis/visualization/text.py
+-rw-r--r--   0        0        0     5150 1970-01-01 00:00:00.000000 qulacsvis-0.7.2/PKG-INFO
```

### Comparing `qulacsvis-0.7.1/LICENSE` & `qulacsvis-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `qulacsvis-0.7.1/README.md` & `qulacsvis-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `qulacsvis-0.7.1/pyproject.toml` & `qulacsvis-0.7.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qulacsvis"
-version = "0.7.1"
+version = "0.7.2"
 readme = "README.md"
 description = "visualizers for qulacs"
 repository = "https://github.com/Qulacs-Osaka/qulacs-visualizer"
 homepage = "https://github.com/Qulacs-Osaka/qulacs-visualizer"
 documentation = "https://qulacs-osaka.github.io/qulacs-visualizer"
 authors = ["Qulacs-Osaka <you@example.com>"]
 license = "MIT"
```

### Comparing `qulacsvis-0.7.1/qulacsvis/utils/gate.py` & `qulacsvis-0.7.2/qulacsvis/utils/gate.py`

 * *Files identical despite different names*

### Comparing `qulacsvis-0.7.1/qulacsvis/utils/latex.py` & `qulacsvis-0.7.2/qulacsvis/utils/latex.py`

 * *Files identical despite different names*

### Comparing `qulacsvis-0.7.1/qulacsvis/visualization/circuit_drawer.py` & `qulacsvis-0.7.2/qulacsvis/visualization/circuit_drawer.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 import matplotlib  # NOQA
 from PIL import Image
 from qulacs import QuantumCircuit
 
 from qulacsvis.utils.latex import _LatexCompiler, _PDFtoImage
 
+from ..qulacs.circuit import to_model
 from .latex import LatexSourceGenerator
 from .matplotlib import MPLCircuitlDrawer
 from .text import TextCircuitDrawer
 
 
 def circuit_drawer(
     circuit: QuantumCircuit,
@@ -105,34 +106,34 @@
     if output_method == "text":
         text_drawer = TextCircuitDrawer(circuit, dot=dot)
         text_drawer.draw(verbose=verbose)
         return None
 
     elif output_method == "latex":
         with tempfile.TemporaryDirectory() as tmpdir:
-            generator = LatexSourceGenerator(circuit)
+            generator = LatexSourceGenerator(to_model(circuit))
             latex_source = generator.generate()
             latex = _LatexCompiler()
             pdftoimage = _PDFtoImage()
 
             latex.compile(latex_source, tmpdir, "circuit_drawer")
             pdftoimage.convert(os.path.join(tmpdir, "circuit_drawer"), ppi=ppi)
 
             if filename:
                 shutil.copyfile(os.path.join(tmpdir, "circuit_drawer.png"), filename)
 
             image = Image.open(os.path.join(tmpdir, "circuit_drawer.png"))
             return image
 
     elif output_method == "latex_source":
-        generator = LatexSourceGenerator(circuit)
+        generator = LatexSourceGenerator(to_model(circuit))
         latex_source = generator.generate()
         return latex_source
 
     elif output_method == "mpl":
-        mpl_drawer = MPLCircuitlDrawer(circuit, dpi=dpi, scale=scale)
+        mpl_drawer = MPLCircuitlDrawer(to_model(circuit), dpi=dpi, scale=scale)
         return mpl_drawer.draw(filename=filename)
 
     else:
         raise ValueError(
             "Invalid output_method. Valid options are: 'text', 'latex', 'latex_source', 'mpl'."
         )
```

### Comparing `qulacsvis-0.7.1/qulacsvis/visualization/latex.py` & `qulacsvis-0.7.2/qulacsvis/visualization/latex.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,64 +1,54 @@
 from typing import List
 
 import numpy as np
-from qulacs import QuantumCircuit
 
+from qulacsvis.models.circuit import CircuitData, ControlQubitInfo, GateData
 from qulacsvis.utils.gate import grouping_adjacent_gates, to_latex_style
-from qulacsvis.visualization.circuit_parser import (
-    CircuitParser,
-    ControlQubitInfo,
-    GateData,
-)
 
 
 class LatexSourceGenerator:
-    """Generate latex source from QuantumCircuit
+    """Generate latex source from CircuitData
 
     Parameters
     ----------
-    circuit : QuantumCircuit
+    circuit : CircuitData
         A quantum circuit to be drawn.
 
     Attributes
     ----------
-    _quantum_circuit : QuantumCircuit
-        A quantum circuit to be drawn.
-    _parser : CircuitParser
-        The parser of the quantum circuit.
     _circuit_data : CircuitData
-        The data of the quantum circuit after parsing by CircuitParser.
+        The data of the quantum circuit.
     _circuit : numpy.ndarray
         A matrix containing strings converted from CircuitData for Qcircuit.
         Each element and its position corresponds to one of GateData.
         Quantum circuit only, input values are not contained.
     _head : str
         The head of the latex source containing preamble.
     _tail : str
         The tail of the latex source.
 
     Examples
     --------
     >>> from qulacs import QuantumCircuit
+    >>> from qulacsvis.qulacs.circuit import to_model
     >>> from qulacsvis.visualization import LatexSourceGenerator
     >>>
     >>> circuit = QuantumCircuit(3)
     >>> circuit.add_X_gate(0)
     >>> circuit.add_Y_gate(1)
     >>> circuit.add_Z_gate(2)
     >>>
-    >>> generator = LatexSourceGenerator(circuit)
+    >>> generator = LatexSourceGenerator(to_model(circuit))
     >>> latex_source = generator.generate()
     >>> print(latex_source)
     """
 
-    def __init__(self, circuit: QuantumCircuit):
-        self._quantum_circuit = circuit
-        self._parser = CircuitParser(circuit)
-        self._circuit_data = self._parser.parsed_circuit
+    def __init__(self, circuit: CircuitData):
+        self._circuit_data = circuit
         self._circuit = np.array([[]])
         self._head = r"""
 \documentclass[border={-2pt 5pt 5pt -7pt}]{standalone}
 \usepackage[braket, qm]{qcircuit}
 \usepackage{graphicx}
 
 \begin{document}
@@ -70,16 +60,16 @@
         """Generate latex source from QuantumCircuit
 
         Returns
         -------
         latex_source : str
             String of latex source generated
         """
-        qubit_count = self._parser.qubit_count
-        circuit_layer_count = len(self._circuit_data[0])
+        qubit_count = self._circuit_data.qubit_count
+        circuit_layer_count = self._circuit_data.layer_count
 
         input_label = np.array(
             [
                 [
                     # nghost reserves drawing area for input label,
                     # adjusts the spacing between rows.
                     r"\nghost{ q_{" + str(i) + "} : }",
@@ -92,15 +82,15 @@
         self._circuit = np.array([[] for _ in range(qubit_count)])
         for layer in range(circuit_layer_count):
             # This is an array containing strings.
             # The string for each element is the string for the Qcircuit of the gate
             # corresponding to each qubit row of the layer currently of interest.
             current_layer_latex = [to_latex_style("wire") for _ in range(qubit_count)]
             for qubit in range(qubit_count):
-                gate = self._circuit_data[qubit][layer]
+                gate = self._circuit_data.gates[qubit][layer]
 
                 if gate.name == "ghost":
                     continue
                 elif gate.name == "wire":
                     continue
                 elif gate.name == "CNOT":
                     self._cnot(current_layer_latex, gate)
@@ -122,15 +112,15 @@
 
     def _matrix_to_qcircuit_style(self, matrix: List[List[str]]) -> str:
         """Generate from matrix to string for Qcircuit
 
         Parameters
         ----------
         matrix : List[List[str]]
-            A matrix containing strings converted from CircuitData for Qcircuit.
+            A matrix containing strings converted from GateDataSeq for Qcircuit.
         Returns
         -------
         res : str
             Generated string for Qcircuit from matrix
         """
         lines = [" & ".join(line) for line in matrix]
         # add indent for latex source file
```

### Comparing `qulacsvis-0.7.1/qulacsvis/visualization/matplotlib.py` & `qulacsvis-0.7.2/qulacsvis/visualization/matplotlib.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,26 @@
 from typing import List, Optional, Tuple
 
 import matplotlib
 from matplotlib import patches
 from matplotlib import pyplot as plt
-from qulacs import QuantumCircuit
 from typing_extensions import Final
 
-from qulacsvis.utils.gate import grouping_adjacent_gates, to_latex_style
-
-from .circuit_parser import (
-    GATE_DEFAULT_HEIGHT,
-    GATE_DEFAULT_WIDTH,
-    CircuitData,
-    CircuitParser,
-    ControlQubitInfo,
-    GateData,
-)
+from ..models.circuit import CircuitData, ControlQubitInfo, GateData
+from ..utils.gate import grouping_adjacent_gates, to_latex_style
 
 MATPLOTLIB_INLINE_BACKENDS = {
     "module://ipykernel.pylab.backend_inline",
     "module://matplotlib_inline.backend_inline",
     "nbAgg",
 }
 
+GATE_DEFAULT_WIDTH = 1.0
+GATE_DEFAULT_HEIGHT = 1.5
+
 GATE_MARGIN_RIGHT: Final[float] = 0.5
 GATE_MARGIN_LEFT: Final[float] = 0.5
 GATE_MARGIN_BOTTOM: Final[float] = 0.5
 GATE_MARGIN_TOP: Final[float] = 0.5
 
 PORDER_LINE: Final[int] = 2
 PORDER_GATE: Final[int] = 3
@@ -35,68 +29,63 @@
 
 class MPLCircuitlDrawer:
     """
     Drawing a circuit using Matplotlib.
 
     Parameters
     ----------
-    circuit : QuantumCircuit
+    circuit : CircuitData
         A quantum circuit to be drawn.
     dpi : int optional default=72
         The resolution of the figure.
     scale : float optional default=0.6
         The scale of the figure.
 
     Attributes
     ----------
     _figure : matplotlib.figure.Figure
         The figure of the circuit.
     _ax : matplotlib.axes.Axes
         The axes of the figure.
-    _circuit : QuantumCircuit
+    _circuit : CircuitData
         The quantum circuit to be drawn.
-    _parser : CircuitParser
-        The parser of the quantum circuit.
-    _circuit_data : CircuitData
-        The data of the quantum circuit after parsing by CircuitParser.
     _fig_scale_factor : float
         The scale factor of the figure.
 
     Examples
     --------
     >>> from qulacs import QuantumCircuit
+    >>> from qulacsvis.qulacs.circuit import to_model
     >>> from qulacsvis.visualization import MPLCircuitlDrawer
     >>> import matplotlib.pyplot as plt
     >>>
     >>> circuit = QuantumCircuit(3)
     >>> circuit.add_X_gate(0)
     >>> circuit.add_Y_gate(1)
     >>> circuit.add_Z_gate(2)
     >>>
-    >>> drawer = MPLCircuitlDrawer(circuit)
+    >>> drawer = MPLCircuitlDrawer(to_model(circuit))
     >>> drawer.draw()
     >>> plt.show()
     """
 
     def __init__(
         self,
-        circuit: QuantumCircuit,
+        circuit: CircuitData,
         *,
         dpi: int = 72,
         scale: float = 0.6,
     ):
         self._figure = plt.figure(dpi=dpi)
         self._figure.subplots_adjust(left=0, right=1, bottom=0, top=1)
         self._ax = self._figure.add_subplot(111)
         self._ax.set_aspect("equal")
         self._ax.axis("off")
 
         self._circuit = circuit
-        self._parser = CircuitParser(circuit)
-        self._circuit_data: CircuitData = self._parser.parsed_circuit
         self._fig_scale_factor = scale
 
     def draw(
         self, *, debug: bool = False, filename: Optional[str] = None
     ) -> matplotlib.figure.Figure:
         """
         Draw the circuit.
@@ -113,30 +102,32 @@
         self._figure : matplotlib.figure.Figure
             The figure of the circuit.
         """
         if debug:
             self._ax.axis("on")
             self._ax.grid()
 
-        circuit_layer_count = len(self._circuit_data[0])
+        circuit_qubit_count = self._circuit.qubit_count
+        circuit_layer_count = self._circuit.layer_count
+        layer_width = [GATE_DEFAULT_WIDTH for _ in range(circuit_layer_count)]
         # When the input is an empty quantum circuit
-        if self._parser.layer_width == []:
-            self._parser.layer_width = [GATE_DEFAULT_WIDTH]
+        if layer_width == []:
+            layer_width = [GATE_DEFAULT_WIDTH]
         # X/Y coordinates of the area where the circuit will be drawn.
         # Used to resize the figure.
         # In particular, the X coordinate is also used
         # as the right end (max_x) and left end (min_x) coordinates of the circuit wire.
         circuit_max_x = (
-            sum(self._parser.layer_width)
+            sum(layer_width)
             + circuit_layer_count * GATE_MARGIN_RIGHT
-            - self._parser.layer_width[0] / 2
+            - layer_width[0] / 2
         )
-        circuit_min_x = -self._parser.layer_width[0] / 2 - GATE_MARGIN_LEFT
+        circuit_min_x = -layer_width[0] / 2 - GATE_MARGIN_LEFT
         circuit_max_y = (
-            self._parser.qubit_count * (GATE_DEFAULT_HEIGHT + GATE_MARGIN_BOTTOM)
+            circuit_qubit_count * (GATE_DEFAULT_HEIGHT + GATE_MARGIN_BOTTOM)
             - GATE_MARGIN_BOTTOM
             - GATE_DEFAULT_HEIGHT / 2
         )
 
         # Determine the size of the figure (drawing size of the circuit + margins)
         QUBIT_LABEL_WIDTH = 2
         self._ax.set_xlim(
@@ -151,15 +142,15 @@
         fig_width = abs(self._ax.get_xlim()[1] - self._ax.get_xlim()[0])
         fig_heigth = abs(self._ax.get_ylim()[1] - self._ax.get_ylim()[0])
         self._figure.set_size_inches(
             fig_width * self._fig_scale_factor, fig_heigth * self._fig_scale_factor
         )
 
         # Draw a Qubit label for the number of Qubits in the quantum circuit and a wire
-        for qubit in range(self._parser.qubit_count):
+        for qubit in range(circuit_qubit_count):
             line_ypos = qubit * (GATE_DEFAULT_HEIGHT + GATE_MARGIN_BOTTOM)
             self._text(
                 circuit_min_x - 1,
                 line_ypos,
                 r"$q_{" + str(qubit) + r"}$",
                 fontsize=30,
             )
@@ -173,16 +164,16 @@
             )
 
         # x-coordinate of the layer currently being drawn
         layer_xpos = 0.0
 
         # Draw a gate for each layer
         for layer in range(circuit_layer_count):
-            for qubit in range(self._parser.qubit_count):
-                gate = self._circuit_data[qubit][layer]
+            for qubit in range(circuit_qubit_count):
+                gate = self._circuit.gates[qubit][layer]
                 qubit_ypos = qubit * (GATE_DEFAULT_HEIGHT + GATE_MARGIN_BOTTOM)
                 if gate.name == "ghost":
                     continue
                 elif gate.name == "wire":
                     continue
                 elif gate.name == "CNOT":
                     self._cnot(gate, (layer_xpos, qubit_ypos))
@@ -192,15 +183,15 @@
                     self._swap(gate, (layer_xpos, qubit_ypos))
                 elif len(gate.target_bits) > 1:
                     self._multi_gate(gate, (layer_xpos, qubit_ypos))
                 else:
                     self._gate_with_size(gate, (layer_xpos, qubit_ypos), 1)
 
             # Determine the x-coordinate of the next layer
-            layer_xpos += self._parser.layer_width[layer] + GATE_MARGIN_RIGHT
+            layer_xpos += layer_width[layer] + GATE_MARGIN_RIGHT
 
         if filename:
             self._figure.savefig(
                 filename,
                 # need some options?
             )
```

### Comparing `qulacsvis-0.7.1/qulacsvis/visualization/text.py` & `qulacsvis-0.7.2/qulacsvis/visualization/text.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import dataclasses
 import shutil
 from typing import Dict, List, Tuple
 
 import numpy as np
 from qulacs import QuantumCircuit, QuantumGateBase
 
+from qulacsvis.models.circuit import ControlQubitInfo
 from qulacsvis.utils.gate import to_text_style
-from qulacsvis.visualization.circuit_parser import ControlQubitInfo
 
 
 @dataclasses.dataclass
 class DotStyle:
     ctrl: str
     ctrlo: str
```

### Comparing `qulacsvis-0.7.1/PKG-INFO` & `qulacsvis-0.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qulacsvis
-Version: 0.7.1
+Version: 0.7.2
 Summary: visualizers for qulacs
 Home-page: https://github.com/Qulacs-Osaka/qulacs-visualizer
 License: MIT
 Author: Qulacs-Osaka
 Author-email: you@example.com
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

