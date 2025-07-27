cmake_minimum_required(VERSION 3.31)

project(cmake-discourse-example)

add_subdirectory(lib1)
add_subdirectory(application)

enable_testing()
add_test(NAME application COMMAND application)
