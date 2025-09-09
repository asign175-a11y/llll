| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :-: | :- | :-: | :- | :- | :- |
| 5 | `qc.measure(0, 0)` | * | Deprecation -> `qc.measure` deprecated | QuantumCircuit.measure | `qc.measure([0], [0])` |
| 6 | `qc.measure(1, 1)` | * | Deprecation -> `qc.measure` deprecated | QuantumCircuit.measure | `qc.measure([1], [1])` |
| 11 | `from qiskit import execute` | * | Deprecation -> `execute()` deprecated | execute | `from qiskit import transpile, assemble` |
| 12 | `job = execute(qc, backend, shots=1000)` | * | Deprecation -> `execute()` deprecated | execute | `transpiled = transpile(qc, backend)`<br>`qobj = assemble(transpiled, backend, shots=1000)`<br>`job = backend.run(qobj)` |
| 14 | `from qiskit.tools.visualization import plot_histogram` | * | Import Migration -> `plot_histogram` moved to `qiskit.visualization` | plot_histogram | `from qiskit.visualization import plot_histogram` |
| 19 | `from qiskit import SPSA` | * | Import Migration -> `SPSA` moved to `qiskit.algorithms.optimizers` | SPSA | `from qiskit.algorithms.optimizers import SPSA` |