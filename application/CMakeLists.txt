cmake_minimum_required(VERSION 3.30)

project(cmake-discourse-example)

add_executable(application)

target_sources(application
  PRIVATE
    app.cpp
)

add_subdirectory(${CMAKE_SOURCE_DIR}/../lib1)

target_link_libraries(application
  PRIVATE
    lib1
)

enable_testing()
add_test(NAME application COMMAND application)
