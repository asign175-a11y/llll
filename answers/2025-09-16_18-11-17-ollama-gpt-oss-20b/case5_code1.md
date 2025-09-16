| Line | Code | Scenario ID | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
| 4 | `from qiskit import extensions as ext` | a747 | qiskit.extensions module deprecated | qiskit.extensions | `from qiskit.circuit.library import Barrier` |
| 21 | `qc.append(ext.Barrier(3), [qr[0], qr[1], qr[2]])` | a747 | qiskit.extensions module deprecated | qiskit.extensions | `qc.append(Barrier(3), [qr[0], qr[1], qr[2]])` |