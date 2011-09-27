# make
.PHONY: all
all: hello

hello: main.o hello.o
	gcc -o hello main.o hello.o
main.o: main.c
	gcc -c main.c
hello.o: hello.c
	gcc -c hello.c
hello.o: hello.h

# make clean
.PHONY: clean
clean:
	rm -f hello main.o hello.o

