CFLAGS=-std=c++11

all: nick

nick: nick.o lexer.o
	$(CXX) $(CFLAGS) nick.o lexer.o -o $@

lexer.o: lexer.h lexer.cpp
	$(CXX) $(CFLAGS) -c lexer.cpp

nick.o: lexer.h nick.cpp
	$(CXX) $(CFLAGS) -c nick.cpp

clean:
	rm -f nick *.o *.bin