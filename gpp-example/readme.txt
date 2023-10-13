g++ *.cpp
./a.out





g++ -c helloworld.cpp  main.cpp
g++ -o helloworld helloworld.o main.o
./helloworld









Default Compilation
g++ <filename> compiles a file named "filename" into an executable named "a.out"
Renaming the Output
g++ -o <execname> <filename> compiles a file named "filename" into an executable named "execname"
whatever immediately follows the "-o" becomes the executable name

Creating Object Code
Object code is source code that has been compiled down to machine language (binary) but has not yet been linked with all the libraries and other files.
g++ -c <filename> compiles a file named "filename" into object code named "filename.o"



Linking Object Code
Once object code has been created, an executable can be created by linking the object code with other precompiled pieces of code (other ".o" files)
All the standard libraries have object code compiled for them
g++ -o <execname> filename.o links the object code "filename.o" with any of its libraries and creates an executable named "execname"

Linking External Libraries
Occasionally a library will be needed that is not linked by default
Use the "-l" option to link in the extra library object code
g++ -o <execname> <filename> -lxnet compiles a executable named "execname", from a file named "filename", using the library that contains  the object code for sockets (sys/socket.h)
