| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
| 1 | `from qiskit import qasm` | * | Deprecation -> import qiskit.qasm is deprecated | qiskit.qasm | `from qiskit.qasm import parse_qasm` |
| 5 | `circuit1 = qasm.Qasm(data=qasm_str)` | * | Deprecation -> qiskit.qasm.Qasm class removed | qiskit.qasm.Qasm | `qc1 = parse_qasm(qasm_str)` |
| 6 | `program1 = circuit1.parse()` | * | Deprecation -> program1.parse() removed | program1.parse | *(remove line)* |
| 7 | `qc1 = program1.get_circuit()` | * | Deprecation -> program1.get_circuit() removed | program1.get_circuit | *(remove line)* |