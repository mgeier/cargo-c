CFLAGS = `pkg-config --cflags example_project`
LDLIBS = `pkg-config --libs example_project`
LDFLAGS = -static

test: run_tests
	./run_tests

clean:
	$(RM) run_tests
