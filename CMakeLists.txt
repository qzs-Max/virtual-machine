cmake_minimum_required(VERSION 3.10)
project(outCMakeTest)
set(EXECUTABLE_OUTPUT_PATH ${PROJECT_SOURCE_DIR}/bin)
aux_source_directory(${PROJECT_SOURCE_DIR}/src SRC_LIST)
include_directories(${PROJECT_SOURCE_DIR}/include)

# add_library(calc ${PROJECT_SOURCE_DIR})
link_directories(${CMAKE_CURRENT_SOURCE_DIR}/lib)
link_libraries(calc)


add_executable(${PROJECT_NAME} ${SRC_LIST})
#2.0
#3.0
#morning change one
