| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :-: | :- | :-: | :- | :- | :- |
| 2 | `from qiskit.test.mock import FakeVigo` | * | Deprecation -> `FakeVigo` import from `qiskit.test.mock` deprecated | `qiskit.test.mock` | `from qiskit.providers.fake_provider import FakeVigo` |
| 3 | `from qiskit.test.reference_circuits import ReferenceCircuits` | * | Deprecation -> `ReferenceCircuits` import from `qiskit.test.reference_circuits` deprecated | `qiskit.test.reference_circuits` | `from qiskit.circuit.library import BellState` |
| 7 | `qc = ReferenceCircuits.bell()` | * | Deprecation -> `ReferenceCircuits.bell()` usage deprecated | `ReferenceCircuits.bell` | `qc = BellState()` |
| 20 | `qc = ReferenceCircuits.bell()` | * | Deprecation -> `ReferenceCircuits.bell()` usage deprecated | `ReferenceCircuits.bell` | `qc = BellState()` |