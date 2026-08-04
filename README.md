# C-turn-based-console-game
A tutorial project for practicing object-oriented programming in C++

# Build
## 1. Compile Dynamic lib for My_vector
g++ -fPIC -shared -o .\dyn_lib\My_vector.so .\My_vector\My_vector.cpp
## 2. Compile & Link all other files
g++  .\src\\*.cpp -I .\My_vector\ -L .\dyn_lib\My_vector.so -o game
