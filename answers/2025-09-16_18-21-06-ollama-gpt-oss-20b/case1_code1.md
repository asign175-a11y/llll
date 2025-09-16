| Line | Code | Scenario ID | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
| 3 | `from qiskit import Aer` | 4185 | DEPRECATION - The qiskit.providers.basicaer module and its classes are deprecated from Qiskit 0.46 onwards. | `qiskit.providers.basicaer` | `from qiskit.providers.basic_provider import BasicSimulator` |