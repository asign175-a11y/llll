| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| ----- | ----- | ----- | ----- | ----- | ----- |
| 8 | `job = estimator.run([psi1], [H1], [theta1])` | * | Deprecation -> The Estimator.run() method signature has changed. | `Estimator.run` | `job = estimator.run([(psi1, H1, theta1)])` |