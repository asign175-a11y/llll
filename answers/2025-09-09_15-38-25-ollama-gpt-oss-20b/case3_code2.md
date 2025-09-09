| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :-: | :- | :-: | :- | :- | :- |
| 2 | from qiskit import qasm2 as qasm | * | Deprecation -> qiskit.qasm2 module deprecated | qiskit.qasm2 | import qiskit.qasm as qasm |
| 11 | qasm_qc = qasm.Qasm(data=qasm_str) | * | Deprecation -> qasm.Qasm constructor deprecated | qiskit.qasm2.Qasm | qasm_qc = qiskit.qasm.Qasm(data=qasm_str) |
| 16 | job = execute(qasm_qc, simulator, shots=1024) | * | Deprecation -> executing Qasm object deprecated | qiskit.execute | job = execute(circuit, simulator, shots=1024) |
| 18 | counts = result.get_counts(qasm_qc) | * | Deprecation -> get_counts with Qasm object deprecated | qiskit.result | counts = result.get_counts(circuit) |