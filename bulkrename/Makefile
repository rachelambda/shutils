PREFIX?=/usr
BINDIR?=$(PREFIX)/bin

all:
	@echo "Make options: install, uninstall, configure"

install:
	install -Dm755 bulkrename $(BINDIR)/bulkrename

uninstall:
	rm -f $(BINDIR)/bulkrename
