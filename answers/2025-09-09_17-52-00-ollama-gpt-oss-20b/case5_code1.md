| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :-: | :- | :-: | :- | :- | :- |
| 4 | `from qiskit import extensions as ext` | * | Deprecation -> extensions module removed | qiskit.extensions | Remove import; use `from qiskit.circuit import Barrier` and instantiate `Barrier` directly |
| 19 | `qc.prepare_state(psi, [qr[0]])` | * | Deprecation -> prepare_state deprecated in favor of initialize | QuantumCircuit.prepare_state | `qc.initialize(psi, [qr[0]])` |
| 21 | `qc.append(ext.Barrier(3), [qr[0], qr[1], qr[2]])` | * | Deprecation -> ext.Barrier deprecated; use qiskit.circuit.Barrier | Barrier | `from qiskit.circuit import Barrier` and `qc.append(Barrier(3), [qr[0], qr[1], qr[2]])` |