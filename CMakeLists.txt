cmake_minimum_required(VERSION 3.14)

project(test-string)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

set(CMAKE_TOOLCHAIN_FILE "${CMAKE_SOURCE_DIR}/toolchain.cmake" CACHE FILEPATH "Toolchain file")
set(CMAKE_CONFIGURATION_TYPES "Debug;Release" CACHE STRING "" FORCE)

set(INDEX "2")

configure_file(array_template.cpp.in array.cpp @ONLY)
add_executable(test-string array.cpp)
