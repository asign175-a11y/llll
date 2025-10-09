| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| ----- | ----- | ----- | ----- | ----- | ----- |
| 3 | from qiskit import QuantumCircuit, qasm, execute | * | Deprecation -> The `qiskit.qasm` module import is deprecated. (optional) | qasm | from qiskit import QuantumCircuit, execute |
| 3 | from qiskit import QuantumCircuit, qasm, execute | * | Deprecation -> The `qiskit.execute` function is deprecated. (optional) | execute (import) | from qiskit import QuantumCircuit |
| 13 | job = execute(qc, getMyBackend(), shots=1000) | * | Deprecation -> The `qiskit.execute` function is deprecated; use `backend.run()` instead. (optional) | execute (function call) | job = getMyBackend().run(qc, shots=1000) |