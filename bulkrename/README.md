# bulkrename
A way to rename many files at once

## Installation

Either install with `make install` or if you wish to choose your own location `make BINDIR=<dir> install` or just move it to a directory yourself.

## Usage

If no options are given dir defaults to `.` and depth defaults to 1
```sh
bulkrename [dir] [depth]
```

Here dir is the directory in which files should be renamed and depth is the depth of which to recursively list files.
