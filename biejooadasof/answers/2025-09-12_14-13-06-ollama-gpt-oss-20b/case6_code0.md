| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
| 2 | from qiskit.pulse import Gaussian | * | Import -> missing MeasureChannel import | MeasureChannel | from qiskit.pulse import MeasureChannel |
| 12 | pulse.measure(0) | * | Measurement -> pulse.measure() requires a MeasurementChannel argument | pulse.measure() | pulse.measure(0, pulse.MeasureChannel(0)) |