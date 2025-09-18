| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
| 2 | from qiskit.test.mock import FakeVigo | * | Deprecation -> `qiskit.test.mock` module removed | `qiskit.test.mock.FakeVigo` | from qiskit.providers.fake_provider import FakeVigo |
| 3 | from qiskit.test.reference_circuits import ReferenceCircuits | * | Deprecation -> `qiskit.test.reference_circuits` module removed | `qiskit.test.reference_circuits.ReferenceCircuits` | from qiskit.circuit.library import BellState |
| 5 | qc = ReferenceCircuits.bell() | * | Deprecation -> `ReferenceCircuits.bell()` removed | `qiskit.test.reference_circuits.ReferenceCircuits.bell` | qc = BellState() |