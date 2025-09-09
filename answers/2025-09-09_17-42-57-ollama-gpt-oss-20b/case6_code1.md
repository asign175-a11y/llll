| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :-: | :- | :-: | :- | :- | :- |
| 9 | `pulse.u2(0, math.pi, 0)` | * | Deprecation -> pulse.u2() injection into builder context deprecated (optional) | pulse.u2 | `pulse.call(backend.target['u2'][(0,)])` |
| 10 | `pulse.cx(0, 1)` | * | Deprecation -> pulse.cx() injection into builder context deprecated (optional) | pulse.cx | `pulse.call(backend.target['cx'][(0, 1)])` |