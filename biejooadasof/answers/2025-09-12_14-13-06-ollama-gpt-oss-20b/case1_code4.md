| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
| 10 | from qiskit import Aer | * | Deprecation -> import Aer deprecated | Aer module | from qiskit.providers.aer import AerSimulator |
| 11 | backend = Aer.get_backend('aer_simulator') | * | Deprecation -> Aer.get_backend deprecated | AerSimulator | backend = AerSimulator() |