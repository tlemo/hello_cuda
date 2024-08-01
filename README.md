
# Hello, CUDA

A minimal, cross-platform, CUDA + CMake example

## Building from source

#### Prerequisites

1. A C++ 17 compiler (GCC, Clang, MSVC)
2. CUDA SDK 11.0 or newer
3. CMake 3.25 or newer
4. Ninja (optional)

#### Building on Windows

When building on Windows with MSVC, the CMake configuration must be done from
a MSVC command prompt (ex. run `vcvarsall.bat`)

#### Building with CMake

> Tip: CMake uses the `CUDA_PATH` environment variable. Make sure it is set
> and points to the right location before running `cmake`.

This project uses CMake, so the general build process looks like (assuming
a Ninja build):

```shell
mkdir build && cd build
cmake .. -G Ninja -DCMAKE_BUILD_TYPE=Release
ninja
```
