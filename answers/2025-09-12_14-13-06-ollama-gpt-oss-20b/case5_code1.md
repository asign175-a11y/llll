| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
| 4 | from qiskit import extensions as ext | * | Deprecation -> qiskit.extensions module deprecated | qiskit.extensions | Replace with: `from qiskit.circuit.library import Barrier` |
| 19 | qc.prepare_state(psi, [qr[0]]) | * | Deprecation -> prepare_state() deprecated | prepare_state | Replace with: `qc.initialize(psi, [qr[0]])` |
| 21 | qc.append(ext.Barrier(3), [qr[0], qr[1], qr[2]]) | * | Deprecation -> ext.Barrier() deprecated | ext.Barrier | Replace with: `qc.append(Barrier(3), [qr[0], qr[1], qr[2]])` |