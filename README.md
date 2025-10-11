zig-binarystream

zig-binarystream is a lightweight, low-level binary stream library for the Zig programming language
. It provides a set of utilities for efficient reading and writing of binary data, ideal for applications such as file I/O, network communication, and custom serialization formats.

⚙️ Features

Stream-based I/O: Efficient reading and writing of binary data streams.

Low-level operations: Direct manipulation of bytes for performance-critical applications.

Minimal dependencies: Pure Zig implementation with no external dependencies.

Flexible API: Supports various data types and custom structures.

📦 Installation

To include zig-binarystream in your Zig project, add it as a dependency in your build.zig file:

```zig
const bstream = b.addPackage("binarystream", "path/to/zig-binarystream"); 
```


Then, import and use it in your code:

```zig const bstream = @import("binarystream");
```

🛠️ Usage Example
```zig const bstream = @import("binarystream");
const writer = bstream.Writer.init(...);
try writer.writeU8(42);
try writer.writeU16(1234);
try writer.flush();
```

📄 License

Distributed under the MIT License. See LICENSE for more information.


