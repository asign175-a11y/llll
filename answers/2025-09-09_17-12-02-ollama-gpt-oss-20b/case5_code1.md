| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :-: | :- | :-: | :- | :- | :- |
| 4 | `from qiskit import extensions as ext` | * | Deprecation -> qiskit.extensions module deprecated | qiskit.extensions | # import removed; use `qc.barrier()` instead |
| 19 | `qc.prepare_state(psi, [qr[0]])` | * | Deprecation -> QuantumCircuit.prepare_state() function deprecated (optional) | QuantumCircuit.prepare_state | `qc.initialize(psi, [qr[0]])` |
| 21 | `qc.append(ext.Barrier(3), [qr[0], qr[1], qr[2]])` | * | Deprecation -> Barrier() class deprecated; use QuantumCircuit.barrier() (optional) | Barrier | `qc.barrier(qr[0], qr[1], qr[2])` |