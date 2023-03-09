cmake_minimum_required(VERSION 3.4)

project(hello_world)

set(CMAKE_CXX_STANDART 17)

set(CMAKE_CXX_STANDARD_REQUIRED ON)

add_executable(${PROJECT_NAME} hello_world.cpp)

target_include_directories(${PROJECT_NAME} PUBLIC ../formatter_ex_lib)

target_link_libraries(${PROJECT_NAME} formatter_ex)
