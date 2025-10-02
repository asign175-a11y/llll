| Line | Code | Scenario ID | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
| 1 | `from qiskit import qasm` | 5fc9 | DEPRECATION - The `qiskit.qasm` module is deprecated. | `qiskit.qasm` | `from qiskit.circuit import QuantumCircuit` |
| 11 | `circuit1 = qasm.Qasm(data=qasm_str)` | 5fc9 | DEPRECATION - The `qiskit.qasm.Qasm` class for parsing OpenQASM 2 is deprecated. Use `QuantumCircuit.from_qasm_str()` instead. | `qiskit.qasm.Qasm` | `qc1 = QuantumCircuit.from_qasm_str(qasm_str)` |