| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :-: | :- | :-: | :- | :- | :- |
| 3 | `from qiskit import QuantumCircuit, qasm, execute` | * | Deprecation -> qiskit.qasm deprecated | qiskit.qasm | Remove `qasm` import |
| 3 | `from qiskit import QuantumCircuit, qasm, execute` | * | Deprecation -> qiskit.execute deprecated | qiskit.execute | `from qiskit.compiler import execute` |