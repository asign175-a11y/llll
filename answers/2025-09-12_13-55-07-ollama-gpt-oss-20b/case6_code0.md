| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
| 1 | from qiskit import pulse | * | Deprecation → `from qiskit import pulse` deprecated (optional) | qiskit import pulse | from qiskit.pulse import pulse |
| 3 | from qiskit.providers import fake_provider | * | Import → `fake_provider` moved to submodule | qiskit.providers.fake_provider | from qiskit.providers.fake_provider import FakeOpenPulse3Q |
| 5 | backend = fake_provider.FakeOpenPulse3Q() | * | Usage → replace `fake_provider.FakeOpenPulse3Q()` with direct class import | FakeOpenPulse3Q class | backend = FakeOpenPulse3Q() |
| 7 | with pulse.build(backend) as schedule: | * | Deprecation → `pulse.build()` removed | pulse.build | with pulse.schedule(backend) as schedule: |