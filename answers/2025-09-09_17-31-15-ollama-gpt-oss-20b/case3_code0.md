| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :-: | :- | :-: | :- | :- | :- |
| 1 | `from qiskit import qasm` | * | Deprecation -> qiskit import qasm module deprecated | qiskit.qasm | `from qiskit.qasm.compiler import QasmParser` |
| 13 | `circuit1 = qasm.Qasm(data=qasm_str)` | * | Deprecation -> qasm.Qasm class deprecated | qiskit.qasm.Qasm | `parser = QasmParser(data=qasm_str)` |
| 14 | `program1 = circuit1.parse()` | * | Deprecation -> circuit1.parse() method deprecated | qiskit.qasm.Qasm | `qobj = parser.parse()` |
| 15 | `qc1 = program1.get_circuit()` | * | Deprecation -> program1.get_circuit() method deprecated | qiskit.qasm.Qasm | `qc1 = qobj.to_circuit()` |