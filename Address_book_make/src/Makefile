CPPFLAGS:=-I../lib
SRC:=$(wildcard *.c)
OBJS:=$(SRC:.c=.o)
BIN:=address_book
LIB:=-L../lib -llist

.PHONY: all clean

all: $(BIN)

$(BIN): $(OBJS)
	gcc $(CPPFLAGS) $^ $(LIB) -o $@

clean:
	$(RM) -f $(BIN) $(OBJS)
