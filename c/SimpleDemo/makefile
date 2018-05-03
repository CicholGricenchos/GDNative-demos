all:
	gcc -fPIC -shared -o bin/libplugin.so src/plugin.c
	gcc -std=c11 -fPIC -c src/simple.c -I/home/cichol/godot_headers/ -I./src -o src/simple.os
	gcc -shared -L./bin -lplugin -Wall src/simple.os -o bin/libsimple.so
