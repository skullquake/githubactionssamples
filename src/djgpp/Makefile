# Makefile for compiling src/a.c into bin/a.out or bin/a.exe

# Allow overriding the compiler: make CC=x86_64-w64-mingw32-gcc
CC ?= gcc
SRC = ./src/a.c
BIN_DIR = ./bin
OUT = $(BIN_DIR)/a.out

ifeq ($(findstring mingw,$(CC)),mingw)
	OUT = $(BIN_DIR)/a.exe
endif

all: $(OUT)

$(OUT): $(SRC) | $(BIN_DIR)
	$(CC) -o $@ $<

$(BIN_DIR):
	mkdir -p $(BIN_DIR)

clean:
	rm -rf $(BIN_DIR)

.PHONY: all clean
