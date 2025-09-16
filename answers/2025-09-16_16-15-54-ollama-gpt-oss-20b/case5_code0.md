| Line | Code | Scenario ID | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
| 1 | {"data":"from qiskit import QuantumCircuit, QuantumRegister | | | | |
| 2 | from qiskit.extensions import HGate, XGate, Initialize | S001 | DEPRECATION - The qiskit.extensions module is deprecated | qiskit.extensions | from qiskit.circuit.library import HGate, XGate, Initialize |
| 3 | from qiskit.extensions import Barrier | S002 | DEPRECATION - The qiskit.extensions module is deprecated | qiskit.extensions | from qiskit.circuit import Barrier |
| 4 | from qiskit.extensions import UnitaryGate | S003 | DEPRECATION - The qiskit.extensions module is deprecated | qiskit.extensions | from qiskit.circuit.library import UnitaryGate |
| 5 | import numpy as np | | | | |
| 6 |  | | | | |
| 7 | qr = QuantumRegister(3) | | | | |
| 8 | qc = QuantumCircuit(qr) | | | | |
| 9 |  | | | | |
| 10 | qc.append(HGate(), [qr[0]]) | | | | |
| 11 | qc.append(XGate(), [qr[1]]) | | | | |
| 12 |  | | | | |
| 13 | custom_matrix = np.array([[0, 1], [1, 0]]) | | | | |
| 14 | custom_gate = UnitaryGate(custom_matrix, label="Custom") | | | | |
| 15 | qc.append(custom_gate, [qr[2]]) | | | | |
| 16 |  | | | | |
| 17 | psi = [1/np.sqrt(2), 1/np.sqrt(2)] | | | | |
| 18 | init_gate = Initialize(psi) | | | | |
| 19 | qc.append(init_gate, [qr[0]]) | | | | |
| 20 |  | | | | |
| 21 | qc.append(Barrier(3), [qr[0], qr[1], qr[2]]) | | | | |
| 22 | print(qc.draw())"} | | | | |