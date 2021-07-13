cmake_minimum_required(VERSION 3.19)
project(cppGOL)

set(CMAKE_CXX_STANDARD 20)

find_package(SDL2 REQUIRED)
include_directories(cppGOL ${SDL2_INCLUDE_DIRS})

add_executable(cppGOL main.cpp)
target_link_libraries(cppGOL ${SDL2_LIBRARIES})