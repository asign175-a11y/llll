| Line | Code | Scenario ID | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
| 3 | from qiskit.providers.fake_provider import FakeOpenPulse3Q | b0ee | The qiskit.providers.fake_provider module has been migrated to the qiskit-ibm-runtime Python package. | qiskit.providers.fake_provider | from qiskit_ibm_runtime.fake_provider import FakeOpenPulse3Q |
| 5 | backend = FakeOpenPulse3Q() | a747 | Fake backends designed for special testing purposes have been superseded by the new GenericBackendV2 class, and are also deprecated as of Qiskit 0.46. | FakeOpenPulse3Q | GenericBackendV2(num_qubits=3) |
| 9 |     pulse.u2(0, math.pi, 0) | 1f3a | Injecting circuit gate operations into the pulse builder context is now deprecated. | pulse.u2 | |
| 10 |     pulse.cx(0, 1) | 1f3a | Injecting circuit gate operations into the pulse builder context is now deprecated. | pulse.cx | |
| 15 |         pulse.play(pulse.Constant(bell_prep.duration, 0.02), d2) | 1f3a | Injecting circuit gate operations into the pulse builder context is now deprecated. | pulse.play | |
| 16 |         pulse.barrier(0, 1, 2) | 1f3a | Injecting circuit gate operations into the pulse builder context is now deprecated. | pulse.barrier | |
| 17 |         registers = pulse.measure_all() | 1f3a | Injecting circuit gate operations into the pulse builder context is now deprecated. | pulse.measure_all |