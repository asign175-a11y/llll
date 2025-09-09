| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :-: | :- | :-: | :- | :- | :- |
| 2 | `from qiskit.extensions import HGate, XGate, Initialize` | * | * | HGate | `from qiskit.circuit.library import HGate` |
| 2 | `from qiskit.extensions import HGate, XGate, Initialize` | * | * | XGate | `from qiskit.circuit.library import XGate` |
| 2 | `from qiskit.extensions import HGate, XGate, Initialize` | * | * | Initialize | `from qiskit.circuit.library import Initialize` |
| 3 | `from qiskit.extensions import Barrier` | * | * | Barrier | `from qiskit.circuit.library import Barrier` |
| 4 | `from qiskit.extensions import UnitaryGate` | * | * | UnitaryGate | `from qiskit.circuit.library import UnitaryGate` |
| 21 | `qc.append(Barrier(3), [qr[0], qr[1], qr[2]])` | * | * | Barrier gate | `qc.barrier([qr[0], qr[1], qr[2]])` |
| 18 | `init_gate = Initialize(psi)` | * | * | Initialize gate | `qc.initialize(psi, qr[0])`