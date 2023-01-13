cmake_minimum_required(VERSION 3.0)
project(cccc)

find_package(OpenCV  REQUIRED)

include_directories(${OpenCV_INCLUDE_DIRS})

add_executable(main main.cc)

target_link_libraries(main ${OpenCV_LIBS})