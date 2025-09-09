| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :-: | :- | :-: | :- | :- | :- |
| 3 | `from qiskit import QuantumCircuit, execute, Aer, qasm` | * | Deprecation -> execute function deprecated (optional) | qiskit.execute | # Replace usage with `backend.run(qc)` or remove the import if not used |
| 3 | `from qiskit import QuantumCircuit, execute, Aer, qasm` | * | Deprecation -> qasm function deprecated (optional) | qiskit.qasm | # Remove `qasm` import; use `QuantumCircuit.from_qasm_str` if a QASM string is needed |