| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
| 10 | from qiskit import Aer | * | Import -> `Aer` deprecated | `Aer` | `from qiskit.providers.aer import AerSimulator` |
| 11 | backend = Aer.get_backend('aer_simulator') | * | Function -> `Aer.get_backend()` deprecated | `Aer.get_backend` | `backend = AerSimulator()` |