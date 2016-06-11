include_directories(
        ${${PROJECT_NAME}_SOURCE_DIR}/src
)

set(EXECUTABLE_OUTPUT_PATH ${PROJECT_BINARY_DIR}/bin)

add_subdirectory(canvas_typed)
add_subdirectory(canvas_variant)
add_subdirectory(decoration)
add_subdirectory(demo)
add_subdirectory(extension)
add_subdirectory(extension_filepath_typed)
add_subdirectory(extension_filepath_variant)
add_subdirectory(object_controller)
add_subdirectory(simple)
