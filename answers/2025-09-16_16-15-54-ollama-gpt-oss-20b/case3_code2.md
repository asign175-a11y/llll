| Line | Code | Scenario ID | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
| 1 | from qiskit import QuantumCircuit, Aer, execute |  |  |  | from qiskit import execute, QuantumCircuit |
| 2 | from qiskit import qasm2 as qasm |  |  |  | from qiskit.qasm2 import dumps as qasm_dumps |
| 3 | qc = QuantumCircuit(2, 2) |  |  |  | qc = QuantumCircuit(2, 2) |
| 4 | qc.h(0) |  |  |  | qc.h(0) |
| 5 | qc.cx(0, 1) |  |  |  | qc.cx(0, 1) |
| 6 | qc.measure([0, 1], [0, 1]) |  |  |  | qc.measure([0, 1], [0, 1]) |
| 7 |  |  |  |  |  |
| 8 | qasm_str = qc.qasm() | 65659cda-9607-423a-9403-c8a7826003c2 | DEPRECATION - `QuantumCircuit.qasm()` is deprecated | `QuantumCircuit.qasm()` | qasm_str = qasm_dumps(qc) |
| 9 |  |  |  |  |  |
| 10 | qasm_qc = qasm.Qasm(data=qasm_str) | 65659cda-9607-423a-9403-c8a7826003c2 | DEPRECATION - `qasm.Qasm` class is removed | `qasm.Qasm` |  |
| 11 | program = qasm_qc.parse() |  |  |  |  |
| 12 | circuit = program.get_circuit() |  |  |  |  |
| 13 |  |  |  |  |  |
| 14 | simulator = Aer.get_backend('qasm_simulator') | bc3463cc-6d45-4fc4-94b8-8ec25c34b185 | DEPRECATION - `Aer` backend access moved | `Aer.get_backend` | simulator = Aer.get_backend('qasm_simulator') |
| 15 | job = execute(qasm_qc, simulator, shots=1024) |  |  |  | job = execute(qc, simulator, shots=1024) |
| 16 | result = job.result() |  |  |  | result = job.result() |
| 17 | counts = result.get_counts(qasm_qc) |  |  |  | counts = result.get_counts(qc) |
| 18 | print(counts) |  |  |  | print(counts) |