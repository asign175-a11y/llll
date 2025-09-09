| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :-: | :- | :-: | :- | :- | :- |
| 4 | `from qiskit import extensions as ext` | * | Deprecation -> from qiskit import extensions module removed | qiskit.extensions | `from qiskit.circuit import Barrier` |
| 19 | `qc.prepare_state(psi, [qr[0]])` | * | Deprecation -> QuantumCircuit.prepare_state method removed | QuantumCircuit.prepare_state | `qc.initialize(psi, [qr[0]])` |
| 21 | `qc.append(ext.Barrier(3), [qr[0], qr[1], qr[2]])` | * | Deprecation -> ext.Barrier usage replaced with qc.barrier | qiskit.extensions.Barrier | `qc.barrier([qr[0], qr[1], qr[2]])` |