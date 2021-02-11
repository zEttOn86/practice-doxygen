cmake_minimum_required(VERSION 3.10)
project(practice_doxygen)

#--------
# C++ setup
#--------
set(CMAKE_CXX_STANDARD 11)

#--------
# Practice Doxygen executable
#--------
add_subdirectory(src)

#--------
# Build documentations
#--------
add_subdirectory(docs)