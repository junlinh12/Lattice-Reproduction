# Applying the Reproduction Patches

The patch series is intended for the exact upstream base revision:

`05664a26af63e0898828a37b4387efc188388dbf`

A generic workflow is:

    git clone https://github.com/LatticeEnclave/Lattice.git Lattice-upstream
    git -C Lattice-upstream checkout 05664a26af63e0898828a37b4387efc188388dbf

    for patch in Lattice-Reproduction/patches/*.patch
    do
        git -C Lattice-upstream apply --check "../$patch" || exit 1
        git -C Lattice-upstream apply "../$patch" || exit 1
    done

The patches are numbered so ordinary lexical ordering gives the required
application order.

## Expected modified paths

After all four patches are applied, the affected paths are:

    Cargo.toml
    platform/qemu-virt/firmware.mk
    crates/sm/src/init.rs

No raw logs, host configuration, credentials, or build output are
required by the patch series itself.
