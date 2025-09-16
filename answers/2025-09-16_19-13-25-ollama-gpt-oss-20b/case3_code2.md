| Line | Code | Scenario ID | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
| 1 | `from qiskit import QuantumCircuit, Aer, execute` | b185 | Importing from `qiskit.providers.aer` (including `Aer`) is deprecated; use `qiskit_aer` instead. | `qiskit.Aer` | `from qiskit import QuantumCircuit, execute`<br>`from qiskit_aer import Aer` |
| 9 | `qasm_str = qc.qasm()` | 03c2 | The `QuantumCircuit.qasm()` method is deprecated; use `qasm2.dumps()` instead. | `QuantumCircuit.qasm()` | `qasm_str = qasm.dumps(qc)` |