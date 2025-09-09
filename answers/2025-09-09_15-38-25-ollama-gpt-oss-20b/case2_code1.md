| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :-: | :- | :-: | :- | :- | :- |
| 3 | `from qiskit.primitives import BackendEstimator` | * | Deprecation -> qiskit.primitives BackendEstimator import path deprecated (optional) | qiskit.primitives.BackendEstimator | `from qiskit.primitives.estimators import BackendEstimator` |
| 17 | `options={"shots": 1024}  # Configurar shots aquí` | * | Deprecation -> BackendEstimator options keyword replaced with estimator_options (optional) | BackendEstimator.options | `estimator_options={"shots": 1024}` |