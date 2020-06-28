# VSCode CMake Boilerplate
VSCode Boilerplate for building &amp; debugging w/ cmake

Tested with:
- GCC/GDB
- Clang/GDB
- MSVC

## Step 0: Installation

1. Install 
2. Install VSCode extensions:
	- C++ Extension
	- CMake Extension
3. Select CMake Kit
   - Ctrl+Shift+P and "CMake: Select a kit"

## Step 1: Configure

Click `CMake: [Debug]: Ready` in the bottom left status bar. Select a configuration and this will configure the cmake project

## Step 2: Build

Click `Build` in the bottom left status bar

## Step 3: Debug

Copy the `launch.json` from this project into your project's `.vscode/` directory.

Press F5 to begin debugging!
