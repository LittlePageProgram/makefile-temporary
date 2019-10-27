# This is a Makefile

main:main.o printXX.o printXXX.o
	gcc main.o printXX.o printXXX.o
main.o:main.c printXX.h printXXX.h
	gcc -c main.c
printXX.o:printXX.c printXX.h
	gcc -c printXX.c
printXXX.o:printXXX.c printXXX.h
	gcc -c printXXX.c

.PHONY: clean

clean:
	rm a.out
	rm *.o 
