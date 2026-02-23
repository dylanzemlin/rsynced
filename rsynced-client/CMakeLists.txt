cmake_minimum_required(VERSION 3.25)

project(rsynced-client
    VERSION 0.1.0
    LANGUAGES CXX
)

set(CMAKE_CXX_STANDARD 23)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_CXX_EXTENSIONS OFF)

add_subdirectory(src)

option(BUILD_TESTING "Enable tests" ON)
if(BUILD_TESTING)
    enable_testing()
    add_subdirectory(tests)
endif()