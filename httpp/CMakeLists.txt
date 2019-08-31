cmake_minimum_required(VERSION 3.2)

project(httpp VERSION 1.0 LANGUAGES C)

set(SOURCES encoding.c httpp.c)
set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -fPIC")

add_library(httpp STATIC ${SOURCES})
target_include_directories(httpp PRIVATE ..)