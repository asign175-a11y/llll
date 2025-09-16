```markdown
| Line | Code | Scenario ID | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
| 13 | `job = estimator.run([psi1], [H1], [theta1])` | 8c20 | Using a PauliList as an observable that is implicitly converted to a SparsePauliOp with coefficients 1 when calling Estimator.run() is deprecated. Instead you should explicitly convert the argument using SparsePauliOp(pauli_list) first. | Estimator.run | `job = estimator.run([psi1], [SparsePauliOp(H1)], [theta1])` |
```