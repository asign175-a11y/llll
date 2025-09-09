| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :-: | :- | :-: | :- | :- | :- |
| 11 | `qasm_qc = qasm.Qasm(data=qasm_str)` | * | Deprecation -> qasm.Qasm class deprecated (optional) | qasm.Qasm | `circuit = qiskit.qasm2.parse(qasm_str)` |
| 12 | `program = qasm_qc.parse()` | * | Deprecation -> Qasm.parse() method removed (optional) | qasm.Qasm | * |
| 13 | `circuit = program.get_circuit()` | * | Deprecation -> Program.get_circuit() method removed (optional) | Program | * |
| 16 | `job = execute(qasm_qc, simulator, shots=1024)` | * | Deprecation -> execute() on Qasm instance (optional) | execute | `job = execute(circuit, simulator, shots=1024)` |
| 18 | `counts = result.get_counts(qasm_qc)` | * | Deprecation -> get_counts() on Qasm instance (optional) | Result | `counts = result.get_counts(circuit)` |