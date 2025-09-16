| Line | Code | Scenario ID | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
| 3 | `from qiskit.providers.fake_provider import FakeOpenPulse3Q` | b0ee | Deprecation - The qiskit.providers.fake_provider module has been migrated to qiskit-ibm-runtime. | `qiskit.providers.fake_provider.FakeOpenPulse3Q` | `from qiskit_ibm_runtime.fake_provider import FakeProvider` |
| 5 | `backend = FakeOpenPulse3Q()` | b0ee | Deprecation - The qiskit.providers.fake_provider module has been migrated to qiskit-ibm-runtime. | `qiskit.providers.fake_provider.FakeOpenPulse3Q` | `backend = GenericBackendV2(num_qubits=3)` |
| 9 | `pulse.u2(0, math.pi, 0)` | a747 | Deprecated gate function u2. | `pulse.u2` |  |
| 10 | `pulse.cx(0, 1)` | a747 | Deprecated gate function cx. | `pulse.cx` |  |