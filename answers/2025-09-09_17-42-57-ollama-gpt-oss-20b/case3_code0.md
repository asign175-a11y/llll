| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :-: | :- | :-: | :- | :- | :- |
| 1 | `from qiskit import qasm` | * | Deprecation -> qiskit.qasm module deprecated | qiskit.qasm | `from qiskit.qasm import parse_qasm` |
| 9 | `circuit1 = qasm.Qasm(data=qasm_str)` | * | Deprecation -> qiskit.qasm.Qasm class deprecated | qiskit.qasm.Qasm | `qc1 = QuantumCircuit.from_qasm_str(qasm_str)` |
| 10 | `program1 = circuit1.parse()` | * | Deprecation -> qiskit.qasm.Qasm.parse method deprecated | qiskit.qasm.Qasm.parse | *(remove; use QuantumCircuit.from_qasm_str instead)* |
| 11 | `qc1 = program1.get_circuit()` | * | Deprecation -> qiskit.qasm.QasmProgram.get_circuit method deprecated | qiskit.qasm.QasmProgram.get_circuit | *(remove; use QuantumCircuit.from_qasm_str instead)* |
