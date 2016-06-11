set(EXAMPLE_NAME extension_filepath_typed)

set(CMAKE_AUTOMOC ON)

set(EXAMPLE_SRCS
        fileedit.cpp
        fileeditfactory.cpp
        filepathmanager.cpp
        main.cpp
        variantfactory.cpp
        variantmanager.cpp
    )

add_executable(${EXAMPLE_NAME} ${EXAMPLE_SRCS})
target_link_libraries(${EXAMPLE_NAME} ${PROJECT_NAME})
