cmake_minimum_required(VERSION 3.13)

target_include_directories(tinyxml
  PRIVATE ${CMAKE_CURRENT_LIST_DIR}
  )

target_sources(tinyxml PRIVATE
  tinystr.cpp
  tinyxml.cpp
  tinyxmlerror.cpp
  tinyxmlparser.cpp
  )
