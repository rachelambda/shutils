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

Restart wifi
```
wctl restart
```

Wifi status
```
wctl status
```

## To be added

Add and remove networks from wpa_supplicant.conf
