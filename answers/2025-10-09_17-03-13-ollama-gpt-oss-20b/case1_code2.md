| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| ----- | ----- | ----- | ----- | ----- | ----- |
| 3 | `from qiskit import QuantumCircuit, qasm, execute` | * | Deprecation -> The `qiskit.qasm` module is deprecated. | `qasm` (module) | `from qiskit import QuantumCircuit` |
| 3 | `from qiskit import QuantumCircuit, qasm, execute` | * | Deprecation -> The `qiskit.execute` function is deprecated. | `execute` (function import) | `from qiskit import QuantumCircuit` |
| 13 | `job = execute(qc, getMyBackend(), shots=1000)` | * | Deprecation -> The `qiskit.execute` function is deprecated. Use the backend's `run` method instead. | `execute` (function call) | `job = getMyBackend().run(qc, shots=1000)` |
| 14 | `result = job.result().get_counts(qc)` | * | Deprecation -> The `get_counts()` method argument `qc` is no longer required for single-circuit jobs (optional). | `get_counts(qc)` (method call) | `result = job.result().get_counts()` |