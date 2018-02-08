cmake_minimum_required(VERSION 2.8)
project(protobuf CXX)

###############
# ASI default settings
list(APPEND CMAKE_MODULE_PATH "$ENV{ASV_CMAKE}")
include(asv_cmake_defaults)
asv_cmake_defaults( )
###############

if (MSVC)
    set (BUILD_SHARED_LIBS 0)
else (MSVC) # UNIX
    set (BUILD_SHARED_LIBS 1)
endif (MSVC)
set (protobuf_BUILD_TESTS OFF)

add_subdirectory(cmake)
