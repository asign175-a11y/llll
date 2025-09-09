| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :-: | :- | :-: | :- | :- | :- |
| 8 | `from qiskit import Aer` | * | Deprecation -> import Aer from qiskit deprecated | qiskit import Aer | `from qiskit_aer import Aer` |
| 14 | `from qiskit.tools.visualization import plot_histogram` | * | Deprecation -> import plot_histogram from qiskit.tools.visualization deprecated | qiskit.tools.visualization plot_histogram | `from qiskit.visualization import plot_histogram` |
| 19 | `from qiskit import SPSA` | * | Deprecation -> import SPSA from qiskit deprecated | qiskit import SPSA | `from qiskit.algorithms.optimizers import SPSA` |