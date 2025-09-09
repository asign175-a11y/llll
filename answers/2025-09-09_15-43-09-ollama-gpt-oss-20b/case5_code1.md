| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
|:-:|:-|:-:|:-|:-|:-|
| 4 | from qiskit import extensions as ext | * | Deprecation -> qiskit.extensions module removed | qiskit.extensions | Remove the import; use `qc.barrier()` or `from qiskit.circuit.library.standard_gates import Barrier` instead. |
| 19 | qc.prepare_state(psi, [qr[0]]) | * | Deprecation -> QuantumCircuit.prepare_state deprecated | QuantumCircuit.prepare_state | Replace with `qc.initialize(psi, qr[0])`. |
| 21 | qc.append(ext.Barrier(3), [qr[0], qr[1], qr[2]]) | * | Deprecation -> ext.Barrier usage replaced | qiskit.extensions.Barrier | Replace with `qc.barrier(qr)` (or `qc.barrier()` with no args). |