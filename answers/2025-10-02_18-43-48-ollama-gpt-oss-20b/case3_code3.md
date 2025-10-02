| Line | Code | Scenario ID | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
| 2 | `from qiskit import qasm2 as qasm` | 5fc9 | DEPRECATION - The `qiskit.qasm` module, aliased as `qasm2` in this import, is deprecated. | `qiskit.qasm` | |
| 11 | `parsed_circuit = qasm.loads(qasm_str)` | 5fc9 | DEPRECATION - `qiskit.qasm.loads` is deprecated. Use `QuantumCircuit.from_qasm_str()` for parsing. | `qiskit.qasm.loads` | `parsed_circuit = QuantumCircuit.from_qasm_str(qasm_str)` |