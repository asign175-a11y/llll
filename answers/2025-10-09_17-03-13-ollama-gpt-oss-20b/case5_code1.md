| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| ----- | ----- | ----- | ----- | ----- | ----- |
| 4 | from qiskit import extensions as ext | * | Deprecation -> The `qiskit.extensions` module is deprecated. (optional) | qiskit.extensions | |
| 19 | qc.prepare_state(psi, [qr[0]]) | * | Deprecation -> The `QuantumCircuit.prepare_state` method is deprecated. Use `QuantumCircuit.initialize` instead. | QuantumCircuit.prepare_state | qc.initialize(psi, [qr[0]]) |
| 21 | qc.append(ext.Barrier(3), [qr[0], qr[1], qr[2]]) | * | Relocation -> The `Barrier` instruction has moved to `qiskit.circuit.library`. | ext.Barrier | qc.append(Barrier(3), [qr[0], qr[1], qr[2]]) |