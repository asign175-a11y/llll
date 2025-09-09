| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :-: | :- | :-: | :- | :- | :- |
| 8 | `with pulse.build(backend) as bell_prep:` | * | Deprecation -> pulse.build deprecated | pulse.build |  |
| 9 | `    pulse.u2(0, math.pi, 0)` | * | Deprecation -> pulse.u2 deprecated | pulse.u2 |  |
| 10 | `    pulse.cx(0, 1)` | * | Deprecation -> pulse.cx deprecated | pulse.cx |  |
| 12 | `with pulse.build(backend) as decoupled_bell_prep_and_measure:` | * | Deprecation -> pulse.build deprecated | pulse.build |  |
| 13 | `    with pulse.align_right():` | * | Deprecation -> pulse.align_right deprecated | pulse.align_right |  |
| 14 | `        pulse.call(bell_prep)` | * | Deprecation -> pulse.call deprecated | pulse.call |  |