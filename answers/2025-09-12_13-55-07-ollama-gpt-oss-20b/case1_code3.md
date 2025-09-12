Find migration rules to update the following Qiskit code to version 0.46.0.

```python
{"data":"import os\nfrom datetime import datetime\nfrom qiskit import QuantumCircuit, execute, Aer, qasm\nimport matplotlib.pyplot as plt\nfrom utils import getJob\n\nqc = QuantumCircuit(2, 2)\nqc.h(0)\nqc.cx(0, 1)\nqc.measure(0, 0)\nqc.measure(1, 1)\n\nbackend = Aer.get_backend('aer_simulator')\njob = getJob(qc, backend, 1000)\nresult = job.result().get_counts(qc)\nplt.show()"}
```
