| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :-: | :- | :-: | :- | :- | :- |
| 1 | `from qiskit import QuantumCircuit, Aer, execute` | * | Deprecation -> qiskit.Aer module deprecated (optional) | qiskit.Aer | `from qiskit_aer import Aer` |
| 2 | `from qiskit.quantum_info import Pauli, state_fidelity` | * | Deprecation -> state_fidelity moved to qiskit.quantum_info.states (optional) | qiskit.quantum_info.state_fidelity | `from qiskit.quantum_info.states import state_fidelity` |