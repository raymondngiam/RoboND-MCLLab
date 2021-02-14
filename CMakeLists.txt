project(RoboND-MCLLab)
cmake_minimum_required(VERSION 3.19)

set(CMAKE_CXX_STANDARD 17)

find_package(Python3 COMPONENTS Development NumPy)
include_directories(${Python3_INCLUDE_DIRS} 
  ${Python3_NumPy_INCLUDE_DIRS})
  
set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${PROJECT_SOURCE_DIR}/bin)
set(CMAKE_LIBRARY_OUTPUT_DIRECTORY ${PROJECT_SOURCE_DIR}/lib)
set(CMAKE_ARCHIVE_OUTPUT_DIRECTORY ${PROJECT_SOURCE_DIR}/lib)

add_subdirectory(${PROJECT_SOURCE_DIR}/src)
