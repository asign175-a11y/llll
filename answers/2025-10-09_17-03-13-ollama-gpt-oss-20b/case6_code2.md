| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| ----- | ----- | ----- | ----- | ----- | ----- |
| 2 | `from qiskit.providers.fake_provider import *` | * | Module Relocation -> The `qiskit.providers.fake_provider` module has been moved. | `qiskit.providers.fake_provider` | `from qiskit_ibm_runtime.fake_provider import *` |