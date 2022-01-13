# cargo-c saves all the information in the .pc file
# Do not try to pass simply -lname since it will not work for static linking

LDLIBS = `pkg-config --libs example_project --static`
CFLAGS = `pkg-config --cflags example_project` -fno-builtin
LDFLAGS = -static

test: run_tests
	./run_tests

clean:
	$(RM) run_tests
