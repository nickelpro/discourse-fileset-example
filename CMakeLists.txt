cmake_minimum_required(VERSION 3.31)

project(cmake-discourse-example)

add_executable(application)

target_sources(application
  PRIVATE
    application/app.cpp
)

add_subdirectory(lib1)

target_link_libraries(application
  PRIVATE
    lib1
)

enable_testing()
add_test(NAME application COMMAND application)
