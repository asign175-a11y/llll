| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| ----- | ----- | ----- | ----- | ----- | ----- |
| 3 | `from qiskit.providers import fake_provider` | `*` | `Module Relocation -> The qiskit.providers.fake_provider module has been moved.` | `qiskit.providers.fake_provider` | `from qiskit.providers import fake_backends` |
| 4 | `backend = fake_provider.FakeOpenPulse3Q()` | `*` | `Module Relocation -> The FakeOpenPulse3Q class has been moved along with its module.` | `fake_provider.FakeOpenPulse3Q` | `backend = fake_backends.FakeOpenPulse3Q()` |