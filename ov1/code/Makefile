CC=g++
LDLLIBS= -lGLEW -framework OpenGL -framework GLUT
CFLAGS= -Wno-deprecated

.PHONY:
all: shaderDemo

shaderDemo: shaderDemo.o
	g++ $(LDLIBS) $^ -o shaderDemo

shaderDemo.o: shaderDemo.cpp
	g++ -c $(CFLAGS) shaderDemo.cpp vsShaderLib.cpp vsMathLib.cpp

.PHONY:
clean:
	rm -r *.o shaderDemo
