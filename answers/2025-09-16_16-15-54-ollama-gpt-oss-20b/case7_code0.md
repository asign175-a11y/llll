| Line | Code | Scenario ID | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
| 1 | from mylib import getJob, getCount | | | | |
| 2 | from qiskit.test.mock import FakeVigo | 4ebcee31-18ee-4469-a170-82f4fb0db0ee | DEPRECATION - FakeVigo replaced by GenericBackendV2 | qiskit.providers.fake_provider | from qiskit.providers.fake_provider import GenericBackendV2 |
| 3 | from qiskit.test.reference_circuits import ReferenceCircuits | | | | |