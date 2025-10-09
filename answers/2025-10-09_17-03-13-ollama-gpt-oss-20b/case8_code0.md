| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| ----- | ----- | ----- | ----- | ----- | ----- |
| 2 | `from qiskit.utils import QuantumInstance, algorithm_globals` | * | Deprecation -> The `QuantumInstance` class is deprecated. | `QuantumInstance` | |
| 2 | `from qiskit.utils import QuantumInstance, algorithm_globals` | * | Deprecation -> The `algorithm_globals` module is deprecated. | `algorithm_globals` | |
| 4 | `from qiskit.opflow import Z, I, X` | * | Deprecation -> The `qiskit.opflow` module is deprecated. | `Z, I, X` (from `qiskit.opflow`) | `from qiskit.quantum_info import Pauli` |
| 7 | `hamiltonian = (Z ^ I) + (X ^ X)` | * | Deprecation -> `qiskit.opflow` operators (`^`, `+`) and `OperatorBase` classes are deprecated. | `(Z ^ I) + (X ^ X)` | `hamiltonian = SparsePauliOp.from_list([('ZI', 1), ('XX', 1)])` |
| 10 | `initial_point = algorithm_globals.random.random(ansatz.num_parameters)` | * | Deprecation -> `algorithm_globals.random` is deprecated. | `algorithm_globals.random.random` | `initial_point = np.random.default_rng(seed=12345).random(ansatz.num_parameters)` |
| 13 | `quantum_instance = QuantumInstance(` | * | Deprecation -> The `QuantumInstance` class is deprecated. | `QuantumInstance` | |
| 15 | `    seed_simulator=algorithm_globals.random_seed,` | * | Deprecation -> `algorithm_globals.random_seed` is deprecated. | `algorithm_globals.random_seed` | `    seed_simulator=12345,` |
| 16 | `    seed_transpiler=algorithm_globals.random_seed` | * | Deprecation -> `algorithm_globals.random_seed` is deprecated. | `algorithm_globals.random_seed` | `    seed_transpiler=12345` |