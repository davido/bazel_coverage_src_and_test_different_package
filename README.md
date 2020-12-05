### Reproducer for bazel test coverage problem


````
  $ bazel coverage --test_output=all src/test/java/com/example:test
````


The `coverage.dat` file is empty:

```
WARNING: There was no coverage found.
================================================================================
Target //src/test/java/com/example:test up-to-date:
  bazel-bin/src/test/java/com/example/test.jar
  bazel-bin/src/test/java/com/example/test
INFO: Elapsed time: 20.090s, Critical Path: 6.83s
INFO: 21 processes: 10 internal, 8 linux-sandbox, 3 worker.
INFO: Build completed successfully, 21 total actions
//src/test/java/com/example:test                                         PASSED in 0.8s

Executed 1 out of 1 test: 1 test passes.
INFO: Build completed successfully, 21 total actions
```

