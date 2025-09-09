| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :-: | :- | :-: | :- | :- | :- |
| 2 | `from qiskit.extensions import HGate, XGate, Initialize` | * | Deprecation -> qiskit.extensions imports deprecated | qiskit.extensions | `from qiskit.circuit.library.standard_gates import HGate, XGate, Initialize` |
| 3 | `from qiskit.extensions import Barrier` | * | Deprecation -> qiskit.extensions imports deprecated | qiskit.extensions | `from qiskit.circuit.library.standard_gates import Barrier` |
| 4 | `from qiskit.extensions import UnitaryGate` | * | Deprecation -> qiskit.extensions imports deprecated | qiskit.extensions | `from qiskit.circuit.library.standard_gates import UnitaryGate` |
| 21 | `qc.append(Barrier(3), [qr[0], qr[1], qr[2]])` | * | Deprecated usage of Barrier via append | qiskit.circuit.Barrier | `qc.barrier(qr)` |