set (glad_SOURCES
    ${CMAKE_CURRENT_SOURCE_DIR}/src/glad.c
)

add_library(glad ${glad_SOURCES})

set_target_properties(glad PROPERTIES
    OUTPUT_NAME glad
    POSITION_INDEPENDENT_CODE ON)

target_include_directories(glad PUBLIC
    ${CMAKE_CURRENT_SOURCE_DIR}/include)