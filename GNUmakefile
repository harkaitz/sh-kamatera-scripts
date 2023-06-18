DESTDIR =
PREFIX  =/usr/local


all:
clean:
install:
update:
## -- install-sh --
install: install-sh
install-sh:
	mkdir -p $(DESTDIR)$(PREFIX)/bin
	cp bin/kamatera-h-ssh   $(DESTDIR)$(PREFIX)/bin
	cp bin/kamatera-h-power $(DESTDIR)$(PREFIX)/bin
	cp bin/kamatera-h-ls-hosts $(DESTDIR)$(PREFIX)/bin
	cp bin/kamatera-h-ipaddr $(DESTDIR)$(PREFIX)/bin
	cp bin/kamatera-h-queue $(DESTDIR)$(PREFIX)/bin
	cp bin/kamatera-h-billing $(DESTDIR)$(PREFIX)/bin
	cp bin/kamatera-h-rename $(DESTDIR)$(PREFIX)/bin
	cp bin/kamatera-h-create $(DESTDIR)$(PREFIX)/bin
	cp bin/kamatera-h-create-options $(DESTDIR)$(PREFIX)/bin
	cp bin/kamatera-h-info  $(DESTDIR)$(PREFIX)/bin
	cp bin/kamatera-h-passwd $(DESTDIR)$(PREFIX)/bin
	cp bin/kamatera-h-ls    $(DESTDIR)$(PREFIX)/bin
	cp bin/kamatera-h-uuid  $(DESTDIR)$(PREFIX)/bin
	cp bin/kamatera-h-rest  $(DESTDIR)$(PREFIX)/bin
## -- install-sh --
## -- license --
install: install-license
install-license: LICENSE
	mkdir -p $(DESTDIR)$(PREFIX)/share/doc/sh-kamatera-scripts
	cp LICENSE $(DESTDIR)$(PREFIX)/share/doc/sh-kamatera-scripts
## -- license --
