| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :-: | :- | :-: | :- | :- | :- |
| 3 | `from qiskit.tools.events import TextProgressBar` | * | Deprecation -> qiskit.tools.events.TextProgressBar removed (optional) | qiskit.tools.events.TextProgressBar | Remove this import; it is no longer available in Qiskit 0.46.0. |
| 12 | `TextProgressBar().update(job)` | * | Deprecation -> qiskit.tools.events.TextProgressBar removed (optional) | qiskit.tools.events.TextProgressBar | Replace with job‑status polling or simply remove this line, as the progress bar is no longer provided. |