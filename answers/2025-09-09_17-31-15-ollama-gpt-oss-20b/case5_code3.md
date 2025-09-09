| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :-: | :- | :-: | :- | :- | :- |
| 2 | `from qiskit.extensions import UnitaryGate` | * | Deprecation -> from qiskit.extensions import UnitaryGate deprecated | qiskit.extensions.UnitaryGate | `from qiskit.circuit.library import UnitaryGate` |
| 3 | `from qiskit.extensions.exceptions import ExtensionError` | * | Deprecation -> from qiskit.extensions.exceptions import ExtensionError deprecated | qiskit.extensions.exceptions.ExtensionError | `from qiskit.circuit.exceptions import CircuitError` |
| 9 | `raise ExtensionError("La matriz debe ser cuadrada")` | * | Deprecation -> ExtensionError usage deprecated | qiskit.extensions.exceptions.ExtensionError | `raise ValueError("La matriz debe ser cuadrada")` |