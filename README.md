# zig-best-practice

A Claude Code plugin providing comprehensive Zig best practices for writing safe, performant, and maintainable Zig code.

## Patterns Covered (10 Sections)

1. **Memory Safety** — errdefer chains, arena allocators, poisoning, resource grouping
2. **Infallible Runtime Operations** — AssumeCapacity philosophy across all container types
3. **Error Handling** — narrow error sets, exhaustive switches, error composition
4. **Comptime & Generics** — type functions, `@fieldParentPtr`, `@Type`, `@embedFile`, deep equality
5. **Memory Layout & Copy Safety** — extern structs, SIMD, mmap, cache alignment, packed structs
6. **Naming & Style** — snake_case/PascalCase rules, named arguments, sized types
7. **Code Organization** — imports, intrusive data structures, object pools, ref counting
8. **Thread Safety & Concurrency** — threadlocal, lock-free MPSC, atomics
9. **Smart Pointer Patterns** — copy-on-write, RefCount mixin
10. **C Interop** — export fn, callconv, allocator bridging, pointer smuggling

## Sources

Patterns extracted from production codebases:
- [TigerBeetle](https://github.com/tigerbeetle/tigerbeetle) — financial transactions database
- [Bun](https://github.com/oven-sh/bun) — JavaScript runtime
- [libxev](https://github.com/mitchellh/libxev) — cross-platform event loop
- [Ghostty](https://github.com/ghostty-org/ghostty) — terminal emulator

## Install

```
/plugin install zig-best-practice@<your-marketplace>
```

Or add this repo as a marketplace:

```
/plugin marketplace add <owner>/zig-best-practice-skill
```

## License

MIT
