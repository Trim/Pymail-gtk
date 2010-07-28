RM= rm -fr
DESTDIR=
BIN= pymail-gtk

all:

install:
	mkdir -p $(DESTDIR)/usr/bin/
	mkdir -p $(DESTDIR)/usr/share/pixmaps
	mkdir -p $(DESTDIR)/usr/share/applications
	mkdir -p $(DESTDIR)/usr/share/$(BIN)

	install $(BIN) $(DESTDIR)/usr/bin/
	install ressources/$(BIN).png $(DESTDIR)/usr/share/pixmaps/
	install ressources/$(BIN).desktop $(DESTDIR)/usr/share/applications/
        install ressources/$(BIN).cfg $(DESTDIR)/usr/share/$(BIN)/

uninstall:
	$(RM) $(DESTDIR)/usr/bin/$(BIN)
	$(RM) $(DESTDIR)/usr/share/pixmaps/$(BIN)
	$(RM) $(DESTDIR)/usr/share/applications/$(BIN)
	rmdir $(DESTDIR)/usr/share/$(BIN)

copy:
	install $(BIN) $(DESTDIR)/usr/bin/

