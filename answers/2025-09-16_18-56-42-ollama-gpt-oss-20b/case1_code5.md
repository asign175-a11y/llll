| Line | Code | Scenario ID | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
| 8 | `from qiskit import Aer` | b49 | Importing from qiskit is deprecated; use qiskit_aer instead. | qiskit.providers.aer.Aer | `from qiskit_aer import AerSimulator` |
| 9 | `backend = Aer.get_backend('aer_simulator')` | b49 | Using Aer.get_backend is deprecated; use AerSimulator() instead. | qiskit_aer.AerSimulator | `backend = AerSimulator()` |