all: programexe
#all: clean

programexe: program.o staticlib.a sharedlib.so
	cc program.o source/staticlib.a -o static_block
	cc program.o source/sharedlib.so -o dynamic_block

program.o: program.c
	cc -c program.c -o program.o

staticlib.a: block.o
	cd source; \
	ar qc staticlib.a block.o

sharedlib.so: source/block.c
	cd source; \
	cc -fPIC -c block.c && \
	cc -shared -o sharedlib.so block.o

block.o: source/block.c
	cd source; \
	cc -c block.c -o block.o

block.o: headers/block.h

clean:
	rm *.o dynamic_block static_block; \
	cd source; \
	rm *.o *.so *.a