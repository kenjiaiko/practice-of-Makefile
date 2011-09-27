# make
EXE = hello
OBJS = main.o hello.o
CC = gcc
CFLAGS = -Wall

.SUFFIXES: .c .o

.PHONY: all
all: depend $(EXE)

$(EXE): $(OBJS)
	$(CC) -o $(EXE) $^

.c.o:
	$(CC) $(CFLAGS) -c $<

# make clean
.PHONY: clean
clean:
	$(RM) $(EXE) $(OBJS) depend.inc

.PHONY: depend
depend: $(OBJS:.o=.c)
	-@ $(RM) depend.inc
	-@ for i in $^; do\
		cpp -MM $$i | sed "s/\ [_a-zA-Z0-9][_a-zA-Z0-9]*\.c//g" >> depend.inc;\
	done

-include depend.inc

