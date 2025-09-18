Find migration rules to update the following Qiskit code to version 0.46.0.

```python
from qiskit.qasm import Qasm
from utils import getJob, getBackend

qasm_file="C:/qasm_file.qasm"
circuit2 = Qasm(filename=qasm_file)
program2 = circuit2.parse()
qc2 = program2.get_circuit()

simulator = getBackend()
job = getJob(qc2)
result = job.result()
counts = result.get_counts()
print(counts)
```

| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
|:---:|:-----|:-----------:|:--------|:--------|:------------|
| 1 | from qiskit.qasm import Qasm | * | Deprecation -> Qasm class removed | qiskit.qasm.Qasm | Replace with `from qiskit.qasm import parse_qasm` |
| 4 | circuit2 = Qasm(filename=qasm_file) | * | Deprecation -> Qasm class constructor removed | qiskit.qasm.Qasm | Replace with `circuit2 = parse_qasm(qasm_file)` |
| 5 | program2 = circuit2.parse() | * | Deprecation -> Qasm.parse() method removed | qiskit.qasm.Qasm | Remove this line; use `circuit2` directly |
| 6 | qc2 = program2.get_circuit() | * | Deprecation -> Qasm.get_circuit() method removed | qiskit.qasm.Qasm | Replace with `qc2 = circuit2` |