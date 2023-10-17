apt update
apt install g++ -y



cmake .
make
./helloworld




# cmake .
-- The C compiler identification is GNU 7.5.0
-- The CXX compiler identification is GNU 7.5.0
-- Check for working C compiler: /usr/bin/cc
-- Check for working C compiler: /usr/bin/cc -- works
-- Detecting C compiler ABI info
-- Detecting C compiler ABI info - done
-- Detecting C compile features
-- Detecting C compile features - done
-- Check for working CXX compiler: /usr/bin/c++
-- Check for working CXX compiler: /usr/bin/c++ -- works
-- Detecting CXX compiler ABI info
-- Detecting CXX compiler ABI info - done
-- Detecting CXX compile features
-- Detecting CXX compile features - done
-- Configuring done
-- Generating done
-- Build files have been written to: /root/xxx
#


# make
Scanning dependencies of target helloworld
[ 50%] Building CXX object CMakeFiles/helloworld.dir/main.cpp.o
[100%] Linking CXX executable helloworld
[100%] Built target helloworld
#


# ./helloworld
hello world
#
