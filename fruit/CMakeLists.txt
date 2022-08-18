project(fruit)

add_library(${PROJECT_NAME} STATIC ${PROJECT_SOURCE_DIR}/src/fruit.cpp)
add_library(lib::fruit ALIAS ${PROJECT_NAME})

target_include_directories(${PROJECT_NAME}
        PUBLIC ${PROJECT_SOURCE_DIR}/include)