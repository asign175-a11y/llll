| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
| 2 | `from qiskit import qasm2 as qasm` | \* | Import -> qasm2 import path changed (optional) | qasm2 import | `from qiskit.qasm2 import Qasm as qasm` |
| 11 | `qasm_qc = qasm.Qasm(data=qasm_str)` | \* | Deprecation -> Qasm constructor data argument removed (optional) | qasm.Qasm constructor | `qasm_qc = qasm.Qasm(qasm_str)` |
| 16 | `job = execute(qasm_qc, simulator, shots=1024)` | \* | Function -> execute requires QuantumCircuit, not Qasm (mandatory) | execute input type | `job = execute(circuit, simulator, shots=1024)` |
| 18 | `counts = result.get_counts(qasm_qc)` | \* | Function -> get_counts requires QuantumCircuit (mandatory) | result.get_counts argument | `counts = result.get_counts(circuit)` |