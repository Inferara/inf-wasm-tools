<div align="center">
  <h1><code>inf-wast</code></h1>

<strong><a href="https://inferara.com/">Inferara</a> fork of Bytecode Alliance project</strong>

  <p>
    <strong>A Rust parser for the <a href="https://webassembly.github.io/spec/core/text/index.html">WebAssembly Text Format (WAT)</a>. Extended with <a href="https://www.inferara.com/en/papers/specifying-algorithms-using-non-deterministic-computations/">Inference non-deterministic instructions</a>.</strong>
  </p>

  <p>
    <a href="https://crates.io/crates/inf-wast"><img src="https://img.shields.io/crates/v/inf-wast.svg?style=flat-square" alt="Crates.io version" /></a>
    <a href="https://crates.io/crates/inf-wast"><img src="https://img.shields.io/crates/d/inf-wast.svg?style=flat-square" alt="Download" /></a>
  </p>

</div>

## Inference non-deterministic instructions

This repository extends the WebAssembly Text Format (WAT) with non-deterministic instructions. These instructions are used to specify algorithms in more general way to be able to compile the source code targeting proof assistants like [Rocq](https://rocq-prover.org/) or [Lean](https://lean-lang.org/).

More information about Inference can be found in the official [Inference language spec](https://github.com/Inferara/inference-language-spec) and on the [Inferara website](https://www.inferara.com).

### Block instructions

| Instruction | WAT syntax | Binary representation | Description |
| --- | --- | --- | --- |
| **Forall** | `(forall )` | `0xFC 0x0A` | TBD |
| **Exists** | `(exists )` | `0xFC 0x0B` | TBD |
| **Assume** | `(assume )` | `0xFC 0x0C` | TBD |
| **Unique** | `(unique )` | `0xFC 0x0D` | TBD |

### Stack instructions

WIP

## Origin

This project is a fork of the [wast](https://github.com/bytecodealliance/wasm-tools/tree/main/crates/wast).

## License

This project inherits the license from the original project, which is [Apache-2.0_WITH_LLVM-exception](./LICENSE-Apache-2.0_WITH_LLVM-exception).