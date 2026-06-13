# outpost-manifest

Desired-state manifest read by every `outpost-supervisor` instance in the
fleet. Edits propagate to operator machines on their next reconciliation
cycle (~5 min).

## Format

```yaml
schema_version: 1
formulae:
  - <brew-formula-name>           # homebrew-core
  - <tap>/<repo>/<formula-name>   # external tap
```

See the [outpost-supervisor design spec](https://github.com/dragonflyic/outpost/blob/main/docs/superpowers/specs/2026-06-13-outpost-supervisor-design.md) for semantics.
