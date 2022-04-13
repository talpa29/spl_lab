./all: exec

exec: asmAssignment0.o mainAssignment0.o 
	gcc -m32 -g -Wall -o run asmAssignment0.o mainAssignment0.o 


mainAssignment0.o: mainAssignment0.c
	gcc -g -m32 -Wall -ansi -c mainAssignment0.c -o mainAssignment0.o

asmAssignment0.o: asmAssignment0.s
	nasm -g -f elf -w+all -o asmAssignment0.o asmAssignment0.s

.PHONY: clean
clean:
	rm -f *.o run
