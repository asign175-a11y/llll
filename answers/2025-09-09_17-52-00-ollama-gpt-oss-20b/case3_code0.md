| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :-: | :- | :-: | :- | :- | :- |
| 1 | `from qiskit import qasm` | * | Deprecation -> qiskit.qasm import deprecated (mandatory) | `qiskit.qasm` | `from qiskit.qasm.parser import QasmParser` |
| 5 | `circuit1 = qasm.Qasm(data=qasm_str)` | * | Deprecation -> qiskit.qasm.Qasm constructor deprecated (mandatory) | `qiskit.qasm.Qasm` | `circuit1 = QasmParser(data=qasm_str)` |