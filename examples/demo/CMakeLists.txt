set(EXAMPLE_NAME demo)

set(EXAMPLE_SRCS
        main.cpp
    )

set(EXAMPLE_RES_SRCS
        demo.qrc
     )

qt5_add_resources(EXAMPLE_QRC_SRCS ${EXAMPLE_RES_SRCS})

add_executable(${EXAMPLE_NAME} ${EXAMPLE_SRCS} ${EXAMPLE_QRC_SRCS})
target_link_libraries(${EXAMPLE_NAME} ${PROJECT_NAME})
