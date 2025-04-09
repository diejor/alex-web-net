cmake_minimum_required(VERSION 3.15..4.0)
project(
    alexwebnet 
    VERSION 1.0
    LANGUAGES CXX
)

find_package(Dawn REQUIRED)

add_executable(alexwebnet main.cpp)

target_link_libraries(alexwebnet dawn::webgpu_dawn)
