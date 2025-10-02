| Line | Code | Scenario ID | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
| 3 | `from qiskit import QuantumCircuit, execute, Aer, qasm` | 1b49 | Importing `Aer` from `qiskit.providers.aer` is deprecated. You should instead import from `qiskit_aer`. | `Aer` | `from qiskit_aer import Aer` |
| 3 | `from qiskit import QuantumCircuit, execute, Aer, qasm` | 25fc | The `qiskit.qasm` module has been deprecated and its parser functionality removed. | `qiskit.qasm` | |
| 13 | `backend = Aer.get_backend('aer_simulator')` | b0b8 | Direct instantiation of simulator classes from `qiskit_aer` (like `AerSimulator`) is preferred over `Aer.get_backend()`. | `Aer.get_backend('aer_simulator')` | `backend = AerSimulator()` |