| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :-: | :- | :-: | :- | :- | :- |
| 2 | `from qiskit.extensions import HGate, XGate, Initialize` | * | Deprecation -> qiskit.extensions module deprecated | HGate | `from qiskit.circuit.library.standard_gates import HGate` |
| 2 | `from qiskit.extensions import HGate, XGate, Initialize` | * | Deprecation -> qiskit.extensions module deprecated | XGate | `from qiskit.circuit.library.standard_gates import XGate` |
| 2 | `from qiskit.extensions import HGate, XGate, Initialize` | * | Deprecation -> qiskit.extensions module deprecated | Initialize | `from qiskit.circuit.library import Initialize` |
| 3 | `from qiskit.extensions import Barrier` | * | Deprecation -> qiskit.extensions module deprecated | Barrier | `from qiskit.circuit import Barrier` |
| 4 | `from qiskit.extensions import UnitaryGate` | * | Deprecation -> qiskit.extensions module deprecated | UnitaryGate | `from qiskit.circuit.library import UnitaryGate` |
| 21 | `qc.append(Barrier(3), [qr[0], qr[1], qr[2]])` | * | Deprecation -> Barrier(3) usage deprecated | Barrier usage | `qc.barrier(qr)` |