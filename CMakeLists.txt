cmake_minimum_required(VERSION 3.19)
project(LearnOpenGL)

set(CMAKE_CXX_STANDARD 20)

include_directories(${CMAKE_SOURCE_DIR}/include)

add_executable(LearnOpenGL main.cpp glad.c)
target_link_libraries(LearnOpenGL ${PROJECT_SOURCE_DIR}/lib/GLFW/libglfw.3.dylib)