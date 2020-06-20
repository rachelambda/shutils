PREFIX?=/usr
BINDIR?=$(PREFIX)/bin

all:
	@echo "Make options: install, uninstall, configure"

install:
	install -Dm755 shttp $(BINDIR)/shttp

uninstall:
	rm -f $(BINDIR)/shttp
