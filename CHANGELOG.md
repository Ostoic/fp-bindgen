# CHANGELOG

## main

- Added Deno support for the TypeScript runtime.
- Reorganized examples and improved documentation.
- Added end-to-end tests.
- Fix #105: Correctly handle passing negative integers as primitives (outside
  MessagePack) between Rust and TypeScript.
- Fix type of MessagePack-encoded 64-bit integers in TypeScript bindings.
- Fix handling synchronous responses from async plugin functions in TypeScript
  runtime.
- Fix #108: Serialization of types from the `time` crate now works between Rust
  and TypeScript.
- Implemented warnings when types that rely on custom Serde (de)serializers are
  used in contexts where their annotations cannot be used.
- Various smaller bugfixes.
- **Deprecation**: `BindingsType::TsRuntime` is now deprecated in favor of
  `BindingsType::TsRuntimeWithExtendedConfig`.
