objects=$(shell ls *.cxx | sed "s/.cxx/.o/g") 

all: $(objects)

lib: $(objects)
	$(CXX) $(CFLAGS) --shared -o libthread.so $(objects)

clean:
	rm -f *.o *.so

include $(wildcard *.mk)
