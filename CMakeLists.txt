cmake_minimum_required(VERSION 3.0.0)
project(DisplayImage VERSION 0.1.0 LANGUAGES C CXX)

find_package(OpenCV REQUIRED)

include_directories(${OpenCV_INCLUDE_DIRS})

add_executable(DisplayImage src/DisplayImage.cpp)
target_link_libraries(DisplayImage ${OpenCV_LIBS})

add_executable(Slider src/Slider.cpp)
target_link_libraries(Slider ${OpenCV_LIBS})
