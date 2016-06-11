set(CMAKE_INCLUDE_CURRENT_DIR ON)
set(CMAKE_AUTOMOC ON)

include_directories(${CMAKE_BINARY_DIR})

set(QTPROPERTYBROWSER_SRCS
        qtbuttonpropertybrowser.cpp
        qteditorfactory.cpp
        qtgroupboxpropertybrowser.cpp
        qtpropertybrowser.cpp
        qtpropertybrowserutils.cpp
        qtpropertymanager.cpp
        qttreepropertybrowser.cpp
        qtvariantproperty.cpp
   )

set(QTPROPERTYBROWSER_RES_SRCS
    qtpropertybrowser.qrc
   )

qt5_add_resources(QTPROPERTYBROWSER_QRC_SRCS ${QTPROPERTYBROWSER_RES_SRCS})

add_library(${PROJECT_NAME} ${QTPROPERTYBROWSER_SRCS} ${QTPROPERTYBROWSER_QRC_SRCS})
target_link_libraries(${PROJECT_NAME} Qt5::Widgets)
