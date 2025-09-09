| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :-: | :- | :-: | :- | :- | :- |
| 4 | from qiskit import extensions as ext | * | Deprecation -> qiskit.extensions module deprecated (optional) | qiskit.extensions | from qiskit.circuit import Barrier |
| 13 | qc.unitary(custom_matrix, [qr[2]], label="Custom") | * | Deprecation -> QuantumCircuit.unitary method deprecated (optional) | QuantumCircuit.unitary | from qiskit.circuit.library.standard_gates import UnitaryGate; qc.append(UnitaryGate(custom_matrix), [qr[2]]) |
| 16 | qc.append(ext.Barrier(3), [qr[0], qr[1], qr[2]]) | * | Deprecation -> qiskit.extensions.Barrier deprecated (optional) | qiskit.extensions.Barrier | qc.barrier([qr[0], qr[1], qr[2]]) |