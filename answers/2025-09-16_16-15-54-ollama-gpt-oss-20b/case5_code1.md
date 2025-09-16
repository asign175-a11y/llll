| Line | Code | Scenario ID | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
| 4 | `from qiskit import extensions as ext` | 5db8be17-41de-4bf7-8281-02232d40a747 | DEPRECATION - The qiskit.extensions module is deprecated | qiskit.extensions | `from qiskit.circuit.library import Barrier` |
| 21 | `qc.append(ext.Barrier(3), [qr[0], qr[1], qr[2]])` | 5db8be17-41de-4bf7-8281-02232d40a747 | DEPRECATION - The qiskit.extensions module is deprecated | qiskit.extensions | `qc.append(Barrier(3), [qr[0], qr[1], qr[2]])` |