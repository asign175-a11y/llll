```markdown
| Line | Code | Scenario ID | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
| 15 | `simulator = getBackend.get_backend('statevector_simulator')` | e012 | Migration of statevector simulator to new BasicProvider. | `qiskit.providers.basic_provider.BasicProvider` | `from qiskit.providers.basic_provider import BasicProvider\nprovider = BasicProvider()\nbackend = provider.get_backend(\"basic_simulator\")` |
| 17 | `statevector = result.get_statevector()` | e012 | Use Statevector from qiskit.quantum_info. | `qiskit.quantum_info.Statevector` | `from qiskit.quantum_info import Statevector\nstatevector = Statevector(qc)` |
| 19 | `backend = getBackend.get_backend('qasm_simulator')` | e012 | Migration of qasm simulator to BasicProvider. | `qiskit.providers.basic_provider.BasicProvider` | `from qiskit.providers.basic_provider import BasicProvider\nprovider = BasicProvider()\nbackend = provider.get_backend(\"basic_simulator\")` |
| 20 | `job = execute(qc, backend, shots=1000)` | e012 | Execute job with new backend. | `qiskit.providers.basic_provider.BasicProvider` | Use the backend created via BasicProvider as above. |
```