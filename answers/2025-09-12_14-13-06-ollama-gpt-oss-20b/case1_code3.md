| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
| 3 | `from qiskit import QuantumCircuit, execute, Aer, qasm` | * | Deprecation -> qasm import removed | qasm | `from qiskit import QuantumCircuit, execute, Aer` |
| 13 | `backend = Aer.get_backend('aer_simulator')` | * | Deprecation -> backend name changed | Aer.get_backend | `backend = Aer.get_backend('qasm_simulator')` |