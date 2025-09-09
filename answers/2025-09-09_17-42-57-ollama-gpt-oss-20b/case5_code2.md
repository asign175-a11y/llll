| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :-: | :- | :-: | :- | :- | :- |
| 1 | `from qiskit import QuantumCircuit, Aer, execute` | * | Deprecation -> execute function deprecated (optional) | qiskit.execute | Remove `execute` import; use `backend.run()` instead. |
| 17 | `qc.unitary(Operator(evolution_matrix), [0])` | * | Deprecation -> QuantumCircuit.unitary method deprecated | QuantumCircuit.unitary | Replace with `qc.append(Operator(evolution_matrix), [0], [])`. |
| 19 | `simulator = Aer.get_backend('statevector_simulator')` | * | Deprecation -> Aer.get_backend deprecated | Aer.get_backend | Use `from qiskit.providers.aer import AerSimulator; simulator = AerSimulator(method='statevector')`. |
| 20 | `result = execute(qc, simulator).result()` | * | Deprecation -> execute function usage deprecated | qiskit.execute | Replace with `result = simulator.run(qc).result()`. |