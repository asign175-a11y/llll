**Query for Retriever**

Find migration rules to update the following Qiskit code to version 0.46.0.

```python
{"data":"from qiskit import QuantumCircuit, QuantumRegister\nfrom qiskit.extensions import HGate, XGate, Initialize\nfrom qiskit.extensions import Barrier\nfrom qiskit.extensions import UnitaryGate\nimport numpy as np\n\nqr = QuantumRegister(3)\nqc = QuantumCircuit(qr)\n\nqc.append(HGate(), [qr[0]])\nqc.append(XGate(), [qr[1]])\n\ncustom_matrix = np.array([[0, 1], [1, 0]])\ncustom_gate = UnitaryGate(custom_matrix, label=\"Custom\")\nqc.append(custom_gate, [qr[2]])\n\npsi = [1/np.sqrt(2), 1/np.sqrt(2)]\ninit_gate = Initialize(psi)\nqc.append(init_gate, [qr[0]])\n\nqc.append(Barrier(3), [qr[0], qr[1], qr[2]])\nprint(qc.draw())"}
```

---

**Output Table**

| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
| 2 | `from qiskit.extensions import HGate, XGate, Initialize` | * | Deprecation -> HGate, XGate, Initialize imported from qiskit.extensions (optional) | qiskit.extensions.HGate, qiskit.extensions.XGate, qiskit.extensions.Initialize | `from qiskit.circuit.library import HGate, XGate, Initialize` |
| 3 | `from qiskit.extensions import Barrier` | * | Deprecation -> Barrier imported from qiskit.extensions (optional) | qiskit.extensions.Barrier | `from qiskit.circuit.library import Barrier` |
| 4 | `from qiskit.extensions import UnitaryGate` | * | Deprecation -> UnitaryGate imported from qiskit.extensions (optional) | qiskit.extensions.UnitaryGate | `from qiskit.circuit.library import UnitaryGate` |
| 18 | `qc.append(init_gate, [qr[0]])` | * | Usage of Initialize via append (optional) | qiskit.extensions.Initialize | `qc.initialize(psi, [qr[0]])` (remove `init_gate` variable) |
| 20 | `qc.append(Barrier(3), [qr[0], qr[1], qr[2]])` | * | Usage of Barrier via append (optional) | qiskit.extensions.Barrier | `qc.barrier([qr[0], qr[1], qr[2]])` (or `qc.barrier(qr)`) |
