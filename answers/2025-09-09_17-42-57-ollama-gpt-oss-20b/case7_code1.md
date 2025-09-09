| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :-: | :- | :-: | :- | :- | :- |
| 2 | `from qiskit.test.mock import FakeVigo` | * | Deprecation -> qiskit.test.mock module deprecated (optional) | qiskit.test.mock | `from qiskit_aer.backends.fake import FakeVigo` |
| 3 | `from qiskit.test.reference_circuits import ReferenceCircuits` | * | Deprecation -> qiskit.test.reference_circuits module deprecated (optional) | qiskit.test.reference_circuits | `from qiskit.circuit.library import BellCircuit` <br> `qc = BellCircuit()` |
| 4 | `from qiskit.test.base import BaseTestCase` | * | Deprecation -> qiskit.test.base module deprecated (optional) | qiskit.test.base | `from unittest import TestCase` <br> `class TestBellCircuit(TestCase):` |