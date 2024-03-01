# ZIMD

Additional cross-platform SIMD support for Zig.

Based loosely on [Google Highway](https://github.com/google/highway)

## Why?

Zig has builtin support for SIMD operations using `@Vector`. However this only supports a few
basic operations. This library aims to fill in some of the blanks.

## Operators

### [TableLookupBytesOr0](https://google.github.io/highway/en/master/quick_reference.html#blockwise)

Architectures: Scalar, X86_SSE3, Arm_Neon

Similar to Zig's `@shuffle` operator, except doesn't require the shuffle mask to be comptime known.
