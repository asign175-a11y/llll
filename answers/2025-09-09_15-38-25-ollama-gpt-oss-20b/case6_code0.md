| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :-: | :- | :-: | :- | :- | :- |
| 3 | `from qiskit.providers import fake_provider` | * | Deprecation -> fake_provider import removed | `qiskit.providers.fake_provider` | `from qiskit.providers.fake_provider import FakeOpenPulse3Q` |
| 5 | `backend = fake_provider.FakeOpenPulse3Q()` | * | Deprecation -> fake_provider reference removed | `FakeOpenPulse3Q` | `backend = FakeOpenPulse3Q()` |