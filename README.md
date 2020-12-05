# Garbage-Collector
* This project is about implementing a customized garbage collector, by using C++ default pointers. In addition,verification of memory leakage is provided to confirm the correctness of implementing such a garbage collector.
* In this project, a simple garbage collector pointer class has been implemented. The garbage collector basically uses three classes: `Pointer`, `PtrDetails` and `Iter`:
  * `Pointer` is the core garbage collector class, which implements a garbage-collection pointer
  * `PtrDetails` maintains a list reference counts with allocated memory, and bonds a reference count to a piece of allocated memory
  * `Iter` is a template class similar in function to an `STL` iterator, and it defines all pointer *operations*, including pointer arithmetic, such as `*`, `->`, `begin()`, and `end()`, which work much like their equivalents in the `STL`.

# Building
To build this project, you will need a C++ compiler. The `make` script provided
assumes the GCC compiler, however you may substitute an equivalent C++ compiler
by adjusting the `make` script as needed. Execute the make script, then run the
compiled executable.

If the code fails to compile, the execute won't be created or will remain the
last-compiled version. Adjust your code to resolve compiler errors and try again.

``` shell
$ ./make
$ ./compiled
```

## Reference:
- Udacity nanodegree repo `CppND-Garbage-Collector`

  https://github.com/udacity/CppND-Garbage-Collector

