```markdown
| Line | Code | Scenario ID | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
| 21 | `qc.append(ext.Barrier(3), [qr[0], qr[1], qr[2]])` | 4747 | DEPRECATION - qiskit.extensions module deprecated; objects moved to qiskit.circuit.library. | qiskit.extensions.Barrier | `from qiskit.circuit.library import Barrier`<br>`qc.append(Barrier(3), [qr[0], qr[1], qr[2]])` |
```