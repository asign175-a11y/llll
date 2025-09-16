| Line | Code | Scenario ID | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
| 8 | `from qiskit import Aer` | 4185 | qiskit.providers.basicaer deprecated | qiskit.providers.basicaer.Aer | `from qiskit.providers.basic_provider import BasicProvider` |
| 9 | `backend = Aer.get_backend('aer_simulator')` | 4185 | qiskit.providers.basicaer deprecated | Aer.get_backend | `from qiskit.providers.basic_provider import BasicSimulator; backend = BasicSimulator()` |