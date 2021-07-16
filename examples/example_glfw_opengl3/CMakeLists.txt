get_filename_component(_name ${CMAKE_CURRENT_SOURCE_DIR} NAME_WLE)

add_executable(${_name} main.cpp ${CMAKE_CURRENT_SOURCE_DIR}/../libs/gl3w/GL/gl3w.c)
target_link_libraries(${_name} dl imgui backends)
