| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
|---|---|---|---|---|---|
| 4 | `from qiskit.qasm import Qasm` | `*` | Deprecation -> The `qiskit.qasm` module is deprecated. (optional) | `qiskit.qasm.Qasm` | |
| 5 | `from qiskit.algorithms import VQE` | `qiskit.algorithms.VQE-1` | Deprecation -> `VQE` has moved from `qiskit.algorithms` to `qiskit.algorithms.minimum_eigensolvers`. | `qiskit.algorithms.VQE` | `from qiskit.algorithms.minimum_eigensolvers import VQE` |