# Freelang

After a brief period as an open-source project, Freelang is now closed source.

Freelang is an internal project of DOSAYGO. It is a proprietary, special-purpose compiler and language suitable for AI and humans to design and generate critical applications.

The source code is not publicly available.

# How it started, how it's going

Freelang started on November 18, 2025 as an audacious 10,000-line experiment: could a small JavaScript compiler turn a strange, principled language directly into native x86-64—with no LLVM, VM, JIT, or libc?

Eight months and 1,193 commits later, it has become a real systems stack:

  - Native Linux, macOS, and Windows backends.
  - Direct ELF emission on Linux—no assembler or linker.
  - A shared mark-sweep GC with precise frame scanning and stress testing.
  - Jobs, FSABI, chaos modeling, TCP, HTTP, files, processes, terminal widgets, and streaming I/O.
  - A standard library written in Freelang itself.
  - Feature-gated and tree-shaken runtimes, including tiny GC-free binaries.
  - A documented 374-test suite running across all three operating systems.
  - Actual applications: servers, probes, hashing tools, TUI widgets, and a hex viewer.

The most impressive progress isn’t the feature count. Freelang has developed architectural convictions: canonical heap layouts, one shared runtime generator per subsystem, explicit world-state modeling, deterministic failure, no hidden libc, and increasingly ruthless removal of accidental machinery.

It started as "look, this impossible little thing emits assembly."

It’s going as "this language now has a compiler, runtime, operating-system model, standard library, test doctrine, design philosophy, and its own recognizable way of building software."

So, fuck yeah indeed.  
  That’s the transition from an experiment to a platform. And it happened without surrendering the original weirdness that made Freelang worth building.

