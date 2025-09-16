| Line | Code | Scenario ID | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
| 2 | from qiskit import qasm2 as qasm                # type: ignore | 65659cda-9607-423a-9403-c8a7826003c2 | DEPRECATION - Use qiskit-qasm2 instead of qiskit.qasm2 | qiskit.qasm2 | `from qiskit_qasm2 import dumps, loads` |
| 10 | qasm_str = qasm.dumps(qc) | 65659cda-9607-423a-9403-c8a7826003c2 | DEPRECATION - Use qiskit-qasm2 functions | qiskit.qasm2 | `qasm_str = dumps(qc)` |
| 11 | parsed_circuit = qasm.loads(qasm_str) | 65659cda-9607-423a-9403-c8a7826003c2 | DEPRECATION - Use qiskit-qasm2 functions | qiskit.qasm2 | `parsed_circuit = loads(qasm_str)` |