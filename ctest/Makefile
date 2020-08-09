PREFIX?=/usr
BINDIR?=$(PREFIX)/bin

all:
	@echo "Make options: install, uninstall, configure"

install:
	install -Dm755 ctest $(BINDIR)/ctest

uninstall:
	rm -f $(BINDIR)/ctest
