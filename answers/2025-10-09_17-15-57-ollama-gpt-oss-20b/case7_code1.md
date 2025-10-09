| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| ----- | ----- | ----- | ----- | ----- | ----- |
| 1 | from qiskit import execute | * | Removal -> The `execute` function has been removed. | `execute` function | |
| 2 | from qiskit.test.mock import FakeVigo | * | Deprecation -> Module moved. `qiskit.test.mock` has been moved to `qiskit.providers.fake_provider`. (optional) | `qiskit.test.mock` | `from qiskit.providers.fake_provider import FakeVigo` |
| 3 | from qiskit.test.reference_circuits import ReferenceCircuits | * | Deprecation -> Module removed. `qiskit.test.reference_circuits` is an internal module. | `qiskit.test.reference_circuits` | `from qiskit import QuantumCircuit` |
| 4 | from qiskit.test.base import BaseTestCase | * | Deprecation -> Module removed. `qiskit.test.base.BaseTestCase` is an internal module. | `qiskit.test.base.BaseTestCase` | |
| 7 | qc = ReferenceCircuits.bell() | * | Deprecation -> `ReferenceCircuits` is an internal test utility. | `ReferenceCircuits.bell()` | `qc = QuantumCircuit(2, 2)\nqc.h(0)\nqc.cx(0, 1)` |
| 9 | job = execute(qc, backend, shots=1024) | * | Removal -> The `execute` function has been removed. | `execute` function | `job = backend.run(qc, shots=1024)` |
| 17 | class TestBellCircuit(BaseTestCase): | * | Deprecation -> `BaseTestCase` is an internal test utility. Use `unittest.TestCase`. | `BaseTestCase` | `class TestBellCircuit(unittest.TestCase):` |
| 20 | qc = ReferenceCircuits.bell() | * | Deprecation -> `ReferenceCircuits` is an internal test utility. | `ReferenceCircuits.bell()` | `qc = QuantumCircuit(2, 2)\nqc.h(0)\nqc.cx(0, 1)` |
| 22 | job = execute(qc, backend, shots=1024) | * | Removal -> The `execute` function has been removed. | `execute` function | `job = backend.run(qc, shots=1024)` |