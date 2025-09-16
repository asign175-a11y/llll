| Line | Code | Scenario ID | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
| 1 | `from qiskit import QuantumCircuit, Aer, execute` | 1b49 | Importing from qiskit.providers.aer is deprecated; use qiskit_aer instead. | `qiskit.providers.aer` | `from qiskit_aer import Aer` |
| 19 | `simulator = Aer.get_backend('statevector_simulator')` | 9012 | Statevector simulator migration: replace BasicAer backend with Statevector class. | `statevector_simulator` | `from qiskit.quantum_info import Statevector`<br>`statevector = Statevector(qc)` |