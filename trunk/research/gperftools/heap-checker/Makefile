.PHONY: default clean

default: heap_checker

heap_checker: heap_checker.cc Makefile
	g++ -o heap_checker heap_checker.cc -g -O0 -ansi \
        -fno-builtin-malloc -fno-builtin-calloc -fno-builtin-realloc -fno-builtin-free \
        -I../../../objs/gperf/include ../../../objs/gperf/lib/libtcmalloc_and_profiler.a -lpthread
clean:
	rm -rf heap_checker ./*.dSYM
