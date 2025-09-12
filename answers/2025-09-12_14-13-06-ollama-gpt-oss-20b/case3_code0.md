| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
| 1 | from qiskit import qasm | * | Deprecation -> qiskit import qasm deprecated | qiskit import | from qiskit.qasm import Qasm |
| 13 | circuit1 = qasm.Qasm(data=qasm_str) | * | Usage -> qasm.Qasm usage replaced | qasm.Qasm | circuit1 = Qasm(data=qasm_str) |