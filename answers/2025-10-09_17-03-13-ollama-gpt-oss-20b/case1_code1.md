| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
|---|---|---|---|---|---|
| 3 | `from qiskit import Aer # type: ignore` | QP046-AER-001 | Deprecation -> The `qiskit.Aer` module is deprecated. | `Aer` module | `from qiskit_aer import Aer` |
| 4 | `from qiskit import qasm # type: ignore` | QP046-QASM-002 | Removal -> The `qiskit.qasm` module has been removed. | `qasm` module | `from qiskit.qasm2 import QASM2Importer` |