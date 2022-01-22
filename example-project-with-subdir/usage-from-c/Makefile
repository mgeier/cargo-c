CFLAGS = `pkg-config --cflags example_project_with_subdir`
LDLIBS = `pkg-config --libs example_project_with_subdir`

test-both: test-shared test-static

test-shared: run_tests
	./run_tests

test-static: run_tests_static
	./run_tests_static

clean:
	$(RM) run_tests run_tests_static

%_static: %.c
	$(LINK.c) $^ -static $(LDLIBS) -o $@

.PHONY: test-both test-shared test-static clean
