| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
|---|---|---|---|---|---|
| 2 | `from qiskit import qasm2 as qasm` | `QASM2-01` | `Deprecation -> The qiskit.qasm2 module is deprecated. Use qiskit.qasm instead.` | `module: qiskit.qasm2` | `from qiskit import qasm` |
| 9 | `qasm_str = qasm.dumps(qc)` | `QASM2-01` | `Deprecation -> The qiskit.qasm2 module is deprecated. Use qiskit.qasm instead.` | `function: qiskit.qasm2.dumps` | `qasm_str = qasm.dumps(qc)` |
| 10 | `parsed_circuit = qasm.loads(qasm_str)` | `QASM2-01` | `Deprecation -> The qiskit.qasm2 module is deprecated. Use qiskit.qasm instead.` | `function: qiskit.qasm2.loads` | `parsed_circuit = qasm.loads(qasm_str)` |