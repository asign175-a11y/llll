| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| ----- | ----- | ----- | ----- | ----- | ----- |
| 11 | `from qiskit import execute` | * | Deprecation -> The `execute` function is deprecated. | `execute` function | |
| 12 | `job = execute(qc, backend, shots=1000)` | * | Deprecation -> The `execute` function is deprecated and should be replaced by `backend.run()`. | `execute` function | `job = backend.run(qc, shots=1000)` |
| 17 | `from qiskit.algorithms import VQE` | * | Module relocation -> `VQE` has been relocated from `qiskit.algorithms` to `qiskit.algorithms.minimum_eigensolvers`. | `VQE` class | `from qiskit.algorithms.minimum_eigensolvers import VQE` |
| 19 | `from qiskit import SPSA` | * | Module relocation -> `SPSA` has been relocated from `qiskit` to `qiskit.algorithms.optimizers`. | `SPSA` class | `from qiskit.algorithms.optimizers import SPSA` |