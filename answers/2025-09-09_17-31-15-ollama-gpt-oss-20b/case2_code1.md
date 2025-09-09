| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :-: | :- | :-: | :- | :- | :- |
| 2 | `from qiskit.opflow import PauliSumOp` | * | Deprecation -> qiskit.opflow deprecated (optional) | qiskit.opflow | * |
| 3 | `from qiskit.primitives import BackendEstimator` | * | Deprecation -> qiskit.primitives.BackendEstimator deprecated (optional) | qiskit.primitives.BackendEstimator | `from qiskit.primitives import Estimator` |
| 15 | `estimator = BackendEstimator(` | * | Deprecation -> BackendEstimator constructor deprecated (optional) | qiskit.primitives.BackendEstimator | `estimator = Estimator(backend=backend, options={"shots": 1024})` |
| 21 | `job = estimator.run([psi1], [H1], [theta1])` | * | Deprecation -> BackendEstimator.run returns job (optional) | qiskit.primitives.BackendEstimator | `results = estimator.run([psi1], [H1], [theta1])` |
| 22 | `result = job.result()` | * | Deprecation -> job.result() on BackendEstimator run result (optional) | qiskit.primitives.BackendEstimator | `value = results[0].values[0]` |
| 24 | `print(f"Expectation value: {result.values[0]}")` | * | Usage of result.values after job.result() deprecated (optional) | qiskit.primitives.BackendEstimator | `print(f"Expectation value: {value}")` |