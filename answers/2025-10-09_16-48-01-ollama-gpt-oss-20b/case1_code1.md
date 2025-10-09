| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
|---|---|---|---|---|---|
| 3 | `from qiskit import Aer` | * | Deprecation -> The `Aer` module imported directly from `qiskit` is deprecated in favor of `qiskit_aer.AerSimulator`. | `Aer` module | `from qiskit_aer import AerSimulator` |
| 4 | `from qiskit import qasm` | * | Deprecation -> The `qiskit.qasm` module is deprecated. | `qasm` module | |