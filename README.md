# Codon Language Support for Visual Studio Code

Syntax highlighting, snippets, and language support for [Codon](https://github.com/exaloop/codon) - the high-performance Python compiler that compiles to native machine code.

## Features

- 🎨 **Syntax Highlighting** - Full syntax highlighting for Codon files (`.codon`)
- 📝 **Code Snippets** - Helpful snippets for common Codon patterns
- 🔧 **Language Configuration** - Proper indentation, brackets, and comments
- ⚡ **Codon-Specific Features** - Highlighting for:
    - `@par`, `@gpu`, `@export` decorators
    - `from C import` statements
    - Codon-specific types (`ptr`, `Int`, `UInt`, etc.)
    - LLVM inline IR blocks

## Installation

### From VSIX (Recommended)

1. Download the latest `.vsix` file from [Releases](https://github.com/YOUR-USERNAME/codon-vscode/releases)
2. Open VSCode
3. Press `Cmd/Ctrl + Shift + P`
4. Type "Install from VSIX"
5. Select the downloaded `.vsix` file

- #### Or Using terminal
    ```bash
    code --install-extension codon-lang-0.1.0.vsix
    ```

### From Source

```bash
# Clone the repository
git clone https://github.com/YOUR-USERNAME/codon-vscode.git
cd codon-vscode

# Copy to VSCode extensions folder
# macOS/Linux:
cp -r . ~/.vscode/extensions/codon-lang-0.1.0

# Windows:
# Copy to %USERPROFILE%\.vscode\extensions\codon-lang-0.1.0

# Restart VSCode
```

### From Marketplace (Coming Soon)

Search for "Codon" in the VSCode Extensions Marketplace.

## Usage

Simply open any `.codon` file and enjoy syntax highlighting!

### Snippets

Type these prefixes and press `Tab`:

- `cimport` - Import C function
- `par` - Parallel for loop
- `gpu` - GPU kernel
- `export` - Export function for C/C++
- `httpserver` - HTTP server template
- `route` - HTTP route handler
- `llvm` - LLVM inline IR function
- `main` - Main function template

## Examples

```python
# HTTP Server
from C import socket, bind, listen, accept

class HTTPServer:
    def __init__(self, port: int = 8080):
        self.port = port

    def run(self):
        # Server implementation
        pass

app = HTTPServer(port=8080)
app.run()
```

```python
# Parallel Computing
@par(num_threads=8)
for i in range(1000000):
    process(data[i])
```

```python
# C Interop
from C import malloc, free, memcpy

def use_c_memory():
    ptr = malloc(1024)
    # use memory
    free(ptr)
```

## Requirements

- Visual Studio Code 1.60.0 or higher
- [Codon](https://github.com/exaloop/codon) compiler (optional, for running code)

## Extension Settings

This extension contributes the following settings:

- `codon.highlighting.enableExtended`: Enable/disable extended syntax highlighting for Codon-specific features

## Known Issues

- None yet! [Report issues here](https://github.com/YOUR-USERNAME/codon-vscode/issues)

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## Release Notes

### 0.1.0

- Initial release
- Syntax highlighting for `.codon` files
- Code snippets for common patterns
- Support for Codon-specific keywords and decorators

## License

MIT License - see [LICENSE](LICENSE) file for details

## Links

- [Codon GitHub](https://github.com/exaloop/codon)
- [Codon Documentation](https://docs.exaloop.io/)
- [Report Issues](https://github.com/YOUR-USERNAME/codon-vscode/issues)

---

**Enjoy coding with Codon! 🔥**
