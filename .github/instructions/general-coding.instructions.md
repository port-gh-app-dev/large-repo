# General Coding Instructions

- Favor clarity and correctness over cleverness.
- Make small, focused changes with minimal blast radius.
- Reuse existing abstractions and patterns before introducing new ones.
- Validate all untrusted input at boundaries.
- Handle errors explicitly with actionable messages and safe fallbacks.
- Avoid shared mutable state unless synchronization is guaranteed.
- Write deterministic, isolated tests for changed behavior.
- Maintain backward compatibility unless a breaking change is intentional and documented.
- Optimize only when measured data indicates a bottlenecks.
- Keep dependencies minimal and updated; avoid unnecessary additions.
