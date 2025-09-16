| Line | Code | Scenario ID | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
| 2 | `from qiskit.extensions import UnitaryGate` | a747 | The qiskit.extensions module is deprecated and its objects, including UnitaryGate, have moved to qiskit.circuit.library. | `qiskit.extensions.UnaryGate` | `from qiskit.circuit.library import UnitaryGate` |