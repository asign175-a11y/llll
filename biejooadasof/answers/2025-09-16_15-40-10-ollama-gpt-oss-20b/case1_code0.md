| Line | Code | Scenario ID | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
| 1 | import os |  |  |  |  |
| 2 | from qiskit import QuantumCircuit |  |  |  |  |
| 3 | from datetime import datetime |  |  |  |  |
| 4 | from qiskit.qasm import Qasm | qiskit-0.46-qasm-deprecated | DEPRECATION - qiskit.qasm.Qasm is deprecated in 0.46 | qiskit.qasm | # from qiskit.qasm import Qasm (removed, use qiskit.qasm2 instead) |
| 5 | from qiskit.algorithms import VQE |  |  |  |  |
| 6 | from qiskit import qasm2 as qasm |  |  |  |  |
| 7 |  |  |  |  |  |
| 8 | qc = QuantumCircuit(2, 2) |  |  |  |  |
| 9 | qc.h(0) |  |  |  |  |
| 10 | qc.cx(0, 1) |  |  |  |  |
| 11 | qc.measure(0, 0) |  |  |  |  |
| 12 | qc.measure(1, 1) |  |  |  |  |
| 13 |  |  |  |  |  |
| 14 | # print |  |  |  |  |
| 15 | print("work done !") |  |  |  |  |