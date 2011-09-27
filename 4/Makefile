# make
.PHONY: all
all: hello goodbye

hello: main.o hello.o
	gcc -o hello main.o hello.o
main.o: main.c
	gcc -c main.c
hello.o: hello.c
	gcc -c hello.c

goodbye: goodbye.o
	gcc -o goodbye goodbye.o
goodbye.o: goodbye.c
	gcc -c goodbye.c

# make clean
.PHONY: clean
clean:
	rm -f hello main.o hello.o goodbye goodbye.o

