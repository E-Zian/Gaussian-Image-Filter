cmake_minimum_required(VERSION 4.1)
project(Image_Enhancement)

set(CMAKE_CXX_STANDARD 20)
find_package(OpenCV REQUIRED)
add_executable(Image_Enhancement)

target_sources(Image_Enhancement
PRIVATE
        main.cpp
        GaussianKernel.cpp
        ImageEnhancer.cpp
        ImageEnhancer.h
        GaussianKernel.h
)
target_link_libraries(Image_Enhancement ${OpenCV_LIBS})

