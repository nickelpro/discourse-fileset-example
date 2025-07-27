add_executable(application)

target_sources(application
  PRIVATE
    app.cpp
)

target_link_libraries(application
  PRIVATE
    lib1
)
