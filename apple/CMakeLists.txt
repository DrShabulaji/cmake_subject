project(apple)

add_library(${PROJECT_NAME} STATIC ${PROJECT_SOURCE_DIR}/src/apple.cpp)
add_library(lib::apple ALIAS ${PROJECT_NAME})

target_include_directories(${PROJECT_NAME}
        PUBLIC ${PROJECT_SOURCE_DIR}/include)

# 链接fruit库
target_link_libraries(${PROJECT_NAME}
        PRIVATE lib::fruit)
