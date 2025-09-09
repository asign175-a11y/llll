| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :-: | :- | :-: | :- | :- | :- |
| 3 | `from qiskit import QuantumCircuit, qasm, execute` | * | Deprecation -> qiskit.qasm module deprecated | qiskit.qasm | `# Remove qasm import; use circuit.qasm() if needed` |