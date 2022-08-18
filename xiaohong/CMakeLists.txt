cmake_minimum_required(VERSION 3.22)
project(xiaohong)

set(CMAKE_CXX_STANDARD 11)

add_executable(${PROJECT_NAME} ${PROJECT_SOURCE_DIR}/main.cpp)
target_link_libraries(${PROJECT_NAME} PUBLIC lib::apple)