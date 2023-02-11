CFLAGS=-std=c++11

all: nick-vm

nick-vm: nick-vm.o main.o
	$(CXX) $(CFLAGS) nick-vm.o main.o -o nick-vm

main.o: main.cpp
	$(CXX) $(CFLAGS) -c main.cpp

nick-vm.o: nick-vm.h nick-vm.cpp
	$(CXX) $(CFLAGS) -c nick-vm.cpp

clean:
	rm -f *.o nick-vm