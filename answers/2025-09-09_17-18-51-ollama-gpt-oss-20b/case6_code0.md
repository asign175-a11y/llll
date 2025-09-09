| Line | Code | Scenario Id | Scenario | Artifact | Refactoring |
| :-: | :- | :-: | :- | :- | :- |
| 7 | `with pulse.build(backend) as schedule:` | * | Deprecation -> pulse.build() deprecated (optional) | pulse.build | `with pulse.ScheduleBuilder(backend) as schedule:` |