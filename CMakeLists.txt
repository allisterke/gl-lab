cmake_minimum_required(VERSION 3.5)
project(gl_lab)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11")

set(SOURCE_FILES
    examples/abgr.c)

link_directories($ENV{HOME}/.local/lib)

add_executable(gl_lab ${SOURCE_FILES})
target_link_libraries(gl_lab GL GLU glut)