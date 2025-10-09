| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| ----- | ----- | ----- | ----- | ----- | ----- |
| 1 | `from qiskit import qasm` | qiskit.qasm_2 | Deprecation -> The `qiskit.qasm` module has been deprecated | `qiskit.qasm` | |
| 7 | `circuit1 = qasm.Qasm(data=qasm_str)` | qiskit.qasm.Qasm | Deprecation -> The `Qasm` class has been deprecated | `qasm.Qasm` | `circuit1 = QuantumCircuit.from_qasm_str(qasm_str)` |
| 8 | `program1 = circuit1.parse()` | * | Deprecation -> The `parse()` method on the deprecated `Qasm` object is no longer available. | `parse()` | |
| 9 | `qc1 = program1.get_circuit()` | * | Deprecation -> The `get_circuit()` method on the object returned by the deprecated `parse()` method is no longer available. | `get_circuit()` | |