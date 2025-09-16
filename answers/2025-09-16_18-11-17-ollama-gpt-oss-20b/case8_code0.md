```markdown
| Line | Code | Scenario ID | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
| 1 | `from qiskit import Aer` | 1b49 | Importing from qiskit.providers.aer is deprecated and will stop working in Qiskit 1.0. | qiskit.providers.aer | `from qiskit_aer import Aer` |
| 12 | `backend = Aer.get_backend('qasm_simulator')` | 0012 | Importing from qiskit.providers.basicaer is deprecated and will stop working in Qiskit 1.0. | qiskit.providers.basicaer | `from qiskit.providers.basic_provider import BasicProvider\nbackend = BasicProvider().get_backend('qasm_simulator')` |
```