gcc_include_and_lib = -I/usr/include/SDL2 -lSDL2 -lSDL2_image -lglut -lGLU -lGL -lGLEW -lSOIL
gcc_options = -std=c++17 -Wall --pedantic-error $(gcc_include_and_lib)

default: program

program: *.cpp
	g++ *.cpp $(gcc_options) -o $@

run: program
	./program

clean:
	rm -f ./program

.PHONY: run clean
