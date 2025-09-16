```markdown
| Line | Code | Scenario ID | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
| 2 | `from qiskit.test.mock import FakeVigo` | b0ee | Fake provider deprecation; use qiskit-ibm-runtime FakeProvider | `qiskit.test.mock.FakeVigo` | `from qiskit_ibm_runtime.fake_provider import FakeProvider` |
| 6 | `backend = FakeVigo()` | b0ee | Fake provider deprecation; use qiskit-ibm-runtime FakeProvider | `qiskit.test.mock.FakeVigo` | `backend = FakeProvider().get_backend("fake_vigo")` |
```