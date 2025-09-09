| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :-: | :- | :-: | :- | :- | :- |
| 2 | `from qiskit import qasm2 as qasm` | * | Deprecation -> qiskit.qasm2 import deprecated (optional) | qiskit.qasm2 | `from qiskit.qasm2 import parse_qasm` |
| 11 | `qasm_qc = qasm.Qasm(data=qasm_str)` | * | Deprecation -> Qasm class deprecated | qiskit.qasm2.Qasm | `circuit = qiskit.qasm2.parse_qasm(qasm_str)` |
| 12 | `program = qasm_qc.parse()` | * | Deprecation -> Qasm.parse method deprecated | Qasm.parse |  |
| 16 | `job = execute(qasm_qc, simulator, shots=1024)` | * | Deprecation -> execute expects QuantumCircuit, not Qasm | execute | `job = execute(circuit, simulator, shots=1024)` |
| 18 | `counts = result.get_counts(qasm_qc)` | * | Deprecation -> get_counts expects QuantumCircuit, not Qasm | result.get_counts | `counts = result.get_counts(circuit)` |
| 15 | `simulator = Aer.get_backend('qasm_simulator')` | * | Deprecation -> Aer.get_backend optional | Aer.get_backend |  |