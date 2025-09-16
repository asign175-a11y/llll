| Line | Code | Scenario ID | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
| 15 | `simulator = getBackend.get_backend('statevector_simulator')` | e012 | Migrate statevector simulator to Statevector class | statevector simulator | `from qiskit.quantum_info import Statevector; statevector = Statevector(qc)` |
| 19 | `backend = getBackend.get_backend('qasm_simulator')` | b185 | Replace qasm simulator with BasicSimulator | qasm simulator | `from qiskit.providers.basic_provider import BasicSimulator; backend = BasicSimulator()` |