| Line | Code | Scenario ID | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
| 1 | from qiskit import qasm | 5fc9 | The `qiskit.qasm` module (legacy OpenQASM 2 parser) has been deprecated, and its functionalities for parsing OpenQASM 2 strings are replaced by `QuantumCircuit.from_qasm_str()`. | qiskit.qasm | from qiskit.circuit import QuantumCircuit |
| 12 | circuit1 = qasm.Qasm(data=qasm_str) | 5fc9 | The `qiskit.qasm.Qasm` constructor is deprecated as part of the legacy OpenQASM 2 parser. Use `QuantumCircuit.from_qasm_str()` instead. | qiskit.qasm.Qasm | qc1 = QuantumCircuit.from_qasm_str(qasm_str) |
| 13 | program1 = circuit1.parse() | 5fc9 | The `parse()` method of the deprecated `qiskit.qasm.Qasm` object is no longer used. | circuit1.parse() | |
| 14 | qc1 = program1.get_circuit() | 5fc9 | The `get_circuit()` method of the result of the deprecated `qiskit.qasm` parsing is no longer used. | program1.get_circuit() | |