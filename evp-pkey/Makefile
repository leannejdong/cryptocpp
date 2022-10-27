
SOURCES= evp_generate_rsa.cc evp_readkey_file.cc evp_class.cc evp_class.h 
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