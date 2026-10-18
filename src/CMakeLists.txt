cmake_minimum_required(VERSION 3.10)
project(outCMakeTest)
set(EXECUTABLE_OUTPUT_PATH ${PROJECT_BINARY_DIR}/bin)
aux_source_directory(src SRC_LIST)
include_directories(${PROJECT_SOURCE_DIR}/include)
add_executable(${PROJECT_NAME} ${SRC_LIST})
#2.0
#3.0