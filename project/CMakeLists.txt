cmake_minimum_required (VERSION 3.1)

set(CODEC_TYPE h264)

set(APP_NAME ${CODEC_TYPE}.codec)

set(CMAKE_CXX_COMPILER g++)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_CXX_EXTENSIONS OFF)

project (${APP_NAME})

#include_directories(${CMAKE_SOURCE_DIR}/libraries/your_project_dependencies)
#link_directories(${CMAKE_SOURCE_DIR}/libraries/your_project_dependencies)

set (EXTRA_LIBS ${EXTRA_LIBS})

add_executable(${APP_NAME} src/main.cpp)
target_link_libraries (${APP_NAME} ${EXTRA_LIBS})
