**Query for Retriever**

Find migration rules to update the following Qiskit code to version 0.46.0.

```python
{"data":"from qiskit import QuantumCircuit
from utils import createBackendAndrunJob
from qiskit.tools.events import TextProgressBar

qc = QuantumCircuit(2)
qc.h(0)
qc.cx(0, 1)
qc.measure_all()

job = createBackendAndrunJob()

TextProgressBar().update(job)
result = job.result()
counts = result.get_counts()"}
```

---

**Output Table**

| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
| 3 | `from qiskit.tools.events import TextProgressBar` | 97ea4954-e55d-45cf-8738-2763f068e974 | Deprecation -> qiskit.tools.events.TextProgressBar deprecated (optional) | qiskit.tools.events | `from qiskit.providers.utils import ProgressBar`<br>`ProgressBar().update(job)` |
| 9 | `qc.measure_all()` | * | Deprecation -> QuantumCircuit.measure_all() deprecated (optional) | QuantumCircuit.measure_all | `qc.measure(range(2), range(2))` |

(If any of the above changes are not required for your exact target version, you can omit them; the optional flag indicates they are not mandatory.)