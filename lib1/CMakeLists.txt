add_library(lib1)

target_sources(lib1
  PRIVATE
    lib1.cpp

  INTERFACE
    FILE_SET interface_headers
    TYPE HEADERS
    BASE_DIRS
      ${CMAKE_CURRENT_SOURCE_DIR}
    FILES
      lib1.hpp
)
