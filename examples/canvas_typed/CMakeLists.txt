set(EXAMPLE_NAME canvas_typed)

set(CMAKE_AUTOMOC ON)

set(CMAKE_INCLUDE_CURRENT_DIR ON)

set(EXAMPLE_SRCS
        main.cpp
        mainwindow.cpp
        qtcanvas.cpp
    )

add_executable(${EXAMPLE_NAME} ${EXAMPLE_SRCS})
target_link_libraries(${EXAMPLE_NAME} ${PROJECT_NAME})
