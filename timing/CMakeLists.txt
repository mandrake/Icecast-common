cmake_minimum_required(VERSION 3.2)

project(timing VERSION 1.0 LANGUAGES C)

set(SOURCES timing.c)
set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -fPIC")

add_library(timing STATIC ${SOURCES})
target_include_directories(timing PRIVATE ..)