| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| ----- | ----- | ----- | ----- | ----- | ----- |
| 3 | `from qiskit.tools.events import TextProgressBar` | * | Deprecation -> The `TextProgressBar` class has been moved and deprecated. | `TextProgressBar` | `from qiskit.tools.monitor import job_monitor` |
| 11 | `TextProgressBar().update(job)` | * | Deprecation -> The `TextProgressBar` class is deprecated. | `TextProgressBar().update()` | `job_monitor(job)` |