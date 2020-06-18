PREFIX?=/usr
BINDIR?=$(PREFIX)/bin

all:
	@echo "Make options: install, uninstall, configure"

install:
	sed "s/DEV_PLACEHOLDER/$(shell basename $(shell find -L /sys/class/net -name 'wlp*' -or -name 'wlan*' -maxdepth 2))/g" wctl > $(BINDIR)/wctl
	sed "s/WPA_PLACEHOLDER/$(shell find /etc -name 'wpa_supplicant.conf' | sed -e 's/[\/&]/\\&/g' -e '1q')/g" $(BINDIR)/wctl | tee $(BINDIR)/wctl > /dev/null
	chmod 755 $(BINDIR)/wctl

configure:
	sed "s/DEV_PLACEHOLDER/$(shell basename $(shell find -L /sys/class/net -name 'wlp*' -or -name 'wlan*' -maxdepth 2))/g" wctl > /tmp/wctl
	sed "s/WPA_PLACEHOLDER/$(shell find /etc -name 'wpa_supplicant.conf' | sed -e 's/[\/&]/\\&/g' -e '1q')/g" /tmp/wctl > wctl
	rm -f /tmp/wctl

uninstall:
	rm -f $(BINDIR)/wctl
