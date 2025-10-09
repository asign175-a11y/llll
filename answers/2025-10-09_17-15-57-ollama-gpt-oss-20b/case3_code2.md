| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
|---|---|---|---|---|---|
| 1 | from qiskit import QuantumCircuit, Aer, execute | execute-function-deprecation | Deprecation -> The `qiskit.execute()` function is deprecated. | execute | |
| 2 | from qiskit import qasm2 as qasm | qasm-module-and-class-deprecation | Deprecation -> The `qiskit.qasm2` module and `qiskit.qasm.Qasm` class are deprecated. | qiskit.qasm2 | |
| 9 | qasm_qc = qasm.Qasm(data=qasm_str) | qasm-module-and-class-deprecation | Deprecation -> The `qiskit.qasm.Qasm` class is deprecated. | qasm.Qasm | circuit = QuantumCircuit.from_qasm_str(qasm_str) |
| 10 | program = qasm_qc.parse() | qasm-parser-obsolete | API Change -> The `Qasm.parse()` method is obsolete due to `Qasm` class deprecation. | qasm_qc.parse() | |
| 11 | circuit = program.get_circuit() | qasm-parser-obsolete | API Change -> The `QasmProgram.get_circuit()` method is obsolete due to `Qasm` class deprecation. | program.get_circuit() | |
| 14 | job = execute(qasm_qc, simulator, shots=1024) | execute-function-deprecation | Deprecation -> The `qiskit.execute()` function is deprecated. | execute | job = simulator.run(circuit, shots=1024) |
| 16 | counts = result.get_counts(qasm_qc) | result-get-counts-argument-change | API Change -> `result.get_counts()` expects a `QuantumCircuit` object, not a `Qasm` object. | get_counts parameter | counts = result.get_counts(circuit) |