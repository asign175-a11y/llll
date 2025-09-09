| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
|:-:|:-|:-:|:-|:-|:-|
| 2 | `from qiskit.opflow import PauliSumOp` | * | Deprecation -> PauliSumOp deprecated (optional) | qiskit.opflow.PauliSumOp | `from qiskit.opflow import PauliOp` |
| 3 | `from qiskit.primitives import BackendEstimator` | * | Deprecation -> BackendEstimator deprecated | qiskit.primitives.BackendEstimator | `from qiskit.primitives import Estimator` |
| 21 | `job = estimator.run([psi1], [H1], [theta1])` | * | Deprecation -> estimator.run signature changed | qiskit.primitives.Estimator.run | `job = estimator.run(quantum_circuits=[psi1], observables=[H1], parameter_values=[theta1])` |
| 22 | `result = job.result()` | * | Deprecation -> Job.result() usage | qiskit.primitives.Job.result | `result = job` |