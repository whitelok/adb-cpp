cmake_minimum_required(VERSION 3.13 FATAL_ERROR)

file(GLOB_RECURSE ADB_CPP_SRCS ${PROJECT_SOURCE_DIR}/adb/*.c)

add_library(adb_cpp_lib SHARED ${ADB_CPP_SRCS})
set_target_properties(adb_cpp_lib PROPERTIES LINKER_LANGUAGE CXX)