create CMakeLists.txt
vim this
add_executable(a.out main.cpp)

cmake -B build
cd build
make clean
make

