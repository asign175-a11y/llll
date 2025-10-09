| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| ----- | ----- | ----- | ----- | ----- | ----- |
| 1 | `from qiskit import qasm` | * | Deprecation -> The `qiskit.qasm` module is deprecated. Use `QuantumCircuit.from_qasm_str` from `qiskit.circuit`. | `qiskit.qasm` | `from qiskit.circuit import QuantumCircuit` |
| 12 | `circuit1 = qasm.Qasm(data=qasm_str)` | * | Deprecation -> The `qiskit.qasm.Qasm` class is deprecated. Use `QuantumCircuit.from_qasm_str` to parse QASM strings. | `qasm.Qasm` | `qc1 = QuantumCircuit.from_qasm_str(qasm_str)` |
| 13 | `program1 = circuit1.parse()` | * | Deprecation -> The `parse()` method is deprecated as part of the `qiskit.qasm` module removal. | `circuit1.parse()` | |
| 14 | `qc1 = program1.get_circuit()` | * | Deprecation -> The `get_circuit()` method is deprecated as part of the `qiskit.qasm` module removal. | `program1.get_circuit()` | |