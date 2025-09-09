| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :-: | :- | :-: | :- | :- | :- |
| 4 | `from qiskit.qasm import Qasm` | * | Deprecation -> qiskit.qasm.Qasm deprecated | qiskit.qasm.Qasm | Replace with `from qiskit.qasm2 import load_qasm_file` (or use `qiskit.qasm2.load_qasm_file`) to load QASM files.