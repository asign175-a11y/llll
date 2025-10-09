| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :---- | :---- | :---- | :---- | :---- | :---- |
| 3 | `from qiskit.providers import fake_provider` | * | Deprecation -> The `qiskit.providers.fake_provider` module moved to `qiskit.providers.fake_backends`. | `fake_provider` | `from qiskit.providers.fake_backends import FakeOpenPulse3Q` |
| 5 | `backend = fake_provider.FakeOpenPulse3Q()` | * | Deprecation -> The `fake_provider` reference is no longer valid. | `fake_provider` | `backend = FakeOpenPulse3Q()` |
| 7 | `with pulse.build(backend) as schedule:` | * | Deprecation (optional) -> The `qiskit.pulse.build` context manager is deprecated. | `pulse.build` | `with qiskit.pulse.builder.build(backend) as schedule:` |