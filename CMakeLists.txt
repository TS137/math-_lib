cmake_minimum_required(VERSION 3.22)
project(math-_lib VERSION 0.1)

add_library(math_lib STATIC math_ops.c)
target_include_directories(math_lib  PUBLIC math_ops.h)

add_executable(math-_lib main.c)
target_link_libraries(math-_lib math_lib)



