| Line | Code | Scenario ID | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
| 1 | from qiskit import QuantumCircuit, Aer, execute | 061aaf2e-3a73-4bb9-a610-0cd2c7551b49 | DEPRECATION - Importing from qiskit.providers.aer is deprecated | qiskit.providers.aer | from qiskit_aer import Aer, QuantumCircuit, execute |