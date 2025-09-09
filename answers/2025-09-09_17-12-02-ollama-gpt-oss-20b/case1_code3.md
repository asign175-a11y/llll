| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :-: | :- | :-: | :- | :- | :- |
| 3 | from qiskit import QuantumCircuit, execute, Aer, qasm | * | Deprecation -> qiskit.Aer object deprecated | qiskit.Aer | from qiskit_aer import Aer |
| 3 | from qiskit import QuantumCircuit, execute, Aer, qasm | * | Deprecation -> qiskit.qasm module deprecated | qiskit.qasm | from qiskit.qasm import read_qasm |
| 9 | backend = Aer.get_backend('aer_simulator') | * | Deprecation -> qiskit.Aer.get_backend usage deprecated | qiskit.Aer.get_backend | (no change required after import update) |