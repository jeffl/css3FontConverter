patch: add_stddef.patch
	if [ ! -f OpenTypeUtilities_patched ]; then patch OpenTypeUtilities.cpp < add_stddef.patch && touch OpenTypeUtilities_patched; fi

ttf2eot: OpenTypeUtilities.o ttf2eot.o
	g++ -o $@ $^

clean:
	rm -f *.o *.core *.obj *.exe core ttf2eot
