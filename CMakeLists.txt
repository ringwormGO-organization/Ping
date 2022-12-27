cmake_minimum_required(VERSION 3.16)

set(CMAKE_BUILD_TYPE Release)

project(ping)

file(GLOB SRC CONFIGURE_DEPENDS "*.c")

add_library(${PROJECT_NAME} SHARED ${SRC})

target_link_libraries(${PROJECT_NAME})
