# Building a C++ Project using g++

$ lsb_release -a
$ g++ -v (if it is not installed, sudo apt install g++)

create a .cpp file
$ touch main.cpp
$ /path/to/folder/ g++ main.cpp -o calculator

Let's create different files for different functions

$ touch addition.cpp division.cpp print_result.cpp

In order to the linker to see the function definitions ...
$ g++ main.cpp addition.cpp division.cpp print_result.cpp -o calculator

We should write the function declarations in separate header files and not in the main.cpp

$ touch addition.h division.h print_result.h
