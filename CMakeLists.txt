cmake_minimum_required(VERSION 3.10)
project(tims-hello-world)

set(CMAKE_CXX_STANDARD 17)

add_library(tims-hello-world STATIC tims_hello_world.cpp tims_hello_world.h)

install(FILES "${CMAKE_BINARY_DIR}/libtims-hello-world.a" DESTINATION lib)
install(FILES "${PROJECT_SOURCE_DIR}/tims_hello_world.h" DESTINATION include)


