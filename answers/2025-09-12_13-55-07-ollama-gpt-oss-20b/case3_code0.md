Find migration rules to update the following Qiskit code to version 0.46.0.

```python
{"data":"from qiskit import qasm\nfrom utils import getJob, getBackend\n\nqasm_str = \"\"\"\nOPENQASM 2.0;\ninclude \"qelib1.inc\";\nqreg q[2];\ncreg c[2];\nh q[0];\ncx q[0], q[1];\nmeasure q -> c;\n\"\"\"\ncircuit1 = qasm.Qasm(data=qasm_str)\nprogram1 = circuit1.parse()\nqc1 = program1.get_circuit()\n\nsimulator = getBackend()\njob = getJob(qc1)\nresult = job.result()\ncounts = result.get_counts()\nprint(counts)"}
```