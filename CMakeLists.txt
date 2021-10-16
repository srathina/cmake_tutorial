cmake_minimum_required(VERSION 3.21)  #set the minimum version required to run on another machine

set(target nameexe) 
#set the target name for exe


include_directories(${CMAKE_CURRENT_SOURCE_DIR}) 
#include the header file directories path

add_library(namelib name.c) 
#create a library

add_executable(${target} main.c)
#create an executable

target_link_libraries(${target} namelib)
#link the exectuable with library.