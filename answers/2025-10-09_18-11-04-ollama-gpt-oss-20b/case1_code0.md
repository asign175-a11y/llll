| Line | Code | Scenario ID | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
| 4 | from qiskit.qasm import Qasm | 03c2 | The `qiskit.qasm` module and `QuantumCircuit.qasm()` method are deprecated; use `qiskit.qasm2` and `qasm2.dump()` or `qasm2.dumps()`. | qiskit.qasm.Qasm | from qiskit import qasm2 |