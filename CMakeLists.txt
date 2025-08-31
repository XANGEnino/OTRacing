cmake_minimum_required(VERSION 3.16)
project(OTRacing)

# Set C++ standard
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

# Add submodules
add_subdirectory(external/glfw)
add_subdirectory(external/glad)

# Add source files
add_executable(OTRacing src/main.cpp)

# For include directories (later when adding libraries)
# target_include_directories(OTRacing PRIVATE include)
target_link_libraries(OTRacing PRIVATE glfw)
target_link_libraries(OTRacing PRIVATE glad)