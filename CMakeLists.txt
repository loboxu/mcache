cmake_minimum_required(VERSION 3.12)
project(mcache)

set(CMAKE_CXX_STANDARD 11)

add_executable(mcache main.cpp)

message(${mcache_SOURCE_DIR})

add_custom_target(mcache_makefile COMMAND make -C ${mcache_SOURCE_DIR})