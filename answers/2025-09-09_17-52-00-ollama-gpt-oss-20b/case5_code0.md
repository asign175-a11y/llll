| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :-: | :- | :-: | :- | :- | :- |
| 2 | `from qiskit.extensions import HGate, XGate, Initialize` | * | Deprecation -> qiskit.extensions.HGate class deprecated | qiskit.extensions.HGate | `from qiskit.circuit.library import HGate` |
| 2 | `from qiskit.extensions import HGate, XGate, Initialize` | * | Deprecation -> qiskit.extensions.XGate class deprecated | qiskit.extensions.XGate | `from qiskit.circuit.library import XGate` |
| 2 | `from qiskit.extensions import HGate, XGate, Initialize` | * | Deprecation -> qiskit.extensions.Initialize class deprecated | qiskit.extensions.Initialize | `from qiskit.circuit.library import Initialize` |
| 3 | `from qiskit.extensions import Barrier` | * | Deprecation -> qiskit.extensions.Barrier class deprecated | qiskit.extensions.Barrier | `from qiskit.circuit import Barrier` |
| 4 | `from qiskit.extensions import UnitaryGate` | * | Deprecation -> qiskit.extensions.UnitaryGate class deprecated | qiskit.extensions.UnitaryGate | `from qiskit.circuit.library import UnitaryGate` |