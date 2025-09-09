| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :-: | :- | :-: | :- | :- | :- |
| 9 | `pulse.play(pulse.Constant(100, 0.5), d0)` | * | Deprecation -> pulse.Constant deprecated (optional) | pulse.Constant | `pulse.play(pulse.ConstantPulse(100, 0.5), d0)` |