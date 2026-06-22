cmake_minimum_required(VERSION 3.16)

project(HexEditor)

set(CMAKE_CXX_STANDARD 17)

find_package(Qt6 REQUIRED COMPONENTS Widgets)

add_executable(HexEditor
    src/main.cpp
    src/Window/window.cpp
)   

target_link_libraries(HexEditor Qt6::Widgets)