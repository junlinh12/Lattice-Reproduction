# Lattice Reproduction

This repository contains a clean-room export of reproducibility
artifacts for the public Lattice project.

The original upstream source tree is not duplicated here. Instead,
the repository records the exact upstream base revision and a small,
ordered patch series containing the local reproduction changes.

## Contents

- `UPSTREAM.md` — upstream repository and pinned base revision
- `patches/` — ordered reproduction patches
- `docs/` — reproduction documentation
- `checksums/` — integrity metadata

## Patch application

Apply the patches in numeric order to the exact upstream base revision
documented in `UPSTREAM.md`.

Raw host logs, virtual-machine images, credentials, private keys,
host-specific absolute paths, and other local forensic artifacts are
intentionally excluded.
