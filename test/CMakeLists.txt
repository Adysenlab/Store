
### cmake requires to contact Itk built libraries 
### load wired tiger 
cmake_minimum_required(VERSION 3.0)
project(Store)
set (CMAKE_CXX_STANDARD 11)
find_package(ITK REQUIRED)
include(${ITK_USE_FILE})
add_executable(HelloWorld HelloWorld.cpp)
target_link_libraries(HelloWorld ${ITK_LIBRARIES})