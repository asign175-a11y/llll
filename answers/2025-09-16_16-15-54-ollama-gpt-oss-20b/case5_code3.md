Find migration rules to update the following Qiskit code to version 0.46.0.



```python
{"data":"from qiskit import QuantumCircuit
from qiskit.extensions import UnitaryGate
from qiskit.extensions.exceptions import ExtensionError
import numpy as np

def apply_custom_gate(qc, matrix, qubit):
    try:
        if matrix.shape[0] != matrix.shape[1]:
            raise ExtensionError(\"La matriz debe ser cuadrada\")

        custom_gate = UnitaryGate(matrix)
        qc.append(custom_gate, [qubit])

    except ExtensionError as e:
        print(f\"Error en extensión: {e}\")

qc = QuantumCircuit(1)

print(\"\\nMatriz no cuadrada...\")
apply_custom_gate(qc, np.array([[1, 0, 0], [0, 1, 0]]), 0)"}
```

| Line | Code | Scenario ID | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
| 2 | from qiskit.extensions import UnitaryGate | 5db8be17-41de-4bf7-8281-02232d40a747 | DEPRECATION - The qiskit.extensions module is deprecated | qiskit.extensions | from qiskit.circuit.library import UnitaryGate |
| 3 | from qiskit.extensions.exceptions import ExtensionError | 5db8be17-41de-4bf7-8281-02232d40a747 | DEPRECATION - The qiskit.extensions.exceptions module is deprecated | qiskit.extensions | from qiskit.exceptions import ExtensionError |