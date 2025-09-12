| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
| 11 | from qiskit import execute | * | Import -> execute moved to qiskit.compiler (mandatory) | qiskit.execute | from qiskit.compiler import execute |
| 12 | job = execute(qc, backend, shots=1000) | * | Usage -> execute expects list of circuits (mandatory) | qiskit.execute | job = execute([qc], backend, shots=1000) |
| 14 | from qiskit.tools.visualization import plot_histogram | * | Deprecation -> qiskit.tools.visualization.plot_histogram deprecated (mandatory) | qiskit.tools.visualization | from qiskit.visualization import plot_histogram |
| 19 | from qiskit import SPSA | * | Import -> SPSA moved to qiskit.algorithms.optimizers (mandatory) | qiskit.SPSA | from qiskit.algorithms.optimizers import SPSA |