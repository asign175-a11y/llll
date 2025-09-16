| Line | Code | Scenario ID | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
| 3 | `from qiskit import Aer # type: ignore` | b185 | The qiskit.providers.basicaer module and its classes are deprecated from Qiskit 0.46 onwards. | qiskit.providers.basicaer | `from qiskit.providers.basic_provider import BasicProvider\nprovider = BasicProvider()\nbackend = provider.get_backend('qasm_simulator')` |

