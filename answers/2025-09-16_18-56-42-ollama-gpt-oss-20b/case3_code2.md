```markdown
| Line | Code | Scenario ID | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
| 9 | `qasm_str = qc.qasm()` | c2 | QuantumCircuit.qasm() method used to generate a OpenQASM 2 representation of the QuantumCircuit object has been deprecated and will be removed in the Qiskit 1.0.0 release. The qasm2.dump() or qasm2.dumps() functions which provide similar functionality should be used instead. | QuantumCircuit.qasm | `qasm_str = qasm.dump(qc)` or `qasm_str = qasm.dumps(qc)` |
```