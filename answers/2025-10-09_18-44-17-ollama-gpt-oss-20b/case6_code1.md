| Line | Code | Scenario ID | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
| 3 | from qiskit.providers.fake_provider import FakeOpenPulse3Q | 0db0ee | The qiskit.providers.fake_provider module has been migrated to the qiskit-ibm-runtime Python package. | qiskit.providers.fake_provider.FakeOpenPulse3Q | from qiskit_ibm_runtime.fake_provider import FakeOpenPulse3Q |
| 5 | backend = FakeOpenPulse3Q() | 0db0ee | The qiskit.providers.fake_provider module has been migrated to the qiskit-ibm-runtime Python package. | qiskit.providers.fake_provider.FakeOpenPulse3Q | |
| 9 | pulse.u2(0, math.pi, 0) | 171f3a | Injecting circuit gate operations into the pulse builder context is now deprecated. | pulse.u2 | N/A |
| 10 | pulse.cx(0, 1) | 171f3a | Injecting circuit gate operations into the pulse builder context is now deprecated. | pulse.cx | N/A |
| 15 | pulse.play(pulse.Constant(bell_prep.duration, 0.02), d2) | 03c2 | The ParametricPulse base class and pulses like Constant are deprecated; use corresponding SymbolicPulse with get_waveform(). | pulse.Constant | pulse.play(pulse.Constant(bell_prep.duration, 0.02).get_waveform(), d2) |