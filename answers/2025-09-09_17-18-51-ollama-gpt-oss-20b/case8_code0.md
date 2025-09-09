| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :-: | :- | :-: | :- | :- | :- |
| 1 | `from qiskit import Aer` | * | Deprecation -> from qiskit import Aer deprecated (optional) | Aer | `from qiskit.providers.aer import Aer` |
| 4 | `from qiskit.opflow import Z, I, X` | * | Deprecation -> qiskit.opflow operators deprecated (optional) | qiskit.opflow | `from qiskit.opflow import PauliOp` (use PauliOp('ZI'), PauliOp('XX')) |
| 10 | `initial_point = algorithm_globals.random.random(ansatz.num_parameters)` | * | Deprecation -> algorithm_globals.random.random deprecated (optional) | algorithm_globals.random | `rng = np.random.default_rng(algorithm_globals.random_seed); initial_point = rng.random(ansatz.num_parameters)` |