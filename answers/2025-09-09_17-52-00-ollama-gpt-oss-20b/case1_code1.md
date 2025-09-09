| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :-: | :- | :-: | :- | :- | :- |
| 3 | `from qiskit import Aer              # type: ignore` | * | Deprecation -> Aer import from qiskit is deprecated (optional) | qiskit.Aer | `from qiskit_aer import Aer` |
| 4 | `from qiskit import qasm             # type: ignore` | * | Deprecation -> qiskit.qasm import is deprecated (optional) | qiskit.qasm | * |