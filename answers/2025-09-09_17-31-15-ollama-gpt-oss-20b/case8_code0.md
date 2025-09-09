| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :-: | :- | :-: | :- | :- | :- |
| 4 | `from qiskit.opflow import Z, I, X` | * | Deprecation -> direct Pauli imports from `qiskit.opflow` (optional) | qiskit.opflow | `from qiskit.opflow import PauliOp` |
| 7 | `hamiltonian = (Z ^ I) + (X ^ X)` | * | Deprecation -> Pauli tensor product using `^` operator (optional) | qiskit.opflow.pauli.PauliOp | `hamiltonian = PauliOp('ZI') + PauliOp('XX')` |

