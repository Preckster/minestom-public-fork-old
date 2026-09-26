# Shatterveil patches

Base: upstream tag `2026.09.12-26.2` (`aba93bdb50`). Current level: **`2026.09.12-26.2-sv.0`**.

Rules (Shatterveil design/phase-1/1.9-parallel-tick.md §6):

- One commit per patch, subject `SV-Mn: …`, listing the files it changes (Modified by Shatterveil).
- A patch stays only if it gains ≥ 3% tick time or p99, or unblocks one that does.
- Target ≤ 8 patches. On each upstream release we adopt, rebase the patch commits onto the new
  tag; drop any patch upstream merged.

| # | Patch | Files | Measured gain |
|---|---|---|---|
| — | none yet | — | — |

## Fork maintenance (not patches)

These change only fork metadata or build defaults, never Minestom's runtime code:

- `README.md`, `PATCHES.md`: this documentation.
- `build-src/.../minestom.java-library.gradle.kts`: default version `2026.09.12-26.2-sv.0`
  instead of `dev` when `MINESTOM_VERSION` is unset, so the jar and `Git.version()` name the
  fork build.
