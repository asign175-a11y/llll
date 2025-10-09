| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
|---|---|---|---|---|---|
| 3 | `from qiskit import QuantumCircuit, execute, Aer, qasm` | QISKIT-MIG-046-001 | Deprecation -> The global `execute()` function is deprecated in favor of `backend.run()`. | `execute` | `from qiskit import QuantumCircuit, Aer` |
| 3 | `from qiskit import QuantumCircuit, execute, Aer, qasm` | QISKIT-MIG-046-002 | Deprecation -> The direct import of `qasm` module is deprecated. (optional) | `qasm` | `from qiskit import QuantumCircuit, Aer` |
| 14 | `backend = Aer.get_backend('aer_simulator')` | QISKIT-MIG-046-003 | Deprecation -> `Aer.get_backend()` is deprecated. Use direct instantiation of `AerSimulator`. | `Aer.get_backend` | `backend = AerSimulator()` |
| * | | QISKIT-MIG-046-004 | New Feature -> Import `AerSimulator` for direct instantiation of the Aer simulator. | `AerSimulator` | `from qiskit.providers.aer import AerSimulator` |