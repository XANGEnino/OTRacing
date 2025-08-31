cmake_minimum_required(VERSION 3.16)
project(OTRacing)

# Set C++ standard
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

# Add source files
add_executable(OTRacing src/main.cpp)

# For include directories (later when adding libraries)
target_include_directories(OTRacing PRIVATE include)