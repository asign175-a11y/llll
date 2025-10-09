| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| ----- | ----- | ----- | ----- | ----- | ----- |
| 2 | from qiskit.providers.fake_provider import FakeOpenPulse3Q | FP-DEP-001 | Deprecation -> The qiskit.providers.fake_provider module is deprecated (optional) | qiskit.providers.fake_provider | from qiskit_ibm_runtime.fake_provider import FakeOpenPulse3Q |
| 18 | registers = pulse.measure_all() | PB-DEP-001 | Deprecation -> The pulse.measure_all() function is deprecated | pulse.measure_all | registers = pulse.measure() |