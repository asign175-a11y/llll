| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
| 2 | `from qiskit import qasm2 as qasm` | * | Deprecation → `qasm2` import removed | `qasm2` | `from qiskit.qasm import Qasm2Parser` |
| 11 | `qasm_qc = qasm.Qasm(data=qasm_str)` | * | Deprecation → `Qasm` class removed | `Qasm` | `parser = Qasm2Parser(); qasm_qc = parser.parse(data=qasm_str)` |
| 16 | `job = execute(qasm_qc, simulator, shots=1024)` | * | Migration → `execute` requires a `QuantumCircuit` | `execute` | `job = execute(circuit, simulator, shots=1024)` |
| 18 | `counts = result.get_counts(qasm_qc)` | * | Migration → `get_counts` requires a `QuantumCircuit` | `get_counts` | `counts = result.get_counts(circuit)` |