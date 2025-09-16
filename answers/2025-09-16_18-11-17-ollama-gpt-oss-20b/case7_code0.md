```markdown
| Line | Code | Scenario ID | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
| 2 | `from qiskit.test.mock import FakeVigo` | 4747 | Migration example to the new GenericBackendV2 class | `qiskit.test.mock.FakeVigo` | `from qiskit.providers.fake_provider import GenericBackendV2`<br>`backend = GenericBackendV2(num_qubits=5)` |
```
