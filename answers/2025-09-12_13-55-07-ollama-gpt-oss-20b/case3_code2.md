| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
|:----:|------|-------------|----------|----------|------------|
| 2 | from qiskit import qasm2 as qasm | * | Deprecation -> import qasm2 as alias | qasm2 | from qiskit.qasm2 import Qasm |
| 11 | qasm_qc = qasm.Qasm(data=qasm_str) | * | Deprecation -> Qasm usage via alias | Qasm | qasm_qc = Qasm(data=qasm_str) |
| 16 | job = execute(qasm_qc, simulator, shots=1024) | * | Deprecation -> execute expects QuantumCircuit, not Qasm | execute | job = execute(circuit, simulator, shots=1024) |
| 18 | counts = result.get_counts(qasm_qc) | * | Deprecation -> get_counts expects QuantumCircuit, not Qasm | result.get_counts | counts = result.get_counts(circuit) |