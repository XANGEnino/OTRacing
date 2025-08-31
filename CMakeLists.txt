cmake_minimum_required(VERSION 3.16)
project(OTRacing VERSION 1.0.0)

find_package(OpenGL REQUIRED)

file(GLOB SOURCES
    "src/*.cpp"
    "src/*.c"
)

add_executable(OTRacing ${SOURCES})

target_include_directories(OTRacing PRIVATE include)
target_link_libraries(OTRacing PRIVATE "C:/Dev/C++Libs/GLFW/glfw3.lib")
target_link_libraries(OTRacing PRIVATE OpenGL::GL)