| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
| 3 | `from qiskit.primitives import BackendEstimator` | * | Deprecation -> BackendEstimator import removed | BackendEstimator | `from qiskit.primitives import Estimator` |
| 15 | `estimator = BackendEstimator(` | * | Deprecation -> BackendEstimator instantiation removed | BackendEstimator | `estimator = Estimator(backend=backend, options={"shots": 1024})` |
| 21 | `job = estimator.run([psi1], [H1], [theta1])` | * | Estimator.run returns result directly | Estimator.run | `result = estimator.run([psi1], [H1], [theta1])` |
| 22 | `result = job.result()` | * | Job.result() on Estimator result is invalid | Job.result() |  |

