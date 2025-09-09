| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :-: | :- | :-: | :- | :- | :- |
| 8 | `from qiskit import Aer` | * | Deprecation -> from qiskit import Aer deprecated (optional) | `qiskit.Aer` | `from qiskit_aer import Aer` |
| 14 | `from qiskit.tools.visualization import plot_histogram` | * | Deprecation -> from qiskit.tools.visualization import plot_histogram deprecated (optional) | `qiskit.tools.visualization.plot_histogram` | `from qiskit.visualization import plot_histogram` |
| 19 | `from qiskit import SPSA` | * | Deprecation -> from qiskit import SPSA deprecated (optional) | `qiskit.SPSA` | `from qiskit.algorithms.optimizers import SPSA` |