# shttp
A simple http only webserver. It can serve most file types, throw 404 errors and handle multiple requests after each other.

Note however that this script does not care for safety. While I haven't done it myself it's possible that this script is capable of directory traversal.

## Depends

A netcat with support for the -e flag (I'm using busybox netcat).

If you wish to use another method of handling clients then read [the netcat subheader](#netcat)

## Installation

Either install with `make install` or if you wish to choose your own location `make BINDIR=<dir> install` or just move it to a directory yourself.

## Usage

You will probably want to run this as root.
```sh
shttp [server]
```

## Netcat
The script actually only takes requests as STDIN and sends responses to STDOUT. It just runs itself with netcat unless the "server" argument is given. Therefore you could easily modify the script to work with another method for client handling.
