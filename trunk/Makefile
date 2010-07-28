RM= rm -fr
DESTDIR=
BIN= pymail-gtk

all:

install: pymail-gtk
	install -d $(DESTDIR)/usr/bin/
	install -d $(DESTDIR)/usr/share/pixmaps
	install -d $(DESTDIR)/usr/share/applications
	install -d $(DESTDIR)/usr/share/$(BIN)
	install $(BIN) $(DESTDIR)/usr/bin/
	install ressources/$(BIN).png $(DESTDIR)/usr/share/pixmaps/
	install ressources/$(BIN).desktop $(DESTDIR)/usr/share/applications/
	install ressources/$(BIN).cfg $(DESTDIR)/usr/share/$(BIN)/example.cfg

uninstall: pymail-gtk
	$(RM) $(DESTDIR)/usr/bin/$(BIN)
	$(RM) $(DESTDIR)/usr/share/pixmaps/$(BIN)
	$(RM) $(DESTDIR)/usr/share/applications/$(BIN)
	$(RM) $(DESTDIR)/usr/share/$(BIN)/example.cfg
	rmdir $(DESTDIR)/usr/share/$(BIN)

copy:
	install $(BIN) $(DESTDIR)/usr/bin/
clean:
