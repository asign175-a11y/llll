| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :-: | :- | :-: | :- | :- | :- |
| 2 | `from qiskit.quantum_info import Pauli, state_fidelity` | * | Deprecation -> state_fidelity() function deprecated (optional) | state_fidelity | `from qiskit.quantum_info.states.utils import state_fidelity` |
| 17 | `qc.unitary(Operator(evolution_matrix), [0])` | * | Deprecation -> QuantumCircuit.unitary() method deprecated (optional) | QuantumCircuit.unitary | `qc.unitary(evolution_matrix, [0])` |