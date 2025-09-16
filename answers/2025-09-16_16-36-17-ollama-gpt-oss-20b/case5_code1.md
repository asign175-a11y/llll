```markdown
| Line | Code | Scenario ID | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
| 20 | `qc.append(ext.Barrier(3), [qr[0], qr[1], qr[2]])` | 0747 | The qiskit.extensions module is now deprecated. | `qiskit.extensions` | `from qiskit.circuit.library import Barrier`<br>`qc.append(Barrier(3), [qr[0], qr[1], qr[2]])` |
```