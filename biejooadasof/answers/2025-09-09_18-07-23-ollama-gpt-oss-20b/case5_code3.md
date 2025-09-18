Find migration rules to update the following Qiskit code to version 0.46.0.

```python
{"data":"from qiskit import QuantumCircuit\nfrom qiskit.extensions import UnitaryGate\nfrom qiskit.extensions.exceptions import ExtensionError\nimport numpy as np\n\ndef apply_custom_gate(qc, matrix, qubit):\n    try:\n        if matrix.shape[0] != matrix.shape[1]:\n            raise ExtensionError(\"La matriz debe ser cuadrada\")\n            \n        custom_gate = UnitaryGate(matrix)\n        qc.append(custom_gate, [qubit])\n        \n    except ExtensionError as e:\n        print(f\"Error en extensión: {e}\")\n\nqc = QuantumCircuit(1)\n\nprint(\"\\nMatriz no cuadrada...\")\napply_custom_gate(qc, np.array([[1, 0, 0], [0, 1, 0]]), 0)"}
```