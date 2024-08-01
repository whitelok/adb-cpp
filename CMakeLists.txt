cmake_minimum_required(VERSION 3.13 FATAL_ERROR)

project(adb_cpp LANGUAGES CXX)

include_directories(
  ${PROJECT_SOURCE_DIR}
  ${PROJECT_SOURCE_DIR}/include
)

add_subdirectory(adb)
add_subdirectory(adb_cpp_client)