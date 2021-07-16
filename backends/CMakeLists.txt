get_filename_component(_name ${CMAKE_CURRENT_SOURCE_DIR} NAME_WLE)
add_library(${_name} imgui_impl_glfw.cpp imgui_impl_opengl3.cpp)
target_link_libraries(${_name} PUBLIC glfw GL)
