cmake_minimum_required(VERSION 2.8.12.2)

set(CMAKE_INCLUDE_CURRENT_DIR ON)

set(SOURCES
  test8.cpp
)

add_executable(paltest_snwprintf_test8
  ${SOURCES}
)

add_dependencies(paltest_snwprintf_test8 coreclrpal)

target_link_libraries(paltest_snwprintf_test8
  pthread
  m
  coreclrpal
)
