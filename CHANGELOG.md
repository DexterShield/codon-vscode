# Change Log

All notable changes to the "codon-lang" extension will be documented in this file.

## [0.1.0] - 2025-02-07

### Added

- Initial release
- Syntax highlighting for `.codon` files
- Support for Codon-specific decorators (`@par`, `@gpu`, `@export`, etc.)
- Highlighting for `from C import` statements
- Codon type highlighting (`ptr`, `Int`, `UInt`, etc.)
- Code snippets for common patterns:
    - C imports
    - Parallel loops
    - GPU kernels
    - HTTP server
    - LLVM inline IR
- Language configuration for proper indentation and brackets
- Examples and documentation

### Fixed

- N/A (initial release)

### Changed

- N/A (initial release)

## [Unreleased]

### Planned

- Language server support
- Code completion
- Go to definition
- Hover documentation
- Integrated terminal for `codon run`

```

---

### **📄 LICENSE**
```

MIT License

Copyright (c) 2025 [Your Name]

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

```

---

### **📄 .gitignore**
```

node_modules/
_.vsix
.vscode-test/
_.log
.DS_Store

```

---

### **📄 .vscodeignore**
```

.vscode/**
.gitignore
.git/**
node_modules/**
\*.vsix
examples/**
.github/\*\*
