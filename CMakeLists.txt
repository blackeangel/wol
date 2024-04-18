cmake_minimum_required(VERSION 3.27)
project(wol)

set(CMAKE_CXX_STANDARD 20)
set(CMAKE_EXE_LINKER_FLAGS "-static")
set(CMAKE_CXX_FLAGS_RELEASE "-O2")
add_executable(wol main.cpp)
target_link_libraries(wol ${CMAKE_SOURCE_DIR}/libwsock32.a)