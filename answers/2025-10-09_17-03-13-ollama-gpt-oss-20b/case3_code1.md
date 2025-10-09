| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
|---|---|---|---|---|---|
| 1 | from qiskit.qasm import Qasm | * | Deprecation -> The `qiskit.qasm.Qasm` module and class are deprecated. | `qiskit.qasm.Qasm` | from qiskit.circuit import QuantumCircuit |
| 4 | circuit2 = Qasm(filename=qasm_file) | * | Deprecation -> Instantiating `qiskit.qasm.Qasm` is deprecated. Use `QuantumCircuit.from_qasm_file` instead. | `Qasm` constructor | qc2 = QuantumCircuit.from_qasm_file(qasm_file) |
| 5 | program2 = circuit2.parse() | * | Deprecation -> The `parse()` method of the `Qasm` object is deprecated and no longer needed. | `parse()` method | |
| 6 | qc2 = program2.get_circuit() | * | Deprecation -> The `get_circuit()` method of the parsed `Qasm` object is deprecated and no longer needed. | `get_circuit()` method | |