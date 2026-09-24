# Reproduction Status

## Scope

This repository records the publication-safe artifacts produced while
reproducing the public Lattice project.

It is intentionally a clean-room artifact repository rather than a
copy of the complete upstream source tree.

## Source baseline

Upstream repository:

`https://github.com/LatticeEnclave/Lattice`

Upstream base revision:

`05664a26af63e0898828a37b4387efc188388dbf`

Local reproduction revision from which the patch series was exported:

`7d0fd2d04337a050418ca0f059bd6e931ab2641f`

## Current validated state

The current reproduction workflow has reached a validated minimal
enclave functional-loop checkpoint.

The four local reproduction changes have also been exported as an
ordered patch series and independently replayed from the exact upstream
base revision. After replay, all three modified source files matched the
corresponding files at the local reproduction revision byte-for-byte by
SHA-256 comparison.

This first repository snapshot should not be interpreted as a claim
that every experiment or evaluation result from the paper has already
been reproduced.

## Publication boundary

The following material is intentionally not included:

- raw host execution logs
- raw QEMU logs
- virtual-machine images
- memory images or core dumps
- SSH credentials or private keys
- host-specific absolute paths
- machine-specific identifiers
- local untracked build artifacts

Detailed raw evidence remains outside this repository.
