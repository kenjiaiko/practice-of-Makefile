# make
EXE = hello
OBJS = main.o hello.o
CC = gcc
CFLAGS = -Wall

$(EXE): $(OBJS)
	$(CC) -o $(EXE) $^
main.o: main.c
	$(CC) $(CFLAGS) -c $<
hello.o: hello.c
	$(CC) $(CFLAGS) -c $<
hello.o: hello.h

# make clean
.PHONY: clean
clean:
	$(RM) $(EXE) $(OBJS)

