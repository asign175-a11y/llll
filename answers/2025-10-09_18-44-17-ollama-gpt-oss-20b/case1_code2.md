| Line | Code | Scenario ID | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
| 3 | from qiskit import QuantumCircuit, qasm, execute | ade7 | DEPRECATION - The legacy `qiskit.qasm` module (OpenQASM 2 parser) is deprecated. Use `qiskit.qasm2` instead. | qiskit.qasm | from qiskit import QuantumCircuit, qasm2, execute |
| 12 | job = execute(qc, getMyBackend(), shots=1000) | b0b8 | DEPRECATION - The `execute()` function is implicitly replaced by `backend.run()`. | execute function | job = getMyBackend().run(qc, shots=1000) |