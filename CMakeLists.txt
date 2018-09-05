cmake_minimum_required(VERSION 3.5)
project(threadPool)

set(EXECUTABLE_OUTPUT_PATH ${PROJECT_SOURCE_DIR}/build)

add_compile_options(-fPIC)
add_definitions(-DDEBUG_ERR -DDEBUG_INFO)
set(CMAKE_BUILD_TYPE debug)

add_subdirectory(ThreadPoolCpp98)
add_subdirectory(ThreadPoolCpp03)
add_subdirectory(ThreadPoolCpp11)