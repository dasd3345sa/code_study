cmake_minimum_required(VERSION 3.12)
project(
  demo
  VERSION 0.0.1
  LANGUAGES C CXX)
set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_SOURCE_DIR}/bin)

# 全局包含目录
include_directories(${CMAKE_SOURCE_DIR}/include)

# 源文件
file(GLOB test ${CMAKE_SOURCE_DIR}/src/test.c)

# 可执行文件
add_executable(test ${test})