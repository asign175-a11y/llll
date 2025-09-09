| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :-: | :- | :-: | :- | :- | :- |
| 1 | `from qiskit import QuantumCircuit, Aer, execute` | * | `Deprecation -> Aer provider import deprecated` | `Aer` | `from qiskit.providers.aer import AerSimulator` (remove `Aer` import) |
| 7 | `pauli_z = Pauli('Z').to_matrix()` | * | `Deprecation -> Pauli.to_matrix() deprecated` | `Pauli.to_matrix` | `pauli_z = Pauli('Z').to_numpy_array()` |
| 8 | `pauli_x = Pauli('X').to_matrix()` | * | `Deprecation -> Pauli.to_matrix() deprecated` | `Pauli.to_matrix` | `pauli_x = Pauli('X').to_numpy_array()` |
| 19 | `simulator = Aer.get_backend('statevector_simulator')` | * | `Deprecation -> Aer.get_backend() deprecated` | `Aer.get_backend` | `simulator = AerSimulator(method='statevector')` |
