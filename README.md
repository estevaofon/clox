# clox

A C bytecode virtual machine for the Lox programming language, following [Crafting Interpreters](https://craftinginterpreters.com/) by Robert Nystrom.

## About

**clox** is a bytecode interpreter for Lox. It compiles Lox code into bytecode and executes it on a custom VM for better performance than the tree-walk interpreter (jlox).

**Current Status**: Early development
- ✅ Bytecode chunk system (dynamic arrays)
- ✅ Memory management
- ✅ Debug/disassembler utilities

## Building

Compile with any C compiler:

```bash
gcc -o clox main.c chunk.c debug.c memory.c
```

Run the program:

```bash
./clox        # Linux/macOS
clox.exe      # Windows
```

## Project Structure

```
├── chunk.h/c       # Bytecode storage
├── common.h        # Common definitions
├── debug.h/c       # Disassembler
├── memory.h/c      # Memory management
└── main.c          # Entry point
```

## Roadmap

Following the "Crafting Interpreters" book:

- [ ] Values and types
- [ ] Arithmetic operations
- [ ] Compiler (parser + codegen)
- [ ] VM execution
- [ ] Variables and scopes
- [ ] Control flow
- [ ] Functions and closures
- [ ] Classes and inheritance
- [ ] Garbage collection

## References

- [Crafting Interpreters](https://craftinginterpreters.com/)
- [Lox Language Spec](https://craftinginterpreters.com/the-lox-language.html)

## License

Educational project based on "Crafting Interpreters".

