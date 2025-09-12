| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
|:--:|:---|:---------:|:-------|:-------|:----------|
| 3 | from qiskit import QuantumCircuit, qasm, execute | * | Deprecation -> qasm() function deprecated (optional) | qiskit.qasm | Remove `qasm` import; replace any usage with `qc.qasm()` or remove if unused. |