# Set the minimum version of CMake that can be used
# To find the cmake version run
# $ cmake --version
cmake_minimum_required(VERSION 3.5)

# Set the project name
project (macserial)

include_directories(${PROJECT_SOURCE_DIR}/Project/MacSerialPort/SerialPort)
include_directories(${PROJECT_SOURCE_DIR}/Project/MacSerialPort/TypeAbbreviations)

# Add an executable
add_executable(macserial  ${PROJECT_SOURCE_DIR}/Project/MacSerialPort/main.cpp ${PROJECT_SOURCE_DIR}/Project/MacSerialPort/SerialPort/SerialPort.cpp )