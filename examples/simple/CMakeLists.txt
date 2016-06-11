set(EXAMPLE_NAME simple)

set(EXAMPLE_SRCS
        main.cpp
    )

add_executable(${EXAMPLE_NAME} ${EXAMPLE_SRCS})
target_link_libraries(${EXAMPLE_NAME} ${PROJECT_NAME})
