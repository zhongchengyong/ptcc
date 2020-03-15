cmake_minimum_required(VERSION 3.15)
project(tcc)
add_subdirectory(src)
add_subdirectory(test)

set(CMAKE_CXX_STANDARD 17)

add_executable(tcc main.cpp)

target_link_libraries(tcc compiler)
