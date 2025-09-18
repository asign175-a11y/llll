| Line | Code | Scenario ID | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
| 4 | `from qiskit.qasm import Qasm` | * | DEPRECATION - The qiskit.qasm module is removed | qiskit.qasm | `from qiskit.qasm2 import Qasm` |
| 6 | `from qiskit import qasm2 as qasm` | * | DEPRECATION - The qiskit.qasm2 module is not available | qiskit.qasm2 | `# from qiskit import qasm2 as qasm` |