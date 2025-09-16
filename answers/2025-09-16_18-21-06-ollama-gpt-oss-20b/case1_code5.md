```markdown
| Line | Code | Scenario ID | Scenario | Artifact | Refactoring |
| :--: | :--- | :---------: | :------- | :------- | :---------- |
| 8 | `from qiskit import Aer` | e012 | Deprecated qiskit.providers.basicaer module; migrate to qiskit.providers.basic_provider. | `qiskit.providers.basicaer` | ```python\nfrom qiskit.providers.basic_provider import BasicProvider\nprovider = BasicProvider()\nbackend = provider.get_backend(\"sim_name\")\n``` |
| 9 | `backend = Aer.get_backend('aer_simulator')` | e012 | Deprecated qiskit.providers.basicaer module; migrate to qiskit.providers.basic_provider. | `qiskit.providers.basicaer` | ```python\nfrom qiskit.providers.basic_provider import BasicProvider\nprovider = BasicProvider()\nbackend = provider.get_backend(\"sim_name\")\n``` |
```