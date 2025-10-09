| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
|---|---|---|---|---|---|
| 9 | from qiskit import Aer | AER-DEPRECATION | Deprecation -> `qiskit.Aer` module is deprecated. Import `AerSimulator` from `qiskit_aer` instead. | `qiskit.Aer` | from qiskit_aer import AerSimulator |
| 10 | backend = Aer.get_backend('aer_simulator') | AER-DEPRECATION | Deprecation -> `Aer.get_backend()` method is deprecated. Instantiate `AerSimulator` directly. | `Aer.get_backend` | backend = AerSimulator() |