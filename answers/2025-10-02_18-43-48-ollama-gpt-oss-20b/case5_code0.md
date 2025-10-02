| Line | Code | Scenario ID | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
| 2 | `from qiskit.extensions import HGate, XGate, Initialize` | a747 | The `qiskit.extensions` module is now deprecated. | `qiskit.extensions` | |
| 2 | `from qiskit.extensions import HGate, XGate, Initialize` | a747 | Most objects from the deprecated `qiskit.extensions` module have been moved to `qiskit.circuit.library`, including `Initialize`. | `qiskit.extensions.Initialize` | `from qiskit.circuit.library import Initialize` |
| 3 | `from qiskit.extensions import Barrier` | a747 | The `qiskit.extensions` module is now deprecated. | `qiskit.extensions` | |
| 4 | `from qiskit.extensions import UnitaryGate` | a747 | Most objects from the deprecated `qiskit.extensions` module have been moved to `qiskit.circuit.library`, including `UnitaryGate`. | `qiskit.extensions.UnitaryGate` | `from qiskit.circuit.library import UnitaryGate` |