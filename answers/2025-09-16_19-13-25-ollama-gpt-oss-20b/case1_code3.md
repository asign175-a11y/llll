```markdown
| Line | Code | Scenario ID | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
| 3 | `from qiskit import QuantumCircuit, execute, Aer, qasm` | 4185 | Deprecation of qiskit.providers.basicaer module and its components. | `qiskit.providers.basicaer` | `from qiskit.providers.basic_provider import BasicProvider, BasicSimulator` |
| 11 | `backend = Aer.get_backend('aer_simulator')` | b0b8 | The global BasicAer provider is no longer exposed; use BasicProvider to obtain backends. | `qiskit.providers.basic_provider` | `backend = BasicSimulator()` |
```