| Line | Code | Scenario ID | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
| 4 | `from qiskit.qasm import Qasm` | QISKIT-0.46.0-DEPRECATION-QASM-CLASS | DEPRECATION - The qiskit.qasm.Qasm class is deprecated | qiskit.qasm.Qasm | Remove this import or replace with `from qiskit.qasm import export_qasm` (or use `qc.qasm()` to obtain QASM). |