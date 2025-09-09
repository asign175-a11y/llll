| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :-: | :- | :-: | :- | :- | :- |
| 2 | `from qiskit.extensions import HGate, XGate, Initialize` | \* | Deprecation -> from qiskit.extensions import HGate, XGate, Initialize deprecated (optional) | qiskit.extensions | `from qiskit.circuit.library import HGate, XGate, Initialize` |
| 3 | `from qiskit.extensions import Barrier` | \* | Deprecation -> from qiskit.extensions import Barrier deprecated (optional) | qiskit.extensions | `from qiskit.circuit import Barrier` |
| 4 | `from qiskit.extensions import UnitaryGate` | \* | Deprecation -> from qiskit.extensions import UnitaryGate deprecated (optional) | qiskit.extensions | `from qiskit.circuit.library import UnitaryGate` |