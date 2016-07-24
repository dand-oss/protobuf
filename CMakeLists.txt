cmake_minimum_required(VERSION 2.8)
project(protobuf CXX)

###############
# ASI default settings
list(APPEND CMAKE_MODULE_PATH "$ENV{ASI}/cmake/Modules")
include(asv_cmake_defaults)
asv_cmake_defaults( )
###############

set (BUILD_SHARED_LIBS 1)
set (protobuf_BUILD_TESTS OFF)

add_subdirectory(cmake)
