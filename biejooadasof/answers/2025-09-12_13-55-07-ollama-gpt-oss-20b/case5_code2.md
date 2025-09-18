| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
| 17 | `qc.unitary(Operator(evolution_matrix), [0])` | * | Deprecation -> unitary() method deprecated (optional) | QuantumCircuit.unitary | `qc.append(Operator(evolution_matrix), [0], [])` |