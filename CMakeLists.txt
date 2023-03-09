cmake_minimum_required(VERSION 3.4)

project(main)

set(CMAKE_CXX_STANDART 17)

set(CMAKE_CXX_STANDARD_REQUIRED ON)

add_subdirectory(formatter_lib)
add_subdirectory(formatter_ex_lib)
add_subdirectory(hello_world_application)
add_subdirectory(solver_lib)
add_subdirectory(solver_application)

