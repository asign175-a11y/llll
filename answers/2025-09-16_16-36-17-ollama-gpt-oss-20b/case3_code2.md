```markdown
| Line | Code | Scenario ID | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
| 1 | `from qiskit import QuantumCircuit, Aer, execute` | 4185 | qiskit.providers.basicaer module deprecated. | `qiskit.providers.basicaer` | `from qiskit.providers.basic_provider import BasicProvider`<br>`provider = BasicProvider()`<br>`backend = provider.get_backend('qasm_simulator')` |
| 8 | `qasm_str = qc.qasm()` | 03c2 | QuantumCircuit.qasm() deprecated. | `QuantumCircuit.qasm()` | `qasm_str = qasm2.dumps(qc)` |
```