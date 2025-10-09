| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
|---|---|---|---|---|---|
| 8 | from qiskit import Aer | QiskitAer_0_12_Aer_import | Deprecation -> Importing Aer directly for backends is no longer recommended. | Aer | from qiskit_aer import AerSimulator |
| 9 | backend = Aer.get_backend('aer_simulator') | QiskitAer_0_12_Aer_get_backend_deprecated | Deprecation -> `Aer.get_backend()` is deprecated. | Aer.get_backend | backend = AerSimulator() |
| 11 | from qiskit import execute | Qiskit_0_46_execute_import_deprecated | Deprecation -> Importing `execute` function is deprecated. | execute | |
| 12 | job = execute(qc, backend, shots=1000) | Qiskit_0_46_execute_function_deprecated | Deprecation -> The `execute` function is deprecated. | execute | job = backend.run(qc, shots=1000) |
| 17 | from qiskit.algorithms import VQE | Qiskit_0_46_VQE_module_moved | Module Restructuring -> `VQE` moved to `qiskit.algorithms.minimum_eigensolvers`. | VQE | from qiskit.algorithms.minimum_eigensolvers import VQE |
| 19 | from qiskit import SPSA | Qiskit_0_46_SPSA_module_moved | Module Restructuring -> `SPSA` optimizer moved to `qiskit.algorithms.optimizers`. | SPSA | from qiskit.algorithms.optimizers import SPSA |
| 20 | vqe = VQE(TwoLocal(rotation_blocks="ry", entanglement_blocks="cz"), SPSA()) | Qiskit_0_46_VQE_module_moved | Module Restructuring -> `VQE` class now imported from `qiskit.algorithms.minimum_eigensolvers`. | VQE | |
| 20 | vqe = VQE(TwoLocal(rotation_blocks="ry", entanglement_blocks="cz"), SPSA()) | Qiskit_0_46_SPSA_module_moved | Module Restructuring -> `SPSA` class now imported from `qiskit.algorithms.optimizers`. | SPSA | |