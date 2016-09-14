cmake_minimum_required(VERSION 2.8)

project( stitching_detailed_x )

set(CMAKE_BUILD_TYPE "Debug")
set(CMAKE_CXX_FLAGS_DEBUG "$ENV{CXXFLAGS} -O0 -Wall -g2 -ggdb")

find_package( OpenCV REQUIRED )
add_executable( stitching_detailed_x stitching_detailed_x.cpp )
target_link_libraries( stitching_detailed_x ${OpenCV_LIBS} )
