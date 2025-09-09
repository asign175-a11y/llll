| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :-: | :- | :-: | :- | :- | :- |
| 10 | `from qiskit import Aer` | * | Deprecation -> Aer module import | Aer | `from qiskit.providers.aer import AerSimulator` |
| 11 | `backend = Aer.get_backend('aer_simulator')` | * | Deprecation -> Aer.get_backend('aer_simulator') | Aer | `backend = AerSimulator()` |