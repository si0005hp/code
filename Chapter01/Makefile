gcc_include_and_lib = -I/usr/include/SDL2 -lSDL2
gcc_options = -std=c++17 -Wall --pedantic-error $(gcc_include_and_lib)

default: program

program: Main.cpp Game.cpp Game.h
	g++ Main.cpp Game.cpp Game.h $(gcc_options) -o $@

run: program
	./program

clean:
	rm -f ./program

.PHONY: run clean
