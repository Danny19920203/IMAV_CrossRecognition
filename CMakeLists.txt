cmake_minimum_required(VERSION 3.0.2)
project(ImageMatching)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11")

find_package( OpenCV REQUIRED)
 
set(SOURCE_FILES main.cpp TemplateMatching.cpp TemplateMatching.h)
add_executable(ImageMatching ${SOURCE_FILES})

target_link_libraries(ImageMatching ${OpenCV_LIBS} ) 
