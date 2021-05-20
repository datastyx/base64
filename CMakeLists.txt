cmake_minimum_required(VERSION 3.0.0)
project(base64 VERSION 0.1.0)
add_library(${PROJECT_NAME} STATIC )
target_include_directories (${PROJECT_NAME} PUBLIC ${CMAKE_CURRENT_SOURCE_DIR}/include)
target_sources(${PROJECT_NAME} PRIVATE ${CMAKE_CURRENT_SOURCE_DIR}/src/base64.c)
set(CPACK_PROJECT_NAME ${PROJECT_NAME})
set(CPACK_PROJECT_VERSION ${PROJECT_VERSION})
include(CPack)



