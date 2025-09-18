| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
| 8 | from qiskit import Aer | * | Deprecation -> Aer provider import changed | Aer | from qiskit.providers.aer import AerSimulator |
| 9 | backend = Aer.get_backend('aer_simulator') | * | Deprecation -> Aer simulator instantiation changed | AerSimulator | backend = AerSimulator() |
| 14 | from qiskit.tools.visualization import plot_histogram | * | Deprecation -> plot_histogram import path changed | plot_histogram | from qiskit.visualization import plot_histogram |
| 19 | from qiskit import SPSA | * | Deprecation -> SPSA import moved to optimizers | SPSA | from qiskit.algorithms.optimizers import SPSA |