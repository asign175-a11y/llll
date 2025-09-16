| Line | Code | Scenario ID | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
| 3 | `from qiskit import QuantumCircuit, execute, Aer, qasm` | b185 | The qiskit.providers.basicaer module and all of its classes are deprecated from Qiskit 0.46 onwards. Their use should be replaced with the qiskit.quantum_info module and the new qiskit.providers.basic_provider module. | `qiskit.providers.basicaer` | ```python
from qiskit.providers.basic_provider import BasicProvider
from qiskit import QuantumCircuit, execute, qasm
``` |
| 13 | `backend = Aer.get_backend('aer_simulator')` | b185 | The qiskit.providers.basicaer module and all of its classes are deprecated from Qiskit 0.46 onwards. Their use should be replaced with the qiskit.quantum_info module and the new qiskit.providers.basic_provider module. | `qiskit.providers.basicaer.BasicAer` | ```python
provider = BasicProvider()
backend = provider.get_backend('basic_simulator')
``` |