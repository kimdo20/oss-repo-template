cmake_minimum_required(VERSION 3.0)
project(Blocks)

add_library(stat STATIC source/block.c headers/block.h)
add_library(dyna SHARED source/block.c headers/block.h)

add_executable(prog1 program.c)
target_link_libraries(prog1 stat)

add_executable(prog2 program.c)
target_link_libraries(prog2 dyna)