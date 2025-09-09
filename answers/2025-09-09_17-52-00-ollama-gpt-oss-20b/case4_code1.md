| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :-: | :- | :-: | :- | :- | :- |
| 3 | from qiskit.tools.events import TextProgressBar | * | Deprecation -> qiskit.tools.events.TextProgressBar removed | qiskit.tools.events.TextProgressBar | Remove the import (no replacement needed). |
| 12 | TextProgressBar().update(job) | * | Deprecation -> TextProgressBar.update removed | TextProgressBar | Remove the line or replace with job status monitoring (e.g., `job.status()`). |