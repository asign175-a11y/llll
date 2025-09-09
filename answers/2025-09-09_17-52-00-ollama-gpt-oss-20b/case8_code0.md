| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :-: | :- | :-: | :- | :- | :- |
| 4 | `from qiskit.opflow import Z, I, X` | \* | Deprecation -> qiskit.opflow module removed (optional) | qiskit.opflow | `from qiskit.opflow import Pauli, PauliSumOp\nZ = Pauli('Z'); I = Pauli('I'); X = Pauli('X')` |
| 10 | `initial_point = algorithm_globals.random.random(ansatz.num_parameters)` | \* | Deprecation -> algorithm_globals.random removed (optional) | algorithm_globals.random | `initial_point = np.random.random(ansatz.num_parameters)` |
| 16 | `seed_simulator=algorithm_globals.random_seed` | \* | Deprecation -> algorithm_globals.random_seed removed (optional) | algorithm_globals.random_seed | `seed_simulator=42` |
| 17 | `seed_transpiler=algorithm_globals.random_seed` | \* | Deprecation -> algorithm_globals.random_seed removed (optional) | algorithm_globals.random_seed | `seed_transpiler=42` |