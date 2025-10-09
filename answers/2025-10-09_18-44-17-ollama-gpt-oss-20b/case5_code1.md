| Line | Code | Scenario ID | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
| 4 | from qiskit import extensions as ext | a747 | The qiskit.extensions module is now deprecated. Most objects have been moved to qiskit.circuit.library. | qiskit.extensions | |
| 19 | qc.append(ext.Barrier(3), [qr[0], qr[1], qr[2]]) | a747 | Usage of objects from the deprecated qiskit.extensions module. | ext.Barrier | |