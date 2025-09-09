| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :-: | :- | :-: | :- | :- | :- |
| 1 | `from qiskit import pulse` | * | Deprecation -> import pulse from qiskit is deprecated (optional) | qiskit | `import qiskit.pulse as pulse` |
| 3 | `from qiskit.providers import fake_provider` | * | Deprecation -> importing fake_provider from qiskit.providers is deprecated (optional) | fake_provider | `from qiskit.providers.fake_provider import FakeOpenPulse3Q` |
| 7 | `with pulse.build(backend) as schedule:` | * | Deprecation -> pulse.build context manager is deprecated (mandatory) | pulse.build | `with pulse.Schedule(backend) as schedule:` |
| 12 | `pulse.measure(0)` | * | Deprecation -> pulse.measure without backend is deprecated (optional) | pulse.measure | `pulse.measure(0, backend)` |