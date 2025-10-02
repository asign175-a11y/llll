| Line | Code | Scenario ID | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
| 1 | `from qiskit.qasm import Qasm` | 25fc | The `qiskit.qasm` module has been deprecated and will be removed in Qiskit 1.0.0. | `qiskit.qasm.Qasm` | Use `QuantumCircuit.from_qasm_file()` or `QuantumCircuit.from_qasm_str()` |
| 4 | `circuit2 = Qasm(filename=qasm_file)` | 25fc | The `qiskit.qasm` module has been deprecated and will be removed in Qiskit 1.0.0. | `Qasm(filename=qasm_file)` | Use `QuantumCircuit.from_qasm_file(qasm_file)` |