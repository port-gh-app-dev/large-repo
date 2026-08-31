# Command Injection Rules

- Avoid shell execution when a native library/API exists.
- If process execution is required, use argument arrays (no shell interpolation).
- Never concatenate untrusted input into commands.
- Denylist approaches are insufficient; use strict allowlists for commands and arguments.
- Validate and normalize file paths, flags, and option values before execution.
- Drop privileges and run subprocesses with least-privilege service accounts.
- Set execution timeouts and output size limits for all subprocess calls.
- Isolate execution in containers/sandboxes for risky workflows.
- Log command invocations safely (redact secrets, avoid logging raw untrusted input).
- Add tests for payloads using separators, subshells, pipes, and escape sequences.
