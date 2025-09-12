| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
| 2 | from qiskit.extensions import HGate, XGate, Initialize | * | Deprecation -> HGate moved to circuit library | HGate | Replace with `from qiskit.circuit.library import HGate` |
| 2 | from qiskit.extensions import HGate, XGate, Initialize | * | Deprecation -> XGate moved to circuit library | XGate | Replace with `from qiskit.circuit.library import XGate` |
| 2 | from qiskit.extensions import HGate, XGate, Initialize | * | Deprecation -> Initialize moved to circuit library | Initialize | Replace with `from qiskit.circuit.library import Initialize` |
| 3 | from qiskit.extensions import Barrier | * | Deprecation -> Barrier moved to qiskit.circuit | Barrier | Replace with `from qiskit.circuit import Barrier` |
| 4 | from qiskit.extensions import UnitaryGate | * | Deprecation -> UnitaryGate moved to circuit library | UnitaryGate | Replace with `from qiskit.circuit.library import UnitaryGate` |
| 10 | qc.append(HGate(), [qr[0]]) | * | Deprecation -> use native h method | HGate | Replace with `qc.h(qr[0])` |
| 11 | qc.append(XGate(), [qr[1]]) | * | Deprecation -> use native x method | XGate | Replace with `qc.x(qr[1])` |
| 14 | custom_gate = UnitaryGate(custom_matrix, label="Custom") | * | Deprecation -> UnitaryGate moved to circuit library | UnitaryGate | No change needed after import adjustment |
| 18 | init_gate = Initialize(psi) | * | Deprecation -> use native initialize method | Initialize | Replace with `qc.initialize(psi, [qr[0]])` |
| 21 | qc.append(Barrier(3), [qr[0], qr[1], qr[2]]) | * | Deprecation -> use native barrier method | Barrier | Replace with `qc.barrier([qr[0], qr[1], qr[2]])` |