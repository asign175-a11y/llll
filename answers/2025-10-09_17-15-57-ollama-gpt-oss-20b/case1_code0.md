| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| ----- | ----- | ----- | ----- | ----- | ----- |
| 4 | `from qiskit.qasm import Qasm` | `qiskit-terra-0.24.0-qasm-removal` | Deprecation -> The `qiskit.qasm` module and `Qasm` class have been removed. (optional) | `qiskit.qasm.Qasm` | Remove line |
| 5 | `from qiskit.algorithms import VQE` | `qiskit-algorithms-0.1.0-vqe-move` | Deprecation -> The `VQE` class has been moved to `qiskit.algorithms.minimum_eigensolvers`. | `qiskit.algorithms.VQE` | `from qiskit.algorithms.minimum_eigensolvers import VQE` |
| 6 | `from qiskit import qasm2 as qasm` | `*` | Removal -> The `qiskit.qasm2` module does not exist. | `qiskit.qasm2` | Remove line |