# Chapter 03. A Basic C++ Programs

```cpp
#include <iostream>

using namespace std;

int main() {
    cout << "Hello world\n";
    return 0;
}
```

* Every C++ program must have a `main` function. The `main` function is where the program starts.
* The `main` function returns 0, meaning that the program runs successfully. If the `main` function returns a different value, that means there is an error.
* `cout` is an **object** which belongs to the `iostream` library. The cout object is used to print output to the console. You will get to know what object is in the chapter of Structs and Classes.
* To include a library, use the following syntax:
```cpp
#include <library-name>
```
* In C++, namespaces are used to identify groups of names. Roughly speaking, everything defined in the C++ standard library belongs to the `std` namespace - for example, the `cout` object. If you do not have the line `using namespace std,`, then every time you use `cout`, you must type `std::cout` instead of `cout` only. You will get to know about namespace is in the chapter of Namespaces.
