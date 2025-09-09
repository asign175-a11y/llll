| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :-: | :- | :-: | :- | :- | :- |
| 3 | `from qiskit.providers import fake_provider` | * | Deprecation -> fake_provider import deprecated (mandatory) | `qiskit.providers.fake_provider` | `from qiskit.providers.fake_provider import FakeOpenPulse3Q` |
| 5 | `backend = fake_provider.FakeOpenPulse3Q()` | * | Deprecation -> use of fake_provider to instantiate backend deprecated (mandatory) | `qiskit.providers.fake_provider` | `backend = FakeOpenPulse3Q()` |