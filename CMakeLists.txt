cmake_minimum_required(VERSION 3.10)
project(outCMakeTest)
set(EXECUTABLE_OUTPUT_PATH ${PROJECT_SOURCE_DIR}/bin)
aux_source_directory(${PROJECT_SOURCE_DIR}/src SRC_LIST)
include_directories(${PROJECT_SOURCE_DIR}/include)

add_library(calc
    lib/test1.cpp
    lib/test2.cpp
)

add_executable(${PROJECT_NAME} ${SRC_LIST})
target_link_libraries(${PROJECT_NAME} PRIVATE calc)
#2.0
#3.0
#morning change one
