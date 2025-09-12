**Migrated code for Qiskit 0.46.0**

| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
| 4 | `from qiskit.qasm import Qasm` | * | Deprecation -> `qiskit.qasm` module removed | `qiskit.qasm` | `from qiskit.qasm2 import Qasm2 as Qasm` |