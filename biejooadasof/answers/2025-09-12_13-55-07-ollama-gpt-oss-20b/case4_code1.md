| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
| 3 | from qiskit.tools.events import TextProgressBar | * | Importing from qiskit.tools.events is deprecated | qiskit.tools.events | Remove the import; replace with a custom progress bar or omit progress updates. |
| 12 | TextProgressBar().update(job) | * | Use of TextProgressBar is deprecated | TextProgressBar | Remove the call; replace with an alternative progress display or no progress bar. |