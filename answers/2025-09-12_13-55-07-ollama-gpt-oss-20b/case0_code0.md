Find migration rules to update the following Qiskit code to version 0.46.0.

```python
{"data":"'''\n    Test code for importing and \n    using libraries that are not related to Qiskit.\n'''\n\n\n# requeriments imports\n\n# import os funcionalities\nimport os\n\n# import QuantumCircuit funcionalities\nfrom qiskit import QuantumCircuit\n\n# import datetime funcionalidades\nfrom datetime import datetime\n\n# create a Quantum Circuit\nqc = QuantumCircuit(2, 2)\nqc.h(0)\nqc.cx(0, 1)\nqc.measure(0, 0)\nqc.measure(1, 1)\n\n# print\nprint(\"work done !\")"}
```

| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
|  |  |  |  |  |  |