| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
|:--:|:---|:---------:|:-------|:-------|:----------|
| 2 | `from qiskit.extensions import HGate, XGate, Initialize` | * | Deprecation -> qiskit.extensions import for HGate | qiskit.extensions.HGate | `from qiskit.circuit.library.standard_gates import HGate` |
| 2 | `from qiskit.extensions import HGate, XGate, Initialize` | * | Deprecation -> qiskit.extensions import for XGate | qiskit.extensions.XGate | `from qiskit.circuit.library.standard_gates import XGate` |
| 2 | `from qiskit.extensions import HGate, XGate, Initialize` | * | Deprecation -> qiskit.extensions import for Initialize | qiskit.extensions.Initialize | `from qiskit.circuit.library.initialize import Initialize` |
| 3 | `from qiskit.extensions import Barrier` | * | Deprecation -> qiskit.extensions import for Barrier | qiskit.extensions.Barrier | `from qiskit.circuit.barrier import Barrier` |
| 4 | `from qiskit.extensions import UnitaryGate` | * | Deprecation -> qiskit.extensions import for UnitaryGate | qiskit.extensions.UnitaryGate | `from qiskit.circuit.library import UnitaryGate` |
| 21 | `qc.append(Barrier(3), [qr[0], qr[1], qr[2]])` | * | Optional -> replace Barrier usage with qc.barrier | qiskit.circuit.Barrier | `qc.barrier(qr)` |