| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :-: | :- | :-: | :- | :- | :- |
| 1 | `from qiskit.qasm import Qasm` | * | Deprecation -> qiskit.qasm.Qasm deprecated | qiskit.qasm.Qasm | `from qiskit.circuit import QuantumCircuit` |
| 5 | `circuit2 = Qasm(filename=qasm_file)` | * | Deprecation -> Qasm constructor usage deprecated | qiskit.qasm.Qasm | `qc2 = QuantumCircuit.from_qasm_file(qasm_file)` |
| 6 | `program2 = circuit2.parse()` | * | Deprecation -> Qasm.parse() deprecated | qiskit.qasm.Qasm | *(remove this line)* |
| 7 | `qc2 = program2.get_circuit()` | * | Deprecation -> get_circuit() deprecated | qiskit.qasm.Qasm | *(remove this line)* |