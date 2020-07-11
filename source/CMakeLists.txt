cmake_minimum_required (VERSION 3.4)
project (seqan3_tutorial CXX)
 
find_package (SeqAn3 3.0.0 REQUIRED HINTS "${CMAKE_SOURCE_DIR}/../seqan3/build_system")
 
add_executable (hello_world hello_world.cpp)
 
target_link_libraries (hello_world seqan3::seqan3)
