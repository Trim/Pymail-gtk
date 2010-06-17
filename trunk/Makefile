RM= rm -fr
DESTDIR=
BIN= pymail-gtk

all:

install:
	mkdir -p $(DESTDIR)/usr/bin/
	mkdir -p $(DESTDIR)/usr/share/pixmaps
	mkdir -p $(DESTDIR)/usr/share/applications
	mkdir -p $(DESTDIR)/usr/share/$(BIN)
	mkdir -p $(DESTDIR)/home/hackable1/.$(BIN)

	install $(BIN) $(DESTDIR)/usr/bin/
	install ressources/$(BIN).png $(DESTDIR)/usr/share/pixmaps/
	install ressources/$(BIN).desktop $(DESTDIR)/usr/share/applications/
	install ressources/$(BIN).cfg $(DESTDIR)/home/hackable1/.$(BIN)
	chown hackable1:hackable1 $(DESTDIR)/home/hackable1/.$(BIN)

uninstall:
	$(RM) $(DESTDIR)/usr/bin/$(BIN)
	$(RM) $(DESTDIR)/usr/share/pixmaps/$(BIN)
	$(RM) $(DESTDIR)/usr/share/applications/$(BIN)
	#$(RM) $(DESTDIR)/home/hackable1/.$(BIN)/$(BIN)

	#rmdir $(DESTDIR)/home/hackable1/.$(BIN)
	rmdir $(DESTDIR)/usr/share/$(BIN)

copy:
	install $(BIN) $(DESTDIR)/usr/bin/

clean:
	rm *~
