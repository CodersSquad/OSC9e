# the compiler: gcc for C program, define as g++ for C++
CC = gcc
# Remove command for with recursive and force flags
RM = rm -rf
# compiler flags:
#  -g    adds debugging information to the executable file
#  -Wall turns on most, but not all, compiler warnings
CFLAGS  = -g -Wall
# OpenMP Flag
OMP_FLAGS = -fopenmp
# PThreads Flag
PTH_FLAGS = -lpthread

openmp: openmp.c
	$(CC) $(CFLAGS) $(OMP_FLAGS) -o $@.o $<

thrd-posix: thrd-posix.c
	$(CC) $(CFLAGS) $(PTH_FLAGS) -o $@.o $<

clean:
	$(RM) *.o
