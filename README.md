# Minestom — Shatterveil fork

This is **Shatterveil's fork** of [Minestom](https://github.com/Minestom/Minestom), used by the
Shatterveil game server (`Preckster/mcrpg`) as a git submodule and Gradle composite build.

- **Upstream base:** tag `2026.09.12-26.2` (commit `aba93bdb5096179bd66dc35c9849d9f0bacdc17e`).
- **Branch:** `shatterveil` (the default branch `master` mirrors upstream and is not used).
- **Version scheme:** `2026.09.12-26.2-sv.N` — the upstream release plus our patch level, so
  logs show which build runs. `sv.0` means the plain upstream code.
- **Patches:** none yet. Every patch is one commit with the subject `SV-Mn: …` and is listed,
  with its measured gain, in [`PATCHES.md`](PATCHES.md).

For Minestom itself (API, docs, community) see the upstream repository and
<https://minestom.net>.

## Licence

Minestom is licensed under the Apache License 2.0; see [`LICENSE`](LICENSE), which this fork
keeps unchanged. Files changed by Shatterveil are listed per patch in `PATCHES.md`
("Modified by Shatterveil").
