| Line | Code | Scenario ID | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
| 1 | `from qiskit.test.mock import FakeVigo` | 0ee | Deprecated FakeVigo backend superseded by GenericBackendV2 | `qiskit.test.mock.FakeVigo` | `from qiskit.providers.fake_provider import GenericBackendV2` |
| 7 | `backend = FakeVigo()` | 0ee | Deprecated FakeVigo backend superseded by GenericBackendV2 | `qiskit.test.mock.FakeVigo` | `backend = GenericBackendV2(num_qubits=5)` |