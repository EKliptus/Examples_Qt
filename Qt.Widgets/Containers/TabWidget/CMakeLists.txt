cmake_minimum_required(VERSION 3.1)

# Project
project(TabWidget)
find_package(Qt5Widgets CONFIG REQUIRED)

# Options
set(CMAKE_AUTOMOC ON)
set(CMAKE_AUTORCC ON)
set(CMAKE_AUTOUIC ON)
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

# Application
add_executable(TabWidget WIN32 MACOSX_BUNDLE src/TabWidget.cpp src/TabWidget.h)
target_link_libraries(TabWidget Qt5::Widgets)
set_target_properties(${PROJECT_NAME} PROPERTIES FOLDER "Containers")
