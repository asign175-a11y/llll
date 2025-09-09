| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :-: | :- | :-: | :- | :- | :- |
| 3 | from qiskit import QuantumCircuit, execute, Aer, qasm | * | Deprecation -> qiskit.qasm() function deprecated | qiskit.qasm | # Remove qasm import; use `circuit.qasm()` method instead |