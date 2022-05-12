cmake_minimum_required(VERSION 3.21)
project(Caller)

set(CMAKE_CXX_STANDARD 14)
set(CMAKE_AUTOMOC ON)
set(CMAKE_AUTORCC ON)
set(CMAKE_AUTOUIC ON)

set(CMAKE_PREFIX_PATH "C:\\Qt\\5.15.2\\mingw81_64\\lib\\cmake")

find_package(Qt5Widgets
        REQUIRED)

add_executable(Caller main.cpp caller.ui callerMainWindow.h)
target_link_libraries(Caller
        Qt5::Widgets
        )