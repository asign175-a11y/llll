| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
| 3 | `from qiskit.providers import fake_provider` | `*` | `Deprecated -> Use direct import from submodule (optional)` | `qiskit.providers.fake_provider` | `from qiskit.providers.fake_provider import FakeOpenPulse3Q` |
| 5 | `backend = fake_provider.FakeOpenPulse3Q()` | `*` | `Deprecated -> Direct instantiation (optional)` | `FakeOpenPulse3Q` | `backend = FakeOpenPulse3Q()` |
| 7 | `with pulse.build(backend) as schedule:` | `*` | `Deprecated -> use pulse.schedule (optional)` | `pulse.build` | `with pulse.schedule(backend) as schedule:` |

