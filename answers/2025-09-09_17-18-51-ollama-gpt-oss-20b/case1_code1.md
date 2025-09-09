| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :-: | :- | :-: | :- | :- | :- |
| 3 | `from qiskit import Aer              # type: ignore` | * | Deprecation -> `qiskit.Aer` import deprecated | `qiskit.Aer` | `from qiskit_aer import Aer` |
| 4 | `from qiskit import qasm             # type: ignore` | * | Deprecation -> `qiskit.qasm` module removed | `qiskit.qasm` | Remove import or replace with appropriate parser from the new Qiskit version |