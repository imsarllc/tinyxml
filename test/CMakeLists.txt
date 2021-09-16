cmake_minimum_required(VERSION 3.13)

add_executable(tinyxml_test EXCLUDE_FROM_ALL)

target_link_libraries(tinyxml_test PRIVATE tinyxml)
target_sources(tinyxml_test PRIVATE
  xmltest.cpp
  )

