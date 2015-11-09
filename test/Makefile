include ../Makefile.setup

CFLAGS ?= -Wall

all: test

test: ../config.mk test.c
	arm-none-linux-gnueabi-gcc $(CFLAGS) -o $@ test.c -lEGL -lGLESv2 -lMali -lUMP

clean:
	rm -f test
