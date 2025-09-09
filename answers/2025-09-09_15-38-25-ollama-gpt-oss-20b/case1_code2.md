| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :-: | :- | :-: | :- | :- | :- |
| 3 | `from qiskit import QuantumCircuit, qasm, execute` | * | Deprecation -> qasm() function deprecated (optional) | qiskit.qasm | `from qiskit import QuantumCircuit, execute` |
| 13 | `job = execute(qc, getMyBackend(), shots=1000)` | * | Deprecation -> execute() usage deprecated (optional) | qiskit.execute | `job = getMyBackend().run(qc, shots=1000)` |
