| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :-: | :- | :-: | :- | :- | :- |
| 2 | `from qiskit.test.mock import FakeVigo` | * | Deprecation -> qiskit.test.mock module deprecated | qiskit.test.mock | `from qiskit.providers.fake_provider import FakeVigo` |
| 3 | `from qiskit.test.reference_circuits import ReferenceCircuits` | * | Deprecation -> qiskit.test.reference_circuits module deprecated | qiskit.test.reference_circuits | `from qiskit.circuit.library import BellCircuit` (use `BellCircuit()` in place of `ReferenceCircuits.bell()`) |