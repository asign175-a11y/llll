| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :-: | :- | :-: | :- | :- | :- |
| 8 | `with pulse.build(backend) as bell_prep:` | * | | | |
| 9 | `    pulse.u2(0, math.pi, 0)` | * | | | |
| 10 | `    pulse.cx(0, 1)` | * | | | |
| 14 | `        pulse.call(bell_prep)` | * | | | |
| 16 | `        pulse.barrier(0, 1, 2)` | * | | | |