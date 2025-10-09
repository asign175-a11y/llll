| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| ----- | ----- | ----- | ----- | ----- | ----- |
| 10 | `from qiskit import Aer` | `*` | Structural Change -> `AerSimulator` is now imported directly from `qiskit_aer`. | `from qiskit import Aer` | `from qiskit_aer import AerSimulator` |
| 11 | `backend = Aer.get_backend('aer_simulator')` | `qiskit-aer-0.12.0-0.45.0-aer_get_backend_deprecated` | Deprecation -> The `Aer.get_backend()` function is deprecated. | `Aer.get_backend` | `backend = AerSimulator()` |
| 18 | `qc.draw(output='mpl')` | `qiskit-terra-0.24.0-0.44.0-quantumcircuit_draw_output_mpl_deprecated` | Deprecation -> The `output` parameter in `QuantumCircuit.draw()` for 'mpl' is deprecated. | `QuantumCircuit.draw(output='mpl')` | `qc.draw('mpl')` |