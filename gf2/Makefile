CXX ?= g++
CXXLAGS ?= -O2 -march=native

.PHONY: all clean install

all: gf2
gf2: gf2.cpp
	/bin/bash -x build.sh
install: gf2
	install -D -m 0755 --strip -t $(DESTDIR) gf2
clean:
	rm -f gf2
