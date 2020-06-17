# wctl
A minimal network manager.

## Depends

* sudo or doas (only needed for non root operation)
* wpa_supplicant
* dhcpcd
## Installation

Either install with `make install` or if you wish to choose your own location `make BINDIR=<dir> install` or to just set up the backlight path in the script `make configure`.

## Usage

Enable wifi
```
wctl enable
```

Disable wifi
```
wctl disable
```

Wifi status
```
wctl status
```

List remembered networks
```
wctl list
```

Add a network
```
wctl add <SSID> [password]
```

Remove a network
```
wctl remove <SSID>
```
