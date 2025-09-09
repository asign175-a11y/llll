| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :-: | :- | :-: | :- | :- | :- |
| 3 | `from qiskit.primitives import BackendEstimator` | * | Deprecation -> BackendEstimator class removed; use Estimator | qiskit.primitives.BackendEstimator | `from qiskit.primitives import Estimator` |
| 15 | `estimator = BackendEstimator(` | * | Deprecation -> BackendEstimator class removed; use Estimator | qiskit.primitives.BackendEstimator | `estimator = Estimator(` |