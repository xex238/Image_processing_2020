cmake_minimum_required(VERSION 3.0)

project(lab_00)

find_package(OpenCV REQUIRED)
include_directories(${OpenCV_INCLUDE_DIRS})

add_executable(lab_00 lab_00.cpp)

file(COPY ${CMAKE_CURRENT_SOURCE_DIR}/Cutie_cat.jpg DESTINATION ${CMAKE_CURRENT_BINARY_DIR})

target_link_libraries(lab_00 ${OpenCV_LIBS})