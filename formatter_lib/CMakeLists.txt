cmake_minimum_required(VERSION 3.4)

project(formatter)

set(CMAKE_CXX_STANDART 17)

set(CMAKE_CXX_STANDARD_REQUIRED ON)

add_library(${PROJECT_NAME} STATIC formatter.cpp)
