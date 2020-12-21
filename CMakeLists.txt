cmake_minimum_required(VERSION 3.17)
project(automatic_linting)

set(CMAKE_CXX_STANDARD 17)
add_definitions("-Wall -Wextra")

add_executable(format_me src/format_me.cpp)