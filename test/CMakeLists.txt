cmake_minimum_required(VERSION 3.13)

add_executable(test EXCLUDE_FROM_ALL)

target_link_libraries(test PRIVATE tinyxml)
target_sources(test PRIVATE
  xmltest.cpp
  )

