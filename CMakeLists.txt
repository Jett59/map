cmake_minimum_required(VERSION 3.15)

project(map LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED true)

add_library(map src/map.cpp)

add_executable(time src/time.cpp)

target_link_libraries(time map)
