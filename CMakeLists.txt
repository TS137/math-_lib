cmake_minimum_required(VERSION 3.22)
project(math-_lib VERSION 0.2)

add_library(math_lib STATIC inc/math_ops.c)
target_include_directories(math_lib  PUBLIC inc/)

add_executable(math-_lib src/main.c)
target_link_libraries(math-_lib math_lib)



