# GCC Test
cmake_minimum_required(VERSION 3.0)
project(gcc_test)

## C++ Standard: C++17
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED True)

## Output paths
set(CMAKE_BINARY_DIR "bin/${CMAKE_BUILD_TYPE}")
set(EXECUTABLE_OUTPUT_PATH ${CMAKE_BINARY_DIR})
set(LIBRARY_OUTPUT_PATH ${CMAKE_BINARY_DIR})

## Source paths
file(GLOB SOURCES src/*)

## Compile Libraries
add_subdirectory(mylibrary)

## Output
add_executable(gcc_test ${SOURCES})

## Link Libraries
target_link_libraries(gcc_test PUBLIC mylibrary)
target_include_directories(gcc_test PUBLIC
    mylibrary/    
)
