#
#
#
SRC := commands.c network.c sys_bsd.c terminal.c ring.c telnet.c utilities.c main.c genget.c
OBJ := commands.o network.o sys_bsd.o terminal.o ring.o telnet.o utilities.o main.o genget.o 
ADDLIB := libncurses.5.4.tbd 
LIBPATH := /Applications/Xcode.app/Contents/Developer/Platforms/MacOSX.platform/Developer/SDKs/MacOSX.sdk/usr/lib/
CLEANFILES := telnet $(OBJ)

#----------------------
.c.o: $(SRC)
	cc -DUSE_TERMIO -c $(SRC)

telnet: $(OBJ)
	cc -lsystem $(LIBPATH)$(ADDLIB) -o telnet $(OBJ)

clean:
	rm $(CLEANFILES)
#----------------------
# Sources files
main.o: main.c
commands.o: commands.c
network.o: network.c
sys_bsd.o: sys_bsd.c
terminal.o: terminal.c
ring.o: ring.c
telnet.o: telnet.c
utilities.o: utilities.c
genget.o: genget.c
#----------------------
# End of Makefile
