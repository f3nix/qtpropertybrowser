set(EXAMPLE_NAME extension)

set(CMAKE_AUTOMOC ON)

set(CMAKE_INCLUDE_CURRENT_DIR ON)

set(EXAMPLE_SRCS
        main.cpp
    )

add_executable(${EXAMPLE_NAME} ${EXAMPLE_SRCS})
target_link_libraries(${EXAMPLE_NAME} ${PROJECT_NAME})
