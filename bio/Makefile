
SOURCES=bio_file.cc bio_b64_encode.cc bio_b64_decode.cc
PROGRAMS = $(SOURCES:.cc=)

default: $(PROGRAMS)


clean:
	-rm -f $(PROGRAMS)
	-rm -f *.o

.cc.o:
	$(CXX) $(CXXFLAGS) -c $< -o $@

.c.o:
	$(CC) $(CFLAGS) -c $< -o $@

.cc:
	$(CXX) -o $@ $< $(CXXFLAGS) $(LDFLAGS) -lssl -lcrypto

