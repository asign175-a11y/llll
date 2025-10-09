| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
|---|---|---|---|---|---|
| 3 | `from qiskit.tools.events import TextProgressBar` | * | Deprecation and Removal -> `qiskit.tools.events.TextProgressBar` is removed. | `qiskit.tools.events.TextProgressBar` | `from qiskit_ibm_provider.job import text_progressbar` |
| 12 | `TextProgressBar().update(job)` | * | Usage Change -> The method for displaying a progress bar for Qiskit jobs has changed. | `TextProgressBar().update(job)` | `job.wait_for_final_state(callback=text_progressbar)` |