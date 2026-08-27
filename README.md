# Quad Tree Visualizer

An interactive C++ visualization of a point quad tree built with [olcPixelGameEngine](https://github.com/OneLoneCoder/olcPixelGameEngine).

Clicking in the 400 × 400 window inserts a point. A node stores up to four points before subdividing into four child regions, and the program draws both the subdivision boundaries and inserted points.

## Requirements

- A C++ compiler
- Platform dependencies required by olcPixelGameEngine
- Visual Studio on Windows if you want to use the included `quad_tree.vcxproj`

## Run on Windows

1. Open `quad_tree.vcxproj` in Visual Studio.
2. Build the project.
3. Run the generated executable.
4. Left-click in the window to add points and watch the tree subdivide.

The repository includes `olcPixelGameEngine.h`, so no separate engine download is required.

## Source overview

- `main.cpp` — quad-tree data structures, insertion logic, rendering, and application entry point
- `olcPixelGameEngine.h` — the single-header rendering framework
- `quad_tree.vcxproj` — Visual Studio project configuration

## Status

This is a compact educational demo. It visualizes insertion and subdivision; querying, deletion, balancing, and memory cleanup are not implemented.
