| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| ----- | ----- | ----- | ----- | ----- | ----- |
| 1 | from qiskit.qasm import Qasm | qiskit.qasm.Qasm.removed_0_46 | Deprecation -> The `qiskit.qasm.Qasm` class has been removed. | qiskit.qasm.Qasm | from qiskit.circuit import QuantumCircuit |
| 5 | circuit2 = Qasm(filename=qasm_file) | qiskit.qasm.Qasm.removed_0_46 | Deprecation -> The `qiskit.qasm.Qasm` class has been removed. | qiskit.qasm.Qasm | qc2 = QuantumCircuit.from_qasm_file(qasm_file) |
| 6 | program2 = circuit2.parse() | qiskit.qasm.Qasm.removed_0_46 | Deprecation -> The `qiskit.qasm.Qasm` class has been removed. | qiskit.qasm.Qasm.parse | |
| 7 | qc2 = program2.get_circuit() | qiskit.qasm.Qasm.removed_0_46 | Deprecation -> The `qiskit.qasm.Qasm` class has been removed. | qiskit.qasm.Qasm.get_circuit | |