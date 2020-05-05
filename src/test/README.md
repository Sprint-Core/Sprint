### Compiling/running unit tests

Unit tests will be automatically compiled if dependencies were met in `./configure`
and tests weren't explicitly disabled.

After configuring, they can be run with `make check`.

To run the sprintd tests manually, launch `src/test/test_sprint`.

To add more sprintd tests, add `BOOST_AUTO_TEST_CASE` functions to the existing
.cpp files in the `test/` directory or add new .cpp files that
implement new BOOST_AUTO_TEST_SUITE sections.

To run the sprint-qt tests manually, launch `src/qt/test/test_sprint-qt`

To add more sprint-qt tests, add them to the `src/qt/test/` directory and
the `src/qt/test/test_main.cpp` file.

### Running individual tests

test_sprint has some built-in command-line arguments; for
example, to run just the getarg_tests verbosely:

    test_sprint --log_level=all --run_test=getarg_tests

... or to run just the doublesprint test:

    test_sprint --run_test=getarg_tests/doublesprint

Run `test_sprint --help` for the full list.

