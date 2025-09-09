| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :-: | :- | :-: | :- | :- | :- |
| 1 | from mylib import getJob, getCount | * |  |  |  |
| 2 | from qiskit.test.mock import FakeVigo | * |  |  |  |
| 3 | from qiskit.test.reference_circuits import ReferenceCircuits | * |  |  |  |
| 5 | qc = ReferenceCircuits.bell() | * |  |  |  |
| 6 | backend = FakeVigo() | * |  |  |  |
| 8 | job = getJob(qc, backend) | * |  |  |  |
| 9 | counts = getCount(job) | * |  |  |  |
| 11 | print("Resultados del circuito Bell:") | * |  |  |  |
| 12 | print(counts) | * |  |  |  |