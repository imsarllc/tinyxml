cmake_minimum_required(VERSION 3.13)

project(tinyxml CXX)

set(CMAKE_CXX_STANDARD 11)

add_library(tinyxml)
add_library(tinyxml::tinyxml ALIAS tinyxml)

target_include_directories(tinyxml
  PUBLIC include
  PRIVATE include/tinyxml
  )

add_subdirectory(src)
add_subdirectory(test)

  
