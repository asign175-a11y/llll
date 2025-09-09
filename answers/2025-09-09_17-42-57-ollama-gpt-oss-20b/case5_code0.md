| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :-: | :- | :-: | :- | :- | :- |
| 2 | `from qiskit.extensions import HGate, XGate, Initialize` | * | Deprecation -> HGate deprecated | HGate | `from qiskit.circuit.library import HGate` |
| 2 | `from qiskit.extensions import HGate, XGate, Initialize` | * | Deprecation -> XGate deprecated | XGate | `from qiskit.circuit.library import XGate` |
| 2 | `from qiskit.extensions import HGate, XGate, Initialize` | * | Deprecation -> Initialize deprecated | Initialize | `from qiskit.circuit.library import Initialize` |
| 3 | `from qiskit.extensions import Barrier` | * | Deprecation -> Barrier deprecated | Barrier | `from qiskit.circuit import Barrier` |
| 4 | `from qiskit.extensions import UnitaryGate` | * | Deprecation -> UnitaryGate deprecated | UnitaryGate | `from qiskit.circuit.library import UnitaryGate`