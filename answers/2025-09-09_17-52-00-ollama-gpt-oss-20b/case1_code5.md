| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :-: | :- | :-: | :- | :- | :- |
| 8 | `from qiskit import Aer` | * | Deprecation -> import Aer from qiskit deprecated (optional) | qiskit.Aer | `from qiskit.providers.aer import AerSimulator` |
| 9 | `backend = Aer.get_backend('aer_simulator')` | * | Deprecation -> Aer.get_backend('aer_simulator') deprecated (optional) | qiskit.Aer.get_backend | `backend = AerSimulator()` |
| 14 | `from qiskit.tools.visualization import plot_histogram` | * | Deprecation -> plot_histogram import path deprecated (optional) | qiskit.tools.visualization.plot_histogram | `from qiskit.visualization import plot_histogram` |
| 19 | `from qiskit import SPSA` | * | Deprecation -> SPSA import from qiskit deprecated (optional) | qiskit.SPSA | `from qiskit.algorithms.optimizers import SPSA` |