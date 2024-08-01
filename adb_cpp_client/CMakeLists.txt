cmake_minimum_required(VERSION 3.13 FATAL_ERROR)

file(GLOB_RECURSE ADB_CPP_CLIENT_SRCS ${PROJECT_SOURCE_DIR}/adb_cpp_client/adb_cpp_client.cc)

add_executable(adb_cpp_client ${ADB_CPP_CLIENT_SRCS})
set_target_properties(adb_cpp_client PROPERTIES LINKER_LANGUAGE CXX)
add_dependencies(adb_cpp_client adb_cpp_lib)