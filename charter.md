# Charter

The main goal of the asm project group is to design and implement an `asm!` macro using a syntax that we feel we can maintain, easily write, and stabilize.

The project group has the following additional goals:
* to provide a transition path for existing users of the unstable `asm!` macro.
* to ensure that the chosen `asm!` syntax is portable to different compiler backends such as LLVM, GCC, etc.
* to provide a fallback implementation on compiler backends that do not support inline assembly natively (e.g. [Cranelift][cranelift]).
* to initially support most major architectures (x86, ARM, RISC-V) with the intention of extending to other architectures in the future.

With a lower priority, the project group also intends to tackle the following secondary, future goals:
* support for module-level assembly (`global_asm!`).
* support for naked functions (`#[naked]`).

[cranelift]: https://github.com/CraneStation/cranelift/issues/444
