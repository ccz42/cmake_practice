cmake_minimum_required(VERSION 3.16)
project(cmake_practice VERSION 1.0 LANGUAGES CXX)
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
add_executable(talker
talker/src/calculator.cpp
talker/src/main.cpp
)
target_include_directories(talker PRIVATE talker/include)
add_executable(
listener
listener/src/calculator.cpp
listener/src/main.cpp
)
target_include_directories(listener PRIVATE listener/include)
