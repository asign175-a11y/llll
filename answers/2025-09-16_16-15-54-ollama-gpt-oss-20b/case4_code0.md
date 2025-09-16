| Line | Code | Scenario ID | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
| 1 | from qiskit import QuantumCircuit                                    # type: ignore |  |  |  |  |
| 2 | from mylib import execute, getBackend                                # type: ignore |  |  |  |  |
| 3 | from qiskit.tools.visualization import plot_histogram                   # type: ignore |  |  |  | from qiskit.visualization import plot_histogram |
| 4 | from qiskit.tools.monitor import job_monitor                        # type: ignore |  |  |  | from qiskit.providers.utils import job_monitor |
| 5 | import matplotlib.pyplot as plt |  |  |  |  |
| 7 | qc = QuantumCircuit(2, 2) |  |  |  |  |
| 8 | qc.h(0) |  |  |  |  |
| 9 | qc.cx(0, 1) |  |  |  |  |
| 10 | qc.measure([0, 1], [0, 1]) |  |  |  |  |
| 12 | print("Circuito cuántico:") |  |  |  |  |
| 13 | print(qc.draw(output='text')) |  |  |  |  |
| 15 | simulator = getBackend.get_backend('statevector_simulator') |  |  |  |  |
| 16 | result = execute(qc, simulator).result() |  |  |  |  |
| 17 | statevector = result.get_statevector() |  |  |  |  |
| 19 | backend = getBackend.get_backend('qasm_simulator') |  |  |  |  |
| 20 | job = execute(qc, backend, shots=1000) |  |  |  |  |
| 22 | job_monitor(job) |  |  |  |  |
| 23 | counts = job.result().get_counts(qc) |  |  |  |  |
| 24 | plot_histogram(counts) |  |  |  |  |