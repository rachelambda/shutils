# ctest
A simple tool for testing stuff in C

## Installation

Either install with `make install` or if you wish to choose your own location `make BINDIR=<dir> install` or just move it to a directory yourself.

## Usage

After the program starts you can type c code. To stop typing press `Ctrl+D`. After this the typed code will be used as the body for a main function, compiled and executed.
```sh
ctest [program args]
```
