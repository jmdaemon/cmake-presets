# CMake Presets

This repository contains some useful CMake presets for various CMake build configurations.

This repository supports the following build presets:

- gcc-debug-ninja
- gcc-debug-unix-makefiles
- clang-debug-ninja
- clang-debug-unix-makefiles

## Usage

1. Include one of these presets into your `CMakePresets.json` file:

To include the GCC configuration build preset:

``` json
{
  "version": 4,
  "cmakeMinimumRequired": {
    "major": 3,
    "minor": 23,
    "patch": 0
  },
  "include": [
    "presets/gcc.json"
  ]
}
```

2. Run CMake with the desired build preset:

``` bash
cmake --preset=gcc-debug-unix-makefiles
```
