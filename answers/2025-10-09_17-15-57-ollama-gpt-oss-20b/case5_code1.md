| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| ----- | ----- | ----- | ----- | ----- | ----- |
| 4 | `from qiskit import extensions as ext` | `qiskit.extensions` removal | Deprecation -> The `qiskit.extensions` module is deprecated. | `qiskit.extensions` | `from qiskit.circuit.library import Barrier` |
| 15 | `qc.prepare_state(psi, [qr[0]])` | `QuantumCircuit.prepare_state` moved/removed | Deprecation -> The `prepare_state()` method is deprecated. | `QuantumCircuit.prepare_state` | `qc.initialize(psi, [qr[0]])` |
| 16 | `qc.append(ext.Barrier(3), [qr[0], qr[1], qr[2]])` | `qiskit.extensions` removal | Deprecation -> Usage of a class from the deprecated `qiskit.extensions` module. | `ext.Barrier` | `qc.append(Barrier(3), [qr[0], qr[1], qr[2]])` |