| Line | Code | Scenario ID | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
| 13 | `backend = Aer.get_backend('aer_simulator')` | b185 | Deprecation of qiskit.providers.basicaer; use qiskit.providers.basic_provider | `qiskit.providers.basicaer` | `from qiskit.providers.basic_provider import BasicSimulator\nbackend = BasicSimulator()` |