cmake_minimum_required(VERSION 2.8)
project(server)

set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -Wall -Wextra")

find_package (Threads)
set(SOURCE_FILES server.c)
add_executable(server ${SOURCE_FILES})

target_link_libraries (server ${CMAKE_THREAD_LIBS_INIT})
