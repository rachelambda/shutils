PREFIX?=/usr
BINDIR?=$(PREFIX)/bin

all:
	@echo "Make options: install, uninstall, configure"

install:
	sed "s/PATH_PLACEHOLDER/$(shell find -L /sys/class/backlight -name 'brightness' -maxdepth 2 | sed -e 's/[\/&]/\\&/g' -e '1q')/g" bri > $(BINDIR)/bri
	chmod 755 $(BINDIR)/bri

configure:
	sed "s/PATH_PLACEHOLDER/$(shell find -L /sys/class/backlight -name 'brightness' -maxdepth 2 | sed -e 's/[\/&]/\\&/g' -e '1q')/g" bri > /tmp/bri
	cat /tmp/bri > bri
	rm -f /tmp/bri

uninstall:
	rm -f $(BINDIR)/bri
