| Line | Code | Scenario ID | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
| 7 | `from qiskit import Aer` | 1b49 | Importing from `qiskit.providers.aer` is deprecated and will stop working in Qiskit 1.0. Use `qiskit_aer` instead. | `qiskit.providers.aer.Aer` | `from qiskit_aer import AerSimulator` |
| 8 | `backend = Aer.get_backend('aer_simulator')` | 1b49 | Importing from `qiskit.providers.aer` is deprecated and will stop working in Qiskit 1.0. Use `qiskit_aer` instead. | `Aer.get_backend` | `backend = AerSimulator()` |