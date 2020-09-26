SRC = drw.c dwm.c util.c

INCLUDE = -I/usr/X11R6/include -I/usr/include/freetype2

DEFS = -D_DEFAULT_SOURCE -D_BSD_SOURCE -D_POSIX_C_SOURCE=200809L -DVERSION=\"6.2\" -DXINERAMA

LDFLAGS = -lX11 -lXinerama -lfontconfig -lXft

CFLAGS = -Ofast -march=native -funroll-loops -flto

BIN = dwm

CC = gcc

$(BIN): $(SRC) *.h Makefile
	$(CC) $(SRC) $(CFLAGS) $(INCLUDE) $(DEFS) $(LDFLAGS) -o $(BIN)

clean:
	rm -f $(BIN)

install: $(BIN)
	mkdir -p $(DESTDIR)$(PREFIX)/bin
	cp -f dwm $(DESTDIR)$(PREFIX)/bin
	chmod 755 $(DESTDIR)$(PREFIX)/bin/$(BIN)

uninstall:
	rm -f $(DESTDIR)$(PREFIX)/bin/$(BIN)
