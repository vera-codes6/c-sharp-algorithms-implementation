## C# Algorithms and Data Structures

This repository is a curated collection of algorithms, data structures, and utilities implemented in modern C# for educational and reference purposes. The solution targets .NET 8 and includes comprehensive unit tests.

### Solution layout

- `Algorithms/` — core algorithms across topics such as graphs, numeric methods, encoders/crypto, machine learning, search, sorters, sequences, and more.
- `DataStructures/` — classic and advanced data structures (trees, heaps, graphs, tries, probabilistic, caches, etc.).
- `Utilities/` — small helpers and extensions used by the library projects.
- `Algorithms.Tests/`, `DataStructures.Tests/`, `Utilities.Tests/` — NUnit-based test projects covering the above libraries.

### Requirements

- .NET 8 SDK
- Any editor or IDE with C# support (VS Code, Visual Studio, Rider)

### Build

- Build everything: `dotnet build C-Sharp.sln -c Release`

### Test

- Run all tests: `dotnet test C-Sharp.sln`
- Collect coverage (uses coverlet.collector): `dotnet test C-Sharp.sln --collect:"XPlat Code Coverage"`

Coverage reports are written under each test project's `TestResults` directory.

### Browse by topic

- Algorithms: `Algorithms/`
  - Crypto: `Algorithms/Crypto/` (Digests, Paddings, Utils)
  - Data Compression: `Algorithms/DataCompression/`
  - Encoders: `Algorithms/Encoders/`
  - Graph: `Algorithms/Graph/`
  - Numeric and Modular Arithmetic: `Algorithms/Numeric/`, `Algorithms/ModularArithmetic/`
  - Machine Learning: `Algorithms/MachineLearning/`
  - Search and Sorters: `Algorithms/Search/`, `Algorithms/Sorters/`
  - Sequences, Shufflers, Strings, Problems, and more
- Data Structures: `DataStructures/`
  - Trees (AA, AVL, Red-Black, Scapegoat, Segment Trees, BST)
  - Heaps (Binary, Fibonacci, Pairing, Min-Max)
  - Graph, Disjoint Set, Fenwick, Tries, Hashing, Queues/Stacks, Linked Lists
  - Probabilistic (Bloom Filter, Count-Min Sketch, HyperLogLog), Caches (LRU, LFU)

Some algorithms that render images (e.g., fractals) use SkiaSharp; see `Algorithms/Algorithms.csproj` for dependencies.

### Coding standards

- C# nullable reference types enabled; warnings treated as errors.
- StyleCop analyzers configured via `stylecop.json` and `stylecop.ruleset`.
- Please keep implementations minimal, well-documented (XML docs), and add unit tests.

### Contributing

Contributions are welcome. To add a new algorithm/data structure:

1) Place the implementation in the most appropriate folder under `Algorithms/` or `DataStructures/`.
2) Add NUnit tests in the matching test project.
3) Ensure `dotnet build` and `dotnet test` pass locally.

Open an issue for questions or proposals.

### License

This project is licensed under the GNU General Public License v3.0. See `LICENSE` for details.
