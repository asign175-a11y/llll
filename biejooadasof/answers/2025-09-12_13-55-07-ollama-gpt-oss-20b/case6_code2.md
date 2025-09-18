| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
| 2 | `from qiskit.providers.fake_provider import *` | `*` | Import -> import * from fake_provider is deprecated | import * | `from qiskit.providers.fake_provider import FakeOpenPulse2Q` |
| 8 | `with pulse.build() as pulse_prog:` | `*` | Deprecated -> pulse.build context manager removed | pulse.build context manager | `pulse_prog = pulse.build()` |