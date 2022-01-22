test-both: test-shared test-static

test-shared: run_tests
	./run_tests

test-static: run_tests_static
	./run_tests_static

clean:
	$(RM) run_tests run_tests_static

run_tests: LDLIBS = -lexample_project

run_tests_static: LDLIBS = `pkg-config --static --libs example_project`

%_static: %.c
	$(LINK.c) $^ -static $(LDLIBS) -o $@

.PHONY: test-both test-shared test-static clean
