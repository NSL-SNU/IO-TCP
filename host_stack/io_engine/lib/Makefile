.PHONY: clean

CC=gcc
PS=

ifeq ($(PS),1)
all: pslib.a

pslib.a: pslib.c
	$(CC) -O3 -c -g -Wall -fPIC -o pslib.o pslib.c
	ar rcs libps.a pslib.o

clean:
	rm -f *.o *.a
else
all:

clean:

endif

distclean: clean
	rm -f Makefile
