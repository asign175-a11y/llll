| Line | Code | Scenario ID | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
| 14 | `simulator = Aer.get_backend('qasm_simulator')` | b185 | The `qiskit.providers.basicaer` module and all of its classes are deprecated from Qiskit 0.46 onwards. Their use should be replaced with the `qiskit.quantum_info` module and the new `qiskit.providers.basic_provider` module. | `Aer.get_backend('qasm_simulator')` | `from qiskit.providers.basic_provider import BasicSimulator`
`simulator = BasicSimulator()` |
| 15 | `job = execute(qasm_qc, simulator, shots=1024)` | 8c20 | The execution of circuits on backends is performed via the `run` method of the backend object. | `execute` | `job = simulator.run(qasm_qc, shots=1024)` |