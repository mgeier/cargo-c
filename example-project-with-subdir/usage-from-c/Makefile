CFLAGS = `pkg-config --cflags example_project_with_subdir` -fno-builtin
LDLIBS = `pkg-config --libs example_project_with_subdir --static`
LDFLAGS = -static

test: run_tests
	./run_tests

clean:
	$(RM) run_tests
