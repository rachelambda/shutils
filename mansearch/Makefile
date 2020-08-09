PREFIX?=/usr
BINDIR?=$(PREFIX)/bin

all:
	@echo "Make options: install, uninstall, configure"

install:
	install -Dm755 mansearch $(BINDIR)/mansearch

uninstall:
	rm -f $(BINDIR)/mansearch
