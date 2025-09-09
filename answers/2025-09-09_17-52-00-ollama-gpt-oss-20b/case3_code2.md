| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :-: | :- | :-: | :- | :- | :- |
| 2 | `from qiskit import qasm2 as qasm` | * | Deprecation -> qiskit.qasm2 module deprecated (optional) | qiskit.qasm2 | `from qiskit.qasm2 import qasm2_to_circuit` |
| 11 | `qasm_qc = qasm.Qasm(data=qasm_str)` | * | Deprecation -> qiskit.qasm2.Qasm class deprecated (optional) | qiskit.qasm2.Qasm | `circuit = qasm2_to_circuit(qasm_str)` |
| 12 | `program = qasm_qc.parse()` | * | Deprecation -> qiskit.qasm2.Qasm.parse() deprecated (optional) | qiskit.qasm2.Qasm | *remove or replace by `circuit = qasm2_to_circuit(qasm_str)`* |
| 13 | `circuit = program.get_circuit()` | * | Deprecation -> qiskit.qasm2.Program.get_circuit() deprecated (optional) | qiskit.qasm2.Program | *remove or replace by `circuit = qasm2_to_circuit(qasm_str)`* |
| 16 | `job = execute(qasm_qc, simulator, shots=1024)` | * | Deprecation -> execute() should receive a QuantumCircuit (optional) | qiskit.execute | `job = execute(circuit, simulator, shots=1024)` |
| 18 | `counts = result.get_counts(qasm_qc)` | * | Deprecation -> result.get_counts() should receive a QuantumCircuit (optional) | qiskit.result | `counts = result.get_counts(circuit)` |