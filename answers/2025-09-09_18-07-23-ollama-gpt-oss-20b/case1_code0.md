| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
| 4 | `from qiskit.qasm import Qasm` | * | Deprecation -> qiskit.qasm module removed (optional) | qiskit.qasm.Qasm | `# Remove this import` |
| 5 | `from qiskit.algorithms import VQE` | * | Deprecation -> VQE moved to qiskit.algorithms.VQE (optional) | qiskit.algorithms.VQE | `from qiskit.algorithms.VQE import VQE` |
| 6 | `from qiskit import qasm2 as qasm` | * | Import qasm2 deprecated in top-level, use from qiskit.qasm2 import dump as qasm (optional) | qiskit.qasm2 | `from qiskit.qasm2 import dump as qasm` |