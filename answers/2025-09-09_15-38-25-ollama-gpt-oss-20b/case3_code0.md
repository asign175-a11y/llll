| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :-: | :- | :-: | :- | :- | :- |
| 1 | `from qiskit import qasm` | * | Deprecation -> qiskit.qasm module deprecated | `qiskit.qasm` | `from qiskit.circuit import QuantumCircuit` |
| 13 | `circuit1 = qasm.Qasm(data=qasm_str)` | * | Deprecation -> qasm.Qasm constructor deprecated | `qiskit.qasm.Qasm` | `qc1 = QuantumCircuit.from_qasm_str(qasm_str)` |
| 14 | `program1 = circuit1.parse()` | * | Deprecation -> qasm.Qasm.parse() deprecated | `qiskit.qasm.Qasm.parse` | `qc1 = QuantumCircuit.from_qasm_str(qasm_str)` |
| 15 | `qc1 = program1.get_circuit()` | * | Deprecation -> qasm.Program.get_circuit() deprecated | `qiskit.qasm.Program.get_circuit` | `qc1 = QuantumCircuit.from_qasm_str(qasm_str)` |