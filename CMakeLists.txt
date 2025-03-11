cmake_minimum_required(VERSION 3.22)
project(h2lib)

list(APPEND CMAKE_MODULE_PATH ${CMAKE_SOURCE_DIR}/cmake)

set(H2LIB_INCLUDE_DIR "${CMAKE_SOURCE_DIR}/Library")
set(H2LIB_TESTS_DIR "${CMAKE_SOURCE_DIR}/Tests")

#---------------------------------------------------------------------------#
# Blas                                                                      #
#---------------------------------------------------------------------------#

find_package(BLAS REQUIRED)

#---------------------------------------------------------------------------#
# Lapack                                                                    #
#---------------------------------------------------------------------------#

find_package(LAPACK REQUIRED)

#---------------------------------------------------------------------------#
# Compile library                                                           #
#---------------------------------------------------------------------------#

file(GLOB H2LIB_SOURCES Library/*.c)
add_library(h2lib ${H2LIB_SOURCES})
target_link_libraries(h2lib 
  BLAS::BLAS
  LAPACK::LAPACK
)
target_compile_options(h2lib PUBLIC -DUSE_BLAS)

#---------------------------------------------------------------------------#
# Tests                                                                     #
#---------------------------------------------------------------------------#

add_subdirectory(${H2LIB_TESTS_DIR})
