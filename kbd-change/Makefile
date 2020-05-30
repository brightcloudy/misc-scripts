PREFIX ?= /usr/local
DIST_SCRIPTS = bin/kbd-change bin/kbd-disable bin/kbd-enable 
all: $(DIST_SCRIPTS)

bin/kbd-change: src/kbd-change
	cp src/kbd-change bin/
	chmod +x bin/kbd-change

bin/kbd-disable bin/kbd-enable: bin/kbd-change
	ln -sf ./kbd-change $@

clean:
	rm bin/*

install:
	cp -d -t $(PREFIX)/bin/ bin/* && chown root: $(addprefix $(PREFIX)/,$(DIST_SCRIPTS))
	chcon unconfined_u:object_r:bin_t:s0 $(addprefix $(PREFIX)/,$(DIST_SCRIPTS))

uninstall:
	rm $(addprefix $(PREFIX)/,$(DIST_SCRIPTS))
