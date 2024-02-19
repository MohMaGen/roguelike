cmake_minimum_required(VERSION 3.1)

project(roguelike LANGUAGES CXX)

set(CMAKE_COMPILER_FLAGS "-Wall -G")
set(CMAKE_CXX_STANDARD 20)

set(LIB_OUTPUT_DIR ${CMAKE_SOURCE_DIR}/target/lib/)
set(RUNTIME_OUTPUT_DIRECTORY ${CMAKE_SOURCE_DIR}/target/bin)

find_package(glfw3 REQUIRED)
find_package(glm REQUIRED)


option(NDEBUG "specify debug or release build." off)



add_subdirectory(external/ecs_lib)
add_subdirectory(code)
