cmake_minimum_required(VERSION 3.2)

project(net VERSION 1.0 LANGUAGES C)

set(SOURCES resolver.c sock.c)
set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -fPIC")

add_library(net STATIC ${SOURCES})
target_include_directories(net PRIVATE ..)