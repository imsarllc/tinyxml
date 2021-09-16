cmake_minimum_required(VERSION 3.13)

project(tinyxml CXX)

set(CMAKE_CXX_STANDARD 11)

add_library(tinyxml)
add_library(tinyxml::tinyxml ALIAS tinyxml)

# Allows cmake to turn STL use on or off
if (TIXML_USE_STL)
  # This needs to be public because any consumer that includes tinyxml.h
  # will need TIXML_USE_STL defined
  target_compile_definitions(tinyxml PUBLIC TIXML_USE_STL)
endif()

target_include_directories(tinyxml
  PUBLIC include
  PRIVATE include/tinyxml
  )

add_subdirectory(src)
add_subdirectory(test)

  
