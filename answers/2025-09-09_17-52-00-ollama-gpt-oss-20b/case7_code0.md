| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :-: | :- | :-: | :- | :- | :- |
| 2 | `from qiskit.test.mock import FakeVigo` | * | Deprecation -> qiskit.test.mock import FakeVigo deprecated | qiskit.test.mock | `from qiskit.providers.fake_provider import FakeVigo` |
| 3 | `from qiskit.test.reference_circuits import ReferenceCircuits` | * | Deprecation -> qiskit.test.reference_circuits import ReferenceCircuits deprecated | qiskit.test.reference_circuits | `from qiskit.circuit.library import BellState` |
| 5 | `qc = ReferenceCircuits.bell()` | * | Deprecation -> ReferenceCircuits.bell() usage deprecated | ReferenceCircuits | `qc = BellState()` |