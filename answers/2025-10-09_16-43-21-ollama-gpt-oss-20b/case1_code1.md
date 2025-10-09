| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| ----- | ----- | ----- | ----- | ----- | ----- |
| 3 | `from qiskit import Aer # type: ignore` | * | Deprecation -> The `Aer` backend should be imported from `qiskit_aer`. | `qiskit.Aer` | `from qiskit_aer import Aer` |
| 4 | `from qiskit import qasm # type: ignore` | * | Deprecation -> The `qiskit.qasm` module has been removed. | `qiskit.qasm` | |