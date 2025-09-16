| Line | Code | Scenario ID | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
| 15 | `simulator = getBackend.get_backend('statevector_simulator')` | e012 | Migration of the deprecated statevector simulator to `Statevector` in `qiskit.quantum_info`. | `statevector_simulator` | ```python<br>from qiskit.quantum_info import Statevector<br>statevector = Statevector(qc)``` |
| 19 | `backend = getBackend.get_backend('qasm_simulator')` | b185 | Migration of the deprecated qasm simulator to `BasicProvider`/`BasicSimulator`. | `qasm_simulator` | ```python<br>from qiskit.providers.basic_provider import BasicProvider<br>provider = BasicProvider()<br>backend = provider.get_backend('basic_simulator')``` |
