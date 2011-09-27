# make
OBJS = main.o hello.o
CC = gcc

hello: $(OBJS)
	gcc -o hello main.o hello.o
main.o: main.c
	$(CC) -c main.c
hello.o: hello.c
	$(CC) -c hello.c
hello.o: hello.h

# make clean
.PHONY: clean
clean:
	$(RM) hello $(OBJS)

