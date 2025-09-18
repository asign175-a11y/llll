Find migration rules to update the following Qiskit code to version 0.46.0.

```python
{"data":"from qiskit import QuantumCircuit\nqc = QuantumCircuit(2, 2)\nqc.h(0)\nqc.cx(0, 1)\nqc.measure(0, 0)\nqc.measure(1, 1)\n\nfrom qiskit import Aer\nbackend = Aer.get_backend('aer_simulator')\n\nfrom qiskit import execute\njob = execute(qc, backend, shots=1000)\n\nfrom qiskit.tools.visualization import plot_histogram\nplot_histogram(job.result().get_counts(qc))\n\nfrom qiskit.algorithms import VQE\nfrom qiskit.circuit.library import TwoLocal\nfrom qiskit import SPSA\nvqe = VQE(TwoLocal(rotation_blocks=\"ry\", entanglement_blocks=\"cz\"), SPSA())"}
```