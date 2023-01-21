cmake_minimum_required(VERSION 3.0.0)
project(F111)
find_package(GTest REQUIRED)

add_executable(main main.cpp)
add_library(myLib  functions.cpp)

target_link_libraries(main
 PRIVATE
  GTest::GTest)

enable_testing()