cmake_minimum_required(VERSION 3.2)

project(avl VERSION 1.0 LANGUAGES C)

set(SOURCES avl.c)
set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -fPIC")

add_library(avl STATIC ${SOURCES})
target_include_directories(avl PRIVATE ..)