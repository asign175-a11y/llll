| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :-: | :- | :-: | :- | :- | :- |
| 4 | `from qiskit import qasm             # type: ignore` | * | Deprecation -> qiskit.qasm module deprecated | qiskit.qasm | Remove this import. If you need to obtain QASM, use `qc.qasm()` on the circuit. |