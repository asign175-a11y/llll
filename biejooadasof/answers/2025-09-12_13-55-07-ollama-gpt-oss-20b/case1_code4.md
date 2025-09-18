Find migration rules to update the following Qiskit code to version 0.46.0.

```python
{"data":"import os\n\nfrom qiskit import QuantumCircuit \nqc = QuantumCircuit(2, 2)\nqc.h(0)\nqc.cx(0, 1)\nqc.measure(0, 0)\nqc.measure(1, 1)\n\nfrom qiskit import Aer\nbackend = Aer.get_backend('aer_simulator')\n\nfrom utils import getJob\nfrom datetime import datetime\njob = getJob(qc, backend, 1000).result().get_counts(qc)\n\nimport matplotlib.pyplot as plt\nqc.draw(output='mpl')\nplt.show()"}
```

---


| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
|     |     |             |          |          |             |