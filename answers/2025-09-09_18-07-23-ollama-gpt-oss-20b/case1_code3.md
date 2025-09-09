| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
| 3 | `from qiskit import QuantumCircuit, execute, Aer, qasm` | * | ImportError -> `qasm` import removed (optional) | qasm | `from qiskit import QuantumCircuit, execute, Aer` |