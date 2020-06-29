gcc_include_and_lib = -I/usr/include/SDL2 -lSDL2 -lSDL2_image -lglut -lGLU -lGL -lGLEW -lSOIL -I../deps/fmod1.09.09/inc -L../deps/fmod1.09.09/lib -lfmodstudioL -lfmodL
gcc_options = -std=c++17 -Wall $(gcc_include_and_lib) -Wl,-R../deps/fmod1.09.09/lib

default: program

program: *.cpp
	g++ *.cpp $(gcc_options) -o $@

run: program
	./program

clean:
	rm -f ./program

.PHONY: run clean
