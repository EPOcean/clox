cmake_minimum_required(VERSION 3.0.0)
project(clox LANGUAGES C)

include(CTest)
enable_testing()

add_executable(clox main.c chunk.c value.c memory.c debug.c)

set(CPACK_PROJECT_NAME ${PROJECT_NAME})
set(CPACK_PROJECT_VERSION ${PROJECT_VERSION})
include(CPack)

