
SOURCES= evp_display.cc evp_file_encrypt.cc evp_file_decrypt.cc evp_class.cc evp_class.h 
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

