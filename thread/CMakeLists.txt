cmake_minimum_required(VERSION 3.2)

project(thread VERSION 1.0 LANGUAGES C)

set(SOURCES thread.c)
set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -fPIC")

add_library(thread STATIC ${SOURCES})
target_include_directories(thread PRIVATE ..)