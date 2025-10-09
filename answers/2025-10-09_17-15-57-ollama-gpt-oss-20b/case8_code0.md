| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
|---|---|---|---|---|---|
| 2 | `from qiskit.utils import QuantumInstance, algorithm_globals` | * | Deprecation -> `QuantumInstance` class is deprecated. | `QuantumInstance` | |
| 2 | `from qiskit.utils import QuantumInstance, algorithm_globals` | * | Deprecation -> `algorithm_globals` object is deprecated. | `algorithm_globals` | |
| 4 | `from qiskit.opflow import Z, I, X` | * | Deprecation -> `qiskit.opflow` module is deprecated. | `Z, I, X` | |
| 7 | `hamiltonian = (Z ^ I) + (X ^ X)` | * | Deprecation -> Operators from `qiskit.opflow` are deprecated. | `Z, I, X` (operators) | `hamiltonian = SparsePauliOp.from_list([("ZI", 1), ("XX", 1)])` |
| 10 | `initial_point = algorithm_globals.random.random(ansatz.num_parameters)` | * | Deprecation -> `algorithm_globals.random` is deprecated. | `algorithm_globals.random` | `initial_point = np.random.rand(ansatz.num_parameters)` |
| 13 | `quantum_instance = QuantumInstance(` | * | Deprecation -> `QuantumInstance` class is deprecated. | `QuantumInstance` | `estimator = Estimator(` |
| 14 | `    backend,` | * | Deprecation -> `backend` parameter of `QuantumInstance` is deprecated in the context of primitives. | `backend` | |
| 15 | `    shots=1024,` | * | Deprecation -> `shots` parameter of `QuantumInstance` moved to primitive options. | `shots` | `    options={"shots": 1024,` |
| 16 | `    seed_simulator=algorithm_globals.random_seed,` | * | Deprecation -> `algorithm_globals.random_seed` is deprecated; `seed_simulator` moved to primitive options. | `algorithm_globals.random_seed`, `seed_simulator` | `    "seed_simulator": 42,` |
| 17 | `    seed_transpiler=algorithm_globals.random_seed` | * | Deprecation -> `algorithm_globals.random_seed` is deprecated; `seed_transpiler` moved to primitive options. | `algorithm_globals.random_seed`, `seed_transpiler` | `    "seed_transpiler": 42}` |
| 18 | `)` | * | Deprecation -> `QuantumInstance` call termination. | `)` | `)` |