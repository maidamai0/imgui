cmake_minimum_required(VERSION 3.20)
project(imgui)

file(GLOB srcs *.cpp)
add_library(imgui STATIC ${srcs})

include_directories(${CMAKE_CURRENT_SOURCE_DIR})
include_directories(${CMAKE_CURRENT_SOURCE_DIR}/backends)
include_directories(${CMAKE_CURRENT_SOURCE_DIR}/examples/libs/gl3w)

add_compile_definitions(IMGUI_IMPL_OPENGL_LOADER_GL3W)

add_subdirectory(backends)
add_subdirectory(examples)
