| Line | Code | Scenario ID | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
| 3 | `from qiskit import QuantumCircuit, execute, Aer, qasm` | 1b49 | Importing from `qiskit.providers.aer` is deprecated; use `qiskit_aer` instead. | `qiskit.Aer` | `from qiskit import QuantumCircuit, execute, qasm` |