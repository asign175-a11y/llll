| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
|---|---|---|---|---|---|
| 3 | `from qiskit import Aer              # type type: ignore` | `*` | Deprecation -> The `Aer` module from `qiskit` is deprecated; use `qiskit_aer` components instead. (optional) | `Aer` | `from qiskit_aer import AerSimulator` |
| 4 | `from qiskit import qasm             # type: ignore` | `*` | Deprecation -> The `qasm` module from `qiskit` is deprecated and no longer directly importable. Its functionalities are now in `qiskit_aer`. (optional) | `qasm` | |