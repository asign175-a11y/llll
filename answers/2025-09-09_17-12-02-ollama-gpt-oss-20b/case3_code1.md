| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :-: | :- | :-: | :- | :- | :- |
| 1 | `from qiskit.qasm import Qasm` | * | Deprecation -> qiskit.qasm module deprecated (optional) | qiskit.qasm | `from qiskit.circuit import QuantumCircuit` |
| 5 | `circuit2 = Qasm(filename=qasm_file)` | * | Deprecation -> qiskit.qasm module deprecated (optional) | qiskit.qasm | `qc2 = QuantumCircuit.from_qasm_file(qasm_file)` |
| 6 | `program2 = circuit2.parse()` | * | Deprecation -> qiskit.qasm module deprecated (optional) | qiskit.qasm |  |
| 7 | `qc2 = program2.get_circuit()` | * | Deprecation -> qiskit.qasm module deprecated (optional) | qiskit.qasm |  |