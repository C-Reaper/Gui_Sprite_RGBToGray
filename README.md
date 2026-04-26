# Project README

## Overview
The project is a simple GUI application that converts RGB sprites to grayscale (G). It provides a basic window where users can see the current sprite and interact with it. The application uses libraries such as X11 for Linux, user32 and gdi32 for Windows, and SDL for WebAssembly.

## Features
- Simple GUI window
- Display of RGB sprite
- Interaction controls (not explicitly supported in code)

## Project Structure

### Prerequisites
- C/C++ Compiler and Debugger (GCC)
- Make utility
- Standard development tools
- X11 library (Linux)
- user32, gdi32, winmm libraries (Windows)

## Build & Run
The project includes four makefiles for different operating systems:
- `Makefile.linux` for Linux
- `Makefile.windows` for Windows
- `Makefile.wine` for Linux cross-compilation to Windows
- `Makefile.web` for WebAssembly

### Building the Project
1. Navigate to the project directory.
2. Use the appropriate Makefile depending on your operating system:
   ```sh
   make -f Makefile.(os) all  # Build output
   make -f Makefile.(os) do   # Build + executable output
   make -f Makefile.(os) clean # Remove build artifacts
   ```

### Executing the Project
- Linux: `make -f Makefile.linux exe`
- Windows: `make -f Makefile.windows exe`
- Wine: `make -f Makefile.wine exe`
- WebAssembly: Open `build/index.html` in a web browser

---

The project is organized with specific directories and files as outlined in the Project Organization section. The build process involves compiling the source code using the appropriate Makefile for the target platform.