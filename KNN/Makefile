CC=g++
SRC := $(MNIST_ML_ROOT)/KNN/src
CFLAGS := -std=c++11 -DEUCLID
INCLUDE_DIR := $(MNIST_ML_ROOT)/KNN/include/
LIB_DIR := $(MNIST_ML_ROOT)/lib

all: main

main: $(SRC)/knn.cc
	$(CC) $(CFLAGS) $(SRC)/knn.cc -o main -L$(LIB_DIR)/ -I$(INCLUDE_DIR)\
	-I$(MNIST_ML_ROOT)/include -ldata -Wl,--verbose
clean:
	rm -f main