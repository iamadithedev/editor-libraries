project(imgui)

add_library(${PROJECT_NAME})

target_include_directories(${PROJECT_NAME} PUBLIC .)
target_link_libraries(${PROJECT_NAME} PRIVATE glfw)

target_sources(${PROJECT_NAME} PRIVATE imgui.cpp imgui_draw.cpp imgui_widgets.cpp imgui_tables.cpp
                                       backends/imgui_impl_glfw.cpp backends/imgui_impl_opengl3.cpp)