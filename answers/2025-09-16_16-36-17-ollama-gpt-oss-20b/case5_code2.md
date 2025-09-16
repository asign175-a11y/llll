| Line | Code | Scenario ID | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
| 19 | `simulator = Aer.get_backend('statevector_simulator')` | 0012 | Migrate from BasicAer statevector_simulator to Statevector class. | `qiskit.providers.basicaer` | `from qiskit.quantum_info import Statevector` |
| 20 | `result = execute(qc, simulator).result()` | 0012 | Replace execution with Statevector constructor. | `qiskit.providers.basicaer` | `statevector = Statevector(qc)` |
| 21 | `statevector = result.get_statevector()` | 0012 | Remove unnecessary result retrieval; use Statevector directly. | `qiskit.providers.basicaer` | `statevector = Statevector(qc)` |

