| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :-: | :- | :-: | :- | :- | :- |
| 4 | from qiskit import extensions as ext | * | Deprecation -> qiskit.extensions module deprecated | qiskit.extensions | from qiskit.circuit import Barrier |
| 21 | qc.append(ext.Barrier(3), [qr[0], qr[1], qr[2]]) | * | Deprecation -> ext.Barrier deprecated | qiskit.circuit.Barrier | qc.append(Barrier(3), [qr[0], qr[1], qr[2]]) |