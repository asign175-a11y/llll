| Line | Code | Scenario ID | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
| 1 | `from qiskit import Aer` | 1b49 | Importing from `qiskit.providers.aer` is deprecated and will stop working in Qiskit 1.0. You should instead import from `qiskit_aer`, which is a drop-in replacement. | `qiskit.providers.aer` | `from qiskit_aer import Aer` |