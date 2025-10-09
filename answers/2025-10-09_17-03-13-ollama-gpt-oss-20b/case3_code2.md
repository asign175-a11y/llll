| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :---- | :---- | :---- | :---- | :---- | :---- |
| 1 | `from qiskit import QuantumCircuit, Aer, execute` | qiskit-0.46.0-execute-import-001 | Deprecation -> The `execute()` function is deprecated. | `execute` | |
| 2 | `from qiskit import qasm2 as qasm` | qiskit-0.46.0-qasm2-module-001 | Deprecation -> The `qiskit.qasm2` module is deprecated. | `qiskit.qasm2` | `from qiskit import qasm` |
| 9 | `qasm_str = qc.qasm()` | qiskit-0.46.0-qc-qasm-method-001 | Deprecation -> `QuantumCircuit.qasm()` method is deprecated. | `QuantumCircuit.qasm()` | `qasm_str = qc.qasm(encoding='qasm2')` |
| 11 | `qasm_qc = qasm.Qasm(data=qasm_str)` | qiskit-0.46.0-qasm-Qasm-class-001 | Deprecation -> The `qiskit.qasm.Qasm` class constructor is deprecated. | `qasm.Qasm` | `parsed_circuit = qasm.loads(qasm_str)` |
| 12 | `program = qasm_qc.parse()` | qiskit-0.46.0-qasm-parse-method-001 | Deprecation -> `qiskit.qasm.Qasm.parse()` method is deprecated. | `qasm.Qasm.parse()` | |
| 13 | `circuit = program.get_circuit()` | qiskit-0.46.0-qasm-get_circuit-method-001 | Deprecation -> `qiskit.qasm.Qasm.get_circuit()` method is deprecated. | `qasm.Qasm.get_circuit()` | |
| 16 | `job = execute(qasm_qc, simulator, shots=1024)` | qiskit-0.46.0-execute-function-001 | Deprecation -> The `execute()` function is deprecated. | `execute` | `job = simulator.run(parsed_circuit, shots=1024)` |
| 18 | `counts = result.get_counts(qasm_qc)` | qiskit-0.46.0-result-get_counts-001 | Deprecation -> `Result.get_counts()` method no longer accepts a circuit argument. | `Result.get_counts()` | `counts = result.get_counts()` |