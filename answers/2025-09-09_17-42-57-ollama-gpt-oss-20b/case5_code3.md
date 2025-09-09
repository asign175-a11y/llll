| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :-: | :- | :-: | :- | :- | :- |
| 2 | `from qiskit.extensions import UnitaryGate` | * | Deprecation -> qiskit.extensions UnitaryGate deprecated (optional) | qiskit.extensions | `from qiskit.circuit.library import UnitaryGate` |
| 3 | `from qiskit.extensions.exceptions import ExtensionError` | * | Deprecation -> qiskit.extensions.exceptions ExtensionError deprecated (optional) | qiskit.extensions.exceptions | `from qiskit.exceptions import ExtensionError` |