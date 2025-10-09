| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
|---|---|---|---|---|---|
| 1 | `from qiskit import QuantumCircuit, Aer, execute` | QS_001 | Deprecation -> The `execute()` function is deprecated. | `execute` | `from qiskit import QuantumCircuit, Aer` |
| 2 | `from qiskit.quantum_info import Pauli, state_fidelity` | QS_002 | Deprecation -> The `state_fidelity()` function is deprecated. | `state_fidelity` | `from qiskit.quantum_info import Pauli, Statevector` |
| 19 | `simulator = Aer.get_backend('statevector_simulator')` | * | Change in API -> The `Aer.get_backend()` method for simulator instantiation now uses `AerSimulator()`. | `Aer.get_backend` | `simulator = AerSimulator()` |
| 20 | `result = execute(qc, simulator).result()` | QS_001 | Deprecation -> The `execute()` function is deprecated. | `execute` | `result = simulator.run(qc).result()` |
| 24 | `fidelity = state_fidelity(statevector, target_state)` | QS_002 | Deprecation -> The `state_fidelity()` function is deprecated. | `state_fidelity` | `fidelity = Statevector(statevector).fidelity(Statevector(target_state))` |