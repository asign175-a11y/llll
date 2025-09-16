| Line | Code | Scenario ID | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
| 1 | `from qiskit import QuantumCircuit, Aer, execute` | 8c20 | Replace deprecated Aer provider with BasicProvider/BasicSimulator | `qiskit.providers.basicaer.Aer` | `from qiskit import QuantumCircuit; from qiskit.providers.basic_provider import BasicSimulator` |
| 19 | `simulator = Aer.get_backend('statevector_simulator')` | 8c20 | Switch to new BasicSimulator backend | `qiskit.providers.basicaer.StatevectorSimulatorPy` | `backend = BasicSimulator()` |
| 20 | `result = execute(qc, simulator).result()` | 6012 | Use Statevector object directly instead of executing backend | `result.get_statevector()` | `statevector = Statevector(qc)` |