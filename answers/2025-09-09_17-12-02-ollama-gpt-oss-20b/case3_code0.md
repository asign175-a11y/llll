| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :-: | :- | :-: | :- | :- | :- |
| 1 | from qiskit import qasm | * | Deprecation -> qasm module deprecated | qiskit.qasm | Remove this line; instead import QuantumCircuit: `from qiskit.circuit.quantumcircuit import QuantumCircuit` |
| 5 | circuit1 = qasm.Qasm(data=qasm_str) | * | Deprecation -> qasm.Qasm constructor deprecated | qasm.Qasm | Replace with: `qc1 = QuantumCircuit.from_qasm_str(qasm_str)` |
| 6 | program1 = circuit1.parse() | * | Deprecation -> qasm.Qasm.parse method deprecated | qasm.Qasm.parse | This line is no longer needed; remove it. |
| 7 | qc1 = program1.get_circuit() | * | Deprecation -> qasm.Qasm.get_circuit method deprecated | qasm.Qasm.get_circuit | This line is no longer needed; remove it. |