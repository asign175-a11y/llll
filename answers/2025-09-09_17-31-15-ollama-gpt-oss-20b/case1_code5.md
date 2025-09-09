| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :-: | :- | :-: | :- | :- | :- |
| 14 | `from qiskit.tools.visualization import plot_histogram` | * | Deprecation -> qiskit.tools.visualization module deprecated (optional) | qiskit.tools.visualization | `from qiskit.visualization import plot_histogram` |
| 19 | `from qiskit import SPSA` | * | Deprecation -> qiskit.SPSA import deprecated (optional) | qiskit.SPSA | `from qiskit.algorithms.optimizers import SPSA` |
| 8 | `from qiskit import Aer` | * | Deprecation -> qiskit.Aer import deprecated (optional) | qiskit.Aer | `from qiskit.providers.aer import AerSimulator as Aer` |