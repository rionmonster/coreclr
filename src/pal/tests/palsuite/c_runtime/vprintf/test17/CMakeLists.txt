cmake_minimum_required(VERSION 2.8.12.2)

set(CMAKE_INCLUDE_CURRENT_DIR ON)

set(SOURCES
  test17.cpp
)

add_executable(paltest_vprintf_test17
  ${SOURCES}
)

add_dependencies(paltest_vprintf_test17 coreclrpal)

target_link_libraries(paltest_vprintf_test17
  ${COMMON_TEST_LIBRARIES}
)
