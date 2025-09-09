| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :-: | :- | :-: | :- | :- | :- |
| 10 | `from qiskit import Aer` | * | Deprecation -> qiskit.Aer object deprecated (optional) | qiskit.Aer | `from qiskit_aer import Aer` |
| 11 | `backend = Aer.get_backend('aer_simulator')` | * | Deprecation -> Aer.get_backend usage deprecated (optional) | qiskit.Aer | Keep the same line after updating the import to `qiskit_aer` |