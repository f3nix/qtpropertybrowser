cmake_minimum_required(VERSION 2.8.11)

project(QtPropertyBrowser)

find_package(Qt5Widgets REQUIRED)

add_subdirectory(src)

option(BUILD_EXAMPLES "Build examples" ON)
if(BUILD_EXAMPLES)
    add_subdirectory(examples)
endif()
