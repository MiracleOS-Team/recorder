cmake_minimum_required(VERSION 1.14)

project(miracle-recorder LANGUAGES CXX)

set(CMAKE_INCLUDE_CURRENT_DIR ON)

set(CMAKE_AUTOUIC ON)
set(CMAKE_AUTOMOC ON)
set(CMAKE_AUTORCC ON)

set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

find_package(Qt5 COMPONENTS Core Quick Multimedia LinguistTools REQUIRED)
find_package(MeuiKit)

add_subdirectory(src)

install(FILES miracle-recorder.desktop DESTINATION "/usr/share/applications")
