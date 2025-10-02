| Line | Code | Scenario ID | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
| 2 | `from qiskit.extensions import UnitaryGate` | a747 | The `qiskit.extensions` module is deprecated. `UnitaryGate` has moved to `qiskit.circuit.library`. | `qiskit.extensions.UnitaryGate` | `from qiskit.circuit.library import UnitaryGate` |
| 11 | `custom_gate = UnitaryGate(matrix)` | a747 | The `qiskit.extensions` module is deprecated. `UnitaryGate` has moved to `qiskit.circuit.library`. | `UnitaryGate` | |