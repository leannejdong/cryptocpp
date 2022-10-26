
SOURCES=evp_digest_disp.cc evp_digest_file.cc evp_digest_verify.cc

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

