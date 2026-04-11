cmake_minimum_required(VERSION 3.10)
project(HelloTriangle)

set(CMAKE_CXX_STANDARD 17)

include_directories(
    /Users/tachibis/LocalDocuments/OpenGL/include
)

link_directories(
    /Users/tachibis/LocalDocuments/OpenGL/lib
)

add_executable(HelloTriangle main.cpp glad.c)


target_link_libraries(HelloTriangle
    libglfw3.a
    "-framework Cocoa"
    "-framework OpenGL"
    "-framework IOKit"
)
