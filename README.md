# Protocol Buffers
Protocol Buffers are a language-neutral, platform-neutral extensible mechanism for serializing structured data.

[Protocol Buffers](https://protobuf.dev/overview/)

Protocol Buffers (often shortened to "protobuf") is a method developed by Google for serializing structured data, similar to JSON or XML. It's both a language-agnostic binary serialization format and a language for defining these data structures: the .proto files.

* Efficiency: Protocol Buffers offer a compact binary format which can be much smaller than equivalent JSON or XML representations.
* Strong Typing: The generated Rust code has strong types based on your .proto definitions, which can catch potential errors at compile time.
* Interoperability: Since Protocol Buffers is language-agnostic, you can use it to communicate between systems written in different languages.
* Schema Evolution: Protocol Buffers are designed to allow you to add new fields to your data structures without breaking old programs.

## Protocol Buffer Work
1. Create .proto file to define data structures.
2. Generate code using protoc compiler. Output will be Rust code for this project.
3. Use the generated enums and structs in your code to serialize, share and deserializee data.


[Prost](https://crates.io/crates/prost) is a Protocol Buffers implementation for the Rust Language. prost generates simple, idiomatic Rust code from proto2 and proto3 files.

```bash
cargo add prost --no-default-features --features prost-derive
```
