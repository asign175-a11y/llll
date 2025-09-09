| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :-: | :- | :-: | :- | :- | :- |
| 14 | `from qiskit.tools.visualization import plot_histogram` | * | Deprecation -> plot_histogram function deprecated | qiskit.tools.visualization.plot_histogram | `from qiskit.visualization import plot_histogram` |
| 19 | `from qiskit import SPSA` | * | Deprecation -> SPSA class deprecated | qiskit.SPSA | `from qiskit.algorithms.optimizers import SPSA` |
| 11 | `from qiskit import execute` | * | Deprecation -> execute function deprecated | qiskit.execute | `from qiskit import execute` (no change, but keep for reference) |