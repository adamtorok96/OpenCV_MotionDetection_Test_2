cmake_minimum_required(VERSION 3.6)
project(opencv_test_2)

find_package(OpenCV REQUIRED)
message(STATUS "OpenCV_FOUND = ${OpenCV_FOUND}")

set(CMAKE_CXX_STANDARD 11)

set(SOURCE_FILES main.cpp)
add_executable(opencv_test_2 ${SOURCE_FILES})
target_link_libraries(opencv_test_2 ${OpenCV_LIBS} )