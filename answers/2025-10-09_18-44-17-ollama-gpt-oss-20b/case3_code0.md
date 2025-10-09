| Line | Code | Scenario ID | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
| 1 | from qiskit import qasm | 25fc9 | The `qiskit.qasm` module, which contains the legacy OpenQASM 2 parser, is deprecated. | qiskit.qasm module | Remove import as functionality is now available via `QuantumCircuit.from_qasm_str()` |
| 11 | circuit1 = qasm.Qasm(data=qasm_str) | 25fc9 | The `qiskit.qasm.Qasm` class for parsing OpenQASM 2 strings is deprecated. | qiskit.qasm.Qasm | circuit1 = QuantumCircuit.from_qasm_str(qasm_str) |