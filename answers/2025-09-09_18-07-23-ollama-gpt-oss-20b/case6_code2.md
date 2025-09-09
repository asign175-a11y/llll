| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
| 2 | `from qiskit.providers.fake_provider import *` | * | Deprecation -> wildcard imports are not allowed (optional) | Imports | `from qiskit.providers.fake_provider import FakeOpenPulse2Q` |