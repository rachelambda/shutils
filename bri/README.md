# bri
A minimal backlight tool

## Depends

* sudo or doas (only needed for non root operation)

## Installation

Either install with `make install` or if you wish to choose your own location `make BINDIR=<dir> install` or to just set up the backlight path in the script `make configure`.

## Usage

If no amount is given it will default to 1.

Increase brightness
```
bri inc [amount]
```

Decrease brightness
```
bri dec [amount]
```

Set brightness
```
bri set [amount]
```

Set brightness to highest possible value
```
bri max
```

Get brightness
```
bri get
```
