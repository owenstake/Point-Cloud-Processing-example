cmake_minimum_required(VERSION 2.6 FATAL_ERROR)

project(pcl-interactive_icp)

find_package(PCL 1.5 REQUIRED)

include_directories(${PCL_INCLUDE_DIRS})
link_directories(${PCL_LIBRARY_DIRS})
add_definitions(${PCL_DEFINITIONS})

add_executable (LiveCloud LiveCloud.cpp)
target_link_libraries (LiveCloud ${PCL_LIBRARIES})
