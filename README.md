# wctl
A simple shell script for turning on and off wifi (using dhcpcd and wpa_supplicant)

## Usage

First configure all the variables in the script to fit your system. Then kill wpa_supplicant and dhcpcd. From now on only use the script to control them.

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
