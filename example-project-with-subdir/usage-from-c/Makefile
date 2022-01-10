CFLAGS = `pkg-config --cflags example_project_with_subdir`
LDLIBS = `pkg-config --libs example_project_with_subdir`
LDFLAGS = -static

test: run_tests
	./run_tests

clean:
	$(RM) run_tests
