# Reproduction Patch Series

The patches in `patches/` must be applied in numeric order.

| Order | Source commit | Repository-relative path | Purpose |
|---|---|---|---|
| 0001 | `29b1754ba12103b52b083ba035e0a38bf18c503d` | `Cargo.toml` | Remove the nonexistent `tests` workspace member. |
| 0002 | `7aa0a6b77f9e67101caaeda5d365fdaae46d83f7` | `Cargo.toml` | Exclude inactive HTEE workspace members from the active workspace. |
| 0003 | `acd48a82d74bda213efa9dc0a032726456fb7d0b` | `platform/qemu-virt/firmware.mk` | Make OpenSBI firmware-directory cleanup tolerate an absent build directory. |
| 0004 | `7d0fd2d04337a050418ca0f059bd6e931ab2641f` | `crates/sm/src/init.rs` | Extend the FDT reserved-memory region to cover SM-private memory used after the SBI region. |

## Aggregate delta

Relative to upstream base
`05664a26af63e0898828a37b4387efc188388dbf`,
the reproduction branch changes three tracked paths:

- `Cargo.toml`
- `platform/qemu-virt/firmware.mk`
- `crates/sm/src/init.rs`

The complete local delta consists of four commits.

## Untracked Cargo.lock

A locally generated `Cargo.lock` exists in the reproduction worktree,
but it is not tracked at either the upstream base or the reproduction
revision.

It is therefore excluded from this publication candidate.
