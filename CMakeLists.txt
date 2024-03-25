cmake_minimum_required(VERSION 3.15)
project(http-test-client CXX)

find_package(cpr REQUIRED)

add_executable(${PROJECT_NAME} src/main.c)
target_link_libraries(${PROJECT_NAME} cpr::cpr)