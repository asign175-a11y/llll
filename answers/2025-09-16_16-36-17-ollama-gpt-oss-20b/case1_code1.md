| Line | Code | Scenario ID | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
| 1 | `import os` |  |  |  |  |
| 2 | `from qiskit import QuantumCircuit   # type: ignore` |  |  |  |  |
| 3 | `from qiskit import Aer              # type: ignore` | b185 | Deprecation of qiskit.providers.basicaer; use qiskit.providers.basic_provider | qiskit.providers.basicaer | `from qiskit.providers.basic_provider import BasicProvider` |