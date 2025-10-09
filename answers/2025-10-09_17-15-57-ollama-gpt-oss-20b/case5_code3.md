| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| ----- | ----- | ----- | ----- | ----- | ----- |
| 2 | `from qiskit.extensions import UnitaryGate` | * | Deprecation -> The `UnitaryGate` class has moved. | `UnitaryGate` | `from qiskit.circuit.library import UnitaryGate` |
| 3 | `from qiskit.extensions.exceptions import ExtensionError` | * | Deprecation -> The `ExtensionError` class has been replaced. | `ExtensionError` | `from qiskit.exceptions import QiskitError` |
| 8 | `raise ExtensionError("La matriz debe ser cuadrada")` | * | Refactor -> Use the updated exception class. | `ExtensionError` | `raise QiskitError("La matriz debe ser cuadrada")` |
| 11 | `except ExtensionError as e:` | * | Refactor -> Catch the updated exception class. | `ExtensionError` | `except QiskitError as e:` |