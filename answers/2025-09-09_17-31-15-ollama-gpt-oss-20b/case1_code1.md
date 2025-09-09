| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :-: | :- | :-: | :- | :- | :- |
| 2 | `from qiskit import QuantumCircuit   # type: ignore` | 107 | Deprecation -> QuantumCircuit deprecated (optional) | qiskit.circuit.QuantumCircuit | `from qiskit.circuit import QuantumCircuit` |
| 3 | `from qiskit import Aer              # type: ignore` | 108 | Deprecation -> Aer module deprecated (optional) | qiskit.providers.aer.Aer | `from qiskit.providers.aer import Aer` |
| 4 | `from qiskit import qasm             # type: ignore` | * | Deprecation -> qasm module deprecated (optional) | qiskit.qasm |  |