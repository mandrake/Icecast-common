cmake_minimum_required(VERSION 3.2)

project(log VERSION 1.0 LANGUAGES C)

set(SOURCES log.c)
set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -fPIC")

add_library(log STATIC ${SOURCES})
target_include_directories(log PRIVATE ..)