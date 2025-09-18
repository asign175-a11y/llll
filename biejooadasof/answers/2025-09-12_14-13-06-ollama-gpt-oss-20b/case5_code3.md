| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
|:----:|------|:-----------:|----------|----------|------------|
| 2 | from qiskit.extensions import UnitaryGate | * | Deprecation -> UnitaryGate moved from qiskit.extensions to qiskit.circuit.library | qiskit.extensions.UnitaryGate | from qiskit.circuit.library import UnitaryGate |
| 3 | from qiskit.extensions.exceptions import ExtensionError | * | Deprecation -> ExtensionError moved to qiskit.exceptions | qiskit.extensions.exceptions.ExtensionError | from qiskit.exceptions import QiskitError |
| 9 | raise ExtensionError("La matriz debe ser cuadrada") | * | Deprecation -> raise QiskitError instead of ExtensionError | ExtensionError | raise QiskitError("La matriz debe ser cuadrada") |
| 14 | except ExtensionError as e: | * | Deprecation -> catch QiskitError instead of ExtensionError | ExtensionError | except QiskitError as e: |