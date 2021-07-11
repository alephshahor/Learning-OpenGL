cmake_minimum_required(VERSION 3.19)
project(LearnOpenGL)

set(CMAKE_CXX_STANDARD 20)

#add_subdirectory(/usr/local/Cellar/glfw/3.3.4/)
#include_directories(/usr/local/Cellar/glfw/3.3.4/include)
#include_directories(${PROJECT_SOURCE_DIR}/include/GLFW)
include_directories(${CMAKE_SOURCE_DIR}/include)

add_executable(LearnOpenGL main.cpp)
target_link_libraries(LearnOpenGL ${PROJECT_SOURCE_DIR}/lib/GLFW/libglfw.3.dylib)