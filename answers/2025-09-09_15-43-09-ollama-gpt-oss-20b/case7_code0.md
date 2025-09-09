| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
|:-:|:-|:-:|:-|:-|:-|
| 2 | `from qiskit.test.mock import FakeVigo` | * | Deprecation -> `FakeVigo` class moved to `qiskit.providers.fake_provider` | `qiskit.providers.fake_provider` | `from qiskit.providers.fake_provider import FakeVigo` |