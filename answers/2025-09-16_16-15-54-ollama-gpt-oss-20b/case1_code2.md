| Line | Code | Scenario ID | Scenario | Artifact | Refactoring |
| :--: | :--- | :----------: | :------- | :------- | :---------- |
| 1 | import os |  |  |  |  |
| 2 | from datetime import datetime |  |  |  |  |
| 3 | from qiskit import QuantumCircuit, qasm, execute |  | DEPRECATION - `qiskit.qasm` module is deprecated | `qiskit.qasm` | from qiskit import QuantumCircuit, execute |
| 4 | import matplotlib.pyplot as plt |  |  |  |  |
| 5 | from utils import getMyBackend |  |  |  |  |
| 6 |  |  |  |  |  |
| 7 | qc = QuantumCircuit(2, 2) |  |  |  |  |
| 8 | qc.h(0) |  |  |  |  |
| 9 | qc.cx(0, 1) |  |  |  |  |
| 10 | qc.measure(0, 0) |  |  |  |  |
| 11 | qc.measure(1, 1) |  |  |  |  |
| 12 |  |  |  |  |  |
| 13 | job = execute(qc, getMyBackend(), shots=1000) |  |  |  |  |
| 14 | result = job.result().get_counts(qc) |  |  |  |  |
| 15 | plt.show() |  |  |  |  |