cmake_minimum_required(VERSION 3.10)

# set the project name and version
project(Playground VERSION 0.0.1)

# specify the C++ standard
set(CMAKE_CXX_STANDARD 20)

set(CMAKE_MODULE_PATH ${CMAKE_BINARY_DIR} ${CMAKE_MODULE_PATH})
include(${CMAKE_BINARY_DIR}/conanbuildinfo.cmake)
conan_basic_setup()

find_package(fmt)

add_executable(playground src/main.cpp)
target_link_libraries(playground ${CONAN_LIBS})
