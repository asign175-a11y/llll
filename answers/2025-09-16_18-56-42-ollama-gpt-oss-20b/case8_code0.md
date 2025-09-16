| Line | Code | Scenario ID | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
| 1 | `from qiskit import Aer` | 1b49 | DEPRECATION - Importing from qiskit.providers.aer is deprecated and will stop working in Qiskit 1.0. Use qiskit_aer. | `qiskit.providers.aer` | `from qiskit_aer import Aer` |
| 12 | `backend = Aer.get_backend('qasm_simulator')` | 1b49 | DEPRECATION - Importing from qiskit.providers.aer is deprecated and will stop working in Qiskit 1.0. Use qiskit_aer. | `qiskit.providers.aer` | `backend = Aer.get_backend('qasm_simulator')` |