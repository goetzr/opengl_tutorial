find_package(glfw3 REQUIRED CONFIG)

add_executable(draw_triangle draw_triangle.cpp ${draw_triangle_SOURCE_DIR}/../glad/glad.c)
target_include_directories(draw_triangle PRIVATE ${draw_triangle_SOURCE_DIR}/../glad/include)
target_link_libraries(draw_triangle glfw GL dl)