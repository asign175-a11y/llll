| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
|---|---|---|---|---|---|
| 2 | `from qiskit import qasm2 as qasm                # type: ignore` | `qasm2-module-removed` | Deprecation -> The `qiskit.qasm2` module has been removed. | `qiskit.qasm2` | |
| 10 | `qasm_str = qasm.dumps(qc)` | `qasm2-dumps-removed` | Deprecation -> The `qiskit.qasm2.dumps` function has been removed. | `qiskit.qasm2.dumps` | `qasm_str = qc.qasm()` |
| 11 | `parsed_circuit = qasm.loads(qasm_str)` | `qasm2-loads-removed` | Deprecation -> The `qiskit.qasm2.loads` function has been removed. | `qiskit.qasm2.loads` | `parsed_circuit = QuantumCircuit.from_qasm_str(qasm_str)` |