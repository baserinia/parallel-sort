# C++ Parallel Sort
An efficient C++ multi-threaded sorting function based on C++11 threads

## How to use
To use this function, simply include the the file `parasort.h` in your program and call the template function `parasort(sz, list, np, sf)`
with proper argument values. Here is the list of arguments:
* sz: Length of array of type `size_t`;
* list: Array of arbitrary type `T`. This array is used as both input and output since the sorted output is written to it.
If `T` is not a built-in type, overload the operator `<`.
* np: Number of concurrent threads. By default, `np=2`, so it can be omitted.
* sf: Sampling factor. By default `sf=100', so it can be omitted.

## How to compile
This function uses only the standard C++ constructs, so you can compile it like any other C++ program. Just make sure you are
using these flags in gcc:
* -std=c++11
* -pthread
