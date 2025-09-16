| Line | Code | Scenario ID | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
| 2 | `from qiskit.providers.fake_provider import *` | b0ee | Deprecated - fake provider moved to qiskit-ibm-runtime | qiskit.providers.fake_provider | `from qiskit_ibm_runtime.fake_provider import *` |
| 4 | `backend = FakeOpenPulse2Q()` | b0ee | Deprecated - fake provider moved to qiskit-ibm-runtime | qiskit.providers.fake_provider.FakeOpenPulse2Q | `from qiskit_ibm_runtime.fake_provider import FakeOpenPulse2Q` |