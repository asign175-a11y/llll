| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
| 4 | from qiskit.qasm import Qasm | * | Deprecation -> Qasm import from qiskit.qasm deprecated | qiskit.qasm.Qasm | from qiskit.qasm2 import Qasm |
| 8 | qc = QuantumCircuit(2, 2) | * | Deprecation -> QuantumCircuit constructor with classical bits deprecated (optional) | qiskit.circuit.QuantumCircuit | qc = QuantumCircuit(2)<br>qc.add_register(ClassicalRegister(2))