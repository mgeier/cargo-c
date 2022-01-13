CFLAGS = `pkg-config --cflags example_project` -fno-builtin
LDLIBS = `pkg-config --libs example_project --static`
LDFLAGS = -static

test: run_tests
	./run_tests

clean:
	$(RM) run_tests
