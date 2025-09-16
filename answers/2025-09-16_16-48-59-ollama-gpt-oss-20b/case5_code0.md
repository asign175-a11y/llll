| Line | Code | Scenario ID | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
| 1 | `from qiskit.extensions import HGate, XGate, Initialize` | 4747 | The qiskit.extensions module is deprecated; objects moved to qiskit.circuit.library. | `qiskit.extensions.HGate`, `qiskit.extensions.XGate`, `qiskit.extensions.Initialize` |  |
| 2 | `from qiskit.extensions import Barrier` | 4747 | The qiskit.extensions module is deprecated; objects moved to qiskit.circuit.library. | `qiskit.extensions.Barrier` |  |
| 3 | `from qiskit.extensions import UnitaryGate` | 4747 | The qiskit.extensions module is deprecated; objects moved to qiskit.circuit.library. | `qiskit.extensions.UnitaryGate` |  |
| 4 | `init_gate = Initialize(psi)` | 4747 | The qiskit.extensions module is deprecated; objects moved to qiskit.circuit.library. | `qiskit.extensions.Initialize` |  |
| 5 | `custom_gate = UnitaryGate(custom_matrix, label="Custom")` | 4747 | The qiskit.extensions module is deprecated; objects moved to qiskit.circuit.library. | `qiskit.extensions.UnitaryGate` |  |