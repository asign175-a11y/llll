| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :-: | :- | :-: | :- | :- | :- |
| 3 | `from qiskit.tools.visualization import plot_histogram                   # type: ignore` | * | Deprecation -> qiskit.tools.visualization module deprecated (optional) | qiskit.tools.visualization | `from qiskit.visualization import plot_histogram` |
| 4 | `from qiskit.tools.monitor import job_monitor                        # type: ignore` | * | Deprecation -> qiskit.tools.monitor module deprecated (optional) | qiskit.tools.monitor | `from qiskit.providers.jobmonitor import job_monitor` |