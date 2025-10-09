| Line | Code | Scenario ID | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
| 3 | from qiskit import QuantumCircuit, execute, Aer, qasm | 1b49 | DEPRECATION - Importing Aer from qiskit.providers.aer is deprecated. Use qiskit_aer instead. | qiskit.Aer | from qiskit_aer import Aer |
| 3 | from qiskit import QuantumCircuit, execute, Aer, qasm | 25fc | DEPRECATION - The qiskit.qasm module is deprecated. Its functionality has been moved to qiskit.qasm2 for OpenQASM 2 support. | qiskit.qasm | from qiskit import qasm2 |