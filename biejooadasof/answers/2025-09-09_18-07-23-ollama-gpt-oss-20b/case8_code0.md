```markdown
| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
| 1 | from qiskit import Aer | * | Deprecation -> qiskit Aer object is deprecated (optional) | qiskit Aer | from qiskit_aer import Aer |
| 9 | ansatz = TwoLocal(num_qubits, rotation_blocks='ry', entanglement_blocks='cz', reps=1) | * | Deprecation -> entanglement_blocks parameter is deprecated (optional) | TwoLocal.entanglement_blocks | ansatz = TwoLocal(num_qubits, rotation_blocks='ry', entanglement='cz', reps=1) |
```