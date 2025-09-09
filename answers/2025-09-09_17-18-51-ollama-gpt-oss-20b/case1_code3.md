| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :-: | :- | :-: | :- | :- | :- |
| 3 | from qiskit import QuantumCircuit, execute, Aer, qasm | * | Deprecation -> qiskit.Aer object deprecated (optional) | qiskit.Aer | `from qiskit_aer import Aer` |
| 3 | from qiskit import QuantumCircuit, execute, Aer, qasm | * | Deprecation -> qiskit.qasm module deprecated (optional) | qiskit.qasm | `from qiskit import qasm2` |
| 13 | backend = Aer.get_backend('aer_simulator') | * | Deprecation -> qiskit.Aer object deprecated (optional) | qiskit.Aer | `backend = Aer.get_backend('aer_simulator')`  *(import updated to qiskit_aer)* |