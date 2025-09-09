| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :-: | :- | :-: | :- | :- | :- |
| 1 | `from qiskit import transpile, pulse` | * | Deprecation -> import qiskit.pulse from top-level qiskit deprecated (optional) | qiskit.pulse | `from qiskit import transpile`<br>`import qiskit.pulse as pulse` |