| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
|:--:|:---|:-----------:|:--------|:--------|:-----------|
| 2 | `from qiskit.opflow import PauliSumOp` | * | Deprecation -> PauliSumOp import deprecated | qiskit.opflow PauliSumOp import path | `from qiskit.opflow.operators import PauliSumOp` |
| 3 | `from qiskit.primitives import BackendEstimator` | * | Deprecation -> BackendEstimator deprecated | qiskit.primitives BackendEstimator | `from qiskit.primitives import Estimator` |
| 15 | `estimator = BackendEstimator(` | * | Deprecation -> BackendEstimator usage deprecated | qiskit.primitives Estimator instantiation | `estimator = Estimator(` |