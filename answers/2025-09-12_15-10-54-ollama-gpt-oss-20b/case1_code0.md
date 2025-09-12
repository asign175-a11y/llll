**In the very last Qiskit release (the first 1.x release) a number of APIs were marked deprecated that never appeared as deprecation warnings in the 0.46.x series.**  
These new “future‑breaking” deprecations were added only in the 1.x release and are *not* present in the 0.46 release notes. The most visible ones are:

| Deprecated feature (last release) | What was deprecated | Why it was not in 0.46 |
|-----------------------------------|---------------------|------------------------|
| **ScheduleBlock scoped‑parameter helpers** | `ScheduleBlock.scoped_parameters()` and `ScheduleBlock.search_parameters()` | They were only added after 0.46 to simplify pulse‑scoping; 0.46 had no concept of scoped parameters. |
| **Distribution plotting helpers** | Passing a `QuasiDistribution`, `ProbDistribution` or a distribution dict to `plot_histogram()` | In 0.46 this helper was never removed; the new `plot_distribution()` was never added. |
| **Discrete pulse library** | `constant()`, `zero()`, `square()`, `sawtooth()`, `triangle()`, `cos()`, `sin()`, `gaussian()`, `gaussian_deriv()`, `sech()`, `sech_deriv()`, `gaussian_square()`, `drag()` | The discrete pulse API was superseded by the SymbolicPulse library long before 0.46. 0.46 had no deprecation warnings for these. |
| **Fake‑backend helpers** | The old `qiskit.providers.fake_provider.FakeBackend*` classes (e.g., `FakeBackend5QV2`) and the `ConfigurableFakeBackend` class | 0.46 did not contain the new `GenericBackendV2` implementation; the deprecation notes for the legacy fakes only appeared in 1.x. |
| **Other new primitives** | The `GenericBackendV2` class in `qiskit.providers.fake_provider` and the new `basic_provider` module that replaces `basicaer` | 0.46 did not expose these modules; the deprecation guidance for BasicAer was added in 0.46 but the actual new modules were introduced only in 1.x. |

In short, the last Qiskit release (the 1.0.x line) introduced deprecations for:

* The `ScheduleBlock` scoped‑parameter helpers  
* The `plot_histogram` helper for `QuasiDistribution`/`ProbDistribution`/dicts  
* The entire discrete pulse helper functions  
* The legacy fake‑backend classes and the `ConfigurableFakeBackend`  
* The new `GenericBackendV2` and `basic_provider` modules (replacing `basicaer`)

None of these were part of the deprecation warnings or features in the 0.46.0 release.