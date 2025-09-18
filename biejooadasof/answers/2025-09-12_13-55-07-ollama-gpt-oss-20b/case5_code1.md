| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
| 4 | `from qiskit import extensions as ext` | * | Deprecation -> extensions module removed in 0.46 | extensions module | Remove this import line (the `extensions` module is no longer available in 0.46) |
| 19 | `qc.prepare_state(psi, [qr[0]])` | * | Deletion -> `qc.prepare_state` removed in 0.46 | `prepare_state` method | `qc.initialize(psi, [qr[0]])` |
| 21 | `qc.append(ext.Barrier(3), [qr[0], qr[1], qr[2]])` | * | Deletion -> `ext.Barrier` removed in 0.46 | Barrier gate from `extensions` | `qc.barrier([qr[0], qr[1], qr[2]])` |