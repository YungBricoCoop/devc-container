# 🐋 c-devbox

A lightweight development container for C and C++ development with tools for compiling, linting, formatting, and debugging!

Contains:

- `Clang` and `Clang-Extra-Tools` for compilation and additional tooling.
- `Valgrind` for memory debugging.
- `CMake` and `Ninja` for efficient build automation.
- `Cppcheck` and `Cpplint` for static code analysis.
- `Zsh` with `Oh My Zsh` and plugins: Syntax highlighting, Autosuggestions, You-Should-Use for alias suggestions
- `gcc` and `g++` for C and C++ compilation (musl version only)

## 🚀 Run (musl version, based on Alpine)

Windows :

```sh
docker run --name c-devbox -v ".\code:/code" -it yungbricocoop/c-devbox
```

Linux :

```sh
docker run --name c-devbox -v "./code:/code" -it yungbricocoop/c-devbox
```

## 🚀 Run (glib version, based on bookworm-slim)

Windows :

```sh
docker run --name c-devbox -v ".\code:/code" -it yungbricocoop/c-devbox:glib
```

Linux :

```sh
docker run --name c-devbox -v "./code:/code" -it yungbricocoop/c-devbox:glib
```

## ⌨️ Shortcuts

- Compile C++: `x` compiles main.cpp and runs the output.
- Compile C: `cx` compiles main.c and runs the output.
- Format Code: `cformat` applies clang-format to all .cpp and .h files.
- Run Static Analysis: `ccheck` runs cppcheck on all files.
