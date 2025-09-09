| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :-: | :- | :-: | :- | :- | :- |
| 4 | from qiskit.opflow import Z, I, X | * | Deprecation -> qiskit.opflow module deprecated (optional) | qiskit.opflow | from qiskit.opflow import PauliSumOp |
| 7 | hamiltonian = (Z ^ I) + (X ^ X) | * | Deprecation -> qiskit.opflow operators deprecated (optional) | qiskit.opflow | hamiltonian = PauliSumOp.from_list([('ZI', 1), ('XX', 1)]) |