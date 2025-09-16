| Line | Code | Scenario ID | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
| 10 | `from qiskit import Aer` | 1b49 | Importing from qiskit.providers.aer is deprecated; use qiskit_aer instead. | `qiskit_aer.Aer` | `from qiskit_aer import Aer` |
| 11 | `backend = Aer.get_backend('aer_simulator')` | b185 | Replacement of Aer simulator with BasicSimulator. | `qiskit.providers.basic_provider.BasicSimulator` | `from qiskit.providers.basic_provider import BasicSimulator\nbackend = BasicSimulator()`