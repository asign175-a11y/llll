| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :-: | :- | :-: | :- | :- | :- |
| 17 | `qc.unitary(Operator(evolution_matrix), [0])` | * | Deprecation -> QuantumCircuit.unitary() deprecated (optional) | QuantumCircuit.unitary | `qc.append(Operator(evolution_matrix), [0])` |
| 19 | `simulator = Aer.get_backend('statevector_simulator')` | * | Deprecation -> Aer.get_backend('statevector_simulator') deprecated (optional) | Aer.get_backend('statevector_simulator') | `simulator = Aer.get_backend('aer_simulator_statevector')` |