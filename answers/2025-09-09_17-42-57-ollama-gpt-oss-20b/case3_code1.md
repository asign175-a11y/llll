| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
|:-:|:-|:-:|:-|:-|:-|
| 1 | from qiskit.qasm import Qasm | * | Deprecation -> qiskit.qasm.Qasm class deprecated | qiskit.qasm.Qasm | from qiskit.circuit import QuantumCircuit |
| 5 | circuit2 = Qasm(filename=qasm_file) | * | Deprecation -> qiskit.qasm.Qasm class usage deprecated | qiskit.qasm.Qasm | qc2 = QuantumCircuit.from_qasm_file(qasm_file) |
| 6 | program2 = circuit2.parse() | * | Deprecation -> qiskit.qasm.Qasm parse method deprecated | qiskit.qasm.Qasm | # removed |
| 7 | qc2 = program2.get_circuit() | * | Deprecation -> qiskit.qasm.Qasm get_circuit method deprecated | qiskit.qasm.Qasm | # removed |