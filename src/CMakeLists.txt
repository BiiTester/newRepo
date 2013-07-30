cmake_minimum_required (VERSION 2.6)


project (zlib)

include_directories(${CMAKE_SOURCE_DIR}/include)
link_directories (${CMAKE_SOURCE_DIR}/lib)

add_executable (zlib zpipe.c)

target_link_libraries (zlib zlibd)