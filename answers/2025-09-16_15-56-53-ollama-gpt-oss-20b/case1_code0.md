```markdown
| Line | Code | Scenario ID | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
| 1 | import os | | | | |
| 2 | from qiskit import QuantumCircuit | | | | |
| 3 | from datetime import datetime | | | | |
| 4 | from qiskit.qasm import Qasm | d385f8bd-1f25-4635-bb9e-26b168b25fc9 | DEPRECATION - The qiskit.qasm module is deprecated | qiskit.qasm | from qiskit.qasm2 import Qasm |
| 5 | from qiskit.algorithms import VQE | | | | |
| 6 | from qiskit import qasm2 as qasm | | | | |
| 7 |  | | | | |
| 8 | qc = QuantumCircuit(2, 2) | | | | |
| 9 | qc.h(0) | | | | |
| 10 | qc.cx(0, 1) | | | | |
| 11 | qc.measure(0, 0) | | | | |
| 12 | qc.measure(1, 1) | | | | |
| 13 |  | | | | |
| 14 | # print | | | | |
| 15 | print("work done !") | | | | |
```