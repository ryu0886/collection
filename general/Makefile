INC=-I./ -I./
default: main
main: general.c
	gcc -Wall $(INC) -c general.c
	gcc -o main.out general.o
win32: general.c
	x86_64-w64-mingw32-gcc-win32 -Wall $(INC) -c general.c
	x86_64-w64-mingw32-gcc-win32 -o main32.exe general.o
win64: general.c
	i686-w64-mingw32-gcc-win32 -Wall $(INC) -c general.c
	i686-w64-mingw32-gcc-win32 -o main64.exe general.o
clean:
	-rm -f general.o
	-rm -f main32.exe
	-rm -f main64.exe
	-rm -f main.out
