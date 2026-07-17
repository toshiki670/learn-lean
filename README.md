# learn-lean
Learning Lean through examples, exercises, and proofs.

## Setup

1. Install [elan](https://github.com/leanprover/elan) (the Lean toolchain manager):

   ```sh
   brew install elan-init
   ```

2. Fetch the prebuilt Mathlib cache (avoids compiling Mathlib from source):

   ```sh
   lake exe cache get
   ```

3. Build the project:

   ```sh
   lake build
   ```

The Lean version is pinned in `lean-toolchain`; elan installs it automatically on first use.

## Editor

The [official Lean 4 extension](https://marketplace.visualstudio.com/items?itemName=leanprover.lean4) for VS Code (or Cursor) is the most complete option, with a working goal/InfoView panel for interactive proof development.

A [Lean 4 extension](https://zed.dev/extensions/lean4) exists for Zed too, but it doesn't implement the InfoView yet — you get syntax highlighting and diagnostics, but no live goal state, which makes writing proofs harder. Fine for reading code; VS Code/Cursor is the better choice for actually proving things.
