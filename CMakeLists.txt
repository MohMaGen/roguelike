cmake_mininmum_required(VERSION 3.20)

progect(roguelike LANGUAGES CXX)

set(CMAKE_CXX_COMPILER clang++)
set(CMAKE_COMPILER_FLAGS "-Wall -G")

set(LIB_OUTPUT_DIR ${CMAKE_SOURCE_DIR}/target/lib/)
set(RUNTIME_OUTPUT_DIRECTORY ${CMAKE_SOURCE_DIR}/target/bin)

add_subdirectorty(code)
