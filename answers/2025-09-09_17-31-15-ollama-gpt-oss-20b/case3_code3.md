| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :-: | :- | :-: | :- | :- | :- |
| 2 | `from qiskit import qasm2 as qasm                # type: ignore` | * | Deprecation -> qiskit import qasm2 module deprecated (optional) | qiskit.qasm2 | `from qiskit.qasm2 import dumps, loads` (update usage to `dumps(qc)` and `loads(qasm_str)`) |