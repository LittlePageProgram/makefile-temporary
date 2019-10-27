# This is a Makefile

IDIR = ../include

CC = gcc
CFLAGS = -g -I$(IDIR)

ODIR = obj

$(ODIR)/printNX: main.c $(IDIR)/main.h $(ODIR)/printXX.o $(ODIR)/printXXX.o
	$(CC) -o $@ $^ $(CFLAGS) 

$(ODIR)/printXX.o: printXX.c $(IDIR)/printXX.h
	$(CC) -c -o $@ $< $(CFLAGS)

$(ODIR)/printXXX.o: printXXX.c $(IDIR)/printXXX.h
	$(CC) -c -o $@ $< $(CFLAGS)

.PHONY: clean

clean:
	rm printNX 
	rm -f $(ODIR)/*.o *~ core $(IDIR)/*~
