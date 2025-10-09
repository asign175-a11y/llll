| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
|---|---|---|---|---|---|
| 2 | `from qiskit.extensions import HGate, XGate, Initialize` | * | Deprecation -> Importing `HGate` from `qiskit.extensions` is deprecated. | `HGate` | `from qiskit.circuit.library import HGate` |
| 2 | `from qiskit.extensions import HGate, XGate, Initialize` | * | Deprecation -> Importing `XGate` from `qiskit.extensions` is deprecated. | `XGate` | `from qiskit.circuit.library import XGate` |
| 2 | `from qiskit.extensions import HGate, XGate, Initialize` | * | Deprecation -> Importing `Initialize` from `qiskit.extensions` is deprecated. | `Initialize` | `from qiskit.circuit.library import Initialize` |
| 3 | `from qiskit.extensions import Barrier` | * | Deprecation -> Importing `Barrier` from `qiskit.extensions` is deprecated. | `Barrier` | `from qiskit.circuit.library import Barrier` |
| 4 | `from qiskit.extensions import UnitaryGate` | * | Deprecation -> Importing `UnitaryGate` from `qiskit.extensions` is deprecated. | `UnitaryGate` | `from qiskit.circuit.library import UnitaryGate` |
| 10 | `qc.append(HGate(), [qr[0]])` | * | Usage Pattern (optional) -> Direct application of `HGate` as a method is preferred. | `HGate()` | `qc.h(qr[0])` |
| 11 | `qc.append(XGate(), [qr[1]])` | * | Usage Pattern (optional) -> Direct application of `XGate` as a method is preferred. | `XGate()` | `qc.x(qr[1])` |
| 19 | `qc.append(init_gate, [qr[0]])` | * | Usage Pattern (optional) -> Direct application of `initialize` as a method is preferred. | `init_gate` (`Initialize`) | `qc.initialize(psi, [qr[0]])` |
| 21 | `qc.append(Barrier(3), [qr[0], qr[1], qr[2]])` | * | Deprecation -> Usage of `Barrier` class for appending is deprecated; use `qc.barrier()` method. | `Barrier(3)` | `qc.barrier(qr[0], qr[1], qr[2])` |